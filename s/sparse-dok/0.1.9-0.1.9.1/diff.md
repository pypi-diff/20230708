# Comparing `tmp/sparse_dok-0.1.9.tar.gz` & `tmp/sparse_dok-0.1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sparse_dok-0.1.9.tar", last modified: Sat Jul  8 01:13:32 2023, max compression
+gzip compressed data, was "sparse_dok-0.1.9.1.tar", last modified: Sat Jul  8 01:15:09 2023, max compression
```

## Comparing `sparse_dok-0.1.9.tar` & `sparse_dok-0.1.9.1.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxrwxrwx   0        0        0        0 2023-07-08 01:13:32.164100 sparse_dok-0.1.9/
--rw-rw-rw-   0        0        0     1088 2023-07-08 01:12:38.000000 sparse_dok-0.1.9/LICENCE
--rw-rw-rw-   0        0        0       39 2022-06-03 19:13:32.000000 sparse_dok-0.1.9/MANIFEST.in
--rw-rw-rw-   0        0        0      953 2023-07-08 01:13:32.163100 sparse_dok-0.1.9/PKG-INFO
--rw-rw-rw-   0        0        0     8731 2023-07-08 01:12:38.000000 sparse_dok-0.1.9/README.md
--rw-rw-rw-   0        0        0       42 2023-07-08 01:13:32.164100 sparse_dok-0.1.9/setup.cfg
--rw-rw-rw-   0        0        0     1301 2023-03-21 13:22:47.000000 sparse_dok-0.1.9/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-08 01:13:32.063101 sparse_dok-0.1.9/sparse_dok/
--rw-rw-rw-   0        0        0       95 2023-07-08 01:11:28.000000 sparse_dok-0.1.9/sparse_dok/__init__.py
--rw-rw-rw-   0        0        0       21 2023-07-08 01:10:29.000000 sparse_dok-0.1.9/sparse_dok/__version__.py
-drwxrwxrwx   0        0        0        0 2023-07-08 01:13:32.084102 sparse_dok-0.1.9/sparse_dok/components/
--rw-rw-rw-   0        0        0       98 2022-06-03 18:42:54.000000 sparse_dok-0.1.9/sparse_dok/components/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-08 01:13:32.159101 sparse_dok-0.1.9/sparse_dok/components/cuda/
--rw-rw-rw-   0        0        0        0 2022-05-23 01:01:14.000000 sparse_dok-0.1.9/sparse_dok/components/cuda/__init__.py
--rw-rw-rw-   0        0        0     2878 2022-05-30 20:40:04.000000 sparse_dok-0.1.9/sparse_dok/components/cuda/binary_search.cu
--rw-rw-rw-   0        0        0    18343 2022-05-24 15:02:58.000000 sparse_dok-0.1.9/sparse_dok/components/cuda/bitonic.cu
--rw-rw-rw-   0        0        0    14628 2022-05-23 01:50:08.000000 sparse_dok-0.1.9/sparse_dok/components/cuda/bmm_helpers.cu
--rw-rw-rw-   0        0        0     6398 2022-11-15 22:41:58.000000 sparse_dok-0.1.9/sparse_dok/components/cuda/closed_hashmap_impl.cu
--rw-rw-rw-   0        0        0     9899 2022-12-05 14:46:18.000000 sparse_dok-0.1.9/sparse_dok/components/cuda/closed_hashmap_impl.py
--rw-rw-rw-   0        0        0    18328 2022-11-20 15:11:16.000000 sparse_dok-0.1.9/sparse_dok/components/cuda/closed_hashmap_impl_class.cu
--rw-rw-rw-   0        0        0    38155 2023-07-08 01:13:31.000000 sparse_dok-0.1.9/sparse_dok/components/cuda/closed_hashmap_impl_preview.cu
--rw-rw-rw-   0        0        0     6776 2022-11-19 20:13:52.000000 sparse_dok-0.1.9/sparse_dok/components/cuda/cuda_kernel.py
--rw-rw-rw-   0        0        0     1362 2022-11-11 22:10:53.000000 sparse_dok-0.1.9/sparse_dok/components/cuda/filtered_elementwise.py
--rw-rw-rw-   0        0        0     6711 2022-05-25 17:47:18.000000 sparse_dok-0.1.9/sparse_dok/components/cuda/hashmap.cu
--rw-rw-rw-   0        0        0     4028 2022-12-05 13:56:04.000000 sparse_dok-0.1.9/sparse_dok/components/cuda/head.cu
--rw-rw-rw-   0        0        0    35905 2022-11-17 22:43:16.000000 sparse_dok-0.1.9/sparse_dok/components/cuda/preview.cu
--rw-rw-rw-   0        0        0     3417 2022-11-15 23:20:13.000000 sparse_dok-0.1.9/sparse_dok/components/cuda/reduce.cu
--rw-rw-rw-   0        0        0    15548 2022-12-06 13:06:16.000000 sparse_dok-0.1.9/sparse_dok/components/cuda/safe_closed_hashmap_impl_class.cu
--rw-rw-rw-   0        0        0     7944 2022-05-31 14:14:10.000000 sparse_dok-0.1.9/sparse_dok/components/cuda/smem_hashmap.cu
--rw-rw-rw-   0        0        0     7903 2022-05-29 01:53:58.000000 sparse_dok-0.1.9/sparse_dok/components/cuda/smem_hashmap_simple.cu
--rw-rw-rw-   0        0        0     9395 2022-11-13 23:05:51.000000 sparse_dok-0.1.9/sparse_dok/components/cuda/smem_tensor.cu
--rw-rw-rw-   0        0        0    10707 2022-11-20 14:28:17.000000 sparse_dok-0.1.9/sparse_dok/components/cuda/sparse_dok_tensor_impl.cu
--rw-rw-rw-   0        0        0    25049 2022-12-06 13:06:44.000000 sparse_dok-0.1.9/sparse_dok/components/cuda/sparse_dok_tensor_impl.py
--rw-rw-rw-   0        0        0    52037 2023-07-08 01:13:31.000000 sparse_dok-0.1.9/sparse_dok/components/cuda/sparse_dok_tensor_impl_preview.cu
--rw-rw-rw-   0        0        0     1541 2022-05-24 20:22:36.000000 sparse_dok-0.1.9/sparse_dok/components/cuda/stack.cu
--rw-rw-rw-   0        0        0     6152 2022-11-20 23:38:59.000000 sparse_dok-0.1.9/sparse_dok/components/cuda/tensor_accessor.cu
--rw-rw-rw-   0        0        0    11198 2022-06-03 18:56:52.000000 sparse_dok-0.1.9/sparse_dok/components/cuda/topkspspcsim.cu
--rw-rw-rw-   0        0        0    10190 2022-11-11 21:44:22.000000 sparse_dok-0.1.9/sparse_dok/components/cuda/topkspspcsim.py
--rw-rw-rw-   0        0        0     1161 2022-11-17 22:40:56.000000 sparse_dok-0.1.9/sparse_dok/components/cuda_callable.py
--rw-rw-rw-   0        0        0    15308 2022-11-19 20:01:57.000000 sparse_dok-0.1.9/sparse_dok/components/cuda_closed_hashmap.py
--rw-rw-rw-   0        0        0    17858 2022-11-20 00:15:06.000000 sparse_dok-0.1.9/sparse_dok/components/sparse_dok_tensor.py
--rw-rw-rw-   0        0        0     6264 2022-11-11 21:43:04.000000 sparse_dok-0.1.9/sparse_dok/functions.py
--rw-rw-rw-   0        0        0    10849 2022-11-19 19:06:50.000000 sparse_dok-0.1.9/sparse_dok/util.py
-drwxrwxrwx   0        0        0        0 2023-07-08 01:13:32.081100 sparse_dok-0.1.9/sparse_dok.egg-info/
--rw-rw-rw-   0        0        0      953 2023-07-08 01:13:31.000000 sparse_dok-0.1.9/sparse_dok.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1705 2023-07-08 01:13:31.000000 sparse_dok-0.1.9/sparse_dok.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-08 01:13:31.000000 sparse_dok-0.1.9/sparse_dok.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       31 2023-07-08 01:13:31.000000 sparse_dok-0.1.9/sparse_dok.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-07-08 01:13:31.000000 sparse_dok-0.1.9/sparse_dok.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-08 01:13:32.163100 sparse_dok-0.1.9/tests/
--rw-rw-rw-   0        0        0     2616 2022-11-13 00:44:01.000000 sparse_dok-0.1.9/tests/test_remove.py
--rw-rw-rw-   0        0        0     1587 2022-11-12 19:56:37.000000 sparse_dok-0.1.9/tests/test_reshape.py
--rw-rw-rw-   0        0        0     1490 2022-11-12 16:31:01.000000 sparse_dok-0.1.9/tests/test_sparse_dok_methods.py
--rw-rw-rw-   0        0        0     3121 2022-12-06 12:53:47.000000 sparse_dok-0.1.9/tests/test_spget.py
+drwxrwxrwx   0        0        0        0 2023-07-08 01:15:09.581873 sparse_dok-0.1.9.1/
+-rw-rw-rw-   0        0        0     1088 2023-07-08 01:12:38.000000 sparse_dok-0.1.9.1/LICENCE
+-rw-rw-rw-   0        0        0       39 2022-06-03 19:13:32.000000 sparse_dok-0.1.9.1/MANIFEST.in
+-rw-rw-rw-   0        0        0      956 2023-07-08 01:15:09.580873 sparse_dok-0.1.9.1/PKG-INFO
+-rw-rw-rw-   0        0        0     8731 2023-07-08 01:12:38.000000 sparse_dok-0.1.9.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-08 01:15:09.581873 sparse_dok-0.1.9.1/setup.cfg
+-rw-rw-rw-   0        0        0     1303 2023-07-08 01:14:44.000000 sparse_dok-0.1.9.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-08 01:15:09.526366 sparse_dok-0.1.9.1/sparse_dok/
+-rw-rw-rw-   0        0        0       95 2023-07-08 01:11:28.000000 sparse_dok-0.1.9.1/sparse_dok/__init__.py
+-rw-rw-rw-   0        0        0       23 2023-07-08 01:15:04.000000 sparse_dok-0.1.9.1/sparse_dok/__version__.py
+drwxrwxrwx   0        0        0        0 2023-07-08 01:15:09.543365 sparse_dok-0.1.9.1/sparse_dok/components/
+-rw-rw-rw-   0        0        0       98 2022-06-03 18:42:54.000000 sparse_dok-0.1.9.1/sparse_dok/components/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-08 01:15:09.576873 sparse_dok-0.1.9.1/sparse_dok/components/cuda/
+-rw-rw-rw-   0        0        0        0 2022-05-23 01:01:14.000000 sparse_dok-0.1.9.1/sparse_dok/components/cuda/__init__.py
+-rw-rw-rw-   0        0        0     2878 2022-05-30 20:40:04.000000 sparse_dok-0.1.9.1/sparse_dok/components/cuda/binary_search.cu
+-rw-rw-rw-   0        0        0    18343 2022-05-24 15:02:58.000000 sparse_dok-0.1.9.1/sparse_dok/components/cuda/bitonic.cu
+-rw-rw-rw-   0        0        0    14628 2022-05-23 01:50:08.000000 sparse_dok-0.1.9.1/sparse_dok/components/cuda/bmm_helpers.cu
+-rw-rw-rw-   0        0        0     6398 2022-11-15 22:41:58.000000 sparse_dok-0.1.9.1/sparse_dok/components/cuda/closed_hashmap_impl.cu
+-rw-rw-rw-   0        0        0     9899 2022-12-05 14:46:18.000000 sparse_dok-0.1.9.1/sparse_dok/components/cuda/closed_hashmap_impl.py
+-rw-rw-rw-   0        0        0    18328 2022-11-20 15:11:16.000000 sparse_dok-0.1.9.1/sparse_dok/components/cuda/closed_hashmap_impl_class.cu
+-rw-rw-rw-   0        0        0    38155 2023-07-08 01:15:08.000000 sparse_dok-0.1.9.1/sparse_dok/components/cuda/closed_hashmap_impl_preview.cu
+-rw-rw-rw-   0        0        0     6776 2022-11-19 20:13:52.000000 sparse_dok-0.1.9.1/sparse_dok/components/cuda/cuda_kernel.py
+-rw-rw-rw-   0        0        0     1362 2022-11-11 22:10:53.000000 sparse_dok-0.1.9.1/sparse_dok/components/cuda/filtered_elementwise.py
+-rw-rw-rw-   0        0        0     6711 2022-05-25 17:47:18.000000 sparse_dok-0.1.9.1/sparse_dok/components/cuda/hashmap.cu
+-rw-rw-rw-   0        0        0     4028 2022-12-05 13:56:04.000000 sparse_dok-0.1.9.1/sparse_dok/components/cuda/head.cu
+-rw-rw-rw-   0        0        0    35905 2022-11-17 22:43:16.000000 sparse_dok-0.1.9.1/sparse_dok/components/cuda/preview.cu
+-rw-rw-rw-   0        0        0     3417 2022-11-15 23:20:13.000000 sparse_dok-0.1.9.1/sparse_dok/components/cuda/reduce.cu
+-rw-rw-rw-   0        0        0    15548 2022-12-06 13:06:16.000000 sparse_dok-0.1.9.1/sparse_dok/components/cuda/safe_closed_hashmap_impl_class.cu
+-rw-rw-rw-   0        0        0     7944 2022-05-31 14:14:10.000000 sparse_dok-0.1.9.1/sparse_dok/components/cuda/smem_hashmap.cu
+-rw-rw-rw-   0        0        0     7903 2022-05-29 01:53:58.000000 sparse_dok-0.1.9.1/sparse_dok/components/cuda/smem_hashmap_simple.cu
+-rw-rw-rw-   0        0        0     9395 2022-11-13 23:05:51.000000 sparse_dok-0.1.9.1/sparse_dok/components/cuda/smem_tensor.cu
+-rw-rw-rw-   0        0        0    10707 2022-11-20 14:28:17.000000 sparse_dok-0.1.9.1/sparse_dok/components/cuda/sparse_dok_tensor_impl.cu
+-rw-rw-rw-   0        0        0    25049 2022-12-06 13:06:44.000000 sparse_dok-0.1.9.1/sparse_dok/components/cuda/sparse_dok_tensor_impl.py
+-rw-rw-rw-   0        0        0    52037 2023-07-08 01:15:09.000000 sparse_dok-0.1.9.1/sparse_dok/components/cuda/sparse_dok_tensor_impl_preview.cu
+-rw-rw-rw-   0        0        0     1541 2022-05-24 20:22:36.000000 sparse_dok-0.1.9.1/sparse_dok/components/cuda/stack.cu
+-rw-rw-rw-   0        0        0     6152 2022-11-20 23:38:59.000000 sparse_dok-0.1.9.1/sparse_dok/components/cuda/tensor_accessor.cu
+-rw-rw-rw-   0        0        0    11198 2022-06-03 18:56:52.000000 sparse_dok-0.1.9.1/sparse_dok/components/cuda/topkspspcsim.cu
+-rw-rw-rw-   0        0        0    10190 2022-11-11 21:44:22.000000 sparse_dok-0.1.9.1/sparse_dok/components/cuda/topkspspcsim.py
+-rw-rw-rw-   0        0        0     1161 2022-11-17 22:40:56.000000 sparse_dok-0.1.9.1/sparse_dok/components/cuda_callable.py
+-rw-rw-rw-   0        0        0    15308 2022-11-19 20:01:57.000000 sparse_dok-0.1.9.1/sparse_dok/components/cuda_closed_hashmap.py
+-rw-rw-rw-   0        0        0    17858 2022-11-20 00:15:06.000000 sparse_dok-0.1.9.1/sparse_dok/components/sparse_dok_tensor.py
+-rw-rw-rw-   0        0        0     6264 2022-11-11 21:43:04.000000 sparse_dok-0.1.9.1/sparse_dok/functions.py
+-rw-rw-rw-   0        0        0    10849 2022-11-19 19:06:50.000000 sparse_dok-0.1.9.1/sparse_dok/util.py
+drwxrwxrwx   0        0        0        0 2023-07-08 01:15:09.540367 sparse_dok-0.1.9.1/sparse_dok.egg-info/
+-rw-rw-rw-   0        0        0      956 2023-07-08 01:15:09.000000 sparse_dok-0.1.9.1/sparse_dok.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1705 2023-07-08 01:15:09.000000 sparse_dok-0.1.9.1/sparse_dok.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-08 01:15:09.000000 sparse_dok-0.1.9.1/sparse_dok.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       26 2023-07-08 01:15:09.000000 sparse_dok-0.1.9.1/sparse_dok.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-07-08 01:15:09.000000 sparse_dok-0.1.9.1/sparse_dok.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-08 01:15:09.579874 sparse_dok-0.1.9.1/tests/
+-rw-rw-rw-   0        0        0     2616 2022-11-13 00:44:01.000000 sparse_dok-0.1.9.1/tests/test_remove.py
+-rw-rw-rw-   0        0        0     1587 2022-11-12 19:56:37.000000 sparse_dok-0.1.9.1/tests/test_reshape.py
+-rw-rw-rw-   0        0        0     1490 2022-11-12 16:31:01.000000 sparse_dok-0.1.9.1/tests/test_sparse_dok_methods.py
+-rw-rw-rw-   0        0        0     3121 2022-12-06 12:53:47.000000 sparse_dok-0.1.9.1/tests/test_spget.py
```

### Comparing `sparse_dok-0.1.9/LICENCE` & `sparse_dok-0.1.9.1/LICENCE`

 * *Files identical despite different names*

### Comparing `sparse_dok-0.1.9/PKG-INFO` & `sparse_dok-0.1.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: sparse_dok
-Version: 0.1.9
+Version: 0.1.9.1
 Summary: sparse dok tensor implementation
 Home-page: https://github.com/DeMoriarty/SparseDOK
-Download-URL: https://github.com/DeMoriarty/SparseDOK/archive/v_019.tar.gz
+Download-URL: https://github.com/DeMoriarty/SparseDOK/archive/v_0191.tar.gz
 Author: demoriarty
 Author-email: sahbanjan@gmail.com
 License: MIT
 Keywords: pytorch,sparse
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `sparse_dok-0.1.9/README.md` & `sparse_dok-0.1.9.1/README.md`

 * *Files identical despite different names*

### Comparing `sparse_dok-0.1.9/setup.py` & `sparse_dok-0.1.9.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
   url = 'https://github.com/DeMoriarty/SparseDOK',
   download_url = f'https://github.com/DeMoriarty/SparseDOK/archive/v_{__version__.replace(".", "")}.tar.gz',
   keywords = ['pytorch', "sparse"],
   install_requires=[ 
     'numpy',
     'torch>=1.10.0',
     'sympy',
-    'cupy',
+    # 'cupy',
   ],
   classifiers=[
     'Development Status :: 3 - Alpha',
     'Intended Audience :: Developers',
     'Topic :: Software Development :: Build Tools',
     'License :: OSI Approved :: MIT License',
     'Programming Language :: Python :: 3',
```

### Comparing `sparse_dok-0.1.9/sparse_dok/components/cuda/binary_search.cu` & `sparse_dok-0.1.9.1/sparse_dok/components/cuda/binary_search.cu`

 * *Files identical despite different names*

### Comparing `sparse_dok-0.1.9/sparse_dok/components/cuda/bitonic.cu` & `sparse_dok-0.1.9.1/sparse_dok/components/cuda/bitonic.cu`

 * *Files identical despite different names*

### Comparing `sparse_dok-0.1.9/sparse_dok/components/cuda/bmm_helpers.cu` & `sparse_dok-0.1.9.1/sparse_dok/components/cuda/bmm_helpers.cu`

 * *Files identical despite different names*

### Comparing `sparse_dok-0.1.9/sparse_dok/components/cuda/closed_hashmap_impl.cu` & `sparse_dok-0.1.9.1/sparse_dok/components/cuda/closed_hashmap_impl.cu`

 * *Files identical despite different names*

### Comparing `sparse_dok-0.1.9/sparse_dok/components/cuda/closed_hashmap_impl.py` & `sparse_dok-0.1.9.1/sparse_dok/components/cuda/closed_hashmap_impl.py`

 * *Files identical despite different names*

### Comparing `sparse_dok-0.1.9/sparse_dok/components/cuda/closed_hashmap_impl_class.cu` & `sparse_dok-0.1.9.1/sparse_dok/components/cuda/closed_hashmap_impl_class.cu`

 * *Files identical despite different names*

### Comparing `sparse_dok-0.1.9/sparse_dok/components/cuda/closed_hashmap_impl_preview.cu` & `sparse_dok-0.1.9.1/sparse_dok/components/cuda/closed_hashmap_impl_preview.cu`

 * *Files identical despite different names*

### Comparing `sparse_dok-0.1.9/sparse_dok/components/cuda/cuda_kernel.py` & `sparse_dok-0.1.9.1/sparse_dok/components/cuda/cuda_kernel.py`

 * *Files identical despite different names*

### Comparing `sparse_dok-0.1.9/sparse_dok/components/cuda/filtered_elementwise.py` & `sparse_dok-0.1.9.1/sparse_dok/components/cuda/filtered_elementwise.py`

 * *Files identical despite different names*

### Comparing `sparse_dok-0.1.9/sparse_dok/components/cuda/hashmap.cu` & `sparse_dok-0.1.9.1/sparse_dok/components/cuda/hashmap.cu`

 * *Files identical despite different names*

### Comparing `sparse_dok-0.1.9/sparse_dok/components/cuda/head.cu` & `sparse_dok-0.1.9.1/sparse_dok/components/cuda/head.cu`

 * *Files identical despite different names*

### Comparing `sparse_dok-0.1.9/sparse_dok/components/cuda/preview.cu` & `sparse_dok-0.1.9.1/sparse_dok/components/cuda/preview.cu`

 * *Files identical despite different names*

### Comparing `sparse_dok-0.1.9/sparse_dok/components/cuda/reduce.cu` & `sparse_dok-0.1.9.1/sparse_dok/components/cuda/reduce.cu`

 * *Files identical despite different names*

### Comparing `sparse_dok-0.1.9/sparse_dok/components/cuda/safe_closed_hashmap_impl_class.cu` & `sparse_dok-0.1.9.1/sparse_dok/components/cuda/safe_closed_hashmap_impl_class.cu`

 * *Files identical despite different names*

### Comparing `sparse_dok-0.1.9/sparse_dok/components/cuda/smem_hashmap.cu` & `sparse_dok-0.1.9.1/sparse_dok/components/cuda/smem_hashmap.cu`

 * *Files identical despite different names*

### Comparing `sparse_dok-0.1.9/sparse_dok/components/cuda/smem_hashmap_simple.cu` & `sparse_dok-0.1.9.1/sparse_dok/components/cuda/smem_hashmap_simple.cu`

 * *Files identical despite different names*

### Comparing `sparse_dok-0.1.9/sparse_dok/components/cuda/smem_tensor.cu` & `sparse_dok-0.1.9.1/sparse_dok/components/cuda/smem_tensor.cu`

 * *Files identical despite different names*

### Comparing `sparse_dok-0.1.9/sparse_dok/components/cuda/sparse_dok_tensor_impl.cu` & `sparse_dok-0.1.9.1/sparse_dok/components/cuda/sparse_dok_tensor_impl.cu`

 * *Files identical despite different names*

### Comparing `sparse_dok-0.1.9/sparse_dok/components/cuda/sparse_dok_tensor_impl.py` & `sparse_dok-0.1.9.1/sparse_dok/components/cuda/sparse_dok_tensor_impl.py`

 * *Files identical despite different names*

### Comparing `sparse_dok-0.1.9/sparse_dok/components/cuda/sparse_dok_tensor_impl_preview.cu` & `sparse_dok-0.1.9.1/sparse_dok/components/cuda/sparse_dok_tensor_impl_preview.cu`

 * *Files identical despite different names*

### Comparing `sparse_dok-0.1.9/sparse_dok/components/cuda/stack.cu` & `sparse_dok-0.1.9.1/sparse_dok/components/cuda/stack.cu`

 * *Files identical despite different names*

### Comparing `sparse_dok-0.1.9/sparse_dok/components/cuda/tensor_accessor.cu` & `sparse_dok-0.1.9.1/sparse_dok/components/cuda/tensor_accessor.cu`

 * *Files identical despite different names*

### Comparing `sparse_dok-0.1.9/sparse_dok/components/cuda/topkspspcsim.cu` & `sparse_dok-0.1.9.1/sparse_dok/components/cuda/topkspspcsim.cu`

 * *Files identical despite different names*

### Comparing `sparse_dok-0.1.9/sparse_dok/components/cuda/topkspspcsim.py` & `sparse_dok-0.1.9.1/sparse_dok/components/cuda/topkspspcsim.py`

 * *Files identical despite different names*

### Comparing `sparse_dok-0.1.9/sparse_dok/components/cuda_callable.py` & `sparse_dok-0.1.9.1/sparse_dok/components/cuda_callable.py`

 * *Files identical despite different names*

### Comparing `sparse_dok-0.1.9/sparse_dok/components/cuda_closed_hashmap.py` & `sparse_dok-0.1.9.1/sparse_dok/components/cuda_closed_hashmap.py`

 * *Files identical despite different names*

### Comparing `sparse_dok-0.1.9/sparse_dok/components/sparse_dok_tensor.py` & `sparse_dok-0.1.9.1/sparse_dok/components/sparse_dok_tensor.py`

 * *Files identical despite different names*

### Comparing `sparse_dok-0.1.9/sparse_dok/functions.py` & `sparse_dok-0.1.9.1/sparse_dok/functions.py`

 * *Files identical despite different names*

### Comparing `sparse_dok-0.1.9/sparse_dok/util.py` & `sparse_dok-0.1.9.1/sparse_dok/util.py`

 * *Files identical despite different names*

### Comparing `sparse_dok-0.1.9/sparse_dok.egg-info/PKG-INFO` & `sparse_dok-0.1.9.1/sparse_dok.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: sparse-dok
-Version: 0.1.9
+Version: 0.1.9.1
 Summary: sparse dok tensor implementation
 Home-page: https://github.com/DeMoriarty/SparseDOK
-Download-URL: https://github.com/DeMoriarty/SparseDOK/archive/v_019.tar.gz
+Download-URL: https://github.com/DeMoriarty/SparseDOK/archive/v_0191.tar.gz
 Author: demoriarty
 Author-email: sahbanjan@gmail.com
 License: MIT
 Keywords: pytorch,sparse
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `sparse_dok-0.1.9/sparse_dok.egg-info/SOURCES.txt` & `sparse_dok-0.1.9.1/sparse_dok.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sparse_dok-0.1.9/tests/test_remove.py` & `sparse_dok-0.1.9.1/tests/test_remove.py`

 * *Files identical despite different names*

### Comparing `sparse_dok-0.1.9/tests/test_reshape.py` & `sparse_dok-0.1.9.1/tests/test_reshape.py`

 * *Files identical despite different names*

### Comparing `sparse_dok-0.1.9/tests/test_sparse_dok_methods.py` & `sparse_dok-0.1.9.1/tests/test_sparse_dok_methods.py`

 * *Files identical despite different names*

### Comparing `sparse_dok-0.1.9/tests/test_spget.py` & `sparse_dok-0.1.9.1/tests/test_spget.py`

 * *Files identical despite different names*

