# Comparing `tmp/tarandm_analytics-0.0.7.tar.gz` & `tmp/tarandm_analytics-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tarandm_analytics-0.0.7.tar", max compression
+gzip compressed data, was "tarandm_analytics-0.0.8.tar", max compression
```

## Comparing `tarandm_analytics-0.0.7.tar` & `tarandm_analytics-0.0.8.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1033 2023-07-08 13:47:35.819728 tarandm_analytics-0.0.7/pyproject.toml
--rw-r--r--   0        0        0     6370 2023-06-29 09:18:17.981136 tarandm_analytics-0.0.7/README.md
--rw-r--r--   0        0        0        0 2023-06-29 09:18:17.984041 tarandm_analytics-0.0.7/tarandm_analytics/__init__.py
--rw-r--r--   0        0        0      911 2023-07-05 14:43:36.988316 tarandm_analytics-0.0.7/tarandm_analytics/base_class.py
--rw-r--r--   0        0        0        0 2023-07-03 15:26:41.279844 tarandm_analytics-0.0.7/tarandm_analytics/export_predictive_model/__init__.py
--rw-r--r--   0        0        0      207 2023-07-04 06:21:18.742105 tarandm_analytics-0.0.7/tarandm_analytics/export_predictive_model/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0    26096 2023-07-06 13:24:31.720712 tarandm_analytics-0.0.7/tarandm_analytics/export_predictive_model/__pycache__/create_predictive_model.cpython-310.pyc
--rw-r--r--   0        0        0     4023 2023-07-04 06:21:24.012030 tarandm_analytics-0.0.7/tarandm_analytics/export_predictive_model/__pycache__/model_visualization.cpython-310.pyc
--rw-r--r--   0        0        0    37475 2023-07-08 12:33:47.556516 tarandm_analytics-0.0.7/tarandm_analytics/export_predictive_model/create_predictive_model.py
--rw-r--r--   0        0        0     4670 2023-07-08 13:45:38.487547 tarandm_analytics-0.0.7/tarandm_analytics/export_predictive_model/model_visualization.py
--rw-r--r--   0        0        0      342 2023-07-06 11:25:46.354702 tarandm_analytics-0.0.7/tarandm_analytics/utils.py
--rw-r--r--   0        0        0     6935 1970-01-01 00:00:00.000000 tarandm_analytics-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0     1033 2023-07-08 18:33:54.233026 tarandm_analytics-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0     6370 2023-06-29 09:18:17.981136 tarandm_analytics-0.0.8/README.md
+-rw-r--r--   0        0        0       21 2023-07-08 18:33:54.226019 tarandm_analytics-0.0.8/tarandm_analytics/__init__.py
+-rw-r--r--   0        0        0      911 2023-07-05 14:43:36.988316 tarandm_analytics-0.0.8/tarandm_analytics/base_class.py
+-rw-r--r--   0        0        0        0 2023-07-03 15:26:41.279844 tarandm_analytics-0.0.8/tarandm_analytics/export_predictive_model/__init__.py
+-rw-r--r--   0        0        0      207 2023-07-04 06:21:18.742105 tarandm_analytics-0.0.8/tarandm_analytics/export_predictive_model/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0    26096 2023-07-06 13:24:31.720712 tarandm_analytics-0.0.8/tarandm_analytics/export_predictive_model/__pycache__/create_predictive_model.cpython-310.pyc
+-rw-r--r--   0        0        0     4023 2023-07-04 06:21:24.012030 tarandm_analytics-0.0.8/tarandm_analytics/export_predictive_model/__pycache__/model_visualization.cpython-310.pyc
+-rw-r--r--   0        0        0    37475 2023-07-08 12:33:47.556516 tarandm_analytics-0.0.8/tarandm_analytics/export_predictive_model/create_predictive_model.py
+-rw-r--r--   0        0        0     4670 2023-07-08 13:45:38.487547 tarandm_analytics-0.0.8/tarandm_analytics/export_predictive_model/model_visualization.py
+-rw-r--r--   0        0        0      342 2023-07-06 11:25:46.354702 tarandm_analytics-0.0.8/tarandm_analytics/utils.py
+-rw-r--r--   0        0        0     6935 1970-01-01 00:00:00.000000 tarandm_analytics-0.0.8/PKG-INFO
```

### Comparing `tarandm_analytics-0.0.7/pyproject.toml` & `tarandm_analytics-0.0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tarandm_analytics"
-version = "0.0.7"
+version = "0.0.8"
 description = "Package contains support functions for creating predictive models in format compatible with TaranDM software."
 authors = ["Marek Teller <mteller@taran.ai>"]
 readme = "README.md"
 packages = [
     { include = "tarandm_analytics" }
 ]
```

### Comparing `tarandm_analytics-0.0.7/README.md` & `tarandm_analytics-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `tarandm_analytics-0.0.7/tarandm_analytics/base_class.py` & `tarandm_analytics-0.0.8/tarandm_analytics/base_class.py`

 * *Files identical despite different names*

### Comparing `tarandm_analytics-0.0.7/tarandm_analytics/export_predictive_model/__pycache__/create_predictive_model.cpython-310.pyc` & `tarandm_analytics-0.0.8/tarandm_analytics/export_predictive_model/__pycache__/create_predictive_model.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `tarandm_analytics-0.0.7/tarandm_analytics/export_predictive_model/__pycache__/model_visualization.cpython-310.pyc` & `tarandm_analytics-0.0.8/tarandm_analytics/export_predictive_model/__pycache__/model_visualization.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `tarandm_analytics-0.0.7/tarandm_analytics/export_predictive_model/create_predictive_model.py` & `tarandm_analytics-0.0.8/tarandm_analytics/export_predictive_model/create_predictive_model.py`

 * *Files identical despite different names*

### Comparing `tarandm_analytics-0.0.7/tarandm_analytics/export_predictive_model/model_visualization.py` & `tarandm_analytics-0.0.8/tarandm_analytics/export_predictive_model/model_visualization.py`

 * *Files identical despite different names*

### Comparing `tarandm_analytics-0.0.7/PKG-INFO` & `tarandm_analytics-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tarandm-analytics
-Version: 0.0.7
+Version: 0.0.8
 Summary: Package contains support functions for creating predictive models in format compatible with TaranDM software.
 Author: Marek Teller
 Author-email: mteller@taran.ai
 Requires-Python: >=3.10,<3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: llvmlite
```

