# Comparing `tmp/Final2x-core-1.0.0.tar.gz` & `tmp/Final2x-core-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Final2x-core-1.0.0.tar", last modified: Wed Jul  5 07:50:00 2023, max compression
+gzip compressed data, was "Final2x-core-1.0.1.tar", last modified: Sat Jul  8 03:06:40 2023, max compression
```

## Comparing `Final2x-core-1.0.0.tar` & `Final2x-core-1.0.1.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 07:50:00.787943 Final2x-core-1.0.0/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 07:50:00.783943 Final2x-core-1.0.0/Final2x_core/
--rw-r--r--   0 runner    (1001) docker     (122)       49 2023-07-05 07:49:29.000000 Final2x-core-1.0.0/Final2x_core/Final2x-core-pip.md
--rw-r--r--   0 runner    (1001) docker     (122)       28 2023-07-05 07:49:59.000000 Final2x-core-1.0.0/Final2x_core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2758 2023-07-05 07:49:59.000000 Final2x-core-1.0.0/Final2x_core/__main__.py
--rw-r--r--   0 runner    (1001) docker     (122)      778 2023-07-05 07:49:59.000000 Final2x-core-1.0.0/Final2x_core/config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 07:50:00.787943 Final2x-core-1.0.0/Final2x_core/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 07:50:00.787943 Final2x-core-1.0.0/Final2x_core/src/SRFactory/
--rw-r--r--   0 runner    (1001) docker     (122)     2535 2023-07-05 07:49:59.000000 Final2x-core-1.0.0/Final2x_core/src/SRFactory/REALCUGAN.py
--rw-r--r--   0 runner    (1001) docker     (122)     2522 2023-07-05 07:49:59.000000 Final2x-core-1.0.0/Final2x_core/src/SRFactory/REALESRGAN.py
--rw-r--r--   0 runner    (1001) docker     (122)     3491 2023-07-05 07:49:59.000000 Final2x-core-1.0.0/Final2x_core/src/SRFactory/SRBaseClass.py
--rw-r--r--   0 runner    (1001) docker     (122)     1982 2023-07-05 07:49:59.000000 Final2x-core-1.0.0/Final2x_core/src/SRFactory/SRFactory.py
--rw-r--r--   0 runner    (1001) docker     (122)     1365 2023-07-05 07:49:59.000000 Final2x-core-1.0.0/Final2x_core/src/SRFactory/SRMD.py
--rw-r--r--   0 runner    (1001) docker     (122)     2898 2023-07-05 07:49:59.000000 Final2x-core-1.0.0/Final2x_core/src/SRFactory/WAIFU2X.py
--rw-r--r--   0 runner    (1001) docker     (122)      645 2023-07-05 07:49:59.000000 Final2x-core-1.0.0/Final2x_core/src/SRFactory/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 07:50:00.787943 Final2x-core-1.0.0/Final2x_core/src/SRncnn/
--rw-r--r--   0 runner    (1001) docker     (122)     1787 2023-07-05 07:49:59.000000 Final2x-core-1.0.0/Final2x_core/src/SRncnn/REALCUGANncnn.py
--rw-r--r--   0 runner    (1001) docker     (122)     2219 2023-07-05 07:49:59.000000 Final2x-core-1.0.0/Final2x_core/src/SRncnn/REALESRGANncnn.py
--rw-r--r--   0 runner    (1001) docker     (122)     1146 2023-07-05 07:49:59.000000 Final2x-core-1.0.0/Final2x_core/src/SRncnn/SRMDncnn.py
--rw-r--r--   0 runner    (1001) docker     (122)     1414 2023-07-05 07:49:59.000000 Final2x-core-1.0.0/Final2x_core/src/SRncnn/WAIFU2Xncnn.py
--rw-r--r--   0 runner    (1001) docker     (122)     2535 2023-07-05 07:49:59.000000 Final2x-core-1.0.0/Final2x_core/src/SRqueue.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 07:50:00.787943 Final2x-core-1.0.0/Final2x_core/src/utils/
--rw-r--r--   0 runner    (1001) docker     (122)     5330 2023-07-05 07:49:59.000000 Final2x-core-1.0.0/Final2x_core/src/utils/getConfig.py
--rw-r--r--   0 runner    (1001) docker     (122)     1062 2023-07-05 07:49:59.000000 Final2x-core-1.0.0/Final2x_core/src/utils/progressLog.py
--rw-r--r--   0 runner    (1001) docker     (122)      421 2023-07-05 07:49:59.000000 Final2x-core-1.0.0/Final2x_core/src/utils/singleton.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 07:50:00.783943 Final2x-core-1.0.0/Final2x_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     7099 2023-07-05 07:50:00.000000 Final2x-core-1.0.0/Final2x_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      935 2023-07-05 07:50:00.000000 Final2x-core-1.0.0/Final2x_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-05 07:50:00.000000 Final2x-core-1.0.0/Final2x_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       61 2023-07-05 07:50:00.000000 Final2x-core-1.0.0/Final2x_core.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)      128 2023-07-05 07:50:00.000000 Final2x-core-1.0.0/Final2x_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)      104 2023-07-05 07:50:00.000000 Final2x-core-1.0.0/Final2x_core.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1493 2023-07-05 07:49:29.000000 Final2x-core-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)       32 2023-07-05 07:49:29.000000 Final2x-core-1.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     7099 2023-07-05 07:50:00.787943 Final2x-core-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     6393 2023-07-05 07:49:29.000000 Final2x-core-1.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-05 07:50:00.787943 Final2x-core-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1593 2023-07-05 07:49:30.000000 Final2x-core-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-08 03:06:40.817253 Final2x-core-1.0.1/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-08 03:06:40.813253 Final2x-core-1.0.1/Final2x_core/
+-rw-r--r--   0 runner    (1001) docker     (122)       49 2023-07-08 03:06:16.000000 Final2x-core-1.0.1/Final2x_core/Final2x-core-pip.md
+-rw-r--r--   0 runner    (1001) docker     (122)       28 2023-07-08 03:06:39.000000 Final2x-core-1.0.1/Final2x_core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2862 2023-07-08 03:06:39.000000 Final2x-core-1.0.1/Final2x_core/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      778 2023-07-08 03:06:39.000000 Final2x-core-1.0.1/Final2x_core/config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-08 03:06:40.813253 Final2x-core-1.0.1/Final2x_core/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-08 03:06:40.817253 Final2x-core-1.0.1/Final2x_core/src/SRFactory/
+-rw-r--r--   0 runner    (1001) docker     (122)     2535 2023-07-08 03:06:39.000000 Final2x-core-1.0.1/Final2x_core/src/SRFactory/REALCUGAN.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2522 2023-07-08 03:06:39.000000 Final2x-core-1.0.1/Final2x_core/src/SRFactory/REALESRGAN.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3491 2023-07-08 03:06:39.000000 Final2x-core-1.0.1/Final2x_core/src/SRFactory/SRBaseClass.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1982 2023-07-08 03:06:39.000000 Final2x-core-1.0.1/Final2x_core/src/SRFactory/SRFactory.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1365 2023-07-08 03:06:39.000000 Final2x-core-1.0.1/Final2x_core/src/SRFactory/SRMD.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2898 2023-07-08 03:06:39.000000 Final2x-core-1.0.1/Final2x_core/src/SRFactory/WAIFU2X.py
+-rw-r--r--   0 runner    (1001) docker     (122)      645 2023-07-08 03:06:39.000000 Final2x-core-1.0.1/Final2x_core/src/SRFactory/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-08 03:06:40.817253 Final2x-core-1.0.1/Final2x_core/src/SRncnn/
+-rw-r--r--   0 runner    (1001) docker     (122)     1787 2023-07-08 03:06:39.000000 Final2x-core-1.0.1/Final2x_core/src/SRncnn/REALCUGANncnn.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2219 2023-07-08 03:06:39.000000 Final2x-core-1.0.1/Final2x_core/src/SRncnn/REALESRGANncnn.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1146 2023-07-08 03:06:39.000000 Final2x-core-1.0.1/Final2x_core/src/SRncnn/SRMDncnn.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1414 2023-07-08 03:06:39.000000 Final2x-core-1.0.1/Final2x_core/src/SRncnn/WAIFU2Xncnn.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2535 2023-07-08 03:06:39.000000 Final2x-core-1.0.1/Final2x_core/src/SRqueue.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-08 03:06:40.817253 Final2x-core-1.0.1/Final2x_core/src/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)     5330 2023-07-08 03:06:39.000000 Final2x-core-1.0.1/Final2x_core/src/utils/getConfig.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1062 2023-07-08 03:06:39.000000 Final2x-core-1.0.1/Final2x_core/src/utils/progressLog.py
+-rw-r--r--   0 runner    (1001) docker     (122)      421 2023-07-08 03:06:39.000000 Final2x-core-1.0.1/Final2x_core/src/utils/singleton.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-08 03:06:40.813253 Final2x-core-1.0.1/Final2x_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     7240 2023-07-08 03:06:40.000000 Final2x-core-1.0.1/Final2x_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      935 2023-07-08 03:06:40.000000 Final2x-core-1.0.1/Final2x_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-08 03:06:40.000000 Final2x-core-1.0.1/Final2x_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       61 2023-07-08 03:06:40.000000 Final2x-core-1.0.1/Final2x_core.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      128 2023-07-08 03:06:40.000000 Final2x-core-1.0.1/Final2x_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      104 2023-07-08 03:06:40.000000 Final2x-core-1.0.1/Final2x_core.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     1493 2023-07-08 03:06:16.000000 Final2x-core-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       32 2023-07-08 03:06:16.000000 Final2x-core-1.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     7240 2023-07-08 03:06:40.817253 Final2x-core-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     6534 2023-07-08 03:06:16.000000 Final2x-core-1.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-08 03:06:40.817253 Final2x-core-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1593 2023-07-08 03:06:17.000000 Final2x-core-1.0.1/setup.py
```

### Comparing `Final2x-core-1.0.0/Final2x_core/__main__.py` & `Final2x-core-1.0.1/Final2x_core/__main__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 import argparse
 import os
 import sys
 from pathlib import Path
-
-import cv2
 from loguru import logger
 
 try:
     from src.SRqueue import SR_queue
     from src.utils.getConfig import SRCONFIG
 except ImportError:
     # for pip cli
@@ -25,14 +23,15 @@
 
 # parse args
 parser = argparse.ArgumentParser()
 parser.description = "when para is not specified, the config.yaml file in the directory will be read automatically"
 parser.add_argument("-b", "--BASE64", help="base64 string for config json", type=str)
 parser.add_argument("-j", "--JSON", help="JSON string for config", type=str)
 parser.add_argument("-y", "--YAML", help="yaml config file path", type=str)
+parser.add_argument("-l", "--LOG", help="save log", action="store_true")
 parser.add_argument("-o", "--OP", help="check install", action="store_true")
 args = parser.parse_args()
 
 if args.OP:
     print("114514")
     exit(0)
 
@@ -49,15 +48,17 @@
             logger.error("cannot open output folder")
     except Exception as e:
         logger.error(e)
         logger.error("cannot open output folder")
 
 
 def main():
-    logger.add(projectPATH / "logs" / "log-{time}.log", encoding="utf-8", retention="60 days")
+    if args.LOG:
+        # init logger
+        logger.add(projectPATH / "logs" / "log-{time}.log", encoding="utf-8", retention="60 days")
     logger.info("projectPATH: " + str(projectPATH))
 
     # load config
     config = SRCONFIG()
     if args.BASE64 is not None:
         config.getConfigfromBase64toJson(str(args.BASE64), str(projectPATH / "models"))
     elif args.JSON is not None:
```

### Comparing `Final2x-core-1.0.0/Final2x_core/config.yaml` & `Final2x-core-1.0.1/Final2x_core/config.yaml`

 * *Files identical despite different names*

### Comparing `Final2x-core-1.0.0/Final2x_core/src/SRFactory/REALCUGAN.py` & `Final2x-core-1.0.1/Final2x_core/src/SRFactory/REALCUGAN.py`

 * *Files identical despite different names*

### Comparing `Final2x-core-1.0.0/Final2x_core/src/SRFactory/REALESRGAN.py` & `Final2x-core-1.0.1/Final2x_core/src/SRFactory/REALESRGAN.py`

 * *Files identical despite different names*

### Comparing `Final2x-core-1.0.0/Final2x_core/src/SRFactory/SRBaseClass.py` & `Final2x-core-1.0.1/Final2x_core/src/SRFactory/SRBaseClass.py`

 * *Files identical despite different names*

### Comparing `Final2x-core-1.0.0/Final2x_core/src/SRFactory/SRFactory.py` & `Final2x-core-1.0.1/Final2x_core/src/SRFactory/SRFactory.py`

 * *Files identical despite different names*

### Comparing `Final2x-core-1.0.0/Final2x_core/src/SRFactory/SRMD.py` & `Final2x-core-1.0.1/Final2x_core/src/SRFactory/SRMD.py`

 * *Files identical despite different names*

### Comparing `Final2x-core-1.0.0/Final2x_core/src/SRFactory/WAIFU2X.py` & `Final2x-core-1.0.1/Final2x_core/src/SRFactory/WAIFU2X.py`

 * *Files identical despite different names*

### Comparing `Final2x-core-1.0.0/Final2x_core/src/SRFactory/__init__.py` & `Final2x-core-1.0.1/Final2x_core/src/SRFactory/__init__.py`

 * *Files identical despite different names*

### Comparing `Final2x-core-1.0.0/Final2x_core/src/SRncnn/REALCUGANncnn.py` & `Final2x-core-1.0.1/Final2x_core/src/SRncnn/REALCUGANncnn.py`

 * *Files identical despite different names*

### Comparing `Final2x-core-1.0.0/Final2x_core/src/SRncnn/REALESRGANncnn.py` & `Final2x-core-1.0.1/Final2x_core/src/SRncnn/REALESRGANncnn.py`

 * *Files identical despite different names*

### Comparing `Final2x-core-1.0.0/Final2x_core/src/SRncnn/SRMDncnn.py` & `Final2x-core-1.0.1/Final2x_core/src/SRncnn/SRMDncnn.py`

 * *Files identical despite different names*

### Comparing `Final2x-core-1.0.0/Final2x_core/src/SRncnn/WAIFU2Xncnn.py` & `Final2x-core-1.0.1/Final2x_core/src/SRncnn/WAIFU2Xncnn.py`

 * *Files identical despite different names*

### Comparing `Final2x-core-1.0.0/Final2x_core/src/SRqueue.py` & `Final2x-core-1.0.1/Final2x_core/src/SRqueue.py`

 * *Files identical despite different names*

### Comparing `Final2x-core-1.0.0/Final2x_core/src/utils/getConfig.py` & `Final2x-core-1.0.1/Final2x_core/src/utils/getConfig.py`

 * *Files identical despite different names*

### Comparing `Final2x-core-1.0.0/Final2x_core/src/utils/progressLog.py` & `Final2x-core-1.0.1/Final2x_core/src/utils/progressLog.py`

 * *Files identical despite different names*

### Comparing `Final2x-core-1.0.0/Final2x_core.egg-info/PKG-INFO` & `Final2x-core-1.0.1/Final2x_core.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Final2x-core
-Version: 1.0.0
+Version: 1.0.1
 Summary: UNKNOWN
 Home-page: https://github.com/Tohrusky/Final2x-core
 Author: Tohrusky
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -37,15 +37,15 @@
 [![CI-build](https://github.com/Tohrusky/Final2x-core/actions/workflows/CI-build.yml/badge.svg)](https://github.com/Tohrusky/Final2x-core/actions/workflows/CI-build.yml)
 [![Release](https://github.com/Tohrusky/Final2x-core/actions/workflows/Release.yml/badge.svg)](https://github.com/Tohrusky/Final2x-core/actions/workflows/Release.yml)
 [![PIP-test](https://github.com/Tohrusky/Final2x-core/actions/workflows/PIP-test.yml/badge.svg)](https://github.com/Tohrusky/Final2x-core/actions/workflows/PIP-test.yml)
 [![Release-pypi](https://github.com/Tohrusky/Final2x-core/actions/workflows/Release-pypi.yml/badge.svg)](https://github.com/Tohrusky/Final2x-core/actions/workflows/Release-pypi.yml)
 [![PyPI version](https://badge.fury.io/py/Final2x-core.svg)](https://badge.fury.io/py/Final2x-core)
 ![GitHub](https://img.shields.io/github/license/Tohrusky/Final2x-core)
 
-Final2x-core is a cross-platform image super-resolution CLI tool for [Final2x](https://github.com/Tohrusky/Final2x).
+Final2x-core is a cross-platform image super-resolution CLI tool for [Final2x](https://github.com/Tohrusky/Final2x). If you have any questions, please raise an issue [in this repository](https://github.com/Tohrusky/Final2x).
 
 # Install
 
 Download in [Release](https://github.com/Tohrusky/Final2x-core/releases) or use pip (python >= 3.6, >=3.9 for MacOS
 arm64)
 
 ```shell
@@ -61,14 +61,15 @@
 
 optional arguments:
   -h, --help            show this help message and exit
   -b BASE64, --BASE64 BASE64
                         base64 string for config json
   -j JSON, --JSON JSON  JSON string for config
   -y YAML, --YAML YAML  yaml config file path
+  -l, --LOG             save log
   -o, --OP              check install
 ```
 
 # Config
 
 Pass the config json string to the program through the `-j` parameter.
```

### Comparing `Final2x-core-1.0.0/Final2x_core.egg-info/SOURCES.txt` & `Final2x-core-1.0.1/Final2x_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Final2x-core-1.0.0/LICENSE` & `Final2x-core-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `Final2x-core-1.0.0/PKG-INFO` & `Final2x-core-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Final2x-core
-Version: 1.0.0
+Version: 1.0.1
 Summary: UNKNOWN
 Home-page: https://github.com/Tohrusky/Final2x-core
 Author: Tohrusky
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -37,15 +37,15 @@
 [![CI-build](https://github.com/Tohrusky/Final2x-core/actions/workflows/CI-build.yml/badge.svg)](https://github.com/Tohrusky/Final2x-core/actions/workflows/CI-build.yml)
 [![Release](https://github.com/Tohrusky/Final2x-core/actions/workflows/Release.yml/badge.svg)](https://github.com/Tohrusky/Final2x-core/actions/workflows/Release.yml)
 [![PIP-test](https://github.com/Tohrusky/Final2x-core/actions/workflows/PIP-test.yml/badge.svg)](https://github.com/Tohrusky/Final2x-core/actions/workflows/PIP-test.yml)
 [![Release-pypi](https://github.com/Tohrusky/Final2x-core/actions/workflows/Release-pypi.yml/badge.svg)](https://github.com/Tohrusky/Final2x-core/actions/workflows/Release-pypi.yml)
 [![PyPI version](https://badge.fury.io/py/Final2x-core.svg)](https://badge.fury.io/py/Final2x-core)
 ![GitHub](https://img.shields.io/github/license/Tohrusky/Final2x-core)
 
-Final2x-core is a cross-platform image super-resolution CLI tool for [Final2x](https://github.com/Tohrusky/Final2x).
+Final2x-core is a cross-platform image super-resolution CLI tool for [Final2x](https://github.com/Tohrusky/Final2x). If you have any questions, please raise an issue [in this repository](https://github.com/Tohrusky/Final2x).
 
 # Install
 
 Download in [Release](https://github.com/Tohrusky/Final2x-core/releases) or use pip (python >= 3.6, >=3.9 for MacOS
 arm64)
 
 ```shell
@@ -61,14 +61,15 @@
 
 optional arguments:
   -h, --help            show this help message and exit
   -b BASE64, --BASE64 BASE64
                         base64 string for config json
   -j JSON, --JSON JSON  JSON string for config
   -y YAML, --YAML YAML  yaml config file path
+  -l, --LOG             save log
   -o, --OP              check install
 ```
 
 # Config
 
 Pass the config json string to the program through the `-j` parameter.
```

### Comparing `Final2x-core-1.0.0/README.md` & `Final2x-core-1.0.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 [![CI-build](https://github.com/Tohrusky/Final2x-core/actions/workflows/CI-build.yml/badge.svg)](https://github.com/Tohrusky/Final2x-core/actions/workflows/CI-build.yml)
 [![Release](https://github.com/Tohrusky/Final2x-core/actions/workflows/Release.yml/badge.svg)](https://github.com/Tohrusky/Final2x-core/actions/workflows/Release.yml)
 [![PIP-test](https://github.com/Tohrusky/Final2x-core/actions/workflows/PIP-test.yml/badge.svg)](https://github.com/Tohrusky/Final2x-core/actions/workflows/PIP-test.yml)
 [![Release-pypi](https://github.com/Tohrusky/Final2x-core/actions/workflows/Release-pypi.yml/badge.svg)](https://github.com/Tohrusky/Final2x-core/actions/workflows/Release-pypi.yml)
 [![PyPI version](https://badge.fury.io/py/Final2x-core.svg)](https://badge.fury.io/py/Final2x-core)
 ![GitHub](https://img.shields.io/github/license/Tohrusky/Final2x-core)
 
-Final2x-core is a cross-platform image super-resolution CLI tool for [Final2x](https://github.com/Tohrusky/Final2x).
+Final2x-core is a cross-platform image super-resolution CLI tool for [Final2x](https://github.com/Tohrusky/Final2x). If you have any questions, please raise an issue [in this repository](https://github.com/Tohrusky/Final2x).
 
 # Install
 
 Download in [Release](https://github.com/Tohrusky/Final2x-core/releases) or use pip (python >= 3.6, >=3.9 for MacOS
 arm64)
 
 ```shell
@@ -40,14 +40,15 @@
 
 optional arguments:
   -h, --help            show this help message and exit
   -b BASE64, --BASE64 BASE64
                         base64 string for config json
   -j JSON, --JSON JSON  JSON string for config
   -y YAML, --YAML YAML  yaml config file path
+  -l, --LOG             save log
   -o, --OP              check install
 ```
 
 # Config
 
 Pass the config json string to the program through the `-j` parameter.
```

### Comparing `Final2x-core-1.0.0/setup.py` & `Final2x-core-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 
 from setuptools import setup
 
-_version: str = "1.0.0"
+_version: str = "1.0.1"
 
 
 def My_find_packages(*tops):
     packages = []
     for d in tops:
         for root, dirs, files in os.walk(d, followlinks=True):
             packages.append(root)
```

