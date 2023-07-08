# Comparing `tmp/sigtonoise-1.0.0.tar.gz` & `tmp/sigtonoise-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sigtonoise-1.0.0.tar", last modified: Sat Jul  8 13:49:48 2023, max compression
+gzip compressed data, was "sigtonoise-1.0.1.tar", last modified: Sat Jul  8 14:01:01 2023, max compression
```

## Comparing `sigtonoise-1.0.0.tar` & `sigtonoise-1.0.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-07-08 13:49:48.025767 sigtonoise-1.0.0/
--rw-rw-rw-   0        0        0     1477 2023-07-08 13:23:55.000000 sigtonoise-1.0.0/LICENSE.txt
--rw-rw-rw-   0        0        0      577 2023-07-08 13:49:48.025767 sigtonoise-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-07-08 13:49:48.026765 sigtonoise-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      793 2023-07-08 13:49:28.000000 sigtonoise-1.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-08 13:49:48.002628 sigtonoise-1.0.0/sigtonoise/
--rw-rw-rw-   0        0        0        0 2023-07-08 13:45:43.000000 sigtonoise-1.0.0/sigtonoise/__init__.py
--rw-rw-rw-   0        0        0      504 2023-07-08 13:19:09.000000 sigtonoise-1.0.0/sigtonoise/a.py
-drwxrwxrwx   0        0        0        0 2023-07-08 13:49:48.023770 sigtonoise-1.0.0/sigtonoise.egg-info/
--rw-rw-rw-   0        0        0      577 2023-07-08 13:49:47.000000 sigtonoise-1.0.0/sigtonoise.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      228 2023-07-08 13:49:47.000000 sigtonoise-1.0.0/sigtonoise.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-08 13:49:47.000000 sigtonoise-1.0.0/sigtonoise.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2023-07-08 13:49:47.000000 sigtonoise-1.0.0/sigtonoise.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-07-08 13:49:47.000000 sigtonoise-1.0.0/sigtonoise.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-08 14:01:01.386054 sigtonoise-1.0.1/
+-rw-rw-rw-   0        0        0     1477 2023-07-08 13:23:55.000000 sigtonoise-1.0.1/LICENSE.txt
+-rw-rw-rw-   0        0        0      577 2023-07-08 14:01:01.385056 sigtonoise-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-07-08 14:01:01.386054 sigtonoise-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      793 2023-07-08 14:00:51.000000 sigtonoise-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-08 14:01:01.365110 sigtonoise-1.0.1/sigtonoise/
+-rw-rw-rw-   0        0        0      504 2023-07-08 14:00:53.000000 sigtonoise-1.0.1/sigtonoise/__init__.py
+-rw-rw-rw-   0        0        0      504 2023-07-08 13:19:09.000000 sigtonoise-1.0.1/sigtonoise/a.py
+drwxrwxrwx   0        0        0        0 2023-07-08 14:01:01.383062 sigtonoise-1.0.1/sigtonoise.egg-info/
+-rw-rw-rw-   0        0        0      577 2023-07-08 14:01:01.000000 sigtonoise-1.0.1/sigtonoise.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      228 2023-07-08 14:01:01.000000 sigtonoise-1.0.1/sigtonoise.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-08 14:01:01.000000 sigtonoise-1.0.1/sigtonoise.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2023-07-08 14:01:01.000000 sigtonoise-1.0.1/sigtonoise.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-07-08 14:01:01.000000 sigtonoise-1.0.1/sigtonoise.egg-info/top_level.txt
```

### Comparing `sigtonoise-1.0.0/LICENSE.txt` & `sigtonoise-1.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sigtonoise-1.0.0/PKG-INFO` & `sigtonoise-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sigtonoise
-Version: 1.0.0
+Version: 1.0.1
 Summary: A module for image processing
 Author: Armankhanvsit
 Author-email: armanpconly@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `sigtonoise-1.0.0/setup.py` & `sigtonoise-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='sigtonoise',
-    version='1.0.0',
+    version='1.0.1',
     author='Armankhanvsit',
     author_email='armanpconly@gmail.com',
     description='A module for image processing',
     long_description='A module for image processing using numpy, PIL, scipy, and matplotlib.',
     packages=['sigtonoise'],
     install_requires=[
         'numpy',
```

### Comparing `sigtonoise-1.0.0/sigtonoise.egg-info/PKG-INFO` & `sigtonoise-1.0.1/sigtonoise.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sigtonoise
-Version: 1.0.0
+Version: 1.0.1
 Summary: A module for image processing
 Author: Armankhanvsit
 Author-email: armanpconly@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

