# Comparing `tmp/dynamic-service-1.3.0.tar.gz` & `tmp/dynamic-service-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dynamic-service-1.3.0.tar", last modified: Sat Jul  8 10:41:46 2023, max compression
+gzip compressed data, was "dynamic-service-1.3.1.tar", last modified: Sat Jul  8 12:13:04 2023, max compression
```

## Comparing `dynamic-service-1.3.0.tar` & `dynamic-service-1.3.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2023-07-08 10:41:46.850583 dynamic-service-1.3.0/
--rw-rw-rw-   0        0        0      236 2023-07-08 10:41:46.000000 dynamic-service-1.3.0/MANIFEST.in
--rw-rw-rw-   0        0        0     2023 2023-07-08 10:41:46.850583 dynamic-service-1.3.0/PKG-INFO
--rw-rw-rw-   0        0        0     1226 2023-07-01 09:47:05.000000 dynamic-service-1.3.0/README.md
--rw-rw-rw-   0        0        0    12920 2023-07-01 09:47:05.000000 dynamic-service-1.3.0/build.py
-drwxrwxrwx   0        0        0        0 2023-07-08 10:41:46.834582 dynamic-service-1.3.0/dynamic_service/
--rw-rw-rw-   0        0        0     1439 2023-07-01 09:47:05.000000 dynamic-service-1.3.0/dynamic_service/base.py
-drwxrwxrwx   0        0        0        0 2023-07-08 10:41:46.846582 dynamic-service-1.3.0/dynamic_service/endpoints/
--rw-rw-rw-   0        0        0      210 2023-07-01 09:47:05.000000 dynamic-service-1.3.0/dynamic_service/endpoints/__init__.py
--rw-rw-rw-   0        0        0     2539 2023-07-03 14:24:04.000000 dynamic-service-1.3.0/dynamic_service/endpoints/data.py
--rw-rw-rw-   0        0        0     9234 2023-07-03 14:30:46.000000 dynamic-service-1.3.0/dynamic_service/endpoints/engine.py
--rw-rw-rw-   0        0        0     1569 2023-07-03 06:52:10.000000 dynamic-service-1.3.0/dynamic_service/endpoints/exceptions.py
--rw-rw-rw-   0        0        0     1608 2023-07-03 06:51:55.000000 dynamic-service-1.3.0/dynamic_service/endpoints/process.py
-drwxrwxrwx   0        0        0        0 2023-07-08 10:41:46.848582 dynamic-service-1.3.0/dynamic_service/service/
--rw-rw-rw-   0        0        0      106 2023-07-01 09:47:05.000000 dynamic-service-1.3.0/dynamic_service/service/__init__.py
--rw-rw-rw-   0        0        0    20526 2023-07-07 15:49:38.000000 dynamic-service-1.3.0/dynamic_service/service/rest.py
--rw-rw-rw-   0        0        0     3387 2023-07-08 10:41:33.000000 dynamic-service-1.3.0/dynamic_service/service/sockets.py
-drwxrwxrwx   0        0        0        0 2023-07-08 10:41:46.828581 dynamic-service-1.3.0/dynamic_service/source/
-drwxrwxrwx   0        0        0        0 2023-07-08 10:41:46.828581 dynamic-service-1.3.0/dynamic_service/source/assets/
-drwxrwxrwx   0        0        0        0 2023-07-08 10:41:46.849583 dynamic-service-1.3.0/dynamic_service/source/assets/icon/
--rw-rw-rw-   0        0        0     2834 2023-07-01 09:47:05.000000 dynamic-service-1.3.0/dynamic_service/source/assets/icon/icon.ico
--rw-rw-rw-   0        0        0    27619 2023-07-01 09:47:05.000000 dynamic-service-1.3.0/dynamic_service/source/assets/icon/icon.png
-drwxrwxrwx   0        0        0        0 2023-07-08 10:41:46.843582 dynamic-service-1.3.0/dynamic_service.egg-info/
--rw-rw-rw-   0        0        0     2023 2023-07-08 10:41:46.000000 dynamic-service-1.3.0/dynamic_service.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      686 2023-07-08 10:41:46.000000 dynamic-service-1.3.0/dynamic_service.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-08 10:41:46.000000 dynamic-service-1.3.0/dynamic_service.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       83 2023-07-08 10:41:46.000000 dynamic-service-1.3.0/dynamic_service.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-07-08 10:41:46.000000 dynamic-service-1.3.0/dynamic_service.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      627 2023-07-08 10:41:46.000000 dynamic-service-1.3.0/pyproject.toml
--rw-rw-rw-   0        0        0       85 2023-07-03 14:45:22.000000 dynamic-service-1.3.0/requirements-dev.txt
--rw-rw-rw-   0        0        0       69 2023-07-01 09:47:05.000000 dynamic-service-1.3.0/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-07-08 10:41:46.851581 dynamic-service-1.3.0/setup.cfg
--rw-rw-rw-   0        0        0     1603 2023-07-08 10:41:40.000000 dynamic-service-1.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-08 12:13:04.272884 dynamic-service-1.3.1/
+-rw-rw-rw-   0        0        0      236 2023-07-08 12:13:02.000000 dynamic-service-1.3.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     2023 2023-07-08 12:13:04.271884 dynamic-service-1.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1226 2023-07-01 09:47:05.000000 dynamic-service-1.3.1/README.md
+-rw-rw-rw-   0        0        0    12920 2023-07-01 09:47:05.000000 dynamic-service-1.3.1/build.py
+drwxrwxrwx   0        0        0        0 2023-07-08 12:13:04.215885 dynamic-service-1.3.1/dynamic_service/
+-rw-rw-rw-   0        0        0     1439 2023-07-01 09:47:05.000000 dynamic-service-1.3.1/dynamic_service/base.py
+drwxrwxrwx   0        0        0        0 2023-07-08 12:13:04.257884 dynamic-service-1.3.1/dynamic_service/endpoints/
+-rw-rw-rw-   0        0        0      210 2023-07-01 09:47:05.000000 dynamic-service-1.3.1/dynamic_service/endpoints/__init__.py
+-rw-rw-rw-   0        0        0     2539 2023-07-03 14:24:04.000000 dynamic-service-1.3.1/dynamic_service/endpoints/data.py
+-rw-rw-rw-   0        0        0     9234 2023-07-03 14:30:46.000000 dynamic-service-1.3.1/dynamic_service/endpoints/engine.py
+-rw-rw-rw-   0        0        0     1569 2023-07-03 06:52:10.000000 dynamic-service-1.3.1/dynamic_service/endpoints/exceptions.py
+-rw-rw-rw-   0        0        0     1608 2023-07-03 06:51:55.000000 dynamic-service-1.3.1/dynamic_service/endpoints/process.py
+drwxrwxrwx   0        0        0        0 2023-07-08 12:13:04.265884 dynamic-service-1.3.1/dynamic_service/service/
+-rw-rw-rw-   0        0        0      106 2023-07-01 09:47:05.000000 dynamic-service-1.3.1/dynamic_service/service/__init__.py
+-rw-rw-rw-   0        0        0    20625 2023-07-08 12:06:30.000000 dynamic-service-1.3.1/dynamic_service/service/rest.py
+-rw-rw-rw-   0        0        0     3387 2023-07-08 10:41:33.000000 dynamic-service-1.3.1/dynamic_service/service/sockets.py
+drwxrwxrwx   0        0        0        0 2023-07-08 12:13:04.205808 dynamic-service-1.3.1/dynamic_service/source/
+drwxrwxrwx   0        0        0        0 2023-07-08 12:13:04.205808 dynamic-service-1.3.1/dynamic_service/source/assets/
+drwxrwxrwx   0        0        0        0 2023-07-08 12:13:04.270884 dynamic-service-1.3.1/dynamic_service/source/assets/icon/
+-rw-rw-rw-   0        0        0     2834 2023-07-01 09:47:05.000000 dynamic-service-1.3.1/dynamic_service/source/assets/icon/icon.ico
+-rw-rw-rw-   0        0        0    27619 2023-07-01 09:47:05.000000 dynamic-service-1.3.1/dynamic_service/source/assets/icon/icon.png
+drwxrwxrwx   0        0        0        0 2023-07-08 12:13:04.229884 dynamic-service-1.3.1/dynamic_service.egg-info/
+-rw-rw-rw-   0        0        0     2023 2023-07-08 12:13:04.000000 dynamic-service-1.3.1/dynamic_service.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      686 2023-07-08 12:13:04.000000 dynamic-service-1.3.1/dynamic_service.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-08 12:13:04.000000 dynamic-service-1.3.1/dynamic_service.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       83 2023-07-08 12:13:04.000000 dynamic-service-1.3.1/dynamic_service.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-07-08 12:13:04.000000 dynamic-service-1.3.1/dynamic_service.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      627 2023-07-08 12:13:02.000000 dynamic-service-1.3.1/pyproject.toml
+-rw-rw-rw-   0        0        0       85 2023-07-03 14:45:22.000000 dynamic-service-1.3.1/requirements-dev.txt
+-rw-rw-rw-   0        0        0       69 2023-07-01 09:47:05.000000 dynamic-service-1.3.1/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-07-08 12:13:04.272884 dynamic-service-1.3.1/setup.cfg
+-rw-rw-rw-   0        0        0     1603 2023-07-08 12:12:54.000000 dynamic-service-1.3.1/setup.py
```

### Comparing `dynamic-service-1.3.0/PKG-INFO` & `dynamic-service-1.3.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dynamic-service
-Version: 1.3.0
+Version: 1.3.1
 Summary: A framework for developing responsive, live and dynamic REST APIs with python.
 Home-page: https://github.com/Shahaf-F-S/dynamic-service
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `dynamic-service-1.3.0/README.md` & `dynamic-service-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `dynamic-service-1.3.0/build.py` & `dynamic-service-1.3.1/build.py`

 * *Files identical despite different names*

### Comparing `dynamic-service-1.3.0/dynamic_service/base.py` & `dynamic-service-1.3.1/dynamic_service/base.py`

 * *Files identical despite different names*

### Comparing `dynamic-service-1.3.0/dynamic_service/endpoints/data.py` & `dynamic-service-1.3.1/dynamic_service/endpoints/data.py`

 * *Files identical despite different names*

### Comparing `dynamic-service-1.3.0/dynamic_service/endpoints/engine.py` & `dynamic-service-1.3.1/dynamic_service/endpoints/engine.py`

 * *Files identical despite different names*

### Comparing `dynamic-service-1.3.0/dynamic_service/endpoints/exceptions.py` & `dynamic-service-1.3.1/dynamic_service/endpoints/exceptions.py`

 * *Files identical despite different names*

### Comparing `dynamic-service-1.3.0/dynamic_service/endpoints/process.py` & `dynamic-service-1.3.1/dynamic_service/endpoints/process.py`

 * *Files identical despite different names*

### Comparing `dynamic-service-1.3.0/dynamic_service/service/rest.py` & `dynamic-service-1.3.1/dynamic_service/service/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -77,14 +77,18 @@
     if isinstance(name, str):
         command.__name__ = name
     # end if
 
     return command
 # end override_signature
 
+class Endpoint(partial):
+    """A class to wrap around an endpoint object."""
+# end Endpoint
+
 class RESTService(ServiceInterface):
     """
     A class to represent a service object.
 
     The BaseService is the parent class of service class.
     The service class creates a service object to deploy
     functionality of endpoint objects as a REST API.
@@ -460,15 +464,15 @@
 
         for endpoint in self.endpoints.values():
             endpoint.set_root(self.root)
 
             path = ("/" + endpoint.root if endpoint.root else '') + endpoint.path
 
             command = override_signature(
-                partial(endpoint.__call__, endpoint),
+                Endpoint(endpoint.__call__, endpoint),
                 new=endpoint.endpoint, name=type(endpoint).__name__
             )
 
             try:
                 router.add_api_route(
                     path, command,
                     methods=endpoint.methods, description=endpoint.description,
```

### Comparing `dynamic-service-1.3.0/dynamic_service/service/sockets.py` & `dynamic-service-1.3.1/dynamic_service/service/sockets.py`

 * *Files identical despite different names*

### Comparing `dynamic-service-1.3.0/dynamic_service/source/assets/icon/icon.ico` & `dynamic-service-1.3.1/dynamic_service/source/assets/icon/icon.ico`

 * *Files identical despite different names*

### Comparing `dynamic-service-1.3.0/dynamic_service/source/assets/icon/icon.png` & `dynamic-service-1.3.1/dynamic_service/source/assets/icon/icon.png`

 * *Files identical despite different names*

### Comparing `dynamic-service-1.3.0/dynamic_service.egg-info/PKG-INFO` & `dynamic-service-1.3.1/dynamic_service.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dynamic-service
-Version: 1.3.0
+Version: 1.3.1
 Summary: A framework for developing responsive, live and dynamic REST APIs with python.
 Home-page: https://github.com/Shahaf-F-S/dynamic-service
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `dynamic-service-1.3.0/dynamic_service.egg-info/SOURCES.txt` & `dynamic-service-1.3.1/dynamic_service.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dynamic-service-1.3.0/pyproject.toml` & `dynamic-service-1.3.1/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = 'dynamic-service'
-version = '1.3.0'
+version = '1.3.1'
 description = 'A framework for developing responsive, live and dynamic REST APIs with python.'
 classifiers = [
 	'Intended Audience :: Developers',
 	'License :: OSI Approved :: MIT License',
 	'Programming Language :: Python',
 	'Programming Language :: Python :: 3',
 	'Programming Language :: Python :: 3.8',
```

### Comparing `dynamic-service-1.3.0/setup.py` & `dynamic-service-1.3.1/setup.py`

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
-        version='1.3.0',
+        version='1.3.1',
         description=(
             "A framework for developing responsive, "
             "live and dynamic REST APIs with python."
         ),
         license='MIT',
         author="Shahaf Frank-Shapir",
         author_email='shahaffrs@gmail.com',
```

