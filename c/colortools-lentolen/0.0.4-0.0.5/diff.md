# Comparing `tmp/colortools_lentolen-0.0.4.tar.gz` & `tmp/colortools_lentolen-0.0.5.tar.gz`

## Comparing `colortools_lentolen-0.0.4.tar` & `colortools_lentolen-0.0.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 colortools_lentolen-0.0.4/src/colortools/__about__.py
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 colortools_lentolen-0.0.4/src/colortools/__init__.py
--rw-r--r--   0        0        0    26129 2020-02-02 00:00:00.000000 colortools_lentolen-0.0.4/src/colortools/color_utils.py
--rw-r--r--   0        0        0    29823 2020-02-02 00:00:00.000000 colortools_lentolen-0.0.4/src/colortools/data/color-meanings.com.csv
--rw-r--r--   0        0        0     2962 2020-02-02 00:00:00.000000 colortools_lentolen-0.0.4/src/colortools/data/html-ger.csv
--rw-r--r--   0        0        0     2714 2020-02-02 00:00:00.000000 colortools_lentolen-0.0.4/src/colortools/data/html.csv
--rw-r--r--   0        0        0   658468 2020-02-02 00:00:00.000000 colortools_lentolen-0.0.4/src/colortools/data/meodai.csv
--rw-r--r--   0        0        0     9471 2020-02-02 00:00:00.000000 colortools_lentolen-0.0.4/src/colortools/data/x11.csv
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 colortools_lentolen-0.0.4/tests/__init__.py
--rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 colortools_lentolen-0.0.4/LICENSE.txt
--rw-r--r--   0        0        0     2384 2020-02-02 00:00:00.000000 colortools_lentolen-0.0.4/README.md
--rw-r--r--   0        0        0     3263 2020-02-02 00:00:00.000000 colortools_lentolen-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     3343 2020-02-02 00:00:00.000000 colortools_lentolen-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 colortools_lentolen-0.0.5/src/colortools/__about__.py
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 colortools_lentolen-0.0.5/src/colortools/__init__.py
+-rw-r--r--   0        0        0    26131 2020-02-02 00:00:00.000000 colortools_lentolen-0.0.5/src/colortools/color_utils.py
+-rw-r--r--   0        0        0    29823 2020-02-02 00:00:00.000000 colortools_lentolen-0.0.5/src/colortools/data/color-meanings.com.csv
+-rw-r--r--   0        0        0     2962 2020-02-02 00:00:00.000000 colortools_lentolen-0.0.5/src/colortools/data/html-ger.csv
+-rw-r--r--   0        0        0     2714 2020-02-02 00:00:00.000000 colortools_lentolen-0.0.5/src/colortools/data/html.csv
+-rw-r--r--   0        0        0   658468 2020-02-02 00:00:00.000000 colortools_lentolen-0.0.5/src/colortools/data/meodai.csv
+-rw-r--r--   0        0        0     9471 2020-02-02 00:00:00.000000 colortools_lentolen-0.0.5/src/colortools/data/x11.csv
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 colortools_lentolen-0.0.5/tests/__init__.py
+-rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 colortools_lentolen-0.0.5/LICENSE.txt
+-rw-r--r--   0        0        0     2384 2020-02-02 00:00:00.000000 colortools_lentolen-0.0.5/README.md
+-rw-r--r--   0        0        0     3263 2020-02-02 00:00:00.000000 colortools_lentolen-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     3343 2020-02-02 00:00:00.000000 colortools_lentolen-0.0.5/PKG-INFO
```

### Comparing `colortools_lentolen-0.0.4/src/colortools/color_utils.py` & `colortools_lentolen-0.0.5/src/colortools/color_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -994,15 +994,15 @@
         reader = csv.reader(file)
         for row in reader:
             color_name = row[0]
             hex_code = row[1]
             color_dict[color_name] = hex_code
     
     for color_name, hex_code in color_dict.items():
-        if colorname.lower == color_name.lower():
+        if colorname.lower() == color_name.lower():
             return hex_code
         
     return None
 
 def rgb_to_colorname(rgb: tuple, naming_standard="html"):
     """
     Find the closest matching color name for a given rgb color tuple in a color name system.
```

### Comparing `colortools_lentolen-0.0.4/src/colortools/data/color-meanings.com.csv` & `colortools_lentolen-0.0.5/src/colortools/data/color-meanings.com.csv`

 * *Files identical despite different names*

### Comparing `colortools_lentolen-0.0.4/src/colortools/data/html-ger.csv` & `colortools_lentolen-0.0.5/src/colortools/data/html-ger.csv`

 * *Files identical despite different names*

### Comparing `colortools_lentolen-0.0.4/src/colortools/data/html.csv` & `colortools_lentolen-0.0.5/src/colortools/data/html.csv`

 * *Files identical despite different names*

### Comparing `colortools_lentolen-0.0.4/src/colortools/data/meodai.csv` & `colortools_lentolen-0.0.5/src/colortools/data/meodai.csv`

 * *Files identical despite different names*

### Comparing `colortools_lentolen-0.0.4/src/colortools/data/x11.csv` & `colortools_lentolen-0.0.5/src/colortools/data/x11.csv`

 * *Files identical despite different names*

### Comparing `colortools_lentolen-0.0.4/LICENSE.txt` & `colortools_lentolen-0.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `colortools_lentolen-0.0.4/README.md` & `colortools_lentolen-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `colortools_lentolen-0.0.4/pyproject.toml` & `colortools_lentolen-0.0.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `colortools_lentolen-0.0.4/PKG-INFO` & `colortools_lentolen-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: colortools_lentolen
-Version: 0.0.4
+Version: 0.0.5
 Summary: A package to do color conversions and comparisons
 Project-URL: Documentation, https://github.com/LentoLen/colortools#readme
 Project-URL: Issues, https://github.com/LentoLen/colortools/issues
 Project-URL: Source, https://github.com/LentoLen/colortools
 Author-email: LentoLen <len.vnn@gmail.com>
 License-Expression: MIT
 License-File: LICENSE.txt
```

