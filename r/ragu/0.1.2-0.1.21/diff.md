# Comparing `tmp/ragu-0.1.2.tar.gz` & `tmp/ragu-0.1.21.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ragu-0.1.2.tar", last modified: Sat Jul  8 14:27:47 2023, max compression
+gzip compressed data, was "ragu-0.1.21.tar", last modified: Sat Jul  8 16:21:40 2023, max compression
```

## Comparing `ragu-0.1.2.tar` & `ragu-0.1.21.tar`

### file list

```diff
@@ -1,57 +1,65 @@
-drwxr-xr-x   0 btober     (501) staff       (20)        0 2023-07-08 14:27:47.767211 ragu-0.1.2/
--rw-r--r--   0 btober     (501) staff       (20)    35149 2023-07-08 00:09:50.000000 ragu-0.1.2/LICENSE.txt
--rw-r--r--   0 btober     (501) staff       (20)    46800 2023-07-08 14:27:47.767075 ragu-0.1.2/PKG-INFO
--rw-r--r--   0 btober     (501) staff       (20)     5827 2023-07-08 14:26:19.000000 ragu-0.1.2/README.md
--rw-r--r--   0 btober     (501) staff       (20)     1194 2023-07-08 14:26:06.000000 ragu-0.1.2/pyproject.toml
--rw-r--r--   0 btober     (501) staff       (20)       38 2023-07-08 14:27:47.767253 ragu-0.1.2/setup.cfg
--rw-r--r--   0 btober     (501) staff       (20)       91 2023-07-08 14:00:18.000000 ragu-0.1.2/setup.py
-drwxr-xr-x   0 btober     (501) staff       (20)        0 2023-07-08 14:27:47.758719 ragu-0.1.2/src/
-drwxr-xr-x   0 btober     (501) staff       (20)        0 2023-07-08 14:27:47.760189 ragu-0.1.2/src/ragu/
--rw-r--r--   0 btober     (501) staff       (20)        0 2023-07-08 00:09:51.000000 ragu-0.1.2/src/ragu/__init__.py
-drwxr-xr-x   0 btober     (501) staff       (20)        0 2023-07-08 14:27:47.761342 ragu-0.1.2/src/ragu/bin/
--rw-r--r--   0 btober     (501) staff       (20)     1988 2023-07-08 14:00:14.000000 ragu-0.1.2/src/ragu/bin/ragu.py
--rw-r--r--   0 btober     (501) staff       (20)     1993 2023-07-08 00:09:51.000000 ragu-0.1.2/src/ragu/config.py
-drwxr-xr-x   0 btober     (501) staff       (20)        0 2023-07-08 14:27:47.763622 ragu-0.1.2/src/ragu/ingest/
--rw-r--r--   0 btober     (501) staff       (20)     5753 2023-07-08 00:09:51.000000 ragu-0.1.2/src/ragu/ingest/__init__.py
--rw-r--r--   0 btober     (501) staff       (20)     2344 2023-07-08 00:09:51.000000 ragu-0.1.2/src/ragu/ingest/ingest_cresis_rds.py
--rw-r--r--   0 btober     (501) staff       (20)     2387 2023-07-08 00:09:51.000000 ragu-0.1.2/src/ragu/ingest/ingest_cresis_snow.py
--rw-r--r--   0 btober     (501) staff       (20)     2935 2023-07-08 00:09:51.000000 ragu-0.1.2/src/ragu/ingest/ingest_groundhog.py
--rw-r--r--   0 btober     (501) staff       (20)     3299 2023-07-08 00:09:51.000000 ragu-0.1.2/src/ragu/ingest/ingest_gssi.py
--rw-r--r--   0 btober     (501) staff       (20)     2495 2023-07-08 00:09:51.000000 ragu-0.1.2/src/ragu/ingest/ingest_lrs.py
--rw-r--r--   0 btober     (501) staff       (20)     2829 2023-07-08 00:09:51.000000 ragu-0.1.2/src/ragu/ingest/ingest_marsis.py
--rw-r--r--   0 btober     (501) staff       (20)     2407 2023-07-08 00:09:51.000000 ragu-0.1.2/src/ragu/ingest/ingest_marsis_ipc.py
--rw-r--r--   0 btober     (501) staff       (20)     5713 2023-07-08 00:09:51.000000 ragu-0.1.2/src/ragu/ingest/ingest_oibAK.py
--rw-r--r--   0 btober     (501) staff       (20)    14114 2023-07-08 00:09:51.000000 ragu-0.1.2/src/ragu/ingest/ingest_pulseekko.py
--rw-r--r--   0 btober     (501) staff       (20)     2470 2023-07-08 00:09:51.000000 ragu-0.1.2/src/ragu/ingest/ingest_rimfax.py
--rw-r--r--   0 btober     (501) staff       (20)     2864 2023-07-08 00:09:51.000000 ragu-0.1.2/src/ragu/ingest/ingest_sharad.py
--rw-r--r--   0 btober     (501) staff       (20)     3573 2023-07-08 00:09:51.000000 ragu-0.1.2/src/ragu/ingest/ingest_template.py
--rw-r--r--   0 btober     (501) staff       (20)     2444 2023-07-08 00:09:51.000000 ragu-0.1.2/src/ragu/ingest/ingest_uaf_kentech.py
-drwxr-xr-x   0 btober     (501) staff       (20)        0 2023-07-08 14:27:47.764040 ragu-0.1.2/src/ragu/nav/
--rw-r--r--   0 btober     (501) staff       (20)      153 2023-07-08 00:09:51.000000 ragu-0.1.2/src/ragu/nav/__init__.py
--rw-r--r--   0 btober     (501) staff       (20)     5086 2023-07-08 00:09:51.000000 ragu-0.1.2/src/ragu/nav/gps.py
--rw-r--r--   0 btober     (501) staff       (20)    20723 2023-07-08 00:09:51.000000 ragu-0.1.2/src/ragu/nav/navparse.py
-drwxr-xr-x   0 btober     (501) staff       (20)        0 2023-07-08 14:27:47.764704 ragu-0.1.2/src/ragu/radar/
--rw-r--r--   0 btober     (501) staff       (20)     7537 2023-07-08 00:09:51.000000 ragu-0.1.2/src/ragu/radar/__init__.py
--rw-r--r--   0 btober     (501) staff       (20)      505 2023-07-08 00:09:51.000000 ragu-0.1.2/src/ragu/radar/flags.py
--rw-r--r--   0 btober     (501) staff       (20)     1185 2023-07-08 00:09:51.000000 ragu-0.1.2/src/ragu/radar/pick.py
--rw-r--r--   0 btober     (501) staff       (20)    11495 2023-07-08 00:09:51.000000 ragu-0.1.2/src/ragu/radar/processing.py
--rw-r--r--   0 btober     (501) staff       (20)      225 2023-07-08 00:09:51.000000 ragu-0.1.2/src/ragu/raguError.py
-drwxr-xr-x   0 btober     (501) staff       (20)        0 2023-07-08 14:27:47.765418 ragu-0.1.2/src/ragu/tools/
--rw-r--r--   0 btober     (501) staff       (20)      152 2023-07-08 00:09:51.000000 ragu-0.1.2/src/ragu/tools/__init__.py
--rw-r--r--   0 btober     (501) staff       (20)      481 2023-07-08 00:09:51.000000 ragu-0.1.2/src/ragu/tools/constants.py
--rw-r--r--   0 btober     (501) staff       (20)     9427 2023-07-08 00:09:51.000000 ragu-0.1.2/src/ragu/tools/export.py
--rw-r--r--   0 btober     (501) staff       (20)     9845 2023-07-08 00:09:51.000000 ragu-0.1.2/src/ragu/tools/utils.py
-drwxr-xr-x   0 btober     (501) staff       (20)        0 2023-07-08 14:27:47.766749 ragu-0.1.2/src/ragu/ui/
--rw-r--r--   0 btober     (501) staff       (20)      152 2023-07-08 00:09:51.000000 ragu-0.1.2/src/ragu/ui/__init__.py
--rw-r--r--   0 btober     (501) staff       (20)    16554 2023-07-08 00:09:51.000000 ragu-0.1.2/src/ragu/ui/basemap.py
--rw-r--r--   0 btober     (501) staff       (20)    68357 2023-07-08 00:09:51.000000 ragu-0.1.2/src/ragu/ui/gui.py
--rw-r--r--   0 btober     (501) staff       (20)    70973 2023-07-08 00:09:51.000000 ragu-0.1.2/src/ragu/ui/impick.py
--rw-r--r--   0 btober     (501) staff       (20)    10803 2023-07-08 00:09:51.000000 ragu-0.1.2/src/ragu/ui/notepad.py
--rw-r--r--   0 btober     (501) staff       (20)    23544 2023-07-08 00:09:51.000000 ragu-0.1.2/src/ragu/ui/wvpick.py
-drwxr-xr-x   0 btober     (501) staff       (20)        0 2023-07-08 14:27:47.761214 ragu-0.1.2/src/ragu.egg-info/
--rw-r--r--   0 btober     (501) staff       (20)    46800 2023-07-08 14:27:47.000000 ragu-0.1.2/src/ragu.egg-info/PKG-INFO
--rw-r--r--   0 btober     (501) staff       (20)     1209 2023-07-08 14:27:47.000000 ragu-0.1.2/src/ragu.egg-info/SOURCES.txt
--rw-r--r--   0 btober     (501) staff       (20)        1 2023-07-08 14:27:47.000000 ragu-0.1.2/src/ragu.egg-info/dependency_links.txt
--rw-r--r--   0 btober     (501) staff       (20)       44 2023-07-08 14:27:47.000000 ragu-0.1.2/src/ragu.egg-info/entry_points.txt
--rw-r--r--   0 btober     (501) staff       (20)       64 2023-07-08 14:27:47.000000 ragu-0.1.2/src/ragu.egg-info/requires.txt
--rw-r--r--   0 btober     (501) staff       (20)       19 2023-07-08 14:27:47.000000 ragu-0.1.2/src/ragu.egg-info/top_level.txt
+drwxr-xr-x   0 btober     (501) staff       (20)        0 2023-07-08 16:21:40.486413 ragu-0.1.21/
+-rw-r--r--   0 btober     (501) staff       (20)    35149 2023-07-08 00:09:50.000000 ragu-0.1.21/LICENSE.txt
+-rw-r--r--   0 btober     (501) staff       (20)    46836 2023-07-08 16:21:40.486268 ragu-0.1.21/PKG-INFO
+-rw-r--r--   0 btober     (501) staff       (20)     5862 2023-07-08 14:36:05.000000 ragu-0.1.21/README.md
+-rw-r--r--   0 btober     (501) staff       (20)     1018 2023-07-08 16:21:15.000000 ragu-0.1.21/pyproject.toml
+-rw-r--r--   0 btober     (501) staff       (20)       38 2023-07-08 16:21:40.486449 ragu-0.1.21/setup.cfg
+-rw-r--r--   0 btober     (501) staff       (20)       91 2023-07-08 14:00:18.000000 ragu-0.1.21/setup.py
+drwxr-xr-x   0 btober     (501) staff       (20)        0 2023-07-08 16:21:40.462648 ragu-0.1.21/src/
+drwxr-xr-x   0 btober     (501) staff       (20)        0 2023-07-08 16:21:40.463993 ragu-0.1.21/src/ragu/
+-rw-r--r--   0 btober     (501) staff       (20)        0 2023-07-08 00:09:51.000000 ragu-0.1.21/src/ragu/__init__.py
+drwxr-xr-x   0 btober     (501) staff       (20)        0 2023-07-08 16:21:40.464883 ragu-0.1.21/src/ragu/bin/
+-rw-r--r--   0 btober     (501) staff       (20)     1988 2023-07-08 14:00:14.000000 ragu-0.1.21/src/ragu/bin/ragu.py
+-rw-r--r--   0 btober     (501) staff       (20)     1993 2023-07-08 00:09:51.000000 ragu-0.1.21/src/ragu/config.py
+drwxr-xr-x   0 btober     (501) staff       (20)        0 2023-07-08 16:21:40.462824 ragu-0.1.21/src/ragu/dat/
+drwxr-xr-x   0 btober     (501) staff       (20)        0 2023-07-08 16:21:40.465008 ragu-0.1.21/src/ragu/dat/mars/
+-rw-r--r--   0 btober     (501) staff       (20) 33196562 2023-07-08 00:09:51.000000 ragu-0.1.21/src/ragu/dat/mars/mega90n000eb.tif
+drwxr-xr-x   0 btober     (501) staff       (20)        0 2023-07-08 16:21:40.482584 ragu-0.1.21/src/ragu/ingest/
+-rw-r--r--   0 btober     (501) staff       (20)     5753 2023-07-08 00:09:51.000000 ragu-0.1.21/src/ragu/ingest/__init__.py
+-rw-r--r--   0 btober     (501) staff       (20)     2344 2023-07-08 00:09:51.000000 ragu-0.1.21/src/ragu/ingest/ingest_cresis_rds.py
+-rw-r--r--   0 btober     (501) staff       (20)     2387 2023-07-08 00:09:51.000000 ragu-0.1.21/src/ragu/ingest/ingest_cresis_snow.py
+-rw-r--r--   0 btober     (501) staff       (20)     2935 2023-07-08 00:09:51.000000 ragu-0.1.21/src/ragu/ingest/ingest_groundhog.py
+-rw-r--r--   0 btober     (501) staff       (20)     3299 2023-07-08 00:09:51.000000 ragu-0.1.21/src/ragu/ingest/ingest_gssi.py
+-rw-r--r--   0 btober     (501) staff       (20)     2495 2023-07-08 00:09:51.000000 ragu-0.1.21/src/ragu/ingest/ingest_lrs.py
+-rw-r--r--   0 btober     (501) staff       (20)     2829 2023-07-08 00:09:51.000000 ragu-0.1.21/src/ragu/ingest/ingest_marsis.py
+-rw-r--r--   0 btober     (501) staff       (20)     2407 2023-07-08 00:09:51.000000 ragu-0.1.21/src/ragu/ingest/ingest_marsis_ipc.py
+-rw-r--r--   0 btober     (501) staff       (20)     5713 2023-07-08 00:09:51.000000 ragu-0.1.21/src/ragu/ingest/ingest_oibAK.py
+-rw-r--r--   0 btober     (501) staff       (20)    14114 2023-07-08 00:09:51.000000 ragu-0.1.21/src/ragu/ingest/ingest_pulseekko.py
+-rw-r--r--   0 btober     (501) staff       (20)     2470 2023-07-08 00:09:51.000000 ragu-0.1.21/src/ragu/ingest/ingest_rimfax.py
+-rw-r--r--   0 btober     (501) staff       (20)     2864 2023-07-08 00:09:51.000000 ragu-0.1.21/src/ragu/ingest/ingest_sharad.py
+-rw-r--r--   0 btober     (501) staff       (20)     3573 2023-07-08 00:09:51.000000 ragu-0.1.21/src/ragu/ingest/ingest_template.py
+-rw-r--r--   0 btober     (501) staff       (20)     2444 2023-07-08 00:09:51.000000 ragu-0.1.21/src/ragu/ingest/ingest_uaf_kentech.py
+drwxr-xr-x   0 btober     (501) staff       (20)        0 2023-07-08 16:21:40.482973 ragu-0.1.21/src/ragu/nav/
+-rw-r--r--   0 btober     (501) staff       (20)      153 2023-07-08 00:09:51.000000 ragu-0.1.21/src/ragu/nav/__init__.py
+-rw-r--r--   0 btober     (501) staff       (20)     5086 2023-07-08 00:09:51.000000 ragu-0.1.21/src/ragu/nav/gps.py
+-rw-r--r--   0 btober     (501) staff       (20)    20721 2023-07-08 16:18:44.000000 ragu-0.1.21/src/ragu/nav/navparse.py
+drwxr-xr-x   0 btober     (501) staff       (20)        0 2023-07-08 16:21:40.483553 ragu-0.1.21/src/ragu/radar/
+-rw-r--r--   0 btober     (501) staff       (20)     7537 2023-07-08 00:09:51.000000 ragu-0.1.21/src/ragu/radar/__init__.py
+-rw-r--r--   0 btober     (501) staff       (20)      505 2023-07-08 00:09:51.000000 ragu-0.1.21/src/ragu/radar/flags.py
+-rw-r--r--   0 btober     (501) staff       (20)     1185 2023-07-08 00:09:51.000000 ragu-0.1.21/src/ragu/radar/pick.py
+-rw-r--r--   0 btober     (501) staff       (20)    11495 2023-07-08 00:09:51.000000 ragu-0.1.21/src/ragu/radar/processing.py
+-rw-r--r--   0 btober     (501) staff       (20)      225 2023-07-08 00:09:51.000000 ragu-0.1.21/src/ragu/raguError.py
+drwxr-xr-x   0 btober     (501) staff       (20)        0 2023-07-08 16:21:40.484623 ragu-0.1.21/src/ragu/recs/
+-rw-r--r--   0 btober     (501) staff       (20)  1079564 2023-07-08 00:09:51.000000 ragu-0.1.21/src/ragu/recs/20190928-235534_compiled.jpg
+-rw-r--r--   0 btober     (501) staff       (20)    16176 2023-07-08 00:09:51.000000 ragu-0.1.21/src/ragu/recs/basemap_icon.png
+-rw-r--r--   0 btober     (501) staff       (20)    92542 2023-07-08 00:09:51.000000 ragu-0.1.21/src/ragu/recs/bulb.jpg
+-rw-r--r--   0 btober     (501) staff       (20)    21590 2023-07-08 00:09:51.000000 ragu-0.1.21/src/ragu/recs/ragu_logo.png
+drwxr-xr-x   0 btober     (501) staff       (20)        0 2023-07-08 16:21:40.485133 ragu-0.1.21/src/ragu/tools/
+-rw-r--r--   0 btober     (501) staff       (20)      152 2023-07-08 00:09:51.000000 ragu-0.1.21/src/ragu/tools/__init__.py
+-rw-r--r--   0 btober     (501) staff       (20)      481 2023-07-08 00:09:51.000000 ragu-0.1.21/src/ragu/tools/constants.py
+-rw-r--r--   0 btober     (501) staff       (20)     9427 2023-07-08 00:09:51.000000 ragu-0.1.21/src/ragu/tools/export.py
+-rw-r--r--   0 btober     (501) staff       (20)     9845 2023-07-08 00:09:51.000000 ragu-0.1.21/src/ragu/tools/utils.py
+drwxr-xr-x   0 btober     (501) staff       (20)        0 2023-07-08 16:21:40.486016 ragu-0.1.21/src/ragu/ui/
+-rw-r--r--   0 btober     (501) staff       (20)      152 2023-07-08 00:09:51.000000 ragu-0.1.21/src/ragu/ui/__init__.py
+-rw-r--r--   0 btober     (501) staff       (20)    16552 2023-07-08 16:18:38.000000 ragu-0.1.21/src/ragu/ui/basemap.py
+-rw-r--r--   0 btober     (501) staff       (20)    68357 2023-07-08 00:09:51.000000 ragu-0.1.21/src/ragu/ui/gui.py
+-rw-r--r--   0 btober     (501) staff       (20)    70973 2023-07-08 00:09:51.000000 ragu-0.1.21/src/ragu/ui/impick.py
+-rw-r--r--   0 btober     (501) staff       (20)    10803 2023-07-08 00:09:51.000000 ragu-0.1.21/src/ragu/ui/notepad.py
+-rw-r--r--   0 btober     (501) staff       (20)    23544 2023-07-08 00:09:51.000000 ragu-0.1.21/src/ragu/ui/wvpick.py
+drwxr-xr-x   0 btober     (501) staff       (20)        0 2023-07-08 16:21:40.464767 ragu-0.1.21/src/ragu.egg-info/
+-rw-r--r--   0 btober     (501) staff       (20)    46836 2023-07-08 16:21:40.000000 ragu-0.1.21/src/ragu.egg-info/PKG-INFO
+-rw-r--r--   0 btober     (501) staff       (20)     1369 2023-07-08 16:21:40.000000 ragu-0.1.21/src/ragu.egg-info/SOURCES.txt
+-rw-r--r--   0 btober     (501) staff       (20)        1 2023-07-08 16:21:40.000000 ragu-0.1.21/src/ragu.egg-info/dependency_links.txt
+-rw-r--r--   0 btober     (501) staff       (20)       44 2023-07-08 16:21:40.000000 ragu-0.1.21/src/ragu.egg-info/entry_points.txt
+-rw-r--r--   0 btober     (501) staff       (20)       64 2023-07-08 16:21:40.000000 ragu-0.1.21/src/ragu.egg-info/requires.txt
+-rw-r--r--   0 btober     (501) staff       (20)       10 2023-07-08 16:21:40.000000 ragu-0.1.21/src/ragu.egg-info/top_level.txt
```

### Comparing `ragu-0.1.2/LICENSE.txt` & `ragu-0.1.21/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ragu-0.1.2/PKG-INFO` & `ragu-0.1.21/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ragu
-Version: 0.1.2
+Version: 0.1.21
 Summary: Radar Analysis Graphical Utility (RAGU)
 Author: Brandon S. Tober
 Author-email: tobers.brandon@gmail.com
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
@@ -771,15 +771,16 @@
 - pyproj
 - rasterio
 - h5py
 
 ### Setup
 **Nonte: Prior to installation, one may first wish to create an anaconda environment from which to install ragu**.
 
-1. Install ragu via pypa
+1. Install ragu via [PyPi](https://pypi.org/project/ragu/)
+
 ```
 $ pip install ragu
 ```
 
 2. To run ragu, call ragu from the command line to initialize the GUI:
 ```
 $ ragu
```

### Comparing `ragu-0.1.2/README.md` & `ragu-0.1.21/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -83,15 +83,16 @@
 - pyproj
 - rasterio
 - h5py
 
 ### Setup
 **Nonte: Prior to installation, one may first wish to create an anaconda environment from which to install ragu**.
 
-1. Install ragu via pypa
+1. Install ragu via [PyPi](https://pypi.org/project/ragu/)
+
 ```
 $ pip install ragu
 ```
 
 2. To run ragu, call ragu from the command line to initialize the GUI:
 ```
 $ ragu
```

### Comparing `ragu-0.1.2/pyproject.toml` & `ragu-0.1.21/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ragu"
-version = "0.1.2"
+version = "0.1.21"
 description = "Radar Analysis Graphical Utility (RAGU)"
 readme = "README.md"
 requires-python = ">=3.6"
 license = {file = "LICENSE.txt"}
 authors = [
     {name = "Brandon S. Tober"},
     {email = "tobers.brandon@gmail.com"}
@@ -29,25 +29,18 @@
 repository = "https://github.com/btobers/ragu"
 
 # The following would provide a command line executable called `sample`
 # which executes the function `main` from this package when invoked.
 [project.scripts]
 ragu = "ragu.bin.ragu:main"
 
-[tool.setuptools]
-include-package-data = true
-
 [tool.setuptools.packages.find]
 namespaces = true
 where = ["src"]
 
-
-# [tool.setuptools]
-# packages = ["src"]
-# include-package-data = true
-# package-data = ["mega90n000eb.tif", "mega90n000eb.lbl", "*.png", "*.jpg", "*.pdf"]
-# [tool.setuptools.package-data]
-# mypkg = ["*.txt", "*.rst"]
+[tool.setuptools.package-data]
+"ragu.recs" = ["*.png", "*.jpg"]
+"ragu.dat" = ["*/*.tif"]
 
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
```

### Comparing `ragu-0.1.2/src/ragu/bin/ragu.py` & `ragu-0.1.21/src/ragu/bin/ragu.py`

 * *Files identical despite different names*

### Comparing `ragu-0.1.2/src/ragu/config.py` & `ragu-0.1.21/src/ragu/config.py`

 * *Files identical despite different names*

### Comparing `ragu-0.1.2/src/ragu/ingest/__init__.py` & `ragu-0.1.21/src/ragu/ingest/__init__.py`

 * *Files identical despite different names*

### Comparing `ragu-0.1.2/src/ragu/ingest/ingest_cresis_rds.py` & `ragu-0.1.21/src/ragu/ingest/ingest_cresis_rds.py`

 * *Files identical despite different names*

### Comparing `ragu-0.1.2/src/ragu/ingest/ingest_cresis_snow.py` & `ragu-0.1.21/src/ragu/ingest/ingest_cresis_snow.py`

 * *Files identical despite different names*

### Comparing `ragu-0.1.2/src/ragu/ingest/ingest_groundhog.py` & `ragu-0.1.21/src/ragu/ingest/ingest_groundhog.py`

 * *Files identical despite different names*

### Comparing `ragu-0.1.2/src/ragu/ingest/ingest_gssi.py` & `ragu-0.1.21/src/ragu/ingest/ingest_gssi.py`

 * *Files identical despite different names*

### Comparing `ragu-0.1.2/src/ragu/ingest/ingest_lrs.py` & `ragu-0.1.21/src/ragu/ingest/ingest_lrs.py`

 * *Files identical despite different names*

### Comparing `ragu-0.1.2/src/ragu/ingest/ingest_marsis.py` & `ragu-0.1.21/src/ragu/ingest/ingest_marsis.py`

 * *Files identical despite different names*

### Comparing `ragu-0.1.2/src/ragu/ingest/ingest_marsis_ipc.py` & `ragu-0.1.21/src/ragu/ingest/ingest_marsis_ipc.py`

 * *Files identical despite different names*

### Comparing `ragu-0.1.2/src/ragu/ingest/ingest_oibAK.py` & `ragu-0.1.21/src/ragu/ingest/ingest_oibAK.py`

 * *Files identical despite different names*

### Comparing `ragu-0.1.2/src/ragu/ingest/ingest_pulseekko.py` & `ragu-0.1.21/src/ragu/ingest/ingest_pulseekko.py`

 * *Files identical despite different names*

### Comparing `ragu-0.1.2/src/ragu/ingest/ingest_rimfax.py` & `ragu-0.1.21/src/ragu/ingest/ingest_rimfax.py`

 * *Files identical despite different names*

### Comparing `ragu-0.1.2/src/ragu/ingest/ingest_sharad.py` & `ragu-0.1.21/src/ragu/ingest/ingest_sharad.py`

 * *Files identical despite different names*

### Comparing `ragu-0.1.2/src/ragu/ingest/ingest_template.py` & `ragu-0.1.21/src/ragu/ingest/ingest_template.py`

 * *Files identical despite different names*

### Comparing `ragu-0.1.2/src/ragu/ingest/ingest_uaf_kentech.py` & `ragu-0.1.21/src/ragu/ingest/ingest_uaf_kentech.py`

 * *Files identical despite different names*

### Comparing `ragu-0.1.2/src/ragu/nav/gps.py` & `ragu-0.1.21/src/ragu/nav/gps.py`

 * *Files identical despite different names*

### Comparing `ragu-0.1.2/src/ragu/nav/navparse.py` & `ragu-0.1.21/src/ragu/nav/navparse.py`

 * *Files 0% similar despite different names*

```diff
@@ -430,15 +430,15 @@
     df["dist"] = euclid_dist(
         df["x"].to_numpy(),
         df["y"].to_numpy(),
         df["z"].to_numpy())
 
     # SHARAD FPB sample 1800 corresponds to the areoid height - use areoid to reference elevation and get absolute twtt - aeroid height in meters after subtracting 3396000 m
     # aerPath = os.path.split(os.getcwd())[0] + "/dat/mars/mega90n000eb.tif"
-    aerPath = os.path.join(os.path.dirname(__file__), '../../dat/mars', 'mega90n000eb.tif')
+    aerPath = os.path.join(os.path.dirname(__file__), '/../dat/mars', 'mega90n000eb.tif')
     try:
         aer = rio.open(aerPath, mode="r")
 
     except:
         print("Unable to open areoid file. Is it located at : " + aerPath + " ?")
         sys.exit(1)
```

### Comparing `ragu-0.1.2/src/ragu/radar/__init__.py` & `ragu-0.1.21/src/ragu/radar/__init__.py`

 * *Files identical despite different names*

### Comparing `ragu-0.1.2/src/ragu/radar/pick.py` & `ragu-0.1.21/src/ragu/radar/pick.py`

 * *Files identical despite different names*

### Comparing `ragu-0.1.2/src/ragu/radar/processing.py` & `ragu-0.1.21/src/ragu/radar/processing.py`

 * *Files identical despite different names*

### Comparing `ragu-0.1.2/src/ragu/tools/export.py` & `ragu-0.1.21/src/ragu/tools/export.py`

 * *Files identical despite different names*

### Comparing `ragu-0.1.2/src/ragu/tools/utils.py` & `ragu-0.1.21/src/ragu/tools/utils.py`

 * *Files identical despite different names*

### Comparing `ragu-0.1.2/src/ragu/ui/basemap.py` & `ragu-0.1.21/src/ragu/ui/basemap.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
         self.parent = parent
         self.datPath = datPath
         self.navcrs = navcrs
         self.body = body
         self.to_gui = to_gui
         # create tkinter toplevel window to display basemap
         self.basemap_window = tk.Toplevel(self.parent)
-        img = tk.PhotoImage(file=os.path.join(os.path.dirname(__file__), "../../recs", "basemap_icon.png"))
+        img = tk.PhotoImage(file=os.path.join(os.path.dirname(__file__), "/../recs", "basemap_icon.png"))
         self.basemap_window.tk.call("wm", "iconphoto", self.basemap_window._w, img)
         self.basemap_window.config(bg="#d9d9d9")
         self.basemap_window.title("RAGU - Map Window")
         self.map_display = tk.Frame(self.basemap_window)
         self.map_display.pack(side="bottom", fill="both", expand=1)
         # bind ctrl-q key to basemap_close()
         self.basemap_window.bind("<Control-q>", self.basemap_close)
```

### Comparing `ragu-0.1.2/src/ragu/ui/gui.py` & `ragu-0.1.21/src/ragu/ui/gui.py`

 * *Files identical despite different names*

### Comparing `ragu-0.1.2/src/ragu/ui/impick.py` & `ragu-0.1.21/src/ragu/ui/impick.py`

 * *Files identical despite different names*

### Comparing `ragu-0.1.2/src/ragu/ui/notepad.py` & `ragu-0.1.21/src/ragu/ui/notepad.py`

 * *Files identical despite different names*

### Comparing `ragu-0.1.2/src/ragu/ui/wvpick.py` & `ragu-0.1.21/src/ragu/ui/wvpick.py`

 * *Files identical despite different names*

### Comparing `ragu-0.1.2/src/ragu.egg-info/PKG-INFO` & `ragu-0.1.21/src/ragu.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ragu
-Version: 0.1.2
+Version: 0.1.21
 Summary: Radar Analysis Graphical Utility (RAGU)
 Author: Brandon S. Tober
 Author-email: tobers.brandon@gmail.com
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
@@ -771,15 +771,16 @@
 - pyproj
 - rasterio
 - h5py
 
 ### Setup
 **Nonte: Prior to installation, one may first wish to create an anaconda environment from which to install ragu**.
 
-1. Install ragu via pypa
+1. Install ragu via [PyPi](https://pypi.org/project/ragu/)
+
 ```
 $ pip install ragu
 ```
 
 2. To run ragu, call ragu from the command line to initialize the GUI:
 ```
 $ ragu
```

