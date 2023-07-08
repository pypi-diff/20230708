# Comparing `tmp/reliableGPT-0.2.980.tar.gz` & `tmp/reliableGPT-0.2.981.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reliableGPT-0.2.980.tar", last modified: Sat Jul  8 03:24:07 2023, max compression
+gzip compressed data, was "reliableGPT-0.2.981.tar", last modified: Sat Jul  8 03:29:31 2023, max compression
```

## Comparing `reliableGPT-0.2.980.tar` & `reliableGPT-0.2.981.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 krrishdholakia   (501) staff       (20)        0 2023-07-08 03:24:07.177889 reliableGPT-0.2.980/
--rw-r--r--   0 krrishdholakia   (501) staff       (20)     1065 2023-06-23 13:49:22.000000 reliableGPT-0.2.980/LICENSE
--rw-r--r--   0 krrishdholakia   (501) staff       (20)      156 2023-07-08 03:24:07.177775 reliableGPT-0.2.980/PKG-INFO
--rw-r--r--   0 krrishdholakia   (501) staff       (20)     8377 2023-07-08 02:45:37.000000 reliableGPT-0.2.980/README.md
--rw-r--r--   0 krrishdholakia   (501) staff       (20)      497 2023-06-29 02:51:34.000000 reliableGPT-0.2.980/pyproject.toml
-drwxr-xr-x   0 krrishdholakia   (501) staff       (20)        0 2023-07-08 03:24:07.176364 reliableGPT-0.2.980/reliableGPT.egg-info/
--rw-r--r--   0 krrishdholakia   (501) staff       (20)      156 2023-07-08 03:24:07.000000 reliableGPT-0.2.980/reliableGPT.egg-info/PKG-INFO
--rw-r--r--   0 krrishdholakia   (501) staff       (20)      366 2023-07-08 03:24:07.000000 reliableGPT-0.2.980/reliableGPT.egg-info/SOURCES.txt
--rw-r--r--   0 krrishdholakia   (501) staff       (20)        1 2023-07-08 03:24:07.000000 reliableGPT-0.2.980/reliableGPT.egg-info/dependency_links.txt
--rw-r--r--   0 krrishdholakia   (501) staff       (20)       63 2023-07-08 03:24:07.000000 reliableGPT-0.2.980/reliableGPT.egg-info/requires.txt
--rw-r--r--   0 krrishdholakia   (501) staff       (20)       12 2023-07-08 03:24:07.000000 reliableGPT-0.2.980/reliableGPT.egg-info/top_level.txt
-drwxr-xr-x   0 krrishdholakia   (501) staff       (20)        0 2023-07-08 03:24:07.177585 reliableGPT-0.2.980/reliablegpt/
--rw-r--r--   0 krrishdholakia   (501) staff       (20)     3149 2023-07-07 02:48:09.000000 reliableGPT-0.2.980/reliablegpt/Alerting.py
--rw-r--r--   0 krrishdholakia   (501) staff       (20)    18415 2023-07-08 02:52:42.000000 reliableGPT-0.2.980/reliablegpt/IndividualRequest.py
--rw-r--r--   0 krrishdholakia   (501) staff       (20)     1286 2023-07-01 20:41:40.000000 reliableGPT-0.2.980/reliablegpt/Model.py
--rw-r--r--   0 krrishdholakia   (501) staff       (20)       58 2023-07-08 03:07:22.000000 reliableGPT-0.2.980/reliablegpt/__init__.py
--rw-r--r--   0 krrishdholakia   (501) staff       (20)     5175 2023-07-08 03:08:08.000000 reliableGPT-0.2.980/reliablegpt/main.py
--rw-r--r--   0 krrishdholakia   (501) staff       (20)     2363 2023-07-03 15:14:41.000000 reliableGPT-0.2.980/reliablegpt/reliableQuery.py
--rw-r--r--   0 krrishdholakia   (501) staff       (20)       38 2023-07-08 03:24:07.177975 reliableGPT-0.2.980/setup.cfg
--rw-r--r--   0 krrishdholakia   (501) staff       (20)      418 2023-07-08 03:23:39.000000 reliableGPT-0.2.980/setup.py
+drwxr-xr-x   0 krrishdholakia   (501) staff       (20)        0 2023-07-08 03:29:31.329740 reliableGPT-0.2.981/
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)     1065 2023-06-23 13:49:22.000000 reliableGPT-0.2.981/LICENSE
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)      156 2023-07-08 03:29:31.329597 reliableGPT-0.2.981/PKG-INFO
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)     8377 2023-07-08 02:45:37.000000 reliableGPT-0.2.981/README.md
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)      497 2023-06-29 02:51:34.000000 reliableGPT-0.2.981/pyproject.toml
+drwxr-xr-x   0 krrishdholakia   (501) staff       (20)        0 2023-07-08 03:29:31.328010 reliableGPT-0.2.981/reliableGPT.egg-info/
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)      156 2023-07-08 03:29:31.000000 reliableGPT-0.2.981/reliableGPT.egg-info/PKG-INFO
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)      366 2023-07-08 03:29:31.000000 reliableGPT-0.2.981/reliableGPT.egg-info/SOURCES.txt
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)        1 2023-07-08 03:29:31.000000 reliableGPT-0.2.981/reliableGPT.egg-info/dependency_links.txt
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)       63 2023-07-08 03:29:31.000000 reliableGPT-0.2.981/reliableGPT.egg-info/requires.txt
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)       12 2023-07-08 03:29:31.000000 reliableGPT-0.2.981/reliableGPT.egg-info/top_level.txt
+drwxr-xr-x   0 krrishdholakia   (501) staff       (20)        0 2023-07-08 03:29:31.329391 reliableGPT-0.2.981/reliablegpt/
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)     3149 2023-07-07 02:48:09.000000 reliableGPT-0.2.981/reliablegpt/Alerting.py
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)    18415 2023-07-08 02:52:42.000000 reliableGPT-0.2.981/reliablegpt/IndividualRequest.py
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)     1286 2023-07-01 20:41:40.000000 reliableGPT-0.2.981/reliablegpt/Model.py
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)       58 2023-07-08 03:07:22.000000 reliableGPT-0.2.981/reliablegpt/__init__.py
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)     5208 2023-07-08 03:25:36.000000 reliableGPT-0.2.981/reliablegpt/main.py
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)     2363 2023-07-03 15:14:41.000000 reliableGPT-0.2.981/reliablegpt/reliableQuery.py
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)       38 2023-07-08 03:29:31.329808 reliableGPT-0.2.981/setup.cfg
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)      418 2023-07-08 03:29:10.000000 reliableGPT-0.2.981/setup.py
```

### Comparing `reliableGPT-0.2.980/LICENSE` & `reliableGPT-0.2.981/LICENSE`

 * *Files identical despite different names*

### Comparing `reliableGPT-0.2.980/README.md` & `reliableGPT-0.2.981/README.md`

 * *Files identical despite different names*

### Comparing `reliableGPT-0.2.980/reliablegpt/Alerting.py` & `reliableGPT-0.2.981/reliablegpt/Alerting.py`

 * *Files identical despite different names*

### Comparing `reliableGPT-0.2.980/reliablegpt/IndividualRequest.py` & `reliableGPT-0.2.981/reliablegpt/IndividualRequest.py`

 * *Files identical despite different names*

### Comparing `reliableGPT-0.2.980/reliablegpt/Model.py` & `reliableGPT-0.2.981/reliablegpt/Model.py`

 * *Files identical despite different names*

### Comparing `reliableGPT-0.2.980/reliablegpt/main.py` & `reliableGPT-0.2.981/reliablegpt/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 
 # # Dev Imports
 # from IndividualRequest import IndividualRequest
 # from Model import Model
 # from Alerting import Alerting
 
 from posthog import Posthog
+from flask import Flask, request
 
 posthog = Posthog(
   project_api_key='phc_yZ30KsPzRXd3nYaET3VFDmquFKtMZwMTuFKVOei6viB',
   host='https://app.posthog.com')
 
 alerting = Alerting()
```

### Comparing `reliableGPT-0.2.980/reliablegpt/reliableQuery.py` & `reliableGPT-0.2.981/reliablegpt/reliableQuery.py`

 * *Files identical despite different names*

