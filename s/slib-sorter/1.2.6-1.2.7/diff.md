# Comparing `tmp/slib-sorter-1.2.6.tar.gz` & `tmp/slib-sorter-1.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slib-sorter-1.2.6.tar", last modified: Sat Jul  8 05:26:24 2023, max compression
+gzip compressed data, was "slib-sorter-1.2.7.tar", last modified: Sat Jul  8 06:06:31 2023, max compression
```

## Comparing `slib-sorter-1.2.6.tar` & `slib-sorter-1.2.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-08 05:26:24.364142 slib-sorter-1.2.6/
--rw-rw-rw-   0        0        0    11558 2023-07-07 20:03:54.000000 slib-sorter-1.2.6/LICENSE
--rw-rw-rw-   0        0        0     2267 2023-07-08 05:26:24.364142 slib-sorter-1.2.6/PKG-INFO
--rw-rw-rw-   0        0        0     1783 2023-07-08 03:49:36.000000 slib-sorter-1.2.6/README.md
--rw-rw-rw-   0        0        0       42 2023-07-08 05:26:24.365116 slib-sorter-1.2.6/setup.cfg
--rw-rw-rw-   0        0        0     3000 2023-07-08 05:25:54.000000 slib-sorter-1.2.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-08 05:26:24.362157 slib-sorter-1.2.6/slib_sorter.egg-info/
--rw-rw-rw-   0        0        0     2267 2023-07-08 05:26:24.000000 slib-sorter-1.2.6/slib_sorter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      273 2023-07-08 05:26:24.000000 slib-sorter-1.2.6/slib_sorter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-08 05:26:24.000000 slib-sorter-1.2.6/slib_sorter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       57 2023-07-08 05:26:24.000000 slib-sorter-1.2.6/slib_sorter.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       17 2023-07-08 05:26:24.000000 slib-sorter-1.2.6/slib_sorter.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-07-08 05:26:24.000000 slib-sorter-1.2.6/slib_sorter.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-08 05:26:24.363142 slib-sorter-1.2.6/src/
--rw-rw-rw-   0        0        0        0 2023-06-28 15:10:46.000000 slib-sorter-1.2.6/src/__init__.py
--rw-rw-rw-   0        0        0    68023 2023-07-08 05:25:21.000000 slib-sorter-1.2.6/src/slib_sorter.py
+drwxrwxrwx   0        0        0        0 2023-07-08 06:06:31.149413 slib-sorter-1.2.7/
+-rw-rw-rw-   0        0        0    11558 2023-07-07 20:03:54.000000 slib-sorter-1.2.7/LICENSE
+-rw-rw-rw-   0        0        0     2249 2023-07-08 06:06:31.148438 slib-sorter-1.2.7/PKG-INFO
+-rw-rw-rw-   0        0        0     1773 2023-07-08 06:05:27.000000 slib-sorter-1.2.7/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-08 06:06:31.149413 slib-sorter-1.2.7/setup.cfg
+-rw-rw-rw-   0        0        0     2992 2023-07-08 06:06:03.000000 slib-sorter-1.2.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-08 06:06:31.139449 slib-sorter-1.2.7/slib_sorter.egg-info/
+-rw-rw-rw-   0        0        0     2249 2023-07-08 06:06:31.000000 slib-sorter-1.2.7/slib_sorter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      273 2023-07-08 06:06:31.000000 slib-sorter-1.2.7/slib_sorter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-08 06:06:31.000000 slib-sorter-1.2.7/slib_sorter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       57 2023-07-08 06:06:31.000000 slib-sorter-1.2.7/slib_sorter.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       17 2023-07-08 06:06:31.000000 slib-sorter-1.2.7/slib_sorter.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-07-08 06:06:31.000000 slib-sorter-1.2.7/slib_sorter.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-08 06:06:31.148438 slib-sorter-1.2.7/src/
+-rw-rw-rw-   0        0        0        0 2023-06-28 15:10:46.000000 slib-sorter-1.2.7/src/__init__.py
+-rw-rw-rw-   0        0        0    68083 2023-07-08 06:02:52.000000 slib-sorter-1.2.7/src/slib_sorter.py
```

### Comparing `slib-sorter-1.2.6/LICENSE` & `slib-sorter-1.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `slib-sorter-1.2.6/PKG-INFO` & `slib-sorter-1.2.7/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: slib-sorter
-Version: 1.2.6
+Version: 1.2.7
 Summary: A Python package for sorting Sample Libraries
 Home-page: https://github.com/nrdrch/slib-sorter
-Author: Lukas Hübinger
+Author: Lukas H
 Author-email: fettkindasindauchoke@gmail.com
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -24,45 +24,45 @@
 ```
 > from GitHub 
 ```
 git clone https://github.com/nrdrch/slib-sorter.git; python3 \slib-sorter\src\slib-sorter.py
 ```
 
 ### Usage 
+> If its the first time running or if the directories don't exist, it will create these on your desktop.
+<img src="https://raw.githubusercontent.com/nrdrch/slib-sorter/main/examples/direxample.png?token=GHSAT0AAAAAACCUPKWOJF3EUJNKTAR7NJSSZEUEOLA">
+
+1. Copy all your files into the 'To Be Sorted' directory
+2. Run the command again and wait for the process to be completed 
 ```
 Slib-Sorter
 ```
+3. Inspect the newly created Sample Library
+> for other options look at:
+```
+Slib-Sorter -help
+```
+
 
 
-> If its the first time running this, it will now have created two directories on your desktop. 
 
 
 
-<img src="https://raw.githubusercontent.com/nrdrch/slib-sorter/main/examples/direxample.png?token=GHSAT0AAAAAACCUPKWOJF3EUJNKTAR7NJSSZEUEOLA">
 
 
 
 <img src="https://raw.githubusercontent.com/nrdrch/slib-sorter/main/examples/outputstatistics.png">
 
 #### Note: Among other things, the names of these two directories & the name of the finished library can be changed in the settings file. 
 ```
 $home\Documents\slib-sorter\settings.json
 ```
 ```
 Slib-Sorter -config
 ```
 
 
-2. Move all your files into the 'To Be Sorted' directory
-3. Run the same command again and wait for the process to be completed 
-4. Inspect the newly created Sample Library located under 'Documents\Sample Library' folder.
-
-
-### Suggestions
-
-
-
 ### Future additions
 - [x] Make any used path easier configurable by the user.
 - [x] Fix minor issues regarding time.
 - [ ] Further improve pattern matching
 - [ ] Apply somewhat simple AI to further boost accuracy, including sorting not based on names but sound.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `slib-sorter-1.2.6/README.md` & `slib-sorter-1.2.7/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -11,45 +11,45 @@
 ```
 > from GitHub 
 ```
 git clone https://github.com/nrdrch/slib-sorter.git; python3 \slib-sorter\src\slib-sorter.py
 ```
 
 ### Usage 
+> If its the first time running or if the directories don't exist, it will create these on your desktop.
+<img src="https://raw.githubusercontent.com/nrdrch/slib-sorter/main/examples/direxample.png?token=GHSAT0AAAAAACCUPKWOJF3EUJNKTAR7NJSSZEUEOLA">
+
+1. Copy all your files into the 'To Be Sorted' directory
+2. Run the command again and wait for the process to be completed 
 ```
 Slib-Sorter
 ```
+3. Inspect the newly created Sample Library
+> for other options look at:
+```
+Slib-Sorter -help
+```
+
 
 
-> If its the first time running this, it will now have created two directories on your desktop. 
 
 
 
-<img src="https://raw.githubusercontent.com/nrdrch/slib-sorter/main/examples/direxample.png?token=GHSAT0AAAAAACCUPKWOJF3EUJNKTAR7NJSSZEUEOLA">
 
 
 
 <img src="https://raw.githubusercontent.com/nrdrch/slib-sorter/main/examples/outputstatistics.png">
 
 #### Note: Among other things, the names of these two directories & the name of the finished library can be changed in the settings file. 
 ```
 $home\Documents\slib-sorter\settings.json
 ```
 ```
 Slib-Sorter -config
 ```
 
 
-2. Move all your files into the 'To Be Sorted' directory
-3. Run the same command again and wait for the process to be completed 
-4. Inspect the newly created Sample Library located under 'Documents\Sample Library' folder.
-
-
-### Suggestions
-
-
-
 ### Future additions
 - [x] Make any used path easier configurable by the user.
 - [x] Fix minor issues regarding time.
 - [ ] Further improve pattern matching
 - [ ] Apply somewhat simple AI to further boost accuracy, including sorting not based on names but sound.
```

### Comparing `slib-sorter-1.2.6/setup.py` & `slib-sorter-1.2.7/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -50,16 +50,16 @@
         with open(settings_file, 'w') as f:
             f.write(default_config)
     else:
         pass
 
     setuptools.setup(
         name="slib-sorter",
-        version="1.2.6",
-        author="Lukas Hübinger",
+        version="1.2.7",
+        author="Lukas H",
         author_email="fettkindasindauchoke@gmail.com",
         description="A Python package for sorting Sample Libraries",
         long_description=long_description,
         long_description_content_type="text/markdown",
         url="https://github.com/nrdrch/slib-sorter",
         packages=setuptools.find_packages(), 
         entry_points={
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `slib-sorter-1.2.6/slib_sorter.egg-info/PKG-INFO` & `slib-sorter-1.2.7/slib_sorter.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: slib-sorter
-Version: 1.2.6
+Version: 1.2.7
 Summary: A Python package for sorting Sample Libraries
 Home-page: https://github.com/nrdrch/slib-sorter
-Author: Lukas Hübinger
+Author: Lukas H
 Author-email: fettkindasindauchoke@gmail.com
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -24,45 +24,45 @@
 ```
 > from GitHub 
 ```
 git clone https://github.com/nrdrch/slib-sorter.git; python3 \slib-sorter\src\slib-sorter.py
 ```
 
 ### Usage 
+> If its the first time running or if the directories don't exist, it will create these on your desktop.
+<img src="https://raw.githubusercontent.com/nrdrch/slib-sorter/main/examples/direxample.png?token=GHSAT0AAAAAACCUPKWOJF3EUJNKTAR7NJSSZEUEOLA">
+
+1. Copy all your files into the 'To Be Sorted' directory
+2. Run the command again and wait for the process to be completed 
 ```
 Slib-Sorter
 ```
+3. Inspect the newly created Sample Library
+> for other options look at:
+```
+Slib-Sorter -help
+```
+
 
 
-> If its the first time running this, it will now have created two directories on your desktop. 
 
 
 
-<img src="https://raw.githubusercontent.com/nrdrch/slib-sorter/main/examples/direxample.png?token=GHSAT0AAAAAACCUPKWOJF3EUJNKTAR7NJSSZEUEOLA">
 
 
 
 <img src="https://raw.githubusercontent.com/nrdrch/slib-sorter/main/examples/outputstatistics.png">
 
 #### Note: Among other things, the names of these two directories & the name of the finished library can be changed in the settings file. 
 ```
 $home\Documents\slib-sorter\settings.json
 ```
 ```
 Slib-Sorter -config
 ```
 
 
-2. Move all your files into the 'To Be Sorted' directory
-3. Run the same command again and wait for the process to be completed 
-4. Inspect the newly created Sample Library located under 'Documents\Sample Library' folder.
-
-
-### Suggestions
-
-
-
 ### Future additions
 - [x] Make any used path easier configurable by the user.
 - [x] Fix minor issues regarding time.
 - [ ] Further improve pattern matching
 - [ ] Apply somewhat simple AI to further boost accuracy, including sorting not based on names but sound.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `slib-sorter-1.2.6/src/slib_sorter.py` & `slib-sorter-1.2.7/src/slib_sorter.py`

 * *Files 0% similar despite different names*

```diff
@@ -77,15 +77,15 @@
             child_path = os.path.join(path, child_path)
             remove_directory_tree(child_path)
     try:
         os.remove(path)
     except OSError as error:
         os.chmod(path, stat.S_IWRITE)
         os.remove(path)
-file_path = path1 = os.path.join(os.environ['USERPROFILE'], settings.get('TBPDPath'), settings.get('To Be Processed Directory'))
+file_path = path1 = os.path.join(os.environ['USERPROFILE'], settings.get(os.path.expanduser('TBPDPath')), settings.get('To Be Processed Directory'))
 path2 = os.path.join(os.environ['USERPROFILE'], settings.get('NOFLDPath'), settings.get("Name Of Top Library Directory"))
 def split_files_in_subdirectories(path2, max_files_per_dir=50):
     for root, dirs, files in os.walk(path2):
         if root == path2:
             continue
         num_files = len(files)
         dir_count = len(dirs)
@@ -126,15 +126,15 @@
 start_time = time.time()
 current_location = path_finder(0)
 source_file = os.path.join(current_location, 'slib_sorter.py')
 settings_f = os.path.join(os.environ['USERPROFILE'], 'Documents', 'WindowsPowerShell', 'Scripts', 'slib_sorter', 'settings.json')
 
 #settings = os.path.join(path_finder(0), 'settings.json')
 
-file_path = path1 = os.path.join(os.environ['USERPROFILE'], settings.get('TBPDPath'), settings.get('To Be Processed Directory'))
+file_path = path1 = os.path.join(os.environ['USERPROFILE'], settings.get(os.path.expanduser('TBPDPath')), settings.get('To Be Processed Directory'))
 path2 = os.path.join(os.environ['USERPROFILE'], settings.get('NOFLDPath'), settings.get("Name Of Top Library Directory"))
 folder_path = path2
 check_dir(path1, path2)
 if settings.get("Run Shell Command On Startup", True):
     CmdOnStartup = settings.get("Command On Startup")
     os.system(CmdOnStartup)
 else:
@@ -965,15 +965,15 @@
     else:
         pass
     def remove_readonly(func, path, _):
         os.chmod(path, stat.S_IWRITE)
         func(path)
     shutil.rmtree(path1, onerror=remove_readonly)
     check_dir(path1)
-temp_content = "\nSorted Library Location:        "+ f"{os.path.join(os.environ['USERPROFILE'], settings.get('NOFLDPath'), settings.get('Name Of Top Library Directory'))}"+ "\nSettings Location:     "+ f"{os.path.join(os.environ['USERPROFILE'], 'Documents', 'WindowsPowerShell', 'Scripts', 'slib_sorter', 'settings.json')}"+ "\nPyhton Script Location:    " f"{os.path.join(current_location, 'slib_sorter.py')}"+ "\nTo Be Sorted Location:    " f"{os.path.join(os.environ['USERPROFILE'], settings.get('TBPDPath'), settings.get('To Be Processed Directory'))}"+ "\nRejected Files Location:     " f"{os.path.join(os.environ['USERPROFILE'], settings.get('RFPath'), settings.get('Rejected Files'))}"
+temp_content = "\nSorted Library Location:        "+ f"{os.path.join(os.environ['USERPROFILE'], settings.get('NOFLDPath'), settings.get('Name Of Top Library Directory'))}"+ "\nSettings Location:     "+ f"{os.path.join(os.environ['USERPROFILE'], 'Documents', 'WindowsPowerShell', 'Scripts', 'slib_sorter', 'settings.json')}"+ "\nPyhton Script Location:    " f"{os.path.join(current_location, 'slib_sorter.py')}"+ "\nTo Be Sorted Location:    " f"{os.path.join(os.environ['USERPROFILE'], settings.get(os.path.expanduser('TBPDPath')), settings.get('To Be Processed Directory'))}"+ "\nRejected Files Location:     " f"{os.path.join(os.environ['USERPROFILE'], settings.get('RFPath'), settings.get('Rejected Files'))}"
 def print_help_message():
     parser = argparse.ArgumentParser()
     parser.add_argument("-paths", action="store_true")
     parser.add_argument("-help", action="store_true")
     parser.add_argument("-colors", action="store_true")
     parser.add_argument("-config", action="store_true")
     temp_file_path = temp_path_file(temp_content)
```

