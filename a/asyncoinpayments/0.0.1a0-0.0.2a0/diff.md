# Comparing `tmp/asyncoinpayments-0.0.1a0.tar.gz` & `tmp/asyncoinpayments-0.0.2a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asyncoinpayments-0.0.1a0.tar", last modified: Sat Jul  8 19:58:03 2023, max compression
+gzip compressed data, was "asyncoinpayments-0.0.2a0.tar", last modified: Sat Jul  8 20:21:08 2023, max compression
```

## Comparing `asyncoinpayments-0.0.1a0.tar` & `asyncoinpayments-0.0.2a0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 flalugli  (1000) flalugli  (1000)        0 2023-07-08 19:58:03.562988 asyncoinpayments-0.0.1a0/
--rw-rw-r--   0 flalugli  (1000) flalugli  (1000)     1207 2023-07-08 19:58:03.562988 asyncoinpayments-0.0.1a0/PKG-INFO
--rw-rw-r--   0 flalugli  (1000) flalugli  (1000)      403 2023-07-08 16:29:30.000000 asyncoinpayments-0.0.1a0/README.md
-drwxrwxr-x   0 flalugli  (1000) flalugli  (1000)        0 2023-07-08 19:58:03.562988 asyncoinpayments-0.0.1a0/asyncoinpayments/
--rw-rw-r--   0 flalugli  (1000) flalugli  (1000)       43 2023-07-08 19:34:54.000000 asyncoinpayments-0.0.1a0/asyncoinpayments/__init__.py
--rw-rw-r--   0 flalugli  (1000) flalugli  (1000)    16708 2023-07-08 19:53:58.000000 asyncoinpayments-0.0.1a0/asyncoinpayments/coinpayments.py
--rw-rw-r--   0 flalugli  (1000) flalugli  (1000)      155 2023-07-08 15:55:02.000000 asyncoinpayments-0.0.1a0/asyncoinpayments/errors.py
--rw-rw-r--   0 flalugli  (1000) flalugli  (1000)       51 2023-07-08 15:55:21.000000 asyncoinpayments-0.0.1a0/asyncoinpayments/utils.py
-drwxrwxr-x   0 flalugli  (1000) flalugli  (1000)        0 2023-07-08 19:58:03.562988 asyncoinpayments-0.0.1a0/asyncoinpayments.egg-info/
--rw-rw-r--   0 flalugli  (1000) flalugli  (1000)     1207 2023-07-08 19:58:03.000000 asyncoinpayments-0.0.1a0/asyncoinpayments.egg-info/PKG-INFO
--rw-rw-r--   0 flalugli  (1000) flalugli  (1000)      332 2023-07-08 19:58:03.000000 asyncoinpayments-0.0.1a0/asyncoinpayments.egg-info/SOURCES.txt
--rw-rw-r--   0 flalugli  (1000) flalugli  (1000)        1 2023-07-08 19:58:03.000000 asyncoinpayments-0.0.1a0/asyncoinpayments.egg-info/dependency_links.txt
--rw-rw-r--   0 flalugli  (1000) flalugli  (1000)       37 2023-07-08 19:58:03.000000 asyncoinpayments-0.0.1a0/asyncoinpayments.egg-info/requires.txt
--rw-rw-r--   0 flalugli  (1000) flalugli  (1000)       17 2023-07-08 19:58:03.000000 asyncoinpayments-0.0.1a0/asyncoinpayments.egg-info/top_level.txt
--rw-rw-r--   0 flalugli  (1000) flalugli  (1000)       38 2023-07-08 19:58:03.562988 asyncoinpayments-0.0.1a0/setup.cfg
--rw-rw-r--   0 flalugli  (1000) flalugli  (1000)     1137 2023-07-08 19:56:20.000000 asyncoinpayments-0.0.1a0/setup.py
+drwxrwxr-x   0 flalugli  (1000) flalugli  (1000)        0 2023-07-08 20:21:08.363525 asyncoinpayments-0.0.2a0/
+-rw-rw-r--   0 flalugli  (1000) flalugli  (1000)     1258 2023-07-08 20:21:08.363525 asyncoinpayments-0.0.2a0/PKG-INFO
+-rw-rw-r--   0 flalugli  (1000) flalugli  (1000)      432 2023-07-08 20:18:04.000000 asyncoinpayments-0.0.2a0/README.md
+drwxrwxr-x   0 flalugli  (1000) flalugli  (1000)        0 2023-07-08 20:21:08.363525 asyncoinpayments-0.0.2a0/asyncoinpayments/
+-rw-rw-r--   0 flalugli  (1000) flalugli  (1000)       43 2023-07-08 19:34:54.000000 asyncoinpayments-0.0.2a0/asyncoinpayments/__init__.py
+-rw-rw-r--   0 flalugli  (1000) flalugli  (1000)    16708 2023-07-08 19:53:58.000000 asyncoinpayments-0.0.2a0/asyncoinpayments/coinpayments.py
+-rw-rw-r--   0 flalugli  (1000) flalugli  (1000)      155 2023-07-08 15:55:02.000000 asyncoinpayments-0.0.2a0/asyncoinpayments/errors.py
+-rw-rw-r--   0 flalugli  (1000) flalugli  (1000)       51 2023-07-08 15:55:21.000000 asyncoinpayments-0.0.2a0/asyncoinpayments/utils.py
+drwxrwxr-x   0 flalugli  (1000) flalugli  (1000)        0 2023-07-08 20:21:08.363525 asyncoinpayments-0.0.2a0/asyncoinpayments.egg-info/
+-rw-rw-r--   0 flalugli  (1000) flalugli  (1000)     1258 2023-07-08 20:21:08.000000 asyncoinpayments-0.0.2a0/asyncoinpayments.egg-info/PKG-INFO
+-rw-rw-r--   0 flalugli  (1000) flalugli  (1000)      332 2023-07-08 20:21:08.000000 asyncoinpayments-0.0.2a0/asyncoinpayments.egg-info/SOURCES.txt
+-rw-rw-r--   0 flalugli  (1000) flalugli  (1000)        1 2023-07-08 20:21:08.000000 asyncoinpayments-0.0.2a0/asyncoinpayments.egg-info/dependency_links.txt
+-rw-rw-r--   0 flalugli  (1000) flalugli  (1000)       37 2023-07-08 20:21:08.000000 asyncoinpayments-0.0.2a0/asyncoinpayments.egg-info/requires.txt
+-rw-rw-r--   0 flalugli  (1000) flalugli  (1000)       17 2023-07-08 20:21:08.000000 asyncoinpayments-0.0.2a0/asyncoinpayments.egg-info/top_level.txt
+-rw-rw-r--   0 flalugli  (1000) flalugli  (1000)       38 2023-07-08 20:21:08.363525 asyncoinpayments-0.0.2a0/setup.cfg
+-rw-rw-r--   0 flalugli  (1000) flalugli  (1000)     1127 2023-07-08 20:20:54.000000 asyncoinpayments-0.0.2a0/setup.py
```

### Comparing `asyncoinpayments-0.0.1a0/PKG-INFO` & `asyncoinpayments-0.0.2a0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,36 +1,40 @@
 Metadata-Version: 2.1
 Name: asyncoinpayments
-Version: 0.0.1a0
+Version: 0.0.2a0
 Summary: Python Asynchronous Wrapper of the CoinPayments API
 Home-page: https://github.com/flalugli/asyncoinpayments
-Author: fla (Flavio Lugli)
+Author: flalugli
 Author-email: <flalugli.dev@gmail.com>
 License: Apache License 2.0
 Description: 
         # AsynCoinpayments  
         
         An async/await compatible python wrapper for the CoinPayments API  
         
         ---
         
         ## How to install  
         
-        In the command prompt, type `pip install asyncoinpayments`
+        ```
+        # run this in the command propt or terminal
+        pip install asyncoinpayments  
+        ```
         
         ## Features  
         - Fast to setup and simple to use
         - Easy to use async/await interface
         - API calls using aiohttp requests  
         - create your own API calls
         
         ### Contact me
         
-        **Email** : <flalugli.dev@gmail.com>
-        **Discord** : flalugli 
+        **Email** : <flalugli.dev@gmail.com>  
+        **Discord** : flalugli   
+        
 Keywords: python,crypto,cryptocurrency,payment gateway,async,aiohttp
 Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `asyncoinpayments-0.0.1a0/asyncoinpayments/coinpayments.py` & `asyncoinpayments-0.0.2a0/asyncoinpayments/coinpayments.py`

 * *Files identical despite different names*

### Comparing `asyncoinpayments-0.0.1a0/asyncoinpayments.egg-info/PKG-INFO` & `asyncoinpayments-0.0.2a0/asyncoinpayments.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,36 +1,40 @@
 Metadata-Version: 2.1
 Name: asyncoinpayments
-Version: 0.0.1a0
+Version: 0.0.2a0
 Summary: Python Asynchronous Wrapper of the CoinPayments API
 Home-page: https://github.com/flalugli/asyncoinpayments
-Author: fla (Flavio Lugli)
+Author: flalugli
 Author-email: <flalugli.dev@gmail.com>
 License: Apache License 2.0
 Description: 
         # AsynCoinpayments  
         
         An async/await compatible python wrapper for the CoinPayments API  
         
         ---
         
         ## How to install  
         
-        In the command prompt, type `pip install asyncoinpayments`
+        ```
+        # run this in the command propt or terminal
+        pip install asyncoinpayments  
+        ```
         
         ## Features  
         - Fast to setup and simple to use
         - Easy to use async/await interface
         - API calls using aiohttp requests  
         - create your own API calls
         
         ### Contact me
         
-        **Email** : <flalugli.dev@gmail.com>
-        **Discord** : flalugli 
+        **Email** : <flalugli.dev@gmail.com>  
+        **Discord** : flalugli   
+        
 Keywords: python,crypto,cryptocurrency,payment gateway,async,aiohttp
 Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `asyncoinpayments-0.0.1a0/setup.py` & `asyncoinpayments-0.0.2a0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,23 +4,23 @@
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     
     long_description = "\n" + fh.read()
 
-VERSION = '0.0.1a'
+VERSION = '0.0.2a'
 DESCRIPTION = 'Python Asynchronous Wrapper of the CoinPayments API'
 
 
 # Setting up
 setup(
     name="asyncoinpayments",
     version=VERSION,
-    author="fla (Flavio Lugli)",
+    author="flalugli",
     author_email="<flalugli.dev@gmail.com>",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=long_description,
     url="https://github.com/flalugli/asyncoinpayments",
     license="Apache License 2.0",
     packages=find_packages(),
```

