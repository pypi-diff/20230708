# Comparing `tmp/PySide2-Frameless-Window-0.1.1.tar.gz` & `tmp/PySide2-Frameless-Window-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\PySide2-Frameless-Window-0.1.1.tar", last modified: Sat Apr 29 16:04:25 2023, max compression
+gzip compressed data, was "dist\PySide2-Frameless-Window-0.1.2.tar", last modified: Sat Jul  8 13:17:20 2023, max compression
```

## Comparing `PySide2-Frameless-Window-0.1.1.tar` & `PySide2-Frameless-Window-0.1.2.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxrwx   0        0        0        0 2023-04-29 16:04:25.734097 PySide2-Frameless-Window-0.1.1/
--rw-rw-rw-   0        0        0     7815 2023-04-29 15:59:29.000000 PySide2-Frameless-Window-0.1.1/LICENSE
--rw-rw-rw-   0        0        0     5496 2023-04-29 16:04:25.733096 PySide2-Frameless-Window-0.1.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-29 16:04:25.682230 PySide2-Frameless-Window-0.1.1/PySide2_Frameless_Window.egg-info/
--rw-rw-rw-   0        0        0     5496 2023-04-29 16:04:25.000000 PySide2-Frameless-Window-0.1.1/PySide2_Frameless_Window.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      858 2023-04-29 16:04:25.000000 PySide2-Frameless-Window-0.1.1/PySide2_Frameless_Window.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-29 16:04:25.000000 PySide2-Frameless-Window-0.1.1/PySide2_Frameless_Window.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       88 2023-04-29 16:04:25.000000 PySide2-Frameless-Window-0.1.1/PySide2_Frameless_Window.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-04-29 16:04:25.000000 PySide2-Frameless-Window-0.1.1/PySide2_Frameless_Window.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     4906 2023-04-29 15:59:29.000000 PySide2-Frameless-Window-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-29 16:04:25.692734 PySide2-Frameless-Window-0.1.1/qframelesswindow/
--rw-rw-rw-   0        0        0     2251 2023-04-29 16:03:35.000000 PySide2-Frameless-Window-0.1.1/qframelesswindow/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-29 16:04:25.697582 PySide2-Frameless-Window-0.1.1/qframelesswindow/_rc/
--rw-rw-rw-   0        0        0        0 2023-01-28 14:21:55.000000 PySide2-Frameless-Window-0.1.1/qframelesswindow/_rc/__init__.py
--rw-rw-rw-   0        0        0     2730 2023-04-29 15:59:29.000000 PySide2-Frameless-Window-0.1.1/qframelesswindow/_rc/resource.py
-drwxrwxrwx   0        0        0        0 2023-04-29 16:04:25.702695 PySide2-Frameless-Window-0.1.1/qframelesswindow/linux/
--rw-rw-rw-   0        0        0     2878 2023-04-29 15:59:29.000000 PySide2-Frameless-Window-0.1.1/qframelesswindow/linux/__init__.py
--rw-rw-rw-   0        0        0     2683 2023-04-27 01:27:44.000000 PySide2-Frameless-Window-0.1.1/qframelesswindow/linux/window_effect.py
-drwxrwxrwx   0        0        0        0 2023-04-29 16:04:25.707445 PySide2-Frameless-Window-0.1.1/qframelesswindow/mac/
--rw-rw-rw-   0        0        0     3024 2023-04-29 15:59:29.000000 PySide2-Frameless-Window-0.1.1/qframelesswindow/mac/__init__.py
--rw-rw-rw-   0        0        0     4085 2023-04-29 15:59:29.000000 PySide2-Frameless-Window-0.1.1/qframelesswindow/mac/window_effect.py
-drwxrwxrwx   0        0        0        0 2023-04-29 16:04:25.713342 PySide2-Frameless-Window-0.1.1/qframelesswindow/titlebar/
--rw-rw-rw-   0        0        0     4942 2023-04-29 15:59:29.000000 PySide2-Frameless-Window-0.1.1/qframelesswindow/titlebar/__init__.py
--rw-rw-rw-   0        0        0     9039 2023-04-29 15:59:29.000000 PySide2-Frameless-Window-0.1.1/qframelesswindow/titlebar/title_bar_buttons.py
-drwxrwxrwx   0        0        0        0 2023-04-29 16:04:25.723432 PySide2-Frameless-Window-0.1.1/qframelesswindow/utils/
--rw-rw-rw-   0        0        0      885 2022-07-25 01:20:40.000000 PySide2-Frameless-Window-0.1.1/qframelesswindow/utils/__init__.py
--rw-rw-rw-   0        0        0     1216 2023-04-29 15:59:29.000000 PySide2-Frameless-Window-0.1.1/qframelesswindow/utils/linux_utils.py
--rw-rw-rw-   0        0        0     1844 2023-04-29 15:59:29.000000 PySide2-Frameless-Window-0.1.1/qframelesswindow/utils/mac_utils.py
--rw-rw-rw-   0        0        0     7973 2023-04-29 15:59:29.000000 PySide2-Frameless-Window-0.1.1/qframelesswindow/utils/win32_utils.py
-drwxrwxrwx   0        0        0        0 2023-04-29 16:04:25.729934 PySide2-Frameless-Window-0.1.1/qframelesswindow/windows/
--rw-rw-rw-   0        0        0     7078 2023-04-29 16:01:31.000000 PySide2-Frameless-Window-0.1.1/qframelesswindow/windows/__init__.py
--rw-rw-rw-   0        0        0     4013 2023-04-27 01:27:44.000000 PySide2-Frameless-Window-0.1.1/qframelesswindow/windows/c_structures.py
--rw-rw-rw-   0        0        0     8346 2023-04-29 15:59:29.000000 PySide2-Frameless-Window-0.1.1/qframelesswindow/windows/window_effect.py
--rw-rw-rw-   0        0        0       42 2023-04-29 16:04:25.734097 PySide2-Frameless-Window-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1001 2023-04-29 16:03:39.000000 PySide2-Frameless-Window-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-08 13:17:20.621784 PySide2-Frameless-Window-0.1.2/
+-rw-rw-rw-   0        0        0     7815 2023-07-08 13:07:29.000000 PySide2-Frameless-Window-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0     5496 2023-07-08 13:17:20.619395 PySide2-Frameless-Window-0.1.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-08 13:17:20.574522 PySide2-Frameless-Window-0.1.2/PySide2_Frameless_Window.egg-info/
+-rw-rw-rw-   0        0        0     5496 2023-07-08 13:17:20.000000 PySide2-Frameless-Window-0.1.2/PySide2_Frameless_Window.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      858 2023-07-08 13:17:20.000000 PySide2-Frameless-Window-0.1.2/PySide2_Frameless_Window.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-08 13:17:20.000000 PySide2-Frameless-Window-0.1.2/PySide2_Frameless_Window.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       88 2023-07-08 13:17:20.000000 PySide2-Frameless-Window-0.1.2/PySide2_Frameless_Window.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-07-08 13:17:20.000000 PySide2-Frameless-Window-0.1.2/PySide2_Frameless_Window.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     4906 2023-07-08 13:12:31.000000 PySide2-Frameless-Window-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-08 13:17:20.581021 PySide2-Frameless-Window-0.1.2/qframelesswindow/
+-rw-rw-rw-   0        0        0     2314 2023-07-08 13:15:23.000000 PySide2-Frameless-Window-0.1.2/qframelesswindow/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-08 13:17:20.582795 PySide2-Frameless-Window-0.1.2/qframelesswindow/_rc/
+-rw-rw-rw-   0        0        0        0 2023-01-28 14:21:55.000000 PySide2-Frameless-Window-0.1.2/qframelesswindow/_rc/__init__.py
+-rw-rw-rw-   0        0        0     2730 2023-07-08 13:12:32.000000 PySide2-Frameless-Window-0.1.2/qframelesswindow/_rc/resource.py
+drwxrwxrwx   0        0        0        0 2023-07-08 13:17:20.591507 PySide2-Frameless-Window-0.1.2/qframelesswindow/linux/
+-rw-rw-rw-   0        0        0     2878 2023-07-08 13:12:32.000000 PySide2-Frameless-Window-0.1.2/qframelesswindow/linux/__init__.py
+-rw-rw-rw-   0        0        0     2912 2023-07-08 13:13:12.000000 PySide2-Frameless-Window-0.1.2/qframelesswindow/linux/window_effect.py
+drwxrwxrwx   0        0        0        0 2023-07-08 13:17:20.595847 PySide2-Frameless-Window-0.1.2/qframelesswindow/mac/
+-rw-rw-rw-   0        0        0     3024 2023-07-08 13:12:32.000000 PySide2-Frameless-Window-0.1.2/qframelesswindow/mac/__init__.py
+-rw-rw-rw-   0        0        0     4314 2023-07-08 13:12:55.000000 PySide2-Frameless-Window-0.1.2/qframelesswindow/mac/window_effect.py
+drwxrwxrwx   0        0        0        0 2023-07-08 13:17:20.599358 PySide2-Frameless-Window-0.1.2/qframelesswindow/titlebar/
+-rw-rw-rw-   0        0        0     4942 2023-07-08 13:12:32.000000 PySide2-Frameless-Window-0.1.2/qframelesswindow/titlebar/__init__.py
+-rw-rw-rw-   0        0        0     9039 2023-07-08 13:12:32.000000 PySide2-Frameless-Window-0.1.2/qframelesswindow/titlebar/title_bar_buttons.py
+drwxrwxrwx   0        0        0        0 2023-07-08 13:17:20.611234 PySide2-Frameless-Window-0.1.2/qframelesswindow/utils/
+-rw-rw-rw-   0        0        0      885 2022-07-25 01:20:40.000000 PySide2-Frameless-Window-0.1.2/qframelesswindow/utils/__init__.py
+-rw-rw-rw-   0        0        0     1216 2023-07-08 13:12:32.000000 PySide2-Frameless-Window-0.1.2/qframelesswindow/utils/linux_utils.py
+-rw-rw-rw-   0        0        0     1844 2023-07-08 13:12:32.000000 PySide2-Frameless-Window-0.1.2/qframelesswindow/utils/mac_utils.py
+-rw-rw-rw-   0        0        0     7973 2023-07-08 13:12:32.000000 PySide2-Frameless-Window-0.1.2/qframelesswindow/utils/win32_utils.py
+drwxrwxrwx   0        0        0        0 2023-07-08 13:17:20.617133 PySide2-Frameless-Window-0.1.2/qframelesswindow/windows/
+-rw-rw-rw-   0        0        0     7078 2023-07-08 13:12:32.000000 PySide2-Frameless-Window-0.1.2/qframelesswindow/windows/__init__.py
+-rw-rw-rw-   0        0        0     4013 2023-07-08 13:12:32.000000 PySide2-Frameless-Window-0.1.2/qframelesswindow/windows/c_structures.py
+-rw-rw-rw-   0        0        0     8810 2023-07-08 13:12:43.000000 PySide2-Frameless-Window-0.1.2/qframelesswindow/windows/window_effect.py
+-rw-rw-rw-   0        0        0       42 2023-07-08 13:17:20.621784 PySide2-Frameless-Window-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1001 2023-07-08 13:14:31.000000 PySide2-Frameless-Window-0.1.2/setup.py
```

### Comparing `PySide2-Frameless-Window-0.1.1/LICENSE` & `PySide2-Frameless-Window-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `PySide2-Frameless-Window-0.1.1/PKG-INFO` & `PySide2-Frameless-Window-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PySide2-Frameless-Window
-Version: 0.1.1
+Version: 0.1.2
 Summary: A cross-platform frameless window based on pyside2, support Win32, Linux and macOS.
 Home-page: https://github.com/zhiyiYo/PyQt-Frameless-Window/tree/Pyside2
 Author: zhiyiYo
 Author-email: shokokawaii@outlook.com
 License: LGPLv3
 Keywords: pyside2 frameless
 Classifier: Programming Language :: Python :: 3
```

### Comparing `PySide2-Frameless-Window-0.1.1/PySide2_Frameless_Window.egg-info/PKG-INFO` & `PySide2-Frameless-Window-0.1.2/PySide2_Frameless_Window.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PySide2-Frameless-Window
-Version: 0.1.1
+Version: 0.1.2
 Summary: A cross-platform frameless window based on pyside2, support Win32, Linux and macOS.
 Home-page: https://github.com/zhiyiYo/PyQt-Frameless-Window/tree/Pyside2
 Author: zhiyiYo
 Author-email: shokokawaii@outlook.com
 License: LGPLv3
 Keywords: pyside2 frameless
 Classifier: Programming Language :: Python :: 3
```

### Comparing `PySide2-Frameless-Window-0.1.1/PySide2_Frameless_Window.egg-info/SOURCES.txt` & `PySide2-Frameless-Window-0.1.2/PySide2_Frameless_Window.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PySide2-Frameless-Window-0.1.1/README.md` & `PySide2-Frameless-Window-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `PySide2-Frameless-Window-0.1.1/qframelesswindow/__init__.py` & `PySide2-Frameless-Window-0.1.2/qframelesswindow/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 Examples are available at https://github.com/zhiyiYo/PyQt-Frameless-Window/tree/Pyside2/examples.
 
 :copyright: (c) 2021 by zhiyiYo.
 :license: LGPLv3, see LICENSE for more details.
 """
 
-__version__ = "0.1.1"
+__version__ = "0.1.2"
 
 import sys
 
 from PySide2.QtWidgets import QDialog, QMainWindow
 
 from .titlebar import TitleBar, TitleBarButton, SvgTitleBarButton, StandardTitleBar
 
@@ -48,14 +48,15 @@
 
     def __init__(self, parent=None):
         super().__init__(parent=parent)
         self._initFrameless()
         self.titleBar.minBtn.hide()
         self.titleBar.maxBtn.hide()
         self.titleBar.setDoubleClickEnabled(False)
+        self.windowEffect.disableMaximizeButton(self.winId())
 
     def resizeEvent(self, e):
         self.titleBar.resize(self.width(), self.titleBar.height())
 
 
 class FramelessMainWindow(QMainWindow, FramelessWindowBase):
     """ Frameless main window """
```

### Comparing `PySide2-Frameless-Window-0.1.1/qframelesswindow/_rc/resource.py` & `PySide2-Frameless-Window-0.1.2/qframelesswindow/_rc/resource.py`

 * *Files identical despite different names*

### Comparing `PySide2-Frameless-Window-0.1.1/qframelesswindow/linux/__init__.py` & `PySide2-Frameless-Window-0.1.2/qframelesswindow/linux/__init__.py`

 * *Files identical despite different names*

### Comparing `PySide2-Frameless-Window-0.1.1/qframelesswindow/linux/window_effect.py` & `PySide2-Frameless-Window-0.1.2/qframelesswindow/linux/window_effect.py`

 * *Files 5% similar despite different names*

```diff
@@ -112,7 +112,17 @@
 
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
```

### Comparing `PySide2-Frameless-Window-0.1.1/qframelesswindow/mac/__init__.py` & `PySide2-Frameless-Window-0.1.2/qframelesswindow/mac/__init__.py`

 * *Files identical despite different names*

### Comparing `PySide2-Frameless-Window-0.1.1/qframelesswindow/mac/window_effect.py` & `PySide2-Frameless-Window-0.1.2/qframelesswindow/mac/window_effect.py`

 * *Files 3% similar despite different names*

```diff
@@ -142,7 +142,17 @@
 
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
```

### Comparing `PySide2-Frameless-Window-0.1.1/qframelesswindow/titlebar/__init__.py` & `PySide2-Frameless-Window-0.1.2/qframelesswindow/titlebar/__init__.py`

 * *Files identical despite different names*

### Comparing `PySide2-Frameless-Window-0.1.1/qframelesswindow/titlebar/title_bar_buttons.py` & `PySide2-Frameless-Window-0.1.2/qframelesswindow/titlebar/title_bar_buttons.py`

 * *Files identical despite different names*

### Comparing `PySide2-Frameless-Window-0.1.1/qframelesswindow/utils/__init__.py` & `PySide2-Frameless-Window-0.1.2/qframelesswindow/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `PySide2-Frameless-Window-0.1.1/qframelesswindow/utils/linux_utils.py` & `PySide2-Frameless-Window-0.1.2/qframelesswindow/utils/linux_utils.py`

 * *Files identical despite different names*

### Comparing `PySide2-Frameless-Window-0.1.1/qframelesswindow/utils/mac_utils.py` & `PySide2-Frameless-Window-0.1.2/qframelesswindow/utils/mac_utils.py`

 * *Files identical despite different names*

### Comparing `PySide2-Frameless-Window-0.1.1/qframelesswindow/utils/win32_utils.py` & `PySide2-Frameless-Window-0.1.2/qframelesswindow/utils/win32_utils.py`

 * *Files identical despite different names*

### Comparing `PySide2-Frameless-Window-0.1.1/qframelesswindow/windows/__init__.py` & `PySide2-Frameless-Window-0.1.2/qframelesswindow/windows/__init__.py`

 * *Files identical despite different names*

### Comparing `PySide2-Frameless-Window-0.1.1/qframelesswindow/windows/c_structures.py` & `PySide2-Frameless-Window-0.1.2/qframelesswindow/windows/c_structures.py`

 * *Files identical despite different names*

### Comparing `PySide2-Frameless-Window-0.1.1/qframelesswindow/windows/window_effect.py` & `PySide2-Frameless-Window-0.1.2/qframelesswindow/windows/window_effect.py`

 * *Files 6% similar despite different names*

```diff
@@ -213,14 +213,31 @@
         """
         hWnd = int(hWnd)
         style = win32gui.GetClassLong(hWnd, win32con.GCL_STYLE)
         style &= ~0x00020000  # CS_DROPSHADOW
         win32api.SetClassLong(hWnd, win32con.GCL_STYLE, style)
 
     @staticmethod
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
+    @staticmethod
     def addWindowAnimation(hWnd):
         """ Enables the maximize and minimize animation of the window
 
         Parameters
         ----------
         hWnd : int or `sip.voidptr`
             Window handle
```

### Comparing `PySide2-Frameless-Window-0.1.1/setup.py` & `PySide2-Frameless-Window-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 with open('README.md', encoding='utf-8') as f:
     long_description = f.read()
 
 setuptools.setup(
     name="PySide2-Frameless-Window",
-    version="0.1.1",
+    version="0.1.2",
     keywords="pyside2 frameless",
     author="zhiyiYo",
     author_email="shokokawaii@outlook.com",
     description="A cross-platform frameless window based on pyside2, support Win32, Linux and macOS.",
     long_description=long_description,
     long_description_content_type='text/markdown',
     license="LGPLv3",
```

