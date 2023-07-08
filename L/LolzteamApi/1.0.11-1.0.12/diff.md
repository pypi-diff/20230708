# Comparing `tmp/LolzteamApi-1.0.11.tar.gz` & `tmp/LolzteamApi-1.0.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LolzteamApi-1.0.11.tar", last modified: Fri Jul  7 15:58:15 2023, max compression
+gzip compressed data, was "LolzteamApi-1.0.12.tar", last modified: Fri Jul  7 21:05:15 2023, max compression
```

## Comparing `LolzteamApi-1.0.11.tar` & `LolzteamApi-1.0.12.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-07-07 15:58:15.136317 LolzteamApi-1.0.11/
--rw-rw-rw-   0        0        0     1082 2023-07-07 14:49:03.000000 LolzteamApi-1.0.11/LICENSE
-drwxrwxrwx   0        0        0        0 2023-07-07 15:58:15.127318 LolzteamApi-1.0.11/LolzteamApi/
--rw-rw-rw-   0        0        0   163281 2023-07-07 15:57:48.000000 LolzteamApi-1.0.11/LolzteamApi/LolzteamApi.py
--rw-rw-rw-   0        0        0       36 2023-07-07 15:50:35.000000 LolzteamApi-1.0.11/LolzteamApi/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-07 15:58:15.134314 LolzteamApi-1.0.11/LolzteamApi.egg-info/
--rw-rw-rw-   0        0        0     1650 2023-07-07 15:58:14.000000 LolzteamApi-1.0.11/LolzteamApi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      251 2023-07-07 15:58:14.000000 LolzteamApi-1.0.11/LolzteamApi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-07 15:58:14.000000 LolzteamApi-1.0.11/LolzteamApi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-07-07 15:58:14.000000 LolzteamApi-1.0.11/LolzteamApi.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-07-07 15:58:14.000000 LolzteamApi-1.0.11/LolzteamApi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1650 2023-07-07 15:58:15.135316 LolzteamApi-1.0.11/PKG-INFO
--rw-rw-rw-   0        0        0      690 2023-07-06 22:34:30.000000 LolzteamApi-1.0.11/README.md
--rw-rw-rw-   0        0        0       42 2023-07-07 15:58:15.136317 LolzteamApi-1.0.11/setup.cfg
--rw-rw-rw-   0        0        0      674 2023-07-07 15:57:10.000000 LolzteamApi-1.0.11/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-07 21:05:15.321929 LolzteamApi-1.0.12/
+-rw-rw-rw-   0        0        0     1082 2023-07-07 14:49:03.000000 LolzteamApi-1.0.12/LICENSE
+drwxrwxrwx   0        0        0        0 2023-07-07 21:05:15.314929 LolzteamApi-1.0.12/LolzteamApi/
+-rw-rw-rw-   0        0        0   163270 2023-07-07 21:04:12.000000 LolzteamApi-1.0.12/LolzteamApi/LolzteamApi.py
+-rw-rw-rw-   0        0        0       38 2023-07-07 21:04:12.000000 LolzteamApi-1.0.12/LolzteamApi/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-07 21:05:15.319927 LolzteamApi-1.0.12/LolzteamApi.egg-info/
+-rw-rw-rw-   0        0        0     2282 2023-07-07 21:05:14.000000 LolzteamApi-1.0.12/LolzteamApi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      251 2023-07-07 21:05:15.000000 LolzteamApi-1.0.12/LolzteamApi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-07 21:05:15.000000 LolzteamApi-1.0.12/LolzteamApi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-07-07 21:05:15.000000 LolzteamApi-1.0.12/LolzteamApi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-07-07 21:05:15.000000 LolzteamApi-1.0.12/LolzteamApi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2282 2023-07-07 21:05:15.320926 LolzteamApi-1.0.12/PKG-INFO
+-rw-rw-rw-   0        0        0     1881 2023-07-07 21:02:06.000000 LolzteamApi-1.0.12/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-07 21:05:15.321929 LolzteamApi-1.0.12/setup.cfg
+-rw-rw-rw-   0        0        0      674 2023-07-07 21:03:24.000000 LolzteamApi-1.0.12/setup.py
```

### Comparing `LolzteamApi-1.0.11/LICENSE` & `LolzteamApi-1.0.12/LICENSE`

 * *Files identical despite different names*

### Comparing `LolzteamApi-1.0.11/LolzteamApi/LolzteamApi.py` & `LolzteamApi-1.0.12/LolzteamApi/LolzteamApi.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import requests
 import time
 import json
 
-# Lolzteam
+
 class LolzteamApi:
     def __init__(self, token: str, bypass_429: bool = True):
         """
         :param token: Your token. You can get in there -> https://zelenka.guru/account/api
         :param bypass_429: Bypass status code 429 by sleep
         """
 
@@ -1916,15 +1916,15 @@
 
         class __Conversations:
             class __Conversations_messages:
                 def __init__(self, __api_self):
                     self.__api = __api_self
 
                 def get_all(self, conversation_id: int, page: int = None, limit: int = None, order: str = None,
-                             before: int = None, after: int = None):
+                            before: int = None, after: int = None):
                     """
                     GET https://api.zelenka.guru/conversation-messages
 
                     List of messages in a conversation (with pagination).
 
                     Required scopes: conversate, read
```

### Comparing `LolzteamApi-1.0.11/setup.py` & `LolzteamApi-1.0.12/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 requirements = ["requests"]
 
 setuptools.setup(
     name="LolzteamApi",
-    version="1.0.11",
+    version="1.0.12",
     author="AS7RID",
     author_email="as7ridwork@gmail.com",
     description="A library that contains all the methods of the Lolzteam API (Market/Forum)",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/AS7RIDENIED/Lolzteam_Python_Api",
     packages=setuptools.find_packages(),
```

