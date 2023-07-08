# Comparing `tmp/mosparo_api_client-1.0.0.tar.gz` & `tmp/mosparo_api_client-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mosparo_api_client-1.0.0.tar", last modified: Sat Apr 29 12:54:04 2023, max compression
+gzip compressed data, was "mosparo_api_client-1.0.1.tar", last modified: Sat Jul  8 08:59:02 2023, max compression
```

## Comparing `mosparo_api_client-1.0.0.tar` & `mosparo_api_client-1.0.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxr-x   0 mzo       (5678) mzo       (5678)        0 2023-04-29 12:54:04.711460 mosparo_api_client-1.0.0/
--rw-rw-r--   0 mzo       (5678) mzo       (5678)     1102 2023-04-29 12:53:56.000000 mosparo_api_client-1.0.0/LICENSE
--rw-rw-r--   0 mzo       (5678) mzo       (5678)     8209 2023-04-29 12:54:04.711460 mosparo_api_client-1.0.0/PKG-INFO
--rw-rw-r--   0 mzo       (5678) mzo       (5678)     5907 2023-04-29 12:53:56.000000 mosparo_api_client-1.0.0/README.md
-drwxrwxr-x   0 mzo       (5678) mzo       (5678)        0 2023-04-29 12:54:04.707460 mosparo_api_client-1.0.0/mosparo_api_client/
--rw-rw-r--   0 mzo       (5678) mzo       (5678)     6784 2023-04-29 12:53:56.000000 mosparo_api_client-1.0.0/mosparo_api_client/Client.py
--rw-rw-r--   0 mzo       (5678) mzo       (5678)       43 2023-04-29 12:53:56.000000 mosparo_api_client-1.0.0/mosparo_api_client/MosparoException.py
--rw-rw-r--   0 mzo       (5678) mzo       (5678)     4078 2023-04-29 12:53:56.000000 mosparo_api_client-1.0.0/mosparo_api_client/RequestHelper.py
--rw-rw-r--   0 mzo       (5678) mzo       (5678)     1651 2023-04-29 12:53:56.000000 mosparo_api_client-1.0.0/mosparo_api_client/StatisticResult.py
--rw-rw-r--   0 mzo       (5678) mzo       (5678)     2635 2023-04-29 12:53:56.000000 mosparo_api_client-1.0.0/mosparo_api_client/VerificationResult.py
--rw-rw-r--   0 mzo       (5678) mzo       (5678)      205 2023-04-29 12:53:56.000000 mosparo_api_client-1.0.0/mosparo_api_client/__init__.py
-drwxrwxr-x   0 mzo       (5678) mzo       (5678)        0 2023-04-29 12:54:04.707460 mosparo_api_client-1.0.0/mosparo_api_client.egg-info/
--rw-rw-r--   0 mzo       (5678) mzo       (5678)     8209 2023-04-29 12:54:04.000000 mosparo_api_client-1.0.0/mosparo_api_client.egg-info/PKG-INFO
--rw-rw-r--   0 mzo       (5678) mzo       (5678)      567 2023-04-29 12:54:04.000000 mosparo_api_client-1.0.0/mosparo_api_client.egg-info/SOURCES.txt
--rw-rw-r--   0 mzo       (5678) mzo       (5678)        1 2023-04-29 12:54:04.000000 mosparo_api_client-1.0.0/mosparo_api_client.egg-info/dependency_links.txt
--rw-rw-r--   0 mzo       (5678) mzo       (5678)       54 2023-04-29 12:54:04.000000 mosparo_api_client-1.0.0/mosparo_api_client.egg-info/requires.txt
--rw-rw-r--   0 mzo       (5678) mzo       (5678)       19 2023-04-29 12:54:04.000000 mosparo_api_client-1.0.0/mosparo_api_client.egg-info/top_level.txt
--rw-rw-r--   0 mzo       (5678) mzo       (5678)     1205 2023-04-29 12:53:56.000000 mosparo_api_client-1.0.0/pyproject.toml
--rw-rw-r--   0 mzo       (5678) mzo       (5678)       38 2023-04-29 12:54:04.711460 mosparo_api_client-1.0.0/setup.cfg
-drwxrwxr-x   0 mzo       (5678) mzo       (5678)        0 2023-04-29 12:54:04.711460 mosparo_api_client-1.0.0/tests/
--rw-rw-r--   0 mzo       (5678) mzo       (5678)     7919 2023-04-29 12:53:56.000000 mosparo_api_client-1.0.0/tests/test_Client.py
--rw-rw-r--   0 mzo       (5678) mzo       (5678)     2916 2023-04-29 12:53:56.000000 mosparo_api_client-1.0.0/tests/test_RequestHelper.py
--rw-rw-r--   0 mzo       (5678) mzo       (5678)      412 2023-04-29 12:53:56.000000 mosparo_api_client-1.0.0/tests/test_StatisticResult.py
--rw-rw-r--   0 mzo       (5678) mzo       (5678)      759 2023-04-29 12:53:56.000000 mosparo_api_client-1.0.0/tests/test_VerificationResult.py
+drwxrwxr-x   0 mzo       (5678) mzo       (5678)        0 2023-07-08 08:59:02.189947 mosparo_api_client-1.0.1/
+-rw-rw-r--   0 mzo       (5678) mzo       (5678)     1102 2023-07-08 08:58:55.000000 mosparo_api_client-1.0.1/LICENSE
+-rw-rw-r--   0 mzo       (5678) mzo       (5678)     8265 2023-07-08 08:59:02.189947 mosparo_api_client-1.0.1/PKG-INFO
+-rw-rw-r--   0 mzo       (5678) mzo       (5678)     5907 2023-07-08 08:58:55.000000 mosparo_api_client-1.0.1/README.md
+drwxrwxr-x   0 mzo       (5678) mzo       (5678)        0 2023-07-08 08:59:02.185947 mosparo_api_client-1.0.1/mosparo_api_client/
+-rw-rw-r--   0 mzo       (5678) mzo       (5678)     6784 2023-07-08 08:58:55.000000 mosparo_api_client-1.0.1/mosparo_api_client/Client.py
+-rw-rw-r--   0 mzo       (5678) mzo       (5678)       43 2023-07-08 08:58:55.000000 mosparo_api_client-1.0.1/mosparo_api_client/MosparoException.py
+-rw-rw-r--   0 mzo       (5678) mzo       (5678)     4078 2023-07-08 08:58:55.000000 mosparo_api_client-1.0.1/mosparo_api_client/RequestHelper.py
+-rw-rw-r--   0 mzo       (5678) mzo       (5678)     1651 2023-07-08 08:58:55.000000 mosparo_api_client-1.0.1/mosparo_api_client/StatisticResult.py
+-rw-rw-r--   0 mzo       (5678) mzo       (5678)     2635 2023-07-08 08:58:55.000000 mosparo_api_client-1.0.1/mosparo_api_client/VerificationResult.py
+-rw-rw-r--   0 mzo       (5678) mzo       (5678)      205 2023-07-08 08:58:55.000000 mosparo_api_client-1.0.1/mosparo_api_client/__init__.py
+drwxrwxr-x   0 mzo       (5678) mzo       (5678)        0 2023-07-08 08:59:02.185947 mosparo_api_client-1.0.1/mosparo_api_client.egg-info/
+-rw-rw-r--   0 mzo       (5678) mzo       (5678)     8265 2023-07-08 08:59:02.000000 mosparo_api_client-1.0.1/mosparo_api_client.egg-info/PKG-INFO
+-rw-rw-r--   0 mzo       (5678) mzo       (5678)      567 2023-07-08 08:59:02.000000 mosparo_api_client-1.0.1/mosparo_api_client.egg-info/SOURCES.txt
+-rw-rw-r--   0 mzo       (5678) mzo       (5678)        1 2023-07-08 08:59:02.000000 mosparo_api_client-1.0.1/mosparo_api_client.egg-info/dependency_links.txt
+-rw-rw-r--   0 mzo       (5678) mzo       (5678)       62 2023-07-08 08:59:02.000000 mosparo_api_client-1.0.1/mosparo_api_client.egg-info/requires.txt
+-rw-rw-r--   0 mzo       (5678) mzo       (5678)       19 2023-07-08 08:59:02.000000 mosparo_api_client-1.0.1/mosparo_api_client.egg-info/top_level.txt
+-rw-rw-r--   0 mzo       (5678) mzo       (5678)     1264 2023-07-08 08:58:55.000000 mosparo_api_client-1.0.1/pyproject.toml
+-rw-rw-r--   0 mzo       (5678) mzo       (5678)       38 2023-07-08 08:59:02.189947 mosparo_api_client-1.0.1/setup.cfg
+drwxrwxr-x   0 mzo       (5678) mzo       (5678)        0 2023-07-08 08:59:02.185947 mosparo_api_client-1.0.1/tests/
+-rw-rw-r--   0 mzo       (5678) mzo       (5678)     7919 2023-07-08 08:58:55.000000 mosparo_api_client-1.0.1/tests/test_Client.py
+-rw-rw-r--   0 mzo       (5678) mzo       (5678)     2916 2023-07-08 08:58:55.000000 mosparo_api_client-1.0.1/tests/test_RequestHelper.py
+-rw-rw-r--   0 mzo       (5678) mzo       (5678)      412 2023-07-08 08:58:55.000000 mosparo_api_client-1.0.1/tests/test_StatisticResult.py
+-rw-rw-r--   0 mzo       (5678) mzo       (5678)      759 2023-07-08 08:58:55.000000 mosparo_api_client-1.0.1/tests/test_VerificationResult.py
```

### Comparing `mosparo_api_client-1.0.0/LICENSE` & `mosparo_api_client-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mosparo_api_client-1.0.0/PKG-INFO` & `mosparo_api_client-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mosparo_api_client
-Version: 1.0.0
+Version: 1.0.1
 Summary: Python API Client to communicate with mosparo.
 Author-email: mosparo Core Developers <info@mosparo.io>
 License: The MIT License (MIT)
         
         Copyright 2023 mosparo Core Developers and contributors
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -23,14 +23,15 @@
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
         THE SOFTWARE.
 Project-URL: Website, https://mosparo.io
 Project-URL: GitHub, https://github.com/mosparo/python-api-client
 Keywords: mosparo,api-client,spam-protection,accessibility,captcha
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mosparo_api_client Version: 1.0.0 Summary: Python
+Metadata-Version: 2.1 Name: mosparo_api_client Version: 1.0.1 Summary: Python
 API Client to communicate with mosparo. Author-email: mosparo Core Developers
 mosparo.io> License: The MIT License (MIT) Copyright 2023 mosparo Core
 Developers and contributors Permission is hereby granted, free of charge, to
 any person obtaining a copy of this software and associated documentation files
 (the "Software"), to deal in the Software without restriction, including
 without limitation the rights to use, copy, modify, merge, publish, distribute,
 sublicense, and/or sell copies of the Software, and to permit persons to whom
@@ -13,24 +13,24 @@
 LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE
 AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE
 LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF
 CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE
 SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE. Project-URL: Website,
 https://mosparo.io Project-URL: GitHub, https://github.com/mosparo/python-api-
 client Keywords: mosparo,api-client,spam-protection,accessibility,captcha
-Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
-:: MIT License Classifier: Operating System :: OS Independent Classifier:
-Programming Language :: Python :: 3.5 Classifier: Programming Language ::
-Python :: 3.6 Classifier: Programming Language :: Python :: 3.7 Classifier:
-Programming Language :: Python :: 3.8 Classifier: Programming Language ::
-Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
-Programming Language :: Python :: 3.11 Classifier: Programming Language ::
-Python :: 3.12 Classifier: Topic :: Internet Requires-Python: >=3.5
-Description-Content-Type: text/markdown Provides-Extra: dev License-File:
-LICENSE  
+Classifier: Development Status :: 5 - Production/Stable Classifier: Intended
+Audience :: Developers Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent Classifier: Programming Language
+:: Python :: 3.5 Classifier: Programming Language :: Python :: 3.6 Classifier:
+Programming Language :: Python :: 3.7 Classifier: Programming Language ::
+Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
+Programming Language :: Python :: 3.10 Classifier: Programming Language ::
+Python :: 3.11 Classifier: Programming Language :: Python :: 3.12 Classifier:
+Topic :: Internet Requires-Python: >=3.5 Description-Content-Type: text/
+markdown Provides-Extra: dev License-File: LICENSE  
      [mosparo logo contains a bird with the name Mo and the mosparo text]
                         ****** Python API Client ******
   This library offers the API client to communicate with mosparo to verify a
                                   submission.
 ----- ## Description This Python library lets you connect to a mosparo
 installation and verify the submitted data. ## Installation ### Install using
 pip Install this library by using pip: ```text pip install mosparo-api-client
```

### Comparing `mosparo_api_client-1.0.0/README.md` & `mosparo_api_client-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `mosparo_api_client-1.0.0/mosparo_api_client/Client.py` & `mosparo_api_client-1.0.1/mosparo_api_client/Client.py`

 * *Files identical despite different names*

### Comparing `mosparo_api_client-1.0.0/mosparo_api_client/RequestHelper.py` & `mosparo_api_client-1.0.1/mosparo_api_client/RequestHelper.py`

 * *Files identical despite different names*

### Comparing `mosparo_api_client-1.0.0/mosparo_api_client/StatisticResult.py` & `mosparo_api_client-1.0.1/mosparo_api_client/StatisticResult.py`

 * *Files identical despite different names*

### Comparing `mosparo_api_client-1.0.0/mosparo_api_client/VerificationResult.py` & `mosparo_api_client-1.0.1/mosparo_api_client/VerificationResult.py`

 * *Files identical despite different names*

### Comparing `mosparo_api_client-1.0.0/mosparo_api_client.egg-info/PKG-INFO` & `mosparo_api_client-1.0.1/mosparo_api_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mosparo-api-client
-Version: 1.0.0
+Version: 1.0.1
 Summary: Python API Client to communicate with mosparo.
 Author-email: mosparo Core Developers <info@mosparo.io>
 License: The MIT License (MIT)
         
         Copyright 2023 mosparo Core Developers and contributors
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -23,14 +23,15 @@
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
         THE SOFTWARE.
 Project-URL: Website, https://mosparo.io
 Project-URL: GitHub, https://github.com/mosparo/python-api-client
 Keywords: mosparo,api-client,spam-protection,accessibility,captcha
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mosparo-api-client Version: 1.0.0 Summary: Python
+Metadata-Version: 2.1 Name: mosparo-api-client Version: 1.0.1 Summary: Python
 API Client to communicate with mosparo. Author-email: mosparo Core Developers
 mosparo.io> License: The MIT License (MIT) Copyright 2023 mosparo Core
 Developers and contributors Permission is hereby granted, free of charge, to
 any person obtaining a copy of this software and associated documentation files
 (the "Software"), to deal in the Software without restriction, including
 without limitation the rights to use, copy, modify, merge, publish, distribute,
 sublicense, and/or sell copies of the Software, and to permit persons to whom
@@ -13,24 +13,24 @@
 LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE
 AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE
 LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF
 CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE
 SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE. Project-URL: Website,
 https://mosparo.io Project-URL: GitHub, https://github.com/mosparo/python-api-
 client Keywords: mosparo,api-client,spam-protection,accessibility,captcha
-Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
-:: MIT License Classifier: Operating System :: OS Independent Classifier:
-Programming Language :: Python :: 3.5 Classifier: Programming Language ::
-Python :: 3.6 Classifier: Programming Language :: Python :: 3.7 Classifier:
-Programming Language :: Python :: 3.8 Classifier: Programming Language ::
-Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
-Programming Language :: Python :: 3.11 Classifier: Programming Language ::
-Python :: 3.12 Classifier: Topic :: Internet Requires-Python: >=3.5
-Description-Content-Type: text/markdown Provides-Extra: dev License-File:
-LICENSE  
+Classifier: Development Status :: 5 - Production/Stable Classifier: Intended
+Audience :: Developers Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent Classifier: Programming Language
+:: Python :: 3.5 Classifier: Programming Language :: Python :: 3.6 Classifier:
+Programming Language :: Python :: 3.7 Classifier: Programming Language ::
+Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
+Programming Language :: Python :: 3.10 Classifier: Programming Language ::
+Python :: 3.11 Classifier: Programming Language :: Python :: 3.12 Classifier:
+Topic :: Internet Requires-Python: >=3.5 Description-Content-Type: text/
+markdown Provides-Extra: dev License-File: LICENSE  
      [mosparo logo contains a bird with the name Mo and the mosparo text]
                         ****** Python API Client ******
   This library offers the API client to communicate with mosparo to verify a
                                   submission.
 ----- ## Description This Python library lets you connect to a mosparo
 installation and verify the submitted data. ## Installation ### Install using
 pip Install this library by using pip: ```text pip install mosparo-api-client
```

### Comparing `mosparo_api_client-1.0.0/mosparo_api_client.egg-info/SOURCES.txt` & `mosparo_api_client-1.0.1/mosparo_api_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mosparo_api_client-1.0.0/pyproject.toml` & `mosparo_api_client-1.0.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mosparo_api_client"
-version = "1.0.0"
+version = "1.0.1"
 description = "Python API Client to communicate with mosparo."
 readme = "README.md"
 authors = [{ name = "mosparo Core Developers", email = "info@mosparo.io" }]
 license = { file = "LICENSE" }
 classifiers = [
+    "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3.5",
     "Programming Language :: Python :: 3.6",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
@@ -21,15 +22,15 @@
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "Topic :: Internet",
 ]
 keywords = ["mosparo", "api-client", "spam-protection", "accessibility", "captcha"]
 dependencies = [
-    "requests"
+    "requests>=2.31.0"
 ]
 requires-python = ">=3.5"
 
 [project.optional-dependencies]
 dev = ["pytest-runner", "requests-mock", "pip-tools"]
 
 [project.urls]
```

### Comparing `mosparo_api_client-1.0.0/tests/test_Client.py` & `mosparo_api_client-1.0.1/tests/test_Client.py`

 * *Files identical despite different names*

### Comparing `mosparo_api_client-1.0.0/tests/test_RequestHelper.py` & `mosparo_api_client-1.0.1/tests/test_RequestHelper.py`

 * *Files identical despite different names*

### Comparing `mosparo_api_client-1.0.0/tests/test_VerificationResult.py` & `mosparo_api_client-1.0.1/tests/test_VerificationResult.py`

 * *Files identical despite different names*

