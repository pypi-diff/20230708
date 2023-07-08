# Comparing `tmp/samus-logging-0.1.77.tar.gz` & `tmp/samus-logging-0.1.86.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "samus-logging-0.1.77.tar", last modified: Fri Jul  7 22:51:28 2023, max compression
+gzip compressed data, was "samus-logging-0.1.86.tar", last modified: Sat Jul  8 10:03:03 2023, max compression
```

## Comparing `samus-logging-0.1.77.tar` & `samus-logging-0.1.86.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 samu      (1000) samu      (1000)        0 2023-07-07 22:51:28.358104 samus-logging-0.1.77/
--rw-rw-r--   0 samu      (1000) samu      (1000)        0 2023-06-28 14:33:05.000000 samus-logging-0.1.77/LICENSE
--rw-rw-r--   0 samu      (1000) samu      (1000)      389 2023-07-07 22:51:28.358104 samus-logging-0.1.77/PKG-INFO
--rw-rw-r--   0 samu      (1000) samu      (1000)        0 2023-06-28 14:33:21.000000 samus-logging-0.1.77/README.md
-drwxrwxr-x   0 samu      (1000) samu      (1000)        0 2023-07-07 22:51:28.358104 samus-logging-0.1.77/samus_logging/
--rw-rw-r--   0 samu      (1000) samu      (1000)       83 2023-07-07 22:03:29.000000 samus-logging-0.1.77/samus_logging/__init__.py
--rw-rw-r--   0 samu      (1000) samu      (1000)      446 2023-07-07 21:42:20.000000 samus-logging-0.1.77/samus_logging/level_filter.py
--rw-rw-r--   0 samu      (1000) samu      (1000)     4797 2023-07-07 21:57:53.000000 samus-logging-0.1.77/samus_logging/samus_logging.py
-drwxrwxr-x   0 samu      (1000) samu      (1000)        0 2023-07-07 22:51:28.358104 samus-logging-0.1.77/samus_logging.egg-info/
--rw-rw-r--   0 samu      (1000) samu      (1000)      389 2023-07-07 22:51:28.000000 samus-logging-0.1.77/samus_logging.egg-info/PKG-INFO
--rw-rw-r--   0 samu      (1000) samu      (1000)      303 2023-07-07 22:51:28.000000 samus-logging-0.1.77/samus_logging.egg-info/SOURCES.txt
--rw-rw-r--   0 samu      (1000) samu      (1000)        1 2023-07-07 22:51:28.000000 samus-logging-0.1.77/samus_logging.egg-info/dependency_links.txt
--rw-rw-r--   0 samu      (1000) samu      (1000)       20 2023-07-07 22:51:28.000000 samus-logging-0.1.77/samus_logging.egg-info/requires.txt
--rw-rw-r--   0 samu      (1000) samu      (1000)       14 2023-07-07 22:51:28.000000 samus-logging-0.1.77/samus_logging.egg-info/top_level.txt
--rw-rw-r--   0 samu      (1000) samu      (1000)       38 2023-07-07 22:51:28.358104 samus-logging-0.1.77/setup.cfg
--rw-rw-r--   0 samu      (1000) samu      (1000)      975 2023-07-07 20:39:48.000000 samus-logging-0.1.77/setup.py
+drwxrwxr-x   0 samu      (1000) samu      (1000)        0 2023-07-08 10:03:03.184050 samus-logging-0.1.86/
+-rw-rw-r--   0 samu      (1000) samu      (1000)        0 2023-06-28 14:33:05.000000 samus-logging-0.1.86/LICENSE
+-rw-rw-r--   0 samu      (1000) samu      (1000)      787 2023-07-08 10:03:03.184050 samus-logging-0.1.86/PKG-INFO
+-rw-rw-r--   0 samu      (1000) samu      (1000)      365 2023-07-08 09:46:06.000000 samus-logging-0.1.86/README.md
+drwxrwxr-x   0 samu      (1000) samu      (1000)        0 2023-07-08 10:03:03.184050 samus-logging-0.1.86/samus_logging/
+-rw-rw-r--   0 samu      (1000) samu      (1000)       83 2023-07-08 08:29:30.000000 samus-logging-0.1.86/samus_logging/__init__.py
+-rw-rw-r--   0 samu      (1000) samu      (1000)      473 2023-07-08 08:28:01.000000 samus-logging-0.1.86/samus_logging/level_filter.py
+-rw-rw-r--   0 samu      (1000) samu      (1000)     4797 2023-07-08 08:29:38.000000 samus-logging-0.1.86/samus_logging/samus_logging.py
+drwxrwxr-x   0 samu      (1000) samu      (1000)        0 2023-07-08 10:03:03.184050 samus-logging-0.1.86/samus_logging.egg-info/
+-rw-rw-r--   0 samu      (1000) samu      (1000)      787 2023-07-08 10:03:03.000000 samus-logging-0.1.86/samus_logging.egg-info/PKG-INFO
+-rw-rw-r--   0 samu      (1000) samu      (1000)      303 2023-07-08 10:03:03.000000 samus-logging-0.1.86/samus_logging.egg-info/SOURCES.txt
+-rw-rw-r--   0 samu      (1000) samu      (1000)        1 2023-07-08 10:03:03.000000 samus-logging-0.1.86/samus_logging.egg-info/dependency_links.txt
+-rw-rw-r--   0 samu      (1000) samu      (1000)       20 2023-07-08 10:03:03.000000 samus-logging-0.1.86/samus_logging.egg-info/requires.txt
+-rw-rw-r--   0 samu      (1000) samu      (1000)       14 2023-07-08 10:03:03.000000 samus-logging-0.1.86/samus_logging.egg-info/top_level.txt
+-rw-rw-r--   0 samu      (1000) samu      (1000)       38 2023-07-08 10:03:03.184050 samus-logging-0.1.86/setup.cfg
+-rw-rw-r--   0 samu      (1000) samu      (1000)     1014 2023-07-08 10:02:31.000000 samus-logging-0.1.86/setup.py
```

### Comparing `samus-logging-0.1.77/samus_logging/samus_logging.py` & `samus-logging-0.1.86/samus_logging/samus_logging.py`

 * *Files identical despite different names*

### Comparing `samus-logging-0.1.77/setup.py` & `samus-logging-0.1.86/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,36 +1,36 @@
-import os
 from pathlib import Path
 from setuptools import setup, find_packages
 
 
 def read_file(filepath: str) -> str | None:
     if Path(filepath).is_file():
         with open(filepath, 'r') as file:
             content = file.read().strip()
         file.close()
 
         if len(content) >= 1:
             return content
 
-    return None
+    return ''
 
 
 setup(
     name='samus-logging',
     version=read_file(f'VERSION'),
     python_requires='>=3.10',
     package_dir={'': '.'},
     packages=find_packages(where='.'),
     install_requires=[],
     extras_require={'dev': ['twine==4.0.2']},
 
     # license='',
     description='A minimal Logging-controller.',
     long_description=read_file('README.md'),
+    long_description_content_type='text/markdown',
     author='Samu Rabin',
     author_email='samu.ca.rabin@gmail.com',
     maintainer='Samu Rabin',
     maintainer_email='samu.ca.rabin@gmail.com',
     url='',
     # download_url=''
```

