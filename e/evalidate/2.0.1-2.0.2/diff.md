# Comparing `tmp/evalidate-2.0.1.tar.gz` & `tmp/evalidate-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "evalidate-2.0.1.tar", last modified: Thu Jun 22 14:47:46 2023, max compression
+gzip compressed data, was "evalidate-2.0.2.tar", last modified: Sat Jul  8 07:56:22 2023, max compression
```

## Comparing `evalidate-2.0.1.tar` & `evalidate-2.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 xenon     (1000) xenon     (1000)        0 2023-06-22 14:47:46.245852 evalidate-2.0.1/
--rw-r--r--   0 xenon     (1000) xenon     (1000)    12026 2023-06-22 14:47:46.245852 evalidate-2.0.1/PKG-INFO
--rw-r--r--   0 xenon     (1000) xenon     (1000)     9256 2023-06-21 21:43:38.000000 evalidate-2.0.1/README.md
-drwxr-xr-x   0 xenon     (1000) xenon     (1000)        0 2023-06-22 14:47:46.245852 evalidate-2.0.1/evalidate/
--rwxr-xr-x   0 xenon     (1000) xenon     (1000)     4083 2023-06-22 14:44:37.000000 evalidate-2.0.1/evalidate/__init__.py
--rw-r--r--   0 xenon     (1000) xenon     (1000)     2506 2023-06-21 21:43:38.000000 evalidate-2.0.1/evalidate/security.py
-drwxr-xr-x   0 xenon     (1000) xenon     (1000)        0 2023-06-22 14:47:46.245852 evalidate-2.0.1/evalidate.egg-info/
--rw-r--r--   0 xenon     (1000) xenon     (1000)    12026 2023-06-22 14:47:46.000000 evalidate-2.0.1/evalidate.egg-info/PKG-INFO
--rw-r--r--   0 xenon     (1000) xenon     (1000)      226 2023-06-22 14:47:46.000000 evalidate-2.0.1/evalidate.egg-info/SOURCES.txt
--rw-r--r--   0 xenon     (1000) xenon     (1000)        1 2023-06-22 14:47:46.000000 evalidate-2.0.1/evalidate.egg-info/dependency_links.txt
--rw-r--r--   0 xenon     (1000) xenon     (1000)        1 2022-08-10 17:45:22.000000 evalidate-2.0.1/evalidate.egg-info/not-zip-safe
--rw-r--r--   0 xenon     (1000) xenon     (1000)       10 2023-06-22 14:47:46.000000 evalidate-2.0.1/evalidate.egg-info/top_level.txt
--rw-r--r--   0 xenon     (1000) xenon     (1000)       38 2023-06-22 14:47:46.245852 evalidate-2.0.1/setup.cfg
--rw-r--r--   0 xenon     (1000) xenon     (1000)     1077 2023-06-15 17:42:59.000000 evalidate-2.0.1/setup.py
+drwxr-xr-x   0 xenon     (1000) xenon     (1000)        0 2023-07-08 07:56:22.914012 evalidate-2.0.2/
+-rw-r--r--   0 xenon     (1000) xenon     (1000)    12326 2023-07-08 07:56:22.914012 evalidate-2.0.2/PKG-INFO
+-rw-r--r--   0 xenon     (1000) xenon     (1000)     9540 2023-06-22 14:53:25.000000 evalidate-2.0.2/README.md
+drwxr-xr-x   0 xenon     (1000) xenon     (1000)        0 2023-07-08 07:56:22.914012 evalidate-2.0.2/evalidate/
+-rwxr-xr-x   0 xenon     (1000) xenon     (1000)     4091 2023-07-08 07:54:46.000000 evalidate-2.0.2/evalidate/__init__.py
+-rw-r--r--   0 xenon     (1000) xenon     (1000)     2506 2023-06-21 21:43:38.000000 evalidate-2.0.2/evalidate/security.py
+drwxr-xr-x   0 xenon     (1000) xenon     (1000)        0 2023-07-08 07:56:22.914012 evalidate-2.0.2/evalidate.egg-info/
+-rw-r--r--   0 xenon     (1000) xenon     (1000)    12326 2023-07-08 07:56:22.000000 evalidate-2.0.2/evalidate.egg-info/PKG-INFO
+-rw-r--r--   0 xenon     (1000) xenon     (1000)      226 2023-07-08 07:56:22.000000 evalidate-2.0.2/evalidate.egg-info/SOURCES.txt
+-rw-r--r--   0 xenon     (1000) xenon     (1000)        1 2023-07-08 07:56:22.000000 evalidate-2.0.2/evalidate.egg-info/dependency_links.txt
+-rw-r--r--   0 xenon     (1000) xenon     (1000)        1 2022-08-10 17:45:22.000000 evalidate-2.0.2/evalidate.egg-info/not-zip-safe
+-rw-r--r--   0 xenon     (1000) xenon     (1000)       10 2023-07-08 07:56:22.000000 evalidate-2.0.2/evalidate.egg-info/top_level.txt
+-rw-r--r--   0 xenon     (1000) xenon     (1000)       38 2023-07-08 07:56:22.914012 evalidate-2.0.2/setup.cfg
+-rw-r--r--   0 xenon     (1000) xenon     (1000)     1077 2023-06-15 17:42:59.000000 evalidate-2.0.2/setup.py
```

### Comparing `evalidate-2.0.1/PKG-INFO` & `evalidate-2.0.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 Metadata-Version: 2.1
 Name: evalidate
-Version: 2.0.1
+Version: 2.0.2
 Summary: Validation and secure evaluation of untrusted python expressions
 Home-page: http://github.com/yaroslaff/evalidate
 Author: Yaroslav Polyakov
 Author-email: xenon@sysattack.com
 License: MIT
 Description: ﻿# Evalidate
         Evalidate is simple python module for safe and very fast eval()'uating user-supplied (possible malicious) python expressions.
         
         ## Upgrade warning
-        Version 2.0 is backward incompatible with older versions. safeeval and evalidate methods are removed, and EvalMode class is introduced.
+        Version 2.0 is backward incompatible with older versions. `safeeval()` and `evalidate()` methods are removed, and EvalMode class is introduced.
+        
+        See [upgrade example in ticket](https://github.com/yaroslaff/evalidate/issues/5) or use older (any before 2.0.0, e.g. [v1.1.0](https://pypi.org/project/evalidate/1.1.0/)) if you have old code and do not want to upgrade. But upgrading is easy, so please consider this option.
         
         ## Purpose
         Originally it's developed for filtering complex data structures e.g. 
         
         Find cheap smartphones available for sale:
         ```python
         category="smartphones" and price<300 and stock>0
```

### Comparing `evalidate-2.0.1/README.md` & `evalidate-2.0.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 ﻿# Evalidate
 Evalidate is simple python module for safe and very fast eval()'uating user-supplied (possible malicious) python expressions.
 
 ## Upgrade warning
-Version 2.0 is backward incompatible with older versions. safeeval and evalidate methods are removed, and EvalMode class is introduced.
+Version 2.0 is backward incompatible with older versions. `safeeval()` and `evalidate()` methods are removed, and EvalMode class is introduced.
+
+See [upgrade example in ticket](https://github.com/yaroslaff/evalidate/issues/5) or use older (any before 2.0.0, e.g. [v1.1.0](https://pypi.org/project/evalidate/1.1.0/)) if you have old code and do not want to upgrade. But upgrading is easy, so please consider this option.
 
 ## Purpose
 Originally it's developed for filtering complex data structures e.g. 
 
 Find cheap smartphones available for sale:
 ```python
 category="smartphones" and price<300 and stock>0
```

### Comparing `evalidate-2.0.1/evalidate/__init__.py` & `evalidate-2.0.2/evalidate/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 """Safe user-supplied python expression evaluation."""
 
 import ast
 import dataclasses
 from typing import Callable
 
-__version__ = '2.0.1'
+__version__ = '2.0.2'
 
 
 class EvalException(Exception):
     pass
 
 
 class ValidationException(EvalException):
@@ -90,15 +90,15 @@
                 # any expression or constant
                 'Expression', 'Constant',
                 # == ...
                 'Compare', 'Eq', 'NotEq', 'Gt', 'GtE', 'Lt', 'LtE',
                 # variable name
                 'Name', 'Load',
                 'BinOp',
-                'Add', 'Sub',
+                'Add', 'Sub', 'USub',
                 'Subscript', 'Index',  # person['name']
                 'BoolOp', 'And', 'Or', 'UnaryOp', 'Not',  # True and True
                 "In", "NotIn",  # "aaa" in i['list']
                 "IfExp",  # for if expressions, like: expr1 if expr2 else expr3
                 "NameConstant",  # for True and False constants
                 "Div", "Mod"
             ],
```

### Comparing `evalidate-2.0.1/evalidate/security.py` & `evalidate-2.0.2/evalidate/security.py`

 * *Files identical despite different names*

### Comparing `evalidate-2.0.1/evalidate.egg-info/PKG-INFO` & `evalidate-2.0.2/evalidate.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 Metadata-Version: 2.1
 Name: evalidate
-Version: 2.0.1
+Version: 2.0.2
 Summary: Validation and secure evaluation of untrusted python expressions
 Home-page: http://github.com/yaroslaff/evalidate
 Author: Yaroslav Polyakov
 Author-email: xenon@sysattack.com
 License: MIT
 Description: ﻿# Evalidate
         Evalidate is simple python module for safe and very fast eval()'uating user-supplied (possible malicious) python expressions.
         
         ## Upgrade warning
-        Version 2.0 is backward incompatible with older versions. safeeval and evalidate methods are removed, and EvalMode class is introduced.
+        Version 2.0 is backward incompatible with older versions. `safeeval()` and `evalidate()` methods are removed, and EvalMode class is introduced.
+        
+        See [upgrade example in ticket](https://github.com/yaroslaff/evalidate/issues/5) or use older (any before 2.0.0, e.g. [v1.1.0](https://pypi.org/project/evalidate/1.1.0/)) if you have old code and do not want to upgrade. But upgrading is easy, so please consider this option.
         
         ## Purpose
         Originally it's developed for filtering complex data structures e.g. 
         
         Find cheap smartphones available for sale:
         ```python
         category="smartphones" and price<300 and stock>0
```

### Comparing `evalidate-2.0.1/setup.py` & `evalidate-2.0.2/setup.py`

 * *Files identical despite different names*

