# Comparing `tmp/cereja-1.8.4.tar.gz` & `tmp/cereja-1.8.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cereja-1.8.4.tar", last modified: Sun Mar 12 18:31:03 2023, max compression
+gzip compressed data, was "cereja-1.8.5.tar", last modified: Sat Jul  8 07:21:58 2023, max compression
```

## Comparing `cereja-1.8.4.tar` & `cereja-1.8.5.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 18:31:03.069774 cereja-1.8.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-03-12 18:30:48.000000 cereja-1.8.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    12657 2023-03-12 18:31:03.065774 cereja-1.8.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10469 2023-03-12 18:30:48.000000 cereja-1.8.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 18:31:03.061774 cereja-1.8.4/cereja/
--rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-03-12 18:30:48.000000 cereja-1.8.4/cereja/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-03-12 18:30:48.000000 cereja-1.8.4/cereja/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 18:31:03.061774 cereja-1.8.4/cereja/_requests/
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-03-12 18:30:48.000000 cereja-1.8.4/cereja/_requests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9236 2023-03-12 18:30:48.000000 cereja-1.8.4/cereja/_requests/_http.py
--rw-r--r--   0 runner    (1001) docker     (123)     4112 2023-03-12 18:30:48.000000 cereja-1.8.4/cereja/_requests/request.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 18:31:03.061774 cereja-1.8.4/cereja/array/
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-03-12 18:30:48.000000 cereja-1.8.4/cereja/array/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20590 2023-03-12 18:30:48.000000 cereja-1.8.4/cereja/array/_array.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 18:31:03.061774 cereja-1.8.4/cereja/concurrently/
--rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-03-12 18:30:48.000000 cereja-1.8.4/cereja/concurrently/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9957 2023-03-12 18:30:48.000000 cereja-1.8.4/cereja/concurrently/_concurrence.py
--rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-03-12 18:30:48.000000 cereja-1.8.4/cereja/concurrently/process.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 18:31:03.061774 cereja-1.8.4/cereja/config/
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-03-12 18:30:48.000000 cereja-1.8.4/cereja/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6553 2023-03-12 18:30:48.000000 cereja-1.8.4/cereja/config/_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-03-12 18:30:48.000000 cereja-1.8.4/cereja/config/cj_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     3562 2023-03-12 18:30:48.000000 cereja-1.8.4/cereja/config/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 18:31:03.065774 cereja-1.8.4/cereja/date/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-03-12 18:30:48.000000 cereja-1.8.4/cereja/date/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-03-12 18:30:48.000000 cereja-1.8.4/cereja/date/_datetime.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 18:31:03.065774 cereja-1.8.4/cereja/display/
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-03-12 18:30:48.000000 cereja-1.8.4/cereja/display/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    34480 2023-03-12 18:30:48.000000 cereja-1.8.4/cereja/display/_display.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 18:31:03.065774 cereja-1.8.4/cereja/experimental/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-03-12 18:30:48.000000 cereja-1.8.4/cereja/experimental/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3253 2023-03-12 18:30:48.000000 cereja-1.8.4/cereja/experimental/commons.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 18:31:03.065774 cereja-1.8.4/cereja/file/
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-03-12 18:30:48.000000 cereja-1.8.4/cereja/file/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29548 2023-03-12 18:30:48.000000 cereja-1.8.4/cereja/file/_io.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 18:31:03.065774 cereja-1.8.4/cereja/hashtools/
--rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-03-12 18:30:48.000000 cereja-1.8.4/cereja/hashtools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-03-12 18:30:48.000000 cereja-1.8.4/cereja/hashtools/_hash.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 18:31:03.065774 cereja-1.8.4/cereja/mathtools/
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-03-12 18:30:48.000000 cereja-1.8.4/cereja/mathtools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3870 2023-03-12 18:30:48.000000 cereja-1.8.4/cereja/mathtools/_op.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 18:31:03.065774 cereja-1.8.4/cereja/mltools/
--rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-03-12 18:30:48.000000 cereja-1.8.4/cereja/mltools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20528 2023-03-12 18:30:48.000000 cereja-1.8.4/cereja/mltools/data.py
--rw-r--r--   0 runner    (1001) docker     (123)    12321 2023-03-12 18:30:48.000000 cereja-1.8.4/cereja/mltools/pln.py
--rw-r--r--   0 runner    (1001) docker     (123)     5669 2023-03-12 18:30:48.000000 cereja-1.8.4/cereja/mltools/preprocess.py
--rw-r--r--   0 runner    (1001) docker     (123)    15584 2023-03-12 18:30:48.000000 cereja-1.8.4/cereja/mltools/split_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 18:31:03.065774 cereja-1.8.4/cereja/system/
--rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-03-12 18:30:48.000000 cereja-1.8.4/cereja/system/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16599 2023-03-12 18:30:48.000000 cereja-1.8.4/cereja/system/_path.py
--rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-03-12 18:30:48.000000 cereja-1.8.4/cereja/system/commons.py
--rw-r--r--   0 runner    (1001) docker     (123)     5545 2023-03-12 18:30:48.000000 cereja-1.8.4/cereja/system/unicode.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 18:31:03.065774 cereja-1.8.4/cereja/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-03-12 18:30:48.000000 cereja-1.8.4/cereja/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    35476 2023-03-12 18:30:48.000000 cereja-1.8.4/cereja/utils/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-03-12 18:30:48.000000 cereja-1.8.4/cereja/utils/colab.py
--rw-r--r--   0 runner    (1001) docker     (123)     5338 2023-03-12 18:30:48.000000 cereja-1.8.4/cereja/utils/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     3354 2023-03-12 18:30:48.000000 cereja-1.8.4/cereja/utils/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 18:31:03.061774 cereja-1.8.4/cereja.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12657 2023-03-12 18:31:03.000000 cereja-1.8.4/cereja.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-03-12 18:31:03.000000 cereja-1.8.4/cereja.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-12 18:31:03.000000 cereja-1.8.4/cereja.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-03-12 18:31:03.000000 cereja-1.8.4/cereja.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-03-12 18:30:48.000000 cereja-1.8.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-12 18:31:03.069774 cereja-1.8.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 18:31:03.065774 cereja-1.8.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-03-12 18:30:48.000000 cereja-1.8.4/tests/testhashtools.py
--rw-r--r--   0 runner    (1001) docker     (123)    12733 2023-03-12 18:30:48.000000 cereja-1.8.4/tests/tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     5499 2023-03-12 18:30:48.000000 cereja-1.8.4/tests/testsfiletools.py
--rw-r--r--   0 runner    (1001) docker     (123)     6624 2023-03-12 18:30:48.000000 cereja-1.8.4/tests/testsmltools.py
--rw-r--r--   0 runner    (1001) docker     (123)    13844 2023-03-12 18:30:48.000000 cereja-1.8.4/tests/testsutils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 07:21:58.857824 cereja-1.8.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-07-08 07:21:36.000000 cereja-1.8.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12657 2023-07-08 07:21:58.857824 cereja-1.8.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10469 2023-07-08 07:21:36.000000 cereja-1.8.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 07:21:58.849824 cereja-1.8.5/cereja/
+-rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-07-08 07:21:36.000000 cereja-1.8.5/cereja/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-07-08 07:21:36.000000 cereja-1.8.5/cereja/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 07:21:58.853824 cereja-1.8.5/cereja/_requests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-07-08 07:21:36.000000 cereja-1.8.5/cereja/_requests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9236 2023-07-08 07:21:36.000000 cereja-1.8.5/cereja/_requests/_http.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4112 2023-07-08 07:21:36.000000 cereja-1.8.5/cereja/_requests/request.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 07:21:58.853824 cereja-1.8.5/cereja/array/
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-07-08 07:21:36.000000 cereja-1.8.5/cereja/array/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20590 2023-07-08 07:21:36.000000 cereja-1.8.5/cereja/array/_array.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 07:21:58.853824 cereja-1.8.5/cereja/concurrently/
+-rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-07-08 07:21:36.000000 cereja-1.8.5/cereja/concurrently/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9957 2023-07-08 07:21:36.000000 cereja-1.8.5/cereja/concurrently/_concurrence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3191 2023-07-08 07:21:36.000000 cereja-1.8.5/cereja/concurrently/process.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 07:21:58.853824 cereja-1.8.5/cereja/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-07-08 07:21:36.000000 cereja-1.8.5/cereja/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6553 2023-07-08 07:21:36.000000 cereja-1.8.5/cereja/config/_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-07-08 07:21:36.000000 cereja-1.8.5/cereja/config/cj_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3562 2023-07-08 07:21:36.000000 cereja-1.8.5/cereja/config/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 07:21:58.853824 cereja-1.8.5/cereja/date/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-08 07:21:36.000000 cereja-1.8.5/cereja/date/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-07-08 07:21:36.000000 cereja-1.8.5/cereja/date/_datetime.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 07:21:58.853824 cereja-1.8.5/cereja/display/
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-07-08 07:21:36.000000 cereja-1.8.5/cereja/display/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34480 2023-07-08 07:21:36.000000 cereja-1.8.5/cereja/display/_display.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 07:21:58.853824 cereja-1.8.5/cereja/experimental/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-08 07:21:36.000000 cereja-1.8.5/cereja/experimental/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3253 2023-07-08 07:21:36.000000 cereja-1.8.5/cereja/experimental/commons.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 07:21:58.853824 cereja-1.8.5/cereja/file/
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-07-08 07:21:36.000000 cereja-1.8.5/cereja/file/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29548 2023-07-08 07:21:36.000000 cereja-1.8.5/cereja/file/_io.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 07:21:58.853824 cereja-1.8.5/cereja/hashtools/
+-rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-07-08 07:21:36.000000 cereja-1.8.5/cereja/hashtools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-07-08 07:21:36.000000 cereja-1.8.5/cereja/hashtools/_hash.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 07:21:58.853824 cereja-1.8.5/cereja/mathtools/
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-07-08 07:21:36.000000 cereja-1.8.5/cereja/mathtools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3870 2023-07-08 07:21:36.000000 cereja-1.8.5/cereja/mathtools/_op.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 07:21:58.857824 cereja-1.8.5/cereja/mltools/
+-rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-07-08 07:21:36.000000 cereja-1.8.5/cereja/mltools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20528 2023-07-08 07:21:36.000000 cereja-1.8.5/cereja/mltools/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12321 2023-07-08 07:21:36.000000 cereja-1.8.5/cereja/mltools/pln.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7033 2023-07-08 07:21:36.000000 cereja-1.8.5/cereja/mltools/preprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15584 2023-07-08 07:21:36.000000 cereja-1.8.5/cereja/mltools/split_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 07:21:58.857824 cereja-1.8.5/cereja/system/
+-rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-07-08 07:21:36.000000 cereja-1.8.5/cereja/system/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16599 2023-07-08 07:21:36.000000 cereja-1.8.5/cereja/system/_path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-07-08 07:21:36.000000 cereja-1.8.5/cereja/system/commons.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5545 2023-07-08 07:21:36.000000 cereja-1.8.5/cereja/system/unicode.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 07:21:58.857824 cereja-1.8.5/cereja/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-07-08 07:21:36.000000 cereja-1.8.5/cereja/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36510 2023-07-08 07:21:36.000000 cereja-1.8.5/cereja/utils/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-07-08 07:21:36.000000 cereja-1.8.5/cereja/utils/colab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5338 2023-07-08 07:21:36.000000 cereja-1.8.5/cereja/utils/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3354 2023-07-08 07:21:36.000000 cereja-1.8.5/cereja/utils/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 07:21:58.853824 cereja-1.8.5/cereja.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12657 2023-07-08 07:21:58.000000 cereja-1.8.5/cereja.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-07-08 07:21:58.000000 cereja-1.8.5/cereja.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 07:21:58.000000 cereja-1.8.5/cereja.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-08 07:21:58.000000 cereja-1.8.5/cereja.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-07-08 07:21:36.000000 cereja-1.8.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 07:21:58.857824 cereja-1.8.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 07:21:58.857824 cereja-1.8.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-07-08 07:21:36.000000 cereja-1.8.5/tests/testhashtools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12733 2023-07-08 07:21:36.000000 cereja-1.8.5/tests/tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5499 2023-07-08 07:21:36.000000 cereja-1.8.5/tests/testsfiletools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6624 2023-07-08 07:21:36.000000 cereja-1.8.5/tests/testsmltools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14972 2023-07-08 07:21:36.000000 cereja-1.8.5/tests/testsutils.py
```

### Comparing `cereja-1.8.4/LICENSE` & `cereja-1.8.5/LICENSE`

 * *Files identical despite different names*

### Comparing `cereja-1.8.4/PKG-INFO` & `cereja-1.8.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cereja
-Version: 1.8.4
+Version: 1.8.5
 Summary: Cereja is a bundle of useful functions that I don't want to rewrite.
 Author-email: Joab Leite <leitejoab@gmail.com>
 License: Copyright (c) 2019 The Cereja Project
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `cereja-1.8.4/README.md` & `cereja-1.8.5/README.md`

 * *Files identical despite different names*

### Comparing `cereja-1.8.4/cereja/__init__.py` & `cereja-1.8.5/cereja/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 from .date import *
 from . import hashtools
 from . import mathtools
 from .mathtools import *
 from . import experimental
 from ._requests import request
 
-VERSION = "1.8.4.final.0"
+VERSION = "1.8.5.final.0"
 
 __version__ = get_version_pep440_compliant(VERSION)
 
 NON_BMP_SUPPORTED = None
 if NON_BMP_SUPPORTED is None:
     # This is important, as there may be an exception if the terminal does not support unicode bmp
     try:
```

### Comparing `cereja-1.8.4/cereja/__main__.py` & `cereja-1.8.5/cereja/__main__.py`

 * *Files identical despite different names*

### Comparing `cereja-1.8.4/cereja/_requests/__init__.py` & `cereja-1.8.5/cereja/_requests/__init__.py`

 * *Files identical despite different names*

### Comparing `cereja-1.8.4/cereja/_requests/_http.py` & `cereja-1.8.5/cereja/_requests/_http.py`

 * *Files identical despite different names*

### Comparing `cereja-1.8.4/cereja/_requests/request.py` & `cereja-1.8.5/cereja/_requests/request.py`

 * *Files identical despite different names*

### Comparing `cereja-1.8.4/cereja/array/__init__.py` & `cereja-1.8.5/cereja/array/__init__.py`

 * *Files identical despite different names*

### Comparing `cereja-1.8.4/cereja/array/_array.py` & `cereja-1.8.5/cereja/array/_array.py`

 * *Files identical despite different names*

### Comparing `cereja-1.8.4/cereja/concurrently/__init__.py` & `cereja-1.8.5/cereja/concurrently/__init__.py`

 * *Files identical despite different names*

### Comparing `cereja-1.8.4/cereja/concurrently/_concurrence.py` & `cereja-1.8.5/cereja/concurrently/_concurrence.py`

 * *Files identical despite different names*

### Comparing `cereja-1.8.4/cereja/config/_constants.py` & `cereja-1.8.5/cereja/config/_constants.py`

 * *Files identical despite different names*

### Comparing `cereja-1.8.4/cereja/config/cj_types.py` & `cereja-1.8.5/cereja/config/cj_types.py`

 * *Files identical despite different names*

### Comparing `cereja-1.8.4/cereja/config/conf.py` & `cereja-1.8.5/cereja/config/conf.py`

 * *Files identical despite different names*

### Comparing `cereja-1.8.4/cereja/date/_datetime.py` & `cereja-1.8.5/cereja/date/_datetime.py`

 * *Files identical despite different names*

### Comparing `cereja-1.8.4/cereja/display/__init__.py` & `cereja-1.8.5/cereja/display/__init__.py`

 * *Files identical despite different names*

### Comparing `cereja-1.8.4/cereja/display/_display.py` & `cereja-1.8.5/cereja/display/_display.py`

 * *Files identical despite different names*

### Comparing `cereja-1.8.4/cereja/experimental/commons.py` & `cereja-1.8.5/cereja/experimental/commons.py`

 * *Files identical despite different names*

### Comparing `cereja-1.8.4/cereja/file/__init__.py` & `cereja-1.8.5/cereja/file/__init__.py`

 * *Files identical despite different names*

### Comparing `cereja-1.8.4/cereja/file/_io.py` & `cereja-1.8.5/cereja/file/_io.py`

 * *Files identical despite different names*

### Comparing `cereja-1.8.4/cereja/hashtools/__init__.py` & `cereja-1.8.5/cereja/hashtools/__init__.py`

 * *Files identical despite different names*

### Comparing `cereja-1.8.4/cereja/hashtools/_hash.py` & `cereja-1.8.5/cereja/hashtools/_hash.py`

 * *Files identical despite different names*

### Comparing `cereja-1.8.4/cereja/mathtools/__init__.py` & `cereja-1.8.5/cereja/mathtools/__init__.py`

 * *Files identical despite different names*

### Comparing `cereja-1.8.4/cereja/mathtools/_op.py` & `cereja-1.8.5/cereja/mathtools/_op.py`

 * *Files identical despite different names*

### Comparing `cereja-1.8.4/cereja/mltools/__init__.py` & `cereja-1.8.5/cereja/mltools/__init__.py`

 * *Files identical despite different names*

### Comparing `cereja-1.8.4/cereja/mltools/data.py` & `cereja-1.8.5/cereja/mltools/data.py`

 * *Files identical despite different names*

### Comparing `cereja-1.8.4/cereja/mltools/pln.py` & `cereja-1.8.5/cereja/mltools/pln.py`

 * *Files identical despite different names*

### Comparing `cereja-1.8.4/cereja/mltools/preprocess.py` & `cereja-1.8.5/cereja/mltools/preprocess.py`

 * *Files 21% similar despite different names*

```diff
@@ -18,28 +18,66 @@
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 """
 
 import re
-from typing import AnyStr, Sequence, Union, List
+from typing import AnyStr, Sequence, Union, List, Tuple
 from unicodedata import normalize as _normalize
 
 from ..config import (
     ENG_CONTRACTIONS,
     PUNCTUATION,
     VALID_LANGUAGE_CHAR,
     LANGUAGES,
     STOP_WORDS,
 )
 
 _NORMALIZE_VALUES = "".join(PUNCTUATION)
 
 
+def split_by_punct(text: str, punct: str = '.!?') -> list:
+    """
+    split text by periods.
+
+    :param text: any string
+    :param punct: string of chars
+    :return:
+    """
+    assert isinstance(punct, str), 'Send punct send the strings in string format: "!.?"'
+    # Regular expression to split text by periods
+    pattern = r'(?<=[%s])\s+' % punct
+    texts = re.split(pattern, text)
+    return texts
+
+
+def remove_delimited_text(text, delimiters: Sequence[Tuple[AnyStr, AnyStr]] = (("*", '*'), ("(", ")"), ("[", "]"))):
+    """
+    Remove words or phrases delimited by bullets from the provided text.
+
+    Arguments:
+      text(str): The text to be processed.
+      delimiters (Sequence[Tuple[AnyStr, AnyStr]], optional): A sequence of tuples that specify the start and end markers of the delimited words or phrases.
+          The default is (("*", '*'), ("(", ")"), ("[", "]")).
+
+    Returns:
+      str: The rendered text, without the delimited words or phrases.
+
+    Example:
+      >>> text = "Hello world of *options*! [shows options] How are you (walks out and says)?"
+      >>> clear_text = remove_delimited_text(text)
+      >>> print(clear_text)
+      "Hello world! How are you?"
+    """
+    pattern = '|'.join(f'({re.escape(start)}{r".*?"}{re.escape(end)})' for start, end in delimiters)
+    text = re.sub(pattern, "", text)
+    return text
+
+
 def separate(
         text: AnyStr, sep: Union[AnyStr, Sequence[AnyStr]] = PUNCTUATION, between_char=False
 ) -> str:
     """
     Creating a space between an element in sep values
     PUNCTUATION = {'?', '!', ',', '.'}
     e.g:
```

### Comparing `cereja-1.8.4/cereja/mltools/split_data.py` & `cereja-1.8.5/cereja/mltools/split_data.py`

 * *Files identical despite different names*

### Comparing `cereja-1.8.4/cereja/system/__init__.py` & `cereja-1.8.5/cereja/system/__init__.py`

 * *Files identical despite different names*

### Comparing `cereja-1.8.4/cereja/system/_path.py` & `cereja-1.8.5/cereja/system/_path.py`

 * *Files identical despite different names*

### Comparing `cereja-1.8.4/cereja/system/commons.py` & `cereja-1.8.5/cereja/system/commons.py`

 * *Files identical despite different names*

### Comparing `cereja-1.8.4/cereja/system/unicode.py` & `cereja-1.8.5/cereja/system/unicode.py`

 * *Files identical despite different names*

### Comparing `cereja-1.8.4/cereja/utils/__init__.py` & `cereja-1.8.5/cereja/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `cereja-1.8.4/cereja/utils/_utils.py` & `cereja-1.8.5/cereja/utils/_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,14 +76,15 @@
     "dict_max_value",
     "dict_min_value",
     "dict_filter_value",
     "get_zero_mask",
     "get_batch_strides",
     "Thread",
     "prune_values",
+    "split_sequence"
 ]
 
 logger = logging.getLogger(__name__)
 
 
 class Thread(threading.Thread):
     def __init__(
@@ -107,14 +108,44 @@
             self._callback(res)
 
 
 def is_indexable(v):
     return hasattr(v, "__getitem__")
 
 
+def split_sequence(seq, is_break_fn):
+    """
+    Divide a sequence into sub-sequences at the point defined by a given is_break_fn function.
+
+    Args:
+        seq (list): The sequence to be divided into sub-sequences.
+        is_break_fn (callable): A function that takes two elements from the sequence and
+            returns True if there is a break between them and False otherwise.
+
+    Returns:
+        list: A list of sub-sequences, each containing a sequence of consecutive elements.
+
+    Examples:
+        >>> seq = [1, 2, 3, 4, 5, 2, 3, 4, 5, 6, 7, 8]
+        >>> is_even = lambda x, y: x % 2 == 0 and y % 2 == 0
+        >>> sub_seqs = split_sequence(seq, is_even)
+        >>> sub_seqs
+        [[1, 2, 3, 4, 5], [2, 3, 4, 5, 6, 7, 8]]
+    """
+    sub_seqs = []
+    sub_seq = [seq[0]]
+    for i in range(1, len(seq)):
+        if is_break_fn(seq[i-1], seq[i]):
+            sub_seqs.append(sub_seq)
+            sub_seq = []
+        sub_seq.append(seq[i])
+    sub_seqs.append(sub_seq)
+    return sub_seqs
+
+
 def chunk(
         data: Sequence,
         batch_size: int = None,
         fill_with: Any = None,
         is_random: bool = False,
         max_batches: int = None,
 ) -> List[Union[Sequence, List, Tuple, Dict]]:
```

### Comparing `cereja-1.8.4/cereja/utils/colab.py` & `cereja-1.8.5/cereja/utils/colab.py`

 * *Files identical despite different names*

### Comparing `cereja-1.8.4/cereja/utils/decorators.py` & `cereja-1.8.5/cereja/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `cereja-1.8.4/cereja/utils/version.py` & `cereja-1.8.5/cereja/utils/version.py`

 * *Files identical despite different names*

### Comparing `cereja-1.8.4/cereja.egg-info/PKG-INFO` & `cereja-1.8.5/cereja.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cereja
-Version: 1.8.4
+Version: 1.8.5
 Summary: Cereja is a bundle of useful functions that I don't want to rewrite.
 Author-email: Joab Leite <leitejoab@gmail.com>
 License: Copyright (c) 2019 The Cereja Project
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `cereja-1.8.4/cereja.egg-info/SOURCES.txt` & `cereja-1.8.5/cereja.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cereja-1.8.4/pyproject.toml` & `cereja-1.8.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `cereja-1.8.4/tests/testhashtools.py` & `cereja-1.8.5/tests/testhashtools.py`

 * *Files identical despite different names*

### Comparing `cereja-1.8.4/tests/tests.py` & `cereja-1.8.5/tests/tests.py`

 * *Files identical despite different names*

### Comparing `cereja-1.8.4/tests/testsfiletools.py` & `cereja-1.8.5/tests/testsfiletools.py`

 * *Files identical despite different names*

### Comparing `cereja-1.8.4/tests/testsmltools.py` & `cereja-1.8.5/tests/testsmltools.py`

 * *Files identical despite different names*

### Comparing `cereja-1.8.4/tests/testsutils.py` & `cereja-1.8.5/tests/testsutils.py`

 * *Files 8% similar despite different names*

```diff
@@ -29,14 +29,22 @@
 
     def test_import_string(self):
         pass
 
     def test_install_if_not(self):
         pass
 
+    def test_split_sequence(self):
+        val = [10, 11, 12, 13, 14, 15, 16, 17, 18, 19, 117, 118, 119, 120, 121, 122, 123, 124, 125, 126, 127, 128, 129,
+               130, 131, 132, 133, 134, 135, 136, 137, 138, 139, 140, 141, 142]
+        expected = [[10, 11, 12, 13, 14, 15, 16, 17, 18, 19],
+                    [117, 118, 119, 120, 121, 122, 123, 124, 125, 126, 127, 128, 129, 130, 131, 132, 133, 134, 135, 136,
+                     137, 138, 139, 140, 141, 142]]
+        self.assertListEqual(utils.split_sequence(val, lambda x, y: x + 1 != y), expected)
+
     def test_invert_dict(self):
         data = {
             "s": 0,
             "y": 1,
             "v": 2,
             "l": 3,
             "i": 4,
@@ -59,24 +67,24 @@
             "h": 21,
             "r": 22,
             "w": 23,
             "m": 24,
             "q": 25,
         }
         expected = {
-            0: "s",
-            1: "y",
-            2: "v",
-            3: "l",
-            4: "i",
-            5: "p",
-            6: "b",
-            7: "z",
-            8: "c",
-            9: "a",
+            0:  "s",
+            1:  "y",
+            2:  "v",
+            3:  "l",
+            4:  "i",
+            5:  "p",
+            6:  "b",
+            7:  "z",
+            8:  "c",
+            9:  "a",
             10: "k",
             11: "e",
             12: "d",
             13: "j",
             14: "x",
             15: "u",
             16: "o",
@@ -169,15 +177,15 @@
             "joab",
             "joab",
             "joab",
             "joab",
         ]
 
         self.assertEqual(
-            rescale_values(value, 22, fill_with="joab", filling="post"), expected
+                rescale_values(value, 22, fill_with="joab", filling="post"), expected
         )
 
         expected = [
             "joab",
             "joab",
             "joab",
             "joab",
@@ -198,15 +206,15 @@
             6,
             7,
             8,
             9,
         ]
 
         self.assertEqual(
-            rescale_values(value, 22, fill_with="joab", filling="pre"), expected
+                rescale_values(value, 22, fill_with="joab", filling="pre"), expected
         )
 
         expected = [0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 1, 2, 3, 4, 5, 6, 7, 8, 9]
         self.assertEqual(rescale_values(value, 22, filling="pre"), expected)
 
         expected = [0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 9, 9, 9, 9, 9, 9, 9, 9, 9, 9, 9, 9]
         self.assertEqual(rescale_values(value, 22, filling="post"), expected)
@@ -285,98 +293,98 @@
 
     def test_type_table_of(self):
         pass
 
     def test_sort_dict(self):
         val = {0: 1, 1: 2, 2: 1, 3: 4, 4: 1, 5: 43, 6: 1, 7: 10, 8: 22, 9: 0}
         self.assertDictEqual(
-            utils.sort_dict(val),
-            OrderedDict(
-                [
-                    (0, 1),
-                    (1, 2),
-                    (2, 1),
-                    (3, 4),
-                    (4, 1),
-                    (5, 43),
-                    (6, 1),
-                    (7, 10),
-                    (8, 22),
-                    (9, 0),
-                ]
-            ),
+                utils.sort_dict(val),
+                OrderedDict(
+                        [
+                            (0, 1),
+                            (1, 2),
+                            (2, 1),
+                            (3, 4),
+                            (4, 1),
+                            (5, 43),
+                            (6, 1),
+                            (7, 10),
+                            (8, 22),
+                            (9, 0),
+                        ]
+                ),
         )
         self.assertDictEqual(
-            utils.sort_dict(val, by_values=True),
-            OrderedDict(
-                [
-                    (9, 0),
-                    (0, 1),
-                    (2, 1),
-                    (4, 1),
-                    (6, 1),
-                    (1, 2),
-                    (3, 4),
-                    (7, 10),
-                    (8, 22),
-                    (5, 43),
-                ]
-            ),
+                utils.sort_dict(val, by_values=True),
+                OrderedDict(
+                        [
+                            (9, 0),
+                            (0, 1),
+                            (2, 1),
+                            (4, 1),
+                            (6, 1),
+                            (1, 2),
+                            (3, 4),
+                            (7, 10),
+                            (8, 22),
+                            (5, 43),
+                        ]
+                ),
         )
         self.assertDictEqual(
-            utils.sort_dict(val, by_values=True, reverse=True),
-            OrderedDict(
-                [
-                    (5, 43),
-                    (8, 22),
-                    (7, 10),
-                    (3, 4),
-                    (1, 2),
-                    (0, 1),
-                    (2, 1),
-                    (4, 1),
-                    (6, 1),
-                    (9, 0),
-                ]
-            ),
+                utils.sort_dict(val, by_values=True, reverse=True),
+                OrderedDict(
+                        [
+                            (5, 43),
+                            (8, 22),
+                            (7, 10),
+                            (3, 4),
+                            (1, 2),
+                            (0, 1),
+                            (2, 1),
+                            (4, 1),
+                            (6, 1),
+                            (9, 0),
+                        ]
+                ),
         )
 
         self.assertDictEqual(
-            utils.sort_dict(val, by_keys=True),
-            OrderedDict(
-                [
-                    (0, 1),
-                    (1, 2),
-                    (2, 1),
-                    (3, 4),
-                    (4, 1),
-                    (5, 43),
-                    (6, 1),
-                    (7, 10),
-                    (8, 22),
-                    (9, 0),
-                ]
-            ),
+                utils.sort_dict(val, by_keys=True),
+                OrderedDict(
+                        [
+                            (0, 1),
+                            (1, 2),
+                            (2, 1),
+                            (3, 4),
+                            (4, 1),
+                            (5, 43),
+                            (6, 1),
+                            (7, 10),
+                            (8, 22),
+                            (9, 0),
+                        ]
+                ),
         )
         self.assertDictEqual(
-            utils.sort_dict(val, by_keys=True, reverse=True),
-            OrderedDict(
-                [
-                    (9, 0),
-                    (8, 22),
-                    (7, 10),
-                    (6, 1),
-                    (5, 43),
-                    (4, 1),
-                    (3, 4),
-                    (2, 1),
-                    (1, 2),
-                    (0, 1),
-                ]
-            ),
+                utils.sort_dict(val, by_keys=True, reverse=True),
+                OrderedDict(
+                        [
+                            (9, 0),
+                            (8, 22),
+                            (7, 10),
+                            (6, 1),
+                            (5, 43),
+                            (4, 1),
+                            (3, 4),
+                            (2, 1),
+                            (1, 2),
+                            (0, 1),
+                        ]
+                ),
         )
 
     def test_dict_append(self):
         my_dict = {}
         utils.dict_append(my_dict, "key_eg", 1, 2, 3, 4, 5, 6)
         self.assertDictEqual(my_dict, {"key_eg": [1, 2, 3, 4, 5, 6]})
         my_dict = utils.dict_append(my_dict, "key_eg", [1, 2])
@@ -461,16 +469,16 @@
                     [21, 22, 23, 24, 25],
                     [23, 24, 25, 25, 25],
                 ],
             ),
         ]
         for test_value, kernel_size, strides, expected in tests:
             self.assertEqual(
-                list(utils.get_batch_strides(test_value, kernel_size, strides)),
-                expected,
+                    list(utils.get_batch_strides(test_value, kernel_size, strides)),
+                    expected,
             )
 
 
 class CjTestTest(unittest.TestCase):
     def test_add_check(self):
         pass
```

