# Comparing `tmp/pypdfe-0.1.1.tar.gz` & `tmp/pypdfe-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypdfe-0.1.1.tar", last modified: Thu Jun 22 04:08:00 2023, max compression
+gzip compressed data, was "pypdfe-0.1.2.tar", last modified: Sat Jul  8 18:38:19 2023, max compression
```

## Comparing `pypdfe-0.1.1.tar` & `pypdfe-0.1.2.tar`

### file list

```diff
@@ -1,93 +1,15 @@
-drwxr-xr-x   0 nate       (501) staff       (20)        0 2023-06-22 04:08:00.409236 pypdfe-0.1.1/
--rw-r--r--   0 nate       (501) staff       (20)       20 2023-06-22 01:29:19.000000 pypdfe-0.1.1/MANIFEST.in
--rw-r--r--   0 nate       (501) staff       (20)      580 2023-06-22 04:08:00.409142 pypdfe-0.1.1/PKG-INFO
-drwxr-xr-x   0 nate       (501) staff       (20)        0 2023-06-22 04:08:00.402196 pypdfe-0.1.1/pypdfe.egg-info/
--rw-r--r--   0 nate       (501) staff       (20)      580 2023-06-22 04:08:00.000000 pypdfe-0.1.1/pypdfe.egg-info/PKG-INFO
--rw-r--r--   0 nate       (501) staff       (20)     3373 2023-06-22 04:08:00.000000 pypdfe-0.1.1/pypdfe.egg-info/SOURCES.txt
--rw-r--r--   0 nate       (501) staff       (20)        1 2023-06-22 04:08:00.000000 pypdfe-0.1.1/pypdfe.egg-info/dependency_links.txt
--rw-r--r--   0 nate       (501) staff       (20)       12 2023-06-22 04:08:00.000000 pypdfe-0.1.1/pypdfe.egg-info/requires.txt
--rw-r--r--   0 nate       (501) staff       (20)       15 2023-06-22 04:08:00.000000 pypdfe-0.1.1/pypdfe.egg-info/top_level.txt
-drwxr-xr-x   0 nate       (501) staff       (20)        0 2023-06-22 04:08:00.402678 pypdfe-0.1.1/pypdfe_builder/
--rw-r--r--   0 nate       (501) staff       (20)     6148 2023-06-21 23:11:07.000000 pypdfe-0.1.1/pypdfe_builder/.DS_Store
--rw-r--r--   0 nate       (501) staff       (20)     1628 2023-06-21 22:57:15.000000 pypdfe-0.1.1/pypdfe_builder/CMakeLists.txt
--rw-r--r--   0 nate       (501) staff       (20)      643 2023-06-22 01:18:17.000000 pypdfe-0.1.1/pypdfe_builder/__init__.py
-drwxr-xr-x   0 nate       (501) staff       (20)        0 2023-06-22 04:08:00.402803 pypdfe-0.1.1/pypdfe_builder/__pycache__/
--rw-r--r--   0 nate       (501) staff       (20)      192 2023-06-22 02:55:25.000000 pypdfe-0.1.1/pypdfe_builder/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 nate       (501) staff       (20)     2324 2023-06-22 03:51:51.000000 pypdfe-0.1.1/pypdfe_builder/pyproject.toml
-drwxr-xr-x   0 nate       (501) staff       (20)        0 2023-06-22 04:08:00.403011 pypdfe-0.1.1/pypdfe_builder/src/
--rw-r--r--   0 nate       (501) staff       (20)     8196 2023-06-21 22:56:34.000000 pypdfe-0.1.1/pypdfe_builder/src/.DS_Store
-drwxr-xr-x   0 nate       (501) staff       (20)        0 2023-06-22 04:08:00.405781 pypdfe-0.1.1/pypdfe_builder/src/PDF-Estimator/
--rw-r--r--   0 nate       (501) staff       (20)     8196 2023-06-21 21:23:08.000000 pypdfe-0.1.1/pypdfe_builder/src/PDF-Estimator/.DS_Store
-drwxr-xr-x   0 nate       (501) staff       (20)        0 2023-06-22 04:08:00.406369 pypdfe-0.1.1/pypdfe_builder/src/PDF-Estimator/.git/
--rw-r--r--   0 nate       (501) staff       (20)      103 2023-06-21 22:03:26.000000 pypdfe-0.1.1/pypdfe_builder/src/PDF-Estimator/.git/FETCH_HEAD
--rw-r--r--   0 nate       (501) staff       (20)       21 2023-06-21 20:32:32.000000 pypdfe-0.1.1/pypdfe_builder/src/PDF-Estimator/.git/HEAD
--rw-r--r--   0 nate       (501) staff       (20)      309 2023-06-21 20:32:32.000000 pypdfe-0.1.1/pypdfe_builder/src/PDF-Estimator/.git/config
--rw-r--r--   0 nate       (501) staff       (20)       73 2023-06-21 20:32:31.000000 pypdfe-0.1.1/pypdfe_builder/src/PDF-Estimator/.git/description
-drwxr-xr-x   0 nate       (501) staff       (20)        0 2023-06-22 04:08:00.407755 pypdfe-0.1.1/pypdfe_builder/src/PDF-Estimator/.git/hooks/
--rwxr-xr-x   0 nate       (501) staff       (20)      478 2023-06-21 20:32:31.000000 pypdfe-0.1.1/pypdfe_builder/src/PDF-Estimator/.git/hooks/applypatch-msg.sample
--rwxr-xr-x   0 nate       (501) staff       (20)      896 2023-06-21 20:32:31.000000 pypdfe-0.1.1/pypdfe_builder/src/PDF-Estimator/.git/hooks/commit-msg.sample
--rwxr-xr-x   0 nate       (501) staff       (20)     4726 2023-06-21 20:32:31.000000 pypdfe-0.1.1/pypdfe_builder/src/PDF-Estimator/.git/hooks/fsmonitor-watchman.sample
--rwxr-xr-x   0 nate       (501) staff       (20)      189 2023-06-21 20:32:31.000000 pypdfe-0.1.1/pypdfe_builder/src/PDF-Estimator/.git/hooks/post-update.sample
--rwxr-xr-x   0 nate       (501) staff       (20)      424 2023-06-21 20:32:31.000000 pypdfe-0.1.1/pypdfe_builder/src/PDF-Estimator/.git/hooks/pre-applypatch.sample
--rwxr-xr-x   0 nate       (501) staff       (20)     1643 2023-06-21 20:32:31.000000 pypdfe-0.1.1/pypdfe_builder/src/PDF-Estimator/.git/hooks/pre-commit.sample
--rwxr-xr-x   0 nate       (501) staff       (20)      416 2023-06-21 20:32:31.000000 pypdfe-0.1.1/pypdfe_builder/src/PDF-Estimator/.git/hooks/pre-merge-commit.sample
--rwxr-xr-x   0 nate       (501) staff       (20)     1374 2023-06-21 20:32:31.000000 pypdfe-0.1.1/pypdfe_builder/src/PDF-Estimator/.git/hooks/pre-push.sample
--rwxr-xr-x   0 nate       (501) staff       (20)     4898 2023-06-21 20:32:31.000000 pypdfe-0.1.1/pypdfe_builder/src/PDF-Estimator/.git/hooks/pre-rebase.sample
--rwxr-xr-x   0 nate       (501) staff       (20)      544 2023-06-21 20:32:31.000000 pypdfe-0.1.1/pypdfe_builder/src/PDF-Estimator/.git/hooks/pre-receive.sample
--rwxr-xr-x   0 nate       (501) staff       (20)     1492 2023-06-21 20:32:31.000000 pypdfe-0.1.1/pypdfe_builder/src/PDF-Estimator/.git/hooks/prepare-commit-msg.sample
--rwxr-xr-x   0 nate       (501) staff       (20)     2783 2023-06-21 20:32:31.000000 pypdfe-0.1.1/pypdfe_builder/src/PDF-Estimator/.git/hooks/push-to-checkout.sample
--rwxr-xr-x   0 nate       (501) staff       (20)     3650 2023-06-21 20:32:31.000000 pypdfe-0.1.1/pypdfe_builder/src/PDF-Estimator/.git/hooks/update.sample
--rw-r--r--   0 nate       (501) staff       (20)     2102 2023-06-22 03:25:25.000000 pypdfe-0.1.1/pypdfe_builder/src/PDF-Estimator/.git/index
-drwxr-xr-x   0 nate       (501) staff       (20)        0 2023-06-22 04:08:00.407883 pypdfe-0.1.1/pypdfe_builder/src/PDF-Estimator/.git/info/
--rw-r--r--   0 nate       (501) staff       (20)      240 2023-06-21 20:32:31.000000 pypdfe-0.1.1/pypdfe_builder/src/PDF-Estimator/.git/info/exclude
-drwxr-xr-x   0 nate       (501) staff       (20)        0 2023-06-22 04:08:00.408002 pypdfe-0.1.1/pypdfe_builder/src/PDF-Estimator/.git/logs/
--rw-r--r--   0 nate       (501) staff       (20)      213 2023-06-21 20:32:32.000000 pypdfe-0.1.1/pypdfe_builder/src/PDF-Estimator/.git/logs/HEAD
-drwxr-xr-x   0 nate       (501) staff       (20)        0 2023-06-22 04:08:00.401063 pypdfe-0.1.1/pypdfe_builder/src/PDF-Estimator/.git/logs/refs/
-drwxr-xr-x   0 nate       (501) staff       (20)        0 2023-06-22 04:08:00.408120 pypdfe-0.1.1/pypdfe_builder/src/PDF-Estimator/.git/logs/refs/heads/
--rw-r--r--   0 nate       (501) staff       (20)      213 2023-06-21 20:32:32.000000 pypdfe-0.1.1/pypdfe_builder/src/PDF-Estimator/.git/logs/refs/heads/main
-drwxr-xr-x   0 nate       (501) staff       (20)        0 2023-06-22 04:08:00.401103 pypdfe-0.1.1/pypdfe_builder/src/PDF-Estimator/.git/logs/refs/remotes/
-drwxr-xr-x   0 nate       (501) staff       (20)        0 2023-06-22 04:08:00.408238 pypdfe-0.1.1/pypdfe_builder/src/PDF-Estimator/.git/logs/refs/remotes/origin/
--rw-r--r--   0 nate       (501) staff       (20)      213 2023-06-21 20:32:32.000000 pypdfe-0.1.1/pypdfe_builder/src/PDF-Estimator/.git/logs/refs/remotes/origin/HEAD
-drwxr-xr-x   0 nate       (501) staff       (20)        0 2023-06-22 04:08:00.401207 pypdfe-0.1.1/pypdfe_builder/src/PDF-Estimator/.git/objects/
-drwxr-xr-x   0 nate       (501) staff       (20)        0 2023-06-22 04:08:00.408496 pypdfe-0.1.1/pypdfe_builder/src/PDF-Estimator/.git/objects/pack/
--r--r--r--   0 nate       (501) staff       (20)     1996 2023-06-21 20:32:32.000000 pypdfe-0.1.1/pypdfe_builder/src/PDF-Estimator/.git/objects/pack/pack-68fcf6d5b1d91b28c20241431b9241a5762ddad3.idx
--r--r--r--   0 nate       (501) staff       (20)    47733 2023-06-21 20:32:32.000000 pypdfe-0.1.1/pypdfe_builder/src/PDF-Estimator/.git/objects/pack/pack-68fcf6d5b1d91b28c20241431b9241a5762ddad3.pack
--rw-r--r--   0 nate       (501) staff       (20)      112 2023-06-21 20:32:32.000000 pypdfe-0.1.1/pypdfe_builder/src/PDF-Estimator/.git/packed-refs
-drwxr-xr-x   0 nate       (501) staff       (20)        0 2023-06-22 04:08:00.401367 pypdfe-0.1.1/pypdfe_builder/src/PDF-Estimator/.git/refs/
-drwxr-xr-x   0 nate       (501) staff       (20)        0 2023-06-22 04:08:00.408642 pypdfe-0.1.1/pypdfe_builder/src/PDF-Estimator/.git/refs/heads/
--rw-r--r--   0 nate       (501) staff       (20)       41 2023-06-21 20:32:32.000000 pypdfe-0.1.1/pypdfe_builder/src/PDF-Estimator/.git/refs/heads/main
-drwxr-xr-x   0 nate       (501) staff       (20)        0 2023-06-22 04:08:00.401415 pypdfe-0.1.1/pypdfe_builder/src/PDF-Estimator/.git/refs/remotes/
-drwxr-xr-x   0 nate       (501) staff       (20)        0 2023-06-22 04:08:00.408744 pypdfe-0.1.1/pypdfe_builder/src/PDF-Estimator/.git/refs/remotes/origin/
--rw-r--r--   0 nate       (501) staff       (20)       30 2023-06-21 20:32:32.000000 pypdfe-0.1.1/pypdfe_builder/src/PDF-Estimator/.git/refs/remotes/origin/HEAD
--rw-r--r--   0 nate       (501) staff       (20)     2947 2023-06-21 20:32:32.000000 pypdfe-0.1.1/pypdfe_builder/src/PDF-Estimator/ChebyShev.cpp
--rw-r--r--   0 nate       (501) staff       (20)     1542 2023-06-21 20:32:32.000000 pypdfe-0.1.1/pypdfe_builder/src/PDF-Estimator/ChebyShev.h
--rw-r--r--   0 nate       (501) staff       (20)     9785 2023-06-21 20:32:32.000000 pypdfe-0.1.1/pypdfe_builder/src/PDF-Estimator/InputData.cpp
--rw-r--r--   0 nate       (501) staff       (20)     2214 2023-06-21 20:32:32.000000 pypdfe-0.1.1/pypdfe_builder/src/PDF-Estimator/InputData.h
--rw-r--r--   0 nate       (501) staff       (20)     8394 2023-06-21 20:32:32.000000 pypdfe-0.1.1/pypdfe_builder/src/PDF-Estimator/InputParameters.cpp
--rw-r--r--   0 nate       (501) staff       (20)     2470 2023-06-21 20:32:32.000000 pypdfe-0.1.1/pypdfe_builder/src/PDF-Estimator/InputParameters.h
--rw-r--r--   0 nate       (501) staff       (20)     4922 2023-06-21 20:32:32.000000 pypdfe-0.1.1/pypdfe_builder/src/PDF-Estimator/JointProbability.cpp
--rw-r--r--   0 nate       (501) staff       (20)     1711 2023-06-21 20:32:32.000000 pypdfe-0.1.1/pypdfe_builder/src/PDF-Estimator/JointProbability.h
--rw-r--r--   0 nate       (501) staff       (20)    35149 2023-06-21 20:32:32.000000 pypdfe-0.1.1/pypdfe_builder/src/PDF-Estimator/LICENSE
--rw-r--r--   0 nate       (501) staff       (20)    17168 2023-06-21 20:32:32.000000 pypdfe-0.1.1/pypdfe_builder/src/PDF-Estimator/MinimizeScore.cpp
--rw-r--r--   0 nate       (501) staff       (20)     2839 2023-06-21 20:32:32.000000 pypdfe-0.1.1/pypdfe_builder/src/PDF-Estimator/MinimizeScore.h
--rw-r--r--   0 nate       (501) staff       (20)     4372 2023-06-21 20:32:32.000000 pypdfe-0.1.1/pypdfe_builder/src/PDF-Estimator/OutputControl.cpp
--rw-r--r--   0 nate       (501) staff       (20)     2028 2023-06-21 20:32:32.000000 pypdfe-0.1.1/pypdfe_builder/src/PDF-Estimator/OutputControl.h
--rw-r--r--   0 nate       (501) staff       (20)      773 2023-06-21 20:32:32.000000 pypdfe-0.1.1/pypdfe_builder/src/PDF-Estimator/README.txt
--rw-r--r--   0 nate       (501) staff       (20)     1959 2023-06-21 20:32:32.000000 pypdfe-0.1.1/pypdfe_builder/src/PDF-Estimator/Score.cpp
--rw-r--r--   0 nate       (501) staff       (20)     1857 2023-06-21 20:32:32.000000 pypdfe-0.1.1/pypdfe_builder/src/PDF-Estimator/Score.h
--rw-r--r--   0 nate       (501) staff       (20)    16156 2023-06-21 20:32:32.000000 pypdfe-0.1.1/pypdfe_builder/src/PDF-Estimator/ScoreQZ.cpp
--rw-r--r--   0 nate       (501) staff       (20)     1410 2023-06-21 20:32:32.000000 pypdfe-0.1.1/pypdfe_builder/src/PDF-Estimator/ScoreQZ.h
--rw-r--r--   0 nate       (501) staff       (20)     5467 2023-06-21 20:32:32.000000 pypdfe-0.1.1/pypdfe_builder/src/PDF-Estimator/Variable.cpp
--rw-r--r--   0 nate       (501) staff       (20)     1995 2023-06-21 20:32:32.000000 pypdfe-0.1.1/pypdfe_builder/src/PDF-Estimator/Variable.h
--rw-r--r--   0 nate       (501) staff       (20)    11691 2023-06-21 20:32:32.000000 pypdfe-0.1.1/pypdfe_builder/src/PDF-Estimator/WriteResults.cpp
--rw-r--r--   0 nate       (501) staff       (20)     2352 2023-06-21 20:32:32.000000 pypdfe-0.1.1/pypdfe_builder/src/PDF-Estimator/WriteResults.h
--rw-r--r--   0 nate       (501) staff       (20)     2407 2023-06-21 20:32:32.000000 pypdfe-0.1.1/pypdfe_builder/src/PDF-Estimator/callPDF.cpp
--rw-r--r--   0 nate       (501) staff       (20)     1007 2023-06-21 20:32:32.000000 pypdfe-0.1.1/pypdfe_builder/src/PDF-Estimator/callPDF.h
--rw-r--r--   0 nate       (501) staff       (20)     1669 2023-06-21 20:32:32.000000 pypdfe-0.1.1/pypdfe_builder/src/PDF-Estimator/mvPDFMain.cpp
--rw-r--r--   0 nate       (501) staff       (20)     1454 2023-06-21 23:11:04.000000 pypdfe-0.1.1/pypdfe_builder/src/main.cpp
-drwxr-xr-x   0 nate       (501) staff       (20)        0 2023-06-22 04:08:00.408854 pypdfe-0.1.1/pypdfe_builder/src/pypdfe/
--rw-r--r--   0 nate       (501) staff       (20)      450 2023-06-21 22:56:29.000000 pypdfe-0.1.1/pypdfe_builder/src/pypdfe/__init__.py
-drwxr-xr-x   0 nate       (501) staff       (20)        0 2023-06-22 04:08:00.408961 pypdfe-0.1.1/pypdfe_builder/src/pypdfe/__pycache__/
--rw-r--r--   0 nate       (501) staff       (20)     1293 2023-06-22 00:50:39.000000 pypdfe-0.1.1/pypdfe_builder/src/pypdfe/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 nate       (501) staff       (20)       38 2023-06-22 04:08:00.409276 pypdfe-0.1.1/setup.cfg
--rw-r--r--   0 nate       (501) staff       (20)     1704 2023-06-22 04:07:51.000000 pypdfe-0.1.1/setup.py
+drwxr-xr-x   0 nate       (501) staff       (20)        0 2023-07-08 18:38:19.847067 pypdfe-0.1.2/
+-rw-r--r--   0 nate       (501) staff       (20)    35148 2023-07-08 07:31:18.000000 pypdfe-0.1.2/LICENSE
+-rw-r--r--   0 nate       (501) staff       (20)      297 2023-07-08 18:38:19.846976 pypdfe-0.1.2/PKG-INFO
+drwxr-xr-x   0 nate       (501) staff       (20)        0 2023-07-08 18:38:19.846098 pypdfe-0.1.2/pypdfe/
+-rw-r--r--   0 nate       (501) staff       (20)     1025 2023-07-08 07:18:43.000000 pypdfe-0.1.2/pypdfe/__init__.py
+drwxr-xr-x   0 nate       (501) staff       (20)        0 2023-07-08 18:38:19.846818 pypdfe-0.1.2/pypdfe.egg-info/
+-rw-r--r--   0 nate       (501) staff       (20)      297 2023-07-08 18:38:19.000000 pypdfe-0.1.2/pypdfe.egg-info/PKG-INFO
+-rw-r--r--   0 nate       (501) staff       (20)     1532 2023-07-08 18:38:19.000000 pypdfe-0.1.2/pypdfe.egg-info/SOURCES.txt
+-rw-r--r--   0 nate       (501) staff       (20)        1 2023-07-08 18:38:19.000000 pypdfe-0.1.2/pypdfe.egg-info/dependency_links.txt
+-rw-r--r--   0 nate       (501) staff       (20)        1 2023-07-08 18:38:19.000000 pypdfe-0.1.2/pypdfe.egg-info/not-zip-safe
+-rw-r--r--   0 nate       (501) staff       (20)       26 2023-07-08 18:38:19.000000 pypdfe-0.1.2/pypdfe.egg-info/requires.txt
+-rw-r--r--   0 nate       (501) staff       (20)        7 2023-07-08 18:38:19.000000 pypdfe-0.1.2/pypdfe.egg-info/top_level.txt
+-rw-r--r--   0 nate       (501) staff       (20)      143 2023-07-08 18:37:36.000000 pypdfe-0.1.2/pyproject.toml
+-rw-r--r--   0 nate       (501) staff       (20)       38 2023-07-08 18:38:19.847100 pypdfe-0.1.2/setup.cfg
+-rw-r--r--   0 nate       (501) staff       (20)     1642 2023-07-08 18:37:36.000000 pypdfe-0.1.2/setup.py
```

### Comparing `pypdfe-0.1.1/pypdfe_builder/src/PDF-Estimator/LICENSE` & `pypdfe-0.1.2/LICENSE`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -667,8 +667,8 @@
 <https://www.gnu.org/licenses/>.
 
   The GNU General Public License does not permit incorporating your program
 into proprietary programs.  If your program is a subroutine library, you
 may consider it more useful to permit linking proprietary applications with
 the library.  If this is what you want to do, use the GNU Lesser General
 Public License instead of this License.  But first, please read
-<https://www.gnu.org/licenses/why-not-lgpl.html>.
+<https://www.gnu.org/licenses/why-not-lgpl.html>.
```

