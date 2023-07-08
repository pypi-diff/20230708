# Comparing `tmp/ragu-0.1.1.tar.gz` & `tmp/ragu-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ragu-0.1.1.tar", last modified: Sat Jul  8 14:16:57 2023, max compression
+gzip compressed data, was "ragu-0.1.2.tar", last modified: Sat Jul  8 14:27:47 2023, max compression
```

## Comparing `ragu-0.1.1.tar` & `ragu-0.1.2.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 btober     (501) staff       (20)        0 2023-07-08 14:16:57.395974 ragu-0.1.1/
--rw-r--r--   0 btober     (501) staff       (20)    35149 2023-07-08 00:09:50.000000 ragu-0.1.1/LICENSE.txt
--rw-r--r--   0 btober     (501) staff       (20)    46803 2023-07-08 14:16:57.395840 ragu-0.1.1/PKG-INFO
--rw-r--r--   0 btober     (501) staff       (20)     5830 2023-07-08 14:14:25.000000 ragu-0.1.1/README.md
--rw-r--r--   0 btober     (501) staff       (20)     1194 2023-07-08 14:15:49.000000 ragu-0.1.1/pyproject.toml
--rw-r--r--   0 btober     (501) staff       (20)       38 2023-07-08 14:16:57.396008 ragu-0.1.1/setup.cfg
--rw-r--r--   0 btober     (501) staff       (20)       91 2023-07-08 14:00:18.000000 ragu-0.1.1/setup.py
-drwxr-xr-x   0 btober     (501) staff       (20)        0 2023-07-08 14:16:57.387185 ragu-0.1.1/src/
-drwxr-xr-x   0 btober     (501) staff       (20)        0 2023-07-08 14:16:57.388707 ragu-0.1.1/src/ragu/
--rw-r--r--   0 btober     (501) staff       (20)        0 2023-07-08 00:09:51.000000 ragu-0.1.1/src/ragu/__init__.py
-drwxr-xr-x   0 btober     (501) staff       (20)        0 2023-07-08 14:16:57.389953 ragu-0.1.1/src/ragu/bin/
--rw-r--r--   0 btober     (501) staff       (20)     1988 2023-07-08 14:00:14.000000 ragu-0.1.1/src/ragu/bin/ragu.py
--rw-r--r--   0 btober     (501) staff       (20)     1993 2023-07-08 00:09:51.000000 ragu-0.1.1/src/ragu/config.py
-drwxr-xr-x   0 btober     (501) staff       (20)        0 2023-07-08 14:16:57.392529 ragu-0.1.1/src/ragu/ingest/
--rw-r--r--   0 btober     (501) staff       (20)     5753 2023-07-08 00:09:51.000000 ragu-0.1.1/src/ragu/ingest/__init__.py
--rw-r--r--   0 btober     (501) staff       (20)     2344 2023-07-08 00:09:51.000000 ragu-0.1.1/src/ragu/ingest/ingest_cresis_rds.py
--rw-r--r--   0 btober     (501) staff       (20)     2387 2023-07-08 00:09:51.000000 ragu-0.1.1/src/ragu/ingest/ingest_cresis_snow.py
--rw-r--r--   0 btober     (501) staff       (20)     2935 2023-07-08 00:09:51.000000 ragu-0.1.1/src/ragu/ingest/ingest_groundhog.py
--rw-r--r--   0 btober     (501) staff       (20)     3299 2023-07-08 00:09:51.000000 ragu-0.1.1/src/ragu/ingest/ingest_gssi.py
--rw-r--r--   0 btober     (501) staff       (20)     2495 2023-07-08 00:09:51.000000 ragu-0.1.1/src/ragu/ingest/ingest_lrs.py
--rw-r--r--   0 btober     (501) staff       (20)     2829 2023-07-08 00:09:51.000000 ragu-0.1.1/src/ragu/ingest/ingest_marsis.py
--rw-r--r--   0 btober     (501) staff       (20)     2407 2023-07-08 00:09:51.000000 ragu-0.1.1/src/ragu/ingest/ingest_marsis_ipc.py
--rw-r--r--   0 btober     (501) staff       (20)     5713 2023-07-08 00:09:51.000000 ragu-0.1.1/src/ragu/ingest/ingest_oibAK.py
--rw-r--r--   0 btober     (501) staff       (20)    14114 2023-07-08 00:09:51.000000 ragu-0.1.1/src/ragu/ingest/ingest_pulseekko.py
--rw-r--r--   0 btober     (501) staff       (20)     2470 2023-07-08 00:09:51.000000 ragu-0.1.1/src/ragu/ingest/ingest_rimfax.py
--rw-r--r--   0 btober     (501) staff       (20)     2864 2023-07-08 00:09:51.000000 ragu-0.1.1/src/ragu/ingest/ingest_sharad.py
--rw-r--r--   0 btober     (501) staff       (20)     3573 2023-07-08 00:09:51.000000 ragu-0.1.1/src/ragu/ingest/ingest_template.py
--rw-r--r--   0 btober     (501) staff       (20)     2444 2023-07-08 00:09:51.000000 ragu-0.1.1/src/ragu/ingest/ingest_uaf_kentech.py
-drwxr-xr-x   0 btober     (501) staff       (20)        0 2023-07-08 14:16:57.392943 ragu-0.1.1/src/ragu/nav/
--rw-r--r--   0 btober     (501) staff       (20)      153 2023-07-08 00:09:51.000000 ragu-0.1.1/src/ragu/nav/__init__.py
--rw-r--r--   0 btober     (501) staff       (20)     5086 2023-07-08 00:09:51.000000 ragu-0.1.1/src/ragu/nav/gps.py
--rw-r--r--   0 btober     (501) staff       (20)    20723 2023-07-08 00:09:51.000000 ragu-0.1.1/src/ragu/nav/navparse.py
-drwxr-xr-x   0 btober     (501) staff       (20)        0 2023-07-08 14:16:57.393559 ragu-0.1.1/src/ragu/radar/
--rw-r--r--   0 btober     (501) staff       (20)     7537 2023-07-08 00:09:51.000000 ragu-0.1.1/src/ragu/radar/__init__.py
--rw-r--r--   0 btober     (501) staff       (20)      505 2023-07-08 00:09:51.000000 ragu-0.1.1/src/ragu/radar/flags.py
--rw-r--r--   0 btober     (501) staff       (20)     1185 2023-07-08 00:09:51.000000 ragu-0.1.1/src/ragu/radar/pick.py
--rw-r--r--   0 btober     (501) staff       (20)    11495 2023-07-08 00:09:51.000000 ragu-0.1.1/src/ragu/radar/processing.py
--rw-r--r--   0 btober     (501) staff       (20)      225 2023-07-08 00:09:51.000000 ragu-0.1.1/src/ragu/raguError.py
-drwxr-xr-x   0 btober     (501) staff       (20)        0 2023-07-08 14:16:57.394381 ragu-0.1.1/src/ragu/tools/
--rw-r--r--   0 btober     (501) staff       (20)      152 2023-07-08 00:09:51.000000 ragu-0.1.1/src/ragu/tools/__init__.py
--rw-r--r--   0 btober     (501) staff       (20)      481 2023-07-08 00:09:51.000000 ragu-0.1.1/src/ragu/tools/constants.py
--rw-r--r--   0 btober     (501) staff       (20)     9427 2023-07-08 00:09:51.000000 ragu-0.1.1/src/ragu/tools/export.py
--rw-r--r--   0 btober     (501) staff       (20)     9845 2023-07-08 00:09:51.000000 ragu-0.1.1/src/ragu/tools/utils.py
-drwxr-xr-x   0 btober     (501) staff       (20)        0 2023-07-08 14:16:57.395550 ragu-0.1.1/src/ragu/ui/
--rw-r--r--   0 btober     (501) staff       (20)      152 2023-07-08 00:09:51.000000 ragu-0.1.1/src/ragu/ui/__init__.py
--rw-r--r--   0 btober     (501) staff       (20)    16554 2023-07-08 00:09:51.000000 ragu-0.1.1/src/ragu/ui/basemap.py
--rw-r--r--   0 btober     (501) staff       (20)    68357 2023-07-08 00:09:51.000000 ragu-0.1.1/src/ragu/ui/gui.py
--rw-r--r--   0 btober     (501) staff       (20)    70973 2023-07-08 00:09:51.000000 ragu-0.1.1/src/ragu/ui/impick.py
--rw-r--r--   0 btober     (501) staff       (20)    10803 2023-07-08 00:09:51.000000 ragu-0.1.1/src/ragu/ui/notepad.py
--rw-r--r--   0 btober     (501) staff       (20)    23544 2023-07-08 00:09:51.000000 ragu-0.1.1/src/ragu/ui/wvpick.py
-drwxr-xr-x   0 btober     (501) staff       (20)        0 2023-07-08 14:16:57.389835 ragu-0.1.1/src/ragu.egg-info/
--rw-r--r--   0 btober     (501) staff       (20)    46803 2023-07-08 14:16:57.000000 ragu-0.1.1/src/ragu.egg-info/PKG-INFO
--rw-r--r--   0 btober     (501) staff       (20)     1209 2023-07-08 14:16:57.000000 ragu-0.1.1/src/ragu.egg-info/SOURCES.txt
--rw-r--r--   0 btober     (501) staff       (20)        1 2023-07-08 14:16:57.000000 ragu-0.1.1/src/ragu.egg-info/dependency_links.txt
--rw-r--r--   0 btober     (501) staff       (20)       44 2023-07-08 14:16:57.000000 ragu-0.1.1/src/ragu.egg-info/entry_points.txt
--rw-r--r--   0 btober     (501) staff       (20)       64 2023-07-08 14:16:57.000000 ragu-0.1.1/src/ragu.egg-info/requires.txt
--rw-r--r--   0 btober     (501) staff       (20)       19 2023-07-08 14:16:57.000000 ragu-0.1.1/src/ragu.egg-info/top_level.txt
+drwxr-xr-x   0 btober     (501) staff       (20)        0 2023-07-08 14:27:47.767211 ragu-0.1.2/
+-rw-r--r--   0 btober     (501) staff       (20)    35149 2023-07-08 00:09:50.000000 ragu-0.1.2/LICENSE.txt
+-rw-r--r--   0 btober     (501) staff       (20)    46800 2023-07-08 14:27:47.767075 ragu-0.1.2/PKG-INFO
+-rw-r--r--   0 btober     (501) staff       (20)     5827 2023-07-08 14:26:19.000000 ragu-0.1.2/README.md
+-rw-r--r--   0 btober     (501) staff       (20)     1194 2023-07-08 14:26:06.000000 ragu-0.1.2/pyproject.toml
+-rw-r--r--   0 btober     (501) staff       (20)       38 2023-07-08 14:27:47.767253 ragu-0.1.2/setup.cfg
+-rw-r--r--   0 btober     (501) staff       (20)       91 2023-07-08 14:00:18.000000 ragu-0.1.2/setup.py
+drwxr-xr-x   0 btober     (501) staff       (20)        0 2023-07-08 14:27:47.758719 ragu-0.1.2/src/
+drwxr-xr-x   0 btober     (501) staff       (20)        0 2023-07-08 14:27:47.760189 ragu-0.1.2/src/ragu/
+-rw-r--r--   0 btober     (501) staff       (20)        0 2023-07-08 00:09:51.000000 ragu-0.1.2/src/ragu/__init__.py
+drwxr-xr-x   0 btober     (501) staff       (20)        0 2023-07-08 14:27:47.761342 ragu-0.1.2/src/ragu/bin/
+-rw-r--r--   0 btober     (501) staff       (20)     1988 2023-07-08 14:00:14.000000 ragu-0.1.2/src/ragu/bin/ragu.py
+-rw-r--r--   0 btober     (501) staff       (20)     1993 2023-07-08 00:09:51.000000 ragu-0.1.2/src/ragu/config.py
+drwxr-xr-x   0 btober     (501) staff       (20)        0 2023-07-08 14:27:47.763622 ragu-0.1.2/src/ragu/ingest/
+-rw-r--r--   0 btober     (501) staff       (20)     5753 2023-07-08 00:09:51.000000 ragu-0.1.2/src/ragu/ingest/__init__.py
+-rw-r--r--   0 btober     (501) staff       (20)     2344 2023-07-08 00:09:51.000000 ragu-0.1.2/src/ragu/ingest/ingest_cresis_rds.py
+-rw-r--r--   0 btober     (501) staff       (20)     2387 2023-07-08 00:09:51.000000 ragu-0.1.2/src/ragu/ingest/ingest_cresis_snow.py
+-rw-r--r--   0 btober     (501) staff       (20)     2935 2023-07-08 00:09:51.000000 ragu-0.1.2/src/ragu/ingest/ingest_groundhog.py
+-rw-r--r--   0 btober     (501) staff       (20)     3299 2023-07-08 00:09:51.000000 ragu-0.1.2/src/ragu/ingest/ingest_gssi.py
+-rw-r--r--   0 btober     (501) staff       (20)     2495 2023-07-08 00:09:51.000000 ragu-0.1.2/src/ragu/ingest/ingest_lrs.py
+-rw-r--r--   0 btober     (501) staff       (20)     2829 2023-07-08 00:09:51.000000 ragu-0.1.2/src/ragu/ingest/ingest_marsis.py
+-rw-r--r--   0 btober     (501) staff       (20)     2407 2023-07-08 00:09:51.000000 ragu-0.1.2/src/ragu/ingest/ingest_marsis_ipc.py
+-rw-r--r--   0 btober     (501) staff       (20)     5713 2023-07-08 00:09:51.000000 ragu-0.1.2/src/ragu/ingest/ingest_oibAK.py
+-rw-r--r--   0 btober     (501) staff       (20)    14114 2023-07-08 00:09:51.000000 ragu-0.1.2/src/ragu/ingest/ingest_pulseekko.py
+-rw-r--r--   0 btober     (501) staff       (20)     2470 2023-07-08 00:09:51.000000 ragu-0.1.2/src/ragu/ingest/ingest_rimfax.py
+-rw-r--r--   0 btober     (501) staff       (20)     2864 2023-07-08 00:09:51.000000 ragu-0.1.2/src/ragu/ingest/ingest_sharad.py
+-rw-r--r--   0 btober     (501) staff       (20)     3573 2023-07-08 00:09:51.000000 ragu-0.1.2/src/ragu/ingest/ingest_template.py
+-rw-r--r--   0 btober     (501) staff       (20)     2444 2023-07-08 00:09:51.000000 ragu-0.1.2/src/ragu/ingest/ingest_uaf_kentech.py
+drwxr-xr-x   0 btober     (501) staff       (20)        0 2023-07-08 14:27:47.764040 ragu-0.1.2/src/ragu/nav/
+-rw-r--r--   0 btober     (501) staff       (20)      153 2023-07-08 00:09:51.000000 ragu-0.1.2/src/ragu/nav/__init__.py
+-rw-r--r--   0 btober     (501) staff       (20)     5086 2023-07-08 00:09:51.000000 ragu-0.1.2/src/ragu/nav/gps.py
+-rw-r--r--   0 btober     (501) staff       (20)    20723 2023-07-08 00:09:51.000000 ragu-0.1.2/src/ragu/nav/navparse.py
+drwxr-xr-x   0 btober     (501) staff       (20)        0 2023-07-08 14:27:47.764704 ragu-0.1.2/src/ragu/radar/
+-rw-r--r--   0 btober     (501) staff       (20)     7537 2023-07-08 00:09:51.000000 ragu-0.1.2/src/ragu/radar/__init__.py
+-rw-r--r--   0 btober     (501) staff       (20)      505 2023-07-08 00:09:51.000000 ragu-0.1.2/src/ragu/radar/flags.py
+-rw-r--r--   0 btober     (501) staff       (20)     1185 2023-07-08 00:09:51.000000 ragu-0.1.2/src/ragu/radar/pick.py
+-rw-r--r--   0 btober     (501) staff       (20)    11495 2023-07-08 00:09:51.000000 ragu-0.1.2/src/ragu/radar/processing.py
+-rw-r--r--   0 btober     (501) staff       (20)      225 2023-07-08 00:09:51.000000 ragu-0.1.2/src/ragu/raguError.py
+drwxr-xr-x   0 btober     (501) staff       (20)        0 2023-07-08 14:27:47.765418 ragu-0.1.2/src/ragu/tools/
+-rw-r--r--   0 btober     (501) staff       (20)      152 2023-07-08 00:09:51.000000 ragu-0.1.2/src/ragu/tools/__init__.py
+-rw-r--r--   0 btober     (501) staff       (20)      481 2023-07-08 00:09:51.000000 ragu-0.1.2/src/ragu/tools/constants.py
+-rw-r--r--   0 btober     (501) staff       (20)     9427 2023-07-08 00:09:51.000000 ragu-0.1.2/src/ragu/tools/export.py
+-rw-r--r--   0 btober     (501) staff       (20)     9845 2023-07-08 00:09:51.000000 ragu-0.1.2/src/ragu/tools/utils.py
+drwxr-xr-x   0 btober     (501) staff       (20)        0 2023-07-08 14:27:47.766749 ragu-0.1.2/src/ragu/ui/
+-rw-r--r--   0 btober     (501) staff       (20)      152 2023-07-08 00:09:51.000000 ragu-0.1.2/src/ragu/ui/__init__.py
+-rw-r--r--   0 btober     (501) staff       (20)    16554 2023-07-08 00:09:51.000000 ragu-0.1.2/src/ragu/ui/basemap.py
+-rw-r--r--   0 btober     (501) staff       (20)    68357 2023-07-08 00:09:51.000000 ragu-0.1.2/src/ragu/ui/gui.py
+-rw-r--r--   0 btober     (501) staff       (20)    70973 2023-07-08 00:09:51.000000 ragu-0.1.2/src/ragu/ui/impick.py
+-rw-r--r--   0 btober     (501) staff       (20)    10803 2023-07-08 00:09:51.000000 ragu-0.1.2/src/ragu/ui/notepad.py
+-rw-r--r--   0 btober     (501) staff       (20)    23544 2023-07-08 00:09:51.000000 ragu-0.1.2/src/ragu/ui/wvpick.py
+drwxr-xr-x   0 btober     (501) staff       (20)        0 2023-07-08 14:27:47.761214 ragu-0.1.2/src/ragu.egg-info/
+-rw-r--r--   0 btober     (501) staff       (20)    46800 2023-07-08 14:27:47.000000 ragu-0.1.2/src/ragu.egg-info/PKG-INFO
+-rw-r--r--   0 btober     (501) staff       (20)     1209 2023-07-08 14:27:47.000000 ragu-0.1.2/src/ragu.egg-info/SOURCES.txt
+-rw-r--r--   0 btober     (501) staff       (20)        1 2023-07-08 14:27:47.000000 ragu-0.1.2/src/ragu.egg-info/dependency_links.txt
+-rw-r--r--   0 btober     (501) staff       (20)       44 2023-07-08 14:27:47.000000 ragu-0.1.2/src/ragu.egg-info/entry_points.txt
+-rw-r--r--   0 btober     (501) staff       (20)       64 2023-07-08 14:27:47.000000 ragu-0.1.2/src/ragu.egg-info/requires.txt
+-rw-r--r--   0 btober     (501) staff       (20)       19 2023-07-08 14:27:47.000000 ragu-0.1.2/src/ragu.egg-info/top_level.txt
```

### Comparing `ragu-0.1.1/LICENSE.txt` & `ragu-0.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ragu-0.1.1/PKG-INFO` & `ragu-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ragu
-Version: 0.1.1
+Version: 0.1.2
 Summary: Radar Analysis Graphical Utility (RAGU)
 Author: Brandon S. Tober
 Author-email: tobers.brandon@gmail.com
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
@@ -682,15 +682,15 @@
 Project-URL: documentation, https://github.com/btobers/ragu/wiki
 Project-URL: repository, https://github.com/btobers/ragu
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
-<img src="https://github.com/btobers/RAGU/blob/master/src/recs/ragu_logo.png" height="200">
+<img src="https://github.com/btobers/RAGU/raw/master/src/recs/ragu_logo.png" height="200">
 
 # Radar Analysis Graphical Utility
 ### Authors: Brandon Tober and Michael Christoffersen
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.3968981.svg)](https://doi.org/10.5281/zenodo.3968981)
 
 ## What is RAGU?
 RAGU is a user-interface radar interpretation software written in Python 3 and released under the GNU General Public License v3. RAGU was originally developed to ingest and interpret NASA Operation IceBridge airborne radar sounding data, but has been expanded for use with other sounder and ground penetrating radar datasets. While RAGU is primarily an interpretation software, minimal radar processing tools are included with the software.
@@ -731,15 +731,15 @@
 2. **Geopackage (.gpkg)**
 
     For **CSV** and **Geopackage** files, see the [format file](https://github.com/btobers/RAGU/blob/master/docs/RAGU_pk_format.pdf) in for per trace export attribute information.
 
 #### Figure:
 A figure each may also be exported for the uninterpreted radar profile, the accompanying clutter simulation, and the interpreted radar profile. Example over Malaspina Glacier, AK:  
 <p align="center">
-  <img src="https://github.com/btobers/RAGU/blob/master/src/recs/20190928-235534_compiled.jpg" height="500"><br>
+  <img src="https://github.com/btobers/RAGU/raw/master/src/recs/20190928-235534_compiled.jpg" height="500"><br>
 </p>
 
 #### Processing Script:
 A file log/processing script may also be exported to keep track of and easily repeat any data processing steps. Example processing script:
 ```
 ### RAGU processing log ###
 import sys
@@ -780,15 +780,15 @@
 $ pip install ragu
 ```
 
 2. To run ragu, call ragu from the command line to initialize the GUI:
 ```
 $ ragu
 ```
-**Nonte: The first time ragu is run on your machine, a configuration file will be created at *~/RAGU/config.ini*.** This configuration file can be edited to set appropriate data paths, data coordinate reference system, and output preferences. Path variables may be left blank, but must remain uncommented. An example ragu configuration file can be found [here](https://github.com/btobers/RAGU/blob/master/src/docs/config.ini).
+**Nonte: The first time ragu is run on your machine, a configuration file will be created at *~/RAGU/config.ini*.** This configuration file can be edited to set appropriate data paths, data coordinate reference system, and output preferences. Path variables may be left blank, but must remain uncommented. An example ragu configuration file can be found [here](https://github.com/btobers/RAGU/raw/master/src/docs/config.ini).
 
 
 ## Notes
 Several auxiliary tools which RAGU users may find useful can be found at [radar_tools](https://github.com/btobers/radar_tools)
 
 ### Future Development
 Additional dataset ingesters:
```

### Comparing `ragu-0.1.1/README.md` & `ragu-0.1.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-<img src="https://github.com/btobers/RAGU/blob/master/src/recs/ragu_logo.png" height="200">
+<img src="https://github.com/btobers/RAGU/raw/master/src/recs/ragu_logo.png" height="200">
 
 # Radar Analysis Graphical Utility
 ### Authors: Brandon Tober and Michael Christoffersen
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.3968981.svg)](https://doi.org/10.5281/zenodo.3968981)
 
 ## What is RAGU?
 RAGU is a user-interface radar interpretation software written in Python 3 and released under the GNU General Public License v3. RAGU was originally developed to ingest and interpret NASA Operation IceBridge airborne radar sounding data, but has been expanded for use with other sounder and ground penetrating radar datasets. While RAGU is primarily an interpretation software, minimal radar processing tools are included with the software.
@@ -43,15 +43,15 @@
 2. **Geopackage (.gpkg)**
 
     For **CSV** and **Geopackage** files, see the [format file](https://github.com/btobers/RAGU/blob/master/docs/RAGU_pk_format.pdf) in for per trace export attribute information.
 
 #### Figure:
 A figure each may also be exported for the uninterpreted radar profile, the accompanying clutter simulation, and the interpreted radar profile. Example over Malaspina Glacier, AK:  
 <p align="center">
-  <img src="https://github.com/btobers/RAGU/blob/master/src/recs/20190928-235534_compiled.jpg" height="500"><br>
+  <img src="https://github.com/btobers/RAGU/raw/master/src/recs/20190928-235534_compiled.jpg" height="500"><br>
 </p>
 
 #### Processing Script:
 A file log/processing script may also be exported to keep track of and easily repeat any data processing steps. Example processing script:
 ```
 ### RAGU processing log ###
 import sys
@@ -92,15 +92,15 @@
 $ pip install ragu
 ```
 
 2. To run ragu, call ragu from the command line to initialize the GUI:
 ```
 $ ragu
 ```
-**Nonte: The first time ragu is run on your machine, a configuration file will be created at *~/RAGU/config.ini*.** This configuration file can be edited to set appropriate data paths, data coordinate reference system, and output preferences. Path variables may be left blank, but must remain uncommented. An example ragu configuration file can be found [here](https://github.com/btobers/RAGU/blob/master/src/docs/config.ini).
+**Nonte: The first time ragu is run on your machine, a configuration file will be created at *~/RAGU/config.ini*.** This configuration file can be edited to set appropriate data paths, data coordinate reference system, and output preferences. Path variables may be left blank, but must remain uncommented. An example ragu configuration file can be found [here](https://github.com/btobers/RAGU/raw/master/src/docs/config.ini).
 
 
 ## Notes
 Several auxiliary tools which RAGU users may find useful can be found at [radar_tools](https://github.com/btobers/radar_tools)
 
 ### Future Development
 Additional dataset ingesters:
```

### Comparing `ragu-0.1.1/pyproject.toml` & `ragu-0.1.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ragu"
-version = "0.1.1"
+version = "0.1.2"
 description = "Radar Analysis Graphical Utility (RAGU)"
 readme = "README.md"
 requires-python = ">=3.6"
 license = {file = "LICENSE.txt"}
 authors = [
     {name = "Brandon S. Tober"},
     {email = "tobers.brandon@gmail.com"}
```

### Comparing `ragu-0.1.1/src/ragu/bin/ragu.py` & `ragu-0.1.2/src/ragu/bin/ragu.py`

 * *Files identical despite different names*

### Comparing `ragu-0.1.1/src/ragu/config.py` & `ragu-0.1.2/src/ragu/config.py`

 * *Files identical despite different names*

### Comparing `ragu-0.1.1/src/ragu/ingest/__init__.py` & `ragu-0.1.2/src/ragu/ingest/__init__.py`

 * *Files identical despite different names*

### Comparing `ragu-0.1.1/src/ragu/ingest/ingest_cresis_rds.py` & `ragu-0.1.2/src/ragu/ingest/ingest_cresis_rds.py`

 * *Files identical despite different names*

### Comparing `ragu-0.1.1/src/ragu/ingest/ingest_cresis_snow.py` & `ragu-0.1.2/src/ragu/ingest/ingest_cresis_snow.py`

 * *Files identical despite different names*

### Comparing `ragu-0.1.1/src/ragu/ingest/ingest_groundhog.py` & `ragu-0.1.2/src/ragu/ingest/ingest_groundhog.py`

 * *Files identical despite different names*

### Comparing `ragu-0.1.1/src/ragu/ingest/ingest_gssi.py` & `ragu-0.1.2/src/ragu/ingest/ingest_gssi.py`

 * *Files identical despite different names*

### Comparing `ragu-0.1.1/src/ragu/ingest/ingest_lrs.py` & `ragu-0.1.2/src/ragu/ingest/ingest_lrs.py`

 * *Files identical despite different names*

### Comparing `ragu-0.1.1/src/ragu/ingest/ingest_marsis.py` & `ragu-0.1.2/src/ragu/ingest/ingest_marsis.py`

 * *Files identical despite different names*

### Comparing `ragu-0.1.1/src/ragu/ingest/ingest_marsis_ipc.py` & `ragu-0.1.2/src/ragu/ingest/ingest_marsis_ipc.py`

 * *Files identical despite different names*

### Comparing `ragu-0.1.1/src/ragu/ingest/ingest_oibAK.py` & `ragu-0.1.2/src/ragu/ingest/ingest_oibAK.py`

 * *Files identical despite different names*

### Comparing `ragu-0.1.1/src/ragu/ingest/ingest_pulseekko.py` & `ragu-0.1.2/src/ragu/ingest/ingest_pulseekko.py`

 * *Files identical despite different names*

### Comparing `ragu-0.1.1/src/ragu/ingest/ingest_rimfax.py` & `ragu-0.1.2/src/ragu/ingest/ingest_rimfax.py`

 * *Files identical despite different names*

### Comparing `ragu-0.1.1/src/ragu/ingest/ingest_sharad.py` & `ragu-0.1.2/src/ragu/ingest/ingest_sharad.py`

 * *Files identical despite different names*

### Comparing `ragu-0.1.1/src/ragu/ingest/ingest_template.py` & `ragu-0.1.2/src/ragu/ingest/ingest_template.py`

 * *Files identical despite different names*

### Comparing `ragu-0.1.1/src/ragu/ingest/ingest_uaf_kentech.py` & `ragu-0.1.2/src/ragu/ingest/ingest_uaf_kentech.py`

 * *Files identical despite different names*

### Comparing `ragu-0.1.1/src/ragu/nav/gps.py` & `ragu-0.1.2/src/ragu/nav/gps.py`

 * *Files identical despite different names*

### Comparing `ragu-0.1.1/src/ragu/nav/navparse.py` & `ragu-0.1.2/src/ragu/nav/navparse.py`

 * *Files identical despite different names*

### Comparing `ragu-0.1.1/src/ragu/radar/__init__.py` & `ragu-0.1.2/src/ragu/radar/__init__.py`

 * *Files identical despite different names*

### Comparing `ragu-0.1.1/src/ragu/radar/pick.py` & `ragu-0.1.2/src/ragu/radar/pick.py`

 * *Files identical despite different names*

### Comparing `ragu-0.1.1/src/ragu/radar/processing.py` & `ragu-0.1.2/src/ragu/radar/processing.py`

 * *Files identical despite different names*

### Comparing `ragu-0.1.1/src/ragu/tools/export.py` & `ragu-0.1.2/src/ragu/tools/export.py`

 * *Files identical despite different names*

### Comparing `ragu-0.1.1/src/ragu/tools/utils.py` & `ragu-0.1.2/src/ragu/tools/utils.py`

 * *Files identical despite different names*

### Comparing `ragu-0.1.1/src/ragu/ui/basemap.py` & `ragu-0.1.2/src/ragu/ui/basemap.py`

 * *Files identical despite different names*

### Comparing `ragu-0.1.1/src/ragu/ui/gui.py` & `ragu-0.1.2/src/ragu/ui/gui.py`

 * *Files identical despite different names*

### Comparing `ragu-0.1.1/src/ragu/ui/impick.py` & `ragu-0.1.2/src/ragu/ui/impick.py`

 * *Files identical despite different names*

### Comparing `ragu-0.1.1/src/ragu/ui/notepad.py` & `ragu-0.1.2/src/ragu/ui/notepad.py`

 * *Files identical despite different names*

### Comparing `ragu-0.1.1/src/ragu/ui/wvpick.py` & `ragu-0.1.2/src/ragu/ui/wvpick.py`

 * *Files identical despite different names*

### Comparing `ragu-0.1.1/src/ragu.egg-info/PKG-INFO` & `ragu-0.1.2/src/ragu.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ragu
-Version: 0.1.1
+Version: 0.1.2
 Summary: Radar Analysis Graphical Utility (RAGU)
 Author: Brandon S. Tober
 Author-email: tobers.brandon@gmail.com
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
@@ -682,15 +682,15 @@
 Project-URL: documentation, https://github.com/btobers/ragu/wiki
 Project-URL: repository, https://github.com/btobers/ragu
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
-<img src="https://github.com/btobers/RAGU/blob/master/src/recs/ragu_logo.png" height="200">
+<img src="https://github.com/btobers/RAGU/raw/master/src/recs/ragu_logo.png" height="200">
 
 # Radar Analysis Graphical Utility
 ### Authors: Brandon Tober and Michael Christoffersen
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.3968981.svg)](https://doi.org/10.5281/zenodo.3968981)
 
 ## What is RAGU?
 RAGU is a user-interface radar interpretation software written in Python 3 and released under the GNU General Public License v3. RAGU was originally developed to ingest and interpret NASA Operation IceBridge airborne radar sounding data, but has been expanded for use with other sounder and ground penetrating radar datasets. While RAGU is primarily an interpretation software, minimal radar processing tools are included with the software.
@@ -731,15 +731,15 @@
 2. **Geopackage (.gpkg)**
 
     For **CSV** and **Geopackage** files, see the [format file](https://github.com/btobers/RAGU/blob/master/docs/RAGU_pk_format.pdf) in for per trace export attribute information.
 
 #### Figure:
 A figure each may also be exported for the uninterpreted radar profile, the accompanying clutter simulation, and the interpreted radar profile. Example over Malaspina Glacier, AK:  
 <p align="center">
-  <img src="https://github.com/btobers/RAGU/blob/master/src/recs/20190928-235534_compiled.jpg" height="500"><br>
+  <img src="https://github.com/btobers/RAGU/raw/master/src/recs/20190928-235534_compiled.jpg" height="500"><br>
 </p>
 
 #### Processing Script:
 A file log/processing script may also be exported to keep track of and easily repeat any data processing steps. Example processing script:
 ```
 ### RAGU processing log ###
 import sys
@@ -780,15 +780,15 @@
 $ pip install ragu
 ```
 
 2. To run ragu, call ragu from the command line to initialize the GUI:
 ```
 $ ragu
 ```
-**Nonte: The first time ragu is run on your machine, a configuration file will be created at *~/RAGU/config.ini*.** This configuration file can be edited to set appropriate data paths, data coordinate reference system, and output preferences. Path variables may be left blank, but must remain uncommented. An example ragu configuration file can be found [here](https://github.com/btobers/RAGU/blob/master/src/docs/config.ini).
+**Nonte: The first time ragu is run on your machine, a configuration file will be created at *~/RAGU/config.ini*.** This configuration file can be edited to set appropriate data paths, data coordinate reference system, and output preferences. Path variables may be left blank, but must remain uncommented. An example ragu configuration file can be found [here](https://github.com/btobers/RAGU/raw/master/src/docs/config.ini).
 
 
 ## Notes
 Several auxiliary tools which RAGU users may find useful can be found at [radar_tools](https://github.com/btobers/radar_tools)
 
 ### Future Development
 Additional dataset ingesters:
```

### Comparing `ragu-0.1.1/src/ragu.egg-info/SOURCES.txt` & `ragu-0.1.2/src/ragu.egg-info/SOURCES.txt`

 * *Files identical despite different names*

