# Comparing `tmp/python-postman-0.2.0.tar.gz` & `tmp/python-postman-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-postman-0.2.0.tar", last modified: Sat Jun 24 15:22:08 2023, max compression
+gzip compressed data, was "python-postman-0.3.0.tar", last modified: Sat Jul  8 04:31:17 2023, max compression
```

## Comparing `python-postman-0.2.0.tar` & `python-postman-0.3.0.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxrwxrwx   0        0        0        0 2023-06-24 15:22:08.266810 python-postman-0.2.0/
--rw-rw-rw-   0        0        0     1941 2023-06-24 14:45:03.000000 python-postman-0.2.0/.gitignore
--rw-rw-rw-   0        0        0     1085 2023-02-14 00:08:21.000000 python-postman-0.2.0/LICENSE
--rw-rw-rw-   0        0        0     2103 2023-06-24 15:22:08.265808 python-postman-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     1697 2023-06-24 14:59:14.000000 python-postman-0.2.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-24 15:22:08.214808 python-postman-0.2.0/examples/
-drwxrwxrwx   0        0        0        0 2023-06-24 15:22:08.232808 python-postman-0.2.0/examples/collections/
--rw-rw-rw-   0        0        0     2001 2023-06-24 14:59:14.000000 python-postman-0.2.0/examples/collections/Coinmarketcap.postman_collection.json
--rw-rw-rw-   0        0        0     1150 2023-06-24 14:59:14.000000 python-postman-0.2.0/examples/collections/PokeAPI.postman_collection.json
-drwxrwxrwx   0        0        0        0 2023-06-24 15:22:08.234808 python-postman-0.2.0/examples/models/
--rw-rw-rw-   0        0        0     2299 2023-06-24 14:59:14.000000 python-postman-0.2.0/examples/models/coinmarketcap_example.py
--rw-rw-rw-   0        0        0     2492 2023-06-24 14:59:14.000000 python-postman-0.2.0/examples/models/pokeapi_example.py
-drwxrwxrwx   0        0        0        0 2023-06-24 15:22:08.243808 python-postman-0.2.0/pypostman/
--rw-rw-rw-   0        0        0        0 2023-06-24 14:45:03.000000 python-postman-0.2.0/pypostman/__init__.py
--rw-rw-rw-   0        0        0      461 2023-06-24 14:45:03.000000 python-postman-0.2.0/pypostman/__main__.py
--rw-rw-rw-   0        0        0     2458 2023-06-24 14:45:03.000000 python-postman-0.2.0/pypostman/auth.py
--rw-rw-rw-   0        0        0      185 2023-06-24 14:45:03.000000 python-postman-0.2.0/pypostman/body.py
--rw-rw-rw-   0        0        0     1430 2023-06-24 14:45:03.000000 python-postman-0.2.0/pypostman/collection.py
--rw-rw-rw-   0        0        0     2519 2023-06-24 14:45:03.000000 python-postman-0.2.0/pypostman/config.py
--rw-rw-rw-   0        0        0     3629 2023-06-24 14:45:03.000000 python-postman-0.2.0/pypostman/environment.py
--rw-rw-rw-   0        0        0      737 2023-06-24 14:45:03.000000 python-postman-0.2.0/pypostman/event.py
--rw-rw-rw-   0        0        0      455 2023-06-24 14:45:03.000000 python-postman-0.2.0/pypostman/header.py
--rw-rw-rw-   0        0        0      746 2023-06-24 14:45:03.000000 python-postman-0.2.0/pypostman/item.py
-drwxrwxrwx   0        0        0        0 2023-06-24 15:22:08.246808 python-postman-0.2.0/pypostman/modules/
--rw-rw-rw-   0        0        0     8312 2023-06-24 14:45:03.000000 python-postman-0.2.0/pypostman/modules/file.py
--rw-rw-rw-   0        0        0     4031 2023-06-24 14:59:14.000000 python-postman-0.2.0/pypostman/modules/http.py
--rw-rw-rw-   0        0        0     1710 2023-06-24 14:45:03.000000 python-postman-0.2.0/pypostman/modules/logger.py
--rw-rw-rw-   0        0        0     4822 2023-06-24 14:45:03.000000 python-postman-0.2.0/pypostman/postman.py
--rw-rw-rw-   0        0        0      710 2023-06-24 14:45:03.000000 python-postman-0.2.0/pypostman/request.py
--rw-rw-rw-   0        0        0      106 2023-06-24 14:45:03.000000 python-postman-0.2.0/pypostman/template.py
--rw-rw-rw-   0        0        0     3143 2023-06-24 14:45:03.000000 python-postman-0.2.0/pypostman/url.py
-drwxrwxrwx   0        0        0        0 2023-06-24 15:22:08.247808 python-postman-0.2.0/pypostman/utils/
--rw-rw-rw-   0        0        0        0 2023-06-24 14:45:03.000000 python-postman-0.2.0/pypostman/utils/.gitkeep
--rw-rw-rw-   0        0        0     1017 2023-06-24 14:45:03.000000 python-postman-0.2.0/pypostman/utils/cli.py
--rw-rw-rw-   0        0        0     2370 2023-06-24 14:45:03.000000 python-postman-0.2.0/pypostman/variable.py
--rw-rw-rw-   0        0        0      849 2023-06-24 15:21:56.000000 python-postman-0.2.0/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-06-24 15:22:08.264813 python-postman-0.2.0/python_postman.egg-info/
--rw-rw-rw-   0        0        0     2103 2023-06-24 15:22:08.000000 python-postman-0.2.0/python_postman.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      898 2023-06-24 15:22:08.000000 python-postman-0.2.0/python_postman.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-24 15:22:08.000000 python-postman-0.2.0/python_postman.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       54 2023-06-24 15:22:08.000000 python-postman-0.2.0/python_postman.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      116 2023-06-24 15:22:08.000000 python-postman-0.2.0/python_postman.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-06-24 15:22:08.000000 python-postman-0.2.0/python_postman.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-24 15:22:08.266810 python-postman-0.2.0/setup.cfg
+drwxr-xr-x   0 wry        (501) staff       (20)        0 2023-07-08 04:31:17.330135 python-postman-0.3.0/
+-rw-r--r--   0 wry        (501) staff       (20)     1810 2023-07-08 04:20:36.000000 python-postman-0.3.0/.gitignore
+-rw-r--r--   0 wry        (501) staff       (20)     1064 2022-12-01 02:32:51.000000 python-postman-0.3.0/LICENSE
+-rw-r--r--   0 wry        (501) staff       (20)     2030 2023-07-08 04:31:17.329964 python-postman-0.3.0/PKG-INFO
+-rw-r--r--   0 wry        (501) staff       (20)     1697 2023-06-24 15:15:52.000000 python-postman-0.3.0/README.md
+drwxr-xr-x   0 wry        (501) staff       (20)        0 2023-07-08 04:31:17.323197 python-postman-0.3.0/examples/
+drwxr-xr-x   0 wry        (501) staff       (20)        0 2023-07-08 04:31:17.324554 python-postman-0.3.0/examples/collections/
+-rw-r--r--   0 wry        (501) staff       (20)     4705 2023-07-08 03:51:35.000000 python-postman-0.3.0/examples/collections/Coinmarketcap.postman_collection.json
+-rw-r--r--   0 wry        (501) staff       (20)     1085 2023-03-06 17:39:27.000000 python-postman-0.3.0/examples/collections/PokeAPI.postman_collection.json
+drwxr-xr-x   0 wry        (501) staff       (20)        0 2023-07-08 04:31:17.325006 python-postman-0.3.0/examples/models/
+-rw-r--r--   0 wry        (501) staff       (20)     2367 2023-07-08 03:51:35.000000 python-postman-0.3.0/examples/models/coinmarketcap_example.py
+-rw-r--r--   0 wry        (501) staff       (20)     2426 2023-06-24 15:15:52.000000 python-postman-0.3.0/examples/models/pokeapi_example.py
+drwxr-xr-x   0 wry        (501) staff       (20)        0 2023-07-08 04:31:17.327956 python-postman-0.3.0/pypostman/
+-rw-r--r--   0 wry        (501) staff       (20)        0 2023-03-06 17:39:27.000000 python-postman-0.3.0/pypostman/__init__.py
+-rw-r--r--   0 wry        (501) staff       (20)      444 2023-03-06 17:39:27.000000 python-postman-0.3.0/pypostman/__main__.py
+-rw-r--r--   0 wry        (501) staff       (20)     2381 2023-03-06 17:39:27.000000 python-postman-0.3.0/pypostman/auth.py
+-rw-r--r--   0 wry        (501) staff       (20)      177 2023-03-06 17:39:27.000000 python-postman-0.3.0/pypostman/body.py
+-rw-r--r--   0 wry        (501) staff       (20)     1394 2023-03-06 17:39:27.000000 python-postman-0.3.0/pypostman/collection.py
+-rw-r--r--   0 wry        (501) staff       (20)     2411 2023-03-06 17:39:27.000000 python-postman-0.3.0/pypostman/config.py
+-rw-r--r--   0 wry        (501) staff       (20)     3528 2023-03-06 17:39:27.000000 python-postman-0.3.0/pypostman/environment.py
+-rw-r--r--   0 wry        (501) staff       (20)      707 2023-03-06 17:39:27.000000 python-postman-0.3.0/pypostman/event.py
+-rw-r--r--   0 wry        (501) staff       (20)      437 2023-03-06 17:39:27.000000 python-postman-0.3.0/pypostman/header.py
+-rw-r--r--   0 wry        (501) staff       (20)      718 2023-03-06 17:39:27.000000 python-postman-0.3.0/pypostman/item.py
+drwxr-xr-x   0 wry        (501) staff       (20)        0 2023-07-08 04:31:17.328610 python-postman-0.3.0/pypostman/modules/
+-rw-r--r--   0 wry        (501) staff       (20)     8108 2023-06-24 20:49:48.000000 python-postman-0.3.0/pypostman/modules/file.py
+-rw-r--r--   0 wry        (501) staff       (20)     3905 2023-03-06 17:39:27.000000 python-postman-0.3.0/pypostman/modules/http.py
+-rw-r--r--   0 wry        (501) staff       (20)     1661 2023-03-06 17:39:27.000000 python-postman-0.3.0/pypostman/modules/logger.py
+-rw-r--r--   0 wry        (501) staff       (20)     4679 2023-03-06 17:39:27.000000 python-postman-0.3.0/pypostman/postman.py
+-rw-r--r--   0 wry        (501) staff       (20)      693 2023-03-06 17:39:27.000000 python-postman-0.3.0/pypostman/request.py
+-rw-r--r--   0 wry        (501) staff       (20)      101 2023-03-06 17:39:27.000000 python-postman-0.3.0/pypostman/template.py
+-rw-r--r--   0 wry        (501) staff       (20)     3049 2023-03-06 17:39:27.000000 python-postman-0.3.0/pypostman/url.py
+drwxr-xr-x   0 wry        (501) staff       (20)        0 2023-07-08 04:31:17.328906 python-postman-0.3.0/pypostman/utils/
+-rw-r--r--   0 wry        (501) staff       (20)      975 2023-03-06 17:39:27.000000 python-postman-0.3.0/pypostman/utils/cli.py
+-rw-r--r--   0 wry        (501) staff       (20)     2917 2023-07-08 03:51:35.000000 python-postman-0.3.0/pypostman/utils/load_dotenvc.py
+-rw-r--r--   0 wry        (501) staff       (20)     2308 2023-03-06 17:39:27.000000 python-postman-0.3.0/pypostman/variable.py
+-rw-r--r--   0 wry        (501) staff       (20)      828 2023-07-08 04:30:51.000000 python-postman-0.3.0/pyproject.toml
+drwxr-xr-x   0 wry        (501) staff       (20)        0 2023-07-08 04:31:17.329694 python-postman-0.3.0/python_postman.egg-info/
+-rw-r--r--   0 wry        (501) staff       (20)     2030 2023-07-08 04:31:17.000000 python-postman-0.3.0/python_postman.egg-info/PKG-INFO
+-rw-r--r--   0 wry        (501) staff       (20)      905 2023-07-08 04:31:17.000000 python-postman-0.3.0/python_postman.egg-info/SOURCES.txt
+-rw-r--r--   0 wry        (501) staff       (20)        1 2023-07-08 04:31:17.000000 python-postman-0.3.0/python_postman.egg-info/dependency_links.txt
+-rw-r--r--   0 wry        (501) staff       (20)       54 2023-07-08 04:31:17.000000 python-postman-0.3.0/python_postman.egg-info/entry_points.txt
+-rw-r--r--   0 wry        (501) staff       (20)      116 2023-07-08 04:31:17.000000 python-postman-0.3.0/python_postman.egg-info/requires.txt
+-rw-r--r--   0 wry        (501) staff       (20)       10 2023-07-08 04:31:17.000000 python-postman-0.3.0/python_postman.egg-info/top_level.txt
+-rw-r--r--   0 wry        (501) staff       (20)       38 2023-07-08 04:31:17.330170 python-postman-0.3.0/setup.cfg
```

### Comparing `python-postman-0.2.0/LICENSE` & `python-postman-0.3.0/LICENSE`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2022 Yudiell
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2022 Yudiell
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `python-postman-0.2.0/PKG-INFO` & `python-postman-0.3.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,73 +1,73 @@
-Metadata-Version: 2.1
-Name: python-postman
-Version: 0.2.0
-Summary: Pypostman allows users to parse postman environments and postman collections.
-License: MIT
-Keywords: postman,python-postman,pypostman,api,requests
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-Provides-Extra: mypy
-Provides-Extra: black
-License-File: LICENSE
-
-# Python Postman
-
-**pypostman** is a command-line interface that allows to `automate` multiple api calls from postman collections, additionally it also allow you to `compress` and `save` the response to a local directory or to an AWS S3 bucket.
-Thereby allowing you to manage your api calls using postman, then `automate` and `process` their response using python.
-
-Example:
-
-```
-from pypostman.postman import Postman
-from pypostman.modules.http import Request
-
-postman = Postman()
-
-collections_dir = "../collections"
-collections = postman._get_collections(dir=collections_dir)
-pokeapi_collection = postman._get_collection(name="PokeAPI", collections=collections)
-pokeapi_requests = postman._get_requests(collection=pokeapi_collection)
-
-def pokemon(self, **kwargs):
-    # Make an API request.
-    # The request name should match the Postman request name.
-    name = "/pokemon"
-    pokemon = postman._get_request(name=name, requests=pokeapi_requests)
-    prepared_request: Request = Request(request=pokemon)
-    prepared_request.set_path_vars(kwargs)
-    prepared_request.set_params(kwargs)
-    response = prepared_request.send
-    return response
-```
-## What is Included?
-
-- The **pypostman** source code.
-- collections
-  - Coinmarketcap.postman_collection.json
-  - PokeAPI.postman_collection.json
-- models
-  - coinmarketcap_example.py
-  - pokeapi_example.py
-
-### Included Modules
-- file.py
-- http.py
-- logger.py
-
-## Installation
-
-### Python >= 3.8
-
-Pypi Test:
-  ```
-  pip install -i https://test.pypi.org/simple/ python-postman
-  ```
-Pypi (Not implemented Yet):
-  ```  
-  pip install python-postman
-  ```
-
-## How to Use It
-
-See examples.
+Metadata-Version: 2.1
+Name: python-postman
+Version: 0.3.0
+Summary: Pypostman allows users to parse postman environments and postman collections.
+License: MIT
+Keywords: postman,python-postman,pypostman,api,requests
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+Provides-Extra: mypy
+Provides-Extra: black
+License-File: LICENSE
+
+# Python Postman
+
+**pypostman** is a command-line interface that allows to `automate` multiple api calls from postman collections, additionally it also allow you to `compress` and `save` the response to a local directory or to an AWS S3 bucket.
+Thereby allowing you to manage your api calls using postman, then `automate` and `process` their response using python.
+
+Example:
+
+```
+from pypostman.postman import Postman
+from pypostman.modules.http import Request
+
+postman = Postman()
+
+collections_dir = "../collections"
+collections = postman._get_collections(dir=collections_dir)
+pokeapi_collection = postman._get_collection(name="PokeAPI", collections=collections)
+pokeapi_requests = postman._get_requests(collection=pokeapi_collection)
+
+def pokemon(self, **kwargs):
+    # Make an API request.
+    # The request name should match the Postman request name.
+    name = "/pokemon"
+    pokemon = postman._get_request(name=name, requests=pokeapi_requests)
+    prepared_request: Request = Request(request=pokemon)
+    prepared_request.set_path_vars(kwargs)
+    prepared_request.set_params(kwargs)
+    response = prepared_request.send
+    return response
+```
+## What is Included?
+
+- The **pypostman** source code.
+- collections
+  - Coinmarketcap.postman_collection.json
+  - PokeAPI.postman_collection.json
+- models
+  - coinmarketcap_example.py
+  - pokeapi_example.py
+
+### Included Modules
+- file.py
+- http.py
+- logger.py
+
+## Installation
+
+### Python >= 3.8
+
+Pypi Test:
+  ```
+  pip install -i https://test.pypi.org/simple/ python-postman
+  ```
+Pypi (Not implemented Yet):
+  ```  
+  pip install python-postman
+  ```
+
+## How to Use It
+
+See examples.
```

### Comparing `python-postman-0.2.0/README.md` & `python-postman-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `python-postman-0.2.0/examples/collections/PokeAPI.postman_collection.json` & `python-postman-0.3.0/examples/collections/PokeAPI.postman_collection.json`

 * *Format-specific differences are supported for JSON files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JSON text data*

 * *Files 22% similar despite different names*

```diff
@@ -1,72 +1,68 @@
-00000000: 7b0d 0a09 2269 6e66 6f22 3a20 7b0d 0a09  {..."info": {...
-00000010: 0922 5f70 6f73 746d 616e 5f69 6422 3a20  ."_postman_id": 
-00000020: 2261 3237 3732 3631 342d 3432 3964 2d34  "a2772614-429d-4
-00000030: 3730 372d 6238 6164 2d62 3837 6163 3837  707-b8ad-b87ac87
-00000040: 6664 3336 3522 2c0d 0a09 0922 6e61 6d65  fd365",...."name
-00000050: 223a 2022 506f 6b65 4150 4922 2c0d 0a09  ": "PokeAPI",...
-00000060: 0922 7363 6865 6d61 223a 2022 6874 7470  ."schema": "http
-00000070: 733a 2f2f 7363 6865 6d61 2e67 6574 706f  s://schema.getpo
-00000080: 7374 6d61 6e2e 636f 6d2f 6a73 6f6e 2f63  stman.com/json/c
-00000090: 6f6c 6c65 6374 696f 6e2f 7632 2e31 2e30  ollection/v2.1.0
-000000a0: 2f63 6f6c 6c65 6374 696f 6e2e 6a73 6f6e  /collection.json
-000000b0: 222c 0d0a 0909 225f 6578 706f 7274 6572  ",...."_exporter
-000000c0: 5f69 6422 3a20 2233 3030 3936 3533 220d  _id": "3009653".
-000000d0: 0a09 7d2c 0d0a 0922 6974 656d 223a 205b  ..},..."item": [
-000000e0: 0d0a 0909 7b0d 0a09 0909 226e 616d 6522  ....{....."name"
-000000f0: 3a20 222f 706f 6b65 6d6f 6e22 2c0d 0a09  : "/pokemon",...
-00000100: 0909 2272 6571 7565 7374 223a 207b 0d0a  .."request": {..
-00000110: 0909 0909 226d 6574 686f 6422 3a20 2247  ...."method": "G
-00000120: 4554 222c 0d0a 0909 0909 2268 6561 6465  ET",......"heade
-00000130: 7222 3a20 5b5d 2c0d 0a09 0909 0922 7572  r": [],......"ur
-00000140: 6c22 3a20 7b0d 0a09 0909 0909 2272 6177  l": {......."raw
-00000150: 223a 2022 7b7b 6261 7365 5f75 726c 7d7d  ": "{{base_url}}
-00000160: 2f70 6f6b 656d 6f6e 2f3a 6e61 6d65 5f6f  /pokemon/:name_o
-00000170: 725f 6964 222c 0d0a 0909 0909 0922 686f  r_id",......."ho
-00000180: 7374 223a 205b 0d0a 0909 0909 0909 227b  st": [........"{
-00000190: 7b62 6173 655f 7572 6c7d 7d22 0d0a 0909  {base_url}}"....
-000001a0: 0909 095d 2c0d 0a09 0909 0909 2270 6174  ...],......."pat
-000001b0: 6822 3a20 5b0d 0a09 0909 0909 0922 706f  h": [........"po
-000001c0: 6b65 6d6f 6e22 2c0d 0a09 0909 0909 0922  kemon",........"
-000001d0: 3a6e 616d 655f 6f72 5f69 6422 0d0a 0909  :name_or_id"....
-000001e0: 0909 095d 2c0d 0a09 0909 0909 2276 6172  ...],......."var
-000001f0: 6961 626c 6522 3a20 5b0d 0a09 0909 0909  iable": [.......
-00000200: 097b 0d0a 0909 0909 0909 0922 6b65 7922  .{........."key"
-00000210: 3a20 226e 616d 655f 6f72 5f69 6422 2c0d  : "name_or_id",.
-00000220: 0a09 0909 0909 0909 2276 616c 7565 223a  ........"value":
-00000230: 2022 7069 6b61 6368 7522 0d0a 0909 0909   "pikachu"......
-00000240: 0909 7d0d 0a09 0909 0909 5d0d 0a09 0909  ..}.......].....
-00000250: 097d 0d0a 0909 097d 2c0d 0a09 0909 2272  .}.....},....."r
-00000260: 6573 706f 6e73 6522 3a20 5b5d 0d0a 0909  esponse": []....
-00000270: 7d0d 0a09 5d2c 0d0a 0922 6576 656e 7422  }...],..."event"
-00000280: 3a20 5b0d 0a09 097b 0d0a 0909 0922 6c69  : [....{....."li
-00000290: 7374 656e 223a 2022 7072 6572 6571 7565  sten": "prereque
-000002a0: 7374 222c 0d0a 0909 0922 7363 7269 7074  st",....."script
-000002b0: 223a 207b 0d0a 0909 0909 2274 7970 6522  ": {......"type"
-000002c0: 3a20 2274 6578 742f 6a61 7661 7363 7269  : "text/javascri
-000002d0: 7074 222c 0d0a 0909 0909 2265 7865 6322  pt",......"exec"
-000002e0: 3a20 5b0d 0a09 0909 0909 2222 0d0a 0909  : [.......""....
-000002f0: 0909 5d0d 0a09 0909 7d0d 0a09 097d 2c0d  ..].....}....},.
-00000300: 0a09 097b 0d0a 0909 0922 6c69 7374 656e  ...{....."listen
-00000310: 223a 2022 7465 7374 222c 0d0a 0909 0922  ": "test",....."
-00000320: 7363 7269 7074 223a 207b 0d0a 0909 0909  script": {......
-00000330: 2274 7970 6522 3a20 2274 6578 742f 6a61  "type": "text/ja
-00000340: 7661 7363 7269 7074 222c 0d0a 0909 0909  vascript",......
-00000350: 2265 7865 6322 3a20 5b0d 0a09 0909 0909  "exec": [.......
-00000360: 2222 0d0a 0909 0909 5d0d 0a09 0909 7d0d  ""......].....}.
-00000370: 0a09 097d 0d0a 095d 2c0d 0a09 2276 6172  ...}...],..."var
-00000380: 6961 626c 6522 3a20 5b0d 0a09 097b 0d0a  iable": [....{..
-00000390: 0909 0922 6b65 7922 3a20 2262 6173 655f  ..."key": "base_
-000003a0: 7572 6c22 2c0d 0a09 0909 2276 616c 7565  url",....."value
-000003b0: 223a 2022 6874 7470 733a 2f2f 706f 6b65  ": "https://poke
-000003c0: 6170 692e 636f 2f61 7069 2f76 3222 2c0d  api.co/api/v2",.
-000003d0: 0a09 0909 2274 7970 6522 3a20 2273 7472  ...."type": "str
-000003e0: 696e 6722 0d0a 0909 7d2c 0d0a 0909 7b0d  ing"....},....{.
-000003f0: 0a09 0909 226b 6579 223a 2022 7333 5f70  ...."key": "s3_p
-00000400: 7265 6669 7822 2c0d 0a09 0909 2276 616c  refix",....."val
-00000410: 7565 223a 2022 7b7b 454e 567d 7d2f 6275  ue": "{{ENV}}/bu
-00000420: 7369 6e65 7373 5f73 7973 7465 6d73 2f70  siness_systems/p
-00000430: 6f6b 6561 7069 2f70 6f6b 656d 6f6e 2f73  okeapi/pokemon/s
-00000440: 6e61 7073 686f 7473 2f7b 7b44 4154 455f  napshots/{{DATE_
-00000450: 5041 5254 4954 494f 4e7d 7d22 2c0d 0a09  PARTITION}}",...
-00000460: 0909 2274 7970 6522 3a20 2273 7472 696e  .."type": "strin
-00000470: 6722 0d0a 0909 7d0d 0a09 5d0d 0a7d       g"....}...]..}
+00000000: 7b0a 0922 696e 666f 223a 207b 0a09 0922  {.."info": {..."
+00000010: 5f70 6f73 746d 616e 5f69 6422 3a20 2261  _postman_id": "a
+00000020: 3237 3732 3631 342d 3432 3964 2d34 3730  2772614-429d-470
+00000030: 372d 6238 6164 2d62 3837 6163 3837 6664  7-b8ad-b87ac87fd
+00000040: 3336 3522 2c0a 0909 226e 616d 6522 3a20  365",..."name": 
+00000050: 2250 6f6b 6541 5049 222c 0a09 0922 7363  "PokeAPI",..."sc
+00000060: 6865 6d61 223a 2022 6874 7470 733a 2f2f  hema": "https://
+00000070: 7363 6865 6d61 2e67 6574 706f 7374 6d61  schema.getpostma
+00000080: 6e2e 636f 6d2f 6a73 6f6e 2f63 6f6c 6c65  n.com/json/colle
+00000090: 6374 696f 6e2f 7632 2e31 2e30 2f63 6f6c  ction/v2.1.0/col
+000000a0: 6c65 6374 696f 6e2e 6a73 6f6e 222c 0a09  lection.json",..
+000000b0: 0922 5f65 7870 6f72 7465 725f 6964 223a  ."_exporter_id":
+000000c0: 2022 3330 3039 3635 3322 0a09 7d2c 0a09   "3009653"..},..
+000000d0: 2269 7465 6d22 3a20 5b0a 0909 7b0a 0909  "item": [...{...
+000000e0: 0922 6e61 6d65 223a 2022 2f70 6f6b 656d  ."name": "/pokem
+000000f0: 6f6e 222c 0a09 0909 2272 6571 7565 7374  on",...."request
+00000100: 223a 207b 0a09 0909 0922 6d65 7468 6f64  ": {....."method
+00000110: 223a 2022 4745 5422 2c0a 0909 0909 2268  ": "GET",....."h
+00000120: 6561 6465 7222 3a20 5b5d 2c0a 0909 0909  eader": [],.....
+00000130: 2275 726c 223a 207b 0a09 0909 0909 2272  "url": {......"r
+00000140: 6177 223a 2022 7b7b 6261 7365 5f75 726c  aw": "{{base_url
+00000150: 7d7d 2f70 6f6b 656d 6f6e 2f3a 6e61 6d65  }}/pokemon/:name
+00000160: 5f6f 725f 6964 222c 0a09 0909 0909 2268  _or_id",......"h
+00000170: 6f73 7422 3a20 5b0a 0909 0909 0909 227b  ost": [......."{
+00000180: 7b62 6173 655f 7572 6c7d 7d22 0a09 0909  {base_url}}"....
+00000190: 0909 5d2c 0a09 0909 0909 2270 6174 6822  ..],......"path"
+000001a0: 3a20 5b0a 0909 0909 0909 2270 6f6b 656d  : [......."pokem
+000001b0: 6f6e 222c 0a09 0909 0909 0922 3a6e 616d  on",.......":nam
+000001c0: 655f 6f72 5f69 6422 0a09 0909 0909 5d2c  e_or_id"......],
+000001d0: 0a09 0909 0909 2276 6172 6961 626c 6522  ......"variable"
+000001e0: 3a20 5b0a 0909 0909 0909 7b0a 0909 0909  : [.......{.....
+000001f0: 0909 0922 6b65 7922 3a20 226e 616d 655f  ..."key": "name_
+00000200: 6f72 5f69 6422 2c0a 0909 0909 0909 0922  or_id",........"
+00000210: 7661 6c75 6522 3a20 2270 696b 6163 6875  value": "pikachu
+00000220: 220a 0909 0909 0909 7d0a 0909 0909 095d  ".......}......]
+00000230: 0a09 0909 097d 0a09 0909 7d2c 0a09 0909  .....}....},....
+00000240: 2272 6573 706f 6e73 6522 3a20 5b5d 0a09  "response": []..
+00000250: 097d 0a09 5d2c 0a09 2265 7665 6e74 223a  .}..],.."event":
+00000260: 205b 0a09 097b 0a09 0909 226c 6973 7465   [...{...."liste
+00000270: 6e22 3a20 2270 7265 7265 7175 6573 7422  n": "prerequest"
+00000280: 2c0a 0909 0922 7363 7269 7074 223a 207b  ,...."script": {
+00000290: 0a09 0909 0922 7479 7065 223a 2022 7465  ....."type": "te
+000002a0: 7874 2f6a 6176 6173 6372 6970 7422 2c0a  xt/javascript",.
+000002b0: 0909 0909 2265 7865 6322 3a20 5b0a 0909  ...."exec": [...
+000002c0: 0909 0922 220a 0909 0909 5d0a 0909 097d  ..."".....]....}
+000002d0: 0a09 097d 2c0a 0909 7b0a 0909 0922 6c69  ...},...{...."li
+000002e0: 7374 656e 223a 2022 7465 7374 222c 0a09  sten": "test",..
+000002f0: 0909 2273 6372 6970 7422 3a20 7b0a 0909  .."script": {...
+00000300: 0909 2274 7970 6522 3a20 2274 6578 742f  .."type": "text/
+00000310: 6a61 7661 7363 7269 7074 222c 0a09 0909  javascript",....
+00000320: 0922 6578 6563 223a 205b 0a09 0909 0909  ."exec": [......
+00000330: 2222 0a09 0909 095d 0a09 0909 7d0a 0909  "".....]....}...
+00000340: 7d0a 095d 2c0a 0922 7661 7269 6162 6c65  }..],.."variable
+00000350: 223a 205b 0a09 097b 0a09 0909 226b 6579  ": [...{...."key
+00000360: 223a 2022 6261 7365 5f75 726c 222c 0a09  ": "base_url",..
+00000370: 0909 2276 616c 7565 223a 2022 6874 7470  .."value": "http
+00000380: 733a 2f2f 706f 6b65 6170 692e 636f 2f61  s://pokeapi.co/a
+00000390: 7069 2f76 3222 2c0a 0909 0922 7479 7065  pi/v2",...."type
+000003a0: 223a 2022 7374 7269 6e67 220a 0909 7d2c  ": "string"...},
+000003b0: 0a09 097b 0a09 0909 226b 6579 223a 2022  ...{...."key": "
+000003c0: 7333 5f70 7265 6669 7822 2c0a 0909 0922  s3_prefix",...."
+000003d0: 7661 6c75 6522 3a20 227b 7b45 4e56 7d7d  value": "{{ENV}}
+000003e0: 2f62 7573 696e 6573 735f 7379 7374 656d  /business_system
+000003f0: 732f 706f 6b65 6170 692f 706f 6b65 6d6f  s/pokeapi/pokemo
+00000400: 6e2f 736e 6170 7368 6f74 732f 7b7b 4441  n/snapshots/{{DA
+00000410: 5445 5f50 4152 5449 5449 4f4e 7d7d 222c  TE_PARTITION}}",
+00000420: 0a09 0909 2274 7970 6522 3a20 2273 7472  ...."type": "str
+00000430: 696e 6722 0a09 097d 0a09 5d0a 7d         ing"...}..].}
```

### Comparing `python-postman-0.2.0/examples/models/coinmarketcap_example.py` & `python-postman-0.3.0/python_postman.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,61 +1,73 @@
-import pendulum
-import uuid
-
-from pypostman.postman import Postman
-from pypostman.modules.http import Request
-from pypostman.modules.file import File
-from pypostman.utils.cli import Cli
-from pypostman.modules.logger import Log
-
-postman = Postman()
-cli = Cli()
-log = Log()
-ARGS = cli.parse_arguments()
-
-# Postman collection and rerquest names should be used.
-# Use a .env file for Auth.
-
-collections_dir = "../collections"
-collections = postman._get_collections(dir=collections_dir)
-coinmarketcap_collection = postman._get_collection(
-    name="Coinmarketcap", collections=collections
-)
-coinmarketcap_requests = postman._get_requests(collection=coinmarketcap_collection)
-
-
-class Coinmarketcap:
-    ## NOTE: This api requires an API key added to the .env file.
-    def __init__(self) -> None:
-        self.env = ARGS.environment
-        self.bucket = "bucket_name"
-        self.s3_prefix = coinmarketcap_collection._variables.s3_prefix(env=self.env)
-
-    def listings(self, **kwargs):
-        # Make an API request.
-        # The request name should match the Postman request name.
-        name = "/listings/latest"
-        listings = postman._get_request(name=name, requests=coinmarketcap_requests)
-        prepared_request: Request = Request(request=listings)
-        prepared_request.set_path_vars(kwargs)
-        prepared_request.set_params(kwargs)
-        response = prepared_request.send
-
-        # Do something with the response(es)
-        file: File = File()
-        content_type = response.headers.get("Content-Type")
-        file_ext = file.get_file_extension(content_type=content_type)
-        filename = f"{uuid.uuid4().hex[:6].upper()}{file_ext}"
-        source: str = file.write(payload=response, filename=filename)
-        compressed: str = file.compress(source)
-
-        # Do something with the file(s)
-        # S3 authentication required
-        file_timestamp = pendulum.now("UTC")
-        key = f"{self.s3_prefix}/{filename}.gz|{file_timestamp}"
-        file.s3_upload(filepath=compressed, bucket=self.bucket, key=key)
-        log.info(f"Completed Process: {name} \n")
-
-
-if __name__ == "__main__":
-    coinmarketcap = Coinmarketcap()
-    coinmarketcap.listings(circulating_supply_max=1000000000, limit=10, price_max=1)
+Metadata-Version: 2.1
+Name: python-postman
+Version: 0.3.0
+Summary: Pypostman allows users to parse postman environments and postman collections.
+License: MIT
+Keywords: postman,python-postman,pypostman,api,requests
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+Provides-Extra: mypy
+Provides-Extra: black
+License-File: LICENSE
+
+# Python Postman
+
+**pypostman** is a command-line interface that allows to `automate` multiple api calls from postman collections, additionally it also allow you to `compress` and `save` the response to a local directory or to an AWS S3 bucket.
+Thereby allowing you to manage your api calls using postman, then `automate` and `process` their response using python.
+
+Example:
+
+```
+from pypostman.postman import Postman
+from pypostman.modules.http import Request
+
+postman = Postman()
+
+collections_dir = "../collections"
+collections = postman._get_collections(dir=collections_dir)
+pokeapi_collection = postman._get_collection(name="PokeAPI", collections=collections)
+pokeapi_requests = postman._get_requests(collection=pokeapi_collection)
+
+def pokemon(self, **kwargs):
+    # Make an API request.
+    # The request name should match the Postman request name.
+    name = "/pokemon"
+    pokemon = postman._get_request(name=name, requests=pokeapi_requests)
+    prepared_request: Request = Request(request=pokemon)
+    prepared_request.set_path_vars(kwargs)
+    prepared_request.set_params(kwargs)
+    response = prepared_request.send
+    return response
+```
+## What is Included?
+
+- The **pypostman** source code.
+- collections
+  - Coinmarketcap.postman_collection.json
+  - PokeAPI.postman_collection.json
+- models
+  - coinmarketcap_example.py
+  - pokeapi_example.py
+
+### Included Modules
+- file.py
+- http.py
+- logger.py
+
+## Installation
+
+### Python >= 3.8
+
+Pypi Test:
+  ```
+  pip install -i https://test.pypi.org/simple/ python-postman
+  ```
+Pypi (Not implemented Yet):
+  ```  
+  pip install python-postman
+  ```
+
+## How to Use It
+
+See examples.
```

### Comparing `python-postman-0.2.0/examples/models/pokeapi_example.py` & `python-postman-0.3.0/examples/models/pokeapi_example.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,66 +1,66 @@
-import pendulum
-import uuid
-from concurrent.futures import ProcessPoolExecutor, as_completed
-
-from pypostman.postman import Postman
-from pypostman.modules.http import Request
-from pypostman.modules.file import File
-from pypostman.utils.cli import Cli
-from pypostman.modules.logger import Log
-
-postman = Postman()
-cli = Cli()
-log = Log()
-ARGS = cli.parse_arguments()
-
-# Postman collection and rerquest names should be used.
-# Use a .env file for Auth.
-
-collections_dir = "../collections"
-collections = postman._get_collections(dir=collections_dir)
-pokeapi_collection = postman._get_collection(name="PokeAPI", collections=collections)
-pokeapi_requests = postman._get_requests(collection=pokeapi_collection)
-
-
-class PokeAPI:
-    def __init__(self) -> None:
-        self.env = ARGS.environment
-        self.bucket = "bucket_name"
-        self.s3_prefix = pokeapi_collection._variables.s3_prefix(env=self.env)
-
-    def pokemon(self, **kwargs):
-        # Make an API request.
-        # The request name should match the Postman request name.
-        name = "/pokemon"
-        pokemon = postman._get_request(name=name, requests=pokeapi_requests)
-        prepared_request: Request = Request(request=pokemon)
-        prepared_request.set_path_vars(kwargs)
-        prepared_request.set_params(kwargs)
-        response = prepared_request.send
-
-        # Do something with the response(es)
-        file: File = File()
-        content_type = response.headers.get("Content-Type")
-        file_ext = file.get_file_extension(content_type=content_type)
-        filename = f"{uuid.uuid4().hex[:6].upper()}{file_ext}"
-        source: str = file.write(payload=response, filename=filename)
-        compressed: str = file.compress(source)
-
-        # Do something with the file(s)
-        # S3 authentication required
-        file_timestamp = pendulum.now("UTC")
-        key = f"{self.s3_prefix}/{filename}.gz|{file_timestamp}"
-        file.s3_upload(filepath=compressed, bucket=self.bucket, key=key)
-        log.info(f"Completed Process: {name} \n")
-
-
-if __name__ == "__main__":
-    pokeapi = PokeAPI()
-    # pokeapi.pokemon(name_or_id="pikachu")
-
-    pokemons = ["pikachu", "bayleef", "bulbasaur", "caterpie"]
-    with ProcessPoolExecutor(max_workers=4) as pool:
-        results = [
-            pool.submit(pokeapi.pokemon, name_or_id=pokemon) for pokemon in pokemons
-        ]
-        [print(result.result()) for result in as_completed(results)]
+import pendulum
+import uuid
+from concurrent.futures import ProcessPoolExecutor, as_completed
+
+from pypostman.postman import Postman
+from pypostman.modules.http import Request
+from pypostman.modules.file import File
+from pypostman.utils.cli import Cli
+from pypostman.modules.logger import Log
+
+postman = Postman()
+cli = Cli()
+log = Log()
+ARGS = cli.parse_arguments()
+
+# Postman collection and rerquest names should be used.
+# Use a .env file for Auth.
+
+collections_dir = "../collections"
+collections = postman._get_collections(dir=collections_dir)
+pokeapi_collection = postman._get_collection(name="PokeAPI", collections=collections)
+pokeapi_requests = postman._get_requests(collection=pokeapi_collection)
+
+
+class PokeAPI:
+    def __init__(self) -> None:
+        self.env = ARGS.environment
+        self.bucket = "bucket_name"
+        self.s3_prefix = pokeapi_collection._variables.s3_prefix(env=self.env)
+
+    def pokemon(self, **kwargs):
+        # Make an API request.
+        # The request name should match the Postman request name.
+        name = "/pokemon"
+        pokemon = postman._get_request(name=name, requests=pokeapi_requests)
+        prepared_request: Request = Request(request=pokemon)
+        prepared_request.set_path_vars(kwargs)
+        prepared_request.set_params(kwargs)
+        response = prepared_request.send
+
+        # Do something with the response(es)
+        file: File = File()
+        content_type = response.headers.get("Content-Type")
+        file_ext = file.get_file_extension(content_type=content_type)
+        filename = f"{uuid.uuid4().hex[:6].upper()}{file_ext}"
+        source: str = file.write(payload=response, filename=filename)
+        compressed: str = file.compress(source)
+
+        # Do something with the file(s)
+        # S3 authentication required
+        file_timestamp = pendulum.now("UTC")
+        key = f"{self.s3_prefix}/{filename}.gz|{file_timestamp}"
+        file.s3_upload(filepath=compressed, bucket=self.bucket, key=key)
+        log.info(f"Completed Process: {name} \n")
+
+
+if __name__ == "__main__":
+    pokeapi = PokeAPI()
+    # pokeapi.pokemon(name_or_id="pikachu")
+
+    pokemons = ["pikachu", "bayleef", "bulbasaur", "caterpie"]
+    with ProcessPoolExecutor(max_workers=4) as pool:
+        results = [
+            pool.submit(pokeapi.pokemon, name_or_id=pokemon) for pokemon in pokemons
+        ]
+        [print(result.result()) for result in as_completed(results)]
```

### Comparing `python-postman-0.2.0/pypostman/auth.py` & `python-postman-0.3.0/pypostman/auth.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,77 +1,77 @@
-from requests.auth import HTTPBasicAuth, AuthBase
-
-from .config import Auth as ConfigAuth
-
-
-class BearerAuth(AuthBase):
-    def __init__(self, token):
-        self.token = token
-
-    def __call__(self, r):
-        r.headers["Authorization"] = f"Bearer {self.token}"
-        return r
-
-
-class ApiKeyAuth(AuthBase):
-    def __init__(self, apikey):
-        self.apikey = apikey
-
-    def __call__(self, r):
-        """
-        The postman collection auth determines
-        where the apikey should be applied.
-        1. Query: Is to be added to the query params.
-        2. Header: Is to be added to the header.
-        The postman collection auth apikey is to be applied to -
-        the query params if the auth api key contains the key "in".
-        """
-        key = self.apikey["key"]
-        value = self.apikey["value"]
-        if self.apikey.get("in") is not None:
-            r.prepare_url(url=r.url, params={key: value})
-        else:
-            r.headers[key] = value
-        return r
-
-
-class Auth:
-    def __init__(self, auth: ConfigAuth):
-        self.type = auth.type if auth else None
-        self.__auth_config = (
-            auth.noauth or auth.basic or auth.apikey or auth.bearer if auth else None
-        )
-
-        self.http_auth = (
-            self.noauth or self.basic or self.apikey or self.bearer if auth else None
-        )
-
-    @property
-    def noauth(self) -> None:
-        if self.__auth_config and self.type == "noauth":
-            return None
-
-    @property
-    def basic(self) -> HTTPBasicAuth:
-        if self.__auth_config and self.type == "basic":
-            basic = {}
-            for item in self.__auth_config:
-                basic[item.key] = item.value
-            # print(basic)
-            return HTTPBasicAuth(username=basic["username"], password=basic["password"])
-
-    @property
-    def apikey(self) -> ApiKeyAuth:
-        if self.__auth_config and self.type == "apikey":
-            apikey = {}
-            for item in self.__auth_config:
-                apikey[item.key] = item.value
-            return ApiKeyAuth(apikey=apikey)
-
-    @property
-    def bearer(self) -> BearerAuth:
-        if self.__auth_config and self.type == "bearer":
-            bearer = {}
-            for item in self.__auth_config:
-                bearer[item.key] = item.value
-            # print(bearer)
-            return BearerAuth(token=bearer["token"])
+from requests.auth import HTTPBasicAuth, AuthBase
+
+from .config import Auth as ConfigAuth
+
+
+class BearerAuth(AuthBase):
+    def __init__(self, token):
+        self.token = token
+
+    def __call__(self, r):
+        r.headers["Authorization"] = f"Bearer {self.token}"
+        return r
+
+
+class ApiKeyAuth(AuthBase):
+    def __init__(self, apikey):
+        self.apikey = apikey
+
+    def __call__(self, r):
+        """
+        The postman collection auth determines
+        where the apikey should be applied.
+        1. Query: Is to be added to the query params.
+        2. Header: Is to be added to the header.
+        The postman collection auth apikey is to be applied to -
+        the query params if the auth api key contains the key "in".
+        """
+        key = self.apikey["key"]
+        value = self.apikey["value"]
+        if self.apikey.get("in") is not None:
+            r.prepare_url(url=r.url, params={key: value})
+        else:
+            r.headers[key] = value
+        return r
+
+
+class Auth:
+    def __init__(self, auth: ConfigAuth):
+        self.type = auth.type if auth else None
+        self.__auth_config = (
+            auth.noauth or auth.basic or auth.apikey or auth.bearer if auth else None
+        )
+
+        self.http_auth = (
+            self.noauth or self.basic or self.apikey or self.bearer if auth else None
+        )
+
+    @property
+    def noauth(self) -> None:
+        if self.__auth_config and self.type == "noauth":
+            return None
+
+    @property
+    def basic(self) -> HTTPBasicAuth:
+        if self.__auth_config and self.type == "basic":
+            basic = {}
+            for item in self.__auth_config:
+                basic[item.key] = item.value
+            # print(basic)
+            return HTTPBasicAuth(username=basic["username"], password=basic["password"])
+
+    @property
+    def apikey(self) -> ApiKeyAuth:
+        if self.__auth_config and self.type == "apikey":
+            apikey = {}
+            for item in self.__auth_config:
+                apikey[item.key] = item.value
+            return ApiKeyAuth(apikey=apikey)
+
+    @property
+    def bearer(self) -> BearerAuth:
+        if self.__auth_config and self.type == "bearer":
+            bearer = {}
+            for item in self.__auth_config:
+                bearer[item.key] = item.value
+            # print(bearer)
+            return BearerAuth(token=bearer["token"])
```

### Comparing `python-postman-0.2.0/pypostman/collection.py` & `python-postman-0.3.0/pypostman/collection.py`

 * *Ordering differences only*

 * *Files 8% similar despite different names*

```diff
@@ -1,36 +1,36 @@
-import os
-import json
-from pathlib import Path
-
-from .config import Config
-from .variable import Variables
-from .auth import Auth
-from .event import Events
-from .item import Items
-from .template import CustomTemplate
-
-
-class Collection:
-    def __init__(self, collection_file) -> None:
-        with open(Path(collection_file)) as file:
-            text = file.read().replace("{{", "${").replace("}}", "}")
-            template: str = CustomTemplate(text).safe_substitute(os.environ)
-            data: dict = json.loads(template)
-
-        self._template = template
-        self._collection = Config(**data)
-        self._info = self._collection.info
-        self._variables: Variables = Variables(variables=self._collection.variables)
-        self._auth: Auth = Auth(auth=self._collection.auth)
-        self._events = Events(events=self._collection.events)
-        self._test = self._events.test
-        self._prerequest = self._events.prerequest
-        self._items: Items = Items(items=self._collection.items)
-        self._requests = self._items.requests()
-        for request in self._requests:
-            request.auth = self._auth if not request.auth else request.auth
-            if request.url:
-                template: str = CustomTemplate(request.url.base).safe_substitute(
-                    self._variables.as_dict
-                )
-                request.url.base_url = template
+import os
+import json
+from pathlib import Path
+
+from .config import Config
+from .variable import Variables
+from .auth import Auth
+from .event import Events
+from .item import Items
+from .template import CustomTemplate
+
+
+class Collection:
+    def __init__(self, collection_file) -> None:
+        with open(Path(collection_file)) as file:
+            text = file.read().replace("{{", "${").replace("}}", "}")
+            template: str = CustomTemplate(text).safe_substitute(os.environ)
+            data: dict = json.loads(template)
+
+        self._template = template
+        self._collection = Config(**data)
+        self._info = self._collection.info
+        self._variables: Variables = Variables(variables=self._collection.variables)
+        self._auth: Auth = Auth(auth=self._collection.auth)
+        self._events = Events(events=self._collection.events)
+        self._test = self._events.test
+        self._prerequest = self._events.prerequest
+        self._items: Items = Items(items=self._collection.items)
+        self._requests = self._items.requests()
+        for request in self._requests:
+            request.auth = self._auth if not request.auth else request.auth
+            if request.url:
+                template: str = CustomTemplate(request.url.base).safe_substitute(
+                    self._variables.as_dict
+                )
+                request.url.base_url = template
```

### Comparing `python-postman-0.2.0/pypostman/environment.py` & `python-postman-0.3.0/pypostman/environment.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,101 +1,101 @@
-import os
-import json
-from typing import List, Optional, Dict
-from pydantic import Field, BaseModel
-from pathlib import Path
-
-from .template import CustomTemplate
-
-
-class Variable(BaseModel):
-    key: str
-    value: str
-    type: Optional[str]
-    enabled: bool
-
-
-class Environment(BaseModel):
-    """
-    Examples
-
-    # Load Environment
-    environment: Environment = Environment.load("environment.json")
-
-    # Access Properties
-    print(environment.id)  # Environment Id
-    print(environment.name)  # Environment Name
-    print(environment.variables[0].key)  # First Variable Key
-
-    # As Dictionary
-    variables_as_dict: dict = environment.variables_as_dict
-    print(variables_as_dict)  # {'key': 'value'}
-    """
-
-    id: str
-    name: str
-    postman_variable_scope: str = Field(None, alias="_postman_variable_scope")
-    postman_exported_at: str = Field(None, alias="_postman_exported_at")
-    postman_exported_using: str = Field(None, alias="_postman_exported_using")
-    variables: List[Variable] = Field(None, alias="values")
-
-    def load(environment_file: str) -> "Environment":
-        """
-        Loads a Postman environment.json file.
-        Replaces the postman {{var}} with a python ${var} ready for use with -
-        string template.
-        Replaces ${VAR} with os environment variables. The os env variables must match the ${VAR} name.
-        Unpacs the environment json to an Environment.
-        Returns an Environment Object.
-        """
-        assert (
-            ".postman_environment.json" in environment_file
-        ), f"File Error: {environment_file} - Please verify that you are using a postman_envrionment file."
-
-        def replace(json_data: str) -> str:
-            """
-            This function takes a string of JSON data and replaces the the variable value
-            with the variable key if the variable name is value -
-            if the variable is enabled otherwise if the variable is disabled
-            it will not be included in the return JSON data string.
-
-            This behaviour is similar to the behaviour implemented on the Postman Envrironments
-
-            Returns a JSON data string.
-            """
-            data: dict = json.loads(json_data)
-            for variable in data["values"]:
-                value = not variable["value"]
-                is_enabled = bool(variable["enabled"])
-
-                replace = all([value, is_enabled])
-
-                if replace:
-                    variable["value"] = f"""${{{variable["key"]}}}"""
-
-                elif not is_enabled:
-                    data["values"].remove(variable)
-
-            return json.dumps(data)
-
-        with open(Path(environment_file)) as file:
-            json_data: str = file.read().replace("{{", "${").replace("}}", "}")
-            text = replace(json_data=json_data)
-            template: CustomTemplate = CustomTemplate(text).safe_substitute(os.environ)
-            data: dict = json.loads(template)
-            environment = Environment(**data)
-
-            return environment
-
-    @property
-    def variables_as_dict(self) -> Dict[str, str]:
-        """
-        This property returns the environment as a -
-        python dictionary.
-        This dictionary is used when replacing the -
-        required parameters in the Postman Collection.
-        """
-        variables: List[Variable] = self.variables
-        variables_as_dict: dict = {}
-        for variable in variables:
-            variables_as_dict[variable.key] = variable.value
-        return variables_as_dict
+import os
+import json
+from typing import List, Optional, Dict
+from pydantic import Field, BaseModel
+from pathlib import Path
+
+from .template import CustomTemplate
+
+
+class Variable(BaseModel):
+    key: str
+    value: str
+    type: Optional[str]
+    enabled: bool
+
+
+class Environment(BaseModel):
+    """
+    Examples
+
+    # Load Environment
+    environment: Environment = Environment.load("environment.json")
+
+    # Access Properties
+    print(environment.id)  # Environment Id
+    print(environment.name)  # Environment Name
+    print(environment.variables[0].key)  # First Variable Key
+
+    # As Dictionary
+    variables_as_dict: dict = environment.variables_as_dict
+    print(variables_as_dict)  # {'key': 'value'}
+    """
+
+    id: str
+    name: str
+    postman_variable_scope: str = Field(None, alias="_postman_variable_scope")
+    postman_exported_at: str = Field(None, alias="_postman_exported_at")
+    postman_exported_using: str = Field(None, alias="_postman_exported_using")
+    variables: List[Variable] = Field(None, alias="values")
+
+    def load(environment_file: str) -> "Environment":
+        """
+        Loads a Postman environment.json file.
+        Replaces the postman {{var}} with a python ${var} ready for use with -
+        string template.
+        Replaces ${VAR} with os environment variables. The os env variables must match the ${VAR} name.
+        Unpacs the environment json to an Environment.
+        Returns an Environment Object.
+        """
+        assert (
+            ".postman_environment.json" in environment_file
+        ), f"File Error: {environment_file} - Please verify that you are using a postman_envrionment file."
+
+        def replace(json_data: str) -> str:
+            """
+            This function takes a string of JSON data and replaces the the variable value
+            with the variable key if the variable name is value -
+            if the variable is enabled otherwise if the variable is disabled
+            it will not be included in the return JSON data string.
+
+            This behaviour is similar to the behaviour implemented on the Postman Envrironments
+
+            Returns a JSON data string.
+            """
+            data: dict = json.loads(json_data)
+            for variable in data["values"]:
+                value = not variable["value"]
+                is_enabled = bool(variable["enabled"])
+
+                replace = all([value, is_enabled])
+
+                if replace:
+                    variable["value"] = f"""${{{variable["key"]}}}"""
+
+                elif not is_enabled:
+                    data["values"].remove(variable)
+
+            return json.dumps(data)
+
+        with open(Path(environment_file)) as file:
+            json_data: str = file.read().replace("{{", "${").replace("}}", "}")
+            text = replace(json_data=json_data)
+            template: CustomTemplate = CustomTemplate(text).safe_substitute(os.environ)
+            data: dict = json.loads(template)
+            environment = Environment(**data)
+
+            return environment
+
+    @property
+    def variables_as_dict(self) -> Dict[str, str]:
+        """
+        This property returns the environment as a -
+        python dictionary.
+        This dictionary is used when replacing the -
+        required parameters in the Postman Collection.
+        """
+        variables: List[Variable] = self.variables
+        variables_as_dict: dict = {}
+        for variable in variables:
+            variables_as_dict[variable.key] = variable.value
+        return variables_as_dict
```

### Comparing `python-postman-0.2.0/pypostman/modules/file.py` & `python-postman-0.3.0/pypostman/modules/file.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,203 +1,203 @@
-import os
-import platform
-import gzip
-import boto3
-import pytz
-import tempfile
-import glob
-
-from pathlib import PurePath
-from zipfile import ZipFile
-from typing import Iterator
-from datetime import datetime
-from .logger import Log
-
-
-class File:
-    def __init__(self) -> None:
-        self.log = Log()
-        self.tempdir = tempfile.TemporaryDirectory()
-        self.current_os = platform.system()
-
-    def unzip(self, file: str, path: str, extn: str) -> list:
-        """
-        param: file: str -> The file to be unzipped.
-        param: path: str -> The path where the unzipped file will be written to.
-        param: extn: str -> The unzipped file extension. Ex: csv, json
-
-        Returns a file(s) list that match the extn param.
-        """
-        self.log.info(f"Unzipping file: {file}")
-        with ZipFile(file=file, mode="r") as zipfile:
-            zipfile.extractall(path=path)
-            files = glob.glob(f"{path}/*.{extn}")
-            self.log.info(f"File(s) unzipped: {files}")
-            return files
-
-    def compress(self, file: str) -> str:
-        """
-        gzip the imput temp file.
-        returns the filename.
-        """
-        if self.current_os == "Windows":
-            with gzip.open(f"{file}.gz", "wb") as compressed:
-                chunks = self.read_file_in_chunks(file=file, n=10000)
-                for chunk in chunks:
-                    compressed.write(chunk)
-                self.log.info(f"{file} Compressed.")
-                return compressed.name
-        else:
-            self.log.info(f"Compressing file {file}...")
-            os.system(f"gzip {file}")
-            self.log.info(f"{file} compressed successfully.")
-            return f"{file}.gz"
-
-    def write(self, payload: Iterator, filename: str) -> str:
-        """
-        : param payload: Any response payload, csv, json, zip, gzip.
-        : param filename: Any preferred filename, ex. myFile.csv. (Will be written to a temporary)
-        Returns the temporary directory path + filename.
-        The temprary directory will be garbage collected if the File object is disposed or due to an exception.
-        """
-        tempfile = "".join([self.tempdir.name, "/", filename])
-        tempfile = PurePath(tempfile)
-        self.log.info(f"Writing to: {tempfile}...")
-        with open(file=tempfile, mode="wb") as file:
-            payload_size = 0
-            total_size = 0
-            for chunk in payload:
-                payload_size += payload.__sizeof__()
-                total_size += len(chunk)
-                file.write(chunk)
-        self.log.info(f"Write to file completed.")
-        return tempfile
-
-    def s3_upload(self, filepath: str, bucket: str, key: str) -> None:
-        """
-        Upload a file to S3.
-        :param filepath: The source file path.
-        :param bucket: The s3 target bucket name.
-        :param key: The s3 object name. (File name in s3, ex. /dev/business_unit/dataset/subdataset/daily/date/filename.json.gz)
-        """
-        self.log.info(f"Uploading file to S3...")
-        self.log.info(f"Source: {filepath}")
-        self.log.info(f"Target: {key}")
-        client = boto3.client("s3")
-        client.upload_file(Filename=filepath, Bucket=bucket, Key=key)
-        self.log.info(f"File uploaded successfully to: {key}")
-
-    def list_objects(self, bucket: str, prefix: str) -> list:
-        """
-        List objects from the bucket.
-        :param bucket: Name of the bucket
-        :type bucket: str
-        :param prefix: The key prefix
-        :type prefix: str
-        :return: Metadata for all objects from the bucket
-        :rtype: collections.Iterable[dict[str, any]]
-        """
-        client = boto3.client("s3")
-        # Use paginator abstraction to seamlessly iterate over pages.
-        # list_objects_v2 provides maximum 1000 objects per request, pagination
-        # is used in AWS sdk in order to split large collections into several
-        # smaller, limited requests)
-        paginator = client.get_paginator("list_objects_v2")
-        page = 1
-
-        for result in paginator.paginate(
-            Bucket=bucket, Prefix=prefix, RequestPayer="requester"
-        ):
-            self.log.info("\tReading page {}.".format(page))
-            page += 1
-
-            for item in result.get("Contents", []):
-                yield item
-
-    def s3_delete(
-        self, bucket: str, prefix: str, last_modified: datetime, max_count: int = 20
-    ) -> bool:
-        """
-        Delete a file from an S3 bucket
-        ***** Please verify that the prefix parameter is correct... Objects are permanetnly deleted. *****
-        :param bucket, Bucket to delete from
-        :param prefix, filter to be passed to the s3 bucket it selects the objects that match the prefix. Ex: dev/musket_systems/kpler/trades/cpp
-        :param last_modified, Select files oder than the timestamp passed.
-            The filter targets the s3 object's last modified date. Ex: last_modified = datetime.now() - timedelta(days=31).
-            Uses last_modified.replace(tzinfo=pytz.UTC)
-        :param max_count (not required, default = 20), pass a value if you need more than 20 objects deleted.
-        Returns True if objects were deleted, else False
-        Logs the s3 response.
-        """
-        # self.log.info('Deleting files from S3.')
-        last_modified = last_modified.replace(tzinfo=pytz.UTC)
-        self.log.info(f"Bucket: {bucket}")
-        self.log.info(f"Prefix: {prefix}")
-        self.log.info(f"Last modified: {last_modified}")
-        self.log.info(f"Max count: {max_count}")
-        # Deleted files
-        client = boto3.client("s3")
-        bucket = bucket
-
-        content = self.list_objects(bucket=bucket, prefix=prefix)
-
-        if content:
-            delete = {}
-            delete["Objects"] = [
-                {"Key": item["Key"]}
-                for item in content
-                if item["LastModified"] < last_modified
-            ]
-
-            delete_count = len(delete["Objects"])
-            if delete_count != 0:
-                assert delete_count <= max_count, self.log.error(
-                    f"""Delete count: {delete_count}\r\nThere are too many objects to delete, please verify that the prefix is correct. Max count = {max_count}
-                ----> Objects available for deletion [{delete_count}]."""
-                )
-                self.log.info(f"Deleting objects with prefix: {prefix}")
-                delete_response = client.delete_objects(Bucket=bucket, Delete=delete)
-                self.log.info(delete_response)
-                return True
-            else:
-                self.log.info(
-                    f"No objects met the last modified condition {last_modified}"
-                )
-                return False
-        else:
-            self.log.info(f"No objects met the prefix condition {prefix}")
-            return False
-
-    def get_file_extension(self, content_type: str) -> str:
-        """
-        This function takes in a content type as an argument and returns the corresponding file extension as a string.
-        If no corresponding file extension exists, it returns '.bin' as the file extension.
-        """
-        self.log.info(f"API response content type: {content_type}")
-        extensions = {
-            "image/jpeg": ".jpg",
-            "image/png": ".png",
-            "image/gif": ".gif",
-            "image/bmp": ".bmp",
-            "audio/mp3": ".mp3",
-            "audio/wav": ".wav",
-            "audio/aac": ".aac",
-            "video/mp4": ".mp4",
-            "video/avi": ".avi",
-            "video/mkv": ".mkv",
-            "text/html": ".html",
-            "text/plain": ".txt",
-            "text/javascript": ".js",
-            "application/pdf": ".pdf",
-            "application/json": ".json",
-            "application/xml": ".xml",
-            "application/csv": ".csv",
-            "application/x-zip-compressed": ".zip",
-        }
-        ext: str = None
-        for extension in extensions:
-            if extension in content_type:
-                ext = extensions[extension]
-
-        if ext:
-            return ext
-        return ".bin"
+import os
+import platform
+import gzip
+import boto3
+import pytz
+import tempfile
+import glob
+
+from pathlib import PurePath
+from zipfile import ZipFile
+from typing import Iterator
+from datetime import datetime
+from .logger import Log
+
+
+class File:
+    def __init__(self) -> None:
+        self.log = Log()
+        self.tempdir = tempfile.TemporaryDirectory()
+        self.current_os = platform.system()
+
+    def unzip(self, file: str, path: str, extn: str) -> list:
+        """
+        param: file: str -> The file to be unzipped.
+        param: path: str -> The path where the unzipped file will be written to.
+        param: extn: str -> The unzipped file extension. Ex: csv, json
+
+        Returns a file(s) list that match the extn param.
+        """
+        self.log.info(f"Unzipping file: {file}")
+        with ZipFile(file=file, mode="r") as zipfile:
+            zipfile.extractall(path=path)
+            files = glob.glob(f"{path}/*.{extn}")
+            self.log.info(f"File(s) unzipped: {files}")
+            return files
+
+    def compress(self, file: str) -> str:
+        """
+        gzip the imput temp file.
+        returns the filename.
+        """
+        if self.current_os == "Windows":
+            with gzip.open(f"{file}.gz", "wb") as compressed:
+                chunks = self.read_file_in_chunks(file=file, n=10000)
+                for chunk in chunks:
+                    compressed.write(chunk)
+                self.log.info(f"{file} Compressed.")
+                return compressed.name
+        else:
+            self.log.info(f"Compressing file {file}...")
+            os.system(f"gzip {file}")
+            self.log.info(f"{file} compressed successfully.")
+            return f"{file}.gz"
+
+    def write(self, payload: Iterator, filename: str) -> str:
+        """
+        : param payload: Any response payload, csv, json, zip, gzip.
+        : param filename: Any preferred filename, ex. myFile.csv. (Will be written to a temporary)
+        Returns the temporary directory path + filename.
+        The temprary directory will be garbage collected if the File object is disposed or due to an exception.
+        """
+        tempfile = "".join([self.tempdir.name, "/", filename])
+        tempfile = PurePath(tempfile)
+        self.log.info(f"Writing to: {tempfile}...")
+        with open(file=tempfile, mode="wb") as file:
+            payload_size = 0
+            total_size = 0
+            for chunk in payload:
+                payload_size += payload.__sizeof__()
+                total_size += len(chunk)
+                file.write(chunk)
+        self.log.info(f"Write to file completed.")
+        return tempfile
+
+    def s3_upload(self, filepath: str, bucket: str, key: str) -> None:
+        """
+        Upload a file to S3.
+        :param filepath: The source file path.
+        :param bucket: The s3 target bucket name.
+        :param key: The s3 object name. (File name in s3, ex. /dev/business_unit/dataset/subdataset/daily/date/filename.json.gz)
+        """
+        self.log.info(f"Uploading file to S3...")
+        self.log.info(f"Source: {filepath}")
+        self.log.info(f"Target: {key}")
+        client = boto3.client("s3")
+        client.upload_file(Filename=filepath, Bucket=bucket, Key=key)
+        self.log.info(f"File uploaded successfully to: {key}")
+
+    def list_objects(self, bucket: str, prefix: str) -> list:
+        """
+        List objects from the bucket.
+        :param bucket: Name of the bucket
+        :type bucket: str
+        :param prefix: The key prefix
+        :type prefix: str
+        :return: Metadata for all objects from the bucket
+        :rtype: collections.Iterable[dict[str, any]]
+        """
+        client = boto3.client("s3")
+        # Use paginator abstraction to seamlessly iterate over pages.
+        # list_objects_v2 provides maximum 1000 objects per request, pagination
+        # is used in AWS sdk in order to split large collections into several
+        # smaller, limited requests)
+        paginator = client.get_paginator("list_objects_v2")
+        page = 1
+
+        for result in paginator.paginate(
+            Bucket=bucket, Prefix=prefix, RequestPayer="requester"
+        ):
+            self.log.info("\tReading page {}.".format(page))
+            page += 1
+
+            for item in result.get("Contents", []):
+                yield item
+
+    def s3_delete(
+        self, bucket: str, prefix: str, last_modified: datetime, max_count: int = 20
+    ) -> bool:
+        """
+        Delete a file from an S3 bucket
+        ***** Please verify that the prefix parameter is correct... Objects are permanetnly deleted. *****
+        :param bucket, Bucket to delete from
+        :param prefix, filter to be passed to the s3 bucket it selects the objects that match the prefix. Ex: dev/system/prefix1/prefix2/prefix3
+        :param last_modified, Select files oder than the timestamp passed.
+            The filter targets the s3 object's last modified date. Ex: last_modified = datetime.now() - timedelta(days=31).
+            Uses last_modified.replace(tzinfo=pytz.UTC)
+        :param max_count (not required, default = 20), pass a value if you need more than 20 objects deleted.
+        Returns True if objects were deleted, else False
+        Logs the s3 response.
+        """
+        # self.log.info('Deleting files from S3.')
+        last_modified = last_modified.replace(tzinfo=pytz.UTC)
+        self.log.info(f"Bucket: {bucket}")
+        self.log.info(f"Prefix: {prefix}")
+        self.log.info(f"Last modified: {last_modified}")
+        self.log.info(f"Max count: {max_count}")
+        # Deleted files
+        client = boto3.client("s3")
+        bucket = bucket
+
+        content = self.list_objects(bucket=bucket, prefix=prefix)
+
+        if content:
+            delete = {}
+            delete["Objects"] = [
+                {"Key": item["Key"]}
+                for item in content
+                if item["LastModified"] < last_modified
+            ]
+
+            delete_count = len(delete["Objects"])
+            if delete_count != 0:
+                assert delete_count <= max_count, self.log.error(
+                    f"""Delete count: {delete_count}\r\nThere are too many objects to delete, please verify that the prefix is correct. Max count = {max_count}
+                ----> Objects available for deletion [{delete_count}]."""
+                )
+                self.log.info(f"Deleting objects with prefix: {prefix}")
+                delete_response = client.delete_objects(Bucket=bucket, Delete=delete)
+                self.log.info(delete_response)
+                return True
+            else:
+                self.log.info(
+                    f"No objects met the last modified condition {last_modified}"
+                )
+                return False
+        else:
+            self.log.info(f"No objects met the prefix condition {prefix}")
+            return False
+
+    def get_file_extension(self, content_type: str) -> str:
+        """
+        This function takes in a content type as an argument and returns the corresponding file extension as a string.
+        If no corresponding file extension exists, it returns '.bin' as the file extension.
+        """
+        self.log.info(f"API response content type: {content_type}")
+        extensions = {
+            "image/jpeg": ".jpg",
+            "image/png": ".png",
+            "image/gif": ".gif",
+            "image/bmp": ".bmp",
+            "audio/mp3": ".mp3",
+            "audio/wav": ".wav",
+            "audio/aac": ".aac",
+            "video/mp4": ".mp4",
+            "video/avi": ".avi",
+            "video/mkv": ".mkv",
+            "text/html": ".html",
+            "text/plain": ".txt",
+            "text/javascript": ".js",
+            "application/pdf": ".pdf",
+            "application/json": ".json",
+            "application/xml": ".xml",
+            "application/csv": ".csv",
+            "application/x-zip-compressed": ".zip",
+        }
+        ext: str = None
+        for extension in extensions:
+            if extension in content_type:
+                ext = extensions[extension]
+
+        if ext:
+            return ext
+        return ".bin"
```

### Comparing `python-postman-0.2.0/pypostman/modules/http.py` & `python-postman-0.3.0/pypostman/modules/http.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,126 +1,126 @@
-import os
-import json
-from requests import Session, Response
-from urllib3 import Timeout
-
-from ..request import Request as CollectionRequest
-from ..template import CustomTemplate
-from .logger import Log
-
-
-class Request(Session):
-    def __init__(
-        self,
-        request: CollectionRequest,
-        timeout: Timeout = Timeout(connect=15, read=60),
-        stream: bool = True,
-    ) -> None:
-        super().__init__()
-        self._request: CollectionRequest = request
-        self.log: Log = Log()
-        self.timeout: Timeout = timeout
-        self.stream: bool = stream
-        self.url: str = self._request.url.base_url
-
-    def set_params(self, params: dict):
-        """
-        Set URL parameters on the request object.
-
-        Args:
-            params (dict): Parameters to set on the request object.
-
-        Returns:
-            None
-        """
-        if self._request.url.params:
-            text = json.dumps(self._request.url.params)
-            template: str = CustomTemplate(text).safe_substitute(params)
-            params = {
-                key: value
-                for key, value in json.loads(template).items()
-                if "${" not in value
-            }
-            self.params = params
-
-    def set_headers(self, headers: dict):
-        """
-        Set the headers of the request.
-
-        Args:
-            headers (dict): The headers to set.
-
-        Returns:
-            None
-        """
-        if self._request.headers:
-            text = json.dumps(self._request.headers.as_dict)
-            template: str = CustomTemplate(text).safe_substitute(headers)
-            headers = {
-                key: value
-                for key, value in json.loads(template).items()
-                if "${" not in value
-            }
-            self.headers = headers
-
-    def set_path_vars(self, path_variables: dict):
-        """
-        This function sets the path variables for a given request.
-
-        Parameters:
-            path_variables (dict): The data to be substituted into the url template.
-
-        Returns:
-            None
-        """
-        if self._request.url.base_url:
-            request_url = self._request.url.base_url
-            path: str = CustomTemplate(request_url).safe_substitute(path_variables)
-            self.url = path
-
-    def substitute_bearer_token(self) -> None:
-        if self._request.auth and self._request.auth.type == "bearer":
-            self._request.auth.http_auth.token = CustomTemplate(
-                self._request.auth.http_auth.token
-            ).safe_substitute(os.environ)
-
-    @property
-    def send(self) -> Response:
-        log: Log = self.log
-        with Session() as session:
-            # Setting the requests
-            request: CollectionRequest = self._request
-            log.info(f"Request Name: {request.name}")
-
-            # Substitute the a bearer token at the API call level.
-            # This is a substitution for the postman "test" script that sets a bearer token.
-            self.substitute_bearer_token()
-
-            # Setting the request params
-            method = request.method
-            url = self.url
-            headers = self._request.headers.as_dict
-            params = self.params
-            data = request.body.raw if request.body else None
-            timeout = self.timeout
-            stream = self.stream
-            auth = request.auth.http_auth
-
-            self.log.request(url=url)
-
-            response = session.request(
-                auth=auth,
-                method=method,
-                url=url,
-                headers=headers,
-                params=params,
-                data=data,
-                stream=stream,
-                timeout=timeout,
-            )
-
-            if response.ok:
-                self.log.successful(url=url)
-            else:
-                self.log.raise_error(url=url, response=response)
-
-            return response
+import os
+import json
+from requests import Session, Response
+from urllib3 import Timeout
+
+from ..request import Request as CollectionRequest
+from ..template import CustomTemplate
+from .logger import Log
+
+
+class Request(Session):
+    def __init__(
+        self,
+        request: CollectionRequest,
+        timeout: Timeout = Timeout(connect=15, read=60),
+        stream: bool = True,
+    ) -> None:
+        super().__init__()
+        self._request: CollectionRequest = request
+        self.log: Log = Log()
+        self.timeout: Timeout = timeout
+        self.stream: bool = stream
+        self.url: str = self._request.url.base_url
+
+    def set_params(self, params: dict):
+        """
+        Set URL parameters on the request object.
+
+        Args:
+            params (dict): Parameters to set on the request object.
+
+        Returns:
+            None
+        """
+        if self._request.url.params:
+            text = json.dumps(self._request.url.params)
+            template: str = CustomTemplate(text).safe_substitute(params)
+            params = {
+                key: value
+                for key, value in json.loads(template).items()
+                if "${" not in value
+            }
+            self.params = params
+
+    def set_headers(self, headers: dict):
+        """
+        Set the headers of the request.
+
+        Args:
+            headers (dict): The headers to set.
+
+        Returns:
+            None
+        """
+        if self._request.headers:
+            text = json.dumps(self._request.headers.as_dict)
+            template: str = CustomTemplate(text).safe_substitute(headers)
+            headers = {
+                key: value
+                for key, value in json.loads(template).items()
+                if "${" not in value
+            }
+            self.headers = headers
+
+    def set_path_vars(self, path_variables: dict):
+        """
+        This function sets the path variables for a given request.
+
+        Parameters:
+            path_variables (dict): The data to be substituted into the url template.
+
+        Returns:
+            None
+        """
+        if self._request.url.base_url:
+            request_url = self._request.url.base_url
+            path: str = CustomTemplate(request_url).safe_substitute(path_variables)
+            self.url = path
+
+    def substitute_bearer_token(self) -> None:
+        if self._request.auth and self._request.auth.type == "bearer":
+            self._request.auth.http_auth.token = CustomTemplate(
+                self._request.auth.http_auth.token
+            ).safe_substitute(os.environ)
+
+    @property
+    def send(self) -> Response:
+        log: Log = self.log
+        with Session() as session:
+            # Setting the requests
+            request: CollectionRequest = self._request
+            log.info(f"Request Name: {request.name}")
+
+            # Substitute the a bearer token at the API call level.
+            # This is a substitution for the postman "test" script that sets a bearer token.
+            self.substitute_bearer_token()
+
+            # Setting the request params
+            method = request.method
+            url = self.url
+            headers = self._request.headers.as_dict
+            params = self.params
+            data = request.body.raw if request.body else None
+            timeout = self.timeout
+            stream = self.stream
+            auth = request.auth.http_auth
+
+            self.log.request(url=url)
+
+            response = session.request(
+                auth=auth,
+                method=method,
+                url=url,
+                headers=headers,
+                params=params,
+                data=data,
+                stream=stream,
+                timeout=timeout,
+            )
+
+            if response.ok:
+                self.log.successful(url=url)
+            else:
+                self.log.raise_error(url=url, response=response)
+
+            return response
```

### Comparing `python-postman-0.2.0/pypostman/postman.py` & `python-postman-0.3.0/pypostman/postman.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,143 +1,143 @@
-import glob
-from typing import List
-
-from .modules.logger import Log
-from .environment import Environment
-from .collection import Collection
-from .request import Request
-
-log = Log()
-
-
-class Postman:
-    def __init__(self) -> None:
-        pass
-
-    def get_postman_environment_files(self, dir: str) -> List[str]:
-        """
-        This function returns a list of all the postman environments in the given directory -
-        if the file name contains .postman_environment.json
-        """
-        environments = glob.glob(f"{dir}/*")
-        environments = [
-            environment
-            for environment in environments
-            if ".postman_environment.json" in environment
-        ]
-        return environments
-
-    def get_postman_collection_files(self, dir: str) -> List[str]:
-        """
-        This function returns a list of all the postman collections in the given directory -
-        if the file name contains .postman_collection.json
-        """
-        collections = glob.glob(f"{dir}/*")
-        collections = [
-            collection
-            for collection in collections
-            if ".postman_collection.json" in collection
-        ]
-        return collections
-
-    def _get_environments(self, dir: str) -> List[Environment]:
-        """
-        Retrieve a list of Postman environments from the given directory.
-
-        Args:
-            dir (str): The directory containing Postman environments.
-
-        Returns:
-            List[Environment]: List of Postman environments.
-        """
-        environment_files = self.get_postman_environment_files(dir=dir)
-        return [
-            Environment.load(environment_file=environment_file)
-            for environment_file in environment_files
-        ]
-
-    def _get_environment(
-        self, environments: List[Environment], name: str
-    ) -> Environment:
-
-        """
-        This function finds an Environment in a list of Environments based on its name and returns it.
-
-        Args:
-            environments (List[Environment]): List of Environment objects.
-            name (str): Name of the Environment to be found.
-
-        Returns:
-            Environment: Environment object with the same name as the argument.
-        """
-        for environment in environments:
-            if environment.name == name:
-                return environment
-
-    def _get_collections(self, dir: str) -> List[Collection]:
-        """
-        Gets the postman collection files in the given directory and returns a list of Collection objects.
-        If no collection files are found, an error is logged.
-
-        Parameters:
-            dir (str): The directory path to search for postman collection files
-
-        Returns:
-            List[Collection]: A list of Collection objects
-        """
-        collections_files = self.get_postman_collection_files(dir=dir)
-        if len(collections_files) > 0:
-            return [
-                Collection(collection_file=collection_file)
-                for collection_file in collections_files
-            ]
-        log.error(f'No collection files were found in path "{dir}"')
-
-    def _get_collection(self, name: str, collections: List[Collection]) -> Collection:
-        """
-        Gets the specified collection from the list of collections.
-
-        Args:
-            name (str): Name of the collection.
-            collections (List[Collection]): List of collections.
-
-        Returns:
-            Collection: The specified collection.
-
-        Raises:
-            error (Exception): No collection named "{name}" was found.
-        """
-        for collection in collections:
-            if collection._info.name == name:
-                return collection
-
-        log.error(f'No collection named "{name}" was found.')
-
-    def _get_requests(self, collection: Collection) -> List[Request]:
-        """
-        This function returns a list of requests from a given collection.
-
-        Args:
-            collection (Collection): The collection to get requests from.
-
-        Returns:
-            List[Request]: A list of requests from the collection.
-        """
-        requests = collection._requests
-        return requests
-
-    def _get_request(self, name: str, requests: List[Request]):
-        """
-        Get the request object from the list of requests.
-
-        Args:
-            name (str): The name of the request.
-            requests (List[Request]): The list of requests.
-
-        Returns:
-            Request: The request object.
-        """
-        for request in requests:
-            if request.name == name:
-                return request
-
-        log.error(f"The request {name} was not found. Please verify the request name.")
+import glob
+from typing import List
+
+from .modules.logger import Log
+from .environment import Environment
+from .collection import Collection
+from .request import Request
+
+log = Log()
+
+
+class Postman:
+    def __init__(self) -> None:
+        pass
+
+    def get_postman_environment_files(self, dir: str) -> List[str]:
+        """
+        This function returns a list of all the postman environments in the given directory -
+        if the file name contains .postman_environment.json
+        """
+        environments = glob.glob(f"{dir}/*")
+        environments = [
+            environment
+            for environment in environments
+            if ".postman_environment.json" in environment
+        ]
+        return environments
+
+    def get_postman_collection_files(self, dir: str) -> List[str]:
+        """
+        This function returns a list of all the postman collections in the given directory -
+        if the file name contains .postman_collection.json
+        """
+        collections = glob.glob(f"{dir}/*")
+        collections = [
+            collection
+            for collection in collections
+            if ".postman_collection.json" in collection
+        ]
+        return collections
+
+    def _get_environments(self, dir: str) -> List[Environment]:
+        """
+        Retrieve a list of Postman environments from the given directory.
+
+        Args:
+            dir (str): The directory containing Postman environments.
+
+        Returns:
+            List[Environment]: List of Postman environments.
+        """
+        environment_files = self.get_postman_environment_files(dir=dir)
+        return [
+            Environment.load(environment_file=environment_file)
+            for environment_file in environment_files
+        ]
+
+    def _get_environment(
+        self, environments: List[Environment], name: str
+    ) -> Environment:
+
+        """
+        This function finds an Environment in a list of Environments based on its name and returns it.
+
+        Args:
+            environments (List[Environment]): List of Environment objects.
+            name (str): Name of the Environment to be found.
+
+        Returns:
+            Environment: Environment object with the same name as the argument.
+        """
+        for environment in environments:
+            if environment.name == name:
+                return environment
+
+    def _get_collections(self, dir: str) -> List[Collection]:
+        """
+        Gets the postman collection files in the given directory and returns a list of Collection objects.
+        If no collection files are found, an error is logged.
+
+        Parameters:
+            dir (str): The directory path to search for postman collection files
+
+        Returns:
+            List[Collection]: A list of Collection objects
+        """
+        collections_files = self.get_postman_collection_files(dir=dir)
+        if len(collections_files) > 0:
+            return [
+                Collection(collection_file=collection_file)
+                for collection_file in collections_files
+            ]
+        log.error(f'No collection files were found in path "{dir}"')
+
+    def _get_collection(self, name: str, collections: List[Collection]) -> Collection:
+        """
+        Gets the specified collection from the list of collections.
+
+        Args:
+            name (str): Name of the collection.
+            collections (List[Collection]): List of collections.
+
+        Returns:
+            Collection: The specified collection.
+
+        Raises:
+            error (Exception): No collection named "{name}" was found.
+        """
+        for collection in collections:
+            if collection._info.name == name:
+                return collection
+
+        log.error(f'No collection named "{name}" was found.')
+
+    def _get_requests(self, collection: Collection) -> List[Request]:
+        """
+        This function returns a list of requests from a given collection.
+
+        Args:
+            collection (Collection): The collection to get requests from.
+
+        Returns:
+            List[Request]: A list of requests from the collection.
+        """
+        requests = collection._requests
+        return requests
+
+    def _get_request(self, name: str, requests: List[Request]):
+        """
+        Get the request object from the list of requests.
+
+        Args:
+            name (str): The name of the request.
+            requests (List[Request]): The list of requests.
+
+        Returns:
+            Request: The request object.
+        """
+        for request in requests:
+            if request.name == name:
+                return request
+
+        log.error(f"The request {name} was not found. Please verify the request name.")
```

### Comparing `python-postman-0.2.0/pypostman/request.py` & `python-postman-0.3.0/pypostman/request.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-from .config import Item
-from .header import Headers
-from .auth import Auth
-from .body import Body
-from .event import Events
-from .url import Url
-
-
-class Request:
-    def __init__(self, item: Item) -> None:
-        self.name: str = item.name
-        self.events: Events = Events(events=item.events) if item.events else None
-        self.method: str = item.request.method
-        self.auth: Auth = Auth(auth=item.request.auth) if item.request.auth else None
-        self.headers: Headers = Headers(headers=item.request.headers)
-        self.body: Body = Body(body=item.request.body) if item.request.body else None
-        self.url: Url = Url(url=item.request.url) if item.request.url else None
+from .config import Item
+from .header import Headers
+from .auth import Auth
+from .body import Body
+from .event import Events
+from .url import Url
+
+
+class Request:
+    def __init__(self, item: Item) -> None:
+        self.name: str = item.name
+        self.events: Events = Events(events=item.events) if item.events else None
+        self.method: str = item.request.method
+        self.auth: Auth = Auth(auth=item.request.auth) if item.request.auth else None
+        self.headers: Headers = Headers(headers=item.request.headers)
+        self.body: Body = Body(body=item.request.body) if item.request.body else None
+        self.url: Url = Url(url=item.request.url) if item.request.url else None
```

### Comparing `python-postman-0.2.0/pypostman/url.py` & `python-postman-0.3.0/pypostman/url.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,94 +1,94 @@
-from typing import Dict, List
-
-from .config import Url, Param, Variable
-
-
-class Variable:
-    def __init__(self, variable: Variable) -> None:
-        self.key: str = variable.key
-        self.value: str = variable.value
-        self.description: str = variable.description
-
-
-class Param:
-    def __init__(self, param: Param) -> None:
-        self.key: str = param.key
-        self.value: str = param.value
-        self.description: str = param.description
-        self.disabled: str = param.disabled
-
-
-class Url:
-    def __init__(self, url: Url) -> None:
-        self.raw: str = url.raw
-        self.protocol: str = url.protocol
-        self.host: str = url.host
-        self.path: str = url.path
-        self.variables: List[Variable] = url.variable
-        self.query: List[Param] = url.query
-        self.base_url: str = None
-
-    @property
-    def base(self) -> str:
-        """
-        This property returns a complete URL from the provided host and path.
-        If no protocol is given, it defaults to 'https://'.
-        Raises an AssertionError if no host or path are found in the postman collection.
-        """
-        assert self.host and self.path, print(
-            "Error: No host or path were found in the postman collection."
-        )
-        protocol = f"{self.protocol}" if self.protocol else "https://"
-        host = ".".join(self.host) + "/"
-        path = "/".join(self.update_path())
-        url = "".join([protocol, host, path])
-        url = "".join([host, path])
-        return url
-
-    @property
-    def params(self) -> Dict[str, str]:
-        """
-        A parameter is enabled/disabled in the Postman App.
-        Enabled parameters are parameters that do not contain a "disabled: true" key: value
-        returns a dictionary of enabled parameters.
-        """
-        if self.query:
-            params: Dict = {}
-            for param in self.query:
-                param = Param(param=param)
-                if not param.disabled:
-                    params[param.key] = param.value
-            return params
-
-    @property
-    def path_variables(self) -> Dict[str, str]:
-        """
-        A parameter is enabled/disabled in the Postman App.
-        Enabled parameters are parameters that do not contain a "disabled: true" key: value
-        returns a dictionary of enabled parameters.
-        """
-        if self.variables:
-            variables: Dict = {}
-            for variable in self.variables:
-                variable = Variable(variable=variable)
-                variables[variable.key] = variable.value
-            return variables
-
-    def update_path(self):
-        """
-        Update the path to replace each colon ":" with "${}"
-
-        Args:
-            self: The object itself
-
-        Returns:
-            path: The updated path
-        """
-        path = self.path
-        for i, element in enumerate(path):
-            if ":" in element:
-                element = element.replace(":", "${")
-                element = element + "}"
-                self.path[i] = element
-
-        return path
+from typing import Dict, List
+
+from .config import Url, Param, Variable
+
+
+class Variable:
+    def __init__(self, variable: Variable) -> None:
+        self.key: str = variable.key
+        self.value: str = variable.value
+        self.description: str = variable.description
+
+
+class Param:
+    def __init__(self, param: Param) -> None:
+        self.key: str = param.key
+        self.value: str = param.value
+        self.description: str = param.description
+        self.disabled: str = param.disabled
+
+
+class Url:
+    def __init__(self, url: Url) -> None:
+        self.raw: str = url.raw
+        self.protocol: str = url.protocol
+        self.host: str = url.host
+        self.path: str = url.path
+        self.variables: List[Variable] = url.variable
+        self.query: List[Param] = url.query
+        self.base_url: str = None
+
+    @property
+    def base(self) -> str:
+        """
+        This property returns a complete URL from the provided host and path.
+        If no protocol is given, it defaults to 'https://'.
+        Raises an AssertionError if no host or path are found in the postman collection.
+        """
+        assert self.host and self.path, print(
+            "Error: No host or path were found in the postman collection."
+        )
+        protocol = f"{self.protocol}" if self.protocol else "https://"
+        host = ".".join(self.host) + "/"
+        path = "/".join(self.update_path())
+        url = "".join([protocol, host, path])
+        url = "".join([host, path])
+        return url
+
+    @property
+    def params(self) -> Dict[str, str]:
+        """
+        A parameter is enabled/disabled in the Postman App.
+        Enabled parameters are parameters that do not contain a "disabled: true" key: value
+        returns a dictionary of enabled parameters.
+        """
+        if self.query:
+            params: Dict = {}
+            for param in self.query:
+                param = Param(param=param)
+                if not param.disabled:
+                    params[param.key] = param.value
+            return params
+
+    @property
+    def path_variables(self) -> Dict[str, str]:
+        """
+        A parameter is enabled/disabled in the Postman App.
+        Enabled parameters are parameters that do not contain a "disabled: true" key: value
+        returns a dictionary of enabled parameters.
+        """
+        if self.variables:
+            variables: Dict = {}
+            for variable in self.variables:
+                variable = Variable(variable=variable)
+                variables[variable.key] = variable.value
+            return variables
+
+    def update_path(self):
+        """
+        Update the path to replace each colon ":" with "${}"
+
+        Args:
+            self: The object itself
+
+        Returns:
+            path: The updated path
+        """
+        path = self.path
+        for i, element in enumerate(path):
+            if ":" in element:
+                element = element.replace(":", "${")
+                element = element + "}"
+                self.path[i] = element
+
+        return path
```

### Comparing `python-postman-0.2.0/pypostman/variable.py` & `python-postman-0.3.0/pypostman/variable.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,62 +1,62 @@
-import os
-import pendulum
-from string import Template
-
-from .template import CustomTemplate
-from .config import Variables
-
-
-class Variables:
-    def __init__(self, variables: Variables) -> None:
-        # load_dotenv()
-        self.variables = variables
-
-    @property
-    def as_dict(self):
-        collection_variables = {}
-        if self.variables:
-            for variable in self.variables:
-                collection_variables[variable.key] = variable.value
-        # collection_variables.update(os.environ)
-        return collection_variables
-
-    @property
-    def api_tags(self):
-        """
-        This property fetches the API tags associated with this object. It searches
-        through the variables associated with the object and looks for keys called
-        'API_TAGS', 'TAGS', or 'TAG'. If one of these is found, the associated value
-        is split into a list by comma and returned. If none of these are found, an
-        empty list is returned.
-        """
-        if self.variables:
-            for variable in self.variables:
-                if variable.key.upper() in ["API_TAGS", "TAGS", "TAG"]:
-                    return variable.value.split(",")
-        return []
-
-    def s3_prefix(self, **kwargs):
-        """
-        This function takes in an environment string and returns the S3 prefix
-        based on the provided environment and the current date. The S3 prefix is
-        based on the variables stored in self.variables and is created using the
-        CustomTemplate class.
-        """
-        if self.variables:
-            for variable in self.variables:
-                if variable.key.upper() in ["S3_PREFIX", "PREFIX"]:
-                    s3_prefix = CustomTemplate(variable.value).safe_substitute(**kwargs)
-                    return s3_prefix
-
-    @property
-    def model_name(self):
-        """
-        This function takes in an environment string and returns the S3 prefix
-        based on the provided environment and the current date. The S3 prefix is
-        based on the variables stored in self.variables and is created using the
-        CustomTemplate class.
-        """
-        if self.variables:
-            for variable in self.variables:
-                if variable.key.upper() in ["MODEL_NAME", "MODEL"]:
-                    return variable.value
+import os
+import pendulum
+from string import Template
+
+from .template import CustomTemplate
+from .config import Variables
+
+
+class Variables:
+    def __init__(self, variables: Variables) -> None:
+        # load_dotenv()
+        self.variables = variables
+
+    @property
+    def as_dict(self):
+        collection_variables = {}
+        if self.variables:
+            for variable in self.variables:
+                collection_variables[variable.key] = variable.value
+        # collection_variables.update(os.environ)
+        return collection_variables
+
+    @property
+    def api_tags(self):
+        """
+        This property fetches the API tags associated with this object. It searches
+        through the variables associated with the object and looks for keys called
+        'API_TAGS', 'TAGS', or 'TAG'. If one of these is found, the associated value
+        is split into a list by comma and returned. If none of these are found, an
+        empty list is returned.
+        """
+        if self.variables:
+            for variable in self.variables:
+                if variable.key.upper() in ["API_TAGS", "TAGS", "TAG"]:
+                    return variable.value.split(",")
+        return []
+
+    def s3_prefix(self, **kwargs):
+        """
+        This function takes in an environment string and returns the S3 prefix
+        based on the provided environment and the current date. The S3 prefix is
+        based on the variables stored in self.variables and is created using the
+        CustomTemplate class.
+        """
+        if self.variables:
+            for variable in self.variables:
+                if variable.key.upper() in ["S3_PREFIX", "PREFIX"]:
+                    s3_prefix = CustomTemplate(variable.value).safe_substitute(**kwargs)
+                    return s3_prefix
+
+    @property
+    def model_name(self):
+        """
+        This function takes in an environment string and returns the S3 prefix
+        based on the provided environment and the current date. The S3 prefix is
+        based on the variables stored in self.variables and is created using the
+        CustomTemplate class.
+        """
+        if self.variables:
+            for variable in self.variables:
+                if variable.key.upper() in ["MODEL_NAME", "MODEL"]:
+                    return variable.value
```

### Comparing `python-postman-0.2.0/pyproject.toml` & `python-postman-0.3.0/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-[build-system]
-requires = ["setuptools", "wheel", "setuptools-scm"]
-build-backend = "setuptools.build_meta"
-
-[project]
-name = "python-postman"
-version = "0.2.0"
-description = "Pypostman allows users to parse postman environments and postman collections."
-readme = "README.md"
-# homepage = "https://github.com/yudiell/python-postman"
-# repository = "https://github.com/yudiell/python-postman"
-requires-python = ">=3.8"
-keywords = ["postman", "python-postman", "pypostman", "api", "requests"]
-license = {text = "MIT"}
-classifiers = ["Programming Language :: Python :: 3"]
-dependencies = ["pydantic", "cryptography", "python-dotenv", "urllib3", "requests", "logbook", "pendulum", "boto3", "pytz", "retry2"]
-
-[project.optional-dependencies]
-mypy = ["mypy"]
-black = ["black"]
-
-[project.scripts]
+[build-system]
+requires = ["setuptools", "wheel", "setuptools-scm"]
+build-backend = "setuptools.build_meta"
+
+[project]
+name = "python-postman"
+version = "0.3.0"
+description = "Pypostman allows users to parse postman environments and postman collections."
+readme = "README.md"
+# homepage = "https://github.com/yudiell/python-postman" 
+# repository = "https://github.com/yudiell/python-postman"
+requires-python = ">=3.8"
+keywords = ["postman", "python-postman", "pypostman", "api", "requests"]
+license = {text = "MIT"}
+classifiers = ["Programming Language :: Python :: 3"]
+dependencies = ["pydantic", "cryptography", "python-dotenv", "urllib3", "requests", "logbook", "pendulum", "boto3", "pytz", "retry2"]
+
+[project.optional-dependencies]
+mypy = ["mypy"]
+black = ["black"]
+
+[project.scripts]
 pypostman = "pypostman.__main__:main"
```

### Comparing `python-postman-0.2.0/python_postman.egg-info/SOURCES.txt` & `python-postman-0.3.0/python_postman.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 pypostman/request.py
 pypostman/template.py
 pypostman/url.py
 pypostman/variable.py
 pypostman/modules/file.py
 pypostman/modules/http.py
 pypostman/modules/logger.py
-pypostman/utils/.gitkeep
 pypostman/utils/cli.py
+pypostman/utils/load_dotenvc.py
 python_postman.egg-info/PKG-INFO
 python_postman.egg-info/SOURCES.txt
 python_postman.egg-info/dependency_links.txt
 python_postman.egg-info/entry_points.txt
 python_postman.egg-info/requires.txt
 python_postman.egg-info/top_level.txt
```

