# Comparing `tmp/MusicBGX-1.0.0.tar.gz` & `tmp/MusicBGX-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MusicBGX-1.0.0.tar", last modified: Sat Jul  8 12:46:45 2023, max compression
+gzip compressed data, was "MusicBGX-1.0.5.tar", last modified: Sat Jul  8 13:32:01 2023, max compression
```

## Comparing `MusicBGX-1.0.0.tar` & `MusicBGX-1.0.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-07-08 12:46:45.620111 MusicBGX-1.0.0/
--rw-rw-rw-   0        0        0     1067 2023-07-08 08:12:01.000000 MusicBGX-1.0.0/LICENSE
-drwxrwxrwx   0        0        0        0 2023-07-08 12:46:45.452068 MusicBGX-1.0.0/MusicBGX/
--rw-rw-rw-   0        0        0      390 2023-07-08 12:37:17.000000 MusicBGX-1.0.0/MusicBGX/Bg.py
-drwxrwxrwx   0        0        0        0 2023-07-08 12:46:45.607104 MusicBGX-1.0.0/MusicBGX.egg-info/
--rw-rw-rw-   0        0        0      627 2023-07-08 12:46:45.000000 MusicBGX-1.0.0/MusicBGX.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      210 2023-07-08 12:46:45.000000 MusicBGX-1.0.0/MusicBGX.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-08 12:46:45.000000 MusicBGX-1.0.0/MusicBGX.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-07-08 12:46:45.000000 MusicBGX-1.0.0/MusicBGX.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-07-08 12:46:45.000000 MusicBGX-1.0.0/MusicBGX.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      627 2023-07-08 12:46:45.640110 MusicBGX-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0      247 2023-07-08 12:45:44.000000 MusicBGX-1.0.0/README.md
--rw-rw-rw-   0        0        0       81 2023-07-08 12:46:45.662119 MusicBGX-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      694 2023-07-08 12:45:38.000000 MusicBGX-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-08 13:32:01.275042 MusicBGX-1.0.5/
+-rw-rw-rw-   0        0        0     1067 2023-07-08 08:12:01.000000 MusicBGX-1.0.5/LICENSE
+drwxrwxrwx   0        0        0        0 2023-07-08 13:32:00.969973 MusicBGX-1.0.5/MusicBGX/
+-rw-rw-rw-   0        0        0      520 2023-07-08 13:09:04.000000 MusicBGX-1.0.5/MusicBGX/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-08 13:32:01.242040 MusicBGX-1.0.5/MusicBGX.egg-info/
+-rw-rw-rw-   0        0        0      622 2023-07-08 13:32:00.000000 MusicBGX-1.0.5/MusicBGX.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      216 2023-07-08 13:32:00.000000 MusicBGX-1.0.5/MusicBGX.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-08 13:32:00.000000 MusicBGX-1.0.5/MusicBGX.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-07-08 13:32:00.000000 MusicBGX-1.0.5/MusicBGX.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-08 13:32:00.000000 MusicBGX-1.0.5/MusicBGX.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      622 2023-07-08 13:32:01.290069 MusicBGX-1.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0      242 2023-07-08 13:10:30.000000 MusicBGX-1.0.5/README.md
+-rw-rw-rw-   0        0        0       81 2023-07-08 13:32:01.298059 MusicBGX-1.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      694 2023-07-08 13:16:12.000000 MusicBGX-1.0.5/setup.py
```

### Comparing `MusicBGX-1.0.0/LICENSE` & `MusicBGX-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `MusicBGX-1.0.0/MusicBGX.egg-info/PKG-INFO` & `MusicBGX-1.0.5/MusicBGX.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MusicBGX
-Version: 1.0.0
+Version: 1.0.5
 Summary: A light and simple library for playing offline and online music in the background (:
 Home-page: https://github.com/aminrngbr1122
 Author: Amin Rngbr
 Author-email: rngbramin@gmail.com
 Keywords: music
 Requires-Python: >=3.4
 Description-Content-Type: text/markdown
@@ -15,17 +15,17 @@
 ```sh
 pip install MusicBGX
 ```
 
 ## Useage
 
 ```python
-from MusicBg import Bg
-back = Bg.BackGround(path)
-back.play_background_music()
+from MusicBGX import *
+app = BackGround(path)
+app.play_background_music()
 ```
 
 ## Project status
 
 - Alpha
 
 ## Author
```

### Comparing `MusicBGX-1.0.0/PKG-INFO` & `MusicBGX-1.0.5/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MusicBGX
-Version: 1.0.0
+Version: 1.0.5
 Summary: A light and simple library for playing offline and online music in the background (:
 Home-page: https://github.com/aminrngbr1122
 Author: Amin Rngbr
 Author-email: rngbramin@gmail.com
 Keywords: music
 Requires-Python: >=3.4
 Description-Content-Type: text/markdown
@@ -15,17 +15,17 @@
 ```sh
 pip install MusicBGX
 ```
 
 ## Useage
 
 ```python
-from MusicBg import Bg
-back = Bg.BackGround(path)
-back.play_background_music()
+from MusicBGX import *
+app = BackGround(path)
+app.play_background_music()
 ```
 
 ## Project status
 
 - Alpha
 
 ## Author
```

### Comparing `MusicBGX-1.0.0/setup.py` & `MusicBGX-1.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open('README.md', "r") as f:
     long_description = f.read()
 
 setuptools.setup(
     name="MusicBGX",
-    version="1.0.0",
+    version="1.0.5",
     author="Amin Rngbr",
     author_email="rngbramin@gmail.com",
     description="A light and simple library for playing offline and online music in the background (:",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/aminrngbr1122",
     keywords="music",
```

