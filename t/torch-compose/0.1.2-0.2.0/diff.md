# Comparing `tmp/torch_compose-0.1.2.tar.gz` & `tmp/torch_compose-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torch_compose-0.1.2.tar", max compression
+gzip compressed data, was "torch_compose-0.2.0.tar", max compression
```

## Comparing `torch_compose-0.1.2.tar` & `torch_compose-0.2.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1062 2023-07-04 03:44:54.065101 torch_compose-0.1.2/LICENSE
--rw-r--r--   0        0        0        0 2023-07-02 00:03:31.365915 torch_compose-0.1.2/README.md
--rw-r--r--   0        0        0      634 2023-07-07 23:11:03.401997 torch_compose-0.1.2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-02 00:03:31.365915 torch_compose-0.1.2/torch_compose/__init__.py
--rw-r--r--   0        0        0   250222 2023-07-04 04:28:07.930671 torch_compose-0.1.2/torch_compose/demo.ipynb
--rw-r--r--   0        0        0    10630 2023-07-07 23:08:56.607072 torch_compose-0.1.2/torch_compose/module.py
--rw-r--r--   0        0        0      542 1970-01-01 00:00:00.000000 torch_compose-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-07-04 03:44:54.065101 torch_compose-0.2.0/LICENSE
+-rw-r--r--   0        0        0     5127 2023-07-08 00:05:13.488581 torch_compose-0.2.0/README.md
+-rw-r--r--   0        0        0      634 2023-07-08 00:05:40.296046 torch_compose-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0       92 2023-07-08 00:05:13.488581 torch_compose-0.2.0/torch_compose/__init__.py
+-rw-r--r--   0        0        0   361140 2023-07-08 00:05:13.492580 torch_compose-0.2.0/torch_compose/demo.ipynb
+-rw-r--r--   0        0        0    10395 2023-07-08 00:05:13.492580 torch_compose-0.2.0/torch_compose/module.py
+-rw-r--r--   0        0        0     5669 1970-01-01 00:00:00.000000 torch_compose-0.2.0/PKG-INFO
```

### Comparing `torch_compose-0.1.2/LICENSE` & `torch_compose-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `torch_compose-0.1.2/pyproject.toml` & `torch_compose-0.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "torch-compose"
-version = "0.1.2"
+version = "0.2.0"
 description = ""
 authors = ["Alex Naka <alex.naka@gmail.com>"]
 readme = "README.md"
 packages = [{include = "torch_compose"}]
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.11"
```

### Comparing `torch_compose-0.1.2/torch_compose/module.py` & `torch_compose-0.2.0/torch_compose/module.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,66 +1,64 @@
-from abc import abstractmethod
 from collections import OrderedDict
 from graphlib import TopologicalSorter
-from typing import Dict, Tuple, Union, Callable
+from typing import Callable, Dict, Tuple, Union
 
 import networkx as nx
 import torch
 from matplotlib import pyplot as plt
 from torch import nn
 
 
 class DirectedModule(nn.Module):
     """
     An abstract base class for a module that takes a set of inputs and produces a set of outputs.
     The module's forward function needs to be implemented by any subclass. This module can be integrated
     in a module graph where data is flowing from one module to another.
 
+    3 ways to play:
+    1. Pass in a module argument to wrap a module
+    2. Pass in a forward argument to point to a function/method
+    3. Subclass or use as a mixin and define a forward method
+
     Args:
         input_keys: The keys used to extract inputs from the batch.
         output_keys: The keys used to add outputs to the batch.
     """
 
     def __init__(
         self,
         input_keys: Union[str, Tuple, Dict] = None,  # keys to extract from batch
         output_keys: Union[str, Tuple, Dict] = None,  # keys to add to batch
-        forward_function: Callable = None,  # function to run on batch
+        module: nn.Module = None,  # module to wrap
+        forward: Callable = None,  # function/method to point to
         **kwargs,
     ):
         super().__init__()
 
-        # If input_keys is a single string, convert it to a list for consistency
-        if isinstance(input_keys, str):
-            input_keys = [input_keys]
-
-        # If input_keys is not a dict, convert it to a tuple to handle multiple inputs
-        try:
-            input_keys.keys()
-        except AttributeError:
-            input_keys = tuple(input_keys)
-
-        self.input_keys = input_keys
-
-        # If output_keys is a single string, convert it to a list for consistency
-        if isinstance(output_keys, str):
-            output_keys = [output_keys]
-
-        # If output_keys is not a dict, convert it to a tuple to handle multiple outputs
-        try:
-            output_keys.keys()
-        except AttributeError:
-            output_keys = tuple(output_keys)
-
-        self.output_keys = output_keys
-        
-        if forward_function is not None:
-            self.forward = forward_function
-        else:
-            self.forward = self._placeholder_forward
+        self.input_keys = self._process_keys(input_keys)
+        self.output_keys = self._process_keys(output_keys)
+
+        assert (
+            module is None or forward is None
+        ), "Only one of module or forward can be specified"
+
+        if module is not None:
+            self.add_module("node", module)
+            self.forward = module.forward
+        elif forward is not None:
+            self.forward = forward
+            
+    def _process_keys(self, keys):
+        # If keys is a single string, convert it to a list for consistency
+        if isinstance(keys, str):
+            keys = [keys]
+        # If keys is not a dict, convert it to a tuple to handle multiple inputs/outputs
+        if not isinstance(keys, dict):
+            keys = tuple(keys)
+        return keys
 
     def _graph_forward(self, batch: Dict[str, torch.Tensor]) -> Dict[str, torch.Tensor]:
         """
         Runs the forward pass for the module, using the specified input and output keys.
 
         Args:
             batch: The batch of data to be processed.
@@ -148,20 +146,14 @@
         """Returns the set of output batch keys"""
 
         if isinstance(self.output_keys, dict):
             return set(self.output_keys.values())
         else:
             return set(self.output_keys)
 
-    def _placeholder_forward(self, *args, **kwargs):
-        """
-        Defines the computation performed at every call. Should be overridden by all subclasses.
-        """
-        raise NotImplementedError("forward method must be implemented in subclass")
-
 
 class ModuleGraph(nn.ModuleDict):
     """
     This class defines a graph of DirectedModules, where each module can take as input the output of another module.
 
     Args:
         modules: A dictionary of DirectedModule, with keys as the module names and values as the module instances.
```

