# Comparing `tmp/spike2py-0.2.1.tar.gz` & `tmp/spike2py-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spike2py-0.2.1.tar", last modified: Wed Jul  5 05:21:06 2023, max compression
+gzip compressed data, was "spike2py-0.2.2.tar", last modified: Sat Jul  8 02:57:38 2023, max compression
```

## Comparing `spike2py-0.2.1.tar` & `spike2py-0.2.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-07-05 05:21:06.684959 spike2py-0.2.1/
--rw-r--r--   0 martin    (1000) martin    (1000)    35149 2023-04-08 08:32:31.000000 spike2py-0.2.1/LICENSE
--rw-rw-r--   0 martin    (1000) martin    (1000)     3396 2023-07-05 05:21:06.684959 spike2py-0.2.1/PKG-INFO
--rw-r--r--   0 martin    (1000) martin    (1000)     2922 2023-07-05 05:17:42.000000 spike2py-0.2.1/README.md
--rw-rw-r--   0 martin    (1000) martin    (1000)       38 2023-07-05 05:21:06.684959 spike2py-0.2.1/setup.cfg
--rw-rw-r--   0 martin    (1000) martin    (1000)      945 2023-07-05 05:18:35.000000 spike2py-0.2.1/setup.py
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-07-05 05:21:06.684959 spike2py-0.2.1/spike2py/
--rw-r--r--   0 martin    (1000) martin    (1000)      166 2023-04-08 08:32:31.000000 spike2py-0.2.1/spike2py/__init__.py
--rw-r--r--   0 martin    (1000) martin    (1000)     8662 2023-07-05 04:37:33.000000 spike2py-0.2.1/spike2py/channels.py
--rw-r--r--   0 martin    (1000) martin    (1000)     1264 2023-04-08 08:32:31.000000 spike2py-0.2.1/spike2py/demo.py
--rw-r--r--   0 martin    (1000) martin    (1000)     7474 2023-07-03 02:40:10.000000 spike2py-0.2.1/spike2py/plot.py
--rw-r--r--   0 martin    (1000) martin    (1000)     7891 2023-07-05 05:12:52.000000 spike2py-0.2.1/spike2py/read.py
--rw-r--r--   0 martin    (1000) martin    (1000)     1569 2023-04-08 08:32:31.000000 spike2py-0.2.1/spike2py/reflex.py
--rw-r--r--   0 martin    (1000) martin    (1000)     6980 2023-04-08 08:32:31.000000 spike2py-0.2.1/spike2py/sig_proc.py
--rw-rw-r--   0 martin    (1000) martin    (1000)      606 2023-04-08 08:32:31.000000 spike2py-0.2.1/spike2py/temp_script.py
--rw-r--r--   0 martin    (1000) martin    (1000)     6091 2023-07-05 04:38:10.000000 spike2py-0.2.1/spike2py/trial.py
--rw-r--r--   0 martin    (1000) martin    (1000)      934 2023-07-05 04:25:25.000000 spike2py-0.2.1/spike2py/types.py
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-07-05 05:21:06.684959 spike2py-0.2.1/spike2py.egg-info/
--rw-rw-r--   0 martin    (1000) martin    (1000)     3396 2023-07-05 05:21:06.000000 spike2py-0.2.1/spike2py.egg-info/PKG-INFO
--rw-rw-r--   0 martin    (1000) martin    (1000)      378 2023-07-05 05:21:06.000000 spike2py-0.2.1/spike2py.egg-info/SOURCES.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)        1 2023-07-05 05:21:06.000000 spike2py-0.2.1/spike2py.egg-info/dependency_links.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)       23 2023-07-05 05:21:06.000000 spike2py-0.2.1/spike2py.egg-info/requires.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)        9 2023-07-05 05:21:06.000000 spike2py-0.2.1/spike2py.egg-info/top_level.txt
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-07-08 02:57:38.026599 spike2py-0.2.2/
+-rw-rw-r--   0 martin    (1000) martin    (1000)    35149 2023-04-08 08:32:31.000000 spike2py-0.2.2/LICENSE
+-rw-rw-r--   0 martin    (1000) martin    (1000)     3396 2023-07-08 02:57:38.026599 spike2py-0.2.2/PKG-INFO
+-rw-r--r--   0 martin    (1000) martin    (1000)     2922 2023-07-05 05:17:42.000000 spike2py-0.2.2/README.md
+-rw-rw-r--   0 martin    (1000) martin    (1000)       38 2023-07-08 02:57:38.026599 spike2py-0.2.2/setup.cfg
+-rw-r--r--   0 martin    (1000) martin    (1000)      945 2023-07-08 02:56:14.000000 spike2py-0.2.2/setup.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-07-08 02:57:38.026599 spike2py-0.2.2/spike2py/
+-rw-rw-r--   0 martin    (1000) martin    (1000)      166 2023-04-08 08:32:31.000000 spike2py-0.2.2/spike2py/__init__.py
+-rw-r--r--   0 martin    (1000) martin    (1000)     8662 2023-07-05 04:37:33.000000 spike2py-0.2.2/spike2py/channels.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1264 2023-04-08 08:32:31.000000 spike2py-0.2.2/spike2py/demo.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     7474 2023-07-03 02:40:10.000000 spike2py-0.2.2/spike2py/plot.py
+-rw-r--r--   0 martin    (1000) martin    (1000)     8470 2023-07-08 02:35:05.000000 spike2py-0.2.2/spike2py/read.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1569 2023-04-08 08:32:31.000000 spike2py-0.2.2/spike2py/reflex.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     6980 2023-04-08 08:32:31.000000 spike2py-0.2.2/spike2py/sig_proc.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)      606 2023-04-08 08:32:31.000000 spike2py-0.2.2/spike2py/temp_script.py
+-rw-r--r--   0 martin    (1000) martin    (1000)     6091 2023-07-05 04:38:10.000000 spike2py-0.2.2/spike2py/trial.py
+-rw-r--r--   0 martin    (1000) martin    (1000)      934 2023-07-05 04:25:25.000000 spike2py-0.2.2/spike2py/types.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-07-08 02:57:38.026599 spike2py-0.2.2/spike2py.egg-info/
+-rw-rw-r--   0 martin    (1000) martin    (1000)     3396 2023-07-08 02:57:37.000000 spike2py-0.2.2/spike2py.egg-info/PKG-INFO
+-rw-rw-r--   0 martin    (1000) martin    (1000)      378 2023-07-08 02:57:38.000000 spike2py-0.2.2/spike2py.egg-info/SOURCES.txt
+-rw-rw-r--   0 martin    (1000) martin    (1000)        1 2023-07-08 02:57:37.000000 spike2py-0.2.2/spike2py.egg-info/dependency_links.txt
+-rw-rw-r--   0 martin    (1000) martin    (1000)       23 2023-07-08 02:57:37.000000 spike2py-0.2.2/spike2py.egg-info/requires.txt
+-rw-rw-r--   0 martin    (1000) martin    (1000)        9 2023-07-08 02:57:37.000000 spike2py-0.2.2/spike2py.egg-info/top_level.txt
```

### Comparing `spike2py-0.2.1/LICENSE` & `spike2py-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `spike2py-0.2.1/PKG-INFO` & `spike2py-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spike2py
-Version: 0.2.1
+Version: 0.2.2
 Summary: Import, parse and process data collected with Spike2
 Home-page: https://github.com/MartinHeroux/spike2py
 Author: Martin Héroux
 Author-email: heroux.martin@gmail.com
 License: GNU General Public License v3 or later (GPLv3+)
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `spike2py-0.2.1/README.md` & `spike2py-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `spike2py-0.2.1/setup.py` & `spike2py-0.2.2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 # This call to setup() does all the work
 setup(
     name="spike2py",
-    version="0.2.1",
+    version="0.2.2",
     description="Import, parse and process data collected with Spike2",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/MartinHeroux/spike2py",
     author="Martin Héroux",
     author_email="heroux.martin@gmail.com",
     license="GNU General Public License v3 or later (GPLv3+)",
```

### Comparing `spike2py-0.2.1/spike2py/channels.py` & `spike2py-0.2.2/spike2py/channels.py`

 * *Files identical despite different names*

### Comparing `spike2py-0.2.1/spike2py/demo.py` & `spike2py-0.2.2/spike2py/demo.py`

 * *Files identical despite different names*

### Comparing `spike2py-0.2.1/spike2py/plot.py` & `spike2py-0.2.2/spike2py/plot.py`

 * *Files identical despite different names*

### Comparing `spike2py-0.2.1/spike2py/read.py` & `spike2py-0.2.2/spike2py/read.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import sys
 from pathlib import Path
 import textwrap
 from typing import List, Final
 
 import scipy.io as sio
 import numpy as np
 
@@ -77,22 +78,37 @@
 
     Returns
     -------
     dict
         Requested channels with channel names as `keys` and deeply nested
         arrays containing channel data as `values`.
     """
-    data: dict = sio.loadmat(mat_file)
+    try:
+        data: dict = sio.loadmat(mat_file)
+    except:
+        print(f'File {mat_file} not found. Please verify path and file name and try again.')
+        sys.exit(1)
+    all_channels = [data_key for data_key in data.keys() if not data_key.startswith("__")]
     if channels is None:
-        channels = [
-            data_key for data_key in data.keys() if not data_key.startswith("__")
-        ]
+        channels = all_channels
+    else:
+        _verify_channels_exists(channels, all_channels, mat_data)
     return {key: value for (key, value) in data.items() if key in channels}
 
 
+def _verify_channels_exists(channels, all_channels, mat_file):
+    for channel in channels:
+        if channel not in all_channels:
+            print(f"Channel {channel} does not exist in {mat_file}. \n"
+                  f"Available channels include:\n")
+            for ch in all_channels:
+                print(ch)
+            sys.exit(1)
+
+
 def _parse_mat_data(mat_data: mat_data) -> parsed_mat_data:
     """Parse deeply nested array that contain channel data
 
     Parameters
     ----------
     mat_data
         Deeply nested array containing channel data and metadata.
```

### Comparing `spike2py-0.2.1/spike2py/reflex.py` & `spike2py-0.2.2/spike2py/reflex.py`

 * *Files identical despite different names*

### Comparing `spike2py-0.2.1/spike2py/sig_proc.py` & `spike2py-0.2.2/spike2py/sig_proc.py`

 * *Files identical despite different names*

### Comparing `spike2py-0.2.1/spike2py/temp_script.py` & `spike2py-0.2.2/spike2py/temp_script.py`

 * *Files identical despite different names*

### Comparing `spike2py-0.2.1/spike2py/trial.py` & `spike2py-0.2.2/spike2py/trial.py`

 * *Files identical despite different names*

### Comparing `spike2py-0.2.1/spike2py/types.py` & `spike2py-0.2.2/spike2py/types.py`

 * *Files identical despite different names*

### Comparing `spike2py-0.2.1/spike2py.egg-info/PKG-INFO` & `spike2py-0.2.2/spike2py.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spike2py
-Version: 0.2.1
+Version: 0.2.2
 Summary: Import, parse and process data collected with Spike2
 Home-page: https://github.com/MartinHeroux/spike2py
 Author: Martin Héroux
 Author-email: heroux.martin@gmail.com
 License: GNU General Public License v3 or later (GPLv3+)
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3.8
```

