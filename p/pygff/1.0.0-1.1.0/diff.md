# Comparing `tmp/pygff-1.0.0.tar.gz` & `tmp/pygff-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygff-1.0.0.tar", last modified: Fri Aug 12 17:29:12 2022, max compression
+gzip compressed data, was "pygff-1.1.0.tar", last modified: Sat Jul  8 18:06:19 2023, max compression
```

## Comparing `pygff-1.0.0.tar` & `pygff-1.1.0.tar`

### file list

```diff
@@ -1,19 +1,23 @@
-drwxrwxrwx   0        0        0        0 2022-08-12 17:29:12.277925 pygff-1.0.0/
--rw-rw-rw-   0        0        0     1090 2022-06-02 08:09:31.000000 pygff-1.0.0/LICENSE
--rw-rw-rw-   0        0        0     3216 2022-08-12 17:29:12.277925 pygff-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     2662 2022-08-12 17:13:03.000000 pygff-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2022-08-12 17:29:12.266928 pygff-1.0.0/pygff/
--rw-rw-rw-   0        0        0     6162 2022-08-12 17:06:33.000000 pygff-1.0.0/pygff/GFF.py
--rw-rw-rw-   0        0        0       89 2022-06-28 20:30:20.000000 pygff-1.0.0/pygff/__init__.py
--rw-rw-rw-   0        0        0     1851 2022-06-28 20:30:20.000000 pygff-1.0.0/pygff/_util.py
--rw-rw-rw-   0        0        0    13321 2022-08-12 17:26:02.000000 pygff-1.0.0/pygff/load.py
--rw-rw-rw-   0        0        0    10752 2022-08-12 17:26:54.000000 pygff-1.0.0/pygff/save.py
-drwxrwxrwx   0        0        0        0 2022-08-12 17:29:12.276924 pygff-1.0.0/pygff.egg-info/
--rw-rw-rw-   0        0        0     3216 2022-08-12 17:29:12.000000 pygff-1.0.0/pygff.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      269 2022-08-12 17:29:12.000000 pygff-1.0.0/pygff.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-08-12 17:29:12.000000 pygff-1.0.0/pygff.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       28 2022-08-12 17:29:12.000000 pygff-1.0.0/pygff.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2022-08-12 17:29:12.000000 pygff-1.0.0/pygff.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      101 2022-07-18 10:13:50.000000 pygff-1.0.0/pyproject.toml
--rw-rw-rw-   0        0        0      676 2022-08-12 17:29:12.278924 pygff-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      176 2022-07-18 10:13:22.000000 pygff-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-08 18:06:19.494035 pygff-1.1.0/
+-rw-rw-rw-   0        0        0     1090 2022-06-02 08:09:31.000000 pygff-1.1.0/LICENSE
+-rw-rw-rw-   0        0        0     4353 2023-07-08 18:06:19.494035 pygff-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3791 2023-07-08 18:02:39.000000 pygff-1.1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-08 18:06:19.475034 pygff-1.1.0/pygff/
+-rw-rw-rw-   0        0        0     8378 2023-06-27 11:46:47.000000 pygff-1.1.0/pygff/GFF.py
+-rw-rw-rw-   0        0        0       89 2022-06-28 20:30:20.000000 pygff-1.1.0/pygff/__init__.py
+-rw-rw-rw-   0        0        0     1851 2022-06-28 20:30:20.000000 pygff-1.1.0/pygff/_util.py
+-rw-rw-rw-   0        0        0    13294 2023-06-21 14:45:36.000000 pygff-1.1.0/pygff/load.py
+-rw-rw-rw-   0        0        0    11314 2023-06-27 10:49:44.000000 pygff-1.1.0/pygff/save.py
+drwxrwxrwx   0        0        0        0 2023-07-08 18:06:19.486034 pygff-1.1.0/pygff.egg-info/
+-rw-rw-rw-   0        0        0     4353 2023-07-08 18:06:19.000000 pygff-1.1.0/pygff.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      330 2023-07-08 18:06:19.000000 pygff-1.1.0/pygff.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-08 18:06:19.000000 pygff-1.1.0/pygff.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       28 2023-07-08 18:06:19.000000 pygff-1.1.0/pygff.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-07-08 18:06:19.000000 pygff-1.1.0/pygff.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      101 2022-07-18 10:13:50.000000 pygff-1.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0      684 2023-07-08 18:06:19.496032 pygff-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      176 2022-07-18 10:13:22.000000 pygff-1.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-08 18:06:19.492033 pygff-1.1.0/tests/
+-rw-rw-rw-   0        0        0      724 2023-06-27 09:24:49.000000 pygff-1.1.0/tests/test_load.py
+-rw-rw-rw-   0        0        0      856 2023-06-27 08:53:06.000000 pygff-1.1.0/tests/test_metadata.py
+-rw-rw-rw-   0        0        0     2088 2023-06-27 11:42:02.000000 pygff-1.1.0/tests/test_save.py
```

### Comparing `pygff-1.0.0/LICENSE` & `pygff-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pygff-1.0.0/PKG-INFO` & `pygff-1.1.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,64 +1,92 @@
-Metadata-Version: 2.1
-Name: pygff
-Version: 1.0.0
-Summary: A package to read and write Grace Format files (.gff)
-Home-page: https://bitbucket.org/felixgremse/gff_file_format/src/master/
-Author: Gremse-IT GmbH
-Author-email: info@gremse-it.de
-Maintainer: Nicholas Book
-Maintainer-email: nbook@gremse-it.com
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # PyGFF
 ---
-A Python package to read and write Grace Format Files (*.gff*).
+A Python package to read and write Grace Format files (*.gff / .segff*).
 
-## Easiest way to install PyGFF:
-`pip install pygff`
+## Easiest way to install PyGFF
+---
+```bash
+$ pip install pygff
+```
 
-## Basic usage:
-1. Loading a *.gff* file:
-	```
-	from pygff import load
-	data = load('image.gff')
+## Basic usage
+---
+- Loading a *.gff* file:
+	```python
+	>>> from pygff import load
+	>>> data = load("image.gff")
 	```
-2. Saving a numpy array `np_arr` as a *.gff* file:
+- Saving a numpy ndarray `np_array` as a *.gff* file:
+	```python
+	>>> from pygff import GFF, save
+	>>> save("image.gff", GFF(np_arr))
 	```
-	from pygff import GFF, save
-	save('image.gff', GFF(np_arr))
+- Saving a numpy array `seg_array` as a *.segff* (segmentation) file with class names, indices, and colors:
+	```python
+	>>> from pygff import GFF, save
+	>>> segff = GFF(seg_array)
+	>>> segff.info.set_class_dict(
+        {"Heart": {"index": 1, "color": (255, 0, 0, 255)},
+          "Liver": {"index": 2, "color": (0, 255, 0, 255)}})
+	>>> save("segmentation.segff", segff)
 	```
+	Note that `seg_array` is converted to `np.uint8` before saving. Colors are specified as RGBA, and class index 0 is reserved for "unclassified" data.
+
+## Tutorials
+---
+Tutorial notebooks can be found in the `/tutorials/` directory of [this](https://bitbucket.org/felixgremse/gff_file_format/src/master/) repository. They are not included with the PyGFF package. We recommed that you to start with `01_load_and_save.ipynb` to learn more about loading, saving, and GFF objects. More tutorials will be added in the future.
+
+Running the examples requires the packages `jupyter`, `matplotlib`, `numpy`, and `scipy` to be installed. Also, please download the required example datasets if you have not cloned the repository yet.
 
 ## What is GFF?
-GFF is an open source file format for multimodal biomedical images. The format supports datasets with up to five dimensions (three spatial dimensions, time-variant, and multi-channel) and a rich set of metadata key-value pairs. By default, the implementation uses a lossless compression algorithm to reduce file size and cryptographic hashing for secure writing. Multithreading is also used if possible to speed up reading and writing of *.gff* files.
+---
+GFF is an open source file format for multimodal biomedical images (*.gff*) and segmentations (*.segff*). The format supports datasets with up to five dimensions (three spatial dimensions, time-variant, and multi-channel) and a rich set of metadata key-value pairs. By default, the implementation uses a lossless compression algorithm to reduce file size and cryptographic hashing for secure writing. Multithreading is also used if possible to speed up reading and writing of GFF files.
 
-The PyGFF package is developed by [Gremse-IT GmbH](https://gremse-it.com/) (Aachen, Germany) as a Python interface for [Imalytics Preclinical 3.0](https://gremse-it.com/imalytics-preclinical/) which utilizes *.gff* by default for underlay, overlay, segmentation, and project files. 
+The PyGFF package is developed by [Gremse-IT GmbH](https://gremse-it.com/) (Aachen, Germany) as a Python interface for [Imalytics Preclinical 3.0](https://gremse-it.com/imalytics-preclinical/) which utilizes *.gff* by default for underlay, overlay, segmentation (*.segff*), and project files (*.imaproj*). 
 
-For more details, please check out this publication:
+For more details, please refer to this publication:
 
 > Yamoah, Grace Gyamfuah et al. “Data Curation for Preclinical and Clinical Multimodal Imaging Studies.” 
 > Molecular imaging and biology vol. 21,6 (2019): 1034-1043. doi:10.1007/s11307-019-01339-0
 
 Full text: https://pubmed.ncbi.nlm.nih.gov/30868426/
 
-## How to build the package yourself:
-1. Clone the repository: `git clone git@bitbucket.org:felixgremse/gff_file_format.git`
-2. Make sure you have the Python build package installed: `py -m pip install --upgrade build`
-3. Then, install `pygff` in editable mode using: `py -m pip install -e .`	
-
-## Examples:
-Example notebooks can be found in the `/examples/` directory of the repository. They are not included with the PyGFF package. We recommed that you to start with `01_load_and_save.ipynb` to learn more about loading, saving, and GFF objects. More tutorials will be added in the future.
-
-Running the examples requires the packages `jupyter`, `matplotlib`, `numpy`, and `scipy` to be installed. Also, please download the required example datasets if you have not cloned the repository yet.
-
-## How to run package tests:
-1. Go to the `./test/` directory and simply run `pytest`
+## How to build the package yourself
+---
+1. Clone the repository
+	```bash
+	$ git clone git@bitbucket.org:felixgremse/gff_file_format.git
+	```
+2. (Optional) Create a virtual environment, e.g. with `venv`
+	```bash
+	$ python -m venv env
+	...
+	$ source env/bin/activate
+	```
+	or using `conda`
+	```bash
+	$ conda env create --file environment.yml
+	...
+	$ conda activate pygff
+	```
+3. Then, install `pygff` in editable mode, e.g. using `build`
+	```bash
+	$ python -m pip install --upgrade build
+	...
+	$ python -m pip install -e .
+	```
+	or `conda-build`
+	```bash
+	$ conda develop .
+	```
+## How to run package tests
+---
+Make sure that `pytest` is installed and then simply call it from a shell in the main directory.
+```bash
+$ pytest
+```
 
-## License:
+## License
+---
 The PyGFF package is licensed under the terms of the [MIT license](https://opensource.org/licenses/MIT).
 
-All *.gff* files and Jupyter notebooks contained in the `/examples/` directory of the repository are licensed under [CC BY-NC-SA 4.0](https://creativecommons.org/licenses/by-nc-sa/4.0/legalcode).
+All *.gff* files, *.segff* files, and Jupyter notebooks contained in the `/tutorials/` directory of the repository are licensed under [CC BY-NC-SA 4.0](https://creativecommons.org/licenses/by-nc-sa/4.0/legalcode).
```

### Comparing `pygff-1.0.0/pygff/GFF.py` & `pygff-1.1.0/pygff/GFF.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from multiprocessing.sharedctypes import Value
 import numpy as np
 import copy
 
 __all__ = ["GFF", "StepInfo", "GFFInfo"]
 
 
 class StepInfo:
@@ -108,54 +107,110 @@
         """Returns a list of class names from the metadata."""
         try:
             proj_info = self.meta["Project info"]
             class_names = proj_info["ClassNames"]  # A|B|C...
             names_list = class_names.split("|")
             return names_list
         except KeyError:
-            print("No segmentation classes.")
-            return []
+            raise ValueError("No segmentation classes.")
 
     def get_class_indices(self):
         """Returns a list of class indices from the metadata."""
         try:
             proj_info = self.meta["Project info"]
             class_names = proj_info["ClassIndices"]
             ind_list = class_names.split("|")
             return [int(i) for i in ind_list]
         except KeyError:
-            print("No segmentation classes.")
-            return []
+            raise ValueError("No segmentation classes.")
 
     def get_class_colors(self):
         """Returns a list of class colors (rgba) from the metadata."""
         try:
             proj_info = self.meta["Project info"]
             class_names = proj_info["ClassColors"]
             col_list = class_names.split("|")  # b g r a
             new_list = []
             for c in col_list:
                 tmp = c.split(" ")
                 new_list.append((int(tmp[2]), int(tmp[1]), int(tmp[0]), int(tmp[3])))
             return new_list
 
         except KeyError:
-            print("No segmentation classes.")
-            return []
+            raise ValueError("No segmentation classes.")
 
     def get_class_dict(self):
         """Returns a dictionary with class names as keys and a dictionary of 'color' and 'index' as value."""
         class_dict = {}
-        names = self.get_class_names()
-        indices = self.get_class_indices()
-        colors = self.get_class_colors()
-
-        for i in range(len(names)):
-            class_dict[names[i]] = {"index": indices[i], "color": colors[i]}
-        return class_dict
+        try:
+            names = self.get_class_names()
+            indices = self.get_class_indices()
+            colors = self.get_class_colors()
+
+            for i in range(len(names)):
+                class_dict[names[i]] = {"index": indices[i], "color": colors[i]}
+            return class_dict
+
+        except:
+            raise ValueError("No segmentation classes.")
+
+    def __set_default_segmentation_dict(self):
+        if self.meta.get("Project info") is None:
+            self.meta["Project info"] = {
+                "ClassColors": "0 0 0 255",
+                "ClassIndices": "0",
+                "ClassNames": "unclassified",
+            }
+
+    def __add_class(
+        self, prof_dict: dict, class_name: str, class_color: tuple, class_index: int
+    ) -> None:
+        try:
+            prof_dict["ClassNames"] += "|" + str(class_name)
+            assert len(class_color) == 4
+            for c in class_color:
+                if not 0 <= c <= 255:
+                    raise ValueError(f"Class color values must be between 0 and 255.")
+            prof_dict["ClassColors"] += "|" + " ".join(
+                [
+                    str(class_color[2]),
+                    str(class_color[1]),
+                    str(class_color[0]),
+                    str(class_color[3]),
+                ]
+            )  # stored as BGRA
+            prof_dict["ClassIndices"] += "|" + str(class_index)
+        except:
+            raise ValueError("Invalid new class.")
+
+    def set_class_dict(self, class_dict: dict) -> None:
+        """Sets the class dictionary in the metadata.
+        Keys are class names and values are a nested dictionary of 'color' (RGBA) and 'index' (uchar) values.
+        """
+        try:
+            self.__set_default_segmentation_dict()
+
+            proj_info = self.meta["Project info"]
+
+            for k, v in class_dict.items():
+                self.__add_class(proj_info, str(k), v["color"], v["index"])
+        except:
+            raise ValueError("Invalid class dictionary.")
+
+    def add_class(self, new_class: dict) -> None:
+        """Adds a new class to the metadata dictionary.
+        Keys must be "name", "color", and "index".
+        """
+        try:
+            proj_info = self.meta["Project info"]
+        except KeyError:
+            print("No classes configured yet. Please use 'set_class_dict'.")
+        self.__add_class(
+            proj_info, new_class["name"], new_class["color"], new_class["index"]
+        )
 
 
 class GFF(np.ndarray):
     """Representation of a GFF dataset with associated metadata ("info")."""
 
     def __new__(cls, input_array=None, info=None):
         obj = (
@@ -171,7 +226,10 @@
             return
         self.info = getattr(obj, "info", GFFInfo())
 
     def __str__(self):
         return str(self.info) + "Dimensions: {shape}\nArray: {array}".format(
             shape=super().shape, array=super().__str__()
         )
+
+
+# TODO: introduce SEGFF subclass?
```

### Comparing `pygff-1.0.0/pygff/_util.py` & `pygff-1.1.0/pygff/_util.py`

 * *Files identical despite different names*

### Comparing `pygff-1.0.0/pygff/load.py` & `pygff-1.1.0/pygff/load.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from pygff import GFF, StepInfo, GFFInfo
-from py.path import local
 from struct import unpack
 import numpy as np
 import hashlib
 import multiprocessing as mp
 import threading
 import zlib
 import os
```

### Comparing `pygff-1.0.0/pygff/save.py` & `pygff-1.1.0/pygff/save.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,17 @@
-from pygff import GFF, StepInfo
 from struct import pack
 import numpy as np
 import hashlib
 import multiprocessing as mp
 import threading
 import zlib
+import pathlib
+from .GFF import GFF
+from os import PathLike
+from typing import Union
 
 from ._util import (
     __special_tag,
     __my_software_version,
     _voxel_type_id_to_type,
     _voxel_type_id_to_channel_number,
 )
@@ -94,19 +97,27 @@
         return self.ba
 
 
 def __get_header_bytes(gff):
     """Serialize information into wrapper, so we know how many bytes are stored therein."""
     header_bytes = ByteArrayWriteInterface()
 
-    shape = gff.shape
+    if not 0 < len(gff.shape) <= 5:
+        raise ValueError(
+            f"GFF shape ({gff.shape}) must be 1, 2, 3, 4, or 5 dimensional."
+        )
 
-    __save_int64(header_bytes, int(shape[0]))
-    __save_int64(header_bytes, int(shape[1]))
-    __save_int64(header_bytes, int(shape[2]))
+    if len(gff.shape) == 1:
+        gff.shape = (gff.shape[0], 1, 1)
+    elif len(gff.shape) == 2:
+        gff.shape = (gff.shape[0], gff.shape[1], 1)
+
+    __save_int64(header_bytes, int(gff.shape[0]))
+    __save_int64(header_bytes, int(gff.shape[1]))
+    __save_int64(header_bytes, int(gff.shape[2]))
 
     vX, vY, vZ = gff.info.voxel_sizes
 
     __save_double(header_bytes, float(vX))
     __save_double(header_bytes, float(vY))
     __save_double(header_bytes, float(vZ))
 
@@ -235,15 +246,14 @@
             memLevel=9,
             strategy=zlib.Z_DEFAULT_STRATEGY,
         )
         compressed = bytearray()
 
         chunk_size = 512**2
         for offset in range(0, len(bytes), chunk_size):
-
             rem = min(len(bytes) - offset, chunk_size)
 
             chunk = memoryview(bytes)[offset : offset + rem]
             compressed_chunk = compressor.compress(chunk)
             compressed.extend(compressed_chunk)
             hash.update(compressed_chunk)
 
@@ -352,15 +362,19 @@
     __save_uint64(bytes, len(file_digest))
     bytes.write(file_digest)
 
     # Signal nonexisting timestamp
     __save_string(bytes, "No Timestamp")
 
 
-def save(path_or_byteslike, gff):
-    """Saves a GFF object as a .gff file."""
+def save(path_or_byteslike: Union[str, bytes, PathLike], gff: GFF):
+    """Saves a GFF object as a .gff/.segff file."""
+
     write, tell = [getattr(path_or_byteslike, x, None) for x in ["write", "tell"]]
-    if callable(write) and callable(tell):
+    if callable(write) and callable(tell):  # bytes
         __save_bytes_like(path_or_byteslike, gff)
-    else:
+    else:  # filepath
+        if pathlib.Path(path_or_byteslike).suffix == ".segff":
+            gff.info.set_class_dict({})
+            gff = gff.astype(np.uint8)
         with open(path_or_byteslike, "wb") as f:
             __save_bytes_like(f, gff)
```

### Comparing `pygff-1.0.0/pygff.egg-info/PKG-INFO` & `pygff-1.1.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,64 +1,108 @@
 Metadata-Version: 2.1
 Name: pygff
-Version: 1.0.0
-Summary: A package to read and write Grace Format files (.gff)
+Version: 1.1.0
+Summary: A package to read and write Grace Format files (.gff/.segff)
 Home-page: https://bitbucket.org/felixgremse/gff_file_format/src/master/
 Author: Gremse-IT GmbH
-Author-email: info@gremse-it.de
+Author-email: info@gremse-it.com
 Maintainer: Nicholas Book
 Maintainer-email: nbook@gremse-it.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # PyGFF
 ---
-A Python package to read and write Grace Format Files (*.gff*).
+A Python package to read and write Grace Format files (*.gff / .segff*).
 
-## Easiest way to install PyGFF:
-`pip install pygff`
+## Easiest way to install PyGFF
+---
+```bash
+$ pip install pygff
+```
 
-## Basic usage:
-1. Loading a *.gff* file:
-	```
-	from pygff import load
-	data = load('image.gff')
+## Basic usage
+---
+- Loading a *.gff* file:
+	```python
+	>>> from pygff import load
+	>>> data = load("image.gff")
 	```
-2. Saving a numpy array `np_arr` as a *.gff* file:
+- Saving a numpy ndarray `np_array` as a *.gff* file:
+	```python
+	>>> from pygff import GFF, save
+	>>> save("image.gff", GFF(np_arr))
 	```
-	from pygff import GFF, save
-	save('image.gff', GFF(np_arr))
+- Saving a numpy array `seg_array` as a *.segff* (segmentation) file with class names, indices, and colors:
+	```python
+	>>> from pygff import GFF, save
+	>>> segff = GFF(seg_array)
+	>>> segff.info.set_class_dict(
+        {"Heart": {"index": 1, "color": (255, 0, 0, 255)},
+          "Liver": {"index": 2, "color": (0, 255, 0, 255)}})
+	>>> save("segmentation.segff", segff)
 	```
+	Note that `seg_array` is converted to `np.uint8` before saving. Colors are specified as RGBA, and class index 0 is reserved for "unclassified" data.
+
+## Tutorials
+---
+Tutorial notebooks can be found in the `/tutorials/` directory of [this](https://bitbucket.org/felixgremse/gff_file_format/src/master/) repository. They are not included with the PyGFF package. We recommed that you to start with `01_load_and_save.ipynb` to learn more about loading, saving, and GFF objects. More tutorials will be added in the future.
+
+Running the examples requires the packages `jupyter`, `matplotlib`, `numpy`, and `scipy` to be installed. Also, please download the required example datasets if you have not cloned the repository yet.
 
 ## What is GFF?
-GFF is an open source file format for multimodal biomedical images. The format supports datasets with up to five dimensions (three spatial dimensions, time-variant, and multi-channel) and a rich set of metadata key-value pairs. By default, the implementation uses a lossless compression algorithm to reduce file size and cryptographic hashing for secure writing. Multithreading is also used if possible to speed up reading and writing of *.gff* files.
+---
+GFF is an open source file format for multimodal biomedical images (*.gff*) and segmentations (*.segff*). The format supports datasets with up to five dimensions (three spatial dimensions, time-variant, and multi-channel) and a rich set of metadata key-value pairs. By default, the implementation uses a lossless compression algorithm to reduce file size and cryptographic hashing for secure writing. Multithreading is also used if possible to speed up reading and writing of GFF files.
 
-The PyGFF package is developed by [Gremse-IT GmbH](https://gremse-it.com/) (Aachen, Germany) as a Python interface for [Imalytics Preclinical 3.0](https://gremse-it.com/imalytics-preclinical/) which utilizes *.gff* by default for underlay, overlay, segmentation, and project files. 
+The PyGFF package is developed by [Gremse-IT GmbH](https://gremse-it.com/) (Aachen, Germany) as a Python interface for [Imalytics Preclinical 3.0](https://gremse-it.com/imalytics-preclinical/) which utilizes *.gff* by default for underlay, overlay, segmentation (*.segff*), and project files (*.imaproj*). 
 
-For more details, please check out this publication:
+For more details, please refer to this publication:
 
 > Yamoah, Grace Gyamfuah et al. “Data Curation for Preclinical and Clinical Multimodal Imaging Studies.” 
 > Molecular imaging and biology vol. 21,6 (2019): 1034-1043. doi:10.1007/s11307-019-01339-0
 
 Full text: https://pubmed.ncbi.nlm.nih.gov/30868426/
 
-## How to build the package yourself:
-1. Clone the repository: `git clone git@bitbucket.org:felixgremse/gff_file_format.git`
-2. Make sure you have the Python build package installed: `py -m pip install --upgrade build`
-3. Then, install `pygff` in editable mode using: `py -m pip install -e .`	
-
-## Examples:
-Example notebooks can be found in the `/examples/` directory of the repository. They are not included with the PyGFF package. We recommed that you to start with `01_load_and_save.ipynb` to learn more about loading, saving, and GFF objects. More tutorials will be added in the future.
-
-Running the examples requires the packages `jupyter`, `matplotlib`, `numpy`, and `scipy` to be installed. Also, please download the required example datasets if you have not cloned the repository yet.
-
-## How to run package tests:
-1. Go to the `./test/` directory and simply run `pytest`
+## How to build the package yourself
+---
+1. Clone the repository
+	```bash
+	$ git clone git@bitbucket.org:felixgremse/gff_file_format.git
+	```
+2. (Optional) Create a virtual environment, e.g. with `venv`
+	```bash
+	$ python -m venv env
+	...
+	$ source env/bin/activate
+	```
+	or using `conda`
+	```bash
+	$ conda env create --file environment.yml
+	...
+	$ conda activate pygff
+	```
+3. Then, install `pygff` in editable mode, e.g. using `build`
+	```bash
+	$ python -m pip install --upgrade build
+	...
+	$ python -m pip install -e .
+	```
+	or `conda-build`
+	```bash
+	$ conda develop .
+	```
+## How to run package tests
+---
+Make sure that `pytest` is installed and then simply call it from a shell in the main directory.
+```bash
+$ pytest
+```
 
-## License:
+## License
+---
 The PyGFF package is licensed under the terms of the [MIT license](https://opensource.org/licenses/MIT).
 
-All *.gff* files and Jupyter notebooks contained in the `/examples/` directory of the repository are licensed under [CC BY-NC-SA 4.0](https://creativecommons.org/licenses/by-nc-sa/4.0/legalcode).
+All *.gff* files, *.segff* files, and Jupyter notebooks contained in the `/tutorials/` directory of the repository are licensed under [CC BY-NC-SA 4.0](https://creativecommons.org/licenses/by-nc-sa/4.0/legalcode).
```

### Comparing `pygff-1.0.0/setup.cfg` & `pygff-1.1.0/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -1,43 +1,43 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2070 7967 6666 0d0a 7665 7273 696f   = pygff..versio
-00000020: 6e20 3d20 312e 302e 300d 0a61 7574 686f  n = 1.0.0..autho
+00000020: 6e20 3d20 312e 312e 300d 0a61 7574 686f  n = 1.1.0..autho
 00000030: 7220 3d20 4772 656d 7365 2d49 5420 476d  r = Gremse-IT Gm
 00000040: 6248 0d0a 6175 7468 6f72 5f65 6d61 696c  bH..author_email
 00000050: 203d 2069 6e66 6f40 6772 656d 7365 2d69   = info@gremse-i
-00000060: 742e 6465 0d0a 6d61 696e 7461 696e 6572  t.de..maintainer
-00000070: 203d 204e 6963 686f 6c61 7320 426f 6f6b   = Nicholas Book
-00000080: 0d0a 6d61 696e 7461 696e 6572 5f65 6d61  ..maintainer_ema
-00000090: 696c 203d 206e 626f 6f6b 4067 7265 6d73  il = nbook@grems
-000000a0: 652d 6974 2e63 6f6d 0d0a 6465 7363 7269  e-it.com..descri
-000000b0: 7074 696f 6e20 3d20 4120 7061 636b 6167  ption = A packag
-000000c0: 6520 746f 2072 6561 6420 616e 6420 7772  e to read and wr
-000000d0: 6974 6520 4772 6163 6520 466f 726d 6174  ite Grace Format
-000000e0: 2066 696c 6573 2028 2e67 6666 290d 0a6c   files (.gff)..l
-000000f0: 6f6e 675f 6465 7363 7269 7074 696f 6e20  ong_description 
-00000100: 3d20 6669 6c65 3a20 5245 4144 4d45 2e6d  = file: README.m
-00000110: 640d 0a6c 6f6e 675f 6465 7363 7269 7074  d..long_descript
-00000120: 696f 6e5f 636f 6e74 656e 745f 7479 7065  ion_content_type
-00000130: 203d 2074 6578 742f 6d61 726b 646f 776e   = text/markdown
-00000140: 0d0a 7572 6c20 3d20 6874 7470 733a 2f2f  ..url = https://
-00000150: 6269 7462 7563 6b65 742e 6f72 672f 6665  bitbucket.org/fe
-00000160: 6c69 7867 7265 6d73 652f 6766 665f 6669  lixgremse/gff_fi
-00000170: 6c65 5f66 6f72 6d61 742f 7372 632f 6d61  le_format/src/ma
-00000180: 7374 6572 2f0d 0a63 6c61 7373 6966 6965  ster/..classifie
-00000190: 7273 203d 200d 0a09 5072 6f67 7261 6d6d  rs = ...Programm
-000001a0: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
-000001b0: 5079 7468 6f6e 203a 3a20 330d 0a09 4c69  Python :: 3...Li
-000001c0: 6365 6e73 6520 3a3a 204f 5349 2041 7070  cense :: OSI App
-000001d0: 726f 7665 6420 3a3a 204d 4954 204c 6963  roved :: MIT Lic
-000001e0: 656e 7365 0d0a 094f 7065 7261 7469 6e67  ense...Operating
-000001f0: 2053 7973 7465 6d20 3a3a 204f 5320 496e   System :: OS In
-00000200: 6465 7065 6e64 656e 740d 0a0d 0a5b 6f70  dependent....[op
-00000210: 7469 6f6e 735d 0d0a 7061 636b 6167 6573  tions]..packages
-00000220: 203d 2070 7967 6666 0d0a 7079 7468 6f6e   = pygff..python
-00000230: 5f72 6571 7569 7265 7320 3d20 3e3d 332e  _requires = >=3.
-00000240: 360d 0a69 6e73 7461 6c6c 5f72 6571 7569  6..install_requi
-00000250: 7265 7320 3d20 0d0a 096e 756d 7079 3e3d  res = ...numpy>=
-00000260: 312e 3133 2e33 0d0a 0970 7974 6573 743e  1.13.3...pytest>
-00000270: 3d34 2e34 2e31 0d0a 0d0a 5b65 6767 5f69  =4.4.1....[egg_i
-00000280: 6e66 6f5d 0d0a 7461 675f 6275 696c 6420  nfo]..tag_build 
-00000290: 3d20 0d0a 7461 675f 6461 7465 203d 2030  = ..tag_date = 0
-000002a0: 0d0a 0d0a                                ....
+00000060: 742e 636f 6d0d 0a6d 6169 6e74 6169 6e65  t.com..maintaine
+00000070: 7220 3d20 4e69 6368 6f6c 6173 2042 6f6f  r = Nicholas Boo
+00000080: 6b0d 0a6d 6169 6e74 6169 6e65 725f 656d  k..maintainer_em
+00000090: 6169 6c20 3d20 6e62 6f6f 6b40 6772 656d  ail = nbook@grem
+000000a0: 7365 2d69 742e 636f 6d0d 0a64 6573 6372  se-it.com..descr
+000000b0: 6970 7469 6f6e 203d 2041 2070 6163 6b61  iption = A packa
+000000c0: 6765 2074 6f20 7265 6164 2061 6e64 2077  ge to read and w
+000000d0: 7269 7465 2047 7261 6365 2046 6f72 6d61  rite Grace Forma
+000000e0: 7420 6669 6c65 7320 282e 6766 662f 2e73  t files (.gff/.s
+000000f0: 6567 6666 290d 0a6c 6f6e 675f 6465 7363  egff)..long_desc
+00000100: 7269 7074 696f 6e20 3d20 6669 6c65 3a20  ription = file: 
+00000110: 5245 4144 4d45 2e6d 640d 0a6c 6f6e 675f  README.md..long_
+00000120: 6465 7363 7269 7074 696f 6e5f 636f 6e74  description_cont
+00000130: 656e 745f 7479 7065 203d 2074 6578 742f  ent_type = text/
+00000140: 6d61 726b 646f 776e 0d0a 7572 6c20 3d20  markdown..url = 
+00000150: 6874 7470 733a 2f2f 6269 7462 7563 6b65  https://bitbucke
+00000160: 742e 6f72 672f 6665 6c69 7867 7265 6d73  t.org/felixgrems
+00000170: 652f 6766 665f 6669 6c65 5f66 6f72 6d61  e/gff_file_forma
+00000180: 742f 7372 632f 6d61 7374 6572 2f0d 0a63  t/src/master/..c
+00000190: 6c61 7373 6966 6965 7273 203d 200d 0a09  lassifiers = ...
+000001a0: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
+000001b0: 7561 6765 203a 3a20 5079 7468 6f6e 203a  uage :: Python :
+000001c0: 3a20 330d 0a09 4c69 6365 6e73 6520 3a3a  : 3...License ::
+000001d0: 204f 5349 2041 7070 726f 7665 6420 3a3a   OSI Approved ::
+000001e0: 204d 4954 204c 6963 656e 7365 0d0a 094f   MIT License...O
+000001f0: 7065 7261 7469 6e67 2053 7973 7465 6d20  perating System 
+00000200: 3a3a 204f 5320 496e 6465 7065 6e64 656e  :: OS Independen
+00000210: 740d 0a0d 0a5b 6f70 7469 6f6e 735d 0d0a  t....[options]..
+00000220: 7061 636b 6167 6573 203d 2070 7967 6666  packages = pygff
+00000230: 0d0a 7079 7468 6f6e 5f72 6571 7569 7265  ..python_require
+00000240: 7320 3d20 3e3d 332e 360d 0a69 6e73 7461  s = >=3.6..insta
+00000250: 6c6c 5f72 6571 7569 7265 7320 3d20 0d0a  ll_requires = ..
+00000260: 096e 756d 7079 3e3d 312e 3133 2e33 0d0a  .numpy>=1.13.3..
+00000270: 0970 7974 6573 743e 3d34 2e34 2e31 0d0a  .pytest>=4.4.1..
+00000280: 0d0a 5b65 6767 5f69 6e66 6f5d 0d0a 7461  ..[egg_info]..ta
+00000290: 675f 6275 696c 6420 3d20 0d0a 7461 675f  g_build = ..tag_
+000002a0: 6461 7465 203d 2030 0d0a 0d0a            date = 0....
```

