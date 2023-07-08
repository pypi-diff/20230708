# Comparing `tmp/slib-sorter-1.5.5.tar.gz` & `tmp/slib-sorter-1.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slib-sorter-1.5.5.tar", last modified: Sat Jul  8 13:02:48 2023, max compression
+gzip compressed data, was "dist\slib-sorter-1.5.6.tar", last modified: Sat Jul  8 13:09:30 2023, max compression
```

## Comparing `slib-sorter-1.5.5.tar` & `slib-sorter-1.5.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-08 13:02:48.503401 slib-sorter-1.5.5/
--rw-rw-rw-   0        0        0    11558 2023-07-07 20:03:54.000000 slib-sorter-1.5.5/LICENSE
--rw-rw-rw-   0        0        0     2249 2023-07-08 13:02:48.503401 slib-sorter-1.5.5/PKG-INFO
--rw-rw-rw-   0        0        0     1773 2023-07-08 06:05:27.000000 slib-sorter-1.5.5/README.md
--rw-rw-rw-   0        0        0       42 2023-07-08 13:02:48.503401 slib-sorter-1.5.5/setup.cfg
--rw-rw-rw-   0        0        0     3139 2023-07-08 13:02:41.000000 slib-sorter-1.5.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-08 13:02:48.500414 slib-sorter-1.5.5/slib_sorter.egg-info/
--rw-rw-rw-   0        0        0     2249 2023-07-08 13:02:48.000000 slib-sorter-1.5.5/slib_sorter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      273 2023-07-08 13:02:48.000000 slib-sorter-1.5.5/slib_sorter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-08 13:02:48.000000 slib-sorter-1.5.5/slib_sorter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       57 2023-07-08 13:02:48.000000 slib-sorter-1.5.5/slib_sorter.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       17 2023-07-08 13:02:48.000000 slib-sorter-1.5.5/slib_sorter.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-07-08 13:02:48.000000 slib-sorter-1.5.5/slib_sorter.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-08 13:02:48.502428 slib-sorter-1.5.5/src/
--rw-rw-rw-   0        0        0        0 2023-06-28 15:10:46.000000 slib-sorter-1.5.5/src/__init__.py
--rw-rw-rw-   0        0        0    67035 2023-07-08 12:51:23.000000 slib-sorter-1.5.5/src/slib_sorter.py
+drwxrwxrwx   0        0        0        0 2023-07-08 13:09:30.000000 slib-sorter-1.5.6/
+-rw-rw-rw-   0        0        0    11558 2023-07-07 20:03:54.000000 slib-sorter-1.5.6/LICENSE
+-rw-rw-rw-   0        0        0     2249 2023-07-08 13:09:30.000000 slib-sorter-1.5.6/PKG-INFO
+-rw-rw-rw-   0        0        0     1773 2023-07-08 06:05:27.000000 slib-sorter-1.5.6/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-08 13:09:30.000000 slib-sorter-1.5.6/setup.cfg
+-rw-rw-rw-   0        0        0     3139 2023-07-08 13:08:53.000000 slib-sorter-1.5.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-08 13:09:30.000000 slib-sorter-1.5.6/slib_sorter.egg-info/
+-rw-rw-rw-   0        0        0     2249 2023-07-08 13:09:30.000000 slib-sorter-1.5.6/slib_sorter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      273 2023-07-08 13:09:30.000000 slib-sorter-1.5.6/slib_sorter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-08 13:09:30.000000 slib-sorter-1.5.6/slib_sorter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       57 2023-07-08 13:09:30.000000 slib-sorter-1.5.6/slib_sorter.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       17 2023-07-08 13:09:30.000000 slib-sorter-1.5.6/slib_sorter.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-07-08 13:09:30.000000 slib-sorter-1.5.6/slib_sorter.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-08 13:09:30.000000 slib-sorter-1.5.6/src/
+-rw-rw-rw-   0        0        0        0 2023-06-28 15:10:46.000000 slib-sorter-1.5.6/src/__init__.py
+-rw-rw-rw-   0        0        0    67233 2023-07-08 13:08:43.000000 slib-sorter-1.5.6/src/slib_sorter.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `slib-sorter-1.5.5/LICENSE` & `slib-sorter-1.5.6/LICENSE`

 * *Files identical despite different names*

### Comparing `slib-sorter-1.5.5/PKG-INFO` & `slib-sorter-1.5.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slib-sorter
-Version: 1.5.5
+Version: 1.5.6
 Summary: A Python package for sorting Sample Libraries
 Home-page: https://github.com/nrdrch/slib-sorter
 Author: Lukas H
 Author-email: fettkindasindauchoke@gmail.com
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
```

### Comparing `slib-sorter-1.5.5/README.md` & `slib-sorter-1.5.6/README.md`

 * *Files identical despite different names*

### Comparing `slib-sorter-1.5.5/setup.py` & `slib-sorter-1.5.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,15 +54,15 @@
 ''' 
         f.write(default_config)
     else:
         pass
 
     setuptools.setup(
         name="slib-sorter",
-        version="1.5.5",
+        version="1.5.6",
         author="Lukas H",
         author_email="fettkindasindauchoke@gmail.com",
         description="A Python package for sorting Sample Libraries",
         long_description=long_description,
         long_description_content_type="text/markdown",
         url="https://github.com/nrdrch/slib-sorter",
         packages=setuptools.find_packages(),
```

### Comparing `slib-sorter-1.5.5/slib_sorter.egg-info/PKG-INFO` & `slib-sorter-1.5.6/slib_sorter.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slib-sorter
-Version: 1.5.5
+Version: 1.5.6
 Summary: A Python package for sorting Sample Libraries
 Home-page: https://github.com/nrdrch/slib-sorter
 Author: Lukas H
 Author-email: fettkindasindauchoke@gmail.com
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
```

### Comparing `slib-sorter-1.5.5/src/slib_sorter.py` & `slib-sorter-1.5.6/src/slib_sorter.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 def check_dir(*paths):
     for path in paths:
         if not os.path.exists(*paths):
             os.makedirs(*paths)
         else:
             pass
 def join_corrected_paths(settings):
+    settings_folder = os.path.join(os.environ['USERPROFILE'], 'Documents', 'WindowsPowerShell', 'Scripts', 'slib_sorter')
+    settings = os.path.join(settings_folder, 'settings.json')
     with open(settings, "r") as file:
         settings = json.load(file)
 
     paths = settings.get('Paths', {})
     joined_paths = {}
     
     for key, path in paths.items():
@@ -104,15 +106,15 @@
             remove_directory_tree(child_path)
     try:
         os.remove(path)
     except OSError as error:
         os.chmod(path, stat.S_IWRITE)
         os.remove(path)
 
-path1 = j_paths.get('To Be Processed Directory')
+file_path = path1 = j_paths.get('To Be Processed Directory')
 
 
 path2 = j_paths.get('Name Of Top Library Directory')
 
 
 def split_files_in_subdirectories(path2, max_files_per_dir=50):
     for root, dirs, files in os.walk(path2):
```

