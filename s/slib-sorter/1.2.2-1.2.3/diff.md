# Comparing `tmp/slib-sorter-1.2.2.tar.gz` & `tmp/slib-sorter-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slib-sorter-1.2.2.tar", last modified: Sat Jul  8 04:30:35 2023, max compression
+gzip compressed data, was "slib-sorter-1.2.3.tar", last modified: Sat Jul  8 04:42:27 2023, max compression
```

## Comparing `slib-sorter-1.2.2.tar` & `slib-sorter-1.2.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-08 04:30:35.271140 slib-sorter-1.2.2/
--rw-rw-rw-   0        0        0    11558 2023-07-07 20:03:54.000000 slib-sorter-1.2.2/LICENSE
--rw-rw-rw-   0        0        0     2267 2023-07-08 04:30:35.270140 slib-sorter-1.2.2/PKG-INFO
--rw-rw-rw-   0        0        0     1783 2023-07-08 03:49:36.000000 slib-sorter-1.2.2/README.md
--rw-rw-rw-   0        0        0       42 2023-07-08 04:30:35.271140 slib-sorter-1.2.2/setup.cfg
--rw-rw-rw-   0        0        0     4478 2023-07-08 04:30:05.000000 slib-sorter-1.2.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-08 04:30:35.268116 slib-sorter-1.2.2/slib_sorter.egg-info/
--rw-rw-rw-   0        0        0     2267 2023-07-08 04:30:35.000000 slib-sorter-1.2.2/slib_sorter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      273 2023-07-08 04:30:35.000000 slib-sorter-1.2.2/slib_sorter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-08 04:30:35.000000 slib-sorter-1.2.2/slib_sorter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       57 2023-07-08 04:30:35.000000 slib-sorter-1.2.2/slib_sorter.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       17 2023-07-08 04:30:35.000000 slib-sorter-1.2.2/slib_sorter.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-07-08 04:30:35.000000 slib-sorter-1.2.2/slib_sorter.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-08 04:30:35.269127 slib-sorter-1.2.2/src/
--rw-rw-rw-   0        0        0        0 2023-06-28 15:10:46.000000 slib-sorter-1.2.2/src/__init__.py
--rw-rw-rw-   0        0        0    69268 2023-07-08 04:15:41.000000 slib-sorter-1.2.2/src/slib_sorter.py
+drwxrwxrwx   0        0        0        0 2023-07-08 04:42:27.242838 slib-sorter-1.2.3/
+-rw-rw-rw-   0        0        0    11558 2023-07-07 20:03:54.000000 slib-sorter-1.2.3/LICENSE
+-rw-rw-rw-   0        0        0     2267 2023-07-08 04:42:27.242838 slib-sorter-1.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1783 2023-07-08 03:49:36.000000 slib-sorter-1.2.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-08 04:42:27.242838 slib-sorter-1.2.3/setup.cfg
+-rw-rw-rw-   0        0        0     4382 2023-07-08 04:42:08.000000 slib-sorter-1.2.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-08 04:42:27.239820 slib-sorter-1.2.3/slib_sorter.egg-info/
+-rw-rw-rw-   0        0        0     2267 2023-07-08 04:42:27.000000 slib-sorter-1.2.3/slib_sorter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      273 2023-07-08 04:42:27.000000 slib-sorter-1.2.3/slib_sorter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-08 04:42:27.000000 slib-sorter-1.2.3/slib_sorter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       57 2023-07-08 04:42:27.000000 slib-sorter-1.2.3/slib_sorter.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       17 2023-07-08 04:42:27.000000 slib-sorter-1.2.3/slib_sorter.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-07-08 04:42:27.000000 slib-sorter-1.2.3/slib_sorter.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-08 04:42:27.241823 slib-sorter-1.2.3/src/
+-rw-rw-rw-   0        0        0        0 2023-06-28 15:10:46.000000 slib-sorter-1.2.3/src/__init__.py
+-rw-rw-rw-   0        0        0    69292 2023-07-08 04:39:16.000000 slib-sorter-1.2.3/src/slib_sorter.py
```

### Comparing `slib-sorter-1.2.2/LICENSE` & `slib-sorter-1.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `slib-sorter-1.2.2/PKG-INFO` & `slib-sorter-1.2.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slib-sorter
-Version: 1.2.2
+Version: 1.2.3
 Summary: A Python package for sorting Sample Libraries
 Home-page: https://github.com/nrdrch/slib-sorter
 Author: Lukas Hübinger
 Author-email: fettkindasindauchoke@gmail.com
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
```

### Comparing `slib-sorter-1.2.2/README.md` & `slib-sorter-1.2.3/README.md`

 * *Files identical despite different names*

### Comparing `slib-sorter-1.2.2/setup.py` & `slib-sorter-1.2.3/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 settings_folder = os.path.join(os.environ['USERPROFILE'], 'Documents', 'WindowsPowerShell', 'Scripts', 'slib_sorter')
 settings = os.path.join(settings_folder, "settings.json")
 def ps_script(source_file):
     winpro = os.path.join(os.environ['USERPROFILE'],'Documents', 'WindowsPowerShell')
     powershell_scripts_folder = os.path.join(winpro, 'Scripts', 'slib_sorter')
     if not os.path.exists(powershell_scripts_folder):
         os.makedirs(powershell_scripts_folder)
+    else:
+        pass
     powershell_script_file = os.path.join(powershell_scripts_folder, 'slib_sorter' + ".psm1")
     settings_file = os.path.join(powershell_scripts_folder, 'settings.json')
     script_content = f'''
 function Start-Sorter {{
     [CmdletBinding()]
     param(
         [Parameter(ValueFromRemainingArguments=$true)]
@@ -24,14 +26,16 @@
 }}
     '''
     #with open(powershell_script_file, 'a') as f:
     #    f.write(script_content)
     
     if not os.path.exists(settings_folder):
         os.makedirs(settings_folder)
+    else:
+        pass
     default_config = f'''
 {{
     "Foregroud Color 1": "white",
     "Top Bar Color": "dark_grey",
     "Show Top Bar": true,
     "Top Bar": "<   Sample Library Sorter   >",
     "Prompt Color": "dark_grey",
@@ -54,17 +58,14 @@
     '''
     settings = settings_file
     if not os.path.exists(settings):
         with open(settings, 'w') as f:
             f.write(default_config)
     else:
         pass
-    with open(settings, 'r') as file:
-        settings = json.load(file)
-    
     #profile_path = os.path.expanduser("~/Documents/WindowsPowerShell/Microsoft.PowerShell_profile.ps1")
     #with open(profile_path, 'r') as f:
     #    profile_content = f.read()
     #    if f"Import-Module -DisableNameChecking \"{powershell_script_file}\"" in profile_content:
     #        pass
     #    else:
     #        with open(profile_path, 'a') as f:
@@ -74,28 +75,26 @@
             CmdOnStartup = settings.get("Command On Startup")
             os.system(CmdOnStartup)
         else:
             pass
     except:
         winpro = os.path.join(os.environ['USERPROFILE'],'Documents', 'WindowsPowerShell')
         powershell_scripts_folder = os.path.join(winpro, 'Scripts', 'slib_sorter')
-        
-        importlib.reload(settings)
         #setupfile = os.path.join(path_finder(0), 'setup.py')
 
 
 
 current_location = os.path.abspath(os.path.dirname(__file__))
 def install():
     with open("README.md", "r", encoding="utf-8") as fh:
         long_description = fh.read()
 
     setuptools.setup(
         name="slib-sorter",
-        version="1.2.2",
+        version="1.2.3",
         author="Lukas Hübinger",
         author_email="fettkindasindauchoke@gmail.com",
         description="A Python package for sorting Sample Libraries",
         long_description=long_description,
         long_description_content_type="text/markdown",
         url="https://github.com/nrdrch/slib-sorter",
         packages=setuptools.find_packages(), 
@@ -109,17 +108,17 @@
         ],
         classifiers=[
             "Programming Language :: Python :: 3.7",
             "License :: OSI Approved :: Apache Software License",
             "Operating System :: Microsoft :: Windows :: Windows 10"
         ],
     )
-    ps_script(os.path.join(current_location, "src", "slib_sorter.py"))
+    if not os.path.exists(settings):
+        ps_script(os.path.join(current_location, "src", "slib_sorter.py"))
+    else:
+        pass
     
-def reload():
-    importlib.reload(settings)
-def __main__():
-    try:
-        install()
-    except:
-        reload()
-__main__()
+
+def __setup__():
+    install()
+
+__setup__()
```

### Comparing `slib-sorter-1.2.2/slib_sorter.egg-info/PKG-INFO` & `slib-sorter-1.2.3/slib_sorter.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slib-sorter
-Version: 1.2.2
+Version: 1.2.3
 Summary: A Python package for sorting Sample Libraries
 Home-page: https://github.com/nrdrch/slib-sorter
 Author: Lukas Hübinger
 Author-email: fettkindasindauchoke@gmail.com
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
```

### Comparing `slib-sorter-1.2.2/src/slib_sorter.py` & `slib-sorter-1.2.3/src/slib_sorter.py`

 * *Files 0% similar despite different names*

```diff
@@ -149,17 +149,18 @@
 
 start_time = time.time()
 current_location = path_finder(0)
 source_file = os.path.join(current_location, 'slib_sorter.py')
 icon_path = os.path.join(path_finder(1), 'examples', 'icn.ico')
 
 settings_f = os.path.join(os.environ['USERPROFILE'], 'Documents', 'WindowsPowerShell', 'Scripts', 'slib_sorter', 'settings.json')
+settings = settings_f
 #settings = os.path.join(path_finder(0), 'settings.json')
-with open(settings_f, 'r') as file:
-    settings_f = json.load(file)
+with open(settings, 'r') as file:
+    settings = json.load(file)
 file_path = path1 = os.path.join(os.environ['USERPROFILE'], settings.get('TBPDPath'), settings.get('To Be Processed Directory'))
 path2 = os.path.join(os.environ['USERPROFILE'], settings.get('NOFLDPath'), settings.get("Name Of Top Library Directory"))
 folder_path = path2
 check_dir(path1, path2)
 if settings.get("Run Shell Command On Startup", True):
     CmdOnStartup = settings.get("Command On Startup")
     os.system(CmdOnStartup)
@@ -1036,14 +1037,14 @@
         log_message('Displays Possible Color Settings', f'{settings.get("Statistics Value Color")}', False, True)
         log_message('           -config'+ f'{spacer}', f'{settings.get("Foregroud Color 1")}', False, False)
         log_message('Launch Config File', f'{settings.get("Statistics Value Color")}', False, True)
         log_message('           -help  '+ f'{spacer}', f'{settings.get("Foregroud Color 1")}', False, False)
         log_message('Displays Help', f'{settings.get("Statistics Value Color")}', False, True)
     elif args.config:
         settingsfile = settings_f
-        cmd = "Start "+ settingsfile
+        cmd = "Start "+ f'{settingsfile}'
         os.system(cmd)
     else:
         sort_files(path1, pattern_lists) 
 def __main__():
     print_help_message()
 __main__()
```

