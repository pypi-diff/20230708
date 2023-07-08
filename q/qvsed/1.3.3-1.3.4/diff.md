# Comparing `tmp/qvsed-1.3.3.tar.gz` & `tmp/qvsed-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qvsed-1.3.3.tar", last modified: Sat Jul  8 18:18:39 2023, max compression
+gzip compressed data, was "qvsed-1.3.4.tar", last modified: Sat Jul  8 19:30:44 2023, max compression
```

## Comparing `qvsed-1.3.3.tar` & `qvsed-1.3.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-07-08 18:18:39.756590 qvsed-1.3.3/
--rw-rw-rw-   0        0        0    35823 2023-07-06 15:36:27.000000 qvsed-1.3.3/LICENSE.txt
--rw-rw-rw-   0        0        0       57 2023-07-07 19:12:44.000000 qvsed-1.3.3/MANIFEST.in
--rw-rw-rw-   0        0        0     1263 2023-07-08 18:18:39.755475 qvsed-1.3.3/PKG-INFO
--rw-rw-rw-   0        0        0     6070 2023-07-08 17:32:53.000000 qvsed-1.3.3/README.md
-drwxrwxrwx   0        0        0        0 2023-07-08 18:18:39.737090 qvsed-1.3.3/qvsed/
--rw-rw-rw-   0        0        0       50 2023-07-06 20:42:20.000000 qvsed-1.3.3/qvsed/__init__.py
--rw-rw-rw-   0        0        0      597 2023-07-08 15:55:18.000000 qvsed-1.3.3/qvsed/config_default.py
--rw-rw-rw-   0        0        0    14274 2023-07-08 18:16:26.000000 qvsed-1.3.3/qvsed/qvsed.py
--rw-rw-rw-   0        0        0    21342 2023-07-08 18:13:57.000000 qvsed-1.3.3/qvsed/qvsed.ui
-drwxrwxrwx   0        0        0        0 2023-07-08 18:18:39.750254 qvsed-1.3.3/qvsed.egg-info/
--rw-rw-rw-   0        0        0     1263 2023-07-08 18:18:39.000000 qvsed-1.3.3/qvsed.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      290 2023-07-08 18:18:39.000000 qvsed-1.3.3/qvsed.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-08 18:18:39.000000 qvsed-1.3.3/qvsed.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2023-07-08 18:18:39.000000 qvsed-1.3.3/qvsed.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        6 2023-07-08 18:18:39.000000 qvsed-1.3.3/qvsed.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-07-08 18:18:39.000000 qvsed-1.3.3/qvsed.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-08 18:18:39.756590 qvsed-1.3.3/setup.cfg
--rw-rw-rw-   0        0        0     1633 2023-07-08 18:08:58.000000 qvsed-1.3.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-08 19:30:44.155598 qvsed-1.3.4/
+-rw-rw-rw-   0        0        0    35823 2023-07-06 15:36:27.000000 qvsed-1.3.4/LICENSE.txt
+-rw-rw-rw-   0        0        0       57 2023-07-07 19:12:44.000000 qvsed-1.3.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     1263 2023-07-08 19:30:44.155598 qvsed-1.3.4/PKG-INFO
+-rw-rw-rw-   0        0        0     6070 2023-07-08 17:32:53.000000 qvsed-1.3.4/README.md
+drwxrwxrwx   0        0        0        0 2023-07-08 19:30:44.139335 qvsed-1.3.4/qvsed/
+-rw-rw-rw-   0        0        0       50 2023-07-06 20:42:20.000000 qvsed-1.3.4/qvsed/__init__.py
+-rw-rw-rw-   0        0        0      597 2023-07-08 15:55:18.000000 qvsed-1.3.4/qvsed/config_default.py
+-rw-rw-rw-   0        0        0    14675 2023-07-08 19:30:13.000000 qvsed-1.3.4/qvsed/qvsed.py
+-rw-rw-rw-   0        0        0    21342 2023-07-08 18:13:57.000000 qvsed-1.3.4/qvsed/qvsed.ui
+drwxrwxrwx   0        0        0        0 2023-07-08 19:30:44.153361 qvsed-1.3.4/qvsed.egg-info/
+-rw-rw-rw-   0        0        0     1263 2023-07-08 19:30:44.000000 qvsed-1.3.4/qvsed.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      290 2023-07-08 19:30:44.000000 qvsed-1.3.4/qvsed.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-08 19:30:44.000000 qvsed-1.3.4/qvsed.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2023-07-08 19:30:44.000000 qvsed-1.3.4/qvsed.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        6 2023-07-08 19:30:44.000000 qvsed-1.3.4/qvsed.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-07-08 19:30:44.000000 qvsed-1.3.4/qvsed.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-08 19:30:44.155598 qvsed-1.3.4/setup.cfg
+-rw-rw-rw-   0        0        0     1633 2023-07-08 19:30:40.000000 qvsed-1.3.4/setup.py
```

### Comparing `qvsed-1.3.3/LICENSE.txt` & `qvsed-1.3.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `qvsed-1.3.3/PKG-INFO` & `qvsed-1.3.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qvsed
-Version: 1.3.3
+Version: 1.3.4
 Summary: Qt-Based Volatile Small Editor
 Home-page: https://github.com/That1M8Head/QVSED/
 Author: Arsalan Kazmi
 License: GPL-3.0-or-later
 License-File: LICENSE.txt
 
 QVSED is a volatile and small text editor.
```

### Comparing `qvsed-1.3.3/README.md` & `qvsed-1.3.4/README.md`

 * *Files identical despite different names*

### Comparing `qvsed-1.3.3/qvsed/config_default.py` & `qvsed-1.3.4/qvsed/config_default.py`

 * *Files identical despite different names*

### Comparing `qvsed-1.3.3/qvsed/qvsed.py` & `qvsed-1.3.4/qvsed/qvsed.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 See README.md or "Get Help" inside QVSED for more info
 """
 
 # pylint: disable=no-name-in-module
 # pylint: disable=attribute-defined-outside-init
 # pylint: disable=broad-exception-caught
 
-import os
+import os, sys
 import shutil
 import importlib.util
 import pkg_resources
 from PyQt5.QtWidgets import (
     QApplication, QMainWindow, QPushButton, QWidget,
     QFileDialog, QPlainTextEdit, QLineEdit,
     QAction, QShortcut
@@ -54,15 +54,17 @@
         super().__init__()
         self.load_ui_file()
         self.focus_text_area()
         self.set_text_area_encoding("UTF-8")
         self.set_up_action_deck()
         self.load_config()
         self.set_up_fonts()
-        self.echo_area_update(f"Welcome to QVSED version {self.get_qvsed_version()}!")
+        self.echo_area_update(f"Welcome to QVSED v{self.get_qvsed_version()}!")
+        if self.check_if_file_parameter():
+            self.load_from_file(sys.argv[1])
 
     def apply_style_sheet(self):
         """
         Generate and apply a style sheet based on the config.py file.
         """
 
         stylesheet = f"""QMainWindow, QLabel, QPushButton, #textArea, #echoArea {{
@@ -107,14 +109,24 @@
     background: none;
 }}
         """
 
         # Apply the stylesheet to the app
         self.setStyleSheet(stylesheet)
 
+    def check_if_file_parameter(self):
+        """
+        Check if a file path was specified at the parameter.
+        """
+        if len(sys.argv) < 2:
+            return False
+
+        file_path = sys.argv[1]
+        return os.path.isfile(file_path)
+
     def clear_text_area(self):
         """
         Clear the Text Area.
         """
         text_area = self.findChild(QPlainTextEdit, "textArea")
 
         if text_area.toPlainText() == "":
@@ -235,21 +247,22 @@
             self.scrollbar_background_color = qvsed_config.scrollbar_background_color
             self.scrollbar_handle_background_color = qvsed_config.scrollbar_handle_background_color
             self.scrollbar_handle_hover_background_color = qvsed_config.scrollbar_handle_hover_background_color
             self.apply_style_sheet()
         except AttributeError as error:
             self.echo_area_update(f"Check config.py: {str(error)}")
 
-    def load_from_file(self):
+    def load_from_file(self, file_path = None):
         """
         Open a file dialog, and load the contents of a file into the Text Area.
         """
         text_area = self.findChild(QPlainTextEdit, "textArea")
 
-        file_path, _ = QFileDialog.getOpenFileName(self, "Open File")
+        if not file_path:
+            file_path, _ = QFileDialog.getOpenFileName(self, "Open File")
 
         if file_path:
             try:
                 with open(file_path, "r", encoding="utf-8") as file:
                     text_area.setPlainText(file.read())
                 file_name = os.path.basename(file_path)
                 self.echo_area_update(f"Opened file {file_name}.")
```

### Comparing `qvsed-1.3.3/qvsed/qvsed.ui` & `qvsed-1.3.4/qvsed/qvsed.ui`

 * *Files identical despite different names*

### Comparing `qvsed-1.3.3/qvsed.egg-info/PKG-INFO` & `qvsed-1.3.4/qvsed.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qvsed
-Version: 1.3.3
+Version: 1.3.4
 Summary: Qt-Based Volatile Small Editor
 Home-page: https://github.com/That1M8Head/QVSED/
 Author: Arsalan Kazmi
 License: GPL-3.0-or-later
 License-File: LICENSE.txt
 
 QVSED is a volatile and small text editor.
```

### Comparing `qvsed-1.3.3/setup.py` & `qvsed-1.3.4/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 The setup.py file for QVSED.
 """
 from setuptools import setup, find_packages
 
 setup(
     name='qvsed',
-    version='1.3.3',
+    version='1.3.4',
     author='Arsalan Kazmi',
     description='Qt-Based Volatile Small Editor',
     long_description="""QVSED is a volatile and small text editor.
 
 "Volatile" means that QVSED is entirely stateless - once you open a file, QVSED doesn't store any file paths or any other data other than the text contents of the file you loaded.
 Additionally, QVSED won't prompt you if you're about to potentially lose an unsaved file, since it doesn't know of any file metadata.
 You may be prompted if you're about to overwrite a file, but that's up to your OS, not QVSED.
```

