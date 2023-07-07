# Comparing `tmp/hickleable-0.2.1.tar.gz` & `tmp/hickleable-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hickleable-0.2.1.tar", last modified: Fri Jul  7 19:09:24 2023, max compression
+gzip compressed data, was "hickleable-0.2.2.tar", last modified: Fri Jul  7 23:37:21 2023, max compression
```

## Comparing `hickleable-0.2.1.tar` & `hickleable-0.2.2.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 19:09:24.530201 hickleable-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-07 19:09:10.000000 hickleable-0.2.1/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-07-07 19:09:10.000000 hickleable-0.2.1/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 19:09:24.526201 hickleable-0.2.1/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-07-07 19:09:10.000000 hickleable-0.2.1/.github/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-07-07 19:09:10.000000 hickleable-0.2.1/.github/labels.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-07-07 19:09:10.000000 hickleable-0.2.1/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 19:09:24.526201 hickleable-0.2.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-07-07 19:09:10.000000 hickleable-0.2.1/.github/workflows/auto-merge-deps.yml
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-07-07 19:09:10.000000 hickleable-0.2.1/.github/workflows/check-build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-07-07 19:09:10.000000 hickleable-0.2.1/.github/workflows/deploy.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-07-07 19:09:10.000000 hickleable-0.2.1/.github/workflows/labeler.yml
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-07-07 19:09:10.000000 hickleable-0.2.1/.github/workflows/release-draft.yml
--rw-r--r--   0 runner    (1001) docker     (123)      968 2023-07-07 19:09:10.000000 hickleable-0.2.1/.github/workflows/testsuite.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-07-07 19:09:10.000000 hickleable-0.2.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-07-07 19:09:10.000000 hickleable-0.2.1/.isort.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-07-07 19:09:10.000000 hickleable-0.2.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-07-07 19:09:10.000000 hickleable-0.2.1/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-07 19:09:10.000000 hickleable-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5715 2023-07-07 19:09:24.530201 hickleable-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5260 2023-07-07 19:09:10.000000 hickleable-0.2.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 19:09:24.530201 hickleable-0.2.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     5586 2023-07-07 19:09:10.000000 hickleable-0.2.1/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 19:09:24.530201 hickleable-0.2.1/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-07 19:09:10.000000 hickleable-0.2.1/docs/_static/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-07 19:09:10.000000 hickleable-0.2.1/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8295 2023-07-07 19:09:10.000000 hickleable-0.2.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 19:09:10.000000 hickleable-0.2.1/docs/contents.rst
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-07 19:09:10.000000 hickleable-0.2.1/docs/environment.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 19:09:24.530201 hickleable-0.2.1/docs/faqs/
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-07-07 19:09:10.000000 hickleable-0.2.1/docs/faqs/misc.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-07-07 19:09:10.000000 hickleable-0.2.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-07-07 19:09:10.000000 hickleable-0.2.1/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-07 19:09:10.000000 hickleable-0.2.1/docs/license.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 19:09:24.530201 hickleable-0.2.1/docs/reference/
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-07 19:09:10.000000 hickleable-0.2.1/docs/reference/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 19:09:24.530201 hickleable-0.2.1/docs/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-07-07 19:09:10.000000 hickleable-0.2.1/docs/templates/class.rst
--rw-r--r--   0 runner    (1001) docker     (123)      727 2023-07-07 19:09:10.000000 hickleable-0.2.1/docs/templates/module.rst
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-07-07 19:09:10.000000 hickleable-0.2.1/docs/tutorials.rst
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-07 19:09:10.000000 hickleable-0.2.1/docs/usage.rst
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-07-07 19:09:10.000000 hickleable-0.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-07-07 19:09:24.534201 hickleable-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-07 19:09:10.000000 hickleable-0.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 19:09:24.522201 hickleable-0.2.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 19:09:24.530201 hickleable-0.2.1/src/hickleable/
--rw-r--r--   0 runner    (1001) docker     (123)     9460 2023-07-07 19:09:10.000000 hickleable-0.2.1/src/hickleable/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 19:09:24.530201 hickleable-0.2.1/src/hickleable.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5715 2023-07-07 19:09:24.000000 hickleable-0.2.1/src/hickleable.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-07-07 19:09:24.000000 hickleable-0.2.1/src/hickleable.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 19:09:24.000000 hickleable-0.2.1/src/hickleable.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 19:09:24.000000 hickleable-0.2.1/src/hickleable.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-07-07 19:09:24.000000 hickleable-0.2.1/src/hickleable.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-07 19:09:24.000000 hickleable-0.2.1/src/hickleable.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 19:09:24.530201 hickleable-0.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3692 2023-07-07 19:09:10.000000 hickleable-0.2.1/tests/test_hickleable.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 23:37:21.887752 hickleable-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-07 23:37:12.000000 hickleable-0.2.2/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-07-07 23:37:12.000000 hickleable-0.2.2/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 23:37:21.879752 hickleable-0.2.2/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-07-07 23:37:12.000000 hickleable-0.2.2/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-07-07 23:37:12.000000 hickleable-0.2.2/.github/labels.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-07-07 23:37:12.000000 hickleable-0.2.2/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 23:37:21.879752 hickleable-0.2.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-07-07 23:37:12.000000 hickleable-0.2.2/.github/workflows/auto-merge-deps.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-07-07 23:37:12.000000 hickleable-0.2.2/.github/workflows/check-build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-07-07 23:37:12.000000 hickleable-0.2.2/.github/workflows/deploy.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-07-07 23:37:12.000000 hickleable-0.2.2/.github/workflows/labeler.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-07-07 23:37:12.000000 hickleable-0.2.2/.github/workflows/release-draft.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-07-07 23:37:12.000000 hickleable-0.2.2/.github/workflows/testsuite.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-07-07 23:37:12.000000 hickleable-0.2.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-07-07 23:37:12.000000 hickleable-0.2.2/.isort.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-07-07 23:37:12.000000 hickleable-0.2.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-07-07 23:37:12.000000 hickleable-0.2.2/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-07 23:37:12.000000 hickleable-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5715 2023-07-07 23:37:21.887752 hickleable-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5260 2023-07-07 23:37:12.000000 hickleable-0.2.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 23:37:21.883751 hickleable-0.2.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     5586 2023-07-07 23:37:12.000000 hickleable-0.2.2/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 23:37:21.883751 hickleable-0.2.2/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-07 23:37:12.000000 hickleable-0.2.2/docs/_static/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-07 23:37:12.000000 hickleable-0.2.2/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8295 2023-07-07 23:37:12.000000 hickleable-0.2.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 23:37:12.000000 hickleable-0.2.2/docs/contents.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-07 23:37:12.000000 hickleable-0.2.2/docs/environment.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 23:37:21.883751 hickleable-0.2.2/docs/faqs/
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-07-07 23:37:12.000000 hickleable-0.2.2/docs/faqs/misc.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-07-07 23:37:12.000000 hickleable-0.2.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-07-07 23:37:12.000000 hickleable-0.2.2/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-07 23:37:12.000000 hickleable-0.2.2/docs/license.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 23:37:21.883751 hickleable-0.2.2/docs/reference/
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-07 23:37:12.000000 hickleable-0.2.2/docs/reference/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 23:37:21.883751 hickleable-0.2.2/docs/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-07-07 23:37:12.000000 hickleable-0.2.2/docs/templates/class.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2023-07-07 23:37:12.000000 hickleable-0.2.2/docs/templates/module.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-07-07 23:37:12.000000 hickleable-0.2.2/docs/tutorials.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-07 23:37:12.000000 hickleable-0.2.2/docs/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-07-07 23:37:12.000000 hickleable-0.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-07-07 23:37:21.887752 hickleable-0.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-07 23:37:12.000000 hickleable-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 23:37:21.871751 hickleable-0.2.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 23:37:21.883751 hickleable-0.2.2/src/hickleable/
+-rw-r--r--   0 runner    (1001) docker     (123)     9170 2023-07-07 23:37:12.000000 hickleable-0.2.2/src/hickleable/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 23:37:21.887752 hickleable-0.2.2/src/hickleable.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5715 2023-07-07 23:37:21.000000 hickleable-0.2.2/src/hickleable.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-07-07 23:37:21.000000 hickleable-0.2.2/src/hickleable.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 23:37:21.000000 hickleable-0.2.2/src/hickleable.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 23:37:21.000000 hickleable-0.2.2/src/hickleable.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-07-07 23:37:21.000000 hickleable-0.2.2/src/hickleable.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-07 23:37:21.000000 hickleable-0.2.2/src/hickleable.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 23:37:21.887752 hickleable-0.2.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3692 2023-07-07 23:37:12.000000 hickleable-0.2.2/tests/test_hickleable.py
```

### Comparing `hickleable-0.2.1/.github/labels.yml` & `hickleable-0.2.2/.github/labels.yml`

 * *Files identical despite different names*

### Comparing `hickleable-0.2.1/.github/release-drafter.yml` & `hickleable-0.2.2/.github/release-drafter.yml`

 * *Files identical despite different names*

### Comparing `hickleable-0.2.1/.github/workflows/check-build.yml` & `hickleable-0.2.2/.github/workflows/check-build.yml`

 * *Files identical despite different names*

### Comparing `hickleable-0.2.1/.github/workflows/deploy.yaml` & `hickleable-0.2.2/.github/workflows/deploy.yaml`

 * *Files identical despite different names*

### Comparing `hickleable-0.2.1/.github/workflows/testsuite.yaml` & `hickleable-0.2.2/.github/workflows/testsuite.yaml`

 * *Files identical despite different names*

### Comparing `hickleable-0.2.1/.gitignore` & `hickleable-0.2.2/.gitignore`

 * *Files identical despite different names*

### Comparing `hickleable-0.2.1/.pre-commit-config.yaml` & `hickleable-0.2.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `hickleable-0.2.1/.readthedocs.yml` & `hickleable-0.2.2/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `hickleable-0.2.1/LICENSE` & `hickleable-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `hickleable-0.2.1/PKG-INFO` & `hickleable-0.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hickleable
-Version: 0.2.1
+Version: 0.2.2
 Summary: A simple decorator to make your classes hickle-able
 Home-page: https://github.com/steven-murray/hickleable
 Author: Steven Murray
 License: mit
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
```

### Comparing `hickleable-0.2.1/README.rst` & `hickleable-0.2.2/README.rst`

 * *Files identical despite different names*

### Comparing `hickleable-0.2.1/docs/Makefile` & `hickleable-0.2.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `hickleable-0.2.1/docs/conf.py` & `hickleable-0.2.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `hickleable-0.2.1/docs/index.rst` & `hickleable-0.2.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `hickleable-0.2.1/docs/templates/class.rst` & `hickleable-0.2.2/docs/templates/class.rst`

 * *Files identical despite different names*

### Comparing `hickleable-0.2.1/docs/templates/module.rst` & `hickleable-0.2.2/docs/templates/module.rst`

 * *Files identical despite different names*

### Comparing `hickleable-0.2.1/setup.cfg` & `hickleable-0.2.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `hickleable-0.2.1/src/hickleable/__init__.py` & `hickleable-0.2.2/src/hickleable/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,23 +10,82 @@
 import warnings
 from functools import cached_property
 from h5py import AttributeManager, Group
 from hickle.lookup import LoaderManager, PyContainer
 from pathlib import Path
 from typing import Any, Callable, Iterable, List, Tuple
 
+try:
+    import attrs
+except ImportError:
+    attrs = None
+
 DumpOutput = Tuple[Group, List[Tuple[str, Any, dict, dict]]]
 DumpFunctionType = Callable[[Any, Group, str], DumpOutput]
 
 try:
     import yaml
 except ImportError:
     yaml = None
 
 
+class _LoadContainer(PyContainer):  # noqa: N801
+    def __init__(self, h5_attrs: dict, base_type: str, object_type: Any):
+        """The load container.
+
+        Parameters
+        ----------
+        h5_attrs
+            the attrs dictionary attached to the group representing the
+            custom class.
+        base_type
+            byte string naming the loader to be used for restoring the
+            custom class object
+        py_obj_type
+            Custom class (or subclass)
+        """
+        # the optional protected _content parameter of the PyContainer
+        # __init__ method can be used to change the data structure used to
+        # store the subitems passed to the append method of the PyContainer
+        # class per default it is set to []
+        super().__init__(h5_attrs, base_type, object_type, _content=dict(h5_attrs))
+
+    def append(self, name: str, item: Any, h5_attrs: AttributeManager):
+        """Add a particular item to the content defining the object.
+
+        Parameters
+        ----------
+        name
+            Identifies the subitem within the parent ``hdf5.Group``
+        item
+            The object representing the subitem
+        h5_attrs
+            An ``attrs`` dictionary attached to the ``h5py.Dataset`` or
+            ``h5py.Group`` representing the item.
+        """
+        self._content[name] = item
+
+    def convert(self):
+        """Convert the content read from file to the object itself."""
+        # py_obj_type should point to MyClass or any of its subclasses
+        new_instance = self.object_type.__new__(self.object_type)
+
+        if hasattr(new_instance, "__sethstate__"):
+            new_instance.__sethstate__(self._content)
+        elif hasattr(new_instance, "__setstate__"):
+            new_instance.__setstate__(self._content)
+        else:
+            new_instance.__dict__.update(self._content)
+
+        if hasattr(new_instance, "__attrs_post_init__"):
+            new_instance.__attrs_post_init__()
+
+        return new_instance
+
+
 def hickleable(
     hkl_str: bytes | None = None,
     dump_function: None | DumpFunctionType = None,
     load_container: None | Callable[[Any], PyContainer] | PyContainer = None,
     metadata_keys: Iterable[str] | None = None,
     evaluate_cached_properties: bool = False,
     **kwargs,
@@ -108,16 +167,20 @@
                     for cp in all_cached_properties:
                         getattr(py_obj, cp)
 
                 if hasattr(py_obj, "__gethstate__"):
                     state = py_obj.__gethstate__()
                 elif hasattr(py_obj, "__getstate__"):
                     state = py_obj.__getstate__()
-                else:
+                elif py_obj.__dict__ is not None:
                     state = py_obj.__dict__
+                elif attrs is not None and attrs.has(py_obj):
+                    state = attrs.asdict(py_obj)
+                else:
+                    state = {}
 
                 for k in metadata_keys or []:
                     if k in state:
                         ds.attrs[k] = state.pop(k)
                     else:
                         warnings.warn(
                             f"Ignoring metadata key {k} since it's not in the object.",
@@ -130,70 +193,15 @@
 
                 return ds, subitems
 
         else:
             _dump_function = dump_function  # pragma: no cover
 
         if load_container is None:
-
-            class _load_container(PyContainer):  # noqa: N801
-                def __init__(self, h5_attrs: dict, base_type: str, object_type: Any):
-                    """The load container.
-
-                    Parameters
-                    ----------
-                    h5_attrs
-                        the attrs dictionary attached to the group representing the
-                        custom class.
-                    base_type
-                        byte string naming the loader to be used for restoring the
-                        custom class object
-                    py_obj_type
-                        Custom class (or subclass)
-                    """
-                    # the optional protected _content parameter of the PyContainer
-                    # __init__ method can be used to change the data structure used to
-                    # store the subitems passed to the append method of the PyContainer
-                    # class per default it is set to []
-                    super().__init__(
-                        h5_attrs, base_type, object_type, _content=dict(h5_attrs)
-                    )
-
-                def append(self, name: str, item: Any, h5_attrs: AttributeManager):
-                    """Add a particular item to the content defining the object.
-
-                    Parameters
-                    ----------
-                    name
-                        Identifies the subitem within the parent ``hdf5.Group``
-                    item
-                        The object representing the subitem
-                    h5_attrs
-                        An ``attrs`` dictionary attached to the ``h5py.Dataset`` or
-                        ``h5py.Group`` representing the item.
-                    """
-                    self._content[name] = item
-
-                def convert(self):
-                    """Convert the content read from file to the object itself."""
-                    # py_obj_type should point to MyClass or any of its subclasses
-                    new_instance = self.object_type.__new__(self.object_type)
-
-                    if hasattr(new_instance, "__sethstate__"):
-                        new_instance.__sethstate__(self._content)
-                    elif hasattr(new_instance, "__setstate__"):
-                        new_instance.__setstate__(self._content)
-                    else:
-                        new_instance.__dict__.update(self._content)
-
-                    if hasattr(new_instance, "__attrs_post_init__"):
-                        new_instance.__attrs_post_init__()
-
-                    return new_instance
-
+            _load_container = _LoadContainer
         else:
             _load_container = (
                 load_container(cls) if callable(load_container) else load_container
             )
 
         LoaderManager.register_class(
             cls,
```

### Comparing `hickleable-0.2.1/src/hickleable.egg-info/PKG-INFO` & `hickleable-0.2.2/src/hickleable.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hickleable
-Version: 0.2.1
+Version: 0.2.2
 Summary: A simple decorator to make your classes hickle-able
 Home-page: https://github.com/steven-murray/hickleable
 Author: Steven Murray
 License: mit
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
```

### Comparing `hickleable-0.2.1/src/hickleable.egg-info/SOURCES.txt` & `hickleable-0.2.2/src/hickleable.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hickleable-0.2.1/tests/test_hickleable.py` & `hickleable-0.2.2/tests/test_hickleable.py`

 * *Files identical despite different names*

