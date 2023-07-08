# Comparing `tmp/pygeocodio-1.3.0.tar.gz` & `tmp/pygeocodio-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygeocodio-1.3.0.tar", last modified: Wed May 31 14:31:35 2023, max compression
+gzip compressed data, was "pygeocodio-1.4.0.tar", last modified: Sat Jul  8 19:31:09 2023, max compression
```

## Comparing `pygeocodio-1.3.0.tar` & `pygeocodio-1.4.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:31:35.035903 pygeocodio-1.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)      830 2023-05-31 14:31:22.000000 pygeocodio-1.3.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3200 2023-05-31 14:31:22.000000 pygeocodio-1.3.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3273 2023-05-31 14:31:22.000000 pygeocodio-1.3.0/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-05-31 14:31:22.000000 pygeocodio-1.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-31 14:31:22.000000 pygeocodio-1.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     9699 2023-05-31 14:31:35.035903 pygeocodio-1.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5624 2023-05-31 14:31:22.000000 pygeocodio-1.3.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 14:31:35.035903 pygeocodio-1.3.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1629 2023-05-31 14:31:22.000000 pygeocodio-1.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:31:35.035903 pygeocodio-1.3.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:31:35.035903 pygeocodio-1.3.0/src/geocodio/
--rwxr-xr-x   0 runner    (1001) docker     (123)      443 2023-05-31 14:31:22.000000 pygeocodio-1.3.0/src/geocodio/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10734 2023-05-31 14:31:22.000000 pygeocodio-1.3.0/src/geocodio/client.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6771 2023-05-31 14:31:22.000000 pygeocodio-1.3.0/src/geocodio/data.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      438 2023-05-31 14:31:22.000000 pygeocodio-1.3.0/src/geocodio/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:31:35.035903 pygeocodio-1.3.0/src/pygeocodio.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9699 2023-05-31 14:31:34.000000 pygeocodio-1.3.0/src/pygeocodio.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-05-31 14:31:35.000000 pygeocodio-1.3.0/src/pygeocodio.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 14:31:34.000000 pygeocodio-1.3.0/src/pygeocodio.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 14:31:34.000000 pygeocodio-1.3.0/src/pygeocodio.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-31 14:31:34.000000 pygeocodio-1.3.0/src/pygeocodio.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-31 14:31:34.000000 pygeocodio-1.3.0/src/pygeocodio.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 19:31:09.710387 pygeocodio-1.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-07-08 19:31:01.000000 pygeocodio-1.4.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3200 2023-07-08 19:31:01.000000 pygeocodio-1.4.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3344 2023-07-08 19:31:01.000000 pygeocodio-1.4.0/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-07-08 19:31:01.000000 pygeocodio-1.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-08 19:31:01.000000 pygeocodio-1.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9720 2023-07-08 19:31:09.710387 pygeocodio-1.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5624 2023-07-08 19:31:01.000000 pygeocodio-1.4.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 19:31:09.710387 pygeocodio-1.4.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1580 2023-07-08 19:31:01.000000 pygeocodio-1.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 19:31:09.710387 pygeocodio-1.4.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 19:31:09.710387 pygeocodio-1.4.0/src/geocodio/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      443 2023-07-08 19:31:01.000000 pygeocodio-1.4.0/src/geocodio/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10734 2023-07-08 19:31:01.000000 pygeocodio-1.4.0/src/geocodio/client.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6771 2023-07-08 19:31:01.000000 pygeocodio-1.4.0/src/geocodio/data.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      438 2023-07-08 19:31:01.000000 pygeocodio-1.4.0/src/geocodio/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 19:31:09.710387 pygeocodio-1.4.0/src/pygeocodio.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9720 2023-07-08 19:31:09.000000 pygeocodio-1.4.0/src/pygeocodio.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-07-08 19:31:09.000000 pygeocodio-1.4.0/src/pygeocodio.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 19:31:09.000000 pygeocodio-1.4.0/src/pygeocodio.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 19:31:09.000000 pygeocodio-1.4.0/src/pygeocodio.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-08 19:31:09.000000 pygeocodio-1.4.0/src/pygeocodio.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-08 19:31:09.000000 pygeocodio-1.4.0/src/pygeocodio.egg-info/top_level.txt
```

### Comparing `pygeocodio-1.3.0/AUTHORS.rst` & `pygeocodio-1.4.0/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `pygeocodio-1.3.0/CONTRIBUTING.rst` & `pygeocodio-1.4.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `pygeocodio-1.3.0/HISTORY.rst` & `pygeocodio-1.4.0/HISTORY.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,17 @@
 .. :changelog:
 
 History
 -------
 
+1.4.0 (2023-07-08)
++++++++++++++++++++
+
+* Drop support for Python 3.7
+
 1.3.0 (2023-05-31)
 +++++++++++++++++++
 
 * Adds support for the 'limit' parameter to limit results (thanks bruno-uy!)
 
 1.2.0 (2023-03-21)
 +++++++++++++++++++
```

### Comparing `pygeocodio-1.3.0/LICENSE` & `pygeocodio-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pygeocodio-1.3.0/PKG-INFO` & `pygeocodio-1.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 Metadata-Version: 2.1
 Name: pygeocodio
-Version: 1.3.0
+Version: 1.4.0
 Summary: Python wrapper for Geocod.io API
 Home-page: https://github.com/bennylope/pygeocodio
 Author: Ben Lopatin
 Author-email: ben@benlopatin.com
 License: BSD
 Keywords: geocodio
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet :: WWW/HTTP
 License-File: LICENSE
 License-File: AUTHORS.rst
@@ -235,14 +234,19 @@
 
 
 
 
 History
 -------
 
+1.4.0 (2023-07-08)
++++++++++++++++++++
+
+* Drop support for Python 3.7
+
 1.3.0 (2023-05-31)
 +++++++++++++++++++
 
 * Adds support for the 'limit' parameter to limit results (thanks bruno-uy!)
 
 1.2.0 (2023-03-21)
 +++++++++++++++++++
```

### Comparing `pygeocodio-1.3.0/README.rst` & `pygeocodio-1.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `pygeocodio-1.3.0/setup.py` & `pygeocodio-1.4.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -38,15 +38,14 @@
     keywords="geocodio",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: BSD License",
         "Natural Language :: English",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Topic :: Internet :: WWW/HTTP",
     ],
     test_suite="tests",
```

### Comparing `pygeocodio-1.3.0/src/geocodio/client.py` & `pygeocodio-1.4.0/src/geocodio/client.py`

 * *Files identical despite different names*

### Comparing `pygeocodio-1.3.0/src/geocodio/data.py` & `pygeocodio-1.4.0/src/geocodio/data.py`

 * *Files identical despite different names*

### Comparing `pygeocodio-1.3.0/src/pygeocodio.egg-info/PKG-INFO` & `pygeocodio-1.4.0/src/pygeocodio.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 Metadata-Version: 2.1
 Name: pygeocodio
-Version: 1.3.0
+Version: 1.4.0
 Summary: Python wrapper for Geocod.io API
 Home-page: https://github.com/bennylope/pygeocodio
 Author: Ben Lopatin
 Author-email: ben@benlopatin.com
 License: BSD
 Keywords: geocodio
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet :: WWW/HTTP
 License-File: LICENSE
 License-File: AUTHORS.rst
@@ -235,14 +234,19 @@
 
 
 
 
 History
 -------
 
+1.4.0 (2023-07-08)
++++++++++++++++++++
+
+* Drop support for Python 3.7
+
 1.3.0 (2023-05-31)
 +++++++++++++++++++
 
 * Adds support for the 'limit' parameter to limit results (thanks bruno-uy!)
 
 1.2.0 (2023-03-21)
 +++++++++++++++++++
```

