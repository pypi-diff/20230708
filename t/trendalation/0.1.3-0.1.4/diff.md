# Comparing `tmp/trendalation-0.1.3.tar.gz` & `tmp/trendalation-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trendalation-0.1.3.tar", last modified: Sat Jul  8 17:20:47 2023, max compression
+gzip compressed data, was "trendalation-0.1.4.tar", last modified: Sat Jul  8 17:31:52 2023, max compression
```

## Comparing `trendalation-0.1.3.tar` & `trendalation-0.1.4.tar`

### file list

```diff
@@ -1,20 +1,11 @@
-drwxr-xr-x   0 raghavsaboo   (501) staff       (20)        0 2023-07-08 17:20:47.000309 trendalation-0.1.3/
--rw-r--r--   0 raghavsaboo   (501) staff       (20)     1084 2023-07-08 16:44:54.000000 trendalation-0.1.3/LICENSE.rst
--rw-r--r--   0 raghavsaboo   (501) staff       (20)      550 2023-07-08 17:20:47.000368 trendalation-0.1.3/PKG-INFO
--rw-r--r--   0 raghavsaboo   (501) staff       (20)      872 2023-07-08 16:44:54.000000 trendalation-0.1.3/README.md
--rw-r--r--   0 raghavsaboo   (501) staff       (20)       84 2023-07-08 17:03:14.000000 trendalation-0.1.3/pyproject.toml
--rw-r--r--   0 raghavsaboo   (501) staff       (20)      107 2023-07-08 17:20:47.000584 trendalation-0.1.3/setup.cfg
--rw-r--r--   0 raghavsaboo   (501) staff       (20)      789 2023-07-08 17:20:37.000000 trendalation-0.1.3/setup.py
-drwxr-xr-x   0 raghavsaboo   (501) staff       (20)        0 2023-07-08 17:20:46.997799 trendalation-0.1.3/src/
-drwxr-xr-x   0 raghavsaboo   (501) staff       (20)        0 2023-07-08 17:20:46.999147 trendalation-0.1.3/src/classifiers/
--rw-r--r--   0 raghavsaboo   (501) staff       (20)       43 2023-07-08 17:01:22.000000 trendalation-0.1.3/src/classifiers/__init__.py
--rw-r--r--   0 raghavsaboo   (501) staff       (20)     5885 2023-07-08 17:00:29.000000 trendalation-0.1.3/src/classifiers/proc_classifier.py
-drwxr-xr-x   0 raghavsaboo   (501) staff       (20)        0 2023-07-08 17:20:46.999414 trendalation-0.1.3/src/metrics/
--rw-r--r--   0 raghavsaboo   (501) staff       (20)       48 2023-07-08 17:01:25.000000 trendalation-0.1.3/src/metrics/__init__.py
--rw-r--r--   0 raghavsaboo   (501) staff       (20)     1479 2023-07-08 16:44:54.000000 trendalation-0.1.3/src/metrics/metrics.py
-drwxr-xr-x   0 raghavsaboo   (501) staff       (20)        0 2023-07-08 17:20:47.000135 trendalation-0.1.3/src/trendalation.egg-info/
--rw-r--r--   0 raghavsaboo   (501) staff       (20)      550 2023-07-08 17:20:46.000000 trendalation-0.1.3/src/trendalation.egg-info/PKG-INFO
--rw-r--r--   0 raghavsaboo   (501) staff       (20)      364 2023-07-08 17:20:46.000000 trendalation-0.1.3/src/trendalation.egg-info/SOURCES.txt
--rw-r--r--   0 raghavsaboo   (501) staff       (20)        1 2023-07-08 17:20:46.000000 trendalation-0.1.3/src/trendalation.egg-info/dependency_links.txt
--rw-r--r--   0 raghavsaboo   (501) staff       (20)       25 2023-07-08 17:20:46.000000 trendalation-0.1.3/src/trendalation.egg-info/requires.txt
--rw-r--r--   0 raghavsaboo   (501) staff       (20)       20 2023-07-08 17:20:46.000000 trendalation-0.1.3/src/trendalation.egg-info/top_level.txt
+drwxr-xr-x   0 raghavsaboo   (501) staff       (20)        0 2023-07-08 17:31:52.553351 trendalation-0.1.4/
+-rw-r--r--   0 raghavsaboo   (501) staff       (20)     1084 2023-07-08 16:44:54.000000 trendalation-0.1.4/LICENSE.rst
+-rw-r--r--   0 raghavsaboo   (501) staff       (20)     1436 2023-07-08 17:31:52.553402 trendalation-0.1.4/PKG-INFO
+-rw-r--r--   0 raghavsaboo   (501) staff       (20)      872 2023-07-08 16:44:54.000000 trendalation-0.1.4/README.md
+-rw-r--r--   0 raghavsaboo   (501) staff       (20)       93 2023-07-08 17:30:19.000000 trendalation-0.1.4/pyproject.toml
+-rw-r--r--   0 raghavsaboo   (501) staff       (20)      756 2023-07-08 17:31:52.553649 trendalation-0.1.4/setup.cfg
+drwxr-xr-x   0 raghavsaboo   (501) staff       (20)        0 2023-07-08 17:31:52.553219 trendalation-0.1.4/trendalation.egg-info/
+-rw-r--r--   0 raghavsaboo   (501) staff       (20)     1436 2023-07-08 17:31:52.000000 trendalation-0.1.4/trendalation.egg-info/PKG-INFO
+-rw-r--r--   0 raghavsaboo   (501) staff       (20)      190 2023-07-08 17:31:52.000000 trendalation-0.1.4/trendalation.egg-info/SOURCES.txt
+-rw-r--r--   0 raghavsaboo   (501) staff       (20)        1 2023-07-08 17:31:52.000000 trendalation-0.1.4/trendalation.egg-info/dependency_links.txt
+-rw-r--r--   0 raghavsaboo   (501) staff       (20)        1 2023-07-08 17:31:52.000000 trendalation-0.1.4/trendalation.egg-info/top_level.txt
```

### Comparing `trendalation-0.1.3/LICENSE.rst` & `trendalation-0.1.4/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `trendalation-0.1.3/README.md` & `trendalation-0.1.4/README.md`

 * *Files identical despite different names*

