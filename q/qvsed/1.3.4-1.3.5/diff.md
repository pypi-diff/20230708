# Comparing `tmp/qvsed-1.3.4.tar.gz` & `tmp/qvsed-1.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qvsed-1.3.4.tar", last modified: Sat Jul  8 19:30:44 2023, max compression
+gzip compressed data, was "qvsed-1.3.5.tar", last modified: Sat Jul  8 21:15:15 2023, max compression
```

## Comparing `qvsed-1.3.4.tar` & `qvsed-1.3.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-07-08 19:30:44.155598 qvsed-1.3.4/
--rw-rw-rw-   0        0        0    35823 2023-07-06 15:36:27.000000 qvsed-1.3.4/LICENSE.txt
--rw-rw-rw-   0        0        0       57 2023-07-07 19:12:44.000000 qvsed-1.3.4/MANIFEST.in
--rw-rw-rw-   0        0        0     1263 2023-07-08 19:30:44.155598 qvsed-1.3.4/PKG-INFO
--rw-rw-rw-   0        0        0     6070 2023-07-08 17:32:53.000000 qvsed-1.3.4/README.md
-drwxrwxrwx   0        0        0        0 2023-07-08 19:30:44.139335 qvsed-1.3.4/qvsed/
--rw-rw-rw-   0        0        0       50 2023-07-06 20:42:20.000000 qvsed-1.3.4/qvsed/__init__.py
--rw-rw-rw-   0        0        0      597 2023-07-08 15:55:18.000000 qvsed-1.3.4/qvsed/config_default.py
--rw-rw-rw-   0        0        0    14675 2023-07-08 19:30:13.000000 qvsed-1.3.4/qvsed/qvsed.py
--rw-rw-rw-   0        0        0    21342 2023-07-08 18:13:57.000000 qvsed-1.3.4/qvsed/qvsed.ui
-drwxrwxrwx   0        0        0        0 2023-07-08 19:30:44.153361 qvsed-1.3.4/qvsed.egg-info/
--rw-rw-rw-   0        0        0     1263 2023-07-08 19:30:44.000000 qvsed-1.3.4/qvsed.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      290 2023-07-08 19:30:44.000000 qvsed-1.3.4/qvsed.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-08 19:30:44.000000 qvsed-1.3.4/qvsed.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2023-07-08 19:30:44.000000 qvsed-1.3.4/qvsed.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        6 2023-07-08 19:30:44.000000 qvsed-1.3.4/qvsed.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-07-08 19:30:44.000000 qvsed-1.3.4/qvsed.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-08 19:30:44.155598 qvsed-1.3.4/setup.cfg
--rw-rw-rw-   0        0        0     1633 2023-07-08 19:30:40.000000 qvsed-1.3.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-08 21:15:15.680575 qvsed-1.3.5/
+-rw-rw-rw-   0        0        0    35823 2023-07-06 15:36:27.000000 qvsed-1.3.5/LICENSE.txt
+-rw-rw-rw-   0        0        0       57 2023-07-08 21:12:53.000000 qvsed-1.3.5/MANIFEST.in
+-rw-rw-rw-   0        0        0     1263 2023-07-08 21:15:15.679403 qvsed-1.3.5/PKG-INFO
+-rw-rw-rw-   0        0        0     6070 2023-07-08 17:32:53.000000 qvsed-1.3.5/README.md
+drwxrwxrwx   0        0        0        0 2023-07-08 21:15:15.669752 qvsed-1.3.5/qvsed/
+-rw-rw-rw-   0        0        0       50 2023-07-08 20:05:55.000000 qvsed-1.3.5/qvsed/__init__.py
+-rw-rw-rw-   0        0        0      383 2023-07-08 21:13:12.000000 qvsed-1.3.5/qvsed/config_default.py
+-rw-rw-rw-   0        0        0    14233 2023-07-08 21:14:48.000000 qvsed-1.3.5/qvsed/qvsed.py
+-rw-rw-rw-   0        0        0     9193 2023-07-08 21:06:50.000000 qvsed-1.3.5/qvsed/qvsed.ui
+drwxrwxrwx   0        0        0        0 2023-07-08 21:15:15.678395 qvsed-1.3.5/qvsed.egg-info/
+-rw-rw-rw-   0        0        0     1263 2023-07-08 21:15:15.000000 qvsed-1.3.5/qvsed.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      290 2023-07-08 21:15:15.000000 qvsed-1.3.5/qvsed.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-08 21:15:15.000000 qvsed-1.3.5/qvsed.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2023-07-08 21:15:15.000000 qvsed-1.3.5/qvsed.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        6 2023-07-08 21:15:15.000000 qvsed-1.3.5/qvsed.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-07-08 21:15:15.000000 qvsed-1.3.5/qvsed.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-08 21:15:15.680575 qvsed-1.3.5/setup.cfg
+-rw-rw-rw-   0        0        0     1633 2023-07-08 21:12:36.000000 qvsed-1.3.5/setup.py
```

### Comparing `qvsed-1.3.4/LICENSE.txt` & `qvsed-1.3.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `qvsed-1.3.4/PKG-INFO` & `qvsed-1.3.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qvsed
-Version: 1.3.4
+Version: 1.3.5
 Summary: Qt-Based Volatile Small Editor
 Home-page: https://github.com/That1M8Head/QVSED/
 Author: Arsalan Kazmi
 License: GPL-3.0-or-later
 License-File: LICENSE.txt
 
 QVSED is a volatile and small text editor.
```

### Comparing `qvsed-1.3.4/README.md` & `qvsed-1.3.5/README.md`

 * *Files identical despite different names*

### Comparing `qvsed-1.3.4/qvsed/qvsed.py` & `qvsed-1.3.5/qvsed/qvsed.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,16 @@
 See README.md or "Get Help" inside QVSED for more info
 """
 
 # pylint: disable=no-name-in-module
 # pylint: disable=attribute-defined-outside-init
 # pylint: disable=broad-exception-caught
 
-import os, sys
+import os
+import sys
 import shutil
 import importlib.util
 import pkg_resources
 from PyQt5.QtWidgets import (
     QApplication, QMainWindow, QPushButton, QWidget,
     QFileDialog, QPlainTextEdit, QLineEdit,
     QAction, QShortcut
@@ -52,66 +53,72 @@
         Initialize the QVSED window.
         """
         super().__init__()
         self.load_ui_file()
         self.focus_text_area()
         self.set_text_area_encoding("UTF-8")
         self.set_up_action_deck()
+        self.echo_area_update(f"Welcome to QVSED v{self.get_qvsed_version()}!")
         self.load_config()
         self.set_up_fonts()
-        self.echo_area_update(f"Welcome to QVSED v{self.get_qvsed_version()}!")
         if self.check_if_file_parameter():
             self.load_from_file(sys.argv[1])
 
-    def apply_style_sheet(self):
+    def apply_style_sheet(self, text_color, background_color, button_color, button_focus_color):
         """
         Generate and apply a style sheet based on the config.py file.
         """
 
-        stylesheet = f"""QMainWindow, QLabel, QPushButton, #textArea, #echoArea {{
-    color: {self.text_color};
-    background: {self.background_color};
+        stylesheet = f"""
+QPlainTextEdit, QLineEdit {{
+    background: {button_focus_color};
+    border: 2px solid {button_color};
 }}
 
-QWidget#centralwidget QPushButton {{
-    border: 2px solid #31353f;
-    background: {self.button_background_color};
+QPushButton {{
+    border: 2px solid {button_focus_color};
+    background: {button_color};
     padding: 2px;
 }}
 
-QWidget#centralwidget QPushButton:hover {{
-    background: {self.button_hover_background_color};
+QPushButton:hover {{
+    background: {button_focus_color};
 }}
 
-QWidget#centralwidget QPushButton:pressed {{
-    background: {self.button_pressed_background_color};
+QPushButton:pressed {{
+    background: {background_color};
 }}
 
 QScrollBar:vertical {{
-    background-color: {self.scrollbar_background_color};
+    background-color: {button_focus_color};
     width: 16px;
     margin: 16px 0 16px 0;
 }}
 
 QScrollBar::handle:vertical {{
-    background-color: {self.scrollbar_handle_background_color};
+    background-color: {button_color};
     min-height: 20px;
 }}
 
 QScrollBar::handle:vertical:hover {{
-    background-color: {self.scrollbar_handle_hover_background_color};
+    background-color: {button_color};
 }}
 
 QScrollBar::add-line:vertical, QScrollBar::sub-line:vertical {{
     background: none;
 }}
 
 QScrollBar::add-page:vertical, QScrollBar::sub-page:vertical {{
     background: none;
 }}
+
+QMainWindow {{
+    color: {text_color};
+    background: {background_color};
+}}
         """
 
         # Apply the stylesheet to the app
         self.setStyleSheet(stylesheet)
 
     def check_if_file_parameter(self):
         """
@@ -235,23 +242,19 @@
 
         self.font_family = qvsed_config.font_family
         self.font_size = qvsed_config.font_size
 
         # Load the colour scheme settings from the config file
         # We use the shorter American spellings because it's standard, I guess
         try:
-            self.text_color = qvsed_config.text_color
-            self.background_color = qvsed_config.background_color
-            self.button_background_color = qvsed_config.button_background_color
-            self.button_hover_background_color = qvsed_config.button_hover_background_color
-            self.button_pressed_background_color = qvsed_config.button_pressed_background_color
-            self.scrollbar_background_color = qvsed_config.scrollbar_background_color
-            self.scrollbar_handle_background_color = qvsed_config.scrollbar_handle_background_color
-            self.scrollbar_handle_hover_background_color = qvsed_config.scrollbar_handle_hover_background_color
-            self.apply_style_sheet()
+            text_color = qvsed_config.text_color
+            background_color = qvsed_config.background_color
+            button_color = qvsed_config.button_color
+            button_focus_color = qvsed_config.button_focus_color
+            self.apply_style_sheet(text_color, background_color, button_color, button_focus_color)
         except AttributeError as error:
             self.echo_area_update(f"Check config.py: {str(error)}")
 
     def load_from_file(self, file_path = None):
         """
         Open a file dialog, and load the contents of a file into the Text Area.
         """
```

### Comparing `qvsed-1.3.4/qvsed.egg-info/PKG-INFO` & `qvsed-1.3.5/qvsed.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qvsed
-Version: 1.3.4
+Version: 1.3.5
 Summary: Qt-Based Volatile Small Editor
 Home-page: https://github.com/That1M8Head/QVSED/
 Author: Arsalan Kazmi
 License: GPL-3.0-or-later
 License-File: LICENSE.txt
 
 QVSED is a volatile and small text editor.
```

### Comparing `qvsed-1.3.4/setup.py` & `qvsed-1.3.5/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 The setup.py file for QVSED.
 """
 from setuptools import setup, find_packages
 
 setup(
     name='qvsed',
-    version='1.3.4',
+    version='1.3.5',
     author='Arsalan Kazmi',
     description='Qt-Based Volatile Small Editor',
     long_description="""QVSED is a volatile and small text editor.
 
 "Volatile" means that QVSED is entirely stateless - once you open a file, QVSED doesn't store any file paths or any other data other than the text contents of the file you loaded.
 Additionally, QVSED won't prompt you if you're about to potentially lose an unsaved file, since it doesn't know of any file metadata.
 You may be prompted if you're about to overwrite a file, but that's up to your OS, not QVSED.
```

