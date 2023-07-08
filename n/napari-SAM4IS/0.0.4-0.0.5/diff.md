# Comparing `tmp/napari-SAM4IS-0.0.4.tar.gz` & `tmp/napari-SAM4IS-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "napari-SAM4IS-0.0.4.tar", last modified: Mon May  1 06:31:34 2023, max compression
+gzip compressed data, was "napari-SAM4IS-0.0.5.tar", last modified: Sat Jul  8 11:11:21 2023, max compression
```

## Comparing `napari-SAM4IS-0.0.4.tar` & `napari-SAM4IS-0.0.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 hiroki     (501) staff       (20)        0 2023-05-01 06:31:34.798148 napari-SAM4IS-0.0.4/
--rw-r--r--   0 hiroki     (501) staff       (20)    11358 2023-04-23 07:36:32.000000 napari-SAM4IS-0.0.4/LICENSE
--rw-r--r--   0 hiroki     (501) staff       (20)       96 2023-04-23 07:36:32.000000 napari-SAM4IS-0.0.4/MANIFEST.in
--rw-r--r--   0 hiroki     (501) staff       (20)     7487 2023-05-01 06:31:34.798259 napari-SAM4IS-0.0.4/PKG-INFO
--rw-r--r--   0 hiroki     (501) staff       (20)     6202 2023-04-30 03:47:39.000000 napari-SAM4IS-0.0.4/README.md
--rw-r--r--   0 hiroki     (501) staff       (20)     1177 2023-04-23 07:36:32.000000 napari-SAM4IS-0.0.4/pyproject.toml
--rw-r--r--   0 hiroki     (501) staff       (20)     1764 2023-05-01 06:31:34.798689 napari-SAM4IS-0.0.4/setup.cfg
-drwxr-xr-x   0 hiroki     (501) staff       (20)        0 2023-05-01 06:31:34.795024 napari-SAM4IS-0.0.4/src/
-drwxr-xr-x   0 hiroki     (501) staff       (20)        0 2023-05-01 06:31:34.796532 napari-SAM4IS-0.0.4/src/napari_SAM4IS.egg-info/
--rw-r--r--   0 hiroki     (501) staff       (20)     7487 2023-05-01 06:31:34.000000 napari-SAM4IS-0.0.4/src/napari_SAM4IS.egg-info/PKG-INFO
--rw-r--r--   0 hiroki     (501) staff       (20)      496 2023-05-01 06:31:34.000000 napari-SAM4IS-0.0.4/src/napari_SAM4IS.egg-info/SOURCES.txt
--rw-r--r--   0 hiroki     (501) staff       (20)        1 2023-05-01 06:31:34.000000 napari-SAM4IS-0.0.4/src/napari_SAM4IS.egg-info/dependency_links.txt
--rw-r--r--   0 hiroki     (501) staff       (20)       60 2023-05-01 06:31:34.000000 napari-SAM4IS-0.0.4/src/napari_SAM4IS.egg-info/entry_points.txt
--rw-r--r--   0 hiroki     (501) staff       (20)      107 2023-05-01 06:31:34.000000 napari-SAM4IS-0.0.4/src/napari_SAM4IS.egg-info/requires.txt
--rw-r--r--   0 hiroki     (501) staff       (20)       14 2023-05-01 06:31:34.000000 napari-SAM4IS-0.0.4/src/napari_SAM4IS.egg-info/top_level.txt
-drwxr-xr-x   0 hiroki     (501) staff       (20)        0 2023-05-01 06:31:34.797407 napari-SAM4IS-0.0.4/src/napari_sam4is/
--rw-r--r--   0 hiroki     (501) staff       (20)       85 2023-05-01 06:31:21.000000 napari-SAM4IS-0.0.4/src/napari_sam4is/__init__.py
-drwxr-xr-x   0 hiroki     (501) staff       (20)        0 2023-05-01 06:31:34.797803 napari-SAM4IS-0.0.4/src/napari_sam4is/_tests/
--rw-r--r--   0 hiroki     (501) staff       (20)        0 2023-04-23 07:36:32.000000 napari-SAM4IS-0.0.4/src/napari_sam4is/_tests/__init__.py
--rw-r--r--   0 hiroki     (501) staff       (20)     1246 2023-04-23 07:36:32.000000 napari-SAM4IS-0.0.4/src/napari_sam4is/_tests/test_widget.py
--rw-r--r--   0 hiroki     (501) staff       (20)     4710 2023-05-01 06:20:29.000000 napari-SAM4IS-0.0.4/src/napari_sam4is/_utils.py
--rw-r--r--   0 hiroki     (501) staff       (20)    12071 2023-05-01 06:27:14.000000 napari-SAM4IS-0.0.4/src/napari_sam4is/_widget.py
--rw-r--r--   0 hiroki     (501) staff       (20)      282 2023-04-24 04:30:49.000000 napari-SAM4IS-0.0.4/src/napari_sam4is/napari.yaml
+drwxr-xr-x   0 hiroki     (501) staff       (20)        0 2023-07-08 11:11:21.304920 napari-SAM4IS-0.0.5/
+-rw-r--r--   0 hiroki     (501) staff       (20)    11358 2023-04-23 07:36:32.000000 napari-SAM4IS-0.0.5/LICENSE
+-rw-r--r--   0 hiroki     (501) staff       (20)       96 2023-04-23 07:36:32.000000 napari-SAM4IS-0.0.5/MANIFEST.in
+-rw-r--r--   0 hiroki     (501) staff       (20)     7487 2023-07-08 11:11:21.304991 napari-SAM4IS-0.0.5/PKG-INFO
+-rw-r--r--   0 hiroki     (501) staff       (20)     6202 2023-04-30 03:47:39.000000 napari-SAM4IS-0.0.5/README.md
+-rw-r--r--   0 hiroki     (501) staff       (20)     1177 2023-04-23 07:36:32.000000 napari-SAM4IS-0.0.5/pyproject.toml
+-rw-r--r--   0 hiroki     (501) staff       (20)     1764 2023-07-08 11:11:21.305326 napari-SAM4IS-0.0.5/setup.cfg
+drwxr-xr-x   0 hiroki     (501) staff       (20)        0 2023-07-08 11:11:21.302364 napari-SAM4IS-0.0.5/src/
+drwxr-xr-x   0 hiroki     (501) staff       (20)        0 2023-07-08 11:11:21.304069 napari-SAM4IS-0.0.5/src/napari_SAM4IS.egg-info/
+-rw-r--r--   0 hiroki     (501) staff       (20)     7487 2023-07-08 11:11:21.000000 napari-SAM4IS-0.0.5/src/napari_SAM4IS.egg-info/PKG-INFO
+-rw-r--r--   0 hiroki     (501) staff       (20)      496 2023-07-08 11:11:21.000000 napari-SAM4IS-0.0.5/src/napari_SAM4IS.egg-info/SOURCES.txt
+-rw-r--r--   0 hiroki     (501) staff       (20)        1 2023-07-08 11:11:21.000000 napari-SAM4IS-0.0.5/src/napari_SAM4IS.egg-info/dependency_links.txt
+-rw-r--r--   0 hiroki     (501) staff       (20)       60 2023-07-08 11:11:21.000000 napari-SAM4IS-0.0.5/src/napari_SAM4IS.egg-info/entry_points.txt
+-rw-r--r--   0 hiroki     (501) staff       (20)      107 2023-07-08 11:11:21.000000 napari-SAM4IS-0.0.5/src/napari_SAM4IS.egg-info/requires.txt
+-rw-r--r--   0 hiroki     (501) staff       (20)       14 2023-07-08 11:11:21.000000 napari-SAM4IS-0.0.5/src/napari_SAM4IS.egg-info/top_level.txt
+drwxr-xr-x   0 hiroki     (501) staff       (20)        0 2023-07-08 11:11:21.304540 napari-SAM4IS-0.0.5/src/napari_sam4is/
+-rw-r--r--   0 hiroki     (501) staff       (20)       85 2023-07-08 10:30:24.000000 napari-SAM4IS-0.0.5/src/napari_sam4is/__init__.py
+drwxr-xr-x   0 hiroki     (501) staff       (20)        0 2023-07-08 11:11:21.304746 napari-SAM4IS-0.0.5/src/napari_sam4is/_tests/
+-rw-r--r--   0 hiroki     (501) staff       (20)        0 2023-04-23 07:36:32.000000 napari-SAM4IS-0.0.5/src/napari_sam4is/_tests/__init__.py
+-rw-r--r--   0 hiroki     (501) staff       (20)     1246 2023-04-23 07:36:32.000000 napari-SAM4IS-0.0.5/src/napari_sam4is/_tests/test_widget.py
+-rw-r--r--   0 hiroki     (501) staff       (20)     5083 2023-07-08 10:49:47.000000 napari-SAM4IS-0.0.5/src/napari_sam4is/_utils.py
+-rw-r--r--   0 hiroki     (501) staff       (20)    15086 2023-07-08 11:07:40.000000 napari-SAM4IS-0.0.5/src/napari_sam4is/_widget.py
+-rw-r--r--   0 hiroki     (501) staff       (20)      282 2023-04-24 04:30:49.000000 napari-SAM4IS-0.0.5/src/napari_sam4is/napari.yaml
```

### Comparing `napari-SAM4IS-0.0.4/LICENSE` & `napari-SAM4IS-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `napari-SAM4IS-0.0.4/PKG-INFO` & `napari-SAM4IS-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-SAM4IS
-Version: 0.0.4
+Version: 0.0.5
 Summary: Create annotations for instance segmentation using Segment Anything models
 Home-page: https://github.com/hiroalchem/napari-SAM4IS
 Author: Hiroki Kawai
 Author-email: h.kawai888@gmail.com
 License: Apache-2.0
 Project-URL: Bug Tracker, https://github.com/hiroalchem/napari-SAM4IS/issues
 Project-URL: Documentation, https://github.com/hiroalchem/napari-SAM4IS#README.md
```

### Comparing `napari-SAM4IS-0.0.4/README.md` & `napari-SAM4IS-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `napari-SAM4IS-0.0.4/pyproject.toml` & `napari-SAM4IS-0.0.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `napari-SAM4IS-0.0.4/setup.cfg` & `napari-SAM4IS-0.0.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `napari-SAM4IS-0.0.4/src/napari_SAM4IS.egg-info/PKG-INFO` & `napari-SAM4IS-0.0.5/src/napari_SAM4IS.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-SAM4IS
-Version: 0.0.4
+Version: 0.0.5
 Summary: Create annotations for instance segmentation using Segment Anything models
 Home-page: https://github.com/hiroalchem/napari-SAM4IS
 Author: Hiroki Kawai
 Author-email: h.kawai888@gmail.com
 License: Apache-2.0
 Project-URL: Bug Tracker, https://github.com/hiroalchem/napari-SAM4IS/issues
 Project-URL: Documentation, https://github.com/hiroalchem/napari-SAM4IS#README.md
```

### Comparing `napari-SAM4IS-0.0.4/src/napari_sam4is/_tests/test_widget.py` & `napari-SAM4IS-0.0.5/src/napari_sam4is/_tests/test_widget.py`

 * *Files identical despite different names*

### Comparing `napari-SAM4IS-0.0.4/src/napari_sam4is/_utils.py` & `napari-SAM4IS-0.0.5/src/napari_sam4is/_utils.py`

 * *Files 23% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import numpy as np
 from segment_anything import sam_model_registry
 from skimage.color import gray2rgb, rgba2rgb
 from skimage.draw import polygon2mask
 from skimage.measure import find_contours
 
 
-def load_model(model_name):
+def load_model(model_name: str = 'default') -> sam_model_registry:
     """Load model
 
     Args:
         model_name (str): model name
 
     :return: model
     """
@@ -25,15 +25,15 @@
     os.makedirs(os.path.dirname(model_path), exist_ok=True)
     if not os.path.exists(model_path):
         autodownload(model_url)
     sam = sam_model_registry[model_name](checkpoint=model_path)
     return sam
 
 
-def autodownload(model_url):
+def autodownload(model_url: str):
     """Download model
 
     Args:
         model_url (str): model url
 
     """
 
@@ -137,7 +137,19 @@
     json = {
         "images": images,
         "annotations": annotations,
         "categories": categories
     }
     return json
 
+
+def find_first_missing(arr):
+    arr = np.unique(arr)  # remove duplicates
+    arr = arr[arr >= 0]  # keep only positive values and zero
+    arr.sort()  # sort the array
+
+    # check for missing integers
+    for index, value in np.ndenumerate(arr):
+        if index[0] != value:
+            return index[0]
+    return len(arr)
+
```

### Comparing `napari-SAM4IS-0.0.4/src/napari_sam4is/_widget.py` & `napari-SAM4IS-0.0.5/src/napari_sam4is/_widget.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 import json
 import os
 
 import napari
 import numpy as np
 import torch
-from qtpy.QtWidgets import QVBoxLayout, QPushButton, QWidget, QComboBox, QLabel, QButtonGroup, QRadioButton
+from qtpy.QtWidgets import QVBoxLayout, QPushButton, QWidget, QComboBox, QLabel, QButtonGroup, QRadioButton, QCheckBox
 from segment_anything import sam_model_registry, SamPredictor
 
-from ._utils import load_model, preprocess, label2polygon, create_json, check_image_type
+from ._utils import load_model, preprocess, label2polygon, create_json, check_image_type, find_first_missing
 
 
 class SAMWidget(QWidget):
     def __init__(self, napari_viewer):
         super().__init__()
         self._viewer = napari_viewer
 
         self._shapes_layer_selection = None
         self._labels_layer_selection = None
         self._image_type = None
         self._current_slice = None
+        self._input_box = None
+        self._input_point = None
+        self._point_label = None
 
         #self._corner = None
 
         self.vbox = QVBoxLayout()
         self._model_selection = QComboBox()
         self._model_selection.addItems(list(sam_model_registry.keys()))
         self.vbox.addWidget(self._model_selection)
@@ -31,26 +34,30 @@
         self.vbox.addWidget(self._model_load_btn)
         self.vbox.addWidget(QLabel("input image layer"))
         self._image_layer_selection = QComboBox()
         self._image_layer_selection.addItems([layer.name for layer in self._viewer.layers if isinstance(layer, napari.layers.image.image.Image)])
         self._image_layer_selection.currentTextChanged.connect(self._on_image_layer_changed)
         self.vbox.addWidget(self._image_layer_selection)
 
-        self.vbox.addWidget(QLabel("select output layer type \nif you want to use the output\nas a mask, select 'semantic'.\n"
-                                   "3D image is currently only\nsupported for 'semantic'"))
+        self.vbox.addWidget(QLabel("select output layer type \nif you want to use the output\n"
+                                   "as a mask, select 'labels'.\n"
+                                   "3D image is currently only\nsupported for 'labels'"))
         self._radio_btn_group = QButtonGroup()
         self._radio_btn_shape = QRadioButton("instance (Shapes layer)")
         self._radio_btn_shape.toggled.connect(self._on_radio_btn_toggled)
-        self._radio_btn_label = QRadioButton("semantic (Labels layer)")
+        self._radio_btn_label = QRadioButton("labels (Labels layer)")
         self._radio_btn_label.toggled.connect(self._on_radio_btn_toggled)
         self._radio_btn_group.addButton(self._radio_btn_shape, 0)
         self._radio_btn_group.addButton(self._radio_btn_label, 1)
         self.vbox.addWidget(self._radio_btn_shape)
         self.vbox.addWidget(self._radio_btn_label)
 
+        self.check_box = QCheckBox("instance labels")
+        self.vbox.addWidget(self.check_box)
+
         self.vbox.addWidget(QLabel("output shapes layer"))
         self._shapes_layer_selection = QComboBox()
         self._shapes_layer_selection.addItems([layer.name for layer in self._viewer.layers if isinstance(layer, napari.layers.shapes.shapes.Shapes)])
         self.vbox.addWidget(self._shapes_layer_selection)
 
         self.vbox.addWidget(QLabel("output labels layer"))
         self._labels_layer_selection = QComboBox()
@@ -66,14 +73,20 @@
         self._test_btn.clicked.connect(self.print_corner_value)
         self.vbox.addWidget(self._test_btn)
         """
 
         self._sam_box_layer = self._viewer.add_shapes(name="SAM-Box", edge_color="red", edge_width=2, face_color="transparent")
         self._sam_box_layer.mouse_drag_callbacks.append(self._on_sam_box_created)
         self.lock_controls(self._sam_box_layer)
+        self._sam_positive_point_layer = self._viewer.add_points(name="SAM-Positive", face_color="green", size=10)
+        self._sam_negative_point_layer = self._viewer.add_points(name="SAM-Negative", face_color="red", size=10)
+        #self._sam_positive_point_layer.mouse_drag_callbacks.append(self._on_sam_point_created)
+        #self._sam_negative_point_layer.mouse_drag_callbacks.append(self._on_sam_point_created)
+        self._sam_positive_point_layer.events.data.connect(self._on_sam_point_changed)
+        self._sam_negative_point_layer.events.data.connect(self._on_sam_point_changed)
 
         if self._image_layer_selection.currentText() != "":
             self._image_type = check_image_type(self._viewer, self._image_layer_selection.currentText())
             if "stack" in self._image_type:
                 shape = self._viewer.layers[self._image_layer_selection.currentText()].data.shape[1:3]
             else :
                 shape = self._viewer.layers[self._image_layer_selection.currentText()].data.shape[:2]
@@ -121,19 +134,24 @@
         button_id = self._radio_btn_group.checkedId()
         if (self._shapes_layer_selection is not None) & (self._labels_layer_selection is not None):
             if button_id == 0:
                 self._shapes_layer_selection.clear()
                 self._shapes_layer_selection.addItems([layer.name for layer in self._viewer.layers if (isinstance(layer, napari.layers.shapes.shapes.Shapes))&(layer.name != self._sam_box_layer.name)])
                 self._labels_layer_selection.clear()
                 self._save_btn.setEnabled(True)
+                self.check_box.setEnabled(False)
+                self.check_box.setStyleSheet("text-decoration: line-through")
+
             else:
                 self._labels_layer_selection.clear()
                 self._labels_layer_selection.addItems([layer.name for layer in self._viewer.layers if (isinstance(layer, napari.layers.labels.labels.Labels))&(layer.name != self._labels_layer.name)])
                 self._shapes_layer_selection.clear()
                 self._save_btn.setEnabled(False)
+                self.check_box.setEnabled(True)
+                self.check_box.setStyleSheet("text-decoration: none")
 
     def _load_model(self):
         model_name = self._model_selection.currentText()
         self._sam_model = load_model(model_name)
         self._sam_model.to(device=self.device)
         self.sam_predictor = SamPredictor(self._sam_model)
         print("model loaded")
@@ -168,26 +186,55 @@
             else:
                 pass
             coords = self._sam_box_layer.data[0]
             y1 = int(coords[0][0])
             x1 = int(coords[0][1])
             y2 = int(coords[2][0])
             x2 = int(coords[2][1])
-            print(x1, y1, x2, y2)
-            input_box = np.array([x1, y1, x2, y2])
-            if self.sam_predictor is not None:
-                masks, _, _ = self.sam_predictor.predict(
-                    point_coords=None,
-                    point_labels=None,
-                    box=input_box[None, :],
-                    multimask_output=False,
-                )
-                self._labels_layer.data = masks[0] * 1
+            print(f"x1 = {x1}, y1 = {y1}, x2 = {x2}, y2 = {y2}")
+            self._input_box = np.array([x1, y1, x2, y2])
+            self._create_input_point()
+            self._predict()
             self._sam_box_layer.data = []
-            self._viewer.layers.selection.active = self._labels_layer
+
+    def _on_sam_point_changed(self):
+        if (len(self._sam_positive_point_layer.data) != 0) or (self._input_box is not None):
+            if "stack" in self._image_type:
+                if self._current_slice == self._viewer.dims.current_step[0]:
+                    pass
+                else:
+                    self._on_image_layer_changed(None)
+            else:
+                pass
+            self._create_input_point()
+            self._predict()
+
+    def _predict(self):
+        if self.sam_predictor is not None:
+            masks, _, _ = self.sam_predictor.predict(
+                point_coords=self._input_point,
+                point_labels=self._point_label,
+                box=self._input_box[None, :] if self._input_box is not None else None,
+                multimask_output=False,
+            )
+            self._labels_layer.data = masks[0] * 1
+        self._viewer.layers.selection.active = self._labels_layer
+
+
+    def _create_input_point(self):
+        positive_points = self._sam_positive_point_layer.data
+        negative_points = self._sam_negative_point_layer.data
+        if len(positive_points) + len(negative_points) == 0:
+            self._input_point = None
+            self._point_label = None
+            return
+        self._point_label = np.array(len(positive_points) * [1] + len(negative_points) * [0])
+        coords = np.concatenate((positive_points, negative_points), axis=0)
+        self._input_point = coords[:, ::-1].astype(np.int32)
+
 
     def _accept_mask(self, layer):
         button_id = self._radio_btn_group.checkedId()
         if button_id == 0:
             if self._shapes_layer_selection.currentText() != "":
                 output_layer = self._viewer.layers[self._shapes_layer_selection.currentText()]
                 if isinstance(output_layer, napari.layers.shapes.shapes.Shapes):
@@ -198,26 +245,42 @@
             else:
                 pass
         else:
             if self._labels_layer_selection.currentText() != "":
                 output_layer = self._viewer.layers[self._labels_layer_selection.currentText()]
                 if isinstance(output_layer, napari.layers.labels.labels.Labels):
                     if self._current_slice is not None:
-                        output_layer.data[self._current_slice] = output_layer.data[self._current_slice] | self._labels_layer.data
+                        if self.check_box.isChecked():
+                            num = find_first_missing(output_layer.data[self._current_slice])
+                        else:
+                            num = 1
+                        output_layer.data[self._current_slice] = output_layer.data[self._current_slice] | self._labels_layer.data * num
                         output_layer.refresh()
                     else:
-                        output_layer.data = output_layer.data | self._labels_layer.data
+                        if self.check_box.isChecked():
+                            num = find_first_missing(output_layer.data)
+                        else:
+                            num = 1
+                        output_layer.data = output_layer.data | self._labels_layer.data * num
                     self._viewer.layers.selection.active = self._sam_box_layer
                 else:
                     pass
         self._labels_layer.data = np.zeros_like(self._labels_layer.data)
+        self._input_box = None
+        self._sam_positive_point_layer.data = []
+        self._sam_negative_point_layer.data = []
+        self._input_point = None
+        self._point_label = None
 
     def _reject_mask(self, layer):
         self._labels_layer.data = np.zeros_like(self._labels_layer.data)
         self._viewer.layers.selection.active = self._sam_box_layer
+        self._input_box = None
+        self._sam_positive_point_layer.data = []
+        self._sam_negative_point_layer.data = []
 
     def _save(self):
         if self._shapes_layer_selection.currentText() != "":
             image_layer = self._viewer.layers[self._image_layer_selection.currentText()]
             image_path = image_layer.source.path
             image_name = os.path.basename(image_path)
             output_layer = self._viewer.layers[self._shapes_layer_selection.currentText()]
```

