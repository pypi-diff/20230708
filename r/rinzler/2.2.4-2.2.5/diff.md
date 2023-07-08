# Comparing `tmp/rinzler-2.2.4.tar.gz` & `tmp/rinzler-2.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/rinzler-2.2.4.tar", last modified: Tue Jul  7 13:16:45 2020, max compression
+gzip compressed data, was "dist/rinzler-2.2.5.tar", last modified: Thu Oct 15 19:44:33 2020, max compression
```

## Comparing `rinzler-2.2.4.tar` & `rinzler-2.2.5.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 andre      (501) staff       (20)        0 2020-07-07 13:16:45.000000 rinzler-2.2.4/
--rw-r--r--   0 andre      (501) staff       (20)     5304 2020-07-07 13:16:45.000000 rinzler-2.2.4/PKG-INFO
-drwxr-xr-x   0 andre      (501) staff       (20)        0 2020-07-07 13:16:45.000000 rinzler-2.2.4/rinzler/
-drwxr-xr-x   0 andre      (501) staff       (20)        0 2020-07-07 13:16:45.000000 rinzler-2.2.4/rinzler/core/
--rw-r--r--   0 andre      (501) staff       (20)     2934 2020-07-06 21:01:03.000000 rinzler-2.2.4/rinzler/core/route_mapping.py
--rw-r--r--   0 andre      (501) staff       (20)      173 2020-07-06 21:00:55.000000 rinzler-2.2.4/rinzler/core/request.py
--rw-r--r--   0 andre      (501) staff       (20)        0 2019-01-07 18:44:35.000000 rinzler-2.2.4/rinzler/core/__init__.py
--rw-r--r--   0 andre      (501) staff       (20)     1739 2020-07-06 21:00:55.000000 rinzler-2.2.4/rinzler/core/response.py
--rw-r--r--   0 andre      (501) staff       (20)      557 2020-07-06 21:00:55.000000 rinzler-2.2.4/rinzler/core/main_controller.py
-drwxr-xr-x   0 andre      (501) staff       (20)        0 2020-07-07 13:16:45.000000 rinzler-2.2.4/rinzler/logger/
--rw-r--r--   0 andre      (501) staff       (20)      500 2019-01-07 18:44:35.000000 rinzler-2.2.4/rinzler/logger/log.py
--rw-r--r--   0 andre      (501) staff       (20)     1761 2019-01-07 18:44:35.000000 rinzler-2.2.4/rinzler/logger/__init__.py
-drwxr-xr-x   0 andre      (501) staff       (20)        0 2020-07-07 13:16:45.000000 rinzler-2.2.4/rinzler/auth/
--rw-r--r--   0 andre      (501) staff       (20)        0 2020-07-06 21:00:55.000000 rinzler-2.2.4/rinzler/auth/__init__.py
--rw-r--r--   0 andre      (501) staff       (20)      756 2020-07-06 21:08:08.000000 rinzler-2.2.4/rinzler/auth/base_auth_service.py
--rw-r--r--   0 andre      (501) staff       (20)    16827 2020-07-06 21:28:18.000000 rinzler-2.2.4/rinzler/__init__.py
-drwxr-xr-x   0 andre      (501) staff       (20)        0 2020-07-07 13:16:45.000000 rinzler-2.2.4/rinzler/exceptions/
--rw-r--r--   0 andre      (501) staff       (20)      615 2020-07-06 21:00:55.000000 rinzler-2.2.4/rinzler/exceptions/precondition_required_exception.py
--rw-r--r--   0 andre      (501) staff       (20)      343 2020-07-06 21:00:55.000000 rinzler-2.2.4/rinzler/exceptions/unauthorized_exception.py
--rw-r--r--   0 andre      (501) staff       (20)      372 2020-07-06 21:00:55.000000 rinzler-2.2.4/rinzler/exceptions/not_found_exception.py
--rw-r--r--   0 andre      (501) staff       (20)      377 2020-07-06 21:00:55.000000 rinzler-2.2.4/rinzler/exceptions/failed_dependency_exception.py
--rw-r--r--   0 andre      (501) staff       (20)      443 2020-07-06 21:00:55.000000 rinzler-2.2.4/rinzler/exceptions/expectation_failed_exception.py
--rw-r--r--   0 andre      (501) staff       (20)      432 2020-07-06 21:00:55.000000 rinzler-2.2.4/rinzler/exceptions/unacceptable_input_exception.py
--rw-r--r--   0 andre      (501) staff       (20)      400 2020-07-06 21:00:55.000000 rinzler-2.2.4/rinzler/exceptions/conflict_exception.py
--rw-r--r--   0 andre      (501) staff       (20)      371 2020-07-06 21:00:55.000000 rinzler-2.2.4/rinzler/exceptions/internal_exception.py
--rw-r--r--   0 andre      (501) staff       (20)      613 2020-07-06 21:00:55.000000 rinzler-2.2.4/rinzler/exceptions/__init__.py
--rw-r--r--   0 andre      (501) staff       (20)      434 2020-07-06 21:00:55.000000 rinzler-2.2.4/rinzler/exceptions/precondition_failed_exception.py
--rw-r--r--   0 andre      (501) staff       (20)      400 2020-07-06 21:00:55.000000 rinzler-2.2.4/rinzler/exceptions/invalid_input_exception.py
--rw-r--r--   0 andre      (501) staff       (20)      363 2020-07-06 21:00:55.000000 rinzler-2.2.4/rinzler/exceptions/not_allowed_exception.py
--rw-r--r--   0 andre      (501) staff       (20)      395 2020-07-06 21:00:55.000000 rinzler-2.2.4/rinzler/exceptions/gone_exception.py
--rw-r--r--   0 andre      (501) staff       (20)      393 2020-07-06 21:00:55.000000 rinzler-2.2.4/rinzler/exceptions/service_unavailable_exception.py
--rw-r--r--   0 andre      (501) staff       (20)      378 2020-07-06 21:00:55.000000 rinzler-2.2.4/rinzler/exceptions/content_too_large_exception.py
--rw-r--r--   0 andre      (501) staff       (20)      261 2020-07-06 21:00:55.000000 rinzler-2.2.4/rinzler/exceptions/i_am_a_teapot_exception.py
--rw-r--r--   0 andre      (501) staff       (20)      324 2020-07-06 21:00:55.000000 rinzler-2.2.4/rinzler/exceptions/auth_exception.py
--rw-r--r--   0 andre      (501) staff       (20)       47 2019-01-07 18:44:35.000000 rinzler-2.2.4/MANIFEST.in
--rw-r--r--   0 andre      (501) staff       (20)     3318 2019-01-07 18:44:35.000000 rinzler-2.2.4/README.md
--rw-r--r--   0 andre      (501) staff       (20)     3134 2020-07-06 21:01:03.000000 rinzler-2.2.4/setup.py
--rw-r--r--   0 andre      (501) staff       (20)       38 2020-07-07 13:16:45.000000 rinzler-2.2.4/setup.cfg
-drwxr-xr-x   0 andre      (501) staff       (20)        0 2020-07-07 13:16:45.000000 rinzler-2.2.4/rinzler.egg-info/
--rw-r--r--   0 andre      (501) staff       (20)     5304 2020-07-07 13:16:45.000000 rinzler-2.2.4/rinzler.egg-info/PKG-INFO
--rw-r--r--   0 andre      (501) staff       (20)     1230 2020-07-07 13:16:45.000000 rinzler-2.2.4/rinzler.egg-info/SOURCES.txt
--rw-r--r--   0 andre      (501) staff       (20)       81 2020-07-07 13:16:45.000000 rinzler-2.2.4/rinzler.egg-info/requires.txt
--rw-r--r--   0 andre      (501) staff       (20)        8 2020-07-07 13:16:45.000000 rinzler-2.2.4/rinzler.egg-info/top_level.txt
--rw-r--r--   0 andre      (501) staff       (20)        1 2020-07-07 13:16:45.000000 rinzler-2.2.4/rinzler.egg-info/dependency_links.txt
--rw-r--r--   0 andre      (501) staff       (20)     1080 2019-01-07 18:44:35.000000 rinzler-2.2.4/LICENSE.txt
+drwxr-xr-x   0 andreleite   (501) staff       (20)        0 2020-10-15 19:44:33.000000 rinzler-2.2.5/
+-rw-r--r--   0 andreleite   (501) staff       (20)     5304 2020-10-15 19:44:33.000000 rinzler-2.2.5/PKG-INFO
+drwxr-xr-x   0 andreleite   (501) staff       (20)        0 2020-10-15 19:44:33.000000 rinzler-2.2.5/rinzler/
+drwxr-xr-x   0 andreleite   (501) staff       (20)        0 2020-10-15 19:44:33.000000 rinzler-2.2.5/rinzler/core/
+-rw-r--r--   0 andreleite   (501) staff       (20)     2934 2020-10-15 19:35:45.000000 rinzler-2.2.5/rinzler/core/route_mapping.py
+-rw-r--r--   0 andreleite   (501) staff       (20)      173 2020-10-15 19:35:45.000000 rinzler-2.2.5/rinzler/core/request.py
+-rwxrwxrwx   0 andreleite   (501) staff       (20)        0 2019-01-07 18:44:34.000000 rinzler-2.2.5/rinzler/core/__init__.py
+-rw-r--r--   0 andreleite   (501) staff       (20)     1845 2020-10-15 19:35:45.000000 rinzler-2.2.5/rinzler/core/response.py
+-rw-r--r--   0 andreleite   (501) staff       (20)      557 2020-10-15 19:35:45.000000 rinzler-2.2.5/rinzler/core/main_controller.py
+drwxr-xr-x   0 andreleite   (501) staff       (20)        0 2020-10-15 19:44:33.000000 rinzler-2.2.5/rinzler/logger/
+-rwxrwxrwx   0 andreleite   (501) staff       (20)      500 2019-01-07 18:44:34.000000 rinzler-2.2.5/rinzler/logger/log.py
+-rwxrwxrwx   0 andreleite   (501) staff       (20)     1761 2019-01-07 18:44:34.000000 rinzler-2.2.5/rinzler/logger/__init__.py
+drwxr-xr-x   0 andreleite   (501) staff       (20)        0 2020-10-15 19:44:33.000000 rinzler-2.2.5/rinzler/auth/
+-rw-r--r--   0 andreleite   (501) staff       (20)        0 2020-10-15 19:35:45.000000 rinzler-2.2.5/rinzler/auth/__init__.py
+-rw-r--r--   0 andreleite   (501) staff       (20)      756 2020-10-15 19:35:45.000000 rinzler-2.2.5/rinzler/auth/base_auth_service.py
+-rw-r--r--   0 andreleite   (501) staff       (20)    16827 2020-10-15 19:35:45.000000 rinzler-2.2.5/rinzler/__init__.py
+drwxr-xr-x   0 andreleite   (501) staff       (20)        0 2020-10-15 19:44:33.000000 rinzler-2.2.5/rinzler/exceptions/
+-rw-r--r--   0 andreleite   (501) staff       (20)      615 2020-10-15 19:35:45.000000 rinzler-2.2.5/rinzler/exceptions/precondition_required_exception.py
+-rw-r--r--   0 andreleite   (501) staff       (20)      343 2020-10-15 19:35:45.000000 rinzler-2.2.5/rinzler/exceptions/unauthorized_exception.py
+-rw-r--r--   0 andreleite   (501) staff       (20)      372 2020-10-15 19:35:45.000000 rinzler-2.2.5/rinzler/exceptions/not_found_exception.py
+-rw-r--r--   0 andreleite   (501) staff       (20)      377 2020-10-15 19:35:45.000000 rinzler-2.2.5/rinzler/exceptions/failed_dependency_exception.py
+-rw-r--r--   0 andreleite   (501) staff       (20)      443 2020-10-15 19:35:45.000000 rinzler-2.2.5/rinzler/exceptions/expectation_failed_exception.py
+-rw-r--r--   0 andreleite   (501) staff       (20)      432 2020-10-15 19:35:45.000000 rinzler-2.2.5/rinzler/exceptions/unacceptable_input_exception.py
+-rw-r--r--   0 andreleite   (501) staff       (20)      400 2020-10-15 19:35:45.000000 rinzler-2.2.5/rinzler/exceptions/conflict_exception.py
+-rw-r--r--   0 andreleite   (501) staff       (20)      371 2020-10-15 19:35:45.000000 rinzler-2.2.5/rinzler/exceptions/internal_exception.py
+-rw-r--r--   0 andreleite   (501) staff       (20)      613 2020-10-15 19:35:45.000000 rinzler-2.2.5/rinzler/exceptions/__init__.py
+-rw-r--r--   0 andreleite   (501) staff       (20)      434 2020-10-15 19:35:45.000000 rinzler-2.2.5/rinzler/exceptions/precondition_failed_exception.py
+-rw-r--r--   0 andreleite   (501) staff       (20)      400 2020-10-15 19:35:45.000000 rinzler-2.2.5/rinzler/exceptions/invalid_input_exception.py
+-rw-r--r--   0 andreleite   (501) staff       (20)      363 2020-10-15 19:35:45.000000 rinzler-2.2.5/rinzler/exceptions/not_allowed_exception.py
+-rw-r--r--   0 andreleite   (501) staff       (20)      395 2020-10-15 19:35:45.000000 rinzler-2.2.5/rinzler/exceptions/gone_exception.py
+-rw-r--r--   0 andreleite   (501) staff       (20)      393 2020-10-15 19:35:45.000000 rinzler-2.2.5/rinzler/exceptions/service_unavailable_exception.py
+-rw-r--r--   0 andreleite   (501) staff       (20)      378 2020-10-15 19:35:45.000000 rinzler-2.2.5/rinzler/exceptions/content_too_large_exception.py
+-rw-r--r--   0 andreleite   (501) staff       (20)      261 2020-10-15 19:35:45.000000 rinzler-2.2.5/rinzler/exceptions/i_am_a_teapot_exception.py
+-rw-r--r--   0 andreleite   (501) staff       (20)      324 2020-10-15 19:35:45.000000 rinzler-2.2.5/rinzler/exceptions/auth_exception.py
+-rwxrwxrwx   0 andreleite   (501) staff       (20)       47 2019-01-07 18:44:34.000000 rinzler-2.2.5/MANIFEST.in
+-rwxrwxrwx   0 andreleite   (501) staff       (20)     3318 2019-01-07 18:44:34.000000 rinzler-2.2.5/README.md
+-rw-r--r--   0 andreleite   (501) staff       (20)     3134 2020-10-15 19:35:45.000000 rinzler-2.2.5/setup.py
+-rw-r--r--   0 andreleite   (501) staff       (20)       38 2020-10-15 19:44:33.000000 rinzler-2.2.5/setup.cfg
+drwxr-xr-x   0 andreleite   (501) staff       (20)        0 2020-10-15 19:44:33.000000 rinzler-2.2.5/rinzler.egg-info/
+-rwxrwxrwx   0 andreleite   (501) staff       (20)     5304 2020-10-15 19:44:32.000000 rinzler-2.2.5/rinzler.egg-info/PKG-INFO
+-rwxrwxrwx   0 andreleite   (501) staff       (20)     1230 2020-10-15 19:44:33.000000 rinzler-2.2.5/rinzler.egg-info/SOURCES.txt
+-rwxrwxrwx   0 andreleite   (501) staff       (20)       81 2020-10-15 19:44:32.000000 rinzler-2.2.5/rinzler.egg-info/requires.txt
+-rwxrwxrwx   0 andreleite   (501) staff       (20)        8 2020-10-15 19:44:32.000000 rinzler-2.2.5/rinzler.egg-info/top_level.txt
+-rwxrwxrwx   0 andreleite   (501) staff       (20)        1 2020-10-15 19:44:32.000000 rinzler-2.2.5/rinzler.egg-info/dependency_links.txt
+-rwxrwxrwx   0 andreleite   (501) staff       (20)     1080 2019-01-07 18:44:34.000000 rinzler-2.2.5/LICENSE.txt
```

### Comparing `rinzler-2.2.4/PKG-INFO` & `rinzler-2.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rinzler
-Version: 2.2.4
+Version: 2.2.5
 Summary: Django-based REST API Framework
 Home-page: https://github.com/feliphebueno/Rinzler
 Author: Rinzler
 Author-email: feliphezion@gmail.com
 License: MIT
 Description: # Rinzler REST Framework
```

### Comparing `rinzler-2.2.4/rinzler/core/route_mapping.py` & `rinzler-2.2.5/rinzler/core/route_mapping.py`

 * *Files identical despite different names*

### Comparing `rinzler-2.2.4/rinzler/core/response.py` & `rinzler-2.2.5/rinzler/core/response.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 """
 Interface for HttpResponse
 """
 __author__ = "Rinzler<github.com/feliphebueno>"
 
 import json
 from collections import OrderedDict
+
+from django.core.serializers.json import DjangoJSONEncoder
 from django.http.response import HttpResponse
 
 
 class Response(object):
     """
     Response
     """
@@ -41,20 +43,20 @@
         return HttpResponse(
             str(self), content_type=self.__content_type, charset=self.__charset, **self.__kwargs
         )
 
     def __str__(self):
         if self.__indent > 0:
             if self.__content is not None:
-                return json.dumps(self.__content, indent=self.__indent, sort_keys=False)
+                return json.dumps(self.__content, indent=self.__indent, sort_keys=False, cls=DjangoJSONEncoder)
             else:
                 return str()
         else:
             if self.__content is not None:
-                return json.dumps(self.__content, sort_keys=False)
+                return json.dumps(self.__content, sort_keys=False, cls=DjangoJSONEncoder)
             else:
                 return str()
 
     def __repr__(self):
         return self.__str__()
 
     def get_decoded(self):
```

### Comparing `rinzler-2.2.4/rinzler/core/main_controller.py` & `rinzler-2.2.5/rinzler/core/main_controller.py`

 * *Files identical despite different names*

### Comparing `rinzler-2.2.4/rinzler/logger/__init__.py` & `rinzler-2.2.5/rinzler/logger/__init__.py`

 * *Files identical despite different names*

### Comparing `rinzler-2.2.4/rinzler/auth/base_auth_service.py` & `rinzler-2.2.5/rinzler/auth/base_auth_service.py`

 * *Files identical despite different names*

### Comparing `rinzler-2.2.4/rinzler/__init__.py` & `rinzler-2.2.5/rinzler/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 Main
 """
 from typing import Union, Tuple, List, Dict, Any
 
 from django.core.exceptions import RequestDataTooBig
 
 __name__ = "Rinzler REST Framework"
-__version__ = "2.2.4"
+__version__ = "2.2.5"
 __author__ = ["Rinzler<github.com/feliphebueno>", "4ndr<github.com/4ndr>"]
 
 import os
 import re
 from datetime import datetime
 from collections import OrderedDict
 from logging import Logger, getLogger
```

### Comparing `rinzler-2.2.4/rinzler/exceptions/precondition_required_exception.py` & `rinzler-2.2.5/rinzler/exceptions/precondition_required_exception.py`

 * *Files identical despite different names*

### Comparing `rinzler-2.2.4/rinzler/exceptions/__init__.py` & `rinzler-2.2.5/rinzler/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `rinzler-2.2.4/README.md` & `rinzler-2.2.5/README.md`

 * *Files identical despite different names*

### Comparing `rinzler-2.2.4/setup.py` & `rinzler-2.2.5/setup.py`

 * *Files identical despite different names*

### Comparing `rinzler-2.2.4/rinzler.egg-info/PKG-INFO` & `rinzler-2.2.5/rinzler.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rinzler
-Version: 2.2.4
+Version: 2.2.5
 Summary: Django-based REST API Framework
 Home-page: https://github.com/feliphebueno/Rinzler
 Author: Rinzler
 Author-email: feliphezion@gmail.com
 License: MIT
 Description: # Rinzler REST Framework
```

### Comparing `rinzler-2.2.4/rinzler.egg-info/SOURCES.txt` & `rinzler-2.2.5/rinzler.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rinzler-2.2.4/LICENSE.txt` & `rinzler-2.2.5/LICENSE.txt`

 * *Files identical despite different names*

