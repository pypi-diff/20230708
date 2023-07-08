# Comparing `tmp/comwatt-client-0.1.0.tar.gz` & `tmp/comwatt-client-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "comwatt-client-0.1.0.tar", last modified: Sat Jul  8 14:14:30 2023, max compression
+gzip compressed data, was "comwatt-client-0.1.1.tar", last modified: Sat Jul  8 14:20:00 2023, max compression
```

## Comparing `comwatt-client-0.1.0.tar` & `comwatt-client-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 mat       (1000) mat       (1000)        0 2023-07-08 14:14:30.973400 comwatt-client-0.1.0/
--rw-rw-r--   0 mat       (1000) mat       (1000)      549 2023-07-08 14:14:30.973400 comwatt-client-0.1.0/PKG-INFO
--rw-rw-r--   0 mat       (1000) mat       (1000)     2706 2023-07-08 13:38:01.000000 comwatt-client-0.1.0/README.md
-drwxrwxr-x   0 mat       (1000) mat       (1000)        0 2023-07-08 14:14:30.973400 comwatt-client-0.1.0/comwatt_client.egg-info/
--rw-rw-r--   0 mat       (1000) mat       (1000)      549 2023-07-08 14:14:30.000000 comwatt-client-0.1.0/comwatt_client.egg-info/PKG-INFO
--rw-rw-r--   0 mat       (1000) mat       (1000)      237 2023-07-08 14:14:30.000000 comwatt-client-0.1.0/comwatt_client.egg-info/SOURCES.txt
--rw-rw-r--   0 mat       (1000) mat       (1000)        1 2023-07-08 14:14:30.000000 comwatt-client-0.1.0/comwatt_client.egg-info/dependency_links.txt
--rw-rw-r--   0 mat       (1000) mat       (1000)        9 2023-07-08 14:14:30.000000 comwatt-client-0.1.0/comwatt_client.egg-info/requires.txt
--rw-rw-r--   0 mat       (1000) mat       (1000)        4 2023-07-08 14:14:30.000000 comwatt-client-0.1.0/comwatt_client.egg-info/top_level.txt
--rw-rw-r--   0 mat       (1000) mat       (1000)       38 2023-07-08 14:14:30.973400 comwatt-client-0.1.0/setup.cfg
--rw-rw-r--   0 mat       (1000) mat       (1000)      649 2023-07-08 14:13:05.000000 comwatt-client-0.1.0/setup.py
-drwxrwxr-x   0 mat       (1000) mat       (1000)        0 2023-07-08 14:14:30.973400 comwatt-client-0.1.0/src/
--rw-rw-r--   0 mat       (1000) mat       (1000)        0 2023-07-08 13:37:30.000000 comwatt-client-0.1.0/src/__init__.py
--rw-rw-r--   0 mat       (1000) mat       (1000)     6043 2023-07-08 14:02:41.000000 comwatt-client-0.1.0/src/client.py
+drwxrwxr-x   0 mat       (1000) mat       (1000)        0 2023-07-08 14:20:00.526389 comwatt-client-0.1.1/
+-rw-rw-r--   0 mat       (1000) mat       (1000)      549 2023-07-08 14:20:00.526389 comwatt-client-0.1.1/PKG-INFO
+-rw-rw-r--   0 mat       (1000) mat       (1000)     2706 2023-07-08 13:38:01.000000 comwatt-client-0.1.1/README.rst
+drwxrwxr-x   0 mat       (1000) mat       (1000)        0 2023-07-08 14:20:00.526389 comwatt-client-0.1.1/comwatt_client.egg-info/
+-rw-rw-r--   0 mat       (1000) mat       (1000)      549 2023-07-08 14:20:00.000000 comwatt-client-0.1.1/comwatt_client.egg-info/PKG-INFO
+-rw-rw-r--   0 mat       (1000) mat       (1000)      238 2023-07-08 14:20:00.000000 comwatt-client-0.1.1/comwatt_client.egg-info/SOURCES.txt
+-rw-rw-r--   0 mat       (1000) mat       (1000)        1 2023-07-08 14:20:00.000000 comwatt-client-0.1.1/comwatt_client.egg-info/dependency_links.txt
+-rw-rw-r--   0 mat       (1000) mat       (1000)        9 2023-07-08 14:20:00.000000 comwatt-client-0.1.1/comwatt_client.egg-info/requires.txt
+-rw-rw-r--   0 mat       (1000) mat       (1000)        4 2023-07-08 14:20:00.000000 comwatt-client-0.1.1/comwatt_client.egg-info/top_level.txt
+-rw-rw-r--   0 mat       (1000) mat       (1000)       38 2023-07-08 14:20:00.526389 comwatt-client-0.1.1/setup.cfg
+-rw-rw-r--   0 mat       (1000) mat       (1000)      649 2023-07-08 14:19:32.000000 comwatt-client-0.1.1/setup.py
+drwxrwxr-x   0 mat       (1000) mat       (1000)        0 2023-07-08 14:20:00.526389 comwatt-client-0.1.1/src/
+-rw-rw-r--   0 mat       (1000) mat       (1000)        0 2023-07-08 13:37:30.000000 comwatt-client-0.1.1/src/__init__.py
+-rw-rw-r--   0 mat       (1000) mat       (1000)     6043 2023-07-08 14:02:41.000000 comwatt-client-0.1.1/src/client.py
```

### Comparing `comwatt-client-0.1.0/PKG-INFO` & `comwatt-client-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: comwatt-client
-Version: 0.1.0
+Version: 0.1.1
 Summary: Python Client for Comwatt API
 Home-page: UNKNOWN
 Author: Matéo Greil
 Author-email: contact@greil.fr
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `comwatt-client-0.1.0/README.md` & `comwatt-client-0.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `comwatt-client-0.1.0/comwatt_client.egg-info/PKG-INFO` & `comwatt-client-0.1.1/comwatt_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: comwatt-client
-Version: 0.1.0
+Version: 0.1.1
 Summary: Python Client for Comwatt API
 Home-page: UNKNOWN
 Author: Matéo Greil
 Author-email: contact@greil.fr
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `comwatt-client-0.1.0/setup.py` & `comwatt-client-0.1.1/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='comwatt-client',
-    version='0.1.0',
+    version='0.1.1',
     author='Matéo Greil',
     author_email='contact@greil.fr',
     description='Python Client for Comwatt API',
     packages=find_packages(),
     install_requires=[
         'requests',
     ],
```

### Comparing `comwatt-client-0.1.0/src/client.py` & `comwatt-client-0.1.1/src/client.py`

 * *Files identical despite different names*

