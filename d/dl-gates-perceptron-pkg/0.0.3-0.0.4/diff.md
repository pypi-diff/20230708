# Comparing `tmp/dl_gates_perceptron_pkg-0.0.3.tar.gz` & `tmp/dl_gates_perceptron_pkg-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dl_gates_perceptron_pkg-0.0.3.tar", last modified: Sat Jul  8 11:48:03 2023, max compression
+gzip compressed data, was "dl_gates_perceptron_pkg-0.0.4.tar", last modified: Sat Jul  8 12:09:24 2023, max compression
```

## Comparing `dl_gates_perceptron_pkg-0.0.3.tar` & `dl_gates_perceptron_pkg-0.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 11:48:03.174291 dl_gates_perceptron_pkg-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-08 11:47:51.000000 dl_gates_perceptron_pkg-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      522 2023-07-08 11:48:03.174291 dl_gates_perceptron_pkg-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-08 11:47:51.000000 dl_gates_perceptron_pkg-0.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-07-08 11:47:51.000000 dl_gates_perceptron_pkg-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 11:48:03.174291 dl_gates_perceptron_pkg-0.0.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 11:48:03.174291 dl_gates_perceptron_pkg-0.0.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 11:48:03.174291 dl_gates_perceptron_pkg-0.0.3/src/Perceptron/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 11:47:51.000000 dl_gates_perceptron_pkg-0.0.3/src/Perceptron/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2611 2023-07-08 11:47:51.000000 dl_gates_perceptron_pkg-0.0.3/src/Perceptron/perceptron.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 11:48:03.174291 dl_gates_perceptron_pkg-0.0.3/src/dl_gates_perceptron_pkg.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      522 2023-07-08 11:48:03.000000 dl_gates_perceptron_pkg-0.0.3/src/dl_gates_perceptron_pkg.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-07-08 11:48:03.000000 dl_gates_perceptron_pkg-0.0.3/src/dl_gates_perceptron_pkg.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 11:48:03.000000 dl_gates_perceptron_pkg-0.0.3/src/dl_gates_perceptron_pkg.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-08 11:48:03.000000 dl_gates_perceptron_pkg-0.0.3/src/dl_gates_perceptron_pkg.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 12:09:24.057233 dl_gates_perceptron_pkg-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-08 12:09:12.000000 dl_gates_perceptron_pkg-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-07-08 12:09:24.057233 dl_gates_perceptron_pkg-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-07-08 12:09:12.000000 dl_gates_perceptron_pkg-0.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-07-08 12:09:12.000000 dl_gates_perceptron_pkg-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 12:09:24.057233 dl_gates_perceptron_pkg-0.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 12:09:24.057233 dl_gates_perceptron_pkg-0.0.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 12:09:24.057233 dl_gates_perceptron_pkg-0.0.4/src/Perceptron/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 12:09:12.000000 dl_gates_perceptron_pkg-0.0.4/src/Perceptron/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2611 2023-07-08 12:09:12.000000 dl_gates_perceptron_pkg-0.0.4/src/Perceptron/perceptron.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 12:09:24.057233 dl_gates_perceptron_pkg-0.0.4/src/dl_gates_perceptron_pkg.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-07-08 12:09:24.000000 dl_gates_perceptron_pkg-0.0.4/src/dl_gates_perceptron_pkg.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-07-08 12:09:24.000000 dl_gates_perceptron_pkg-0.0.4/src/dl_gates_perceptron_pkg.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 12:09:24.000000 dl_gates_perceptron_pkg-0.0.4/src/dl_gates_perceptron_pkg.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-08 12:09:24.000000 dl_gates_perceptron_pkg-0.0.4/src/dl_gates_perceptron_pkg.egg-info/top_level.txt
```

### Comparing `dl_gates_perceptron_pkg-0.0.3/LICENSE` & `dl_gates_perceptron_pkg-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `dl_gates_perceptron_pkg-0.0.3/pyproject.toml` & `dl_gates_perceptron_pkg-0.0.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "dl_gates_perceptron_pkg"
-version = "0.0.3"
+version = "0.0.4"
 authors = [{name = "junaid-o"}]
 description = "A small package for perceptron"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
```

### Comparing `dl_gates_perceptron_pkg-0.0.3/src/Perceptron/perceptron.py` & `dl_gates_perceptron_pkg-0.0.4/src/Perceptron/perceptron.py`

 * *Files identical despite different names*

