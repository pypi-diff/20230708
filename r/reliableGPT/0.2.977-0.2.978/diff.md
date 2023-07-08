# Comparing `tmp/reliableGPT-0.2.977.tar.gz` & `tmp/reliableGPT-0.2.978.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reliableGPT-0.2.977.tar", last modified: Sat Jul  8 02:51:01 2023, max compression
+gzip compressed data, was "reliableGPT-0.2.978.tar", last modified: Sat Jul  8 02:53:14 2023, max compression
```

## Comparing `reliableGPT-0.2.977.tar` & `reliableGPT-0.2.978.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 krrishdholakia   (501) staff       (20)        0 2023-07-08 02:51:01.757357 reliableGPT-0.2.977/
--rw-r--r--   0 krrishdholakia   (501) staff       (20)     1065 2023-06-23 13:49:22.000000 reliableGPT-0.2.977/LICENSE
--rw-r--r--   0 krrishdholakia   (501) staff       (20)      156 2023-07-08 02:51:01.757104 reliableGPT-0.2.977/PKG-INFO
--rw-r--r--   0 krrishdholakia   (501) staff       (20)     8377 2023-07-08 02:45:37.000000 reliableGPT-0.2.977/README.md
--rw-r--r--   0 krrishdholakia   (501) staff       (20)      497 2023-06-29 02:51:34.000000 reliableGPT-0.2.977/pyproject.toml
-drwxr-xr-x   0 krrishdholakia   (501) staff       (20)        0 2023-07-08 02:51:01.755353 reliableGPT-0.2.977/reliableGPT.egg-info/
--rw-r--r--   0 krrishdholakia   (501) staff       (20)      156 2023-07-08 02:51:01.000000 reliableGPT-0.2.977/reliableGPT.egg-info/PKG-INFO
--rw-r--r--   0 krrishdholakia   (501) staff       (20)      514 2023-07-08 02:51:01.000000 reliableGPT-0.2.977/reliableGPT.egg-info/SOURCES.txt
--rw-r--r--   0 krrishdholakia   (501) staff       (20)        1 2023-07-08 02:51:01.000000 reliableGPT-0.2.977/reliableGPT.egg-info/dependency_links.txt
--rw-r--r--   0 krrishdholakia   (501) staff       (20)       63 2023-07-08 02:51:01.000000 reliableGPT-0.2.977/reliableGPT.egg-info/requires.txt
--rw-r--r--   0 krrishdholakia   (501) staff       (20)       12 2023-07-08 02:51:01.000000 reliableGPT-0.2.977/reliableGPT.egg-info/top_level.txt
-drwxr-xr-x   0 krrishdholakia   (501) staff       (20)        0 2023-07-08 02:51:01.756908 reliableGPT-0.2.977/reliablegpt/
--rw-r--r--   0 krrishdholakia   (501) staff       (20)     4210 2023-06-29 02:51:34.000000 reliableGPT-0.2.977/reliablegpt/APICallHandler.py
--rw-r--r--   0 krrishdholakia   (501) staff       (20)     3149 2023-07-07 02:48:09.000000 reliableGPT-0.2.977/reliablegpt/Alerting.py
--rw-r--r--   0 krrishdholakia   (501) staff       (20)     4407 2023-06-29 02:51:34.000000 reliableGPT-0.2.977/reliablegpt/CustomQueue.py
--rw-r--r--   0 krrishdholakia   (501) staff       (20)    18630 2023-07-07 02:48:47.000000 reliableGPT-0.2.977/reliablegpt/IndividualRequest.py
--rw-r--r--   0 krrishdholakia   (501) staff       (20)     1286 2023-07-01 20:41:40.000000 reliableGPT-0.2.977/reliablegpt/Model.py
--rw-r--r--   0 krrishdholakia   (501) staff       (20)     5170 2023-07-03 15:14:41.000000 reliableGPT-0.2.977/reliablegpt/RateLimitHandler.py
--rw-r--r--   0 krrishdholakia   (501) staff       (20)     7483 2023-07-06 13:49:42.000000 reliableGPT-0.2.977/reliablegpt/ReliableDataLoaders.py
--rw-r--r--   0 krrishdholakia   (501) staff       (20)      375 2023-07-06 17:39:33.000000 reliableGPT-0.2.977/reliablegpt/__init__.py
--rw-r--r--   0 krrishdholakia   (501) staff       (20)     5233 2023-07-08 02:45:37.000000 reliableGPT-0.2.977/reliablegpt/main.py
--rw-r--r--   0 krrishdholakia   (501) staff       (20)     2363 2023-07-03 15:14:41.000000 reliableGPT-0.2.977/reliablegpt/reliableQuery.py
--rw-r--r--   0 krrishdholakia   (501) staff       (20)       38 2023-07-08 02:51:01.757404 reliableGPT-0.2.977/setup.cfg
--rw-r--r--   0 krrishdholakia   (501) staff       (20)      418 2023-07-08 02:49:24.000000 reliableGPT-0.2.977/setup.py
+drwxr-xr-x   0 krrishdholakia   (501) staff       (20)        0 2023-07-08 02:53:14.109065 reliableGPT-0.2.978/
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)     1065 2023-06-23 13:49:22.000000 reliableGPT-0.2.978/LICENSE
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)      156 2023-07-08 02:53:14.108946 reliableGPT-0.2.978/PKG-INFO
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)     8377 2023-07-08 02:45:37.000000 reliableGPT-0.2.978/README.md
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)      497 2023-06-29 02:51:34.000000 reliableGPT-0.2.978/pyproject.toml
+drwxr-xr-x   0 krrishdholakia   (501) staff       (20)        0 2023-07-08 02:53:14.107051 reliableGPT-0.2.978/reliableGPT.egg-info/
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)      156 2023-07-08 02:53:14.000000 reliableGPT-0.2.978/reliableGPT.egg-info/PKG-INFO
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)      514 2023-07-08 02:53:14.000000 reliableGPT-0.2.978/reliableGPT.egg-info/SOURCES.txt
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)        1 2023-07-08 02:53:14.000000 reliableGPT-0.2.978/reliableGPT.egg-info/dependency_links.txt
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)       63 2023-07-08 02:53:14.000000 reliableGPT-0.2.978/reliableGPT.egg-info/requires.txt
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)       12 2023-07-08 02:53:14.000000 reliableGPT-0.2.978/reliableGPT.egg-info/top_level.txt
+drwxr-xr-x   0 krrishdholakia   (501) staff       (20)        0 2023-07-08 02:53:14.108771 reliableGPT-0.2.978/reliablegpt/
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)     4210 2023-06-29 02:51:34.000000 reliableGPT-0.2.978/reliablegpt/APICallHandler.py
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)     3149 2023-07-07 02:48:09.000000 reliableGPT-0.2.978/reliablegpt/Alerting.py
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)     4407 2023-06-29 02:51:34.000000 reliableGPT-0.2.978/reliablegpt/CustomQueue.py
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)    18415 2023-07-08 02:52:42.000000 reliableGPT-0.2.978/reliablegpt/IndividualRequest.py
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)     1286 2023-07-01 20:41:40.000000 reliableGPT-0.2.978/reliablegpt/Model.py
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)     5170 2023-07-03 15:14:41.000000 reliableGPT-0.2.978/reliablegpt/RateLimitHandler.py
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)     7483 2023-07-06 13:49:42.000000 reliableGPT-0.2.978/reliablegpt/ReliableDataLoaders.py
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)      375 2023-07-06 17:39:33.000000 reliableGPT-0.2.978/reliablegpt/__init__.py
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)     5233 2023-07-08 02:45:37.000000 reliableGPT-0.2.978/reliablegpt/main.py
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)     2363 2023-07-03 15:14:41.000000 reliableGPT-0.2.978/reliablegpt/reliableQuery.py
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)       38 2023-07-08 02:53:14.109107 reliableGPT-0.2.978/setup.cfg
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)      418 2023-07-08 02:53:02.000000 reliableGPT-0.2.978/setup.py
```

### Comparing `reliableGPT-0.2.977/LICENSE` & `reliableGPT-0.2.978/LICENSE`

 * *Files identical despite different names*

### Comparing `reliableGPT-0.2.977/README.md` & `reliableGPT-0.2.978/README.md`

 * *Files identical despite different names*

### Comparing `reliableGPT-0.2.977/reliableGPT.egg-info/SOURCES.txt` & `reliableGPT-0.2.978/reliableGPT.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `reliableGPT-0.2.977/reliablegpt/APICallHandler.py` & `reliableGPT-0.2.978/reliablegpt/APICallHandler.py`

 * *Files identical despite different names*

### Comparing `reliableGPT-0.2.977/reliablegpt/Alerting.py` & `reliableGPT-0.2.978/reliablegpt/Alerting.py`

 * *Files identical despite different names*

### Comparing `reliableGPT-0.2.977/reliablegpt/CustomQueue.py` & `reliableGPT-0.2.978/reliablegpt/CustomQueue.py`

 * *Files identical despite different names*

### Comparing `reliableGPT-0.2.977/reliablegpt/IndividualRequest.py` & `reliableGPT-0.2.978/reliablegpt/IndividualRequest.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,19 @@
 from termcolor import colored
-import time
 import requests
 import copy
 import posthog
-import importlib
 import openai
 from openai import ChatCompletion
 import traceback
-import random
 from uuid import uuid4
-import subprocess
-import importlib
 from waitress import serve
 from flask import Flask, request
-import random
 from uuid import uuid4
-from transformers import AutoTokenizer, AutoModel
-import torch
-import numpy as np
 import traceback
-import hashlib 
-import psutil
-import os 
 from threading import active_count
 
 class IndividualRequest:
   """A brief description of the class."""
 
   def __init__(self,
                model=None,
```

### Comparing `reliableGPT-0.2.977/reliablegpt/Model.py` & `reliableGPT-0.2.978/reliablegpt/Model.py`

 * *Files identical despite different names*

### Comparing `reliableGPT-0.2.977/reliablegpt/RateLimitHandler.py` & `reliableGPT-0.2.978/reliablegpt/RateLimitHandler.py`

 * *Files identical despite different names*

### Comparing `reliableGPT-0.2.977/reliablegpt/ReliableDataLoaders.py` & `reliableGPT-0.2.978/reliablegpt/ReliableDataLoaders.py`

 * *Files identical despite different names*

### Comparing `reliableGPT-0.2.977/reliablegpt/main.py` & `reliableGPT-0.2.978/reliablegpt/main.py`

 * *Files identical despite different names*

### Comparing `reliableGPT-0.2.977/reliablegpt/reliableQuery.py` & `reliableGPT-0.2.978/reliablegpt/reliableQuery.py`

 * *Files identical despite different names*

