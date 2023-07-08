# Comparing `tmp/types-aiobotocore-cloudsearch-2.5.1.tar.gz` & `tmp/types-aiobotocore-cloudsearch-2.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-cloudsearch-2.5.1.tar", last modified: Wed Jun 28 01:43:13 2023, max compression
+gzip compressed data, was "types-aiobotocore-cloudsearch-2.5.2.tar", last modified: Sat Jul  8 01:43:21 2023, max compression
```

## Comparing `types-aiobotocore-cloudsearch-2.5.1.tar` & `types-aiobotocore-cloudsearch-2.5.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 01:43:13.490107 types-aiobotocore-cloudsearch-2.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-28 01:27:33.000000 types-aiobotocore-cloudsearch-2.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15550 2023-06-28 01:43:13.490107 types-aiobotocore-cloudsearch-2.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13969 2023-06-28 01:27:33.000000 types-aiobotocore-cloudsearch-2.5.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-28 01:43:13.490107 types-aiobotocore-cloudsearch-2.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-06-28 01:27:33.000000 types-aiobotocore-cloudsearch-2.5.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 01:43:13.490107 types-aiobotocore-cloudsearch-2.5.1/types_aiobotocore_cloudsearch/
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-06-28 01:27:33.000000 types-aiobotocore-cloudsearch-2.5.1/types_aiobotocore_cloudsearch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      473 2023-06-28 01:27:33.000000 types-aiobotocore-cloudsearch-2.5.1/types_aiobotocore_cloudsearch/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-06-28 01:27:33.000000 types-aiobotocore-cloudsearch-2.5.1/types_aiobotocore_cloudsearch/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20176 2023-06-28 01:27:34.000000 types-aiobotocore-cloudsearch-2.5.1/types_aiobotocore_cloudsearch/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    20142 2023-06-28 01:27:34.000000 types-aiobotocore-cloudsearch-2.5.1/types_aiobotocore_cloudsearch/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9412 2023-06-28 01:27:34.000000 types-aiobotocore-cloudsearch-2.5.1/types_aiobotocore_cloudsearch/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9410 2023-06-28 01:27:34.000000 types-aiobotocore-cloudsearch-2.5.1/types_aiobotocore_cloudsearch/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 01:27:33.000000 types-aiobotocore-cloudsearch-2.5.1/types_aiobotocore_cloudsearch/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    25551 2023-06-28 01:27:34.000000 types-aiobotocore-cloudsearch-2.5.1/types_aiobotocore_cloudsearch/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    25526 2023-06-28 01:27:34.000000 types-aiobotocore-cloudsearch-2.5.1/types_aiobotocore_cloudsearch/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-28 01:27:33.000000 types-aiobotocore-cloudsearch-2.5.1/types_aiobotocore_cloudsearch/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 01:43:13.490107 types-aiobotocore-cloudsearch-2.5.1/types_aiobotocore_cloudsearch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15550 2023-06-28 01:43:13.000000 types-aiobotocore-cloudsearch-2.5.1/types_aiobotocore_cloudsearch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-06-28 01:43:13.000000 types-aiobotocore-cloudsearch-2.5.1/types_aiobotocore_cloudsearch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 01:43:13.000000 types-aiobotocore-cloudsearch-2.5.1/types_aiobotocore_cloudsearch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 01:43:13.000000 types-aiobotocore-cloudsearch-2.5.1/types_aiobotocore_cloudsearch.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-28 01:43:13.000000 types-aiobotocore-cloudsearch-2.5.1/types_aiobotocore_cloudsearch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-28 01:43:13.000000 types-aiobotocore-cloudsearch-2.5.1/types_aiobotocore_cloudsearch.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:21.649827 types-aiobotocore-cloudsearch-2.5.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:27:09.000000 types-aiobotocore-cloudsearch-2.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15550 2023-07-08 01:43:21.641827 types-aiobotocore-cloudsearch-2.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13969 2023-07-08 01:27:09.000000 types-aiobotocore-cloudsearch-2.5.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:43:21.649827 types-aiobotocore-cloudsearch-2.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-07-08 01:27:09.000000 types-aiobotocore-cloudsearch-2.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:21.637827 types-aiobotocore-cloudsearch-2.5.2/types_aiobotocore_cloudsearch/
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-07-08 01:27:09.000000 types-aiobotocore-cloudsearch-2.5.2/types_aiobotocore_cloudsearch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-07-08 01:27:09.000000 types-aiobotocore-cloudsearch-2.5.2/types_aiobotocore_cloudsearch/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-07-08 01:27:10.000000 types-aiobotocore-cloudsearch-2.5.2/types_aiobotocore_cloudsearch/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20176 2023-07-08 01:27:10.000000 types-aiobotocore-cloudsearch-2.5.2/types_aiobotocore_cloudsearch/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20142 2023-07-08 01:27:10.000000 types-aiobotocore-cloudsearch-2.5.2/types_aiobotocore_cloudsearch/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9412 2023-07-08 01:27:10.000000 types-aiobotocore-cloudsearch-2.5.2/types_aiobotocore_cloudsearch/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9410 2023-07-08 01:27:10.000000 types-aiobotocore-cloudsearch-2.5.2/types_aiobotocore_cloudsearch/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:27:10.000000 types-aiobotocore-cloudsearch-2.5.2/types_aiobotocore_cloudsearch/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    25551 2023-07-08 01:27:11.000000 types-aiobotocore-cloudsearch-2.5.2/types_aiobotocore_cloudsearch/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25526 2023-07-08 01:27:11.000000 types-aiobotocore-cloudsearch-2.5.2/types_aiobotocore_cloudsearch/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:27:09.000000 types-aiobotocore-cloudsearch-2.5.2/types_aiobotocore_cloudsearch/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:21.641827 types-aiobotocore-cloudsearch-2.5.2/types_aiobotocore_cloudsearch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15550 2023-07-08 01:43:21.000000 types-aiobotocore-cloudsearch-2.5.2/types_aiobotocore_cloudsearch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-07-08 01:43:21.000000 types-aiobotocore-cloudsearch-2.5.2/types_aiobotocore_cloudsearch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:21.000000 types-aiobotocore-cloudsearch-2.5.2/types_aiobotocore_cloudsearch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:21.000000 types-aiobotocore-cloudsearch-2.5.2/types_aiobotocore_cloudsearch.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:43:21.000000 types-aiobotocore-cloudsearch-2.5.2/types_aiobotocore_cloudsearch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-08 01:43:21.000000 types-aiobotocore-cloudsearch-2.5.2/types_aiobotocore_cloudsearch.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-cloudsearch-2.5.1/LICENSE` & `types-aiobotocore-cloudsearch-2.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudsearch-2.5.1/PKG-INFO` & `types-aiobotocore-cloudsearch-2.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-cloudsearch
-Version: 2.5.1
-Summary: Type annotations for aiobotocore.CloudSearch 2.5.1 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2
+Summary: Type annotations for aiobotocore.CloudSearch 2.5.2 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudsearch/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-cloudsearch.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cloudsearch)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudsearch/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-cloudsearch?color=blue)](https://pypistats.org/packages/types-aiobotocore-cloudsearch)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.CloudSearch 2.5.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudsearch.html#CloudSearch)
+[aiobotocore.CloudSearch 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudsearch.html#CloudSearch)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-cloudsearch-2.5.1/README.md` & `types-aiobotocore-cloudsearch-2.5.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-cloudsearch.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cloudsearch)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudsearch/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-cloudsearch?color=blue)](https://pypistats.org/packages/types-aiobotocore-cloudsearch)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.CloudSearch 2.5.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudsearch.html#CloudSearch)
+[aiobotocore.CloudSearch 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudsearch.html#CloudSearch)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-cloudsearch-2.5.1/setup.py` & `types-aiobotocore-cloudsearch-2.5.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-cloudsearch",
-    version="2.5.1",
+    version="2.5.2",
     packages=["types_aiobotocore_cloudsearch"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.CloudSearch 2.5.1 service generated with"
+        "Type annotations for aiobotocore.CloudSearch 2.5.2 service generated with"
         " mypy-boto3-builder 7.14.5"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-cloudsearch-2.5.1/types_aiobotocore_cloudsearch/__main__.py` & `types-aiobotocore-cloudsearch-2.5.2/types_aiobotocore_cloudsearch/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.CloudSearch 2.5.1\nVersion:         2.5.1\nBuilder"
+        "Type annotations for aiobotocore.CloudSearch 2.5.2\nVersion:         2.5.2\nBuilder"
         " version: 7.14.5\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudsearch//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudsearch.html#CloudSearch\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("2.5.1")
+    print("2.5.2")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `types-aiobotocore-cloudsearch-2.5.1/types_aiobotocore_cloudsearch/client.py` & `types-aiobotocore-cloudsearch-2.5.2/types_aiobotocore_cloudsearch/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudsearch-2.5.1/types_aiobotocore_cloudsearch/client.pyi` & `types-aiobotocore-cloudsearch-2.5.2/types_aiobotocore_cloudsearch/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudsearch-2.5.1/types_aiobotocore_cloudsearch/literals.py` & `types-aiobotocore-cloudsearch-2.5.2/types_aiobotocore_cloudsearch/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudsearch-2.5.1/types_aiobotocore_cloudsearch/literals.pyi` & `types-aiobotocore-cloudsearch-2.5.2/types_aiobotocore_cloudsearch/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudsearch-2.5.1/types_aiobotocore_cloudsearch/type_defs.py` & `types-aiobotocore-cloudsearch-2.5.2/types_aiobotocore_cloudsearch/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudsearch-2.5.1/types_aiobotocore_cloudsearch/type_defs.pyi` & `types-aiobotocore-cloudsearch-2.5.2/types_aiobotocore_cloudsearch/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudsearch-2.5.1/types_aiobotocore_cloudsearch.egg-info/PKG-INFO` & `types-aiobotocore-cloudsearch-2.5.2/types_aiobotocore_cloudsearch.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-cloudsearch
-Version: 2.5.1
-Summary: Type annotations for aiobotocore.CloudSearch 2.5.1 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2
+Summary: Type annotations for aiobotocore.CloudSearch 2.5.2 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudsearch/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-cloudsearch.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cloudsearch)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudsearch/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-cloudsearch?color=blue)](https://pypistats.org/packages/types-aiobotocore-cloudsearch)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.CloudSearch 2.5.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudsearch.html#CloudSearch)
+[aiobotocore.CloudSearch 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudsearch.html#CloudSearch)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-cloudsearch-2.5.1/types_aiobotocore_cloudsearch.egg-info/SOURCES.txt` & `types-aiobotocore-cloudsearch-2.5.2/types_aiobotocore_cloudsearch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

