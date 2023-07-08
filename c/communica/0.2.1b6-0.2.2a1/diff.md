# Comparing `tmp/communica-0.2.1b6.tar.gz` & `tmp/communica-0.2.2a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "communica-0.2.1b6.tar", last modified: Mon Jul  3 06:14:47 2023, max compression
+gzip compressed data, was "communica-0.2.2a1.tar", last modified: Sat Jul  8 09:22:56 2023, max compression
```

## Comparing `communica-0.2.1b6.tar` & `communica-0.2.2a1.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxrwxrwx   0        0        0        0 2023-07-03 06:14:47.065554 communica-0.2.1b6/
--rw-rw-rw-   0        0        0      568 2023-03-25 20:48:52.000000 communica-0.2.1b6/LICENSE.txt
--rw-rw-rw-   0        0        0     2233 2023-07-03 06:14:47.065554 communica-0.2.1b6/PKG-INFO
--rw-rw-rw-   0        0        0     1456 2023-04-04 20:46:58.000000 communica-0.2.1b6/README.md
-drwxrwxrwx   0        0        0        0 2023-07-03 06:14:47.036555 communica-0.2.1b6/communica/
--rw-rw-rw-   0        0        0      101 2023-02-15 13:48:00.000000 communica-0.2.1b6/communica/__init__.py
--rw-rw-rw-   0        0        0      130 2023-03-19 21:29:46.000000 communica-0.2.1b6/communica/clients.py
-drwxrwxrwx   0        0        0        0 2023-07-03 06:14:47.053575 communica-0.2.1b6/communica/connectors/
--rw-rw-rw-   0        0        0      170 2023-03-31 19:34:58.000000 communica-0.2.1b6/communica/connectors/__init__.py
--rw-rw-rw-   0        0        0     2919 2023-05-30 15:52:39.000000 communica-0.2.1b6/communica/connectors/_stream_local.py
--rw-rw-rw-   0        0        0     5553 2023-07-03 06:13:05.000000 communica-0.2.1b6/communica/connectors/base.py
--rw-rw-rw-   0        0        0    28175 2023-07-03 06:08:14.000000 communica-0.2.1b6/communica/connectors/rabbitmq.py
--rw-rw-rw-   0        0        0    10130 2023-05-21 11:36:08.000000 communica-0.2.1b6/communica/connectors/stream.py
--rw-rw-rw-   0        0        0     1945 2023-05-08 09:05:11.000000 communica-0.2.1b6/communica/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-07-03 06:14:47.056553 communica-0.2.1b6/communica/pairs/
--rw-rw-rw-   0        0        0      223 2023-03-19 15:01:07.000000 communica-0.2.1b6/communica/pairs/__init__.py
--rw-rw-rw-   0        0        0     2975 2023-05-04 13:02:31.000000 communica-0.2.1b6/communica/pairs/base.py
--rw-rw-rw-   0        0        0     9863 2023-05-21 12:35:07.000000 communica-0.2.1b6/communica/pairs/route.py
--rw-rw-rw-   0        0        0    16363 2023-07-03 05:53:23.000000 communica-0.2.1b6/communica/pairs/simple.py
-drwxrwxrwx   0        0        0        0 2023-07-03 06:14:47.060553 communica-0.2.1b6/communica/serializers/
--rw-rw-rw-   0        0        0      242 2023-05-08 07:15:52.000000 communica-0.2.1b6/communica/serializers/__init__.py
--rw-rw-rw-   0        0        0     1672 2023-05-23 11:23:18.000000 communica-0.2.1b6/communica/serializers/adaptix.py
--rw-rw-rw-   0        0        0      657 2023-03-18 18:41:17.000000 communica-0.2.1b6/communica/serializers/base.py
--rw-rw-rw-   0        0        0      315 2023-03-18 19:40:10.000000 communica-0.2.1b6/communica/serializers/json.py
--rw-rw-rw-   0        0        0      128 2023-03-19 21:29:36.000000 communica-0.2.1b6/communica/servers.py
--rw-rw-rw-   0        0        0     4375 2023-05-30 16:58:39.000000 communica-0.2.1b6/communica/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-03 06:14:47.047553 communica-0.2.1b6/communica.egg-info/
--rw-rw-rw-   0        0        0     2233 2023-07-03 06:14:47.000000 communica-0.2.1b6/communica.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      811 2023-07-03 06:14:47.000000 communica-0.2.1b6/communica.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-03 06:14:47.000000 communica-0.2.1b6/communica.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      164 2023-07-03 06:14:47.000000 communica-0.2.1b6/communica.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-07-03 06:14:47.000000 communica-0.2.1b6/communica.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1130 2023-07-03 06:14:12.000000 communica-0.2.1b6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-03 06:14:47.065554 communica-0.2.1b6/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-03 06:14:47.064554 communica-0.2.1b6/tests/
--rw-rw-rw-   0        0        0     2495 2023-07-03 06:04:05.000000 communica-0.2.1b6/tests/test_connectors.py
--rw-rw-rw-   0        0        0     6508 2023-05-08 10:49:51.000000 communica-0.2.1b6/tests/test_entities.py
--rw-rw-rw-   0        0        0     2481 2023-07-03 05:55:23.000000 communica-0.2.1b6/tests/test_rmq_conn_check_policy.py
--rw-rw-rw-   0        0        0     1081 2023-05-08 10:22:35.000000 communica-0.2.1b6/tests/test_serializers.py
+drwxrwxrwx   0        0        0        0 2023-07-08 09:22:56.404833 communica-0.2.2a1/
+-rw-rw-rw-   0        0        0      568 2023-03-25 20:48:52.000000 communica-0.2.2a1/LICENSE.txt
+-rw-rw-rw-   0        0        0     2233 2023-07-08 09:22:56.404833 communica-0.2.2a1/PKG-INFO
+-rw-rw-rw-   0        0        0     1456 2023-04-04 20:46:58.000000 communica-0.2.2a1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-08 09:22:56.383834 communica-0.2.2a1/communica/
+-rw-rw-rw-   0        0        0      101 2023-02-15 13:48:00.000000 communica-0.2.2a1/communica/__init__.py
+-rw-rw-rw-   0        0        0      130 2023-03-19 21:29:46.000000 communica-0.2.2a1/communica/clients.py
+drwxrwxrwx   0        0        0        0 2023-07-08 09:22:56.392833 communica-0.2.2a1/communica/connectors/
+-rw-rw-rw-   0        0        0      170 2023-03-31 19:34:58.000000 communica-0.2.2a1/communica/connectors/__init__.py
+-rw-rw-rw-   0        0        0     2919 2023-05-30 15:52:39.000000 communica-0.2.2a1/communica/connectors/_stream_local.py
+-rw-rw-rw-   0        0        0     5553 2023-07-03 06:13:05.000000 communica-0.2.2a1/communica/connectors/base.py
+-rw-rw-rw-   0        0        0    28175 2023-07-03 06:08:14.000000 communica-0.2.2a1/communica/connectors/rabbitmq.py
+-rw-rw-rw-   0        0        0    10130 2023-05-21 11:36:08.000000 communica-0.2.2a1/communica/connectors/stream.py
+-rw-rw-rw-   0        0        0     1945 2023-05-08 09:05:11.000000 communica-0.2.2a1/communica/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-07-08 09:22:56.396834 communica-0.2.2a1/communica/pairs/
+-rw-rw-rw-   0        0        0      223 2023-03-19 15:01:07.000000 communica-0.2.2a1/communica/pairs/__init__.py
+-rw-rw-rw-   0        0        0     2975 2023-05-04 13:02:31.000000 communica-0.2.2a1/communica/pairs/base.py
+-rw-rw-rw-   0        0        0     9877 2023-07-08 09:19:50.000000 communica-0.2.2a1/communica/pairs/route.py
+-rw-rw-rw-   0        0        0    16366 2023-07-08 09:15:21.000000 communica-0.2.2a1/communica/pairs/simple.py
+drwxrwxrwx   0        0        0        0 2023-07-08 09:22:56.399833 communica-0.2.2a1/communica/serializers/
+-rw-rw-rw-   0        0        0      242 2023-05-08 07:15:52.000000 communica-0.2.2a1/communica/serializers/__init__.py
+-rw-rw-rw-   0        0        0     1991 2023-07-08 09:13:26.000000 communica-0.2.2a1/communica/serializers/adaptix.py
+-rw-rw-rw-   0        0        0      750 2023-07-08 09:12:00.000000 communica-0.2.2a1/communica/serializers/base.py
+-rw-rw-rw-   0        0        0      315 2023-03-18 19:40:10.000000 communica-0.2.2a1/communica/serializers/json.py
+-rw-rw-rw-   0        0        0      128 2023-03-19 21:29:36.000000 communica-0.2.2a1/communica/servers.py
+-rw-rw-rw-   0        0        0     4375 2023-07-03 06:24:57.000000 communica-0.2.2a1/communica/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-08 09:22:56.387834 communica-0.2.2a1/communica.egg-info/
+-rw-rw-rw-   0        0        0     2233 2023-07-08 09:22:56.000000 communica-0.2.2a1/communica.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      811 2023-07-08 09:22:56.000000 communica-0.2.2a1/communica.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-08 09:22:56.000000 communica-0.2.2a1/communica.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      164 2023-07-08 09:22:56.000000 communica-0.2.2a1/communica.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-08 09:22:56.000000 communica-0.2.2a1/communica.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1130 2023-07-08 09:17:56.000000 communica-0.2.2a1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-08 09:22:56.404833 communica-0.2.2a1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-08 09:22:56.403833 communica-0.2.2a1/tests/
+-rw-rw-rw-   0        0        0     2495 2023-07-03 06:04:05.000000 communica-0.2.2a1/tests/test_connectors.py
+-rw-rw-rw-   0        0        0     6508 2023-05-08 10:49:51.000000 communica-0.2.2a1/tests/test_entities.py
+-rw-rw-rw-   0        0        0     2481 2023-07-03 05:55:23.000000 communica-0.2.2a1/tests/test_rmq_conn_check_policy.py
+-rw-rw-rw-   0        0        0     1081 2023-05-08 10:22:35.000000 communica-0.2.2a1/tests/test_serializers.py
```

### Comparing `communica-0.2.1b6/LICENSE.txt` & `communica-0.2.2a1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `communica-0.2.1b6/PKG-INFO` & `communica-0.2.2a1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: communica
-Version: 0.2.1b6
+Version: 0.2.2a1
 Summary: Easy to use IPC library
 Author-email: Elchin Sarkarov <elchin751@gmail.com>
 Project-URL: Homepage, https://github.com/elchinchel/communica-py
 Project-URL: Bug Tracker, https://github.com/elchinchel/communica-py/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `communica-0.2.1b6/README.md` & `communica-0.2.2a1/README.md`

 * *Files identical despite different names*

### Comparing `communica-0.2.1b6/communica/connectors/_stream_local.py` & `communica-0.2.2a1/communica/connectors/_stream_local.py`

 * *Files identical despite different names*

### Comparing `communica-0.2.1b6/communica/connectors/base.py` & `communica-0.2.2a1/communica/connectors/base.py`

 * *Files identical despite different names*

### Comparing `communica-0.2.1b6/communica/connectors/rabbitmq.py` & `communica-0.2.2a1/communica/connectors/rabbitmq.py`

 * *Files identical despite different names*

### Comparing `communica-0.2.1b6/communica/connectors/stream.py` & `communica-0.2.2a1/communica/connectors/stream.py`

 * *Files identical despite different names*

### Comparing `communica-0.2.1b6/communica/exceptions.py` & `communica-0.2.2a1/communica/exceptions.py`

 * *Files identical despite different names*

### Comparing `communica-0.2.1b6/communica/pairs/base.py` & `communica-0.2.2a1/communica/pairs/base.py`

 * *Files identical despite different names*

### Comparing `communica-0.2.1b6/communica/pairs/route.py` & `communica-0.2.2a1/communica/pairs/route.py`

 * *Files 0% similar despite different names*

```diff
@@ -114,28 +114,28 @@
         elif saved_serializer is not serializer:
             raise TypeError('You should always use the same serializer for '
                            f'the same route ({saved_serializer!r} '
                             'has already been used earlier)')
 
         await self._connection.send(
             Metadata(id=request_id, type=RequestType.REQ_REP, route=route),
-            serializer.dump(data)
+            serializer.client_dump(data)
         )
 
         return await fut
 
     async def throw(
             self,
             route: str,
             serializer: 'BaseSerializer | None',
             data: Any
     ) -> None:
         await self._connection.send(
             Metadata(id='', type=RequestType.REQ_THROW, route=route),
-            (serializer or default_serializer).dump(data)
+            (serializer or default_serializer).client_dump(data)
         )
 
 
 class RouteClient(ReqRepClient):
     """
     Pair for RouteServer.
```

### Comparing `communica-0.2.1b6/communica/pairs/simple.py` & `communica-0.2.2a1/communica/pairs/simple.py`

 * *Files 0% similar despite different names*

```diff
@@ -110,23 +110,23 @@
             logger.warning('Drop response for unknown or expired request')
             return
 
         req_type = metadata['type']
 
         if req_type == RequestType.RESP_OK:
             try:
-                fut.set_result(serializer.load(raw_data))
+                fut.set_result(serializer.client_load(raw_data))
             except Exception as e:
                 # if serializer can't load response, considering this
                 # requester's error, cause responder can't do
                 # anything about it after sending response
                 fut.set_exception(e)
             return
 
-        data = default_serializer.load(raw_data)
+        data = default_serializer.client_load(raw_data)
         if req_type == RequestType.RESP_ERR_REQUESTER:
             fut.set_exception(ReqError.from_dict(data))
         elif req_type == RequestType.RESP_ERR_RESPONDER:
             fut.set_exception(RespError.from_dict(data))
         elif req_type == RequestType.RESP_ERR_UNKNOWN:
             fut.set_exception(UnknownError.from_dict(data))
         elif req_type == RequestType.RESP_ERR_DATA_LOAD:
@@ -144,15 +144,14 @@
             metadata: Metadata,
             raw_data: Any
     ) -> 'tuple[dict, Any]':
         resp_meta = metadata.copy()
 
         try:
             data = serializer.load(raw_data)
-            print(data)
         except Exception as e:
             resp_meta['type'] = RequestType.RESP_ERR_DATA_LOAD
             resp_data = SerializerError(repr(e)).to_dict()
             return resp_meta, resp_data  # type: ignore
 
         try:
             if handler.is_async:
@@ -232,23 +231,23 @@
         )
 
     async def request(self, data: Any) -> bytes:
         request_id, fut = self._create_response_waiter()
 
         await self._connection.send(
             Metadata(id=request_id, type=RequestType.REQ_REP),
-            self.serializer.dump(data)
+            self.serializer.client_dump(data)
         )
 
         return await fut
 
     async def throw(self, data: Any) -> None:
         await self._connection.send(
             Metadata(id='', type=RequestType.REQ_THROW),
-            self.serializer.dump(data)
+            self.serializer.client_dump(data)
         )
 
 
 class ReqRepClient(BaseClient):
     __slots__ = ('_connected_event', '_run_task', '_client_id', '_flow')
 
     _run_task: 'asyncio.Task | None'
```

### Comparing `communica-0.2.1b6/communica/serializers/adaptix.py` & `communica-0.2.2a1/communica/serializers/adaptix.py`

 * *Files 10% similar despite different names*

```diff
@@ -44,7 +44,18 @@
             self._req_model
         )
 
     def dump(self, data: TResp) -> bytes:
         return json_dumpb(
             self._retort.dump(data, self._resp_model)
         )
+
+    def client_load(self, raw_data: bytes) -> 'TResp | Any':
+        return self._retort.load(
+            json_loadb(raw_data),
+            self._resp_model
+        )
+
+    def client_dump(self, data: TReq) -> bytes:
+        return json_dumpb(
+            self._retort.dump(data, self._req_model)
+        )
```

### Comparing `communica-0.2.1b6/communica/utils.py` & `communica-0.2.2a1/communica/utils.py`

 * *Files identical despite different names*

### Comparing `communica-0.2.1b6/communica.egg-info/PKG-INFO` & `communica-0.2.2a1/communica.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: communica
-Version: 0.2.1b6
+Version: 0.2.2a1
 Summary: Easy to use IPC library
 Author-email: Elchin Sarkarov <elchin751@gmail.com>
 Project-URL: Homepage, https://github.com/elchinchel/communica-py
 Project-URL: Bug Tracker, https://github.com/elchinchel/communica-py/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `communica-0.2.1b6/communica.egg-info/SOURCES.txt` & `communica-0.2.2a1/communica.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `communica-0.2.1b6/pyproject.toml` & `communica-0.2.2a1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "communica"
-version = "0.2.1b6"
+version = "0.2.2a1"
 authors = [
   { name="Elchin Sarkarov", email="elchin751@gmail.com" },
 ]
 description = "Easy to use IPC library"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `communica-0.2.1b6/tests/test_connectors.py` & `communica-0.2.2a1/tests/test_connectors.py`

 * *Files identical despite different names*

### Comparing `communica-0.2.1b6/tests/test_entities.py` & `communica-0.2.2a1/tests/test_entities.py`

 * *Files identical despite different names*

### Comparing `communica-0.2.1b6/tests/test_rmq_conn_check_policy.py` & `communica-0.2.2a1/tests/test_rmq_conn_check_policy.py`

 * *Files identical despite different names*

### Comparing `communica-0.2.1b6/tests/test_serializers.py` & `communica-0.2.2a1/tests/test_serializers.py`

 * *Files identical despite different names*

