# Comparing `tmp/napari-live-recording-0.3.0.tar.gz` & `tmp/napari-live-recording-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "napari-live-recording-0.3.0.tar", last modified: Fri Jun  9 18:49:21 2023, max compression
+gzip compressed data, was "napari-live-recording-0.3.2.tar", last modified: Sat Jul  8 18:30:00 2023, max compression
```

## Comparing `napari-live-recording-0.3.0.tar` & `napari-live-recording-0.3.2.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxrwxrwx   0        0        0        0 2023-06-09 18:49:21.209030 napari-live-recording-0.3.0/
-drwxrwxrwx   0        0        0        0 2023-06-09 18:49:21.139921 napari-live-recording-0.3.0/.github/
-drwxrwxrwx   0        0        0        0 2023-06-09 18:49:21.155111 napari-live-recording-0.3.0/.github/workflows/
--rw-rw-rw-   0        0        0      590 2023-01-27 10:07:39.000000 napari-live-recording-0.3.0/.github/workflows/plugin_preview.yml
--rw-rw-rw-   0        0        0     1076 2023-01-27 10:07:39.000000 napari-live-recording-0.3.0/.gitignore
--rw-rw-rw-   0        0        0     1101 2023-01-27 10:07:39.000000 napari-live-recording-0.3.0/LICENSE
--rw-rw-rw-   0        0        0     4527 2023-06-09 18:49:21.209030 napari-live-recording-0.3.0/PKG-INFO
--rw-rw-rw-   0        0        0     3206 2023-06-09 18:21:57.000000 napari-live-recording-0.3.0/README.md
--rwxrwxrwx   0        0        0      213 2023-01-27 10:07:39.000000 napari-live-recording-0.3.0/deploy.bat
-drwxrwxrwx   0        0        0        0 2023-06-09 18:49:21.157112 napari-live-recording-0.3.0/docs/
--rw-rw-rw-   0        0        0       67 2023-06-09 17:35:28.000000 napari-live-recording-0.3.0/docs/README.md
--rw-rw-rw-   0        0        0     1184 2023-06-09 18:45:26.000000 napari-live-recording-0.3.0/docs/changelog.md
--rw-rw-rw-   0        0        0       91 2023-01-27 10:07:39.000000 napari-live-recording-0.3.0/pyproject.toml
--rw-rw-rw-   0        0        0     1718 2023-06-09 18:49:21.211091 napari-live-recording-0.3.0/setup.cfg
--rw-rw-rw-   0        0        0       87 2023-01-27 10:07:39.000000 napari-live-recording-0.3.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-09 18:49:21.141918 napari-live-recording-0.3.0/src/
-drwxrwxrwx   0        0        0        0 2023-06-09 18:49:21.159113 napari-live-recording-0.3.0/src/napari_live_recording/
--rw-rw-rw-   0        0        0      676 2023-06-09 17:35:28.000000 napari-live-recording-0.3.0/src/napari_live_recording/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-09 18:49:21.197108 napari-live-recording-0.3.0/src/napari_live_recording/common/
--rw-rw-rw-   0        0        0     2671 2023-06-09 17:35:28.000000 napari-live-recording-0.3.0/src/napari_live_recording/common/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-09 18:49:21.198110 napari-live-recording-0.3.0/src/napari_live_recording/control/
--rw-rw-rw-   0        0        0     9015 2023-06-09 18:24:39.000000 napari-live-recording-0.3.0/src/napari_live_recording/control/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-09 18:49:21.205108 napari-live-recording-0.3.0/src/napari_live_recording/control/devices/
--rw-rw-rw-   0        0        0     1585 2023-06-09 17:35:28.000000 napari-live-recording-0.3.0/src/napari_live_recording/control/devices/__init__.py
--rw-rw-rw-   0        0        0     3916 2023-06-09 17:35:28.000000 napari-live-recording-0.3.0/src/napari_live_recording/control/devices/interface.py
--rw-rw-rw-   0        0        0     2655 2023-06-09 18:17:32.000000 napari-live-recording-0.3.0/src/napari_live_recording/control/devices/micro_manager.py
--rw-rw-rw-   0        0        0     4061 2023-06-09 17:35:28.000000 napari-live-recording-0.3.0/src/napari_live_recording/control/devices/opencv.py
--rw-rw-rw-   0        0        0      299 2023-01-27 10:07:39.000000 napari-live-recording-0.3.0/src/napari_live_recording/napari.yaml
-drwxrwxrwx   0        0        0        0 2023-06-09 18:49:21.207970 napari-live-recording-0.3.0/src/napari_live_recording/ui/
--rw-rw-rw-   0        0        0     7754 2023-06-09 17:35:28.000000 napari-live-recording-0.3.0/src/napari_live_recording/ui/__init__.py
--rw-rw-rw-   0        0        0    24878 2023-06-09 18:25:13.000000 napari-live-recording-0.3.0/src/napari_live_recording/ui/widgets.py
-drwxrwxrwx   0        0        0        0 2023-06-09 18:49:21.195109 napari-live-recording-0.3.0/src/napari_live_recording.egg-info/
--rw-rw-rw-   0        0        0     4527 2023-06-09 18:49:20.000000 napari-live-recording-0.3.0/src/napari_live_recording.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      915 2023-06-09 18:49:21.000000 napari-live-recording-0.3.0/src/napari_live_recording.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-09 18:49:20.000000 napari-live-recording-0.3.0/src/napari_live_recording.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       76 2023-06-09 18:49:20.000000 napari-live-recording-0.3.0/src/napari_live_recording.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      113 2023-06-09 18:49:20.000000 napari-live-recording-0.3.0/src/napari_live_recording.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2023-06-09 18:49:20.000000 napari-live-recording-0.3.0/src/napari_live_recording.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      896 2023-01-27 10:07:39.000000 napari-live-recording-0.3.0/tox.ini
+drwxrwxrwx   0        0        0        0 2023-07-08 18:30:00.096266 napari-live-recording-0.3.2/
+drwxrwxrwx   0        0        0        0 2023-07-08 18:30:00.047666 napari-live-recording-0.3.2/.github/
+drwxrwxrwx   0        0        0        0 2023-07-08 18:30:00.065860 napari-live-recording-0.3.2/.github/workflows/
+-rw-rw-rw-   0        0        0      590 2023-01-27 10:07:39.000000 napari-live-recording-0.3.2/.github/workflows/plugin_preview.yml
+-rw-rw-rw-   0        0        0     1076 2023-01-27 10:07:39.000000 napari-live-recording-0.3.2/.gitignore
+-rw-rw-rw-   0        0        0     1101 2023-01-27 10:07:39.000000 napari-live-recording-0.3.2/LICENSE
+-rw-rw-rw-   0        0        0     4527 2023-07-08 18:30:00.097276 napari-live-recording-0.3.2/PKG-INFO
+-rw-rw-rw-   0        0        0     3206 2023-06-09 18:21:57.000000 napari-live-recording-0.3.2/README.md
+-rwxrwxrwx   0        0        0      213 2023-01-27 10:07:39.000000 napari-live-recording-0.3.2/deploy.bat
+drwxrwxrwx   0        0        0        0 2023-07-08 18:30:00.067862 napari-live-recording-0.3.2/docs/
+-rw-rw-rw-   0        0        0       67 2023-06-09 17:35:28.000000 napari-live-recording-0.3.2/docs/README.md
+-rw-rw-rw-   0        0        0     1423 2023-07-08 18:28:29.000000 napari-live-recording-0.3.2/docs/changelog.md
+-rw-rw-rw-   0        0        0       91 2023-01-27 10:07:39.000000 napari-live-recording-0.3.2/pyproject.toml
+-rw-rw-rw-   0        0        0     1737 2023-07-08 18:30:00.099267 napari-live-recording-0.3.2/setup.cfg
+-rw-rw-rw-   0        0        0       87 2023-01-27 10:07:39.000000 napari-live-recording-0.3.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-08 18:30:00.050181 napari-live-recording-0.3.2/src/
+drwxrwxrwx   0        0        0        0 2023-07-08 18:30:00.070859 napari-live-recording-0.3.2/src/napari_live_recording/
+-rw-rw-rw-   0        0        0      676 2023-06-09 17:35:28.000000 napari-live-recording-0.3.2/src/napari_live_recording/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-08 18:30:00.085732 napari-live-recording-0.3.2/src/napari_live_recording/common/
+-rw-rw-rw-   0        0        0     2167 2023-07-08 18:24:17.000000 napari-live-recording-0.3.2/src/napari_live_recording/common/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-08 18:30:00.086733 napari-live-recording-0.3.2/src/napari_live_recording/control/
+-rw-rw-rw-   0        0        0     8998 2023-07-08 18:22:28.000000 napari-live-recording-0.3.2/src/napari_live_recording/control/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-08 18:30:00.093266 napari-live-recording-0.3.2/src/napari_live_recording/control/devices/
+-rw-rw-rw-   0        0        0     1605 2023-07-08 18:08:57.000000 napari-live-recording-0.3.2/src/napari_live_recording/control/devices/__init__.py
+-rw-rw-rw-   0        0        0     3916 2023-06-09 17:35:28.000000 napari-live-recording-0.3.2/src/napari_live_recording/control/devices/interface.py
+-rw-rw-rw-   0        0        0     2655 2023-06-09 18:17:32.000000 napari-live-recording-0.3.2/src/napari_live_recording/control/devices/micro_manager.py
+-rw-rw-rw-   0        0        0     4061 2023-06-09 17:35:28.000000 napari-live-recording-0.3.2/src/napari_live_recording/control/devices/opencv.py
+-rw-rw-rw-   0        0        0      299 2023-01-27 10:07:39.000000 napari-live-recording-0.3.2/src/napari_live_recording/napari.yaml
+drwxrwxrwx   0        0        0        0 2023-07-08 18:30:00.095264 napari-live-recording-0.3.2/src/napari_live_recording/ui/
+-rw-rw-rw-   0        0        0     7754 2023-06-09 17:35:28.000000 napari-live-recording-0.3.2/src/napari_live_recording/ui/__init__.py
+-rw-rw-rw-   0        0        0    24878 2023-06-09 18:25:13.000000 napari-live-recording-0.3.2/src/napari_live_recording/ui/widgets.py
+drwxrwxrwx   0        0        0        0 2023-07-08 18:30:00.084365 napari-live-recording-0.3.2/src/napari_live_recording.egg-info/
+-rw-rw-rw-   0        0        0     4527 2023-07-08 18:29:59.000000 napari-live-recording-0.3.2/src/napari_live_recording.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      915 2023-07-08 18:29:59.000000 napari-live-recording-0.3.2/src/napari_live_recording.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-08 18:29:59.000000 napari-live-recording-0.3.2/src/napari_live_recording.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       76 2023-07-08 18:29:59.000000 napari-live-recording-0.3.2/src/napari_live_recording.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      130 2023-07-08 18:29:59.000000 napari-live-recording-0.3.2/src/napari_live_recording.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2023-07-08 18:29:59.000000 napari-live-recording-0.3.2/src/napari_live_recording.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      896 2023-01-27 10:07:39.000000 napari-live-recording-0.3.2/tox.ini
```

### Comparing `napari-live-recording-0.3.0/.github/workflows/plugin_preview.yml` & `napari-live-recording-0.3.2/.github/workflows/plugin_preview.yml`

 * *Files identical despite different names*

### Comparing `napari-live-recording-0.3.0/.gitignore` & `napari-live-recording-0.3.2/.gitignore`

 * *Files identical despite different names*

### Comparing `napari-live-recording-0.3.0/LICENSE` & `napari-live-recording-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `napari-live-recording-0.3.0/PKG-INFO` & `napari-live-recording-0.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-live-recording
-Version: 0.3.0
+Version: 0.3.2
 Summary: A napari plugin for live video recording with a generic camera device.
 Home-page: https://github.com/jethro33/napari-live-recording
 Author: Jacopo Abramo
 Author-email: jacopo.abramo@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/jacopoabramo/napari-live-recording/issues
 Project-URL: Documentation, https://github.com/jacopoabramo/napari-live-recording#README.md
```

### Comparing `napari-live-recording-0.3.0/README.md` & `napari-live-recording-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `napari-live-recording-0.3.0/docs/changelog.md` & `napari-live-recording-0.3.2/docs/changelog.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,9 +1,18 @@
 # Changelog
 
+## 0.3.2
+
+Removed reference of tifffile enumerator `PHOTOMETRIC` (see #22)
+
+## 0.3.1
+
+- Added missing reference to `pymmcore-widgets` from `setup.cfg`
+- Added exception print when initializing list of available camera interfaces
+
 ## 0.3.0
 
 - Full rework of the plugin architecture ad user interface (hopefully for the last time)
 - Removed old device interface documentation
 - Fixed issues #16, #17
 - Added MicroManager interface (@felixwanitschke)
```

### Comparing `napari-live-recording-0.3.0/setup.cfg` & `napari-live-recording-0.3.2/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 206e 6170 6172 692d 6c69 7665 2d72   = napari-live-r
 00000020: 6563 6f72 6469 6e67 0d0a 7665 7273 696f  ecording..versio
-00000030: 6e20 3d20 302e 332e 300d 0a61 7574 686f  n = 0.3.0..autho
+00000030: 6e20 3d20 302e 332e 320d 0a61 7574 686f  n = 0.3.2..autho
 00000040: 7220 3d20 4a61 636f 706f 2041 6272 616d  r = Jacopo Abram
 00000050: 6f0d 0a61 7574 686f 725f 656d 6169 6c20  o..author_email 
 00000060: 3d20 6a61 636f 706f 2e61 6272 616d 6f40  = jacopo.abramo@
 00000070: 676d 6169 6c2e 636f 6d0d 0a75 726c 203d  gmail.com..url =
 00000080: 2068 7474 7073 3a2f 2f67 6974 6875 622e   https://github.
 00000090: 636f 6d2f 6a65 7468 726f 3333 2f6e 6170  com/jethro33/nap
 000000a0: 6172 692d 6c69 7665 2d72 6563 6f72 6469  ari-live-recordi
@@ -80,29 +80,30 @@
 000004f0: 096e 705f 696d 6167 655f 6275 6666 6572  .np_image_buffer
 00000500: 0d0a 096f 7065 6e63 762d 7079 7468 6f6e  ...opencv-python
 00000510: 0d0a 096f 7065 6e63 762d 636f 6e74 7269  ...opencv-contri
 00000520: 622d 7079 7468 6f6e 0d0a 0974 6966 6666  b-python...tifff
 00000530: 696c 650d 0a09 6835 7079 0d0a 096e 6170  ile...h5py...nap
 00000540: 6172 690d 0a09 7174 7079 0d0a 0970 796d  ari...qtpy...pym
 00000550: 6d63 6f72 652d 706c 7573 203e 3d20 302e  mcore-plus >= 0.
-00000560: 362e 370d 0a70 7974 686f 6e5f 7265 7175  6.7..python_requ
-00000570: 6972 6573 203d 203e 3d33 2e38 0d0a 7061  ires = >=3.8..pa
-00000580: 636b 6167 655f 6469 7220 3d20 0d0a 093d  ckage_dir = ...=
-00000590: 7372 630d 0a73 6574 7570 5f72 6571 7569  src..setup_requi
-000005a0: 7265 7320 3d20 0d0a 0973 6574 7570 746f  res = ...setupto
-000005b0: 6f6c 732d 7363 6d0d 0a0d 0a5b 6f70 7469  ols-scm....[opti
-000005c0: 6f6e 732e 7061 636b 6167 6573 2e66 696e  ons.packages.fin
-000005d0: 645d 0d0a 7768 6572 6520 3d20 7372 630d  d]..where = src.
-000005e0: 0a0d 0a5b 6f70 7469 6f6e 732e 656e 7472  ...[options.entr
-000005f0: 795f 706f 696e 7473 5d0d 0a6e 6170 6172  y_points]..napar
-00000600: 692e 6d61 6e69 6665 7374 203d 200d 0a09  i.manifest = ...
-00000610: 6e61 7061 7269 2d6c 6976 652d 7265 636f  napari-live-reco
-00000620: 7264 696e 6720 3d20 6e61 7061 7269 5f6c  rding = napari_l
-00000630: 6976 655f 7265 636f 7264 696e 673a 6e61  ive_recording:na
-00000640: 7061 7269 2e79 616d 6c0d 0a0d 0a5b 6f70  pari.yaml....[op
-00000650: 7469 6f6e 732e 7061 636b 6167 655f 6461  tions.package_da
-00000660: 7461 5d0d 0a6e 6170 6172 692d 6c69 7665  ta]..napari-live
-00000670: 2d72 6563 6f72 6469 6e67 203d 206e 6170  -recording = nap
-00000680: 6172 692e 7961 6d6c 0d0a 0d0a 5b65 6767  ari.yaml....[egg
-00000690: 5f69 6e66 6f5d 0d0a 7461 675f 6275 696c  _info]..tag_buil
-000006a0: 6420 3d20 0d0a 7461 675f 6461 7465 203d  d = ..tag_date =
-000006b0: 2030 0d0a 0d0a                            0....
+00000560: 362e 370d 0a09 7079 6d6d 636f 7265 2d77  6.7...pymmcore-w
+00000570: 6964 6765 7473 0d0a 7079 7468 6f6e 5f72  idgets..python_r
+00000580: 6571 7569 7265 7320 3d20 3e3d 332e 380d  equires = >=3.8.
+00000590: 0a70 6163 6b61 6765 5f64 6972 203d 200d  .package_dir = .
+000005a0: 0a09 3d73 7263 0d0a 7365 7475 705f 7265  ..=src..setup_re
+000005b0: 7175 6972 6573 203d 200d 0a09 7365 7475  quires = ...setu
+000005c0: 7074 6f6f 6c73 2d73 636d 0d0a 0d0a 5b6f  ptools-scm....[o
+000005d0: 7074 696f 6e73 2e70 6163 6b61 6765 732e  ptions.packages.
+000005e0: 6669 6e64 5d0d 0a77 6865 7265 203d 2073  find]..where = s
+000005f0: 7263 0d0a 0d0a 5b6f 7074 696f 6e73 2e65  rc....[options.e
+00000600: 6e74 7279 5f70 6f69 6e74 735d 0d0a 6e61  ntry_points]..na
+00000610: 7061 7269 2e6d 616e 6966 6573 7420 3d20  pari.manifest = 
+00000620: 0d0a 096e 6170 6172 692d 6c69 7665 2d72  ...napari-live-r
+00000630: 6563 6f72 6469 6e67 203d 206e 6170 6172  ecording = napar
+00000640: 695f 6c69 7665 5f72 6563 6f72 6469 6e67  i_live_recording
+00000650: 3a6e 6170 6172 692e 7961 6d6c 0d0a 0d0a  :napari.yaml....
+00000660: 5b6f 7074 696f 6e73 2e70 6163 6b61 6765  [options.package
+00000670: 5f64 6174 615d 0d0a 6e61 7061 7269 2d6c  _data]..napari-l
+00000680: 6976 652d 7265 636f 7264 696e 6720 3d20  ive-recording = 
+00000690: 6e61 7061 7269 2e79 616d 6c0d 0a0d 0a5b  napari.yaml....[
+000006a0: 6567 675f 696e 666f 5d0d 0a74 6167 5f62  egg_info]..tag_b
+000006b0: 7569 6c64 203d 200d 0a74 6167 5f64 6174  uild = ..tag_dat
+000006c0: 6520 3d20 300d 0a0d 0a                   e = 0....
```

### Comparing `napari-live-recording-0.3.0/src/napari_live_recording/__init__.py` & `napari-live-recording-0.3.2/src/napari_live_recording/__init__.py`

 * *Files identical despite different names*

### Comparing `napari-live-recording-0.3.0/src/napari_live_recording/common/__init__.py` & `napari-live-recording-0.3.2/src/napari_live_recording/common/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from __future__ import annotations
 from enum import IntEnum
 from dataclasses import dataclass
 from functools import total_ordering
-from tifffile.tifffile import PHOTOMETRIC
 import pymmcore_plus as mmc
 
 # equivalent number of milliseconds
 # for 30 Hz and 60 Hz refresh rates
 THIRTY_FPS = 33
 SIXTY_FPS = 16
 
@@ -23,38 +22,16 @@
 class ColorType(IntEnum):
     GRAYLEVEL = 0
     RGB = 1
 
 
 TIFF_PHOTOMETRIC_MAP = {
     # ColorType -> photometric, number of channels
-    ColorType.GRAYLEVEL: (PHOTOMETRIC.MINISBLACK, 1),
-    ColorType.RGB: (PHOTOMETRIC.RGB, 3),
-}
-
-
-@dataclass(frozen=True)
-class WriterInfo:
-    folder: str
-    filename: str
-    fileFormat: FileFormat
-    recordType: RecordType
-    stackSize: int = 0
-    acquisitionTime: float = 0
-
-
-class ColorType(IntEnum):
-    GRAYLEVEL = 0
-    RGB = 1
-
-
-TIFF_PHOTOMETRIC_MAP = {
-    # ColorType -> photometric, number of channels
-    ColorType.GRAYLEVEL: (PHOTOMETRIC.MINISBLACK, 1),
-    ColorType.RGB: (PHOTOMETRIC.RGB, 3),
+    ColorType.GRAYLEVEL: ("minisblack", 1),
+    ColorType.RGB: ("rgb", 3),
 }
 
 
 @dataclass(frozen=True)
 class WriterInfo:
     folder: str
     filename: str
```

### Comparing `napari-live-recording-0.3.0/src/napari_live_recording/control/__init__.py` & `napari-live-recording-0.3.2/src/napari_live_recording/control/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 import os
 from contextlib import contextmanager
 from napari.qt.threading import thread_worker, FunctionWorker
 from qtpy.QtCore import QThread, QObject, Signal
 from napari_live_recording.common import (
     TIFF_PHOTOMETRIC_MAP,
     WriterInfo,
-    FileFormat,
     RecordType, 
     ROI
 )
 from napari_live_recording.control.devices.interface import ICamera
 from typing import Dict, NamedTuple
 from functools import partial
 from time import time
```

### Comparing `napari-live-recording-0.3.0/src/napari_live_recording/control/devices/__init__.py` & `napari-live-recording-0.3.2/src/napari_live_recording/control/devices/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,17 +17,17 @@
         if module_name != "interface":
             module = import_module(f"{__name__}.{module_name}")
             for attr in getmembers(module, isclass):
                 # attr[0]: class name as string
                 # attr[1]: class object
                 if attr[1] != ICamera and issubclass(attr[1], ICamera):
                     devicesDict[attr[0]] = attr[1]
-    except ImportError:
+    except ImportError as e:
         # This check is added to make sure that modules from cameras
         # which must be added manually (i.e. Ximea's APIs) do not 
         # cause issues when loading the plugin.
         # The camera won't be visibile in the supported camera list
         # but the plugin will still be working as expected.
         # In case there are cameras which require external components,
         # remember to wrap them in a try-except snippet and raise an
         # ImportError exception if there is any missing package.
-        raise TypeError(f"Importing of {module_name} failed. Check napari's traceback for more informations.")
+        raise TypeError(f"Importing of {module_name} failed. Check napari's traceback for more informations. Exception: {e}")
```

### Comparing `napari-live-recording-0.3.0/src/napari_live_recording/control/devices/interface.py` & `napari-live-recording-0.3.2/src/napari_live_recording/control/devices/interface.py`

 * *Files identical despite different names*

### Comparing `napari-live-recording-0.3.0/src/napari_live_recording/control/devices/micro_manager.py` & `napari-live-recording-0.3.2/src/napari_live_recording/control/devices/micro_manager.py`

 * *Files identical despite different names*

### Comparing `napari-live-recording-0.3.0/src/napari_live_recording/control/devices/opencv.py` & `napari-live-recording-0.3.2/src/napari_live_recording/control/devices/opencv.py`

 * *Files identical despite different names*

### Comparing `napari-live-recording-0.3.0/src/napari_live_recording/ui/__init__.py` & `napari-live-recording-0.3.2/src/napari_live_recording/ui/__init__.py`

 * *Files identical despite different names*

### Comparing `napari-live-recording-0.3.0/src/napari_live_recording/ui/widgets.py` & `napari-live-recording-0.3.2/src/napari_live_recording/ui/widgets.py`

 * *Files identical despite different names*

### Comparing `napari-live-recording-0.3.0/src/napari_live_recording.egg-info/PKG-INFO` & `napari-live-recording-0.3.2/src/napari_live_recording.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-live-recording
-Version: 0.3.0
+Version: 0.3.2
 Summary: A napari plugin for live video recording with a generic camera device.
 Home-page: https://github.com/jethro33/napari-live-recording
 Author: Jacopo Abramo
 Author-email: jacopo.abramo@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/jacopoabramo/napari-live-recording/issues
 Project-URL: Documentation, https://github.com/jacopoabramo/napari-live-recording#README.md
```

### Comparing `napari-live-recording-0.3.0/src/napari_live_recording.egg-info/SOURCES.txt` & `napari-live-recording-0.3.2/src/napari_live_recording.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `napari-live-recording-0.3.0/tox.ini` & `napari-live-recording-0.3.2/tox.ini`

 * *Files identical despite different names*

