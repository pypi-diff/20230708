# Comparing `tmp/slib-sorter-1.5.8.tar.gz` & `tmp/slib-sorter-1.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slib-sorter-1.5.8.tar", last modified: Sat Jul  8 14:01:56 2023, max compression
+gzip compressed data, was "slib-sorter-1.5.9.tar", last modified: Sat Jul  8 14:03:45 2023, max compression
```

## Comparing `slib-sorter-1.5.8.tar` & `slib-sorter-1.5.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-08 14:01:56.159932 slib-sorter-1.5.8/
--rw-rw-rw-   0        0        0    11558 2023-07-07 20:03:54.000000 slib-sorter-1.5.8/LICENSE
--rw-rw-rw-   0        0        0     2249 2023-07-08 14:01:56.159932 slib-sorter-1.5.8/PKG-INFO
--rw-rw-rw-   0        0        0     1773 2023-07-08 06:05:27.000000 slib-sorter-1.5.8/README.md
--rw-rw-rw-   0        0        0       42 2023-07-08 14:01:56.160959 slib-sorter-1.5.8/setup.cfg
--rw-rw-rw-   0        0        0     3018 2023-07-08 14:01:32.000000 slib-sorter-1.5.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-08 14:01:56.156939 slib-sorter-1.5.8/slib_sorter.egg-info/
--rw-rw-rw-   0        0        0     2249 2023-07-08 14:01:56.000000 slib-sorter-1.5.8/slib_sorter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      273 2023-07-08 14:01:56.000000 slib-sorter-1.5.8/slib_sorter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-08 14:01:56.000000 slib-sorter-1.5.8/slib_sorter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       57 2023-07-08 14:01:56.000000 slib-sorter-1.5.8/slib_sorter.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       17 2023-07-08 14:01:56.000000 slib-sorter-1.5.8/slib_sorter.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-07-08 14:01:56.000000 slib-sorter-1.5.8/slib_sorter.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-08 14:01:56.158934 slib-sorter-1.5.8/src/
--rw-rw-rw-   0        0        0        0 2023-06-28 15:10:46.000000 slib-sorter-1.5.8/src/__init__.py
--rw-rw-rw-   0        0        0    67214 2023-07-08 13:39:36.000000 slib-sorter-1.5.8/src/slib_sorter.py
+drwxrwxrwx   0        0        0        0 2023-07-08 14:03:45.155292 slib-sorter-1.5.9/
+-rw-rw-rw-   0        0        0    11558 2023-07-07 20:03:54.000000 slib-sorter-1.5.9/LICENSE
+-rw-rw-rw-   0        0        0     2249 2023-07-08 14:03:45.154324 slib-sorter-1.5.9/PKG-INFO
+-rw-rw-rw-   0        0        0     1773 2023-07-08 06:05:27.000000 slib-sorter-1.5.9/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-08 14:03:45.155292 slib-sorter-1.5.9/setup.cfg
+-rw-rw-rw-   0        0        0     3018 2023-07-08 14:03:36.000000 slib-sorter-1.5.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-08 14:03:45.152323 slib-sorter-1.5.9/slib_sorter.egg-info/
+-rw-rw-rw-   0        0        0     2249 2023-07-08 14:03:45.000000 slib-sorter-1.5.9/slib_sorter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      273 2023-07-08 14:03:45.000000 slib-sorter-1.5.9/slib_sorter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-08 14:03:45.000000 slib-sorter-1.5.9/slib_sorter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       57 2023-07-08 14:03:45.000000 slib-sorter-1.5.9/slib_sorter.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       17 2023-07-08 14:03:45.000000 slib-sorter-1.5.9/slib_sorter.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-07-08 14:03:45.000000 slib-sorter-1.5.9/slib_sorter.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-08 14:03:45.153317 slib-sorter-1.5.9/src/
+-rw-rw-rw-   0        0        0        0 2023-06-28 15:10:46.000000 slib-sorter-1.5.9/src/__init__.py
+-rw-rw-rw-   0        0        0    67210 2023-07-08 14:03:13.000000 slib-sorter-1.5.9/src/slib_sorter.py
```

### Comparing `slib-sorter-1.5.8/LICENSE` & `slib-sorter-1.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `slib-sorter-1.5.8/PKG-INFO` & `slib-sorter-1.5.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slib-sorter
-Version: 1.5.8
+Version: 1.5.9
 Summary: A Python package for sorting Sample Libraries
 Home-page: https://github.com/nrdrch/slib-sorter
 Author: Lukas H
 Author-email: fettkindasindauchoke@gmail.com
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
```

### Comparing `slib-sorter-1.5.8/README.md` & `slib-sorter-1.5.9/README.md`

 * *Files identical despite different names*

### Comparing `slib-sorter-1.5.8/setup.py` & `slib-sorter-1.5.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,15 +57,15 @@
     
     if not os.path.exists(settings):
         with open(settings, 'w') as f:
             f.write(default_config)
     
     setuptools.setup(
         name="slib-sorter",
-        version="1.5.8",
+        version="1.5.9",
         author="Lukas H",
         author_email="fettkindasindauchoke@gmail.com",
         description="A Python package for sorting Sample Libraries",
         long_description=long_description,
         long_description_content_type="text/markdown",
         url="https://github.com/nrdrch/slib-sorter",
         packages=setuptools.find_packages(),
```

### Comparing `slib-sorter-1.5.8/slib_sorter.egg-info/PKG-INFO` & `slib-sorter-1.5.9/slib_sorter.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slib-sorter
-Version: 1.5.8
+Version: 1.5.9
 Summary: A Python package for sorting Sample Libraries
 Home-page: https://github.com/nrdrch/slib-sorter
 Author: Lukas H
 Author-email: fettkindasindauchoke@gmail.com
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
```

### Comparing `slib-sorter-1.5.8/src/slib_sorter.py` & `slib-sorter-1.5.9/src/slib_sorter.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,16 +36,16 @@
     clors = settings.get('Colors', {})
     parsed_clors = {}
     for key, value in clors.items():
         parsed_clors[key] = value
     return parsed_clors
 #settings = os.path.join(path_finder(0), 'settings.json')
 
-j_clrs = clr_get(settings_f)
-j_paths = join_corrected_paths(settings_f)
+j_clrs = clr_get(settings)
+j_paths = join_corrected_paths(settings)
 with open(settings, 'r') as file:
     settings = json.load(file)
 
 def log_message(message, color, centered=False, newline=True):
     if centered:
         message = message.center(119)
     end = "\n" if newline else ""
```

