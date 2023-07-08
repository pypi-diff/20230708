# Comparing `tmp/MusicBGX-1.0.5.tar.gz` & `tmp/MusicBGX-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MusicBGX-1.0.5.tar", last modified: Sat Jul  8 13:32:01 2023, max compression
+gzip compressed data, was "MusicBGX-1.0.7.tar", last modified: Sat Jul  8 15:13:16 2023, max compression
```

## Comparing `MusicBGX-1.0.5.tar` & `MusicBGX-1.0.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-07-08 13:32:01.275042 MusicBGX-1.0.5/
--rw-rw-rw-   0        0        0     1067 2023-07-08 08:12:01.000000 MusicBGX-1.0.5/LICENSE
-drwxrwxrwx   0        0        0        0 2023-07-08 13:32:00.969973 MusicBGX-1.0.5/MusicBGX/
--rw-rw-rw-   0        0        0      520 2023-07-08 13:09:04.000000 MusicBGX-1.0.5/MusicBGX/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-08 13:32:01.242040 MusicBGX-1.0.5/MusicBGX.egg-info/
--rw-rw-rw-   0        0        0      622 2023-07-08 13:32:00.000000 MusicBGX-1.0.5/MusicBGX.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      216 2023-07-08 13:32:00.000000 MusicBGX-1.0.5/MusicBGX.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-08 13:32:00.000000 MusicBGX-1.0.5/MusicBGX.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-07-08 13:32:00.000000 MusicBGX-1.0.5/MusicBGX.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-07-08 13:32:00.000000 MusicBGX-1.0.5/MusicBGX.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      622 2023-07-08 13:32:01.290069 MusicBGX-1.0.5/PKG-INFO
--rw-rw-rw-   0        0        0      242 2023-07-08 13:10:30.000000 MusicBGX-1.0.5/README.md
--rw-rw-rw-   0        0        0       81 2023-07-08 13:32:01.298059 MusicBGX-1.0.5/setup.cfg
--rw-rw-rw-   0        0        0      694 2023-07-08 13:16:12.000000 MusicBGX-1.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-08 15:13:16.265085 MusicBGX-1.0.7/
+-rw-rw-rw-   0        0        0     1067 2023-07-08 08:12:01.000000 MusicBGX-1.0.7/LICENSE
+drwxrwxrwx   0        0        0        0 2023-07-08 15:13:16.119057 MusicBGX-1.0.7/MusicBGX/
+-rw-rw-rw-   0        0        0      862 2023-07-08 15:11:30.000000 MusicBGX-1.0.7/MusicBGX/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-08 15:13:16.253082 MusicBGX-1.0.7/MusicBGX.egg-info/
+-rw-rw-rw-   0        0        0      647 2023-07-08 15:13:15.000000 MusicBGX-1.0.7/MusicBGX.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      216 2023-07-08 15:13:15.000000 MusicBGX-1.0.7/MusicBGX.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-08 15:13:15.000000 MusicBGX-1.0.7/MusicBGX.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-07-08 15:13:15.000000 MusicBGX-1.0.7/MusicBGX.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-08 15:13:15.000000 MusicBGX-1.0.7/MusicBGX.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      647 2023-07-08 15:13:16.266085 MusicBGX-1.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0      267 2023-07-08 15:12:13.000000 MusicBGX-1.0.7/README.md
+-rw-rw-rw-   0        0        0       81 2023-07-08 15:13:16.276107 MusicBGX-1.0.7/setup.cfg
+-rw-rw-rw-   0        0        0      694 2023-07-08 15:11:45.000000 MusicBGX-1.0.7/setup.py
```

### Comparing `MusicBGX-1.0.5/LICENSE` & `MusicBGX-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `MusicBGX-1.0.5/MusicBGX.egg-info/PKG-INFO` & `MusicBGX-1.0.7/MusicBGX.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MusicBGX
-Version: 1.0.5
+Version: 1.0.7
 Summary: A light and simple library for playing offline and online music in the background (:
 Home-page: https://github.com/aminrngbr1122
 Author: Amin Rngbr
 Author-email: rngbramin@gmail.com
 Keywords: music
 Requires-Python: >=3.4
 Description-Content-Type: text/markdown
@@ -16,15 +16,15 @@
 pip install MusicBGX
 ```
 
 ## Useage
 
 ```python
 from MusicBGX import *
-app = BackGround(path)
+app = BackGround(paths=['ads1.mp3', 'ads2.mp3])
 app.play_background_music()
 ```
 
 ## Project status
 
 - Alpha
```

### Comparing `MusicBGX-1.0.5/PKG-INFO` & `MusicBGX-1.0.7/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MusicBGX
-Version: 1.0.5
+Version: 1.0.7
 Summary: A light and simple library for playing offline and online music in the background (:
 Home-page: https://github.com/aminrngbr1122
 Author: Amin Rngbr
 Author-email: rngbramin@gmail.com
 Keywords: music
 Requires-Python: >=3.4
 Description-Content-Type: text/markdown
@@ -16,15 +16,15 @@
 pip install MusicBGX
 ```
 
 ## Useage
 
 ```python
 from MusicBGX import *
-app = BackGround(path)
+app = BackGround(paths=['ads1.mp3', 'ads2.mp3])
 app.play_background_music()
 ```
 
 ## Project status
 
 - Alpha
```

### Comparing `MusicBGX-1.0.5/setup.py` & `MusicBGX-1.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open('README.md', "r") as f:
     long_description = f.read()
 
 setuptools.setup(
     name="MusicBGX",
-    version="1.0.5",
+    version="1.0.7",
     author="Amin Rngbr",
     author_email="rngbramin@gmail.com",
     description="A light and simple library for playing offline and online music in the background (:",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/aminrngbr1122",
     keywords="music",
```

