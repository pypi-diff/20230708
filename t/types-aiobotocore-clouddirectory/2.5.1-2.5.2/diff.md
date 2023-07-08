# Comparing `tmp/types-aiobotocore-clouddirectory-2.5.1.tar.gz` & `tmp/types-aiobotocore-clouddirectory-2.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-clouddirectory-2.5.1.tar", last modified: Wed Jun 28 01:43:13 2023, max compression
+gzip compressed data, was "types-aiobotocore-clouddirectory-2.5.2.tar", last modified: Sat Jul  8 01:43:21 2023, max compression
```

## Comparing `types-aiobotocore-clouddirectory-2.5.1.tar` & `types-aiobotocore-clouddirectory-2.5.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 01:43:13.290107 types-aiobotocore-clouddirectory-2.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-28 01:27:16.000000 types-aiobotocore-clouddirectory-2.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    26375 2023-06-28 01:43:13.290107 types-aiobotocore-clouddirectory-2.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    24782 2023-06-28 01:27:16.000000 types-aiobotocore-clouddirectory-2.5.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-28 01:43:13.290107 types-aiobotocore-clouddirectory-2.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-06-28 01:27:16.000000 types-aiobotocore-clouddirectory-2.5.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 01:43:13.286107 types-aiobotocore-clouddirectory-2.5.1/types_aiobotocore_clouddirectory/
--rw-r--r--   0 runner    (1001) docker     (123)     4839 2023-06-28 01:27:16.000000 types-aiobotocore-clouddirectory-2.5.1/types_aiobotocore_clouddirectory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4838 2023-06-28 01:27:16.000000 types-aiobotocore-clouddirectory-2.5.1/types_aiobotocore_clouddirectory/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-06-28 01:27:16.000000 types-aiobotocore-clouddirectory-2.5.1/types_aiobotocore_clouddirectory/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    59759 2023-06-28 01:27:16.000000 types-aiobotocore-clouddirectory-2.5.1/types_aiobotocore_clouddirectory/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    59665 2023-06-28 01:27:16.000000 types-aiobotocore-clouddirectory-2.5.1/types_aiobotocore_clouddirectory/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11877 2023-06-28 01:27:17.000000 types-aiobotocore-clouddirectory-2.5.1/types_aiobotocore_clouddirectory/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    11875 2023-06-28 01:27:17.000000 types-aiobotocore-clouddirectory-2.5.1/types_aiobotocore_clouddirectory/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    25363 2023-06-28 01:27:17.000000 types-aiobotocore-clouddirectory-2.5.1/types_aiobotocore_clouddirectory/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    25342 2023-06-28 01:27:17.000000 types-aiobotocore-clouddirectory-2.5.1/types_aiobotocore_clouddirectory/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 01:27:16.000000 types-aiobotocore-clouddirectory-2.5.1/types_aiobotocore_clouddirectory/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    86520 2023-06-28 01:27:19.000000 types-aiobotocore-clouddirectory-2.5.1/types_aiobotocore_clouddirectory/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    86393 2023-06-28 01:27:18.000000 types-aiobotocore-clouddirectory-2.5.1/types_aiobotocore_clouddirectory/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-28 01:27:16.000000 types-aiobotocore-clouddirectory-2.5.1/types_aiobotocore_clouddirectory/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 01:43:13.290107 types-aiobotocore-clouddirectory-2.5.1/types_aiobotocore_clouddirectory.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    26375 2023-06-28 01:43:13.000000 types-aiobotocore-clouddirectory-2.5.1/types_aiobotocore_clouddirectory.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      946 2023-06-28 01:43:13.000000 types-aiobotocore-clouddirectory-2.5.1/types_aiobotocore_clouddirectory.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 01:43:13.000000 types-aiobotocore-clouddirectory-2.5.1/types_aiobotocore_clouddirectory.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 01:43:13.000000 types-aiobotocore-clouddirectory-2.5.1/types_aiobotocore_clouddirectory.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-28 01:43:13.000000 types-aiobotocore-clouddirectory-2.5.1/types_aiobotocore_clouddirectory.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-28 01:43:13.000000 types-aiobotocore-clouddirectory-2.5.1/types_aiobotocore_clouddirectory.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:21.313821 types-aiobotocore-clouddirectory-2.5.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:26:52.000000 types-aiobotocore-clouddirectory-2.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    26375 2023-07-08 01:43:21.309821 types-aiobotocore-clouddirectory-2.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    24782 2023-07-08 01:26:52.000000 types-aiobotocore-clouddirectory-2.5.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:43:21.313821 types-aiobotocore-clouddirectory-2.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-07-08 01:26:52.000000 types-aiobotocore-clouddirectory-2.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:21.305821 types-aiobotocore-clouddirectory-2.5.2/types_aiobotocore_clouddirectory/
+-rw-r--r--   0 runner    (1001) docker     (123)     4839 2023-07-08 01:26:52.000000 types-aiobotocore-clouddirectory-2.5.2/types_aiobotocore_clouddirectory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4838 2023-07-08 01:26:52.000000 types-aiobotocore-clouddirectory-2.5.2/types_aiobotocore_clouddirectory/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-07-08 01:26:52.000000 types-aiobotocore-clouddirectory-2.5.2/types_aiobotocore_clouddirectory/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59759 2023-07-08 01:26:53.000000 types-aiobotocore-clouddirectory-2.5.2/types_aiobotocore_clouddirectory/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59665 2023-07-08 01:26:52.000000 types-aiobotocore-clouddirectory-2.5.2/types_aiobotocore_clouddirectory/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11877 2023-07-08 01:26:53.000000 types-aiobotocore-clouddirectory-2.5.2/types_aiobotocore_clouddirectory/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11875 2023-07-08 01:26:53.000000 types-aiobotocore-clouddirectory-2.5.2/types_aiobotocore_clouddirectory/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    25363 2023-07-08 01:26:53.000000 types-aiobotocore-clouddirectory-2.5.2/types_aiobotocore_clouddirectory/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25342 2023-07-08 01:26:53.000000 types-aiobotocore-clouddirectory-2.5.2/types_aiobotocore_clouddirectory/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:26:52.000000 types-aiobotocore-clouddirectory-2.5.2/types_aiobotocore_clouddirectory/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    86520 2023-07-08 01:26:55.000000 types-aiobotocore-clouddirectory-2.5.2/types_aiobotocore_clouddirectory/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    86393 2023-07-08 01:26:54.000000 types-aiobotocore-clouddirectory-2.5.2/types_aiobotocore_clouddirectory/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:26:52.000000 types-aiobotocore-clouddirectory-2.5.2/types_aiobotocore_clouddirectory/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:21.309821 types-aiobotocore-clouddirectory-2.5.2/types_aiobotocore_clouddirectory.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    26375 2023-07-08 01:43:21.000000 types-aiobotocore-clouddirectory-2.5.2/types_aiobotocore_clouddirectory.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-07-08 01:43:21.000000 types-aiobotocore-clouddirectory-2.5.2/types_aiobotocore_clouddirectory.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:21.000000 types-aiobotocore-clouddirectory-2.5.2/types_aiobotocore_clouddirectory.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:21.000000 types-aiobotocore-clouddirectory-2.5.2/types_aiobotocore_clouddirectory.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:43:21.000000 types-aiobotocore-clouddirectory-2.5.2/types_aiobotocore_clouddirectory.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-08 01:43:21.000000 types-aiobotocore-clouddirectory-2.5.2/types_aiobotocore_clouddirectory.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-clouddirectory-2.5.1/LICENSE` & `types-aiobotocore-clouddirectory-2.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-clouddirectory-2.5.1/PKG-INFO` & `types-aiobotocore-clouddirectory-2.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-clouddirectory
-Version: 2.5.1
-Summary: Type annotations for aiobotocore.CloudDirectory 2.5.1 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2
+Summary: Type annotations for aiobotocore.CloudDirectory 2.5.2 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_clouddirectory/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-clouddirectory.svg?color=blue)](https://pypi.org/project/types-aiobotocore-clouddirectory)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_clouddirectory/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-clouddirectory?color=blue)](https://pypistats.org/packages/types-aiobotocore-clouddirectory)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.CloudDirectory 2.5.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory)
+[aiobotocore.CloudDirectory 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-clouddirectory-2.5.1/README.md` & `types-aiobotocore-clouddirectory-2.5.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-clouddirectory.svg?color=blue)](https://pypi.org/project/types-aiobotocore-clouddirectory)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_clouddirectory/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-clouddirectory?color=blue)](https://pypistats.org/packages/types-aiobotocore-clouddirectory)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.CloudDirectory 2.5.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory)
+[aiobotocore.CloudDirectory 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-clouddirectory-2.5.1/setup.py` & `types-aiobotocore-clouddirectory-2.5.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-clouddirectory",
-    version="2.5.1",
+    version="2.5.2",
     packages=["types_aiobotocore_clouddirectory"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.CloudDirectory 2.5.1 service generated with"
+        "Type annotations for aiobotocore.CloudDirectory 2.5.2 service generated with"
         " mypy-boto3-builder 7.14.5"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-clouddirectory-2.5.1/types_aiobotocore_clouddirectory/__init__.py` & `types-aiobotocore-clouddirectory-2.5.2/types_aiobotocore_clouddirectory/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-clouddirectory-2.5.1/types_aiobotocore_clouddirectory/__init__.pyi` & `types-aiobotocore-clouddirectory-2.5.2/types_aiobotocore_clouddirectory/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-clouddirectory-2.5.1/types_aiobotocore_clouddirectory/__main__.py` & `types-aiobotocore-clouddirectory-2.5.2/types_aiobotocore_clouddirectory/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.CloudDirectory 2.5.1\nVersion:         2.5.1\nBuilder"
+        "Type annotations for aiobotocore.CloudDirectory 2.5.2\nVersion:         2.5.2\nBuilder"
         " version: 7.14.5\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_clouddirectory//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory\nOther"
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

### Comparing `types-aiobotocore-clouddirectory-2.5.1/types_aiobotocore_clouddirectory/client.py` & `types-aiobotocore-clouddirectory-2.5.2/types_aiobotocore_clouddirectory/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-clouddirectory-2.5.1/types_aiobotocore_clouddirectory/client.pyi` & `types-aiobotocore-clouddirectory-2.5.2/types_aiobotocore_clouddirectory/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-clouddirectory-2.5.1/types_aiobotocore_clouddirectory/literals.py` & `types-aiobotocore-clouddirectory-2.5.2/types_aiobotocore_clouddirectory/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-clouddirectory-2.5.1/types_aiobotocore_clouddirectory/literals.pyi` & `types-aiobotocore-clouddirectory-2.5.2/types_aiobotocore_clouddirectory/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-clouddirectory-2.5.1/types_aiobotocore_clouddirectory/paginator.py` & `types-aiobotocore-clouddirectory-2.5.2/types_aiobotocore_clouddirectory/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-clouddirectory-2.5.1/types_aiobotocore_clouddirectory/paginator.pyi` & `types-aiobotocore-clouddirectory-2.5.2/types_aiobotocore_clouddirectory/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-clouddirectory-2.5.1/types_aiobotocore_clouddirectory/type_defs.py` & `types-aiobotocore-clouddirectory-2.5.2/types_aiobotocore_clouddirectory/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-clouddirectory-2.5.1/types_aiobotocore_clouddirectory/type_defs.pyi` & `types-aiobotocore-clouddirectory-2.5.2/types_aiobotocore_clouddirectory/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-clouddirectory-2.5.1/types_aiobotocore_clouddirectory.egg-info/PKG-INFO` & `types-aiobotocore-clouddirectory-2.5.2/types_aiobotocore_clouddirectory.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-clouddirectory
-Version: 2.5.1
-Summary: Type annotations for aiobotocore.CloudDirectory 2.5.1 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2
+Summary: Type annotations for aiobotocore.CloudDirectory 2.5.2 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_clouddirectory/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-clouddirectory.svg?color=blue)](https://pypi.org/project/types-aiobotocore-clouddirectory)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_clouddirectory/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-clouddirectory?color=blue)](https://pypistats.org/packages/types-aiobotocore-clouddirectory)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.CloudDirectory 2.5.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory)
+[aiobotocore.CloudDirectory 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-clouddirectory-2.5.1/types_aiobotocore_clouddirectory.egg-info/SOURCES.txt` & `types-aiobotocore-clouddirectory-2.5.2/types_aiobotocore_clouddirectory.egg-info/SOURCES.txt`

 * *Files identical despite different names*

