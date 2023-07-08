# Comparing `tmp/mapperr-0.2.1.tar.gz` & `tmp/mapperr-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mapperr-0.2.1.tar", last modified: Sat Jul  8 18:32:20 2023, max compression
+gzip compressed data, was "mapperr-0.2.2.tar", last modified: Sat Jul  8 19:32:20 2023, max compression
```

## Comparing `mapperr-0.2.1.tar` & `mapperr-0.2.2.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 mujdecisy   (501) staff       (20)        0 2023-07-08 18:32:20.846466 mapperr-0.2.1/
--rw-r--r--   0 mujdecisy   (501) staff       (20)     1076 2023-05-15 14:31:09.000000 mapperr-0.2.1/LICENSE
--rw-r--r--   0 mujdecisy   (501) staff       (20)     2905 2023-07-08 18:32:20.846286 mapperr-0.2.1/PKG-INFO
--rw-rw-r--   0 mujdecisy   (501) staff       (20)     2535 2023-07-08 17:53:17.000000 mapperr-0.2.1/README.md
-drwxr-xr-x   0 mujdecisy   (501) staff       (20)        0 2023-07-08 18:32:20.844120 mapperr-0.2.1/mapperr/
--rw-rw-r--   0 mujdecisy   (501) staff       (20)     1080 2023-07-08 17:45:59.000000 mapperr-0.2.1/mapperr/__init__.py
--rw-r--r--   0 mujdecisy   (501) staff       (20)     3280 2023-07-08 18:26:33.000000 mapperr-0.2.1/mapperr/mapper.py
--rw-r--r--   0 mujdecisy   (501) staff       (20)      243 2023-07-08 11:49:55.000000 mapperr-0.2.1/mapperr/util.py
-drwxr-xr-x   0 mujdecisy   (501) staff       (20)        0 2023-07-08 18:32:20.844853 mapperr-0.2.1/mapperr.egg-info/
--rw-r--r--   0 mujdecisy   (501) staff       (20)     2905 2023-07-08 18:32:20.000000 mapperr-0.2.1/mapperr.egg-info/PKG-INFO
--rw-r--r--   0 mujdecisy   (501) staff       (20)      346 2023-07-08 18:32:20.000000 mapperr-0.2.1/mapperr.egg-info/SOURCES.txt
--rw-r--r--   0 mujdecisy   (501) staff       (20)        1 2023-07-08 18:32:20.000000 mapperr-0.2.1/mapperr.egg-info/dependency_links.txt
--rw-r--r--   0 mujdecisy   (501) staff       (20)        8 2023-07-08 18:32:20.000000 mapperr-0.2.1/mapperr.egg-info/top_level.txt
--rw-r--r--   0 mujdecisy   (501) staff       (20)       38 2023-07-08 18:32:20.846512 mapperr-0.2.1/setup.cfg
--rw-rw-r--   0 mujdecisy   (501) staff       (20)      697 2023-07-08 18:32:16.000000 mapperr-0.2.1/setup.py
-drwxr-xr-x   0 mujdecisy   (501) staff       (20)        0 2023-07-08 18:32:20.846042 mapperr-0.2.1/test/
--rw-rw-r--   0 mujdecisy   (501) staff       (20)      624 2023-07-08 18:30:43.000000 mapperr-0.2.1/test/test_dict_attributes.py
--rw-rw-r--   0 mujdecisy   (501) staff       (20)     1889 2023-07-07 23:58:08.000000 mapperr-0.2.1/test/test_nested_objects.py
--rw-rw-r--   0 mujdecisy   (501) staff       (20)      711 2023-05-19 20:18:23.000000 mapperr-0.2.1/test/test_op_required.py
--rw-r--r--   0 mujdecisy   (501) staff       (20)      822 2023-07-08 18:28:47.000000 mapperr-0.2.1/test/test_recursive_objects.py
--rw-rw-r--   0 mujdecisy   (501) staff       (20)      763 2023-07-01 05:54:21.000000 mapperr-0.2.1/test/test_unmatched_types.py
+drwxr-xr-x   0 mujdecisy   (501) staff       (20)        0 2023-07-08 19:32:20.989349 mapperr-0.2.2/
+-rw-r--r--   0 mujdecisy   (501) staff       (20)     1076 2023-05-15 14:31:09.000000 mapperr-0.2.2/LICENSE
+-rw-r--r--   0 mujdecisy   (501) staff       (20)     2905 2023-07-08 19:32:20.989139 mapperr-0.2.2/PKG-INFO
+-rw-rw-r--   0 mujdecisy   (501) staff       (20)     2535 2023-07-08 17:53:17.000000 mapperr-0.2.2/README.md
+drwxr-xr-x   0 mujdecisy   (501) staff       (20)        0 2023-07-08 19:32:20.986659 mapperr-0.2.2/mapperr/
+-rw-rw-r--   0 mujdecisy   (501) staff       (20)     1080 2023-07-08 17:45:59.000000 mapperr-0.2.2/mapperr/__init__.py
+-rw-r--r--   0 mujdecisy   (501) staff       (20)     3702 2023-07-08 19:24:53.000000 mapperr-0.2.2/mapperr/mapper.py
+-rw-r--r--   0 mujdecisy   (501) staff       (20)      243 2023-07-08 11:49:55.000000 mapperr-0.2.2/mapperr/util.py
+drwxr-xr-x   0 mujdecisy   (501) staff       (20)        0 2023-07-08 19:32:20.987374 mapperr-0.2.2/mapperr.egg-info/
+-rw-r--r--   0 mujdecisy   (501) staff       (20)     2905 2023-07-08 19:32:20.000000 mapperr-0.2.2/mapperr.egg-info/PKG-INFO
+-rw-r--r--   0 mujdecisy   (501) staff       (20)      373 2023-07-08 19:32:20.000000 mapperr-0.2.2/mapperr.egg-info/SOURCES.txt
+-rw-r--r--   0 mujdecisy   (501) staff       (20)        1 2023-07-08 19:32:20.000000 mapperr-0.2.2/mapperr.egg-info/dependency_links.txt
+-rw-r--r--   0 mujdecisy   (501) staff       (20)        8 2023-07-08 19:32:20.000000 mapperr-0.2.2/mapperr.egg-info/top_level.txt
+-rw-r--r--   0 mujdecisy   (501) staff       (20)       38 2023-07-08 19:32:20.989401 mapperr-0.2.2/setup.cfg
+-rw-rw-r--   0 mujdecisy   (501) staff       (20)      697 2023-07-08 19:31:47.000000 mapperr-0.2.2/setup.py
+drwxr-xr-x   0 mujdecisy   (501) staff       (20)        0 2023-07-08 19:32:20.988712 mapperr-0.2.2/test/
+-rw-rw-r--   0 mujdecisy   (501) staff       (20)      624 2023-07-08 19:25:31.000000 mapperr-0.2.2/test/test_dict_attributes.py
+-rw-rw-r--   0 mujdecisy   (501) staff       (20)     1889 2023-07-07 23:58:08.000000 mapperr-0.2.2/test/test_nested_objects.py
+-rw-rw-r--   0 mujdecisy   (501) staff       (20)      711 2023-05-19 20:18:23.000000 mapperr-0.2.2/test/test_op_required.py
+-rw-r--r--   0 mujdecisy   (501) staff       (20)      822 2023-07-08 18:28:47.000000 mapperr-0.2.2/test/test_recursive_objects.py
+-rw-rw-r--   0 mujdecisy   (501) staff       (20)      923 2023-07-08 19:31:11.000000 mapperr-0.2.2/test/test_super_classes.py
+-rw-rw-r--   0 mujdecisy   (501) staff       (20)      763 2023-07-01 05:54:21.000000 mapperr-0.2.2/test/test_unmatched_types.py
```

### Comparing `mapperr-0.2.1/LICENSE` & `mapperr-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mapperr-0.2.1/PKG-INFO` & `mapperr-0.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mapperr
-Version: 0.2.1
+Version: 0.2.2
 Summary: mapperr for mapping across dict and object, recursively
 Home-page: https://github.com/mujdecisy/mapperr
 Author: mujdecisy
 Author-email: mujdecisy@gmail.com
 Keywords: python,mapper,recursive mapping
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
```

### Comparing `mapperr-0.2.1/README.md` & `mapperr-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `mapperr-0.2.1/mapperr/__init__.py` & `mapperr-0.2.2/mapperr/__init__.py`

 * *Files identical despite different names*

### Comparing `mapperr-0.2.1/mapperr/mapper.py` & `mapperr-0.2.2/mapperr/mapper.py`

 * *Files 5% similar despite different names*

```diff
@@ -33,14 +33,26 @@
             if local_classs_definition is None:
                 warnings.warn(f"Class {class_definition} not found")
                 local_classs_definition = object
         elif class_definition.__module__ not in ["typing", "builtins"]:
             self.__all_classes.add(class_definition)
         return local_classs_definition
 
+    def __get_all_annotations(self, class_definition: type) -> dict:
+        classes = [class_definition]
+        while classes[0].__name__ != 'object':
+            classes.insert(0, classes[0].__base__)
+        del classes[0]
+
+        annotations = {}
+        for a_class in classes:
+            annotations.update(a_class.__annotations__)
+
+        return annotations
+
     def map(self, src: Union[dict, object, None], blueprint: type):
         self.__add_class(blueprint)
         mapped_item = None
         if src is None:
             mapped_item = None
         elif blueprint.__module__ == "builtins":
             if blueprint.__name__ not in NOT_ALLOWED_BUILTINS and isinstance(
@@ -66,12 +78,15 @@
                 )
         else:
             mapped_item = (
                 blueprint()
                 if self.__direction == MappingDirection.DICT_TO_OBJECT
                 else {}
             )
-            for key, type_ in blueprint.__annotations__.items():
+
+            annotations = self.__get_all_annotations(blueprint)
+
+            for key, type_ in annotations.items():
                 value = self.__read(src, key)
                 class_def = self.__add_class(type_)
                 self.__write(mapped_item, key, self.map(value, class_def))
         return mapped_item
```

### Comparing `mapperr-0.2.1/mapperr.egg-info/PKG-INFO` & `mapperr-0.2.2/mapperr.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mapperr
-Version: 0.2.1
+Version: 0.2.2
 Summary: mapperr for mapping across dict and object, recursively
 Home-page: https://github.com/mujdecisy/mapperr
 Author: mujdecisy
 Author-email: mujdecisy@gmail.com
 Keywords: python,mapper,recursive mapping
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
```

### Comparing `mapperr-0.2.1/setup.py` & `mapperr-0.2.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 HERE = os.path.abspath(os.path.dirname(__file__))
 
 with open(os.path.join(HERE, "README.md")) as fid:
     README = fid.read()
 
 setup(
     name="mapperr",
-    version="0.2.1",
+    version="0.2.2",
     description="mapperr for mapping across dict and object, recursively",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/mujdecisy/mapperr",
     keywords=["python", "mapper", "recursive mapping"],
     author="mujdecisy",
     author_email="mujdecisy@gmail.com",
```

### Comparing `mapperr-0.2.1/test/test_dict_attributes.py` & `mapperr-0.2.2/test/test_dict_attributes.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from unittest import TestCase
 from mapperr import to_dict, to_obj
 from typing import Dict
 
 class A:
     a1: Dict[str, int]
 
-class TestUnmatchedTypes(TestCase):
+class TestDictAttributes(TestCase):
     def setUp(self) -> None:
         self.a = A()
         self.a.a1 = {"apple": 5, "banana": 6}
         self.ad = {"a1": {"apple": 5, "banana": 6}}
 
     def test__to_dict__when_dictAttrExist(self):
         actual = to_dict(self.a)
```

### Comparing `mapperr-0.2.1/test/test_nested_objects.py` & `mapperr-0.2.2/test/test_nested_objects.py`

 * *Files identical despite different names*

### Comparing `mapperr-0.2.1/test/test_op_required.py` & `mapperr-0.2.2/test/test_op_required.py`

 * *Files identical despite different names*

### Comparing `mapperr-0.2.1/test/test_recursive_objects.py` & `mapperr-0.2.2/test/test_recursive_objects.py`

 * *Files identical despite different names*

### Comparing `mapperr-0.2.1/test/test_unmatched_types.py` & `mapperr-0.2.2/test/test_unmatched_types.py`

 * *Files identical despite different names*

