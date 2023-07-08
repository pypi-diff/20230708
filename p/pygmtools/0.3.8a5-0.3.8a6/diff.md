# Comparing `tmp/pygmtools-0.3.8a5.tar.gz` & `tmp/pygmtools-0.3.8a6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygmtools-0.3.8a5.tar", last modified: Fri Jul  7 17:10:52 2023, max compression
+gzip compressed data, was "pygmtools-0.3.8a6.tar", last modified: Fri Jul  7 17:30:17 2023, max compression
```

## Comparing `pygmtools-0.3.8a5.tar` & `pygmtools-0.3.8a6.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxrwxrwx   0        0        0        0 2023-07-07 17:10:52.193519 pygmtools-0.3.8a5/
--rw-rw-rw-   0        0        0      508 2023-05-03 08:07:01.000000 pygmtools-0.3.8a5/LICENSE
--rw-rw-rw-   0        0        0    13827 2023-07-07 17:10:52.193519 pygmtools-0.3.8a5/PKG-INFO
--rw-rw-rw-   0        0        0    12718 2023-05-03 08:07:01.000000 pygmtools-0.3.8a5/README.md
-drwxrwxrwx   0        0        0        0 2023-07-07 17:10:52.182234 pygmtools-0.3.8a5/pygmtools/
--rw-rw-rw-   0        0        0     2120 2023-07-07 16:55:51.000000 pygmtools-0.3.8a5/pygmtools/__init__.py
--rw-rw-rw-   0        0        0    27000 2023-07-07 11:54:30.000000 pygmtools-0.3.8a5/pygmtools/benchmark.py
--rw-rw-rw-   0        0        0    58666 2023-07-07 12:42:20.000000 pygmtools-0.3.8a5/pygmtools/classic_solvers.py
--rw-rw-rw-   0        0        0    59231 2023-07-07 11:54:30.000000 pygmtools-0.3.8a5/pygmtools/dataset.py
--rw-rw-rw-   0        0        0     3112 2023-07-07 11:54:30.000000 pygmtools-0.3.8a5/pygmtools/dataset_config.py
--rw-rw-rw-   0        0        0    58908 2023-07-07 11:54:30.000000 pygmtools-0.3.8a5/pygmtools/jittor_backend.py
--rw-rw-rw-   0        0        0    12371 2023-07-07 11:54:30.000000 pygmtools-0.3.8a5/pygmtools/jittor_modules.py
-drwxrwxrwx   0        0        0        0 2023-07-07 17:10:52.187364 pygmtools-0.3.8a5/pygmtools/lib/
--rw-rw-rw-   0        0        0  1138391 2023-07-02 08:40:47.000000 pygmtools-0.3.8a5/pygmtools/lib/a_star.tar.gz
--rw-rw-rw-   0        0        0  3203980 2023-07-02 08:39:54.000000 pygmtools-0.3.8a5/pygmtools/lib/a_star.zip
--rw-rw-rw-   0        0        0    77128 2023-07-07 11:54:30.000000 pygmtools-0.3.8a5/pygmtools/linear_solvers.py
--rw-rw-rw-   0        0        0    21736 2023-07-07 11:54:30.000000 pygmtools-0.3.8a5/pygmtools/mindspore_backend.py
--rw-rw-rw-   0        0        0    44038 2023-07-07 11:54:30.000000 pygmtools-0.3.8a5/pygmtools/multi_graph_solvers.py
--rw-rw-rw-   0        0        0    70477 2023-07-07 11:54:30.000000 pygmtools-0.3.8a5/pygmtools/neural_solvers.py
--rw-rw-rw-   0        0        0    60669 2023-07-07 11:54:30.000000 pygmtools-0.3.8a5/pygmtools/numpy_backend.py
--rw-rw-rw-   0        0        0    15282 2023-07-07 11:54:30.000000 pygmtools-0.3.8a5/pygmtools/numpy_modules.py
--rw-rw-rw-   0        0        0    57860 2023-07-07 11:54:30.000000 pygmtools-0.3.8a5/pygmtools/paddle_backend.py
--rw-rw-rw-   0        0        0    11899 2023-07-07 11:54:30.000000 pygmtools-0.3.8a5/pygmtools/paddle_modules.py
--rw-rw-rw-   0        0        0    15443 2023-07-07 12:38:50.000000 pygmtools-0.3.8a5/pygmtools/pytorch_astar_modules.py
--rw-rw-rw-   0        0        0    74579 2023-07-07 12:56:18.000000 pygmtools-0.3.8a5/pygmtools/pytorch_backend.py
--rw-rw-rw-   0        0        0    12329 2023-07-07 11:54:30.000000 pygmtools-0.3.8a5/pygmtools/pytorch_modules.py
--rw-rw-rw-   0        0        0    23046 2023-07-07 11:54:30.000000 pygmtools-0.3.8a5/pygmtools/tensorflow_backend.py
--rw-rw-rw-   0        0        0      508 2023-07-07 11:54:30.000000 pygmtools-0.3.8a5/pygmtools/tensorflow_modules.py
--rw-rw-rw-   0        0        0    51707 2023-07-07 11:54:30.000000 pygmtools-0.3.8a5/pygmtools/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-07 17:10:52.184291 pygmtools-0.3.8a5/pygmtools.egg-info/
--rw-rw-rw-   0        0        0    13827 2023-07-07 17:10:52.000000 pygmtools-0.3.8a5/pygmtools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      982 2023-07-07 17:10:52.000000 pygmtools-0.3.8a5/pygmtools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-07 17:10:52.000000 pygmtools-0.3.8a5/pygmtools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      110 2023-07-07 17:10:52.000000 pygmtools-0.3.8a5/pygmtools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-07-07 17:10:52.000000 pygmtools-0.3.8a5/pygmtools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-07 17:10:52.194543 pygmtools-0.3.8a5/setup.cfg
--rw-rw-rw-   0        0        0     5922 2023-07-07 17:10:41.000000 pygmtools-0.3.8a5/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-07 17:10:52.192516 pygmtools-0.3.8a5/tests/
--rw-rw-rw-   0        0        0    16089 2023-07-02 10:34:16.000000 pygmtools-0.3.8a5/tests/test_classic_solvers.py
--rw-rw-rw-   0        0        0     5561 2023-05-03 08:07:01.000000 pygmtools-0.3.8a5/tests/test_dataset.py
--rw-rw-rw-   0        0        0     3800 2023-05-03 08:07:01.000000 pygmtools-0.3.8a5/tests/test_misc.py
--rw-rw-rw-   0        0        0    13302 2023-05-03 08:07:01.000000 pygmtools-0.3.8a5/tests/test_multi_graph_solvers.py
--rw-rw-rw-   0        0        0     9288 2023-05-03 08:07:01.000000 pygmtools-0.3.8a5/tests/test_neural_solvers.py
--rw-rw-rw-   0        0        0     1007 2023-05-03 08:07:01.000000 pygmtools-0.3.8a5/tests/test_utils.py
+drwxrwxrwx   0        0        0        0 2023-07-07 17:30:17.971159 pygmtools-0.3.8a6/
+-rw-rw-rw-   0        0        0      508 2023-05-03 08:07:01.000000 pygmtools-0.3.8a6/LICENSE
+-rw-rw-rw-   0        0        0    13827 2023-07-07 17:30:17.971159 pygmtools-0.3.8a6/PKG-INFO
+-rw-rw-rw-   0        0        0    12718 2023-05-03 08:07:01.000000 pygmtools-0.3.8a6/README.md
+drwxrwxrwx   0        0        0        0 2023-07-07 17:30:17.959634 pygmtools-0.3.8a6/pygmtools/
+-rw-rw-rw-   0        0        0     2120 2023-07-07 17:29:55.000000 pygmtools-0.3.8a6/pygmtools/__init__.py
+-rw-rw-rw-   0        0        0    27000 2023-07-07 11:54:30.000000 pygmtools-0.3.8a6/pygmtools/benchmark.py
+-rw-rw-rw-   0        0        0    58666 2023-07-07 12:42:20.000000 pygmtools-0.3.8a6/pygmtools/classic_solvers.py
+-rw-rw-rw-   0        0        0    59231 2023-07-07 11:54:30.000000 pygmtools-0.3.8a6/pygmtools/dataset.py
+-rw-rw-rw-   0        0        0     3112 2023-07-07 11:54:30.000000 pygmtools-0.3.8a6/pygmtools/dataset_config.py
+-rw-rw-rw-   0        0        0    58908 2023-07-07 11:54:30.000000 pygmtools-0.3.8a6/pygmtools/jittor_backend.py
+-rw-rw-rw-   0        0        0    12371 2023-07-07 11:54:30.000000 pygmtools-0.3.8a6/pygmtools/jittor_modules.py
+drwxrwxrwx   0        0        0        0 2023-07-07 17:30:17.964898 pygmtools-0.3.8a6/pygmtools/lib/
+-rw-rw-rw-   0        0        0  1138391 2023-07-02 08:40:47.000000 pygmtools-0.3.8a6/pygmtools/lib/a_star.tar.gz
+-rw-rw-rw-   0        0        0  3203980 2023-07-02 08:39:54.000000 pygmtools-0.3.8a6/pygmtools/lib/a_star.zip
+-rw-rw-rw-   0        0        0    77128 2023-07-07 11:54:30.000000 pygmtools-0.3.8a6/pygmtools/linear_solvers.py
+-rw-rw-rw-   0        0        0    21736 2023-07-07 11:54:30.000000 pygmtools-0.3.8a6/pygmtools/mindspore_backend.py
+-rw-rw-rw-   0        0        0    44038 2023-07-07 11:54:30.000000 pygmtools-0.3.8a6/pygmtools/multi_graph_solvers.py
+-rw-rw-rw-   0        0        0    70477 2023-07-07 11:54:30.000000 pygmtools-0.3.8a6/pygmtools/neural_solvers.py
+-rw-rw-rw-   0        0        0    60669 2023-07-07 11:54:30.000000 pygmtools-0.3.8a6/pygmtools/numpy_backend.py
+-rw-rw-rw-   0        0        0    15282 2023-07-07 11:54:30.000000 pygmtools-0.3.8a6/pygmtools/numpy_modules.py
+-rw-rw-rw-   0        0        0    57860 2023-07-07 11:54:30.000000 pygmtools-0.3.8a6/pygmtools/paddle_backend.py
+-rw-rw-rw-   0        0        0    11899 2023-07-07 11:54:30.000000 pygmtools-0.3.8a6/pygmtools/paddle_modules.py
+-rw-rw-rw-   0        0        0    15443 2023-07-07 12:38:50.000000 pygmtools-0.3.8a6/pygmtools/pytorch_astar_modules.py
+-rw-rw-rw-   0        0        0    74579 2023-07-07 12:56:18.000000 pygmtools-0.3.8a6/pygmtools/pytorch_backend.py
+-rw-rw-rw-   0        0        0    12329 2023-07-07 11:54:30.000000 pygmtools-0.3.8a6/pygmtools/pytorch_modules.py
+-rw-rw-rw-   0        0        0    23046 2023-07-07 11:54:30.000000 pygmtools-0.3.8a6/pygmtools/tensorflow_backend.py
+-rw-rw-rw-   0        0        0      508 2023-07-07 11:54:30.000000 pygmtools-0.3.8a6/pygmtools/tensorflow_modules.py
+-rw-rw-rw-   0        0        0    51707 2023-07-07 11:54:30.000000 pygmtools-0.3.8a6/pygmtools/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-07 17:30:17.962713 pygmtools-0.3.8a6/pygmtools.egg-info/
+-rw-rw-rw-   0        0        0    13827 2023-07-07 17:30:17.000000 pygmtools-0.3.8a6/pygmtools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      982 2023-07-07 17:30:17.000000 pygmtools-0.3.8a6/pygmtools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-07 17:30:17.000000 pygmtools-0.3.8a6/pygmtools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      110 2023-07-07 17:30:17.000000 pygmtools-0.3.8a6/pygmtools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-07 17:30:17.000000 pygmtools-0.3.8a6/pygmtools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-07 17:30:17.971159 pygmtools-0.3.8a6/setup.cfg
+-rw-rw-rw-   0        0        0     5916 2023-07-07 17:29:39.000000 pygmtools-0.3.8a6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-07 17:30:17.970138 pygmtools-0.3.8a6/tests/
+-rw-rw-rw-   0        0        0    16089 2023-07-02 10:34:16.000000 pygmtools-0.3.8a6/tests/test_classic_solvers.py
+-rw-rw-rw-   0        0        0     5561 2023-05-03 08:07:01.000000 pygmtools-0.3.8a6/tests/test_dataset.py
+-rw-rw-rw-   0        0        0     3800 2023-05-03 08:07:01.000000 pygmtools-0.3.8a6/tests/test_misc.py
+-rw-rw-rw-   0        0        0    13302 2023-05-03 08:07:01.000000 pygmtools-0.3.8a6/tests/test_multi_graph_solvers.py
+-rw-rw-rw-   0        0        0     9288 2023-05-03 08:07:01.000000 pygmtools-0.3.8a6/tests/test_neural_solvers.py
+-rw-rw-rw-   0        0        0     1007 2023-05-03 08:07:01.000000 pygmtools-0.3.8a6/tests/test_utils.py
```

### Comparing `pygmtools-0.3.8a5/PKG-INFO` & `pygmtools-0.3.8a6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygmtools
-Version: 0.3.8a5
+Version: 0.3.8a6
 Summary: pygmtools provides graph matching solvers in Python API and supports numpy and pytorch backends. pygmtools also provides dataset API for standard graph matching benchmarks.
 Home-page: https://pygmtools.readthedocs.io/
 Author: ThinkLab at SJTU
 License: Mulan PSL v2
 Classifier: License :: OSI Approved :: Mulan Permissive Software License v2 (MulanPSL-2.0)
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Operating System :: OS Independent
```

### Comparing `pygmtools-0.3.8a5/README.md` & `pygmtools-0.3.8a6/README.md`

 * *Files identical despite different names*

### Comparing `pygmtools-0.3.8a5/pygmtools/__init__.py` & `pygmtools-0.3.8a6/pygmtools/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from .benchmark import Benchmark
 from .linear_solvers import sinkhorn, hungarian
 from .classic_solvers import rrwm, sm, ipfp, a_star
 from .multi_graph_solvers import cao, mgm_floyd, gamgm
 from .neural_solvers import pca_gm, ipca_gm, cie, ngm
 import pygmtools.utils as utils
 BACKEND = 'numpy'
-__version__ = '0.3.8-alpha5'
+__version__ = '0.3.8-alpha6'
 __author__ = 'ThinkLab at SJTU'
 
 
 def env_report():
     """
     Print environment report
     """
```

### Comparing `pygmtools-0.3.8a5/pygmtools/benchmark.py` & `pygmtools-0.3.8a6/pygmtools/benchmark.py`

 * *Files identical despite different names*

### Comparing `pygmtools-0.3.8a5/pygmtools/classic_solvers.py` & `pygmtools-0.3.8a6/pygmtools/classic_solvers.py`

 * *Files identical despite different names*

### Comparing `pygmtools-0.3.8a5/pygmtools/dataset.py` & `pygmtools-0.3.8a6/pygmtools/dataset.py`

 * *Files identical despite different names*

### Comparing `pygmtools-0.3.8a5/pygmtools/dataset_config.py` & `pygmtools-0.3.8a6/pygmtools/dataset_config.py`

 * *Files identical despite different names*

### Comparing `pygmtools-0.3.8a5/pygmtools/jittor_backend.py` & `pygmtools-0.3.8a6/pygmtools/jittor_backend.py`

 * *Files identical despite different names*

### Comparing `pygmtools-0.3.8a5/pygmtools/jittor_modules.py` & `pygmtools-0.3.8a6/pygmtools/jittor_modules.py`

 * *Files identical despite different names*

### Comparing `pygmtools-0.3.8a5/pygmtools/lib/a_star.tar.gz` & `pygmtools-0.3.8a6/pygmtools/lib/a_star.tar.gz`

 * *Files identical despite different names*

### Comparing `pygmtools-0.3.8a5/pygmtools/lib/a_star.zip` & `pygmtools-0.3.8a6/pygmtools/lib/a_star.zip`

 * *Files identical despite different names*

### Comparing `pygmtools-0.3.8a5/pygmtools/linear_solvers.py` & `pygmtools-0.3.8a6/pygmtools/linear_solvers.py`

 * *Files identical despite different names*

### Comparing `pygmtools-0.3.8a5/pygmtools/mindspore_backend.py` & `pygmtools-0.3.8a6/pygmtools/mindspore_backend.py`

 * *Files identical despite different names*

### Comparing `pygmtools-0.3.8a5/pygmtools/multi_graph_solvers.py` & `pygmtools-0.3.8a6/pygmtools/multi_graph_solvers.py`

 * *Files identical despite different names*

### Comparing `pygmtools-0.3.8a5/pygmtools/neural_solvers.py` & `pygmtools-0.3.8a6/pygmtools/neural_solvers.py`

 * *Files identical despite different names*

### Comparing `pygmtools-0.3.8a5/pygmtools/numpy_backend.py` & `pygmtools-0.3.8a6/pygmtools/numpy_backend.py`

 * *Files identical despite different names*

### Comparing `pygmtools-0.3.8a5/pygmtools/numpy_modules.py` & `pygmtools-0.3.8a6/pygmtools/numpy_modules.py`

 * *Files identical despite different names*

### Comparing `pygmtools-0.3.8a5/pygmtools/paddle_backend.py` & `pygmtools-0.3.8a6/pygmtools/paddle_backend.py`

 * *Files identical despite different names*

### Comparing `pygmtools-0.3.8a5/pygmtools/paddle_modules.py` & `pygmtools-0.3.8a6/pygmtools/paddle_modules.py`

 * *Files identical despite different names*

### Comparing `pygmtools-0.3.8a5/pygmtools/pytorch_astar_modules.py` & `pygmtools-0.3.8a6/pygmtools/pytorch_astar_modules.py`

 * *Files identical despite different names*

### Comparing `pygmtools-0.3.8a5/pygmtools/pytorch_backend.py` & `pygmtools-0.3.8a6/pygmtools/pytorch_backend.py`

 * *Files identical despite different names*

### Comparing `pygmtools-0.3.8a5/pygmtools/pytorch_modules.py` & `pygmtools-0.3.8a6/pygmtools/pytorch_modules.py`

 * *Files identical despite different names*

### Comparing `pygmtools-0.3.8a5/pygmtools/tensorflow_backend.py` & `pygmtools-0.3.8a6/pygmtools/tensorflow_backend.py`

 * *Files identical despite different names*

### Comparing `pygmtools-0.3.8a5/pygmtools/utils.py` & `pygmtools-0.3.8a6/pygmtools/utils.py`

 * *Files identical despite different names*

### Comparing `pygmtools-0.3.8a5/pygmtools.egg-info/PKG-INFO` & `pygmtools-0.3.8a6/pygmtools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygmtools
-Version: 0.3.8a5
+Version: 0.3.8a6
 Summary: pygmtools provides graph matching solvers in Python API and supports numpy and pytorch backends. pygmtools also provides dataset API for standard graph matching benchmarks.
 Home-page: https://pygmtools.readthedocs.io/
 Author: ThinkLab at SJTU
 License: Mulan PSL v2
 Classifier: License :: OSI Approved :: Mulan Permissive Software License v2 (MulanPSL-2.0)
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Operating System :: OS Independent
```

### Comparing `pygmtools-0.3.8a5/pygmtools.egg-info/SOURCES.txt` & `pygmtools-0.3.8a6/pygmtools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pygmtools-0.3.8a5/setup.py` & `pygmtools-0.3.8a6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     system = platform.system()
     python_version = ".".join(map(str, sys.version_info[:2]))
     if system.lower() == "windows":
         os_version = "windows"
     elif system.lower() == "darwin":
         os_version = "macos"
     elif system.lower() == "linux":
-        os_version = distro.linux_distribution(full_distribution_name=False)[0].lower()
+        os_version = distro.name().lower()
     else:
         raise ValueError("Unknown System")
     if (os_version == 'windows'):
         if (python_version == '3.11'):
             python_version = '3.10'
     else:
         if (python_version == '3.10') or (python_version == '3.11'):
@@ -95,15 +95,15 @@
                             '3.9':'a_star.cpython-39-x86_64-linux-gnu.so'}}
     dynamic_link = filename[os_version][python_version]
     if not os.path.exists(os.path.join(NAME,dynamic_link)):
         if os_version == 'windows':
             unzip_file(os.path.join(NAME,'lib/a_star.zip'),os.path.join(NAME,'lib'))
         else:
             untar_file(os.path.join(NAME,'lib/a_star.tar.gz'),os.path.join(NAME,'lib'))
-        shutil.copy2(dynamic_link, NAME)
+        shutil.copy2(os.path.join(NAME,os.path.join('lib',dynamic_link)), NAME)
 
 class UploadCommand(Command):
     """Support setup.py upload."""
 
     description = 'Build and publish the package.'
     user_options = []
```

### Comparing `pygmtools-0.3.8a5/tests/test_classic_solvers.py` & `pygmtools-0.3.8a6/tests/test_classic_solvers.py`

 * *Files identical despite different names*

### Comparing `pygmtools-0.3.8a5/tests/test_dataset.py` & `pygmtools-0.3.8a6/tests/test_dataset.py`

 * *Files identical despite different names*

### Comparing `pygmtools-0.3.8a5/tests/test_misc.py` & `pygmtools-0.3.8a6/tests/test_misc.py`

 * *Files identical despite different names*

### Comparing `pygmtools-0.3.8a5/tests/test_multi_graph_solvers.py` & `pygmtools-0.3.8a6/tests/test_multi_graph_solvers.py`

 * *Files identical despite different names*

### Comparing `pygmtools-0.3.8a5/tests/test_neural_solvers.py` & `pygmtools-0.3.8a6/tests/test_neural_solvers.py`

 * *Files identical despite different names*

### Comparing `pygmtools-0.3.8a5/tests/test_utils.py` & `pygmtools-0.3.8a6/tests/test_utils.py`

 * *Files identical despite different names*

