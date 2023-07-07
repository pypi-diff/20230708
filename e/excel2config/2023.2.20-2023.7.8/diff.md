# Comparing `tmp/excel2config-2023.2.20.tar.gz` & `tmp/excel2config-2023.7.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "excel2config-2023.2.20.tar", last modified: Sun Feb 19 22:00:31 2023, max compression
+gzip compressed data, was "excel2config-2023.7.8.tar", last modified: Fri Jul  7 23:38:25 2023, max compression
```

## Comparing `excel2config-2023.2.20.tar` & `excel2config-2023.7.8.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-02-19 22:00:31.724930 excel2config-2023.2.20/
--rw-rw-rw-   0        0        0     1067 2023-02-19 21:45:13.000000 excel2config-2023.2.20/LICENSE
--rw-rw-rw-   0        0        0     5559 2023-02-19 22:00:31.723602 excel2config-2023.2.20/PKG-INFO
--rw-rw-rw-   0        0        0     3664 2023-02-19 21:45:13.000000 excel2config-2023.2.20/README.md
--rw-rw-rw-   0        0        0      662 2023-02-19 21:45:13.000000 excel2config-2023.2.20/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-02-19 22:00:31.724930 excel2config-2023.2.20/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-02-19 22:00:31.655754 excel2config-2023.2.20/src/
-drwxrwxrwx   0        0        0        0 2023-02-19 22:00:31.678550 excel2config-2023.2.20/src/excel2config/
--rw-rw-rw-   0        0        0       41 2023-02-19 21:45:13.000000 excel2config-2023.2.20/src/excel2config/__init__.py
--rw-rw-rw-   0        0        0    19180 2023-02-19 21:45:13.000000 excel2config-2023.2.20/src/excel2config/excel2config.py
-drwxrwxrwx   0        0        0        0 2023-02-19 22:00:31.717915 excel2config-2023.2.20/src/excel2config.egg-info/
--rw-rw-rw-   0        0        0     5559 2023-02-19 22:00:31.000000 excel2config-2023.2.20/src/excel2config.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      336 2023-02-19 22:00:31.000000 excel2config-2023.2.20/src/excel2config.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-19 22:00:31.000000 excel2config-2023.2.20/src/excel2config.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       64 2023-02-19 22:00:31.000000 excel2config-2023.2.20/src/excel2config.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       26 2023-02-19 22:00:31.000000 excel2config-2023.2.20/src/excel2config.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-02-19 22:00:31.000000 excel2config-2023.2.20/src/excel2config.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-07 23:38:25.848821 excel2config-2023.7.8/
+-rw-rw-rw-   0        0        0     1067 2023-07-07 23:21:18.000000 excel2config-2023.7.8/LICENSE
+-rw-rw-rw-   0        0        0     5380 2023-07-07 23:38:25.847824 excel2config-2023.7.8/PKG-INFO
+-rw-rw-rw-   0        0        0     3498 2023-07-07 23:21:18.000000 excel2config-2023.7.8/README.md
+-rw-rw-rw-   0        0        0      662 2023-07-07 23:21:18.000000 excel2config-2023.7.8/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-07 23:38:25.849262 excel2config-2023.7.8/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-07 23:38:25.803242 excel2config-2023.7.8/src/
+drwxrwxrwx   0        0        0        0 2023-07-07 23:38:25.820267 excel2config-2023.7.8/src/excel2config/
+-rw-rw-rw-   0        0        0       41 2023-07-07 23:21:18.000000 excel2config-2023.7.8/src/excel2config/__init__.py
+-rw-rw-rw-   0        0        0    19143 2023-07-07 23:32:36.000000 excel2config-2023.7.8/src/excel2config/excel2config.py
+drwxrwxrwx   0        0        0        0 2023-07-07 23:38:25.843582 excel2config-2023.7.8/src/excel2config.egg-info/
+-rw-rw-rw-   0        0        0     5380 2023-07-07 23:38:25.000000 excel2config-2023.7.8/src/excel2config.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      336 2023-07-07 23:38:25.000000 excel2config-2023.7.8/src/excel2config.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-07 23:38:25.000000 excel2config-2023.7.8/src/excel2config.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       64 2023-07-07 23:38:25.000000 excel2config-2023.7.8/src/excel2config.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       26 2023-07-07 23:38:25.000000 excel2config-2023.7.8/src/excel2config.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-07-07 23:38:25.000000 excel2config-2023.7.8/src/excel2config.egg-info/top_level.txt
```

### Comparing `excel2config-2023.2.20/LICENSE` & `excel2config-2023.7.8/LICENSE`

 * *Files identical despite different names*

### Comparing `excel2config-2023.2.20/PKG-INFO` & `excel2config-2023.7.8/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: excel2config
-Version: 2023.2.20
+Version: 2023.7.8
 Summary: Generating network configuration with Excel sheets which include Jinja2 templates and data tables
 Author: Umur Arslan
 License: MIT License
         
         Copyright (c) 2022 umurarslan
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -45,30 +45,18 @@
 
 > For Windows, select the **Add Python 3.x to PATH** checkbox during installation.
 
 ---
 
 ## Installation
 
-**Option 1:** 
-
-From Python Package Index (PyPI) Repo:
-
 ```
 pip install excel2config
 ```
 
-**Option 2:** 
-
-Download project ZIP file and run below command:    
-
-```
-pip install excel2config-X.zip
-```
-
 ### Installation Check
 
 After installation **excel2config** command added to **System Path** and can be executed from any path easily as below:
 
 ```
 > excel2config -h
 usage: excel2config [-h] [excelfile]
```

### Comparing `excel2config-2023.2.20/README.md` & `excel2config-2023.7.8/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -10,30 +10,18 @@
 
 > For Windows, select the **Add Python 3.x to PATH** checkbox during installation.
 
 ---
 
 ## Installation
 
-**Option 1:** 
-
-From Python Package Index (PyPI) Repo:
-
 ```
 pip install excel2config
 ```
 
-**Option 2:** 
-
-Download project ZIP file and run below command:    
-
-```
-pip install excel2config-X.zip
-```
-
 ### Installation Check
 
 After installation **excel2config** command added to **System Path** and can be executed from any path easily as below:
 
 ```
 > excel2config -h
 usage: excel2config [-h] [excelfile]
```

### Comparing `excel2config-2023.2.20/pyproject.toml` & `excel2config-2023.7.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "excel2config"
-version = "2023.02.20"
+version = "2023.07.08"
 description = "Generating network configuration with Excel sheets which include Jinja2 templates and data tables"
 readme = "README.md"
 license = { file="LICENSE" }
 authors = [
   {name="Umur Arslan"},
 ]
```

### Comparing `excel2config-2023.2.20/src/excel2config/excel2config.py` & `excel2config-2023.7.8/src/excel2config/excel2config.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 Render excel file to text file with Jinja
 
-Version: 2023.02.20
+Version: 2023.07.08
 '''
 
 import argparse
 import ast
 import os
 import re
 import time
@@ -294,16 +294,15 @@
                 data = self._get_excel_row(sheet, row_start=3, col_start=2)
                 header = [i for i in header_w_space if i != '']
 
                 for line in data:
                     # if empty line then break
                     if all(v == '' for v in line):
                         break
-                    line_range = [self._range_text_to_list(
-                        i) for i in line if i != '']
+                    line_range = [self._range_text_to_list(i) for i in line]
 
                     line_range_product = [i for i in product(*line_range)]
 
                     for line_product in line_range_product:
                         line_render = dict(zip(header, line_product))
 
                         for key_header in line_render.keys():
```

### Comparing `excel2config-2023.2.20/src/excel2config.egg-info/PKG-INFO` & `excel2config-2023.7.8/src/excel2config.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: excel2config
-Version: 2023.2.20
+Version: 2023.7.8
 Summary: Generating network configuration with Excel sheets which include Jinja2 templates and data tables
 Author: Umur Arslan
 License: MIT License
         
         Copyright (c) 2022 umurarslan
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -45,30 +45,18 @@
 
 > For Windows, select the **Add Python 3.x to PATH** checkbox during installation.
 
 ---
 
 ## Installation
 
-**Option 1:** 
-
-From Python Package Index (PyPI) Repo:
-
 ```
 pip install excel2config
 ```
 
-**Option 2:** 
-
-Download project ZIP file and run below command:    
-
-```
-pip install excel2config-X.zip
-```
-
 ### Installation Check
 
 After installation **excel2config** command added to **System Path** and can be executed from any path easily as below:
 
 ```
 > excel2config -h
 usage: excel2config [-h] [excelfile]
```

