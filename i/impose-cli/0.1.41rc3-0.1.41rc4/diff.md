# Comparing `tmp/impose_cli-0.1.41rc3-py3-none-any.whl.zip` & `tmp/impose_cli-0.1.41rc4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 8766 bytes, number of entries: 14
+Zip file size: 8820 bytes, number of entries: 14
 -rw-r--r--  2.0 unx        0 b- defN 23-Jul-08 14:49 impose_cli/__init__.py
--rw-r--r--  2.0 unx    12087 b- defN 23-Jul-08 14:42 impose_cli/_utils.py
--rw-r--r--  2.0 unx      112 b- defN 23-Jul-08 14:42 impose_cli/decorators.py
+-rw-r--r--  2.0 unx    12270 b- defN 23-Jul-08 17:10 impose_cli/_utils.py
+-rw-r--r--  2.0 unx      149 b- defN 23-Jul-08 17:10 impose_cli/decorators.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Jul-08 14:42 impose_cli/errors.py
 -rw-r--r--  2.0 unx     1237 b- defN 23-Jul-08 14:42 impose_cli/impose_cli.py
 -rw-r--r--  2.0 unx     5029 b- defN 23-Jul-08 14:42 impose_cli/impose_cli_2.py
 -rw-r--r--  2.0 unx      197 b- defN 23-Jul-08 14:42 impose_cli/types.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Jul-08 04:10 tests/__init__.py
 -rw-r--r--  2.0 unx      446 b- defN 23-Jul-08 14:42 tests/test.py
--rw-r--r--  2.0 unx     1071 b- defN 23-Jul-08 14:49 impose_cli-0.1.41rc3.dist-info/LICENSE
--rw-r--r--  2.0 unx      358 b- defN 23-Jul-08 14:49 impose_cli-0.1.41rc3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-08 14:49 impose_cli-0.1.41rc3.dist-info/WHEEL
--rw-r--r--  2.0 unx       17 b- defN 23-Jul-08 14:49 impose_cli-0.1.41rc3.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1107 b- defN 23-Jul-08 14:49 impose_cli-0.1.41rc3.dist-info/RECORD
-14 files, 21753 bytes uncompressed, 6922 bytes compressed:  68.2%
+-rw-r--r--  2.0 unx     1071 b- defN 23-Jul-08 17:11 impose_cli-0.1.41rc4.dist-info/LICENSE
+-rw-r--r--  2.0 unx      358 b- defN 23-Jul-08 17:11 impose_cli-0.1.41rc4.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-08 17:11 impose_cli-0.1.41rc4.dist-info/WHEEL
+-rw-r--r--  2.0 unx       17 b- defN 23-Jul-08 17:11 impose_cli-0.1.41rc4.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1107 b- defN 23-Jul-08 17:11 impose_cli-0.1.41rc4.dist-info/RECORD
+14 files, 21973 bytes uncompressed, 6976 bytes compressed:  68.3%
```

## zipnote {}

```diff
@@ -21,23 +21,23 @@
 
 Filename: tests/__init__.py
 Comment: 
 
 Filename: tests/test.py
 Comment: 
 
-Filename: impose_cli-0.1.41rc3.dist-info/LICENSE
+Filename: impose_cli-0.1.41rc4.dist-info/LICENSE
 Comment: 
 
-Filename: impose_cli-0.1.41rc3.dist-info/METADATA
+Filename: impose_cli-0.1.41rc4.dist-info/METADATA
 Comment: 
 
-Filename: impose_cli-0.1.41rc3.dist-info/WHEEL
+Filename: impose_cli-0.1.41rc4.dist-info/WHEEL
 Comment: 
 
-Filename: impose_cli-0.1.41rc3.dist-info/top_level.txt
+Filename: impose_cli-0.1.41rc4.dist-info/top_level.txt
 Comment: 
 
-Filename: impose_cli-0.1.41rc3.dist-info/RECORD
+Filename: impose_cli-0.1.41rc4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## impose_cli/_utils.py

```diff
@@ -1,25 +1,22 @@
-import inspect
+from .decorators import *  # Do not remove this import
 import os
+import inspect
 import builtins
 import click
-from typing import Any
 from docstring_parser import parse as docparse
-from .decorators import *
 from inspect import signature as sig
 from ast import parse, FunctionDef, Import, ImportFrom, unparse
 from importlib.util import spec_from_file_location, module_from_spec
 from os.path import dirname, join, exists, abspath, splitext, basename, relpath
 
-
 _SUPPORTED_TYPES = [str, int, list, dict]
 
 
 def parse_nodes(entry: str, target: str):
-
     class Function(object):
         def __init__(self, name, function_info: dict):
             self.name = name
             self.arguments = function_info["arguments"]
             self.options = function_info["options"]
             self.decorators = function_info["decorators"]
             self.long_description = function_info["long_description"]
@@ -59,15 +56,17 @@
                     matching_node = Node(name=parts[i])
                     node.add_child(matching_node)
                 node = matching_node
             node.add_function(func_info)
 
     def build_tree(node_info: dict):
         rel_path_start = entry if target is None else join(dirname(entry), target)
-        relative_dict = {"/{}".format(relpath(x, rel_path_start).replace(".py", "").replace("_", "-").replace(".", "")): y for x, y in node_info.items()}
+        relative_dict = {
+            "/{}".format(relpath(x, rel_path_start).replace(".py", "").replace("_", "-").replace(".", "")): y for x, y
+            in node_info.items()}
         tree = Tree(Node(None))
         list_of_tuples = []
         for file, func_info in relative_dict.items():
             for func in func_info:
                 list_of_tuples.append((file, {
                     "name": func,
                     "function_info": relative_dict[file][func]
@@ -168,29 +167,32 @@
     def produce_module_map(python_modules_files: list[str]):
         file_function_map = {}
         for file in python_modules_files:
             module, module_name = load_module_from_file(file)
             analysis = analyze_file(file, module)
             if "_settings" in analysis and "impose" in analysis["_settings"]["decorators"]:
                 for function_name in analysis.keys():
-                    if "impose" not in analysis[function_name]["decorators"] and "hide" not in analysis[function_name]["decorators"]:
+                    if "impose" not in analysis[function_name]["decorators"] and "hide" not in analysis[function_name][
+                        "decorators"]:
                         analysis[function_name]["decorators"].append("impose")
-            file_function_map[file] = {x: y for x, y in analysis.items() if "impose" in y["decorators"] and x != "_settings"}
+            file_function_map[file] = {x: y for x, y in analysis.items() if
+                                       "impose" in y["decorators"] and x != "_settings"}
         return file_function_map
 
     def find_files():
         if target is None:
             return [entry]
 
         else:
             directory = join(dirname(entry), target)
         if not exists(directory):
             raise FileNotFoundError(f"There is no directory {directory}.")
 
-        dirs = [os.path.join(root, file) for root, _, files in os.walk(directory) for file in files if file.endswith('.py')]
+        dirs = [os.path.join(root, file) for root, _, files in os.walk(directory) for file in files if
+                file.endswith('.py')]
         return [abspath(join(directory, f)) for f in dirs]
 
     files = find_files()
     meta = produce_module_map(files)
     tree = build_tree(meta)
     if len(tree.root.children) == 1 and not len(tree.root.functions) and tree.root.children[0].name == "":
         tree.root = tree.root.children[0]
@@ -257,17 +259,18 @@
 
 def build_api_with_tree(tree, root_name=None, return_before_executing=False, host="0.0.0.0", port=8000):
     import fastapi
     import uvicorn
     api = fastapi.FastAPI()
 
     def create_endpoint(router, function):
-        @router.get(function.name)
+        @router.get(("/{}".format(function.name) if not function.name.startswith("/") else function.name))
         def dynamic_route():
             return function.reference
+
         return router
 
     def handle_child(child, parent_group):
         child_group = fastapi.APIRouter(prefix=child.name)
         parent_group.add_command(child_group)
         child.external_object = child_group
         for function in child.functions:
@@ -279,12 +282,13 @@
         base_route = fastapi.APIRouter()
         root.external_object = base_route
         for function in root.functions:
             create_endpoint(base_route, function)
         root.alter_children(handle_child)
         api.include_router(base_route)
         return api
+
     res = dft(tree.root)
     if return_before_executing:
         return res
     else:
         uvicorn.run(res, host=host, port=port)
```

## impose_cli/decorators.py

```diff
@@ -5,7 +5,11 @@
 
 def require_flags(func):
     return func
 
 
 def hide(func):
     return func
+
+
+def cleanup(func):
+    return func
```

## Comparing `impose_cli-0.1.41rc3.dist-info/LICENSE` & `impose_cli-0.1.41rc4.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `impose_cli-0.1.41rc3.dist-info/RECORD` & `impose_cli-0.1.41rc4.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 impose_cli/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-impose_cli/_utils.py,sha256=eZRxMO7T9LYrr5kr8WTZ1N50Cegc2Rxl5VtT7Oo5CLc,12087
-impose_cli/decorators.py,sha256=dtCX2DgpHDxLlFsKst7Prf3Ys-y5EVMo48mJoRGYmxo,112
+impose_cli/_utils.py,sha256=YOBzfUAy0Hs_r6iQXtukGpptkEfpsz0gtBNwgCQT4uc,12270
+impose_cli/decorators.py,sha256=ArmkwmkTPhGYuCJ52wNnqgcmfAl1a0xryoU4iDwTW48,149
 impose_cli/errors.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 impose_cli/impose_cli.py,sha256=CbJu9so1U6Cuwe2b75_5uqemxNur9-rmNF4Vbi3aAd4,1237
 impose_cli/impose_cli_2.py,sha256=YaQv41Ee5NfxV81rMmELEcx8eFmVNMP69MKR3cAiwj0,5029
 impose_cli/types.py,sha256=80g42_q9bbai8byU-TIXnoLKziTJD0nfkek-WFRwkYo,197
 tests/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tests/test.py,sha256=rFszJ_8zyb7YX6NbVaPDMzrKgof7olFgbFIO-FCS4lk,446
-impose_cli-0.1.41rc3.dist-info/LICENSE,sha256=zbz0DcNhgXN5XVIbf__i0DoJPXOL9ybrCwGb2x4Z-tY,1071
-impose_cli-0.1.41rc3.dist-info/METADATA,sha256=j60zc2ksxx-wnnabn-MtLrQSX0iyCewNu_gfZcYJLQE,358
-impose_cli-0.1.41rc3.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-impose_cli-0.1.41rc3.dist-info/top_level.txt,sha256=mF0ZPzXJ1dKbHYbVkC04Bj0o60Pwq0WeyEDbIeIN_EA,17
-impose_cli-0.1.41rc3.dist-info/RECORD,,
+impose_cli-0.1.41rc4.dist-info/LICENSE,sha256=zbz0DcNhgXN5XVIbf__i0DoJPXOL9ybrCwGb2x4Z-tY,1071
+impose_cli-0.1.41rc4.dist-info/METADATA,sha256=XYZnJbTU58fe0foGEWFOArsUtwEbE_4AgwOP8GdqxCk,358
+impose_cli-0.1.41rc4.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+impose_cli-0.1.41rc4.dist-info/top_level.txt,sha256=mF0ZPzXJ1dKbHYbVkC04Bj0o60Pwq0WeyEDbIeIN_EA,17
+impose_cli-0.1.41rc4.dist-info/RECORD,,
```

