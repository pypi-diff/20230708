# Comparing `tmp/pyno_logger-0.0.6.tar.gz` & `tmp/pyno_logger-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/ben/projects/open-source/pyno-logger/dist/.tmp-tx1gldxq/pyno_logger-0.0.6.tar", last modified: Sat Jul  8 01:21:15 2023, max compression
+gzip compressed data, was "/Users/ben/projects/open-source/pyno-logger/dist/.tmp-v9_eq_ml/pyno_logger-0.0.7.tar", last modified: Sat Jul  8 01:22:30 2023, max compression
```

## Comparing `pyno_logger-0.0.6.tar` & `pyno_logger-0.0.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 ben        (501) staff       (20)        0 2023-07-08 01:21:15.803133 pyno_logger-0.0.6/
--rw-r--r--   0 ben        (501) staff       (20)     1066 2023-07-07 05:59:36.000000 pyno_logger-0.0.6/LICENSE
--rw-r--r--   0 ben        (501) staff       (20)     5774 2023-07-08 01:21:15.803018 pyno_logger-0.0.6/PKG-INFO
--rw-r--r--   0 ben        (501) staff       (20)     5256 2023-07-08 01:20:52.000000 pyno_logger-0.0.6/README.md
-drwxr-xr-x   0 ben        (501) staff       (20)        0 2023-07-08 01:21:15.802394 pyno_logger-0.0.6/pyno_logger/
--rw-r--r--   0 ben        (501) staff       (20)       30 2023-07-07 19:29:37.000000 pyno_logger-0.0.6/pyno_logger/__init__.py
--rw-r--r--   0 ben        (501) staff       (20)     5771 2023-07-08 01:15:39.000000 pyno_logger-0.0.6/pyno_logger/pyno_logger.py
-drwxr-xr-x   0 ben        (501) staff       (20)        0 2023-07-08 01:21:15.802859 pyno_logger-0.0.6/pyno_logger.egg-info/
--rw-r--r--   0 ben        (501) staff       (20)     5774 2023-07-08 01:21:15.000000 pyno_logger-0.0.6/pyno_logger.egg-info/PKG-INFO
--rw-r--r--   0 ben        (501) staff       (20)      223 2023-07-08 01:21:15.000000 pyno_logger-0.0.6/pyno_logger.egg-info/SOURCES.txt
--rw-r--r--   0 ben        (501) staff       (20)        1 2023-07-08 01:21:15.000000 pyno_logger-0.0.6/pyno_logger.egg-info/dependency_links.txt
--rw-r--r--   0 ben        (501) staff       (20)       12 2023-07-08 01:21:15.000000 pyno_logger-0.0.6/pyno_logger.egg-info/top_level.txt
--rw-r--r--   0 ben        (501) staff       (20)      503 2023-07-08 01:21:11.000000 pyno_logger-0.0.6/pyproject.toml
--rw-r--r--   0 ben        (501) staff       (20)       38 2023-07-08 01:21:15.803176 pyno_logger-0.0.6/setup.cfg
+drwxr-xr-x   0 ben        (501) staff       (20)        0 2023-07-08 01:22:30.325380 pyno_logger-0.0.7/
+-rw-r--r--   0 ben        (501) staff       (20)     1066 2023-07-07 05:59:36.000000 pyno_logger-0.0.7/LICENSE
+-rw-r--r--   0 ben        (501) staff       (20)     5783 2023-07-08 01:22:30.325252 pyno_logger-0.0.7/PKG-INFO
+-rw-r--r--   0 ben        (501) staff       (20)     5265 2023-07-08 01:22:18.000000 pyno_logger-0.0.7/README.md
+drwxr-xr-x   0 ben        (501) staff       (20)        0 2023-07-08 01:22:30.324616 pyno_logger-0.0.7/pyno_logger/
+-rw-r--r--   0 ben        (501) staff       (20)       30 2023-07-07 19:29:37.000000 pyno_logger-0.0.7/pyno_logger/__init__.py
+-rw-r--r--   0 ben        (501) staff       (20)     5771 2023-07-08 01:15:39.000000 pyno_logger-0.0.7/pyno_logger/pyno_logger.py
+drwxr-xr-x   0 ben        (501) staff       (20)        0 2023-07-08 01:22:30.325088 pyno_logger-0.0.7/pyno_logger.egg-info/
+-rw-r--r--   0 ben        (501) staff       (20)     5783 2023-07-08 01:22:30.000000 pyno_logger-0.0.7/pyno_logger.egg-info/PKG-INFO
+-rw-r--r--   0 ben        (501) staff       (20)      223 2023-07-08 01:22:30.000000 pyno_logger-0.0.7/pyno_logger.egg-info/SOURCES.txt
+-rw-r--r--   0 ben        (501) staff       (20)        1 2023-07-08 01:22:30.000000 pyno_logger-0.0.7/pyno_logger.egg-info/dependency_links.txt
+-rw-r--r--   0 ben        (501) staff       (20)       12 2023-07-08 01:22:30.000000 pyno_logger-0.0.7/pyno_logger.egg-info/top_level.txt
+-rw-r--r--   0 ben        (501) staff       (20)      503 2023-07-08 01:22:24.000000 pyno_logger-0.0.7/pyproject.toml
+-rw-r--r--   0 ben        (501) staff       (20)       38 2023-07-08 01:22:30.325431 pyno_logger-0.0.7/setup.cfg
```

### Comparing `pyno_logger-0.0.6/LICENSE` & `pyno_logger-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pyno_logger-0.0.6/PKG-INFO` & `pyno_logger-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyno_logger
-Version: 0.0.6
+Version: 0.0.7
 Summary: A JSON logger for Python, inspired by Pino.
 Author-email: Ben Miner <ben@getampt.com>
 Project-URL: Homepage, https://github.com/benminer/pyno-logger
 Project-URL: Bug Tracker, https://github.com/benminer/pyno-logger/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -32,15 +32,15 @@
 from pyno_logger import Pyno
 
 logger = Pyno(config={"level": "INFO"}, mixin=SomeFunction)
 ```
 
 The `Pyno` class takes an optional configuration dictionary as an argument. The configuration options are as follows:
 
-- `level` (optional): Specifies the log level. Valid log levels are "ERROR", "WARNING", "INFO", "DEBUG", "TRACE", and "SILENT". The default log level is "INFO". By default, Pyno uses the `LOG_LEVEL` environment variable if nothing is passed via the `config` dict.
+- `level` (optional): Specifies the log level. Valid log levels are "ERROR", "WARNING", "INFO", "DEBUG", "TRACE", "FATAL", and "SILENT". The default log level is "INFO". By default, Pyno uses the `LOG_LEVEL` environment variable if nothing is passed via the `config` dict.
 
 - `base` (optional): Dictionary with any base configuration that is applied to all logs.
 
 - `msg_key` (optional): Custom key value for the message value. Defaults to `msg`.
 
 - `error_key` (optional): Custom key value for Exception values. Defaults to `error`.
```

### Comparing `pyno_logger-0.0.6/README.md` & `pyno_logger-0.0.7/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 from pyno_logger import Pyno
 
 logger = Pyno(config={"level": "INFO"}, mixin=SomeFunction)
 ```
 
 The `Pyno` class takes an optional configuration dictionary as an argument. The configuration options are as follows:
 
-- `level` (optional): Specifies the log level. Valid log levels are "ERROR", "WARNING", "INFO", "DEBUG", "TRACE", and "SILENT". The default log level is "INFO". By default, Pyno uses the `LOG_LEVEL` environment variable if nothing is passed via the `config` dict.
+- `level` (optional): Specifies the log level. Valid log levels are "ERROR", "WARNING", "INFO", "DEBUG", "TRACE", "FATAL", and "SILENT". The default log level is "INFO". By default, Pyno uses the `LOG_LEVEL` environment variable if nothing is passed via the `config` dict.
 
 - `base` (optional): Dictionary with any base configuration that is applied to all logs.
 
 - `msg_key` (optional): Custom key value for the message value. Defaults to `msg`.
 
 - `error_key` (optional): Custom key value for Exception values. Defaults to `error`.
```

### Comparing `pyno_logger-0.0.6/pyno_logger/pyno_logger.py` & `pyno_logger-0.0.7/pyno_logger/pyno_logger.py`

 * *Files identical despite different names*

### Comparing `pyno_logger-0.0.6/pyno_logger.egg-info/PKG-INFO` & `pyno_logger-0.0.7/pyno_logger.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyno-logger
-Version: 0.0.6
+Version: 0.0.7
 Summary: A JSON logger for Python, inspired by Pino.
 Author-email: Ben Miner <ben@getampt.com>
 Project-URL: Homepage, https://github.com/benminer/pyno-logger
 Project-URL: Bug Tracker, https://github.com/benminer/pyno-logger/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -32,15 +32,15 @@
 from pyno_logger import Pyno
 
 logger = Pyno(config={"level": "INFO"}, mixin=SomeFunction)
 ```
 
 The `Pyno` class takes an optional configuration dictionary as an argument. The configuration options are as follows:
 
-- `level` (optional): Specifies the log level. Valid log levels are "ERROR", "WARNING", "INFO", "DEBUG", "TRACE", and "SILENT". The default log level is "INFO". By default, Pyno uses the `LOG_LEVEL` environment variable if nothing is passed via the `config` dict.
+- `level` (optional): Specifies the log level. Valid log levels are "ERROR", "WARNING", "INFO", "DEBUG", "TRACE", "FATAL", and "SILENT". The default log level is "INFO". By default, Pyno uses the `LOG_LEVEL` environment variable if nothing is passed via the `config` dict.
 
 - `base` (optional): Dictionary with any base configuration that is applied to all logs.
 
 - `msg_key` (optional): Custom key value for the message value. Defaults to `msg`.
 
 - `error_key` (optional): Custom key value for Exception values. Defaults to `error`.
```

