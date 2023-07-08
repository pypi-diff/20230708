# Comparing `tmp/aiocomelit-0.0.0.tar.gz` & `tmp/aiocomelit-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiocomelit-0.0.0.tar", max compression
+gzip compressed data, was "aiocomelit-0.0.1.tar", max compression
```

## Comparing `aiocomelit-0.0.0.tar` & `aiocomelit-0.0.1.tar`

### file list

```diff
@@ -1,10 +1,9 @@
--rw-r--r--   0        0        0    11346 2023-07-04 19:31:04.621003 aiocomelit-0.0.0/LICENSE
--rw-r--r--   0        0        0     3306 2023-07-04 19:31:04.721003 aiocomelit-0.0.0/README.md
--rw-r--r--   0        0        0     1939 2023-07-04 21:27:08.278185 aiocomelit-0.0.0/pyproject.toml
--rw-r--r--   0        0        0       22 2023-07-04 21:29:02.313525 aiocomelit-0.0.0/src/aiocomelit/__init__.py
--rw-r--r--   0        0        0     7316 2023-07-05 17:48:03.745164 aiocomelit-0.0.0/src/aiocomelit/api.py
--rw-r--r--   0        0        0      247 2023-07-05 16:34:23.360134 aiocomelit-0.0.0/src/aiocomelit/const.py
--rw-r--r--   0        0        0      441 2023-07-05 15:21:44.223026 aiocomelit-0.0.0/src/aiocomelit/exceptions.py
--rw-r--r--   0        0        0       53 2023-07-04 19:31:04.441003 aiocomelit-0.0.0/src/aiocomelit/main.py
--rw-r--r--   0        0        0        0 2023-07-04 19:31:04.451003 aiocomelit-0.0.0/src/aiocomelit/py.typed
--rw-r--r--   0        0        0     4371 1970-01-01 00:00:00.000000 aiocomelit-0.0.0/PKG-INFO
+-rw-r--r--   0        0        0    11346 2023-07-04 19:31:04.621003 aiocomelit-0.0.1/LICENSE
+-rw-r--r--   0        0        0     3306 2023-07-04 19:31:04.721003 aiocomelit-0.0.1/README.md
+-rw-r--r--   0        0        0     1940 2023-07-06 13:19:21.749209 aiocomelit-0.0.1/pyproject.toml
+-rw-r--r--   0        0        0      420 2023-07-05 21:05:53.271526 aiocomelit-0.0.1/src/aiocomelit/__init__.py
+-rw-r--r--   0        0        0     7695 2023-07-05 21:05:53.271526 aiocomelit-0.0.1/src/aiocomelit/api.py
+-rw-r--r--   0        0        0      319 2023-07-05 21:05:53.271526 aiocomelit-0.0.1/src/aiocomelit/const.py
+-rw-r--r--   0        0        0      441 2023-07-05 21:05:53.271526 aiocomelit-0.0.1/src/aiocomelit/exceptions.py
+-rw-r--r--   0        0        0        0 2023-07-04 19:31:04.451003 aiocomelit-0.0.1/src/aiocomelit/py.typed
+-rw-r--r--   0        0        0     4322 1970-01-01 00:00:00.000000 aiocomelit-0.0.1/PKG-INFO
```

### Comparing `aiocomelit-0.0.0/LICENSE` & `aiocomelit-0.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aiocomelit-0.0.0/README.md` & `aiocomelit-0.0.1/README.md`

 * *Files identical despite different names*

### Comparing `aiocomelit-0.0.0/pyproject.toml` & `aiocomelit-0.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aiocomelit"
-version = "0.0.0"
+version = "0.0.1"
 description = "Python library to control Comelit Simplehome"
 authors = ["Simone Chemelli <simone.chemelli@gmail.com>"]
 license = "Apache Software License 2.0"
 readme = "README.md"
 repository = "https://github.com/chemelli74/aiocomelit"
 classifiers = [
     "Development Status :: 2 - Pre-Alpha",
@@ -18,15 +18,15 @@
 ]
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/chemelli74/aiocomelit/issues"
 "Changelog" = "https://github.com/chemelli74/aiocomelit/blob/main/CHANGELOG.md"
 
 [tool.poetry.dependencies]
-python = "^3.9"
+python = "^3.10"
 aiohttp = "*"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.0"
 pytest-cov = "^3.0"
 
 [tool.semantic_release]
```

### Comparing `aiocomelit-0.0.0/src/aiocomelit/api.py` & `aiocomelit-0.0.1/src/aiocomelit/api.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,25 +3,26 @@
 from dataclasses import dataclass
 from datetime import datetime
 from http.cookies import SimpleCookie
 from typing import Any
 
 import aiohttp
 
-from .const import _LOGGER, CLIMATE, COVER, LIGHT, MAX_ZONES, OTHER
+from .const import _LOGGER, CLIMATE, COVER, COVER_STATUS, LIGHT, MAX_ZONES, OTHER
 from .exceptions import CannotAuthenticate, CannotConnect
 
 
 @dataclass
 class ComelitSerialBridgeObject:
     """Comelit SimpleHome Serial bridge class."""
 
     index: int
     name: str
-    status: int  # On / Off / Opening / Closing
+    status: int
+    human_status: str
     type: str
     val: int | dict[Any, Any]  # Temperature or Humidity (CLIMATE)
     protected: int
     zone: str
 
 
 @dataclass
@@ -132,31 +133,41 @@
             url,
             headers=self.headers,
             timeout=10,
         )
 
         return await response.json() if response.status == 200 else {}
 
+    async def _translate_device_status(self, dev_type: str, dev_status: int) -> str:
+        """Makes status human readable."""
+
+        if dev_type == COVER:
+            return COVER_STATUS[dev_status]
+
+        return "on" if dev_status == 1 else "off"
+
     async def get_all_devices(self) -> list[ComelitSerialBridgeObject]:
         """Get all connected devices."""
 
         _LOGGER.debug("Getting all devices for host %s", self.host)
 
         for dev_type in (CLIMATE, COVER, LIGHT, OTHER):
             reply_json = await self._get_devices(dev_type)
             _LOGGER.debug(
                 "List of devices of type %s: %s",
                 dev_type,
                 reply_json,
             )
             for i in range(reply_json["num"]):
+                status = reply_json["status"][i]
                 dev_info = ComelitSerialBridgeObject(
                     index=i,
                     name=reply_json["desc"][i],
-                    status=reply_json["status"][i],
+                    status=status,
+                    human_status=await self._translate_device_status(dev_type, status),
                     type=dev_type,
                     val=reply_json["val"][i],
                     protected=reply_json["protected"][i],
                     zone=reply_json["env_desc"][reply_json["env"][i]],
                 )
                 self._devices.append(dev_info)
```

### Comparing `aiocomelit-0.0.0/PKG-INFO` & `aiocomelit-0.0.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: aiocomelit
-Version: 0.0.0
+Version: 0.0.1
 Summary: Python library to control Comelit Simplehome
 Home-page: https://github.com/chemelli74/aiocomelit
 License: Apache Software License 2.0
 Author: Simone Chemelli
 Author-email: simone.chemelli@gmail.com
-Requires-Python: >=3.9,<4.0
+Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: Other/Proprietary License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries
 Requires-Dist: aiohttp
 Project-URL: Bug Tracker, https://github.com/chemelli74/aiocomelit/issues
 Project-URL: Changelog, https://github.com/chemelli74/aiocomelit/blob/main/CHANGELOG.md
 Project-URL: Repository, https://github.com/chemelli74/aiocomelit
```

#### html2text {}

```diff
@@ -1,22 +1,21 @@
-Metadata-Version: 2.1 Name: aiocomelit Version: 0.0.0 Summary: Python library
+Metadata-Version: 2.1 Name: aiocomelit Version: 0.0.1 Summary: Python library
 to control Comelit Simplehome Home-page: https://github.com/chemelli74/
 aiocomelit License: Apache Software License 2.0 Author: Simone Chemelli Author-
-email: simone.chemelli@gmail.com Requires-Python: >=3.9,<4.0 Classifier:
+email: simone.chemelli@gmail.com Requires-Python: >=3.10,<4.0 Classifier:
 Development Status :: 2 - Pre-Alpha Classifier: Intended Audience :: Developers
 Classifier: License :: Other/Proprietary License Classifier: Natural Language
 :: English Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
-:: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
-Programming Language :: Python :: 3.11 Classifier: Topic :: Software
-Development :: Libraries Requires-Dist: aiohttp Project-URL: Bug Tracker,
-https://github.com/chemelli74/aiocomelit/issues Project-URL: Changelog, https:/
-/github.com/chemelli74/aiocomelit/blob/main/CHANGELOG.md Project-URL:
-Repository, https://github.com/chemelli74/aiocomelit Description-Content-Type:
-text/markdown # aiocomelit
+:: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier: Topic ::
+Software Development :: Libraries Requires-Dist: aiohttp Project-URL: Bug
+Tracker, https://github.com/chemelli74/aiocomelit/issues Project-URL:
+Changelog, https://github.com/chemelli74/aiocomelit/blob/main/CHANGELOG.md
+Project-URL: Repository, https://github.com/chemelli74/aiocomelit Description-
+Content-Type: text/markdown # aiocomelit
                     [CI_Status] [Test_coverage_percentage]
                          [Poetry] [black] [pre-commit]
              [PyPI_Version] [Supported Python versions] [License]
 Python library to control Comelit Simplehome ## Installation Install this via
 pip (or your favourite package manager): `pip install aiocomelit` ##
 Contributors â¨ Thanks goes to these wonderful people ([emoji key](https://
 allcontributors.org/docs/en/emoji-key)):       This project follows the [all-
```

