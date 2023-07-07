# Comparing `tmp/otio-aaf-adapter-0.15.0.dev1.tar.gz` & `tmp/otio-aaf-adapter-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "otio-aaf-adapter-0.15.0.dev1.tar", last modified: Fri Jul  7 22:06:47 2023, max compression
+gzip compressed data, was "otio-aaf-adapter-1.0.0.tar", last modified: Fri Jul  7 22:16:50 2023, max compression
```

## Comparing `otio-aaf-adapter-0.15.0.dev1.tar` & `otio-aaf-adapter-1.0.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 22:06:47.879032 otio-aaf-adapter-0.15.0.dev1/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-07-07 22:06:39.000000 otio-aaf-adapter-0.15.0.dev1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3817 2023-07-07 22:06:47.879032 otio-aaf-adapter-0.15.0.dev1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-07-07 22:06:39.000000 otio-aaf-adapter-0.15.0.dev1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-07-07 22:06:47.879032 otio-aaf-adapter-0.15.0.dev1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-07-07 22:06:39.000000 otio-aaf-adapter-0.15.0.dev1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 22:06:47.871032 otio-aaf-adapter-0.15.0.dev1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 22:06:47.875032 otio-aaf-adapter-0.15.0.dev1/src/otio_aaf_adapter/
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-07-07 22:06:39.000000 otio-aaf-adapter-0.15.0.dev1/src/otio_aaf_adapter/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 22:06:47.875032 otio-aaf-adapter-0.15.0.dev1/src/otio_aaf_adapter/adapters/
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-07 22:06:39.000000 otio-aaf-adapter-0.15.0.dev1/src/otio_aaf_adapter/adapters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 22:06:47.875032 otio-aaf-adapter-0.15.0.dev1/src/otio_aaf_adapter/adapters/aaf_adapter/
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-07 22:06:39.000000 otio-aaf-adapter-0.15.0.dev1/src/otio_aaf_adapter/adapters/aaf_adapter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    30972 2023-07-07 22:06:39.000000 otio-aaf-adapter-0.15.0.dev1/src/otio_aaf_adapter/adapters/aaf_adapter/aaf_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)    61229 2023-07-07 22:06:39.000000 otio-aaf-adapter-0.15.0.dev1/src/otio_aaf_adapter/adapters/advanced_authoring_format.py
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-07-07 22:06:39.000000 otio-aaf-adapter-0.15.0.dev1/src/otio_aaf_adapter/plugin_manifest.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 22:06:47.875032 otio-aaf-adapter-0.15.0.dev1/src/otio_aaf_adapter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3817 2023-07-07 22:06:47.000000 otio-aaf-adapter-0.15.0.dev1/src/otio_aaf_adapter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-07-07 22:06:47.000000 otio-aaf-adapter-0.15.0.dev1/src/otio_aaf_adapter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 22:06:47.000000 otio-aaf-adapter-0.15.0.dev1/src/otio_aaf_adapter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-07 22:06:47.000000 otio-aaf-adapter-0.15.0.dev1/src/otio_aaf_adapter.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-07 22:06:47.000000 otio-aaf-adapter-0.15.0.dev1/src/otio_aaf_adapter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-07 22:06:47.000000 otio-aaf-adapter-0.15.0.dev1/src/otio_aaf_adapter.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 22:06:47.879032 otio-aaf-adapter-0.15.0.dev1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    81937 2023-07-07 22:06:39.000000 otio-aaf-adapter-0.15.0.dev1/tests/test_aaf_adapter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 22:16:50.919180 otio-aaf-adapter-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-07-07 22:16:42.000000 otio-aaf-adapter-1.0.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3811 2023-07-07 22:16:50.919180 otio-aaf-adapter-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-07-07 22:16:42.000000 otio-aaf-adapter-1.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-07-07 22:16:50.919180 otio-aaf-adapter-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-07-07 22:16:42.000000 otio-aaf-adapter-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 22:16:50.911180 otio-aaf-adapter-1.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 22:16:50.915180 otio-aaf-adapter-1.0.0/src/otio_aaf_adapter/
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-07-07 22:16:42.000000 otio-aaf-adapter-1.0.0/src/otio_aaf_adapter/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 22:16:50.919180 otio-aaf-adapter-1.0.0/src/otio_aaf_adapter/adapters/
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-07 22:16:42.000000 otio-aaf-adapter-1.0.0/src/otio_aaf_adapter/adapters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 22:16:50.919180 otio-aaf-adapter-1.0.0/src/otio_aaf_adapter/adapters/aaf_adapter/
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-07 22:16:42.000000 otio-aaf-adapter-1.0.0/src/otio_aaf_adapter/adapters/aaf_adapter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30972 2023-07-07 22:16:42.000000 otio-aaf-adapter-1.0.0/src/otio_aaf_adapter/adapters/aaf_adapter/aaf_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61229 2023-07-07 22:16:42.000000 otio-aaf-adapter-1.0.0/src/otio_aaf_adapter/adapters/advanced_authoring_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-07-07 22:16:42.000000 otio-aaf-adapter-1.0.0/src/otio_aaf_adapter/plugin_manifest.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 22:16:50.919180 otio-aaf-adapter-1.0.0/src/otio_aaf_adapter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3811 2023-07-07 22:16:50.000000 otio-aaf-adapter-1.0.0/src/otio_aaf_adapter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-07-07 22:16:50.000000 otio-aaf-adapter-1.0.0/src/otio_aaf_adapter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 22:16:50.000000 otio-aaf-adapter-1.0.0/src/otio_aaf_adapter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-07 22:16:50.000000 otio-aaf-adapter-1.0.0/src/otio_aaf_adapter.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-07 22:16:50.000000 otio-aaf-adapter-1.0.0/src/otio_aaf_adapter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-07 22:16:50.000000 otio-aaf-adapter-1.0.0/src/otio_aaf_adapter.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 22:16:50.919180 otio-aaf-adapter-1.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    81937 2023-07-07 22:16:42.000000 otio-aaf-adapter-1.0.0/tests/test_aaf_adapter.py
```

### Comparing `otio-aaf-adapter-0.15.0.dev1/LICENSE.txt` & `otio-aaf-adapter-1.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `otio-aaf-adapter-0.15.0.dev1/PKG-INFO` & `otio-aaf-adapter-1.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: otio-aaf-adapter
-Version: 0.15.0.dev1
+Version: 1.0.0
 Summary: OpenTimelineIO Advanced Authoring Format (AAF) Adapter
 Home-page: https://github.com/markreidvfx/otio-aaf-adapter
 Author: Contributors to the OpenTimelineIO project
 Author-email: otio-discussion@lists.aswf.io
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `otio-aaf-adapter-0.15.0.dev1/README.md` & `otio-aaf-adapter-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `otio-aaf-adapter-0.15.0.dev1/setup.py` & `otio-aaf-adapter-1.0.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     long_description = f.read()
 
 
 setuptools.setup(
     name="otio-aaf-adapter",
     author="Contributors to the OpenTimelineIO project",
     author_email="otio-discussion@lists.aswf.io",
-    version="0.15.0.dev1",
+    version="1.0.0",
     description="OpenTimelineIO Advanced Authoring Format (AAF) Adapter",
     long_description=long_description,
     long_description_content_type="text/markdown",
     # Replace url with your repo
     url="https://github.com/markreidvfx/otio-aaf-adapter",
     platforms='any',
     packages=setuptools.find_packages(where='src'),
```

### Comparing `otio-aaf-adapter-0.15.0.dev1/src/otio_aaf_adapter/adapters/aaf_adapter/aaf_writer.py` & `otio-aaf-adapter-1.0.0/src/otio_aaf_adapter/adapters/aaf_adapter/aaf_writer.py`

 * *Files identical despite different names*

### Comparing `otio-aaf-adapter-0.15.0.dev1/src/otio_aaf_adapter/adapters/advanced_authoring_format.py` & `otio-aaf-adapter-1.0.0/src/otio_aaf_adapter/adapters/advanced_authoring_format.py`

 * *Files identical despite different names*

### Comparing `otio-aaf-adapter-0.15.0.dev1/src/otio_aaf_adapter.egg-info/PKG-INFO` & `otio-aaf-adapter-1.0.0/src/otio_aaf_adapter.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: otio-aaf-adapter
-Version: 0.15.0.dev1
+Version: 1.0.0
 Summary: OpenTimelineIO Advanced Authoring Format (AAF) Adapter
 Home-page: https://github.com/markreidvfx/otio-aaf-adapter
 Author: Contributors to the OpenTimelineIO project
 Author-email: otio-discussion@lists.aswf.io
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `otio-aaf-adapter-0.15.0.dev1/src/otio_aaf_adapter.egg-info/SOURCES.txt` & `otio-aaf-adapter-1.0.0/src/otio_aaf_adapter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `otio-aaf-adapter-0.15.0.dev1/tests/test_aaf_adapter.py` & `otio-aaf-adapter-1.0.0/tests/test_aaf_adapter.py`

 * *Files identical despite different names*

