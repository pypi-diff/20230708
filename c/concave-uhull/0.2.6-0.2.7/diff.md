# Comparing `tmp/concave_uhull-0.2.6.tar.gz` & `tmp/concave_uhull-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "concave_uhull-0.2.6.tar", max compression
+gzip compressed data, was "concave_uhull-0.2.7.tar", max compression
```

## Comparing `concave_uhull-0.2.6.tar` & `concave_uhull-0.2.7.tar`

### file list

```diff
@@ -1,8 +1,7 @@
--rw-r--r--   0        0        0      321 2023-02-13 23:11:05.234480 concave_uhull-0.2.6/README_pypi.rst
--rw-r--r--   0        0        0        0 2023-02-08 19:07:35.341531 concave_uhull-0.2.6/concave_uhull/__init__.py
--rw-r--r--   0        0        0    12313 2023-07-08 14:53:02.390568 concave_uhull-0.2.6/concave_uhull/alpha_shape.py
--rw-r--r--   0        0        0     3706 2023-02-08 19:07:35.341531 concave_uhull-0.2.6/concave_uhull/geometry.py
--rw-r--r--   0        0        0     7660 2023-06-17 20:10:07.464809 concave_uhull-0.2.6/concave_uhull/graph.py
--rw-r--r--   0        0        0      834 2023-07-08 15:09:57.743993 concave_uhull-0.2.6/pyproject.toml
--rw-r--r--   0        0        0     1076 1970-01-01 00:00:00.000000 concave_uhull-0.2.6/setup.py
--rw-r--r--   0        0        0      994 1970-01-01 00:00:00.000000 concave_uhull-0.2.6/PKG-INFO
+-rw-r--r--   0        0        0      283 2023-07-08 19:10:53.906520 concave_uhull-0.2.7/README_pypi.rst
+-rw-r--r--   0        0        0        0 2023-07-08 17:11:45.095432 concave_uhull-0.2.7/concave_uhull/__init__.py
+-rw-r--r--   0        0        0    12313 2023-07-08 18:56:26.115876 concave_uhull-0.2.7/concave_uhull/alpha_shape.py
+-rw-r--r--   0        0        0     3706 2023-07-08 17:11:45.095432 concave_uhull-0.2.7/concave_uhull/geometry.py
+-rw-r--r--   0        0        0     7660 2023-07-08 17:11:45.095432 concave_uhull-0.2.7/concave_uhull/graph.py
+-rw-r--r--   0        0        0      819 2023-07-08 19:05:09.016402 concave_uhull-0.2.7/pyproject.toml
+-rw-r--r--   0        0        0      954 1970-01-01 00:00:00.000000 concave_uhull-0.2.7/PKG-INFO
```

### Comparing `concave_uhull-0.2.6/concave_uhull/alpha_shape.py` & `concave_uhull-0.2.7/concave_uhull/alpha_shape.py`

 * *Files identical despite different names*

### Comparing `concave_uhull-0.2.6/concave_uhull/geometry.py` & `concave_uhull-0.2.7/concave_uhull/geometry.py`

 * *Files identical despite different names*

### Comparing `concave_uhull-0.2.6/concave_uhull/graph.py` & `concave_uhull-0.2.7/concave_uhull/graph.py`

 * *Files identical despite different names*

### Comparing `concave_uhull-0.2.6/pyproject.toml` & `concave_uhull-0.2.7/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [tool.poetry]
 name = "concave_uhull"
-version = "0.2.6"
+version = "0.2.7"
 description = "A simple (but not simpler) algorithm for concave hull of 2D point sets using an alpha shape algorithm."
 readme = "README_pypi.rst"
 authors = ["Luan <llvdmoraes@gmail.com>"]
-repository = "https://github.com/luanleonardo/concave_uhull"
-homepage = "https://luanleonardo.github.io/concave_uhull/"
+repository = "https://github.com/luanleonardo/uhull"
+homepage = "https://luanleonardo.github.io/uhull/"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<3.12"
-numpy = "1.22.4"
+numpy = "^1.24.1"
 scipy = "^1.10.0"
 
 [tool.poetry.group.dev.dependencies]
 black = {extras = ["jupyter"], version = "^22.12.0"}
 isort = "^5.11.4"
 ipython = "^8.8.0"
 pytest-cov = "^4.0.0"
```

