# Comparing `tmp/slib-sorter-1.2.1.tar.gz` & `tmp/slib-sorter-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slib-sorter-1.2.1.tar", last modified: Sat Jul  8 04:16:23 2023, max compression
+gzip compressed data, was "slib-sorter-1.2.2.tar", last modified: Sat Jul  8 04:30:35 2023, max compression
```

## Comparing `slib-sorter-1.2.1.tar` & `slib-sorter-1.2.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-08 04:16:23.605795 slib-sorter-1.2.1/
--rw-rw-rw-   0        0        0    11558 2023-07-07 20:03:54.000000 slib-sorter-1.2.1/LICENSE
--rw-rw-rw-   0        0        0     2267 2023-07-08 04:16:23.605795 slib-sorter-1.2.1/PKG-INFO
--rw-rw-rw-   0        0        0     1783 2023-07-08 03:49:36.000000 slib-sorter-1.2.1/README.md
--rw-rw-rw-   0        0        0       42 2023-07-08 04:16:23.605795 slib-sorter-1.2.1/setup.cfg
--rw-rw-rw-   0        0        0     4416 2023-07-08 04:15:00.000000 slib-sorter-1.2.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-08 04:16:23.595795 slib-sorter-1.2.1/slib_sorter.egg-info/
--rw-rw-rw-   0        0        0     2267 2023-07-08 04:16:23.000000 slib-sorter-1.2.1/slib_sorter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      273 2023-07-08 04:16:23.000000 slib-sorter-1.2.1/slib_sorter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-08 04:16:23.000000 slib-sorter-1.2.1/slib_sorter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       57 2023-07-08 04:16:23.000000 slib-sorter-1.2.1/slib_sorter.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       17 2023-07-08 04:16:23.000000 slib-sorter-1.2.1/slib_sorter.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-07-08 04:16:23.000000 slib-sorter-1.2.1/slib_sorter.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-08 04:16:23.604794 slib-sorter-1.2.1/src/
--rw-rw-rw-   0        0        0        0 2023-06-28 15:10:46.000000 slib-sorter-1.2.1/src/__init__.py
--rw-rw-rw-   0        0        0    69268 2023-07-08 04:15:41.000000 slib-sorter-1.2.1/src/slib_sorter.py
+drwxrwxrwx   0        0        0        0 2023-07-08 04:30:35.271140 slib-sorter-1.2.2/
+-rw-rw-rw-   0        0        0    11558 2023-07-07 20:03:54.000000 slib-sorter-1.2.2/LICENSE
+-rw-rw-rw-   0        0        0     2267 2023-07-08 04:30:35.270140 slib-sorter-1.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1783 2023-07-08 03:49:36.000000 slib-sorter-1.2.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-08 04:30:35.271140 slib-sorter-1.2.2/setup.cfg
+-rw-rw-rw-   0        0        0     4478 2023-07-08 04:30:05.000000 slib-sorter-1.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-08 04:30:35.268116 slib-sorter-1.2.2/slib_sorter.egg-info/
+-rw-rw-rw-   0        0        0     2267 2023-07-08 04:30:35.000000 slib-sorter-1.2.2/slib_sorter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      273 2023-07-08 04:30:35.000000 slib-sorter-1.2.2/slib_sorter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-08 04:30:35.000000 slib-sorter-1.2.2/slib_sorter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       57 2023-07-08 04:30:35.000000 slib-sorter-1.2.2/slib_sorter.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       17 2023-07-08 04:30:35.000000 slib-sorter-1.2.2/slib_sorter.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-07-08 04:30:35.000000 slib-sorter-1.2.2/slib_sorter.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-08 04:30:35.269127 slib-sorter-1.2.2/src/
+-rw-rw-rw-   0        0        0        0 2023-06-28 15:10:46.000000 slib-sorter-1.2.2/src/__init__.py
+-rw-rw-rw-   0        0        0    69268 2023-07-08 04:15:41.000000 slib-sorter-1.2.2/src/slib_sorter.py
```

### Comparing `slib-sorter-1.2.1/LICENSE` & `slib-sorter-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `slib-sorter-1.2.1/PKG-INFO` & `slib-sorter-1.2.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slib-sorter
-Version: 1.2.1
+Version: 1.2.2
 Summary: A Python package for sorting Sample Libraries
 Home-page: https://github.com/nrdrch/slib-sorter
 Author: Lukas Hübinger
 Author-email: fettkindasindauchoke@gmail.com
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
```

### Comparing `slib-sorter-1.2.1/README.md` & `slib-sorter-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `slib-sorter-1.2.1/setup.py` & `slib-sorter-1.2.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,19 +48,23 @@
     "Name Of Top Library Directory": "Sample Library",
     "RFPath": "Desktop",
     "Rejected Files": "Rejected Files",
     "Run Shell Command On Startup": false,
     "Command On Startup": "cls" 
 }}
     '''
-    with open(settings_file, 'w') as f:
-        f.write(default_config)
-    with open(settings_file, 'r') as file:
-        settings_file = json.load(file)
     settings = settings_file
+    if not os.path.exists(settings):
+        with open(settings, 'w') as f:
+            f.write(default_config)
+    else:
+        pass
+    with open(settings, 'r') as file:
+        settings = json.load(file)
+    
     #profile_path = os.path.expanduser("~/Documents/WindowsPowerShell/Microsoft.PowerShell_profile.ps1")
     #with open(profile_path, 'r') as f:
     #    profile_content = f.read()
     #    if f"Import-Module -DisableNameChecking \"{powershell_script_file}\"" in profile_content:
     #        pass
     #    else:
     #        with open(profile_path, 'a') as f:
@@ -83,15 +87,15 @@
 current_location = os.path.abspath(os.path.dirname(__file__))
 def install():
     with open("README.md", "r", encoding="utf-8") as fh:
         long_description = fh.read()
 
     setuptools.setup(
         name="slib-sorter",
-        version="1.2.1",
+        version="1.2.2",
         author="Lukas Hübinger",
         author_email="fettkindasindauchoke@gmail.com",
         description="A Python package for sorting Sample Libraries",
         long_description=long_description,
         long_description_content_type="text/markdown",
         url="https://github.com/nrdrch/slib-sorter",
         packages=setuptools.find_packages(),
```

### Comparing `slib-sorter-1.2.1/slib_sorter.egg-info/PKG-INFO` & `slib-sorter-1.2.2/slib_sorter.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slib-sorter
-Version: 1.2.1
+Version: 1.2.2
 Summary: A Python package for sorting Sample Libraries
 Home-page: https://github.com/nrdrch/slib-sorter
 Author: Lukas Hübinger
 Author-email: fettkindasindauchoke@gmail.com
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
```

### Comparing `slib-sorter-1.2.1/src/slib_sorter.py` & `slib-sorter-1.2.2/src/slib_sorter.py`

 * *Files identical despite different names*

