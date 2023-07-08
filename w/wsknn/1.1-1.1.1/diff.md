# Comparing `tmp/wsknn-1.1.tar.gz` & `tmp/wsknn-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wsknn-1.1.tar", last modified: Fri Mar 31 11:31:41 2023, max compression
+gzip compressed data, was "wsknn-1.1.1.tar", last modified: Sat Jul  8 11:31:22 2023, max compression
```

## Comparing `wsknn-1.1.tar` & `wsknn-1.1.1.tar`

### file list

```diff
@@ -1,66 +1,82 @@
-drwxrwxr-x   0 szymon    (1000) szymon    (1000)        0 2023-03-31 11:31:41.111921 wsknn-1.1/
--rw-rw-r--   0 szymon    (1000) szymon    (1000)     1532 2023-03-29 08:54:17.000000 wsknn-1.1/LICENSE.md
--rw-rw-r--   0 szymon    (1000) szymon    (1000)     8780 2023-03-31 11:31:41.111921 wsknn-1.1/PKG-INFO
--rw-rw-r--   0 szymon    (1000) szymon    (1000)     7664 2023-03-30 19:34:34.000000 wsknn-1.1/README.md
--rw-rw-r--   0 szymon    (1000) szymon    (1000)       80 2023-03-31 10:10:43.000000 wsknn-1.1/pyproject.toml
--rw-rw-r--   0 szymon    (1000) szymon    (1000)     1284 2023-03-31 11:31:41.111921 wsknn-1.1/setup.cfg
-drwxrwxr-x   0 szymon    (1000) szymon    (1000)        0 2023-03-31 11:31:41.107921 wsknn-1.1/tests/
--rw-rw-r--   0 szymon    (1000) szymon    (1000)      832 2023-03-29 08:54:18.000000 wsknn-1.1/tests/test_calc.py
--rw-rw-r--   0 szymon    (1000) szymon    (1000)      407 2023-03-29 08:54:18.000000 wsknn-1.1/tests/test_data_loading.py
--rw-rw-r--   0 szymon    (1000) szymon    (1000)      657 2023-03-29 08:54:18.000000 wsknn-1.1/tests/test_evaluation_metrics.py
--rw-rw-r--   0 szymon    (1000) szymon    (1000)     1043 2023-03-30 19:34:34.000000 wsknn-1.1/tests/test_get_larger_value.py
--rw-rw-r--   0 szymon    (1000) szymon    (1000)     1054 2023-03-30 19:34:34.000000 wsknn-1.1/tests/test_get_smaller_value.py
--rw-rw-r--   0 szymon    (1000) szymon    (1000)     8076 2023-03-30 19:34:34.000000 wsknn-1.1/tests/test_items_class.py
--rw-rw-r--   0 szymon    (1000) szymon    (1000)     2216 2023-03-30 19:34:34.000000 wsknn-1.1/tests/test_merge_dicts.py
--rw-rw-r--   0 szymon    (1000) szymon    (1000)     5587 2023-03-30 19:34:34.000000 wsknn-1.1/tests/test_parse.py
--rw-rw-r--   0 szymon    (1000) szymon    (1000)      761 2023-03-30 19:34:34.000000 wsknn-1.1/tests/test_parse_times.py
--rw-rw-r--   0 szymon    (1000) szymon    (1000)     6965 2023-03-30 19:34:34.000000 wsknn-1.1/tests/test_sessions_class.py
--rw-rw-r--   0 szymon    (1000) szymon    (1000)     2052 2023-03-29 08:54:18.000000 wsknn-1.1/tests/test_weighting.py
--rw-rw-r--   0 szymon    (1000) szymon    (1000)     3827 2023-03-29 08:54:18.000000 wsknn-1.1/tests/test_wsknn.py
-drwxrwxr-x   0 szymon    (1000) szymon    (1000)        0 2023-03-31 11:31:41.107921 wsknn-1.1/wsknn/
--rw-rw-r--   0 szymon    (1000) szymon    (1000)      195 2023-03-30 19:34:34.000000 wsknn-1.1/wsknn/__init__.py
-drwxrwxr-x   0 szymon    (1000) szymon    (1000)        0 2023-03-31 11:31:41.107921 wsknn-1.1/wsknn/evaluate/
--rw-rw-r--   0 szymon    (1000) szymon    (1000)      100 2023-03-29 08:54:18.000000 wsknn-1.1/wsknn/evaluate/__init__.py
--rw-rw-r--   0 szymon    (1000) szymon    (1000)    15180 2023-03-29 08:54:18.000000 wsknn-1.1/wsknn/evaluate/metrics.py
-drwxrwxr-x   0 szymon    (1000) szymon    (1000)        0 2023-03-31 11:31:41.107921 wsknn-1.1/wsknn/evaluate/scores/
--rw-rw-r--   0 szymon    (1000) szymon    (1000)       79 2023-03-29 08:54:18.000000 wsknn-1.1/wsknn/evaluate/scores/__init__.py
--rw-rw-r--   0 szymon    (1000) szymon    (1000)     2006 2023-03-29 08:54:18.000000 wsknn-1.1/wsknn/evaluate/scores/scores.py
--rw-rw-r--   0 szymon    (1000) szymon    (1000)     3283 2023-03-30 19:34:34.000000 wsknn-1.1/wsknn/evaluate/simulate.py
--rw-rw-r--   0 szymon    (1000) szymon    (1000)     4640 2023-03-29 08:54:18.000000 wsknn-1.1/wsknn/fit_transform.py
-drwxrwxr-x   0 szymon    (1000) szymon    (1000)        0 2023-03-31 11:31:41.107921 wsknn-1.1/wsknn/model/
--rw-rw-r--   0 szymon    (1000) szymon    (1000)        0 2023-03-29 08:54:18.000000 wsknn-1.1/wsknn/model/__init__.py
--rw-rw-r--   0 szymon    (1000) szymon    (1000)    31010 2023-03-29 08:54:18.000000 wsknn-1.1/wsknn/model/wsknn.py
--rw-rw-r--   0 szymon    (1000) szymon    (1000)     1535 2023-03-29 08:54:18.000000 wsknn-1.1/wsknn/predict.py
-drwxrwxr-x   0 szymon    (1000) szymon    (1000)        0 2023-03-31 11:31:41.107921 wsknn-1.1/wsknn/preprocessing/
--rw-rw-r--   0 szymon    (1000) szymon    (1000)        0 2023-03-30 19:34:34.000000 wsknn-1.1/wsknn/preprocessing/__init__.py
-drwxrwxr-x   0 szymon    (1000) szymon    (1000)        0 2023-03-31 11:31:41.107921 wsknn-1.1/wsknn/preprocessing/export/
--rw-rw-r--   0 szymon    (1000) szymon    (1000)        0 2023-03-30 19:34:34.000000 wsknn-1.1/wsknn/preprocessing/export/__init__.py
--rw-rw-r--   0 szymon    (1000) szymon    (1000)     1181 2023-03-30 19:34:34.000000 wsknn-1.1/wsknn/preprocessing/export/export.py
--rw-rw-r--   0 szymon    (1000) szymon    (1000)    12806 2023-03-30 19:34:34.000000 wsknn-1.1/wsknn/preprocessing/parse_static.py
-drwxrwxr-x   0 szymon    (1000) szymon    (1000)        0 2023-03-31 11:31:41.107921 wsknn-1.1/wsknn/preprocessing/structure/
--rw-rw-r--   0 szymon    (1000) szymon    (1000)        0 2023-03-30 19:34:34.000000 wsknn-1.1/wsknn/preprocessing/structure/__init__.py
--rw-rw-r--   0 szymon    (1000) szymon    (1000)    10796 2023-03-30 19:34:34.000000 wsknn-1.1/wsknn/preprocessing/structure/item.py
--rw-rw-r--   0 szymon    (1000) szymon    (1000)    13159 2023-03-30 19:34:34.000000 wsknn-1.1/wsknn/preprocessing/structure/session.py
-drwxrwxr-x   0 szymon    (1000) szymon    (1000)        0 2023-03-31 11:31:41.107921 wsknn-1.1/wsknn/preprocessing/utils/
--rw-rw-r--   0 szymon    (1000) szymon    (1000)        0 2023-03-30 19:34:34.000000 wsknn-1.1/wsknn/preprocessing/utils/__init__.py
--rw-rw-r--   0 szymon    (1000) szymon    (1000)      542 2023-03-30 19:34:34.000000 wsknn-1.1/wsknn/preprocessing/utils/calc.py
--rw-rw-r--   0 szymon    (1000) szymon    (1000)     5016 2023-03-30 19:34:34.000000 wsknn-1.1/wsknn/preprocessing/utils/files.py
--rw-rw-r--   0 szymon    (1000) szymon    (1000)     3793 2023-03-30 19:34:34.000000 wsknn-1.1/wsknn/preprocessing/utils/transform.py
-drwxrwxr-x   0 szymon    (1000) szymon    (1000)        0 2023-03-31 11:31:41.107921 wsknn-1.1/wsknn/utils/
--rw-rw-r--   0 szymon    (1000) szymon    (1000)      144 2023-03-29 08:54:18.000000 wsknn-1.1/wsknn/utils/__init__.py
--rw-rw-r--   0 szymon    (1000) szymon    (1000)     1337 2023-03-29 08:54:18.000000 wsknn-1.1/wsknn/utils/calc.py
--rw-rw-r--   0 szymon    (1000) szymon    (1000)     2561 2023-03-29 08:54:18.000000 wsknn-1.1/wsknn/utils/errors.py
--rw-rw-r--   0 szymon    (1000) szymon    (1000)      442 2023-03-29 08:54:18.000000 wsknn-1.1/wsknn/utils/meta.py
--rw-rw-r--   0 szymon    (1000) szymon    (1000)     1732 2023-03-29 08:54:18.000000 wsknn-1.1/wsknn/utils/transform.py
-drwxrwxr-x   0 szymon    (1000) szymon    (1000)        0 2023-03-31 11:31:41.111921 wsknn-1.1/wsknn/weighting/
--rw-rw-r--   0 szymon    (1000) szymon    (1000)       78 2023-03-29 08:54:18.000000 wsknn-1.1/wsknn/weighting/__init__.py
--rw-rw-r--   0 szymon    (1000) szymon    (1000)     1611 2023-03-29 08:54:18.000000 wsknn-1.1/wsknn/weighting/item_weighting.py
--rw-rw-r--   0 szymon    (1000) szymon    (1000)     2140 2023-03-29 08:54:18.000000 wsknn-1.1/wsknn/weighting/session_weighting.py
--rw-rw-r--   0 szymon    (1000) szymon    (1000)     1651 2023-03-29 08:54:18.000000 wsknn-1.1/wsknn/weighting/weighting.py
-drwxrwxr-x   0 szymon    (1000) szymon    (1000)        0 2023-03-31 11:31:41.107921 wsknn-1.1/wsknn.egg-info/
--rw-rw-r--   0 szymon    (1000) szymon    (1000)     8780 2023-03-31 11:31:41.000000 wsknn-1.1/wsknn.egg-info/PKG-INFO
--rw-rw-r--   0 szymon    (1000) szymon    (1000)     1429 2023-03-31 11:31:41.000000 wsknn-1.1/wsknn.egg-info/SOURCES.txt
--rw-rw-r--   0 szymon    (1000) szymon    (1000)        1 2023-03-31 11:31:41.000000 wsknn-1.1/wsknn.egg-info/dependency_links.txt
--rw-rw-r--   0 szymon    (1000) szymon    (1000)        1 2023-03-31 11:31:40.000000 wsknn-1.1/wsknn.egg-info/not-zip-safe
--rw-rw-r--   0 szymon    (1000) szymon    (1000)       28 2023-03-31 11:31:41.000000 wsknn-1.1/wsknn.egg-info/requires.txt
--rw-rw-r--   0 szymon    (1000) szymon    (1000)        6 2023-03-31 11:31:41.000000 wsknn-1.1/wsknn.egg-info/top_level.txt
+drwxrwxr-x   0 szymon    (1000) szymon    (1000)        0 2023-07-08 11:31:22.616915 wsknn-1.1.1/
+-rw-rw-r--   0 szymon    (1000) szymon    (1000)     1532 2023-07-08 11:28:47.000000 wsknn-1.1.1/LICENSE.md
+-rw-rw-r--   0 szymon    (1000) szymon    (1000)     8782 2023-07-08 11:31:22.616915 wsknn-1.1.1/PKG-INFO
+-rw-rw-r--   0 szymon    (1000) szymon    (1000)     7664 2023-03-30 19:34:34.000000 wsknn-1.1.1/README.md
+-rw-rw-r--   0 szymon    (1000) szymon    (1000)       80 2023-07-08 11:28:38.000000 wsknn-1.1.1/pyproject.toml
+-rw-rw-r--   0 szymon    (1000) szymon    (1000)     1284 2023-07-08 11:31:22.616915 wsknn-1.1.1/setup.cfg
+drwxrwxr-x   0 szymon    (1000) szymon    (1000)        0 2023-07-08 11:31:22.604915 wsknn-1.1.1/tests/
+-rw-rw-r--   0 szymon    (1000) szymon    (1000)      832 2023-03-29 08:54:18.000000 wsknn-1.1.1/tests/test_calc.py
+-rw-rw-r--   0 szymon    (1000) szymon    (1000)      408 2023-07-08 11:28:47.000000 wsknn-1.1.1/tests/test_data_loading.py
+-rw-rw-r--   0 szymon    (1000) szymon    (1000)      657 2023-03-29 08:54:18.000000 wsknn-1.1.1/tests/test_evaluation_metrics.py
+-rw-rw-r--   0 szymon    (1000) szymon    (1000)     1043 2023-03-30 19:34:34.000000 wsknn-1.1.1/tests/test_get_larger_value.py
+-rw-rw-r--   0 szymon    (1000) szymon    (1000)     1054 2023-03-30 19:34:34.000000 wsknn-1.1.1/tests/test_get_smaller_value.py
+-rw-rw-r--   0 szymon    (1000) szymon    (1000)     8076 2023-03-30 19:34:34.000000 wsknn-1.1.1/tests/test_items_class.py
+-rw-rw-r--   0 szymon    (1000) szymon    (1000)     2216 2023-03-30 19:34:34.000000 wsknn-1.1.1/tests/test_merge_dicts.py
+-rw-rw-r--   0 szymon    (1000) szymon    (1000)     5587 2023-03-30 19:34:34.000000 wsknn-1.1.1/tests/test_parse.py
+-rw-rw-r--   0 szymon    (1000) szymon    (1000)      761 2023-03-30 19:34:34.000000 wsknn-1.1.1/tests/test_parse_times.py
+-rw-rw-r--   0 szymon    (1000) szymon    (1000)     6965 2023-03-30 19:34:34.000000 wsknn-1.1.1/tests/test_sessions_class.py
+-rw-rw-r--   0 szymon    (1000) szymon    (1000)     1767 2023-07-08 11:28:47.000000 wsknn-1.1.1/tests/test_static_parsing.py
+-rw-rw-r--   0 szymon    (1000) szymon    (1000)     2052 2023-03-29 08:54:18.000000 wsknn-1.1.1/tests/test_weighting.py
+-rw-rw-r--   0 szymon    (1000) szymon    (1000)     3827 2023-03-29 08:54:18.000000 wsknn-1.1.1/tests/test_wsknn.py
+drwxrwxr-x   0 szymon    (1000) szymon    (1000)        0 2023-07-08 11:31:22.604915 wsknn-1.1.1/wsknn/
+-rw-rw-r--   0 szymon    (1000) szymon    (1000)      299 2023-07-08 11:28:47.000000 wsknn-1.1.1/wsknn/__init__.py
+drwxrwxr-x   0 szymon    (1000) szymon    (1000)        0 2023-07-08 11:31:22.608915 wsknn-1.1.1/wsknn/evaluate/
+-rw-rw-r--   0 szymon    (1000) szymon    (1000)      100 2023-03-29 08:54:18.000000 wsknn-1.1.1/wsknn/evaluate/__init__.py
+-rw-rw-r--   0 szymon    (1000) szymon    (1000)    15180 2023-03-29 08:54:18.000000 wsknn-1.1.1/wsknn/evaluate/metrics.py
+drwxrwxr-x   0 szymon    (1000) szymon    (1000)        0 2023-07-08 11:31:22.608915 wsknn-1.1.1/wsknn/evaluate/scores/
+-rw-rw-r--   0 szymon    (1000) szymon    (1000)       79 2023-03-29 08:54:18.000000 wsknn-1.1.1/wsknn/evaluate/scores/__init__.py
+-rw-rw-r--   0 szymon    (1000) szymon    (1000)     2006 2023-03-29 08:54:18.000000 wsknn-1.1.1/wsknn/evaluate/scores/scores.py
+-rw-rw-r--   0 szymon    (1000) szymon    (1000)     3283 2023-03-30 19:34:34.000000 wsknn-1.1.1/wsknn/evaluate/simulate.py
+-rw-rw-r--   0 szymon    (1000) szymon    (1000)     4640 2023-03-29 08:54:18.000000 wsknn-1.1.1/wsknn/fit_transform.py
+drwxrwxr-x   0 szymon    (1000) szymon    (1000)        0 2023-07-08 11:31:22.608915 wsknn-1.1.1/wsknn/model/
+-rw-rw-r--   0 szymon    (1000) szymon    (1000)        0 2023-03-29 08:54:18.000000 wsknn-1.1.1/wsknn/model/__init__.py
+-rw-rw-r--   0 szymon    (1000) szymon    (1000)    31010 2023-03-29 08:54:18.000000 wsknn-1.1.1/wsknn/model/wsknn.py
+-rw-rw-r--   0 szymon    (1000) szymon    (1000)     1535 2023-03-29 08:54:18.000000 wsknn-1.1.1/wsknn/predict.py
+drwxrwxr-x   0 szymon    (1000) szymon    (1000)        0 2023-07-08 11:31:22.608915 wsknn-1.1.1/wsknn/preprocessing/
+-rw-rw-r--   0 szymon    (1000) szymon    (1000)        0 2023-03-30 19:34:34.000000 wsknn-1.1.1/wsknn/preprocessing/__init__.py
+drwxrwxr-x   0 szymon    (1000) szymon    (1000)        0 2023-07-08 11:31:22.608915 wsknn-1.1.1/wsknn/preprocessing/export/
+-rw-rw-r--   0 szymon    (1000) szymon    (1000)        0 2023-03-30 19:34:34.000000 wsknn-1.1.1/wsknn/preprocessing/export/__init__.py
+-rw-rw-r--   0 szymon    (1000) szymon    (1000)     1181 2023-03-30 19:34:34.000000 wsknn-1.1.1/wsknn/preprocessing/export/export.py
+-rw-rw-r--   0 szymon    (1000) szymon    (1000)     3941 2023-07-08 11:28:47.000000 wsknn-1.1.1/wsknn/preprocessing/parse_static.py
+drwxrwxr-x   0 szymon    (1000) szymon    (1000)        0 2023-07-08 11:31:22.608915 wsknn-1.1.1/wsknn/preprocessing/static_parsers/
+-rw-rw-r--   0 szymon    (1000) szymon    (1000)        0 2023-07-08 11:28:47.000000 wsknn-1.1.1/wsknn/preprocessing/static_parsers/__init__.py
+drwxrwxr-x   0 szymon    (1000) szymon    (1000)        0 2023-07-08 11:31:22.608915 wsknn-1.1.1/wsknn/preprocessing/static_parsers/checkers/
+-rw-rw-r--   0 szymon    (1000) szymon    (1000)        0 2023-07-08 11:28:47.000000 wsknn-1.1.1/wsknn/preprocessing/static_parsers/checkers/__init__.py
+-rw-rw-r--   0 szymon    (1000) szymon    (1000)     1210 2023-07-08 11:28:47.000000 wsknn-1.1.1/wsknn/preprocessing/static_parsers/checkers/validation.py
+drwxrwxr-x   0 szymon    (1000) szymon    (1000)        0 2023-07-08 11:31:22.608915 wsknn-1.1.1/wsknn/preprocessing/static_parsers/cleaners/
+-rw-rw-r--   0 szymon    (1000) szymon    (1000)        0 2023-07-08 11:28:47.000000 wsknn-1.1.1/wsknn/preprocessing/static_parsers/cleaners/__init__.py
+-rw-rw-r--   0 szymon    (1000) szymon    (1000)     1278 2023-07-08 11:28:47.000000 wsknn-1.1.1/wsknn/preprocessing/static_parsers/cleaners/time_transform.py
+drwxrwxr-x   0 szymon    (1000) szymon    (1000)        0 2023-07-08 11:31:22.608915 wsknn-1.1.1/wsknn/preprocessing/static_parsers/csv_parser/
+-rw-rw-r--   0 szymon    (1000) szymon    (1000)        0 2023-07-08 11:28:47.000000 wsknn-1.1.1/wsknn/preprocessing/static_parsers/csv_parser/__init__.py
+-rw-rw-r--   0 szymon    (1000) szymon    (1000)     2160 2023-07-08 11:28:47.000000 wsknn-1.1.1/wsknn/preprocessing/static_parsers/csv_parser/parse.py
+drwxrwxr-x   0 szymon    (1000) szymon    (1000)        0 2023-07-08 11:31:22.608915 wsknn-1.1.1/wsknn/preprocessing/static_parsers/json_parser/
+-rw-rw-r--   0 szymon    (1000) szymon    (1000)        0 2023-07-08 11:28:47.000000 wsknn-1.1.1/wsknn/preprocessing/static_parsers/json_parser/__init__.py
+-rw-rw-r--   0 szymon    (1000) szymon    (1000)     4256 2023-07-08 11:28:47.000000 wsknn-1.1.1/wsknn/preprocessing/static_parsers/json_parser/parse.py
+-rw-rw-r--   0 szymon    (1000) szymon    (1000)     3700 2023-07-08 11:28:47.000000 wsknn-1.1.1/wsknn/preprocessing/static_parsers/parse.py
+drwxrwxr-x   0 szymon    (1000) szymon    (1000)        0 2023-07-08 11:31:22.612915 wsknn-1.1.1/wsknn/preprocessing/structure/
+-rw-rw-r--   0 szymon    (1000) szymon    (1000)        0 2023-03-30 19:34:34.000000 wsknn-1.1.1/wsknn/preprocessing/structure/__init__.py
+-rw-rw-r--   0 szymon    (1000) szymon    (1000)    10796 2023-03-30 19:34:34.000000 wsknn-1.1.1/wsknn/preprocessing/structure/item.py
+-rw-rw-r--   0 szymon    (1000) szymon    (1000)    13159 2023-03-30 19:34:34.000000 wsknn-1.1.1/wsknn/preprocessing/structure/session.py
+drwxrwxr-x   0 szymon    (1000) szymon    (1000)        0 2023-07-08 11:31:22.612915 wsknn-1.1.1/wsknn/preprocessing/utils/
+-rw-rw-r--   0 szymon    (1000) szymon    (1000)        0 2023-03-30 19:34:34.000000 wsknn-1.1.1/wsknn/preprocessing/utils/__init__.py
+-rw-rw-r--   0 szymon    (1000) szymon    (1000)      542 2023-03-30 19:34:34.000000 wsknn-1.1.1/wsknn/preprocessing/utils/calc.py
+-rw-rw-r--   0 szymon    (1000) szymon    (1000)     5016 2023-03-30 19:34:34.000000 wsknn-1.1.1/wsknn/preprocessing/utils/files.py
+-rw-rw-r--   0 szymon    (1000) szymon    (1000)     3793 2023-03-30 19:34:34.000000 wsknn-1.1.1/wsknn/preprocessing/utils/transform.py
+drwxrwxr-x   0 szymon    (1000) szymon    (1000)        0 2023-07-08 11:31:22.612915 wsknn-1.1.1/wsknn/utils/
+-rw-rw-r--   0 szymon    (1000) szymon    (1000)      144 2023-03-29 08:54:18.000000 wsknn-1.1.1/wsknn/utils/__init__.py
+-rw-rw-r--   0 szymon    (1000) szymon    (1000)     1337 2023-03-29 08:54:18.000000 wsknn-1.1.1/wsknn/utils/calc.py
+-rw-rw-r--   0 szymon    (1000) szymon    (1000)     2561 2023-03-29 08:54:18.000000 wsknn-1.1.1/wsknn/utils/errors.py
+-rw-rw-r--   0 szymon    (1000) szymon    (1000)      442 2023-03-29 08:54:18.000000 wsknn-1.1.1/wsknn/utils/meta.py
+-rw-rw-r--   0 szymon    (1000) szymon    (1000)     1732 2023-03-29 08:54:18.000000 wsknn-1.1.1/wsknn/utils/transform.py
+drwxrwxr-x   0 szymon    (1000) szymon    (1000)        0 2023-07-08 11:31:22.616915 wsknn-1.1.1/wsknn/weighting/
+-rw-rw-r--   0 szymon    (1000) szymon    (1000)       78 2023-03-29 08:54:18.000000 wsknn-1.1.1/wsknn/weighting/__init__.py
+-rw-rw-r--   0 szymon    (1000) szymon    (1000)     1611 2023-03-29 08:54:18.000000 wsknn-1.1.1/wsknn/weighting/item_weighting.py
+-rw-rw-r--   0 szymon    (1000) szymon    (1000)     2140 2023-03-29 08:54:18.000000 wsknn-1.1.1/wsknn/weighting/session_weighting.py
+-rw-rw-r--   0 szymon    (1000) szymon    (1000)     1651 2023-03-29 08:54:18.000000 wsknn-1.1.1/wsknn/weighting/weighting.py
+drwxrwxr-x   0 szymon    (1000) szymon    (1000)        0 2023-07-08 11:31:22.604915 wsknn-1.1.1/wsknn.egg-info/
+-rw-rw-r--   0 szymon    (1000) szymon    (1000)     8782 2023-07-08 11:31:22.000000 wsknn-1.1.1/wsknn.egg-info/PKG-INFO
+-rw-rw-r--   0 szymon    (1000) szymon    (1000)     2009 2023-07-08 11:31:22.000000 wsknn-1.1.1/wsknn.egg-info/SOURCES.txt
+-rw-rw-r--   0 szymon    (1000) szymon    (1000)        1 2023-07-08 11:31:22.000000 wsknn-1.1.1/wsknn.egg-info/dependency_links.txt
+-rw-rw-r--   0 szymon    (1000) szymon    (1000)        1 2023-03-31 11:31:40.000000 wsknn-1.1.1/wsknn.egg-info/not-zip-safe
+-rw-rw-r--   0 szymon    (1000) szymon    (1000)       28 2023-07-08 11:31:22.000000 wsknn-1.1.1/wsknn.egg-info/requires.txt
+-rw-rw-r--   0 szymon    (1000) szymon    (1000)        6 2023-07-08 11:31:22.000000 wsknn-1.1.1/wsknn.egg-info/top_level.txt
```

### Comparing `wsknn-1.1/LICENSE.md` & `wsknn-1.1.1/LICENSE.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright (c) Szymon Moliński, Sales Intelligence Sp. z o.o. (Digitree Group SA), 2022
+Copyright (c) Szymon Moliński, Sales Intelligence Sp. z o.o. (Digitree Group SA), 2023
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without modification,
 are permitted provided that the following conditions are met:
 
 * Redistributions of source code must retain the above copyright notice,
   this list of conditions and the following disclaimer.
```

### Comparing `wsknn-1.1/PKG-INFO` & `wsknn-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wsknn
-Version: 1.1
+Version: 1.1.1
 Summary: Weighted session-based model for recommendations
 Home-page: https://github.com/nokaut/wsknn
 Author: Szymon Moliński
 Author-email: s.molinski@digitree.pl
 License: MIT
 Project-URL: Documentation, https://readthedocs.org/projects/wsknn/
 Project-URL: Source, https://github.com/nokaut/wsknn
```

### Comparing `wsknn-1.1/README.md` & `wsknn-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `wsknn-1.1/setup.cfg` & `wsknn-1.1.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `wsknn-1.1/tests/test_calc.py` & `wsknn-1.1.1/tests/test_calc.py`

 * *Files identical despite different names*

### Comparing `wsknn-1.1/tests/test_evaluation_metrics.py` & `wsknn-1.1.1/tests/test_evaluation_metrics.py`

 * *Files identical despite different names*

### Comparing `wsknn-1.1/tests/test_get_larger_value.py` & `wsknn-1.1.1/tests/test_get_larger_value.py`

 * *Files identical despite different names*

### Comparing `wsknn-1.1/tests/test_get_smaller_value.py` & `wsknn-1.1.1/tests/test_get_smaller_value.py`

 * *Files identical despite different names*

### Comparing `wsknn-1.1/tests/test_items_class.py` & `wsknn-1.1.1/tests/test_items_class.py`

 * *Files identical despite different names*

### Comparing `wsknn-1.1/tests/test_merge_dicts.py` & `wsknn-1.1.1/tests/test_merge_dicts.py`

 * *Files identical despite different names*

### Comparing `wsknn-1.1/tests/test_parse.py` & `wsknn-1.1.1/tests/test_parse.py`

 * *Files identical despite different names*

### Comparing `wsknn-1.1/tests/test_parse_times.py` & `wsknn-1.1.1/tests/test_parse_times.py`

 * *Files identical despite different names*

### Comparing `wsknn-1.1/tests/test_sessions_class.py` & `wsknn-1.1.1/tests/test_sessions_class.py`

 * *Files identical despite different names*

### Comparing `wsknn-1.1/tests/test_weighting.py` & `wsknn-1.1.1/tests/test_weighting.py`

 * *Files identical despite different names*

### Comparing `wsknn-1.1/tests/test_wsknn.py` & `wsknn-1.1.1/tests/test_wsknn.py`

 * *Files identical despite different names*

### Comparing `wsknn-1.1/wsknn/evaluate/metrics.py` & `wsknn-1.1.1/wsknn/evaluate/metrics.py`

 * *Files identical despite different names*

### Comparing `wsknn-1.1/wsknn/evaluate/scores/scores.py` & `wsknn-1.1.1/wsknn/evaluate/scores/scores.py`

 * *Files identical despite different names*

### Comparing `wsknn-1.1/wsknn/evaluate/simulate.py` & `wsknn-1.1.1/wsknn/evaluate/simulate.py`

 * *Files identical despite different names*

### Comparing `wsknn-1.1/wsknn/fit_transform.py` & `wsknn-1.1.1/wsknn/fit_transform.py`

 * *Files identical despite different names*

### Comparing `wsknn-1.1/wsknn/model/wsknn.py` & `wsknn-1.1.1/wsknn/model/wsknn.py`

 * *Files identical despite different names*

### Comparing `wsknn-1.1/wsknn/predict.py` & `wsknn-1.1.1/wsknn/predict.py`

 * *Files identical despite different names*

### Comparing `wsknn-1.1/wsknn/preprocessing/export/export.py` & `wsknn-1.1.1/wsknn/preprocessing/export/export.py`

 * *Files identical despite different names*

### Comparing `wsknn-1.1/wsknn/preprocessing/structure/item.py` & `wsknn-1.1.1/wsknn/preprocessing/structure/item.py`

 * *Files identical despite different names*

### Comparing `wsknn-1.1/wsknn/preprocessing/structure/session.py` & `wsknn-1.1.1/wsknn/preprocessing/structure/session.py`

 * *Files identical despite different names*

### Comparing `wsknn-1.1/wsknn/preprocessing/utils/calc.py` & `wsknn-1.1.1/wsknn/preprocessing/utils/calc.py`

 * *Files identical despite different names*

### Comparing `wsknn-1.1/wsknn/preprocessing/utils/files.py` & `wsknn-1.1.1/wsknn/preprocessing/utils/files.py`

 * *Files identical despite different names*

### Comparing `wsknn-1.1/wsknn/preprocessing/utils/transform.py` & `wsknn-1.1.1/wsknn/preprocessing/utils/transform.py`

 * *Files identical despite different names*

### Comparing `wsknn-1.1/wsknn/utils/calc.py` & `wsknn-1.1.1/wsknn/utils/calc.py`

 * *Files identical despite different names*

### Comparing `wsknn-1.1/wsknn/utils/errors.py` & `wsknn-1.1.1/wsknn/utils/errors.py`

 * *Files identical despite different names*

### Comparing `wsknn-1.1/wsknn/utils/transform.py` & `wsknn-1.1.1/wsknn/utils/transform.py`

 * *Files identical despite different names*

### Comparing `wsknn-1.1/wsknn/weighting/item_weighting.py` & `wsknn-1.1.1/wsknn/weighting/item_weighting.py`

 * *Files identical despite different names*

### Comparing `wsknn-1.1/wsknn/weighting/session_weighting.py` & `wsknn-1.1.1/wsknn/weighting/session_weighting.py`

 * *Files identical despite different names*

### Comparing `wsknn-1.1/wsknn/weighting/weighting.py` & `wsknn-1.1.1/wsknn/weighting/weighting.py`

 * *Files identical despite different names*

### Comparing `wsknn-1.1/wsknn.egg-info/PKG-INFO` & `wsknn-1.1.1/wsknn.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wsknn
-Version: 1.1
+Version: 1.1.1
 Summary: Weighted session-based model for recommendations
 Home-page: https://github.com/nokaut/wsknn
 Author: Szymon Moliński
 Author-email: s.molinski@digitree.pl
 License: MIT
 Project-URL: Documentation, https://readthedocs.org/projects/wsknn/
 Project-URL: Source, https://github.com/nokaut/wsknn
```

### Comparing `wsknn-1.1/wsknn.egg-info/SOURCES.txt` & `wsknn-1.1.1/wsknn.egg-info/SOURCES.txt`

 * *Files 27% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 tests/test_get_larger_value.py
 tests/test_get_smaller_value.py
 tests/test_items_class.py
 tests/test_merge_dicts.py
 tests/test_parse.py
 tests/test_parse_times.py
 tests/test_sessions_class.py
+tests/test_static_parsing.py
 tests/test_weighting.py
 tests/test_wsknn.py
 wsknn/__init__.py
 wsknn/fit_transform.py
 wsknn/predict.py
 wsknn.egg-info/PKG-INFO
 wsknn.egg-info/SOURCES.txt
@@ -30,14 +31,24 @@
 wsknn/evaluate/scores/scores.py
 wsknn/model/__init__.py
 wsknn/model/wsknn.py
 wsknn/preprocessing/__init__.py
 wsknn/preprocessing/parse_static.py
 wsknn/preprocessing/export/__init__.py
 wsknn/preprocessing/export/export.py
+wsknn/preprocessing/static_parsers/__init__.py
+wsknn/preprocessing/static_parsers/parse.py
+wsknn/preprocessing/static_parsers/checkers/__init__.py
+wsknn/preprocessing/static_parsers/checkers/validation.py
+wsknn/preprocessing/static_parsers/cleaners/__init__.py
+wsknn/preprocessing/static_parsers/cleaners/time_transform.py
+wsknn/preprocessing/static_parsers/csv_parser/__init__.py
+wsknn/preprocessing/static_parsers/csv_parser/parse.py
+wsknn/preprocessing/static_parsers/json_parser/__init__.py
+wsknn/preprocessing/static_parsers/json_parser/parse.py
 wsknn/preprocessing/structure/__init__.py
 wsknn/preprocessing/structure/item.py
 wsknn/preprocessing/structure/session.py
 wsknn/preprocessing/utils/__init__.py
 wsknn/preprocessing/utils/calc.py
 wsknn/preprocessing/utils/files.py
 wsknn/preprocessing/utils/transform.py
```

