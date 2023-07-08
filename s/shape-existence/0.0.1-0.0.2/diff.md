# Comparing `tmp/shape_existence-0.0.1.tar.gz` & `tmp/shape_existence-0.0.2.tar.gz`

## Comparing `shape_existence-0.0.1.tar` & `shape_existence-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,12 @@
--rw-r--r--   0        0        0     8196 2020-02-02 00:00:00.000000 shape_existence-0.0.1/.DS_Store
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 shape_existence-0.0.1/.gitattributes
--rw-r--r--   0        0        0    13605 2020-02-02 00:00:00.000000 shape_existence-0.0.1/obj_files/345_triangle.obj
--rw-r--r--   0        0        0   132217 2020-02-02 00:00:00.000000 shape_existence-0.0.1/obj_files/icosahedron.obj
--rw-r--r--   0        0        0    53429 2020-02-02 00:00:00.000000 shape_existence-0.0.1/obj_files/octahedron.obj
--rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 shape_existence-0.0.1/obj_files/shape_existence.mtl
--rw-r--r--   0        0        0    26231 2020-02-02 00:00:00.000000 shape_existence-0.0.1/obj_files/tetrahedron.obj
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 shape_existence-0.0.1/src/__init__.py
--rw-r--r--   0        0        0    13379 2020-02-02 00:00:00.000000 shape_existence-0.0.1/src/flexible_cqp.py
--rw-r--r--   0        0        0    16698 2020-02-02 00:00:00.000000 shape_existence-0.0.1/src/fractions_and_interval_arithmetic.py
--rw-r--r--   0        0        0     4928 2020-02-02 00:00:00.000000 shape_existence-0.0.1/src/obj_stuff.py
--rw-r--r--   0        0        0    21252 2020-02-02 00:00:00.000000 shape_existence-0.0.1/src/shape_existence.py
--rw-r--r--   0        0        0     1058 2020-02-02 00:00:00.000000 shape_existence-0.0.1/LICENSE
--rw-r--r--   0        0        0     3126 2020-02-02 00:00:00.000000 shape_existence-0.0.1/README.md
--rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 shape_existence-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     3752 2020-02-02 00:00:00.000000 shape_existence-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 shape_existence-0.0.2/.DS_Store
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 shape_existence-0.0.2/.gitattributes
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 shape_existence-0.0.2/src/.DS_Store
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 shape_existence-0.0.2/src/shape_existence/__init__.py
+-rw-r--r--   0        0        0    21252 2020-02-02 00:00:00.000000 shape_existence-0.0.2/src/shape_existence/complexes_and_proofs.py
+-rw-r--r--   0        0        0    13379 2020-02-02 00:00:00.000000 shape_existence-0.0.2/src/shape_existence/flexible_cqp.py
+-rw-r--r--   0        0        0    16698 2020-02-02 00:00:00.000000 shape_existence-0.0.2/src/shape_existence/fractions_and_interval_arithmetic.py
+-rw-r--r--   0        0        0     4928 2020-02-02 00:00:00.000000 shape_existence-0.0.2/src/shape_existence/obj_stuff.py
+-rw-r--r--   0        0        0     1058 2020-02-02 00:00:00.000000 shape_existence-0.0.2/LICENSE
+-rw-r--r--   0        0        0     3126 2020-02-02 00:00:00.000000 shape_existence-0.0.2/README.md
+-rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 shape_existence-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     3752 2020-02-02 00:00:00.000000 shape_existence-0.0.2/PKG-INFO
```

### Comparing `shape_existence-0.0.1/src/flexible_cqp.py` & `shape_existence-0.0.2/src/shape_existence/flexible_cqp.py`

 * *Files identical despite different names*

### Comparing `shape_existence-0.0.1/src/fractions_and_interval_arithmetic.py` & `shape_existence-0.0.2/src/shape_existence/fractions_and_interval_arithmetic.py`

 * *Files identical despite different names*

### Comparing `shape_existence-0.0.1/src/obj_stuff.py` & `shape_existence-0.0.2/src/shape_existence/obj_stuff.py`

 * *Files identical despite different names*

### Comparing `shape_existence-0.0.1/src/shape_existence.py` & `shape_existence-0.0.2/src/shape_existence/complexes_and_proofs.py`

 * *Files identical despite different names*

### Comparing `shape_existence-0.0.1/LICENSE` & `shape_existence-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `shape_existence-0.0.1/README.md` & `shape_existence-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `shape_existence-0.0.1/pyproject.toml` & `shape_existence-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "shape_existence"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Matthew Ellison", email="matthew.v.ellison@gmail.com" },
 ]
 description = "A package to prove the existence of non-intersecting realizations of abstract simplicial complexes with specified edge lengths."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/mve17/shape_existence"
-"Bug Tracker" = "https://github.com/mve17/shape_existence/issues"
+"Bug Tracker" = "https://github.com/mve17/shape_existence/issues"
```

### Comparing `shape_existence-0.0.1/PKG-INFO` & `shape_existence-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shape_existence
-Version: 0.0.1
+Version: 0.0.2
 Summary: A package to prove the existence of non-intersecting realizations of abstract simplicial complexes with specified edge lengths.
 Project-URL: Homepage, https://github.com/mve17/shape_existence
 Project-URL: Bug Tracker, https://github.com/mve17/shape_existence/issues
 Author-email: Matthew Ellison <matthew.v.ellison@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

