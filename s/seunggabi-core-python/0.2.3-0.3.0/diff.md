# Comparing `tmp/seunggabi_core_python-0.2.3.tar.gz` & `tmp/seunggabi_core_python-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seunggabi_core_python-0.2.3.tar", last modified: Sun Jun 11 18:13:45 2023, max compression
+gzip compressed data, was "seunggabi_core_python-0.3.0.tar", last modified: Sat Jul  8 06:47:56 2023, max compression
```

## Comparing `seunggabi_core_python-0.2.3.tar` & `seunggabi_core_python-0.3.0.tar`

### file list

```diff
@@ -1,24 +1,26 @@
-drwxr-xr-x   0 seunggabi   (501) staff       (20)        0 2023-06-11 18:13:45.828478 seunggabi_core_python-0.2.3/
--rw-r--r--   0 seunggabi   (501) staff       (20)     1070 2023-05-13 14:31:33.000000 seunggabi_core_python-0.2.3/LICENSE
--rw-r--r--   0 seunggabi   (501) staff       (20)      573 2023-06-11 18:13:45.828366 seunggabi_core_python-0.2.3/PKG-INFO
--rw-r--r--   0 seunggabi   (501) staff       (20)      362 2023-06-11 16:46:36.000000 seunggabi_core_python-0.2.3/README.md
--rw-r--r--   0 seunggabi   (501) staff       (20)       38 2023-06-11 18:13:45.828513 seunggabi_core_python-0.2.3/setup.cfg
--rw-r--r--   0 seunggabi   (501) staff       (20)      746 2023-05-15 13:20:26.000000 seunggabi_core_python-0.2.3/setup.py
-drwxr-xr-x   0 seunggabi   (501) staff       (20)        0 2023-06-11 18:13:45.826617 seunggabi_core_python-0.2.3/seunggabi_core_python/
--rw-r--r--   0 seunggabi   (501) staff       (20)       22 2023-06-11 18:13:42.000000 seunggabi_core_python-0.2.3/seunggabi_core_python/__init__.py
--rw-r--r--   0 seunggabi   (501) staff       (20)       48 2023-05-15 13:10:17.000000 seunggabi_core_python-0.2.3/seunggabi_core_python/const.py
-drwxr-xr-x   0 seunggabi   (501) staff       (20)        0 2023-06-11 18:13:45.827587 seunggabi_core_python-0.2.3/seunggabi_core_python/exception/
--rw-r--r--   0 seunggabi   (501) staff       (20)        0 2023-05-15 12:46:34.000000 seunggabi_core_python-0.2.3/seunggabi_core_python/exception/__init__.py
--rw-r--r--   0 seunggabi   (501) staff       (20)      143 2023-06-11 18:12:39.000000 seunggabi_core_python-0.2.3/seunggabi_core_python/exception/bad_request.py
--rw-r--r--   0 seunggabi   (501) staff       (20)      139 2023-06-11 18:12:39.000000 seunggabi_core_python-0.2.3/seunggabi_core_python/exception/not_found.py
-drwxr-xr-x   0 seunggabi   (501) staff       (20)        0 2023-06-11 18:13:45.828182 seunggabi_core_python-0.2.3/seunggabi_core_python/util/
--rw-r--r--   0 seunggabi   (501) staff       (20)        0 2023-05-13 15:22:13.000000 seunggabi_core_python-0.2.3/seunggabi_core_python/util/__init__.py
--rw-r--r--   0 seunggabi   (501) staff       (20)     1001 2023-05-18 14:08:20.000000 seunggabi_core_python-0.2.3/seunggabi_core_python/util/arg_util.py
--rw-r--r--   0 seunggabi   (501) staff       (20)      915 2023-06-11 18:11:25.000000 seunggabi_core_python-0.2.3/seunggabi_core_python/util/config_util.py
--rw-r--r--   0 seunggabi   (501) staff       (20)      149 2023-05-15 15:07:03.000000 seunggabi_core_python-0.2.3/seunggabi_core_python/util/json_util.py
--rw-r--r--   0 seunggabi   (501) staff       (20)      193 2023-05-18 14:08:20.000000 seunggabi_core_python-0.2.3/seunggabi_core_python/util/request_util.py
-drwxr-xr-x   0 seunggabi   (501) staff       (20)        0 2023-06-11 18:13:45.827195 seunggabi_core_python-0.2.3/seunggabi_core_python.egg-info/
--rw-r--r--   0 seunggabi   (501) staff       (20)      573 2023-06-11 18:13:45.000000 seunggabi_core_python-0.2.3/seunggabi_core_python.egg-info/PKG-INFO
--rw-r--r--   0 seunggabi   (501) staff       (20)      610 2023-06-11 18:13:45.000000 seunggabi_core_python-0.2.3/seunggabi_core_python.egg-info/SOURCES.txt
--rw-r--r--   0 seunggabi   (501) staff       (20)        1 2023-06-11 18:13:45.000000 seunggabi_core_python-0.2.3/seunggabi_core_python.egg-info/dependency_links.txt
--rw-r--r--   0 seunggabi   (501) staff       (20)       22 2023-06-11 18:13:45.000000 seunggabi_core_python-0.2.3/seunggabi_core_python.egg-info/top_level.txt
+drwxr-xr-x   0 seunggabi   (501) staff       (20)        0 2023-07-08 06:47:56.302150 seunggabi_core_python-0.3.0/
+-rw-r--r--   0 seunggabi   (501) staff       (20)     1070 2023-05-13 14:31:33.000000 seunggabi_core_python-0.3.0/LICENSE
+-rw-r--r--   0 seunggabi   (501) staff       (20)      573 2023-07-08 06:47:56.302041 seunggabi_core_python-0.3.0/PKG-INFO
+-rw-r--r--   0 seunggabi   (501) staff       (20)      366 2023-07-08 06:47:51.000000 seunggabi_core_python-0.3.0/README.md
+-rw-r--r--   0 seunggabi   (501) staff       (20)       38 2023-07-08 06:47:56.302179 seunggabi_core_python-0.3.0/setup.cfg
+-rw-r--r--   0 seunggabi   (501) staff       (20)      746 2023-05-15 13:20:26.000000 seunggabi_core_python-0.3.0/setup.py
+drwxr-xr-x   0 seunggabi   (501) staff       (20)        0 2023-07-08 06:47:56.299518 seunggabi_core_python-0.3.0/seunggabi_core_python/
+-rw-r--r--   0 seunggabi   (501) staff       (20)       22 2023-07-08 06:47:51.000000 seunggabi_core_python-0.3.0/seunggabi_core_python/__init__.py
+-rw-r--r--   0 seunggabi   (501) staff       (20)       48 2023-05-15 13:10:17.000000 seunggabi_core_python-0.3.0/seunggabi_core_python/const.py
+drwxr-xr-x   0 seunggabi   (501) staff       (20)        0 2023-07-08 06:47:56.300598 seunggabi_core_python-0.3.0/seunggabi_core_python/exception/
+-rw-r--r--   0 seunggabi   (501) staff       (20)        0 2023-05-15 12:46:34.000000 seunggabi_core_python-0.3.0/seunggabi_core_python/exception/__init__.py
+-rw-r--r--   0 seunggabi   (501) staff       (20)      143 2023-06-11 18:12:39.000000 seunggabi_core_python-0.3.0/seunggabi_core_python/exception/bad_request.py
+-rw-r--r--   0 seunggabi   (501) staff       (20)      139 2023-06-11 18:12:39.000000 seunggabi_core_python-0.3.0/seunggabi_core_python/exception/not_found.py
+drwxr-xr-x   0 seunggabi   (501) staff       (20)        0 2023-07-08 06:47:56.301895 seunggabi_core_python-0.3.0/seunggabi_core_python/util/
+-rw-r--r--   0 seunggabi   (501) staff       (20)        0 2023-05-13 15:22:13.000000 seunggabi_core_python-0.3.0/seunggabi_core_python/util/__init__.py
+-rw-r--r--   0 seunggabi   (501) staff       (20)     1001 2023-05-18 14:08:20.000000 seunggabi_core_python-0.3.0/seunggabi_core_python/util/arg_util.py
+-rw-r--r--   0 seunggabi   (501) staff       (20)      458 2023-07-08 06:46:01.000000 seunggabi_core_python-0.3.0/seunggabi_core_python/util/bs_util.py
+-rw-r--r--   0 seunggabi   (501) staff       (20)      915 2023-06-11 18:11:25.000000 seunggabi_core_python-0.3.0/seunggabi_core_python/util/config_util.py
+-rw-r--r--   0 seunggabi   (501) staff       (20)      149 2023-05-15 15:07:03.000000 seunggabi_core_python-0.3.0/seunggabi_core_python/util/json_util.py
+-rw-r--r--   0 seunggabi   (501) staff       (20)      219 2023-07-08 06:24:47.000000 seunggabi_core_python-0.3.0/seunggabi_core_python/util/obj_util.py
+-rw-r--r--   0 seunggabi   (501) staff       (20)      271 2023-07-08 06:46:01.000000 seunggabi_core_python-0.3.0/seunggabi_core_python/util/request_util.py
+drwxr-xr-x   0 seunggabi   (501) staff       (20)        0 2023-07-08 06:47:56.300099 seunggabi_core_python-0.3.0/seunggabi_core_python.egg-info/
+-rw-r--r--   0 seunggabi   (501) staff       (20)      573 2023-07-08 06:47:56.000000 seunggabi_core_python-0.3.0/seunggabi_core_python.egg-info/PKG-INFO
+-rw-r--r--   0 seunggabi   (501) staff       (20)      687 2023-07-08 06:47:56.000000 seunggabi_core_python-0.3.0/seunggabi_core_python.egg-info/SOURCES.txt
+-rw-r--r--   0 seunggabi   (501) staff       (20)        1 2023-07-08 06:47:56.000000 seunggabi_core_python-0.3.0/seunggabi_core_python.egg-info/dependency_links.txt
+-rw-r--r--   0 seunggabi   (501) staff       (20)       22 2023-07-08 06:47:56.000000 seunggabi_core_python-0.3.0/seunggabi_core_python.egg-info/top_level.txt
```

### Comparing `seunggabi_core_python-0.2.3/LICENSE` & `seunggabi_core_python-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `seunggabi_core_python-0.2.3/PKG-INFO` & `seunggabi_core_python-0.3.0/seunggabi_core_python.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: seunggabi_core_python
-Version: 0.2.3
+Name: seunggabi-core-python
+Version: 0.3.0
 Summary: A collection of core Python modules
 Home-page: https://github.com/seunggabi/core_python
 Author: seunggabi
 Author-email: seunggabi@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `seunggabi_core_python-0.2.3/setup.py` & `seunggabi_core_python-0.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `seunggabi_core_python-0.2.3/seunggabi_core_python/util/arg_util.py` & `seunggabi_core_python-0.3.0/seunggabi_core_python/util/arg_util.py`

 * *Files identical despite different names*

### Comparing `seunggabi_core_python-0.2.3/seunggabi_core_python/util/config_util.py` & `seunggabi_core_python-0.3.0/seunggabi_core_python/util/config_util.py`

 * *Files identical despite different names*

### Comparing `seunggabi_core_python-0.2.3/seunggabi_core_python.egg-info/PKG-INFO` & `seunggabi_core_python-0.3.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: seunggabi-core-python
-Version: 0.2.3
+Name: seunggabi_core_python
+Version: 0.3.0
 Summary: A collection of core Python modules
 Home-page: https://github.com/seunggabi/core_python
 Author: seunggabi
 Author-email: seunggabi@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `seunggabi_core_python-0.2.3/seunggabi_core_python.egg-info/SOURCES.txt` & `seunggabi_core_python-0.3.0/seunggabi_core_python.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -8,10 +8,12 @@
 seunggabi_core_python.egg-info/dependency_links.txt
 seunggabi_core_python.egg-info/top_level.txt
 seunggabi_core_python/exception/__init__.py
 seunggabi_core_python/exception/bad_request.py
 seunggabi_core_python/exception/not_found.py
 seunggabi_core_python/util/__init__.py
 seunggabi_core_python/util/arg_util.py
+seunggabi_core_python/util/bs_util.py
 seunggabi_core_python/util/config_util.py
 seunggabi_core_python/util/json_util.py
+seunggabi_core_python/util/obj_util.py
 seunggabi_core_python/util/request_util.py
```

