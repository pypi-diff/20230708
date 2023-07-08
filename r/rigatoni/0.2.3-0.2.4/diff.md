# Comparing `tmp/rigatoni-0.2.3.tar.gz` & `tmp/rigatoni-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rigatoni-0.2.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "rigatoni-0.2.4.tar", last modified: Sat Jul  8 17:35:03 2023, max compression
```

## Comparing `rigatoni-0.2.3.tar` & `rigatoni-0.2.4.tar`

### file list

```diff
@@ -1,10 +1,49 @@
--rw-r--r--   0        0        0     1945 2023-06-22 21:54:00.405660 rigatoni-0.2.3/README.md
--rw-r--r--   0        0        0      942 2023-06-22 21:54:00.405660 rigatoni-0.2.3/pyproject.toml
--rw-r--r--   0        0        0      956 2023-06-22 21:54:00.405660 rigatoni-0.2.3/rigatoni/__init__.py
--rw-r--r--   0        0        0    43438 2023-06-22 21:54:00.405660 rigatoni-0.2.3/rigatoni/core.py
--rw-r--r--   0        0        0      503 2023-06-22 21:54:00.405660 rigatoni-0.2.3/rigatoni/geometry/__init__.py
--rw-r--r--   0        0        0     4804 2023-06-22 21:54:00.405660 rigatoni-0.2.3/rigatoni/geometry/byte_server.py
--rw-r--r--   0        0        0    31856 2023-06-22 21:54:00.405660 rigatoni-0.2.3/rigatoni/geometry/methods.py
--rw-r--r--   0        0        0     1498 2023-06-22 21:54:00.405660 rigatoni-0.2.3/rigatoni/geometry/objects.py
--rw-r--r--   0        0        0    29937 2023-06-22 21:54:00.405660 rigatoni-0.2.3/rigatoni/noodle_objects.py
--rw-r--r--   0        0        0     2961 1970-01-01 00:00:00.000000 rigatoni-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0     3506 2023-06-20 19:54:44.942275 rigatoni-0.2.4/.github/workflows/continuous_integration.yml
+-rw-r--r--   0        0        0     1421 2023-05-05 15:45:08.191319 rigatoni-0.2.4/.github/workflows/coverage.yml
+-rw-r--r--   0        0        0     1047 2023-05-05 15:45:08.191768 rigatoni-0.2.4/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0     1119 2023-06-20 19:54:44.945276 rigatoni-0.2.4/.github/workflows/test.yml
+-rw-r--r--   0        0        0     3135 2023-06-13 16:27:24.044950 rigatoni-0.2.4/.gitignore
+-rw-r--r--   0        0        0     1101 2022-08-12 15:03:40.714647 rigatoni-0.2.4/LICENSE
+-rw-r--r--   0        0        0     1945 2023-06-21 19:05:15.039195 rigatoni-0.2.4/README.md
+-rw-r--r--   0        0        0      115 2023-06-15 19:54:17.470002 rigatoni-0.2.4/docs/.pages
+-rw-r--r--   0        0        0       58 2023-06-15 15:57:38.411606 rigatoni-0.2.4/docs/api_reference/.pages
+-rw-r--r--   0        0        0      352 2023-06-15 18:27:29.368893 rigatoni-0.2.4/docs/api_reference/components.md
+-rw-r--r--   0        0        0      368 2023-06-26 21:08:32.850540 rigatoni-0.2.4/docs/api_reference/geometry.md
+-rw-r--r--   0        0        0      231 2023-06-14 18:11:17.854247 rigatoni-0.2.4/docs/api_reference/server.md
+-rw-r--r--   0        0        0     1206 2023-06-15 18:47:51.441171 rigatoni-0.2.4/docs/api_reference/support_objects.md
+-rw-r--r--   0        0        0    40440 2023-06-15 19:28:11.494980 rigatoni-0.2.4/docs/assets/concepts.svg
+-rw-r--r--   0        0        0      968 2023-06-15 14:35:12.652491 rigatoni-0.2.4/docs/assets/favicon.png
+-rw-r--r--   0        0        0     1254 2023-06-15 14:35:10.529923 rigatoni-0.2.4/docs/assets/logo.svg
+-rw-r--r--   0        0        0     3321 2023-06-21 14:17:01.116762 rigatoni-0.2.4/docs/basic_usage.md
+-rw-r--r--   0        0        0     3077 2023-06-21 14:50:48.227826 rigatoni-0.2.4/docs/index.md
+-rw-r--r--   0        0        0      824 2023-06-14 23:48:11.136509 rigatoni-0.2.4/docs/install.md
+-rw-r--r--   0        0        0     1592 2023-06-15 19:56:42.301700 rigatoni-0.2.4/docs/noodles.md
+-rw-r--r--   0        0        0      808 2023-06-14 21:17:16.319749 rigatoni-0.2.4/docs/quick_start.md
+-rw-r--r--   0        0        0     1464 2023-06-20 19:39:07.963858 rigatoni-0.2.4/mkdocs.yml
+-rw-r--r--   0        0        0      942 2023-06-20 19:55:39.438455 rigatoni-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0       45 2023-07-07 17:41:39.859872 rigatoni-0.2.4/requirements.txt
+-rw-r--r--   0        0        0      947 2023-07-08 17:33:49.679166 rigatoni-0.2.4/rigatoni/__init__.py
+-rw-r--r--   0        0        0     4804 2023-06-20 19:51:39.651166 rigatoni-0.2.4/rigatoni/byte_server.py
+-rw-r--r--   0        0        0    43479 2023-07-08 17:05:47.244627 rigatoni-0.2.4/rigatoni/core.py
+-rw-r--r--   0        0        0      467 2023-06-26 21:08:32.836421 rigatoni-0.2.4/rigatoni/geometry/__init__.py
+-rw-r--r--   0        0        0    31969 2023-06-28 15:14:39.539867 rigatoni-0.2.4/rigatoni/geometry/methods.py
+-rw-r--r--   0        0        0     1498 2023-06-22 21:03:55.102593 rigatoni-0.2.4/rigatoni/geometry/objects.py
+-rw-r--r--   0        0        0    30416 2023-07-08 17:33:04.117093 rigatoni-0.2.4/rigatoni/noodle_objects.py
+-rw-r--r--   0        0        0        0 2023-05-05 15:45:08.200874 rigatoni-0.2.4/tests/__init__.py
+-rw-r--r--   0        0        0     8622 2023-06-14 20:03:53.431955 rigatoni-0.2.4/tests/clients.py
+-rw-r--r--   0        0        0        0 2023-05-05 15:45:08.201078 rigatoni-0.2.4/tests/examples/__init__.py
+-rw-r--r--   0        0        0     8158 2023-06-21 17:44:26.776995 rigatoni-0.2.4/tests/examples/basic_server.py
+-rw-r--r--   0        0        0    11872 2023-07-07 17:33:30.120374 rigatoni-0.2.4/tests/examples/geometry_server.py
+-rw-r--r--   0        0        0  2309522 2023-05-05 15:45:08.213596 rigatoni-0.2.4/tests/mesh_data/boot.obj
+-rw-r--r--   0        0        0     2898 2023-06-20 13:49:01.077673 rigatoni-0.2.4/tests/mesh_data/box.gltf
+-rw-r--r--   0        0        0      648 2023-06-20 13:48:02.901111 rigatoni-0.2.4/tests/mesh_data/box0.bin
+-rw-r--r--   0        0        0   205922 2023-05-05 15:45:08.216659 rigatoni-0.2.4/tests/mesh_data/data.csv
+-rw-r--r--   0        0        0  2408417 2023-05-05 15:45:08.232076 rigatoni-0.2.4/tests/mesh_data/stanford-bunny.obj
+-rw-r--r--   0        0        0  3645817 2023-07-07 17:36:00.242186 rigatoni-0.2.4/tests/mesh_data/test_mesh.obj
+-rw-r--r--   0        0        0     3106 2023-07-07 17:35:56.388919 rigatoni-0.2.4/tests/mesh_data/test_sphere.obj
+-rw-r--r--   0        0        0     3347 2023-06-20 18:13:41.376089 rigatoni-0.2.4/tests/servers.py
+-rw-r--r--   0        0        0      795 2023-07-07 18:02:05.023194 rigatoni-0.2.4/tests/test_byte_server.py
+-rw-r--r--   0        0        0    12489 2023-06-20 22:05:38.111108 rigatoni-0.2.4/tests/test_core.py
+-rw-r--r--   0        0        0    12643 2023-07-07 17:28:51.869864 rigatoni-0.2.4/tests/test_geometry_creation.py
+-rw-r--r--   0        0        0     5183 2023-06-20 19:28:59.553008 rigatoni-0.2.4/tests/test_noodle_objects.py
+-rw-r--r--   0        0        0     2961 1970-01-01 00:00:00.000000 rigatoni-0.2.4/PKG-INFO
```

### Comparing `rigatoni-0.2.3/README.md` & `rigatoni-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `rigatoni-0.2.3/pyproject.toml` & `rigatoni-0.2.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `rigatoni-0.2.3/rigatoni/__init__.py` & `rigatoni-0.2.4/rigatoni/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,19 +13,19 @@
         objects.py
     delegates.py
     noodle_objects.py
     server.py
 """
 
 
-__version__ = "0.2.3"
+__version__ = "0.2.4"
 
 from .core import Server
 from .noodle_objects import *
-from .geometry.byte_server import ByteServer
+from .byte_server import ByteServer
 
 # Ensure that dependencies are installed for optional module
 try:
     import numpy
     import meshio
     optionals = True
 except ImportError:
```

### Comparing `rigatoni-0.2.3/rigatoni/core.py` & `rigatoni-0.2.4/rigatoni/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -358,37 +358,37 @@
             noodle_object (NoodleObject): Delegate, Reply, or Invoke object
             delta (set): field names to be included in update
         """
 
         contents = {}
         if action == "create":
             base_delegate = self.id_decoder[type(noodle_object.id)]
-            include = {field for field in base_delegate.__fields__ if field not in ["server", "signals"]}
-            contents = noodle_object.dict(exclude_none=True, include=include)
+            include = {field for field in base_delegate.model_fields if field not in ["server", "signals"]}
+            contents = noodle_object.model_dump(exclude_none=True, include=include)
 
         elif action == "invoke":
-            contents = noodle_object.dict(exclude_none=True)
+            contents = noodle_object.model_dump(exclude_none=True)
 
         elif action == "reply":
 
             if noodle_object.method_exception:
                 e = noodle_object.method_exception
-                contents = noodle_object.dict(exclude_none=True)
+                contents = noodle_object.model_dump(exclude_none=True)
                 contents["method_exception"] = {"code": e.code, "message": e.message, "data": e.data}
             else:
-                contents = noodle_object.dict(exclude_none=True)
+                contents = noodle_object.model_dump(exclude_none=True)
 
         elif action == "update":
             if not noodle_object:  # Document case
                 contents["methods_list"] = self.get_ids_by_type(Method)
                 contents["signals_list"] = self.get_ids_by_type(Signal)
             else:  # Normal update, include id, and any field in delta
                 delta = set() if not delta else delta
                 delta.add("id")
-                contents = noodle_object.dict(exclude_none=True, include=delta)
+                contents = noodle_object.model_dump(exclude_none=True, include=delta)
 
         elif action == "delete":
             try:
                 contents["id"] = noodle_object.id
             except AttributeError:
                 raise Exception(f"Cannot delete a {noodle_object}")
 
@@ -601,15 +601,15 @@
         try:
             new_delegate = comp_type(server=self, id=comp_id, **kwargs)
         except Exception as e:
             raise ValueError(f"Args: {kwargs}, invalid for initializing a {comp_type}: {e}")
 
         # Update state and keep track of initial version for changes / update messages
         self.state[comp_id] = new_delegate
-        self.client_state[comp_id] = new_delegate.copy()
+        self.client_state[comp_id] = new_delegate.model_copy()
 
         # Update references for each component referenced by this one
         self._update_references(new_delegate, new_delegate)
 
         # Create message and broadcast
         message = self._prepare_message("create", new_delegate)
         self.broadcast(message)
@@ -683,15 +683,15 @@
             # Check if anything in the queue is now clear to be deleted
             for comp_id in list(self.delete_queue):
                 if not self.references.get(comp_id):
                     self.delete_queue.remove(comp_id)
                     self.delete_component(comp_id)
 
         else:
-            logging.warning(f"Couldn't delete {delegate}, referenced by {self.references[del_id]}, added to queue")
+            logging.info(f"Couldn't delete {delegate}, referenced by {self.references[del_id]}, added to queue")
             self.delete_queue.add(del_id)
 
     @staticmethod
     def _find_delta(state, edited):
         """Helper to find differences between two objects
         
         Also checks to find recursive cases and cases where references
@@ -722,15 +722,15 @@
         delta = self._find_delta(outdated, current)
 
         # Update references
         self._update_references(outdated, outdated, removing=True)
         self._update_references(current, current)
 
         # Update tracking state
-        self.client_state[current.id] = current.copy()
+        self.client_state[current.id] = current.model_copy()
 
         # Form message and broadcast
         try:
             message = self._prepare_message("update", current, delta)
             self.broadcast(message)
         except Exception as e:
             raise ValueError(f"This obj can not be updated: {e}")
```

### Comparing `rigatoni-0.2.3/rigatoni/geometry/byte_server.py` & `rigatoni-0.2.4/rigatoni/byte_server.py`

 * *Files identical despite different names*

### Comparing `rigatoni-0.2.3/rigatoni/geometry/methods.py` & `rigatoni-0.2.4/rigatoni/geometry/methods.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import numpy as np
 import meshio
 
 from .. import noodle_objects as nooobs
 from ..core import Server
 
 from .objects import AttributeInput, GeometryPatchInput
-from .byte_server import ByteServer
+from rigatoni.byte_server import ByteServer
 
 INLINE_LIMIT = 10000
 
 SIZES = {
     # in bytes
     "U8": 1,
     "U16": 2,
@@ -257,24 +257,24 @@
     index_format = _get_format(vert_count)
 
     # Set up attributes with given lists
     attribute_info = _set_up_attributes(patch_input, generate_normals=generate_normals, ordered=ordered_indices)
 
     # Build buffer with given lists
     buffer: nooobs.Buffer
-    buffer, index_offset = _build_geometry_buffer(server, name, patch_input, index_format, attribute_info, byte_server)
+    buffer, index_offset = _build_geometry_buffer(server, f"{name} Buffer", patch_input, index_format, attribute_info, byte_server)
 
     # Make buffer view component
     buffer_view: nooobs.BufferView = server.create_component(
         nooobs.BufferView,
-        name=name,
+        name=f"{name} Buffer View",
         source_buffer=buffer.id,
         type="GEOMETRY",
-        offset=0,  # What is this? cant always assume 0
-        length=buffer.size
+        offset=0,
+        length=index_offset  # For this format of buffer
     )
 
     # Create attribute objects from buffer view and attribute info
     attributes = []
     for attribute in attribute_info:
         attr_obj = nooobs.Attribute(view=buffer_view.id, **dict(attribute))
         attributes.append(attr_obj)
@@ -331,15 +331,19 @@
         instances (Mat4): optional instance matrix, can use create_instances to generate
 
     Returns:
         Entity: newly created entity delegate
     """
 
     # Set name to match geometry
-    name = geometry.name if geometry.name else None
+    if geometry.name:
+        name = geometry.name
+        geometry.name = f"{name} Geometry"
+    else:
+        name = "No Name Entity"
 
     # Create instance buffer and view if specified
     if instances:
         buffer = build_instance_buffer(server, name, instances)
         buffer_view = server.create_component(
             nooobs.BufferView,
             name=f"Instance View for {name}",
```

### Comparing `rigatoni-0.2.3/rigatoni/geometry/objects.py` & `rigatoni-0.2.4/rigatoni/geometry/objects.py`

 * *Files identical despite different names*

### Comparing `rigatoni-0.2.3/rigatoni/noodle_objects.py` & `rigatoni-0.2.4/rigatoni/noodle_objects.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 """
 
 from enum import Enum
 from math import pi
 from queue import Queue
 from typing import Callable, Optional, Any, List, Tuple, Dict, NamedTuple
 
-from pydantic import BaseModel, root_validator
+from pydantic import ConfigDict, BaseModel, model_validator
 
 """ =============================== ID's ============================= """
 
 
 class ID(NamedTuple):
     """Base class for all ID's
 
@@ -118,20 +118,15 @@
 
 
 """ ====================== Generic Parent Class ====================== """
 
 
 class NoodleObject(BaseModel):
     """Parent Class for all noodle objects"""
-
-    class Config:
-        """Configuration for Validation"""
-
-        arbitrary_types_allowed = True
-        use_enum_values = True
+    model_config = ConfigDict(arbitrary_types_allowed=True, use_enum_values=True)
 
 
 class Delegate(NoodleObject):
     """Parent class for all delegates
 
     Defines general methods that should be available for all delegates.
 
@@ -511,15 +506,15 @@
         table (Optional[TableID]): Table to invoke signal on
         plot (Optional[PlotID]): Plot to invoke signal on
     """
     entity: Optional[EntityID] = None
     table: Optional[TableID] = None
     plot: Optional[PlotID] = None
 
-    @root_validator(allow_reuse=True)
+    @model_validator(mode="after")
     def one_of_three(cls, values):
         already_found = False
         for field in values:
             if values[field] and already_found:
                 raise ValueError("More than one field entered")
             elif values[field]:
                 already_found = True
@@ -552,15 +547,15 @@
     """
     columns: List[TableColumnInfo]
     keys: List[int]
     data: List[List[Any]]  # Originally tried union, but currently order is used to coerce by pydantic
     selections: Optional[List[Selection]] = None
 
     # too much overhead? - strict mode
-    @root_validator(allow_reuse=True)
+    @model_validator(mode="after")
     def types_match(cls, values):
         for row in values['data']:
             for col, i in zip(values['columns'], range(len(row))):
                 text_mismatch = isinstance(row[i], str) and col.type != "TEXT"
                 real_mismatch = isinstance(row[i], float) and col.type != "REAL"
                 int_mismatch = isinstance(row[i], int) and col.type != "INTEGER"
                 if text_mismatch or real_mismatch or int_mismatch:
@@ -665,15 +660,15 @@
 
     simple_plot: Optional[str] = None
     url_plot: Optional[str] = None
 
     methods_list: Optional[List[MethodID]] = None
     signals_list: Optional[List[SignalID]] = None
 
-    @root_validator(allow_reuse=True)
+    @model_validator(mode="after")
     def one_of(cls, values):
         if bool(values['simple_plot']) != bool(values['url_plot']):
             return values
         else:
             raise ValueError("One plot type must be specified")
 
 
@@ -690,15 +685,15 @@
     id: BufferID
     name: Optional[str] = None
     size: int = None
 
     inline_bytes: bytes = None
     uri_bytes: str = None
 
-    @root_validator(allow_reuse=True)
+    @model_validator(mode="after")
     def one_of(cls, values):
         if bool(values['inline_bytes']) != bool(values['uri_bytes']):
             return values
         else:
             raise ValueError("One plot type must be specified")
 
 
@@ -767,15 +762,15 @@
     """
     id: ImageID
     name: Optional[str] = None
 
     buffer_source: BufferID = None
     uri_source: str = None
 
-    @root_validator(allow_reuse=True)
+    @model_validator(mode="after")
     def one_of(cls, values):
         if bool(values['buffer_source']) != bool(values['uri_source']):
             return values
         else:
             raise ValueError("One plot type must be specified")
 
 
@@ -833,15 +828,15 @@
     color: Optional[RGB] = [1.0, 1.0, 1.0]
     intensity: Optional[float] = 1.0
 
     point: PointLight = None
     spot: SpotLight = None
     directional: DirectionalLight = None
 
-    @root_validator(allow_reuse=True)
+    @model_validator(mode="after")
     def one_of(cls, values):
         already_found = False
         for field in ['point', 'spot', 'directional']:
             if values[field] and already_found:
                 raise ValueError("More than one field entered")
             elif values[field]:
                 already_found = True
@@ -916,14 +911,30 @@
         pass
 
     def table_selection_updated(self, selection: Selection):
         """Invoke table selection updated signal"""
         pass
 
 
+# TODO: need to work this in to specify which methods are avaiable in which contexts
+class Document(Delegate):
+    """Represents the scope of the whole session
+
+    Attributes:
+        name (str): name will be "Document"
+        methods_list (list[MethodID]): list of methods available on the document
+        signals_list (list[SignalID]): list of signals available on the document
+    """
+
+    name: str = "Document"
+
+    methods_list: List[MethodID] = []  # Server usually sends as an update
+    signals_list: List[SignalID] = []
+
+
 """ ====================== Communication Objects ====================== """
 
 
 class Invoke(NoodleObject):
     id: SignalID
     context: Optional[InvokeIDType] = None  # if empty - document
     signal_data: List[Any]
```

### Comparing `rigatoni-0.2.3/PKG-INFO` & `rigatoni-0.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rigatoni
-Version: 0.2.3
+Version: 0.2.4
 Summary: Python Server Library for NOODLES Protocol
 Keywords: noodles,cbor,Websockets,server,NOODLES
 Author: Alex Racapé
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
```

