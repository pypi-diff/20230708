# Comparing `tmp/deltafi-1.0.2.tar.gz` & `tmp/deltafi-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deltafi-1.0.2.tar", max compression
+gzip compressed data, was "deltafi-1.0.3.tar", max compression
```

## Comparing `deltafi-1.0.2.tar` & `deltafi-1.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0      189 2023-04-10 13:34:58.932322 deltafi-1.0.2/README.md
--rw-r--r--   0        0        0      706 2023-04-10 13:34:58.932322 deltafi-1.0.2/deltafi/__init__.py
--rw-r--r--   0        0        0     7330 2023-06-09 15:16:11.399155 deltafi-1.0.2/deltafi/action.py
--rw-r--r--   0        0        0     1981 2023-04-10 13:34:58.932322 deltafi-1.0.2/deltafi/actioneventqueue.py
--rw-r--r--   0        0        0      985 2023-05-17 20:43:32.059753 deltafi-1.0.2/deltafi/actiontype.py
--rw-r--r--   0        0        0    11025 2023-06-09 15:16:11.400155 deltafi-1.0.2/deltafi/domain.py
--rw-r--r--   0        0        0     1149 2023-04-24 17:42:15.589313 deltafi-1.0.2/deltafi/exception.py
--rw-r--r--   0        0        0     6290 2023-06-09 15:16:11.401155 deltafi-1.0.2/deltafi/input.py
--rw-r--r--   0        0        0     2136 2023-04-10 13:34:58.937322 deltafi-1.0.2/deltafi/logger.py
--rw-r--r--   0        0        0      967 2023-04-10 13:34:58.938322 deltafi-1.0.2/deltafi/metric.py
--rw-r--r--   0        0        0    11666 2023-06-06 18:39:40.022585 deltafi-1.0.2/deltafi/plugin.py
--rw-r--r--   0        0        0    10706 2023-05-22 14:40:08.186270 deltafi-1.0.2/deltafi/result.py
--rw-r--r--   0        0        0     2740 2023-05-17 20:43:32.061753 deltafi-1.0.2/deltafi/storage.py
--rw-r--r--   0        0        0     1277 2023-06-29 14:25:05.584352 deltafi-1.0.2/pyproject.toml
--rw-r--r--   0        0        0     1708 1970-01-01 00:00:00.000000 deltafi-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0      189 2023-04-10 13:34:58.932322 deltafi-1.0.3/README.md
+-rw-r--r--   0        0        0      706 2023-04-10 13:34:58.932322 deltafi-1.0.3/deltafi/__init__.py
+-rw-r--r--   0        0        0     7330 2023-06-09 15:16:11.399155 deltafi-1.0.3/deltafi/action.py
+-rw-r--r--   0        0        0     1981 2023-04-10 13:34:58.932322 deltafi-1.0.3/deltafi/actioneventqueue.py
+-rw-r--r--   0        0        0      985 2023-05-17 20:43:32.059753 deltafi-1.0.3/deltafi/actiontype.py
+-rw-r--r--   0        0        0    11025 2023-06-09 15:16:11.400155 deltafi-1.0.3/deltafi/domain.py
+-rw-r--r--   0        0        0     1149 2023-04-24 17:42:15.589313 deltafi-1.0.3/deltafi/exception.py
+-rw-r--r--   0        0        0     6290 2023-06-09 15:16:11.401155 deltafi-1.0.3/deltafi/input.py
+-rw-r--r--   0        0        0     2136 2023-04-10 13:34:58.937322 deltafi-1.0.3/deltafi/logger.py
+-rw-r--r--   0        0        0      967 2023-04-10 13:34:58.938322 deltafi-1.0.3/deltafi/metric.py
+-rw-r--r--   0        0        0    11666 2023-06-06 18:39:40.022585 deltafi-1.0.3/deltafi/plugin.py
+-rw-r--r--   0        0        0    10706 2023-05-22 14:40:08.186270 deltafi-1.0.3/deltafi/result.py
+-rw-r--r--   0        0        0     2740 2023-05-17 20:43:32.061753 deltafi-1.0.3/deltafi/storage.py
+-rw-r--r--   0        0        0     1276 2023-07-08 05:32:09.989987 deltafi-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0     1715 1970-01-01 00:00:00.000000 deltafi-1.0.3/PKG-INFO
```

### Comparing `deltafi-1.0.2/deltafi/__init__.py` & `deltafi-1.0.3/deltafi/__init__.py`

 * *Files identical despite different names*

### Comparing `deltafi-1.0.2/deltafi/action.py` & `deltafi-1.0.3/deltafi/action.py`

 * *Files identical despite different names*

### Comparing `deltafi-1.0.2/deltafi/actioneventqueue.py` & `deltafi-1.0.3/deltafi/actioneventqueue.py`

 * *Files identical despite different names*

### Comparing `deltafi-1.0.2/deltafi/actiontype.py` & `deltafi-1.0.3/deltafi/actiontype.py`

 * *Files identical despite different names*

### Comparing `deltafi-1.0.2/deltafi/domain.py` & `deltafi-1.0.3/deltafi/domain.py`

 * *Files identical despite different names*

### Comparing `deltafi-1.0.2/deltafi/exception.py` & `deltafi-1.0.3/deltafi/exception.py`

 * *Files identical despite different names*

### Comparing `deltafi-1.0.2/deltafi/input.py` & `deltafi-1.0.3/deltafi/input.py`

 * *Files identical despite different names*

### Comparing `deltafi-1.0.2/deltafi/logger.py` & `deltafi-1.0.3/deltafi/logger.py`

 * *Files identical despite different names*

### Comparing `deltafi-1.0.2/deltafi/metric.py` & `deltafi-1.0.3/deltafi/metric.py`

 * *Files identical despite different names*

### Comparing `deltafi-1.0.2/deltafi/plugin.py` & `deltafi-1.0.3/deltafi/plugin.py`

 * *Files identical despite different names*

### Comparing `deltafi-1.0.2/deltafi/result.py` & `deltafi-1.0.3/deltafi/result.py`

 * *Files identical despite different names*

### Comparing `deltafi-1.0.2/deltafi/storage.py` & `deltafi-1.0.3/deltafi/storage.py`

 * *Files identical despite different names*

### Comparing `deltafi-1.0.2/pyproject.toml` & `deltafi-1.0.3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "deltafi"
-version = "1.0.2"
+version = "1.0.3"
 description = "SDK for DeltaFi plugins and actions"
 authors = ["DeltaFi <deltafi@systolic.com>"]
 license = "Apache License, Version 2.0"
 readme = "README.md"
 keywords = ["deltafi"]
 classifiers = [
     "License :: OSI Approved :: Apache Software License",
@@ -18,26 +18,26 @@
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10"
 ]
 
 [tool.poetry.dependencies]
 python = "^3.7"
 json-logging = ">=1.3.0"
-minio = ">=7.1.14"
-pydantic = ">=1.10.7"
-redis = ">=4.5.5"
-requests = ">=2.30.0"
-urllib3 = "^1.26.12"
+minio = ">=7.1.15"
+pydantic = "^1.10.9"
+redis = ">=4.6.0"
+requests = ">=2.31.0"
+urllib3 = "^1.26.16"
 
 [tool.poetry.group.test]
 optional = true
 
 [tool.poetry.group.test.dependencies]
-pytest = ">=7.3.1"
-pytest-mock = ">=3.10.0"
+pytest = ">=7.4.0"
+pytest-mock = ">=3.11.1"
 mockito = ">=1.4.0"
 
 [tool.poetry.urls]
 'Source Code' = "https://gitlab.com/deltafi/deltafi"
 Documentation = "https://docs.deltafi.org/#/"
 'Bug Reports' = "https://chat.deltafi.org/deltafi/channels/bug-reports"
```

### Comparing `deltafi-1.0.2/PKG-INFO` & `deltafi-1.0.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deltafi
-Version: 1.0.2
+Version: 1.0.3
 Summary: SDK for DeltaFi plugins and actions
 License: Apache License, Version 2.0
 Keywords: deltafi
 Author: DeltaFi
 Author-email: deltafi@systolic.com
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 4 - Beta
@@ -21,19 +21,19 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development
 Requires-Dist: json-logging (>=1.3.0)
-Requires-Dist: minio (>=7.1.14)
-Requires-Dist: pydantic (>=1.10.7)
-Requires-Dist: redis (>=4.5.5)
-Requires-Dist: requests (>=2.30.0)
-Requires-Dist: urllib3 (>=1.26.12,<2.0.0)
+Requires-Dist: minio (>=7.1.15)
+Requires-Dist: pydantic (>=1.10.9,<2.0.0)
+Requires-Dist: redis (>=4.6.0)
+Requires-Dist: requests (>=2.31.0)
+Requires-Dist: urllib3 (>=1.26.16,<2.0.0)
 Project-URL: Bug Reports, https://chat.deltafi.org/deltafi/channels/bug-reports
 Project-URL: Documentation, https://docs.deltafi.org/#/
 Project-URL: Source Code, https://gitlab.com/deltafi/deltafi
 Description-Content-Type: text/markdown
 
 # DeltaFi Action Kit
```

