# Comparing `tmp/euclipy-1.0.0.tar.gz` & `tmp/euclipy-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "euclipy-1.0.0.tar", last modified: Wed Jun 21 01:36:42 2023, max compression
+gzip compressed data, was "euclipy-1.0.1.tar", last modified: Sat Jul  8 19:55:50 2023, max compression
```

## Comparing `euclipy-1.0.0.tar` & `euclipy-1.0.1.tar`

### file list

```diff
@@ -1,51 +1,52 @@
-drwxr-xr-x   0 joshuavaron  (1000) joshuavaron  (1000)        0 2023-06-21 01:36:42.970635 euclipy-1.0.0/
--rw-r--r--   0 joshuavaron  (1000) joshuavaron  (1000)     1051 2023-03-18 23:11:56.000000 euclipy-1.0.0/LICENSE.txt
--rw-r--r--   0 joshuavaron  (1000) joshuavaron  (1000)       73 2023-03-18 23:11:56.000000 euclipy-1.0.0/MANIFEST.in
--rw-r--r--   0 joshuavaron  (1000) joshuavaron  (1000)     2121 2023-06-21 01:36:42.970635 euclipy-1.0.0/PKG-INFO
--rw-r--r--   0 joshuavaron  (1000) joshuavaron  (1000)     1422 2023-03-18 23:11:56.000000 euclipy-1.0.0/README.md
-drwxr-xr-x   0 joshuavaron  (1000) joshuavaron  (1000)        0 2023-06-21 01:36:42.960635 euclipy-1.0.0/docs/
-drwxr-xr-x   0 joshuavaron  (1000) joshuavaron  (1000)        0 2023-06-21 01:36:42.970635 euclipy-1.0.0/docs/changelog/
--rw-r--r--   0 joshuavaron  (1000) joshuavaron  (1000)       53 2023-03-18 23:11:56.000000 euclipy-1.0.0/docs/changelog/0.0.1-changelog.txt
--rw-r--r--   0 joshuavaron  (1000) joshuavaron  (1000)       77 2023-03-18 23:11:56.000000 euclipy-1.0.0/docs/changelog/0.0.2-changelog.txt
--rw-r--r--   0 joshuavaron  (1000) joshuavaron  (1000)       74 2023-03-18 23:11:56.000000 euclipy-1.0.0/docs/changelog/0.0.3-changelog.txt
--rw-r--r--   0 joshuavaron  (1000) joshuavaron  (1000)      119 2023-03-18 23:11:56.000000 euclipy-1.0.0/docs/changelog/0.1.0-changelog.txt
--rw-r--r--   0 joshuavaron  (1000) joshuavaron  (1000)       50 2023-03-18 23:11:56.000000 euclipy-1.0.0/docs/changelog/0.1.1-changelog.txt
--rw-r--r--   0 joshuavaron  (1000) joshuavaron  (1000)       63 2023-03-18 23:11:56.000000 euclipy-1.0.0/docs/changelog/0.2.0-changelog.txt
--rw-r--r--   0 joshuavaron  (1000) joshuavaron  (1000)       60 2023-03-18 23:11:56.000000 euclipy-1.0.0/docs/changelog/0.2.1-changelog.txt
--rw-r--r--   0 joshuavaron  (1000) joshuavaron  (1000)       60 2023-03-18 23:11:56.000000 euclipy-1.0.0/docs/changelog/0.2.10-changelog.txt
--rw-r--r--   0 joshuavaron  (1000) joshuavaron  (1000)       52 2023-03-18 23:11:56.000000 euclipy-1.0.0/docs/changelog/0.2.11-changelog.txt
--rw-r--r--   0 joshuavaron  (1000) joshuavaron  (1000)       96 2023-03-18 23:11:56.000000 euclipy-1.0.0/docs/changelog/0.2.12-changelog.txt
--rw-r--r--   0 joshuavaron  (1000) joshuavaron  (1000)       99 2023-03-18 23:11:56.000000 euclipy-1.0.0/docs/changelog/0.2.13-changelog.txt
--rw-r--r--   0 joshuavaron  (1000) joshuavaron  (1000)       95 2023-03-18 23:11:56.000000 euclipy-1.0.0/docs/changelog/0.2.2-changelog.txt
--rw-r--r--   0 joshuavaron  (1000) joshuavaron  (1000)       70 2023-03-18 23:11:56.000000 euclipy-1.0.0/docs/changelog/0.2.3-changelog.txt
--rw-r--r--   0 joshuavaron  (1000) joshuavaron  (1000)       53 2023-03-18 23:11:56.000000 euclipy-1.0.0/docs/changelog/0.2.4-changelog.txt
--rw-r--r--   0 joshuavaron  (1000) joshuavaron  (1000)      110 2023-03-18 23:11:56.000000 euclipy-1.0.0/docs/changelog/0.2.5-changelog.txt
--rw-r--r--   0 joshuavaron  (1000) joshuavaron  (1000)      205 2023-03-18 23:11:56.000000 euclipy-1.0.0/docs/changelog/0.2.6-changelog.txt
--rw-r--r--   0 joshuavaron  (1000) joshuavaron  (1000)       62 2023-03-18 23:11:56.000000 euclipy-1.0.0/docs/changelog/0.2.7.changelog.txt
--rw-r--r--   0 joshuavaron  (1000) joshuavaron  (1000)       59 2023-03-18 23:11:56.000000 euclipy-1.0.0/docs/changelog/0.2.8-changelog.txt
--rw-r--r--   0 joshuavaron  (1000) joshuavaron  (1000)       59 2023-03-18 23:11:56.000000 euclipy-1.0.0/docs/changelog/0.2.9-changelog.txt
--rw-r--r--   0 joshuavaron  (1000) joshuavaron  (1000)      236 2023-03-18 23:11:56.000000 euclipy-1.0.0/docs/changelog/0.3.0-changelog.txt
--rw-r--r--   0 joshuavaron  (1000) joshuavaron  (1000)      102 2023-03-18 23:11:56.000000 euclipy-1.0.0/docs/changelog/0.3.1-changelog.txt
--rw-r--r--   0 joshuavaron  (1000) joshuavaron  (1000)      553 2023-06-21 01:31:45.000000 euclipy-1.0.0/docs/changelog/1.0.0-changelog.txt
--rw-r--r--   0 joshuavaron  (1000) joshuavaron  (1000)     1924 2023-06-21 01:20:42.000000 euclipy-1.0.0/docs/conf.py
--rw-r--r--   0 joshuavaron  (1000) joshuavaron  (1000)      397 2023-06-21 01:26:36.000000 euclipy-1.0.0/docs/theorems.txt
-drwxr-xr-x   0 joshuavaron  (1000) joshuavaron  (1000)        0 2023-06-21 01:36:42.970635 euclipy-1.0.0/euclipy/
--rw-r--r--   0 joshuavaron  (1000) joshuavaron  (1000)        0 2023-03-18 23:11:56.000000 euclipy-1.0.0/euclipy/__init__.py
--rw-r--r--   0 joshuavaron  (1000) joshuavaron  (1000)    17167 2023-05-30 17:15:14.000000 euclipy-1.0.0/euclipy/core.py
--rw-r--r--   0 joshuavaron  (1000) joshuavaron  (1000)      783 2023-03-19 02:51:14.000000 euclipy-1.0.0/euclipy/exceptions.py
--rw-r--r--   0 joshuavaron  (1000) joshuavaron  (1000)    18193 2023-06-21 01:06:56.000000 euclipy-1.0.0/euclipy/geometricobjects.py
--rw-r--r--   0 joshuavaron  (1000) joshuavaron  (1000)     2962 2023-06-21 00:46:34.000000 euclipy-1.0.0/euclipy/polygon.py
--rw-r--r--   0 joshuavaron  (1000) joshuavaron  (1000)     1875 2023-06-21 01:17:17.000000 euclipy-1.0.0/euclipy/theorems.py
-drwxr-xr-x   0 joshuavaron  (1000) joshuavaron  (1000)        0 2023-06-21 01:36:42.970635 euclipy-1.0.0/euclipy.egg-info/
--rw-r--r--   0 joshuavaron  (1000) joshuavaron  (1000)     2121 2023-06-21 01:36:42.000000 euclipy-1.0.0/euclipy.egg-info/PKG-INFO
--rw-r--r--   0 joshuavaron  (1000) joshuavaron  (1000)     1213 2023-06-21 01:36:42.000000 euclipy-1.0.0/euclipy.egg-info/SOURCES.txt
--rw-r--r--   0 joshuavaron  (1000) joshuavaron  (1000)        1 2023-06-21 01:36:42.000000 euclipy-1.0.0/euclipy.egg-info/dependency_links.txt
--rw-r--r--   0 joshuavaron  (1000) joshuavaron  (1000)        6 2023-06-21 01:36:42.000000 euclipy-1.0.0/euclipy.egg-info/requires.txt
--rw-r--r--   0 joshuavaron  (1000) joshuavaron  (1000)        8 2023-06-21 01:36:42.000000 euclipy-1.0.0/euclipy.egg-info/top_level.txt
--rw-r--r--   0 joshuavaron  (1000) joshuavaron  (1000)        5 2023-03-18 23:11:56.000000 euclipy-1.0.0/requirements.txt
--rw-r--r--   0 joshuavaron  (1000) joshuavaron  (1000)       38 2023-06-21 01:36:42.970635 euclipy-1.0.0/setup.cfg
--rw-r--r--   0 joshuavaron  (1000) joshuavaron  (1000)     1016 2023-06-21 01:25:03.000000 euclipy-1.0.0/setup.py
-drwxr-xr-x   0 joshuavaron  (1000) joshuavaron  (1000)        0 2023-06-21 01:36:42.970635 euclipy-1.0.0/tests/
--rw-r--r--   0 joshuavaron  (1000) joshuavaron  (1000)       27 2023-03-18 23:11:56.000000 euclipy-1.0.0/tests/__init__.py
--rw-r--r--   0 joshuavaron  (1000) joshuavaron  (1000)    19121 2023-06-21 00:46:04.000000 euclipy-1.0.0/tests/test_object_framework.py
--rw-r--r--   0 joshuavaron  (1000) joshuavaron  (1000)     1588 2023-06-21 01:18:03.000000 euclipy-1.0.0/tests/test_proofs.py
+drwxr-xr-x   0 joshuavaron  (1000) joshuavaron  (1000)        0 2023-07-08 19:55:50.588505 euclipy-1.0.1/
+-rw-r--r--   0 joshuavaron  (1000) joshuavaron  (1000)     1051 2023-03-18 23:11:56.000000 euclipy-1.0.1/LICENSE.txt
+-rw-r--r--   0 joshuavaron  (1000) joshuavaron  (1000)       73 2023-03-18 23:11:56.000000 euclipy-1.0.1/MANIFEST.in
+-rw-r--r--   0 joshuavaron  (1000) joshuavaron  (1000)     2232 2023-07-08 19:55:50.588505 euclipy-1.0.1/PKG-INFO
+-rw-r--r--   0 joshuavaron  (1000) joshuavaron  (1000)     1533 2023-07-08 19:51:42.000000 euclipy-1.0.1/README.md
+drwxr-xr-x   0 joshuavaron  (1000) joshuavaron  (1000)        0 2023-07-08 19:55:50.588505 euclipy-1.0.1/docs/
+drwxr-xr-x   0 joshuavaron  (1000) joshuavaron  (1000)        0 2023-07-08 19:55:50.588505 euclipy-1.0.1/docs/changelog/
+-rw-r--r--   0 joshuavaron  (1000) joshuavaron  (1000)       53 2023-03-18 23:11:56.000000 euclipy-1.0.1/docs/changelog/0.0.1-changelog.txt
+-rw-r--r--   0 joshuavaron  (1000) joshuavaron  (1000)       77 2023-03-18 23:11:56.000000 euclipy-1.0.1/docs/changelog/0.0.2-changelog.txt
+-rw-r--r--   0 joshuavaron  (1000) joshuavaron  (1000)       74 2023-03-18 23:11:56.000000 euclipy-1.0.1/docs/changelog/0.0.3-changelog.txt
+-rw-r--r--   0 joshuavaron  (1000) joshuavaron  (1000)      119 2023-03-18 23:11:56.000000 euclipy-1.0.1/docs/changelog/0.1.0-changelog.txt
+-rw-r--r--   0 joshuavaron  (1000) joshuavaron  (1000)       50 2023-03-18 23:11:56.000000 euclipy-1.0.1/docs/changelog/0.1.1-changelog.txt
+-rw-r--r--   0 joshuavaron  (1000) joshuavaron  (1000)       63 2023-03-18 23:11:56.000000 euclipy-1.0.1/docs/changelog/0.2.0-changelog.txt
+-rw-r--r--   0 joshuavaron  (1000) joshuavaron  (1000)       60 2023-03-18 23:11:56.000000 euclipy-1.0.1/docs/changelog/0.2.1-changelog.txt
+-rw-r--r--   0 joshuavaron  (1000) joshuavaron  (1000)       60 2023-03-18 23:11:56.000000 euclipy-1.0.1/docs/changelog/0.2.10-changelog.txt
+-rw-r--r--   0 joshuavaron  (1000) joshuavaron  (1000)       52 2023-03-18 23:11:56.000000 euclipy-1.0.1/docs/changelog/0.2.11-changelog.txt
+-rw-r--r--   0 joshuavaron  (1000) joshuavaron  (1000)       96 2023-03-18 23:11:56.000000 euclipy-1.0.1/docs/changelog/0.2.12-changelog.txt
+-rw-r--r--   0 joshuavaron  (1000) joshuavaron  (1000)       99 2023-03-18 23:11:56.000000 euclipy-1.0.1/docs/changelog/0.2.13-changelog.txt
+-rw-r--r--   0 joshuavaron  (1000) joshuavaron  (1000)       95 2023-03-18 23:11:56.000000 euclipy-1.0.1/docs/changelog/0.2.2-changelog.txt
+-rw-r--r--   0 joshuavaron  (1000) joshuavaron  (1000)       70 2023-03-18 23:11:56.000000 euclipy-1.0.1/docs/changelog/0.2.3-changelog.txt
+-rw-r--r--   0 joshuavaron  (1000) joshuavaron  (1000)       53 2023-03-18 23:11:56.000000 euclipy-1.0.1/docs/changelog/0.2.4-changelog.txt
+-rw-r--r--   0 joshuavaron  (1000) joshuavaron  (1000)      110 2023-03-18 23:11:56.000000 euclipy-1.0.1/docs/changelog/0.2.5-changelog.txt
+-rw-r--r--   0 joshuavaron  (1000) joshuavaron  (1000)      205 2023-03-18 23:11:56.000000 euclipy-1.0.1/docs/changelog/0.2.6-changelog.txt
+-rw-r--r--   0 joshuavaron  (1000) joshuavaron  (1000)       62 2023-03-18 23:11:56.000000 euclipy-1.0.1/docs/changelog/0.2.7.changelog.txt
+-rw-r--r--   0 joshuavaron  (1000) joshuavaron  (1000)       59 2023-03-18 23:11:56.000000 euclipy-1.0.1/docs/changelog/0.2.8-changelog.txt
+-rw-r--r--   0 joshuavaron  (1000) joshuavaron  (1000)       59 2023-03-18 23:11:56.000000 euclipy-1.0.1/docs/changelog/0.2.9-changelog.txt
+-rw-r--r--   0 joshuavaron  (1000) joshuavaron  (1000)      236 2023-03-18 23:11:56.000000 euclipy-1.0.1/docs/changelog/0.3.0-changelog.txt
+-rw-r--r--   0 joshuavaron  (1000) joshuavaron  (1000)      102 2023-03-18 23:11:56.000000 euclipy-1.0.1/docs/changelog/0.3.1-changelog.txt
+-rw-r--r--   0 joshuavaron  (1000) joshuavaron  (1000)      553 2023-06-21 01:31:45.000000 euclipy-1.0.1/docs/changelog/1.0.0-changelog.txt
+-rw-r--r--   0 joshuavaron  (1000) joshuavaron  (1000)       68 2023-07-08 19:55:21.000000 euclipy-1.0.1/docs/changelog/1.0.1-changelog.txt
+-rw-r--r--   0 joshuavaron  (1000) joshuavaron  (1000)     1924 2023-06-21 01:20:42.000000 euclipy-1.0.1/docs/conf.py
+-rw-r--r--   0 joshuavaron  (1000) joshuavaron  (1000)      397 2023-06-21 01:26:36.000000 euclipy-1.0.1/docs/theorems.txt
+drwxr-xr-x   0 joshuavaron  (1000) joshuavaron  (1000)        0 2023-07-08 19:55:50.588505 euclipy-1.0.1/euclipy/
+-rw-r--r--   0 joshuavaron  (1000) joshuavaron  (1000)        0 2023-03-18 23:11:56.000000 euclipy-1.0.1/euclipy/__init__.py
+-rw-r--r--   0 joshuavaron  (1000) joshuavaron  (1000)    17167 2023-05-30 17:15:14.000000 euclipy-1.0.1/euclipy/core.py
+-rw-r--r--   0 joshuavaron  (1000) joshuavaron  (1000)      783 2023-03-19 02:51:14.000000 euclipy-1.0.1/euclipy/exceptions.py
+-rw-r--r--   0 joshuavaron  (1000) joshuavaron  (1000)    18193 2023-07-08 19:52:30.000000 euclipy-1.0.1/euclipy/geometricobjects.py
+-rw-r--r--   0 joshuavaron  (1000) joshuavaron  (1000)     2962 2023-06-21 00:46:34.000000 euclipy-1.0.1/euclipy/polygon.py
+-rw-r--r--   0 joshuavaron  (1000) joshuavaron  (1000)     1875 2023-06-21 01:17:17.000000 euclipy-1.0.1/euclipy/theorems.py
+drwxr-xr-x   0 joshuavaron  (1000) joshuavaron  (1000)        0 2023-07-08 19:55:50.588505 euclipy-1.0.1/euclipy.egg-info/
+-rw-r--r--   0 joshuavaron  (1000) joshuavaron  (1000)     2232 2023-07-08 19:55:50.000000 euclipy-1.0.1/euclipy.egg-info/PKG-INFO
+-rw-r--r--   0 joshuavaron  (1000) joshuavaron  (1000)     1248 2023-07-08 19:55:50.000000 euclipy-1.0.1/euclipy.egg-info/SOURCES.txt
+-rw-r--r--   0 joshuavaron  (1000) joshuavaron  (1000)        1 2023-07-08 19:55:50.000000 euclipy-1.0.1/euclipy.egg-info/dependency_links.txt
+-rw-r--r--   0 joshuavaron  (1000) joshuavaron  (1000)        6 2023-07-08 19:55:50.000000 euclipy-1.0.1/euclipy.egg-info/requires.txt
+-rw-r--r--   0 joshuavaron  (1000) joshuavaron  (1000)        8 2023-07-08 19:55:50.000000 euclipy-1.0.1/euclipy.egg-info/top_level.txt
+-rw-r--r--   0 joshuavaron  (1000) joshuavaron  (1000)        5 2023-03-18 23:11:56.000000 euclipy-1.0.1/requirements.txt
+-rw-r--r--   0 joshuavaron  (1000) joshuavaron  (1000)       38 2023-07-08 19:55:50.588505 euclipy-1.0.1/setup.cfg
+-rw-r--r--   0 joshuavaron  (1000) joshuavaron  (1000)     1016 2023-07-08 19:54:47.000000 euclipy-1.0.1/setup.py
+drwxr-xr-x   0 joshuavaron  (1000) joshuavaron  (1000)        0 2023-07-08 19:55:50.588505 euclipy-1.0.1/tests/
+-rw-r--r--   0 joshuavaron  (1000) joshuavaron  (1000)       27 2023-03-18 23:11:56.000000 euclipy-1.0.1/tests/__init__.py
+-rw-r--r--   0 joshuavaron  (1000) joshuavaron  (1000)    19121 2023-06-21 00:46:04.000000 euclipy-1.0.1/tests/test_object_framework.py
+-rw-r--r--   0 joshuavaron  (1000) joshuavaron  (1000)     1588 2023-06-21 01:18:03.000000 euclipy-1.0.1/tests/test_proofs.py
```

### Comparing `euclipy-1.0.0/LICENSE.txt` & `euclipy-1.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `euclipy-1.0.0/PKG-INFO` & `euclipy-1.0.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: euclipy
-Version: 1.0.0
+Version: 1.0.1
 Summary: A Synthetic Euclidean Geometry based library
 Home-page: 
 Author: Joshua Varon
 Author-email: 32440072+joshuavaron@users.noreply.github.com
 License: MIT
 Project-URL: Documentation, https://joshuavaron.github.io/euclipy/
 Project-URL: Source Code, https://github.com/joshuavaron/euclipy
@@ -32,15 +32,17 @@
 
 ## Features:
 
   
 
 - Create symbolic geometric objects (Triangle(), Segment(), Point(), etc.)
 
-- Implicitly defines segments created by constructions
+- Implicitly defines objects created by constructions
+
+- Implicitly gathers implicit information created by previous constructions
 
   
 
 ## Installation
 
 ```sh
 
@@ -50,16 +52,16 @@
 
 ```
 
 ## Sample Code (With Comments):
 
 ```py
 
-from euclipy.core import Line, Segment, Expression
-
+from euclipy.core import Expression
+from euclipy.geometricobjects import Line, Segment
 import euclipy.theorems as theorems
 
   
 
 if  __name__ == '__main__':
     # Construct a line with colinear points: A, B, C, D, E
     line = Line('A B C D E')
@@ -67,15 +69,15 @@
     # Define the lengths of line segments lying on line AE
     Segment('A C').measure = 5
     Segment('C E').measure = 12
     Segment('B E').measure = 15
     
     # Apply the relevant theorem which creates expressions about the sums of
     # contiguous subsegments of line segments
-    theorems.theorem_subsegment_sum(line)
+    theorems.subsegment_sum_theorem(line)
 
     # Solve the system of equations resresented by all of the expressions
     # created by theorems
     Expression.solve_system()
 
     # Verify one of the solutions found
     print(f"Segment('A B').measure = {Segment('A B').measure}") # 2
```

### Comparing `euclipy-1.0.0/README.md` & `euclipy-1.0.1/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -13,15 +13,17 @@
 
 ## Features:
 
   
 
 - Create symbolic geometric objects (Triangle(), Segment(), Point(), etc.)
 
-- Implicitly defines segments created by constructions
+- Implicitly defines objects created by constructions
+
+- Implicitly gathers implicit information created by previous constructions
 
   
 
 ## Installation
 
 ```sh
 
@@ -31,16 +33,16 @@
 
 ```
 
 ## Sample Code (With Comments):
 
 ```py
 
-from euclipy.core import Line, Segment, Expression
-
+from euclipy.core import Expression
+from euclipy.geometricobjects import Line, Segment
 import euclipy.theorems as theorems
 
   
 
 if  __name__ == '__main__':
     # Construct a line with colinear points: A, B, C, D, E
     line = Line('A B C D E')
@@ -48,15 +50,15 @@
     # Define the lengths of line segments lying on line AE
     Segment('A C').measure = 5
     Segment('C E').measure = 12
     Segment('B E').measure = 15
     
     # Apply the relevant theorem which creates expressions about the sums of
     # contiguous subsegments of line segments
-    theorems.theorem_subsegment_sum(line)
+    theorems.subsegment_sum_theorem(line)
 
     # Solve the system of equations resresented by all of the expressions
     # created by theorems
     Expression.solve_system()
 
     # Verify one of the solutions found
     print(f"Segment('A B').measure = {Segment('A B').measure}") # 2
```

### Comparing `euclipy-1.0.0/docs/changelog/1.0.0-changelog.txt` & `euclipy-1.0.1/docs/changelog/1.0.0-changelog.txt`

 * *Files identical despite different names*

### Comparing `euclipy-1.0.0/docs/conf.py` & `euclipy-1.0.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `euclipy-1.0.0/euclipy/core.py` & `euclipy-1.0.1/euclipy/core.py`

 * *Files identical despite different names*

### Comparing `euclipy-1.0.0/euclipy/exceptions.py` & `euclipy-1.0.1/euclipy/exceptions.py`

 * *Files identical despite different names*

### Comparing `euclipy-1.0.0/euclipy/geometricobjects.py` & `euclipy-1.0.1/euclipy/geometricobjects.py`

 * *Files 1% similar despite different names*

```diff
@@ -381,15 +381,15 @@
     def __new__(cls, pts_or_rays, reflex=None): #TODO: Should reflex default to True?
         '''Argument pts is one of the following:
         - a space separated triple of point labels representing an angle, e.g. 'B A C'
         - a tuple of three Point objects
         
         The points are to be ordered in a clockwise fashion, for example:
         - Angle('A B C') represents the angle between Segment('A B') and Segment('B C'), 
-            starting at Segment('B C') and moving counterclockwise.
+            starting at Segment('A B') and moving counterclockwise.
         '''
         if len(pts_or_rays) == 2 and isinstance(pts_or_rays[0], Ray) and isinstance(pts_or_rays[1], Ray):
             ray1, ray2 = pts_or_rays
         else:
             pts = points(pts_or_rays)
             if not (isinstance(pts, tuple) and len(pts) == 3):
                 raise ValueError('Instantiating an Angle requires exactly 3 points or 2 rays.')
```

### Comparing `euclipy-1.0.0/euclipy/polygon.py` & `euclipy-1.0.1/euclipy/polygon.py`

 * *Files identical despite different names*

### Comparing `euclipy-1.0.0/euclipy/theorems.py` & `euclipy-1.0.1/euclipy/theorems.py`

 * *Files identical despite different names*

### Comparing `euclipy-1.0.0/euclipy.egg-info/PKG-INFO` & `euclipy-1.0.1/euclipy.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: euclipy
-Version: 1.0.0
+Version: 1.0.1
 Summary: A Synthetic Euclidean Geometry based library
 Home-page: 
 Author: Joshua Varon
 Author-email: 32440072+joshuavaron@users.noreply.github.com
 License: MIT
 Project-URL: Documentation, https://joshuavaron.github.io/euclipy/
 Project-URL: Source Code, https://github.com/joshuavaron/euclipy
@@ -32,15 +32,17 @@
 
 ## Features:
 
   
 
 - Create symbolic geometric objects (Triangle(), Segment(), Point(), etc.)
 
-- Implicitly defines segments created by constructions
+- Implicitly defines objects created by constructions
+
+- Implicitly gathers implicit information created by previous constructions
 
   
 
 ## Installation
 
 ```sh
 
@@ -50,16 +52,16 @@
 
 ```
 
 ## Sample Code (With Comments):
 
 ```py
 
-from euclipy.core import Line, Segment, Expression
-
+from euclipy.core import Expression
+from euclipy.geometricobjects import Line, Segment
 import euclipy.theorems as theorems
 
   
 
 if  __name__ == '__main__':
     # Construct a line with colinear points: A, B, C, D, E
     line = Line('A B C D E')
@@ -67,15 +69,15 @@
     # Define the lengths of line segments lying on line AE
     Segment('A C').measure = 5
     Segment('C E').measure = 12
     Segment('B E').measure = 15
     
     # Apply the relevant theorem which creates expressions about the sums of
     # contiguous subsegments of line segments
-    theorems.theorem_subsegment_sum(line)
+    theorems.subsegment_sum_theorem(line)
 
     # Solve the system of equations resresented by all of the expressions
     # created by theorems
     Expression.solve_system()
 
     # Verify one of the solutions found
     print(f"Segment('A B').measure = {Segment('A B').measure}") # 2
```

### Comparing `euclipy-1.0.0/euclipy.egg-info/SOURCES.txt` & `euclipy-1.0.1/euclipy.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 docs/changelog/0.2.6-changelog.txt
 docs/changelog/0.2.7.changelog.txt
 docs/changelog/0.2.8-changelog.txt
 docs/changelog/0.2.9-changelog.txt
 docs/changelog/0.3.0-changelog.txt
 docs/changelog/0.3.1-changelog.txt
 docs/changelog/1.0.0-changelog.txt
+docs/changelog/1.0.1-changelog.txt
 euclipy/__init__.py
 euclipy/core.py
 euclipy/exceptions.py
 euclipy/geometricobjects.py
 euclipy/polygon.py
 euclipy/theorems.py
 euclipy.egg-info/PKG-INFO
```

### Comparing `euclipy-1.0.0/setup.py` & `euclipy-1.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
   'Operating System :: Microsoft :: Windows :: Windows 10',
   'License :: OSI Approved :: MIT License',
   'Programming Language :: Python :: 3'
 ]
 
 setup(
   name='euclipy',
-  version='1.0.0',
+  version='1.0.1',
   description='A Synthetic Euclidean Geometry based library',
   long_description=open('README.md', encoding='utf-8').read(),
   long_description_content_type='text/markdown',
   url='',
   project_urls={
             #"Bug Tracker": "",
             "Documentation": "https://joshuavaron.github.io/euclipy/",
```

### Comparing `euclipy-1.0.0/tests/test_object_framework.py` & `euclipy-1.0.1/tests/test_object_framework.py`

 * *Files identical despite different names*

### Comparing `euclipy-1.0.0/tests/test_proofs.py` & `euclipy-1.0.1/tests/test_proofs.py`

 * *Files identical despite different names*

