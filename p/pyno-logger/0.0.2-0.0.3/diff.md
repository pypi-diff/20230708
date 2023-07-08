# Comparing `tmp/pyno_logger-0.0.2.tar.gz` & `tmp/pyno_logger-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/ben/projects/open-source/pyno-logger/dist/.tmp-clmo55fs/pyno_logger-0.0.2.tar", last modified: Fri Jul  7 19:47:59 2023, max compression
+gzip compressed data, was "/Users/ben/projects/open-source/pyno-logger/dist/.tmp-loj6a5ad/pyno_logger-0.0.3.tar", last modified: Sat Jul  8 00:59:36 2023, max compression
```

## Comparing `pyno_logger-0.0.2.tar` & `pyno_logger-0.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 ben        (501) staff       (20)        0 2023-07-07 19:47:59.366493 pyno_logger-0.0.2/
--rw-r--r--   0 ben        (501) staff       (20)     1066 2023-07-07 05:59:36.000000 pyno_logger-0.0.2/LICENSE
--rw-r--r--   0 ben        (501) staff       (20)     5185 2023-07-07 19:47:59.366345 pyno_logger-0.0.2/PKG-INFO
--rw-r--r--   0 ben        (501) staff       (20)     4667 2023-07-07 19:47:47.000000 pyno_logger-0.0.2/README.md
-drwxr-xr-x   0 ben        (501) staff       (20)        0 2023-07-07 19:47:59.365459 pyno_logger-0.0.2/pyno_logger/
--rw-r--r--   0 ben        (501) staff       (20)       30 2023-07-07 19:29:37.000000 pyno_logger-0.0.2/pyno_logger/__init__.py
--rw-r--r--   0 ben        (501) staff       (20)     4696 2023-07-07 18:52:07.000000 pyno_logger-0.0.2/pyno_logger/pyno_logger.py
-drwxr-xr-x   0 ben        (501) staff       (20)        0 2023-07-07 19:47:59.366162 pyno_logger-0.0.2/pyno_logger.egg-info/
--rw-r--r--   0 ben        (501) staff       (20)     5185 2023-07-07 19:47:59.000000 pyno_logger-0.0.2/pyno_logger.egg-info/PKG-INFO
--rw-r--r--   0 ben        (501) staff       (20)      223 2023-07-07 19:47:59.000000 pyno_logger-0.0.2/pyno_logger.egg-info/SOURCES.txt
--rw-r--r--   0 ben        (501) staff       (20)        1 2023-07-07 19:47:59.000000 pyno_logger-0.0.2/pyno_logger.egg-info/dependency_links.txt
--rw-r--r--   0 ben        (501) staff       (20)       12 2023-07-07 19:47:59.000000 pyno_logger-0.0.2/pyno_logger.egg-info/top_level.txt
--rw-r--r--   0 ben        (501) staff       (20)      503 2023-07-07 19:47:52.000000 pyno_logger-0.0.2/pyproject.toml
--rw-r--r--   0 ben        (501) staff       (20)       38 2023-07-07 19:47:59.366550 pyno_logger-0.0.2/setup.cfg
+drwxr-xr-x   0 ben        (501) staff       (20)        0 2023-07-08 00:59:36.825373 pyno_logger-0.0.3/
+-rw-r--r--   0 ben        (501) staff       (20)     1066 2023-07-07 05:59:36.000000 pyno_logger-0.0.3/LICENSE
+-rw-r--r--   0 ben        (501) staff       (20)     5299 2023-07-08 00:59:36.825251 pyno_logger-0.0.3/PKG-INFO
+-rw-r--r--   0 ben        (501) staff       (20)     4781 2023-07-08 00:59:14.000000 pyno_logger-0.0.3/README.md
+drwxr-xr-x   0 ben        (501) staff       (20)        0 2023-07-08 00:59:36.824605 pyno_logger-0.0.3/pyno_logger/
+-rw-r--r--   0 ben        (501) staff       (20)       30 2023-07-07 19:29:37.000000 pyno_logger-0.0.3/pyno_logger/__init__.py
+-rw-r--r--   0 ben        (501) staff       (20)     4845 2023-07-08 00:55:23.000000 pyno_logger-0.0.3/pyno_logger/pyno_logger.py
+drwxr-xr-x   0 ben        (501) staff       (20)        0 2023-07-08 00:59:36.825079 pyno_logger-0.0.3/pyno_logger.egg-info/
+-rw-r--r--   0 ben        (501) staff       (20)     5299 2023-07-08 00:59:36.000000 pyno_logger-0.0.3/pyno_logger.egg-info/PKG-INFO
+-rw-r--r--   0 ben        (501) staff       (20)      223 2023-07-08 00:59:36.000000 pyno_logger-0.0.3/pyno_logger.egg-info/SOURCES.txt
+-rw-r--r--   0 ben        (501) staff       (20)        1 2023-07-08 00:59:36.000000 pyno_logger-0.0.3/pyno_logger.egg-info/dependency_links.txt
+-rw-r--r--   0 ben        (501) staff       (20)       12 2023-07-08 00:59:36.000000 pyno_logger-0.0.3/pyno_logger.egg-info/top_level.txt
+-rw-r--r--   0 ben        (501) staff       (20)      503 2023-07-08 00:59:28.000000 pyno_logger-0.0.3/pyproject.toml
+-rw-r--r--   0 ben        (501) staff       (20)       38 2023-07-08 00:59:36.825422 pyno_logger-0.0.3/setup.cfg
```

### Comparing `pyno_logger-0.0.2/LICENSE` & `pyno_logger-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyno_logger-0.0.2/PKG-INFO` & `pyno_logger-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyno_logger
-Version: 0.0.2
+Version: 0.0.3
 Summary: A JSON logger for Python, inspired by Pino.
 Author-email: Ben Miner <ben@getampt.com>
 Project-URL: Homepage, https://github.com/benminer/pyno-logger
 Project-URL: Bug Tracker, https://github.com/benminer/pyno-logger/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -30,18 +30,20 @@
 
 ```python
 from pyno_logger import Pyno
 
 logger = Pyno(config={"level": "INFO"}, mixin=SomeFunction)
 ```
 
-The `Pyno` class takes am optional configuration dictionary as an argument. The configuration options are as follows:
+The `Pyno` class takes an optional configuration dictionary as an argument. The configuration options are as follows:
 
 - `level` (optional): Specifies the log level. Valid log levels are "ERROR", "WARNING", "INFO", "DEBUG", "TRACE", and "SILENT". The default log level is "INFO". By default, Pyno uses the `LOG_LEVEL` environment variable if nothing is passed via the `config` dict.
 
+- `base` (optional): Dictionary with any base configuration that is applied to all logs.
+
 - `omitted_keys` (optional): Specifies a list of keys to omit from the logged data. It can be a list, tuple, or comma-separated string.
 - `newlines` (optional): Specifies whether to append a newline character to the end of each log message. It should be a boolean value.
 
 The second param, `mixin`, allows for injecting a function that returns additional contextual data. Useful for any global state or dynamic data.
 
 - `mixin` (optional): Specifies a mixin function that returns a dictionary of additional data to include in log messages.
 
@@ -81,15 +83,15 @@
 
 ### Examples
 
 Here are some examples of how to use Pyno:
 
 ```python
 # Create a logger with default configuration
-logger = Pyno(config={"level": "INFO"})
+logger = Pyno()
 
 logger.info("This is an informational message.")
 logger.warning({"user_id": 123}, "This is a warning message.")
 logger.error({"error_code": 500}, "An error occurred.")
 # or log an Exception instance
 logger.error(Exception('something went wrong!'), "An error occured")
 
@@ -115,7 +117,9 @@
 
 In the above example, the log messages will be printed to the console in JSON format.
 
 ## TODOS
 
 - Customizable Log Levels
 - Configurable Serializers for logging class instances
+- File destinations
+- Stack/Flush functionality
```

### Comparing `pyno_logger-0.0.2/README.md` & `pyno_logger-0.0.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -16,18 +16,20 @@
 
 ```python
 from pyno_logger import Pyno
 
 logger = Pyno(config={"level": "INFO"}, mixin=SomeFunction)
 ```
 
-The `Pyno` class takes am optional configuration dictionary as an argument. The configuration options are as follows:
+The `Pyno` class takes an optional configuration dictionary as an argument. The configuration options are as follows:
 
 - `level` (optional): Specifies the log level. Valid log levels are "ERROR", "WARNING", "INFO", "DEBUG", "TRACE", and "SILENT". The default log level is "INFO". By default, Pyno uses the `LOG_LEVEL` environment variable if nothing is passed via the `config` dict.
 
+- `base` (optional): Dictionary with any base configuration that is applied to all logs.
+
 - `omitted_keys` (optional): Specifies a list of keys to omit from the logged data. It can be a list, tuple, or comma-separated string.
 - `newlines` (optional): Specifies whether to append a newline character to the end of each log message. It should be a boolean value.
 
 The second param, `mixin`, allows for injecting a function that returns additional contextual data. Useful for any global state or dynamic data.
 
 - `mixin` (optional): Specifies a mixin function that returns a dictionary of additional data to include in log messages.
 
@@ -67,15 +69,15 @@
 
 ### Examples
 
 Here are some examples of how to use Pyno:
 
 ```python
 # Create a logger with default configuration
-logger = Pyno(config={"level": "INFO"})
+logger = Pyno()
 
 logger.info("This is an informational message.")
 logger.warning({"user_id": 123}, "This is a warning message.")
 logger.error({"error_code": 500}, "An error occurred.")
 # or log an Exception instance
 logger.error(Exception('something went wrong!'), "An error occured")
 
@@ -101,7 +103,9 @@
 
 In the above example, the log messages will be printed to the console in JSON format.
 
 ## TODOS
 
 - Customizable Log Levels
 - Configurable Serializers for logging class instances
+- File destinations
+- Stack/Flush functionality
```

### Comparing `pyno_logger-0.0.2/pyno_logger/pyno_logger.py` & `pyno_logger-0.0.3/pyno_logger/pyno_logger.py`

 * *Files 3% similar despite different names*

```diff
@@ -74,14 +74,18 @@
             and config["level"] in LogLevel.keys()
         ):
             self.log_level = config["level"]
 
         if mixin and callable(mixin):
             self.mixin = mixin
 
+        if config.get("base"):
+            if isinstance(config["base"], dict):
+                self.base_ctx = {**self.base_ctx, **config["base"]}
+
     def log(self, level, data, message=None):
         level_num = LogLevel.get(level)
 
         if not level_num or not isinstance(level_num, int):
             raise Exception(f"Invalid log level: {level}")
 
         if self.log_level == "SILENT" or level_num == 0:
```

### Comparing `pyno_logger-0.0.2/pyno_logger.egg-info/PKG-INFO` & `pyno_logger-0.0.3/pyno_logger.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyno-logger
-Version: 0.0.2
+Version: 0.0.3
 Summary: A JSON logger for Python, inspired by Pino.
 Author-email: Ben Miner <ben@getampt.com>
 Project-URL: Homepage, https://github.com/benminer/pyno-logger
 Project-URL: Bug Tracker, https://github.com/benminer/pyno-logger/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -30,18 +30,20 @@
 
 ```python
 from pyno_logger import Pyno
 
 logger = Pyno(config={"level": "INFO"}, mixin=SomeFunction)
 ```
 
-The `Pyno` class takes am optional configuration dictionary as an argument. The configuration options are as follows:
+The `Pyno` class takes an optional configuration dictionary as an argument. The configuration options are as follows:
 
 - `level` (optional): Specifies the log level. Valid log levels are "ERROR", "WARNING", "INFO", "DEBUG", "TRACE", and "SILENT". The default log level is "INFO". By default, Pyno uses the `LOG_LEVEL` environment variable if nothing is passed via the `config` dict.
 
+- `base` (optional): Dictionary with any base configuration that is applied to all logs.
+
 - `omitted_keys` (optional): Specifies a list of keys to omit from the logged data. It can be a list, tuple, or comma-separated string.
 - `newlines` (optional): Specifies whether to append a newline character to the end of each log message. It should be a boolean value.
 
 The second param, `mixin`, allows for injecting a function that returns additional contextual data. Useful for any global state or dynamic data.
 
 - `mixin` (optional): Specifies a mixin function that returns a dictionary of additional data to include in log messages.
 
@@ -81,15 +83,15 @@
 
 ### Examples
 
 Here are some examples of how to use Pyno:
 
 ```python
 # Create a logger with default configuration
-logger = Pyno(config={"level": "INFO"})
+logger = Pyno()
 
 logger.info("This is an informational message.")
 logger.warning({"user_id": 123}, "This is a warning message.")
 logger.error({"error_code": 500}, "An error occurred.")
 # or log an Exception instance
 logger.error(Exception('something went wrong!'), "An error occured")
 
@@ -115,7 +117,9 @@
 
 In the above example, the log messages will be printed to the console in JSON format.
 
 ## TODOS
 
 - Customizable Log Levels
 - Configurable Serializers for logging class instances
+- File destinations
+- Stack/Flush functionality
```

