# Comparing `tmp/napari-script-editor-0.2.8.tar.gz` & `tmp/napari-script-editor-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "napari-script-editor-0.2.8.tar", last modified: Sun Mar 20 10:14:11 2022, max compression
+gzip compressed data, was "napari-script-editor-0.2.9.tar", last modified: Thu Oct  6 07:04:00 2022, max compression
```

## Comparing `napari-script-editor-0.2.8.tar` & `napari-script-editor-0.2.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2022-03-20 10:14:11.802665 napari-script-editor-0.2.8/
--rw-rw-rw-   0        0        0     1519 2021-11-06 07:24:30.000000 napari-script-editor-0.2.8/LICENSE
--rw-rw-rw-   0        0        0      127 2021-11-06 07:24:30.000000 napari-script-editor-0.2.8/MANIFEST.in
--rw-rw-rw-   0        0        0     5476 2022-03-20 10:14:11.803665 napari-script-editor-0.2.8/PKG-INFO
--rw-rw-rw-   0        0        0     4134 2021-12-30 14:53:14.000000 napari-script-editor-0.2.8/README.md
--rw-rw-rw-   0        0        0      329 2022-01-01 15:31:17.000000 napari-script-editor-0.2.8/requirements.txt
--rw-rw-rw-   0        0        0     1593 2022-03-20 10:14:11.828186 napari-script-editor-0.2.8/setup.cfg
--rw-rw-rw-   0        0        0       89 2021-11-06 07:24:30.000000 napari-script-editor-0.2.8/setup.py
-drwxrwxrwx   0        0        0        0 2022-03-20 10:14:11.781981 napari-script-editor-0.2.8/src/
-drwxrwxrwx   0        0        0        0 2022-03-20 10:14:11.790983 napari-script-editor-0.2.8/src/napari_script_editor/
--rw-rw-rw-   0        0        0      186 2022-03-20 10:13:30.000000 napari-script-editor-0.2.8/src/napari_script_editor/__init__.py
--rw-rw-rw-   0        0        0     4643 2022-03-20 10:07:58.000000 napari-script-editor-0.2.8/src/napari_script_editor/_dock_widget.py
--rw-rw-rw-   0        0        0     2004 2021-12-02 20:38:13.000000 napari-script-editor-0.2.8/src/napari_script_editor/_scripts_directory.py
-drwxrwxrwx   0        0        0        0 2022-03-20 10:14:11.801664 napari-script-editor-0.2.8/src/napari_script_editor/_tests/
--rw-rw-rw-   0        0        0        0 2021-11-06 07:24:30.000000 napari-script-editor-0.2.8/src/napari_script_editor/_tests/__init__.py
--rw-rw-rw-   0        0        0      996 2022-01-03 14:55:01.000000 napari-script-editor-0.2.8/src/napari_script_editor/_tests/test_dock_widget.py
-drwxrwxrwx   0        0        0        0 2022-03-20 10:14:11.800665 napari-script-editor-0.2.8/src/napari_script_editor.egg-info/
--rw-rw-rw-   0        0        0     5476 2022-03-20 10:14:11.000000 napari-script-editor-0.2.8/src/napari_script_editor.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      576 2022-03-20 10:14:11.000000 napari-script-editor-0.2.8/src/napari_script_editor.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-03-20 10:14:11.000000 napari-script-editor-0.2.8/src/napari_script_editor.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       60 2022-03-20 10:14:11.000000 napari-script-editor-0.2.8/src/napari_script_editor.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      142 2022-03-20 10:14:11.000000 napari-script-editor-0.2.8/src/napari_script_editor.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2022-03-20 10:14:11.000000 napari-script-editor-0.2.8/src/napari_script_editor.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2022-10-06 07:04:00.098748 napari-script-editor-0.2.9/
+-rw-rw-rw-   0        0        0     1519 2021-11-06 07:24:30.000000 napari-script-editor-0.2.9/LICENSE
+-rw-rw-rw-   0        0        0      127 2021-11-06 07:24:30.000000 napari-script-editor-0.2.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     5453 2022-10-06 07:04:00.098748 napari-script-editor-0.2.9/PKG-INFO
+-rw-rw-rw-   0        0        0     4134 2021-12-30 14:53:14.000000 napari-script-editor-0.2.9/README.md
+-rw-rw-rw-   0        0        0      393 2022-10-06 06:59:46.000000 napari-script-editor-0.2.9/requirements.txt
+-rw-rw-rw-   0        0        0     1658 2022-10-06 07:04:00.098748 napari-script-editor-0.2.9/setup.cfg
+-rw-rw-rw-   0        0        0       89 2021-11-06 07:24:30.000000 napari-script-editor-0.2.9/setup.py
+drwxrwxrwx   0        0        0        0 2022-10-06 07:04:00.052183 napari-script-editor-0.2.9/src/
+drwxrwxrwx   0        0        0        0 2022-10-06 07:04:00.067495 napari-script-editor-0.2.9/src/napari_script_editor/
+-rw-rw-rw-   0        0        0      186 2022-10-06 07:00:10.000000 napari-script-editor-0.2.9/src/napari_script_editor/__init__.py
+-rw-rw-rw-   0        0        0     4643 2022-03-20 10:07:58.000000 napari-script-editor-0.2.9/src/napari_script_editor/_dock_widget.py
+-rw-rw-rw-   0        0        0     2004 2021-12-02 20:38:13.000000 napari-script-editor-0.2.9/src/napari_script_editor/_scripts_directory.py
+drwxrwxrwx   0        0        0        0 2022-10-06 07:04:00.098748 napari-script-editor-0.2.9/src/napari_script_editor/_tests/
+-rw-rw-rw-   0        0        0        0 2021-11-06 07:24:30.000000 napari-script-editor-0.2.9/src/napari_script_editor/_tests/__init__.py
+-rw-rw-rw-   0        0        0      996 2022-01-03 14:55:01.000000 napari-script-editor-0.2.9/src/napari_script_editor/_tests/test_dock_widget.py
+drwxrwxrwx   0        0        0        0 2022-10-06 07:04:00.098748 napari-script-editor-0.2.9/src/napari_script_editor.egg-info/
+-rw-rw-rw-   0        0        0     5453 2022-10-06 07:03:59.000000 napari-script-editor-0.2.9/src/napari_script_editor.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      576 2022-10-06 07:03:59.000000 napari-script-editor-0.2.9/src/napari_script_editor.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-10-06 07:03:59.000000 napari-script-editor-0.2.9/src/napari_script_editor.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       60 2022-10-06 07:03:59.000000 napari-script-editor-0.2.9/src/napari_script_editor.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      158 2022-10-06 07:03:59.000000 napari-script-editor-0.2.9/src/napari_script_editor.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2022-10-06 07:03:59.000000 napari-script-editor-0.2.9/src/napari_script_editor.egg-info/top_level.txt
```

### Comparing `napari-script-editor-0.2.8/LICENSE` & `napari-script-editor-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `napari-script-editor-0.2.8/PKG-INFO` & `napari-script-editor-0.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: napari-script-editor
-Version: 0.2.8
+Version: 0.2.9
 Summary: A python script editor for napari
 Home-page: https://github.com/haesleinhuepf/napari-script-editor
 Author: Robert Haase
 Author-email: robert.haase@tu-dresden.de
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/haesleinhuepf/napari-script-editor/issues
 Project-URL: Documentation, https://github.com/haesleinhuepf/napari-script-editor#README.md
 Project-URL: Source Code, https://github.com/haesleinhuepf/napari-script-editor
 Project-URL: User Support, https://github.com/haesleinhuepf/napari-script-editor/issues
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Framework :: napari
 Classifier: Topic :: Scientific/Engineering :: Image Processing
 Classifier: Topic :: Text Editors :: Integrated Development Environments (IDE)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -109,9 +108,7 @@
 
 [file an issue]: https://github.com/haesleinhuepf/napari-script-editor/issues
 
 [napari]: https://github.com/napari/napari
 [tox]: https://tox.readthedocs.io/en/latest/
 [pip]: https://pypi.org/project/pip/
 [PyPI]: https://pypi.org/
-
-
```

### Comparing `napari-script-editor-0.2.8/README.md` & `napari-script-editor-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `napari-script-editor-0.2.8/setup.cfg` & `napari-script-editor-0.2.9/setup.cfg`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 206e 6170 6172 692d 7363 7269 7074   = napari-script
 00000020: 2d65 6469 746f 720d 0a76 6572 7369 6f6e  -editor..version
-00000030: 203d 2030 2e32 2e38 0d0a 6175 7468 6f72   = 0.2.8..author
+00000030: 203d 2030 2e32 2e39 0d0a 6175 7468 6f72   = 0.2.9..author
 00000040: 203d 2052 6f62 6572 7420 4861 6173 650d   = Robert Haase.
 00000050: 0a61 7574 686f 725f 656d 6169 6c20 3d20  .author_email = 
 00000060: 726f 6265 7274 2e68 6161 7365 4074 752d  robert.haase@tu-
 00000070: 6472 6573 6465 6e2e 6465 0d0a 7572 6c20  dresden.de..url 
 00000080: 3d20 6874 7470 733a 2f2f 6769 7468 7562  = https://github
 00000090: 2e63 6f6d 2f68 6165 736c 6569 6e68 7565  .com/haesleinhue
 000000a0: 7066 2f6e 6170 6172 692d 7363 7269 7074  pf/napari-script
@@ -82,19 +82,23 @@
 00000510: 6d70 790d 0a09 6e61 7061 7269 0d0a 0968  mpy...napari...h
 00000520: 6165 736c 6569 6e68 7565 7066 2d70 7971  aesleinhuepf-pyq
 00000530: 6f64 652e 636f 7265 3e3d 322e 3135 2e35  ode.core>=2.15.5
 00000540: 0d0a 0968 6165 736c 6569 6e68 7565 7066  ...haesleinhuepf
 00000550: 2d70 7971 6f64 652e 7079 7468 6f6e 3e3d  -pyqode.python>=
 00000560: 322e 3135 2e32 0d0a 096e 6170 6172 692d  2.15.2...napari-
 00000570: 746f 6f6c 732d 6d65 6e75 0d0a 096a 6564  tools-menu...jed
-00000580: 693e 3d30 2e31 382e 300d 0a0d 0a5b 6f70  i>=0.18.0....[op
-00000590: 7469 6f6e 732e 7061 636b 6167 6573 2e66  tions.packages.f
-000005a0: 696e 645d 0d0a 7768 6572 6520 3d20 7372  ind]..where = sr
-000005b0: 630d 0a0d 0a5b 6f70 7469 6f6e 732e 656e  c....[options.en
-000005c0: 7472 795f 706f 696e 7473 5d0d 0a6e 6170  try_points]..nap
-000005d0: 6172 692e 706c 7567 696e 203d 200d 0a09  ari.plugin = ...
-000005e0: 6e61 7061 7269 2d73 6372 6970 742d 6564  napari-script-ed
-000005f0: 6974 6f72 203d 206e 6170 6172 695f 7363  itor = napari_sc
-00000600: 7269 7074 5f65 6469 746f 720d 0a0d 0a5b  ript_editor....[
-00000610: 6567 675f 696e 666f 5d0d 0a74 6167 5f62  egg_info]..tag_b
-00000620: 7569 6c64 203d 200d 0a74 6167 5f64 6174  uild = ..tag_dat
-00000630: 6520 3d20 300d 0a0d 0a                   e = 0....
+00000580: 693e 3d30 2e31 382e 300d 0a09 7079 666c  i>=0.18.0...pyfl
+00000590: 616b 6573 3c3d 322e 342e 3020 2320 6874  akes<=2.4.0 # ht
+000005a0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+000005b0: 2f50 7943 5141 2f70 7966 6c61 6b65 732f  /PyCQA/pyflakes/
+000005c0: 6973 7375 6573 2f37 3333 0d0a 0d0a 5b6f  issues/733....[o
+000005d0: 7074 696f 6e73 2e70 6163 6b61 6765 732e  ptions.packages.
+000005e0: 6669 6e64 5d0d 0a77 6865 7265 203d 2073  find]..where = s
+000005f0: 7263 0d0a 0d0a 5b6f 7074 696f 6e73 2e65  rc....[options.e
+00000600: 6e74 7279 5f70 6f69 6e74 735d 0d0a 6e61  ntry_points]..na
+00000610: 7061 7269 2e70 6c75 6769 6e20 3d20 0d0a  pari.plugin = ..
+00000620: 096e 6170 6172 692d 7363 7269 7074 2d65  .napari-script-e
+00000630: 6469 746f 7220 3d20 6e61 7061 7269 5f73  ditor = napari_s
+00000640: 6372 6970 745f 6564 6974 6f72 0d0a 0d0a  cript_editor....
+00000650: 5b65 6767 5f69 6e66 6f5d 0d0a 7461 675f  [egg_info]..tag_
+00000660: 6275 696c 6420 3d20 0d0a 7461 675f 6461  build = ..tag_da
+00000670: 7465 203d 2030 0d0a 0d0a                 te = 0....
```

### Comparing `napari-script-editor-0.2.8/src/napari_script_editor/_dock_widget.py` & `napari-script-editor-0.2.9/src/napari_script_editor/_dock_widget.py`

 * *Files identical despite different names*

### Comparing `napari-script-editor-0.2.8/src/napari_script_editor/_scripts_directory.py` & `napari-script-editor-0.2.9/src/napari_script_editor/_scripts_directory.py`

 * *Files identical despite different names*

### Comparing `napari-script-editor-0.2.8/src/napari_script_editor/_tests/test_dock_widget.py` & `napari-script-editor-0.2.9/src/napari_script_editor/_tests/test_dock_widget.py`

 * *Files identical despite different names*

### Comparing `napari-script-editor-0.2.8/src/napari_script_editor.egg-info/PKG-INFO` & `napari-script-editor-0.2.9/src/napari_script_editor.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: napari-script-editor
-Version: 0.2.8
+Version: 0.2.9
 Summary: A python script editor for napari
 Home-page: https://github.com/haesleinhuepf/napari-script-editor
 Author: Robert Haase
 Author-email: robert.haase@tu-dresden.de
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/haesleinhuepf/napari-script-editor/issues
 Project-URL: Documentation, https://github.com/haesleinhuepf/napari-script-editor#README.md
 Project-URL: Source Code, https://github.com/haesleinhuepf/napari-script-editor
 Project-URL: User Support, https://github.com/haesleinhuepf/napari-script-editor/issues
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Framework :: napari
 Classifier: Topic :: Scientific/Engineering :: Image Processing
 Classifier: Topic :: Text Editors :: Integrated Development Environments (IDE)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -109,9 +108,7 @@
 
 [file an issue]: https://github.com/haesleinhuepf/napari-script-editor/issues
 
 [napari]: https://github.com/napari/napari
 [tox]: https://tox.readthedocs.io/en/latest/
 [pip]: https://pypi.org/project/pip/
 [PyPI]: https://pypi.org/
-
-
```

### Comparing `napari-script-editor-0.2.8/src/napari_script_editor.egg-info/SOURCES.txt` & `napari-script-editor-0.2.9/src/napari_script_editor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

