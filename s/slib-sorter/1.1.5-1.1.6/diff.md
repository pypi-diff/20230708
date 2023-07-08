# Comparing `tmp/slib-sorter-1.1.5.tar.gz` & `tmp/slib-sorter-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slib-sorter-1.1.5.tar", last modified: Sat Jul  8 02:58:06 2023, max compression
+gzip compressed data, was "slib-sorter-1.1.6.tar", last modified: Sat Jul  8 03:03:55 2023, max compression
```

## Comparing `slib-sorter-1.1.5.tar` & `slib-sorter-1.1.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-08 02:58:06.219812 slib-sorter-1.1.5/
--rw-rw-rw-   0        0        0    11558 2023-07-07 20:03:54.000000 slib-sorter-1.1.5/LICENSE
--rw-rw-rw-   0        0        0     2291 2023-07-08 02:58:06.218817 slib-sorter-1.1.5/PKG-INFO
--rw-rw-rw-   0        0        0     1807 2023-07-07 20:03:54.000000 slib-sorter-1.1.5/README.md
--rw-rw-rw-   0        0        0       42 2023-07-08 02:58:06.219812 slib-sorter-1.1.5/setup.cfg
--rw-rw-rw-   0        0        0     4378 2023-07-08 02:57:56.000000 slib-sorter-1.1.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-08 02:58:06.216808 slib-sorter-1.1.5/slib_sorter.egg-info/
--rw-rw-rw-   0        0        0     2291 2023-07-08 02:58:06.000000 slib-sorter-1.1.5/slib_sorter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      273 2023-07-08 02:58:06.000000 slib-sorter-1.1.5/slib_sorter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-08 02:58:06.000000 slib-sorter-1.1.5/slib_sorter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       57 2023-07-08 02:58:06.000000 slib-sorter-1.1.5/slib_sorter.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       17 2023-07-08 02:58:06.000000 slib-sorter-1.1.5/slib_sorter.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-07-08 02:58:06.000000 slib-sorter-1.1.5/slib_sorter.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-08 02:58:06.217815 slib-sorter-1.1.5/src/
--rw-rw-rw-   0        0        0        0 2023-06-28 15:10:46.000000 slib-sorter-1.1.5/src/__init__.py
--rw-rw-rw-   0        0        0    72412 2023-07-08 02:54:58.000000 slib-sorter-1.1.5/src/slib_sorter.py
+drwxrwxrwx   0        0        0        0 2023-07-08 03:03:55.345655 slib-sorter-1.1.6/
+-rw-rw-rw-   0        0        0    11558 2023-07-07 20:03:54.000000 slib-sorter-1.1.6/LICENSE
+-rw-rw-rw-   0        0        0     2291 2023-07-08 03:03:55.345655 slib-sorter-1.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0     1807 2023-07-07 20:03:54.000000 slib-sorter-1.1.6/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-08 03:03:55.346630 slib-sorter-1.1.6/setup.cfg
+-rw-rw-rw-   0        0        0     4378 2023-07-08 03:03:41.000000 slib-sorter-1.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-08 03:03:55.336662 slib-sorter-1.1.6/slib_sorter.egg-info/
+-rw-rw-rw-   0        0        0     2291 2023-07-08 03:03:55.000000 slib-sorter-1.1.6/slib_sorter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      273 2023-07-08 03:03:55.000000 slib-sorter-1.1.6/slib_sorter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-08 03:03:55.000000 slib-sorter-1.1.6/slib_sorter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       57 2023-07-08 03:03:55.000000 slib-sorter-1.1.6/slib_sorter.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       17 2023-07-08 03:03:55.000000 slib-sorter-1.1.6/slib_sorter.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-07-08 03:03:55.000000 slib-sorter-1.1.6/slib_sorter.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-08 03:03:55.344655 slib-sorter-1.1.6/src/
+-rw-rw-rw-   0        0        0        0 2023-06-28 15:10:46.000000 slib-sorter-1.1.6/src/__init__.py
+-rw-rw-rw-   0        0        0    72651 2023-07-08 03:03:27.000000 slib-sorter-1.1.6/src/slib_sorter.py
```

### Comparing `slib-sorter-1.1.5/LICENSE` & `slib-sorter-1.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `slib-sorter-1.1.5/PKG-INFO` & `slib-sorter-1.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slib-sorter
-Version: 1.1.5
+Version: 1.1.6
 Summary: A Python library for sorting Sample Libraries
 Home-page: https://github.com/nrdrch/slib-sorter
 Author: Lukas Hübinger
 Author-email: fettkindasindauchoke@gmail.com
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
```

### Comparing `slib-sorter-1.1.5/README.md` & `slib-sorter-1.1.6/README.md`

 * *Files identical despite different names*

### Comparing `slib-sorter-1.1.5/setup.py` & `slib-sorter-1.1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,15 +80,15 @@
         importlib.reload(settings_file)
 def install():
     with open("README.md", "r", encoding="utf-8") as fh:
         long_description = fh.read()
 
     setuptools.setup(
         name="slib-sorter",
-        version="1.1.5",
+        version="1.1.6",
         author="Lukas Hübinger",
         author_email="fettkindasindauchoke@gmail.com",
         description="A Python library for sorting Sample Libraries",
         long_description=long_description,
         long_description_content_type="text/markdown",
         url="https://github.com/nrdrch/slib-sorter",
         packages=setuptools.find_packages(),
```

### Comparing `slib-sorter-1.1.5/slib_sorter.egg-info/PKG-INFO` & `slib-sorter-1.1.6/slib_sorter.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slib-sorter
-Version: 1.1.5
+Version: 1.1.6
 Summary: A Python library for sorting Sample Libraries
 Home-page: https://github.com/nrdrch/slib-sorter
 Author: Lukas Hübinger
 Author-email: fettkindasindauchoke@gmail.com
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
```

### Comparing `slib-sorter-1.1.5/src/slib_sorter.py` & `slib-sorter-1.1.6/src/slib_sorter.py`

 * *Files 0% similar despite different names*

```diff
@@ -230,14 +230,15 @@
 start_time = time.time()
 current_location = path_finder(0)
 source_file = os.path.join(current_location, 'slib_sorter.py')
 ps_script(source_file)
 icon_path = os.path.join(path_finder(1), 'examples', 'icn.ico')
 settings_folder = os.path.join(os.environ['USERPROFILE'], 'Documents', 'WindowsPowerShell', 'Scripts', 'slib_sorter')
 settings = os.path.join(settings_folder, "settings.json")
+settings_f = os.path.join(os.environ['USERPROFILE'], 'Documents', 'WindowsPowerShell', 'Scripts', 'slib_sorter', 'settings.json')
 #settings = os.path.join(path_finder(0), 'settings.json')
 with open(settings, 'r') as file:
     settings = json.load(file)
 file_path = path1 = os.path.join(os.environ['USERPROFILE'], settings.get('TBPDPath'), settings.get('To Be Processed Directory'))
 path2 = os.path.join(os.environ['USERPROFILE'], settings.get('NOFLDPath'), settings.get("Name Of Top Library Directory"))
 folder_path = path2
 check_dir(path1, path2)
@@ -1072,15 +1073,15 @@
     else:
         pass
     def remove_readonly(func, path, _):
         os.chmod(path, stat.S_IWRITE)
         func(path)
     shutil.rmtree(path1, onerror=remove_readonly)
     check_dir(path1)
-temp_content = "\nSorted Library Location:        "+ f"{os.path.join(os.environ['USERPROFILE'], settings.get('NOFLDPath'), settings.get('Name Of Top Library Directory'))}"+ "\nSettings Location:     "+ f"{settings}"+ "\nPyhton Script Location:    " f"{os.path.join(current_location, 'slib_sorter.py')}"+ "\nTo Be Sorted Location:    " f"{os.path.join(os.environ['USERPROFILE'], settings.get('TBPDPath'), settings.get('To Be Processed Directory'))}"+ "\nRejected Files Location:     " f"{os.path.join(os.environ['USERPROFILE'], settings.get('RFPath'), settings.get('Rejected Files'))}"
+temp_content = "\nSorted Library Location:        "+ f"{os.path.join(os.environ['USERPROFILE'], settings.get('NOFLDPath'), settings.get('Name Of Top Library Directory'))}"+ "\nSettings Location:     "+ f"{os.path.join(os.environ['USERPROFILE'], 'Documents', 'WindowsPowerShell', 'Scripts', 'slib_sorter', 'settings.json')}"+ "\nPyhton Script Location:    " f"{os.path.join(current_location, 'slib_sorter.py')}"+ "\nTo Be Sorted Location:    " f"{os.path.join(os.environ['USERPROFILE'], settings.get('TBPDPath'), settings.get('To Be Processed Directory'))}"+ "\nRejected Files Location:     " f"{os.path.join(os.environ['USERPROFILE'], settings.get('RFPath'), settings.get('Rejected Files'))}"
 def print_help_message():
     parser = argparse.ArgumentParser()
     parser.add_argument("-paths", action="store_true")
     parser.add_argument("-help", action="store_true")
     parser.add_argument("-colors", action="store_true")
     parser.add_argument("-config", action="store_true")
     temp_file_path = temp_path_file(temp_content)
```

