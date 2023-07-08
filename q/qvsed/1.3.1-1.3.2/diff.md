# Comparing `tmp/qvsed-1.3.1.tar.gz` & `tmp/qvsed-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qvsed-1.3.1.tar", last modified: Sat Jul  8 17:31:10 2023, max compression
+gzip compressed data, was "qvsed-1.3.2.tar", last modified: Sat Jul  8 18:02:53 2023, max compression
```

## Comparing `qvsed-1.3.1.tar` & `qvsed-1.3.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-07-08 17:31:10.385096 qvsed-1.3.1/
--rw-rw-rw-   0        0        0    35823 2023-07-06 15:36:27.000000 qvsed-1.3.1/LICENSE.txt
--rw-rw-rw-   0        0        0       57 2023-07-07 19:12:44.000000 qvsed-1.3.1/MANIFEST.in
--rw-rw-rw-   0        0        0     1263 2023-07-08 17:31:10.385096 qvsed-1.3.1/PKG-INFO
--rw-rw-rw-   0        0        0     6068 2023-07-08 17:30:58.000000 qvsed-1.3.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-08 17:31:10.363725 qvsed-1.3.1/qvsed/
--rw-rw-rw-   0        0        0       50 2023-07-06 20:42:20.000000 qvsed-1.3.1/qvsed/__init__.py
--rw-rw-rw-   0        0        0      597 2023-07-08 15:55:18.000000 qvsed-1.3.1/qvsed/config_default.py
--rw-rw-rw-   0        0        0    13655 2023-07-08 17:28:21.000000 qvsed-1.3.1/qvsed/qvsed.py
--rw-rw-rw-   0        0        0    21365 2023-07-08 17:21:24.000000 qvsed-1.3.1/qvsed/qvsed.ui
-drwxrwxrwx   0        0        0        0 2023-07-08 17:31:10.382077 qvsed-1.3.1/qvsed.egg-info/
--rw-rw-rw-   0        0        0     1263 2023-07-08 17:31:10.000000 qvsed-1.3.1/qvsed.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      290 2023-07-08 17:31:10.000000 qvsed-1.3.1/qvsed.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-08 17:31:10.000000 qvsed-1.3.1/qvsed.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2023-07-08 17:31:10.000000 qvsed-1.3.1/qvsed.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        6 2023-07-08 17:31:10.000000 qvsed-1.3.1/qvsed.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-07-08 17:31:10.000000 qvsed-1.3.1/qvsed.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-08 17:31:10.385096 qvsed-1.3.1/setup.cfg
--rw-rw-rw-   0        0        0     1633 2023-07-08 17:30:42.000000 qvsed-1.3.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-08 18:02:53.588077 qvsed-1.3.2/
+-rw-rw-rw-   0        0        0    35823 2023-07-06 15:36:27.000000 qvsed-1.3.2/LICENSE.txt
+-rw-rw-rw-   0        0        0       57 2023-07-07 19:12:44.000000 qvsed-1.3.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     1263 2023-07-08 18:02:53.587071 qvsed-1.3.2/PKG-INFO
+-rw-rw-rw-   0        0        0     6070 2023-07-08 17:32:53.000000 qvsed-1.3.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-08 18:02:53.558292 qvsed-1.3.2/qvsed/
+-rw-rw-rw-   0        0        0       50 2023-07-06 20:42:20.000000 qvsed-1.3.2/qvsed/__init__.py
+-rw-rw-rw-   0        0        0      597 2023-07-08 15:55:18.000000 qvsed-1.3.2/qvsed/config_default.py
+-rw-rw-rw-   0        0        0    13883 2023-07-08 18:02:06.000000 qvsed-1.3.2/qvsed/qvsed.py
+-rw-rw-rw-   0        0        0    21365 2023-07-08 17:21:24.000000 qvsed-1.3.2/qvsed/qvsed.ui
+drwxrwxrwx   0        0        0        0 2023-07-08 18:02:53.585106 qvsed-1.3.2/qvsed.egg-info/
+-rw-rw-rw-   0        0        0     1263 2023-07-08 18:02:53.000000 qvsed-1.3.2/qvsed.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      290 2023-07-08 18:02:53.000000 qvsed-1.3.2/qvsed.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-08 18:02:53.000000 qvsed-1.3.2/qvsed.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2023-07-08 18:02:53.000000 qvsed-1.3.2/qvsed.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        6 2023-07-08 18:02:53.000000 qvsed-1.3.2/qvsed.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-07-08 18:02:53.000000 qvsed-1.3.2/qvsed.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-08 18:02:53.588077 qvsed-1.3.2/setup.cfg
+-rw-rw-rw-   0        0        0     1633 2023-07-08 18:02:43.000000 qvsed-1.3.2/setup.py
```

### Comparing `qvsed-1.3.1/LICENSE.txt` & `qvsed-1.3.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `qvsed-1.3.1/PKG-INFO` & `qvsed-1.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qvsed
-Version: 1.3.1
+Version: 1.3.2
 Summary: Qt-Based Volatile Small Editor
 Home-page: https://github.com/That1M8Head/QVSED/
 Author: Arsalan Kazmi
 License: GPL-3.0-or-later
 License-File: LICENSE.txt
 
 QVSED is a volatile and small text editor.
```

### Comparing `qvsed-1.3.1/README.md` & `qvsed-1.3.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # QVSED - Qt-based Volatile Small Editor
 
 QVSED is a volatile text editor.
 
-![QVSED screenshot, showing the help message](qvsed_screenie.png)
+![QVSED screenshot, showing the help message](qvsed-screenshot.png)
 
 "Volatile" means that QVSED is entirely stateless - once you open a file, QVSED doesn't store any file paths or any other data other than the text contents of the file you loaded. Additionally, QVSED won't prompt you if you're about to potentially lose an unsaved file, since it doesn't know of any file metadata. You may be prompted if you're about to overwrite a file, but that's up to your OS, not QVSED.
 
 QVSED follows the philosophy of ultra-minimalism, with its heavy emphasis on just editing text and nothing more. QVSED's editing style is text-based, not file-based like basically every other editor out there. Text goes in, from a file, and then text later comes out, into another or perhaps the same file.
 
 QVSED can be used as a simple scratchpad or throwaway editor, as well as a general editing software application, since it won't prompt you if you do anything destructive, It stays out of your way on many occasions. Whether or not that's a good thing is up to you.
```

### Comparing `qvsed-1.3.1/qvsed/config_default.py` & `qvsed-1.3.2/qvsed/config_default.py`

 * *Files identical despite different names*

### Comparing `qvsed-1.3.1/qvsed/qvsed.py` & `qvsed-1.3.2/qvsed/qvsed.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,14 +48,15 @@
 
     def __init__(self):
         """
         Initialize the QVSED window.
         """
         super().__init__()
         self.load_ui_file()
+        self.focus_text_area()
         self.set_text_area_encoding("UTF-8")
         self.set_up_action_deck()
         self.load_config()
         self.set_up_fonts()
 
     def apply_style_sheet(self):
         """
@@ -151,14 +152,21 @@
         Args:
             message (str): The message to display in the Echo Area.
         """
         echo_area = self.findChild(QLineEdit, "echoArea")
         echo_area.setText(message)
         echo_area.setCursorPosition(0)
 
+    def focus_text_area(self):
+        """
+        Set the Text Area to have focus.
+        """
+        text_area = self.findChild(QPlainTextEdit, "textArea")
+        text_area.setFocus()
+
     def generate_config(self):
         """
         Generate the config file for QVSED.
         """
         current_dir = os.path.dirname(os.path.abspath(__file__))
         config_default = os.path.join(current_dir, "config_default.py")
```

### Comparing `qvsed-1.3.1/qvsed/qvsed.ui` & `qvsed-1.3.2/qvsed/qvsed.ui`

 * *Files identical despite different names*

### Comparing `qvsed-1.3.1/qvsed.egg-info/PKG-INFO` & `qvsed-1.3.2/qvsed.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qvsed
-Version: 1.3.1
+Version: 1.3.2
 Summary: Qt-Based Volatile Small Editor
 Home-page: https://github.com/That1M8Head/QVSED/
 Author: Arsalan Kazmi
 License: GPL-3.0-or-later
 License-File: LICENSE.txt
 
 QVSED is a volatile and small text editor.
```

### Comparing `qvsed-1.3.1/setup.py` & `qvsed-1.3.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 The setup.py file for QVSED.
 """
 from setuptools import setup, find_packages
 
 setup(
     name='qvsed',
-    version='1.3.1',
+    version='1.3.2',
     author='Arsalan Kazmi',
     description='Qt-Based Volatile Small Editor',
     long_description="""QVSED is a volatile and small text editor.
 
 "Volatile" means that QVSED is entirely stateless - once you open a file, QVSED doesn't store any file paths or any other data other than the text contents of the file you loaded.
 Additionally, QVSED won't prompt you if you're about to potentially lose an unsaved file, since it doesn't know of any file metadata.
 You may be prompted if you're about to overwrite a file, but that's up to your OS, not QVSED.
```

