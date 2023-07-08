# Comparing `tmp/dynamic-service-1.3.1.tar.gz` & `tmp/dynamic-service-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dynamic-service-1.3.1.tar", last modified: Sat Jul  8 12:13:04 2023, max compression
+gzip compressed data, was "dynamic-service-1.4.0.tar", last modified: Sat Jul  8 16:06:07 2023, max compression
```

## Comparing `dynamic-service-1.3.1.tar` & `dynamic-service-1.4.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2023-07-08 12:13:04.272884 dynamic-service-1.3.1/
--rw-rw-rw-   0        0        0      236 2023-07-08 12:13:02.000000 dynamic-service-1.3.1/MANIFEST.in
--rw-rw-rw-   0        0        0     2023 2023-07-08 12:13:04.271884 dynamic-service-1.3.1/PKG-INFO
--rw-rw-rw-   0        0        0     1226 2023-07-01 09:47:05.000000 dynamic-service-1.3.1/README.md
--rw-rw-rw-   0        0        0    12920 2023-07-01 09:47:05.000000 dynamic-service-1.3.1/build.py
-drwxrwxrwx   0        0        0        0 2023-07-08 12:13:04.215885 dynamic-service-1.3.1/dynamic_service/
--rw-rw-rw-   0        0        0     1439 2023-07-01 09:47:05.000000 dynamic-service-1.3.1/dynamic_service/base.py
-drwxrwxrwx   0        0        0        0 2023-07-08 12:13:04.257884 dynamic-service-1.3.1/dynamic_service/endpoints/
--rw-rw-rw-   0        0        0      210 2023-07-01 09:47:05.000000 dynamic-service-1.3.1/dynamic_service/endpoints/__init__.py
--rw-rw-rw-   0        0        0     2539 2023-07-03 14:24:04.000000 dynamic-service-1.3.1/dynamic_service/endpoints/data.py
--rw-rw-rw-   0        0        0     9234 2023-07-03 14:30:46.000000 dynamic-service-1.3.1/dynamic_service/endpoints/engine.py
--rw-rw-rw-   0        0        0     1569 2023-07-03 06:52:10.000000 dynamic-service-1.3.1/dynamic_service/endpoints/exceptions.py
--rw-rw-rw-   0        0        0     1608 2023-07-03 06:51:55.000000 dynamic-service-1.3.1/dynamic_service/endpoints/process.py
-drwxrwxrwx   0        0        0        0 2023-07-08 12:13:04.265884 dynamic-service-1.3.1/dynamic_service/service/
--rw-rw-rw-   0        0        0      106 2023-07-01 09:47:05.000000 dynamic-service-1.3.1/dynamic_service/service/__init__.py
--rw-rw-rw-   0        0        0    20625 2023-07-08 12:06:30.000000 dynamic-service-1.3.1/dynamic_service/service/rest.py
--rw-rw-rw-   0        0        0     3387 2023-07-08 10:41:33.000000 dynamic-service-1.3.1/dynamic_service/service/sockets.py
-drwxrwxrwx   0        0        0        0 2023-07-08 12:13:04.205808 dynamic-service-1.3.1/dynamic_service/source/
-drwxrwxrwx   0        0        0        0 2023-07-08 12:13:04.205808 dynamic-service-1.3.1/dynamic_service/source/assets/
-drwxrwxrwx   0        0        0        0 2023-07-08 12:13:04.270884 dynamic-service-1.3.1/dynamic_service/source/assets/icon/
--rw-rw-rw-   0        0        0     2834 2023-07-01 09:47:05.000000 dynamic-service-1.3.1/dynamic_service/source/assets/icon/icon.ico
--rw-rw-rw-   0        0        0    27619 2023-07-01 09:47:05.000000 dynamic-service-1.3.1/dynamic_service/source/assets/icon/icon.png
-drwxrwxrwx   0        0        0        0 2023-07-08 12:13:04.229884 dynamic-service-1.3.1/dynamic_service.egg-info/
--rw-rw-rw-   0        0        0     2023 2023-07-08 12:13:04.000000 dynamic-service-1.3.1/dynamic_service.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      686 2023-07-08 12:13:04.000000 dynamic-service-1.3.1/dynamic_service.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-08 12:13:04.000000 dynamic-service-1.3.1/dynamic_service.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       83 2023-07-08 12:13:04.000000 dynamic-service-1.3.1/dynamic_service.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-07-08 12:13:04.000000 dynamic-service-1.3.1/dynamic_service.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      627 2023-07-08 12:13:02.000000 dynamic-service-1.3.1/pyproject.toml
--rw-rw-rw-   0        0        0       85 2023-07-03 14:45:22.000000 dynamic-service-1.3.1/requirements-dev.txt
--rw-rw-rw-   0        0        0       69 2023-07-01 09:47:05.000000 dynamic-service-1.3.1/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-07-08 12:13:04.272884 dynamic-service-1.3.1/setup.cfg
--rw-rw-rw-   0        0        0     1603 2023-07-08 12:12:54.000000 dynamic-service-1.3.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-08 16:06:07.432208 dynamic-service-1.4.0/
+-rw-rw-rw-   0        0        0      236 2023-07-08 16:06:07.000000 dynamic-service-1.4.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     2023 2023-07-08 16:06:07.431201 dynamic-service-1.4.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1226 2023-07-01 09:47:05.000000 dynamic-service-1.4.0/README.md
+-rw-rw-rw-   0        0        0    12920 2023-07-01 09:47:05.000000 dynamic-service-1.4.0/build.py
+drwxrwxrwx   0        0        0        0 2023-07-08 16:06:07.378543 dynamic-service-1.4.0/dynamic_service/
+-rw-rw-rw-   0        0        0     1439 2023-07-01 09:47:05.000000 dynamic-service-1.4.0/dynamic_service/base.py
+drwxrwxrwx   0        0        0        0 2023-07-08 16:06:07.416293 dynamic-service-1.4.0/dynamic_service/endpoints/
+-rw-rw-rw-   0        0        0      210 2023-07-01 09:47:05.000000 dynamic-service-1.4.0/dynamic_service/endpoints/__init__.py
+-rw-rw-rw-   0        0        0     2539 2023-07-03 14:24:04.000000 dynamic-service-1.4.0/dynamic_service/endpoints/data.py
+-rw-rw-rw-   0        0        0     8954 2023-07-08 15:55:29.000000 dynamic-service-1.4.0/dynamic_service/endpoints/engine.py
+-rw-rw-rw-   0        0        0     1569 2023-07-03 06:52:10.000000 dynamic-service-1.4.0/dynamic_service/endpoints/exceptions.py
+-rw-rw-rw-   0        0        0     1608 2023-07-03 06:51:55.000000 dynamic-service-1.4.0/dynamic_service/endpoints/process.py
+drwxrwxrwx   0        0        0        0 2023-07-08 16:06:07.426185 dynamic-service-1.4.0/dynamic_service/service/
+-rw-rw-rw-   0        0        0      106 2023-07-01 09:47:05.000000 dynamic-service-1.4.0/dynamic_service/service/__init__.py
+-rw-rw-rw-   0        0        0    20599 2023-07-08 16:05:28.000000 dynamic-service-1.4.0/dynamic_service/service/rest.py
+-rw-rw-rw-   0        0        0     3387 2023-07-08 10:41:33.000000 dynamic-service-1.4.0/dynamic_service/service/sockets.py
+drwxrwxrwx   0        0        0        0 2023-07-08 16:06:07.368055 dynamic-service-1.4.0/dynamic_service/source/
+drwxrwxrwx   0        0        0        0 2023-07-08 16:06:07.368055 dynamic-service-1.4.0/dynamic_service/source/assets/
+drwxrwxrwx   0        0        0        0 2023-07-08 16:06:07.430215 dynamic-service-1.4.0/dynamic_service/source/assets/icon/
+-rw-rw-rw-   0        0        0     2834 2023-07-01 09:47:05.000000 dynamic-service-1.4.0/dynamic_service/source/assets/icon/icon.ico
+-rw-rw-rw-   0        0        0    27619 2023-07-01 09:47:05.000000 dynamic-service-1.4.0/dynamic_service/source/assets/icon/icon.png
+drwxrwxrwx   0        0        0        0 2023-07-08 16:06:07.392599 dynamic-service-1.4.0/dynamic_service.egg-info/
+-rw-rw-rw-   0        0        0     2023 2023-07-08 16:06:07.000000 dynamic-service-1.4.0/dynamic_service.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      686 2023-07-08 16:06:07.000000 dynamic-service-1.4.0/dynamic_service.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-08 16:06:07.000000 dynamic-service-1.4.0/dynamic_service.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       89 2023-07-08 16:06:07.000000 dynamic-service-1.4.0/dynamic_service.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-07-08 16:06:07.000000 dynamic-service-1.4.0/dynamic_service.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      627 2023-07-08 16:06:07.000000 dynamic-service-1.4.0/pyproject.toml
+-rw-rw-rw-   0        0        0       92 2023-07-08 15:54:50.000000 dynamic-service-1.4.0/requirements-dev.txt
+-rw-rw-rw-   0        0        0       76 2023-07-08 15:54:50.000000 dynamic-service-1.4.0/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-07-08 16:06:07.432208 dynamic-service-1.4.0/setup.cfg
+-rw-rw-rw-   0        0        0     1603 2023-07-08 16:06:01.000000 dynamic-service-1.4.0/setup.py
```

### Comparing `dynamic-service-1.3.1/PKG-INFO` & `dynamic-service-1.4.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dynamic-service
-Version: 1.3.1
+Version: 1.4.0
 Summary: A framework for developing responsive, live and dynamic REST APIs with python.
 Home-page: https://github.com/Shahaf-F-S/dynamic-service
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `dynamic-service-1.3.1/README.md` & `dynamic-service-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `dynamic-service-1.3.1/build.py` & `dynamic-service-1.4.0/build.py`

 * *Files identical despite different names*

### Comparing `dynamic-service-1.3.1/dynamic_service/base.py` & `dynamic-service-1.4.0/dynamic_service/base.py`

 * *Files identical despite different names*

### Comparing `dynamic-service-1.3.1/dynamic_service/endpoints/data.py` & `dynamic-service-1.4.0/dynamic_service/endpoints/data.py`

 * *Files identical despite different names*

### Comparing `dynamic-service-1.3.1/dynamic_service/endpoints/engine.py` & `dynamic-service-1.4.0/dynamic_service/endpoints/engine.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,36 +1,37 @@
 # engine.py
 
-from dataclasses import dataclass, field
 from functools import wraps
 from typing import (
     List, Any, Dict, Optional,
     Tuple, Callable, Iterable, TypeVar, Generic
 )
 
+from attrs import define, field
+
 from fastapi.openapi.docs import get_swagger_ui_html, HTMLResponse
 
 from represent import Modifiers, represent
 
 from dynamic_service.endpoints.data import DOCS
 
 __all__ = [
     "BaseEndpoint",
     "DocsEndpoint",
     "Record",
     "valid_endpoints"
 ]
 
-@dataclass(repr=False, slots=True)
+@define(repr=False)
 @represent
 class Record:
     """A class to represent a result object for commands and conditions calls."""
 
-    args: Optional[Tuple] = field(default_factory=tuple),
-    kwargs: Optional[Dict[str, Any]] = field(default_factory=dict),
+    args: Optional[Tuple] = field(factory=tuple),
+    kwargs: Optional[Dict[str, Any]] = field(factory=dict),
     returns: Optional[Any] = None
 
     def collect(
             self, *,
             args: Optional[Tuple] = None,
             kwargs: Optional[Dict[str, Any]] = None,
             returns: Optional[Any] = None
@@ -101,14 +102,19 @@
     __modifiers__ = Modifiers(
         excluded=["options"], hidden=["record", "service"]
     )
 
     PATH: str
     METHODS: List[str]
 
+    __slots__ = (
+        "path", "methods", "service", "description",
+        "root", "options", "record"
+    )
+
     def __init__(
             self,
             path: Optional[str] = None,
             methods: Optional[Iterable[str]] = None,
             service: Optional[_ServiceType] = None,
             description: Optional[str] = None,
             root: Optional[str] = None,
@@ -202,34 +208,14 @@
 
             return endpoint(*args[1:], **kwargs)
         # end wrapper
 
         return wrapper
     # end process
 
-    def set_root(self, root: str, /) -> None:
-        """
-        Sets the root path of the endpoint.
-
-        :param root: The root path.
-        """
-
-        self.root = root
-    # end set_root
-
-    def get_root(self) -> str:
-        """
-        Gets the root path of the endpoint.
-
-        :returns: The root path.
-        """
-
-        return self.root
-    # end get_root
-
     def endpoint(self, *args: Any, **kwargs: Any) -> _ReturnType:
         """
         Returns the response for the API endpoint.
 
         :param args: The positional arguments.
         :param kwargs: Any keyword argument.
 
@@ -237,14 +223,16 @@
         """
     # end endpoint
 # end BaseEndpoint
 
 class DocsEndpoint(BaseEndpoint):
     """A class to represent an endpoint."""
 
+    __slots__ = "icon", "title"
+
     def __init__(
             self,
             methods: Optional[Iterable[str]] = None,
             service: Optional[object] = None,
             title: Optional[str] = None,
             description: Optional[str] = None,
             icon: Optional[str] = None,
```

### Comparing `dynamic-service-1.3.1/dynamic_service/endpoints/exceptions.py` & `dynamic-service-1.4.0/dynamic_service/endpoints/exceptions.py`

 * *Files identical despite different names*

### Comparing `dynamic-service-1.3.1/dynamic_service/endpoints/process.py` & `dynamic-service-1.4.0/dynamic_service/endpoints/process.py`

 * *Files identical despite different names*

### Comparing `dynamic-service-1.3.1/dynamic_service/service/rest.py` & `dynamic-service-1.4.0/dynamic_service/service/rest.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,14 +79,16 @@
     # end if
 
     return command
 # end override_signature
 
 class Endpoint(partial):
     """A class to wrap around an endpoint object."""
+
+    __slots__ = ()
 # end Endpoint
 
 class RESTService(ServiceInterface):
     """
     A class to represent a service object.
 
     The BaseService is the parent class of service class.
@@ -133,22 +135,17 @@
     """
 
     SILENT = False
 
     ICON = icons() + "\\icon.ico"
     VERSION = "0.0.0"
     DESCRIPTION = ""
-    NAME = "Live Auto-API Service"
+    NAME = "Dynamic-Service"
 
-    __modifiers__ = Modifiers(
-        excluded=[
-            "app", "_root", "timeout_process",
-            "service_process", "modifiers"
-        ]
-    )
+    __modifiers__ = Modifiers(excluded=["app", "server"])
 
     def __init__(
             self,
             name: Optional[str] = None,
             version: Optional[str] = None,
             endpoints: Optional[EndpointsContainer] = None,
             root: Optional[str] = None,
@@ -168,15 +165,15 @@
         :param root: The root to the path.
         :param home: The home endpoint.
         :param debug: The value to create the docs' endpoint for the home endpoint.
         """
 
         super().__init__()
 
-        self._root = None
+        self._root: Optional[str] = None
 
         _Base = type(self)
 
         self.endpoints: Dict[str, BaseEndpoint[_Base]] = {}
 
         if (
             (isinstance(home, bool) and home) or
@@ -184,17 +181,17 @@
         ):
             home = True
         # end if
 
         self.app: Optional[FastAPI] = None
         self.server: Optional[Server] = None
 
-        self._service_process: Optional[threading.Thread] = None
+        self._serving_process: Optional[threading.Thread] = None
 
-        self._run_parameters: Optional[Dict[str, Any]] = None
+        self._running_parameters: Optional[Dict[str, Any]] = None
 
         self._serving = False
 
         self.description = description or self.DESCRIPTION
         self.root = root or ""
         self.icon = icon or self.ICON
         self.home = home
@@ -211,18 +208,19 @@
     def __getstate__(self) -> Dict[str, Any]:
         """
         Gets the state of the object.
 
         :return: The state of the object.
         """
 
-        data = self.__dict__.copy()
+        data = super().__getstate__()
 
         data["app"] = None
-        data["_service_process"] = None
+        data["server"] = None
+        data["_serving_process"] = None
 
         return data
     # end __getstate__
 
     @staticmethod
     def valid_endpoints(endpoints: Optional[Any] = None) -> Endpoints:
         """
@@ -311,15 +309,15 @@
     def created(self) -> bool:
         """
         Checks if the service was created.
 
         :return: The value for the service being created.
         """
 
-        return isinstance(self._service_process, threading.Thread)
+        return isinstance(self._serving_process, threading.Thread)
     # end created
 
     def add_endpoint(self, endpoint: BaseEndpoint, path: Optional[str] = None) -> None:
         """
         Adds the endpoint to the service.
 
         :param path: The path for the endpoint.
@@ -459,15 +457,15 @@
             version=self.version,
             docs_url=None
         )
 
         router = APIRouter()
 
         for endpoint in self.endpoints.values():
-            endpoint.set_root(self.root)
+            endpoint.root = self.root
 
             path = ("/" + endpoint.root if endpoint.root else '') + endpoint.path
 
             command = override_signature(
                 Endpoint(endpoint.__call__, endpoint),
                 new=endpoint.endpoint, name=type(endpoint).__name__
             )
@@ -545,15 +543,15 @@
 
         self.server = Server(
             config=ServiceConfig(
                 app=self.app, host=host, port=port
             )
         )
 
-        self._service_process = threading.Thread(
+        self._serving_process = threading.Thread(
             target=lambda: (
                 (
                     logging.disable(logging.INFO) if silent else ()
                 ), self.server.run()
             ), daemon=daemon
         )
     # end create
@@ -583,15 +581,15 @@
         if not self.created:
             self.create(
                 host=host, port=port, silent=silent,
                 daemon=daemon
             )
         # end if
 
-        self._service_process.start()
+        self._serving_process.start()
     # end start_serving
 
     def run(
             self,
             serve: Optional[bool] = True,
             host: Optional[Host] = None,
             port: Optional[Port] = None,
@@ -614,15 +612,15 @@
         :param block: The value to block the execution and wain for the service.
         :param refresh: The value to refresh the system.
         :param update: The value to update the service.
         :param wait: The waiting time.
         :param timeout: The start_timeout for the process.
         """
 
-        self._run_parameters = dict(
+        self._running_parameters = dict(
             host=host, port=port, serve=serve,
             silent=silent, daemon=daemon, wait=wait,
             update=update, refresh=refresh,
             timeout=timeout, block=block
         )
 
         if serve:
@@ -676,28 +674,28 @@
         )
 
         parameters = {
             key: value for key, value in parameters.items()
             if value is not None
         }
 
-        self._run_parameters.update(parameters)
+        self._running_parameters.update(parameters)
 
-        self.run(**self._run_parameters)
+        self.run(**self._running_parameters)
     # end rerun
 
     def stop_serving(self) -> None:
         """Stops the service process."""
 
         if self.serving:
             self._serving = False
         # end if
 
-        if self.created and self._service_process.is_alive():
-            self._service_process = None
+        if self.created and self._serving_process.is_alive():
+            self._serving_process = None
         # end if
     # end stop_serving
 
     def terminate(self) -> None:
         """Pauses the process of service."""
 
         super().terminate()
```

### Comparing `dynamic-service-1.3.1/dynamic_service/service/sockets.py` & `dynamic-service-1.4.0/dynamic_service/service/sockets.py`

 * *Files identical despite different names*

### Comparing `dynamic-service-1.3.1/dynamic_service/source/assets/icon/icon.ico` & `dynamic-service-1.4.0/dynamic_service/source/assets/icon/icon.ico`

 * *Files identical despite different names*

### Comparing `dynamic-service-1.3.1/dynamic_service/source/assets/icon/icon.png` & `dynamic-service-1.4.0/dynamic_service/source/assets/icon/icon.png`

 * *Files identical despite different names*

### Comparing `dynamic-service-1.3.1/dynamic_service.egg-info/PKG-INFO` & `dynamic-service-1.4.0/dynamic_service.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dynamic-service
-Version: 1.3.1
+Version: 1.4.0
 Summary: A framework for developing responsive, live and dynamic REST APIs with python.
 Home-page: https://github.com/Shahaf-F-S/dynamic-service
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `dynamic-service-1.3.1/dynamic_service.egg-info/SOURCES.txt` & `dynamic-service-1.4.0/dynamic_service.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dynamic-service-1.3.1/pyproject.toml` & `dynamic-service-1.4.0/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = 'dynamic-service'
-version = '1.3.1'
+version = '1.4.0'
 description = 'A framework for developing responsive, live and dynamic REST APIs with python.'
 classifiers = [
 	'Intended Audience :: Developers',
 	'License :: OSI Approved :: MIT License',
 	'Programming Language :: Python',
 	'Programming Language :: Python :: 3',
 	'Programming Language :: Python :: 3.8',
```

### Comparing `dynamic-service-1.3.1/setup.py` & `dynamic-service-1.4.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
         ],
         include=[
             "dynamic_service/source"
         ],
         requirements="requirements.txt",
         dev_requirements="requirements-dev.txt",
         name='dynamic-service',
-        version='1.3.1',
+        version='1.4.0',
         description=(
             "A framework for developing responsive, "
             "live and dynamic REST APIs with python."
         ),
         license='MIT',
         author="Shahaf Frank-Shapir",
         author_email='shahaffrs@gmail.com',
```

