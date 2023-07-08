# Comparing `tmp/decorator_parser-1.0.5-py3-none-any.whl.zip` & `tmp/decorator_parser-1.0.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 5716 bytes, number of entries: 9
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-25 14:21 decorator_parser/__init__.py
+Zip file size: 5763 bytes, number of entries: 9
+-rw-r--r--  2.0 unx       65 b- defN 23-Jul-08 10:31 decorator_parser/__init__.py
 -rw-r--r--  2.0 unx     1093 b- defN 23-Jun-25 15:50 decorator_parser/errors.py
--rw-r--r--  2.0 unx     4192 b- defN 23-Jul-08 10:19 decorator_parser/parse.py
+-rw-r--r--  2.0 unx     4226 b- defN 23-Jul-08 10:32 decorator_parser/parse.py
 -rw-r--r--  2.0 unx      240 b- defN 23-Jun-25 15:50 decorator_parser/utils.py
--rw-r--r--  2.0 unx      519 b- defN 23-Jul-08 10:19 decorator_parser-1.0.5.dist-info/LICENSE
--rw-r--r--  2.0 unx     4165 b- defN 23-Jul-08 10:19 decorator_parser-1.0.5.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-08 10:19 decorator_parser-1.0.5.dist-info/WHEEL
--rw-r--r--  2.0 unx       17 b- defN 23-Jul-08 10:19 decorator_parser-1.0.5.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      758 b- defN 23-Jul-08 10:19 decorator_parser-1.0.5.dist-info/RECORD
-9 files, 11076 bytes uncompressed, 4394 bytes compressed:  60.3%
+-rw-r--r--  2.0 unx      519 b- defN 23-Jul-08 10:33 decorator_parser-1.0.6.dist-info/LICENSE
+-rw-r--r--  2.0 unx     4165 b- defN 23-Jul-08 10:33 decorator_parser-1.0.6.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-08 10:33 decorator_parser-1.0.6.dist-info/WHEEL
+-rw-r--r--  2.0 unx       17 b- defN 23-Jul-08 10:33 decorator_parser-1.0.6.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      759 b- defN 23-Jul-08 10:33 decorator_parser-1.0.6.dist-info/RECORD
+9 files, 11176 bytes uncompressed, 4441 bytes compressed:  60.3%
```

## zipnote {}

```diff
@@ -6,23 +6,23 @@
 
 Filename: decorator_parser/parse.py
 Comment: 
 
 Filename: decorator_parser/utils.py
 Comment: 
 
-Filename: decorator_parser-1.0.5.dist-info/LICENSE
+Filename: decorator_parser-1.0.6.dist-info/LICENSE
 Comment: 
 
-Filename: decorator_parser-1.0.5.dist-info/METADATA
+Filename: decorator_parser-1.0.6.dist-info/METADATA
 Comment: 
 
-Filename: decorator_parser-1.0.5.dist-info/WHEEL
+Filename: decorator_parser-1.0.6.dist-info/WHEEL
 Comment: 
 
-Filename: decorator_parser-1.0.5.dist-info/top_level.txt
+Filename: decorator_parser-1.0.6.dist-info/top_level.txt
 Comment: 
 
-Filename: decorator_parser-1.0.5.dist-info/RECORD
+Filename: decorator_parser-1.0.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## decorator_parser/__init__.py

```diff
@@ -0,0 +1,5 @@
+00000000: 6672 6f6d 2065 7272 6f72 7320 696d 706f  from errors impo
+00000010: 7274 202a 0a66 726f 6d20 7574 696c 7320  rt *.from utils 
+00000020: 696d 706f 7274 202a 0a66 726f 6d20 7061  import *.from pa
+00000030: 7273 6520 696d 706f 7274 2050 6172 7365  rse import Parse
+00000040: 72                                       r
```

## decorator_parser/parse.py

```diff
@@ -1,13 +1,13 @@
 # Author: Michał Kostyk for Smartschool Inc.
 # Date: 2023
-# Version: 1.0.5
+# Version: 1.0.6
 
-from errors import *
-from utils import *
+from decorator_parser.utils import *
+from decorator_parser.errors import *
 import re
 
 
 class Parser:
     def __init__(self, constraints={}):
         for key in constraints:
             if not 'regex' in constraints[key] or not 'description' in constraints[key]:
```

## Comparing `decorator_parser-1.0.5.dist-info/LICENSE` & `decorator_parser-1.0.6.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `decorator_parser-1.0.5.dist-info/METADATA` & `decorator_parser-1.0.6.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: decorator-parser
-Version: 1.0.5
+Version: 1.0.6
 Summary: Parser for text files with decorators into Python dictionaries
 Author-email: Michal Kostyk <m.kostyk22@gmail.com>
 Project-URL: Homepage, https://github.com/mkostyk/decorators-parser
 Project-URL: Bug Tracker, https://github.com/mkostyk/decorators-parser/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

## Comparing `decorator_parser-1.0.5.dist-info/RECORD` & `decorator_parser-1.0.6.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-decorator_parser/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+decorator_parser/__init__.py,sha256=4ueunyha5_qZsz4ogAm2uGumu2zzxfgb9labs0c36DY,65
 decorator_parser/errors.py,sha256=2o9vv3ek_25pCt5Nmy1qID7wSkiBjjPK0jR9G_epyzE,1093
-decorator_parser/parse.py,sha256=6dhxHuBkUbuGFs4ql3FGPkRsHBgqdBlJdsZ3E9E9S5E,4192
+decorator_parser/parse.py,sha256=3P_SJ-exiEmrfVZxXB5cWEDt6WZzZg0muDSSJBPb5gU,4226
 decorator_parser/utils.py,sha256=83D2giM9d645tGZDPI27sWRN-zkiJn82CYHbPDBlqbA,240
-decorator_parser-1.0.5.dist-info/LICENSE,sha256=d0IchUxRoZd6yiEkgwlRF6MEDtdQLuG3CiDQolTTkw8,519
-decorator_parser-1.0.5.dist-info/METADATA,sha256=jgp_Sb_INbedX_DsN381xdgF11Dh4dAR_vVGThzuLnk,4165
-decorator_parser-1.0.5.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-decorator_parser-1.0.5.dist-info/top_level.txt,sha256=wp3MzzKLv5-NNCQtdxjJPnk80INShwww5TfQfiIj95M,17
-decorator_parser-1.0.5.dist-info/RECORD,,
+decorator_parser-1.0.6.dist-info/LICENSE,sha256=d0IchUxRoZd6yiEkgwlRF6MEDtdQLuG3CiDQolTTkw8,519
+decorator_parser-1.0.6.dist-info/METADATA,sha256=p6BEDDJipYnxQOI_EVCWi7VeWQ1D-jQe5Xw5CFWIDDM,4165
+decorator_parser-1.0.6.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+decorator_parser-1.0.6.dist-info/top_level.txt,sha256=wp3MzzKLv5-NNCQtdxjJPnk80INShwww5TfQfiIj95M,17
+decorator_parser-1.0.6.dist-info/RECORD,,
```

