# Comparing `tmp/hat_chatter-0.5.8-cp38.cp39.cp310-none-any.whl.zip` & `tmp/hat_chatter-0.5.9-cp38.cp39.cp310-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 10840 bytes, number of entries: 8
--rw-r--r--  2.0 unx    15341 b- defN 22-Sep-28 14:34 hat/chatter/__init__.py
+Zip file size: 10867 bytes, number of entries: 8
+-rw-r--r--  2.0 unx    15408 b- defN 22-Oct-14 00:23 hat/chatter/__init__.py
 -rw-r--r--  2.0 unx     1375 b- defN 22-Sep-28 14:35 hat/chatter/sbs_repo.json
--rw-r--r--  2.0 unx    11358 b- defN 22-Sep-28 14:35 hat_chatter-0.5.8.dist-info/LICENSE
--rw-r--r--  2.0 unx     1929 b- defN 22-Sep-28 14:35 hat_chatter-0.5.8.dist-info/METADATA
--rw-r--r--  2.0 unx      132 b- defN 22-Sep-28 14:35 hat_chatter-0.5.8.dist-info/WHEEL
--rw-r--r--  2.0 unx        4 b- defN 22-Sep-28 14:35 hat_chatter-0.5.8.dist-info/top_level.txt
--rw-r--r--  2.0 unx        1 b- defN 22-Sep-28 14:35 hat_chatter-0.5.8.dist-info/zip-safe
-?rw-rw-r--  2.0 unx      660 b- defN 22-Sep-28 14:35 hat_chatter-0.5.8.dist-info/RECORD
-8 files, 30800 bytes uncompressed, 9684 bytes compressed:  68.6%
+-rw-r--r--  2.0 unx    11358 b- defN 22-Oct-14 00:26 hat_chatter-0.5.9.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1929 b- defN 22-Oct-14 00:26 hat_chatter-0.5.9.dist-info/METADATA
+-rw-r--r--  2.0 unx      132 b- defN 22-Oct-14 00:26 hat_chatter-0.5.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx        4 b- defN 22-Oct-14 00:26 hat_chatter-0.5.9.dist-info/top_level.txt
+-rw-r--r--  2.0 unx        1 b- defN 22-Oct-14 00:26 hat_chatter-0.5.9.dist-info/zip-safe
+?rw-rw-r--  2.0 unx      660 b- defN 22-Oct-14 00:26 hat_chatter-0.5.9.dist-info/RECORD
+8 files, 30867 bytes uncompressed, 9711 bytes compressed:  68.5%
```

## zipnote {}

```diff
@@ -1,25 +1,25 @@
 Filename: hat/chatter/__init__.py
 Comment: 
 
 Filename: hat/chatter/sbs_repo.json
 Comment: 
 
-Filename: hat_chatter-0.5.8.dist-info/LICENSE
+Filename: hat_chatter-0.5.9.dist-info/LICENSE
 Comment: 
 
-Filename: hat_chatter-0.5.8.dist-info/METADATA
+Filename: hat_chatter-0.5.9.dist-info/METADATA
 Comment: 
 
-Filename: hat_chatter-0.5.8.dist-info/WHEEL
+Filename: hat_chatter-0.5.9.dist-info/WHEEL
 Comment: 
 
-Filename: hat_chatter-0.5.8.dist-info/top_level.txt
+Filename: hat_chatter-0.5.9.dist-info/top_level.txt
 Comment: 
 
-Filename: hat_chatter-0.5.8.dist-info/zip-safe
+Filename: hat_chatter-0.5.9.dist-info/zip-safe
 Comment: 
 
-Filename: hat_chatter-0.5.8.dist-info/RECORD
+Filename: hat_chatter-0.5.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## hat/chatter/__init__.py

```diff
@@ -5,14 +5,15 @@
 To implement communication with other Hat components, user should always
 implement independent communication service (or use one of predefined
 services).
 
 """
 
 import asyncio
+import contextlib
 import importlib.resources
 import logging
 import math
 import ssl
 import typing
 import urllib.parse
 
@@ -429,15 +430,16 @@
         self._writer.write(msg_len_len_bytes + msg_len_bytes + msg_bytes)
 
     async def drain(self):
         await self._writer.drain()
 
     async def async_close(self):
         self._writer.close()
-        await self._writer.wait_closed()
+        with contextlib.suppress(Exception):
+            await self._writer.wait_closed()
 
 
 def _sock_info_to_address(sock_info, scheme):
     host, port = sock_info[0], sock_info[1]
     if ':' in host:
         host = '[' + host + ']'
     return '{}://{}:{}'.format(scheme, host, port)
```

## Comparing `hat_chatter-0.5.8.dist-info/LICENSE` & `hat_chatter-0.5.9.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `hat_chatter-0.5.8.dist-info/METADATA` & `hat_chatter-0.5.9.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hat-chatter
-Version: 0.5.8
+Version: 0.5.9
 Summary: Hat Chatter protocol
 Home-page: https://github.com/hat-open/hat-chatter
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
```

