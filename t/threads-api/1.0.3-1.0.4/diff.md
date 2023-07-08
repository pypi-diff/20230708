# Comparing `tmp/threads-api-1.0.3.tar.gz` & `tmp/threads-api-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "threads-api-1.0.3.tar", last modified: Fri Jul  7 22:25:15 2023, max compression
+gzip compressed data, was "threads-api-1.0.4.tar", last modified: Fri Jul  7 22:36:38 2023, max compression
```

## Comparing `threads-api-1.0.3.tar` & `threads-api-1.0.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-07 22:25:15.805283 threads-api-1.0.3/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     1068 2023-07-06 22:22:29.000000 threads-api-1.0.3/LICENSE
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     9732 2023-07-07 22:25:15.801283 threads-api-1.0.3/PKG-INFO
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     9206 2023-07-07 21:26:44.000000 threads-api-1.0.3/README.md
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      349 2023-07-06 21:24:15.000000 threads-api-1.0.3/pyproject.toml
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       38 2023-07-07 22:25:15.805283 threads-api-1.0.3/setup.cfg
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      787 2023-07-07 22:25:08.000000 threads-api-1.0.3/setup.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-07 22:25:15.801283 threads-api-1.0.3/threads_api/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)        0 2023-07-06 20:59:49.000000 threads-api-1.0.3/threads_api/__init__.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-07 22:25:15.801283 threads-api-1.0.3/threads_api/src/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)        0 2023-07-06 21:13:21.000000 threads-api-1.0.3/threads_api/src/__init__.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)    15315 2023-07-07 21:21:06.000000 threads-api-1.0.3/threads_api/src/threads_api.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-07 22:25:15.801283 threads-api-1.0.3/threads_api/tests/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)        0 2023-07-06 21:19:18.000000 threads-api-1.0.3/threads_api/tests/__init__.py
--rwxrwxr-x   0 daniel    (1000) daniel    (1000)      404 2023-07-07 21:21:06.000000 threads-api-1.0.3/threads_api/tests/get_threads_test.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-07 22:25:15.801283 threads-api-1.0.3/threads_api.egg-info/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     9732 2023-07-07 22:25:15.000000 threads-api-1.0.3/threads_api.egg-info/PKG-INFO
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      366 2023-07-07 22:25:15.000000 threads-api-1.0.3/threads_api.egg-info/SOURCES.txt
--rw-rw-r--   0 daniel    (1000) daniel    (1000)        1 2023-07-07 22:25:15.000000 threads-api-1.0.3/threads_api.egg-info/dependency_links.txt
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       17 2023-07-07 22:25:15.000000 threads-api-1.0.3/threads_api.egg-info/requires.txt
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       12 2023-07-07 22:25:15.000000 threads-api-1.0.3/threads_api.egg-info/top_level.txt
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-07 22:36:38.929481 threads-api-1.0.4/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     1068 2023-07-06 22:22:29.000000 threads-api-1.0.4/LICENSE
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     9425 2023-07-07 22:36:38.929481 threads-api-1.0.4/PKG-INFO
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     8899 2023-07-07 22:31:38.000000 threads-api-1.0.4/README.md
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      349 2023-07-06 21:24:15.000000 threads-api-1.0.4/pyproject.toml
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       38 2023-07-07 22:36:38.929481 threads-api-1.0.4/setup.cfg
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      787 2023-07-07 22:36:31.000000 threads-api-1.0.4/setup.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-07 22:36:38.925481 threads-api-1.0.4/threads_api/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)        0 2023-07-06 20:59:49.000000 threads-api-1.0.4/threads_api/__init__.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-07 22:36:38.929481 threads-api-1.0.4/threads_api/src/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)        0 2023-07-06 21:13:21.000000 threads-api-1.0.4/threads_api/src/__init__.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)    15315 2023-07-07 21:21:06.000000 threads-api-1.0.4/threads_api/src/threads_api.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-07 22:36:38.929481 threads-api-1.0.4/threads_api/tests/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)        0 2023-07-06 21:19:18.000000 threads-api-1.0.4/threads_api/tests/__init__.py
+-rwxrwxr-x   0 daniel    (1000) daniel    (1000)      404 2023-07-07 21:21:06.000000 threads-api-1.0.4/threads_api/tests/get_threads_test.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-07 22:36:38.929481 threads-api-1.0.4/threads_api.egg-info/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     9425 2023-07-07 22:36:38.000000 threads-api-1.0.4/threads_api.egg-info/PKG-INFO
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      366 2023-07-07 22:36:38.000000 threads-api-1.0.4/threads_api.egg-info/SOURCES.txt
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)        1 2023-07-07 22:36:38.000000 threads-api-1.0.4/threads_api.egg-info/dependency_links.txt
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       17 2023-07-07 22:36:38.000000 threads-api-1.0.4/threads_api.egg-info/requires.txt
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       12 2023-07-07 22:36:38.000000 threads-api-1.0.4/threads_api.egg-info/top_level.txt
```

### Comparing `threads-api-1.0.3/LICENSE` & `threads-api-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `threads-api-1.0.3/PKG-INFO` & `threads-api-1.0.4/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,50 +1,25 @@
-Metadata-Version: 2.1
-Name: threads-api
-Version: 1.0.3
-Summary: Unofficial Python client for Meta Threads API
-Home-page: https://github.com/danie1/threads-api
-Author: Danie1
-Author-email: 
-License: UNKNOWN
-Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # [<img src="./.github/logo.jpg" width="36" height="36" />](https://github.com/junhoyeo) Threads API
 
 [![Python](https://img.shields.io/badge/python-3.9%20%7C%203.10-blue)](https://www.npmjs.com/package/threads-api) [![MIT License](https://img.shields.io/badge/license-MIT-blue?style=flat-square&labelColor=black)](https://github.com/junhoyeo/threads-api/blob/main/license) [![Prettier Code Formatting](https://img.shields.io/badge/code_style-prettier-brightgreen.svg?style=flat-square&labelColor=black)](https://prettier.io)
 
 > Unofficial, Reverse-Engineered Python client for Meta's [Threads](https://threads.net).
 
 Inspired by [NPM Threads-API](https://github.com/junhoyeo/threads-api)
 
 # Threads API - Python
 
 Threads API is an unofficial Python client for Meta's Threads API. It allows you to interact with the API to retrieve user profile information, user IDs, and user profile threads.
 
 Table of content:
 
-* [Disclaimer](#disclaimer)
 * [Getting started](#getting-started)
-  * [How to install](#how-to-install)
-  * [Initialization](#initialization)
-  * [Examples](#examples)
-* [API](#api)
-  * [Login](#login)
-  * [Get User By Username](#get-user-by-username)
-  * [Get User By Identifier](#get-user-by-identifier)
-  * [Get User Threads](#get-user-threads)
-  * [Get User Replies](#get-user-replies)
-  * [Get Post](#get-post)
+  * [Installation](#Installation)
+* [Usage Examples](#Usage-Examples)
+
 
 ## Getting Started
 
 ### 📦 Installation
 ```bash
 pip install threads-api
 ```
@@ -270,9 +245,8 @@
 - [ ] 🚧 Write data (i.e. write automated Threads)
 - [ ]🚧  CI/CD
   - [ ]🚧  Pytest
   - [ ]🚧  GitHub Actions Pipeline
 
 
 # License
-This project is licensed under the MIT license.
-
+This project is licensed under the MIT license.
```

### Comparing `threads-api-1.0.3/README.md` & `threads-api-1.0.4/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,33 +1,42 @@
+Metadata-Version: 2.1
+Name: threads-api
+Version: 1.0.4
+Summary: Unofficial Python client for Meta Threads API
+Home-page: https://github.com/danie1/threads-api
+Author: Danie1
+Author-email: 
+License: UNKNOWN
+Platform: UNKNOWN
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # [<img src="./.github/logo.jpg" width="36" height="36" />](https://github.com/junhoyeo) Threads API
 
 [![Python](https://img.shields.io/badge/python-3.9%20%7C%203.10-blue)](https://www.npmjs.com/package/threads-api) [![MIT License](https://img.shields.io/badge/license-MIT-blue?style=flat-square&labelColor=black)](https://github.com/junhoyeo/threads-api/blob/main/license) [![Prettier Code Formatting](https://img.shields.io/badge/code_style-prettier-brightgreen.svg?style=flat-square&labelColor=black)](https://prettier.io)
 
 > Unofficial, Reverse-Engineered Python client for Meta's [Threads](https://threads.net).
 
 Inspired by [NPM Threads-API](https://github.com/junhoyeo/threads-api)
 
 # Threads API - Python
 
 Threads API is an unofficial Python client for Meta's Threads API. It allows you to interact with the API to retrieve user profile information, user IDs, and user profile threads.
 
 Table of content:
 
-* [Disclaimer](#disclaimer)
 * [Getting started](#getting-started)
-  * [How to install](#how-to-install)
-  * [Initialization](#initialization)
-  * [Examples](#examples)
-* [API](#api)
-  * [Login](#login)
-  * [Get User By Username](#get-user-by-username)
-  * [Get User By Identifier](#get-user-by-identifier)
-  * [Get User Threads](#get-user-threads)
-  * [Get User Replies](#get-user-replies)
-  * [Get Post](#get-post)
+  * [Installation](#Installation)
+* [Usage Examples](#Usage-Examples)
+
 
 ## Getting Started
 
 ### 📦 Installation
 ```bash
 pip install threads-api
 ```
@@ -253,8 +262,9 @@
 - [ ] 🚧 Write data (i.e. write automated Threads)
 - [ ]🚧  CI/CD
   - [ ]🚧  Pytest
   - [ ]🚧  GitHub Actions Pipeline
 
 
 # License
-This project is licensed under the MIT license.
+This project is licensed under the MIT license.
+
```

### Comparing `threads-api-1.0.3/setup.py` & `threads-api-1.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='threads-api',
-    version='1.0.3',
+    version='1.0.4',
     description='Unofficial Python client for Meta Threads API',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Danie1',
     author_email='',
     url='https://github.com/danie1/threads-api',
     py_modules=find_packages(),
```

### Comparing `threads-api-1.0.3/threads_api/src/threads_api.py` & `threads-api-1.0.4/threads_api/src/threads_api.py`

 * *Files identical despite different names*

### Comparing `threads-api-1.0.3/threads_api.egg-info/PKG-INFO` & `threads-api-1.0.4/threads_api.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: threads-api
-Version: 1.0.3
+Version: 1.0.4
 Summary: Unofficial Python client for Meta Threads API
 Home-page: https://github.com/danie1/threads-api
 Author: Danie1
 Author-email: 
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
@@ -25,26 +25,18 @@
 
 # Threads API - Python
 
 Threads API is an unofficial Python client for Meta's Threads API. It allows you to interact with the API to retrieve user profile information, user IDs, and user profile threads.
 
 Table of content:
 
-* [Disclaimer](#disclaimer)
 * [Getting started](#getting-started)
-  * [How to install](#how-to-install)
-  * [Initialization](#initialization)
-  * [Examples](#examples)
-* [API](#api)
-  * [Login](#login)
-  * [Get User By Username](#get-user-by-username)
-  * [Get User By Identifier](#get-user-by-identifier)
-  * [Get User Threads](#get-user-threads)
-  * [Get User Replies](#get-user-replies)
-  * [Get Post](#get-post)
+  * [Installation](#Installation)
+* [Usage Examples](#Usage-Examples)
+
 
 ## Getting Started
 
 ### 📦 Installation
 ```bash
 pip install threads-api
 ```
```

