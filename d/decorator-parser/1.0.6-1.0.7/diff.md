# Comparing `tmp/decorator_parser-1.0.6-py3-none-any.whl.zip` & `tmp/decorator_parser-1.0.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 5763 bytes, number of entries: 9
--rw-r--r--  2.0 unx       65 b- defN 23-Jul-08 10:31 decorator_parser/__init__.py
+Zip file size: 5760 bytes, number of entries: 9
+-rw-r--r--  2.0 unx       65 b- defN 23-Jul-08 10:37 decorator_parser/__init__.py
 -rw-r--r--  2.0 unx     1093 b- defN 23-Jun-25 15:50 decorator_parser/errors.py
 -rw-r--r--  2.0 unx     4226 b- defN 23-Jul-08 10:32 decorator_parser/parse.py
 -rw-r--r--  2.0 unx      240 b- defN 23-Jun-25 15:50 decorator_parser/utils.py
--rw-r--r--  2.0 unx      519 b- defN 23-Jul-08 10:33 decorator_parser-1.0.6.dist-info/LICENSE
--rw-r--r--  2.0 unx     4165 b- defN 23-Jul-08 10:33 decorator_parser-1.0.6.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-08 10:33 decorator_parser-1.0.6.dist-info/WHEEL
--rw-r--r--  2.0 unx       17 b- defN 23-Jul-08 10:33 decorator_parser-1.0.6.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      759 b- defN 23-Jul-08 10:33 decorator_parser-1.0.6.dist-info/RECORD
-9 files, 11176 bytes uncompressed, 4441 bytes compressed:  60.3%
+-rw-r--r--  2.0 unx      519 b- defN 23-Jul-08 10:38 decorator_parser-1.0.7.dist-info/LICENSE
+-rw-r--r--  2.0 unx     4165 b- defN 23-Jul-08 10:38 decorator_parser-1.0.7.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-08 10:38 decorator_parser-1.0.7.dist-info/WHEEL
+-rw-r--r--  2.0 unx       17 b- defN 23-Jul-08 10:38 decorator_parser-1.0.7.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      759 b- defN 23-Jul-08 10:38 decorator_parser-1.0.7.dist-info/RECORD
+9 files, 11176 bytes uncompressed, 4438 bytes compressed:  60.3%
```

## zipnote {}

```diff
@@ -6,23 +6,23 @@
 
 Filename: decorator_parser/parse.py
 Comment: 
 
 Filename: decorator_parser/utils.py
 Comment: 
 
-Filename: decorator_parser-1.0.6.dist-info/LICENSE
+Filename: decorator_parser-1.0.7.dist-info/LICENSE
 Comment: 
 
-Filename: decorator_parser-1.0.6.dist-info/METADATA
+Filename: decorator_parser-1.0.7.dist-info/METADATA
 Comment: 
 
-Filename: decorator_parser-1.0.6.dist-info/WHEEL
+Filename: decorator_parser-1.0.7.dist-info/WHEEL
 Comment: 
 
-Filename: decorator_parser-1.0.6.dist-info/top_level.txt
+Filename: decorator_parser-1.0.7.dist-info/top_level.txt
 Comment: 
 
-Filename: decorator_parser-1.0.6.dist-info/RECORD
+Filename: decorator_parser-1.0.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## decorator_parser/__init__.py

```diff
@@ -1,3 +1,3 @@
-from errors import *
-from utils import *
+from . import errors
+from . import utils
 from parse import Parser
```

## Comparing `decorator_parser-1.0.6.dist-info/LICENSE` & `decorator_parser-1.0.7.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `decorator_parser-1.0.6.dist-info/METADATA` & `decorator_parser-1.0.7.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: decorator-parser
-Version: 1.0.6
+Version: 1.0.7
 Summary: Parser for text files with decorators into Python dictionaries
 Author-email: Michal Kostyk <m.kostyk22@gmail.com>
 Project-URL: Homepage, https://github.com/mkostyk/decorators-parser
 Project-URL: Bug Tracker, https://github.com/mkostyk/decorators-parser/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

