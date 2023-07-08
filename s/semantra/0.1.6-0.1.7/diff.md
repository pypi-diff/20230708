# Comparing `tmp/semantra-0.1.6.tar.gz` & `tmp/semantra-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "semantra-0.1.6.tar", last modified: Sat Apr 29 15:53:21 2023, max compression
+gzip compressed data, was "semantra-0.1.7.tar", last modified: Sat Jul  8 14:50:10 2023, max compression
```

## Comparing `semantra-0.1.6.tar` & `semantra-0.1.7.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 freedmand   (501) staff       (20)        0 2023-04-29 15:53:21.553142 semantra-0.1.6/
--rw-r--r--   0 freedmand   (501) staff       (20)     1071 2023-03-31 03:28:18.000000 semantra-0.1.6/LICENSE
--rw-r--r--   0 freedmand   (501) staff       (20)    10690 2023-04-29 15:53:21.550984 semantra-0.1.6/PKG-INFO
--rw-r--r--   0 freedmand   (501) staff       (20)    10147 2023-04-29 15:53:11.000000 semantra-0.1.6/README.md
-drwxr-xr-x   0 freedmand   (501) staff       (20)        0 2023-04-29 15:53:21.529888 semantra-0.1.6/client/
-drwxr-xr-x   0 freedmand   (501) staff       (20)        0 2023-04-29 15:53:21.531758 semantra-0.1.6/client/public/
-drwxr-xr-x   0 freedmand   (501) staff       (20)        0 2023-04-29 15:53:21.534017 semantra-0.1.6/client/public/build/
--rw-r--r--   0 freedmand   (501) staff       (20)    14304 2023-04-29 13:52:26.000000 semantra-0.1.6/client/public/build/bundle.css
--rw-r--r--   0 freedmand   (501) staff       (20)   449103 2023-04-29 13:52:26.000000 semantra-0.1.6/client/public/build/bundle.js
--rw-r--r--   0 freedmand   (501) staff       (20)  1495745 2023-04-29 13:52:26.000000 semantra-0.1.6/client/public/build/bundle.js.map
--rw-r--r--   0 freedmand   (501) staff       (20)     3300 2023-04-09 04:23:49.000000 semantra-0.1.6/client/public/favicon.png
--rw-r--r--   0 freedmand   (501) staff       (20)      890 2023-02-15 22:52:41.000000 semantra-0.1.6/client/public/global.css
--rw-r--r--   0 freedmand   (501) staff       (20)      434 2023-04-29 13:52:21.000000 semantra-0.1.6/client/public/index.html
--rw-r--r--   0 freedmand   (501) staff       (20)     1020 2023-04-29 15:53:11.000000 semantra-0.1.6/pyproject.toml
--rw-r--r--   0 freedmand   (501) staff       (20)       38 2023-04-29 15:53:21.553207 semantra-0.1.6/setup.cfg
-drwxr-xr-x   0 freedmand   (501) staff       (20)        0 2023-04-29 15:53:21.530149 semantra-0.1.6/src/
-drwxr-xr-x   0 freedmand   (501) staff       (20)        0 2023-04-29 15:53:21.539080 semantra-0.1.6/src/semantra/
--rw-r--r--   0 freedmand   (501) staff       (20)        0 2023-04-23 04:39:23.000000 semantra-0.1.6/src/semantra/__init__.py
-drwxr-xr-x   0 freedmand   (501) staff       (20)        0 2023-04-29 15:53:21.542379 semantra-0.1.6/src/semantra/__pycache__/
--rw-r--r--   0 freedmand   (501) staff       (20)      148 2023-04-23 04:39:41.000000 semantra-0.1.6/src/semantra/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 freedmand   (501) staff       (20)    10961 2023-04-23 04:37:57.000000 semantra-0.1.6/src/semantra/__pycache__/models.cpython-39.pyc
--rw-r--r--   0 freedmand   (501) staff       (20)     3086 2023-04-23 04:37:58.000000 semantra-0.1.6/src/semantra/__pycache__/pdf.cpython-39.pyc
--rw-r--r--   0 freedmand   (501) staff       (20)    19561 2023-04-23 12:15:19.000000 semantra-0.1.6/src/semantra/__pycache__/semantra.cpython-39.pyc
--rw-r--r--   0 freedmand   (501) staff       (20)     4744 2023-04-23 04:37:58.000000 semantra-0.1.6/src/semantra/__pycache__/util.cpython-39.pyc
-drwxr-xr-x   0 freedmand   (501) staff       (20)        0 2023-04-29 15:53:21.543121 semantra-0.1.6/src/semantra/client_public/
-drwxr-xr-x   0 freedmand   (501) staff       (20)        0 2023-04-29 15:53:21.546116 semantra-0.1.6/src/semantra/client_public/build/
--rw-r--r--   0 freedmand   (501) staff       (20)    14304 2023-04-29 13:52:26.000000 semantra-0.1.6/src/semantra/client_public/build/bundle.css
--rw-r--r--   0 freedmand   (501) staff       (20)   449103 2023-04-29 13:52:26.000000 semantra-0.1.6/src/semantra/client_public/build/bundle.js
--rw-r--r--   0 freedmand   (501) staff       (20)  1495745 2023-04-29 13:52:26.000000 semantra-0.1.6/src/semantra/client_public/build/bundle.js.map
--rw-r--r--   0 freedmand   (501) staff       (20)     3300 2023-04-09 04:23:49.000000 semantra-0.1.6/src/semantra/client_public/favicon.png
--rw-r--r--   0 freedmand   (501) staff       (20)      890 2023-02-15 22:52:41.000000 semantra-0.1.6/src/semantra/client_public/global.css
--rw-r--r--   0 freedmand   (501) staff       (20)      434 2023-04-29 13:52:21.000000 semantra-0.1.6/src/semantra/client_public/index.html
--rw-r--r--   0 freedmand   (501) staff       (20)    11501 2023-04-29 13:52:21.000000 semantra-0.1.6/src/semantra/models.py
--rw-r--r--   0 freedmand   (501) staff       (20)     3325 2023-04-29 13:52:21.000000 semantra-0.1.6/src/semantra/pdf.py
--rw-r--r--   0 freedmand   (501) staff       (20)    29168 2023-04-29 15:53:11.000000 semantra-0.1.6/src/semantra/semantra.py
--rw-r--r--   0 freedmand   (501) staff       (20)     4524 2023-04-29 13:52:21.000000 semantra-0.1.6/src/semantra/util.py
-drwxr-xr-x   0 freedmand   (501) staff       (20)        0 2023-04-29 15:53:21.540312 semantra-0.1.6/src/semantra.egg-info/
--rw-r--r--   0 freedmand   (501) staff       (20)    10690 2023-04-29 15:53:21.000000 semantra-0.1.6/src/semantra.egg-info/PKG-INFO
--rw-r--r--   0 freedmand   (501) staff       (20)     1018 2023-04-29 15:53:21.000000 semantra-0.1.6/src/semantra.egg-info/SOURCES.txt
--rw-r--r--   0 freedmand   (501) staff       (20)        1 2023-04-29 15:53:21.000000 semantra-0.1.6/src/semantra.egg-info/dependency_links.txt
--rw-r--r--   0 freedmand   (501) staff       (20)       52 2023-04-29 15:53:21.000000 semantra-0.1.6/src/semantra.egg-info/entry_points.txt
--rw-r--r--   0 freedmand   (501) staff       (20)      176 2023-04-29 15:53:21.000000 semantra-0.1.6/src/semantra.egg-info/requires.txt
--rw-r--r--   0 freedmand   (501) staff       (20)        9 2023-04-29 15:53:21.000000 semantra-0.1.6/src/semantra.egg-info/top_level.txt
+drwxr-xr-x   0 freedmand   (501) staff       (20)        0 2023-07-08 14:50:10.501530 semantra-0.1.7/
+-rw-r--r--   0 freedmand   (501) staff       (20)     1071 2023-03-31 03:28:18.000000 semantra-0.1.7/LICENSE
+-rw-r--r--   0 freedmand   (501) staff       (20)    10818 2023-07-08 14:50:10.501264 semantra-0.1.7/PKG-INFO
+-rw-r--r--   0 freedmand   (501) staff       (20)    10275 2023-07-08 13:57:38.000000 semantra-0.1.7/README.md
+drwxr-xr-x   0 freedmand   (501) staff       (20)        0 2023-07-08 14:50:10.485736 semantra-0.1.7/client/
+drwxr-xr-x   0 freedmand   (501) staff       (20)        0 2023-07-08 14:50:10.488568 semantra-0.1.7/client/public/
+drwxr-xr-x   0 freedmand   (501) staff       (20)        0 2023-07-08 14:50:10.491191 semantra-0.1.7/client/public/build/
+-rw-r--r--   0 freedmand   (501) staff       (20)    14304 2023-07-08 13:57:37.000000 semantra-0.1.7/client/public/build/bundle.css
+-rw-r--r--   0 freedmand   (501) staff       (20)   449103 2023-07-08 13:57:37.000000 semantra-0.1.7/client/public/build/bundle.js
+-rw-r--r--   0 freedmand   (501) staff       (20)  1495745 2023-07-08 13:57:37.000000 semantra-0.1.7/client/public/build/bundle.js.map
+-rw-r--r--   0 freedmand   (501) staff       (20)     3300 2023-04-09 04:23:49.000000 semantra-0.1.7/client/public/favicon.png
+-rw-r--r--   0 freedmand   (501) staff       (20)      890 2023-02-15 22:52:41.000000 semantra-0.1.7/client/public/global.css
+-rw-r--r--   0 freedmand   (501) staff       (20)      434 2023-04-29 13:52:21.000000 semantra-0.1.7/client/public/index.html
+-rw-r--r--   0 freedmand   (501) staff       (20)     1020 2023-07-08 14:49:47.000000 semantra-0.1.7/pyproject.toml
+-rw-r--r--   0 freedmand   (501) staff       (20)       38 2023-07-08 14:50:10.501586 semantra-0.1.7/setup.cfg
+drwxr-xr-x   0 freedmand   (501) staff       (20)        0 2023-07-08 14:50:10.486234 semantra-0.1.7/src/
+drwxr-xr-x   0 freedmand   (501) staff       (20)        0 2023-07-08 14:50:10.495337 semantra-0.1.7/src/semantra/
+-rw-r--r--   0 freedmand   (501) staff       (20)        0 2023-04-23 04:39:23.000000 semantra-0.1.7/src/semantra/__init__.py
+drwxr-xr-x   0 freedmand   (501) staff       (20)        0 2023-07-08 14:50:10.498046 semantra-0.1.7/src/semantra/__pycache__/
+-rw-r--r--   0 freedmand   (501) staff       (20)      148 2023-04-23 04:39:41.000000 semantra-0.1.7/src/semantra/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 freedmand   (501) staff       (20)    11287 2023-07-08 14:32:51.000000 semantra-0.1.7/src/semantra/__pycache__/models.cpython-39.pyc
+-rw-r--r--   0 freedmand   (501) staff       (20)     3164 2023-07-08 14:02:14.000000 semantra-0.1.7/src/semantra/__pycache__/pdf.cpython-39.pyc
+-rw-r--r--   0 freedmand   (501) staff       (20)    20095 2023-07-08 14:46:06.000000 semantra-0.1.7/src/semantra/__pycache__/semantra.cpython-39.pyc
+-rw-r--r--   0 freedmand   (501) staff       (20)     4744 2023-07-08 14:02:14.000000 semantra-0.1.7/src/semantra/__pycache__/util.cpython-39.pyc
+drwxr-xr-x   0 freedmand   (501) staff       (20)        0 2023-07-08 14:50:10.498672 semantra-0.1.7/src/semantra/client_public/
+drwxr-xr-x   0 freedmand   (501) staff       (20)        0 2023-07-08 14:50:10.499625 semantra-0.1.7/src/semantra/client_public/build/
+-rw-r--r--   0 freedmand   (501) staff       (20)    14304 2023-07-08 13:57:37.000000 semantra-0.1.7/src/semantra/client_public/build/bundle.css
+-rw-r--r--   0 freedmand   (501) staff       (20)   449103 2023-07-08 13:57:37.000000 semantra-0.1.7/src/semantra/client_public/build/bundle.js
+-rw-r--r--   0 freedmand   (501) staff       (20)  1495745 2023-07-08 13:57:37.000000 semantra-0.1.7/src/semantra/client_public/build/bundle.js.map
+-rw-r--r--   0 freedmand   (501) staff       (20)     3300 2023-04-09 04:23:49.000000 semantra-0.1.7/src/semantra/client_public/favicon.png
+-rw-r--r--   0 freedmand   (501) staff       (20)      890 2023-02-15 22:52:41.000000 semantra-0.1.7/src/semantra/client_public/global.css
+-rw-r--r--   0 freedmand   (501) staff       (20)      434 2023-04-29 13:52:21.000000 semantra-0.1.7/src/semantra/client_public/index.html
+-rw-r--r--   0 freedmand   (501) staff       (20)    11577 2023-07-08 14:49:47.000000 semantra-0.1.7/src/semantra/models.py
+-rw-r--r--   0 freedmand   (501) staff       (20)     3325 2023-07-08 13:57:37.000000 semantra-0.1.7/src/semantra/pdf.py
+-rw-r--r--   0 freedmand   (501) staff       (20)    29784 2023-07-08 14:49:47.000000 semantra-0.1.7/src/semantra/semantra.py
+-rw-r--r--   0 freedmand   (501) staff       (20)     4524 2023-07-08 13:57:37.000000 semantra-0.1.7/src/semantra/util.py
+drwxr-xr-x   0 freedmand   (501) staff       (20)        0 2023-07-08 14:50:10.496630 semantra-0.1.7/src/semantra.egg-info/
+-rw-r--r--   0 freedmand   (501) staff       (20)    10818 2023-07-08 14:50:10.000000 semantra-0.1.7/src/semantra.egg-info/PKG-INFO
+-rw-r--r--   0 freedmand   (501) staff       (20)     1018 2023-07-08 14:50:10.000000 semantra-0.1.7/src/semantra.egg-info/SOURCES.txt
+-rw-r--r--   0 freedmand   (501) staff       (20)        1 2023-07-08 14:50:10.000000 semantra-0.1.7/src/semantra.egg-info/dependency_links.txt
+-rw-r--r--   0 freedmand   (501) staff       (20)       52 2023-07-08 14:50:10.000000 semantra-0.1.7/src/semantra.egg-info/entry_points.txt
+-rw-r--r--   0 freedmand   (501) staff       (20)      176 2023-07-08 14:50:10.000000 semantra-0.1.7/src/semantra.egg-info/requires.txt
+-rw-r--r--   0 freedmand   (501) staff       (20)        9 2023-07-08 14:50:10.000000 semantra-0.1.7/src/semantra.egg-info/top_level.txt
```

### Comparing `semantra-0.1.6/LICENSE` & `semantra-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `semantra-0.1.6/PKG-INFO` & `semantra-0.1.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: semantra
-Version: 0.1.6
+Version: 0.1.7
 Summary: A semantic search CLI tool
 Author-email: Dylan Freedman <freedmand@gmail.com>
 Project-URL: Homepage, https://github.com/freedmand/semantra
 Project-URL: Repository, https://github.com/freedmand/semantra
 Project-URL: Bug Tracker, https://github.com/freedmand/semantra/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -20,20 +20,20 @@
 
 The tool, made to run on the command line, analyzes specified text and PDF files on your computer and launches a local web search application for interactively querying them. The purpose of Semantra is to make running a specialized semantic search engine easy, friendly, configurable, and private/secure.
 
 Semantra is built for individuals seeking needles in haystacks — journalists sifting through leaked documents on deadline, researchers seeking insights within papers, students engaging with literature by querying themes, historians connecting events across books, and so forth.
 
 ## Resources
 
-- [Tutorial](docs/tutorial.md): a gentle introduction to getting started with Semantra — everything from installing the tool to hands-on examples of analyzing documents with it
+- [Tutorial](docs/tutorial.md): a gentle introduction to getting started with Semantra — everything from installing the tool to hands-on examples of analyzing documents with it
 - [Guides](docs/guides.md): practical guides on how to do more with Semantra
 - [Concepts](docs/concepts.md): Explainers on some concepts to better understand how Semantra works
 - [Using the web interface](docs/help.md): A reference on how to use the Semantra web app
 
-This page gives a high-level overview of Semantra and a reference of its features.
+This page gives a high-level overview of Semantra and a reference of its features. It's also available in other languages: [Semantra en español](docs/README_es.md), [Semantra 中文说明](docs/README_zh-CN.md)
 
 ## Installation
 
 Ensure you have [Python >= 3.9](https://www.python.org/downloads/).
 
 The easiest way to install Semantra is via `pipx`. If you do not have `pipx` installed, run:
```

### Comparing `semantra-0.1.6/README.md` & `semantra-0.1.7/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,20 +6,20 @@
 
 The tool, made to run on the command line, analyzes specified text and PDF files on your computer and launches a local web search application for interactively querying them. The purpose of Semantra is to make running a specialized semantic search engine easy, friendly, configurable, and private/secure.
 
 Semantra is built for individuals seeking needles in haystacks — journalists sifting through leaked documents on deadline, researchers seeking insights within papers, students engaging with literature by querying themes, historians connecting events across books, and so forth.
 
 ## Resources
 
-- [Tutorial](docs/tutorial.md): a gentle introduction to getting started with Semantra — everything from installing the tool to hands-on examples of analyzing documents with it
+- [Tutorial](docs/tutorial.md): a gentle introduction to getting started with Semantra — everything from installing the tool to hands-on examples of analyzing documents with it
 - [Guides](docs/guides.md): practical guides on how to do more with Semantra
 - [Concepts](docs/concepts.md): Explainers on some concepts to better understand how Semantra works
 - [Using the web interface](docs/help.md): A reference on how to use the Semantra web app
 
-This page gives a high-level overview of Semantra and a reference of its features.
+This page gives a high-level overview of Semantra and a reference of its features. It's also available in other languages: [Semantra en español](docs/README_es.md), [Semantra 中文说明](docs/README_zh-CN.md)
 
 ## Installation
 
 Ensure you have [Python >= 3.9](https://www.python.org/downloads/).
 
 The easiest way to install Semantra is via `pipx`. If you do not have `pipx` installed, run:
```

### Comparing `semantra-0.1.6/client/public/build/bundle.css` & `semantra-0.1.7/client/public/build/bundle.css`

 * *Files identical despite different names*

### Comparing `semantra-0.1.6/client/public/build/bundle.js` & `semantra-0.1.7/client/public/build/bundle.js`

 * *Files identical despite different names*

### Comparing `semantra-0.1.6/client/public/build/bundle.js.map` & `semantra-0.1.7/client/public/build/bundle.js.map`

 * *Files identical despite different names*

### Comparing `semantra-0.1.6/client/public/favicon.png` & `semantra-0.1.7/client/public/favicon.png`

 * *Files identical despite different names*

### Comparing `semantra-0.1.6/client/public/global.css` & `semantra-0.1.7/client/public/global.css`

 * *Files identical despite different names*

### Comparing `semantra-0.1.6/pyproject.toml` & `semantra-0.1.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "semantra"
-version = "0.1.6"
+version = "0.1.7"
 description = "A semantic search CLI tool"
 authors = [{name = "Dylan Freedman", email = "freedmand@gmail.com"}]
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
```

### Comparing `semantra-0.1.6/src/semantra/__pycache__/models.cpython-39.pyc` & `semantra-0.1.7/src/semantra/__pycache__/models.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Apr 20 17:02:30 2023 UTC, .py size: 11172 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 14% similar despite different names*

```diff
@@ -1,686 +1,706 @@
-00000000: 610d 0d0a 0000 0000 2670 4164 a42b 0000  a.......&pAd.+..
+00000000: 610d 0d0a 0000 0000 f66d a964 392d 0000  a........m.d9-..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0008 0000 0040 0000 0073 2201 0000 6400  .....@...s"...d.
+00000020: 0008 0000 0040 0000 0073 1e01 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
-00000040: 6d03 5a03 0100 6400 6403 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
-00000050: 6d06 5a06 0100 6400 6401 6c07 5a07 6400  m.Z...d.d.l.Z.d.
-00000060: 6401 6c08 5a09 6400 6401 6c0a 5a0a 6400  d.l.Z.d.d.l.Z.d.
-00000070: 6404 6c0b 6d0c 5a0c 0100 6400 6401 6c0d  d.l.m.Z...d.d.l.
-00000080: 5a0d 650c 8300 0100 6405 650d 6a0e 7600  Z.e.....d.e.j.v.
-00000090: 7270 650d a00f 6405 a101 650a 5f10 6406  rpe...d...e._.d.
-000000a0: 5a11 6407 5a12 6408 5a13 6409 5a14 640a  Z.d.Z.d.Z.d.Z.d.
-000000b0: 640b 8400 5a15 640c 640d 8400 5a16 640e  d...Z.d.d...Z.d.
-000000c0: 640f 8400 5a17 4700 6410 6411 8400 6411  d...Z.G.d.d...d.
-000000d0: 6502 8303 5a18 4700 6412 6413 8400 6413  e...Z.G.d.d...d.
-000000e0: 6518 8303 5a19 6414 6415 8400 5a1a 4700  e...Z.d.d...Z.G.
-000000f0: 6416 6417 8400 6417 6518 8303 5a1b 6418  d.d...d.e...Z.d.
-00000100: 6419 641a 641b 641c 8400 641d 9c04 6401  d.d.d.d...d...d.
-00000110: 6419 641e 641c 8400 641f 9c03 6401 6420  d.d.d...d...d.d 
-00000120: 6421 641c 8400 641f 9c03 6401 6422 6423  d!d...d...d.d"d#
-00000130: 641c 8400 641f 9c03 6401 6424 6425 641c  d...d...d.d$d%d.
-00000140: 8400 641f 9c03 6426 9c05 5a1c 6401 5300  ..d...d&..Z.d.S.
-00000150: 2927 e900 0000 004e 2902 da03 4142 43da  )'.....N)...ABC.
-00000160: 0e61 6273 7472 6163 746d 6574 686f 6429  .abstractmethod)
-00000170: 02da 0d41 7574 6f54 6f6b 656e 697a 6572  ...AutoTokenizer
-00000180: da09 4175 746f 4d6f 6465 6c29 01da 0b6c  ..AutoModel)...l
-00000190: 6f61 645f 646f 7465 6e76 5a0e 4f50 454e  oad_dotenvZ.OPEN
-000001a0: 4149 5f41 5049 5f4b 4559 7a26 7365 6e74  AI_API_KEYz&sent
-000001b0: 656e 6365 2d74 7261 6e73 666f 726d 6572  ence-transformer
-000001c0: 732f 616c 6c2d 4d69 6e69 4c4d 2d4c 362d  s/all-MiniLM-L6-
-000001d0: 7632 7a27 7365 6e74 656e 6365 2d74 7261  v2z'sentence-tra
-000001e0: 6e73 666f 726d 6572 732f 616c 6c2d 6d70  nsformers/all-mp
-000001f0: 6e65 742d 6261 7365 2d76 327a 374d 7565  net-base-v2z7Mue
-00000200: 6e6e 6967 686f 6666 2f53 4750 542d 3132  nnighoff/SGPT-12
-00000210: 354d 2d77 6569 6768 7465 646d 6561 6e2d  5M-weightedmean-
-00000220: 6d73 6d61 7263 6f2d 7370 6563 622d 6269  msmarco-specb-bi
-00000230: 7466 6974 7a37 4d75 656e 6e69 6768 6f66  tfitz7Muennighof
-00000240: 662f 5347 5054 2d31 2e33 422d 7765 6967  f/SGPT-1.3B-weig
-00000250: 6874 6564 6d65 616e 2d6d 736d 6172 636f  htedmean-msmarco
-00000260: 2d73 7065 6362 2d62 6974 6669 7463 0200  -specb-bitfitc..
-00000270: 0000 0000 0000 0000 0000 0600 0000 0400  ................
-00000280: 0000 4300 0000 734c 0000 007c 0064 0119  ..C...sL...|.d..
-00000290: 007d 027c 01a0 0064 02a1 01a0 017c 02a0  .}.|...d.....|..
-000002a0: 02a1 00a1 01a0 03a1 007d 0374 04a0 057c  .........}.t...|
-000002b0: 027c 0314 0064 03a1 027d 0474 046a 067c  .|...d...}.t.j.|
-000002c0: 03a0 0564 03a1 0164 0464 058d 027d 057c  ...d...d.d...}.|
-000002d0: 047c 051b 0053 0029 064e 7201 0000 00e9  .|...S.).Nr.....
-000002e0: ffff ffff e901 0000 0067 95d6 26e8 0b2e  .........g..&...
-000002f0: 113e 2901 da03 6d69 6e29 075a 0975 6e73  .>)...min).Z.uns
-00000300: 7175 6565 7a65 da06 6578 7061 6e64 da04  queeze..expand..
-00000310: 7369 7a65 da05 666c 6f61 74da 0574 6f72  size..float..tor
-00000320: 6368 da03 7375 6dda 0563 6c61 6d70 2906  ch..sum..clamp).
-00000330: da0c 6d6f 6465 6c5f 6f75 7470 7574 da0e  ..model_output..
-00000340: 6174 7465 6e74 696f 6e5f 6d61 736b 5a10  attention_maskZ.
-00000350: 746f 6b65 6e5f 656d 6265 6464 696e 6773  token_embeddings
-00000360: 5a13 696e 7075 745f 6d61 736b 5f65 7870  Z.input_mask_exp
-00000370: 616e 6465 645a 0e73 756d 5f65 6d62 6564  andedZ.sum_embed
-00000380: 6469 6e67 735a 0873 756d 5f6d 6173 6ba9  dingsZ.sum_mask.
-00000390: 0072 1200 0000 fa37 2f55 7365 7273 2f66  .r.....7/Users/f
-000003a0: 7265 6564 6d61 6e64 2f73 6372 6170 732f  reedmand/scraps/
-000003b0: 7365 6d61 6e74 7261 2f73 7263 2f73 656d  semantra/src/sem
-000003c0: 616e 7472 612f 6d6f 6465 6c73 2e70 79da  antra/models.py.
-000003d0: 0c6d 6561 6e5f 706f 6f6c 696e 6716 0000  .mean_pooling...
-000003e0: 0073 1000 0000 0001 0201 02ff 0404 16ff  .s..............
-000003f0: 0203 1001 1401 7214 0000 0063 0100 0000  ......r....c....
-00000400: 0000 0000 0000 0000 0100 0000 0200 0000  ................
-00000410: 4300 0000 730e 0000 0064 0164 0284 007c  C...s....d.d...|
-00000420: 0044 0083 0153 0029 034e 6301 0000 0000  .D...S.).Nc.....
-00000430: 0000 0000 0000 0002 0000 0004 0000 0053  ...............S
-00000440: 0000 0073 1800 0000 6700 7c00 5d10 7d01  ...s....g.|.].}.
-00000450: 7c01 6400 7501 7204 7c01 9102 7104 5300  |.d.u.r.|...q.S.
-00000460: a901 4e72 1200 0000 2902 da02 2e30 da01  ..Nr....)....0..
-00000470: 6972 1200 0000 7212 0000 0072 1300 0000  ir....r....r....
-00000480: da0a 3c6c 6973 7463 6f6d 703e 2300 0000  ..<listcomp>#...
-00000490: f300 0000 007a 1f66 696c 7465 725f 6e6f  .....z.filter_no
-000004a0: 6e65 2e3c 6c6f 6361 6c73 3e2e 3c6c 6973  ne.<locals>.<lis
-000004b0: 7463 6f6d 703e 7212 0000 00a9 01da 0178  tcomp>r........x
-000004c0: 7212 0000 0072 1200 0000 7213 0000 00da  r....r....r.....
-000004d0: 0b66 696c 7465 725f 6e6f 6e65 2200 0000  .filter_none"...
-000004e0: 7302 0000 0000 0172 1c00 0000 6301 0000  s......r....c...
-000004f0: 0000 0000 0000 0000 0001 0000 0003 0000  ................
-00000500: 0043 0000 0073 1c00 0000 7400 7c00 7401  .C...s....t.|.t.
-00000510: 6a02 8302 7218 7c00 a003 a100 a004 a100  j...r.|.........
-00000520: 5300 7c00 5300 7215 0000 0029 05da 0a69  S.|.S.r....)...i
-00000530: 7369 6e73 7461 6e63 6572 0d00 0000 5a06  sinstancer....Z.
-00000540: 5465 6e73 6f72 da03 6370 75da 056e 756d  Tensor..cpu..num
-00000550: 7079 721a 0000 0072 1200 0000 7212 0000  pyr....r....r...
-00000560: 0072 1300 0000 da08 6173 5f6e 756d 7079  .r......as_numpy
-00000570: 2600 0000 7306 0000 0000 020c 010c 0172  &...s..........r
-00000580: 2000 0000 6300 0000 0000 0000 0000 0000   ...c...........
-00000590: 0000 0000 0005 0000 0040 0000 0073 b400  .........@...s..
-000005a0: 0000 6500 5a01 6400 5a02 6503 6504 6401  ..e.Z.d.Z.e.e.d.
-000005b0: 9c01 6402 6403 8404 8301 5a05 6503 6506  ..d.d.....Z.e.e.
-000005c0: 6404 9c01 6405 6406 8404 8301 5a07 6503  d...d.d.....Z.e.
-000005d0: 6504 6401 9c01 6407 6408 8404 8301 5a08  e.d...d.d.....Z.
-000005e0: 6503 6506 6409 640a 9c02 640b 640c 8404  e.e.d.d...d.d...
-000005f0: 8301 5a09 6503 640d 640e 8400 8301 5a0a  ..Z.e.d.d.....Z.
-00000600: 6503 6421 650b 6410 6411 9c02 6412 6413  e.d!e.d.d...d.d.
-00000610: 8405 8301 5a0c 6414 6401 9c01 6415 6416  ....Z.d.d...d.d.
-00000620: 8404 5a0d 6506 6414 6417 9c02 6418 6419  ..Z.e.d.d...d.d.
-00000630: 8404 5a0e 6414 6401 9c01 641a 641b 8404  ..Z.d.d...d.d...
-00000640: 5a0f 641c 641d 8400 5a10 641e 641f 8400  Z.d.d...Z.d.d...
-00000650: 5a11 6420 5300 2922 da09 4261 7365 4d6f  Z.d S.)"..BaseMo
-00000660: 6465 6ca9 01da 0672 6574 7572 6e63 0100  del....returnc..
-00000670: 0000 0000 0000 0000 0000 0100 0000 0100  ................
-00000680: 0000 4300 0000 7304 0000 0064 0053 0072  ..C...s....d.S.r
-00000690: 1500 0000 7212 0000 00a9 01da 0473 656c  ....r........sel
-000006a0: 6672 1200 0000 7212 0000 0072 1300 0000  fr....r....r....
-000006b0: da12 6765 745f 6e75 6d5f 6469 6d65 6e73  ..get_num_dimens
-000006c0: 696f 6e73 2e00 0000 7302 0000 0000 027a  ions....s......z
-000006d0: 1c42 6173 654d 6f64 656c 2e67 6574 5f6e  .BaseModel.get_n
-000006e0: 756d 5f64 696d 656e 7369 6f6e 73a9 01da  um_dimensions...
-000006f0: 0474 6578 7463 0200 0000 0000 0000 0000  .textc..........
-00000700: 0000 0200 0000 0100 0000 4300 0000 7304  ..........C...s.
-00000710: 0000 0064 0053 0072 1500 0000 7212 0000  ...d.S.r....r...
-00000720: 00a9 0272 2500 0000 7228 0000 0072 1200  ...r%...r(...r..
-00000730: 0000 7212 0000 0072 1300 0000 da0a 6765  ..r....r......ge
-00000740: 745f 746f 6b65 6e73 3200 0000 7302 0000  t_tokens2...s...
-00000750: 0000 027a 1442 6173 654d 6f64 656c 2e67  ...z.BaseModel.g
-00000760: 6574 5f74 6f6b 656e 7363 0200 0000 0000  et_tokensc......
-00000770: 0000 0000 0000 0200 0000 0100 0000 4300  ..............C.
-00000780: 0000 7304 0000 0064 0053 0072 1500 0000  ..s....d.S.r....
-00000790: 7212 0000 00a9 0272 2500 0000 da06 746f  r......r%.....to
-000007a0: 6b65 6e73 7212 0000 0072 1200 0000 7213  kensr....r....r.
-000007b0: 0000 00da 1067 6574 5f74 6f6b 656e 5f6c  .....get_token_l
-000007c0: 656e 6774 6836 0000 0073 0200 0000 0002  ength6...s......
-000007d0: 7a1a 4261 7365 4d6f 6465 6c2e 6765 745f  z.BaseModel.get_
-000007e0: 746f 6b65 6e5f 6c65 6e67 7468 fa09 6c69  token_length..li
-000007f0: 7374 5b73 7472 5da9 0272 2800 0000 7223  st[str]..r(...r#
-00000800: 0000 0063 0300 0000 0000 0000 0000 0000  ...c............
-00000810: 0300 0000 0100 0000 4300 0000 7304 0000  ........C...s...
-00000820: 0064 0053 0072 1500 0000 7212 0000 0029  .d.S.r....r....)
-00000830: 0372 2500 0000 7228 0000 0072 2c00 0000  .r%...r(...r,...
-00000840: 7212 0000 0072 1200 0000 7213 0000 00da  r....r....r.....
-00000850: 0f67 6574 5f74 6578 745f 6368 756e 6b73  .get_text_chunks
-00000860: 3a00 0000 7302 0000 0000 027a 1942 6173  :...s......z.Bas
-00000870: 654d 6f64 656c 2e67 6574 5f74 6578 745f  eModel.get_text_
-00000880: 6368 756e 6b73 6301 0000 0000 0000 0000  chunksc.........
-00000890: 0000 0001 0000 0001 0000 0043 0000 0073  ...........C...s
-000008a0: 0400 0000 6400 5300 7215 0000 0072 1200  ....d.S.r....r..
-000008b0: 0000 7224 0000 0072 1200 0000 7212 0000  ..r$...r....r...
-000008c0: 0072 1300 0000 da0a 6765 745f 636f 6e66  .r......get_conf
-000008d0: 6967 3e00 0000 7302 0000 0000 027a 1442  ig>...s......z.B
-000008e0: 6173 654d 6f64 656c 2e67 6574 5f63 6f6e  aseModel.get_con
-000008f0: 6669 6746 fa11 6c69 7374 5b6c 6973 745b  figF..list[list[
-00000900: 666c 6f61 745d 5d29 02da 0869 735f 7175  float]])...is_qu
-00000910: 6572 7972 2300 0000 6304 0000 0000 0000  eryr#...c.......
-00000920: 0000 0000 0004 0000 0001 0000 0043 0000  .............C..
-00000930: 0073 0400 0000 6400 5300 7215 0000 0072  .s....d.S.r....r
-00000940: 1200 0000 2904 7225 0000 0072 2c00 0000  ....).r%...r,...
-00000950: da07 6f66 6673 6574 7372 3300 0000 7212  ..offsetsr3...r.
-00000960: 0000 0072 1200 0000 7213 0000 00da 0565  ...r....r......e
-00000970: 6d62 6564 4200 0000 7302 0000 0000 027a  mbedB...s......z
-00000980: 0f42 6173 654d 6f64 656c 2e65 6d62 6564  .BaseModel.embed
-00000990: 7a0b 6c69 7374 5b66 6c6f 6174 5d63 0200  z.list[float]c..
-000009a0: 0000 0000 0000 0000 0000 0300 0000 0700  ................
-000009b0: 0000 4300 0000 7328 0000 007c 00a0 007c  ..C...s(...|...|
-000009c0: 01a1 017d 027c 00a0 017c 0264 017c 00a0  ...}.|...|.d.|..
-000009d0: 027c 02a1 0166 0267 0164 02a1 0364 0119  .|...f.g.d...d..
-000009e0: 0053 0029 034e 7201 0000 0046 a903 722a  .S.).Nr....F..r*
-000009f0: 0000 0072 3500 0000 722d 0000 0029 0372  ...r5...r-...).r
-00000a00: 2500 0000 5a08 646f 6375 6d65 6e74 722c  %...Z.documentr,
-00000a10: 0000 0072 1200 0000 7212 0000 0072 1300  ...r....r....r..
-00000a20: 0000 da0e 656d 6265 645f 646f 6375 6d65  ....embed_docume
-00000a30: 6e74 4600 0000 7304 0000 0000 010a 017a  ntF...s........z
-00000a40: 1842 6173 654d 6f64 656c 2e65 6d62 6564  .BaseModel.embed
-00000a50: 5f64 6f63 756d 656e 7429 02da 0571 7565  _document)...que
-00000a60: 7279 7223 0000 0063 0200 0000 0000 0000  ryr#...c........
-00000a70: 0000 0000 0300 0000 0700 0000 4300 0000  ............C...
-00000a80: 7328 0000 007c 00a0 007c 01a1 017d 027c  s(...|...|...}.|
-00000a90: 00a0 017c 0264 017c 00a0 027c 02a1 0166  ...|.d.|...|...f
-00000aa0: 0267 0164 02a1 0364 0119 0053 0029 034e  .g.d...d...S.).N
-00000ab0: 7201 0000 0054 7236 0000 0029 0372 2500  r....Tr6...).r%.
-00000ac0: 0000 7238 0000 0072 2c00 0000 7212 0000  ..r8...r,...r...
-00000ad0: 0072 1200 0000 7213 0000 00da 0b65 6d62  .r....r......emb
-00000ae0: 6564 5f71 7565 7279 4a00 0000 7304 0000  ed_queryJ...s...
-00000af0: 0000 010a 017a 1542 6173 654d 6f64 656c  .....z.BaseModel
-00000b00: 2e65 6d62 6564 5f71 7565 7279 6302 0000  .embed_queryc...
-00000b10: 0000 0000 0000 0000 0003 0000 0004 0000  ................
-00000b20: 0003 0000 0073 2000 0000 8700 6601 6401  .....s .....f.d.
-00000b30: 6402 8408 7c01 4400 8301 7d02 7400 6a01  d...|.D...}.t.j.
-00000b40: 7c02 6403 6404 8d02 5300 2905 4e63 0100  |.d.d...S.).Nc..
-00000b50: 0000 0000 0000 0000 0000 0200 0000 0700  ................
-00000b60: 0000 1300 0000 7326 0000 0067 007c 005d  ......s&...g.|.]
-00000b70: 1e7d 0174 0088 00a0 017c 0164 0019 00a1  .}.t.....|.d....
-00000b80: 0183 017c 0164 0119 0014 0091 0271 0453  ...|.d.......q.S
-00000b90: 0029 0272 3800 0000 da06 7765 6967 6874  .).r8.....weight
-00000ba0: 2902 7220 0000 0072 3900 0000 2902 7216  ).r ...r9...).r.
-00000bb0: 0000 0072 3800 0000 7224 0000 0072 1200  ...r8...r$...r..
-00000bc0: 0000 7213 0000 0072 1800 0000 4f00 0000  ..r....r....O...
-00000bd0: 7304 0000 0006 0202 ff7a 2b42 6173 654d  s........z+BaseM
-00000be0: 6f64 656c 2e65 6d62 6564 5f71 7565 7269  odel.embed_queri
-00000bf0: 6573 2e3c 6c6f 6361 6c73 3e2e 3c6c 6973  es.<locals>.<lis
-00000c00: 7463 6f6d 703e 7201 0000 00a9 01da 0461  tcomp>r........a
-00000c10: 7869 7329 02da 026e 7072 0e00 0000 2903  xis)...npr....).
-00000c20: 7225 0000 00da 0771 7565 7269 6573 5a0e  r%.....queriesZ.
-00000c30: 616c 6c5f 656d 6265 6464 696e 6773 7212  all_embeddingsr.
-00000c40: 0000 0072 2400 0000 7213 0000 00da 0d65  ...r$...r......e
-00000c50: 6d62 6564 5f71 7565 7269 6573 4e00 0000  mbed_queriesN...
-00000c60: 7308 0000 0000 010a 0202 fe06 057a 1742  s............z.B
-00000c70: 6173 654d 6f64 656c 2e65 6d62 6564 5f71  aseModel.embed_q
-00000c80: 7565 7269 6573 6304 0000 0000 0000 0000  ueriesc.........
-00000c90: 0000 0005 0000 0005 0000 0003 0000 0073  ...............s
-00000ca0: 4c00 0000 7400 7c01 8301 6401 6b04 7216  L...t.|...d.k.r.
-00000cb0: 7c00 a001 7c01 a101 6e02 6400 7d04 7402  |...|...n.d.}.t.
-00000cc0: 6a03 6700 7c04 6400 7501 722e 7c04 6701  j.g.|.d.u.r.|.g.
-00000cd0: 6e02 6700 a201 8700 6601 6402 6403 8408  n.g.....f.d.d...
-00000ce0: 7c02 4400 8301 a201 6401 6404 8d02 5300  |.D.....d.d...S.
-00000cf0: 2905 4e72 0100 0000 6301 0000 0000 0000  ).Nr....c.......
-00000d00: 0000 0000 0002 0000 0005 0000 0013 0000  ................
-00000d10: 0073 3200 0000 6700 7c00 5d2a 7d01 8800  .s2...g.|.]*}...
-00000d20: 7c01 6400 1900 6401 1900 1900 6a00 7c01  |.d...d.....j.|.
-00000d30: 6402 1900 6403 1900 1900 7c01 6404 1900  d...d.....|.d...
-00000d40: 1400 9102 7104 5300 2905 da04 6669 6c65  ....q.S.)...file
-00000d50: da08 6669 6c65 6e61 6d65 5a0c 7365 6172  ..filenameZ.sear
-00000d60: 6368 5265 7375 6c74 da05 696e 6465 7872  chResult..indexr
-00000d70: 3a00 0000 2901 da0a 656d 6265 6464 696e  :...)...embeddin
-00000d80: 6773 2902 7216 0000 005a 0470 7265 66a9  gs).r....Z.pref.
-00000d90: 01da 0964 6f63 756d 656e 7473 7212 0000  ...documentsr...
-00000da0: 0072 1300 0000 7218 0000 005c 0000 0073  .r....r....\...s
-00000db0: 0c00 0000 0605 02fc 1001 0aff 0203 06fd  ................
-00000dc0: 7a3b 4261 7365 4d6f 6465 6c2e 656d 6265  z;BaseModel.embe
-00000dd0: 645f 7175 6572 6965 735f 616e 645f 7072  d_queries_and_pr
-00000de0: 6566 6572 656e 6365 732e 3c6c 6f63 616c  eferences.<local
-00000df0: 733e 2e3c 6c69 7374 636f 6d70 3e72 3b00  s>.<listcomp>r;.
-00000e00: 0000 2904 da03 6c65 6e72 3f00 0000 723d  ..)...lenr?...r=
-00000e10: 0000 0072 0e00 0000 2905 7225 0000 0072  ...r....).r%...r
-00000e20: 3e00 0000 da0b 7072 6566 6572 656e 6365  >.....preference
-00000e30: 7372 4500 0000 5a0f 7175 6572 795f 656d  srE...Z.query_em
-00000e40: 6265 6464 696e 6772 1200 0000 7244 0000  beddingr....rD..
-00000e50: 0072 1300 0000 da1d 656d 6265 645f 7175  .r......embed_qu
-00000e60: 6572 6965 735f 616e 645f 7072 6566 6572  eries_and_prefer
-00000e70: 656e 6365 7356 0000 0073 1600 0000 0001  encesV...s......
-00000e80: 1a02 0401 0201 10ff 0202 0a05 02fb 04fe  ................
-00000e90: 020a 02f5 7a27 4261 7365 4d6f 6465 6c2e  ....z'BaseModel.
-00000ea0: 656d 6265 645f 7175 6572 6965 735f 616e  embed_queries_an
-00000eb0: 645f 7072 6566 6572 656e 6365 7363 0100  d_preferencesc..
-00000ec0: 0000 0000 0000 0000 0000 0100 0000 0100  ................
-00000ed0: 0000 4300 0000 7304 0000 0064 0153 0029  ..C...s....d.S.)
-00000ee0: 024e 4672 1200 0000 7224 0000 0072 1200  .NFr....r$...r..
-00000ef0: 0000 7212 0000 0072 1300 0000 da0d 6973  ..r....r......is
-00000f00: 5f61 7379 6d6d 6574 7269 6367 0000 0073  _asymmetricg...s
-00000f10: 0200 0000 0001 7a17 4261 7365 4d6f 6465  ......z.BaseMode
-00000f20: 6c2e 6973 5f61 7379 6d6d 6574 7269 634e  l.is_asymmetricN
-00000f30: 2901 4629 12da 085f 5f6e 616d 655f 5fda  ).F)...__name__.
-00000f40: 0a5f 5f6d 6f64 756c 655f 5fda 0c5f 5f71  .__module__..__q
-00000f50: 7561 6c6e 616d 655f 5f72 0300 0000 da03  ualname__r......
-00000f60: 696e 7472 2600 0000 da03 7374 7272 2a00  intr&.....strr*.
-00000f70: 0000 722d 0000 0072 3000 0000 7231 0000  ..r-...r0...r1..
-00000f80: 00da 0462 6f6f 6c72 3500 0000 7237 0000  ...boolr5...r7..
-00000f90: 0072 3900 0000 723f 0000 0072 4800 0000  .r9...r?...rH...
-00000fa0: 7249 0000 0072 1200 0000 7212 0000 0072  rI...r....r....r
-00000fb0: 1200 0000 7213 0000 0072 2100 0000 2d00  ....r....r!...-.
-00000fc0: 0000 7322 0000 0008 0102 0110 0302 0110  ..s"............
-00000fd0: 0302 0110 0302 0112 0302 010a 0302 0114  ................
-00000fe0: 030e 0410 040e 0808 1172 2100 0000 6300  .........r!...c.
-00000ff0: 0000 0000 0000 0000 0000 0000 0000 0004  ................
-00001000: 0000 0040 0000 0073 6800 0000 6500 5a01  ...@...sh...e.Z.
-00001010: 6400 5a02 6419 6404 6405 8401 5a03 6406  d.Z.d.d.d...Z.d.
-00001020: 6407 8400 5a04 6505 6408 9c01 6409 640a  d...Z.e.d...d.d.
-00001030: 8404 5a06 6507 640b 9c01 640c 640d 8404  ..Z.e.d...d.d...
-00001040: 5a08 6505 6408 9c01 640e 640f 8404 5a09  Z.e.d...d.d...Z.
-00001050: 6507 6410 6411 9c02 6412 6413 8404 5a0a  e.d.d...d.d...Z.
-00001060: 641a 6415 6408 9c01 6416 6417 8405 5a0b  d.d.d...d.d...Z.
-00001070: 6418 5300 291b da0b 4f70 656e 4149 4d6f  d.S.)...OpenAIMo
-00001080: 6465 6cfa 1674 6578 742d 656d 6265 6464  del..text-embedd
-00001090: 696e 672d 6164 612d 3030 32e9 0006 0000  ing-ada-002.....
-000010a0: da0b 636c 3130 306b 5f62 6173 6563 0400  ..cl100k_basec..
-000010b0: 0000 0000 0000 0000 0000 0400 0000 0300  ................
-000010c0: 0000 4300 0000 731c 0000 007c 017c 005f  ..C...s....|.|._
-000010d0: 007c 027c 005f 0174 02a0 037c 03a1 017c  .|.|._.t...|...|
-000010e0: 005f 0464 0053 0072 1500 0000 2905 da0a  ._.d.S.r....)...
-000010f0: 6d6f 6465 6c5f 6e61 6d65 da0e 6e75 6d5f  model_name..num_
-00001100: 6469 6d65 6e73 696f 6e73 da08 7469 6b74  dimensions..tikt
-00001110: 6f6b 656e 5a0c 6765 745f 656e 636f 6469  okenZ.get_encodi
-00001120: 6e67 da09 746f 6b65 6e69 7a65 7229 0472  ng..tokenizer).r
-00001130: 2500 0000 7254 0000 0072 5500 0000 da0e  %...rT...rU.....
-00001140: 746f 6b65 6e69 7a65 725f 6e61 6d65 7212  tokenizer_namer.
-00001150: 0000 0072 1200 0000 7213 0000 00da 085f  ...r....r......_
-00001160: 5f69 6e69 745f 5f6c 0000 0073 0600 0000  _init__l...s....
-00001170: 0006 0601 0601 7a14 4f70 656e 4149 4d6f  ......z.OpenAIMo
-00001180: 6465 6c2e 5f5f 696e 6974 5f5f 6301 0000  del.__init__c...
-00001190: 0000 0000 0000 0000 0001 0000 0004 0000  ................
-000011a0: 0043 0000 0073 1200 0000 6401 7c00 6a00  .C...s....d.|.j.
-000011b0: 7c00 6a01 6a02 6402 9c03 5300 2903 4eda  |.j.j.d...S.).N.
-000011c0: 066f 7065 6e61 6929 03da 0a6d 6f64 656c  .openai)...model
-000011d0: 5f74 7970 6572 5400 0000 7258 0000 0029  _typerT...rX...)
-000011e0: 0372 5400 0000 7257 0000 00da 046e 616d  .rT...rW.....nam
-000011f0: 6572 2400 0000 7212 0000 0072 1200 0000  er$...r....r....
-00001200: 7213 0000 0072 3100 0000 7600 0000 7308  r....r1...v...s.
-00001210: 0000 0000 0202 0104 0106 fd7a 164f 7065  ...........z.Ope
-00001220: 6e41 494d 6f64 656c 2e67 6574 5f63 6f6e  nAIModel.get_con
-00001230: 6669 6772 2200 0000 6301 0000 0000 0000  figr"...c.......
-00001240: 0000 0000 0001 0000 0001 0000 0043 0000  .............C..
-00001250: 0073 0600 0000 7c00 6a00 5300 7215 0000  .s....|.j.S.r...
-00001260: 0029 0172 5500 0000 7224 0000 0072 1200  .).rU...r$...r..
-00001270: 0000 7212 0000 0072 1300 0000 7226 0000  ..r....r....r&..
-00001280: 007d 0000 0073 0200 0000 0001 7a1e 4f70  .}...s......z.Op
-00001290: 656e 4149 4d6f 6465 6c2e 6765 745f 6e75  enAIModel.get_nu
-000012a0: 6d5f 6469 6d65 6e73 696f 6e73 7227 0000  m_dimensionsr'..
-000012b0: 0063 0200 0000 0000 0000 0000 0000 0200  .c..............
-000012c0: 0000 0300 0000 4300 0000 730c 0000 007c  ......C...s....|
-000012d0: 006a 00a0 017c 01a1 0153 0072 1500 0000  .j...|...S.r....
-000012e0: 2902 7257 0000 00da 0665 6e63 6f64 6572  ).rW.....encoder
-000012f0: 2900 0000 7212 0000 0072 1200 0000 7213  )...r....r....r.
-00001300: 0000 0072 2a00 0000 8000 0000 7302 0000  ...r*.......s...
-00001310: 0000 017a 164f 7065 6e41 494d 6f64 656c  ...z.OpenAIModel
-00001320: 2e67 6574 5f74 6f6b 656e 7363 0200 0000  .get_tokensc....
-00001330: 0000 0000 0000 0000 0200 0000 0200 0000  ................
-00001340: 4300 0000 7308 0000 0074 007c 0183 0153  C...s....t.|...S
-00001350: 0072 1500 0000 a901 7246 0000 0072 2b00  .r......rF...r+.
-00001360: 0000 7212 0000 0072 1200 0000 7213 0000  ..r....r....r...
-00001370: 0072 2d00 0000 8300 0000 7302 0000 0000  .r-.......s.....
-00001380: 017a 1c4f 7065 6e41 494d 6f64 656c 2e67  .z.OpenAIModel.g
-00001390: 6574 5f74 6f6b 656e 5f6c 656e 6774 6872  et_token_lengthr
-000013a0: 2e00 0000 2902 da01 5f72 2300 0000 6303  ....)..._r#...c.
-000013b0: 0000 0000 0000 0000 0000 0003 0000 0003  ................
-000013c0: 0000 0003 0000 0073 1200 0000 8700 6601  .......s......f.
-000013d0: 6401 6402 8408 7c02 4400 8301 5300 2903  d.d...|.D...S.).
-000013e0: 4e63 0100 0000 0000 0000 0000 0000 0200  Nc..............
-000013f0: 0000 0500 0000 1300 0000 731a 0000 0067  ..........s....g
-00001400: 007c 005d 127d 0188 006a 00a0 017c 0167  .|.].}...j...|.g
-00001410: 01a1 0191 0271 0453 0072 1200 0000 2902  .....q.S.r....).
-00001420: 7257 0000 00da 0664 6563 6f64 6529 0272  rW.....decode).r
-00001430: 1600 0000 da05 746f 6b65 6e72 2400 0000  ......tokenr$...
-00001440: 7212 0000 0072 1300 0000 7218 0000 0087  r....r....r.....
-00001450: 0000 0072 1900 0000 7a2f 4f70 656e 4149  ...r....z/OpenAI
-00001460: 4d6f 6465 6c2e 6765 745f 7465 7874 5f63  Model.get_text_c
-00001470: 6875 6e6b 732e 3c6c 6f63 616c 733e 2e3c  hunks.<locals>.<
-00001480: 6c69 7374 636f 6d70 3e72 1200 0000 2903  listcomp>r....).
-00001490: 7225 0000 0072 5f00 0000 722c 0000 0072  r%...r_...r,...r
-000014a0: 1200 0000 7224 0000 0072 1300 0000 7230  ....r$...r....r0
-000014b0: 0000 0086 0000 0073 0200 0000 0001 7a1b  .......s......z.
-000014c0: 4f70 656e 4149 4d6f 6465 6c2e 6765 745f  OpenAIModel.get_
-000014d0: 7465 7874 5f63 6875 6e6b 7346 7232 0000  text_chunksFr2..
-000014e0: 0063 0400 0000 0000 0000 0000 0000 0600  .c..............
-000014f0: 0000 0500 0000 0300 0000 733c 0000 0087  ..........s<....
-00001500: 0066 0164 0164 0284 087c 0244 0083 017d  .f.d.d...|.D...}
-00001510: 0474 006a 016a 027c 006a 037c 0464 038d  .t.j.j.|.j.|.d..
-00001520: 027d 0574 04a0 0564 0464 0284 007c 0564  .}.t...d.d...|.d
-00001530: 0519 0044 0083 01a1 0153 0029 064e 6301  ...D.....S.).Nc.
-00001540: 0000 0000 0000 0000 0000 0003 0000 0005  ................
-00001550: 0000 0013 0000 0073 1c00 0000 6700 7c00  .......s....g.|.
-00001560: 5d14 5c02 7d01 7d02 8800 7c01 7c02 8502  ].\.}.}...|.|...
-00001570: 1900 9102 7104 5300 7212 0000 0072 1200  ....q.S.r....r..
-00001580: 0000 a903 7216 0000 0072 1700 0000 da01  ....r....r......
-00001590: 6aa9 0172 2c00 0000 7212 0000 0072 1300  j..r,...r....r..
-000015a0: 0000 7218 0000 008a 0000 0072 1900 0000  ..r........r....
-000015b0: 7a25 4f70 656e 4149 4d6f 6465 6c2e 656d  z%OpenAIModel.em
-000015c0: 6265 642e 3c6c 6f63 616c 733e 2e3c 6c69  bed.<locals>.<li
-000015d0: 7374 636f 6d70 3e29 02da 056d 6f64 656c  stcomp>)...model
-000015e0: da05 696e 7075 7463 0100 0000 0000 0000  ..inputc........
-000015f0: 0000 0000 0200 0000 0400 0000 5300 0000  ............S...
-00001600: 7314 0000 0067 007c 005d 0c7d 017c 0164  s....g.|.].}.|.d
-00001610: 0019 0091 0271 0453 0029 01da 0965 6d62  .....q.S.)...emb
-00001620: 6564 6469 6e67 7212 0000 0029 0272 1600  eddingr....).r..
-00001630: 0000 da04 6461 7461 7212 0000 0072 1200  ....datar....r..
-00001640: 0000 7213 0000 0072 1800 0000 8c00 0000  ..r....r........
-00001650: 7219 0000 0072 6800 0000 2906 725a 0000  r....rh...).rZ..
-00001660: 005a 0945 6d62 6564 6469 6e67 da06 6372  .Z.Embedding..cr
-00001670: 6561 7465 7254 0000 0072 3d00 0000 da05  eaterT...r=.....
-00001680: 6172 7261 7929 0672 2500 0000 722c 0000  array).r%...r,..
-00001690: 0072 3400 0000 5a09 5f69 735f 7175 6572  .r4...Z._is_quer
-000016a0: 795a 0574 6578 7473 da08 7265 7370 6f6e  yZ.texts..respon
-000016b0: 7365 7212 0000 0072 6400 0000 7213 0000  ser....rd...r...
-000016c0: 0072 3500 0000 8900 0000 7306 0000 0000  .r5.......s.....
-000016d0: 0112 0112 017a 114f 7065 6e41 494d 6f64  .....z.OpenAIMod
-000016e0: 656c 2e65 6d62 6564 4e29 0372 5100 0000  el.embedN).rQ...
-000016f0: 7252 0000 0072 5300 0000 2901 4629 0c72  rR...rS...).F).r
-00001700: 4a00 0000 724b 0000 0072 4c00 0000 7259  J...rK...rL...rY
-00001710: 0000 0072 3100 0000 724d 0000 0072 2600  ...r1...rM...r&.
-00001720: 0000 724e 0000 0072 2a00 0000 722d 0000  ..rN...r*...r-..
-00001730: 0072 3000 0000 7235 0000 0072 1200 0000  .r0...r5...r....
-00001740: 7212 0000 0072 1200 0000 7213 0000 0072  r....r....r....r
-00001750: 5000 0000 6b00 0000 7314 0000 0008 0300  P...k...s.......
-00001760: 0100 0100 fc0a 0a08 070e 030e 030e 0310  ................
-00001770: 0372 5000 0000 6301 0000 0000 0000 0000  .rP...c.........
-00001780: 0000 0001 0000 0002 0000 0043 0000 0073  ...........C...s
-00001790: 1000 0000 7c00 6400 7500 720c 6401 5300  ....|.d.u.r.d.S.
-000017a0: 7c00 5300 2902 4e72 0100 0000 7212 0000  |.S.).Nr....r...
-000017b0: 0072 1a00 0000 7212 0000 0072 1200 0000  .r....r....r....
-000017c0: 7213 0000 00da 0c7a 6572 6f5f 6966 5f6e  r......zero_if_n
-000017d0: 6f6e 658f 0000 0073 0200 0000 0001 726c  one....s......rl
-000017e0: 0000 0063 0000 0000 0000 0000 0000 0000  ...c............
-000017f0: 0000 0000 0600 0000 4000 0000 7380 0000  ........@...s...
-00001800: 0065 005a 0164 005a 0264 1c64 0364 0484  .e.Z.d.Z.d.d.d..
-00001810: 015a 0364 0564 0684 005a 0464 0764 0884  .Z.d.d...Z.d.d..
-00001820: 005a 0565 0664 099c 0164 0a64 0b84 045a  .Z.e.d...d.d...Z
-00001830: 0765 0864 0c9c 0164 0d64 0e84 045a 0965  .e.d...d.d...Z.e
-00001840: 0664 099c 0164 0f64 1084 045a 0a65 0864  .d...d.d...Z.e.d
-00001850: 1164 129c 0264 1364 1484 045a 0b64 1564  .d...d.d...Z.d.d
-00001860: 1684 005a 0c64 1764 1884 005a 0d64 1d64  ...Z.d.d...Z.d.d
-00001870: 1964 099c 0164 1a64 1b84 055a 0e64 0153  .d...d.d...Z.d.S
-00001880: 0029 1eda 1054 7261 6e73 666f 726d 6572  .)...Transformer
-00001890: 4d6f 6465 6c4e 4663 0800 0000 0000 0000  ModelNFc........
-000018a0: 0000 0000 0800 0000 0400 0000 4300 0000  ............C...
-000018b0: 73c8 0000 007c 0764 0075 0072 1274 006a  s....|.d.u.r.t.j
-000018c0: 01a0 02a1 007d 077c 017c 005f 0374 04a0  .....}.|.|._.t..
-000018d0: 057c 01a1 017c 005f 0674 07a0 057c 01a1  .|...|._.t...|..
-000018e0: 017c 005f 087c 027c 037c 047c 0567 047c  .|._.|.|.|.|.g.|
-000018f0: 005f 097c 0272 527c 006a 066a 0a7c 0264  ._.|.rR|.j.j.|.d
-00001900: 0164 028d 026e 0264 007c 005f 0b7c 0372  .d...n.d.|._.|.r
-00001910: 6c7c 006a 066a 0a7c 0364 0164 028d 026e  l|.j.j.|.d.d...n
-00001920: 0264 007c 005f 0c7c 0472 867c 006a 066a  .d.|._.|.r.|.j.j
-00001930: 0a7c 0464 0164 028d 026e 0264 007c 005f  .|.d.d...n.d.|._
-00001940: 0d7c 0572 a07c 006a 066a 0a7c 0564 0164  .|.r.|.j.j.|.d.d
-00001950: 028d 026e 0264 007c 005f 0e7c 067c 005f  ...n.d.|._.|.|._
-00001960: 0f7c 077c 005f 017c 006a 0172 c47c 006a  .|.|._.|.j.r.|.j
-00001970: 08a0 01a1 007c 005f 0864 0053 0029 034e  .....|._.d.S.).N
-00001980: 4629 015a 1261 6464 5f73 7065 6369 616c  F).Z.add_special
-00001990: 5f74 6f6b 656e 7329 1072 0d00 0000 da04  _tokens).r......
-000019a0: 6375 6461 5a0c 6973 5f61 7661 696c 6162  cudaZ.is_availab
-000019b0: 6c65 7254 0000 0072 0400 0000 5a0f 6672  lerT...r....Z.fr
-000019c0: 6f6d 5f70 7265 7472 6169 6e65 6472 5700  om_pretrainedrW.
-000019d0: 0000 7205 0000 0072 6500 0000 da0f 7072  ..r....re.....pr
-000019e0: 655f 706f 7374 5f74 6f6b 656e 7372 5d00  e_post_tokensr].
-000019f0: 0000 da0d 646f 635f 746f 6b65 6e5f 7072  ....doc_token_pr
-00001a00: 65da 0e64 6f63 5f74 6f6b 656e 5f70 6f73  e..doc_token_pos
-00001a10: 74da 0f71 7565 7279 5f74 6f6b 656e 5f70  t..query_token_p
-00001a20: 7265 da10 7175 6572 795f 746f 6b65 6e5f  re..query_token_
-00001a30: 706f 7374 da0a 6173 796d 6d65 7472 6963  post..asymmetric
-00001a40: 2908 7225 0000 0072 5400 0000 7270 0000  ).r%...rT...rp..
-00001a50: 0072 7100 0000 7272 0000 0072 7300 0000  .rq...rr...rs...
-00001a60: 7274 0000 0072 6e00 0000 7212 0000 0072  rt...rn...r....r
-00001a70: 1200 0000 7213 0000 0072 5900 0000 9400  ....r....rY.....
-00001a80: 0000 733c 0000 0000 0a08 010a 0106 010c  ..s<............
-00001a90: 010c 0402 0102 0102 0102 fc06 0802 ff12  ................
-00001aa0: 0202 fd04 0702 ff12 0202 fd04 0702 ff12  ................
-00001ab0: 0202 fd04 0702 ff12 0202 fd04 0606 0206  ................
-00001ac0: 0106 017a 1954 7261 6e73 666f 726d 6572  ...z.Transformer
-00001ad0: 4d6f 6465 6c2e 5f5f 696e 6974 5f5f 6301  Model.__init__c.
-00001ae0: 0000 0000 0000 0000 0000 0001 0000 0008  ................
-00001af0: 0000 0043 0000 0073 3000 0000 6401 7c00  ...C...s0...d.|.
-00001b00: 6a00 7c00 6a01 6402 1900 7c00 6a01 6403  j.|.j.d...|.j.d.
-00001b10: 1900 7c00 6a01 6404 1900 7c00 6a01 6405  ..|.j.d...|.j.d.
-00001b20: 1900 7c00 6a02 6406 9c07 5300 2907 4eda  ..|.j.d...S.).N.
-00001b30: 0c74 7261 6e73 666f 726d 6572 7372 0100  .transformersr..
-00001b40: 0000 7208 0000 00e9 0200 0000 e903 0000  ..r.............
-00001b50: 0029 0772 5b00 0000 7254 0000 0072 7000  .).r[...rT...rp.
-00001b60: 0000 7271 0000 0072 7200 0000 7273 0000  ..rq...rr...rs..
-00001b70: 0072 7400 0000 2903 7254 0000 0072 6f00  .rt...).rT...ro.
-00001b80: 0000 7274 0000 0072 2400 0000 7212 0000  ..rt...r$...r...
-00001b90: 0072 1200 0000 7213 0000 0072 3100 0000  .r....r....r1...
-00001ba0: c600 0000 7310 0000 0000 0202 0104 0108  ....s...........
-00001bb0: 0108 0108 0108 0104 f97a 1b54 7261 6e73  .........z.Trans
-00001bc0: 666f 726d 6572 4d6f 6465 6c2e 6765 745f  formerModel.get_
-00001bd0: 636f 6e66 6967 6301 0000 0000 0000 0000  configc.........
-00001be0: 0000 0001 0000 0001 0000 0043 0000 0073  ...........C...s
-00001bf0: 0600 0000 7c00 6a00 5300 7215 0000 0029  ....|.j.S.r....)
-00001c00: 0172 7400 0000 7224 0000 0072 1200 0000  .rt...r$...r....
-00001c10: 7212 0000 0072 1300 0000 7249 0000 00d1  r....r....rI....
-00001c20: 0000 0073 0200 0000 0001 7a1e 5472 616e  ...s......z.Tran
-00001c30: 7366 6f72 6d65 724d 6f64 656c 2e69 735f  sformerModel.is_
-00001c40: 6173 796d 6d65 7472 6963 7222 0000 0063  asymmetricr"...c
-00001c50: 0100 0000 0000 0000 0000 0000 0100 0000  ................
-00001c60: 0200 0000 4300 0000 730e 0000 0074 007c  ....C...s....t.|
-00001c70: 006a 016a 026a 0383 0153 0072 1500 0000  .j.j.j...S.r....
-00001c80: 2904 724d 0000 0072 6500 0000 da06 636f  ).rM...re.....co
-00001c90: 6e66 6967 5a0b 6869 6464 656e 5f73 697a  nfigZ.hidden_siz
-00001ca0: 6572 2400 0000 7212 0000 0072 1200 0000  er$...r....r....
-00001cb0: 7213 0000 0072 2600 0000 d400 0000 7302  r....r&.......s.
-00001cc0: 0000 0000 017a 2354 7261 6e73 666f 726d  .....z#Transform
-00001cd0: 6572 4d6f 6465 6c2e 6765 745f 6e75 6d5f  erModel.get_num_
-00001ce0: 6469 6d65 6e73 696f 6e73 7227 0000 0063  dimensionsr'...c
-00001cf0: 0200 0000 0000 0000 0000 0000 0200 0000  ................
-00001d00: 0600 0000 4300 0000 7312 0000 007c 006a  ....C...s....|.j
-00001d10: 007c 0164 0164 0264 0364 048d 0453 0029  .|.d.d.d.d...S.)
-00001d20: 054e 5446 da02 7074 2903 5a16 7265 7475  .NTF..pt).Z.retu
-00001d30: 726e 5f6f 6666 7365 7473 5f6d 6170 7069  rn_offsets_mappi
-00001d40: 6e67 da07 7665 7262 6f73 655a 0e72 6574  ng..verboseZ.ret
-00001d50: 7572 6e5f 7465 6e73 6f72 7329 0172 5700  urn_tensors).rW.
-00001d60: 0000 7229 0000 0072 1200 0000 7212 0000  ..r)...r....r...
-00001d70: 0072 1300 0000 722a 0000 00d7 0000 0073  .r....r*.......s
-00001d80: 0600 0000 0001 0401 08ff 7a1b 5472 616e  ..........z.Tran
-00001d90: 7366 6f72 6d65 724d 6f64 656c 2e67 6574  sformerModel.get
-00001da0: 5f74 6f6b 656e 7363 0200 0000 0000 0000  _tokensc........
-00001db0: 0000 0000 0200 0000 0300 0000 4300 0000  ............C...
-00001dc0: 7310 0000 0074 007c 0164 0119 0064 0219  s....t.|.d...d..
-00001dd0: 0083 0153 0029 034e da09 696e 7075 745f  ...S.).N..input_
-00001de0: 6964 7372 0100 0000 725e 0000 0072 2b00  idsr....r^...r+.
-00001df0: 0000 7212 0000 0072 1200 0000 7213 0000  ..r....r....r...
-00001e00: 0072 2d00 0000 dc00 0000 7302 0000 0000  .r-.......s.....
-00001e10: 017a 2154 7261 6e73 666f 726d 6572 4d6f  .z!TransformerMo
-00001e20: 6465 6c2e 6765 745f 746f 6b65 6e5f 6c65  del.get_token_le
-00001e30: 6e67 7468 722e 0000 0072 2f00 0000 6303  ngthr....r/...c.
-00001e40: 0000 0000 0000 0000 0000 000a 0000 0006  ................
-00001e50: 0000 0043 0000 0073 a600 0000 7c02 6401  ...C...s....|.d.
-00001e60: 1900 6402 1900 7d03 6700 7d04 6400 7d05  ..d...}.g.}.d.}.
-00001e70: 6400 7d06 7c03 4400 5d66 5c02 7d07 7d08  d.}.|.D.]f\.}.}.
-00001e80: 7c07 7c08 6b02 7230 7c06 6e02 7c07 7d09  |.|.k.r0|.n.|.}.
-00001e90: 7c05 6400 7501 724e 7c04 a000 7c01 7c05  |.d.u.rN|...|.|.
-00001ea0: 7c09 8502 1900 a101 0100 7c05 6400 7500  |.........|.d.u.
-00001eb0: 725c 6402 7d05 6e0c 7c09 7c05 6b04 7268  r\d.}.n.|.|.k.rh
-00001ec0: 7c09 7d05 7c06 6400 7500 7276 7c08 7d06  |.}.|.d.u.rv|.}.
-00001ed0: 711c 7c08 7c06 6b04 721c 7c08 7d06 711c  q.|.|.k.r.|.}.q.
-00001ee0: 7c04 a000 7c01 7c05 6400 7500 7296 6402  |...|.|.d.u.r.d.
-00001ef0: 6e02 7c05 6400 8502 1900 a101 0100 7c04  n.|.d.........|.
-00001f00: 5300 2903 4e5a 0e6f 6666 7365 745f 6d61  S.).NZ.offset_ma
-00001f10: 7070 696e 6772 0100 0000 2901 da06 6170  ppingr....)...ap
-00001f20: 7065 6e64 290a 7225 0000 0072 2800 0000  pend).r%...r(...
-00001f30: 722c 0000 0072 3400 0000 da06 6368 756e  r,...r4.....chun
-00001f40: 6b73 5a06 7072 6576 5f69 5a06 7072 6576  ksZ.prev_iZ.prev
-00001f50: 5f6a 7217 0000 0072 6300 0000 5a05 6e65  _jr....rc...Z.ne
-00001f60: 775f 6972 1200 0000 7212 0000 0072 1300  w_ir....r....r..
-00001f70: 0000 7230 0000 00df 0000 0073 2400 0000  ..r0.......s$...
-00001f80: 0001 0c01 0401 0401 0401 0c01 1001 0801  ................
-00001f90: 1201 0801 0601 0801 0401 0801 0601 0801  ................
-00001fa0: 0601 1e01 7a20 5472 616e 7366 6f72 6d65  ....z Transforme
-00001fb0: 724d 6f64 656c 2e67 6574 5f74 6578 745f  rModel.get_text_
-00001fc0: 6368 756e 6b73 6303 0000 0000 0000 0000  chunksc.........
-00001fd0: 0000 0005 0000 0008 0000 0043 0000 0073  ...........C...s
-00001fe0: 7400 0000 7c00 6a00 6400 7500 7218 7c00  t...|.j.d.u.r.|.
-00001ff0: 6a01 6400 7500 7218 7c01 5300 7c02 7222  j.d.u.r.|.S.|.r"
-00002000: 7c00 6a00 6e04 7c00 6a02 7d03 7c02 7232  |.j.n.|.j.}.|.r2
-00002010: 7c00 6a01 6e04 7c00 6a03 7d04 7404 a005  |.j.n.|.j.}.t...
-00002020: 7406 7c03 6400 7501 7250 7404 a007 7c03  t.|.d.u.rPt...|.
-00002030: a101 6e02 6400 7c01 7c04 6400 7501 7266  ..n.d.|.|.d.u.rf
-00002040: 7404 a007 7c04 a101 6e02 6400 6703 8301  t...|...n.d.g...
-00002050: a101 5300 6400 5300 7215 0000 0029 0872  ..S.d.S.r....).r
-00002060: 7200 0000 7273 0000 0072 7000 0000 7271  r...rs...rp...rq
-00002070: 0000 0072 0d00 0000 da03 6361 7472 1c00  ...r......catr..
-00002080: 0000 da06 7465 6e73 6f72 2905 7225 0000  ....tensor).r%..
-00002090: 0072 7b00 0000 7233 0000 00da 0974 6f6b  .r{...r3.....tok
-000020a0: 656e 5f70 7265 da0a 746f 6b65 6e5f 706f  en_pre..token_po
-000020b0: 7374 7212 0000 0072 1200 0000 7213 0000  str....r....r...
-000020c0: 00da 136e 6f72 6d61 6c69 7a65 5f69 6e70  ...normalize_inp
-000020d0: 7574 5f69 6473 f300 0000 7318 0000 0000  ut_ids....s.....
-000020e0: 0114 0104 0210 0110 0104 0102 0214 0102  ................
-000020f0: 0114 fd02 ff02 ff7a 2454 7261 6e73 666f  .......z$Transfo
-00002100: 726d 6572 4d6f 6465 6c2e 6e6f 726d 616c  rmerModel.normal
-00002110: 697a 655f 696e 7075 745f 6964 7363 0300  ize_input_idsc..
-00002120: 0000 0000 0000 0000 0000 0500 0000 0900  ................
-00002130: 0000 4300 0000 737c 0000 007c 006a 0064  ..C...s|...|.j.d
-00002140: 0075 0072 187c 006a 0164 0075 0072 187c  .u.r.|.j.d.u.r.|
-00002150: 0153 007c 0272 227c 006a 006e 047c 006a  .S.|.r"|.j.n.|.j
-00002160: 027d 037c 0272 327c 006a 016e 047c 006a  .}.|.r2|.j.n.|.j
-00002170: 037d 0474 04a0 0574 067c 0364 0075 0172  .}.t...t.|.d.u.r
-00002180: 5474 04a0 0774 087c 0383 01a1 016e 0264  Tt...t.|.....n.d
-00002190: 007c 017c 0464 0075 0172 6e74 04a0 0774  .|.|.d.u.rnt...t
-000021a0: 087c 0483 01a1 016e 0264 0067 0383 01a1  .|.....n.d.g....
-000021b0: 0153 0064 0053 0072 1500 0000 2909 7272  .S.d.S.r....).rr
-000021c0: 0000 0072 7300 0000 7270 0000 0072 7100  ...rs...rp...rq.
-000021d0: 0000 720d 0000 0072 7e00 0000 721c 0000  ..r....r~...r...
-000021e0: 00da 046f 6e65 7372 4600 0000 2905 7225  ...onesrF...).r%
-000021f0: 0000 0072 1100 0000 7233 0000 0072 8000  ...r....r3...r..
-00002200: 0000 7281 0000 0072 1200 0000 7212 0000  ..r....r....r...
-00002210: 0072 1300 0000 da18 6e6f 726d 616c 697a  .r......normaliz
-00002220: 655f 6174 7465 6e74 696f 6e5f 6d61 736b  e_attention_mask
-00002230: 0301 0000 7318 0000 0000 0114 0104 0210  ....s...........
-00002240: 0110 0104 0102 0218 0102 0118 fd02 ff02  ................
-00002250: ff7a 2954 7261 6e73 666f 726d 6572 4d6f  .z)TransformerMo
-00002260: 6465 6c2e 6e6f 726d 616c 697a 655f 6174  del.normalize_at
-00002270: 7465 6e74 696f 6e5f 6d61 736b 7232 0000  tention_maskr2..
-00002280: 0063 0400 0000 0000 0000 0000 0000 0700  .c..............
-00002290: 0000 0800 0000 0300 0000 73ae 0000 0074  ..........s....t
-000022a0: 006a 016a 026a 036a 0487 0087 0187 0266  .j.j.j.j.......f
-000022b0: 0364 0164 0284 087c 0244 0083 0164 0374  .d.d...|.D...d.t
-000022c0: 0588 016a 066a 0783 0164 048d 037d 0474  ...j.j...d...}.t
-000022d0: 006a 016a 026a 036a 0487 0087 0187 0266  .j.j.j.j.......f
-000022e0: 0364 0564 0284 087c 0244 0083 0164 0364  .d.d...|.D...d.d
-000022f0: 0664 048d 037d 0588 016a 0872 6e7c 04a0  .d...}...j.rn|..
-00002300: 08a1 007d 047c 05a0 08a1 007d 0574 00a0  ...}.|.....}.t..
-00002310: 09a1 008f 1e01 0088 016a 0a7c 047c 0564  .........j.|.|.d
-00002320: 078d 027d 0657 0064 0004 0004 0083 0301  ...}.W.d........
-00002330: 006e 1031 0073 9a30 0001 0001 0001 0059  .n.1.s.0.......Y
-00002340: 0001 0074 0b7c 067c 0583 0253 0029 084e  ...t.|.|...S.).N
-00002350: 6301 0000 0000 0000 0000 0000 0003 0000  c...............
-00002360: 000c 0000 0013 0000 0073 3800 0000 6700  .........s8...g.
-00002370: 7c00 5d30 5c02 7d01 7d02 8801 a000 8802  |.]0\.}.}.......
-00002380: 6400 1900 6401 1900 a001 6401 7402 a003  d...d.....d.t...
-00002390: 7404 7c01 7c02 8302 a101 a102 8800 a102  t.|.|...........
-000023a0: 9102 7104 5300 2902 727b 0000 0072 0100  ..q.S.).r{...r..
-000023b0: 0000 2905 7282 0000 00da 0c69 6e64 6578  ..).r......index
-000023c0: 5f73 656c 6563 7472 0d00 0000 727f 0000  _selectr....r...
-000023d0: 00da 0572 616e 6765 7262 0000 00a9 0372  ...rangerb.....r
-000023e0: 3300 0000 7225 0000 0072 2c00 0000 7212  3...r%...r,...r.
-000023f0: 0000 0072 1300 0000 7218 0000 0015 0100  ...r....r.......
-00002400: 0073 0a00 0000 0605 06fc 0401 1e01 02fe  .s..............
-00002410: 7a2a 5472 616e 7366 6f72 6d65 724d 6f64  z*TransformerMod
-00002420: 656c 2e65 6d62 6564 2e3c 6c6f 6361 6c73  el.embed.<locals
-00002430: 3e2e 3c6c 6973 7463 6f6d 703e 5429 025a  >.<listcomp>T).Z
-00002440: 0b62 6174 6368 5f66 6972 7374 5a0d 7061  .batch_firstZ.pa
-00002450: 6464 696e 675f 7661 6c75 6563 0100 0000  dding_valuec....
-00002460: 0000 0000 0000 0000 0300 0000 0c00 0000  ................
-00002470: 1300 0000 7338 0000 0067 007c 005d 305c  ....s8...g.|.]0\
-00002480: 027d 017d 0288 01a0 0088 0264 0019 0064  .}.}.......d...d
-00002490: 0119 00a0 0164 0174 02a0 0374 047c 017c  .....d.t...t.|.|
-000024a0: 0283 02a1 01a1 0288 00a1 0291 0271 0453  .............q.S
-000024b0: 0029 0272 1100 0000 7201 0000 0029 0572  .).r....r....).r
-000024c0: 8400 0000 7285 0000 0072 0d00 0000 727f  ....r....r....r.
-000024d0: 0000 0072 8600 0000 7262 0000 0072 8700  ...r....rb...r..
-000024e0: 0000 7212 0000 0072 1300 0000 7218 0000  ..r....r....r...
-000024f0: 0020 0100 0073 0e00 0000 0607 06fa 0401  . ...s..........
-00002500: 0c01 10ff 0203 02fc 7201 0000 0029 0272  ........r....).r
-00002510: 7b00 0000 7211 0000 0029 0c72 0d00 0000  {...r....).r....
-00002520: da02 6e6e da05 7574 696c 735a 0372 6e6e  ..nn..utilsZ.rnn
-00002530: 5a0c 7061 645f 7365 7175 656e 6365 726c  Z.pad_sequencerl
-00002540: 0000 0072 5700 0000 5a0c 7061 645f 746f  ...rW...Z.pad_to
-00002550: 6b65 6e5f 6964 726e 0000 005a 076e 6f5f  ken_idrn...Z.no_
-00002560: 6772 6164 7265 0000 0072 1400 0000 2907  gradre...r....).
-00002570: 7225 0000 0072 2c00 0000 7234 0000 0072  r%...r,...r4...r
-00002580: 3300 0000 727b 0000 0072 1100 0000 7210  3...r{...r....r.
-00002590: 0000 0072 1200 0000 7287 0000 0072 1300  ...r....r....r..
-000025a0: 0000 7235 0000 0013 0100 0073 2c00 0000  ..r5.......s,...
-000025b0: 0001 0a01 0e05 02fb 0407 0201 0af7 060b  ................
-000025c0: 0a01 0e07 02f9 0409 0201 02f5 060d 0601  ................
-000025d0: 0801 0801 0a01 0401 04ff 2403 7a16 5472  ..........$.z.Tr
-000025e0: 616e 7366 6f72 6d65 724d 6f64 656c 2e65  ansformerModel.e
-000025f0: 6d62 6564 2906 4e4e 4e4e 464e 2901 4629  mbed).NNNNFN).F)
-00002600: 0f72 4a00 0000 724b 0000 0072 4c00 0000  .rJ...rK...rL...
-00002610: 7259 0000 0072 3100 0000 7249 0000 0072  rY...r1...rI...r
-00002620: 4d00 0000 7226 0000 0072 4e00 0000 722a  M...r&...rN...r*
-00002630: 0000 0072 2d00 0000 7230 0000 0072 8200  ...r-...r0...r..
-00002640: 0000 7284 0000 0072 3500 0000 7212 0000  ..r....r5...r...
-00002650: 0072 1200 0000 7212 0000 0072 1300 0000  .r....r....r....
-00002660: 726d 0000 0093 0000 0073 2000 0000 0804  rm.......s .....
-00002670: 0001 0001 0001 0001 0001 00f8 0a32 080b  .............2..
-00002680: 0803 0e03 0e05 0e03 1014 0810 0810 726d  ..............rm
-00002690: 0000 0067 49af bc9a f2d7 9a3e 6950 c300  ...gI......>iP..
-000026a0: 0069 d007 0000 6300 0000 0000 0000 0000  .i....c.........
-000026b0: 0000 0000 0000 0005 0000 0043 0000 0073  ...........C...s
-000026c0: 0e00 0000 7400 6401 6402 6403 6404 8d03  ....t.d.d.d.d...
-000026d0: 5300 2905 4e72 5100 0000 7252 0000 0072  S.).NrQ...rR...r
-000026e0: 5300 0000 2903 7254 0000 0072 5500 0000  S...).rT...rU...
-000026f0: 7258 0000 0029 0172 5000 0000 7212 0000  rX...).rP...r...
-00002700: 0072 1200 0000 7212 0000 0072 1300 0000  .r....r....r....
-00002710: da08 3c6c 616d 6264 613e 3b01 0000 7308  ..<lambda>;...s.
-00002720: 0000 0002 0102 0102 0102 fd72 8a00 0000  ...........r....
-00002730: 2904 da0e 636f 7374 5f70 6572 5f74 6f6b  )...cost_per_tok
-00002740: 656e da09 706f 6f6c 5f73 697a 65da 0a70  en..pool_size..p
-00002750: 6f6f 6c5f 636f 756e 74da 0967 6574 5f6d  ool_count..get_m
-00002760: 6f64 656c 6300 0000 0000 0000 0000 0000  odelc...........
-00002770: 0000 0000 0003 0000 0043 0000 0073 0a00  .........C...s..
-00002780: 0000 7400 7401 6401 8d01 5300 a902 4e29  ..t.t.d...S...N)
-00002790: 0172 5400 0000 2902 726d 0000 00da 116d  .rT...).rm.....m
-000027a0: 696e 696c 6d5f 6d6f 6465 6c5f 6e61 6d65  inilm_model_name
-000027b0: 7212 0000 0072 1200 0000 7212 0000 0072  r....r....r....r
-000027c0: 1300 0000 728a 0000 0044 0100 0072 1900  ....r....D...r..
-000027d0: 0000 2903 728b 0000 0072 8c00 0000 728e  ..).r....r....r.
-000027e0: 0000 0069 983a 0000 6300 0000 0000 0000  ...i.:..c.......
-000027f0: 0000 0000 0000 0000 0003 0000 0043 0000  .............C..
-00002800: 0073 0a00 0000 7400 7401 6401 8d01 5300  .s....t.t.d...S.
-00002810: 728f 0000 0029 0272 6d00 0000 da10 6d70  r....).rm.....mp
-00002820: 6e65 745f 6d6f 6465 6c5f 6e61 6d65 7212  net_model_namer.
-00002830: 0000 0072 1200 0000 7212 0000 0072 1300  ...r....r....r..
-00002840: 0000 728a 0000 0049 0100 0072 1900 0000  ..r....I...r....
-00002850: 6910 2700 0063 0000 0000 0000 0000 0000  i.'..c..........
-00002860: 0000 0000 0000 0800 0000 4300 0000 7314  ..........C...s.
-00002870: 0000 0074 0074 0164 0164 0264 0364 0464  ...t.t.d.d.d.d.d
-00002880: 0564 068d 0653 00a9 074e fa01 5bfa 015d  .d...S...N..[..]
-00002890: da01 7bda 017d 5429 0672 5400 0000 7272  ..{..}T).rT...rr
-000028a0: 0000 0072 7300 0000 7270 0000 0072 7100  ...rs...rp...rq.
-000028b0: 0000 7274 0000 0029 0272 6d00 0000 da0f  ..rt...).rm.....
-000028c0: 7367 7074 5f6d 6f64 656c 5f6e 616d 6572  sgpt_model_namer
-000028d0: 1200 0000 7212 0000 0072 1200 0000 7213  ....r....r....r.
-000028e0: 0000 0072 8a00 0000 4e01 0000 730e 0000  ...r....N...s...
-000028f0: 0002 0102 0102 0102 0102 0102 0102 fa69  ...............i
-00002900: e803 0000 6300 0000 0000 0000 0000 0000  ....c...........
-00002910: 0000 0000 0008 0000 0043 0000 0073 1400  .........C...s..
-00002920: 0000 7400 7401 6401 6402 6403 6404 6405  ..t.t.d.d.d.d.d.
-00002930: 6406 8d06 5300 7292 0000 0029 0272 6d00  d...S.r....).rm.
-00002940: 0000 da14 7367 7074 5f31 5f33 425f 6d6f  ....sgpt_1_3B_mo
-00002950: 6465 6c5f 6e61 6d65 7212 0000 0072 1200  del_namer....r..
-00002960: 0000 7212 0000 0072 1300 0000 728a 0000  ..r....r....r...
-00002970: 005a 0100 0073 0e00 0000 0201 0201 0201  .Z...s..........
-00002980: 0201 0201 0201 02fa 2905 725a 0000 005a  ........).rZ...Z
-00002990: 066d 696e 696c 6dda 056d 706e 6574 5a04  .minilm..mpnetZ.
-000029a0: 7367 7074 7a09 7367 7074 2d31 2e33 4229  sgptz.sgpt-1.3B)
-000029b0: 1d72 0d00 0000 da03 6162 6372 0200 0000  .r......abcr....
-000029c0: 7203 0000 0072 7500 0000 7204 0000 0072  r....ru...r....r
-000029d0: 0500 0000 7256 0000 0072 1f00 0000 723d  ....rV...r....r=
-000029e0: 0000 0072 5a00 0000 da06 646f 7465 6e76  ...rZ.....dotenv
-000029f0: 7206 0000 00da 026f 73da 0765 6e76 6972  r......os..envir
-00002a00: 6f6e da06 6765 7465 6e76 5a07 6170 695f  on..getenvZ.api_
-00002a10: 6b65 7972 9000 0000 7291 0000 0072 9700  keyr....r....r..
-00002a20: 0000 7298 0000 0072 1400 0000 721c 0000  ..r....r....r...
-00002a30: 0072 2000 0000 7221 0000 0072 5000 0000  .r ...r!...rP...
-00002a40: 726c 0000 0072 6d00 0000 da06 6d6f 6465  rl...rm.....mode
-00002a50: 6c73 7212 0000 0072 1200 0000 7212 0000  lsr....r....r...
-00002a60: 0072 1300 0000 da08 3c6d 6f64 756c 653e  .r......<module>
-00002a70: 0100 0000 7358 0000 0008 0110 0110 0108  ....sX..........
-00002a80: 0108 0108 010c 0108 0206 020a 010c 0304  ................
-00002a90: 0104 0104 0104 0308 0c08 0408 0710 3e10  ..............>.
-00002aa0: 2408 0410 7f00 2602 0102 0102 0106 fc04  $.....&.........
-00002ab0: 0b02 0102 0106 fd04 0602 0102 0106 fd04  ................
-00002ac0: 0602 0102 0106 fd04 0d02 0102 0106 fd04  ................
-00002ad0: df                                       .
+00000040: 6d03 5a03 0100 6400 6401 6c04 5a05 6400  m.Z...d.d.l.Z.d.
+00000050: 6401 6c06 5a06 6400 6401 6c07 5a07 6400  d.l.Z.d.d.l.Z.d.
+00000060: 6401 6c08 5a08 6400 6403 6c09 6d0a 5a0a  d.l.Z.d.d.l.m.Z.
+00000070: 0100 6400 6404 6c0b 6d0c 5a0c 6d0d 5a0d  ..d.d.l.m.Z.m.Z.
+00000080: 0100 650a 6500 6a0e a00f 6500 a010 a100  ..e.e.j...e.....
+00000090: 6405 a102 6406 8d01 0100 6407 5a11 6408  d...d.....d.Z.d.
+000000a0: 5a12 6409 5a13 640a 5a14 640b 640c 8400  Z.d.Z.d.Z.d.d...
+000000b0: 5a15 640d 640e 8400 5a16 640f 6410 8400  Z.d.d...Z.d.d...
+000000c0: 5a17 4700 6411 6412 8400 6412 6502 8303  Z.G.d.d...d.e...
+000000d0: 5a18 4700 6413 6414 8400 6414 6518 8303  Z.G.d.d...d.e...
+000000e0: 5a19 6415 6416 8400 5a1a 4700 6417 6418  Z.d.d...Z.G.d.d.
+000000f0: 8400 6418 6518 8303 5a1b 6419 641a 641b  ..d.e...Z.d.d.d.
+00000100: 641c 641d 8400 641e 9c04 6401 641a 641f  d.d...d...d.d.d.
+00000110: 641d 8400 6420 9c03 6401 6421 6422 641d  d...d ..d.d!d"d.
+00000120: 8400 6420 9c03 6401 6423 6424 641d 8400  ..d ..d.d#d$d...
+00000130: 6420 9c03 6401 6425 6426 641d 8400 6420  d ..d.d%d&d...d 
+00000140: 9c03 6427 9c05 5a1c 6401 5300 2928 e900  ..d'..Z.d.S.)(..
+00000150: 0000 004e 2902 da03 4142 43da 0e61 6273  ...N)...ABC..abs
+00000160: 7472 6163 746d 6574 686f 6429 01da 0b6c  tractmethod)...l
+00000170: 6f61 645f 646f 7465 6e76 2902 da09 4175  oad_dotenv)...Au
+00000180: 746f 4d6f 6465 6cda 0d41 7574 6f54 6f6b  toModel..AutoTok
+00000190: 656e 697a 6572 7a04 2e65 6e76 2901 da0b  enizerz..env)...
+000001a0: 646f 7465 6e76 5f70 6174 687a 2673 656e  dotenv_pathz&sen
+000001b0: 7465 6e63 652d 7472 616e 7366 6f72 6d65  tence-transforme
+000001c0: 7273 2f61 6c6c 2d4d 696e 694c 4d2d 4c36  rs/all-MiniLM-L6
+000001d0: 2d76 327a 2773 656e 7465 6e63 652d 7472  -v2z'sentence-tr
+000001e0: 616e 7366 6f72 6d65 7273 2f61 6c6c 2d6d  ansformers/all-m
+000001f0: 706e 6574 2d62 6173 652d 7632 7a37 4d75  pnet-base-v2z7Mu
+00000200: 656e 6e69 6768 6f66 662f 5347 5054 2d31  ennighoff/SGPT-1
+00000210: 3235 4d2d 7765 6967 6874 6564 6d65 616e  25M-weightedmean
+00000220: 2d6d 736d 6172 636f 2d73 7065 6362 2d62  -msmarco-specb-b
+00000230: 6974 6669 747a 374d 7565 6e6e 6967 686f  itfitz7Muennigho
+00000240: 6666 2f53 4750 542d 312e 3342 2d77 6569  ff/SGPT-1.3B-wei
+00000250: 6768 7465 646d 6561 6e2d 6d73 6d61 7263  ghtedmean-msmarc
+00000260: 6f2d 7370 6563 622d 6269 7466 6974 6302  o-specb-bitfitc.
+00000270: 0000 0000 0000 0000 0000 0006 0000 0004  ................
+00000280: 0000 0043 0000 0073 4c00 0000 7c00 6401  ...C...sL...|.d.
+00000290: 1900 7d02 7c01 a000 6402 a101 a001 7c02  ..}.|...d.....|.
+000002a0: a002 a100 a101 a003 a100 7d03 7404 a005  ..........}.t...
+000002b0: 7c02 7c03 1400 6403 a102 7d04 7404 6a06  |.|...d...}.t.j.
+000002c0: 7c03 a005 6403 a101 6404 6405 8d02 7d05  |...d...d.d...}.
+000002d0: 7c04 7c05 1b00 5300 2906 4e72 0100 0000  |.|...S.).Nr....
+000002e0: e9ff ffff ffe9 0100 0000 6795 d626 e80b  ..........g..&..
+000002f0: 2e11 3e29 01da 036d 696e 2907 5a09 756e  ..>)...min).Z.un
+00000300: 7371 7565 657a 65da 0665 7870 616e 64da  squeeze..expand.
+00000310: 0473 697a 65da 0566 6c6f 6174 da05 746f  .size..float..to
+00000320: 7263 68da 0373 756d da05 636c 616d 7029  rch..sum..clamp)
+00000330: 06da 0c6d 6f64 656c 5f6f 7574 7075 74da  ...model_output.
+00000340: 0e61 7474 656e 7469 6f6e 5f6d 6173 6b5a  .attention_maskZ
+00000350: 1074 6f6b 656e 5f65 6d62 6564 6469 6e67  .token_embedding
+00000360: 735a 1369 6e70 7574 5f6d 6173 6b5f 6578  sZ.input_mask_ex
+00000370: 7061 6e64 6564 5a0e 7375 6d5f 656d 6265  pandedZ.sum_embe
+00000380: 6464 696e 6773 5a08 7375 6d5f 6d61 736b  ddingsZ.sum_mask
+00000390: a900 7213 0000 00fa 372f 5573 6572 732f  ..r.....7/Users/
+000003a0: 6672 6565 646d 616e 642f 7363 7261 7073  freedmand/scraps
+000003b0: 2f73 656d 616e 7472 612f 7372 632f 7365  /semantra/src/se
+000003c0: 6d61 6e74 7261 2f6d 6f64 656c 732e 7079  mantra/models.py
+000003d0: da0c 6d65 616e 5f70 6f6f 6c69 6e67 1300  ..mean_pooling..
+000003e0: 0000 7310 0000 0000 0102 0102 ff04 0416  ..s.............
+000003f0: ff02 0310 0114 0172 1500 0000 6301 0000  .......r....c...
+00000400: 0000 0000 0000 0000 0001 0000 0002 0000  ................
+00000410: 0043 0000 0073 0e00 0000 6401 6402 8400  .C...s....d.d...
+00000420: 7c00 4400 8301 5300 2903 4e63 0100 0000  |.D...S.).Nc....
+00000430: 0000 0000 0000 0000 0200 0000 0400 0000  ................
+00000440: 5300 0000 7318 0000 0067 007c 005d 107d  S...s....g.|.].}
+00000450: 017c 0164 0075 0172 047c 0191 0271 0453  .|.d.u.r.|...q.S
+00000460: 00a9 014e 7213 0000 0029 02da 022e 30da  ...Nr....)....0.
+00000470: 0169 7213 0000 0072 1300 0000 7214 0000  .ir....r....r...
+00000480: 00da 0a3c 6c69 7374 636f 6d70 3e20 0000  ...<listcomp> ..
+00000490: 00f3 0000 0000 7a1f 6669 6c74 6572 5f6e  ......z.filter_n
+000004a0: 6f6e 652e 3c6c 6f63 616c 733e 2e3c 6c69  one.<locals>.<li
+000004b0: 7374 636f 6d70 3e72 1300 0000 a901 da01  stcomp>r........
+000004c0: 7872 1300 0000 7213 0000 0072 1400 0000  xr....r....r....
+000004d0: da0b 6669 6c74 6572 5f6e 6f6e 651f 0000  ..filter_none...
+000004e0: 0073 0200 0000 0001 721d 0000 0063 0100  .s......r....c..
+000004f0: 0000 0000 0000 0000 0000 0100 0000 0300  ................
+00000500: 0000 4300 0000 731c 0000 0074 007c 0074  ..C...s....t.|.t
+00000510: 016a 0283 0272 187c 00a0 03a1 00a0 04a1  .j...r.|........
+00000520: 0053 007c 0053 0072 1600 0000 2905 da0a  .S.|.S.r....)...
+00000530: 6973 696e 7374 616e 6365 720e 0000 005a  isinstancer....Z
+00000540: 0654 656e 736f 72da 0363 7075 da05 6e75  .Tensor..cpu..nu
+00000550: 6d70 7972 1b00 0000 7213 0000 0072 1300  mpyr....r....r..
+00000560: 0000 7214 0000 00da 0861 735f 6e75 6d70  ..r......as_nump
+00000570: 7923 0000 0073 0600 0000 0002 0c01 0c01  y#...s..........
+00000580: 7221 0000 0063 0000 0000 0000 0000 0000  r!...c..........
+00000590: 0000 0000 0000 0500 0000 4000 0000 73b4  ..........@...s.
+000005a0: 0000 0065 005a 0164 005a 0265 0365 0464  ...e.Z.d.Z.e.e.d
+000005b0: 019c 0164 0264 0384 0483 015a 0565 0365  ...d.d.....Z.e.e
+000005c0: 0664 049c 0164 0564 0684 0483 015a 0765  .d...d.d.....Z.e
+000005d0: 0365 0464 019c 0164 0764 0884 0483 015a  .e.d...d.d.....Z
+000005e0: 0865 0365 0664 0964 0a9c 0264 0b64 0c84  .e.e.d.d...d.d..
+000005f0: 0483 015a 0965 0364 0d64 0e84 0083 015a  ...Z.e.d.d.....Z
+00000600: 0a65 0364 2165 0b64 1064 119c 0264 1264  .e.d!e.d.d...d.d
+00000610: 1384 0583 015a 0c64 1464 019c 0164 1564  .....Z.d.d...d.d
+00000620: 1684 045a 0d65 0664 1464 179c 0264 1864  ...Z.e.d.d...d.d
+00000630: 1984 045a 0e64 1464 019c 0164 1a64 1b84  ...Z.d.d...d.d..
+00000640: 045a 0f64 1c64 1d84 005a 1064 1e64 1f84  .Z.d.d...Z.d.d..
+00000650: 005a 1164 2053 0029 22da 0942 6173 654d  .Z.d S.)"..BaseM
+00000660: 6f64 656c a901 da06 7265 7475 726e 6301  odel....returnc.
+00000670: 0000 0000 0000 0000 0000 0001 0000 0001  ................
+00000680: 0000 0043 0000 0073 0400 0000 6400 5300  ...C...s....d.S.
+00000690: 7216 0000 0072 1300 0000 a901 da04 7365  r....r........se
+000006a0: 6c66 7213 0000 0072 1300 0000 7214 0000  lfr....r....r...
+000006b0: 00da 1267 6574 5f6e 756d 5f64 696d 656e  ...get_num_dimen
+000006c0: 7369 6f6e 732b 0000 0073 0200 0000 0002  sions+...s......
+000006d0: 7a1c 4261 7365 4d6f 6465 6c2e 6765 745f  z.BaseModel.get_
+000006e0: 6e75 6d5f 6469 6d65 6e73 696f 6e73 a901  num_dimensions..
+000006f0: da04 7465 7874 6302 0000 0000 0000 0000  ..textc.........
+00000700: 0000 0002 0000 0001 0000 0043 0000 0073  ...........C...s
+00000710: 0400 0000 6400 5300 7216 0000 0072 1300  ....d.S.r....r..
+00000720: 0000 a902 7226 0000 0072 2900 0000 7213  ....r&...r)...r.
+00000730: 0000 0072 1300 0000 7214 0000 00da 0a67  ...r....r......g
+00000740: 6574 5f74 6f6b 656e 732f 0000 0073 0200  et_tokens/...s..
+00000750: 0000 0002 7a14 4261 7365 4d6f 6465 6c2e  ....z.BaseModel.
+00000760: 6765 745f 746f 6b65 6e73 6302 0000 0000  get_tokensc.....
+00000770: 0000 0000 0000 0002 0000 0001 0000 0043  ...............C
+00000780: 0000 0073 0400 0000 6400 5300 7216 0000  ...s....d.S.r...
+00000790: 0072 1300 0000 a902 7226 0000 00da 0674  .r......r&.....t
+000007a0: 6f6b 656e 7372 1300 0000 7213 0000 0072  okensr....r....r
+000007b0: 1400 0000 da10 6765 745f 746f 6b65 6e5f  ......get_token_
+000007c0: 6c65 6e67 7468 3300 0000 7302 0000 0000  length3...s.....
+000007d0: 027a 1a42 6173 654d 6f64 656c 2e67 6574  .z.BaseModel.get
+000007e0: 5f74 6f6b 656e 5f6c 656e 6774 68fa 096c  _token_length..l
+000007f0: 6973 745b 7374 725d a902 7229 0000 0072  ist[str]..r)...r
+00000800: 2400 0000 6303 0000 0000 0000 0000 0000  $...c...........
+00000810: 0003 0000 0001 0000 0043 0000 0073 0400  .........C...s..
+00000820: 0000 6400 5300 7216 0000 0072 1300 0000  ..d.S.r....r....
+00000830: 2903 7226 0000 0072 2900 0000 722d 0000  ).r&...r)...r-..
+00000840: 0072 1300 0000 7213 0000 0072 1400 0000  .r....r....r....
+00000850: da0f 6765 745f 7465 7874 5f63 6875 6e6b  ..get_text_chunk
+00000860: 7337 0000 0073 0200 0000 0002 7a19 4261  s7...s......z.Ba
+00000870: 7365 4d6f 6465 6c2e 6765 745f 7465 7874  seModel.get_text
+00000880: 5f63 6875 6e6b 7363 0100 0000 0000 0000  _chunksc........
+00000890: 0000 0000 0100 0000 0100 0000 4300 0000  ............C...
+000008a0: 7304 0000 0064 0053 0072 1600 0000 7213  s....d.S.r....r.
+000008b0: 0000 0072 2500 0000 7213 0000 0072 1300  ...r%...r....r..
+000008c0: 0000 7214 0000 00da 0a67 6574 5f63 6f6e  ..r......get_con
+000008d0: 6669 673b 0000 0073 0200 0000 0002 7a14  fig;...s......z.
+000008e0: 4261 7365 4d6f 6465 6c2e 6765 745f 636f  BaseModel.get_co
+000008f0: 6e66 6967 46fa 116c 6973 745b 6c69 7374  nfigF..list[list
+00000900: 5b66 6c6f 6174 5d5d 2902 da08 6973 5f71  [float]])...is_q
+00000910: 7565 7279 7224 0000 0063 0400 0000 0000  ueryr$...c......
+00000920: 0000 0000 0000 0400 0000 0100 0000 4300  ..............C.
+00000930: 0000 7304 0000 0064 0053 0072 1600 0000  ..s....d.S.r....
+00000940: 7213 0000 0029 0472 2600 0000 722d 0000  r....).r&...r-..
+00000950: 00da 076f 6666 7365 7473 7234 0000 0072  ...offsetsr4...r
+00000960: 1300 0000 7213 0000 0072 1400 0000 da05  ....r....r......
+00000970: 656d 6265 643f 0000 0073 0200 0000 0002  embed?...s......
+00000980: 7a0f 4261 7365 4d6f 6465 6c2e 656d 6265  z.BaseModel.embe
+00000990: 647a 0b6c 6973 745b 666c 6f61 745d 6302  dz.list[float]c.
+000009a0: 0000 0000 0000 0000 0000 0003 0000 0007  ................
+000009b0: 0000 0043 0000 0073 2800 0000 7c00 a000  ...C...s(...|...
+000009c0: 7c01 a101 7d02 7c00 a001 7c02 6401 7c00  |...}.|...|.d.|.
+000009d0: a002 7c02 a101 6602 6701 6402 a103 6401  ..|...f.g.d...d.
+000009e0: 1900 5300 2903 4e72 0100 0000 46a9 0372  ..S.).Nr....F..r
+000009f0: 2b00 0000 7236 0000 0072 2e00 0000 2903  +...r6...r....).
+00000a00: 7226 0000 005a 0864 6f63 756d 656e 7472  r&...Z.documentr
+00000a10: 2d00 0000 7213 0000 0072 1300 0000 7214  -...r....r....r.
+00000a20: 0000 00da 0e65 6d62 6564 5f64 6f63 756d  .....embed_docum
+00000a30: 656e 7443 0000 0073 0400 0000 0001 0a01  entC...s........
+00000a40: 7a18 4261 7365 4d6f 6465 6c2e 656d 6265  z.BaseModel.embe
+00000a50: 645f 646f 6375 6d65 6e74 2902 da05 7175  d_document)...qu
+00000a60: 6572 7972 2400 0000 6302 0000 0000 0000  eryr$...c.......
+00000a70: 0000 0000 0003 0000 0007 0000 0043 0000  .............C..
+00000a80: 0073 2800 0000 7c00 a000 7c01 a101 7d02  .s(...|...|...}.
+00000a90: 7c00 a001 7c02 6401 7c00 a002 7c02 a101  |...|.d.|...|...
+00000aa0: 6602 6701 6402 a103 6401 1900 5300 2903  f.g.d...d...S.).
+00000ab0: 4e72 0100 0000 5472 3700 0000 2903 7226  Nr....Tr7...).r&
+00000ac0: 0000 0072 3900 0000 722d 0000 0072 1300  ...r9...r-...r..
+00000ad0: 0000 7213 0000 0072 1400 0000 da0b 656d  ..r....r......em
+00000ae0: 6265 645f 7175 6572 7947 0000 0073 0400  bed_queryG...s..
+00000af0: 0000 0001 0a01 7a15 4261 7365 4d6f 6465  ......z.BaseMode
+00000b00: 6c2e 656d 6265 645f 7175 6572 7963 0200  l.embed_queryc..
+00000b10: 0000 0000 0000 0000 0000 0300 0000 0400  ................
+00000b20: 0000 0300 0000 7320 0000 0087 0066 0164  ......s .....f.d
+00000b30: 0164 0284 087c 0144 0083 017d 0274 006a  .d...|.D...}.t.j
+00000b40: 017c 0264 0364 048d 0253 0029 054e 6301  .|.d.d...S.).Nc.
+00000b50: 0000 0000 0000 0000 0000 0002 0000 0007  ................
+00000b60: 0000 0013 0000 0073 2600 0000 6700 7c00  .......s&...g.|.
+00000b70: 5d1e 7d01 7400 8800 a001 7c01 6400 1900  ].}.t.....|.d...
+00000b80: a101 8301 7c01 6401 1900 1400 9102 7104  ....|.d.......q.
+00000b90: 5300 2902 7239 0000 00da 0677 6569 6768  S.).r9.....weigh
+00000ba0: 7429 0272 2100 0000 723a 0000 0029 0272  t).r!...r:...).r
+00000bb0: 1700 0000 7239 0000 0072 2500 0000 7213  ....r9...r%...r.
+00000bc0: 0000 0072 1400 0000 7219 0000 004c 0000  ...r....r....L..
+00000bd0: 0073 0400 0000 0602 02ff 7a2b 4261 7365  .s........z+Base
+00000be0: 4d6f 6465 6c2e 656d 6265 645f 7175 6572  Model.embed_quer
+00000bf0: 6965 732e 3c6c 6f63 616c 733e 2e3c 6c69  ies.<locals>.<li
+00000c00: 7374 636f 6d70 3e72 0100 0000 a901 da04  stcomp>r........
+00000c10: 6178 6973 2902 da02 6e70 720f 0000 0029  axis)...npr....)
+00000c20: 0372 2600 0000 da07 7175 6572 6965 735a  .r&.....queriesZ
+00000c30: 0e61 6c6c 5f65 6d62 6564 6469 6e67 7372  .all_embeddingsr
+00000c40: 1300 0000 7225 0000 0072 1400 0000 da0d  ....r%...r......
+00000c50: 656d 6265 645f 7175 6572 6965 734b 0000  embed_queriesK..
+00000c60: 0073 0800 0000 0001 0a02 02fe 0605 7a17  .s............z.
+00000c70: 4261 7365 4d6f 6465 6c2e 656d 6265 645f  BaseModel.embed_
+00000c80: 7175 6572 6965 7363 0400 0000 0000 0000  queriesc........
+00000c90: 0000 0000 0500 0000 0500 0000 0300 0000  ................
+00000ca0: 734c 0000 0074 007c 0183 0164 016b 0472  sL...t.|...d.k.r
+00000cb0: 167c 00a0 017c 01a1 016e 0264 007d 0474  .|...|...n.d.}.t
+00000cc0: 026a 0367 007c 0464 0075 0172 2e7c 0467  .j.g.|.d.u.r.|.g
+00000cd0: 016e 0267 00a2 0187 0066 0164 0264 0384  .n.g.....f.d.d..
+00000ce0: 087c 0244 0083 01a2 0164 0164 048d 0253  .|.D.....d.d...S
+00000cf0: 0029 054e 7201 0000 0063 0100 0000 0000  .).Nr....c......
+00000d00: 0000 0000 0000 0200 0000 0500 0000 1300  ................
+00000d10: 0000 7332 0000 0067 007c 005d 2a7d 0188  ..s2...g.|.]*}..
+00000d20: 007c 0164 0019 0064 0119 0019 006a 007c  .|.d...d.....j.|
+00000d30: 0164 0219 0064 0319 0019 007c 0164 0419  .d...d.....|.d..
+00000d40: 0014 0091 0271 0453 0029 05da 0466 696c  .....q.S.)...fil
+00000d50: 65da 0866 696c 656e 616d 655a 0c73 6561  e..filenameZ.sea
+00000d60: 7263 6852 6573 756c 74da 0569 6e64 6578  rchResult..index
+00000d70: 723b 0000 0029 01da 0a65 6d62 6564 6469  r;...)...embeddi
+00000d80: 6e67 7329 0272 1700 0000 5a04 7072 6566  ngs).r....Z.pref
+00000d90: a901 da09 646f 6375 6d65 6e74 7372 1300  ....documentsr..
+00000da0: 0000 7214 0000 0072 1900 0000 5900 0000  ..r....r....Y...
+00000db0: 730c 0000 0006 0502 fc10 010a ff02 0306  s...............
+00000dc0: fd7a 3b42 6173 654d 6f64 656c 2e65 6d62  .z;BaseModel.emb
+00000dd0: 6564 5f71 7565 7269 6573 5f61 6e64 5f70  ed_queries_and_p
+00000de0: 7265 6665 7265 6e63 6573 2e3c 6c6f 6361  references.<loca
+00000df0: 6c73 3e2e 3c6c 6973 7463 6f6d 703e 723c  ls>.<listcomp>r<
+00000e00: 0000 0029 04da 036c 656e 7240 0000 0072  ...)...lenr@...r
+00000e10: 3e00 0000 720f 0000 0029 0572 2600 0000  >...r....).r&...
+00000e20: 723f 0000 00da 0b70 7265 6665 7265 6e63  r?.....preferenc
+00000e30: 6573 7246 0000 005a 0f71 7565 7279 5f65  esrF...Z.query_e
+00000e40: 6d62 6564 6469 6e67 7213 0000 0072 4500  mbeddingr....rE.
+00000e50: 0000 7214 0000 00da 1d65 6d62 6564 5f71  ..r......embed_q
+00000e60: 7565 7269 6573 5f61 6e64 5f70 7265 6665  ueries_and_prefe
+00000e70: 7265 6e63 6573 5300 0000 7316 0000 0000  rencesS...s.....
+00000e80: 011a 0204 0102 0110 ff02 020a 0502 fb04  ................
+00000e90: fe02 0a02 f57a 2742 6173 654d 6f64 656c  .....z'BaseModel
+00000ea0: 2e65 6d62 6564 5f71 7565 7269 6573 5f61  .embed_queries_a
+00000eb0: 6e64 5f70 7265 6665 7265 6e63 6573 6301  nd_preferencesc.
+00000ec0: 0000 0000 0000 0000 0000 0001 0000 0001  ................
+00000ed0: 0000 0043 0000 0073 0400 0000 6401 5300  ...C...s....d.S.
+00000ee0: 2902 4e46 7213 0000 0072 2500 0000 7213  ).NFr....r%...r.
+00000ef0: 0000 0072 1300 0000 7214 0000 00da 0d69  ...r....r......i
+00000f00: 735f 6173 796d 6d65 7472 6963 6400 0000  s_asymmetricd...
+00000f10: 7302 0000 0000 017a 1742 6173 654d 6f64  s......z.BaseMod
+00000f20: 656c 2e69 735f 6173 796d 6d65 7472 6963  el.is_asymmetric
+00000f30: 4e29 0146 2912 da08 5f5f 6e61 6d65 5f5f  N).F)...__name__
+00000f40: da0a 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f  ..__module__..__
+00000f50: 7175 616c 6e61 6d65 5f5f 7203 0000 00da  qualname__r.....
+00000f60: 0369 6e74 7227 0000 00da 0373 7472 722b  .intr'.....strr+
+00000f70: 0000 0072 2e00 0000 7231 0000 0072 3200  ...r....r1...r2.
+00000f80: 0000 da04 626f 6f6c 7236 0000 0072 3800  ....boolr6...r8.
+00000f90: 0000 723a 0000 0072 4000 0000 7249 0000  ..r:...r@...rI..
+00000fa0: 0072 4a00 0000 7213 0000 0072 1300 0000  .rJ...r....r....
+00000fb0: 7213 0000 0072 1400 0000 7222 0000 002a  r....r....r"...*
+00000fc0: 0000 0073 2200 0000 0801 0201 1003 0201  ...s"...........
+00000fd0: 1003 0201 1003 0201 1203 0201 0a03 0201  ................
+00000fe0: 1403 0e04 1004 0e08 0811 7222 0000 0063  ..........r"...c
+00000ff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001000: 0400 0000 4000 0000 7368 0000 0065 005a  ....@...sh...e.Z
+00001010: 0164 005a 0264 1964 0464 0584 015a 0364  .d.Z.d.d.d...Z.d
+00001020: 0664 0784 005a 0465 0564 089c 0164 0964  .d...Z.e.d...d.d
+00001030: 0a84 045a 0665 0764 0b9c 0164 0c64 0d84  ...Z.e.d...d.d..
+00001040: 045a 0865 0564 089c 0164 0e64 0f84 045a  .Z.e.d...d.d...Z
+00001050: 0965 0764 1064 119c 0264 1264 1384 045a  .e.d.d...d.d...Z
+00001060: 0a64 1a64 1564 089c 0164 1664 1784 055a  .d.d.d...d.d...Z
+00001070: 0b64 1853 0029 1bda 0b4f 7065 6e41 494d  .d.S.)...OpenAIM
+00001080: 6f64 656c fa16 7465 7874 2d65 6d62 6564  odel..text-embed
+00001090: 6469 6e67 2d61 6461 2d30 3032 e900 0600  ding-ada-002....
+000010a0: 00da 0b63 6c31 3030 6b5f 6261 7365 6304  ...cl100k_basec.
+000010b0: 0000 0000 0000 0000 0000 0004 0000 0003  ................
+000010c0: 0000 0043 0000 0073 3a00 0000 6401 7400  ...C...s:...d.t.
+000010d0: 6a01 7601 7212 7402 6402 8301 8201 7400  j.v.r.t.d.....t.
+000010e0: a003 6401 a101 7404 5f05 7c01 7c00 5f06  ..d...t._.|.|._.
+000010f0: 7c02 7c00 5f07 7408 a009 7c03 a101 7c00  |.|._.t...|...|.
+00001100: 5f0a 6400 5300 2903 4e5a 0e4f 5045 4e41  _.d.S.).NZ.OPENA
+00001110: 495f 4150 495f 4b45 597a e84f 7065 6e41  I_API_KEYz.OpenA
+00001120: 4920 4150 4920 6b65 7920 6e6f 7420 7365  I API key not se
+00001130: 742e 2050 6c65 6173 6520 7365 7420 7468  t. Please set th
+00001140: 6520 4f50 454e 4149 5f41 5049 5f4b 4559  e OPENAI_API_KEY
+00001150: 2065 6e76 6972 6f6e 6d65 6e74 2076 6172   environment var
+00001160: 6961 626c 6520 6f72 2063 7265 6174 6520  iable or create 
+00001170: 6120 602e 656e 7660 2066 696c 6520 7769  a `.env` file wi
+00001180: 7468 2074 6865 206b 6579 2069 6e20 7468  th the key in th
+00001190: 6520 6375 7272 656e 7420 776f 726b 696e  e current workin
+000011a0: 6720 6469 7265 6374 6f72 7920 6f72 2074  g directory or t
+000011b0: 6865 2053 656d 616e 7472 6120 6469 7265  he Semantra dire
+000011c0: 6374 6f72 792c 2077 6869 6368 2069 7320  ctory, which is 
+000011d0: 7265 7665 616c 6564 2062 7920 7275 6e6e  revealed by runn
+000011e0: 696e 6720 6073 656d 616e 7472 6120 2d2d  ing `semantra --
+000011f0: 7368 6f77 2d73 656d 616e 7472 612d 6469  show-semantra-di
+00001200: 7260 2e29 0bda 026f 73da 0765 6e76 6972  r`.)...os..envir
+00001210: 6f6e da09 4578 6365 7074 696f 6eda 0667  on..Exception..g
+00001220: 6574 656e 76da 066f 7065 6e61 695a 0761  etenv..openaiZ.a
+00001230: 7069 5f6b 6579 da0a 6d6f 6465 6c5f 6e61  pi_key..model_na
+00001240: 6d65 da0e 6e75 6d5f 6469 6d65 6e73 696f  me..num_dimensio
+00001250: 6e73 da08 7469 6b74 6f6b 656e 5a0c 6765  ns..tiktokenZ.ge
+00001260: 745f 656e 636f 6469 6e67 da09 746f 6b65  t_encoding..toke
+00001270: 6e69 7a65 7229 0472 2600 0000 725a 0000  nizer).r&...rZ..
+00001280: 0072 5b00 0000 da0e 746f 6b65 6e69 7a65  .r[.....tokenize
+00001290: 725f 6e61 6d65 7213 0000 0072 1300 0000  r_namer....r....
+000012a0: 7214 0000 00da 085f 5f69 6e69 745f 5f69  r......__init__i
+000012b0: 0000 0073 1000 0000 0007 0a01 0201 02ff  ...s............
+000012c0: 0404 0c02 0601 0601 7a14 4f70 656e 4149  ........z.OpenAI
+000012d0: 4d6f 6465 6c2e 5f5f 696e 6974 5f5f 6301  Model.__init__c.
+000012e0: 0000 0000 0000 0000 0000 0001 0000 0004  ................
+000012f0: 0000 0043 0000 0073 1200 0000 6401 7c00  ...C...s....d.|.
+00001300: 6a00 7c00 6a01 6a02 6402 9c03 5300 2903  j.|.j.j.d...S.).
+00001310: 4e72 5900 0000 2903 da0a 6d6f 6465 6c5f  NrY...)...model_
+00001320: 7479 7065 725a 0000 0072 5e00 0000 2903  typerZ...r^...).
+00001330: 725a 0000 0072 5d00 0000 da04 6e61 6d65  rZ...r].....name
+00001340: 7225 0000 0072 1300 0000 7213 0000 0072  r%...r....r....r
+00001350: 1400 0000 7232 0000 007b 0000 0073 0800  ....r2...{...s..
+00001360: 0000 0002 0201 0401 06fd 7a16 4f70 656e  ..........z.Open
+00001370: 4149 4d6f 6465 6c2e 6765 745f 636f 6e66  AIModel.get_conf
+00001380: 6967 7223 0000 0063 0100 0000 0000 0000  igr#...c........
+00001390: 0000 0000 0100 0000 0100 0000 4300 0000  ............C...
+000013a0: 7306 0000 007c 006a 0053 0072 1600 0000  s....|.j.S.r....
+000013b0: 2901 725b 0000 0072 2500 0000 7213 0000  ).r[...r%...r...
+000013c0: 0072 1300 0000 7214 0000 0072 2700 0000  .r....r....r'...
+000013d0: 8200 0000 7302 0000 0000 017a 1e4f 7065  ....s......z.Ope
+000013e0: 6e41 494d 6f64 656c 2e67 6574 5f6e 756d  nAIModel.get_num
+000013f0: 5f64 696d 656e 7369 6f6e 7372 2800 0000  _dimensionsr(...
+00001400: 6302 0000 0000 0000 0000 0000 0002 0000  c...............
+00001410: 0003 0000 0043 0000 0073 0c00 0000 7c00  .....C...s....|.
+00001420: 6a00 a001 7c01 a101 5300 7216 0000 0029  j...|...S.r....)
+00001430: 0272 5d00 0000 da06 656e 636f 6465 722a  .r].....encoder*
+00001440: 0000 0072 1300 0000 7213 0000 0072 1400  ...r....r....r..
+00001450: 0000 722b 0000 0085 0000 0073 0200 0000  ..r+.......s....
+00001460: 0001 7a16 4f70 656e 4149 4d6f 6465 6c2e  ..z.OpenAIModel.
+00001470: 6765 745f 746f 6b65 6e73 6302 0000 0000  get_tokensc.....
+00001480: 0000 0000 0000 0002 0000 0002 0000 0043  ...............C
+00001490: 0000 0073 0800 0000 7400 7c01 8301 5300  ...s....t.|...S.
+000014a0: 7216 0000 00a9 0172 4700 0000 722c 0000  r......rG...r,..
+000014b0: 0072 1300 0000 7213 0000 0072 1400 0000  .r....r....r....
+000014c0: 722e 0000 0088 0000 0073 0200 0000 0001  r........s......
+000014d0: 7a1c 4f70 656e 4149 4d6f 6465 6c2e 6765  z.OpenAIModel.ge
+000014e0: 745f 746f 6b65 6e5f 6c65 6e67 7468 722f  t_token_lengthr/
+000014f0: 0000 0029 02da 015f 7224 0000 0063 0300  ...)..._r$...c..
+00001500: 0000 0000 0000 0000 0000 0300 0000 0300  ................
+00001510: 0000 0300 0000 7312 0000 0087 0066 0164  ......s......f.d
+00001520: 0164 0284 087c 0244 0083 0153 0029 034e  .d...|.D...S.).N
+00001530: 6301 0000 0000 0000 0000 0000 0002 0000  c...............
+00001540: 0005 0000 0013 0000 0073 1a00 0000 6700  .........s....g.
+00001550: 7c00 5d12 7d01 8800 6a00 a001 7c01 6701  |.].}...j...|.g.
+00001560: a101 9102 7104 5300 7213 0000 0029 0272  ....q.S.r....).r
+00001570: 5d00 0000 da06 6465 636f 6465 2902 7217  ].....decode).r.
+00001580: 0000 00da 0574 6f6b 656e 7225 0000 0072  .....tokenr%...r
+00001590: 1300 0000 7214 0000 0072 1900 0000 8c00  ....r....r......
+000015a0: 0000 721a 0000 007a 2f4f 7065 6e41 494d  ..r....z/OpenAIM
+000015b0: 6f64 656c 2e67 6574 5f74 6578 745f 6368  odel.get_text_ch
+000015c0: 756e 6b73 2e3c 6c6f 6361 6c73 3e2e 3c6c  unks.<locals>.<l
+000015d0: 6973 7463 6f6d 703e 7213 0000 0029 0372  istcomp>r....).r
+000015e0: 2600 0000 7264 0000 0072 2d00 0000 7213  &...rd...r-...r.
+000015f0: 0000 0072 2500 0000 7214 0000 0072 3100  ...r%...r....r1.
+00001600: 0000 8b00 0000 7302 0000 0000 017a 1b4f  ......s......z.O
+00001610: 7065 6e41 494d 6f64 656c 2e67 6574 5f74  penAIModel.get_t
+00001620: 6578 745f 6368 756e 6b73 4672 3300 0000  ext_chunksFr3...
+00001630: 6304 0000 0000 0000 0000 0000 0006 0000  c...............
+00001640: 0005 0000 0003 0000 0073 3c00 0000 8700  .........s<.....
+00001650: 6601 6401 6402 8408 7c02 4400 8301 7d04  f.d.d...|.D...}.
+00001660: 7400 6a01 6a02 7c00 6a03 7c04 6403 8d02  t.j.j.|.j.|.d...
+00001670: 7d05 7404 a005 6404 6402 8400 7c05 6405  }.t...d.d...|.d.
+00001680: 1900 4400 8301 a101 5300 2906 4e63 0100  ..D.....S.).Nc..
+00001690: 0000 0000 0000 0000 0000 0300 0000 0500  ................
+000016a0: 0000 1300 0000 731c 0000 0067 007c 005d  ......s....g.|.]
+000016b0: 145c 027d 017d 0288 007c 017c 0285 0219  .\.}.}...|.|....
+000016c0: 0091 0271 0453 0072 1300 0000 7213 0000  ...q.S.r....r...
+000016d0: 00a9 0372 1700 0000 7218 0000 00da 016a  ...r....r......j
+000016e0: a901 722d 0000 0072 1300 0000 7214 0000  ..r-...r....r...
+000016f0: 0072 1900 0000 8f00 0000 721a 0000 007a  .r........r....z
+00001700: 254f 7065 6e41 494d 6f64 656c 2e65 6d62  %OpenAIModel.emb
+00001710: 6564 2e3c 6c6f 6361 6c73 3e2e 3c6c 6973  ed.<locals>.<lis
+00001720: 7463 6f6d 703e 2902 da05 6d6f 6465 6cda  tcomp>)...model.
+00001730: 0569 6e70 7574 6301 0000 0000 0000 0000  .inputc.........
+00001740: 0000 0002 0000 0004 0000 0053 0000 0073  ...........S...s
+00001750: 1400 0000 6700 7c00 5d0c 7d01 7c01 6400  ....g.|.].}.|.d.
+00001760: 1900 9102 7104 5300 2901 da09 656d 6265  ....q.S.)...embe
+00001770: 6464 696e 6772 1300 0000 2902 7217 0000  ddingr....).r...
+00001780: 00da 0464 6174 6172 1300 0000 7213 0000  ...datar....r...
+00001790: 0072 1400 0000 7219 0000 0091 0000 0072  .r....r........r
+000017a0: 1a00 0000 726d 0000 0029 0672 5900 0000  ....rm...).rY...
+000017b0: 5a09 456d 6265 6464 696e 67da 0663 7265  Z.Embedding..cre
+000017c0: 6174 6572 5a00 0000 723e 0000 00da 0561  aterZ...r>.....a
+000017d0: 7272 6179 2906 7226 0000 0072 2d00 0000  rray).r&...r-...
+000017e0: 7235 0000 005a 095f 6973 5f71 7565 7279  r5...Z._is_query
+000017f0: 5a05 7465 7874 73da 0872 6573 706f 6e73  Z.texts..respons
+00001800: 6572 1300 0000 7269 0000 0072 1400 0000  er....ri...r....
+00001810: 7236 0000 008e 0000 0073 0600 0000 0001  r6.......s......
+00001820: 1201 1201 7a11 4f70 656e 4149 4d6f 6465  ....z.OpenAIMode
+00001830: 6c2e 656d 6265 644e 2903 7252 0000 0072  l.embedN).rR...r
+00001840: 5300 0000 7254 0000 0029 0146 290c 724b  S...rT...).F).rK
+00001850: 0000 0072 4c00 0000 724d 0000 0072 5f00  ...rL...rM...r_.
+00001860: 0000 7232 0000 0072 4e00 0000 7227 0000  ..r2...rN...r'..
+00001870: 0072 4f00 0000 722b 0000 0072 2e00 0000  .rO...r+...r....
+00001880: 7231 0000 0072 3600 0000 7213 0000 0072  r1...r6...r....r
+00001890: 1300 0000 7213 0000 0072 1400 0000 7251  ....r....r....rQ
+000018a0: 0000 0068 0000 0073 1400 0000 0803 0001  ...h...s........
+000018b0: 0001 00fc 0a12 0807 0e03 0e03 0e03 1003  ................
+000018c0: 7251 0000 0063 0100 0000 0000 0000 0000  rQ...c..........
+000018d0: 0000 0100 0000 0200 0000 4300 0000 7310  ..........C...s.
+000018e0: 0000 007c 0064 0075 0072 0c64 0153 007c  ...|.d.u.r.d.S.|
+000018f0: 0053 0029 024e 7201 0000 0072 1300 0000  .S.).Nr....r....
+00001900: 721b 0000 0072 1300 0000 7213 0000 0072  r....r....r....r
+00001910: 1400 0000 da0c 7a65 726f 5f69 665f 6e6f  ......zero_if_no
+00001920: 6e65 9400 0000 7302 0000 0000 0172 7100  ne....s......rq.
+00001930: 0000 6300 0000 0000 0000 0000 0000 0000  ..c.............
+00001940: 0000 0006 0000 0040 0000 0073 8000 0000  .......@...s....
+00001950: 6500 5a01 6400 5a02 641c 6403 6404 8401  e.Z.d.Z.d.d.d...
+00001960: 5a03 6405 6406 8400 5a04 6407 6408 8400  Z.d.d...Z.d.d...
+00001970: 5a05 6506 6409 9c01 640a 640b 8404 5a07  Z.e.d...d.d...Z.
+00001980: 6508 640c 9c01 640d 640e 8404 5a09 6506  e.d...d.d...Z.e.
+00001990: 6409 9c01 640f 6410 8404 5a0a 6508 6411  d...d.d...Z.e.d.
+000019a0: 6412 9c02 6413 6414 8404 5a0b 6415 6416  d...d.d...Z.d.d.
+000019b0: 8400 5a0c 6417 6418 8400 5a0d 641d 6419  ..Z.d.d...Z.d.d.
+000019c0: 6409 9c01 641a 641b 8405 5a0e 6401 5300  d...d.d...Z.d.S.
+000019d0: 291e da10 5472 616e 7366 6f72 6d65 724d  )...TransformerM
+000019e0: 6f64 656c 4e46 6308 0000 0000 0000 0000  odelNFc.........
+000019f0: 0000 0008 0000 0004 0000 0043 0000 0073  ...........C...s
+00001a00: c800 0000 7c07 6400 7500 7212 7400 6a01  ....|.d.u.r.t.j.
+00001a10: a002 a100 7d07 7c01 7c00 5f03 7404 a005  ....}.|.|._.t...
+00001a20: 7c01 a101 7c00 5f06 7407 a005 7c01 a101  |...|._.t...|...
+00001a30: 7c00 5f08 7c02 7c03 7c04 7c05 6704 7c00  |._.|.|.|.|.g.|.
+00001a40: 5f09 7c02 7252 7c00 6a06 6a0a 7c02 6401  _.|.rR|.j.j.|.d.
+00001a50: 6402 8d02 6e02 6400 7c00 5f0b 7c03 726c  d...n.d.|._.|.rl
+00001a60: 7c00 6a06 6a0a 7c03 6401 6402 8d02 6e02  |.j.j.|.d.d...n.
+00001a70: 6400 7c00 5f0c 7c04 7286 7c00 6a06 6a0a  d.|._.|.r.|.j.j.
+00001a80: 7c04 6401 6402 8d02 6e02 6400 7c00 5f0d  |.d.d...n.d.|._.
+00001a90: 7c05 72a0 7c00 6a06 6a0a 7c05 6401 6402  |.r.|.j.j.|.d.d.
+00001aa0: 8d02 6e02 6400 7c00 5f0e 7c06 7c00 5f0f  ..n.d.|._.|.|._.
+00001ab0: 7c07 7c00 5f01 7c00 6a01 72c4 7c00 6a08  |.|._.|.j.r.|.j.
+00001ac0: a001 a100 7c00 5f08 6400 5300 2903 4e46  ....|._.d.S.).NF
+00001ad0: 2901 5a12 6164 645f 7370 6563 6961 6c5f  ).Z.add_special_
+00001ae0: 746f 6b65 6e73 2910 720e 0000 00da 0463  tokens).r......c
+00001af0: 7564 615a 0c69 735f 6176 6169 6c61 626c  udaZ.is_availabl
+00001b00: 6572 5a00 0000 7206 0000 005a 0f66 726f  erZ...r....Z.fro
+00001b10: 6d5f 7072 6574 7261 696e 6564 725d 0000  m_pretrainedr]..
+00001b20: 0072 0500 0000 726a 0000 00da 0f70 7265  .r....rj.....pre
+00001b30: 5f70 6f73 745f 746f 6b65 6e73 7262 0000  _post_tokensrb..
+00001b40: 00da 0d64 6f63 5f74 6f6b 656e 5f70 7265  ...doc_token_pre
+00001b50: da0e 646f 635f 746f 6b65 6e5f 706f 7374  ..doc_token_post
+00001b60: da0f 7175 6572 795f 746f 6b65 6e5f 7072  ..query_token_pr
+00001b70: 65da 1071 7565 7279 5f74 6f6b 656e 5f70  e..query_token_p
+00001b80: 6f73 74da 0a61 7379 6d6d 6574 7269 6329  ost..asymmetric)
+00001b90: 0872 2600 0000 725a 0000 0072 7500 0000  .r&...rZ...ru...
+00001ba0: 7276 0000 0072 7700 0000 7278 0000 0072  rv...rw...rx...r
+00001bb0: 7900 0000 7273 0000 0072 1300 0000 7213  y...rs...r....r.
+00001bc0: 0000 0072 1400 0000 725f 0000 0099 0000  ...r....r_......
+00001bd0: 0073 3c00 0000 000a 0801 0a01 0601 0c01  .s<.............
+00001be0: 0c04 0201 0201 0201 02fc 0608 02ff 1202  ................
+00001bf0: 02fd 0407 02ff 1202 02fd 0407 02ff 1202  ................
+00001c00: 02fd 0407 02ff 1202 02fd 0406 0602 0601  ................
+00001c10: 0601 7a19 5472 616e 7366 6f72 6d65 724d  ..z.TransformerM
+00001c20: 6f64 656c 2e5f 5f69 6e69 745f 5f63 0100  odel.__init__c..
+00001c30: 0000 0000 0000 0000 0000 0100 0000 0800  ................
+00001c40: 0000 4300 0000 7330 0000 0064 017c 006a  ..C...s0...d.|.j
+00001c50: 007c 006a 0164 0219 007c 006a 0164 0319  .|.j.d...|.j.d..
+00001c60: 007c 006a 0164 0419 007c 006a 0164 0519  .|.j.d...|.j.d..
+00001c70: 007c 006a 0264 069c 0753 0029 074e da0c  .|.j.d...S.).N..
+00001c80: 7472 616e 7366 6f72 6d65 7273 7201 0000  transformersr...
+00001c90: 0072 0900 0000 e902 0000 00e9 0300 0000  .r..............
+00001ca0: 2907 7260 0000 0072 5a00 0000 7275 0000  ).r`...rZ...ru..
+00001cb0: 0072 7600 0000 7277 0000 0072 7800 0000  .rv...rw...rx...
+00001cc0: 7279 0000 0029 0372 5a00 0000 7274 0000  ry...).rZ...rt..
+00001cd0: 0072 7900 0000 7225 0000 0072 1300 0000  .ry...r%...r....
+00001ce0: 7213 0000 0072 1400 0000 7232 0000 00cb  r....r....r2....
+00001cf0: 0000 0073 1000 0000 0002 0201 0401 0801  ...s............
+00001d00: 0801 0801 0801 04f9 7a1b 5472 616e 7366  ........z.Transf
+00001d10: 6f72 6d65 724d 6f64 656c 2e67 6574 5f63  ormerModel.get_c
+00001d20: 6f6e 6669 6763 0100 0000 0000 0000 0000  onfigc..........
+00001d30: 0000 0100 0000 0100 0000 4300 0000 7306  ..........C...s.
+00001d40: 0000 007c 006a 0053 0072 1600 0000 2901  ...|.j.S.r....).
+00001d50: 7279 0000 0072 2500 0000 7213 0000 0072  ry...r%...r....r
+00001d60: 1300 0000 7214 0000 0072 4a00 0000 d600  ....r....rJ.....
+00001d70: 0000 7302 0000 0000 017a 1e54 7261 6e73  ..s......z.Trans
+00001d80: 666f 726d 6572 4d6f 6465 6c2e 6973 5f61  formerModel.is_a
+00001d90: 7379 6d6d 6574 7269 6372 2300 0000 6301  symmetricr#...c.
+00001da0: 0000 0000 0000 0000 0000 0001 0000 0002  ................
+00001db0: 0000 0043 0000 0073 0e00 0000 7400 7c00  ...C...s....t.|.
+00001dc0: 6a01 6a02 6a03 8301 5300 7216 0000 0029  j.j.j...S.r....)
+00001dd0: 0472 4e00 0000 726a 0000 00da 0663 6f6e  .rN...rj.....con
+00001de0: 6669 675a 0b68 6964 6465 6e5f 7369 7a65  figZ.hidden_size
+00001df0: 7225 0000 0072 1300 0000 7213 0000 0072  r%...r....r....r
+00001e00: 1400 0000 7227 0000 00d9 0000 0073 0200  ....r'.......s..
+00001e10: 0000 0001 7a23 5472 616e 7366 6f72 6d65  ....z#Transforme
+00001e20: 724d 6f64 656c 2e67 6574 5f6e 756d 5f64  rModel.get_num_d
+00001e30: 696d 656e 7369 6f6e 7372 2800 0000 6302  imensionsr(...c.
+00001e40: 0000 0000 0000 0000 0000 0002 0000 0006  ................
+00001e50: 0000 0043 0000 0073 1200 0000 7c00 6a00  ...C...s....|.j.
+00001e60: 7c01 6401 6402 6403 6404 8d04 5300 2905  |.d.d.d.d...S.).
+00001e70: 4e54 46da 0270 7429 035a 1672 6574 7572  NTF..pt).Z.retur
+00001e80: 6e5f 6f66 6673 6574 735f 6d61 7070 696e  n_offsets_mappin
+00001e90: 67da 0776 6572 626f 7365 5a0e 7265 7475  g..verboseZ.retu
+00001ea0: 726e 5f74 656e 736f 7273 2901 725d 0000  rn_tensors).r]..
+00001eb0: 0072 2a00 0000 7213 0000 0072 1300 0000  .r*...r....r....
+00001ec0: 7214 0000 0072 2b00 0000 dc00 0000 7306  r....r+.......s.
+00001ed0: 0000 0000 0104 0108 ff7a 1b54 7261 6e73  .........z.Trans
+00001ee0: 666f 726d 6572 4d6f 6465 6c2e 6765 745f  formerModel.get_
+00001ef0: 746f 6b65 6e73 6302 0000 0000 0000 0000  tokensc.........
+00001f00: 0000 0002 0000 0003 0000 0043 0000 0073  ...........C...s
+00001f10: 1000 0000 7400 7c01 6401 1900 6402 1900  ....t.|.d...d...
+00001f20: 8301 5300 2903 4eda 0969 6e70 7574 5f69  ..S.).N..input_i
+00001f30: 6473 7201 0000 0072 6300 0000 722c 0000  dsr....rc...r,..
+00001f40: 0072 1300 0000 7213 0000 0072 1400 0000  .r....r....r....
+00001f50: 722e 0000 00e1 0000 0073 0200 0000 0001  r........s......
+00001f60: 7a21 5472 616e 7366 6f72 6d65 724d 6f64  z!TransformerMod
+00001f70: 656c 2e67 6574 5f74 6f6b 656e 5f6c 656e  el.get_token_len
+00001f80: 6774 6872 2f00 0000 7230 0000 0063 0300  gthr/...r0...c..
+00001f90: 0000 0000 0000 0000 0000 0a00 0000 0600  ................
+00001fa0: 0000 4300 0000 73a6 0000 007c 0264 0119  ..C...s....|.d..
+00001fb0: 0064 0219 007d 0367 007d 0464 007d 0564  .d...}.g.}.d.}.d
+00001fc0: 007d 067c 0344 005d 665c 027d 077d 087c  .}.|.D.]f\.}.}.|
+00001fd0: 077c 086b 0272 307c 066e 027c 077d 097c  .|.k.r0|.n.|.}.|
+00001fe0: 0564 0075 0172 4e7c 04a0 007c 017c 057c  .d.u.rN|...|.|.|
+00001ff0: 0985 0219 00a1 0101 007c 0564 0075 0072  .........|.d.u.r
+00002000: 5c64 027d 056e 0c7c 097c 056b 0472 687c  \d.}.n.|.|.k.rh|
+00002010: 097d 057c 0664 0075 0072 767c 087d 0671  .}.|.d.u.rv|.}.q
+00002020: 1c7c 087c 066b 0472 1c7c 087d 0671 1c7c  .|.|.k.r.|.}.q.|
+00002030: 04a0 007c 017c 0564 0075 0072 9664 026e  ...|.|.d.u.r.d.n
+00002040: 027c 0564 0085 0219 00a1 0101 007c 0453  .|.d.........|.S
+00002050: 0029 034e 5a0e 6f66 6673 6574 5f6d 6170  .).NZ.offset_map
+00002060: 7069 6e67 7201 0000 0029 01da 0661 7070  pingr....)...app
+00002070: 656e 6429 0a72 2600 0000 7229 0000 0072  end).r&...r)...r
+00002080: 2d00 0000 7235 0000 00da 0663 6875 6e6b  -...r5.....chunk
+00002090: 735a 0670 7265 765f 695a 0670 7265 765f  sZ.prev_iZ.prev_
+000020a0: 6a72 1800 0000 7268 0000 005a 056e 6577  jr....rh...Z.new
+000020b0: 5f69 7213 0000 0072 1300 0000 7214 0000  _ir....r....r...
+000020c0: 0072 3100 0000 e400 0000 7324 0000 0000  .r1.......s$....
+000020d0: 010c 0104 0104 0104 010c 0110 0108 0112  ................
+000020e0: 0108 0106 0108 0104 0108 0106 0108 0106  ................
+000020f0: 011e 017a 2054 7261 6e73 666f 726d 6572  ...z Transformer
+00002100: 4d6f 6465 6c2e 6765 745f 7465 7874 5f63  Model.get_text_c
+00002110: 6875 6e6b 7363 0300 0000 0000 0000 0000  hunksc..........
+00002120: 0000 0500 0000 0800 0000 4300 0000 7374  ..........C...st
+00002130: 0000 007c 006a 0064 0075 0072 187c 006a  ...|.j.d.u.r.|.j
+00002140: 0164 0075 0072 187c 0153 007c 0272 227c  .d.u.r.|.S.|.r"|
+00002150: 006a 006e 047c 006a 027d 037c 0272 327c  .j.n.|.j.}.|.r2|
+00002160: 006a 016e 047c 006a 037d 0474 04a0 0574  .j.n.|.j.}.t...t
+00002170: 067c 0364 0075 0172 5074 04a0 077c 03a1  .|.d.u.rPt...|..
+00002180: 016e 0264 007c 017c 0464 0075 0172 6674  .n.d.|.|.d.u.rft
+00002190: 04a0 077c 04a1 016e 0264 0067 0383 01a1  ...|...n.d.g....
+000021a0: 0153 0064 0053 0072 1600 0000 2908 7277  .S.d.S.r....).rw
+000021b0: 0000 0072 7800 0000 7275 0000 0072 7600  ...rx...ru...rv.
+000021c0: 0000 720e 0000 00da 0363 6174 721d 0000  ..r......catr...
+000021d0: 00da 0674 656e 736f 7229 0572 2600 0000  ...tensor).r&...
+000021e0: 7280 0000 0072 3400 0000 da09 746f 6b65  r....r4.....toke
+000021f0: 6e5f 7072 65da 0a74 6f6b 656e 5f70 6f73  n_pre..token_pos
+00002200: 7472 1300 0000 7213 0000 0072 1400 0000  tr....r....r....
+00002210: da13 6e6f 726d 616c 697a 655f 696e 7075  ..normalize_inpu
+00002220: 745f 6964 73f8 0000 0073 1800 0000 0001  t_ids....s......
+00002230: 1401 0402 1001 1001 0401 0202 1401 0201  ................
+00002240: 14fd 02ff 02ff 7a24 5472 616e 7366 6f72  ......z$Transfor
+00002250: 6d65 724d 6f64 656c 2e6e 6f72 6d61 6c69  merModel.normali
+00002260: 7a65 5f69 6e70 7574 5f69 6473 6303 0000  ze_input_idsc...
+00002270: 0000 0000 0000 0000 0005 0000 0009 0000  ................
+00002280: 0043 0000 0073 7c00 0000 7c00 6a00 6400  .C...s|...|.j.d.
+00002290: 7500 7218 7c00 6a01 6400 7500 7218 7c01  u.r.|.j.d.u.r.|.
+000022a0: 5300 7c02 7222 7c00 6a00 6e04 7c00 6a02  S.|.r"|.j.n.|.j.
+000022b0: 7d03 7c02 7232 7c00 6a01 6e04 7c00 6a03  }.|.r2|.j.n.|.j.
+000022c0: 7d04 7404 a005 7406 7c03 6400 7501 7254  }.t...t.|.d.u.rT
+000022d0: 7404 a007 7408 7c03 8301 a101 6e02 6400  t...t.|.....n.d.
+000022e0: 7c01 7c04 6400 7501 726e 7404 a007 7408  |.|.d.u.rnt...t.
+000022f0: 7c04 8301 a101 6e02 6400 6703 8301 a101  |.....n.d.g.....
+00002300: 5300 6400 5300 7216 0000 0029 0972 7700  S.d.S.r....).rw.
+00002310: 0000 7278 0000 0072 7500 0000 7276 0000  ..rx...ru...rv..
+00002320: 0072 0e00 0000 7283 0000 0072 1d00 0000  .r....r....r....
+00002330: da04 6f6e 6573 7247 0000 0029 0572 2600  ..onesrG...).r&.
+00002340: 0000 7212 0000 0072 3400 0000 7285 0000  ..r....r4...r...
+00002350: 0072 8600 0000 7213 0000 0072 1300 0000  .r....r....r....
+00002360: 7214 0000 00da 186e 6f72 6d61 6c69 7a65  r......normalize
+00002370: 5f61 7474 656e 7469 6f6e 5f6d 6173 6b08  _attention_mask.
+00002380: 0100 0073 1800 0000 0001 1401 0402 1001  ...s............
+00002390: 1001 0401 0202 1801 0201 18fd 02ff 02ff  ................
+000023a0: 7a29 5472 616e 7366 6f72 6d65 724d 6f64  z)TransformerMod
+000023b0: 656c 2e6e 6f72 6d61 6c69 7a65 5f61 7474  el.normalize_att
+000023c0: 656e 7469 6f6e 5f6d 6173 6b72 3300 0000  ention_maskr3...
+000023d0: 6304 0000 0000 0000 0000 0000 0007 0000  c...............
+000023e0: 0008 0000 0003 0000 0073 ae00 0000 7400  .........s....t.
+000023f0: 6a01 6a02 6a03 6a04 8700 8701 8702 6603  j.j.j.j.......f.
+00002400: 6401 6402 8408 7c02 4400 8301 6403 7405  d.d...|.D...d.t.
+00002410: 8801 6a06 6a07 8301 6404 8d03 7d04 7400  ..j.j...d...}.t.
+00002420: 6a01 6a02 6a03 6a04 8700 8701 8702 6603  j.j.j.j.......f.
+00002430: 6405 6402 8408 7c02 4400 8301 6403 6406  d.d...|.D...d.d.
+00002440: 6404 8d03 7d05 8801 6a08 726e 7c04 a008  d...}...j.rn|...
+00002450: a100 7d04 7c05 a008 a100 7d05 7400 a009  ..}.|.....}.t...
+00002460: a100 8f1e 0100 8801 6a0a 7c04 7c05 6407  ........j.|.|.d.
+00002470: 8d02 7d06 5700 6400 0400 0400 8303 0100  ..}.W.d.........
+00002480: 6e10 3100 739a 3000 0100 0100 0100 5900  n.1.s.0.......Y.
+00002490: 0100 740b 7c06 7c05 8302 5300 2908 4e63  ..t.|.|...S.).Nc
+000024a0: 0100 0000 0000 0000 0000 0000 0300 0000  ................
+000024b0: 0c00 0000 1300 0000 7338 0000 0067 007c  ........s8...g.|
+000024c0: 005d 305c 027d 017d 0288 01a0 0088 0264  .]0\.}.}.......d
+000024d0: 0019 0064 0119 00a0 0164 0174 02a0 0374  ...d.....d.t...t
+000024e0: 047c 017c 0283 02a1 01a1 0288 00a1 0291  .|.|............
+000024f0: 0271 0453 0029 0272 8000 0000 7201 0000  .q.S.).r....r...
+00002500: 0029 0572 8700 0000 da0c 696e 6465 785f  .).r......index_
+00002510: 7365 6c65 6374 720e 0000 0072 8400 0000  selectr....r....
+00002520: da05 7261 6e67 6572 6700 0000 a903 7234  ..rangerg.....r4
+00002530: 0000 0072 2600 0000 722d 0000 0072 1300  ...r&...r-...r..
+00002540: 0000 7214 0000 0072 1900 0000 1a01 0000  ..r....r........
+00002550: 730a 0000 0006 0506 fc04 011e 0102 fe7a  s..............z
+00002560: 2a54 7261 6e73 666f 726d 6572 4d6f 6465  *TransformerMode
+00002570: 6c2e 656d 6265 642e 3c6c 6f63 616c 733e  l.embed.<locals>
+00002580: 2e3c 6c69 7374 636f 6d70 3e54 2902 5a0b  .<listcomp>T).Z.
+00002590: 6261 7463 685f 6669 7273 745a 0d70 6164  batch_firstZ.pad
+000025a0: 6469 6e67 5f76 616c 7565 6301 0000 0000  ding_valuec.....
+000025b0: 0000 0000 0000 0003 0000 000c 0000 0013  ................
+000025c0: 0000 0073 3800 0000 6700 7c00 5d30 5c02  ...s8...g.|.]0\.
+000025d0: 7d01 7d02 8801 a000 8802 6400 1900 6401  }.}.......d...d.
+000025e0: 1900 a001 6401 7402 a003 7404 7c01 7c02  ....d.t...t.|.|.
+000025f0: 8302 a101 a102 8800 a102 9102 7104 5300  ............q.S.
+00002600: 2902 7212 0000 0072 0100 0000 2905 7289  ).r....r....).r.
+00002610: 0000 0072 8a00 0000 720e 0000 0072 8400  ...r....r....r..
+00002620: 0000 728b 0000 0072 6700 0000 728c 0000  ..r....rg...r...
+00002630: 0072 1300 0000 7214 0000 0072 1900 0000  .r....r....r....
+00002640: 2501 0000 730e 0000 0006 0706 fa04 010c  %...s...........
+00002650: 0110 ff02 0302 fc72 0100 0000 2902 7280  .......r....).r.
+00002660: 0000 0072 1200 0000 290c 720e 0000 00da  ...r....).r.....
+00002670: 026e 6eda 0575 7469 6c73 5a03 726e 6e5a  .nn..utilsZ.rnnZ
+00002680: 0c70 6164 5f73 6571 7565 6e63 6572 7100  .pad_sequencerq.
+00002690: 0000 725d 0000 005a 0c70 6164 5f74 6f6b  ..r]...Z.pad_tok
+000026a0: 656e 5f69 6472 7300 0000 5a07 6e6f 5f67  en_idrs...Z.no_g
+000026b0: 7261 6472 6a00 0000 7215 0000 0029 0772  radrj...r....).r
+000026c0: 2600 0000 722d 0000 0072 3500 0000 7234  &...r-...r5...r4
+000026d0: 0000 0072 8000 0000 7212 0000 0072 1100  ...r....r....r..
+000026e0: 0000 7213 0000 0072 8c00 0000 7214 0000  ..r....r....r...
+000026f0: 0072 3600 0000 1801 0000 732c 0000 0000  .r6.......s,....
+00002700: 010a 010e 0502 fb04 0702 010a f706 0b0a  ................
+00002710: 010e 0702 f904 0902 0102 f506 0d06 0108  ................
+00002720: 0108 010a 0104 0104 ff24 037a 1654 7261  .........$.z.Tra
+00002730: 6e73 666f 726d 6572 4d6f 6465 6c2e 656d  nsformerModel.em
+00002740: 6265 6429 064e 4e4e 4e46 4e29 0146 290f  bed).NNNNFN).F).
+00002750: 724b 0000 0072 4c00 0000 724d 0000 0072  rK...rL...rM...r
+00002760: 5f00 0000 7232 0000 0072 4a00 0000 724e  _...r2...rJ...rN
+00002770: 0000 0072 2700 0000 724f 0000 0072 2b00  ...r'...rO...r+.
+00002780: 0000 722e 0000 0072 3100 0000 7287 0000  ..r....r1...r...
+00002790: 0072 8900 0000 7236 0000 0072 1300 0000  .r....r6...r....
+000027a0: 7213 0000 0072 1300 0000 7214 0000 0072  r....r....r....r
+000027b0: 7200 0000 9800 0000 7320 0000 0008 0400  r.......s ......
+000027c0: 0100 0100 0100 0100 0100 f80a 3208 0b08  ............2...
+000027d0: 030e 030e 050e 0310 1408 1008 1072 7200  .............rr.
+000027e0: 0000 6749 afbc 9af2 d79a 3e69 50c3 0000  ..gI......>iP...
+000027f0: 69d0 0700 0063 0000 0000 0000 0000 0000  i....c..........
+00002800: 0000 0000 0000 0500 0000 4300 0000 730e  ..........C...s.
+00002810: 0000 0074 0064 0164 0264 0364 048d 0353  ...t.d.d.d.d...S
+00002820: 0029 054e 7252 0000 0072 5300 0000 7254  .).NrR...rS...rT
+00002830: 0000 0029 0372 5a00 0000 725b 0000 0072  ...).rZ...r[...r
+00002840: 5e00 0000 2901 7251 0000 0072 1300 0000  ^...).rQ...r....
+00002850: 7213 0000 0072 1300 0000 7214 0000 00da  r....r....r.....
+00002860: 083c 6c61 6d62 6461 3e40 0100 0073 0800  .<lambda>@...s..
+00002870: 0000 0201 0201 0201 02fd 728f 0000 0029  ..........r....)
+00002880: 04da 0e63 6f73 745f 7065 725f 746f 6b65  ...cost_per_toke
+00002890: 6eda 0970 6f6f 6c5f 7369 7a65 da0a 706f  n..pool_size..po
+000028a0: 6f6c 5f63 6f75 6e74 da09 6765 745f 6d6f  ol_count..get_mo
+000028b0: 6465 6c63 0000 0000 0000 0000 0000 0000  delc............
+000028c0: 0000 0000 0300 0000 4300 0000 730a 0000  ........C...s...
+000028d0: 0074 0074 0164 018d 0153 00a9 024e 2901  .t.t.d...S...N).
+000028e0: 725a 0000 0029 0272 7200 0000 da11 6d69  rZ...).rr.....mi
+000028f0: 6e69 6c6d 5f6d 6f64 656c 5f6e 616d 6572  nilm_model_namer
+00002900: 1300 0000 7213 0000 0072 1300 0000 7214  ....r....r....r.
+00002910: 0000 0072 8f00 0000 4901 0000 721a 0000  ...r....I...r...
+00002920: 0029 0372 9000 0000 7291 0000 0072 9300  .).r....r....r..
+00002930: 0000 6998 3a00 0063 0000 0000 0000 0000  ..i.:..c........
+00002940: 0000 0000 0000 0000 0300 0000 4300 0000  ............C...
+00002950: 730a 0000 0074 0074 0164 018d 0153 0072  s....t.t.d...S.r
+00002960: 9400 0000 2902 7272 0000 00da 106d 706e  ....).rr.....mpn
+00002970: 6574 5f6d 6f64 656c 5f6e 616d 6572 1300  et_model_namer..
+00002980: 0000 7213 0000 0072 1300 0000 7214 0000  ..r....r....r...
+00002990: 0072 8f00 0000 4e01 0000 721a 0000 0069  .r....N...r....i
+000029a0: 1027 0000 6300 0000 0000 0000 0000 0000  .'..c...........
+000029b0: 0000 0000 0008 0000 0043 0000 0073 1400  .........C...s..
+000029c0: 0000 7400 7401 6401 6402 6403 6404 6405  ..t.t.d.d.d.d.d.
+000029d0: 6406 8d06 5300 a907 4efa 015b fa01 5dda  d...S...N..[..].
+000029e0: 017b da01 7d54 2906 725a 0000 0072 7700  .{..}T).rZ...rw.
+000029f0: 0000 7278 0000 0072 7500 0000 7276 0000  ..rx...ru...rv..
+00002a00: 0072 7900 0000 2902 7272 0000 00da 0f73  .ry...).rr.....s
+00002a10: 6770 745f 6d6f 6465 6c5f 6e61 6d65 7213  gpt_model_namer.
+00002a20: 0000 0072 1300 0000 7213 0000 0072 1400  ...r....r....r..
+00002a30: 0000 728f 0000 0053 0100 0073 0e00 0000  ..r....S...s....
+00002a40: 0201 0201 0201 0201 0201 0201 02fa 69e8  ..............i.
+00002a50: 0300 0063 0000 0000 0000 0000 0000 0000  ...c............
+00002a60: 0000 0000 0800 0000 4300 0000 7314 0000  ........C...s...
+00002a70: 0074 0074 0164 0164 0264 0364 0464 0564  .t.t.d.d.d.d.d.d
+00002a80: 068d 0653 0072 9700 0000 2902 7272 0000  ...S.r....).rr..
+00002a90: 00da 1473 6770 745f 315f 3342 5f6d 6f64  ...sgpt_1_3B_mod
+00002aa0: 656c 5f6e 616d 6572 1300 0000 7213 0000  el_namer....r...
+00002ab0: 0072 1300 0000 7214 0000 0072 8f00 0000  .r....r....r....
+00002ac0: 5f01 0000 730e 0000 0002 0102 0102 0102  _...s...........
+00002ad0: 0102 0102 0102 fa29 0572 5900 0000 5a06  .......).rY...Z.
+00002ae0: 6d69 6e69 6c6d da05 6d70 6e65 745a 0473  minilm..mpnetZ.s
+00002af0: 6770 747a 0973 6770 742d 312e 3342 291d  gptz.sgpt-1.3B).
+00002b00: 7255 0000 00da 0361 6263 7202 0000 0072  rU.....abcr....r
+00002b10: 0300 0000 7220 0000 0072 3e00 0000 7259  ....r ...r>...rY
+00002b20: 0000 0072 5c00 0000 720e 0000 00da 0664  ...r\...r......d
+00002b30: 6f74 656e 7672 0400 0000 727a 0000 0072  otenvr....rz...r
+00002b40: 0500 0000 7206 0000 00da 0470 6174 68da  ....r......path.
+00002b50: 046a 6f69 6eda 0667 6574 6377 6472 9500  .join..getcwdr..
+00002b60: 0000 7296 0000 0072 9c00 0000 729d 0000  ..r....r....r...
+00002b70: 0072 1500 0000 721d 0000 0072 2100 0000  .r....r....r!...
+00002b80: 7222 0000 0072 5100 0000 7271 0000 0072  r"...rQ...rq...r
+00002b90: 7200 0000 da06 6d6f 6465 6c73 7213 0000  r.....modelsr...
+00002ba0: 0072 1300 0000 7213 0000 0072 1400 0000  .r....r....r....
+00002bb0: da08 3c6d 6f64 756c 653e 0100 0000 7354  ..<module>....sT
+00002bc0: 0000 0008 0110 0208 0108 0108 0108 010c  ................
+00002bd0: 0110 0218 0204 0104 0104 0104 0308 0c08  ................
+00002be0: 0408 0710 3e10 2c08 0410 7f00 2602 0102  ....>.,.....&...
+00002bf0: 0102 0106 fc04 0b02 0102 0106 fd04 0602  ................
+00002c00: 0102 0106 fd04 0602 0102 0106 fd04 0d02  ................
+00002c10: 0102 0106 fd04 df                        .......
```

### Comparing `semantra-0.1.6/src/semantra/__pycache__/pdf.cpython-39.pyc` & `semantra-0.1.7/src/semantra/__pycache__/pdf.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Sun Apr 23 04:31:52 2023 UTC, .py size: 3118 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 b8b4 4464 2e0c 0000  a.........Dd....
+00000000: 610d 0d0a 0000 0000 516b a964 fd0c 0000  a.......Qk.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 6a00 0000 6400  .....@...sj...d.
 00000030: 6401 6c00 5a01 6400 6402 6c02 6d03 5a03  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6400 6401 6c04 5a04 6400 6401 6c05  ..d.d.l.Z.d.d.l.
 00000050: 5a05 6400 6403 6c06 6d06 5a06 0100 6404  Z.d.d.l.m.Z...d.
 00000060: 6405 6c07 6d08 5a08 6d09 5a09 0100 6900  d.l.m.Z.m.Z...i.
 00000070: 5a0a 6406 6407 8400 5a0b 4700 6408 6409  Z.d.d...Z.G.d.d.
@@ -113,81 +113,86 @@
 00000700: 655f 5fda 0a5f 5f6d 6f64 756c 655f 5fda  e__..__module__.
 00000710: 0c5f 5f71 7561 6c6e 616d 655f 5f72 1500  .__qualname__r..
 00000720: 0000 721a 0000 0072 2c00 0000 7209 0000  ..r....r,...r...
 00000730: 0072 0900 0000 7209 0000 0072 0a00 0000  .r....r....r....
 00000740: 720c 0000 0012 0000 0073 0600 0000 0801  r........s......
 00000750: 0808 0806 720c 0000 00fa 010c 6305 0000  ....r.......c...
 00000760: 0000 0000 0000 0000 0013 0000 0008 0000  ................
-00000770: 0043 0000 0073 f001 0000 7400 6a01 a002  .C...s....t.j...
+00000770: 0043 0000 0073 0402 0000 7400 6a01 a002  .C...s....t.j...
 00000780: 7c02 7403 7c00 8301 a102 7d05 7400 6a01  |.t.|.....}.t.j.
 00000790: a002 7c02 7404 7c00 8301 a102 7d06 7405  ..|.t.|.....}.t.
 000007a0: a006 7c01 a101 7d07 7407 7c07 8301 7d08  ..|...}.t.|...}.
 000007b0: 7c03 7354 7400 6a01 a008 7c05 a101 7254  |.sTt.j...|...rT
-000007c0: 7400 6a01 a008 7c06 a101 9001 7372 6700  t.j...|.....srg.
+000007c0: 7400 6a01 a008 7c06 a101 9001 737e 6700  t.j...|.....s~g.
 000007d0: 7d09 6401 7d0a 7409 7c05 6402 6403 6404  }.d.}.t.|.d.d.d.
-000007e0: 8d03 8f7c 7d0b 740a 740b 7c08 8301 6405  ...|}.t.t.|...d.
-000007f0: 6406 7c04 6407 8d04 4400 5d56 7d0c 7c07  d.|.d...D.]V}.|.
-00000800: 7c0c 1900 7d0d 7c0d a00c a100 5c02 7d0e  |...}.|.....\.}.
-00000810: 7d0f 7c0d a00d a100 7d10 7c10 a00e a100  }.|.....}.|.....
-00000820: 7d11 7c09 a00f 7c0a 7c0e 7c0f 6408 9c03  }.|...|.|.|.d...
-00000830: a101 0100 7c0a 7c0b a010 7c11 a101 3700  ....|.|...|...7.
-00000840: 7d0a 7c0a 7c0b a010 7411 a101 3700 7d0a  }.|.|...t...7.}.
-00000850: 7180 5700 6400 0400 0400 8303 0100 6e10  q.W.d.........n.
-00000860: 3100 73ec 3000 0100 0100 0100 5900 0100  1.s.0.......Y...
-00000870: 7409 7c06 6402 8302 8f1c 7d0b 7412 a013  t.|.d.....}.t...
-00000880: 7c09 7c0b a102 0100 5700 6400 0400 0400  |.|.....W.d.....
-00000890: 8303 0100 6e12 3100 9001 7324 3000 0100  ....n.1...s$0...
-000008a0: 0100 0100 5900 0100 7409 7c05 6409 6403  ....Y...t.|.d.d.
-000008b0: 6404 8d03 8f18 7d0b 7c0b a014 a100 7d12  d.....}.|.....}.
-000008c0: 5700 6400 0400 0400 8303 0100 6e12 3100  W.d.........n.1.
-000008d0: 9001 735c 3000 0100 0100 0100 5900 0100  ..s\0.......Y...
-000008e0: 7415 7c12 7c01 7c09 8303 5300 7409 7c05  t.|.|.|...S.t.|.
-000008f0: 6409 6403 6404 8d03 8f18 7d0b 7c0b a014  d.d.d.....}.|...
-00000900: a100 7d12 5700 6400 0400 0400 8303 0100  ..}.W.d.........
-00000910: 6e12 3100 9001 73a0 3000 0100 0100 0100  n.1...s.0.......
-00000920: 5900 0100 7409 7c06 6409 8302 8f1a 7d0b  Y...t.|.d.....}.
-00000930: 7412 a016 7c0b a101 7d09 5700 6400 0400  t...|...}.W.d...
-00000940: 0400 8303 0100 6e12 3100 9001 73d6 3000  ......n.1...s.0.
-00000950: 0100 0100 0100 5900 0100 7415 7c12 7c01  ......Y...t.|.|.
-00000960: 7c09 8303 5300 6400 5300 290a 4e72 0100  |...S.d.S.).Nr..
-00000970: 0000 da01 77da 0029 01da 076e 6577 6c69  ....w..)...newli
-00000980: 6e65 7a17 4578 7472 6163 7469 6e67 2050  nez.Extracting P
-00000990: 4446 2063 6f6e 7465 6e74 7346 2903 da04  DF contentsF)...
-000009a0: 6465 7363 da05 6c65 6176 65da 0764 6973  desc..leave..dis
-000009b0: 6162 6c65 2903 da0a 6368 6172 5f69 6e64  able)...char_ind
-000009c0: 6578 da0a 7061 6765 5f77 6964 7468 da0b  ex..page_width..
-000009d0: 7061 6765 5f68 6569 6768 74da 0172 2917  page_height..r).
-000009e0: da02 6f73 da04 7061 7468 da04 6a6f 696e  ..os..path..join
-000009f0: 7205 0000 0072 0600 0000 7210 0000 0072  r....r....r....r
-00000a00: 1100 0000 da03 6c65 6eda 0665 7869 7374  ......len..exist
-00000a10: 73da 046f 7065 6e72 0300 0000 7228 0000  s..openr....r(..
-00000a20: 005a 0867 6574 5f73 697a 6572 2700 0000  .Z.get_sizer'...
-00000a30: 7224 0000 00da 0661 7070 656e 64da 0577  r$.....append..w
-00000a40: 7269 7465 da09 4c49 4e45 5f46 4545 44da  rite..LINE_FEED.
-00000a50: 046a 736f 6eda 0464 756d 70da 0472 6561  .json..dump..rea
-00000a60: 6472 0c00 0000 da04 6c6f 6164 2913 da03  dr......load)...
-00000a70: 6d64 3572 0800 0000 da0c 7365 6d61 6e74  md5r......semant
-00000a80: 7261 5f64 6972 da05 666f 7263 65da 0673  ra_dir..force..s
-00000a90: 696c 656e 745a 0d63 6f6e 7665 7274 6564  ilentZ.converted
-00000aa0: 5f74 7874 5a0e 706f 7369 7469 6f6e 5f69  _txtZ.position_i
-00000ab0: 6e64 6578 720d 0000 005a 076e 5f70 6167  ndexr....Z.n_pag
-00000ac0: 6573 720f 0000 00da 0870 6f73 6974 696f  esr......positio
-00000ad0: 6eda 0166 da0a 7061 6765 5f69 6e64 6578  n..f..page_index
-00000ae0: 7219 0000 0072 3800 0000 7239 0000 0072  r....r8...r9...r
-00000af0: 1f00 0000 5a08 7061 6765 7465 7874 720e  ....Z.pagetextr.
-00000b00: 0000 0072 0900 0000 7209 0000 0072 0a00  ...r....r....r..
-00000b10: 0000 da0f 6765 745f 7064 665f 636f 6e74  ....get_pdf_cont
-00000b20: 656e 7431 0000 0073 4800 0000 0001 1201  ent1...sH.......
-00000b30: 1202 0a01 0802 1e01 0401 0402 1001 0201  ................
-00000b40: 0601 0201 0201 02fc 0a06 0801 0c01 0801  ................
-00000b50: 0802 0402 0201 0201 02fd 04ff 0407 0e01  ................
-00000b60: 2e01 0c01 2c01 1001 2801 0c02 1001 2801  ....,...(.....(.
-00000b70: 0c01 2a02 724f 0000 0029 0f5a 0970 7970  ..*.rO...).Z.pyp
-00000b80: 6466 6975 6d32 7210 0000 00da 0974 6872  dfium2r......thr
-00000b90: 6561 6469 6e67 7202 0000 0072 4400 0000  eadingr....rD...
-00000ba0: 723b 0000 0072 0300 0000 da04 7574 696c  r;...r......util
-00000bb0: 7205 0000 0072 0600 0000 7207 0000 0072  r....r....r....r
-00000bc0: 0b00 0000 720c 0000 0072 4300 0000 724f  ....r....rC...rO
-00000bd0: 0000 0072 0900 0000 7209 0000 0072 0900  ...r....r....r..
-00000be0: 0000 720a 0000 00da 083c 6d6f 6475 6c65  ..r......<module
-00000bf0: 3e01 0000 0073 1400 0000 0801 0c01 0801  >....s..........
-00000c00: 0801 0c01 1002 0403 0807 0e1c 0403       ..............
+000007e0: 6405 6406 8d05 8f7c 7d0b 740a 740b 7c08  d.d....|}.t.t.|.
+000007f0: 8301 6407 6408 7c04 6409 8d04 4400 5d56  ..d.d.|.d...D.]V
+00000800: 7d0c 7c07 7c0c 1900 7d0d 7c0d a00c a100  }.|.|...}.|.....
+00000810: 5c02 7d0e 7d0f 7c0d a00d a100 7d10 7c10  \.}.}.|.....}.|.
+00000820: a00e a100 7d11 7c09 a00f 7c0a 7c0e 7c0f  ....}.|...|.|.|.
+00000830: 640a 9c03 a101 0100 7c0a 7c0b a010 7c11  d.......|.|...|.
+00000840: a101 3700 7d0a 7c0a 7c0b a010 7411 a101  ..7.}.|.|...t...
+00000850: 3700 7d0a 7184 5700 6400 0400 0400 8303  7.}.q.W.d.......
+00000860: 0100 6e10 3100 73f0 3000 0100 0100 0100  ..n.1.s.0.......
+00000870: 5900 0100 7409 7c06 6402 6404 640b 8d03  Y...t.|.d.d.d...
+00000880: 8f1c 7d0b 7412 a013 7c09 7c0b a102 0100  ..}.t...|.|.....
+00000890: 5700 6400 0400 0400 8303 0100 6e12 3100  W.d.........n.1.
+000008a0: 9001 732c 3000 0100 0100 0100 5900 0100  ..s,0.......Y...
+000008b0: 7409 7c05 640c 6403 6404 6405 6406 8d05  t.|.d.d.d.d.d...
+000008c0: 8f18 7d0b 7c0b a014 a100 7d12 5700 6400  ..}.|.....}.W.d.
+000008d0: 0400 0400 8303 0100 6e12 3100 9001 7368  ........n.1...sh
+000008e0: 3000 0100 0100 0100 5900 0100 7415 7c12  0.......Y...t.|.
+000008f0: 7c01 7c09 8303 5300 7409 7c05 640c 6403  |.|...S.t.|.d.d.
+00000900: 6404 6405 6406 8d05 8f18 7d0b 7c0b a014  d.d.d.....}.|...
+00000910: a100 7d12 5700 6400 0400 0400 8303 0100  ..}.W.d.........
+00000920: 6e12 3100 9001 73b0 3000 0100 0100 0100  n.1...s.0.......
+00000930: 5900 0100 7409 7c06 640c 6404 640b 8d03  Y...t.|.d.d.d...
+00000940: 8f1a 7d0b 7412 a016 7c0b a101 7d09 5700  ..}.t...|...}.W.
+00000950: 6400 0400 0400 8303 0100 6e12 3100 9001  d.........n.1...
+00000960: 73ea 3000 0100 0100 0100 5900 0100 7415  s.0.......Y...t.
+00000970: 7c12 7c01 7c09 8303 5300 6400 5300 290d  |.|.|...S.d.S.).
+00000980: 4e72 0100 0000 da01 77da 007a 0575 7466  Nr......w..z.utf
+00000990: 2d38 da06 6967 6e6f 7265 2903 da07 6e65  -8..ignore)...ne
+000009a0: 776c 696e 65da 0865 6e63 6f64 696e 67da  wline..encoding.
+000009b0: 0665 7272 6f72 737a 1745 7874 7261 6374  .errorsz.Extract
+000009c0: 696e 6720 5044 4620 636f 6e74 656e 7473  ing PDF contents
+000009d0: 4629 03da 0464 6573 63da 056c 6561 7665  F)...desc..leave
+000009e0: da07 6469 7361 626c 6529 03da 0a63 6861  ..disable)...cha
+000009f0: 725f 696e 6465 78da 0a70 6167 655f 7769  r_index..page_wi
+00000a00: 6474 68da 0b70 6167 655f 6865 6967 6874  dth..page_height
+00000a10: 2901 7235 0000 00da 0172 2917 da02 6f73  ).r5.....r)...os
+00000a20: da04 7061 7468 da04 6a6f 696e 7205 0000  ..path..joinr...
+00000a30: 0072 0600 0000 7210 0000 0072 1100 0000  .r....r....r....
+00000a40: da03 6c65 6eda 0665 7869 7374 73da 046f  ..len..exists..o
+00000a50: 7065 6e72 0300 0000 7228 0000 005a 0867  penr....r(...Z.g
+00000a60: 6574 5f73 697a 6572 2700 0000 7224 0000  et_sizer'...r$..
+00000a70: 00da 0661 7070 656e 64da 0577 7269 7465  ...append..write
+00000a80: da09 4c49 4e45 5f46 4545 44da 046a 736f  ..LINE_FEED..jso
+00000a90: 6eda 0464 756d 70da 0472 6561 6472 0c00  n..dump..readr..
+00000aa0: 0000 da04 6c6f 6164 2913 da03 6d64 3572  ....load)...md5r
+00000ab0: 0800 0000 da0c 7365 6d61 6e74 7261 5f64  ......semantra_d
+00000ac0: 6972 da05 666f 7263 65da 0673 696c 656e  ir..force..silen
+00000ad0: 745a 0d63 6f6e 7665 7274 6564 5f74 7874  tZ.converted_txt
+00000ae0: 5a0e 706f 7369 7469 6f6e 5f69 6e64 6578  Z.position_index
+00000af0: 720d 0000 005a 076e 5f70 6167 6573 720f  r....Z.n_pagesr.
+00000b00: 0000 00da 0870 6f73 6974 696f 6eda 0166  .....position..f
+00000b10: da0a 7061 6765 5f69 6e64 6578 7219 0000  ..page_indexr...
+00000b20: 0072 3b00 0000 723c 0000 0072 1f00 0000  .r;...r<...r....
+00000b30: 5a08 7061 6765 7465 7874 720e 0000 0072  Z.pagetextr....r
+00000b40: 0900 0000 7209 0000 0072 0a00 0000 da0f  ....r....r......
+00000b50: 6765 745f 7064 665f 636f 6e74 656e 7431  get_pdf_content1
+00000b60: 0000 0073 5a00 0000 0001 1201 1202 0a01  ...sZ...........
+00000b70: 0802 1e01 0401 0402 0201 0aff 0602 0201  ................
+00000b80: 0201 0601 0201 0201 02fc 0a06 0801 0c01  ................
+00000b90: 0801 0802 0402 0201 0201 02fd 04ff 0407  ................
+00000ba0: 0e01 2e01 1001 2c01 0201 0aff 0602 0201  ......,.........
+00000bb0: 2801 0c02 0201 0aff 0602 0201 2801 1001  (...........(...
+00000bc0: 2a02 7252 0000 0029 0f5a 0970 7970 6466  *.rR...).Z.pypdf
+00000bd0: 6975 6d32 7210 0000 00da 0974 6872 6561  ium2r......threa
+00000be0: 6469 6e67 7202 0000 0072 4700 0000 723e  dingr....rG...r>
+00000bf0: 0000 0072 0300 0000 da04 7574 696c 7205  ...r......utilr.
+00000c00: 0000 0072 0600 0000 7207 0000 0072 0b00  ...r....r....r..
+00000c10: 0000 720c 0000 0072 4600 0000 7252 0000  ..r....rF...rR..
+00000c20: 0072 0900 0000 7209 0000 0072 0900 0000  .r....r....r....
+00000c30: 720a 0000 00da 083c 6d6f 6475 6c65 3e01  r......<module>.
+00000c40: 0000 0073 1400 0000 0801 0c01 0801 0801  ...s............
+00000c50: 0c01 1002 0403 0807 0e1c 0403            ............
```

### Comparing `semantra-0.1.6/src/semantra/__pycache__/semantra.cpython-39.pyc` & `semantra-0.1.7/src/semantra/__pycache__/semantra.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Sun Apr 23 12:15:14 2023 UTC, .py size: 28787 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 26% similar despite different names*

```diff
@@ -1,1223 +1,1256 @@
-00000000: 610d 0d0a 0000 0000 5221 4564 7370 0000  a.......R!Edsp..
+00000000: 610d 0d0a 0000 0000 ad76 a964 5874 0000  a........v.dXt..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0038 0000 0040 0000 0073 ba03 0000 6400  .8...@...s....d.
+00000020: 003a 0000 0040 0000 0073 ea03 0000 6400  .:...@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
-00000040: 6402 6c02 6d02 5a02 0100 6400 6401 6c03  d.l.m.Z...d.d.l.
-00000050: 5a04 6400 6403 6c05 6d06 5a06 6d07 5a07  Z.d.d.l.m.Z.m.Z.
-00000060: 6d08 5a08 6d09 5a09 6d0a 5a0a 6d0b 5a0b  m.Z.m.Z.m.Z.m.Z.
-00000070: 0100 6400 6401 6c0c 5a0c 6404 6405 6c0d  ..d.d.l.Z.d.d.l.
-00000080: 6d0d 5a0d 6d0e 5a0e 6d0f 5a0f 6d10 5a10  m.Z.m.Z.m.Z.m.Z.
-00000090: 0100 6400 6401 6c11 5a11 6404 6406 6c12  ..d.d.l.Z.d.d.l.
-000000a0: 6d13 5a13 0100 6400 6401 6c14 5a14 6400  m.Z...d.d.l.Z.d.
-000000b0: 6401 6c15 5a15 6404 6407 6c16 6d17 5a17  d.l.Z.d.d.l.m.Z.
-000000c0: 6d18 5a18 6d19 5a19 6d1a 5a1a 6d1b 5a1b  m.Z.m.Z.m.Z.m.Z.
-000000d0: 6d1c 5a1c 6d1d 5a1d 6d1e 5a1e 6d1f 5a1f  m.Z.m.Z.m.Z.m.Z.
-000000e0: 6d20 5a20 6d21 5a21 6d22 5a22 6d23 5a23  m Z m!Z!m"Z"m#Z#
-000000f0: 6d24 5a24 6d25 5a25 0100 6400 6401 6c26  m$Z$m%Z%..d.d.l&
-00000100: 5a26 6527 6526 a028 6408 6409 a102 640a  Z&e'e&.(d.d...d.
-00000110: 8302 8f1c 5a29 6529 a02a a100 a02b a100  ....Z)e).*...+..
-00000120: 5a2c 5700 6401 0400 0400 8303 0100 6e12  Z,W.d.........n.
-00000130: 3100 9001 730a 3000 0100 0100 0100 5900  1...s.0.......Y.
-00000140: 0100 6501 6a2d a02e 6501 6a2d a02f 6530  ..e.j-..e.j-./e0
-00000150: a101 a101 5a31 4700 640b 640c 8400 640c  ....Z1G.d.d...d.
-00000160: 8302 5a32 640d 640e 8400 5a33 640f 5a34  ..Z2d.d...Z3d.Z4
-00000170: 4700 6410 6411 8400 6411 8302 5a35 6412  G.d.d...d...Z5d.
-00000180: 6413 8400 5a36 6537 6414 6415 9c02 6416  d...Z6e7d.d...d.
-00000190: 6417 8404 5a38 650c a039 a100 650c 6a3a  d...Z8e..9..e.j:
-000001a0: 6418 650c 6a3b 6419 641a 8d01 641b 641c  d.e.j;d.d...d.d.
-000001b0: 8d03 650c 6a3c 641d 650c 6a3d 650d a03e  ..e.j<d.e.j=e..>
-000001c0: a100 6419 641e 8d02 641f 6419 6420 6421  ..d.d...d.d.d d!
-000001d0: 8d05 650c 6a3c 6422 6537 6423 6424 8d03  ..e.j<d"e7d#d$..
-000001e0: 650c 6a3c 6425 6537 6426 6419 6427 6421  e.j<d%e7d&d.d'd!
-000001f0: 8d05 650c 6a3c 6428 6419 6429 6419 642a  ..e.j<d(d.d)d.d*
-00000200: 642b 8d05 650c 6a3c 642c 653f 642d 6419  d+..e.j<d,e?d-d.
-00000210: 642e 6421 8d05 650c 6a3c 642f 6537 6430  d.d!..e.j<d/e7d0
-00000220: 6419 6431 6421 8d05 650c 6a3c 6432 653f  d.d1d!..e.j<d2e?
-00000230: 6401 6433 6434 8d04 650c 6a3c 6435 653f  d.d3d4..e.j<d5e?
-00000240: 6401 6436 6434 8d04 650c 6a3c 6437 6537  d.d6d4..e.j<d7e7
-00000250: 6401 6438 6434 8d04 650c 6a3c 6439 6537  d.d8d4..e.j<d9e7
-00000260: 6401 643a 6434 8d04 650c 6a3c 643b 6537  d.d:d4..e.j<d;e7
-00000270: 6401 643c 6434 8d04 650c 6a3c 643d 6537  d.d<d4..e.j<d=e7
-00000280: 6401 643e 6434 8d04 650c 6a3c 643f 653f  d.d>d4..e.j<d?e?
-00000290: 6440 6419 6441 6421 8d05 650c 6a3c 6442  d@d.dAd!..e.j<dB
-000002a0: 6419 6419 6419 6443 642b 8d05 650c 6a3c  d.d.d.dCd+..e.j<
-000002b0: 6444 653f 6445 6419 6446 6421 8d05 650c  dDe?dEd.dFd!..e.
-000002c0: 6a3c 6447 6419 6429 6419 6448 642b 8d05  j<dGd.d)d.dHd+..
-000002d0: 650c 6a3c 6449 6540 644a 6419 644b 6421  e.j<dIe@dJd.dKd!
-000002e0: 8d05 650c 6a3c 644c 653f 644d 6419 644e  ..e.j<dLe?dMd.dN
-000002f0: 6421 8d05 650c 6a3c 644f 653f 6450 6419  d!..e.j<dOe?dPd.
-00000300: 6451 6421 8d05 650c 6a3c 6452 653f 6453  dQd!..e.j<dRe?dS
-00000310: 6419 6454 6421 8d05 650c 6a3c 6455 6419  d.dTd!..e.j<dUd.
-00000320: 6429 6456 6457 8d04 650c 6a3c 6458 6419  d)dVdW..e.j<dXd.
-00000330: 6429 6459 6457 8d04 650c 6a3c 645a 6419  d)dYdW..e.j<dZd.
-00000340: 6429 645b 6457 8d04 650c 6a3c 645c 6419  d)d[dW..e.j<d\d.
-00000350: 6429 645d 6457 8d04 650c 6a3c 645e 6419  d)d]dW..e.j<d^d.
-00000360: 6429 645f 6457 8d04 650c 6a3c 6460 6419  d)d_dW..e.j<d`d.
-00000370: 6429 6461 6457 8d04 650c 6a3c 6462 650c  d)dadW..e.j<dbe.
-00000380: 6a3b 6429 641a 8d01 6401 6463 6434 8d04  j;d)d...d.dcd4..
-00000390: 6467 6464 6465 8401 8301 8301 8301 8301  dgddde..........
-000003a0: 8301 8301 8301 8301 8301 8301 8301 8301  ................
-000003b0: 8301 8301 8301 8301 8301 8301 8301 8301  ................
-000003c0: 8301 8301 8301 8301 8301 8301 8301 8301  ................
-000003d0: 8301 5a41 6542 6466 6b02 9003 72b6 6541  ..ZAeBdfk...r.eA
-000003e0: 8300 0100 6401 5300 2968 e900 0000 004e  ....d.S.)h.....N
-000003f0: 2901 da04 7471 646d 2906 da05 466c 6173  )...tqdm)...Flas
-00000400: 6bda 0772 6571 7565 7374 da07 6a73 6f6e  k..request..json
-00000410: 6966 79da 1373 656e 645f 6672 6f6d 5f64  ify..send_from_d
-00000420: 6972 6563 746f 7279 da09 7365 6e64 5f66  irectory..send_f
-00000430: 696c 65da 0d6d 616b 655f 7265 7370 6f6e  ile..make_respon
-00000440: 7365 e901 0000 0029 04da 066d 6f64 656c  se.....)...model
-00000450: 73da 0942 6173 654d 6f64 656c da10 5472  s..BaseModel..Tr
-00000460: 616e 7366 6f72 6d65 724d 6f64 656c da08  ansformerModel..
-00000470: 6173 5f6e 756d 7079 2901 da0f 6765 745f  as_numpy)...get_
-00000480: 7064 665f 636f 6e74 656e 7429 0fda 0866  pdf_content)...f
-00000490: 696c 655f 6d64 35da 1367 6574 5f74 6f6b  ile_md5..get_tok
-000004a0: 656e 735f 6669 6c65 6e61 6d65 da13 6765  ens_filename..ge
-000004b0: 745f 636f 6e66 6967 5f66 696c 656e 616d  t_config_filenam
-000004c0: 65da 1767 6574 5f65 6d62 6564 6469 6e67  e..get_embedding
-000004d0: 735f 6669 6c65 6e61 6d65 da12 6765 745f  s_filename..get_
-000004e0: 6e75 6d5f 656d 6265 6464 696e 6773 da0b  num_embeddings..
-000004f0: 6765 745f 6f66 6673 6574 73da 1472 6561  get_offsets..rea
-00000500: 645f 656d 6265 6464 696e 6773 5f66 696c  d_embeddings_fil
-00000510: 65da 0f77 7269 7465 5f65 6d62 6564 6469  e..write_embeddi
-00000520: 6e67 da10 6a6f 696e 5f74 6578 745f 6368  ng..join_text_ch
-00000530: 756e 6b73 da12 6765 745f 616e 6e6f 795f  unks..get_annoy_
-00000540: 6669 6c65 6e61 6d65 da18 6765 745f 6e75  filename..get_nu
-00000550: 6d5f 616e 6e6f 795f 656d 6265 6464 696e  m_annoy_embeddin
-00000560: 6773 da0e 7772 6974 655f 616e 6e6f 795f  gs..write_annoy_
-00000570: 6462 da0d 6c6f 6164 5f61 6e6e 6f79 5f64  db..load_annoy_d
-00000580: 62da 0c73 6f72 745f 7265 7375 6c74 73da  b..sort_results.
-00000590: 0b48 4153 485f 4c45 4e47 5448 fa11 7365  .HASH_LENGTH..se
-000005a0: 6d61 6e74 7261 2e73 656d 616e 7472 617a  mantra.semantraz
-000005b0: 0d2e 2e2f 2e2e 2f56 4552 5349 4f4e da01  .../../VERSION..
-000005c0: 7263 0000 0000 0000 0000 0000 0000 0000  rc..............
-000005d0: 0000 0200 0000 4000 0000 7314 0000 0065  ......@...s....e
-000005e0: 005a 0164 005a 0264 0164 0284 005a 0364  .Z.d.Z.d.d...Z.d
-000005f0: 0353 0029 04da 0743 6f6e 7465 6e74 6303  .S.)...Contentc.
-00000600: 0000 0000 0000 0000 0000 0003 0000 0002  ................
-00000610: 0000 0043 0000 0073 1600 0000 7c01 7c00  ...C...s....|.|.
-00000620: 5f00 7c02 7c00 5f01 6401 7c00 5f02 6400  _.|.|._.d.|._.d.
-00000630: 5300 2902 4eda 0474 6578 7429 03da 0772  S.).N..text)...r
-00000640: 6177 7465 7874 da08 6669 6c65 6e61 6d65  awtext..filename
-00000650: da08 6669 6c65 7479 7065 2903 da04 7365  ..filetype)...se
-00000660: 6c66 7222 0000 0072 2300 0000 a900 7226  lfr"...r#.....r&
-00000670: 0000 00fa 392f 5573 6572 732f 6672 6565  ....9/Users/free
-00000680: 646d 616e 642f 7363 7261 7073 2f73 656d  dmand/scraps/sem
-00000690: 616e 7472 612f 7372 632f 7365 6d61 6e74  antra/src/semant
-000006a0: 7261 2f73 656d 616e 7472 612e 7079 da08  ra/semantra.py..
-000006b0: 5f5f 696e 6974 5f5f 2800 0000 7306 0000  __init__(...s...
-000006c0: 0000 0106 0106 017a 1043 6f6e 7465 6e74  .......z.Content
-000006d0: 2e5f 5f69 6e69 745f 5f4e 2904 da08 5f5f  .__init__N)...__
-000006e0: 6e61 6d65 5f5f da0a 5f5f 6d6f 6475 6c65  name__..__module
-000006f0: 5f5f da0c 5f5f 7175 616c 6e61 6d65 5f5f  __..__qualname__
-00000700: 7228 0000 0072 2600 0000 7226 0000 0072  r(...r&...r&...r
-00000710: 2600 0000 7227 0000 0072 2000 0000 2700  &...r'...r ...'.
-00000720: 0000 7302 0000 0008 0172 2000 0000 6305  ..s......r ...c.
-00000730: 0000 0000 0000 0000 0000 0007 0000 0008  ................
-00000740: 0000 0043 0000 0073 6000 0000 7c01 a000  ...C...s`...|...
-00000750: 6401 a101 721a 7401 7c00 7c01 7c02 7c03  d...r.t.|.|.|.|.
-00000760: 7c04 8305 5300 7402 7c01 6402 6403 6404  |...S.t.|.d.d.d.
-00000770: 6405 8d04 8f22 7d05 7c05 a003 a100 7d06  d...."}.|.....}.
-00000780: 7404 7c06 7c01 8302 5700 0200 6400 0400  t.|.|...W...d...
-00000790: 0400 8303 0100 5300 3100 7352 3000 0100  ......S.1.sR0...
-000007a0: 0100 0100 5900 0100 6400 5300 2906 4e7a  ....Y...d.S.).Nz
-000007b0: 042e 7064 6672 1f00 0000 7a05 7574 662d  ..pdfr....z.utf-
-000007c0: 38da 0669 676e 6f72 6529 02da 0865 6e63  8..ignore)...enc
-000007d0: 6f64 696e 67da 0665 7272 6f72 7329 05da  oding..errors)..
-000007e0: 0865 6e64 7377 6974 6872 0e00 0000 da04  .endswithr......
-000007f0: 6f70 656e da04 7265 6164 7220 0000 0029  open..readr ...)
-00000800: 07da 036d 6435 7223 0000 00da 0c73 656d  ...md5r#.....sem
-00000810: 616e 7472 615f 6469 72da 0566 6f72 6365  antra_dir..force
-00000820: da06 7369 6c65 6e74 da01 6672 2200 0000  ..silent..fr"...
-00000830: 7226 0000 0072 2600 0000 7227 0000 00da  r&...r&...r'....
-00000840: 1067 6574 5f74 6578 745f 636f 6e74 656e  .get_text_conten
-00000850: 742e 0000 0073 0a00 0000 0001 0a01 1002  t....s..........
-00000860: 1201 0801 7237 0000 0069 983a 0000 6300  ....r7...i.:..c.
-00000870: 0000 0000 0000 0000 0000 0000 0000 0003  ................
-00000880: 0000 0040 0000 0073 5000 0000 6500 5a01  ...@...sP...e.Z.
-00000890: 6400 5a02 6401 6402 8400 5a03 6504 6403  d.Z.d.d...Z.e.d.
-000008a0: 6404 8400 8301 5a05 6504 6405 6406 8400  d.....Z.e.d.d...
-000008b0: 8301 5a06 6504 6407 6408 8400 8301 5a07  ..Z.e.d.d.....Z.
-000008c0: 6504 6409 640a 8400 8301 5a08 6504 640b  e.d.d.....Z.e.d.
-000008d0: 640c 8400 8301 5a09 640d 5300 290e da08  d.....Z.d.S.)...
-000008e0: 446f 6375 6d65 6e74 630d 0000 0000 0000  Documentc.......
-000008f0: 0000 0000 000d 0000 0002 0000 0043 0000  .............C..
-00000900: 0073 4c00 0000 7c01 7c00 5f00 7c02 7c00  .sL...|.|._.|.|.
-00000910: 5f01 7c03 7c00 5f02 7c04 7c00 5f03 7c05  _.|.|._.|.|._.|.
-00000920: 7c00 5f04 7c06 7c00 5f05 7c07 7c00 5f06  |._.|.|._.|.|._.
-00000930: 7c08 7c00 5f07 7c09 7c00 5f08 7c0a 7c00  |.|._.|.|._.|.|.
-00000940: 5f09 7c0b 7c00 5f0a 7c0c 7c00 5f0b 6400  _.|.|._.|.|._.d.
-00000950: 5300 a901 4ea9 0c72 2300 0000 7232 0000  S...N..r#...r2..
-00000960: 0072 3300 0000 da0d 6261 7365 5f66 696c  .r3.....base_fil
-00000970: 656e 616d 65da 0663 6f6e 6669 67da 1465  ename..config..e
-00000980: 6d62 6564 6469 6e67 735f 6669 6c65 6e61  mbeddings_filena
-00000990: 6d65 73da 0975 7365 5f61 6e6e 6f79 da0f  mes..use_annoy..
-000009a0: 616e 6e6f 795f 6669 6c65 6e61 6d65 73da  annoy_filenames.
-000009b0: 0777 696e 646f 7773 da07 6f66 6673 6574  .windows..offset
-000009c0: 73da 0f74 6f6b 656e 735f 6669 6c65 6e61  s..tokens_filena
-000009d0: 6d65 da0e 6e75 6d5f 6469 6d65 6e73 696f  me..num_dimensio
-000009e0: 6e73 290d 7225 0000 0072 2300 0000 7232  ns).r%...r#...r2
-000009f0: 0000 0072 3300 0000 723b 0000 0072 3c00  ...r3...r;...r<.
-00000a00: 0000 723d 0000 0072 3e00 0000 723f 0000  ..r=...r>...r?..
-00000a10: 0072 4000 0000 7241 0000 0072 4200 0000  .r@...rA...rB...
-00000a20: 7243 0000 0072 2600 0000 7226 0000 0072  rC...r&...r&...r
-00000a30: 2700 0000 7228 0000 003b 0000 0073 1800  '...r(...;...s..
-00000a40: 0000 000f 0601 0601 0601 0601 0601 0601  ................
-00000a50: 0601 0601 0601 0601 0601 7a11 446f 6375  ..........z.Docu
-00000a60: 6d65 6e74 2e5f 5f69 6e69 745f 5f63 0100  ment.__init__c..
-00000a70: 0000 0000 0000 0000 0000 0100 0000 0600  ................
-00000a80: 0000 4300 0000 7316 0000 0074 007c 006a  ..C...s....t.|.j
-00000a90: 017c 006a 027c 006a 0364 0164 0283 0553  .|.j.|.j.d.d...S
-00000aa0: 0029 034e 4654 2904 7237 0000 0072 3200  .).NFT).r7...r2.
-00000ab0: 0000 7223 0000 0072 3300 0000 a901 7225  ..r#...r3.....r%
-00000ac0: 0000 0072 2600 0000 7226 0000 0072 2700  ...r&...r&...r'.
-00000ad0: 0000 da07 636f 6e74 656e 7457 0000 0073  ....contentW...s
-00000ae0: 0200 0000 0002 7a10 446f 6375 6d65 6e74  ......z.Document
-00000af0: 2e63 6f6e 7465 6e74 6301 0000 0000 0000  .contentc.......
-00000b00: 0000 0000 0002 0000 0008 0000 0043 0000  .............C..
-00000b10: 0073 3e00 0000 7400 7c00 6a01 6401 8302  .s>...t.|.j.d...
-00000b20: 8f1e 7d01 7402 a003 7c01 a004 a100 a101  ..}.t...|.......
-00000b30: 5700 0200 6400 0400 0400 8303 0100 5300  W...d.........S.
-00000b40: 3100 7330 3000 0100 0100 0100 5900 0100  1.s00.......Y...
-00000b50: 6400 5300 2902 4e72 1f00 0000 2905 7230  d.S.).Nr....).r0
-00000b60: 0000 0072 4200 0000 da04 6a73 6f6e da05  ...rB.....json..
-00000b70: 6c6f 6164 7372 3100 0000 2902 7225 0000  loadsr1...).r%..
-00000b80: 0072 3600 0000 7226 0000 0072 2600 0000  .r6...r&...r&...
-00000b90: 7227 0000 00da 0b74 6578 745f 6368 756e  r'.....text_chun
-00000ba0: 6b73 5b00 0000 7304 0000 0000 020e 017a  ks[...s........z
-00000bb0: 1444 6f63 756d 656e 742e 7465 7874 5f63  .Document.text_c
-00000bc0: 6875 6e6b 7363 0100 0000 0000 0000 0000  hunksc..........
-00000bd0: 0000 0100 0000 0300 0000 4300 0000 730e  ..........C...s.
-00000be0: 0000 0074 007c 006a 0164 0119 0083 0153  ...t.|.j.d.....S
-00000bf0: 00a9 024e 7201 0000 0029 02da 036c 656e  ...Nr....)...len
-00000c00: 7241 0000 0072 4400 0000 7226 0000 0072  rA...rD...r&...r
-00000c10: 2600 0000 7227 0000 00da 0e6e 756d 5f65  &...r'.....num_e
-00000c20: 6d62 6564 6469 6e67 7360 0000 0073 0200  mbeddings`...s..
-00000c30: 0000 0002 7a17 446f 6375 6d65 6e74 2e6e  ....z.Document.n
-00000c40: 756d 5f65 6d62 6564 6469 6e67 7363 0100  um_embeddingsc..
-00000c50: 0000 0000 0000 0000 0000 0100 0000 0300  ................
-00000c60: 0000 4300 0000 7320 0000 007c 006a 0073  ..C...s ...|.j.s
-00000c70: 0e74 0164 0183 0182 0174 027c 006a 0364  .t.d.....t.|.j.d
-00000c80: 0219 007c 006a 0483 0253 0029 034e 7a2b  ...|.j...S.).Nz+
-00000c90: 456d 6265 6464 696e 6773 2061 7265 206e  Embeddings are n
-00000ca0: 6f74 2073 746f 7265 6420 696e 2041 6e6e  ot stored in Ann
-00000cb0: 6f79 2064 6174 6162 6173 6572 0100 0000  oy databaser....
-00000cc0: 2905 723e 0000 00da 0a56 616c 7565 4572  ).r>.....ValueEr
-00000cd0: 726f 7272 1b00 0000 723f 0000 0072 4300  rorr....r?...rC.
-00000ce0: 0000 7244 0000 0072 2600 0000 7226 0000  ..rD...r&...r&..
-00000cf0: 0072 2700 0000 da0c 656d 6265 6464 696e  .r'.....embeddin
-00000d00: 675f 6462 6400 0000 7306 0000 0000 0206  g_dbd...s.......
-00000d10: 0108 017a 1544 6f63 756d 656e 742e 656d  ...z.Document.em
-00000d20: 6265 6464 696e 675f 6462 6301 0000 0000  bedding_dbc.....
-00000d30: 0000 0000 0000 0003 0000 0004 0000 0043  ...............C
-00000d40: 0000 0073 2c00 0000 7400 7c00 6a01 6401  ...s,...t.|.j.d.
-00000d50: 1900 7c00 6a02 7c00 6a03 8303 5c02 7d01  ..|.j.|.j...\.}.
-00000d60: 7d02 7c02 7c00 6a03 6b02 7328 4a00 8201  }.|.|.j.k.s(J...
-00000d70: 7c01 5300 7249 0000 0029 0472 1500 0000  |.S.rI...).r....
-00000d80: 723d 0000 0072 4300 0000 724b 0000 0029  r=...rC...rK...)
-00000d90: 0372 2500 0000 da07 7265 7375 6c74 735a  .r%.....resultsZ
-00000da0: 0f65 6d62 6564 6469 6e67 5f63 6f75 6e74  .embedding_count
-00000db0: 7226 0000 0072 2600 0000 7227 0000 00da  r&...r&...r'....
-00000dc0: 0a65 6d62 6564 6469 6e67 736a 0000 0073  .embeddingsj...s
-00000dd0: 0e00 0000 0002 0201 0801 0401 04fd 0805  ................
-00000de0: 0e01 7a13 446f 6375 6d65 6e74 2e65 6d62  ..z.Document.emb
-00000df0: 6564 6469 6e67 734e 290a 7229 0000 0072  eddingsN).r)...r
-00000e00: 2a00 0000 722b 0000 0072 2800 0000 da08  *...r+...r(.....
-00000e10: 7072 6f70 6572 7479 7245 0000 0072 4800  propertyrE...rH.
-00000e20: 0000 724b 0000 0072 4d00 0000 724f 0000  ..rK...rM...rO..
-00000e30: 0072 2600 0000 7226 0000 0072 2600 0000  .r&...r&...r&...
-00000e40: 7227 0000 0072 3800 0000 3a00 0000 7316  r'...r8...:...s.
-00000e50: 0000 0008 0108 1c02 010a 0302 010a 0402  ................
-00000e60: 010a 0302 010a 0502 0172 3800 0000 630d  .........r8...c.
-00000e70: 0000 0000 0000 0000 0000 002a 0000 000e  ...........*....
-00000e80: 0000 0003 0000 0073 9e04 0000 7400 6a01  .......s....t.j.
-00000e90: a002 7c01 a101 7316 7400 a003 7c01 a101  ..|...s.t...|...
-00000ea0: 0100 7404 7c00 8301 7d0d 7400 6a01 a005  ..t.|...}.t.j...
-00000eb0: 7c00 a101 7d0e 8803 a006 a100 7d0f 7407  |...}.......}.t.
-00000ec0: a008 7409 a00a 7c0f a101 a00b a100 a101  ..t...|.........
-00000ed0: a00c 740d a101 7d10 7400 6a01 a00e 7c01  ..t...}.t.j...|.
-00000ee0: 740f 7c0d 7c10 8302 a102 7d11 7400 6a01  t.|.|.....}.t.j.
-00000ef0: a00e 7c01 7410 7c0d 7c10 8302 a102 7d12  ..|.t.|.|.....}.
-00000f00: 6401 7d13 7c0a 7388 7400 6a01 a002 7c11  d.}.|.s.t.j...|.
-00000f10: a101 73f4 7411 7c0d 7c00 7c01 7c0a 7c0b  ..s.t.|.|.|.|.|.
-00000f20: 8305 7d14 7c14 6a12 7d15 8803 a013 7c15  ..}.|.j.}.....|.
-00000f30: a101 8907 6402 7d13 8803 a014 7c15 8807  ....d.}.....|...
-00000f40: a102 7d16 7415 7c11 6403 8302 8f20 8902  ..}.t.|.d.... ..
-00000f50: 8802 a016 7409 a00a 7c16 a101 a101 0100  ....t...|.......
-00000f60: 5700 6400 0400 0400 8303 0100 6e10 3100  W.d.........n.1.
-00000f70: 73e8 3000 0100 0100 0100 5900 0100 6e3a  s.0.......Y...n:
-00000f80: 7415 7c11 6404 8302 8f1e 8902 7409 a017  t.|.d.......t...
-00000f90: 8802 a018 a100 a101 7d16 5700 6400 0400  ........}.W.d...
-00000fa0: 0400 8303 0100 6e12 3100 9001 7324 3000  ......n.1...s$0.
-00000fb0: 0100 0100 0100 5900 0100 7419 7c16 8301  ......Y...t.|...
-00000fc0: 7d17 741a 7c17 7c06 8302 5c02 7d18 7d19  }.t.|.|...\.}.}.
-00000fd0: 6900 7c0f a501 7c00 7c0d 7c0e 8804 7c07  i.|...|.|.|...|.
-00000fe0: 7c06 7c17 7419 7c18 8301 7c19 7c04 7c05  |.|.t.|...|.|.|.
-00000ff0: 741b 6405 9c0c a501 7d1a 7c0a 9001 7382  t.d.....}.|...s.
-00001000: 7400 6a01 a002 7c12 a101 9001 73ae 7c07  t.j...|.....s.|.
-00001010: 6400 7501 9001 72ae 7c0c 9001 73ae 741c  d.u...r.|...s.t.
-00001020: 6a1d 6406 7c19 7c07 1400 6407 9b04 6408  j.d.|.|...d...d.
-00001030: 9d03 6401 6409 8d02 0100 7415 7c12 6403  ..d.d.....t.|.d.
-00001040: 8302 8f20 8902 8802 a016 7409 a00a 7c1a  ... ......t...|.
-00001050: a101 a101 0100 5700 6400 0400 0400 8303  ......W.d.......
-00001060: 0100 6e12 3100 9001 73e0 3000 0100 0100  ..n.1...s.0.....
-00001070: 0100 5900 0100 6700 7d1b 6700 7d1c 741e  ..Y...g.}.g.}.t.
-00001080: 7c19 640a 6402 7c0b 640b 8d04 9002 8f68  |.d.d.|.d......h
-00001090: 7d1d 741f 7c06 7c18 8302 4400 9002 5d4a  }.t.|.|...D...]J
-000010a0: 5c02 5c03 7d1e 7d1f 7d20 7d21 7400 6a01  \.\.}.}.} }!t.j.
-000010b0: a00e 7c01 7420 7c0d 7c10 7c1e 7c1f 7c20  ..|.t |.|.|.|.| 
-000010c0: 8305 a102 7d22 7400 6a01 a00e 7c01 7421  ....}"t.j...|.t!
-000010d0: 7c0d 7c10 7c1e 7c1f 7c20 7c05 8306 a102  |.|.|.|.| |.....
-000010e0: 7d23 7c1b a022 7c22 a101 0100 7c1c a022  }#|.."|"....|.."
-000010f0: 7c23 a101 0100 7400 6a01 a002 7c22 a101  |#....t.j...|"..
-00001100: 9002 72d2 7c04 9002 728c 7400 6a01 a002  ..r.|...r.t.j...
-00001110: 7c23 a101 9002 72d2 7423 7c22 8804 8302  |#....r.t#|"....
-00001120: 7d24 7c04 9002 72a6 7424 7c23 8804 8302  }$|...r.t$|#....
-00001130: 7d25 7c0a 9002 73d2 7c24 7419 7c21 8301  }%|...s.|$t.|!..
-00001140: 6b02 9002 72d2 7c04 9002 7210 7c25 7419  k...r.|...r.|%t.
-00001150: 7c21 8301 6b02 9002 72d2 9002 7110 7c13  |!..k...r...q.|.
-00001160: 9002 72ea 8803 a013 7425 7c16 8301 a101  ..r.....t%|.....
-00001170: 8907 6402 7d13 640c 8900 7c0a 9003 7318  ..d.}.d...|...s.
-00001180: 7400 6a01 a002 7c22 a101 9003 7218 7426  t.j...|"....r.t&
-00001190: 7c22 8804 7419 7c21 8301 8303 5c02 8901  |"..t.|!....\...
-000011a0: 8900 6e1c 7427 6a28 7419 7c21 8301 8804  ..n.t'j(t.|!....
-000011b0: 6602 7427 6a29 640d 8d02 8901 640c 8900  f.t'j)d.....d...
-000011c0: 8800 7d26 640c 7d27 6700 8905 640c 8906  ..}&d.}'g...d...
-000011d0: 7415 7c22 640e 8302 8fe4 8902 8700 8701  t.|"d...........
-000011e0: 8702 8703 8704 8705 8706 8707 6608 640f  ............f.d.
-000011f0: 6410 8408 7d28 7c21 4400 5dae 7d1f 7c1f  d...}(|!D.].}.|.
-00001200: 6411 1900 7c1f 640c 1900 1800 7d1e 7c27  d...|.d.....}.|'
-00001210: 7c26 6b00 9003 72a2 7c27 6411 3700 7d27  |&k...r.|'d.7.}'
-00001220: 7c1d a02a 7c1e a101 0100 9003 716e 7425  |..*|.......qnt%
-00001230: 7c16 7c1f 640c 1900 7c1f 6411 1900 8502  |.|.d...|.d.....
-00001240: 1900 8301 7d29 7419 7c29 8301 640c 6b02  ....})t.|)..d.k.
-00001250: 9003 72d6 7c1d a02a 7c1e a101 0100 9003  ..r.|..*|.......
-00001260: 716e 8805 a022 7c1f a101 0100 8806 7c1e  qn..."|.......|.
-00001270: 3700 8906 7c08 6400 7501 9004 7200 7419  7...|.d.u...r.t.
-00001280: 8805 8301 7c08 6b05 9004 730a 8806 7c09  ....|.k...s...|.
-00001290: 6b05 9004 7210 7c28 8300 0100 7c1d a02a  k...r.|(....|..*
-000012a0: 7c1e a101 0100 9003 716e 7c28 8300 0100  |.......qn|(....
-000012b0: 5700 6400 0400 0400 8303 0100 6e12 3100  W.d.........n.1.
-000012c0: 9004 733a 3000 0100 0100 0100 5900 0100  ..s:0.......Y...
-000012d0: 7c04 9002 7210 742b 7c23 8804 8801 7c05  |...r.t+|#....|.
-000012e0: 6412 8d04 0100 9002 7110 5700 6400 0400  d.......q.W.d...
-000012f0: 0400 8303 0100 6e12 3100 9004 7374 3000  ......n.1...st0.
-00001300: 0100 0100 0100 5900 0100 742c 7c00 7c0d  ......Y...t,|.|.
-00001310: 7c01 7c0e 7c1a 7c1b 7c04 7c1c 7c06 7c18  |.|.|.|.|.|.|.|.
-00001320: 7c11 8804 6413 8d0c 5300 2914 4e54 46da  |...d...S.).NTF.
-00001330: 0177 721f 0000 0029 0c72 2300 0000 7232  .wr....).r#...r2
-00001340: 0000 0072 3b00 0000 7243 0000 00da 0e63  ...r;...rC.....c
-00001350: 6f73 745f 7065 725f 746f 6b65 6e72 4000  ost_per_tokenr@.
-00001360: 0000 da0a 6e75 6d5f 746f 6b65 6e73 724b  ....num_tokensrK
-00001370: 0000 00da 146e 756d 5f65 6d62 6564 6469  .....num_embeddi
-00001380: 6e67 5f74 6f6b 656e 7372 3e00 0000 da0f  ng_tokensr>.....
-00001390: 6e75 6d5f 616e 6e6f 795f 7472 6565 735a  num_annoy_treesZ
-000013a0: 1073 656d 616e 7472 615f 7665 7273 696f  .semantra_versio
-000013b0: 6e7a 1254 6f6b 656e 7320 7769 6c6c 2063  nz.Tokens will c
-000013c0: 6f73 7420 247a 032e 3266 7a0a 2e20 5072  ost $z..2fz.. Pr
-000013d0: 6f63 6565 643f 2901 da05 6162 6f72 747a  oceed?)...abortz
-000013e0: 1643 616c 6375 6c61 7469 6e67 2065 6d62  .Calculating emb
-000013f0: 6564 6469 6e67 7329 04da 0574 6f74 616c  eddings)...total
-00001400: 5a04 6465 7363 5a05 6c65 6176 65da 0764  Z.descZ.leave..d
-00001410: 6973 6162 6c65 7201 0000 0029 015a 0564  isabler....).Z.d
-00001420: 7479 7065 da02 6162 6300 0000 0000 0000  type..abc.......
-00001430: 0000 0000 0002 0000 0006 0000 0013 0000  ................
-00001440: 0073 6c00 0000 7400 8805 8301 6401 6b04  .sl...t.....d.k.
-00001450: 7268 8803 a001 8807 8805 a102 7d00 7402  rh..........}.t.
-00001460: 7c00 6402 8302 722a 7c00 a003 a100 7d00  |.d...r*|.....}.
-00001470: 7c00 8801 8800 8800 7400 8805 8301 1700  |.......t.......
-00001480: 8502 3c00 7c00 4400 5d10 7d01 7404 8802  ..<.|.D.].}.t...
-00001490: 7c01 8804 8303 0100 7142 8800 7400 8805  |.......qB..t...
-000014a0: 8301 3700 8900 6700 8905 6401 8906 6400  ..7...g...d...d.
-000014b0: 5300 2903 4e72 0100 0000 da03 6370 7529  S.).Nr......cpu)
-000014c0: 0572 4a00 0000 5a05 656d 6265 64da 0768  .rJ...Z.embed..h
-000014d0: 6173 6174 7472 725a 0000 0072 1600 0000  asattrrZ...r....
-000014e0: 2902 5a11 656d 6265 6464 696e 675f 7265  ).Z.embedding_re
-000014f0: 7375 6c74 73da 0965 6d62 6564 6469 6e67  sults..embedding
-00001500: a908 5a0f 656d 6265 6464 696e 675f 696e  ..Z.embedding_in
-00001510: 6465 7872 4f00 0000 7236 0000 00da 056d  dexrO...r6.....m
-00001520: 6f64 656c 7243 0000 005a 0470 6f6f 6c5a  odelrC...Z.poolZ
-00001530: 1070 6f6f 6c5f 746f 6b65 6e5f 636f 756e  .pool_token_coun
-00001540: 74da 0674 6f6b 656e 7372 2600 0000 7227  t..tokensr&...r'
-00001550: 0000 00da 0a66 6c75 7368 5f70 6f6f 6c03  .....flush_pool.
-00001560: 0100 0073 1a00 0000 0003 0c01 0c02 0a01  ...s............
-00001570: 0803 02fe 0201 0eff 0203 0801 0e01 0c01  ................
-00001580: 0401 7a1b 7072 6f63 6573 732e 3c6c 6f63  ..z.process.<loc
-00001590: 616c 733e 2e66 6c75 7368 5f70 6f6f 6c72  als>.flush_poolr
-000015a0: 0900 0000 2904 7223 0000 0072 4300 0000  ....).r#...rC...
-000015b0: 724f 0000 005a 096e 756d 5f74 7265 6573  rO...Z.num_trees
-000015c0: 723a 0000 0029 2dda 026f 73da 0470 6174  r:...)-..os..pat
-000015d0: 68da 0665 7869 7374 73da 086d 616b 6564  h..exists..maked
-000015e0: 6972 7372 0f00 0000 da08 6261 7365 6e61  irsr......basena
-000015f0: 6d65 5a0a 6765 745f 636f 6e66 6967 da07  meZ.get_config..
-00001600: 6861 7368 6c69 625a 0973 6861 6b65 5f32  hashlibZ.shake_2
-00001610: 3536 7246 0000 00da 0564 756d 7073 da06  56rF.....dumps..
-00001620: 656e 636f 6465 5a09 6865 7864 6967 6573  encodeZ.hexdiges
-00001630: 7472 1d00 0000 da04 6a6f 696e 7210 0000  tr......joinr...
-00001640: 0072 1100 0000 7237 0000 0072 2200 0000  .r....r7...r"...
-00001650: 5a0a 6765 745f 746f 6b65 6e73 5a0f 6765  Z.get_tokensZ.ge
-00001660: 745f 7465 7874 5f63 6875 6e6b 7372 3000  t_text_chunksr0.
-00001670: 0000 da05 7772 6974 6572 4700 0000 7231  ....writerG...r1
-00001680: 0000 0072 4a00 0000 7214 0000 00da 0756  ...rJ...r......V
-00001690: 4552 5349 4f4e da05 636c 6963 6b5a 0763  ERSION..clickZ.c
-000016a0: 6f6e 6669 726d 7202 0000 00da 037a 6970  onfirmr......zip
-000016b0: 7212 0000 0072 1800 0000 da06 6170 7065  r....r......appe
-000016c0: 6e64 7213 0000 0072 1900 0000 7217 0000  ndr....r....r...
-000016d0: 0072 1500 0000 da02 6e70 da05 656d 7074  .r......np..empt
-000016e0: 795a 0766 6c6f 6174 3332 da06 7570 6461  yZ.float32..upda
-000016f0: 7465 721a 0000 0072 3800 0000 292a 7223  ter....r8...)*r#
-00001700: 0000 0072 3300 0000 725e 0000 0072 4300  ...r3...r^...rC.
-00001710: 0000 723e 0000 0072 5500 0000 7240 0000  ..r>...rU...r@..
-00001720: 0072 5200 0000 da0a 706f 6f6c 5f63 6f75  .rR.....pool_cou
-00001730: 6e74 da09 706f 6f6c 5f73 697a 6572 3400  nt..pool_sizer4.
-00001740: 0000 7235 0000 00da 0a6e 6f5f 636f 6e66  ..r5.....no_conf
-00001750: 6972 6d72 3200 0000 723b 0000 0072 3c00  irmr2...r;...r<.
-00001760: 0000 5a0b 636f 6e66 6967 5f68 6173 6872  ..Z.config_hashr
-00001770: 4200 0000 5a0f 636f 6e66 6967 5f66 696c  B...Z.config_fil
-00001780: 656e 616d 655a 1773 686f 756c 645f 6361  enameZ.should_ca
-00001790: 6c63 756c 6174 655f 746f 6b65 6e73 7245  lculate_tokensrE
-000017a0: 0000 0072 2100 0000 7248 0000 0072 5300  ...r!...rH...rS.
-000017b0: 0000 7241 0000 0072 5400 0000 5a0b 6675  ..rA...rT...Z.fu
-000017c0: 6c6c 5f63 6f6e 6669 6772 3d00 0000 723f  ll_configr=...r?
-000017d0: 0000 00da 0470 6261 72da 0473 697a 65da  .....pbar..size.
-000017e0: 066f 6666 7365 74da 0672 6577 696e 645a  .offset..rewindZ
-000017f0: 0b73 7562 5f6f 6666 7365 7473 5a13 656d  .sub_offsetsZ.em
-00001800: 6265 6464 696e 6773 5f66 696c 656e 616d  beddings_filenam
-00001810: 655a 0e61 6e6e 6f79 5f66 696c 656e 616d  eZ.annoy_filenam
-00001820: 6572 4b00 0000 5a14 6e75 6d5f 616e 6e6f  erK...Z.num_anno
-00001830: 795f 656d 6265 6464 696e 6773 5a08 6e75  y_embeddingsZ.nu
-00001840: 6d5f 736b 6970 da09 6974 6572 6174 696f  m_skip..iteratio
-00001850: 6e72 6000 0000 5a0b 7769 6e64 6f77 5f74  nr`...Z.window_t
-00001860: 6578 7472 2600 0000 725d 0000 0072 2700  extr&...r]...r'.
-00001870: 0000 da07 7072 6f63 6573 7375 0000 0073  ....processu...s
-00001880: 2a01 0000 0010 0c01 0a03 0801 0c01 0801  *...............
-00001890: 1a03 1401 1402 0401 1002 1001 0601 0a01  ................
-000018a0: 0401 0c01 0c01 3002 0c01 2e01 0806 08fd  ......0.........
-000018b0: 0201 0201 0204 0201 02ff 0202 0201 0201  ................
-000018c0: 0201 0201 0201 0201 0201 0601 0201 0201  ................
-000018d0: 0201 02f3 0810 1401 1001 0401 1001 02fe  ................
-000018e0: 0606 0c01 3002 0401 0401 0201 0201 0201  ....0...........
-000018f0: 0201 02fc 0805 0201 1a01 0601 0201 0efe  ................
-00001900: 0404 0601 0201 0201 0cff 02fe 0406 0a01  ................
-00001910: 0a02 0e01 02ff 0401 0aff 0403 0a01 0601  ................
-00001920: 0201 04ff 0405 02ff 0402 0afe 0403 02fd  ................
-00001930: 0403 0afd 0406 0402 0601 0e01 0403 0401  ................
-00001940: 1401 0201 0aff 0a04 0401 0eff 0603 0402  ................
-00001950: 0401 0403 0401 0402 0c02 1a11 0801 1003  ................
-00001960: 0a01 0801 0a01 0402 1801 0e01 0a01 0402  ................
-00001970: 0a01 0802 06ff 0401 0aff 0402 06fe 0403  ................
-00001980: 0601 0e02 2603 0601 0201 0201 0201 0201  ....&...........
-00001990: 02fc 2a07 0201 0201 0201 0201 0201 0201  ..*.............
-000019a0: 0201 0201 0201 0201 0201 0201 02f4 727a  ..............rz
-000019b0: 0000 007a 1a6c 6973 745b 7475 706c 655b  ...z.list[tuple[
-000019c0: 696e 742c 2069 6e74 2c20 696e 745d 5d29  int, int, int]])
-000019d0: 0272 4000 0000 da06 7265 7475 726e 6301  .r@.....returnc.
-000019e0: 0000 0000 0000 0000 0000 0005 0000 0005  ................
-000019f0: 0000 0063 0000 0073 7800 0000 7c00 a000  ...c...sx...|...
-00001a00: 6401 a101 4400 5d68 7d01 6402 7c01 7600  d...D.]h}.d.|.v.
-00001a10: 7262 7c01 a001 6402 a101 6403 6b02 7238  rb|...d...d.k.r8
-00001a20: 7c01 a000 6402 a101 5c02 7d02 7d03 6404  |...d...\.}.}.d.
-00001a30: 7d04 6e10 7c01 a000 6402 a101 5c03 7d02  }.n.|...d...\.}.
-00001a40: 7d03 7d04 7402 7c02 8301 7402 7c03 8301  }.}.t.|...t.|...
-00001a50: 7402 7c04 8301 6603 5600 0100 710a 7402  t.|...f.V...q.t.
-00001a60: 7c01 8301 6404 6404 6603 5600 0100 710a  |...d.d.f.V...q.
-00001a70: 6400 5300 2905 4efa 012c da01 5f72 0900  d.S.).N..,.._r..
-00001a80: 0000 7201 0000 0029 03da 0573 706c 6974  ..r....)...split
-00001a90: da05 636f 756e 74da 0369 6e74 2905 7240  ..count..int).r@
-00001aa0: 0000 005a 0677 696e 646f 7772 7600 0000  ...Z.windowrv...
-00001ab0: 7277 0000 0072 7800 0000 7226 0000 0072  rw...rx...r&...r
-00001ac0: 2600 0000 7227 0000 00da 0f70 726f 6365  &...r'.....proce
-00001ad0: 7373 5f77 696e 646f 7773 4501 0000 7310  ss_windowsE...s.
-00001ae0: 0000 0000 010e 0108 020e 010e 0106 0210  ................
-00001af0: 011a 0272 8100 0000 7223 0000 0054 2901  ...r....r#...T).
-00001b00: 7263 0000 00e9 ffff ffff 2902 da04 7479  rc........)...ty
-00001b10: 7065 da05 6e61 7267 737a 072d 2d6d 6f64  pe..nargsz.--mod
-00001b20: 656c 2901 5a0e 6361 7365 5f73 656e 7369  el).Z.case_sensi
-00001b30: 7469 7665 da05 6d70 6e65 747a 2150 7265  tive..mpnetz!Pre
-00001b40: 7365 7420 6d6f 6465 6c20 746f 2075 7365  set model to use
-00001b50: 2066 6f72 2065 6d62 6564 6469 6e67 2904   for embedding).
-00001b60: 7283 0000 00da 0764 6566 6175 6c74 da0c  r......default..
-00001b70: 7368 6f77 5f64 6566 6175 6c74 da04 6865  show_default..he
-00001b80: 6c70 7a13 2d2d 7472 616e 7366 6f72 6d65  lpz.--transforme
-00001b90: 722d 6d6f 6465 6c7a 3f43 7573 746f 6d20  r-modelz?Custom 
-00001ba0: 4875 6767 696e 6766 6163 6520 7472 616e  Huggingface tran
-00001bb0: 7366 6f72 6d65 7273 206d 6f64 656c 206e  sformers model n
-00001bc0: 616d 6520 746f 2075 7365 2066 6f72 2065  ame to use for e
-00001bd0: 6d62 6564 6469 6e67 2902 7283 0000 0072  mbedding).r....r
-00001be0: 8800 0000 7a09 2d2d 7769 6e64 6f77 73da  ....z.--windows.
-00001bf0: 0831 3238 5f30 5f31 3661 1601 0000 456d  .128_0_16a....Em
-00001c00: 6265 6464 696e 6720 7769 6e64 6f77 7320  bedding windows 
-00001c10: 746f 2065 7874 7261 6374 2e20 4120 636f  to extract. A co
-00001c20: 6d6d 612d 7365 7061 7261 7465 6420 6c69  mma-separated li
-00001c30: 7374 206f 6620 7468 6520 666f 726d 6174  st of the format
-00001c40: 2022 7369 7a65 5b5f 6f66 6673 6574 3d30   "size[_offset=0
-00001c50: 5d5b 5f72 6577 696e 643d 305d 2e20 4120  ][_rewind=0]. A 
-00001c60: 7769 6e64 6f77 2077 6974 6820 7369 7a65  window with size
-00001c70: 2031 3238 2c20 6f66 6673 6574 2030 2c20   128, offset 0, 
-00001c80: 616e 6420 7265 7769 6e64 206f 6620 3136  and rewind of 16
-00001c90: 2028 3132 385f 305f 3136 2920 7769 6c6c   (128_0_16) will
-00001ca0: 2065 6d62 6564 2074 6865 2064 6f63 756d   embed the docum
-00001cb0: 656e 7420 696e 2063 6875 6e6b 7320 6f66  ent in chunks of
-00001cc0: 2031 3238 2074 6f6b 656e 7320 7768 6963   128 tokens whic
-00001cd0: 6820 7061 7274 6961 6c6c 7920 6f76 6572  h partially over
-00001ce0: 6c61 7020 6279 2031 362e 204f 6e6c 7920  lap by 16. Only 
-00001cf0: 7468 6520 6669 7273 7420 7769 6e64 6f77  the first window
-00001d00: 2069 7320 7573 6564 2066 6f72 2073 6561   is used for sea
-00001d10: 7263 682e 7a0b 2d2d 6e6f 2d73 6572 7665  rch.z.--no-serve
-00001d20: 7246 7a29 446f 206e 6f74 2073 7461 7274  rFz)Do not start
-00001d30: 2074 6865 2055 4920 7365 7276 6572 2028   the UI server (
-00001d40: 6f6e 6c79 2070 726f 6365 7373 2929 04da  only process))..
-00001d50: 0769 735f 666c 6167 7286 0000 0072 8700  .is_flagr....r..
-00001d60: 0000 7288 0000 007a 062d 2d70 6f72 74e9  ..r....z.--port.
-00001d70: 901f 0000 7a20 506f 7274 2074 6f20 7573  ....z Port to us
-00001d80: 6520 666f 7220 656d 6265 6464 696e 6720  e for embedding 
-00001d90: 7365 7276 6572 7a06 2d2d 686f 7374 fa07  serverz.--host..
-00001da0: 302e 302e 302e 307a 2048 6f73 7420 746f  0.0.0.0z Host to
-00001db0: 2075 7365 2066 6f72 2065 6d62 6564 6469   use for embeddi
-00001dc0: 6e67 2073 6572 7665 727a 0b2d 2d70 6f6f  ng serverz.--poo
-00001dd0: 6c2d 7369 7a65 7a3b 4d61 7820 6e75 6d62  l-sizez;Max numb
-00001de0: 6572 206f 6620 656d 6265 6464 696e 6720  er of embedding 
-00001df0: 746f 6b65 6e73 2074 6f20 706f 6f6c 2074  tokens to pool t
-00001e00: 6f67 6574 6865 7220 696e 2072 6571 7565  ogether in reque
-00001e10: 7374 7329 0372 8300 0000 7286 0000 0072  sts).r....r....r
-00001e20: 8800 0000 7a0c 2d2d 706f 6f6c 2d63 6f75  ....z.--pool-cou
-00001e30: 6e74 7a35 4d61 7820 6e75 6d62 6572 206f  ntz5Max number o
-00001e40: 6620 656d 6265 6464 696e 6773 2074 6f20  f embeddings to 
-00001e50: 706f 6f6c 2074 6f67 6574 6865 7220 696e  pool together in
-00001e60: 2072 6571 7565 7374 737a 0f2d 2d64 6f63   requestsz.--doc
-00001e70: 2d74 6f6b 656e 2d70 7265 7a47 546f 6b65  -token-prezGToke
-00001e80: 6e20 746f 2070 7265 7065 6e64 2074 6f20  n to prepend to 
-00001e90: 6561 6368 2064 6f63 756d 656e 7420 696e  each document in
-00001ea0: 2074 7261 6e73 666f 726d 6572 206d 6f64   transformer mod
-00001eb0: 656c 7320 2864 6566 6175 6c74 3a20 4e6f  els (default: No
-00001ec0: 6e65 297a 102d 2d64 6f63 2d74 6f6b 656e  ne)z.--doc-token
-00001ed0: 2d70 6f73 747a 4654 6f6b 656e 2074 6f20  -postzFToken to 
-00001ee0: 6170 7065 6e64 2074 6f20 6561 6368 2064  append to each d
-00001ef0: 6f63 756d 656e 7420 696e 2074 7261 6e73  ocument in trans
-00001f00: 666f 726d 6572 206d 6f64 656c 7320 2864  former models (d
-00001f10: 6566 6175 6c74 3a20 4e6f 6e65 297a 112d  efault: None)z.-
-00001f20: 2d71 7565 7279 2d74 6f6b 656e 2d70 7265  -query-token-pre
-00001f30: 7a44 546f 6b65 6e20 746f 2070 7265 7065  zDToken to prepe
-00001f40: 6e64 2074 6f20 6561 6368 2071 7565 7279  nd to each query
-00001f50: 2069 6e20 7472 616e 7366 6f72 6d65 7220   in transformer 
-00001f60: 6d6f 6465 6c73 2028 6465 6661 756c 743a  models (default:
-00001f70: 204e 6f6e 6529 7a12 2d2d 7175 6572 792d   None)z.--query-
-00001f80: 746f 6b65 6e2d 706f 7374 7a43 546f 6b65  token-postzCToke
-00001f90: 6e20 746f 2061 7070 656e 6420 746f 2065  n to append to e
-00001fa0: 6163 6820 7175 6572 7920 696e 2074 7261  ach query in tra
+00000040: 6401 6c02 5a02 6400 6401 6c03 5a03 6400  d.l.Z.d.d.l.Z.d.
+00000050: 6401 6c04 5a04 6400 6401 6c05 5a05 6400  d.l.Z.d.d.l.Z.d.
+00000060: 6401 6c06 5a07 6400 6401 6c08 5a08 6400  d.l.Z.d.d.l.Z.d.
+00000070: 6402 6c09 6d0a 5a0a 0100 6400 6403 6c0b  d.l.m.Z...d.d.l.
+00000080: 6d0c 5a0c 6d0d 5a0d 6d0e 5a0e 6d0f 5a0f  m.Z.m.Z.m.Z.m.Z.
+00000090: 6d10 5a10 6d11 5a11 0100 6400 6404 6c12  m.Z.m.Z...d.d.l.
+000000a0: 6d12 5a12 0100 6405 6406 6c13 6d14 5a14  m.Z...d.d.l.m.Z.
+000000b0: 6d15 5a15 6d16 5a16 6d13 5a13 0100 6405  m.Z.m.Z.m.Z...d.
+000000c0: 6407 6c17 6d18 5a18 0100 6405 6408 6c19  d.l.m.Z...d.d.l.
+000000d0: 6d1a 5a1a 6d1b 5a1b 6d1c 5a1c 6d1d 5a1d  m.Z.m.Z.m.Z.m.Z.
+000000e0: 6d1e 5a1e 6d1f 5a1f 6d20 5a20 6d21 5a21  m.Z.m.Z.m Z m!Z!
+000000f0: 6d22 5a22 6d23 5a23 6d24 5a24 6d25 5a25  m"Z"m#Z#m$Z$m%Z%
+00000100: 6d26 5a26 6d27 5a27 6d28 5a28 0100 6508  m&Z&m'Z'm(Z(..e.
+00000110: a029 6409 a101 6400 1900 6a2a 5a2b 640a  .)d...d...j*Z+d.
+00000120: 5a2c 640b 5a2d 6504 6a2e a02f 6504 6a2e  Z,d.Z-e.j../e.j.
+00000130: a030 6531 a101 a101 5a32 4700 640c 640d  .0e1....Z2G.d.d.
+00000140: 8400 640d 8302 5a33 640e 640f 8400 5a34  ..d...Z3d.d...Z4
+00000150: 6410 5a35 4700 6411 6412 8400 6412 8302  d.Z5G.d.d...d...
+00000160: 5a36 6413 6414 8400 5a37 6538 6415 6416  Z6d.d...Z7e8d.d.
+00000170: 9c02 6417 6418 8404 5a39 6505 a03a a100  ..d.d...Z9e..:..
+00000180: 6505 6a3b 6419 6505 6a3c 641a 641b 8d01  e.j;d.e.j<d.d...
+00000190: 641c 641d 8d03 6505 6a3d 641e 6505 6a3e  d.d...e.j=d.e.j>
+000001a0: 6513 a03f a100 641a 641f 8d02 6420 641a  e..?..d.d...d d.
+000001b0: 6421 6422 8d05 6505 6a3d 6423 6538 652c  d!d"..e.j=d#e8e,
+000001c0: 641a 6424 6422 8d05 6505 6a3d 6425 6538  d.d$d"..e.j=d%e8
+000001d0: 6426 6427 8d03 6505 6a3d 6428 6538 6429  d&d'..e.j=d(e8d)
+000001e0: 641a 642a 6422 8d05 6505 6a3d 642b 641a  d.d*d"..e.j=d+d.
+000001f0: 642c 641a 642d 642e 8d05 6505 6a3d 642f  d,d.d-d...e.j=d/
+00000200: 6540 652d 641a 6430 6422 8d05 6505 6a3d  e@e-d.d0d"..e.j=
+00000210: 6431 6538 6432 641a 6433 6422 8d05 6505  d1e8d2d.d3d"..e.
+00000220: 6a3d 6434 6540 6401 6435 6436 8d04 6505  j=d4e@d.d5d6..e.
+00000230: 6a3d 6437 6540 6401 6438 6436 8d04 6505  j=d7e@d.d8d6..e.
+00000240: 6a3d 6439 6538 6401 643a 6436 8d04 6505  j=d9e8d.d:d6..e.
+00000250: 6a3d 643b 6538 6401 643c 6436 8d04 6505  j=d;e8d.d<d6..e.
+00000260: 6a3d 643d 6538 6401 643e 6436 8d04 6505  j=d=e8d.d>d6..e.
+00000270: 6a3d 643f 6538 6401 6440 6436 8d04 6505  j=d?e8d.d@d6..e.
+00000280: 6a3d 6441 6540 6442 641a 6443 6422 8d05  j=dAe@dBd.dCd"..
+00000290: 6505 6a3d 6444 641a 641a 641a 6445 642e  e.j=dDd.d.d.dEd.
+000002a0: 8d05 6505 6a3d 6446 6540 6447 641a 6448  ..e.j=dFe@dGd.dH
+000002b0: 6422 8d05 6505 6a3d 6449 641a 642c 641a  d"..e.j=dId.d,d.
+000002c0: 644a 642e 8d05 6505 6a3d 644b 6541 644c  dJd...e.j=dKeAdL
+000002d0: 641a 644d 6422 8d05 6505 6a3d 644e 6540  d.dMd"..e.j=dNe@
+000002e0: 644f 641a 6450 6422 8d05 6505 6a3d 6451  dOd.dPd"..e.j=dQ
+000002f0: 6540 6452 641a 6453 6422 8d05 6505 6a3d  e@dRd.dSd"..e.j=
+00000300: 6454 6540 6455 641a 6456 6422 8d05 6505  dTe@dUd.dVd"..e.
+00000310: 6a3d 6457 641a 642c 6458 6459 8d04 6505  j=dWd.d,dXdY..e.
+00000320: 6a3d 645a 641a 642c 645b 6459 8d04 6505  j=dZd.d,d[dY..e.
+00000330: 6a3d 645c 641a 642c 645d 6459 8d04 6505  j=d\d.d,d]dY..e.
+00000340: 6a3d 645e 641a 642c 645f 6459 8d04 6505  j=d^d.d,d_dY..e.
+00000350: 6a3d 6460 641a 642c 6461 6459 8d04 6505  j=d`d.d,dadY..e.
+00000360: 6a3d 6462 641a 642c 6463 6459 8d04 6505  j=dbd.d,dcdY..e.
+00000370: 6a3d 6464 6505 6a3c 642c 641b 8d01 6401  j=dde.j<d,d...d.
+00000380: 6465 6436 8d04 6429 642c 640b 6432 6401  ded6..d)d,d.d2d.
+00000390: 6401 6401 6401 6401 6401 6420 6401 652c  d.d.d.d.d.d d.e,
+000003a0: 6447 6442 641a 642c 644c 644f 6452 6455  dGdBd.d,dLdOdRdU
+000003b0: 642c 642c 642c 642c 642c 642c 6401 661c  d,d,d,d,d,d,d.f.
+000003c0: 6466 6467 8401 8301 8301 8301 8301 8301  dfdg............
+000003d0: 8301 8301 8301 8301 8301 8301 8301 8301  ................
+000003e0: 8301 8301 8301 8301 8301 8301 8301 8301  ................
+000003f0: 8301 8301 8301 8301 8301 8301 8301 8301  ................
+00000400: 8301 5a42 6543 6468 6b02 9003 72e6 6542  ..ZBeCdhk...r.eB
+00000410: 8300 0100 6401 5300 2969 e900 0000 004e  ....d.S.)i.....N
+00000420: 2901 da0b 6c6f 6164 5f64 6f74 656e 7629  )...load_dotenv)
+00000430: 06da 0546 6c61 736b da07 6a73 6f6e 6966  ...Flask..jsonif
+00000440: 79da 0d6d 616b 655f 7265 7370 6f6e 7365  y..make_response
+00000450: da07 7265 7175 6573 74da 0973 656e 645f  ..request..send_
+00000460: 6669 6c65 da13 7365 6e64 5f66 726f 6d5f  file..send_from_
+00000470: 6469 7265 6374 6f72 7929 01da 0474 7164  directory)...tqd
+00000480: 6de9 0100 0000 2904 da09 4261 7365 4d6f  m.....)...BaseMo
+00000490: 6465 6cda 1054 7261 6e73 666f 726d 6572  del..Transformer
+000004a0: 4d6f 6465 6cda 0861 735f 6e75 6d70 79da  Model..as_numpy.
+000004b0: 066d 6f64 656c 7329 01da 0f67 6574 5f70  .models)...get_p
+000004c0: 6466 5f63 6f6e 7465 6e74 290f da0b 4841  df_content)...HA
+000004d0: 5348 5f4c 454e 4754 48da 0866 696c 655f  SH_LENGTH..file_
+000004e0: 6d64 35da 1267 6574 5f61 6e6e 6f79 5f66  md5..get_annoy_f
+000004f0: 696c 656e 616d 65da 1367 6574 5f63 6f6e  ilename..get_con
+00000500: 6669 675f 6669 6c65 6e61 6d65 da17 6765  fig_filename..ge
+00000510: 745f 656d 6265 6464 696e 6773 5f66 696c  t_embeddings_fil
+00000520: 656e 616d 65da 1867 6574 5f6e 756d 5f61  ename..get_num_a
+00000530: 6e6e 6f79 5f65 6d62 6564 6469 6e67 73da  nnoy_embeddings.
+00000540: 1267 6574 5f6e 756d 5f65 6d62 6564 6469  .get_num_embeddi
+00000550: 6e67 73da 0b67 6574 5f6f 6666 7365 7473  ngs..get_offsets
+00000560: da13 6765 745f 746f 6b65 6e73 5f66 696c  ..get_tokens_fil
+00000570: 656e 616d 65da 106a 6f69 6e5f 7465 7874  ename..join_text
+00000580: 5f63 6875 6e6b 73da 0d6c 6f61 645f 616e  _chunks..load_an
+00000590: 6e6f 795f 6462 da14 7265 6164 5f65 6d62  noy_db..read_emb
+000005a0: 6564 6469 6e67 735f 6669 6c65 da0c 736f  eddings_file..so
+000005b0: 7274 5f72 6573 756c 7473 da0e 7772 6974  rt_results..writ
+000005c0: 655f 616e 6e6f 795f 6462 da0f 7772 6974  e_annoy_db..writ
+000005d0: 655f 656d 6265 6464 696e 67da 0873 656d  e_embedding..sem
+000005e0: 616e 7472 617a 0575 7466 2d38 6990 1f00  antraz.utf-8i...
+000005f0: 0063 0000 0000 0000 0000 0000 0000 0000  .c..............
+00000600: 0000 0200 0000 4000 0000 7314 0000 0065  ......@...s....e
+00000610: 005a 0164 005a 0264 0164 0284 005a 0364  .Z.d.Z.d.d...Z.d
+00000620: 0353 0029 04da 0743 6f6e 7465 6e74 6303  .S.)...Contentc.
+00000630: 0000 0000 0000 0000 0000 0003 0000 0002  ................
+00000640: 0000 0043 0000 0073 1600 0000 7c01 7c00  ...C...s....|.|.
+00000650: 5f00 7c02 7c00 5f01 6401 7c00 5f02 6400  _.|.|._.d.|._.d.
+00000660: 5300 2902 4eda 0474 6578 7429 03da 0772  S.).N..text)...r
+00000670: 6177 7465 7874 da08 6669 6c65 6e61 6d65  awtext..filename
+00000680: da08 6669 6c65 7479 7065 2903 da04 7365  ..filetype)...se
+00000690: 6c66 7222 0000 0072 2300 0000 a900 7226  lfr"...r#.....r&
+000006a0: 0000 00fa 392f 5573 6572 732f 6672 6565  ....9/Users/free
+000006b0: 646d 616e 642f 7363 7261 7073 2f73 656d  dmand/scraps/sem
+000006c0: 616e 7472 612f 7372 632f 7365 6d61 6e74  antra/src/semant
+000006d0: 7261 2f73 656d 616e 7472 612e 7079 da08  ra/semantra.py..
+000006e0: 5f5f 696e 6974 5f5f 2a00 0000 7306 0000  __init__*...s...
+000006f0: 0000 0106 0106 017a 1043 6f6e 7465 6e74  .......z.Content
+00000700: 2e5f 5f69 6e69 745f 5f4e 2904 da08 5f5f  .__init__N)...__
+00000710: 6e61 6d65 5f5f da0a 5f5f 6d6f 6475 6c65  name__..__module
+00000720: 5f5f da0c 5f5f 7175 616c 6e61 6d65 5f5f  __..__qualname__
+00000730: 7228 0000 0072 2600 0000 7226 0000 0072  r(...r&...r&...r
+00000740: 2600 0000 7227 0000 0072 2000 0000 2900  &...r'...r ...).
+00000750: 0000 7302 0000 0008 0172 2000 0000 6306  ..s......r ...c.
+00000760: 0000 0000 0000 0000 0000 0008 0000 0008  ................
+00000770: 0000 0043 0000 0073 6000 0000 7c01 a000  ...C...s`...|...
+00000780: 6401 a101 721a 7401 7c00 7c01 7c02 7c03  d...r.t.|.|.|.|.
+00000790: 7c04 8305 5300 7402 7c01 6402 7c05 6403  |...S.t.|.d.|.d.
+000007a0: 6404 8d04 8f22 7d06 7c06 a003 a100 7d07  d...."}.|.....}.
+000007b0: 7404 7c07 7c01 8302 5700 0200 6400 0400  t.|.|...W...d...
+000007c0: 0400 8303 0100 5300 3100 7352 3000 0100  ......S.1.sR0...
+000007d0: 0100 0100 5900 0100 6400 5300 2905 4e7a  ....Y...d.S.).Nz
+000007e0: 042e 7064 66da 0172 da06 6967 6e6f 7265  ..pdf..r..ignore
+000007f0: 2902 da08 656e 636f 6469 6e67 da06 6572  )...encoding..er
+00000800: 726f 7273 2905 da08 656e 6473 7769 7468  rors)...endswith
+00000810: 720f 0000 00da 046f 7065 6eda 0472 6561  r......open..rea
+00000820: 6472 2000 0000 2908 da03 6d64 3572 2300  dr ...)...md5r#.
+00000830: 0000 da0c 7365 6d61 6e74 7261 5f64 6972  ....semantra_dir
+00000840: da05 666f 7263 65da 0673 696c 656e 7472  ..force..silentr
+00000850: 2e00 0000 da01 6672 2200 0000 7226 0000  ......fr"...r&..
+00000860: 0072 2600 0000 7227 0000 00da 1067 6574  .r&...r'.....get
+00000870: 5f74 6578 745f 636f 6e74 656e 7430 0000  _text_content0..
+00000880: 0073 0a00 0000 0001 0a01 1002 1201 0801  .s..............
+00000890: 7238 0000 0069 983a 0000 6300 0000 0000  r8...i.:..c.....
+000008a0: 0000 0000 0000 0000 0000 0003 0000 0040  ...............@
+000008b0: 0000 0073 5000 0000 6500 5a01 6400 5a02  ...sP...e.Z.d.Z.
+000008c0: 6401 6402 8400 5a03 6504 6403 6404 8400  d.d...Z.e.d.d...
+000008d0: 8301 5a05 6504 6405 6406 8400 8301 5a06  ..Z.e.d.d.....Z.
+000008e0: 6504 6407 6408 8400 8301 5a07 6504 6409  e.d.d.....Z.e.d.
+000008f0: 640a 8400 8301 5a08 6504 640b 640c 8400  d.....Z.e.d.d...
+00000900: 8301 5a09 640d 5300 290e da08 446f 6375  ..Z.d.S.)...Docu
+00000910: 6d65 6e74 630e 0000 0000 0000 0000 0000  mentc...........
+00000920: 000e 0000 0002 0000 0043 0000 0073 5200  .........C...sR.
+00000930: 0000 7c01 7c00 5f00 7c02 7c00 5f01 7c03  ..|.|._.|.|._.|.
+00000940: 7c00 5f02 7c04 7c00 5f03 7c05 7c00 5f04  |._.|.|._.|.|._.
+00000950: 7c06 7c00 5f05 7c07 7c00 5f06 7c08 7c00  |.|._.|.|._.|.|.
+00000960: 5f07 7c09 7c00 5f08 7c0a 7c00 5f09 7c0b  _.|.|._.|.|._.|.
+00000970: 7c00 5f0a 7c0c 7c00 5f0b 7c0d 7c00 5f0c  |._.|.|._.|.|._.
+00000980: 6400 5300 a901 4ea9 0d72 2300 0000 7233  d.S...N..r#...r3
+00000990: 0000 0072 3400 0000 da0d 6261 7365 5f66  ...r4.....base_f
+000009a0: 696c 656e 616d 65da 0663 6f6e 6669 67da  ilename..config.
+000009b0: 1465 6d62 6564 6469 6e67 735f 6669 6c65  .embeddings_file
+000009c0: 6e61 6d65 73da 0975 7365 5f61 6e6e 6f79  names..use_annoy
+000009d0: da0f 616e 6e6f 795f 6669 6c65 6e61 6d65  ..annoy_filename
+000009e0: 73da 0777 696e 646f 7773 da07 6f66 6673  s..windows..offs
+000009f0: 6574 73da 0f74 6f6b 656e 735f 6669 6c65  ets..tokens_file
+00000a00: 6e61 6d65 da0e 6e75 6d5f 6469 6d65 6e73  name..num_dimens
+00000a10: 696f 6e73 722e 0000 0029 0e72 2500 0000  ionsr....).r%...
+00000a20: 7223 0000 0072 3300 0000 7234 0000 0072  r#...r3...r4...r
+00000a30: 3c00 0000 723d 0000 0072 3e00 0000 723f  <...r=...r>...r?
+00000a40: 0000 0072 4000 0000 7241 0000 0072 4200  ...r@...rA...rB.
+00000a50: 0000 7243 0000 0072 4400 0000 722e 0000  ..rC...rD...r...
+00000a60: 0072 2600 0000 7226 0000 0072 2700 0000  .r&...r&...r'...
+00000a70: 7228 0000 003d 0000 0073 1a00 0000 0010  r(...=...s......
+00000a80: 0601 0601 0601 0601 0601 0601 0601 0601  ................
+00000a90: 0601 0601 0601 0601 7a11 446f 6375 6d65  ........z.Docume
+00000aa0: 6e74 2e5f 5f69 6e69 745f 5f63 0100 0000  nt.__init__c....
+00000ab0: 0000 0000 0000 0000 0100 0000 0700 0000  ................
+00000ac0: 4300 0000 731a 0000 0074 007c 006a 017c  C...s....t.|.j.|
+00000ad0: 006a 027c 006a 0364 0164 027c 006a 0483  .j.|.j.d.d.|.j..
+00000ae0: 0653 0029 034e 4654 2905 7238 0000 0072  .S.).NFT).r8...r
+00000af0: 3300 0000 7223 0000 0072 3400 0000 722e  3...r#...r4...r.
+00000b00: 0000 00a9 0172 2500 0000 7226 0000 0072  .....r%...r&...r
+00000b10: 2600 0000 7227 0000 00da 0763 6f6e 7465  &...r'.....conte
+00000b20: 6e74 5b00 0000 7306 0000 0000 0202 0114  nt[...s.........
+00000b30: ff7a 1044 6f63 756d 656e 742e 636f 6e74  .z.Document.cont
+00000b40: 656e 7463 0100 0000 0000 0000 0000 0000  entc............
+00000b50: 0200 0000 0800 0000 4300 0000 733e 0000  ........C...s>..
+00000b60: 0074 007c 006a 0164 0183 028f 1e7d 0174  .t.|.j.d.....}.t
+00000b70: 02a0 037c 01a0 04a1 00a1 0157 0002 0064  ...|.......W...d
+00000b80: 0004 0004 0083 0301 0053 0031 0073 3030  .........S.1.s00
+00000b90: 0001 0001 0001 0059 0001 0064 0053 0029  .......Y...d.S.)
+00000ba0: 024e 722c 0000 0029 0572 3100 0000 7243  .Nr,...).r1...rC
+00000bb0: 0000 00da 046a 736f 6eda 056c 6f61 6473  .....json..loads
+00000bc0: 7232 0000 0029 0272 2500 0000 7237 0000  r2...).r%...r7..
+00000bd0: 0072 2600 0000 7226 0000 0072 2700 0000  .r&...r&...r'...
+00000be0: da0b 7465 7874 5f63 6875 6e6b 7361 0000  ..text_chunksa..
+00000bf0: 0073 0400 0000 0002 0e01 7a14 446f 6375  .s........z.Docu
+00000c00: 6d65 6e74 2e74 6578 745f 6368 756e 6b73  ment.text_chunks
+00000c10: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
+00000c20: 0003 0000 0043 0000 0073 0e00 0000 7400  .....C...s....t.
+00000c30: 7c00 6a01 6401 1900 8301 5300 a902 4e72  |.j.d.....S...Nr
+00000c40: 0100 0000 2902 da03 6c65 6e72 4200 0000  ....)...lenrB...
+00000c50: 7245 0000 0072 2600 0000 7226 0000 0072  rE...r&...r&...r
+00000c60: 2700 0000 da0e 6e75 6d5f 656d 6265 6464  '.....num_embedd
+00000c70: 696e 6773 6600 0000 7302 0000 0000 027a  ingsf...s......z
+00000c80: 1744 6f63 756d 656e 742e 6e75 6d5f 656d  .Document.num_em
+00000c90: 6265 6464 696e 6773 6301 0000 0000 0000  beddingsc.......
+00000ca0: 0000 0000 0001 0000 0003 0000 0043 0000  .............C..
+00000cb0: 0073 2000 0000 7c00 6a00 730e 7401 6401  .s ...|.j.s.t.d.
+00000cc0: 8301 8201 7402 7c00 6a03 6402 1900 7c00  ....t.|.j.d...|.
+00000cd0: 6a04 8302 5300 2903 4e7a 2b45 6d62 6564  j...S.).Nz+Embed
+00000ce0: 6469 6e67 7320 6172 6520 6e6f 7420 7374  dings are not st
+00000cf0: 6f72 6564 2069 6e20 416e 6e6f 7920 6461  ored in Annoy da
+00000d00: 7461 6261 7365 7201 0000 0029 0572 3f00  tabaser....).r?.
+00000d10: 0000 da0a 5661 6c75 6545 7272 6f72 721a  ....ValueErrorr.
+00000d20: 0000 0072 4000 0000 7244 0000 0072 4500  ...r@...rD...rE.
+00000d30: 0000 7226 0000 0072 2600 0000 7227 0000  ..r&...r&...r'..
+00000d40: 00da 0c65 6d62 6564 6469 6e67 5f64 626a  ...embedding_dbj
+00000d50: 0000 0073 0600 0000 0002 0601 0801 7a15  ...s..........z.
+00000d60: 446f 6375 6d65 6e74 2e65 6d62 6564 6469  Document.embeddi
+00000d70: 6e67 5f64 6263 0100 0000 0000 0000 0000  ng_dbc..........
+00000d80: 0000 0300 0000 0400 0000 4300 0000 732c  ..........C...s,
+00000d90: 0000 0074 007c 006a 0164 0119 007c 006a  ...t.|.j.d...|.j
+00000da0: 027c 006a 0383 035c 027d 017d 027c 027c  .|.j...\.}.}.|.|
+00000db0: 006a 036b 0273 284a 0082 017c 0153 0072  .j.k.s(J...|.S.r
+00000dc0: 4a00 0000 2904 721b 0000 0072 3e00 0000  J...).r....r>...
+00000dd0: 7244 0000 0072 4c00 0000 2903 7225 0000  rD...rL...).r%..
+00000de0: 00da 0772 6573 756c 7473 5a0f 656d 6265  ...resultsZ.embe
+00000df0: 6464 696e 675f 636f 756e 7472 2600 0000  dding_countr&...
+00000e00: 7226 0000 0072 2700 0000 da0a 656d 6265  r&...r'.....embe
+00000e10: 6464 696e 6773 7000 0000 730e 0000 0000  ddingsp...s.....
+00000e20: 0202 0108 0104 0104 fd08 050e 017a 1344  .............z.D
+00000e30: 6f63 756d 656e 742e 656d 6265 6464 696e  ocument.embeddin
+00000e40: 6773 4e29 0a72 2900 0000 722a 0000 0072  gsN).r)...r*...r
+00000e50: 2b00 0000 7228 0000 00da 0870 726f 7065  +...r(.....prope
+00000e60: 7274 7972 4600 0000 7249 0000 0072 4c00  rtyrF...rI...rL.
+00000e70: 0000 724e 0000 0072 5000 0000 7226 0000  ..rN...rP...r&..
+00000e80: 0072 2600 0000 7226 0000 0072 2700 0000  .r&...r&...r'...
+00000e90: 7239 0000 003c 0000 0073 1600 0000 0801  r9...<...s......
+00000ea0: 081e 0201 0a05 0201 0a04 0201 0a03 0201  ................
+00000eb0: 0a05 0201 7239 0000 0063 0e00 0000 0000  ....r9...c......
+00000ec0: 0000 0000 0000 2b00 0000 0f00 0000 0300  ......+.........
+00000ed0: 0000 73b4 0400 0074 006a 01a0 027c 01a1  ..s....t.j...|..
+00000ee0: 0173 1674 00a0 037c 01a1 0101 0074 047c  .s.t...|.....t.|
+00000ef0: 0083 017d 0e74 006a 01a0 057c 00a1 017d  ...}.t.j...|...}
+00000f00: 0f88 03a0 06a1 007d 107c 0d74 076b 0372  .......}.|.t.k.r
+00000f10: 427c 0d7c 1064 013c 0074 08a0 0974 0aa0  B|.|.d.<.t...t..
+00000f20: 0b7c 10a1 01a0 0ca1 00a1 01a0 0d74 0ea1  .|...........t..
+00000f30: 017d 1174 006a 01a0 0f7c 0174 107c 0e7c  .}.t.j...|.t.|.|
+00000f40: 1183 02a1 027d 1274 006a 01a0 0f7c 0174  .....}.t.j...|.t
+00000f50: 117c 0e7c 1183 02a1 027d 1364 027d 147c  .|.|.....}.d.}.|
+00000f60: 0a73 9a74 006a 01a0 027c 12a1 0190 0173  .s.t.j...|.....s
+00000f70: 0874 127c 0e7c 007c 017c 0a7c 0b7c 0d83  .t.|.|.|.|.|.|..
+00000f80: 067d 157c 156a 137d 1688 03a0 147c 16a1  .}.|.j.}.....|..
+00000f90: 0189 0764 037d 1488 03a0 157c 1688 07a1  ...d.}.....|....
+00000fa0: 027d 1774 167c 1264 0483 028f 2089 0288  .}.t.|.d.... ...
+00000fb0: 02a0 1774 0aa0 0b7c 17a1 01a1 0101 0057  ...t...|.......W
+00000fc0: 0064 0004 0004 0083 0301 006e 1031 0073  .d.........n.1.s
+00000fd0: fc30 0001 0001 0001 0059 0001 006e 3a74  .0.......Y...n:t
+00000fe0: 167c 1264 0583 028f 1e89 0274 0aa0 1888  .|.d.......t....
+00000ff0: 02a0 19a1 00a1 017d 1757 0064 0004 0004  .......}.W.d....
+00001000: 0083 0301 006e 1231 0090 0173 3830 0001  .....n.1...s80..
+00001010: 0001 0001 0059 0001 0074 1a7c 1783 017d  .....Y...t.|...}
+00001020: 1874 1b7c 187c 0683 025c 027d 197d 1a69  .t.|.|...\.}.}.i
+00001030: 007c 10a5 017c 007c 0e7c 0f88 047c 077c  .|...|.|.|...|.|
+00001040: 067c 1874 1a7c 1983 017c 1a7c 047c 0574  .|.t.|...|.|.|.t
+00001050: 1c64 069c 0ca5 017d 1b7c 0a90 0173 9674  .d.....}.|...s.t
+00001060: 006a 01a0 027c 13a1 0190 0173 c27c 0764  .j...|.....s.|.d
+00001070: 0075 0190 0172 c27c 0c90 0173 c274 1d6a  .u...r.|...s.t.j
+00001080: 1e64 077c 1a7c 0714 0064 089b 0464 099d  .d.|.|...d...d..
+00001090: 0364 0264 0a8d 0201 0074 167c 1364 0483  .d.d.....t.|.d..
+000010a0: 028f 2089 0288 02a0 1774 0aa0 0b7c 1ba1  .. ......t...|..
+000010b0: 01a1 0101 0057 0064 0004 0004 0083 0301  .....W.d........
+000010c0: 006e 1231 0090 0173 f430 0001 0001 0001  .n.1...s.0......
+000010d0: 0059 0001 0067 007d 1c67 007d 1d74 1f7c  .Y...g.}.g.}.t.|
+000010e0: 1a64 0b64 037c 0b64 0c8d 0490 028f 687d  .d.d.|.d......h}
+000010f0: 1e74 207c 067c 1983 0244 0090 025d 4a5c  .t |.|...D...]J\
+00001100: 025c 037d 1f7d 207d 217d 2274 006a 01a0  .\.}.} }!}"t.j..
+00001110: 0f7c 0174 217c 0e7c 117c 1f7c 207c 2183  .|.t!|.|.|.| |!.
+00001120: 05a1 027d 2374 006a 01a0 0f7c 0174 227c  ...}#t.j...|.t"|
+00001130: 0e7c 117c 1f7c 207c 217c 0583 06a1 027d  .|.|.| |!|.....}
+00001140: 247c 1ca0 237c 23a1 0101 007c 1da0 237c  $|..#|#....|..#|
+00001150: 24a1 0101 0074 006a 01a0 027c 23a1 0190  $....t.j...|#...
+00001160: 0272 e67c 0490 0272 a074 006a 01a0 027c  .r.|...r.t.j...|
+00001170: 24a1 0190 0272 e674 247c 2388 0483 027d  $....r.t$|#....}
+00001180: 257c 0490 0272 ba74 257c 2488 0483 027d  %|...r.t%|$....}
+00001190: 267c 0a90 0273 e67c 2574 1a7c 2283 016b  &|...s.|%t.|"..k
+000011a0: 0290 0272 e67c 0490 0272 247c 2674 1a7c  ...r.|...r$|&t.|
+000011b0: 2283 016b 0290 0272 e690 0271 247c 1490  "..k...r...q$|..
+000011c0: 0272 fe88 03a0 1474 267c 1783 01a1 0189  .r.....t&|......
+000011d0: 0764 037d 1464 0d89 007c 0a90 0373 2c74  .d.}.d...|...s,t
+000011e0: 006a 01a0 027c 23a1 0190 0372 2c74 277c  .j...|#....r,t'|
+000011f0: 2388 0474 1a7c 2283 0183 035c 0289 0189  #..t.|"....\....
+00001200: 006e 1c74 286a 2974 1a7c 2283 0188 0466  .n.t(j)t.|"....f
+00001210: 0274 286a 2a64 0e8d 0289 0164 0d89 0088  .t(j*d.....d....
+00001220: 007d 2764 0d7d 2867 0089 0564 0d89 0674  .}'d.}(g...d...t
+00001230: 167c 2364 0f83 028f e489 0287 0087 0187  .|#d............
+00001240: 0287 0387 0487 0587 0687 0766 0864 1064  ...........f.d.d
+00001250: 1184 087d 297c 2244 005d ae7d 207c 2064  ...})|"D.].} | d
+00001260: 1219 007c 2064 0d19 0018 007d 1f7c 287c  ...| d.....}.|(|
+00001270: 276b 0090 0372 b67c 2864 1237 007d 287c  'k...r.|(d.7.}(|
+00001280: 1ea0 2b7c 1fa1 0101 0090 0371 8274 267c  ..+|.......q.t&|
+00001290: 177c 2064 0d19 007c 2064 1219 0085 0219  .| d...| d......
+000012a0: 0083 017d 2a74 1a7c 2a83 0164 0d6b 0290  ...}*t.|*..d.k..
+000012b0: 0372 ea7c 1ea0 2b7c 1fa1 0101 0090 0371  .r.|..+|.......q
+000012c0: 8288 05a0 237c 20a1 0101 0088 067c 1f37  ....#| ......|.7
+000012d0: 0089 067c 0864 0075 0190 0472 1474 1a88  ...|.d.u...r.t..
+000012e0: 0583 017c 086b 0590 0473 1e88 067c 096b  ...|.k...s...|.k
+000012f0: 0590 0472 247c 2983 0001 007c 1ea0 2b7c  ...r$|)....|..+|
+00001300: 1fa1 0101 0090 0371 827c 2983 0001 0057  .......q.|)....W
+00001310: 0064 0004 0004 0083 0301 006e 1231 0090  .d.........n.1..
+00001320: 0473 4e30 0001 0001 0001 0059 0001 007c  .sN0.......Y...|
+00001330: 0490 0272 2474 2c7c 2488 0488 017c 0564  ...r$t,|$....|.d
+00001340: 138d 0401 0090 0271 2457 0064 0004 0004  .......q$W.d....
+00001350: 0083 0301 006e 1231 0090 0473 8830 0001  .....n.1...s.0..
+00001360: 0001 0001 0059 0001 0074 2d7c 007c 0e7c  .....Y...t-|.|.|
+00001370: 017c 0f7c 1b7c 1c7c 047c 1d7c 067c 197c  .|.|.|.|.|.|.|.|
+00001380: 1288 047c 0d64 148d 0d53 0029 154e 722e  ...|.d...S.).Nr.
+00001390: 0000 0054 46da 0177 722c 0000 0029 0c72  ...TF..wr,...).r
+000013a0: 2300 0000 7233 0000 0072 3c00 0000 7244  #...r3...r<...rD
+000013b0: 0000 00da 0e63 6f73 745f 7065 725f 746f  .....cost_per_to
+000013c0: 6b65 6e72 4100 0000 da0a 6e75 6d5f 746f  kenrA.....num_to
+000013d0: 6b65 6e73 724c 0000 00da 146e 756d 5f65  kensrL.....num_e
+000013e0: 6d62 6564 6469 6e67 5f74 6f6b 656e 7372  mbedding_tokensr
+000013f0: 3f00 0000 da0f 6e75 6d5f 616e 6e6f 795f  ?.....num_annoy_
+00001400: 7472 6565 735a 1073 656d 616e 7472 615f  treesZ.semantra_
+00001410: 7665 7273 696f 6e7a 1254 6f6b 656e 7320  versionz.Tokens 
+00001420: 7769 6c6c 2063 6f73 7420 247a 032e 3266  will cost $z..2f
+00001430: 7a0a 2e20 5072 6f63 6565 643f 2901 da05  z.. Proceed?)...
+00001440: 6162 6f72 747a 1643 616c 6375 6c61 7469  abortz.Calculati
+00001450: 6e67 2065 6d62 6564 6469 6e67 7329 04da  ng embeddings)..
+00001460: 0574 6f74 616c 5a04 6465 7363 5a05 6c65  .totalZ.descZ.le
+00001470: 6176 65da 0764 6973 6162 6c65 7201 0000  ave..disabler...
+00001480: 0029 015a 0564 7479 7065 5a02 6162 6300  .).Z.dtypeZ.abc.
+00001490: 0000 0000 0000 0000 0000 0002 0000 0006  ................
+000014a0: 0000 0013 0000 0073 6c00 0000 7400 8805  .......sl...t...
+000014b0: 8301 6401 6b04 7268 8803 a001 8807 8805  ..d.k.rh........
+000014c0: a102 7d00 7402 7c00 6402 8302 722a 7c00  ..}.t.|.d...r*|.
+000014d0: a003 a100 7d00 7c00 8801 8800 8800 7400  ....}.|.......t.
+000014e0: 8805 8301 1700 8502 3c00 7c00 4400 5d10  ........<.|.D.].
+000014f0: 7d01 7404 8802 7c01 8804 8303 0100 7142  }.t...|.......qB
+00001500: 8800 7400 8805 8301 3700 8900 6700 8905  ..t.....7...g...
+00001510: 6401 8906 6400 5300 2903 4e72 0100 0000  d...d.S.).Nr....
+00001520: da03 6370 7529 0572 4b00 0000 5a05 656d  ..cpu).rK...Z.em
+00001530: 6265 64da 0768 6173 6174 7472 725a 0000  bed..hasattrrZ..
+00001540: 0072 1e00 0000 2902 5a11 656d 6265 6464  .r....).Z.embedd
+00001550: 696e 675f 7265 7375 6c74 73da 0965 6d62  ing_results..emb
+00001560: 6564 6469 6e67 a908 5a0f 656d 6265 6464  edding..Z.embedd
+00001570: 696e 675f 696e 6465 7872 5000 0000 7237  ing_indexrP...r7
+00001580: 0000 00da 056d 6f64 656c 7244 0000 005a  .....modelrD...Z
+00001590: 0470 6f6f 6c5a 1070 6f6f 6c5f 746f 6b65  .poolZ.pool_toke
+000015a0: 6e5f 636f 756e 74da 0674 6f6b 656e 7372  n_count..tokensr
+000015b0: 2600 0000 7227 0000 00da 0a66 6c75 7368  &...r'.....flush
+000015c0: 5f70 6f6f 6c0c 0100 0073 1a00 0000 0003  _pool....s......
+000015d0: 0c01 0c02 0a01 0803 02fe 0201 0eff 0203  ................
+000015e0: 0801 0e01 0c01 0401 7a1b 7072 6f63 6573  ........z.proces
+000015f0: 732e 3c6c 6f63 616c 733e 2e66 6c75 7368  s.<locals>.flush
+00001600: 5f70 6f6f 6c72 0a00 0000 2904 7223 0000  _poolr....).r#..
+00001610: 0072 4400 0000 7250 0000 005a 096e 756d  .rD...rP...Z.num
+00001620: 5f74 7265 6573 723b 0000 0029 2eda 026f  _treesr;...)...o
+00001630: 73da 0470 6174 68da 0665 7869 7374 73da  s..path..exists.
+00001640: 086d 616b 6564 6972 7372 1100 0000 da08  .makedirsr......
+00001650: 6261 7365 6e61 6d65 5a0a 6765 745f 636f  basenameZ.get_co
+00001660: 6e66 6967 da10 4445 4641 554c 545f 454e  nfig..DEFAULT_EN
+00001670: 434f 4449 4e47 da07 6861 7368 6c69 625a  CODING..hashlibZ
+00001680: 0973 6861 6b65 5f32 3536 7247 0000 00da  .shake_256rG....
+00001690: 0564 756d 7073 da06 656e 636f 6465 5a09  .dumps..encodeZ.
+000016a0: 6865 7864 6967 6573 7472 1000 0000 da04  hexdigestr......
+000016b0: 6a6f 696e 7218 0000 0072 1300 0000 7238  joinr....r....r8
+000016c0: 0000 0072 2200 0000 5a0a 6765 745f 746f  ...r"...Z.get_to
+000016d0: 6b65 6e73 5a0f 6765 745f 7465 7874 5f63  kensZ.get_text_c
+000016e0: 6875 6e6b 7372 3100 0000 da05 7772 6974  hunksr1.....writ
+000016f0: 6572 4800 0000 7232 0000 0072 4b00 0000  erH...r2...rK...
+00001700: 7217 0000 00da 0756 4552 5349 4f4e da05  r......VERSION..
+00001710: 636c 6963 6b5a 0763 6f6e 6669 726d 7209  clickZ.confirmr.
+00001720: 0000 00da 037a 6970 7214 0000 0072 1200  .....zipr....r..
+00001730: 0000 da06 6170 7065 6e64 7216 0000 0072  ....appendr....r
+00001740: 1500 0000 7219 0000 0072 1b00 0000 da02  ....r....r......
+00001750: 6e70 da05 656d 7074 795a 0766 6c6f 6174  np..emptyZ.float
+00001760: 3332 da06 7570 6461 7465 721d 0000 0072  32..updater....r
+00001770: 3900 0000 292b 7223 0000 0072 3400 0000  9...)+r#...r4...
+00001780: 725e 0000 0072 4400 0000 723f 0000 0072  r^...rD...r?...r
+00001790: 5600 0000 7241 0000 0072 5300 0000 da0a  V...rA...rS.....
+000017a0: 706f 6f6c 5f63 6f75 6e74 da09 706f 6f6c  pool_count..pool
+000017b0: 5f73 697a 6572 3500 0000 7236 0000 00da  _sizer5...r6....
+000017c0: 0a6e 6f5f 636f 6e66 6972 6d72 2e00 0000  .no_confirmr....
+000017d0: 7233 0000 0072 3c00 0000 723d 0000 005a  r3...r<...r=...Z
+000017e0: 0b63 6f6e 6669 675f 6861 7368 7243 0000  .config_hashrC..
+000017f0: 005a 0f63 6f6e 6669 675f 6669 6c65 6e61  .Z.config_filena
+00001800: 6d65 5a17 7368 6f75 6c64 5f63 616c 6375  meZ.should_calcu
+00001810: 6c61 7465 5f74 6f6b 656e 7372 4600 0000  late_tokensrF...
+00001820: 7221 0000 0072 4900 0000 7254 0000 0072  r!...rI...rT...r
+00001830: 4200 0000 7255 0000 005a 0b66 756c 6c5f  B...rU...Z.full_
+00001840: 636f 6e66 6967 723e 0000 0072 4000 0000  configr>...r@...
+00001850: da04 7062 6172 da04 7369 7a65 da06 6f66  ..pbar..size..of
+00001860: 6673 6574 da06 7265 7769 6e64 5a0b 7375  fset..rewindZ.su
+00001870: 625f 6f66 6673 6574 735a 1365 6d62 6564  b_offsetsZ.embed
+00001880: 6469 6e67 735f 6669 6c65 6e61 6d65 5a0e  dings_filenameZ.
+00001890: 616e 6e6f 795f 6669 6c65 6e61 6d65 724c  annoy_filenamerL
+000018a0: 0000 005a 146e 756d 5f61 6e6e 6f79 5f65  ...Z.num_annoy_e
+000018b0: 6d62 6564 6469 6e67 735a 086e 756d 5f73  mbeddingsZ.num_s
+000018c0: 6b69 705a 0969 7465 7261 7469 6f6e 7260  kipZ.iterationr`
+000018d0: 0000 005a 0b77 696e 646f 775f 7465 7874  ...Z.window_text
+000018e0: 7226 0000 0072 5d00 0000 7227 0000 00da  r&...r]...r'....
+000018f0: 0770 726f 6365 7373 7b00 0000 7330 0100  .process{...s0..
+00001900: 0000 110c 010a 0308 010c 0108 0108 0108  ................
+00001910: 011a 0314 0114 0204 0112 0212 0106 010a  ................
+00001920: 0104 010c 010c 0130 020c 012e 0108 0608  .......0........
+00001930: fd02 0102 0102 0402 0102 ff02 0202 0102  ................
+00001940: 0102 0102 0102 0102 0102 0106 0102 0102  ................
+00001950: 0102 0102 f308 1014 0110 0104 0110 0102  ................
+00001960: fe06 060c 0130 0204 0104 0102 0102 0102  .....0..........
+00001970: 0102 0102 fc08 0502 011a 0106 0102 010e  ................
+00001980: fe04 0406 0102 0102 010c ff02 fe04 060a  ................
+00001990: 010a 020e 0102 ff04 010a ff04 030a 0106  ................
+000019a0: 0102 0104 ff04 0502 ff04 020a fe04 0302  ................
+000019b0: fd04 030a fd04 0604 0206 010e 0104 0304  ................
+000019c0: 0114 0102 010a ff0a 0404 010e ff06 0304  ................
+000019d0: 0204 0104 0304 0104 020c 021a 1108 0110  ................
+000019e0: 030a 0108 010a 0104 0218 010e 010a 0104  ................
+000019f0: 020a 0108 0206 ff04 010a ff04 0206 fe04  ................
+00001a00: 0306 010e 0226 0306 0102 0102 0102 0102  .....&..........
+00001a10: 0102 fc2a 0702 0102 0102 0102 0102 0102  ...*............
+00001a20: 0102 0102 0102 0102 0102 0102 0102 0102  ................
+00001a30: f372 7a00 0000 7a1a 6c69 7374 5b74 7570  .rz...z.list[tup
+00001a40: 6c65 5b69 6e74 2c20 696e 742c 2069 6e74  le[int, int, int
+00001a50: 5d5d 2902 7241 0000 00da 0672 6574 7572  ]]).rA.....retur
+00001a60: 6e63 0100 0000 0000 0000 0000 0000 0500  nc..............
+00001a70: 0000 0500 0000 6300 0000 7378 0000 007c  ......c...sx...|
+00001a80: 00a0 0064 01a1 0144 005d 687d 0164 027c  ...d...D.]h}.d.|
+00001a90: 0176 0072 627c 01a0 0164 02a1 0164 036b  .v.rb|...d...d.k
+00001aa0: 0272 387c 01a0 0064 02a1 015c 027d 027d  .r8|...d...\.}.}
+00001ab0: 0364 047d 046e 107c 01a0 0064 02a1 015c  .d.}.n.|...d...\
+00001ac0: 037d 027d 037d 0474 027c 0283 0174 027c  .}.}.}.t.|...t.|
+00001ad0: 0383 0174 027c 0483 0166 0356 0001 0071  ...t.|...f.V...q
+00001ae0: 0a74 027c 0183 0164 0464 0466 0356 0001  .t.|...d.d.f.V..
+00001af0: 0071 0a64 0053 0029 054e fa01 2cda 015f  .q.d.S.).N..,.._
+00001b00: 720a 0000 0072 0100 0000 2903 da05 7370  r....r....)...sp
+00001b10: 6c69 74da 0563 6f75 6e74 da03 696e 7429  lit..count..int)
+00001b20: 0572 4100 0000 5a06 7769 6e64 6f77 7277  .rA...Z.windowrw
+00001b30: 0000 0072 7800 0000 7279 0000 0072 2600  ...rx...ry...r&.
+00001b40: 0000 7226 0000 0072 2700 0000 da0f 7072  ..r&...r'.....pr
+00001b50: 6f63 6573 735f 7769 6e64 6f77 734f 0100  ocess_windowsO..
+00001b60: 0073 1000 0000 0001 0e01 0802 0e01 0e01  .s..............
+00001b70: 0602 1001 1a02 7281 0000 0072 2300 0000  ......r....r#...
+00001b80: 5429 0172 6300 0000 e9ff ffff ff29 02da  T).rc........)..
+00001b90: 0474 7970 655a 056e 6172 6773 7a07 2d2d  .typeZ.nargsz.--
+00001ba0: 6d6f 6465 6c29 015a 0e63 6173 655f 7365  model).Z.case_se
+00001bb0: 6e73 6974 6976 655a 056d 706e 6574 7a21  nsitiveZ.mpnetz!
+00001bc0: 5072 6573 6574 206d 6f64 656c 2074 6f20  Preset model to 
+00001bd0: 7573 6520 666f 7220 656d 6265 6464 696e  use for embeddin
+00001be0: 6729 0472 8300 0000 da07 6465 6661 756c  g).r......defaul
+00001bf0: 74da 0c73 686f 775f 6465 6661 756c 74da  t..show_default.
+00001c00: 0468 656c 707a 0a2d 2d65 6e63 6f64 696e  .helpz.--encodin
+00001c10: 677a 2645 6e63 6f64 696e 6720 746f 2075  gz&Encoding to u
+00001c20: 7365 2066 6f72 2072 6561 6469 6e67 2074  se for reading t
+00001c30: 6578 7420 6669 6c65 737a 132d 2d74 7261  ext filesz.--tra
+00001c40: 6e73 666f 726d 6572 2d6d 6f64 656c 7a3f  nsformer-modelz?
+00001c50: 4375 7374 6f6d 2048 7567 6769 6e67 6661  Custom Huggingfa
+00001c60: 6365 2074 7261 6e73 666f 726d 6572 7320  ce transformers 
+00001c70: 6d6f 6465 6c20 6e61 6d65 2074 6f20 7573  model name to us
+00001c80: 6520 666f 7220 656d 6265 6464 696e 6729  e for embedding)
+00001c90: 0272 8300 0000 7286 0000 007a 092d 2d77  .r....r....z.--w
+00001ca0: 696e 646f 7773 5a08 3132 385f 305f 3136  indowsZ.128_0_16
+00001cb0: 6116 0100 0045 6d62 6564 6469 6e67 2077  a....Embedding w
+00001cc0: 696e 646f 7773 2074 6f20 6578 7472 6163  indows to extrac
+00001cd0: 742e 2041 2063 6f6d 6d61 2d73 6570 6172  t. A comma-separ
+00001ce0: 6174 6564 206c 6973 7420 6f66 2074 6865  ated list of the
+00001cf0: 2066 6f72 6d61 7420 2273 697a 655b 5f6f   format "size[_o
+00001d00: 6666 7365 743d 305d 5b5f 7265 7769 6e64  ffset=0][_rewind
+00001d10: 3d30 5d2e 2041 2077 696e 646f 7720 7769  =0]. A window wi
+00001d20: 7468 2073 697a 6520 3132 382c 206f 6666  th size 128, off
+00001d30: 7365 7420 302c 2061 6e64 2072 6577 696e  set 0, and rewin
+00001d40: 6420 6f66 2031 3620 2831 3238 5f30 5f31  d of 16 (128_0_1
+00001d50: 3629 2077 696c 6c20 656d 6265 6420 7468  6) will embed th
+00001d60: 6520 646f 6375 6d65 6e74 2069 6e20 6368  e document in ch
+00001d70: 756e 6b73 206f 6620 3132 3820 746f 6b65  unks of 128 toke
+00001d80: 6e73 2077 6869 6368 2070 6172 7469 616c  ns which partial
+00001d90: 6c79 206f 7665 726c 6170 2062 7920 3136  ly overlap by 16
+00001da0: 2e20 4f6e 6c79 2074 6865 2066 6972 7374  . Only the first
+00001db0: 2077 696e 646f 7720 6973 2075 7365 6420   window is used 
+00001dc0: 666f 7220 7365 6172 6368 2e7a 0b2d 2d6e  for search.z.--n
+00001dd0: 6f2d 7365 7276 6572 467a 2944 6f20 6e6f  o-serverFz)Do no
+00001de0: 7420 7374 6172 7420 7468 6520 5549 2073  t start the UI s
+00001df0: 6572 7665 7220 286f 6e6c 7920 7072 6f63  erver (only proc
+00001e00: 6573 7329 2904 da07 6973 5f66 6c61 6772  ess))...is_flagr
+00001e10: 8400 0000 7285 0000 0072 8600 0000 7a06  ....r....r....z.
+00001e20: 2d2d 706f 7274 7a20 506f 7274 2074 6f20  --portz Port to 
+00001e30: 7573 6520 666f 7220 656d 6265 6464 696e  use for embeddin
+00001e40: 6720 7365 7276 6572 7a06 2d2d 686f 7374  g serverz.--host
+00001e50: 7a07 302e 302e 302e 307a 2048 6f73 7420  z.0.0.0.0z Host 
+00001e60: 746f 2075 7365 2066 6f72 2065 6d62 6564  to use for embed
+00001e70: 6469 6e67 2073 6572 7665 727a 0b2d 2d70  ding serverz.--p
+00001e80: 6f6f 6c2d 7369 7a65 7a3b 4d61 7820 6e75  ool-sizez;Max nu
+00001e90: 6d62 6572 206f 6620 656d 6265 6464 696e  mber of embeddin
+00001ea0: 6720 746f 6b65 6e73 2074 6f20 706f 6f6c  g tokens to pool
+00001eb0: 2074 6f67 6574 6865 7220 696e 2072 6571   together in req
+00001ec0: 7565 7374 7329 0372 8300 0000 7284 0000  uests).r....r...
+00001ed0: 0072 8600 0000 7a0c 2d2d 706f 6f6c 2d63  .r....z.--pool-c
+00001ee0: 6f75 6e74 7a35 4d61 7820 6e75 6d62 6572  ountz5Max number
+00001ef0: 206f 6620 656d 6265 6464 696e 6773 2074   of embeddings t
+00001f00: 6f20 706f 6f6c 2074 6f67 6574 6865 7220  o pool together 
+00001f10: 696e 2072 6571 7565 7374 737a 0f2d 2d64  in requestsz.--d
+00001f20: 6f63 2d74 6f6b 656e 2d70 7265 7a47 546f  oc-token-prezGTo
+00001f30: 6b65 6e20 746f 2070 7265 7065 6e64 2074  ken to prepend t
+00001f40: 6f20 6561 6368 2064 6f63 756d 656e 7420  o each document 
+00001f50: 696e 2074 7261 6e73 666f 726d 6572 206d  in transformer m
+00001f60: 6f64 656c 7320 2864 6566 6175 6c74 3a20  odels (default: 
+00001f70: 4e6f 6e65 297a 102d 2d64 6f63 2d74 6f6b  None)z.--doc-tok
+00001f80: 656e 2d70 6f73 747a 4654 6f6b 656e 2074  en-postzFToken t
+00001f90: 6f20 6170 7065 6e64 2074 6f20 6561 6368  o append to each
+00001fa0: 2064 6f63 756d 656e 7420 696e 2074 7261   document in tra
 00001fb0: 6e73 666f 726d 6572 206d 6f64 656c 7320  nsformer models 
 00001fc0: 2864 6566 6175 6c74 3a20 4e6f 6e65 297a  (default: None)z
-00001fd0: 0d2d 2d6e 756d 2d72 6573 756c 7473 e90a  .--num-results..
-00001fe0: 0000 007a 3e4e 756d 6265 7220 6f66 2072  ...z>Number of r
-00001ff0: 6573 756c 7473 2028 6e65 6967 6862 6f72  esults (neighbor
-00002000: 7329 2074 6f20 7265 7472 6965 7665 2070  s) to retrieve p
-00002010: 6572 2066 696c 6520 666f 7220 7175 6572  er file for quer
-00002020: 6965 737a 072d 2d61 6e6e 6f79 7a7c 5573  iesz.--annoyz|Us
-00002030: 6520 6170 7072 6f78 696d 6174 6520 6b4e  e approximate kN
-00002040: 4e20 7669 6120 416e 6e6f 7920 666f 7220  N via Annoy for 
-00002050: 7175 6572 6965 7320 2866 6173 7465 7220  queries (faster 
-00002060: 7175 6572 7969 6e67 2061 7420 6120 736c  querying at a sl
-00002070: 6967 6874 2063 6f73 7420 6f66 2061 6363  ight cost of acc
-00002080: 7572 6163 7929 3b20 6966 2066 616c 7365  uracy); if false
-00002090: 2c20 7573 6520 6578 6163 7420 6578 6861  , use exact exha
-000020a0: 7573 7469 7665 206b 4e4e 7a11 2d2d 6e75  ustive kNNz.--nu
-000020b0: 6d2d 616e 6e6f 792d 7472 6565 73e9 6400  m-annoy-trees.d.
-000020c0: 0000 7a34 4e75 6d62 6572 206f 6620 7472  ..z4Number of tr
-000020d0: 6565 7320 746f 2075 7365 2066 6f72 2061  ees to use for a
-000020e0: 7070 726f 7869 6d61 7465 206b 4e4e 2076  pproximate kNN v
-000020f0: 6961 2041 6e6e 6f79 7a05 2d2d 7376 6d7a  ia Annoyz.--svmz
-00002100: 5a55 7365 2053 564d 2069 6e73 7465 6164  ZUse SVM instead
-00002110: 206f 6620 616e 7920 6b69 6e64 206f 6620   of any kind of 
-00002120: 6b4e 4e20 666f 7220 7175 6572 6965 7320  kNN for queries 
-00002130: 2873 6c6f 7765 7220 616e 6420 6f6e 6c79  (slower and only
-00002140: 2077 6f72 6b73 206f 6e20 7379 6d6d 6574   works on symmet
-00002150: 7269 6320 6d6f 6465 6c73 297a 072d 2d73  ric models)z.--s
-00002160: 766d 2d63 e700 0000 0000 00f0 3f7a 4853  vm-c........?zHS
-00002170: 564d 2072 6567 756c 6172 697a 6174 696f  VM regularizatio
-00002180: 6e20 7061 7261 6d65 7465 723b 2068 6967  n parameter; hig
-00002190: 6865 7220 7661 6c75 6573 2070 656e 616c  her values penal
-000021a0: 697a 6520 6d69 7370 7265 6469 6374 696f  ize mispredictio
-000021b0: 6e73 206d 6f72 657a 152d 2d65 7870 6c61  ns morez.--expla
-000021c0: 696e 2d73 706c 6974 2d63 6f75 6e74 e909  in-split-count..
-000021d0: 0000 007a 404e 756d 6265 7220 6f66 2073  ...z@Number of s
-000021e0: 706c 6974 7320 6f6e 2061 2067 6976 656e  plits on a given
-000021f0: 2077 696e 646f 7720 746f 2075 7365 2066   window to use f
-00002200: 6f72 2065 7870 6c61 696e 696e 6720 6120  or explaining a 
-00002210: 7175 6572 797a 162d 2d65 7870 6c61 696e  queryz.--explain
-00002220: 2d73 706c 6974 2d64 6976 6964 65e9 0600  -split-divide...
-00002230: 0000 7a53 4661 6374 6f72 2074 6f20 6469  ..zSFactor to di
-00002240: 7669 6465 2074 6865 2077 696e 646f 7720  vide the window 
-00002250: 7369 7a65 2062 7920 746f 2067 6574 2065  size by to get e
-00002260: 6163 6820 7370 6c69 7420 6c65 6e67 7468  ach split length
-00002270: 2066 6f72 2065 7870 6c61 696e 696e 6720   for explaining 
-00002280: 6120 7175 6572 797a 182d 2d6e 756d 2d65  a queryz.--num-e
-00002290: 7870 6c61 696e 2d68 6967 686c 6967 6874  xplain-highlight
-000022a0: 73e9 0200 0000 7a3b 4e75 6d62 6572 206f  s.....z;Number o
-000022b0: 6620 7370 6c69 7420 7265 7375 6c74 7320  f split results 
-000022c0: 746f 2068 6967 686c 6967 6874 2066 6f72  to highlight for
-000022d0: 2065 7870 6c61 696e 696e 6720 6120 7175   explaining a qu
-000022e0: 6572 797a 072d 2d66 6f72 6365 7a1c 466f  eryz.--forcez.Fo
-000022f0: 7263 6520 7072 6f63 6573 7320 6576 656e  rce process even
-00002300: 2069 6620 6361 6368 6564 2903 728a 0000   if cached).r...
-00002310: 0072 8600 0000 7288 0000 007a 082d 2d73  .r....r....z.--s
-00002320: 696c 656e 747a 2144 6f20 6e6f 7420 7072  ilentz!Do not pr
-00002330: 696e 7420 7072 6f67 7265 7373 2069 6e66  int progress inf
-00002340: 6f72 6d61 7469 6f6e 7a0c 2d2d 6e6f 2d63  ormationz.--no-c
-00002350: 6f6e 6669 726d 7a47 446f 206e 6f74 2073  onfirmzGDo not s
-00002360: 686f 7720 636f 7374 2061 6e64 2061 736b  how cost and ask
-00002370: 2066 6f72 2063 6f6e 6669 726d 6174 696f   for confirmatio
-00002380: 6e20 6265 666f 7265 2070 726f 6365 7373  n before process
-00002390: 696e 6720 7769 7468 204f 7065 6e41 497a  ing with OpenAIz
-000023a0: 092d 2d76 6572 7369 6f6e 7a16 5072 696e  .--versionz.Prin
-000023b0: 7420 7665 7273 696f 6e20 616e 6420 6578  t version and ex
-000023c0: 6974 7a0d 2d2d 6c69 7374 2d6d 6f64 656c  itz.--list-model
-000023d0: 737a 1b4c 6973 7420 7072 6573 6574 206d  sz.List preset m
-000023e0: 6f64 656c 7320 616e 6420 6578 6974 7a13  odels and exitz.
-000023f0: 2d2d 7368 6f77 2d73 656d 616e 7472 612d  --show-semantra-
-00002400: 6469 727a 4750 7269 6e74 2074 6865 2064  dirzGPrint the d
-00002410: 6972 6563 746f 7279 2073 656d 616e 7472  irectory semantr
-00002420: 6120 7769 6c6c 2075 7365 2074 6f20 7374  a will use to st
-00002430: 6f72 6520 7072 6f63 6573 7365 6420 6669  ore processed fi
-00002440: 6c65 7320 616e 6420 6578 6974 7a0e 2d2d  les and exitz.--
-00002450: 7365 6d61 6e74 7261 2d64 6972 7a24 4469  semantra-dirz$Di
-00002460: 7265 6374 6f72 7920 746f 2073 746f 7265  rectory to store
-00002470: 2073 656d 616e 7472 6120 6669 6c65 7320   semantra files 
-00002480: 696e 631c 0000 0000 0000 0000 0000 002d  inc............-
-00002490: 0000 0010 0000 0003 0000 0073 e602 0000  ...........s....
-000024a0: 7c18 7210 7400 7401 8301 0100 6400 5300  |.r.t.t.....d.S.
-000024b0: 7c19 7230 7402 4400 5d12 7d1c 7400 6401  |.r0t.D.].}.t.d.
-000024c0: 7c1c 9b00 9d02 8301 0100 7118 6400 5300  |.........q.d.S.
-000024d0: 7c1b 6400 7500 7242 7403 a004 6402 a101  |.d.u.rBt...d...
-000024e0: 7d1b 7c1a 7252 7400 7c1b 8301 0100 6400  }.|.rRt.|.....d.
-000024f0: 5300 7c00 6400 7500 7366 7405 7c00 8301  S.|.d.u.sft.|...
-00002500: 6403 6b02 7270 7403 a006 6404 a101 8201  d.k.rpt...d.....
-00002510: 7407 7408 7c01 8301 8301 7d1d 7c0c 6400  t.t.|.....}.|.d.
-00002520: 7501 72a8 7c05 6400 7500 7290 7409 7d05  u.r.|.d.u.r.t.}.
-00002530: 6400 7d1e 740a 7c0c 7c07 7c08 7c09 7c0a  d.}.t.|.|.|.|.|.
-00002540: 6405 8d05 8907 6e3e 7402 8807 1900 7d1f  d.....n>t.....}.
-00002550: 7c1f 6406 1900 7d1e 7c05 6400 7500 72c8  |.d...}.|.d.u.r.
-00002560: 7c1f 6407 1900 7d05 7c06 6400 7500 72dc  |.d...}.|.d.u.r.
-00002570: 7c1f a00b 6408 6400 a102 7d06 7c1f 6409  |...d.d...}.|.d.
-00002580: 1900 8300 8907 880c 72fa 8807 a00c a100  ........r.......
-00002590: 72fa 740d 640a 8301 8201 6900 8903 740e  r.t.d.....i...t.
-000025a0: 7c00 7c16 640b 8d02 7d20 7c20 4400 5d44  |.|.d...} | D.]D
-000025b0: 7d21 7c20 a00f 7410 6a11 a012 7c21 a101  }!| ..t.j...|!..
-000025c0: 9b00 a101 0100 7413 7c21 7c1b 8807 8807  ......t.|!|.....
-000025d0: a014 a100 8800 7c0d 7c1d 7c1e 7c06 7c05  ......|.|.|.|.|.
-000025e0: 7c15 7c16 7c17 640c 8d0d 8803 7c21 3c00  |.|.|.d.....|!<.
-000025f0: 9001 710e 6400 8901 6400 8902 8701 8702  ..q.d...d.......
-00002600: 8703 6603 640d 640e 8408 8906 7415 7416  ..f.d.d.....t.t.
-00002610: 8301 7d22 7c22 a017 640f a101 6410 6411  ..}"|"..d...d.d.
-00002620: 8400 8301 7d23 7c22 a017 6412 a101 6413  ....}#|"..d...d.
-00002630: 6414 8400 8301 7d24 7c22 6a17 6415 6416  d.....}$|"j.d.d.
-00002640: 6701 6417 8d02 8703 6601 6418 6419 8408  g.d.....f.d.d...
-00002650: 8301 7d25 7c22 6a17 641a 641b 6701 6417  ..}%|"j.d.d.g.d.
-00002660: 8d02 8700 8703 8707 8709 870a 870b 870c  ................
-00002670: 6607 641c 641d 8408 8301 7d26 7c22 6a17  f.d.d.....}&|"j.
-00002680: 641e 641b 6701 6417 8d02 8703 8707 8709  d.d.g.d.........
-00002690: 870d 6604 641f 6420 8408 8301 890b 7c22  ..f.d.d ......|"
-000026a0: 6a17 6421 641b 6701 6417 8d02 8703 8707  j.d!d.g.d.......
-000026b0: 8709 6603 6422 6423 8408 8301 890a 7c22  ..f.d"d#......|"
-000026c0: 6a17 6424 641b 6701 6417 8d02 8703 8704  j.d$d.g.d.......
-000026d0: 8705 8707 8708 6605 6425 6426 8408 8301  ......f.d%d&....
-000026e0: 7d27 7c22 6a17 6427 6416 6701 6417 8d02  }'|"j.d'd.g.d...
-000026f0: 8706 6601 6428 6429 8408 8301 7d28 7c22  ..f.d(d)....}(|"
-00002700: 6a17 642a 6416 6701 6417 8d02 8706 6601  j.d*d.g.d.....f.
-00002710: 642b 642c 8408 8301 7d29 7c22 6a17 642d  d+d,....})|"j.d-
-00002720: 6416 6701 6417 8d02 8706 6601 642e 642f  d.g.d.....f.d.d/
-00002730: 8408 8301 7d2a 7c22 6a17 6430 6416 6701  ....}*|"j.d0d.g.
-00002740: 6417 8d02 8706 6601 6431 6432 8408 8301  d.....f.d1d2....
-00002750: 7d2b 7c22 6a17 6433 6416 6701 6417 8d02  }+|"j.d3d.g.d...
-00002760: 8703 6601 6434 6435 8408 8301 7d2c 7c02  ..f.d4d5....},|.
-00002770: 9002 73e2 7c22 6a18 7c04 7c03 6436 8d02  ..s.|"j.|.|.d6..
-00002780: 0100 6400 5300 2937 4e7a 022d 205a 0853  ..d.S.)7Nz.- Z.S
-00002790: 656d 616e 7472 6172 0100 0000 7a28 4d75  emantrar....z(Mu
-000027a0: 7374 2070 726f 7669 6465 2061 2066 696c  st provide a fil
-000027b0: 656e 616d 6520 746f 2070 726f 6365 7373  ename to process
-000027c0: 2f71 7565 7279 2904 da0d 646f 635f 746f  /query)...doc_to
-000027d0: 6b65 6e5f 7072 65da 0e64 6f63 5f74 6f6b  ken_pre..doc_tok
-000027e0: 656e 5f70 6f73 74da 0f71 7565 7279 5f74  en_post..query_t
-000027f0: 6f6b 656e 5f70 7265 da10 7175 6572 795f  oken_pre..query_
-00002800: 746f 6b65 6e5f 706f 7374 7252 0000 0072  token_postrR...r
-00002810: 7300 0000 7272 0000 005a 0967 6574 5f6d  s...rr...Z.get_m
-00002820: 6f64 656c 7a52 5356 4d20 6973 206e 6f74  odelzRSVM is not
-00002830: 2063 6f6d 7061 7469 626c 6520 7769 7468   compatible with
-00002840: 2061 7379 6d6d 6574 7269 6320 6d6f 6465   asymmetric mode
-00002850: 6c73 2e20 506c 6561 7365 2075 7365 2061  ls. Please use a
-00002860: 2073 796d 6d65 7472 6963 206d 6f64 656c   symmetric model
-00002870: 206f 7220 6b4e 4e2e 2901 7258 0000 0029   or kNN.).rX...)
-00002880: 0d72 2300 0000 7233 0000 0072 5e00 0000  .r#...r3...r^...
-00002890: 7243 0000 0072 3e00 0000 7255 0000 0072  rC...r>...rU...r
-000028a0: 4000 0000 7252 0000 0072 7200 0000 7273  @...rR...rr...rs
-000028b0: 0000 0072 3400 0000 7235 0000 0072 7400  ...r4...r5...rt.
-000028c0: 0000 6301 0000 0000 0000 0000 0000 0002  ..c.............
-000028d0: 0000 0002 0000 0013 0000 0073 2200 0000  ...........s"...
-000028e0: 7c00 8801 6b02 720c 8800 5300 8802 7c00  |...k.r...S...|.
-000028f0: 1900 6a00 7d01 7c00 8901 7c01 8900 7c01  ..j.}.|...|...|.
-00002900: 5300 7239 0000 0029 0172 4500 0000 a902  S.r9...).rE.....
-00002910: 7223 0000 0072 4500 0000 2903 da0e 6361  r#...rE...)...ca
-00002920: 6368 6564 5f63 6f6e 7465 6e74 da17 6361  ched_content..ca
-00002930: 6368 6564 5f63 6f6e 7465 6e74 5f66 696c  ched_content_fil
-00002940: 656e 616d 65da 0964 6f63 756d 656e 7473  ename..documents
-00002950: 7226 0000 0072 2700 0000 da0b 6765 745f  r&...r'.....get_
-00002960: 636f 6e74 656e 7468 0200 0073 0c00 0000  contenth...s....
-00002970: 0003 0801 0402 0a02 0401 0402 7a19 6d61  ............z.ma
-00002980: 696e 2e3c 6c6f 6361 6c73 3e2e 6765 745f  in.<locals>.get_
-00002990: 636f 6e74 656e 74fa 012f 6300 0000 0000  content../c.....
-000029a0: 0000 0000 0000 0000 0000 0005 0000 0053  ...............S
-000029b0: 0000 0073 1200 0000 7400 7401 a002 6401  ...s....t.t...d.
-000029c0: 6402 a102 6403 8302 5300 2904 4e72 1e00  d...d...S.).Nr..
-000029d0: 0000 fa13 2e2e 2f2e 2e2f 636c 6965 6e74  ....../../client
-000029e0: 2f70 7562 6c69 637a 0a69 6e64 6578 2e68  /publicz.index.h
-000029f0: 746d 6ca9 0372 0600 0000 da0d 706b 675f  tml..r......pkg_
-00002a00: 7265 736f 7572 6365 73da 1172 6573 6f75  resources..resou
-00002a10: 7263 655f 6669 6c65 6e61 6d65 7226 0000  rce_filenamer&..
-00002a20: 0072 2600 0000 7226 0000 0072 2700 0000  .r&...r&...r'...
-00002a30: da04 6261 7365 7802 0000 7308 0000 0000  ..basex...s.....
-00002a40: 0202 010a 0102 fe7a 126d 6169 6e2e 3c6c  .......z.main.<l
-00002a50: 6f63 616c 733e 2e62 6173 657a 0c2f 3c70  ocals>.basez./<p
-00002a60: 6174 683a 7061 7468 3e63 0100 0000 0000  ath:path>c......
-00002a70: 0000 0000 0000 0100 0000 0500 0000 5300  ..............S.
-00002a80: 0000 7312 0000 0074 0074 01a0 0264 0164  ..s....t.t...d.d
-00002a90: 02a1 027c 0083 0253 0029 034e 721e 0000  ...|...S.).Nr...
-00002aa0: 0072 9d00 0000 729e 0000 0029 0172 6200  .r....r....).rb.
-00002ab0: 0000 7226 0000 0072 2600 0000 7227 0000  ..r&...r&...r'..
-00002ac0: 00da 0468 6f6d 6580 0200 0073 0800 0000  ...home....s....
-00002ad0: 0002 0201 0a01 02fe 7a12 6d61 696e 2e3c  ........z.main.<
-00002ae0: 6c6f 6361 6c73 3e2e 686f 6d65 7a0a 2f61  locals>.homez./a
-00002af0: 7069 2f66 696c 6573 5a03 4745 5429 01da  pi/filesZ.GET)..
-00002b00: 076d 6574 686f 6473 6300 0000 0000 0000  .methodsc.......
-00002b10: 0000 0000 0000 0000 0004 0000 0013 0000  ................
-00002b20: 0073 1600 0000 7400 6401 6402 8400 8800  .s....t.d.d.....
-00002b30: a001 a100 4400 8301 8301 5300 2903 4e63  ....D.....S.).Nc
-00002b40: 0100 0000 0000 0000 0000 0000 0200 0000  ................
-00002b50: 0600 0000 5300 0000 7320 0000 0067 007c  ....S...s ...g.|
-00002b60: 005d 187d 017c 016a 007c 016a 017c 016a  .].}.|.j.|.j.|.j
-00002b70: 026a 0364 009c 0391 0271 0453 0029 0129  .j.d.....q.S.).)
-00002b80: 0372 6500 0000 7223 0000 0072 2400 0000  .re...r#...r$...
-00002b90: 2904 723b 0000 0072 2300 0000 7245 0000  ).r;...r#...rE..
-00002ba0: 0072 2400 0000 2902 da02 2e30 da03 646f  .r$...)....0..do
-00002bb0: 6372 2600 0000 7226 0000 0072 2700 0000  cr&...r&...r'...
-00002bc0: da0a 3c6c 6973 7463 6f6d 703e 8a02 0000  ..<listcomp>....
-00002bd0: 730a 0000 0006 0602 fc04 0104 0106 fd7a  s..............z
-00002be0: 276d 6169 6e2e 3c6c 6f63 616c 733e 2e66  'main.<locals>.f
-00002bf0: 696c 6573 2e3c 6c6f 6361 6c73 3e2e 3c6c  iles.<locals>.<l
-00002c00: 6973 7463 6f6d 703e 2902 7205 0000 00da  istcomp>).r.....
-00002c10: 0676 616c 7565 7372 2600 0000 a901 729a  .valuesr&.....r.
-00002c20: 0000 0072 2600 0000 7227 0000 00da 0566  ...r&...r'.....f
-00002c30: 696c 6573 8702 0000 730a 0000 0000 0202  iles....s.......
-00002c40: 0106 0606 fa04 ff7a 136d 6169 6e2e 3c6c  .......z.main.<l
-00002c50: 6f63 616c 733e 2e66 696c 6573 7a0a 2f61  ocals>.filesz./a
-00002c60: 7069 2f71 7565 7279 5a04 504f 5354 6300  pi/queryZ.POSTc.
-00002c70: 0000 0000 0000 0000 0000 000f 0000 000c  ................
-00002c80: 0000 0013 0000 0073 1201 0000 7400 6a01  .......s....t.j.
-00002c90: 6401 1900 7d00 7400 6a01 6402 1900 7d01  d...}.t.j.d...}.
-00002ca0: 8806 721e 8805 8300 5300 8800 7228 8804  ..r.....S...r(..
-00002cb0: 8300 5300 8802 a002 7c00 7c01 8801 a103  ..S.....|.|.....
-00002cc0: 7d02 6700 7d03 8801 a003 a100 4400 5dc0  }.g.}.......D.].
-00002cd0: 7d04 7c04 6a04 7d05 7405 a006 7c05 7c02  }.|.j.}.t...|.|.
-00002ce0: a102 7405 6a07 6a08 7c05 6403 6404 8d02  ..t.j.j.|.d.d...
-00002cf0: 7405 6a07 a008 7c02 a101 1400 1b00 7d06  t.j...|.......}.
-00002d00: 7405 a009 7c06 0b00 a101 7d07 7c04 6a0a  t...|.....}.|.j.
-00002d10: 7d08 7c04 6a0b 6405 1900 7d09 6700 7d0a  }.|.j.d...}.g.}.
-00002d20: 7c07 6400 8803 8502 1900 4400 5d50 7d0b  |.d.......D.]P}.
-00002d30: 740c 7c06 7c0b 1900 8301 7d0c 7c09 7c0b  t.|.|.....}.|.|.
-00002d40: 1900 7d0d 740d 7c08 7c0d 6405 1900 7c0d  ..}.t.|.|.d...|.
-00002d50: 6403 1900 8502 1900 8301 7d0e 7c0a a00e  d.........}.|...
-00002d60: 7c0e 7c0c 7c0d 740f 7c0b 8301 7c04 6a10  |.|.|.t.|...|.j.
-00002d70: 7c00 7c01 6406 9c07 a101 0100 71a0 7c03  |.|.d.......q.|.
-00002d80: a00e 7c04 6a10 7c0a 6702 a101 0100 7142  ..|.j.|.g.....qB
-00002d90: 7411 7412 7c03 6407 8302 8301 5300 2908  t.t.|.d.....S.).
-00002da0: 4eda 0771 7565 7269 6573 da0b 7072 6566  N..queries..pref
-00002db0: 6572 656e 6365 7372 0900 0000 a901 5a04  erencesr......Z.
-00002dc0: 6178 6973 7201 0000 00a9 0772 2100 0000  axisr......r!...
-00002dd0: da08 6469 7374 616e 6365 7277 0000 00da  ..distancerw....
-00002de0: 0569 6e64 6578 7223 0000 0072 aa00 0000  .indexr#...r....
-00002df0: 72ab 0000 0054 2913 7204 0000 0072 4600  r....T).r....rF.
-00002e00: 0000 da1d 656d 6265 645f 7175 6572 6965  ....embed_querie
-00002e10: 735f 616e 645f 7072 6566 6572 656e 6365  s_and_preference
-00002e20: 7372 a700 0000 724f 0000 0072 6f00 0000  sr....rO...ro...
-00002e30: da03 646f 74da 066c 696e 616c 67da 046e  ..dot..linalg..n
-00002e40: 6f72 6dda 0761 7267 736f 7274 7248 0000  orm..argsortrH..
-00002e50: 0072 4100 0000 da05 666c 6f61 7472 1700  .rA.....floatr..
-00002e60: 0000 726e 0000 0072 8000 0000 7223 0000  ..rn...r....r#..
-00002e70: 0072 0500 0000 721c 0000 0029 0f72 aa00  .r....r....).r..
-00002e80: 0000 72ab 0000 0072 5c00 0000 724e 0000  ..r....r\...rN..
-00002e90: 0072 a500 0000 724f 0000 00da 0964 6973  .r....rO.....dis
-00002ea0: 7461 6e63 6573 da09 736f 7274 6564 5f69  tances..sorted_i
-00002eb0: 7872 4800 0000 7241 0000 00da 0b73 7562  xrH...rA.....sub
-00002ec0: 5f72 6573 756c 7473 72af 0000 0072 ae00  _resultsr....r..
-00002ed0: 0000 7277 0000 0072 2100 0000 2907 da05  ..rw...r!...)...
-00002ee0: 616e 6e6f 7972 9a00 0000 725e 0000 00da  annoyr....r^....
-00002ef0: 0b6e 756d 5f72 6573 756c 7473 da08 7175  .num_results..qu
-00002f00: 6572 7961 6e6e da08 7175 6572 7973 766d  eryann..querysvm
-00002f10: da03 7376 6d72 2600 0000 7227 0000 00da  ..svmr&...r'....
-00002f20: 0571 7565 7279 9402 0000 7342 0000 0000  .query....sB....
-00002f30: 020a 010a 0104 0106 0104 0106 030e 0204  ................
-00002f40: 010c 0106 030a 011a ff04 030c 0206 010a  ................
-00002f50: 0104 0110 010c 0108 0118 0104 0202 0102  ................
-00002f60: 0102 0106 0104 0102 0102 f904 ff06 0b12  ................
-00002f70: 017a 136d 6169 6e2e 3c6c 6f63 616c 733e  .z.main.<locals>
-00002f80: 2e71 7565 7279 7a0d 2f61 7069 2f71 7565  .queryz./api/que
-00002f90: 7279 7376 6d63 0000 0000 0000 0000 0000  rysvmc..........
-00002fa0: 0000 1300 0000 0c00 0000 1300 0000 733c  ..............s<
-00002fb0: 0100 0064 0164 026c 006d 017d 0001 0074  ...d.d.l.m.}...t
-00002fc0: 026a 0364 0319 007d 0174 026a 0364 0419  .j.d...}.t.j.d..
-00002fd0: 007d 0288 01a0 047c 017c 0288 00a1 037d  .}.....|.|.....}
-00002fe0: 0367 007d 0488 00a0 05a1 0044 005d f27d  .g.}.......D.].}
-00002ff0: 057c 056a 067d 0674 07a0 087c 067c 0364  .|.j.}.t...|.|.d
-00003000: 0519 0067 02a1 017d 0774 07a0 0974 0a7c  ...g...}.t...t.|
-00003010: 0683 0164 0617 00a1 017d 0864 067c 0864  ...d.....}.d.|.d
-00003020: 073c 007c 006a 0b64 0864 0964 0a64 0b88  .<.|.j.d.d.d.d..
-00003030: 0364 0c8d 057d 097c 09a0 0c7c 077c 08a1  .d...}.|...|.|..
-00003040: 0201 007c 09a0 0d7c 07a1 0164 0074 0a7c  ...|...|...d.t.|
-00003050: 0683 0185 0219 007d 0a74 07a0 0e7c 0a0b  .......}.t...|..
-00003060: 00a1 017d 0b7c 056a 0f7d 0c7c 056a 107d  ...}.|.j.}.|.j.}
-00003070: 0d67 007d 0e7c 0b64 0088 0285 0219 0044  .g.}.|.d.......D
-00003080: 005d 4c7d 0f7c 0a7c 0f19 007d 107c 0d7c  .]L}.|.|...}.|.|
-00003090: 0f19 007d 1174 117c 0c7c 1164 0119 007c  ...}.t.|.|.d...|
-000030a0: 1164 0619 0085 0219 0083 017d 127c 0ea0  .d.........}.|..
-000030b0: 127c 127c 107c 1174 137c 0f83 017c 056a  .|.|.|.t.|...|.j
-000030c0: 147c 017c 0264 0d9c 07a1 0101 0071 ce7c  .|.|.d.......q.|
-000030d0: 04a0 127c 056a 147c 0e67 02a1 0101 0071  ...|.j.|.g.....q
-000030e0: 3a74 1574 167c 0464 0e83 0283 0153 0029  :t.t.|.d.....S.)
-000030f0: 0f4e 7201 0000 0029 0172 bd00 0000 72aa  .Nr....).r....r.
-00003100: 0000 0072 ab00 0000 2902 4e2e 7209 0000  ...r....).N.r...
-00003110: 0072 8200 0000 5a08 6261 6c61 6e63 6564  .r....Z.balanced
-00003120: 4669 1027 0000 678d edb5 a0f7 c6b0 3e29  Fi.'..g.......>)
-00003130: 055a 0c63 6c61 7373 5f77 6569 6768 74da  .Z.class_weight.
-00003140: 0776 6572 626f 7365 5a08 6d61 785f 6974  .verboseZ.max_it
-00003150: 6572 5a03 746f 6cda 0143 72ad 0000 0054  erZ.tol..Cr....T
-00003160: 2917 5a07 736b 6c65 6172 6e72 bd00 0000  ).Z.sklearnr....
-00003170: 7204 0000 0072 4600 0000 72b0 0000 0072  r....rF...r....r
-00003180: a700 0000 724f 0000 0072 6f00 0000 5a0b  ....rO...ro...Z.
-00003190: 636f 6e63 6174 656e 6174 655a 057a 6572  concatenateZ.zer
-000031a0: 6f73 724a 0000 005a 094c 696e 6561 7253  osrJ...Z.LinearS
-000031b0: 5643 5a03 6669 745a 1164 6563 6973 696f  VCZ.fitZ.decisio
-000031c0: 6e5f 6675 6e63 7469 6f6e 72b4 0000 0072  n_functionr....r
-000031d0: 4800 0000 7241 0000 0072 1700 0000 726e  H...rA...r....rn
-000031e0: 0000 0072 8000 0000 7223 0000 0072 0500  ...r....r#...r..
-000031f0: 0000 721c 0000 0029 1372 bd00 0000 72aa  ..r....).r....r.
-00003200: 0000 0072 ab00 0000 725c 0000 0072 4e00  ...r....r\...rN.
-00003210: 0000 72a5 0000 0072 4f00 0000 da01 78da  ..r....rO.....x.
-00003220: 0179 5a03 636c 665a 0c73 696d 696c 6172  .yZ.clfZ.similar
-00003230: 6974 6965 7372 b700 0000 7248 0000 0072  itiesr....rH...r
-00003240: 4100 0000 72b8 0000 0072 af00 0000 72ae  A...r....r....r.
-00003250: 0000 0072 7700 0000 7221 0000 0029 0472  ...rw...r!...).r
-00003260: 9a00 0000 725e 0000 0072 ba00 0000 da05  ....r^...r......
-00003270: 7376 6d5f 6372 2600 0000 7227 0000 0072  svm_cr&...r'...r
-00003280: bc00 0000 bf02 0000 734e 0000 0000 020c  ........sN......
-00003290: 020a 010a 030e 0104 010c 0106 0212 0112  ................
-000032a0: 0108 0304 0102 0102 0102 0102 0102 fb06  ................
-000032b0: 070c 0316 010c 0206 0106 0104 0110 0108  ................
-000032c0: 0108 0118 0104 0202 0102 0102 0106 0104  ................
-000032d0: 0102 0102 f904 ff06 0b12 027a 166d 6169  ...........z.mai
-000032e0: 6e2e 3c6c 6f63 616c 733e 2e71 7565 7279  n.<locals>.query
-000032f0: 7376 6d7a 0d2f 6170 692f 7175 6572 7961  svmz./api/querya
-00003300: 6e6e 6300 0000 0000 0000 0000 0000 000d  nnc.............
-00003310: 0000 000c 0000 0013 0000 0073 d600 0000  ...........s....
-00003320: 7400 6a01 6401 1900 7d00 7400 6a01 6402  t.j.d...}.t.j.d.
-00003330: 1900 7d01 8801 a002 7c00 7c01 8800 a103  ..}.....|.|.....
-00003340: 7d02 6700 7d03 8800 a003 a100 4400 5d98  }.g.}.......D.].
-00003350: 7d04 7c04 6a04 7d05 7c04 6a05 7d06 7c04  }.|.j.}.|.j.}.|.
-00003360: 6a06 6403 1900 7d07 6700 7d08 7407 7c05  j.d...}.g.}.t.|.
-00003370: a008 7c02 8802 6404 6405 a104 8e00 4400  ..|...d.d.....D.
-00003380: 5d54 5c02 7d09 7d0a 7c07 7c09 1900 7d0b  ]T\.}.}.|.|...}.
-00003390: 7409 7c06 7c0b 6403 1900 7c0b 6406 1900  t.|.|.d...|.d...
-000033a0: 8502 1900 8301 7d0c 7c08 a00a 7c0c 6406  ......}.|...|.d.
-000033b0: 7c0a 6407 1300 6407 1b00 1800 7c0b 740b  |.d...d.....|.t.
-000033c0: 7c09 8301 7c04 6a0c 7c00 7c01 6408 9c07  |...|.j.|.|.d...
-000033d0: a101 0100 7160 7c03 a00a 7c04 6a0c 7c08  ....q`|...|.j.|.
-000033e0: 6702 a101 0100 712e 740d 740e 7c03 6405  g.....q.t.t.|.d.
-000033f0: 8302 8301 5300 2909 4e72 aa00 0000 72ab  ....S.).Nr....r.
-00003400: 0000 0072 0100 0000 7282 0000 0054 7209  ...r....r....Tr.
-00003410: 0000 0067 0000 0000 0000 0040 72ad 0000  ...g.......@r...
-00003420: 0029 0f72 0400 0000 7246 0000 0072 b000  .).r....rF...r..
-00003430: 0000 72a7 0000 0072 4d00 0000 7248 0000  ..r....rM...rH..
-00003440: 0072 4100 0000 726d 0000 005a 1167 6574  .rA...rm...Z.get
-00003450: 5f6e 6e73 5f62 795f 7665 6374 6f72 7217  _nns_by_vectorr.
-00003460: 0000 0072 6e00 0000 7280 0000 0072 2300  ...rn...r....r#.
-00003470: 0000 7205 0000 0072 1c00 0000 290d 72aa  ..r....r....).r.
-00003480: 0000 0072 ab00 0000 725c 0000 0072 4e00  ...r....r\...rN.
-00003490: 0000 72a5 0000 0072 4d00 0000 7248 0000  ..r....rM...rH..
-000034a0: 0072 4100 0000 72b8 0000 0072 af00 0000  .rA...r....r....
-000034b0: 72ae 0000 0072 7700 0000 7221 0000 0029  r....rw...r!...)
-000034c0: 0372 9a00 0000 725e 0000 0072 ba00 0000  .r....r^...r....
-000034d0: 7226 0000 0072 2700 0000 72bb 0000 00f4  r&...r'...r.....
-000034e0: 0200 0073 3400 0000 0002 0a01 0a03 0e02  ...s4...........
-000034f0: 0401 0c01 0601 0601 0a01 0401 0201 0eff  ................
-00003500: 0c03 0801 1801 0402 0202 0e01 0201 0601  ................
-00003510: 0401 0201 02f8 04ff 060c 1201 7a16 6d61  ............z.ma
-00003520: 696e 2e3c 6c6f 6361 6c73 3e2e 7175 6572  in.<locals>.quer
-00003530: 7961 6e6e 7a0c 2f61 7069 2f65 7870 6c61  yannz./api/expla
-00003540: 696e 6300 0000 0000 0000 0000 0000 0009  inc.............
-00003550: 0000 0006 0000 0013 0000 0073 c000 0000  ...........s....
-00003560: 7400 6a01 6401 1900 7d00 7400 6a01 6402  t.j.d...}.t.j.d.
-00003570: 1900 7d01 8803 7c00 1900 6a02 7c01 6403  ..}...|...j.|.d.
-00003580: 1900 7c01 6404 1900 8502 1900 8902 7400  ..|.d.........t.
-00003590: 6a01 6405 1900 7d02 7400 6a01 6406 1900  j.d...}.t.j.d...
-000035a0: 7d03 8806 a003 7c02 7c03 8803 a103 8900  }.....|.|.......
-000035b0: 6407 6408 6403 7404 8802 8301 6604 6409  d.d.d.t.....f.d.
-000035c0: 640a 8401 7d04 8702 6601 640b 640c 8408  d...}...f.d.d...
-000035d0: 8901 8700 8701 8706 8702 6604 640d 640e  ..........f.d.d.
-000035e0: 8408 7d05 8702 6601 640f 6410 8408 7d06  ..}...f.d.d...}.
-000035f0: 7c04 8805 8804 6403 7404 8802 8301 6411  |.....d.t.....d.
-00003600: 8d04 7d07 7c05 7c07 8301 6400 8807 8502  ..}.|.|...d.....
-00003610: 1900 7d08 7405 7c06 7c08 8301 8301 5300  ..}.t.|.|.....S.
-00003620: 2912 4e72 2300 0000 7277 0000 0072 0100  ).Nr#...rw...r..
-00003630: 0000 7209 0000 0072 aa00 0000 72ab 0000  ..r....r....r...
-00003640: 0072 9200 0000 e903 0000 0063 0400 0000  .r.........c....
-00003650: 0000 0000 0000 0000 0800 0000 0900 0000  ................
-00003660: 5300 0000 7362 0000 0074 00a0 017c 037c  S...sb...t...|.|
-00003670: 0218 007c 001b 00a1 017d 0474 00a0 017c  ...|.....}.t...|
-00003680: 037c 0218 007c 011b 00a1 017d 0567 007d  .|...|.....}.g.}
-00003690: 0674 027c 0183 0144 005d 2c7d 077c 06a0  .t.|...D.],}.|..
-000036a0: 037c 027c 077c 0514 0017 0074 047c 037c  .|.|.|.....t.|.|
-000036b0: 027c 077c 0514 0017 007c 0417 0083 0266  .|.|.....|.....f
-000036c0: 02a1 0101 0071 307c 0653 0072 3900 0000  .....q0|.S.r9...
-000036d0: 2905 da04 6d61 7468 5a04 6365 696c da05  )...mathZ.ceil..
-000036e0: 7261 6e67 6572 6e00 0000 da03 6d69 6e29  rangern.....min)
-000036f0: 08da 0d64 6976 6964 655f 6661 6374 6f72  ...divide_factor
-00003700: da0a 6e75 6d5f 7370 6c69 7473 da05 7374  ..num_splits..st
-00003710: 6172 74da 0365 6e64 5a0d 7769 6e64 6f77  art..endZ.window
-00003720: 5f6c 656e 6774 685a 0c73 706c 6974 5f6c  _lengthZ.split_l
-00003730: 656e 6774 68da 0673 706c 6974 73da 0169  ength..splits..i
-00003740: 7226 0000 0072 2600 0000 7227 0000 00da  r&...r&...r'....
-00003750: 0a67 6574 5f73 706c 6974 7320 0300 0073  .get_splits ...s
-00003760: 1400 0000 0001 1201 1201 0401 0c01 0402  ................
-00003770: 0a01 14fe 02ff 0606 7a29 6d61 696e 2e3c  ........z)main.<
-00003780: 6c6f 6361 6c73 3e2e 6578 706c 6169 6e2e  locals>.explain.
-00003790: 3c6c 6f63 616c 733e 2e67 6574 5f73 706c  <locals>.get_spl
-000037a0: 6974 7363 0200 0000 0000 0000 0000 0000  itsc............
-000037b0: 0200 0000 0500 0000 1300 0000 731c 0000  ............s...
-000037c0: 0074 0088 0064 007c 0085 0219 0088 007c  .t...d.|.......|
-000037d0: 0164 0085 0219 0017 0083 0153 0072 3900  .d.........S.r9.
-000037e0: 0000 2901 7217 0000 0029 0272 ca00 0000  ..).r....).r....
-000037f0: 72cb 0000 00a9 0172 5f00 0000 7226 0000  r......r_...r&..
-00003800: 0072 2700 0000 da0e 6578 636c 7564 655f  .r'.....exclude_
-00003810: 7769 6e64 6f77 2d03 0000 7302 0000 0000  window-...s.....
-00003820: 027a 2d6d 6169 6e2e 3c6c 6f63 616c 733e  .z-main.<locals>
-00003830: 2e65 7870 6c61 696e 2e3c 6c6f 6361 6c73  .explain.<locals
-00003840: 3e2e 6578 636c 7564 655f 7769 6e64 6f77  >.exclude_window
-00003850: 6301 0000 0000 0000 0000 0000 0004 0000  c...............
-00003860: 0005 0000 0013 0000 0073 6800 0000 8701  .........sh.....
-00003870: 6601 6401 6402 8408 7c00 4400 8301 7d01  f.d.d...|.D...}.
-00003880: 7400 a001 8702 6601 6403 6402 8408 7c01  t.....f.d.d...|.
-00003890: 4400 8301 a101 7d02 7c02 a002 8800 a101  D.....}.|.......
-000038a0: 7400 6a03 6a04 7c02 6404 6405 8d02 7400  t.j.j.|.d.d...t.
-000038b0: 6a03 a004 8800 a101 1400 1b00 7d03 7405  j...........}.t.
-000038c0: 7406 7c00 7c03 8302 6406 6407 8400 6408  t.|.|...d.d...d.
-000038d0: 6409 8d03 5300 290a 4e63 0100 0000 0000  d...S.).Nc......
-000038e0: 0000 0000 0000 0300 0000 0500 0000 1300  ................
-000038f0: 0000 731a 0000 0067 007c 005d 125c 027d  ..s....g.|.].\.}
-00003900: 017d 0288 007c 017c 0283 0291 0271 0453  .}...|.|.....q.S
-00003910: 0072 2600 0000 7226 0000 0029 0372 a400  .r&...r&...).r..
-00003920: 0000 72ca 0000 0072 cb00 0000 2901 72d0  ..r....r....).r.
-00003930: 0000 0072 2600 0000 7227 0000 0072 a600  ...r&...r'...r..
-00003940: 0000 3303 0000 f300 0000 007a 4b6d 6169  ..3........zKmai
-00003950: 6e2e 3c6c 6f63 616c 733e 2e65 7870 6c61  n.<locals>.expla
-00003960: 696e 2e3c 6c6f 6361 6c73 3e2e 6765 745f  in.<locals>.get_
-00003970: 6869 6768 6573 745f 7261 6e6b 6564 5f73  highest_ranked_s
-00003980: 706c 6974 2e3c 6c6f 6361 6c73 3e2e 3c6c  plit.<locals>.<l
-00003990: 6973 7463 6f6d 703e 6301 0000 0000 0000  istcomp>c.......
-000039a0: 0000 0000 0002 0000 0006 0000 0013 0000  ................
-000039b0: 0073 1a00 0000 6700 7c00 5d12 7d01 7400  .s....g.|.].}.t.
-000039c0: 8800 a001 7c01 a101 8301 9102 7104 5300  ....|.......q.S.
-000039d0: 7226 0000 0029 0272 0d00 0000 5a0e 656d  r&...).r....Z.em
-000039e0: 6265 645f 646f 6375 6d65 6e74 2902 72a4  bed_document).r.
-000039f0: 0000 005a 0b73 706c 6974 5f71 7565 7279  ...Z.split_query
-00003a00: 2901 725e 0000 0072 2600 0000 7227 0000  ).r^...r&...r'..
-00003a10: 0072 a600 0000 3503 0000 7304 0000 0006  .r....5...s.....
-00003a20: 0202 ff72 0900 0000 72ac 0000 0063 0100  ...r....r....c..
-00003a30: 0000 0000 0000 0000 0000 0100 0000 0200  ................
-00003a40: 0000 5300 0000 7308 0000 007c 0064 0119  ..S...s....|.d..
-00003a50: 0053 0029 024e 7209 0000 0072 2600 0000  .S.).Nr....r&...
-00003a60: a901 72c1 0000 0072 2600 0000 7226 0000  ..r....r&...r&..
-00003a70: 0072 2700 0000 da08 3c6c 616d 6264 613e  .r'.....<lambda>
-00003a80: 3e03 0000 72d1 0000 007a 496d 6169 6e2e  >...r....zImain.
-00003a90: 3c6c 6f63 616c 733e 2e65 7870 6c61 696e  <locals>.explain
-00003aa0: 2e3c 6c6f 6361 6c73 3e2e 6765 745f 6869  .<locals>.get_hi
-00003ab0: 6768 6573 745f 7261 6e6b 6564 5f73 706c  ghest_ranked_spl
-00003ac0: 6974 2e3c 6c6f 6361 6c73 3e2e 3c6c 616d  it.<locals>.<lam
-00003ad0: 6264 613e 4629 02da 036b 6579 da07 7265  bda>F)...key..re
-00003ae0: 7665 7273 6529 0772 6f00 0000 5a05 6172  verse).ro...Z.ar
-00003af0: 7261 7972 b100 0000 72b2 0000 0072 b300  rayr....r....r..
-00003b00: 0000 da06 736f 7274 6564 726d 0000 0029  ....sortedrm...)
-00003b10: 0472 cc00 0000 5a0d 7370 6c69 745f 7175  .r....Z.split_qu
-00003b20: 6572 6965 735a 0d73 706c 6974 5f77 696e  eriesZ.split_win
-00003b30: 646f 7773 72b6 0000 0029 0472 5c00 0000  dowsr....).r\...
-00003b40: 72d0 0000 0072 5e00 0000 725f 0000 0072  r....r^...r_...r
-00003b50: 2600 0000 7227 0000 00da 1867 6574 5f68  &...r'.....get_h
-00003b60: 6967 6865 7374 5f72 616e 6b65 645f 7370  ighest_ranked_sp
-00003b70: 6c69 7431 0300 0073 1400 0000 0002 1201  lit1...s........
-00003b80: 0401 0a02 02fe 04ff 0406 0801 1aff 0404  ................
-00003b90: 7a37 6d61 696e 2e3c 6c6f 6361 6c73 3e2e  z7main.<locals>.
-00003ba0: 6578 706c 6169 6e2e 3c6c 6f63 616c 733e  explain.<locals>
-00003bb0: 2e67 6574 5f68 6967 6865 7374 5f72 616e  .get_highest_ran
-00003bc0: 6b65 645f 7370 6c69 7463 0100 0000 0000  ked_splitc......
-00003bd0: 0000 0000 0000 0500 0000 0500 0000 1300  ................
-00003be0: 0000 7380 0000 0074 0064 0164 0284 007c  ..s....t.d.d...|
-00003bf0: 0044 0083 0164 0364 0484 0064 058d 027d  .D...d.d...d...}
-00003c00: 0164 067d 0267 0089 0087 0087 0166 0264  .d.}.g.......f.d
-00003c10: 0764 0884 087d 037c 0144 005d 367d 047c  .d...}.|.D.]6}.|
-00003c20: 037c 027c 0464 0619 0064 0983 0301 007c  .|.|.d...d.....|
-00003c30: 0374 017c 0464 0619 007c 0283 027c 0464  .t.|.d...|...|.d
-00003c40: 0a19 0064 0b83 0301 007c 0464 0a19 007d  ...d.....|.d...}
-00003c50: 0271 347c 037c 0274 0288 0183 0164 0983  .q4|.|.t.....d..
-00003c60: 0301 0088 0053 0029 0c4e 6301 0000 0000  .....S.).Nc.....
-00003c70: 0000 0000 0000 0002 0000 0004 0000 0053  ...............S
-00003c80: 0000 0073 1400 0000 6700 7c00 5d0c 7d01  ...s....g.|.].}.
-00003c90: 7c01 6400 1900 9102 7104 5300 2901 7201  |.d.....q.S.).r.
-00003ca0: 0000 0072 2600 0000 2902 72a4 0000 0072  ...r&...).r....r
-00003cb0: 7e00 0000 7226 0000 0072 2600 0000 7227  ~...r&...r&...r'
-00003cc0: 0000 0072 a600 0000 4203 0000 72d1 0000  ...r....B...r...
-00003cd0: 007a 3c6d 6169 6e2e 3c6c 6f63 616c 733e  .z<main.<locals>
-00003ce0: 2e65 7870 6c61 696e 2e3c 6c6f 6361 6c73  .explain.<locals
-00003cf0: 3e2e 6173 5f74 6f6b 656e 732e 3c6c 6f63  >.as_tokens.<loc
-00003d00: 616c 733e 2e3c 6c69 7374 636f 6d70 3e63  als>.<listcomp>c
-00003d10: 0100 0000 0000 0000 0000 0000 0100 0000  ................
-00003d20: 0200 0000 5300 0000 7308 0000 007c 0064  ....S...s....|.d
-00003d30: 0119 0053 0072 4900 0000 7226 0000 0072  ...S.rI...r&...r
-00003d40: d200 0000 7226 0000 0072 2600 0000 7227  ....r&...r&...r'
-00003d50: 0000 0072 d300 0000 4203 0000 72d1 0000  ...r....B...r...
-00003d60: 007a 3a6d 6169 6e2e 3c6c 6f63 616c 733e  .z:main.<locals>
-00003d70: 2e65 7870 6c61 696e 2e3c 6c6f 6361 6c73  .explain.<locals
-00003d80: 3e2e 6173 5f74 6f6b 656e 732e 3c6c 6f63  >.as_tokens.<loc
-00003d90: 616c 733e 2e3c 6c61 6d62 6461 3e29 0172  als>.<lambda>).r
-00003da0: d400 0000 7201 0000 0063 0300 0000 0000  ....r....c......
-00003db0: 0000 0000 0000 0300 0000 0600 0000 1300  ................
-00003dc0: 0000 732c 0000 007c 007c 016b 0572 0c64  ..s,...|.|.k.r.d
-00003dd0: 0053 0088 00a0 0074 0188 017c 007c 0185  .S.....t...|.|..
-00003de0: 0219 0083 017c 0264 019c 02a1 0101 0064  .....|.d.......d
-00003df0: 0053 0029 024e 2902 7221 0000 0072 8300  .S.).N).r!...r..
-00003e00: 0000 2902 726e 0000 0072 1700 0000 2903  ..).rn...r....).
-00003e10: 72ca 0000 0072 cb00 0000 7283 0000 0029  r....r....r....)
-00003e20: 02da 0663 6875 6e6b 7372 5f00 0000 7226  ...chunksr_...r&
-00003e30: 0000 0072 2700 0000 726e 0000 0046 0300  ...r'...rn...F..
-00003e40: 0073 0e00 0000 0001 0801 0402 0402 0e01  .s..............
-00003e50: 02fe 04ff 7a38 6d61 696e 2e3c 6c6f 6361  ....z8main.<loca
-00003e60: 6c73 3e2e 6578 706c 6169 6e2e 3c6c 6f63  ls>.explain.<loc
-00003e70: 616c 733e 2e61 735f 746f 6b65 6e73 2e3c  als>.as_tokens.<
-00003e80: 6c6f 6361 6c73 3e2e 6170 7065 6e64 5a06  locals>.appendZ.
-00003e90: 6e6f 726d 616c 7209 0000 005a 0968 6967  normalr....Z.hig
-00003ea0: 686c 6967 6874 2903 72d6 0000 00da 036d  hlight).r......m
-00003eb0: 6178 724a 0000 0029 0572 cc00 0000 da07  axrJ...).r......
-00003ec0: 696e 6469 6365 735a 0a6c 6173 745f 696e  indicesZ.last_in
-00003ed0: 6465 7872 6e00 0000 72af 0000 0072 cf00  dexrn...r....r..
-00003ee0: 0000 2901 72d8 0000 0072 2700 0000 da09  ..).r....r'.....
-00003ef0: 6173 5f74 6f6b 656e 7340 0300 0073 1400  as_tokens@...s..
-00003f00: 0000 0002 1a01 0401 0402 0e0b 0801 1001  ................
-00003f10: 1a01 0a02 1001 7a28 6d61 696e 2e3c 6c6f  ......z(main.<lo
-00003f20: 6361 6c73 3e2e 6578 706c 6169 6e2e 3c6c  cals>.explain.<l
-00003f30: 6f63 616c 733e 2e61 735f 746f 6b65 6e73  ocals>.as_tokens
-00003f40: 2904 72c8 0000 0072 c900 0000 72ca 0000  ).r....r....r...
-00003f50: 0072 cb00 0000 2906 7204 0000 0072 4600  .r....).r....rF.
-00003f60: 0000 7248 0000 0072 b000 0000 724a 0000  ..rH...r....rJ..
-00003f70: 0072 0500 0000 2909 7223 0000 0072 7700  .r....).r#...rw.
-00003f80: 0000 72aa 0000 0072 ab00 0000 72ce 0000  ..r....r....r...
-00003f90: 0072 d700 0000 72db 0000 0072 cc00 0000  .r....r....r....
-00003fa0: 5a0a 746f 705f 7370 6c69 7473 2905 729a  Z.top_splits).r.
-00003fb0: 0000 00da 1365 7870 6c61 696e 5f73 706c  .....explain_spl
-00003fc0: 6974 5f63 6f75 6e74 da14 6578 706c 6169  it_count..explai
-00003fd0: 6e5f 7370 6c69 745f 6469 7669 6465 725e  n_split_divider^
-00003fe0: 0000 00da 166e 756d 5f65 7870 6c61 696e  .....num_explain
-00003ff0: 5f68 6967 686c 6967 6874 7329 0372 5c00  _highlights).r\.
-00004000: 0000 72d0 0000 0072 5f00 0000 7227 0000  ..r....r_...r'..
-00004010: 00da 0765 7870 6c61 696e 1603 0000 7324  ...explain....s$
-00004020: 0000 0000 020a 010a 011a 010a 010a 010e  ................
-00004030: 0316 0d0c 0412 0f0c 1902 0102 0102 0102  ................
-00004040: 0106 fc06 0610 017a 156d 6169 6e2e 3c6c  .......z.main.<l
-00004050: 6f63 616c 733e 2e65 7870 6c61 696e 7a0c  ocals>.explainz.
-00004060: 2f61 7069 2f67 6574 6669 6c65 6300 0000  /api/getfilec...
-00004070: 0000 0000 0000 0000 0002 0000 0003 0000  ................
-00004080: 0013 0000 0073 2200 0000 7400 6a01 a002  .....s"...t.j...
-00004090: 6401 a101 7d00 8800 7c00 8301 7d01 7c01  d...}...|...}.|.
-000040a0: 6a03 7d00 7404 7c00 8301 5300 a902 4e72  j.}.t.|...S...Nr
-000040b0: 2300 0000 2905 7204 0000 00da 0461 7267  #...).r......arg
-000040c0: 73da 0367 6574 7223 0000 0072 0700 0000  s..getr#...r....
-000040d0: 7297 0000 00a9 0172 9b00 0000 7226 0000  r......r....r&..
-000040e0: 0072 2700 0000 da07 6765 7466 696c 6562  .r'.....getfileb
-000040f0: 0300 0073 0800 0000 0002 0c01 0801 0601  ...s............
-00004100: 7a15 6d61 696e 2e3c 6c6f 6361 6c73 3e2e  z.main.<locals>.
-00004110: 6765 7466 696c 657a 112f 6170 692f 7064  getfilez./api/pd
-00004120: 6670 6f73 6974 696f 6e73 6300 0000 0000  fpositionsc.....
-00004130: 0000 0000 0000 0002 0000 0003 0000 0013  ................
-00004140: 0000 0073 3400 0000 7400 6a01 a002 6401  ...s4...t.j...d.
-00004150: a101 7d00 8800 7c00 8301 7d01 7c01 6a03  ..}...|...}.|.j.
-00004160: 6402 6b02 7228 7404 7c01 6a05 8301 5300  d.k.r(t.|.j...S.
-00004170: 7404 6700 8301 5300 6400 5300 2903 4e72  t.g...S.d.S.).Nr
-00004180: 2300 0000 da03 7064 6629 0672 0400 0000  #.....pdf).r....
-00004190: 72e1 0000 0072 e200 0000 7224 0000 0072  r....r....r$...r
-000041a0: 0500 0000 5a09 706f 7369 7469 6f6e 7372  ....Z.positionsr
-000041b0: 9700 0000 72e3 0000 0072 2600 0000 7227  ....r....r&...r'
-000041c0: 0000 00da 0c70 6466 706f 7369 7469 6f6e  .....pdfposition
-000041d0: 7369 0300 0073 0a00 0000 0002 0c01 0801  si...s..........
-000041e0: 0a01 0a02 7a1a 6d61 696e 2e3c 6c6f 6361  ....z.main.<loca
-000041f0: 6c73 3e2e 7064 6670 6f73 6974 696f 6e73  ls>.pdfpositions
-00004200: 7a0c 2f61 7069 2f70 6466 7061 6765 6300  z./api/pdfpagec.
-00004210: 0000 0000 0000 0000 0000 0007 0000 0005  ................
-00004220: 0000 0013 0000 0073 8200 0000 7400 6a01  .......s....t.j.
-00004230: a002 6401 a101 7d00 8800 7c00 8301 7d01  ..d...}...|...}.
-00004240: 7400 6a01 a002 6402 a101 7d02 7400 6a01  t.j...d...}.t.j.
-00004250: a002 6403 a101 7d03 7c01 6a03 6404 6b02  ..d...}.|.j.d.k.
-00004260: 727e 7c01 a004 7405 7c02 8301 7406 7c03  r~|...t.|...t.|.
-00004270: 8301 a102 7d04 7407 a008 a100 7d05 7c04  ....}.t.....}.|.
-00004280: 6a09 7c05 6405 6406 8d02 0100 740a 7c05  j.|.d.d.....t.|.
-00004290: a00b a100 8301 7d06 7c06 6a0c a00d 6407  ......}.|.j...d.
-000042a0: 6408 a102 0100 7c06 5300 6400 5300 2909  d.....|.S.d.S.).
-000042b0: 4e72 2300 0000 da04 7061 6765 da05 7363  Nr#.....page..sc
-000042c0: 616c 6572 e500 0000 5a03 504e 4729 01da  aler....Z.PNG)..
-000042d0: 0666 6f72 6d61 747a 0c43 6f6e 7465 6e74  .formatz.Content
-000042e0: 2d54 7970 657a 0969 6d61 6765 2f70 6e67  -Typez.image/png
-000042f0: 290e 7204 0000 0072 e100 0000 72e2 0000  ).r....r....r...
-00004300: 0072 2400 0000 5a12 6765 745f 7061 6765  .r$...Z.get_page
-00004310: 5f69 6d61 6765 5f70 696c 7280 0000 0072  _image_pilr....r
-00004320: b500 0000 da02 696f da07 4279 7465 7349  ......io..BytesI
-00004330: 4f5a 0473 6176 6572 0800 0000 da08 6765  OZ.saver......ge
-00004340: 7476 616c 7565 5a07 6865 6164 6572 73da  tvalueZ.headers.
-00004350: 0373 6574 2907 7223 0000 0072 4500 0000  .set).r#...rE...
-00004360: 72e7 0000 0072 e800 0000 5a09 7069 6c5f  r....r....Z.pil_
-00004370: 696d 6167 655a 0c69 6d67 5f62 7974 655f  imageZ.img_byte_
-00004380: 6172 725a 0872 6573 706f 6e73 6572 e300  arrZ.responser..
-00004390: 0000 7226 0000 0072 2700 0000 da07 7064  ..r&...r'.....pd
-000043a0: 6670 6167 6572 0300 0073 1600 0000 0002  fpager...s......
-000043b0: 0c01 0801 0c01 0c01 0a01 1401 0801 0e01  ................
-000043c0: 0c01 0e01 7a15 6d61 696e 2e3c 6c6f 6361  ....z.main.<loca
-000043d0: 6c73 3e2e 7064 6670 6167 657a 0d2f 6170  ls>.pdfpagez./ap
-000043e0: 692f 7064 6663 6861 7273 6300 0000 0000  i/pdfcharsc.....
-000043f0: 0000 0000 0000 0003 0000 0005 0000 0013  ................
-00004400: 0000 0073 4400 0000 7400 6a01 a002 6401  ...sD...t.j...d.
-00004410: a101 7d00 8800 7c00 8301 7d01 7c01 6a03  ..}...|...}.|.j.
-00004420: 6402 6b03 7226 7404 6700 8301 5300 7400  d.k.r&t.g...S.t.
-00004430: 6a01 a002 6403 a101 7d02 7404 7c01 a005  j...d...}.t.|...
-00004440: 7406 7c02 8301 a101 8301 5300 2904 4e72  t.|.......S.).Nr
-00004450: 2300 0000 72e5 0000 0072 e700 0000 2907  #...r....r....).
-00004460: 7204 0000 0072 e100 0000 72e2 0000 0072  r....r....r....r
-00004470: 2400 0000 7205 0000 005a 0e67 6574 5f70  $...r....Z.get_p
-00004480: 6167 655f 6368 6172 7372 8000 0000 2903  age_charsr....).
-00004490: 7223 0000 0072 4500 0000 72e7 0000 0072  r#...rE...r....r
-000044a0: e300 0000 7226 0000 0072 2700 0000 da08  ....r&...r'.....
-000044b0: 7064 6663 6861 7273 8003 0000 730c 0000  pdfchars....s...
-000044c0: 0000 020c 0108 010a 0108 010c 017a 166d  .............z.m
-000044d0: 6169 6e2e 3c6c 6f63 616c 733e 2e70 6466  ain.<locals>.pdf
-000044e0: 6368 6172 737a 092f 6170 692f 7465 7874  charsz./api/text
-000044f0: 6300 0000 0000 0000 0000 0000 0001 0000  c...............
-00004500: 0003 0000 0013 0000 0073 1a00 0000 7400  .........s....t.
-00004510: 6a01 a002 6401 a101 7d00 7403 8800 7c00  j...d...}.t...|.
-00004520: 1900 6a04 8301 5300 72e0 0000 0029 0572  ..j...S.r....).r
-00004530: 0400 0000 72e1 0000 0072 e200 0000 7205  ....r....r....r.
-00004540: 0000 0072 4800 0000 2901 7223 0000 0072  ...rH...).r#...r
-00004550: a800 0000 7226 0000 0072 2700 0000 7221  ....r&...r'...r!
-00004560: 0000 0089 0300 0073 0400 0000 0002 0c01  .......s........
-00004570: 7a12 6d61 696e 2e3c 6c6f 6361 6c73 3e2e  z.main.<locals>.
-00004580: 7465 7874 2902 da04 686f 7374 da04 706f  text)...host..po
-00004590: 7274 2919 da05 7072 696e 7472 6b00 0000  rt)...printrk...
-000045a0: 720a 0000 0072 6c00 0000 5a0b 6765 745f  r....rl...Z.get_
-000045b0: 6170 705f 6469 7272 4a00 0000 5a0a 5573  app_dirrJ...Z.Us
-000045c0: 6167 6545 7272 6f72 da04 6c69 7374 7281  ageError..listr.
-000045d0: 0000 00da 1854 5241 4e53 464f 524d 4552  .....TRANSFORMER
-000045e0: 5f50 4f4f 4c5f 4445 4641 554c 5472 0c00  _POOL_DEFAULTr..
-000045f0: 0000 72e2 0000 005a 0d69 735f 6173 796d  ..r....Z.is_asym
-00004600: 6d65 7472 6963 724c 0000 0072 0200 0000  metricrL...r....
-00004610: 5a0f 7365 745f 6465 7363 7269 7074 696f  Z.set_descriptio
-00004620: 6e72 6100 0000 7262 0000 0072 6500 0000  nra...rb...re...
-00004630: 727a 0000 005a 1267 6574 5f6e 756d 5f64  rz...Z.get_num_d
-00004640: 696d 656e 7369 6f6e 7372 0300 0000 7229  imensionsr....r)
-00004650: 0000 005a 0572 6f75 7465 da03 7275 6e29  ...Z.route..run)
-00004660: 2d72 2300 0000 7240 0000 005a 096e 6f5f  -r#...r@...Z.no_
-00004670: 7365 7276 6572 72f1 0000 0072 f000 0000  serverr....r....
-00004680: 7273 0000 0072 7200 0000 7293 0000 0072  rs...rr...r....r
-00004690: 9400 0000 7295 0000 0072 9600 0000 725e  ....r....r....r^
-000046a0: 0000 005a 1174 7261 6e73 666f 726d 6572  ...Z.transformer
-000046b0: 5f6d 6f64 656c 7255 0000 0072 ba00 0000  _modelrU...r....
-000046c0: 72b9 0000 0072 bd00 0000 72c3 0000 0072  r....r....r....r
-000046d0: dc00 0000 72dd 0000 0072 de00 0000 7234  ....r....r....r4
-000046e0: 0000 0072 3500 0000 7274 0000 00da 0776  ...r5...rt.....v
-000046f0: 6572 7369 6f6e 5a0b 6c69 7374 5f6d 6f64  ersionZ.list_mod
-00004700: 656c 735a 1173 686f 775f 7365 6d61 6e74  elsZ.show_semant
-00004710: 7261 5f64 6972 7233 0000 005a 0a6d 6f64  ra_dirr3...Z.mod
-00004720: 656c 5f6e 616d 655a 1170 726f 6365 7373  el_nameZ.process
-00004730: 6564 5f77 696e 646f 7773 7252 0000 005a  ed_windowsrR...Z
-00004740: 0c6d 6f64 656c 5f63 6f6e 6669 6772 7500  .model_configru.
-00004750: 0000 da02 666e 5a03 6170 7072 a100 0000  ....fnZ.appr....
-00004760: 72a2 0000 0072 a900 0000 72be 0000 0072  r....r....r....r
-00004770: df00 0000 72e4 0000 0072 e600 0000 72ee  ....r....r....r.
-00004780: 0000 0072 ef00 0000 7221 0000 0072 2600  ...r....r!...r&.
-00004790: 0000 290e 72b9 0000 0072 9800 0000 7299  ..).r....r....r.
-000047a0: 0000 0072 9a00 0000 72dc 0000 0072 dd00  ...r....r....r..
-000047b0: 0000 729b 0000 0072 5e00 0000 72de 0000  ..r....r^...r...
-000047c0: 0072 ba00 0000 72bb 0000 0072 bc00 0000  .r....r....r....
-000047d0: 72bd 0000 0072 c300 0000 7227 0000 00da  r....r....r'....
-000047e0: 046d 6169 6e53 0100 0073 ae00 0000 007f  .mainS...s......
-000047f0: 004c 0401 0801 0402 0401 0801 1001 0402  .L..............
-00004800: 0801 0a02 0401 0801 0402 1401 0a02 0c02  ................
-00004810: 0802 0801 0402 0401 0201 0201 0201 0201  ................
-00004820: 0201 02fb 0809 0801 0801 0801 0801 0801  ................
-00004830: 0c01 0a03 0c01 0201 02ff 0405 0401 0c01  ................
-00004840: 0801 1401 0201 0201 0201 0201 0601 0201  ................
-00004850: 0201 0201 0201 0201 0201 0201 0201 02f3  ................
-00004860: 0e10 0401 0402 100e 0802 0801 0a07 0801  ................
-00004870: 0a06 0e01 0e0c 0e01 1a2a 0e01 1434 0e01  .........*...4..
-00004880: 1221 0e01 164b 0e01 0e06 0e01 0e08 0e01  .!...K..........
-00004890: 0e0d 0e01 0e08 0e01 0e04 0601 72f8 0000  ............r...
-000048a0: 00da 085f 5f6d 6169 6e5f 5f29 1b72 8900  ...__main__).r..
-000048b0: 0000 4672 8b00 0000 728c 0000 004e 4e4e  ..Fr....r....NNN
-000048c0: 4e4e 4e72 8500 0000 4e72 8e00 0000 728d  NNNr....Nr....r.
-000048d0: 0000 0054 4672 8f00 0000 7290 0000 0072  ...TFr....r....r
-000048e0: 9100 0000 7292 0000 0046 4646 4646 464e  ....r....FFFFFFN
-000048f0: 2943 7246 0000 0072 6100 0000 7202 0000  )CrF...ra...r...
-00004900: 005a 056e 756d 7079 726f 0000 005a 0566  .Z.numpyro...Z.f
-00004910: 6c61 736b 7203 0000 0072 0400 0000 7205  laskr....r....r.
-00004920: 0000 0072 0600 0000 7207 0000 0072 0800  ...r....r....r..
-00004930: 0000 726c 0000 0072 0a00 0000 720b 0000  ..rl...r....r...
-00004940: 0072 0c00 0000 720d 0000 0072 ea00 0000  .r....r....r....
-00004950: 72e5 0000 0072 0e00 0000 72c5 0000 0072  r....r....r....r
-00004960: 6600 0000 da04 7574 696c 720f 0000 0072  f.....utilr....r
-00004970: 1000 0000 7211 0000 0072 1200 0000 7213  ....r....r....r.
-00004980: 0000 0072 1400 0000 7215 0000 0072 1600  ...r....r....r..
-00004990: 0000 7217 0000 0072 1800 0000 7219 0000  ..r....r....r...
-000049a0: 0072 1a00 0000 721b 0000 0072 1c00 0000  .r....r....r....
-000049b0: 721d 0000 0072 9f00 0000 7230 0000 0072  r....r....r0...r
-000049c0: a000 0000 7236 0000 0072 3100 0000 da05  ....r6...r1.....
-000049d0: 7374 7269 7072 6b00 0000 7262 0000 00da  striprk...rb....
-000049e0: 0764 6972 6e61 6d65 da07 6162 7370 6174  .dirname..abspat
-000049f0: 68da 085f 5f66 696c 655f 5f5a 1170 6163  h..__file__Z.pac
-00004a00: 6b61 6765 5f64 6972 6563 746f 7279 7220  kage_directoryr 
-00004a10: 0000 0072 3700 0000 72f4 0000 0072 3800  ...r7...r....r8.
-00004a20: 0000 727a 0000 00da 0373 7472 7281 0000  ..rz.....strr...
-00004a30: 005a 0763 6f6d 6d61 6e64 5a08 6172 6775  .Z.commandZ.argu
-00004a40: 6d65 6e74 da04 5061 7468 da06 6f70 7469  ment..Path..opti
-00004a50: 6f6e 5a06 4368 6f69 6365 da04 6b65 7973  onZ.Choice..keys
-00004a60: 7280 0000 0072 b500 0000 72f8 0000 0072  r....r....r....r
-00004a70: 2900 0000 7226 0000 0072 2600 0000 7226  )...r&...r&...r&
-00004a80: 0000 0072 2700 0000 da08 3c6d 6f64 756c  ...r'.....<modul
-00004a90: 653e 0100 0000 73ce 0100 0008 0108 010c  e>....s.........
-00004aa0: 0108 0120 0108 0118 0108 010c 0108 0108  ... ............
-00004ab0: 0144 1108 0202 010c ff04 0202 012c 0214  .D...........,..
-00004ac0: 030e 0708 0904 030e 3b08 7f00 5110 0e06  ........;...Q...
-00004ad0: 0116 0104 0102 0110 0102 0102 0102 fb04  ................
-00004ae0: 0704 0102 0102 0102 fd04 0504 0102 0102  ................
-00004af0: 0102 0102 0102 fb04 0704 0102 0102 0102  ................
-00004b00: 0102 0102 fb04 0704 0102 0102 0102 0102  ................
-00004b10: 0102 fb04 0704 0102 0102 0102 0102 0102  ................
-00004b20: fb04 0704 0102 0102 0102 0102 fc04 0604  ................
-00004b30: 0102 0102 0102 0102 fc04 0604 0102 0102  ................
-00004b40: 0102 0102 fc04 0604 0102 0102 0102 0102  ................
-00004b50: fc04 0604 0102 0102 0102 0102 fc04 0604  ................
-00004b60: 0102 0102 0102 0102 fc04 0604 0102 0102  ................
-00004b70: 0102 0102 0102 fb04 0704 0102 0102 0102  ................
-00004b80: 0102 0102 fb04 0704 0102 0102 0102 0102  ................
-00004b90: 0102 fb04 0704 0102 0102 0102 0102 0102  ................
-00004ba0: fb04 0704 0102 0102 0102 0102 0102 fb04  ................
-00004bb0: 0704 0102 0102 0102 0102 0102 fb04 0704  ................
-00004bc0: 0102 0102 0102 0102 0102 fb04 0704 0102  ................
-00004bd0: 0102 0102 0102 0102 fb04 0704 0108 ff04  ................
-00004be0: 0304 0102 0102 0102 0102 fc04 0604 0102  ................
-00004bf0: 0102 0102 0102 fc04 0604 0102 0102 0102  ................
-00004c00: 0102 fc04 0604 0102 0102 0102 0102 fc04  ................
-00004c10: 0604 0102 0102 0102 0102 fc04 0604 0102  ................
-00004c20: 010a 0102 0102 fc04 0800 0100 0100 0100  ................
-00004c30: 0100 0100 0100 0100 0100 0100 0100 0100  ................
-00004c40: 0100 0100 0100 0100 0100 0100 0100 0100  ................
-00004c50: 0100 0100 0100 0100 0100 0100 0100 e444  ...............D
-00004c60: 7f00 7f00 7f00 150a 01                   .........
+00001fd0: 112d 2d71 7565 7279 2d74 6f6b 656e 2d70  .--query-token-p
+00001fe0: 7265 7a44 546f 6b65 6e20 746f 2070 7265  rezDToken to pre
+00001ff0: 7065 6e64 2074 6f20 6561 6368 2071 7565  pend to each que
+00002000: 7279 2069 6e20 7472 616e 7366 6f72 6d65  ry in transforme
+00002010: 7220 6d6f 6465 6c73 2028 6465 6661 756c  r models (defaul
+00002020: 743a 204e 6f6e 6529 7a12 2d2d 7175 6572  t: None)z.--quer
+00002030: 792d 746f 6b65 6e2d 706f 7374 7a43 546f  y-token-postzCTo
+00002040: 6b65 6e20 746f 2061 7070 656e 6420 746f  ken to append to
+00002050: 2065 6163 6820 7175 6572 7920 696e 2074   each query in t
+00002060: 7261 6e73 666f 726d 6572 206d 6f64 656c  ransformer model
+00002070: 7320 2864 6566 6175 6c74 3a20 4e6f 6e65  s (default: None
+00002080: 297a 0d2d 2d6e 756d 2d72 6573 756c 7473  )z.--num-results
+00002090: e90a 0000 007a 3e4e 756d 6265 7220 6f66  .....z>Number of
+000020a0: 2072 6573 756c 7473 2028 6e65 6967 6862   results (neighb
+000020b0: 6f72 7329 2074 6f20 7265 7472 6965 7665  ors) to retrieve
+000020c0: 2070 6572 2066 696c 6520 666f 7220 7175   per file for qu
+000020d0: 6572 6965 737a 072d 2d61 6e6e 6f79 7a7c  eriesz.--annoyz|
+000020e0: 5573 6520 6170 7072 6f78 696d 6174 6520  Use approximate 
+000020f0: 6b4e 4e20 7669 6120 416e 6e6f 7920 666f  kNN via Annoy fo
+00002100: 7220 7175 6572 6965 7320 2866 6173 7465  r queries (faste
+00002110: 7220 7175 6572 7969 6e67 2061 7420 6120  r querying at a 
+00002120: 736c 6967 6874 2063 6f73 7420 6f66 2061  slight cost of a
+00002130: 6363 7572 6163 7929 3b20 6966 2066 616c  ccuracy); if fal
+00002140: 7365 2c20 7573 6520 6578 6163 7420 6578  se, use exact ex
+00002150: 6861 7573 7469 7665 206b 4e4e 7a11 2d2d  haustive kNNz.--
+00002160: 6e75 6d2d 616e 6e6f 792d 7472 6565 73e9  num-annoy-trees.
+00002170: 6400 0000 7a34 4e75 6d62 6572 206f 6620  d...z4Number of 
+00002180: 7472 6565 7320 746f 2075 7365 2066 6f72  trees to use for
+00002190: 2061 7070 726f 7869 6d61 7465 206b 4e4e   approximate kNN
+000021a0: 2076 6961 2041 6e6e 6f79 7a05 2d2d 7376   via Annoyz.--sv
+000021b0: 6d7a 5a55 7365 2053 564d 2069 6e73 7465  mzZUse SVM inste
+000021c0: 6164 206f 6620 616e 7920 6b69 6e64 206f  ad of any kind o
+000021d0: 6620 6b4e 4e20 666f 7220 7175 6572 6965  f kNN for querie
+000021e0: 7320 2873 6c6f 7765 7220 616e 6420 6f6e  s (slower and on
+000021f0: 6c79 2077 6f72 6b73 206f 6e20 7379 6d6d  ly works on symm
+00002200: 6574 7269 6320 6d6f 6465 6c73 297a 072d  etric models)z.-
+00002210: 2d73 766d 2d63 6700 0000 0000 00f0 3f7a  -svm-cg.......?z
+00002220: 4853 564d 2072 6567 756c 6172 697a 6174  HSVM regularizat
+00002230: 696f 6e20 7061 7261 6d65 7465 723b 2068  ion parameter; h
+00002240: 6967 6865 7220 7661 6c75 6573 2070 656e  igher values pen
+00002250: 616c 697a 6520 6d69 7370 7265 6469 6374  alize mispredict
+00002260: 696f 6e73 206d 6f72 657a 152d 2d65 7870  ions morez.--exp
+00002270: 6c61 696e 2d73 706c 6974 2d63 6f75 6e74  lain-split-count
+00002280: e909 0000 007a 404e 756d 6265 7220 6f66  .....z@Number of
+00002290: 2073 706c 6974 7320 6f6e 2061 2067 6976   splits on a giv
+000022a0: 656e 2077 696e 646f 7720 746f 2075 7365  en window to use
+000022b0: 2066 6f72 2065 7870 6c61 696e 696e 6720   for explaining 
+000022c0: 6120 7175 6572 797a 162d 2d65 7870 6c61  a queryz.--expla
+000022d0: 696e 2d73 706c 6974 2d64 6976 6964 65e9  in-split-divide.
+000022e0: 0600 0000 7a53 4661 6374 6f72 2074 6f20  ....zSFactor to 
+000022f0: 6469 7669 6465 2074 6865 2077 696e 646f  divide the windo
+00002300: 7720 7369 7a65 2062 7920 746f 2067 6574  w size by to get
+00002310: 2065 6163 6820 7370 6c69 7420 6c65 6e67   each split leng
+00002320: 7468 2066 6f72 2065 7870 6c61 696e 696e  th for explainin
+00002330: 6720 6120 7175 6572 797a 182d 2d6e 756d  g a queryz.--num
+00002340: 2d65 7870 6c61 696e 2d68 6967 686c 6967  -explain-highlig
+00002350: 6874 73e9 0200 0000 7a3b 4e75 6d62 6572  hts.....z;Number
+00002360: 206f 6620 7370 6c69 7420 7265 7375 6c74   of split result
+00002370: 7320 746f 2068 6967 686c 6967 6874 2066  s to highlight f
+00002380: 6f72 2065 7870 6c61 696e 696e 6720 6120  or explaining a 
+00002390: 7175 6572 797a 072d 2d66 6f72 6365 7a1c  queryz.--forcez.
+000023a0: 466f 7263 6520 7072 6f63 6573 7320 6576  Force process ev
+000023b0: 656e 2069 6620 6361 6368 6564 2903 7287  en if cached).r.
+000023c0: 0000 0072 8400 0000 7286 0000 007a 082d  ...r....r....z.-
+000023d0: 2d73 696c 656e 747a 2144 6f20 6e6f 7420  -silentz!Do not 
+000023e0: 7072 696e 7420 7072 6f67 7265 7373 2069  print progress i
+000023f0: 6e66 6f72 6d61 7469 6f6e 7a0c 2d2d 6e6f  nformationz.--no
+00002400: 2d63 6f6e 6669 726d 7a47 446f 206e 6f74  -confirmzGDo not
+00002410: 2073 686f 7720 636f 7374 2061 6e64 2061   show cost and a
+00002420: 736b 2066 6f72 2063 6f6e 6669 726d 6174  sk for confirmat
+00002430: 696f 6e20 6265 666f 7265 2070 726f 6365  ion before proce
+00002440: 7373 696e 6720 7769 7468 204f 7065 6e41  ssing with OpenA
+00002450: 497a 092d 2d76 6572 7369 6f6e 7a16 5072  Iz.--versionz.Pr
+00002460: 696e 7420 7665 7273 696f 6e20 616e 6420  int version and 
+00002470: 6578 6974 7a0d 2d2d 6c69 7374 2d6d 6f64  exitz.--list-mod
+00002480: 656c 737a 1b4c 6973 7420 7072 6573 6574  elsz.List preset
+00002490: 206d 6f64 656c 7320 616e 6420 6578 6974   models and exit
+000024a0: 7a13 2d2d 7368 6f77 2d73 656d 616e 7472  z.--show-semantr
+000024b0: 612d 6469 727a 4750 7269 6e74 2074 6865  a-dirzGPrint the
+000024c0: 2064 6972 6563 746f 7279 2073 656d 616e   directory seman
+000024d0: 7472 6120 7769 6c6c 2075 7365 2074 6f20  tra will use to 
+000024e0: 7374 6f72 6520 7072 6f63 6573 7365 6420  store processed 
+000024f0: 6669 6c65 7320 616e 6420 6578 6974 7a0e  files and exitz.
+00002500: 2d2d 7365 6d61 6e74 7261 2d64 6972 7a24  --semantra-dirz$
+00002510: 4469 7265 6374 6f72 7920 746f 2073 746f  Directory to sto
+00002520: 7265 2073 656d 616e 7472 6120 6669 6c65  re semantra file
+00002530: 7320 696e 631d 0000 0000 0000 0000 0000  s inc...........
+00002540: 0031 0000 0011 0000 0003 0000 0073 5c03  .1...........s\.
+00002550: 0000 7c19 7210 7400 7401 8301 0100 6400  ..|.r.t.t.....d.
+00002560: 5300 7c1a 7230 7402 4400 5d12 7d1d 7400  S.|.r0t.D.].}.t.
+00002570: 6401 7c1d 9b00 9d02 8301 0100 7118 6400  d.|.........q.d.
+00002580: 5300 7c1c 6400 7500 7242 7403 a004 6402  S.|.d.u.rBt...d.
+00002590: a101 7d1c 7c1b 7252 7400 7c1c 8301 0100  ..}.|.rRt.|.....
+000025a0: 6400 5300 7405 6a06 a007 7c1c 6403 a102  d.S.t.j...|.d...
+000025b0: 7d1e 7408 7c1e 8301 0100 7c00 6400 7500  }.t.|.....|.d.u.
+000025c0: 737c 7409 7c00 8301 6404 6b02 7286 7403  s|t.|...d.k.r.t.
+000025d0: a00a 6405 a101 8201 740b 740c 7c01 8301  ..d.....t.t.|...
+000025e0: 8301 7d1f 7c0c 6400 7501 72be 7c05 6400  ..}.|.d.u.r.|.d.
+000025f0: 7500 72a6 740d 7d05 6400 7d20 740e 7c0c  u.r.t.}.d.} t.|.
+00002600: 7c07 7c08 7c09 7c0a 6406 8d05 8907 6e3e  |.|.|.|.d.....n>
+00002610: 7402 8807 1900 7d21 7c21 6407 1900 7d20  t.....}!|!d...} 
+00002620: 7c05 6400 7500 72de 7c21 6408 1900 7d05  |.d.u.r.|!d...}.
+00002630: 7c06 6400 7500 72f2 7c21 a00f 6409 6400  |.d.u.r.|!..d.d.
+00002640: a102 7d06 7c21 640a 1900 8300 8907 880c  ..}.|!d.........
+00002650: 9001 7214 8807 a010 a100 9001 7214 7411  ..r.........r.t.
+00002660: 640b 8301 8201 6900 8903 7412 7c00 7c17  d.....i...t.|.|.
+00002670: 640c 8d02 7d22 7c22 4400 5d46 7d23 7c22  d...}"|"D.]F}#|"
+00002680: a013 7405 6a06 a014 7c23 a101 9b00 a101  ..t.j...|#......
+00002690: 0100 7415 7c23 7c1c 8807 8807 a016 a100  ..t.|#|.........
+000026a0: 8800 7c0e 7c1f 7c20 7c06 7c05 7c16 7c17  ..|.|.| |.|.|.|.
+000026b0: 7c18 7c0d 640d 8d0e 8803 7c23 3c00 9001  |.|.d.....|#<...
+000026c0: 7128 6400 8901 6400 8902 8701 8702 8703  q(d...d.........
+000026d0: 6603 640e 640f 8408 8906 7417 7418 8301  f.d.d.....t.t...
+000026e0: 7d24 7c24 a019 6410 a101 6411 6412 8400  }$|$..d...d.d...
+000026f0: 8301 7d25 7c24 a019 6413 a101 6414 6415  ..}%|$..d...d.d.
+00002700: 8400 8301 7d26 7c24 6a19 6416 6417 6701  ....}&|$j.d.d.g.
+00002710: 6418 8d02 8703 6601 6419 641a 8408 8301  d.....f.d.d.....
+00002720: 7d27 7c24 6a19 641b 641c 6701 6418 8d02  }'|$j.d.d.g.d...
+00002730: 8700 8703 8707 8709 870a 870b 870c 6607  ..............f.
+00002740: 641d 641e 8408 8301 7d28 7c24 6a19 641f  d.d.....}(|$j.d.
+00002750: 641c 6701 6418 8d02 8703 8707 8709 870d  d.g.d...........
+00002760: 6604 6420 6421 8408 8301 890b 7c24 6a19  f.d d!......|$j.
+00002770: 6422 641c 6701 6418 8d02 8703 8707 8709  d"d.g.d.........
+00002780: 6603 6423 6424 8408 8301 890a 7c24 6a19  f.d#d$......|$j.
+00002790: 6425 641c 6701 6418 8d02 8703 8704 8705  d%d.g.d.........
+000027a0: 8707 8708 6605 6426 6427 8408 8301 7d29  ....f.d&d'....})
+000027b0: 7c24 6a19 6428 6417 6701 6418 8d02 8706  |$j.d(d.g.d.....
+000027c0: 6601 6429 642a 8408 8301 7d2a 7c24 6a19  f.d)d*....}*|$j.
+000027d0: 642b 6417 6701 6418 8d02 8706 6601 642c  d+d.g.d.....f.d,
+000027e0: 642d 8408 8301 7d2b 7c24 6a19 642e 6417  d-....}+|$j.d.d.
+000027f0: 6701 6418 8d02 8706 6601 642f 6430 8408  g.d.....f.d/d0..
+00002800: 8301 7d2c 7c24 6a19 6431 6417 6701 6418  ..},|$j.d1d.g.d.
+00002810: 8d02 8706 6601 6432 6433 8408 8301 7d2d  ....f.d2d3....}-
+00002820: 7c24 6a19 6434 6417 6701 6418 8d02 8703  |$j.d4d.g.d.....
+00002830: 6601 6435 6436 8408 8301 7d2e 7c02 9003  f.d5d6....}.|...
+00002840: 7358 7a12 7c24 6a1a 7c04 7c03 6437 8d02  sXz.|$j.|.|.d7..
+00002850: 0100 5700 6e54 0400 741b 9003 7956 0100  ..W.nT..t...yV..
+00002860: 7d2f 0100 7a3a 6404 6400 6c1c 7d30 6404  }/..z:d.d.l.}0d.
+00002870: 7c30 5f1d 7c03 741e 6b02 9003 7238 741f  |0_.|.t.k...r8t.
+00002880: 6438 8301 6400 8202 6e0a 741f 6439 8301  d8..d...n.t.d9..
+00002890: 6400 8202 5700 5900 6400 7d2f 7e2f 6e0a  d...W.Y.d.}/~/n.
+000028a0: 6400 7d2f 7e2f 3000 3000 6400 5300 293a  d.}/~/0.0.d.S.):
+000028b0: 4e7a 022d 205a 0853 656d 616e 7472 617a  Nz.- Z.Semantraz
+000028c0: 042e 656e 7672 0100 0000 7a28 4d75 7374  ..envr....z(Must
+000028d0: 2070 726f 7669 6465 2061 2066 696c 656e   provide a filen
+000028e0: 616d 6520 746f 2070 726f 6365 7373 2f71  ame to process/q
+000028f0: 7565 7279 2904 da0d 646f 635f 746f 6b65  uery)...doc_toke
+00002900: 6e5f 7072 65da 0e64 6f63 5f74 6f6b 656e  n_pre..doc_token
+00002910: 5f70 6f73 74da 0f71 7565 7279 5f74 6f6b  _post..query_tok
+00002920: 656e 5f70 7265 da10 7175 6572 795f 746f  en_pre..query_to
+00002930: 6b65 6e5f 706f 7374 7253 0000 0072 7400  ken_postrS...rt.
+00002940: 0000 7273 0000 005a 0967 6574 5f6d 6f64  ..rs...Z.get_mod
+00002950: 656c 7a52 5356 4d20 6973 206e 6f74 2063  elzRSVM is not c
+00002960: 6f6d 7061 7469 626c 6520 7769 7468 2061  ompatible with a
+00002970: 7379 6d6d 6574 7269 6320 6d6f 6465 6c73  symmetric models
+00002980: 2e20 506c 6561 7365 2075 7365 2061 2073  . Please use a s
+00002990: 796d 6d65 7472 6963 206d 6f64 656c 206f  ymmetric model o
+000029a0: 7220 6b4e 4e2e 2901 7259 0000 0029 0e72  r kNN.).rY...).r
+000029b0: 2300 0000 7234 0000 0072 5e00 0000 7244  #...r4...r^...rD
+000029c0: 0000 0072 3f00 0000 7256 0000 0072 4100  ...r?...rV...rA.
+000029d0: 0000 7253 0000 0072 7300 0000 7274 0000  ..rS...rs...rt..
+000029e0: 0072 3500 0000 7236 0000 0072 7500 0000  .r5...r6...ru...
+000029f0: 722e 0000 0063 0100 0000 0000 0000 0000  r....c..........
+00002a00: 0000 0200 0000 0200 0000 1300 0000 7322  ..............s"
+00002a10: 0000 007c 0088 016b 0272 0c88 0053 0088  ...|...k.r...S..
+00002a20: 027c 0019 006a 007d 017c 0089 017c 0189  .|...j.}.|...|..
+00002a30: 007c 0153 0072 3a00 0000 2901 7246 0000  .|.S.r:...).rF..
+00002a40: 00a9 0272 2300 0000 7246 0000 0029 03da  ...r#...rF...)..
+00002a50: 0e63 6163 6865 645f 636f 6e74 656e 74da  .cached_content.
+00002a60: 1763 6163 6865 645f 636f 6e74 656e 745f  .cached_content_
+00002a70: 6669 6c65 6e61 6d65 da09 646f 6375 6d65  filename..docume
+00002a80: 6e74 7372 2600 0000 7227 0000 00da 0b67  ntsr&...r'.....g
+00002a90: 6574 5f63 6f6e 7465 6e74 7f02 0000 730c  et_content....s.
+00002aa0: 0000 0000 0308 0104 020a 0204 0104 027a  ...............z
+00002ab0: 196d 6169 6e2e 3c6c 6f63 616c 733e 2e67  .main.<locals>.g
+00002ac0: 6574 5f63 6f6e 7465 6e74 fa01 2f63 0000  et_content../c..
+00002ad0: 0000 0000 0000 0000 0000 0000 0000 0500  ................
+00002ae0: 0000 5300 0000 7312 0000 0074 0074 01a0  ..S...s....t.t..
+00002af0: 0264 0164 02a1 0264 0383 0253 0029 044e  .d.d...d...S.).N
+00002b00: fa11 7365 6d61 6e74 7261 2e73 656d 616e  ..semantra.seman
+00002b10: 7472 61da 0d63 6c69 656e 745f 7075 626c  tra..client_publ
+00002b20: 6963 7a0a 696e 6465 782e 6874 6d6c a903  icz.index.html..
+00002b30: 7208 0000 00da 0d70 6b67 5f72 6573 6f75  r......pkg_resou
+00002b40: 7263 6573 5a11 7265 736f 7572 6365 5f66  rcesZ.resource_f
+00002b50: 696c 656e 616d 6572 2600 0000 7226 0000  ilenamer&...r&..
+00002b60: 0072 2600 0000 7227 0000 00da 0462 6173  .r&...r'.....bas
+00002b70: 658f 0200 0073 0800 0000 0002 0201 0a01  e....s..........
+00002b80: 02fe 7a12 6d61 696e 2e3c 6c6f 6361 6c73  ..z.main.<locals
+00002b90: 3e2e 6261 7365 7a0c 2f3c 7061 7468 3a70  >.basez./<path:p
+00002ba0: 6174 683e 6301 0000 0000 0000 0000 0000  ath>c...........
+00002bb0: 0001 0000 0005 0000 0053 0000 0073 1200  .........S...s..
+00002bc0: 0000 7400 7401 a002 6401 6402 a102 7c00  ..t.t...d.d...|.
+00002bd0: 8302 5300 2903 4e72 9700 0000 7298 0000  ..S.).Nr....r...
+00002be0: 0072 9900 0000 2901 7262 0000 0072 2600  .r....).rb...r&.
+00002bf0: 0000 7226 0000 0072 2700 0000 da04 686f  ..r&...r'.....ho
+00002c00: 6d65 9702 0000 7308 0000 0000 0202 010a  me....s.........
+00002c10: 0102 fe7a 126d 6169 6e2e 3c6c 6f63 616c  ...z.main.<local
+00002c20: 733e 2e68 6f6d 657a 0a2f 6170 692f 6669  s>.homez./api/fi
+00002c30: 6c65 735a 0347 4554 2901 da07 6d65 7468  lesZ.GET)...meth
+00002c40: 6f64 7363 0000 0000 0000 0000 0000 0000  odsc............
+00002c50: 0000 0000 0400 0000 1300 0000 7316 0000  ............s...
+00002c60: 0074 0064 0164 0284 0088 00a0 01a1 0044  .t.d.d.........D
+00002c70: 0083 0183 0153 0029 034e 6301 0000 0000  .....S.).Nc.....
+00002c80: 0000 0000 0000 0002 0000 0006 0000 0053  ...............S
+00002c90: 0000 0073 2000 0000 6700 7c00 5d18 7d01  ...s ...g.|.].}.
+00002ca0: 7c01 6a00 7c01 6a01 7c01 6a02 6a03 6400  |.j.|.j.|.j.j.d.
+00002cb0: 9c03 9102 7104 5300 2901 2903 7265 0000  ....q.S.).).re..
+00002cc0: 0072 2300 0000 7224 0000 0029 0472 3c00  .r#...r$...).r<.
+00002cd0: 0000 7223 0000 0072 4600 0000 7224 0000  ..r#...rF...r$..
+00002ce0: 0029 02da 022e 30da 0364 6f63 7226 0000  .)....0..docr&..
+00002cf0: 0072 2600 0000 7227 0000 00da 0a3c 6c69  .r&...r'.....<li
+00002d00: 7374 636f 6d70 3ea1 0200 0073 0a00 0000  stcomp>....s....
+00002d10: 0606 02fc 0401 0401 06fd 7a27 6d61 696e  ..........z'main
+00002d20: 2e3c 6c6f 6361 6c73 3e2e 6669 6c65 732e  .<locals>.files.
+00002d30: 3c6c 6f63 616c 733e 2e3c 6c69 7374 636f  <locals>.<listco
+00002d40: 6d70 3e29 0272 0400 0000 da06 7661 6c75  mp>).r......valu
+00002d50: 6573 7226 0000 00a9 0172 9400 0000 7226  esr&.....r....r&
+00002d60: 0000 0072 2700 0000 da05 6669 6c65 739e  ...r'.....files.
+00002d70: 0200 0073 0a00 0000 0002 0201 0606 06fa  ...s............
+00002d80: 04ff 7a13 6d61 696e 2e3c 6c6f 6361 6c73  ..z.main.<locals
+00002d90: 3e2e 6669 6c65 737a 0a2f 6170 692f 7175  >.filesz./api/qu
+00002da0: 6572 795a 0450 4f53 5463 0000 0000 0000  eryZ.POSTc......
+00002db0: 0000 0000 0000 0f00 0000 0c00 0000 1300  ................
+00002dc0: 0000 7312 0100 0074 006a 0164 0119 007d  ..s....t.j.d...}
+00002dd0: 0074 006a 0164 0219 007d 0188 0672 1e88  .t.j.d...}...r..
+00002de0: 0583 0053 0088 0072 2888 0483 0053 0088  ...S...r(....S..
+00002df0: 02a0 027c 007c 0188 01a1 037d 0267 007d  ...|.|.....}.g.}
+00002e00: 0388 01a0 03a1 0044 005d c07d 047c 046a  .......D.].}.|.j
+00002e10: 047d 0574 05a0 067c 057c 02a1 0274 056a  .}.t...|.|...t.j
+00002e20: 076a 087c 0564 0364 048d 0274 056a 07a0  .j.|.d.d...t.j..
+00002e30: 087c 02a1 0114 001b 007d 0674 05a0 097c  .|.......}.t...|
+00002e40: 060b 00a1 017d 077c 046a 0a7d 087c 046a  .....}.|.j.}.|.j
+00002e50: 0b64 0519 007d 0967 007d 0a7c 0764 0088  .d...}.g.}.|.d..
+00002e60: 0385 0219 0044 005d 507d 0b74 0c7c 067c  .....D.]P}.t.|.|
+00002e70: 0b19 0083 017d 0c7c 097c 0b19 007d 0d74  .....}.|.|...}.t
+00002e80: 0d7c 087c 0d64 0519 007c 0d64 0319 0085  .|.|.d...|.d....
+00002e90: 0219 0083 017d 0e7c 0aa0 0e7c 0e7c 0c7c  .....}.|...|.|.|
+00002ea0: 0d74 0f7c 0b83 017c 046a 107c 007c 0164  .t.|...|.j.|.|.d
+00002eb0: 069c 07a1 0101 0071 a07c 03a0 0e7c 046a  .......q.|...|.j
+00002ec0: 107c 0a67 02a1 0101 0071 4274 1174 127c  .|.g.....qBt.t.|
+00002ed0: 0364 0783 0283 0153 0029 084e da07 7175  .d.....S.).N..qu
+00002ee0: 6572 6965 73da 0b70 7265 6665 7265 6e63  eries..preferenc
+00002ef0: 6573 720a 0000 00a9 015a 0461 7869 7372  esr......Z.axisr
+00002f00: 0100 0000 a907 7221 0000 00da 0864 6973  ......r!.....dis
+00002f10: 7461 6e63 6572 7800 0000 da05 696e 6465  tancerx.....inde
+00002f20: 7872 2300 0000 72a4 0000 0072 a500 0000  xr#...r....r....
+00002f30: 5429 1372 0600 0000 7247 0000 00da 1d65  T).r....rG.....e
+00002f40: 6d62 6564 5f71 7565 7269 6573 5f61 6e64  mbed_queries_and
+00002f50: 5f70 7265 6665 7265 6e63 6573 72a1 0000  _preferencesr...
+00002f60: 0072 5000 0000 7270 0000 00da 0364 6f74  .rP...rp.....dot
+00002f70: da06 6c69 6e61 6c67 da04 6e6f 726d da07  ..linalg..norm..
+00002f80: 6172 6773 6f72 7472 4900 0000 7242 0000  argsortrI...rB..
+00002f90: 00da 0566 6c6f 6174 7219 0000 0072 6f00  ...floatr....ro.
+00002fa0: 0000 7280 0000 0072 2300 0000 7204 0000  ..r....r#...r...
+00002fb0: 0072 1c00 0000 290f 72a4 0000 0072 a500  .r....).r....r..
+00002fc0: 0000 725c 0000 0072 4f00 0000 729f 0000  ..r\...rO...r...
+00002fd0: 0072 5000 0000 da09 6469 7374 616e 6365  .rP.....distance
+00002fe0: 73da 0973 6f72 7465 645f 6978 7249 0000  s..sorted_ixrI..
+00002ff0: 0072 4200 0000 da0b 7375 625f 7265 7375  .rB.....sub_resu
+00003000: 6c74 7372 a900 0000 72a8 0000 0072 7800  ltsr....r....rx.
+00003010: 0000 7221 0000 0029 07da 0561 6e6e 6f79  ..r!...)...annoy
+00003020: 7294 0000 0072 5e00 0000 da0b 6e75 6d5f  r....r^.....num_
+00003030: 7265 7375 6c74 73da 0871 7565 7279 616e  results..queryan
+00003040: 6eda 0871 7565 7279 7376 6dda 0373 766d  n..querysvm..svm
+00003050: 7226 0000 0072 2700 0000 da05 7175 6572  r&...r'.....quer
+00003060: 79ab 0200 0073 4200 0000 0002 0a01 0a01  y....sB.........
+00003070: 0401 0601 0401 0603 0e02 0401 0c01 0603  ................
+00003080: 0a01 1aff 0403 0c02 0601 0a01 0401 1001  ................
+00003090: 0c01 0801 1801 0402 0201 0201 0201 0601  ................
+000030a0: 0401 0201 02f9 04ff 060b 1201 7a13 6d61  ............z.ma
+000030b0: 696e 2e3c 6c6f 6361 6c73 3e2e 7175 6572  in.<locals>.quer
+000030c0: 797a 0d2f 6170 692f 7175 6572 7973 766d  yz./api/querysvm
+000030d0: 6300 0000 0000 0000 0000 0000 0013 0000  c...............
+000030e0: 000c 0000 0013 0000 0073 3c01 0000 6401  .........s<...d.
+000030f0: 6402 6c00 6d01 7d00 0100 7402 6a03 6403  d.l.m.}...t.j.d.
+00003100: 1900 7d01 7402 6a03 6404 1900 7d02 8801  ..}.t.j.d...}...
+00003110: a004 7c01 7c02 8800 a103 7d03 6700 7d04  ..|.|.....}.g.}.
+00003120: 8800 a005 a100 4400 5df2 7d05 7c05 6a06  ......D.].}.|.j.
+00003130: 7d06 7407 a008 7c06 7c03 6405 1900 6702  }.t...|.|.d...g.
+00003140: a101 7d07 7407 a009 740a 7c06 8301 6406  ..}.t...t.|...d.
+00003150: 1700 a101 7d08 6406 7c08 6407 3c00 7c00  ....}.d.|.d.<.|.
+00003160: 6a0b 6408 6409 640a 640b 8803 640c 8d05  j.d.d.d.d...d...
+00003170: 7d09 7c09 a00c 7c07 7c08 a102 0100 7c09  }.|...|.|.....|.
+00003180: a00d 7c07 a101 6400 740a 7c06 8301 8502  ..|...d.t.|.....
+00003190: 1900 7d0a 7407 a00e 7c0a 0b00 a101 7d0b  ..}.t...|.....}.
+000031a0: 7c05 6a0f 7d0c 7c05 6a10 7d0d 6700 7d0e  |.j.}.|.j.}.g.}.
+000031b0: 7c0b 6400 8802 8502 1900 4400 5d4c 7d0f  |.d.......D.]L}.
+000031c0: 7c0a 7c0f 1900 7d10 7c0d 7c0f 1900 7d11  |.|...}.|.|...}.
+000031d0: 7411 7c0c 7c11 6401 1900 7c11 6406 1900  t.|.|.d...|.d...
+000031e0: 8502 1900 8301 7d12 7c0e a012 7c12 7c10  ......}.|...|.|.
+000031f0: 7c11 7413 7c0f 8301 7c05 6a14 7c01 7c02  |.t.|...|.j.|.|.
+00003200: 640d 9c07 a101 0100 71ce 7c04 a012 7c05  d.......q.|...|.
+00003210: 6a14 7c0e 6702 a101 0100 713a 7415 7416  j.|.g.....q:t.t.
+00003220: 7c04 640e 8302 8301 5300 290f 4e72 0100  |.d.....S.).Nr..
+00003230: 0000 2901 72b7 0000 0072 a400 0000 72a5  ..).r....r....r.
+00003240: 0000 0029 024e 2e72 0a00 0000 7282 0000  ...).N.r....r...
+00003250: 005a 0862 616c 616e 6365 6446 6910 2700  .Z.balancedFi.'.
+00003260: 0067 8ded b5a0 f7c6 b03e 2905 5a0c 636c  .g.......>).Z.cl
+00003270: 6173 735f 7765 6967 6874 da07 7665 7262  ass_weight..verb
+00003280: 6f73 655a 086d 6178 5f69 7465 725a 0374  oseZ.max_iterZ.t
+00003290: 6f6c da01 4372 a700 0000 5429 175a 0773  ol..Cr....T).Z.s
+000032a0: 6b6c 6561 726e 72b7 0000 0072 0600 0000  klearnr....r....
+000032b0: 7247 0000 0072 aa00 0000 72a1 0000 0072  rG...r....r....r
+000032c0: 5000 0000 7270 0000 005a 0b63 6f6e 6361  P...rp...Z.conca
+000032d0: 7465 6e61 7465 5a05 7a65 726f 7372 4b00  tenateZ.zerosrK.
+000032e0: 0000 5a09 4c69 6e65 6172 5356 435a 0366  ..Z.LinearSVCZ.f
+000032f0: 6974 5a11 6465 6369 7369 6f6e 5f66 756e  itZ.decision_fun
+00003300: 6374 696f 6e72 ae00 0000 7249 0000 0072  ctionr....rI...r
+00003310: 4200 0000 7219 0000 0072 6f00 0000 7280  B...r....ro...r.
+00003320: 0000 0072 2300 0000 7204 0000 0072 1c00  ...r#...r....r..
+00003330: 0000 2913 72b7 0000 0072 a400 0000 72a5  ..).r....r....r.
+00003340: 0000 0072 5c00 0000 724f 0000 0072 9f00  ...r\...rO...r..
+00003350: 0000 7250 0000 00da 0178 da01 795a 0363  ..rP.....x..yZ.c
+00003360: 6c66 5a0c 7369 6d69 6c61 7269 7469 6573  lfZ.similarities
+00003370: 72b1 0000 0072 4900 0000 7242 0000 0072  r....rI...rB...r
+00003380: b200 0000 72a9 0000 0072 a800 0000 7278  ....r....r....rx
+00003390: 0000 0072 2100 0000 2904 7294 0000 0072  ...r!...).r....r
+000033a0: 5e00 0000 72b4 0000 00da 0573 766d 5f63  ^...r......svm_c
+000033b0: 7226 0000 0072 2700 0000 72b6 0000 00d6  r&...r'...r.....
+000033c0: 0200 0073 4e00 0000 0002 0c02 0a01 0a03  ...sN...........
+000033d0: 0e01 0401 0c01 0602 1201 1201 0803 0401  ................
+000033e0: 0201 0201 0201 0201 02fb 0607 0c03 1601  ................
+000033f0: 0c02 0601 0601 0401 1001 0801 0801 1801  ................
+00003400: 0402 0201 0201 0201 0601 0401 0201 02f9  ................
+00003410: 04ff 060b 1202 7a16 6d61 696e 2e3c 6c6f  ......z.main.<lo
+00003420: 6361 6c73 3e2e 7175 6572 7973 766d 7a0d  cals>.querysvmz.
+00003430: 2f61 7069 2f71 7565 7279 616e 6e63 0000  /api/queryannc..
+00003440: 0000 0000 0000 0000 0000 0d00 0000 0c00  ................
+00003450: 0000 1300 0000 73d6 0000 0074 006a 0164  ......s....t.j.d
+00003460: 0119 007d 0074 006a 0164 0219 007d 0188  ...}.t.j.d...}..
+00003470: 01a0 027c 007c 0188 00a1 037d 0267 007d  ...|.|.....}.g.}
+00003480: 0388 00a0 03a1 0044 005d 987d 047c 046a  .......D.].}.|.j
+00003490: 047d 057c 046a 057d 067c 046a 0664 0319  .}.|.j.}.|.j.d..
+000034a0: 007d 0767 007d 0874 077c 05a0 087c 0288  .}.g.}.t.|...|..
+000034b0: 0264 0464 05a1 048e 0044 005d 545c 027d  .d.d.....D.]T\.}
+000034c0: 097d 0a7c 077c 0919 007d 0b74 097c 067c  .}.|.|...}.t.|.|
+000034d0: 0b64 0319 007c 0b64 0619 0085 0219 0083  .d...|.d........
+000034e0: 017d 0c7c 08a0 0a7c 0c64 067c 0a64 0713  .}.|...|.d.|.d..
+000034f0: 0064 071b 0018 007c 0b74 0b7c 0983 017c  .d.....|.t.|...|
+00003500: 046a 0c7c 007c 0164 089c 07a1 0101 0071  .j.|.|.d.......q
+00003510: 607c 03a0 0a7c 046a 0c7c 0867 02a1 0101  `|...|.j.|.g....
+00003520: 0071 2e74 0d74 0e7c 0364 0583 0283 0153  .q.t.t.|.d.....S
+00003530: 0029 094e 72a4 0000 0072 a500 0000 7201  .).Nr....r....r.
+00003540: 0000 0072 8200 0000 5472 0a00 0000 6700  ...r....Tr....g.
+00003550: 0000 0000 0000 4072 a700 0000 290f 7206  ......@r....).r.
+00003560: 0000 0072 4700 0000 72aa 0000 0072 a100  ...rG...r....r..
+00003570: 0000 724e 0000 0072 4900 0000 7242 0000  ..rN...rI...rB..
+00003580: 0072 6e00 0000 5a11 6765 745f 6e6e 735f  .rn...Z.get_nns_
+00003590: 6279 5f76 6563 746f 7272 1900 0000 726f  by_vectorr....ro
+000035a0: 0000 0072 8000 0000 7223 0000 0072 0400  ...r....r#...r..
+000035b0: 0000 721c 0000 0029 0d72 a400 0000 72a5  ..r....).r....r.
+000035c0: 0000 0072 5c00 0000 724f 0000 0072 9f00  ...r\...rO...r..
+000035d0: 0000 724e 0000 0072 4900 0000 7242 0000  ..rN...rI...rB..
+000035e0: 0072 b200 0000 72a9 0000 0072 a800 0000  .r....r....r....
+000035f0: 7278 0000 0072 2100 0000 2903 7294 0000  rx...r!...).r...
+00003600: 0072 5e00 0000 72b4 0000 0072 2600 0000  .r^...r....r&...
+00003610: 7227 0000 0072 b500 0000 0b03 0000 7334  r'...r........s4
+00003620: 0000 0000 020a 010a 030e 0204 010c 0106  ................
+00003630: 0106 010a 0104 0102 010e ff0c 0308 0118  ................
+00003640: 0104 0202 020e 0102 0106 0104 0102 0102  ................
+00003650: f804 ff06 0c12 017a 166d 6169 6e2e 3c6c  .......z.main.<l
+00003660: 6f63 616c 733e 2e71 7565 7279 616e 6e7a  ocals>.queryannz
+00003670: 0c2f 6170 692f 6578 706c 6169 6e63 0000  ./api/explainc..
+00003680: 0000 0000 0000 0000 0000 0900 0000 0600  ................
+00003690: 0000 1300 0000 73c0 0000 0074 006a 0164  ......s....t.j.d
+000036a0: 0119 007d 0074 006a 0164 0219 007d 0188  ...}.t.j.d...}..
+000036b0: 037c 0019 006a 027c 0164 0319 007c 0164  .|...j.|.d...|.d
+000036c0: 0419 0085 0219 0089 0274 006a 0164 0519  .........t.j.d..
+000036d0: 007d 0274 006a 0164 0619 007d 0388 06a0  .}.t.j.d...}....
+000036e0: 037c 027c 0388 03a1 0389 0064 0764 0864  .|.|.......d.d.d
+000036f0: 0374 0488 0283 0166 0464 0964 0a84 017d  .t.....f.d.d...}
+00003700: 0487 0266 0164 0b64 0c84 0889 0187 0087  ...f.d.d........
+00003710: 0187 0687 0266 0464 0d64 0e84 087d 0587  .....f.d.d...}..
+00003720: 0266 0164 0f64 1084 087d 067c 0488 0588  .f.d.d...}.|....
+00003730: 0464 0374 0488 0283 0164 118d 047d 077c  .d.t.....d...}.|
+00003740: 057c 0783 0164 0088 0785 0219 007d 0874  .|...d.......}.t
+00003750: 057c 067c 0883 0183 0153 0029 124e 7223  .|.|.....S.).Nr#
+00003760: 0000 0072 7800 0000 7201 0000 0072 0a00  ...rx...r....r..
+00003770: 0000 72a4 0000 0072 a500 0000 728c 0000  ..r....r....r...
+00003780: 00e9 0300 0000 6304 0000 0000 0000 0000  ......c.........
+00003790: 0000 0008 0000 0009 0000 0053 0000 0073  ...........S...s
+000037a0: 6200 0000 7400 a001 7c03 7c02 1800 7c00  b...t...|.|...|.
+000037b0: 1b00 a101 7d04 7400 a001 7c03 7c02 1800  ....}.t...|.|...
+000037c0: 7c01 1b00 a101 7d05 6700 7d06 7402 7c01  |.....}.g.}.t.|.
+000037d0: 8301 4400 5d2c 7d07 7c06 a003 7c02 7c07  ..D.],}.|...|.|.
+000037e0: 7c05 1400 1700 7404 7c03 7c02 7c07 7c05  |.....t.|.|.|.|.
+000037f0: 1400 1700 7c04 1700 8302 6602 a101 0100  ....|.....f.....
+00003800: 7130 7c06 5300 723a 0000 0029 05da 046d  q0|.S.r:...)...m
+00003810: 6174 685a 0463 6569 6cda 0572 616e 6765  athZ.ceil..range
+00003820: 726f 0000 00da 036d 696e 2908 da0d 6469  ro.....min)...di
+00003830: 7669 6465 5f66 6163 746f 72da 0a6e 756d  vide_factor..num
+00003840: 5f73 706c 6974 73da 0573 7461 7274 da03  _splits..start..
+00003850: 656e 645a 0d77 696e 646f 775f 6c65 6e67  endZ.window_leng
+00003860: 7468 5a0c 7370 6c69 745f 6c65 6e67 7468  thZ.split_length
+00003870: da06 7370 6c69 7473 da01 6972 2600 0000  ..splits..ir&...
+00003880: 7226 0000 0072 2700 0000 da0a 6765 745f  r&...r'.....get_
+00003890: 7370 6c69 7473 3703 0000 7314 0000 0000  splits7...s.....
+000038a0: 0112 0112 0104 010c 0104 020a 0114 fe02  ................
+000038b0: ff06 067a 296d 6169 6e2e 3c6c 6f63 616c  ...z)main.<local
+000038c0: 733e 2e65 7870 6c61 696e 2e3c 6c6f 6361  s>.explain.<loca
+000038d0: 6c73 3e2e 6765 745f 7370 6c69 7473 6302  ls>.get_splitsc.
+000038e0: 0000 0000 0000 0000 0000 0002 0000 0005  ................
+000038f0: 0000 0013 0000 0073 1c00 0000 7400 8800  .......s....t...
+00003900: 6400 7c00 8502 1900 8800 7c01 6400 8502  d.|.......|.d...
+00003910: 1900 1700 8301 5300 723a 0000 0029 0172  ......S.r:...).r
+00003920: 1900 0000 2902 72c4 0000 0072 c500 0000  ....).r....r....
+00003930: a901 725f 0000 0072 2600 0000 7227 0000  ..r_...r&...r'..
+00003940: 00da 0e65 7863 6c75 6465 5f77 696e 646f  ...exclude_windo
+00003950: 7744 0300 0073 0200 0000 0002 7a2d 6d61  wD...s......z-ma
+00003960: 696e 2e3c 6c6f 6361 6c73 3e2e 6578 706c  in.<locals>.expl
+00003970: 6169 6e2e 3c6c 6f63 616c 733e 2e65 7863  ain.<locals>.exc
+00003980: 6c75 6465 5f77 696e 646f 7763 0100 0000  lude_windowc....
+00003990: 0000 0000 0000 0000 0400 0000 0500 0000  ................
+000039a0: 1300 0000 7368 0000 0087 0166 0164 0164  ....sh.....f.d.d
+000039b0: 0284 087c 0044 0083 017d 0174 00a0 0187  ...|.D...}.t....
+000039c0: 0266 0164 0364 0284 087c 0144 0083 01a1  .f.d.d...|.D....
+000039d0: 017d 027c 02a0 0288 00a1 0174 006a 036a  .}.|.......t.j.j
+000039e0: 047c 0264 0464 058d 0274 006a 03a0 0488  .|.d.d...t.j....
+000039f0: 00a1 0114 001b 007d 0374 0574 067c 007c  .......}.t.t.|.|
+00003a00: 0383 0264 0664 0784 0064 0864 098d 0353  ...d.d...d.d...S
+00003a10: 0029 0a4e 6301 0000 0000 0000 0000 0000  .).Nc...........
+00003a20: 0003 0000 0005 0000 0013 0000 0073 1a00  .............s..
+00003a30: 0000 6700 7c00 5d12 5c02 7d01 7d02 8800  ..g.|.].\.}.}...
+00003a40: 7c01 7c02 8302 9102 7104 5300 7226 0000  |.|.....q.S.r&..
+00003a50: 0072 2600 0000 2903 729e 0000 0072 c400  .r&...).r....r..
+00003a60: 0000 72c5 0000 0029 0172 ca00 0000 7226  ..r....).r....r&
+00003a70: 0000 0072 2700 0000 72a0 0000 004a 0300  ...r'...r....J..
+00003a80: 00f3 0000 0000 7a4b 6d61 696e 2e3c 6c6f  ......zKmain.<lo
+00003a90: 6361 6c73 3e2e 6578 706c 6169 6e2e 3c6c  cals>.explain.<l
+00003aa0: 6f63 616c 733e 2e67 6574 5f68 6967 6865  ocals>.get_highe
+00003ab0: 7374 5f72 616e 6b65 645f 7370 6c69 742e  st_ranked_split.
+00003ac0: 3c6c 6f63 616c 733e 2e3c 6c69 7374 636f  <locals>.<listco
+00003ad0: 6d70 3e63 0100 0000 0000 0000 0000 0000  mp>c............
+00003ae0: 0200 0000 0600 0000 1300 0000 731a 0000  ............s...
+00003af0: 0067 007c 005d 127d 0174 0088 00a0 017c  .g.|.].}.t.....|
+00003b00: 01a1 0183 0191 0271 0453 0072 2600 0000  .......q.S.r&...
+00003b10: 2902 720d 0000 005a 0e65 6d62 6564 5f64  ).r....Z.embed_d
+00003b20: 6f63 756d 656e 7429 0272 9e00 0000 5a0b  ocument).r....Z.
+00003b30: 7370 6c69 745f 7175 6572 7929 0172 5e00  split_query).r^.
+00003b40: 0000 7226 0000 0072 2700 0000 72a0 0000  ..r&...r'...r...
+00003b50: 004c 0300 0073 0400 0000 0602 02ff 720a  .L...s........r.
+00003b60: 0000 0072 a600 0000 6301 0000 0000 0000  ...r....c.......
+00003b70: 0000 0000 0001 0000 0002 0000 0053 0000  .............S..
+00003b80: 0073 0800 0000 7c00 6401 1900 5300 2902  .s....|.d...S.).
+00003b90: 4e72 0a00 0000 7226 0000 00a9 0172 bb00  Nr....r&.....r..
+00003ba0: 0000 7226 0000 0072 2600 0000 7227 0000  ..r&...r&...r'..
+00003bb0: 00da 083c 6c61 6d62 6461 3e55 0300 0072  ...<lambda>U...r
+00003bc0: cb00 0000 7a49 6d61 696e 2e3c 6c6f 6361  ....zImain.<loca
+00003bd0: 6c73 3e2e 6578 706c 6169 6e2e 3c6c 6f63  ls>.explain.<loc
+00003be0: 616c 733e 2e67 6574 5f68 6967 6865 7374  als>.get_highest
+00003bf0: 5f72 616e 6b65 645f 7370 6c69 742e 3c6c  _ranked_split.<l
+00003c00: 6f63 616c 733e 2e3c 6c61 6d62 6461 3e46  ocals>.<lambda>F
+00003c10: 2902 da03 6b65 79da 0772 6576 6572 7365  )...key..reverse
+00003c20: 2907 7270 0000 005a 0561 7272 6179 72ab  ).rp...Z.arrayr.
+00003c30: 0000 0072 ac00 0000 72ad 0000 00da 0673  ...r....r......s
+00003c40: 6f72 7465 6472 6e00 0000 2904 72c6 0000  ortedrn...).r...
+00003c50: 005a 0d73 706c 6974 5f71 7565 7269 6573  .Z.split_queries
+00003c60: 5a0d 7370 6c69 745f 7769 6e64 6f77 7372  Z.split_windowsr
+00003c70: b000 0000 2904 725c 0000 0072 ca00 0000  ....).r\...r....
+00003c80: 725e 0000 0072 5f00 0000 7226 0000 0072  r^...r_...r&...r
+00003c90: 2700 0000 da18 6765 745f 6869 6768 6573  '.....get_highes
+00003ca0: 745f 7261 6e6b 6564 5f73 706c 6974 4803  t_ranked_splitH.
+00003cb0: 0000 7314 0000 0000 0212 0104 010a 0202  ..s.............
+00003cc0: fe04 ff04 0608 011a ff04 047a 376d 6169  ...........z7mai
+00003cd0: 6e2e 3c6c 6f63 616c 733e 2e65 7870 6c61  n.<locals>.expla
+00003ce0: 696e 2e3c 6c6f 6361 6c73 3e2e 6765 745f  in.<locals>.get_
+00003cf0: 6869 6768 6573 745f 7261 6e6b 6564 5f73  highest_ranked_s
+00003d00: 706c 6974 6301 0000 0000 0000 0000 0000  plitc...........
+00003d10: 0005 0000 0005 0000 0013 0000 0073 8000  .............s..
+00003d20: 0000 7400 6401 6402 8400 7c00 4400 8301  ..t.d.d...|.D...
+00003d30: 6403 6404 8400 6405 8d02 7d01 6406 7d02  d.d...d...}.d.}.
+00003d40: 6700 8900 8700 8701 6602 6407 6408 8408  g.......f.d.d...
+00003d50: 7d03 7c01 4400 5d36 7d04 7c03 7c02 7c04  }.|.D.]6}.|.|.|.
+00003d60: 6406 1900 6409 8303 0100 7c03 7401 7c04  d...d.....|.t.|.
+00003d70: 6406 1900 7c02 8302 7c04 640a 1900 640b  d...|...|.d...d.
+00003d80: 8303 0100 7c04 640a 1900 7d02 7134 7c03  ....|.d...}.q4|.
+00003d90: 7c02 7402 8801 8301 6409 8303 0100 8800  |.t.....d.......
+00003da0: 5300 290c 4e63 0100 0000 0000 0000 0000  S.).Nc..........
+00003db0: 0000 0200 0000 0400 0000 5300 0000 7314  ..........S...s.
+00003dc0: 0000 0067 007c 005d 0c7d 017c 0164 0019  ...g.|.].}.|.d..
+00003dd0: 0091 0271 0453 0029 0172 0100 0000 7226  ...q.S.).r....r&
+00003de0: 0000 0029 0272 9e00 0000 727e 0000 0072  ...).r....r~...r
+00003df0: 2600 0000 7226 0000 0072 2700 0000 72a0  &...r&...r'...r.
+00003e00: 0000 0059 0300 0072 cb00 0000 7a3c 6d61  ...Y...r....z<ma
+00003e10: 696e 2e3c 6c6f 6361 6c73 3e2e 6578 706c  in.<locals>.expl
+00003e20: 6169 6e2e 3c6c 6f63 616c 733e 2e61 735f  ain.<locals>.as_
+00003e30: 746f 6b65 6e73 2e3c 6c6f 6361 6c73 3e2e  tokens.<locals>.
+00003e40: 3c6c 6973 7463 6f6d 703e 6301 0000 0000  <listcomp>c.....
+00003e50: 0000 0000 0000 0001 0000 0002 0000 0053  ...............S
+00003e60: 0000 0073 0800 0000 7c00 6401 1900 5300  ...s....|.d...S.
+00003e70: 724a 0000 0072 2600 0000 72cc 0000 0072  rJ...r&...r....r
+00003e80: 2600 0000 7226 0000 0072 2700 0000 72cd  &...r&...r'...r.
+00003e90: 0000 0059 0300 0072 cb00 0000 7a3a 6d61  ...Y...r....z:ma
+00003ea0: 696e 2e3c 6c6f 6361 6c73 3e2e 6578 706c  in.<locals>.expl
+00003eb0: 6169 6e2e 3c6c 6f63 616c 733e 2e61 735f  ain.<locals>.as_
+00003ec0: 746f 6b65 6e73 2e3c 6c6f 6361 6c73 3e2e  tokens.<locals>.
+00003ed0: 3c6c 616d 6264 613e 2901 72ce 0000 0072  <lambda>).r....r
+00003ee0: 0100 0000 6303 0000 0000 0000 0000 0000  ....c...........
+00003ef0: 0003 0000 0006 0000 0013 0000 0073 2c00  .............s,.
+00003f00: 0000 7c00 7c01 6b05 720c 6400 5300 8800  ..|.|.k.r.d.S...
+00003f10: a000 7401 8801 7c00 7c01 8502 1900 8301  ..t...|.|.......
+00003f20: 7c02 6401 9c02 a101 0100 6400 5300 2902  |.d.......d.S.).
+00003f30: 4e29 0272 2100 0000 7283 0000 0029 0272  N).r!...r....).r
+00003f40: 6f00 0000 7219 0000 0029 0372 c400 0000  o...r....).r....
+00003f50: 72c5 0000 0072 8300 0000 2902 da06 6368  r....r....)...ch
+00003f60: 756e 6b73 725f 0000 0072 2600 0000 7227  unksr_...r&...r'
+00003f70: 0000 0072 6f00 0000 5d03 0000 730e 0000  ...ro...]...s...
+00003f80: 0000 0108 0104 0204 020e 0102 fe04 ff7a  ...............z
+00003f90: 386d 6169 6e2e 3c6c 6f63 616c 733e 2e65  8main.<locals>.e
+00003fa0: 7870 6c61 696e 2e3c 6c6f 6361 6c73 3e2e  xplain.<locals>.
+00003fb0: 6173 5f74 6f6b 656e 732e 3c6c 6f63 616c  as_tokens.<local
+00003fc0: 733e 2e61 7070 656e 645a 066e 6f72 6d61  s>.appendZ.norma
+00003fd0: 6c72 0a00 0000 5a09 6869 6768 6c69 6768  lr....Z.highligh
+00003fe0: 7429 0372 d000 0000 da03 6d61 7872 4b00  t).r......maxrK.
+00003ff0: 0000 2905 72c6 0000 00da 0769 6e64 6963  ..).r......indic
+00004000: 6573 5a0a 6c61 7374 5f69 6e64 6578 726f  esZ.last_indexro
+00004010: 0000 0072 a900 0000 72c9 0000 0029 0172  ...r....r....).r
+00004020: d200 0000 7227 0000 00da 0961 735f 746f  ....r'.....as_to
+00004030: 6b65 6e73 5703 0000 7314 0000 0000 021a  kensW...s.......
+00004040: 0104 0104 020e 0b08 0110 011a 010a 0210  ................
+00004050: 017a 286d 6169 6e2e 3c6c 6f63 616c 733e  .z(main.<locals>
+00004060: 2e65 7870 6c61 696e 2e3c 6c6f 6361 6c73  .explain.<locals
+00004070: 3e2e 6173 5f74 6f6b 656e 7329 0472 c200  >.as_tokens).r..
+00004080: 0000 72c3 0000 0072 c400 0000 72c5 0000  ..r....r....r...
+00004090: 0029 0672 0600 0000 7247 0000 0072 4900  .).r....rG...rI.
+000040a0: 0000 72aa 0000 0072 4b00 0000 7204 0000  ..r....rK...r...
+000040b0: 0029 0972 2300 0000 7278 0000 0072 a400  .).r#...rx...r..
+000040c0: 0000 72a5 0000 0072 c800 0000 72d1 0000  ..r....r....r...
+000040d0: 0072 d500 0000 72c6 0000 005a 0a74 6f70  .r....r....Z.top
+000040e0: 5f73 706c 6974 7329 0572 9400 0000 da13  _splits).r......
+000040f0: 6578 706c 6169 6e5f 7370 6c69 745f 636f  explain_split_co
+00004100: 756e 74da 1465 7870 6c61 696e 5f73 706c  unt..explain_spl
+00004110: 6974 5f64 6976 6964 6572 5e00 0000 da16  it_divider^.....
+00004120: 6e75 6d5f 6578 706c 6169 6e5f 6869 6768  num_explain_high
+00004130: 6c69 6768 7473 2903 725c 0000 0072 ca00  lights).r\...r..
+00004140: 0000 725f 0000 0072 2700 0000 da07 6578  ..r_...r'.....ex
+00004150: 706c 6169 6e2d 0300 0073 2400 0000 0002  plain-...s$.....
+00004160: 0a01 0a01 1a01 0a01 0a01 0e03 160d 0c04  ................
+00004170: 120f 0c19 0201 0201 0201 0201 06fc 0606  ................
+00004180: 1001 7a15 6d61 696e 2e3c 6c6f 6361 6c73  ..z.main.<locals
+00004190: 3e2e 6578 706c 6169 6e7a 0c2f 6170 692f  >.explainz./api/
+000041a0: 6765 7466 696c 6563 0000 0000 0000 0000  getfilec........
+000041b0: 0000 0000 0200 0000 0300 0000 1300 0000  ................
+000041c0: 7322 0000 0074 006a 01a0 0264 01a1 017d  s"...t.j...d...}
+000041d0: 0088 007c 0083 017d 017c 016a 037d 0074  ...|...}.|.j.}.t
+000041e0: 047c 0083 0153 00a9 024e 7223 0000 0029  .|...S...Nr#...)
+000041f0: 0572 0600 0000 da04 6172 6773 da03 6765  .r......args..ge
+00004200: 7472 2300 0000 7207 0000 0072 9100 0000  tr#...r....r....
+00004210: a901 7295 0000 0072 2600 0000 7227 0000  ..r....r&...r'..
+00004220: 00da 0767 6574 6669 6c65 7903 0000 7308  ...getfiley...s.
+00004230: 0000 0000 020c 0108 0106 017a 156d 6169  ...........z.mai
+00004240: 6e2e 3c6c 6f63 616c 733e 2e67 6574 6669  n.<locals>.getfi
+00004250: 6c65 7a11 2f61 7069 2f70 6466 706f 7369  lez./api/pdfposi
+00004260: 7469 6f6e 7363 0000 0000 0000 0000 0000  tionsc..........
+00004270: 0000 0200 0000 0300 0000 1300 0000 7334  ..............s4
+00004280: 0000 0074 006a 01a0 0264 01a1 017d 0088  ...t.j...d...}..
+00004290: 007c 0083 017d 017c 016a 0364 026b 0272  .|...}.|.j.d.k.r
+000042a0: 2874 047c 016a 0583 0153 0074 0467 0083  (t.|.j...S.t.g..
+000042b0: 0153 0064 0053 0029 034e 7223 0000 00da  .S.d.S.).Nr#....
+000042c0: 0370 6466 2906 7206 0000 0072 db00 0000  .pdf).r....r....
+000042d0: 72dc 0000 0072 2400 0000 7204 0000 005a  r....r$...r....Z
+000042e0: 0970 6f73 6974 696f 6e73 7291 0000 0072  .positionsr....r
+000042f0: dd00 0000 7226 0000 0072 2700 0000 da0c  ....r&...r'.....
+00004300: 7064 6670 6f73 6974 696f 6e73 8003 0000  pdfpositions....
+00004310: 730a 0000 0000 020c 0108 010a 010a 027a  s..............z
+00004320: 1a6d 6169 6e2e 3c6c 6f63 616c 733e 2e70  .main.<locals>.p
+00004330: 6466 706f 7369 7469 6f6e 737a 0c2f 6170  dfpositionsz./ap
+00004340: 692f 7064 6670 6167 6563 0000 0000 0000  i/pdfpagec......
+00004350: 0000 0000 0000 0700 0000 0500 0000 1300  ................
+00004360: 0000 7382 0000 0074 006a 01a0 0264 01a1  ..s....t.j...d..
+00004370: 017d 0088 007c 0083 017d 0174 006a 01a0  .}...|...}.t.j..
+00004380: 0264 02a1 017d 0274 006a 01a0 0264 03a1  .d...}.t.j...d..
+00004390: 017d 037c 016a 0364 046b 0272 7e7c 01a0  .}.|.j.d.k.r~|..
+000043a0: 0474 057c 0283 0174 067c 0383 01a1 027d  .t.|...t.|.....}
+000043b0: 0474 07a0 08a1 007d 057c 046a 097c 0564  .t.....}.|.j.|.d
+000043c0: 0564 068d 0201 0074 0a7c 05a0 0ba1 0083  .d.....t.|......
+000043d0: 017d 067c 066a 0ca0 0d64 0764 08a1 0201  .}.|.j...d.d....
+000043e0: 007c 0653 0064 0053 0029 094e 7223 0000  .|.S.d.S.).Nr#..
+000043f0: 00da 0470 6167 65da 0573 6361 6c65 72df  ...page..scaler.
+00004400: 0000 005a 0350 4e47 2901 da06 666f 726d  ...Z.PNG)...form
+00004410: 6174 7a0c 436f 6e74 656e 742d 5479 7065  atz.Content-Type
+00004420: 7a09 696d 6167 652f 706e 6729 0e72 0600  z.image/png).r..
+00004430: 0000 72db 0000 0072 dc00 0000 7224 0000  ..r....r....r$..
+00004440: 005a 1267 6574 5f70 6167 655f 696d 6167  .Z.get_page_imag
+00004450: 655f 7069 6c72 8000 0000 72af 0000 00da  e_pilr....r.....
+00004460: 0269 6fda 0742 7974 6573 494f 5a04 7361  .io..BytesIOZ.sa
+00004470: 7665 7205 0000 00da 0867 6574 7661 6c75  ver......getvalu
+00004480: 655a 0768 6561 6465 7273 da03 7365 7429  eZ.headers..set)
+00004490: 0772 2300 0000 7246 0000 0072 e100 0000  .r#...rF...r....
+000044a0: 72e2 0000 005a 0970 696c 5f69 6d61 6765  r....Z.pil_image
+000044b0: 5a0c 696d 675f 6279 7465 5f61 7272 5a08  Z.img_byte_arrZ.
+000044c0: 7265 7370 6f6e 7365 72dd 0000 0072 2600  responser....r&.
+000044d0: 0000 7227 0000 00da 0770 6466 7061 6765  ..r'.....pdfpage
+000044e0: 8903 0000 7316 0000 0000 020c 0108 010c  ....s...........
+000044f0: 010c 010a 0114 0108 010e 010c 010e 017a  ...............z
+00004500: 156d 6169 6e2e 3c6c 6f63 616c 733e 2e70  .main.<locals>.p
+00004510: 6466 7061 6765 7a0d 2f61 7069 2f70 6466  dfpagez./api/pdf
+00004520: 6368 6172 7363 0000 0000 0000 0000 0000  charsc..........
+00004530: 0000 0300 0000 0500 0000 1300 0000 7344  ..............sD
+00004540: 0000 0074 006a 01a0 0264 01a1 017d 0088  ...t.j...d...}..
+00004550: 007c 0083 017d 017c 016a 0364 026b 0372  .|...}.|.j.d.k.r
+00004560: 2674 0467 0083 0153 0074 006a 01a0 0264  &t.g...S.t.j...d
+00004570: 03a1 017d 0274 047c 01a0 0574 067c 0283  ...}.t.|...t.|..
+00004580: 01a1 0183 0153 0029 044e 7223 0000 0072  .....S.).Nr#...r
+00004590: df00 0000 72e1 0000 0029 0772 0600 0000  ....r....).r....
+000045a0: 72db 0000 0072 dc00 0000 7224 0000 0072  r....r....r$...r
+000045b0: 0400 0000 5a0e 6765 745f 7061 6765 5f63  ....Z.get_page_c
+000045c0: 6861 7273 7280 0000 0029 0372 2300 0000  harsr....).r#...
+000045d0: 7246 0000 0072 e100 0000 72dd 0000 0072  rF...r....r....r
+000045e0: 2600 0000 7227 0000 00da 0870 6466 6368  &...r'.....pdfch
+000045f0: 6172 7397 0300 0073 0c00 0000 0002 0c01  ars....s........
+00004600: 0801 0a01 0801 0c01 7a16 6d61 696e 2e3c  ........z.main.<
+00004610: 6c6f 6361 6c73 3e2e 7064 6663 6861 7273  locals>.pdfchars
+00004620: 7a09 2f61 7069 2f74 6578 7463 0000 0000  z./api/textc....
+00004630: 0000 0000 0000 0000 0100 0000 0300 0000  ................
+00004640: 1300 0000 731a 0000 0074 006a 01a0 0264  ....s....t.j...d
+00004650: 01a1 017d 0074 0388 007c 0019 006a 0483  ...}.t...|...j..
+00004660: 0153 0072 da00 0000 2905 7206 0000 0072  .S.r....).r....r
+00004670: db00 0000 72dc 0000 0072 0400 0000 7249  ....r....r....rI
+00004680: 0000 0029 0172 2300 0000 72a2 0000 0072  ...).r#...r....r
+00004690: 2600 0000 7227 0000 0072 2100 0000 a003  &...r'...r!.....
+000046a0: 0000 7304 0000 0000 020c 017a 126d 6169  ..s........z.mai
+000046b0: 6e2e 3c6c 6f63 616c 733e 2e74 6578 7429  n.<locals>.text)
+000046c0: 02da 0468 6f73 74da 0470 6f72 747a 5854  ...host..portzXT
+000046d0: 7279 2072 756e 6e69 6e67 2061 6761 696e  ry running again
+000046e0: 2061 6e64 2061 6464 696e 6720 602d 2d70   and adding `--p
+000046f0: 6f72 7420 3c70 6f72 743e 6020 746f 2074  ort <port>` to t
+00004700: 6865 2063 6f6d 6d61 6e64 2074 6f20 7370  he command to sp
+00004710: 6563 6966 7920 6120 6469 6666 6572 656e  ecify a differen
+00004720: 7420 706f 7274 2e7a 3554 7279 2073 7065  t port.z5Try spe
+00004730: 6369 6679 696e 6720 6120 6469 6666 6572  cifying a differ
+00004740: 656e 7420 706f 7274 2077 6974 6820 602d  ent port with `-
+00004750: 2d70 6f72 7420 3c70 6f72 743e 602e 2920  -port <port>`.) 
+00004760: da05 7072 696e 7472 6c00 0000 720e 0000  ..printrl...r...
+00004770: 0072 6d00 0000 5a0b 6765 745f 6170 705f  .rm...Z.get_app_
+00004780: 6469 7272 6100 0000 7262 0000 0072 6a00  dirra...rb...rj.
+00004790: 0000 7202 0000 0072 4b00 0000 5a0a 5573  ..r....rK...Z.Us
+000047a0: 6167 6545 7272 6f72 da04 6c69 7374 7281  ageError..listr.
+000047b0: 0000 00da 1854 5241 4e53 464f 524d 4552  .....TRANSFORMER
+000047c0: 5f50 4f4f 4c5f 4445 4641 554c 5472 0c00  _POOL_DEFAULTr..
+000047d0: 0000 72dc 0000 005a 0d69 735f 6173 796d  ..r....Z.is_asym
+000047e0: 6d65 7472 6963 724d 0000 0072 0900 0000  metricrM...r....
+000047f0: 5a0f 7365 745f 6465 7363 7269 7074 696f  Z.set_descriptio
+00004800: 6e72 6500 0000 727a 0000 005a 1267 6574  nre...rz...Z.get
+00004810: 5f6e 756d 5f64 696d 656e 7369 6f6e 7372  _num_dimensionsr
+00004820: 0300 0000 7229 0000 005a 0572 6f75 7465  ....r)...Z.route
+00004830: da03 7275 6eda 0a53 7973 7465 6d45 7869  ..run..SystemExi
+00004840: 74da 0373 7973 5a0e 7472 6163 6562 6163  t..sysZ.tracebac
+00004850: 6b6c 696d 6974 da0c 4445 4641 554c 545f  klimit..DEFAULT_
+00004860: 504f 5254 da09 4578 6365 7074 696f 6e29  PORT..Exception)
+00004870: 3172 2300 0000 7241 0000 005a 096e 6f5f  1r#...rA...Z.no_
+00004880: 7365 7276 6572 72eb 0000 0072 ea00 0000  serverr....r....
+00004890: 7274 0000 0072 7300 0000 728d 0000 0072  rt...rs...r....r
+000048a0: 8e00 0000 728f 0000 0072 9000 0000 725e  ....r....r....r^
+000048b0: 0000 005a 1174 7261 6e73 666f 726d 6572  ...Z.transformer
+000048c0: 5f6d 6f64 656c 722e 0000 0072 5600 0000  _modelr....rV...
+000048d0: 72b4 0000 0072 b300 0000 72b7 0000 0072  r....r....r....r
+000048e0: bd00 0000 72d6 0000 0072 d700 0000 72d8  ....r....r....r.
+000048f0: 0000 0072 3500 0000 7236 0000 0072 7500  ...r5...r6...ru.
+00004900: 0000 da07 7665 7273 696f 6e5a 0b6c 6973  ....versionZ.lis
+00004910: 745f 6d6f 6465 6c73 5a11 7368 6f77 5f73  t_modelsZ.show_s
+00004920: 656d 616e 7472 615f 6469 7272 3400 0000  emantra_dirr4...
+00004930: 5a0a 6d6f 6465 6c5f 6e61 6d65 5a08 656e  Z.model_nameZ.en
+00004940: 765f 7061 7468 5a11 7072 6f63 6573 7365  v_pathZ.processe
+00004950: 645f 7769 6e64 6f77 7372 5300 0000 5a0c  d_windowsrS...Z.
+00004960: 6d6f 6465 6c5f 636f 6e66 6967 7276 0000  model_configrv..
+00004970: 00da 0266 6e5a 0361 7070 729b 0000 0072  ...fnZ.appr....r
+00004980: 9c00 0000 72a3 0000 0072 b800 0000 72d9  ....r....r....r.
+00004990: 0000 0072 de00 0000 72e0 0000 0072 e800  ...r....r....r..
+000049a0: 0000 72e9 0000 0072 2100 0000 da01 6572  ..r....r!.....er
+000049b0: f100 0000 7226 0000 0029 0e72 b300 0000  ....r&...).r....
+000049c0: 7292 0000 0072 9300 0000 7294 0000 0072  r....r....r....r
+000049d0: d600 0000 72d7 0000 0072 9500 0000 725e  ....r....r....r^
+000049e0: 0000 0072 d800 0000 72b4 0000 0072 b500  ...r....r....r..
+000049f0: 0000 72b6 0000 0072 b700 0000 72bd 0000  ..r....r....r...
+00004a00: 0072 2700 0000 da04 6d61 696e 5d01 0000  .r'.....main]...
+00004a10: 73ca 0000 0000 7f00 5404 0108 0104 0204  s.......T.......
+00004a20: 0108 0110 0104 0208 010a 0204 0108 0104  ................
+00004a30: 030e 0108 0214 010a 020c 0208 0208 0104  ................
+00004a40: 0204 0102 0102 0102 0102 0102 0102 fb08  ................
+00004a50: 0908 0108 0108 0108 0108 010c 010a 0310  ................
+00004a60: 0102 0102 ff04 0504 010c 0108 0114 0102  ................
+00004a70: 0102 0102 0102 0106 0102 0102 0102 0102  ................
+00004a80: 0102 0102 0102 0102 0102 0102 f20e 1104  ................
+00004a90: 0104 0210 0e08 0208 010a 0708 010a 060e  ................
+00004aa0: 010e 0c0e 011a 2a0e 0114 340e 0112 210e  ......*...4...!.
+00004ab0: 0116 4b0e 010e 060e 010e 080e 010e 0d0e  ..K.............
+00004ac0: 010e 080e 010e 0406 0102 0112 0110 0108  ................
+00004ad0: 0106 010a 0102 0102 ff02 0202 fe04 0472  ...............r
+00004ae0: f700 0000 da08 5f5f 6d61 696e 5f5f 2944  ......__main__)D
+00004af0: 7267 0000 0072 e400 0000 7247 0000 0072  rg...r....rG...r
+00004b00: bf00 0000 7261 0000 0072 6d00 0000 5a05  ....ra...rm...Z.
+00004b10: 6e75 6d70 7972 7000 0000 729a 0000 005a  numpyrp...r....Z
+00004b20: 0664 6f74 656e 7672 0200 0000 5a05 666c  .dotenvr....Z.fl
+00004b30: 6173 6b72 0300 0000 7204 0000 0072 0500  askr....r....r..
+00004b40: 0000 7206 0000 0072 0700 0000 7208 0000  ..r....r....r...
+00004b50: 0072 0900 0000 720e 0000 0072 0b00 0000  .r....r....r....
+00004b60: 720c 0000 0072 0d00 0000 72df 0000 0072  r....r....r....r
+00004b70: 0f00 0000 da04 7574 696c 7210 0000 0072  ......utilr....r
+00004b80: 1100 0000 7212 0000 0072 1300 0000 7214  ....r....r....r.
+00004b90: 0000 0072 1500 0000 7216 0000 0072 1700  ...r....r....r..
+00004ba0: 0000 7218 0000 0072 1900 0000 721a 0000  ..r....r....r...
+00004bb0: 0072 1b00 0000 721c 0000 0072 1d00 0000  .r....r....r....
+00004bc0: 721e 0000 005a 0772 6571 7569 7265 72f4  r....Z.requirer.
+00004bd0: 0000 0072 6c00 0000 7266 0000 0072 f200  ...rl...rf...r..
+00004be0: 0000 7262 0000 00da 0764 6972 6e61 6d65  ..rb.....dirname
+00004bf0: da07 6162 7370 6174 68da 085f 5f66 696c  ..abspath..__fil
+00004c00: 655f 5f5a 1170 6163 6b61 6765 5f64 6972  e__Z.package_dir
+00004c10: 6563 746f 7279 7220 0000 0072 3800 0000  ectoryr ...r8...
+00004c20: 72ee 0000 0072 3900 0000 727a 0000 00da  r....r9...rz....
+00004c30: 0373 7472 7281 0000 005a 0763 6f6d 6d61  .strr....Z.comma
+00004c40: 6e64 5a08 6172 6775 6d65 6e74 da04 5061  ndZ.argument..Pa
+00004c50: 7468 5a06 6f70 7469 6f6e 5a06 4368 6f69  thZ.optionZ.Choi
+00004c60: 6365 da04 6b65 7973 7280 0000 0072 af00  ce..keysr....r..
+00004c70: 0000 72f7 0000 0072 2900 0000 7226 0000  ..r....r)...r&..
+00004c80: 0072 2600 0000 7226 0000 0072 2700 0000  .r&...r&...r'...
+00004c90: da08 3c6d 6f64 756c 653e 0100 0000 73dc  ..<module>....s.
+00004ca0: 0100 0008 0108 0108 0108 0108 0208 0108  ................
+00004cb0: 0108 010c 0120 010c 0218 010c 0144 1210  ..... .......D..
+00004cc0: 0104 0104 0214 030e 0708 0904 030e 3f08  ..............?.
+00004cd0: 7f00 5510 0e06 0116 0104 0102 0110 0102  ..U.............
+00004ce0: 0102 0102 fb04 0704 0102 0102 0102 0102  ................
+00004cf0: 0102 fb04 0704 0102 0102 0102 fd04 0504  ................
+00004d00: 0102 0102 0102 0102 0102 fb04 0704 0102  ................
+00004d10: 0102 0102 0102 0102 fb04 0704 0102 0102  ................
+00004d20: 0102 0102 0102 fb04 0704 0102 0102 0102  ................
+00004d30: 0102 0102 fb04 0704 0102 0102 0102 0102  ................
+00004d40: fc04 0604 0102 0102 0102 0102 fc04 0604  ................
+00004d50: 0102 0102 0102 0102 fc04 0604 0102 0102  ................
+00004d60: 0102 0102 fc04 0604 0102 0102 0102 0102  ................
+00004d70: fc04 0604 0102 0102 0102 0102 fc04 0604  ................
+00004d80: 0102 0102 0102 0102 0102 fb04 0704 0102  ................
+00004d90: 0102 0102 0102 0102 fb04 0704 0102 0102  ................
+00004da0: 0102 0102 0102 fb04 0704 0102 0102 0102  ................
+00004db0: 0102 0102 fb04 0704 0102 0102 0102 0102  ................
+00004dc0: 0102 fb04 0704 0102 0102 0102 0102 0102  ................
+00004dd0: fb04 0704 0102 0102 0102 0102 0102 fb04  ................
+00004de0: 0704 0102 0102 0102 0102 0102 fb04 0704  ................
+00004df0: 0108 ff04 0304 0102 0102 0102 0102 fc04  ................
+00004e00: 0604 0102 0102 0102 0102 fc04 0604 0102  ................
+00004e10: 0102 0102 0102 fc04 0604 0102 0102 0102  ................
+00004e20: 0102 fc04 0604 0102 0102 0102 0102 fc04  ................
+00004e30: 0604 0102 010a 0102 0102 fc04 0802 0102  ................
+00004e40: 0102 0102 0102 0102 0102 0102 0102 0102  ................
+00004e50: 0102 0102 0102 0102 0102 0102 0102 0102  ................
+00004e60: 0102 0102 0102 0102 0102 0102 0102 0102  ................
+00004e70: 0102 0102 e346 7f00 7f00 7f00 250a 01    .....F......%..
```

### Comparing `semantra-0.1.6/src/semantra/__pycache__/util.cpython-39.pyc` & `semantra-0.1.7/src/semantra/__pycache__/util.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Sat Apr 22 20:05:23 2023 UTC, .py size: 4524 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 033e 4464 ac11 0000  a........>Dd....
+00000000: 610d 0d0a 0000 0000 516b a964 ac11 0000  a.......Qk.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 b800 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6400 6401 6c03 5a04 6402  d.l.Z.d.d.l.Z.d.
 00000050: 5a05 6403 6404 8400 5a06 6405 6406 8400  Z.d.d...Z.d.d...
 00000060: 5a07 6407 6408 8400 5a08 6409 640a 8400  Z.d.d...Z.d.d...
 00000070: 5a09 640b 640c 8400 5a0a 640d 640e 8400  Z.d.d...Z.d.d...
```

### Comparing `semantra-0.1.6/src/semantra/client_public/build/bundle.css` & `semantra-0.1.7/src/semantra/client_public/build/bundle.css`

 * *Files identical despite different names*

### Comparing `semantra-0.1.6/src/semantra/client_public/build/bundle.js` & `semantra-0.1.7/src/semantra/client_public/build/bundle.js`

 * *Files identical despite different names*

### Comparing `semantra-0.1.6/src/semantra/client_public/build/bundle.js.map` & `semantra-0.1.7/src/semantra/client_public/build/bundle.js.map`

 * *Files identical despite different names*

### Comparing `semantra-0.1.6/src/semantra/client_public/favicon.png` & `semantra-0.1.7/src/semantra/client_public/favicon.png`

 * *Files identical despite different names*

### Comparing `semantra-0.1.6/src/semantra/client_public/global.css` & `semantra-0.1.7/src/semantra/client_public/global.css`

 * *Files identical despite different names*

### Comparing `semantra-0.1.6/src/semantra/models.py` & `semantra-0.1.7/src/semantra/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,19 @@
-import torch
+import os
 from abc import ABC, abstractmethod
-from transformers import AutoTokenizer, AutoModel
-import tiktoken
+
 import numpy as np
 import openai
+import tiktoken
+import torch
 from dotenv import load_dotenv
-import os
+from transformers import AutoModel, AutoTokenizer
 
 load_dotenv(dotenv_path=os.path.join(os.getcwd(), ".env"))
 
-if "OPENAI_API_KEY" in os.environ:
-    openai.api_key = os.getenv("OPENAI_API_KEY")
-
-
 minilm_model_name = "sentence-transformers/all-MiniLM-L6-v2"
 mpnet_model_name = "sentence-transformers/all-mpnet-base-v2"
 sgpt_model_name = "Muennighoff/SGPT-125M-weightedmean-msmarco-specb-bitfit"
 sgpt_1_3B_model_name = "Muennighoff/SGPT-1.3B-weightedmean-msmarco-specb-bitfit"
 
 
 def mean_pooling(model_output, attention_mask):
@@ -110,16 +107,19 @@
         model_name="text-embedding-ada-002",
         num_dimensions=1536,
         tokenizer_name="cl100k_base",
     ):
         # Check if OpenAI API key is set
         if "OPENAI_API_KEY" not in os.environ:
             raise Exception(
-                "OpenAI API key not set. Please set the OPENAI_API_KEY environment variable or create a `.env` file with the key in the same directory."
+                "OpenAI API key not set. Please set the OPENAI_API_KEY environment variable or create a `.env` file with the key in the current working directory or the Semantra directory, which is revealed by running `semantra --show-semantra-dir`."
             )
+        
+        openai.api_key = os.getenv("OPENAI_API_KEY")
+
         self.model_name = model_name
         self.num_dimensions = num_dimensions
         self.tokenizer = tiktoken.get_encoding(tokenizer_name)
 
     def get_config(self):
         return {
             "model_type": "openai",
```

### Comparing `semantra-0.1.6/src/semantra/pdf.py` & `semantra-0.1.7/src/semantra/pdf.py`

 * *Files identical despite different names*

### Comparing `semantra-0.1.6/src/semantra/semantra.py` & `semantra-0.1.7/src/semantra/semantra.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,39 +1,43 @@
+import hashlib
+import io
 import json
+import math
 import os
-from tqdm import tqdm
-import numpy as np
-from flask import Flask, request, jsonify, send_from_directory, send_file, make_response
+
 import click
-from .models import models, BaseModel, TransformerModel, as_numpy
-import io
+import numpy as np
+import pkg_resources
+from dotenv import load_dotenv
+from flask import Flask, jsonify, make_response, request, send_file, send_from_directory
+from tqdm import tqdm
+
+from .models import BaseModel, TransformerModel, as_numpy, models
 from .pdf import get_pdf_content
-import math
-import hashlib
 from .util import (
+    HASH_LENGTH,
     file_md5,
-    get_tokens_filename,
+    get_annoy_filename,
     get_config_filename,
     get_embeddings_filename,
+    get_num_annoy_embeddings,
     get_num_embeddings,
     get_offsets,
-    read_embeddings_file,
-    write_embedding,
+    get_tokens_filename,
     join_text_chunks,
-    get_annoy_filename,
-    get_num_annoy_embeddings,
-    write_annoy_db,
     load_annoy_db,
+    read_embeddings_file,
     sort_results,
-    HASH_LENGTH,
+    write_annoy_db,
+    write_embedding,
 )
-import pkg_resources
 
 VERSION = pkg_resources.require("semantra")[0].version
 DEFAULT_ENCODING = "utf-8"
+DEFAULT_PORT = 8080
 
 package_directory = os.path.dirname(os.path.abspath(__file__))
 
 
 class Content:
     def __init__(self, rawtext, filename):
         self.rawtext = rawtext
@@ -376,15 +380,15 @@
     default=False,
     show_default=True,
     help="Do not start the UI server (only process)",
 )
 @click.option(
     "--port",
     type=int,
-    default=8080,
+    default=DEFAULT_PORT,
     show_default=True,
     help="Port to use for embedding server",
 )
 @click.option(
     "--host",
     type=str,
     default="0.0.0.0",
@@ -564,14 +568,18 @@
 
     if semantra_dir is None:
         semantra_dir = click.get_app_dir("Semantra")
 
     if show_semantra_dir:
         print(semantra_dir)
         return
+    
+    # Load environment from Semantra dir
+    env_path = os.path.join(semantra_dir, ".env")
+    load_dotenv(env_path)
 
     if filename is None or len(filename) == 0:
         raise click.UsageError("Must provide a filename to process/query")
 
     processed_windows = list(process_windows(windows))
 
     if transformer_model is not None:
@@ -919,12 +927,22 @@
 
     @app.route("/api/text", methods=["GET"])
     def text():
         filename = request.args.get("filename")
         return jsonify(documents[filename].text_chunks)
 
     if not no_server:
-        app.run(host=host, port=port)
+        try:
+            app.run(host=host, port=port)
+        except SystemExit as e:
+            import sys
+            sys.tracebacklimit=0
+            if port == DEFAULT_PORT:
+                raise Exception(
+                    f'Try running again and adding `--port <port>` to the command to specify a different port.'
+                ) from None
+            else:
+                raise Exception(f"Try specifying a different port with `--port <port>`.") from None
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `semantra-0.1.6/src/semantra/util.py` & `semantra-0.1.7/src/semantra/util.py`

 * *Files identical despite different names*

### Comparing `semantra-0.1.6/src/semantra.egg-info/PKG-INFO` & `semantra-0.1.7/src/semantra.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: semantra
-Version: 0.1.6
+Version: 0.1.7
 Summary: A semantic search CLI tool
 Author-email: Dylan Freedman <freedmand@gmail.com>
 Project-URL: Homepage, https://github.com/freedmand/semantra
 Project-URL: Repository, https://github.com/freedmand/semantra
 Project-URL: Bug Tracker, https://github.com/freedmand/semantra/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -20,20 +20,20 @@
 
 The tool, made to run on the command line, analyzes specified text and PDF files on your computer and launches a local web search application for interactively querying them. The purpose of Semantra is to make running a specialized semantic search engine easy, friendly, configurable, and private/secure.
 
 Semantra is built for individuals seeking needles in haystacks — journalists sifting through leaked documents on deadline, researchers seeking insights within papers, students engaging with literature by querying themes, historians connecting events across books, and so forth.
 
 ## Resources
 
-- [Tutorial](docs/tutorial.md): a gentle introduction to getting started with Semantra — everything from installing the tool to hands-on examples of analyzing documents with it
+- [Tutorial](docs/tutorial.md): a gentle introduction to getting started with Semantra — everything from installing the tool to hands-on examples of analyzing documents with it
 - [Guides](docs/guides.md): practical guides on how to do more with Semantra
 - [Concepts](docs/concepts.md): Explainers on some concepts to better understand how Semantra works
 - [Using the web interface](docs/help.md): A reference on how to use the Semantra web app
 
-This page gives a high-level overview of Semantra and a reference of its features.
+This page gives a high-level overview of Semantra and a reference of its features. It's also available in other languages: [Semantra en español](docs/README_es.md), [Semantra 中文说明](docs/README_zh-CN.md)
 
 ## Installation
 
 Ensure you have [Python >= 3.9](https://www.python.org/downloads/).
 
 The easiest way to install Semantra is via `pipx`. If you do not have `pipx` installed, run:
```

### Comparing `semantra-0.1.6/src/semantra.egg-info/SOURCES.txt` & `semantra-0.1.7/src/semantra.egg-info/SOURCES.txt`

 * *Files identical despite different names*

