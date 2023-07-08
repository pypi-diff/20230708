# Comparing `tmp/roxbot-0.8.2.tar.gz` & `tmp/roxbot-0.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "roxbot-0.8.2.tar", last modified: Sat Jul  8 10:56:15 2023, max compression
+gzip compressed data, was "roxbot-0.8.3.tar", last modified: Sat Jul  8 11:13:20 2023, max compression
```

## Comparing `roxbot-0.8.2.tar` & `roxbot-0.8.3.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-08 10:56:15.710415 roxbot-0.8.2/
--rw-rw-rw-   0 root         (0) root         (0)     1081 2023-07-08 10:56:04.000000 roxbot-0.8.2/LICENCE
--rw-r--r--   0 root         (0) root         (0)      382 2023-07-08 10:56:15.710415 roxbot-0.8.2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1734 2023-07-08 10:56:04.000000 roxbot-0.8.2/README.md
--rw-rw-rw-   0 root         (0) root         (0)      360 2023-07-08 10:56:15.710415 roxbot-0.8.2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1219 2023-07-08 10:56:04.000000 roxbot-0.8.2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-08 10:56:15.704415 roxbot-0.8.2/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-08 10:56:15.707415 roxbot-0.8.2/src/roxbot/
--rw-rw-rw-   0 root         (0) root         (0)       22 2023-07-08 10:56:04.000000 roxbot-0.8.2/src/roxbot/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1095 2023-07-08 10:56:04.000000 roxbot-0.8.2/src/roxbot/base_classes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-08 10:56:15.708415 roxbot-0.8.2/src/roxbot/bridges/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-08 10:56:04.000000 roxbot-0.8.2/src/roxbot/bridges/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4917 2023-07-08 10:56:04.000000 roxbot-0.8.2/src/roxbot/bridges/web_bridge.py
--rw-rw-rw-   0 root         (0) root         (0)      334 2023-07-08 10:56:04.000000 roxbot-0.8.2/src/roxbot/cli.py
--rw-rw-rw-   0 root         (0) root         (0)     5874 2023-07-08 10:56:04.000000 roxbot-0.8.2/src/roxbot/gps.py
--rw-rw-rw-   0 root         (0) root         (0)      337 2023-07-08 10:56:04.000000 roxbot-0.8.2/src/roxbot/interfaces.py
--rw-rw-rw-   0 root         (0) root         (0)     9200 2023-07-08 10:56:04.000000 roxbot-0.8.2/src/roxbot/models.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-08 10:56:04.000000 roxbot-0.8.2/src/roxbot/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-08 10:56:15.709415 roxbot-0.8.2/src/roxbot/simulators/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-08 10:56:04.000000 roxbot-0.8.2/src/roxbot/simulators/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      209 2023-07-08 10:56:04.000000 roxbot-0.8.2/src/roxbot/utils.py
--rw-rw-rw-   0 root         (0) root         (0)     5020 2023-07-08 10:56:04.000000 roxbot-0.8.2/src/roxbot/vectors.py
--rw-rw-rw-   0 root         (0) root         (0)     2640 2023-07-08 10:56:04.000000 roxbot-0.8.2/src/roxbot/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-08 10:56:15.708415 roxbot-0.8.2/src/roxbot.egg-info/
--rw-r--r--   0 root         (0) root         (0)      382 2023-07-08 10:56:15.000000 roxbot-0.8.2/src/roxbot.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-08 10:56:15.000000 roxbot-0.8.2/src/roxbot.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-08 10:56:15.000000 roxbot-0.8.2/src/roxbot.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       42 2023-07-08 10:56:15.000000 roxbot-0.8.2/src/roxbot.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-08 10:56:07.000000 roxbot-0.8.2/src/roxbot.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       55 2023-07-08 10:56:15.000000 roxbot-0.8.2/src/roxbot.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-07-08 10:56:15.000000 roxbot-0.8.2/src/roxbot.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-08 10:56:15.710415 roxbot-0.8.2/tests/
--rw-rw-rw-   0 root         (0) root         (0)      462 2023-07-08 10:56:04.000000 roxbot-0.8.2/tests/test_cli.py
--rw-rw-rw-   0 root         (0) root         (0)     2780 2023-07-08 10:56:04.000000 roxbot-0.8.2/tests/test_gps.py
--rw-rw-rw-   0 root         (0) root         (0)      103 2023-07-08 10:56:04.000000 roxbot-0.8.2/tests/test_interfaces.py
--rw-rw-rw-   0 root         (0) root         (0)     2345 2023-07-08 10:56:04.000000 roxbot-0.8.2/tests/test_models.py
--rw-rw-rw-   0 root         (0) root         (0)     1847 2023-07-08 10:56:04.000000 roxbot-0.8.2/tests/test_trike.py
--rw-rw-rw-   0 root         (0) root         (0)     2781 2023-07-08 10:56:04.000000 roxbot-0.8.2/tests/test_vectors.py
--rw-rw-rw-   0 root         (0) root         (0)     1982 2023-07-08 10:56:04.000000 roxbot-0.8.2/tests/test_ws_bridge.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-08 11:13:20.552539 roxbot-0.8.3/
+-rw-rw-rw-   0 root         (0) root         (0)     1081 2023-07-08 11:13:09.000000 roxbot-0.8.3/LICENCE
+-rw-r--r--   0 root         (0) root         (0)      382 2023-07-08 11:13:20.552539 roxbot-0.8.3/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1734 2023-07-08 11:13:09.000000 roxbot-0.8.3/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      360 2023-07-08 11:13:20.553539 roxbot-0.8.3/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1219 2023-07-08 11:13:09.000000 roxbot-0.8.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-08 11:13:20.546539 roxbot-0.8.3/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-08 11:13:20.549539 roxbot-0.8.3/src/roxbot/
+-rw-rw-rw-   0 root         (0) root         (0)       22 2023-07-08 11:13:09.000000 roxbot-0.8.3/src/roxbot/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1095 2023-07-08 11:13:09.000000 roxbot-0.8.3/src/roxbot/base_classes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-08 11:13:20.551539 roxbot-0.8.3/src/roxbot/bridges/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-08 11:13:09.000000 roxbot-0.8.3/src/roxbot/bridges/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4917 2023-07-08 11:13:09.000000 roxbot-0.8.3/src/roxbot/bridges/web_bridge.py
+-rw-rw-rw-   0 root         (0) root         (0)      334 2023-07-08 11:13:09.000000 roxbot-0.8.3/src/roxbot/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     5874 2023-07-08 11:13:09.000000 roxbot-0.8.3/src/roxbot/gps.py
+-rw-rw-rw-   0 root         (0) root         (0)      337 2023-07-08 11:13:09.000000 roxbot-0.8.3/src/roxbot/interfaces.py
+-rw-rw-rw-   0 root         (0) root         (0)     9200 2023-07-08 11:13:09.000000 roxbot-0.8.3/src/roxbot/models.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-08 11:13:09.000000 roxbot-0.8.3/src/roxbot/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-08 11:13:20.551539 roxbot-0.8.3/src/roxbot/simulators/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-08 11:13:09.000000 roxbot-0.8.3/src/roxbot/simulators/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      209 2023-07-08 11:13:09.000000 roxbot-0.8.3/src/roxbot/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     5020 2023-07-08 11:13:09.000000 roxbot-0.8.3/src/roxbot/vectors.py
+-rw-rw-rw-   0 root         (0) root         (0)     2894 2023-07-08 11:13:09.000000 roxbot-0.8.3/src/roxbot/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-08 11:13:20.551539 roxbot-0.8.3/src/roxbot.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      382 2023-07-08 11:13:20.000000 roxbot-0.8.3/src/roxbot.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-08 11:13:20.000000 roxbot-0.8.3/src/roxbot.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-08 11:13:20.000000 roxbot-0.8.3/src/roxbot.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       42 2023-07-08 11:13:20.000000 roxbot-0.8.3/src/roxbot.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-08 11:13:12.000000 roxbot-0.8.3/src/roxbot.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       55 2023-07-08 11:13:20.000000 roxbot-0.8.3/src/roxbot.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-07-08 11:13:20.000000 roxbot-0.8.3/src/roxbot.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-08 11:13:20.552539 roxbot-0.8.3/tests/
+-rw-rw-rw-   0 root         (0) root         (0)      462 2023-07-08 11:13:09.000000 roxbot-0.8.3/tests/test_cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     2780 2023-07-08 11:13:09.000000 roxbot-0.8.3/tests/test_gps.py
+-rw-rw-rw-   0 root         (0) root         (0)      103 2023-07-08 11:13:09.000000 roxbot-0.8.3/tests/test_interfaces.py
+-rw-rw-rw-   0 root         (0) root         (0)     2345 2023-07-08 11:13:09.000000 roxbot-0.8.3/tests/test_models.py
+-rw-rw-rw-   0 root         (0) root         (0)     1847 2023-07-08 11:13:09.000000 roxbot-0.8.3/tests/test_trike.py
+-rw-rw-rw-   0 root         (0) root         (0)     2781 2023-07-08 11:13:09.000000 roxbot-0.8.3/tests/test_vectors.py
+-rw-rw-rw-   0 root         (0) root         (0)     1982 2023-07-08 11:13:09.000000 roxbot-0.8.3/tests/test_ws_bridge.py
```

### Comparing `roxbot-0.8.2/LICENCE` & `roxbot-0.8.3/LICENCE`

 * *Files identical despite different names*

### Comparing `roxbot-0.8.2/README.md` & `roxbot-0.8.3/README.md`

 * *Files identical despite different names*

### Comparing `roxbot-0.8.2/setup.py` & `roxbot-0.8.3/setup.py`

 * *Files identical despite different names*

### Comparing `roxbot-0.8.2/src/roxbot/base_classes.py` & `roxbot-0.8.3/src/roxbot/base_classes.py`

 * *Files identical despite different names*

### Comparing `roxbot-0.8.2/src/roxbot/bridges/web_bridge.py` & `roxbot-0.8.3/src/roxbot/bridges/web_bridge.py`

 * *Files identical despite different names*

### Comparing `roxbot-0.8.2/src/roxbot/gps.py` & `roxbot-0.8.3/src/roxbot/gps.py`

 * *Files identical despite different names*

### Comparing `roxbot-0.8.2/src/roxbot/models.py` & `roxbot-0.8.3/src/roxbot/models.py`

 * *Files identical despite different names*

### Comparing `roxbot-0.8.2/src/roxbot/vectors.py` & `roxbot-0.8.3/src/roxbot/vectors.py`

 * *Files identical despite different names*

### Comparing `roxbot-0.8.2/src/roxbot/version.py` & `roxbot-0.8.3/src/roxbot/version.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,19 +13,19 @@
 
     setup(
         ...
         version=get_version(),
         ...
     )
 """
-
-from pathlib import Path
 import codecs
 import os
 import subprocess
+from pathlib import Path
+from typing import Optional, Any
 
 
 def read(rel_path):
     here = os.path.abspath(os.path.dirname(__file__))
     with codecs.open(os.path.join(here, rel_path), "r") as fp:
         return fp.read()
 
@@ -35,25 +35,29 @@
         if line.startswith("__version__"):
             delim = '"' if '"' in line else "'"
             return line.split(delim)[1]
         else:
             raise RuntimeError("Unable to find version string.")
 
 
-def get_version(traverse_up=2) -> str:
+def get_version(pkg: Optional[Any] = None, traverse_up=2) -> str:
     """get version from git or __init__.py
 
     Args:
+        pkg (Optional[Any], optional): package, must have __file__ object. Defaults to None.
         traverse_up (int, optional): directory levels up to repo root. Defaults to 2.
 
     Returns:
-        _type_: _description_
+        str: package version
     """
     # get directory two levels up
-    root = Path(__file__).resolve().parents[traverse_up]
+    if pkg is not None:
+        root = Path(pkg.__file__).resolve().parents[traverse_up]
+    else:
+        root = Path(__file__).resolve().parents[traverse_up]
 
     if (root / ".git").exists():
         # Get the version using "git describe".
         cmd = "git describe --tags --match v[0-9]*".split()
         try:
             version = subprocess.check_output(cmd).decode().strip()
         except subprocess.CalledProcessError:
```

### Comparing `roxbot-0.8.2/src/roxbot.egg-info/SOURCES.txt` & `roxbot-0.8.3/src/roxbot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `roxbot-0.8.2/tests/test_gps.py` & `roxbot-0.8.3/tests/test_gps.py`

 * *Files identical despite different names*

### Comparing `roxbot-0.8.2/tests/test_models.py` & `roxbot-0.8.3/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `roxbot-0.8.2/tests/test_trike.py` & `roxbot-0.8.3/tests/test_trike.py`

 * *Files identical despite different names*

### Comparing `roxbot-0.8.2/tests/test_vectors.py` & `roxbot-0.8.3/tests/test_vectors.py`

 * *Files identical despite different names*

### Comparing `roxbot-0.8.2/tests/test_ws_bridge.py` & `roxbot-0.8.3/tests/test_ws_bridge.py`

 * *Files identical despite different names*

