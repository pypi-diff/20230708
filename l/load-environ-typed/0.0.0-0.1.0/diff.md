# Comparing `tmp/load_environ_typed-0.0.0.tar.gz` & `tmp/load_environ_typed-0.1.0.tar.gz`

## Comparing `load_environ_typed-0.0.0.tar` & `load_environ_typed-0.1.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 load_environ_typed-0.0.0/Makefile
--rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 load_environ_typed-0.0.0/password.txt
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 load_environ_typed-0.0.0/requirements-dev.txt
--rw-r--r--   0        0        0     4288 2020-02-02 00:00:00.000000 load_environ_typed-0.0.0/test.py
--rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 load_environ_typed-0.0.0/.github/workflows/workflow.yml
--rw-r--r--   0        0        0     2619 2020-02-02 00:00:00.000000 load_environ_typed-0.0.0/load_environ_typed/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 load_environ_typed-0.0.0/load_environ_typed/py.typed
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 load_environ_typed-0.0.0/.gitignore
--rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 load_environ_typed-0.0.0/LICENSE.txt
--rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 load_environ_typed-0.0.0/README.md
--rw-r--r--   0        0        0      662 2020-02-02 00:00:00.000000 load_environ_typed-0.0.0/pyproject.toml
--rw-r--r--   0        0        0     2463 2020-02-02 00:00:00.000000 load_environ_typed-0.0.0/PKG-INFO
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 load_environ_typed-0.1.0/Makefile
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 load_environ_typed-0.1.0/password.txt
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 load_environ_typed-0.1.0/requirements-dev.txt
+-rw-r--r--   0        0        0     4288 2020-02-02 00:00:00.000000 load_environ_typed-0.1.0/test.py
+-rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 load_environ_typed-0.1.0/.github/workflows/workflow.yml
+-rw-r--r--   0        0        0     2619 2020-02-02 00:00:00.000000 load_environ_typed-0.1.0/load_environ_typed/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 load_environ_typed-0.1.0/load_environ_typed/py.typed
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 load_environ_typed-0.1.0/.gitignore
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 load_environ_typed-0.1.0/LICENSE.txt
+-rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 load_environ_typed-0.1.0/README.md
+-rw-r--r--   0        0        0      662 2020-02-02 00:00:00.000000 load_environ_typed-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     2441 2020-02-02 00:00:00.000000 load_environ_typed-0.1.0/PKG-INFO
```

### Comparing `load_environ_typed-0.0.0/test.py` & `load_environ_typed-0.1.0/test.py`

 * *Files identical despite different names*

### Comparing `load_environ_typed-0.0.0/.github/workflows/workflow.yml` & `load_environ_typed-0.1.0/.github/workflows/workflow.yml`

 * *Files identical despite different names*

### Comparing `load_environ_typed-0.0.0/load_environ_typed/__init__.py` & `load_environ_typed-0.1.0/load_environ_typed/__init__.py`

 * *Files identical despite different names*

### Comparing `load_environ_typed-0.0.0/LICENSE.txt` & `load_environ_typed-0.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `load_environ_typed-0.0.0/README.md` & `load_environ_typed-0.1.0/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -29,9 +29,9 @@
 make test
 ```
 
 ## Deploying
 
 ```sh
 venv/bin/python -m build
-venv/bin/python -m twine upload --repository testpypi dist/*
+venv/bin/python -m twine upload dist/*
 ```
```

### Comparing `load_environ_typed-0.0.0/pyproject.toml` & `load_environ_typed-0.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "load-environ-typed"
-version = "0.0.0"
+version = "0.1.0"
 authors = [
   { name="Johan B.W. de Vries" },
 ]
 description = "You define a class, we load i up from environment in a type safe way"
 readme = "README.md"
 license = {file = "LICENSE.txt" }
 requires-python = ">=3.7"
```

### Comparing `load_environ_typed-0.0.0/PKG-INFO` & `load_environ_typed-0.1.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: load-environ-typed
-Version: 0.0.0
+Version: 0.1.0
 Summary: You define a class, we load i up from environment in a type safe way
 Project-URL: Homepage, https://github.com/jbwdevries/python-load-environ-typed
 Project-URL: Bug Tracker, https://github.com/jbwdevries/python-load-environ-typed/issues
 Author: Johan B.W. de Vries
 License: Copyright (c) 2023, Johan B.W. de Vries
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -62,9 +62,9 @@
 make test
 ```
 
 ## Deploying
 
 ```sh
 venv/bin/python -m build
-venv/bin/python -m twine upload --repository testpypi dist/*
+venv/bin/python -m twine upload dist/*
 ```
```

