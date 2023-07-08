# Comparing `tmp/spike2py_preprocess-0.0.2.tar.gz` & `tmp/spike2py_preprocess-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spike2py_preprocess-0.0.2.tar", last modified: Tue Jul  4 06:06:01 2023, max compression
+gzip compressed data, was "spike2py_preprocess-0.0.3.tar", last modified: Sat Jul  8 04:05:40 2023, max compression
```

## Comparing `spike2py_preprocess-0.0.2.tar` & `spike2py_preprocess-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-07-04 06:06:01.070707 spike2py_preprocess-0.0.2/
--rw-r--r--   0 martin    (1000) martin    (1000)    35149 2023-07-02 04:35:06.000000 spike2py_preprocess-0.0.2/LICENSE
--rw-rw-r--   0 martin    (1000) martin    (1000)     6052 2023-07-04 06:06:01.070707 spike2py_preprocess-0.0.2/PKG-INFO
--rw-r--r--   0 martin    (1000) martin    (1000)     5579 2023-07-04 04:06:53.000000 spike2py_preprocess-0.0.2/README.md
--rw-rw-r--   0 martin    (1000) martin    (1000)       38 2023-07-04 06:06:01.070707 spike2py_preprocess-0.0.2/setup.cfg
--rw-rw-r--   0 martin    (1000) martin    (1000)      975 2023-07-04 06:04:37.000000 spike2py_preprocess-0.0.2/setup.py
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-07-04 06:06:01.070707 spike2py_preprocess-0.0.2/spike2py_preprocess/
--rw-r--r--   0 martin    (1000) martin    (1000)       22 2023-07-02 04:35:07.000000 spike2py_preprocess-0.0.2/spike2py_preprocess/__init__.py
--rw-r--r--   0 martin    (1000) martin    (1000)     6755 2023-07-04 05:41:14.000000 spike2py_preprocess-0.0.2/spike2py_preprocess/preprocess.py
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-07-04 06:06:01.070707 spike2py_preprocess-0.0.2/spike2py_preprocess.egg-info/
--rw-rw-r--   0 martin    (1000) martin    (1000)     6052 2023-07-04 06:06:01.000000 spike2py_preprocess-0.0.2/spike2py_preprocess.egg-info/PKG-INFO
--rw-rw-r--   0 martin    (1000) martin    (1000)      306 2023-07-04 06:06:01.000000 spike2py_preprocess-0.0.2/spike2py_preprocess.egg-info/SOURCES.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)        1 2023-07-04 06:06:01.000000 spike2py_preprocess-0.0.2/spike2py_preprocess.egg-info/dependency_links.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)        9 2023-07-04 06:06:01.000000 spike2py_preprocess-0.0.2/spike2py_preprocess.egg-info/requires.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)       20 2023-07-04 06:06:01.000000 spike2py_preprocess-0.0.2/spike2py_preprocess.egg-info/top_level.txt
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-07-08 04:05:40.120379 spike2py_preprocess-0.0.3/
+-rw-r--r--   0 martin    (1000) martin    (1000)    35149 2023-07-02 04:35:06.000000 spike2py_preprocess-0.0.3/LICENSE
+-rw-rw-r--   0 martin    (1000) martin    (1000)     6072 2023-07-08 04:05:40.120379 spike2py_preprocess-0.0.3/PKG-INFO
+-rw-r--r--   0 martin    (1000) martin    (1000)     5579 2023-07-04 04:06:53.000000 spike2py_preprocess-0.0.3/README.md
+-rw-rw-r--   0 martin    (1000) martin    (1000)       38 2023-07-08 04:05:40.120379 spike2py_preprocess-0.0.3/setup.cfg
+-rw-r--r--   0 martin    (1000) martin    (1000)      975 2023-07-08 04:02:19.000000 spike2py_preprocess-0.0.3/setup.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-07-08 04:05:40.120379 spike2py_preprocess-0.0.3/spike2py_preprocess/
+-rw-r--r--   0 martin    (1000) martin    (1000)       22 2023-07-02 04:35:07.000000 spike2py_preprocess-0.0.3/spike2py_preprocess/__init__.py
+-rw-r--r--   0 martin    (1000) martin    (1000)     7183 2023-07-08 04:01:12.000000 spike2py_preprocess-0.0.3/spike2py_preprocess/preprocess.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-07-08 04:05:40.120379 spike2py_preprocess-0.0.3/spike2py_preprocess.egg-info/
+-rw-r--r--   0 martin    (1000) martin    (1000)     6072 2023-07-08 04:05:40.000000 spike2py_preprocess-0.0.3/spike2py_preprocess.egg-info/PKG-INFO
+-rw-r--r--   0 martin    (1000) martin    (1000)      306 2023-07-08 04:05:40.000000 spike2py_preprocess-0.0.3/spike2py_preprocess.egg-info/SOURCES.txt
+-rw-r--r--   0 martin    (1000) martin    (1000)        1 2023-07-08 04:05:40.000000 spike2py_preprocess-0.0.3/spike2py_preprocess.egg-info/dependency_links.txt
+-rw-r--r--   0 martin    (1000) martin    (1000)        9 2023-07-08 04:05:40.000000 spike2py_preprocess-0.0.3/spike2py_preprocess.egg-info/requires.txt
+-rw-r--r--   0 martin    (1000) martin    (1000)       20 2023-07-08 04:05:40.000000 spike2py_preprocess-0.0.3/spike2py_preprocess.egg-info/top_level.txt
```

### Comparing `spike2py_preprocess-0.0.2/LICENSE` & `spike2py_preprocess-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `spike2py_preprocess-0.0.2/PKG-INFO` & `spike2py_preprocess-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: spike2py_preprocess
-Version: 0.0.2
+Version: 0.0.3
 Summary: Preprocess data with spike2py
 Home-page: https://github.com/MartinHeroux/spike2py_preprocess
 Author: Martin Héroux
 Author-email: heroux.martin@gmail.com
 License: GNU General Public License v3 or later (GPLv3+)
+Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![spike2py](https://raw.githubusercontent.com/MartinHeroux/spike2py_preprocess/master/spike2py_preprocess_icon_600x300.png)](https://github.com/MartinHeroux/spike2py)
 
@@ -156,7 +157,9 @@
 ## Code of conduct
 
 This project adheres to the Contributor Covenant code of conduct. By participating, you are expected to uphold this code. Please report unacceptable behavior to [heroux.martin@gmail.com](heroux.martin@gmail.com).
 
 ## License
 
 [GPLv3](./LICENSE)
+
+
```

### Comparing `spike2py_preprocess-0.0.2/README.md` & `spike2py_preprocess-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `spike2py_preprocess-0.0.2/setup.py` & `spike2py_preprocess-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 # This call to setup() does all the work
 setup(
     name="spike2py_preprocess",
-    version="0.0.2",
+    version="0.0.3",
     description="Preprocess data with spike2py",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/MartinHeroux/spike2py_preprocess",
     author="Martin Héroux",
     author_email="heroux.martin@gmail.com",
     license="GNU General Public License v3 or later (GPLv3+)",
```

### Comparing `spike2py_preprocess-0.0.2/spike2py_preprocess/preprocess.py` & `spike2py_preprocess-0.0.3/spike2py_preprocess/preprocess.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import sys
 import json
 from pathlib import Path
 from typing import Union
 from dataclasses import dataclass
 
 from rich import print
 
@@ -58,18 +59,18 @@
     None
         When file not found and strict=False.
     """
     try:
         with open(json_path, "r") as file:
             return json.load(file)
     except FileNotFoundError:
-        message = f'{json_path.name} does not exist.'
-        if strict:
-            raise FileNotFoundError(message)
+        message = f'{json_path} does not exist.'
         print(message)
+        if strict:
+            sys.exit(1)
         return
 
 
 def trial(trial_info: TrialInfo, preprocess_info: Union[dict, None] = None):
     """
     Read, preprocess (if required) and pickle trial data.
 
@@ -99,26 +100,36 @@
     if preprocess_file.exists():
         return read_json(preprocess_file)
     else:
         return preprocess_info
 
 
 def _get_data(trial_info):
-    data = Trial(trial_info)
+    try:
+        data = Trial(trial_info)
+    except FileNotFoundError:
+        print(f'Unable to read {trial_info.file}. Please make sure it exists.')
+        sys.exit(1)
     return data
 
 
 def _preprocess_trial(data, preprocess_info):
     """Preprocess each channel specified in preprocess_info.
 
     Each preprocessing step is specified with relevant arguments;
     these are applied to the relevant channels."""
     for channel, preprocesses in preprocess_info.items():
         for preprocess_name, preprocess_arguments in preprocesses.items():
-            exec(f"data.{channel}.{preprocess_name}({preprocess_arguments})")
+            try:
+                exec(f"data.{channel}.{preprocess_name}({preprocess_arguments})")
+            except AttributeError:
+                print(f'Following spike2py data does not have requested attribute: \n'
+                      f"\tdata.{channel}.{preprocess_name}({preprocess_arguments})\n"
+                      f"{data.info.name}")
+                sys.exit(1)
     return data
 
 
 def subject(
     subject_path: Path,
     preprocess_info: Union[dict, None] = None,
     study_info: Union[dict, None] = None,
```

### Comparing `spike2py_preprocess-0.0.2/spike2py_preprocess.egg-info/PKG-INFO` & `spike2py_preprocess-0.0.3/spike2py_preprocess.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: spike2py-preprocess
-Version: 0.0.2
+Version: 0.0.3
 Summary: Preprocess data with spike2py
 Home-page: https://github.com/MartinHeroux/spike2py_preprocess
 Author: Martin Héroux
 Author-email: heroux.martin@gmail.com
 License: GNU General Public License v3 or later (GPLv3+)
+Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![spike2py](https://raw.githubusercontent.com/MartinHeroux/spike2py_preprocess/master/spike2py_preprocess_icon_600x300.png)](https://github.com/MartinHeroux/spike2py)
 
@@ -156,7 +157,9 @@
 ## Code of conduct
 
 This project adheres to the Contributor Covenant code of conduct. By participating, you are expected to uphold this code. Please report unacceptable behavior to [heroux.martin@gmail.com](heroux.martin@gmail.com).
 
 ## License
 
 [GPLv3](./LICENSE)
+
+
```

