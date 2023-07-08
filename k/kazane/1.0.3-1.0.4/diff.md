# Comparing `tmp/kazane-1.0.3.tar.gz` & `tmp/kazane-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kazane-1.0.3.tar", last modified: Mon Aug 29 02:12:10 2022, max compression
+gzip compressed data, was "kazane-1.0.4.tar", last modified: Sat Jul  8 16:00:04 2023, max compression
```

## Comparing `kazane-1.0.3.tar` & `kazane-1.0.4.tar`

### file list

```diff
@@ -1,24 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-29 02:12:10.857776 kazane-1.0.3/
--rw-r--r--   0 runner    (1001) docker     (121)     1068 2022-08-29 02:12:01.000000 kazane-1.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     2621 2022-08-29 02:12:10.857776 kazane-1.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2251 2022-08-29 02:12:01.000000 kazane-1.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-29 02:12:10.857776 kazane-1.0.3/kazane/
--rw-r--r--   0 runner    (1001) docker     (121)      150 2022-08-29 02:12:01.000000 kazane-1.0.3/kazane/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2261 2022-08-29 02:12:01.000000 kazane-1.0.3/kazane/decimate.py
--rw-r--r--   0 runner    (1001) docker     (121)     1797 2022-08-29 02:12:01.000000 kazane-1.0.3/kazane/fftconv.py
--rw-r--r--   0 runner    (1001) docker     (121)     5610 2022-08-29 02:12:01.000000 kazane-1.0.3/kazane/resample.py
--rw-r--r--   0 runner    (1001) docker     (121)      689 2022-08-29 02:12:01.000000 kazane-1.0.3/kazane/sinc.py
--rw-r--r--   0 runner    (1001) docker     (121)     3556 2022-08-29 02:12:01.000000 kazane-1.0.3/kazane/upsample.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-29 02:12:10.857776 kazane-1.0.3/kazane.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2621 2022-08-29 02:12:10.000000 kazane-1.0.3/kazane.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      370 2022-08-29 02:12:10.000000 kazane-1.0.3/kazane.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-29 02:12:10.000000 kazane-1.0.3/kazane.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        6 2022-08-29 02:12:10.000000 kazane-1.0.3/kazane.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       13 2022-08-29 02:12:10.000000 kazane-1.0.3/kazane.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-29 02:12:10.857776 kazane-1.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      684 2022-08-29 02:12:01.000000 kazane-1.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-29 02:12:10.857776 kazane-1.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-29 02:12:01.000000 kazane-1.0.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1869 2022-08-29 02:12:01.000000 kazane-1.0.3/tests/test_decimate.py
--rw-r--r--   0 runner    (1001) docker     (121)      377 2022-08-29 02:12:01.000000 kazane-1.0.3/tests/test_padding.py
--rw-r--r--   0 runner    (1001) docker     (121)     1449 2022-08-29 02:12:01.000000 kazane-1.0.3/tests/test_upsample.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 16:00:04.539583 kazane-1.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-08 15:59:51.000000 kazane-1.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-07-08 16:00:04.539583 kazane-1.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-07-08 15:59:51.000000 kazane-1.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 16:00:04.539583 kazane-1.0.4/kazane/
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-07-08 15:59:51.000000 kazane-1.0.4/kazane/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-07-08 15:59:51.000000 kazane-1.0.4/kazane/decimate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-07-08 15:59:51.000000 kazane-1.0.4/kazane/fftconv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5610 2023-07-08 15:59:51.000000 kazane-1.0.4/kazane/resample.py
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-07-08 15:59:51.000000 kazane-1.0.4/kazane/sinc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-07-08 15:59:51.000000 kazane-1.0.4/kazane/upsample.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 16:00:04.539583 kazane-1.0.4/kazane.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-07-08 16:00:04.000000 kazane-1.0.4/kazane.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-07-08 16:00:04.000000 kazane-1.0.4/kazane.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 16:00:04.000000 kazane-1.0.4/kazane.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-08 16:00:04.000000 kazane-1.0.4/kazane.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-08 16:00:04.000000 kazane-1.0.4/kazane.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 16:00:04.539583 kazane-1.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-07-08 15:59:51.000000 kazane-1.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 16:00:04.539583 kazane-1.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-07-08 15:59:51.000000 kazane-1.0.4/tests/test_decimate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-07-08 15:59:51.000000 kazane-1.0.4/tests/test_padding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-07-08 15:59:51.000000 kazane-1.0.4/tests/test_upsample.py
```

### Comparing `kazane-1.0.3/LICENSE` & `kazane-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `kazane-1.0.3/PKG-INFO` & `kazane-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kazane
-Version: 1.0.3
+Version: 1.0.4
 Home-page: https://github.com/yoyololicon/kazane
 Author: Chin-Yun Yu
 Author-email: lolimaster.cs03@nctu.edu.tw
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `kazane-1.0.3/README.md` & `kazane-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `kazane-1.0.3/kazane/decimate.py` & `kazane-1.0.4/kazane/decimate.py`

 * *Files identical despite different names*

### Comparing `kazane-1.0.3/kazane/fftconv.py` & `kazane-1.0.4/kazane/fftconv.py`

 * *Files identical despite different names*

### Comparing `kazane-1.0.3/kazane/resample.py` & `kazane-1.0.4/kazane/resample.py`

 * *Files identical despite different names*

### Comparing `kazane-1.0.3/kazane/sinc.py` & `kazane-1.0.4/kazane/sinc.py`

 * *Files identical despite different names*

### Comparing `kazane-1.0.3/kazane/upsample.py` & `kazane-1.0.4/kazane/upsample.py`

 * *Files identical despite different names*

### Comparing `kazane-1.0.3/kazane.egg-info/PKG-INFO` & `kazane-1.0.4/kazane.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kazane
-Version: 1.0.3
+Version: 1.0.4
 Home-page: https://github.com/yoyololicon/kazane
 Author: Chin-Yun Yu
 Author-email: lolimaster.cs03@nctu.edu.tw
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `kazane-1.0.3/setup.py` & `kazane-1.0.4/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 import setuptools
 
 NAME = "kazane"
-VERSION = '1.0.3'
-AUTHOR = 'Chin-Yun Yu'
-EMAIL = 'lolimaster.cs03@nctu.edu.tw'
+VERSION = "1.0.4"
+AUTHOR = "Chin-Yun Yu"
+EMAIL = "lolimaster.cs03@nctu.edu.tw"
 
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name=NAME,
     version=VERSION,
     author=AUTHOR,
     author_email=EMAIL,
     description="",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/yoyololicon/kazane",
-    packages=setuptools.find_packages(),
-    install_requires=['torch'],
+    packages=["kazane"],
+    install_requires=["torch"],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
 )
```

### Comparing `kazane-1.0.3/tests/test_decimate.py` & `kazane-1.0.4/tests/test_decimate.py`

 * *Files identical despite different names*

### Comparing `kazane-1.0.3/tests/test_upsample.py` & `kazane-1.0.4/tests/test_upsample.py`

 * *Files identical despite different names*

