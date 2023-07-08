# Comparing `tmp/GameWidgets-0.1.7.tar.gz` & `tmp/GameWidgets-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GameWidgets-0.1.7.tar", last modified: Mon Jun 26 18:44:21 2023, max compression
+gzip compressed data, was "GameWidgets-0.1.8.tar", last modified: Sat Jul  8 21:18:25 2023, max compression
```

## Comparing `GameWidgets-0.1.7.tar` & `GameWidgets-0.1.8.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-26 18:44:21.623480 GameWidgets-0.1.7/
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-26 18:44:21.611480 GameWidgets-0.1.7/GameWidgets/
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-26 18:44:21.611480 GameWidgets-0.1.7/GameWidgets/Assets/
--rw-------   0 runner    (1000) runner    (1000)        0 2023-06-26 18:43:15.000000 GameWidgets-0.1.7/GameWidgets/Assets/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-26 18:44:21.611480 GameWidgets-0.1.7/GameWidgets/Engine/
--rw-------   0 runner    (1000) runner    (1000)     1011 2023-06-26 18:43:15.000000 GameWidgets-0.1.7/GameWidgets/Engine/Backdrop.py
--rw-------   0 runner    (1000) runner    (1000)      602 2023-06-26 18:43:15.000000 GameWidgets-0.1.7/GameWidgets/Engine/Entity.py
--rw-------   0 runner    (1000) runner    (1000)     1041 2023-06-26 18:43:15.000000 GameWidgets-0.1.7/GameWidgets/Engine/Group.py
--rw-------   0 runner    (1000) runner    (1000)      122 2023-06-26 18:43:15.000000 GameWidgets-0.1.7/GameWidgets/Engine/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-26 18:44:21.615480 GameWidgets-0.1.7/GameWidgets/Examples/
--rw-------   0 runner    (1000) runner    (1000)     1766 2023-06-26 18:43:15.000000 GameWidgets-0.1.7/GameWidgets/Examples/Widget_Screen_GameWidgets_Example.py
--rw-------   0 runner    (1000) runner    (1000)        4 2023-06-26 18:43:15.000000 GameWidgets-0.1.7/GameWidgets/Examples/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-26 18:44:21.615480 GameWidgets-0.1.7/GameWidgets/GameWidgets/
--rw-------   0 runner    (1000) runner    (1000)     1422 2023-06-26 18:43:15.000000 GameWidgets-0.1.7/GameWidgets/GameWidgets/Animatrix.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-26 18:44:21.615480 GameWidgets-0.1.7/GameWidgets/GameWidgets/Controller/
--rw-------   0 runner    (1000) runner    (1000)     1497 2023-06-26 18:43:15.000000 GameWidgets-0.1.7/GameWidgets/GameWidgets/Controller/Button.py
--rw-------   0 runner    (1000) runner    (1000)     1404 2023-06-26 18:43:15.000000 GameWidgets-0.1.7/GameWidgets/GameWidgets/Controller/Joystick.py
--rw-------   0 runner    (1000) runner    (1000)       13 2023-06-26 18:43:15.000000 GameWidgets-0.1.7/GameWidgets/GameWidgets/Controller/R1_R2.py
--rw-------   0 runner    (1000) runner    (1000)      148 2023-06-26 18:43:15.000000 GameWidgets-0.1.7/GameWidgets/GameWidgets/Controller/__init__.py
--rw-------   0 runner    (1000) runner    (1000)      735 2023-06-26 18:43:15.000000 GameWidgets-0.1.7/GameWidgets/GameWidgets/Draw.py
--rw-------   0 runner    (1000) runner    (1000)      652 2023-06-26 18:43:15.000000 GameWidgets-0.1.7/GameWidgets/GameWidgets/ScreenSlide.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-26 18:44:21.615480 GameWidgets-0.1.7/GameWidgets/GameWidgets/TileMaps/
--rw-------   0 runner    (1000) runner    (1000)      424 2023-06-26 18:43:15.000000 GameWidgets-0.1.7/GameWidgets/GameWidgets/TileMaps/Sprite.py
--rw-------   0 runner    (1000) runner    (1000)      703 2023-06-26 18:43:15.000000 GameWidgets-0.1.7/GameWidgets/GameWidgets/TileMaps/Tile.py
--rw-------   0 runner    (1000) runner    (1000)      124 2023-06-26 18:43:15.000000 GameWidgets-0.1.7/GameWidgets/GameWidgets/TileMaps/__init__.py
--rw-------   0 runner    (1000) runner    (1000)      121 2023-06-26 18:43:15.000000 GameWidgets-0.1.7/GameWidgets/GameWidgets/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-26 18:44:21.619480 GameWidgets-0.1.7/GameWidgets/RuntimeTests/
--rw-------   0 runner    (1000) runner    (1000)      649 2023-06-26 18:43:15.000000 GameWidgets-0.1.7/GameWidgets/RuntimeTests/AllTest.py
--rw-------   0 runner    (1000) runner    (1000)      397 2023-06-26 18:43:15.000000 GameWidgets-0.1.7/GameWidgets/RuntimeTests/GameWidgetTest.py
--rw-------   0 runner    (1000) runner    (1000)      359 2023-06-26 18:43:15.000000 GameWidgets-0.1.7/GameWidgets/RuntimeTests/SetUpTest.py
--rw-------   0 runner    (1000) runner    (1000)      369 2023-06-26 18:43:15.000000 GameWidgets-0.1.7/GameWidgets/RuntimeTests/WidgetTest.py
--rw-------   0 runner    (1000) runner    (1000)        4 2023-06-26 18:43:15.000000 GameWidgets-0.1.7/GameWidgets/RuntimeTests/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-26 18:44:21.619480 GameWidgets-0.1.7/GameWidgets/SetUp/
--rw-------   0 runner    (1000) runner    (1000)     1689 2023-06-26 18:43:15.000000 GameWidgets-0.1.7/GameWidgets/SetUp/ScreenCommands.py
--rw-------   0 runner    (1000) runner    (1000)      109 2023-06-26 18:43:15.000000 GameWidgets-0.1.7/GameWidgets/SetUp/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-26 18:44:21.619480 GameWidgets-0.1.7/GameWidgets/Widgets/
--rw-------   0 runner    (1000) runner    (1000)     3691 2023-06-26 18:43:15.000000 GameWidgets-0.1.7/GameWidgets/Widgets/Btn.py
--rw-------   0 runner    (1000) runner    (1000)      597 2023-06-26 18:43:15.000000 GameWidgets-0.1.7/GameWidgets/Widgets/Clock.py
--rw-------   0 runner    (1000) runner    (1000)     3643 2023-06-26 18:43:15.000000 GameWidgets-0.1.7/GameWidgets/Widgets/Colors.py
--rw-------   0 runner    (1000) runner    (1000)     1489 2023-06-26 18:43:15.000000 GameWidgets-0.1.7/GameWidgets/Widgets/Cursor.py
--rw-------   0 runner    (1000) runner    (1000)     2761 2023-06-26 18:43:15.000000 GameWidgets-0.1.7/GameWidgets/Widgets/DialogeBox.py
--rw-------   0 runner    (1000) runner    (1000)     1574 2023-06-26 18:43:15.000000 GameWidgets-0.1.7/GameWidgets/Widgets/ImgDecoder.py
--rw-------   0 runner    (1000) runner    (1000)      246 2023-06-26 18:43:15.000000 GameWidgets-0.1.7/GameWidgets/Widgets/Sound.py
--rw-------   0 runner    (1000) runner    (1000)     1914 2023-06-26 18:43:15.000000 GameWidgets-0.1.7/GameWidgets/Widgets/TextInp.py
--rw-------   0 runner    (1000) runner    (1000)     2801 2023-06-26 18:43:15.000000 GameWidgets-0.1.7/GameWidgets/Widgets/ToggleBtn.py
--rw-------   0 runner    (1000) runner    (1000)      159 2023-06-26 18:43:15.000000 GameWidgets-0.1.7/GameWidgets/Widgets/__init__.py
--rw-------   0 runner    (1000) runner    (1000)      620 2023-06-26 18:43:15.000000 GameWidgets-0.1.7/GameWidgets/__init__.py
--rw-------   0 runner    (1000) runner    (1000)      567 2023-06-26 18:43:15.000000 GameWidgets-0.1.7/GameWidgets/setup.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-26 18:44:21.611480 GameWidgets-0.1.7/GameWidgets.egg-info/
--rw-r--r--   0 runner    (1000) runner    (1000)      732 2023-06-26 18:44:21.000000 GameWidgets-0.1.7/GameWidgets.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)     1498 2023-06-26 18:44:21.000000 GameWidgets-0.1.7/GameWidgets.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-06-26 18:44:21.000000 GameWidgets-0.1.7/GameWidgets.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        7 2023-06-26 18:44:21.000000 GameWidgets-0.1.7/GameWidgets.egg-info/requires.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       12 2023-06-26 18:44:21.000000 GameWidgets-0.1.7/GameWidgets.egg-info/top_level.txt
--rw-r--r--   0 runner    (1000) runner    (1000)      732 2023-06-26 18:44:21.623480 GameWidgets-0.1.7/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)      385 2022-09-11 21:19:38.000000 GameWidgets-0.1.7/pyproject.toml
--rw-r--r--   0 runner    (1000) runner    (1000)       38 2023-06-26 18:44:21.623480 GameWidgets-0.1.7/setup.cfg
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-08 21:18:25.028021 GameWidgets-0.1.8/
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-08 21:18:25.016021 GameWidgets-0.1.8/GameWidgets/
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-08 21:18:25.016021 GameWidgets-0.1.8/GameWidgets/Assets/
+-rw-------   0 runner    (1000) runner    (1000)        0 2023-07-08 21:17:33.000000 GameWidgets-0.1.8/GameWidgets/Assets/__init__.py
+-rw-------   0 runner    (1000) runner    (1000)     5844 2023-07-08 21:17:33.000000 GameWidgets-0.1.8/GameWidgets/Constants.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-08 21:18:25.016021 GameWidgets-0.1.8/GameWidgets/Engine/
+-rw-------   0 runner    (1000) runner    (1000)     1011 2023-07-08 21:17:33.000000 GameWidgets-0.1.8/GameWidgets/Engine/Backdrop.py
+-rw-------   0 runner    (1000) runner    (1000)      602 2023-07-08 21:17:33.000000 GameWidgets-0.1.8/GameWidgets/Engine/Entity.py
+-rw-------   0 runner    (1000) runner    (1000)     1041 2023-07-08 21:17:33.000000 GameWidgets-0.1.8/GameWidgets/Engine/Group.py
+-rw-------   0 runner    (1000) runner    (1000)      122 2023-07-08 21:17:33.000000 GameWidgets-0.1.8/GameWidgets/Engine/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-08 21:18:25.016021 GameWidgets-0.1.8/GameWidgets/Examples/
+-rw-------   0 runner    (1000) runner    (1000)     1758 2023-07-08 21:17:33.000000 GameWidgets-0.1.8/GameWidgets/Examples/Widget_Screen_GameWidgets_Example.py
+-rw-------   0 runner    (1000) runner    (1000)        4 2023-07-08 21:17:33.000000 GameWidgets-0.1.8/GameWidgets/Examples/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-08 21:18:25.020021 GameWidgets-0.1.8/GameWidgets/GameWidgets/
+-rw-------   0 runner    (1000) runner    (1000)     1422 2023-07-08 21:17:33.000000 GameWidgets-0.1.8/GameWidgets/GameWidgets/Animatrix.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-08 21:18:25.020021 GameWidgets-0.1.8/GameWidgets/GameWidgets/Controller/
+-rw-------   0 runner    (1000) runner    (1000)     1497 2023-07-08 21:17:33.000000 GameWidgets-0.1.8/GameWidgets/GameWidgets/Controller/Button.py
+-rw-------   0 runner    (1000) runner    (1000)     1404 2023-07-08 21:17:33.000000 GameWidgets-0.1.8/GameWidgets/GameWidgets/Controller/Joystick.py
+-rw-------   0 runner    (1000) runner    (1000)       13 2023-07-08 21:17:33.000000 GameWidgets-0.1.8/GameWidgets/GameWidgets/Controller/R1_R2.py
+-rw-------   0 runner    (1000) runner    (1000)      148 2023-07-08 21:17:33.000000 GameWidgets-0.1.8/GameWidgets/GameWidgets/Controller/__init__.py
+-rw-------   0 runner    (1000) runner    (1000)      735 2023-07-08 21:17:33.000000 GameWidgets-0.1.8/GameWidgets/GameWidgets/Draw.py
+-rw-------   0 runner    (1000) runner    (1000)      652 2023-07-08 21:17:33.000000 GameWidgets-0.1.8/GameWidgets/GameWidgets/ScreenSlide.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-08 21:18:25.020021 GameWidgets-0.1.8/GameWidgets/GameWidgets/TileMaps/
+-rw-------   0 runner    (1000) runner    (1000)      424 2023-07-08 21:17:33.000000 GameWidgets-0.1.8/GameWidgets/GameWidgets/TileMaps/Sprite.py
+-rw-------   0 runner    (1000) runner    (1000)      703 2023-07-08 21:17:33.000000 GameWidgets-0.1.8/GameWidgets/GameWidgets/TileMaps/Tile.py
+-rw-------   0 runner    (1000) runner    (1000)      124 2023-07-08 21:17:33.000000 GameWidgets-0.1.8/GameWidgets/GameWidgets/TileMaps/__init__.py
+-rw-------   0 runner    (1000) runner    (1000)      121 2023-07-08 21:17:33.000000 GameWidgets-0.1.8/GameWidgets/GameWidgets/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-08 21:18:25.024021 GameWidgets-0.1.8/GameWidgets/RuntimeTests/
+-rw-------   0 runner    (1000) runner    (1000)      649 2023-07-08 21:17:33.000000 GameWidgets-0.1.8/GameWidgets/RuntimeTests/AllTest.py
+-rw-------   0 runner    (1000) runner    (1000)      397 2023-07-08 21:17:33.000000 GameWidgets-0.1.8/GameWidgets/RuntimeTests/GameWidgetTest.py
+-rw-------   0 runner    (1000) runner    (1000)      359 2023-07-08 21:17:33.000000 GameWidgets-0.1.8/GameWidgets/RuntimeTests/SetUpTest.py
+-rw-------   0 runner    (1000) runner    (1000)      369 2023-07-08 21:17:33.000000 GameWidgets-0.1.8/GameWidgets/RuntimeTests/WidgetTest.py
+-rw-------   0 runner    (1000) runner    (1000)        4 2023-07-08 21:17:33.000000 GameWidgets-0.1.8/GameWidgets/RuntimeTests/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-08 21:18:25.024021 GameWidgets-0.1.8/GameWidgets/SetUp/
+-rw-------   0 runner    (1000) runner    (1000)     1689 2023-07-08 21:17:33.000000 GameWidgets-0.1.8/GameWidgets/SetUp/ScreenCommands.py
+-rw-------   0 runner    (1000) runner    (1000)      109 2023-07-08 21:17:33.000000 GameWidgets-0.1.8/GameWidgets/SetUp/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-08 21:18:25.028021 GameWidgets-0.1.8/GameWidgets/Widgets/
+-rw-------   0 runner    (1000) runner    (1000)     3691 2023-07-08 21:17:33.000000 GameWidgets-0.1.8/GameWidgets/Widgets/Btn.py
+-rw-------   0 runner    (1000) runner    (1000)      597 2023-07-08 21:17:33.000000 GameWidgets-0.1.8/GameWidgets/Widgets/Clock.py
+-rw-------   0 runner    (1000) runner    (1000)     1489 2023-07-08 21:17:33.000000 GameWidgets-0.1.8/GameWidgets/Widgets/Cursor.py
+-rw-------   0 runner    (1000) runner    (1000)     2761 2023-07-08 21:17:33.000000 GameWidgets-0.1.8/GameWidgets/Widgets/DialogeBox.py
+-rw-------   0 runner    (1000) runner    (1000)     1574 2023-07-08 21:17:33.000000 GameWidgets-0.1.8/GameWidgets/Widgets/ImgDecoder.py
+-rw-------   0 runner    (1000) runner    (1000)      246 2023-07-08 21:17:33.000000 GameWidgets-0.1.8/GameWidgets/Widgets/Sound.py
+-rw-------   0 runner    (1000) runner    (1000)     1876 2023-07-08 21:17:33.000000 GameWidgets-0.1.8/GameWidgets/Widgets/TextInp.py
+-rw-------   0 runner    (1000) runner    (1000)     2807 2023-07-08 21:17:33.000000 GameWidgets-0.1.8/GameWidgets/Widgets/ToggleBtn.py
+-rw-------   0 runner    (1000) runner    (1000)      191 2023-07-08 21:17:33.000000 GameWidgets-0.1.8/GameWidgets/Widgets/__init__.py
+-rw-------   0 runner    (1000) runner    (1000)      654 2023-07-08 21:17:33.000000 GameWidgets-0.1.8/GameWidgets/__init__.py
+-rw-------   0 runner    (1000) runner    (1000)      567 2023-07-08 21:17:33.000000 GameWidgets-0.1.8/GameWidgets/setup.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-08 21:18:25.016021 GameWidgets-0.1.8/GameWidgets.egg-info/
+-rw-r--r--   0 runner    (1000) runner    (1000)     1325 2023-07-08 21:18:24.000000 GameWidgets-0.1.8/GameWidgets.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)     1493 2023-07-08 21:18:24.000000 GameWidgets-0.1.8/GameWidgets.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-07-08 21:18:24.000000 GameWidgets-0.1.8/GameWidgets.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        7 2023-07-08 21:18:24.000000 GameWidgets-0.1.8/GameWidgets.egg-info/requires.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       12 2023-07-08 21:18:24.000000 GameWidgets-0.1.8/GameWidgets.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)     1325 2023-07-08 21:18:25.028021 GameWidgets-0.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)      385 2022-09-11 21:19:38.000000 GameWidgets-0.1.8/pyproject.toml
+-rw-r--r--   0 runner    (1000) runner    (1000)       38 2023-07-08 21:18:25.028021 GameWidgets-0.1.8/setup.cfg
```

### Comparing `GameWidgets-0.1.7/GameWidgets/Engine/Backdrop.py` & `GameWidgets-0.1.8/GameWidgets/Engine/Backdrop.py`

 * *Files identical despite different names*

### Comparing `GameWidgets-0.1.7/GameWidgets/Engine/Entity.py` & `GameWidgets-0.1.8/GameWidgets/Engine/Entity.py`

 * *Files identical despite different names*

### Comparing `GameWidgets-0.1.7/GameWidgets/Engine/Group.py` & `GameWidgets-0.1.8/GameWidgets/Engine/Group.py`

 * *Files identical despite different names*

### Comparing `GameWidgets-0.1.7/GameWidgets/Examples/Widget_Screen_GameWidgets_Example.py` & `GameWidgets-0.1.8/GameWidgets/Examples/Widget_Screen_GameWidgets_Example.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # Get all essential Files
-from GameWidgets.Widgets import Colors, Clock, Btn,Cursor
+from GameWidgets.Widgets import Clock, Btn,Cursor
 from GameWidgets.SetUp import ScreenCommands
 from GameWidgets.GameWidgets.ScreenSlide import Slide
 # Pygame is required
 import pygame
 
 # You always have to run the init of pygame
 pygame.init()
```

### Comparing `GameWidgets-0.1.7/GameWidgets/GameWidgets/Animatrix.py` & `GameWidgets-0.1.8/GameWidgets/GameWidgets/Animatrix.py`

 * *Files identical despite different names*

### Comparing `GameWidgets-0.1.7/GameWidgets/GameWidgets/Controller/Button.py` & `GameWidgets-0.1.8/GameWidgets/GameWidgets/Controller/Button.py`

 * *Files identical despite different names*

### Comparing `GameWidgets-0.1.7/GameWidgets/GameWidgets/Controller/Joystick.py` & `GameWidgets-0.1.8/GameWidgets/GameWidgets/Controller/Joystick.py`

 * *Files identical despite different names*

### Comparing `GameWidgets-0.1.7/GameWidgets/GameWidgets/Draw.py` & `GameWidgets-0.1.8/GameWidgets/GameWidgets/Draw.py`

 * *Files identical despite different names*

### Comparing `GameWidgets-0.1.7/GameWidgets/GameWidgets/ScreenSlide.py` & `GameWidgets-0.1.8/GameWidgets/GameWidgets/ScreenSlide.py`

 * *Files identical despite different names*

### Comparing `GameWidgets-0.1.7/GameWidgets/GameWidgets/TileMaps/Tile.py` & `GameWidgets-0.1.8/GameWidgets/GameWidgets/TileMaps/Tile.py`

 * *Files identical despite different names*

### Comparing `GameWidgets-0.1.7/GameWidgets/RuntimeTests/AllTest.py` & `GameWidgets-0.1.8/GameWidgets/RuntimeTests/AllTest.py`

 * *Files identical despite different names*

### Comparing `GameWidgets-0.1.7/GameWidgets/SetUp/ScreenCommands.py` & `GameWidgets-0.1.8/GameWidgets/SetUp/ScreenCommands.py`

 * *Files identical despite different names*

### Comparing `GameWidgets-0.1.7/GameWidgets/Widgets/Btn.py` & `GameWidgets-0.1.8/GameWidgets/Widgets/Btn.py`

 * *Files identical despite different names*

### Comparing `GameWidgets-0.1.7/GameWidgets/Widgets/Clock.py` & `GameWidgets-0.1.8/GameWidgets/Widgets/Clock.py`

 * *Files identical despite different names*

### Comparing `GameWidgets-0.1.7/GameWidgets/Widgets/Cursor.py` & `GameWidgets-0.1.8/GameWidgets/Widgets/Cursor.py`

 * *Files identical despite different names*

### Comparing `GameWidgets-0.1.7/GameWidgets/Widgets/DialogeBox.py` & `GameWidgets-0.1.8/GameWidgets/Widgets/DialogeBox.py`

 * *Files identical despite different names*

### Comparing `GameWidgets-0.1.7/GameWidgets/Widgets/ImgDecoder.py` & `GameWidgets-0.1.8/GameWidgets/Widgets/ImgDecoder.py`

 * *Files identical despite different names*

### Comparing `GameWidgets-0.1.7/GameWidgets/Widgets/TextInp.py` & `GameWidgets-0.1.8/GameWidgets/Widgets/TextInp.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,15 +12,14 @@
         self.d=Disarmed_FG
         self.bg=Outline_Color
     def Update(self):
         if self.active:
             text=self.font.render(str(self.val),(255,0,0),self.a)
         else:
             text=self.font.render(str(self.val),(255,255,255),self.d)
-        self.screen.fill((0,150,150))
         self.screen.blit(text,(self.pos[0]+5,self.pos[1]+5))
         self.rect=text.get_rect(topleft=self.pos)
         rect1=self.rect.copy()
         if self.rect.width<self.width:
             rect1.width=self.width
             rect1.height+=10
             rect1.topleft=self.pos
```

### Comparing `GameWidgets-0.1.7/GameWidgets/Widgets/ToggleBtn.py` & `GameWidgets-0.1.8/GameWidgets/Widgets/ToggleBtn.py`

 * *Files 0% similar despite different names*

```diff
@@ -63,12 +63,12 @@
 
             if event.type == pygame.MOUSEBUTTONDOWN:
                 if self.state==1:
                     self.state = 0
                 else:
                    self.state+=1
 
-class MultiStateSim:
+'''class MultiStateSim:
     def __init__(self,screen, states:tuple,messages:tuple,default:int, xy:tuple,
                  size:tuple):
         self.screen = screen
-
+'''
```

### Comparing `GameWidgets-0.1.7/GameWidgets/__init__.py` & `GameWidgets-0.1.8/GameWidgets/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     from GameWidgets.GameWidgets import *
 except:
     print('GameWidgets.GameWidgets File has been edited, moved, or deleted')
 try:
     from GameWidgets.SetUp import *
 except:
     print('GameWidgets.SetUp File has been edited, moved, or deleted')'''
+from GameWidgets import Constants
 print('GameWidgets Active!')
 __author__='Manomay Tyagi'
 __credits__='Tyagi Family'
 '''__Widgets__=Automatic Import:
 Btn
 Clock
 Colors
```

### Comparing `GameWidgets-0.1.7/GameWidgets/setup.py` & `GameWidgets-0.1.8/GameWidgets/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
   
 with open("GameWidgets/README.md", "r") as fh:
     description = fh.read()
   
 setup(
     name="GameWidgets",
-    version="0.1.7",
+    version="0.1.8",
     author="Manomay tyagi",
     author_email="tyagimanomay57@gmail.com",
     description="Make Game Easier with pygame and GameWidgets",
     long_description=description,
     long_description_content_type="text/markdown",
     url="https://github.com/SuperGuy123456/GameWidgets",
     license='MIT',
```

### Comparing `GameWidgets-0.1.7/GameWidgets.egg-info/SOURCES.txt` & `GameWidgets-0.1.8/GameWidgets.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 pyproject.toml
+GameWidgets/Constants.py
 GameWidgets/__init__.py
 GameWidgets/setup.py
 GameWidgets.egg-info/PKG-INFO
 GameWidgets.egg-info/SOURCES.txt
 GameWidgets.egg-info/dependency_links.txt
 GameWidgets.egg-info/requires.txt
 GameWidgets.egg-info/top_level.txt
@@ -29,15 +30,14 @@
 GameWidgets/RuntimeTests/SetUpTest.py
 GameWidgets/RuntimeTests/WidgetTest.py
 GameWidgets/RuntimeTests/__init__.py
 GameWidgets/SetUp/ScreenCommands.py
 GameWidgets/SetUp/__init__.py
 GameWidgets/Widgets/Btn.py
 GameWidgets/Widgets/Clock.py
-GameWidgets/Widgets/Colors.py
 GameWidgets/Widgets/Cursor.py
 GameWidgets/Widgets/DialogeBox.py
 GameWidgets/Widgets/ImgDecoder.py
 GameWidgets/Widgets/Sound.py
 GameWidgets/Widgets/TextInp.py
 GameWidgets/Widgets/ToggleBtn.py
 GameWidgets/Widgets/__init__.py
```

