# Comparing `tmp/threads-api-1.0.1.tar.gz` & `tmp/threads-api-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "threads-api-1.0.1.tar", last modified: Fri Jul  7 21:30:13 2023, max compression
+gzip compressed data, was "threads-api-1.0.3.tar", last modified: Fri Jul  7 22:25:15 2023, max compression
```

## Comparing `threads-api-1.0.1.tar` & `threads-api-1.0.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-07 21:30:13.242602 threads-api-1.0.1/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     1068 2023-07-06 22:22:29.000000 threads-api-1.0.1/LICENSE
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      493 2023-07-07 21:30:13.242602 threads-api-1.0.1/PKG-INFO
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     9206 2023-07-07 21:26:44.000000 threads-api-1.0.1/README.md
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      349 2023-07-06 21:24:15.000000 threads-api-1.0.1/pyproject.toml
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       38 2023-07-07 21:30:13.242602 threads-api-1.0.1/setup.cfg
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      610 2023-07-07 21:30:11.000000 threads-api-1.0.1/setup.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-07 21:30:13.238602 threads-api-1.0.1/threads_api/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)        0 2023-07-06 20:59:49.000000 threads-api-1.0.1/threads_api/__init__.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-07 21:30:13.242602 threads-api-1.0.1/threads_api/src/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)        0 2023-07-06 21:13:21.000000 threads-api-1.0.1/threads_api/src/__init__.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)    15315 2023-07-07 21:21:06.000000 threads-api-1.0.1/threads_api/src/threads_api.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-07 21:30:13.242602 threads-api-1.0.1/threads_api/tests/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)        0 2023-07-06 21:19:18.000000 threads-api-1.0.1/threads_api/tests/__init__.py
--rwxrwxr-x   0 daniel    (1000) daniel    (1000)      404 2023-07-07 21:21:06.000000 threads-api-1.0.1/threads_api/tests/get_threads_test.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-07 21:30:13.242602 threads-api-1.0.1/threads_api.egg-info/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      493 2023-07-07 21:30:13.000000 threads-api-1.0.1/threads_api.egg-info/PKG-INFO
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      366 2023-07-07 21:30:13.000000 threads-api-1.0.1/threads_api.egg-info/SOURCES.txt
--rw-rw-r--   0 daniel    (1000) daniel    (1000)        1 2023-07-07 21:30:13.000000 threads-api-1.0.1/threads_api.egg-info/dependency_links.txt
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       17 2023-07-07 21:30:13.000000 threads-api-1.0.1/threads_api.egg-info/requires.txt
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       12 2023-07-07 21:30:13.000000 threads-api-1.0.1/threads_api.egg-info/top_level.txt
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-07 22:25:15.805283 threads-api-1.0.3/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     1068 2023-07-06 22:22:29.000000 threads-api-1.0.3/LICENSE
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     9732 2023-07-07 22:25:15.801283 threads-api-1.0.3/PKG-INFO
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     9206 2023-07-07 21:26:44.000000 threads-api-1.0.3/README.md
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      349 2023-07-06 21:24:15.000000 threads-api-1.0.3/pyproject.toml
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       38 2023-07-07 22:25:15.805283 threads-api-1.0.3/setup.cfg
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      787 2023-07-07 22:25:08.000000 threads-api-1.0.3/setup.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-07 22:25:15.801283 threads-api-1.0.3/threads_api/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)        0 2023-07-06 20:59:49.000000 threads-api-1.0.3/threads_api/__init__.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-07 22:25:15.801283 threads-api-1.0.3/threads_api/src/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)        0 2023-07-06 21:13:21.000000 threads-api-1.0.3/threads_api/src/__init__.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)    15315 2023-07-07 21:21:06.000000 threads-api-1.0.3/threads_api/src/threads_api.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-07 22:25:15.801283 threads-api-1.0.3/threads_api/tests/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)        0 2023-07-06 21:19:18.000000 threads-api-1.0.3/threads_api/tests/__init__.py
+-rwxrwxr-x   0 daniel    (1000) daniel    (1000)      404 2023-07-07 21:21:06.000000 threads-api-1.0.3/threads_api/tests/get_threads_test.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-07 22:25:15.801283 threads-api-1.0.3/threads_api.egg-info/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     9732 2023-07-07 22:25:15.000000 threads-api-1.0.3/threads_api.egg-info/PKG-INFO
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      366 2023-07-07 22:25:15.000000 threads-api-1.0.3/threads_api.egg-info/SOURCES.txt
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)        1 2023-07-07 22:25:15.000000 threads-api-1.0.3/threads_api.egg-info/dependency_links.txt
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       17 2023-07-07 22:25:15.000000 threads-api-1.0.3/threads_api.egg-info/requires.txt
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       12 2023-07-07 22:25:15.000000 threads-api-1.0.3/threads_api.egg-info/top_level.txt
```

### Comparing `threads-api-1.0.1/LICENSE` & `threads-api-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `threads-api-1.0.1/README.md` & `threads-api-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `threads-api-1.0.1/setup.py` & `threads-api-1.0.3/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,22 @@
 from setuptools import setup, find_packages
 
+with open('README.md', 'r', encoding='utf-8') as f:
+    long_description = f.read()
+
 setup(
     name='threads-api',
-    version='1.0.1',
+    version='1.0.3',
     description='Unofficial Python client for Meta Threads API',
+    long_description=long_description,
+    long_description_content_type='text/markdown',
     author='Danie1',
     author_email='',
     url='https://github.com/danie1/threads-api',
-    packages=find_packages(),
+    py_modules=find_packages(),
     install_requires=[
         'aiohttp',
         'requests',
     ],
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
```

### Comparing `threads-api-1.0.1/threads_api/src/threads_api.py` & `threads-api-1.0.3/threads_api/src/threads_api.py`

 * *Files identical despite different names*

