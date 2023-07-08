# Comparing `tmp/pypdl-0.0.9.tar.gz` & `tmp/pypdl-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypdl-0.0.9.tar", last modified: Thu Jun 29 07:51:16 2023, max compression
+gzip compressed data, was "pypdl-1.0.2.tar", last modified: Sat Jul  8 08:19:10 2023, max compression
```

## Comparing `pypdl-0.0.9.tar` & `pypdl-1.0.2.tar`

### file list

```diff
@@ -1,18 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-06-29 07:51:16.225355 pypdl-0.0.9/
--rw-rw-rw-   0        0        0     1086 2023-03-20 10:21:57.000000 pypdl-0.0.9/LICENSE
--rw-rw-rw-   0        0        0     9384 2023-06-29 07:51:16.224249 pypdl-0.0.9/PKG-INFO
--rw-rw-rw-   0        0        0     8795 2023-06-29 04:38:39.000000 pypdl-0.0.9/README.md
-drwxrwxrwx   0        0        0        0 2023-06-29 07:51:16.205378 pypdl-0.0.9/pypdl/
--rw-rw-rw-   0        0        0       30 2023-03-21 10:24:52.000000 pypdl-0.0.9/pypdl/__init__.py
--rw-rw-rw-   0        0        0    13931 2023-06-29 07:40:46.000000 pypdl-0.0.9/pypdl/main.py
--rw-rw-rw-   0        0        0     1226 2023-06-29 07:39:20.000000 pypdl-0.0.9/pypdl/test.py
--rw-rw-rw-   0        0        0    12153 2023-06-28 14:37:57.000000 pypdl-0.0.9/pypdl/test1.py
--rw-rw-rw-   0        0        0     6110 2023-06-29 07:32:49.000000 pypdl-0.0.9/pypdl/utls.py
-drwxrwxrwx   0        0        0        0 2023-06-29 07:51:16.223236 pypdl-0.0.9/pypdl.egg-info/
--rw-rw-rw-   0        0        0     9384 2023-06-29 07:51:16.000000 pypdl-0.0.9/pypdl.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      245 2023-06-29 07:51:16.000000 pypdl-0.0.9/pypdl.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-29 07:51:16.000000 pypdl-0.0.9/pypdl.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-06-29 07:51:16.000000 pypdl-0.0.9/pypdl.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-06-29 07:51:16.000000 pypdl-0.0.9/pypdl.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-29 07:51:16.225355 pypdl-0.0.9/setup.cfg
--rw-rw-rw-   0        0        0      927 2023-06-29 07:51:06.000000 pypdl-0.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-08 08:19:10.051984 pypdl-1.0.2/
+-rw-rw-rw-   0        0        0     1086 2023-03-20 10:21:57.000000 pypdl-1.0.2/LICENSE
+-rw-rw-rw-   0        0        0     9384 2023-07-08 08:19:10.050925 pypdl-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     8795 2023-06-29 04:38:39.000000 pypdl-1.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-08 08:19:10.029965 pypdl-1.0.2/pypdl/
+-rw-rw-rw-   0        0        0       30 2023-03-21 10:24:52.000000 pypdl-1.0.2/pypdl/__init__.py
+-rw-rw-rw-   0        0        0    14287 2023-07-08 08:14:48.000000 pypdl-1.0.2/pypdl/main.py
+-rw-rw-rw-   0        0        0     1228 2023-07-08 08:11:19.000000 pypdl-1.0.2/pypdl/test.py
+-rw-rw-rw-   0        0        0     6412 2023-07-08 08:14:46.000000 pypdl-1.0.2/pypdl/utls.py
+drwxrwxrwx   0        0        0        0 2023-07-08 08:19:10.049691 pypdl-1.0.2/pypdl.egg-info/
+-rw-rw-rw-   0        0        0     9384 2023-07-08 08:19:09.000000 pypdl-1.0.2/pypdl.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      230 2023-07-08 08:19:09.000000 pypdl-1.0.2/pypdl.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-08 08:19:09.000000 pypdl-1.0.2/pypdl.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-07-08 08:19:09.000000 pypdl-1.0.2/pypdl.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-07-08 08:19:09.000000 pypdl-1.0.2/pypdl.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-08 08:19:10.051984 pypdl-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      927 2023-07-08 08:19:07.000000 pypdl-1.0.2/setup.py
```

### Comparing `pypdl-0.0.9/LICENSE` & `pypdl-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pypdl-0.0.9/PKG-INFO` & `pypdl-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: pypdl
-Version: 0.0.9
+Version: 1.0.2
 Summary: A concurrent python download manager
 Home-page: https://github.com/m-jishnu/pypdl
 Author: m-jishnu
 Author-email: <jishnum499@gmail.com>
 License: MIT
 Keywords: python,downloader,concurrent-downloader,parrel-downloader,download manager,fast-downloader
-Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3
+Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pypdl
 
 pypdl is a Python library for downloading files from the internet. It provides features such as multi-threaded downloads, retry download incase of failure and option to continue downloading using a different url if necessary, progress tracking, pause/resume functionality and many more.
```

### Comparing `pypdl-0.0.9/README.md` & `pypdl-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `pypdl-0.0.9/pypdl/main.py` & `pypdl-1.0.2/pypdl/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,50 +1,52 @@
 import json
 import threading
 import time
 from collections import deque
 from datetime import datetime
 from math import inf
 from pathlib import Path
+from typing import Callable, Dict, List, Optional, Union
 
 import requests
 from reprint import output
+
 from .utls import Multidown, Singledown, timestring
 
 
 class Downloader:
-    def __init__(self, StopEvent=None, headers=None):
+    def __init__(self, StopEvent: Optional[threading.Event] = None, headers: Optional[Dict[str, str]] = None):
         """
         Initializes the Downloader object.
 
         Parameters:
             StopEvent (threading.Event): Event to stop the download.
             headers (dict): User headers to be used in the download request.
         """
         # private attributes
         # keep track of recent download speed
         self._recent = deque([0] * 12, maxlen=12)
-        self._dic = {}  # dictionary to keep track of download progress
-        self._workers = []  # list of download worker threads
+        self._dic: Dict[Union[str, int], Union[int, bool, str, Dict[str, Union[str, int, bool]]]] = {}  # dictionary to keep track of download progress
+        self._workers: List[Union[Multidown, Singledown]] = []  # list of download worker threads
         self._Error = threading.Event()  # event to signal any download errors
 
         # public attributes
         self.totalMB = 0  # total download size in MB
         self.progress = 0  # download progress percentage
         self.speed = 0  # download speed in MB/s
         self.download_mode = ""  # download mode: single-threaded or multi-threaded
-        self.time_spent = None  # time spent downloading
+        self.time_spent: Optional[float] = None  # time spent downloading
         self.doneMB = 0  # amount of data downloaded in MB
         self.eta = "99:59:59"  # estimated time remaining for download completion
         self.remaining = 0  # amount of data remaining to be downloaded
         self.Stop = StopEvent if StopEvent else threading.Event() # event to signal download stop
         self.headers = headers if headers else {} # user-defined headers
         self.Failed = False  # flag to indicate if download failure
 
-    def download(self, url, filepath, num_connections, display, multithread):
+    def download(self, url: str, filepath: str, num_connections: int, display: bool, multithread: bool):
         """
         Download a file from the given URL.
 
         Parameters:
             url (str): The URL of the file to download.
             filepath (str): The file path to save the download.
             num_connections (int): The number of connections to use for a multi-threaded download.
@@ -233,22 +235,22 @@
         """
         Stop the download process.
         """
         self.Stop.set()
 
     def start(
         self,
-        url,
-        filepath,
-        num_connections=10,
-        display=True,
-        multithread=True,
-        block=True,
-        retries=0,
-        retry_func=None,
+        url: str,
+        filepath: str,
+        num_connections: int = 10,
+        display: bool = True,
+        multithread: bool = True,
+        block: bool = True,
+        retries: int = 0,
+        retry_func: Optional[Callable[[], str]] = None,
     ):
         """
         Start the download process.
 
         Parameters:
             url (str): The download URL.
             filepath (str): The file path to save the download.
```

### Comparing `pypdl-0.0.9/pypdl/test.py` & `pypdl-1.0.2/pypdl/test.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from main import Downloader
 import time
 
 if __name__ == "__main__":
     d = Downloader()
-    # url = "https://gamedownloads.rockstargames.com/public/installer/Rockstar-Games-Launcher.exe"
-    url = r"https://upcdn.io/kW15bUL/raw/y2mate.com%20-%20How%20to%20make%20dlls%20for%20m%20centers%20Minecraft%20bedrock_1080p.mp4"
-    d.headers = {"Authorization": "Bearer public_kW15bUL8oWrFf4ZvEEcU5cGfpMp3"}
+    url = "https://gamedownloads.rockstargames.com/public/installer/Rockstar-Games-Launcher.exe"
+    # url = r"https://upcdn.io/kW15bUL/raw/y2mate.com%20-%20How%20to%20make%20dlls%20for%20m%20centers%20Minecraft%20bedrock_1080p.mp4"
+    # d.headers = {"Authorization": "Bearer public_kW15bUL8oWrFf4ZvEEcU5cGfpMp3"}
     d.start(
         url,
         "r.exe",
         2,
         retries=2,
         display=True,
         multithread=True,
```

### Comparing `pypdl-0.0.9/pypdl/utls.py` & `pypdl-1.0.2/pypdl/utls.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 import os
+import threading
 import time
 from pathlib import Path
+from typing import Any, Dict, Union
 
 import requests
 
 
-def timestring(sec):
+def timestring(sec: int) -> str:
     """
     Converts seconds to a string formatted as HH:MM:SS.
 
     Parameters:
         sec (int): The number of seconds.
 
     Returns:
@@ -22,15 +24,16 @@
 
 
 class Multidown:
     """
     Class for downloading a specific part of a file in multiple chunks.
     """
 
-    def __init__(self, dic, id, stop, error, headers):
+    def __init__(self, dic: Dict[Union[str, int], Union[int, bool, str, Dict[str, Union[str, int, bool]]]], id: int,
+                 stop: threading.Event, error: threading.Event, headers: Dict[str, str]):
         """
         Initializes the Multidown object.
 
         Parameters:
             dic (dict): Dictionary containing download information for all parts.
                         Format: {start, curr, end, filepath, count, size, url, completed}
             id (int): ID of this download part.
@@ -42,27 +45,27 @@
         self.completed = 0  # whether the download for this part is complete
         self.id = id  # ID of this download part
         self.dic = dic  # dictionary containing download information for all parts
         self.stop = stop  # event to stop the download
         self.error = error  # event to indicate an error occurred
         self.headers = headers  # user headers
 
-    def getval(self, key):
+    def getval(self, key: str) -> Any:
         """
         Get the value of a key from the dictionary.
 
         Parameters:
             key (str): The key to retrieve the value for.
 
         Returns:
             Any: The value associated with the given key in the dictionary.
         """
         return self.dic[self.id][key]
 
-    def setval(self, key, val):
+    def setval(self, key: str, val: Any):
         """
         Set the value of a key in the dictionary.
 
         Parameters:
             key (str): The key to set the value for.
             val (Any): The value to set for the given key.
         """
@@ -119,15 +122,15 @@
 
 
 class Singledown:
     """
     Class for downloading a whole file in a single chunk.
     """
 
-    def __init__(self, url, path, stop, error, headers):
+    def __init__(self, url: str, path: str, stop: threading.Event, error: threading.Event, headers: Dict[str, str]):
         """
         Initializes the Singledown object.
 
         Parameters:
             url (str): The URL of the file to download.
             path (str): The path to save the downloaded file.
             stop (threading.Event): Event to stop the download.
```

### Comparing `pypdl-0.0.9/pypdl.egg-info/PKG-INFO` & `pypdl-1.0.2/pypdl.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: pypdl
-Version: 0.0.9
+Version: 1.0.2
 Summary: A concurrent python download manager
 Home-page: https://github.com/m-jishnu/pypdl
 Author: m-jishnu
 Author-email: <jishnum499@gmail.com>
 License: MIT
 Keywords: python,downloader,concurrent-downloader,parrel-downloader,download manager,fast-downloader
-Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3
+Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pypdl
 
 pypdl is a Python library for downloading files from the internet. It provides features such as multi-threaded downloads, retry download incase of failure and option to continue downloading using a different url if necessary, progress tracking, pause/resume functionality and many more.
```

### Comparing `pypdl-0.0.9/setup.py` & `pypdl-1.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.9'
+VERSION = '1.0.2'
 DESCRIPTION = 'A concurrent python download manager'
 with open("README.md", "r") as f:
     LONG_DESCRIPTION = f.read()
 
 setup(
     name="pypdl",
     version=VERSION,
```

