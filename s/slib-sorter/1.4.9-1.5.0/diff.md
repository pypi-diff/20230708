# Comparing `tmp/slib-sorter-1.4.9.tar.gz` & `tmp/slib-sorter-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slib-sorter-1.4.9.tar", last modified: Sat Jul  8 11:42:27 2023, max compression
+gzip compressed data, was "slib-sorter-1.5.0.tar", last modified: Sat Jul  8 12:04:41 2023, max compression
```

## Comparing `slib-sorter-1.4.9.tar` & `slib-sorter-1.5.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-08 11:42:27.001710 slib-sorter-1.4.9/
--rw-rw-rw-   0        0        0    11558 2023-07-07 20:03:54.000000 slib-sorter-1.4.9/LICENSE
--rw-rw-rw-   0        0        0     2249 2023-07-08 11:42:27.001710 slib-sorter-1.4.9/PKG-INFO
--rw-rw-rw-   0        0        0     1773 2023-07-08 06:05:27.000000 slib-sorter-1.4.9/README.md
--rw-rw-rw-   0        0        0       42 2023-07-08 11:42:27.001710 slib-sorter-1.4.9/setup.cfg
--rw-rw-rw-   0        0        0     3242 2023-07-08 11:41:52.000000 slib-sorter-1.4.9/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-08 11:42:26.991737 slib-sorter-1.4.9/slib_sorter.egg-info/
--rw-rw-rw-   0        0        0     2249 2023-07-08 11:42:26.000000 slib-sorter-1.4.9/slib_sorter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      273 2023-07-08 11:42:26.000000 slib-sorter-1.4.9/slib_sorter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-08 11:42:26.000000 slib-sorter-1.4.9/slib_sorter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       57 2023-07-08 11:42:26.000000 slib-sorter-1.4.9/slib_sorter.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       17 2023-07-08 11:42:26.000000 slib-sorter-1.4.9/slib_sorter.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-07-08 11:42:26.000000 slib-sorter-1.4.9/slib_sorter.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-08 11:42:27.000741 slib-sorter-1.4.9/src/
--rw-rw-rw-   0        0        0        0 2023-06-28 15:10:46.000000 slib-sorter-1.4.9/src/__init__.py
--rw-rw-rw-   0        0        0    67147 2023-07-08 11:41:49.000000 slib-sorter-1.4.9/src/slib_sorter.py
+drwxrwxrwx   0        0        0        0 2023-07-08 12:04:41.795261 slib-sorter-1.5.0/
+-rw-rw-rw-   0        0        0    11558 2023-07-07 20:03:54.000000 slib-sorter-1.5.0/LICENSE
+-rw-rw-rw-   0        0        0     2249 2023-07-08 12:04:41.795261 slib-sorter-1.5.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1773 2023-07-08 06:05:27.000000 slib-sorter-1.5.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-08 12:04:41.796259 slib-sorter-1.5.0/setup.cfg
+-rw-rw-rw-   0        0        0     3245 2023-07-08 12:04:14.000000 slib-sorter-1.5.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-08 12:04:41.785269 slib-sorter-1.5.0/slib_sorter.egg-info/
+-rw-rw-rw-   0        0        0     2249 2023-07-08 12:04:41.000000 slib-sorter-1.5.0/slib_sorter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      273 2023-07-08 12:04:41.000000 slib-sorter-1.5.0/slib_sorter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-08 12:04:41.000000 slib-sorter-1.5.0/slib_sorter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       57 2023-07-08 12:04:41.000000 slib-sorter-1.5.0/slib_sorter.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       17 2023-07-08 12:04:41.000000 slib-sorter-1.5.0/slib_sorter.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-07-08 12:04:41.000000 slib-sorter-1.5.0/slib_sorter.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-08 12:04:41.794249 slib-sorter-1.5.0/src/
+-rw-rw-rw-   0        0        0        0 2023-06-28 15:10:46.000000 slib-sorter-1.5.0/src/__init__.py
+-rw-rw-rw-   0        0        0    66815 2023-07-08 12:03:29.000000 slib-sorter-1.5.0/src/slib_sorter.py
```

### Comparing `slib-sorter-1.4.9/LICENSE` & `slib-sorter-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `slib-sorter-1.4.9/PKG-INFO` & `slib-sorter-1.5.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slib-sorter
-Version: 1.4.9
+Version: 1.5.0
 Summary: A Python package for sorting Sample Libraries
 Home-page: https://github.com/nrdrch/slib-sorter
 Author: Lukas H
 Author-email: fettkindasindauchoke@gmail.com
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
```

### Comparing `slib-sorter-1.4.9/README.md` & `slib-sorter-1.5.0/README.md`

 * *Files identical despite different names*

### Comparing `slib-sorter-1.4.9/setup.py` & `slib-sorter-1.5.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,25 +26,25 @@
     if not os.path.exists(settings_file):
         with open(settings_file, 'w') as f:
             default_config = f'''
 {{
     "Paths": {
         "To Be Processed Directory": "~/Desktop/To Be Processed",
         "Name Of Top Library Directory": "~/Desktop/Sample Library",
-        "Rejected Files Directory": "~/Desktop/Rejected Files"
+        "Rejected Filetype Directory": "~/Desktop/Rejected Files"
     },
     "Colors": {
         "Foregroud Color 1": "white",
         "Foregroud Color 2": "dark_grey",
-        "Top Title Bar Color": "white",
+        "Top Title Bar Color": "dark_grey",
         "Prompt Color": "dark_grey",
         "Statistics Value Color": "light_red",
         "Successfully Sorted File Color": "light_green",
         "Unsorted File Color": "light_yellow",
-        "Rejected Filetype Color": "magenta"
+        "Rejected Filetype Color": "red"
     },
     "Show More Console Logs": true,
     "Console Log Seperator": "  >>>--<>  ",
     "Top Title Bar": "<   Sample Library Sorter   >",
     "Prompt": "$ ",
     "Max files per Dir": 50,
     "Command On Startup": "cls",
@@ -56,15 +56,15 @@
 ''' 
         f.write(default_config)
     else:
         pass
 
     setuptools.setup(
         name="slib-sorter",
-        version="1.4.9",
+        version="1.5.0",
         author="Lukas H",
         author_email="fettkindasindauchoke@gmail.com",
         description="A Python package for sorting Sample Libraries",
         long_description=long_description,
         long_description_content_type="text/markdown",
         url="https://github.com/nrdrch/slib-sorter",
         packages=setuptools.find_packages(),
```

### Comparing `slib-sorter-1.4.9/slib_sorter.egg-info/PKG-INFO` & `slib-sorter-1.5.0/slib_sorter.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slib-sorter
-Version: 1.4.9
+Version: 1.5.0
 Summary: A Python package for sorting Sample Libraries
 Home-page: https://github.com/nrdrch/slib-sorter
 Author: Lukas H
 Author-email: fettkindasindauchoke@gmail.com
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
```

### Comparing `slib-sorter-1.4.9/src/slib_sorter.py` & `slib-sorter-1.5.0/src/slib_sorter.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,30 +1,23 @@
 import os, shutil, stat, tempfile, json, ctypes, argparse, time, sys, subprocess
 from termcolor import colored
-
-
-
-
 def join_corrected_paths(settings):
-    # Load the settings from the file
     with open(settings, "r") as file:
         settings = json.load(file)
 
     paths = settings.get('Paths', {})
     joined_paths = {}
 
     for key, path in paths.items():
         corrected_path = path.replace("/", "\\")
         more_corrected_path = corrected_path.replace("~", os.environ['USERPROFILE'])
         joined_paths[key] = more_corrected_path
-        check_dir(more_corrected_path)
+        check_dir(joined_paths)
     return joined_paths 
 def clr_get(settings):
-    settings_folder = os.path.join(os.environ['USERPROFILE'], 'Documents', 'WindowsPowerShell', 'Scripts', 'slib_sorter')
-    settings = os.path.join(settings_folder, "settings.json")
     with open(settings, "r") as file:
         settings = json.load(file)
     clors = settings.get('Colors', {})
     parsed_clors = {}
     for key, value in clors.items():
         parsed_clors[key] = value
     return parsed_clors
@@ -149,17 +142,18 @@
     with open(file_path, 'a') as file:
         if isinstance(temp_content, dict):
             json.dump(temp_content, file)
         else:
             file.write(temp_content)
     return file_path
 current_location = path_finder(0)
+
 source_file = os.path.join(current_location, 'slib_sorter.py')
 settings_f = os.path.join(os.environ['USERPROFILE'], 'Documents', 'WindowsPowerShell', 'Scripts', 'slib_sorter', 'settings.json')
-temp_content = "\nSorted Library Location:        "+ f"{j_paths.get('Name Of Top Library Directory')}"+ "\nSettings Location:     "+ f"{settings_f}"+ "\nPyhton Script Location:    " f"{os.path.join(current_location, 'slib_sorter.py')}"+ "\nTo Be Sorted Location:    " f"{j_paths.get('To Be Processed Directory')}"+ "\nRejected Files Location:     " f"{j_paths.get('Rejected Files Directory')}"
+temp_content = "\nSorted Library Location:        "+ f"{j_paths.get('Name Of Top Library Directory')}"+ "\nSettings Location:     "+ f"{settings_f}"+ "\nPyhton Script Location:    " f"{os.path.join(current_location, 'slib_sorter.py')}"+ "\nTo Be Sorted Location:    " f"{j_paths.get('To Be Processed Directory')}"+ "\nRejected Files Location:     " f"{j_paths.get('Rejected Filetype Directory')}"
 
 
 start_time = time.time()
 
 
 
 #settings = os.path.join(path_finder(0), 'settings.json')
@@ -215,15 +209,15 @@
     "Templates": ['temp', 'Temp', 'Template']
 }
 def sort_files(file_path, pattern_lists):
     total = 0
     num_failed = 0
     num_failed2 = 0
     num_succeeded = 0
-    rejected_unsorted_path = j_paths.get('Rejected Files Directory')
+    rejected_unsorted_path = j_paths.get('Rejected Filetype Directory')
     check_dir(rejected_unsorted_path)
     audio_exts = ["wav", "mp3", "aif", "aiff", "flac", "ogg", "WAV", "m4a"]
     plugin_exts = ["vst", "aax", "dll", "vst3"]
     seperator = settings.get("Console Log Seperator")
     for root, dirs, files in os.walk(file_path):
         for filename in files:
             file_path = os.path.join(root, filename)
@@ -987,17 +981,14 @@
         log_message(f' mb ', j_clrs.get('Foreground Color 1'), False, False)
         log_message(f'or ', j_clrs.get('Foreground Color 2'), False, False)
         log_message(f'{total_size_gb:.2f}', j_clrs.get('Statistics Value Color'), False, False)
         log_message(f' gb', j_clrs.get('Foreground Color 1'), False, False)
         log_message(f'', j_clrs.get('Foreground Color 1'), False, True)
     else:
         pass
-    def remove_readonly(func, path, _):
-        os.chmod(path, stat.S_IWRITE)
-        func(path)
     shutil.rmtree(path1, onerror=remove_readonly)
     check_dir(path1)
 def print_help_message():
     parser = argparse.ArgumentParser()
     parser.add_argument("-paths", action="store_true")
     parser.add_argument("-help", action="store_true")
     parser.add_argument("-colors", action="store_true")
```

