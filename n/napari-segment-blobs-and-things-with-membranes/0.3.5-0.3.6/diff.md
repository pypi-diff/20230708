# Comparing `tmp/napari-segment-blobs-and-things-with-membranes-0.3.5.tar.gz` & `tmp/napari-segment-blobs-and-things-with-membranes-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "napari-segment-blobs-and-things-with-membranes-0.3.5.tar", last modified: Thu Jun 29 14:03:37 2023, max compression
+gzip compressed data, was "napari-segment-blobs-and-things-with-membranes-0.3.6.tar", last modified: Sat Jul  8 15:53:38 2023, max compression
```

## Comparing `napari-segment-blobs-and-things-with-membranes-0.3.5.tar` & `napari-segment-blobs-and-things-with-membranes-0.3.6.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-06-29 14:03:37.942925 napari-segment-blobs-and-things-with-membranes-0.3.5/
--rw-rw-rw-   0        0        0     1545 2023-02-23 17:18:17.000000 napari-segment-blobs-and-things-with-membranes-0.3.5/LICENSE
--rw-rw-rw-   0        0        0      127 2023-02-23 17:18:17.000000 napari-segment-blobs-and-things-with-membranes-0.3.5/MANIFEST.in
--rw-rw-rw-   0        0        0    10368 2023-06-29 14:03:37.942925 napari-segment-blobs-and-things-with-membranes-0.3.5/PKG-INFO
--rw-rw-rw-   0        0        0     8782 2023-02-23 17:18:17.000000 napari-segment-blobs-and-things-with-membranes-0.3.5/README.md
-drwxrwxrwx   0        0        0        0 2023-06-29 14:03:37.911671 napari-segment-blobs-and-things-with-membranes-0.3.5/napari_segment_blobs_and_things_with_membranes/
--rw-rw-rw-   0        0        0    37937 2023-06-29 14:02:19.000000 napari-segment-blobs-and-things-with-membranes-0.3.5/napari_segment_blobs_and_things_with_membranes/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-29 14:03:37.942925 napari-segment-blobs-and-things-with-membranes-0.3.5/napari_segment_blobs_and_things_with_membranes/_tests/
--rw-rw-rw-   0        0        0        0 2023-02-23 17:18:17.000000 napari-segment-blobs-and-things-with-membranes-0.3.5/napari_segment_blobs_and_things_with_membranes/_tests/__init__.py
--rw-rw-rw-   0        0        0     3995 2023-06-29 13:51:48.000000 napari-segment-blobs-and-things-with-membranes-0.3.5/napari_segment_blobs_and_things_with_membranes/_tests/test_function.py
-drwxrwxrwx   0        0        0        0 2023-06-29 14:03:37.942925 napari-segment-blobs-and-things-with-membranes-0.3.5/napari_segment_blobs_and_things_with_membranes.egg-info/
--rw-rw-rw-   0        0        0    10368 2023-06-29 14:03:37.000000 napari-segment-blobs-and-things-with-membranes-0.3.5/napari_segment_blobs_and_things_with_membranes.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      683 2023-06-29 14:03:37.000000 napari-segment-blobs-and-things-with-membranes-0.3.5/napari_segment_blobs_and_things_with_membranes.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-29 14:03:37.000000 napari-segment-blobs-and-things-with-membranes-0.3.5/napari_segment_blobs_and_things_with_membranes.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      112 2023-06-29 14:03:37.000000 napari-segment-blobs-and-things-with-membranes-0.3.5/napari_segment_blobs_and_things_with_membranes.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      139 2023-06-29 14:03:37.000000 napari-segment-blobs-and-things-with-membranes-0.3.5/napari_segment_blobs_and_things_with_membranes.egg-info/requires.txt
--rw-rw-rw-   0        0        0       47 2023-06-29 14:03:37.000000 napari-segment-blobs-and-things-with-membranes-0.3.5/napari_segment_blobs_and_things_with_membranes.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      302 2023-02-23 17:18:17.000000 napari-segment-blobs-and-things-with-membranes-0.3.5/requirements.txt
--rw-rw-rw-   0        0        0     1848 2023-06-29 14:03:37.942925 napari-segment-blobs-and-things-with-membranes-0.3.5/setup.cfg
--rw-rw-rw-   0        0        0       89 2023-02-23 17:18:17.000000 napari-segment-blobs-and-things-with-membranes-0.3.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-08 15:53:38.115176 napari-segment-blobs-and-things-with-membranes-0.3.6/
+-rw-rw-rw-   0        0        0     1545 2023-02-23 17:18:17.000000 napari-segment-blobs-and-things-with-membranes-0.3.6/LICENSE
+-rw-rw-rw-   0        0        0      127 2023-02-23 17:18:17.000000 napari-segment-blobs-and-things-with-membranes-0.3.6/MANIFEST.in
+-rw-rw-rw-   0        0        0    10177 2023-07-08 15:53:38.116179 napari-segment-blobs-and-things-with-membranes-0.3.6/PKG-INFO
+-rw-rw-rw-   0        0        0     8591 2023-07-08 15:51:37.000000 napari-segment-blobs-and-things-with-membranes-0.3.6/README.md
+drwxrwxrwx   0        0        0        0 2023-07-08 15:53:38.085097 napari-segment-blobs-and-things-with-membranes-0.3.6/napari_segment_blobs_and_things_with_membranes/
+-rw-rw-rw-   0        0        0    38294 2023-07-08 15:52:27.000000 napari-segment-blobs-and-things-with-membranes-0.3.6/napari_segment_blobs_and_things_with_membranes/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-08 15:53:38.115176 napari-segment-blobs-and-things-with-membranes-0.3.6/napari_segment_blobs_and_things_with_membranes/_tests/
+-rw-rw-rw-   0        0        0        0 2023-02-23 17:18:17.000000 napari-segment-blobs-and-things-with-membranes-0.3.6/napari_segment_blobs_and_things_with_membranes/_tests/__init__.py
+-rw-rw-rw-   0        0        0     4033 2023-07-08 15:51:56.000000 napari-segment-blobs-and-things-with-membranes-0.3.6/napari_segment_blobs_and_things_with_membranes/_tests/test_function.py
+drwxrwxrwx   0        0        0        0 2023-07-08 15:53:38.112168 napari-segment-blobs-and-things-with-membranes-0.3.6/napari_segment_blobs_and_things_with_membranes.egg-info/
+-rw-rw-rw-   0        0        0    10177 2023-07-08 15:53:37.000000 napari-segment-blobs-and-things-with-membranes-0.3.6/napari_segment_blobs_and_things_with_membranes.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      683 2023-07-08 15:53:37.000000 napari-segment-blobs-and-things-with-membranes-0.3.6/napari_segment_blobs_and_things_with_membranes.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-08 15:53:37.000000 napari-segment-blobs-and-things-with-membranes-0.3.6/napari_segment_blobs_and_things_with_membranes.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      112 2023-07-08 15:53:37.000000 napari-segment-blobs-and-things-with-membranes-0.3.6/napari_segment_blobs_and_things_with_membranes.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      139 2023-07-08 15:53:37.000000 napari-segment-blobs-and-things-with-membranes-0.3.6/napari_segment_blobs_and_things_with_membranes.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       47 2023-07-08 15:53:37.000000 napari-segment-blobs-and-things-with-membranes-0.3.6/napari_segment_blobs_and_things_with_membranes.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      302 2023-02-23 17:18:17.000000 napari-segment-blobs-and-things-with-membranes-0.3.6/requirements.txt
+-rw-rw-rw-   0        0        0     1848 2023-07-08 15:53:38.117181 napari-segment-blobs-and-things-with-membranes-0.3.6/setup.cfg
+-rw-rw-rw-   0        0        0       89 2023-02-23 17:18:17.000000 napari-segment-blobs-and-things-with-membranes-0.3.6/setup.py
```

### Comparing `napari-segment-blobs-and-things-with-membranes-0.3.5/LICENSE` & `napari-segment-blobs-and-things-with-membranes-0.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `napari-segment-blobs-and-things-with-membranes-0.3.5/PKG-INFO` & `napari-segment-blobs-and-things-with-membranes-0.3.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-segment-blobs-and-things-with-membranes
-Version: 0.3.5
+Version: 0.3.6
 Summary: A plugin based on scikit-image for segmenting nuclei and cells based on fluorescent microscopy images with high intensity in nuclei and/or membranes
 Home-page: https://github.com/haesleinhuepf/napari-segment-blobs-and-things-with-membranes
 Author: Robert Haase
 Author-email: robert.haase@tu-dresden.de
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/haesleinhuepf/napari-segment-blobs-and-things-with-membranes/issues
 Project-URL: Documentation, https://github.com/haesleinhuepf/napari-segment-blobs-and-things-with-membranes#README.md
@@ -126,19 +126,15 @@
 
 ----------------------------------
 
 This [napari] plugin was generated with [Cookiecutter] using with [@napari]'s [cookiecutter-napari-plugin] template.
 
 ## Installation
 
-You can install `napari-segment-blobs-and-things-with-membranes` using `conda` and `pip`.
-If you have never used `conda` before, please go through [this tutorial](https://biapol.github.io/blog/johannes_mueller/anaconda_getting_started/) first.
-
-    conda install -c conda-forge napari
-    pip install napari-segment-blobs-and-things-with-membranes
+This plugin is part of devbio-napari. To install it, please follow its [installation instructions](https://github.com/haesleinhuepf/devbio-napari#installation).
 
 ## Contributing
 
 Contributions are very welcome. Tests can be run with [tox], please ensure
 the coverage at least stays the same before you submit a pull request.
 
 ## License
```

### Comparing `napari-segment-blobs-and-things-with-membranes-0.3.5/README.md` & `napari-segment-blobs-and-things-with-membranes-0.3.6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -98,19 +98,15 @@
 
 ----------------------------------
 
 This [napari] plugin was generated with [Cookiecutter] using with [@napari]'s [cookiecutter-napari-plugin] template.
 
 ## Installation
 
-You can install `napari-segment-blobs-and-things-with-membranes` using `conda` and `pip`.
-If you have never used `conda` before, please go through [this tutorial](https://biapol.github.io/blog/johannes_mueller/anaconda_getting_started/) first.
-
-    conda install -c conda-forge napari
-    pip install napari-segment-blobs-and-things-with-membranes
+This plugin is part of devbio-napari. To install it, please follow its [installation instructions](https://github.com/haesleinhuepf/devbio-napari#installation).
 
 ## Contributing
 
 Contributions are very welcome. Tests can be run with [tox], please ensure
 the coverage at least stays the same before you submit a pull request.
 
 ## License
```

### Comparing `napari-segment-blobs-and-things-with-membranes-0.3.5/napari_segment_blobs_and_things_with_membranes/__init__.py` & `napari-segment-blobs-and-things-with-membranes-0.3.6/napari_segment_blobs_and_things_with_membranes/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 00000000: 0d0a 5f5f 7665 7273 696f 6e5f 5f20 3d20  ..__version__ = 
-00000010: 2230 2e33 2e35 220d 0a5f 5f63 6f6d 6d6f  "0.3.5"..__commo
+00000010: 2230 2e33 2e36 220d 0a5f 5f63 6f6d 6d6f  "0.3.6"..__commo
 00000020: 6e5f 616c 6961 735f 5f20 3d20 226e 7362  n_alias__ = "nsb
 00000030: 6174 776d 220d 0a0d 0a66 726f 6d20 6e61  atwm"....from na
 00000040: 7061 7269 5f70 6c75 6769 6e5f 656e 6769  pari_plugin_engi
 00000050: 6e65 2069 6d70 6f72 7420 6e61 7061 7269  ne import napari
 00000060: 5f68 6f6f 6b5f 696d 706c 656d 656e 7461  _hook_implementa
 00000070: 7469 6f6e 0d0a 696d 706f 7274 206e 756d  tion..import num
 00000080: 7079 2061 7320 6e70 0d0a 6672 6f6d 2073  py as np..from s
@@ -2365,8 +2365,30 @@
 000093c0: 616d 706c 655f 792c 203a 3a73 616d 706c  ample_y, ::sampl
 000093d0: 655f 785d 0d0a 2020 2020 656c 7365 3a0d  e_x]..    else:.
 000093e0: 0a20 2020 2020 2020 2072 6169 7365 2056  .        raise V
 000093f0: 616c 7565 4572 726f 7228 2253 7562 2d73  alueError("Sub-s
 00009400: 616d 706c 696e 6720 6f6e 6c79 2073 7570  ampling only sup
 00009410: 706f 7274 6564 2066 6f72 2032 4420 616e  ported for 2D an
 00009420: 6420 3344 2069 6d61 6765 7322 290d 0a0d  d 3D images")...
-00009430: 0a                                       .
+00009430: 0a0d 0a40 7265 6769 7374 6572 5f66 756e  ...@register_fun
+00009440: 6374 696f 6e28 6d65 6e75 3d22 5472 616e  ction(menu="Tran
+00009450: 7366 6f72 6d73 203e 2052 656d 6f76 6520  sforms > Remove 
+00009460: 6178 6573 206f 6620 6c65 6e67 7468 2031  axes of length 1
+00009470: 2028 6e75 6d70 792e 7371 7565 657a 652c   (numpy.squeeze,
+00009480: 206e 7362 6174 776d 2922 290d 0a40 6a75   nsbatwm)")..@ju
+00009490: 7079 7465 725f 6469 7370 6c61 7961 626c  pyter_displayabl
+000094a0: 655f 6f75 7470 7574 286c 6962 7261 7279  e_output(library
+000094b0: 5f6e 616d 653d 276e 7362 6174 776d 272c  _name='nsbatwm',
+000094c0: 2068 656c 705f 7572 6c3d 2768 7474 7073   help_url='https
+000094d0: 3a2f 2f77 7777 2e6e 6170 6172 692d 6875  ://www.napari-hu
+000094e0: 622e 6f72 672f 706c 7567 696e 732f 6e61  b.org/plugins/na
+000094f0: 7061 7269 2d73 6567 6d65 6e74 2d62 6c6f  pari-segment-blo
+00009500: 6273 2d61 6e64 2d74 6869 6e67 732d 7769  bs-and-things-wi
+00009510: 7468 2d6d 656d 6272 616e 6573 2729 0d0a  th-membranes')..
+00009520: 4074 696d 655f 736c 6963 6572 0d0a 6465  @time_slicer..de
+00009530: 6620 7371 7565 657a 6528 696d 6167 653a  f squeeze(image:
+00009540: 226e 6170 6172 692e 7479 7065 732e 496d  "napari.types.Im
+00009550: 6167 6544 6174 6122 2920 2d3e 2022 6e61  ageData") -> "na
+00009560: 7061 7269 2e74 7970 6573 2e49 6d61 6765  pari.types.Image
+00009570: 4461 7461 223a 0d0a 2020 2020 7265 7475  Data":..    retu
+00009580: 726e 206e 702e 7371 7565 657a 6528 696d  rn np.squeeze(im
+00009590: 6167 6529 0d0a                           age)..
```

### Comparing `napari-segment-blobs-and-things-with-membranes-0.3.5/napari_segment_blobs_and_things_with_membranes/_tests/test_function.py` & `napari-segment-blobs-and-things-with-membranes-0.3.6/napari_segment_blobs_and_things_with_membranes/_tests/test_function.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,15 +36,16 @@
         divide_images,\
         invert_image, \
         skeletonize, \
         rescale, \
         resize, \
         butterworth, \
         extract_slice, \
-        sub_sample
+        sub_sample, \
+        squeeze
 
     import numpy as np
 
     image = np.asarray([[0, 1, 2, 3],
                         [2, 0, 1, 3],
                         [2, 253, 1, 3],
                         [255, 253, 1, 3]])
@@ -73,15 +74,16 @@
         morphological_gradient,
         local_minima_seeded_watershed,
         invert_image,
         rescale,
         resize,
         butterworth,
         extract_slice,
-        sub_sample]:
+        sub_sample,
+        squeeze]:
 
         print(operation)
 
         operation(image)
 
     for operation in [
         seeded_watershed,
```

### Comparing `napari-segment-blobs-and-things-with-membranes-0.3.5/napari_segment_blobs_and_things_with_membranes.egg-info/PKG-INFO` & `napari-segment-blobs-and-things-with-membranes-0.3.6/napari_segment_blobs_and_things_with_membranes.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-segment-blobs-and-things-with-membranes
-Version: 0.3.5
+Version: 0.3.6
 Summary: A plugin based on scikit-image for segmenting nuclei and cells based on fluorescent microscopy images with high intensity in nuclei and/or membranes
 Home-page: https://github.com/haesleinhuepf/napari-segment-blobs-and-things-with-membranes
 Author: Robert Haase
 Author-email: robert.haase@tu-dresden.de
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/haesleinhuepf/napari-segment-blobs-and-things-with-membranes/issues
 Project-URL: Documentation, https://github.com/haesleinhuepf/napari-segment-blobs-and-things-with-membranes#README.md
@@ -126,19 +126,15 @@
 
 ----------------------------------
 
 This [napari] plugin was generated with [Cookiecutter] using with [@napari]'s [cookiecutter-napari-plugin] template.
 
 ## Installation
 
-You can install `napari-segment-blobs-and-things-with-membranes` using `conda` and `pip`.
-If you have never used `conda` before, please go through [this tutorial](https://biapol.github.io/blog/johannes_mueller/anaconda_getting_started/) first.
-
-    conda install -c conda-forge napari
-    pip install napari-segment-blobs-and-things-with-membranes
+This plugin is part of devbio-napari. To install it, please follow its [installation instructions](https://github.com/haesleinhuepf/devbio-napari#installation).
 
 ## Contributing
 
 Contributions are very welcome. Tests can be run with [tox], please ensure
 the coverage at least stays the same before you submit a pull request.
 
 ## License
```

### Comparing `napari-segment-blobs-and-things-with-membranes-0.3.5/napari_segment_blobs_and_things_with_membranes.egg-info/SOURCES.txt` & `napari-segment-blobs-and-things-with-membranes-0.3.6/napari_segment_blobs_and_things_with_membranes.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `napari-segment-blobs-and-things-with-membranes-0.3.5/setup.cfg` & `napari-segment-blobs-and-things-with-membranes-0.3.6/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 206e 6170 6172 692d 7365 676d 656e   = napari-segmen
 00000020: 742d 626c 6f62 732d 616e 642d 7468 696e  t-blobs-and-thin
 00000030: 6773 2d77 6974 682d 6d65 6d62 7261 6e65  gs-with-membrane
 00000040: 730d 0a76 6572 7369 6f6e 203d 2030 2e33  s..version = 0.3
-00000050: 2e35 0d0a 6175 7468 6f72 203d 2052 6f62  .5..author = Rob
+00000050: 2e36 0d0a 6175 7468 6f72 203d 2052 6f62  .6..author = Rob
 00000060: 6572 7420 4861 6173 650d 0a61 7574 686f  ert Haase..autho
 00000070: 725f 656d 6169 6c20 3d20 726f 6265 7274  r_email = robert
 00000080: 2e68 6161 7365 4074 752d 6472 6573 6465  .haase@tu-dresde
 00000090: 6e2e 6465 0d0a 7572 6c20 3d20 6874 7470  n.de..url = http
 000000a0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f68  s://github.com/h
 000000b0: 6165 736c 6569 6e68 7565 7066 2f6e 6170  aesleinhuepf/nap
 000000c0: 6172 692d 7365 676d 656e 742d 626c 6f62  ari-segment-blob
```

