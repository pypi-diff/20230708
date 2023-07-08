# Comparing `tmp/sphractal-0.8.0.tar.gz` & `tmp/sphractal-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sphractal-0.8.0.tar", max compression
+gzip compressed data, was "sphractal-0.8.1.tar", max compression
```

## Comparing `sphractal-0.8.0.tar` & `sphractal-0.8.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1082 2023-07-07 09:11:28.347972 sphractal-0.8.0/LICENSE
--rw-r--r--   0        0        0     4017 2023-07-07 09:11:28.347972 sphractal-0.8.0/README.md
--rw-r--r--   0        0        0     2056 2023-07-07 09:12:06.575822 sphractal-0.8.0/pyproject.toml
--rw-r--r--   0        0        0      736 2023-07-07 09:12:06.575822 sphractal-0.8.0/setup.py
--rw-r--r--   0        0        0     1429 2023-07-07 09:11:28.411972 sphractal-0.8.0/src/sphractal/__init__.py
--rw-r--r--   0        0        0    23050 2023-07-07 09:11:28.411972 sphractal-0.8.0/src/sphractal/boxCnt.py
--rw-r--r--   0        0        0     4382 2023-07-07 09:11:28.415972 sphractal-0.8.0/src/sphractal/constants.py
--rw-r--r--   0        0        0        0 2023-07-07 09:11:28.415972 sphractal-0.8.0/src/sphractal/data/__init__.py
--rw-r--r--   0        0        0    20105 2023-07-07 09:11:28.415972 sphractal-0.8.0/src/sphractal/data/example.xyz
--rw-r--r--   0        0        0      264 2023-07-07 09:11:28.415972 sphractal-0.8.0/src/sphractal/datasets.py
--rw-r--r--   0        0        0     8750 2023-07-07 09:11:28.415972 sphractal-0.8.0/src/sphractal/surfExact.py
--rw-r--r--   0        0        0     8121 2023-07-07 09:11:28.415972 sphractal-0.8.0/src/sphractal/surfPointClouds.py
--rw-r--r--   0        0        0    11515 2023-07-07 09:11:28.415972 sphractal-0.8.0/src/sphractal/utils.py
--rw-r--r--   0        0        0    94032 2023-07-07 09:11:28.415972 sphractal-0.8.0/tests/fixtures.py
--rw-r--r--   0        0        0    17618 2023-07-07 09:11:28.415972 sphractal-0.8.0/tests/test_sphractal.py
--rw-r--r--   0        0        0     5286 1970-01-01 00:00:00.000000 sphractal-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1082 2023-07-08 10:21:27.636502 sphractal-0.8.1/LICENSE
+-rw-r--r--   0        0        0     4017 2023-07-08 10:21:27.636502 sphractal-0.8.1/README.md
+-rw-r--r--   0        0        0     2056 2023-07-08 10:22:11.617038 sphractal-0.8.1/pyproject.toml
+-rw-r--r--   0        0        0      736 2023-07-08 10:22:11.617038 sphractal-0.8.1/setup.py
+-rw-r--r--   0        0        0     1429 2023-07-08 10:21:27.692502 sphractal-0.8.1/src/sphractal/__init__.py
+-rw-r--r--   0        0        0    23050 2023-07-08 10:21:27.696502 sphractal-0.8.1/src/sphractal/boxCnt.py
+-rw-r--r--   0        0        0     4382 2023-07-08 10:21:27.696502 sphractal-0.8.1/src/sphractal/constants.py
+-rw-r--r--   0        0        0        0 2023-07-08 10:21:27.696502 sphractal-0.8.1/src/sphractal/data/__init__.py
+-rw-r--r--   0        0        0    20105 2023-07-08 10:21:27.696502 sphractal-0.8.1/src/sphractal/data/example.xyz
+-rw-r--r--   0        0        0      264 2023-07-08 10:21:27.696502 sphractal-0.8.1/src/sphractal/datasets.py
+-rw-r--r--   0        0        0     8750 2023-07-08 10:21:27.696502 sphractal-0.8.1/src/sphractal/surfExact.py
+-rw-r--r--   0        0        0     8121 2023-07-08 10:21:27.696502 sphractal-0.8.1/src/sphractal/surfPointClouds.py
+-rw-r--r--   0        0        0    11515 2023-07-08 10:21:27.696502 sphractal-0.8.1/src/sphractal/utils.py
+-rw-r--r--   0        0        0    94032 2023-07-08 10:21:27.696502 sphractal-0.8.1/tests/fixtures.py
+-rw-r--r--   0        0        0    17618 2023-07-08 10:21:27.696502 sphractal-0.8.1/tests/test_sphractal.py
+-rw-r--r--   0        0        0     5286 1970-01-01 00:00:00.000000 sphractal-0.8.1/PKG-INFO
```

### Comparing `sphractal-0.8.0/LICENSE` & `sphractal-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sphractal-0.8.0/README.md` & `sphractal-0.8.1/README.md`

 * *Files identical despite different names*

### Comparing `sphractal-0.8.0/pyproject.toml` & `sphractal-0.8.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sphractal"
-version = "0.8.0"
+version = "0.8.1"
 description = "Package to estimate fractal dimension of 3D surfaces formed from overlapping spheres via box-counting algorithm."
 authors = ["Jonathan Yik Chang Ting <jonting97@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/Jon-Ting/sphractal"
 repository = "https://github.com/Jon-Ting/sphractal"
 documentation = "https://sphractal.readthedocs.io/en/latest/"
```

### Comparing `sphractal-0.8.0/setup.py` & `sphractal-0.8.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import setuptools
 
 
-__version__ = '0.8.0'
+__version__ = '0.8.1'
 with open('README.md', 'r') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="sphractal",
     version=__version__,
     author="Jonathan Yik Chang Ting",
```

### Comparing `sphractal-0.8.0/src/sphractal/__init__.py` & `sphractal-0.8.1/src/sphractal/__init__.py`

 * *Files identical despite different names*

### Comparing `sphractal-0.8.0/src/sphractal/boxCnt.py` & `sphractal-0.8.1/src/sphractal/boxCnt.py`

 * *Files identical despite different names*

### Comparing `sphractal-0.8.0/src/sphractal/constants.py` & `sphractal-0.8.1/src/sphractal/constants.py`

 * *Files identical despite different names*

### Comparing `sphractal-0.8.0/src/sphractal/data/example.xyz` & `sphractal-0.8.1/src/sphractal/data/example.xyz`

 * *Files identical despite different names*

### Comparing `sphractal-0.8.0/src/sphractal/surfExact.py` & `sphractal-0.8.1/src/sphractal/surfExact.py`

 * *Files identical despite different names*

### Comparing `sphractal-0.8.0/src/sphractal/surfPointClouds.py` & `sphractal-0.8.1/src/sphractal/surfPointClouds.py`

 * *Files identical despite different names*

### Comparing `sphractal-0.8.0/src/sphractal/utils.py` & `sphractal-0.8.1/src/sphractal/utils.py`

 * *Files identical despite different names*

### Comparing `sphractal-0.8.0/tests/fixtures.py` & `sphractal-0.8.1/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `sphractal-0.8.0/tests/test_sphractal.py` & `sphractal-0.8.1/tests/test_sphractal.py`

 * *Files identical despite different names*

### Comparing `sphractal-0.8.0/PKG-INFO` & `sphractal-0.8.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphractal
-Version: 0.8.0
+Version: 0.8.1
 Summary: Package to estimate fractal dimension of 3D surfaces formed from overlapping spheres via box-counting algorithm.
 Home-page: https://github.com/Jon-Ting/sphractal
 License: MIT
 Keywords: box-counting,box-count,fractal,dimension,sphere,surface
 Author: Jonathan Yik Chang Ting
 Author-email: jonting97@gmail.com
 Requires-Python: >=3.9
```

