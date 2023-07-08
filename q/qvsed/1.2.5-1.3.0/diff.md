# Comparing `tmp/qvsed-1.2.5.tar.gz` & `tmp/qvsed-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qvsed-1.2.5.tar", last modified: Fri Jul  7 19:30:05 2023, max compression
+gzip compressed data, was "qvsed-1.3.0.tar", last modified: Sat Jul  8 16:26:55 2023, max compression
```

## Comparing `qvsed-1.2.5.tar` & `qvsed-1.3.0.tar`

### file list

```diff
@@ -1,20 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-07-07 19:30:05.661543 qvsed-1.2.5/
--rw-rw-rw-   0        0        0    35823 2023-07-06 15:36:27.000000 qvsed-1.2.5/LICENSE.txt
--rw-rw-rw-   0        0        0       57 2023-07-07 19:12:44.000000 qvsed-1.2.5/MANIFEST.in
--rw-rw-rw-   0        0        0     1263 2023-07-07 19:30:05.661543 qvsed-1.2.5/PKG-INFO
--rw-rw-rw-   0        0        0     5751 2023-07-07 12:20:45.000000 qvsed-1.2.5/README.md
-drwxrwxrwx   0        0        0        0 2023-07-07 19:30:05.640431 qvsed-1.2.5/qvsed/
--rw-rw-rw-   0        0        0       50 2023-07-06 20:42:20.000000 qvsed-1.2.5/qvsed/__init__.py
--rw-rw-rw-   0        0        0      200 2023-07-06 19:49:30.000000 qvsed-1.2.5/qvsed/config.py
--rw-rw-rw-   0        0        0      261 2023-07-06 20:11:25.000000 qvsed-1.2.5/qvsed/config_default.py
--rw-rw-rw-   0        0        0    11290 2023-07-07 18:52:58.000000 qvsed-1.2.5/qvsed/qvsed.py
--rw-rw-rw-   0        0        0    20071 2023-07-06 21:04:23.000000 qvsed-1.2.5/qvsed/qvsed.ui
-drwxrwxrwx   0        0        0        0 2023-07-07 19:30:05.660386 qvsed-1.2.5/qvsed.egg-info/
--rw-rw-rw-   0        0        0     1263 2023-07-07 19:30:05.000000 qvsed-1.2.5/qvsed.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      306 2023-07-07 19:30:05.000000 qvsed-1.2.5/qvsed.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-07 19:30:05.000000 qvsed-1.2.5/qvsed.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2023-07-07 19:30:05.000000 qvsed-1.2.5/qvsed.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        6 2023-07-07 19:30:05.000000 qvsed-1.2.5/qvsed.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-07-07 19:30:05.000000 qvsed-1.2.5/qvsed.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-07 19:30:05.663741 qvsed-1.2.5/setup.cfg
--rw-rw-rw-   0        0        0     1633 2023-07-07 19:29:42.000000 qvsed-1.2.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-08 16:26:55.305394 qvsed-1.3.0/
+-rw-rw-rw-   0        0        0    35823 2023-07-06 15:36:27.000000 qvsed-1.3.0/LICENSE.txt
+-rw-rw-rw-   0        0        0       57 2023-07-07 19:12:44.000000 qvsed-1.3.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     1263 2023-07-08 16:26:55.303084 qvsed-1.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0     6065 2023-07-08 16:26:32.000000 qvsed-1.3.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-08 16:26:55.289728 qvsed-1.3.0/qvsed/
+-rw-rw-rw-   0        0        0       50 2023-07-06 20:42:20.000000 qvsed-1.3.0/qvsed/__init__.py
+-rw-rw-rw-   0        0        0      597 2023-07-08 15:55:18.000000 qvsed-1.3.0/qvsed/config_default.py
+-rw-rw-rw-   0        0        0    13654 2023-07-08 16:22:56.000000 qvsed-1.3.0/qvsed/qvsed.py
+-rw-rw-rw-   0        0        0    20071 2023-07-08 15:47:30.000000 qvsed-1.3.0/qvsed/qvsed.ui
+drwxrwxrwx   0        0        0        0 2023-07-08 16:26:55.303084 qvsed-1.3.0/qvsed.egg-info/
+-rw-rw-rw-   0        0        0     1263 2023-07-08 16:26:55.000000 qvsed-1.3.0/qvsed.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      290 2023-07-08 16:26:55.000000 qvsed-1.3.0/qvsed.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-08 16:26:55.000000 qvsed-1.3.0/qvsed.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2023-07-08 16:26:55.000000 qvsed-1.3.0/qvsed.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        6 2023-07-08 16:26:55.000000 qvsed-1.3.0/qvsed.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-07-08 16:26:55.000000 qvsed-1.3.0/qvsed.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-08 16:26:55.305394 qvsed-1.3.0/setup.cfg
+-rw-rw-rw-   0        0        0     1633 2023-07-08 16:25:32.000000 qvsed-1.3.0/setup.py
```

### Comparing `qvsed-1.2.5/LICENSE.txt` & `qvsed-1.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `qvsed-1.2.5/PKG-INFO` & `qvsed-1.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qvsed
-Version: 1.2.5
+Version: 1.3.0
 Summary: Qt-Based Volatile Small Editor
 Home-page: https://github.com/That1M8Head/QVSED/
 Author: Arsalan Kazmi
 License: GPL-3.0-or-later
 License-File: LICENSE.txt
 
 QVSED is a volatile and small text editor.
```

### Comparing `qvsed-1.2.5/README.md` & `qvsed-1.3.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -76,20 +76,32 @@
 
 When QVSED is started, it looks for a configuration file. If it can't find one, it creates one and populates it with defaults.
 
 On Windows, the configuration file will be stored at `C:\Users\<username>\AppData\Roaming\QVSED\config.py`, where `<username>` is your Windows username.
 
 On *nix systems, the configuration file will be stored at `~/.config/QVSED/config.py`, where `~` is your home directory (`/home/<username>`).
 
-At the moment, QVSED currently only supports two options to configure, `font_family` and `font_size`.
+As of QVSED 1.3.0, you can customise the font and the colour scheme.
 
 ```python
 # The default QVSED config.
+
+# Font
 font_family = ["JetBrains Mono", "Cascadia Code", "Consolas", "Menlo", "monospace"]
 font_size = 11
+
+# Colours
+text_color = "white"
+background_color = "#282c34"
+button_background_color = "#393f4a"
+button_hover_background_color = "#31353f"
+button_pressed_background_color = background_color
+scrollbar_background_color = "#31353f"
+scrollbar_handle_background_color = "#393f4a"
+scrollbar_handle_hover_background_color = "#555B67"
 ```
 
 Keep in mind that `font_family` *must* be a list. If you want only one font, specify:
 
 ```python
 # Obviously replace "My Font" with the name of the font you want.
 font_family = ["My Font"]
```

### Comparing `qvsed-1.2.5/qvsed/qvsed.py` & `qvsed-1.3.0/qvsed/qvsed.py`

 * *Files 15% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 import os
 import shutil
 import importlib.util
 from PyQt5.QtWidgets import (
     QApplication, QMainWindow, QPushButton, QWidget,
     QFileDialog, QPlainTextEdit, QLineEdit,
-    QAction, QShortcut,
+    QAction, QShortcut
 )
 from PyQt5.QtGui import QKeySequence, QFont
 from PyQt5.QtCore import QTextCodec
 from PyQt5.uic import loadUi
 
 
 class QVSEDApp:
@@ -53,40 +53,111 @@
         super().__init__()
         self.load_ui_file()
         self.set_text_area_encoding("UTF-8")
         self.set_up_action_deck()
         self.load_config()
         self.set_up_fonts()
 
-    def echo_area_update(self, message):
+    def apply_style_sheet(self):
+        """
+        Generate and apply a style sheet based on the config.py file.
         """
-        Update the Echo Area with the given message.
 
-        Args:
-            message (str): The message to display in the Echo Area.
+        stylesheet = f"""QMainWindow, QLabel, QPushButton, #textArea, #echoArea {{
+    color: {self.text_color};
+    background: {self.background_color};
+}}
+
+QWidget#centralwidget QPushButton {{
+    border: 2px solid #31353f;
+    background: {self.button_background_color};
+    padding: 2px;
+}}
+
+QWidget#centralwidget QPushButton:hover {{
+    background: {self.button_hover_background_color};
+}}
+
+QWidget#centralwidget QPushButton:pressed {{
+    background: {self.button_pressed_background_color};
+}}
+
+QScrollBar:vertical {{
+    background-color: {self.scrollbar_background_color};
+    width: 16px;
+    margin: 16px 0 16px 0;
+}}
+
+QScrollBar::handle:vertical {{
+    background-color: {self.scrollbar_handle_background_color};
+    min-height: 20px;
+}}
+
+QScrollBar::handle:vertical:hover {{
+    background-color: {self.scrollbar_handle_hover_background_color};
+}}
+
+QScrollBar::add-line:vertical, QScrollBar::sub-line:vertical {{
+    background: none;
+}}
+
+QScrollBar::add-page:vertical, QScrollBar::sub-page:vertical {{
+    background: none;
+}}
         """
-        echo_area = self.findChild(QLineEdit, "echoArea")
-        echo_area.setText(message)
 
-    def set_text_area_encoding(self, encoding):
+        # Apply the stylesheet to the app
+        self.setStyleSheet(stylesheet)
+        
+    def clear_text_area(self):
         """
-        Set the Text Area encoding.
+        Clear the Text Area.
+        """
+        text_area = self.findChild(QPlainTextEdit, "textArea")
 
-        Args:
-            encoding (str): The encoding to set for the Text Area.
+        if text_area.toPlainText() == "":
+            self.echo_area_update("Text Area is already blank.")
+            return
+
+        text_area.clear()
+
+        self.echo_area_update("Text Area has been cleared.")
+
+    def connect_command_buttons(self):
         """
-        QTextCodec.setCodecForLocale(QTextCodec.codecForName(encoding))
+        Connect the Action Deck command buttons to their respective functions.
+        """
+        self.findChild(QPushButton, "clearButton").clicked.connect(self.clear_text_area)
+        self.findChild(QPushButton, "saveButton").clicked.connect(self.save_text_contents)
+        self.findChild(QPushButton, "openButton").clicked.connect(self.load_from_file)
+        self.findChild(QPushButton, "helpButton").clicked.connect(self.show_help)
+        self.findChild(QPushButton, "quitButton").clicked.connect(self.quit_app)
+        self.findChild(QPushButton, "fullscreenButton").clicked.connect(self.toggle_fullscreen)
 
-    def load_ui_file(self):
+    def connect_key_bindings(self):
         """
-        Load the UI file for the QVSED window.
+        Connect the Action Deck keybindings to their respective functions.
         """
-        current_dir = os.path.dirname(os.path.abspath(__file__))
-        ui_file = os.path.join(current_dir, "qvsed.ui")
-        loadUi(ui_file, self)
+        self.clear_shortcut.activated.connect(self.clear_text_area)
+        self.save_shortcut.activated.connect(self.save_text_contents)
+        self.open_shortcut.activated.connect(self.load_from_file)
+        self.help_shortcut.activated.connect(self.show_help)
+        self.quit_shortcut.activated.connect(self.quit_app)
+        self.fullscreen_shortcut.activated.connect(self.toggle_fullscreen)
+
+    def echo_area_update(self, message):
+        """
+        Update the Echo Area with the given message.
+
+        Args:
+            message (str): The message to display in the Echo Area.
+        """
+        echo_area = self.findChild(QLineEdit, "echoArea")
+        echo_area.setText(message)
+        echo_area.setCursorPosition(0)
 
     def generate_config(self):
         """
         Generate the config file for QVSED.
         """
         current_dir = os.path.dirname(os.path.abspath(__file__))
         config_default = os.path.join(current_dir, "config_default.py")
@@ -130,98 +201,59 @@
         spec = importlib.util.spec_from_file_location("qvsed_config", user_config_file)
         qvsed_config = importlib.util.module_from_spec(spec)
         spec.loader.exec_module(qvsed_config)
 
         self.font_family = qvsed_config.font_family
         self.font_size = qvsed_config.font_size
 
-    def set_up_fonts(self):
-        """
-        Set up the fonts for the QVSED window.
-        """
-        font = QFont()
-        font.setFamilies(self.font_family)
-        font.setPointSize(self.font_size)
-        QApplication.instance().setFont(font)
-        self.update_widget_fonts(self)
-
-    def set_up_actions(self):
-        """
-        Set up the Action Deck commands for the QVSED window.
-        """
-        self.clear_action = QAction("Clear Text", self)
-        self.save_action = QAction("Save File", self)
-        self.open_action = QAction("Open File", self)
-        self.help_action = QAction("Get Help", self)
-        self.quit_action = QAction("Quit QVSED", self)
+        # Load the colour scheme settings from the config file
+        # We use the shorter American spellings because it's standard, I guess
+        try:
+            self.text_color = qvsed_config.text_color
+            self.background_color = qvsed_config.background_color
+            self.button_background_color = qvsed_config.button_background_color
+            self.button_hover_background_color = qvsed_config.button_hover_background_color
+            self.button_pressed_background_color = qvsed_config.button_pressed_background_color
+            self.scrollbar_background_color = qvsed_config.scrollbar_background_color
+            self.scrollbar_handle_background_color = qvsed_config.scrollbar_handle_background_color
+            self.scrollbar_handle_hover_background_color = qvsed_config.scrollbar_handle_hover_background_color
+            self.apply_style_sheet()
+        except AttributeError as error:
+            self.echo_area_update(f"Check config.py: {str(error)}")
 
-    def set_up_shortcuts(self):
-        """
-        Set up the key bindings for the Action Deck commands.
-        """
-        self.clear_shortcut = QShortcut(QKeySequence("Ctrl+N"), self)
-        self.save_shortcut = QShortcut(QKeySequence("Ctrl+S"), self)
-        self.open_shortcut = QShortcut(QKeySequence("Ctrl+F"), self)
-        self.help_shortcut = QShortcut(QKeySequence("Ctrl+H"), self)
-        self.quit_shortcut = QShortcut(QKeySequence("Alt+Q"), self)
-        self.fullscreen_shortcut = QShortcut(QKeySequence("Alt+F"), self)
-
-    def set_up_event_handlers(self):
+    def load_from_file(self):
         """
-        Set up the event handlers for the Action Deck.
+        Open a file dialog, and load the contents of a file into the Text Area.
         """
-        self.connect_key_bindings()
-        self.connect_command_buttons()
+        text_area = self.findChild(QPlainTextEdit, "textArea")
 
-    def connect_key_bindings(self):
-        """
-        Connect the Action Deck keybindings to their respective functions.
-        """
-        self.clear_shortcut.activated.connect(self.clear_text_area)
-        self.save_shortcut.activated.connect(self.save_text_contents)
-        self.open_shortcut.activated.connect(self.load_from_file)
-        self.help_shortcut.activated.connect(self.show_help)
-        self.quit_shortcut.activated.connect(self.quit_app)
-        self.fullscreen_shortcut.activated.connect(self.toggle_fullscreen)
+        file_path, _ = QFileDialog.getOpenFileName(self, "Open File")
 
-    def connect_command_buttons(self):
-        """
-        Connect the Action Deck command buttons to their respective functions.
-        """
-        self.findChild(QPushButton, "clearButton").clicked.connect(self.clear_text_area)
-        self.findChild(QPushButton, "saveButton").clicked.connect(self.save_text_contents)
-        self.findChild(QPushButton, "openButton").clicked.connect(self.load_from_file)
-        self.findChild(QPushButton, "helpButton").clicked.connect(self.show_help)
-        self.findChild(QPushButton, "quitButton").clicked.connect(self.quit_app)
-        self.findChild(QPushButton, "fullscreenButton").clicked.connect(self.toggle_fullscreen)
+        if file_path:
+            try:
+                with open(file_path, "r", encoding="utf-8") as file:
+                    text_area.setPlainText(file.read())
+                file_name = os.path.basename(file_path)
+                self.echo_area_update(f"Opened file {file_name}.")
+            except Exception as error:
+                self.echo_area_update(f"Error opening file: {str(error)}")
 
-    def set_up_action_deck(self):
+    def load_ui_file(self):
         """
-        Set up the Action Deck for the QVSED window.
-
-        This module does nothing by itself, but it's used to run the
-        below three modules, which are all components of the Action Deck.
+        Load the UI file for the QVSED window.
         """
-        self.set_up_actions()
-        self.set_up_shortcuts()
-        self.set_up_event_handlers()
+        current_dir = os.path.dirname(os.path.abspath(__file__))
+        ui_file = os.path.join(current_dir, "qvsed.ui")
+        loadUi(ui_file, self)
 
-    def clear_text_area(self):
+    def quit_app(self):
         """
-        Clear the Text Area.
+        Quit QVSED.
         """
-        text_area = self.findChild(QPlainTextEdit, "textArea")
-
-        if text_area.toPlainText() == "":
-            self.echo_area_update("Text Area is already blank.")
-            return
-
-        text_area.clear()
-
-        self.echo_area_update("Text Area has been cleared.")
+        QApplication.quit()
 
     def save_text_contents(self):
         """
         Open a file dialog, and save the contents of the Text Area to a file.
         """
         text_area = self.findChild(QPlainTextEdit, "textArea")
 
@@ -236,30 +268,71 @@
                 with open(file_path, "w", encoding="UTF-8") as file:
                     file.write(text_area.toPlainText())
                 file_name = os.path.basename(file_path)
                 self.echo_area_update(f"Saved file {file_name}.")
             except Exception as error:
                 self.echo_area_update(f"Error saving file: {str(error)}")
 
-    def load_from_file(self):
+    def set_text_area_encoding(self, encoding):
         """
-        Open a file dialog, and load the contents of a file into the Text Area.
+        Set the Text Area encoding.
+
+        Args:
+            encoding (str): The encoding to set for the Text Area.
         """
-        text_area = self.findChild(QPlainTextEdit, "textArea")
+        QTextCodec.setCodecForLocale(QTextCodec.codecForName(encoding))
 
-        file_path, _ = QFileDialog.getOpenFileName(self, "Open File")
+    def set_up_action_deck(self):
+        """
+        Set up the Action Deck for the QVSED window.
 
-        if file_path:
-            try:
-                with open(file_path, "r", encoding="utf-8") as file:
-                    text_area.setPlainText(file.read())
-                file_name = os.path.basename(file_path)
-                self.echo_area_update(f"Opened file {file_name}.")
-            except Exception as error:
-                self.echo_area_update(f"Error opening file: {str(error)}")
+        This module does nothing by itself, but it's used to run the
+        below three modules, which are all components of the Action Deck.
+        """
+        self.set_up_actions()
+        self.set_up_shortcuts()
+        self.set_up_event_handlers()
+
+    def set_up_actions(self):
+        """
+        Set up the Action Deck commands for the QVSED window.
+        """
+        self.clear_action = QAction("Clear Text", self)
+        self.save_action = QAction("Save File", self)
+        self.open_action = QAction("Open File", self)
+        self.help_action = QAction("Get Help", self)
+        self.quit_action = QAction("Quit QVSED", self)
+
+    def set_up_event_handlers(self):
+        """
+        Set up the event handlers for the Action Deck.
+        """
+        self.connect_command_buttons()
+        self.connect_key_bindings()
+
+    def set_up_fonts(self):
+        """
+        Set up the fonts for the QVSED window.
+        """
+        font = QFont()
+        font.setFamilies(self.font_family)
+        font.setPointSize(self.font_size)
+        QApplication.instance().setFont(font)
+        self.update_widget_fonts(self)
+
+    def set_up_shortcuts(self):
+        """
+        Set up the key bindings for the Action Deck commands.
+        """
+        self.clear_shortcut = QShortcut(QKeySequence("Ctrl+N"), self)
+        self.save_shortcut = QShortcut(QKeySequence("Ctrl+S"), self)
+        self.open_shortcut = QShortcut(QKeySequence("Ctrl+F"), self)
+        self.help_shortcut = QShortcut(QKeySequence("Ctrl+H"), self)
+        self.quit_shortcut = QShortcut(QKeySequence("Alt+Q"), self)
+        self.fullscreen_shortcut = QShortcut(QKeySequence("Alt+F"), self)
 
     def show_help(self):
         """
         Display the help message in the Text Area.
         """
         text_area = self.findChild(QPlainTextEdit, "textArea")
 
@@ -275,20 +348,14 @@
 
 - Arsalan Kazmi <sonicspeed848@gmail.com>, That1M8Head on GitHub"""
 
         self.echo_area_update("Help message shown in Text Area.")
 
         text_area.setPlainText(help_message)
 
-    def quit_app(self):
-        """
-        Quit QVSED.
-        """
-        QApplication.quit()
-
     def toggle_fullscreen(self):
         """
         Toggle the QVSED window between fullscreen and normal mode.
         """
         if self.isFullScreen():
             self.showNormal()
         else:
```

### Comparing `qvsed-1.2.5/qvsed/qvsed.ui` & `qvsed-1.3.0/qvsed/qvsed.ui`

 * *Files identical despite different names*

### Comparing `qvsed-1.2.5/qvsed.egg-info/PKG-INFO` & `qvsed-1.3.0/qvsed.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qvsed
-Version: 1.2.5
+Version: 1.3.0
 Summary: Qt-Based Volatile Small Editor
 Home-page: https://github.com/That1M8Head/QVSED/
 Author: Arsalan Kazmi
 License: GPL-3.0-or-later
 License-File: LICENSE.txt
 
 QVSED is a volatile and small text editor.
```

### Comparing `qvsed-1.2.5/setup.py` & `qvsed-1.3.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 The setup.py file for QVSED.
 """
 from setuptools import setup, find_packages
 
 setup(
     name='qvsed',
-    version='1.2.5',
+    version='1.3.0',
     author='Arsalan Kazmi',
     description='Qt-Based Volatile Small Editor',
     long_description="""QVSED is a volatile and small text editor.
 
 "Volatile" means that QVSED is entirely stateless - once you open a file, QVSED doesn't store any file paths or any other data other than the text contents of the file you loaded.
 Additionally, QVSED won't prompt you if you're about to potentially lose an unsaved file, since it doesn't know of any file metadata.
 You may be prompted if you're about to overwrite a file, but that's up to your OS, not QVSED.
```

