# Comparing `tmp/pypdfe-0.1.4.tar.gz` & `tmp/pypdfe-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypdfe-0.1.4.tar", last modified: Sat Jul  8 19:03:32 2023, max compression
+gzip compressed data, was "pypdfe-0.1.5.tar", last modified: Sat Jul  8 19:24:15 2023, max compression
```

## Comparing `pypdfe-0.1.4.tar` & `pypdfe-0.1.5.tar`

### file list

```diff
@@ -1,43 +1,87 @@
-drwxr-xr-x   0 nate       (501) staff       (20)        0 2023-07-08 19:03:32.809295 pypdfe-0.1.4/
--rw-r--r--   0 nate       (501) staff       (20)    35148 2023-07-08 07:31:18.000000 pypdfe-0.1.4/LICENSE
--rw-r--r--   0 nate       (501) staff       (20)      297 2023-07-08 19:03:32.809203 pypdfe-0.1.4/PKG-INFO
-drwxr-xr-x   0 nate       (501) staff       (20)        0 2023-07-08 19:03:32.804990 pypdfe-0.1.4/pypdfe/
--rw-r--r--   0 nate       (501) staff       (20)     1025 2023-07-08 07:18:43.000000 pypdfe-0.1.4/pypdfe/__init__.py
-drwxr-xr-x   0 nate       (501) staff       (20)        0 2023-07-08 19:03:32.805741 pypdfe-0.1.4/pypdfe.egg-info/
--rw-r--r--   0 nate       (501) staff       (20)      297 2023-07-08 19:03:32.000000 pypdfe-0.1.4/pypdfe.egg-info/PKG-INFO
--rw-r--r--   0 nate       (501) staff       (20)     2604 2023-07-08 19:03:32.000000 pypdfe-0.1.4/pypdfe.egg-info/SOURCES.txt
--rw-r--r--   0 nate       (501) staff       (20)        1 2023-07-08 19:03:32.000000 pypdfe-0.1.4/pypdfe.egg-info/dependency_links.txt
--rw-r--r--   0 nate       (501) staff       (20)        1 2023-07-08 19:03:32.000000 pypdfe-0.1.4/pypdfe.egg-info/not-zip-safe
--rw-r--r--   0 nate       (501) staff       (20)        6 2023-07-08 19:03:32.000000 pypdfe-0.1.4/pypdfe.egg-info/requires.txt
--rw-r--r--   0 nate       (501) staff       (20)        7 2023-07-08 19:03:32.000000 pypdfe-0.1.4/pypdfe.egg-info/top_level.txt
--rw-r--r--   0 nate       (501) staff       (20)      130 2023-07-08 19:03:11.000000 pypdfe-0.1.4/pyproject.toml
--rw-r--r--   0 nate       (501) staff       (20)       38 2023-07-08 19:03:32.809337 pypdfe-0.1.4/setup.cfg
--rw-r--r--   0 nate       (501) staff       (20)     1723 2023-07-08 19:03:11.000000 pypdfe-0.1.4/setup.py
-drwxr-xr-x   0 nate       (501) staff       (20)        0 2023-07-08 19:03:32.805865 pypdfe-0.1.4/src/
-drwxr-xr-x   0 nate       (501) staff       (20)        0 2023-07-08 19:03:32.809027 pypdfe-0.1.4/src/PDF-Estimator/
--rw-r--r--   0 nate       (501) staff       (20)     2947 2023-06-21 20:32:32.000000 pypdfe-0.1.4/src/PDF-Estimator/ChebyShev.cpp
--rw-r--r--   0 nate       (501) staff       (20)     1542 2023-06-21 20:32:32.000000 pypdfe-0.1.4/src/PDF-Estimator/ChebyShev.h
--rw-r--r--   0 nate       (501) staff       (20)     9785 2023-06-21 20:32:32.000000 pypdfe-0.1.4/src/PDF-Estimator/InputData.cpp
--rw-r--r--   0 nate       (501) staff       (20)     2214 2023-06-21 20:32:32.000000 pypdfe-0.1.4/src/PDF-Estimator/InputData.h
--rw-r--r--   0 nate       (501) staff       (20)     8394 2023-06-21 20:32:32.000000 pypdfe-0.1.4/src/PDF-Estimator/InputParameters.cpp
--rw-r--r--   0 nate       (501) staff       (20)     2470 2023-06-21 20:32:32.000000 pypdfe-0.1.4/src/PDF-Estimator/InputParameters.h
--rw-r--r--   0 nate       (501) staff       (20)     4922 2023-06-21 20:32:32.000000 pypdfe-0.1.4/src/PDF-Estimator/JointProbability.cpp
--rw-r--r--   0 nate       (501) staff       (20)     1711 2023-06-21 20:32:32.000000 pypdfe-0.1.4/src/PDF-Estimator/JointProbability.h
--rw-r--r--   0 nate       (501) staff       (20)    35149 2023-06-21 20:32:32.000000 pypdfe-0.1.4/src/PDF-Estimator/LICENSE
--rw-r--r--   0 nate       (501) staff       (20)    17168 2023-06-21 20:32:32.000000 pypdfe-0.1.4/src/PDF-Estimator/MinimizeScore.cpp
--rw-r--r--   0 nate       (501) staff       (20)     2839 2023-06-21 20:32:32.000000 pypdfe-0.1.4/src/PDF-Estimator/MinimizeScore.h
--rw-r--r--   0 nate       (501) staff       (20)     4372 2023-06-21 20:32:32.000000 pypdfe-0.1.4/src/PDF-Estimator/OutputControl.cpp
--rw-r--r--   0 nate       (501) staff       (20)     2028 2023-06-21 20:32:32.000000 pypdfe-0.1.4/src/PDF-Estimator/OutputControl.h
--rw-r--r--   0 nate       (501) staff       (20)      773 2023-06-21 20:32:32.000000 pypdfe-0.1.4/src/PDF-Estimator/README.txt
--rw-r--r--   0 nate       (501) staff       (20)     1959 2023-06-21 20:32:32.000000 pypdfe-0.1.4/src/PDF-Estimator/Score.cpp
--rw-r--r--   0 nate       (501) staff       (20)     1857 2023-06-21 20:32:32.000000 pypdfe-0.1.4/src/PDF-Estimator/Score.h
--rw-r--r--   0 nate       (501) staff       (20)    16156 2023-06-21 20:32:32.000000 pypdfe-0.1.4/src/PDF-Estimator/ScoreQZ.cpp
--rw-r--r--   0 nate       (501) staff       (20)     1410 2023-06-21 20:32:32.000000 pypdfe-0.1.4/src/PDF-Estimator/ScoreQZ.h
--rw-r--r--   0 nate       (501) staff       (20)     5467 2023-06-21 20:32:32.000000 pypdfe-0.1.4/src/PDF-Estimator/Variable.cpp
--rw-r--r--   0 nate       (501) staff       (20)     1995 2023-06-21 20:32:32.000000 pypdfe-0.1.4/src/PDF-Estimator/Variable.h
--rw-r--r--   0 nate       (501) staff       (20)    11691 2023-06-21 20:32:32.000000 pypdfe-0.1.4/src/PDF-Estimator/WriteResults.cpp
--rw-r--r--   0 nate       (501) staff       (20)     2352 2023-06-21 20:32:32.000000 pypdfe-0.1.4/src/PDF-Estimator/WriteResults.h
--rw-r--r--   0 nate       (501) staff       (20)     2407 2023-06-21 20:32:32.000000 pypdfe-0.1.4/src/PDF-Estimator/callPDF.cpp
--rw-r--r--   0 nate       (501) staff       (20)     1007 2023-06-21 20:32:32.000000 pypdfe-0.1.4/src/PDF-Estimator/callPDF.h
--rw-r--r--   0 nate       (501) staff       (20)     1669 2023-06-21 20:32:32.000000 pypdfe-0.1.4/src/PDF-Estimator/mvPDFMain.cpp
--rw-r--r--   0 nate       (501) staff       (20)     1149 2023-07-08 19:03:11.000000 pypdfe-0.1.4/src/main.cpp
+drwxr-xr-x   0 nate       (501) staff       (20)        0 2023-07-08 19:24:15.511738 pypdfe-0.1.5/
+-rw-r--r--   0 nate       (501) staff       (20)    35148 2023-07-08 07:31:18.000000 pypdfe-0.1.5/LICENSE
+-rw-r--r--   0 nate       (501) staff       (20)        9 2023-07-08 19:23:32.000000 pypdfe-0.1.5/MANIFEST.in
+-rw-r--r--   0 nate       (501) staff       (20)      297 2023-07-08 19:24:15.511637 pypdfe-0.1.5/PKG-INFO
+drwxr-xr-x   0 nate       (501) staff       (20)        0 2023-07-08 19:24:15.503744 pypdfe-0.1.5/pypdfe/
+-rw-r--r--   0 nate       (501) staff       (20)     1025 2023-07-08 07:18:43.000000 pypdfe-0.1.5/pypdfe/__init__.py
+drwxr-xr-x   0 nate       (501) staff       (20)        0 2023-07-08 19:24:15.504485 pypdfe-0.1.5/pypdfe.egg-info/
+-rw-r--r--   0 nate       (501) staff       (20)      297 2023-07-08 19:24:15.000000 pypdfe-0.1.5/pypdfe.egg-info/PKG-INFO
+-rw-r--r--   0 nate       (501) staff       (20)     3658 2023-07-08 19:24:15.000000 pypdfe-0.1.5/pypdfe.egg-info/SOURCES.txt
+-rw-r--r--   0 nate       (501) staff       (20)        1 2023-07-08 19:24:15.000000 pypdfe-0.1.5/pypdfe.egg-info/dependency_links.txt
+-rw-r--r--   0 nate       (501) staff       (20)        1 2023-07-08 19:24:15.000000 pypdfe-0.1.5/pypdfe.egg-info/not-zip-safe
+-rw-r--r--   0 nate       (501) staff       (20)        6 2023-07-08 19:24:15.000000 pypdfe-0.1.5/pypdfe.egg-info/requires.txt
+-rw-r--r--   0 nate       (501) staff       (20)        7 2023-07-08 19:24:15.000000 pypdfe-0.1.5/pypdfe.egg-info/top_level.txt
+-rw-r--r--   0 nate       (501) staff       (20)      131 2023-07-08 19:23:32.000000 pypdfe-0.1.5/pyproject.toml
+-rw-r--r--   0 nate       (501) staff       (20)       38 2023-07-08 19:24:15.511783 pypdfe-0.1.5/setup.cfg
+-rw-r--r--   0 nate       (501) staff       (20)     1698 2023-07-08 19:23:32.000000 pypdfe-0.1.5/setup.py
+drwxr-xr-x   0 nate       (501) staff       (20)        0 2023-07-08 19:24:15.504733 pypdfe-0.1.5/src/
+-rw-r--r--   0 nate       (501) staff       (20)     8196 2023-07-08 03:12:16.000000 pypdfe-0.1.5/src/.DS_Store
+drwxr-xr-x   0 nate       (501) staff       (20)        0 2023-07-08 19:24:15.508040 pypdfe-0.1.5/src/PDF-Estimator/
+-rw-r--r--   0 nate       (501) staff       (20)     8196 2023-06-21 21:23:08.000000 pypdfe-0.1.5/src/PDF-Estimator/.DS_Store
+drwxr-xr-x   0 nate       (501) staff       (20)        0 2023-07-08 19:24:15.508772 pypdfe-0.1.5/src/PDF-Estimator/.git/
+-rw-r--r--   0 nate       (501) staff       (20)      103 2023-06-21 22:03:26.000000 pypdfe-0.1.5/src/PDF-Estimator/.git/FETCH_HEAD
+-rw-r--r--   0 nate       (501) staff       (20)       21 2023-06-21 20:32:32.000000 pypdfe-0.1.5/src/PDF-Estimator/.git/HEAD
+-rw-r--r--   0 nate       (501) staff       (20)      309 2023-06-21 20:32:32.000000 pypdfe-0.1.5/src/PDF-Estimator/.git/config
+-rw-r--r--   0 nate       (501) staff       (20)       73 2023-06-21 20:32:31.000000 pypdfe-0.1.5/src/PDF-Estimator/.git/description
+drwxr-xr-x   0 nate       (501) staff       (20)        0 2023-07-08 19:24:15.510331 pypdfe-0.1.5/src/PDF-Estimator/.git/hooks/
+-rwxr-xr-x   0 nate       (501) staff       (20)      478 2023-06-21 20:32:31.000000 pypdfe-0.1.5/src/PDF-Estimator/.git/hooks/applypatch-msg.sample
+-rwxr-xr-x   0 nate       (501) staff       (20)      896 2023-06-21 20:32:31.000000 pypdfe-0.1.5/src/PDF-Estimator/.git/hooks/commit-msg.sample
+-rwxr-xr-x   0 nate       (501) staff       (20)     4726 2023-06-21 20:32:31.000000 pypdfe-0.1.5/src/PDF-Estimator/.git/hooks/fsmonitor-watchman.sample
+-rwxr-xr-x   0 nate       (501) staff       (20)      189 2023-06-21 20:32:31.000000 pypdfe-0.1.5/src/PDF-Estimator/.git/hooks/post-update.sample
+-rwxr-xr-x   0 nate       (501) staff       (20)      424 2023-06-21 20:32:31.000000 pypdfe-0.1.5/src/PDF-Estimator/.git/hooks/pre-applypatch.sample
+-rwxr-xr-x   0 nate       (501) staff       (20)     1643 2023-06-21 20:32:31.000000 pypdfe-0.1.5/src/PDF-Estimator/.git/hooks/pre-commit.sample
+-rwxr-xr-x   0 nate       (501) staff       (20)      416 2023-06-21 20:32:31.000000 pypdfe-0.1.5/src/PDF-Estimator/.git/hooks/pre-merge-commit.sample
+-rwxr-xr-x   0 nate       (501) staff       (20)     1374 2023-06-21 20:32:31.000000 pypdfe-0.1.5/src/PDF-Estimator/.git/hooks/pre-push.sample
+-rwxr-xr-x   0 nate       (501) staff       (20)     4898 2023-06-21 20:32:31.000000 pypdfe-0.1.5/src/PDF-Estimator/.git/hooks/pre-rebase.sample
+-rwxr-xr-x   0 nate       (501) staff       (20)      544 2023-06-21 20:32:31.000000 pypdfe-0.1.5/src/PDF-Estimator/.git/hooks/pre-receive.sample
+-rwxr-xr-x   0 nate       (501) staff       (20)     1492 2023-06-21 20:32:31.000000 pypdfe-0.1.5/src/PDF-Estimator/.git/hooks/prepare-commit-msg.sample
+-rwxr-xr-x   0 nate       (501) staff       (20)     2783 2023-06-21 20:32:31.000000 pypdfe-0.1.5/src/PDF-Estimator/.git/hooks/push-to-checkout.sample
+-rwxr-xr-x   0 nate       (501) staff       (20)     3650 2023-06-21 20:32:31.000000 pypdfe-0.1.5/src/PDF-Estimator/.git/hooks/update.sample
+-rw-r--r--   0 nate       (501) staff       (20)     2102 2023-06-22 03:25:25.000000 pypdfe-0.1.5/src/PDF-Estimator/.git/index
+drwxr-xr-x   0 nate       (501) staff       (20)        0 2023-07-08 19:24:15.510459 pypdfe-0.1.5/src/PDF-Estimator/.git/info/
+-rw-r--r--   0 nate       (501) staff       (20)      240 2023-06-21 20:32:31.000000 pypdfe-0.1.5/src/PDF-Estimator/.git/info/exclude
+drwxr-xr-x   0 nate       (501) staff       (20)        0 2023-07-08 19:24:15.510578 pypdfe-0.1.5/src/PDF-Estimator/.git/logs/
+-rw-r--r--   0 nate       (501) staff       (20)      213 2023-06-21 20:32:32.000000 pypdfe-0.1.5/src/PDF-Estimator/.git/logs/HEAD
+drwxr-xr-x   0 nate       (501) staff       (20)        0 2023-07-08 19:24:15.502333 pypdfe-0.1.5/src/PDF-Estimator/.git/logs/refs/
+drwxr-xr-x   0 nate       (501) staff       (20)        0 2023-07-08 19:24:15.510717 pypdfe-0.1.5/src/PDF-Estimator/.git/logs/refs/heads/
+-rw-r--r--   0 nate       (501) staff       (20)      213 2023-06-21 20:32:32.000000 pypdfe-0.1.5/src/PDF-Estimator/.git/logs/refs/heads/main
+drwxr-xr-x   0 nate       (501) staff       (20)        0 2023-07-08 19:24:15.502377 pypdfe-0.1.5/src/PDF-Estimator/.git/logs/refs/remotes/
+drwxr-xr-x   0 nate       (501) staff       (20)        0 2023-07-08 19:24:15.510853 pypdfe-0.1.5/src/PDF-Estimator/.git/logs/refs/remotes/origin/
+-rw-r--r--   0 nate       (501) staff       (20)      213 2023-06-21 20:32:32.000000 pypdfe-0.1.5/src/PDF-Estimator/.git/logs/refs/remotes/origin/HEAD
+drwxr-xr-x   0 nate       (501) staff       (20)        0 2023-07-08 19:24:15.502503 pypdfe-0.1.5/src/PDF-Estimator/.git/objects/
+drwxr-xr-x   0 nate       (501) staff       (20)        0 2023-07-08 19:24:15.511157 pypdfe-0.1.5/src/PDF-Estimator/.git/objects/pack/
+-r--r--r--   0 nate       (501) staff       (20)     1996 2023-06-21 20:32:32.000000 pypdfe-0.1.5/src/PDF-Estimator/.git/objects/pack/pack-68fcf6d5b1d91b28c20241431b9241a5762ddad3.idx
+-r--r--r--   0 nate       (501) staff       (20)    47733 2023-06-21 20:32:32.000000 pypdfe-0.1.5/src/PDF-Estimator/.git/objects/pack/pack-68fcf6d5b1d91b28c20241431b9241a5762ddad3.pack
+-rw-r--r--   0 nate       (501) staff       (20)      112 2023-06-21 20:32:32.000000 pypdfe-0.1.5/src/PDF-Estimator/.git/packed-refs
+drwxr-xr-x   0 nate       (501) staff       (20)        0 2023-07-08 19:24:15.502701 pypdfe-0.1.5/src/PDF-Estimator/.git/refs/
+drwxr-xr-x   0 nate       (501) staff       (20)        0 2023-07-08 19:24:15.511318 pypdfe-0.1.5/src/PDF-Estimator/.git/refs/heads/
+-rw-r--r--   0 nate       (501) staff       (20)       41 2023-06-21 20:32:32.000000 pypdfe-0.1.5/src/PDF-Estimator/.git/refs/heads/main
+drwxr-xr-x   0 nate       (501) staff       (20)        0 2023-07-08 19:24:15.502740 pypdfe-0.1.5/src/PDF-Estimator/.git/refs/remotes/
+drwxr-xr-x   0 nate       (501) staff       (20)        0 2023-07-08 19:24:15.511450 pypdfe-0.1.5/src/PDF-Estimator/.git/refs/remotes/origin/
+-rw-r--r--   0 nate       (501) staff       (20)       30 2023-06-21 20:32:32.000000 pypdfe-0.1.5/src/PDF-Estimator/.git/refs/remotes/origin/HEAD
+-rw-r--r--   0 nate       (501) staff       (20)     2947 2023-06-21 20:32:32.000000 pypdfe-0.1.5/src/PDF-Estimator/ChebyShev.cpp
+-rw-r--r--   0 nate       (501) staff       (20)     1542 2023-06-21 20:32:32.000000 pypdfe-0.1.5/src/PDF-Estimator/ChebyShev.h
+-rw-r--r--   0 nate       (501) staff       (20)     9785 2023-06-21 20:32:32.000000 pypdfe-0.1.5/src/PDF-Estimator/InputData.cpp
+-rw-r--r--   0 nate       (501) staff       (20)     2214 2023-06-21 20:32:32.000000 pypdfe-0.1.5/src/PDF-Estimator/InputData.h
+-rw-r--r--   0 nate       (501) staff       (20)     8394 2023-06-21 20:32:32.000000 pypdfe-0.1.5/src/PDF-Estimator/InputParameters.cpp
+-rw-r--r--   0 nate       (501) staff       (20)     2470 2023-06-21 20:32:32.000000 pypdfe-0.1.5/src/PDF-Estimator/InputParameters.h
+-rw-r--r--   0 nate       (501) staff       (20)     4922 2023-06-21 20:32:32.000000 pypdfe-0.1.5/src/PDF-Estimator/JointProbability.cpp
+-rw-r--r--   0 nate       (501) staff       (20)     1711 2023-06-21 20:32:32.000000 pypdfe-0.1.5/src/PDF-Estimator/JointProbability.h
+-rw-r--r--   0 nate       (501) staff       (20)    35149 2023-06-21 20:32:32.000000 pypdfe-0.1.5/src/PDF-Estimator/LICENSE
+-rw-r--r--   0 nate       (501) staff       (20)    17168 2023-06-21 20:32:32.000000 pypdfe-0.1.5/src/PDF-Estimator/MinimizeScore.cpp
+-rw-r--r--   0 nate       (501) staff       (20)     2839 2023-06-21 20:32:32.000000 pypdfe-0.1.5/src/PDF-Estimator/MinimizeScore.h
+-rw-r--r--   0 nate       (501) staff       (20)     4372 2023-06-21 20:32:32.000000 pypdfe-0.1.5/src/PDF-Estimator/OutputControl.cpp
+-rw-r--r--   0 nate       (501) staff       (20)     2028 2023-06-21 20:32:32.000000 pypdfe-0.1.5/src/PDF-Estimator/OutputControl.h
+-rw-r--r--   0 nate       (501) staff       (20)      773 2023-06-21 20:32:32.000000 pypdfe-0.1.5/src/PDF-Estimator/README.txt
+-rw-r--r--   0 nate       (501) staff       (20)     1959 2023-06-21 20:32:32.000000 pypdfe-0.1.5/src/PDF-Estimator/Score.cpp
+-rw-r--r--   0 nate       (501) staff       (20)     1857 2023-06-21 20:32:32.000000 pypdfe-0.1.5/src/PDF-Estimator/Score.h
+-rw-r--r--   0 nate       (501) staff       (20)    16156 2023-06-21 20:32:32.000000 pypdfe-0.1.5/src/PDF-Estimator/ScoreQZ.cpp
+-rw-r--r--   0 nate       (501) staff       (20)     1410 2023-06-21 20:32:32.000000 pypdfe-0.1.5/src/PDF-Estimator/ScoreQZ.h
+-rw-r--r--   0 nate       (501) staff       (20)     5467 2023-06-21 20:32:32.000000 pypdfe-0.1.5/src/PDF-Estimator/Variable.cpp
+-rw-r--r--   0 nate       (501) staff       (20)     1995 2023-06-21 20:32:32.000000 pypdfe-0.1.5/src/PDF-Estimator/Variable.h
+-rw-r--r--   0 nate       (501) staff       (20)    11691 2023-06-21 20:32:32.000000 pypdfe-0.1.5/src/PDF-Estimator/WriteResults.cpp
+-rw-r--r--   0 nate       (501) staff       (20)     2352 2023-06-21 20:32:32.000000 pypdfe-0.1.5/src/PDF-Estimator/WriteResults.h
+-rw-r--r--   0 nate       (501) staff       (20)     2407 2023-06-21 20:32:32.000000 pypdfe-0.1.5/src/PDF-Estimator/callPDF.cpp
+-rw-r--r--   0 nate       (501) staff       (20)     1007 2023-06-21 20:32:32.000000 pypdfe-0.1.5/src/PDF-Estimator/callPDF.h
+-rw-r--r--   0 nate       (501) staff       (20)     1669 2023-06-21 20:32:32.000000 pypdfe-0.1.5/src/PDF-Estimator/mvPDFMain.cpp
+-rw-r--r--   0 nate       (501) staff       (20)     1149 2023-07-08 19:23:32.000000 pypdfe-0.1.5/src/main.cpp
```

### Comparing `pypdfe-0.1.4/LICENSE` & `pypdfe-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pypdfe-0.1.4/pypdfe/__init__.py` & `pypdfe-0.1.5/pypdfe/__init__.py`

 * *Files identical despite different names*

### Comparing `pypdfe-0.1.4/pypdfe.egg-info/SOURCES.txt` & `pypdfe-0.1.5/pypdfe.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 LICENSE
+MANIFEST.in
 pyproject.toml
 setup.py
 /Users/nate/Desktop/Research/pyPDFe_dev/setuptools_for_self_replacing/pypdfe/src/main.cpp
 /Users/nate/Desktop/Research/pyPDFe_dev/setuptools_for_self_replacing/pypdfe/src/PDF-Estimator/ChebyShev.cpp
 /Users/nate/Desktop/Research/pyPDFe_dev/setuptools_for_self_replacing/pypdfe/src/PDF-Estimator/InputData.cpp
 /Users/nate/Desktop/Research/pyPDFe_dev/setuptools_for_self_replacing/pypdfe/src/PDF-Estimator/InputParameters.cpp
 /Users/nate/Desktop/Research/pyPDFe_dev/setuptools_for_self_replacing/pypdfe/src/PDF-Estimator/JointProbability.cpp
@@ -16,33 +17,62 @@
 pypdfe/__init__.py
 pypdfe.egg-info/PKG-INFO
 pypdfe.egg-info/SOURCES.txt
 pypdfe.egg-info/dependency_links.txt
 pypdfe.egg-info/not-zip-safe
 pypdfe.egg-info/requires.txt
 pypdfe.egg-info/top_level.txt
-pypdfe/../src/main.cpp
-pypdfe/../src/PDF-Estimator/ChebyShev.cpp
-pypdfe/../src/PDF-Estimator/ChebyShev.h
-pypdfe/../src/PDF-Estimator/InputData.cpp
-pypdfe/../src/PDF-Estimator/InputData.h
-pypdfe/../src/PDF-Estimator/InputParameters.cpp
-pypdfe/../src/PDF-Estimator/InputParameters.h
-pypdfe/../src/PDF-Estimator/JointProbability.cpp
-pypdfe/../src/PDF-Estimator/JointProbability.h
-pypdfe/../src/PDF-Estimator/LICENSE
-pypdfe/../src/PDF-Estimator/MinimizeScore.cpp
-pypdfe/../src/PDF-Estimator/MinimizeScore.h
-pypdfe/../src/PDF-Estimator/OutputControl.cpp
-pypdfe/../src/PDF-Estimator/OutputControl.h
-pypdfe/../src/PDF-Estimator/README.txt
-pypdfe/../src/PDF-Estimator/Score.cpp
-pypdfe/../src/PDF-Estimator/Score.h
-pypdfe/../src/PDF-Estimator/ScoreQZ.cpp
-pypdfe/../src/PDF-Estimator/ScoreQZ.h
-pypdfe/../src/PDF-Estimator/Variable.cpp
-pypdfe/../src/PDF-Estimator/Variable.h
-pypdfe/../src/PDF-Estimator/WriteResults.cpp
-pypdfe/../src/PDF-Estimator/WriteResults.h
-pypdfe/../src/PDF-Estimator/callPDF.cpp
-pypdfe/../src/PDF-Estimator/callPDF.h
-pypdfe/../src/PDF-Estimator/mvPDFMain.cpp
+src/.DS_Store
+src/main.cpp
+src/PDF-Estimator/.DS_Store
+src/PDF-Estimator/ChebyShev.cpp
+src/PDF-Estimator/ChebyShev.h
+src/PDF-Estimator/InputData.cpp
+src/PDF-Estimator/InputData.h
+src/PDF-Estimator/InputParameters.cpp
+src/PDF-Estimator/InputParameters.h
+src/PDF-Estimator/JointProbability.cpp
+src/PDF-Estimator/JointProbability.h
+src/PDF-Estimator/LICENSE
+src/PDF-Estimator/MinimizeScore.cpp
+src/PDF-Estimator/MinimizeScore.h
+src/PDF-Estimator/OutputControl.cpp
+src/PDF-Estimator/OutputControl.h
+src/PDF-Estimator/README.txt
+src/PDF-Estimator/Score.cpp
+src/PDF-Estimator/Score.h
+src/PDF-Estimator/ScoreQZ.cpp
+src/PDF-Estimator/ScoreQZ.h
+src/PDF-Estimator/Variable.cpp
+src/PDF-Estimator/Variable.h
+src/PDF-Estimator/WriteResults.cpp
+src/PDF-Estimator/WriteResults.h
+src/PDF-Estimator/callPDF.cpp
+src/PDF-Estimator/callPDF.h
+src/PDF-Estimator/mvPDFMain.cpp
+src/PDF-Estimator/.git/FETCH_HEAD
+src/PDF-Estimator/.git/HEAD
+src/PDF-Estimator/.git/config
+src/PDF-Estimator/.git/description
+src/PDF-Estimator/.git/index
+src/PDF-Estimator/.git/packed-refs
+src/PDF-Estimator/.git/hooks/applypatch-msg.sample
+src/PDF-Estimator/.git/hooks/commit-msg.sample
+src/PDF-Estimator/.git/hooks/fsmonitor-watchman.sample
+src/PDF-Estimator/.git/hooks/post-update.sample
+src/PDF-Estimator/.git/hooks/pre-applypatch.sample
+src/PDF-Estimator/.git/hooks/pre-commit.sample
+src/PDF-Estimator/.git/hooks/pre-merge-commit.sample
+src/PDF-Estimator/.git/hooks/pre-push.sample
+src/PDF-Estimator/.git/hooks/pre-rebase.sample
+src/PDF-Estimator/.git/hooks/pre-receive.sample
+src/PDF-Estimator/.git/hooks/prepare-commit-msg.sample
+src/PDF-Estimator/.git/hooks/push-to-checkout.sample
+src/PDF-Estimator/.git/hooks/update.sample
+src/PDF-Estimator/.git/info/exclude
+src/PDF-Estimator/.git/logs/HEAD
+src/PDF-Estimator/.git/logs/refs/heads/main
+src/PDF-Estimator/.git/logs/refs/remotes/origin/HEAD
+src/PDF-Estimator/.git/objects/pack/pack-68fcf6d5b1d91b28c20241431b9241a5762ddad3.idx
+src/PDF-Estimator/.git/objects/pack/pack-68fcf6d5b1d91b28c20241431b9241a5762ddad3.pack
+src/PDF-Estimator/.git/refs/heads/main
+src/PDF-Estimator/.git/refs/remotes/origin/HEAD
```

### Comparing `pypdfe-0.1.4/setup.py` & `pypdfe-0.1.5/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Available at setup time due to pyproject.toml
 from pybind11.setup_helpers import Pybind11Extension, build_ext
 from setuptools import setup
 from glob import glob
 import os
 
-__version__ = "0.1.4"
+__version__ = "0.1.5"
 
 # The main interface is through Pybind11Extension.
 # * You can add cxx_std=11/14/17, and then build_ext can be removed.
 # * You can set include_pybind11=false to add the include directory yourself,
 #   say from a submodule.
 #
 # Note:
@@ -34,15 +34,13 @@
     author="Nate Mauney",
     author_email="nmauney4@uncc.edu",
     url="https://github.com/CHANGE_ME",
     description="A Python package for PDF estimation using Dr. Jennifer Farmer's PDFe and multivariate PDF libraries.",
     long_description="",
     ext_modules=ext_modules,
     packages=['pypdfe'],
-    package_data={'pypdfe': ['_pypdfe.*']+src_files},
+    package_data={'pypdfe': ['_pypdfe.*']},
     cmdclass={"build_ext": build_ext},
     zip_safe=False,
     python_requires=">=3.8",
-    install_requires=[
-        'numpy',
-    ],
+    install_requires=['numpy'],
 )
```

### Comparing `pypdfe-0.1.4/src/PDF-Estimator/ChebyShev.cpp` & `pypdfe-0.1.5/src/PDF-Estimator/ChebyShev.cpp`

 * *Files identical despite different names*

### Comparing `pypdfe-0.1.4/src/PDF-Estimator/ChebyShev.h` & `pypdfe-0.1.5/src/PDF-Estimator/ChebyShev.h`

 * *Files identical despite different names*

### Comparing `pypdfe-0.1.4/src/PDF-Estimator/InputData.cpp` & `pypdfe-0.1.5/src/PDF-Estimator/InputData.cpp`

 * *Files identical despite different names*

### Comparing `pypdfe-0.1.4/src/PDF-Estimator/InputData.h` & `pypdfe-0.1.5/src/PDF-Estimator/InputData.h`

 * *Files identical despite different names*

### Comparing `pypdfe-0.1.4/src/PDF-Estimator/InputParameters.cpp` & `pypdfe-0.1.5/src/PDF-Estimator/InputParameters.cpp`

 * *Files identical despite different names*

### Comparing `pypdfe-0.1.4/src/PDF-Estimator/InputParameters.h` & `pypdfe-0.1.5/src/PDF-Estimator/InputParameters.h`

 * *Files identical despite different names*

### Comparing `pypdfe-0.1.4/src/PDF-Estimator/JointProbability.cpp` & `pypdfe-0.1.5/src/PDF-Estimator/JointProbability.cpp`

 * *Files identical despite different names*

### Comparing `pypdfe-0.1.4/src/PDF-Estimator/JointProbability.h` & `pypdfe-0.1.5/src/PDF-Estimator/JointProbability.h`

 * *Files identical despite different names*

### Comparing `pypdfe-0.1.4/src/PDF-Estimator/LICENSE` & `pypdfe-0.1.5/src/PDF-Estimator/LICENSE`

 * *Files identical despite different names*

### Comparing `pypdfe-0.1.4/src/PDF-Estimator/MinimizeScore.cpp` & `pypdfe-0.1.5/src/PDF-Estimator/MinimizeScore.cpp`

 * *Files identical despite different names*

### Comparing `pypdfe-0.1.4/src/PDF-Estimator/MinimizeScore.h` & `pypdfe-0.1.5/src/PDF-Estimator/MinimizeScore.h`

 * *Files identical despite different names*

### Comparing `pypdfe-0.1.4/src/PDF-Estimator/OutputControl.cpp` & `pypdfe-0.1.5/src/PDF-Estimator/OutputControl.cpp`

 * *Files identical despite different names*

### Comparing `pypdfe-0.1.4/src/PDF-Estimator/OutputControl.h` & `pypdfe-0.1.5/src/PDF-Estimator/OutputControl.h`

 * *Files identical despite different names*

### Comparing `pypdfe-0.1.4/src/PDF-Estimator/README.txt` & `pypdfe-0.1.5/src/PDF-Estimator/README.txt`

 * *Files identical despite different names*

### Comparing `pypdfe-0.1.4/src/PDF-Estimator/Score.cpp` & `pypdfe-0.1.5/src/PDF-Estimator/Score.cpp`

 * *Files identical despite different names*

### Comparing `pypdfe-0.1.4/src/PDF-Estimator/Score.h` & `pypdfe-0.1.5/src/PDF-Estimator/Score.h`

 * *Files identical despite different names*

### Comparing `pypdfe-0.1.4/src/PDF-Estimator/ScoreQZ.cpp` & `pypdfe-0.1.5/src/PDF-Estimator/ScoreQZ.cpp`

 * *Files identical despite different names*

### Comparing `pypdfe-0.1.4/src/PDF-Estimator/ScoreQZ.h` & `pypdfe-0.1.5/src/PDF-Estimator/ScoreQZ.h`

 * *Files identical despite different names*

### Comparing `pypdfe-0.1.4/src/PDF-Estimator/Variable.cpp` & `pypdfe-0.1.5/src/PDF-Estimator/Variable.cpp`

 * *Files identical despite different names*

### Comparing `pypdfe-0.1.4/src/PDF-Estimator/Variable.h` & `pypdfe-0.1.5/src/PDF-Estimator/Variable.h`

 * *Files identical despite different names*

### Comparing `pypdfe-0.1.4/src/PDF-Estimator/WriteResults.cpp` & `pypdfe-0.1.5/src/PDF-Estimator/WriteResults.cpp`

 * *Files identical despite different names*

### Comparing `pypdfe-0.1.4/src/PDF-Estimator/WriteResults.h` & `pypdfe-0.1.5/src/PDF-Estimator/WriteResults.h`

 * *Files identical despite different names*

### Comparing `pypdfe-0.1.4/src/PDF-Estimator/callPDF.cpp` & `pypdfe-0.1.5/src/PDF-Estimator/callPDF.cpp`

 * *Files identical despite different names*

### Comparing `pypdfe-0.1.4/src/PDF-Estimator/callPDF.h` & `pypdfe-0.1.5/src/PDF-Estimator/callPDF.h`

 * *Files identical despite different names*

### Comparing `pypdfe-0.1.4/src/PDF-Estimator/mvPDFMain.cpp` & `pypdfe-0.1.5/src/PDF-Estimator/mvPDFMain.cpp`

 * *Files identical despite different names*

### Comparing `pypdfe-0.1.4/src/main.cpp` & `pypdfe-0.1.5/src/main.cpp`

 * *Files identical despite different names*

