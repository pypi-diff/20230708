# Comparing `tmp/slib-sorter-1.1.1.tar.gz` & `tmp/slib-sorter-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\slib-sorter-1.1.1.tar", last modified: Sat Jul  8 02:05:20 2023, max compression
+gzip compressed data, was "slib-sorter-1.1.2.tar", last modified: Sat Jul  8 02:27:10 2023, max compression
```

## Comparing `slib-sorter-1.1.1.tar` & `slib-sorter-1.1.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-07-08 02:05:20.000000 slib-sorter-1.1.1/
--rw-rw-rw-   0        0        0    11558 2023-07-07 20:03:54.000000 slib-sorter-1.1.1/LICENSE
--rw-rw-rw-   0        0        0     2289 2023-07-08 02:05:20.000000 slib-sorter-1.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     1807 2023-07-07 20:03:54.000000 slib-sorter-1.1.1/README.md
--rw-rw-rw-   0        0        0       42 2023-07-08 02:05:20.000000 slib-sorter-1.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1412 2023-07-08 02:04:18.000000 slib-sorter-1.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-08 02:05:20.000000 slib-sorter-1.1.1/slib_sorter.egg-info/
--rw-rw-rw-   0        0        0     2289 2023-07-08 02:05:20.000000 slib-sorter-1.1.1/slib_sorter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      300 2023-07-08 02:05:20.000000 slib-sorter-1.1.1/slib_sorter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-08 02:05:20.000000 slib-sorter-1.1.1/slib_sorter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       57 2023-07-08 02:05:20.000000 slib-sorter-1.1.1/slib_sorter.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       17 2023-07-08 02:05:20.000000 slib-sorter-1.1.1/slib_sorter.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-07-08 02:05:20.000000 slib-sorter-1.1.1/slib_sorter.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-08 02:05:20.000000 slib-sorter-1.1.1/src/
--rw-rw-rw-   0        0        0        0 2023-06-28 15:10:46.000000 slib-sorter-1.1.1/src/__init__.py
--rw-rw-rw-   0        0        0     9364 2023-07-08 01:47:57.000000 slib-sorter-1.1.1/src/filesorterfunctions.py
--rw-rw-rw-   0        0        0    63702 2023-07-08 01:08:16.000000 slib-sorter-1.1.1/src/slib_sorter.py
+drwxrwxrwx   0        0        0        0 2023-07-08 02:27:10.145461 slib-sorter-1.1.2/
+-rw-rw-rw-   0        0        0    11558 2023-07-07 20:03:54.000000 slib-sorter-1.1.2/LICENSE
+-rw-rw-rw-   0        0        0     2289 2023-07-08 02:27:10.145461 slib-sorter-1.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1807 2023-07-07 20:03:54.000000 slib-sorter-1.1.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-08 02:27:10.145461 slib-sorter-1.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1412 2023-07-08 02:27:00.000000 slib-sorter-1.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-08 02:27:10.142428 slib-sorter-1.1.2/slib_sorter.egg-info/
+-rw-rw-rw-   0        0        0     2289 2023-07-08 02:27:10.000000 slib-sorter-1.1.2/slib_sorter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      300 2023-07-08 02:27:10.000000 slib-sorter-1.1.2/slib_sorter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-08 02:27:10.000000 slib-sorter-1.1.2/slib_sorter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       57 2023-07-08 02:27:10.000000 slib-sorter-1.1.2/slib_sorter.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       17 2023-07-08 02:27:10.000000 slib-sorter-1.1.2/slib_sorter.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-07-08 02:27:10.000000 slib-sorter-1.1.2/slib_sorter.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-08 02:27:10.144428 slib-sorter-1.1.2/src/
+-rw-rw-rw-   0        0        0        0 2023-06-28 15:10:46.000000 slib-sorter-1.1.2/src/__init__.py
+-rw-rw-rw-   0        0        0     9364 2023-07-08 01:47:57.000000 slib-sorter-1.1.2/src/filesorterfunctions.py
+-rw-rw-rw-   0        0        0    72457 2023-07-08 02:20:39.000000 slib-sorter-1.1.2/src/slib_sorter.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `slib-sorter-1.1.1/LICENSE` & `slib-sorter-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `slib-sorter-1.1.1/PKG-INFO` & `slib-sorter-1.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slib-sorter
-Version: 1.1.1
+Version: 1.1.2
 Summary: A Python library for sorting Sample Libraries
 Home-page: https://github.com/nrdrch/slib-sorter
 Author: Lukas Hübinger
 Author-email: fettkindasindauchoke@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
```

### Comparing `slib-sorter-1.1.1/README.md` & `slib-sorter-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `slib-sorter-1.1.1/setup.py` & `slib-sorter-1.1.2/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 def install():
     with open("README.md", "r", encoding="utf-8") as fh:
         long_description = fh.read()
 
     setuptools.setup(
         name="slib-sorter",
-        version="1.1.1",
+        version="1.1.2",
         author="Lukas Hübinger",
         author_email="fettkindasindauchoke@gmail.com",
         description="A Python library for sorting Sample Libraries",
         long_description=long_description,
         long_description_content_type="text/markdown",
         url="https://github.com/nrdrch/slib-sorter",
         packages=setuptools.find_packages(),
```

### Comparing `slib-sorter-1.1.1/slib_sorter.egg-info/PKG-INFO` & `slib-sorter-1.1.2/slib_sorter.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slib-sorter
-Version: 1.1.1
+Version: 1.1.2
 Summary: A Python library for sorting Sample Libraries
 Home-page: https://github.com/nrdrch/slib-sorter
 Author: Lukas Hübinger
 Author-email: fettkindasindauchoke@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
```

### Comparing `slib-sorter-1.1.1/src/filesorterfunctions.py` & `slib-sorter-1.1.2/src/filesorterfunctions.py`

 * *Files identical despite different names*

### Comparing `slib-sorter-1.1.1/src/slib_sorter.py` & `slib-sorter-1.1.2/src/slib_sorter.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,25 +1,253 @@
 import os, shutil, stat, argparse
-import filesorterfunctions as fsf
+
 import time
 import json
+
+import os, shutil, stat, tempfile, json, ctypes, importlib
+from termcolor import colored
+
+def path_finder(levels_up=0):
+    current_dir = os.path.abspath(os.path.dirname(__file__))
+    if levels_up > 0:
+        for _ in range(levels_up):
+            current_dir = os.path.dirname(current_dir)
+    return current_dir
+#settings = os.path.join(path_finder(0), 'settings.json')
+def check_dir(*paths):
+    for path in paths:
+        if not os.path.exists(path):
+            os.makedirs(path)
+settings_folder = os.path.join(os.environ['USERPROFILE'], 'Documents', 'WindowsPowerShell', 'Scripts', 'slib_sorter')
+settings = os.path.join(settings_folder, "settings.json")
+#def check_settings():
+#    settings_folder = os.path.join(os.environ['USERPROFILE'], 'Documents', 'WindowsPowerShell', 'Scripts', 'slib_sorter')
+#    settings_file = os.path.join(settings_folder, "settings.json")
+#
+#    
+#    if not os.path.exists(settings_folder):
+#        os.makedirs(settings_folder)
+#    with open(settings_file, 'w') as file:
+#        file.write(default_config)
+
+
+def log_message(message, color, centered=False, newline=True):
+    if centered:
+        message = message.center(119)
+    end = "\n" if newline else ""
+    print(colored(message, color), end=end)
+def log_console(file_name, seperator, dest_path, color):
+    if settings.get("Show More Console Logs", True):
+        log_message(f'{file_name}', f'{color}', False, False)
+        log_message(f'{seperator}', "dark_grey", False, False)
+        log_message(f' {dest_path}', "white", False, True)
+    else:
+        pass
+def ps_script(source_file):
+    winpro = os.path.join(os.environ['USERPROFILE'],'Documents', 'WindowsPowerShell')
+    powershell_scripts_folder = os.path.join(winpro, 'Scripts', 'slib_sorter')
+    if not os.path.exists(powershell_scripts_folder):
+        os.makedirs(powershell_scripts_folder)
+    powershell_script_file = os.path.join(powershell_scripts_folder, 'slib_sorter' + ".psm1")
+    settings_file = os.path.join(powershell_scripts_folder, 'settings.json')
+    script_content = f'''
+function Start-Sorter {{
+    [CmdletBinding()]
+    param(
+        [Parameter(ValueFromRemainingArguments=$true)]
+        [string]$CustomInput
+    )
+    $argsString = $CustomInput -join "' '"
+    $pythonScript = '{source_file}'
+    python3 $pythonScript $argsString
+}}
+    '''
+    with open(powershell_script_file, 'a') as f:
+        f.write(script_content)
+    
+    if not os.path.exists(settings_folder):
+        os.makedirs(settings_folder)
+    default_config = f'''
+{{
+    "Foregroud Color 1": "white",
+    "Top Bar Color": "dark_grey",
+    "Show Top Bar": true,
+    "Top Bar": "<   Sample Library Sorter   >",
+    "Prompt Color": "dark_grey",
+    "Prompt": "$ ",
+    "Console Log Seperator": "  >>>--<>  ",
+    "Show More Console Logs": false,
+    "Show Seperator": true,
+    "Show Statistics": true,
+    "Statistics Value Color": "light_red",
+    "Max files per Dir": 50,
+    "TBPDPath": "Desktop",
+    "To Be Processed Directory": "To Be Sorted",
+    "NOFLDPath": "Desktop",
+    "Name Of Top Library Directory": "Sample Library",
+    "RFPath": "Desktop",
+    "Rejected Files": "Rejected Files",
+    "Run Shell Command On Startup": false,
+    "Command On Startup": "cls" 
+}}
+    '''
+    with open(settings_file, 'w') as f:
+        f.write(default_config)
+    with open(settings_file, 'r') as file:
+        settings_file = json.load(file)
+    profile_path = os.path.expanduser("~/Documents/WindowsPowerShell/Microsoft.PowerShell_profile.ps1")
+    with open(profile_path, 'r') as f:
+        profile_content = f.read()
+        if f"Import-Module -DisableNameChecking \"{powershell_script_file}\"" in profile_content:
+            pass
+        else:
+            with open(profile_path, 'a') as f:
+                f.write(f"\nImport-Module -DisableNameChecking \"{powershell_script_file}\"")
+    try:
+        if settings.get("Run Shell Command On Startup", True):
+            CmdOnStartup = settings.get("Command On Startup")
+            os.system(CmdOnStartup)
+        else:
+            pass
+    except:
+        winpro = os.path.join(os.environ['USERPROFILE'],'Documents', 'WindowsPowerShell')
+        powershell_scripts_folder = os.path.join(winpro, 'Scripts', 'slib_sorter')
+        settings_file = os.path.join(powershell_scripts_folder, 'settings.json')
+        importlib.reload(settings_file)
+        #setupfile = os.path.join(path_finder(0), 'setup.py')
+        importlib.reload(settings_file)
+def change_folder_icon(folder_path, icon_path):
+    if not os.path.exists(folder_path):
+        print("Folder does not exist.")
+        return
+    folder_path = os.path.abspath(folder_path)
+    try:
+        ini_path = os.path.join(folder_path, "desktop.ini")
+        with open(ini_path, "w") as ini_file:
+            ini_file.write("[.ShellClassInfo]\n")
+            ini_file.write(f"IconFile={icon_path}\n")
+            ini_file.write("IconIndex=0\n")
+        ctypes.windll.kernel32.SetFileAttributesW(ini_path, 0x2 | 0x4)
+        ctypes.windll.shell32.SHChangeNotify(0x08000000, 0x0000, None, None)
+        print("Folder icon changed successfully.")
+    except Exception as e:
+        print(f"An error occurred: {str(e)}")
+
+if not os.path.exists(settings):
+    current_location = path_finder(0)
+    source_file = os.path.join(current_location, 'slib_sorter.py')
+    ps_script(source_file)
+
+else:
+    with open(settings, 'r') as file:
+        settings = json.load(file)
+
+def organize_files_by_extension(path):
+    if not os.path.isdir(path):
+        raise Exception("The path provided is not a directory.")
+    files = [f for f in os.listdir(path) if os.path.isfile(os.path.join(path, f))]
+    for file in files:
+        file_name, file_extension = os.path.splitext(file)
+        if file_extension:
+            subfolder_name = file_extension.lstrip(".")
+        else:
+            subfolder_name = "typeless"
+        subfolder_path = os.path.join(path, subfolder_name)
+        if not os.path.exists(subfolder_path):
+            os.makedirs(subfolder_path)
+        file_path = os.path.join(path, file)
+        shutil.move(file_path, os.path.join(subfolder_path, file))
+def remove_empty_lines(file_path):
+    with open(file_path, 'r') as file:
+        lines = file.readlines()
+    lines = [line for line in lines if line.strip() != '']
+    with open(file_path, 'w') as file:
+        file.writelines(lines)
+    return len(lines)
+def count_files_in_directory(path):
+    file_count = 0
+    dir_count = 0
+    total_size = 0
+    for root, dirs, files in os.walk(path):
+        file_count += len(files)
+        dir_count += len(dirs)
+        for file in files:
+            file_path = os.path.join(root, file)
+            total_size += os.path.getsize(file_path)
+    total_size_mb = total_size / (1024 * 1024)
+    total_size_gb = total_size_mb / 1024
+    return file_count, dir_count, total_size_mb, total_size_gb
+def remove_directory_tree(path):
+    if os.path.isdir(path):
+        for child_path in os.listdir(path):
+            child_path = os.path.join(path, child_path)
+            remove_directory_tree(child_path)
+    try:
+        os.remove(path)
+    except OSError as error:
+        os.chmod(path, stat.S_IWRITE)
+        os.remove(path)
+file_path = path1 = os.path.join(os.environ['USERPROFILE'], settings.get('TBPDPath'), settings.get('To Be Processed Directory'))
+path2 = os.path.join(os.environ['USERPROFILE'], settings.get('NOFLDPath'), settings.get("Name Of Top Library Directory"))
+def split_files_in_subdirectories(path2, max_files_per_dir=50):
+    for root, dirs, files in os.walk(path2):
+        if root == path2:
+            continue
+        num_files = len(files)
+        dir_count = len(dirs)
+        if num_files > max_files_per_dir:
+            dir_count = num_files // max_files_per_dir
+            if num_files % max_files_per_dir != 0:
+                dir_count += 1
+            for i in range(dir_count):
+                start_index = i * max_files_per_dir
+                end_index = min((i + 1) * max_files_per_dir, num_files)
+                new_dir_name = f"{start_index}-{end_index-1}"
+                new_dir_path = os.path.join(root, new_dir_name)
+                try:
+                    os.mkdir(new_dir_path)
+                except FileExistsError:
+                    print()
+            for i, file_name in enumerate(files):
+                old_file_path = os.path.join(root, file_name)
+                new_dir_index = i // max_files_per_dir
+                start_index = new_dir_index * max_files_per_dir
+                end_index = min((new_dir_index + 1) * max_files_per_dir, num_files)
+                new_dir_name = f"{start_index}-{end_index-1}"
+                new_dir_path = os.path.join(root, new_dir_name)
+                new_file_path = os.path.join(new_dir_path, file_name)
+                shutil.move(old_file_path, new_file_path)
+def temp_path_file(temp_content):
+    temp_dir = tempfile.gettempdir()
+    file_path = tempfile.mktemp(dir=temp_dir)
+    with open(file_path, 'a') as file:
+        if isinstance(temp_content, dict):
+            json.dump(temp_content, file)
+        else:
+            file.write(temp_content)
+    return file_path
+
+
+
+
+
 start_time = time.time()
-current_location = fsf.path_finder(0)
+current_location = path_finder(0)
 source_file = os.path.join(current_location, 'slib_sorter.py')
-fsf.ps_script(source_file)
-icon_path = os.path.join(fsf.path_finder(1), 'examples', 'icn.ico')
+ps_script(source_file)
+icon_path = os.path.join(path_finder(1), 'examples', 'icn.ico')
 settings_folder = os.path.join(os.environ['USERPROFILE'], 'Documents', 'WindowsPowerShell', 'Scripts', 'slib_sorter')
 settings = os.path.join(settings_folder, "settings.json")
-#settings = os.path.join(fsf.path_finder(0), 'settings.json')
+#settings = os.path.join(path_finder(0), 'settings.json')
 with open(settings, 'r') as file:
     settings = json.load(file)
 file_path = path1 = os.path.join(os.environ['USERPROFILE'], settings.get('TBPDPath'), settings.get('To Be Processed Directory'))
 path2 = os.path.join(os.environ['USERPROFILE'], settings.get('NOFLDPath'), settings.get("Name Of Top Library Directory"))
 folder_path = path2
-fsf.check_dir(path1, path2)
+check_dir(path1, path2)
 if settings.get("Run Shell Command On Startup", True):
     CmdOnStartup = settings.get("Command On Startup")
     os.system(CmdOnStartup)
 else:
     pass
 pattern_lists = {
     "Bass": ['bass', 'BS', 'BASS', 'Bass', 'sub', 'contrabass', 'BA', 'BS', 'Growl', 'GROWL', 'growl'],
@@ -67,839 +295,839 @@
 }
 def sort_files(file_path, pattern_lists):
     total = 0
     num_failed = 0
     num_failed2 = 0
     num_succeeded = 0
     rejected_unsorted_path = os.path.join(os.environ['USERPROFILE'], settings.get('RFPath'), settings.get("Rejected Files"))
-    fsf.check_dir(rejected_unsorted_path)
+    check_dir(rejected_unsorted_path)
     audio_exts = ["wav", "mp3", "aif", "aiff", "flac", "ogg", "WAV", "m4a"]
     plugin_exts = ["vst", "aax", "dll", "vst3"]
     seperator = settings.get("Console Log Seperator")
     for root, dirs, files in os.walk(file_path):
         for filename in files:
             file_path = os.path.join(root, filename)
             file_name, file_extension = os.path.splitext(filename)
             file_extension = file_extension[1:]
             if file_extension in audio_exts:
                 if any(pattern in file_name for pattern in pattern_lists.get("DrumPercs", [])):
                     total += 1
                     num_succeeded += 1
                     dest_path = os.path.join(os.environ['USERPROFILE'], settings.get('NOFLDPath'), settings.get("Name Of Top Library Directory"), 'Samples', 'Drum', 'Percussion')
                     if settings.get("Show More Console Logs", True):
-                        fsf.log_console(f'{file_name}', f'{seperator}', f'{dest_path}', "green")
+                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', "green")
                     else:
                         pass
                 elif any(pattern in file_name for pattern in pattern_lists.get("DrumLoops", [])):
                     total += 1
                     num_succeeded += 1
                     dest_path = os.path.join(os.environ['USERPROFILE'], settings.get('NOFLDPath'), settings.get("Name Of Top Library Directory"), 'Samples', 'Drum', 'Loops')
                     if settings.get("Show More Console Logs", True):
-                        fsf.log_console(f'{file_name}', f'{seperator}', f'{dest_path}', "green")
+                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', "green")
                     else:
                         pass
                 elif any(pattern in file_name for pattern in pattern_lists.get("VocalLoops", [])):
                     total += 1
                     num_succeeded += 1
                     dest_path = os.path.join(os.environ['USERPROFILE'], settings.get('NOFLDPath'), settings.get("Name Of Top Library Directory"), 'Samples', 'Voice', 'Loops')
                     if settings.get("Show More Console Logs", True):
-                        fsf.log_console(f'{file_name}', f'{seperator}', f'{dest_path}', "green")
+                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', "green")
                     else:
                         pass
                 elif any(pattern in file_name for pattern in pattern_lists.get("MelodicLoops", [])):
                     total += 1
                     num_succeeded += 1
                     dest_path = os.path.join(os.environ['USERPROFILE'], settings.get('NOFLDPath'), settings.get("Name Of Top Library Directory"), 'Samples', 'Melodic', 'Loops')
                     if settings.get("Show More Console Logs", True):
-                        fsf.log_console(f'{file_name}', f'{seperator}', f'{dest_path}', "green")
+                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', "green")
                     else:
                         pass
                 elif any(pattern in file_name for pattern in pattern_lists.get("BassLoops", [])):
                     total += 1
                     num_succeeded += 1
                     dest_path = os.path.join(os.environ['USERPROFILE'], settings.get('NOFLDPath'), settings.get("Name Of Top Library Directory"), 'Samples', 'Melodic', 'Bass', 'Loops')
                     if settings.get("Show More Console Logs", True):
-                        fsf.log_console(f'{file_name}', f'{seperator}', f'{dest_path}', "green")
+                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', "green")
                     else:
                         pass
                 elif any(pattern in file_name for pattern in pattern_lists.get("DrumKick", [])):
                     total += 1
                     num_succeeded += 1
                     dest_path = os.path.join(os.environ['USERPROFILE'], settings.get('NOFLDPath'), settings.get("Name Of Top Library Directory"), 'Samples', 'Drum', 'Kicks')
                     if settings.get("Show More Console Logs", True):
-                        fsf.log_console(f'{file_name}', f'{seperator}', f'{dest_path}', "green")
+                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', "green")
                     else:
                         pass
                 elif any(pattern in file_name for pattern in pattern_lists.get("DrumSnare", [])):
                     total += 1
                     num_succeeded += 1
                     dest_path = os.path.join(os.environ['USERPROFILE'], settings.get('NOFLDPath'), settings.get("Name Of Top Library Directory"), 'Samples', 'Drum', 'Snares')
                     if settings.get("Show More Console Logs", True):
-                        fsf.log_console(f'{file_name}', f'{seperator}', f'{dest_path}', "green")
+                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', "green")
                     else:
                         pass
                 elif any(pattern in file_name for pattern in pattern_lists.get("DrumShakers", [])):
                     total += 1
                     num_succeeded += 1
                     dest_path = os.path.join(os.environ['USERPROFILE'], settings.get('NOFLDPath'), settings.get("Name Of Top Library Directory"), 'Samples', 'Drum', 'Shakers')
                     if settings.get("Show More Console Logs", True):
-                        fsf.log_console(f'{file_name}', f'{seperator}', f'{dest_path}', "green")
+                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', "green")
                     else:
                         pass
                 elif any(pattern in file_name for pattern in pattern_lists.get("Synth", [])):
                     total += 1
                     num_succeeded += 1
                     dest_path = os.path.join(os.environ['USERPROFILE'], settings.get('NOFLDPath'), settings.get("Name Of Top Library Directory"), 'Samples', 'Melodic', 'Synths')
                     if settings.get("Show More Console Logs", True):
-                        fsf.log_console(f'{file_name}', f'{seperator}', f'{dest_path}', "green")
+                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', "green")
                     else:
                         pass
                 elif any(pattern in file_name for pattern in pattern_lists.get("Plucks", [])):
                     total += 1
                     num_succeeded += 1
                     dest_path = os.path.join(os.environ['USERPROFILE'], settings.get('NOFLDPath'), settings.get("Name Of Top Library Directory"), 'Samples', 'Melodic', 'Plucks')
                     if settings.get("Show More Console Logs", True):
-                        fsf.log_console(f'{file_name}', f'{seperator}', f'{dest_path}', "green")
+                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', "green")
                     else:
                         pass
                 elif any(pattern in file_name for pattern in pattern_lists.get("Bass", [])):
                     total += 1
                     num_succeeded += 1
                     dest_path = os.path.join(os.environ['USERPROFILE'], settings.get('NOFLDPath'), settings.get("Name Of Top Library Directory"), 'Samples', 'Melodic', 'Bass')
                     if settings.get("Show More Console Logs", "True"):
-                        fsf.log_console(f'{file_name}', f'{seperator}', f'{dest_path}', "green")
+                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', "green")
                     else:
                         pass
                 elif any(pattern in file_name for pattern in pattern_lists.get("Keys", [])):
                     total += 1
                     num_succeeded += 1
                     dest_path = os.path.join(os.environ['USERPROFILE'], settings.get('NOFLDPath'), settings.get("Name Of Top Library Directory"), 'Samples', 'Melodic', 'Keys')
                     if settings.get("Show More Console Logs", True):
-                        fsf.log_console(f'{file_name}', f'{seperator}', f'{dest_path}', "green")
+                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', "green")
                     else:
                         pass
                 elif any(pattern in file_name for pattern in pattern_lists.get("Lead", [])):
                     total += 1
                     num_succeeded += 1
                     dest_path = os.path.join(os.environ['USERPROFILE'], settings.get('NOFLDPath'), settings.get("Name Of Top Library Directory"), 'Samples', 'Melodic', 'Lead')
                     if settings.get("Show More Console Logs", True):
-                        fsf.log_console(f'{file_name}', f'{seperator}', f'{dest_path}', "green")
+                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', "green")
                     else:
                         pass
                 elif any(pattern in file_name for pattern in pattern_lists.get("Pad", [])):
                     total += 1
                     num_succeeded += 1
                     dest_path = os.path.join(os.environ['USERPROFILE'], settings.get('NOFLDPath'), settings.get("Name Of Top Library Directory"), 'Samples', 'Melodic', 'Pad')
                     if settings.get("Show More Console Logs", True):
-                        fsf.log_console(f'{file_name}', f'{seperator}', f'{dest_path}', "green")
+                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', "green")
                     else:
                         pass
                 elif any(pattern in file_name for pattern in pattern_lists.get("Synth", [])):
                     total += 1
                     num_succeeded += 1
                     dest_path = os.path.join(os.environ['USERPROFILE'], settings.get('NOFLDPath'), settings.get("Name Of Top Library Directory"), 'Samples', 'Melodic', 'Synth')
                     if settings.get("Show More Console Logs", True):
-                        fsf.log_console(f'{file_name}', f'{seperator}', f'{dest_path}', "green")
+                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', "green")
                     else:
                         pass
                 elif any(pattern in file_name for pattern in pattern_lists.get("Wind", [])):
                     total += 1
                     num_succeeded += 1
                     dest_path = os.path.join(os.environ['USERPROFILE'], settings.get('NOFLDPath'), settings.get("Name Of Top Library Directory"), 'Samples', 'Melodic', 'Wind')
                     if settings.get("Show More Console Logs", True):
-                        fsf.log_console(f'{file_name}', f'{seperator}', f'{dest_path}', "green")
+                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', "green")
                     else:
                         pass
                 elif any(pattern in file_name for pattern in pattern_lists.get("String", [])):
                     total += 1
                     num_succeeded += 1
                     dest_path = os.path.join(os.environ['USERPROFILE'], settings.get('NOFLDPath'), settings.get("Name Of Top Library Directory"), 'Samples', 'Melodic', 'String')
                     if settings.get("Show More Console Logs", True):
-                        fsf.log_console(f'{file_name}', f'{seperator}', f'{dest_path}', "green")
+                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', "green")
                     else:
                         pass
                 elif any(pattern in file_name for pattern in pattern_lists.get("BassHits", [])):
                     total += 1
                     num_succeeded += 1
                     dest_path = os.path.join(os.environ['USERPROFILE'], settings.get('NOFLDPath'), settings.get("Name Of Top Library Directory"), 'Samples', 'Melodic', 'Bass', 'Hits')
                     if settings.get("Show More Console Logs", True):
-                        fsf.log_console(f'{file_name}', f'{seperator}', f'{dest_path}', "green")
+                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', "green")
                     else:
                         pass
                 elif any(pattern in file_name for pattern in pattern_lists.get("Riser", [])):
                     total += 1
                     num_succeeded += 1
                     dest_path = os.path.join(os.environ['USERPROFILE'], settings.get('NOFLDPath'), settings.get("Name Of Top Library Directory"), 'Samples', 'FX', 'Riser')
                     if settings.get("Show More Console Logs", True):
-                        fsf.log_console(f'{file_name}', f'{seperator}', f'{dest_path}', "green")
+                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', "green")
                     else:
                         pass
                 elif any(pattern in file_name for pattern in pattern_lists.get("Noise", [])):
                     total += 1
                     num_succeeded += 1
                     dest_path = os.path.join(os.environ['USERPROFILE'], settings.get('NOFLDPath'), settings.get("Name Of Top Library Directory"), 'Samples', 'FX', 'Noise')
                     if settings.get("Show More Console Logs", True):
-                        fsf.log_console(f'{file_name}', f'{seperator}', f'{dest_path}', "green")
+                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', "green")
                     else:
                         pass
                 elif any(pattern in file_name for pattern in pattern_lists.get("Siren", [])):
                     total += 1
                     num_succeeded += 1
                     dest_path = os.path.join(os.environ['USERPROFILE'], settings.get('NOFLDPath'), settings.get("Name Of Top Library Directory"), 'Samples', 'FX', 'Siren')
                     if settings.get("Show More Console Logs", True):
-                        fsf.log_console(f'{file_name}', f'{seperator}', f'{dest_path}', "green")
+                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', "green")
                     else:
                         pass
                 elif any(pattern in file_name for pattern in pattern_lists.get("Vinyl", [])):
                     total += 1
                     num_succeeded += 1
                     dest_path = os.path.join(os.environ['USERPROFILE'], settings.get('NOFLDPath'), settings.get("Name Of Top Library Directory"), 'Samples', 'FX', 'Vinyl')
                     if settings.get("Show More Console Logs", True):
-                        fsf.log_console(f'{file_name}', f'{seperator}', f'{dest_path}', "green")
+                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', "green")
                     else:
                         pass
                 elif any(pattern in file_name for pattern in pattern_lists.get("Impact", [])):
                     total += 1
                     num_succeeded += 1
                     dest_path = os.path.join(os.environ['USERPROFILE'], settings.get('NOFLDPath'), settings.get("Name Of Top Library Directory"), 'Samples', 'FX', 'Impact')
                     if settings.get("Show More Console Logs", True):
-                        fsf.log_console(f'{file_name}', f'{seperator}', f'{dest_path}', "green")
+                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', "green")
                     else:
                         pass
                 elif any(pattern in file_name for pattern in pattern_lists.get("FX", [])):
                     total += 1
                     num_succeeded += 1
                     dest_path = os.path.join(os.environ['USERPROFILE'], settings.get('NOFLDPath'), settings.get("Name Of Top Library Directory"), 'Samples', 'FX')
                     if settings.get("Show More Console Logs", True):
-                        fsf.log_console(f'{file_name}', f'{seperator}', f'{dest_path}', "green")
+                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', "green")
                     else:
                         pass
                 elif any(pattern in file_name for pattern in pattern_lists.get("DrumClap", [])):
                     total += 1
                     num_succeeded += 1
                     dest_path = os.path.join(os.environ['USERPROFILE'], settings.get('NOFLDPath'), settings.get("Name Of Top Library Directory"), 'Samples', 'Drum', 'Claps')
                     if settings.get("Show More Console Logs", True):
-                        fsf.log_console(f'{file_name}', f'{seperator}', f'{dest_path}', "green")
+                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', "green")
                     else:
                         pass
                 elif any(pattern in file_name for pattern in pattern_lists.get("DrumHats", [])):
                     total += 1
                     num_succeeded += 1
                     dest_path = os.path.join(os.environ['USERPROFILE'], settings.get('NOFLDPath'), settings.get("Name Of Top Library Directory"), 'Samples', 'Drum', 'Hats')
                     if settings.get("Show More Console Logs", True):
-                        fsf.log_console(f'{file_name}', f'{seperator}', f'{dest_path}', "green")
+                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', "green")
                     else:
                         pass
                 elif any(pattern in file_name for pattern in pattern_lists.get("DrumTom", [])):
                     total += 1
                     num_succeeded += 1
                     dest_path = os.path.join(os.environ['USERPROFILE'], settings.get('NOFLDPath'), settings.get("Name Of Top Library Directory"), 'Samples', 'Drum', 'Toms')
                     if settings.get("Show More Console Logs", True):
-                        fsf.log_console(f'{file_name}', f'{seperator}', f'{dest_path}', "green")
+                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', "green")
                     else:
                         pass
                 elif any(pattern in file_name for pattern in pattern_lists.get("808", [])):
                     total += 1
                     num_succeeded += 1
                     dest_path = os.path.join(os.environ['USERPROFILE'], settings.get('NOFLDPath'), settings.get("Name Of Top Library Directory"), 'Samples', 'Drum', '808')
                     if settings.get("Show More Console Logs", True):
-                        fsf.log_console(f'{file_name}', f'{seperator}', f'{dest_path}', "green")
+                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', "green")
                     else:
                         pass
                 elif any(pattern in file_name for pattern in pattern_lists.get("DrumPercs", [])):
                     total += 1
                     num_succeeded += 1
                     dest_path = os.path.join(os.environ['USERPROFILE'], settings.get('NOFLDPath'), settings.get("Name Of Top Library Directory"), 'Samples', 'Drum', 'Percussion')
                     if settings.get("Show More Console Logs", True):
-                        fsf.log_console(f'{file_name}', f'{seperator}', f'{dest_path}', "green")
+                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', "green")
                     else:
                         pass
                 elif any(pattern in file_name for pattern in pattern_lists.get("Percs", [])):
                     total += 1
                     num_succeeded += 1
                     dest_path = os.path.join(os.environ['USERPROFILE'], settings.get('NOFLDPath'), settings.get("Name Of Top Library Directory"), 'Samples', 'Drum', 'Percussion')
                     if settings.get("Show More Console Logs", True):
-                        fsf.log_console(f'{file_name}', f'{seperator}', f'{dest_path}', "green")
+                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', "green")
                     else:
                         pass
                 elif any(pattern in file_name for pattern in pattern_lists.get("DrumHats", [])):
                     total += 1
                     num_succeeded += 1
                     dest_path = os.path.join(os.environ['USERPROFILE'], settings.get('NOFLDPath'), settings.get("Name Of Top Library Directory"), 'Samples', 'Drum', 'Hats')
                     if settings.get("Show More Console Logs", True):
-                        fsf.log_console(f'{file_name}', f'{seperator}', f'{dest_path}', "green")
+                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', "green")
                     else:
                         pass
                 elif any(pattern in file_name for pattern in pattern_lists.get("DrumHatsOpen", [])):
                     total += 1
                     num_succeeded += 1
                     dest_path = os.path.join(os.environ['USERPROFILE'], settings.get('NOFLDPath'), settings.get("Name Of Top Library Directory"), 'Samples', 'Drum', 'Hats', 'Open')
                     if settings.get("Show More Console Logs", True):
-                        fsf.log_console(f'{file_name}', f'{seperator}', f'{dest_path}', "green")
+                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', "green")
                     else:
                         pass
                 elif any(pattern in file_name for pattern in pattern_lists.get("DrumHatsClosed", [])):
                     total += 1
                     num_succeeded += 1
                     dest_path = os.path.join(os.environ['USERPROFILE'], settings.get('NOFLDPath'), settings.get("Name Of Top Library Directory"), 'Samples', 'Drum', 'Hats', 'Closed')
                     if settings.get("Show More Console Logs", True):
-                        fsf.log_console(f'{file_name}', f'{seperator}', f'{dest_path}', "green")
+                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', "green")
                     else:
                         pass
                 elif any(pattern in file_name for pattern in pattern_lists.get("Vox", [])):
                     total += 1
                     num_succeeded += 1
                     dest_path = os.path.join(os.environ['USERPROFILE'], settings.get('NOFLDPath'), settings.get("Name Of Top Library Directory"), 'Samples', 'Voice', 'Vox')
                     if settings.get("Show More Console Logs", True):
-                        fsf.log_console(f'{file_name}', f'{seperator}', f'{dest_path}', "green")
+                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', "green")
                     else:
                         pass
                 elif any(pattern in file_name for pattern in pattern_lists.get("Vocal Chop", [])):
                     total += 1
                     num_succeeded += 1
                     dest_path = os.path.join(os.environ['USERPROFILE'], settings.get('NOFLDPath'), settings.get("Name Of Top Library Directory"), 'Samples', 'Voice', 'Vocal Chop')
                     if settings.get("Show More Console Logs", True):
-                        fsf.log_console(f'{file_name}', f'{seperator}', f'{dest_path}', "green")
+                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', "green")
                     else:
                         pass
                 elif any(pattern in file_name for pattern in pattern_lists.get("Vocal Arp", [])):
                     total += 1
                     num_succeeded += 1
                     dest_path = os.path.join(os.environ['USERPROFILE'], settings.get('NOFLDPath'), settings.get("Name Of Top Library Directory"), 'Samples', 'Voice', 'Vocal Arp')
                     if settings.get("Show More Console Logs", True):
-                        fsf.log_console(f'{file_name}', f'{seperator}', f'{dest_path}', "green")
+                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', "green")
                     else:
                         pass
                 elif any(pattern in file_name for pattern in pattern_lists.get("Hooks", [])):
                     total += 1
                     num_succeeded += 1
                     dest_path = os.path.join(os.environ['USERPROFILE'], settings.get('NOFLDPath'), settings.get("Name Of Top Library Directory"), 'Samples', 'Voice', 'Hooks')
                     if settings.get("Show More Console Logs", True):
-                        fsf.log_console(f'{file_name}', f'{seperator}', f'{dest_path}', "green")
+                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', "green")
                     else:
                         pass
                 elif any(pattern in file_name for pattern in pattern_lists.get("Screams", [])):
                     total += 1
                     num_succeeded += 1
                     dest_path = os.path.join(os.environ['USERPROFILE'], settings.get('NOFLDPath'), settings.get("Name Of Top Library Directory"), 'Samples', 'Voice', 'Scream')
                     if settings.get("Show More Console Logs", True):
-                        fsf.log_console(f'{file_name}', f'{seperator}', f'{dest_path}', "green")
+                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', "green")
                     else:
                         pass
                 elif any(pattern in file_name for pattern in pattern_lists.get("Chants", [])):
                     total += 1
                     num_succeeded += 1
                     dest_path = os.path.join(os.environ['USERPROFILE'], settings.get('NOFLDPath'), settings.get("Name Of Top Library Directory"), 'Samples', 'Voice', 'Chant')
                     if settings.get("Show More Console Logs", True):
-                        fsf.log_console(f'{file_name}', f'{seperator}', f'{dest_path}', "green")
+                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', "green")
                     else:
                         pass
                 elif any(pattern in file_name for pattern in pattern_lists.get("Phrases", [])):
                     total += 1
                     num_succeeded += 1
                     dest_path = os.path.join(os.environ['USERPROFILE'], settings.get('NOFLDPath'), settings.get("Name Of Top Library Directory"), 'Samples', 'Voice', 'Phrases')
                     if settings.get("Show More Console Logs", True):
-                        fsf.log_console(f'{file_name}', f'{seperator}', f'{dest_path}', "green")
+                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', "green")
                     else:
                         pass
                 elif any(pattern in file_name for pattern in pattern_lists.get("Voice", [])):
                     total += 1
                     num_succeeded += 1
                     dest_path = os.path.join(os.environ['USERPROFILE'], settings.get('NOFLDPath'), settings.get("Name Of Top Library Directory"), 'Samples', 'Voice')
                     if settings.get("Show More Console Logs", True):
-                        fsf.log_console(f'{file_name}', f'{seperator}', f'{dest_path}', "green")
+                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', "green")
                     else:
                         pass
                 elif any(pattern in file_name for pattern in pattern_lists.get("Atmos", [])):
                     total += 1
                     num_succeeded += 1
                     dest_path = os.path.join(os.environ['USERPROFILE'], settings.get('NOFLDPath'), settings.get("Name Of Top Library Directory"), 'Samples', 'Atmos')
                     if settings.get("Show More Console Logs", True):
-                        fsf.log_console(f'{file_name}', f'{seperator}', f'{dest_path}', "green")
+                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', "green")
                     else:
                         pass
                 else:
                     dest_path = os.path.join(os.environ['USERPROFILE'], settings.get('NOFLDPath'), settings.get("Name Of Top Library Directory"), 'Samples', 'Unsorted')
                     total += 1
                     num_failed += 1
                     if settings.get("Show More Console Logs", True):
-                        fsf.log_console(f'{file_name}', f'{seperator}', f'{dest_path}', "yellow")
+                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', "yellow")
                     else:
                         pass   
             elif file_extension in ["fxp"]:
                 if any(pattern in file_name for pattern in pattern_lists.get("Bass", [])):
                     total += 1
                     num_succeeded += 1
                     dest_path = os.path.join(os.environ['USERPROFILE'], settings.get('NOFLDPath'), settings.get("Name Of Top Library Directory"), 'Presets', 'Serum Presets', 'Bass')
                     if settings.get("Show More Console Logs", True):
-                        fsf.log_console(f'{file_name}', f'{seperator}', f'{dest_path}', "green")
+                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', "green")
                     else:
                         pass
                 elif any(pattern in file_name for pattern in pattern_lists.get("Keys", [])):
                     total += 1
                     num_succeeded += 1
                     dest_path = os.path.join(os.environ['USERPROFILE'], settings.get('NOFLDPath'), settings.get("Name Of Top Library Directory"), 'Presets', 'Serum Presets', 'Keys')
                     if settings.get("Show More Console Logs", True):
-                        fsf.log_console(f'{file_name}', f'{seperator}', f'{dest_path}', "green")
+                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', "green")
                     else:
                         pass
                 elif any(pattern in file_name for pattern in pattern_lists.get("Plucks", [])):
                     total += 1
                     num_succeeded += 1
                     dest_path = os.path.join(os.environ['USERPROFILE'], settings.get('NOFLDPath'), settings.get("Name Of Top Library Directory"), 'Presets', 'Serum Presets', 'Plucks')
                     if settings.get("Show More Console Logs", True):
-                        fsf.log_console(f'{file_name}', f'{seperator}', f'{dest_path}', "green")
+                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', "green")
                     else:
                         pass
                 elif any(pattern in file_name for pattern in pattern_lists.get("Lead", [])):
                     total += 1
                     num_succeeded += 1
                     dest_path = os.path.join(os.environ['USERPROFILE'], settings.get('NOFLDPath'), settings.get("Name Of Top Library Directory"), 'Presets', 'Serum Presets' ,'Lead')
                     if settings.get("Show More Console Logs", True):
-                        fsf.log_console(f'{file_name}', f'{seperator}', f'{dest_path}', "green")
+                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', "green")
                     else:
                         pass
                 elif any(pattern in file_name for pattern in pattern_lists.get("Synth", [])):
                     total += 1
                     num_succeeded += 1
                     dest_path = os.path.join(os.environ['USERPROFILE'], settings.get('NOFLDPath'), settings.get("Name Of Top Library Directory"), 'Presets', 'Serum Presets' ,'Synth')
                     if settings.get("Show More Console Logs", True):
-                        fsf.log_console(f'{file_name}', f'{seperator}', f'{dest_path}', "green")
+                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', "green")
                     else:
                         pass
                 elif any(pattern in file_name for pattern in pattern_lists.get("Pad", [])):
                     total += 1
                     num_succeeded += 1
                     dest_path = os.path.join(os.environ['USERPROFILE'], settings.get('NOFLDPath'), settings.get("Name Of Top Library Directory"), 'Presets', 'Serum Presets' ,'Pad')
                     if settings.get("Show More Console Logs", True):
-                        fsf.log_console(f'{file_name}', f'{seperator}', f'{dest_path}', "green")
+                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', "green")
                     else:
                         pass
                 elif any(pattern in file_name for pattern in pattern_lists.get("FX", [])):
                     total += 1
                     num_succeeded += 1
                     dest_path = os.path.join(os.environ['USERPROFILE'], settings.get('NOFLDPath'), settings.get("Name Of Top Library Directory"), 'Presets', 'Serum Presets', 'FX')
                     if settings.get("Show More Console Logs", True):
-                        fsf.log_console(f'{file_name}', f'{seperator}', f'{dest_path}', "green")
+                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', "green")
                     else:
                         pass
                 elif any(pattern in file_name for pattern in pattern_lists.get("Atmos", [])):
                     total += 1
                     num_succeeded += 1
                     dest_path = os.path.join(os.environ['USERPROFILE'], settings.get('NOFLDPath'), settings.get("Name Of Top Library Directory"), 'Presets', 'Serum Presets', 'Atmos')
                     if settings.get("Show More Console Logs"):
-                        fsf.log_console(f'{file_name}', f'{seperator}', f'{dest_path}', "green")
+                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', "green")
                 elif any(pattern in file_name for pattern in pattern_lists.get("Voice", [])):
                     total += 1
                     num_succeeded += 1
                     dest_path = os.path.join(os.environ['USERPROFILE'], settings.get('NOFLDPath'), settings.get("Name Of Top Library Directory"), 'Presets', 'Serum Presets', 'Voice')
                     if settings.get("Show More Console Logs", True):
-                        fsf.log_console(f'{file_name}', f'{seperator}', f'{dest_path}', "green")
+                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', "green")
                     else:
                         pass
                 elif any(pattern in file_name for pattern in pattern_lists.get("808", [])):
                     total += 1
                     num_succeeded += 1
                     dest_path = os.path.join(os.environ['USERPROFILE'], settings.get('NOFLDPath'), settings.get("Name Of Top Library Directory"), 'Presets', 'Serum Presets', '808')
                     if settings.get("Show More Console Logs", True):
-                        fsf.log_console(f'{file_name}', f'{seperator}', f'{dest_path}', "green")
+                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', "green")
                     else:
                         pass
                 elif any(pattern in file_name for pattern in pattern_lists.get("DrumPresets", [])):
                     total += 1
                     num_succeeded += 1
                     dest_path = os.path.join(os.environ['USERPROFILE'], settings.get('NOFLDPath'), settings.get("Name Of Top Library Directory"), 'Presets', 'Serum Presets', 'DrumPresets')
                     if settings.get("Show More Console Logs", True):
-                        fsf.log_console(f'{file_name}', f'{seperator}', f'{dest_path}', "green")
+                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', "green")
                     else:
                         pass
                 else:
                     dest_path = os.path.join(os.environ['USERPROFILE'], settings.get('NOFLDPath'), settings.get("Name Of Top Library Directory"), 'Presets', 'Serum Presets', 'Unsorted')
                     total += 1
                     num_failed += 1
                     if settings.get("Show More Console Logs", True):
-                        fsf.log_console(f'{file_name}', f'{seperator}', f'{dest_path}', "green")
+                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', "green")
                     else:
                         pass
             elif file_extension in ["nki"]:
                 total += 1
                 num_succeeded += 1
                 dest_path = os.path.join(os.environ['USERPROFILE'], settings.get('NOFLDPath'), settings.get("Name Of Top Library Directory"), 'Presets', 'Native Instruments')
                 if settings.get("Show More Console Logs", True):
-                    fsf.log_console(f'{file_name}', f'{seperator}', f'{dest_path}', "green")
+                    log_console(f'{file_name}', f'{seperator}', f'{dest_path}', "green")
                 else:
                     pass
             elif file_extension in ["mid"]:
                 if any(pattern in file_name for pattern in pattern_lists.get("DrumSnare", [])):
                     total += 1
                     num_succeeded += 1
                     dest_path = os.path.join(os.environ['USERPROFILE'], settings.get('NOFLDPath'), settings.get("Name Of Top Library Directory"), 'Midi', 'Drum', 'Snares')
                     if settings.get("Show More Console Logs", True):
-                        fsf.log_console(f'{file_name}', f'{seperator}', f'{dest_path}', "green")
+                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', "green")
                     else:
                         pass
                 elif any(pattern in file_name for pattern in pattern_lists.get("DrumClap", [])):
                     total += 1
                     num_succeeded += 1
                     dest_path = os.path.join(os.environ['USERPROFILE'], settings.get('NOFLDPath'), settings.get("Name Of Top Library Directory"), 'Midi', 'Drum', 'Claps')
                     if settings.get("Show More Console Logs", True):
-                        fsf.log_console(f'{file_name}', f'{seperator}', f'{dest_path}', "green")
+                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', "green")
                     else:
                         pass
                 elif any(pattern in file_name for pattern in pattern_lists.get("Melodic", [])):
                     total += 1
                     num_succeeded += 1
                     dest_path = os.path.join(os.environ['USERPROFILE'], settings.get('NOFLDPath'), settings.get("Name Of Top Library Directory"), 'Midi', 'Melodic')
                 elif any(pattern in file_name for pattern in pattern_lists.get("DrumTom", [])):
                     total += 1
                     num_succeeded += 1
                     dest_path = os.path.join(os.environ['USERPROFILE'], settings.get('NOFLDPath'), settings.get("Name Of Top Library Directory"), 'Midi', 'Drum', 'Toms')
                     if settings.get("Show More Console Logs", True):
-                        fsf.log_console(f'{file_name}', f'{seperator}', f'{dest_path}', "green")
+                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', "green")
                     else:
                         pass
                 elif any(pattern in file_name for pattern in pattern_lists.get("808", [])):
                     total += 1
                     num_succeeded += 1
                     dest_path = os.path.join(os.environ['USERPROFILE'], settings.get('NOFLDPath'), settings.get("Name Of Top Library Directory"), 'Midi', 'Drum', '808')
                     if settings.get("Show More Console Logs", True):
-                        fsf.log_console(f'{file_name}', f'{seperator}', f'{dest_path}', "green")
+                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', "green")
                     else:
                         pass
                 elif any(pattern in file_name for pattern in pattern_lists.get("DrumKick", [])):
                     total += 1
                     num_succeeded += 1
                     dest_path = os.path.join(os.environ['USERPROFILE'], settings.get('NOFLDPath'), settings.get("Name Of Top Library Directory"), 'Midi', 'Drum', 'Kicks')
                     if settings.get("Show More Console Logs", True):
-                        fsf.log_console(f'{file_name}', f'{seperator}', f'{dest_path}', "green")
+                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', "green")
                     else:
                         pass
                 elif any(pattern in file_name for pattern in pattern_lists.get("DrumPercs", [])):
                     total += 1
                     num_succeeded += 1
                     dest_path = os.path.join(os.environ['USERPROFILE'], settings.get('NOFLDPath'), settings.get("Name Of Top Library Directory"), 'Midi', 'Drum', 'Percussion')
                     if settings.get("Show More Console Logs", True):
-                        fsf.log_console(f'{file_name}', f'{seperator}', f'{dest_path}', "green")
+                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', "green")
                     else:
                         pass
                 elif any(pattern in file_name for pattern in pattern_lists.get("DrumShakers", [])):
                     total += 1
                     num_succeeded += 1
                     dest_path = os.path.join(os.environ['USERPROFILE'], settings.get('NOFLDPath'), settings.get("Name Of Top Library Directory"), 'Midi', 'Drum', 'Shakers')
                     if settings.get("Show More Console Logs", True):
-                        fsf.log_console(f'{file_name}', f'{seperator}', f'{dest_path}', "green")
+                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', "green")
                     else:
                         pass
                 elif any(pattern in file_name for pattern in pattern_lists.get("FX", [])):
                     total += 1
                     num_succeeded += 1
                     dest_path = os.path.join(os.environ['USERPROFILE'], settings.get('NOFLDPath'), settings.get("Name Of Top Library Directory"), 'Midi', 'FX')
                     if settings.get("Show More Console Logs", True):
-                        fsf.log_console(f'{file_name}', f'{seperator}', f'{dest_path}', "green")
+                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', "green")
                     else:
                         pass
                 elif any(pattern in file_name for pattern in pattern_lists.get("DrumLoops", [])):
                     total += 1
                     num_succeeded += 1
                     dest_path = os.path.join(os.environ['USERPROFILE'], settings.get('NOFLDPath'), settings.get("Name Of Top Library Directory"), 'Midi', 'Drum', 'Loops')
                     if settings.get("Show More Console Logs", True):
-                        fsf.log_console(f'{file_name}', f'{seperator}', f'{dest_path}', "green")
+                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', "green")
                     else:
                         pass
                 elif any(pattern in file_name for pattern in pattern_lists.get("DrumHats", [])):
                     total += 1
                     num_succeeded += 1
                     dest_path = os.path.join(os.environ['USERPROFILE'], settings.get('NOFLDPath'), settings.get("Name Of Top Library Directory"), 'Midi', 'Drum', 'Hats')
                     if settings.get("Show More Console Logs", True):
-                        fsf.log_console(f'{file_name}', f'{seperator}', f'{dest_path}', "green")
+                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', "green")
                     else:
                         pass
                 elif any(pattern in file_name for pattern in pattern_lists.get("DrumHatsOpen", [])):
                     total += 1
                     num_succeeded += 1
                     dest_path = os.path.join(os.environ['USERPROFILE'], settings.get('NOFLDPath'), settings.get("Name Of Top Library Directory"), 'Midi', 'Drum', 'Hats', 'Open')
                     if settings.get("Show More Console Logs", True):
-                        fsf.log_console(f'{file_name}', f'{seperator}', f'{dest_path}', "green")
+                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', "green")
                     else:
                         pass
                 elif any(pattern in file_name for pattern in pattern_lists.get("DrumHatsClosed", [])):
                     total += 1
                     num_succeeded += 1
                     dest_path = os.path.join(os.environ['USERPROFILE'], settings.get('NOFLDPath'), settings.get("Name Of Top Library Directory"), 'Midi', 'Drum', 'Hats', 'Closed')
                     if settings.get("Show More Console Logs", True):
-                        fsf.log_console(f'{file_name}', f'{seperator}', f'{dest_path}', "green")
+                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', "green")
                     else:
                         pass
                 elif any(pattern in file_name for pattern in pattern_lists.get("Voice", [])):
                     total += 1
                     num_succeeded += 1
                     dest_path = os.path.join(os.environ['USERPROFILE'], settings.get('NOFLDPath'), settings.get("Name Of Top Library Directory"), 'Midi', 'Voice')
                     if settings.get("Show More Console Logs", True):
-                        fsf.log_console(f'{file_name}', f'{seperator}', f'{dest_path}', "green")
+                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', "green")
                     else:
                         pass
                 elif any(pattern in file_name for pattern in pattern_lists.get("Bass", [])):
                     total += 1
                     num_succeeded += 1
                     dest_path = os.path.join(os.environ['USERPROFILE'], settings.get('NOFLDPath'), settings.get("Name Of Top Library Directory"), 'Midi', 'Bass')
                     if settings.get("Show More Console Logs", True):
-                        fsf.log_console(f'{file_name}', f'{seperator}', f'{dest_path}', "green")
+                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', "green")
                     else:
                         pass
                 elif any(pattern in file_name for pattern in pattern_lists.get("Atmos", [])):
                     total += 1
                     num_succeeded += 1
                     dest_path = os.path.join(os.environ['USERPROFILE'], settings.get('NOFLDPath'), settings.get("Name Of Top Library Directory"), 'Midi', 'Atmos')
                     if settings.get("Show More Console Logs", True):
-                        fsf.log_console(f'{file_name}', f'{seperator}', f'{dest_path}', "green")
+                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', "green")
                     else:
                         pass
                 else:
                     dest_path = os.path.join(os.environ['USERPROFILE'], settings.get('NOFLDPath'), settings.get("Name Of Top Library Directory"), 'Midi', 'Unsorted')
                     total += 1
                     num_failed += 1
                     if settings.get("Show More Console Logs", True):
-                        fsf.log_console(f'{file_name}', f'{seperator}', f'{dest_path}', "green")
+                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', "green")
                     else:
                         pass
             elif file_extension in ["nmsv"]:
                 if any(pattern in file_name for pattern in pattern_lists.get("Bass", [])):
                     num_succeeded += 1
                     dest_path = os.path.join(os.environ['USERPROFILE'], settings.get('NOFLDPath'), settings.get("Name Of Top Library Directory"), 'Presets', 'Massive Presets', 'Bass')
                     total += 1
                     if settings.get("Show More Console Logs", True):
-                        fsf.log_console(f'{file_name}', f'{seperator}', f'{dest_path}', "green")
+                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', "green")
                     else:
                         pass  
                 elif any(pattern in file_name for pattern in pattern_lists.get("Plucks", [])):
                     total += 1
                     num_succeeded += 1
                     dest_path = os.path.join(os.environ['USERPROFILE'], settings.get('NOFLDPath'), settings.get("Name Of Top Library Directory"), 'Presets', 'Massive Presets', 'Plucks')
                     if settings.get("Show More Console Logs", True):
-                        fsf.log_console(f'{file_name}', f'{seperator}', f'{dest_path}', "green")
+                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', "green")
                     else:
                         pass
                 elif any(pattern in file_name for pattern in pattern_lists.get("Keys", [])):
                     total += 1
                     num_succeeded += 1
                     dest_path = os.path.join(os.environ['USERPROFILE'], settings.get('NOFLDPath'), settings.get("Name Of Top Library Directory"), 'Presets', 'Massive Presets', 'Keys')
                     if settings.get("Show More Console Logs", True):
-                        fsf.log_console(f'{file_name}', f'{seperator}', f'{dest_path}', "green")
+                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', "green")
                     else:
                         pass
                 elif any(pattern in file_name for pattern in pattern_lists.get("Pad", [])):
                     total += 1
                     num_succeeded += 1
                     dest_path = os.path.join(os.environ['USERPROFILE'], settings.get('NOFLDPath'), settings.get("Name Of Top Library Directory"), 'Presets', 'Massive Presets', 'Pad')
                     if settings.get("Show More Console Logs", True):
-                        fsf.log_console(f'{file_name}', f'{seperator}', f'{dest_path}', "green")
+                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', "green")
                     else:
                         pass
                 elif any(pattern in file_name for pattern in pattern_lists.get("Lead", [])):
                     total += 1
                     num_succeeded += 1
                     dest_path = os.path.join(os.environ['USERPROFILE'], settings.get('NOFLDPath'), settings.get("Name Of Top Library Directory"), 'Presets', 'Massive Presets', 'Lead')
                     if settings.get("Show More Console Logs", True):
-                        fsf.log_console(f'{file_name}', f'{seperator}', f'{dest_path}', "green")
+                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', "green")
                     else:
                         pass
                 elif any(pattern in file_name for pattern in pattern_lists.get("Synth", [])):
                     total += 1
                     num_succeeded += 1
                     dest_path = os.path.join(os.environ['USERPROFILE'], settings.get('NOFLDPath'), settings.get("Name Of Top Library Directory"), 'Presets', 'Massive Presets', 'Synth')
                     if settings.get("Show More Console Logs", True):
-                        fsf.log_console(f'{file_name}', f'{seperator}', f'{dest_path}', "green")
+                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', "green")
                     else:
                         pass
                 elif any(pattern in file_name for pattern in pattern_lists.get("FX", [])):
                     total += 1
                     num_succeeded += 1
                     dest_path = os.path.join(os.environ['USERPROFILE'], settings.get('NOFLDPath'), settings.get("Name Of Top Library Directory"), 'Presets', 'Massive Presets', 'FX')
                     if settings.get("Show More Console Logs", True):
-                        fsf.log_console(f'{file_name}', f'{seperator}', f'{dest_path}', "green")
+                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', "green")
                     else:
                         pass
                 elif any(pattern in file_name for pattern in pattern_lists.get("Atmos", [])):
                     total += 1
                     num_succeeded += 1
                     dest_path = os.path.join(os.environ['USERPROFILE'], settings.get('NOFLDPath'), settings.get("Name Of Top Library Directory"), 'Presets', 'Massive Presets', 'Atmos')
                     if settings.get("Show More Console Logs", True):
-                        fsf.log_console(f'{file_name}', f'{seperator}', f'{dest_path}', "green")
+                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', "green")
                     else:
                         pass
                 elif any(pattern in file_name for pattern in pattern_lists.get("Voice", [])):
                     total += 1
                     num_succeeded += 1
                     dest_path = os.path.join(os.environ['USERPROFILE'], settings.get('NOFLDPath'), settings.get("Name Of Top Library Directory"), 'Presets', 'Massive Presets', 'Voice')
                     if settings.get("Show More Console Logs", True):
-                        fsf.log_console(f'{file_name}', f'{seperator}', f'{dest_path}', "green")
+                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', "green")
                     else:
                         pass
                 elif any(pattern in file_name for pattern in pattern_lists.get("808", [])):
                     total += 1
                     num_succeeded += 1
                     dest_path = os.path.join(os.environ['USERPROFILE'], settings.get('NOFLDPath'), settings.get("Name Of Top Library Directory"), 'Presets', 'Massive Presets', '808')
                     if settings.get("Show More Console Logs", True):
-                        fsf.log_console(f'{file_name}', f'{seperator}', f'{dest_path}', "green")
+                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', "green")
                     else:
                         pass
                 elif any(pattern in file_name for pattern in pattern_lists.get("DrumPresets", [])):
                     total += 1
                     num_succeeded += 1
                     dest_path = os.path.join(os.environ['USERPROFILE'], settings.get('NOFLDPath'), settings.get("Name Of Top Library Directory"), 'Presets', 'Massive Presets', 'DrumPresets')
                     if settings.get("Show More Console Logs", True):
-                        fsf.log_console(f'{file_name}', f'{seperator}', f'{dest_path}', "green")
+                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', "green")
                     else:
                         pass
                 else:
                     dest_path = os.path.join(os.environ['USERPROFILE'], settings.get('NOFLDPath'), settings.get("Name Of Top Library Directory"), 'Presets', 'Massive Presets', 'Unsorted')
                     total += 1
                     num_succeeded += 1
                     if settings.get("Show More Console Logs", True):
-                        fsf.log_console(f'{file_name}', f'{seperator}', f'{dest_path}', "green")
+                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', "green")
                     else:
                         pass
                         num_failed += 1
             elif file_extension in ["flp", "abl"] and any(pattern in file_name for pattern in pattern_lists.get("Templates")):
                 total += 1
                 num_succeeded += 1
                 dest_path = os.path.join(os.environ['USERPROFILE'], settings.get('NOFLDPath'), settings.get("Name Of Top Library Directory"), 'Projects', 'Templates')
                 if settings.get("Show More Console Logs", True):
-                    fsf.log_console(f'{file_name}', f'{seperator}', f'{dest_path}', "green")
+                    log_console(f'{file_name}', f'{seperator}', f'{dest_path}', "green")
                 else:
                     pass
             elif file_extension in ["flp", "abl"]:
                 total += 1
                 num_succeeded += 1
                 dest_path = os.path.join(os.environ['USERPROFILE'], settings.get('NOFLDPath'), settings.get("Name Of Top Library Directory"), 'Projects')
                 if settings.get("Show More Console Logs", True):
-                    fsf.log_console(f'{file_name}', f'{seperator}', f'{dest_path}', "green")
+                    log_console(f'{file_name}', f'{seperator}', f'{dest_path}', "green")
                 else:
                     pass
             elif file_extension in plugin_exts:
                 total += 1
                 num_succeeded += 1
                 dest_path = os.path.join(os.environ['USERPROFILE'], settings.get('NOFLDPath'), settings.get("Name Of Top Library Directory"), 'Plugins')
                 if settings.get("Show More Console Logs", True):
-                    fsf.log_console(f'{file_name}', f'{seperator}', f'{dest_path}', "green")
+                    log_console(f'{file_name}', f'{seperator}', f'{dest_path}', "green")
                 else:
                     pass
             else:
                 dest_path = rejected_unsorted_path
                 total += 1
                 num_failed2 += 1
                 if settings.get("Show More Console Logs", True):
-                    fsf.log_console(f'{file_name}', f'{seperator}', f'{rejected_unsorted_path}', "red")
+                    log_console(f'{file_name}', f'{seperator}', f'{rejected_unsorted_path}', "red")
                 else:
                     pass
-            fsf.organize_files_by_extension(rejected_unsorted_path)
+            organize_files_by_extension(rejected_unsorted_path)
             if not os.path.exists(os.path.join(dest_path, filename)):
                 os.makedirs(dest_path, exist_ok="green")
                 shutil.move(file_path, dest_path)
             else:
                 pass
     elapsed_time = time.time() - start_time
     prompt1 = settings.get("Prompt")
     def remove_readonly(func, path, _):
         os.chmod(path, stat.S_IWRITE)
         func(path)
     shutil.rmtree(path1, onerror=remove_readonly)
-    fsf.check_dir(path1)
+    check_dir(path1)
     def remove_readonly(func, path, _):
         os.chmod(path, stat.S_IWRITE)
         func(path)
     shutil.rmtree(path1, onerror=remove_readonly)
-    fsf.check_dir(path1)
+    check_dir(path1)
     if settings.get("Show Top Bar", True):
         bar = settings.get("Top Bar")
-        fsf.log_message(bar, f'{settings.get("Top Bar Color")}', True, True)
+        log_message(bar, f'{settings.get("Top Bar Color")}', True, True)
     else:
         pass
     if settings.get("Show Statistics", True):
-        fsf.log_message(prompt1, f'{settings.get("Prompt Color")}', False, False)
-        fsf.log_message(f'sorted by name & file type:   ', f'{settings.get("Foregroud Color 1")}', False, False)
-        fsf.log_message(f' {num_succeeded}', "green")
-        fsf.log_message(prompt1, f'{settings.get("Prompt Color")}', False, False)
-        fsf.log_message(f'sorted only by file type: ', f'{settings.get("Foregroud Color 1")}', False, False)
-        fsf.log_message(f' {num_failed}', "yellow")
-        fsf.log_message(prompt1, f'{settings.get("Prompt Color")}', False, False)
-        fsf.log_message(f'rejected file types: ', f'{settings.get("Foregroud Color 1")}', False, False)
-        fsf.log_message(f' {num_failed2}', "red")
-        fsf.log_message(f'      {total}', f'{settings.get("Statistics Value Color")}', False, False)
-        fsf.log_message(f' files processed in ', "dark_grey", False, False)
-        fsf.log_message(f'{elapsed_time:.2f}', f'{settings.get("Statistics Value Color")}', False, False)
-        fsf.log_message(f' seconds', "dark_grey", False, True)
+        log_message(prompt1, f'{settings.get("Prompt Color")}', False, False)
+        log_message(f'sorted by name & file type:   ', f'{settings.get("Foregroud Color 1")}', False, False)
+        log_message(f' {num_succeeded}', "green")
+        log_message(prompt1, f'{settings.get("Prompt Color")}', False, False)
+        log_message(f'sorted only by file type: ', f'{settings.get("Foregroud Color 1")}', False, False)
+        log_message(f' {num_failed}', "yellow")
+        log_message(prompt1, f'{settings.get("Prompt Color")}', False, False)
+        log_message(f'rejected file types: ', f'{settings.get("Foregroud Color 1")}', False, False)
+        log_message(f' {num_failed2}', "red")
+        log_message(f'      {total}', f'{settings.get("Statistics Value Color")}', False, False)
+        log_message(f' files processed in ', "dark_grey", False, False)
+        log_message(f'{elapsed_time:.2f}', f'{settings.get("Statistics Value Color")}', False, False)
+        log_message(f' seconds', "dark_grey", False, True)
         maxfile = settings.get('Max files per Dir')
-        fsf.split_files_in_subdirectories(path2, max_files_per_dir=maxfile)
-        file_count, dir_count, total_size_mb, total_size_gb = fsf.count_files_in_directory(f'{path2}')
-        fsf.log_message(f'          in ', "dark_grey", False, False)
-        fsf.log_message(f'{settings.get("Name Of Top Library Directory")}', f'{settings.get("Statistics Value Color")}', False, True)
-        fsf.log_message(f'              files', "dark_grey", False, False)
-        fsf.log_message(f' {file_count}', f'{settings.get("Statistics Value Color")}', False, True)
-        fsf.log_message(f'                  subdirectories', "dark_grey", False, False)
-        fsf.log_message(f' {dir_count}', f'{settings.get("Statistics Value Color")}', False, True)
-        fsf.log_message(f'                      size', "dark_grey", False, False)
-        fsf.log_message(f' {total_size_mb:.2f}', f'{settings.get("Statistics Value Color")}', False, False)
-        fsf.log_message(f' mb ', "light_grey", False, False)
-        fsf.log_message(f'or ', "dark_grey", False, False)
-        fsf.log_message(f'{total_size_gb:.2f}', f'{settings.get("Statistics Value Color")}', False, False)
-        fsf.log_message(f' gb', "light_grey", False, False)
-        fsf.log_message(f'', "light_grey", False, True)
+        split_files_in_subdirectories(path2, max_files_per_dir=maxfile)
+        file_count, dir_count, total_size_mb, total_size_gb = count_files_in_directory(f'{path2}')
+        log_message(f'          in ', "dark_grey", False, False)
+        log_message(f'{settings.get("Name Of Top Library Directory")}', f'{settings.get("Statistics Value Color")}', False, True)
+        log_message(f'              files', "dark_grey", False, False)
+        log_message(f' {file_count}', f'{settings.get("Statistics Value Color")}', False, True)
+        log_message(f'                  subdirectories', "dark_grey", False, False)
+        log_message(f' {dir_count}', f'{settings.get("Statistics Value Color")}', False, True)
+        log_message(f'                      size', "dark_grey", False, False)
+        log_message(f' {total_size_mb:.2f}', f'{settings.get("Statistics Value Color")}', False, False)
+        log_message(f' mb ', "light_grey", False, False)
+        log_message(f'or ', "dark_grey", False, False)
+        log_message(f'{total_size_gb:.2f}', f'{settings.get("Statistics Value Color")}', False, False)
+        log_message(f' gb', "light_grey", False, False)
+        log_message(f'', "light_grey", False, True)
     else:
         pass
     def remove_readonly(func, path, _):
         os.chmod(path, stat.S_IWRITE)
         func(path)
     shutil.rmtree(path1, onerror=remove_readonly)
-    fsf.check_dir(path1)
-temp_content = "\nSorted Library Location:        "+ f"{os.path.join(os.environ['USERPROFILE'], settings.get('NOFLDPath'), settings.get('Name Of Top Library Directory'))}"+ "\nSettings Location:     "+ f"{os.path.join(fsf.path_finder(0), 'settings.json')}"+ "\nPyhton Script Location:    " f"{os.path.join(current_location, 'slib_sorter.py')}"+ "\nTo Be Sorted Location:    " f"{os.path.join(os.environ['USERPROFILE'], settings.get('TBPDPath'), settings.get('To Be Processed Directory'))}"+ "\nRejected Files Location:     " f"{os.path.join(os.environ['USERPROFILE'], settings.get('RFPath'), settings.get('Rejected Files'))}"
+    check_dir(path1)
+temp_content = "\nSorted Library Location:        "+ f"{os.path.join(os.environ['USERPROFILE'], settings.get('NOFLDPath'), settings.get('Name Of Top Library Directory'))}"+ "\nSettings Location:     "+ f"{os.path.join(path_finder(0), 'settings.json')}"+ "\nPyhton Script Location:    " f"{os.path.join(current_location, 'slib_sorter.py')}"+ "\nTo Be Sorted Location:    " f"{os.path.join(os.environ['USERPROFILE'], settings.get('TBPDPath'), settings.get('To Be Processed Directory'))}"+ "\nRejected Files Location:     " f"{os.path.join(os.environ['USERPROFILE'], settings.get('RFPath'), settings.get('Rejected Files'))}"
 def print_help_message():
     parser = argparse.ArgumentParser()
     parser.add_argument("-paths", action="store_true")
     parser.add_argument("-help", action="store_true")
     parser.add_argument("-colors", action="store_true")
     parser.add_argument("-config", action="store_true")
-    temp_file_path = fsf.temp_path_file(temp_content)
+    temp_file_path = temp_path_file(temp_content)
     args = parser.parse_args()
     spacer = "              "
     if args.paths:
         with open(temp_file_path, 'r') as file:
             temp_file_path = file.read()
         os.system('cls')
         bar = settings.get("Top Bar")
-        fsf.log_message(bar, f'{settings.get("Top Bar Color")}', True, True)
-        fsf.log_message(temp_content, 'white', False, True)
+        log_message(bar, f'{settings.get("Top Bar Color")}', True, True)
+        log_message(temp_content, 'white', False, True)
     elif args.colors:
         os.system('cls')
         bar = settings.get("Top Bar")
-        fsf.log_message(bar, f'{settings.get("Top Bar Color")}', True, True)
+        log_message(bar, f'{settings.get("Top Bar Color")}', True, True)
         clist = {
             "Colors": ['black', 'red', 'green', 'yellow', 'blue', 'magenta', 'cyan', 'white', 'light_grey', 'dark_grey', 'light_red', 'light_green', 'light_yellow', 'light_blue', 'light_magenta', 'light_cyan']
         }
         colors = clist["Colors"]
-        fsf.log_message("Possible Color Settings", f'{settings.get("Statistics Value Color")}', False, False)
-        fsf.log_message(':', f'{settings.get("Foregroud Color 1")}', False, True)
+        log_message("Possible Color Settings", f'{settings.get("Statistics Value Color")}', False, False)
+        log_message(':', f'{settings.get("Foregroud Color 1")}', False, True)
         for color in colors:
-            fsf.log_message(spacer+ color, f'{color}', False, True)
+            log_message(spacer+ color, f'{color}', False, True)
     elif args.help:
         os.system('cls')
         bar = settings.get("Top Bar")
-        fsf.log_message(bar, f'{settings.get("Top Bar Color")}', True, True)
-        fsf.log_message('Help', f'{settings.get("Statistics Value Color")}', False, False)
-        fsf.log_message(':', f'{settings.get("Foregroud Color 1")}', False, True)
-        fsf.log_message('           -paths '+ f'{spacer}', f'{settings.get("Foregroud Color 1")}', False, False)
-        fsf.log_message('Displays Paths', f'{settings.get("Statistics Value Color")}', False, True)
-        fsf.log_message('           -colors'+ f'{spacer}', f'{settings.get("Foregroud Color 1")}', False, False)
-        fsf.log_message('Displays Possible Color Settings', f'{settings.get("Statistics Value Color")}', False, True)
-        fsf.log_message('           -config'+ f'{spacer}', f'{settings.get("Foregroud Color 1")}', False, False)
-        fsf.log_message('Launch Config File', f'{settings.get("Statistics Value Color")}', False, True)
-        fsf.log_message('           -help  '+ f'{spacer}', f'{settings.get("Foregroud Color 1")}', False, False)
-        fsf.log_message('Displays Help', f'{settings.get("Statistics Value Color")}', False, True)
+        log_message(bar, f'{settings.get("Top Bar Color")}', True, True)
+        log_message('Help', f'{settings.get("Statistics Value Color")}', False, False)
+        log_message(':', f'{settings.get("Foregroud Color 1")}', False, True)
+        log_message('           -paths '+ f'{spacer}', f'{settings.get("Foregroud Color 1")}', False, False)
+        log_message('Displays Paths', f'{settings.get("Statistics Value Color")}', False, True)
+        log_message('           -colors'+ f'{spacer}', f'{settings.get("Foregroud Color 1")}', False, False)
+        log_message('Displays Possible Color Settings', f'{settings.get("Statistics Value Color")}', False, True)
+        log_message('           -config'+ f'{spacer}', f'{settings.get("Foregroud Color 1")}', False, False)
+        log_message('Launch Config File', f'{settings.get("Statistics Value Color")}', False, True)
+        log_message('           -help  '+ f'{spacer}', f'{settings.get("Foregroud Color 1")}', False, False)
+        log_message('Displays Help', f'{settings.get("Statistics Value Color")}', False, True)
     elif args.config:
-        settingsfile = os.path.join(fsf.path_finder(0), 'settings.json')
+        settingsfile = os.path.join(path_finder(0), 'settings.json')
         cmd = "Start "+ settingsfile
         os.system(cmd)
     else:
         sort_files(path1, pattern_lists) 
 def __main__():
     print_help_message()
 __main__()
```

