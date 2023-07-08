# Comparing `tmp/slib-sorter-1.2.4.tar.gz` & `tmp/slib-sorter-1.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slib-sorter-1.2.4.tar", last modified: Sat Jul  8 05:10:25 2023, max compression
+gzip compressed data, was "slib-sorter-1.2.5.tar", last modified: Sat Jul  8 05:14:30 2023, max compression
```

## Comparing `slib-sorter-1.2.4.tar` & `slib-sorter-1.2.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-08 05:10:25.694906 slib-sorter-1.2.4/
--rw-rw-rw-   0        0        0    11558 2023-07-07 20:03:54.000000 slib-sorter-1.2.4/LICENSE
--rw-rw-rw-   0        0        0     2267 2023-07-08 05:10:25.693867 slib-sorter-1.2.4/PKG-INFO
--rw-rw-rw-   0        0        0     1783 2023-07-08 03:49:36.000000 slib-sorter-1.2.4/README.md
--rw-rw-rw-   0        0        0       42 2023-07-08 05:10:25.694906 slib-sorter-1.2.4/setup.cfg
--rw-rw-rw-   0        0        0     3000 2023-07-08 05:09:24.000000 slib-sorter-1.2.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-08 05:10:25.691884 slib-sorter-1.2.4/slib_sorter.egg-info/
--rw-rw-rw-   0        0        0     2267 2023-07-08 05:10:25.000000 slib-sorter-1.2.4/slib_sorter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      273 2023-07-08 05:10:25.000000 slib-sorter-1.2.4/slib_sorter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-08 05:10:25.000000 slib-sorter-1.2.4/slib_sorter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       57 2023-07-08 05:10:25.000000 slib-sorter-1.2.4/slib_sorter.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       17 2023-07-08 05:10:25.000000 slib-sorter-1.2.4/slib_sorter.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-07-08 05:10:25.000000 slib-sorter-1.2.4/slib_sorter.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-08 05:10:25.692872 slib-sorter-1.2.4/src/
--rw-rw-rw-   0        0        0        0 2023-06-28 15:10:46.000000 slib-sorter-1.2.4/src/__init__.py
--rw-rw-rw-   0        0        0    68044 2023-07-08 05:02:00.000000 slib-sorter-1.2.4/src/slib_sorter.py
+drwxrwxrwx   0        0        0        0 2023-07-08 05:14:30.538428 slib-sorter-1.2.5/
+-rw-rw-rw-   0        0        0    11558 2023-07-07 20:03:54.000000 slib-sorter-1.2.5/LICENSE
+-rw-rw-rw-   0        0        0     2267 2023-07-08 05:14:30.538428 slib-sorter-1.2.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1783 2023-07-08 03:49:36.000000 slib-sorter-1.2.5/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-08 05:14:30.539474 slib-sorter-1.2.5/setup.cfg
+-rw-rw-rw-   0        0        0     3000 2023-07-08 05:14:15.000000 slib-sorter-1.2.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-08 05:14:30.528420 slib-sorter-1.2.5/slib_sorter.egg-info/
+-rw-rw-rw-   0        0        0     2267 2023-07-08 05:14:30.000000 slib-sorter-1.2.5/slib_sorter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      273 2023-07-08 05:14:30.000000 slib-sorter-1.2.5/slib_sorter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-08 05:14:30.000000 slib-sorter-1.2.5/slib_sorter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       57 2023-07-08 05:14:30.000000 slib-sorter-1.2.5/slib_sorter.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       17 2023-07-08 05:14:30.000000 slib-sorter-1.2.5/slib_sorter.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-07-08 05:14:30.000000 slib-sorter-1.2.5/slib_sorter.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-08 05:14:30.537453 slib-sorter-1.2.5/src/
+-rw-rw-rw-   0        0        0        0 2023-06-28 15:10:46.000000 slib-sorter-1.2.5/src/__init__.py
+-rw-rw-rw-   0        0        0    68032 2023-07-08 05:13:23.000000 slib-sorter-1.2.5/src/slib_sorter.py
```

### Comparing `slib-sorter-1.2.4/LICENSE` & `slib-sorter-1.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `slib-sorter-1.2.4/PKG-INFO` & `slib-sorter-1.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slib-sorter
-Version: 1.2.4
+Version: 1.2.5
 Summary: A Python package for sorting Sample Libraries
 Home-page: https://github.com/nrdrch/slib-sorter
 Author: Lukas Hübinger
 Author-email: fettkindasindauchoke@gmail.com
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
```

### Comparing `slib-sorter-1.2.4/README.md` & `slib-sorter-1.2.5/README.md`

 * *Files identical despite different names*

### Comparing `slib-sorter-1.2.4/setup.py` & `slib-sorter-1.2.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -50,15 +50,15 @@
         with open(settings_file, 'w') as f:
             f.write(default_config)
     else:
         pass
 
     setuptools.setup(
         name="slib-sorter",
-        version="1.2.4",
+        version="1.2.5",
         author="Lukas Hübinger",
         author_email="fettkindasindauchoke@gmail.com",
         description="A Python package for sorting Sample Libraries",
         long_description=long_description,
         long_description_content_type="text/markdown",
         url="https://github.com/nrdrch/slib-sorter",
         packages=setuptools.find_packages(),
```

### Comparing `slib-sorter-1.2.4/slib_sorter.egg-info/PKG-INFO` & `slib-sorter-1.2.5/slib_sorter.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slib-sorter
-Version: 1.2.4
+Version: 1.2.5
 Summary: A Python package for sorting Sample Libraries
 Home-page: https://github.com/nrdrch/slib-sorter
 Author: Lukas Hübinger
 Author-email: fettkindasindauchoke@gmail.com
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
```

### Comparing `slib-sorter-1.2.4/src/slib_sorter.py` & `slib-sorter-1.2.5/src/slib_sorter.py`

 * *Files 0% similar despite different names*

```diff
@@ -1015,9 +1015,8 @@
     elif args.config:
         settingsfile = settings_f
         cmd = "Start "+ f'{settingsfile}'
         os.system(cmd)
     else:
         sort_files(path1, pattern_lists) 
 def __main__():
-    print_help_message()
-__main__()
+    print_help_message()
```

