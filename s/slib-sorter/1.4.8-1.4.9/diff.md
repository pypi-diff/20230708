# Comparing `tmp/slib-sorter-1.4.8.tar.gz` & `tmp/slib-sorter-1.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slib-sorter-1.4.8.tar", last modified: Sat Jul  8 11:40:59 2023, max compression
+gzip compressed data, was "slib-sorter-1.4.9.tar", last modified: Sat Jul  8 11:42:27 2023, max compression
```

## Comparing `slib-sorter-1.4.8.tar` & `slib-sorter-1.4.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-08 11:40:59.368414 slib-sorter-1.4.8/
--rw-rw-rw-   0        0        0    11558 2023-07-07 20:03:54.000000 slib-sorter-1.4.8/LICENSE
--rw-rw-rw-   0        0        0     2249 2023-07-08 11:40:59.367418 slib-sorter-1.4.8/PKG-INFO
--rw-rw-rw-   0        0        0     1773 2023-07-08 06:05:27.000000 slib-sorter-1.4.8/README.md
--rw-rw-rw-   0        0        0       42 2023-07-08 11:40:59.368414 slib-sorter-1.4.8/setup.cfg
--rw-rw-rw-   0        0        0     3242 2023-07-08 11:40:52.000000 slib-sorter-1.4.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-08 11:40:59.357401 slib-sorter-1.4.8/slib_sorter.egg-info/
--rw-rw-rw-   0        0        0     2249 2023-07-08 11:40:59.000000 slib-sorter-1.4.8/slib_sorter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      273 2023-07-08 11:40:59.000000 slib-sorter-1.4.8/slib_sorter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-08 11:40:59.000000 slib-sorter-1.4.8/slib_sorter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       57 2023-07-08 11:40:59.000000 slib-sorter-1.4.8/slib_sorter.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       17 2023-07-08 11:40:59.000000 slib-sorter-1.4.8/slib_sorter.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-07-08 11:40:59.000000 slib-sorter-1.4.8/slib_sorter.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-08 11:40:59.366402 slib-sorter-1.4.8/src/
--rw-rw-rw-   0        0        0        0 2023-06-28 15:10:46.000000 slib-sorter-1.4.8/src/__init__.py
--rw-rw-rw-   0        0        0    67146 2023-07-08 11:40:39.000000 slib-sorter-1.4.8/src/slib_sorter.py
+drwxrwxrwx   0        0        0        0 2023-07-08 11:42:27.001710 slib-sorter-1.4.9/
+-rw-rw-rw-   0        0        0    11558 2023-07-07 20:03:54.000000 slib-sorter-1.4.9/LICENSE
+-rw-rw-rw-   0        0        0     2249 2023-07-08 11:42:27.001710 slib-sorter-1.4.9/PKG-INFO
+-rw-rw-rw-   0        0        0     1773 2023-07-08 06:05:27.000000 slib-sorter-1.4.9/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-08 11:42:27.001710 slib-sorter-1.4.9/setup.cfg
+-rw-rw-rw-   0        0        0     3242 2023-07-08 11:41:52.000000 slib-sorter-1.4.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-08 11:42:26.991737 slib-sorter-1.4.9/slib_sorter.egg-info/
+-rw-rw-rw-   0        0        0     2249 2023-07-08 11:42:26.000000 slib-sorter-1.4.9/slib_sorter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      273 2023-07-08 11:42:26.000000 slib-sorter-1.4.9/slib_sorter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-08 11:42:26.000000 slib-sorter-1.4.9/slib_sorter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       57 2023-07-08 11:42:26.000000 slib-sorter-1.4.9/slib_sorter.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       17 2023-07-08 11:42:26.000000 slib-sorter-1.4.9/slib_sorter.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-07-08 11:42:26.000000 slib-sorter-1.4.9/slib_sorter.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-08 11:42:27.000741 slib-sorter-1.4.9/src/
+-rw-rw-rw-   0        0        0        0 2023-06-28 15:10:46.000000 slib-sorter-1.4.9/src/__init__.py
+-rw-rw-rw-   0        0        0    67147 2023-07-08 11:41:49.000000 slib-sorter-1.4.9/src/slib_sorter.py
```

### Comparing `slib-sorter-1.4.8/LICENSE` & `slib-sorter-1.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `slib-sorter-1.4.8/PKG-INFO` & `slib-sorter-1.4.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slib-sorter
-Version: 1.4.8
+Version: 1.4.9
 Summary: A Python package for sorting Sample Libraries
 Home-page: https://github.com/nrdrch/slib-sorter
 Author: Lukas H
 Author-email: fettkindasindauchoke@gmail.com
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
```

### Comparing `slib-sorter-1.4.8/README.md` & `slib-sorter-1.4.9/README.md`

 * *Files identical despite different names*

### Comparing `slib-sorter-1.4.8/setup.py` & `slib-sorter-1.4.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -56,15 +56,15 @@
 ''' 
         f.write(default_config)
     else:
         pass
 
     setuptools.setup(
         name="slib-sorter",
-        version="1.4.8",
+        version="1.4.9",
         author="Lukas H",
         author_email="fettkindasindauchoke@gmail.com",
         description="A Python package for sorting Sample Libraries",
         long_description=long_description,
         long_description_content_type="text/markdown",
         url="https://github.com/nrdrch/slib-sorter",
         packages=setuptools.find_packages(),
```

### Comparing `slib-sorter-1.4.8/slib_sorter.egg-info/PKG-INFO` & `slib-sorter-1.4.9/slib_sorter.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slib-sorter
-Version: 1.4.8
+Version: 1.4.9
 Summary: A Python package for sorting Sample Libraries
 Home-page: https://github.com/nrdrch/slib-sorter
 Author: Lukas H
 Author-email: fettkindasindauchoke@gmail.com
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
```

### Comparing `slib-sorter-1.4.8/src/slib_sorter.py` & `slib-sorter-1.4.9/src/slib_sorter.py`

 * *Files 0% similar despite different names*

```diff
@@ -960,15 +960,15 @@
         pass
     
     if settings.get("Show Statistics", True):
         log_message(prompt1, j_clrs.get('Prompt Color'), False, False)
         log_message(f'sorted by name & file type:   ', j_clrs.get('Foreground Color 1'), False, False)
         log_message(f' {num_succeeded}', j_clrs.get('Successfully Sorted File Color'), False, True)
         log_message(prompt1, j_clrs.get('Prompt Color'), False, False)
-        log_message(f'sorted only by file type: ', j_clrs.get('Foreground Color 1'), False, True)
+        log_message(f'sorted only by file type: ', j_clrs.get('Foreground Color 1'), False, False)
         log_message(f' {num_failed}', j_clrs.get('Unsorted File Color'), False, True)
         log_message(prompt1, j_clrs.get('Prompt Color'), False, False)
         log_message(f'rejected file types: ', j_clrs.get('Foreground Color 1'), False, False)
         log_message(f' {num_failed2}', j_clrs.get('Rejected Filetype Color'), False, True)
         log_message(f'      {total}', j_clrs.get('Statistics Value Color'), False, False)
         log_message(f' files processed in ', j_clrs.get('Foreground Color 2'), False, False)
         log_message(f'{elapsed_time:.2f}', j_clrs.get('Statistics Value Color'), False, False)
```

