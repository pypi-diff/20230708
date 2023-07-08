# Comparing `tmp/trab_devops_ci_cd_process-0.0.5.tar.gz` & `tmp/trab_devops_ci_cd_process-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trab_devops_ci_cd_process-0.0.5.tar", last modified: Sat Jul  8 18:10:26 2023, max compression
+gzip compressed data, was "trab_devops_ci_cd_process-0.0.6.tar", last modified: Sat Jul  8 18:46:54 2023, max compression
```

## Comparing `trab_devops_ci_cd_process-0.0.5.tar` & `trab_devops_ci_cd_process-0.0.6.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 18:10:26.918766 trab_devops_ci_cd_process-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-07-08 18:10:14.000000 trab_devops_ci_cd_process-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-07-08 18:10:26.918766 trab_devops_ci_cd_process-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-07-08 18:10:14.000000 trab_devops_ci_cd_process-0.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      893 2023-07-08 18:10:14.000000 trab_devops_ci_cd_process-0.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-07-08 18:10:14.000000 trab_devops_ci_cd_process-0.0.5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 18:10:26.918766 trab_devops_ci_cd_process-0.0.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 18:10:26.918766 trab_devops_ci_cd_process-0.0.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 18:10:26.918766 trab_devops_ci_cd_process-0.0.5/src/bhaskara/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 18:10:14.000000 trab_devops_ci_cd_process-0.0.5/src/bhaskara/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-07-08 18:10:14.000000 trab_devops_ci_cd_process-0.0.5/src/bhaskara/eq_bhaskara.py
--rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-07-08 18:10:14.000000 trab_devops_ci_cd_process-0.0.5/src/bhaskara/eq_segundo_grau.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 18:10:26.918766 trab_devops_ci_cd_process-0.0.5/src/trab_devops_ci_cd_process.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-07-08 18:10:26.000000 trab_devops_ci_cd_process-0.0.5/src/trab_devops_ci_cd_process.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-07-08 18:10:26.000000 trab_devops_ci_cd_process-0.0.5/src/trab_devops_ci_cd_process.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 18:10:26.000000 trab_devops_ci_cd_process-0.0.5/src/trab_devops_ci_cd_process.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-08 18:10:26.000000 trab_devops_ci_cd_process-0.0.5/src/trab_devops_ci_cd_process.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-08 18:10:26.000000 trab_devops_ci_cd_process-0.0.5/src/trab_devops_ci_cd_process.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 18:10:26.918766 trab_devops_ci_cd_process-0.0.5/test/
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-07-08 18:10:14.000000 trab_devops_ci_cd_process-0.0.5/test/test_solucao.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 18:46:54.088642 trab_devops_ci_cd_process-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-07-08 18:46:44.000000 trab_devops_ci_cd_process-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-07-08 18:46:54.088642 trab_devops_ci_cd_process-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-07-08 18:46:44.000000 trab_devops_ci_cd_process-0.0.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      893 2023-07-08 18:46:44.000000 trab_devops_ci_cd_process-0.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-07-08 18:46:44.000000 trab_devops_ci_cd_process-0.0.6/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 18:46:54.088642 trab_devops_ci_cd_process-0.0.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 18:46:54.088642 trab_devops_ci_cd_process-0.0.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 18:46:54.088642 trab_devops_ci_cd_process-0.0.6/src/bhaskara/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 18:46:44.000000 trab_devops_ci_cd_process-0.0.6/src/bhaskara/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-07-08 18:46:44.000000 trab_devops_ci_cd_process-0.0.6/src/bhaskara/eq_bhaskara.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-07-08 18:46:44.000000 trab_devops_ci_cd_process-0.0.6/src/bhaskara/eq_segundo_grau.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 18:46:54.088642 trab_devops_ci_cd_process-0.0.6/src/trab_devops_ci_cd_process.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-07-08 18:46:54.000000 trab_devops_ci_cd_process-0.0.6/src/trab_devops_ci_cd_process.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-07-08 18:46:54.000000 trab_devops_ci_cd_process-0.0.6/src/trab_devops_ci_cd_process.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 18:46:54.000000 trab_devops_ci_cd_process-0.0.6/src/trab_devops_ci_cd_process.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-08 18:46:54.000000 trab_devops_ci_cd_process-0.0.6/src/trab_devops_ci_cd_process.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-08 18:46:54.000000 trab_devops_ci_cd_process-0.0.6/src/trab_devops_ci_cd_process.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 18:46:54.088642 trab_devops_ci_cd_process-0.0.6/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-07-08 18:46:44.000000 trab_devops_ci_cd_process-0.0.6/test/test_solucao.py
```

### Comparing `trab_devops_ci_cd_process-0.0.5/LICENSE` & `trab_devops_ci_cd_process-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `trab_devops_ci_cd_process-0.0.5/pyproject.toml` & `trab_devops_ci_cd_process-0.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 # informações do projeto para envio ao pypi.org
 [project]
 name = "trab_devops_ci_cd_process"
-version = "0.0.5"
+version = "0.0.6"
 authors = [
   { name="Ricardo Báfica Pontes", email="ricardo.bafica@gmail.com" },
 ]
 description = "quadratic equation roots calculating package for devops course"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `trab_devops_ci_cd_process-0.0.5/src/bhaskara/eq_bhaskara.py` & `trab_devops_ci_cd_process-0.0.6/src/bhaskara/eq_bhaskara.py`

 * *Files identical despite different names*

### Comparing `trab_devops_ci_cd_process-0.0.5/src/bhaskara/eq_segundo_grau.py` & `trab_devops_ci_cd_process-0.0.6/src/bhaskara/eq_segundo_grau.py`

 * *Files identical despite different names*

### Comparing `trab_devops_ci_cd_process-0.0.5/test/test_solucao.py` & `trab_devops_ci_cd_process-0.0.6/test/test_solucao.py`

 * *Files identical despite different names*

