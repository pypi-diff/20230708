# Comparing `tmp/pydid-0.3.8.tar.gz` & `tmp/pydid-0.3.9a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydid-0.3.8.tar", max compression
+gzip compressed data, was "pydid-0.3.9a0.tar", max compression
```

## Comparing `pydid-0.3.8.tar` & `pydid-0.3.9a0.tar`

### file list

```diff
@@ -1,18 +1,17 @@
--rw-r--r--   0        0        0    11357 2023-06-01 15:20:49.282083 pydid-0.3.8/LICENSE
--rw-r--r--   0        0        0      848 2023-06-01 15:20:49.282083 pydid-0.3.8/README.md
--rw-r--r--   0        0        0     1680 2023-06-01 15:20:49.282083 pydid-0.3.8/pydid/__init__.py
--rw-r--r--   0        0        0      318 2023-06-01 15:20:49.282083 pydid-0.3.8/pydid/common.py
--rw-r--r--   0        0        0     2294 2023-06-01 15:20:49.282083 pydid-0.3.8/pydid/did.py
--rw-r--r--   0        0        0     2773 2023-06-01 15:20:49.282083 pydid-0.3.8/pydid/did_url.py
--rw-r--r--   0        0        0      560 2023-06-01 15:20:49.282083 pydid-0.3.8/pydid/doc/__init__.py
--rw-r--r--   0        0        0     8263 2023-06-01 15:20:49.282083 pydid-0.3.8/pydid/doc/builder.py
--rw-r--r--   0        0        0     1322 2023-06-01 15:20:49.282083 pydid-0.3.8/pydid/doc/corrections.py
--rw-r--r--   0        0        0     8247 2023-06-01 15:20:49.282083 pydid-0.3.8/pydid/doc/doc.py
--rw-r--r--   0        0        0     1807 2023-06-01 15:20:49.282083 pydid-0.3.8/pydid/doc/generic.py
--rw-r--r--   0        0        0     4647 2023-06-01 15:20:49.282083 pydid-0.3.8/pydid/resource.py
--rw-r--r--   0        0        0      912 2023-06-01 15:20:49.282083 pydid-0.3.8/pydid/service.py
--rw-r--r--   0        0        0     1002 2023-06-01 15:20:49.282083 pydid-0.3.8/pydid/validation.py
--rw-r--r--   0        0        0     8458 2023-06-01 15:20:49.282083 pydid-0.3.8/pydid/verification_method.py
--rw-r--r--   0        0        0     1089 2023-06-01 15:20:49.282083 pydid-0.3.8/pyproject.toml
--rw-r--r--   0        0        0     1661 2023-06-01 15:21:52.866118 pydid-0.3.8/setup.py
--rw-r--r--   0        0        0     1714 2023-06-01 15:21:52.866602 pydid-0.3.8/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-07-08 15:51:00.765497 pydid-0.3.9a0/LICENSE
+-rw-r--r--   0        0        0      848 2023-07-08 15:51:00.765497 pydid-0.3.9a0/README.md
+-rw-r--r--   0        0        0     1680 2023-07-08 15:51:00.765497 pydid-0.3.9a0/pydid/__init__.py
+-rw-r--r--   0        0        0      318 2023-07-08 15:51:00.765497 pydid-0.3.9a0/pydid/common.py
+-rw-r--r--   0        0        0     2294 2023-07-08 15:51:00.765497 pydid-0.3.9a0/pydid/did.py
+-rw-r--r--   0        0        0     2773 2023-07-08 15:51:00.765497 pydid-0.3.9a0/pydid/did_url.py
+-rw-r--r--   0        0        0      560 2023-07-08 15:51:00.765497 pydid-0.3.9a0/pydid/doc/__init__.py
+-rw-r--r--   0        0        0     8263 2023-07-08 15:51:00.765497 pydid-0.3.9a0/pydid/doc/builder.py
+-rw-r--r--   0        0        0     1322 2023-07-08 15:51:00.765497 pydid-0.3.9a0/pydid/doc/corrections.py
+-rw-r--r--   0        0        0     8287 2023-07-08 15:51:00.765497 pydid-0.3.9a0/pydid/doc/doc.py
+-rw-r--r--   0        0        0     1807 2023-07-08 15:51:00.765497 pydid-0.3.9a0/pydid/doc/generic.py
+-rw-r--r--   0        0        0     4647 2023-07-08 15:51:00.765497 pydid-0.3.9a0/pydid/resource.py
+-rw-r--r--   0        0        0     1463 2023-07-08 15:51:00.765497 pydid-0.3.9a0/pydid/service.py
+-rw-r--r--   0        0        0     1002 2023-07-08 15:51:00.765497 pydid-0.3.9a0/pydid/validation.py
+-rw-r--r--   0        0        0     8458 2023-07-08 15:51:00.765497 pydid-0.3.9a0/pydid/verification_method.py
+-rw-r--r--   0        0        0     1106 2023-07-08 15:51:00.765497 pydid-0.3.9a0/pyproject.toml
+-rw-r--r--   0        0        0     1767 1970-01-01 00:00:00.000000 pydid-0.3.9a0/PKG-INFO
```

### Comparing `pydid-0.3.8/LICENSE` & `pydid-0.3.9a0/LICENSE`

 * *Files identical despite different names*

### Comparing `pydid-0.3.8/README.md` & `pydid-0.3.9a0/README.md`

 * *Files identical despite different names*

### Comparing `pydid-0.3.8/pydid/__init__.py` & `pydid-0.3.9a0/pydid/__init__.py`

 * *Files identical despite different names*

### Comparing `pydid-0.3.8/pydid/did.py` & `pydid-0.3.9a0/pydid/did.py`

 * *Files identical despite different names*

### Comparing `pydid-0.3.8/pydid/did_url.py` & `pydid-0.3.9a0/pydid/did_url.py`

 * *Files identical despite different names*

### Comparing `pydid-0.3.8/pydid/doc/__init__.py` & `pydid-0.3.9a0/pydid/doc/__init__.py`

 * *Files identical despite different names*

### Comparing `pydid-0.3.8/pydid/doc/builder.py` & `pydid-0.3.9a0/pydid/doc/builder.py`

 * *Files identical despite different names*

### Comparing `pydid-0.3.8/pydid/doc/corrections.py` & `pydid-0.3.9a0/pydid/doc/corrections.py`

 * *Files identical despite different names*

### Comparing `pydid-0.3.8/pydid/doc/doc.py` & `pydid-0.3.9a0/pydid/doc/doc.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from pydantic import Field, root_validator, validator
 from typing_extensions import Annotated
 
 from ..did import DID, InvalidDIDError
 from ..did_url import DIDUrl, InvalidDIDUrlError
 from ..resource import IndexedResource, Resource
-from ..service import DIDCommService, Service, UnknownService
+from ..service import DIDCommV1Service, DIDCommV2Service, Service, UnknownService
 from ..verification_method import (
     KnownVerificationMethods,
     UnknownVerificationMethod,
     VerificationMethod,
 )
 
 
@@ -143,15 +143,15 @@
 
         if reference not in self._index:
             raise IDNotFoundError("ID {} not found in document".format(reference))
         return self._index[reference]
 
 
 PossibleMethodTypes = Union[KnownVerificationMethods, UnknownVerificationMethod]
-PossibleServiceTypes = Union[DIDCommService, UnknownService]
+PossibleServiceTypes = Union[DIDCommV1Service, DIDCommV2Service, UnknownService]
 
 
 class DIDDocument(BasicDIDDocument):
     """
     DID Document for DID Spec version 1.0.
 
     Registered verification method and service types are parsed into specific objects.
```

### Comparing `pydid-0.3.8/pydid/doc/generic.py` & `pydid-0.3.9a0/pydid/doc/generic.py`

 * *Files identical despite different names*

### Comparing `pydid-0.3.8/pydid/resource.py` & `pydid-0.3.9a0/pydid/resource.py`

 * *Files identical despite different names*

### Comparing `pydid-0.3.8/pydid/service.py` & `pydid-0.3.9a0/pydid/service.py`

 * *Files 21% similar despite different names*

```diff
@@ -19,24 +19,49 @@
     """Representation of DID Document Services."""
 
     id: DIDUrl
     type: str
     service_endpoint: Union[DIDUrl, AnyUrl, Literal[""], List[ServiceEndpoint]]
 
 
-class DIDCommService(Service):
+class DIDCommV1Service(Service):
     """DID Communication Service."""
 
     class Config:
         """DIDComm Service Config."""
 
         extra = Extra.forbid
 
-    type: Literal["IndyAgent", "did-communication"] = "did-communication"
+    type: Literal[
+        "IndyAgent", "did-communication", "DIDCommMessaging"
+    ] = "did-communication"
     recipient_keys: List[DIDUrl]
     routing_keys: List[DIDUrl] = []
     accept: Optional[List[str]] = None
     priority: int = 0
 
 
+DIDCommService = DIDCommV1Service
+
+
+class DIDCommV2ServiceEndpoint(ServiceEndpoint):
+    """DID Communication Service Endpoint."""
+
+    uri: Union[DIDUrl, AnyUrl]
+    accept: Optional[List[str]] = None
+    routing_keys: List[DIDUrl] = []
+
+
+class DIDCommV2Service(Service):
+    """DID Communication V2 Service."""
+
+    class Config:
+        """DIDComm Service Config."""
+
+        extra = Extra.forbid
+
+    type: Literal["DIDCommMessaging"] = "DIDCommMessaging"
+    service_endpoint: List[DIDCommV2ServiceEndpoint]
+
+
 class UnknownService(Service):
     """Unknown Service."""
```

### Comparing `pydid-0.3.8/pydid/validation.py` & `pydid-0.3.9a0/pydid/validation.py`

 * *Files identical despite different names*

### Comparing `pydid-0.3.8/pydid/verification_method.py` & `pydid-0.3.9a0/pydid/verification_method.py`

 * *Files identical despite different names*

### Comparing `pydid-0.3.8/pyproject.toml` & `pydid-0.3.9a0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pydid"
-version = "0.3.8"
+version = "0.3.9a0"
 description = "Python library for validating, constructing, and representing DIDs and DID Documents"
 authors = ["Daniel Bluhm <dbluhm@pm.me>"]
 license = "Apache 2.0"
 readme = "README.md"
 homepage = "https://github.com/Indicio-tech/pydid"
 repository = "https://github.com/Indicio-tech/pydid"
 keywords = [
@@ -39,7 +39,9 @@
 [tool.coverage.report]
 exclude_lines = [
     "pragma: no cover",
     "@abstract"
 ]
 precision = 2
 show_missing = true
+
+[tool.flake8]
```

### Comparing `pydid-0.3.8/PKG-INFO` & `pydid-0.3.9a0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: pydid
-Version: 0.3.8
+Version: 0.3.9a0
 Summary: Python library for validating, constructing, and representing DIDs and DID Documents
 Home-page: https://github.com/Indicio-tech/pydid
 License: Apache 2.0
 Keywords: decentralized,identity,ssi
 Author: Daniel Bluhm
 Author-email: dbluhm@pm.me
 Requires-Python: >=3.6.9,<4.0.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: inflection (>=0.5.1,<0.6.0)
 Requires-Dist: pydantic (>=1.8.1,<2.0.0)
 Requires-Dist: typing-extensions (>=4.0.0,<4.1.0)
 Project-URL: Repository, https://github.com/Indicio-tech/pydid
 Description-Content-Type: text/markdown
 
 # PyDID
```

