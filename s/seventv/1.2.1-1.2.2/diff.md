# Comparing `tmp/seventv-1.2.1.tar.gz` & `tmp/seventv-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seventv-1.2.1.tar", last modified: Sat Jul  8 12:10:43 2023, max compression
+gzip compressed data, was "seventv-1.2.2.tar", last modified: Sat Jul  8 12:39:33 2023, max compression
```

## Comparing `seventv-1.2.1.tar` & `seventv-1.2.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 12:10:43.088722 seventv-1.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)    35823 2023-07-08 12:10:30.000000 seventv-1.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-07-08 12:10:43.088722 seventv-1.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2902 2023-07-08 12:10:30.000000 seventv-1.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 12:10:43.088722 seventv-1.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-07-08 12:10:30.000000 seventv-1.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 12:10:43.088722 seventv-1.2.1/seventv/
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-07-08 12:10:30.000000 seventv-1.2.1/seventv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3415 2023-07-08 12:10:30.000000 seventv-1.2.1/seventv/seventv.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 12:10:43.088722 seventv-1.2.1/seventv.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-07-08 12:10:43.000000 seventv-1.2.1/seventv.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-07-08 12:10:43.000000 seventv-1.2.1/seventv.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 12:10:43.000000 seventv-1.2.1/seventv.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-08 12:10:43.000000 seventv-1.2.1/seventv.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-08 12:10:43.000000 seventv-1.2.1/seventv.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 12:10:43.088722 seventv-1.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-07-08 12:10:30.000000 seventv-1.2.1/tests/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 12:39:33.032331 seventv-1.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    35823 2023-07-08 12:39:23.000000 seventv-1.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-07-08 12:39:33.032331 seventv-1.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2889 2023-07-08 12:39:23.000000 seventv-1.2.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 12:39:33.032331 seventv-1.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-07-08 12:39:23.000000 seventv-1.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 12:39:33.028331 seventv-1.2.2/seventv/
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-07-08 12:39:23.000000 seventv-1.2.2/seventv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3415 2023-07-08 12:39:23.000000 seventv-1.2.2/seventv/seventv.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 12:39:33.032331 seventv-1.2.2/seventv.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-07-08 12:39:33.000000 seventv-1.2.2/seventv.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-07-08 12:39:33.000000 seventv-1.2.2/seventv.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 12:39:33.000000 seventv-1.2.2/seventv.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-08 12:39:33.000000 seventv-1.2.2/seventv.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-08 12:39:33.000000 seventv-1.2.2/seventv.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 12:39:33.032331 seventv-1.2.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-07-08 12:39:23.000000 seventv-1.2.2/tests/test.py
```

### Comparing `seventv-1.2.1/LICENSE` & `seventv-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `seventv-1.2.1/PKG-INFO` & `seventv-1.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seventv
-Version: 1.2.1
+Version: 1.2.2
 Summary: An asynchronous API-wrapper for 7tv.app
 Author: Jässin Aouani
 Author-email: jassin@aouani.de
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `seventv-1.2.1/README.md` & `seventv-1.2.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -20,24 +20,24 @@
 - create a class instance of sevenTV
 - await the ```.emote_search``` method with your search query string and optional filters
 - don't forget to close the session at some later point, using ```.close()```.
 
 Example usage:
 ```
 import asyncio
-from sevenTV import sevenTV
+import seventv
 
 async def myFunctionSearchEmote():
-    mySevenTVSession = sevenTV() # initialize the session
+    mySeventvSession = seventv() # initialize the session
     
-    emotes = await mySevenTVSession.emote_search("pepe", case_sensitive=True)
+    emotes = await mySeventvSession.emote_search("pepe", case_sensitive=True)
     # searches for "pepe", using the optional filter "case_sensitive"
     
     print(emotes[2]) # get the third emote from the search results
-    await mySevenTVSession.close() # later close the session
+    await mySeventvSession.close() # later close the session
 
 asyncio.run(getemote())
 ```
 
 Sample output: third Emote object in the search results:
 ```Emote(id: 60a304efac2bcb20ef20fa89, name: pepeMeltdown, owner_username: supernoahtv, host_url: //cdn.7tv.app/emote/60a304efac2bcb20ef20fa89)```
```

### Comparing `seventv-1.2.1/setup.py` & `seventv-1.2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='seventv',
-    version='1.2.1',
+    version='1.2.2',
     author='Jässin Aouani',
     author_email='jassin@aouani.de',
     description='An asynchronous API-wrapper for 7tv.app',
     long_description = """
         An asynchronous Python API-wrapper for 7tv.app. 
         It makes use of the 7tv API (v3) to make it possible to get emotes, details about them, and soon some more things the API supports.
         To get emotes by search query, the wrapper uses the GraphQL endpoint
```

### Comparing `seventv-1.2.1/seventv/seventv.py` & `seventv-1.2.2/seventv/seventv.py`

 * *Files identical despite different names*

### Comparing `seventv-1.2.1/seventv.egg-info/PKG-INFO` & `seventv-1.2.2/seventv.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seventv
-Version: 1.2.1
+Version: 1.2.2
 Summary: An asynchronous API-wrapper for 7tv.app
 Author: Jässin Aouani
 Author-email: jassin@aouani.de
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

