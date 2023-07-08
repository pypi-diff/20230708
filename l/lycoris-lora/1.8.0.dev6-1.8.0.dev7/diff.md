# Comparing `tmp/lycoris_lora-1.8.0.dev6.tar.gz` & `tmp/lycoris_lora-1.8.0.dev7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lycoris_lora-1.8.0.dev6.tar", last modified: Sat Jul  1 13:34:49 2023, max compression
+gzip compressed data, was "lycoris_lora-1.8.0.dev7.tar", last modified: Sat Jul  8 09:15:00 2023, max compression
```

## Comparing `lycoris_lora-1.8.0.dev6.tar` & `lycoris_lora-1.8.0.dev7.tar`

### file list

```diff
@@ -1,28 +1,47 @@
-drwxrwxrwx   0        0        0        0 2023-07-01 13:34:49.373167 lycoris_lora-1.8.0.dev6/
--rw-rw-rw-   0        0        0    11545 2023-06-04 13:36:43.000000 lycoris_lora-1.8.0.dev6/LICENSE.md
--rw-rw-rw-   0        0        0      353 2023-07-01 13:34:49.372142 lycoris_lora-1.8.0.dev6/PKG-INFO
--rw-rw-rw-   0        0        0     7677 2023-06-28 12:51:02.000000 lycoris_lora-1.8.0.dev6/README.md
-drwxrwxrwx   0        0        0        0 2023-07-01 13:34:49.357799 lycoris_lora-1.8.0.dev6/lycoris/
--rw-rw-rw-   0        0        0        0 2023-07-01 11:57:57.000000 lycoris_lora-1.8.0.dev6/lycoris/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-01 13:34:49.359799 lycoris_lora-1.8.0.dev6/lycoris/kohya/
--rw-rw-rw-   0        0        0    24690 2023-06-29 04:44:57.000000 lycoris_lora-1.8.0.dev6/lycoris/kohya/__init__.py
--rw-rw-rw-   0        0        0    48868 2023-06-29 04:44:57.000000 lycoris_lora-1.8.0.dev6/lycoris/kohya/kohya_model_utils.py
--rw-rw-rw-   0        0        0     1512 2023-06-29 04:44:57.000000 lycoris_lora-1.8.0.dev6/lycoris/kohya/kohya_utils.py
-drwxrwxrwx   0        0        0        0 2023-07-01 13:34:49.363803 lycoris_lora-1.8.0.dev6/lycoris/modules/
--rw-rw-rw-   0        0        0        0 2023-07-01 07:43:35.000000 lycoris_lora-1.8.0.dev6/lycoris/modules/__init__.py
--rw-rw-rw-   0        0        0     4762 2023-06-30 13:07:32.000000 lycoris_lora-1.8.0.dev6/lycoris/modules/dylora.py
--rw-rw-rw-   0        0        0     4117 2023-06-29 04:44:57.000000 lycoris_lora-1.8.0.dev6/lycoris/modules/glora.py
--rw-rw-rw-   0        0        0     2103 2023-06-29 04:44:57.000000 lycoris_lora-1.8.0.dev6/lycoris/modules/ia3.py
--rw-rw-rw-   0        0        0     4468 2023-06-29 04:44:57.000000 lycoris_lora-1.8.0.dev6/lycoris/modules/locon.py
--rw-rw-rw-   0        0        0     8831 2023-06-29 04:44:57.000000 lycoris_lora-1.8.0.dev6/lycoris/modules/loha.py
--rw-rw-rw-   0        0        0    10810 2023-07-01 13:34:19.000000 lycoris_lora-1.8.0.dev6/lycoris/modules/lokr.py
--rw-rw-rw-   0        0        0    20963 2023-06-04 13:36:43.000000 lycoris_lora-1.8.0.dev6/lycoris/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-01 13:34:49.372142 lycoris_lora-1.8.0.dev6/lycoris_lora.egg-info/
--rw-rw-rw-   0        0        0      353 2023-07-01 13:34:49.000000 lycoris_lora-1.8.0.dev6/lycoris_lora.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      545 2023-07-01 13:34:49.000000 lycoris_lora-1.8.0.dev6/lycoris_lora.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-01 13:34:49.000000 lycoris_lora-1.8.0.dev6/lycoris_lora.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-06-04 13:39:16.000000 lycoris_lora-1.8.0.dev6/lycoris_lora.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       41 2023-07-01 13:34:49.000000 lycoris_lora-1.8.0.dev6/lycoris_lora.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-07-01 13:34:49.000000 lycoris_lora-1.8.0.dev6/lycoris_lora.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-01 13:34:49.373167 lycoris_lora-1.8.0.dev6/setup.cfg
--rw-rw-rw-   0        0        0      566 2023-07-01 13:34:47.000000 lycoris_lora-1.8.0.dev6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-08 09:15:00.688833 lycoris_lora-1.8.0.dev7/
+-rw-rw-rw-   0        0        0     1623 2023-03-09 05:37:07.000000 lycoris_lora-1.8.0.dev7/.gitignore
+-rw-rw-rw-   0        0        0     4436 2023-04-09 13:45:45.000000 lycoris_lora-1.8.0.dev7/Algo.md
+-rw-rw-rw-   0        0        0      977 2023-07-02 13:30:53.000000 lycoris_lora-1.8.0.dev7/Change.md
+-rw-rw-rw-   0        0        0     2828 2023-03-09 12:01:15.000000 lycoris_lora-1.8.0.dev7/Demo.md
+-rw-rw-rw-   0        0        0    11545 2023-03-09 05:37:07.000000 lycoris_lora-1.8.0.dev7/LICENSE.md
+-rw-rw-rw-   0        0        0      353 2023-07-08 09:15:00.688332 lycoris_lora-1.8.0.dev7/PKG-INFO
+-rw-rw-rw-   0        0        0     7677 2023-07-02 13:30:53.000000 lycoris_lora-1.8.0.dev7/README.md
+drwxrwxrwx   0        0        0        0 2023-07-08 09:15:00.671808 lycoris_lora-1.8.0.dev7/experiments/
+-rw-rw-rw-   0        0        0     3579 2023-03-12 01:46:48.000000 lycoris_lora-1.8.0.dev7/experiments/better_conv.py
+-rw-rw-rw-   0        0        0     1967 2023-03-12 01:46:43.000000 lycoris_lora-1.8.0.dev7/experiments/better_conv_extract.py
+-rw-rw-rw-   0        0        0     8783 2023-03-12 03:21:33.000000 lycoris_lora-1.8.0.dev7/experiments/concept_neuron.py
+-rw-rw-rw-   0        0        0      894 2023-03-09 14:26:54.000000 lycoris_lora-1.8.0.dev7/experiments/locon_extract_test.py
+-rw-rw-rw-   0        0        0      755 2023-03-10 15:36:09.000000 lycoris_lora-1.8.0.dev7/experiments/locon_merge_test.py
+-rw-rw-rw-   0        0        0     3411 2023-03-09 05:37:07.000000 lycoris_lora-1.8.0.dev7/experiments/singular_value_test.py
+-rw-rw-rw-   0        0        0     2334 2023-03-11 09:28:26.000000 lycoris_lora-1.8.0.dev7/experiments/sparse_bias_test.py
+-rw-rw-rw-   0        0        0     2791 2023-03-12 01:46:48.000000 lycoris_lora-1.8.0.dev7/experiments/time_test.py
+-rw-rw-rw-   0        0        0      255 2023-06-25 07:25:35.000000 lycoris_lora-1.8.0.dev7/experiments/weakre_speed.py
+drwxrwxrwx   0        0        0        0 2023-07-08 09:15:00.672308 lycoris_lora-1.8.0.dev7/lycoris/
+-rw-rw-rw-   0        0        0        0 2023-07-02 13:30:53.000000 lycoris_lora-1.8.0.dev7/lycoris/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-08 09:15:00.672808 lycoris_lora-1.8.0.dev7/lycoris/kohya/
+-rw-rw-rw-   0        0        0    24690 2023-07-02 13:30:53.000000 lycoris_lora-1.8.0.dev7/lycoris/kohya/__init__.py
+-rw-rw-rw-   0        0        0    48868 2023-07-02 13:30:53.000000 lycoris_lora-1.8.0.dev7/lycoris/kohya/kohya_model_utils.py
+-rw-rw-rw-   0        0        0     1512 2023-07-02 13:30:53.000000 lycoris_lora-1.8.0.dev7/lycoris/kohya/kohya_utils.py
+drwxrwxrwx   0        0        0        0 2023-07-08 09:15:00.676312 lycoris_lora-1.8.0.dev7/lycoris/modules/
+-rw-rw-rw-   0        0        0        0 2023-07-02 13:30:53.000000 lycoris_lora-1.8.0.dev7/lycoris/modules/__init__.py
+-rw-rw-rw-   0        0        0     4762 2023-07-02 13:30:53.000000 lycoris_lora-1.8.0.dev7/lycoris/modules/dylora.py
+-rw-rw-rw-   0        0        0    10763 2023-07-06 08:19:32.000000 lycoris_lora-1.8.0.dev7/lycoris/modules/glokr.py
+-rw-rw-rw-   0        0        0     4117 2023-07-02 13:30:53.000000 lycoris_lora-1.8.0.dev7/lycoris/modules/glora.py
+-rw-rw-rw-   0        0        0     2103 2023-07-02 13:30:53.000000 lycoris_lora-1.8.0.dev7/lycoris/modules/ia3.py
+-rw-rw-rw-   0        0        0     4468 2023-07-02 13:30:53.000000 lycoris_lora-1.8.0.dev7/lycoris/modules/locon.py
+-rw-rw-rw-   0        0        0     8830 2023-07-08 06:50:22.000000 lycoris_lora-1.8.0.dev7/lycoris/modules/loha.py
+-rw-rw-rw-   0        0        0    10896 2023-07-08 09:14:16.000000 lycoris_lora-1.8.0.dev7/lycoris/modules/lokr.py
+-rw-rw-rw-   0        0        0    20963 2023-06-05 03:39:30.000000 lycoris_lora-1.8.0.dev7/lycoris/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-08 09:15:00.687327 lycoris_lora-1.8.0.dev7/lycoris_lora.egg-info/
+-rw-rw-rw-   0        0        0      353 2023-07-08 09:15:00.000000 lycoris_lora-1.8.0.dev7/lycoris_lora.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      940 2023-07-08 09:15:00.000000 lycoris_lora-1.8.0.dev7/lycoris_lora.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-08 09:15:00.000000 lycoris_lora-1.8.0.dev7/lycoris_lora.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-03-09 13:25:15.000000 lycoris_lora-1.8.0.dev7/lycoris_lora.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       41 2023-07-08 09:15:00.000000 lycoris_lora-1.8.0.dev7/lycoris_lora.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-07-08 09:15:00.000000 lycoris_lora-1.8.0.dev7/lycoris_lora.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       58 2023-07-02 13:30:53.000000 lycoris_lora-1.8.0.dev7/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-07-08 09:15:00.688833 lycoris_lora-1.8.0.dev7/setup.cfg
+-rw-rw-rw-   0        0        0      566 2023-07-08 09:14:44.000000 lycoris_lora-1.8.0.dev7/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-08 09:15:00.688332 lycoris_lora-1.8.0.dev7/tools/
+-rw-rw-rw-   0        0        0     4087 2023-03-12 16:11:52.000000 lycoris_lora-1.8.0.dev7/tools/extract_locon.py
+-rw-rw-rw-   0        0        0     2293 2023-06-05 03:39:47.000000 lycoris_lora-1.8.0.dev7/tools/merge.py
```

### Comparing `lycoris_lora-1.8.0.dev6/LICENSE.md` & `lycoris_lora-1.8.0.dev7/LICENSE.md`

 * *Files identical despite different names*

### Comparing `lycoris_lora-1.8.0.dev6/README.md` & `lycoris_lora-1.8.0.dev7/README.md`

 * *Files identical despite different names*

### Comparing `lycoris_lora-1.8.0.dev6/lycoris/kohya/__init__.py` & `lycoris_lora-1.8.0.dev7/lycoris/kohya/__init__.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-1.8.0.dev6/lycoris/kohya/kohya_model_utils.py` & `lycoris_lora-1.8.0.dev7/lycoris/kohya/kohya_model_utils.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-1.8.0.dev6/lycoris/kohya/kohya_utils.py` & `lycoris_lora-1.8.0.dev7/lycoris/kohya/kohya_utils.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-1.8.0.dev6/lycoris/modules/dylora.py` & `lycoris_lora-1.8.0.dev7/lycoris/modules/dylora.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-1.8.0.dev6/lycoris/modules/glora.py` & `lycoris_lora-1.8.0.dev7/lycoris/modules/glora.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-1.8.0.dev6/lycoris/modules/ia3.py` & `lycoris_lora-1.8.0.dev7/lycoris/modules/ia3.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-1.8.0.dev6/lycoris/modules/locon.py` & `lycoris_lora-1.8.0.dev7/lycoris/modules/locon.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-1.8.0.dev6/lycoris/modules/loha.py` & `lycoris_lora-1.8.0.dev7/lycoris/modules/loha.py`

 * *Files 0% similar despite different names*

```diff
@@ -148,21 +148,21 @@
         
         if type(alpha) == torch.Tensor:
             alpha = alpha.detach().float().numpy()  # without casting, bf16 causes error
         alpha = lora_dim if alpha is None or alpha == 0 else alpha
         self.scale = alpha / self.lora_dim
         self.register_buffer('alpha', torch.tensor(alpha)) # 定数として扱える
 
-        # Need more experiences on init method
+        # Need more experiments on init method
         if self.cp:
             torch.nn.init.normal_(self.hada_t1, std=0.1)
             torch.nn.init.normal_(self.hada_t2, std=0.1)
         torch.nn.init.normal_(self.hada_w1_b, std=1)
-        torch.nn.init.normal_(self.hada_w2_b, std=0.01)
-        torch.nn.init.normal_(self.hada_w1_a, std=1)
+        torch.nn.init.normal_(self.hada_w1_a, std=0.1)
+        torch.nn.init.normal_(self.hada_w2_b, std=1)
         torch.nn.init.constant_(self.hada_w2_a, 0)
 
         self.multiplier = multiplier
         self.org_module = [org_module] # remove in applying
         self.grad_ckpt = False
 
     def apply_to(self):
```

### Comparing `lycoris_lora-1.8.0.dev6/lycoris/modules/lokr.py` & `lycoris_lora-1.8.0.dev7/lycoris/modules/glokr.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 import math
 
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 
-# 4, build custom backward function
-#  - 
-
 
 def factorization(dimension: int, factor:int=-1) -> tuple[int, int]:
     '''
     return a tuple of two value of input dimension decomposed by the number closest to factor
     second value is higher or equal than first value.
     
     In LoRA with Kroneckor Product, first value is a value for weight scale.
@@ -19,15 +16,15 @@
     Becuase of non-commutative property, A⊗B ≠ B⊗A. Meaning of two matrices is slightly different.
     
     examples)
     factor
         -1               2                4               8               16               ...
     127 -> 127, 1   127 -> 127, 1    127 -> 127, 1   127 -> 127, 1   127 -> 127, 1
     128 -> 16, 8    128 -> 64, 2     128 -> 32, 4    128 -> 16, 8    128 -> 16, 8
-    250 -> 125, 2   250 -> 125, 2    250 -> 125, 2   250 -> 125, 2   250 -> 125, 2
+    250 -> 25, 10   250 -> 125, 2    250 -> 125, 2   250 -> 50, 5   250 -> 25, 10
     360 -> 45, 8    360 -> 180, 2    360 -> 90, 4    360 -> 45, 8    360 -> 45, 8
     512 -> 32, 16   512 -> 256, 2    512 -> 128, 4   512 -> 64, 8    512 -> 32, 16
     1024 -> 32, 32  1024 -> 512, 2   1024 -> 256, 4  1024 -> 128, 8  1024 -> 64, 16
     '''
     
     if factor > 0 and (dimension % factor) == 0:
         m = factor
```

### Comparing `lycoris_lora-1.8.0.dev6/lycoris/utils.py` & `lycoris_lora-1.8.0.dev7/lycoris/utils.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-1.8.0.dev6/lycoris_lora.egg-info/SOURCES.txt` & `lycoris_lora-1.8.0.dev7/lycoris_lora.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,38 @@
+.gitignore
+Algo.md
+Change.md
+Demo.md
 LICENSE.md
 README.md
+requirements.txt
 setup.py
+experiments/better_conv.py
+experiments/better_conv_extract.py
+experiments/concept_neuron.py
+experiments/locon_extract_test.py
+experiments/locon_merge_test.py
+experiments/singular_value_test.py
+experiments/sparse_bias_test.py
+experiments/time_test.py
+experiments/weakre_speed.py
 lycoris/__init__.py
 lycoris/utils.py
 lycoris/kohya/__init__.py
 lycoris/kohya/kohya_model_utils.py
 lycoris/kohya/kohya_utils.py
 lycoris/modules/__init__.py
 lycoris/modules/dylora.py
+lycoris/modules/glokr.py
 lycoris/modules/glora.py
 lycoris/modules/ia3.py
 lycoris/modules/locon.py
 lycoris/modules/loha.py
 lycoris/modules/lokr.py
 lycoris_lora.egg-info/PKG-INFO
 lycoris_lora.egg-info/SOURCES.txt
 lycoris_lora.egg-info/dependency_links.txt
 lycoris_lora.egg-info/not-zip-safe
 lycoris_lora.egg-info/requires.txt
-lycoris_lora.egg-info/top_level.txt
+lycoris_lora.egg-info/top_level.txt
+tools/extract_locon.py
+tools/merge.py
```

### Comparing `lycoris_lora-1.8.0.dev6/setup.py` & `lycoris_lora-1.8.0.dev7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
     name='lycoris_lora',
     packages=find_packages(),
-    version='1.8.0.dev6',
+    version='1.8.0.dev7',
     url='https://github.com/KohakuBlueleaf/LyCORIS',
     description='Lora beYond Conventional methods, Other Rank adaptation Implementations for Stable diffusion',
     author='Shih-Ying Yeh(KohakuBlueLeaf), Yu-Guan Hsieh, Zhidong Gao',
     author_email='apolloyeh0123@gmail.com',
     zip_safe=False,
     install_requires=[
         'torch',
```

