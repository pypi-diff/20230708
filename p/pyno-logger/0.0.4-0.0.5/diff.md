# Comparing `tmp/pyno_logger-0.0.4.tar.gz` & `tmp/pyno_logger-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/ben/projects/open-source/pyno-logger/dist/.tmp-z8i8h2d0/pyno_logger-0.0.4.tar", last modified: Sat Jul  8 01:17:12 2023, max compression
+gzip compressed data, was "/Users/ben/projects/open-source/pyno-logger/dist/.tmp-qtrngdxg/pyno_logger-0.0.5.tar", last modified: Sat Jul  8 01:18:47 2023, max compression
```

## Comparing `pyno_logger-0.0.4.tar` & `pyno_logger-0.0.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 ben        (501) staff       (20)        0 2023-07-08 01:17:12.155174 pyno_logger-0.0.4/
--rw-r--r--   0 ben        (501) staff       (20)     1066 2023-07-07 05:59:36.000000 pyno_logger-0.0.4/LICENSE
--rw-r--r--   0 ben        (501) staff       (20)     5480 2023-07-08 01:17:12.155060 pyno_logger-0.0.4/PKG-INFO
--rw-r--r--   0 ben        (501) staff       (20)     4962 2023-07-08 01:16:32.000000 pyno_logger-0.0.4/README.md
-drwxr-xr-x   0 ben        (501) staff       (20)        0 2023-07-08 01:17:12.154439 pyno_logger-0.0.4/pyno_logger/
--rw-r--r--   0 ben        (501) staff       (20)       30 2023-07-07 19:29:37.000000 pyno_logger-0.0.4/pyno_logger/__init__.py
--rw-r--r--   0 ben        (501) staff       (20)     5771 2023-07-08 01:15:39.000000 pyno_logger-0.0.4/pyno_logger/pyno_logger.py
-drwxr-xr-x   0 ben        (501) staff       (20)        0 2023-07-08 01:17:12.154908 pyno_logger-0.0.4/pyno_logger.egg-info/
--rw-r--r--   0 ben        (501) staff       (20)     5480 2023-07-08 01:17:12.000000 pyno_logger-0.0.4/pyno_logger.egg-info/PKG-INFO
--rw-r--r--   0 ben        (501) staff       (20)      223 2023-07-08 01:17:12.000000 pyno_logger-0.0.4/pyno_logger.egg-info/SOURCES.txt
--rw-r--r--   0 ben        (501) staff       (20)        1 2023-07-08 01:17:12.000000 pyno_logger-0.0.4/pyno_logger.egg-info/dependency_links.txt
--rw-r--r--   0 ben        (501) staff       (20)       12 2023-07-08 01:17:12.000000 pyno_logger-0.0.4/pyno_logger.egg-info/top_level.txt
--rw-r--r--   0 ben        (501) staff       (20)      503 2023-07-08 01:17:04.000000 pyno_logger-0.0.4/pyproject.toml
--rw-r--r--   0 ben        (501) staff       (20)       38 2023-07-08 01:17:12.155216 pyno_logger-0.0.4/setup.cfg
+drwxr-xr-x   0 ben        (501) staff       (20)        0 2023-07-08 01:18:47.457713 pyno_logger-0.0.5/
+-rw-r--r--   0 ben        (501) staff       (20)     1066 2023-07-07 05:59:36.000000 pyno_logger-0.0.5/LICENSE
+-rw-r--r--   0 ben        (501) staff       (20)     5603 2023-07-08 01:18:47.457595 pyno_logger-0.0.5/PKG-INFO
+-rw-r--r--   0 ben        (501) staff       (20)     5085 2023-07-08 01:18:38.000000 pyno_logger-0.0.5/README.md
+drwxr-xr-x   0 ben        (501) staff       (20)        0 2023-07-08 01:18:47.456954 pyno_logger-0.0.5/pyno_logger/
+-rw-r--r--   0 ben        (501) staff       (20)       30 2023-07-07 19:29:37.000000 pyno_logger-0.0.5/pyno_logger/__init__.py
+-rw-r--r--   0 ben        (501) staff       (20)     5771 2023-07-08 01:15:39.000000 pyno_logger-0.0.5/pyno_logger/pyno_logger.py
+drwxr-xr-x   0 ben        (501) staff       (20)        0 2023-07-08 01:18:47.457442 pyno_logger-0.0.5/pyno_logger.egg-info/
+-rw-r--r--   0 ben        (501) staff       (20)     5603 2023-07-08 01:18:47.000000 pyno_logger-0.0.5/pyno_logger.egg-info/PKG-INFO
+-rw-r--r--   0 ben        (501) staff       (20)      223 2023-07-08 01:18:47.000000 pyno_logger-0.0.5/pyno_logger.egg-info/SOURCES.txt
+-rw-r--r--   0 ben        (501) staff       (20)        1 2023-07-08 01:18:47.000000 pyno_logger-0.0.5/pyno_logger.egg-info/dependency_links.txt
+-rw-r--r--   0 ben        (501) staff       (20)       12 2023-07-08 01:18:47.000000 pyno_logger-0.0.5/pyno_logger.egg-info/top_level.txt
+-rw-r--r--   0 ben        (501) staff       (20)      503 2023-07-08 01:18:43.000000 pyno_logger-0.0.5/pyproject.toml
+-rw-r--r--   0 ben        (501) staff       (20)       38 2023-07-08 01:18:47.457754 pyno_logger-0.0.5/setup.cfg
```

### Comparing `pyno_logger-0.0.4/LICENSE` & `pyno_logger-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pyno_logger-0.0.4/PKG-INFO` & `pyno_logger-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyno_logger
-Version: 0.0.4
+Version: 0.0.5
 Summary: A JSON logger for Python, inspired by Pino.
 Author-email: Ben Miner <ben@getampt.com>
 Project-URL: Homepage, https://github.com/benminer/pyno-logger
 Project-URL: Bug Tracker, https://github.com/benminer/pyno-logger/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -54,23 +54,25 @@
 
 - `info(data={}, message=None)`: Logs an informational message with the provided data and an optional message.
 - `warning(data={}, message=None)`: Logs a warning message with the provided data and an optional message.
 - `warn(data={}, message=None)`: Logs a warning message (alias for `warning`).
 - `debug(data={}, message=None)`: Logs a debug message with the provided data and an optional message.
 - `trace(data={}, message=None)`: Logs a trace message with the provided data and an optional message.
 - `error(data={}, message=None)`: Logs an error message with the provided data and an optional message.
+- `fatal(data={}, message=None)`: Logs a fatal error message with the provided data and an optional message.
 
 Each logging method takes two optional arguments: `data` and `message`. The `data` argument can be a dictionary, list, tuple, string, or Exception object containing additional contextual data. The `message` argument is a string that represents the log message. If not provided, the log message will be automatically generated based on the log level and data.
 
 By default, Pyno includes the fields `time`, `pid`, `hostname` and `level`. These can be omitted via the `omitted_keys` config param, if desired.
 
 ### Log Levels
 
 Pyno uses the following log levels:
 
+- `FATAL`: 60
 - `ERROR`: 50
 - `WARNING`: 40
 - `INFO`: 30
 - `DEBUG`: 20
 - `TRACE`: 10
 - `SILENT`: 0
```

### Comparing `pyno_logger-0.0.4/README.md` & `pyno_logger-0.0.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -40,23 +40,25 @@
 
 - `info(data={}, message=None)`: Logs an informational message with the provided data and an optional message.
 - `warning(data={}, message=None)`: Logs a warning message with the provided data and an optional message.
 - `warn(data={}, message=None)`: Logs a warning message (alias for `warning`).
 - `debug(data={}, message=None)`: Logs a debug message with the provided data and an optional message.
 - `trace(data={}, message=None)`: Logs a trace message with the provided data and an optional message.
 - `error(data={}, message=None)`: Logs an error message with the provided data and an optional message.
+- `fatal(data={}, message=None)`: Logs a fatal error message with the provided data and an optional message.
 
 Each logging method takes two optional arguments: `data` and `message`. The `data` argument can be a dictionary, list, tuple, string, or Exception object containing additional contextual data. The `message` argument is a string that represents the log message. If not provided, the log message will be automatically generated based on the log level and data.
 
 By default, Pyno includes the fields `time`, `pid`, `hostname` and `level`. These can be omitted via the `omitted_keys` config param, if desired.
 
 ### Log Levels
 
 Pyno uses the following log levels:
 
+- `FATAL`: 60
 - `ERROR`: 50
 - `WARNING`: 40
 - `INFO`: 30
 - `DEBUG`: 20
 - `TRACE`: 10
 - `SILENT`: 0
```

### Comparing `pyno_logger-0.0.4/pyno_logger/pyno_logger.py` & `pyno_logger-0.0.5/pyno_logger/pyno_logger.py`

 * *Files identical despite different names*

### Comparing `pyno_logger-0.0.4/pyno_logger.egg-info/PKG-INFO` & `pyno_logger-0.0.5/pyno_logger.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyno-logger
-Version: 0.0.4
+Version: 0.0.5
 Summary: A JSON logger for Python, inspired by Pino.
 Author-email: Ben Miner <ben@getampt.com>
 Project-URL: Homepage, https://github.com/benminer/pyno-logger
 Project-URL: Bug Tracker, https://github.com/benminer/pyno-logger/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -54,23 +54,25 @@
 
 - `info(data={}, message=None)`: Logs an informational message with the provided data and an optional message.
 - `warning(data={}, message=None)`: Logs a warning message with the provided data and an optional message.
 - `warn(data={}, message=None)`: Logs a warning message (alias for `warning`).
 - `debug(data={}, message=None)`: Logs a debug message with the provided data and an optional message.
 - `trace(data={}, message=None)`: Logs a trace message with the provided data and an optional message.
 - `error(data={}, message=None)`: Logs an error message with the provided data and an optional message.
+- `fatal(data={}, message=None)`: Logs a fatal error message with the provided data and an optional message.
 
 Each logging method takes two optional arguments: `data` and `message`. The `data` argument can be a dictionary, list, tuple, string, or Exception object containing additional contextual data. The `message` argument is a string that represents the log message. If not provided, the log message will be automatically generated based on the log level and data.
 
 By default, Pyno includes the fields `time`, `pid`, `hostname` and `level`. These can be omitted via the `omitted_keys` config param, if desired.
 
 ### Log Levels
 
 Pyno uses the following log levels:
 
+- `FATAL`: 60
 - `ERROR`: 50
 - `WARNING`: 40
 - `INFO`: 30
 - `DEBUG`: 20
 - `TRACE`: 10
 - `SILENT`: 0
```

