# Comparing `tmp/iprocess-0.0.1.tar.gz` & `tmp/iprocess-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iprocess-0.0.1.tar", last modified: Sat Jul  8 17:00:20 2023, max compression
+gzip compressed data, was "iprocess-0.0.2.tar", last modified: Sat Jul  8 17:32:51 2023, max compression
```

## Comparing `iprocess-0.0.1.tar` & `iprocess-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-07-08 17:00:20.110369 iprocess-0.0.1/
--rw-rw-rw-   0        0        0      534 2023-07-08 17:00:20.108371 iprocess-0.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-08 17:00:20.023419 iprocess-0.0.1/iprocess/
--rw-rw-rw-   0        0        0        0 2023-07-08 16:59:20.000000 iprocess-0.0.1/iprocess/__init__.py
--rw-rw-rw-   0        0        0     1303 2023-07-08 16:55:36.000000 iprocess-0.0.1/iprocess/process.py
-drwxrwxrwx   0        0        0        0 2023-07-08 17:00:20.105376 iprocess-0.0.1/iprocess.egg-info/
--rw-rw-rw-   0        0        0      534 2023-07-08 17:00:19.000000 iprocess-0.0.1/iprocess.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      216 2023-07-08 17:00:19.000000 iprocess-0.0.1/iprocess.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-08 17:00:19.000000 iprocess-0.0.1/iprocess.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-07-08 17:00:19.000000 iprocess-0.0.1/iprocess.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-07-08 17:00:19.000000 iprocess-0.0.1/iprocess.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-08 17:00:20.111369 iprocess-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      796 2023-07-08 16:58:54.000000 iprocess-0.0.1/setup_ipocess.py
+drwxrwxrwx   0        0        0        0 2023-07-08 17:32:51.787696 iprocess-0.0.2/
+-rw-rw-rw-   0        0        0      534 2023-07-08 17:32:51.786695 iprocess-0.0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-08 17:32:51.779700 iprocess-0.0.2/iprocess.egg-info/
+-rw-rw-rw-   0        0        0      534 2023-07-08 17:32:51.000000 iprocess-0.0.2/iprocess.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      199 2023-07-08 17:32:51.000000 iprocess-0.0.2/iprocess.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-08 17:32:51.000000 iprocess-0.0.2/iprocess.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-07-08 17:32:51.000000 iprocess-0.0.2/iprocess.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-07-08 17:32:51.000000 iprocess-0.0.2/iprocess.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-08 17:32:51.783699 iprocess-0.0.2/pytransform/
+-rw-rw-rw-   0        0        0    13587 2023-07-05 17:15:54.000000 iprocess-0.0.2/pytransform/__init__.py
+-rw-rw-rw-   0        0        0       42 2023-07-08 17:32:51.788697 iprocess-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      796 2023-07-08 17:32:00.000000 iprocess-0.0.2/setup_ipocess.py
```

### Comparing `iprocess-0.0.1/PKG-INFO` & `iprocess-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iprocess
-Version: 0.0.1
+Version: 0.0.2
 Summary: nope
 Home-page: UNKNOWN
 Author: anonymos
 Author-email: dontknow@gmail.com
 License: UNKNOWN
 Description: NOTHING SPECIAL
 Platform: UNKNOWN
```

### Comparing `iprocess-0.0.1/iprocess.egg-info/PKG-INFO` & `iprocess-0.0.2/iprocess.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iprocess
-Version: 0.0.1
+Version: 0.0.2
 Summary: nope
 Home-page: UNKNOWN
 Author: anonymos
 Author-email: dontknow@gmail.com
 License: UNKNOWN
 Description: NOTHING SPECIAL
 Platform: UNKNOWN
```

### Comparing `iprocess-0.0.1/setup_ipocess.py` & `iprocess-0.0.2/setup_ipocess.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
-VERSION = '0.0.1'
+VERSION = '0.0.2'
 DESCRIPTION = 'nope'
 LONG_DESCRIPTION = "NOTHING SPECIAL"
 # Setting up
 setup(
     name="iprocess",
     version=VERSION,
     author="anonymos",
```

