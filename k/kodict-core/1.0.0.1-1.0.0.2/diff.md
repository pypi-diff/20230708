# Comparing `tmp/kodict_core-1.0.0.1.tar.gz` & `tmp/kodict_core-1.0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kodict_core-1.0.0.1.tar", last modified: Fri Jul  7 22:19:43 2023, max compression
+gzip compressed data, was "kodict_core-1.0.0.2.tar", last modified: Fri Jul  7 22:26:06 2023, max compression
```

## Comparing `kodict_core-1.0.0.1.tar` & `kodict_core-1.0.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 k         (1000) k         (1001)        0 2023-07-07 22:19:43.317362 kodict_core-1.0.0.1/
--rw-r--r--   0 k         (1000) k         (1001)      598 2023-07-07 22:19:43.317362 kodict_core-1.0.0.1/PKG-INFO
--rw-r--r--   0 k         (1000) k         (1001)      389 2023-07-07 22:10:02.000000 kodict_core-1.0.0.1/README.md
--rw-r--r--   0 k         (1000) k         (1001)      715 2023-07-07 22:19:43.317362 kodict_core-1.0.0.1/setup.cfg
--rw-r--r--   0 k         (1000) k         (1001)       69 2023-07-07 05:07:27.000000 kodict_core-1.0.0.1/setup.py
-drwxr-xr-x   0 k         (1000) k         (1001)        0 2023-07-07 22:19:43.314029 kodict_core-1.0.0.1/src/
-drwxr-xr-x   0 k         (1000) k         (1001)        0 2023-07-07 22:19:43.314029 kodict_core-1.0.0.1/src/kodict_core/
--rw-r--r--   0 k         (1000) k         (1001)        0 2023-07-07 06:19:28.000000 kodict_core-1.0.0.1/src/kodict_core/__init__.py
--rw-r--r--   0 k         (1000) k         (1001)      596 2023-07-07 06:32:10.000000 kodict_core-1.0.0.1/src/kodict_core/main.py
-drwxr-xr-x   0 k         (1000) k         (1001)        0 2023-07-07 22:19:43.317362 kodict_core-1.0.0.1/src/kodict_core/services/
--rw-r--r--   0 k         (1000) k         (1001)     1526 2023-07-07 06:32:09.000000 kodict_core-1.0.0.1/src/kodict_core/services/deepl.py
--rw-r--r--   0 k         (1000) k         (1001)     4541 2023-07-07 06:32:10.000000 kodict_core-1.0.0.1/src/kodict_core/services/krdict.py
-drwxr-xr-x   0 k         (1000) k         (1001)        0 2023-07-07 22:19:43.317362 kodict_core-1.0.0.1/src/kodict_core.egg-info/
--rw-r--r--   0 k         (1000) k         (1001)      598 2023-07-07 22:19:43.000000 kodict_core-1.0.0.1/src/kodict_core.egg-info/PKG-INFO
--rw-r--r--   0 k         (1000) k         (1001)      305 2023-07-07 22:19:43.000000 kodict_core-1.0.0.1/src/kodict_core.egg-info/SOURCES.txt
--rw-r--r--   0 k         (1000) k         (1001)        1 2023-07-07 22:19:43.000000 kodict_core-1.0.0.1/src/kodict_core.egg-info/dependency_links.txt
--rw-r--r--   0 k         (1000) k         (1001)       12 2023-07-07 22:19:43.000000 kodict_core-1.0.0.1/src/kodict_core.egg-info/top_level.txt
+drwxr-xr-x   0 k         (1000) k         (1001)        0 2023-07-07 22:26:06.259410 kodict_core-1.0.0.2/
+-rw-r--r--   0 k         (1000) k         (1001)      988 2023-07-07 22:26:06.259410 kodict_core-1.0.0.2/PKG-INFO
+-rw-r--r--   0 k         (1000) k         (1001)      389 2023-07-07 22:24:58.000000 kodict_core-1.0.0.2/README.md
+-rw-r--r--   0 k         (1000) k         (1001)      750 2023-07-07 22:26:06.262743 kodict_core-1.0.0.2/setup.cfg
+-rw-r--r--   0 k         (1000) k         (1001)       69 2023-07-07 05:07:27.000000 kodict_core-1.0.0.2/setup.py
+drwxr-xr-x   0 k         (1000) k         (1001)        0 2023-07-07 22:26:06.256076 kodict_core-1.0.0.2/src/
+drwxr-xr-x   0 k         (1000) k         (1001)        0 2023-07-07 22:26:06.259410 kodict_core-1.0.0.2/src/kodict_core/
+-rw-r--r--   0 k         (1000) k         (1001)        0 2023-07-07 06:19:28.000000 kodict_core-1.0.0.2/src/kodict_core/__init__.py
+-rw-r--r--   0 k         (1000) k         (1001)      596 2023-07-07 06:32:10.000000 kodict_core-1.0.0.2/src/kodict_core/main.py
+drwxr-xr-x   0 k         (1000) k         (1001)        0 2023-07-07 22:26:06.259410 kodict_core-1.0.0.2/src/kodict_core/services/
+-rw-r--r--   0 k         (1000) k         (1001)     1526 2023-07-07 06:32:09.000000 kodict_core-1.0.0.2/src/kodict_core/services/deepl.py
+-rw-r--r--   0 k         (1000) k         (1001)     4541 2023-07-07 06:32:10.000000 kodict_core-1.0.0.2/src/kodict_core/services/krdict.py
+drwxr-xr-x   0 k         (1000) k         (1001)        0 2023-07-07 22:26:06.259410 kodict_core-1.0.0.2/src/kodict_core.egg-info/
+-rw-r--r--   0 k         (1000) k         (1001)      988 2023-07-07 22:26:06.000000 kodict_core-1.0.0.2/src/kodict_core.egg-info/PKG-INFO
+-rw-r--r--   0 k         (1000) k         (1001)      305 2023-07-07 22:26:06.000000 kodict_core-1.0.0.2/src/kodict_core.egg-info/SOURCES.txt
+-rw-r--r--   0 k         (1000) k         (1001)        1 2023-07-07 22:26:06.000000 kodict_core-1.0.0.2/src/kodict_core.egg-info/dependency_links.txt
+-rw-r--r--   0 k         (1000) k         (1001)       12 2023-07-07 22:26:06.000000 kodict_core-1.0.0.2/src/kodict_core.egg-info/top_level.txt
```

### Comparing `kodict_core-1.0.0.1/setup.cfg` & `kodict_core-1.0.0.2/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 [metadata]
 name = kodict_core
-version = 1.0.0.1
+version = 1.0.0.2
 author = coffeebank
 description = A Korean Dictionary bot for searching language and vocabulary information from Krdict and DeepL.
+long_description = file: README.md
 keywords = korean dictionary api
 url = https://github.com/coffeebank/kodict_core
 project_urls = 
 	Source Code = https://github.com/coffeebank/kodict_core
 	Bug Tracker = https://github.com/coffeebank/kodict_core/issues
 	Documentation = https://github.com/coffeebank/kodict_core
 classifiers =
```

### Comparing `kodict_core-1.0.0.1/src/kodict_core/main.py` & `kodict_core-1.0.0.2/src/kodict_core/main.py`

 * *Files identical despite different names*

### Comparing `kodict_core-1.0.0.1/src/kodict_core/services/deepl.py` & `kodict_core-1.0.0.2/src/kodict_core/services/deepl.py`

 * *Files identical despite different names*

### Comparing `kodict_core-1.0.0.1/src/kodict_core/services/krdict.py` & `kodict_core-1.0.0.2/src/kodict_core/services/krdict.py`

 * *Files identical despite different names*

