# Comparing `tmp/PyQt6-Frameless-Window-0.1.1.tar.gz` & `tmp/PyQt6-Frameless-Window-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\PyQt6-Frameless-Window-0.1.1.tar", last modified: Mon Apr 17 07:16:57 2023, max compression
+gzip compressed data, was "dist\PyQt6-Frameless-Window-0.1.2.tar", last modified: Sat Jul  8 13:24:26 2023, max compression
```

## Comparing `PyQt6-Frameless-Window-0.1.1.tar` & `PyQt6-Frameless-Window-0.1.2.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxrwx   0        0        0        0 2023-04-17 07:16:57.759624 PyQt6-Frameless-Window-0.1.1/
--rw-rw-rw-   0        0        0    35823 2023-04-14 02:47:40.000000 PyQt6-Frameless-Window-0.1.1/LICENSE
--rw-rw-rw-   0        0        0     5582 2023-04-17 07:16:57.758530 PyQt6-Frameless-Window-0.1.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-17 07:16:57.718817 PyQt6-Frameless-Window-0.1.1/PyQt6_Frameless_Window.egg-info/
--rw-rw-rw-   0        0        0     5582 2023-04-17 07:16:57.000000 PyQt6-Frameless-Window-0.1.1/PyQt6_Frameless_Window.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      848 2023-04-17 07:16:57.000000 PyQt6-Frameless-Window-0.1.1/PyQt6_Frameless_Window.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-17 07:16:57.000000 PyQt6-Frameless-Window-0.1.1/PyQt6_Frameless_Window.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       88 2023-04-17 07:16:57.000000 PyQt6-Frameless-Window-0.1.1/PyQt6_Frameless_Window.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-04-17 07:16:57.000000 PyQt6-Frameless-Window-0.1.1/PyQt6_Frameless_Window.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     5007 2023-04-17 07:14:43.000000 PyQt6-Frameless-Window-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-17 07:16:57.721387 PyQt6-Frameless-Window-0.1.1/qframelesswindow/
--rw-rw-rw-   0        0        0     1615 2023-04-17 07:15:33.000000 PyQt6-Frameless-Window-0.1.1/qframelesswindow/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-17 07:16:57.725809 PyQt6-Frameless-Window-0.1.1/qframelesswindow/_rc/
--rw-rw-rw-   0        0        0        0 2023-01-28 14:21:55.000000 PyQt6-Frameless-Window-0.1.1/qframelesswindow/_rc/__init__.py
--rw-rw-rw-   0        0        0     2728 2023-04-17 07:14:43.000000 PyQt6-Frameless-Window-0.1.1/qframelesswindow/_rc/resource.py
-drwxrwxrwx   0        0        0        0 2023-04-17 07:16:57.730780 PyQt6-Frameless-Window-0.1.1/qframelesswindow/linux/
--rw-rw-rw-   0        0        0     3110 2023-04-17 07:14:43.000000 PyQt6-Frameless-Window-0.1.1/qframelesswindow/linux/__init__.py
--rw-rw-rw-   0        0        0     2920 2023-04-17 07:14:43.000000 PyQt6-Frameless-Window-0.1.1/qframelesswindow/linux/window_effect.py
-drwxrwxrwx   0        0        0        0 2023-04-17 07:16:57.735564 PyQt6-Frameless-Window-0.1.1/qframelesswindow/mac/
--rw-rw-rw-   0        0        0     3015 2023-04-17 07:14:44.000000 PyQt6-Frameless-Window-0.1.1/qframelesswindow/mac/__init__.py
--rw-rw-rw-   0        0        0     4095 2023-04-17 07:14:44.000000 PyQt6-Frameless-Window-0.1.1/qframelesswindow/mac/window_effect.py
-drwxrwxrwx   0        0        0        0 2023-04-17 07:16:57.739746 PyQt6-Frameless-Window-0.1.1/qframelesswindow/titlebar/
--rw-rw-rw-   0        0        0     5083 2023-04-17 07:14:44.000000 PyQt6-Frameless-Window-0.1.1/qframelesswindow/titlebar/__init__.py
--rw-rw-rw-   0        0        0     9205 2023-04-17 07:14:44.000000 PyQt6-Frameless-Window-0.1.1/qframelesswindow/titlebar/title_bar_buttons.py
-drwxrwxrwx   0        0        0        0 2023-04-17 07:16:57.749907 PyQt6-Frameless-Window-0.1.1/qframelesswindow/utils/
--rw-rw-rw-   0        0        0      885 2022-07-25 01:20:40.000000 PyQt6-Frameless-Window-0.1.1/qframelesswindow/utils/__init__.py
--rw-rw-rw-   0        0        0      644 2023-04-17 07:14:44.000000 PyQt6-Frameless-Window-0.1.1/qframelesswindow/utils/linux_utils.py
--rw-rw-rw-   0        0        0     1850 2023-04-17 07:14:44.000000 PyQt6-Frameless-Window-0.1.1/qframelesswindow/utils/mac_utils.py
--rw-rw-rw-   0        0        0     8352 2023-04-17 07:15:38.000000 PyQt6-Frameless-Window-0.1.1/qframelesswindow/utils/win32_utils.py
-drwxrwxrwx   0        0        0        0 2023-04-17 07:16:57.756301 PyQt6-Frameless-Window-0.1.1/qframelesswindow/windows/
--rw-rw-rw-   0        0        0     6624 2023-04-17 07:14:44.000000 PyQt6-Frameless-Window-0.1.1/qframelesswindow/windows/__init__.py
--rw-rw-rw-   0        0        0     4261 2023-04-17 07:14:44.000000 PyQt6-Frameless-Window-0.1.1/qframelesswindow/windows/c_structures.py
--rw-rw-rw-   0        0        0     8949 2023-04-17 07:14:44.000000 PyQt6-Frameless-Window-0.1.1/qframelesswindow/windows/window_effect.py
--rw-rw-rw-   0        0        0       42 2023-04-17 07:16:57.759624 PyQt6-Frameless-Window-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      984 2023-04-17 07:15:25.000000 PyQt6-Frameless-Window-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-08 13:24:26.674354 PyQt6-Frameless-Window-0.1.2/
+-rw-rw-rw-   0        0        0    35823 2023-07-08 13:18:44.000000 PyQt6-Frameless-Window-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0     5582 2023-07-08 13:24:26.674354 PyQt6-Frameless-Window-0.1.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-08 13:24:26.625336 PyQt6-Frameless-Window-0.1.2/PyQt6_Frameless_Window.egg-info/
+-rw-rw-rw-   0        0        0     5582 2023-07-08 13:24:26.000000 PyQt6-Frameless-Window-0.1.2/PyQt6_Frameless_Window.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      848 2023-07-08 13:24:26.000000 PyQt6-Frameless-Window-0.1.2/PyQt6_Frameless_Window.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-08 13:24:26.000000 PyQt6-Frameless-Window-0.1.2/PyQt6_Frameless_Window.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       88 2023-07-08 13:24:26.000000 PyQt6-Frameless-Window-0.1.2/PyQt6_Frameless_Window.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-07-08 13:24:26.000000 PyQt6-Frameless-Window-0.1.2/PyQt6_Frameless_Window.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     5007 2023-07-08 13:18:44.000000 PyQt6-Frameless-Window-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-08 13:24:26.638633 PyQt6-Frameless-Window-0.1.2/qframelesswindow/
+-rw-rw-rw-   0        0        0     1678 2023-07-08 13:23:07.000000 PyQt6-Frameless-Window-0.1.2/qframelesswindow/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-08 13:24:26.643174 PyQt6-Frameless-Window-0.1.2/qframelesswindow/_rc/
+-rw-rw-rw-   0        0        0        0 2023-01-28 14:21:55.000000 PyQt6-Frameless-Window-0.1.2/qframelesswindow/_rc/__init__.py
+-rw-rw-rw-   0        0        0     2728 2023-07-08 13:18:44.000000 PyQt6-Frameless-Window-0.1.2/qframelesswindow/_rc/resource.py
+drwxrwxrwx   0        0        0        0 2023-07-08 13:24:26.647615 PyQt6-Frameless-Window-0.1.2/qframelesswindow/linux/
+-rw-rw-rw-   0        0        0     3110 2023-07-08 13:18:44.000000 PyQt6-Frameless-Window-0.1.2/qframelesswindow/linux/__init__.py
+-rw-rw-rw-   0        0        0     3149 2023-07-08 13:19:21.000000 PyQt6-Frameless-Window-0.1.2/qframelesswindow/linux/window_effect.py
+drwxrwxrwx   0        0        0        0 2023-07-08 13:24:26.649625 PyQt6-Frameless-Window-0.1.2/qframelesswindow/mac/
+-rw-rw-rw-   0        0        0     3015 2023-07-08 13:18:44.000000 PyQt6-Frameless-Window-0.1.2/qframelesswindow/mac/__init__.py
+-rw-rw-rw-   0        0        0     4563 2023-07-08 13:19:46.000000 PyQt6-Frameless-Window-0.1.2/qframelesswindow/mac/window_effect.py
+drwxrwxrwx   0        0        0        0 2023-07-08 13:24:26.658001 PyQt6-Frameless-Window-0.1.2/qframelesswindow/titlebar/
+-rw-rw-rw-   0        0        0     5083 2023-07-08 13:18:44.000000 PyQt6-Frameless-Window-0.1.2/qframelesswindow/titlebar/__init__.py
+-rw-rw-rw-   0        0        0     9205 2023-07-08 13:18:44.000000 PyQt6-Frameless-Window-0.1.2/qframelesswindow/titlebar/title_bar_buttons.py
+drwxrwxrwx   0        0        0        0 2023-07-08 13:24:26.666179 PyQt6-Frameless-Window-0.1.2/qframelesswindow/utils/
+-rw-rw-rw-   0        0        0      885 2022-07-25 01:20:40.000000 PyQt6-Frameless-Window-0.1.2/qframelesswindow/utils/__init__.py
+-rw-rw-rw-   0        0        0      644 2023-07-08 13:18:44.000000 PyQt6-Frameless-Window-0.1.2/qframelesswindow/utils/linux_utils.py
+-rw-rw-rw-   0        0        0     1850 2023-07-08 13:18:44.000000 PyQt6-Frameless-Window-0.1.2/qframelesswindow/utils/mac_utils.py
+-rw-rw-rw-   0        0        0     8352 2023-07-08 13:18:44.000000 PyQt6-Frameless-Window-0.1.2/qframelesswindow/utils/win32_utils.py
+drwxrwxrwx   0        0        0        0 2023-07-08 13:24:26.674354 PyQt6-Frameless-Window-0.1.2/qframelesswindow/windows/
+-rw-rw-rw-   0        0        0     6624 2023-07-08 13:18:44.000000 PyQt6-Frameless-Window-0.1.2/qframelesswindow/windows/__init__.py
+-rw-rw-rw-   0        0        0     4261 2023-07-08 13:18:44.000000 PyQt6-Frameless-Window-0.1.2/qframelesswindow/windows/c_structures.py
+-rw-rw-rw-   0        0        0     9413 2023-07-08 13:18:53.000000 PyQt6-Frameless-Window-0.1.2/qframelesswindow/windows/window_effect.py
+-rw-rw-rw-   0        0        0       42 2023-07-08 13:24:26.674354 PyQt6-Frameless-Window-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      984 2023-07-08 13:20:08.000000 PyQt6-Frameless-Window-0.1.2/setup.py
```

### Comparing `PyQt6-Frameless-Window-0.1.1/LICENSE` & `PyQt6-Frameless-Window-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `PyQt6-Frameless-Window-0.1.1/PKG-INFO` & `PyQt6-Frameless-Window-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyQt6-Frameless-Window
-Version: 0.1.1
+Version: 0.1.2
 Summary: A cross-platform frameless window based on pyqt6, support Win32, Linux and macOS.
 Home-page: https://github.com/zhiyiYo/PyQt-Frameless-Window/tree/PyQt6
 Author: zhiyiYo
 Author-email: shokokawaii@outlook.com
 License: GPLv3
 Keywords: pyqt6 frameless
 Classifier: Programming Language :: Python :: 3
```

### Comparing `PyQt6-Frameless-Window-0.1.1/PyQt6_Frameless_Window.egg-info/PKG-INFO` & `PyQt6-Frameless-Window-0.1.2/PyQt6_Frameless_Window.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyQt6-Frameless-Window
-Version: 0.1.1
+Version: 0.1.2
 Summary: A cross-platform frameless window based on pyqt6, support Win32, Linux and macOS.
 Home-page: https://github.com/zhiyiYo/PyQt-Frameless-Window/tree/PyQt6
 Author: zhiyiYo
 Author-email: shokokawaii@outlook.com
 License: GPLv3
 Keywords: pyqt6 frameless
 Classifier: Programming Language :: Python :: 3
```

### Comparing `PyQt6-Frameless-Window-0.1.1/PyQt6_Frameless_Window.egg-info/SOURCES.txt` & `PyQt6-Frameless-Window-0.1.2/PyQt6_Frameless_Window.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PyQt6-Frameless-Window-0.1.1/README.md` & `PyQt6-Frameless-Window-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `PyQt6-Frameless-Window-0.1.1/qframelesswindow/__init__.py` & `PyQt6-Frameless-Window-0.1.2/qframelesswindow/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 Examples are available at https://github.com/zhiyiYo/PyQt-Frameless-Window/tree/PyQt6/examples.
 
 :copyright: (c) 2021 by zhiyiYo.
 :license: GPLv3, see LICENSE for more details.
 """
 
-__version__ = "0.1.1"
+__version__ = "0.1.2"
 
 import sys
 
 from PyQt6.QtWidgets import QDialog, QMainWindow
 
 from .titlebar import TitleBar, TitleBarButton, SvgTitleBarButton, StandardTitleBar
 
@@ -39,14 +39,15 @@
     """ Frameless dialog """
 
     def __init__(self, parent=None):
         super().__init__(parent)
         self.titleBar.minBtn.hide()
         self.titleBar.maxBtn.hide()
         self.titleBar.setDoubleClickEnabled(False)
+        self.windowEffect.disableMaximizeButton(self.winId())
 
 
 class FramelessMainWindow(QMainWindow, FramelessWindow):
     """ Frameless main window """
 
     def __init__(self, parent=None):
         super().__init__(parent)
```

### Comparing `PyQt6-Frameless-Window-0.1.1/qframelesswindow/_rc/resource.py` & `PyQt6-Frameless-Window-0.1.2/qframelesswindow/_rc/resource.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Frameless-Window-0.1.1/qframelesswindow/linux/__init__.py` & `PyQt6-Frameless-Window-0.1.2/qframelesswindow/linux/__init__.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Frameless-Window-0.1.1/qframelesswindow/linux/window_effect.py` & `PyQt6-Frameless-Window-0.1.2/qframelesswindow/linux/window_effect.py`

 * *Files 2% similar despite different names*

```diff
@@ -113,14 +113,24 @@
         Parameters
         ----------
         hWnd : int or `sip.voidptr`
             Window handle
         """
         pass
 
+    @staticmethod
+    def disableMaximizeButton(hWnd):
+        """ Disable the maximize button of window
+
+        Parameters
+        ----------
+        hWnd : int or `sip.voidptr`
+            Window handle
+        """
+
     def enableBlurBehindWindow(self, hWnd):
         """ enable the blur effect behind the whole client
 
         Parameters
         ----------
         hWnd: int or `sip.voidptr`
             Window handle
```

### Comparing `PyQt6-Frameless-Window-0.1.1/qframelesswindow/mac/__init__.py` & `PyQt6-Frameless-Window-0.1.2/qframelesswindow/mac/__init__.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Frameless-Window-0.1.1/qframelesswindow/mac/window_effect.py` & `PyQt6-Frameless-Window-0.1.2/qframelesswindow/mac/window_effect.py`

 * *Files 4% similar despite different names*

```diff
@@ -141,7 +141,27 @@
 
         Parameters
         ----------
         hWnd : int or `sip.voidptr`
             Window handle
         """
         pass
+
+    @staticmethod
+    def disableMaximizeButton(hWnd):
+        """ Disable the maximize button of window
+
+        Parameters
+        ----------
+        hWnd : int or `sip.voidptr`
+            Window handle
+        """
+
+    def enableBlurBehindWindow(self, hWnd):
+        """ enable the blur effect behind the whole client
+
+        Parameters
+        ----------
+        hWnd: int or `sip.voidptr`
+            Window handle
+        """
+        pass
```

### Comparing `PyQt6-Frameless-Window-0.1.1/qframelesswindow/titlebar/__init__.py` & `PyQt6-Frameless-Window-0.1.2/qframelesswindow/titlebar/__init__.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Frameless-Window-0.1.1/qframelesswindow/titlebar/title_bar_buttons.py` & `PyQt6-Frameless-Window-0.1.2/qframelesswindow/titlebar/title_bar_buttons.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Frameless-Window-0.1.1/qframelesswindow/utils/__init__.py` & `PyQt6-Frameless-Window-0.1.2/qframelesswindow/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Frameless-Window-0.1.1/qframelesswindow/utils/linux_utils.py` & `PyQt6-Frameless-Window-0.1.2/qframelesswindow/utils/linux_utils.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Frameless-Window-0.1.1/qframelesswindow/utils/mac_utils.py` & `PyQt6-Frameless-Window-0.1.2/qframelesswindow/utils/mac_utils.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Frameless-Window-0.1.1/qframelesswindow/utils/win32_utils.py` & `PyQt6-Frameless-Window-0.1.2/qframelesswindow/utils/win32_utils.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Frameless-Window-0.1.1/qframelesswindow/windows/__init__.py` & `PyQt6-Frameless-Window-0.1.2/qframelesswindow/windows/__init__.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Frameless-Window-0.1.1/qframelesswindow/windows/c_structures.py` & `PyQt6-Frameless-Window-0.1.2/qframelesswindow/windows/c_structures.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Frameless-Window-0.1.1/qframelesswindow/windows/window_effect.py` & `PyQt6-Frameless-Window-0.1.2/qframelesswindow/windows/window_effect.py`

 * *Files 3% similar despite different names*

```diff
@@ -239,14 +239,31 @@
             | win32con.WS_MINIMIZEBOX
             | win32con.WS_MAXIMIZEBOX
             | win32con.WS_CAPTION
             | win32con.CS_DBLCLKS
             | win32con.WS_THICKFRAME,
         )
 
+    @staticmethod
+    def disableMaximizeButton(hWnd):
+        """ Disable the maximize button of window
+
+        Parameters
+        ----------
+        hWnd : int or `sip.voidptr`
+            Window handle
+        """
+        hWnd = int(hWnd)
+        style = win32gui.GetWindowLong(hWnd, win32con.GWL_STYLE)
+        win32gui.SetWindowLong(
+            hWnd,
+            win32con.GWL_STYLE,
+            style & ~win32con.WS_MAXIMIZEBOX,
+        )
+
     def enableBlurBehindWindow(self, hWnd):
         """ enable the blur effect behind the whole client
 
         Parameters
         ----------
         hWnd: int or `sip.voidptr`
             Window handle
```

### Comparing `PyQt6-Frameless-Window-0.1.1/setup.py` & `PyQt6-Frameless-Window-0.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 with open('README.md', encoding='utf-8') as f:
     long_description = f.read()
 
 setuptools.setup(
     name="PyQt6-Frameless-Window",
-    version="0.1.1",
+    version="0.1.2",
     keywords="pyqt6 frameless",
     author="zhiyiYo",
     author_email="shokokawaii@outlook.com",
     description="A cross-platform frameless window based on pyqt6, support Win32, Linux and macOS.",
     long_description=long_description,
     long_description_content_type='text/markdown',
     license="GPLv3",
```

