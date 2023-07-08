# Comparing `tmp/slib-sorter-1.5.9.tar.gz` & `tmp/slib-sorter-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slib-sorter-1.5.9.tar", last modified: Sat Jul  8 14:03:45 2023, max compression
+gzip compressed data, was "slib-sorter-1.6.0.tar", last modified: Sat Jul  8 14:11:32 2023, max compression
```

## Comparing `slib-sorter-1.5.9.tar` & `slib-sorter-1.6.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-08 14:03:45.155292 slib-sorter-1.5.9/
--rw-rw-rw-   0        0        0    11558 2023-07-07 20:03:54.000000 slib-sorter-1.5.9/LICENSE
--rw-rw-rw-   0        0        0     2249 2023-07-08 14:03:45.154324 slib-sorter-1.5.9/PKG-INFO
--rw-rw-rw-   0        0        0     1773 2023-07-08 06:05:27.000000 slib-sorter-1.5.9/README.md
--rw-rw-rw-   0        0        0       42 2023-07-08 14:03:45.155292 slib-sorter-1.5.9/setup.cfg
--rw-rw-rw-   0        0        0     3018 2023-07-08 14:03:36.000000 slib-sorter-1.5.9/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-08 14:03:45.152323 slib-sorter-1.5.9/slib_sorter.egg-info/
--rw-rw-rw-   0        0        0     2249 2023-07-08 14:03:45.000000 slib-sorter-1.5.9/slib_sorter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      273 2023-07-08 14:03:45.000000 slib-sorter-1.5.9/slib_sorter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-08 14:03:45.000000 slib-sorter-1.5.9/slib_sorter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       57 2023-07-08 14:03:45.000000 slib-sorter-1.5.9/slib_sorter.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       17 2023-07-08 14:03:45.000000 slib-sorter-1.5.9/slib_sorter.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-07-08 14:03:45.000000 slib-sorter-1.5.9/slib_sorter.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-08 14:03:45.153317 slib-sorter-1.5.9/src/
--rw-rw-rw-   0        0        0        0 2023-06-28 15:10:46.000000 slib-sorter-1.5.9/src/__init__.py
--rw-rw-rw-   0        0        0    67210 2023-07-08 14:03:13.000000 slib-sorter-1.5.9/src/slib_sorter.py
+drwxrwxrwx   0        0        0        0 2023-07-08 14:11:32.381840 slib-sorter-1.6.0/
+-rw-rw-rw-   0        0        0    11558 2023-07-07 20:03:54.000000 slib-sorter-1.6.0/LICENSE
+-rw-rw-rw-   0        0        0     2249 2023-07-08 14:11:32.381840 slib-sorter-1.6.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1773 2023-07-08 06:05:27.000000 slib-sorter-1.6.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-08 14:11:32.381840 slib-sorter-1.6.0/setup.cfg
+-rw-rw-rw-   0        0        0     3018 2023-07-08 14:11:22.000000 slib-sorter-1.6.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-08 14:11:32.371841 slib-sorter-1.6.0/slib_sorter.egg-info/
+-rw-rw-rw-   0        0        0     2249 2023-07-08 14:11:32.000000 slib-sorter-1.6.0/slib_sorter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      273 2023-07-08 14:11:32.000000 slib-sorter-1.6.0/slib_sorter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-08 14:11:32.000000 slib-sorter-1.6.0/slib_sorter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       57 2023-07-08 14:11:32.000000 slib-sorter-1.6.0/slib_sorter.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       17 2023-07-08 14:11:32.000000 slib-sorter-1.6.0/slib_sorter.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-07-08 14:11:32.000000 slib-sorter-1.6.0/slib_sorter.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-08 14:11:32.380841 slib-sorter-1.6.0/src/
+-rw-rw-rw-   0        0        0        0 2023-06-28 15:10:46.000000 slib-sorter-1.6.0/src/__init__.py
+-rw-rw-rw-   0        0        0    67202 2023-07-08 14:10:10.000000 slib-sorter-1.6.0/src/slib_sorter.py
```

### Comparing `slib-sorter-1.5.9/LICENSE` & `slib-sorter-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `slib-sorter-1.5.9/PKG-INFO` & `slib-sorter-1.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slib-sorter
-Version: 1.5.9
+Version: 1.6.0
 Summary: A Python package for sorting Sample Libraries
 Home-page: https://github.com/nrdrch/slib-sorter
 Author: Lukas H
 Author-email: fettkindasindauchoke@gmail.com
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
```

### Comparing `slib-sorter-1.5.9/README.md` & `slib-sorter-1.6.0/README.md`

 * *Files identical despite different names*

### Comparing `slib-sorter-1.5.9/setup.py` & `slib-sorter-1.6.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,15 +57,15 @@
     
     if not os.path.exists(settings):
         with open(settings, 'w') as f:
             f.write(default_config)
     
     setuptools.setup(
         name="slib-sorter",
-        version="1.5.9",
+        version="1.6.0",
         author="Lukas H",
         author_email="fettkindasindauchoke@gmail.com",
         description="A Python package for sorting Sample Libraries",
         long_description=long_description,
         long_description_content_type="text/markdown",
         url="https://github.com/nrdrch/slib-sorter",
         packages=setuptools.find_packages(),
```

### Comparing `slib-sorter-1.5.9/slib_sorter.egg-info/PKG-INFO` & `slib-sorter-1.6.0/slib_sorter.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slib-sorter
-Version: 1.5.9
+Version: 1.6.0
 Summary: A Python package for sorting Sample Libraries
 Home-page: https://github.com/nrdrch/slib-sorter
 Author: Lukas H
 Author-email: fettkindasindauchoke@gmail.com
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
```

### Comparing `slib-sorter-1.5.9/src/slib_sorter.py` & `slib-sorter-1.6.0/src/slib_sorter.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from termcolor import colored
 def path_finder(levels_up=0):
     current_dir = os.path.abspath(os.path.dirname(__file__))
     if levels_up > 0:
         for _ in range(levels_up):
             current_dir = os.path.dirname(current_dir)
     return current_dir
-settings_f = os.path.join(os.environ['USERPROFILE'], 'Documents', 'WindowsPowerShell', 'Scripts', 'slib_sorter', 'settings.json')
+settings = os.path.join(os.environ['USERPROFILE'], 'Documents', 'WindowsPowerShell', 'Scripts', 'slib_sorter', 'settings.json')
 def check_dir(*paths):
     for path in paths:
         if not os.path.exists(path):
             os.makedirs(path)
 def join_corrected_paths(settings):
     settings_folder = os.path.join(os.environ['USERPROFILE'], 'Documents', 'WindowsPowerShell', 'Scripts', 'slib_sorter')
     settings = os.path.join(settings_folder, 'settings.json')
@@ -24,16 +24,16 @@
         corrected_path = path.replace("/", "\\")
         more_corrected_path = corrected_path.replace("~", os.environ['USERPROFILE'])
         joined_paths[key] = more_corrected_path
         check_dir(more_corrected_path)
     return joined_paths 
 settings_folder = os.path.join(os.environ['USERPROFILE'], 'Documents', 'WindowsPowerShell', 'Scripts', 'slib_sorter')
 settings = os.path.join(settings_folder, 'settings.json')
-with open(settings_f, "r") as file:
-        settings_f = json.load(file)
+with open(settings, "r") as file:
+        settings = json.load(file)
 def clr_get(settings):
     with open(settings, "r") as file:
         settings = json.load(file)
     clors = settings.get('Colors', {})
     parsed_clors = {}
     for key, value in clors.items():
         parsed_clors[key] = value
@@ -953,15 +953,14 @@
     shutil.rmtree(path1, onerror=remove_readonly)
     check_dir(path1)
     if settings.get("Show Top Title Bar", True):
         bar = settings.get("Top Title Bar")
         log_message(bar, j_clrs.get('Top Title Bar Color'), True, True)
     else:
         pass
-    
     if settings.get("Show Statistics", True):
         log_message(prompt1, j_clrs.get('Prompt Color'), False, False)
         log_message(f'sorted by name & file type:   ', j_clrs.get('Foreground Color 1'), False, False)
         log_message(f' {num_succeeded}', j_clrs.get('Successfully Sorted File Color'), False, True)
         log_message(prompt1, j_clrs.get('Prompt Color'), False, False)
         log_message(f'sorted only by file type: ', j_clrs.get('Foreground Color 1'), False, False)
         log_message(f' {num_failed}', j_clrs.get('Unsorted File Color'), False, True)
@@ -1044,10 +1043,10 @@
         log_message('           -help  '+ f'{spacer}', j_clrs.get('Foreground Color 1'), False, False)
         log_message('Displays Help', j_clrs.get('Statistics Value Color'), False, True)
     elif args.config:
         settingsfile = settings_f
         cmd = "Start "+ f'{settingsfile}'
         os.system(cmd)
     else:
-        sort_files(path1, pattern_lists) 
+        sort_files(file_path, pattern_lists) 
 def __main__():
     print_help_message()
```

