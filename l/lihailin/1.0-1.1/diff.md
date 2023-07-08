# Comparing `tmp/lihailin-1.0.tar.gz` & `tmp/lihailin-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lihailin-1.0.tar", last modified: Sat Jul  8 13:00:36 2023, max compression
+gzip compressed data, was "lihailin-1.1.tar", last modified: Sat Jul  8 13:15:25 2023, max compression
```

## Comparing `lihailin-1.0.tar` & `lihailin-1.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-07-08 13:00:36.610578 lihailin-1.0/
--rw-rw-rw-   0        0        0      206 2023-07-08 13:00:36.610578 lihailin-1.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-08 13:00:36.610578 lihailin-1.0/lihailin.egg-info/
--rw-rw-rw-   0        0        0      206 2023-07-08 13:00:36.000000 lihailin-1.0/lihailin.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      202 2023-07-08 13:00:36.000000 lihailin-1.0/lihailin.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-08 13:00:36.000000 lihailin-1.0/lihailin.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       40 2023-07-08 13:00:36.000000 lihailin-1.0/lihailin.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       17 2023-07-08 13:00:36.000000 lihailin-1.0/lihailin.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-07-08 13:00:36.000000 lihailin-1.0/lihailin.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-08 13:00:36.610578 lihailin-1.0/setup.cfg
--rw-rw-rw-   0        0        0      585 2023-07-08 12:58:35.000000 lihailin-1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-08 13:15:25.555252 lihailin-1.1/
+-rw-rw-rw-   0        0        0      206 2023-07-08 13:15:25.555252 lihailin-1.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-08 13:15:25.555252 lihailin-1.1/lihailin.egg-info/
+-rw-rw-rw-   0        0        0      206 2023-07-08 13:15:25.000000 lihailin-1.1/lihailin.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      202 2023-07-08 13:15:25.000000 lihailin-1.1/lihailin.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-08 13:15:25.000000 lihailin-1.1/lihailin.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       40 2023-07-08 13:15:25.000000 lihailin-1.1/lihailin.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       17 2023-07-08 13:15:25.000000 lihailin-1.1/lihailin.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-07-08 13:15:25.000000 lihailin-1.1/lihailin.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-08 13:15:25.555252 lihailin-1.1/setup.cfg
+-rw-rw-rw-   0        0        0      585 2023-07-08 13:15:14.000000 lihailin-1.1/setup.py
```

### Comparing `lihailin-1.0/setup.py` & `lihailin-1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
  
   
  
 setup(
  
  name = "lihailin",
  
- version = "1.0",
+ version = "1.1",
  
  description = "eds sdk",
  
  long_description = "eds sdk for python",
  
  license = "MIT Licence",
```

