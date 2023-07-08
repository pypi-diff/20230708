# Comparing `tmp/PySideSix-Frameless-Window-0.1.0.tar.gz` & `tmp/PySideSix-Frameless-Window-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\PySideSix-Frameless-Window-0.1.0.tar", last modified: Mon Apr 17 07:24:01 2023, max compression
+gzip compressed data, was "dist\PySideSix-Frameless-Window-0.1.1.tar", last modified: Sat Jul  8 13:11:41 2023, max compression
```

## Comparing `PySideSix-Frameless-Window-0.1.0.tar` & `PySideSix-Frameless-Window-0.1.1.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxrwx   0        0        0        0 2023-04-17 07:24:01.418397 PySideSix-Frameless-Window-0.1.0/
--rw-rw-rw-   0        0        0     7815 2023-04-17 07:22:03.000000 PySideSix-Frameless-Window-0.1.0/LICENSE
--rw-rw-rw-   0        0        0     5519 2023-04-17 07:24:01.417322 PySideSix-Frameless-Window-0.1.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-17 07:24:01.377817 PySideSix-Frameless-Window-0.1.0/PySideSix_Frameless_Window.egg-info/
--rw-rw-rw-   0        0        0     5519 2023-04-17 07:24:01.000000 PySideSix-Frameless-Window-0.1.0/PySideSix_Frameless_Window.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      868 2023-04-17 07:24:01.000000 PySideSix-Frameless-Window-0.1.0/PySideSix_Frameless_Window.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-17 07:24:01.000000 PySideSix-Frameless-Window-0.1.0/PySideSix_Frameless_Window.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       88 2023-04-17 07:24:01.000000 PySideSix-Frameless-Window-0.1.0/PySideSix_Frameless_Window.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-04-17 07:24:01.000000 PySideSix-Frameless-Window-0.1.0/PySideSix_Frameless_Window.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     4927 2023-04-17 07:22:03.000000 PySideSix-Frameless-Window-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-17 07:24:01.379900 PySideSix-Frameless-Window-0.1.0/qframelesswindow/
--rw-rw-rw-   0        0        0     1614 2023-04-17 07:22:33.000000 PySideSix-Frameless-Window-0.1.0/qframelesswindow/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-17 07:24:01.384387 PySideSix-Frameless-Window-0.1.0/qframelesswindow/_rc/
--rw-rw-rw-   0        0        0        0 2023-01-28 14:21:55.000000 PySideSix-Frameless-Window-0.1.0/qframelesswindow/_rc/__init__.py
--rw-rw-rw-   0        0        0     1477 2023-04-17 07:22:03.000000 PySideSix-Frameless-Window-0.1.0/qframelesswindow/_rc/resource.py
-drwxrwxrwx   0        0        0        0 2023-04-17 07:24:01.388872 PySideSix-Frameless-Window-0.1.0/qframelesswindow/linux/
--rw-rw-rw-   0        0        0     4320 2023-04-17 07:22:03.000000 PySideSix-Frameless-Window-0.1.0/qframelesswindow/linux/__init__.py
--rw-rw-rw-   0        0        0     2918 2023-04-17 07:22:03.000000 PySideSix-Frameless-Window-0.1.0/qframelesswindow/linux/window_effect.py
-drwxrwxrwx   0        0        0        0 2023-04-17 07:24:01.394310 PySideSix-Frameless-Window-0.1.0/qframelesswindow/mac/
--rw-rw-rw-   0        0        0     4529 2023-04-17 07:22:03.000000 PySideSix-Frameless-Window-0.1.0/qframelesswindow/mac/__init__.py
--rw-rw-rw-   0        0        0     4320 2023-04-17 07:22:03.000000 PySideSix-Frameless-Window-0.1.0/qframelesswindow/mac/window_effect.py
-drwxrwxrwx   0        0        0        0 2023-04-17 07:24:01.398503 PySideSix-Frameless-Window-0.1.0/qframelesswindow/titlebar/
--rw-rw-rw-   0        0        0     5062 2023-04-17 07:22:03.000000 PySideSix-Frameless-Window-0.1.0/qframelesswindow/titlebar/__init__.py
--rw-rw-rw-   0        0        0     9039 2023-04-17 07:22:03.000000 PySideSix-Frameless-Window-0.1.0/qframelesswindow/titlebar/title_bar_buttons.py
-drwxrwxrwx   0        0        0        0 2023-04-17 07:24:01.407557 PySideSix-Frameless-Window-0.1.0/qframelesswindow/utils/
--rw-rw-rw-   0        0        0      885 2022-07-25 01:20:40.000000 PySideSix-Frameless-Window-0.1.0/qframelesswindow/utils/__init__.py
--rw-rw-rw-   0        0        0     1216 2023-04-17 07:22:03.000000 PySideSix-Frameless-Window-0.1.0/qframelesswindow/utils/linux_utils.py
--rw-rw-rw-   0        0        0     1844 2023-04-17 07:22:03.000000 PySideSix-Frameless-Window-0.1.0/qframelesswindow/utils/mac_utils.py
--rw-rw-rw-   0        0        0     8093 2023-04-17 07:22:38.000000 PySideSix-Frameless-Window-0.1.0/qframelesswindow/utils/win32_utils.py
-drwxrwxrwx   0        0        0        0 2023-04-17 07:24:01.415177 PySideSix-Frameless-Window-0.1.0/qframelesswindow/windows/
--rw-rw-rw-   0        0        0     8180 2023-04-17 07:22:03.000000 PySideSix-Frameless-Window-0.1.0/qframelesswindow/windows/__init__.py
--rw-rw-rw-   0        0        0     4261 2023-04-17 07:22:03.000000 PySideSix-Frameless-Window-0.1.0/qframelesswindow/windows/c_structures.py
--rw-rw-rw-   0        0        0     8905 2023-04-17 07:22:03.000000 PySideSix-Frameless-Window-0.1.0/qframelesswindow/windows/window_effect.py
--rw-rw-rw-   0        0        0       42 2023-04-17 07:24:01.418397 PySideSix-Frameless-Window-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1003 2023-04-17 07:22:24.000000 PySideSix-Frameless-Window-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-08 13:11:41.949763 PySideSix-Frameless-Window-0.1.1/
+-rw-rw-rw-   0        0        0     7815 2023-07-08 13:07:29.000000 PySideSix-Frameless-Window-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0     5519 2023-07-08 13:11:41.948742 PySideSix-Frameless-Window-0.1.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-08 13:11:41.900262 PySideSix-Frameless-Window-0.1.1/PySideSix_Frameless_Window.egg-info/
+-rw-rw-rw-   0        0        0     5519 2023-07-08 13:11:41.000000 PySideSix-Frameless-Window-0.1.1/PySideSix_Frameless_Window.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      868 2023-07-08 13:11:41.000000 PySideSix-Frameless-Window-0.1.1/PySideSix_Frameless_Window.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-08 13:11:41.000000 PySideSix-Frameless-Window-0.1.1/PySideSix_Frameless_Window.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       88 2023-07-08 13:11:41.000000 PySideSix-Frameless-Window-0.1.1/PySideSix_Frameless_Window.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-07-08 13:11:41.000000 PySideSix-Frameless-Window-0.1.1/PySideSix_Frameless_Window.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     4927 2023-07-08 13:07:29.000000 PySideSix-Frameless-Window-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-08 13:11:41.911055 PySideSix-Frameless-Window-0.1.1/qframelesswindow/
+-rw-rw-rw-   0        0        0     1614 2023-07-08 13:08:40.000000 PySideSix-Frameless-Window-0.1.1/qframelesswindow/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-08 13:11:41.915335 PySideSix-Frameless-Window-0.1.1/qframelesswindow/_rc/
+-rw-rw-rw-   0        0        0        0 2023-01-28 14:21:55.000000 PySideSix-Frameless-Window-0.1.1/qframelesswindow/_rc/__init__.py
+-rw-rw-rw-   0        0        0     1477 2023-07-08 13:07:29.000000 PySideSix-Frameless-Window-0.1.1/qframelesswindow/_rc/resource.py
+drwxrwxrwx   0        0        0        0 2023-07-08 13:11:41.919688 PySideSix-Frameless-Window-0.1.1/qframelesswindow/linux/
+-rw-rw-rw-   0        0        0     4320 2023-07-08 13:07:29.000000 PySideSix-Frameless-Window-0.1.1/qframelesswindow/linux/__init__.py
+-rw-rw-rw-   0        0        0     3147 2023-07-08 13:08:00.000000 PySideSix-Frameless-Window-0.1.1/qframelesswindow/linux/window_effect.py
+drwxrwxrwx   0        0        0        0 2023-07-08 13:11:41.924514 PySideSix-Frameless-Window-0.1.1/qframelesswindow/mac/
+-rw-rw-rw-   0        0        0     4529 2023-07-08 13:07:29.000000 PySideSix-Frameless-Window-0.1.1/qframelesswindow/mac/__init__.py
+-rw-rw-rw-   0        0        0     4549 2023-07-08 13:07:53.000000 PySideSix-Frameless-Window-0.1.1/qframelesswindow/mac/window_effect.py
+drwxrwxrwx   0        0        0        0 2023-07-08 13:11:41.928272 PySideSix-Frameless-Window-0.1.1/qframelesswindow/titlebar/
+-rw-rw-rw-   0        0        0     5062 2023-07-08 13:07:29.000000 PySideSix-Frameless-Window-0.1.1/qframelesswindow/titlebar/__init__.py
+-rw-rw-rw-   0        0        0     9039 2023-07-08 13:07:29.000000 PySideSix-Frameless-Window-0.1.1/qframelesswindow/titlebar/title_bar_buttons.py
+drwxrwxrwx   0        0        0        0 2023-07-08 13:11:41.934270 PySideSix-Frameless-Window-0.1.1/qframelesswindow/utils/
+-rw-rw-rw-   0        0        0      885 2022-07-25 01:20:40.000000 PySideSix-Frameless-Window-0.1.1/qframelesswindow/utils/__init__.py
+-rw-rw-rw-   0        0        0     1216 2023-07-08 13:07:29.000000 PySideSix-Frameless-Window-0.1.1/qframelesswindow/utils/linux_utils.py
+-rw-rw-rw-   0        0        0     1844 2023-07-08 13:07:29.000000 PySideSix-Frameless-Window-0.1.1/qframelesswindow/utils/mac_utils.py
+-rw-rw-rw-   0        0        0     8093 2023-07-08 13:07:29.000000 PySideSix-Frameless-Window-0.1.1/qframelesswindow/utils/win32_utils.py
+drwxrwxrwx   0        0        0        0 2023-07-08 13:11:41.942680 PySideSix-Frameless-Window-0.1.1/qframelesswindow/windows/
+-rw-rw-rw-   0        0        0     8243 2023-07-08 13:09:21.000000 PySideSix-Frameless-Window-0.1.1/qframelesswindow/windows/__init__.py
+-rw-rw-rw-   0        0        0     4261 2023-07-08 13:07:29.000000 PySideSix-Frameless-Window-0.1.1/qframelesswindow/windows/c_structures.py
+-rw-rw-rw-   0        0        0     9369 2023-07-08 13:07:42.000000 PySideSix-Frameless-Window-0.1.1/qframelesswindow/windows/window_effect.py
+-rw-rw-rw-   0        0        0       42 2023-07-08 13:11:41.949763 PySideSix-Frameless-Window-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1003 2023-07-08 13:08:36.000000 PySideSix-Frameless-Window-0.1.1/setup.py
```

### Comparing `PySideSix-Frameless-Window-0.1.0/LICENSE` & `PySideSix-Frameless-Window-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `PySideSix-Frameless-Window-0.1.0/PKG-INFO` & `PySideSix-Frameless-Window-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PySideSix-Frameless-Window
-Version: 0.1.0
+Version: 0.1.1
 Summary: A cross-platform frameless window based on pyside6, support Win32, Linux and macOS.
 Home-page: https://github.com/zhiyiYo/PyQt-Frameless-Window/tree/PySide6
 Author: zhiyiYo
 Author-email: shokokawaii@outlook.com
 License: LGPLv3
 Keywords: pyside6 frameless
 Classifier: Programming Language :: Python :: 3
```

### Comparing `PySideSix-Frameless-Window-0.1.0/PySideSix_Frameless_Window.egg-info/PKG-INFO` & `PySideSix-Frameless-Window-0.1.1/PySideSix_Frameless_Window.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PySideSix-Frameless-Window
-Version: 0.1.0
+Version: 0.1.1
 Summary: A cross-platform frameless window based on pyside6, support Win32, Linux and macOS.
 Home-page: https://github.com/zhiyiYo/PyQt-Frameless-Window/tree/PySide6
 Author: zhiyiYo
 Author-email: shokokawaii@outlook.com
 License: LGPLv3
 Keywords: pyside6 frameless
 Classifier: Programming Language :: Python :: 3
```

### Comparing `PySideSix-Frameless-Window-0.1.0/PySideSix_Frameless_Window.egg-info/SOURCES.txt` & `PySideSix-Frameless-Window-0.1.1/PySideSix_Frameless_Window.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PySideSix-Frameless-Window-0.1.0/README.md` & `PySideSix-Frameless-Window-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `PySideSix-Frameless-Window-0.1.0/qframelesswindow/__init__.py` & `PySideSix-Frameless-Window-0.1.1/qframelesswindow/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 Examples are available at https://github.com/zhiyiYo/PyQt-Frameless-Window/tree/PySide6/examples.
 
 :copyright: (c) 2021 by zhiyiYo.
 :license: LGPLv3, see LICENSE for more details.
 """
 
-__version__ = "0.1.0"
+__version__ = "0.1.1"
 
 import sys
 
 from PySide6.QtCore import Qt
 from PySide6.QtWidgets import QDialog, QMainWindow
 
 from .titlebar import TitleBar, TitleBarButton, SvgTitleBarButton, StandardTitleBar
```

### Comparing `PySideSix-Frameless-Window-0.1.0/qframelesswindow/_rc/resource.py` & `PySideSix-Frameless-Window-0.1.1/qframelesswindow/_rc/resource.py`

 * *Files identical despite different names*

### Comparing `PySideSix-Frameless-Window-0.1.0/qframelesswindow/linux/__init__.py` & `PySideSix-Frameless-Window-0.1.1/qframelesswindow/linux/__init__.py`

 * *Files identical despite different names*

### Comparing `PySideSix-Frameless-Window-0.1.0/qframelesswindow/linux/window_effect.py` & `PySideSix-Frameless-Window-0.1.1/qframelesswindow/linux/window_effect.py`

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
         """
```

### Comparing `PySideSix-Frameless-Window-0.1.0/qframelesswindow/mac/__init__.py` & `PySideSix-Frameless-Window-0.1.1/qframelesswindow/mac/__init__.py`

 * *Files identical despite different names*

### Comparing `PySideSix-Frameless-Window-0.1.0/qframelesswindow/mac/window_effect.py` & `PySideSix-Frameless-Window-0.1.1/qframelesswindow/mac/window_effect.py`

 * *Files 2% similar despite different names*

```diff
@@ -143,14 +143,24 @@
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
         """
```

### Comparing `PySideSix-Frameless-Window-0.1.0/qframelesswindow/titlebar/__init__.py` & `PySideSix-Frameless-Window-0.1.1/qframelesswindow/titlebar/__init__.py`

 * *Files identical despite different names*

### Comparing `PySideSix-Frameless-Window-0.1.0/qframelesswindow/titlebar/title_bar_buttons.py` & `PySideSix-Frameless-Window-0.1.1/qframelesswindow/titlebar/title_bar_buttons.py`

 * *Files identical despite different names*

### Comparing `PySideSix-Frameless-Window-0.1.0/qframelesswindow/utils/__init__.py` & `PySideSix-Frameless-Window-0.1.1/qframelesswindow/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `PySideSix-Frameless-Window-0.1.0/qframelesswindow/utils/linux_utils.py` & `PySideSix-Frameless-Window-0.1.1/qframelesswindow/utils/linux_utils.py`

 * *Files identical despite different names*

### Comparing `PySideSix-Frameless-Window-0.1.0/qframelesswindow/utils/mac_utils.py` & `PySideSix-Frameless-Window-0.1.1/qframelesswindow/utils/mac_utils.py`

 * *Files identical despite different names*

### Comparing `PySideSix-Frameless-Window-0.1.0/qframelesswindow/utils/win32_utils.py` & `PySideSix-Frameless-Window-0.1.1/qframelesswindow/utils/win32_utils.py`

 * *Files identical despite different names*

### Comparing `PySideSix-Frameless-Window-0.1.0/qframelesswindow/windows/__init__.py` & `PySideSix-Frameless-Window-0.1.1/qframelesswindow/windows/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -219,13 +219,14 @@
 
     def __init__(self, parent=None):
         super().__init__(parent=parent)
         self._initFrameless()
         self.titleBar.minBtn.hide()
         self.titleBar.maxBtn.hide()
         self.titleBar.setDoubleClickEnabled(False)
+        self.windowEffect.disableMaximizeButton(self.winId())
 
     def resizeEvent(self, e):
         WindowsFramelessWindowBase.resizeEvent(self, e)
 
     def nativeEvent(self, eventType, message):
         return WindowsFramelessWindowBase.nativeEvent(self, eventType, message)
```

### Comparing `PySideSix-Frameless-Window-0.1.0/qframelesswindow/windows/c_structures.py` & `PySideSix-Frameless-Window-0.1.1/qframelesswindow/windows/c_structures.py`

 * *Files identical despite different names*

### Comparing `PySideSix-Frameless-Window-0.1.0/qframelesswindow/windows/window_effect.py` & `PySideSix-Frameless-Window-0.1.1/qframelesswindow/windows/window_effect.py`

 * *Files 4% similar despite different names*

```diff
@@ -238,14 +238,31 @@
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
         """
```

### Comparing `PySideSix-Frameless-Window-0.1.0/setup.py` & `PySideSix-Frameless-Window-0.1.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 with open('README.md', encoding='utf-8') as f:
     long_description = f.read()
 
 setuptools.setup(
     name="PySideSix-Frameless-Window",
-    version="0.1.0",
+    version="0.1.1",
     keywords="pyside6 frameless",
     author="zhiyiYo",
     author_email="shokokawaii@outlook.com",
     description="A cross-platform frameless window based on pyside6, support Win32, Linux and macOS.",
     long_description=long_description,
     long_description_content_type='text/markdown',
     license="LGPLv3",
```

