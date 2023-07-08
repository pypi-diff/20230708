# Comparing `tmp/slib-sorter-1.5.2.tar.gz` & `tmp/slib-sorter-1.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slib-sorter-1.5.2.tar", last modified: Sat Jul  8 12:19:44 2023, max compression
+gzip compressed data, was "slib-sorter-1.5.3.tar", last modified: Sat Jul  8 12:25:18 2023, max compression
```

## Comparing `slib-sorter-1.5.2.tar` & `slib-sorter-1.5.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-08 12:19:44.000276 slib-sorter-1.5.2/
--rw-rw-rw-   0        0        0    11558 2023-07-07 20:03:54.000000 slib-sorter-1.5.2/LICENSE
--rw-rw-rw-   0        0        0     2249 2023-07-08 12:19:43.999268 slib-sorter-1.5.2/PKG-INFO
--rw-rw-rw-   0        0        0     1773 2023-07-08 06:05:27.000000 slib-sorter-1.5.2/README.md
--rw-rw-rw-   0        0        0       42 2023-07-08 12:19:44.000276 slib-sorter-1.5.2/setup.cfg
--rw-rw-rw-   0        0        0     3245 2023-07-08 12:19:05.000000 slib-sorter-1.5.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-08 12:19:43.990263 slib-sorter-1.5.2/slib_sorter.egg-info/
--rw-rw-rw-   0        0        0     2249 2023-07-08 12:19:43.000000 slib-sorter-1.5.2/slib_sorter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      273 2023-07-08 12:19:43.000000 slib-sorter-1.5.2/slib_sorter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-08 12:19:43.000000 slib-sorter-1.5.2/slib_sorter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       57 2023-07-08 12:19:43.000000 slib-sorter-1.5.2/slib_sorter.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       17 2023-07-08 12:19:43.000000 slib-sorter-1.5.2/slib_sorter.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-07-08 12:19:43.000000 slib-sorter-1.5.2/slib_sorter.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-08 12:19:43.998245 slib-sorter-1.5.2/src/
--rw-rw-rw-   0        0        0        0 2023-06-28 15:10:46.000000 slib-sorter-1.5.2/src/__init__.py
--rw-rw-rw-   0        0        0    66999 2023-07-08 12:18:38.000000 slib-sorter-1.5.2/src/slib_sorter.py
+drwxrwxrwx   0        0        0        0 2023-07-08 12:25:18.994617 slib-sorter-1.5.3/
+-rw-rw-rw-   0        0        0    11558 2023-07-07 20:03:54.000000 slib-sorter-1.5.3/LICENSE
+-rw-rw-rw-   0        0        0     2249 2023-07-08 12:25:18.993646 slib-sorter-1.5.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1773 2023-07-08 06:05:27.000000 slib-sorter-1.5.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-08 12:25:18.994617 slib-sorter-1.5.3/setup.cfg
+-rw-rw-rw-   0        0        0     3245 2023-07-08 12:24:16.000000 slib-sorter-1.5.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-08 12:25:18.991647 slib-sorter-1.5.3/slib_sorter.egg-info/
+-rw-rw-rw-   0        0        0     2249 2023-07-08 12:25:18.000000 slib-sorter-1.5.3/slib_sorter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      273 2023-07-08 12:25:18.000000 slib-sorter-1.5.3/slib_sorter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-08 12:25:18.000000 slib-sorter-1.5.3/slib_sorter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       57 2023-07-08 12:25:18.000000 slib-sorter-1.5.3/slib_sorter.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       17 2023-07-08 12:25:18.000000 slib-sorter-1.5.3/slib_sorter.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-07-08 12:25:18.000000 slib-sorter-1.5.3/slib_sorter.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-08 12:25:18.993646 slib-sorter-1.5.3/src/
+-rw-rw-rw-   0        0        0        0 2023-06-28 15:10:46.000000 slib-sorter-1.5.3/src/__init__.py
+-rw-rw-rw-   0        0        0    67001 2023-07-08 12:23:31.000000 slib-sorter-1.5.3/src/slib_sorter.py
```

### Comparing `slib-sorter-1.5.2/LICENSE` & `slib-sorter-1.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `slib-sorter-1.5.2/PKG-INFO` & `slib-sorter-1.5.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slib-sorter
-Version: 1.5.2
+Version: 1.5.3
 Summary: A Python package for sorting Sample Libraries
 Home-page: https://github.com/nrdrch/slib-sorter
 Author: Lukas H
 Author-email: fettkindasindauchoke@gmail.com
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
```

### Comparing `slib-sorter-1.5.2/README.md` & `slib-sorter-1.5.3/README.md`

 * *Files identical despite different names*

### Comparing `slib-sorter-1.5.2/setup.py` & `slib-sorter-1.5.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -56,15 +56,15 @@
 ''' 
         f.write(default_config)
     else:
         pass
 
     setuptools.setup(
         name="slib-sorter",
-        version="1.5.2",
+        version="1.5.3",
         author="Lukas H",
         author_email="fettkindasindauchoke@gmail.com",
         description="A Python package for sorting Sample Libraries",
         long_description=long_description,
         long_description_content_type="text/markdown",
         url="https://github.com/nrdrch/slib-sorter",
         packages=setuptools.find_packages(),
```

### Comparing `slib-sorter-1.5.2/slib_sorter.egg-info/PKG-INFO` & `slib-sorter-1.5.3/slib_sorter.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slib-sorter
-Version: 1.5.2
+Version: 1.5.3
 Summary: A Python package for sorting Sample Libraries
 Home-page: https://github.com/nrdrch/slib-sorter
 Author: Lukas H
 Author-email: fettkindasindauchoke@gmail.com
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
```

### Comparing `slib-sorter-1.5.2/src/slib_sorter.py` & `slib-sorter-1.5.3/src/slib_sorter.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 import os, shutil, stat, tempfile, json, ctypes, argparse, time, sys, subprocess
 from termcolor import colored
+settings_folder = os.path.join(os.environ['USERPROFILE'], 'Documents', 'WindowsPowerShell', 'Scripts', 'slib_sorter')
+settings = os.path.join(settings_folder, 'settings.json')
 def join_corrected_paths(settings):
     with open(settings, "r") as file:
         settings = json.load(file)
 
     paths = settings.get('Paths', {})
     joined_paths = {}
 
     for key, path in paths.items():
         corrected_path = path.replace("/", "\\")
         more_corrected_path = corrected_path.replace("~", os.environ['USERPROFILE'])
         joined_paths[key] = more_corrected_path
         check_dir(joined_paths)
     return joined_paths 
-settings_folder = os.path.join(os.environ['USERPROFILE'], 'Documents', 'WindowsPowerShell', 'Scripts', 'slib_sorter')
-settings = os.path.join(settings_folder, 'settings.json')
+
 def clr_get(settings):
     with open(settings, "r") as file:
         settings = json.load(file)
     clors = settings.get('Colors', {})
     parsed_clors = {}
     for key, value in clors.items():
         parsed_clors[key] = value
```

