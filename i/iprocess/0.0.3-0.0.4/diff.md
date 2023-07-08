# Comparing `tmp/iprocess-0.0.3.tar.gz` & `tmp/iprocess-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iprocess-0.0.3.tar", last modified: Sat Jul  8 17:42:43 2023, max compression
+gzip compressed data, was "iprocess-0.0.4.tar", last modified: Sat Jul  8 18:06:44 2023, max compression
```

## Comparing `iprocess-0.0.3.tar` & `iprocess-0.0.4.tar`

### file list

```diff
@@ -1,15 +1,10 @@
-drwxrwxrwx   0        0        0        0 2023-07-08 17:42:43.798673 iprocess-0.0.3/
--rw-rw-rw-   0        0        0      534 2023-07-08 17:42:43.796674 iprocess-0.0.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-08 17:42:43.756697 iprocess-0.0.3/iprocess/
--rw-rw-rw-   0        0        0     1039 2023-07-08 17:21:37.000000 iprocess-0.0.3/iprocess/__init__.py
--rw-rw-rw-   0        0        0     8467 2023-07-08 17:21:37.000000 iprocess-0.0.3/iprocess/process.py
-drwxrwxrwx   0        0        0        0 2023-07-08 17:42:43.794675 iprocess-0.0.3/iprocess/pytransform/
--rw-rw-rw-   0        0        0    13587 2023-07-05 17:15:54.000000 iprocess-0.0.3/iprocess/pytransform/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-08 17:42:43.792677 iprocess-0.0.3/iprocess.egg-info/
--rw-rw-rw-   0        0        0      534 2023-07-08 17:42:43.000000 iprocess-0.0.3/iprocess.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      249 2023-07-08 17:42:43.000000 iprocess-0.0.3/iprocess.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-08 17:42:43.000000 iprocess-0.0.3/iprocess.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-07-08 17:42:43.000000 iprocess-0.0.3/iprocess.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-07-08 17:42:43.000000 iprocess-0.0.3/iprocess.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-08 17:42:43.799673 iprocess-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      796 2023-07-08 17:41:47.000000 iprocess-0.0.3/setup_ipocess.py
+drwxrwxrwx   0        0        0        0 2023-07-08 18:06:44.901117 iprocess-0.0.4/
+-rw-rw-rw-   0        0        0      534 2023-07-08 18:06:44.899117 iprocess-0.0.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-08 18:06:44.896119 iprocess-0.0.4/iprocess.egg-info/
+-rw-rw-rw-   0        0        0      534 2023-07-08 18:06:44.000000 iprocess-0.0.4/iprocess.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      175 2023-07-08 18:06:44.000000 iprocess-0.0.4/iprocess.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-08 18:06:44.000000 iprocess-0.0.4/iprocess.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-07-08 18:06:44.000000 iprocess-0.0.4/iprocess.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-07-08 18:06:44.000000 iprocess-0.0.4/iprocess.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-08 18:06:44.906124 iprocess-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      796 2023-07-08 18:06:32.000000 iprocess-0.0.4/setup_ipocess.py
```

### Comparing `iprocess-0.0.3/PKG-INFO` & `iprocess-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iprocess
-Version: 0.0.3
+Version: 0.0.4
 Summary: nope
 Home-page: UNKNOWN
 Author: anonymos
 Author-email: dontknow@gmail.com
 License: UNKNOWN
 Description: NOTHING SPECIAL
 Platform: UNKNOWN
```

### Comparing `iprocess-0.0.3/iprocess.egg-info/PKG-INFO` & `iprocess-0.0.4/iprocess.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iprocess
-Version: 0.0.3
+Version: 0.0.4
 Summary: nope
 Home-page: UNKNOWN
 Author: anonymos
 Author-email: dontknow@gmail.com
 License: UNKNOWN
 Description: NOTHING SPECIAL
 Platform: UNKNOWN
```

### Comparing `iprocess-0.0.3/setup_ipocess.py` & `iprocess-0.0.4/setup_ipocess.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
-VERSION = '0.0.3'
+VERSION = '0.0.4'
 DESCRIPTION = 'nope'
 LONG_DESCRIPTION = "NOTHING SPECIAL"
 # Setting up
 setup(
     name="iprocess",
     version=VERSION,
     author="anonymos",
```

