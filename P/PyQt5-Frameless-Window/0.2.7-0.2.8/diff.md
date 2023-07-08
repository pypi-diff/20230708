# Comparing `tmp/PyQt5-Frameless-Window-0.2.7.tar.gz` & `tmp/PyQt5-Frameless-Window-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\PyQt5-Frameless-Window-0.2.7.tar", last modified: Mon May  8 13:19:02 2023, max compression
+gzip compressed data, was "dist\PyQt5-Frameless-Window-0.2.8.tar", last modified: Sat Jul  8 13:06:26 2023, max compression
```

## Comparing `PyQt5-Frameless-Window-0.2.7.tar` & `PyQt5-Frameless-Window-0.2.8.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxrwx   0        0        0        0 2023-05-08 13:19:01.995115 PyQt5-Frameless-Window-0.2.7/
--rw-rw-rw-   0        0        0    35823 2023-04-29 16:05:01.000000 PyQt5-Frameless-Window-0.2.7/LICENSE
--rw-rw-rw-   0        0        0     5051 2023-05-08 13:19:01.995115 PyQt5-Frameless-Window-0.2.7/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-08 13:19:01.967979 PyQt5-Frameless-Window-0.2.7/PyQt5_Frameless_Window.egg-info/
--rw-rw-rw-   0        0        0     5051 2023-05-08 13:19:01.000000 PyQt5-Frameless-Window-0.2.7/PyQt5_Frameless_Window.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      848 2023-05-08 13:19:01.000000 PyQt5-Frameless-Window-0.2.7/PyQt5_Frameless_Window.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-08 13:19:01.000000 PyQt5-Frameless-Window-0.2.7/PyQt5_Frameless_Window.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      126 2023-05-08 13:19:01.000000 PyQt5-Frameless-Window-0.2.7/PyQt5_Frameless_Window.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-05-08 13:19:01.000000 PyQt5-Frameless-Window-0.2.7/PyQt5_Frameless_Window.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     4481 2023-04-29 16:05:01.000000 PyQt5-Frameless-Window-0.2.7/README.md
-drwxrwxrwx   0        0        0        0 2023-05-08 13:19:01.969498 PyQt5-Frameless-Window-0.2.7/qframelesswindow/
--rw-rw-rw-   0        0        0     1616 2023-05-08 13:15:17.000000 PyQt5-Frameless-Window-0.2.7/qframelesswindow/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-08 13:19:01.972501 PyQt5-Frameless-Window-0.2.7/qframelesswindow/_rc/
--rw-rw-rw-   0        0        0        0 2023-01-28 14:21:55.000000 PyQt5-Frameless-Window-0.2.7/qframelesswindow/_rc/__init__.py
--rw-rw-rw-   0        0        0     2728 2023-04-29 16:05:01.000000 PyQt5-Frameless-Window-0.2.7/qframelesswindow/_rc/resource.py
-drwxrwxrwx   0        0        0        0 2023-05-08 13:19:01.976015 PyQt5-Frameless-Window-0.2.7/qframelesswindow/linux/
--rw-rw-rw-   0        0        0     2891 2023-04-29 16:05:01.000000 PyQt5-Frameless-Window-0.2.7/qframelesswindow/linux/__init__.py
--rw-rw-rw-   0        0        0     2904 2023-05-08 13:12:25.000000 PyQt5-Frameless-Window-0.2.7/qframelesswindow/linux/window_effect.py
-drwxrwxrwx   0        0        0        0 2023-05-08 13:19:01.978256 PyQt5-Frameless-Window-0.2.7/qframelesswindow/mac/
--rw-rw-rw-   0        0        0     2994 2023-04-29 16:05:01.000000 PyQt5-Frameless-Window-0.2.7/qframelesswindow/mac/__init__.py
--rw-rw-rw-   0        0        0     4119 2023-05-08 13:12:11.000000 PyQt5-Frameless-Window-0.2.7/qframelesswindow/mac/window_effect.py
-drwxrwxrwx   0        0        0        0 2023-05-08 13:19:01.982278 PyQt5-Frameless-Window-0.2.7/qframelesswindow/titlebar/
--rw-rw-rw-   0        0        0     4984 2023-04-29 16:05:01.000000 PyQt5-Frameless-Window-0.2.7/qframelesswindow/titlebar/__init__.py
--rw-rw-rw-   0        0        0     9057 2023-04-29 16:05:01.000000 PyQt5-Frameless-Window-0.2.7/qframelesswindow/titlebar/title_bar_buttons.py
-drwxrwxrwx   0        0        0        0 2023-05-08 13:19:01.988191 PyQt5-Frameless-Window-0.2.7/qframelesswindow/utils/
--rw-rw-rw-   0        0        0      885 2022-07-25 01:20:40.000000 PyQt5-Frameless-Window-0.2.7/qframelesswindow/utils/__init__.py
--rw-rw-rw-   0        0        0     5299 2023-04-29 16:05:01.000000 PyQt5-Frameless-Window-0.2.7/qframelesswindow/utils/linux_utils.py
--rw-rw-rw-   0        0        0     1850 2023-04-29 16:05:01.000000 PyQt5-Frameless-Window-0.2.7/qframelesswindow/utils/mac_utils.py
--rw-rw-rw-   0        0        0     8352 2023-05-08 13:03:27.000000 PyQt5-Frameless-Window-0.2.7/qframelesswindow/utils/win32_utils.py
-drwxrwxrwx   0        0        0        0 2023-05-08 13:19:01.993600 PyQt5-Frameless-Window-0.2.7/qframelesswindow/windows/
--rw-rw-rw-   0        0        0     6942 2023-05-08 13:08:28.000000 PyQt5-Frameless-Window-0.2.7/qframelesswindow/windows/__init__.py
--rw-rw-rw-   0        0        0     4263 2023-05-08 13:07:12.000000 PyQt5-Frameless-Window-0.2.7/qframelesswindow/windows/c_structures.py
--rw-rw-rw-   0        0        0     8523 2023-05-08 13:12:49.000000 PyQt5-Frameless-Window-0.2.7/qframelesswindow/windows/window_effect.py
--rw-rw-rw-   0        0        0       42 2023-05-08 13:19:01.996213 PyQt5-Frameless-Window-0.2.7/setup.cfg
--rw-rw-rw-   0        0        0     1023 2023-05-08 13:15:11.000000 PyQt5-Frameless-Window-0.2.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-08 13:06:26.900991 PyQt5-Frameless-Window-0.2.8/
+-rw-rw-rw-   0        0        0    35823 2023-07-08 12:30:11.000000 PyQt5-Frameless-Window-0.2.8/LICENSE
+-rw-rw-rw-   0        0        0     5320 2023-07-08 13:06:26.900991 PyQt5-Frameless-Window-0.2.8/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-08 13:06:26.865163 PyQt5-Frameless-Window-0.2.8/PyQt5_Frameless_Window.egg-info/
+-rw-rw-rw-   0        0        0     5320 2023-07-08 13:06:26.000000 PyQt5-Frameless-Window-0.2.8/PyQt5_Frameless_Window.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      848 2023-07-08 13:06:26.000000 PyQt5-Frameless-Window-0.2.8/PyQt5_Frameless_Window.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-08 13:06:26.000000 PyQt5-Frameless-Window-0.2.8/PyQt5_Frameless_Window.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      126 2023-07-08 13:06:26.000000 PyQt5-Frameless-Window-0.2.8/PyQt5_Frameless_Window.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-07-08 13:06:26.000000 PyQt5-Frameless-Window-0.2.8/PyQt5_Frameless_Window.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     4750 2023-07-08 12:30:12.000000 PyQt5-Frameless-Window-0.2.8/README.md
+drwxrwxrwx   0        0        0        0 2023-07-08 13:06:26.867253 PyQt5-Frameless-Window-0.2.8/qframelesswindow/
+-rw-rw-rw-   0        0        0     1679 2023-07-08 13:05:13.000000 PyQt5-Frameless-Window-0.2.8/qframelesswindow/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-08 13:06:26.871000 PyQt5-Frameless-Window-0.2.8/qframelesswindow/_rc/
+-rw-rw-rw-   0        0        0        0 2023-01-28 14:21:55.000000 PyQt5-Frameless-Window-0.2.8/qframelesswindow/_rc/__init__.py
+-rw-rw-rw-   0        0        0     2728 2023-07-08 12:30:12.000000 PyQt5-Frameless-Window-0.2.8/qframelesswindow/_rc/resource.py
+drwxrwxrwx   0        0        0        0 2023-07-08 13:06:26.875613 PyQt5-Frameless-Window-0.2.8/qframelesswindow/linux/
+-rw-rw-rw-   0        0        0     2891 2023-07-08 12:30:12.000000 PyQt5-Frameless-Window-0.2.8/qframelesswindow/linux/__init__.py
+-rw-rw-rw-   0        0        0     3119 2023-07-08 13:00:28.000000 PyQt5-Frameless-Window-0.2.8/qframelesswindow/linux/window_effect.py
+drwxrwxrwx   0        0        0        0 2023-07-08 13:06:26.880237 PyQt5-Frameless-Window-0.2.8/qframelesswindow/mac/
+-rw-rw-rw-   0        0        0     2994 2023-07-08 12:30:12.000000 PyQt5-Frameless-Window-0.2.8/qframelesswindow/mac/__init__.py
+-rw-rw-rw-   0        0        0     4334 2023-07-08 13:00:17.000000 PyQt5-Frameless-Window-0.2.8/qframelesswindow/mac/window_effect.py
+drwxrwxrwx   0        0        0        0 2023-07-08 13:06:26.885460 PyQt5-Frameless-Window-0.2.8/qframelesswindow/titlebar/
+-rw-rw-rw-   0        0        0     4984 2023-07-08 12:30:12.000000 PyQt5-Frameless-Window-0.2.8/qframelesswindow/titlebar/__init__.py
+-rw-rw-rw-   0        0        0     9057 2023-07-08 12:30:12.000000 PyQt5-Frameless-Window-0.2.8/qframelesswindow/titlebar/title_bar_buttons.py
+drwxrwxrwx   0        0        0        0 2023-07-08 13:06:26.893014 PyQt5-Frameless-Window-0.2.8/qframelesswindow/utils/
+-rw-rw-rw-   0        0        0      885 2022-07-25 01:20:40.000000 PyQt5-Frameless-Window-0.2.8/qframelesswindow/utils/__init__.py
+-rw-rw-rw-   0        0        0     5299 2023-07-08 12:30:12.000000 PyQt5-Frameless-Window-0.2.8/qframelesswindow/utils/linux_utils.py
+-rw-rw-rw-   0        0        0     1850 2023-07-08 12:30:12.000000 PyQt5-Frameless-Window-0.2.8/qframelesswindow/utils/mac_utils.py
+-rw-rw-rw-   0        0        0     8352 2023-07-08 12:30:12.000000 PyQt5-Frameless-Window-0.2.8/qframelesswindow/utils/win32_utils.py
+drwxrwxrwx   0        0        0        0 2023-07-08 13:06:26.900991 PyQt5-Frameless-Window-0.2.8/qframelesswindow/windows/
+-rw-rw-rw-   0        0        0     6942 2023-07-08 12:30:12.000000 PyQt5-Frameless-Window-0.2.8/qframelesswindow/windows/__init__.py
+-rw-rw-rw-   0        0        0     4263 2023-07-08 12:30:12.000000 PyQt5-Frameless-Window-0.2.8/qframelesswindow/windows/c_structures.py
+-rw-rw-rw-   0        0        0     8987 2023-07-08 12:59:48.000000 PyQt5-Frameless-Window-0.2.8/qframelesswindow/windows/window_effect.py
+-rw-rw-rw-   0        0        0       42 2023-07-08 13:06:26.900991 PyQt5-Frameless-Window-0.2.8/setup.cfg
+-rw-rw-rw-   0        0        0     1023 2023-07-08 13:03:03.000000 PyQt5-Frameless-Window-0.2.8/setup.py
```

### Comparing `PyQt5-Frameless-Window-0.2.7/LICENSE` & `PyQt5-Frameless-Window-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `PyQt5-Frameless-Window-0.2.7/PKG-INFO` & `PyQt5-Frameless-Window-0.2.8/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,7 @@
-Metadata-Version: 2.1
-Name: PyQt5-Frameless-Window
-Version: 0.2.7
-Summary: A cross-platform frameless window based on pyqt5, support Win32, X11, Wayland and macOS.
-Home-page: https://github.com/zhiyiYo/PyQt-Frameless-Window
-Author: zhiyiYo
-Author-email: shokokawaii@outlook.com
-License: GPLv3
-Keywords: pyqt frameless
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <p align="center">
   <img width="15%" align="center" src="screenshot/logo.png" alt="logo">
 </p>
   <h1 align="center">
   PyQt-Frameless-Window
 </h1>
 <p align="center">
@@ -116,21 +101,24 @@
 4. If you encounter this problem on Windows:
    > ImportError: DLL load failed while importing win32api
 
    see my answer on [stackoverflow](https://stackoverflow.com/questions/58612306/how-to-fix-importerror-dll-load-failed-while-importing-win32api/72488468#72488468) or my [blog](https://www.cnblogs.com/zhiyiYo/p/16340429.html) for the solution.
 
 5. If you are using PySide2, PySide6 or PyQt6, you can download the code in [PySide2](https://github.com/zhiyiYo/PyQt-Frameless-Window/tree/Pyside2), [PySide6](https://github.com/zhiyiYo/PyQt-Frameless-Window/tree/PySide6) or [PyQt6](https://github.com/zhiyiYo/PyQt-Frameless-Window/tree/PyQt6) branch.
 
+## Support
+If this project helps you a lot and you want to support the development and maintenance of this project, feel free to sponsor me via [爱发电](https://afdian.net/a/zhiyiYo) or [ko-fi](https://ko-fi.com/zhiyiYo). Your support is highly appreciated 🥰
+
 ## See Also
 Here are some projects that use PyQt-Frameless-Window:
 * [**zhiyiYo/Groove**: A cross-platform music player based on PyQt5](https://github.com/zhiyiYo/Groove)
 * [**zhiyiYo/Alpha-Gobang-Zero**: A gobang robot based on reinforcement learning](https://github.com/zhiyiYo/Alpha-Gobang-Zero)
 * [**zhiyiYo/PyQt-Fluent-Widgets**: A fluent design widgets library based on PyQt5](https://github.com/zhiyiYo/PyQt-Fluent-Widgets)
 
 ## Reference
 * [**wangwenx190/framelesshelper**: Frameless windows for Qt Widgets and Qt Quick applications. Support Win32, X11, Wayland and macOS](https://github.com/wangwenx190/framelesshelper)
 * [**libxcb**: Basic Graphics Programming With The XCB Library](https://www.x.org/releases/X11R7.5/doc/libxcb/tutorial)
 
 ## License
 PyQt-Frameless-Window is licensed under [GPLv3](./LICENSE).
 
-Copyright © 2021 by zhiyiYo.
+Copyright © 2021 by zhiyiYo.
```

### Comparing `PyQt5-Frameless-Window-0.2.7/PyQt5_Frameless_Window.egg-info/PKG-INFO` & `PyQt5-Frameless-Window-0.2.8/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyQt5-Frameless-Window
-Version: 0.2.7
+Version: 0.2.8
 Summary: A cross-platform frameless window based on pyqt5, support Win32, X11, Wayland and macOS.
 Home-page: https://github.com/zhiyiYo/PyQt-Frameless-Window
 Author: zhiyiYo
 Author-email: shokokawaii@outlook.com
 License: GPLv3
 Keywords: pyqt frameless
 Classifier: Programming Language :: Python :: 3
@@ -116,14 +116,17 @@
 4. If you encounter this problem on Windows:
    > ImportError: DLL load failed while importing win32api
 
    see my answer on [stackoverflow](https://stackoverflow.com/questions/58612306/how-to-fix-importerror-dll-load-failed-while-importing-win32api/72488468#72488468) or my [blog](https://www.cnblogs.com/zhiyiYo/p/16340429.html) for the solution.
 
 5. If you are using PySide2, PySide6 or PyQt6, you can download the code in [PySide2](https://github.com/zhiyiYo/PyQt-Frameless-Window/tree/Pyside2), [PySide6](https://github.com/zhiyiYo/PyQt-Frameless-Window/tree/PySide6) or [PyQt6](https://github.com/zhiyiYo/PyQt-Frameless-Window/tree/PyQt6) branch.
 
+## Support
+If this project helps you a lot and you want to support the development and maintenance of this project, feel free to sponsor me via [爱发电](https://afdian.net/a/zhiyiYo) or [ko-fi](https://ko-fi.com/zhiyiYo). Your support is highly appreciated 🥰
+
 ## See Also
 Here are some projects that use PyQt-Frameless-Window:
 * [**zhiyiYo/Groove**: A cross-platform music player based on PyQt5](https://github.com/zhiyiYo/Groove)
 * [**zhiyiYo/Alpha-Gobang-Zero**: A gobang robot based on reinforcement learning](https://github.com/zhiyiYo/Alpha-Gobang-Zero)
 * [**zhiyiYo/PyQt-Fluent-Widgets**: A fluent design widgets library based on PyQt5](https://github.com/zhiyiYo/PyQt-Fluent-Widgets)
 
 ## Reference
```

### Comparing `PyQt5-Frameless-Window-0.2.7/PyQt5_Frameless_Window.egg-info/SOURCES.txt` & `PyQt5-Frameless-Window-0.2.8/PyQt5_Frameless_Window.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PyQt5-Frameless-Window-0.2.7/README.md` & `PyQt5-Frameless-Window-0.2.8/PyQt5_Frameless_Window.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+Metadata-Version: 2.1
+Name: PyQt5-Frameless-Window
+Version: 0.2.8
+Summary: A cross-platform frameless window based on pyqt5, support Win32, X11, Wayland and macOS.
+Home-page: https://github.com/zhiyiYo/PyQt-Frameless-Window
+Author: zhiyiYo
+Author-email: shokokawaii@outlook.com
+License: GPLv3
+Keywords: pyqt frameless
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 <p align="center">
   <img width="15%" align="center" src="screenshot/logo.png" alt="logo">
 </p>
   <h1 align="center">
   PyQt-Frameless-Window
 </h1>
 <p align="center">
@@ -101,21 +116,24 @@
 4. If you encounter this problem on Windows:
    > ImportError: DLL load failed while importing win32api
 
    see my answer on [stackoverflow](https://stackoverflow.com/questions/58612306/how-to-fix-importerror-dll-load-failed-while-importing-win32api/72488468#72488468) or my [blog](https://www.cnblogs.com/zhiyiYo/p/16340429.html) for the solution.
 
 5. If you are using PySide2, PySide6 or PyQt6, you can download the code in [PySide2](https://github.com/zhiyiYo/PyQt-Frameless-Window/tree/Pyside2), [PySide6](https://github.com/zhiyiYo/PyQt-Frameless-Window/tree/PySide6) or [PyQt6](https://github.com/zhiyiYo/PyQt-Frameless-Window/tree/PyQt6) branch.
 
+## Support
+If this project helps you a lot and you want to support the development and maintenance of this project, feel free to sponsor me via [爱发电](https://afdian.net/a/zhiyiYo) or [ko-fi](https://ko-fi.com/zhiyiYo). Your support is highly appreciated 🥰
+
 ## See Also
 Here are some projects that use PyQt-Frameless-Window:
 * [**zhiyiYo/Groove**: A cross-platform music player based on PyQt5](https://github.com/zhiyiYo/Groove)
 * [**zhiyiYo/Alpha-Gobang-Zero**: A gobang robot based on reinforcement learning](https://github.com/zhiyiYo/Alpha-Gobang-Zero)
 * [**zhiyiYo/PyQt-Fluent-Widgets**: A fluent design widgets library based on PyQt5](https://github.com/zhiyiYo/PyQt-Fluent-Widgets)
 
 ## Reference
 * [**wangwenx190/framelesshelper**: Frameless windows for Qt Widgets and Qt Quick applications. Support Win32, X11, Wayland and macOS](https://github.com/wangwenx190/framelesshelper)
 * [**libxcb**: Basic Graphics Programming With The XCB Library](https://www.x.org/releases/X11R7.5/doc/libxcb/tutorial)
 
 ## License
 PyQt-Frameless-Window is licensed under [GPLv3](./LICENSE).
 
-Copyright © 2021 by zhiyiYo.
+Copyright © 2021 by zhiyiYo.
```

### Comparing `PyQt5-Frameless-Window-0.2.7/qframelesswindow/__init__.py` & `PyQt5-Frameless-Window-0.2.8/qframelesswindow/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 Examples are available at https://github.com/zhiyiYo/PyQt-Frameless-Window/tree/master/examples.
 
 :copyright: (c) 2021 by zhiyiYo.
 :license: GPLv3, see LICENSE for more details.
 """
 
-__version__ = "0.2.7"
+__version__ = "0.2.8"
 
 import sys
 
 from PyQt5.QtWidgets import QDialog, QMainWindow
 
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

### Comparing `PyQt5-Frameless-Window-0.2.7/qframelesswindow/_rc/resource.py` & `PyQt5-Frameless-Window-0.2.8/qframelesswindow/_rc/resource.py`

 * *Files identical despite different names*

### Comparing `PyQt5-Frameless-Window-0.2.7/qframelesswindow/linux/__init__.py` & `PyQt5-Frameless-Window-0.2.8/qframelesswindow/linux/__init__.py`

 * *Files identical despite different names*

### Comparing `PyQt5-Frameless-Window-0.2.7/qframelesswindow/linux/window_effect.py` & `PyQt5-Frameless-Window-0.2.8/qframelesswindow/linux/window_effect.py`

 * *Files 6% similar despite different names*

```diff
@@ -111,15 +111,24 @@
         """ Enables the maximize and minimize animation of the window
 
         Parameters
         ----------
         hWnd : int or `sip.voidptr`
             Window handle
         """
-        pass
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
 
     def enableBlurBehindWindow(self, hWnd):
         """ enable the blur effect behind the whole client
         Parameters
         ----------
         hWnd: int or `sip.voidptr`
             Window handle
```

### Comparing `PyQt5-Frameless-Window-0.2.7/qframelesswindow/mac/__init__.py` & `PyQt5-Frameless-Window-0.2.8/qframelesswindow/mac/__init__.py`

 * *Files identical despite different names*

### Comparing `PyQt5-Frameless-Window-0.2.7/qframelesswindow/mac/window_effect.py` & `PyQt5-Frameless-Window-0.2.8/qframelesswindow/mac/window_effect.py`

 * *Files 2% similar despite different names*

```diff
@@ -132,15 +132,24 @@
         """ Enables the maximize and minimize animation of the window
 
         Parameters
         ----------
         hWnd : int or `sip.voidptr`
             Window handle
         """
-        pass
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
 
     def enableBlurBehindWindow(self, hWnd):
         """ enable the blur effect behind the whole client
         Parameters
         ----------
         hWnd: int or `sip.voidptr`
             Window handle
```

### Comparing `PyQt5-Frameless-Window-0.2.7/qframelesswindow/titlebar/__init__.py` & `PyQt5-Frameless-Window-0.2.8/qframelesswindow/titlebar/__init__.py`

 * *Files identical despite different names*

### Comparing `PyQt5-Frameless-Window-0.2.7/qframelesswindow/titlebar/title_bar_buttons.py` & `PyQt5-Frameless-Window-0.2.8/qframelesswindow/titlebar/title_bar_buttons.py`

 * *Files identical despite different names*

### Comparing `PyQt5-Frameless-Window-0.2.7/qframelesswindow/utils/__init__.py` & `PyQt5-Frameless-Window-0.2.8/qframelesswindow/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `PyQt5-Frameless-Window-0.2.7/qframelesswindow/utils/linux_utils.py` & `PyQt5-Frameless-Window-0.2.8/qframelesswindow/utils/linux_utils.py`

 * *Files identical despite different names*

### Comparing `PyQt5-Frameless-Window-0.2.7/qframelesswindow/utils/mac_utils.py` & `PyQt5-Frameless-Window-0.2.8/qframelesswindow/utils/mac_utils.py`

 * *Files identical despite different names*

### Comparing `PyQt5-Frameless-Window-0.2.7/qframelesswindow/utils/win32_utils.py` & `PyQt5-Frameless-Window-0.2.8/qframelesswindow/utils/win32_utils.py`

 * *Files identical despite different names*

### Comparing `PyQt5-Frameless-Window-0.2.7/qframelesswindow/windows/__init__.py` & `PyQt5-Frameless-Window-0.2.8/qframelesswindow/windows/__init__.py`

 * *Files identical despite different names*

### Comparing `PyQt5-Frameless-Window-0.2.7/qframelesswindow/windows/c_structures.py` & `PyQt5-Frameless-Window-0.2.8/qframelesswindow/windows/c_structures.py`

 * *Files identical despite different names*

### Comparing `PyQt5-Frameless-Window-0.2.7/qframelesswindow/windows/window_effect.py` & `PyQt5-Frameless-Window-0.2.8/qframelesswindow/windows/window_effect.py`

 * *Files 2% similar despite different names*

```diff
@@ -223,14 +223,31 @@
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

### Comparing `PyQt5-Frameless-Window-0.2.7/setup.py` & `PyQt5-Frameless-Window-0.2.8/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 with open('README.md', encoding='utf-8') as f:
     long_description = f.read()
 
 setuptools.setup(
     name="PyQt5-Frameless-Window",
-    version="0.2.7",
+    version="0.2.8",
     keywords="pyqt frameless",
     author="zhiyiYo",
     author_email="shokokawaii@outlook.com",
     description="A cross-platform frameless window based on pyqt5, support Win32, X11, Wayland and macOS.",
     long_description=long_description,
     long_description_content_type='text/markdown',
     license="GPLv3",
```

