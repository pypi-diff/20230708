# Comparing `tmp/slib-sorter-1.0.7.tar.gz` & `tmp/slib_sorter-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slib-sorter-1.0.7.tar", last modified: Tue Jun 27 14:08:07 2023, max compression
+gzip compressed data, was "slib_sorter-1.0.8.tar", last modified: Fri Jul  7 22:20:05 2023, max compression
```

## Comparing `slib-sorter-1.0.7.tar` & `slib_sorter-1.0.8.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-06-27 14:08:07.785281 slib-sorter-1.0.7/
--rw-rw-rw-   0        0        0    11558 2023-06-27 12:38:43.000000 slib-sorter-1.0.7/LICENSE
--rw-rw-rw-   0        0        0      262 2023-06-27 14:08:07.785281 slib-sorter-1.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     1876 2023-06-27 12:38:43.000000 slib-sorter-1.0.7/README.md
--rw-rw-rw-   0        0        0       42 2023-06-27 14:08:07.785281 slib-sorter-1.0.7/setup.cfg
--rw-rw-rw-   0        0        0      515 2023-06-27 14:00:27.000000 slib-sorter-1.0.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-27 14:08:07.782260 slib-sorter-1.0.7/slib_sorter.egg-info/
--rw-rw-rw-   0        0        0      262 2023-06-27 14:08:07.000000 slib-sorter-1.0.7/slib_sorter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      297 2023-06-27 14:08:07.000000 slib-sorter-1.0.7/slib_sorter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-27 14:08:07.000000 slib-sorter-1.0.7/slib_sorter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       56 2023-06-27 14:08:07.000000 slib-sorter-1.0.7/slib_sorter.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       10 2023-06-27 14:08:07.000000 slib-sorter-1.0.7/slib_sorter.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-06-27 14:08:07.000000 slib-sorter-1.0.7/slib_sorter.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-27 14:08:07.784283 slib-sorter-1.0.7/src/
--rw-rw-rw-   0        0        0      151 2023-06-27 13:51:07.000000 slib-sorter-1.0.7/src/__init__.py
--rw-rw-rw-   0        0        0    63494 2023-06-27 13:44:51.000000 slib-sorter-1.0.7/src/__main__.py
--rw-rw-rw-   0        0        0     7179 2023-06-27 12:38:43.000000 slib-sorter-1.0.7/src/filesorterfunctions.py
+drwxrwxrwx   0        0        0        0 2023-07-07 22:20:05.377344 slib_sorter-1.0.8/
+-rw-rw-rw-   0        0        0    11558 2023-07-07 20:03:54.000000 slib_sorter-1.0.8/LICENSE
+-rw-rw-rw-   0        0        0     2291 2023-07-07 22:20:05.376344 slib_sorter-1.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     1807 2023-07-07 20:03:54.000000 slib_sorter-1.0.8/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-07 22:20:05.377344 slib_sorter-1.0.8/setup.cfg
+-rw-rw-rw-   0        0        0     2078 2023-07-07 22:12:23.000000 slib_sorter-1.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-07 22:20:05.372341 slib_sorter-1.0.8/slib_sorter.egg-info/
+-rw-rw-rw-   0        0        0     2291 2023-07-07 22:20:05.000000 slib_sorter-1.0.8/slib_sorter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      316 2023-07-07 22:20:05.000000 slib_sorter-1.0.8/slib_sorter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-07 22:20:05.000000 slib_sorter-1.0.8/slib_sorter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       98 2023-07-07 22:20:05.000000 slib_sorter-1.0.8/slib_sorter.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       17 2023-07-07 22:20:05.000000 slib_sorter-1.0.8/slib_sorter.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-07-07 22:20:05.000000 slib_sorter-1.0.8/slib_sorter.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-07 22:20:05.375364 slib_sorter-1.0.8/src/
+-rw-rw-rw-   0        0        0        0 2023-06-28 15:10:46.000000 slib_sorter-1.0.8/src/__init__.py
+-rw-rw-rw-   0        0        0      825 2023-07-07 21:32:50.000000 slib_sorter-1.0.8/src/__main__.py
+-rw-rw-rw-   0        0        0     7063 2023-07-07 21:31:37.000000 slib_sorter-1.0.8/src/filesorterfunctions.py
+-rw-rw-rw-   0        0        0    63523 2023-07-07 20:37:42.000000 slib_sorter-1.0.8/src/slib_sorter.py
```

### Comparing `slib-sorter-1.0.7/LICENSE` & `slib_sorter-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `slib-sorter-1.0.7/README.md` & `slib_sorter-1.0.8/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -13,34 +13,35 @@
 git clone https://github.com/nrdrch/slib-sorter.git; python3 .\slib-sorter\src\slib-sorter.py
 ```
 
 ### Usage 
 1. Restart your PowerShell.
 2. Run:
 ```
-Start-Sorter -help
+Start-Sorter
 ```
-<img src="https://raw.githubusercontent.com/nrdrch/slib-sorter/main/examples/outputstatistics.png">
+
 
 > If its the first time running this, it will now have created two directories on your desktop. 
 
 
 
 <img src="https://raw.githubusercontent.com/nrdrch/slib-sorter/main/examples/direxample.png?token=GHSAT0AAAAAACCUPKWOJF3EUJNKTAR7NJSSZEUEOLA">
 <img examples/direxample.png>
 
 
+<img src="https://raw.githubusercontent.com/nrdrch/slib-sorter/main/examples/outputstatistics.png">
 
 #### Note: Among other things, the names of these two directories & the name of the finished library can be changed in the settings file. 
 ```
 $home\Documents\slib-sorter\settings.json
 ```
-
-
-<img src="https://raw.githubusercontent.com/nrdrch/slib-sorter/main/examples/settings.png">
+```
+Start-Sorter -config
+```
 
 
 2. Move all your files into the 'To Be Sorted' directory
 3. Run the same command again and wait for the process to be completed 
 4. Inspect the newly created Sample Library located under 'Documents\Sample Library' folder.
```

### Comparing `slib-sorter-1.0.7/src/__main__.py` & `slib_sorter-1.0.8/src/slib_sorter.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os, shutil, stat, argparse
 import filesorterfunctions as fsf
 import time
 import json
 start_time = time.time()
 current_location = fsf.path_finder(0)
-source_file = os.path.join(current_location, 'slib-sorter.py')
+source_file = os.path.join(current_location, 'slib_sorter.py')
 fsf.ps_script(source_file)
 icon_path = os.path.join(fsf.path_finder(1), 'examples', 'icn.ico')
 settings = os.path.join(fsf.path_finder(1), 'settings.json')
 with open(settings, 'r') as file:
     settings = json.load(file)
 file_path = path1 = os.path.join(os.environ['USERPROFILE'], settings.get('TBPDPath'), settings.get('To Be Processed Directory'))
 path2 = os.path.join(os.environ['USERPROFILE'], settings.get('NOFLDPath'), settings.get("Name Of Top Library Directory"))
@@ -65,15 +65,15 @@
 }
 def sort_files(file_path, pattern_lists):
     total = 0
     num_failed = 0
     num_failed2 = 0
     num_succeeded = 0
     rejected_unsorted_path = os.path.join(os.environ['USERPROFILE'], settings.get('RFPath'), settings.get("Rejected Files"))
-    fsf.check_if(rejected_unsorted_path)
+    fsf.check_dir(rejected_unsorted_path)
     audio_exts = ["wav", "mp3", "aif", "aiff", "flac", "ogg", "WAV", "m4a"]
     plugin_exts = ["vst", "aax", "dll", "vst3"]
     seperator = settings.get("Console Log Seperator")
     for root, dirs, files in os.walk(file_path):
         for filename in files:
             file_path = os.path.join(root, filename)
             file_name, file_extension = os.path.splitext(filename)
@@ -797,20 +797,20 @@
                 pass
     elapsed_time = time.time() - start_time
     prompt1 = settings.get("Prompt")
     def remove_readonly(func, path, _):
         os.chmod(path, stat.S_IWRITE)
         func(path)
     shutil.rmtree(path1, onerror=remove_readonly)
-    fsf.check_if(path1)
+    fsf.check_dir(path1)
     def remove_readonly(func, path, _):
         os.chmod(path, stat.S_IWRITE)
         func(path)
     shutil.rmtree(path1, onerror=remove_readonly)
-    fsf.check_if(path1)
+    fsf.check_dir(path1)
     if settings.get("Show Top Bar", True):
         bar = settings.get("Top Bar")
         fsf.log_message(bar, f'{settings.get("Top Bar Color")}', True, True)
     else:
         pass
     if settings.get("Show Statistics", True):
         fsf.log_message(prompt1, f'{settings.get("Prompt Color")}', False, False)
@@ -845,17 +845,15 @@
     else:
         pass
     def remove_readonly(func, path, _):
         os.chmod(path, stat.S_IWRITE)
         func(path)
     shutil.rmtree(path1, onerror=remove_readonly)
     fsf.check_dir(path1)
-
-sort_files(path1, pattern_lists)
-temp_content = "\nSorted Library Location:        "+ f"{os.path.join(os.environ['USERPROFILE'], settings.get('NOFLDPath'), settings.get('Name Of Top Library Directory'))}"+ "\nSettings Location:     "+ f"{os.path.join(fsf.path_finder(1), 'settings.json')}"+ "\nPyhton Script Location:    " f"{os.path.join(current_location, 'slib-sorter.py')}"+ "\nTo Be Sorted Location:    " f"{os.path.join(os.environ['USERPROFILE'], settings.get('TBPDPath'), settings.get('To Be Processed Directory'))}"+ "\nRejected Files Location:     " f"{os.path.join(os.environ['USERPROFILE'], settings.get('RFPath'), settings.get('Rejected Files'))}"
+temp_content = "\nSorted Library Location:        "+ f"{os.path.join(os.environ['USERPROFILE'], settings.get('NOFLDPath'), settings.get('Name Of Top Library Directory'))}"+ "\nSettings Location:     "+ f"{os.path.join(fsf.path_finder(1), 'settings.json')}"+ "\nPyhton Script Location:    " f"{os.path.join(current_location, 'slib_sorter.py')}"+ "\nTo Be Sorted Location:    " f"{os.path.join(os.environ['USERPROFILE'], settings.get('TBPDPath'), settings.get('To Be Processed Directory'))}"+ "\nRejected Files Location:     " f"{os.path.join(os.environ['USERPROFILE'], settings.get('RFPath'), settings.get('Rejected Files'))}"
 def print_help_message():
     parser = argparse.ArgumentParser()
     parser.add_argument("-paths", action="store_true")
     parser.add_argument("-help", action="store_true")
     parser.add_argument("-colors", action="store_true")
     parser.add_argument("-config", action="store_true")
     temp_file_path = fsf.temp_path_file(temp_content)
@@ -895,9 +893,11 @@
         fsf.log_message('           -help  '+ f'{spacer}', f'{settings.get("Foregroud Color 1")}', False, False)
         fsf.log_message('Displays Help', f'{settings.get("Statistics Value Color")}', False, True)
     elif args.config:
         settingsfile = os.path.join(fsf.path_finder(1), 'settings.json')
         cmd = "Start "+ settingsfile
         os.system(cmd)
     else:
-        pass
-print_help_message()
+        sort_files(path1, pattern_lists) 
+def __main__():
+    print_help_message()
+__main__()
```

### Comparing `slib-sorter-1.0.7/src/filesorterfunctions.py` & `slib_sorter-1.0.8/src/filesorterfunctions.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,24 +21,20 @@
 def log_console(file_name, seperator, dest_path, color):
     if settings.get("Show More Console Logs", True):
         log_message(f'{file_name}', f'{color}', False, False)
         log_message(f'{seperator}', "dark_grey", False, False)
         log_message(f' {dest_path}', "white", False, True)
     else:
         pass
-def check_if(*paths):
-    for path in paths:
-        if not os.path.exists(path):
-            os.makedirs(path)
 def ps_script(source_file):
     winpro = os.path.join(os.environ['USERPROFILE'],'Documents', 'WindowsPowerShell')
     powershell_scripts_folder = os.path.join(winpro, 'Scripts')
     if not os.path.exists(powershell_scripts_folder):
         os.makedirs(powershell_scripts_folder)
-    powershell_script_file = os.path.join(powershell_scripts_folder, 'slib-sorter' + ".psm1")
+    powershell_script_file = os.path.join(powershell_scripts_folder, 'slib_sorter' + ".psm1")
     script_content = f'''
     function Start-Sorter {{
         [CmdletBinding()]
         param(
             [Parameter(ValueFromRemainingArguments=$true)]
             [string]$CustomInput
         )
```

