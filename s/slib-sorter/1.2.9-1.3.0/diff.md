# Comparing `tmp/slib-sorter-1.2.9.tar.gz` & `tmp/slib-sorter-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slib-sorter-1.2.9.tar", last modified: Sat Jul  8 06:37:05 2023, max compression
+gzip compressed data, was "slib-sorter-1.3.0.tar", last modified: Sat Jul  8 06:45:29 2023, max compression
```

## Comparing `slib-sorter-1.2.9.tar` & `slib-sorter-1.3.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-08 06:37:05.969541 slib-sorter-1.2.9/
--rw-rw-rw-   0        0        0    11558 2023-07-07 20:03:54.000000 slib-sorter-1.2.9/LICENSE
--rw-rw-rw-   0        0        0     2249 2023-07-08 06:37:05.969541 slib-sorter-1.2.9/PKG-INFO
--rw-rw-rw-   0        0        0     1773 2023-07-08 06:05:27.000000 slib-sorter-1.2.9/README.md
--rw-rw-rw-   0        0        0       42 2023-07-08 06:37:05.970518 slib-sorter-1.2.9/setup.cfg
--rw-rw-rw-   0        0        0     2994 2023-07-08 06:27:38.000000 slib-sorter-1.2.9/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-08 06:37:05.960533 slib-sorter-1.2.9/slib_sorter.egg-info/
--rw-rw-rw-   0        0        0     2249 2023-07-08 06:37:05.000000 slib-sorter-1.2.9/slib_sorter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      273 2023-07-08 06:37:05.000000 slib-sorter-1.2.9/slib_sorter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-08 06:37:05.000000 slib-sorter-1.2.9/slib_sorter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       57 2023-07-08 06:37:05.000000 slib-sorter-1.2.9/slib_sorter.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       17 2023-07-08 06:37:05.000000 slib-sorter-1.2.9/slib_sorter.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-07-08 06:37:05.000000 slib-sorter-1.2.9/slib_sorter.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-08 06:37:05.968546 slib-sorter-1.2.9/src/
--rw-rw-rw-   0        0        0        0 2023-06-28 15:10:46.000000 slib-sorter-1.2.9/src/__init__.py
--rw-rw-rw-   0        0        0    67792 2023-07-08 06:36:21.000000 slib-sorter-1.2.9/src/slib_sorter.py
+drwxrwxrwx   0        0        0        0 2023-07-08 06:45:29.640083 slib-sorter-1.3.0/
+-rw-rw-rw-   0        0        0    11558 2023-07-07 20:03:54.000000 slib-sorter-1.3.0/LICENSE
+-rw-rw-rw-   0        0        0     2249 2023-07-08 06:45:29.640083 slib-sorter-1.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1773 2023-07-08 06:05:27.000000 slib-sorter-1.3.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-08 06:45:29.641079 slib-sorter-1.3.0/setup.cfg
+-rw-rw-rw-   0        0        0     2994 2023-07-08 06:42:27.000000 slib-sorter-1.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-08 06:45:29.630103 slib-sorter-1.3.0/slib_sorter.egg-info/
+-rw-rw-rw-   0        0        0     2249 2023-07-08 06:45:29.000000 slib-sorter-1.3.0/slib_sorter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      273 2023-07-08 06:45:29.000000 slib-sorter-1.3.0/slib_sorter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-08 06:45:29.000000 slib-sorter-1.3.0/slib_sorter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       57 2023-07-08 06:45:29.000000 slib-sorter-1.3.0/slib_sorter.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       17 2023-07-08 06:45:29.000000 slib-sorter-1.3.0/slib_sorter.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-07-08 06:45:29.000000 slib-sorter-1.3.0/slib_sorter.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-08 06:45:29.639108 slib-sorter-1.3.0/src/
+-rw-rw-rw-   0        0        0        0 2023-06-28 15:10:46.000000 slib-sorter-1.3.0/src/__init__.py
+-rw-rw-rw-   0        0        0    67655 2023-07-08 06:44:21.000000 slib-sorter-1.3.0/src/slib_sorter.py
```

### Comparing `slib-sorter-1.2.9/LICENSE` & `slib-sorter-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `slib-sorter-1.2.9/PKG-INFO` & `slib-sorter-1.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slib-sorter
-Version: 1.2.9
+Version: 1.3.0
 Summary: A Python package for sorting Sample Libraries
 Home-page: https://github.com/nrdrch/slib-sorter
 Author: Lukas H
 Author-email: fettkindasindauchoke@gmail.com
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
```

### Comparing `slib-sorter-1.2.9/README.md` & `slib-sorter-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `slib-sorter-1.2.9/setup.py` & `slib-sorter-1.3.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,15 +50,15 @@
         with open(settings_file, 'w') as f:
             f.write(default_config)
     else:
         pass
 
     setuptools.setup(
         name="slib-sorter",
-        version="1.2.9",
+        version="1.3.0",
         author="Lukas H",
         author_email="fettkindasindauchoke@gmail.com",
         description="A Python package for sorting Sample Libraries",
         long_description=long_description,
         long_description_content_type="text/markdown",
         url="https://github.com/nrdrch/slib-sorter",
         packages=setuptools.find_packages(),
```

### Comparing `slib-sorter-1.2.9/slib_sorter.egg-info/PKG-INFO` & `slib-sorter-1.3.0/slib_sorter.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slib-sorter
-Version: 1.2.9
+Version: 1.3.0
 Summary: A Python package for sorting Sample Libraries
 Home-page: https://github.com/nrdrch/slib-sorter
 Author: Lukas H
 Author-email: fettkindasindauchoke@gmail.com
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
```

### Comparing `slib-sorter-1.2.9/src/slib_sorter.py` & `slib-sorter-1.3.0/src/slib_sorter.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,14 +80,15 @@
         os.remove(path)
     except OSError as error:
         os.chmod(path, stat.S_IWRITE)
         os.remove(path)
 TBPDPath = settings.get('TBPDPath')
 joined_TBPDPath_path = os.path.join(TBPDPath, settings.get('To Be Processed Directory'))
 corrected_TBPDPath_path = joined_TBPDPath_path.replace("/", "\\")
+check_dir(corrected_TBPDPath_path)
 file_path = path1 = corrected_TBPDPath_path
 path2 = os.path.join(os.environ['USERPROFILE'], settings.get('NOFLDPath'), settings.get("Name Of Top Library Directory"))
 def split_files_in_subdirectories(path2, max_files_per_dir=50):
     for root, dirs, files in os.walk(path2):
         if root == path2:
             continue
         num_files = len(files)
@@ -918,19 +919,14 @@
     elapsed_time = time.time() - start_time
     prompt1 = settings.get("Prompt")
     def remove_readonly(func, path, _):
         os.chmod(path, stat.S_IWRITE)
         func(path)
     shutil.rmtree(path1, onerror=remove_readonly)
     check_dir(path1)
-    def remove_readonly(func, path, _):
-        os.chmod(path, stat.S_IWRITE)
-        func(path)
-    shutil.rmtree(path1, onerror=remove_readonly)
-    check_dir(path1)
     if settings.get("Show Top Bar", True):
         bar = settings.get("Top Bar")
         log_message(bar, f'{settings.get("Top Bar Color")}', True, True)
     else:
         pass
     if settings.get("Show Statistics", True):
         log_message(prompt1, f'{settings.get("Prompt Color")}', False, False)
```

