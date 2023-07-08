# Comparing `tmp/trendalation-0.0.1.tar.gz` & `tmp/trendalation-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trendalation-0.0.1.tar", last modified: Fri Jul  7 00:48:56 2023, max compression
+gzip compressed data, was "trendalation-0.0.2.tar", last modified: Sat Jul  8 16:37:02 2023, max compression
```

## Comparing `trendalation-0.0.1.tar` & `trendalation-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 raghavsaboo   (501) staff       (20)        0 2023-07-07 00:48:56.698835 trendalation-0.0.1/
--rw-r--r--   0 raghavsaboo   (501) staff       (20)     1084 2023-07-07 00:41:12.000000 trendalation-0.0.1/LICENSE.rst
--rw-r--r--   0 raghavsaboo   (501) staff       (20)        0 2023-07-02 18:27:10.000000 trendalation-0.0.1/MANIFEST.in
--rw-r--r--   0 raghavsaboo   (501) staff       (20)      542 2023-07-07 00:48:56.698898 trendalation-0.0.1/PKG-INFO
--rw-r--r--   0 raghavsaboo   (501) staff       (20)      685 2023-07-07 00:38:17.000000 trendalation-0.0.1/README.md
--rw-r--r--   0 raghavsaboo   (501) staff       (20)        0 2023-07-02 18:27:10.000000 trendalation-0.0.1/pyproject.toml
--rw-r--r--   0 raghavsaboo   (501) staff       (20)      107 2023-07-07 00:48:56.699201 trendalation-0.0.1/setup.cfg
--rw-r--r--   0 raghavsaboo   (501) staff       (20)      707 2023-07-07 00:48:01.000000 trendalation-0.0.1/setup.py
-drwxr-xr-x   0 raghavsaboo   (501) staff       (20)        0 2023-07-07 00:48:56.697010 trendalation-0.0.1/src/
-drwxr-xr-x   0 raghavsaboo   (501) staff       (20)        0 2023-07-07 00:48:56.698680 trendalation-0.0.1/src/trendalation.egg-info/
--rw-r--r--   0 raghavsaboo   (501) staff       (20)      542 2023-07-07 00:48:56.000000 trendalation-0.0.1/src/trendalation.egg-info/PKG-INFO
--rw-r--r--   0 raghavsaboo   (501) staff       (20)      266 2023-07-07 00:48:56.000000 trendalation-0.0.1/src/trendalation.egg-info/SOURCES.txt
--rw-r--r--   0 raghavsaboo   (501) staff       (20)        1 2023-07-07 00:48:56.000000 trendalation-0.0.1/src/trendalation.egg-info/dependency_links.txt
--rw-r--r--   0 raghavsaboo   (501) staff       (20)       25 2023-07-07 00:48:56.000000 trendalation-0.0.1/src/trendalation.egg-info/requires.txt
--rw-r--r--   0 raghavsaboo   (501) staff       (20)        1 2023-07-07 00:48:56.000000 trendalation-0.0.1/src/trendalation.egg-info/top_level.txt
+drwxr-xr-x   0 raghavsaboo   (501) staff       (20)        0 2023-07-08 16:37:02.451065 trendalation-0.0.2/
+-rw-r--r--   0 raghavsaboo   (501) staff       (20)     1084 2023-07-07 00:41:12.000000 trendalation-0.0.2/LICENSE.rst
+-rw-r--r--   0 raghavsaboo   (501) staff       (20)        0 2023-07-02 18:27:10.000000 trendalation-0.0.2/MANIFEST.in
+-rw-r--r--   0 raghavsaboo   (501) staff       (20)      542 2023-07-08 16:37:02.451136 trendalation-0.0.2/PKG-INFO
+-rw-r--r--   0 raghavsaboo   (501) staff       (20)      872 2023-07-08 16:25:51.000000 trendalation-0.0.2/README.md
+-rw-r--r--   0 raghavsaboo   (501) staff       (20)        0 2023-07-02 18:27:10.000000 trendalation-0.0.2/pyproject.toml
+-rw-r--r--   0 raghavsaboo   (501) staff       (20)      107 2023-07-08 16:37:02.451414 trendalation-0.0.2/setup.cfg
+-rw-r--r--   0 raghavsaboo   (501) staff       (20)      707 2023-07-08 16:36:43.000000 trendalation-0.0.2/setup.py
+drwxr-xr-x   0 raghavsaboo   (501) staff       (20)        0 2023-07-08 16:37:02.449103 trendalation-0.0.2/src/
+drwxr-xr-x   0 raghavsaboo   (501) staff       (20)        0 2023-07-08 16:37:02.450921 trendalation-0.0.2/src/trendalation.egg-info/
+-rw-r--r--   0 raghavsaboo   (501) staff       (20)      542 2023-07-08 16:37:02.000000 trendalation-0.0.2/src/trendalation.egg-info/PKG-INFO
+-rw-r--r--   0 raghavsaboo   (501) staff       (20)      266 2023-07-08 16:37:02.000000 trendalation-0.0.2/src/trendalation.egg-info/SOURCES.txt
+-rw-r--r--   0 raghavsaboo   (501) staff       (20)        1 2023-07-08 16:37:02.000000 trendalation-0.0.2/src/trendalation.egg-info/dependency_links.txt
+-rw-r--r--   0 raghavsaboo   (501) staff       (20)       25 2023-07-08 16:37:02.000000 trendalation-0.0.2/src/trendalation.egg-info/requires.txt
+-rw-r--r--   0 raghavsaboo   (501) staff       (20)        1 2023-07-08 16:37:02.000000 trendalation-0.0.2/src/trendalation.egg-info/top_level.txt
```

### Comparing `trendalation-0.0.1/LICENSE.rst` & `trendalation-0.0.2/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `trendalation-0.0.1/PKG-INFO` & `trendalation-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trendalation
-Version: 0.0.1
+Version: 0.0.2
 Summary: UNKNOWN
 Home-page: https://github.com/kartikeysinha/trendalation
 Author: Raghav Saboo, Kartikey Sinha
 Author-email: raghs2000@gmail.com
 License: MIT
 Keywords: anomaly detection
 Platform: UNKNOWN
```

### Comparing `trendalation-0.0.1/README.md` & `trendalation-0.0.2/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -16,17 +16,18 @@
 SciPy (>= 1.11.1)
 
 ### Using pip
 
 The easiest way to install trendalation is using pip:
 `pip install trendalation`
 
-### Build from source
-
 ## Documentation
 
 ## Help and Support
 
-## Citation
+In order to report bugfixes and new feature requests, simply create a new issue on the repository.
+The issues will be reviewed by the authors on a regular basis & you're welcome to work on any open issues.
+
+## Contribution
 
-If you use scikit-learn in a scientific publication, we would appreciate citations:
-```insert link for citation instructions```
+This project is a community effort, and everyone is welcome to contribute.
+Feel free to work on any open issues and setup PRs.
```

### Comparing `trendalation-0.0.1/setup.py` & `trendalation-0.0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='trendalation',
-    version='0.0.1',
+    version='0.0.2',
     license='MIT',
     author="Raghav Saboo, Kartikey Sinha",
     author_email='raghs2000@gmail.com',
     packages=find_packages('src'),
     package_dir={'': 'src'},
     url='https://github.com/kartikeysinha/trendalation',
     keywords='anomaly detection',
```

### Comparing `trendalation-0.0.1/src/trendalation.egg-info/PKG-INFO` & `trendalation-0.0.2/src/trendalation.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trendalation
-Version: 0.0.1
+Version: 0.0.2
 Summary: UNKNOWN
 Home-page: https://github.com/kartikeysinha/trendalation
 Author: Raghav Saboo, Kartikey Sinha
 Author-email: raghs2000@gmail.com
 License: MIT
 Keywords: anomaly detection
 Platform: UNKNOWN
```

