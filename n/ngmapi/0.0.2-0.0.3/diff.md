# Comparing `tmp/ngmapi-0.0.2.tar.gz` & `tmp/ngmapi-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ngmapi-0.0.2.tar", last modified: Fri Jul  7 10:03:21 2023, max compression
+gzip compressed data, was "ngmapi-0.0.3.tar", last modified: Fri Jul  7 10:16:13 2023, max compression
```

## Comparing `ngmapi-0.0.2.tar` & `ngmapi-0.0.3.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxr-xr-x   0 ngmaibulat   (502) staff       (20)        0 2023-07-07 10:03:21.201709 ngmapi-0.0.2/
--rw-r--r--   0 ngmaibulat   (502) staff       (20)      375 2023-07-07 10:03:21.201410 ngmapi-0.0.2/PKG-INFO
-drwxr-xr-x   0 ngmaibulat   (502) staff       (20)        0 2023-07-07 10:03:21.198073 ngmapi-0.0.2/ngmapi/
--rw-r--r--   0 ngmaibulat   (502) staff       (20)        0 2023-07-07 06:42:48.000000 ngmapi-0.0.2/ngmapi/__init__.py
--rw-r--r--   0 ngmaibulat   (502) staff       (20)      258 2023-07-07 09:46:14.000000 ngmapi-0.0.2/ngmapi/app.py
--rw-r--r--   0 ngmaibulat   (502) staff       (20)       32 2023-07-07 09:46:31.000000 ngmapi-0.0.2/ngmapi/func.py
-drwxr-xr-x   0 ngmaibulat   (502) staff       (20)        0 2023-07-07 10:03:21.200476 ngmapi-0.0.2/ngmapi.egg-info/
--rw-r--r--   0 ngmaibulat   (502) staff       (20)      375 2023-07-07 10:03:21.000000 ngmapi-0.0.2/ngmapi.egg-info/PKG-INFO
--rw-r--r--   0 ngmaibulat   (502) staff       (20)      262 2023-07-07 10:03:21.000000 ngmapi-0.0.2/ngmapi.egg-info/SOURCES.txt
--rw-r--r--   0 ngmaibulat   (502) staff       (20)        1 2023-07-07 10:03:21.000000 ngmapi-0.0.2/ngmapi.egg-info/dependency_links.txt
--rw-r--r--   0 ngmaibulat   (502) staff       (20)       40 2023-07-07 10:03:21.000000 ngmapi-0.0.2/ngmapi.egg-info/entry_points.txt
--rw-r--r--   0 ngmaibulat   (502) staff       (20)       24 2023-07-07 10:03:21.000000 ngmapi-0.0.2/ngmapi.egg-info/requires.txt
--rw-r--r--   0 ngmaibulat   (502) staff       (20)        7 2023-07-07 10:03:21.000000 ngmapi-0.0.2/ngmapi.egg-info/top_level.txt
--rw-r--r--   0 ngmaibulat   (502) staff       (20)      542 2023-07-07 10:01:41.000000 ngmapi-0.0.2/pyproject.toml
--rw-r--r--   0 ngmaibulat   (502) staff       (20)       38 2023-07-07 10:03:21.201800 ngmapi-0.0.2/setup.cfg
-drwxr-xr-x   0 ngmaibulat   (502) staff       (20)        0 2023-07-07 10:03:21.200850 ngmapi-0.0.2/tests/
--rw-r--r--   0 ngmaibulat   (502) staff       (20)      285 2023-07-07 09:46:42.000000 ngmapi-0.0.2/tests/test_add.py
+drwxr-xr-x   0 ngmaibulat   (502) staff       (20)        0 2023-07-07 10:16:13.081674 ngmapi-0.0.3/
+-rw-r--r--   0 ngmaibulat   (502) staff       (20)      375 2023-07-07 10:16:13.081168 ngmapi-0.0.3/PKG-INFO
+drwxr-xr-x   0 ngmaibulat   (502) staff       (20)        0 2023-07-07 10:16:13.075989 ngmapi-0.0.3/ngmapi/
+-rw-r--r--   0 ngmaibulat   (502) staff       (20)        0 2023-07-07 06:42:48.000000 ngmapi-0.0.3/ngmapi/__init__.py
+-rw-r--r--   0 ngmaibulat   (502) staff       (20)       95 2023-07-07 10:11:21.000000 ngmapi-0.0.3/ngmapi/__main__.py
+-rw-r--r--   0 ngmaibulat   (502) staff       (20)      258 2023-07-07 09:46:14.000000 ngmapi-0.0.3/ngmapi/app.py
+-rw-r--r--   0 ngmaibulat   (502) staff       (20)       32 2023-07-07 09:46:31.000000 ngmapi-0.0.3/ngmapi/func.py
+drwxr-xr-x   0 ngmaibulat   (502) staff       (20)        0 2023-07-07 10:16:13.079543 ngmapi-0.0.3/ngmapi.egg-info/
+-rw-r--r--   0 ngmaibulat   (502) staff       (20)      375 2023-07-07 10:16:13.000000 ngmapi-0.0.3/ngmapi.egg-info/PKG-INFO
+-rw-r--r--   0 ngmaibulat   (502) staff       (20)      281 2023-07-07 10:16:13.000000 ngmapi-0.0.3/ngmapi.egg-info/SOURCES.txt
+-rw-r--r--   0 ngmaibulat   (502) staff       (20)        1 2023-07-07 10:16:13.000000 ngmapi-0.0.3/ngmapi.egg-info/dependency_links.txt
+-rw-r--r--   0 ngmaibulat   (502) staff       (20)       48 2023-07-07 10:16:13.000000 ngmapi-0.0.3/ngmapi.egg-info/entry_points.txt
+-rw-r--r--   0 ngmaibulat   (502) staff       (20)       24 2023-07-07 10:16:13.000000 ngmapi-0.0.3/ngmapi.egg-info/requires.txt
+-rw-r--r--   0 ngmaibulat   (502) staff       (20)        7 2023-07-07 10:16:13.000000 ngmapi-0.0.3/ngmapi.egg-info/top_level.txt
+-rw-r--r--   0 ngmaibulat   (502) staff       (20)      550 2023-07-07 10:13:40.000000 ngmapi-0.0.3/pyproject.toml
+-rw-r--r--   0 ngmaibulat   (502) staff       (20)       38 2023-07-07 10:16:13.081836 ngmapi-0.0.3/setup.cfg
+drwxr-xr-x   0 ngmaibulat   (502) staff       (20)        0 2023-07-07 10:16:13.080107 ngmapi-0.0.3/tests/
+-rw-r--r--   0 ngmaibulat   (502) staff       (20)      285 2023-07-07 09:46:42.000000 ngmapi-0.0.3/tests/test_add.py
```

### Comparing `ngmapi-0.0.2/pyproject.toml` & `ngmapi-0.0.3/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ngmapi"
-version = "0.0.2"
+version = "0.0.3"
 description = "Just a demo project"
 readme = "README.md"
 requires-python = ">=3.10"
 keywords = ["flask", "project"]
 dependencies = [
     "Flask",
     "Jinja2",
@@ -13,12 +13,12 @@
 
 [project.urls]
 Homepage = "https://github.com/ngmaibulat/training-flask"
 Documentation = "https://github.com/ngmaibulat/training-flask"
 Changes = "https://github.com/ngmaibulat/training-flask"
 
 [project.scripts]
-ngmapi = "bin.app:main"
+ngmapi = "ngmapi.__main__:main"
 
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
```

