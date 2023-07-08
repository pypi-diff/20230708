# Comparing `tmp/tarandm_analytics-0.0.6.tar.gz` & `tmp/tarandm_analytics-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tarandm_analytics-0.0.6.tar", max compression
+gzip compressed data, was "tarandm_analytics-0.0.7.tar", max compression
```

## Comparing `tarandm_analytics-0.0.6.tar` & `tarandm_analytics-0.0.7.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1033 2023-07-06 14:28:20.037786 tarandm_analytics-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     6370 2023-06-29 09:18:17.981136 tarandm_analytics-0.0.6/README.md
--rw-r--r--   0        0        0        0 2023-06-29 09:18:17.984041 tarandm_analytics-0.0.6/tarandm_analytics/__init__.py
--rw-r--r--   0        0        0      911 2023-07-05 14:43:36.988316 tarandm_analytics-0.0.6/tarandm_analytics/base.py
--rw-r--r--   0        0        0        0 2023-07-03 15:26:41.279844 tarandm_analytics-0.0.6/tarandm_analytics/export_predictive_model/__init__.py
--rw-r--r--   0        0        0      207 2023-07-04 06:21:18.742105 tarandm_analytics-0.0.6/tarandm_analytics/export_predictive_model/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0    26096 2023-07-06 13:24:31.720712 tarandm_analytics-0.0.6/tarandm_analytics/export_predictive_model/__pycache__/create_predictive_model.cpython-310.pyc
--rw-r--r--   0        0        0     4023 2023-07-04 06:21:24.012030 tarandm_analytics-0.0.6/tarandm_analytics/export_predictive_model/__pycache__/model_visualization.cpython-310.pyc
--rw-r--r--   0        0        0    37469 2023-07-06 13:25:44.694037 tarandm_analytics-0.0.6/tarandm_analytics/export_predictive_model/create_predictive_model.py
--rw-r--r--   0        0        0     4641 2023-06-29 09:18:17.986082 tarandm_analytics-0.0.6/tarandm_analytics/export_predictive_model/model_visualization.py
--rw-r--r--   0        0        0      342 2023-07-06 11:25:46.354702 tarandm_analytics-0.0.6/tarandm_analytics/utils.py
--rw-r--r--   0        0        0     6935 1970-01-01 00:00:00.000000 tarandm_analytics-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0     1033 2023-07-08 13:47:35.819728 tarandm_analytics-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     6370 2023-06-29 09:18:17.981136 tarandm_analytics-0.0.7/README.md
+-rw-r--r--   0        0        0        0 2023-06-29 09:18:17.984041 tarandm_analytics-0.0.7/tarandm_analytics/__init__.py
+-rw-r--r--   0        0        0      911 2023-07-05 14:43:36.988316 tarandm_analytics-0.0.7/tarandm_analytics/base_class.py
+-rw-r--r--   0        0        0        0 2023-07-03 15:26:41.279844 tarandm_analytics-0.0.7/tarandm_analytics/export_predictive_model/__init__.py
+-rw-r--r--   0        0        0      207 2023-07-04 06:21:18.742105 tarandm_analytics-0.0.7/tarandm_analytics/export_predictive_model/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0    26096 2023-07-06 13:24:31.720712 tarandm_analytics-0.0.7/tarandm_analytics/export_predictive_model/__pycache__/create_predictive_model.cpython-310.pyc
+-rw-r--r--   0        0        0     4023 2023-07-04 06:21:24.012030 tarandm_analytics-0.0.7/tarandm_analytics/export_predictive_model/__pycache__/model_visualization.cpython-310.pyc
+-rw-r--r--   0        0        0    37475 2023-07-08 12:33:47.556516 tarandm_analytics-0.0.7/tarandm_analytics/export_predictive_model/create_predictive_model.py
+-rw-r--r--   0        0        0     4670 2023-07-08 13:45:38.487547 tarandm_analytics-0.0.7/tarandm_analytics/export_predictive_model/model_visualization.py
+-rw-r--r--   0        0        0      342 2023-07-06 11:25:46.354702 tarandm_analytics-0.0.7/tarandm_analytics/utils.py
+-rw-r--r--   0        0        0     6935 1970-01-01 00:00:00.000000 tarandm_analytics-0.0.7/PKG-INFO
```

### Comparing `tarandm_analytics-0.0.6/pyproject.toml` & `tarandm_analytics-0.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tarandm_analytics"
-version = "0.0.6"
+version = "0.0.7"
 description = "Package contains support functions for creating predictive models in format compatible with TaranDM software."
 authors = ["Marek Teller <mteller@taran.ai>"]
 readme = "README.md"
 packages = [
     { include = "tarandm_analytics" }
 ]
```

### Comparing `tarandm_analytics-0.0.6/README.md` & `tarandm_analytics-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `tarandm_analytics-0.0.6/tarandm_analytics/base.py` & `tarandm_analytics-0.0.7/tarandm_analytics/base_class.py`

 * *Files identical despite different names*

### Comparing `tarandm_analytics-0.0.6/tarandm_analytics/export_predictive_model/__pycache__/create_predictive_model.cpython-310.pyc` & `tarandm_analytics-0.0.7/tarandm_analytics/export_predictive_model/__pycache__/create_predictive_model.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `tarandm_analytics-0.0.6/tarandm_analytics/export_predictive_model/__pycache__/model_visualization.cpython-310.pyc` & `tarandm_analytics-0.0.7/tarandm_analytics/export_predictive_model/__pycache__/model_visualization.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `tarandm_analytics-0.0.6/tarandm_analytics/export_predictive_model/create_predictive_model.py` & `tarandm_analytics-0.0.7/tarandm_analytics/export_predictive_model/create_predictive_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 from tarandm_analytics.export_predictive_model.model_visualization import (
     shap_summary_plot_logistic_regression,
     shap_summary_plot_xgboost,
     shap_summary_plot_random_forest,
     learning_curves_plot,
 )
-from tarandm_analytics.base import TaranDMAnalytics
+from tarandm_analytics.base_class import TaranDMAnalytics
 from tarandm_analytics.utils import get_number_formatting
 
 logger = structlog.get_logger(__name__)
 
 
 class ExportPredictiveModel(TaranDMAnalytics):
     supported_model_types = ["XGB", "LOGISTIC_REGRESSION", "RANDOM_FOREST", "EXPERT_SCORE"]
```

### Comparing `tarandm_analytics-0.0.6/tarandm_analytics/export_predictive_model/model_visualization.py` & `tarandm_analytics-0.0.7/tarandm_analytics/export_predictive_model/model_visualization.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,16 @@
         plot_type="bar",
     )
 
     ax = plt.gca()
     ax.tick_params(labelsize=14)
     ax.set_xlabel("mean(|SHAP value|) (average impact on model output magnitude)", fontsize=12)
 
-    ax.get_legend().remove()
+    if ax.get_legend():
+        ax.get_legend().remove()
 
     image_stream = BytesIO()
     plt.savefig(image_stream, format="svg", bbox_inches="tight")
     plt.close()
 
     return image_stream
```

### Comparing `tarandm_analytics-0.0.6/PKG-INFO` & `tarandm_analytics-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tarandm-analytics
-Version: 0.0.6
+Version: 0.0.7
 Summary: Package contains support functions for creating predictive models in format compatible with TaranDM software.
 Author: Marek Teller
 Author-email: mteller@taran.ai
 Requires-Python: >=3.10,<3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: llvmlite
```

