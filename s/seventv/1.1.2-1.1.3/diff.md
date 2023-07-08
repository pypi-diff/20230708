# Comparing `tmp/seventv-1.1.2.tar.gz` & `tmp/seventv-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seventv-1.1.2.tar", last modified: Sat Jul  8 08:15:41 2023, max compression
+gzip compressed data, was "seventv-1.1.3.tar", last modified: Sat Jul  8 09:28:52 2023, max compression
```

## Comparing `seventv-1.1.2.tar` & `seventv-1.1.3.tar`

### file list

```diff
@@ -1,12 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-07-08 08:15:41.138136 seventv-1.1.2/
--rw-rw-rw-   0        0        0    35823 2023-07-08 06:31:19.000000 seventv-1.1.2/LICENSE
--rw-rw-rw-   0        0        0      436 2023-07-08 08:15:41.135141 seventv-1.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     2894 2023-07-08 08:15:11.000000 seventv-1.1.2/README.md
--rw-rw-rw-   0        0        0       42 2023-07-08 08:15:41.139138 seventv-1.1.2/setup.cfg
--rw-rw-rw-   0        0        0      551 2023-07-08 08:14:55.000000 seventv-1.1.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-08 08:15:41.127127 seventv-1.1.2/seventv.egg-info/
--rw-rw-rw-   0        0        0      436 2023-07-08 08:15:40.000000 seventv-1.1.2/seventv.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      180 2023-07-08 08:15:40.000000 seventv-1.1.2/seventv.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-08 08:15:40.000000 seventv-1.1.2/seventv.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-07-08 08:15:40.000000 seventv-1.1.2/seventv.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-07-08 08:15:40.000000 seventv-1.1.2/seventv.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-08 09:28:52.185625 seventv-1.1.3/
+-rw-rw-rw-   0        0        0    35823 2023-07-08 06:31:19.000000 seventv-1.1.3/LICENSE
+-rw-rw-rw-   0        0        0      436 2023-07-08 09:28:52.164622 seventv-1.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2894 2023-07-08 08:15:11.000000 seventv-1.1.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-08 09:28:52.187623 seventv-1.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      566 2023-07-08 09:28:43.000000 seventv-1.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-08 09:28:52.041083 seventv-1.1.3/seventv/
+-rw-rw-rw-   0        0        0        0 2023-07-08 06:22:08.000000 seventv-1.1.3/seventv/__init__.py
+-rw-rw-rw-   0        0        0     3497 2023-07-08 07:10:57.000000 seventv-1.1.3/seventv/seventv.py
+drwxrwxrwx   0        0        0        0 2023-07-08 09:28:52.156632 seventv-1.1.3/seventv.egg-info/
+-rw-rw-rw-   0        0        0      436 2023-07-08 09:28:51.000000 seventv-1.1.3/seventv.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      219 2023-07-08 09:28:51.000000 seventv-1.1.3/seventv.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-08 09:28:51.000000 seventv-1.1.3/seventv.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-07-08 09:28:51.000000 seventv-1.1.3/seventv.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-07-08 09:28:51.000000 seventv-1.1.3/seventv.egg-info/top_level.txt
```

### Comparing `seventv-1.1.2/LICENSE` & `seventv-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `seventv-1.1.2/README.md` & `seventv-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `seventv-1.1.2/setup.py` & `seventv-1.1.3/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-from setuptools import setup
+from setuptools import setup, find_packages
 
 setup(
     name='seventv',
-    version='1.1.2',
+    version='1.1.3',
     author='Jässin Aouani',
     author_email='jassin@aouani.de',
     description='An asynchronous API-wrapper for 7tv.app',
     packages=['seventv'],
     install_requires=['aiohttp'],
     classifiers=[
         'Programming Language :: Python :: 3',
```

