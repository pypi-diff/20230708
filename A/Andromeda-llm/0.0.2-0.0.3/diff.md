# Comparing `tmp/Andromeda-llm-0.0.2.tar.gz` & `tmp/Andromeda-llm-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Andromeda-llm-0.0.2.tar", last modified: Sun Jul  2 04:56:18 2023, max compression
+gzip compressed data, was "Andromeda-llm-0.0.3.tar", last modified: Fri Jul  7 22:22:36 2023, max compression
```

## Comparing `Andromeda-llm-0.0.2.tar` & `Andromeda-llm-0.0.3.tar`

### file list

```diff
@@ -1,28 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 04:56:18.778125 Andromeda-llm-0.0.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 04:56:18.774125 Andromeda-llm-0.0.2/Andromeda/
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-02 04:56:09.000000 Andromeda-llm-0.0.2/Andromeda/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3214 2023-07-02 04:56:09.000000 Andromeda-llm-0.0.2/Andromeda/build_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2122 2023-07-02 04:56:09.000000 Andromeda-llm-0.0.2/Andromeda/inference.py
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-07-02 04:56:09.000000 Andromeda-llm-0.0.2/Andromeda/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 04:56:18.778125 Andromeda-llm-0.0.2/Andromeda/optimus_prime/
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-07-02 04:56:09.000000 Andromeda-llm-0.0.2/Andromeda/optimus_prime/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7660 2023-07-02 04:56:09.000000 Andromeda-llm-0.0.2/Andromeda/optimus_prime/attend.py
--rw-r--r--   0 runner    (1001) docker     (123)     4523 2023-07-02 04:56:09.000000 Andromeda-llm-0.0.2/Andromeda/optimus_prime/autoregressive_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-07-02 04:56:09.000000 Andromeda-llm-0.0.2/Andromeda/optimus_prime/continuous_autoregressive_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    10414 2023-07-02 04:56:09.000000 Andromeda-llm-0.0.2/Andromeda/optimus_prime/nonautoregressive_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    55026 2023-07-02 04:56:09.000000 Andromeda-llm-0.0.2/Andromeda/optimus_prime/x_transformers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3987 2023-07-02 04:56:09.000000 Andromeda-llm-0.0.2/Andromeda/optimus_prime/xl_autoregressive_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    23945 2023-07-02 04:56:09.000000 Andromeda-llm-0.0.2/Andromeda/train_distributed.py
--rw-r--r--   0 runner    (1001) docker     (123)    23620 2023-07-02 04:56:09.000000 Andromeda-llm-0.0.2/Andromeda/train_distributed_accelerate.py
--rw-r--r--   0 runner    (1001) docker     (123)    11404 2023-07-02 04:56:09.000000 Andromeda-llm-0.0.2/Andromeda/training.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 04:56:18.778125 Andromeda-llm-0.0.2/Andromeda_llm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-07-02 04:56:18.000000 Andromeda-llm-0.0.2/Andromeda_llm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-07-02 04:56:18.000000 Andromeda-llm-0.0.2/Andromeda_llm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 04:56:18.000000 Andromeda-llm-0.0.2/Andromeda_llm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-02 04:56:18.000000 Andromeda-llm-0.0.2/Andromeda_llm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-02 04:56:18.000000 Andromeda-llm-0.0.2/Andromeda_llm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-02 04:56:09.000000 Andromeda-llm-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-07-02 04:56:18.778125 Andromeda-llm-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9721 2023-07-02 04:56:09.000000 Andromeda-llm-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-02 04:56:18.778125 Andromeda-llm-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      981 2023-07-02 04:56:09.000000 Andromeda-llm-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 22:22:36.467905 Andromeda-llm-0.0.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 22:22:36.463905 Andromeda-llm-0.0.3/Andromeda/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-07 22:22:22.000000 Andromeda-llm-0.0.3/Andromeda/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3214 2023-07-07 22:22:22.000000 Andromeda-llm-0.0.3/Andromeda/build_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2122 2023-07-07 22:22:22.000000 Andromeda-llm-0.0.3/Andromeda/inference.py
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-07-07 22:22:22.000000 Andromeda-llm-0.0.3/Andromeda/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 22:22:36.463905 Andromeda-llm-0.0.3/Andromeda/optimus_prime/
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-07-07 22:22:22.000000 Andromeda-llm-0.0.3/Andromeda/optimus_prime/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7660 2023-07-07 22:22:22.000000 Andromeda-llm-0.0.3/Andromeda/optimus_prime/attend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4523 2023-07-07 22:22:22.000000 Andromeda-llm-0.0.3/Andromeda/optimus_prime/autoregressive_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-07-07 22:22:22.000000 Andromeda-llm-0.0.3/Andromeda/optimus_prime/continuous_autoregressive_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10414 2023-07-07 22:22:22.000000 Andromeda-llm-0.0.3/Andromeda/optimus_prime/nonautoregressive_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55026 2023-07-07 22:22:22.000000 Andromeda-llm-0.0.3/Andromeda/optimus_prime/x_transformers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3987 2023-07-07 22:22:22.000000 Andromeda-llm-0.0.3/Andromeda/optimus_prime/xl_autoregressive_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23945 2023-07-07 22:22:22.000000 Andromeda-llm-0.0.3/Andromeda/train_distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23620 2023-07-07 22:22:22.000000 Andromeda-llm-0.0.3/Andromeda/train_distributed_accelerate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 22:22:36.467905 Andromeda-llm-0.0.3/Andromeda_llm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-07-07 22:22:36.000000 Andromeda-llm-0.0.3/Andromeda_llm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-07-07 22:22:36.000000 Andromeda-llm-0.0.3/Andromeda_llm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 22:22:36.000000 Andromeda-llm-0.0.3/Andromeda_llm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-07 22:22:36.000000 Andromeda-llm-0.0.3/Andromeda_llm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-07 22:22:36.000000 Andromeda-llm-0.0.3/Andromeda_llm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-07 22:22:22.000000 Andromeda-llm-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-07-07 22:22:36.467905 Andromeda-llm-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9721 2023-07-07 22:22:22.000000 Andromeda-llm-0.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 22:22:36.467905 Andromeda-llm-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-07-07 22:22:22.000000 Andromeda-llm-0.0.3/setup.py
```

### Comparing `Andromeda-llm-0.0.2/Andromeda/build_dataset.py` & `Andromeda-llm-0.0.3/Andromeda/build_dataset.py`

 * *Files identical despite different names*

### Comparing `Andromeda-llm-0.0.2/Andromeda/inference.py` & `Andromeda-llm-0.0.3/Andromeda/inference.py`

 * *Files identical despite different names*

### Comparing `Andromeda-llm-0.0.2/Andromeda/model.py` & `Andromeda-llm-0.0.3/Andromeda/model.py`

 * *Files identical despite different names*

### Comparing `Andromeda-llm-0.0.2/Andromeda/optimus_prime/__init__.py` & `Andromeda-llm-0.0.3/Andromeda/optimus_prime/__init__.py`

 * *Files identical despite different names*

### Comparing `Andromeda-llm-0.0.2/Andromeda/optimus_prime/attend.py` & `Andromeda-llm-0.0.3/Andromeda/optimus_prime/attend.py`

 * *Files identical despite different names*

### Comparing `Andromeda-llm-0.0.2/Andromeda/optimus_prime/autoregressive_wrapper.py` & `Andromeda-llm-0.0.3/Andromeda/optimus_prime/autoregressive_wrapper.py`

 * *Files identical despite different names*

### Comparing `Andromeda-llm-0.0.2/Andromeda/optimus_prime/continuous_autoregressive_wrapper.py` & `Andromeda-llm-0.0.3/Andromeda/optimus_prime/continuous_autoregressive_wrapper.py`

 * *Files identical despite different names*

### Comparing `Andromeda-llm-0.0.2/Andromeda/optimus_prime/nonautoregressive_wrapper.py` & `Andromeda-llm-0.0.3/Andromeda/optimus_prime/nonautoregressive_wrapper.py`

 * *Files identical despite different names*

### Comparing `Andromeda-llm-0.0.2/Andromeda/optimus_prime/x_transformers.py` & `Andromeda-llm-0.0.3/Andromeda/optimus_prime/x_transformers.py`

 * *Files identical despite different names*

### Comparing `Andromeda-llm-0.0.2/Andromeda/optimus_prime/xl_autoregressive_wrapper.py` & `Andromeda-llm-0.0.3/Andromeda/optimus_prime/xl_autoregressive_wrapper.py`

 * *Files identical despite different names*

### Comparing `Andromeda-llm-0.0.2/Andromeda/train_distributed.py` & `Andromeda-llm-0.0.3/Andromeda/train_distributed.py`

 * *Files identical despite different names*

### Comparing `Andromeda-llm-0.0.2/Andromeda/train_distributed_accelerate.py` & `Andromeda-llm-0.0.3/Andromeda/train_distributed_accelerate.py`

 * *Files identical despite different names*

### Comparing `Andromeda-llm-0.0.2/Andromeda_llm.egg-info/PKG-INFO` & `Andromeda-llm-0.0.3/Andromeda_llm.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Andromeda-llm
-Version: 0.0.2
+Version: 0.0.3
 Summary: andromeda - Pytorch
 Home-page: https://github.com/kyegomez/Andromeda
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,attention mechanism,transformers
 Classifier: Development Status :: 4 - Beta
```

### Comparing `Andromeda-llm-0.0.2/Andromeda_llm.egg-info/SOURCES.txt` & `Andromeda-llm-0.0.3/Andromeda_llm.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 setup.py
 Andromeda/__init__.py
 Andromeda/build_dataset.py
 Andromeda/inference.py
 Andromeda/model.py
 Andromeda/train_distributed.py
 Andromeda/train_distributed_accelerate.py
-Andromeda/training.py
 Andromeda/optimus_prime/__init__.py
 Andromeda/optimus_prime/attend.py
 Andromeda/optimus_prime/autoregressive_wrapper.py
 Andromeda/optimus_prime/continuous_autoregressive_wrapper.py
 Andromeda/optimus_prime/nonautoregressive_wrapper.py
 Andromeda/optimus_prime/x_transformers.py
 Andromeda/optimus_prime/xl_autoregressive_wrapper.py
```

### Comparing `Andromeda-llm-0.0.2/LICENSE` & `Andromeda-llm-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `Andromeda-llm-0.0.2/PKG-INFO` & `Andromeda-llm-0.0.3/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Andromeda-llm
-Version: 0.0.2
+Version: 0.0.3
 Summary: andromeda - Pytorch
 Home-page: https://github.com/kyegomez/Andromeda
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,attention mechanism,transformers
 Classifier: Development Status :: 4 - Beta
```

### Comparing `Andromeda-llm-0.0.2/README.md` & `Andromeda-llm-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `Andromeda-llm-0.0.2/setup.py` & `Andromeda-llm-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'Andromeda-llm',
   packages = find_packages(exclude=['examples']),
-  version = '0.0.2',
+  version = '0.0.3',
   license='MIT',
   description = 'andromeda - Pytorch',
   author = 'Kye Gomez',
   author_email = 'kye@apac.ai',
   url = 'https://github.com/kyegomez/Andromeda',
   long_description_content_type = 'text/markdown',
   keywords = [
```

