# Comparing `tmp/seventv-1.1.1.tar.gz` & `tmp/seventv-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seventv-1.1.1.tar", last modified: Sat Jul  8 08:04:43 2023, max compression
+gzip compressed data, was "seventv-1.1.2.tar", last modified: Sat Jul  8 08:15:41 2023, max compression
```

## Comparing `seventv-1.1.1.tar` & `seventv-1.1.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-07-08 08:04:41.816975 seventv-1.1.1/
--rw-rw-rw-   0        0        0    35823 2023-07-08 06:31:19.000000 seventv-1.1.1/LICENSE
--rw-rw-rw-   0        0        0      436 2023-07-08 08:04:41.511124 seventv-1.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     2894 2023-07-08 07:47:49.000000 seventv-1.1.1/README.md
--rw-rw-rw-   0        0        0       42 2023-07-08 08:04:41.816975 seventv-1.1.1/setup.cfg
--rw-rw-rw-   0        0        0      559 2023-07-08 07:48:03.000000 seventv-1.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-08 08:04:41.407052 seventv-1.1.1/seventv.egg-info/
--rw-rw-rw-   0        0        0      436 2023-07-08 08:04:39.000000 seventv-1.1.1/seventv.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      180 2023-07-08 08:04:39.000000 seventv-1.1.1/seventv.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-08 08:04:39.000000 seventv-1.1.1/seventv.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-07-08 08:04:39.000000 seventv-1.1.1/seventv.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-07-08 08:04:39.000000 seventv-1.1.1/seventv.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-08 08:15:41.138136 seventv-1.1.2/
+-rw-rw-rw-   0        0        0    35823 2023-07-08 06:31:19.000000 seventv-1.1.2/LICENSE
+-rw-rw-rw-   0        0        0      436 2023-07-08 08:15:41.135141 seventv-1.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2894 2023-07-08 08:15:11.000000 seventv-1.1.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-08 08:15:41.139138 seventv-1.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      551 2023-07-08 08:14:55.000000 seventv-1.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-08 08:15:41.127127 seventv-1.1.2/seventv.egg-info/
+-rw-rw-rw-   0        0        0      436 2023-07-08 08:15:40.000000 seventv-1.1.2/seventv.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      180 2023-07-08 08:15:40.000000 seventv-1.1.2/seventv.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-08 08:15:40.000000 seventv-1.1.2/seventv.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-07-08 08:15:40.000000 seventv-1.1.2/seventv.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-07-08 08:15:40.000000 seventv-1.1.2/seventv.egg-info/top_level.txt
```

### Comparing `seventv-1.1.1/LICENSE` & `seventv-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `seventv-1.1.1/README.md` & `seventv-1.1.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 json
 ```
 ```
 pip install git+https://github.com/probablyjassin/sevenTVpy
 ```
 or
 ```
-pip install seventv==1.1.1
+pip install seventv==1.1.2
 ```
 
 # Usage
 To search for an emote and make use of the search results, do the following (asynchronously):
 - create a class instance of sevenTV
 - await the ```.emote_search``` method with your search query string and optional filters
 - don't forget to close the session at some later point, using ```.close()```.
```

### Comparing `seventv-1.1.1/setup.py` & `seventv-1.1.2/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from setuptools import setup
 
 setup(
     name='seventv',
-    version='1.1.1',
+    version='1.1.2',
     author='Jässin Aouani',
     author_email='jassin@aouani.de',
     description='An asynchronous API-wrapper for 7tv.app',
     packages=['seventv'],
-    install_requires=['json', 'aiohttp'],
+    install_requires=['aiohttp'],
     classifiers=[
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
     ],
```

