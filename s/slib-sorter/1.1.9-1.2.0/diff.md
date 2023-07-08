# Comparing `tmp/slib-sorter-1.1.9.tar.gz` & `tmp/slib-sorter-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slib-sorter-1.1.9.tar", last modified: Sat Jul  8 03:26:13 2023, max compression
+gzip compressed data, was "slib-sorter-1.2.0.tar", last modified: Sat Jul  8 04:01:07 2023, max compression
```

## Comparing `slib-sorter-1.1.9.tar` & `slib-sorter-1.2.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-08 03:26:13.963678 slib-sorter-1.1.9/
--rw-rw-rw-   0        0        0    11558 2023-07-07 20:03:54.000000 slib-sorter-1.1.9/LICENSE
--rw-rw-rw-   0        0        0     2291 2023-07-08 03:26:13.963678 slib-sorter-1.1.9/PKG-INFO
--rw-rw-rw-   0        0        0     1807 2023-07-07 20:03:54.000000 slib-sorter-1.1.9/README.md
--rw-rw-rw-   0        0        0       42 2023-07-08 03:26:13.963678 slib-sorter-1.1.9/setup.cfg
--rw-rw-rw-   0        0        0     4368 2023-07-08 03:25:42.000000 slib-sorter-1.1.9/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-08 03:26:13.961693 slib-sorter-1.1.9/slib_sorter.egg-info/
--rw-rw-rw-   0        0        0     2291 2023-07-08 03:26:13.000000 slib-sorter-1.1.9/slib_sorter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      273 2023-07-08 03:26:13.000000 slib-sorter-1.1.9/slib_sorter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-08 03:26:13.000000 slib-sorter-1.1.9/slib_sorter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       57 2023-07-08 03:26:13.000000 slib-sorter-1.1.9/slib_sorter.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       17 2023-07-08 03:26:13.000000 slib-sorter-1.1.9/slib_sorter.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-07-08 03:26:13.000000 slib-sorter-1.1.9/slib_sorter.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-08 03:26:13.962706 slib-sorter-1.1.9/src/
--rw-rw-rw-   0        0        0        0 2023-06-28 15:10:46.000000 slib-sorter-1.1.9/src/__init__.py
--rw-rw-rw-   0        0        0    72626 2023-07-08 03:18:42.000000 slib-sorter-1.1.9/src/slib_sorter.py
+drwxrwxrwx   0        0        0        0 2023-07-08 04:01:07.230651 slib-sorter-1.2.0/
+-rw-rw-rw-   0        0        0    11558 2023-07-07 20:03:54.000000 slib-sorter-1.2.0/LICENSE
+-rw-rw-rw-   0        0        0     2267 2023-07-08 04:01:07.230651 slib-sorter-1.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1783 2023-07-08 03:49:36.000000 slib-sorter-1.2.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-08 04:01:07.230651 slib-sorter-1.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     4368 2023-07-08 04:00:58.000000 slib-sorter-1.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-08 04:01:07.228687 slib-sorter-1.2.0/slib_sorter.egg-info/
+-rw-rw-rw-   0        0        0     2267 2023-07-08 04:01:07.000000 slib-sorter-1.2.0/slib_sorter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      273 2023-07-08 04:01:07.000000 slib-sorter-1.2.0/slib_sorter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-08 04:01:07.000000 slib-sorter-1.2.0/slib_sorter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       57 2023-07-08 04:01:07.000000 slib-sorter-1.2.0/slib_sorter.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       17 2023-07-08 04:01:07.000000 slib-sorter-1.2.0/slib_sorter.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-07-08 04:01:07.000000 slib-sorter-1.2.0/slib_sorter.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-08 04:01:07.229657 slib-sorter-1.2.0/src/
+-rw-rw-rw-   0        0        0        0 2023-06-28 15:10:46.000000 slib-sorter-1.2.0/src/__init__.py
+-rw-rw-rw-   0        0        0    72332 2023-07-08 03:43:41.000000 slib-sorter-1.2.0/src/slib_sorter.py
```

### Comparing `slib-sorter-1.1.9/LICENSE` & `slib-sorter-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `slib-sorter-1.1.9/PKG-INFO` & `slib-sorter-1.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,59 +1,58 @@
 Metadata-Version: 2.1
 Name: slib-sorter
-Version: 1.1.9
+Version: 1.2.0
 Summary: A Python package for sorting Sample Libraries
 Home-page: https://github.com/nrdrch/slib-sorter
 Author: Lukas Hübinger
 Author-email: fettkindasindauchoke@gmail.com
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Sample Library Sorter
 ###### *for now only meant to run on Windows10
 > This script allows you to quickly sort a massive amount of files, any kind you might find in your Sample Library as a Music Producer.
 ##### Audio, Project Files & Plugin Presets (for now just Serum and Massive)
-### Dependecies
-#### 
-[Python](https://www.python.org/downloads/), [termcolor 2.3.0 ](https://pypi.org/project/termcolor/)
+### Dependecies 
+#### [Python](https://www.python.org/downloads/), [termcolor 2.3.0 ](https://pypi.org/project/termcolor/)
+### Installation 
+> from [PyPI](https://pypi.org/)
 ```
-python3 -m pip install --upgrade termcolor
+py -m pip install --upgrade slib-sorter
 ```
-### Installation 
+> from GitHub 
 ```
-git clone https://github.com/nrdrch/slib-sorter.git; python3 .\slib-sorter\src\slib-sorter.py
+git clone https://github.com/nrdrch/slib-sorter.git; python3 \slib-sorter\src\slib-sorter.py
 ```
 
 ### Usage 
-1. Restart your PowerShell.
-2. Run:
 ```
-Start-Sorter
+Slib-Sorter
 ```
 
 
 > If its the first time running this, it will now have created two directories on your desktop. 
 
 
 
 <img src="https://raw.githubusercontent.com/nrdrch/slib-sorter/main/examples/direxample.png?token=GHSAT0AAAAAACCUPKWOJF3EUJNKTAR7NJSSZEUEOLA">
-<img examples/direxample.png>
+
 
 
 <img src="https://raw.githubusercontent.com/nrdrch/slib-sorter/main/examples/outputstatistics.png">
 
 #### Note: Among other things, the names of these two directories & the name of the finished library can be changed in the settings file. 
 ```
 $home\Documents\slib-sorter\settings.json
 ```
 ```
-Start-Sorter -config
+Slib-Sorter -config
 ```
 
 
 2. Move all your files into the 'To Be Sorted' directory
 3. Run the same command again and wait for the process to be completed 
 4. Inspect the newly created Sample Library located under 'Documents\Sample Library' folder.
```

### Comparing `slib-sorter-1.1.9/README.md` & `slib-sorter-1.2.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,46 +1,45 @@
 # Sample Library Sorter
 ###### *for now only meant to run on Windows10
 > This script allows you to quickly sort a massive amount of files, any kind you might find in your Sample Library as a Music Producer.
 ##### Audio, Project Files & Plugin Presets (for now just Serum and Massive)
-### Dependecies
-#### 
-[Python](https://www.python.org/downloads/), [termcolor 2.3.0 ](https://pypi.org/project/termcolor/)
+### Dependecies 
+#### [Python](https://www.python.org/downloads/), [termcolor 2.3.0 ](https://pypi.org/project/termcolor/)
+### Installation 
+> from [PyPI](https://pypi.org/)
 ```
-python3 -m pip install --upgrade termcolor
+py -m pip install --upgrade slib-sorter
 ```
-### Installation 
+> from GitHub 
 ```
-git clone https://github.com/nrdrch/slib-sorter.git; python3 .\slib-sorter\src\slib-sorter.py
+git clone https://github.com/nrdrch/slib-sorter.git; python3 \slib-sorter\src\slib-sorter.py
 ```
 
 ### Usage 
-1. Restart your PowerShell.
-2. Run:
 ```
-Start-Sorter
+Slib-Sorter
 ```
 
 
 > If its the first time running this, it will now have created two directories on your desktop. 
 
 
 
 <img src="https://raw.githubusercontent.com/nrdrch/slib-sorter/main/examples/direxample.png?token=GHSAT0AAAAAACCUPKWOJF3EUJNKTAR7NJSSZEUEOLA">
-<img examples/direxample.png>
+
 
 
 <img src="https://raw.githubusercontent.com/nrdrch/slib-sorter/main/examples/outputstatistics.png">
 
 #### Note: Among other things, the names of these two directories & the name of the finished library can be changed in the settings file. 
 ```
 $home\Documents\slib-sorter\settings.json
 ```
 ```
-Start-Sorter -config
+Slib-Sorter -config
 ```
 
 
 2. Move all your files into the 'To Be Sorted' directory
 3. Run the same command again and wait for the process to be completed 
 4. Inspect the newly created Sample Library located under 'Documents\Sample Library' folder.
```

### Comparing `slib-sorter-1.1.9/setup.py` & `slib-sorter-1.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -79,15 +79,15 @@
         importlib.reload(settings_file)
 def install():
     with open("README.md", "r", encoding="utf-8") as fh:
         long_description = fh.read()
 
     setuptools.setup(
         name="slib-sorter",
-        version="1.1.9",
+        version="1.2.0",
         author="Lukas Hübinger",
         author_email="fettkindasindauchoke@gmail.com",
         description="A Python package for sorting Sample Libraries",
         long_description=long_description,
         long_description_content_type="text/markdown",
         url="https://github.com/nrdrch/slib-sorter",
         packages=setuptools.find_packages(),
```

### Comparing `slib-sorter-1.1.9/slib_sorter.egg-info/PKG-INFO` & `slib-sorter-1.2.0/slib_sorter.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,59 +1,58 @@
 Metadata-Version: 2.1
 Name: slib-sorter
-Version: 1.1.9
+Version: 1.2.0
 Summary: A Python package for sorting Sample Libraries
 Home-page: https://github.com/nrdrch/slib-sorter
 Author: Lukas Hübinger
 Author-email: fettkindasindauchoke@gmail.com
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Sample Library Sorter
 ###### *for now only meant to run on Windows10
 > This script allows you to quickly sort a massive amount of files, any kind you might find in your Sample Library as a Music Producer.
 ##### Audio, Project Files & Plugin Presets (for now just Serum and Massive)
-### Dependecies
-#### 
-[Python](https://www.python.org/downloads/), [termcolor 2.3.0 ](https://pypi.org/project/termcolor/)
+### Dependecies 
+#### [Python](https://www.python.org/downloads/), [termcolor 2.3.0 ](https://pypi.org/project/termcolor/)
+### Installation 
+> from [PyPI](https://pypi.org/)
 ```
-python3 -m pip install --upgrade termcolor
+py -m pip install --upgrade slib-sorter
 ```
-### Installation 
+> from GitHub 
 ```
-git clone https://github.com/nrdrch/slib-sorter.git; python3 .\slib-sorter\src\slib-sorter.py
+git clone https://github.com/nrdrch/slib-sorter.git; python3 \slib-sorter\src\slib-sorter.py
 ```
 
 ### Usage 
-1. Restart your PowerShell.
-2. Run:
 ```
-Start-Sorter
+Slib-Sorter
 ```
 
 
 > If its the first time running this, it will now have created two directories on your desktop. 
 
 
 
 <img src="https://raw.githubusercontent.com/nrdrch/slib-sorter/main/examples/direxample.png?token=GHSAT0AAAAAACCUPKWOJF3EUJNKTAR7NJSSZEUEOLA">
-<img examples/direxample.png>
+
 
 
 <img src="https://raw.githubusercontent.com/nrdrch/slib-sorter/main/examples/outputstatistics.png">
 
 #### Note: Among other things, the names of these two directories & the name of the finished library can be changed in the settings file. 
 ```
 $home\Documents\slib-sorter\settings.json
 ```
 ```
-Start-Sorter -config
+Slib-Sorter -config
 ```
 
 
 2. Move all your files into the 'To Be Sorted' directory
 3. Run the same command again and wait for the process to be completed 
 4. Inspect the newly created Sample Library located under 'Documents\Sample Library' folder.
```

### Comparing `slib-sorter-1.1.9/src/slib_sorter.py` & `slib-sorter-1.2.0/src/slib_sorter.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import os, shutil, stat, argparse
 import time
 import json
 from termcolor import colored
 import os, shutil, stat, tempfile, json, ctypes, importlib
+
 def path_finder(levels_up=0):
     current_dir = os.path.abspath(os.path.dirname(__file__))
     if levels_up > 0:
         for _ in range(levels_up):
             current_dir = os.path.dirname(current_dir)
     return current_dir
 #settings = os.path.join(path_finder(0), 'settings.json')
@@ -21,16 +22,14 @@
 #    settings_file = os.path.join(settings_folder, "settings.json")
 #
 #    
 #    if not os.path.exists(settings_folder):
 #        os.makedirs(settings_folder)
 #    with open(settings_file, 'w') as file:
 #        file.write(default_config)
-
-
 def log_message(message, color, centered=False, newline=True):
     if centered:
         message = message.center(119)
     end = "\n" if newline else ""
     print(colored(message, color), end=end)
 def log_console(file_name, seperator, dest_path, color):
     if settings.get("Show More Console Logs", True):
@@ -104,18 +103,17 @@
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
+        importlib.reload(settings_f)
         #setupfile = os.path.join(path_finder(0), 'setup.py')
-        importlib.reload(settings_file)
 def change_folder_icon(folder_path, icon_path):
     if not os.path.exists(folder_path):
         print("Folder does not exist.")
         return
     folder_path = os.path.abspath(folder_path)
     try:
         ini_path = os.path.join(folder_path, "desktop.ini")
@@ -221,27 +219,24 @@
             json.dump(temp_content, file)
         else:
             file.write(temp_content)
     return file_path
 
 
 
-
-
 start_time = time.time()
 current_location = path_finder(0)
 source_file = os.path.join(current_location, 'slib_sorter.py')
 ps_script(source_file)
 icon_path = os.path.join(path_finder(1), 'examples', 'icn.ico')
-settings_folder = os.path.join(os.environ['USERPROFILE'], 'Documents', 'WindowsPowerShell', 'Scripts', 'slib_sorter')
-settings = os.path.join(settings_folder, "settings.json")
+
 settings_f = os.path.join(os.environ['USERPROFILE'], 'Documents', 'WindowsPowerShell', 'Scripts', 'slib_sorter', 'settings.json')
 #settings = os.path.join(path_finder(0), 'settings.json')
-with open(settings, 'r') as file:
-    settings = json.load(file)
+with open(settings_f, 'r') as file:
+    settings_f = json.load(file)
 file_path = path1 = os.path.join(os.environ['USERPROFILE'], settings.get('TBPDPath'), settings.get('To Be Processed Directory'))
 path2 = os.path.join(os.environ['USERPROFILE'], settings.get('NOFLDPath'), settings.get("Name Of Top Library Directory"))
 folder_path = path2
 check_dir(path1, path2)
 if settings.get("Run Shell Command On Startup", True):
     CmdOnStartup = settings.get("Command On Startup")
     os.system(CmdOnStartup)
```

