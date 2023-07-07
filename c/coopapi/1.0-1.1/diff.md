# Comparing `tmp/coopapi-1.0.tar.gz` & `tmp/coopapi-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coopapi-1.0.tar", last modified: Thu Jul  6 15:53:45 2023, max compression
+gzip compressed data, was "coopapi-1.1.tar", last modified: Fri Jul  7 22:21:44 2023, max compression
```

## Comparing `coopapi-1.0.tar` & `coopapi-1.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-07-06 15:53:45.278031 coopapi-1.0/
--rw-rw-rw-   0        0        0     2838 2023-07-06 15:53:45.277031 coopapi-1.0/PKG-INFO
--rw-rw-rw-   0        0        0     2087 2023-01-10 15:30:28.000000 coopapi-1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-06 15:53:45.230080 coopapi-1.0/coopapi/
--rw-rw-rw-   0        0        0      324 2023-07-06 13:56:43.000000 coopapi-1.0/coopapi/__init__.py
--rw-rw-rw-   0        0        0    11887 2023-07-06 13:58:02.000000 coopapi-1.0/coopapi/apiShell.py
--rw-rw-rw-   0        0        0      214 2023-02-23 19:25:03.000000 coopapi-1.0/coopapi/enums.py
--rw-rw-rw-   0        0        0      185 2022-12-06 20:55:58.000000 coopapi-1.0/coopapi/errors.py
--rw-rw-rw-   0        0        0     5954 2023-06-02 17:15:47.000000 coopapi-1.0/coopapi/http_request.py
--rw-rw-rw-   0        0        0     6269 2023-07-06 15:51:17.000000 coopapi-1.0/coopapi/http_request_handlers.py
-drwxrwxrwx   0        0        0        0 2023-07-06 15:53:45.274038 coopapi-1.0/coopapi.egg-info/
--rw-rw-rw-   0        0        0     2838 2023-07-06 15:53:45.000000 coopapi-1.0/coopapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      334 2023-07-06 15:53:45.000000 coopapi-1.0/coopapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-06 15:53:45.000000 coopapi-1.0/coopapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-01-10 15:32:25.000000 coopapi-1.0/coopapi.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      279 2023-07-06 15:53:45.000000 coopapi-1.0/coopapi.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-07-06 15:53:45.000000 coopapi-1.0/coopapi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-06 15:53:45.279034 coopapi-1.0/setup.cfg
--rw-rw-rw-   0        0        0     1236 2023-07-06 15:53:22.000000 coopapi-1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-07 22:21:44.423658 coopapi-1.1/
+-rw-rw-rw-   0        0        0     2838 2023-07-07 22:21:44.422621 coopapi-1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2087 2023-01-10 15:30:28.000000 coopapi-1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-07 22:21:44.393655 coopapi-1.1/coopapi/
+-rw-rw-rw-   0        0        0      324 2023-07-06 13:56:43.000000 coopapi-1.1/coopapi/__init__.py
+-rw-rw-rw-   0        0        0    12325 2023-07-06 16:43:24.000000 coopapi-1.1/coopapi/apiShell.py
+-rw-rw-rw-   0        0        0      214 2023-02-23 19:25:03.000000 coopapi-1.1/coopapi/enums.py
+-rw-rw-rw-   0        0        0      185 2022-12-06 20:55:58.000000 coopapi-1.1/coopapi/errors.py
+-rw-rw-rw-   0        0        0     5954 2023-06-02 17:15:47.000000 coopapi-1.1/coopapi/http_request.py
+-rw-rw-rw-   0        0        0     6269 2023-07-06 15:51:17.000000 coopapi-1.1/coopapi/http_request_handlers.py
+drwxrwxrwx   0        0        0        0 2023-07-07 22:21:44.420659 coopapi-1.1/coopapi.egg-info/
+-rw-rw-rw-   0        0        0     2838 2023-07-07 22:21:44.000000 coopapi-1.1/coopapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      334 2023-07-07 22:21:44.000000 coopapi-1.1/coopapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-07 22:21:44.000000 coopapi-1.1/coopapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-01-10 15:32:25.000000 coopapi-1.1/coopapi.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      504 2023-07-07 22:21:44.000000 coopapi-1.1/coopapi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-07-07 22:21:44.000000 coopapi-1.1/coopapi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-07 22:21:44.423658 coopapi-1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1237 2023-07-07 22:21:41.000000 coopapi-1.1/setup.py
```

### Comparing `coopapi-1.0/PKG-INFO` & `coopapi-1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coopapi
-Version: 1.0
+Version: 1.1
 Summary: Tools for setting up an API. Built on the FastAPI framework
 Home-page: https://github.com/tylertjburns/coopapi
 Author: tburns
 Author-email: tyler.tj.burns@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `coopapi-1.0/README.md` & `coopapi-1.1/README.md`

 * *Files identical despite different names*

### Comparing `coopapi-1.0/coopapi/apiShell.py` & `coopapi-1.1/coopapi/apiShell.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,31 +1,39 @@
 import uvicorn
 from fastapi import Body, Request, status
 from coopapi import http_request_handlers as hrh
-from typing import Any, Dict, List, Callable, Tuple
+from typing import Any, Dict, List, Callable, Tuple, Optional
 from fastapi import APIRouter
 from pydantic.dataclasses import dataclass as pydataclass, Field
 from dataclasses import dataclass, field
 import json
 from urllib.parse import parse_qs
 import logging
 from coopapi.enums import RequestType
 
 logger = logging.getLogger('APIHandler')
 
-
 def route(callback: hrh.requestCallback,
-          schema: type):
-    def internal(request: Request, item: schema = Body(...)) -> schema:
-        ret = hrh.request_handler(request=request,
-                                       item=item,
-                                       callback=callback
-                                       )
+          schema: type = None):
+    if schema is None:
+        def internal(request: Request)-> schema:
+            ret = hrh.request_handler(request=request,
+                                      item=None,
+                                      callback=callback
+                                      )
+
+            return ret
+    else:
+        def internal(request: Request, item: schema = Body(...)) -> schema:
+            ret = hrh.request_handler(request=request,
+                                           item=item,
+                                           callback=callback
+                                           )
 
-        return ret
+            return ret
     return internal
 
 
 
 
 # def post_route(create_callback: hrh.postRequestCallback,
 #                schema: type):
@@ -101,48 +109,48 @@
 #         return ret
 #     return dirty_post_route
 
 # class Config:
 #     arbitrary_types_allowed = True
 
 @dataclass
-class CallbackPackage:
+class RequestCallbackPackage:
     method: RequestType
     callback: Callable
-    input_schema: type
     response_schema: type
+    input_body_schema: Optional[type]
 
 @dataclass
 class ApiShell:
     base_route: str
-    on_post_callback: CallbackPackage = field(default=None)
-    on_put_callback: CallbackPackage = field(default=None)
-    on_delete_callback: CallbackPackage = field(default=None)
-    on_getone_callback: CallbackPackage = field(default=None)
-    on_getmany_callback: CallbackPackage = field(default=None)
+    on_post_callback: RequestCallbackPackage = field(default=None)
+    on_put_callback: RequestCallbackPackage = field(default=None)
+    on_delete_callback: RequestCallbackPackage = field(default=None)
+    on_getone_callback: RequestCallbackPackage = field(default=None)
+    on_getmany_callback: RequestCallbackPackage = field(default=None)
     # dirty_create: dirtyCleaner = field(default=None)
     router: APIRouter = field(default_factory=APIRouter)
 
 
     def __post_init__(self):
         self.register_routes()
         print(f"{self.base_route} routes registered")
 
     # def __post_init_post_parse__(self):
     #     self.register_routes()
     #     print(f"{self.base_route} routes registered")
 
 
     def _register_route_internal(self,
-                                 callback_package: CallbackPackage):
+                                 callback_package: RequestCallbackPackage):
         self.router.add_api_route(
             f"{self.base_route}/api/",
-            route(callback=callback_package.callback, schema=callback_package.input_schema),
+            route(callback=callback_package.callback, schema=callback_package.input_body_schema),
             methods=[callback_package.method.value],
-            response_description=f"{callback_package.method.value} a new {callback_package.input_schema.__name__}",
+            response_description=f"{callback_package.method.value} a new {callback_package.response_schema.__name__}",
             response_model=callback_package.response_schema,
             status_code=ApiShell._success_status_code(callback_package.method))
 
     @staticmethod
     def _success_status_code(method: RequestType):
         switch = {
             RequestType.POST: status.HTTP_201_CREATED,
@@ -278,18 +286,18 @@
     class DummyOut:
         c: Tuple[str, int]
         e: Dict
 
     def callback(req: Request, i: DummyIn) -> DummyOut:
         return DummyOut(c=(i.a, i.b), e=i.d)
 
-    cpac = CallbackPackage(
+    cpac = RequestCallbackPackage(
         method=RequestType.POST,
         callback=callback,
-        input_schema=DummyIn,
+        input_body_schema=DummyIn,
         response_schema=DummyOut
     )
 
     shell = ApiShell(base_route='/dummy',
                      on_post_callback=cpac)
 
     app = FastAPI()
```

### Comparing `coopapi-1.0/coopapi/http_request.py` & `coopapi-1.1/coopapi/http_request.py`

 * *Files identical despite different names*

### Comparing `coopapi-1.0/coopapi/http_request_handlers.py` & `coopapi-1.1/coopapi/http_request_handlers.py`

 * *Files identical despite different names*

### Comparing `coopapi-1.0/coopapi.egg-info/PKG-INFO` & `coopapi-1.1/coopapi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coopapi
-Version: 1.0
+Version: 1.1
 Summary: Tools for setting up an API. Built on the FastAPI framework
 Home-page: https://github.com/tylertjburns/coopapi
 Author: tburns
 Author-email: tyler.tj.burns@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `coopapi-1.0/setup.py` & `coopapi-1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 with open('README.md') as f:
     README = f.read()
 
 with open('requirements.txt') as f:
     requirements = f.read().splitlines()
 
 setuptools.setup(name='coopapi',
-      version='1.0',
+      version='1.01',
       description='Tools for setting up an API. Built on the FastAPI framework',
       url='https://github.com/tylertjburns/coopapi',
       author='tburns',
       author_email='tyler.tj.burns@gmail.com',
       license='MIT',
       packages=setuptools.find_packages(),
       python_requires=">3.5",
```

