# Comparing `tmp/shadowcopy-0.0.1.tar.gz` & `tmp/shadowcopy-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shadowcopy-0.0.1.tar", last modified: Fri Jul  7 23:47:18 2023, max compression
+gzip compressed data, was "shadowcopy-0.0.2.tar", last modified: Fri Jul  7 23:52:40 2023, max compression
```

## Comparing `shadowcopy-0.0.1.tar` & `shadowcopy-0.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 23:47:18.734317 shadowcopy-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-07 23:46:58.000000 shadowcopy-0.0.1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-07-07 23:47:18.734317 shadowcopy-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-07-07 23:46:58.000000 shadowcopy-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      987 2023-07-07 23:46:58.000000 shadowcopy-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 23:47:18.734317 shadowcopy-0.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 23:47:18.734317 shadowcopy-0.0.1/shadowcopy/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-07 23:46:58.000000 shadowcopy-0.0.1/shadowcopy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-07-07 23:46:58.000000 shadowcopy-0.0.1/shadowcopy/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-07-07 23:46:58.000000 shadowcopy-0.0.1/shadowcopy/shadow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 23:47:18.734317 shadowcopy-0.0.1/shadowcopy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-07-07 23:47:18.000000 shadowcopy-0.0.1/shadowcopy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-07 23:47:18.000000 shadowcopy-0.0.1/shadowcopy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 23:47:18.000000 shadowcopy-0.0.1/shadowcopy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-07 23:47:18.000000 shadowcopy-0.0.1/shadowcopy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-07 23:47:18.000000 shadowcopy-0.0.1/shadowcopy.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 23:47:18.734317 shadowcopy-0.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-07-07 23:46:58.000000 shadowcopy-0.0.1/tests/test_shadowcopy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 23:52:40.203965 shadowcopy-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-07 23:52:26.000000 shadowcopy-0.0.2/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-07-07 23:52:40.203965 shadowcopy-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-07-07 23:52:26.000000 shadowcopy-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      987 2023-07-07 23:52:26.000000 shadowcopy-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 23:52:40.203965 shadowcopy-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 23:52:40.203965 shadowcopy-0.0.2/shadowcopy/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-07 23:52:26.000000 shadowcopy-0.0.2/shadowcopy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-07-07 23:52:26.000000 shadowcopy-0.0.2/shadowcopy/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-07-07 23:52:26.000000 shadowcopy-0.0.2/shadowcopy/shadow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 23:52:40.203965 shadowcopy-0.0.2/shadowcopy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-07-07 23:52:40.000000 shadowcopy-0.0.2/shadowcopy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-07 23:52:40.000000 shadowcopy-0.0.2/shadowcopy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 23:52:40.000000 shadowcopy-0.0.2/shadowcopy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-07 23:52:40.000000 shadowcopy-0.0.2/shadowcopy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-07 23:52:40.000000 shadowcopy-0.0.2/shadowcopy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 23:52:40.203965 shadowcopy-0.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-07-07 23:52:26.000000 shadowcopy-0.0.2/tests/test_shadowcopy.py
```

### Comparing `shadowcopy-0.0.1/LICENSE.md` & `shadowcopy-0.0.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `shadowcopy-0.0.1/PKG-INFO` & `shadowcopy-0.0.2/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shadowcopy
-Version: 0.0.1
+Version: 0.0.2
 Summary: A project for shadowcopy
 Author-email: csm10495 <csm10495@gmail.com>
 License: MIT License
 Project-URL: homepage, https://github.com/csm10495/shadowcopy
 Project-URL: repository, https://github.com/csm10495/shadowcopy
 Project-URL: documentation, https://csm10495.github.io/shadowcopy
 Classifier: Intended Audience :: Developers
@@ -20,16 +20,21 @@
 
 shadowcopy is a module for performing file copies from 'shadows' on Windows. Shadow copies are typically used to copy files that are locked for usage by other processes.
 
 More info on shadow copies in Windows can be found [here](https://learn.microsoft.com/en-us/windows-server/storage/file-server/volume-shadow-copy-service)
 
 Creating/Deleting shadown copies requires admin access.
 
-## Example
+## Installing
 
 ```
+pip install shadowcopy
+```
 
+## Example
+
+```
 from shadowcopy import shadow_copy
 
 # Internally this creates a shadow copy instance via WMI, copies the file, then deletes the shadow copy.
 shadow_copy("source.txt", "destination.txt")
 ```
```

### Comparing `shadowcopy-0.0.1/README.md` & `shadowcopy-0.0.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -2,16 +2,21 @@
 
 shadowcopy is a module for performing file copies from 'shadows' on Windows. Shadow copies are typically used to copy files that are locked for usage by other processes.
 
 More info on shadow copies in Windows can be found [here](https://learn.microsoft.com/en-us/windows-server/storage/file-server/volume-shadow-copy-service)
 
 Creating/Deleting shadown copies requires admin access.
 
-## Example
+## Installing
 
 ```
+pip install shadowcopy
+```
 
+## Example
+
+```
 from shadowcopy import shadow_copy
 
 # Internally this creates a shadow copy instance via WMI, copies the file, then deletes the shadow copy.
 shadow_copy("source.txt", "destination.txt")
 ```
```

### Comparing `shadowcopy-0.0.1/pyproject.toml` & `shadowcopy-0.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `shadowcopy-0.0.1/shadowcopy/exceptions.py` & `shadowcopy-0.0.2/shadowcopy/exceptions.py`

 * *Files identical despite different names*

### Comparing `shadowcopy-0.0.1/shadowcopy/shadow.py` & `shadowcopy-0.0.2/shadowcopy/shadow.py`

 * *Files identical despite different names*

### Comparing `shadowcopy-0.0.1/shadowcopy.egg-info/PKG-INFO` & `shadowcopy-0.0.2/shadowcopy.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shadowcopy
-Version: 0.0.1
+Version: 0.0.2
 Summary: A project for shadowcopy
 Author-email: csm10495 <csm10495@gmail.com>
 License: MIT License
 Project-URL: homepage, https://github.com/csm10495/shadowcopy
 Project-URL: repository, https://github.com/csm10495/shadowcopy
 Project-URL: documentation, https://csm10495.github.io/shadowcopy
 Classifier: Intended Audience :: Developers
@@ -20,16 +20,21 @@
 
 shadowcopy is a module for performing file copies from 'shadows' on Windows. Shadow copies are typically used to copy files that are locked for usage by other processes.
 
 More info on shadow copies in Windows can be found [here](https://learn.microsoft.com/en-us/windows-server/storage/file-server/volume-shadow-copy-service)
 
 Creating/Deleting shadown copies requires admin access.
 
-## Example
+## Installing
 
 ```
+pip install shadowcopy
+```
 
+## Example
+
+```
 from shadowcopy import shadow_copy
 
 # Internally this creates a shadow copy instance via WMI, copies the file, then deletes the shadow copy.
 shadow_copy("source.txt", "destination.txt")
 ```
```

### Comparing `shadowcopy-0.0.1/tests/test_shadowcopy.py` & `shadowcopy-0.0.2/tests/test_shadowcopy.py`

 * *Files identical despite different names*

