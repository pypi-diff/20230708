# Comparing `tmp/apibara-0.6.7.tar.gz` & `tmp/apibara-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apibara-0.6.7.tar", max compression
+gzip compressed data, was "apibara-0.7.0.tar", max compression
```

## Comparing `apibara-0.6.7.tar` & `apibara-0.7.0.tar`

### file list

```diff
@@ -1,38 +1,37 @@
--rw-r--r--   0        0        0    11358 2023-01-15 18:52:09.124336 apibara-0.6.7/LICENSE.txt
--rw-r--r--   0        0        0     1342 2023-01-18 12:16:07.977321 apibara-0.6.7/README.rst
--rw-r--r--   0        0        0     1073 2023-06-08 12:56:25.054784 apibara-0.6.7/pyproject.toml
--rw-r--r--   0        0        0        0 2023-01-15 18:52:09.124336 apibara-0.6.7/src/apibara/__init__.py
--rw-r--r--   0        0        0      514 2023-01-15 18:52:09.124336 apibara-0.6.7/src/apibara/cursor.py
--rw-r--r--   0        0        0      160 2023-01-15 18:52:09.124336 apibara-0.6.7/src/apibara/indexer/__init__.py
--rw-r--r--   0        0        0      375 2023-01-15 18:52:09.124336 apibara-0.6.7/src/apibara/indexer/configuration.py
--rw-r--r--   0        0        0     2393 2023-03-16 21:14:54.127582 apibara-0.6.7/src/apibara/indexer/indexer.py
--rw-r--r--   0        0        0     1026 2023-01-16 18:48:50.663792 apibara-0.6.7/src/apibara/indexer/info.py
--rw-r--r--   0        0        0    10488 2023-03-26 09:46:17.305447 apibara-0.6.7/src/apibara/indexer/runner.py
--rw-r--r--   0        0        0    10502 2023-06-08 12:55:13.026953 apibara-0.6.7/src/apibara/indexer/storage.py
--rw-r--r--   0        0        0      687 2023-03-20 22:42:06.349998 apibara-0.6.7/src/apibara/protocol/__init__.py
--rw-r--r--   0        0        0     3521 2023-03-20 22:42:06.414999 apibara-0.6.7/src/apibara/protocol/client.py
--rw-r--r--   0        0        0        0 2023-01-15 18:52:09.125336 apibara-0.6.7/src/apibara/protocol/proto/__init__.py
--rw-r--r--   0        0        0     3107 2023-01-15 18:52:09.125336 apibara-0.6.7/src/apibara/protocol/proto/stream_pb2.py
--rw-r--r--   0        0        0     9814 2023-01-15 18:52:09.125336 apibara-0.6.7/src/apibara/protocol/proto/stream_pb2.pyi
--rw-r--r--   0        0        0     2517 2023-01-15 18:52:09.125336 apibara-0.6.7/src/apibara/protocol/proto/stream_pb2_grpc.py
--rw-r--r--   0        0        0      878 2023-01-15 18:52:09.125336 apibara-0.6.7/src/apibara/protocol/proto/stream_pb2_grpc.pyi
--rw-r--r--   0        0        0      264 2023-01-15 18:52:09.125336 apibara-0.6.7/src/apibara/starknet/__init__.py
--rw-r--r--   0        0        0     1038 2023-01-15 18:52:09.125336 apibara-0.6.7/src/apibara/starknet/cursor.py
--rw-r--r--   0        0        0     1375 2023-01-15 18:52:09.125336 apibara-0.6.7/src/apibara/starknet/felt.py
--rw-r--r--   0        0        0    14725 2023-03-16 21:14:54.127582 apibara-0.6.7/src/apibara/starknet/filter.py
--rw-r--r--   0        0        0      404 2023-01-15 18:52:09.125336 apibara-0.6.7/src/apibara/starknet/indexer.py
--rw-r--r--   0        0        0        0 2023-01-15 18:52:09.125336 apibara-0.6.7/src/apibara/starknet/proto/__init__.py
--rw-r--r--   0        0        0     7060 2023-01-18 12:09:05.990737 apibara-0.6.7/src/apibara/starknet/proto/filter_pb2.py
--rw-r--r--   0        0        0    11215 2023-01-18 12:08:22.304579 apibara-0.6.7/src/apibara/starknet/proto/filter_pb2.pyi
--rw-r--r--   0        0        0      158 2023-01-15 18:52:09.125336 apibara-0.6.7/src/apibara/starknet/proto/filter_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-01-15 18:52:09.125336 apibara-0.6.7/src/apibara/starknet/proto/filter_pb2_grpc.pyi
--rw-r--r--   0        0        0    10601 2023-03-20 22:42:06.408999 apibara-0.6.7/src/apibara/starknet/proto/starknet_pb2.py
--rw-r--r--   0        0        0    17756 2023-01-18 12:08:07.126530 apibara-0.6.7/src/apibara/starknet/proto/starknet_pb2.pyi
--rw-r--r--   0        0        0      158 2023-01-15 18:52:09.125336 apibara-0.6.7/src/apibara/starknet/proto/starknet_pb2_grpc.py
--rw-r--r--   0        0        0      100 2023-01-15 18:52:09.125336 apibara-0.6.7/src/apibara/starknet/proto/starknet_pb2_grpc.pyi
--rw-r--r--   0        0        0     1096 2023-01-18 12:07:16.874395 apibara-0.6.7/src/apibara/starknet/proto/types_pb2.py
--rw-r--r--   0        0        0      732 2023-01-18 12:07:16.871395 apibara-0.6.7/src/apibara/starknet/proto/types_pb2.pyi
--rw-r--r--   0        0        0      158 2023-01-15 18:52:09.125336 apibara-0.6.7/src/apibara/starknet/proto/types_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-01-15 18:52:09.125336 apibara-0.6.7/src/apibara/starknet/proto/types_pb2_grpc.pyi
--rw-r--r--   0        0        0     2386 1970-01-01 00:00:00.000000 apibara-0.6.7/setup.py
--rw-r--r--   0        0        0     2408 1970-01-01 00:00:00.000000 apibara-0.6.7/PKG-INFO
+-rw-r--r--   0        0        0    11358 2023-01-15 18:52:09.124336 apibara-0.7.0/LICENSE.txt
+-rw-r--r--   0        0        0     1342 2023-01-18 12:16:07.977321 apibara-0.7.0/README.rst
+-rw-r--r--   0        0        0     1073 2023-07-08 12:11:24.025439 apibara-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-01-15 18:52:09.124336 apibara-0.7.0/src/apibara/__init__.py
+-rw-r--r--   0        0        0      514 2023-01-15 18:52:09.124336 apibara-0.7.0/src/apibara/cursor.py
+-rw-r--r--   0        0        0      160 2023-01-15 18:52:09.124336 apibara-0.7.0/src/apibara/indexer/__init__.py
+-rw-r--r--   0        0        0      375 2023-01-15 18:52:09.124336 apibara-0.7.0/src/apibara/indexer/configuration.py
+-rw-r--r--   0        0        0     2393 2023-03-16 21:14:54.127582 apibara-0.7.0/src/apibara/indexer/indexer.py
+-rw-r--r--   0        0        0     1026 2023-01-16 18:48:50.663792 apibara-0.7.0/src/apibara/indexer/info.py
+-rw-r--r--   0        0        0    10488 2023-07-08 12:11:24.025439 apibara-0.7.0/src/apibara/indexer/runner.py
+-rw-r--r--   0        0        0    10502 2023-06-08 12:55:13.026953 apibara-0.7.0/src/apibara/indexer/storage.py
+-rw-r--r--   0        0        0      697 2023-07-08 12:11:24.025439 apibara-0.7.0/src/apibara/protocol/__init__.py
+-rw-r--r--   0        0        0     3596 2023-07-08 12:11:24.025439 apibara-0.7.0/src/apibara/protocol/client.py
+-rw-r--r--   0        0        0        0 2023-01-15 18:52:09.125336 apibara-0.7.0/src/apibara/protocol/proto/__init__.py
+-rw-r--r--   0        0        0     3107 2023-01-15 18:52:09.125336 apibara-0.7.0/src/apibara/protocol/proto/stream_pb2.py
+-rw-r--r--   0        0        0     9814 2023-01-15 18:52:09.125336 apibara-0.7.0/src/apibara/protocol/proto/stream_pb2.pyi
+-rw-r--r--   0        0        0     2517 2023-01-15 18:52:09.125336 apibara-0.7.0/src/apibara/protocol/proto/stream_pb2_grpc.py
+-rw-r--r--   0        0        0      878 2023-01-15 18:52:09.125336 apibara-0.7.0/src/apibara/protocol/proto/stream_pb2_grpc.pyi
+-rw-r--r--   0        0        0      264 2023-01-15 18:52:09.125336 apibara-0.7.0/src/apibara/starknet/__init__.py
+-rw-r--r--   0        0        0     1038 2023-01-15 18:52:09.125336 apibara-0.7.0/src/apibara/starknet/cursor.py
+-rw-r--r--   0        0        0     1375 2023-01-15 18:52:09.125336 apibara-0.7.0/src/apibara/starknet/felt.py
+-rw-r--r--   0        0        0    14725 2023-03-16 21:14:54.127582 apibara-0.7.0/src/apibara/starknet/filter.py
+-rw-r--r--   0        0        0      404 2023-01-15 18:52:09.125336 apibara-0.7.0/src/apibara/starknet/indexer.py
+-rw-r--r--   0        0        0        0 2023-01-15 18:52:09.125336 apibara-0.7.0/src/apibara/starknet/proto/__init__.py
+-rw-r--r--   0        0        0     7836 2023-07-08 12:11:24.025439 apibara-0.7.0/src/apibara/starknet/proto/filter_pb2.py
+-rw-r--r--   0        0        0    12814 2023-07-08 12:11:24.025439 apibara-0.7.0/src/apibara/starknet/proto/filter_pb2.pyi
+-rw-r--r--   0        0        0      158 2023-01-15 18:52:09.125336 apibara-0.7.0/src/apibara/starknet/proto/filter_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-01-15 18:52:09.125336 apibara-0.7.0/src/apibara/starknet/proto/filter_pb2_grpc.pyi
+-rw-r--r--   0        0        0    11734 2023-07-08 12:11:24.025439 apibara-0.7.0/src/apibara/starknet/proto/starknet_pb2.py
+-rw-r--r--   0        0        0    20085 2023-07-08 12:11:24.025439 apibara-0.7.0/src/apibara/starknet/proto/starknet_pb2.pyi
+-rw-r--r--   0        0        0      158 2023-01-15 18:52:09.125336 apibara-0.7.0/src/apibara/starknet/proto/starknet_pb2_grpc.py
+-rw-r--r--   0        0        0      100 2023-01-15 18:52:09.125336 apibara-0.7.0/src/apibara/starknet/proto/starknet_pb2_grpc.pyi
+-rw-r--r--   0        0        0     1096 2023-06-30 17:37:45.778732 apibara-0.7.0/src/apibara/starknet/proto/types_pb2.py
+-rw-r--r--   0        0        0      732 2023-06-30 17:37:45.775732 apibara-0.7.0/src/apibara/starknet/proto/types_pb2.pyi
+-rw-r--r--   0        0        0      158 2023-01-15 18:52:09.125336 apibara-0.7.0/src/apibara/starknet/proto/types_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-01-15 18:52:09.125336 apibara-0.7.0/src/apibara/starknet/proto/types_pb2_grpc.pyi
+-rw-r--r--   0        0        0     2408 1970-01-01 00:00:00.000000 apibara-0.7.0/PKG-INFO
```

### Comparing `apibara-0.6.7/LICENSE.txt` & `apibara-0.7.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `apibara-0.6.7/README.rst` & `apibara-0.7.0/README.rst`

 * *Files identical despite different names*

### Comparing `apibara-0.6.7/pyproject.toml` & `apibara-0.7.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "apibara"
-version = "0.6.7"
+version = "0.7.0"
 description = "Apibara cliend SDK. Stream and transform on-chain data with Python."
 authors = ["Francesco Ceccon <francesco@apibara.com>"]
 license = "Apache-2.0"
 readme = "README.rst"
 homepage = "https://www.apibara.com"
 repository= "https://github.com/apibara/python-sdk"
 keywords = [
```

### Comparing `apibara-0.6.7/src/apibara/cursor.py` & `apibara-0.7.0/src/apibara/cursor.py`

 * *Files identical despite different names*

### Comparing `apibara-0.6.7/src/apibara/indexer/indexer.py` & `apibara-0.7.0/src/apibara/indexer/indexer.py`

 * *Files identical despite different names*

### Comparing `apibara-0.6.7/src/apibara/indexer/info.py` & `apibara-0.7.0/src/apibara/indexer/info.py`

 * *Files identical despite different names*

### Comparing `apibara-0.6.7/src/apibara/indexer/runner.py` & `apibara-0.7.0/src/apibara/indexer/runner.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from grpc import ssl_channel_credentials
 from grpc.aio import insecure_channel, secure_channel
 
 from apibara.indexer.indexer import Indexer
 from apibara.indexer.info import Info, UserContext
 from apibara.indexer.storage import Filter, IndexerStorage
 from apibara.protocol import StreamService, credentials_with_auth_token
-from apibara.protocol.proto.stream_pb2 import DataFinality, Cursor
+from apibara.protocol.proto.stream_pb2 import Cursor, DataFinality
 
 logger = logging.getLogger(__name__)
 
 
 MAX_MESSAGE_LENGTH = 100 * 1024 * 1024
 
 DEFAULT_CLIENT_OPTIONS = [
```

### Comparing `apibara-0.6.7/src/apibara/indexer/storage.py` & `apibara-0.7.0/src/apibara/indexer/storage.py`

 * *Files identical despite different names*

### Comparing `apibara-0.6.7/src/apibara/protocol/__init__.py` & `apibara-0.7.0/src/apibara/protocol/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,14 @@
 from dataclasses import dataclass
 from typing import ClassVar
 
-from .client import (
-    BearerTokenAuth,
-    StreamClient,
-    StreamIter,
-    StreamService,
-    credentials_with_auth_token,
-)
-from .proto.stream_pb2 import (
-    Cursor,
-    DataFinality,
-    StreamDataRequest,
-    StreamDataResponse,
-)
+from .client import (BearerTokenAuth, StreamClient, StreamIter, StreamService,
+                     credentials_with_auth_token)
+from .proto.stream_pb2 import (Cursor, DataFinality, StreamDataRequest,
+                               StreamDataResponse)
 
 
 @dataclass
 class StarkNetStreamAddress:
     Mainnet: ClassVar[str] = "mainnet.starknet.a5a.ch"
     Goerli: ClassVar[str] = "goerli.starknet.a5a.ch"
     Goerli2: ClassVar[str] = "goerli-2.starknet.a5a.ch"
```

### Comparing `apibara-0.6.7/src/apibara/protocol/client.py` & `apibara-0.7.0/src/apibara/protocol/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,17 @@
 import asyncio
 from asyncio.queues import Queue
 from typing import AsyncIterable, Iterable, Optional, Tuple, Union
 
 import grpc
 from grpc.aio import Channel
 
-from apibara.protocol.proto.stream_pb2 import (
-    Cursor,
-    DataFinality,
-    StreamDataRequest,
-    StreamDataResponse,
-)
+from apibara.protocol.proto.stream_pb2 import (Cursor, DataFinality,
+                                               StreamDataRequest,
+                                               StreamDataResponse)
 from apibara.protocol.proto.stream_pb2_grpc import StreamStub
 
 DEFAULT_TIMEOUT = 45.0
 
 
 class BearerTokenAuth(grpc.AuthMetadataPlugin):
     def __init__(self, token: str):
```

### Comparing `apibara-0.6.7/src/apibara/protocol/proto/stream_pb2.py` & `apibara-0.7.0/src/apibara/protocol/proto/stream_pb2.py`

 * *Files identical despite different names*

### Comparing `apibara-0.6.7/src/apibara/protocol/proto/stream_pb2.pyi` & `apibara-0.7.0/src/apibara/protocol/proto/stream_pb2.pyi`

 * *Files identical despite different names*

### Comparing `apibara-0.6.7/src/apibara/protocol/proto/stream_pb2_grpc.py` & `apibara-0.7.0/src/apibara/protocol/proto/stream_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `apibara-0.6.7/src/apibara/protocol/proto/stream_pb2_grpc.pyi` & `apibara-0.7.0/src/apibara/protocol/proto/stream_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `apibara-0.6.7/src/apibara/starknet/cursor.py` & `apibara-0.7.0/src/apibara/starknet/cursor.py`

 * *Files identical despite different names*

### Comparing `apibara-0.6.7/src/apibara/starknet/felt.py` & `apibara-0.7.0/src/apibara/starknet/felt.py`

 * *Files identical despite different names*

### Comparing `apibara-0.6.7/src/apibara/starknet/filter.py` & `apibara-0.7.0/src/apibara/starknet/filter.py`

 * *Files identical despite different names*

### Comparing `apibara-0.6.7/src/apibara/starknet/proto/filter_pb2.py` & `apibara-0.7.0/src/apibara/starknet/proto/filter_pb2.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,18 +8,16 @@
 from google.protobuf.internal import builder as _builder
 
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
-import apibara.starknet.proto.types_pb2 as types__pb2
-
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(
-    b"\n\x0c\x66ilter.proto\x12\x19\x61pibara.starknet.v1alpha2\x1a\x0btypes.proto\"\xc3\x02\n\x06\x46ilter\x12\x37\n\x06header\x18\x01 \x01(\x0b\x32'.apibara.starknet.v1alpha2.HeaderFilter\x12\x42\n\x0ctransactions\x18\x02 \x03(\x0b\x32,.apibara.starknet.v1alpha2.TransactionFilter\x12\x42\n\x0cstate_update\x18\x03 \x01(\x0b\x32,.apibara.starknet.v1alpha2.StateUpdateFilter\x12\x36\n\x06\x65vents\x18\x04 \x03(\x0b\x32&.apibara.starknet.v1alpha2.EventFilter\x12@\n\x08messages\x18\x05 \x03(\x0b\x32..apibara.starknet.v1alpha2.L2ToL1MessageFilter\"\x1c\n\x0cHeaderFilter\x12\x0c\n\x04weak\x18\x01 \x01(\x08\"\xe3\x03\n\x11TransactionFilter\x12I\n\tinvoke_v0\x18\x01 \x01(\x0b\x32\x34.apibara.starknet.v1alpha2.InvokeTransactionV0FilterH\x00\x12I\n\tinvoke_v1\x18\x02 \x01(\x0b\x32\x34.apibara.starknet.v1alpha2.InvokeTransactionV1FilterH\x00\x12\x44\n\x06\x64\x65ploy\x18\x03 \x01(\x0b\x32\x32.apibara.starknet.v1alpha2.DeployTransactionFilterH\x00\x12\x46\n\x07\x64\x65\x63lare\x18\x04 \x01(\x0b\x32\x33.apibara.starknet.v1alpha2.DeclareTransactionFilterH\x00\x12K\n\nl1_handler\x18\x05 \x01(\x0b\x32\x35.apibara.starknet.v1alpha2.L1HandlerTransactionFilterH\x00\x12S\n\x0e\x64\x65ploy_account\x18\x06 \x01(\x0b\x32\x39.apibara.starknet.v1alpha2.DeployAccountTransactionFilterH\x00\x42\x08\n\x06\x66ilter\"\xe0\x01\n\x19InvokeTransactionV0Filter\x12\x41\n\x10\x63ontract_address\x18\x01 \x01(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\x12\x45\n\x14\x65ntry_point_selector\x18\x02 \x01(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\x12\x39\n\x08\x63\x61lldata\x18\x03 \x03(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\"\x97\x01\n\x19InvokeTransactionV1Filter\x12?\n\x0esender_address\x18\x01 \x01(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\x12\x39\n\x08\x63\x61lldata\x18\x03 \x03(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\"\xe5\x01\n\x17\x44\x65ployTransactionFilter\x12\x46\n\x15\x63ontract_address_salt\x18\x01 \x01(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\x12;\n\nclass_hash\x18\x02 \x01(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\x12\x45\n\x14\x63onstructor_calldata\x18\x04 \x03(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\"\x98\x01\n\x18\x44\x65\x63lareTransactionFilter\x12;\n\nclass_hash\x18\x01 \x01(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\x12?\n\x0esender_address\x18\x02 \x01(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\"\xe1\x01\n\x1aL1HandlerTransactionFilter\x12\x41\n\x10\x63ontract_address\x18\x01 \x01(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\x12\x45\n\x14\x65ntry_point_selector\x18\x02 \x01(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\x12\x39\n\x08\x63\x61lldata\x18\x03 \x03(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\"\xec\x01\n\x1e\x44\x65ployAccountTransactionFilter\x12\x46\n\x15\x63ontract_address_salt\x18\x01 \x01(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\x12;\n\nclass_hash\x18\x02 \x01(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\x12\x45\n\x14\x63onstructor_calldata\x18\x04 \x03(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\"\x8c\x01\n\x13L2ToL1MessageFilter\x12;\n\nto_address\x18\x01 \x01(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\x12\x38\n\x07payload\x18\x02 \x03(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\"\xba\x01\n\x0b\x45ventFilter\x12=\n\x0c\x66rom_address\x18\x01 \x01(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\x12\x35\n\x04keys\x18\x02 \x03(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\x12\x35\n\x04\x64\x61ta\x18\x03 \x03(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\"\xb4\x02\n\x11StateUpdateFilter\x12\x43\n\rstorage_diffs\x18\x01 \x03(\x0b\x32,.apibara.starknet.v1alpha2.StorageDiffFilter\x12M\n\x12\x64\x65\x63lared_contracts\x18\x02 \x03(\x0b\x32\x31.apibara.starknet.v1alpha2.DeclaredContractFilter\x12M\n\x12\x64\x65ployed_contracts\x18\x03 \x03(\x0b\x32\x31.apibara.starknet.v1alpha2.DeployedContractFilter\x12<\n\x06nonces\x18\x04 \x03(\x0b\x32,.apibara.starknet.v1alpha2.NonceUpdateFilter\"V\n\x11StorageDiffFilter\x12\x41\n\x10\x63ontract_address\x18\x01 \x01(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\"U\n\x16\x44\x65\x63laredContractFilter\x12;\n\nclass_hash\x18\x01 \x01(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\"\x98\x01\n\x16\x44\x65ployedContractFilter\x12\x41\n\x10\x63ontract_address\x18\x01 \x01(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\x12;\n\nclass_hash\x18\x02 \x01(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\"\x8e\x01\n\x11NonceUpdateFilter\x12\x41\n\x10\x63ontract_address\x18\x01 \x01(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\x12\x36\n\x05nonce\x18\x02 \x01(\x0b\x32'.apibara.starknet.v1alpha2.FieldElementb\x06proto3"
+    b"\n\x0c\x66ilter.proto\x12\x19\x61pibara.starknet.v1alpha2\x1a\x0btypes.proto\"\xc3\x02\n\x06\x46ilter\x12\x37\n\x06header\x18\x01 \x01(\x0b\x32'.apibara.starknet.v1alpha2.HeaderFilter\x12\x42\n\x0ctransactions\x18\x02 \x03(\x0b\x32,.apibara.starknet.v1alpha2.TransactionFilter\x12\x42\n\x0cstate_update\x18\x03 \x01(\x0b\x32,.apibara.starknet.v1alpha2.StateUpdateFilter\x12\x36\n\x06\x65vents\x18\x04 \x03(\x0b\x32&.apibara.starknet.v1alpha2.EventFilter\x12@\n\x08messages\x18\x05 \x03(\x0b\x32..apibara.starknet.v1alpha2.L2ToL1MessageFilter\"\x1c\n\x0cHeaderFilter\x12\x0c\n\x04weak\x18\x01 \x01(\x08\"\xe3\x03\n\x11TransactionFilter\x12I\n\tinvoke_v0\x18\x01 \x01(\x0b\x32\x34.apibara.starknet.v1alpha2.InvokeTransactionV0FilterH\x00\x12I\n\tinvoke_v1\x18\x02 \x01(\x0b\x32\x34.apibara.starknet.v1alpha2.InvokeTransactionV1FilterH\x00\x12\x44\n\x06\x64\x65ploy\x18\x03 \x01(\x0b\x32\x32.apibara.starknet.v1alpha2.DeployTransactionFilterH\x00\x12\x46\n\x07\x64\x65\x63lare\x18\x04 \x01(\x0b\x32\x33.apibara.starknet.v1alpha2.DeclareTransactionFilterH\x00\x12K\n\nl1_handler\x18\x05 \x01(\x0b\x32\x35.apibara.starknet.v1alpha2.L1HandlerTransactionFilterH\x00\x12S\n\x0e\x64\x65ploy_account\x18\x06 \x01(\x0b\x32\x39.apibara.starknet.v1alpha2.DeployAccountTransactionFilterH\x00\x42\x08\n\x06\x66ilter\"\xe0\x01\n\x19InvokeTransactionV0Filter\x12\x41\n\x10\x63ontract_address\x18\x01 \x01(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\x12\x45\n\x14\x65ntry_point_selector\x18\x02 \x01(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\x12\x39\n\x08\x63\x61lldata\x18\x03 \x03(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\"\x97\x01\n\x19InvokeTransactionV1Filter\x12?\n\x0esender_address\x18\x01 \x01(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\x12\x39\n\x08\x63\x61lldata\x18\x03 \x03(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\"\xe5\x01\n\x17\x44\x65ployTransactionFilter\x12\x46\n\x15\x63ontract_address_salt\x18\x01 \x01(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\x12;\n\nclass_hash\x18\x02 \x01(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\x12\x45\n\x14\x63onstructor_calldata\x18\x04 \x03(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\"\x98\x01\n\x18\x44\x65\x63lareTransactionFilter\x12;\n\nclass_hash\x18\x01 \x01(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\x12?\n\x0esender_address\x18\x02 \x01(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\"\xe1\x01\n\x1aL1HandlerTransactionFilter\x12\x41\n\x10\x63ontract_address\x18\x01 \x01(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\x12\x45\n\x14\x65ntry_point_selector\x18\x02 \x01(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\x12\x39\n\x08\x63\x61lldata\x18\x03 \x03(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\"\xec\x01\n\x1e\x44\x65ployAccountTransactionFilter\x12\x46\n\x15\x63ontract_address_salt\x18\x01 \x01(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\x12;\n\nclass_hash\x18\x02 \x01(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\x12\x45\n\x14\x63onstructor_calldata\x18\x04 \x03(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\"\x8c\x01\n\x13L2ToL1MessageFilter\x12;\n\nto_address\x18\x01 \x01(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\x12\x38\n\x07payload\x18\x02 \x03(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\"\xba\x01\n\x0b\x45ventFilter\x12=\n\x0c\x66rom_address\x18\x01 \x01(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\x12\x35\n\x04keys\x18\x02 \x03(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\x12\x35\n\x04\x64\x61ta\x18\x03 \x03(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\"\xc8\x03\n\x11StateUpdateFilter\x12\x43\n\rstorage_diffs\x18\x01 \x03(\x0b\x32,.apibara.starknet.v1alpha2.StorageDiffFilter\x12M\n\x12\x64\x65\x63lared_contracts\x18\x02 \x03(\x0b\x32\x31.apibara.starknet.v1alpha2.DeclaredContractFilter\x12M\n\x12\x64\x65ployed_contracts\x18\x03 \x03(\x0b\x32\x31.apibara.starknet.v1alpha2.DeployedContractFilter\x12<\n\x06nonces\x18\x04 \x03(\x0b\x32,.apibara.starknet.v1alpha2.NonceUpdateFilter\x12H\n\x10\x64\x65\x63lared_classes\x18\x05 \x03(\x0b\x32..apibara.starknet.v1alpha2.DeclaredClassFilter\x12H\n\x10replaced_classes\x18\x06 \x03(\x0b\x32..apibara.starknet.v1alpha2.ReplacedClassFilter\"V\n\x11StorageDiffFilter\x12\x41\n\x10\x63ontract_address\x18\x01 \x01(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\"U\n\x16\x44\x65\x63laredContractFilter\x12;\n\nclass_hash\x18\x01 \x01(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\"\x98\x01\n\x13\x44\x65\x63laredClassFilter\x12;\n\nclass_hash\x18\x01 \x01(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\x12\x44\n\x13\x63ompiled_class_hash\x18\x02 \x01(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\"\x95\x01\n\x13ReplacedClassFilter\x12\x41\n\x10\x63ontract_address\x18\x01 \x01(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\x12;\n\nclass_hash\x18\x02 \x01(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\"\x98\x01\n\x16\x44\x65ployedContractFilter\x12\x41\n\x10\x63ontract_address\x18\x01 \x01(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\x12;\n\nclass_hash\x18\x02 \x01(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\"\x8e\x01\n\x11NonceUpdateFilter\x12\x41\n\x10\x63ontract_address\x18\x01 \x01(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\x12\x36\n\x05nonce\x18\x02 \x01(\x0b\x32'.apibara.starknet.v1alpha2.FieldElementb\x06proto3"
 )
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, "filter_pb2", globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
     DESCRIPTOR._options = None
@@ -42,17 +40,21 @@
     _DEPLOYACCOUNTTRANSACTIONFILTER._serialized_start = 1895
     _DEPLOYACCOUNTTRANSACTIONFILTER._serialized_end = 2131
     _L2TOL1MESSAGEFILTER._serialized_start = 2134
     _L2TOL1MESSAGEFILTER._serialized_end = 2274
     _EVENTFILTER._serialized_start = 2277
     _EVENTFILTER._serialized_end = 2463
     _STATEUPDATEFILTER._serialized_start = 2466
-    _STATEUPDATEFILTER._serialized_end = 2774
-    _STORAGEDIFFFILTER._serialized_start = 2776
-    _STORAGEDIFFFILTER._serialized_end = 2862
-    _DECLAREDCONTRACTFILTER._serialized_start = 2864
-    _DECLAREDCONTRACTFILTER._serialized_end = 2949
-    _DEPLOYEDCONTRACTFILTER._serialized_start = 2952
-    _DEPLOYEDCONTRACTFILTER._serialized_end = 3104
-    _NONCEUPDATEFILTER._serialized_start = 3107
-    _NONCEUPDATEFILTER._serialized_end = 3249
+    _STATEUPDATEFILTER._serialized_end = 2922
+    _STORAGEDIFFFILTER._serialized_start = 2924
+    _STORAGEDIFFFILTER._serialized_end = 3010
+    _DECLAREDCONTRACTFILTER._serialized_start = 3012
+    _DECLAREDCONTRACTFILTER._serialized_end = 3097
+    _DECLAREDCLASSFILTER._serialized_start = 3100
+    _DECLAREDCLASSFILTER._serialized_end = 3252
+    _REPLACEDCLASSFILTER._serialized_start = 3255
+    _REPLACEDCLASSFILTER._serialized_end = 3404
+    _DEPLOYEDCONTRACTFILTER._serialized_start = 3407
+    _DEPLOYEDCONTRACTFILTER._serialized_end = 3559
+    _NONCEUPDATEFILTER._serialized_start = 3562
+    _NONCEUPDATEFILTER._serialized_end = 3704
 # @@protoc_insertion_point(module_scope)
```

### Comparing `apibara-0.6.7/src/apibara/starknet/proto/filter_pb2.pyi` & `apibara-0.7.0/src/apibara/starknet/proto/filter_pb2.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -20,14 +20,26 @@
     sender_address: _types_pb2.FieldElement
     def __init__(
         self,
         class_hash: _Optional[_Union[_types_pb2.FieldElement, _Mapping]] = ...,
         sender_address: _Optional[_Union[_types_pb2.FieldElement, _Mapping]] = ...,
     ) -> None: ...
 
+class DeclaredClassFilter(_message.Message):
+    __slots__ = ["class_hash", "compiled_class_hash"]
+    CLASS_HASH_FIELD_NUMBER: _ClassVar[int]
+    COMPILED_CLASS_HASH_FIELD_NUMBER: _ClassVar[int]
+    class_hash: _types_pb2.FieldElement
+    compiled_class_hash: _types_pb2.FieldElement
+    def __init__(
+        self,
+        class_hash: _Optional[_Union[_types_pb2.FieldElement, _Mapping]] = ...,
+        compiled_class_hash: _Optional[_Union[_types_pb2.FieldElement, _Mapping]] = ...,
+    ) -> None: ...
+
 class DeclaredContractFilter(_message.Message):
     __slots__ = ["class_hash"]
     CLASS_HASH_FIELD_NUMBER: _ClassVar[int]
     class_hash: _types_pb2.FieldElement
     def __init__(
         self, class_hash: _Optional[_Union[_types_pb2.FieldElement, _Mapping]] = ...
     ) -> None: ...
@@ -194,38 +206,67 @@
     nonce: _types_pb2.FieldElement
     def __init__(
         self,
         contract_address: _Optional[_Union[_types_pb2.FieldElement, _Mapping]] = ...,
         nonce: _Optional[_Union[_types_pb2.FieldElement, _Mapping]] = ...,
     ) -> None: ...
 
+class ReplacedClassFilter(_message.Message):
+    __slots__ = ["class_hash", "contract_address"]
+    CLASS_HASH_FIELD_NUMBER: _ClassVar[int]
+    CONTRACT_ADDRESS_FIELD_NUMBER: _ClassVar[int]
+    class_hash: _types_pb2.FieldElement
+    contract_address: _types_pb2.FieldElement
+    def __init__(
+        self,
+        contract_address: _Optional[_Union[_types_pb2.FieldElement, _Mapping]] = ...,
+        class_hash: _Optional[_Union[_types_pb2.FieldElement, _Mapping]] = ...,
+    ) -> None: ...
+
 class StateUpdateFilter(_message.Message):
-    __slots__ = ["declared_contracts", "deployed_contracts", "nonces", "storage_diffs"]
+    __slots__ = [
+        "declared_classes",
+        "declared_contracts",
+        "deployed_contracts",
+        "nonces",
+        "replaced_classes",
+        "storage_diffs",
+    ]
+    DECLARED_CLASSES_FIELD_NUMBER: _ClassVar[int]
     DECLARED_CONTRACTS_FIELD_NUMBER: _ClassVar[int]
     DEPLOYED_CONTRACTS_FIELD_NUMBER: _ClassVar[int]
     NONCES_FIELD_NUMBER: _ClassVar[int]
+    REPLACED_CLASSES_FIELD_NUMBER: _ClassVar[int]
     STORAGE_DIFFS_FIELD_NUMBER: _ClassVar[int]
+    declared_classes: _containers.RepeatedCompositeFieldContainer[DeclaredClassFilter]
     declared_contracts: _containers.RepeatedCompositeFieldContainer[
         DeclaredContractFilter
     ]
     deployed_contracts: _containers.RepeatedCompositeFieldContainer[
         DeployedContractFilter
     ]
     nonces: _containers.RepeatedCompositeFieldContainer[NonceUpdateFilter]
+    replaced_classes: _containers.RepeatedCompositeFieldContainer[ReplacedClassFilter]
     storage_diffs: _containers.RepeatedCompositeFieldContainer[StorageDiffFilter]
     def __init__(
         self,
         storage_diffs: _Optional[_Iterable[_Union[StorageDiffFilter, _Mapping]]] = ...,
         declared_contracts: _Optional[
             _Iterable[_Union[DeclaredContractFilter, _Mapping]]
         ] = ...,
         deployed_contracts: _Optional[
             _Iterable[_Union[DeployedContractFilter, _Mapping]]
         ] = ...,
         nonces: _Optional[_Iterable[_Union[NonceUpdateFilter, _Mapping]]] = ...,
+        declared_classes: _Optional[
+            _Iterable[_Union[DeclaredClassFilter, _Mapping]]
+        ] = ...,
+        replaced_classes: _Optional[
+            _Iterable[_Union[ReplacedClassFilter, _Mapping]]
+        ] = ...,
     ) -> None: ...
 
 class StorageDiffFilter(_message.Message):
     __slots__ = ["contract_address"]
     CONTRACT_ADDRESS_FIELD_NUMBER: _ClassVar[int]
     contract_address: _types_pb2.FieldElement
     def __init__(
```

### Comparing `apibara-0.6.7/src/apibara/starknet/proto/starknet_pb2.py` & `apibara-0.7.0/src/apibara/starknet/proto/starknet_pb2.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,27 +8,28 @@
 from google.protobuf.internal import builder as _builder
 
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
-from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
+from google.protobuf import \
+    timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(
-    b"\n\x0estarknet.proto\x12\x19\x61pibara.starknet.v1alpha2\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x0btypes.proto\"\x93\x03\n\x05\x42lock\x12\x36\n\x06status\x18\x01 \x01(\x0e\x32&.apibara.starknet.v1alpha2.BlockStatus\x12\x36\n\x06header\x18\x02 \x01(\x0b\x32&.apibara.starknet.v1alpha2.BlockHeader\x12G\n\x0ctransactions\x18\x03 \x03(\x0b\x32\x31.apibara.starknet.v1alpha2.TransactionWithReceipt\x12<\n\x0cstate_update\x18\x04 \x01(\x0b\x32&.apibara.starknet.v1alpha2.StateUpdate\x12?\n\x06\x65vents\x18\x05 \x03(\x0b\x32/.apibara.starknet.v1alpha2.EventWithTransaction\x12R\n\x11l2_to_l1_messages\x18\x06 \x03(\x0b\x32\x37.apibara.starknet.v1alpha2.L2ToL1MessageWithTransaction\"\xd2\x02\n\x0b\x42lockHeader\x12;\n\nblock_hash\x18\x01 \x01(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\x12\x42\n\x11parent_block_hash\x18\x02 \x01(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\x12\x14\n\x0c\x62lock_number\x18\x03 \x01(\x04\x12\x42\n\x11sequencer_address\x18\x04 \x01(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\x12\x39\n\x08new_root\x18\x05 \x01(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\x12-\n\ttimestamp\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"\x95\x01\n\x16TransactionWithReceipt\x12;\n\x0btransaction\x18\x01 \x01(\x0b\x32&.apibara.starknet.v1alpha2.Transaction\x12>\n\x07receipt\x18\x02 \x01(\x0b\x32-.apibara.starknet.v1alpha2.TransactionReceipt\"\xf8\x03\n\x0bTransaction\x12\x38\n\x04meta\x18\x01 \x01(\x0b\x32*.apibara.starknet.v1alpha2.TransactionMeta\x12\x43\n\tinvoke_v0\x18\x02 \x01(\x0b\x32..apibara.starknet.v1alpha2.InvokeTransactionV0H\x00\x12\x43\n\tinvoke_v1\x18\x03 \x01(\x0b\x32..apibara.starknet.v1alpha2.InvokeTransactionV1H\x00\x12>\n\x06\x64\x65ploy\x18\x04 \x01(\x0b\x32,.apibara.starknet.v1alpha2.DeployTransactionH\x00\x12@\n\x07\x64\x65\x63lare\x18\x05 \x01(\x0b\x32-.apibara.starknet.v1alpha2.DeclareTransactionH\x00\x12\x45\n\nl1_handler\x18\x06 \x01(\x0b\x32/.apibara.starknet.v1alpha2.L1HandlerTransactionH\x00\x12M\n\x0e\x64\x65ploy_account\x18\x07 \x01(\x0b\x32\x33.apibara.starknet.v1alpha2.DeployAccountTransactionH\x00\x42\r\n\x0btransaction\"\x87\x02\n\x0fTransactionMeta\x12\x35\n\x04hash\x18\x01 \x01(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\x12\x38\n\x07max_fee\x18\x02 \x01(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\x12:\n\tsignature\x18\x03 \x03(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\x12\x36\n\x05nonce\x18\x04 \x01(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\x12\x0f\n\x07version\x18\x05 \x01(\x04\"\xda\x01\n\x13InvokeTransactionV0\x12\x41\n\x10\x63ontract_address\x18\x01 \x01(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\x12\x45\n\x14\x65ntry_point_selector\x18\x02 \x01(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\x12\x39\n\x08\x63\x61lldata\x18\x03 \x03(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\"\x91\x01\n\x13InvokeTransactionV1\x12?\n\x0esender_address\x18\x01 \x01(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\x12\x39\n\x08\x63\x61lldata\x18\x02 \x03(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\"\xdf\x01\n\x11\x44\x65ployTransaction\x12\x45\n\x14\x63onstructor_calldata\x18\x02 \x03(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\x12\x46\n\x15\x63ontract_address_salt\x18\x03 \x01(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\x12;\n\nclass_hash\x18\x04 \x01(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\"\x92\x01\n\x12\x44\x65\x63lareTransaction\x12;\n\nclass_hash\x18\x01 \x01(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\x12?\n\x0esender_address\x18\x02 \x01(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\"\xdb\x01\n\x14L1HandlerTransaction\x12\x41\n\x10\x63ontract_address\x18\x02 \x01(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\x12\x45\n\x14\x65ntry_point_selector\x18\x03 \x01(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\x12\x39\n\x08\x63\x61lldata\x18\x04 \x03(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\"\xe6\x01\n\x18\x44\x65ployAccountTransaction\x12\x45\n\x14\x63onstructor_calldata\x18\x02 \x03(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\x12\x46\n\x15\x63ontract_address_salt\x18\x03 \x01(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\x12;\n\nclass_hash\x18\x04 \x01(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\"\xa6\x02\n\x12TransactionReceipt\x12\x41\n\x10transaction_hash\x18\x01 \x01(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\x12\x19\n\x11transaction_index\x18\x02 \x01(\x04\x12;\n\nactual_fee\x18\x03 \x01(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\x12\x43\n\x11l2_to_l1_messages\x18\x04 \x03(\x0b\x32(.apibara.starknet.v1alpha2.L2ToL1Message\x12\x30\n\x06\x65vents\x18\x05 \x03(\x0b\x32 .apibara.starknet.v1alpha2.Event\"\xd6\x01\n\x1cL2ToL1MessageWithTransaction\x12;\n\x0btransaction\x18\x01 \x01(\x0b\x32&.apibara.starknet.v1alpha2.Transaction\x12>\n\x07receipt\x18\x02 \x01(\x0b\x32-.apibara.starknet.v1alpha2.TransactionReceipt\x12\x39\n\x07message\x18\x03 \x01(\x0b\x32(.apibara.starknet.v1alpha2.L2ToL1Message\"\x86\x01\n\rL2ToL1Message\x12;\n\nto_address\x18\x03 \x01(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\x12\x38\n\x07payload\x18\x04 \x03(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\"\xc4\x01\n\x14\x45ventWithTransaction\x12;\n\x0btransaction\x18\x01 \x01(\x0b\x32&.apibara.starknet.v1alpha2.Transaction\x12>\n\x07receipt\x18\x02 \x01(\x0b\x32-.apibara.starknet.v1alpha2.TransactionReceipt\x12/\n\x05\x65vent\x18\x03 \x01(\x0b\x32 .apibara.starknet.v1alpha2.Event\"\xb4\x01\n\x05\x45vent\x12=\n\x0c\x66rom_address\x18\x01 \x01(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\x12\x35\n\x04keys\x18\x02 \x03(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\x12\x35\n\x04\x64\x61ta\x18\x03 \x03(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\"\xbd\x01\n\x0bStateUpdate\x12\x39\n\x08new_root\x18\x01 \x01(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\x12\x39\n\x08old_root\x18\x02 \x01(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\x12\x38\n\nstate_diff\x18\x03 \x01(\x0b\x32$.apibara.starknet.v1alpha2.StateDiff\"\x94\x02\n\tStateDiff\x12=\n\rstorage_diffs\x18\x01 \x03(\x0b\x32&.apibara.starknet.v1alpha2.StorageDiff\x12G\n\x12\x64\x65\x63lared_contracts\x18\x02 \x03(\x0b\x32+.apibara.starknet.v1alpha2.DeclaredContract\x12G\n\x12\x64\x65ployed_contracts\x18\x03 \x03(\x0b\x32+.apibara.starknet.v1alpha2.DeployedContract\x12\x36\n\x06nonces\x18\x04 \x03(\x0b\x32&.apibara.starknet.v1alpha2.NonceUpdate\"\x92\x01\n\x0bStorageDiff\x12\x41\n\x10\x63ontract_address\x18\x01 \x01(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\x12@\n\x0fstorage_entries\x18\x02 \x03(\x0b\x32'.apibara.starknet.v1alpha2.StorageEntry\"|\n\x0cStorageEntry\x12\x34\n\x03key\x18\x01 \x01(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\x12\x36\n\x05value\x18\x02 \x01(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\"O\n\x10\x44\x65\x63laredContract\x12;\n\nclass_hash\x18\x01 \x01(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\"\x92\x01\n\x10\x44\x65ployedContract\x12\x41\n\x10\x63ontract_address\x18\x01 \x01(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\x12;\n\nclass_hash\x18\x02 \x01(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\"\x88\x01\n\x0bNonceUpdate\x12\x41\n\x10\x63ontract_address\x18\x01 \x01(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\x12\x36\n\x05nonce\x18\x02 \x01(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement*\xa2\x01\n\x0b\x42lockStatus\x12\x1c\n\x18\x42LOCK_STATUS_UNSPECIFIED\x10\x00\x12\x18\n\x14\x42LOCK_STATUS_PENDING\x10\x01\x12\x1f\n\x1b\x42LOCK_STATUS_ACCEPTED_ON_L2\x10\x02\x12\x1f\n\x1b\x42LOCK_STATUS_ACCEPTED_ON_L1\x10\x03\x12\x19\n\x15\x42LOCK_STATUS_REJECTED\x10\x04\x62\x06proto3"
+    b"\n\x0estarknet.proto\x12\x19\x61pibara.starknet.v1alpha2\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x0btypes.proto\"\x93\x03\n\x05\x42lock\x12\x36\n\x06status\x18\x01 \x01(\x0e\x32&.apibara.starknet.v1alpha2.BlockStatus\x12\x36\n\x06header\x18\x02 \x01(\x0b\x32&.apibara.starknet.v1alpha2.BlockHeader\x12G\n\x0ctransactions\x18\x03 \x03(\x0b\x32\x31.apibara.starknet.v1alpha2.TransactionWithReceipt\x12<\n\x0cstate_update\x18\x04 \x01(\x0b\x32&.apibara.starknet.v1alpha2.StateUpdate\x12?\n\x06\x65vents\x18\x05 \x03(\x0b\x32/.apibara.starknet.v1alpha2.EventWithTransaction\x12R\n\x11l2_to_l1_messages\x18\x06 \x03(\x0b\x32\x37.apibara.starknet.v1alpha2.L2ToL1MessageWithTransaction\"\xd2\x02\n\x0b\x42lockHeader\x12;\n\nblock_hash\x18\x01 \x01(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\x12\x42\n\x11parent_block_hash\x18\x02 \x01(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\x12\x14\n\x0c\x62lock_number\x18\x03 \x01(\x04\x12\x42\n\x11sequencer_address\x18\x04 \x01(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\x12\x39\n\x08new_root\x18\x05 \x01(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\x12-\n\ttimestamp\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"\x95\x01\n\x16TransactionWithReceipt\x12;\n\x0btransaction\x18\x01 \x01(\x0b\x32&.apibara.starknet.v1alpha2.Transaction\x12>\n\x07receipt\x18\x02 \x01(\x0b\x32-.apibara.starknet.v1alpha2.TransactionReceipt\"\xf8\x03\n\x0bTransaction\x12\x38\n\x04meta\x18\x01 \x01(\x0b\x32*.apibara.starknet.v1alpha2.TransactionMeta\x12\x43\n\tinvoke_v0\x18\x02 \x01(\x0b\x32..apibara.starknet.v1alpha2.InvokeTransactionV0H\x00\x12\x43\n\tinvoke_v1\x18\x03 \x01(\x0b\x32..apibara.starknet.v1alpha2.InvokeTransactionV1H\x00\x12>\n\x06\x64\x65ploy\x18\x04 \x01(\x0b\x32,.apibara.starknet.v1alpha2.DeployTransactionH\x00\x12@\n\x07\x64\x65\x63lare\x18\x05 \x01(\x0b\x32-.apibara.starknet.v1alpha2.DeclareTransactionH\x00\x12\x45\n\nl1_handler\x18\x06 \x01(\x0b\x32/.apibara.starknet.v1alpha2.L1HandlerTransactionH\x00\x12M\n\x0e\x64\x65ploy_account\x18\x07 \x01(\x0b\x32\x33.apibara.starknet.v1alpha2.DeployAccountTransactionH\x00\x42\r\n\x0btransaction\"\x87\x02\n\x0fTransactionMeta\x12\x35\n\x04hash\x18\x01 \x01(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\x12\x38\n\x07max_fee\x18\x02 \x01(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\x12:\n\tsignature\x18\x03 \x03(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\x12\x36\n\x05nonce\x18\x04 \x01(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\x12\x0f\n\x07version\x18\x05 \x01(\x04\"\xda\x01\n\x13InvokeTransactionV0\x12\x41\n\x10\x63ontract_address\x18\x01 \x01(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\x12\x45\n\x14\x65ntry_point_selector\x18\x02 \x01(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\x12\x39\n\x08\x63\x61lldata\x18\x03 \x03(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\"\x91\x01\n\x13InvokeTransactionV1\x12?\n\x0esender_address\x18\x01 \x01(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\x12\x39\n\x08\x63\x61lldata\x18\x02 \x03(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\"\xdf\x01\n\x11\x44\x65ployTransaction\x12\x45\n\x14\x63onstructor_calldata\x18\x02 \x03(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\x12\x46\n\x15\x63ontract_address_salt\x18\x03 \x01(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\x12;\n\nclass_hash\x18\x04 \x01(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\"\xd8\x01\n\x12\x44\x65\x63lareTransaction\x12;\n\nclass_hash\x18\x01 \x01(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\x12?\n\x0esender_address\x18\x02 \x01(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\x12\x44\n\x13\x63ompiled_class_hash\x18\x03 \x01(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\"\xdb\x01\n\x14L1HandlerTransaction\x12\x41\n\x10\x63ontract_address\x18\x02 \x01(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\x12\x45\n\x14\x65ntry_point_selector\x18\x03 \x01(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\x12\x39\n\x08\x63\x61lldata\x18\x04 \x03(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\"\xe6\x01\n\x18\x44\x65ployAccountTransaction\x12\x45\n\x14\x63onstructor_calldata\x18\x02 \x03(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\x12\x46\n\x15\x63ontract_address_salt\x18\x03 \x01(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\x12;\n\nclass_hash\x18\x04 \x01(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\"\xe9\x02\n\x12TransactionReceipt\x12\x41\n\x10transaction_hash\x18\x01 \x01(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\x12\x19\n\x11transaction_index\x18\x02 \x01(\x04\x12;\n\nactual_fee\x18\x03 \x01(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\x12\x43\n\x11l2_to_l1_messages\x18\x04 \x03(\x0b\x32(.apibara.starknet.v1alpha2.L2ToL1Message\x12\x30\n\x06\x65vents\x18\x05 \x03(\x0b\x32 .apibara.starknet.v1alpha2.Event\x12\x41\n\x10\x63ontract_address\x18\x06 \x01(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\"\xd6\x01\n\x1cL2ToL1MessageWithTransaction\x12;\n\x0btransaction\x18\x01 \x01(\x0b\x32&.apibara.starknet.v1alpha2.Transaction\x12>\n\x07receipt\x18\x02 \x01(\x0b\x32-.apibara.starknet.v1alpha2.TransactionReceipt\x12\x39\n\x07message\x18\x03 \x01(\x0b\x32(.apibara.starknet.v1alpha2.L2ToL1Message\"\xd4\x01\n\rL2ToL1Message\x12;\n\nto_address\x18\x03 \x01(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\x12\x38\n\x07payload\x18\x04 \x03(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\x12\r\n\x05index\x18\x05 \x01(\x04\x12=\n\x0c\x66rom_address\x18\x06 \x01(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\"\xc4\x01\n\x14\x45ventWithTransaction\x12;\n\x0btransaction\x18\x01 \x01(\x0b\x32&.apibara.starknet.v1alpha2.Transaction\x12>\n\x07receipt\x18\x02 \x01(\x0b\x32-.apibara.starknet.v1alpha2.TransactionReceipt\x12/\n\x05\x65vent\x18\x03 \x01(\x0b\x32 .apibara.starknet.v1alpha2.Event\"\xc3\x01\n\x05\x45vent\x12=\n\x0c\x66rom_address\x18\x01 \x01(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\x12\x35\n\x04keys\x18\x02 \x03(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\x12\x35\n\x04\x64\x61ta\x18\x03 \x03(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\x12\r\n\x05index\x18\x04 \x01(\x04\"\xbd\x01\n\x0bStateUpdate\x12\x39\n\x08new_root\x18\x01 \x01(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\x12\x39\n\x08old_root\x18\x02 \x01(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\x12\x38\n\nstate_diff\x18\x03 \x01(\x0b\x32$.apibara.starknet.v1alpha2.StateDiff\"\x9c\x03\n\tStateDiff\x12=\n\rstorage_diffs\x18\x01 \x03(\x0b\x32&.apibara.starknet.v1alpha2.StorageDiff\x12G\n\x12\x64\x65\x63lared_contracts\x18\x02 \x03(\x0b\x32+.apibara.starknet.v1alpha2.DeclaredContract\x12G\n\x12\x64\x65ployed_contracts\x18\x03 \x03(\x0b\x32+.apibara.starknet.v1alpha2.DeployedContract\x12\x36\n\x06nonces\x18\x04 \x03(\x0b\x32&.apibara.starknet.v1alpha2.NonceUpdate\x12\x42\n\x10\x64\x65\x63lared_classes\x18\x05 \x03(\x0b\x32(.apibara.starknet.v1alpha2.DeclaredClass\x12\x42\n\x10replaced_classes\x18\x06 \x03(\x0b\x32(.apibara.starknet.v1alpha2.ReplacedClass\"\x92\x01\n\x0bStorageDiff\x12\x41\n\x10\x63ontract_address\x18\x01 \x01(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\x12@\n\x0fstorage_entries\x18\x02 \x03(\x0b\x32'.apibara.starknet.v1alpha2.StorageEntry\"|\n\x0cStorageEntry\x12\x34\n\x03key\x18\x01 \x01(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\x12\x36\n\x05value\x18\x02 \x01(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\"O\n\x10\x44\x65\x63laredContract\x12;\n\nclass_hash\x18\x01 \x01(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\"\x92\x01\n\rDeclaredClass\x12;\n\nclass_hash\x18\x01 \x01(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\x12\x44\n\x13\x63ompiled_class_hash\x18\x02 \x01(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\"\x8f\x01\n\rReplacedClass\x12\x41\n\x10\x63ontract_address\x18\x01 \x01(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\x12;\n\nclass_hash\x18\x02 \x01(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\"\x92\x01\n\x10\x44\x65ployedContract\x12\x41\n\x10\x63ontract_address\x18\x01 \x01(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\x12;\n\nclass_hash\x18\x02 \x01(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\"\x88\x01\n\x0bNonceUpdate\x12\x41\n\x10\x63ontract_address\x18\x01 \x01(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\x12\x36\n\x05nonce\x18\x02 \x01(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement*\xa2\x01\n\x0b\x42lockStatus\x12\x1c\n\x18\x42LOCK_STATUS_UNSPECIFIED\x10\x00\x12\x18\n\x14\x42LOCK_STATUS_PENDING\x10\x01\x12\x1f\n\x1b\x42LOCK_STATUS_ACCEPTED_ON_L2\x10\x02\x12\x1f\n\x1b\x42LOCK_STATUS_ACCEPTED_ON_L1\x10\x03\x12\x19\n\x15\x42LOCK_STATUS_REJECTED\x10\x04\x62\x06proto3"
 )
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, "starknet_pb2", globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
     DESCRIPTOR._options = None
-    _BLOCKSTATUS._serialized_start = 5111
-    _BLOCKSTATUS._serialized_end = 5273
+    _BLOCKSTATUS._serialized_start = 5772
+    _BLOCKSTATUS._serialized_end = 5934
     _BLOCK._serialized_start = 92
     _BLOCK._serialized_end = 495
     _BLOCKHEADER._serialized_start = 498
     _BLOCKHEADER._serialized_end = 836
     _TRANSACTIONWITHRECEIPT._serialized_start = 839
     _TRANSACTIONWITHRECEIPT._serialized_end = 988
     _TRANSACTION._serialized_start = 991
@@ -38,37 +39,41 @@
     _INVOKETRANSACTIONV0._serialized_start = 1764
     _INVOKETRANSACTIONV0._serialized_end = 1982
     _INVOKETRANSACTIONV1._serialized_start = 1985
     _INVOKETRANSACTIONV1._serialized_end = 2130
     _DEPLOYTRANSACTION._serialized_start = 2133
     _DEPLOYTRANSACTION._serialized_end = 2356
     _DECLARETRANSACTION._serialized_start = 2359
-    _DECLARETRANSACTION._serialized_end = 2505
-    _L1HANDLERTRANSACTION._serialized_start = 2508
-    _L1HANDLERTRANSACTION._serialized_end = 2727
-    _DEPLOYACCOUNTTRANSACTION._serialized_start = 2730
-    _DEPLOYACCOUNTTRANSACTION._serialized_end = 2960
-    _TRANSACTIONRECEIPT._serialized_start = 2963
-    _TRANSACTIONRECEIPT._serialized_end = 3257
-    _L2TOL1MESSAGEWITHTRANSACTION._serialized_start = 3260
-    _L2TOL1MESSAGEWITHTRANSACTION._serialized_end = 3474
-    _L2TOL1MESSAGE._serialized_start = 3477
-    _L2TOL1MESSAGE._serialized_end = 3611
-    _EVENTWITHTRANSACTION._serialized_start = 3614
-    _EVENTWITHTRANSACTION._serialized_end = 3810
-    _EVENT._serialized_start = 3813
-    _EVENT._serialized_end = 3993
-    _STATEUPDATE._serialized_start = 3996
-    _STATEUPDATE._serialized_end = 4185
-    _STATEDIFF._serialized_start = 4188
-    _STATEDIFF._serialized_end = 4464
-    _STORAGEDIFF._serialized_start = 4467
-    _STORAGEDIFF._serialized_end = 4613
-    _STORAGEENTRY._serialized_start = 4615
-    _STORAGEENTRY._serialized_end = 4739
-    _DECLAREDCONTRACT._serialized_start = 4741
-    _DECLAREDCONTRACT._serialized_end = 4820
-    _DEPLOYEDCONTRACT._serialized_start = 4823
-    _DEPLOYEDCONTRACT._serialized_end = 4969
-    _NONCEUPDATE._serialized_start = 4972
-    _NONCEUPDATE._serialized_end = 5108
+    _DECLARETRANSACTION._serialized_end = 2575
+    _L1HANDLERTRANSACTION._serialized_start = 2578
+    _L1HANDLERTRANSACTION._serialized_end = 2797
+    _DEPLOYACCOUNTTRANSACTION._serialized_start = 2800
+    _DEPLOYACCOUNTTRANSACTION._serialized_end = 3030
+    _TRANSACTIONRECEIPT._serialized_start = 3033
+    _TRANSACTIONRECEIPT._serialized_end = 3394
+    _L2TOL1MESSAGEWITHTRANSACTION._serialized_start = 3397
+    _L2TOL1MESSAGEWITHTRANSACTION._serialized_end = 3611
+    _L2TOL1MESSAGE._serialized_start = 3614
+    _L2TOL1MESSAGE._serialized_end = 3826
+    _EVENTWITHTRANSACTION._serialized_start = 3829
+    _EVENTWITHTRANSACTION._serialized_end = 4025
+    _EVENT._serialized_start = 4028
+    _EVENT._serialized_end = 4223
+    _STATEUPDATE._serialized_start = 4226
+    _STATEUPDATE._serialized_end = 4415
+    _STATEDIFF._serialized_start = 4418
+    _STATEDIFF._serialized_end = 4830
+    _STORAGEDIFF._serialized_start = 4833
+    _STORAGEDIFF._serialized_end = 4979
+    _STORAGEENTRY._serialized_start = 4981
+    _STORAGEENTRY._serialized_end = 5105
+    _DECLAREDCONTRACT._serialized_start = 5107
+    _DECLAREDCONTRACT._serialized_end = 5186
+    _DECLAREDCLASS._serialized_start = 5189
+    _DECLAREDCLASS._serialized_end = 5335
+    _REPLACEDCLASS._serialized_start = 5338
+    _REPLACEDCLASS._serialized_end = 5481
+    _DEPLOYEDCONTRACT._serialized_start = 5484
+    _DEPLOYEDCONTRACT._serialized_end = 5630
+    _NONCEUPDATE._serialized_start = 5633
+    _NONCEUPDATE._serialized_end = 5769
 # @@protoc_insertion_point(module_scope)
```

### Comparing `apibara-0.6.7/src/apibara/starknet/proto/starknet_pb2.pyi` & `apibara-0.7.0/src/apibara/starknet/proto/starknet_pb2.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -84,23 +84,38 @@
         block_number: _Optional[int] = ...,
         sequencer_address: _Optional[_Union[_types_pb2.FieldElement, _Mapping]] = ...,
         new_root: _Optional[_Union[_types_pb2.FieldElement, _Mapping]] = ...,
         timestamp: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ...,
     ) -> None: ...
 
 class DeclareTransaction(_message.Message):
-    __slots__ = ["class_hash", "sender_address"]
+    __slots__ = ["class_hash", "compiled_class_hash", "sender_address"]
     CLASS_HASH_FIELD_NUMBER: _ClassVar[int]
+    COMPILED_CLASS_HASH_FIELD_NUMBER: _ClassVar[int]
     SENDER_ADDRESS_FIELD_NUMBER: _ClassVar[int]
     class_hash: _types_pb2.FieldElement
+    compiled_class_hash: _types_pb2.FieldElement
     sender_address: _types_pb2.FieldElement
     def __init__(
         self,
         class_hash: _Optional[_Union[_types_pb2.FieldElement, _Mapping]] = ...,
         sender_address: _Optional[_Union[_types_pb2.FieldElement, _Mapping]] = ...,
+        compiled_class_hash: _Optional[_Union[_types_pb2.FieldElement, _Mapping]] = ...,
+    ) -> None: ...
+
+class DeclaredClass(_message.Message):
+    __slots__ = ["class_hash", "compiled_class_hash"]
+    CLASS_HASH_FIELD_NUMBER: _ClassVar[int]
+    COMPILED_CLASS_HASH_FIELD_NUMBER: _ClassVar[int]
+    class_hash: _types_pb2.FieldElement
+    compiled_class_hash: _types_pb2.FieldElement
+    def __init__(
+        self,
+        class_hash: _Optional[_Union[_types_pb2.FieldElement, _Mapping]] = ...,
+        compiled_class_hash: _Optional[_Union[_types_pb2.FieldElement, _Mapping]] = ...,
     ) -> None: ...
 
 class DeclaredContract(_message.Message):
     __slots__ = ["class_hash"]
     CLASS_HASH_FIELD_NUMBER: _ClassVar[int]
     class_hash: _types_pb2.FieldElement
     def __init__(
@@ -158,26 +173,29 @@
     def __init__(
         self,
         contract_address: _Optional[_Union[_types_pb2.FieldElement, _Mapping]] = ...,
         class_hash: _Optional[_Union[_types_pb2.FieldElement, _Mapping]] = ...,
     ) -> None: ...
 
 class Event(_message.Message):
-    __slots__ = ["data", "from_address", "keys"]
+    __slots__ = ["data", "from_address", "index", "keys"]
     DATA_FIELD_NUMBER: _ClassVar[int]
     FROM_ADDRESS_FIELD_NUMBER: _ClassVar[int]
+    INDEX_FIELD_NUMBER: _ClassVar[int]
     KEYS_FIELD_NUMBER: _ClassVar[int]
     data: _containers.RepeatedCompositeFieldContainer[_types_pb2.FieldElement]
     from_address: _types_pb2.FieldElement
+    index: int
     keys: _containers.RepeatedCompositeFieldContainer[_types_pb2.FieldElement]
     def __init__(
         self,
         from_address: _Optional[_Union[_types_pb2.FieldElement, _Mapping]] = ...,
         keys: _Optional[_Iterable[_Union[_types_pb2.FieldElement, _Mapping]]] = ...,
         data: _Optional[_Iterable[_Union[_types_pb2.FieldElement, _Mapping]]] = ...,
+        index: _Optional[int] = ...,
     ) -> None: ...
 
 class EventWithTransaction(_message.Message):
     __slots__ = ["event", "receipt", "transaction"]
     EVENT_FIELD_NUMBER: _ClassVar[int]
     RECEIPT_FIELD_NUMBER: _ClassVar[int]
     TRANSACTION_FIELD_NUMBER: _ClassVar[int]
@@ -234,23 +252,29 @@
         entry_point_selector: _Optional[
             _Union[_types_pb2.FieldElement, _Mapping]
         ] = ...,
         calldata: _Optional[_Iterable[_Union[_types_pb2.FieldElement, _Mapping]]] = ...,
     ) -> None: ...
 
 class L2ToL1Message(_message.Message):
-    __slots__ = ["payload", "to_address"]
+    __slots__ = ["from_address", "index", "payload", "to_address"]
+    FROM_ADDRESS_FIELD_NUMBER: _ClassVar[int]
+    INDEX_FIELD_NUMBER: _ClassVar[int]
     PAYLOAD_FIELD_NUMBER: _ClassVar[int]
     TO_ADDRESS_FIELD_NUMBER: _ClassVar[int]
+    from_address: _types_pb2.FieldElement
+    index: int
     payload: _containers.RepeatedCompositeFieldContainer[_types_pb2.FieldElement]
     to_address: _types_pb2.FieldElement
     def __init__(
         self,
         to_address: _Optional[_Union[_types_pb2.FieldElement, _Mapping]] = ...,
         payload: _Optional[_Iterable[_Union[_types_pb2.FieldElement, _Mapping]]] = ...,
+        index: _Optional[int] = ...,
+        from_address: _Optional[_Union[_types_pb2.FieldElement, _Mapping]] = ...,
     ) -> None: ...
 
 class L2ToL1MessageWithTransaction(_message.Message):
     __slots__ = ["message", "receipt", "transaction"]
     MESSAGE_FIELD_NUMBER: _ClassVar[int]
     RECEIPT_FIELD_NUMBER: _ClassVar[int]
     TRANSACTION_FIELD_NUMBER: _ClassVar[int]
@@ -272,34 +296,59 @@
     nonce: _types_pb2.FieldElement
     def __init__(
         self,
         contract_address: _Optional[_Union[_types_pb2.FieldElement, _Mapping]] = ...,
         nonce: _Optional[_Union[_types_pb2.FieldElement, _Mapping]] = ...,
     ) -> None: ...
 
+class ReplacedClass(_message.Message):
+    __slots__ = ["class_hash", "contract_address"]
+    CLASS_HASH_FIELD_NUMBER: _ClassVar[int]
+    CONTRACT_ADDRESS_FIELD_NUMBER: _ClassVar[int]
+    class_hash: _types_pb2.FieldElement
+    contract_address: _types_pb2.FieldElement
+    def __init__(
+        self,
+        contract_address: _Optional[_Union[_types_pb2.FieldElement, _Mapping]] = ...,
+        class_hash: _Optional[_Union[_types_pb2.FieldElement, _Mapping]] = ...,
+    ) -> None: ...
+
 class StateDiff(_message.Message):
-    __slots__ = ["declared_contracts", "deployed_contracts", "nonces", "storage_diffs"]
+    __slots__ = [
+        "declared_classes",
+        "declared_contracts",
+        "deployed_contracts",
+        "nonces",
+        "replaced_classes",
+        "storage_diffs",
+    ]
+    DECLARED_CLASSES_FIELD_NUMBER: _ClassVar[int]
     DECLARED_CONTRACTS_FIELD_NUMBER: _ClassVar[int]
     DEPLOYED_CONTRACTS_FIELD_NUMBER: _ClassVar[int]
     NONCES_FIELD_NUMBER: _ClassVar[int]
+    REPLACED_CLASSES_FIELD_NUMBER: _ClassVar[int]
     STORAGE_DIFFS_FIELD_NUMBER: _ClassVar[int]
+    declared_classes: _containers.RepeatedCompositeFieldContainer[DeclaredClass]
     declared_contracts: _containers.RepeatedCompositeFieldContainer[DeclaredContract]
     deployed_contracts: _containers.RepeatedCompositeFieldContainer[DeployedContract]
     nonces: _containers.RepeatedCompositeFieldContainer[NonceUpdate]
+    replaced_classes: _containers.RepeatedCompositeFieldContainer[ReplacedClass]
     storage_diffs: _containers.RepeatedCompositeFieldContainer[StorageDiff]
     def __init__(
         self,
         storage_diffs: _Optional[_Iterable[_Union[StorageDiff, _Mapping]]] = ...,
         declared_contracts: _Optional[
             _Iterable[_Union[DeclaredContract, _Mapping]]
         ] = ...,
         deployed_contracts: _Optional[
             _Iterable[_Union[DeployedContract, _Mapping]]
         ] = ...,
         nonces: _Optional[_Iterable[_Union[NonceUpdate, _Mapping]]] = ...,
+        declared_classes: _Optional[_Iterable[_Union[DeclaredClass, _Mapping]]] = ...,
+        replaced_classes: _Optional[_Iterable[_Union[ReplacedClass, _Mapping]]] = ...,
     ) -> None: ...
 
 class StateUpdate(_message.Message):
     __slots__ = ["new_root", "old_root", "state_diff"]
     NEW_ROOT_FIELD_NUMBER: _ClassVar[int]
     OLD_ROOT_FIELD_NUMBER: _ClassVar[int]
     STATE_DIFF_FIELD_NUMBER: _ClassVar[int]
@@ -394,36 +443,40 @@
         nonce: _Optional[_Union[_types_pb2.FieldElement, _Mapping]] = ...,
         version: _Optional[int] = ...,
     ) -> None: ...
 
 class TransactionReceipt(_message.Message):
     __slots__ = [
         "actual_fee",
+        "contract_address",
         "events",
         "l2_to_l1_messages",
         "transaction_hash",
         "transaction_index",
     ]
     ACTUAL_FEE_FIELD_NUMBER: _ClassVar[int]
+    CONTRACT_ADDRESS_FIELD_NUMBER: _ClassVar[int]
     EVENTS_FIELD_NUMBER: _ClassVar[int]
     L2_TO_L1_MESSAGES_FIELD_NUMBER: _ClassVar[int]
     TRANSACTION_HASH_FIELD_NUMBER: _ClassVar[int]
     TRANSACTION_INDEX_FIELD_NUMBER: _ClassVar[int]
     actual_fee: _types_pb2.FieldElement
+    contract_address: _types_pb2.FieldElement
     events: _containers.RepeatedCompositeFieldContainer[Event]
     l2_to_l1_messages: _containers.RepeatedCompositeFieldContainer[L2ToL1Message]
     transaction_hash: _types_pb2.FieldElement
     transaction_index: int
     def __init__(
         self,
         transaction_hash: _Optional[_Union[_types_pb2.FieldElement, _Mapping]] = ...,
         transaction_index: _Optional[int] = ...,
         actual_fee: _Optional[_Union[_types_pb2.FieldElement, _Mapping]] = ...,
         l2_to_l1_messages: _Optional[_Iterable[_Union[L2ToL1Message, _Mapping]]] = ...,
         events: _Optional[_Iterable[_Union[Event, _Mapping]]] = ...,
+        contract_address: _Optional[_Union[_types_pb2.FieldElement, _Mapping]] = ...,
     ) -> None: ...
 
 class TransactionWithReceipt(_message.Message):
     __slots__ = ["receipt", "transaction"]
     RECEIPT_FIELD_NUMBER: _ClassVar[int]
     TRANSACTION_FIELD_NUMBER: _ClassVar[int]
     receipt: TransactionReceipt
```

### Comparing `apibara-0.6.7/src/apibara/starknet/proto/types_pb2.py` & `apibara-0.7.0/src/apibara/starknet/proto/types_pb2.py`

 * *Files identical despite different names*

### Comparing `apibara-0.6.7/src/apibara/starknet/proto/types_pb2.pyi` & `apibara-0.7.0/src/apibara/starknet/proto/types_pb2.pyi`

 * *Files identical despite different names*

### Comparing `apibara-0.6.7/PKG-INFO` & `apibara-0.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apibara
-Version: 0.6.7
+Version: 0.7.0
 Summary: Apibara cliend SDK. Stream and transform on-chain data with Python.
 Home-page: https://www.apibara.com
 License: Apache-2.0
 Keywords: ethereum,web3,starknet
 Author: Francesco Ceccon
 Author-email: francesco@apibara.com
 Requires-Python: >=3.8,<3.11
```

