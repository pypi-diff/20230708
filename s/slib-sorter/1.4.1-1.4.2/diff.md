# Comparing `tmp/slib-sorter-1.4.1.tar.gz` & `tmp/slib-sorter-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slib-sorter-1.4.1.tar", last modified: Sat Jul  8 10:31:14 2023, max compression
+gzip compressed data, was "slib-sorter-1.4.2.tar", last modified: Sat Jul  8 10:52:06 2023, max compression
```

## Comparing `slib-sorter-1.4.1.tar` & `slib-sorter-1.4.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-08 10:31:14.048305 slib-sorter-1.4.1/
--rw-rw-rw-   0        0        0    11558 2023-07-07 20:03:54.000000 slib-sorter-1.4.1/LICENSE
--rw-rw-rw-   0        0        0     2249 2023-07-08 10:31:14.048305 slib-sorter-1.4.1/PKG-INFO
--rw-rw-rw-   0        0        0     1773 2023-07-08 06:05:27.000000 slib-sorter-1.4.1/README.md
--rw-rw-rw-   0        0        0       42 2023-07-08 10:31:14.049306 slib-sorter-1.4.1/setup.cfg
--rw-rw-rw-   0        0        0     3242 2023-07-08 10:30:35.000000 slib-sorter-1.4.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-08 10:31:14.045334 slib-sorter-1.4.1/slib_sorter.egg-info/
--rw-rw-rw-   0        0        0     2249 2023-07-08 10:31:13.000000 slib-sorter-1.4.1/slib_sorter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      273 2023-07-08 10:31:13.000000 slib-sorter-1.4.1/slib_sorter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-08 10:31:13.000000 slib-sorter-1.4.1/slib_sorter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       57 2023-07-08 10:31:13.000000 slib-sorter-1.4.1/slib_sorter.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       17 2023-07-08 10:31:13.000000 slib-sorter-1.4.1/slib_sorter.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-07-08 10:31:13.000000 slib-sorter-1.4.1/slib_sorter.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-08 10:31:14.047306 slib-sorter-1.4.1/src/
--rw-rw-rw-   0        0        0        0 2023-06-28 15:10:46.000000 slib-sorter-1.4.1/src/__init__.py
--rw-rw-rw-   0        0        0    67316 2023-07-08 10:29:41.000000 slib-sorter-1.4.1/src/slib_sorter.py
+drwxrwxrwx   0        0        0        0 2023-07-08 10:52:06.157323 slib-sorter-1.4.2/
+-rw-rw-rw-   0        0        0    11558 2023-07-07 20:03:54.000000 slib-sorter-1.4.2/LICENSE
+-rw-rw-rw-   0        0        0     2249 2023-07-08 10:52:06.157323 slib-sorter-1.4.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1773 2023-07-08 06:05:27.000000 slib-sorter-1.4.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-08 10:52:06.157323 slib-sorter-1.4.2/setup.cfg
+-rw-rw-rw-   0        0        0     3242 2023-07-08 10:52:00.000000 slib-sorter-1.4.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-08 10:52:06.146333 slib-sorter-1.4.2/slib_sorter.egg-info/
+-rw-rw-rw-   0        0        0     2249 2023-07-08 10:52:06.000000 slib-sorter-1.4.2/slib_sorter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      273 2023-07-08 10:52:06.000000 slib-sorter-1.4.2/slib_sorter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-08 10:52:06.000000 slib-sorter-1.4.2/slib_sorter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       57 2023-07-08 10:52:06.000000 slib-sorter-1.4.2/slib_sorter.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       17 2023-07-08 10:52:06.000000 slib-sorter-1.4.2/slib_sorter.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-07-08 10:52:06.000000 slib-sorter-1.4.2/slib_sorter.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-08 10:52:06.156298 slib-sorter-1.4.2/src/
+-rw-rw-rw-   0        0        0        0 2023-06-28 15:10:46.000000 slib-sorter-1.4.2/src/__init__.py
+-rw-rw-rw-   0        0        0    67728 2023-07-08 10:51:19.000000 slib-sorter-1.4.2/src/slib_sorter.py
```

### Comparing `slib-sorter-1.4.1/LICENSE` & `slib-sorter-1.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `slib-sorter-1.4.1/PKG-INFO` & `slib-sorter-1.4.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slib-sorter
-Version: 1.4.1
+Version: 1.4.2
 Summary: A Python package for sorting Sample Libraries
 Home-page: https://github.com/nrdrch/slib-sorter
 Author: Lukas H
 Author-email: fettkindasindauchoke@gmail.com
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
```

### Comparing `slib-sorter-1.4.1/README.md` & `slib-sorter-1.4.2/README.md`

 * *Files identical despite different names*

### Comparing `slib-sorter-1.4.1/setup.py` & `slib-sorter-1.4.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,15 +56,15 @@
 ''' 
         f.write(default_config)
     else:
         pass
 
     setuptools.setup(
         name="slib-sorter",
-        version="1.4.1",
+        version="1.4.2",
         author="Lukas H",
         author_email="fettkindasindauchoke@gmail.com",
         description="A Python package for sorting Sample Libraries",
         long_description=long_description,
         long_description_content_type="text/markdown",
         url="https://github.com/nrdrch/slib-sorter",
         packages=setuptools.find_packages(),
```

### Comparing `slib-sorter-1.4.1/slib_sorter.egg-info/PKG-INFO` & `slib-sorter-1.4.2/slib_sorter.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slib-sorter
-Version: 1.4.1
+Version: 1.4.2
 Summary: A Python package for sorting Sample Libraries
 Home-page: https://github.com/nrdrch/slib-sorter
 Author: Lukas H
 Author-email: fettkindasindauchoke@gmail.com
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
```

### Comparing `slib-sorter-1.4.1/src/slib_sorter.py` & `slib-sorter-1.4.2/src/slib_sorter.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,10 @@
-import os, shutil, stat, argparse
-import time
-import json
+import os, shutil, stat, tempfile, json, ctypes, argparse, time, sys, subprocess
 from termcolor import colored
-import os, shutil, stat, tempfile, json, ctypes, importlib
+
 
 
 
 def join_corrected_paths(settings):
     # Load the settings from the file
     with open(settings, "r") as file:
         settings = json.load(file)
@@ -56,15 +54,15 @@
     end = "\n" if newline else ""
     print(colored(message, color), end=end)
 
 def log_console(file_name, seperator, dest_path, color):
     if settings.get("Show More Console Logs", True):
         log_message(f'{file_name}', f'{color}', False, False)
         log_message(f'{seperator}', f'{j_clrs.get("Foreground Color 2")}', False, False)
-        log_message(f' {dest_path}', f'{j_clrs.get("Foreground Color 1")}', False, True)
+        log_message(f'{dest_path}', f'{j_clrs.get("Foreground Color 1")}', False, True)
     else:
         pass
 
 
 def organize_files_by_extension(path):
     if not os.path.isdir(path):
         raise Exception("The path provided is not a directory.")
@@ -233,747 +231,747 @@
             file_extension = file_extension[1:]
             if file_extension in audio_exts:
                 if any(pattern in file_name for pattern in pattern_lists.get("DrumPercs", [])):
                     total += 1
                     num_succeeded += 1
                     dest_path = os.path.join(j_paths.get('Name Of Top Library Directory'), 'Samples', 'Drum', 'Percussion')
                     if settings.get("Show More Console Logs", True):
-                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', j_clrs.get('Successfully Sorted File Color'))
+                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', f'{j_clrs.get("Successfully Sorted File Color")}')
                     else:
                         pass
                 elif any(pattern in file_name for pattern in pattern_lists.get("DrumLoops", [])):
                     total += 1
                     num_succeeded += 1
                     dest_path = os.path.join(j_paths.get('Name Of Top Library Directory'), 'Samples', 'Drum', 'Loops')
                     if settings.get("Show More Console Logs", True):
-                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', j_clrs.get('Successfully Sorted File Color'))
+                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', f'{j_clrs.get("Successfully Sorted File Color")}')
                     else:
                         pass
                 elif any(pattern in file_name for pattern in pattern_lists.get("VocalLoops", [])):
                     total += 1
                     num_succeeded += 1
                     dest_path = os.path.join(j_paths.get('Name Of Top Library Directory'), 'Samples', 'Voice', 'Loops')
                     if settings.get("Show More Console Logs", True):
-                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', j_clrs.get('Successfully Sorted File Color'))
+                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', f'{j_clrs.get("Successfully Sorted File Color")}')
                     else:
                         pass
                 elif any(pattern in file_name for pattern in pattern_lists.get("MelodicLoops", [])):
                     total += 1
                     num_succeeded += 1
                     dest_path = os.path.join(j_paths.get('Name Of Top Library Directory'), 'Samples', 'Melodic', 'Loops')
                     if settings.get("Show More Console Logs", True):
-                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', j_clrs.get('Successfully Sorted File Color'))
+                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', f'{j_clrs.get("Successfully Sorted File Color")}')
                     else:
                         pass
                 elif any(pattern in file_name for pattern in pattern_lists.get("BassLoops", [])):
                     total += 1
                     num_succeeded += 1
                     dest_path = os.path.join(j_paths.get('Name Of Top Library Directory'), 'Samples', 'Melodic', 'Bass', 'Loops')
                     if settings.get("Show More Console Logs", True):
-                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', j_clrs.get('Successfully Sorted File Color'))
+                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', f'{j_clrs.get("Successfully Sorted File Color")}')
                     else:
                         pass
                 elif any(pattern in file_name for pattern in pattern_lists.get("DrumKick", [])):
                     total += 1
                     num_succeeded += 1
                     dest_path = os.path.join(j_paths.get('Name Of Top Library Directory'), 'Samples', 'Drum', 'Kicks')
                     if settings.get("Show More Console Logs", True):
-                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', j_clrs.get('Successfully Sorted File Color'))
+                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', f'{j_clrs.get("Successfully Sorted File Color")}')
                     else:
                         pass
                 elif any(pattern in file_name for pattern in pattern_lists.get("DrumSnare", [])):
                     total += 1
                     num_succeeded += 1
                     dest_path = os.path.join(j_paths.get('Name Of Top Library Directory'), 'Samples', 'Drum', 'Snares')
                     if settings.get("Show More Console Logs", True):
-                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', j_clrs.get('Successfully Sorted File Color'))
+                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', f'{j_clrs.get("Successfully Sorted File Color")}')
                     else:
                         pass
                 elif any(pattern in file_name for pattern in pattern_lists.get("DrumShakers", [])):
                     total += 1
                     num_succeeded += 1
                     dest_path = os.path.join(j_paths.get('Name Of Top Library Directory'), 'Samples', 'Drum', 'Shakers')
                     if settings.get("Show More Console Logs", True):
-                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', j_clrs.get('Successfully Sorted File Color'))
+                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', f'{j_clrs.get("Successfully Sorted File Color")}')
                     else:
                         pass
                 elif any(pattern in file_name for pattern in pattern_lists.get("Synth", [])):
                     total += 1
                     num_succeeded += 1
                     dest_path = os.path.join(j_paths.get('Name Of Top Library Directory'), 'Samples', 'Melodic', 'Synths')
                     if settings.get("Show More Console Logs", True):
-                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', j_clrs.get('Successfully Sorted File Color'))
+                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', f'{j_clrs.get("Successfully Sorted File Color")}')
                     else:
                         pass
                 elif any(pattern in file_name for pattern in pattern_lists.get("Plucks", [])):
                     total += 1
                     num_succeeded += 1
                     dest_path = os.path.join(j_paths.get('Name Of Top Library Directory'), 'Samples', 'Melodic', 'Plucks')
                     if settings.get("Show More Console Logs", True):
-                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', j_clrs.get('Successfully Sorted File Color'))
+                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', f'{j_clrs.get("Successfully Sorted File Color")}')
                     else:
                         pass
                 elif any(pattern in file_name for pattern in pattern_lists.get("Bass", [])):
                     total += 1
                     num_succeeded += 1
                     dest_path = os.path.join(j_paths.get('Name Of Top Library Directory'), 'Samples', 'Melodic', 'Bass')
                     if settings.get("Show More Console Logs", "True"):
-                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', j_clrs.get('Successfully Sorted File Color'))
+                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', f'{j_clrs.get("Successfully Sorted File Color")}')
                     else:
                         pass
                 elif any(pattern in file_name for pattern in pattern_lists.get("Keys", [])):
                     total += 1
                     num_succeeded += 1
                     dest_path = os.path.join(j_paths.get('Name Of Top Library Directory'), 'Samples', 'Melodic', 'Keys')
                     if settings.get("Show More Console Logs", True):
-                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', j_clrs.get('Successfully Sorted File Color'))
+                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', f'{j_clrs.get("Successfully Sorted File Color")}')
                     else:
                         pass
                 elif any(pattern in file_name for pattern in pattern_lists.get("Lead", [])):
                     total += 1
                     num_succeeded += 1
                     dest_path = os.path.join(j_paths.get('Name Of Top Library Directory'), 'Samples', 'Melodic', 'Lead')
                     if settings.get("Show More Console Logs", True):
-                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', j_clrs.get('Successfully Sorted File Color'))
+                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', f'{j_clrs.get("Successfully Sorted File Color")}')
                     else:
                         pass
                 elif any(pattern in file_name for pattern in pattern_lists.get("Pad", [])):
                     total += 1
                     num_succeeded += 1
                     dest_path = os.path.join(j_paths.get('Name Of Top Library Directory'), 'Samples', 'Melodic', 'Pad')
                     if settings.get("Show More Console Logs", True):
-                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', j_clrs.get('Successfully Sorted File Color'))
+                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', f'{j_clrs.get("Successfully Sorted File Color")}')
                     else:
                         pass
                 elif any(pattern in file_name for pattern in pattern_lists.get("Synth", [])):
                     total += 1
                     num_succeeded += 1
                     dest_path = os.path.join(j_paths.get('Name Of Top Library Directory'), 'Samples', 'Melodic', 'Synth')
                     if settings.get("Show More Console Logs", True):
-                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', j_clrs.get('Successfully Sorted File Color'))
+                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', f'{j_clrs.get("Successfully Sorted File Color")}')
                     else:
                         pass
                 elif any(pattern in file_name for pattern in pattern_lists.get("Wind", [])):
                     total += 1
                     num_succeeded += 1
                     dest_path = os.path.join(j_paths.get('Name Of Top Library Directory'), 'Samples', 'Melodic', 'Wind')
                     if settings.get("Show More Console Logs", True):
-                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', j_clrs.get('Successfully Sorted File Color'))
+                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', f'{j_clrs.get("Successfully Sorted File Color")}')
                     else:
                         pass
                 elif any(pattern in file_name for pattern in pattern_lists.get("String", [])):
                     total += 1
                     num_succeeded += 1
                     dest_path = os.path.join(j_paths.get('Name Of Top Library Directory'), 'Samples', 'Melodic', 'String')
                     if settings.get("Show More Console Logs", True):
-                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', j_clrs.get('Successfully Sorted File Color'))
+                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', f'{j_clrs.get("Successfully Sorted File Color")}')
                     else:
                         pass
                 elif any(pattern in file_name for pattern in pattern_lists.get("BassHits", [])):
                     total += 1
                     num_succeeded += 1
                     dest_path = os.path.join(j_paths.get('Name Of Top Library Directory'), 'Samples', 'Melodic', 'Bass', 'Hits')
                     if settings.get("Show More Console Logs", True):
-                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', j_clrs.get('Successfully Sorted File Color'))
+                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', f'{j_clrs.get("Successfully Sorted File Color")}')
                     else:
                         pass
                 elif any(pattern in file_name for pattern in pattern_lists.get("Riser", [])):
                     total += 1
                     num_succeeded += 1
                     dest_path = os.path.join(j_paths.get('Name Of Top Library Directory'), 'Samples', 'FX', 'Riser')
                     if settings.get("Show More Console Logs", True):
-                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', j_clrs.get('Successfully Sorted File Color'))
+                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', f'{j_clrs.get("Successfully Sorted File Color")}')
                     else:
                         pass
                 elif any(pattern in file_name for pattern in pattern_lists.get("Noise", [])):
                     total += 1
                     num_succeeded += 1
                     dest_path = os.path.join(j_paths.get('Name Of Top Library Directory'), 'Samples', 'FX', 'Noise')
                     if settings.get("Show More Console Logs", True):
-                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', j_clrs.get('Successfully Sorted File Color'))
+                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', f'{j_clrs.get("Successfully Sorted File Color")}')
                     else:
                         pass
                 elif any(pattern in file_name for pattern in pattern_lists.get("Siren", [])):
                     total += 1
                     num_succeeded += 1
                     dest_path = os.path.join(j_paths.get('Name Of Top Library Directory'), 'Samples', 'FX', 'Siren')
                     if settings.get("Show More Console Logs", True):
-                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', j_clrs.get('Successfully Sorted File Color'))
+                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', f'{j_clrs.get("Successfully Sorted File Color")}')
                     else:
                         pass
                 elif any(pattern in file_name for pattern in pattern_lists.get("Vinyl", [])):
                     total += 1
                     num_succeeded += 1
                     dest_path = os.path.join(j_paths.get('Name Of Top Library Directory'), 'Samples', 'FX', 'Vinyl')
                     if settings.get("Show More Console Logs", True):
-                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', j_clrs.get('Successfully Sorted File Color'))
+                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', f'{j_clrs.get("Successfully Sorted File Color")}')
                     else:
                         pass
                 elif any(pattern in file_name for pattern in pattern_lists.get("Impact", [])):
                     total += 1
                     num_succeeded += 1
                     dest_path = os.path.join(j_paths.get('Name Of Top Library Directory'), 'Samples', 'FX', 'Impact')
                     if settings.get("Show More Console Logs", True):
-                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', j_clrs.get('Successfully Sorted File Color'))
+                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', f'{j_clrs.get("Successfully Sorted File Color")}')
                     else:
                         pass
                 elif any(pattern in file_name for pattern in pattern_lists.get("FX", [])):
                     total += 1
                     num_succeeded += 1
                     dest_path = os.path.join(j_paths.get('Name Of Top Library Directory'), 'Samples', 'FX')
                     if settings.get("Show More Console Logs", True):
-                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', j_clrs.get('Successfully Sorted File Color'))
+                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', f'{j_clrs.get("Successfully Sorted File Color")}')
                     else:
                         pass
                 elif any(pattern in file_name for pattern in pattern_lists.get("DrumClap", [])):
                     total += 1
                     num_succeeded += 1
                     dest_path = os.path.join(j_paths.get('Name Of Top Library Directory'), 'Samples', 'Drum', 'Claps')
                     if settings.get("Show More Console Logs", True):
-                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', j_clrs.get('Successfully Sorted File Color'))
+                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', f'{j_clrs.get("Successfully Sorted File Color")}')
                     else:
                         pass
                 elif any(pattern in file_name for pattern in pattern_lists.get("DrumHats", [])):
                     total += 1
                     num_succeeded += 1
                     dest_path = os.path.join(j_paths.get('Name Of Top Library Directory'), 'Samples', 'Drum', 'Hats')
                     if settings.get("Show More Console Logs", True):
-                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', j_clrs.get('Successfully Sorted File Color'))
+                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', f'{j_clrs.get("Successfully Sorted File Color")}')
                     else:
                         pass
                 elif any(pattern in file_name for pattern in pattern_lists.get("DrumTom", [])):
                     total += 1
                     num_succeeded += 1
                     dest_path = os.path.join(j_paths.get('Name Of Top Library Directory'), 'Samples', 'Drum', 'Toms')
                     if settings.get("Show More Console Logs", True):
-                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', j_clrs.get('Successfully Sorted File Color'))
+                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', f'{j_clrs.get("Successfully Sorted File Color")}')
                     else:
                         pass
                 elif any(pattern in file_name for pattern in pattern_lists.get("808", [])):
                     total += 1
                     num_succeeded += 1
                     dest_path = os.path.join(j_paths.get('Name Of Top Library Directory'), 'Samples', 'Drum', '808')
                     if settings.get("Show More Console Logs", True):
-                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', j_clrs.get('Successfully Sorted File Color'))
+                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', f'{j_clrs.get("Successfully Sorted File Color")}')
                     else:
                         pass
                 elif any(pattern in file_name for pattern in pattern_lists.get("DrumPercs", [])):
                     total += 1
                     num_succeeded += 1
                     dest_path = os.path.join(j_paths.get('Name Of Top Library Directory'), 'Samples', 'Drum', 'Percussion')
                     if settings.get("Show More Console Logs", True):
-                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', j_clrs.get('Successfully Sorted File Color'))
+                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', f'{j_clrs.get("Successfully Sorted File Color")}')
                     else:
                         pass
                 elif any(pattern in file_name for pattern in pattern_lists.get("Percs", [])):
                     total += 1
                     num_succeeded += 1
                     dest_path = os.path.join(j_paths.get('Name Of Top Library Directory'), 'Samples', 'Drum', 'Percussion')
                     if settings.get("Show More Console Logs", True):
-                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', j_clrs.get('Successfully Sorted File Color'))
+                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', f'{j_clrs.get("Successfully Sorted File Color")}')
                     else:
                         pass
                 elif any(pattern in file_name for pattern in pattern_lists.get("DrumHats", [])):
                     total += 1
                     num_succeeded += 1
                     dest_path = os.path.join(j_paths.get('Name Of Top Library Directory'), 'Samples', 'Drum', 'Hats')
                     if settings.get("Show More Console Logs", True):
-                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', j_clrs.get('Successfully Sorted File Color'))
+                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', f'{j_clrs.get("Successfully Sorted File Color")}')
                     else:
                         pass
                 elif any(pattern in file_name for pattern in pattern_lists.get("DrumHatsOpen", [])):
                     total += 1
                     num_succeeded += 1
                     dest_path = os.path.join(j_paths.get('Name Of Top Library Directory'), 'Samples', 'Drum', 'Hats', 'Open')
                     if settings.get("Show More Console Logs", True):
-                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', j_clrs.get('Successfully Sorted File Color'))
+                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', f'{j_clrs.get("Successfully Sorted File Color")}')
                     else:
                         pass
                 elif any(pattern in file_name for pattern in pattern_lists.get("DrumHatsClosed", [])):
                     total += 1
                     num_succeeded += 1
                     dest_path = os.path.join(j_paths.get('Name Of Top Library Directory'), 'Samples', 'Drum', 'Hats', 'Closed')
                     if settings.get("Show More Console Logs", True):
-                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', j_clrs.get('Successfully Sorted File Color'))
+                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', f'{j_clrs.get("Successfully Sorted File Color")}')
                     else:
                         pass
                 elif any(pattern in file_name for pattern in pattern_lists.get("Vox", [])):
                     total += 1
                     num_succeeded += 1
                     dest_path = os.path.join(j_paths.get('Name Of Top Library Directory'), 'Samples', 'Voice', 'Vox')
                     if settings.get("Show More Console Logs", True):
-                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', j_clrs.get('Successfully Sorted File Color'))
+                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', f'{j_clrs.get("Successfully Sorted File Color")}')
                     else:
                         pass
                 elif any(pattern in file_name for pattern in pattern_lists.get("Vocal Chop", [])):
                     total += 1
                     num_succeeded += 1
                     dest_path = os.path.join(j_paths.get('Name Of Top Library Directory'), 'Samples', 'Voice', 'Vocal Chop')
                     if settings.get("Show More Console Logs", True):
-                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', j_clrs.get('Successfully Sorted File Color'))
+                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', f'{j_clrs.get("Successfully Sorted File Color")}')
                     else:
                         pass
                 elif any(pattern in file_name for pattern in pattern_lists.get("Vocal Arp", [])):
                     total += 1
                     num_succeeded += 1
                     dest_path = os.path.join(j_paths.get('Name Of Top Library Directory'), 'Samples', 'Voice', 'Vocal Arp')
                     if settings.get("Show More Console Logs", True):
-                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', j_clrs.get('Successfully Sorted File Color'))
+                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', f'{j_clrs.get("Successfully Sorted File Color")}')
                     else:
                         pass
                 elif any(pattern in file_name for pattern in pattern_lists.get("Hooks", [])):
                     total += 1
                     num_succeeded += 1
                     dest_path = os.path.join(j_paths.get('Name Of Top Library Directory'), 'Samples', 'Voice', 'Hooks')
                     if settings.get("Show More Console Logs", True):
-                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', j_clrs.get('Successfully Sorted File Color'))
+                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', f'{j_clrs.get("Successfully Sorted File Color")}')
                     else:
                         pass
                 elif any(pattern in file_name for pattern in pattern_lists.get("Screams", [])):
                     total += 1
                     num_succeeded += 1
                     dest_path = os.path.join(j_paths.get('Name Of Top Library Directory'), 'Samples', 'Voice', 'Scream')
                     if settings.get("Show More Console Logs", True):
-                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', j_clrs.get('Successfully Sorted File Color'))
+                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', f'{j_clrs.get("Successfully Sorted File Color")}')
                     else:
                         pass
                 elif any(pattern in file_name for pattern in pattern_lists.get("Chants", [])):
                     total += 1
                     num_succeeded += 1
                     dest_path = os.path.join(j_paths.get('Name Of Top Library Directory'), 'Samples', 'Voice', 'Chant')
                     if settings.get("Show More Console Logs", True):
-                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', j_clrs.get('Successfully Sorted File Color'))
+                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', f'{j_clrs.get("Successfully Sorted File Color")}')
                     else:
                         pass
                 elif any(pattern in file_name for pattern in pattern_lists.get("Phrases", [])):
                     total += 1
                     num_succeeded += 1
                     dest_path = os.path.join(j_paths.get('Name Of Top Library Directory'), 'Samples', 'Voice', 'Phrases')
                     if settings.get("Show More Console Logs", True):
-                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', j_clrs.get('Successfully Sorted File Color'))
+                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', f'{j_clrs.get("Successfully Sorted File Color")}')
                     else:
                         pass
                 elif any(pattern in file_name for pattern in pattern_lists.get("Voice", [])):
                     total += 1
                     num_succeeded += 1
                     dest_path = os.path.join(j_paths.get('Name Of Top Library Directory'), 'Samples', 'Voice')
                     if settings.get("Show More Console Logs", True):
-                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', j_clrs.get('Successfully Sorted File Color'))
+                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', f'{j_clrs.get("Successfully Sorted File Color")}')
                     else:
                         pass
                 elif any(pattern in file_name for pattern in pattern_lists.get("Atmos", [])):
                     total += 1
                     num_succeeded += 1
                     dest_path = os.path.join(j_paths.get('Name Of Top Library Directory'), 'Samples', 'Atmos')
                     if settings.get("Show More Console Logs", True):
-                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', j_clrs.get('Successfully Sorted File Color'))
+                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', f'{j_clrs.get("Successfully Sorted File Color")}')
                     else:
                         pass
                 else:
                     dest_path = os.path.join(j_paths.get('Name Of Top Library Directory'), 'Samples', 'Unsorted')
                     total += 1
                     num_failed += 1
                     if settings.get("Show More Console Logs", True):
-                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', j_clrs.get('Unsorted File Color'))
+                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', f'{j_clrs.get("Unsorted File Color")}')
                     else:
                         pass   
             elif file_extension in ["fxp"]:
                 if any(pattern in file_name for pattern in pattern_lists.get("Bass", [])):
                     total += 1
                     num_succeeded += 1
                     dest_path = os.path.join(j_paths.get('Name Of Top Library Directory'), 'Presets', 'Serum Presets', 'Bass')
                     if settings.get("Show More Console Logs", True):
-                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', j_clrs.get('Successfully Sorted File Color'))
+                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', f'{j_clrs.get("Successfully Sorted File Color")}')
                     else:
                         pass
                 elif any(pattern in file_name for pattern in pattern_lists.get("Keys", [])):
                     total += 1
                     num_succeeded += 1
                     dest_path = os.path.join(j_paths.get('Name Of Top Library Directory'), 'Presets', 'Serum Presets', 'Keys')
                     if settings.get("Show More Console Logs", True):
-                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', j_clrs.get('Successfully Sorted File Color'))
+                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', f'{j_clrs.get("Successfully Sorted File Color")}')
                     else:
                         pass
                 elif any(pattern in file_name for pattern in pattern_lists.get("Plucks", [])):
                     total += 1
                     num_succeeded += 1
                     dest_path = os.path.join(j_paths.get('Name Of Top Library Directory'), 'Presets', 'Serum Presets', 'Plucks')
                     if settings.get("Show More Console Logs", True):
-                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', j_clrs.get('Successfully Sorted File Color'))
+                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', f'{j_clrs.get("Successfully Sorted File Color")}')
                     else:
                         pass
                 elif any(pattern in file_name for pattern in pattern_lists.get("Lead", [])):
                     total += 1
                     num_succeeded += 1
                     dest_path = os.path.join(j_paths.get('Name Of Top Library Directory'), 'Presets', 'Serum Presets' ,'Lead')
                     if settings.get("Show More Console Logs", True):
-                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', j_clrs.get('Successfully Sorted File Color'))
+                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', f'{j_clrs.get("Successfully Sorted File Color")}')
                     else:
                         pass
                 elif any(pattern in file_name for pattern in pattern_lists.get("Synth", [])):
                     total += 1
                     num_succeeded += 1
                     dest_path = os.path.join(j_paths.get('Name Of Top Library Directory'), 'Presets', 'Serum Presets' ,'Synth')
                     if settings.get("Show More Console Logs", True):
-                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', j_clrs.get('Successfully Sorted File Color'))
+                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', f'{j_clrs.get("Successfully Sorted File Color")}')
                     else:
                         pass
                 elif any(pattern in file_name for pattern in pattern_lists.get("Pad", [])):
                     total += 1
                     num_succeeded += 1
                     dest_path = os.path.join(j_paths.get('Name Of Top Library Directory'), 'Presets', 'Serum Presets' ,'Pad')
                     if settings.get("Show More Console Logs", True):
-                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', j_clrs.get('Successfully Sorted File Color'))
+                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', f'{j_clrs.get("Successfully Sorted File Color")}')
                     else:
                         pass
                 elif any(pattern in file_name for pattern in pattern_lists.get("FX", [])):
                     total += 1
                     num_succeeded += 1
                     dest_path = os.path.join(j_paths.get('Name Of Top Library Directory'), 'Presets', 'Serum Presets', 'FX')
                     if settings.get("Show More Console Logs", True):
-                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', j_clrs.get('Successfully Sorted File Color'))
+                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', f'{j_clrs.get("Successfully Sorted File Color")}')
                     else:
                         pass
                 elif any(pattern in file_name for pattern in pattern_lists.get("Atmos", [])):
                     total += 1
                     num_succeeded += 1
                     dest_path = os.path.join(j_paths.get('Name Of Top Library Directory'), 'Presets', 'Serum Presets', 'Atmos')
                     if settings.get("Show More Console Logs"):
-                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', j_clrs.get('Successfully Sorted File Color'))
+                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', f'{j_clrs.get("Successfully Sorted File Color")}')
                 elif any(pattern in file_name for pattern in pattern_lists.get("Voice", [])):
                     total += 1
                     num_succeeded += 1
                     dest_path = os.path.join(j_paths.get('Name Of Top Library Directory'), 'Presets', 'Serum Presets', 'Voice')
                     if settings.get("Show More Console Logs", True):
-                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', j_clrs.get('Successfully Sorted File Color'))
+                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', f'{j_clrs.get("Successfully Sorted File Color")}')
                     else:
                         pass
                 elif any(pattern in file_name for pattern in pattern_lists.get("808", [])):
                     total += 1
                     num_succeeded += 1
                     dest_path = os.path.join(j_paths.get('Name Of Top Library Directory'), 'Presets', 'Serum Presets', '808')
                     if settings.get("Show More Console Logs", True):
-                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', j_clrs.get('Successfully Sorted File Color'))
+                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', f'{j_clrs.get("Successfully Sorted File Color")}')
                     else:
                         pass
                 elif any(pattern in file_name for pattern in pattern_lists.get("DrumPresets", [])):
                     total += 1
                     num_succeeded += 1
                     dest_path = os.path.join(j_paths.get('Name Of Top Library Directory'), 'Presets', 'Serum Presets', 'DrumPresets')
                     if settings.get("Show More Console Logs", True):
-                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', j_clrs.get('Successfully Sorted File Color'))
+                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', f'{j_clrs.get("Successfully Sorted File Color")}')
                     else:
                         pass
                 else:
                     dest_path = os.path.join(j_paths.get('Name Of Top Library Directory'), 'Presets', 'Serum Presets', 'Unsorted')
                     total += 1
                     num_failed += 1
                     if settings.get("Show More Console Logs", True):
-                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', j_clrs.get('Successfully Sorted File Color'))
+                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', f'{j_clrs.get("Successfully Sorted File Color")}')
                     else:
                         pass
             elif file_extension in ["nki"]:
                 total += 1
                 num_succeeded += 1
                 dest_path = os.path.join(j_paths.get('Name Of Top Library Directory'), 'Presets', 'Native Instruments')
                 if settings.get("Show More Console Logs", True):
-                    log_console(f'{file_name}', f'{seperator}', f'{dest_path}', j_clrs.get('Successfully Sorted File Color'))
+                    log_console(f'{file_name}', f'{seperator}', f'{dest_path}', f'{j_clrs.get("Successfully Sorted File Color")}')
                 else:
                     pass
             elif file_extension in ["mid"]:
                 if any(pattern in file_name for pattern in pattern_lists.get("DrumSnare", [])):
                     total += 1
                     num_succeeded += 1
                     dest_path = os.path.join(j_paths.get('Name Of Top Library Directory'), 'Midi', 'Drum', 'Snares')
                     if settings.get("Show More Console Logs", True):
-                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', j_clrs.get('Successfully Sorted File Color'))
+                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', f'{j_clrs.get("Successfully Sorted File Color")}')
                     else:
                         pass
                 elif any(pattern in file_name for pattern in pattern_lists.get("DrumClap", [])):
                     total += 1
                     num_succeeded += 1
                     dest_path = os.path.join(j_paths.get('Name Of Top Library Directory'), 'Midi', 'Drum', 'Claps')
                     if settings.get("Show More Console Logs", True):
-                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', j_clrs.get('Successfully Sorted File Color'))
+                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', f'{j_clrs.get("Successfully Sorted File Color")}')
                     else:
                         pass
                 elif any(pattern in file_name for pattern in pattern_lists.get("Melodic", [])):
                     total += 1
                     num_succeeded += 1
                     dest_path = os.path.join(j_paths.get('Name Of Top Library Directory'), 'Midi', 'Melodic')
                 elif any(pattern in file_name for pattern in pattern_lists.get("DrumTom", [])):
                     total += 1
                     num_succeeded += 1
                     dest_path = os.path.join(j_paths.get('Name Of Top Library Directory'), 'Midi', 'Drum', 'Toms')
                     if settings.get("Show More Console Logs", True):
-                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', j_clrs.get('Successfully Sorted File Color'))
+                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', f'{j_clrs.get("Successfully Sorted File Color")}')
                     else:
                         pass
                 elif any(pattern in file_name for pattern in pattern_lists.get("808", [])):
                     total += 1
                     num_succeeded += 1
                     dest_path = os.path.join(j_paths.get('Name Of Top Library Directory'), 'Midi', 'Drum', '808')
                     if settings.get("Show More Console Logs", True):
-                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', j_clrs.get('Successfully Sorted File Color'))
+                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', f'{j_clrs.get("Successfully Sorted File Color")}')
                     else:
                         pass
                 elif any(pattern in file_name for pattern in pattern_lists.get("DrumKick", [])):
                     total += 1
                     num_succeeded += 1
                     dest_path = os.path.join(j_paths.get('Name Of Top Library Directory'), 'Midi', 'Drum', 'Kicks')
                     if settings.get("Show More Console Logs", True):
-                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', j_clrs.get('Successfully Sorted File Color'))
+                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', f'{j_clrs.get("Successfully Sorted File Color")}')
                     else:
                         pass
                 elif any(pattern in file_name for pattern in pattern_lists.get("DrumPercs", [])):
                     total += 1
                     num_succeeded += 1
                     dest_path = os.path.join(j_paths.get('Name Of Top Library Directory'), 'Midi', 'Drum', 'Percussion')
                     if settings.get("Show More Console Logs", True):
-                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', j_clrs.get('Successfully Sorted File Color'))
+                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', f'{j_clrs.get("Successfully Sorted File Color")}')
                     else:
                         pass
                 elif any(pattern in file_name for pattern in pattern_lists.get("DrumShakers", [])):
                     total += 1
                     num_succeeded += 1
                     dest_path = os.path.join(j_paths.get('Name Of Top Library Directory'), 'Midi', 'Drum', 'Shakers')
                     if settings.get("Show More Console Logs", True):
-                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', j_clrs.get('Successfully Sorted File Color'))
+                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', f'{j_clrs.get("Successfully Sorted File Color")}')
                     else:
                         pass
                 elif any(pattern in file_name for pattern in pattern_lists.get("FX", [])):
                     total += 1
                     num_succeeded += 1
                     dest_path = os.path.join(j_paths.get('Name Of Top Library Directory'), 'Midi', 'FX')
                     if settings.get("Show More Console Logs", True):
-                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', j_clrs.get('Successfully Sorted File Color'))
+                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', f'{j_clrs.get("Successfully Sorted File Color")}')
                     else:
                         pass
                 elif any(pattern in file_name for pattern in pattern_lists.get("DrumLoops", [])):
                     total += 1
                     num_succeeded += 1
                     dest_path = os.path.join(j_paths.get('Name Of Top Library Directory'), 'Midi', 'Drum', 'Loops')
                     if settings.get("Show More Console Logs", True):
-                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', j_clrs.get('Successfully Sorted File Color'))
+                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', f'{j_clrs.get("Successfully Sorted File Color")}')
                     else:
                         pass
                 elif any(pattern in file_name for pattern in pattern_lists.get("DrumHats", [])):
                     total += 1
                     num_succeeded += 1
                     dest_path = os.path.join(j_paths.get('Name Of Top Library Directory'), 'Midi', 'Drum', 'Hats')
                     if settings.get("Show More Console Logs", True):
-                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', j_clrs.get('Successfully Sorted File Color'))
+                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', f'{j_clrs.get("Successfully Sorted File Color")}')
                     else:
                         pass
                 elif any(pattern in file_name for pattern in pattern_lists.get("DrumHatsOpen", [])):
                     total += 1
                     num_succeeded += 1
                     dest_path = os.path.join(j_paths.get('Name Of Top Library Directory'), 'Midi', 'Drum', 'Hats', 'Open')
                     if settings.get("Show More Console Logs", True):
-                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', j_clrs.get('Successfully Sorted File Color'))
+                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', f'{j_clrs.get("Successfully Sorted File Color")}')
                     else:
                         pass
                 elif any(pattern in file_name for pattern in pattern_lists.get("DrumHatsClosed", [])):
                     total += 1
                     num_succeeded += 1
                     dest_path = os.path.join(j_paths.get('Name Of Top Library Directory'), 'Midi', 'Drum', 'Hats', 'Closed')
                     if settings.get("Show More Console Logs", True):
-                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', j_clrs.get('Successfully Sorted File Color'))
+                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', f'{j_clrs.get("Successfully Sorted File Color")}')
                     else:
                         pass
                 elif any(pattern in file_name for pattern in pattern_lists.get("Voice", [])):
                     total += 1
                     num_succeeded += 1
                     dest_path = os.path.join(j_paths.get('Name Of Top Library Directory'), 'Midi', 'Voice')
                     if settings.get("Show More Console Logs", True):
-                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', j_clrs.get('Successfully Sorted File Color'))
+                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', f'{j_clrs.get("Successfully Sorted File Color")}')
                     else:
                         pass
                 elif any(pattern in file_name for pattern in pattern_lists.get("Bass", [])):
                     total += 1
                     num_succeeded += 1
                     dest_path = os.path.join(j_paths.get('Name Of Top Library Directory'), 'Midi', 'Bass')
                     if settings.get("Show More Console Logs", True):
-                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', j_clrs.get('Successfully Sorted File Color'))
+                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', f'{j_clrs.get("Successfully Sorted File Color")}')
                     else:
                         pass
                 elif any(pattern in file_name for pattern in pattern_lists.get("Atmos", [])):
                     total += 1
                     num_succeeded += 1
                     dest_path = os.path.join(j_paths.get('Name Of Top Library Directory'), 'Midi', 'Atmos')
                     if settings.get("Show More Console Logs", True):
-                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', j_clrs.get('Successfully Sorted File Color'))
+                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', f'{j_clrs.get("Successfully Sorted File Color")}')
                     else:
                         pass
                 else:
                     dest_path = os.path.join(j_paths.get('Name Of Top Library Directory'), 'Midi', 'Unsorted')
                     total += 1
                     num_failed += 1
                     if settings.get("Show More Console Logs", True):
-                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', j_clrs.get('Successfully Sorted File Color'))
+                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', f'{j_clrs.get("Successfully Sorted File Color")}')
                     else:
                         pass
             elif file_extension in ["nmsv"]:
                 if any(pattern in file_name for pattern in pattern_lists.get("Bass", [])):
                     num_succeeded += 1
                     dest_path = os.path.join(j_paths.get('Name Of Top Library Directory'), 'Presets', 'Massive Presets', 'Bass')
                     total += 1
                     if settings.get("Show More Console Logs", True):
-                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', j_clrs.get('Successfully Sorted File Color'))
+                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', f'{j_clrs.get("Successfully Sorted File Color")}')
                     else:
                         pass  
                 elif any(pattern in file_name for pattern in pattern_lists.get("Plucks", [])):
                     total += 1
                     num_succeeded += 1
                     dest_path = os.path.join(j_paths.get('Name Of Top Library Directory'), 'Presets', 'Massive Presets', 'Plucks')
                     if settings.get("Show More Console Logs", True):
-                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', j_clrs.get('Successfully Sorted File Color'))
+                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', f'{j_clrs.get("Successfully Sorted File Color")}')
                     else:
                         pass
                 elif any(pattern in file_name for pattern in pattern_lists.get("Keys", [])):
                     total += 1
                     num_succeeded += 1
                     dest_path = os.path.join(j_paths.get('Name Of Top Library Directory'), 'Presets', 'Massive Presets', 'Keys')
                     if settings.get("Show More Console Logs", True):
-                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', j_clrs.get('Successfully Sorted File Color'))
+                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', f'{j_clrs.get("Successfully Sorted File Color")}')
                     else:
                         pass
                 elif any(pattern in file_name for pattern in pattern_lists.get("Pad", [])):
                     total += 1
                     num_succeeded += 1
                     dest_path = os.path.join(j_paths.get('Name Of Top Library Directory'), 'Presets', 'Massive Presets', 'Pad')
                     if settings.get("Show More Console Logs", True):
-                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', j_clrs.get('Successfully Sorted File Color'))
+                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', f'{j_clrs.get("Successfully Sorted File Color")}')
                     else:
                         pass
                 elif any(pattern in file_name for pattern in pattern_lists.get("Lead", [])):
                     total += 1
                     num_succeeded += 1
                     dest_path = os.path.join(j_paths.get('Name Of Top Library Directory'), 'Presets', 'Massive Presets', 'Lead')
                     if settings.get("Show More Console Logs", True):
-                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', j_clrs.get('Successfully Sorted File Color'))
+                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', f'{j_clrs.get("Successfully Sorted File Color")}')
                     else:
                         pass
                 elif any(pattern in file_name for pattern in pattern_lists.get("Synth", [])):
                     total += 1
                     num_succeeded += 1
                     dest_path = os.path.join(j_paths.get('Name Of Top Library Directory'), 'Presets', 'Massive Presets', 'Synth')
                     if settings.get("Show More Console Logs", True):
-                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', j_clrs.get('Successfully Sorted File Color'))
+                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', f'{j_clrs.get("Successfully Sorted File Color")}')
                     else:
                         pass
                 elif any(pattern in file_name for pattern in pattern_lists.get("FX", [])):
                     total += 1
                     num_succeeded += 1
                     dest_path = os.path.join(j_paths.get('Name Of Top Library Directory'), 'Presets', 'Massive Presets', 'FX')
                     if settings.get("Show More Console Logs", True):
-                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', j_clrs.get('Successfully Sorted File Color'))
+                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', f'{j_clrs.get("Successfully Sorted File Color")}')
                     else:
                         pass
                 elif any(pattern in file_name for pattern in pattern_lists.get("Atmos", [])):
                     total += 1
                     num_succeeded += 1
                     dest_path = os.path.join(j_paths.get('Name Of Top Library Directory'), 'Presets', 'Massive Presets', 'Atmos')
                     if settings.get("Show More Console Logs", True):
-                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', j_clrs.get('Successfully Sorted File Color'))
+                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', f'{j_clrs.get("Successfully Sorted File Color")}')
                     else:
                         pass
                 elif any(pattern in file_name for pattern in pattern_lists.get("Voice", [])):
                     total += 1
                     num_succeeded += 1
                     dest_path = os.path.join(j_paths.get('Name Of Top Library Directory'), 'Presets', 'Massive Presets', 'Voice')
                     if settings.get("Show More Console Logs", True):
-                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', j_clrs.get('Successfully Sorted File Color'))
+                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', f'{j_clrs.get("Successfully Sorted File Color")}')
                     else:
                         pass
                 elif any(pattern in file_name for pattern in pattern_lists.get("808", [])):
                     total += 1
                     num_succeeded += 1
                     dest_path = os.path.join(j_paths.get('Name Of Top Library Directory'), 'Presets', 'Massive Presets', '808')
                     if settings.get("Show More Console Logs", True):
-                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', j_clrs.get('Successfully Sorted File Color'))
+                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', f'{j_clrs.get("Successfully Sorted File Color")}')
                     else:
                         pass
                 elif any(pattern in file_name for pattern in pattern_lists.get("DrumPresets", [])):
                     total += 1
                     num_succeeded += 1
                     dest_path = os.path.join(j_paths.get('Name Of Top Library Directory'), 'Presets', 'Massive Presets', 'DrumPresets')
                     if settings.get("Show More Console Logs", True):
-                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', j_clrs.get('Successfully Sorted File Color'))
+                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', f'{j_clrs.get("Successfully Sorted File Color")}')
                     else:
                         pass
                 else:
                     dest_path = os.path.join(j_paths.get('Name Of Top Library Directory'), 'Presets', 'Massive Presets', 'Unsorted')
                     total += 1
                     num_succeeded += 1
                     if settings.get("Show More Console Logs", True):
-                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', j_clrs.get('Successfully Sorted File Color'))
+                        log_console(f'{file_name}', f'{seperator}', f'{dest_path}', f'{j_clrs.get("Successfully Sorted File Color")}')
                     else:
                         pass
                         num_failed += 1
             elif file_extension in ["flp", "abl"] and any(pattern in file_name for pattern in pattern_lists.get("Templates")):
                 total += 1
                 num_succeeded += 1
                 dest_path = os.path.join(j_paths.get('Name Of Top Library Directory'), 'Projects', 'Templates')
                 if settings.get("Show More Console Logs", True):
-                    log_console(f'{file_name}', f'{seperator}', f'{dest_path}', j_clrs.get('Successfully Sorted File Color'))
+                    log_console(f'{file_name}', f'{seperator}', f'{dest_path}', f'{j_clrs.get("Successfully Sorted File Color")}')
                 else:
                     pass
             elif file_extension in ["flp", "abl"]:
                 total += 1
                 num_succeeded += 1
                 dest_path = os.path.join(j_paths.get('Name Of Top Library Directory'), 'Projects')
                 if settings.get("Show More Console Logs", True):
-                    log_console(f'{file_name}', f'{seperator}', f'{dest_path}', j_clrs.get('Successfully Sorted File Color'))
+                    log_console(f'{file_name}', f'{seperator}', f'{dest_path}', f'{j_clrs.get("Successfully Sorted File Color")}')
                 else:
                     pass
             elif file_extension in plugin_exts:
                 total += 1
                 num_succeeded += 1
                 dest_path = os.path.join(j_paths.get('Name Of Top Library Directory'), 'Plugins')
                 if settings.get("Show More Console Logs", True):
-                    log_console(f'{file_name}', f'{seperator}', f'{dest_path}', j_clrs.get('Successfully Sorted File Color'))
+                    log_console(f'{file_name}', f'{seperator}', f'{dest_path}', f'{j_clrs.get("Successfully Sorted File Color")}')
                 else:
                     pass
             else:
                 dest_path = rejected_unsorted_path
                 total += 1
                 num_failed2 += 1
                 if settings.get("Show More Console Logs", True):
-                    log_console(f'{file_name}', f'{seperator}', f'{rejected_unsorted_path}', j_clrs.get('Rejected Filetype Color'))
+                    log_console(f'{file_name}', f'{seperator}', f'{rejected_unsorted_path}', f'{j_clrs.get("Rejected Filetype Color")}')
                 else:
                     pass
             organize_files_by_extension(rejected_unsorted_path)
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
-    check_dir(path1)
+    check_dir(f'{path1}')
     if settings.get("Show Top Title Bar", True):
         bar = settings.get("Top Title Bar")
         log_message(bar, f'{j_clrs.get("Top Title Bar Color")}', True, True)
     else:
         pass
     
     if settings.get("Show Statistics", True):
         log_message(prompt1, f'{j_clrs.get("Prompt Color")}', False, False)
-        log_message(f'sorted by name & file type:   ', f'{j_clrs.get("Foregroud Color 1")}', False, False)
+        log_message(f'sorted by name & file type:   ', f'{j_clrs.get("Foreground Color 1")}', False, False)
         log_message(f' {num_succeeded}', f'{j_clrs.get("Successfully Sorted File Color")}')
         log_message(prompt1, f'{j_clrs.get("Prompt Color")}', False, False)
-        log_message(f'sorted only by file type: ', f'{j_clrs.get("Foregroud Color 1")}', False, False)
+        log_message(f'sorted only by file type: ', f'{j_clrs.get("Foreground Color 1")}', False, False)
         log_message(f' {num_failed}', f'{j_clrs.get("Unsorted File Color")}')
         log_message(prompt1, f'{j_clrs.get("Prompt Color")}', False, False)
-        log_message(f'rejected file types: ', f'{j_clrs.get("Foregroud Color 1")}', False, False)
+        log_message(f'rejected file types: ', f'{j_clrs.get("Foreground Color 1")}', False, False)
         log_message(f' {num_failed2}', f'{j_clrs.get("Rejected Filetype Color")}')
         log_message(f'      {total}', f'{j_clrs.get("Statistics Value Color")}', False, False)
         log_message(f' files processed in ', f'{j_clrs.get("Foreground Color 2")}', False, False)
         log_message(f'{elapsed_time:.2f}', f'{j_clrs.get("Statistics Value Color")}', False, False)
         log_message(f' seconds', f'{j_clrs.get("Foreground Color 1")}', False, True)
         maxfile = settings.get('Max files per Dir')
         split_files_in_subdirectories(path2, max_files_per_dir=maxfile)
@@ -1012,48 +1010,48 @@
             temp_file_path = file.read()
         if settings.get("Run Shell Command On Startup", True):
             os.system(CmdOnStartup)
         else:
             pass
         bar = settings.get("Top Title Bar")
         log_message(bar, f'{j_clrs.get("Top Title Bar Color")}', True, True)
-        log_message(temp_content, f'{j_clrs.get("Foregroud Color 1")}', False, True)
+        log_message(temp_content, f'{j_clrs.get("Foreground Color 1")}', False, True)
     elif args.colors:
         if settings.get("Run Shell Command On Startup", True):
             os.system(CmdOnStartup)
         else:
             pass
         bar = settings.get("Top Title Bar")
         log_message(bar, f'{j_clrs.get("Top Title Bar Color")}', True, True)
         clist = {
             "Colors": ['black', 'red', 'green', 'yellow', 'blue', 'magenta', 'cyan', 'white', 'light_grey', 'dark_grey', 'light_red', 'light_green', 'light_yellow', 'light_blue', 'light_magenta', 'light_cyan']
         }
         colors = clist["Colors"]
         log_message("Possible Color Settings", f'{j_clrs.get("Statistics Value Color")}', False, False)
-        log_message(':', f'{j_clrs.get("Foregroud Color 1")}', False, True)
+        log_message(':', f'{j_clrs.get("Foreground Color 1")}', False, True)
         for color in colors:
             log_message(spacer+ color, f'{color}', False, True)
     elif args.help:
         if settings.get("Run Shell Command On Startup", True):
             os.system(CmdOnStartup)
         else:
             pass
         bar = settings.get("Top Title Bar")
         log_message(bar, f'{j_clrs.get("Top Title Bar Color")}', True, True)
         log_message('Help', f'{j_clrs.get("Statistics Value Color")}', False, False)
-        log_message(':', f'{j_clrs.get("Foregroud Color 1")}', False, True)
-        log_message('           -paths '+ f'{spacer}', f'{j_clrs.get("Foregroud Color 1")}', False, False)
+        log_message(':', f'{j_clrs.get("Foreground Color 1")}', False, True)
+        log_message('           -paths '+ f'{spacer}', f'{j_clrs.get("Foreground Color 1")}', False, False)
         log_message('Displays Paths', f'{j_clrs.get("Statistics Value Color")}', False, True)
-        log_message('           -colors'+ f'{spacer}', f'{j_clrs.get("Foregroud Color 1")}', False, False)
+        log_message('           -colors'+ f'{spacer}', f'{j_clrs.get("Foreground Color 1")}', False, False)
         log_message('Displays Possible Color Settings', f'{j_clrs.get("Statistics Value Color")}', False, True)
-        log_message('           -config'+ f'{spacer}', f'{j_clrs.get("Foregroud Color 1")}', False, False)
+        log_message('           -config'+ f'{spacer}', f'{j_clrs.get("Foreground Color 1")}', False, False)
         log_message('Launch Config File', f'{j_clrs.get("Statistics Value Color")}', False, True)
-        log_message('           -help  '+ f'{spacer}', f'{j_clrs.get("Foregroud Color 1")}', False, False)
+        log_message('           -help  '+ f'{spacer}', f'{j_clrs.get("Foreground Color 1")}', False, False)
         log_message('Displays Help', f'{j_clrs.get("Statistics Value Color")}', False, True)
     elif args.config:
         settingsfile = settings_f
         cmd = "Start "+ f'{settingsfile}'
         os.system(cmd)
     else:
-        sort_files(f'{path1}', pattern_lists) 
+        sort_files(path1, pattern_lists) 
 def __main__():
     print_help_message()
```

