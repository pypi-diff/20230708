# Comparing `tmp/mapperr-0.2.0.tar.gz` & `tmp/mapperr-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mapperr-0.2.0.tar", last modified: Sat Jul  8 17:54:35 2023, max compression
+gzip compressed data, was "mapperr-0.2.1.tar", last modified: Sat Jul  8 18:32:20 2023, max compression
```

## Comparing `mapperr-0.2.0.tar` & `mapperr-0.2.1.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 mujdecisy   (501) staff       (20)        0 2023-07-08 17:54:35.926318 mapperr-0.2.0/
--rw-r--r--   0 mujdecisy   (501) staff       (20)     1076 2023-05-15 14:31:09.000000 mapperr-0.2.0/LICENSE
--rw-r--r--   0 mujdecisy   (501) staff       (20)     2905 2023-07-08 17:54:35.926146 mapperr-0.2.0/PKG-INFO
--rw-rw-r--   0 mujdecisy   (501) staff       (20)     2535 2023-07-08 17:53:17.000000 mapperr-0.2.0/README.md
-drwxr-xr-x   0 mujdecisy   (501) staff       (20)        0 2023-07-08 17:54:35.924301 mapperr-0.2.0/mapperr/
--rw-rw-r--   0 mujdecisy   (501) staff       (20)     1080 2023-07-08 17:45:59.000000 mapperr-0.2.0/mapperr/__init__.py
--rw-r--r--   0 mujdecisy   (501) staff       (20)     3018 2023-07-08 17:45:04.000000 mapperr-0.2.0/mapperr/mapper.py
--rw-r--r--   0 mujdecisy   (501) staff       (20)      243 2023-07-08 11:49:55.000000 mapperr-0.2.0/mapperr/util.py
-drwxr-xr-x   0 mujdecisy   (501) staff       (20)        0 2023-07-08 17:54:35.925202 mapperr-0.2.0/mapperr.egg-info/
--rw-r--r--   0 mujdecisy   (501) staff       (20)     2905 2023-07-08 17:54:35.000000 mapperr-0.2.0/mapperr.egg-info/PKG-INFO
--rw-r--r--   0 mujdecisy   (501) staff       (20)      317 2023-07-08 17:54:35.000000 mapperr-0.2.0/mapperr.egg-info/SOURCES.txt
--rw-r--r--   0 mujdecisy   (501) staff       (20)        1 2023-07-08 17:54:35.000000 mapperr-0.2.0/mapperr.egg-info/dependency_links.txt
--rw-r--r--   0 mujdecisy   (501) staff       (20)        8 2023-07-08 17:54:35.000000 mapperr-0.2.0/mapperr.egg-info/top_level.txt
--rw-r--r--   0 mujdecisy   (501) staff       (20)       38 2023-07-08 17:54:35.926367 mapperr-0.2.0/setup.cfg
--rw-rw-r--   0 mujdecisy   (501) staff       (20)      697 2023-07-08 17:54:24.000000 mapperr-0.2.0/setup.py
-drwxr-xr-x   0 mujdecisy   (501) staff       (20)        0 2023-07-08 17:54:35.925923 mapperr-0.2.0/test/
--rw-rw-r--   0 mujdecisy   (501) staff       (20)     1889 2023-07-07 23:58:08.000000 mapperr-0.2.0/test/test_nested_objects.py
--rw-rw-r--   0 mujdecisy   (501) staff       (20)      711 2023-05-19 20:18:23.000000 mapperr-0.2.0/test/test_op_required.py
--rw-r--r--   0 mujdecisy   (501) staff       (20)      822 2023-07-08 11:47:15.000000 mapperr-0.2.0/test/test_recursive_objects.py
--rw-rw-r--   0 mujdecisy   (501) staff       (20)      763 2023-07-01 05:54:21.000000 mapperr-0.2.0/test/test_unmatched_types.py
+drwxr-xr-x   0 mujdecisy   (501) staff       (20)        0 2023-07-08 18:32:20.846466 mapperr-0.2.1/
+-rw-r--r--   0 mujdecisy   (501) staff       (20)     1076 2023-05-15 14:31:09.000000 mapperr-0.2.1/LICENSE
+-rw-r--r--   0 mujdecisy   (501) staff       (20)     2905 2023-07-08 18:32:20.846286 mapperr-0.2.1/PKG-INFO
+-rw-rw-r--   0 mujdecisy   (501) staff       (20)     2535 2023-07-08 17:53:17.000000 mapperr-0.2.1/README.md
+drwxr-xr-x   0 mujdecisy   (501) staff       (20)        0 2023-07-08 18:32:20.844120 mapperr-0.2.1/mapperr/
+-rw-rw-r--   0 mujdecisy   (501) staff       (20)     1080 2023-07-08 17:45:59.000000 mapperr-0.2.1/mapperr/__init__.py
+-rw-r--r--   0 mujdecisy   (501) staff       (20)     3280 2023-07-08 18:26:33.000000 mapperr-0.2.1/mapperr/mapper.py
+-rw-r--r--   0 mujdecisy   (501) staff       (20)      243 2023-07-08 11:49:55.000000 mapperr-0.2.1/mapperr/util.py
+drwxr-xr-x   0 mujdecisy   (501) staff       (20)        0 2023-07-08 18:32:20.844853 mapperr-0.2.1/mapperr.egg-info/
+-rw-r--r--   0 mujdecisy   (501) staff       (20)     2905 2023-07-08 18:32:20.000000 mapperr-0.2.1/mapperr.egg-info/PKG-INFO
+-rw-r--r--   0 mujdecisy   (501) staff       (20)      346 2023-07-08 18:32:20.000000 mapperr-0.2.1/mapperr.egg-info/SOURCES.txt
+-rw-r--r--   0 mujdecisy   (501) staff       (20)        1 2023-07-08 18:32:20.000000 mapperr-0.2.1/mapperr.egg-info/dependency_links.txt
+-rw-r--r--   0 mujdecisy   (501) staff       (20)        8 2023-07-08 18:32:20.000000 mapperr-0.2.1/mapperr.egg-info/top_level.txt
+-rw-r--r--   0 mujdecisy   (501) staff       (20)       38 2023-07-08 18:32:20.846512 mapperr-0.2.1/setup.cfg
+-rw-rw-r--   0 mujdecisy   (501) staff       (20)      697 2023-07-08 18:32:16.000000 mapperr-0.2.1/setup.py
+drwxr-xr-x   0 mujdecisy   (501) staff       (20)        0 2023-07-08 18:32:20.846042 mapperr-0.2.1/test/
+-rw-rw-r--   0 mujdecisy   (501) staff       (20)      624 2023-07-08 18:30:43.000000 mapperr-0.2.1/test/test_dict_attributes.py
+-rw-rw-r--   0 mujdecisy   (501) staff       (20)     1889 2023-07-07 23:58:08.000000 mapperr-0.2.1/test/test_nested_objects.py
+-rw-rw-r--   0 mujdecisy   (501) staff       (20)      711 2023-05-19 20:18:23.000000 mapperr-0.2.1/test/test_op_required.py
+-rw-r--r--   0 mujdecisy   (501) staff       (20)      822 2023-07-08 18:28:47.000000 mapperr-0.2.1/test/test_recursive_objects.py
+-rw-rw-r--   0 mujdecisy   (501) staff       (20)      763 2023-07-01 05:54:21.000000 mapperr-0.2.1/test/test_unmatched_types.py
```

### Comparing `mapperr-0.2.0/LICENSE` & `mapperr-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mapperr-0.2.0/PKG-INFO` & `mapperr-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mapperr
-Version: 0.2.0
+Version: 0.2.1
 Summary: mapperr for mapping across dict and object, recursively
 Home-page: https://github.com/mujdecisy/mapperr
 Author: mujdecisy
 Author-email: mujdecisy@gmail.com
 Keywords: python,mapper,recursive mapping
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
```

### Comparing `mapperr-0.2.0/README.md` & `mapperr-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `mapperr-0.2.0/mapperr/__init__.py` & `mapperr-0.2.1/mapperr/__init__.py`

 * *Files identical despite different names*

### Comparing `mapperr-0.2.0/mapperr/mapper.py` & `mapperr-0.2.1/mapperr/mapper.py`

 * *Files 7% similar despite different names*

```diff
@@ -52,14 +52,18 @@
                     f"Type {blueprint.__name__} not allowed OR value {type(src).__name__} not matched with type"
                 )
         elif blueprint.__module__ == "typing":
             if blueprint.__name__ == "List" and isinstance(src, list):
                 mapped_item = []
                 for list_element in src:
                     mapped_item.append(self.map(list_element, blueprint.__args__[0]))
+            if blueprint.__name__ == "Dict" and isinstance(src, dict):
+                mapped_item = {}
+                for key, value in src.items():
+                    mapped_item[self.map(key, blueprint.__args__[0])] = self.map(value, blueprint.__args__[1])
             else:
                 warnings.warn(
                     f"Type {blueprint.__name__} not allowed OR value {type(src).__name__} not matched with type"
                 )
         else:
             mapped_item = (
                 blueprint()
```

### Comparing `mapperr-0.2.0/mapperr.egg-info/PKG-INFO` & `mapperr-0.2.1/mapperr.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mapperr
-Version: 0.2.0
+Version: 0.2.1
 Summary: mapperr for mapping across dict and object, recursively
 Home-page: https://github.com/mujdecisy/mapperr
 Author: mujdecisy
 Author-email: mujdecisy@gmail.com
 Keywords: python,mapper,recursive mapping
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
```

### Comparing `mapperr-0.2.0/setup.py` & `mapperr-0.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 HERE = os.path.abspath(os.path.dirname(__file__))
 
 with open(os.path.join(HERE, "README.md")) as fid:
     README = fid.read()
 
 setup(
     name="mapperr",
-    version="0.2.0",
+    version="0.2.1",
     description="mapperr for mapping across dict and object, recursively",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/mujdecisy/mapperr",
     keywords=["python", "mapper", "recursive mapping"],
     author="mujdecisy",
     author_email="mujdecisy@gmail.com",
```

### Comparing `mapperr-0.2.0/test/test_nested_objects.py` & `mapperr-0.2.1/test/test_nested_objects.py`

 * *Files identical despite different names*

### Comparing `mapperr-0.2.0/test/test_op_required.py` & `mapperr-0.2.1/test/test_op_required.py`

 * *Files identical despite different names*

### Comparing `mapperr-0.2.0/test/test_recursive_objects.py` & `mapperr-0.2.1/test/test_recursive_objects.py`

 * *Files identical despite different names*

### Comparing `mapperr-0.2.0/test/test_unmatched_types.py` & `mapperr-0.2.1/test/test_unmatched_types.py`

 * *Files identical despite different names*

