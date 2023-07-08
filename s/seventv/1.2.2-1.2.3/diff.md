# Comparing `tmp/seventv-1.2.2.tar.gz` & `tmp/seventv-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seventv-1.2.2.tar", last modified: Sat Jul  8 12:39:33 2023, max compression
+gzip compressed data, was "seventv-1.2.3.tar", last modified: Sat Jul  8 14:04:46 2023, max compression
```

## Comparing `seventv-1.2.2.tar` & `seventv-1.2.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 12:39:33.032331 seventv-1.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)    35823 2023-07-08 12:39:23.000000 seventv-1.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-07-08 12:39:33.032331 seventv-1.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2889 2023-07-08 12:39:23.000000 seventv-1.2.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 12:39:33.032331 seventv-1.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-07-08 12:39:23.000000 seventv-1.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 12:39:33.028331 seventv-1.2.2/seventv/
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-07-08 12:39:23.000000 seventv-1.2.2/seventv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3415 2023-07-08 12:39:23.000000 seventv-1.2.2/seventv/seventv.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 12:39:33.032331 seventv-1.2.2/seventv.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-07-08 12:39:33.000000 seventv-1.2.2/seventv.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-07-08 12:39:33.000000 seventv-1.2.2/seventv.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 12:39:33.000000 seventv-1.2.2/seventv.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-08 12:39:33.000000 seventv-1.2.2/seventv.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-08 12:39:33.000000 seventv-1.2.2/seventv.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 12:39:33.032331 seventv-1.2.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-07-08 12:39:23.000000 seventv-1.2.2/tests/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:04:46.148646 seventv-1.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    35823 2023-07-08 14:04:34.000000 seventv-1.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-07-08 14:04:46.148646 seventv-1.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3394 2023-07-08 14:04:34.000000 seventv-1.2.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 14:04:46.148646 seventv-1.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-07-08 14:04:34.000000 seventv-1.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:04:46.148646 seventv-1.2.3/seventv/
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-08 14:04:34.000000 seventv-1.2.3/seventv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3621 2023-07-08 14:04:34.000000 seventv-1.2.3/seventv/seventv.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:04:46.148646 seventv-1.2.3/seventv.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-07-08 14:04:46.000000 seventv-1.2.3/seventv.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-07-08 14:04:46.000000 seventv-1.2.3/seventv.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 14:04:46.000000 seventv-1.2.3/seventv.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-08 14:04:46.000000 seventv-1.2.3/seventv.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-08 14:04:46.000000 seventv-1.2.3/seventv.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:04:46.148646 seventv-1.2.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-07-08 14:04:34.000000 seventv-1.2.3/tests/test.py
```

### Comparing `seventv-1.2.2/LICENSE` & `seventv-1.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `seventv-1.2.2/PKG-INFO` & `seventv-1.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seventv
-Version: 1.2.2
+Version: 1.2.3
 Summary: An asynchronous API-wrapper for 7tv.app
 Author: Jässin Aouani
 Author-email: jassin@aouani.de
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `seventv-1.2.2/README.md` & `seventv-1.2.3/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 # seventv
 an asynchronous Python API-wrapper for [7tv.app](https://7tv.app)
 
 This API-wrapper makes use of the 7tv API (v3) to make it possible to get emotes, details about them, and soon some more things the API supports.
 
 To get emotes by search query, the wrapper uses the GraphQL endpoint ```https://7tv.io/v3/gql``` because it seems to currently be the only working one for searching emotes. 
 
+<sub>this project is not associated with or owned by 7tv or it's owners<sub>
+
 # Installation
 ## How to install:
 ```
 pip install seventv
 ```
 ### requires:
 ```
@@ -23,24 +25,30 @@
 
 Example usage:
 ```
 import asyncio
 import seventv
 
 async def myFunctionSearchEmote():
-    mySeventvSession = seventv() # initialize the session
+    mySevenTvSession = seventv.seventv() # initialize an instance of the seventv() class
     
-    emotes = await mySeventvSession.emote_search("pepe", case_sensitive=True)
+    emotes = await mySevenTvSession.emote_search("pepe", case_sensitive=True)
     # searches for "pepe", using the optional filter "case_sensitive"
     
     print(emotes[2]) # get the third emote from the search results
-    await mySeventvSession.close() # later close the session
+    await mySevenTvSession.close() # later close the session
 
 asyncio.run(getemote())
 ```
+_About closing sessions: initializing a session with seventv.sevent() creates an aiohttp session. This session should be closed by calling yourSession.close() at some point. Not doing so will cause a warning like this:_ 
+```
+Unclosed session
+client_session: <aiohttp.client.ClientSession object at 0x7fd2b06469b0>
+```
+_Closing/reopening it after every request does avoid the warning, but is not very efficent. It would be optimal to close the session when the service/code that uses it stops._
 
 Sample output: third Emote object in the search results:
 ```Emote(id: 60a304efac2bcb20ef20fa89, name: pepeMeltdown, owner_username: supernoahtv, host_url: //cdn.7tv.app/emote/60a304efac2bcb20ef20fa89)```
 
 The output from a search is an array with the Emote objects inside.
 Each emote contains the following properties:
 - id
@@ -51,15 +59,14 @@
 _Sidenote: Keep in mind that to get the emote using the url, the file extension must be appended to the host_url. Emotes are stored on 7tv in different sizes, usually ranging from 1x.webp to 4x.webp. Not every emote might have every size though, so look it up or go with x2 or x3 which the majority of emotes have._
 
 ### Currently available search filters (optional):
 
 | filter                         | meaning | default value |     
 | ---------------------------------------------- | -------- | --------------- | 
 | limit (int) | how many emotes are contained in the response      | 12             |     
-| case_sensitive (bool)                         | whether or not upper-/lowercase letters are treated differently or will not be distinguished      | False             |     
-| animated (bool)                                     |only return animated emotes in search results          | False                 |     
-| ---more to be added soon---                                  |          |                 |     |                                               |          |                 |     
+| case_sensitive (bool) | whether or not upper-/lowercase letters are treated differently or will not be distinguished   | False |     
+| animated (bool) |only return animated emotes in search results          | False                 |     
+| exact_match (bool) | only return emotes that exactly match the search query | False   |     |                                               |          |                 |     
 
 
 soon to be added functionality: 
-- more search filters
-- getting an emote by it's id
+- get an emote by it's id
```

### Comparing `seventv-1.2.2/setup.py` & `seventv-1.2.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='seventv',
-    version='1.2.2',
+    version='1.2.3',
     author='Jässin Aouani',
     author_email='jassin@aouani.de',
     description='An asynchronous API-wrapper for 7tv.app',
     long_description = """
         An asynchronous Python API-wrapper for 7tv.app. 
         It makes use of the 7tv API (v3) to make it possible to get emotes, details about them, and soon some more things the API supports.
         To get emotes by search query, the wrapper uses the GraphQL endpoint
```

### Comparing `seventv-1.2.2/seventv/seventv.py` & `seventv-1.2.3/seventv/seventv.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,15 +43,21 @@
     def __init__(self):
         self.endpoint = "https://7tv.io/v3/gql"
         self.session = aiohttp.ClientSession()
 
     async def close(self):
         await self.session.close()
 
-    async def emote_search(self, searchterm: str = "", limit: int = 12, case_sensitive: bool = False, animated: bool = False):
+    async def emote_search(self, 
+                           searchterm: str = "", 
+                           limit: int = 12, 
+                           case_sensitive: bool = False, 
+                           animated: bool = False,
+                           exact_match: bool = False
+                           ):
         url = self.endpoint
         headers = {
             "Content-Type": "application/json"
         }
         payload = {
             "operationName": "SearchEmotes",
             "variables": {
@@ -60,15 +66,15 @@
                 "page": 1,
                 "sort": {
                     "value": "popularity",
                     "order": "DESCENDING"
                 },
                 "filter": {
                     "category": "TOP",
-                    "exact_match": False,
+                    "exact_match": exact_match,
                     "case_sensitive": case_sensitive,
                     "ignore_tags": False,
                     "zero_width": False,
                     "animated": animated,
                     "aspect_ratio": ""
                 }
             },
```

### Comparing `seventv-1.2.2/seventv.egg-info/PKG-INFO` & `seventv-1.2.3/seventv.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seventv
-Version: 1.2.2
+Version: 1.2.3
 Summary: An asynchronous API-wrapper for 7tv.app
 Author: Jässin Aouani
 Author-email: jassin@aouani.de
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

