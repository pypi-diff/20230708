# Comparing `tmp/alchemy_graph-0.1.2.tar.gz` & `tmp/alchemy_graph-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alchemy_graph-0.1.2.tar", max compression
+gzip compressed data, was "alchemy_graph-0.1.3.tar", max compression
```

## Comparing `alchemy_graph-0.1.2.tar` & `alchemy_graph-0.1.3.tar`

### file list

```diff
@@ -1,9 +1,11 @@
--rw-r--r--   0        0        0     1062 2023-05-25 16:53:32.336463 alchemy_graph-0.1.2/LICENSE
--rw-r--r--   0        0        0     3183 2023-05-25 16:53:32.336463 alchemy_graph-0.1.2/README.md
--rw-r--r--   0        0        0      268 2023-05-25 16:53:32.336463 alchemy_graph-0.1.2/alchemy_graph/__init__.py
--rw-r--r--   0        0        0       22 2023-05-25 16:53:32.336463 alchemy_graph-0.1.2/alchemy_graph/__version__.py
--rw-r--r--   0        0        0     6844 2023-05-25 16:53:32.336463 alchemy_graph-0.1.2/alchemy_graph/main.py
--rw-r--r--   0        0        0     3279 2023-05-25 16:53:32.336463 alchemy_graph-0.1.2/alchemy_graph/utils.py
--rw-r--r--   0        0        0     1656 2023-05-25 16:53:32.336463 alchemy_graph-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     2651 2023-05-25 16:53:32.336463 alchemy_graph-0.1.2/tests/test_utils.py
--rw-r--r--   0        0        0     4160 1970-01-01 00:00:00.000000 alchemy_graph-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-07-07 23:01:27.672531 alchemy_graph-0.1.3/LICENSE
+-rw-r--r--   0        0        0     3188 2023-07-07 23:01:27.672531 alchemy_graph-0.1.3/README.md
+-rw-r--r--   0        0        0      238 2023-07-07 23:01:27.672531 alchemy_graph-0.1.3/alchemy_graph/__init__.py
+-rw-r--r--   0        0        0       22 2023-07-07 23:01:27.672531 alchemy_graph-0.1.3/alchemy_graph/__version__.py
+-rw-r--r--   0        0        0     5132 2023-07-07 23:01:27.672531 alchemy_graph-0.1.3/alchemy_graph/main.py
+-rw-r--r--   0        0        0      166 2023-07-07 23:01:27.672531 alchemy_graph-0.1.3/alchemy_graph/types.py
+-rw-r--r--   0        0        0     3032 2023-07-07 23:01:27.672531 alchemy_graph-0.1.3/alchemy_graph/utils.py
+-rw-r--r--   0        0        0     1766 2023-07-07 23:01:27.672531 alchemy_graph-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     2771 2023-07-07 23:01:27.672531 alchemy_graph-0.1.3/tests/test_lib.py
+-rw-r--r--   0        0        0     2651 2023-07-07 23:01:27.672531 alchemy_graph-0.1.3/tests/test_utils.py
+-rw-r--r--   0        0        0     4093 1970-01-01 00:00:00.000000 alchemy_graph-0.1.3/PKG-INFO
```

### Comparing `alchemy_graph-0.1.2/LICENSE` & `alchemy_graph-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `alchemy_graph-0.1.2/README.md` & `alchemy_graph-0.1.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 <h2 align="center">:small_red_triangle: alchemy_graph :small_red_triangle:</h2>
 
-![New Project](https://user-images.githubusercontent.com/68655454/236483334-a3c86f5c-f732-4465-bf78-692ddd4609b2.png)
+![photo_2023-05-26_16-50-36](https://github.com/kieled/alchemy_graph/assets/68655454/ac2e2804-4cf3-4eea-942a-07fb4c5f0db2)
 
 <p align="center">
     <a href="https://pypi.python.org/pypi/alchemy_graph" alt="PyPi Package Version">
         <img src="https://img.shields.io/pypi/v/alchemy_graph.svg" /></a>
     <a href="https://pypi.python.org/pypi/alchemy_graph" alt="Supported Python versions">
         <img src="https://img.shields.io/pypi/pyversions/alchemy_graph.svg" /></a>
     <a href="https://github.com/kieled/alchemy_graph/actions/workflows/test.yml" alt="GitFlow">
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
       ***** :small_red_triangle: alchemy_graph :small_red_triangle: *****
-![New Project](https://user-images.githubusercontent.com/68655454/236483334-
-a3c86f5c-f732-4465-bf78-692ddd4609b2.png)
+![photo_2023-05-26_16-50-36](https://github.com/kieled/alchemy_graph/assets/
+68655454/ac2e2804-4cf3-4eea-942a-07fb4c5f0db2)
 [https://img.shields.io/pypi/v/alchemy_graph.svg] [https://img.shields.io/pypi/
 pyversions/alchemy_graph.svg] [https://github.com/kieled/alchemy_graph/actions/
                          workflows/test.yml/badge.svg]
                      SQLAlchemy mapper to Strawberry types
 ## :pencil2: Installation You can install mapper using pip: ```bash pip install
 alchemy-graph ``` ## Functions: ### `get_only_selected_fields` Given a
 SQLAlchemy model class and a Strawberry Info object representing a selection
```

### Comparing `alchemy_graph-0.1.2/alchemy_graph/utils.py` & `alchemy_graph-0.1.3/alchemy_graph/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,96 +1,85 @@
 import copy
 import re
+from typing import Sequence
+
 from sqlalchemy.orm import class_mapper
-from strawberry.types import Info
+
+from alchemy_graph.types import AL, F, T
 
 
 def convert_camel_case(name: str) -> str:
-    pattern = re.compile(r'(?<!^)(?=[A-Z])')
-    name = pattern.sub('_', name).lower()
+    pattern = re.compile(r"(?<!^)(?=[A-Z])")
+    name = pattern.sub("_", name).lower()
     return name
 
 
-def find_info_in_args(*args, **kwargs) -> Info:
-    if 'info' in kwargs:
-        return kwargs.get('info')
-    for i in args:
-        if isinstance(i, Info):
-            return i
-    raise Exception('orm_mapper should used only with Strawberry fields')
-
-
-def flatten(items):
+def flatten(items: list[F]):
     if not items:
         return items
     if isinstance(items[0], list):
         return flatten(items[0]) + flatten(items[1:])
     return items[:1] + flatten(items[1:])
 
 
-def _to_dict(obj):
+def _to_dict(obj: T) -> dict | list[dict]:
     if isinstance(obj, list) or isinstance(obj, tuple):
         return [_to_dict(i) for i in obj]
-    if not hasattr(obj, '__dict__'):
+    if not hasattr(obj, "__dict__"):
         return obj
     temp = obj.__dict__
     for key, value in temp.items():
-        if hasattr(value, '_enum_definition') or isinstance(value, bytes):
+        if hasattr(value, "_enum_definition") or isinstance(value, bytes):
             continue
-        elif hasattr(value, '__dict__'):
+        elif hasattr(value, "__dict__"):
             temp[key] = _to_dict(value)
         elif isinstance(value, list):
             temp[key] = [_to_dict(i) for i in value]
     return temp
 
 
 def strawberry_to_dict(
-        strawberry_model,
-        exclude_none: bool = False,
-        exclude: set | None = None,
+    strawberry_model: T,
+    exclude_none: bool = False,
+    exclude: set | None = None,
 ):
     """
     Converts a Strawberry type to a dictionary.
 
     :param strawberry_model: The Strawberry type to convert to dictionary.
     :param exclude_none: Whether to exclude dictionary keys with `None` values. Defaults to `False`.
     :param exclude: Set of field names to exclude from the resulting dictionary. Defaults to `None`.
 
     :return: A dictionary with the values of the Strawberry type.
     """
-    dict_obj: dict = _to_dict(
-        copy.deepcopy(strawberry_model)
-    )
+    dict_obj: dict = _to_dict(copy.deepcopy(strawberry_model))
     result_dict = {**dict_obj}
     for k, v in dict_obj.items():
         if exclude:
             if k in exclude:
                 result_dict.pop(k, None)
         if exclude_none and v is None:
             result_dict.pop(k, None)
     return result_dict
 
 
-def get_dict_object(model) -> dict | list[dict]:
+def get_dict_object(model: Sequence[AL] | AL) -> dict | list[dict]:
     """
     Map sqlalchemy model or list of them to dict
 
     :param model: SQLAlchemy model
     :return: dict or list of dicts
     """
 
     if isinstance(model, list):
         return [get_dict_object(i) for i in model]
     if isinstance(model, dict):
         for k, v in model.items():
             if isinstance(v, list):
-                return {
-                    **model,
-                    k: [get_dict_object(i) for i in v]
-                }
+                return {**model, k: [get_dict_object(i) for i in v]}
         return model
     mapper = class_mapper(model.__class__)
     out = {
         col.key: getattr(model, col.key)
         for col in mapper.columns
         if col.key in model.__dict__
     }
```

### Comparing `alchemy_graph-0.1.2/pyproject.toml` & `alchemy_graph-0.1.3/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "alchemy_graph"
-version = "0.1.2"
+version = "0.1.3"
 description = ""
 authors = ["Kiel Ed <kieledssh@gmail.com>"]
 readme = "README.md"
 keywords = ["strawberry-graphql", "sqlalchemy-mapper", "sqlalchemy", "strawberry", "mapper", "dict"]
 homepage = "https://github.com/kieled/alchemy_graph"
 repository = "https://github.com/kieled/alchemy_graph"
 packages = [
@@ -19,24 +19,28 @@
     "Programming Language :: Python :: Implementation :: PyPy",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Intended Audience :: Developers",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.10"
-sqlalchemy = "^2.0.15"
-fastapi = "^0.95.2"
-strawberry-graphql = { extras = ["fastapi"], version = "^0.178.0" }
+sqlalchemy = "^2"
+strawberry-graphql = "^0"
 
 
 [tool.poetry.group.dev.dependencies]
 ruff = "^0.0.264"
+strawberry-graphql = { extras = ["fastapi"], version = "^0" }
+fastapi = "^0.95.2"
 pytest = "^7.3.1"
 pytest-asyncio = "^0.21.0"
 pre-commit = "^3.3.1"
+httpx = "^0.24.1"
+aiosqlite = "^0.19.0"
+uvicorn = {extras = ["standart"], version = "^0.22.0"}
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.isort]
 profile = "black"
```

### Comparing `alchemy_graph-0.1.2/tests/test_utils.py` & `alchemy_graph-0.1.3/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `alchemy_graph-0.1.2/PKG-INFO` & `alchemy_graph-0.1.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,32 @@
 Metadata-Version: 2.1
 Name: alchemy-graph
-Version: 0.1.2
+Version: 0.1.3
 Summary: 
 Home-page: https://github.com/kieled/alchemy_graph
 Keywords: strawberry-graphql,sqlalchemy-mapper,sqlalchemy,strawberry,mapper,dict
 Author: Kiel Ed
 Author-email: kieledssh@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Dist: fastapi (>=0.95.2,<0.96.0)
-Requires-Dist: sqlalchemy (>=2.0.15,<3.0.0)
-Requires-Dist: strawberry-graphql[fastapi] (>=0.178.0,<0.179.0)
+Requires-Dist: sqlalchemy (>=2,<3)
+Requires-Dist: strawberry-graphql (>=0,<1)
 Project-URL: Repository, https://github.com/kieled/alchemy_graph
 Description-Content-Type: text/markdown
 
 <h2 align="center">:small_red_triangle: alchemy_graph :small_red_triangle:</h2>
 
-![New Project](https://user-images.githubusercontent.com/68655454/236483334-a3c86f5c-f732-4465-bf78-692ddd4609b2.png)
+![photo_2023-05-26_16-50-36](https://github.com/kieled/alchemy_graph/assets/68655454/ac2e2804-4cf3-4eea-942a-07fb4c5f0db2)
 
 <p align="center">
     <a href="https://pypi.python.org/pypi/alchemy_graph" alt="PyPi Package Version">
         <img src="https://img.shields.io/pypi/v/alchemy_graph.svg" /></a>
     <a href="https://pypi.python.org/pypi/alchemy_graph" alt="Supported Python versions">
         <img src="https://img.shields.io/pypi/pyversions/alchemy_graph.svg" /></a>
     <a href="https://github.com/kieled/alchemy_graph/actions/workflows/test.yml" alt="GitFlow">
```

#### html2text {}

```diff
@@ -1,23 +1,22 @@
-Metadata-Version: 2.1 Name: alchemy-graph Version: 0.1.2 Summary: Home-page:
+Metadata-Version: 2.1 Name: alchemy-graph Version: 0.1.3 Summary: Home-page:
 https://github.com/kieled/alchemy_graph Keywords: strawberry-
 graphql,sqlalchemy-mapper,sqlalchemy,strawberry,mapper,dict Author: Kiel Ed
 Author-email: kieledssh@gmail.com Requires-Python: >=3.10,<4.0 Classifier:
 Intended Audience :: Developers Classifier: License :: OSI Approved :: Apache
 Software License Classifier: Programming Language :: Python Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
 Programming Language :: Python :: Implementation :: PyPy Classifier: Topic ::
-Software Development :: Libraries :: Python Modules Requires-Dist: fastapi
-(>=0.95.2,<0.96.0) Requires-Dist: sqlalchemy (>=2.0.15,<3.0.0) Requires-Dist:
-strawberry-graphql[fastapi] (>=0.178.0,<0.179.0) Project-URL: Repository,
+Software Development :: Libraries :: Python Modules Requires-Dist: sqlalchemy
+(>=2,<3) Requires-Dist: strawberry-graphql (>=0,<1) Project-URL: Repository,
 https://github.com/kieled/alchemy_graph Description-Content-Type: text/markdown
       ***** :small_red_triangle: alchemy_graph :small_red_triangle: *****
-![New Project](https://user-images.githubusercontent.com/68655454/236483334-
-a3c86f5c-f732-4465-bf78-692ddd4609b2.png)
+![photo_2023-05-26_16-50-36](https://github.com/kieled/alchemy_graph/assets/
+68655454/ac2e2804-4cf3-4eea-942a-07fb4c5f0db2)
 [https://img.shields.io/pypi/v/alchemy_graph.svg] [https://img.shields.io/pypi/
 pyversions/alchemy_graph.svg] [https://github.com/kieled/alchemy_graph/actions/
                          workflows/test.yml/badge.svg]
                      SQLAlchemy mapper to Strawberry types
 ## :pencil2: Installation You can install mapper using pip: ```bash pip install
 alchemy-graph ``` ## Functions: ### `get_only_selected_fields` Given a
 SQLAlchemy model class and a Strawberry Info object representing a selection
```

