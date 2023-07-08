# Comparing `tmp/flask_cognito_lib-1.4.0.tar.gz` & `tmp/flask_cognito_lib-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flask_cognito_lib-1.4.0.tar", max compression
+gzip compressed data, was "flask_cognito_lib-1.4.1.tar", max compression
```

## Comparing `flask_cognito_lib-1.4.0.tar` & `flask_cognito_lib-1.4.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1072 2023-07-08 10:38:09.872064 flask_cognito_lib-1.4.0/LICENSE
--rw-r--r--   0        0        0     7676 2023-07-08 10:38:09.872064 flask_cognito_lib-1.4.0/README.md
--rw-r--r--   0        0        0     2278 2023-07-08 10:38:30.444045 flask_cognito_lib-1.4.0/pyproject.toml
--rw-r--r--   0        0        0       82 2023-07-08 10:38:30.424045 flask_cognito_lib-1.4.0/src/flask_cognito_lib/__init__.py
--rw-r--r--   0        0        0     4687 2023-07-08 10:38:09.872064 flask_cognito_lib-1.4.0/src/flask_cognito_lib/config.py
--rw-r--r--   0        0        0     6129 2023-07-08 10:38:09.872064 flask_cognito_lib-1.4.0/src/flask_cognito_lib/decorators.py
--rw-r--r--   0        0        0      384 2023-07-08 10:38:09.872064 flask_cognito_lib-1.4.0/src/flask_cognito_lib/exceptions.py
--rw-r--r--   0        0        0     6194 2023-07-08 10:38:09.872064 flask_cognito_lib-1.4.0/src/flask_cognito_lib/plugin.py
--rw-r--r--   0        0        0      326 2023-07-08 10:38:09.872064 flask_cognito_lib-1.4.0/src/flask_cognito_lib/services/__init__.py
--rw-r--r--   0        0        0     3820 2023-07-08 10:38:09.872064 flask_cognito_lib-1.4.0/src/flask_cognito_lib/services/cognito_svc.py
--rw-r--r--   0        0        0     5802 2023-07-08 10:38:09.872064 flask_cognito_lib-1.4.0/src/flask_cognito_lib/services/token_svc.py
--rw-r--r--   0        0        0     1124 2023-07-08 10:38:09.872064 flask_cognito_lib-1.4.0/src/flask_cognito_lib/utils.py
--rw-r--r--   0        0        0     9063 1970-01-01 00:00:00.000000 flask_cognito_lib-1.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-07-08 10:56:40.099217 flask_cognito_lib-1.4.1/LICENSE
+-rw-r--r--   0        0        0     7676 2023-07-08 10:56:40.099217 flask_cognito_lib-1.4.1/README.md
+-rw-r--r--   0        0        0     2278 2023-07-08 10:57:01.203231 flask_cognito_lib-1.4.1/pyproject.toml
+-rw-r--r--   0        0        0       82 2023-07-08 10:57:01.183231 flask_cognito_lib-1.4.1/src/flask_cognito_lib/__init__.py
+-rw-r--r--   0        0        0     4687 2023-07-08 10:56:40.099217 flask_cognito_lib-1.4.1/src/flask_cognito_lib/config.py
+-rw-r--r--   0        0        0     6129 2023-07-08 10:56:40.099217 flask_cognito_lib-1.4.1/src/flask_cognito_lib/decorators.py
+-rw-r--r--   0        0        0      384 2023-07-08 10:56:40.099217 flask_cognito_lib-1.4.1/src/flask_cognito_lib/exceptions.py
+-rw-r--r--   0        0        0     5995 2023-07-08 10:56:40.099217 flask_cognito_lib-1.4.1/src/flask_cognito_lib/plugin.py
+-rw-r--r--   0        0        0      326 2023-07-08 10:56:40.099217 flask_cognito_lib-1.4.1/src/flask_cognito_lib/services/__init__.py
+-rw-r--r--   0        0        0     3820 2023-07-08 10:56:40.099217 flask_cognito_lib-1.4.1/src/flask_cognito_lib/services/cognito_svc.py
+-rw-r--r--   0        0        0     5802 2023-07-08 10:56:40.099217 flask_cognito_lib-1.4.1/src/flask_cognito_lib/services/token_svc.py
+-rw-r--r--   0        0        0     1124 2023-07-08 10:56:40.099217 flask_cognito_lib-1.4.1/src/flask_cognito_lib/utils.py
+-rw-r--r--   0        0        0     9063 1970-01-01 00:00:00.000000 flask_cognito_lib-1.4.1/PKG-INFO
```

### Comparing `flask_cognito_lib-1.4.0/LICENSE` & `flask_cognito_lib-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `flask_cognito_lib-1.4.0/README.md` & `flask_cognito_lib-1.4.1/README.md`

 * *Files identical despite different names*

### Comparing `flask_cognito_lib-1.4.0/pyproject.toml` & `flask_cognito_lib-1.4.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "flask_cognito_lib"
-version = "1.4.0"
+version = "1.4.1"
 description = "A Flask extension that supports protecting routes with AWS Cognito following OAuth 2.1 best practices"
 license = "MIT"
 authors = ["mblackgeo <18327836+mblackgeo@users.noreply.github.com>"]
 readme = "README.md"
 homepage = "https://github.com/mblackgeo/flask-cognito-lib"
 repository = "https://github.com/mblackgeo/flask-cognito-lib"
 keywords = ["Flask", "Extension", "OAuth", "Cognito"]
```

### Comparing `flask_cognito_lib-1.4.0/src/flask_cognito_lib/config.py` & `flask_cognito_lib-1.4.1/src/flask_cognito_lib/config.py`

 * *Files identical despite different names*

### Comparing `flask_cognito_lib-1.4.0/src/flask_cognito_lib/decorators.py` & `flask_cognito_lib-1.4.1/src/flask_cognito_lib/decorators.py`

 * *Files identical despite different names*

### Comparing `flask_cognito_lib-1.4.0/src/flask_cognito_lib/plugin.py` & `flask_cognito_lib-1.4.1/src/flask_cognito_lib/plugin.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from typing import Any, Callable, Dict, Optional
 
-from flask import Flask
-from flask import _app_ctx_stack as ctx_stack
+from flask import Flask, g
 
 from flask_cognito_lib.config import Config
 from flask_cognito_lib.exceptions import CognitoError
 from flask_cognito_lib.services import cognito_service_factory, token_service_factory
 from flask_cognito_lib.services.cognito_svc import CognitoService
 from flask_cognito_lib.services.token_svc import TokenService
 from flask_cognito_lib.utils import CognitoTokenResponse
@@ -47,36 +46,32 @@
         """Instantiate an instance of the TokenService within the app context
 
         Returns
         -------
         TokenService
             An instance of TokenService
         """
-        ctx = ctx_stack.top
-        if ctx is not None:
-            if not hasattr(ctx, self.cfg.CONTEXT_KEY_TOKEN_SERVICE):
-                token_service = self.token_service_factory(cfg=self.cfg)
-                setattr(ctx, self.cfg.CONTEXT_KEY_TOKEN_SERVICE, token_service)
-            return getattr(ctx, self.cfg.CONTEXT_KEY_TOKEN_SERVICE)
+        if not hasattr(g, self.cfg.CONTEXT_KEY_TOKEN_SERVICE):
+            token_service = self.token_service_factory(cfg=self.cfg)
+            setattr(g, self.cfg.CONTEXT_KEY_TOKEN_SERVICE, token_service)
+        return getattr(g, self.cfg.CONTEXT_KEY_TOKEN_SERVICE)
 
     @property
     def cognito_service(self) -> CognitoService:
         """Instantiate an instance of the CognitoService within the app context
 
         Returns
         -------
         CognitoService
             An instance of CognitoService
         """
-        ctx = ctx_stack.top
-        if ctx is not None:
-            if not hasattr(ctx, self.cfg.CONTEXT_KEY_COGNITO_SERVICE):
-                cognito_service = self.cognito_service_factory(cfg=self.cfg)
-                setattr(ctx, self.cfg.CONTEXT_KEY_COGNITO_SERVICE, cognito_service)
-            return getattr(ctx, self.cfg.CONTEXT_KEY_COGNITO_SERVICE)
+        if not hasattr(g, self.cfg.CONTEXT_KEY_COGNITO_SERVICE):
+            cognito_service = self.cognito_service_factory(cfg=self.cfg)
+            setattr(g, self.cfg.CONTEXT_KEY_COGNITO_SERVICE, cognito_service)
+        return getattr(g, self.cfg.CONTEXT_KEY_COGNITO_SERVICE)
 
     def get_tokens(
         self,
         request_args: Dict[str, str],
         expected_state: str,
         code_verifier: str,
     ) -> CognitoTokenResponse:
```

### Comparing `flask_cognito_lib-1.4.0/src/flask_cognito_lib/services/cognito_svc.py` & `flask_cognito_lib-1.4.1/src/flask_cognito_lib/services/cognito_svc.py`

 * *Files identical despite different names*

### Comparing `flask_cognito_lib-1.4.0/src/flask_cognito_lib/services/token_svc.py` & `flask_cognito_lib-1.4.1/src/flask_cognito_lib/services/token_svc.py`

 * *Files identical despite different names*

### Comparing `flask_cognito_lib-1.4.0/src/flask_cognito_lib/utils.py` & `flask_cognito_lib-1.4.1/src/flask_cognito_lib/utils.py`

 * *Files identical despite different names*

### Comparing `flask_cognito_lib-1.4.0/PKG-INFO` & `flask_cognito_lib-1.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flask-cognito-lib
-Version: 1.4.0
+Version: 1.4.1
 Summary: A Flask extension that supports protecting routes with AWS Cognito following OAuth 2.1 best practices
 Home-page: https://github.com/mblackgeo/flask-cognito-lib
 License: MIT
 Keywords: Flask,Extension,OAuth,Cognito
 Author: mblackgeo
 Author-email: 18327836+mblackgeo@users.noreply.github.com
 Requires-Python: >=3.8,<4.0
```

