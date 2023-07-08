# Comparing `tmp/openai-promptify-py-0.0.3.tar.gz` & `tmp/openai-promptify-py-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openai-promptify-py-0.0.3.tar", last modified: Fri May 12 05:52:15 2023, max compression
+gzip compressed data, was "openai-promptify-py-0.0.4.tar", last modified: Sat Jul  8 17:05:15 2023, max compression
```

## Comparing `openai-promptify-py-0.0.3.tar` & `openai-promptify-py-0.0.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 maverick   (501) staff       (20)        0 2023-05-12 05:52:15.054950 openai-promptify-py-0.0.3/
--rw-r--r--   0 maverick   (501) staff       (20)     1839 2023-05-12 05:52:15.054814 openai-promptify-py-0.0.3/PKG-INFO
--rw-r--r--   0 maverick   (501) staff       (20)     1473 2023-05-12 05:47:27.000000 openai-promptify-py-0.0.3/README.md
--rw-r--r--   0 maverick   (501) staff       (20)      620 2023-05-12 05:51:56.000000 openai-promptify-py-0.0.3/pyproject.toml
--rw-r--r--   0 maverick   (501) staff       (20)        7 2023-03-21 07:28:20.000000 openai-promptify-py-0.0.3/requirements.txt
--rw-r--r--   0 maverick   (501) staff       (20)       38 2023-05-12 05:52:15.054987 openai-promptify-py-0.0.3/setup.cfg
-drwxr-xr-x   0 maverick   (501) staff       (20)        0 2023-05-12 05:52:15.053432 openai-promptify-py-0.0.3/src/
--rw-r--r--   0 maverick   (501) staff       (20)     7589 2023-05-12 05:44:02.000000 openai-promptify-py-0.0.3/src/openai_promptify.py
-drwxr-xr-x   0 maverick   (501) staff       (20)        0 2023-05-12 05:52:15.054205 openai-promptify-py-0.0.3/src/openai_promptify_py.egg-info/
--rw-r--r--   0 maverick   (501) staff       (20)     1839 2023-05-12 05:52:15.000000 openai-promptify-py-0.0.3/src/openai_promptify_py.egg-info/PKG-INFO
--rw-r--r--   0 maverick   (501) staff       (20)      347 2023-05-12 05:52:15.000000 openai-promptify-py-0.0.3/src/openai_promptify_py.egg-info/SOURCES.txt
--rw-r--r--   0 maverick   (501) staff       (20)        1 2023-05-12 05:52:15.000000 openai-promptify-py-0.0.3/src/openai_promptify_py.egg-info/dependency_links.txt
--rw-r--r--   0 maverick   (501) staff       (20)        7 2023-05-12 05:52:15.000000 openai-promptify-py-0.0.3/src/openai_promptify_py.egg-info/requires.txt
--rw-r--r--   0 maverick   (501) staff       (20)       17 2023-05-12 05:52:15.000000 openai-promptify-py-0.0.3/src/openai_promptify_py.egg-info/top_level.txt
-drwxr-xr-x   0 maverick   (501) staff       (20)        0 2023-05-12 05:52:15.054557 openai-promptify-py-0.0.3/tests/
--rw-r--r--   0 maverick   (501) staff       (20)      613 2023-03-22 09:01:34.000000 openai-promptify-py-0.0.3/tests/test_e2e.py
--rw-r--r--   0 maverick   (501) staff       (20)     7377 2023-05-12 05:44:02.000000 openai-promptify-py-0.0.3/tests/test_openai_promptif.py
+drwxr-xr-x   0 maverick   (501) staff       (20)        0 2023-07-08 17:05:15.200940 openai-promptify-py-0.0.4/
+-rw-r--r--   0 maverick   (501) staff       (20)     1839 2023-07-08 17:05:15.200744 openai-promptify-py-0.0.4/PKG-INFO
+-rw-r--r--   0 maverick   (501) staff       (20)     1473 2023-05-12 05:47:27.000000 openai-promptify-py-0.0.4/README.md
+-rw-r--r--   0 maverick   (501) staff       (20)      620 2023-07-08 16:59:14.000000 openai-promptify-py-0.0.4/pyproject.toml
+-rw-r--r--   0 maverick   (501) staff       (20)       15 2023-07-08 17:03:16.000000 openai-promptify-py-0.0.4/requirements.txt
+-rw-r--r--   0 maverick   (501) staff       (20)       38 2023-07-08 17:05:15.200989 openai-promptify-py-0.0.4/setup.cfg
+drwxr-xr-x   0 maverick   (501) staff       (20)        0 2023-07-08 17:05:15.199110 openai-promptify-py-0.0.4/src/
+-rw-r--r--   0 maverick   (501) staff       (20)     7846 2023-07-08 17:01:13.000000 openai-promptify-py-0.0.4/src/openai_promptify.py
+drwxr-xr-x   0 maverick   (501) staff       (20)        0 2023-07-08 17:05:15.199943 openai-promptify-py-0.0.4/src/openai_promptify_py.egg-info/
+-rw-r--r--   0 maverick   (501) staff       (20)     1839 2023-07-08 17:05:15.000000 openai-promptify-py-0.0.4/src/openai_promptify_py.egg-info/PKG-INFO
+-rw-r--r--   0 maverick   (501) staff       (20)      347 2023-07-08 17:05:15.000000 openai-promptify-py-0.0.4/src/openai_promptify_py.egg-info/SOURCES.txt
+-rw-r--r--   0 maverick   (501) staff       (20)        1 2023-07-08 17:05:15.000000 openai-promptify-py-0.0.4/src/openai_promptify_py.egg-info/dependency_links.txt
+-rw-r--r--   0 maverick   (501) staff       (20)       15 2023-07-08 17:05:15.000000 openai-promptify-py-0.0.4/src/openai_promptify_py.egg-info/requires.txt
+-rw-r--r--   0 maverick   (501) staff       (20)       17 2023-07-08 17:05:15.000000 openai-promptify-py-0.0.4/src/openai_promptify_py.egg-info/top_level.txt
+drwxr-xr-x   0 maverick   (501) staff       (20)        0 2023-07-08 17:05:15.200387 openai-promptify-py-0.0.4/tests/
+-rw-r--r--   0 maverick   (501) staff       (20)      613 2023-03-22 09:01:34.000000 openai-promptify-py-0.0.4/tests/test_e2e.py
+-rw-r--r--   0 maverick   (501) staff       (20)     7377 2023-05-12 05:44:02.000000 openai-promptify-py-0.0.4/tests/test_openai_promptif.py
```

### Comparing `openai-promptify-py-0.0.3/PKG-INFO` & `openai-promptify-py-0.0.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openai-promptify-py
-Version: 0.0.3
+Version: 0.0.4
 Summary: a utility wrapepr for openai calls [NOT OFFICIAL]
 Project-URL: Homepage, https://github.com/tumatrix/openai-promptify-py.git/README.md
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `openai-promptify-py-0.0.3/README.md` & `openai-promptify-py-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `openai-promptify-py-0.0.3/pyproject.toml` & `openai-promptify-py-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [tool.setuptools]
 #packages = ['.']
 package-dir = { "" = "src" }
 
 [project]
 name = "openai-promptify-py"
-version = "0.0.3"
+version = "0.0.4"
 description = "a utility wrapepr for openai calls [NOT OFFICIAL]"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
     "Programming Language :: Python :: 3",
     "Operating System :: OS Independent",
 ]
```

### Comparing `openai-promptify-py-0.0.3/src/openai_promptify.py` & `openai-promptify-py-0.0.4/src/openai_promptify.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 import re
 
 import openai
 from openai import InvalidRequestError
+from time import sleep
+
+from openai.error import RateLimitError
 
 model_prompt_limits = {
     'text-davinci-003': 4000,
     'gpt-3.5-turbo': 4000,
     'text-curie-001': 2048,
     'text-babbage-001': 2048,
     'text-ada-001': 2048,
@@ -161,14 +164,18 @@
     def call_openai_ex(self, input, text, current_chunk_size):
         try:
             return self.call_openai_api(f'{text}')
         except InvalidRequestError as e:
             if self.verbose:
                 print(e)
             return self.try_splitting_further(input, current_chunk_size, )
+        except RateLimitError as rle:
+            print('Rate limit exceeded, waiting 60 seconds')
+            sleep(60)
+            return self.call_openai_ex(input, text, current_chunk_size)
 
     def try_splitting_further(self, input, current_chunk_size):
         chunk_size = current_chunk_size * .75
         return self.execute(input, chunk_size=chunk_size, force_split=True)
 
     def call_openai_api(self, prompt):
         if self.model_name in chat_models:
```

### Comparing `openai-promptify-py-0.0.3/src/openai_promptify_py.egg-info/PKG-INFO` & `openai-promptify-py-0.0.4/src/openai_promptify_py.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openai-promptify-py
-Version: 0.0.3
+Version: 0.0.4
 Summary: a utility wrapepr for openai calls [NOT OFFICIAL]
 Project-URL: Homepage, https://github.com/tumatrix/openai-promptify-py.git/README.md
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `openai-promptify-py-0.0.3/tests/test_e2e.py` & `openai-promptify-py-0.0.4/tests/test_e2e.py`

 * *Files identical despite different names*

### Comparing `openai-promptify-py-0.0.3/tests/test_openai_promptif.py` & `openai-promptify-py-0.0.4/tests/test_openai_promptif.py`

 * *Files identical despite different names*

