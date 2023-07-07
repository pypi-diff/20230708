# Comparing `tmp/torch_compose-0.1.1.tar.gz` & `tmp/torch_compose-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torch_compose-0.1.1.tar", max compression
+gzip compressed data, was "torch_compose-0.1.2.tar", max compression
```

## Comparing `torch_compose-0.1.1.tar` & `torch_compose-0.1.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1062 2023-07-04 00:41:28.256948 torch_compose-0.1.1/LICENSE
--rw-r--r--   0        0        0        0 2023-07-01 01:44:51.699904 torch_compose-0.1.1/README.md
--rw-r--r--   0        0        0      627 2023-07-04 05:27:44.274922 torch_compose-0.1.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-01 01:44:51.699904 torch_compose-0.1.1/torch_compose/__init__.py
--rw-r--r--   0        0        0   248026 2023-07-04 00:25:48.880921 torch_compose-0.1.1/torch_compose/demo.ipynb
--rw-r--r--   0        0        0    10395 2023-07-04 00:25:08.508748 torch_compose-0.1.1/torch_compose/module.py
--rw-r--r--   0        0        0      542 1970-01-01 00:00:00.000000 torch_compose-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-07-04 03:44:54.065101 torch_compose-0.1.2/LICENSE
+-rw-r--r--   0        0        0        0 2023-07-02 00:03:31.365915 torch_compose-0.1.2/README.md
+-rw-r--r--   0        0        0      634 2023-07-07 23:11:03.401997 torch_compose-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-02 00:03:31.365915 torch_compose-0.1.2/torch_compose/__init__.py
+-rw-r--r--   0        0        0   250222 2023-07-04 04:28:07.930671 torch_compose-0.1.2/torch_compose/demo.ipynb
+-rw-r--r--   0        0        0    10630 2023-07-07 23:08:56.607072 torch_compose-0.1.2/torch_compose/module.py
+-rw-r--r--   0        0        0      542 1970-01-01 00:00:00.000000 torch_compose-0.1.2/PKG-INFO
```

### Comparing `torch_compose-0.1.1/LICENSE` & `torch_compose-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `torch_compose-0.1.1/pyproject.toml` & `torch_compose-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [tool.poetry]
 name = "torch-compose"
-version = "0.1.1"
+version = "0.1.2"
 description = ""
 authors = ["Alex Naka <alex.naka@gmail.com>"]
 readme = "README.md"
 packages = [{include = "torch_compose"}]
 
 [tool.poetry.dependencies]
-python = "^3.9"
+python = ">=3.8,<3.11"
+graphlib = "^0.9.5"
 networkx = "^3.1"
 torch = {version= "^1.7.0 || >=2.0.0", source="torch"}
 matplotlib = "^3.7.1"
-graphlib = "^0.9.5"
 
 [tool.poetry.group.dev.dependencies]
 ipykernel = "^6.23.3"
 pytest = "^7.4.0"
 black = "^23.3.0"
 
 [build-system]
```

### Comparing `torch_compose-0.1.1/torch_compose/module.py` & `torch_compose-0.1.2/torch_compose/module.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from abc import abstractmethod
 from collections import OrderedDict
 from graphlib import TopologicalSorter
-from typing import Dict, Tuple, Union
+from typing import Dict, Tuple, Union, Callable
 
 import networkx as nx
 import torch
 from matplotlib import pyplot as plt
 from torch import nn
 
 
@@ -20,14 +20,15 @@
         output_keys: The keys used to add outputs to the batch.
     """
 
     def __init__(
         self,
         input_keys: Union[str, Tuple, Dict] = None,  # keys to extract from batch
         output_keys: Union[str, Tuple, Dict] = None,  # keys to add to batch
+        forward_function: Callable = None,  # function to run on batch
         **kwargs,
     ):
         super().__init__()
 
         # If input_keys is a single string, convert it to a list for consistency
         if isinstance(input_keys, str):
             input_keys = [input_keys]
@@ -47,14 +48,19 @@
         # If output_keys is not a dict, convert it to a tuple to handle multiple outputs
         try:
             output_keys.keys()
         except AttributeError:
             output_keys = tuple(output_keys)
 
         self.output_keys = output_keys
+        
+        if forward_function is not None:
+            self.forward = forward_function
+        else:
+            self.forward = self._placeholder_forward
 
     def _graph_forward(self, batch: Dict[str, torch.Tensor]) -> Dict[str, torch.Tensor]:
         """
         Runs the forward pass for the module, using the specified input and output keys.
 
         Args:
             batch: The batch of data to be processed.
@@ -142,16 +148,15 @@
         """Returns the set of output batch keys"""
 
         if isinstance(self.output_keys, dict):
             return set(self.output_keys.values())
         else:
             return set(self.output_keys)
 
-    @abstractmethod
-    def forward(self, *args, **kwargs):
+    def _placeholder_forward(self, *args, **kwargs):
         """
         Defines the computation performed at every call. Should be overridden by all subclasses.
         """
         raise NotImplementedError("forward method must be implemented in subclass")
 
 
 class ModuleGraph(nn.ModuleDict):
```

### Comparing `torch_compose-0.1.1/PKG-INFO` & `torch_compose-0.1.2/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: torch-compose
-Version: 0.1.1
+Version: 0.1.2
 Summary: 
 Author: Alex Naka
 Author-email: alex.naka@gmail.com
-Requires-Python: >=3.9,<4.0
+Requires-Python: >=3.8,<3.11
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: graphlib (>=0.9.5,<0.10.0)
 Requires-Dist: matplotlib (>=3.7.1,<4.0.0)
 Requires-Dist: networkx (>=3.1,<4.0)
 Requires-Dist: torch (>=1.7.0)
 Description-Content-Type: text/markdown
```

