# Comparing `tmp/einops-0.6.2rc0.tar.gz` & `tmp/einops-0.7.0rc1.tar.gz`

## Comparing `einops-0.6.2rc0.tar` & `einops-0.7.0rc1.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0     1258 2020-02-02 00:00:00.000000 einops-0.6.2rc0/mkdocs.yml
--rw-r--r--   0        0        0     2925 2020-02-02 00:00:00.000000 einops-0.6.2rc0/test.py
--rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 einops-0.6.2rc0/einops/__init__.py
--rw-r--r--   0        0        0    20467 2020-02-02 00:00:00.000000 einops-0.6.2rc0/einops/_backends.py
--rw-r--r--   0        0        0     3656 2020-02-02 00:00:00.000000 einops-0.6.2rc0/einops/_torch_specific.py
--rw-r--r--   0        0        0    34842 2020-02-02 00:00:00.000000 einops-0.6.2rc0/einops/einops.py
--rw-r--r--   0        0        0     7668 2020-02-02 00:00:00.000000 einops-0.6.2rc0/einops/packing.py
--rw-r--r--   0        0        0     6717 2020-02-02 00:00:00.000000 einops-0.6.2rc0/einops/parsing.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 einops-0.6.2rc0/einops/py.typed
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 einops-0.6.2rc0/einops/experimental/__init__.py
--rw-r--r--   0        0        0     4690 2020-02-02 00:00:00.000000 einops-0.6.2rc0/einops/experimental/data_api_packing.py
--rw-r--r--   0        0        0    14777 2020-02-02 00:00:00.000000 einops-0.6.2rc0/einops/experimental/indexing.py
--rw-r--r--   0        0        0     3747 2020-02-02 00:00:00.000000 einops-0.6.2rc0/einops/layers/__init__.py
--rw-r--r--   0        0        0     8578 2020-02-02 00:00:00.000000 einops-0.6.2rc0/einops/layers/_einmix.py
--rw-r--r--   0        0        0     1981 2020-02-02 00:00:00.000000 einops-0.6.2rc0/einops/layers/chainer.py
--rw-r--r--   0        0        0     2621 2020-02-02 00:00:00.000000 einops-0.6.2rc0/einops/layers/flax.py
--rw-r--r--   0        0        0     2101 2020-02-02 00:00:00.000000 einops-0.6.2rc0/einops/layers/gluon.py
--rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 einops-0.6.2rc0/einops/layers/keras.py
--rw-r--r--   0        0        0     2046 2020-02-02 00:00:00.000000 einops-0.6.2rc0/einops/layers/oneflow.py
--rw-r--r--   0        0        0     2063 2020-02-02 00:00:00.000000 einops-0.6.2rc0/einops/layers/paddle.py
--rw-r--r--   0        0        0     3299 2020-02-02 00:00:00.000000 einops-0.6.2rc0/einops/layers/tensorflow.py
--rw-r--r--   0        0        0     2595 2020-02-02 00:00:00.000000 einops-0.6.2rc0/einops/layers/torch.py
--rw-r--r--   0        0        0      953 2020-02-02 00:00:00.000000 einops-0.6.2rc0/scripts/convert_readme.py
--rw-r--r--   0        0        0      881 2020-02-02 00:00:00.000000 einops-0.6.2rc0/scripts/setup.py
--rw-r--r--   0        0        0     3372 2020-02-02 00:00:00.000000 einops-0.6.2rc0/tests/__init__.py
--rw-r--r--   0        0        0    11438 2020-02-02 00:00:00.000000 einops-0.6.2rc0/tests/test_einsum.py
--rw-r--r--   0        0        0    11284 2020-02-02 00:00:00.000000 einops-0.6.2rc0/tests/test_examples.py
--rw-r--r--   0        0        0    17525 2020-02-02 00:00:00.000000 einops-0.6.2rc0/tests/test_layers.py
--rw-r--r--   0        0        0     2430 2020-02-02 00:00:00.000000 einops-0.6.2rc0/tests/test_notebooks.py
--rw-r--r--   0        0        0    22261 2020-02-02 00:00:00.000000 einops-0.6.2rc0/tests/test_ops.py
--rw-r--r--   0        0        0    10986 2020-02-02 00:00:00.000000 einops-0.6.2rc0/tests/test_other.py
--rw-r--r--   0        0        0     9273 2020-02-02 00:00:00.000000 einops-0.6.2rc0/tests/test_packing.py
--rw-r--r--   0        0        0     4303 2020-02-02 00:00:00.000000 einops-0.6.2rc0/tests/test_parsing.py
--rw-r--r--   0        0        0     1491 2020-02-02 00:00:00.000000 einops-0.6.2rc0/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 einops-0.6.2rc0/LICENSE
--rw-r--r--   0        0        0    12282 2020-02-02 00:00:00.000000 einops-0.6.2rc0/README.md
--rw-r--r--   0        0        0     2540 2020-02-02 00:00:00.000000 einops-0.6.2rc0/pyproject.toml
--rw-r--r--   0        0        0    12829 2020-02-02 00:00:00.000000 einops-0.6.2rc0/PKG-INFO
+-rw-r--r--   0        0        0     1293 2020-02-02 00:00:00.000000 einops-0.7.0rc1/mkdocs.yml
+-rw-r--r--   0        0        0     2925 2020-02-02 00:00:00.000000 einops-0.7.0rc1/test.py
+-rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 einops-0.7.0rc1/einops/__init__.py
+-rw-r--r--   0        0        0    19559 2020-02-02 00:00:00.000000 einops-0.7.0rc1/einops/_backends.py
+-rw-r--r--   0        0        0     4138 2020-02-02 00:00:00.000000 einops-0.7.0rc1/einops/_torch_specific.py
+-rw-r--r--   0        0        0     5211 2020-02-02 00:00:00.000000 einops-0.7.0rc1/einops/array_api.py
+-rw-r--r--   0        0        0    36464 2020-02-02 00:00:00.000000 einops-0.7.0rc1/einops/einops.py
+-rw-r--r--   0        0        0     7668 2020-02-02 00:00:00.000000 einops-0.7.0rc1/einops/packing.py
+-rw-r--r--   0        0        0     6717 2020-02-02 00:00:00.000000 einops-0.7.0rc1/einops/parsing.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 einops-0.7.0rc1/einops/py.typed
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 einops-0.7.0rc1/einops/experimental/__init__.py
+-rw-r--r--   0        0        0     4690 2020-02-02 00:00:00.000000 einops-0.7.0rc1/einops/experimental/data_api_packing.py
+-rw-r--r--   0        0        0    14777 2020-02-02 00:00:00.000000 einops-0.7.0rc1/einops/experimental/indexing.py
+-rw-r--r--   0        0        0     3747 2020-02-02 00:00:00.000000 einops-0.7.0rc1/einops/layers/__init__.py
+-rw-r--r--   0        0        0     8578 2020-02-02 00:00:00.000000 einops-0.7.0rc1/einops/layers/_einmix.py
+-rw-r--r--   0        0        0     1981 2020-02-02 00:00:00.000000 einops-0.7.0rc1/einops/layers/chainer.py
+-rw-r--r--   0        0        0     2621 2020-02-02 00:00:00.000000 einops-0.7.0rc1/einops/layers/flax.py
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 einops-0.7.0rc1/einops/layers/keras.py
+-rw-r--r--   0        0        0     2046 2020-02-02 00:00:00.000000 einops-0.7.0rc1/einops/layers/oneflow.py
+-rw-r--r--   0        0        0     2063 2020-02-02 00:00:00.000000 einops-0.7.0rc1/einops/layers/paddle.py
+-rw-r--r--   0        0        0     3299 2020-02-02 00:00:00.000000 einops-0.7.0rc1/einops/layers/tensorflow.py
+-rw-r--r--   0        0        0     2595 2020-02-02 00:00:00.000000 einops-0.7.0rc1/einops/layers/torch.py
+-rw-r--r--   0        0        0      953 2020-02-02 00:00:00.000000 einops-0.7.0rc1/scripts/convert_readme.py
+-rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 einops-0.7.0rc1/scripts/setup.py
+-rw-r--r--   0        0        0     3292 2020-02-02 00:00:00.000000 einops-0.7.0rc1/tests/__init__.py
+-rw-r--r--   0        0        0    11438 2020-02-02 00:00:00.000000 einops-0.7.0rc1/tests/test_einsum.py
+-rw-r--r--   0        0        0    11284 2020-02-02 00:00:00.000000 einops-0.7.0rc1/tests/test_examples.py
+-rw-r--r--   0        0        0    15495 2020-02-02 00:00:00.000000 einops-0.7.0rc1/tests/test_layers.py
+-rw-r--r--   0        0        0     2430 2020-02-02 00:00:00.000000 einops-0.7.0rc1/tests/test_notebooks.py
+-rw-r--r--   0        0        0    24123 2020-02-02 00:00:00.000000 einops-0.7.0rc1/tests/test_ops.py
+-rw-r--r--   0        0        0    10986 2020-02-02 00:00:00.000000 einops-0.7.0rc1/tests/test_other.py
+-rw-r--r--   0        0        0    10381 2020-02-02 00:00:00.000000 einops-0.7.0rc1/tests/test_packing.py
+-rw-r--r--   0        0        0     4303 2020-02-02 00:00:00.000000 einops-0.7.0rc1/tests/test_parsing.py
+-rw-r--r--   0        0        0     1491 2020-02-02 00:00:00.000000 einops-0.7.0rc1/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 einops-0.7.0rc1/LICENSE
+-rw-r--r--   0        0        0    12538 2020-02-02 00:00:00.000000 einops-0.7.0rc1/README.md
+-rw-r--r--   0        0        0     2572 2020-02-02 00:00:00.000000 einops-0.7.0rc1/pyproject.toml
+-rw-r--r--   0        0        0    13085 2020-02-02 00:00:00.000000 einops-0.7.0rc1/PKG-INFO
```

### Comparing `einops-0.6.2rc0/mkdocs.yml` & `einops-0.7.0rc1/mkdocs.yml`

 * *Files 5% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 extra:
   search:
     language: en
 markdown_extensions:
   - admonition
   - codehilite
   - pymdownx.arithmatex
+  - markdown.extensions.md_in_html
 plugins:
   - search
   - mkdocstrings
   - mkdocs-jupyter
 extra_javascript:
   - https://cdnjs.cloudflare.com/ajax/libs/mathjax/2.7.0/MathJax.js?config=TeX-MML-AM_CHTML
 extra_css:
```

### Comparing `einops-0.6.2rc0/test.py` & `einops-0.7.0rc1/test.py`

 * *Files identical despite different names*

### Comparing `einops-0.6.2rc0/einops/_backends.py` & `einops-0.7.0rc1/einops/_backends.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,59 +8,68 @@
 - backend should be either symbolic or imperative (tensorflow is for both, but that causes problems)
     - this determines which methods (from_numpy/to_numpy or create_symbol/eval_symbol) should be defined
 - if backend can't (temporarily) provide symbols for shape dimensions, UnknownSize objects are used
 """
 
 import sys
 
-__author__ = 'Alex Rogozhnikov'
+__author__ = "Alex Rogozhnikov"
 
-_backends: dict = {}
+_loaded_backends: dict = {}
+_type2backend: dict = {}
 _debug_importing = False
 
 
-def get_backend(tensor) -> 'AbstractBackend':
+def get_backend(tensor) -> "AbstractBackend":
     """
     Takes a correct backend (e.g. numpy backend if tensor is numpy.ndarray) for a tensor.
     If needed, imports package and creates backend
     """
-    for framework_name, backend in _backends.items():
+    _type = type(tensor)
+    _result = _type2backend.get(_type, None)
+    if _result is not None:
+        return _result
+
+    for framework_name, backend in _loaded_backends.items():
         if backend.is_appropriate_type(tensor):
+            _type2backend[_type] = backend
             return backend
 
     # Find backend subclasses recursively
     backend_subclasses = []
     backends = AbstractBackend.__subclasses__()
     while backends:
         backend = backends.pop()
         backends += backend.__subclasses__()
         backend_subclasses.append(backend)
 
     for BackendSubclass in backend_subclasses:
         if _debug_importing:
-            print('Testing for subclass of ', BackendSubclass)
-        if BackendSubclass.framework_name not in _backends:
+            print("Testing for subclass of ", BackendSubclass)
+        if BackendSubclass.framework_name not in _loaded_backends:
             # check that module was already imported. Otherwise it can't be imported
             if BackendSubclass.framework_name in sys.modules:
                 if _debug_importing:
-                    print('Imported backend for ', BackendSubclass.framework_name)
+                    print("Imported backend for ", BackendSubclass.framework_name)
                 backend = BackendSubclass()
-                _backends[backend.framework_name] = backend
+                _loaded_backends[backend.framework_name] = backend
                 if backend.is_appropriate_type(tensor):
+                    _type2backend[_type] = backend
                     return backend
 
-    raise RuntimeError('Tensor type unknown to einops {}'.format(type(tensor)))
+    raise RuntimeError("Tensor type unknown to einops {}".format(type(tensor)))
 
 
 class AbstractBackend:
-    """ Base backend class, major part of methods are only for debugging purposes. """
+    """Base backend class, major part of methods are only for debugging purposes."""
+
     framework_name: str
 
     def is_appropriate_type(self, tensor):
-        """ helper method should recognize tensors it can handle """
+        """helper method should recognize tensors it can handle"""
         raise NotImplementedError()
 
     def from_numpy(self, x):
         raise NotImplementedError("framework doesn't support imperative execution")
 
     def to_numpy(self, x):
         raise NotImplementedError("framework doesn't support imperative execution")
@@ -98,19 +107,19 @@
         repeats = [1] * n_axes
         for axis_position, axis_length in pos2len.items():
             x = self.add_axis(x, axis_position)
             repeats[axis_position] = axis_length
         return self.tile(x, tuple(repeats))
 
     def tile(self, x, repeats):
-        """repeats is a number of  """
+        """repeats - same lengths as x.shape"""
         raise NotImplementedError()
 
     def concat(self, tensors, axis: int):
-        """ concatenates tensors along axis.
+        """concatenates tensors along axis.
         Assume identical across tensors: devices, dtypes and shapes except selected axis."""
         raise NotImplementedError()
 
     def is_float_type(self, x):
         # some backends (torch) can't compute average for non-floating types.
         # Decided to drop average for all backends if type is not floating
         raise NotImplementedError()
@@ -122,15 +131,15 @@
         return "<einops backend for {}>".format(self.framework_name)
 
     def einsum(self, pattern, *x):
         raise NotImplementedError("backend does not support einsum")
 
 
 class UnknownSize:
-    """ pseudo-symbol for symbolic frameworks which do not provide symbols for shape elements """
+    """pseudo-symbol for symbolic frameworks which do not provide symbols for shape elements"""
 
     def __floordiv__(self, other):
         return self
 
     def __eq__(self, other):
         return True  # we don't know actual size
 
@@ -141,18 +150,19 @@
         return self
 
     def __hash__(self):
         return hash(None)
 
 
 class NumpyBackend(AbstractBackend):
-    framework_name = 'numpy'
+    framework_name = "numpy"
 
     def __init__(self):
         import numpy
+
         self.np = numpy
 
     def is_appropriate_type(self, tensor):
         return isinstance(tensor, self.np.ndarray)
 
     def from_numpy(self, x):
         return x
@@ -169,94 +179,50 @@
     def tile(self, x, repeats):
         return self.np.tile(x, repeats)
 
     def concat(self, tensors, axis: int):
         return self.np.concatenate(tensors, axis=axis)
 
     def is_float_type(self, x):
-        return x.dtype in ('float16', 'float32', 'float64', 'float128', 'bfloat16')
+        return x.dtype in ("float16", "float32", "float64", "float128", "bfloat16")
 
     def add_axis(self, x, new_position):
         return self.np.expand_dims(x, new_position)
 
     def einsum(self, pattern, *x):
         return self.np.einsum(pattern, *x)
 
 
 class JaxBackend(NumpyBackend):
-    framework_name = 'jax'
+    framework_name = "jax"
 
     def __init__(self):
         super(JaxBackend, self).__init__()
         self.onp = self.np
 
         import jax.numpy
+
         self.np = jax.numpy
 
     def from_numpy(self, x):
         return self.np.asarray(x)
 
     def to_numpy(self, x):
         return self.onp.asarray(x)
 
 
-class GluonBackend(AbstractBackend):
-    framework_name = 'mxnet.ndarray'
-
-    def __init__(self):
-        import mxnet
-        self.mx = mxnet
-
-    def is_appropriate_type(self, tensor):
-        return isinstance(tensor, self.mx.nd.NDArray)
-
-    def from_numpy(self, x):
-        if len(x.shape) == 0:
-            x = x[None]  # poor support of scalars in mxnet, otherwise mxnet can't attach gradients
-        var = self.mx.nd.array(x, dtype=x.dtype)
-        var.attach_grad()
-        return var
-
-    def to_numpy(self, x):
-        return self.mx.nd.NDArray.asnumpy(x)
-
-    def reshape(self, x, shape):
-        if len(shape) == 0:
-            return x  # poor support of scalars in mxnet
-        return x.reshape(shape)
-
-    def arange(self, start, stop):
-        return self.mx.nd.arange(start, stop)
-
-    def stack_on_zeroth_dimension(self, tensors: list):
-        return self.mx.nd.stack(*tensors)
-
-    def tile(self, x, repeats):
-        return self.mx.nd.tile(x, repeats)
-
-    def concat(self, tensors, axis: int):
-        return self.mx.nd.concat(*tensors, dim=axis)
-
-    def add_axis(self, x, new_position):
-        return self.mx.nd.expand_dims(x, new_position)
-
-    def is_float_type(self, x):
-        return 'float' in str(x.dtype)
-
-    def layers(self):
-        from .layers import gluon
-        return gluon
-
-
 class TorchBackend(AbstractBackend):
-    framework_name = 'torch'
+    framework_name = "torch"
 
     def __init__(self):
         import torch
+
         self.torch = torch
+        # importing would register operations in torch._dynamo for torch.compile
+        from . import _torch_specific  # noqa
 
     def is_appropriate_type(self, tensor):
         return isinstance(tensor, self.torch.Tensor)
 
     def from_numpy(self, x):
         variable = self.torch.from_numpy(x)
         if self.is_float_type(variable):
@@ -267,28 +233,28 @@
     def to_numpy(self, x):
         return x.detach().cpu().numpy()
 
     def arange(self, start, stop):
         return self.torch.arange(start, stop, dtype=self.torch.int64)
 
     def reduce(self, x, operation, reduced_axes):
-        if operation == 'min':
+        if operation == "min":
             return x.amin(dim=reduced_axes)
-        elif operation == 'max':
+        elif operation == "max":
             return x.amax(dim=reduced_axes)
-        elif operation == 'sum':
+        elif operation == "sum":
             return x.sum(dim=reduced_axes)
-        elif operation == 'mean':
+        elif operation == "mean":
             return x.mean(dim=reduced_axes)
-        elif operation == 'prod':
+        elif operation == "prod":
             for i in list(sorted(reduced_axes))[::-1]:
                 x = x.prod(dim=i)
             return x
         else:
-            raise NotImplementedError('Unknown reduction ', operation)
+            raise NotImplementedError("Unknown reduction ", operation)
 
     def transpose(self, x, axes):
         return x.permute(axes)
 
     def stack_on_zeroth_dimension(self, tensors: list):
         return self.torch.stack(tensors)
 
@@ -309,25 +275,27 @@
         return self.torch.unsqueeze(x, new_position)
 
     def is_float_type(self, x):
         return x.dtype in [self.torch.float16, self.torch.float32, self.torch.float64, self.torch.bfloat16]
 
     def layers(self):
         from .layers import torch
+
         return torch
 
     def einsum(self, pattern, *x):
         return self.torch.einsum(pattern, *x)
 
 
 class CupyBackend(AbstractBackend):
-    framework_name = 'cupy'
+    framework_name = "cupy"
 
     def __init__(self):
         import cupy
+
         self.cupy = cupy
 
     def is_appropriate_type(self, tensor):
         return isinstance(tensor, self.cupy.ndarray)
 
     def from_numpy(self, x):
         return self.cupy.asarray(x)
@@ -347,34 +315,35 @@
     def concat(self, tensors, axis: int):
         return self.cupy.concatenate(tensors, axis=axis)
 
     def add_axis(self, x, new_position):
         return self.cupy.expand_dims(x, new_position)
 
     def is_float_type(self, x):
-        return x.dtype in ('float16', 'float32', 'float64', 'float128', 'bfloat16')
+        return x.dtype in ("float16", "float32", "float64", "float128", "bfloat16")
 
     def einsum(self, pattern, *x):
         return self.cupy.einsum(pattern, *x)
 
 
 class ChainerBackend(AbstractBackend):
-    framework_name = 'chainer'
+    framework_name = "chainer"
 
     def __init__(self):
         import chainer
         import numpy
+
         self.numpy = numpy
         self.chainer = chainer
 
     def is_appropriate_type(self, tensor):
         return isinstance(tensor, self.chainer.Variable)
 
     def from_numpy(self, x):
-        return self.chainer.Variable(x.astype('float32'))
+        return self.chainer.Variable(x.astype("float32"))
 
     def to_numpy(self, x):
         if isinstance(x, self.chainer.Variable):
             x = x.data
         return x
 
     def arange(self, start, stop):
@@ -392,18 +361,19 @@
     def concat(self, tensors, axis: int):
         return self.chainer.functions.concat(tensors, axis=axis)
 
     def add_axis(self, x, new_position):
         return self.chainer.functions.expand_dims(x, new_position)
 
     def is_float_type(self, x):
-        return x.dtype in ('float16', 'float32', 'float64', 'float128', 'bfloat16')
+        return x.dtype in ("float16", "float32", "float64", "float128", "bfloat16")
 
     def layers(self):
         from .layers import chainer
+
         return chainer
 
     def einsum(self, pattern, *x):
         return self.chainer.functions.einsum(pattern, *x)
 
 
 class HashableTuple:
@@ -420,18 +390,19 @@
         return len(self.elements)
 
     def __getitem__(self, item):
         return self.elements[item]
 
 
 class TensorflowBackend(AbstractBackend):
-    framework_name = 'tensorflow'
+    framework_name = "tensorflow"
 
     def __init__(self):
         import tensorflow
+
         self.tf = tensorflow
 
     def is_appropriate_type(self, tensor):
         return isinstance(tensor, (self.tf.Tensor, self.tf.Variable))
 
     def from_numpy(self, x):
         assert self.tf.executing_eagerly()
@@ -456,15 +427,15 @@
                 hash(shape)
                 return shape
             except:
                 # unhashable symbols in shape. Wrap tuple to be hashable.
                 return HashableTuple(shape)
 
     def reduce(self, x, operation, axes):
-        return getattr(self.tf, 'reduce_' + operation)(x, axis=axes)
+        return getattr(self.tf, "reduce_" + operation)(x, axis=axes)
 
     def reshape(self, x, shape):
         return self.tf.reshape(x, shape)
 
     def transpose(self, x, axes):
         return self.tf.transpose(x, axes)
 
@@ -477,29 +448,31 @@
     def concat(self, tensors, axis: int):
         return self.tf.concat(tensors, axis=axis)
 
     def add_axis(self, x, new_position):
         return self.tf.expand_dims(x, new_position)
 
     def is_float_type(self, x):
-        return x.dtype in ('float16', 'float32', 'float64', 'float128', 'bfloat16')
+        return x.dtype in ("float16", "float32", "float64", "float128", "bfloat16")
 
     def layers(self):
         from .layers import tensorflow
+
         return tensorflow
 
     def einsum(self, pattern, *x):
         return self.tf.einsum(pattern, *x)
 
 
 class KerasBackend(AbstractBackend):
-    framework_name = 'tensorflow.keras'
+    framework_name = "tensorflow.keras"
 
     def __init__(self):
         import tensorflow as tf
+
         self.tf = tf
         self.keras = tf.keras
         self.K = tf.keras.backend
 
     def is_appropriate_type(self, tensor):
         return self.tf.is_tensor(tensor) and self.K.is_keras_tensor(tensor)
 
@@ -535,26 +508,28 @@
     def concat(self, tensors, axis: int):
         return self.K.concatenate(tensors, axis=axis)
 
     def add_axis(self, x, new_position):
         return self.K.expand_dims(x, new_position)
 
     def is_float_type(self, x):
-        return 'float' in self.K.dtype(x)
+        return "float" in self.K.dtype(x)
 
     def layers(self):
         from .layers import keras
+
         return keras
 
 
 class OneFlowBackend(AbstractBackend):
     framework_name = "oneflow"
 
     def __init__(self):
         import oneflow as flow
+
         self.flow = flow
 
     def is_appropriate_type(self, tensor):
         return isinstance(tensor, self.flow.Tensor)
 
     def from_numpy(self, x):
         variable = self.flow.from_numpy(x)
@@ -567,22 +542,22 @@
         return x.detach().cpu().numpy()
 
     def arange(self, start, stop):
         return self.flow.arange(start, stop, dtype=self.flow.int64)
 
     def reduce(self, x, operation, reduced_axes):
         for axis in sorted(reduced_axes, reverse=True):
-            if operation == 'min':
+            if operation == "min":
                 x, _ = x.min(dim=axis)
-            elif operation == 'max':
+            elif operation == "max":
                 x, _ = x.max(dim=axis)
-            elif operation in ['sum', 'mean', 'prod']:
+            elif operation in ["sum", "mean", "prod"]:
                 x = getattr(x, operation)(dim=axis)
             else:
-                raise NotImplementedError('Unknown reduction ', operation)
+                raise NotImplementedError("Unknown reduction ", operation)
         return x
 
     def transpose(self, x, axes):
         return x.permute(axes)
 
     def stack_on_zeroth_dimension(self, tensors: list):
         return self.flow.stack(tensors)
@@ -604,25 +579,27 @@
         return self.flow.unsqueeze(x, new_position)
 
     def is_float_type(self, x):
         return x.dtype in [self.flow.float16, self.flow.float32, self.flow.float64]
 
     def layers(self):
         from .layers import oneflow
+
         return oneflow
 
     def einsum(self, pattern, *x):
         return self.flow.einsum(pattern, *x)
 
 
 class PaddleBackend(AbstractBackend):
     framework_name = "paddle"
 
     def __init__(self):
         import paddle
+
         self.paddle = paddle
 
     def is_appropriate_type(self, tensor):
         return isinstance(tensor, (self.paddle.Tensor, self.paddle.static.Variable))
 
     def from_numpy(self, x):
         tensor = self.paddle.to_tensor(x)
@@ -668,14 +645,15 @@
         return x.unsqueeze(new_position)
 
     def is_float_type(self, x):
         return x.dtype in [self.paddle.float16, self.paddle.float32, self.paddle.float64]
 
     def layers(self):
         from .layers import paddle
+
         return paddle
 
     def einsum(self, pattern, *x):
         return self.paddle.einsum(pattern, *x)
 
     def shape(self, x):
         return tuple(x.shape)
```

### Comparing `einops-0.6.2rc0/einops/_torch_specific.py` & `einops-0.7.0rc1/einops/_torch_specific.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 Specialization of einops for torch.
 
 Unfortunately, torch's jit scripting mechanism isn't strong enough,
 and to have scripting supported at least for layers,
 a number of additional moves is needed.
 
 Design of main operations (dynamic resolution by lookup) is unlikely
-to be implemented by torch.jit.script, but torch.compile seems to work completely fine.
+to be implemented by torch.jit.script, 
+but torch.compile seems to work with operations just fine.
 """
 import warnings
 from typing import Dict, List, Tuple
 
 import torch
 from einops.einops import TransformRecipe, _reconstruct_from_shape_uncached
 
@@ -94,21 +95,33 @@
         tensor = backend.add_axes(tensor, n_axes=n_axes_w_added, pos2len=added_axes)
     if final_shapes is not None:
         tensor = backend.reshape(tensor, final_shapes)
     return tensor
 
 
 def allow_ops_in_compiled_graph():
+    if hasattr(torch, "__version__") and torch.__version__[0] < "2":
+        # torch._dynamo and torch.compile appear in pytorch 2.0
+        return
     try:
         from torch._dynamo import allow_in_graph
     except ImportError:
         warnings.warn("allow_ops_in_compiled_graph failed to import torch: ensure pytorch >=2.0", ImportWarning)
+        return
 
     from .einops import rearrange, reduce, repeat, einsum
     from .packing import pack, unpack
 
     allow_in_graph(rearrange)
     allow_in_graph(reduce)
     allow_in_graph(repeat)
     allow_in_graph(einsum)
     allow_in_graph(pack)
     allow_in_graph(unpack)
+
+    # CF: https://github.com/pytorch/pytorch/blob/2df939aacac68e9621fbd5d876c78d86e72b41e2/torch/_dynamo/__init__.py#L222
+    global _ops_were_registered_in_torchdynamo
+    _ops_were_registered_in_torchdynamo = True
+
+
+# module import automatically registers ops in torchdynamo
+allow_ops_in_compiled_graph()
```

### Comparing `einops-0.6.2rc0/einops/einops.py` & `einops-0.7.0rc1/einops/einops.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import itertools
 import string
 import typing
 from collections import OrderedDict
 from typing import Set, Tuple, List, Dict, Union, Callable, Optional, TypeVar, cast, Any
 
 if typing.TYPE_CHECKING:
+    # for docstrings in pycharm
     import numpy as np
 
 from . import EinopsError
 from ._backends import get_backend
 from .parsing import ParsedExpression, _ellipsis, AnonymousAxis
 
 Tensor = TypeVar("Tensor")
@@ -34,16 +35,14 @@
 
 def _reduce_axes(tensor, reduction_type: Reduction, reduced_axes: List[int], backend):
     if callable(reduction_type):
         # custom callable
         return reduction_type(tensor, tuple(reduced_axes))
     else:
         # one of built-in operations
-        if len(reduced_axes) == 0:
-            return tensor
         assert reduction_type in _reductions
         if reduction_type == "mean":
             if not backend.is_float_type(tensor):
                 raise NotImplementedError("reduce_mean is not available for non-floating tensors")
         return backend.reduce(tensor, reduction_type, tuple(reduced_axes))
 
 
@@ -98,18 +97,21 @@
                 else:
                     axes_reordering.append(axis - 1)
             init_axis_to_final_axis = build_mapping()
 
     return init_shapes, reduced_axes, axes_reordering, final_shapes
 
 
-# This
 CookedRecipe = Tuple[Optional[List[int]], Optional[List[int]], List[int], Dict[int, int], Optional[List[int]], int]
 
-HashableAxesLengths = List[Tuple[str, int]]
+# Actual type is tuple[tuple[str, int], ...]
+# However torch.jit.script does not "understand" the correct type,
+# and torch_specific will use list version.
+HashableAxesLengths = Tuple[Tuple[str, int], ...]
+FakeHashableAxesLengths = List[Tuple[str, int]]
 
 
 class TransformRecipe:
     """
     Recipe describes actual computation pathway.
     Recipe can be applied to a tensor or variable.
     """
@@ -146,15 +148,15 @@
 
         self.first_reduced_axis: int = first_reduced_axis
         self.added_axes: Dict[int, int] = added_axes
         self.output_composite_axes: List[List[int]] = output_composite_axes
 
 
 def _reconstruct_from_shape_uncached(
-    self: TransformRecipe, shape: List[int], axes_dims: HashableAxesLengths
+    self: TransformRecipe, shape: List[int], axes_dims: FakeHashableAxesLengths
 ) -> CookedRecipe:
     """
     Reconstruct all actual parameters using shape.
     Shape is a tuple that may contain integers, shape symbols (tf, theano) and UnknownSize (tf, previously mxnet)
     known axes can be integers or symbols, but not Nones.
     """
     # magic number
@@ -223,15 +225,15 @@
 
 _reconstruct_from_shape = functools.lru_cache(1024)(_reconstruct_from_shape_uncached)
 
 
 def _apply_recipe(
     backend, recipe: TransformRecipe, tensor: Tensor, reduction_type: Reduction, axes_lengths: HashableAxesLengths
 ) -> Tensor:
-    # this method works for all backends but not compilable with
+    # this method implements actual work for all backends for 3 operations
     init_shapes, axes_reordering, reduced_axes, added_axes, final_shapes, n_axes_w_added = _reconstruct_from_shape(
         recipe, backend.shape(tensor), axes_lengths
     )
     if init_shapes is not None:
         tensor = backend.reshape(tensor, init_shapes)
     if axes_reordering is not None:
         tensor = backend.transpose(tensor, axes_reordering)
@@ -240,14 +242,48 @@
     if len(added_axes) > 0:
         tensor = backend.add_axes(tensor, n_axes=n_axes_w_added, pos2len=added_axes)
     if final_shapes is not None:
         tensor = backend.reshape(tensor, final_shapes)
     return tensor
 
 
+def _apply_recipe_array_api(
+    xp, recipe: TransformRecipe, tensor: Tensor, reduction_type: Reduction, axes_lengths: HashableAxesLengths
+) -> Tensor:
+    # completely-inline implementation
+    init_shapes, axes_reordering, reduced_axes, added_axes, final_shapes, n_axes_w_added = _reconstruct_from_shape(
+        recipe, tensor.shape, axes_lengths
+    )
+    if init_shapes is not None:
+        tensor = xp.reshape(tensor, init_shapes)
+    if axes_reordering is not None:
+        tensor = xp.permute_dims(tensor, axes_reordering)
+    if len(reduced_axes) > 0:
+        if callable(reduction_type):
+            # custom callable
+            tensor = reduction_type(tensor, tuple(reduced_axes))
+        else:
+            # one of built-in operations
+            assert reduction_type in _reductions
+            tensor = getattr(xp, reduction_type)(tensor, axis=tuple(reduced_axes))
+    if len(added_axes) > 0:
+        # we use broadcasting
+        for axis_position, axis_length in added_axes.items():
+            tensor = xp.expand_dims(tensor, axis=axis_position)
+
+        final_shape = list(tensor.shape)
+        for axis_position, axis_length in added_axes.items():
+            final_shape[axis_position] = axis_length
+
+        tensor = xp.broadcast_to(tensor, final_shape)
+    if final_shapes is not None:
+        tensor = xp.reshape(tensor, final_shapes)
+    return tensor
+
+
 @functools.lru_cache(256)
 def _prepare_transformation_recipe(
     pattern: str,
     operation: Reduction,
     axes_names: Tuple[str, ...],
     ndim: int,
 ) -> TransformRecipe:
@@ -396,33 +432,30 @@
         axes_permutation=axes_permutation,
         first_reduced_axis=first_reduced_axis,
         added_axes=added_axes,
         output_composite_axes=result_axes_grouping,
     )
 
 
-# TODO multi-recipe should be recomputed when a layer is unpickled.
-
-
 def _prepare_recipes_for_all_dims(
     pattern: str, operation: Reduction, axes_names: Tuple[str, ...]
 ) -> Dict[int, TransformRecipe]:
     """
-    Function to be used in layers.
-    Layer makes all recipe creation when it is initialized, thus to keep recipes simple we pre-compute for all dimensions.
+    Internal function, used in layers.
+    Layer makes all recipe creation when it is initialized, thus to keep recipes simple we pre-compute for all dims
     """
     left_str, rght_str = pattern.split("->")
     left = ParsedExpression(left_str)
     dims = [len(left.composition)]
     if left.has_ellipsis:
         dims = [len(left.composition) - 1 + ellipsis_dims for ellipsis_dims in range(8)]
     return {ndim: _prepare_transformation_recipe(pattern, operation, axes_names, ndim=ndim) for ndim in dims}
 
 
-def reduce(tensor: Tensor, pattern: str, reduction: Reduction, **axes_lengths: int) -> Tensor:
+def reduce(tensor: Union[Tensor, List[Tensor]], pattern: str, reduction: Reduction, **axes_lengths: int) -> Tensor:
     """
     einops.reduce provides combination of reordering and reduction using reader-friendly notation.
 
     Examples for reduce operation:
 
     ```python
     >>> x = np.random.randn(100, 32, 64)
@@ -467,19 +500,28 @@
             This allows using various reductions, examples: np.max, tf.reduce_logsumexp, torch.var, etc.
         axes_lengths: any additional specifications for dimensions
 
     Returns:
         tensor of the same type as input
     """
     try:
-        hashable_axes_lengths = tuple(sorted(axes_lengths.items()))
-        backend = get_backend(tensor)
+        if isinstance(tensor, list):
+            if len(tensor) == 0:
+                raise TypeError("Rearrange/Reduce/Repeat can't be applied to an empty list")
+            backend = get_backend(tensor[0])
+            tensor = backend.stack_on_zeroth_dimension(tensor)
+        else:
+            backend = get_backend(tensor)
+
+        hashable_axes_lengths = tuple(axes_lengths.items())
         shape = backend.shape(tensor)
         recipe = _prepare_transformation_recipe(pattern, reduction, axes_names=tuple(axes_lengths), ndim=len(shape))
-        return _apply_recipe(backend, recipe, tensor, reduction_type=reduction, axes_lengths=hashable_axes_lengths)
+        return _apply_recipe(
+            backend, recipe, cast(Tensor, tensor), reduction_type=reduction, axes_lengths=hashable_axes_lengths
+        )
     except EinopsError as e:
         message = ' Error while processing {}-reduction pattern "{}".'.format(reduction, pattern)
         if not isinstance(tensor, list):
             message += "\n Input tensor shape: {}. ".format(shape)
         else:
             message += "\n Input is list. "
         message += "Additional info: {}.".format(axes_lengths)
@@ -537,22 +579,18 @@
         pattern: string, rearrangement pattern
         axes_lengths: any additional specifications for dimensions
 
     Returns:
         tensor of the same type as input. If possible, a view to the original tensor is returned.
 
     """
-    if isinstance(tensor, list):
-        if len(tensor) == 0:
-            raise TypeError("Rearrange can't be applied to an empty list")
-        tensor = get_backend(tensor[0]).stack_on_zeroth_dimension(tensor)
-    return reduce(cast(Tensor, tensor), pattern, reduction="rearrange", **axes_lengths)
+    return reduce(tensor, pattern, reduction="rearrange", **axes_lengths)
 
 
-def repeat(tensor: Tensor, pattern: str, **axes_lengths) -> Tensor:
+def repeat(tensor: Union[Tensor, List[Tensor]], pattern: str, **axes_lengths) -> Tensor:
     """
     einops.repeat allows reordering elements and repeating them in arbitrary combinations.
     This operation includes functionality of repeat, tile, broadcast functions.
 
     Examples for repeat operation:
 
     ```python
@@ -614,15 +652,15 @@
     (2, 10, 5, 7)
 
     ```
 
     For symbolic frameworks may return symbols, not integers.
 
     Parameters:
-        x: tensor of any of supported frameworks
+        x: tensor of any supported framework
         pattern: str, space separated names for axes, underscore means skip axis
 
     Returns:
         dict, maps axes names to their lengths
     """
     exp = ParsedExpression(pattern, allow_underscore=True)
     shape = get_backend(x).shape(x)
@@ -678,15 +716,15 @@
 
 
 def asnumpy(tensor) -> np_ndarray:
     """
     Convert a tensor of an imperative framework (i.e. numpy/cupy/torch/jax/etc.) to `numpy.ndarray`
 
     Parameters:
-        tensor: tensor of any of known imperative framework
+        tensor: tensor of any known imperative framework
 
     Returns:
         `numpy.ndarray`, converted to numpy
     """
     return get_backend(tensor).to_numpy(tensor)
```

### Comparing `einops-0.6.2rc0/einops/packing.py` & `einops-0.7.0rc1/einops/packing.py`

 * *Files identical despite different names*

### Comparing `einops-0.6.2rc0/einops/parsing.py` & `einops-0.7.0rc1/einops/parsing.py`

 * *Files identical despite different names*

### Comparing `einops-0.6.2rc0/einops/experimental/data_api_packing.py` & `einops-0.7.0rc1/einops/experimental/data_api_packing.py`

 * *Files identical despite different names*

### Comparing `einops-0.6.2rc0/einops/experimental/indexing.py` & `einops-0.7.0rc1/einops/experimental/indexing.py`

 * *Files identical despite different names*

### Comparing `einops-0.6.2rc0/einops/layers/__init__.py` & `einops-0.7.0rc1/einops/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `einops-0.6.2rc0/einops/layers/_einmix.py` & `einops-0.7.0rc1/einops/layers/_einmix.py`

 * *Files identical despite different names*

### Comparing `einops-0.6.2rc0/einops/layers/chainer.py` & `einops-0.7.0rc1/einops/layers/chainer.py`

 * *Files identical despite different names*

### Comparing `einops-0.6.2rc0/einops/layers/flax.py` & `einops-0.7.0rc1/einops/layers/flax.py`

 * *Files identical despite different names*

### Comparing `einops-0.6.2rc0/einops/layers/oneflow.py` & `einops-0.7.0rc1/einops/layers/oneflow.py`

 * *Files identical despite different names*

### Comparing `einops-0.6.2rc0/einops/layers/paddle.py` & `einops-0.7.0rc1/einops/layers/paddle.py`

 * *Files identical despite different names*

### Comparing `einops-0.6.2rc0/einops/layers/tensorflow.py` & `einops-0.7.0rc1/einops/layers/tensorflow.py`

 * *Files identical despite different names*

### Comparing `einops-0.6.2rc0/einops/layers/torch.py` & `einops-0.7.0rc1/einops/layers/torch.py`

 * *Files identical despite different names*

### Comparing `einops-0.6.2rc0/scripts/convert_readme.py` & `einops-0.7.0rc1/scripts/convert_readme.py`

 * *Files identical despite different names*

### Comparing `einops-0.6.2rc0/tests/__init__.py` & `einops-0.7.0rc1/tests/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -61,25 +61,23 @@
     """
     if not symbolic:
         if not layers:
             backend_types = [
                 _backends.NumpyBackend,
                 _backends.JaxBackend,
                 _backends.TorchBackend,
-                _backends.GluonBackend,
                 _backends.ChainerBackend,
                 _backends.TensorflowBackend,
                 _backends.OneFlowBackend,
                 _backends.PaddleBackend,
                 _backends.CupyBackend,
             ]
         else:
             backend_types = [
                 _backends.TorchBackend,
-                _backends.GluonBackend,
                 _backends.ChainerBackend,
                 _backends.OneFlowBackend,
                 _backends.PaddleBackend,
             ]
     else:
         if not layers:
             backend_types = []
```

### Comparing `einops-0.6.2rc0/tests/test_einsum.py` & `einops-0.7.0rc1/tests/test_einsum.py`

 * *Files identical despite different names*

### Comparing `einops-0.6.2rc0/tests/test_examples.py` & `einops-0.7.0rc1/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `einops-0.6.2rc0/tests/test_layers.py` & `einops-0.7.0rc1/tests/test_layers.py`

 * *Files 13% similar despite different names*

```diff
@@ -286,78 +286,20 @@
         model1.save_weights(tmp_filename)
         model4.load_weights(tmp_filename)
         model2.load_weights(tmp_filename)
         assert numpy.allclose(model1.predict_on_batch(input), model4.predict_on_batch(input))
         assert numpy.allclose(model1.predict_on_batch(input), model2.predict_on_batch(input))
 
 
-def _deprecated_check_gluon_layer():
-    # currently gluon is not tested, and will be removed
-    import mxnet
-    from mxnet.gluon.nn import HybridSequential, Dense, Conv2D, LeakyReLU
-    from einops.layers.gluon import Rearrange, Reduce, EinMix
-    from einops import asnumpy
-
-    def create_model():
-        model = HybridSequential()
-        layers = [
-            Conv2D(6, kernel_size=5),
-            Reduce("b c (h h2) (w w2) -> b c h w", "max", h2=2, w2=2),
-            Conv2D(16, kernel_size=5),
-            Reduce("b c (h h2) (w w2) -> b c h w", "max", h2=2, w2=2),
-            Rearrange("b c h w -> b (c h w)"),
-            Dense(120),
-            LeakyReLU(alpha=0.0),
-            Dense(84),
-            LeakyReLU(alpha=0.0),
-            Dense(10),
-        ]
-        for layer in layers:
-            model.add(layer)
-        model.initialize(mxnet.init.Xavier(), ctx=mxnet.cpu())
-        return model
-
-    model1 = create_model()
-    model2 = create_model()
-    x = mxnet.ndarray.random_normal(shape=[10, 3, 32, 32])
-    assert not numpy.allclose(asnumpy(model1(x)), asnumpy(model2(x)))
-
-    with tempfile.NamedTemporaryFile(mode="r+b") as fp:
-        model1.save_parameters(fp.name)
-        model2.load_parameters(fp.name)
-
-    assert numpy.allclose(asnumpy(model1(x)), asnumpy(model2(x)))
-
-    # testing with symbolic (NB with fixed dimensions!)
-    input = mxnet.sym.Variable("data", shape=x.shape)
-    json = model1(input).tojson()
-    model3 = mxnet.gluon.SymbolBlock(outputs=mxnet.sym.load_json(json), inputs=input)
-    model4 = mxnet.gluon.SymbolBlock(outputs=mxnet.sym.load_json(json), inputs=input)
-    model3.initialize(ctx=mxnet.cpu())
-    model3(x)
-
-    with tempfile.NamedTemporaryFile(mode="r+b") as fp:
-        model3.save_parameters(fp.name)
-        model4.load_parameters(fp.name)
-    assert numpy.allclose(asnumpy(model3(x)), asnumpy(model4(x)))
-
-    try:
-        model1.hybridize(static_alloc=True, static_shape=True)
-        model1(x)
-    except:
-        # hybridization is not supported
-        pass
-
-
 def test_chainer_layer():
     chainer_is_present = any(
         "chainer" in backend.framework_name for backend in collect_test_backends(symbolic=False, layers=True)
     )
     if chainer_is_present:
-        # checked that gluon present
+        # checked that chainer is present
         import chainer
         import chainer.links as L
         import chainer.functions as F
         from einops.layers.chainer import Rearrange, Reduce, EinMix
         from einops import asnumpy
         import numpy as np
```

### Comparing `einops-0.6.2rc0/tests/test_notebooks.py` & `einops-0.7.0rc1/tests/test_notebooks.py`

 * *Files identical despite different names*

### Comparing `einops-0.6.2rc0/tests/test_ops.py` & `einops-0.7.0rc1/tests/test_ops.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,85 +1,84 @@
 import itertools
 
 import numpy
 import pytest
 
 from einops import EinopsError
-from einops.einops import (rearrange, reduce, _enumerate_directions, _reductions)
+from einops.einops import rearrange, reduce, repeat, _enumerate_directions, _reductions
 from . import collect_test_backends
 
 imp_op_backends = collect_test_backends(symbolic=False, layers=False)
 sym_op_backends = collect_test_backends(symbolic=True, layers=False)
 
 identity_patterns = [
-    '...->...',
-    'a b c d e-> a b c d e',
-    'a b c d e ...-> ... a b c d e',
-    'a b c d e ...-> a ... b c d e',
-    '... a b c d e -> ... a b c d e',
-    'a ... e-> a ... e',
-    'a ... -> a ... ',
-    'a ... c d e -> a (...) c d e',
+    "...->...",
+    "a b c d e-> a b c d e",
+    "a b c d e ...-> ... a b c d e",
+    "a b c d e ...-> a ... b c d e",
+    "... a b c d e -> ... a b c d e",
+    "a ... e-> a ... e",
+    "a ... -> a ... ",
+    "a ... c d e -> a (...) c d e",
 ]
 
 equivalent_rearrange_patterns = [
-    ('a b c d e -> (a b) c d e', 'a b ... -> (a b) ... '),
-    ('a b c d e -> a b (c d) e', '... c d e -> ... (c d) e'),
-    ('a b c d e -> a b c d e', '... -> ... '),
-    ('a b c d e -> (a b c d e)', '... ->  (...)'),
-    ('a b c d e -> b (c d e) a', 'a b ... -> b (...) a'),
-    ('a b c d e -> b (a c d) e', 'a b ... e -> b (a ...) e'),
+    ("a b c d e -> (a b) c d e", "a b ... -> (a b) ... "),
+    ("a b c d e -> a b (c d) e", "... c d e -> ... (c d) e"),
+    ("a b c d e -> a b c d e", "... -> ... "),
+    ("a b c d e -> (a b c d e)", "... ->  (...)"),
+    ("a b c d e -> b (c d e) a", "a b ... -> b (...) a"),
+    ("a b c d e -> b (a c d) e", "a b ... e -> b (a ...) e"),
 ]
 
 equivalent_reduction_patterns = [
-    ('a b c d e -> ', ' ... ->  '),
-    ('a b c d e -> (e a)', 'a ... e -> (e a)'),
-    ('a b c d e -> d (a e)', ' a b c d e ... -> d (a e) '),
-    ('a b c d e -> (a b)', ' ... c d e  -> (...) '),
+    ("a b c d e -> ", " ... ->  "),
+    ("a b c d e -> (e a)", "a ... e -> (e a)"),
+    ("a b c d e -> d (a e)", " a b c d e ... -> d (a e) "),
+    ("a b c d e -> (a b)", " ... c d e  -> (...) "),
 ]
 
 
 def test_collapsed_ellipsis_errors_out():
     x = numpy.zeros([1, 1, 1, 1, 1])
-    rearrange(x, 'a b c d ... ->  a b c ... d')
+    rearrange(x, "a b c d ... ->  a b c ... d")
     with pytest.raises(EinopsError):
-        rearrange(x, 'a b c d (...) ->  a b c ... d')
+        rearrange(x, "a b c d (...) ->  a b c ... d")
 
-    rearrange(x, '... ->  (...)')
+    rearrange(x, "... ->  (...)")
     with pytest.raises(EinopsError):
-        rearrange(x, '(...) -> (...)')
+        rearrange(x, "(...) -> (...)")
 
 
 def test_ellipsis_ops_numpy():
     x = numpy.arange(2 * 3 * 4 * 5 * 6).reshape([2, 3, 4, 5, 6])
     for pattern in identity_patterns:
         assert numpy.array_equal(x, rearrange(x, pattern)), pattern
 
     for pattern1, pattern2 in equivalent_rearrange_patterns:
         assert numpy.array_equal(rearrange(x, pattern1), rearrange(x, pattern2))
 
-    for reduction in ['min', 'max', 'sum']:
+    for reduction in ["min", "max", "sum"]:
         for pattern1, pattern2 in equivalent_reduction_patterns:
-            assert numpy.array_equal(reduce(x, pattern1, reduction=reduction),
-                                     reduce(x, pattern2, reduction=reduction))
+            assert numpy.array_equal(reduce(x, pattern1, reduction=reduction), reduce(x, pattern2, reduction=reduction))
 
     # now just check coincidence with numpy
     all_rearrange_patterns = [*identity_patterns]
     for pattern_pairs in equivalent_rearrange_patterns:
         all_rearrange_patterns.extend(pattern_pairs)
 
 
-def check_op_against_numpy(backend, numpy_input, pattern, axes_lengths, reduction='rearrange', is_symbolic=False):
+def check_op_against_numpy(backend, numpy_input, pattern, axes_lengths, reduction="rearrange", is_symbolic=False):
     """
     Helper to test result of operation (rearrange or transpose) against numpy
     if reduction == 'rearrange', rearrange op is tested, otherwise reduce
     """
 
     def operation(x):
-        if reduction == 'rearrange':
+        if reduction == "rearrange":
             return rearrange(x, pattern, **axes_lengths)
         else:
             return reduce(x, pattern, reduction, **axes_lengths)
 
     numpy_result = operation(numpy_input)
     check_equal = numpy.array_equal
     p_none_dimension = 0.5
@@ -92,235 +91,272 @@
         backend_result = operation(backend.from_numpy(numpy_input))
         backend_result = backend.to_numpy(backend_result)
 
     check_equal(numpy_result, backend_result)
 
 
 def test_ellipsis_ops_imperative():
-    """ Checking various patterns against numpy """
+    """Checking various patterns against numpy"""
     x = numpy.arange(2 * 3 * 4 * 5 * 6).reshape([2, 3, 4, 5, 6])
     for is_symbolic in [True, False]:
         for backend in collect_test_backends(symbolic=is_symbolic, layers=False):
             for pattern in identity_patterns + list(itertools.chain(*equivalent_rearrange_patterns)):
-                check_op_against_numpy(backend, x, pattern, axes_lengths={},
-                                       reduction='rearrange', is_symbolic=is_symbolic)
+                check_op_against_numpy(
+                    backend, x, pattern, axes_lengths={}, reduction="rearrange", is_symbolic=is_symbolic
+                )
 
-            for reduction in ['min', 'max', 'sum']:
+            for reduction in ["min", "max", "sum"]:
                 for pattern in itertools.chain(*equivalent_reduction_patterns):
-                    check_op_against_numpy(backend, x, pattern, axes_lengths={},
-                                           reduction=reduction, is_symbolic=is_symbolic)
+                    check_op_against_numpy(
+                        backend, x, pattern, axes_lengths={}, reduction=reduction, is_symbolic=is_symbolic
+                    )
+
+
+def test_rearrange_array_api():
+    import numpy.array_api as xp
+    from einops import array_api as AA
+
+    x = numpy.arange(2 * 3 * 4 * 5 * 6).reshape([2, 3, 4, 5, 6])
+    for pattern in identity_patterns + list(itertools.chain(*equivalent_rearrange_patterns)):
+        expected = rearrange(x, pattern)
+        result = AA.rearrange(xp.from_dlpack(x), pattern)
+        assert numpy.array_equal(AA.asnumpy(result + 0), expected)
+
+
+def test_reduce_array_api():
+    import numpy.array_api as xp
+    from einops import array_api as AA
+
+    x = numpy.arange(2 * 3 * 4 * 5 * 6).reshape([2, 3, 4, 5, 6])
+    for pattern in itertools.chain(*equivalent_reduction_patterns):
+        for reduction in ["min", "max", "sum"]:
+            expected = reduce(x, pattern, reduction=reduction)
+            result = AA.reduce(xp.from_dlpack(x), pattern, reduction=reduction)
+            assert numpy.array_equal(AA.asnumpy(result + 0), expected)
 
 
 def test_rearrange_consistency_numpy():
     shape = [1, 2, 3, 5, 7, 11]
     x = numpy.arange(numpy.prod(shape)).reshape(shape)
     for pattern in [
-        'a b c d e f -> a b c d e f',
-        'b a c d e f -> a b d e f c',
-        'a b c d e f -> f e d c b a',
-        'a b c d e f -> (f e) d (c b a)',
-        'a b c d e f -> (f e d c b a)',
+        "a b c d e f -> a b c d e f",
+        "b a c d e f -> a b d e f c",
+        "a b c d e f -> f e d c b a",
+        "a b c d e f -> (f e) d (c b a)",
+        "a b c d e f -> (f e d c b a)",
     ]:
         result = rearrange(x, pattern)
         assert len(numpy.setdiff1d(x, result)) == 0
         assert result.dtype == x.dtype
 
-    result = rearrange(x, 'a b c d e f -> a (b) (c d e) f')
+    result = rearrange(x, "a b c d e f -> a (b) (c d e) f")
     assert numpy.array_equal(x.flatten(), result.flatten())
 
-    result = rearrange(x, 'a aa aa1 a1a1 aaaa a11 -> a aa aa1 a1a1 aaaa a11')
+    result = rearrange(x, "a aa aa1 a1a1 aaaa a11 -> a aa aa1 a1a1 aaaa a11")
     assert numpy.array_equal(x, result)
 
-    result1 = rearrange(x, 'a b c d e f -> f e d c b a')
-    result2 = rearrange(x, 'f e d c b a -> a b c d e f')
+    result1 = rearrange(x, "a b c d e f -> f e d c b a")
+    result2 = rearrange(x, "f e d c b a -> a b c d e f")
     assert numpy.array_equal(result1, result2)
 
-    result = rearrange(rearrange(x, 'a b c d e f -> (f d) c (e b) a'), '(f d) c (e b) a -> a b c d e f', b=2, d=5)
+    result = rearrange(rearrange(x, "a b c d e f -> (f d) c (e b) a"), "(f d) c (e b) a -> a b c d e f", b=2, d=5)
     assert numpy.array_equal(x, result)
 
-    sizes = dict(zip('abcdef', shape))
-    temp = rearrange(x, 'a b c d e f -> (f d) c (e b) a', **sizes)
-    result = rearrange(temp, '(f d) c (e b) a -> a b c d e f', **sizes)
+    sizes = dict(zip("abcdef", shape))
+    temp = rearrange(x, "a b c d e f -> (f d) c (e b) a", **sizes)
+    result = rearrange(temp, "(f d) c (e b) a -> a b c d e f", **sizes)
     assert numpy.array_equal(x, result)
 
     x2 = numpy.arange(2 * 3 * 4).reshape([2, 3, 4])
-    result = rearrange(x2, 'a b c -> b c a')
+    result = rearrange(x2, "a b c -> b c a")
     assert x2[1, 2, 3] == result[2, 3, 1]
     assert x2[0, 1, 2] == result[1, 2, 0]
 
 
 def test_rearrange_permutations_numpy():
     # tests random permutation of axes against two independent numpy ways
     for n_axes in range(1, 10):
-        input = numpy.arange(2 ** n_axes).reshape([2] * n_axes)
+        input = numpy.arange(2**n_axes).reshape([2] * n_axes)
         permutation = numpy.random.permutation(n_axes)
-        left_expression = ' '.join('i' + str(axis) for axis in range(n_axes))
-        right_expression = ' '.join('i' + str(axis) for axis in permutation)
-        expression = left_expression + ' -> ' + right_expression
+        left_expression = " ".join("i" + str(axis) for axis in range(n_axes))
+        right_expression = " ".join("i" + str(axis) for axis in permutation)
+        expression = left_expression + " -> " + right_expression
         result = rearrange(input, expression)
 
         for pick in numpy.random.randint(0, 2, [10, n_axes]):
             assert input[tuple(pick)] == result[tuple(pick[permutation])]
 
     for n_axes in range(1, 10):
-        input = numpy.arange(2 ** n_axes).reshape([2] * n_axes)
+        input = numpy.arange(2**n_axes).reshape([2] * n_axes)
         permutation = numpy.random.permutation(n_axes)
-        left_expression = ' '.join('i' + str(axis) for axis in range(n_axes)[::-1])
-        right_expression = ' '.join('i' + str(axis) for axis in permutation[::-1])
-        expression = left_expression + ' -> ' + right_expression
+        left_expression = " ".join("i" + str(axis) for axis in range(n_axes)[::-1])
+        right_expression = " ".join("i" + str(axis) for axis in permutation[::-1])
+        expression = left_expression + " -> " + right_expression
         result = rearrange(input, expression)
         assert result.shape == input.shape
         expected_result = numpy.zeros_like(input)
         for original_axis, result_axis in enumerate(permutation):
             expected_result |= ((input >> original_axis) & 1) << result_axis
 
         assert numpy.array_equal(result, expected_result)
 
 
 def test_reduction_imperatives():
     for backend in imp_op_backends:
-        print('Reduction tests for ', backend.framework_name)
+        print("Reduction tests for ", backend.framework_name)
         for reduction in _reductions:
             # slight redundancy for simpler order - numpy version is evaluated multiple times
-            input = numpy.arange(2 * 3 * 4 * 5 * 6, dtype='int64').reshape([2, 3, 4, 5, 6])
-            if reduction in ['mean', 'prod']:
-                input = input / input.astype('float64').mean()
+            input = numpy.arange(2 * 3 * 4 * 5 * 6, dtype="int64").reshape([2, 3, 4, 5, 6])
+            if reduction in ["mean", "prod"]:
+                input = input / input.astype("float64").mean()
             test_cases = [
-                ['a b c d e -> ', {},
-                 getattr(input, reduction)()],
-                ['a ... -> ', {},
-                 getattr(input, reduction)()],
-                ['(a1 a2) ... (e1 e2) -> ', dict(a1=1, e2=2),
-                 getattr(input, reduction)()],
-                ['a b c d e -> (e c) a', {},
-                 getattr(input, reduction)(axis=(1, 3)).transpose(2, 1, 0).reshape([-1, 2])],
-                ['a ... c d e -> (e c) a', {},
-                 getattr(input, reduction)(axis=(1, 3)).transpose(2, 1, 0).reshape([-1, 2])],
-                ['a b c d e ... -> (e c) a', {},
-                 getattr(input, reduction)(axis=(1, 3)).transpose(2, 1, 0).reshape([-1, 2])],
-                ['a b c d e -> (e c a)', {},
-                 getattr(input, reduction)(axis=(1, 3)).transpose(2, 1, 0).reshape([-1])],
-                ['(a a2) ... -> (a2 a) ...', dict(a2=1),
-                 input],
+                ["a b c d e -> ", {}, getattr(input, reduction)()],
+                ["a ... -> ", {}, getattr(input, reduction)()],
+                ["(a1 a2) ... (e1 e2) -> ", dict(a1=1, e2=2), getattr(input, reduction)()],
+                [
+                    "a b c d e -> (e c) a",
+                    {},
+                    getattr(input, reduction)(axis=(1, 3)).transpose(2, 1, 0).reshape([-1, 2]),
+                ],
+                [
+                    "a ... c d e -> (e c) a",
+                    {},
+                    getattr(input, reduction)(axis=(1, 3)).transpose(2, 1, 0).reshape([-1, 2]),
+                ],
+                [
+                    "a b c d e ... -> (e c) a",
+                    {},
+                    getattr(input, reduction)(axis=(1, 3)).transpose(2, 1, 0).reshape([-1, 2]),
+                ],
+                ["a b c d e -> (e c a)", {}, getattr(input, reduction)(axis=(1, 3)).transpose(2, 1, 0).reshape([-1])],
+                ["(a a2) ... -> (a2 a) ...", dict(a2=1), input],
             ]
             for pattern, axes_lengths, expected_result in test_cases:
                 result = reduce(backend.from_numpy(input.copy()), pattern, reduction=reduction, **axes_lengths)
                 result = backend.to_numpy(result)
-                assert numpy.allclose(result, expected_result), f'Failed at {pattern}'
+                assert numpy.allclose(result, expected_result), f"Failed at {pattern}"
 
 
 def test_reduction_symbolic():
     for backend in sym_op_backends:
-        print('Reduction tests for ', backend.framework_name)
+        print("Reduction tests for ", backend.framework_name)
         for reduction in _reductions:
-            input = numpy.arange(2 * 3 * 4 * 5 * 6, dtype='int64').reshape([2, 3, 4, 5, 6])
-            input = input / input.astype('float64').mean()
+            input = numpy.arange(2 * 3 * 4 * 5 * 6, dtype="int64").reshape([2, 3, 4, 5, 6])
+            input = input / input.astype("float64").mean()
             # slight redundancy for simpler order - numpy version is evaluated multiple times
             test_cases = [
-                ['a b c d e -> ', {},
-                 getattr(input, reduction)()],
-                ['a ... -> ', {},
-                 getattr(input, reduction)()],
-                ['(a a2) ... (e e2) -> ', dict(a2=1, e2=1),
-                 getattr(input, reduction)()],
-                ['a b c d e -> (e c) a', {},
-                 getattr(input, reduction)(axis=(1, 3)).transpose(2, 1, 0).reshape([-1, 2])],
-                ['a ... c d e -> (e c) a', {},
-                 getattr(input, reduction)(axis=(1, 3)).transpose(2, 1, 0).reshape([-1, 2])],
-                ['a b c d e ... -> (e c) a', {},
-                 getattr(input, reduction)(axis=(1, 3)).transpose(2, 1, 0).reshape([-1, 2])],
-                ['a b c d e -> (e c a)', {},
-                 getattr(input, reduction)(axis=(1, 3)).transpose(2, 1, 0).reshape([-1])],
-                ['(a a2) ... -> (a2 a) ...', dict(a2=1),
-                 input],
+                ["a b c d e -> ", {}, getattr(input, reduction)()],
+                ["a ... -> ", {}, getattr(input, reduction)()],
+                ["(a a2) ... (e e2) -> ", dict(a2=1, e2=1), getattr(input, reduction)()],
+                [
+                    "a b c d e -> (e c) a",
+                    {},
+                    getattr(input, reduction)(axis=(1, 3)).transpose(2, 1, 0).reshape([-1, 2]),
+                ],
+                [
+                    "a ... c d e -> (e c) a",
+                    {},
+                    getattr(input, reduction)(axis=(1, 3)).transpose(2, 1, 0).reshape([-1, 2]),
+                ],
+                [
+                    "a b c d e ... -> (e c) a",
+                    {},
+                    getattr(input, reduction)(axis=(1, 3)).transpose(2, 1, 0).reshape([-1, 2]),
+                ],
+                ["a b c d e -> (e c a)", {}, getattr(input, reduction)(axis=(1, 3)).transpose(2, 1, 0).reshape([-1])],
+                ["(a a2) ... -> (a2 a) ...", dict(a2=1), input],
             ]
             for pattern, axes_lengths, expected_numpy_result in test_cases:
                 shapes = [input.shape, [None for _ in input.shape]]
                 for shape in shapes:
                     sym = backend.create_symbol(shape)
                     result_sym = reduce(sym, pattern, reduction=reduction, **axes_lengths)
                     result = backend.eval_symbol(result_sym, [(sym, input)])
                     assert numpy.allclose(result, expected_numpy_result)
 
                 if True:
                     shape = []
                     _axes_lengths = {**axes_lengths}
-                    for axis, length in zip('abcde', input.shape):
+                    for axis, length in zip("abcde", input.shape):
                         # filling as much as possible with Nones
                         if axis in pattern:
                             shape.append(None)
                             _axes_lengths[axis] = length
                         else:
                             shape.append(length)
                     sym = backend.create_symbol(shape)
                     result_sym = reduce(sym, pattern, reduction=reduction, **_axes_lengths)
                     result = backend.eval_symbol(result_sym, [(sym, input)])
                     assert numpy.allclose(result, expected_numpy_result)
 
 
 def test_reduction_stress_imperatives():
     for backend in imp_op_backends:
-        print('Stress-testing reduction for ', backend.framework_name)
-        for reduction in _reductions + ('rearrange',):
-            dtype = 'int64'
+        print("Stress-testing reduction for ", backend.framework_name)
+        for reduction in _reductions + ("rearrange",):
+            dtype = "int64"
             coincide = numpy.array_equal
-            if reduction in ['mean', 'prod']:
-                dtype = 'float64'
+            if reduction in ["mean", "prod"]:
+                dtype = "float64"
                 coincide = numpy.allclose
             max_dim = 11
-            if 'oneflow' in backend.framework_name:
+            if "oneflow" in backend.framework_name:
                 max_dim = 7
-            if 'paddle' in backend.framework_name:
+            if "paddle" in backend.framework_name:
                 max_dim = 9
             for n_axes in range(max_dim):
                 shape = numpy.random.randint(2, 4, size=n_axes)
                 permutation = numpy.random.permutation(n_axes)
-                skipped = 0 if reduction == 'rearrange' else numpy.random.randint(n_axes + 1)
-                left = ' '.join('x' + str(i) for i in range(n_axes))
-                right = ' '.join('x' + str(i) for i in permutation[skipped:])
-                pattern = left + '->' + right
+                skipped = 0 if reduction == "rearrange" else numpy.random.randint(n_axes + 1)
+                left = " ".join("x" + str(i) for i in range(n_axes))
+                right = " ".join("x" + str(i) for i in permutation[skipped:])
+                pattern = left + "->" + right
                 x = numpy.arange(1, 1 + numpy.prod(shape), dtype=dtype).reshape(shape)
-                if reduction == 'prod':
+                if reduction == "prod":
                     x /= x.mean()  # to avoid overflows
                 result1 = reduce(x, pattern, reduction=reduction)
                 result2 = x.transpose(permutation)
                 if skipped > 0:
                     result2 = getattr(result2, reduction)(axis=tuple(range(skipped)))
                 assert coincide(result1, result2)
                 check_op_against_numpy(backend, x, pattern, reduction=reduction, axes_lengths={}, is_symbolic=False)
 
 
 def test_reduction_with_callable_imperatives():
-    x_numpy = numpy.arange(2 * 3 * 4 * 5 * 6).reshape([2, 3, 4, 5, 6]).astype('float32')
+    x_numpy = numpy.arange(2 * 3 * 4 * 5 * 6).reshape([2, 3, 4, 5, 6]).astype("float32")
     x_numpy /= x_numpy.max()
 
     def logsumexp_torch(x, tuple_of_axes):
         return x.logsumexp(tuple_of_axes)
 
     def logsumexp_tf(x, tuple_of_axes):
         import tensorflow as tf
+
         return tf.reduce_logsumexp(x, tuple_of_axes)
 
     def logsumexp_chainer(x, tuple_of_axes):
         import chainer
+
         return chainer.functions.logsumexp(x, tuple_of_axes)
 
     def logsumexp_keras(x, tuple_of_axes):
         import tensorflow.keras.backend as k
+
         return k.logsumexp(x, tuple_of_axes)
 
     def logsumexp_numpy(x, tuple_of_axes):
         # very naive logsumexp to compare to
         minused = x.max(tuple_of_axes)
         y = x - x.max(tuple_of_axes, keepdims=True)
         y = numpy.exp(y)
         y = numpy.sum(y, axis=tuple_of_axes)
         return numpy.log(y) + minused
 
     from einops._backends import TorchBackend, ChainerBackend, TensorflowBackend, KerasBackend, NumpyBackend
+
     backend2callback = {
         TorchBackend.framework_name: logsumexp_torch,
         ChainerBackend.framework_name: logsumexp_chainer,
         TensorflowBackend.framework_name: logsumexp_tf,
         KerasBackend.framework_name: logsumexp_keras,
         NumpyBackend.framework_name: logsumexp_numpy,
     }
@@ -329,85 +365,85 @@
         if backend.framework_name not in backend2callback:
             continue
 
         backend_callback = backend2callback[backend.framework_name]
 
         x_backend = backend.from_numpy(x_numpy)
         for pattern1, pattern2 in equivalent_reduction_patterns:
-            print('Test reduction with callable for ', backend.framework_name, pattern1, pattern2)
+            print("Test reduction with callable for ", backend.framework_name, pattern1, pattern2)
             output_numpy = reduce(x_numpy, pattern1, reduction=logsumexp_numpy)
             output_backend = reduce(x_backend, pattern1, reduction=backend_callback)
             assert numpy.allclose(
                 output_numpy,
                 backend.to_numpy(output_backend),
             )
 
 
 def test_enumerating_directions():
     for backend in imp_op_backends:
-        print('testing directions for', backend.framework_name)
+        print("testing directions for", backend.framework_name)
         for shape in [[], [1], [1, 1, 1], [2, 3, 5, 7]]:
             x = numpy.arange(numpy.prod(shape)).reshape(shape)
             axes1 = _enumerate_directions(x)
             axes2 = _enumerate_directions(backend.from_numpy(x))
             assert len(axes1) == len(axes2) == len(shape)
             for ax1, ax2 in zip(axes1, axes2):
                 ax2 = backend.to_numpy(ax2)
                 assert ax1.shape == ax2.shape
                 assert numpy.allclose(ax1, ax2)
 
 
 def test_concatenations_and_stacking():
     for backend in imp_op_backends:
-        print('testing shapes for ', backend.framework_name)
+        print("testing shapes for ", backend.framework_name)
         for n_arrays in [1, 2, 5]:
             shapes = [[], [1], [1, 1], [2, 3, 5, 7], [1] * 6]
             for shape in shapes:
                 arrays1 = [numpy.arange(i, i + numpy.prod(shape)).reshape(shape) for i in range(n_arrays)]
                 arrays2 = [backend.from_numpy(array) for array in arrays1]
                 result0 = numpy.asarray(arrays1)
-                result1 = rearrange(arrays1, '...->...')
-                result2 = rearrange(arrays2, '...->...')
+                result1 = rearrange(arrays1, "...->...")
+                result2 = rearrange(arrays2, "...->...")
                 assert numpy.array_equal(result0, result1)
                 assert numpy.array_equal(result1, backend.to_numpy(result2))
 
-                result1 = rearrange(arrays1, 'b ... -> ... b')
-                result2 = rearrange(arrays2, 'b ... -> ... b')
+                result1 = rearrange(arrays1, "b ... -> ... b")
+                result2 = rearrange(arrays2, "b ... -> ... b")
                 assert numpy.array_equal(result1, backend.to_numpy(result2))
 
 
 def test_gradients_imperatives():
     # lazy - just checking reductions
     for reduction in _reductions:
-        x = numpy.arange(1, 1 + 2 * 3 * 4).reshape([2, 3, 4]).astype('float32')
+        x = numpy.arange(1, 1 + 2 * 3 * 4).reshape([2, 3, 4]).astype("float32")
         results = {}
         for backend in imp_op_backends:
             y0 = backend.from_numpy(x)
-            if not hasattr(y0, 'grad'):
+            if not hasattr(y0, "grad"):
                 continue
 
-            y1 = reduce(y0, 'a b c -> c a', reduction=reduction)
-            y2 = reduce(y1, 'c a -> a c', reduction=reduction)
-            y3 = reduce(y2, 'a (c1 c2) -> a', reduction=reduction, c1=2)
-            y4 = reduce(y3, '... -> ', reduction=reduction)
+            y1 = reduce(y0, "a b c -> c a", reduction=reduction)
+            y2 = reduce(y1, "c a -> a c", reduction=reduction)
+            y3 = reduce(y2, "a (c1 c2) -> a", reduction=reduction, c1=2)
+            y4 = reduce(y3, "... -> ", reduction=reduction)
 
             y4.backward()
             grad = backend.to_numpy(y0.grad)
             results[backend.framework_name] = grad
 
-        print('comparing gradients for', results.keys())
+        print("comparing gradients for", results.keys())
         for name1, grad1 in results.items():
             for name2, grad2 in results.items():
-                assert numpy.allclose(grad1, grad2), [name1, name2, 'provided different gradients']
+                assert numpy.allclose(grad1, grad2), [name1, name2, "provided different gradients"]
 
 
 def test_tiling_imperatives():
     for backend in imp_op_backends:
-        print('Tiling tests for ', backend.framework_name)
-        input = numpy.arange(2 * 3 * 5, dtype='int64').reshape([2, 1, 3, 1, 5])
+        print("Tiling tests for ", backend.framework_name)
+        input = numpy.arange(2 * 3 * 5, dtype="int64").reshape([2, 1, 3, 1, 5])
         test_cases = [
             (1, 1, 1, 1, 1),
             (1, 2, 1, 3, 1),
             (3, 1, 1, 4, 1),
         ]
         for repeats in test_cases:
             expected = numpy.tile(input, repeats)
@@ -415,16 +451,16 @@
             repeated = backend.tile(converted, repeats)
             result = backend.to_numpy(repeated)
             assert numpy.array_equal(result, expected)
 
 
 def test_tiling_symbolic():
     for backend in sym_op_backends:
-        print('Tiling tests for ', backend.framework_name)
-        input = numpy.arange(2 * 3 * 5, dtype='int64').reshape([2, 1, 3, 1, 5])
+        print("Tiling tests for ", backend.framework_name)
+        input = numpy.arange(2 * 3 * 5, dtype="int64").reshape([2, 1, 3, 1, 5])
         test_cases = [
             (1, 1, 1, 1, 1),
             (1, 2, 1, 3, 1),
             (3, 1, 1, 4, 1),
         ]
         for repeats in test_cases:
             expected = numpy.tile(input, repeats)
@@ -435,82 +471,111 @@
             sym = backend.create_symbol([None] * len(input.shape))
             result = backend.eval_symbol(backend.tile(sym, repeats), [[sym, input]])
             assert numpy.array_equal(result, expected)
 
 
 repeat_test_cases = [
     # all assume that input has shape [2, 3, 5]
-    ('a b c -> c a b', dict()),
-    ('a b c -> (c copy a b)', dict(copy=2, a=2, b=3, c=5)),
-    ('a b c -> (a copy) b c ', dict(copy=1)),
-    ('a b c -> (c a) (copy1 b copy2)', dict(a=2, copy1=1, copy2=2)),
-    ('a ...  -> a ... copy', dict(copy=4)),
-    ('... c -> ... (copy1 c copy2)', dict(copy1=1, copy2=2)),
-    ('...  -> ... ', dict()),
-    (' ...  -> copy1 ... copy2 ', dict(copy1=2, copy2=3)),
-    ('a b c  -> copy1 a copy2 b c () ', dict(copy1=2, copy2=1)),
+    ("a b c -> c a b", dict()),
+    ("a b c -> (c copy a b)", dict(copy=2, a=2, b=3, c=5)),
+    ("a b c -> (a copy) b c ", dict(copy=1)),
+    ("a b c -> (c a) (copy1 b copy2)", dict(a=2, copy1=1, copy2=2)),
+    ("a ...  -> a ... copy", dict(copy=4)),
+    ("... c -> ... (copy1 c copy2)", dict(copy1=1, copy2=2)),
+    ("...  -> ... ", dict()),
+    (" ...  -> copy1 ... copy2 ", dict(copy1=2, copy2=3)),
+    ("a b c  -> copy1 a copy2 b c () ", dict(copy1=2, copy2=1)),
 ]
 
 
 def check_reversion(x, repeat_pattern, **sizes):
-    """Checks repeat pattern by running reduction """
-    left, right = repeat_pattern.split('->')
-    reduce_pattern = right + '->' + left
-    repeated = reduce(x, repeat_pattern, reduction='repeat', **sizes)
-    reduced_min = reduce(repeated, reduce_pattern, reduction='min', **sizes)
-    reduced_max = reduce(repeated, reduce_pattern, reduction='max', **sizes)
+    """Checks repeat pattern by running reduction"""
+    left, right = repeat_pattern.split("->")
+    reduce_pattern = right + "->" + left
+    repeated = repeat(x, repeat_pattern, **sizes)
+    reduced_min = reduce(repeated, reduce_pattern, reduction="min", **sizes)
+    reduced_max = reduce(repeated, reduce_pattern, reduction="max", **sizes)
     assert numpy.array_equal(x, reduced_min)
     assert numpy.array_equal(x, reduced_max)
 
 
 def test_repeat_numpy():
     # check repeat vs reduce. Repeat works ok if reverse reduction with min and max work well
     x = numpy.arange(2 * 3 * 5).reshape([2, 3, 5])
-    x1 = reduce(x, 'a b c -> copy a b c ', reduction='repeat', copy=1)
+    x1 = repeat(x, "a b c -> copy a b c ", copy=1)
     assert numpy.array_equal(x[None], x1)
     for pattern, axis_dimensions in repeat_test_cases:
         check_reversion(x, pattern, **axis_dimensions)
 
 
 def test_repeat_imperatives():
     x = numpy.arange(2 * 3 * 5).reshape([2, 3, 5])
     for backend in imp_op_backends:
-        print('Repeat tests for ', backend.framework_name)
+        print("Repeat tests for ", backend.framework_name)
 
         for pattern, axis_dimensions in repeat_test_cases:
-            expected = reduce(x, pattern, reduction='repeat', **axis_dimensions)
+            expected = repeat(x, pattern, **axis_dimensions)
             converted = backend.from_numpy(x)
-            repeated = reduce(converted, pattern, reduction='repeat', **axis_dimensions)
+            repeated = repeat(converted, pattern, **axis_dimensions)
             result = backend.to_numpy(repeated)
             assert numpy.array_equal(result, expected)
 
 
 def test_repeat_symbolic():
     x = numpy.arange(2 * 3 * 5).reshape([2, 3, 5])
 
     for backend in sym_op_backends:
-        print('Repeat tests for ', backend.framework_name)
+        print("Repeat tests for ", backend.framework_name)
 
         for pattern, axis_dimensions in repeat_test_cases:
-            expected = reduce(x, pattern, reduction='repeat', **axis_dimensions)
+            expected = repeat(x, pattern, **axis_dimensions)
 
             sym = backend.create_symbol(x.shape)
-            result = backend.eval_symbol(reduce(sym, pattern, reduction='repeat', **axis_dimensions), [[sym, x]])
+            result = backend.eval_symbol(repeat(sym, pattern, **axis_dimensions), [[sym, x]])
             assert numpy.array_equal(result, expected)
 
 
+def test_repeat_array_api():
+    import numpy.array_api as xp
+    from einops import array_api as AA
+
+    x = numpy.arange(2 * 3 * 5).reshape([2, 3, 5])
+
+    for pattern, axis_dimensions in repeat_test_cases:
+        expected = repeat(x, pattern, **axis_dimensions)
+
+        result = AA.repeat(xp.from_dlpack(x), pattern, **axis_dimensions)
+        assert numpy.array_equal(AA.asnumpy(result + 0), expected)
+
+
 test_cases_repeat_anonymous = [
     # all assume that input has shape [1, 2, 4, 6]
-    ('a b c d -> c a d b', dict()),
-    ('a b c d -> (c 2 d a b)', dict(a=1, c=4, d=6)),
-    ('1 b c d -> (d copy 1) 3 b c ', dict(copy=3)),
-    ('1 ...  -> 3 ... ', dict()),
-    ('() ... d -> 1 (copy1 d copy2) ... ', dict(copy1=2, copy2=3)),
-    ('1 b c d -> (1 1) (1 b) 2 c 3 d (1 1)', dict()),
-
+    ("a b c d -> c a d b", dict()),
+    ("a b c d -> (c 2 d a b)", dict(a=1, c=4, d=6)),
+    ("1 b c d -> (d copy 1) 3 b c ", dict(copy=3)),
+    ("1 ...  -> 3 ... ", dict()),
+    ("() ... d -> 1 (copy1 d copy2) ... ", dict(copy1=2, copy2=3)),
+    ("1 b c d -> (1 1) (1 b) 2 c 3 d (1 1)", dict()),
 ]
 
 
 def test_anonymous_axes():
     x = numpy.arange(1 * 2 * 4 * 6).reshape([1, 2, 4, 6])
     for pattern, axis_dimensions in test_cases_repeat_anonymous:
         check_reversion(x, pattern, **axis_dimensions)
+
+
+def test_list_inputs():
+    x = numpy.arange(2 * 3 * 4 * 5 * 6).reshape([2, 3, 4, 5, 6])
+
+    assert numpy.array_equal(
+        rearrange(list(x), "... -> (...)"),
+        rearrange(x, "... -> (...)"),
+    )
+    assert numpy.array_equal(
+        reduce(list(x), "a ... e -> (...)", "min"),
+        reduce(x, "a ... e -> (...)", "min"),
+    )
+    assert numpy.array_equal(
+        repeat(list(x), "...  -> b (...)", b=3),
+        repeat(x, "...  -> b (...)", b=3),
+    )
```

### Comparing `einops-0.6.2rc0/tests/test_other.py` & `einops-0.7.0rc1/tests/test_other.py`

 * *Files identical despite different names*

### Comparing `einops-0.6.2rc0/tests/test_packing.py` & `einops-0.7.0rc1/tests/test_packing.py`

 * *Files 5% similar despite different names*

```diff
@@ -263,7 +263,47 @@
                 unpack_and_pack(x, [[2], [3], [-1]], pattern)
                 unpack_and_pack(x, [[0], [5], [-1]], pattern)
                 unpack_and_pack(x, [[0], [-1], [5]], pattern)
                 unpack_and_pack(x, [[-1], [5], [0]], pattern)
 
                 # -1 takes zero, -1
                 unpack_and_pack(x, [[2, -1], [1, 5]], pattern)
+
+
+
+def test_pack_unpack_array_api():
+    from einops import array_api as AA
+    import numpy.array_api as xp
+
+    for case in cases:
+        shape = case.shape
+        pattern = case.pattern
+        x_np = np.random.random(shape)
+        x_xp = xp.from_dlpack(x_np)
+
+        for ps in [
+            [[2], [1], [2]],
+            [[1], [1], [-1]],
+            [[1], [1], [-1, 3]],
+            [[2, 1], [1, 1, 1], [-1]],
+        ]:
+
+            x_np_split = unpack(x_np, ps, pattern)
+            x_xp_split = AA.unpack(x_xp, ps, pattern)
+            for a, b in zip(x_np_split, x_xp_split):
+                assert np.allclose(a, AA.asnumpy(b + 0))
+
+            x_agg_np, ps1 = pack(x_np_split, pattern)
+            x_agg_xp, ps2 = AA.pack(x_xp_split, pattern)
+            assert ps1 == ps2
+            assert np.allclose(x_agg_np, AA.asnumpy(x_agg_xp))
+
+        for ps in [
+            [[2, 3]],
+            [[1], [5]],
+            [[1], [5], [-1]],
+            [[1], [2, 3]],
+            [[1], [5], [-1, 2]],
+        ]:
+            with pytest.raises(BaseException):
+                unpack(x_np, ps, pattern)
+
```

### Comparing `einops-0.6.2rc0/tests/test_parsing.py` & `einops-0.7.0rc1/tests/test_parsing.py`

 * *Files identical despite different names*

### Comparing `einops-0.6.2rc0/.gitignore` & `einops-0.7.0rc1/.gitignore`

 * *Files identical despite different names*

### Comparing `einops-0.6.2rc0/LICENSE` & `einops-0.7.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `einops-0.6.2rc0/README.md` & `einops-0.7.0rc1/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -25,30 +25,29 @@
 
 
 Flexible and powerful tensor operations for readable and reliable code. <br />
 Supports numpy, pytorch, tensorflow, jax, and [others](#supported-frameworks).
 
 ## Recent updates:
 
+- 0.7.0rc1: no-hassle `torch.compile`, support of [array api standard](https://data-apis.org/array-api/latest/API_specification/index.html) and more
 - 10'000: github reports that more than 10k project use einops 🎂
 - see how to use einops with [torch.compile](https://github.com/arogozhnikov/einops/wiki/Using-torch.compile-with-einops)
 - einops 0.6.1: paddle backend added
 - einops 0.6 introduces [packing and unpacking](https://github.com/arogozhnikov/einops/blob/master/docs/4-pack-and-unpack.ipynb)
 - einops 0.5: einsum is now a part of einops
 - [Einops paper](https://openreview.net/pdf?id=oapKSVM2bcj) is accepted for oral presentation at ICLR 2022 (yes, it worth reading).
   Talk recordings are [available](https://iclr.cc/virtual/2022/oral/6603)
 
 
-<details>
-  <summary>Previous updates</summary>
-  
-  
-  - flax and oneflow backend added
-  - torch.jit.script is supported for pytorch layers
-  - powerful EinMix added to einops. [Einmix tutorial notebook](https://github.com/arogozhnikov/einops/blob/master/docs/3-einmix-layer.ipynb) 
+<details markdown="1">
+<summary>Previous updates</summary>
+- flax and oneflow backend added
+- torch.jit.script is supported for pytorch layers
+- powerful EinMix added to einops. [Einmix tutorial notebook](https://github.com/arogozhnikov/einops/blob/master/docs/3-einmix-layer.ipynb) 
 </details>
 
 <!--<div align="center">
   <img src="http://arogozhnikov.github.io/images/einops/einops_logo_350x350.png" 
   alt="einops package logo" width="250" height="250" />
   <br><br>
 </div> -->
@@ -158,43 +157,42 @@
 
 Einops provides layers (`einops` keeps a separate version for each framework) that reflect corresponding functions
 
 ```python
 from einops.layers.torch      import Rearrange, Reduce
 from einops.layers.tensorflow import Rearrange, Reduce
 from einops.layers.flax       import Rearrange, Reduce
-from einops.layers.gluon      import Rearrange, Reduce
+from einops.layers.paddle     import Rearrange, Reduce
 from einops.layers.keras      import Rearrange, Reduce
 from einops.layers.chainer    import Rearrange, Reduce
 ```
 
-<details>
-  <summary>Example of using layers within a pytorch model</summary>
-  
-  
-  ```python
-  # example given for pytorch, but code in other frameworks is almost identical  
-  from torch.nn import Sequential, Conv2d, MaxPool2d, Linear, ReLU
-  from einops.layers.torch import Rearrange
-
-  model = Sequential(
-      ...,
-      Conv2d(6, 16, kernel_size=5),
-      MaxPool2d(kernel_size=2),
-      # flattening without need to write forward
-      Rearrange('b c h w -> b (c h w)'),  
-      Linear(16*5*5, 120), 
-      ReLU(),
-      Linear(120, 10), 
-  )
-  ```
-  
-  No more flatten needed! 
-  
-  Additionally, torch users will benefit from layers as those are script-able and compile-able.
+<details markdown="1">
+<summary>Example of using layers within a pytorch model</summary>
+Example given for pytorch, but code in other frameworks is almost identical
+
+```python 
+from torch.nn import Sequential, Conv2d, MaxPool2d, Linear, ReLU
+from einops.layers.torch import Rearrange
+
+model = Sequential(
+    ...,
+    Conv2d(6, 16, kernel_size=5),
+    MaxPool2d(kernel_size=2),
+    # flattening without need to write forward
+    Rearrange('b c h w -> b (c h w)'),  
+    Linear(16*5*5, 120), 
+    ReLU(),
+    Linear(120, 10), 
+)
+```
+
+No more flatten needed! 
+
+Additionally, torch users will benefit from layers as those are script-able and compile-able.
 </details>
 
 
 
 
 ## Naming <a name="Naming"></a>
 
@@ -280,15 +278,15 @@
 
 ```python
 y = x.flatten() # or flatten(x)
 ```
 
 Suppose `x`'s shape was `(3, 4, 5)`, then `y` has shape ...
 
-- numpy, cupy, chainer, pytorch: `(60,)`
+- numpy, pytorch, cupy, chainer: `(60,)`
 - keras, tensorflow.layers, gluon: `(3, 20)`
 
 `einops` works the same way in all frameworks.
 
 ### Independence of framework terminology
 
 Example: `tile` vs `repeat` causes lots of confusion. To copy image along width:
@@ -319,15 +317,16 @@
 - [jax](https://github.com/google/jax)
 - [cupy](https://cupy.chainer.org/)
 - [chainer](https://chainer.org/)
 - [tf.keras](https://www.tensorflow.org/guide/keras)
 - [oneflow](https://github.com/Oneflow-Inc/oneflow) (experimental)
 - [flax](https://github.com/google/flax) (experimental)
 - [paddle](https://github.com/PaddlePaddle/Paddle) (experimental)
-- [gluon](https://gluon.mxnet.io/) (deprecated)
+
+Additionally, starting from einops 0.7.0 einops can be used with any framework that supports [Python array API standard](https://data-apis.org/array-api/latest/API_specification/index.html)
 
 ## Citing einops <a name="Citing"></a>
 
 Please use the following bibtex record
 
 ```text
 @inproceedings{
@@ -339,8 +338,8 @@
     url={https://openreview.net/forum?id=oapKSVM2bcj}
 }
 ```
 
 
 ## Supported python versions
 
-`einops` works with python 3.7 or later.
+`einops` works with python 3.8 or later.
```

#### html2text {}

```diff
@@ -5,23 +5,25 @@
 version](https://badge.fury.io/py/einops.svg)](https://badge.fury.io/py/einops)
 [![Documentation](https://img.shields.io/badge/documentation-link-blue.svg)]
 (https://einops.rocks/) ![Supported python versions](https://
 raw.githubusercontent.com/arogozhnikov/einops/master/docs/resources/
 python_badge.svg) Flexible and powerful tensor operations for readable and
 reliable code.
 Supports numpy, pytorch, tensorflow, jax, and [others](#supported-frameworks).
-## Recent updates: - 10'000: github reports that more than 10k project use
-einops ð - see how to use einops with [torch.compile](https://github.com/
-arogozhnikov/einops/wiki/Using-torch.compile-with-einops) - einops 0.6.1:
-paddle backend added - einops 0.6 introduces [packing and unpacking](https://
-github.com/arogozhnikov/einops/blob/master/docs/4-pack-and-unpack.ipynb) -
-einops 0.5: einsum is now a part of einops - [Einops paper](https://
-openreview.net/pdf?id=oapKSVM2bcj) is accepted for oral presentation at ICLR
-2022 (yes, it worth reading). Talk recordings are [available](https://iclr.cc/
-virtual/2022/oral/6603)  Previous updates - flax and oneflow backend added -
+## Recent updates: - 0.7.0rc1: no-hassle `torch.compile`, support of [array api
+standard](https://data-apis.org/array-api/latest/API_specification/index.html)
+and more - 10'000: github reports that more than 10k project use einops ð -
+see how to use einops with [torch.compile](https://github.com/arogozhnikov/
+einops/wiki/Using-torch.compile-with-einops) - einops 0.6.1: paddle backend
+added - einops 0.6 introduces [packing and unpacking](https://github.com/
+arogozhnikov/einops/blob/master/docs/4-pack-and-unpack.ipynb) - einops 0.5:
+einsum is now a part of einops - [Einops paper](https://openreview.net/
+pdf?id=oapKSVM2bcj) is accepted for oral presentation at ICLR 2022 (yes, it
+worth reading). Talk recordings are [available](https://iclr.cc/virtual/2022/
+oral/6603)  Previous updates - flax and oneflow backend added -
 torch.jit.script is supported for pytorch layers - powerful EinMix added to
 einops. [Einmix tutorial notebook](https://github.com/arogozhnikov/einops/blob/
 master/docs/3-einmix-layer.ipynb)   ## Tweets > In case you need convincing
 arguments for setting aside time to learn about einsum and einops... [Tim
 RocktÃ¤schel, FAIR](https://twitter.com/_rockt/status/1230818967205425152) >
 Writing better code with PyTorch and einops ð [Andrej Karpathy, AI at Tesla]
 (https://twitter.com/karpathy/status/1290826075916779520) > Slowly but surely,
@@ -63,19 +65,19 @@
 dot-product # but 1) axes can be multi-lettered 2) pattern goes last 3) works
 with multiple frameworks C = einsum(A, B, 'b t1 head c, b t2 head c -> b head
 t1 t2') ``` ### EinMix `EinMix` is a generic linear layer, perfect for MLP
 Mixers and similar architectures. ### Layers Einops provides layers (`einops`
 keeps a separate version for each framework) that reflect corresponding
 functions ```python from einops.layers.torch import Rearrange, Reduce from
 einops.layers.tensorflow import Rearrange, Reduce from einops.layers.flax
-import Rearrange, Reduce from einops.layers.gluon import Rearrange, Reduce from
-einops.layers.keras import Rearrange, Reduce from einops.layers.chainer import
-Rearrange, Reduce ```  Example of using layers within a pytorch model ```python
-# example given for pytorch, but code in other frameworks is almost identical
-from torch.nn import Sequential, Conv2d, MaxPool2d, Linear, ReLU from
+import Rearrange, Reduce from einops.layers.paddle import Rearrange, Reduce
+from einops.layers.keras import Rearrange, Reduce from einops.layers.chainer
+import Rearrange, Reduce ```  Example of using layers within a pytorch model
+Example given for pytorch, but code in other frameworks is almost identical
+```python from torch.nn import Sequential, Conv2d, MaxPool2d, Linear, ReLU from
 einops.layers.torch import Rearrange model = Sequential( ..., Conv2d(6, 16,
 kernel_size=5), MaxPool2d(kernel_size=2), # flattening without need to write
 forward Rearrange('b c h w -> b (c h w)'), Linear(16*5*5, 120), ReLU(), Linear
 (120, 10), ) ``` No more flatten needed! Additionally, torch users will benefit
 from layers as those are script-able and compile-able.  ## Naming  `einops`
 stands for Einstein-Inspired Notation for operations (though "Einstein
 operations" is more attractive and easier to remember). Notation was loosely
@@ -108,16 +110,16 @@
 c (x dx) (y dy) (z dz) -> b c x y z', 'max', dx=2, dy=3, dz=4) ``` These
 examples demonstrated that we don't use separate operations for 1d/2d/3d
 pooling, those are all defined in a uniform way. Space-to-depth and depth-to
 space are defined in many frameworks but how about width-to-height? Here you
 go: ```python rearrange(x, 'b c h (w w2) -> b c (h w2) w', w2=2) ``` ###
 Framework independent behavior Even simple functions are defined differently by
 different frameworks ```python y = x.flatten() # or flatten(x) ``` Suppose
-`x`'s shape was `(3, 4, 5)`, then `y` has shape ... - numpy, cupy, chainer,
-pytorch: `(60,)` - keras, tensorflow.layers, gluon: `(3, 20)` `einops` works
+`x`'s shape was `(3, 4, 5)`, then `y` has shape ... - numpy, pytorch, cupy,
+chainer: `(60,)` - keras, tensorflow.layers, gluon: `(3, 20)` `einops` works
 the same way in all frameworks. ### Independence of framework terminology
 Example: `tile` vs `repeat` causes lots of confusion. To copy image along
 width: ```python np.tile(image, (1, 2)) # in numpy image.repeat(1, 2) #
 pytorch's repeat ~ numpy's tile ``` With einops you don't need to decipher
 which axis was repeated: ```python repeat(image, 'h w -> h (tile w)', tile=2) #
 in numpy repeat(image, 'h w -> h (tile w)', tile=2) # in pytorch repeat(image,
 'h w -> h (tile w)', tile=2) # in tf repeat(image, 'h w -> h (tile w)', tile=2)
@@ -126,14 +128,16 @@
 perspective on the same question. ## Supported frameworks  Einops works with
 ... - [numpy](http://www.numpy.org/) - [pytorch](https://pytorch.org/) -
 [tensorflow](https://www.tensorflow.org/) - [jax](https://github.com/google/
 jax) - [cupy](https://cupy.chainer.org/) - [chainer](https://chainer.org/) -
 [tf.keras](https://www.tensorflow.org/guide/keras) - [oneflow](https://
 github.com/Oneflow-Inc/oneflow) (experimental) - [flax](https://github.com/
 google/flax) (experimental) - [paddle](https://github.com/PaddlePaddle/Paddle)
-(experimental) - [gluon](https://gluon.mxnet.io/) (deprecated) ## Citing einops
-Please use the following bibtex record ```text @inproceedings
-{ rogozhnikov2022einops, title={Einops: Clear and Reliable Tensor Manipulations
-with Einstein-like Notation}, author={Alex Rogozhnikov}, booktitle=
-{International Conference on Learning Representations}, year={2022}, url=
-{https://openreview.net/forum?id=oapKSVM2bcj} } ``` ## Supported python
-versions `einops` works with python 3.7 or later.
+(experimental) Additionally, starting from einops 0.7.0 einops can be used with
+any framework that supports [Python array API standard](https://data-apis.org/
+array-api/latest/API_specification/index.html) ## Citing einops  Please use the
+following bibtex record ```text @inproceedings{ rogozhnikov2022einops, title=
+{Einops: Clear and Reliable Tensor Manipulations with Einstein-like Notation},
+author={Alex Rogozhnikov}, booktitle={International Conference on Learning
+Representations}, year={2022}, url={https://openreview.net/
+forum?id=oapKSVM2bcj} } ``` ## Supported python versions `einops` works with
+python 3.8 or later.
```

### Comparing `einops-0.6.2rc0/pyproject.toml` & `einops-0.7.0rc1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -93,7 +93,11 @@
     "ignore:Call to deprecated create function FileDescriptor",
     "ignore:Call to deprecated create function OneofDescriptor",
 ]
 
 [tool.black]
 line-length = 120
 target-version = ['py311']
+
+
+[tool.ruff]
+line-length = 120
```

### Comparing `einops-0.6.2rc0/PKG-INFO` & `einops-0.7.0rc1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: einops
-Version: 0.6.2rc0
+Version: 0.7.0rc1
 Summary: A new flavour of deep learning operations
 Project-URL: Homepage, https://github.com/arogozhnikov/einops
 Author: Alex Rogozhnikov
 License: MIT
 License-File: LICENSE
 Keywords: deep learning,einops,machine learning,neural networks,scientific computations,tensor manipulation
 Classifier: Intended Audience :: Science/Research
@@ -40,30 +40,29 @@
 
 
 Flexible and powerful tensor operations for readable and reliable code. <br />
 Supports numpy, pytorch, tensorflow, jax, and [others](#supported-frameworks).
 
 ## Recent updates:
 
+- 0.7.0rc1: no-hassle `torch.compile`, support of [array api standard](https://data-apis.org/array-api/latest/API_specification/index.html) and more
 - 10'000: github reports that more than 10k project use einops 🎂
 - see how to use einops with [torch.compile](https://github.com/arogozhnikov/einops/wiki/Using-torch.compile-with-einops)
 - einops 0.6.1: paddle backend added
 - einops 0.6 introduces [packing and unpacking](https://github.com/arogozhnikov/einops/blob/master/docs/4-pack-and-unpack.ipynb)
 - einops 0.5: einsum is now a part of einops
 - [Einops paper](https://openreview.net/pdf?id=oapKSVM2bcj) is accepted for oral presentation at ICLR 2022 (yes, it worth reading).
   Talk recordings are [available](https://iclr.cc/virtual/2022/oral/6603)
 
 
-<details>
-  <summary>Previous updates</summary>
-  
-  
-  - flax and oneflow backend added
-  - torch.jit.script is supported for pytorch layers
-  - powerful EinMix added to einops. [Einmix tutorial notebook](https://github.com/arogozhnikov/einops/blob/master/docs/3-einmix-layer.ipynb) 
+<details markdown="1">
+<summary>Previous updates</summary>
+- flax and oneflow backend added
+- torch.jit.script is supported for pytorch layers
+- powerful EinMix added to einops. [Einmix tutorial notebook](https://github.com/arogozhnikov/einops/blob/master/docs/3-einmix-layer.ipynb) 
 </details>
 
 <!--<div align="center">
   <img src="http://arogozhnikov.github.io/images/einops/einops_logo_350x350.png" 
   alt="einops package logo" width="250" height="250" />
   <br><br>
 </div> -->
@@ -173,43 +172,42 @@
 
 Einops provides layers (`einops` keeps a separate version for each framework) that reflect corresponding functions
 
 ```python
 from einops.layers.torch      import Rearrange, Reduce
 from einops.layers.tensorflow import Rearrange, Reduce
 from einops.layers.flax       import Rearrange, Reduce
-from einops.layers.gluon      import Rearrange, Reduce
+from einops.layers.paddle     import Rearrange, Reduce
 from einops.layers.keras      import Rearrange, Reduce
 from einops.layers.chainer    import Rearrange, Reduce
 ```
 
-<details>
-  <summary>Example of using layers within a pytorch model</summary>
-  
-  
-  ```python
-  # example given for pytorch, but code in other frameworks is almost identical  
-  from torch.nn import Sequential, Conv2d, MaxPool2d, Linear, ReLU
-  from einops.layers.torch import Rearrange
-
-  model = Sequential(
-      ...,
-      Conv2d(6, 16, kernel_size=5),
-      MaxPool2d(kernel_size=2),
-      # flattening without need to write forward
-      Rearrange('b c h w -> b (c h w)'),  
-      Linear(16*5*5, 120), 
-      ReLU(),
-      Linear(120, 10), 
-  )
-  ```
-  
-  No more flatten needed! 
-  
-  Additionally, torch users will benefit from layers as those are script-able and compile-able.
+<details markdown="1">
+<summary>Example of using layers within a pytorch model</summary>
+Example given for pytorch, but code in other frameworks is almost identical
+
+```python 
+from torch.nn import Sequential, Conv2d, MaxPool2d, Linear, ReLU
+from einops.layers.torch import Rearrange
+
+model = Sequential(
+    ...,
+    Conv2d(6, 16, kernel_size=5),
+    MaxPool2d(kernel_size=2),
+    # flattening without need to write forward
+    Rearrange('b c h w -> b (c h w)'),  
+    Linear(16*5*5, 120), 
+    ReLU(),
+    Linear(120, 10), 
+)
+```
+
+No more flatten needed! 
+
+Additionally, torch users will benefit from layers as those are script-able and compile-able.
 </details>
 
 
 
 
 ## Naming <a name="Naming"></a>
 
@@ -295,15 +293,15 @@
 
 ```python
 y = x.flatten() # or flatten(x)
 ```
 
 Suppose `x`'s shape was `(3, 4, 5)`, then `y` has shape ...
 
-- numpy, cupy, chainer, pytorch: `(60,)`
+- numpy, pytorch, cupy, chainer: `(60,)`
 - keras, tensorflow.layers, gluon: `(3, 20)`
 
 `einops` works the same way in all frameworks.
 
 ### Independence of framework terminology
 
 Example: `tile` vs `repeat` causes lots of confusion. To copy image along width:
@@ -334,15 +332,16 @@
 - [jax](https://github.com/google/jax)
 - [cupy](https://cupy.chainer.org/)
 - [chainer](https://chainer.org/)
 - [tf.keras](https://www.tensorflow.org/guide/keras)
 - [oneflow](https://github.com/Oneflow-Inc/oneflow) (experimental)
 - [flax](https://github.com/google/flax) (experimental)
 - [paddle](https://github.com/PaddlePaddle/Paddle) (experimental)
-- [gluon](https://gluon.mxnet.io/) (deprecated)
+
+Additionally, starting from einops 0.7.0 einops can be used with any framework that supports [Python array API standard](https://data-apis.org/array-api/latest/API_specification/index.html)
 
 ## Citing einops <a name="Citing"></a>
 
 Please use the following bibtex record
 
 ```text
 @inproceedings{
@@ -354,8 +353,8 @@
     url={https://openreview.net/forum?id=oapKSVM2bcj}
 }
 ```
 
 
 ## Supported python versions
 
-`einops` works with python 3.7 or later.
+`einops` works with python 3.8 or later.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: einops Version: 0.6.2rc0 Summary: A new flavour of
+Metadata-Version: 2.1 Name: einops Version: 0.7.0rc1 Summary: A new flavour of
 deep learning operations Project-URL: Homepage, https://github.com/
 arogozhnikov/einops Author: Alex Rogozhnikov License: MIT License-File: LICENSE
 Keywords: deep learning,einops,machine learning,neural networks,scientific
 computations,tensor manipulation Classifier: Intended Audience :: Science/
 Research Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3 Requires-Python: >=3.8 Description-Content-
 Type: text/markdown   https://user-images.githubusercontent.com/6318811/
@@ -12,23 +12,25 @@
 run_tests.yml) [![PyPI version](https://badge.fury.io/py/einops.svg)](https://
 badge.fury.io/py/einops) [![Documentation](https://img.shields.io/badge/
 documentation-link-blue.svg)](https://einops.rocks/) ![Supported python
 versions](https://raw.githubusercontent.com/arogozhnikov/einops/master/docs/
 resources/python_badge.svg) Flexible and powerful tensor operations for
 readable and reliable code.
 Supports numpy, pytorch, tensorflow, jax, and [others](#supported-frameworks).
-## Recent updates: - 10'000: github reports that more than 10k project use
-einops ð - see how to use einops with [torch.compile](https://github.com/
-arogozhnikov/einops/wiki/Using-torch.compile-with-einops) - einops 0.6.1:
-paddle backend added - einops 0.6 introduces [packing and unpacking](https://
-github.com/arogozhnikov/einops/blob/master/docs/4-pack-and-unpack.ipynb) -
-einops 0.5: einsum is now a part of einops - [Einops paper](https://
-openreview.net/pdf?id=oapKSVM2bcj) is accepted for oral presentation at ICLR
-2022 (yes, it worth reading). Talk recordings are [available](https://iclr.cc/
-virtual/2022/oral/6603)  Previous updates - flax and oneflow backend added -
+## Recent updates: - 0.7.0rc1: no-hassle `torch.compile`, support of [array api
+standard](https://data-apis.org/array-api/latest/API_specification/index.html)
+and more - 10'000: github reports that more than 10k project use einops ð -
+see how to use einops with [torch.compile](https://github.com/arogozhnikov/
+einops/wiki/Using-torch.compile-with-einops) - einops 0.6.1: paddle backend
+added - einops 0.6 introduces [packing and unpacking](https://github.com/
+arogozhnikov/einops/blob/master/docs/4-pack-and-unpack.ipynb) - einops 0.5:
+einsum is now a part of einops - [Einops paper](https://openreview.net/
+pdf?id=oapKSVM2bcj) is accepted for oral presentation at ICLR 2022 (yes, it
+worth reading). Talk recordings are [available](https://iclr.cc/virtual/2022/
+oral/6603)  Previous updates - flax and oneflow backend added -
 torch.jit.script is supported for pytorch layers - powerful EinMix added to
 einops. [Einmix tutorial notebook](https://github.com/arogozhnikov/einops/blob/
 master/docs/3-einmix-layer.ipynb)   ## Tweets > In case you need convincing
 arguments for setting aside time to learn about einsum and einops... [Tim
 RocktÃ¤schel, FAIR](https://twitter.com/_rockt/status/1230818967205425152) >
 Writing better code with PyTorch and einops ð [Andrej Karpathy, AI at Tesla]
 (https://twitter.com/karpathy/status/1290826075916779520) > Slowly but surely,
@@ -70,19 +72,19 @@
 dot-product # but 1) axes can be multi-lettered 2) pattern goes last 3) works
 with multiple frameworks C = einsum(A, B, 'b t1 head c, b t2 head c -> b head
 t1 t2') ``` ### EinMix `EinMix` is a generic linear layer, perfect for MLP
 Mixers and similar architectures. ### Layers Einops provides layers (`einops`
 keeps a separate version for each framework) that reflect corresponding
 functions ```python from einops.layers.torch import Rearrange, Reduce from
 einops.layers.tensorflow import Rearrange, Reduce from einops.layers.flax
-import Rearrange, Reduce from einops.layers.gluon import Rearrange, Reduce from
-einops.layers.keras import Rearrange, Reduce from einops.layers.chainer import
-Rearrange, Reduce ```  Example of using layers within a pytorch model ```python
-# example given for pytorch, but code in other frameworks is almost identical
-from torch.nn import Sequential, Conv2d, MaxPool2d, Linear, ReLU from
+import Rearrange, Reduce from einops.layers.paddle import Rearrange, Reduce
+from einops.layers.keras import Rearrange, Reduce from einops.layers.chainer
+import Rearrange, Reduce ```  Example of using layers within a pytorch model
+Example given for pytorch, but code in other frameworks is almost identical
+```python from torch.nn import Sequential, Conv2d, MaxPool2d, Linear, ReLU from
 einops.layers.torch import Rearrange model = Sequential( ..., Conv2d(6, 16,
 kernel_size=5), MaxPool2d(kernel_size=2), # flattening without need to write
 forward Rearrange('b c h w -> b (c h w)'), Linear(16*5*5, 120), ReLU(), Linear
 (120, 10), ) ``` No more flatten needed! Additionally, torch users will benefit
 from layers as those are script-able and compile-able.  ## Naming  `einops`
 stands for Einstein-Inspired Notation for operations (though "Einstein
 operations" is more attractive and easier to remember). Notation was loosely
@@ -115,16 +117,16 @@
 c (x dx) (y dy) (z dz) -> b c x y z', 'max', dx=2, dy=3, dz=4) ``` These
 examples demonstrated that we don't use separate operations for 1d/2d/3d
 pooling, those are all defined in a uniform way. Space-to-depth and depth-to
 space are defined in many frameworks but how about width-to-height? Here you
 go: ```python rearrange(x, 'b c h (w w2) -> b c (h w2) w', w2=2) ``` ###
 Framework independent behavior Even simple functions are defined differently by
 different frameworks ```python y = x.flatten() # or flatten(x) ``` Suppose
-`x`'s shape was `(3, 4, 5)`, then `y` has shape ... - numpy, cupy, chainer,
-pytorch: `(60,)` - keras, tensorflow.layers, gluon: `(3, 20)` `einops` works
+`x`'s shape was `(3, 4, 5)`, then `y` has shape ... - numpy, pytorch, cupy,
+chainer: `(60,)` - keras, tensorflow.layers, gluon: `(3, 20)` `einops` works
 the same way in all frameworks. ### Independence of framework terminology
 Example: `tile` vs `repeat` causes lots of confusion. To copy image along
 width: ```python np.tile(image, (1, 2)) # in numpy image.repeat(1, 2) #
 pytorch's repeat ~ numpy's tile ``` With einops you don't need to decipher
 which axis was repeated: ```python repeat(image, 'h w -> h (tile w)', tile=2) #
 in numpy repeat(image, 'h w -> h (tile w)', tile=2) # in pytorch repeat(image,
 'h w -> h (tile w)', tile=2) # in tf repeat(image, 'h w -> h (tile w)', tile=2)
@@ -133,14 +135,16 @@
 perspective on the same question. ## Supported frameworks  Einops works with
 ... - [numpy](http://www.numpy.org/) - [pytorch](https://pytorch.org/) -
 [tensorflow](https://www.tensorflow.org/) - [jax](https://github.com/google/
 jax) - [cupy](https://cupy.chainer.org/) - [chainer](https://chainer.org/) -
 [tf.keras](https://www.tensorflow.org/guide/keras) - [oneflow](https://
 github.com/Oneflow-Inc/oneflow) (experimental) - [flax](https://github.com/
 google/flax) (experimental) - [paddle](https://github.com/PaddlePaddle/Paddle)
-(experimental) - [gluon](https://gluon.mxnet.io/) (deprecated) ## Citing einops
-Please use the following bibtex record ```text @inproceedings
-{ rogozhnikov2022einops, title={Einops: Clear and Reliable Tensor Manipulations
-with Einstein-like Notation}, author={Alex Rogozhnikov}, booktitle=
-{International Conference on Learning Representations}, year={2022}, url=
-{https://openreview.net/forum?id=oapKSVM2bcj} } ``` ## Supported python
-versions `einops` works with python 3.7 or later.
+(experimental) Additionally, starting from einops 0.7.0 einops can be used with
+any framework that supports [Python array API standard](https://data-apis.org/
+array-api/latest/API_specification/index.html) ## Citing einops  Please use the
+following bibtex record ```text @inproceedings{ rogozhnikov2022einops, title=
+{Einops: Clear and Reliable Tensor Manipulations with Einstein-like Notation},
+author={Alex Rogozhnikov}, booktitle={International Conference on Learning
+Representations}, year={2022}, url={https://openreview.net/
+forum?id=oapKSVM2bcj} } ``` ## Supported python versions `einops` works with
+python 3.8 or later.
```

