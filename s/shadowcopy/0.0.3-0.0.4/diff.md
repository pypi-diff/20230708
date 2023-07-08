# Comparing `tmp/shadowcopy-0.0.3.tar.gz` & `tmp/shadowcopy-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shadowcopy-0.0.3.tar", last modified: Fri Jul  7 23:58:17 2023, max compression
+gzip compressed data, was "shadowcopy-0.0.4.tar", last modified: Sat Jul  8 00:01:26 2023, max compression
```

## Comparing `shadowcopy-0.0.3.tar` & `shadowcopy-0.0.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 23:58:17.024477 shadowcopy-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-07 23:58:02.000000 shadowcopy-0.0.3/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-07-07 23:58:17.024477 shadowcopy-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-07-07 23:58:02.000000 shadowcopy-0.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      987 2023-07-07 23:58:02.000000 shadowcopy-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 23:58:17.024477 shadowcopy-0.0.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 23:58:17.020476 shadowcopy-0.0.3/shadowcopy/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-07 23:58:02.000000 shadowcopy-0.0.3/shadowcopy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-07-07 23:58:02.000000 shadowcopy-0.0.3/shadowcopy/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-07-07 23:58:02.000000 shadowcopy-0.0.3/shadowcopy/shadow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 23:58:17.024477 shadowcopy-0.0.3/shadowcopy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-07-07 23:58:17.000000 shadowcopy-0.0.3/shadowcopy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-07 23:58:17.000000 shadowcopy-0.0.3/shadowcopy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 23:58:17.000000 shadowcopy-0.0.3/shadowcopy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-07 23:58:17.000000 shadowcopy-0.0.3/shadowcopy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-07 23:58:17.000000 shadowcopy-0.0.3/shadowcopy.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 23:58:17.024477 shadowcopy-0.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-07-07 23:58:02.000000 shadowcopy-0.0.3/tests/test_shadowcopy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:01:26.342649 shadowcopy-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-08 00:01:12.000000 shadowcopy-0.0.4/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-07-08 00:01:26.342649 shadowcopy-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-07-08 00:01:12.000000 shadowcopy-0.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      987 2023-07-08 00:01:12.000000 shadowcopy-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 00:01:26.342649 shadowcopy-0.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:01:26.338649 shadowcopy-0.0.4/shadowcopy/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-08 00:01:12.000000 shadowcopy-0.0.4/shadowcopy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-07-08 00:01:12.000000 shadowcopy-0.0.4/shadowcopy/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-07-08 00:01:12.000000 shadowcopy-0.0.4/shadowcopy/shadow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:01:26.338649 shadowcopy-0.0.4/shadowcopy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-07-08 00:01:26.000000 shadowcopy-0.0.4/shadowcopy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-08 00:01:26.000000 shadowcopy-0.0.4/shadowcopy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 00:01:26.000000 shadowcopy-0.0.4/shadowcopy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-08 00:01:26.000000 shadowcopy-0.0.4/shadowcopy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-08 00:01:26.000000 shadowcopy-0.0.4/shadowcopy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:01:26.342649 shadowcopy-0.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-07-08 00:01:12.000000 shadowcopy-0.0.4/tests/test_shadowcopy.py
```

### Comparing `shadowcopy-0.0.3/LICENSE.md` & `shadowcopy-0.0.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `shadowcopy-0.0.3/PKG-INFO` & `shadowcopy-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shadowcopy
-Version: 0.0.3
+Version: 0.0.4
 Summary: A project for shadowcopy
 Author-email: csm10495 <csm10495@gmail.com>
 License: MIT License
 Project-URL: homepage, https://github.com/csm10495/shadowcopy
 Project-URL: repository, https://github.com/csm10495/shadowcopy
 Project-URL: documentation, https://csm10495.github.io/shadowcopy
 Classifier: Intended Audience :: Developers
```

### Comparing `shadowcopy-0.0.3/README.md` & `shadowcopy-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `shadowcopy-0.0.3/pyproject.toml` & `shadowcopy-0.0.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `shadowcopy-0.0.3/shadowcopy/exceptions.py` & `shadowcopy-0.0.4/shadowcopy/exceptions.py`

 * *Files identical despite different names*

### Comparing `shadowcopy-0.0.3/shadowcopy/shadow.py` & `shadowcopy-0.0.4/shadowcopy/shadow.py`

 * *Files identical despite different names*

### Comparing `shadowcopy-0.0.3/shadowcopy.egg-info/PKG-INFO` & `shadowcopy-0.0.4/shadowcopy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shadowcopy
-Version: 0.0.3
+Version: 0.0.4
 Summary: A project for shadowcopy
 Author-email: csm10495 <csm10495@gmail.com>
 License: MIT License
 Project-URL: homepage, https://github.com/csm10495/shadowcopy
 Project-URL: repository, https://github.com/csm10495/shadowcopy
 Project-URL: documentation, https://csm10495.github.io/shadowcopy
 Classifier: Intended Audience :: Developers
```

### Comparing `shadowcopy-0.0.3/tests/test_shadowcopy.py` & `shadowcopy-0.0.4/tests/test_shadowcopy.py`

 * *Files identical despite different names*

