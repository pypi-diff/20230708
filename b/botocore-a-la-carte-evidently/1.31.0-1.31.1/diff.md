# Comparing `tmp/botocore-a-la-carte-evidently-1.31.0.tar.gz` & `tmp/botocore-a-la-carte-evidently-1.31.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botocore-a-la-carte-evidently-1.31.0.tar", last modified: Fri Jul  7 01:43:59 2023, max compression
+gzip compressed data, was "botocore-a-la-carte-evidently-1.31.1.tar", last modified: Sat Jul  8 01:42:24 2023, max compression
```

## Comparing `botocore-a-la-carte-evidently-1.31.0.tar` & `botocore-a-la-carte-evidently-1.31.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 01:43:59.043374 botocore-a-la-carte-evidently-1.31.0/
--rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-07-07 01:43:58.000000 botocore-a-la-carte-evidently-1.31.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      961 2023-07-07 01:43:59.043374 botocore-a-la-carte-evidently-1.31.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 01:43:59.039374 botocore-a-la-carte-evidently-1.31.0/botocore/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 01:43:59.039374 botocore-a-la-carte-evidently-1.31.0/botocore/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 01:43:59.039374 botocore-a-la-carte-evidently-1.31.0/botocore/data/evidently/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 01:43:59.039374 botocore-a-la-carte-evidently-1.31.0/botocore/data/evidently/2021-02-01/
--rw-r--r--   0 runner    (1001) docker     (123)    17636 2023-07-07 01:43:28.000000 botocore-a-la-carte-evidently-1.31.0/botocore/data/evidently/2021-02-01/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-07 01:43:28.000000 botocore-a-la-carte-evidently-1.31.0/botocore/data/evidently/2021-02-01/examples-1.json
--rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-07-07 01:43:28.000000 botocore-a-la-carte-evidently-1.31.0/botocore/data/evidently/2021-02-01/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (123)   165834 2023-07-07 01:43:28.000000 botocore-a-la-carte-evidently-1.31.0/botocore/data/evidently/2021-02-01/service-2.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 01:43:59.039374 botocore-a-la-carte-evidently-1.31.0/botocore_a_la_carte_evidently.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      961 2023-07-07 01:43:59.000000 botocore-a-la-carte-evidently-1.31.0/botocore_a_la_carte_evidently.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-07-07 01:43:59.000000 botocore-a-la-carte-evidently-1.31.0/botocore_a_la_carte_evidently.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 01:43:59.000000 botocore-a-la-carte-evidently-1.31.0/botocore_a_la_carte_evidently.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-07 01:43:59.000000 botocore-a-la-carte-evidently-1.31.0/botocore_a_la_carte_evidently.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 01:43:59.043374 botocore-a-la-carte-evidently-1.31.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-07-07 01:43:58.000000 botocore-a-la-carte-evidently-1.31.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:42:24.070712 botocore-a-la-carte-evidently-1.31.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-07-08 01:42:23.000000 botocore-a-la-carte-evidently-1.31.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      961 2023-07-08 01:42:24.070712 botocore-a-la-carte-evidently-1.31.1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:42:24.070712 botocore-a-la-carte-evidently-1.31.1/botocore/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:42:24.070712 botocore-a-la-carte-evidently-1.31.1/botocore/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:42:24.070712 botocore-a-la-carte-evidently-1.31.1/botocore/data/evidently/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:42:24.070712 botocore-a-la-carte-evidently-1.31.1/botocore/data/evidently/2021-02-01/
+-rw-r--r--   0 runner    (1001) docker     (123)    17636 2023-07-08 01:41:59.000000 botocore-a-la-carte-evidently-1.31.1/botocore/data/evidently/2021-02-01/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-08 01:41:59.000000 botocore-a-la-carte-evidently-1.31.1/botocore/data/evidently/2021-02-01/examples-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-07-08 01:41:59.000000 botocore-a-la-carte-evidently-1.31.1/botocore/data/evidently/2021-02-01/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)   165834 2023-07-08 01:41:59.000000 botocore-a-la-carte-evidently-1.31.1/botocore/data/evidently/2021-02-01/service-2.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:42:24.070712 botocore-a-la-carte-evidently-1.31.1/botocore_a_la_carte_evidently.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      961 2023-07-08 01:42:24.000000 botocore-a-la-carte-evidently-1.31.1/botocore_a_la_carte_evidently.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-07-08 01:42:24.000000 botocore-a-la-carte-evidently-1.31.1/botocore_a_la_carte_evidently.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:42:24.000000 botocore-a-la-carte-evidently-1.31.1/botocore_a_la_carte_evidently.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-08 01:42:24.000000 botocore-a-la-carte-evidently-1.31.1/botocore_a_la_carte_evidently.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:42:24.070712 botocore-a-la-carte-evidently-1.31.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-07-08 01:42:23.000000 botocore-a-la-carte-evidently-1.31.1/setup.py
```

### Comparing `botocore-a-la-carte-evidently-1.31.0/LICENSE.txt` & `botocore-a-la-carte-evidently-1.31.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-evidently-1.31.0/PKG-INFO` & `botocore-a-la-carte-evidently-1.31.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-evidently
-Version: 1.31.0
+Version: 1.31.1
 Summary: evidently data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-evidently-1.31.0/botocore/data/evidently/2021-02-01/endpoint-rule-set-1.json` & `botocore-a-la-carte-evidently-1.31.1/botocore/data/evidently/2021-02-01/endpoint-rule-set-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-evidently-1.31.0/botocore/data/evidently/2021-02-01/paginators-1.json` & `botocore-a-la-carte-evidently-1.31.1/botocore/data/evidently/2021-02-01/paginators-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-evidently-1.31.0/botocore/data/evidently/2021-02-01/service-2.json` & `botocore-a-la-carte-evidently-1.31.1/botocore/data/evidently/2021-02-01/service-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-evidently-1.31.0/botocore_a_la_carte_evidently.egg-info/PKG-INFO` & `botocore-a-la-carte-evidently-1.31.1/botocore_a_la_carte_evidently.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-evidently
-Version: 1.31.0
+Version: 1.31.1
 Summary: evidently data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-evidently-1.31.0/setup.py` & `botocore-a-la-carte-evidently-1.31.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import setup
 
 setup(
     name='botocore-a-la-carte-evidently',
-    version="1.31.0",
+    version="1.31.1",
     description='evidently data for botocore. See the `botocore-a-la-carte` package for more info.',
     author='Amazon Web Services',
     url='https://github.com/thejcannon/botocore-a-la-carte',
     scripts=[],
     packages=["botocore"],
     package_data={
         'botocore': ['data/evidently/*/*.json'],
```

