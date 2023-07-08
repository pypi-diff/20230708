# Comparing `tmp/slib-sorter-1.4.0.tar.gz` & `tmp/slib-sorter-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slib-sorter-1.4.0.tar", last modified: Sat Jul  8 10:23:02 2023, max compression
+gzip compressed data, was "slib-sorter-1.4.1.tar", last modified: Sat Jul  8 10:31:14 2023, max compression
```

## Comparing `slib-sorter-1.4.0.tar` & `slib-sorter-1.4.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-08 10:23:02.649659 slib-sorter-1.4.0/
--rw-rw-rw-   0        0        0    11558 2023-07-07 20:03:54.000000 slib-sorter-1.4.0/LICENSE
--rw-rw-rw-   0        0        0     2249 2023-07-08 10:23:02.649659 slib-sorter-1.4.0/PKG-INFO
--rw-rw-rw-   0        0        0     1773 2023-07-08 06:05:27.000000 slib-sorter-1.4.0/README.md
--rw-rw-rw-   0        0        0       42 2023-07-08 10:23:02.650661 slib-sorter-1.4.0/setup.cfg
--rw-rw-rw-   0        0        0     3052 2023-07-08 10:20:14.000000 slib-sorter-1.4.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-08 10:23:02.638660 slib-sorter-1.4.0/slib_sorter.egg-info/
--rw-rw-rw-   0        0        0     2249 2023-07-08 10:23:02.000000 slib-sorter-1.4.0/slib_sorter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      273 2023-07-08 10:23:02.000000 slib-sorter-1.4.0/slib_sorter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-08 10:23:02.000000 slib-sorter-1.4.0/slib_sorter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       57 2023-07-08 10:23:02.000000 slib-sorter-1.4.0/slib_sorter.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       17 2023-07-08 10:23:02.000000 slib-sorter-1.4.0/slib_sorter.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-07-08 10:23:02.000000 slib-sorter-1.4.0/slib_sorter.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-08 10:23:02.648633 slib-sorter-1.4.0/src/
--rw-rw-rw-   0        0        0        0 2023-06-28 15:10:46.000000 slib-sorter-1.4.0/src/__init__.py
--rw-rw-rw-   0        0        0    67365 2023-07-08 10:21:46.000000 slib-sorter-1.4.0/src/slib_sorter.py
+drwxrwxrwx   0        0        0        0 2023-07-08 10:31:14.048305 slib-sorter-1.4.1/
+-rw-rw-rw-   0        0        0    11558 2023-07-07 20:03:54.000000 slib-sorter-1.4.1/LICENSE
+-rw-rw-rw-   0        0        0     2249 2023-07-08 10:31:14.048305 slib-sorter-1.4.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1773 2023-07-08 06:05:27.000000 slib-sorter-1.4.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-08 10:31:14.049306 slib-sorter-1.4.1/setup.cfg
+-rw-rw-rw-   0        0        0     3242 2023-07-08 10:30:35.000000 slib-sorter-1.4.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-08 10:31:14.045334 slib-sorter-1.4.1/slib_sorter.egg-info/
+-rw-rw-rw-   0        0        0     2249 2023-07-08 10:31:13.000000 slib-sorter-1.4.1/slib_sorter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      273 2023-07-08 10:31:13.000000 slib-sorter-1.4.1/slib_sorter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-08 10:31:13.000000 slib-sorter-1.4.1/slib_sorter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       57 2023-07-08 10:31:13.000000 slib-sorter-1.4.1/slib_sorter.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       17 2023-07-08 10:31:13.000000 slib-sorter-1.4.1/slib_sorter.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-07-08 10:31:13.000000 slib-sorter-1.4.1/slib_sorter.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-08 10:31:14.047306 slib-sorter-1.4.1/src/
+-rw-rw-rw-   0        0        0        0 2023-06-28 15:10:46.000000 slib-sorter-1.4.1/src/__init__.py
+-rw-rw-rw-   0        0        0    67316 2023-07-08 10:29:41.000000 slib-sorter-1.4.1/src/slib_sorter.py
```

### Comparing `slib-sorter-1.4.0/LICENSE` & `slib-sorter-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `slib-sorter-1.4.0/PKG-INFO` & `slib-sorter-1.4.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slib-sorter
-Version: 1.4.0
+Version: 1.4.1
 Summary: A Python package for sorting Sample Libraries
 Home-page: https://github.com/nrdrch/slib-sorter
 Author: Lukas H
 Author-email: fettkindasindauchoke@gmail.com
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
```

### Comparing `slib-sorter-1.4.0/README.md` & `slib-sorter-1.4.1/README.md`

 * *Files identical despite different names*

### Comparing `slib-sorter-1.4.0/setup.py` & `slib-sorter-1.4.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -30,37 +30,41 @@
     "Paths": {
         "To Be Processed Directory": "~/Desktop/To Be Processed",
         "Name Of Top Library Directory": "~/Desktop/Sample Library",
         "Rejected Files Directory": "~/Desktop/Rejected Files"
     },
     "Colors": {
         "Foregroud Color 1": "white",
-        "Top Title Bar Color": "dark_grey",
+        "Foregroud Color 2": "dark_grey",
+        "Top Title Bar Color": "white",
         "Prompt Color": "dark_grey",
-        "Statistics Value Color": "light_red"
+        "Statistics Value Color": "light_red",
+        "Successfully Sorted File Color": "light_green",
+        "Unsorted File Color": "light_yellow",
+        "Rejected Filetype Color": "magenta"
     },
-    "Show Top Title Bar": true,
-    "Show Statistics": true,
-    "Show More Console Logs": false,
-    "Show Seperator": true,
+    "Show More Console Logs": true,
     "Console Log Seperator": "  >>>--<>  ",
     "Top Title Bar": "<   Sample Library Sorter   >",
     "Prompt": "$ ",
     "Max files per Dir": 50,
+    "Command On Startup": "cls",
     "Run Shell Command On Startup": false,
-    "Command On Startup": "cls" 
+    "Show Top Title Bar": true,
+    "Show Statistics": true,
+    "Show Seperator": true
 }}
 ''' 
         f.write(default_config)
     else:
         pass
 
     setuptools.setup(
         name="slib-sorter",
-        version="1.4.0",
+        version="1.4.1",
         author="Lukas H",
         author_email="fettkindasindauchoke@gmail.com",
         description="A Python package for sorting Sample Libraries",
         long_description=long_description,
         long_description_content_type="text/markdown",
         url="https://github.com/nrdrch/slib-sorter",
         packages=setuptools.find_packages(),
```

### Comparing `slib-sorter-1.4.0/slib_sorter.egg-info/PKG-INFO` & `slib-sorter-1.4.1/slib_sorter.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slib-sorter
-Version: 1.4.0
+Version: 1.4.1
 Summary: A Python package for sorting Sample Libraries
 Home-page: https://github.com/nrdrch/slib-sorter
 Author: Lukas H
 Author-email: fettkindasindauchoke@gmail.com
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
```

### Comparing `slib-sorter-1.4.0/src/slib_sorter.py` & `slib-sorter-1.4.1/src/slib_sorter.py`

 * *Files 0% similar despite different names*

```diff
@@ -107,15 +107,15 @@
             remove_directory_tree(child_path)
     try:
         os.remove(path)
     except OSError as error:
         os.chmod(path, stat.S_IWRITE)
         os.remove(path)
 
-file_path = path1 = j_paths.get('To Be Processed Directory')
+path1 = j_paths.get('To Be Processed Directory')
 
 
 path2 = j_paths.get('Name Of Top Library Directory')
 
 
 def split_files_in_subdirectories(path2, max_files_per_dir=50):
     for root, dirs, files in os.walk(path2):
@@ -960,21 +960,21 @@
         log_message(bar, f'{j_clrs.get("Top Title Bar Color")}', True, True)
     else:
         pass
     
     if settings.get("Show Statistics", True):
         log_message(prompt1, f'{j_clrs.get("Prompt Color")}', False, False)
         log_message(f'sorted by name & file type:   ', f'{j_clrs.get("Foregroud Color 1")}', False, False)
-        log_message(f' {num_succeeded}', f'{j_clrs.get("Successfully Sorted File Color")}', False, False)
+        log_message(f' {num_succeeded}', f'{j_clrs.get("Successfully Sorted File Color")}')
         log_message(prompt1, f'{j_clrs.get("Prompt Color")}', False, False)
         log_message(f'sorted only by file type: ', f'{j_clrs.get("Foregroud Color 1")}', False, False)
-        log_message(f' {num_failed}', f'{j_clrs.get("Unsorted File Color")}', False, False)
+        log_message(f' {num_failed}', f'{j_clrs.get("Unsorted File Color")}')
         log_message(prompt1, f'{j_clrs.get("Prompt Color")}', False, False)
         log_message(f'rejected file types: ', f'{j_clrs.get("Foregroud Color 1")}', False, False)
-        log_message(f' {num_failed2}', f'{j_clrs.get("Rejected Filetype Color")}', False, False)
+        log_message(f' {num_failed2}', f'{j_clrs.get("Rejected Filetype Color")}')
         log_message(f'      {total}', f'{j_clrs.get("Statistics Value Color")}', False, False)
         log_message(f' files processed in ', f'{j_clrs.get("Foreground Color 2")}', False, False)
         log_message(f'{elapsed_time:.2f}', f'{j_clrs.get("Statistics Value Color")}', False, False)
         log_message(f' seconds', f'{j_clrs.get("Foreground Color 1")}', False, True)
         maxfile = settings.get('Max files per Dir')
         split_files_in_subdirectories(path2, max_files_per_dir=maxfile)
         file_count, dir_count, total_size_mb, total_size_gb = count_files_in_directory(f'{path2}')
@@ -1050,10 +1050,10 @@
         log_message('           -help  '+ f'{spacer}', f'{j_clrs.get("Foregroud Color 1")}', False, False)
         log_message('Displays Help', f'{j_clrs.get("Statistics Value Color")}', False, True)
     elif args.config:
         settingsfile = settings_f
         cmd = "Start "+ f'{settingsfile}'
         os.system(cmd)
     else:
-        sort_files(path1, pattern_lists) 
+        sort_files(f'{path1}', pattern_lists) 
 def __main__():
     print_help_message()
```

