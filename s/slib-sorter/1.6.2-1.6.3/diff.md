# Comparing `tmp/slib-sorter-1.6.2.tar.gz` & `tmp/slib-sorter-1.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slib-sorter-1.6.2.tar", last modified: Sat Jul  8 14:17:39 2023, max compression
+gzip compressed data, was "slib-sorter-1.6.3.tar", last modified: Sat Jul  8 14:21:17 2023, max compression
```

## Comparing `slib-sorter-1.6.2.tar` & `slib-sorter-1.6.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-08 14:17:39.751297 slib-sorter-1.6.2/
--rw-rw-rw-   0        0        0    11558 2023-07-07 20:03:54.000000 slib-sorter-1.6.2/LICENSE
--rw-rw-rw-   0        0        0     2249 2023-07-08 14:17:39.751297 slib-sorter-1.6.2/PKG-INFO
--rw-rw-rw-   0        0        0     1773 2023-07-08 06:05:27.000000 slib-sorter-1.6.2/README.md
--rw-rw-rw-   0        0        0       42 2023-07-08 14:17:39.751297 slib-sorter-1.6.2/setup.cfg
--rw-rw-rw-   0        0        0     3020 2023-07-08 14:17:26.000000 slib-sorter-1.6.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-08 14:17:39.748324 slib-sorter-1.6.2/slib_sorter.egg-info/
--rw-rw-rw-   0        0        0     2249 2023-07-08 14:17:39.000000 slib-sorter-1.6.2/slib_sorter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      273 2023-07-08 14:17:39.000000 slib-sorter-1.6.2/slib_sorter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-08 14:17:39.000000 slib-sorter-1.6.2/slib_sorter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       57 2023-07-08 14:17:39.000000 slib-sorter-1.6.2/slib_sorter.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       17 2023-07-08 14:17:39.000000 slib-sorter-1.6.2/slib_sorter.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-07-08 14:17:39.000000 slib-sorter-1.6.2/slib_sorter.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-08 14:17:39.750313 slib-sorter-1.6.2/src/
--rw-rw-rw-   0        0        0        0 2023-06-28 15:10:46.000000 slib-sorter-1.6.2/src/__init__.py
--rw-rw-rw-   0        0        0    67378 2023-07-08 14:12:55.000000 slib-sorter-1.6.2/src/slib_sorter.py
+drwxrwxrwx   0        0        0        0 2023-07-08 14:21:17.882071 slib-sorter-1.6.3/
+-rw-rw-rw-   0        0        0    11558 2023-07-07 20:03:54.000000 slib-sorter-1.6.3/LICENSE
+-rw-rw-rw-   0        0        0     2249 2023-07-08 14:21:17.881058 slib-sorter-1.6.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1773 2023-07-08 06:05:27.000000 slib-sorter-1.6.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-08 14:21:17.882071 slib-sorter-1.6.3/setup.cfg
+-rw-rw-rw-   0        0        0     3020 2023-07-08 14:21:04.000000 slib-sorter-1.6.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-08 14:21:17.879058 slib-sorter-1.6.3/slib_sorter.egg-info/
+-rw-rw-rw-   0        0        0     2249 2023-07-08 14:21:17.000000 slib-sorter-1.6.3/slib_sorter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      273 2023-07-08 14:21:17.000000 slib-sorter-1.6.3/slib_sorter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-08 14:21:17.000000 slib-sorter-1.6.3/slib_sorter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       57 2023-07-08 14:21:17.000000 slib-sorter-1.6.3/slib_sorter.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       17 2023-07-08 14:21:17.000000 slib-sorter-1.6.3/slib_sorter.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-07-08 14:21:17.000000 slib-sorter-1.6.3/slib_sorter.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-08 14:21:17.880049 slib-sorter-1.6.3/src/
+-rw-rw-rw-   0        0        0        0 2023-06-28 15:10:46.000000 slib-sorter-1.6.3/src/__init__.py
+-rw-rw-rw-   0        0        0    67524 2023-07-08 14:20:32.000000 slib-sorter-1.6.3/src/slib_sorter.py
```

### Comparing `slib-sorter-1.6.2/LICENSE` & `slib-sorter-1.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `slib-sorter-1.6.2/PKG-INFO` & `slib-sorter-1.6.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slib-sorter
-Version: 1.6.2
+Version: 1.6.3
 Summary: A Python package for sorting Sample Libraries
 Home-page: https://github.com/nrdrch/slib-sorter
 Author: Lukas H
 Author-email: fettkindasindauchoke@gmail.com
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
```

### Comparing `slib-sorter-1.6.2/README.md` & `slib-sorter-1.6.3/README.md`

 * *Files identical despite different names*

### Comparing `slib-sorter-1.6.2/setup.py` & `slib-sorter-1.6.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,15 +57,15 @@
     
     if not os.path.exists(settings):
         with open(settings, 'w') as f:
             f.write(default_config)
     
     setuptools.setup(
         name="slib-sorter",
-        version="1.6.2",
+        version="1.6.3",
         author="Lukas H",
         author_email="fettkindasindauchoke@gmail.com",
         description="A Python package for sorting Sample Libraries",
         long_description=long_description,
         long_description_content_type="text/markdown",
         url="https://github.com/nrdrch/slib-sorter",
         packages=setuptools.find_packages(),
```

### Comparing `slib-sorter-1.6.2/slib_sorter.egg-info/PKG-INFO` & `slib-sorter-1.6.3/slib_sorter.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slib-sorter
-Version: 1.6.2
+Version: 1.6.3
 Summary: A Python package for sorting Sample Libraries
 Home-page: https://github.com/nrdrch/slib-sorter
 Author: Lukas H
 Author-email: fettkindasindauchoke@gmail.com
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
```

### Comparing `slib-sorter-1.6.2/src/slib_sorter.py` & `slib-sorter-1.6.3/src/slib_sorter.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,14 +7,19 @@
             current_dir = os.path.dirname(current_dir)
     return current_dir
 settings = os.path.join(os.environ['USERPROFILE'], 'Documents', 'WindowsPowerShell', 'Scripts', 'slib_sorter', 'settings.json')
 def check_dir(*paths):
     for path in paths:
         if not os.path.exists(path):
             os.makedirs(path)
+def check_file(*paths):
+    for path in paths:
+        if not os.path.exists(path):
+            open(path, 'w').close()
+check_file(settings)
 def join_corrected_paths(settings):
     settings_folder = os.path.join(os.environ['USERPROFILE'], 'Documents', 'WindowsPowerShell', 'Scripts', 'slib_sorter')
     settings = os.path.join(settings_folder, 'settings.json')
     with open(settings, "r") as file:
         settings = json.load(file)
 
     paths = settings.get('Paths', {})
```

