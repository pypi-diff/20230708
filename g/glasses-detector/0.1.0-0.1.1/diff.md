# Comparing `tmp/glasses-detector-0.1.0.tar.gz` & `tmp/glasses-detector-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "glasses-detector-0.1.0.tar", last modified: Sat Jul  8 08:06:07 2023, max compression
+gzip compressed data, was "glasses-detector-0.1.1.tar", last modified: Sat Jul  8 08:27:38 2023, max compression
```

## Comparing `glasses-detector-0.1.0.tar` & `glasses-detector-0.1.1.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 08:06:07.885175 glasses-detector-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-08 08:05:53.000000 glasses-detector-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    17400 2023-07-08 08:06:07.885175 glasses-detector-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    23559 2023-07-08 08:05:53.000000 glasses-detector-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 08:06:07.885175 glasses-detector-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)    18070 2023-07-08 08:05:53.000000 glasses-detector-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 08:06:07.881175 glasses-detector-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 08:06:07.885175 glasses-detector-0.1.0/src/glasses_detector/
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-07-08 08:05:53.000000 glasses-detector-0.1.0/src/glasses_detector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6991 2023-07-08 08:05:53.000000 glasses-detector-0.1.0/src/glasses_detector/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 08:06:07.885175 glasses-detector-0.1.0/src/glasses_detector/_data/
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-07-08 08:05:53.000000 glasses-detector-0.1.0/src/glasses_detector/_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2127 2023-07-08 08:05:53.000000 glasses-detector-0.1.0/src/glasses_detector/_data/classification_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     4349 2023-07-08 08:05:53.000000 glasses-detector-0.1.0/src/glasses_detector/_data/mixins.py
--rw-r--r--   0 runner    (1001) docker     (123)     3010 2023-07-08 08:05:53.000000 glasses-detector-0.1.0/src/glasses_detector/_data/segmentation_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 08:06:07.885175 glasses-detector-0.1.0/src/glasses_detector/_wrappers/
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-08 08:05:53.000000 glasses-detector-0.1.0/src/glasses_detector/_wrappers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2796 2023-07-08 08:05:53.000000 glasses-detector-0.1.0/src/glasses_detector/_wrappers/binary_classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-07-08 08:05:53.000000 glasses-detector-0.1.0/src/glasses_detector/_wrappers/binary_segmenter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 08:06:07.885175 glasses-detector-0.1.0/src/glasses_detector/bases/
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-07-08 08:05:53.000000 glasses-detector-0.1.0/src/glasses_detector/bases/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10335 2023-07-08 08:05:53.000000 glasses-detector-0.1.0/src/glasses_detector/bases/base_classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)    13532 2023-07-08 08:05:53.000000 glasses-detector-0.1.0/src/glasses_detector/bases/base_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    16613 2023-07-08 08:05:53.000000 glasses-detector-0.1.0/src/glasses_detector/bases/base_segmenter.py
--rw-r--r--   0 runner    (1001) docker     (123)     8670 2023-07-08 08:05:53.000000 glasses-detector-0.1.0/src/glasses_detector/classifiers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 08:06:07.885175 glasses-detector-0.1.0/src/glasses_detector/models/
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-08 08:05:53.000000 glasses-detector-0.1.0/src/glasses_detector/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1994 2023-07-08 08:05:53.000000 glasses-detector-0.1.0/src/glasses_detector/models/tiny_binary_classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     3989 2023-07-08 08:05:53.000000 glasses-detector-0.1.0/src/glasses_detector/models/tiny_binary_segmenter.py
--rw-r--r--   0 runner    (1001) docker     (123)    19049 2023-07-08 08:05:53.000000 glasses-detector-0.1.0/src/glasses_detector/segmenters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 08:06:07.885175 glasses-detector-0.1.0/src/glasses_detector.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17400 2023-07-08 08:06:07.000000 glasses-detector-0.1.0/src/glasses_detector.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-08 08:06:07.000000 glasses-detector-0.1.0/src/glasses_detector.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 08:06:07.000000 glasses-detector-0.1.0/src/glasses_detector.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-08 08:06:07.000000 glasses-detector-0.1.0/src/glasses_detector.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 08:06:07.000000 glasses-detector-0.1.0/src/glasses_detector.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-08 08:06:07.000000 glasses-detector-0.1.0/src/glasses_detector.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 08:27:38.440733 glasses-detector-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-08 08:27:27.000000 glasses-detector-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    17410 2023-07-08 08:27:38.440733 glasses-detector-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    23588 2023-07-08 08:27:27.000000 glasses-detector-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 08:27:38.440733 glasses-detector-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)    18080 2023-07-08 08:27:27.000000 glasses-detector-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 08:27:38.432732 glasses-detector-0.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 08:27:38.432732 glasses-detector-0.1.1/src/glasses_detector/
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-07-08 08:27:27.000000 glasses-detector-0.1.1/src/glasses_detector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6991 2023-07-08 08:27:27.000000 glasses-detector-0.1.1/src/glasses_detector/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 08:27:38.436732 glasses-detector-0.1.1/src/glasses_detector/_data/
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-07-08 08:27:27.000000 glasses-detector-0.1.1/src/glasses_detector/_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2127 2023-07-08 08:27:27.000000 glasses-detector-0.1.1/src/glasses_detector/_data/classification_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4349 2023-07-08 08:27:27.000000 glasses-detector-0.1.1/src/glasses_detector/_data/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3010 2023-07-08 08:27:27.000000 glasses-detector-0.1.1/src/glasses_detector/_data/segmentation_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 08:27:38.436732 glasses-detector-0.1.1/src/glasses_detector/_wrappers/
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-08 08:27:27.000000 glasses-detector-0.1.1/src/glasses_detector/_wrappers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2796 2023-07-08 08:27:27.000000 glasses-detector-0.1.1/src/glasses_detector/_wrappers/binary_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-07-08 08:27:27.000000 glasses-detector-0.1.1/src/glasses_detector/_wrappers/binary_segmenter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 08:27:38.436732 glasses-detector-0.1.1/src/glasses_detector/bases/
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-07-08 08:27:27.000000 glasses-detector-0.1.1/src/glasses_detector/bases/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10336 2023-07-08 08:27:27.000000 glasses-detector-0.1.1/src/glasses_detector/bases/base_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13532 2023-07-08 08:27:27.000000 glasses-detector-0.1.1/src/glasses_detector/bases/base_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16614 2023-07-08 08:27:27.000000 glasses-detector-0.1.1/src/glasses_detector/bases/base_segmenter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8670 2023-07-08 08:27:27.000000 glasses-detector-0.1.1/src/glasses_detector/classifiers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 08:27:38.440733 glasses-detector-0.1.1/src/glasses_detector/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-08 08:27:27.000000 glasses-detector-0.1.1/src/glasses_detector/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1994 2023-07-08 08:27:27.000000 glasses-detector-0.1.1/src/glasses_detector/models/tiny_binary_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3989 2023-07-08 08:27:27.000000 glasses-detector-0.1.1/src/glasses_detector/models/tiny_binary_segmenter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19049 2023-07-08 08:27:27.000000 glasses-detector-0.1.1/src/glasses_detector/segmenters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 08:27:38.436732 glasses-detector-0.1.1/src/glasses_detector.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17410 2023-07-08 08:27:38.000000 glasses-detector-0.1.1/src/glasses_detector.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-08 08:27:38.000000 glasses-detector-0.1.1/src/glasses_detector.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 08:27:38.000000 glasses-detector-0.1.1/src/glasses_detector.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-08 08:27:38.000000 glasses-detector-0.1.1/src/glasses_detector.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 08:27:38.000000 glasses-detector-0.1.1/src/glasses_detector.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-08 08:27:38.000000 glasses-detector-0.1.1/src/glasses_detector.egg-info/top_level.txt
```

### Comparing `glasses-detector-0.1.0/LICENSE` & `glasses-detector-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `glasses-detector-0.1.0/PKG-INFO` & `glasses-detector-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glasses-detector
-Version: 0.1.0
+Version: 0.1.1
 Summary: Eyeglasses and sunglasses detector (classifier and segmenter)
 Home-page: https://github.com/mantasu/glasses-detector
 Author: Mantas Birškus
 Author-email: mantix7@gmail.com
 License: MIT
 Project-URL: Documentation, https://mantasu.github.io/glasses-detector
 Project-URL: Bug Tracker, https://github.com/mantasu/glasses-detector/issues
@@ -24,15 +24,15 @@
 
 # Glasses Detector
 
 [![PyPI](https://img.shields.io/pypi/v/glasses-detector?color=orange)](https://pypi.org/project/glasses-detector/)
 [![Python](https://img.shields.io/badge/python-3.10%20|%203.11-yellow)](https://docs.python.org/3/)
 [![CUDA: yes](https://img.shields.io/badge/cuda-yes-green)](https://developer.nvidia.com/cuda-toolkit)
 [![Docs: passing](https://img.shields.io/badge/docs-passing-skyblue)](https://mantasu.github.io/glasses-detector/)
-[![DOI](https://zenodo.org/badge/TODO.svg)](https://zenodo.org/badge/latestdoi/TODO)
+[![DOI](https://zenodo.org/badge/610509640.svg)](https://zenodo.org/badge/latestdoi/610509640)
 [![License: MIT](https://img.shields.io/badge/license-MIT-lightgrey.svg)](https://opensource.org/licenses/MIT)
 
 **Eyeglasses** and **sunglasses** _classifier_ + **glasses** and their **frames** _segmenter_. This project provides a quick way to use the pre-trained models via python script or terminal. Based on selected task, an image or a directory of images will be processed and corresponding labels or masks will be generated.
 
 > **Note**: the project is BETA stage. Currently, only sunglasses classification models (except _huge_) and full glasses segmentation models (except _medium_) are available.
 
 ## Installation
```

### Comparing `glasses-detector-0.1.0/README.md` & `glasses-detector-0.1.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Glasses Detector
 
 [![PyPI](https://img.shields.io/pypi/v/glasses-detector?color=orange)](https://pypi.org/project/glasses-detector/)
 [![Python](https://img.shields.io/badge/python-3.10%20|%203.11-yellow)](https://docs.python.org/3/)
 [![CUDA: yes](https://img.shields.io/badge/cuda-yes-green)](https://developer.nvidia.com/cuda-toolkit)
 [![Docs: passing](https://img.shields.io/badge/docs-passing-skyblue)](https://mantasu.github.io/glasses-detector/)
-[![DOI](https://zenodo.org/badge/TODO.svg)](https://zenodo.org/badge/latestdoi/TODO)
+[![DOI](https://zenodo.org/badge/610509640.svg)](https://zenodo.org/badge/latestdoi/610509640)
 [![License: MIT](https://img.shields.io/badge/license-MIT-lightgrey.svg)](https://opensource.org/licenses/MIT)
 
 **Eyeglasses** and **sunglasses** _classifier_ + **glasses** and their **frames** _segmenter_. This project provides scripts to download the corresponding datasets, train the corresponding models and by itself is a PyPi project that provides a quick way to use the trained models via python script or terminal.
 
 > **Note**: the project is BETA stage. Currently, only full-glasses base segmentation models are provided.
 
 ## Installation
@@ -390,10 +390,10 @@
 @misc{glasses-detector,
   author = {Mantas Birškus},
   title = {Glasses Detector},
   year = {2023},
   publisher = {GitHub},
   journal = {GitHub repository},
   howpublished = {\url{https://github.com/mantasu/glasses-detector}},
-  doi = {TBA}
+  doi = {10.5281/zenodo.8126101}
 }
 ```
```

### Comparing `glasses-detector-0.1.0/setup.py` & `glasses-detector-0.1.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 DESCRIPTION = r"""
 # Glasses Detector
 
 [![PyPI](https://img.shields.io/pypi/v/glasses-detector?color=orange)](https://pypi.org/project/glasses-detector/)
 [![Python](https://img.shields.io/badge/python-3.10%20|%203.11-yellow)](https://docs.python.org/3/)
 [![CUDA: yes](https://img.shields.io/badge/cuda-yes-green)](https://developer.nvidia.com/cuda-toolkit)
 [![Docs: passing](https://img.shields.io/badge/docs-passing-skyblue)](https://mantasu.github.io/glasses-detector/)
-[![DOI](https://zenodo.org/badge/TODO.svg)](https://zenodo.org/badge/latestdoi/TODO)
+[![DOI](https://zenodo.org/badge/610509640.svg)](https://zenodo.org/badge/latestdoi/610509640)
 [![License: MIT](https://img.shields.io/badge/license-MIT-lightgrey.svg)](https://opensource.org/licenses/MIT)
 
 **Eyeglasses** and **sunglasses** _classifier_ + **glasses** and their **frames** _segmenter_. This project provides a quick way to use the pre-trained models via python script or terminal. Based on selected task, an image or a directory of images will be processed and corresponding labels or masks will be generated.
 
 > **Note**: the project is BETA stage. Currently, only sunglasses classification models (except _huge_) and full glasses segmentation models (except _medium_) are available.
 
 ## Installation
@@ -210,15 +210,15 @@
   doi = {TBA}
 }
 ```
 """
 
 setuptools.setup(
     name = "glasses-detector",
-    version = "0.1.0",
+    version = "0.1.1",
     author = "Mantas Birškus",
     author_email = "mantix7@gmail.com",
     license = "MIT",
     description = f"Eyeglasses and sunglasses detector (classifier and segmenter)",
     long_description = DESCRIPTION,
     long_description_content_type = "text/markdown",
     url = "https://github.com/mantasu/glasses-detector",
```

### Comparing `glasses-detector-0.1.0/src/glasses_detector/__main__.py` & `glasses-detector-0.1.1/src/glasses_detector/__main__.py`

 * *Files identical despite different names*

### Comparing `glasses-detector-0.1.0/src/glasses_detector/_data/classification_dataset.py` & `glasses-detector-0.1.1/src/glasses_detector/_data/classification_dataset.py`

 * *Files identical despite different names*

### Comparing `glasses-detector-0.1.0/src/glasses_detector/_data/mixins.py` & `glasses-detector-0.1.1/src/glasses_detector/_data/mixins.py`

 * *Files identical despite different names*

### Comparing `glasses-detector-0.1.0/src/glasses_detector/_data/segmentation_dataset.py` & `glasses-detector-0.1.1/src/glasses_detector/_data/segmentation_dataset.py`

 * *Files identical despite different names*

### Comparing `glasses-detector-0.1.0/src/glasses_detector/_wrappers/binary_classifier.py` & `glasses-detector-0.1.1/src/glasses_detector/_wrappers/binary_classifier.py`

 * *Files identical despite different names*

### Comparing `glasses-detector-0.1.0/src/glasses_detector/_wrappers/binary_segmenter.py` & `glasses-detector-0.1.1/src/glasses_detector/_wrappers/binary_segmenter.py`

 * *Files identical despite different names*

### Comparing `glasses-detector-0.1.0/src/glasses_detector/bases/base_classifier.py` & `glasses-detector-0.1.1/src/glasses_detector/bases/base_classifier.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,15 +51,15 @@
         classification models can be downloaded. To specify a custom 
         abbreviation map, use ``abbrev_map`` argument when instantiating 
         an object and either provide an empty dictionary or a custom one.
     """
     
     VERSION_MAP = {
         "eyeglasses_classifier": None, 
-        "sunglasses_classifier": "0.1.0"
+        "sunglasses_classifier": "v0.1.0"
     }
     """
     dict[str, str]: A dictionary mapping from the possible pretrained 
         classification model kinds, e.g., "eyeglasses", "sunglasses", 
         to their corresponding GitHub release versions, e.g., "v1.0.0" 
         (where the newest weights are stored). This can be customized 
         via ``version_map`` argument as well, e.g., if other versions
```

### Comparing `glasses-detector-0.1.0/src/glasses_detector/bases/base_model.py` & `glasses-detector-0.1.1/src/glasses_detector/bases/base_model.py`

 * *Files identical despite different names*

### Comparing `glasses-detector-0.1.0/src/glasses_detector/bases/base_segmenter.py` & `glasses-detector-0.1.1/src/glasses_detector/bases/base_segmenter.py`

 * *Files 0% similar despite different names*

```diff
@@ -67,15 +67,15 @@
         map, based on which pretrained weights for some kinds of 
         segmentation models can be downloaded. To specify a custom 
         abbreviation map, use ``abbrev_map`` argument when instantiating 
         an object and either provide an empty dictionary or a custom one.
     """
 
     VERSION_MAP = {
-        "full_glasses_segmenter": "0.1.0",
+        "full_glasses_segmenter": "v0.1.0",
         "glass_frames_segmenter": None,
     }
     """
     dict[str, str]: A dictionary mapping from the possible pretrained 
         segmentation model kinds, e.g., "full glasses", "glass frames", 
         to their corresponding GitHub release versions, e.g., "v1.0.0" 
         (where the newest weights are stored). This can be customized
```

### Comparing `glasses-detector-0.1.0/src/glasses_detector/classifiers.py` & `glasses-detector-0.1.1/src/glasses_detector/classifiers.py`

 * *Files identical despite different names*

### Comparing `glasses-detector-0.1.0/src/glasses_detector/models/tiny_binary_classifier.py` & `glasses-detector-0.1.1/src/glasses_detector/models/tiny_binary_classifier.py`

 * *Files identical despite different names*

### Comparing `glasses-detector-0.1.0/src/glasses_detector/models/tiny_binary_segmenter.py` & `glasses-detector-0.1.1/src/glasses_detector/models/tiny_binary_segmenter.py`

 * *Files identical despite different names*

### Comparing `glasses-detector-0.1.0/src/glasses_detector/segmenters.py` & `glasses-detector-0.1.1/src/glasses_detector/segmenters.py`

 * *Files identical despite different names*

### Comparing `glasses-detector-0.1.0/src/glasses_detector.egg-info/PKG-INFO` & `glasses-detector-0.1.1/src/glasses_detector.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glasses-detector
-Version: 0.1.0
+Version: 0.1.1
 Summary: Eyeglasses and sunglasses detector (classifier and segmenter)
 Home-page: https://github.com/mantasu/glasses-detector
 Author: Mantas Birškus
 Author-email: mantix7@gmail.com
 License: MIT
 Project-URL: Documentation, https://mantasu.github.io/glasses-detector
 Project-URL: Bug Tracker, https://github.com/mantasu/glasses-detector/issues
@@ -24,15 +24,15 @@
 
 # Glasses Detector
 
 [![PyPI](https://img.shields.io/pypi/v/glasses-detector?color=orange)](https://pypi.org/project/glasses-detector/)
 [![Python](https://img.shields.io/badge/python-3.10%20|%203.11-yellow)](https://docs.python.org/3/)
 [![CUDA: yes](https://img.shields.io/badge/cuda-yes-green)](https://developer.nvidia.com/cuda-toolkit)
 [![Docs: passing](https://img.shields.io/badge/docs-passing-skyblue)](https://mantasu.github.io/glasses-detector/)
-[![DOI](https://zenodo.org/badge/TODO.svg)](https://zenodo.org/badge/latestdoi/TODO)
+[![DOI](https://zenodo.org/badge/610509640.svg)](https://zenodo.org/badge/latestdoi/610509640)
 [![License: MIT](https://img.shields.io/badge/license-MIT-lightgrey.svg)](https://opensource.org/licenses/MIT)
 
 **Eyeglasses** and **sunglasses** _classifier_ + **glasses** and their **frames** _segmenter_. This project provides a quick way to use the pre-trained models via python script or terminal. Based on selected task, an image or a directory of images will be processed and corresponding labels or masks will be generated.
 
 > **Note**: the project is BETA stage. Currently, only sunglasses classification models (except _huge_) and full glasses segmentation models (except _medium_) are available.
 
 ## Installation
```

### Comparing `glasses-detector-0.1.0/src/glasses_detector.egg-info/SOURCES.txt` & `glasses-detector-0.1.1/src/glasses_detector.egg-info/SOURCES.txt`

 * *Files identical despite different names*

