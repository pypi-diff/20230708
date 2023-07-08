# Comparing `tmp/uhull-0.1.0.tar.gz` & `tmp/uhull-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uhull-0.1.0.tar", max compression
+gzip compressed data, was "uhull-0.1.1.tar", max compression
```

## Comparing `uhull-0.1.0.tar` & `uhull-0.1.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      305 2023-07-08 16:46:19.545598 uhull-0.1.0/README_pypi.rst
--rw-r--r--   0        0        0      810 2023-07-08 16:36:57.073191 uhull-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-08 15:47:32.173097 uhull-0.1.0/uhull/__init__.py
--rw-r--r--   0        0        0    12297 2023-07-08 16:51:52.026831 uhull-0.1.0/uhull/alpha_shape.py
--rw-r--r--   0        0        0     3706 2023-02-08 19:07:35.341530 uhull-0.1.0/uhull/geometry.py
--rw-r--r--   0        0        0     7660 2023-06-17 20:10:07.464808 uhull-0.1.0/uhull/graph.py
--rw-r--r--   0        0        0      954 1970-01-01 00:00:00.000000 uhull-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      305 2023-07-08 16:46:19.545598 uhull-0.1.1/README_pypi.rst
+-rw-r--r--   0        0        0      816 2023-07-08 18:46:14.979210 uhull-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-08 15:47:32.173097 uhull-0.1.1/uhull/__init__.py
+-rw-r--r--   0        0        0    12297 2023-07-08 18:40:34.128529 uhull-0.1.1/uhull/alpha_shape.py
+-rw-r--r--   0        0        0     3706 2023-02-08 19:07:35.341530 uhull-0.1.1/uhull/geometry.py
+-rw-r--r--   0        0        0     7660 2023-06-17 20:10:07.464808 uhull-0.1.1/uhull/graph.py
+-rw-r--r--   0        0        0      958 1970-01-01 00:00:00.000000 uhull-0.1.1/PKG-INFO
```

### Comparing `uhull-0.1.0/pyproject.toml` & `uhull-0.1.1/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [tool.poetry]
 name = "uhull"
-version = "0.1.0"
+version = "0.1.1"
 description = "A simple (but not simpler) algorithm for concave hull of 2D point sets using an alpha shape algorithm."
 readme = "README_pypi.rst"
 authors = ["Luan <llvdmoraes@gmail.com>"]
 repository = "https://github.com/luanleonardo/uhull"
 homepage = "https://luanleonardo.github.io/uhull/"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<3.12"
-numpy = "1.22.4"
+numpy = ">=1.22,<1.24"
 scipy = "^1.10.0"
 
 [tool.poetry.group.dev.dependencies]
 black = {extras = ["jupyter"], version = "^22.12.0"}
 isort = "^5.11.4"
 ipython = "^8.8.0"
 pytest-cov = "^4.0.0"
```

### Comparing `uhull-0.1.0/uhull/alpha_shape.py` & `uhull-0.1.1/uhull/alpha_shape.py`

 * *Files identical despite different names*

### Comparing `uhull-0.1.0/uhull/geometry.py` & `uhull-0.1.1/uhull/geometry.py`

 * *Files identical despite different names*

### Comparing `uhull-0.1.0/uhull/graph.py` & `uhull-0.1.1/uhull/graph.py`

 * *Files identical despite different names*

### Comparing `uhull-0.1.0/PKG-INFO` & `uhull-0.1.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: uhull
-Version: 0.1.0
+Version: 0.1.1
 Summary: A simple (but not simpler) algorithm for concave hull of 2D point sets using an alpha shape algorithm.
 Home-page: https://luanleonardo.github.io/uhull/
 Author: Luan
 Author-email: llvdmoraes@gmail.com
 Requires-Python: >=3.8.1,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: numpy (==1.22.4)
+Requires-Dist: numpy (>=1.22,<1.24)
 Requires-Dist: scipy (>=1.10.0,<2.0.0)
 Project-URL: Repository, https://github.com/luanleonardo/uhull
 Description-Content-Type: text/x-rst
 
 ==============
 Uhull*
 ==============
```

