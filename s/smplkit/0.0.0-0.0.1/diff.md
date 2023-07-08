# Comparing `tmp/smplkit-0.0.0.tar.gz` & `tmp/smplkit-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smplkit-0.0.0.tar", last modified: Fri Jul  7 13:54:03 2023, max compression
+gzip compressed data, was "smplkit-0.0.1.tar", last modified: Sat Jul  8 08:43:57 2023, max compression
```

## Comparing `smplkit-0.0.0.tar` & `smplkit-0.0.1.tar`

### file list

```diff
@@ -1,14 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:54:03.792242 smplkit-0.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-07 13:53:35.000000 smplkit-0.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-07-07 13:54:03.792242 smplkit-0.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-07-07 13:53:35.000000 smplkit-0.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 13:54:03.792242 smplkit-0.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-07-07 13:53:35.000000 smplkit-0.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:54:03.792242 smplkit-0.0.0/smplkit/
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-07 13:53:35.000000 smplkit-0.0.0/smplkit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-07 13:53:36.000000 smplkit-0.0.0/smplkit/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:54:03.792242 smplkit-0.0.0/smplkit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-07-07 13:54:03.000000 smplkit-0.0.0/smplkit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-07-07 13:54:03.000000 smplkit-0.0.0/smplkit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 13:54:03.000000 smplkit-0.0.0/smplkit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-07 13:54:03.000000 smplkit-0.0.0/smplkit.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 08:43:57.115253 smplkit-0.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-08 08:43:46.000000 smplkit-0.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2945 2023-07-08 08:43:57.115253 smplkit-0.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-07-08 08:43:46.000000 smplkit-0.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 08:43:57.115253 smplkit-0.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-07-08 08:43:46.000000 smplkit-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 08:43:57.115253 smplkit-0.0.1/smplkit/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-08 08:43:46.000000 smplkit-0.0.1/smplkit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-08 08:43:47.000000 smplkit-0.0.1/smplkit/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7216 2023-07-08 08:43:46.000000 smplkit-0.0.1/smplkit/layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13836 2023-07-08 08:43:46.000000 smplkit-0.0.1/smplkit/lbs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3693 2023-07-08 08:43:46.000000 smplkit-0.0.1/smplkit/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7280 2023-07-08 08:43:46.000000 smplkit-0.0.1/smplkit/params.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 08:43:57.115253 smplkit-0.0.1/smplkit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2945 2023-07-08 08:43:57.000000 smplkit-0.0.1/smplkit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-07-08 08:43:57.000000 smplkit-0.0.1/smplkit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 08:43:57.000000 smplkit-0.0.1/smplkit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-08 08:43:57.000000 smplkit-0.0.1/smplkit.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 08:43:57.115253 smplkit-0.0.1/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-07-08 08:43:46.000000 smplkit-0.0.1/test/test.py
```

### Comparing `smplkit-0.0.0/LICENSE` & `smplkit-0.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `smplkit-0.0.0/PKG-INFO` & `smplkit-0.0.1/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smplkit
-Version: 0.0.0
+Version: 0.0.1
 Summary: SMPL-KIT: Use SMPL models more easily.
 Home-page: https://github.com/Silverster98/smpl-kit
 Author: Zan Wang
 Author-email: zanwang98@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -37,21 +37,71 @@
 ```
 
 - Or, clone this repository and install it from source:
 
 ```bash
 git clone git@github.com:Silverster98/smpl-kit.git
 cd smpl-kit
-pip install . --use-feature=in-tree-build
+pip install .
 ```
 
 ## Documentation
 
 ### Tutorial
 
-### API Reference
+#### 1. Use the `SMPLLayer` to generate a SMPL body mesh with random translation while keeping other parameters as zero:
+
+```python
+import torch
+import trimesh
+from smplkit import SMPLLayer as SMPL
+
+NJOINTS = 23
+
+body_model = SMPL(num_betas=10)
+
+transl = torch.rand((1, 3), dtype=torch.float32)
+
+verts = body_model(transl=transl, return_verts=True)
+faces = body_model.faces
+verts = verts.cpu().numpy()
+
+mesh = trimesh.Trimesh(vertices=verts[0], faces=body_model.faces)
+```
+
+#### 2. Use the `SMPLParam` to optimize the SMPL parameters (**only tranlation**) with a given mesh:
+
+```python
+import torch
+from smplkit import SMPLLayer as SMPL
+from smplkit import SMPLParam
+from torch.optim import SGD
+
+bm = SMPL(num_betas=10)
+
+target_transl = torch.tensor([[0, 1, 0]], dtype=torch.float32)
+target_verts = bm(transl=target_transl, return_verts=True)
+
+## init param and optimizer
+param = SMPLParam(transl=torch.rand(1, 3), requires_grad=[True, False, False, False])
+opt = SGD(param.trainable_parameters(), lr=0.1)
+
+for i in range(200):
+    opt.zero_grad()
+    output = bm(**param._parameters_dict(), return_verts=True)
+    
+    loss = ((output - target_verts) ** 2).mean()
+    
+    loss.backward()
+    opt.step()
+
+    if (i + 1) % 20 == 0:
+        print(f"Optimization Error in Step {i + 1:3d}: {loss.item()}")
+```
 
 ## License
 
 This project is licensed under the terms of the [MIT](LICENSE) license.
 
 ## Acknowledgement
+
+Some codes are borrowed from [SMPL-X](https://github.com/vchoutas/smplx). If your use this code, please consider citing the most relevant [works](https://github.com/vchoutas/smplx#citation).
```

### Comparing `smplkit-0.0.0/setup.py` & `smplkit-0.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `smplkit-0.0.0/smplkit.egg-info/PKG-INFO` & `smplkit-0.0.1/smplkit.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smplkit
-Version: 0.0.0
+Version: 0.0.1
 Summary: SMPL-KIT: Use SMPL models more easily.
 Home-page: https://github.com/Silverster98/smpl-kit
 Author: Zan Wang
 Author-email: zanwang98@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -37,21 +37,71 @@
 ```
 
 - Or, clone this repository and install it from source:
 
 ```bash
 git clone git@github.com:Silverster98/smpl-kit.git
 cd smpl-kit
-pip install . --use-feature=in-tree-build
+pip install .
 ```
 
 ## Documentation
 
 ### Tutorial
 
-### API Reference
+#### 1. Use the `SMPLLayer` to generate a SMPL body mesh with random translation while keeping other parameters as zero:
+
+```python
+import torch
+import trimesh
+from smplkit import SMPLLayer as SMPL
+
+NJOINTS = 23
+
+body_model = SMPL(num_betas=10)
+
+transl = torch.rand((1, 3), dtype=torch.float32)
+
+verts = body_model(transl=transl, return_verts=True)
+faces = body_model.faces
+verts = verts.cpu().numpy()
+
+mesh = trimesh.Trimesh(vertices=verts[0], faces=body_model.faces)
+```
+
+#### 2. Use the `SMPLParam` to optimize the SMPL parameters (**only tranlation**) with a given mesh:
+
+```python
+import torch
+from smplkit import SMPLLayer as SMPL
+from smplkit import SMPLParam
+from torch.optim import SGD
+
+bm = SMPL(num_betas=10)
+
+target_transl = torch.tensor([[0, 1, 0]], dtype=torch.float32)
+target_verts = bm(transl=target_transl, return_verts=True)
+
+## init param and optimizer
+param = SMPLParam(transl=torch.rand(1, 3), requires_grad=[True, False, False, False])
+opt = SGD(param.trainable_parameters(), lr=0.1)
+
+for i in range(200):
+    opt.zero_grad()
+    output = bm(**param._parameters_dict(), return_verts=True)
+    
+    loss = ((output - target_verts) ** 2).mean()
+    
+    loss.backward()
+    opt.step()
+
+    if (i + 1) % 20 == 0:
+        print(f"Optimization Error in Step {i + 1:3d}: {loss.item()}")
+```
 
 ## License
 
 This project is licensed under the terms of the [MIT](LICENSE) license.
 
 ## Acknowledgement
+
+Some codes are borrowed from [SMPL-X](https://github.com/vchoutas/smplx). If your use this code, please consider citing the most relevant [works](https://github.com/vchoutas/smplx#citation).
```

