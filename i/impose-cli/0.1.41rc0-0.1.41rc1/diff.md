# Comparing `tmp/impose-cli-0.1.41rc0.tar.gz` & `tmp/impose-cli-0.1.41rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "impose-cli-0.1.41rc0.tar", last modified: Sat Jul  8 14:28:30 2023, max compression
+gzip compressed data, was "impose-cli-0.1.41rc1.tar", last modified: Sat Jul  8 14:38:55 2023, max compression
```

## Comparing `impose-cli-0.1.41rc0.tar` & `impose-cli-0.1.41rc1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:28:30.783914 impose-cli-0.1.41rc0/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-08 14:28:08.000000 impose-cli-0.1.41rc0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-07-08 14:28:30.779914 impose-cli-0.1.41rc0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-07-08 14:28:08.000000 impose-cli-0.1.41rc0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:28:30.779914 impose-cli-0.1.41rc0/impose_cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 14:28:08.000000 impose-cli-0.1.41rc0/impose_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12087 2023-07-08 14:28:08.000000 impose-cli-0.1.41rc0/impose_cli/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-08 14:28:08.000000 impose-cli-0.1.41rc0/impose_cli/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 14:28:08.000000 impose-cli-0.1.41rc0/impose_cli/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-07-08 14:28:08.000000 impose-cli-0.1.41rc0/impose_cli/impose_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     5029 2023-07-08 14:28:08.000000 impose-cli-0.1.41rc0/impose_cli/impose_cli_2.py
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-07-08 14:28:08.000000 impose-cli-0.1.41rc0/impose_cli/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:28:30.779914 impose-cli-0.1.41rc0/impose_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-07-08 14:28:30.000000 impose-cli-0.1.41rc0/impose_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-07-08 14:28:30.000000 impose-cli-0.1.41rc0/impose_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 14:28:30.000000 impose-cli-0.1.41rc0/impose_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-08 14:28:30.000000 impose-cli-0.1.41rc0/impose_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-08 14:28:30.000000 impose-cli-0.1.41rc0/impose_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 14:28:30.783914 impose-cli-0.1.41rc0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      510 2023-07-08 14:28:08.000000 impose-cli-0.1.41rc0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:28:30.779914 impose-cli-0.1.41rc0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 14:28:08.000000 impose-cli-0.1.41rc0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-07-08 14:28:08.000000 impose-cli-0.1.41rc0/tests/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:38:55.596831 impose-cli-0.1.41rc1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-08 14:38:33.000000 impose-cli-0.1.41rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-07-08 14:38:55.596831 impose-cli-0.1.41rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-07-08 14:38:33.000000 impose-cli-0.1.41rc1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:38:55.592831 impose-cli-0.1.41rc1/impose_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-08 14:38:33.000000 impose-cli-0.1.41rc1/impose_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12087 2023-07-08 14:38:33.000000 impose-cli-0.1.41rc1/impose_cli/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-08 14:38:33.000000 impose-cli-0.1.41rc1/impose_cli/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 14:38:33.000000 impose-cli-0.1.41rc1/impose_cli/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-07-08 14:38:33.000000 impose-cli-0.1.41rc1/impose_cli/impose_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5029 2023-07-08 14:38:33.000000 impose-cli-0.1.41rc1/impose_cli/impose_cli_2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-07-08 14:38:33.000000 impose-cli-0.1.41rc1/impose_cli/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:38:55.596831 impose-cli-0.1.41rc1/impose_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-07-08 14:38:55.000000 impose-cli-0.1.41rc1/impose_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-07-08 14:38:55.000000 impose-cli-0.1.41rc1/impose_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 14:38:55.000000 impose-cli-0.1.41rc1/impose_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-08 14:38:55.000000 impose-cli-0.1.41rc1/impose_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-08 14:38:55.000000 impose-cli-0.1.41rc1/impose_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 14:38:55.596831 impose-cli-0.1.41rc1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-07-08 14:38:33.000000 impose-cli-0.1.41rc1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:38:55.596831 impose-cli-0.1.41rc1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 14:38:33.000000 impose-cli-0.1.41rc1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-07-08 14:38:33.000000 impose-cli-0.1.41rc1/tests/test.py
```

### Comparing `impose-cli-0.1.41rc0/LICENSE` & `impose-cli-0.1.41rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `impose-cli-0.1.41rc0/impose_cli/_utils.py` & `impose-cli-0.1.41rc1/impose_cli/_utils.py`

 * *Files identical despite different names*

### Comparing `impose-cli-0.1.41rc0/impose_cli/impose_cli.py` & `impose-cli-0.1.41rc1/impose_cli/impose_cli.py`

 * *Files identical despite different names*

### Comparing `impose-cli-0.1.41rc0/impose_cli/impose_cli_2.py` & `impose-cli-0.1.41rc1/impose_cli/impose_cli_2.py`

 * *Files identical despite different names*

