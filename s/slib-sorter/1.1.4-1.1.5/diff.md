# Comparing `tmp/slib-sorter-1.1.4.tar.gz` & `tmp/slib-sorter-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slib-sorter-1.1.4.tar", last modified: Sat Jul  8 02:50:53 2023, max compression
+gzip compressed data, was "slib-sorter-1.1.5.tar", last modified: Sat Jul  8 02:58:06 2023, max compression
```

## Comparing `slib-sorter-1.1.4.tar` & `slib-sorter-1.1.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-08 02:50:53.309754 slib-sorter-1.1.4/
--rw-rw-rw-   0        0        0    11558 2023-07-07 20:03:54.000000 slib-sorter-1.1.4/LICENSE
--rw-rw-rw-   0        0        0     2289 2023-07-08 02:50:53.309754 slib-sorter-1.1.4/PKG-INFO
--rw-rw-rw-   0        0        0     1807 2023-07-07 20:03:54.000000 slib-sorter-1.1.4/README.md
--rw-rw-rw-   0        0        0       42 2023-07-08 02:50:53.309754 slib-sorter-1.1.4/setup.cfg
--rw-rw-rw-   0        0        0     4376 2023-07-08 02:50:15.000000 slib-sorter-1.1.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-08 02:50:53.300778 slib-sorter-1.1.4/slib_sorter.egg-info/
--rw-rw-rw-   0        0        0     2289 2023-07-08 02:50:53.000000 slib-sorter-1.1.4/slib_sorter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      273 2023-07-08 02:50:53.000000 slib-sorter-1.1.4/slib_sorter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-08 02:50:53.000000 slib-sorter-1.1.4/slib_sorter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       57 2023-07-08 02:50:53.000000 slib-sorter-1.1.4/slib_sorter.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       17 2023-07-08 02:50:53.000000 slib-sorter-1.1.4/slib_sorter.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-07-08 02:50:53.000000 slib-sorter-1.1.4/slib_sorter.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-08 02:50:53.308820 slib-sorter-1.1.4/src/
--rw-rw-rw-   0        0        0        0 2023-06-28 15:10:46.000000 slib-sorter-1.1.4/src/__init__.py
--rw-rw-rw-   0        0        0    72439 2023-07-08 02:50:02.000000 slib-sorter-1.1.4/src/slib_sorter.py
+drwxrwxrwx   0        0        0        0 2023-07-08 02:58:06.219812 slib-sorter-1.1.5/
+-rw-rw-rw-   0        0        0    11558 2023-07-07 20:03:54.000000 slib-sorter-1.1.5/LICENSE
+-rw-rw-rw-   0        0        0     2291 2023-07-08 02:58:06.218817 slib-sorter-1.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1807 2023-07-07 20:03:54.000000 slib-sorter-1.1.5/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-08 02:58:06.219812 slib-sorter-1.1.5/setup.cfg
+-rw-rw-rw-   0        0        0     4378 2023-07-08 02:57:56.000000 slib-sorter-1.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-08 02:58:06.216808 slib-sorter-1.1.5/slib_sorter.egg-info/
+-rw-rw-rw-   0        0        0     2291 2023-07-08 02:58:06.000000 slib-sorter-1.1.5/slib_sorter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      273 2023-07-08 02:58:06.000000 slib-sorter-1.1.5/slib_sorter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-08 02:58:06.000000 slib-sorter-1.1.5/slib_sorter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       57 2023-07-08 02:58:06.000000 slib-sorter-1.1.5/slib_sorter.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       17 2023-07-08 02:58:06.000000 slib-sorter-1.1.5/slib_sorter.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-07-08 02:58:06.000000 slib-sorter-1.1.5/slib_sorter.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-08 02:58:06.217815 slib-sorter-1.1.5/src/
+-rw-rw-rw-   0        0        0        0 2023-06-28 15:10:46.000000 slib-sorter-1.1.5/src/__init__.py
+-rw-rw-rw-   0        0        0    72412 2023-07-08 02:54:58.000000 slib-sorter-1.1.5/src/slib_sorter.py
```

### Comparing `slib-sorter-1.1.4/LICENSE` & `slib-sorter-1.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `slib-sorter-1.1.4/PKG-INFO` & `slib-sorter-1.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: slib-sorter
-Version: 1.1.4
+Version: 1.1.5
 Summary: A Python library for sorting Sample Libraries
 Home-page: https://github.com/nrdrch/slib-sorter
 Author: Lukas Hübinger
 Author-email: fettkindasindauchoke@gmail.com
-Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Sample Library Sorter
 ###### *for now only meant to run on Windows10
```

### Comparing `slib-sorter-1.1.4/README.md` & `slib-sorter-1.1.5/README.md`

 * *Files identical despite different names*

### Comparing `slib-sorter-1.1.4/setup.py` & `slib-sorter-1.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,15 +80,15 @@
         importlib.reload(settings_file)
 def install():
     with open("README.md", "r", encoding="utf-8") as fh:
         long_description = fh.read()
 
     setuptools.setup(
         name="slib-sorter",
-        version="1.1.4",
+        version="1.1.5",
         author="Lukas Hübinger",
         author_email="fettkindasindauchoke@gmail.com",
         description="A Python library for sorting Sample Libraries",
         long_description=long_description,
         long_description_content_type="text/markdown",
         url="https://github.com/nrdrch/slib-sorter",
         packages=setuptools.find_packages(), 
@@ -97,15 +97,15 @@
                 "Slib-Sorter = src.slib_sorter:__main__"
             ]
         },
         install_requires=[
             "termcolor==2.3.0"
         ],
         classifiers=[
-            "Programming Language :: Python :: 3",
+            "Programming Language :: Python :: 3.7",
             "License :: OSI Approved :: Apache Software License",
             "Operating System :: Microsoft :: Windows :: Windows 10"
         ],
     )
     ps_script(os.path.join(current_location, "src", "slib_sorter.py"))
     
 def reload():
```

### Comparing `slib-sorter-1.1.4/slib_sorter.egg-info/PKG-INFO` & `slib-sorter-1.1.5/slib_sorter.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: slib-sorter
-Version: 1.1.4
+Version: 1.1.5
 Summary: A Python library for sorting Sample Libraries
 Home-page: https://github.com/nrdrch/slib-sorter
 Author: Lukas Hübinger
 Author-email: fettkindasindauchoke@gmail.com
-Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Sample Library Sorter
 ###### *for now only meant to run on Windows10
```

### Comparing `slib-sorter-1.1.4/src/slib_sorter.py` & `slib-sorter-1.1.5/src/slib_sorter.py`

 * *Files 0% similar despite different names*

```diff
@@ -1072,15 +1072,15 @@
     else:
         pass
     def remove_readonly(func, path, _):
         os.chmod(path, stat.S_IWRITE)
         func(path)
     shutil.rmtree(path1, onerror=remove_readonly)
     check_dir(path1)
-temp_content = "\nSorted Library Location:        "+ f"{os.path.join(os.environ['USERPROFILE'], settings.get('NOFLDPath'), settings.get('Name Of Top Library Directory'))}"+ "\nSettings Location:     "+ f"{os.path.join(path_finder(0), 'settings.json')}"+ "\nPyhton Script Location:    " f"{os.path.join(current_location, 'slib_sorter.py')}"+ "\nTo Be Sorted Location:    " f"{os.path.join(os.environ['USERPROFILE'], settings.get('TBPDPath'), settings.get('To Be Processed Directory'))}"+ "\nRejected Files Location:     " f"{os.path.join(os.environ['USERPROFILE'], settings.get('RFPath'), settings.get('Rejected Files'))}"
+temp_content = "\nSorted Library Location:        "+ f"{os.path.join(os.environ['USERPROFILE'], settings.get('NOFLDPath'), settings.get('Name Of Top Library Directory'))}"+ "\nSettings Location:     "+ f"{settings}"+ "\nPyhton Script Location:    " f"{os.path.join(current_location, 'slib_sorter.py')}"+ "\nTo Be Sorted Location:    " f"{os.path.join(os.environ['USERPROFILE'], settings.get('TBPDPath'), settings.get('To Be Processed Directory'))}"+ "\nRejected Files Location:     " f"{os.path.join(os.environ['USERPROFILE'], settings.get('RFPath'), settings.get('Rejected Files'))}"
 def print_help_message():
     parser = argparse.ArgumentParser()
     parser.add_argument("-paths", action="store_true")
     parser.add_argument("-help", action="store_true")
     parser.add_argument("-colors", action="store_true")
     parser.add_argument("-config", action="store_true")
     temp_file_path = temp_path_file(temp_content)
@@ -1123,7 +1123,8 @@
         settingsfile = os.path.join(path_finder(0), 'settings.json')
         cmd = "Start "+ settingsfile
         os.system(cmd)
     else:
         sort_files(path1, pattern_lists) 
 def __main__():
     print_help_message()
+__main__
```

