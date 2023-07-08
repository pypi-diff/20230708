# Comparing `tmp/botocore-a-la-carte-grafana-1.30.1.tar.gz` & `tmp/botocore-a-la-carte-grafana-1.31.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botocore-a-la-carte-grafana-1.30.1.tar", last modified: Thu Jul  6 01:44:59 2023, max compression
+gzip compressed data, was "botocore-a-la-carte-grafana-1.31.0.tar", last modified: Fri Jul  7 01:43:50 2023, max compression
```

## Comparing `botocore-a-la-carte-grafana-1.30.1.tar` & `botocore-a-la-carte-grafana-1.31.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 01:44:59.666717 botocore-a-la-carte-grafana-1.30.1/
--rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-07-06 01:44:59.000000 botocore-a-la-carte-grafana-1.30.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      957 2023-07-06 01:44:59.666717 botocore-a-la-carte-grafana-1.30.1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 01:44:59.666717 botocore-a-la-carte-grafana-1.30.1/botocore/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 01:44:59.666717 botocore-a-la-carte-grafana-1.30.1/botocore/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 01:44:59.666717 botocore-a-la-carte-grafana-1.30.1/botocore/data/grafana/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 01:44:59.666717 botocore-a-la-carte-grafana-1.30.1/botocore/data/grafana/2020-08-18/
--rw-r--r--   0 runner    (1001) docker     (123)    17628 2023-07-06 01:44:40.000000 botocore-a-la-carte-grafana-1.30.1/botocore/data/grafana/2020-08-18/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-06 01:44:40.000000 botocore-a-la-carte-grafana-1.30.1/botocore/data/grafana/2020-08-18/examples-1.json
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-07-06 01:44:40.000000 botocore-a-la-carte-grafana-1.30.1/botocore/data/grafana/2020-08-18/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    81104 2023-07-06 01:44:40.000000 botocore-a-la-carte-grafana-1.30.1/botocore/data/grafana/2020-08-18/service-2.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 01:44:59.666717 botocore-a-la-carte-grafana-1.30.1/botocore_a_la_carte_grafana.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      957 2023-07-06 01:44:59.000000 botocore-a-la-carte-grafana-1.30.1/botocore_a_la_carte_grafana.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-07-06 01:44:59.000000 botocore-a-la-carte-grafana-1.30.1/botocore_a_la_carte_grafana.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 01:44:59.000000 botocore-a-la-carte-grafana-1.30.1/botocore_a_la_carte_grafana.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-06 01:44:59.000000 botocore-a-la-carte-grafana-1.30.1/botocore_a_la_carte_grafana.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 01:44:59.666717 botocore-a-la-carte-grafana-1.30.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-07-06 01:44:59.000000 botocore-a-la-carte-grafana-1.30.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 01:43:50.171246 botocore-a-la-carte-grafana-1.31.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-07-07 01:43:49.000000 botocore-a-la-carte-grafana-1.31.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-07-07 01:43:50.171246 botocore-a-la-carte-grafana-1.31.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 01:43:50.167246 botocore-a-la-carte-grafana-1.31.0/botocore/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 01:43:50.167246 botocore-a-la-carte-grafana-1.31.0/botocore/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 01:43:50.167246 botocore-a-la-carte-grafana-1.31.0/botocore/data/grafana/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 01:43:50.171246 botocore-a-la-carte-grafana-1.31.0/botocore/data/grafana/2020-08-18/
+-rw-r--r--   0 runner    (1001) docker     (123)    17628 2023-07-07 01:43:28.000000 botocore-a-la-carte-grafana-1.31.0/botocore/data/grafana/2020-08-18/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-07 01:43:28.000000 botocore-a-la-carte-grafana-1.31.0/botocore/data/grafana/2020-08-18/examples-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-07-07 01:43:28.000000 botocore-a-la-carte-grafana-1.31.0/botocore/data/grafana/2020-08-18/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    81104 2023-07-07 01:43:28.000000 botocore-a-la-carte-grafana-1.31.0/botocore/data/grafana/2020-08-18/service-2.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 01:43:50.171246 botocore-a-la-carte-grafana-1.31.0/botocore_a_la_carte_grafana.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-07-07 01:43:50.000000 botocore-a-la-carte-grafana-1.31.0/botocore_a_la_carte_grafana.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-07-07 01:43:50.000000 botocore-a-la-carte-grafana-1.31.0/botocore_a_la_carte_grafana.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 01:43:50.000000 botocore-a-la-carte-grafana-1.31.0/botocore_a_la_carte_grafana.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-07 01:43:50.000000 botocore-a-la-carte-grafana-1.31.0/botocore_a_la_carte_grafana.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 01:43:50.171246 botocore-a-la-carte-grafana-1.31.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-07-07 01:43:49.000000 botocore-a-la-carte-grafana-1.31.0/setup.py
```

### Comparing `botocore-a-la-carte-grafana-1.30.1/LICENSE.txt` & `botocore-a-la-carte-grafana-1.31.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-grafana-1.30.1/PKG-INFO` & `botocore-a-la-carte-grafana-1.31.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-grafana
-Version: 1.30.1
+Version: 1.31.0
 Summary: grafana data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-grafana-1.30.1/botocore/data/grafana/2020-08-18/endpoint-rule-set-1.json` & `botocore-a-la-carte-grafana-1.31.0/botocore/data/grafana/2020-08-18/endpoint-rule-set-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-grafana-1.30.1/botocore/data/grafana/2020-08-18/service-2.json` & `botocore-a-la-carte-grafana-1.31.0/botocore/data/grafana/2020-08-18/service-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-grafana-1.30.1/botocore_a_la_carte_grafana.egg-info/PKG-INFO` & `botocore-a-la-carte-grafana-1.31.0/botocore_a_la_carte_grafana.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-grafana
-Version: 1.30.1
+Version: 1.31.0
 Summary: grafana data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-grafana-1.30.1/setup.py` & `botocore-a-la-carte-grafana-1.31.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import setup
 
 setup(
     name='botocore-a-la-carte-grafana',
-    version="1.30.1",
+    version="1.31.0",
     description='grafana data for botocore. See the `botocore-a-la-carte` package for more info.',
     author='Amazon Web Services',
     url='https://github.com/thejcannon/botocore-a-la-carte',
     scripts=[],
     packages=["botocore"],
     package_data={
         'botocore': ['data/grafana/*/*.json'],
```

