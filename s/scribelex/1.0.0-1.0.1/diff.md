# Comparing `tmp/scribelex-1.0.0.tar.gz` & `tmp/scribelex-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scribelex-1.0.0.tar", last modified: Sat Jul  8 20:50:42 2023, max compression
+gzip compressed data, was "scribelex-1.0.1.tar", last modified: Sat Jul  8 20:54:38 2023, max compression
```

## Comparing `scribelex-1.0.0.tar` & `scribelex-1.0.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-07-08 20:50:42.098465 scribelex-1.0.0/
--rw-rw-rw-   0        0        0     1086 2023-07-08 20:43:01.000000 scribelex-1.0.0/LICENSE
--rw-rw-rw-   0        0        0     1135 2023-07-08 20:50:42.097454 scribelex-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-07-08 20:50:42.098465 scribelex-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1187 2023-07-08 20:45:21.000000 scribelex-1.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-08 20:50:42.085474 scribelex-1.0.0/src/
-drwxrwxrwx   0        0        0        0 2023-07-08 20:50:42.096458 scribelex-1.0.0/src/scribelex.egg-info/
--rw-rw-rw-   0        0        0     1135 2023-07-08 20:50:41.000000 scribelex-1.0.0/src/scribelex.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      164 2023-07-08 20:50:41.000000 scribelex-1.0.0/src/scribelex.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-08 20:50:41.000000 scribelex-1.0.0/src/scribelex.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-07-08 20:50:41.000000 scribelex-1.0.0/src/scribelex.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-08 20:54:38.183545 scribelex-1.0.1/
+-rw-rw-rw-   0        0        0     1086 2023-07-08 20:43:01.000000 scribelex-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0     1239 2023-07-08 20:54:38.182546 scribelex-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-07-08 20:54:38.183545 scribelex-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1289 2023-07-08 20:54:33.000000 scribelex-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-08 20:54:38.172152 scribelex-1.0.1/src/
+drwxrwxrwx   0        0        0        0 2023-07-08 20:54:38.182546 scribelex-1.0.1/src/scribelex.egg-info/
+-rw-rw-rw-   0        0        0     1239 2023-07-08 20:54:38.000000 scribelex-1.0.1/src/scribelex.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      164 2023-07-08 20:54:38.000000 scribelex-1.0.1/src/scribelex.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-08 20:54:38.000000 scribelex-1.0.1/src/scribelex.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2023-07-08 20:54:38.000000 scribelex-1.0.1/src/scribelex.egg-info/top_level.txt
```

### Comparing `scribelex-1.0.0/LICENSE` & `scribelex-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `scribelex-1.0.0/PKG-INFO` & `scribelex-1.0.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scribelex
-Version: 1.0.0
+Version: 1.0.1
 Summary: Scribelex is a lightweight Python library for building parser combinators.
 Home-page: https://github.com/UncleDrema/scribelex
 Author: UncleDrema
 Author-email: missl.wipiece@gmail.com
 License: MIT
 Keywords: parser,parsing,combinator,library,Python,structured data,grammar,syntax,parsing toolkit
 Classifier: Development Status :: 5 - Production/Stable
@@ -12,12 +12,14 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # scribelex
 scribelex - это моя реализация простого кобминатора парсеров, позволяющая гибко преобразовывать любые данные между разными форматами
```

### Comparing `scribelex-1.0.0/setup.py` & `scribelex-1.0.1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="scribelex",
-    version="1.0.0",
+    version="1.0.1",
     author="UncleDrema",
     author_email="missl.wipiece@gmail.com",
     description="Scribelex is a lightweight Python library for building parser combinators.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     keywords=["parser", "parsing", "combinator", "library", "Python", "structured data", "grammar", "syntax", "parsing toolkit"],
     url="https://github.com/UncleDrema/scribelex",
@@ -22,9 +22,11 @@
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
     ],
 )
```

### Comparing `scribelex-1.0.0/src/scribelex.egg-info/PKG-INFO` & `scribelex-1.0.1/src/scribelex.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scribelex
-Version: 1.0.0
+Version: 1.0.1
 Summary: Scribelex is a lightweight Python library for building parser combinators.
 Home-page: https://github.com/UncleDrema/scribelex
 Author: UncleDrema
 Author-email: missl.wipiece@gmail.com
 License: MIT
 Keywords: parser,parsing,combinator,library,Python,structured data,grammar,syntax,parsing toolkit
 Classifier: Development Status :: 5 - Production/Stable
@@ -12,12 +12,14 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # scribelex
 scribelex - это моя реализация простого кобминатора парсеров, позволяющая гибко преобразовывать любые данные между разными форматами
```

