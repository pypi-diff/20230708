# Comparing `tmp/roxbot-0.7.0.tar.gz` & `tmp/roxbot-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "roxbot-0.7.0.tar", last modified: Tue Jul  4 12:03:20 2023, max compression
+gzip compressed data, was "roxbot-0.8.2.tar", last modified: Sat Jul  8 10:56:15 2023, max compression
```

## Comparing `roxbot-0.7.0.tar` & `roxbot-0.8.2.tar`

### file list

```diff
@@ -1,38 +1,39 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 12:03:20.177186 roxbot-0.7.0/
--rw-rw-rw-   0 root         (0) root         (0)     1081 2023-07-04 12:03:08.000000 roxbot-0.7.0/LICENCE
--rw-r--r--   0 root         (0) root         (0)      382 2023-07-04 12:03:20.177186 roxbot-0.7.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1734 2023-07-04 12:03:08.000000 roxbot-0.7.0/README.md
--rw-rw-rw-   0 root         (0) root         (0)      360 2023-07-04 12:03:20.178187 roxbot-0.7.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1570 2023-07-04 12:03:08.000000 roxbot-0.7.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 12:03:20.170186 roxbot-0.7.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 12:03:20.173186 roxbot-0.7.0/src/roxbot/
--rw-rw-rw-   0 root         (0) root         (0)       22 2023-07-04 12:03:08.000000 roxbot-0.7.0/src/roxbot/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1095 2023-07-04 12:03:08.000000 roxbot-0.7.0/src/roxbot/base_classes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 12:03:20.175186 roxbot-0.7.0/src/roxbot/bridges/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-04 12:03:08.000000 roxbot-0.7.0/src/roxbot/bridges/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4917 2023-07-04 12:03:08.000000 roxbot-0.7.0/src/roxbot/bridges/web_bridge.py
--rw-rw-rw-   0 root         (0) root         (0)      302 2023-07-04 12:03:08.000000 roxbot-0.7.0/src/roxbot/cli.py
--rw-rw-rw-   0 root         (0) root         (0)     5874 2023-07-04 12:03:08.000000 roxbot-0.7.0/src/roxbot/gps.py
--rw-rw-rw-   0 root         (0) root         (0)      337 2023-07-04 12:03:08.000000 roxbot-0.7.0/src/roxbot/interfaces.py
--rw-rw-rw-   0 root         (0) root         (0)     9200 2023-07-04 12:03:08.000000 roxbot-0.7.0/src/roxbot/models.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-04 12:03:08.000000 roxbot-0.7.0/src/roxbot/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 12:03:20.175186 roxbot-0.7.0/src/roxbot/simulators/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-04 12:03:08.000000 roxbot-0.7.0/src/roxbot/simulators/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      209 2023-07-04 12:03:08.000000 roxbot-0.7.0/src/roxbot/utils.py
--rw-rw-rw-   0 root         (0) root         (0)     5020 2023-07-04 12:03:08.000000 roxbot-0.7.0/src/roxbot/vectors.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 12:03:20.175186 roxbot-0.7.0/src/roxbot.egg-info/
--rw-r--r--   0 root         (0) root         (0)      382 2023-07-04 12:03:20.000000 roxbot-0.7.0/src/roxbot.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      715 2023-07-04 12:03:20.000000 roxbot-0.7.0/src/roxbot.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-04 12:03:20.000000 roxbot-0.7.0/src/roxbot.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       42 2023-07-04 12:03:20.000000 roxbot-0.7.0/src/roxbot.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-04 12:03:11.000000 roxbot-0.7.0/src/roxbot.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       55 2023-07-04 12:03:20.000000 roxbot-0.7.0/src/roxbot.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-07-04 12:03:20.000000 roxbot-0.7.0/src/roxbot.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 12:03:20.177186 roxbot-0.7.0/tests/
--rw-rw-rw-   0 root         (0) root         (0)      462 2023-07-04 12:03:08.000000 roxbot-0.7.0/tests/test_cli.py
--rw-rw-rw-   0 root         (0) root         (0)     2780 2023-07-04 12:03:08.000000 roxbot-0.7.0/tests/test_gps.py
--rw-rw-rw-   0 root         (0) root         (0)      103 2023-07-04 12:03:08.000000 roxbot-0.7.0/tests/test_interfaces.py
--rw-rw-rw-   0 root         (0) root         (0)     2345 2023-07-04 12:03:08.000000 roxbot-0.7.0/tests/test_models.py
--rw-rw-rw-   0 root         (0) root         (0)     1847 2023-07-04 12:03:08.000000 roxbot-0.7.0/tests/test_trike.py
--rw-rw-rw-   0 root         (0) root         (0)     2781 2023-07-04 12:03:08.000000 roxbot-0.7.0/tests/test_vectors.py
--rw-rw-rw-   0 root         (0) root         (0)     1982 2023-07-04 12:03:08.000000 roxbot-0.7.0/tests/test_ws_bridge.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-08 10:56:15.710415 roxbot-0.8.2/
+-rw-rw-rw-   0 root         (0) root         (0)     1081 2023-07-08 10:56:04.000000 roxbot-0.8.2/LICENCE
+-rw-r--r--   0 root         (0) root         (0)      382 2023-07-08 10:56:15.710415 roxbot-0.8.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1734 2023-07-08 10:56:04.000000 roxbot-0.8.2/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      360 2023-07-08 10:56:15.710415 roxbot-0.8.2/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1219 2023-07-08 10:56:04.000000 roxbot-0.8.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-08 10:56:15.704415 roxbot-0.8.2/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-08 10:56:15.707415 roxbot-0.8.2/src/roxbot/
+-rw-rw-rw-   0 root         (0) root         (0)       22 2023-07-08 10:56:04.000000 roxbot-0.8.2/src/roxbot/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1095 2023-07-08 10:56:04.000000 roxbot-0.8.2/src/roxbot/base_classes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-08 10:56:15.708415 roxbot-0.8.2/src/roxbot/bridges/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-08 10:56:04.000000 roxbot-0.8.2/src/roxbot/bridges/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4917 2023-07-08 10:56:04.000000 roxbot-0.8.2/src/roxbot/bridges/web_bridge.py
+-rw-rw-rw-   0 root         (0) root         (0)      334 2023-07-08 10:56:04.000000 roxbot-0.8.2/src/roxbot/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     5874 2023-07-08 10:56:04.000000 roxbot-0.8.2/src/roxbot/gps.py
+-rw-rw-rw-   0 root         (0) root         (0)      337 2023-07-08 10:56:04.000000 roxbot-0.8.2/src/roxbot/interfaces.py
+-rw-rw-rw-   0 root         (0) root         (0)     9200 2023-07-08 10:56:04.000000 roxbot-0.8.2/src/roxbot/models.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-08 10:56:04.000000 roxbot-0.8.2/src/roxbot/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-08 10:56:15.709415 roxbot-0.8.2/src/roxbot/simulators/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-08 10:56:04.000000 roxbot-0.8.2/src/roxbot/simulators/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      209 2023-07-08 10:56:04.000000 roxbot-0.8.2/src/roxbot/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     5020 2023-07-08 10:56:04.000000 roxbot-0.8.2/src/roxbot/vectors.py
+-rw-rw-rw-   0 root         (0) root         (0)     2640 2023-07-08 10:56:04.000000 roxbot-0.8.2/src/roxbot/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-08 10:56:15.708415 roxbot-0.8.2/src/roxbot.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      382 2023-07-08 10:56:15.000000 roxbot-0.8.2/src/roxbot.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-08 10:56:15.000000 roxbot-0.8.2/src/roxbot.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-08 10:56:15.000000 roxbot-0.8.2/src/roxbot.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       42 2023-07-08 10:56:15.000000 roxbot-0.8.2/src/roxbot.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-08 10:56:07.000000 roxbot-0.8.2/src/roxbot.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       55 2023-07-08 10:56:15.000000 roxbot-0.8.2/src/roxbot.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-07-08 10:56:15.000000 roxbot-0.8.2/src/roxbot.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-08 10:56:15.710415 roxbot-0.8.2/tests/
+-rw-rw-rw-   0 root         (0) root         (0)      462 2023-07-08 10:56:04.000000 roxbot-0.8.2/tests/test_cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     2780 2023-07-08 10:56:04.000000 roxbot-0.8.2/tests/test_gps.py
+-rw-rw-rw-   0 root         (0) root         (0)      103 2023-07-08 10:56:04.000000 roxbot-0.8.2/tests/test_interfaces.py
+-rw-rw-rw-   0 root         (0) root         (0)     2345 2023-07-08 10:56:04.000000 roxbot-0.8.2/tests/test_models.py
+-rw-rw-rw-   0 root         (0) root         (0)     1847 2023-07-08 10:56:04.000000 roxbot-0.8.2/tests/test_trike.py
+-rw-rw-rw-   0 root         (0) root         (0)     2781 2023-07-08 10:56:04.000000 roxbot-0.8.2/tests/test_vectors.py
+-rw-rw-rw-   0 root         (0) root         (0)     1982 2023-07-08 10:56:04.000000 roxbot-0.8.2/tests/test_ws_bridge.py
```

### Comparing `roxbot-0.7.0/LICENCE` & `roxbot-0.8.2/LICENCE`

 * *Files identical despite different names*

### Comparing `roxbot-0.7.0/README.md` & `roxbot-0.8.2/README.md`

 * *Files identical despite different names*

### Comparing `roxbot-0.7.0/setup.py` & `roxbot-0.8.2/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,32 +1,20 @@
 # type: ignore
 
 """The setup script."""
 
-
-import codecs
-import os
-import os.path
-
+from pathlib import Path
+import sys
 from setuptools import find_packages, setup
 
 
-def read(rel_path):
-    here = os.path.abspath(os.path.dirname(__file__))
-    with codecs.open(os.path.join(here, rel_path), "r") as fp:
-        return fp.read()
-
+# add src to path
+sys.path.append(str(Path(__file__).parent / "src"))
 
-def get_version(rel_path):
-    for line in read(rel_path).splitlines():
-        if line.startswith("__version__"):
-            delim = '"' if '"' in line else "'"
-            return line.split(delim)[1]
-        else:
-            raise RuntimeError("Unable to find version string.")
+from roxbot.version import get_version  # noqa: E402
 
 
 # please keep this lean and mean. Add dev requirements to .devcontainer/requirments.txt
 requirements = ["click", "pymap3d", "pynmea2", "websockets", "asyncio-mqtt", "pydantic"]
 
 test_requirements = [
     "pytest>=3",
@@ -48,12 +36,12 @@
     keywords="",
     name="roxbot",
     package_dir={"": "src"},
     packages=find_packages("src"),
     test_suite="tests",
     tests_require=test_requirements,
     url="",
-    version=get_version("src/roxbot/__init__.py"),
+    version=get_version(),
     zip_safe=False,
     package_data={"roxbot": ["py.typed"]},
     entry_points={"console_scripts": ["roxbot=roxbot.cli:cli"]},
 )
```

### Comparing `roxbot-0.7.0/src/roxbot/base_classes.py` & `roxbot-0.8.2/src/roxbot/base_classes.py`

 * *Files identical despite different names*

### Comparing `roxbot-0.7.0/src/roxbot/bridges/web_bridge.py` & `roxbot-0.8.2/src/roxbot/bridges/web_bridge.py`

 * *Files identical despite different names*

### Comparing `roxbot-0.7.0/src/roxbot/gps.py` & `roxbot-0.8.2/src/roxbot/gps.py`

 * *Files identical despite different names*

### Comparing `roxbot-0.7.0/src/roxbot/models.py` & `roxbot-0.8.2/src/roxbot/models.py`

 * *Files identical despite different names*

### Comparing `roxbot-0.7.0/src/roxbot/vectors.py` & `roxbot-0.8.2/src/roxbot/vectors.py`

 * *Files identical despite different names*

### Comparing `roxbot-0.7.0/src/roxbot.egg-info/SOURCES.txt` & `roxbot-0.8.2/src/roxbot.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 src/roxbot/cli.py
 src/roxbot/gps.py
 src/roxbot/interfaces.py
 src/roxbot/models.py
 src/roxbot/py.typed
 src/roxbot/utils.py
 src/roxbot/vectors.py
+src/roxbot/version.py
 src/roxbot.egg-info/PKG-INFO
 src/roxbot.egg-info/SOURCES.txt
 src/roxbot.egg-info/dependency_links.txt
 src/roxbot.egg-info/entry_points.txt
 src/roxbot.egg-info/not-zip-safe
 src/roxbot.egg-info/requires.txt
 src/roxbot.egg-info/top_level.txt
```

### Comparing `roxbot-0.7.0/tests/test_gps.py` & `roxbot-0.8.2/tests/test_gps.py`

 * *Files identical despite different names*

### Comparing `roxbot-0.7.0/tests/test_models.py` & `roxbot-0.8.2/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `roxbot-0.7.0/tests/test_trike.py` & `roxbot-0.8.2/tests/test_trike.py`

 * *Files identical despite different names*

### Comparing `roxbot-0.7.0/tests/test_vectors.py` & `roxbot-0.8.2/tests/test_vectors.py`

 * *Files identical despite different names*

### Comparing `roxbot-0.7.0/tests/test_ws_bridge.py` & `roxbot-0.8.2/tests/test_ws_bridge.py`

 * *Files identical despite different names*

