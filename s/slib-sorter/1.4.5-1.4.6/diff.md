# Comparing `tmp/slib-sorter-1.4.5.tar.gz` & `tmp/slib-sorter-1.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slib-sorter-1.4.5.tar", last modified: Sat Jul  8 11:18:01 2023, max compression
+gzip compressed data, was "slib-sorter-1.4.6.tar", last modified: Sat Jul  8 11:25:38 2023, max compression
```

## Comparing `slib-sorter-1.4.5.tar` & `slib-sorter-1.4.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-08 11:18:01.518013 slib-sorter-1.4.5/
--rw-rw-rw-   0        0        0    11558 2023-07-07 20:03:54.000000 slib-sorter-1.4.5/LICENSE
--rw-rw-rw-   0        0        0     2249 2023-07-08 11:18:01.518013 slib-sorter-1.4.5/PKG-INFO
--rw-rw-rw-   0        0        0     1773 2023-07-08 06:05:27.000000 slib-sorter-1.4.5/README.md
--rw-rw-rw-   0        0        0       42 2023-07-08 11:18:01.518013 slib-sorter-1.4.5/setup.cfg
--rw-rw-rw-   0        0        0     3242 2023-07-08 11:17:50.000000 slib-sorter-1.4.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-08 11:18:01.508018 slib-sorter-1.4.5/slib_sorter.egg-info/
--rw-rw-rw-   0        0        0     2249 2023-07-08 11:18:01.000000 slib-sorter-1.4.5/slib_sorter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      273 2023-07-08 11:18:01.000000 slib-sorter-1.4.5/slib_sorter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-08 11:18:01.000000 slib-sorter-1.4.5/slib_sorter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       57 2023-07-08 11:18:01.000000 slib-sorter-1.4.5/slib_sorter.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       17 2023-07-08 11:18:01.000000 slib-sorter-1.4.5/slib_sorter.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-07-08 11:18:01.000000 slib-sorter-1.4.5/slib_sorter.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-08 11:18:01.517010 slib-sorter-1.4.5/src/
--rw-rw-rw-   0        0        0        0 2023-06-28 15:10:46.000000 slib-sorter-1.4.5/src/__init__.py
--rw-rw-rw-   0        0        0    67249 2023-07-08 11:17:10.000000 slib-sorter-1.4.5/src/slib_sorter.py
+drwxrwxrwx   0        0        0        0 2023-07-08 11:25:38.353706 slib-sorter-1.4.6/
+-rw-rw-rw-   0        0        0    11558 2023-07-07 20:03:54.000000 slib-sorter-1.4.6/LICENSE
+-rw-rw-rw-   0        0        0     2249 2023-07-08 11:25:38.353706 slib-sorter-1.4.6/PKG-INFO
+-rw-rw-rw-   0        0        0     1773 2023-07-08 06:05:27.000000 slib-sorter-1.4.6/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-08 11:25:38.353706 slib-sorter-1.4.6/setup.cfg
+-rw-rw-rw-   0        0        0     3242 2023-07-08 11:25:24.000000 slib-sorter-1.4.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-08 11:25:38.350673 slib-sorter-1.4.6/slib_sorter.egg-info/
+-rw-rw-rw-   0        0        0     2249 2023-07-08 11:25:38.000000 slib-sorter-1.4.6/slib_sorter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      273 2023-07-08 11:25:38.000000 slib-sorter-1.4.6/slib_sorter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-08 11:25:38.000000 slib-sorter-1.4.6/slib_sorter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       57 2023-07-08 11:25:38.000000 slib-sorter-1.4.6/slib_sorter.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       17 2023-07-08 11:25:38.000000 slib-sorter-1.4.6/slib_sorter.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-07-08 11:25:38.000000 slib-sorter-1.4.6/slib_sorter.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-08 11:25:38.352697 slib-sorter-1.4.6/src/
+-rw-rw-rw-   0        0        0        0 2023-06-28 15:10:46.000000 slib-sorter-1.4.6/src/__init__.py
+-rw-rw-rw-   0        0        0    67155 2023-07-08 11:24:49.000000 slib-sorter-1.4.6/src/slib_sorter.py
```

### Comparing `slib-sorter-1.4.5/LICENSE` & `slib-sorter-1.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `slib-sorter-1.4.5/PKG-INFO` & `slib-sorter-1.4.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slib-sorter
-Version: 1.4.5
+Version: 1.4.6
 Summary: A Python package for sorting Sample Libraries
 Home-page: https://github.com/nrdrch/slib-sorter
 Author: Lukas H
 Author-email: fettkindasindauchoke@gmail.com
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
```

### Comparing `slib-sorter-1.4.5/README.md` & `slib-sorter-1.4.6/README.md`

 * *Files identical despite different names*

### Comparing `slib-sorter-1.4.5/setup.py` & `slib-sorter-1.4.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -56,15 +56,15 @@
 ''' 
         f.write(default_config)
     else:
         pass
 
     setuptools.setup(
         name="slib-sorter",
-        version="1.4.5",
+        version="1.4.6",
         author="Lukas H",
         author_email="fettkindasindauchoke@gmail.com",
         description="A Python package for sorting Sample Libraries",
         long_description=long_description,
         long_description_content_type="text/markdown",
         url="https://github.com/nrdrch/slib-sorter",
         packages=setuptools.find_packages(),
```

### Comparing `slib-sorter-1.4.5/slib_sorter.egg-info/PKG-INFO` & `slib-sorter-1.4.6/slib_sorter.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slib-sorter
-Version: 1.4.5
+Version: 1.4.6
 Summary: A Python package for sorting Sample Libraries
 Home-page: https://github.com/nrdrch/slib-sorter
 Author: Lukas H
 Author-email: fettkindasindauchoke@gmail.com
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
```

### Comparing `slib-sorter-1.4.5/src/slib_sorter.py` & `slib-sorter-1.4.6/src/slib_sorter.py`

 * *Files 1% similar despite different names*

```diff
@@ -956,43 +956,43 @@
     if settings.get("Show Top Title Bar", True):
         bar = settings.get("Top Title Bar")
         log_message(bar, j_clrs.get('Top Title Bar Color'), True, True)
     else:
         pass
     
     if settings.get("Show Statistics", True):
-        log_message(prompt1, f'{j_clrs.get("Prompt Color")}', False, False)
-        log_message(f'sorted by name & file type:   ', f'{j_clrs.get("Foreground Color 1")}', False, False)
-        log_message(f' {num_succeeded}', f'{j_clrs.get("Successfully Sorted File Color")}')
-        log_message(prompt1, f'{j_clrs.get("Prompt Color")}', False, False)
-        log_message(f'sorted only by file type: ', f'{j_clrs.get("Foreground Color 1")}', False, False)
-        log_message(f' {num_failed}', f'{j_clrs.get("Unsorted File Color")}')
-        log_message(prompt1, f'{j_clrs.get("Prompt Color")}', False, False)
-        log_message(f'rejected file types: ', f'{j_clrs.get("Foreground Color 1")}', False, False)
-        log_message(f' {num_failed2}', f'{j_clrs.get("Rejected Filetype Color")}')
-        log_message(f'      {total}', f'{j_clrs.get("Statistics Value Color")}', False, False)
-        log_message(f' files processed in ', f'{j_clrs.get("Foreground Color 2")}', False, False)
-        log_message(f'{elapsed_time:.2f}', f'{j_clrs.get("Statistics Value Color")}', False, False)
-        log_message(f' seconds', f'{j_clrs.get("Foreground Color 1")}', False, True)
+        log_message(prompt1, j_clrs.get('Prompt Color'), False, False)
+        log_message(f'sorted by name & file type:   ', j_clrs.get('Foreground Color 1'), False, False)
+        log_message(f' {num_succeeded}', j_clrs.get('Successfully Sorted File Color'), False, False)
+        log_message(prompt1, j_clrs.get('Prompt Color'), False, False)
+        log_message(f'sorted only by file type: ', j_clrs.get('Foreground Color 1'), False, False)
+        log_message(f' {num_failed}', j_clrs.get('Unsorted File Color'), False, False)
+        log_message(prompt1, j_clrs.get('Prompt Color'), False, False)
+        log_message(f'rejected file types: ', j_clrs.get('Foreground Color 1'), False, False)
+        log_message(f' {num_failed2}', j_clrs.get('Rejected Filetype Color'), False, False)
+        log_message(f'      {total}', j_clrs.get('Statistics Value Color'), False, False)
+        log_message(f' files processed in ', j_clrs.get('Foreground Color 2'), False, False)
+        log_message(f'{elapsed_time:.2f}', j_clrs.get('Statistics Value Color'), False, False)
+        log_message(f' seconds', j_clrs.get('Foreground Color 1'), False, True)
         maxfile = settings.get('Max files per Dir')
         split_files_in_subdirectories(path2, max_files_per_dir=maxfile)
         file_count, dir_count, total_size_mb, total_size_gb = count_files_in_directory(path2)
-        log_message(f'          in ', f'{j_clrs.get("Foreground Color 2")}', False, False)
-        log_message(f'{settings.get("Name Of Top Library Directory")}', f'{j_clrs.get("Statistics Value Color")}', False, True)
-        log_message(f'              files', f'{j_clrs.get("Foreground Color 2")}', False, False)
-        log_message(f' {file_count}', f'{j_clrs.get("Statistics Value Color")}', False, True)
-        log_message(f'                  subdirectories', f'{j_clrs.get("Foreground Color 2")}', False, False)
-        log_message(f' {dir_count}', f'{j_clrs.get("Statistics Value Color")}', False, True)
-        log_message(f'                      size', f'{j_clrs.get("Foreground Color 2")}', False, False)
-        log_message(f' {total_size_mb:.2f}', f'{j_clrs.get("Statistics Value Color")}', False, False)
-        log_message(f' mb ', f'{j_clrs.get("Foreground Color 1")}', False, False)
-        log_message(f'or ', f'{j_clrs.get("Foreground Color 2")}', False, False)
-        log_message(f'{total_size_gb:.2f}', f'{j_clrs.get("Statistics Value Color")}', False, False)
-        log_message(f' gb', f'{j_clrs.get("Foreground Color 1")}', False, False)
-        log_message(f'', f'{j_clrs.get("Foreground Color 1")}', False, True)
+        log_message(f'          in ', j_clrs.get('Foreground Color 2'), False, False)
+        log_message(j_paths.get('Name Of Top Library Directory'), j_clrs.get('Statistics Value Color'), False, True)
+        log_message(f'              files', j_clrs.get('Foreground Color 2'), False, False)
+        log_message(f' {file_count}', j_clrs.get('Statistics Value Color'), False, True)
+        log_message(f'                  subdirectories', j_clrs.get('Foreground Color 2'), False, False)
+        log_message(f' {dir_count}', j_clrs.get('Statistics Value Color'), False, True)
+        log_message(f'                      size', j_clrs.get('Foreground Color 2'), False, False)
+        log_message(f' {total_size_mb:.2f}', j_clrs.get('Statistics Value Color'), False, False)
+        log_message(f' mb ', j_clrs.get('Foreground Color 1'), False, False)
+        log_message(f'or ', j_clrs.get('Foreground Color 2'), False, False)
+        log_message(f'{total_size_gb:.2f}', j_clrs.get('Statistics Value Color'), False, False)
+        log_message(f' gb', j_clrs.get('Foreground Color 1'), False, False)
+        log_message(f'', j_clrs.get('Foreground Color 1'), False, True)
     else:
         pass
     def remove_readonly(func, path, _):
         os.chmod(path, stat.S_IWRITE)
         func(path)
     shutil.rmtree(path1, onerror=remove_readonly)
     check_dir(path1)
```

