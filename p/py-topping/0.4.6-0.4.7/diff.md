# Comparing `tmp/py_topping-0.4.6.tar.gz` & `tmp/py_topping-0.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_topping-0.4.6.tar", last modified: Fri Jan 27 15:07:23 2023, max compression
+gzip compressed data, was "py_topping-0.4.7.tar", last modified: Sat Jul  8 16:15:11 2023, max compression
```

## Comparing `py_topping-0.4.6.tar` & `py_topping-0.4.7.tar`

### file list

```diff
@@ -1,45 +1,46 @@
-drwxrwxrwx   0        0        0        0 2023-01-27 15:07:23.450947 py_topping-0.4.6/
--rw-rw-rw-   0        0        0     1076 2021-11-25 06:55:31.000000 py_topping-0.4.6/LICENSE.txt
--rw-rw-rw-   0        0        0     4223 2023-01-27 15:07:23.450947 py_topping-0.4.6/PKG-INFO
--rw-rw-rw-   0        0        0     3577 2022-09-02 02:49:43.000000 py_topping-0.4.6/README.md
-drwxrwxrwx   0        0        0        0 2023-01-27 15:07:23.105565 py_topping-0.4.6/py_topping/
--rw-rw-rw-   0        0        0      640 2021-06-02 08:22:22.000000 py_topping-0.4.6/py_topping/__init__.py
-drwxrwxrwx   0        0        0        0 2023-01-27 15:07:23.353750 py_topping-0.4.6/py_topping/data_connection/
--rw-rw-rw-   0        0        0        0 2020-11-26 08:36:46.000000 py_topping-0.4.6/py_topping/data_connection/__init__.py
--rw-rw-rw-   0        0        0    45119 2023-01-27 14:49:51.000000 py_topping-0.4.6/py_topping/data_connection/database.py
--rw-rw-rw-   0        0        0     3911 2020-11-26 08:35:01.000000 py_topping-0.4.6/py_topping/data_connection/database_old.py
--rw-rw-rw-   0        0        0    10134 2022-04-21 03:07:27.000000 py_topping-0.4.6/py_topping/data_connection/gcp.py
--rw-rw-rw-   0        0        0     1900 2022-10-19 11:02:11.000000 py_topping-0.4.6/py_topping/data_connection/opc.py
--rw-rw-rw-   0        0        0     1708 2022-04-05 04:46:19.000000 py_topping-0.4.6/py_topping/data_connection/sftp.py
--rw-rw-rw-   0        0        0    11954 2022-08-12 07:09:35.000000 py_topping-0.4.6/py_topping/data_connection/sharepoint.py
--rw-rw-rw-   0        0        0     6229 2020-11-27 03:16:36.000000 py_topping-0.4.6/py_topping/data_connection/sharepoint_old.py
--rw-rw-rw-   0        0        0     1170 2022-08-30 07:34:15.000000 py_topping-0.4.6/py_topping/data_connection/socket.py
-drwxrwxrwx   0        0        0        0 2023-01-27 15:07:23.391098 py_topping-0.4.6/py_topping/data_preparation/
--rw-rw-rw-   0        0        0     5985 2021-08-11 06:59:56.000000 py_topping-0.4.6/py_topping/data_preparation/__init__.py
--rw-rw-rw-   0        0        0     3916 2021-04-10 07:34:40.000000 py_topping-0.4.6/py_topping/data_preparation/lazy_ml.py
-drwxrwxrwx   0        0        0        0 2023-01-27 15:07:23.394099 py_topping-0.4.6/py_topping/general_use/
--rw-rw-rw-   0        0        0     7979 2023-01-24 08:47:57.000000 py_topping-0.4.6/py_topping/general_use/__init__.py
-drwxrwxrwx   0        0        0        0 2023-01-27 15:07:23.396089 py_topping-0.4.6/py_topping/image_processing/
--rw-rw-rw-   0        0        0     2913 2022-05-19 08:55:29.000000 py_topping-0.4.6/py_topping/image_processing/__init__.py
-drwxrwxrwx   0        0        0        0 2023-01-27 15:07:23.399090 py_topping-0.4.6/py_topping/run_pipeline/
--rw-rw-rw-   0        0        0     5371 2023-01-24 08:54:08.000000 py_topping-0.4.6/py_topping/run_pipeline/__init__.py
--rw-rw-rw-   0        0        0     6795 2023-01-24 09:17:24.000000 py_topping-0.4.6/py_topping/run_pipeline/api.py
-drwxrwxrwx   0        0        0        0 2023-01-27 15:07:23.111565 py_topping-0.4.6/py_topping.egg-info/
--rw-rw-rw-   0        0        0     4223 2023-01-27 15:07:22.000000 py_topping-0.4.6/py_topping.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1014 2023-01-27 15:07:22.000000 py_topping-0.4.6/py_topping.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-27 15:07:22.000000 py_topping-0.4.6/py_topping.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-01-27 15:07:22.000000 py_topping-0.4.6/py_topping.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-01-27 15:07:23.448940 py_topping-0.4.6/samples/
--rw-rw-rw-   0        0        0    33588 2021-12-22 03:13:06.000000 py_topping-0.4.6/samples/data_preparation.ipynb
--rw-rw-rw-   0        0        0    82591 2022-04-17 10:42:38.000000 py_topping-0.4.6/samples/database.ipynb
--rw-rw-rw-   0        0        0     3692 2022-08-12 07:04:16.000000 py_topping-0.4.6/samples/email_sender.ipynb
--rw-rw-rw-   0        0        0     7821 2023-01-27 15:05:21.000000 py_topping-0.4.6/samples/gcp.ipynb
--rw-rw-rw-   0        0        0     5778 2022-01-05 03:57:39.000000 py_topping-0.4.6/samples/lazy_LINE.ipynb
--rw-rw-rw-   0        0        0   142957 2022-06-03 01:41:50.000000 py_topping-0.4.6/samples/lazy_ml.ipynb
--rw-rw-rw-   0        0        0     7260 2022-04-19 04:31:14.000000 py_topping-0.4.6/samples/other_function.ipynb
--rw-rw-rw-   0        0        0    23047 2021-12-22 02:55:23.000000 py_topping-0.4.6/samples/run_pipeline.ipynb
--rw-rw-rw-   0        0        0    13932 2022-01-10 10:00:04.000000 py_topping-0.4.6/samples/sharepoint.ipynb
--rw-rw-rw-   0        0        0       86 2023-01-27 15:07:23.451954 py_topping-0.4.6/setup.cfg
--rw-rw-rw-   0        0        0     1112 2023-01-27 15:06:02.000000 py_topping-0.4.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-01-27 15:07:23.449948 py_topping-0.4.6/tests/
--rw-rw-rw-   0        0        0   281573 2023-01-27 15:04:06.000000 py_topping-0.4.6/tests/database.ipynb
+drwxrwxrwx   0        0        0        0 2023-07-08 16:15:11.846271 py_topping-0.4.7/
+-rw-rw-rw-   0        0        0     1076 2021-11-25 06:55:31.000000 py_topping-0.4.7/LICENSE.txt
+-rw-rw-rw-   0        0        0     4223 2023-07-08 16:15:11.846271 py_topping-0.4.7/PKG-INFO
+-rw-rw-rw-   0        0        0     3577 2022-09-02 02:49:43.000000 py_topping-0.4.7/README.md
+drwxrwxrwx   0        0        0        0 2023-07-08 16:15:11.815123 py_topping-0.4.7/py_topping/
+-rw-rw-rw-   0        0        0      640 2021-06-02 08:22:22.000000 py_topping-0.4.7/py_topping/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-08 16:15:11.825634 py_topping-0.4.7/py_topping/data_connection/
+-rw-rw-rw-   0        0        0        0 2020-11-26 08:36:46.000000 py_topping-0.4.7/py_topping/data_connection/__init__.py
+-rw-rw-rw-   0        0        0    45119 2023-01-27 14:49:51.000000 py_topping-0.4.7/py_topping/data_connection/database.py
+-rw-rw-rw-   0        0        0     3911 2020-11-26 08:35:01.000000 py_topping-0.4.7/py_topping/data_connection/database_old.py
+-rw-rw-rw-   0        0        0    10134 2022-04-21 03:07:27.000000 py_topping-0.4.7/py_topping/data_connection/gcp.py
+-rw-rw-rw-   0        0        0     1900 2022-10-19 11:02:11.000000 py_topping-0.4.7/py_topping/data_connection/opc.py
+-rw-rw-rw-   0        0        0     1708 2022-04-05 04:46:19.000000 py_topping-0.4.7/py_topping/data_connection/sftp.py
+-rw-rw-rw-   0        0        0    11954 2022-08-12 07:09:35.000000 py_topping-0.4.7/py_topping/data_connection/sharepoint.py
+-rw-rw-rw-   0        0        0     6229 2020-11-27 03:16:36.000000 py_topping-0.4.7/py_topping/data_connection/sharepoint_old.py
+-rw-rw-rw-   0        0        0     1170 2022-08-30 07:34:15.000000 py_topping-0.4.7/py_topping/data_connection/socket.py
+drwxrwxrwx   0        0        0        0 2023-07-08 16:15:11.826648 py_topping-0.4.7/py_topping/data_preparation/
+-rw-rw-rw-   0        0        0     5985 2021-08-11 06:59:56.000000 py_topping-0.4.7/py_topping/data_preparation/__init__.py
+-rw-rw-rw-   0        0        0     3916 2021-04-10 07:34:40.000000 py_topping-0.4.7/py_topping/data_preparation/lazy_ml.py
+drwxrwxrwx   0        0        0        0 2023-07-08 16:15:11.827648 py_topping-0.4.7/py_topping/general_use/
+-rw-rw-rw-   0        0        0     7979 2023-01-24 08:47:57.000000 py_topping-0.4.7/py_topping/general_use/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-08 16:15:11.828647 py_topping-0.4.7/py_topping/image_processing/
+-rw-rw-rw-   0        0        0     2913 2022-05-19 08:55:29.000000 py_topping-0.4.7/py_topping/image_processing/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-08 16:15:11.831648 py_topping-0.4.7/py_topping/run_pipeline/
+-rw-rw-rw-   0        0        0     5371 2023-01-24 08:54:08.000000 py_topping-0.4.7/py_topping/run_pipeline/__init__.py
+-rw-rw-rw-   0        0        0    10542 2023-07-08 15:58:33.000000 py_topping-0.4.7/py_topping/run_pipeline/api.py
+-rw-rw-rw-   0        0        0     9345 2023-07-08 16:07:00.000000 py_topping-0.4.7/py_topping/run_pipeline/test.py
+drwxrwxrwx   0        0        0        0 2023-07-08 16:15:11.818122 py_topping-0.4.7/py_topping.egg-info/
+-rw-rw-rw-   0        0        0     4223 2023-07-08 16:15:11.000000 py_topping-0.4.7/py_topping.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1046 2023-07-08 16:15:11.000000 py_topping-0.4.7/py_topping.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-08 16:15:11.000000 py_topping-0.4.7/py_topping.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-07-08 16:15:11.000000 py_topping-0.4.7/py_topping.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-08 16:15:11.843176 py_topping-0.4.7/samples/
+-rw-rw-rw-   0        0        0    33588 2021-12-22 03:13:06.000000 py_topping-0.4.7/samples/data_preparation.ipynb
+-rw-rw-rw-   0        0        0    82591 2022-04-17 10:42:38.000000 py_topping-0.4.7/samples/database.ipynb
+-rw-rw-rw-   0        0        0     3692 2022-08-12 07:04:16.000000 py_topping-0.4.7/samples/email_sender.ipynb
+-rw-rw-rw-   0        0        0     7821 2023-01-27 15:05:21.000000 py_topping-0.4.7/samples/gcp.ipynb
+-rw-rw-rw-   0        0        0     5778 2022-01-05 03:57:39.000000 py_topping-0.4.7/samples/lazy_LINE.ipynb
+-rw-rw-rw-   0        0        0   142957 2022-06-03 01:41:50.000000 py_topping-0.4.7/samples/lazy_ml.ipynb
+-rw-rw-rw-   0        0        0     7260 2022-04-19 04:31:14.000000 py_topping-0.4.7/samples/other_function.ipynb
+-rw-rw-rw-   0        0        0    23047 2021-12-22 02:55:23.000000 py_topping-0.4.7/samples/run_pipeline.ipynb
+-rw-rw-rw-   0        0        0    13932 2022-01-10 10:00:04.000000 py_topping-0.4.7/samples/sharepoint.ipynb
+-rw-rw-rw-   0        0        0       86 2023-07-08 16:15:11.846732 py_topping-0.4.7/setup.cfg
+-rw-rw-rw-   0        0        0     1112 2023-07-08 16:08:13.000000 py_topping-0.4.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-08 16:15:11.843176 py_topping-0.4.7/tests/
+-rw-rw-rw-   0        0        0   281573 2023-01-27 15:04:06.000000 py_topping-0.4.7/tests/database.ipynb
```

### Comparing `py_topping-0.4.6/LICENSE.txt` & `py_topping-0.4.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `py_topping-0.4.6/PKG-INFO` & `py_topping-0.4.7/py_topping.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
-Name: py_topping
-Version: 0.4.6
+Name: py-topping
+Version: 0.4.7
 Summary: simplify functions from other libraries functions in 1-2 lines
 Home-page: https://github.com/chanon-kr/Shared_Function
 Author: Chanon Krittapholchai
 Author-email: chanon.krittapholchai@gmail.com
 License: MIT
-Download-URL: https://github.com/chanon-kr/Shared_Function/archive/v0.4.6.tar.gz
+Download-URL: https://github.com/chanon-kr/Shared_Function/archive/v0.4.7.tar.gz
 Keywords: utility,ETL
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `py_topping-0.4.6/README.md` & `py_topping-0.4.7/README.md`

 * *Files identical despite different names*

### Comparing `py_topping-0.4.6/py_topping/__init__.py` & `py_topping-0.4.7/py_topping/__init__.py`

 * *Files identical despite different names*

### Comparing `py_topping-0.4.6/py_topping/data_connection/database.py` & `py_topping-0.4.7/py_topping/data_connection/database.py`

 * *Files identical despite different names*

### Comparing `py_topping-0.4.6/py_topping/data_connection/database_old.py` & `py_topping-0.4.7/py_topping/data_connection/database_old.py`

 * *Files identical despite different names*

### Comparing `py_topping-0.4.6/py_topping/data_connection/gcp.py` & `py_topping-0.4.7/py_topping/data_connection/gcp.py`

 * *Files identical despite different names*

### Comparing `py_topping-0.4.6/py_topping/data_connection/opc.py` & `py_topping-0.4.7/py_topping/data_connection/opc.py`

 * *Files identical despite different names*

### Comparing `py_topping-0.4.6/py_topping/data_connection/sftp.py` & `py_topping-0.4.7/py_topping/data_connection/sftp.py`

 * *Files identical despite different names*

### Comparing `py_topping-0.4.6/py_topping/data_connection/sharepoint.py` & `py_topping-0.4.7/py_topping/data_connection/sharepoint.py`

 * *Files identical despite different names*

### Comparing `py_topping-0.4.6/py_topping/data_connection/sharepoint_old.py` & `py_topping-0.4.7/py_topping/data_connection/sharepoint_old.py`

 * *Files identical despite different names*

### Comparing `py_topping-0.4.6/py_topping/data_connection/socket.py` & `py_topping-0.4.7/py_topping/data_connection/socket.py`

 * *Files identical despite different names*

### Comparing `py_topping-0.4.6/py_topping/data_preparation/__init__.py` & `py_topping-0.4.7/py_topping/data_preparation/__init__.py`

 * *Files identical despite different names*

### Comparing `py_topping-0.4.6/py_topping/data_preparation/lazy_ml.py` & `py_topping-0.4.7/py_topping/data_preparation/lazy_ml.py`

 * *Files identical despite different names*

### Comparing `py_topping-0.4.6/py_topping/general_use/__init__.py` & `py_topping-0.4.7/py_topping/general_use/__init__.py`

 * *Files identical despite different names*

### Comparing `py_topping-0.4.6/py_topping/image_processing/__init__.py` & `py_topping-0.4.7/py_topping/image_processing/__init__.py`

 * *Files identical despite different names*

### Comparing `py_topping-0.4.6/py_topping/run_pipeline/__init__.py` & `py_topping-0.4.7/py_topping/run_pipeline/__init__.py`

 * *Files identical despite different names*

### Comparing `py_topping-0.4.6/py_topping/run_pipeline/api.py` & `py_topping-0.4.7/py_topping/run_pipeline/test.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,94 +1,133 @@
 ## FastAPI Core
 from fastapi import FastAPI, Body, Request
 from fastapi.responses import JSONResponse
 import os, traceback, uvicorn
 ## Security Basic Auth
 import secrets, base64
 from fastapi import Depends, FastAPI, HTTPException, status
-from fastapi.security import HTTPBasic, HTTPBasicCredentials
+from fastapi.security import HTTPBasic, HTTPBasicCredentials, HTTPBearer, HTTPAuthorizationCredentials
 ## Add Doc Security
 from fastapi.openapi.docs import get_redoc_html, get_swagger_ui_html
 from fastapi.openapi.utils import get_openapi
-# Get Query Parameter
-# from pydantic import create_model
 
 class lazy_API :
     def __init__(self, title, version, description
                      , username = 'user'
                      , password = 'password'
+                     , authen_type = 'basic' ####
+                     , validate_token = None ####
                      , api_weak_authen = False
                      , callback = None
+                     , document = True
                 ) :
         """lazy_API class, to create FastAPI with a few lines of code"""
         ## Create Fast API
         self.app = FastAPI(   title= title
                             , version= version
                             , description= description
                             , docs_url=None
                             , redoc_url=None
-                            , openapi_url = None)     
+                            , openapi_url = None)
+        ## INIT authen method ####
+        assert authen_type in ['basic', 'token', None], "authen_type must be 'basic', 'token' or None"
+        self.authen_type = authen_type ####
         ## Initial Basic Auth
         self.storage = [base64.b64encode(username.encode('ascii')),
                         base64.b64encode(password.encode('ascii'))]
+        ## Initial Bearer Token
+        if authen_type == 'token' :
+            assert callable(validate_token) | (type(validate_token) == str), "When using authen_type 'token', validate_token must be a function or string"
+        if callable(validate_token) : self.validate_token = validate_token
+        else : 
+            self.storage_token = base64.b64encode(validate_token.encode('ascii'))
+            self.validate_token = lambda x : x == base64.b64decode(self.storage_token).decode('ascii')
+        ## Other Parameter
         self.api_weak_authen = api_weak_authen
-        ## Add Default Callback
         self.callback = callback
+        self.document = document
 
     ## Basic Authen
     def basic_authen_check(self, credentials: HTTPBasicCredentials = Depends(HTTPBasic())):
         """Basic Authentication"""
         correct_username = secrets.compare_digest(credentials.username, base64.b64decode(self.storage[0]).decode('ascii'))
         correct_password = secrets.compare_digest(credentials.password, base64.b64decode(self.storage[1]).decode('ascii'))
         if (correct_username and correct_password): return credentials.username
         raise HTTPException(status_code=status.HTTP_401_UNAUTHORIZED,
                 detail="Incorrect email or password",
                 headers={"WWW-Authenticate": "Basic"},)
+    
+    ## Bearer Token Authen ####
+    def token_authen_check(self, auth: HTTPAuthorizationCredentials = Depends(HTTPBearer())):
+        if not auth or auth.scheme != "Bearer":
+            raise HTTPException(status_code=401, detail="Invalid authentication credentials")
+        token = auth.credentials
+        # Perform token validation logic here
+        if self.validate_token(token): return token
+        raise HTTPException(status_code=401, detail="Invalid token", headers={"WWW-Authenticate": "Bearer Token"})
+
     ## For API
     def weak_authen_check(self, input_dict):
         """
         Sub Authentication for API in order to use with GCP Authentication
         , only use this function when 'api_weak_authen' is True
         """
-        correct_username = input_dict.get('username','') == base64.b64decode(self.storage[0]).decode('ascii')
-        correct_password = input_dict.get('password','') == base64.b64decode(self.storage[1]).decode('ascii')
-        if (correct_username and correct_password): return 'ok'
-        raise HTTPException(status_code=status.HTTP_401_UNAUTHORIZED,
-                detail="Incorrect email or password",
-                headers={"WWW-Authenticate": "Basic"},)
+        if self.authen_type == None : return 'ok'
+        elif self.authen_type == 'basic' :
+            correct_username = input_dict.get('username','') == base64.b64decode(self.storage[0]).decode('ascii')
+            correct_password = input_dict.get('password','') == base64.b64decode(self.storage[1]).decode('ascii')
+            if (correct_username and correct_password): return 'ok'
+            raise HTTPException(status_code=status.HTTP_401_UNAUTHORIZED,
+                    detail="Incorrect email or password",
+                    headers={"WWW-Authenticate": "Basic"},)
+        elif self.authen_type == 'token' :
+            if self.validate_token(input_dict.get('token','')) : return 'ok'
+            raise HTTPException(status_code=status.HTTP_401_UNAUTHORIZED,
+                    detail="Invalid token",
+                    headers={"WWW-Authenticate": "Bearer Token"},)
 
     def get_weak_authen_check(self, request: Request) :
         params = request.query_params
         self.weak_authen_check(params)
 
     def post_weak_authen_check(self, payload: dict):
         self.weak_authen_check(payload)
 
+    #### Added here
+    def select_authen_type(self, weak_method) :
+        if self.api_weak_authen | (self.authen_type == None) :
+            return weak_method
+        elif self.authen_type == 'basic' :
+            return self.basic_authen_check
+        elif self.authen_type == 'token' :
+            return self.token_authen_check
+
     def gen_doc(self) :           
         """Create Auth Doc"""
         @self.app.get("/openapi.json", include_in_schema=False)
         async def openapi(username: str = Depends(self.basic_authen_check)):
-            return get_openapi(title=self.app.title, version=self.app.version, routes=self.app.routes)
+            return get_openapi(title=self.app.title, version=self.app.version, description= self.app.description, routes=self.app.routes)
         @self.app.route('/')
         @self.app.get("/docs", include_in_schema=False)
         async def get_swagger_documentation(username: str = Depends(self.basic_authen_check)):
             return get_swagger_ui_html(openapi_url="/openapi.json", title="docs")
         @self.app.get("/redoc", include_in_schema=False)
         async def get_redoc_documentation(username: str = Depends(self.basic_authen_check)):
             return get_redoc_html(openapi_url="/openapi.json", title="docs")
 
     def create_post(self, function, name, tags = [], example = {}, callback = 'default') :
         """Create POST Method for FastAPI"""
         # Assign Default Callback
         if (type(callback) == str) : 
             if callback == 'default' : callback = self.callback
+        # Assign Authen ####
+        authen_selected = self.select_authen_type(self.post_weak_authen_check)
         @self.app.post(f'/{name}' , tags = tags)
         async def post_function(  payload : dict = Body(... , example = example)
-                                , username : str = Depends( self.post_weak_authen_check if self.api_weak_authen 
-                                                            else self.basic_authen_check)
+                                , username : str = Depends(authen_selected)
                                 ) :
             try :
                 return function(payload)
             except Exception as e :
                 print(traceback.format_exc())
                 if callback == None : 
                     return_error = {"error": str(traceback.format_exc())}
@@ -101,21 +140,22 @@
 
 
     def create_get(self, function, name, tags = [], example = {}, callback = 'default') :
         """Create GET Method for FastAPI"""
         # Assign Default Callback
         if (type(callback) == str) : 
             if callback == 'default' : callback = self.callback
+        # Assign Authen ####
+        authen_selected = self.select_authen_type(self.get_weak_authen_check)
         # query_model = create_model("Query", **query_params)
         @self.app.get(f'/{name}' , tags = tags)
         async def get_function(  
                                 # params: query_model = Depends()
                                 request: Request
-                                , username : str = Depends( self.get_weak_authen_check if self.api_weak_authen 
-                                                            else self.basic_authen_check)
+                                , username : str = Depends( authen_selected)
                                 ) :
             try :
                 params = request.query_params
                 return function(params)
             except Exception as e :
                 print(traceback.format_exc())
                 if callback == None : 
@@ -125,9 +165,20 @@
                                             , 'exception' : e 
                                             , 'input' : request.query_params})
                 return JSONResponse(status_code=500
                                     , content=return_error)
             
     def run(self, port = 8080, host = "0.0.0.0") :
         """To run FastAPI"""
-        self.gen_doc()
+        if self.document : self.gen_doc()
         uvicorn.run(self.app, port=int(os.environ.get("PORT", port)), host = host)
+
+def validate_token(token) :
+    if token == 'ebqaeorgb' : return True
+    else : return False
+
+validate_token = 'ebqaeorgb'
+
+a = lazy_API('a', 1, 'test', authen_type= 'token', api_weak_authen= False, validate_token= validate_token)
+a.create_post(lambda x : str(x), name= 't1', example= {'a' : 1})
+a.create_get(lambda x : str(x), name= 't2', example= {'a' : 1})
+a.run(port= 8082)
```

### Comparing `py_topping-0.4.6/py_topping.egg-info/PKG-INFO` & `py_topping-0.4.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
-Name: py-topping
-Version: 0.4.6
+Name: py_topping
+Version: 0.4.7
 Summary: simplify functions from other libraries functions in 1-2 lines
 Home-page: https://github.com/chanon-kr/Shared_Function
 Author: Chanon Krittapholchai
 Author-email: chanon.krittapholchai@gmail.com
 License: MIT
-Download-URL: https://github.com/chanon-kr/Shared_Function/archive/v0.4.6.tar.gz
+Download-URL: https://github.com/chanon-kr/Shared_Function/archive/v0.4.7.tar.gz
 Keywords: utility,ETL
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `py_topping-0.4.6/py_topping.egg-info/SOURCES.txt` & `py_topping-0.4.7/py_topping.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 py_topping/data_connection/socket.py
 py_topping/data_preparation/__init__.py
 py_topping/data_preparation/lazy_ml.py
 py_topping/general_use/__init__.py
 py_topping/image_processing/__init__.py
 py_topping/run_pipeline/__init__.py
 py_topping/run_pipeline/api.py
+py_topping/run_pipeline/test.py
 samples/data_preparation.ipynb
 samples/database.ipynb
 samples/email_sender.ipynb
 samples/gcp.ipynb
 samples/lazy_LINE.ipynb
 samples/lazy_ml.ipynb
 samples/other_function.ipynb
```

### Comparing `py_topping-0.4.6/samples/data_preparation.ipynb` & `py_topping-0.4.7/samples/data_preparation.ipynb`

 * *Files identical despite different names*

### Comparing `py_topping-0.4.6/samples/database.ipynb` & `py_topping-0.4.7/samples/database.ipynb`

 * *Files identical despite different names*

### Comparing `py_topping-0.4.6/samples/email_sender.ipynb` & `py_topping-0.4.7/samples/email_sender.ipynb`

 * *Files identical despite different names*

### Comparing `py_topping-0.4.6/samples/gcp.ipynb` & `py_topping-0.4.7/samples/gcp.ipynb`

 * *Files identical despite different names*

### Comparing `py_topping-0.4.6/samples/lazy_LINE.ipynb` & `py_topping-0.4.7/samples/lazy_LINE.ipynb`

 * *Files identical despite different names*

### Comparing `py_topping-0.4.6/samples/lazy_ml.ipynb` & `py_topping-0.4.7/samples/lazy_ml.ipynb`

 * *Files identical despite different names*

### Comparing `py_topping-0.4.6/samples/other_function.ipynb` & `py_topping-0.4.7/samples/other_function.ipynb`

 * *Files identical despite different names*

### Comparing `py_topping-0.4.6/samples/run_pipeline.ipynb` & `py_topping-0.4.7/samples/run_pipeline.ipynb`

 * *Files identical despite different names*

### Comparing `py_topping-0.4.6/samples/sharepoint.ipynb` & `py_topping-0.4.7/samples/sharepoint.ipynb`

 * *Files identical despite different names*

### Comparing `py_topping-0.4.6/setup.py` & `py_topping-0.4.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,23 +8,23 @@
 #                "Office365-REST-Python-Client"
 #                ,"SQLAlchemy"
 #                ,"pandas >= 1" , "requests"
               ]
 
 setuptools.setup(
     name="py_topping",
-    version="0.4.6",
+    version="0.4.7",
     license = "MIT",	
     author="Chanon Krittapholchai",
     author_email="chanon.krittapholchai@gmail.com",
     description="simplify functions from other libraries functions in 1-2 lines",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/chanon-kr/Shared_Function",
-    download_url = "https://github.com/chanon-kr/Shared_Function/archive/v0.4.6.tar.gz",
+    download_url = "https://github.com/chanon-kr/Shared_Function/archive/v0.4.7.tar.gz",
     keywords = ["utility","ETL"],
     packages=setuptools.find_packages(),
     classifiers=[
         "Development Status :: 4 - Beta",
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License"
     ],
```

### Comparing `py_topping-0.4.6/tests/database.ipynb` & `py_topping-0.4.7/tests/database.ipynb`

 * *Files identical despite different names*

