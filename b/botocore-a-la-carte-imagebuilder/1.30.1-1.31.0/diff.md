# Comparing `tmp/botocore-a-la-carte-imagebuilder-1.30.1.tar.gz` & `tmp/botocore-a-la-carte-imagebuilder-1.31.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botocore-a-la-carte-imagebuilder-1.30.1.tar", last modified: Thu Jul  6 01:45:02 2023, max compression
+gzip compressed data, was "botocore-a-la-carte-imagebuilder-1.31.0.tar", last modified: Fri Jul  7 01:43:53 2023, max compression
```

## Comparing `botocore-a-la-carte-imagebuilder-1.30.1.tar` & `botocore-a-la-carte-imagebuilder-1.31.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 01:45:02.506760 botocore-a-la-carte-imagebuilder-1.30.1/
--rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-07-06 01:45:02.000000 botocore-a-la-carte-imagebuilder-1.30.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-07-06 01:45:02.506760 botocore-a-la-carte-imagebuilder-1.30.1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 01:45:02.502760 botocore-a-la-carte-imagebuilder-1.30.1/botocore/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 01:45:02.502760 botocore-a-la-carte-imagebuilder-1.30.1/botocore/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 01:45:02.502760 botocore-a-la-carte-imagebuilder-1.30.1/botocore/data/imagebuilder/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 01:45:02.502760 botocore-a-la-carte-imagebuilder-1.30.1/botocore/data/imagebuilder/2019-12-02/
--rw-r--r--   0 runner    (1001) docker     (123)    19620 2023-07-06 01:44:40.000000 botocore-a-la-carte-imagebuilder-1.30.1/botocore/data/imagebuilder/2019-12-02/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-06 01:44:40.000000 botocore-a-la-carte-imagebuilder-1.30.1/botocore/data/imagebuilder/2019-12-02/examples-1.json
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-06 01:44:40.000000 botocore-a-la-carte-imagebuilder-1.30.1/botocore/data/imagebuilder/2019-12-02/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (123)   261754 2023-07-06 01:44:40.000000 botocore-a-la-carte-imagebuilder-1.30.1/botocore/data/imagebuilder/2019-12-02/service-2.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 01:45:02.506760 botocore-a-la-carte-imagebuilder-1.30.1/botocore_a_la_carte_imagebuilder.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-07-06 01:45:02.000000 botocore-a-la-carte-imagebuilder-1.30.1/botocore_a_la_carte_imagebuilder.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-07-06 01:45:02.000000 botocore-a-la-carte-imagebuilder-1.30.1/botocore_a_la_carte_imagebuilder.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 01:45:02.000000 botocore-a-la-carte-imagebuilder-1.30.1/botocore_a_la_carte_imagebuilder.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-06 01:45:02.000000 botocore-a-la-carte-imagebuilder-1.30.1/botocore_a_la_carte_imagebuilder.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 01:45:02.506760 botocore-a-la-carte-imagebuilder-1.30.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-07-06 01:45:02.000000 botocore-a-la-carte-imagebuilder-1.30.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 01:43:53.135290 botocore-a-la-carte-imagebuilder-1.31.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-07-07 01:43:52.000000 botocore-a-la-carte-imagebuilder-1.31.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-07-07 01:43:53.135290 botocore-a-la-carte-imagebuilder-1.31.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 01:43:53.135290 botocore-a-la-carte-imagebuilder-1.31.0/botocore/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 01:43:53.135290 botocore-a-la-carte-imagebuilder-1.31.0/botocore/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 01:43:53.135290 botocore-a-la-carte-imagebuilder-1.31.0/botocore/data/imagebuilder/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 01:43:53.135290 botocore-a-la-carte-imagebuilder-1.31.0/botocore/data/imagebuilder/2019-12-02/
+-rw-r--r--   0 runner    (1001) docker     (123)    19620 2023-07-07 01:43:28.000000 botocore-a-la-carte-imagebuilder-1.31.0/botocore/data/imagebuilder/2019-12-02/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-07 01:43:28.000000 botocore-a-la-carte-imagebuilder-1.31.0/botocore/data/imagebuilder/2019-12-02/examples-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-07 01:43:28.000000 botocore-a-la-carte-imagebuilder-1.31.0/botocore/data/imagebuilder/2019-12-02/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)   261754 2023-07-07 01:43:28.000000 botocore-a-la-carte-imagebuilder-1.31.0/botocore/data/imagebuilder/2019-12-02/service-2.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 01:43:53.135290 botocore-a-la-carte-imagebuilder-1.31.0/botocore_a_la_carte_imagebuilder.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-07-07 01:43:53.000000 botocore-a-la-carte-imagebuilder-1.31.0/botocore_a_la_carte_imagebuilder.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-07-07 01:43:53.000000 botocore-a-la-carte-imagebuilder-1.31.0/botocore_a_la_carte_imagebuilder.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 01:43:53.000000 botocore-a-la-carte-imagebuilder-1.31.0/botocore_a_la_carte_imagebuilder.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-07 01:43:53.000000 botocore-a-la-carte-imagebuilder-1.31.0/botocore_a_la_carte_imagebuilder.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 01:43:53.135290 botocore-a-la-carte-imagebuilder-1.31.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-07-07 01:43:52.000000 botocore-a-la-carte-imagebuilder-1.31.0/setup.py
```

### Comparing `botocore-a-la-carte-imagebuilder-1.30.1/LICENSE.txt` & `botocore-a-la-carte-imagebuilder-1.31.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-imagebuilder-1.30.1/PKG-INFO` & `botocore-a-la-carte-imagebuilder-1.31.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-imagebuilder
-Version: 1.30.1
+Version: 1.31.0
 Summary: imagebuilder data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-imagebuilder-1.30.1/botocore/data/imagebuilder/2019-12-02/endpoint-rule-set-1.json` & `botocore-a-la-carte-imagebuilder-1.31.0/botocore/data/imagebuilder/2019-12-02/endpoint-rule-set-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-imagebuilder-1.30.1/botocore/data/imagebuilder/2019-12-02/service-2.json` & `botocore-a-la-carte-imagebuilder-1.31.0/botocore/data/imagebuilder/2019-12-02/service-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-imagebuilder-1.30.1/botocore_a_la_carte_imagebuilder.egg-info/PKG-INFO` & `botocore-a-la-carte-imagebuilder-1.31.0/botocore_a_la_carte_imagebuilder.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-imagebuilder
-Version: 1.30.1
+Version: 1.31.0
 Summary: imagebuilder data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-imagebuilder-1.30.1/setup.py` & `botocore-a-la-carte-imagebuilder-1.31.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import setup
 
 setup(
     name='botocore-a-la-carte-imagebuilder',
-    version="1.30.1",
+    version="1.31.0",
     description='imagebuilder data for botocore. See the `botocore-a-la-carte` package for more info.',
     author='Amazon Web Services',
     url='https://github.com/thejcannon/botocore-a-la-carte',
     scripts=[],
     packages=["botocore"],
     package_data={
         'botocore': ['data/imagebuilder/*/*.json'],
```

