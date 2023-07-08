# Comparing `tmp/flask_cognito_lib-1.3.2.tar.gz` & `tmp/flask_cognito_lib-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flask_cognito_lib-1.3.2.tar", max compression
+gzip compressed data, was "flask_cognito_lib-1.4.0.tar", max compression
```

## Comparing `flask_cognito_lib-1.3.2.tar` & `flask_cognito_lib-1.4.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1072 2023-05-31 10:45:01.689647 flask_cognito_lib-1.3.2/LICENSE
--rw-r--r--   0        0        0     7676 2023-05-31 10:45:01.689647 flask_cognito_lib-1.3.2/README.md
--rw-r--r--   0        0        0     2278 2023-05-31 10:45:30.765581 flask_cognito_lib-1.3.2/pyproject.toml
--rw-r--r--   0        0        0       82 2023-05-31 10:45:30.737580 flask_cognito_lib-1.3.2/src/flask_cognito_lib/__init__.py
--rw-r--r--   0        0        0     4686 2023-05-31 10:45:01.693647 flask_cognito_lib-1.3.2/src/flask_cognito_lib/config.py
--rw-r--r--   0        0        0     6129 2023-05-31 10:45:01.693647 flask_cognito_lib-1.3.2/src/flask_cognito_lib/decorators.py
--rw-r--r--   0        0        0      384 2023-05-31 10:45:01.693647 flask_cognito_lib-1.3.2/src/flask_cognito_lib/exceptions.py
--rw-r--r--   0        0        0     6194 2023-05-31 10:45:01.693647 flask_cognito_lib-1.3.2/src/flask_cognito_lib/plugin.py
--rw-r--r--   0        0        0      326 2023-05-31 10:45:01.693647 flask_cognito_lib-1.3.2/src/flask_cognito_lib/services/__init__.py
--rw-r--r--   0        0        0     3510 2023-05-31 10:45:01.693647 flask_cognito_lib-1.3.2/src/flask_cognito_lib/services/cognito_svc.py
--rw-r--r--   0        0        0     5802 2023-05-31 10:45:01.693647 flask_cognito_lib-1.3.2/src/flask_cognito_lib/services/token_svc.py
--rw-r--r--   0        0        0     1124 2023-05-31 10:45:01.693647 flask_cognito_lib-1.3.2/src/flask_cognito_lib/utils.py
--rw-r--r--   0        0        0     9063 1970-01-01 00:00:00.000000 flask_cognito_lib-1.3.2/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-07-08 10:38:09.872064 flask_cognito_lib-1.4.0/LICENSE
+-rw-r--r--   0        0        0     7676 2023-07-08 10:38:09.872064 flask_cognito_lib-1.4.0/README.md
+-rw-r--r--   0        0        0     2278 2023-07-08 10:38:30.444045 flask_cognito_lib-1.4.0/pyproject.toml
+-rw-r--r--   0        0        0       82 2023-07-08 10:38:30.424045 flask_cognito_lib-1.4.0/src/flask_cognito_lib/__init__.py
+-rw-r--r--   0        0        0     4687 2023-07-08 10:38:09.872064 flask_cognito_lib-1.4.0/src/flask_cognito_lib/config.py
+-rw-r--r--   0        0        0     6129 2023-07-08 10:38:09.872064 flask_cognito_lib-1.4.0/src/flask_cognito_lib/decorators.py
+-rw-r--r--   0        0        0      384 2023-07-08 10:38:09.872064 flask_cognito_lib-1.4.0/src/flask_cognito_lib/exceptions.py
+-rw-r--r--   0        0        0     6194 2023-07-08 10:38:09.872064 flask_cognito_lib-1.4.0/src/flask_cognito_lib/plugin.py
+-rw-r--r--   0        0        0      326 2023-07-08 10:38:09.872064 flask_cognito_lib-1.4.0/src/flask_cognito_lib/services/__init__.py
+-rw-r--r--   0        0        0     3820 2023-07-08 10:38:09.872064 flask_cognito_lib-1.4.0/src/flask_cognito_lib/services/cognito_svc.py
+-rw-r--r--   0        0        0     5802 2023-07-08 10:38:09.872064 flask_cognito_lib-1.4.0/src/flask_cognito_lib/services/token_svc.py
+-rw-r--r--   0        0        0     1124 2023-07-08 10:38:09.872064 flask_cognito_lib-1.4.0/src/flask_cognito_lib/utils.py
+-rw-r--r--   0        0        0     9063 1970-01-01 00:00:00.000000 flask_cognito_lib-1.4.0/PKG-INFO
```

### Comparing `flask_cognito_lib-1.3.2/LICENSE` & `flask_cognito_lib-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `flask_cognito_lib-1.3.2/README.md` & `flask_cognito_lib-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `flask_cognito_lib-1.3.2/pyproject.toml` & `flask_cognito_lib-1.4.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "flask_cognito_lib"
-version = "1.3.2"
+version = "1.4.0"
 description = "A Flask extension that supports protecting routes with AWS Cognito following OAuth 2.1 best practices"
 license = "MIT"
 authors = ["mblackgeo <18327836+mblackgeo@users.noreply.github.com>"]
 readme = "README.md"
 homepage = "https://github.com/mblackgeo/flask-cognito-lib"
 repository = "https://github.com/mblackgeo/flask-cognito-lib"
 keywords = ["Flask", "Extension", "OAuth", "Cognito"]
```

### Comparing `flask_cognito_lib-1.3.2/src/flask_cognito_lib/config.py` & `flask_cognito_lib-1.4.0/src/flask_cognito_lib/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,15 +63,15 @@
     def user_pool_client_id(self) -> str:
         """Return the Cognito user pool client ID"""
         return get("AWS_COGNITO_USER_POOL_CLIENT_ID", required=True)
 
     @property
     def user_pool_client_secret(self) -> str:
         """Return the Cognito user pool client secret"""
-        return get("AWS_COGNITO_USER_POOL_CLIENT_SECRET", required=True)
+        return get("AWS_COGNITO_USER_POOL_CLIENT_SECRET", required=False)
 
     @property
     def redirect_url(self) -> str:
         """Return the Redirect URL (post-login)"""
         return get("AWS_COGNITO_REDIRECT_URL", required=True)
 
     @property
```

### Comparing `flask_cognito_lib-1.3.2/src/flask_cognito_lib/decorators.py` & `flask_cognito_lib-1.4.0/src/flask_cognito_lib/decorators.py`

 * *Files identical despite different names*

### Comparing `flask_cognito_lib-1.3.2/src/flask_cognito_lib/plugin.py` & `flask_cognito_lib-1.4.0/src/flask_cognito_lib/plugin.py`

 * *Files identical despite different names*

### Comparing `flask_cognito_lib-1.3.2/src/flask_cognito_lib/services/cognito_svc.py` & `flask_cognito_lib-1.4.0/src/flask_cognito_lib/services/cognito_svc.py`

 * *Files 10% similar despite different names*

```diff
@@ -92,19 +92,27 @@
             "grant_type": "authorization_code",
             "client_id": self.cfg.user_pool_client_id,
             "redirect_uri": self.cfg.redirect_url,
             "code": code,
             "code_verifier": code_verifier,
         }
 
+        # The Authorization header must not be present when using a
+        # Public Client, we assume this when the secret is blank.
+        # (Blank secrets are not supported on Confidential Clients)
+        if self.cfg.user_pool_client_secret:
+            auth = (self.cfg.user_pool_client_id, self.cfg.user_pool_client_secret)
+        else:
+            auth = None
+
         try:
             response = requests.post(
                 url=self.cfg.token_endpoint,
                 data=data,
-                auth=(self.cfg.user_pool_client_id, self.cfg.user_pool_client_secret),
+                auth=auth,
             )
             response_json = response.json()
 
         except requests.exceptions.RequestException as e:
             raise CognitoError(str(e)) from e
 
         if "error" in response_json:
```

### Comparing `flask_cognito_lib-1.3.2/src/flask_cognito_lib/services/token_svc.py` & `flask_cognito_lib-1.4.0/src/flask_cognito_lib/services/token_svc.py`

 * *Files identical despite different names*

### Comparing `flask_cognito_lib-1.3.2/src/flask_cognito_lib/utils.py` & `flask_cognito_lib-1.4.0/src/flask_cognito_lib/utils.py`

 * *Files identical despite different names*

### Comparing `flask_cognito_lib-1.3.2/PKG-INFO` & `flask_cognito_lib-1.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flask-cognito-lib
-Version: 1.3.2
+Version: 1.4.0
 Summary: A Flask extension that supports protecting routes with AWS Cognito following OAuth 2.1 best practices
 Home-page: https://github.com/mblackgeo/flask-cognito-lib
 License: MIT
 Keywords: Flask,Extension,OAuth,Cognito
 Author: mblackgeo
 Author-email: 18327836+mblackgeo@users.noreply.github.com
 Requires-Python: >=3.8,<4.0
```

