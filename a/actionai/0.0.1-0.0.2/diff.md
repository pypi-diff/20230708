# Comparing `tmp/actionai-0.0.1.tar.gz` & `tmp/actionai-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "actionai-0.0.1.tar", max compression
+gzip compressed data, was "actionai-0.0.2.tar", max compression
```

## Comparing `actionai-0.0.1.tar` & `actionai-0.0.2.tar`

### file list

```diff
@@ -1,7 +1,8 @@
--rw-r--r--   0        0        0        0 2023-07-08 07:12:09.277610 actionai-0.0.1/README.md
--rw-r--r--   0        0        0      536 2023-07-08 15:05:24.407281 actionai-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     3056 2023-07-08 14:58:23.858550 actionai-0.0.1/src/actionai/__init__.py
--rw-r--r--   0        0        0      599 2023-07-08 14:53:35.508670 actionai-0.0.1/src/actionai/json_schema.py
--rw-r--r--   0        0        0      800 2023-07-08 14:53:35.508673 actionai-0.0.1/src/actionai/types.py
--rw-r--r--   0        0        0      747 1970-01-01 00:00:00.000000 actionai-0.0.1/setup.py
--rw-r--r--   0        0        0      437 1970-01-01 00:00:00.000000 actionai-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-07-08 15:41:43.483740 actionai-0.0.2/LICENSE
+-rw-r--r--   0        0        0     1093 2023-07-08 15:41:43.484129 actionai-0.0.2/README.md
+-rw-r--r--   0        0        0      536 2023-07-08 15:43:27.894573 actionai-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     3056 2023-07-08 14:58:23.858550 actionai-0.0.2/src/actionai/__init__.py
+-rw-r--r--   0        0        0      599 2023-07-08 14:53:35.508670 actionai-0.0.2/src/actionai/json_schema.py
+-rw-r--r--   0        0        0      800 2023-07-08 14:53:35.508673 actionai-0.0.2/src/actionai/types.py
+-rw-r--r--   0        0        0     1887 1970-01-01 00:00:00.000000 actionai-0.0.2/setup.py
+-rw-r--r--   0        0        0     1530 1970-01-01 00:00:00.000000 actionai-0.0.2/PKG-INFO
```

### Comparing `actionai-0.0.1/pyproject.toml` & `actionai-0.0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "actionai"
-version = "0.0.1"
+version = "0.0.2"
 description = "A small library to call local functions using openai function calling"
 authors = ["Amal Shaji <amalshajid@gmail.com>"]
 readme = "README.md"
 packages = [{include = "actionai", from = "src"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `actionai-0.0.1/src/actionai/__init__.py` & `actionai-0.0.2/src/actionai/__init__.py`

 * *Files identical despite different names*

### Comparing `actionai-0.0.1/src/actionai/json_schema.py` & `actionai-0.0.2/src/actionai/json_schema.py`

 * *Files identical despite different names*

### Comparing `actionai-0.0.1/src/actionai/types.py` & `actionai-0.0.2/src/actionai/types.py`

 * *Files identical despite different names*

