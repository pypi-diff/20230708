# Comparing `tmp/slib-sorter-1.2.8.tar.gz` & `tmp/slib-sorter-1.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slib-sorter-1.2.8.tar", last modified: Sat Jul  8 06:12:09 2023, max compression
+gzip compressed data, was "slib-sorter-1.2.9.tar", last modified: Sat Jul  8 06:37:05 2023, max compression
```

## Comparing `slib-sorter-1.2.8.tar` & `slib-sorter-1.2.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-08 06:12:09.649531 slib-sorter-1.2.8/
--rw-rw-rw-   0        0        0    11558 2023-07-07 20:03:54.000000 slib-sorter-1.2.8/LICENSE
--rw-rw-rw-   0        0        0     2249 2023-07-08 06:12:09.649531 slib-sorter-1.2.8/PKG-INFO
--rw-rw-rw-   0        0        0     1773 2023-07-08 06:05:27.000000 slib-sorter-1.2.8/README.md
--rw-rw-rw-   0        0        0       42 2023-07-08 06:12:09.650523 slib-sorter-1.2.8/setup.cfg
--rw-rw-rw-   0        0        0     2992 2023-07-08 06:10:19.000000 slib-sorter-1.2.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-08 06:12:09.640495 slib-sorter-1.2.8/slib_sorter.egg-info/
--rw-rw-rw-   0        0        0     2249 2023-07-08 06:12:09.000000 slib-sorter-1.2.8/slib_sorter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      273 2023-07-08 06:12:09.000000 slib-sorter-1.2.8/slib_sorter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-08 06:12:09.000000 slib-sorter-1.2.8/slib_sorter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       57 2023-07-08 06:12:09.000000 slib-sorter-1.2.8/slib_sorter.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       17 2023-07-08 06:12:09.000000 slib-sorter-1.2.8/slib_sorter.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-07-08 06:12:09.000000 slib-sorter-1.2.8/slib_sorter.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-08 06:12:09.648526 slib-sorter-1.2.8/src/
--rw-rw-rw-   0        0        0        0 2023-06-28 15:10:46.000000 slib-sorter-1.2.8/src/__init__.py
--rw-rw-rw-   0        0        0    68000 2023-07-08 06:11:14.000000 slib-sorter-1.2.8/src/slib_sorter.py
+drwxrwxrwx   0        0        0        0 2023-07-08 06:37:05.969541 slib-sorter-1.2.9/
+-rw-rw-rw-   0        0        0    11558 2023-07-07 20:03:54.000000 slib-sorter-1.2.9/LICENSE
+-rw-rw-rw-   0        0        0     2249 2023-07-08 06:37:05.969541 slib-sorter-1.2.9/PKG-INFO
+-rw-rw-rw-   0        0        0     1773 2023-07-08 06:05:27.000000 slib-sorter-1.2.9/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-08 06:37:05.970518 slib-sorter-1.2.9/setup.cfg
+-rw-rw-rw-   0        0        0     2994 2023-07-08 06:27:38.000000 slib-sorter-1.2.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-08 06:37:05.960533 slib-sorter-1.2.9/slib_sorter.egg-info/
+-rw-rw-rw-   0        0        0     2249 2023-07-08 06:37:05.000000 slib-sorter-1.2.9/slib_sorter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      273 2023-07-08 06:37:05.000000 slib-sorter-1.2.9/slib_sorter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-08 06:37:05.000000 slib-sorter-1.2.9/slib_sorter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       57 2023-07-08 06:37:05.000000 slib-sorter-1.2.9/slib_sorter.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       17 2023-07-08 06:37:05.000000 slib-sorter-1.2.9/slib_sorter.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-07-08 06:37:05.000000 slib-sorter-1.2.9/slib_sorter.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-08 06:37:05.968546 slib-sorter-1.2.9/src/
+-rw-rw-rw-   0        0        0        0 2023-06-28 15:10:46.000000 slib-sorter-1.2.9/src/__init__.py
+-rw-rw-rw-   0        0        0    67792 2023-07-08 06:36:21.000000 slib-sorter-1.2.9/src/slib_sorter.py
```

### Comparing `slib-sorter-1.2.8/LICENSE` & `slib-sorter-1.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `slib-sorter-1.2.8/PKG-INFO` & `slib-sorter-1.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slib-sorter
-Version: 1.2.8
+Version: 1.2.9
 Summary: A Python package for sorting Sample Libraries
 Home-page: https://github.com/nrdrch/slib-sorter
 Author: Lukas H
 Author-email: fettkindasindauchoke@gmail.com
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
```

### Comparing `slib-sorter-1.2.8/README.md` & `slib-sorter-1.2.9/README.md`

 * *Files identical despite different names*

### Comparing `slib-sorter-1.2.8/setup.py` & `slib-sorter-1.2.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     "Prompt": "$ ",
     "Console Log Seperator": "  >>>--<>  ",
     "Show More Console Logs": false,
     "Show Seperator": true,
     "Show Statistics": true,
     "Statistics Value Color": "light_red",
     "Max files per Dir": 50,
-    "TBPDPath": "Desktop",
+    "TBPDPath": "~/Desktop",
     "To Be Processed Directory": "To Be Sorted",
     "NOFLDPath": "Desktop",
     "Name Of Top Library Directory": "Sample Library",
     "RFPath": "Desktop",
     "Rejected Files": "Rejected Files",
     "Run Shell Command On Startup": false,
     "Command On Startup": "cls" 
@@ -50,15 +50,15 @@
         with open(settings_file, 'w') as f:
             f.write(default_config)
     else:
         pass
 
     setuptools.setup(
         name="slib-sorter",
-        version="1.2.8",
+        version="1.2.9",
         author="Lukas H",
         author_email="fettkindasindauchoke@gmail.com",
         description="A Python package for sorting Sample Libraries",
         long_description=long_description,
         long_description_content_type="text/markdown",
         url="https://github.com/nrdrch/slib-sorter",
         packages=setuptools.find_packages(),
```

### Comparing `slib-sorter-1.2.8/slib_sorter.egg-info/PKG-INFO` & `slib-sorter-1.2.9/slib_sorter.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slib-sorter
-Version: 1.2.8
+Version: 1.2.9
 Summary: A Python package for sorting Sample Libraries
 Home-page: https://github.com/nrdrch/slib-sorter
 Author: Lukas H
 Author-email: fettkindasindauchoke@gmail.com
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
```

### Comparing `slib-sorter-1.2.8/src/slib_sorter.py` & `slib-sorter-1.2.9/src/slib_sorter.py`

 * *Files 0% similar despite different names*

```diff
@@ -77,15 +77,18 @@
             child_path = os.path.join(path, child_path)
             remove_directory_tree(child_path)
     try:
         os.remove(path)
     except OSError as error:
         os.chmod(path, stat.S_IWRITE)
         os.remove(path)
-file_path = path1 = os.path.join(os.path.expanduser(settings.get('TBPDPath')), settings.get('To Be Processed Directory'))
+TBPDPath = settings.get('TBPDPath')
+joined_TBPDPath_path = os.path.join(TBPDPath, settings.get('To Be Processed Directory'))
+corrected_TBPDPath_path = joined_TBPDPath_path.replace("/", "\\")
+file_path = path1 = corrected_TBPDPath_path
 path2 = os.path.join(os.environ['USERPROFILE'], settings.get('NOFLDPath'), settings.get("Name Of Top Library Directory"))
 def split_files_in_subdirectories(path2, max_files_per_dir=50):
     for root, dirs, files in os.walk(path2):
         if root == path2:
             continue
         num_files = len(files)
         dir_count = len(dirs)
@@ -125,16 +128,14 @@
 
 start_time = time.time()
 current_location = path_finder(0)
 source_file = os.path.join(current_location, 'slib_sorter.py')
 settings_f = os.path.join(os.environ['USERPROFILE'], 'Documents', 'WindowsPowerShell', 'Scripts', 'slib_sorter', 'settings.json')
 
 #settings = os.path.join(path_finder(0), 'settings.json')
-file_path = path1 = os.path.join(os.path.expanduser(settings.get('TBPDPath')), settings.get('To Be Processed Directory'))
-path2 = os.path.join(os.environ['USERPROFILE'], settings.get('NOFLDPath'), settings.get("Name Of Top Library Directory"))
 folder_path = path2
 check_dir(path1, path2)
 if settings.get("Run Shell Command On Startup", True):
     CmdOnStartup = settings.get("Command On Startup")
     os.system(CmdOnStartup)
 else:
     pass
@@ -964,15 +965,15 @@
     else:
         pass
     def remove_readonly(func, path, _):
         os.chmod(path, stat.S_IWRITE)
         func(path)
     shutil.rmtree(path1, onerror=remove_readonly)
     check_dir(path1)
-temp_content = "\nSorted Library Location:        "+ f"{os.path.join(os.environ['USERPROFILE'], settings.get('NOFLDPath'), settings.get('Name Of Top Library Directory'))}"+ "\nSettings Location:     "+ f"{os.path.join(os.environ['USERPROFILE'], 'Documents', 'WindowsPowerShell', 'Scripts', 'slib_sorter', 'settings.json')}"+ "\nPyhton Script Location:    " f"{os.path.join(current_location, 'slib_sorter.py')}"+ "\nTo Be Sorted Location:    " f"{os.path.join(os.path.expanduser(settings.get('TBPDPath')), settings.get('To Be Processed Directory'))}"+ "\nRejected Files Location:     " f"{os.path.join(os.environ['USERPROFILE'], settings.get('RFPath'), settings.get('Rejected Files'))}"
+temp_content = "\nSorted Library Location:        "+ f"{os.path.join(os.environ['USERPROFILE'], settings.get('NOFLDPath'), settings.get('Name Of Top Library Directory'))}"+ "\nSettings Location:     "+ f"{os.path.join(os.environ['USERPROFILE'], 'Documents', 'WindowsPowerShell', 'Scripts', 'slib_sorter', 'settings.json')}"+ "\nPyhton Script Location:    " f"{os.path.join(current_location, 'slib_sorter.py')}"+ "\nTo Be Sorted Location:    " f"{corrected_TBPDPath_path}"+ "\nRejected Files Location:     " f"{os.path.join(os.environ['USERPROFILE'], settings.get('RFPath'), settings.get('Rejected Files'))}"
 def print_help_message():
     parser = argparse.ArgumentParser()
     parser.add_argument("-paths", action="store_true")
     parser.add_argument("-help", action="store_true")
     parser.add_argument("-colors", action="store_true")
     parser.add_argument("-config", action="store_true")
     temp_file_path = temp_path_file(temp_content)
```

