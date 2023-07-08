# Comparing `tmp/slib-sorter-1.3.6.tar.gz` & `tmp/slib-sorter-1.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slib-sorter-1.3.6.tar", last modified: Sat Jul  8 08:59:54 2023, max compression
+gzip compressed data, was "slib-sorter-1.3.7.tar", last modified: Sat Jul  8 09:11:14 2023, max compression
```

## Comparing `slib-sorter-1.3.6.tar` & `slib-sorter-1.3.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-08 08:59:54.263223 slib-sorter-1.3.6/
--rw-rw-rw-   0        0        0    11558 2023-07-07 20:03:54.000000 slib-sorter-1.3.6/LICENSE
--rw-rw-rw-   0        0        0     2249 2023-07-08 08:59:54.263223 slib-sorter-1.3.6/PKG-INFO
--rw-rw-rw-   0        0        0     1773 2023-07-08 06:05:27.000000 slib-sorter-1.3.6/README.md
--rw-rw-rw-   0        0        0       42 2023-07-08 08:59:54.263223 slib-sorter-1.3.6/setup.cfg
--rw-rw-rw-   0        0        0     3056 2023-07-08 08:59:43.000000 slib-sorter-1.3.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-08 08:59:54.254238 slib-sorter-1.3.6/slib_sorter.egg-info/
--rw-rw-rw-   0        0        0     2249 2023-07-08 08:59:54.000000 slib-sorter-1.3.6/slib_sorter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      273 2023-07-08 08:59:54.000000 slib-sorter-1.3.6/slib_sorter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-08 08:59:54.000000 slib-sorter-1.3.6/slib_sorter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       57 2023-07-08 08:59:54.000000 slib-sorter-1.3.6/slib_sorter.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       17 2023-07-08 08:59:54.000000 slib-sorter-1.3.6/slib_sorter.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-07-08 08:59:54.000000 slib-sorter-1.3.6/slib_sorter.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-08 08:59:54.262232 slib-sorter-1.3.6/src/
--rw-rw-rw-   0        0        0        0 2023-06-28 15:10:46.000000 slib-sorter-1.3.6/src/__init__.py
--rw-rw-rw-   0        0        0    63301 2023-07-08 08:59:24.000000 slib-sorter-1.3.6/src/slib_sorter.py
+drwxrwxrwx   0        0        0        0 2023-07-08 09:11:14.618584 slib-sorter-1.3.7/
+-rw-rw-rw-   0        0        0    11558 2023-07-07 20:03:54.000000 slib-sorter-1.3.7/LICENSE
+-rw-rw-rw-   0        0        0     2249 2023-07-08 09:11:14.618584 slib-sorter-1.3.7/PKG-INFO
+-rw-rw-rw-   0        0        0     1773 2023-07-08 06:05:27.000000 slib-sorter-1.3.7/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-08 09:11:14.618584 slib-sorter-1.3.7/setup.cfg
+-rw-rw-rw-   0        0        0     3056 2023-07-08 09:04:17.000000 slib-sorter-1.3.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-08 09:11:14.608583 slib-sorter-1.3.7/slib_sorter.egg-info/
+-rw-rw-rw-   0        0        0     2249 2023-07-08 09:11:14.000000 slib-sorter-1.3.7/slib_sorter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      273 2023-07-08 09:11:14.000000 slib-sorter-1.3.7/slib_sorter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-08 09:11:14.000000 slib-sorter-1.3.7/slib_sorter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       57 2023-07-08 09:11:14.000000 slib-sorter-1.3.7/slib_sorter.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       17 2023-07-08 09:11:14.000000 slib-sorter-1.3.7/slib_sorter.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-07-08 09:11:14.000000 slib-sorter-1.3.7/slib_sorter.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-08 09:11:14.617584 slib-sorter-1.3.7/src/
+-rw-rw-rw-   0        0        0        0 2023-06-28 15:10:46.000000 slib-sorter-1.3.7/src/__init__.py
+-rw-rw-rw-   0        0        0    63625 2023-07-08 09:10:55.000000 slib-sorter-1.3.7/src/slib_sorter.py
```

### Comparing `slib-sorter-1.3.6/LICENSE` & `slib-sorter-1.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `slib-sorter-1.3.6/PKG-INFO` & `slib-sorter-1.3.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slib-sorter
-Version: 1.3.6
+Version: 1.3.7
 Summary: A Python package for sorting Sample Libraries
 Home-page: https://github.com/nrdrch/slib-sorter
 Author: Lukas H
 Author-email: fettkindasindauchoke@gmail.com
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
```

### Comparing `slib-sorter-1.3.6/README.md` & `slib-sorter-1.3.7/README.md`

 * *Files identical despite different names*

### Comparing `slib-sorter-1.3.6/setup.py` & `slib-sorter-1.3.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,15 +52,15 @@
 ''' 
             f.write(default_config)
     else:
         pass
 
     setuptools.setup(
         name="slib-sorter",
-        version="1.3.6",
+        version="1.3.7",
         author="Lukas H",
         author_email="fettkindasindauchoke@gmail.com",
         description="A Python package for sorting Sample Libraries",
         long_description=long_description,
         long_description_content_type="text/markdown",
         url="https://github.com/nrdrch/slib-sorter",
         packages=setuptools.find_packages(),
```

### Comparing `slib-sorter-1.3.6/slib_sorter.egg-info/PKG-INFO` & `slib-sorter-1.3.7/slib_sorter.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slib-sorter
-Version: 1.3.6
+Version: 1.3.7
 Summary: A Python package for sorting Sample Libraries
 Home-page: https://github.com/nrdrch/slib-sorter
 Author: Lukas H
 Author-email: fettkindasindauchoke@gmail.com
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
```

### Comparing `slib-sorter-1.3.6/src/slib_sorter.py` & `slib-sorter-1.3.7/src/slib_sorter.py`

 * *Files 1% similar despite different names*

```diff
@@ -1004,32 +1004,41 @@
     parser.add_argument("-config", action="store_true")
     temp_file_path = temp_path_file(temp_content)
     args = parser.parse_args()
     spacer = "              "
     if args.paths:
         with open(temp_file_path, 'r') as file:
             temp_file_path = file.read()
-        os.system('cls')
+        if settings.get("Run Shell Command On Startup", True):
+            os.system(CmdOnStartup)
+        else:
+            pass
         bar = settings.get("Top Title Bar")
         log_message(bar, f'{j_clrs.get("Top Title Bar Color")}', True, True)
         log_message(temp_content, 'white', False, True)
     elif args.colors:
-        os.system('cls')
+        if settings.get("Run Shell Command On Startup", True):
+            os.system(CmdOnStartup)
+        else:
+            pass
         bar = settings.get("Top Title Bar")
         log_message(bar, f'{j_clrs.get("Top Title Bar Color")}', True, True)
         clist = {
             "Colors": ['black', 'red', 'green', 'yellow', 'blue', 'magenta', 'cyan', 'white', 'light_grey', 'dark_grey', 'light_red', 'light_green', 'light_yellow', 'light_blue', 'light_magenta', 'light_cyan']
         }
         colors = clist["Colors"]
         log_message("Possible Color Settings", f'{j_clrs.get("Statistics Value Color")}', False, False)
         log_message(':', f'{j_clrs.get("Foregroud Color 1")}', False, True)
         for color in colors:
             log_message(spacer+ color, f'{color}', False, True)
     elif args.help:
-        os.system('cls')
+        if settings.get("Run Shell Command On Startup", True):
+            os.system(CmdOnStartup)
+        else:
+            pass
         bar = settings.get("Top Title Bar")
         log_message(bar, f'{j_clrs.get("Top Title Bar Color")}', True, True)
         log_message('Help', f'{j_clrs.get("Statistics Value Color")}', False, False)
         log_message(':', f'{j_clrs.get("Foregroud Color 1")}', False, True)
         log_message('           -paths '+ f'{spacer}', f'{j_clrs.get("Foregroud Color 1")}', False, False)
         log_message('Displays Paths', f'{j_clrs.get("Statistics Value Color")}', False, True)
         log_message('           -colors'+ f'{spacer}', f'{j_clrs.get("Foregroud Color 1")}', False, False)
```

