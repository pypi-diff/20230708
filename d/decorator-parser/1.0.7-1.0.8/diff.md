# Comparing `tmp/decorator_parser-1.0.7-py3-none-any.whl.zip` & `tmp/decorator_parser-1.0.8-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 5760 bytes, number of entries: 9
+Zip file size: 5769 bytes, number of entries: 9
 -rw-r--r--  2.0 unx       65 b- defN 23-Jul-08 10:37 decorator_parser/__init__.py
--rw-r--r--  2.0 unx     1093 b- defN 23-Jun-25 15:50 decorator_parser/errors.py
+-rw-r--r--  2.0 unx     1110 b- defN 23-Jul-08 10:42 decorator_parser/errors.py
 -rw-r--r--  2.0 unx     4226 b- defN 23-Jul-08 10:32 decorator_parser/parse.py
 -rw-r--r--  2.0 unx      240 b- defN 23-Jun-25 15:50 decorator_parser/utils.py
--rw-r--r--  2.0 unx      519 b- defN 23-Jul-08 10:38 decorator_parser-1.0.7.dist-info/LICENSE
--rw-r--r--  2.0 unx     4165 b- defN 23-Jul-08 10:38 decorator_parser-1.0.7.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-08 10:38 decorator_parser-1.0.7.dist-info/WHEEL
--rw-r--r--  2.0 unx       17 b- defN 23-Jul-08 10:38 decorator_parser-1.0.7.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      759 b- defN 23-Jul-08 10:38 decorator_parser-1.0.7.dist-info/RECORD
-9 files, 11176 bytes uncompressed, 4438 bytes compressed:  60.3%
+-rw-r--r--  2.0 unx      519 b- defN 23-Jul-08 10:44 decorator_parser-1.0.8.dist-info/LICENSE
+-rw-r--r--  2.0 unx     4165 b- defN 23-Jul-08 10:44 decorator_parser-1.0.8.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-08 10:44 decorator_parser-1.0.8.dist-info/WHEEL
+-rw-r--r--  2.0 unx       17 b- defN 23-Jul-08 10:44 decorator_parser-1.0.8.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      759 b- defN 23-Jul-08 10:44 decorator_parser-1.0.8.dist-info/RECORD
+9 files, 11193 bytes uncompressed, 4447 bytes compressed:  60.3%
```

## zipnote {}

```diff
@@ -6,23 +6,23 @@
 
 Filename: decorator_parser/parse.py
 Comment: 
 
 Filename: decorator_parser/utils.py
 Comment: 
 
-Filename: decorator_parser-1.0.7.dist-info/LICENSE
+Filename: decorator_parser-1.0.8.dist-info/LICENSE
 Comment: 
 
-Filename: decorator_parser-1.0.7.dist-info/METADATA
+Filename: decorator_parser-1.0.8.dist-info/METADATA
 Comment: 
 
-Filename: decorator_parser-1.0.7.dist-info/WHEEL
+Filename: decorator_parser-1.0.8.dist-info/WHEEL
 Comment: 
 
-Filename: decorator_parser-1.0.7.dist-info/top_level.txt
+Filename: decorator_parser-1.0.8.dist-info/top_level.txt
 Comment: 
 
-Filename: decorator_parser-1.0.7.dist-info/RECORD
+Filename: decorator_parser-1.0.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## decorator_parser/errors.py

```diff
@@ -1,13 +1,13 @@
 # Author: Michał Kostyk for Smartschool Inc.
 # Date: 2023
 # Version: 1.0.3
 # Description: Custom errors for the project.
 
-from utils import FAIL, ENDC, BOLD
+from decorator_parser.utils import FAIL, ENDC, BOLD
 
 def line_number(data, line):
     matches = data.split(line)
     return len(matches[0].split('\n'))
 
 
 # Exception class that adds coloring to the message
```

## Comparing `decorator_parser-1.0.7.dist-info/LICENSE` & `decorator_parser-1.0.8.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `decorator_parser-1.0.7.dist-info/METADATA` & `decorator_parser-1.0.8.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: decorator-parser
-Version: 1.0.7
+Version: 1.0.8
 Summary: Parser for text files with decorators into Python dictionaries
 Author-email: Michal Kostyk <m.kostyk22@gmail.com>
 Project-URL: Homepage, https://github.com/mkostyk/decorators-parser
 Project-URL: Bug Tracker, https://github.com/mkostyk/decorators-parser/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

## Comparing `decorator_parser-1.0.7.dist-info/RECORD` & `decorator_parser-1.0.8.dist-info/RECORD`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 decorator_parser/__init__.py,sha256=s-3LiX7ek2uhD5vfP-9cJRJIUCZ-3Fyr7mPttPzfgWQ,65
-decorator_parser/errors.py,sha256=2o9vv3ek_25pCt5Nmy1qID7wSkiBjjPK0jR9G_epyzE,1093
+decorator_parser/errors.py,sha256=GefbMbWrJ6yVR-WK-34XbICH31wZKwLzAbwrfZW4vy8,1110
 decorator_parser/parse.py,sha256=3P_SJ-exiEmrfVZxXB5cWEDt6WZzZg0muDSSJBPb5gU,4226
 decorator_parser/utils.py,sha256=83D2giM9d645tGZDPI27sWRN-zkiJn82CYHbPDBlqbA,240
-decorator_parser-1.0.7.dist-info/LICENSE,sha256=d0IchUxRoZd6yiEkgwlRF6MEDtdQLuG3CiDQolTTkw8,519
-decorator_parser-1.0.7.dist-info/METADATA,sha256=7H3iPhbBABXvnfQJcEIjvnBbKPgUUWAl2NBbKUpmLUw,4165
-decorator_parser-1.0.7.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-decorator_parser-1.0.7.dist-info/top_level.txt,sha256=wp3MzzKLv5-NNCQtdxjJPnk80INShwww5TfQfiIj95M,17
-decorator_parser-1.0.7.dist-info/RECORD,,
+decorator_parser-1.0.8.dist-info/LICENSE,sha256=d0IchUxRoZd6yiEkgwlRF6MEDtdQLuG3CiDQolTTkw8,519
+decorator_parser-1.0.8.dist-info/METADATA,sha256=pKul1X8PspC_-eOfijPDLJhKde0Fw3ju8ehC3tRrEeQ,4165
+decorator_parser-1.0.8.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+decorator_parser-1.0.8.dist-info/top_level.txt,sha256=wp3MzzKLv5-NNCQtdxjJPnk80INShwww5TfQfiIj95M,17
+decorator_parser-1.0.8.dist-info/RECORD,,
```

