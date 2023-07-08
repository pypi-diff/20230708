# Comparing `tmp/pydantic_zarr-0.3.0.tar.gz` & `tmp/pydantic_zarr-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydantic_zarr-0.3.0.tar", max compression
+gzip compressed data, was "pydantic_zarr-0.4.0.tar", max compression
```

## Comparing `pydantic_zarr-0.3.0.tar` & `pydantic_zarr-0.4.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1070 2023-05-30 21:01:34.647934 pydantic_zarr-0.3.0/LICENSE
--rw-r--r--   0        0        0     3746 2023-06-22 03:12:34.236303 pydantic_zarr-0.3.0/README.md
--rw-r--r--   0        0        0      489 2023-06-22 03:14:29.111501 pydantic_zarr-0.3.0/pyproject.toml
--rw-r--r--   0        0        0       85 2023-06-03 15:04:37.431488 pydantic_zarr-0.3.0/src/pydantic_zarr/__init__.py
--rw-r--r--   0        0        0    11216 2023-06-22 03:14:05.695358 pydantic_zarr-0.3.0/src/pydantic_zarr/core.py
--rw-r--r--   0        0        0     4230 1970-01-01 00:00:00.000000 pydantic_zarr-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-07-08 03:10:32.682229 pydantic_zarr-0.4.0/LICENSE
+-rw-r--r--   0        0        0     1212 2023-07-08 03:10:32.682229 pydantic_zarr-0.4.0/README.md
+-rw-r--r--   0        0        0      664 2023-07-08 03:10:32.682229 pydantic_zarr-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0       85 2023-07-08 03:10:32.682229 pydantic_zarr-0.4.0/src/pydantic_zarr/__init__.py
+-rw-r--r--   0        0        0    11156 2023-07-08 03:10:32.682229 pydantic_zarr-0.4.0/src/pydantic_zarr/core.py
+-rw-r--r--   0        0        0     1720 1970-01-01 00:00:00.000000 pydantic_zarr-0.4.0/PKG-INFO
```

### Comparing `pydantic_zarr-0.3.0/LICENSE` & `pydantic_zarr-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pydantic_zarr-0.3.0/src/pydantic_zarr/core.py` & `pydantic_zarr-0.4.0/src/pydantic_zarr/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,59 +16,57 @@
 import numcodecs
 import zarr
 import os
 import numpy as np
 import numpy.typing as npt
 from numcodecs.abc import Codec
 
-TAttrs = TypeVar("TAttrs", bound=Union[Mapping[str, Any], BaseModel])
+TAttr = TypeVar("TAttr", bound=Union[Mapping[str, Any], BaseModel])
 TItem = TypeVar("TItem", bound=Union["GroupSpec", "ArraySpec"])
 
 DimensionSeparator = Union[Literal["."], Literal["/"]]
 ZarrVersion = Union[Literal[2], Literal[3]]
 ArrayOrder = Union[Literal["C"], Literal["F"]]
 
 
-class NodeSpec(GenericModel, Generic[TAttrs]):
+class NodeSpec(GenericModel, Generic[TAttr]):
     """
     The base class for ArraySpec and GroupSpec. Generic with respect to the type of
     attrs.
     """
 
     zarr_version: ZarrVersion = 2
 
     class Config:
         extra = "forbid"
 
 
-class ArraySpec(NodeSpec, Generic[TAttrs]):
+class ArraySpec(NodeSpec, Generic[TAttr]):
     """
     This pydantic model represents the structural properties of a zarr array.
     It does not represent the data contained in the array. It is generic with respect to
     the type of attrs.
     """
 
-    attrs: TAttrs
+    attrs: TAttr
     shape: tuple[int, ...]
     chunks: tuple[int, ...]
     dtype: str
     fill_value: Union[None, int, float] = 0
     order: ArrayOrder = "C"
     filters: Optional[list[dict[str, Any]]] = None
     dimension_separator: DimensionSeparator = "/"
     compressor: Optional[dict[str, Any]] = None
 
     @validator("dtype", pre=True)
     def stringify_dtype(cls, v):
         """
         Convert a np.dtype object into a string
         """
-        if isinstance(v, np.dtype):
-            return str(v)
-        return v
+        return np.dtype(v).str
 
     @validator("compressor", pre=True)
     def jsonify_compressor(cls, v):
         if isinstance(v, Codec):
             v = v.get_config()
         return v
 
@@ -180,52 +178,52 @@
                 numcodecs.get_codec(f) for f in spec_dict["filters"]
             ]
         result = zarr.create(store=store, path=path, **spec_dict, overwrite=overwrite)
         result.attrs.put(attrs)
         return result
 
 
-class GroupSpec(NodeSpec, Generic[TAttrs, TItem]):
-    attrs: TAttrs
+class GroupSpec(NodeSpec, Generic[TAttr, TItem]):
+    attrs: TAttr
     items: dict[str, TItem] = {}
 
     @classmethod
-    def from_zarr(cls, zgroup: zarr.Group) -> "GroupSpec[TAttrs, TItem]":
+    def from_zarr(cls, group: zarr.Group) -> "GroupSpec[TAttr, TItem]":
         """
         Create a GroupSpec from a zarr group. Subgroups and arrays contained in the zarr
         group will be converted to instances of GroupSpec and ArraySpec, respectively,
         and these spec instances will be stored in the .items attribute of the parent
         GroupSpec. This occurs recursively, so the entire zarr hierarchy below a given
         group can be represented as a GroupSpec.
 
         Parameters
         ----------
-        zgroup : zarr group
+        group : zarr group
 
         Returns
         -------
         An instance of GroupSpec that represents the structure of the zarr hierarchy.
         """
 
-        result: GroupSpec[TAttrs, TItem]
+        result: GroupSpec[TAttr, TItem]
         items = {}
-        for name, item in zgroup.items():
+        for name, item in group.items():
             if isinstance(item, zarr.Array):
                 _item = ArraySpec.from_zarr(item)
             elif isinstance(item, zarr.Group):
                 _item = cls.from_zarr(item)
             else:
                 msg = f"""
                 Unparseable object encountered: {type(item)}. Expected zarr.Array or
                 zarr.Group.
                 """
                 raise ValueError(msg)
             items[name] = _item
 
-        result = cls(attrs=dict(zgroup.attrs), items=items)
+        result = cls(attrs=dict(group.attrs), items=items)
         return result
 
     def to_zarr(self, store: BaseStore, path: str, overwrite: bool = False):
         """
         Serialize a GroupSpec to a zarr group at a specific path in a zarr store.
 
         Parameters
@@ -262,15 +260,15 @@
         return result
 
 
 def from_zarr(element: Union[zarr.Array, zarr.Group]) -> Union[ArraySpec, GroupSpec]:
     """
     Recursively parse a Zarr group or Zarr array into an ArraySpec or GroupSpec.
 
-    Paramters
+    Parameters
     ---------
     element : a zarr Array or zarr Group
 
     Returns
     -------
     An instance of GroupSpec or ArraySpec that represents the
     structure of the zarr group or array.
```

