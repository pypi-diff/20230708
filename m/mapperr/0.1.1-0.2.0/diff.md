# Comparing `tmp/mapperr-0.1.1.tar.gz` & `tmp/mapperr-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mapperr-0.1.1.tar", last modified: Mon Jun 12 04:25:22 2023, max compression
+gzip compressed data, was "mapperr-0.2.0.tar", last modified: Sat Jul  8 17:54:35 2023, max compression
```

## Comparing `mapperr-0.1.1.tar` & `mapperr-0.2.0.tar`

### file list

```diff
@@ -1,18 +1,20 @@
-drwxr-xr-x   0 mujdecisy   (501) staff       (20)        0 2023-06-12 04:25:22.093165 mapperr-0.1.1/
--rw-r--r--   0 mujdecisy   (501) staff       (20)     1076 2023-05-15 14:31:09.000000 mapperr-0.1.1/LICENSE
--rw-r--r--   0 mujdecisy   (501) staff       (20)     2684 2023-06-12 04:25:22.092992 mapperr-0.1.1/PKG-INFO
--rw-rw-r--   0 mujdecisy   (501) staff       (20)     2314 2023-05-19 20:22:50.000000 mapperr-0.1.1/README.md
-drwxr-xr-x   0 mujdecisy   (501) staff       (20)        0 2023-06-12 04:25:22.091496 mapperr-0.1.1/mapperr/
--rw-rw-r--   0 mujdecisy   (501) staff       (20)      959 2023-05-19 20:57:17.000000 mapperr-0.1.1/mapperr/__init__.py
--rw-rw-r--   0 mujdecisy   (501) staff       (20)     2364 2023-06-12 04:18:50.000000 mapperr-0.1.1/mapperr/mapr.py
-drwxr-xr-x   0 mujdecisy   (501) staff       (20)        0 2023-06-12 04:25:22.092173 mapperr-0.1.1/mapperr.egg-info/
--rw-r--r--   0 mujdecisy   (501) staff       (20)     2684 2023-06-12 04:25:22.000000 mapperr-0.1.1/mapperr.egg-info/PKG-INFO
--rw-r--r--   0 mujdecisy   (501) staff       (20)      268 2023-06-12 04:25:22.000000 mapperr-0.1.1/mapperr.egg-info/SOURCES.txt
--rw-r--r--   0 mujdecisy   (501) staff       (20)        1 2023-06-12 04:25:22.000000 mapperr-0.1.1/mapperr.egg-info/dependency_links.txt
--rw-r--r--   0 mujdecisy   (501) staff       (20)        8 2023-06-12 04:25:22.000000 mapperr-0.1.1/mapperr.egg-info/top_level.txt
--rw-r--r--   0 mujdecisy   (501) staff       (20)       38 2023-06-12 04:25:22.093213 mapperr-0.1.1/setup.cfg
--rw-rw-r--   0 mujdecisy   (501) staff       (20)      697 2023-06-12 04:23:31.000000 mapperr-0.1.1/setup.py
-drwxr-xr-x   0 mujdecisy   (501) staff       (20)        0 2023-06-12 04:25:22.092740 mapperr-0.1.1/test/
--rw-rw-r--   0 mujdecisy   (501) staff       (20)     2064 2023-06-12 04:22:42.000000 mapperr-0.1.1/test/test_nested_objects.py
--rw-rw-r--   0 mujdecisy   (501) staff       (20)      711 2023-05-19 20:18:23.000000 mapperr-0.1.1/test/test_op_required.py
--rw-rw-r--   0 mujdecisy   (501) staff       (20)      763 2023-05-15 14:38:02.000000 mapperr-0.1.1/test/test_unmatched_types.py
+drwxr-xr-x   0 mujdecisy   (501) staff       (20)        0 2023-07-08 17:54:35.926318 mapperr-0.2.0/
+-rw-r--r--   0 mujdecisy   (501) staff       (20)     1076 2023-05-15 14:31:09.000000 mapperr-0.2.0/LICENSE
+-rw-r--r--   0 mujdecisy   (501) staff       (20)     2905 2023-07-08 17:54:35.926146 mapperr-0.2.0/PKG-INFO
+-rw-rw-r--   0 mujdecisy   (501) staff       (20)     2535 2023-07-08 17:53:17.000000 mapperr-0.2.0/README.md
+drwxr-xr-x   0 mujdecisy   (501) staff       (20)        0 2023-07-08 17:54:35.924301 mapperr-0.2.0/mapperr/
+-rw-rw-r--   0 mujdecisy   (501) staff       (20)     1080 2023-07-08 17:45:59.000000 mapperr-0.2.0/mapperr/__init__.py
+-rw-r--r--   0 mujdecisy   (501) staff       (20)     3018 2023-07-08 17:45:04.000000 mapperr-0.2.0/mapperr/mapper.py
+-rw-r--r--   0 mujdecisy   (501) staff       (20)      243 2023-07-08 11:49:55.000000 mapperr-0.2.0/mapperr/util.py
+drwxr-xr-x   0 mujdecisy   (501) staff       (20)        0 2023-07-08 17:54:35.925202 mapperr-0.2.0/mapperr.egg-info/
+-rw-r--r--   0 mujdecisy   (501) staff       (20)     2905 2023-07-08 17:54:35.000000 mapperr-0.2.0/mapperr.egg-info/PKG-INFO
+-rw-r--r--   0 mujdecisy   (501) staff       (20)      317 2023-07-08 17:54:35.000000 mapperr-0.2.0/mapperr.egg-info/SOURCES.txt
+-rw-r--r--   0 mujdecisy   (501) staff       (20)        1 2023-07-08 17:54:35.000000 mapperr-0.2.0/mapperr.egg-info/dependency_links.txt
+-rw-r--r--   0 mujdecisy   (501) staff       (20)        8 2023-07-08 17:54:35.000000 mapperr-0.2.0/mapperr.egg-info/top_level.txt
+-rw-r--r--   0 mujdecisy   (501) staff       (20)       38 2023-07-08 17:54:35.926367 mapperr-0.2.0/setup.cfg
+-rw-rw-r--   0 mujdecisy   (501) staff       (20)      697 2023-07-08 17:54:24.000000 mapperr-0.2.0/setup.py
+drwxr-xr-x   0 mujdecisy   (501) staff       (20)        0 2023-07-08 17:54:35.925923 mapperr-0.2.0/test/
+-rw-rw-r--   0 mujdecisy   (501) staff       (20)     1889 2023-07-07 23:58:08.000000 mapperr-0.2.0/test/test_nested_objects.py
+-rw-rw-r--   0 mujdecisy   (501) staff       (20)      711 2023-05-19 20:18:23.000000 mapperr-0.2.0/test/test_op_required.py
+-rw-r--r--   0 mujdecisy   (501) staff       (20)      822 2023-07-08 11:47:15.000000 mapperr-0.2.0/test/test_recursive_objects.py
+-rw-rw-r--   0 mujdecisy   (501) staff       (20)      763 2023-07-01 05:54:21.000000 mapperr-0.2.0/test/test_unmatched_types.py
```

### Comparing `mapperr-0.1.1/LICENSE` & `mapperr-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mapperr-0.1.1/PKG-INFO` & `mapperr-0.2.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,7 @@
-Metadata-Version: 2.1
-Name: mapperr
-Version: 0.1.1
-Summary: mapperr for mapping across dict and object, recursively
-Home-page: https://github.com/mujdecisy/mapperr
-Author: mujdecisy
-Author-email: mujdecisy@gmail.com
-Keywords: python,mapper,recursive mapping
-Classifier: Programming Language :: Python :: 3
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # **mapperr - mapping across dictionary and class object, recursively**
 
 If you are using python for implementing protocols, cache management, nosql or sql database manupilation with  the object oriented concepts in your code, mapperr can handle your object in your way, easily.
 
 ## Installation
 `via pip`
 ```shell
@@ -96,7 +84,18 @@
 new_book._id = 5
 new_book.title = "Alchemy"
 
 lib.book_shelfs[0].books.append(new_book)
 
 send_library_to_the_source( to_dict(lib) )
 ```
+
+You can add your `recursive` type definitions into your class by using string variables.
+
+```python
+class Person:
+    name: str
+    identity: int
+    mother: 'Person'
+    father: 'Person'
+    friends: List['Person']
+```
```

### Comparing `mapperr-0.1.1/mapperr.egg-info/PKG-INFO` & `mapperr-0.2.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mapperr
-Version: 0.1.1
+Version: 0.2.0
 Summary: mapperr for mapping across dict and object, recursively
 Home-page: https://github.com/mujdecisy/mapperr
 Author: mujdecisy
 Author-email: mujdecisy@gmail.com
 Keywords: python,mapper,recursive mapping
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
@@ -96,7 +96,18 @@
 new_book._id = 5
 new_book.title = "Alchemy"
 
 lib.book_shelfs[0].books.append(new_book)
 
 send_library_to_the_source( to_dict(lib) )
 ```
+
+You can add your `recursive` type definitions into your class by using string variables.
+
+```python
+class Person:
+    name: str
+    identity: int
+    mother: 'Person'
+    father: 'Person'
+    friends: List['Person']
+```
```

### Comparing `mapperr-0.1.1/setup.py` & `mapperr-0.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 HERE = os.path.abspath(os.path.dirname(__file__))
 
 with open(os.path.join(HERE, "README.md")) as fid:
     README = fid.read()
 
 setup(
     name="mapperr",
-    version="0.1.1",
+    version="0.2.0",
     description="mapperr for mapping across dict and object, recursively",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/mujdecisy/mapperr",
     keywords=["python", "mapper", "recursive mapping"],
     author="mujdecisy",
     author_email="mujdecisy@gmail.com",
```

### Comparing `mapperr-0.1.1/test/test_op_required.py` & `mapperr-0.2.0/test/test_op_required.py`

 * *Files identical despite different names*

### Comparing `mapperr-0.1.1/test/test_unmatched_types.py` & `mapperr-0.2.0/test/test_unmatched_types.py`

 * *Files identical despite different names*

