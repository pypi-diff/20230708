# Comparing `tmp/seunggabi_core_python-0.4.0.tar.gz` & `tmp/seunggabi_core_python-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seunggabi_core_python-0.4.0.tar", last modified: Sat Jul  8 08:06:25 2023, max compression
+gzip compressed data, was "seunggabi_core_python-0.5.0.tar", last modified: Sat Jul  8 14:12:16 2023, max compression
```

## Comparing `seunggabi_core_python-0.4.0.tar` & `seunggabi_core_python-0.5.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 seunggabi   (501) staff       (20)        0 2023-07-08 08:06:25.268958 seunggabi_core_python-0.4.0/
--rw-r--r--   0 seunggabi   (501) staff       (20)     1070 2023-05-13 14:31:33.000000 seunggabi_core_python-0.4.0/LICENSE
--rw-r--r--   0 seunggabi   (501) staff       (20)      573 2023-07-08 08:06:25.268850 seunggabi_core_python-0.4.0/PKG-INFO
--rw-r--r--   0 seunggabi   (501) staff       (20)      366 2023-07-08 06:47:51.000000 seunggabi_core_python-0.4.0/README.md
--rw-r--r--   0 seunggabi   (501) staff       (20)       38 2023-07-08 08:06:25.268988 seunggabi_core_python-0.4.0/setup.cfg
--rw-r--r--   0 seunggabi   (501) staff       (20)      821 2023-07-08 08:02:23.000000 seunggabi_core_python-0.4.0/setup.py
-drwxr-xr-x   0 seunggabi   (501) staff       (20)        0 2023-07-08 08:06:25.266772 seunggabi_core_python-0.4.0/seunggabi_core_python/
--rw-r--r--   0 seunggabi   (501) staff       (20)       22 2023-07-08 08:06:20.000000 seunggabi_core_python-0.4.0/seunggabi_core_python/__init__.py
--rw-r--r--   0 seunggabi   (501) staff       (20)       48 2023-05-15 13:10:17.000000 seunggabi_core_python-0.4.0/seunggabi_core_python/const.py
-drwxr-xr-x   0 seunggabi   (501) staff       (20)        0 2023-07-08 08:06:25.267721 seunggabi_core_python-0.4.0/seunggabi_core_python/exception/
--rw-r--r--   0 seunggabi   (501) staff       (20)        0 2023-05-15 12:46:34.000000 seunggabi_core_python-0.4.0/seunggabi_core_python/exception/__init__.py
--rw-r--r--   0 seunggabi   (501) staff       (20)      143 2023-06-11 18:12:39.000000 seunggabi_core_python-0.4.0/seunggabi_core_python/exception/bad_request.py
--rw-r--r--   0 seunggabi   (501) staff       (20)      139 2023-06-11 18:12:39.000000 seunggabi_core_python-0.4.0/seunggabi_core_python/exception/not_found.py
-drwxr-xr-x   0 seunggabi   (501) staff       (20)        0 2023-07-08 08:06:25.268698 seunggabi_core_python-0.4.0/seunggabi_core_python/util/
--rw-r--r--   0 seunggabi   (501) staff       (20)        0 2023-05-13 15:22:13.000000 seunggabi_core_python-0.4.0/seunggabi_core_python/util/__init__.py
--rw-r--r--   0 seunggabi   (501) staff       (20)     1001 2023-05-18 14:08:20.000000 seunggabi_core_python-0.4.0/seunggabi_core_python/util/arg_util.py
--rw-r--r--   0 seunggabi   (501) staff       (20)      458 2023-07-08 06:46:01.000000 seunggabi_core_python-0.4.0/seunggabi_core_python/util/bs_util.py
--rw-r--r--   0 seunggabi   (501) staff       (20)      915 2023-06-11 18:11:25.000000 seunggabi_core_python-0.4.0/seunggabi_core_python/util/config_util.py
--rw-r--r--   0 seunggabi   (501) staff       (20)      157 2023-07-08 08:05:53.000000 seunggabi_core_python-0.4.0/seunggabi_core_python/util/dependency_util.py
--rw-r--r--   0 seunggabi   (501) staff       (20)      149 2023-05-15 15:07:03.000000 seunggabi_core_python-0.4.0/seunggabi_core_python/util/json_util.py
--rw-r--r--   0 seunggabi   (501) staff       (20)      219 2023-07-08 06:24:47.000000 seunggabi_core_python-0.4.0/seunggabi_core_python/util/obj_util.py
--rw-r--r--   0 seunggabi   (501) staff       (20)      271 2023-07-08 06:46:01.000000 seunggabi_core_python-0.4.0/seunggabi_core_python/util/request_util.py
-drwxr-xr-x   0 seunggabi   (501) staff       (20)        0 2023-07-08 08:06:25.267325 seunggabi_core_python-0.4.0/seunggabi_core_python.egg-info/
--rw-r--r--   0 seunggabi   (501) staff       (20)      573 2023-07-08 08:06:25.000000 seunggabi_core_python-0.4.0/seunggabi_core_python.egg-info/PKG-INFO
--rw-r--r--   0 seunggabi   (501) staff       (20)      777 2023-07-08 08:06:25.000000 seunggabi_core_python-0.4.0/seunggabi_core_python.egg-info/SOURCES.txt
--rw-r--r--   0 seunggabi   (501) staff       (20)        1 2023-07-08 08:06:25.000000 seunggabi_core_python-0.4.0/seunggabi_core_python.egg-info/dependency_links.txt
--rw-r--r--   0 seunggabi   (501) staff       (20)       36 2023-07-08 08:06:25.000000 seunggabi_core_python-0.4.0/seunggabi_core_python.egg-info/requires.txt
--rw-r--r--   0 seunggabi   (501) staff       (20)       22 2023-07-08 08:06:25.000000 seunggabi_core_python-0.4.0/seunggabi_core_python.egg-info/top_level.txt
+drwxr-xr-x   0 seunggabi   (501) staff       (20)        0 2023-07-08 14:12:16.088521 seunggabi_core_python-0.5.0/
+-rw-r--r--   0 seunggabi   (501) staff       (20)     1070 2023-05-13 14:31:33.000000 seunggabi_core_python-0.5.0/LICENSE
+-rw-r--r--   0 seunggabi   (501) staff       (20)      573 2023-07-08 14:12:16.088394 seunggabi_core_python-0.5.0/PKG-INFO
+-rw-r--r--   0 seunggabi   (501) staff       (20)      366 2023-07-08 06:47:51.000000 seunggabi_core_python-0.5.0/README.md
+-rw-r--r--   0 seunggabi   (501) staff       (20)       38 2023-07-08 14:12:16.088559 seunggabi_core_python-0.5.0/setup.cfg
+-rw-r--r--   0 seunggabi   (501) staff       (20)      821 2023-07-08 08:02:23.000000 seunggabi_core_python-0.5.0/setup.py
+drwxr-xr-x   0 seunggabi   (501) staff       (20)        0 2023-07-08 14:12:16.084975 seunggabi_core_python-0.5.0/seunggabi_core_python/
+-rw-r--r--   0 seunggabi   (501) staff       (20)       22 2023-07-08 14:12:12.000000 seunggabi_core_python-0.5.0/seunggabi_core_python/__init__.py
+-rw-r--r--   0 seunggabi   (501) staff       (20)       48 2023-05-15 13:10:17.000000 seunggabi_core_python-0.5.0/seunggabi_core_python/const.py
+drwxr-xr-x   0 seunggabi   (501) staff       (20)        0 2023-07-08 14:12:16.086294 seunggabi_core_python-0.5.0/seunggabi_core_python/exception/
+-rw-r--r--   0 seunggabi   (501) staff       (20)        0 2023-05-15 12:46:34.000000 seunggabi_core_python-0.5.0/seunggabi_core_python/exception/__init__.py
+-rw-r--r--   0 seunggabi   (501) staff       (20)      143 2023-06-11 18:12:39.000000 seunggabi_core_python-0.5.0/seunggabi_core_python/exception/bad_request.py
+-rw-r--r--   0 seunggabi   (501) staff       (20)      139 2023-06-11 18:12:39.000000 seunggabi_core_python-0.5.0/seunggabi_core_python/exception/not_found.py
+drwxr-xr-x   0 seunggabi   (501) staff       (20)        0 2023-07-08 14:12:16.088138 seunggabi_core_python-0.5.0/seunggabi_core_python/util/
+-rw-r--r--   0 seunggabi   (501) staff       (20)        0 2023-05-13 15:22:13.000000 seunggabi_core_python-0.5.0/seunggabi_core_python/util/__init__.py
+-rw-r--r--   0 seunggabi   (501) staff       (20)     1001 2023-05-18 14:08:20.000000 seunggabi_core_python-0.5.0/seunggabi_core_python/util/arg_util.py
+-rw-r--r--   0 seunggabi   (501) staff       (20)      458 2023-07-08 06:46:01.000000 seunggabi_core_python-0.5.0/seunggabi_core_python/util/bs_util.py
+-rw-r--r--   0 seunggabi   (501) staff       (20)      915 2023-06-11 18:11:25.000000 seunggabi_core_python-0.5.0/seunggabi_core_python/util/config_util.py
+-rw-r--r--   0 seunggabi   (501) staff       (20)      157 2023-07-08 08:05:53.000000 seunggabi_core_python-0.5.0/seunggabi_core_python/util/dependency_util.py
+-rw-r--r--   0 seunggabi   (501) staff       (20)      210 2023-07-08 14:10:08.000000 seunggabi_core_python-0.5.0/seunggabi_core_python/util/json_util.py
+-rw-r--r--   0 seunggabi   (501) staff       (20)      219 2023-07-08 06:24:47.000000 seunggabi_core_python-0.5.0/seunggabi_core_python/util/obj_util.py
+-rw-r--r--   0 seunggabi   (501) staff       (20)      271 2023-07-08 06:46:01.000000 seunggabi_core_python-0.5.0/seunggabi_core_python/util/request_util.py
+drwxr-xr-x   0 seunggabi   (501) staff       (20)        0 2023-07-08 14:12:16.085793 seunggabi_core_python-0.5.0/seunggabi_core_python.egg-info/
+-rw-r--r--   0 seunggabi   (501) staff       (20)      573 2023-07-08 14:12:16.000000 seunggabi_core_python-0.5.0/seunggabi_core_python.egg-info/PKG-INFO
+-rw-r--r--   0 seunggabi   (501) staff       (20)      777 2023-07-08 14:12:16.000000 seunggabi_core_python-0.5.0/seunggabi_core_python.egg-info/SOURCES.txt
+-rw-r--r--   0 seunggabi   (501) staff       (20)        1 2023-07-08 14:12:16.000000 seunggabi_core_python-0.5.0/seunggabi_core_python.egg-info/dependency_links.txt
+-rw-r--r--   0 seunggabi   (501) staff       (20)       36 2023-07-08 14:12:16.000000 seunggabi_core_python-0.5.0/seunggabi_core_python.egg-info/requires.txt
+-rw-r--r--   0 seunggabi   (501) staff       (20)       22 2023-07-08 14:12:16.000000 seunggabi_core_python-0.5.0/seunggabi_core_python.egg-info/top_level.txt
```

### Comparing `seunggabi_core_python-0.4.0/LICENSE` & `seunggabi_core_python-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `seunggabi_core_python-0.4.0/PKG-INFO` & `seunggabi_core_python-0.5.0/seunggabi_core_python.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: seunggabi_core_python
-Version: 0.4.0
+Name: seunggabi-core-python
+Version: 0.5.0
 Summary: A collection of core Python modules
 Home-page: https://github.com/seunggabi/core_python
 Author: seunggabi
 Author-email: seunggabi@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `seunggabi_core_python-0.4.0/setup.py` & `seunggabi_core_python-0.5.0/setup.py`

 * *Files identical despite different names*

### Comparing `seunggabi_core_python-0.4.0/seunggabi_core_python/util/arg_util.py` & `seunggabi_core_python-0.5.0/seunggabi_core_python/util/arg_util.py`

 * *Files identical despite different names*

### Comparing `seunggabi_core_python-0.4.0/seunggabi_core_python/util/config_util.py` & `seunggabi_core_python-0.5.0/seunggabi_core_python/util/config_util.py`

 * *Files identical despite different names*

### Comparing `seunggabi_core_python-0.4.0/seunggabi_core_python.egg-info/PKG-INFO` & `seunggabi_core_python-0.5.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: seunggabi-core-python
-Version: 0.4.0
+Name: seunggabi_core_python
+Version: 0.5.0
 Summary: A collection of core Python modules
 Home-page: https://github.com/seunggabi/core_python
 Author: seunggabi
 Author-email: seunggabi@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `seunggabi_core_python-0.4.0/seunggabi_core_python.egg-info/SOURCES.txt` & `seunggabi_core_python-0.5.0/seunggabi_core_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

