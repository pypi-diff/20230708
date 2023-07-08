# Comparing `tmp/nicovideo.py-0.0.6.tar.gz` & `tmp/nicovideo.py-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nicovideo.py-0.0.6.tar", last modified: Sat Jul  1 07:59:56 2023, max compression
+gzip compressed data, was "nicovideo.py-0.0.7.tar", last modified: Sat Jul  8 05:38:16 2023, max compression
```

## Comparing `nicovideo.py-0.0.6.tar` & `nicovideo.py-0.0.7.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 okaits    (1000) okaits    (1000)        0 2023-07-01 07:59:56.269100 nicovideo.py-0.0.6/
--rw-rw-r--   0 okaits    (1000) okaits    (1000)     7559 2023-06-24 05:49:10.000000 nicovideo.py-0.0.6/LICENSE.md
--rw-rw-r--   0 okaits    (1000) okaits    (1000)     6180 2023-07-01 07:59:56.269100 nicovideo.py-0.0.6/PKG-INFO
--rw-rw-r--   0 okaits    (1000) okaits    (1000)     5425 2023-07-01 07:58:26.000000 nicovideo.py-0.0.6/README.md
-drwxrwxr-x   0 okaits    (1000) okaits    (1000)        0 2023-07-01 07:59:56.269100 nicovideo.py-0.0.6/nicovideo/
--rw-rw-r--   0 okaits    (1000) okaits    (1000)    12016 2023-07-01 07:59:03.000000 nicovideo.py-0.0.6/nicovideo/__init__.py
-drwxrwxr-x   0 okaits    (1000) okaits    (1000)        0 2023-07-01 07:59:56.269100 nicovideo.py-0.0.6/nicovideo.py.egg-info/
--rw-rw-r--   0 okaits    (1000) okaits    (1000)     6180 2023-07-01 07:59:55.000000 nicovideo.py-0.0.6/nicovideo.py.egg-info/PKG-INFO
--rw-rw-r--   0 okaits    (1000) okaits    (1000)      195 2023-07-01 07:59:56.000000 nicovideo.py-0.0.6/nicovideo.py.egg-info/SOURCES.txt
--rw-rw-r--   0 okaits    (1000) okaits    (1000)        1 2023-07-01 07:59:55.000000 nicovideo.py-0.0.6/nicovideo.py.egg-info/dependency_links.txt
--rw-rw-r--   0 okaits    (1000) okaits    (1000)       10 2023-07-01 07:59:56.000000 nicovideo.py-0.0.6/nicovideo.py.egg-info/top_level.txt
--rw-rw-r--   0 okaits    (1000) okaits    (1000)       38 2023-07-01 07:59:56.269100 nicovideo.py-0.0.6/setup.cfg
--rw-rw-r--   0 okaits    (1000) okaits    (1000)      993 2023-07-01 07:59:09.000000 nicovideo.py-0.0.6/setup.py
+drwxrwxr-x   0 okaits    (1000) okaits    (1000)        0 2023-07-08 05:38:16.962105 nicovideo.py-0.0.7/
+-rw-rw-r--   0 okaits    (1000) okaits    (1000)     7559 2023-06-24 05:49:10.000000 nicovideo.py-0.0.7/LICENSE.md
+-rw-rw-r--   0 okaits    (1000) okaits    (1000)     6180 2023-07-08 05:38:16.962105 nicovideo.py-0.0.7/PKG-INFO
+-rw-rw-r--   0 okaits    (1000) okaits    (1000)     5425 2023-07-01 07:58:26.000000 nicovideo.py-0.0.7/README.md
+drwxrwxr-x   0 okaits    (1000) okaits    (1000)        0 2023-07-08 05:38:16.962105 nicovideo.py-0.0.7/nicovideo/
+-rw-rw-r--   0 okaits    (1000) okaits    (1000)    12320 2023-07-08 05:37:23.000000 nicovideo.py-0.0.7/nicovideo/__init__.py
+drwxrwxr-x   0 okaits    (1000) okaits    (1000)        0 2023-07-08 05:38:16.962105 nicovideo.py-0.0.7/nicovideo.py.egg-info/
+-rw-rw-r--   0 okaits    (1000) okaits    (1000)     6180 2023-07-08 05:38:16.000000 nicovideo.py-0.0.7/nicovideo.py.egg-info/PKG-INFO
+-rw-rw-r--   0 okaits    (1000) okaits    (1000)      195 2023-07-08 05:38:16.000000 nicovideo.py-0.0.7/nicovideo.py.egg-info/SOURCES.txt
+-rw-rw-r--   0 okaits    (1000) okaits    (1000)        1 2023-07-08 05:38:16.000000 nicovideo.py-0.0.7/nicovideo.py.egg-info/dependency_links.txt
+-rw-rw-r--   0 okaits    (1000) okaits    (1000)       10 2023-07-08 05:38:16.000000 nicovideo.py-0.0.7/nicovideo.py.egg-info/top_level.txt
+-rw-rw-r--   0 okaits    (1000) okaits    (1000)       38 2023-07-08 05:38:16.962105 nicovideo.py-0.0.7/setup.cfg
+-rw-rw-r--   0 okaits    (1000) okaits    (1000)      993 2023-07-08 05:37:27.000000 nicovideo.py-0.0.7/setup.py
```

### Comparing `nicovideo.py-0.0.6/LICENSE.md` & `nicovideo.py-0.0.7/LICENSE.md`

 * *Files identical despite different names*

### Comparing `nicovideo.py-0.0.6/PKG-INFO` & `nicovideo.py-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nicovideo.py
-Version: 0.0.6
+Version: 0.0.7
 Summary: Get nicovideo's video metadata.
 Home-page: https://github.com/okaits/nicovideo.py
 Author: okaits#7534
 Author-email: okaits@okaits7534.mydns.jp
 License: GNU Lesser General Public License 3.0
 Keywords: nicovideo
 Platform: UNKNOWN
```

### Comparing `nicovideo.py-0.0.6/README.md` & `nicovideo.py-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `nicovideo.py-0.0.6/nicovideo/__init__.py` & `nicovideo.py-0.0.7/nicovideo/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,37 @@
 """ nicovideo.py (video) """
 from __future__ import annotations
 
 import datetime
 import pprint
-import urllib.request
 import urllib.error
+import urllib.request
+from functools import cache
 from html import unescape
 from typing import Type, Union
 
 import json5
 from bs4 import BeautifulSoup as bs
 
-__version__ = '0.0.6'
+__version__ = '0.0.7'
 
 class Error():
     """ Errors """
     class NicovideoClientError(Exception):
         """ urllib error """
         class VideoNotFound(Exception):
             """ Video not found or deleted """
         class ConnectionError(Exception):
             """ Connection error """
 
+@cache
+def _urllib_request_with_cache(url: str) -> str:
+    with urllib.request.urlopen(url) as response:
+        return response.read()
+
 class Video():
     """ Video """
     def __init__(self, videoid: str) -> Video:
         self.videoid: str  = videoid
         self.rawdict: dict = {}
 
     class Metadata():
@@ -165,20 +171,23 @@
             self.tags       : list[self.Tag]                = tags
             self.ranking    : self.Ranking                  = ranking
             self.series     : self.Series                   = series
             self.thumbnail  : self.Thumbnail                = thumbnail
             self.url        : str                           = \
                 f'https://www.nicovideo.jp/watch/{videoid}'
 
-    def get_metadata(self) -> Video.Metadata:
+    def get_metadata(self, use_cache: bool = False) -> Video.Metadata:
         """ Get video's metadata """
         watch_url = f"https://www.nicovideo.jp/watch/{self.videoid}"
         try:
-            with urllib.request.urlopen(watch_url) as response:
-                text = response.read()
+            if use_cache:
+                text = _urllib_request_with_cache(watch_url)
+            else:
+                with urllib.request.urlopen(watch_url) as response:
+                    text = response.read()
         except urllib.error.HTTPError as exc:
             if exc.code == 404:
                 raise Error.NicovideoClientError.VideoNotFound("Video not found or deleted.")\
                     from exc
             else:
                 raise Error.NicovideoClientError.ConnectionError(
                     f"Unexpected HTTP Error: {exc.code}"
```

### Comparing `nicovideo.py-0.0.6/nicovideo.py.egg-info/PKG-INFO` & `nicovideo.py-0.0.7/nicovideo.py.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nicovideo.py
-Version: 0.0.6
+Version: 0.0.7
 Summary: Get nicovideo's video metadata.
 Home-page: https://github.com/okaits/nicovideo.py
 Author: okaits#7534
 Author-email: okaits@okaits7534.mydns.jp
 License: GNU Lesser General Public License 3.0
 Keywords: nicovideo
 Platform: UNKNOWN
```

### Comparing `nicovideo.py-0.0.6/setup.py` & `nicovideo.py-0.0.7/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 from setuptools import find_packages, setup
 
 readme = (Path(__file__).parent / "README.md").read_text()
 
 setup(
     name='nicovideo.py',
-    version='0.0.6',
+    version='0.0.7',
     description='Get nicovideo\'s video metadata.',
     long_description=readme,
     long_description_content_type='text/markdown',
     author='okaits#7534',
     author_email='okaits@okaits7534.mydns.jp',
     url='https://github.com/okaits/nicovideo.py',
     classifiers=[
```

