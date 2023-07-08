# Comparing `tmp/seventv-1.1.6.tar.gz` & `tmp/seventv-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seventv-1.1.6.tar", last modified: Sat Jul  8 11:19:29 2023, max compression
+gzip compressed data, was "seventv-1.2.1.tar", last modified: Sat Jul  8 12:10:43 2023, max compression
```

## Comparing `seventv-1.1.6.tar` & `seventv-1.2.1.tar`

### file list

```diff
@@ -1,15 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 11:19:29.484246 seventv-1.1.6/
--rw-r--r--   0 runner    (1001) docker     (123)    35823 2023-07-08 11:19:19.000000 seventv-1.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-07-08 11:19:29.484246 seventv-1.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2954 2023-07-08 11:19:19.000000 seventv-1.1.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 11:19:29.484246 seventv-1.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-07-08 11:19:19.000000 seventv-1.1.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 11:19:29.484246 seventv-1.1.6/seventv/
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-07-08 11:19:19.000000 seventv-1.1.6/seventv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3497 2023-07-08 11:19:19.000000 seventv-1.1.6/seventv/seventv.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 11:19:29.484246 seventv-1.1.6/seventv.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-07-08 11:19:29.000000 seventv-1.1.6/seventv.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-07-08 11:19:29.000000 seventv-1.1.6/seventv.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 11:19:29.000000 seventv-1.1.6/seventv.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-08 11:19:29.000000 seventv-1.1.6/seventv.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-08 11:19:29.000000 seventv-1.1.6/seventv.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 12:10:43.088722 seventv-1.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35823 2023-07-08 12:10:30.000000 seventv-1.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-07-08 12:10:43.088722 seventv-1.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2902 2023-07-08 12:10:30.000000 seventv-1.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 12:10:43.088722 seventv-1.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-07-08 12:10:30.000000 seventv-1.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 12:10:43.088722 seventv-1.2.1/seventv/
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-07-08 12:10:30.000000 seventv-1.2.1/seventv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3415 2023-07-08 12:10:30.000000 seventv-1.2.1/seventv/seventv.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 12:10:43.088722 seventv-1.2.1/seventv.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-07-08 12:10:43.000000 seventv-1.2.1/seventv.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-07-08 12:10:43.000000 seventv-1.2.1/seventv.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 12:10:43.000000 seventv-1.2.1/seventv.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-08 12:10:43.000000 seventv-1.2.1/seventv.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-08 12:10:43.000000 seventv-1.2.1/seventv.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 12:10:43.088722 seventv-1.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-07-08 12:10:30.000000 seventv-1.2.1/tests/test.py
```

### Comparing `seventv-1.1.6/LICENSE` & `seventv-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `seventv-1.1.6/README.md` & `seventv-1.2.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,33 +1,30 @@
+# seventv
 an asynchronous Python API-wrapper for [7tv.app](https://7tv.app)
 
 This API-wrapper makes use of the 7tv API (v3) to make it possible to get emotes, details about them, and soon some more things the API supports.
 
 To get emotes by search query, the wrapper uses the GraphQL endpoint ```https://7tv.io/v3/gql``` because it seems to currently be the only working one for searching emotes. 
 
 # Installation
-## requirement(s):
+## How to install:
 ```
-aiohttp
-json
-```
-```
-pip install git+https://github.com/probablyjassin/sevenTVpy
+pip install seventv
 ```
-or
+### requires:
 ```
-pip install seventv
+aiohttp
 ```
 
 # Usage
 To search for an emote and make use of the search results, do the following (asynchronously):
 - create a class instance of sevenTV
 - await the ```.emote_search``` method with your search query string and optional filters
 - don't forget to close the session at some later point, using ```.close()```.
-- 
+
 Example usage:
 ```
 import asyncio
 from sevenTV import sevenTV
 
 async def myFunctionSearchEmote():
     mySevenTVSession = sevenTV() # initialize the session
@@ -47,22 +44,22 @@
 The output from a search is an array with the Emote objects inside.
 Each emote contains the following properties:
 - id
 - name
 - owner_username
 - host_url
 
-_Sidenote: To access the emote using the url, the file extension must be appended to the host_url. Emotes are stored on 7tv in different sizes, usually ranging from 1x.webp to 4x.webp. Not every emote might have every size though, so look it up or go with x2 or x3 which the majority of emotes have._
+_Sidenote: Keep in mind that to get the emote using the url, the file extension must be appended to the host_url. Emotes are stored on 7tv in different sizes, usually ranging from 1x.webp to 4x.webp. Not every emote might have every size though, so look it up or go with x2 or x3 which the majority of emotes have._
 
 ### Currently available search filters (optional):
 
-| filter                         | meaning | default value |     |
-| ---------------------------------------------- | -------- | --------------- | --- |
-| limit (int) | how many emotes are contained in the response      | 12             |     |
-| case_sensitive (bool)                         | whether or not upper-/lowercase letters are treated differently or will not be distinguished      | False             |     |
-| animated (bool)                                     |only return animated emotes in search results          | False                 |     |
-| ---more to be added soon---                                  |          |                 |     |                                               |          |                 |     |
+| filter                         | meaning | default value |     
+| ---------------------------------------------- | -------- | --------------- | 
+| limit (int) | how many emotes are contained in the response      | 12             |     
+| case_sensitive (bool)                         | whether or not upper-/lowercase letters are treated differently or will not be distinguished      | False             |     
+| animated (bool)                                     |only return animated emotes in search results          | False                 |     
+| ---more to be added soon---                                  |          |                 |     |                                               |          |                 |     
 
 
 soon to be added functionality: 
 - more search filters
 - getting an emote by it's id
```

### Comparing `seventv-1.1.6/seventv/seventv.py` & `seventv-1.2.1/seventv/seventv.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 from __future__ import annotations
-
 import aiohttp
-import json
 
 class Emote:
     def __init__(self, id, name, owner_username, host_url):
         self.id = id
         self.name = name
         self.owner_username = owner_username
         self.host_url = host_url
@@ -45,39 +43,36 @@
     def __init__(self):
         self.endpoint = "https://7tv.io/v3/gql"
         self.session = aiohttp.ClientSession()
 
     async def close(self):
         await self.session.close()
 
-    def to_json(self):
-        return json.dumps(self.__dict__, indent=4)
-
-    async def emote_search(self, searchterm, **kwargs):
+    async def emote_search(self, searchterm: str = "", limit: int = 12, case_sensitive: bool = False, animated: bool = False):
         url = self.endpoint
         headers = {
             "Content-Type": "application/json"
         }
         payload = {
             "operationName": "SearchEmotes",
             "variables": {
                 "query": searchterm,
-                "limit": kwargs.get("limit", 12),
+                "limit": limit,
                 "page": 1,
                 "sort": {
                     "value": "popularity",
                     "order": "DESCENDING"
                 },
                 "filter": {
                     "category": "TOP",
                     "exact_match": False,
-                    "case_sensitive": kwargs.get("case_sensitive", False),
+                    "case_sensitive": case_sensitive,
                     "ignore_tags": False,
                     "zero_width": False,
-                    "animated": kwargs.get("animated", False),
+                    "animated": animated,
                     "aspect_ratio": ""
                 }
             },
             "query": "query SearchEmotes($query: String!, $page: Int, $sort: Sort, $limit: Int, $filter: EmoteSearchFilter) {\n  emotes(query: $query, page: $page, sort: $sort, limit: $limit, filter: $filter) {\n    count\n    items {\n      id\n      name\n      state\n      trending\n      owner {\n        id\n        username\n        display_name\n        style {\n          color\n          paint_id\n          __typename\n        }\n        __typename\n      }\n      flags\n      host {\n        url\n        files {\n          name\n          format\n          width\n          height\n          __typename\n        }\n        __typename\n      }\n      __typename\n    }\n    __typename\n  }\n}"
         }
 
         async with self.session.post(url, json=payload, headers=headers) as response:
```

