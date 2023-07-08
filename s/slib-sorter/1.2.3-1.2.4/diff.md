# Comparing `tmp/slib-sorter-1.2.3.tar.gz` & `tmp/slib-sorter-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slib-sorter-1.2.3.tar", last modified: Sat Jul  8 04:42:27 2023, max compression
+gzip compressed data, was "slib-sorter-1.2.4.tar", last modified: Sat Jul  8 05:10:25 2023, max compression
```

## Comparing `slib-sorter-1.2.3.tar` & `slib-sorter-1.2.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-08 04:42:27.242838 slib-sorter-1.2.3/
--rw-rw-rw-   0        0        0    11558 2023-07-07 20:03:54.000000 slib-sorter-1.2.3/LICENSE
--rw-rw-rw-   0        0        0     2267 2023-07-08 04:42:27.242838 slib-sorter-1.2.3/PKG-INFO
--rw-rw-rw-   0        0        0     1783 2023-07-08 03:49:36.000000 slib-sorter-1.2.3/README.md
--rw-rw-rw-   0        0        0       42 2023-07-08 04:42:27.242838 slib-sorter-1.2.3/setup.cfg
--rw-rw-rw-   0        0        0     4382 2023-07-08 04:42:08.000000 slib-sorter-1.2.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-08 04:42:27.239820 slib-sorter-1.2.3/slib_sorter.egg-info/
--rw-rw-rw-   0        0        0     2267 2023-07-08 04:42:27.000000 slib-sorter-1.2.3/slib_sorter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      273 2023-07-08 04:42:27.000000 slib-sorter-1.2.3/slib_sorter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-08 04:42:27.000000 slib-sorter-1.2.3/slib_sorter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       57 2023-07-08 04:42:27.000000 slib-sorter-1.2.3/slib_sorter.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       17 2023-07-08 04:42:27.000000 slib-sorter-1.2.3/slib_sorter.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-07-08 04:42:27.000000 slib-sorter-1.2.3/slib_sorter.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-08 04:42:27.241823 slib-sorter-1.2.3/src/
--rw-rw-rw-   0        0        0        0 2023-06-28 15:10:46.000000 slib-sorter-1.2.3/src/__init__.py
--rw-rw-rw-   0        0        0    69292 2023-07-08 04:39:16.000000 slib-sorter-1.2.3/src/slib_sorter.py
+drwxrwxrwx   0        0        0        0 2023-07-08 05:10:25.694906 slib-sorter-1.2.4/
+-rw-rw-rw-   0        0        0    11558 2023-07-07 20:03:54.000000 slib-sorter-1.2.4/LICENSE
+-rw-rw-rw-   0        0        0     2267 2023-07-08 05:10:25.693867 slib-sorter-1.2.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1783 2023-07-08 03:49:36.000000 slib-sorter-1.2.4/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-08 05:10:25.694906 slib-sorter-1.2.4/setup.cfg
+-rw-rw-rw-   0        0        0     3000 2023-07-08 05:09:24.000000 slib-sorter-1.2.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-08 05:10:25.691884 slib-sorter-1.2.4/slib_sorter.egg-info/
+-rw-rw-rw-   0        0        0     2267 2023-07-08 05:10:25.000000 slib-sorter-1.2.4/slib_sorter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      273 2023-07-08 05:10:25.000000 slib-sorter-1.2.4/slib_sorter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-08 05:10:25.000000 slib-sorter-1.2.4/slib_sorter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       57 2023-07-08 05:10:25.000000 slib-sorter-1.2.4/slib_sorter.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       17 2023-07-08 05:10:25.000000 slib-sorter-1.2.4/slib_sorter.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-07-08 05:10:25.000000 slib-sorter-1.2.4/slib_sorter.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-08 05:10:25.692872 slib-sorter-1.2.4/src/
+-rw-rw-rw-   0        0        0        0 2023-06-28 15:10:46.000000 slib-sorter-1.2.4/src/__init__.py
+-rw-rw-rw-   0        0        0    68044 2023-07-08 05:02:00.000000 slib-sorter-1.2.4/src/slib_sorter.py
```

### Comparing `slib-sorter-1.2.3/LICENSE` & `slib-sorter-1.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `slib-sorter-1.2.3/PKG-INFO` & `slib-sorter-1.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slib-sorter
-Version: 1.2.3
+Version: 1.2.4
 Summary: A Python package for sorting Sample Libraries
 Home-page: https://github.com/nrdrch/slib-sorter
 Author: Lukas Hübinger
 Author-email: fettkindasindauchoke@gmail.com
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
```

### Comparing `slib-sorter-1.2.3/README.md` & `slib-sorter-1.2.4/README.md`

 * *Files identical despite different names*

### Comparing `slib-sorter-1.2.3/slib_sorter.egg-info/PKG-INFO` & `slib-sorter-1.2.4/slib_sorter.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slib-sorter
-Version: 1.2.3
+Version: 1.2.4
 Summary: A Python package for sorting Sample Libraries
 Home-page: https://github.com/nrdrch/slib-sorter
 Author: Lukas Hübinger
 Author-email: fettkindasindauchoke@gmail.com
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
```

### Comparing `slib-sorter-1.2.3/src/slib_sorter.py` & `slib-sorter-1.2.4/src/slib_sorter.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,58 +11,34 @@
             current_dir = os.path.dirname(current_dir)
     return current_dir
 #settings = os.path.join(path_finder(0), 'settings.json')
 def check_dir(*paths):
     for path in paths:
         if not os.path.exists(path):
             os.makedirs(path)
+        else:
+            pass
 settings_folder = os.path.join(os.environ['USERPROFILE'], 'Documents', 'WindowsPowerShell', 'Scripts', 'slib_sorter')
 settings = os.path.join(settings_folder, "settings.json")
-#def check_settings():
-#    settings_folder = os.path.join(os.environ['USERPROFILE'], 'Documents', 'WindowsPowerShell', 'Scripts', 'slib_sorter')
-#    settings_file = os.path.join(settings_folder, "settings.json")
-#
-#    
-#    if not os.path.exists(settings_folder):
-#        os.makedirs(settings_folder)
-#    with open(settings_file, 'w') as file:
-#        file.write(default_config)
+with open(settings, 'r') as file:
+    settings = json.load(file)
+
 def log_message(message, color, centered=False, newline=True):
     if centered:
         message = message.center(119)
     end = "\n" if newline else ""
     print(colored(message, color), end=end)
 def log_console(file_name, seperator, dest_path, color):
     if settings.get("Show More Console Logs", True):
         log_message(f'{file_name}', f'{color}', False, False)
         log_message(f'{seperator}', "dark_grey", False, False)
         log_message(f' {dest_path}', "white", False, True)
     else:
         pass
 
-def change_folder_icon(folder_path, icon_path):
-    if not os.path.exists(folder_path):
-        print("Folder does not exist.")
-        return
-    folder_path = os.path.abspath(folder_path)
-    try:
-        ini_path = os.path.join(folder_path, "desktop.ini")
-        with open(ini_path, "w") as ini_file:
-            ini_file.write("[.ShellClassInfo]\n")
-            ini_file.write(f"IconFile={icon_path}\n")
-            ini_file.write("IconIndex=0\n")
-        ctypes.windll.kernel32.SetFileAttributesW(ini_path, 0x2 | 0x4)
-        ctypes.windll.shell32.SHChangeNotify(0x08000000, 0x0000, None, None)
-        print("Folder icon changed successfully.")
-    except Exception as e:
-        print(f"An error occurred: {str(e)}")
-
-
-with open(settings, 'r') as file:
-    settings = json.load(file)
 
 def organize_files_by_extension(path):
     if not os.path.isdir(path):
         raise Exception("The path provided is not a directory.")
     files = [f for f in os.listdir(path) if os.path.isfile(os.path.join(path, f))]
     for file in files:
         file_name, file_extension = os.path.splitext(file)
@@ -146,22 +122,19 @@
     return file_path
 
 
 
 start_time = time.time()
 current_location = path_finder(0)
 source_file = os.path.join(current_location, 'slib_sorter.py')
-icon_path = os.path.join(path_finder(1), 'examples', 'icn.ico')
-
 settings_f = os.path.join(os.environ['USERPROFILE'], 'Documents', 'WindowsPowerShell', 'Scripts', 'slib_sorter', 'settings.json')
 settings = settings_f
 #settings = os.path.join(path_finder(0), 'settings.json')
-with open(settings, 'r') as file:
-    settings = json.load(file)
-file_path = path1 = os.path.join(os.environ['USERPROFILE'], settings.get('TBPDPath'), settings.get('To Be Processed Directory'))
+
+path1 = os.path.join(os.environ['USERPROFILE'], settings.get('TBPDPath'), settings.get('To Be Processed Directory'))
 path2 = os.path.join(os.environ['USERPROFILE'], settings.get('NOFLDPath'), settings.get("Name Of Top Library Directory"))
 folder_path = path2
 check_dir(path1, path2)
 if settings.get("Run Shell Command On Startup", True):
     CmdOnStartup = settings.get("Command On Startup")
     os.system(CmdOnStartup)
 else:
```

