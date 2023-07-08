# Comparing `tmp/slib-sorter-1.3.5.tar.gz` & `tmp/slib-sorter-1.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slib-sorter-1.3.5.tar", last modified: Sat Jul  8 08:57:50 2023, max compression
+gzip compressed data, was "slib-sorter-1.3.6.tar", last modified: Sat Jul  8 08:59:54 2023, max compression
```

## Comparing `slib-sorter-1.3.5.tar` & `slib-sorter-1.3.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-08 08:57:50.290326 slib-sorter-1.3.5/
--rw-rw-rw-   0        0        0    11558 2023-07-07 20:03:54.000000 slib-sorter-1.3.5/LICENSE
--rw-rw-rw-   0        0        0     2249 2023-07-08 08:57:50.289324 slib-sorter-1.3.5/PKG-INFO
--rw-rw-rw-   0        0        0     1773 2023-07-08 06:05:27.000000 slib-sorter-1.3.5/README.md
--rw-rw-rw-   0        0        0       42 2023-07-08 08:57:50.290326 slib-sorter-1.3.5/setup.cfg
--rw-rw-rw-   0        0        0     3056 2023-07-08 08:57:29.000000 slib-sorter-1.3.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-08 08:57:50.280326 slib-sorter-1.3.5/slib_sorter.egg-info/
--rw-rw-rw-   0        0        0     2249 2023-07-08 08:57:50.000000 slib-sorter-1.3.5/slib_sorter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      273 2023-07-08 08:57:50.000000 slib-sorter-1.3.5/slib_sorter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-08 08:57:50.000000 slib-sorter-1.3.5/slib_sorter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       57 2023-07-08 08:57:50.000000 slib-sorter-1.3.5/slib_sorter.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       17 2023-07-08 08:57:50.000000 slib-sorter-1.3.5/slib_sorter.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-07-08 08:57:50.000000 slib-sorter-1.3.5/slib_sorter.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-08 08:57:50.288348 slib-sorter-1.3.5/src/
--rw-rw-rw-   0        0        0        0 2023-06-28 15:10:46.000000 slib-sorter-1.3.5/src/__init__.py
--rw-rw-rw-   0        0        0    63293 2023-07-08 08:57:21.000000 slib-sorter-1.3.5/src/slib_sorter.py
+drwxrwxrwx   0        0        0        0 2023-07-08 08:59:54.263223 slib-sorter-1.3.6/
+-rw-rw-rw-   0        0        0    11558 2023-07-07 20:03:54.000000 slib-sorter-1.3.6/LICENSE
+-rw-rw-rw-   0        0        0     2249 2023-07-08 08:59:54.263223 slib-sorter-1.3.6/PKG-INFO
+-rw-rw-rw-   0        0        0     1773 2023-07-08 06:05:27.000000 slib-sorter-1.3.6/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-08 08:59:54.263223 slib-sorter-1.3.6/setup.cfg
+-rw-rw-rw-   0        0        0     3056 2023-07-08 08:59:43.000000 slib-sorter-1.3.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-08 08:59:54.254238 slib-sorter-1.3.6/slib_sorter.egg-info/
+-rw-rw-rw-   0        0        0     2249 2023-07-08 08:59:54.000000 slib-sorter-1.3.6/slib_sorter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      273 2023-07-08 08:59:54.000000 slib-sorter-1.3.6/slib_sorter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-08 08:59:54.000000 slib-sorter-1.3.6/slib_sorter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       57 2023-07-08 08:59:54.000000 slib-sorter-1.3.6/slib_sorter.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       17 2023-07-08 08:59:54.000000 slib-sorter-1.3.6/slib_sorter.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-07-08 08:59:54.000000 slib-sorter-1.3.6/slib_sorter.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-08 08:59:54.262232 slib-sorter-1.3.6/src/
+-rw-rw-rw-   0        0        0        0 2023-06-28 15:10:46.000000 slib-sorter-1.3.6/src/__init__.py
+-rw-rw-rw-   0        0        0    63301 2023-07-08 08:59:24.000000 slib-sorter-1.3.6/src/slib_sorter.py
```

### Comparing `slib-sorter-1.3.5/LICENSE` & `slib-sorter-1.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `slib-sorter-1.3.5/PKG-INFO` & `slib-sorter-1.3.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slib-sorter
-Version: 1.3.5
+Version: 1.3.6
 Summary: A Python package for sorting Sample Libraries
 Home-page: https://github.com/nrdrch/slib-sorter
 Author: Lukas H
 Author-email: fettkindasindauchoke@gmail.com
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
```

### Comparing `slib-sorter-1.3.5/README.md` & `slib-sorter-1.3.6/README.md`

 * *Files identical despite different names*

### Comparing `slib-sorter-1.3.5/setup.py` & `slib-sorter-1.3.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,15 +52,15 @@
 ''' 
             f.write(default_config)
     else:
         pass
 
     setuptools.setup(
         name="slib-sorter",
-        version="1.3.5",
+        version="1.3.6",
         author="Lukas H",
         author_email="fettkindasindauchoke@gmail.com",
         description="A Python package for sorting Sample Libraries",
         long_description=long_description,
         long_description_content_type="text/markdown",
         url="https://github.com/nrdrch/slib-sorter",
         packages=setuptools.find_packages(),
```

### Comparing `slib-sorter-1.3.5/slib_sorter.egg-info/PKG-INFO` & `slib-sorter-1.3.6/slib_sorter.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slib-sorter
-Version: 1.3.5
+Version: 1.3.6
 Summary: A Python package for sorting Sample Libraries
 Home-page: https://github.com/nrdrch/slib-sorter
 Author: Lukas H
 Author-email: fettkindasindauchoke@gmail.com
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
```

### Comparing `slib-sorter-1.3.5/src/slib_sorter.py` & `slib-sorter-1.3.6/src/slib_sorter.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
     for key, path in paths.items():
         corrected_path = path.replace("/", "\\")
         more_corrected_path = corrected_path.replace("~", os.environ['USERPROFILE'])
         joined_paths[key] = more_corrected_path
         check_dir(more_corrected_path)
     return joined_paths 
-def clr_get():
+def clr_get(settings):
     settings_folder = os.path.join(os.environ['USERPROFILE'], 'Documents', 'WindowsPowerShell', 'Scripts', 'slib_sorter')
     settings = os.path.join(settings_folder, "settings.json")
     with open(settings, "r") as file:
         settings = json.load(file)
     Colors = settings.get('Colors', {})
     Parsed_Colors = {}
     for key, value in Colors.items():
```

