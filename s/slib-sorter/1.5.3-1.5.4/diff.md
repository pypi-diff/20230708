# Comparing `tmp/slib-sorter-1.5.3.tar.gz` & `tmp/slib-sorter-1.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slib-sorter-1.5.3.tar", last modified: Sat Jul  8 12:25:18 2023, max compression
+gzip compressed data, was "slib-sorter-1.5.4.tar", last modified: Sat Jul  8 12:48:22 2023, max compression
```

## Comparing `slib-sorter-1.5.3.tar` & `slib-sorter-1.5.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-08 12:25:18.994617 slib-sorter-1.5.3/
--rw-rw-rw-   0        0        0    11558 2023-07-07 20:03:54.000000 slib-sorter-1.5.3/LICENSE
--rw-rw-rw-   0        0        0     2249 2023-07-08 12:25:18.993646 slib-sorter-1.5.3/PKG-INFO
--rw-rw-rw-   0        0        0     1773 2023-07-08 06:05:27.000000 slib-sorter-1.5.3/README.md
--rw-rw-rw-   0        0        0       42 2023-07-08 12:25:18.994617 slib-sorter-1.5.3/setup.cfg
--rw-rw-rw-   0        0        0     3245 2023-07-08 12:24:16.000000 slib-sorter-1.5.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-08 12:25:18.991647 slib-sorter-1.5.3/slib_sorter.egg-info/
--rw-rw-rw-   0        0        0     2249 2023-07-08 12:25:18.000000 slib-sorter-1.5.3/slib_sorter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      273 2023-07-08 12:25:18.000000 slib-sorter-1.5.3/slib_sorter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-08 12:25:18.000000 slib-sorter-1.5.3/slib_sorter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       57 2023-07-08 12:25:18.000000 slib-sorter-1.5.3/slib_sorter.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       17 2023-07-08 12:25:18.000000 slib-sorter-1.5.3/slib_sorter.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-07-08 12:25:18.000000 slib-sorter-1.5.3/slib_sorter.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-08 12:25:18.993646 slib-sorter-1.5.3/src/
--rw-rw-rw-   0        0        0        0 2023-06-28 15:10:46.000000 slib-sorter-1.5.3/src/__init__.py
--rw-rw-rw-   0        0        0    67001 2023-07-08 12:23:31.000000 slib-sorter-1.5.3/src/slib_sorter.py
+drwxrwxrwx   0        0        0        0 2023-07-08 12:48:22.783311 slib-sorter-1.5.4/
+-rw-rw-rw-   0        0        0    11558 2023-07-07 20:03:54.000000 slib-sorter-1.5.4/LICENSE
+-rw-rw-rw-   0        0        0     2249 2023-07-08 12:48:22.783311 slib-sorter-1.5.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1773 2023-07-08 06:05:27.000000 slib-sorter-1.5.4/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-08 12:48:22.783311 slib-sorter-1.5.4/setup.cfg
+-rw-rw-rw-   0        0        0     3234 2023-07-08 12:48:12.000000 slib-sorter-1.5.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-08 12:48:22.781311 slib-sorter-1.5.4/slib_sorter.egg-info/
+-rw-rw-rw-   0        0        0     2249 2023-07-08 12:48:22.000000 slib-sorter-1.5.4/slib_sorter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      273 2023-07-08 12:48:22.000000 slib-sorter-1.5.4/slib_sorter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-08 12:48:22.000000 slib-sorter-1.5.4/slib_sorter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       57 2023-07-08 12:48:22.000000 slib-sorter-1.5.4/slib_sorter.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       17 2023-07-08 12:48:22.000000 slib-sorter-1.5.4/slib_sorter.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-07-08 12:48:22.000000 slib-sorter-1.5.4/slib_sorter.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-08 12:48:22.782309 slib-sorter-1.5.4/src/
+-rw-rw-rw-   0        0        0        0 2023-06-28 15:10:46.000000 slib-sorter-1.5.4/src/__init__.py
+-rw-rw-rw-   0        0        0    67024 2023-07-08 12:43:38.000000 slib-sorter-1.5.4/src/slib_sorter.py
```

### Comparing `slib-sorter-1.5.3/LICENSE` & `slib-sorter-1.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `slib-sorter-1.5.3/PKG-INFO` & `slib-sorter-1.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slib-sorter
-Version: 1.5.3
+Version: 1.5.4
 Summary: A Python package for sorting Sample Libraries
 Home-page: https://github.com/nrdrch/slib-sorter
 Author: Lukas H
 Author-email: fettkindasindauchoke@gmail.com
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
```

### Comparing `slib-sorter-1.5.3/README.md` & `slib-sorter-1.5.4/README.md`

 * *Files identical despite different names*

### Comparing `slib-sorter-1.5.3/setup.py` & `slib-sorter-1.5.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 import shutil
 import os
 import json, importlib
 settings_folder = os.path.join(os.environ['USERPROFILE'], 'Documents', 'WindowsPowerShell', 'Scripts', 'slib_sorter')
 settings = os.path.join(settings_folder, "settings.json")
 
 def ps_script(source_file):
-    
     winpro = os.path.join(os.environ['USERPROFILE'],'Documents', 'WindowsPowerShell')
     powershell_scripts_folder = os.path.join(winpro, 'Scripts', 'slib_sorter')
     settings_file_ps = os.path.join(powershell_scripts_folder, 'settings.json')
     if not os.path.exists(powershell_scripts_folder):
         os.makedirs(powershell_scripts_folder)
     else:
         pass
@@ -56,15 +55,15 @@
 ''' 
         f.write(default_config)
     else:
         pass
 
     setuptools.setup(
         name="slib-sorter",
-        version="1.5.3",
+        version="1.5.4",
         author="Lukas H",
         author_email="fettkindasindauchoke@gmail.com",
         description="A Python package for sorting Sample Libraries",
         long_description=long_description,
         long_description_content_type="text/markdown",
         url="https://github.com/nrdrch/slib-sorter",
         packages=setuptools.find_packages(), 
@@ -79,15 +78,15 @@
         classifiers=[
             "Programming Language :: Python :: 3.7",
             "License :: OSI Approved :: Apache Software License",
             "Operating System :: Microsoft :: Windows :: Windows 10"
         ],
     )
 
-    if not os.path.exists(settings_file):
+    if not os.path.exists(settings):
         ps_script(settings_source)
     else:
         pass
     
 
 def __setup__():
     install()
```

### Comparing `slib-sorter-1.5.3/slib_sorter.egg-info/PKG-INFO` & `slib-sorter-1.5.4/slib_sorter.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slib-sorter
-Version: 1.5.3
+Version: 1.5.4
 Summary: A Python package for sorting Sample Libraries
 Home-page: https://github.com/nrdrch/slib-sorter
 Author: Lukas H
 Author-email: fettkindasindauchoke@gmail.com
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
```

### Comparing `slib-sorter-1.5.3/src/slib_sorter.py` & `slib-sorter-1.5.4/src/slib_sorter.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,26 +1,33 @@
 import os, shutil, stat, tempfile, json, ctypes, argparse, time, sys, subprocess
 from termcolor import colored
-settings_folder = os.path.join(os.environ['USERPROFILE'], 'Documents', 'WindowsPowerShell', 'Scripts', 'slib_sorter')
-settings = os.path.join(settings_folder, 'settings.json')
+
+def check_dir(*paths):
+    for path in paths:
+        if not os.path.exists(*paths):
+            os.makedirs(*paths)
+        else:
+            pass
 def join_corrected_paths(settings):
     with open(settings, "r") as file:
         settings = json.load(file)
 
     paths = settings.get('Paths', {})
     joined_paths = {}
-
+    
     for key, path in paths.items():
         corrected_path = path.replace("/", "\\")
         more_corrected_path = corrected_path.replace("~", os.environ['USERPROFILE'])
         joined_paths[key] = more_corrected_path
-        check_dir(joined_paths)
+        check_dir(more_corrected_path)
     return joined_paths 
 
 def clr_get(settings):
+    settings_folder = os.path.join(os.environ['USERPROFILE'], 'Documents', 'WindowsPowerShell', 'Scripts', 'slib_sorter')
+    settings = os.path.join(settings_folder, 'settings.json')
     with open(settings, "r") as file:
         settings = json.load(file)
     clors = settings.get('Colors', {})
     parsed_clors = {}
     for key, value in clors.items():
         parsed_clors[key] = value
     return parsed_clors
@@ -28,26 +35,22 @@
 def path_finder(levels_up=0):
     current_dir = os.path.abspath(os.path.dirname(__file__))
     if levels_up > 0:
         for _ in range(levels_up):
             current_dir = os.path.dirname(current_dir)
     return current_dir
 #settings = os.path.join(path_finder(0), 'settings.json')
-def check_dir(*paths):
-    for path in paths:
-        if not os.path.exists(path):
-            os.makedirs(paths)
-        else:
-            pass
+
 settings_folder = os.path.join(os.environ['USERPROFILE'], 'Documents', 'WindowsPowerShell', 'Scripts', 'slib_sorter')
-settings_file = os.path.join(settings_folder, 'settings.json')
+settings = os.path.join(settings_folder, 'settings.json')
 j_clrs = clr_get(settings)
 j_paths = join_corrected_paths(settings)
 with open(settings, 'r') as file:
     settings = json.load(file)
+
 def log_message(message, color, centered=False, newline=True):
     if centered:
         message = message.center(119)
     end = "\n" if newline else ""
     print(colored(message, color), end=end)
 
 def log_console(file_name, seperator, dest_path, color):
```

