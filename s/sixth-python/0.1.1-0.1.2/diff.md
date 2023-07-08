# Comparing `tmp/sixth-python-0.1.1.tar.gz` & `tmp/sixth-python-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sixth-python-0.1.1.tar", last modified: Mon Jul  3 03:08:14 2023, max compression
+gzip compressed data, was "dist/sixth-python-0.1.2.tar", last modified: Sat Jul  8 18:57:03 2023, max compression
```

## Comparing `sixth-python-0.1.1.tar` & `sixth-python-0.1.2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-07-03 03:08:14.000000 sixth-python-0.1.1/
--rw-r--r--   0 mac        (501) staff       (20)     3114 2023-07-03 03:08:14.000000 sixth-python-0.1.1/PKG-INFO
--rw-r--r--   0 mac        (501) staff       (20)     1899 2023-06-23 11:48:40.000000 sixth-python-0.1.1/README.md
--rw-r--r--   0 mac        (501) staff       (20)       38 2023-07-03 03:08:14.000000 sixth-python-0.1.1/setup.cfg
--rw-r--r--   0 mac        (501) staff       (20)     3773 2023-07-03 03:07:48.000000 sixth-python-0.1.1/setup.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-07-03 03:08:14.000000 sixth-python-0.1.1/sixth/
--rw-r--r--   0 mac        (501) staff       (20)       27 2023-06-23 22:29:11.000000 sixth-python-0.1.1/sixth/__init__.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-07-03 03:08:14.000000 sixth-python-0.1.1/sixth/middlewares/
--rw-r--r--   0 mac        (501) staff       (20)        0 2023-06-10 23:12:54.000000 sixth-python-0.1.1/sixth/middlewares/__init__.py
--rw-r--r--   0 mac        (501) staff       (20)     3703 2023-07-03 02:16:20.000000 sixth-python-0.1.1/sixth/middlewares/encryption_middleware.py
--rw-r--r--   0 mac        (501) staff       (20)     5121 2023-06-10 17:10:19.000000 sixth-python-0.1.1/sixth/middlewares/six_base_http_middleware.py
--rw-r--r--   0 mac        (501) staff       (20)     3924 2023-07-03 02:16:20.000000 sixth-python-0.1.1/sixth/middlewares/six_independent_rate_limiter.py
--rw-r--r--   0 mac        (501) staff       (20)     5573 2023-07-03 02:53:36.000000 sixth-python-0.1.1/sixth/middlewares/six_rate_limiter_middleware.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-07-03 03:08:14.000000 sixth-python-0.1.1/sixth/pen_test/
--rw-r--r--   0 mac        (501) staff       (20)        0 2023-06-12 15:04:45.000000 sixth-python-0.1.1/sixth/pen_test/__init__.py
--rw-r--r--   0 mac        (501) staff       (20)      165 2023-06-14 20:44:10.000000 sixth-python-0.1.1/sixth/pen_test/auto_pen_test.py
--rw-r--r--   0 mac        (501) staff       (20)      916 2023-07-03 00:19:36.000000 sixth-python-0.1.1/sixth/schemas.py
--rw-r--r--   0 mac        (501) staff       (20)     4190 2023-07-03 02:16:20.000000 sixth-python-0.1.1/sixth/sdk.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-07-03 03:08:14.000000 sixth-python-0.1.1/sixth/utils/
--rw-r--r--   0 mac        (501) staff       (20)        0 2023-06-10 23:13:17.000000 sixth-python-0.1.1/sixth/utils/__init__.py
--rw-r--r--   0 mac        (501) staff       (20)     4254 2023-06-12 02:56:13.000000 sixth-python-0.1.1/sixth/utils/encryption_utils.py
--rw-rw-r--   0 mac        (501) staff       (20)     1707 2023-06-09 19:33:11.000000 sixth-python-0.1.1/sixth/utils/time_utils.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-07-03 03:08:14.000000 sixth-python-0.1.1/sixth_python.egg-info/
--rw-r--r--   0 mac        (501) staff       (20)     3114 2023-07-03 03:08:14.000000 sixth-python-0.1.1/sixth_python.egg-info/PKG-INFO
--rw-r--r--   0 mac        (501) staff       (20)      604 2023-07-03 03:08:14.000000 sixth-python-0.1.1/sixth_python.egg-info/SOURCES.txt
--rw-r--r--   0 mac        (501) staff       (20)        1 2023-07-03 03:08:14.000000 sixth-python-0.1.1/sixth_python.egg-info/dependency_links.txt
--rw-r--r--   0 mac        (501) staff       (20)      610 2023-07-03 03:08:14.000000 sixth-python-0.1.1/sixth_python.egg-info/requires.txt
--rw-r--r--   0 mac        (501) staff       (20)        6 2023-07-03 03:08:14.000000 sixth-python-0.1.1/sixth_python.egg-info/top_level.txt
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-07-08 18:57:03.000000 sixth-python-0.1.2/
+-rw-r--r--   0 mac        (501) staff       (20)     3101 2023-07-08 18:57:03.000000 sixth-python-0.1.2/PKG-INFO
+-rw-r--r--   0 mac        (501) staff       (20)     1899 2023-06-23 11:48:40.000000 sixth-python-0.1.2/README.md
+-rw-r--r--   0 mac        (501) staff       (20)       38 2023-07-08 18:57:03.000000 sixth-python-0.1.2/setup.cfg
+-rw-r--r--   0 mac        (501) staff       (20)     3760 2023-07-08 18:53:36.000000 sixth-python-0.1.2/setup.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-07-08 18:57:03.000000 sixth-python-0.1.2/sixth/
+-rw-r--r--   0 mac        (501) staff       (20)       27 2023-06-23 22:29:11.000000 sixth-python-0.1.2/sixth/__init__.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-07-08 18:57:03.000000 sixth-python-0.1.2/sixth/middlewares/
+-rw-r--r--   0 mac        (501) staff       (20)        0 2023-06-10 23:12:54.000000 sixth-python-0.1.2/sixth/middlewares/__init__.py
+-rw-r--r--   0 mac        (501) staff       (20)     3703 2023-07-03 02:16:20.000000 sixth-python-0.1.2/sixth/middlewares/encryption_middleware.py
+-rw-r--r--   0 mac        (501) staff       (20)     5121 2023-06-10 17:10:19.000000 sixth-python-0.1.2/sixth/middlewares/six_base_http_middleware.py
+-rw-r--r--   0 mac        (501) staff       (20)     3924 2023-07-03 02:16:20.000000 sixth-python-0.1.2/sixth/middlewares/six_independent_rate_limiter.py
+-rw-r--r--   0 mac        (501) staff       (20)     5856 2023-07-08 18:52:20.000000 sixth-python-0.1.2/sixth/middlewares/six_rate_limiter_middleware.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-07-08 18:57:03.000000 sixth-python-0.1.2/sixth/pen_test/
+-rw-r--r--   0 mac        (501) staff       (20)        0 2023-06-12 15:04:45.000000 sixth-python-0.1.2/sixth/pen_test/__init__.py
+-rw-r--r--   0 mac        (501) staff       (20)      165 2023-06-14 20:44:10.000000 sixth-python-0.1.2/sixth/pen_test/auto_pen_test.py
+-rw-r--r--   0 mac        (501) staff       (20)      921 2023-07-08 18:20:56.000000 sixth-python-0.1.2/sixth/schemas.py
+-rw-r--r--   0 mac        (501) staff       (20)     4190 2023-07-03 02:16:20.000000 sixth-python-0.1.2/sixth/sdk.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-07-08 18:57:03.000000 sixth-python-0.1.2/sixth/utils/
+-rw-r--r--   0 mac        (501) staff       (20)        0 2023-06-10 23:13:17.000000 sixth-python-0.1.2/sixth/utils/__init__.py
+-rw-r--r--   0 mac        (501) staff       (20)     4254 2023-06-12 02:56:13.000000 sixth-python-0.1.2/sixth/utils/encryption_utils.py
+-rw-rw-r--   0 mac        (501) staff       (20)     1707 2023-06-09 19:33:11.000000 sixth-python-0.1.2/sixth/utils/time_utils.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-07-08 18:57:03.000000 sixth-python-0.1.2/sixth_python.egg-info/
+-rw-r--r--   0 mac        (501) staff       (20)     3101 2023-07-08 18:57:03.000000 sixth-python-0.1.2/sixth_python.egg-info/PKG-INFO
+-rw-r--r--   0 mac        (501) staff       (20)      604 2023-07-08 18:57:03.000000 sixth-python-0.1.2/sixth_python.egg-info/SOURCES.txt
+-rw-r--r--   0 mac        (501) staff       (20)        1 2023-07-08 18:57:03.000000 sixth-python-0.1.2/sixth_python.egg-info/dependency_links.txt
+-rw-r--r--   0 mac        (501) staff       (20)      610 2023-07-08 18:57:03.000000 sixth-python-0.1.2/sixth_python.egg-info/requires.txt
+-rw-r--r--   0 mac        (501) staff       (20)        6 2023-07-08 18:57:03.000000 sixth-python-0.1.2/sixth_python.egg-info/top_level.txt
```

### Comparing `sixth-python-0.1.1/PKG-INFO` & `sixth-python-0.1.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: sixth-python
-Version: 0.1.1
-Summary: Six offical python package
+Version: 0.1.2
+Summary: Sixth offical python package
 Home-page: UNKNOWN
 Author: 6thSense
 Author-email: tech@withsix.co
 License: UNKNOWN
 Description: 
         # **Sixth**
         
@@ -37,15 +37,15 @@
         ```sh
         pip install sixth-python
         ```
         
         #### _usage_
         ```python
         #import sixth SDK
-        from sixth.sdk import SixthSense
+        from sixth.sdk import Sixth
         from fastapi import FastAPI
         
         app = FastAPI()
         # initalize app, add routes, middleware, exception handlers etc
         
         
         #....
@@ -62,20 +62,20 @@
         
         ```sh
         npm i sixth-node
         ```
         
         #### _usage_
         ```js
-        import SixthSense from "sixth-node";
+        import Sixth from "sixth-node";
         import  express  from "express";
         
         const app = express();
         
-        const six = new SixthSense("apikey", app)
+        const six = new Sixth("apikey", app)
         await six.init()
         // add routes, middleware, exception handlers etc
         
         
         // after done adding routes, middleware, etc
         six.sync_project();
         app.listen(PORT, ()=> console.log(`Server running on port: http://localhost:${PORT}`))
```

### Comparing `sixth-python-0.1.1/README.md` & `sixth-python-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `sixth-python-0.1.1/setup.py` & `sixth-python-0.1.2/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 from pip._internal.req import parse_requirements
 
 
 
 
-VERSION = '0.1.1'
-DESCRIPTION = 'Six offical python package'
+VERSION = '0.1.2'
+DESCRIPTION = 'Sixth offical python package'
 LONG_DESCRIPTION = '''
 # **Sixth**
 
 
 [![N|Solid](https://firebasestorage.googleapis.com/v0/b/test-103bf.appspot.com/o/waves.png?alt=media&token=0fa4c489-d9c9-4a3b-9178-593b2b018613)](https://nodesource.com/products/nsolid)
 
 Sixth helps you proactively identify security vulnerabilities and prevent cyberattacks on your system that could cost you millions of dollars.
@@ -37,15 +37,15 @@
 ```sh
 pip install sixth-python
 ```
 
 #### _usage_
 ```python
 #import sixth SDK
-from sixth.sdk import SixthSense
+from sixth.sdk import Sixth
 from fastapi import FastAPI
 
 app = FastAPI()
 # initalize app, add routes, middleware, exception handlers etc
 
 
 #....
@@ -62,20 +62,20 @@
 
 ```sh
 npm i sixth-node
 ```
 
 #### _usage_
 ```js
-import SixthSense from "sixth-node";
+import Sixth from "sixth-node";
 import  express  from "express";
 
 const app = express();
 
-const six = new SixthSense("apikey", app)
+const six = new Sixth("apikey", app)
 await six.init()
 // add routes, middleware, exception handlers etc
 
 
 // after done adding routes, middleware, etc
 six.sync_project();
 app.listen(PORT, ()=> console.log(`Server running on port: http://localhost:${PORT}`))
```

### Comparing `sixth-python-0.1.1/sixth/middlewares/encryption_middleware.py` & `sixth-python-0.1.2/sixth/middlewares/encryption_middleware.py`

 * *Files identical despite different names*

### Comparing `sixth-python-0.1.1/sixth/middlewares/six_base_http_middleware.py` & `sixth-python-0.1.2/sixth/middlewares/six_base_http_middleware.py`

 * *Files identical despite different names*

### Comparing `sixth-python-0.1.1/sixth/middlewares/six_independent_rate_limiter.py` & `sixth-python-0.1.2/sixth/middlewares/six_independent_rate_limiter.py`

 * *Files identical despite different names*

### Comparing `sixth-python-0.1.1/sixth/middlewares/six_rate_limiter_middleware.py` & `sixth-python-0.1.2/sixth/middlewares/six_rate_limiter_middleware.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,31 +74,39 @@
         host = request.client.host
         route = request.scope["path"]
         route = re.sub(r'\W+', '~', route)
         headers = request.headers
         #fail safe if there is an internal server error our servers are currenly in maintnance
         try:
             rate_limit_resp = requests.get("https://backend.withsix.co/project-config/config/get-route-rate-limit/"+self._apikey+"/"+route)
-            body = await request.body()
-            
-            await self.set_body(request, body)
-            body = await self._parse_bools(body)
+            body = None
+
+            try:
+                body = await request.body()
+                await self.set_body(request, body)
+                body = await self._parse_bools(body)
+            except:
+                pass
            
             if rate_limit_resp.status_code == 200:
                 try:
                     rate_limit = schemas.RateLimiter.parse_obj(rate_limit_resp.json())
                     self._config.rate_limiter[route] = rate_limit
                     preferred_id = self._config.rate_limiter[route].unique_id
                    
                     if preferred_id == "" or preferred_id=="host":
                         preferred_id = host
                         
                     else:
                         if rate_limit.rate_limit_type == "body":
-                            preferred_id = body[preferred_id]
+                            if body != None:
+                                preferred_id = body[preferred_id]
+                            else:
+                                _response = await call_next(request)
+                                return _response
                         elif rate_limit.rate_limit_type == "header":
                             preferred_id = headers[preferred_id]
                         else:
                             preferred_id = host
                     
 
                     if self._is_rate_limit_reached(preferred_id, route):
```

### Comparing `sixth-python-0.1.1/sixth/schemas.py` & `sixth-python-0.1.2/sixth/schemas.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from pydantic import BaseModel
 from typing import List, Optional, Dict
 import uuid
 
 
 class RateLimiter(BaseModel): 
-    error_payload_id = str(uuid.uuid4())
+    error_payload_id: str = str(uuid.uuid4())
     id: str
     route: str
     interval: int 
     rate_limit: int
     last_updated: float 
     created_at: float
     rate_limit_type: str = "ip address" #ip address, header, body
```

### Comparing `sixth-python-0.1.1/sixth/sdk.py` & `sixth-python-0.1.2/sixth/sdk.py`

 * *Files identical despite different names*

### Comparing `sixth-python-0.1.1/sixth/utils/encryption_utils.py` & `sixth-python-0.1.2/sixth/utils/encryption_utils.py`

 * *Files identical despite different names*

### Comparing `sixth-python-0.1.1/sixth/utils/time_utils.py` & `sixth-python-0.1.2/sixth/utils/time_utils.py`

 * *Files identical despite different names*

### Comparing `sixth-python-0.1.1/sixth_python.egg-info/PKG-INFO` & `sixth-python-0.1.2/sixth_python.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: sixth-python
-Version: 0.1.1
-Summary: Six offical python package
+Version: 0.1.2
+Summary: Sixth offical python package
 Home-page: UNKNOWN
 Author: 6thSense
 Author-email: tech@withsix.co
 License: UNKNOWN
 Description: 
         # **Sixth**
         
@@ -37,15 +37,15 @@
         ```sh
         pip install sixth-python
         ```
         
         #### _usage_
         ```python
         #import sixth SDK
-        from sixth.sdk import SixthSense
+        from sixth.sdk import Sixth
         from fastapi import FastAPI
         
         app = FastAPI()
         # initalize app, add routes, middleware, exception handlers etc
         
         
         #....
@@ -62,20 +62,20 @@
         
         ```sh
         npm i sixth-node
         ```
         
         #### _usage_
         ```js
-        import SixthSense from "sixth-node";
+        import Sixth from "sixth-node";
         import  express  from "express";
         
         const app = express();
         
-        const six = new SixthSense("apikey", app)
+        const six = new Sixth("apikey", app)
         await six.init()
         // add routes, middleware, exception handlers etc
         
         
         // after done adding routes, middleware, etc
         six.sync_project();
         app.listen(PORT, ()=> console.log(`Server running on port: http://localhost:${PORT}`))
```

### Comparing `sixth-python-0.1.1/sixth_python.egg-info/SOURCES.txt` & `sixth-python-0.1.2/sixth_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sixth-python-0.1.1/sixth_python.egg-info/requires.txt` & `sixth-python-0.1.2/sixth_python.egg-info/requires.txt`

 * *Files identical despite different names*

