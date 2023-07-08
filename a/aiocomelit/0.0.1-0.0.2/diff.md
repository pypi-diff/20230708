# Comparing `tmp/aiocomelit-0.0.1.tar.gz` & `tmp/aiocomelit-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiocomelit-0.0.1.tar", max compression
+gzip compressed data, was "aiocomelit-0.0.2.tar", max compression
```

## Comparing `aiocomelit-0.0.1.tar` & `aiocomelit-0.0.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    11346 2023-07-04 19:31:04.621003 aiocomelit-0.0.1/LICENSE
--rw-r--r--   0        0        0     3306 2023-07-04 19:31:04.721003 aiocomelit-0.0.1/README.md
--rw-r--r--   0        0        0     1940 2023-07-06 13:19:21.749209 aiocomelit-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      420 2023-07-05 21:05:53.271526 aiocomelit-0.0.1/src/aiocomelit/__init__.py
--rw-r--r--   0        0        0     7695 2023-07-05 21:05:53.271526 aiocomelit-0.0.1/src/aiocomelit/api.py
--rw-r--r--   0        0        0      319 2023-07-05 21:05:53.271526 aiocomelit-0.0.1/src/aiocomelit/const.py
--rw-r--r--   0        0        0      441 2023-07-05 21:05:53.271526 aiocomelit-0.0.1/src/aiocomelit/exceptions.py
--rw-r--r--   0        0        0        0 2023-07-04 19:31:04.451003 aiocomelit-0.0.1/src/aiocomelit/py.typed
--rw-r--r--   0        0        0     4322 1970-01-01 00:00:00.000000 aiocomelit-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0    11346 2023-07-04 19:31:04.621003 aiocomelit-0.0.2/LICENSE
+-rw-r--r--   0        0        0     3306 2023-07-04 19:31:04.721003 aiocomelit-0.0.2/README.md
+-rw-r--r--   0        0        0     1940 2023-07-08 10:59:45.676430 aiocomelit-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      420 2023-07-08 10:59:45.676430 aiocomelit-0.0.2/src/aiocomelit/__init__.py
+-rw-r--r--   0        0        0     7833 2023-07-08 10:59:45.676430 aiocomelit-0.0.2/src/aiocomelit/api.py
+-rw-r--r--   0        0        0      319 2023-07-05 21:05:53.271526 aiocomelit-0.0.2/src/aiocomelit/const.py
+-rw-r--r--   0        0        0      441 2023-07-05 21:05:53.271526 aiocomelit-0.0.2/src/aiocomelit/exceptions.py
+-rw-r--r--   0        0        0        0 2023-07-04 19:31:04.451003 aiocomelit-0.0.2/src/aiocomelit/py.typed
+-rw-r--r--   0        0        0     4322 1970-01-01 00:00:00.000000 aiocomelit-0.0.2/PKG-INFO
```

### Comparing `aiocomelit-0.0.1/LICENSE` & `aiocomelit-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `aiocomelit-0.0.1/README.md` & `aiocomelit-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `aiocomelit-0.0.1/pyproject.toml` & `aiocomelit-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aiocomelit"
-version = "0.0.1"
+version = "0.0.2"
 description = "Python library to control Comelit Simplehome"
 authors = ["Simone Chemelli <simone.chemelli@gmail.com>"]
 license = "Apache Software License 2.0"
 readme = "README.md"
 repository = "https://github.com/chemelli74/aiocomelit"
 classifiers = [
     "Development Status :: 2 - Pre-Alpha",
```

### Comparing `aiocomelit-0.0.1/src/aiocomelit/api.py` & `aiocomelit-0.0.2/src/aiocomelit/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -169,26 +169,32 @@
                     protected=reply_json["protected"][i],
                     zone=reply_json["env_desc"][reply_json["env"][i]],
                 )
                 self._devices.append(dev_info)
 
         return self._devices
 
-    async def get_alarm_config(self) -> list[ComelitVedoObject]:
-        """Get Comelit SimpleHome alarm configuration."""
+    async def alarm_login(self) -> bool:
+        """Login to vedo alarm system."""
         _LOGGER.debug("Logging into %s (VEDO)", self.host)
         try:
             logged = await self._do_alarm_login()
         except (asyncio.exceptions.TimeoutError, aiohttp.ClientConnectorError) as exc:
             _LOGGER.warning("Connection error for %s", self.host)
             raise CannotConnect from exc
 
         if not logged:
             raise CannotAuthenticate
 
+        return True
+
+    async def get_alarm_config(self) -> list[ComelitVedoObject]:
+        """Get Comelit SimpleHome alarm configuration."""
+
+        await self.alarm_login()
         await asyncio.sleep(0.5)
 
         reply_json_desc = await self._get_alarm_desc()
         _LOGGER.debug("Alarm description: %s", reply_json_desc)
         reply_json_stat = await self._get_alarm_stat()
         _LOGGER.debug("Alarm statistics: %s", reply_json_stat)
```

### Comparing `aiocomelit-0.0.1/PKG-INFO` & `aiocomelit-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiocomelit
-Version: 0.0.1
+Version: 0.0.2
 Summary: Python library to control Comelit Simplehome
 Home-page: https://github.com/chemelli74/aiocomelit
 License: Apache Software License 2.0
 Author: Simone Chemelli
 Author-email: simone.chemelli@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: aiocomelit Version: 0.0.1 Summary: Python library
+Metadata-Version: 2.1 Name: aiocomelit Version: 0.0.2 Summary: Python library
 to control Comelit Simplehome Home-page: https://github.com/chemelli74/
 aiocomelit License: Apache Software License 2.0 Author: Simone Chemelli Author-
 email: simone.chemelli@gmail.com Requires-Python: >=3.10,<4.0 Classifier:
 Development Status :: 2 - Pre-Alpha Classifier: Intended Audience :: Developers
 Classifier: License :: Other/Proprietary License Classifier: Natural Language
 :: English Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
```

