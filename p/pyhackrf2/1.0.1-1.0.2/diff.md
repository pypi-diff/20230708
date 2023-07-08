# Comparing `tmp/pyhackrf2-1.0.1.tar.gz` & `tmp/pyhackrf2-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyhackrf2-1.0.1.tar", last modified: Sun Jun 25 13:45:00 2023, max compression
+gzip compressed data, was "pyhackrf2-1.0.2.tar", last modified: Sat Jul  8 19:43:31 2023, max compression
```

## Comparing `pyhackrf2-1.0.1.tar` & `pyhackrf2-1.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-06-25 13:45:00.319141 pyhackrf2-1.0.1/
--rw-r--r--   0 alex       (501) staff       (20)     4131 2023-06-25 13:45:00.318980 pyhackrf2-1.0.1/PKG-INFO
--rw-r--r--   0 alex       (501) staff       (20)     3820 2023-06-25 13:42:40.000000 pyhackrf2-1.0.1/README.md
--rw-r--r--   0 alex       (501) staff       (20)      401 2023-06-25 13:44:17.000000 pyhackrf2-1.0.1/pyproject.toml
--rw-r--r--   0 alex       (501) staff       (20)       38 2023-06-25 13:45:00.319189 pyhackrf2-1.0.1/setup.cfg
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-06-25 13:45:00.316708 pyhackrf2-1.0.1/src/
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-06-25 13:45:00.317829 pyhackrf2-1.0.1/src/pyhackrf/
--rw-r--r--   0 alex       (501) staff       (20)        0 2023-05-27 23:45:06.000000 pyhackrf2-1.0.1/src/pyhackrf/__init__.py
--rw-r--r--   0 alex       (501) staff       (20)     5017 2023-05-29 21:31:56.000000 pyhackrf2-1.0.1/src/pyhackrf/cinterface.py
--rw-r--r--   0 alex       (501) staff       (20)    18071 2023-05-29 22:26:21.000000 pyhackrf2-1.0.1/src/pyhackrf/libhackrf.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-06-25 13:45:00.318763 pyhackrf2-1.0.1/src/pyhackrf2.egg-info/
--rw-r--r--   0 alex       (501) staff       (20)     4131 2023-06-25 13:45:00.000000 pyhackrf2-1.0.1/src/pyhackrf2.egg-info/PKG-INFO
--rw-r--r--   0 alex       (501) staff       (20)      250 2023-06-25 13:45:00.000000 pyhackrf2-1.0.1/src/pyhackrf2.egg-info/SOURCES.txt
--rw-r--r--   0 alex       (501) staff       (20)        1 2023-06-25 13:45:00.000000 pyhackrf2-1.0.1/src/pyhackrf2.egg-info/dependency_links.txt
--rw-r--r--   0 alex       (501) staff       (20)        9 2023-06-25 13:45:00.000000 pyhackrf2-1.0.1/src/pyhackrf2.egg-info/top_level.txt
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-07-08 19:43:31.130037 pyhackrf2-1.0.2/
+-rw-r--r--   0 alex       (501) staff       (20)     4627 2023-07-08 19:43:31.129677 pyhackrf2-1.0.2/PKG-INFO
+-rw-r--r--   0 alex       (501) staff       (20)     4316 2023-07-08 19:27:39.000000 pyhackrf2-1.0.2/README.md
+-rw-r--r--   0 alex       (501) staff       (20)      434 2023-07-08 19:28:42.000000 pyhackrf2-1.0.2/pyproject.toml
+-rw-r--r--   0 alex       (501) staff       (20)       38 2023-07-08 19:43:31.130101 pyhackrf2-1.0.2/setup.cfg
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-07-08 19:43:31.126776 pyhackrf2-1.0.2/src/
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-07-08 19:43:31.127605 pyhackrf2-1.0.2/src/pyhackrf2/
+-rw-r--r--   0 alex       (501) staff       (20)    18072 2023-07-08 19:05:33.000000 pyhackrf2-1.0.2/src/pyhackrf2/__init__.py
+-rw-r--r--   0 alex       (501) staff       (20)     5017 2023-05-29 21:31:56.000000 pyhackrf2-1.0.2/src/pyhackrf2/cinterface.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-07-08 19:43:31.128973 pyhackrf2-1.0.2/src/pyhackrf2.egg-info/
+-rw-r--r--   0 alex       (501) staff       (20)     4627 2023-07-08 19:43:31.000000 pyhackrf2-1.0.2/src/pyhackrf2.egg-info/PKG-INFO
+-rw-r--r--   0 alex       (501) staff       (20)      262 2023-07-08 19:43:31.000000 pyhackrf2-1.0.2/src/pyhackrf2.egg-info/SOURCES.txt
+-rw-r--r--   0 alex       (501) staff       (20)        1 2023-07-08 19:43:31.000000 pyhackrf2-1.0.2/src/pyhackrf2.egg-info/dependency_links.txt
+-rw-r--r--   0 alex       (501) staff       (20)       12 2023-07-08 19:43:31.000000 pyhackrf2-1.0.2/src/pyhackrf2.egg-info/requires.txt
+-rw-r--r--   0 alex       (501) staff       (20)       10 2023-07-08 19:43:31.000000 pyhackrf2-1.0.2/src/pyhackrf2.egg-info/top_level.txt
```

### Comparing `pyhackrf2-1.0.1/PKG-INFO` & `pyhackrf2-1.0.2/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,7 @@
-Metadata-Version: 2.1
-Name: pyhackrf2
-Version: 1.0.1
-Summary: Python bindings for libhackrf rewritten
-Classifier: Topic :: Communications :: Ham Radio
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3
-Description-Content-Type: text/markdown
-
 # pyhackrf2
 
 A Python wrappper for libhackrf rewritten.
 
 # Description
 
 Python bindings for native HackRF library libhackrf that aims to implement all features of HackRF accessible via its C interface, but via convenient Pythonic class.
@@ -171,9 +161,20 @@
 hackrf.lna_gain = 8
 hackrf.vga_gain = 22
 
 hackrf.txvga_gain = 40
 
 ```
 
+### Mac M1 users
 
+At the moment, libhackrf is not avalable with arm architecture. If you get message like, the following:
+```
+OSError: dlopen(libhackrf.so.0, 0x0006): ... '/usr/local/lib/libhackrf.so.0' (mach-o file, but is an incompatible architecture (have 'x86_64', need 'arm64')), ...
+```
 
+You need to install using
+```
+arch -x86_64 python -m venv venv
+arch -x86_64 pip install pyhackrf2
+```
+This will fetch x86_64 version of numpy, and will be compatible with libhackrf.so.0 as x86_64 binary.
```

### Comparing `pyhackrf2-1.0.1/src/pyhackrf/cinterface.py` & `pyhackrf2-1.0.2/src/pyhackrf2/cinterface.py`

 * *Files identical despite different names*

### Comparing `pyhackrf2-1.0.1/src/pyhackrf/libhackrf.py` & `pyhackrf2-1.0.2/src/pyhackrf2/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from ctypes import *
 import numpy as np
 from collections.abc import Callable
-from cinterface import (
+from .cinterface import (
     libhackrf,
     p_hackrf_device,
     TransceiverMode,
     lib_hackrf_transfer,
     lib_read_partid_serialno_t,
     ERRORS,
     BASEBAND_FILTER_VALID_VALUES,
```

### Comparing `pyhackrf2-1.0.1/src/pyhackrf2.egg-info/PKG-INFO` & `pyhackrf2-1.0.2/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhackrf2
-Version: 1.0.1
+Version: 1.0.2
 Summary: Python bindings for libhackrf rewritten
 Classifier: Topic :: Communications :: Ham Radio
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 
@@ -171,9 +171,20 @@
 hackrf.lna_gain = 8
 hackrf.vga_gain = 22
 
 hackrf.txvga_gain = 40
 
 ```
 
+### Mac M1 users
 
+At the moment, libhackrf is not avalable with arm architecture. If you get message like, the following:
+```
+OSError: dlopen(libhackrf.so.0, 0x0006): ... '/usr/local/lib/libhackrf.so.0' (mach-o file, but is an incompatible architecture (have 'x86_64', need 'arm64')), ...
+```
 
+You need to install using
+```
+arch -x86_64 python -m venv venv
+arch -x86_64 pip install pyhackrf2
+```
+This will fetch x86_64 version of numpy, and will be compatible with libhackrf.so.0 as x86_64 binary.
```

