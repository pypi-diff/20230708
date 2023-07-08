# Comparing `tmp/test4957-0.2.2.tar.gz` & `tmp/test4957-0.3.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "test4957-0.2.2.tar", last modified: Thu Jun 15 03:26:08 2023, max compression
+gzip compressed data, was "test4957-0.3.16.tar", last modified: Sat Jul  8 18:32:48 2023, max compression
```

## Comparing `test4957-0.2.2.tar` & `test4957-0.3.16.tar`

### file list

```diff
@@ -1,38 +1,15 @@
-drwxr-xr-x   0 nate       (501) staff       (20)        0 2023-06-15 03:26:08.732785 test4957-0.2.2/
--rw-r--r--   0 nate       (501) staff       (20)       26 2023-06-15 03:13:23.000000 test4957-0.2.2/MANIFEST.in
--rw-r--r--   0 nate       (501) staff       (20)      504 2023-06-15 03:26:08.732668 test4957-0.2.2/PKG-INFO
-drwxr-xr-x   0 nate       (501) staff       (20)        0 2023-06-15 03:26:08.709756 test4957-0.2.2/pypdfe/
--rw-r--r--   0 nate       (501) staff       (20)     4049 2023-06-15 00:34:56.000000 test4957-0.2.2/pypdfe/EstimatePDFmv.py
-drwxr-xr-x   0 nate       (501) staff       (20)        0 2023-06-15 03:26:08.731770 test4957-0.2.2/pypdfe/PDF-Estimator/
--rw-r--r--   0 nate       (501) staff       (20)     3056 2022-09-25 16:31:28.000000 test4957-0.2.2/pypdfe/PDF-Estimator/ChebyShev.cpp
--rw-r--r--   0 nate       (501) staff       (20)     1586 2022-09-25 16:33:30.000000 test4957-0.2.2/pypdfe/PDF-Estimator/ChebyShev.h
--rw-r--r--   0 nate       (501) staff       (20)    10093 2022-09-29 15:35:28.000000 test4957-0.2.2/pypdfe/PDF-Estimator/InputData.cpp
--rw-r--r--   0 nate       (501) staff       (20)     2292 2022-04-07 14:12:38.000000 test4957-0.2.2/pypdfe/PDF-Estimator/InputData.h
--rw-r--r--   0 nate       (501) staff       (20)     8394 2022-09-29 15:42:06.000000 test4957-0.2.2/pypdfe/PDF-Estimator/InputParameters.cpp
--rw-r--r--   0 nate       (501) staff       (20)     2561 2022-04-04 18:13:02.000000 test4957-0.2.2/pypdfe/PDF-Estimator/InputParameters.h
--rw-r--r--   0 nate       (501) staff       (20)     5070 2022-07-06 18:40:54.000000 test4957-0.2.2/pypdfe/PDF-Estimator/JointProbability.cpp
--rw-r--r--   0 nate       (501) staff       (20)     1763 2022-05-29 22:47:00.000000 test4957-0.2.2/pypdfe/PDF-Estimator/JointProbability.h
--rw-r--r--   0 nate       (501) staff       (20)    17670 2022-06-05 16:45:36.000000 test4957-0.2.2/pypdfe/PDF-Estimator/MinimizeScore.cpp
--rw-r--r--   0 nate       (501) staff       (20)     2932 2022-06-05 16:42:44.000000 test4957-0.2.2/pypdfe/PDF-Estimator/MinimizeScore.h
--rw-r--r--   0 nate       (501) staff       (20)     4528 2022-08-10 17:22:36.000000 test4957-0.2.2/pypdfe/PDF-Estimator/OutputControl.cpp
--rw-r--r--   0 nate       (501) staff       (20)     2094 2023-04-07 13:47:26.000000 test4957-0.2.2/pypdfe/PDF-Estimator/OutputControl.h
--rw-r--r--   0 nate       (501) staff       (20)     2024 2022-06-05 16:43:32.000000 test4957-0.2.2/pypdfe/PDF-Estimator/Score.cpp
--rw-r--r--   0 nate       (501) staff       (20)     1912 2022-06-05 16:44:50.000000 test4957-0.2.2/pypdfe/PDF-Estimator/Score.h
--rw-r--r--   0 nate       (501) staff       (20)    16296 2022-06-05 16:45:02.000000 test4957-0.2.2/pypdfe/PDF-Estimator/ScoreQZ.cpp
--rw-r--r--   0 nate       (501) staff       (20)     1450 2022-06-05 16:44:30.000000 test4957-0.2.2/pypdfe/PDF-Estimator/ScoreQZ.h
--rw-r--r--   0 nate       (501) staff       (20)     5635 2022-07-03 14:34:52.000000 test4957-0.2.2/pypdfe/PDF-Estimator/Variable.cpp
--rw-r--r--   0 nate       (501) staff       (20)     2053 2022-06-05 16:42:26.000000 test4957-0.2.2/pypdfe/PDF-Estimator/Variable.h
--rw-r--r--   0 nate       (501) staff       (20)    12020 2022-07-01 16:30:00.000000 test4957-0.2.2/pypdfe/PDF-Estimator/WriteResults.cpp
--rw-r--r--   0 nate       (501) staff       (20)     2418 2022-07-01 15:46:10.000000 test4957-0.2.2/pypdfe/PDF-Estimator/WriteResults.h
--rw-r--r--   0 nate       (501) staff       (20)     2490 2022-06-05 16:44:18.000000 test4957-0.2.2/pypdfe/PDF-Estimator/callPDF.cpp
--rw-r--r--   0 nate       (501) staff       (20)     1052 2023-06-14 21:42:19.000000 test4957-0.2.2/pypdfe/PDF-Estimator/callPDF.h
--rw-r--r--   0 nate       (501) staff       (20)     1722 2022-07-15 18:21:28.000000 test4957-0.2.2/pypdfe/PDF-Estimator/mvPDFMain.cpp
--rw-r--r--   0 nate       (501) staff       (20)       41 2023-04-11 08:52:55.000000 test4957-0.2.2/pypdfe/__init__.py
--rw-r--r--   0 nate       (501) staff       (20)       38 2023-06-15 03:26:08.732848 test4957-0.2.2/setup.cfg
--rw-r--r--   0 nate       (501) staff       (20)      972 2023-06-15 03:26:08.000000 test4957-0.2.2/setup.py
-drwxr-xr-x   0 nate       (501) staff       (20)        0 2023-06-15 03:26:08.732470 test4957-0.2.2/test4957.egg-info/
--rw-r--r--   0 nate       (501) staff       (20)      504 2023-06-15 03:26:08.000000 test4957-0.2.2/test4957.egg-info/PKG-INFO
--rw-r--r--   0 nate       (501) staff       (20)     1035 2023-06-15 03:26:08.000000 test4957-0.2.2/test4957.egg-info/SOURCES.txt
--rw-r--r--   0 nate       (501) staff       (20)        1 2023-06-15 03:26:08.000000 test4957-0.2.2/test4957.egg-info/dependency_links.txt
--rw-r--r--   0 nate       (501) staff       (20)        6 2023-06-15 03:26:08.000000 test4957-0.2.2/test4957.egg-info/requires.txt
--rw-r--r--   0 nate       (501) staff       (20)        7 2023-06-15 03:26:08.000000 test4957-0.2.2/test4957.egg-info/top_level.txt
+drwxr-xr-x   0 nate       (501) staff       (20)        0 2023-07-08 18:32:48.448991 test4957-0.3.16/
+-rw-r--r--   0 nate       (501) staff       (20)    35148 2023-07-08 17:48:49.000000 test4957-0.3.16/LICENSE
+-rw-r--r--   0 nate       (501) staff       (20)      153 2023-07-08 18:32:48.448878 test4957-0.3.16/PKG-INFO
+-rw-r--r--   0 nate       (501) staff       (20)       40 2023-07-08 18:12:46.000000 test4957-0.3.16/pyproject.toml
+-rw-r--r--   0 nate       (501) staff       (20)       38 2023-07-08 18:32:48.449043 test4957-0.3.16/setup.cfg
+-rw-r--r--   0 nate       (501) staff       (20)      383 2023-07-08 18:32:37.000000 test4957-0.3.16/setup.py
+drwxr-xr-x   0 nate       (501) staff       (20)        0 2023-07-08 18:32:48.448075 test4957-0.3.16/test4957/
+-rw-r--r--   0 nate       (501) staff       (20)       27 2023-07-08 17:57:38.000000 test4957-0.3.16/test4957/__init__.py
+-rw-r--r--   0 nate       (501) staff       (20)       43 2023-07-08 17:57:38.000000 test4957-0.3.16/test4957/hello.py
+drwxr-xr-x   0 nate       (501) staff       (20)        0 2023-07-08 18:32:48.448698 test4957-0.3.16/test4957.egg-info/
+-rw-r--r--   0 nate       (501) staff       (20)      153 2023-07-08 18:32:48.000000 test4957-0.3.16/test4957.egg-info/PKG-INFO
+-rw-r--r--   0 nate       (501) staff       (20)      229 2023-07-08 18:32:48.000000 test4957-0.3.16/test4957.egg-info/SOURCES.txt
+-rw-r--r--   0 nate       (501) staff       (20)        1 2023-07-08 18:32:48.000000 test4957-0.3.16/test4957.egg-info/dependency_links.txt
+-rw-r--r--   0 nate       (501) staff       (20)       11 2023-07-08 18:32:48.000000 test4957-0.3.16/test4957.egg-info/requires.txt
+-rw-r--r--   0 nate       (501) staff       (20)        9 2023-07-08 18:32:48.000000 test4957-0.3.16/test4957.egg-info/top_level.txt
```

