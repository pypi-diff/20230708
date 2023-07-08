# Comparing `tmp/hat_sbs-0.6.3-cp39-cp39-win_amd64.whl.zip` & `tmp/hat_sbs-0.6.4-cp310.cp311-abi3-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,18 @@
-Zip file size: 52521 bytes, number of entries: 14
--rw-r--r--  2.0 unx     1737 b- defN 22-Aug-29 14:37 hat/sbs/__init__.py
--rwxr-xr-x  2.0 unx   122896 b- defN 23-Feb-23 20:08 hat/sbs/_cserializer.cp39-win_amd64.pyd
--rw-r--r--  2.0 unx     5146 b- defN 22-Aug-29 18:47 hat/sbs/_pyserializer.py
--rw-r--r--  2.0 unx     1212 b- defN 22-Aug-29 14:40 hat/sbs/common.py
--rw-r--r--  2.0 unx     3524 b- defN 22-Aug-29 14:49 hat/sbs/evaluator.py
--rw-r--r--  2.0 unx     5721 b- defN 22-Aug-29 14:44 hat/sbs/parser.py
--rw-r--r--  2.0 unx     3184 b- defN 21-Nov-10 17:38 hat/sbs/repository.py
--rw-r--r--  2.0 unx     1395 b- defN 23-Jan-14 22:55 hat/sbs/serializer.py
--rw-r--r--  2.0 unx    11358 b- defN 23-Feb-23 20:08 hat_sbs-0.6.3.dist-info/LICENSE
--rw-r--r--  2.0 unx     1897 b- defN 23-Feb-23 20:08 hat_sbs-0.6.3.dist-info/METADATA
--rw-r--r--  2.0 unx      100 b- defN 23-Feb-23 20:08 hat_sbs-0.6.3.dist-info/WHEEL
--rw-r--r--  2.0 unx        4 b- defN 23-Feb-23 20:08 hat_sbs-0.6.3.dist-info/top_level.txt
--rw-r--r--  2.0 unx        1 b- defN 23-Feb-23 20:08 hat_sbs-0.6.3.dist-info/zip-safe
-?rw-rw-r--  2.0 unx     1109 b- defN 23-Feb-23 20:08 hat_sbs-0.6.3.dist-info/RECORD
-14 files, 159284 bytes uncompressed, 50697 bytes compressed:  68.2%
+Zip file size: 53376 bytes, number of entries: 16
+-rw-r--r--  2.0 unx     1820 b- defN 23-Jul-08 12:15 hat/sbs/__init__.py
+-rw-r--r--  2.0 unx     1227 b- defN 23-Jul-08 12:21 hat/sbs/common.py
+-rw-r--r--  2.0 unx     3517 b- defN 23-Jul-08 12:17 hat/sbs/evaluator.py
+-rw-r--r--  2.0 unx     5697 b- defN 23-Jul-08 12:18 hat/sbs/parser.py
+-rw-r--r--  2.0 unx     3062 b- defN 23-Jul-08 12:32 hat/sbs/repository.py
+-rw-r--r--  2.0 unx      443 b- defN 23-Jul-08 11:54 hat/sbs/serializer/__init__.py
+-rwxr-xr-x  2.0 unx   123722 b- defN 23-Jul-08 12:56 hat/sbs/serializer/_cserializer.abi3.pyd
+-rw-r--r--  2.0 unx      524 b- defN 23-Jul-08 12:03 hat/sbs/serializer/common.py
+-rw-r--r--  2.0 unx      576 b- defN 23-Jul-08 12:39 hat/sbs/serializer/cserializer.py
+-rw-r--r--  2.0 unx     5043 b- defN 23-Jul-08 12:04 hat/sbs/serializer/pyserializer.py
+-rw-r--r--  2.0 unx    11358 b- defN 23-Jul-08 12:56 hat_sbs-0.6.4.dist-info/LICENSE
+-rw-r--r--  2.0 unx     2272 b- defN 23-Jul-08 12:56 hat_sbs-0.6.4.dist-info/METADATA
+-rw-r--r--  2.0 unx      127 b- defN 23-Jul-08 12:56 hat_sbs-0.6.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx        4 b- defN 23-Jul-08 12:56 hat_sbs-0.6.4.dist-info/top_level.txt
+-rw-r--r--  2.0 unx        1 b- defN 23-Jul-08 12:56 hat_sbs-0.6.4.dist-info/zip-safe
+-rw-rw-r--  2.0 unx     1301 b- defN 23-Jul-08 12:56 hat_sbs-0.6.4.dist-info/RECORD
+16 files, 160694 bytes uncompressed, 51238 bytes compressed:  68.1%
```

## zipnote {}

```diff
@@ -1,43 +1,49 @@
 Filename: hat/sbs/__init__.py
 Comment: 
 
-Filename: hat/sbs/_cserializer.cp39-win_amd64.pyd
-Comment: 
-
-Filename: hat/sbs/_pyserializer.py
-Comment: 
-
 Filename: hat/sbs/common.py
 Comment: 
 
 Filename: hat/sbs/evaluator.py
 Comment: 
 
 Filename: hat/sbs/parser.py
 Comment: 
 
 Filename: hat/sbs/repository.py
 Comment: 
 
-Filename: hat/sbs/serializer.py
+Filename: hat/sbs/serializer/__init__.py
+Comment: 
+
+Filename: hat/sbs/serializer/_cserializer.abi3.pyd
+Comment: 
+
+Filename: hat/sbs/serializer/common.py
+Comment: 
+
+Filename: hat/sbs/serializer/cserializer.py
+Comment: 
+
+Filename: hat/sbs/serializer/pyserializer.py
 Comment: 
 
-Filename: hat_sbs-0.6.3.dist-info/LICENSE
+Filename: hat_sbs-0.6.4.dist-info/LICENSE
 Comment: 
 
-Filename: hat_sbs-0.6.3.dist-info/METADATA
+Filename: hat_sbs-0.6.4.dist-info/METADATA
 Comment: 
 
-Filename: hat_sbs-0.6.3.dist-info/WHEEL
+Filename: hat_sbs-0.6.4.dist-info/WHEEL
 Comment: 
 
-Filename: hat_sbs-0.6.3.dist-info/top_level.txt
+Filename: hat_sbs-0.6.4.dist-info/top_level.txt
 Comment: 
 
-Filename: hat_sbs-0.6.3.dist-info/zip-safe
+Filename: hat_sbs-0.6.4.dist-info/zip-safe
 Comment: 
 
-Filename: hat_sbs-0.6.3.dist-info/RECORD
+Filename: hat_sbs-0.6.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## hat/sbs/__init__.py

```diff
@@ -52,11 +52,13 @@
 
 """
 
 from hat.sbs.common import Data
 from hat.sbs.repository import Repository
 from hat.sbs.serializer import (Serializer,
                                 CSerializer,
-                                PySerializer)
+                                PySerializer,
+                                DefaultSerializer)
 
 
-__all__ = ['Repository', 'Data', 'Serializer', 'CSerializer', 'PySerializer']
+__all__ = ['Repository', 'Data', 'Serializer', 'CSerializer', 'PySerializer',
+           'DefaultSerializer']
```

## hat/sbs/common.py

```diff
@@ -1,14 +1,14 @@
 import typing
 
 from hat import util
 
 
 class Ref(typing.NamedTuple):
-    module: typing.Optional[str]
+    module: str | None
     name: str
 
 
 class NoneType(typing.NamedTuple):
     pass
 
 
@@ -33,33 +33,29 @@
 
 
 class ArrayType(typing.NamedTuple):
     t: 'Type'
 
 
 class RecordType(typing.NamedTuple):
-    entries: typing.List[typing.Tuple[str, 'Type']]
+    entries: list[typing.Tuple[str, 'Type']]
 
 
 class ChoiceType(typing.NamedTuple):
     entries: typing.List[typing.Tuple[str, 'Type']]
 
 
-Type = typing.Union[Ref,
-                    NoneType,
-                    BooleanType,
-                    IntegerType,
-                    FloatType,
-                    StringType,
-                    BytesType,
-                    ArrayType,
-                    RecordType,
-                    ChoiceType]
-
-Data = typing.Union[None, bool, int, float, str, bytes,
-                    typing.List['Data'],
-                    typing.Dict[str, 'Data'],
-                    typing.Tuple[str, 'Data']]
-
-# HACK
-util.register_type_alias('Type')
-util.register_type_alias('Data')
+Type: typing.TypeAlias = (Ref |
+                          NoneType |
+                          BooleanType |
+                          IntegerType |
+                          FloatType |
+                          StringType |
+                          BytesType |
+                          ArrayType |
+                          RecordType |
+                          ChoiceType)
+
+Data: typing.TypeAlias = (None | bool | int | float | str | util.Bytes |
+                          typing.List['Data'] |
+                          typing.Dict[str, 'Data'] |
+                          typing.Tuple[str, 'Data'])
```

## hat/sbs/evaluator.py

```diff
@@ -1,15 +1,15 @@
 import typing
 
 from hat.sbs import common
 from hat.sbs import parser
 
 
 def evaluate_modules(modules: typing.Iterable[parser.AstModule]
-                     ) -> typing.Dict[common.Ref, common.Type]:
+                     ) -> dict[common.Ref, common.Type]:
     """Evaluate modules."""
     refs = dict(_builtin_refs)
     modules_dict = {module.name: module for module in modules}
     for module in modules_dict.values():
         for ast_type_def in module.type_defs.values():
             if ast_type_def.args:
                 continue
```

## hat/sbs/parser.py

```diff
@@ -1,34 +1,34 @@
 import typing
 
 from hat import json
 import hat.peg
 
 
 class AstType(typing.NamedTuple):
-    module: typing.Optional[str]
+    module: str | None
     name: str
     entries: typing.List['AstEntry']
     args: typing.List['AstType']
 
 
 class AstEntry(typing.NamedTuple):
     name: str
     type: AstType
 
 
 class AstTypeDef(typing.NamedTuple):
     name: str
-    args: typing.List[str]
+    args: list[str]
     type: AstType
 
 
 class AstModule(typing.NamedTuple):
     name: str
-    type_defs: typing.Dict[str, AstTypeDef]
+    type_defs: dict[str, AstTypeDef]
 
 
 def parse(schema: str) -> AstModule:
     """Parse SBS schema"""
     ast = _grammar.parse(schema)
     return hat.peg.walk_ast(ast, _actions)
```

## hat/sbs/repository.py

```diff
@@ -1,11 +1,13 @@
 import pathlib
 import typing
 
 from hat import json
+from hat import util
+
 from hat.sbs import common
 from hat.sbs import evaluator
 from hat.sbs import parser
 from hat.sbs import serializer
 
 
 class Repository:
@@ -17,76 +19,78 @@
         * path to direcory recursivly searched for .sbs files
         * other repository
 
     """
 
     def __init__(self,
                  *args: typing.Union['Repository', pathlib.Path, str],
-                 serializer: typing.Optional[typing.Type[serializer.Serializer]] = None):  # NOQA
+                 serializer: typing.Type[serializer.Serializer] = serializer.DefaultSerializer):  # NOQA
         self._serializer = serializer
         self._modules = list(_parse_args(args))
         self._refs = evaluator.evaluate_modules(self._modules)
 
     def encode(self,
-               module_name: typing.Optional[str],
+               module_name: str | None,
                type_name: str,
                value: common.Data
                ) -> bytes:
         """Encode value."""
         ref = common.Ref(module_name, type_name)
-        ser = self._serializer or serializer.default_serializer
-        return ser.encode(self._refs, ref, value)
+        return self._serializer.encode(self._refs, ref, value)
 
     def decode(self,
-               module_name: typing.Optional[str],
+               module_name: str | None,
                type_name: str,
-               data: typing.Union[bytes, bytearray, memoryview]
+               data: util.Bytes
                ) -> common.Data:
         """Decode data."""
         ref = common.Ref(module_name, type_name)
-        ser = self._serializer or serializer.default_serializer
-        return ser.decode(self._refs, ref, memoryview(data))
+        return self._serializer.decode(self._refs, ref, data)
 
     def to_json(self) -> json.Data:
         """Export repository content as json serializable data.
 
         Entire repository content is exported as json serializable data.
         New repository can be created from the exported content by using
         :meth:`Repository.from_json`.
 
         """
         return [parser.module_to_json(module) for module in self._modules]
 
     @staticmethod
-    def from_json(data: typing.Union[pathlib.PurePath, common.Data],
+    def from_json(data: pathlib.PurePath | common.Data,
                   *,
-                  serializer: typing.Optional[typing.Type[serializer.Serializer]] = None  # NOQA
+                  serializer: typing.Type[serializer.Serializer] = serializer.DefaultSerializer  # NOQA
                   ) -> 'Repository':
         """Create new repository from content exported as json serializable
         data.
 
         Creates a new repository from content of another repository that was
         exported by using :meth:`Repository.to_json`.
 
         """
         if isinstance(data, pathlib.PurePath):
             data = json.decode_file(data)
+
         repo = Repository(serializer=serializer)
         repo._modules = [parser.module_from_json(i) for i in data]
         repo._refs = evaluator.evaluate_modules(repo._modules)
         return repo
 
 
 def _parse_args(args):
     for arg in args:
         if isinstance(arg, pathlib.PurePath):
             paths = ([arg] if arg.suffix == '.sbs'
                      else arg.rglob('*.sbs'))
             for path in paths:
                 with open(path, encoding='utf-8') as f:
                     yield parser.parse(f.read())
+
         elif isinstance(arg, Repository):
             yield from arg._modules
+
         elif isinstance(arg, str):
             yield parser.parse(arg)
+
         else:
-            raise ValueError()
+            raise ValueError('unsupported arg')
```

## Comparing `hat/sbs/_pyserializer.py` & `hat/sbs/serializer/pyserializer.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,22 @@
 import collections
 import struct
-import typing
 
-from hat.sbs import common
+from hat.sbs.serializer import common
 
 
-def encode(refs: typing.Dict[common.Ref, common.Type],
-           t: common.Type,
-           value: common.Data
-           ) -> bytes:
-    return bytes(_encode_generic(refs, t, value))
+class PySerializer(common.Serializer):
+    """Serializer implementation in Python"""
 
+    def encode(refs, t, value):
+        return bytes(_encode_generic(refs, t, value))
 
-def decode(refs: typing.Dict[common.Ref, common.Type],
-           t: common.Type,
-           data: memoryview
-           ) -> common.Data:
-    data, _ = _decode_generic(refs, t, data)
-    return data
+    def decode(refs, t, data):
+        value, _ = _decode_generic(refs, t, memoryview(data))
+        return value
 
 
 def _encode_generic(refs, t, value):
     while isinstance(t, common.Ref) and t in refs:
         t = refs[t]
 
     if isinstance(t, common.NoneType):
```

## Comparing `hat_sbs-0.6.3.dist-info/LICENSE` & `hat_sbs-0.6.4.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `hat_sbs-0.6.3.dist-info/METADATA` & `hat_sbs-0.6.4.dist-info/METADATA`

 * *Files 13% similar despite different names*

```diff
@@ -1,57 +1,82 @@
 Metadata-Version: 2.1
 Name: hat-sbs
-Version: 0.6.3
+Version: 0.6.4
 Summary: Hat simple binary serializer
 Home-page: https://github.com/hat-open/hat-sbs
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
-Requires-Python: >=3.8
+Requires-Python: >=3.10
 Description-Content-Type: text/x-rst
 License-File: LICENSE
-Requires-Dist: hat-json (~=0.5.15)
-Requires-Dist: hat-peg (~=0.5.6)
-Requires-Dist: hat-util (~=0.6.7)
+Requires-Dist: hat-json (~=0.5.19)
+Requires-Dist: hat-peg (~=0.5.7)
+Requires-Dist: hat-util (~=0.6.10)
+
+.. _online documentation: https://hat-sbs.hat-open.com
+.. _git repository: https://github.com/hat-open/hat-sbs.git
+.. _PyPI project: https://pypi.org/project/hat-sbs
+.. _pydoit: https://pydoit.org
+.. _Hat Open: https://hat-open.com
+.. _Končar Digital: https://www.koncar.hr/en
+
 
 hat-sbs - Simple binary serialization
 =====================================
 
-This library is part of Hat Open project - open-source framework of tools and
-libraries for developing applications used for remote monitoring, control and
-management of intelligent electronic devices such as IoT devices, PLCs,
-industrial automation or home automation systems.
-
-Development of Hat Open and associated repositories is sponsored by
-`Končar Digital <https://www.koncar.hr>`_.
-
 For more information see:
 
-    * hat-sbs documentation - `<https://hat-sbs.hat-open.com>`_
-    * hat-sbs git repository - `<https://github.com/hat-open/hat-sbs.git>`_
-    * Hat Open homepage - `<https://hat-open.com>`_
-
-.. warning::
-
-    This project is currently in state of active development. Features,
-    functionality and API are unstable.
+* `online documentation`_
+* `git repository`_
 
 
 Install
 -------
 
-::
+`hat-sbs` python library is available as `PyPI project`_::
 
     $ pip install hat-sbs
 
 
+Build
+-----
+
+Build tool used for `hat-sbs` is `pydoit`_. It can be installed together
+with other python dependencies by running::
+
+    $ pip install -r requirements.pip.dev.txt
+
+For listing available doit tasks, use::
+
+    $ doit list
+
+Default task::
+
+    $ doit
+
+creates wheel package inside `build` directory.
+
+
+Hat Open
+--------
+
+`hat-sbs` is part of `Hat Open`_ project - open-source framework of tools
+and libraries for developing applications used for remote monitoring, control
+and management of intelligent electronic devices such as IoT devices, PLCs,
+industrial automation or home automation systems.
+
+Development of Hat Open and associated repositories is sponsored by
+`Končar Digital`_.
+
+
 License
 -------
 
-Copyright 2020-2022 Hat Open AUTHORS
+Copyright 2020-2023 Hat Open AUTHORS
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

