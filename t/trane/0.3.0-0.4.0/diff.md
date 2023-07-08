# Comparing `tmp/trane-0.3.0.tar.gz` & `tmp/trane-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trane-0.3.0.tar", last modified: Sun Feb 26 02:16:08 2023, max compression
+gzip compressed data, was "trane-0.4.0.tar", last modified: Sat Jul  8 21:53:52 2023, max compression
```

## Comparing `trane-0.3.0.tar` & `trane-0.4.0.tar`

### file list

```diff
@@ -1,36 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-26 02:16:08.060114 trane-0.3.0/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1076 2023-02-26 02:15:51.000000 trane-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8241 2023-02-26 02:16:08.060114 trane-0.3.0/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)     6737 2023-02-26 02:15:51.000000 trane-0.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3138 2023-02-26 02:15:51.000000 trane-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-26 02:16:08.060114 trane-0.3.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-26 02:16:08.056114 trane-0.3.0/trane/
--rwxr-xr-x   0 runner    (1001) docker     (123)      216 2023-02-26 02:15:51.000000 trane-0.3.0/trane/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-26 02:16:08.060114 trane-0.3.0/trane/core/
--rwxr-xr-x   0 runner    (1001) docker     (123)      301 2023-02-26 02:15:51.000000 trane-0.3.0/trane/core/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1885 2023-02-26 02:15:51.000000 trane-0.3.0/trane/core/cutoff_strategy.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3062 2023-02-26 02:15:51.000000 trane-0.3.0/trane/core/labeler.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    16267 2023-02-26 02:15:51.000000 trane-0.3.0/trane/core/prediction_problem.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9565 2023-02-26 02:15:51.000000 trane-0.3.0/trane/core/prediction_problem_evaluator.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8146 2023-02-26 02:15:51.000000 trane-0.3.0/trane/core/prediction_problem_generator.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2839 2023-02-26 02:15:51.000000 trane-0.3.0/trane/core/prediction_problem_saver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-26 02:16:08.060114 trane-0.3.0/trane/ops/
--rwxr-xr-x   0 runner    (1001) docker     (123)      173 2023-02-26 02:15:51.000000 trane-0.3.0/trane/ops/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4102 2023-02-26 02:15:51.000000 trane-0.3.0/trane/ops/aggregation_ops.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2698 2023-02-26 02:15:51.000000 trane-0.3.0/trane/ops/filter_ops.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10692 2023-02-26 02:15:51.000000 trane-0.3.0/trane/ops/op_base.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1176 2023-02-26 02:15:51.000000 trane-0.3.0/trane/ops/op_saver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-26 02:16:08.060114 trane-0.3.0/trane/utils/
--rwxr-xr-x   0 runner    (1001) docker     (123)      235 2023-02-26 02:15:51.000000 trane-0.3.0/trane/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3375 2023-02-26 02:15:51.000000 trane-0.3.0/trane/utils/data_parser.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      504 2023-02-26 02:15:51.000000 trane-0.3.0/trane/utils/evaluate_tool.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1551 2023-02-26 02:15:51.000000 trane-0.3.0/trane/utils/featuretools_wrapper.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      213 2023-02-26 02:15:51.000000 trane-0.3.0/trane/utils/helper.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5155 2023-02-26 02:15:51.000000 trane-0.3.0/trane/utils/table_meta.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-02-26 02:15:51.000000 trane-0.3.0/trane/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-26 02:16:08.056114 trane-0.3.0/trane.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8241 2023-02-26 02:16:08.000000 trane-0.3.0/trane.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-02-26 02:16:08.000000 trane-0.3.0/trane.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-26 02:16:08.000000 trane-0.3.0/trane.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-02-26 02:16:08.000000 trane-0.3.0/trane.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-02-26 02:16:08.000000 trane-0.3.0/trane.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 21:53:52.792954 trane-0.4.0/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1076 2023-07-08 21:53:36.000000 trane-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4378 2023-07-08 21:53:52.792954 trane-0.4.0/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2875 2023-07-08 21:53:36.000000 trane-0.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3181 2023-07-08 21:53:36.000000 trane-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 21:53:52.792954 trane-0.4.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 21:53:52.788954 trane-0.4.0/trane/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      383 2023-07-08 21:53:36.000000 trane-0.4.0/trane/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 21:53:52.792954 trane-0.4.0/trane/core/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      197 2023-07-08 21:53:36.000000 trane-0.4.0/trane/core/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      494 2023-07-08 21:53:36.000000 trane-0.4.0/trane/core/cutoff_strategy.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3123 2023-07-08 21:53:36.000000 trane-0.4.0/trane/core/labeler.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9443 2023-07-08 21:53:36.000000 trane-0.4.0/trane/core/prediction_problem.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8038 2023-07-08 21:53:36.000000 trane-0.4.0/trane/core/prediction_problem_evaluator.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7909 2023-07-08 21:53:36.000000 trane-0.4.0/trane/core/prediction_problem_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4247 2023-07-08 21:53:36.000000 trane-0.4.0/trane/core/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 21:53:52.792954 trane-0.4.0/trane/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-07-08 21:53:36.000000 trane-0.4.0/trane/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3904 2023-07-08 21:53:36.000000 trane-0.4.0/trane/datasets/load_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 21:53:52.792954 trane-0.4.0/trane/ops/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      131 2023-07-08 21:53:36.000000 trane-0.4.0/trane/ops/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3611 2023-07-08 21:53:36.000000 trane-0.4.0/trane/ops/aggregation_ops.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2665 2023-07-08 21:53:36.000000 trane-0.4.0/trane/ops/filter_ops.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2965 2023-07-08 21:53:36.000000 trane-0.4.0/trane/ops/op_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-07-08 21:53:36.000000 trane-0.4.0/trane/ops/threshold_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 21:53:36.000000 trane-0.4.0/trane/ops/threshold_functions.test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 21:53:52.792954 trane-0.4.0/trane/typing/
+-rw-r--r--   0 runner    (1001) docker     (123)     5840 2023-07-08 21:53:36.000000 trane-0.4.0/trane/typing/1-1000.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-07-08 21:53:36.000000 trane-0.4.0/trane/typing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-07-08 21:53:36.000000 trane-0.4.0/trane/typing/column_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-07-08 21:53:36.000000 trane-0.4.0/trane/typing/inference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7113 2023-07-08 21:53:36.000000 trane-0.4.0/trane/typing/inference_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-07-08 21:53:36.000000 trane-0.4.0/trane/typing/logical_types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 21:53:52.792954 trane-0.4.0/trane/utils/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      301 2023-07-08 21:53:36.000000 trane-0.4.0/trane/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2509 2023-07-08 21:53:36.000000 trane-0.4.0/trane/utils/data_parser.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1861 2023-07-08 21:53:36.000000 trane-0.4.0/trane/utils/featuretools_wrapper.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1254 2023-07-08 21:53:36.000000 trane-0.4.0/trane/utils/helper.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5495 2023-07-08 21:53:36.000000 trane-0.4.0/trane/utils/table_meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-08 21:53:36.000000 trane-0.4.0/trane/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 21:53:52.788954 trane-0.4.0/trane.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4378 2023-07-08 21:53:52.000000 trane-0.4.0/trane.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-07-08 21:53:52.000000 trane-0.4.0/trane.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 21:53:52.000000 trane-0.4.0/trane.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-08 21:53:52.000000 trane-0.4.0/trane.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-08 21:53:52.000000 trane-0.4.0/trane.egg-info/top_level.txt
```

### Comparing `trane-0.3.0/LICENSE` & `trane-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trane-0.3.0/pyproject.toml` & `trane-0.4.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -30,20 +30,20 @@
 ]
 keywords = ["trane", "data science", "machine learning"]
 license = {text = "MIT License"}
 requires-python = ">=3.8,<4"
 dependencies = [
     "numpy >= 1.13.0",
     "pandas >= 0.21.0",
-    "dill >= 0.2.8.2",
     "scipy >= 1.0.0",
     "composeml >= 0.10.1",
     "featuretools",
     "scikit-learn",
-    "tqdm"
+    "tqdm",
+    "ipywidgets",
 ]
 
 [project.urls]
 "Source Code"= "https://github.com/HDI-Project/Trane/"
 "Changes" = "https://github.com/HDI-Project/Trane/blob/main/docs/changelog.md"
 "Issue Tracker" = "https://github.com/HDI-Project/Trane/issues"
 "Twitter" = "https://twitter.com/lab_dai"
@@ -52,15 +52,15 @@
 test = [
     "pytest >= 3.4.2",
     "pytest-cov >= 2.5.1",
     "pytest-xdist >= 3.1.0",
     "pytest-runner >= 2.11.1",
 ]
 dev = [
-    "ruff >= 0.0.218" ,
+    "ruff >= 0.0.260" ,
     "black[jupyter] >= 22.12.0",
     "pre-commit == 2.20.0",
 ]
 
 [tool.setuptools]
 include-package-data = true
 license-files = [
@@ -111,16 +111,21 @@
 [build-system]
 requires = [
     "setuptools >= 61.0.0",
     "wheel"
 ]
 build-backend = "setuptools.build_meta"
 
+[tool.black]
+line-length = 88
+target-version = ["py311"]
+
 [tool.ruff]
-# Never enforce `E501` (line length violations), lines cannot be > 79 chars
+# Never enforce `E501` (line length violations)
+line-length = 88
 ignore = ["E501"]
 exclude = [
     "Examples",
 ]
 select = [
     # Pyflakes
     "F",
```

### Comparing `trane-0.3.0/trane/core/labeler.py` & `trane-0.4.0/trane/core/labeler.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,84 +1,80 @@
-import copy
-
-from trane.utils.table_meta import TableMeta as TM
-
 __all__ = ["Labeler"]
 
 
 class Labeler:
     """
     Object for executing prediction problems on data in order
     to generate labels for many prediction problems.
     The execute method performs the labelling operation.
     """
 
-    def __init__(self, df, entity_col, cutoff_strategy, sample=2000):
-        self.df = df
-        self.sampled_df = df.sample(sample)
-        self.entity_col = entity_col
-        self.cutoff_strategy = cutoff_strategy
-
-    def threshold_recommend(self, problem):
-        filter_op = problem.operations[0]
-        if len(filter_op.REQUIRED_PARAMETERS) == 0:
-            yield copy.deepcopy(problem), "no threshold"
-        else:
-            if filter_op.input_type == TM.TYPE_CATEGORY:
-                for item in self._categorical_threshold(
-                    self.sampled_df[filter_op.column_name],
-                ):
-                    problem_final = copy.deepcopy(problem)
-                    problem_final.operations[0].set_hyper_parameter(
-                        parameter_name="threshold",
-                        parameter_value=item,
-                    )
-                    yield problem_final, "threshold: {}".format(item)
-            elif filter_op.input_type in [TM.TYPE_FLOAT, TM.TYPE_INTEGER]:
-                for keep_rate in [0.25, 0.5, 0.75]:
-                    threshold = filter_op.find_threshhold_by_remaining(
-                        fraction_of_data_target=keep_rate,
-                        df=self.sampled_df,
-                        col=filter_op.column_name,
-                    )
-                    problem_final = copy.deepcopy(problem)
-                    problem_final.operations[0].set_hyper_parameter(
-                        parameter_name="threshold",
-                        parameter_value=threshold,
-                    )
-                    yield problem_final, "threshold: {} (keep {}%)".format(
-                        threshold,
-                        keep_rate * 100,
-                    )
-
-    def execute(self, problem, entity_id_column):
-        """
-        Generate the labels.
-
-        Parameters
-        ----------
-        cutoff_df: dataframe. Each row corresponds to an entity.
-            entity_id (indexed) | training_cutoff | test_cutoff
-        json_prediction_problems_filename: filename to read
-            prediction problems from, structured in JSON.
-
-        Returns
-        -------
-        dfs: a list of DataFrames. One dataframe for each problem.
-            Each dataframe contains entities, cutoff times and labels.
-
-        """
-        dfs = []
-        _ = [
-            entity_id_column,
-            "training_labels",
-            "test_labels",
-            "training_cutoff_time",
-            "label_cutoff_time",
-        ]
-        for problem_final, threshold_description in self.threshold_recommend(problem):
-            problem_final.cutoff_strategy = self.cutoff_strategy
-            labels = problem_final.execute(self.df)
+    # def __init__(self, df, entity_col, cutoff_strategy, sample=2000):
+    #     self.df = df
+    #     self.sampled_df = df.sample(sample)
+    #     self.entity_col = entity_col
+    #     self.cutoff_strategy = cutoff_strategy
+
+    # def threshold_recommend(self, problem):
+    #     filter_op = problem.operations[0]
+    #     if len(filter_op.REQUIRED_PARAMETERS) == 0:
+    #         yield copy.deepcopy(problem), "no threshold"
+    #     else:
+    #         if filter_op.input_type == TM.TYPE_CATEGORY:
+    #             for item in self._categorical_threshold(
+    #                 self.sampled_df[filter_op.column_name],
+    #             ):
+    #                 problem_final = copy.deepcopy(problem)
+    #                 problem_final.operations[0].set_hyper_parameter(
+    #                     parameter_name="threshold",
+    #                     parameter_value=item,
+    #                 )
+    #                 yield problem_final, "threshold: {}".format(item)
+    #         elif filter_op.input_type in [TM.TYPE_FLOAT, TM.TYPE_INTEGER]:
+    #             for keep_rate in [0.25, 0.5, 0.75]:
+    #                 threshold = filter_op.find_threshhold_by_remaining(
+    #                     fraction_of_data_target=keep_rate,
+    #                     df=self.sampled_df,
+    #                     col=filter_op.column_name,
+    #                 )
+    #                 problem_final = copy.deepcopy(problem)
+    #                 problem_final.operations[0].set_hyper_parameter(
+    #                     parameter_name="threshold",
+    #                     parameter_value=threshold,
+    #                 )
+    #                 yield problem_final, "threshold: {} (keep {}%)".format(
+    #                     threshold,
+    #                     keep_rate * 100,
+    #                 )
+
+    # def execute(self, problem, entity_id_column):
+    #     """
+    #     Generate the labels.
+
+    #     Parameters
+    #     ----------
+    #     cutoff_df: dataframe. Each row corresponds to an entity.
+    #         entity_id (indexed) | training_cutoff | test_cutoff
+    #     json_prediction_problems_filename: filename to read
+    #         prediction problems from, structured in JSON.
+
+    #     Returns
+    #     -------
+    #     dfs: a list of DataFrames. One dataframe for each problem.
+    #         Each dataframe contains entities, cutoff times and labels.
+
+    #     """
+    #     dfs = []
+    #     _ = [
+    #         entity_id_column,
+    #         "training_labels",
+    #         "test_labels",
+    #         "training_cutoff_time",
+    #         "label_cutoff_time",
+    #     ]
+    #     for problem_final, threshold_description in self.threshold_recommend(problem):
+    #         problem_final.cutoff_strategy = self.cutoff_strategy
+    #         labels = problem_final.execute(self.df)
 
-            dfs.append([self.df, labels])
+    #         dfs.append([self.df, labels])
 
-        return dfs
+    #     return dfs
```

### Comparing `trane-0.3.0/trane/core/prediction_problem_evaluator.py` & `trane-0.4.0/trane/core/prediction_problem_evaluator.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,18 +3,14 @@
 import numpy as np
 from sklearn.ensemble import AdaBoostClassifier, AdaBoostRegressor
 from sklearn.linear_model import LinearRegression
 from sklearn.neighbors import KNeighborsClassifier
 from sklearn.preprocessing import OneHotEncoder
 from sklearn.tree import DecisionTreeClassifier, DecisionTreeRegressor
 
-from trane.utils.table_meta import TableMeta as TM
-
-__all__ = ["PredictionProblemEvaluator"]
-
 
 class PredictionProblemEvaluator(object):
     """docstring for PredictionProblemEvaluator."""
 
     def __init__(
         self,
         df,
@@ -100,46 +96,14 @@
                 counter[item] = 1
 
         counter_tuple = list(counter.items())
         counter_tuple = sorted(counter_tuple, key=lambda x: -x[1])
         counter_tuple = counter_tuple[:3]
         return [item[0] for item in counter_tuple]
 
-    def threshold_recommend(self, problem):
-        filter_op = problem.operations[0]
-        if len(filter_op.REQUIRED_PARAMETERS) == 0:
-            yield copy.deepcopy(problem), "no threshold"
-        else:
-            if filter_op.input_type == TM.TYPE_CATEGORY:
-                for item in self._categorical_threshold(
-                    self.sampled_df[filter_op.column_name],
-                ):
-                    problem_final = copy.deepcopy(problem)
-                    problem_final.operations[0].set_hyper_parameter(
-                        parameter_name="threshold",
-                        parameter_value=item,
-                    )
-                    yield problem_final, "threshold: {}".format(item)
-            elif filter_op.input_type in [TM.TYPE_FLOAT, TM.TYPE_INTEGER]:
-                for keep_rate in [0.25, 0.5, 0.75]:
-                    threshold = filter_op.find_threshhold_by_remaining(
-                        fraction_of_data_target=keep_rate,
-                        df=self.sampled_df,
-                        col=filter_op.column_name,
-                    )
-                    problem_final = copy.deepcopy(problem)
-                    problem_final.operations[0].set_hyper_parameter(
-                        parameter_name="threshold",
-                        parameter_value=threshold,
-                    )
-                    yield problem_final, "threshold: {} (keep {}%)".format(
-                        threshold,
-                        keep_rate * 100,
-                    )
-
     def split_dataset(self, problem, problem_type, labels, features):
         X_train, X_test, Y_train, Y_test = [], [], [], []
 
         entity_names = set(labels.index.get_level_values(problem.entity_col))
 
         if problem_type == "classification":
             label_to_index = dict(
@@ -187,20 +151,22 @@
             enc.fit(X_train + X_test)
             X_train = enc.transform(X_train)
             X_test = enc.transform(X_test)
 
         return X_train, X_test, Y_train, Y_test
 
     def evaluate(self, problem, features, labels):
-        if problem.label_type in [TM.TYPE_INTEGER, TM.TYPE_FLOAT]:
-            problem_type = "regression"
-        elif problem.label_type in [TM.TYPE_CATEGORY, TM.TYPE_IDENTIFIER]:
-            problem_type = "classification"
-        else:
-            return {"status": "fail", "description": "unknown problem type"}
+        # totally wrong, just for testing
+        problem_type = "regression"
+        # if problem.label_type in [TM.TYPE_INTEGER, TM.TYPE_FLOAT]:
+        #     problem_type = "regression"
+        # elif problem.label_type in [TM.TYPE_CATEGORY, TM.TYPE_IDENTIFIER]:
+        #     problem_type = "classification"
+        # else:
+        #     return {"status": "fail", "description": "unknown problem type"}
 
         template_res = {"problem_type": problem_type, "template_nl": str(problem)}
         evaluations = []
         # for problem_final, threshold_description in self.threshold_recommend(problem):
         problem_final = problem
         problem_final.cutoff_strategy = self.cutoff_strategy
         labels = labels  # problem_final.execute(self.df)
```

### Comparing `trane-0.3.0/trane/core/prediction_problem_generator.py` & `trane-0.4.0/trane/core/prediction_problem_generator.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,212 +1,222 @@
 import copy
 import itertools
 
+from tqdm.notebook import tqdm
+
 from trane.core.prediction_problem import PredictionProblem
+from trane.core.utils import _parse_table_meta, get_semantic_tags
 from trane.ops import aggregation_ops as agg_ops
 from trane.ops import filter_ops
-from trane.utils.table_meta import TableMeta
+from trane.ops.filter_ops import AllFilterOp
+from trane.ops.threshold_functions import get_k_most_frequent
+from trane.typing.column_schema import ColumnSchema
+from trane.typing.inference import infer_table_meta
+from trane.typing.logical_types import (
+    Categorical,
+    Datetime,
+    Integer,
+)
 
 __all__ = ["PredictionProblemGenerator"]
 
 
 class PredictionProblemGenerator:
     """
     Object for generating prediction problems on data.
     """
 
-    def __init__(self, table_meta, entity_col, time_col, cutoff_strategy=None):
+    def __init__(self, df, entity_col, time_col, table_meta=None, cutoff_strategy=None):
         """
         Parameters
         ----------
-        table_meta: TableMeta object. Contains
-            meta information about the data
+        table_meta: a dictionary containing typing information about the data
         entity_col: column name of
             the column containing entities in the data
-        label_col: column name of the
-            column of interest in the data
         time_col: column name of the column
             containing time information in the data
-        filter_col: column name of the column
-            to be filtered over
 
         Returns
         -------
         None
         """
-        self.table_meta = table_meta
+        self.df = df
         self.entity_col = entity_col
         self.time_col = time_col
         self.cutoff_strategy = cutoff_strategy
-        self.ensure_valid_inputs()
 
-    def generate(self, df_sample=None, generate_thresholds=False, n_problems=None):
+        inferred_table_meta = False
+        if table_meta is None:
+            self.table_meta = infer_table_meta(df)
+            inferred_table_meta = True
+        else:
+            self.table_meta = _parse_table_meta(table_meta)
+        self.transform_data()
+        self.ensure_valid_inputs(inferred_table_meta)
+
+    def ensure_valid_inputs(self, inferred_table_meta=False):
+        """
+        TypeChecking for the problem generator entity_col
+        and label_col. Errors if types don't match up.
+        """
+        for col, column_schema in self.table_meta.items():
+            assert isinstance(col, str)
+            assert isinstance(column_schema, ColumnSchema)
+            assert col in self.df.columns
+            assert column_schema.logical_type.dtype == str(self.df[col].dtype)
+
+        entity_col_type = self.table_meta[self.entity_col]
+        assert entity_col_type.logical_type in [Integer, Categorical]
+        if inferred_table_meta is False:
+            assert "index" in entity_col_type.semantic_tags
+        else:
+            self.table_meta[self.entity_col].semantic_tags.add("index")
+
+        time_col_type = self.table_meta[self.time_col]
+        assert time_col_type.logical_type == Datetime
+
+    def transform_data(self):
+        """
+        Transform the data to the correct types.
+        """
+        for col, column_schema in self.table_meta.items():
+            expected_logical_type = column_schema.logical_type
+            if self.df[col].dtype != expected_logical_type.dtype:
+                self.df[col] = expected_logical_type().transform(series=self.df[col])
+
+    def generate(
+        self,
+        df,
+        generate_thresholds=False,
+        n_problems=None,
+        pbar_position=0,
+    ):
         """
         Generate the prediction problems. The prediction problems operations
         hyper parameters are also set.
 
         Parameters
         ----------
-        df_sample (optional, pd.DataFrame): Dataframe sample to use to generate relevant thresholds.
-            Defaults to None (does not automatically generate thresholds).
+        df (pd.DataFrame): Dataframe to use to generate relevant thresholds. You could use a sample of the
+            dataframe to speed up the process.
         generate_thresholds (optional, bool): Whether to automatically generate thresholds for problems.
             Defaults to False.
         n_problems (optional, int): Maximum number of problems to generate. Defaults to generating all possible
             problems.
 
         Returns
         -------
         problems: a list of Prediction Problem objects.
         """
-        if generate_thresholds and df_sample is None:
+        if generate_thresholds and df is None:
             raise ValueError("Must provide a dataframe sample to generate thresholds")
 
         # a list of problems that will eventually be returned
         problems = []
+        all_columns = list(self.table_meta.keys())
 
-        def iter_over_ops():
-            for ag, filter in itertools.product(
-                agg_ops.AGGREGATION_OPS,
-                filter_ops.FILTER_OPS,
+        possible_ops = []
+        for agg, filter_ in itertools.product(
+            agg_ops.AGGREGATION_OPS,
+            filter_ops.FILTER_OPS,
+        ):
+            filter_columns = all_columns
+            if filter_ == "AllFilterOp":
+                filter_columns = [None]
+
+            agg_columns = all_columns
+            if agg == "CountAggregationOp":
+                agg_columns = [None]
+            for filter_col, agg_col in itertools.product(
+                filter_columns,
+                agg_columns,
             ):
-
-                filter_cols = (
-                    [None] if filter == "AllFilterOp" else self.table_meta.get_columns()
-                )
-                ag_cols = (
-                    [None]
-                    if ag == "CountAggregationOp"
-                    else self.table_meta.get_columns()
-                )
-
-                for filter_col, ag_col in itertools.product(filter_cols, ag_cols):
-                    if filter_col != self.entity_col and ag_col != self.entity_col:
-                        yield ag_col, filter_col, ag, filter
-
-        from tqdm import tqdm
-
-        # might be inefficent
-        total_attempts = sum(1 for _ in iter_over_ops())
+                if filter_col == self.time_col or agg_col == self.time_col:
+                    continue
+                if filter_col != self.entity_col and agg_col != self.entity_col:
+                    possible_ops.append((agg_col, filter_col, agg, filter_))
+        total_attempts = len(possible_ops)
         all_attempts = 0
         success_attempts = 0
-        for op_col_combo in tqdm(iter_over_ops(), total=total_attempts):
-            # for op_col_combo in iter_over_ops():
-            print(
-                "\rSuccess/Attempt = {}/{}".format(success_attempts, all_attempts),
-                end="",
-            )
+        for op_col_combo in tqdm(
+            possible_ops,
+            total=total_attempts,
+            position=pbar_position,
+        ):
             all_attempts += 1
             ag_col, filter_col, agg_op_name, filter_op_name = op_col_combo
 
             agg_op_obj = getattr(agg_ops, agg_op_name)(ag_col)  # noqa
             filter_op_obj = getattr(filter_ops, filter_op_name)(filter_col)  # noqa
 
+            # Note: the order of the operations matters, the filter operation must be first
             operations = [filter_op_obj, agg_op_obj]
 
             problem = PredictionProblem(
                 operations=operations,
                 entity_col=self.entity_col,
                 time_col=self.time_col,
                 table_meta=self.table_meta,
                 cutoff_strategy=self.cutoff_strategy,
             )
-
-            if problem.is_valid() and generate_thresholds:
-                for final_problem, _ in self._threshold_recommend(problem, df_sample):
-                    problems.append(final_problem)
+            if problem.is_valid() and generate_thresholds is True:
+                filter_op = problem.operations[0]
+                if isinstance(filter_op, AllFilterOp):
+                    # the filter operation does not require a threshold
+                    problems.append(problem)
                     success_attempts += 1
+                else:
+                    yielded_thresholds = self._threshold_recommend(filter_op, df)
+                    for threshold in yielded_thresholds:
+                        final_problem = copy.deepcopy(problem)
+                        final_problem.operations[0].set_parameters(
+                            threshold=threshold,
+                        )
+                        problems.append(final_problem)
+                        success_attempts += 1
             elif problem.is_valid():
                 problems.append(problem)
                 success_attempts += 1
             if n_problems and success_attempts >= n_problems:
                 break
-
-        print("\rSuccess/Attempt = {}/{}".format(success_attempts, all_attempts))
         return problems
 
-    def generate_thresholds(self, problems, df_sample):
-        """
-        Generate thresholds for all problems in a list of prediction problems if
-        thresholds can be generated for them.
+    def _threshold_recommend(self, filter_op, df):
+        yielded_thresholds = []
+        valid_semantic_tags = get_semantic_tags(filter_op)
 
-        Parameters
-        ----------
-        problems: a list of Prediction Problem objects that may need thresholds
-        to be set
-        df_sample: a sample of the dataframe that will be used to execute the
-        prediction problems to generate thresholds from
+        if "category" in valid_semantic_tags:
+            yielded_thresholds = recommend_categorical_thresholds(
+                df,
+                filter_op,
+            )
+        elif "numeric" in valid_semantic_tags:
+            yielded_thresholds = recommend_numeric_thresholds(
+                df=df,
+                filter_op=filter_op,
+            )
+        return yielded_thresholds
 
-        Returns
-        -------
-        problems: a list of Prediction Problem objects with thresholds set or the
-        original problem if no thresholds are needed.
-        """
-        final_problems = []
-        for problem in problems:
-            for final_problem, _ in self._threshold_recommend(problem, df_sample):
-                final_problems.append(final_problem)
-        return final_problems
 
-    def ensure_valid_inputs(self):
-        """
-        TypeChecking for the problem generator entity_col
-        and label_col. Errors if types don't match up.
-        """
-        assert self.table_meta.get_type(self.entity_col) in [
-            TableMeta.TYPE_IDENTIFIER,
-            TableMeta.TYPE_TEXT,
-            TableMeta.TYPE_CATEGORY,
-        ]
-
-    def _categorical_threshold(self, df_col, k=3):
-        counter = {}
-        for item in df_col:
-            try:
-                counter[item] += 1
-            except BaseException:
-                counter[item] = 1
-
-        counter_tuple = list(counter.items())
-        counter_tuple = sorted(counter_tuple, key=lambda x: -x[1])
-        counter_tuple = counter_tuple[:3]
-        return [item[0] for item in counter_tuple]
-
-    def _threshold_recommend(self, problem, df_sample):
-        yielded_thresholds = []
-        filter_op = problem.operations[0]
-        if len(filter_op.REQUIRED_PARAMETERS) == 0:
-            yield copy.deepcopy(problem), "no threshold"
-        else:
-            if filter_op.input_type == TableMeta.TYPE_CATEGORY:
-                for item in self._categorical_threshold(
-                    df_sample[filter_op.column_name],
-                ):
-                    if item not in yielded_thresholds:
-                        yielded_thresholds.append(item)
-                        problem_final = copy.deepcopy(problem)
-                        problem_final.operations[0].set_hyper_parameter(
-                            parameter_name="threshold",
-                            parameter_value=item,
-                        )
-                        yield problem_final, "threshold: {}".format(item)
-                    else:
-                        continue
-            elif filter_op.input_type in [TableMeta.TYPE_FLOAT, TableMeta.TYPE_INTEGER]:
-                for keep_rate in [0.25, 0.5, 0.75]:
-                    threshold = filter_op.find_threshhold_by_remaining(
-                        fraction_of_data_target=keep_rate,
-                        df=df_sample,
-                        col=filter_op.column_name,
-                    )
-                    if threshold not in yielded_thresholds:
-                        yielded_thresholds.append(threshold)
-                        problem_final = copy.deepcopy(problem)
-                        problem_final.operations[0].set_hyper_parameter(
-                            parameter_name="threshold",
-                            parameter_value=threshold,
-                        )
-                        yield problem_final, "threshold: {} (keep {}%)".format(
-                            threshold,
-                            keep_rate * 100,
-                        )
-                    else:
-                        continue
+def recommend_categorical_thresholds(df, filter_op, k=3):
+    thresholds = get_k_most_frequent(
+        df[filter_op.column_name],
+        k=k,
+    )
+    thresholds = list(set(thresholds))
+    return thresholds
+
+
+def recommend_numeric_thresholds(
+    df,
+    filter_op,
+    keep_rates=[0.25, 0.5, 0.75],
+):
+    thresholds = []
+    for keep_rate in keep_rates:
+        threshold = filter_op.find_threshold_by_fraction_of_data_to_keep(
+            fraction_of_data_target=keep_rate,
+            df=df,
+            label_col=filter_op.column_name,
+        )
+        thresholds.append(threshold)
+    return thresholds
```

### Comparing `trane-0.3.0/trane/utils/data_parser.py` & `trane-0.4.0/trane/utils/data_parser.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,15 +1,9 @@
-from datetime import datetime
-
 import pandas as pd
 
-from trane.utils.table_meta import TableMeta as TM
-
-__all__ = ["denormalize", "parse_data"]
-
 
 class CsvMerge:
     """
     Simple class for helping with csv merge operations.
     """
 
     def __init__(self, csv_names, data):
@@ -83,33 +77,7 @@
             csv_merge_objs.remove(child_merge_obj)
 
         csv_merge_objs.append(new_merge_obj)
 
     assert len(csv_merge_objs) == 1
 
     return csv_merge_objs[0].get_data()
-
-
-def parse_data(dataframe, table_meta):
-    """
-    Convert columns specified as time in the table_meta from str objects to datetime objects.
-
-    Parameters
-    ----------
-    dataframe: the data
-    table_meta: a TableMeta object specifying meta information about the data
-
-    Returns
-    ----------
-    dataframe: with time columns converted from str to datetime.
-    """
-
-    columns = table_meta.get_columns()
-    for column in columns:
-        if table_meta.get_type(column) == TM.TYPE_TIME:
-            dataframe[column] = dataframe[column].apply(
-                lambda x: datetime.strptime(
-                    x,
-                    table_meta.get_property(column, "format"),
-                ),
-            )
-    return dataframe
```

### Comparing `trane-0.3.0/trane/utils/featuretools_wrapper.py` & `trane-0.4.0/trane/utils/featuretools_wrapper.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,49 +5,54 @@
 
 __all__ = ["FeaturetoolsWrapper"]
 
 
 class FeaturetoolsWrapper(object):
     """docstring for FeaturetoolsWrapper."""
 
-    def __init__(self, df, entity_col, time_col, name):
+    def __init__(self, df, entity_col, time_col, name, logical_types=None):
         assert name != entity_col
 
         self.entity_col = entity_col
         self.es = ft.EntitySet(id=name)
         self.es = self.es.add_dataframe(
             dataframe_name=name,
             dataframe=df,
             time_index=time_col,
             index="__id__",
             make_index=True,
+            logical_types=logical_types,
         )
 
-        entity_df = pd.DataFrame(
-            [[i] for i in set(df[entity_col])],
-            columns=[entity_col],
-        )
+        entity_df = pd.Series(df[entity_col].unique(), name=entity_col).to_frame()
+        # entity_df = pd.DataFrame(
+        #     [[i] for i in set(df[entity_col])],
+        #     columns=[entity_col],
+        # )
         self.es = self.es.add_dataframe(
             dataframe_name=entity_col,
             dataframe=entity_df,
             index=entity_col,
         )
 
         self.es = self.es.add_relationship(entity_col, entity_col, name, entity_col)
 
-    def compute_features(self, df, cutoff_df, feature_window):
+    def compute_features(self, cutoff_strategy, feature_window):
         feature_matrix, features = ft.dfs(
-            target_dataframe_index=self.entity_col,
-            cutoff_time=cutoff_df,
+            target_dataframe_name=self.entity_col,
+            cutoff_time=cutoff_strategy,
             entityset=self.es,
             cutoff_time_in_index=True,
             verbose=True,
         )
+        return feature_matrix, features
 
-        # encode categorical values
-        fm_encoded, features_encoded = ft.encode_features(feature_matrix, features)
-
-        features = fm_encoded.fillna(0)
-        return features
+    def encode_features(self, feature_matrix, features):
+        feature_matrix_encoded, features_encoded = ft.encode_features(
+            feature_matrix,
+            features,
+        )
+        features = feature_matrix_encoded.fillna(0)
+        return feature_matrix_encoded, features_encoded
 
     def get_feature(self, entity_name, cutoff_st):
         return list(self.features.loc[entity_name, cutoff_st - timedelta(days=1)])
```

