# Comparing `tmp/slib-sorter-1.3.3.tar.gz` & `tmp/slib-sorter-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slib-sorter-1.3.3.tar", last modified: Sat Jul  8 08:39:40 2023, max compression
+gzip compressed data, was "slib-sorter-1.3.4.tar", last modified: Sat Jul  8 08:42:24 2023, max compression
```

## Comparing `slib-sorter-1.3.3.tar` & `slib-sorter-1.3.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-08 08:39:40.528324 slib-sorter-1.3.3/
--rw-rw-rw-   0        0        0    11558 2023-07-07 20:03:54.000000 slib-sorter-1.3.3/LICENSE
--rw-rw-rw-   0        0        0     2249 2023-07-08 08:39:40.527324 slib-sorter-1.3.3/PKG-INFO
--rw-rw-rw-   0        0        0     1773 2023-07-08 06:05:27.000000 slib-sorter-1.3.3/README.md
--rw-rw-rw-   0        0        0       42 2023-07-08 08:39:40.528324 slib-sorter-1.3.3/setup.cfg
--rw-rw-rw-   0        0        0     3056 2023-07-08 08:39:06.000000 slib-sorter-1.3.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-08 08:39:40.525324 slib-sorter-1.3.3/slib_sorter.egg-info/
--rw-rw-rw-   0        0        0     2249 2023-07-08 08:39:40.000000 slib-sorter-1.3.3/slib_sorter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      273 2023-07-08 08:39:40.000000 slib-sorter-1.3.3/slib_sorter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-08 08:39:40.000000 slib-sorter-1.3.3/slib_sorter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       57 2023-07-08 08:39:40.000000 slib-sorter-1.3.3/slib_sorter.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       17 2023-07-08 08:39:40.000000 slib-sorter-1.3.3/slib_sorter.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-07-08 08:39:40.000000 slib-sorter-1.3.3/slib_sorter.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-08 08:39:40.526324 slib-sorter-1.3.3/src/
--rw-rw-rw-   0        0        0        0 2023-06-28 15:10:46.000000 slib-sorter-1.3.3/src/__init__.py
--rw-rw-rw-   0        0        0    63211 2023-07-08 08:38:13.000000 slib-sorter-1.3.3/src/slib_sorter.py
+drwxrwxrwx   0        0        0        0 2023-07-08 08:42:24.347213 slib-sorter-1.3.4/
+-rw-rw-rw-   0        0        0    11558 2023-07-07 20:03:54.000000 slib-sorter-1.3.4/LICENSE
+-rw-rw-rw-   0        0        0     2249 2023-07-08 08:42:24.347213 slib-sorter-1.3.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1773 2023-07-08 06:05:27.000000 slib-sorter-1.3.4/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-08 08:42:24.348217 slib-sorter-1.3.4/setup.cfg
+-rw-rw-rw-   0        0        0     3056 2023-07-08 08:42:12.000000 slib-sorter-1.3.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-08 08:42:24.338204 slib-sorter-1.3.4/slib_sorter.egg-info/
+-rw-rw-rw-   0        0        0     2249 2023-07-08 08:42:24.000000 slib-sorter-1.3.4/slib_sorter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      273 2023-07-08 08:42:24.000000 slib-sorter-1.3.4/slib_sorter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-08 08:42:24.000000 slib-sorter-1.3.4/slib_sorter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       57 2023-07-08 08:42:24.000000 slib-sorter-1.3.4/slib_sorter.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       17 2023-07-08 08:42:24.000000 slib-sorter-1.3.4/slib_sorter.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-07-08 08:42:24.000000 slib-sorter-1.3.4/slib_sorter.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-08 08:42:24.346212 slib-sorter-1.3.4/src/
+-rw-rw-rw-   0        0        0        0 2023-06-28 15:10:46.000000 slib-sorter-1.3.4/src/__init__.py
+-rw-rw-rw-   0        0        0    63176 2023-07-08 08:42:07.000000 slib-sorter-1.3.4/src/slib_sorter.py
```

### Comparing `slib-sorter-1.3.3/LICENSE` & `slib-sorter-1.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `slib-sorter-1.3.3/PKG-INFO` & `slib-sorter-1.3.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slib-sorter
-Version: 1.3.3
+Version: 1.3.4
 Summary: A Python package for sorting Sample Libraries
 Home-page: https://github.com/nrdrch/slib-sorter
 Author: Lukas H
 Author-email: fettkindasindauchoke@gmail.com
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
```

### Comparing `slib-sorter-1.3.3/README.md` & `slib-sorter-1.3.4/README.md`

 * *Files identical despite different names*

### Comparing `slib-sorter-1.3.3/setup.py` & `slib-sorter-1.3.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,15 +52,15 @@
 ''' 
             f.write(default_config)
     else:
         pass
 
     setuptools.setup(
         name="slib-sorter",
-        version="1.3.3",
+        version="1.3.4",
         author="Lukas H",
         author_email="fettkindasindauchoke@gmail.com",
         description="A Python package for sorting Sample Libraries",
         long_description=long_description,
         long_description_content_type="text/markdown",
         url="https://github.com/nrdrch/slib-sorter",
         packages=setuptools.find_packages(),
```

### Comparing `slib-sorter-1.3.3/slib_sorter.egg-info/PKG-INFO` & `slib-sorter-1.3.4/slib_sorter.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slib-sorter
-Version: 1.3.3
+Version: 1.3.4
 Summary: A Python package for sorting Sample Libraries
 Home-page: https://github.com/nrdrch/slib-sorter
 Author: Lukas H
 Author-email: fettkindasindauchoke@gmail.com
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
```

### Comparing `slib-sorter-1.3.3/src/slib_sorter.py` & `slib-sorter-1.3.4/src/slib_sorter.py`

 * *Files 0% similar despite different names*

```diff
@@ -1031,10 +1031,10 @@
         log_message('           -help  '+ f'{spacer}', f'{settings.get("Colors", "Foregroud Color 1")}', False, False)
         log_message('Displays Help', f'{settings.get("Colors", "Statistics Value Color")}', False, True)
     elif args.config:
         settingsfile = settings_f
         cmd = "Start "+ f'{settingsfile}'
         os.system(cmd)
     else:
-        sort_files(j_paths.get('To Be Processed Directory'), pattern_lists) 
+        sort_files(path1, pattern_lists) 
 def __main__():
     print_help_message()
```

