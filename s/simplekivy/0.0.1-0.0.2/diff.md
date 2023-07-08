# Comparing `tmp/simplekivy-0.0.1.tar.gz` & `tmp/simplekivy-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simplekivy-0.0.1.tar", last modified: Tue Jul  4 16:34:19 2023, max compression
+gzip compressed data, was "simplekivy-0.0.2.tar", last modified: Sat Jul  8 19:37:33 2023, max compression
```

## Comparing `simplekivy-0.0.1.tar` & `simplekivy-0.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 yoyo      (1000) yoyo      (1000)        0 2023-07-04 16:34:19.388476 simplekivy-0.0.1/
--rw-rw-r--   0 yoyo      (1000) yoyo      (1000)     1057 2023-06-26 12:44:34.000000 simplekivy-0.0.1/LICENSE
--rw-rw-r--   0 yoyo      (1000) yoyo      (1000)     3784 2023-07-04 16:34:19.388476 simplekivy-0.0.1/PKG-INFO
--rw-rw-r--   0 yoyo      (1000) yoyo      (1000)     3232 2023-07-04 16:30:44.000000 simplekivy-0.0.1/README.md
--rw-rw-r--   0 yoyo      (1000) yoyo      (1000)      693 2023-07-04 16:34:07.000000 simplekivy-0.0.1/pyproject.toml
--rw-rw-r--   0 yoyo      (1000) yoyo      (1000)       38 2023-07-04 16:34:19.388476 simplekivy-0.0.1/setup.cfg
-drwxrwxr-x   0 yoyo      (1000) yoyo      (1000)        0 2023-07-04 16:34:19.388476 simplekivy-0.0.1/simplekivy/
--rw-rw-r--   0 yoyo      (1000) yoyo      (1000)       35 2023-06-26 13:46:46.000000 simplekivy-0.0.1/simplekivy/__init__.py
--rw-rw-r--   0 yoyo      (1000) yoyo      (1000)      664 2023-07-04 14:52:36.000000 simplekivy-0.0.1/simplekivy/simplekivy.py
-drwxrwxr-x   0 yoyo      (1000) yoyo      (1000)        0 2023-07-04 16:34:19.388476 simplekivy-0.0.1/simplekivy/widgets/
--rw-rw-r--   0 yoyo      (1000) yoyo      (1000)       25 2023-06-25 14:58:13.000000 simplekivy-0.0.1/simplekivy/widgets/__init__.py
--rw-rw-r--   0 yoyo      (1000) yoyo      (1000)     1649 2023-07-04 14:57:24.000000 simplekivy-0.0.1/simplekivy/widgets/app.py
--rw-rw-r--   0 yoyo      (1000) yoyo      (1000)      443 2023-07-03 11:21:37.000000 simplekivy-0.0.1/simplekivy/widgets/main.kv
-drwxrwxr-x   0 yoyo      (1000) yoyo      (1000)        0 2023-07-04 16:34:19.388476 simplekivy-0.0.1/simplekivy.egg-info/
--rw-rw-r--   0 yoyo      (1000) yoyo      (1000)     3784 2023-07-04 16:34:19.000000 simplekivy-0.0.1/simplekivy.egg-info/PKG-INFO
--rw-rw-r--   0 yoyo      (1000) yoyo      (1000)      300 2023-07-04 16:34:19.000000 simplekivy-0.0.1/simplekivy.egg-info/SOURCES.txt
--rw-rw-r--   0 yoyo      (1000) yoyo      (1000)        1 2023-07-04 16:34:19.000000 simplekivy-0.0.1/simplekivy.egg-info/dependency_links.txt
--rw-rw-r--   0 yoyo      (1000) yoyo      (1000)       11 2023-07-04 16:34:19.000000 simplekivy-0.0.1/simplekivy.egg-info/top_level.txt
+drwxrwxr-x   0 yoyo      (1000) yoyo      (1000)        0 2023-07-08 19:37:33.885800 simplekivy-0.0.2/
+-rw-rw-r--   0 yoyo      (1000) yoyo      (1000)     1057 2023-06-26 12:44:34.000000 simplekivy-0.0.2/LICENSE
+-rw-rw-r--   0 yoyo      (1000) yoyo      (1000)     4012 2023-07-08 19:37:33.885800 simplekivy-0.0.2/PKG-INFO
+-rw-rw-r--   0 yoyo      (1000) yoyo      (1000)     3460 2023-07-08 19:35:07.000000 simplekivy-0.0.2/README.md
+-rw-rw-r--   0 yoyo      (1000) yoyo      (1000)      693 2023-07-06 16:21:28.000000 simplekivy-0.0.2/pyproject.toml
+-rw-rw-r--   0 yoyo      (1000) yoyo      (1000)       38 2023-07-08 19:37:33.885800 simplekivy-0.0.2/setup.cfg
+drwxrwxr-x   0 yoyo      (1000) yoyo      (1000)        0 2023-07-08 19:37:33.885800 simplekivy-0.0.2/simplekivy/
+-rw-rw-r--   0 yoyo      (1000) yoyo      (1000)       35 2023-06-26 13:46:46.000000 simplekivy-0.0.2/simplekivy/__init__.py
+-rw-rw-r--   0 yoyo      (1000) yoyo      (1000)      786 2023-07-06 16:35:37.000000 simplekivy-0.0.2/simplekivy/simplekivy.py
+drwxrwxr-x   0 yoyo      (1000) yoyo      (1000)        0 2023-07-08 19:37:33.885800 simplekivy-0.0.2/simplekivy/widgets/
+-rw-rw-r--   0 yoyo      (1000) yoyo      (1000)       25 2023-06-25 14:58:13.000000 simplekivy-0.0.2/simplekivy/widgets/__init__.py
+-rw-rw-r--   0 yoyo      (1000) yoyo      (1000)     1649 2023-07-04 14:57:24.000000 simplekivy-0.0.2/simplekivy/widgets/app.py
+-rw-rw-r--   0 yoyo      (1000) yoyo      (1000)      443 2023-07-03 11:21:37.000000 simplekivy-0.0.2/simplekivy/widgets/main.kv
+drwxrwxr-x   0 yoyo      (1000) yoyo      (1000)        0 2023-07-08 19:37:33.885800 simplekivy-0.0.2/simplekivy.egg-info/
+-rw-rw-r--   0 yoyo      (1000) yoyo      (1000)     4012 2023-07-08 19:37:33.000000 simplekivy-0.0.2/simplekivy.egg-info/PKG-INFO
+-rw-rw-r--   0 yoyo      (1000) yoyo      (1000)      300 2023-07-08 19:37:33.000000 simplekivy-0.0.2/simplekivy.egg-info/SOURCES.txt
+-rw-rw-r--   0 yoyo      (1000) yoyo      (1000)        1 2023-07-08 19:37:33.000000 simplekivy-0.0.2/simplekivy.egg-info/dependency_links.txt
+-rw-rw-r--   0 yoyo      (1000) yoyo      (1000)       11 2023-07-08 19:37:33.000000 simplekivy-0.0.2/simplekivy.egg-info/top_level.txt
```

### Comparing `simplekivy-0.0.1/LICENSE` & `simplekivy-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `simplekivy-0.0.1/PKG-INFO` & `simplekivy-0.0.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,27 @@
 Metadata-Version: 2.1
 Name: simplekivy
-Version: 0.0.1
+Version: 0.0.2
 Summary: the idea is inspired by PySimpleGui , to quickly create simple kivy apps 
 Author-email: yousuf <yosefmahmoud356@gmail.com>
 Project-URL: Homepage, https://github.com/yousuf60/SimpleKivy
 Project-URL: Bug Tracker, https://github.com/yousuf60/SimpleKivy/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # SimpleKivy
 
+```bash
+pip install simplekivy
+```
+
 ### Perfect versions:
 -------
 * [kivy==2.2.1]("https://pypi.org/project/Kivy/2.2.1/") 
 * python >= 3.7
 
 
 simplekivy is built on kivy to write simple code faster
@@ -36,17 +40,17 @@
 ```python
 
 from simplekivy import SimpleKivy
 s = SimpleKivy(title="test")
 dp = s.metrics.dp
 s + [
     (# floatlayout <=> ()
-        {"size_hint": (1, 1)},#<=> add the floatlayout kwargs
+        {"size_hint": (1, None)},#<=> add the floatlayout kwargs
         s.Label(text="ffljwfe", pos_hint={"center_x":.5, "center_y":.5}),
-        {"height":  dp(100)}, #kwargs
+        {"height":  dp(200)}, #kwargs as you want will be added 
     ),
     [ #boxlayout <=> []
         {"size_hint": (1, .5)},
         s.Button(text="gdddg"),
         s.Button(text="gdgdd")
     ],
     
@@ -104,30 +108,30 @@
 ]
 ```
 <img src="https://github.com/yousuf60/SimpleKivy/assets/64571068/997481b1-20cb-4571-91f5-fed311f6f7bc" width="500">
 
 
 
 you can also add kvlang string directly instead of using 
-s.lang.Builder
-or kivy.lang.Builder
+`s.lang.Builder`
+or `kivy.lang.Builder`
 
 ```python
 from simplekivy import SimpleKivy
 s = SimpleKivy(title="test app")
 
 def on_enter(instance):
     print(instance.text)
     
 def btn_pressed():
     print(ainput.text)
 
 
 #add a new method to app
-s.app.btn_pressed = btn_pressed
+s.myapp.btn_pressed = btn_pressed
 
 KV_BTN = """
 
 Button:
     text: "press me"
     size_hint:.4, .1
     pos_hint: {"center_x": .5}
@@ -154,9 +158,13 @@
 <img src="https://github.com/yousuf60/SimpleKivy/assets/64571068/9e9e445e-0c6f-45de-9580-cd7fbde1f010" width="500">
 
 ### Hints
 ------
 
 - list => BoxLayout
 - tuple => FloatLayout
+- set `make_app` to `False` if you do not want to run the kivy App 
+```python
+s = SimpleKivy(make_app=False)
+```
+- to reach the main App object do `s.myapp`
 - the more you understand kivy, the more you enjoy its flexibility
-
```

### Comparing `simplekivy-0.0.1/README.md` & `simplekivy-0.0.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 # SimpleKivy
 
+```bash
+pip install simplekivy
+```
+
 ### Perfect versions:
 -------
 * [kivy==2.2.1]("https://pypi.org/project/Kivy/2.2.1/") 
 * python >= 3.7
 
 
 simplekivy is built on kivy to write simple code faster
@@ -22,17 +26,17 @@
 ```python
 
 from simplekivy import SimpleKivy
 s = SimpleKivy(title="test")
 dp = s.metrics.dp
 s + [
     (# floatlayout <=> ()
-        {"size_hint": (1, 1)},#<=> add the floatlayout kwargs
+        {"size_hint": (1, None)},#<=> add the floatlayout kwargs
         s.Label(text="ffljwfe", pos_hint={"center_x":.5, "center_y":.5}),
-        {"height":  dp(100)}, #kwargs
+        {"height":  dp(200)}, #kwargs as you want will be added 
     ),
     [ #boxlayout <=> []
         {"size_hint": (1, .5)},
         s.Button(text="gdddg"),
         s.Button(text="gdgdd")
     ],
     
@@ -90,30 +94,30 @@
 ]
 ```
 <img src="https://github.com/yousuf60/SimpleKivy/assets/64571068/997481b1-20cb-4571-91f5-fed311f6f7bc" width="500">
 
 
 
 you can also add kvlang string directly instead of using 
-s.lang.Builder
-or kivy.lang.Builder
+`s.lang.Builder`
+or `kivy.lang.Builder`
 
 ```python
 from simplekivy import SimpleKivy
 s = SimpleKivy(title="test app")
 
 def on_enter(instance):
     print(instance.text)
     
 def btn_pressed():
     print(ainput.text)
 
 
 #add a new method to app
-s.app.btn_pressed = btn_pressed
+s.myapp.btn_pressed = btn_pressed
 
 KV_BTN = """
 
 Button:
     text: "press me"
     size_hint:.4, .1
     pos_hint: {"center_x": .5}
@@ -140,9 +144,13 @@
 <img src="https://github.com/yousuf60/SimpleKivy/assets/64571068/9e9e445e-0c6f-45de-9580-cd7fbde1f010" width="500">
 
 ### Hints
 ------
 
 - list => BoxLayout
 - tuple => FloatLayout
+- set `make_app` to `False` if you do not want to run the kivy App 
+```python
+s = SimpleKivy(make_app=False)
+```
+- to reach the main App object do `s.myapp`
 - the more you understand kivy, the more you enjoy its flexibility
-
```

### Comparing `simplekivy-0.0.1/pyproject.toml` & `simplekivy-0.0.2/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "simplekivy"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="yousuf", email="yosefmahmoud356@gmail.com" },
 ]
 description = "the idea is inspired by PySimpleGui , to quickly create simple kivy apps "
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `simplekivy-0.0.1/simplekivy/simplekivy.py` & `simplekivy-0.0.2/simplekivy/simplekivy.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,28 +6,30 @@
 from threading import Thread
 from time import sleep
 
 from .widgets import MainApp
 
 
 class SimpleKivy:
-    def __init__(self, *args, **kwargs):
-        self.app = MainApp(*args, **kwargs)
+    def __init__(self, make_app=True, *args, **kwargs):
+        if make_app:
+            self.myapp = MainApp(*args, **kwargs)
         
     #use + to add widgets
     def __add__(self, widgets):
-        self.app.widgets = widgets
-        self.app.run()        
+        self.myapp.widgets = widgets
+        self.myapp.run()        
          
    
     def __getattr__(self, attr):
         if hasattr(kivy, attr):
             return getattr(kivy, attr)
 
         elif hasattr(F, attr):
             return getattr(F, attr)
 
         else:
             raise Exception(attr + " doasn't exists")
-
+    def get_running_app(self):
+        return kivy.app.App.get_running_app()
```

### Comparing `simplekivy-0.0.1/simplekivy/widgets/app.py` & `simplekivy-0.0.2/simplekivy/widgets/app.py`

 * *Files identical despite different names*

### Comparing `simplekivy-0.0.1/simplekivy.egg-info/PKG-INFO` & `simplekivy-0.0.2/simplekivy.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,27 @@
 Metadata-Version: 2.1
 Name: simplekivy
-Version: 0.0.1
+Version: 0.0.2
 Summary: the idea is inspired by PySimpleGui , to quickly create simple kivy apps 
 Author-email: yousuf <yosefmahmoud356@gmail.com>
 Project-URL: Homepage, https://github.com/yousuf60/SimpleKivy
 Project-URL: Bug Tracker, https://github.com/yousuf60/SimpleKivy/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # SimpleKivy
 
+```bash
+pip install simplekivy
+```
+
 ### Perfect versions:
 -------
 * [kivy==2.2.1]("https://pypi.org/project/Kivy/2.2.1/") 
 * python >= 3.7
 
 
 simplekivy is built on kivy to write simple code faster
@@ -36,17 +40,17 @@
 ```python
 
 from simplekivy import SimpleKivy
 s = SimpleKivy(title="test")
 dp = s.metrics.dp
 s + [
     (# floatlayout <=> ()
-        {"size_hint": (1, 1)},#<=> add the floatlayout kwargs
+        {"size_hint": (1, None)},#<=> add the floatlayout kwargs
         s.Label(text="ffljwfe", pos_hint={"center_x":.5, "center_y":.5}),
-        {"height":  dp(100)}, #kwargs
+        {"height":  dp(200)}, #kwargs as you want will be added 
     ),
     [ #boxlayout <=> []
         {"size_hint": (1, .5)},
         s.Button(text="gdddg"),
         s.Button(text="gdgdd")
     ],
     
@@ -104,30 +108,30 @@
 ]
 ```
 <img src="https://github.com/yousuf60/SimpleKivy/assets/64571068/997481b1-20cb-4571-91f5-fed311f6f7bc" width="500">
 
 
 
 you can also add kvlang string directly instead of using 
-s.lang.Builder
-or kivy.lang.Builder
+`s.lang.Builder`
+or `kivy.lang.Builder`
 
 ```python
 from simplekivy import SimpleKivy
 s = SimpleKivy(title="test app")
 
 def on_enter(instance):
     print(instance.text)
     
 def btn_pressed():
     print(ainput.text)
 
 
 #add a new method to app
-s.app.btn_pressed = btn_pressed
+s.myapp.btn_pressed = btn_pressed
 
 KV_BTN = """
 
 Button:
     text: "press me"
     size_hint:.4, .1
     pos_hint: {"center_x": .5}
@@ -154,9 +158,13 @@
 <img src="https://github.com/yousuf60/SimpleKivy/assets/64571068/9e9e445e-0c6f-45de-9580-cd7fbde1f010" width="500">
 
 ### Hints
 ------
 
 - list => BoxLayout
 - tuple => FloatLayout
+- set `make_app` to `False` if you do not want to run the kivy App 
+```python
+s = SimpleKivy(make_app=False)
+```
+- to reach the main App object do `s.myapp`
 - the more you understand kivy, the more you enjoy its flexibility
-
```

