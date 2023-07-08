# Comparing `tmp/pygis-0.6.0.tar.gz` & `tmp/pygis-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygis-0.6.0.tar", last modified: Tue Jun 20 01:56:02 2023, max compression
+gzip compressed data, was "pygis-0.6.1.tar", last modified: Sat Jul  8 05:01:46 2023, max compression
```

## Comparing `pygis-0.6.0.tar` & `pygis-0.6.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 01:56:02.752286 pygis-0.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-20 01:55:53.000000 pygis-0.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-20 01:55:53.000000 pygis-0.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-06-20 01:56:02.752286 pygis-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-06-20 01:55:53.000000 pygis-0.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 01:56:02.752286 pygis-0.6.0/pygis/
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-20 01:55:53.000000 pygis-0.6.0/pygis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-20 01:55:53.000000 pygis-0.6.0/pygis/pygis.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 01:56:02.752286 pygis-0.6.0/pygis.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-06-20 01:56:02.000000 pygis-0.6.0/pygis.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-06-20 01:56:02.000000 pygis-0.6.0/pygis.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-06-20 01:56:02.000000 pygis-0.6.0/pygis.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 01:56:02.000000 pygis-0.6.0/pygis.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-06-20 01:56:02.000000 pygis-0.6.0/pygis.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-20 01:56:02.000000 pygis-0.6.0/pygis.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-06-20 01:55:53.000000 pygis-0.6.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-06-20 01:56:02.752286 pygis-0.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-06-20 01:55:53.000000 pygis-0.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 05:01:46.801550 pygis-0.6.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 05:01:37.000000 pygis-0.6.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-07-08 05:01:37.000000 pygis-0.6.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-07-08 05:01:46.801550 pygis-0.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-07-08 05:01:37.000000 pygis-0.6.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 05:01:46.801550 pygis-0.6.1/pygis/
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-07-08 05:01:37.000000 pygis-0.6.1/pygis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-08 05:01:37.000000 pygis-0.6.1/pygis/pygis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 05:01:46.801550 pygis-0.6.1/pygis.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-07-08 05:01:46.000000 pygis-0.6.1/pygis.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-07-08 05:01:46.000000 pygis-0.6.1/pygis.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-07-08 05:01:46.000000 pygis-0.6.1/pygis.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 05:01:46.000000 pygis-0.6.1/pygis.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-07-08 05:01:46.000000 pygis-0.6.1/pygis.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-08 05:01:46.000000 pygis-0.6.1/pygis.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-07-08 05:01:37.000000 pygis-0.6.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-07-08 05:01:46.801550 pygis-0.6.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-07-08 05:01:37.000000 pygis-0.6.1/setup.py
```

### Comparing `pygis-0.6.0/LICENSE` & `pygis-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pygis-0.6.0/PKG-INFO` & `pygis-0.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygis
-Version: 0.6.0
+Version: 0.6.1
 Summary: A Python package for installing optional dependencies for geemap and leafmap.
 Home-page: https://github.com/giswqs/pygis
 Author: Qiusheng Wu
 Author-email: giswqs@gmail.com
 License: MIT license
 Keywords: pygis
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `pygis-0.6.0/README.md` & `pygis-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `pygis-0.6.0/pygis.egg-info/PKG-INFO` & `pygis-0.6.1/pygis.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygis
-Version: 0.6.0
+Version: 0.6.1
 Summary: A Python package for installing optional dependencies for geemap and leafmap.
 Home-page: https://github.com/giswqs/pygis
 Author: Qiusheng Wu
 Author-email: giswqs@gmail.com
 License: MIT license
 Keywords: pygis
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `pygis-0.6.0/pygis.egg-info/dependency_links.txt` & `pygis-0.6.1/requirements.txt`

 * *Files 21% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 gdown
 geeadd
 geedim>=1.6.1
 geemap>=0.22.1
 geojson
 geopandas
 ipynb-py-convert
+kaleido
 leafmap>=0.21.3
 localtileserver>=0.6.1
 mapclassify>=2.4.0
 mss
 netcdf4
 osmnx
 owslib
@@ -19,18 +20,19 @@
 plotly
 pycrs
 retry
 rio-cogeo
 rioxarray
 sankee
 whiteboxgui
+pydeck
+keplergl
 # datapane
 # pydeck
 # here-map-widget-for-jupyter
-# keplergl
 # voila
 # ipython>=7.34.0
 # ipykernel>=6.15.1
 # debugpy>=1.6.2
 # lxml>=4.9.1
 # ipygany
 # ipyvtklink
```

### Comparing `pygis-0.6.0/setup.py` & `pygis-0.6.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,10 +49,10 @@
     keywords='pygis',
     name='pygis',
     packages=find_packages(include=['pygis', 'pygis.*']),
     setup_requires=setup_requirements,
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/giswqs/pygis',
-    version='0.6.0',
+    version='0.6.1',
     zip_safe=False,
 )
```

