# Comparing `tmp/LordPath-2023.5.6.4.tar.gz` & `tmp/LordPath-2023.7.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LordPath-2023.5.6.4.tar", last modified: Sat May  6 13:47:15 2023, max compression
+gzip compressed data, was "LordPath-2023.7.8.tar", last modified: Sat Jul  8 11:08:55 2023, max compression
```

## Comparing `LordPath-2023.5.6.4.tar` & `LordPath-2023.7.8.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxr-xr-x   0 philippkitzmuller   (501) staff       (20)        0 2023-05-06 13:47:15.489013 LordPath-2023.5.6.4/
-drwxr-xr-x   0 philippkitzmuller   (501) staff       (20)        0 2023-05-06 13:47:15.484317 LordPath-2023.5.6.4/LordPath/
--rw-r--r--   0 philippkitzmuller   (501) staff       (20)     3483 2023-05-06 13:46:10.000000 LordPath-2023.5.6.4/LordPath/__init__.py
--rw-r--r--   0 philippkitzmuller   (501) staff       (20)      617 2022-12-09 23:13:08.000000 LordPath-2023.5.6.4/LordPath/dataset.py
--rw-r--r--   0 philippkitzmuller   (501) staff       (20)      583 2023-03-21 08:46:08.000000 LordPath-2023.5.6.4/LordPath/descriptors.py
--rw-r--r--   0 philippkitzmuller   (501) staff       (20)     6385 2023-03-17 16:32:55.000000 LordPath-2023.5.6.4/LordPath/filefolderclass.py
-drwxr-xr-x   0 philippkitzmuller   (501) staff       (20)        0 2023-05-06 13:47:15.488299 LordPath-2023.5.6.4/LordPath/opener/
--rw-r--r--   0 philippkitzmuller   (501) staff       (20)     1051 2023-05-04 14:21:50.000000 LordPath-2023.5.6.4/LordPath/opener/__init__.py
--rw-r--r--   0 philippkitzmuller   (501) staff       (20)      328 2023-03-17 16:42:56.000000 LordPath-2023.5.6.4/LordPath/opener/base.py
--rw-r--r--   0 philippkitzmuller   (501) staff       (20)      868 2023-03-17 16:42:56.000000 LordPath-2023.5.6.4/LordPath/opener/json.py
--rw-r--r--   0 philippkitzmuller   (501) staff       (20)      864 2023-03-17 16:42:56.000000 LordPath-2023.5.6.4/LordPath/opener/pickle.py
--rw-r--r--   0 philippkitzmuller   (501) staff       (20)      490 2023-03-17 16:42:56.000000 LordPath-2023.5.6.4/LordPath/opener/toml.py
--rw-r--r--   0 philippkitzmuller   (501) staff       (20)     1019 2023-03-16 23:58:05.000000 LordPath-2023.5.6.4/LordPath/opener/yaml.py
-drwxr-xr-x   0 philippkitzmuller   (501) staff       (20)        0 2023-05-06 13:47:15.485556 LordPath-2023.5.6.4/LordPath.egg-info/
--rw-r--r--   0 philippkitzmuller   (501) staff       (20)      465 2023-05-06 13:47:15.000000 LordPath-2023.5.6.4/LordPath.egg-info/PKG-INFO
--rw-r--r--   0 philippkitzmuller   (501) staff       (20)      427 2023-05-06 13:47:15.000000 LordPath-2023.5.6.4/LordPath.egg-info/SOURCES.txt
--rw-r--r--   0 philippkitzmuller   (501) staff       (20)        1 2023-05-06 13:47:15.000000 LordPath-2023.5.6.4/LordPath.egg-info/dependency_links.txt
--rw-r--r--   0 philippkitzmuller   (501) staff       (20)       23 2023-05-06 13:47:15.000000 LordPath-2023.5.6.4/LordPath.egg-info/requires.txt
--rw-r--r--   0 philippkitzmuller   (501) staff       (20)        9 2023-05-06 13:47:15.000000 LordPath-2023.5.6.4/LordPath.egg-info/top_level.txt
--rw-r--r--   0 philippkitzmuller   (501) staff       (20)      465 2023-05-06 13:47:15.488837 LordPath-2023.5.6.4/PKG-INFO
--rw-r--r--   0 philippkitzmuller   (501) staff       (20)       58 2023-03-19 09:41:22.000000 LordPath-2023.5.6.4/README.rst
--rw-r--r--   0 philippkitzmuller   (501) staff       (20)      518 2023-05-06 13:47:11.000000 LordPath-2023.5.6.4/pyproject.toml
--rw-r--r--   0 philippkitzmuller   (501) staff       (20)       38 2023-05-06 13:47:15.489053 LordPath-2023.5.6.4/setup.cfg
+drwxr-xr-x   0 philippkitzmuller   (501) staff       (20)        0 2023-07-08 11:08:55.537481 LordPath-2023.7.8/
+drwxr-xr-x   0 philippkitzmuller   (501) staff       (20)        0 2023-07-08 11:08:55.532366 LordPath-2023.7.8/LordPath/
+-rw-r--r--   0 philippkitzmuller   (501) staff       (20)     3483 2023-05-06 13:46:10.000000 LordPath-2023.7.8/LordPath/__init__.py
+-rw-r--r--   0 philippkitzmuller   (501) staff       (20)      617 2022-12-09 23:13:08.000000 LordPath-2023.7.8/LordPath/dataset.py
+-rw-r--r--   0 philippkitzmuller   (501) staff       (20)      583 2023-03-21 08:46:08.000000 LordPath-2023.7.8/LordPath/descriptors.py
+-rw-r--r--   0 philippkitzmuller   (501) staff       (20)     6385 2023-03-17 16:32:55.000000 LordPath-2023.7.8/LordPath/filefolderclass.py
+drwxr-xr-x   0 philippkitzmuller   (501) staff       (20)        0 2023-07-08 11:08:55.536526 LordPath-2023.7.8/LordPath/opener/
+-rw-r--r--   0 philippkitzmuller   (501) staff       (20)     1282 2023-07-08 10:49:10.000000 LordPath-2023.7.8/LordPath/opener/__init__.py
+-rw-r--r--   0 philippkitzmuller   (501) staff       (20)      328 2023-03-17 16:42:56.000000 LordPath-2023.7.8/LordPath/opener/base.py
+-rw-r--r--   0 philippkitzmuller   (501) staff       (20)      868 2023-03-17 16:42:56.000000 LordPath-2023.7.8/LordPath/opener/json.py
+-rw-r--r--   0 philippkitzmuller   (501) staff       (20)      864 2023-03-17 16:42:56.000000 LordPath-2023.7.8/LordPath/opener/pickle.py
+-rw-r--r--   0 philippkitzmuller   (501) staff       (20)      490 2023-03-17 16:42:56.000000 LordPath-2023.7.8/LordPath/opener/toml.py
+-rw-r--r--   0 philippkitzmuller   (501) staff       (20)      644 2023-07-08 11:03:53.000000 LordPath-2023.7.8/LordPath/opener/xml.py
+-rw-r--r--   0 philippkitzmuller   (501) staff       (20)     1019 2023-03-16 23:58:05.000000 LordPath-2023.7.8/LordPath/opener/yaml.py
+drwxr-xr-x   0 philippkitzmuller   (501) staff       (20)        0 2023-07-08 11:08:55.533476 LordPath-2023.7.8/LordPath.egg-info/
+-rw-r--r--   0 philippkitzmuller   (501) staff       (20)      431 2023-07-08 11:08:55.000000 LordPath-2023.7.8/LordPath.egg-info/PKG-INFO
+-rw-r--r--   0 philippkitzmuller   (501) staff       (20)      450 2023-07-08 11:08:55.000000 LordPath-2023.7.8/LordPath.egg-info/SOURCES.txt
+-rw-r--r--   0 philippkitzmuller   (501) staff       (20)        1 2023-07-08 11:08:55.000000 LordPath-2023.7.8/LordPath.egg-info/dependency_links.txt
+-rw-r--r--   0 philippkitzmuller   (501) staff       (20)       23 2023-07-08 11:08:55.000000 LordPath-2023.7.8/LordPath.egg-info/requires.txt
+-rw-r--r--   0 philippkitzmuller   (501) staff       (20)        9 2023-07-08 11:08:55.000000 LordPath-2023.7.8/LordPath.egg-info/top_level.txt
+-rw-r--r--   0 philippkitzmuller   (501) staff       (20)      431 2023-07-08 11:08:55.537335 LordPath-2023.7.8/PKG-INFO
+-rw-r--r--   0 philippkitzmuller   (501) staff       (20)       58 2023-03-19 09:41:22.000000 LordPath-2023.7.8/README.rst
+-rw-r--r--   0 philippkitzmuller   (501) staff       (20)      484 2023-07-08 11:08:51.000000 LordPath-2023.7.8/pyproject.toml
+-rw-r--r--   0 philippkitzmuller   (501) staff       (20)       38 2023-07-08 11:08:55.537524 LordPath-2023.7.8/setup.cfg
```

### Comparing `LordPath-2023.5.6.4/LordPath/__init__.py` & `LordPath-2023.7.8/LordPath/__init__.py`

 * *Files identical despite different names*

### Comparing `LordPath-2023.5.6.4/LordPath/dataset.py` & `LordPath-2023.7.8/LordPath/dataset.py`

 * *Files identical despite different names*

### Comparing `LordPath-2023.5.6.4/LordPath/descriptors.py` & `LordPath-2023.7.8/LordPath/descriptors.py`

 * *Files identical despite different names*

### Comparing `LordPath-2023.5.6.4/LordPath/filefolderclass.py` & `LordPath-2023.7.8/LordPath/filefolderclass.py`

 * *Files identical despite different names*

### Comparing `LordPath-2023.5.6.4/LordPath/opener/__init__.py` & `LordPath-2023.7.8/LordPath/opener/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,34 +1,47 @@
 from os import PathLike
 from pathlib import Path
 
 
 from .base import Opener
 from .. import read_file, save_file
-from . import yaml, json, pickle, toml
+
+all_imported = False
+
+
+def import_all_types():
+    global all_imported
+    if all_imported:
+        return
+    from . import yaml, json, pickle, toml, xml
+    all_imported = True
 
 
 def get_opener(file_ending):
     file_ending = file_ending.replace('.', '')
     for cls in Opener.__subclasses__():
         if cls.check(file_ending):
             return cls
     return None
 
 
 def open_by_type(path: Path, ending=None, default=None):
+    import_all_types()
+    path = Path(path)
     if ending is None:
         ending = path.suffix
     opener_cls = get_opener(ending)
     if opener_cls is None:
         return default
     return opener_cls.load(path)
 
 
 def save_by_type(obj, path, ending=None, default=None):
+    import_all_types()
+    path = Path(path)
     if ending is None:
         ending = path.suffix
     opener_cls = get_opener(ending)
     if opener_cls is None:
         return default
     return opener_cls.save(obj, path)
```

### Comparing `LordPath-2023.5.6.4/LordPath/opener/json.py` & `LordPath-2023.7.8/LordPath/opener/json.py`

 * *Files identical despite different names*

### Comparing `LordPath-2023.5.6.4/LordPath/opener/pickle.py` & `LordPath-2023.7.8/LordPath/opener/pickle.py`

 * *Files identical despite different names*

### Comparing `LordPath-2023.5.6.4/LordPath/opener/yaml.py` & `LordPath-2023.7.8/LordPath/opener/yaml.py`

 * *Files identical despite different names*

