# Comparing `tmp/slib-sorter-1.1.3.tar.gz` & `tmp/slib-sorter-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slib-sorter-1.1.3.tar", last modified: Sat Jul  8 02:36:22 2023, max compression
+gzip compressed data, was "slib-sorter-1.1.4.tar", last modified: Sat Jul  8 02:50:53 2023, max compression
```

## Comparing `slib-sorter-1.1.3.tar` & `slib-sorter-1.1.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-08 02:36:22.928582 slib-sorter-1.1.3/
--rw-rw-rw-   0        0        0    11558 2023-07-07 20:03:54.000000 slib-sorter-1.1.3/LICENSE
--rw-rw-rw-   0        0        0     2289 2023-07-08 02:36:22.928582 slib-sorter-1.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     1807 2023-07-07 20:03:54.000000 slib-sorter-1.1.3/README.md
--rw-rw-rw-   0        0        0       42 2023-07-08 02:36:22.928582 slib-sorter-1.1.3/setup.cfg
--rw-rw-rw-   0        0        0     4375 2023-07-08 02:36:10.000000 slib-sorter-1.1.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-08 02:36:22.926576 slib-sorter-1.1.3/slib_sorter.egg-info/
--rw-rw-rw-   0        0        0     2289 2023-07-08 02:36:22.000000 slib-sorter-1.1.3/slib_sorter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      273 2023-07-08 02:36:22.000000 slib-sorter-1.1.3/slib_sorter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-08 02:36:22.000000 slib-sorter-1.1.3/slib_sorter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       56 2023-07-08 02:36:22.000000 slib-sorter-1.1.3/slib_sorter.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       17 2023-07-08 02:36:22.000000 slib-sorter-1.1.3/slib_sorter.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-07-08 02:36:22.000000 slib-sorter-1.1.3/slib_sorter.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-08 02:36:22.927590 slib-sorter-1.1.3/src/
--rw-rw-rw-   0        0        0        0 2023-06-28 15:10:46.000000 slib-sorter-1.1.3/src/__init__.py
--rw-rw-rw-   0        0        0    72457 2023-07-08 02:20:39.000000 slib-sorter-1.1.3/src/slib_sorter.py
+drwxrwxrwx   0        0        0        0 2023-07-08 02:50:53.309754 slib-sorter-1.1.4/
+-rw-rw-rw-   0        0        0    11558 2023-07-07 20:03:54.000000 slib-sorter-1.1.4/LICENSE
+-rw-rw-rw-   0        0        0     2289 2023-07-08 02:50:53.309754 slib-sorter-1.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1807 2023-07-07 20:03:54.000000 slib-sorter-1.1.4/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-08 02:50:53.309754 slib-sorter-1.1.4/setup.cfg
+-rw-rw-rw-   0        0        0     4376 2023-07-08 02:50:15.000000 slib-sorter-1.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-08 02:50:53.300778 slib-sorter-1.1.4/slib_sorter.egg-info/
+-rw-rw-rw-   0        0        0     2289 2023-07-08 02:50:53.000000 slib-sorter-1.1.4/slib_sorter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      273 2023-07-08 02:50:53.000000 slib-sorter-1.1.4/slib_sorter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-08 02:50:53.000000 slib-sorter-1.1.4/slib_sorter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       57 2023-07-08 02:50:53.000000 slib-sorter-1.1.4/slib_sorter.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       17 2023-07-08 02:50:53.000000 slib-sorter-1.1.4/slib_sorter.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-07-08 02:50:53.000000 slib-sorter-1.1.4/slib_sorter.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-08 02:50:53.308820 slib-sorter-1.1.4/src/
+-rw-rw-rw-   0        0        0        0 2023-06-28 15:10:46.000000 slib-sorter-1.1.4/src/__init__.py
+-rw-rw-rw-   0        0        0    72439 2023-07-08 02:50:02.000000 slib-sorter-1.1.4/src/slib_sorter.py
```

### Comparing `slib-sorter-1.1.3/LICENSE` & `slib-sorter-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `slib-sorter-1.1.3/PKG-INFO` & `slib-sorter-1.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slib-sorter
-Version: 1.1.3
+Version: 1.1.4
 Summary: A Python library for sorting Sample Libraries
 Home-page: https://github.com/nrdrch/slib-sorter
 Author: Lukas Hübinger
 Author-email: fettkindasindauchoke@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
```

### Comparing `slib-sorter-1.1.3/README.md` & `slib-sorter-1.1.4/README.md`

 * *Files identical despite different names*

### Comparing `slib-sorter-1.1.3/setup.py` & `slib-sorter-1.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,25 +80,25 @@
         importlib.reload(settings_file)
 def install():
     with open("README.md", "r", encoding="utf-8") as fh:
         long_description = fh.read()
 
     setuptools.setup(
         name="slib-sorter",
-        version="1.1.3",
+        version="1.1.4",
         author="Lukas Hübinger",
         author_email="fettkindasindauchoke@gmail.com",
         description="A Python library for sorting Sample Libraries",
         long_description=long_description,
         long_description_content_type="text/markdown",
         url="https://github.com/nrdrch/slib-sorter",
         packages=setuptools.find_packages(), 
         entry_points={
             "console_scripts": [
-                "slibsorter = src.slib_sorter:__main__"
+                "Slib-Sorter = src.slib_sorter:__main__"
             ]
         },
         install_requires=[
             "termcolor==2.3.0"
         ],
         classifiers=[
             "Programming Language :: Python :: 3",
```

### Comparing `slib-sorter-1.1.3/slib_sorter.egg-info/PKG-INFO` & `slib-sorter-1.1.4/slib_sorter.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slib-sorter
-Version: 1.1.3
+Version: 1.1.4
 Summary: A Python library for sorting Sample Libraries
 Home-page: https://github.com/nrdrch/slib-sorter
 Author: Lukas Hübinger
 Author-email: fettkindasindauchoke@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
```

### Comparing `slib-sorter-1.1.3/src/slib_sorter.py` & `slib-sorter-1.1.4/src/slib_sorter.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,12 @@
 import os, shutil, stat, argparse
-
 import time
 import json
-
-import os, shutil, stat, tempfile, json, ctypes, importlib
 from termcolor import colored
-
+import os, shutil, stat, tempfile, json, ctypes, importlib
 def path_finder(levels_up=0):
     current_dir = os.path.abspath(os.path.dirname(__file__))
     if levels_up > 0:
         for _ in range(levels_up):
             current_dir = os.path.dirname(current_dir)
     return current_dir
 #settings = os.path.join(path_finder(0), 'settings.json')
@@ -1126,8 +1123,7 @@
         settingsfile = os.path.join(path_finder(0), 'settings.json')
         cmd = "Start "+ settingsfile
         os.system(cmd)
     else:
         sort_files(path1, pattern_lists) 
 def __main__():
     print_help_message()
-__main__()
```

