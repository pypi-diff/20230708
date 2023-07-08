# Comparing `tmp/reliableGPT-0.2.979.tar.gz` & `tmp/reliableGPT-0.2.980.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reliableGPT-0.2.979.tar", last modified: Sat Jul  8 02:54:43 2023, max compression
+gzip compressed data, was "reliableGPT-0.2.980.tar", last modified: Sat Jul  8 03:24:07 2023, max compression
```

## Comparing `reliableGPT-0.2.979.tar` & `reliableGPT-0.2.980.tar`

### file list

```diff
@@ -1,24 +1,20 @@
-drwxr-xr-x   0 krrishdholakia   (501) staff       (20)        0 2023-07-08 02:54:43.861895 reliableGPT-0.2.979/
--rw-r--r--   0 krrishdholakia   (501) staff       (20)     1065 2023-06-23 13:49:22.000000 reliableGPT-0.2.979/LICENSE
--rw-r--r--   0 krrishdholakia   (501) staff       (20)      156 2023-07-08 02:54:43.861778 reliableGPT-0.2.979/PKG-INFO
--rw-r--r--   0 krrishdholakia   (501) staff       (20)     8377 2023-07-08 02:45:37.000000 reliableGPT-0.2.979/README.md
--rw-r--r--   0 krrishdholakia   (501) staff       (20)      497 2023-06-29 02:51:34.000000 reliableGPT-0.2.979/pyproject.toml
-drwxr-xr-x   0 krrishdholakia   (501) staff       (20)        0 2023-07-08 02:54:43.858989 reliableGPT-0.2.979/reliableGPT.egg-info/
--rw-r--r--   0 krrishdholakia   (501) staff       (20)      156 2023-07-08 02:54:43.000000 reliableGPT-0.2.979/reliableGPT.egg-info/PKG-INFO
--rw-r--r--   0 krrishdholakia   (501) staff       (20)      514 2023-07-08 02:54:43.000000 reliableGPT-0.2.979/reliableGPT.egg-info/SOURCES.txt
--rw-r--r--   0 krrishdholakia   (501) staff       (20)        1 2023-07-08 02:54:43.000000 reliableGPT-0.2.979/reliableGPT.egg-info/dependency_links.txt
--rw-r--r--   0 krrishdholakia   (501) staff       (20)       63 2023-07-08 02:54:43.000000 reliableGPT-0.2.979/reliableGPT.egg-info/requires.txt
--rw-r--r--   0 krrishdholakia   (501) staff       (20)       12 2023-07-08 02:54:43.000000 reliableGPT-0.2.979/reliableGPT.egg-info/top_level.txt
-drwxr-xr-x   0 krrishdholakia   (501) staff       (20)        0 2023-07-08 02:54:43.861467 reliableGPT-0.2.979/reliablegpt/
--rw-r--r--   0 krrishdholakia   (501) staff       (20)     4210 2023-06-29 02:51:34.000000 reliableGPT-0.2.979/reliablegpt/APICallHandler.py
--rw-r--r--   0 krrishdholakia   (501) staff       (20)     3149 2023-07-07 02:48:09.000000 reliableGPT-0.2.979/reliablegpt/Alerting.py
--rw-r--r--   0 krrishdholakia   (501) staff       (20)     4407 2023-06-29 02:51:34.000000 reliableGPT-0.2.979/reliablegpt/CustomQueue.py
--rw-r--r--   0 krrishdholakia   (501) staff       (20)    18415 2023-07-08 02:52:42.000000 reliableGPT-0.2.979/reliablegpt/IndividualRequest.py
--rw-r--r--   0 krrishdholakia   (501) staff       (20)     1286 2023-07-01 20:41:40.000000 reliableGPT-0.2.979/reliablegpt/Model.py
--rw-r--r--   0 krrishdholakia   (501) staff       (20)     5170 2023-07-03 15:14:41.000000 reliableGPT-0.2.979/reliablegpt/RateLimitHandler.py
--rw-r--r--   0 krrishdholakia   (501) staff       (20)     7483 2023-07-06 13:49:42.000000 reliableGPT-0.2.979/reliablegpt/ReliableDataLoaders.py
--rw-r--r--   0 krrishdholakia   (501) staff       (20)      375 2023-07-06 17:39:33.000000 reliableGPT-0.2.979/reliablegpt/__init__.py
--rw-r--r--   0 krrishdholakia   (501) staff       (20)     5233 2023-07-08 02:45:37.000000 reliableGPT-0.2.979/reliablegpt/main.py
--rw-r--r--   0 krrishdholakia   (501) staff       (20)     2363 2023-07-03 15:14:41.000000 reliableGPT-0.2.979/reliablegpt/reliableQuery.py
--rw-r--r--   0 krrishdholakia   (501) staff       (20)       38 2023-07-08 02:54:43.861951 reliableGPT-0.2.979/setup.cfg
--rw-r--r--   0 krrishdholakia   (501) staff       (20)      418 2023-07-08 02:54:35.000000 reliableGPT-0.2.979/setup.py
+drwxr-xr-x   0 krrishdholakia   (501) staff       (20)        0 2023-07-08 03:24:07.177889 reliableGPT-0.2.980/
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)     1065 2023-06-23 13:49:22.000000 reliableGPT-0.2.980/LICENSE
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)      156 2023-07-08 03:24:07.177775 reliableGPT-0.2.980/PKG-INFO
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)     8377 2023-07-08 02:45:37.000000 reliableGPT-0.2.980/README.md
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)      497 2023-06-29 02:51:34.000000 reliableGPT-0.2.980/pyproject.toml
+drwxr-xr-x   0 krrishdholakia   (501) staff       (20)        0 2023-07-08 03:24:07.176364 reliableGPT-0.2.980/reliableGPT.egg-info/
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)      156 2023-07-08 03:24:07.000000 reliableGPT-0.2.980/reliableGPT.egg-info/PKG-INFO
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)      366 2023-07-08 03:24:07.000000 reliableGPT-0.2.980/reliableGPT.egg-info/SOURCES.txt
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)        1 2023-07-08 03:24:07.000000 reliableGPT-0.2.980/reliableGPT.egg-info/dependency_links.txt
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)       63 2023-07-08 03:24:07.000000 reliableGPT-0.2.980/reliableGPT.egg-info/requires.txt
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)       12 2023-07-08 03:24:07.000000 reliableGPT-0.2.980/reliableGPT.egg-info/top_level.txt
+drwxr-xr-x   0 krrishdholakia   (501) staff       (20)        0 2023-07-08 03:24:07.177585 reliableGPT-0.2.980/reliablegpt/
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)     3149 2023-07-07 02:48:09.000000 reliableGPT-0.2.980/reliablegpt/Alerting.py
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)    18415 2023-07-08 02:52:42.000000 reliableGPT-0.2.980/reliablegpt/IndividualRequest.py
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)     1286 2023-07-01 20:41:40.000000 reliableGPT-0.2.980/reliablegpt/Model.py
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)       58 2023-07-08 03:07:22.000000 reliableGPT-0.2.980/reliablegpt/__init__.py
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)     5175 2023-07-08 03:08:08.000000 reliableGPT-0.2.980/reliablegpt/main.py
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)     2363 2023-07-03 15:14:41.000000 reliableGPT-0.2.980/reliablegpt/reliableQuery.py
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)       38 2023-07-08 03:24:07.177975 reliableGPT-0.2.980/setup.cfg
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)      418 2023-07-08 03:23:39.000000 reliableGPT-0.2.980/setup.py
```

### Comparing `reliableGPT-0.2.979/LICENSE` & `reliableGPT-0.2.980/LICENSE`

 * *Files identical despite different names*

### Comparing `reliableGPT-0.2.979/README.md` & `reliableGPT-0.2.980/README.md`

 * *Files identical despite different names*

### Comparing `reliableGPT-0.2.979/reliablegpt/Alerting.py` & `reliableGPT-0.2.980/reliablegpt/Alerting.py`

 * *Files identical despite different names*

### Comparing `reliableGPT-0.2.979/reliablegpt/IndividualRequest.py` & `reliableGPT-0.2.980/reliablegpt/IndividualRequest.py`

 * *Files identical despite different names*

### Comparing `reliableGPT-0.2.979/reliablegpt/Model.py` & `reliableGPT-0.2.980/reliablegpt/Model.py`

 * *Files identical despite different names*

### Comparing `reliableGPT-0.2.979/reliablegpt/main.py` & `reliableGPT-0.2.980/reliablegpt/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 # # Prod Imports
 from reliablegpt.IndividualRequest import IndividualRequest
-from reliablegpt.RateLimitHandler import RateLimitHandler
 from reliablegpt.Model import Model
 from reliablegpt.Alerting import Alerting
 from reliablegpt.reliableQuery import reliable_query
 import requests
 
 # # Dev Imports
 # from IndividualRequest import IndividualRequest
```

### Comparing `reliableGPT-0.2.979/reliablegpt/reliableQuery.py` & `reliableGPT-0.2.980/reliablegpt/reliableQuery.py`

 * *Files identical despite different names*

