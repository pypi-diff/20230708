# Comparing `tmp/langchain-chatglm-0.0.4.tar.gz` & `tmp/langchain-chatglm-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langchain-chatglm-0.0.4.tar", last modified: Fri Jul  7 23:44:09 2023, max compression
+gzip compressed data, was "langchain-chatglm-0.0.5.tar", last modified: Sat Jul  8 06:57:23 2023, max compression
```

## Comparing `langchain-chatglm-0.0.4.tar` & `langchain-chatglm-0.0.5.tar`

### file list

```diff
@@ -1,15 +1,17 @@
-drwxr-xr-x   0 tsai      (1000) tsai      (1000)        0 2023-07-07 23:44:09.240769 langchain-chatglm-0.0.4/
--rw-r--r--   0 tsai      (1000) tsai      (1000)     1065 2023-07-07 23:39:43.000000 langchain-chatglm-0.0.4/LICENSE
--rw-r--r--   0 tsai      (1000) tsai      (1000)     1616 2023-07-07 23:44:09.240769 langchain-chatglm-0.0.4/PKG-INFO
--rw-r--r--   0 tsai      (1000) tsai      (1000)     1065 2023-07-07 23:39:43.000000 langchain-chatglm-0.0.4/README.md
-drwxr-xr-x   0 tsai      (1000) tsai      (1000)        0 2023-07-07 23:44:09.240769 langchain-chatglm-0.0.4/langchain_chatglm/
--rw-r--r--   0 tsai      (1000) tsai      (1000)       42 2023-07-07 23:39:43.000000 langchain-chatglm-0.0.4/langchain_chatglm/__init__.py
--rw-r--r--   0 tsai      (1000) tsai      (1000)     4973 2023-07-07 23:39:43.000000 langchain-chatglm-0.0.4/langchain_chatglm/chatglm_pipline.py
-drwxr-xr-x   0 tsai      (1000) tsai      (1000)        0 2023-07-07 23:44:09.240769 langchain-chatglm-0.0.4/langchain_chatglm.egg-info/
--rw-r--r--   0 tsai      (1000) tsai      (1000)     1616 2023-07-07 23:44:09.000000 langchain-chatglm-0.0.4/langchain_chatglm.egg-info/PKG-INFO
--rw-r--r--   0 tsai      (1000) tsai      (1000)      303 2023-07-07 23:44:09.000000 langchain-chatglm-0.0.4/langchain_chatglm.egg-info/SOURCES.txt
--rw-r--r--   0 tsai      (1000) tsai      (1000)        1 2023-07-07 23:44:09.000000 langchain-chatglm-0.0.4/langchain_chatglm.egg-info/dependency_links.txt
--rw-r--r--   0 tsai      (1000) tsai      (1000)       37 2023-07-07 23:44:09.000000 langchain-chatglm-0.0.4/langchain_chatglm.egg-info/requires.txt
--rw-r--r--   0 tsai      (1000) tsai      (1000)       18 2023-07-07 23:44:09.000000 langchain-chatglm-0.0.4/langchain_chatglm.egg-info/top_level.txt
--rw-r--r--   0 tsai      (1000) tsai      (1000)      690 2023-07-07 23:39:43.000000 langchain-chatglm-0.0.4/pyproject.toml
--rw-r--r--   0 tsai      (1000) tsai      (1000)       38 2023-07-07 23:44:09.240769 langchain-chatglm-0.0.4/setup.cfg
+drwxr-xr-x   0 tsai      (1000) tsai      (1000)        0 2023-07-08 06:57:22.999389 langchain-chatglm-0.0.5/
+-rw-r--r--   0 tsai      (1000) tsai      (1000)     1065 2023-07-07 23:39:43.000000 langchain-chatglm-0.0.5/LICENSE
+-rw-r--r--   0 tsai      (1000) tsai      (1000)     1616 2023-07-08 06:57:22.999389 langchain-chatglm-0.0.5/PKG-INFO
+-rw-r--r--   0 tsai      (1000) tsai      (1000)     1065 2023-07-07 23:39:43.000000 langchain-chatglm-0.0.5/README.md
+drwxr-xr-x   0 tsai      (1000) tsai      (1000)        0 2023-07-08 06:57:22.999389 langchain-chatglm-0.0.5/langchain/
+-rw-r--r--   0 tsai      (1000) tsai      (1000)       59 2023-07-08 01:02:44.000000 langchain-chatglm-0.0.5/langchain/__init__.py
+drwxr-xr-x   0 tsai      (1000) tsai      (1000)        0 2023-07-08 06:57:22.999389 langchain-chatglm-0.0.5/langchain/llms/
+-rw-r--r--   0 tsai      (1000) tsai      (1000)       59 2023-07-08 01:01:26.000000 langchain-chatglm-0.0.5/langchain/llms/__init__.py
+-rw-r--r--   0 tsai      (1000) tsai      (1000)     4973 2023-07-08 01:01:15.000000 langchain-chatglm-0.0.5/langchain/llms/chatglm_pipeline.py
+drwxr-xr-x   0 tsai      (1000) tsai      (1000)        0 2023-07-08 06:57:22.999389 langchain-chatglm-0.0.5/langchain_chatglm.egg-info/
+-rw-r--r--   0 tsai      (1000) tsai      (1000)     1616 2023-07-08 06:57:22.000000 langchain-chatglm-0.0.5/langchain_chatglm.egg-info/PKG-INFO
+-rw-r--r--   0 tsai      (1000) tsai      (1000)      320 2023-07-08 06:57:22.000000 langchain-chatglm-0.0.5/langchain_chatglm.egg-info/SOURCES.txt
+-rw-r--r--   0 tsai      (1000) tsai      (1000)        1 2023-07-08 06:57:22.000000 langchain-chatglm-0.0.5/langchain_chatglm.egg-info/dependency_links.txt
+-rw-r--r--   0 tsai      (1000) tsai      (1000)       37 2023-07-08 06:57:22.000000 langchain-chatglm-0.0.5/langchain_chatglm.egg-info/requires.txt
+-rw-r--r--   0 tsai      (1000) tsai      (1000)       10 2023-07-08 06:57:22.000000 langchain-chatglm-0.0.5/langchain_chatglm.egg-info/top_level.txt
+-rw-r--r--   0 tsai      (1000) tsai      (1000)      690 2023-07-08 01:03:02.000000 langchain-chatglm-0.0.5/pyproject.toml
+-rw-r--r--   0 tsai      (1000) tsai      (1000)       38 2023-07-08 06:57:22.999389 langchain-chatglm-0.0.5/setup.cfg
```

### Comparing `langchain-chatglm-0.0.4/LICENSE` & `langchain-chatglm-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `langchain-chatglm-0.0.4/PKG-INFO` & `langchain-chatglm-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langchain-chatglm
-Version: 0.0.4
+Version: 0.0.5
 Summary: esay use ChatGLM in LangChain.
 Author-email: Sim Tsai <13759975+SimTsai@users.noreply.github.com>
 Project-URL: Homepage, https://github.com/SimTsai/langchain_chatglm
 Project-URL: Bug Tracker, https://github.com/SimTsai/langchain_chatglm/issues
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `langchain-chatglm-0.0.4/README.md` & `langchain-chatglm-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `langchain-chatglm-0.0.4/langchain_chatglm/chatglm_pipline.py` & `langchain-chatglm-0.0.5/langchain/llms/chatglm_pipeline.py`

 * *Files identical despite different names*

### Comparing `langchain-chatglm-0.0.4/langchain_chatglm.egg-info/PKG-INFO` & `langchain-chatglm-0.0.5/langchain_chatglm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langchain-chatglm
-Version: 0.0.4
+Version: 0.0.5
 Summary: esay use ChatGLM in LangChain.
 Author-email: Sim Tsai <13759975+SimTsai@users.noreply.github.com>
 Project-URL: Homepage, https://github.com/SimTsai/langchain_chatglm
 Project-URL: Bug Tracker, https://github.com/SimTsai/langchain_chatglm/issues
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `langchain-chatglm-0.0.4/pyproject.toml` & `langchain-chatglm-0.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=68.0.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "langchain-chatglm"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
   { name="Sim Tsai", email="13759975+SimTsai@users.noreply.github.com" },
 ]
 description = "esay use ChatGLM in LangChain."
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

