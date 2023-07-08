# Comparing `tmp/aiohttp-rpc-1.2.0.tar.gz` & `tmp/aiohttp-rpc-1.3.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiohttp-rpc-1.2.0.tar", last modified: Thu Mar 23 19:14:52 2023, max compression
+gzip compressed data, was "aiohttp-rpc-1.3.0b1.tar", last modified: Sat Jul  8 06:30:08 2023, max compression
```

## Comparing `aiohttp-rpc-1.2.0.tar` & `aiohttp-rpc-1.3.0b1.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-03-23 19:14:52.244920 aiohttp-rpc-1.2.0/
--rwxrwxrwx   0 michael   (1000) michael   (1000)     1071 2022-06-22 04:31:16.000000 aiohttp-rpc-1.2.0/LICENSE.txt
--rw-rw-r--   0 michael   (1000) michael   (1000)    14493 2023-03-23 19:14:52.244920 aiohttp-rpc-1.2.0/PKG-INFO
--rwxrwxrwx   0 michael   (1000) michael   (1000)    13133 2023-03-23 18:30:13.000000 aiohttp-rpc-1.2.0/README.md
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-03-23 19:14:52.240920 aiohttp-rpc-1.2.0/aiohttp_rpc/
--rwxrwxrwx   0 michael   (1000) michael   (1000)      376 2022-07-08 14:39:35.000000 aiohttp-rpc-1.2.0/aiohttp_rpc/__init__.py
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-03-23 19:14:52.240920 aiohttp-rpc-1.2.0/aiohttp_rpc/client/
--rwxrwxrwx   0 michael   (1000) michael   (1000)      122 2022-06-22 04:31:15.000000 aiohttp-rpc-1.2.0/aiohttp_rpc/client/__init__.py
--rwxrwxrwx   0 michael   (1000) michael   (1000)     6158 2022-06-22 04:31:15.000000 aiohttp-rpc-1.2.0/aiohttp_rpc/client/base.py
--rwxrwxrwx   0 michael   (1000) michael   (1000)     1832 2022-06-22 04:31:15.000000 aiohttp-rpc-1.2.0/aiohttp_rpc/client/http.py
--rwxrwxrwx   0 michael   (1000) michael   (1000)        0 2022-06-22 04:31:15.000000 aiohttp-rpc-1.2.0/aiohttp_rpc/client/py.typed
--rwxrwxrwx   0 michael   (1000) michael   (1000)     8797 2022-07-08 15:45:16.000000 aiohttp-rpc-1.2.0/aiohttp_rpc/client/websocket.py
--rwxrwxrwx   0 michael   (1000) michael   (1000)      157 2022-06-22 04:31:15.000000 aiohttp-rpc-1.2.0/aiohttp_rpc/constants.py
--rwxrwxrwx   0 michael   (1000) michael   (1000)      585 2022-06-22 04:31:15.000000 aiohttp-rpc-1.2.0/aiohttp_rpc/decorators.py
--rwxrwxrwx   0 michael   (1000) michael   (1000)     2497 2022-06-22 04:31:15.000000 aiohttp-rpc-1.2.0/aiohttp_rpc/errors.py
--rwxrwxrwx   0 michael   (1000) michael   (1000)     2461 2022-06-22 04:31:15.000000 aiohttp-rpc-1.2.0/aiohttp_rpc/middlewares.py
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-03-23 19:14:52.240920 aiohttp-rpc-1.2.0/aiohttp_rpc/protocol/
--rwxrwxrwx   0 michael   (1000) michael   (1000)      126 2022-06-22 04:31:15.000000 aiohttp-rpc-1.2.0/aiohttp_rpc/protocol/__init__.py
--rwxrwxrwx   0 michael   (1000) michael   (1000)     5178 2022-06-22 04:31:15.000000 aiohttp-rpc-1.2.0/aiohttp_rpc/protocol/method.py
--rwxrwxrwx   0 michael   (1000) michael   (1000)        0 2022-06-22 04:31:15.000000 aiohttp-rpc-1.2.0/aiohttp_rpc/protocol/py.typed
--rwxrwxrwx   0 michael   (1000) michael   (1000)     3640 2022-06-22 04:31:15.000000 aiohttp-rpc-1.2.0/aiohttp_rpc/protocol/request.py
--rwxrwxrwx   0 michael   (1000) michael   (1000)     3940 2022-06-22 04:31:15.000000 aiohttp-rpc-1.2.0/aiohttp_rpc/protocol/response.py
--rwxrwxrwx   0 michael   (1000) michael   (1000)        0 2022-06-22 04:31:15.000000 aiohttp-rpc-1.2.0/aiohttp_rpc/py.typed
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-03-23 19:14:52.244920 aiohttp-rpc-1.2.0/aiohttp_rpc/server/
--rwxrwxrwx   0 michael   (1000) michael   (1000)      122 2022-06-22 04:31:15.000000 aiohttp-rpc-1.2.0/aiohttp_rpc/server/__init__.py
--rwxrwxrwx   0 michael   (1000) michael   (1000)     6540 2023-03-23 19:05:25.000000 aiohttp-rpc-1.2.0/aiohttp_rpc/server/base.py
--rwxrwxrwx   0 michael   (1000) michael   (1000)      995 2022-06-22 04:31:15.000000 aiohttp-rpc-1.2.0/aiohttp_rpc/server/http.py
--rwxrwxrwx   0 michael   (1000) michael   (1000)        0 2022-06-22 04:31:15.000000 aiohttp-rpc-1.2.0/aiohttp_rpc/server/py.typed
--rwxrwxrwx   0 michael   (1000) michael   (1000)     3408 2022-07-08 15:43:12.000000 aiohttp-rpc-1.2.0/aiohttp_rpc/server/websocket.py
--rwxrwxrwx   0 michael   (1000) michael   (1000)      946 2023-03-23 19:03:20.000000 aiohttp-rpc-1.2.0/aiohttp_rpc/typedefs.py
--rwxrwxrwx   0 michael   (1000) michael   (1000)     3245 2022-06-22 04:31:15.000000 aiohttp-rpc-1.2.0/aiohttp_rpc/utils.py
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-03-23 19:14:52.240920 aiohttp-rpc-1.2.0/aiohttp_rpc.egg-info/
--rw-rw-r--   0 michael   (1000) michael   (1000)    14493 2023-03-23 19:14:51.000000 aiohttp-rpc-1.2.0/aiohttp_rpc.egg-info/PKG-INFO
--rw-rw-r--   0 michael   (1000) michael   (1000)      858 2023-03-23 19:14:52.000000 aiohttp-rpc-1.2.0/aiohttp_rpc.egg-info/SOURCES.txt
--rw-rw-r--   0 michael   (1000) michael   (1000)        1 2023-03-23 19:14:51.000000 aiohttp-rpc-1.2.0/aiohttp_rpc.egg-info/dependency_links.txt
--rw-rw-r--   0 michael   (1000) michael   (1000)       14 2023-03-23 19:14:52.000000 aiohttp-rpc-1.2.0/aiohttp_rpc.egg-info/requires.txt
--rw-rw-r--   0 michael   (1000) michael   (1000)       12 2023-03-23 19:14:52.000000 aiohttp-rpc-1.2.0/aiohttp_rpc.egg-info/top_level.txt
--rwxrwxrwx   0 michael   (1000) michael   (1000)      436 2023-03-23 17:59:43.000000 aiohttp-rpc-1.2.0/pyproject.toml
--rw-rw-r--   0 michael   (1000) michael   (1000)       38 2023-03-23 19:14:52.244920 aiohttp-rpc-1.2.0/setup.cfg
--rwxrwxrwx   0 michael   (1000) michael   (1000)     2285 2023-03-23 18:30:13.000000 aiohttp-rpc-1.2.0/setup.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-07-08 06:30:08.921718 aiohttp-rpc-1.3.0b1/
+-rwxrwxrwx   0 michael   (1000) michael   (1000)     1071 2022-06-22 04:31:16.000000 aiohttp-rpc-1.3.0b1/LICENSE.txt
+-rw-rw-r--   0 michael   (1000) michael   (1000)    14495 2023-07-08 06:30:08.921718 aiohttp-rpc-1.3.0b1/PKG-INFO
+-rw-rw-r--   0 michael   (1000) michael   (1000)    13133 2023-07-08 06:26:15.000000 aiohttp-rpc-1.3.0b1/README.md
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-07-08 06:30:08.917717 aiohttp-rpc-1.3.0b1/aiohttp_rpc/
+-rwxrwxrwx   0 michael   (1000) michael   (1000)      376 2022-07-08 14:39:35.000000 aiohttp-rpc-1.3.0b1/aiohttp_rpc/__init__.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-07-08 06:30:08.917717 aiohttp-rpc-1.3.0b1/aiohttp_rpc/client/
+-rwxrwxrwx   0 michael   (1000) michael   (1000)      122 2022-06-22 04:31:15.000000 aiohttp-rpc-1.3.0b1/aiohttp_rpc/client/__init__.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     6158 2023-07-08 06:26:15.000000 aiohttp-rpc-1.3.0b1/aiohttp_rpc/client/base.py
+-rwxrwxrwx   0 michael   (1000) michael   (1000)     1832 2022-06-22 04:31:15.000000 aiohttp-rpc-1.3.0b1/aiohttp_rpc/client/http.py
+-rwxrwxrwx   0 michael   (1000) michael   (1000)        0 2022-06-22 04:31:15.000000 aiohttp-rpc-1.3.0b1/aiohttp_rpc/client/py.typed
+-rw-rw-r--   0 michael   (1000) michael   (1000)     8797 2023-07-08 06:26:15.000000 aiohttp-rpc-1.3.0b1/aiohttp_rpc/client/websocket.py
+-rwxrwxrwx   0 michael   (1000) michael   (1000)      157 2022-06-22 04:31:15.000000 aiohttp-rpc-1.3.0b1/aiohttp_rpc/constants.py
+-rwxrwxrwx   0 michael   (1000) michael   (1000)      585 2022-06-22 04:31:15.000000 aiohttp-rpc-1.3.0b1/aiohttp_rpc/decorators.py
+-rwxrwxrwx   0 michael   (1000) michael   (1000)     2497 2022-06-22 04:31:15.000000 aiohttp-rpc-1.3.0b1/aiohttp_rpc/errors.py
+-rwxrwxrwx   0 michael   (1000) michael   (1000)     2461 2022-06-22 04:31:15.000000 aiohttp-rpc-1.3.0b1/aiohttp_rpc/middlewares.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-07-08 06:30:08.921718 aiohttp-rpc-1.3.0b1/aiohttp_rpc/protocol/
+-rwxrwxrwx   0 michael   (1000) michael   (1000)      126 2022-06-22 04:31:15.000000 aiohttp-rpc-1.3.0b1/aiohttp_rpc/protocol/__init__.py
+-rwxrwxrwx   0 michael   (1000) michael   (1000)     5178 2022-06-22 04:31:15.000000 aiohttp-rpc-1.3.0b1/aiohttp_rpc/protocol/method.py
+-rwxrwxrwx   0 michael   (1000) michael   (1000)        0 2022-06-22 04:31:15.000000 aiohttp-rpc-1.3.0b1/aiohttp_rpc/protocol/py.typed
+-rwxrwxrwx   0 michael   (1000) michael   (1000)     3640 2022-06-22 04:31:15.000000 aiohttp-rpc-1.3.0b1/aiohttp_rpc/protocol/request.py
+-rwxrwxrwx   0 michael   (1000) michael   (1000)     3940 2022-06-22 04:31:15.000000 aiohttp-rpc-1.3.0b1/aiohttp_rpc/protocol/response.py
+-rwxrwxrwx   0 michael   (1000) michael   (1000)        0 2022-06-22 04:31:15.000000 aiohttp-rpc-1.3.0b1/aiohttp_rpc/py.typed
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-07-08 06:30:08.921718 aiohttp-rpc-1.3.0b1/aiohttp_rpc/server/
+-rwxrwxrwx   0 michael   (1000) michael   (1000)      122 2022-06-22 04:31:15.000000 aiohttp-rpc-1.3.0b1/aiohttp_rpc/server/__init__.py
+-rwxrwxrwx   0 michael   (1000) michael   (1000)     6540 2023-03-23 19:05:25.000000 aiohttp-rpc-1.3.0b1/aiohttp_rpc/server/base.py
+-rwxrwxrwx   0 michael   (1000) michael   (1000)      995 2022-06-22 04:31:15.000000 aiohttp-rpc-1.3.0b1/aiohttp_rpc/server/http.py
+-rwxrwxrwx   0 michael   (1000) michael   (1000)        0 2022-06-22 04:31:15.000000 aiohttp-rpc-1.3.0b1/aiohttp_rpc/server/py.typed
+-rwxrwxrwx   0 michael   (1000) michael   (1000)     3408 2022-07-08 15:43:12.000000 aiohttp-rpc-1.3.0b1/aiohttp_rpc/server/websocket.py
+-rwxrwxrwx   0 michael   (1000) michael   (1000)      946 2023-03-23 19:03:20.000000 aiohttp-rpc-1.3.0b1/aiohttp_rpc/typedefs.py
+-rwxrwxrwx   0 michael   (1000) michael   (1000)     3245 2022-06-22 04:31:15.000000 aiohttp-rpc-1.3.0b1/aiohttp_rpc/utils.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-07-08 06:30:08.917717 aiohttp-rpc-1.3.0b1/aiohttp_rpc.egg-info/
+-rw-rw-r--   0 michael   (1000) michael   (1000)    14495 2023-07-08 06:30:08.000000 aiohttp-rpc-1.3.0b1/aiohttp_rpc.egg-info/PKG-INFO
+-rw-rw-r--   0 michael   (1000) michael   (1000)      858 2023-07-08 06:30:08.000000 aiohttp-rpc-1.3.0b1/aiohttp_rpc.egg-info/SOURCES.txt
+-rw-rw-r--   0 michael   (1000) michael   (1000)        1 2023-07-08 06:30:08.000000 aiohttp-rpc-1.3.0b1/aiohttp_rpc.egg-info/dependency_links.txt
+-rw-rw-r--   0 michael   (1000) michael   (1000)       14 2023-07-08 06:30:08.000000 aiohttp-rpc-1.3.0b1/aiohttp_rpc.egg-info/requires.txt
+-rw-rw-r--   0 michael   (1000) michael   (1000)       12 2023-07-08 06:30:08.000000 aiohttp-rpc-1.3.0b1/aiohttp_rpc.egg-info/top_level.txt
+-rw-rw-r--   0 michael   (1000) michael   (1000)      438 2023-07-08 06:28:39.000000 aiohttp-rpc-1.3.0b1/pyproject.toml
+-rw-rw-r--   0 michael   (1000) michael   (1000)       38 2023-07-08 06:30:08.921718 aiohttp-rpc-1.3.0b1/setup.cfg
+-rwxrwxrwx   0 michael   (1000) michael   (1000)     2287 2023-07-08 06:28:39.000000 aiohttp-rpc-1.3.0b1/setup.py
```

### Comparing `aiohttp-rpc-1.2.0/LICENSE.txt` & `aiohttp-rpc-1.3.0b1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `aiohttp-rpc-1.2.0/PKG-INFO` & `aiohttp-rpc-1.3.0b1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiohttp-rpc
-Version: 1.2.0
+Version: 1.3.0b1
 Summary: A simple JSON-RPC for aiohttp
 Home-page: https://github.com/expert-m/aiohttp-rpc/
 Author: Michael Sulyak
 Author-email: michael@sulyak.info
 License: MIT license
 Project-URL: GitHub: issues, https://github.com/expert-m/aiohttp-rpc/issues
 Project-URL: GitHub: repo, https://github.com/expert-m/aiohttp-rpc
```

### Comparing `aiohttp-rpc-1.2.0/README.md` & `aiohttp-rpc-1.3.0b1/README.md`

 * *Files identical despite different names*

### Comparing `aiohttp-rpc-1.2.0/aiohttp_rpc/client/base.py` & `aiohttp-rpc-1.3.0b1/aiohttp_rpc/client/base.py`

 * *Files identical despite different names*

### Comparing `aiohttp-rpc-1.2.0/aiohttp_rpc/client/http.py` & `aiohttp-rpc-1.3.0b1/aiohttp_rpc/client/http.py`

 * *Files identical despite different names*

### Comparing `aiohttp-rpc-1.2.0/aiohttp_rpc/client/websocket.py` & `aiohttp-rpc-1.3.0b1/aiohttp_rpc/client/websocket.py`

 * *Files identical despite different names*

### Comparing `aiohttp-rpc-1.2.0/aiohttp_rpc/decorators.py` & `aiohttp-rpc-1.3.0b1/aiohttp_rpc/decorators.py`

 * *Files identical despite different names*

### Comparing `aiohttp-rpc-1.2.0/aiohttp_rpc/errors.py` & `aiohttp-rpc-1.3.0b1/aiohttp_rpc/errors.py`

 * *Files identical despite different names*

### Comparing `aiohttp-rpc-1.2.0/aiohttp_rpc/middlewares.py` & `aiohttp-rpc-1.3.0b1/aiohttp_rpc/middlewares.py`

 * *Files identical despite different names*

### Comparing `aiohttp-rpc-1.2.0/aiohttp_rpc/protocol/method.py` & `aiohttp-rpc-1.3.0b1/aiohttp_rpc/protocol/method.py`

 * *Files identical despite different names*

### Comparing `aiohttp-rpc-1.2.0/aiohttp_rpc/protocol/request.py` & `aiohttp-rpc-1.3.0b1/aiohttp_rpc/protocol/request.py`

 * *Files identical despite different names*

### Comparing `aiohttp-rpc-1.2.0/aiohttp_rpc/protocol/response.py` & `aiohttp-rpc-1.3.0b1/aiohttp_rpc/protocol/response.py`

 * *Files identical despite different names*

### Comparing `aiohttp-rpc-1.2.0/aiohttp_rpc/server/base.py` & `aiohttp-rpc-1.3.0b1/aiohttp_rpc/server/base.py`

 * *Files identical despite different names*

### Comparing `aiohttp-rpc-1.2.0/aiohttp_rpc/server/http.py` & `aiohttp-rpc-1.3.0b1/aiohttp_rpc/server/http.py`

 * *Files identical despite different names*

### Comparing `aiohttp-rpc-1.2.0/aiohttp_rpc/server/websocket.py` & `aiohttp-rpc-1.3.0b1/aiohttp_rpc/server/websocket.py`

 * *Files identical despite different names*

### Comparing `aiohttp-rpc-1.2.0/aiohttp_rpc/typedefs.py` & `aiohttp-rpc-1.3.0b1/aiohttp_rpc/typedefs.py`

 * *Files identical despite different names*

### Comparing `aiohttp-rpc-1.2.0/aiohttp_rpc/utils.py` & `aiohttp-rpc-1.3.0b1/aiohttp_rpc/utils.py`

 * *Files identical despite different names*

### Comparing `aiohttp-rpc-1.2.0/aiohttp_rpc.egg-info/PKG-INFO` & `aiohttp-rpc-1.3.0b1/aiohttp_rpc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiohttp-rpc
-Version: 1.2.0
+Version: 1.3.0b1
 Summary: A simple JSON-RPC for aiohttp
 Home-page: https://github.com/expert-m/aiohttp-rpc/
 Author: Michael Sulyak
 Author-email: michael@sulyak.info
 License: MIT license
 Project-URL: GitHub: issues, https://github.com/expert-m/aiohttp-rpc/issues
 Project-URL: GitHub: repo, https://github.com/expert-m/aiohttp-rpc
```

### Comparing `aiohttp-rpc-1.2.0/aiohttp_rpc.egg-info/SOURCES.txt` & `aiohttp-rpc-1.3.0b1/aiohttp_rpc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aiohttp-rpc-1.2.0/setup.py` & `aiohttp-rpc-1.3.0b1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,15 +9,15 @@
         long_description = file.read()
 
     packages = find_packages(exclude=['tests'])
     package_data = {package: ['py.typed'] for package in packages}
 
     setup(
         name='aiohttp-rpc',
-        version='1.2.0',
+        version='1.3.0b1',
         author='Michael Sulyak',
         url='https://github.com/expert-m/aiohttp-rpc/',
         author_email='michael@sulyak.info',
         keywords=[
             'aiohttp', 'asyncio', 'json-rpc', 'rpc',
         ],
         install_requires=[
```

