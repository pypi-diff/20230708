# Comparing `tmp/fastapi_walletauth-0.1.4.tar.gz` & `tmp/fastapi_walletauth-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_walletauth-0.1.4.tar", max compression
+gzip compressed data, was "fastapi_walletauth-0.1.5.tar", max compression
```

## Comparing `fastapi_walletauth-0.1.4.tar` & `fastapi_walletauth-0.1.5.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     2719 2023-07-08 12:57:30.935074 fastapi_walletauth-0.1.4/README.md
--rw-r--r--   0        0        0      988 2023-07-08 12:57:52.599017 fastapi_walletauth-0.1.4/pyproject.toml
--rw-r--r--   0        0        0       44 2023-07-08 10:30:18.996304 fastapi_walletauth-0.1.4/src/fastapi_walletauth/__init__.py
--rw-r--r--   0        0        0     7686 2023-07-08 12:57:30.951074 fastapi_walletauth-0.1.4/src/fastapi_walletauth/core.py
--rw-r--r--   0        0        0      474 2023-07-08 10:16:40.389853 fastapi_walletauth-0.1.4/src/fastapi_walletauth/magic.py
--rw-r--r--   0        0        0     1993 2023-07-08 12:27:15.855722 fastapi_walletauth-0.1.4/src/fastapi_walletauth/router.py
--rw-r--r--   0        0        0     2616 2023-07-08 12:19:55.853248 fastapi_walletauth-0.1.4/src/fastapi_walletauth/verification.py
--rw-r--r--   0        0        0     3777 1970-01-01 00:00:00.000000 fastapi_walletauth-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     2710 2023-07-08 13:38:48.414070 fastapi_walletauth-0.1.5/README.md
+-rw-r--r--   0        0        0      102 2023-07-08 13:39:37.701784 fastapi_walletauth-0.1.5/fastapi_walletauth/__init__.py
+-rw-r--r--   0        0        0     7682 2023-07-08 13:38:48.422069 fastapi_walletauth-0.1.5/fastapi_walletauth/core.py
+-rw-r--r--   0        0        0      474 2023-07-08 10:16:40.389853 fastapi_walletauth-0.1.5/fastapi_walletauth/magic.py
+-rw-r--r--   0        0        0     1993 2023-07-08 12:27:15.855722 fastapi_walletauth-0.1.5/fastapi_walletauth/router.py
+-rw-r--r--   0        0        0     2616 2023-07-08 12:19:55.853248 fastapi_walletauth-0.1.5/fastapi_walletauth/verification.py
+-rw-r--r--   0        0        0      984 2023-07-08 13:39:37.713784 fastapi_walletauth-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     3768 1970-01-01 00:00:00.000000 fastapi_walletauth-0.1.5/PKG-INFO
```

### Comparing `fastapi_walletauth-0.1.4/README.md` & `fastapi_walletauth-0.1.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 FastAPI application has been created:
 
 ```python
 from fastapi import FastAPI
 
 app = FastAPI()
 
-from src import fastapi_walletauth
+import fastapi_walletauth
 ```
 
 or if you prefer, you can add the endpoints manually:
 
 ```python
 from fastapi import FastAPI
 from fastapi_walletauth.router import authorization
```

### Comparing `fastapi_walletauth-0.1.4/pyproject.toml` & `fastapi_walletauth-0.1.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [tool.poetry]
 name = "fastapi-walletauth"
-version = "0.1.4"
+version = "0.1.5"
 description = "FastAPI extension for user authentication through signature challenges"
 authors = ["mhh <mike.hukiewitz@robotter.ai>"]
 readme = "README.md"
-packages = [{include = "src/fastapi_walletauth"}]
+packages = [{include = "fastapi_walletauth"}]
 keywords = ["FastAPI", "authentication", "signature", "wallet", "ethereum", "solana", "web3"]
 classifiers = [
     "Environment :: Web Environment",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.6",
```

### Comparing `fastapi_walletauth-0.1.4/src/fastapi_walletauth/core.py` & `fastapi_walletauth-0.1.5/fastapi_walletauth/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from fastapi.security import HTTPBearer
 from fastapi.security.utils import get_authorization_scheme_param
 from nacl.bindings.randombytes import randombytes
 from pydantic import BaseModel, Field
 from starlette.requests import Request
 from starlette.status import HTTP_401_UNAUTHORIZED, HTTP_403_FORBIDDEN
 
-from src.fastapi_walletauth.verification import verify_signature_sol, verify_signature_eth
+from fastapi_walletauth.verification import verify_signature_sol, verify_signature_eth
 
 
 APP = os.environ.get("FASTAPI_WALLETAUTH_APP", "unsafe_fastapi_walletauth")
 
 
 class SupportedChains(Enum):
     Solana = "SOL"
```

### Comparing `fastapi_walletauth-0.1.4/src/fastapi_walletauth/router.py` & `fastapi_walletauth-0.1.5/fastapi_walletauth/router.py`

 * *Files identical despite different names*

### Comparing `fastapi_walletauth-0.1.4/src/fastapi_walletauth/verification.py` & `fastapi_walletauth-0.1.5/fastapi_walletauth/verification.py`

 * *Files identical despite different names*

### Comparing `fastapi_walletauth-0.1.4/PKG-INFO` & `fastapi_walletauth-0.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi-walletauth
-Version: 0.1.4
+Version: 0.1.5
 Summary: FastAPI extension for user authentication through signature challenges
 Keywords: FastAPI,authentication,signature,wallet,ethereum,solana,web3
 Author: mhh
 Author-email: mike.hukiewitz@robotter.ai
 Requires-Python: >=3.6.2,<4.0
 Classifier: Environment :: Web Environment
 Classifier: License :: OSI Approved :: MIT License
@@ -41,15 +41,15 @@
 FastAPI application has been created:
 
 ```python
 from fastapi import FastAPI
 
 app = FastAPI()
 
-from src import fastapi_walletauth
+import fastapi_walletauth
 ```
 
 or if you prefer, you can add the endpoints manually:
 
 ```python
 from fastapi import FastAPI
 from fastapi_walletauth.router import authorization
```

