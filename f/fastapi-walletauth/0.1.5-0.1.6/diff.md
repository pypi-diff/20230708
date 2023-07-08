# Comparing `tmp/fastapi_walletauth-0.1.5.tar.gz` & `tmp/fastapi_walletauth-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_walletauth-0.1.5.tar", max compression
+gzip compressed data, was "fastapi_walletauth-0.1.6.tar", max compression
```

## Comparing `fastapi_walletauth-0.1.5.tar` & `fastapi_walletauth-0.1.6.tar`

### file list

```diff
@@ -1,8 +1,7 @@
--rw-r--r--   0        0        0     2710 2023-07-08 13:38:48.414070 fastapi_walletauth-0.1.5/README.md
--rw-r--r--   0        0        0      102 2023-07-08 13:39:37.701784 fastapi_walletauth-0.1.5/fastapi_walletauth/__init__.py
--rw-r--r--   0        0        0     7682 2023-07-08 13:38:48.422069 fastapi_walletauth-0.1.5/fastapi_walletauth/core.py
--rw-r--r--   0        0        0      474 2023-07-08 10:16:40.389853 fastapi_walletauth-0.1.5/fastapi_walletauth/magic.py
--rw-r--r--   0        0        0     1993 2023-07-08 12:27:15.855722 fastapi_walletauth-0.1.5/fastapi_walletauth/router.py
--rw-r--r--   0        0        0     2616 2023-07-08 12:19:55.853248 fastapi_walletauth-0.1.5/fastapi_walletauth/verification.py
--rw-r--r--   0        0        0      984 2023-07-08 13:39:37.713784 fastapi_walletauth-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     3768 1970-01-01 00:00:00.000000 fastapi_walletauth-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     2569 2023-07-08 14:11:52.193005 fastapi_walletauth-0.1.6/README.md
+-rw-r--r--   0        0        0      102 2023-07-08 13:39:37.701784 fastapi_walletauth-0.1.6/fastapi_walletauth/__init__.py
+-rw-r--r--   0        0        0     7682 2023-07-08 13:38:48.422069 fastapi_walletauth-0.1.6/fastapi_walletauth/core.py
+-rw-r--r--   0        0        0     1993 2023-07-08 12:27:15.855722 fastapi_walletauth-0.1.6/fastapi_walletauth/router.py
+-rw-r--r--   0        0        0     2616 2023-07-08 12:19:55.853248 fastapi_walletauth-0.1.6/fastapi_walletauth/verification.py
+-rw-r--r--   0        0        0     1025 2023-07-08 14:12:00.628969 fastapi_walletauth-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     3711 1970-01-01 00:00:00.000000 fastapi_walletauth-0.1.6/PKG-INFO
```

### Comparing `fastapi_walletauth-0.1.5/README.md` & `fastapi_walletauth-0.1.6/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -7,52 +7,40 @@
 
 ```shell
 pip install fastapi-walletauth
 ```
 
 ## Usage
 
-Adding the authentication endpoints is as simple as importing the `fastapi_walletauth.magic` module **after** the
-FastAPI application has been created:
+Adding the authentication endpoints is as simple as importing the `authorization_routes` from `fastapi_walletauth`:
 
 ```python
 from fastapi import FastAPI
+from fastapi_walletauth import authorization_routes
 
 app = FastAPI()
 
-import fastapi_walletauth
-```
-
-or if you prefer, you can add the endpoints manually:
-
-```python
-from fastapi import FastAPI
-from fastapi_walletauth.router import authorization
-
-app = FastAPI()
-
-app.include_router(authorization)
+app.include_router(authorization_routes)
 ```
 
 This will add the following endpoints to your application:
 
 - `POST /authentication/challenge`: Returns a challenge for the user to sign
 - `POST /authentication/solve`: Returns a Bearer token if the signature is valid
 - `POST /authentication/logout`: Invalidates the current token
 - `POST /authentication/refresh`: Returns a new token if the current token is valid
 
 You can then use `WalletAuthDep` to protect your endpoints:
 
 ```python
 from fastapi import FastAPI
-from fastapi_walletauth import WalletAuth, WalletAuthDep
+from fastapi_walletauth import WalletAuth, WalletAuthDep, authorization_routes
 
 app = FastAPI()
-
-import fastapi_walletauth.magic
+app.include_router(authorization_routes)
 
 @app.get("/protected")
 def protected(wa: WalletAuth = WalletAuthDep()):
     return wa.address
 ```
 
 ## Signing the challenge
```

### Comparing `fastapi_walletauth-0.1.5/fastapi_walletauth/core.py` & `fastapi_walletauth-0.1.6/fastapi_walletauth/core.py`

 * *Files identical despite different names*

### Comparing `fastapi_walletauth-0.1.5/fastapi_walletauth/router.py` & `fastapi_walletauth-0.1.6/fastapi_walletauth/router.py`

 * *Files identical despite different names*

### Comparing `fastapi_walletauth-0.1.5/fastapi_walletauth/verification.py` & `fastapi_walletauth-0.1.6/fastapi_walletauth/verification.py`

 * *Files identical despite different names*

### Comparing `fastapi_walletauth-0.1.5/pyproject.toml` & `fastapi_walletauth-0.1.6/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fastapi-walletauth"
-version = "0.1.5"
+version = "0.1.6"
 description = "FastAPI extension for user authentication through signature challenges"
 authors = ["mhh <mike.hukiewitz@robotter.ai>"]
 readme = "README.md"
 packages = [{include = "fastapi_walletauth"}]
 keywords = ["FastAPI", "authentication", "signature", "wallet", "ethereum", "solana", "web3"]
 classifiers = [
     "Environment :: Web Environment",
@@ -16,16 +16,18 @@
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Topic :: Security",
     "Typing :: Typed",
 ]
 
 [tool.poetry.dependencies]
-python = ">=3.6.2,<4.0"
+python = ">=3.7,<4.0"
 fastapi = ">=0.60.1,<1.0"
 pynacl = "^1.5.0"
 base58 = ">=2.0.0,<3.0"
+eth-account = "^0.9.0"
+eth-keys = "^0.4.0"
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `fastapi_walletauth-0.1.5/PKG-INFO` & `fastapi_walletauth-0.1.6/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 Metadata-Version: 2.1
 Name: fastapi-walletauth
-Version: 0.1.5
+Version: 0.1.6
 Summary: FastAPI extension for user authentication through signature challenges
 Keywords: FastAPI,authentication,signature,wallet,ethereum,solana,web3
 Author: mhh
 Author-email: mike.hukiewitz@robotter.ai
-Requires-Python: >=3.6.2,<4.0
+Requires-Python: >=3.7,<4.0
 Classifier: Environment :: Web Environment
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Topic :: Security
 Classifier: Typing :: Typed
 Requires-Dist: base58 (>=2.0.0,<3.0)
+Requires-Dist: eth-account (>=0.9.0,<0.10.0)
+Requires-Dist: eth-keys (>=0.4.0,<0.5.0)
 Requires-Dist: fastapi (>=0.60.1,<1.0)
 Requires-Dist: pynacl (>=1.5.0,<2.0.0)
 Description-Content-Type: text/markdown
 
 # FastAPI Wallet Authentication
 
 fastapi-walletauth provides a simple way to authenticate users in FastAPI applications using a wallet.
@@ -33,52 +35,40 @@
 
 ```shell
 pip install fastapi-walletauth
 ```
 
 ## Usage
 
-Adding the authentication endpoints is as simple as importing the `fastapi_walletauth.magic` module **after** the
-FastAPI application has been created:
+Adding the authentication endpoints is as simple as importing the `authorization_routes` from `fastapi_walletauth`:
 
 ```python
 from fastapi import FastAPI
+from fastapi_walletauth import authorization_routes
 
 app = FastAPI()
 
-import fastapi_walletauth
-```
-
-or if you prefer, you can add the endpoints manually:
-
-```python
-from fastapi import FastAPI
-from fastapi_walletauth.router import authorization
-
-app = FastAPI()
-
-app.include_router(authorization)
+app.include_router(authorization_routes)
 ```
 
 This will add the following endpoints to your application:
 
 - `POST /authentication/challenge`: Returns a challenge for the user to sign
 - `POST /authentication/solve`: Returns a Bearer token if the signature is valid
 - `POST /authentication/logout`: Invalidates the current token
 - `POST /authentication/refresh`: Returns a new token if the current token is valid
 
 You can then use `WalletAuthDep` to protect your endpoints:
 
 ```python
 from fastapi import FastAPI
-from fastapi_walletauth import WalletAuth, WalletAuthDep
+from fastapi_walletauth import WalletAuth, WalletAuthDep, authorization_routes
 
 app = FastAPI()
-
-import fastapi_walletauth.magic
+app.include_router(authorization_routes)
 
 @app.get("/protected")
 def protected(wa: WalletAuth = WalletAuthDep()):
     return wa.address
 ```
 
 ## Signing the challenge
```

