# Comparing `tmp/wizlib-0.2.5.tar.gz` & `tmp/wizlib-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wizlib-0.2.5.tar", last modified: Sun Jun 25 03:49:49 2023, max compression
+gzip compressed data, was "wizlib-0.2.6.tar", last modified: Sat Jul  8 17:05:43 2023, max compression
```

## Comparing `wizlib-0.2.5.tar` & `wizlib-0.2.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 03:49:49.971556 wizlib-0.2.5/
--rw-r--r--   0 root         (0) root         (0)        5 2023-06-25 03:49:19.000000 wizlib-0.2.5/.version
--rw-r--r--   0 root         (0) root         (0)     1771 2023-06-25 03:49:49.970556 wizlib-0.2.5/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1506 2023-06-25 03:49:41.000000 wizlib-0.2.5/README.md
--rw-rw-rw-   0 root         (0) root         (0)      541 2023-06-25 03:49:41.000000 wizlib-0.2.5/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-25 03:49:49.971556 wizlib-0.2.5/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 03:49:49.969556 wizlib-0.2.5/wizlib/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-25 03:49:41.000000 wizlib-0.2.5/wizlib/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1626 2023-06-25 03:49:41.000000 wizlib-0.2.5/wizlib/rlinput.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 03:49:49.970556 wizlib-0.2.5/wizlib.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1771 2023-06-25 03:49:49.000000 wizlib-0.2.5/wizlib.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      219 2023-06-25 03:49:49.000000 wizlib-0.2.5/wizlib.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-25 03:49:49.000000 wizlib-0.2.5/wizlib.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       89 2023-06-25 03:49:49.000000 wizlib-0.2.5/wizlib.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-06-25 03:49:49.000000 wizlib-0.2.5/wizlib.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-08 17:05:43.679513 wizlib-0.2.6/
+-rw-rw-rw-   0 root         (0) root         (0)        5 2023-07-08 17:04:55.000000 wizlib-0.2.6/.version
+-rw-r--r--   0 root         (0) root         (0)     1771 2023-07-08 17:05:43.679513 wizlib-0.2.6/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1506 2023-07-08 17:05:35.000000 wizlib-0.2.6/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      541 2023-07-08 17:05:35.000000 wizlib-0.2.6/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-08 17:05:43.679513 wizlib-0.2.6/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-08 17:05:43.678513 wizlib-0.2.6/wizlib/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-08 17:05:35.000000 wizlib-0.2.6/wizlib/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1626 2023-07-08 17:05:35.000000 wizlib-0.2.6/wizlib/rlinput.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-08 17:05:43.679513 wizlib-0.2.6/wizlib.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1771 2023-07-08 17:05:43.000000 wizlib-0.2.6/wizlib.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      219 2023-07-08 17:05:43.000000 wizlib-0.2.6/wizlib.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-08 17:05:43.000000 wizlib-0.2.6/wizlib.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       89 2023-07-08 17:05:43.000000 wizlib-0.2.6/wizlib.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-07-08 17:05:43.000000 wizlib-0.2.6/wizlib.egg-info/top_level.txt
```

### Comparing `wizlib-0.2.5/PKG-INFO` & `wizlib-0.2.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wizlib
-Version: 0.2.5
+Version: 0.2.6
 Summary: A collection of Python modules that are useful across multiple projects
 Author-email: Francis Potter <wizlib@steampunkwizard.ca>
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # WizLib
```

### Comparing `wizlib-0.2.5/README.md` & `wizlib-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `wizlib-0.2.5/pyproject.toml` & `wizlib-0.2.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `wizlib-0.2.5/wizlib/rlinput.py` & `wizlib-0.2.6/wizlib/rlinput.py`

 * *Files identical despite different names*

### Comparing `wizlib-0.2.5/wizlib.egg-info/PKG-INFO` & `wizlib-0.2.6/wizlib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wizlib
-Version: 0.2.5
+Version: 0.2.6
 Summary: A collection of Python modules that are useful across multiple projects
 Author-email: Francis Potter <wizlib@steampunkwizard.ca>
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # WizLib
```

