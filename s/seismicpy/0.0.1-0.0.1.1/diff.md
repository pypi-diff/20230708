# Comparing `tmp/seismicpy-0.0.1.tar.gz` & `tmp/seismicpy-0.0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seismicpy-0.0.1.tar", last modified: Sat Jul  8 01:41:00 2023, max compression
+gzip compressed data, was "seismicpy-0.0.1.1.tar", last modified: Sat Jul  8 01:49:31 2023, max compression
```

## Comparing `seismicpy-0.0.1.tar` & `seismicpy-0.0.1.1.tar`

### file list

```diff
@@ -1,31 +1,45 @@
-drwxr-xr-x   0 chenyk     (501) staff       (20)        0 2023-07-08 01:41:00.539949 seismicpy-0.0.1/
--rw-r--r--   0 chenyk     (501) staff       (20)     1113 2023-07-08 01:41:00.539594 seismicpy-0.0.1/PKG-INFO
--rw-r--r--   0 chenyk     (501) staff       (20)     3262 2023-07-08 01:10:41.000000 seismicpy-0.0.1/README.md
-drwxr-xr-x   0 chenyk     (501) staff       (20)        0 2023-07-08 01:41:00.530615 seismicpy-0.0.1/pyseis/
--rw-r--r--   0 chenyk     (501) staff       (20)       48 2023-07-08 01:10:41.000000 seismicpy-0.0.1/pyseis/__init__.py
--rw-r--r--   0 chenyk     (501) staff       (20)     1420 2023-07-08 01:10:41.000000 seismicpy-0.0.1/pyseis/npre3d.py
-drwxr-xr-x   0 chenyk     (501) staff       (20)        0 2023-07-08 01:41:00.536206 seismicpy-0.0.1/pyseis/src/
--rw-r--r--   0 chenyk     (501) staff       (20)     8113 2023-07-08 01:28:03.000000 seismicpy-0.0.1/pyseis/src/npre3d.c
--rw-r--r--   0 chenyk     (501) staff       (20)     3272 2023-07-08 01:28:09.000000 seismicpy-0.0.1/pyseis/src/seis_alloc.c
--rw-r--r--   0 chenyk     (501) staff       (20)    15842 2023-07-08 01:29:34.000000 seismicpy-0.0.1/pyseis/src/seis_cdivn.c
--rw-r--r--   0 chenyk     (501) staff       (20)     5294 2023-07-08 01:29:26.000000 seismicpy-0.0.1/pyseis/src/seis_conjgrad.c
--rw-r--r--   0 chenyk     (501) staff       (20)     2704 2023-07-08 01:29:19.000000 seismicpy-0.0.1/pyseis/src/seis_decart.c
--rw-r--r--   0 chenyk     (501) staff       (20)     2441 2023-07-08 01:29:08.000000 seismicpy-0.0.1/pyseis/src/seis_fft1.c
--rw-r--r--   0 chenyk     (501) staff       (20)    18095 2023-07-08 01:29:03.000000 seismicpy-0.0.1/pyseis/src/seis_fxynpre.c
--rw-r--r--   0 chenyk     (501) staff       (20)    18429 2023-07-08 01:26:24.000000 seismicpy-0.0.1/pyseis/src/seis_kissfft.c
--rw-r--r--   0 chenyk     (501) staff       (20)     8978 2023-07-08 01:28:45.000000 seismicpy-0.0.1/pyseis/src/seis_komplex.c
--rw-r--r--   0 chenyk     (501) staff       (20)    10763 2023-07-08 01:28:37.000000 seismicpy-0.0.1/pyseis/src/seis_memcpy.c
--rw-r--r--   0 chenyk     (501) staff       (20)     5699 2023-07-08 01:28:28.000000 seismicpy-0.0.1/pyseis/src/seis_ntriangle.c
--rw-r--r--   0 chenyk     (501) staff       (20)     2576 2023-07-08 01:25:45.000000 seismicpy-0.0.1/pyseis/src/seis_ntrianglen.c
--rw-r--r--   0 chenyk     (501) staff       (20)     3266 2023-07-08 01:25:10.000000 seismicpy-0.0.1/pyseis/src/seis_triangle.c
--rw-r--r--   0 chenyk     (501) staff       (20)     2073 2023-07-08 01:24:47.000000 seismicpy-0.0.1/pyseis/src/seis_trianglen.c
--rw-r--r--   0 chenyk     (501) staff       (20)     2651 2023-07-08 01:13:59.000000 seismicpy-0.0.1/pyseis/src/seis_win.c
-drwxr-xr-x   0 chenyk     (501) staff       (20)        0 2023-07-08 01:41:00.539043 seismicpy-0.0.1/seismicpy.egg-info/
--rw-r--r--   0 chenyk     (501) staff       (20)     1113 2023-07-08 01:41:00.000000 seismicpy-0.0.1/seismicpy.egg-info/PKG-INFO
--rw-r--r--   0 chenyk     (501) staff       (20)      630 2023-07-08 01:41:00.000000 seismicpy-0.0.1/seismicpy.egg-info/SOURCES.txt
--rw-r--r--   0 chenyk     (501) staff       (20)        1 2023-07-08 01:41:00.000000 seismicpy-0.0.1/seismicpy.egg-info/dependency_links.txt
--rw-r--r--   0 chenyk     (501) staff       (20)        1 2023-07-08 01:40:51.000000 seismicpy-0.0.1/seismicpy.egg-info/not-zip-safe
--rw-r--r--   0 chenyk     (501) staff       (20)       53 2023-07-08 01:41:00.000000 seismicpy-0.0.1/seismicpy.egg-info/requires.txt
--rw-r--r--   0 chenyk     (501) staff       (20)       18 2023-07-08 01:41:00.000000 seismicpy-0.0.1/seismicpy.egg-info/top_level.txt
--rw-r--r--   0 chenyk     (501) staff       (20)       38 2023-07-08 01:41:00.540078 seismicpy-0.0.1/setup.cfg
--rw-r--r--   0 chenyk     (501) staff       (20)     2895 2023-07-08 01:40:48.000000 seismicpy-0.0.1/setup.py
+drwxr-xr-x   0 chenyk     (501) staff       (20)        0 2023-07-08 01:49:31.468039 seismicpy-0.0.1.1/
+-rw-r--r--   0 chenyk     (501) staff       (20)     1115 2023-07-08 01:49:31.467582 seismicpy-0.0.1.1/PKG-INFO
+-rw-r--r--   0 chenyk     (501) staff       (20)     3280 2023-07-08 01:43:38.000000 seismicpy-0.0.1.1/README.md
+drwxr-xr-x   0 chenyk     (501) staff       (20)        0 2023-07-08 01:49:31.449381 seismicpy-0.0.1.1/pyseis/
+-rw-r--r--   0 chenyk     (501) staff       (20)       48 2023-07-08 01:10:41.000000 seismicpy-0.0.1.1/pyseis/__init__.py
+-rw-r--r--   0 chenyk     (501) staff       (20)     1420 2023-07-08 01:10:41.000000 seismicpy-0.0.1.1/pyseis/npre3d.py
+drwxr-xr-x   0 chenyk     (501) staff       (20)        0 2023-07-08 01:49:31.463808 seismicpy-0.0.1.1/pyseis/src/
+-rw-r--r--   0 chenyk     (501) staff       (20)     8113 2023-07-08 01:28:03.000000 seismicpy-0.0.1.1/pyseis/src/npre3d.c
+-rw-r--r--   0 chenyk     (501) staff       (20)     3272 2023-07-08 01:28:09.000000 seismicpy-0.0.1.1/pyseis/src/seis_alloc.c
+-rw-r--r--   0 chenyk     (501) staff       (20)     1176 2023-07-08 01:29:42.000000 seismicpy-0.0.1.1/pyseis/src/seis_alloc.h
+-rw-r--r--   0 chenyk     (501) staff       (20)    15842 2023-07-08 01:29:34.000000 seismicpy-0.0.1.1/pyseis/src/seis_cdivn.c
+-rw-r--r--   0 chenyk     (501) staff       (20)     6534 2023-07-08 01:29:29.000000 seismicpy-0.0.1.1/pyseis/src/seis_cdivn.h
+-rw-r--r--   0 chenyk     (501) staff       (20)     5294 2023-07-08 01:29:26.000000 seismicpy-0.0.1.1/pyseis/src/seis_conjgrad.c
+-rw-r--r--   0 chenyk     (501) staff       (20)     2053 2023-07-08 01:29:22.000000 seismicpy-0.0.1.1/pyseis/src/seis_conjgrad.h
+-rw-r--r--   0 chenyk     (501) staff       (20)     2704 2023-07-08 01:29:19.000000 seismicpy-0.0.1.1/pyseis/src/seis_decart.c
+-rw-r--r--   0 chenyk     (501) staff       (20)     1637 2023-07-08 01:29:15.000000 seismicpy-0.0.1.1/pyseis/src/seis_decart.h
+-rw-r--r--   0 chenyk     (501) staff       (20)      188 2023-07-08 01:29:12.000000 seismicpy-0.0.1.1/pyseis/src/seis_dtype.h
+-rw-r--r--   0 chenyk     (501) staff       (20)     2441 2023-07-08 01:29:08.000000 seismicpy-0.0.1.1/pyseis/src/seis_fft1.c
+-rw-r--r--   0 chenyk     (501) staff       (20)    18095 2023-07-08 01:29:03.000000 seismicpy-0.0.1.1/pyseis/src/seis_fxynpre.c
+-rw-r--r--   0 chenyk     (501) staff       (20)     1952 2023-07-08 01:26:32.000000 seismicpy-0.0.1.1/pyseis/src/seis_fxynpre.h
+-rw-r--r--   0 chenyk     (501) staff       (20)    18429 2023-07-08 01:26:24.000000 seismicpy-0.0.1.1/pyseis/src/seis_kissfft.c
+-rw-r--r--   0 chenyk     (501) staff       (20)     8687 2023-07-08 01:13:59.000000 seismicpy-0.0.1.1/pyseis/src/seis_kissfft.h
+-rw-r--r--   0 chenyk     (501) staff       (20)     8978 2023-07-08 01:28:45.000000 seismicpy-0.0.1.1/pyseis/src/seis_komplex.c
+-rw-r--r--   0 chenyk     (501) staff       (20)     3998 2023-07-08 01:28:41.000000 seismicpy-0.0.1.1/pyseis/src/seis_komplex.h
+-rw-r--r--   0 chenyk     (501) staff       (20)    10763 2023-07-08 01:28:37.000000 seismicpy-0.0.1.1/pyseis/src/seis_memcpy.c
+-rw-r--r--   0 chenyk     (501) staff       (20)     7836 2023-07-08 01:26:04.000000 seismicpy-0.0.1.1/pyseis/src/seis_memcpy.h
+-rw-r--r--   0 chenyk     (501) staff       (20)     5699 2023-07-08 01:28:28.000000 seismicpy-0.0.1.1/pyseis/src/seis_ntriangle.c
+-rw-r--r--   0 chenyk     (501) staff       (20)     1125 2023-07-08 01:28:19.000000 seismicpy-0.0.1.1/pyseis/src/seis_ntriangle.h
+-rw-r--r--   0 chenyk     (501) staff       (20)     2576 2023-07-08 01:25:45.000000 seismicpy-0.0.1.1/pyseis/src/seis_ntrianglen.c
+-rw-r--r--   0 chenyk     (501) staff       (20)      599 2023-07-08 01:25:30.000000 seismicpy-0.0.1.1/pyseis/src/seis_ntrianglen.h
+-rw-r--r--   0 chenyk     (501) staff       (20)     3266 2023-07-08 01:25:10.000000 seismicpy-0.0.1.1/pyseis/src/seis_triangle.c
+-rw-r--r--   0 chenyk     (501) staff       (20)      803 2023-07-08 01:24:36.000000 seismicpy-0.0.1.1/pyseis/src/seis_triangle.h
+-rw-r--r--   0 chenyk     (501) staff       (20)     2073 2023-07-08 01:24:47.000000 seismicpy-0.0.1.1/pyseis/src/seis_trianglen.c
+-rw-r--r--   0 chenyk     (501) staff       (20)      428 2023-07-08 01:24:55.000000 seismicpy-0.0.1.1/pyseis/src/seis_trianglen.h
+-rw-r--r--   0 chenyk     (501) staff       (20)     2651 2023-07-08 01:13:59.000000 seismicpy-0.0.1.1/pyseis/src/seis_win.c
+-rw-r--r--   0 chenyk     (501) staff       (20)     1022 2023-07-08 01:13:59.000000 seismicpy-0.0.1.1/pyseis/src/seis_win.h
+drwxr-xr-x   0 chenyk     (501) staff       (20)        0 2023-07-08 01:49:31.466899 seismicpy-0.0.1.1/seismicpy.egg-info/
+-rw-r--r--   0 chenyk     (501) staff       (20)     1115 2023-07-08 01:49:31.000000 seismicpy-0.0.1.1/seismicpy.egg-info/PKG-INFO
+-rw-r--r--   0 chenyk     (501) staff       (20)      991 2023-07-08 01:49:31.000000 seismicpy-0.0.1.1/seismicpy.egg-info/SOURCES.txt
+-rw-r--r--   0 chenyk     (501) staff       (20)        1 2023-07-08 01:49:31.000000 seismicpy-0.0.1.1/seismicpy.egg-info/dependency_links.txt
+-rw-r--r--   0 chenyk     (501) staff       (20)        1 2023-07-08 01:40:51.000000 seismicpy-0.0.1.1/seismicpy.egg-info/not-zip-safe
+-rw-r--r--   0 chenyk     (501) staff       (20)       53 2023-07-08 01:49:31.000000 seismicpy-0.0.1.1/seismicpy.egg-info/requires.txt
+-rw-r--r--   0 chenyk     (501) staff       (20)       18 2023-07-08 01:49:31.000000 seismicpy-0.0.1.1/seismicpy.egg-info/top_level.txt
+-rw-r--r--   0 chenyk     (501) staff       (20)       38 2023-07-08 01:49:31.468210 seismicpy-0.0.1.1/setup.cfg
+-rw-r--r--   0 chenyk     (501) staff       (20)     3466 2023-07-08 01:49:19.000000 seismicpy-0.0.1.1/setup.py
```

### Comparing `seismicpy-0.0.1/PKG-INFO` & `seismicpy-0.0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seismicpy
-Version: 0.0.1
+Version: 0.0.1.1
 Summary: A python package for seismic data processing and inversion
 Home-page: https://github.com/chenyk1990/pyseis
 Author: pyseis developing team
 Author-email: chenyk2016@gmail.com
 License: GNU General Public License, Version 3 (GPLv3)
 Keywords: seismology,earthquake seismology,exploration seismology,array seismology,denoising,science,engineering,structure,local slope,filtering
 Classifier: Development Status :: 4 - Beta
```

### Comparing `seismicpy-0.0.1/README.md` & `seismicpy-0.0.1.1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-**Pynpre**
+**Pyseis**
 ======
 
 ## Description
 
-**Pynpre* is a python package for denoising and interpolation of multi-dimensional multi-channel seismic data. This package has a variety of applications in both exploration and earthquake seismology.
+**Pyseis* is a python package for denoising and interpolation of multi-dimensional multi-channel seismic data. This package has a variety of applications in both exploration and earthquake seismology.
 
 ## Reference
 Wang et al., 2021, Nonstationary predictive filtering for seismic random noise suppression - A tutorial, Geophysics, 86(3), W21–W30. 
 
 Chen et al., 2021, 5D de-aliased seismic data interpolation using non-stationary prediction error filter, Geophysics, 86(5), V419–V429.
 
 BibTeX:
@@ -34,36 +34,36 @@
 	  pages={V419–V429},
 	  doi={10.1190/geo2020.0540.1},
 	  year={2021}
 	}
 
 -----------
 ## Copyright
-    The pynpre developing team, 2021-present
+    The pyseis developing team, 2021-present
 -----------
 
 ## License
     GNU General Public License, Version 3
     (http://www.gnu.org/copyleft/gpl.html)   
 
 -----------
 
 ## Install
 Using the latest version
 
-    git clone https://github.com/chenyk1990/pynpre
-    cd pynpre
+    git clone https://github.com/chenyk1990/pyseis
+    cd pyseis
     pip install -v -e .
 or using Pypi
 
-    pip install pynpre
+    pip install seismicpy
 
 -----------
 ## Examples
-    The "demo" directory contains all runable scripts to demonstrate different applications of pynpre. 
+    The "demo" directory contains all runable scripts to demonstrate different applications of pyseis. 
 
 -----------
 ## Dependence Packages
 * scipy 
 * numpy 
 * matplotlib
 
@@ -80,24 +80,24 @@
 ## Contact
     Regarding any questions, bugs, developments, collaborations, please contact  
     Yangkang Chen
     chenyk2016@gmail.com
 
 -----------
 ## Gallery
-The gallery figures of the pynpre package can be found at
-    https://github.com/chenyk1990/gallery/tree/main/pynpre
+The gallery figures of the pyseis package can be found at
+    https://github.com/chenyk1990/gallery/tree/main/pyseis
 Each figure in the gallery directory corresponds to a DEMO script in the "demo" directory with the exactly the same file name.
 
 These gallery figures are also presented below. 
 
-DEMO1 (test_pynpre_syn2d.py)
+DEMO1 (test_pyseis_npre_syn2d.py)
 
-<img src='https://github.com/chenyk1990/gallery/blob/main/pynpre/test_pynpre_syn2d.png' alt='DEMO1' width=960/>
+<img src='https://github.com/chenyk1990/gallery/blob/main/pyseis/test_pynpre_syn2d.png' alt='DEMO1' width=960/>
 
-DEMO2 (test_pynpre_syn3d.py) This example is to show that there are no perfect denoising methods. One can work on a certain type of data, but not all. The plane-wave synthetic example is biased towards the damped rank-reduction (DRR) method. However, NPRE works perfectly on curving and non-stationary seismic data.
+DEMO2 (test_pyseis_npre_syn3d.py) This example is to show that there are no perfect denoising methods. One can work on a certain type of data, but not all. The plane-wave synthetic example is biased towards the damped rank-reduction (DRR) method. However, NPRE works perfectly on curving and non-stationary seismic data.
 
-<img src='https://github.com/chenyk1990/gallery/blob/main/pynpre/test_pynpre_syn3d.png' alt='DEMO2' width=960/>
+<img src='https://github.com/chenyk1990/gallery/blob/main/pyseis/test_pynpre_syn3d.png' alt='DEMO2' width=960/>
 
-DEMO3 (test_pynpre_real3d.py) 
+DEMO3 (test_pyseis_npre_real3d.py) 
 
-<img src='https://github.com/chenyk1990/gallery/blob/main/pynpre/test_pynpre_real3d.png' alt='DEMO3' width=960/>
+<img src='https://github.com/chenyk1990/gallery/blob/main/pyseis/test_pynpre_real3d.png' alt='DEMO3' width=960/>
```

### Comparing `seismicpy-0.0.1/pyseis/npre3d.py` & `seismicpy-0.0.1.1/pyseis/npre3d.py`

 * *Files identical despite different names*

### Comparing `seismicpy-0.0.1/pyseis/src/npre3d.c` & `seismicpy-0.0.1.1/pyseis/src/npre3d.c`

 * *Files identical despite different names*

### Comparing `seismicpy-0.0.1/pyseis/src/seis_alloc.c` & `seismicpy-0.0.1.1/pyseis/src/seis_alloc.c`

 * *Files identical despite different names*

### Comparing `seismicpy-0.0.1/pyseis/src/seis_cdivn.c` & `seismicpy-0.0.1.1/pyseis/src/seis_cdivn.c`

 * *Files identical despite different names*

### Comparing `seismicpy-0.0.1/pyseis/src/seis_conjgrad.c` & `seismicpy-0.0.1.1/pyseis/src/seis_conjgrad.c`

 * *Files identical despite different names*

### Comparing `seismicpy-0.0.1/pyseis/src/seis_decart.c` & `seismicpy-0.0.1.1/pyseis/src/seis_decart.c`

 * *Files identical despite different names*

### Comparing `seismicpy-0.0.1/pyseis/src/seis_fft1.c` & `seismicpy-0.0.1.1/pyseis/src/seis_fft1.c`

 * *Files identical despite different names*

### Comparing `seismicpy-0.0.1/pyseis/src/seis_fxynpre.c` & `seismicpy-0.0.1.1/pyseis/src/seis_fxynpre.c`

 * *Files identical despite different names*

### Comparing `seismicpy-0.0.1/pyseis/src/seis_kissfft.c` & `seismicpy-0.0.1.1/pyseis/src/seis_kissfft.c`

 * *Files identical despite different names*

### Comparing `seismicpy-0.0.1/pyseis/src/seis_komplex.c` & `seismicpy-0.0.1.1/pyseis/src/seis_komplex.c`

 * *Files identical despite different names*

### Comparing `seismicpy-0.0.1/pyseis/src/seis_memcpy.c` & `seismicpy-0.0.1.1/pyseis/src/seis_memcpy.c`

 * *Files identical despite different names*

### Comparing `seismicpy-0.0.1/pyseis/src/seis_ntriangle.c` & `seismicpy-0.0.1.1/pyseis/src/seis_ntriangle.c`

 * *Files identical despite different names*

### Comparing `seismicpy-0.0.1/pyseis/src/seis_ntrianglen.c` & `seismicpy-0.0.1.1/pyseis/src/seis_ntrianglen.c`

 * *Files identical despite different names*

### Comparing `seismicpy-0.0.1/pyseis/src/seis_triangle.c` & `seismicpy-0.0.1.1/pyseis/src/seis_triangle.c`

 * *Files identical despite different names*

### Comparing `seismicpy-0.0.1/pyseis/src/seis_trianglen.c` & `seismicpy-0.0.1.1/pyseis/src/seis_trianglen.c`

 * *Files identical despite different names*

### Comparing `seismicpy-0.0.1/pyseis/src/seis_win.c` & `seismicpy-0.0.1.1/pyseis/src/seis_win.c`

 * *Files identical despite different names*

### Comparing `seismicpy-0.0.1/seismicpy.egg-info/PKG-INFO` & `seismicpy-0.0.1.1/seismicpy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seismicpy
-Version: 0.0.1
+Version: 0.0.1.1
 Summary: A python package for seismic data processing and inversion
 Home-page: https://github.com/chenyk1990/pyseis
 Author: pyseis developing team
 Author-email: chenyk2016@gmail.com
 License: GNU General Public License, Version 3 (GPLv3)
 Keywords: seismology,earthquake seismology,exploration seismology,array seismology,denoising,science,engineering,structure,local slope,filtering
 Classifier: Development Status :: 4 - Beta
```

