# Comparing `tmp/prestashop-0.1.1-py3-none-any.whl.zip` & `tmp/prestashop-0.1.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 20600 bytes, number of entries: 10
+Zip file size: 20860 bytes, number of entries: 10
 -rw-r--r--  2.0 unx      149 b- defN 23-Jun-13 13:52 prestashop/__init__.py
--rw-r--r--  2.0 unx    14548 b- defN 23-Jun-13 18:25 prestashop/core.py
+-rw-r--r--  2.0 unx    14998 b- defN 23-Jul-08 12:05 prestashop/core.py
 -rw-r--r--  2.0 unx      660 b- defN 23-Jun-12 13:23 prestashop/exceptions.py
--rw-r--r--  2.0 unx     3642 b- defN 23-Jun-10 13:45 prestashop/utils.py
--rw-r--r--  2.0 unx      102 b- defN 23-Jun-13 18:52 prestashop/version.py
--rw-r--r--  2.0 unx    35149 b- defN 23-Jun-13 18:54 prestashop-0.1.1.dist-info/LICENSE
--rw-r--r--  2.0 unx     3597 b- defN 23-Jun-13 18:54 prestashop-0.1.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-13 18:54 prestashop-0.1.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       11 b- defN 23-Jun-13 18:54 prestashop-0.1.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      789 b- defN 23-Jun-13 18:54 prestashop-0.1.1.dist-info/RECORD
-10 files, 58739 bytes uncompressed, 19262 bytes compressed:  67.2%
+-rw-r--r--  2.0 unx     3955 b- defN 23-Jul-08 12:03 prestashop/utils.py
+-rw-r--r--  2.0 unx      102 b- defN 23-Jul-07 12:41 prestashop/version.py
+-rw-r--r--  2.0 unx    35149 b- defN 23-Jul-08 12:12 prestashop-0.1.2.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3597 b- defN 23-Jul-08 12:12 prestashop-0.1.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-08 12:12 prestashop-0.1.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       11 b- defN 23-Jul-08 12:12 prestashop-0.1.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      789 b- defN 23-Jul-08 12:12 prestashop-0.1.2.dist-info/RECORD
+10 files, 59502 bytes uncompressed, 19522 bytes compressed:  67.2%
```

## zipnote {}

```diff
@@ -9,23 +9,23 @@
 
 Filename: prestashop/utils.py
 Comment: 
 
 Filename: prestashop/version.py
 Comment: 
 
-Filename: prestashop-0.1.1.dist-info/LICENSE
+Filename: prestashop-0.1.2.dist-info/LICENSE
 Comment: 
 
-Filename: prestashop-0.1.1.dist-info/METADATA
+Filename: prestashop-0.1.2.dist-info/METADATA
 Comment: 
 
-Filename: prestashop-0.1.1.dist-info/WHEEL
+Filename: prestashop-0.1.2.dist-info/WHEEL
 Comment: 
 
-Filename: prestashop-0.1.1.dist-info/top_level.txt
+Filename: prestashop-0.1.2.dist-info/top_level.txt
 Comment: 
 
-Filename: prestashop-0.1.1.dist-info/RECORD
+Filename: prestashop-0.1.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## prestashop/core.py

```diff
@@ -5,25 +5,27 @@
 
 :copyright: (c) 2023 Aymen Jemi
 :copyright: (c) 2023 AISYSNEXT
 :license: GPLv3, see LICENSE for more details
 """
 import os
 from enum import Enum
-import mimetypes
+
 
 from http.client import HTTPConnection
 from xml.etree import ElementTree
 from xml.parsers.expat import ExpatError
 
 from requests import Session
 from requests.models import PreparedRequest
 
 from .exceptions import PrestaShopError,PrestaShopAuthenticationError
 from .utils import dict2xml
+from .utils import base64_to_tmpfile
+
 
 class Format(Enum):
     """Data types return (JSON,XML)
 
     Args:
         Enum (int): 1 => JSON, 2 => XML
     """
@@ -92,14 +94,20 @@
 
     # search the first 3 taxes with 5 in the name 
     import pprint
     recs = api.search('taxes',_filter='[name]=%[5]%',limit='3')
 
     for rec in recs:
         pprint(rec)
+
+    # create binary (product image)
+
+    api.create_binary('images/products/22','img.jpeg','image')
+    # or
+    api.create_binary('images/products/22','img.jpeg','image')
     """
     api_key = ''
     url = ''
     client = None
     debug = False
     lang = None
     data_format = Format.JSON
@@ -412,21 +420,22 @@
         """
 
 
         data  = {'prestashop' : data}
         _data = dict2xml(data)
         return self._exec(resource=resource,data=_data,method='POST',display=None)
 
-    def create_binary(self,resource:str, file:str,_type:str = 'image'):
+    def create_binary(self,resource:str, file:str,_type:str = 'image',file_name=None):
         """create binary record
 
         Args:
-            resource (str): resource to search ( 'images/products/22' ...).
-            files (str):  a path of file ('image.png', 'image.jpg').
-            _type (str): a type of file (image,pdf ...)
+            resource (str): resource to add file ( 'images/products/22' ...).
+            files (str):  a path of file ('image.png', 'image.jpg') or binary.
+            _type (str, optional): a type of file (image,pdf ...) Default to 'image'
+            file_name (str, optinal): name of file in case of base64. Default to None
         """
 
         params = {}
 
         if self.lang:
             params.update({'language' : self.lang})
         
@@ -437,14 +446,17 @@
         _url = '{}{}'.format(self.url,resource)
         url = self._prepare(_url,params)
 
 
         if os.path.exists(file):
 
             _file = {_type : open(file,'rb')}
+
+        elif isinstance(file ,str):
+            _file = {_type : open(base64_to_tmpfile(file,file_name),'rb') }
         else:
             raise PrestaShopError('File not found',404)
 
 
         response = self.client.post(
             url=url,
             files=_file
```

## prestashop/utils.py

```diff
@@ -1,10 +1,14 @@
 from xml.dom.minidom import getDOMImplementation
 from builtins import str
 from past.types import basestring
+import base64
+import tempfile
+import mimetypes
+import os
 
 
 def _process(doc, tag, tag_value):
     """
     Generate dom object for tag: tag_value
 
     @param doc: xml doc
@@ -107,7 +111,18 @@
     """
     doc = getDOMImplementation().createDocument(None, None, None)
     if len(data) > 1:
         raise Exception('Only one root node allowed')
     root, _ = _process_complex(doc, list(data.items()))
     doc.appendChild(root[0])
     return doc.toxml(encoding)
+
+def base64_to_tmpfile(content,file_name):
+    _,ext = os.path.splitext(file_name)
+    path = ''
+    with  tempfile.NamedTemporaryFile(delete=False,suffix=ext) as tmp:
+        tmp.write(base64.b64decode(content))
+        path = tmp.name
+
+    return path
+
+
```

## prestashop/version.py

```diff
@@ -1,3 +1,3 @@
 # -*- coding: utf-8 -*-
-__version__="0.1.1"
+__version__="0.1.2"
 __author__="Aymen Jemi <jemiaymen@gmail.com> (AISYSNEXT)"
```

## Comparing `prestashop-0.1.1.dist-info/LICENSE` & `prestashop-0.1.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `prestashop-0.1.1.dist-info/METADATA` & `prestashop-0.1.2.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prestashop
-Version: 0.1.1
+Version: 0.1.2
 Summary: Prestashop is a library for Python to interact with the PrestaShop's Web Service API.
 Home-page: https://github.com/AiSyS-Next/prestashop
 Author: Aymen Jemi <jemiaymen@gmail.com> (AISYSNEXT)
 Author-email: jemiaymen@gmail.com
 License: GNU GPL-3
 Keywords: prestashop,e-com,e-commerce,prestashop api,api,webservice
 Classifier: Programming Language :: Python
```

## Comparing `prestashop-0.1.1.dist-info/RECORD` & `prestashop-0.1.2.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 prestashop/__init__.py,sha256=a6LT2Hg7nHgalB_KMPQ-Anch5Eld8tiWfbinewQ3mTQ,149
-prestashop/core.py,sha256=uu1L6xfB0b2WKwgvAJGrGDrV-apmf7emCqsFuIHJFkc,14548
+prestashop/core.py,sha256=fa2xv2-TWpTWxnY3n_dmQWwlkJQ6BFF2Nxlwhwu3U7Y,14998
 prestashop/exceptions.py,sha256=eQdfgz7bCB5p9IiNsGEJHnB0ojVA1UQtMKy9yR3qlZ8,660
-prestashop/utils.py,sha256=iQ8MKyhYJH3rjG7-WqCNklHno-eGOEGaH7GkBvhjGng,3642
-prestashop/version.py,sha256=ClOuEjoMIpZZ82BTtd0DYW6sYv_JREqYaoW6qWFSx_Q,102
-prestashop-0.1.1.dist-info/LICENSE,sha256=OXLcl0T2SZ8Pmy2_dmlvKuetivmyPd5m1q-Gyd-zaYY,35149
-prestashop-0.1.1.dist-info/METADATA,sha256=KztpQ86_V1j2kGHQvJCj-ghpQyfQ5mTZXzygc40vs6Y,3597
-prestashop-0.1.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-prestashop-0.1.1.dist-info/top_level.txt,sha256=ERBv-4esnLO-q9c0lGE1TpfzzCT-075zZJAClhwIVbA,11
-prestashop-0.1.1.dist-info/RECORD,,
+prestashop/utils.py,sha256=qreJqL9t8o9ur3AyyHjF-Tb2q6OsKDdi7EjieUu8hFY,3955
+prestashop/version.py,sha256=5zu2ny7nYFfXZzSamXN3peaHvMj8I56pNiTYATgTcuc,102
+prestashop-0.1.2.dist-info/LICENSE,sha256=OXLcl0T2SZ8Pmy2_dmlvKuetivmyPd5m1q-Gyd-zaYY,35149
+prestashop-0.1.2.dist-info/METADATA,sha256=qJZpH_y_wgE_pXOEwJ5oCWvu7xiqw4I5IOyc-0IAVH4,3597
+prestashop-0.1.2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+prestashop-0.1.2.dist-info/top_level.txt,sha256=ERBv-4esnLO-q9c0lGE1TpfzzCT-075zZJAClhwIVbA,11
+prestashop-0.1.2.dist-info/RECORD,,
```

