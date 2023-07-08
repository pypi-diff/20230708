# Comparing `tmp/qvsed-1.3.6.tar.gz` & `tmp/qvsed-1.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qvsed-1.3.6.tar", last modified: Sat Jul  8 21:35:11 2023, max compression
+gzip compressed data, was "qvsed-1.3.7.tar", last modified: Sat Jul  8 21:38:35 2023, max compression
```

## Comparing `qvsed-1.3.6.tar` & `qvsed-1.3.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-07-08 21:35:11.204442 qvsed-1.3.6/
--rw-rw-rw-   0        0        0    35823 2023-07-06 15:36:27.000000 qvsed-1.3.6/LICENSE.txt
--rw-rw-rw-   0        0        0       57 2023-07-08 21:12:53.000000 qvsed-1.3.6/MANIFEST.in
--rw-rw-rw-   0        0        0     1263 2023-07-08 21:35:11.203445 qvsed-1.3.6/PKG-INFO
--rw-rw-rw-   0        0        0     6070 2023-07-08 17:32:53.000000 qvsed-1.3.6/README.md
-drwxrwxrwx   0        0        0        0 2023-07-08 21:35:11.188373 qvsed-1.3.6/qvsed/
--rw-rw-rw-   0        0        0       50 2023-07-08 20:05:55.000000 qvsed-1.3.6/qvsed/__init__.py
--rw-rw-rw-   0        0        0      383 2023-07-08 21:13:12.000000 qvsed-1.3.6/qvsed/config_default.py
--rw-rw-rw-   0        0        0    14366 2023-07-08 21:34:38.000000 qvsed-1.3.6/qvsed/qvsed.py
--rw-rw-rw-   0        0        0     7950 2023-07-08 21:34:43.000000 qvsed-1.3.6/qvsed/qvsed.ui
-drwxrwxrwx   0        0        0        0 2023-07-08 21:35:11.202435 qvsed-1.3.6/qvsed.egg-info/
--rw-rw-rw-   0        0        0     1263 2023-07-08 21:35:11.000000 qvsed-1.3.6/qvsed.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      290 2023-07-08 21:35:11.000000 qvsed-1.3.6/qvsed.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-08 21:35:11.000000 qvsed-1.3.6/qvsed.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2023-07-08 21:35:11.000000 qvsed-1.3.6/qvsed.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        6 2023-07-08 21:35:11.000000 qvsed-1.3.6/qvsed.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-07-08 21:35:11.000000 qvsed-1.3.6/qvsed.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-08 21:35:11.204442 qvsed-1.3.6/setup.cfg
--rw-rw-rw-   0        0        0     1633 2023-07-08 21:35:03.000000 qvsed-1.3.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-08 21:38:35.070560 qvsed-1.3.7/
+-rw-rw-rw-   0        0        0    35823 2023-07-06 15:36:27.000000 qvsed-1.3.7/LICENSE.txt
+-rw-rw-rw-   0        0        0       57 2023-07-08 21:12:53.000000 qvsed-1.3.7/MANIFEST.in
+-rw-rw-rw-   0        0        0     1263 2023-07-08 21:38:35.069560 qvsed-1.3.7/PKG-INFO
+-rw-rw-rw-   0        0        0     6070 2023-07-08 17:32:53.000000 qvsed-1.3.7/README.md
+drwxrwxrwx   0        0        0        0 2023-07-08 21:38:35.054019 qvsed-1.3.7/qvsed/
+-rw-rw-rw-   0        0        0       50 2023-07-08 20:05:55.000000 qvsed-1.3.7/qvsed/__init__.py
+-rw-rw-rw-   0        0        0      383 2023-07-08 21:13:12.000000 qvsed-1.3.7/qvsed/config_default.py
+-rw-rw-rw-   0        0        0    14370 2023-07-08 21:37:19.000000 qvsed-1.3.7/qvsed/qvsed.py
+-rw-rw-rw-   0        0        0     7950 2023-07-08 21:34:43.000000 qvsed-1.3.7/qvsed/qvsed.ui
+drwxrwxrwx   0        0        0        0 2023-07-08 21:38:35.068551 qvsed-1.3.7/qvsed.egg-info/
+-rw-rw-rw-   0        0        0     1263 2023-07-08 21:38:34.000000 qvsed-1.3.7/qvsed.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      290 2023-07-08 21:38:34.000000 qvsed-1.3.7/qvsed.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-08 21:38:34.000000 qvsed-1.3.7/qvsed.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2023-07-08 21:38:34.000000 qvsed-1.3.7/qvsed.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        6 2023-07-08 21:38:34.000000 qvsed-1.3.7/qvsed.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-07-08 21:38:34.000000 qvsed-1.3.7/qvsed.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-08 21:38:35.070560 qvsed-1.3.7/setup.cfg
+-rw-rw-rw-   0        0        0     1633 2023-07-08 21:37:50.000000 qvsed-1.3.7/setup.py
```

### Comparing `qvsed-1.3.6/LICENSE.txt` & `qvsed-1.3.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `qvsed-1.3.6/PKG-INFO` & `qvsed-1.3.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qvsed
-Version: 1.3.6
+Version: 1.3.7
 Summary: Qt-Based Volatile Small Editor
 Home-page: https://github.com/That1M8Head/QVSED/
 Author: Arsalan Kazmi
 License: GPL-3.0-or-later
 License-File: LICENSE.txt
 
 QVSED is a volatile and small text editor.
```

### Comparing `qvsed-1.3.6/README.md` & `qvsed-1.3.7/README.md`

 * *Files identical despite different names*

### Comparing `qvsed-1.3.6/qvsed/qvsed.py` & `qvsed-1.3.7/qvsed/qvsed.py`

 * *Files 1% similar despite different names*

```diff
@@ -75,15 +75,15 @@
     color: {text_color};
     background: {background_color};
 }}
 
 QPlainTextEdit, QLineEdit {{
     color: {text_color};
     background: {button_focus_color};
-    border: 2px solid {button_color};
+    border: 2px solid {background_color};
 }}
 
 QPushButton {{
     color: {text_color};
     border: 2px solid {button_focus_color};
     background: {button_color};
     padding: 2px;
```

### Comparing `qvsed-1.3.6/qvsed/qvsed.ui` & `qvsed-1.3.7/qvsed/qvsed.ui`

 * *Files identical despite different names*

### Comparing `qvsed-1.3.6/qvsed.egg-info/PKG-INFO` & `qvsed-1.3.7/qvsed.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qvsed
-Version: 1.3.6
+Version: 1.3.7
 Summary: Qt-Based Volatile Small Editor
 Home-page: https://github.com/That1M8Head/QVSED/
 Author: Arsalan Kazmi
 License: GPL-3.0-or-later
 License-File: LICENSE.txt
 
 QVSED is a volatile and small text editor.
```

### Comparing `qvsed-1.3.6/setup.py` & `qvsed-1.3.7/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 The setup.py file for QVSED.
 """
 from setuptools import setup, find_packages
 
 setup(
     name='qvsed',
-    version='1.3.6',
+    version='1.3.7',
     author='Arsalan Kazmi',
     description='Qt-Based Volatile Small Editor',
     long_description="""QVSED is a volatile and small text editor.
 
 "Volatile" means that QVSED is entirely stateless - once you open a file, QVSED doesn't store any file paths or any other data other than the text contents of the file you loaded.
 Additionally, QVSED won't prompt you if you're about to potentially lose an unsaved file, since it doesn't know of any file metadata.
 You may be prompted if you're about to overwrite a file, but that's up to your OS, not QVSED.
```

