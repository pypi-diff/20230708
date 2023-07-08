# Comparing `tmp/slib-sorter-1.1.2.tar.gz` & `tmp/slib-sorter-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slib-sorter-1.1.2.tar", last modified: Sat Jul  8 02:27:10 2023, max compression
+gzip compressed data, was "slib-sorter-1.1.3.tar", last modified: Sat Jul  8 02:36:22 2023, max compression
```

## Comparing `slib-sorter-1.1.2.tar` & `slib-sorter-1.1.3.tar`

### file list

```diff
@@ -1,17 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-08 02:27:10.145461 slib-sorter-1.1.2/
--rw-rw-rw-   0        0        0    11558 2023-07-07 20:03:54.000000 slib-sorter-1.1.2/LICENSE
--rw-rw-rw-   0        0        0     2289 2023-07-08 02:27:10.145461 slib-sorter-1.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     1807 2023-07-07 20:03:54.000000 slib-sorter-1.1.2/README.md
--rw-rw-rw-   0        0        0       42 2023-07-08 02:27:10.145461 slib-sorter-1.1.2/setup.cfg
--rw-rw-rw-   0        0        0     1412 2023-07-08 02:27:00.000000 slib-sorter-1.1.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-08 02:27:10.142428 slib-sorter-1.1.2/slib_sorter.egg-info/
--rw-rw-rw-   0        0        0     2289 2023-07-08 02:27:10.000000 slib-sorter-1.1.2/slib_sorter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      300 2023-07-08 02:27:10.000000 slib-sorter-1.1.2/slib_sorter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-08 02:27:10.000000 slib-sorter-1.1.2/slib_sorter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       57 2023-07-08 02:27:10.000000 slib-sorter-1.1.2/slib_sorter.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       17 2023-07-08 02:27:10.000000 slib-sorter-1.1.2/slib_sorter.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-07-08 02:27:10.000000 slib-sorter-1.1.2/slib_sorter.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-08 02:27:10.144428 slib-sorter-1.1.2/src/
--rw-rw-rw-   0        0        0        0 2023-06-28 15:10:46.000000 slib-sorter-1.1.2/src/__init__.py
--rw-rw-rw-   0        0        0     9364 2023-07-08 01:47:57.000000 slib-sorter-1.1.2/src/filesorterfunctions.py
--rw-rw-rw-   0        0        0    72457 2023-07-08 02:20:39.000000 slib-sorter-1.1.2/src/slib_sorter.py
+drwxrwxrwx   0        0        0        0 2023-07-08 02:36:22.928582 slib-sorter-1.1.3/
+-rw-rw-rw-   0        0        0    11558 2023-07-07 20:03:54.000000 slib-sorter-1.1.3/LICENSE
+-rw-rw-rw-   0        0        0     2289 2023-07-08 02:36:22.928582 slib-sorter-1.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1807 2023-07-07 20:03:54.000000 slib-sorter-1.1.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-08 02:36:22.928582 slib-sorter-1.1.3/setup.cfg
+-rw-rw-rw-   0        0        0     4375 2023-07-08 02:36:10.000000 slib-sorter-1.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-08 02:36:22.926576 slib-sorter-1.1.3/slib_sorter.egg-info/
+-rw-rw-rw-   0        0        0     2289 2023-07-08 02:36:22.000000 slib-sorter-1.1.3/slib_sorter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      273 2023-07-08 02:36:22.000000 slib-sorter-1.1.3/slib_sorter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-08 02:36:22.000000 slib-sorter-1.1.3/slib_sorter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       56 2023-07-08 02:36:22.000000 slib-sorter-1.1.3/slib_sorter.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       17 2023-07-08 02:36:22.000000 slib-sorter-1.1.3/slib_sorter.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-07-08 02:36:22.000000 slib-sorter-1.1.3/slib_sorter.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-08 02:36:22.927590 slib-sorter-1.1.3/src/
+-rw-rw-rw-   0        0        0        0 2023-06-28 15:10:46.000000 slib-sorter-1.1.3/src/__init__.py
+-rw-rw-rw-   0        0        0    72457 2023-07-08 02:20:39.000000 slib-sorter-1.1.3/src/slib_sorter.py
```

### Comparing `slib-sorter-1.1.2/LICENSE` & `slib-sorter-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `slib-sorter-1.1.2/PKG-INFO` & `slib-sorter-1.1.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slib-sorter
-Version: 1.1.2
+Version: 1.1.3
 Summary: A Python library for sorting Sample Libraries
 Home-page: https://github.com/nrdrch/slib-sorter
 Author: Lukas Hübinger
 Author-email: fettkindasindauchoke@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
```

### Comparing `slib-sorter-1.1.2/README.md` & `slib-sorter-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `slib-sorter-1.1.2/slib_sorter.egg-info/PKG-INFO` & `slib-sorter-1.1.3/slib_sorter.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slib-sorter
-Version: 1.1.2
+Version: 1.1.3
 Summary: A Python library for sorting Sample Libraries
 Home-page: https://github.com/nrdrch/slib-sorter
 Author: Lukas Hübinger
 Author-email: fettkindasindauchoke@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
```

### Comparing `slib-sorter-1.1.2/src/slib_sorter.py` & `slib-sorter-1.1.3/src/slib_sorter.py`

 * *Files identical despite different names*

