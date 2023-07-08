# Comparing `tmp/slib-sorter-1.3.1.tar.gz` & `tmp/slib-sorter-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slib-sorter-1.3.1.tar", last modified: Sat Jul  8 06:51:02 2023, max compression
+gzip compressed data, was "slib-sorter-1.3.2.tar", last modified: Sat Jul  8 08:35:50 2023, max compression
```

## Comparing `slib-sorter-1.3.1.tar` & `slib-sorter-1.3.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-08 06:51:02.354162 slib-sorter-1.3.1/
--rw-rw-rw-   0        0        0    11558 2023-07-07 20:03:54.000000 slib-sorter-1.3.1/LICENSE
--rw-rw-rw-   0        0        0     2249 2023-07-08 06:51:02.353158 slib-sorter-1.3.1/PKG-INFO
--rw-rw-rw-   0        0        0     1773 2023-07-08 06:05:27.000000 slib-sorter-1.3.1/README.md
--rw-rw-rw-   0        0        0       42 2023-07-08 06:51:02.354162 slib-sorter-1.3.1/setup.cfg
--rw-rw-rw-   0        0        0     2994 2023-07-08 06:50:39.000000 slib-sorter-1.3.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-08 06:51:02.344188 slib-sorter-1.3.1/slib_sorter.egg-info/
--rw-rw-rw-   0        0        0     2249 2023-07-08 06:51:02.000000 slib-sorter-1.3.1/slib_sorter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      273 2023-07-08 06:51:02.000000 slib-sorter-1.3.1/slib_sorter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-08 06:51:02.000000 slib-sorter-1.3.1/slib_sorter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       57 2023-07-08 06:51:02.000000 slib-sorter-1.3.1/slib_sorter.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       17 2023-07-08 06:51:02.000000 slib-sorter-1.3.1/slib_sorter.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-07-08 06:51:02.000000 slib-sorter-1.3.1/slib_sorter.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-08 06:51:02.352189 slib-sorter-1.3.1/src/
--rw-rw-rw-   0        0        0        0 2023-06-28 15:10:46.000000 slib-sorter-1.3.1/src/__init__.py
--rw-rw-rw-   0        0        0    67740 2023-07-08 06:50:27.000000 slib-sorter-1.3.1/src/slib_sorter.py
+drwxrwxrwx   0        0        0        0 2023-07-08 08:35:50.586832 slib-sorter-1.3.2/
+-rw-rw-rw-   0        0        0    11558 2023-07-07 20:03:54.000000 slib-sorter-1.3.2/LICENSE
+-rw-rw-rw-   0        0        0     2249 2023-07-08 08:35:50.586832 slib-sorter-1.3.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1773 2023-07-08 06:05:27.000000 slib-sorter-1.3.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-08 08:35:50.586832 slib-sorter-1.3.2/setup.cfg
+-rw-rw-rw-   0        0        0     3056 2023-07-08 08:35:46.000000 slib-sorter-1.3.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-08 08:35:50.584802 slib-sorter-1.3.2/slib_sorter.egg-info/
+-rw-rw-rw-   0        0        0     2249 2023-07-08 08:35:50.000000 slib-sorter-1.3.2/slib_sorter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      273 2023-07-08 08:35:50.000000 slib-sorter-1.3.2/slib_sorter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-08 08:35:50.000000 slib-sorter-1.3.2/slib_sorter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       57 2023-07-08 08:35:50.000000 slib-sorter-1.3.2/slib_sorter.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       17 2023-07-08 08:35:50.000000 slib-sorter-1.3.2/slib_sorter.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-07-08 08:35:50.000000 slib-sorter-1.3.2/slib_sorter.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-08 08:35:50.585834 slib-sorter-1.3.2/src/
+-rw-rw-rw-   0        0        0        0 2023-06-28 15:10:46.000000 slib-sorter-1.3.2/src/__init__.py
+-rw-rw-rw-   0        0        0    63176 2023-07-08 08:23:36.000000 slib-sorter-1.3.2/src/slib_sorter.py
```

### Comparing `slib-sorter-1.3.1/LICENSE` & `slib-sorter-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `slib-sorter-1.3.1/PKG-INFO` & `slib-sorter-1.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slib-sorter
-Version: 1.3.1
+Version: 1.3.2
 Summary: A Python package for sorting Sample Libraries
 Home-page: https://github.com/nrdrch/slib-sorter
 Author: Lukas H
 Author-email: fettkindasindauchoke@gmail.com
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
```

### Comparing `slib-sorter-1.3.1/README.md` & `slib-sorter-1.3.2/README.md`

 * *Files identical despite different names*

### Comparing `slib-sorter-1.3.1/setup.py` & `slib-sorter-1.3.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,37 +1,14 @@
 import setuptools
 import shutil
 import os
 import json, importlib
 settings_folder = os.path.join(os.environ['USERPROFILE'], 'Documents', 'WindowsPowerShell', 'Scripts', 'slib_sorter')
 settings = os.path.join(settings_folder, "settings.json")
-default_config = f'''
-{{
-    "Foregroud Color 1": "white",
-    "Top Bar Color": "dark_grey",
-    "Show Top Bar": true,
-    "Top Bar": "<   Sample Library Sorter   >",
-    "Prompt Color": "dark_grey",
-    "Prompt": "$ ",
-    "Console Log Seperator": "  >>>--<>  ",
-    "Show More Console Logs": false,
-    "Show Seperator": true,
-    "Show Statistics": true,
-    "Statistics Value Color": "light_red",
-    "Max files per Dir": 50,
-    "TBPDPath": "~/Desktop",
-    "To Be Processed Directory": "To Be Sorted",
-    "NOFLDPath": "Desktop",
-    "Name Of Top Library Directory": "Sample Library",
-    "RFPath": "Desktop",
-    "Rejected Files": "Rejected Files",
-    "Run Shell Command On Startup": false,
-    "Command On Startup": "cls" 
-}}
-    '''
+
 def ps_script(source_file):
     
     winpro = os.path.join(os.environ['USERPROFILE'],'Documents', 'WindowsPowerShell')
     powershell_scripts_folder = os.path.join(winpro, 'Scripts', 'slib_sorter')
     settings_file_ps = os.path.join(powershell_scripts_folder, 'settings.json')
     if not os.path.exists(powershell_scripts_folder):
         os.makedirs(powershell_scripts_folder)
@@ -44,21 +21,46 @@
 settings_source = 'settings.json'
 
 def install():
     with open("README.md", "r", encoding="utf-8") as fh:
         long_description = fh.read()
     if not os.path.exists(settings_file):
         with open(settings_file, 'w') as f:
+            default_config = f'''
+{{
+    "Paths": {
+        "To Be Processed Directory": "~/Desktop/To Be Processed",
+        "Name Of Top Library Directory": "~/Desktop/Sample Library",
+        "Rejected Files Directory": "~/Desktop/Rejected Files"
+    },
+    "Colors": {
+        "Foregroud Color 1": "white",
+        "Top Title Bar Color": "dark_grey",
+        "Prompt Color": "dark_grey",
+        "Statistics Value Color": "light_red"
+    },
+    "Show Top Title Bar": true,
+    "Show Statistics": true,
+    "Show More Console Logs": false,
+    "Show Seperator": true,
+    "Console Log Seperator": "  >>>--<>  ",
+    "Top Title Bar": "<   Sample Library Sorter   >",
+    "Prompt": "$ ",
+    "Max files per Dir": 50,
+    "Run Shell Command On Startup": false,
+    "Command On Startup": "cls" 
+}}
+''' 
             f.write(default_config)
     else:
         pass
 
     setuptools.setup(
         name="slib-sorter",
-        version="1.3.1",
+        version="1.3.2",
         author="Lukas H",
         author_email="fettkindasindauchoke@gmail.com",
         description="A Python package for sorting Sample Libraries",
         long_description=long_description,
         long_description_content_type="text/markdown",
         url="https://github.com/nrdrch/slib-sorter",
         packages=setuptools.find_packages(),
```

### Comparing `slib-sorter-1.3.1/slib_sorter.egg-info/PKG-INFO` & `slib-sorter-1.3.2/slib_sorter.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slib-sorter
-Version: 1.3.1
+Version: 1.3.2
 Summary: A Python package for sorting Sample Libraries
 Home-page: https://github.com/nrdrch/slib-sorter
 Author: Lukas H
 Author-email: fettkindasindauchoke@gmail.com
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
```

