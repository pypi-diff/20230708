# Comparing `tmp/Simple_ML_Algo-1.0.0.tar.gz` & `tmp/Simple_ML_Algo-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Simple_ML_Algo-1.0.0.tar", last modified: Sat Jul  8 13:50:57 2023, max compression
+gzip compressed data, was "Simple_ML_Algo-1.0.2.tar", last modified: Sat Jul  8 15:58:58 2023, max compression
```

## Comparing `Simple_ML_Algo-1.0.0.tar` & `Simple_ML_Algo-1.0.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-07-08 13:50:57.738484 Simple_ML_Algo-1.0.0/
--rw-rw-rw-   0        0        0      170 2023-07-08 13:50:57.738484 Simple_ML_Algo-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-07-08 13:50:57.739482 Simple_ML_Algo-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      338 2023-07-08 13:45:19.000000 Simple_ML_Algo-1.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-08 13:50:57.363375 Simple_ML_Algo-1.0.0/src/
-drwxrwxrwx   0        0        0        0 2023-07-08 13:50:57.374382 Simple_ML_Algo-1.0.0/src/Simple_ML_Algo.egg-info/
--rw-rw-rw-   0        0        0      170 2023-07-08 13:50:57.000000 Simple_ML_Algo-1.0.0/src/Simple_ML_Algo.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      217 2023-07-08 13:50:57.000000 Simple_ML_Algo-1.0.0/src/Simple_ML_Algo.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-08 13:50:57.000000 Simple_ML_Algo-1.0.0/src/Simple_ML_Algo.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-07-08 13:50:57.000000 Simple_ML_Algo-1.0.0/src/Simple_ML_Algo.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-07-08 13:50:57.000000 Simple_ML_Algo-1.0.0/src/Simple_ML_Algo.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-08 15:58:58.154477 Simple_ML_Algo-1.0.2/
+-rw-rw-rw-   0        0        0      170 2023-07-08 15:58:58.153469 Simple_ML_Algo-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-07-08 15:58:58.154477 Simple_ML_Algo-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      338 2023-07-08 15:48:14.000000 Simple_ML_Algo-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-08 15:58:58.144466 Simple_ML_Algo-1.0.2/src/
+drwxrwxrwx   0        0        0        0 2023-07-08 15:58:58.152474 Simple_ML_Algo-1.0.2/src/Simple_ML_Algo.egg-info/
+-rw-rw-rw-   0        0        0      170 2023-07-08 15:58:57.000000 Simple_ML_Algo-1.0.2/src/Simple_ML_Algo.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      217 2023-07-08 15:58:58.000000 Simple_ML_Algo-1.0.2/src/Simple_ML_Algo.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-08 15:58:57.000000 Simple_ML_Algo-1.0.2/src/Simple_ML_Algo.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-07-08 15:58:57.000000 Simple_ML_Algo-1.0.2/src/Simple_ML_Algo.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-07-08 15:58:57.000000 Simple_ML_Algo-1.0.2/src/Simple_ML_Algo.egg-info/top_level.txt
```

