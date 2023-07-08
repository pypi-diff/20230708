# Comparing `tmp/y2mate-api-0.0.9.tar.gz` & `tmp/y2mate-api-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "y2mate-api-0.0.9.tar", last modified: Sat Jul  1 20:45:50 2023, max compression
+gzip compressed data, was "y2mate-api-1.0.0.tar", last modified: Sat Jul  8 20:39:10 2023, max compression
```

## Comparing `y2mate-api-0.0.9.tar` & `y2mate-api-1.0.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-07-01 20:45:50.389384 y2mate-api-0.0.9/
--rw-rw----   0 root         (0) everybody  (9997)     1064 2023-06-16 15:42:28.000000 y2mate-api-0.0.9/LICENSE
--rw-rw----   0 root         (0) everybody  (9997)    11314 2023-07-01 20:45:50.373384 y2mate-api-0.0.9/PKG-INFO
--rw-rw----   0 root         (0) everybody  (9997)    10219 2023-07-01 20:44:36.000000 y2mate-api-0.0.9/README.md
--rw-rw----   0 root         (0) everybody  (9997)       38 2023-07-01 20:45:50.389384 y2mate-api-0.0.9/setup.cfg
--rw-rw----   0 root         (0) everybody  (9997)     1587 2023-06-30 18:02:19.000000 y2mate-api-0.0.9/setup.py
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-07-01 20:45:49.865383 y2mate-api-0.0.9/tests/
--rw-rw----   0 root         (0) everybody  (9997)     1567 2023-06-21 13:35:40.000000 y2mate-api-0.0.9/tests/test_download.py
--rw-rw----   0 root         (0) everybody  (9997)     5577 2023-06-20 21:29:31.000000 y2mate-api-0.0.9/tests/test_queries.py
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-07-01 20:45:50.037384 y2mate-api-0.0.9/y2mate_api/
--rw-rw----   0 root         (0) everybody  (9997)      490 2023-06-30 18:01:50.000000 y2mate-api-0.0.9/y2mate_api/__init__.py
--rw-rw----   0 root         (0) everybody  (9997)       34 2023-06-19 18:39:03.000000 y2mate-api-0.0.9/y2mate_api/__main__.py
--rw-rw----   0 root         (0) everybody  (9997)     5860 2023-07-01 20:41:24.000000 y2mate-api-0.0.9/y2mate_api/console.py
--rw-rw----   0 root         (0) everybody  (9997)    15396 2023-07-01 20:39:21.000000 y2mate-api-0.0.9/y2mate_api/downloader.py
--rw-rw----   0 root         (0) everybody  (9997)    14731 2023-06-22 17:22:06.000000 y2mate-api-0.0.9/y2mate_api/main.py
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-07-01 20:45:50.345384 y2mate-api-0.0.9/y2mate_api.egg-info/
--rw-rw----   0 root         (0) everybody  (9997)    11314 2023-07-01 20:45:48.000000 y2mate-api-0.0.9/y2mate_api.egg-info/PKG-INFO
--rw-rw----   0 root         (0) everybody  (9997)      389 2023-07-01 20:45:49.000000 y2mate-api-0.0.9/y2mate_api.egg-info/SOURCES.txt
--rw-rw----   0 root         (0) everybody  (9997)        1 2023-07-01 20:45:48.000000 y2mate-api-0.0.9/y2mate_api.egg-info/dependency_links.txt
--rw-rw----   0 root         (0) everybody  (9997)       51 2023-07-01 20:45:48.000000 y2mate-api-0.0.9/y2mate_api.egg-info/entry_points.txt
--rw-rw----   0 root         (0) everybody  (9997)       99 2023-07-01 20:45:48.000000 y2mate-api-0.0.9/y2mate_api.egg-info/requires.txt
--rw-rw----   0 root         (0) everybody  (9997)       11 2023-07-01 20:45:48.000000 y2mate-api-0.0.9/y2mate_api.egg-info/top_level.txt
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-07-08 20:39:10.367456 y2mate-api-1.0.0/
+-rw-rw----   0 root         (0) everybody  (9997)     1064 2023-06-16 15:42:28.000000 y2mate-api-1.0.0/LICENSE
+-rw-rw----   0 root         (0) everybody  (9997)    11314 2023-07-08 20:39:10.331456 y2mate-api-1.0.0/PKG-INFO
+-rw-rw----   0 root         (0) everybody  (9997)    10219 2023-07-08 20:18:33.000000 y2mate-api-1.0.0/README.md
+-rw-rw----   0 root         (0) everybody  (9997)       38 2023-07-08 20:39:10.371456 y2mate-api-1.0.0/setup.cfg
+-rw-rw----   0 root         (0) everybody  (9997)     1615 2023-07-07 14:09:10.000000 y2mate-api-1.0.0/setup.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-07-08 20:39:09.811456 y2mate-api-1.0.0/tests/
+-rw-rw----   0 root         (0) everybody  (9997)     1567 2023-06-21 13:35:40.000000 y2mate-api-1.0.0/tests/test_download.py
+-rw-rw----   0 root         (0) everybody  (9997)     5577 2023-06-20 21:29:31.000000 y2mate-api-1.0.0/tests/test_queries.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-07-08 20:39:09.987456 y2mate-api-1.0.0/y2mate_api/
+-rw-rw----   0 root         (0) everybody  (9997)      490 2023-07-07 12:50:07.000000 y2mate-api-1.0.0/y2mate_api/__init__.py
+-rw-rw----   0 root         (0) everybody  (9997)       34 2023-06-19 18:39:03.000000 y2mate-api-1.0.0/y2mate_api/__main__.py
+-rw-rw----   0 root         (0) everybody  (9997)     5860 2023-07-01 20:41:24.000000 y2mate-api-1.0.0/y2mate_api/console.py
+-rw-rw----   0 root         (0) everybody  (9997)    15945 2023-07-08 20:35:56.000000 y2mate-api-1.0.0/y2mate_api/downloader.py
+-rw-rw----   0 root         (0) everybody  (9997)    14819 2023-07-08 20:29:53.000000 y2mate-api-1.0.0/y2mate_api/main.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-07-08 20:39:10.315456 y2mate-api-1.0.0/y2mate_api.egg-info/
+-rw-rw----   0 root         (0) everybody  (9997)    11314 2023-07-08 20:39:08.000000 y2mate-api-1.0.0/y2mate_api.egg-info/PKG-INFO
+-rw-rw----   0 root         (0) everybody  (9997)      389 2023-07-08 20:39:09.000000 y2mate-api-1.0.0/y2mate_api.egg-info/SOURCES.txt
+-rw-rw----   0 root         (0) everybody  (9997)        1 2023-07-08 20:39:08.000000 y2mate-api-1.0.0/y2mate_api.egg-info/dependency_links.txt
+-rw-rw----   0 root         (0) everybody  (9997)       51 2023-07-08 20:39:08.000000 y2mate-api-1.0.0/y2mate_api.egg-info/entry_points.txt
+-rw-rw----   0 root         (0) everybody  (9997)       99 2023-07-08 20:39:08.000000 y2mate-api-1.0.0/y2mate_api.egg-info/requires.txt
+-rw-rw----   0 root         (0) everybody  (9997)       11 2023-07-08 20:39:08.000000 y2mate-api-1.0.0/y2mate_api.egg-info/top_level.txt
```

### Comparing `y2mate-api-0.0.9/LICENSE` & `y2mate-api-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `y2mate-api-0.0.9/PKG-INFO` & `y2mate-api-1.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: y2mate-api
-Version: 0.0.9
+Version: 1.0.0
 Summary: Download youtube videos and audios by title or link
 Home-page: https://github.com/Simatwa/y2mate-api
 Author: Smartwa
 Author-email: smartwacaleb@gmail.com
 Maintainer: Smartwa
 License: MIT
 Project-URL: Bug Report, https://github.com/Simatwa/y2mate-api/issues/new
@@ -27,15 +27,15 @@
 License-File: LICENSE
 
 <h1 align="center">y2mate-api</h1>
 
 <p align="center">
 <a href="https://github.com/Simatwa/y2mate-api/actions/workflows/python-test.yml"><img src="https://github.com/Simatwa/y2mate-api/actions/workflows/python-test.yml/badge.svg" alt="Python Test"/></a>
 <a href="LICENSE"><img alt="License" src="https://img.shields.io/static/v1?logo=GPL&color=Blue&message=MIT&label=License"/></a>
-<a href="https://pypi.org/project/y2mate-api"><img alt="PyPi" src="https://img.shields.io/static/v1?logo=pypi&label=Pypi&message=v0.0.9&color=green"/></a>
+<a href="https://pypi.org/project/y2mate-api"><img alt="PyPi" src="https://img.shields.io/static/v1?logo=pypi&label=Pypi&message=v1.0.0&color=green"/></a>
 <a href="https://github.com/psf/black"><img alt="Black" src="https://img.shields.io/static/v1?logo=Black&label=Code-style&message=Black"/></a>
 <a href="#"><img alt="Passing" src="https://img.shields.io/static/v1?logo=Docs&label=Docs&message=Passing&color=green"/></a>
 <a href="#"><img alt="coverage" src="https://img.shields.io/static/v1?logo=Coverage&label=Coverage&message=90%&color=yellowgreen"/></a>
 <a href="#" alt="progress"><img alt="Progress" src="https://img.shields.io/static/v1?logo=Progress&label=Progress&message=95%&color=green"/></a>
 <a href="https://pepy.tech/project/livescore-api"><img src="https://static.pepy.tech/personalized-badge/y2mate-api?period=total&units=international_system&left_color=grey&right_color=orange&left_text=Downloads" alt="Downloads"></a>
 </p>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: y2mate-api Version: 0.0.9 Summary: Download youtube
+Metadata-Version: 2.1 Name: y2mate-api Version: 1.0.0 Summary: Download youtube
 videos and audios by title or link Home-page: https://github.com/Simatwa/
 y2mate-api Author: Smartwa Author-email: smartwacaleb@gmail.com Maintainer:
 Smartwa License: MIT Project-URL: Bug Report, https://github.com/Simatwa/
 y2mate-api/issues/new Keywords: y2mate,videos,video-api,youtube Classifier:
 License :: OSI Approved :: MIT License Classifier: Development Status :: 4 -
 Beta Classifier: Intended Audience :: Developers Classifier: Natural Language
 :: English Classifier: License :: Free For Home Use Classifier: Intended
```

### Comparing `y2mate-api-0.0.9/README.md` & `y2mate-api-1.0.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 <h1 align="center">y2mate-api</h1>
 
 <p align="center">
 <a href="https://github.com/Simatwa/y2mate-api/actions/workflows/python-test.yml"><img src="https://github.com/Simatwa/y2mate-api/actions/workflows/python-test.yml/badge.svg" alt="Python Test"/></a>
 <a href="LICENSE"><img alt="License" src="https://img.shields.io/static/v1?logo=GPL&color=Blue&message=MIT&label=License"/></a>
-<a href="https://pypi.org/project/y2mate-api"><img alt="PyPi" src="https://img.shields.io/static/v1?logo=pypi&label=Pypi&message=v0.0.9&color=green"/></a>
+<a href="https://pypi.org/project/y2mate-api"><img alt="PyPi" src="https://img.shields.io/static/v1?logo=pypi&label=Pypi&message=v1.0.0&color=green"/></a>
 <a href="https://github.com/psf/black"><img alt="Black" src="https://img.shields.io/static/v1?logo=Black&label=Code-style&message=Black"/></a>
 <a href="#"><img alt="Passing" src="https://img.shields.io/static/v1?logo=Docs&label=Docs&message=Passing&color=green"/></a>
 <a href="#"><img alt="coverage" src="https://img.shields.io/static/v1?logo=Coverage&label=Coverage&message=90%&color=yellowgreen"/></a>
 <a href="#" alt="progress"><img alt="Progress" src="https://img.shields.io/static/v1?logo=Progress&label=Progress&message=95%&color=green"/></a>
 <a href="https://pepy.tech/project/livescore-api"><img src="https://static.pepy.tech/personalized-badge/y2mate-api?period=total&units=international_system&left_color=grey&right_color=orange&left_text=Downloads" alt="Downloads"></a>
 </p>
```

### Comparing `y2mate-api-0.0.9/setup.py` & `y2mate-api-1.0.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup
 
-version = "0.0.9"
+version = "1.0.0"
 info = "Download youtube videos and audios by title or link"
 author = "Smartwa"
 repo = "https://github.com/Simatwa/y2mate-api"
 
 setup(
     name="y2mate-api",
     packages=["y2mate_api"],
@@ -13,21 +13,21 @@
     author=author,
     maintainer=author,
     author_email="smartwacaleb@gmail.com",
     description=info,
     url=repo,
     project_urls={"Bug Report": f"{repo}/issues/new"},
     install_requires=[
-    "argparse>=1.1",
-    "tqdm==4.65.0",
-    "requests==2.28.2",
-    "colorama==0.4.6",
-    "appdirs==1.4.4",
-    "getch==1.0",
-    "click==8.1.3",
+        "argparse>=1.1",
+        "tqdm==4.65.0",
+        "requests==2.28.2",
+        "colorama==0.4.6",
+        "appdirs==1.4.4",
+        "getch==1.0",
+        "click==8.1.3",
     ],
     python_requires=">=3.8",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     classifiers=[
         "License :: OSI Approved :: MIT License",
         "Development Status :: 4 - Beta",
```

### Comparing `y2mate-api-0.0.9/tests/test_download.py` & `y2mate-api-1.0.0/tests/test_download.py`

 * *Files identical despite different names*

### Comparing `y2mate-api-0.0.9/tests/test_queries.py` & `y2mate-api-1.0.0/tests/test_queries.py`

 * *Files identical despite different names*

### Comparing `y2mate-api-0.0.9/y2mate_api/console.py` & `y2mate-api-1.0.0/y2mate_api/console.py`

 * *Files identical despite different names*

### Comparing `y2mate-api-0.0.9/y2mate_api/downloader.py` & `y2mate-api-1.0.0/y2mate_api/downloader.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,25 @@
-from .main import requests, logging, utils, first_query, second_query, third_query
+from .main import (
+    requests,
+    logging,
+    utils,
+    first_query,
+    second_query,
+    third_query,
+    session,
+    headers,
+)
 from tqdm import tqdm
 from colorama import Fore
 from os import path, getcwd
 from threading import Thread
 from getch import getch
 from sys import stdout
 from click import launch as launch_media
+import warnings
 
 """
 - query string
 - format mp4/3
 - quality 720p/128kbps
 - keywords
 - Specify video author
@@ -57,18 +67,18 @@
         self.dropped = []
         self.total = 1
         self.saved_videos = utils.get_history()
 
     def __str__(self):
         return self.query
 
-    def __enter__(self):
-        pass
+    def __enter__(self, *args, **kwargs):
+        return self
 
-    def __exit__(self):
+    def __exit__(self, *args, **kwargs):
         self.vitems.clear()
         self.total = 1
 
     def __call__(self, *args, **kwargs):
         return self.run(*args, **kwargs)
 
     def __filter_videos(self, entries: list) -> list:
@@ -362,27 +372,36 @@
         """
         if third_dict:
             assert third_dict.get(
                 "dlink"
             ), "The video selected does not support that quality, try lower qualities."
             if third_dict.get("mess"):
                 logging.warning(third_dict.get("mess"))
-            resp = requests.get(third_dict["dlink"], stream=True)
-            size_in_bytes = int(resp.headers.get("content-length", 1000000000000))
+            resp = requests.get(third_dict["dlink"], stream=True, headers=headers)
+            default_content_length = 1000000000
+            size_in_bytes = int(
+                resp.headers.get("content-length", default_content_length)
+            )
+            if size_in_bytes == default_content_length:
+                warnings.warn(
+                    f"Seems the media doesn't support that quality try {'.m4a quality' if 'mp3' in third_dict.get('f','str').lower() else 'other qualities'} or resolvers if this warning persist!"
+                )
             size_in_mb = round(size_in_bytes / 1000000, 2)
             chunk_size_in_bytes = chunk_size * 1024
             filename = self.generate_filename(third_dict, naming_format)
             save_to = path.join(dir, filename)
 
             third_dict["saved_to"] = (
                 save_to
                 if any([save_to.startswith("/"), ":" in save_to])
                 else path.join(getcwd(), dir, filename)
             )
-            try_play_media = lambda: launch_media(third_dict["saved_to"]) if play else None
+            try_play_media = (
+                lambda: launch_media(third_dict["saved_to"]) if play else None
+            )
             if progress_bar:
                 if not quiet:
                     print(f"{filename}")
                 with tqdm(
                     total=size_in_bytes,
                     bar_format="%s%d MB %s{bar} %s{l_bar}%s"
                     % (Fore.GREEN, size_in_mb, Fore.CYAN, Fore.YELLOW, Fore.RESET),
```

### Comparing `y2mate-api-0.0.9/y2mate_api/main.py` & `y2mate-api-1.0.0/y2mate_api/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 session = requests.session()
 
 headers = {
     "Accept": "text/html,application/xhtml+xml,application/xml;q=0.9,image/avif,image/webp,image/apng,*/*;q=0.8,application/signed-exchange;v=b3;q=0.7",
     "User-Agent": "Mozilla/5.0 (Linux; Android 10; K) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/112.0.0.0 Mobile Safari/537.36",
     "Accept-Encoding": "gzip, deflate, br",
     "Accept-Language": "en-US,en;q=0.9",
+    "referer": "https://y2mate.com",
 }
 
 session.headers.update(headers)
 
 get_excep = lambda e: e.args[1] if len(e.args) > 1 else e
 
 appdir = AppDirs(__prog__)
@@ -273,15 +274,15 @@
 
     def __main__(self, *args, **kwargs):
         return self.main(*args, **kwargs)
 
     def __enter__(self, *args, **kwargs):
         return self.__main__(*args, **kwargs)
 
-    def __exit__(self):
+    def __exit__(self, *args, **kwargs):
         self.processed = False
 
     def main(self, item_no: int = 0, timeout: int = 30):
         r"""Requests for video formats and related videos
         :param item_no: (Optional) Index of query_one.vitems
         :type item_no: int
         :param timeout:  (Optional)Http request timeout
@@ -333,18 +334,18 @@
             + self.qualities_plus,
             self.formats[1]: ["mp3", "m4a", ".m4a", "128kbps", "192kbps", "328kbps"],
         }
 
     def __call__(self, *args, **kwargs):
         return self.main(*args, **kwargs)
 
-    def __enter__(self):
+    def __enter__(self, *args, **kwargs):
         return self
 
-    def __exit__(self):
+    def __exit__(self, *args, **kwargs):
         pass
 
     def __str__(self):
         return """
 {
     "status": "ok",
     "mess": "",
```

### Comparing `y2mate-api-0.0.9/y2mate_api.egg-info/PKG-INFO` & `y2mate-api-1.0.0/y2mate_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: y2mate-api
-Version: 0.0.9
+Version: 1.0.0
 Summary: Download youtube videos and audios by title or link
 Home-page: https://github.com/Simatwa/y2mate-api
 Author: Smartwa
 Author-email: smartwacaleb@gmail.com
 Maintainer: Smartwa
 License: MIT
 Project-URL: Bug Report, https://github.com/Simatwa/y2mate-api/issues/new
@@ -27,15 +27,15 @@
 License-File: LICENSE
 
 <h1 align="center">y2mate-api</h1>
 
 <p align="center">
 <a href="https://github.com/Simatwa/y2mate-api/actions/workflows/python-test.yml"><img src="https://github.com/Simatwa/y2mate-api/actions/workflows/python-test.yml/badge.svg" alt="Python Test"/></a>
 <a href="LICENSE"><img alt="License" src="https://img.shields.io/static/v1?logo=GPL&color=Blue&message=MIT&label=License"/></a>
-<a href="https://pypi.org/project/y2mate-api"><img alt="PyPi" src="https://img.shields.io/static/v1?logo=pypi&label=Pypi&message=v0.0.9&color=green"/></a>
+<a href="https://pypi.org/project/y2mate-api"><img alt="PyPi" src="https://img.shields.io/static/v1?logo=pypi&label=Pypi&message=v1.0.0&color=green"/></a>
 <a href="https://github.com/psf/black"><img alt="Black" src="https://img.shields.io/static/v1?logo=Black&label=Code-style&message=Black"/></a>
 <a href="#"><img alt="Passing" src="https://img.shields.io/static/v1?logo=Docs&label=Docs&message=Passing&color=green"/></a>
 <a href="#"><img alt="coverage" src="https://img.shields.io/static/v1?logo=Coverage&label=Coverage&message=90%&color=yellowgreen"/></a>
 <a href="#" alt="progress"><img alt="Progress" src="https://img.shields.io/static/v1?logo=Progress&label=Progress&message=95%&color=green"/></a>
 <a href="https://pepy.tech/project/livescore-api"><img src="https://static.pepy.tech/personalized-badge/y2mate-api?period=total&units=international_system&left_color=grey&right_color=orange&left_text=Downloads" alt="Downloads"></a>
 </p>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: y2mate-api Version: 0.0.9 Summary: Download youtube
+Metadata-Version: 2.1 Name: y2mate-api Version: 1.0.0 Summary: Download youtube
 videos and audios by title or link Home-page: https://github.com/Simatwa/
 y2mate-api Author: Smartwa Author-email: smartwacaleb@gmail.com Maintainer:
 Smartwa License: MIT Project-URL: Bug Report, https://github.com/Simatwa/
 y2mate-api/issues/new Keywords: y2mate,videos,video-api,youtube Classifier:
 License :: OSI Approved :: MIT License Classifier: Development Status :: 4 -
 Beta Classifier: Intended Audience :: Developers Classifier: Natural Language
 :: English Classifier: License :: Free For Home Use Classifier: Intended
```

