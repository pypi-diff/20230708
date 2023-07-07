# Comparing `tmp/socket-log-receiver-20.4.1a0.tar.gz` & `tmp/socket-log-receiver-23.7.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/socket-log-receiver-20.4.1a0.tar", last modified: Mon Apr 20 04:10:38 2020, max compression
+gzip compressed data, was "socket-log-receiver-23.7.0a0.tar", last modified: Fri Jul  7 21:59:22 2023, max compression
```

## Comparing `socket-log-receiver-20.4.1a0.tar` & `socket-log-receiver-23.7.0a0.tar`

### file list

```diff
@@ -1,21 +1,19 @@
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2020-04-20 04:10:38.000000 socket-log-receiver-20.4.1a0/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1073 2020-04-20 04:10:16.000000 socket-log-receiver-20.4.1a0/LICENSE.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       20 2020-04-20 04:10:16.000000 socket-log-receiver-20.4.1a0/MANIFEST.in
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3048 2020-04-20 04:10:38.000000 socket-log-receiver-20.4.1a0/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1796 2020-04-20 04:10:16.000000 socket-log-receiver-20.4.1a0/README.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)      883 2020-04-20 04:10:16.000000 socket-log-receiver-20.4.1a0/pyproject.toml
--rw-r--r--   0 circleci  (3434) circleci  (3434)      173 2020-04-20 04:10:38.000000 socket-log-receiver-20.4.1a0/setup.cfg
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2358 2020-04-20 04:10:16.000000 socket-log-receiver-20.4.1a0/setup.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2020-04-20 04:10:38.000000 socket-log-receiver-20.4.1a0/src/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2020-04-20 04:10:38.000000 socket-log-receiver-20.4.1a0/src/socket_log_receiver/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      137 2020-04-20 04:10:16.000000 socket-log-receiver-20.4.1a0/src/socket_log_receiver/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      516 2020-04-20 04:10:16.000000 socket-log-receiver-20.4.1a0/src/socket_log_receiver/__main__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      515 2020-04-20 04:10:16.000000 socket-log-receiver-20.4.1a0/src/socket_log_receiver/config.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3083 2020-04-20 04:10:16.000000 socket-log-receiver-20.4.1a0/src/socket_log_receiver/receivers.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2020-04-20 04:10:38.000000 socket-log-receiver-20.4.1a0/src/socket_log_receiver.egg-info/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3048 2020-04-20 04:10:38.000000 socket-log-receiver-20.4.1a0/src/socket_log_receiver.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)      494 2020-04-20 04:10:38.000000 socket-log-receiver-20.4.1a0/src/socket_log_receiver.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2020-04-20 04:10:38.000000 socket-log-receiver-20.4.1a0/src/socket_log_receiver.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       68 2020-04-20 04:10:38.000000 socket-log-receiver-20.4.1a0/src/socket_log_receiver.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)      299 2020-04-20 04:10:38.000000 socket-log-receiver-20.4.1a0/src/socket_log_receiver.egg-info/requires.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       20 2020-04-20 04:10:38.000000 socket-log-receiver-20.4.1a0/src/socket_log_receiver.egg-info/top_level.txt
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-07 21:59:22.606831 socket-log-receiver-23.7.0a0/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1073 2023-07-07 21:59:03.000000 socket-log-receiver-23.7.0a0/LICENSE.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3108 2023-07-07 21:59:22.606831 socket-log-receiver-23.7.0a0/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2143 2023-07-07 21:59:03.000000 socket-log-receiver-23.7.0a0/README.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2253 2023-07-07 21:59:03.000000 socket-log-receiver-23.7.0a0/pyproject.toml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2023-07-07 21:59:22.606831 socket-log-receiver-23.7.0a0/setup.cfg
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-07 21:59:22.602831 socket-log-receiver-23.7.0a0/src/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-07 21:59:22.602831 socket-log-receiver-23.7.0a0/src/socket_log_receiver/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-07-07 21:59:03.000000 socket-log-receiver-23.7.0a0/src/socket_log_receiver/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      516 2023-07-07 21:59:03.000000 socket-log-receiver-23.7.0a0/src/socket_log_receiver/__main__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      515 2023-07-07 21:59:03.000000 socket-log-receiver-23.7.0a0/src/socket_log_receiver/config.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3087 2023-07-07 21:59:03.000000 socket-log-receiver-23.7.0a0/src/socket_log_receiver/receivers.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-07 21:59:22.606831 socket-log-receiver-23.7.0a0/src/socket_log_receiver.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3108 2023-07-07 21:59:22.000000 socket-log-receiver-23.7.0a0/src/socket_log_receiver.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      463 2023-07-07 21:59:22.000000 socket-log-receiver-23.7.0a0/src/socket_log_receiver.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-07-07 21:59:22.000000 socket-log-receiver-23.7.0a0/src/socket_log_receiver.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       67 2023-07-07 21:59:22.000000 socket-log-receiver-23.7.0a0/src/socket_log_receiver.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      204 2023-07-07 21:59:22.000000 socket-log-receiver-23.7.0a0/src/socket_log_receiver.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       20 2023-07-07 21:59:22.000000 socket-log-receiver-23.7.0a0/src/socket_log_receiver.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `socket-log-receiver-20.4.1a0/LICENSE.txt` & `socket-log-receiver-23.7.0a0/LICENSE.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2018 - 2020 Taro Sato
+Copyright (c) 2018 - 2023 Taro Sato
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `socket-log-receiver-20.4.1a0/PKG-INFO` & `socket-log-receiver-23.7.0a0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,81 +1,85 @@
 Metadata-Version: 2.1
 Name: socket-log-receiver
-Version: 20.4.1a0
+Version: 23.7.0a0
 Summary: A light-weight socket log receiver
-Home-page: https://github.com/okomestudio/socket-log-receiver
-Author: Taro Sato
-Author-email: okomestudio@gmail.com
-License: MIT
-Description: [![pyversion Status](https://img.shields.io/pypi/pyversions/socket-log-receiver.svg)](https://img.shields.io/pypi/pyversions/socket-log-receiver.svg)
-        [![CircleCI](https://circleci.com/gh/okomestudio/socket-log-receiver.svg?style=shield)](https://circleci.com/gh/okomestudio/socket-log-receiver)
-        [![Coverage Status](https://coveralls.io/repos/github/okomestudio/socket-log-receiver/badge.svg?branch=development)](https://coveralls.io/github/okomestudio/socket-log-receiver?branch=development&kill_cache=1)
-        [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
-        
-        
-        # Socket Log Receiver
-        
-        `socket_log_receiver` is a light-weight socket log receiver. It runs
-        as a server and aggregates messages from multi-process application via
-        socket and logs to a single file. Python's `logging` package does not
-        support logging to a single file from multiple processes. By pointing
-        `SocketHandler` to `socket_log_receiver`, the multi-process
-        application can log to a single file.
-        
-        
-        ## Installation
-        
-        ``` bash
-        $ pip install socket-log-receiver
-        ```
-        
-        
-        ## Basic Usage
-        
-        The receiver service should be run as a service.
-        
-        ``` bash
-        $ python -m socket_log_receiver  # as a module
-        $ log_receiver                   # as a command-line program
-        ```
-        
-        In the application, use `SocketHandler` to send logs to the receiver
-        service.
-        
-        ``` python
-        from logging.handlers import SocketHandler
-        
-        handler = SocketHandler('localhost', 9020)  # handler to send logs to localhost:9020
-        logging.root.addHandler(handler)            # add the socket handler to the root logger
-        ```
-        
-        This way, the root logger sends logging messages to the receiver service.
-        
-        
-        ## Development
-        
-        ```bash
-        $ pip install -e .[dev]
-        $ pre-commit install
-        ```
-        
-        
-        ### Running Tests
-        
-        ``` bash
-        $ python setup.py tests
-        ```
-        
-Platform: Linux
+Author-email: Taro Sato <okomestudio@gmail.com>
+Project-URL: Homepage, https://github.com/okomestudio/socket-log-receiver
+Project-URL: Buck Tracker, https://github.com/okomestudio/socket-log-receiver/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Utilities
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: test
+License-File: LICENSE.txt
+
+[![License](https://img.shields.io/pypi/l/socket-log-receiver.svg)](https://pypi.org/project/socket-log-receiver/)
+[![PyPI Version](https://badge.fury.io/py/socket-log-receiver.svg)](https://pypi.org/project/socket-log-receiver/)
+[![Package Status](https://img.shields.io/pypi/status/socket-log-receiver.svg)](https://pypi.org/project/resconfig/)
+[![pyversion Status](https://img.shields.io/pypi/pyversions/socket-log-receiver.svg)](https://img.shields.io/pypi/pyversions/socket-log-receiver.svg)
+[![CircleCI](https://circleci.com/gh/okomestudio/socket-log-receiver.svg?style=shield)](https://circleci.com/gh/okomestudio/socket-log-receiver)
+[![Coverage Status](https://coveralls.io/repos/github/okomestudio/socket-log-receiver/badge.svg?branch=development)](https://coveralls.io/github/okomestudio/socket-log-receiver?branch=development&kill_cache=1)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+
+
+# Socket Log Receiver
+
+`socket_log_receiver` is a light-weight socket log receiver. It runs
+as a server and aggregates messages from multi-process application via
+socket and logs to a single file. Python's `logging` package does not
+support logging to a single file from multiple processes. By pointing
+`SocketHandler` to `socket_log_receiver`, the multi-process
+application can log to a single file.
+
+
+## Installation
+
+``` bash
+$ pip install socket-log-receiver
+```
+
+
+## Basic Usage
+
+The receiver service should be run as a service.
+
+``` bash
+$ python -m socket_log_receiver  # as a module
+$ log_receiver                   # as a command-line program
+```
+
+In the application, use `SocketHandler` to send logs to the receiver
+service.
+
+``` python
+from logging.handlers import SocketHandler
+
+handler = SocketHandler('localhost', 9020)  # handler to send logs to localhost:9020
+logging.root.addHandler(handler)            # add the socket handler to the root logger
+```
+
+This way, the root logger sends logging messages to the receiver service.
+
+
+## Development
+
+```bash
+$ pip install -e .[dev]
+$ pre-commit install
+```
+
+
+### Running Tests
+
+``` bash
+$ python setup.py tests
+```
```

### Comparing `socket-log-receiver-20.4.1a0/README.md` & `socket-log-receiver-23.7.0a0/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+[![License](https://img.shields.io/pypi/l/socket-log-receiver.svg)](https://pypi.org/project/socket-log-receiver/)
+[![PyPI Version](https://badge.fury.io/py/socket-log-receiver.svg)](https://pypi.org/project/socket-log-receiver/)
+[![Package Status](https://img.shields.io/pypi/status/socket-log-receiver.svg)](https://pypi.org/project/resconfig/)
 [![pyversion Status](https://img.shields.io/pypi/pyversions/socket-log-receiver.svg)](https://img.shields.io/pypi/pyversions/socket-log-receiver.svg)
 [![CircleCI](https://circleci.com/gh/okomestudio/socket-log-receiver.svg?style=shield)](https://circleci.com/gh/okomestudio/socket-log-receiver)
 [![Coverage Status](https://coveralls.io/repos/github/okomestudio/socket-log-receiver/badge.svg?branch=development)](https://coveralls.io/github/okomestudio/socket-log-receiver?branch=development&kill_cache=1)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 
 # Socket Log Receiver
```

### Comparing `socket-log-receiver-20.4.1a0/src/socket_log_receiver/__main__.py` & `socket-log-receiver-23.7.0a0/src/socket_log_receiver/__main__.py`

 * *Files identical despite different names*

### Comparing `socket-log-receiver-20.4.1a0/src/socket_log_receiver/config.py` & `socket-log-receiver-23.7.0a0/src/socket_log_receiver/config.py`

 * *Files identical despite different names*

### Comparing `socket-log-receiver-20.4.1a0/src/socket_log_receiver/receivers.py` & `socket-log-receiver-23.7.0a0/src/socket_log_receiver/receivers.py`

 * *Files 7% similar despite different names*

```diff
@@ -47,29 +47,28 @@
         else:
             name = record.name
         logger = logging.getLogger(name)
         logger.handle(record)
 
 
 class Receiver(ThreadingTCPServer):
-
     allow_reuse_address = True
 
     def __init__(
         self,
         host,
         port,
         handler=_Handler,
         bind_and_activate=True,
         abort=0,
         timeout=1,
         logname=None,
     ):
         ThreadingTCPServer.__init__(
-            self, (host, port), handler, bind_and_activate=bind_and_activate
+            self, (host, int(port)), handler, bind_and_activate=bind_and_activate
         )
         self.abort = abort
         self.timeout = timeout
         self.logname = logname
 
     def serve(self):
         abort = 0
```

### Comparing `socket-log-receiver-20.4.1a0/src/socket_log_receiver.egg-info/PKG-INFO` & `socket-log-receiver-23.7.0a0/src/socket_log_receiver.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,81 +1,85 @@
 Metadata-Version: 2.1
 Name: socket-log-receiver
-Version: 20.4.1a0
+Version: 23.7.0a0
 Summary: A light-weight socket log receiver
-Home-page: https://github.com/okomestudio/socket-log-receiver
-Author: Taro Sato
-Author-email: okomestudio@gmail.com
-License: MIT
-Description: [![pyversion Status](https://img.shields.io/pypi/pyversions/socket-log-receiver.svg)](https://img.shields.io/pypi/pyversions/socket-log-receiver.svg)
-        [![CircleCI](https://circleci.com/gh/okomestudio/socket-log-receiver.svg?style=shield)](https://circleci.com/gh/okomestudio/socket-log-receiver)
-        [![Coverage Status](https://coveralls.io/repos/github/okomestudio/socket-log-receiver/badge.svg?branch=development)](https://coveralls.io/github/okomestudio/socket-log-receiver?branch=development&kill_cache=1)
-        [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
-        
-        
-        # Socket Log Receiver
-        
-        `socket_log_receiver` is a light-weight socket log receiver. It runs
-        as a server and aggregates messages from multi-process application via
-        socket and logs to a single file. Python's `logging` package does not
-        support logging to a single file from multiple processes. By pointing
-        `SocketHandler` to `socket_log_receiver`, the multi-process
-        application can log to a single file.
-        
-        
-        ## Installation
-        
-        ``` bash
-        $ pip install socket-log-receiver
-        ```
-        
-        
-        ## Basic Usage
-        
-        The receiver service should be run as a service.
-        
-        ``` bash
-        $ python -m socket_log_receiver  # as a module
-        $ log_receiver                   # as a command-line program
-        ```
-        
-        In the application, use `SocketHandler` to send logs to the receiver
-        service.
-        
-        ``` python
-        from logging.handlers import SocketHandler
-        
-        handler = SocketHandler('localhost', 9020)  # handler to send logs to localhost:9020
-        logging.root.addHandler(handler)            # add the socket handler to the root logger
-        ```
-        
-        This way, the root logger sends logging messages to the receiver service.
-        
-        
-        ## Development
-        
-        ```bash
-        $ pip install -e .[dev]
-        $ pre-commit install
-        ```
-        
-        
-        ### Running Tests
-        
-        ``` bash
-        $ python setup.py tests
-        ```
-        
-Platform: Linux
+Author-email: Taro Sato <okomestudio@gmail.com>
+Project-URL: Homepage, https://github.com/okomestudio/socket-log-receiver
+Project-URL: Buck Tracker, https://github.com/okomestudio/socket-log-receiver/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Utilities
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: test
+License-File: LICENSE.txt
+
+[![License](https://img.shields.io/pypi/l/socket-log-receiver.svg)](https://pypi.org/project/socket-log-receiver/)
+[![PyPI Version](https://badge.fury.io/py/socket-log-receiver.svg)](https://pypi.org/project/socket-log-receiver/)
+[![Package Status](https://img.shields.io/pypi/status/socket-log-receiver.svg)](https://pypi.org/project/resconfig/)
+[![pyversion Status](https://img.shields.io/pypi/pyversions/socket-log-receiver.svg)](https://img.shields.io/pypi/pyversions/socket-log-receiver.svg)
+[![CircleCI](https://circleci.com/gh/okomestudio/socket-log-receiver.svg?style=shield)](https://circleci.com/gh/okomestudio/socket-log-receiver)
+[![Coverage Status](https://coveralls.io/repos/github/okomestudio/socket-log-receiver/badge.svg?branch=development)](https://coveralls.io/github/okomestudio/socket-log-receiver?branch=development&kill_cache=1)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+
+
+# Socket Log Receiver
+
+`socket_log_receiver` is a light-weight socket log receiver. It runs
+as a server and aggregates messages from multi-process application via
+socket and logs to a single file. Python's `logging` package does not
+support logging to a single file from multiple processes. By pointing
+`SocketHandler` to `socket_log_receiver`, the multi-process
+application can log to a single file.
+
+
+## Installation
+
+``` bash
+$ pip install socket-log-receiver
+```
+
+
+## Basic Usage
+
+The receiver service should be run as a service.
+
+``` bash
+$ python -m socket_log_receiver  # as a module
+$ log_receiver                   # as a command-line program
+```
+
+In the application, use `SocketHandler` to send logs to the receiver
+service.
+
+``` python
+from logging.handlers import SocketHandler
+
+handler = SocketHandler('localhost', 9020)  # handler to send logs to localhost:9020
+logging.root.addHandler(handler)            # add the socket handler to the root logger
+```
+
+This way, the root logger sends logging messages to the receiver service.
+
+
+## Development
+
+```bash
+$ pip install -e .[dev]
+$ pre-commit install
+```
+
+
+### Running Tests
+
+``` bash
+$ python setup.py tests
+```
```

