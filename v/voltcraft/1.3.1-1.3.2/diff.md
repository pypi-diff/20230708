# Comparing `tmp/voltcraft-1.3.1.tar.gz` & `tmp/voltcraft-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "voltcraft-1.3.1.tar", last modified: Sat Jul  8 08:52:35 2023, max compression
+gzip compressed data, was "voltcraft-1.3.2.tar", last modified: Sat Jul  8 08:59:27 2023, max compression
```

## Comparing `voltcraft-1.3.1.tar` & `voltcraft-1.3.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 08:52:35.155655 voltcraft-1.3.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 08:52:35.155655 voltcraft-1.3.1/.github/
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-08 08:52:25.000000 voltcraft-1.3.1/.github/FUNDING.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 08:52:35.155655 voltcraft-1.3.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-07-08 08:52:25.000000 voltcraft-1.3.1/.github/workflows/build_publish.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-07-08 08:52:25.000000 voltcraft-1.3.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-07-08 08:52:25.000000 voltcraft-1.3.1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-08 08:52:25.000000 voltcraft-1.3.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-07-08 08:52:35.155655 voltcraft-1.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-07-08 08:52:25.000000 voltcraft-1.3.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-07-08 08:52:25.000000 voltcraft-1.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      976 2023-07-08 08:52:35.155655 voltcraft-1.3.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 08:52:35.155655 voltcraft-1.3.1/voltcraft/
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-07-08 08:52:25.000000 voltcraft-1.3.1/voltcraft/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-08 08:52:35.000000 voltcraft-1.3.1/voltcraft/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     6602 2023-07-08 08:52:25.000000 voltcraft-1.3.1/voltcraft/pps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 08:52:35.155655 voltcraft-1.3.1/voltcraft.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-07-08 08:52:35.000000 voltcraft-1.3.1/voltcraft.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-07-08 08:52:35.000000 voltcraft-1.3.1/voltcraft.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 08:52:35.000000 voltcraft-1.3.1/voltcraft.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-08 08:52:35.000000 voltcraft-1.3.1/voltcraft.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-08 08:52:35.000000 voltcraft-1.3.1/voltcraft.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 08:59:27.068759 voltcraft-1.3.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 08:59:27.064759 voltcraft-1.3.2/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-08 08:59:11.000000 voltcraft-1.3.2/.github/FUNDING.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 08:59:27.064759 voltcraft-1.3.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-07-08 08:59:11.000000 voltcraft-1.3.2/.github/workflows/build_publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-07-08 08:59:11.000000 voltcraft-1.3.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-07-08 08:59:11.000000 voltcraft-1.3.2/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-08 08:59:11.000000 voltcraft-1.3.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-07-08 08:59:27.068759 voltcraft-1.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-07-08 08:59:11.000000 voltcraft-1.3.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-07-08 08:59:11.000000 voltcraft-1.3.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-07-08 08:59:27.068759 voltcraft-1.3.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 08:59:27.068759 voltcraft-1.3.2/voltcraft/
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-07-08 08:59:11.000000 voltcraft-1.3.2/voltcraft/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-08 08:59:27.000000 voltcraft-1.3.2/voltcraft/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6622 2023-07-08 08:59:11.000000 voltcraft-1.3.2/voltcraft/pps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 08:59:27.068759 voltcraft-1.3.2/voltcraft.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-07-08 08:59:27.000000 voltcraft-1.3.2/voltcraft.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-07-08 08:59:27.000000 voltcraft-1.3.2/voltcraft.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 08:59:27.000000 voltcraft-1.3.2/voltcraft.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-08 08:59:27.000000 voltcraft-1.3.2/voltcraft.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-08 08:59:27.000000 voltcraft-1.3.2/voltcraft.egg-info/top_level.txt
```

### Comparing `voltcraft-1.3.1/.github/workflows/build_publish.yaml` & `voltcraft-1.3.2/.github/workflows/build_publish.yaml`

 * *Files identical despite different names*

### Comparing `voltcraft-1.3.1/.pre-commit-config.yaml` & `voltcraft-1.3.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `voltcraft-1.3.1/LICENSE.md` & `voltcraft-1.3.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `voltcraft-1.3.1/PKG-INFO` & `voltcraft-1.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: voltcraft
-Version: 1.3.1
+Version: 1.3.2
 Summary: library for controlling Voltcraft PPS power supplies
 Home-page: https://github.com/ap--/voltcraft.git
 Download-URL: https://github.com/ap--/voltcraft
 Author: Andreas Poehlmann
 Author-email: andreas@poehlmann.io
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `voltcraft-1.3.1/README.md` & `voltcraft-1.3.2/README.md`

 * *Files identical despite different names*

### Comparing `voltcraft-1.3.1/setup.cfg` & `voltcraft-1.3.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `voltcraft-1.3.1/voltcraft/pps.py` & `voltcraft-1.3.2/voltcraft/pps.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # The model can be identified by the maximum voltage and maximum current.
 # But this is probably one of the weirdest naming-schemes I've seen...
 # It just doesn't really make sense...
 PPS_MODELS = {
     (18.0, 10.0): "PPS11810",  # not confirmed yet
     (36.2, 07.0): "PPS11360",  # confirmed
     (60.0, 02.5): "PPS11603",  # not confirmed yet
-    (18.2, 22.0): "PPS13610",  # confirmed by Yanuino 2021-12-29
+    (18.2, 22.0): "PPS13610",  # confirmed by Yanuino 2021-12-29, ersekcs 2021-11-24
     (36.2, 12.0): "PPS16005",  # confirmed
     (60.0, 05.0): "PPS11815",  # not confirmed yet
     (18.2, 12.0): "PPS11810",  # added MB 2019-01-10
     (32.2, 21.5): "DPPS3220",  # added tykling 2019-03-26
     (60.5, 11.0): "DPPS6010",
 }
```

### Comparing `voltcraft-1.3.1/voltcraft.egg-info/PKG-INFO` & `voltcraft-1.3.2/voltcraft.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: voltcraft
-Version: 1.3.1
+Version: 1.3.2
 Summary: library for controlling Voltcraft PPS power supplies
 Home-page: https://github.com/ap--/voltcraft.git
 Download-URL: https://github.com/ap--/voltcraft
 Author: Andreas Poehlmann
 Author-email: andreas@poehlmann.io
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
```

