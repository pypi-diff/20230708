# Comparing `tmp/seismicpy-0.0.1.4.tar.gz` & `tmp/seismicpy-0.0.1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seismicpy-0.0.1.4.tar", last modified: Sat Jul  8 02:00:14 2023, max compression
+gzip compressed data, was "seismicpy-0.0.1.4.1.tar", last modified: Sat Jul  8 02:08:45 2023, max compression
```

## Comparing `seismicpy-0.0.1.4.tar` & `seismicpy-0.0.1.4.1.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 chenyk     (501) staff       (20)        0 2023-07-08 02:00:14.095164 seismicpy-0.0.1.4/
--rw-r--r--   0 chenyk     (501) staff       (20)     1115 2023-07-08 02:00:14.094682 seismicpy-0.0.1.4/PKG-INFO
--rw-r--r--   0 chenyk     (501) staff       (20)     3280 2023-07-08 01:43:38.000000 seismicpy-0.0.1.4/README.md
-drwxr-xr-x   0 chenyk     (501) staff       (20)        0 2023-07-08 02:00:14.079825 seismicpy-0.0.1.4/pyseis/
--rw-r--r--   0 chenyk     (501) staff       (20)       48 2023-07-08 01:10:41.000000 seismicpy-0.0.1.4/pyseis/__init__.py
--rw-r--r--   0 chenyk     (501) staff       (20)     1420 2023-07-08 01:10:41.000000 seismicpy-0.0.1.4/pyseis/npre3d.py
-drwxr-xr-x   0 chenyk     (501) staff       (20)        0 2023-07-08 02:00:14.091260 seismicpy-0.0.1.4/pyseis/src/
--rw-r--r--   0 chenyk     (501) staff       (20)     8113 2023-07-08 01:28:03.000000 seismicpy-0.0.1.4/pyseis/src/npre3d.c
--rw-r--r--   0 chenyk     (501) staff       (20)     3272 2023-07-08 01:28:09.000000 seismicpy-0.0.1.4/pyseis/src/seis_alloc.c
--rw-r--r--   0 chenyk     (501) staff       (20)     1176 2023-07-08 01:29:42.000000 seismicpy-0.0.1.4/pyseis/src/seis_alloc.h
--rw-r--r--   0 chenyk     (501) staff       (20)    15842 2023-07-08 01:29:34.000000 seismicpy-0.0.1.4/pyseis/src/seis_cdivn.c
--rw-r--r--   0 chenyk     (501) staff       (20)     6534 2023-07-08 01:29:29.000000 seismicpy-0.0.1.4/pyseis/src/seis_cdivn.h
--rw-r--r--   0 chenyk     (501) staff       (20)     5294 2023-07-08 01:29:26.000000 seismicpy-0.0.1.4/pyseis/src/seis_conjgrad.c
--rw-r--r--   0 chenyk     (501) staff       (20)     2053 2023-07-08 01:29:22.000000 seismicpy-0.0.1.4/pyseis/src/seis_conjgrad.h
--rw-r--r--   0 chenyk     (501) staff       (20)     2704 2023-07-08 01:29:19.000000 seismicpy-0.0.1.4/pyseis/src/seis_decart.c
--rw-r--r--   0 chenyk     (501) staff       (20)     1637 2023-07-08 01:29:15.000000 seismicpy-0.0.1.4/pyseis/src/seis_decart.h
--rw-r--r--   0 chenyk     (501) staff       (20)      188 2023-07-08 01:29:12.000000 seismicpy-0.0.1.4/pyseis/src/seis_dtype.h
--rw-r--r--   0 chenyk     (501) staff       (20)     2441 2023-07-08 01:29:08.000000 seismicpy-0.0.1.4/pyseis/src/seis_fft1.c
--rw-r--r--   0 chenyk     (501) staff       (20)    18095 2023-07-08 01:29:03.000000 seismicpy-0.0.1.4/pyseis/src/seis_fxynpre.c
--rw-r--r--   0 chenyk     (501) staff       (20)     1952 2023-07-08 01:26:32.000000 seismicpy-0.0.1.4/pyseis/src/seis_fxynpre.h
--rw-r--r--   0 chenyk     (501) staff       (20)    18429 2023-07-08 01:26:24.000000 seismicpy-0.0.1.4/pyseis/src/seis_kissfft.c
--rw-r--r--   0 chenyk     (501) staff       (20)     8687 2023-07-08 01:13:59.000000 seismicpy-0.0.1.4/pyseis/src/seis_kissfft.h
--rw-r--r--   0 chenyk     (501) staff       (20)     8978 2023-07-08 01:28:45.000000 seismicpy-0.0.1.4/pyseis/src/seis_komplex.c
--rw-r--r--   0 chenyk     (501) staff       (20)     3998 2023-07-08 01:28:41.000000 seismicpy-0.0.1.4/pyseis/src/seis_komplex.h
--rw-r--r--   0 chenyk     (501) staff       (20)    10763 2023-07-08 01:28:37.000000 seismicpy-0.0.1.4/pyseis/src/seis_memcpy.c
--rw-r--r--   0 chenyk     (501) staff       (20)     7836 2023-07-08 01:26:04.000000 seismicpy-0.0.1.4/pyseis/src/seis_memcpy.h
--rw-r--r--   0 chenyk     (501) staff       (20)     5699 2023-07-08 01:28:28.000000 seismicpy-0.0.1.4/pyseis/src/seis_ntriangle.c
--rw-r--r--   0 chenyk     (501) staff       (20)     1125 2023-07-08 01:28:19.000000 seismicpy-0.0.1.4/pyseis/src/seis_ntriangle.h
--rw-r--r--   0 chenyk     (501) staff       (20)     2576 2023-07-08 01:25:45.000000 seismicpy-0.0.1.4/pyseis/src/seis_ntrianglen.c
--rw-r--r--   0 chenyk     (501) staff       (20)      599 2023-07-08 01:25:30.000000 seismicpy-0.0.1.4/pyseis/src/seis_ntrianglen.h
--rw-r--r--   0 chenyk     (501) staff       (20)     3266 2023-07-08 01:25:10.000000 seismicpy-0.0.1.4/pyseis/src/seis_triangle.c
--rw-r--r--   0 chenyk     (501) staff       (20)      803 2023-07-08 01:24:36.000000 seismicpy-0.0.1.4/pyseis/src/seis_triangle.h
--rw-r--r--   0 chenyk     (501) staff       (20)     2073 2023-07-08 01:24:47.000000 seismicpy-0.0.1.4/pyseis/src/seis_trianglen.c
--rw-r--r--   0 chenyk     (501) staff       (20)      428 2023-07-08 01:24:55.000000 seismicpy-0.0.1.4/pyseis/src/seis_trianglen.h
--rw-r--r--   0 chenyk     (501) staff       (20)     2651 2023-07-08 01:13:59.000000 seismicpy-0.0.1.4/pyseis/src/seis_win.c
--rw-r--r--   0 chenyk     (501) staff       (20)     1022 2023-07-08 01:13:59.000000 seismicpy-0.0.1.4/pyseis/src/seis_win.h
-drwxr-xr-x   0 chenyk     (501) staff       (20)        0 2023-07-08 02:00:14.094120 seismicpy-0.0.1.4/seismicpy.egg-info/
--rw-r--r--   0 chenyk     (501) staff       (20)     1115 2023-07-08 02:00:13.000000 seismicpy-0.0.1.4/seismicpy.egg-info/PKG-INFO
--rw-r--r--   0 chenyk     (501) staff       (20)      991 2023-07-08 02:00:14.000000 seismicpy-0.0.1.4/seismicpy.egg-info/SOURCES.txt
--rw-r--r--   0 chenyk     (501) staff       (20)        1 2023-07-08 02:00:13.000000 seismicpy-0.0.1.4/seismicpy.egg-info/dependency_links.txt
--rw-r--r--   0 chenyk     (501) staff       (20)        1 2023-07-08 01:40:51.000000 seismicpy-0.0.1.4/seismicpy.egg-info/not-zip-safe
--rw-r--r--   0 chenyk     (501) staff       (20)       53 2023-07-08 02:00:13.000000 seismicpy-0.0.1.4/seismicpy.egg-info/requires.txt
--rw-r--r--   0 chenyk     (501) staff       (20)       18 2023-07-08 02:00:13.000000 seismicpy-0.0.1.4/seismicpy.egg-info/top_level.txt
--rw-r--r--   0 chenyk     (501) staff       (20)       38 2023-07-08 02:00:14.095319 seismicpy-0.0.1.4/setup.cfg
--rw-r--r--   0 chenyk     (501) staff       (20)     2882 2023-07-08 02:00:08.000000 seismicpy-0.0.1.4/setup.py
+drwxr-xr-x   0 chenyk     (501) staff       (20)        0 2023-07-08 02:08:45.847283 seismicpy-0.0.1.4.1/
+-rw-r--r--   0 chenyk     (501) staff       (20)     1117 2023-07-08 02:08:45.846864 seismicpy-0.0.1.4.1/PKG-INFO
+-rw-r--r--   0 chenyk     (501) staff       (20)     3346 2023-07-08 02:04:11.000000 seismicpy-0.0.1.4.1/README.md
+drwxr-xr-x   0 chenyk     (501) staff       (20)        0 2023-07-08 02:08:45.829630 seismicpy-0.0.1.4.1/pyseis/
+-rw-r--r--   0 chenyk     (501) staff       (20)       48 2023-07-08 01:10:41.000000 seismicpy-0.0.1.4.1/pyseis/__init__.py
+-rw-r--r--   0 chenyk     (501) staff       (20)     1420 2023-07-08 01:10:41.000000 seismicpy-0.0.1.4.1/pyseis/npre3d.py
+drwxr-xr-x   0 chenyk     (501) staff       (20)        0 2023-07-08 02:08:45.843335 seismicpy-0.0.1.4.1/pyseis/src/
+-rw-r--r--   0 chenyk     (501) staff       (20)     8113 2023-07-08 01:28:03.000000 seismicpy-0.0.1.4.1/pyseis/src/npre3d.c
+-rw-r--r--   0 chenyk     (501) staff       (20)     3272 2023-07-08 01:28:09.000000 seismicpy-0.0.1.4.1/pyseis/src/seis_alloc.c
+-rw-r--r--   0 chenyk     (501) staff       (20)     1176 2023-07-08 01:29:42.000000 seismicpy-0.0.1.4.1/pyseis/src/seis_alloc.h
+-rw-r--r--   0 chenyk     (501) staff       (20)    15842 2023-07-08 01:29:34.000000 seismicpy-0.0.1.4.1/pyseis/src/seis_cdivn.c
+-rw-r--r--   0 chenyk     (501) staff       (20)     6534 2023-07-08 01:29:29.000000 seismicpy-0.0.1.4.1/pyseis/src/seis_cdivn.h
+-rw-r--r--   0 chenyk     (501) staff       (20)     5294 2023-07-08 01:29:26.000000 seismicpy-0.0.1.4.1/pyseis/src/seis_conjgrad.c
+-rw-r--r--   0 chenyk     (501) staff       (20)     2053 2023-07-08 01:29:22.000000 seismicpy-0.0.1.4.1/pyseis/src/seis_conjgrad.h
+-rw-r--r--   0 chenyk     (501) staff       (20)     2704 2023-07-08 01:29:19.000000 seismicpy-0.0.1.4.1/pyseis/src/seis_decart.c
+-rw-r--r--   0 chenyk     (501) staff       (20)     1637 2023-07-08 01:29:15.000000 seismicpy-0.0.1.4.1/pyseis/src/seis_decart.h
+-rw-r--r--   0 chenyk     (501) staff       (20)      188 2023-07-08 01:29:12.000000 seismicpy-0.0.1.4.1/pyseis/src/seis_dtype.h
+-rw-r--r--   0 chenyk     (501) staff       (20)     2441 2023-07-08 01:29:08.000000 seismicpy-0.0.1.4.1/pyseis/src/seis_fft1.c
+-rw-r--r--   0 chenyk     (501) staff       (20)    18095 2023-07-08 01:29:03.000000 seismicpy-0.0.1.4.1/pyseis/src/seis_fxynpre.c
+-rw-r--r--   0 chenyk     (501) staff       (20)     1952 2023-07-08 01:26:32.000000 seismicpy-0.0.1.4.1/pyseis/src/seis_fxynpre.h
+-rw-r--r--   0 chenyk     (501) staff       (20)    18429 2023-07-08 01:26:24.000000 seismicpy-0.0.1.4.1/pyseis/src/seis_kissfft.c
+-rw-r--r--   0 chenyk     (501) staff       (20)     8687 2023-07-08 01:13:59.000000 seismicpy-0.0.1.4.1/pyseis/src/seis_kissfft.h
+-rw-r--r--   0 chenyk     (501) staff       (20)     8978 2023-07-08 01:28:45.000000 seismicpy-0.0.1.4.1/pyseis/src/seis_komplex.c
+-rw-r--r--   0 chenyk     (501) staff       (20)     3998 2023-07-08 01:28:41.000000 seismicpy-0.0.1.4.1/pyseis/src/seis_komplex.h
+-rw-r--r--   0 chenyk     (501) staff       (20)    10763 2023-07-08 01:28:37.000000 seismicpy-0.0.1.4.1/pyseis/src/seis_memcpy.c
+-rw-r--r--   0 chenyk     (501) staff       (20)     7836 2023-07-08 01:26:04.000000 seismicpy-0.0.1.4.1/pyseis/src/seis_memcpy.h
+-rw-r--r--   0 chenyk     (501) staff       (20)     5699 2023-07-08 01:28:28.000000 seismicpy-0.0.1.4.1/pyseis/src/seis_ntriangle.c
+-rw-r--r--   0 chenyk     (501) staff       (20)     1125 2023-07-08 01:28:19.000000 seismicpy-0.0.1.4.1/pyseis/src/seis_ntriangle.h
+-rw-r--r--   0 chenyk     (501) staff       (20)     2576 2023-07-08 01:25:45.000000 seismicpy-0.0.1.4.1/pyseis/src/seis_ntrianglen.c
+-rw-r--r--   0 chenyk     (501) staff       (20)      599 2023-07-08 01:25:30.000000 seismicpy-0.0.1.4.1/pyseis/src/seis_ntrianglen.h
+-rw-r--r--   0 chenyk     (501) staff       (20)     3266 2023-07-08 01:25:10.000000 seismicpy-0.0.1.4.1/pyseis/src/seis_triangle.c
+-rw-r--r--   0 chenyk     (501) staff       (20)      803 2023-07-08 01:24:36.000000 seismicpy-0.0.1.4.1/pyseis/src/seis_triangle.h
+-rw-r--r--   0 chenyk     (501) staff       (20)     2073 2023-07-08 01:24:47.000000 seismicpy-0.0.1.4.1/pyseis/src/seis_trianglen.c
+-rw-r--r--   0 chenyk     (501) staff       (20)      428 2023-07-08 01:24:55.000000 seismicpy-0.0.1.4.1/pyseis/src/seis_trianglen.h
+-rw-r--r--   0 chenyk     (501) staff       (20)     2651 2023-07-08 01:13:59.000000 seismicpy-0.0.1.4.1/pyseis/src/seis_win.c
+-rw-r--r--   0 chenyk     (501) staff       (20)     1022 2023-07-08 01:13:59.000000 seismicpy-0.0.1.4.1/pyseis/src/seis_win.h
+drwxr-xr-x   0 chenyk     (501) staff       (20)        0 2023-07-08 02:08:45.846234 seismicpy-0.0.1.4.1/seismicpy.egg-info/
+-rw-r--r--   0 chenyk     (501) staff       (20)     1117 2023-07-08 02:08:45.000000 seismicpy-0.0.1.4.1/seismicpy.egg-info/PKG-INFO
+-rw-r--r--   0 chenyk     (501) staff       (20)      991 2023-07-08 02:08:45.000000 seismicpy-0.0.1.4.1/seismicpy.egg-info/SOURCES.txt
+-rw-r--r--   0 chenyk     (501) staff       (20)        1 2023-07-08 02:08:45.000000 seismicpy-0.0.1.4.1/seismicpy.egg-info/dependency_links.txt
+-rw-r--r--   0 chenyk     (501) staff       (20)        1 2023-07-08 01:40:51.000000 seismicpy-0.0.1.4.1/seismicpy.egg-info/not-zip-safe
+-rw-r--r--   0 chenyk     (501) staff       (20)       53 2023-07-08 02:08:45.000000 seismicpy-0.0.1.4.1/seismicpy.egg-info/requires.txt
+-rw-r--r--   0 chenyk     (501) staff       (20)       18 2023-07-08 02:08:45.000000 seismicpy-0.0.1.4.1/seismicpy.egg-info/top_level.txt
+-rw-r--r--   0 chenyk     (501) staff       (20)       38 2023-07-08 02:08:45.847429 seismicpy-0.0.1.4.1/setup.cfg
+-rw-r--r--   0 chenyk     (501) staff       (20)     4005 2023-07-08 02:08:35.000000 seismicpy-0.0.1.4.1/setup.py
```

### Comparing `seismicpy-0.0.1.4/PKG-INFO` & `seismicpy-0.0.1.4.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seismicpy
-Version: 0.0.1.4
+Version: 0.0.1.4.1
 Summary: A python package for seismic data processing and inversion
 Home-page: https://github.com/chenyk1990/pyseis
 Author: pyseis developing team
 Author-email: chenyk2016@gmail.com
 License: GNU General Public License, Version 3 (GPLv3)
 Keywords: seismology,earthquake seismology,exploration seismology,array seismology,denoising,science,engineering,structure,local slope,filtering
 Classifier: Development Status :: 4 - Beta
@@ -17,8 +17,8 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Provides-Extra: docs
 
-Source code: https://github.com/chenyk1990/pyseis
+Source code: https://github.com/chenyk1990/pynpre
```

### Comparing `seismicpy-0.0.1.4/README.md` & `seismicpy-0.0.1.4.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -52,14 +52,16 @@
 
     git clone https://github.com/chenyk1990/pyseis
     cd pyseis
     pip install -v -e .
 or using Pypi
 
     pip install seismicpy
+    
+    pip install git+https://github.com/chenyk1990/pyseis.git
 
 -----------
 ## Examples
     The "demo" directory contains all runable scripts to demonstrate different applications of pyseis. 
 
 -----------
 ## Dependence Packages
```

### Comparing `seismicpy-0.0.1.4/pyseis/npre3d.py` & `seismicpy-0.0.1.4.1/pyseis/npre3d.py`

 * *Files identical despite different names*

### Comparing `seismicpy-0.0.1.4/pyseis/src/npre3d.c` & `seismicpy-0.0.1.4.1/pyseis/src/npre3d.c`

 * *Files identical despite different names*

### Comparing `seismicpy-0.0.1.4/pyseis/src/seis_alloc.c` & `seismicpy-0.0.1.4.1/pyseis/src/seis_alloc.c`

 * *Files identical despite different names*

### Comparing `seismicpy-0.0.1.4/pyseis/src/seis_alloc.h` & `seismicpy-0.0.1.4.1/pyseis/src/seis_alloc.h`

 * *Files identical despite different names*

### Comparing `seismicpy-0.0.1.4/pyseis/src/seis_cdivn.c` & `seismicpy-0.0.1.4.1/pyseis/src/seis_cdivn.c`

 * *Files identical despite different names*

### Comparing `seismicpy-0.0.1.4/pyseis/src/seis_cdivn.h` & `seismicpy-0.0.1.4.1/pyseis/src/seis_cdivn.h`

 * *Files identical despite different names*

### Comparing `seismicpy-0.0.1.4/pyseis/src/seis_conjgrad.c` & `seismicpy-0.0.1.4.1/pyseis/src/seis_conjgrad.c`

 * *Files identical despite different names*

### Comparing `seismicpy-0.0.1.4/pyseis/src/seis_conjgrad.h` & `seismicpy-0.0.1.4.1/pyseis/src/seis_conjgrad.h`

 * *Files identical despite different names*

### Comparing `seismicpy-0.0.1.4/pyseis/src/seis_decart.c` & `seismicpy-0.0.1.4.1/pyseis/src/seis_decart.c`

 * *Files identical despite different names*

### Comparing `seismicpy-0.0.1.4/pyseis/src/seis_decart.h` & `seismicpy-0.0.1.4.1/pyseis/src/seis_decart.h`

 * *Files identical despite different names*

### Comparing `seismicpy-0.0.1.4/pyseis/src/seis_fft1.c` & `seismicpy-0.0.1.4.1/pyseis/src/seis_fft1.c`

 * *Files identical despite different names*

### Comparing `seismicpy-0.0.1.4/pyseis/src/seis_fxynpre.c` & `seismicpy-0.0.1.4.1/pyseis/src/seis_fxynpre.c`

 * *Files identical despite different names*

### Comparing `seismicpy-0.0.1.4/pyseis/src/seis_fxynpre.h` & `seismicpy-0.0.1.4.1/pyseis/src/seis_fxynpre.h`

 * *Files identical despite different names*

### Comparing `seismicpy-0.0.1.4/pyseis/src/seis_kissfft.c` & `seismicpy-0.0.1.4.1/pyseis/src/seis_kissfft.c`

 * *Files identical despite different names*

### Comparing `seismicpy-0.0.1.4/pyseis/src/seis_kissfft.h` & `seismicpy-0.0.1.4.1/pyseis/src/seis_kissfft.h`

 * *Files identical despite different names*

### Comparing `seismicpy-0.0.1.4/pyseis/src/seis_komplex.c` & `seismicpy-0.0.1.4.1/pyseis/src/seis_komplex.c`

 * *Files identical despite different names*

### Comparing `seismicpy-0.0.1.4/pyseis/src/seis_komplex.h` & `seismicpy-0.0.1.4.1/pyseis/src/seis_komplex.h`

 * *Files identical despite different names*

### Comparing `seismicpy-0.0.1.4/pyseis/src/seis_memcpy.c` & `seismicpy-0.0.1.4.1/pyseis/src/seis_memcpy.c`

 * *Files identical despite different names*

### Comparing `seismicpy-0.0.1.4/pyseis/src/seis_memcpy.h` & `seismicpy-0.0.1.4.1/pyseis/src/seis_memcpy.h`

 * *Files identical despite different names*

### Comparing `seismicpy-0.0.1.4/pyseis/src/seis_ntriangle.c` & `seismicpy-0.0.1.4.1/pyseis/src/seis_ntriangle.c`

 * *Files identical despite different names*

### Comparing `seismicpy-0.0.1.4/pyseis/src/seis_ntriangle.h` & `seismicpy-0.0.1.4.1/pyseis/src/seis_ntriangle.h`

 * *Files identical despite different names*

### Comparing `seismicpy-0.0.1.4/pyseis/src/seis_ntrianglen.c` & `seismicpy-0.0.1.4.1/pyseis/src/seis_ntrianglen.c`

 * *Files identical despite different names*

### Comparing `seismicpy-0.0.1.4/pyseis/src/seis_ntrianglen.h` & `seismicpy-0.0.1.4.1/pyseis/src/seis_ntrianglen.h`

 * *Files identical despite different names*

### Comparing `seismicpy-0.0.1.4/pyseis/src/seis_triangle.c` & `seismicpy-0.0.1.4.1/pyseis/src/seis_triangle.c`

 * *Files identical despite different names*

### Comparing `seismicpy-0.0.1.4/pyseis/src/seis_triangle.h` & `seismicpy-0.0.1.4.1/pyseis/src/seis_triangle.h`

 * *Files identical despite different names*

### Comparing `seismicpy-0.0.1.4/pyseis/src/seis_trianglen.c` & `seismicpy-0.0.1.4.1/pyseis/src/seis_trianglen.c`

 * *Files identical despite different names*

### Comparing `seismicpy-0.0.1.4/pyseis/src/seis_win.c` & `seismicpy-0.0.1.4.1/pyseis/src/seis_win.c`

 * *Files identical despite different names*

### Comparing `seismicpy-0.0.1.4/pyseis/src/seis_win.h` & `seismicpy-0.0.1.4.1/pyseis/src/seis_win.h`

 * *Files identical despite different names*

### Comparing `seismicpy-0.0.1.4/seismicpy.egg-info/PKG-INFO` & `seismicpy-0.0.1.4.1/seismicpy.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seismicpy
-Version: 0.0.1.4
+Version: 0.0.1.4.1
 Summary: A python package for seismic data processing and inversion
 Home-page: https://github.com/chenyk1990/pyseis
 Author: pyseis developing team
 Author-email: chenyk2016@gmail.com
 License: GNU General Public License, Version 3 (GPLv3)
 Keywords: seismology,earthquake seismology,exploration seismology,array seismology,denoising,science,engineering,structure,local slope,filtering
 Classifier: Development Status :: 4 - Beta
@@ -17,8 +17,8 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Provides-Extra: docs
 
-Source code: https://github.com/chenyk1990/pyseis
+Source code: https://github.com/chenyk1990/pynpre
```

### Comparing `seismicpy-0.0.1.4/seismicpy.egg-info/SOURCES.txt` & `seismicpy-0.0.1.4.1/seismicpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

