# Comparing `tmp/slib-sorter-1.2.0.tar.gz` & `tmp/slib-sorter-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slib-sorter-1.2.0.tar", last modified: Sat Jul  8 04:01:07 2023, max compression
+gzip compressed data, was "slib-sorter-1.2.1.tar", last modified: Sat Jul  8 04:16:23 2023, max compression
```

## Comparing `slib-sorter-1.2.0.tar` & `slib-sorter-1.2.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-08 04:01:07.230651 slib-sorter-1.2.0/
--rw-rw-rw-   0        0        0    11558 2023-07-07 20:03:54.000000 slib-sorter-1.2.0/LICENSE
--rw-rw-rw-   0        0        0     2267 2023-07-08 04:01:07.230651 slib-sorter-1.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     1783 2023-07-08 03:49:36.000000 slib-sorter-1.2.0/README.md
--rw-rw-rw-   0        0        0       42 2023-07-08 04:01:07.230651 slib-sorter-1.2.0/setup.cfg
--rw-rw-rw-   0        0        0     4368 2023-07-08 04:00:58.000000 slib-sorter-1.2.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-08 04:01:07.228687 slib-sorter-1.2.0/slib_sorter.egg-info/
--rw-rw-rw-   0        0        0     2267 2023-07-08 04:01:07.000000 slib-sorter-1.2.0/slib_sorter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      273 2023-07-08 04:01:07.000000 slib-sorter-1.2.0/slib_sorter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-08 04:01:07.000000 slib-sorter-1.2.0/slib_sorter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       57 2023-07-08 04:01:07.000000 slib-sorter-1.2.0/slib_sorter.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       17 2023-07-08 04:01:07.000000 slib-sorter-1.2.0/slib_sorter.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-07-08 04:01:07.000000 slib-sorter-1.2.0/slib_sorter.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-08 04:01:07.229657 slib-sorter-1.2.0/src/
--rw-rw-rw-   0        0        0        0 2023-06-28 15:10:46.000000 slib-sorter-1.2.0/src/__init__.py
--rw-rw-rw-   0        0        0    72332 2023-07-08 03:43:41.000000 slib-sorter-1.2.0/src/slib_sorter.py
+drwxrwxrwx   0        0        0        0 2023-07-08 04:16:23.605795 slib-sorter-1.2.1/
+-rw-rw-rw-   0        0        0    11558 2023-07-07 20:03:54.000000 slib-sorter-1.2.1/LICENSE
+-rw-rw-rw-   0        0        0     2267 2023-07-08 04:16:23.605795 slib-sorter-1.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1783 2023-07-08 03:49:36.000000 slib-sorter-1.2.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-08 04:16:23.605795 slib-sorter-1.2.1/setup.cfg
+-rw-rw-rw-   0        0        0     4416 2023-07-08 04:15:00.000000 slib-sorter-1.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-08 04:16:23.595795 slib-sorter-1.2.1/slib_sorter.egg-info/
+-rw-rw-rw-   0        0        0     2267 2023-07-08 04:16:23.000000 slib-sorter-1.2.1/slib_sorter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      273 2023-07-08 04:16:23.000000 slib-sorter-1.2.1/slib_sorter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-08 04:16:23.000000 slib-sorter-1.2.1/slib_sorter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       57 2023-07-08 04:16:23.000000 slib-sorter-1.2.1/slib_sorter.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       17 2023-07-08 04:16:23.000000 slib-sorter-1.2.1/slib_sorter.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-07-08 04:16:23.000000 slib-sorter-1.2.1/slib_sorter.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-08 04:16:23.604794 slib-sorter-1.2.1/src/
+-rw-rw-rw-   0        0        0        0 2023-06-28 15:10:46.000000 slib-sorter-1.2.1/src/__init__.py
+-rw-rw-rw-   0        0        0    69268 2023-07-08 04:15:41.000000 slib-sorter-1.2.1/src/slib_sorter.py
```

### Comparing `slib-sorter-1.2.0/LICENSE` & `slib-sorter-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `slib-sorter-1.2.0/PKG-INFO` & `slib-sorter-1.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slib-sorter
-Version: 1.2.0
+Version: 1.2.1
 Summary: A Python package for sorting Sample Libraries
 Home-page: https://github.com/nrdrch/slib-sorter
 Author: Lukas Hübinger
 Author-email: fettkindasindauchoke@gmail.com
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
```

### Comparing `slib-sorter-1.2.0/README.md` & `slib-sorter-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `slib-sorter-1.2.0/setup.py` & `slib-sorter-1.2.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import setuptools
 import shutil
 import os
 import json, importlib
-current_location = os.path.abspath(os.path.dirname(__file__))
+settings_folder = os.path.join(os.environ['USERPROFILE'], 'Documents', 'WindowsPowerShell', 'Scripts', 'slib_sorter')
+settings = os.path.join(settings_folder, "settings.json")
 def ps_script(source_file):
     winpro = os.path.join(os.environ['USERPROFILE'],'Documents', 'WindowsPowerShell')
     powershell_scripts_folder = os.path.join(winpro, 'Scripts', 'slib_sorter')
     if not os.path.exists(powershell_scripts_folder):
         os.makedirs(powershell_scripts_folder)
     powershell_script_file = os.path.join(powershell_scripts_folder, 'slib_sorter' + ".psm1")
     settings_file = os.path.join(powershell_scripts_folder, 'settings.json')
@@ -21,16 +22,16 @@
     $pythonScript = '{source_file}'
     python3 $pythonScript $argsString
 }}
     '''
     #with open(powershell_script_file, 'a') as f:
     #    f.write(script_content)
     
-    if not os.path.exists(powershell_scripts_folder):
-        os.makedirs(powershell_scripts_folder)
+    if not os.path.exists(settings_folder):
+        os.makedirs(settings_folder)
     default_config = f'''
 {{
     "Foregroud Color 1": "white",
     "Top Bar Color": "dark_grey",
     "Show Top Bar": true,
     "Top Bar": "<   Sample Library Sorter   >",
     "Prompt Color": "dark_grey",
@@ -49,17 +50,17 @@
     "Rejected Files": "Rejected Files",
     "Run Shell Command On Startup": false,
     "Command On Startup": "cls" 
 }}
     '''
     with open(settings_file, 'w') as f:
         f.write(default_config)
+    with open(settings_file, 'r') as file:
+        settings_file = json.load(file)
     settings = settings_file
-    with open(settings, 'r') as file:
-        settings = json.load(file)
     #profile_path = os.path.expanduser("~/Documents/WindowsPowerShell/Microsoft.PowerShell_profile.ps1")
     #with open(profile_path, 'r') as f:
     #    profile_content = f.read()
     #    if f"Import-Module -DisableNameChecking \"{powershell_script_file}\"" in profile_content:
     #        pass
     #    else:
     #        with open(profile_path, 'a') as f:
@@ -69,25 +70,28 @@
             CmdOnStartup = settings.get("Command On Startup")
             os.system(CmdOnStartup)
         else:
             pass
     except:
         winpro = os.path.join(os.environ['USERPROFILE'],'Documents', 'WindowsPowerShell')
         powershell_scripts_folder = os.path.join(winpro, 'Scripts', 'slib_sorter')
-        settings_file = os.path.join(powershell_scripts_folder, 'settings.json')
-        importlib.reload(settings_file)
+        
+        importlib.reload(settings)
         #setupfile = os.path.join(path_finder(0), 'setup.py')
-        importlib.reload(settings_file)
+
+
+
+current_location = os.path.abspath(os.path.dirname(__file__))
 def install():
     with open("README.md", "r", encoding="utf-8") as fh:
         long_description = fh.read()
 
     setuptools.setup(
         name="slib-sorter",
-        version="1.2.0",
+        version="1.2.1",
         author="Lukas Hübinger",
         author_email="fettkindasindauchoke@gmail.com",
         description="A Python package for sorting Sample Libraries",
         long_description=long_description,
         long_description_content_type="text/markdown",
         url="https://github.com/nrdrch/slib-sorter",
         packages=setuptools.find_packages(), 
@@ -104,14 +108,14 @@
             "License :: OSI Approved :: Apache Software License",
             "Operating System :: Microsoft :: Windows :: Windows 10"
         ],
     )
     ps_script(os.path.join(current_location, "src", "slib_sorter.py"))
     
 def reload():
-    importlib.reload(current_location)
+    importlib.reload(settings)
 def __main__():
     try:
         install()
     except:
         reload()
 __main__()
```

### Comparing `slib-sorter-1.2.0/slib_sorter.egg-info/PKG-INFO` & `slib-sorter-1.2.1/slib_sorter.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slib-sorter
-Version: 1.2.0
+Version: 1.2.1
 Summary: A Python package for sorting Sample Libraries
 Home-page: https://github.com/nrdrch/slib-sorter
 Author: Lukas Hübinger
 Author-email: fettkindasindauchoke@gmail.com
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
```

### Comparing `slib-sorter-1.2.0/src/slib_sorter.py` & `slib-sorter-1.2.1/src/slib_sorter.py`

 * *Files 3% similar despite different names*

```diff
@@ -34,86 +34,15 @@
 def log_console(file_name, seperator, dest_path, color):
     if settings.get("Show More Console Logs", True):
         log_message(f'{file_name}', f'{color}', False, False)
         log_message(f'{seperator}', "dark_grey", False, False)
         log_message(f' {dest_path}', "white", False, True)
     else:
         pass
-def ps_script(source_file):
-    winpro = os.path.join(os.environ['USERPROFILE'],'Documents', 'WindowsPowerShell')
-    powershell_scripts_folder = os.path.join(winpro, 'Scripts', 'slib_sorter')
-    if not os.path.exists(powershell_scripts_folder):
-        os.makedirs(powershell_scripts_folder)
-    powershell_script_file = os.path.join(powershell_scripts_folder, 'slib_sorter' + ".psm1")
-    settings_file = os.path.join(powershell_scripts_folder, 'settings.json')
-    script_content = f'''
-function Start-Sorter {{
-    [CmdletBinding()]
-    param(
-        [Parameter(ValueFromRemainingArguments=$true)]
-        [string]$CustomInput
-    )
-    $argsString = $CustomInput -join "' '"
-    $pythonScript = '{source_file}'
-    python3 $pythonScript $argsString
-}}
-    '''
-    #with open(powershell_script_file, 'a') as f:
-    #    f.write(script_content)
-    
-    if not os.path.exists(settings_folder):
-        os.makedirs(settings_folder)
-    default_config = f'''
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
-    "TBPDPath": "Desktop",
-    "To Be Processed Directory": "To Be Sorted",
-    "NOFLDPath": "Desktop",
-    "Name Of Top Library Directory": "Sample Library",
-    "RFPath": "Desktop",
-    "Rejected Files": "Rejected Files",
-    "Run Shell Command On Startup": false,
-    "Command On Startup": "cls" 
-}}
-    '''
-    with open(settings_file, 'w') as f:
-        f.write(default_config)
-    with open(settings_file, 'r') as file:
-        settings_file = json.load(file)
-    #profile_path = os.path.expanduser("~/Documents/WindowsPowerShell/Microsoft.PowerShell_profile.ps1")
-    #with open(profile_path, 'r') as f:
-    #    profile_content = f.read()
-    #    if f"Import-Module -DisableNameChecking \"{powershell_script_file}\"" in profile_content:
-    #        pass
-    #    else:
-    #        with open(profile_path, 'a') as f:
-    #            f.write(f"\nImport-Module -DisableNameChecking \"{powershell_script_file}\"")
-    try:
-        if settings.get("Run Shell Command On Startup", True):
-            CmdOnStartup = settings.get("Command On Startup")
-            os.system(CmdOnStartup)
-        else:
-            pass
-    except:
-        winpro = os.path.join(os.environ['USERPROFILE'],'Documents', 'WindowsPowerShell')
-        powershell_scripts_folder = os.path.join(winpro, 'Scripts', 'slib_sorter')
-        
-        importlib.reload(settings_f)
-        #setupfile = os.path.join(path_finder(0), 'setup.py')
+
 def change_folder_icon(folder_path, icon_path):
     if not os.path.exists(folder_path):
         print("Folder does not exist.")
         return
     folder_path = os.path.abspath(folder_path)
     try:
         ini_path = os.path.join(folder_path, "desktop.ini")
@@ -123,22 +52,17 @@
             ini_file.write("IconIndex=0\n")
         ctypes.windll.kernel32.SetFileAttributesW(ini_path, 0x2 | 0x4)
         ctypes.windll.shell32.SHChangeNotify(0x08000000, 0x0000, None, None)
         print("Folder icon changed successfully.")
     except Exception as e:
         print(f"An error occurred: {str(e)}")
 
-if not os.path.exists(settings):
-    current_location = path_finder(0)
-    source_file = os.path.join(current_location, 'slib_sorter.py')
-    ps_script(source_file)
 
-else:
-    with open(settings, 'r') as file:
-        settings = json.load(file)
+with open(settings, 'r') as file:
+    settings = json.load(file)
 
 def organize_files_by_extension(path):
     if not os.path.isdir(path):
         raise Exception("The path provided is not a directory.")
     files = [f for f in os.listdir(path) if os.path.isfile(os.path.join(path, f))]
     for file in files:
         file_name, file_extension = os.path.splitext(file)
@@ -222,15 +146,14 @@
     return file_path
 
 
 
 start_time = time.time()
 current_location = path_finder(0)
 source_file = os.path.join(current_location, 'slib_sorter.py')
-ps_script(source_file)
 icon_path = os.path.join(path_finder(1), 'examples', 'icn.ico')
 
 settings_f = os.path.join(os.environ['USERPROFILE'], 'Documents', 'WindowsPowerShell', 'Scripts', 'slib_sorter', 'settings.json')
 #settings = os.path.join(path_finder(0), 'settings.json')
 with open(settings_f, 'r') as file:
     settings_f = json.load(file)
 file_path = path1 = os.path.join(os.environ['USERPROFILE'], settings.get('TBPDPath'), settings.get('To Be Processed Directory'))
@@ -1119,8 +1042,8 @@
         settingsfile = settings_f
         cmd = "Start "+ settingsfile
         os.system(cmd)
     else:
         sort_files(path1, pattern_lists) 
 def __main__():
     print_help_message()
-__main__
+__main__()
```

