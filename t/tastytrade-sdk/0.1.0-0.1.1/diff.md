# Comparing `tmp/tastytrade_sdk-0.1.0.tar.gz` & `tmp/tastytrade_sdk-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tastytrade_sdk-0.1.0.tar", max compression
+gzip compressed data, was "tastytrade_sdk-0.1.1.tar", max compression
```

## Comparing `tastytrade_sdk-0.1.0.tar` & `tastytrade_sdk-0.1.1.tar`

### file list

```diff
@@ -1,13 +1,14 @@
--rw-r--r--   0        0        0     1056 2023-07-02 04:27:28.565817 tastytrade_sdk-0.1.0/LICENSE
--rw-r--r--   0        0        0      492 2023-07-02 04:27:28.565817 tastytrade_sdk-0.1.0/README.md
--rw-r--r--   0        0        0      784 2023-07-02 04:27:28.565817 tastytrade_sdk-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      516 2023-07-02 04:27:28.565817 tastytrade_sdk-0.1.0/src/tastytrade_sdk/__init__.py
--rw-r--r--   0        0        0     4166 2023-07-02 04:27:28.565817 tastytrade_sdk-0.1.0/src/tastytrade_sdk/api.py
--rw-r--r--   0        0        0      421 2023-07-02 04:27:28.565817 tastytrade_sdk-0.1.0/src/tastytrade_sdk/exceptions.py
--rw-r--r--   0        0        0        0 2023-07-02 04:27:28.565817 tastytrade_sdk-0.1.0/src/tastytrade_sdk/market_data/__init__.py
--rw-r--r--   0        0        0     1548 2023-07-02 04:27:28.565817 tastytrade_sdk-0.1.0/src/tastytrade_sdk/market_data/market_data.py
--rw-r--r--   0        0        0     2646 2023-07-02 04:27:28.565817 tastytrade_sdk-0.1.0/src/tastytrade_sdk/market_data/models.py
--rw-r--r--   0        0        0     1889 2023-07-02 04:27:28.565817 tastytrade_sdk-0.1.0/src/tastytrade_sdk/market_data/streamer_symbol_translation.py
--rw-r--r--   0        0        0     6137 2023-07-02 04:27:28.565817 tastytrade_sdk-0.1.0/src/tastytrade_sdk/market_data/subscription.py
--rw-r--r--   0        0        0      914 2023-07-02 04:27:28.565817 tastytrade_sdk-0.1.0/src/tastytrade_sdk/tastytrade.py
--rw-r--r--   0        0        0     1293 1970-01-01 00:00:00.000000 tastytrade_sdk-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1053 2023-07-08 07:15:03.319407 tastytrade_sdk-0.1.1/LICENSE
+-rw-r--r--   0        0        0     1652 2023-07-08 07:15:03.319407 tastytrade_sdk-0.1.1/docs/users/README.md
+-rw-r--r--   0        0        0      816 2023-07-08 07:15:03.319407 tastytrade_sdk-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      516 2023-07-08 07:15:03.319407 tastytrade_sdk-0.1.1/src/tastytrade_sdk/__init__.py
+-rw-r--r--   0        0        0     4185 2023-07-08 07:15:03.319407 tastytrade_sdk-0.1.1/src/tastytrade_sdk/api.py
+-rw-r--r--   0        0        0      136 2023-07-08 07:15:03.319407 tastytrade_sdk-0.1.1/src/tastytrade_sdk/config.py
+-rw-r--r--   0        0        0      421 2023-07-08 07:15:03.319407 tastytrade_sdk-0.1.1/src/tastytrade_sdk/exceptions.py
+-rw-r--r--   0        0        0        0 2023-07-08 07:15:03.323407 tastytrade_sdk-0.1.1/src/tastytrade_sdk/market_data/__init__.py
+-rw-r--r--   0        0        0     1548 2023-07-08 07:15:03.323407 tastytrade_sdk-0.1.1/src/tastytrade_sdk/market_data/market_data.py
+-rw-r--r--   0        0        0     2646 2023-07-08 07:15:03.323407 tastytrade_sdk-0.1.1/src/tastytrade_sdk/market_data/models.py
+-rw-r--r--   0        0        0     1889 2023-07-08 07:15:03.323407 tastytrade_sdk-0.1.1/src/tastytrade_sdk/market_data/streamer_symbol_translation.py
+-rw-r--r--   0        0        0     6137 2023-07-08 07:15:03.323407 tastytrade_sdk-0.1.1/src/tastytrade_sdk/market_data/subscription.py
+-rw-r--r--   0        0        0     1266 2023-07-08 07:15:03.323407 tastytrade_sdk-0.1.1/src/tastytrade_sdk/tastytrade.py
+-rw-r--r--   0        0        0     2453 1970-01-01 00:00:00.000000 tastytrade_sdk-0.1.1/PKG-INFO
```

### Comparing `tastytrade_sdk-0.1.0/LICENSE` & `tastytrade_sdk-0.1.1/LICENSE`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright (c) 2023 Aaron Mamparo
+Copyright (c) 2023 tastytrade
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `tastytrade_sdk-0.1.0/pyproject.toml` & `tastytrade_sdk-0.1.1/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 [tool.poetry]
 name = "tastytrade-sdk"
-version = "0.1.0"
+version = "0.1.1"
 description = "A python wrapper around the tastytrade open API"
-authors = ["Aaron Mamparo <aaronmamparo@gmail.com>"]
+authors = [
+    "Aaron Mamparo <aaronmamparo@gmail.com>"
+]
 license = "MIT"
-readme = "README.md"
+readme = "docs/users/README.md"
 packages = [
     { include = "tastytrade_sdk", from = "src" }
 ]
 
 [project.urls]
-documentation = "https://tastytrade-sdk.readthedocs.io"
-repository = "https://github.com/amamparo/tastytrade-sdk-python"
+documentation = "https://tastytrade.github.io/tastytrade-sdk-python"
+repository = "https://github.com/tastytrade/tastytrade-sdk-python"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 injector = "^0.20.1"
 requests = "2.29.0"
 websockets = "^11.0.3"
 bidict = "^0.22.1"
```

### Comparing `tastytrade_sdk-0.1.0/src/tastytrade_sdk/__init__.py` & `tastytrade_sdk-0.1.1/src/tastytrade_sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `tastytrade_sdk-0.1.0/src/tastytrade_sdk/api.py` & `tastytrade_sdk-0.1.1/src/tastytrade_sdk/api.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 import logging
 from typing import Optional, Tuple, List, Any, Union, Dict
 
-import importlib.metadata
 from injector import singleton, inject
 from requests import Session, JSONDecodeError
 
+from tastytrade_sdk.config import Config
 from tastytrade_sdk.exceptions import TastytradeSdkException
 
 QueryParams = Union[Dict[str, Any], List[Tuple[str, Any]]]
-"""foobar"""
 
 
 @singleton
 class RequestsSession:
-    __base_url = 'https://api.tastyworks.com'
     __session = Session()
-    __user_agent = f'tastytrade-sdk-python v{importlib.metadata.version("tastytrade-sdk")}'
+    __user_agent = 'tastytrade-sdk-python'
+
+    @inject
+    def __init__(self, config: Config):
+        self.__base_url = f'https://{config.api_base_url}'
 
     def login(self, login: str, password: str) -> None:
         self.__session.headers['Authorization'] = self.request(
             'POST',
             '/sessions',
             data={'login': login, 'password': password}
         )['data']['session-token']
```

### Comparing `tastytrade_sdk-0.1.0/src/tastytrade_sdk/market_data/market_data.py` & `tastytrade_sdk-0.1.1/src/tastytrade_sdk/market_data/market_data.py`

 * *Files identical despite different names*

### Comparing `tastytrade_sdk-0.1.0/src/tastytrade_sdk/market_data/models.py` & `tastytrade_sdk-0.1.1/src/tastytrade_sdk/market_data/models.py`

 * *Files identical despite different names*

### Comparing `tastytrade_sdk-0.1.0/src/tastytrade_sdk/market_data/streamer_symbol_translation.py` & `tastytrade_sdk-0.1.1/src/tastytrade_sdk/market_data/streamer_symbol_translation.py`

 * *Files identical despite different names*

### Comparing `tastytrade_sdk-0.1.0/src/tastytrade_sdk/market_data/subscription.py` & `tastytrade_sdk-0.1.1/src/tastytrade_sdk/market_data/subscription.py`

 * *Files identical despite different names*

