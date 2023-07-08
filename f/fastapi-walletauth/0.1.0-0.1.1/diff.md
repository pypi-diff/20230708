# Comparing `tmp/fastapi_walletauth-0.1.0.tar.gz` & `tmp/fastapi_walletauth-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_walletauth-0.1.0.tar", max compression
+gzip compressed data, was "fastapi_walletauth-0.1.1.tar", max compression
```

## Comparing `fastapi_walletauth-0.1.0.tar` & `fastapi_walletauth-0.1.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     2133 2023-07-08 12:01:38.681437 fastapi_walletauth-0.1.0/README.md
--rw-r--r--   0        0        0       44 2023-07-08 10:30:18.996304 fastapi_walletauth-0.1.0/fastapi_walletauth/__init__.py
--rw-r--r--   0        0        0     7686 2023-07-08 12:27:15.879722 fastapi_walletauth-0.1.0/fastapi_walletauth/core.py
--rw-r--r--   0        0        0      474 2023-07-08 10:16:40.389853 fastapi_walletauth-0.1.0/fastapi_walletauth/magic.py
--rw-r--r--   0        0        0     1993 2023-07-08 12:27:15.855722 fastapi_walletauth-0.1.0/fastapi_walletauth/router.py
--rw-r--r--   0        0        0     2616 2023-07-08 12:19:55.853248 fastapi_walletauth-0.1.0/fastapi_walletauth/verification.py
--rw-r--r--   0        0        0      379 2023-07-08 12:27:15.883722 fastapi_walletauth-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2601 1970-01-01 00:00:00.000000 fastapi_walletauth-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     2716 2023-07-08 12:37:14.273534 fastapi_walletauth-0.1.1/README.md
+-rw-r--r--   0        0        0       44 2023-07-08 10:30:18.996304 fastapi_walletauth-0.1.1/fastapi_walletauth/__init__.py
+-rw-r--r--   0        0        0     7682 2023-07-08 12:31:15.031675 fastapi_walletauth-0.1.1/fastapi_walletauth/core.py
+-rw-r--r--   0        0        0      474 2023-07-08 10:16:40.389853 fastapi_walletauth-0.1.1/fastapi_walletauth/magic.py
+-rw-r--r--   0        0        0     1993 2023-07-08 12:27:15.855722 fastapi_walletauth-0.1.1/fastapi_walletauth/router.py
+-rw-r--r--   0        0        0     2616 2023-07-08 12:19:55.853248 fastapi_walletauth-0.1.1/fastapi_walletauth/verification.py
+-rw-r--r--   0        0        0      449 2023-07-08 12:37:14.281534 fastapi_walletauth-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     3254 1970-01-01 00:00:00.000000 fastapi_walletauth-0.1.1/PKG-INFO
```

### Comparing `fastapi_walletauth-0.1.0/fastapi_walletauth/core.py` & `fastapi_walletauth-0.1.1/fastapi_walletauth/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 
     class Config:
         allow_population_by_field_name = True
         extra = "allow"
 
     def __init__(self, address: str, chain: SupportedChains, ttl: int = 120):
         valid_til = int(time.time()) + ttl  # 60 seconds
-        challenge = f'{{"chain":"{chain}","sender":"{address}","app":"{APP}","time":"{int(time.time())}"}}'
+        challenge = f'{{"chain":"{chain}","address":"{address}","app":"{APP}","time":"{time.time()}"}}'
         super().__init__(address=address, chain=chain, valid_til=valid_til, challenge=challenge)  # type: ignore
 
     @property
     def token(self) -> Optional[str]:
         if self.expired:
             raise TimeoutError("Token Expired")
         if self._token is False:
```

### Comparing `fastapi_walletauth-0.1.0/fastapi_walletauth/router.py` & `fastapi_walletauth-0.1.1/fastapi_walletauth/router.py`

 * *Files identical despite different names*

### Comparing `fastapi_walletauth-0.1.0/fastapi_walletauth/verification.py` & `fastapi_walletauth-0.1.1/fastapi_walletauth/verification.py`

 * *Files identical despite different names*

### Comparing `fastapi_walletauth-0.1.0/PKG-INFO` & `fastapi_walletauth-0.1.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: fastapi-walletauth
-Version: 0.1.0
-Summary: 
+Version: 0.1.1
+Summary: FastAPI extension for user authentication through signature challenges
 Author: mhh
 Author-email: mike.hukiewitz@robotter.ai
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: base58 (>=2.1.1,<3.0.0)
@@ -68,29 +68,35 @@
 @app.get("/protected")
 def protected(wa: WalletAuth = WalletAuthDep()):
     return wa.address
 ```
 
 ## Signing the challenge
 
-The challenge is a JSON object (similar to Aleph messages) containing the following fields:
+The challenge is a serialized JSON object containing the following fields:
 
 ```python
 message = {
     "chain": "ETH",
     "address": "0x...",
-    "type": "authorization_challenge",
-    "item_hash": "0x...",
+    "app": "myapp",
+    "time": 1688819493.8691394
 }
 ```
 
-- `chain`: The chain ID (e.g. `ETH` for Ethereum mainnet)
-- `address`: The address of the user
-- `type`: The type of message to be signed (`authorization_challenge`)
-- `item_hash`: A random hash
-
-Currently, it requires to be preprocessed into a *Verification Buffer* like this:
-```python
-"{chain}\n{sender}\n{type}\n{item_hash}".format(**message).encode("utf-8")
+**PLEASE NOTE**: The `app` field needs to be set to the name of your application. This is used to prevent replay attacks.
+```shell
+export FASTAPI_WALLETAUTH_APP=myapp
 ```
 
-before being signed with the user's private key. This signature is then sent to the `/authentication/solve` endpoint.
+The signature format depends on the wallet type and is specified in the `chain` field. This signature is then sent to the
+`/authentication/solve` endpoint to obtain a Bearer token.
+
+## Liability
+
+This software is provided "as is" and "with all faults." I make no representations or warranties of any kind concerning
+the safety, suitability, inaccuracies, typographical errors, or other harmful components of this
+software. There are inherent dangers in the use of any software, especially cryptographic implementations. You are solely
+responsible for determining whether this software is compatible with your machine and other software installed on your
+computer. You are also solely responsible for the choice of a wallet and the security of your private keys. You
+acknowledge and agree to waive any liability claim against me from any loss or damage of any kind arising out of or in
+connection with your use of this software.
```

