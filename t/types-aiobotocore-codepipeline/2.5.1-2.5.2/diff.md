# Comparing `tmp/types-aiobotocore-codepipeline-2.5.1.tar.gz` & `tmp/types-aiobotocore-codepipeline-2.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-codepipeline-2.5.1.tar", last modified: Wed Jun 28 01:43:16 2023, max compression
+gzip compressed data, was "types-aiobotocore-codepipeline-2.5.2.tar", last modified: Sat Jul  8 01:43:25 2023, max compression
```

## Comparing `types-aiobotocore-codepipeline-2.5.1.tar` & `types-aiobotocore-codepipeline-2.5.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 01:43:16.878113 types-aiobotocore-codepipeline-2.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-28 01:28:01.000000 types-aiobotocore-codepipeline-2.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    19520 2023-06-28 01:43:16.878113 types-aiobotocore-codepipeline-2.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17935 2023-06-28 01:28:01.000000 types-aiobotocore-codepipeline-2.5.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-28 01:43:16.878113 types-aiobotocore-codepipeline-2.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-06-28 01:28:01.000000 types-aiobotocore-codepipeline-2.5.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 01:43:16.878113 types-aiobotocore-codepipeline-2.5.1/types_aiobotocore_codepipeline/
--rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-06-28 01:28:01.000000 types-aiobotocore-codepipeline-2.5.1/types_aiobotocore_codepipeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-06-28 01:28:01.000000 types-aiobotocore-codepipeline-2.5.1/types_aiobotocore_codepipeline/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-06-28 01:28:01.000000 types-aiobotocore-codepipeline-2.5.1/types_aiobotocore_codepipeline/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    34378 2023-06-28 01:28:01.000000 types-aiobotocore-codepipeline-2.5.1/types_aiobotocore_codepipeline/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    34324 2023-06-28 01:28:01.000000 types-aiobotocore-codepipeline-2.5.1/types_aiobotocore_codepipeline/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10770 2023-06-28 01:28:02.000000 types-aiobotocore-codepipeline-2.5.1/types_aiobotocore_codepipeline/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10768 2023-06-28 01:28:02.000000 types-aiobotocore-codepipeline-2.5.1/types_aiobotocore_codepipeline/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8008 2023-06-28 01:28:01.000000 types-aiobotocore-codepipeline-2.5.1/types_aiobotocore_codepipeline/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8000 2023-06-28 01:28:01.000000 types-aiobotocore-codepipeline-2.5.1/types_aiobotocore_codepipeline/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 01:28:01.000000 types-aiobotocore-codepipeline-2.5.1/types_aiobotocore_codepipeline/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    46263 2023-06-28 01:28:03.000000 types-aiobotocore-codepipeline-2.5.1/types_aiobotocore_codepipeline/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    46202 2023-06-28 01:28:02.000000 types-aiobotocore-codepipeline-2.5.1/types_aiobotocore_codepipeline/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-28 01:28:01.000000 types-aiobotocore-codepipeline-2.5.1/types_aiobotocore_codepipeline/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 01:43:16.878113 types-aiobotocore-codepipeline-2.5.1/types_aiobotocore_codepipeline.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19520 2023-06-28 01:43:16.000000 types-aiobotocore-codepipeline-2.5.1/types_aiobotocore_codepipeline.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-06-28 01:43:16.000000 types-aiobotocore-codepipeline-2.5.1/types_aiobotocore_codepipeline.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 01:43:16.000000 types-aiobotocore-codepipeline-2.5.1/types_aiobotocore_codepipeline.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 01:43:16.000000 types-aiobotocore-codepipeline-2.5.1/types_aiobotocore_codepipeline.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-28 01:43:16.000000 types-aiobotocore-codepipeline-2.5.1/types_aiobotocore_codepipeline.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-28 01:43:16.000000 types-aiobotocore-codepipeline-2.5.1/types_aiobotocore_codepipeline.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:25.101893 types-aiobotocore-codepipeline-2.5.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:27:38.000000 types-aiobotocore-codepipeline-2.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    19520 2023-07-08 01:43:25.093893 types-aiobotocore-codepipeline-2.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17935 2023-07-08 01:27:38.000000 types-aiobotocore-codepipeline-2.5.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:43:25.101893 types-aiobotocore-codepipeline-2.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-07-08 01:27:38.000000 types-aiobotocore-codepipeline-2.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:25.093893 types-aiobotocore-codepipeline-2.5.2/types_aiobotocore_codepipeline/
+-rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-07-08 01:27:38.000000 types-aiobotocore-codepipeline-2.5.2/types_aiobotocore_codepipeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-07-08 01:27:38.000000 types-aiobotocore-codepipeline-2.5.2/types_aiobotocore_codepipeline/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-07-08 01:27:38.000000 types-aiobotocore-codepipeline-2.5.2/types_aiobotocore_codepipeline/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34378 2023-07-08 01:27:39.000000 types-aiobotocore-codepipeline-2.5.2/types_aiobotocore_codepipeline/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34324 2023-07-08 01:27:39.000000 types-aiobotocore-codepipeline-2.5.2/types_aiobotocore_codepipeline/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10770 2023-07-08 01:27:39.000000 types-aiobotocore-codepipeline-2.5.2/types_aiobotocore_codepipeline/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10768 2023-07-08 01:27:39.000000 types-aiobotocore-codepipeline-2.5.2/types_aiobotocore_codepipeline/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8008 2023-07-08 01:27:39.000000 types-aiobotocore-codepipeline-2.5.2/types_aiobotocore_codepipeline/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8000 2023-07-08 01:27:39.000000 types-aiobotocore-codepipeline-2.5.2/types_aiobotocore_codepipeline/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:27:38.000000 types-aiobotocore-codepipeline-2.5.2/types_aiobotocore_codepipeline/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    46263 2023-07-08 01:27:40.000000 types-aiobotocore-codepipeline-2.5.2/types_aiobotocore_codepipeline/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46202 2023-07-08 01:27:39.000000 types-aiobotocore-codepipeline-2.5.2/types_aiobotocore_codepipeline/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:27:38.000000 types-aiobotocore-codepipeline-2.5.2/types_aiobotocore_codepipeline/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:25.093893 types-aiobotocore-codepipeline-2.5.2/types_aiobotocore_codepipeline.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19520 2023-07-08 01:43:24.000000 types-aiobotocore-codepipeline-2.5.2/types_aiobotocore_codepipeline.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-07-08 01:43:24.000000 types-aiobotocore-codepipeline-2.5.2/types_aiobotocore_codepipeline.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:24.000000 types-aiobotocore-codepipeline-2.5.2/types_aiobotocore_codepipeline.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:24.000000 types-aiobotocore-codepipeline-2.5.2/types_aiobotocore_codepipeline.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:43:24.000000 types-aiobotocore-codepipeline-2.5.2/types_aiobotocore_codepipeline.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-08 01:43:24.000000 types-aiobotocore-codepipeline-2.5.2/types_aiobotocore_codepipeline.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-codepipeline-2.5.1/LICENSE` & `types-aiobotocore-codepipeline-2.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codepipeline-2.5.1/PKG-INFO` & `types-aiobotocore-codepipeline-2.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-codepipeline
-Version: 2.5.1
-Summary: Type annotations for aiobotocore.CodePipeline 2.5.1 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2
+Summary: Type annotations for aiobotocore.CodePipeline 2.5.2 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codepipeline/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-codepipeline.svg?color=blue)](https://pypi.org/project/types-aiobotocore-codepipeline)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codepipeline/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-codepipeline?color=blue)](https://pypistats.org/packages/types-aiobotocore-codepipeline)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.CodePipeline 2.5.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline)
+[aiobotocore.CodePipeline 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-codepipeline-2.5.1/README.md` & `types-aiobotocore-codepipeline-2.5.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-codepipeline.svg?color=blue)](https://pypi.org/project/types-aiobotocore-codepipeline)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codepipeline/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-codepipeline?color=blue)](https://pypistats.org/packages/types-aiobotocore-codepipeline)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.CodePipeline 2.5.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline)
+[aiobotocore.CodePipeline 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-codepipeline-2.5.1/setup.py` & `types-aiobotocore-codepipeline-2.5.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-codepipeline",
-    version="2.5.1",
+    version="2.5.2",
     packages=["types_aiobotocore_codepipeline"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.CodePipeline 2.5.1 service generated with"
+        "Type annotations for aiobotocore.CodePipeline 2.5.2 service generated with"
         " mypy-boto3-builder 7.14.5"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-codepipeline-2.5.1/types_aiobotocore_codepipeline/__init__.py` & `types-aiobotocore-codepipeline-2.5.2/types_aiobotocore_codepipeline/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codepipeline-2.5.1/types_aiobotocore_codepipeline/__init__.pyi` & `types-aiobotocore-codepipeline-2.5.2/types_aiobotocore_codepipeline/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codepipeline-2.5.1/types_aiobotocore_codepipeline/__main__.py` & `types-aiobotocore-codepipeline-2.5.2/types_aiobotocore_codepipeline/__main__.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.CodePipeline 2.5.1\nVersion:         2.5.1\nBuilder"
+        "Type annotations for aiobotocore.CodePipeline 2.5.2\nVersion:         2.5.2\nBuilder"
         " version: 7.14.5\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codepipeline//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline\nOther"
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

### Comparing `types-aiobotocore-codepipeline-2.5.1/types_aiobotocore_codepipeline/client.py` & `types-aiobotocore-codepipeline-2.5.2/types_aiobotocore_codepipeline/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codepipeline-2.5.1/types_aiobotocore_codepipeline/client.pyi` & `types-aiobotocore-codepipeline-2.5.2/types_aiobotocore_codepipeline/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codepipeline-2.5.1/types_aiobotocore_codepipeline/literals.py` & `types-aiobotocore-codepipeline-2.5.2/types_aiobotocore_codepipeline/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codepipeline-2.5.1/types_aiobotocore_codepipeline/literals.pyi` & `types-aiobotocore-codepipeline-2.5.2/types_aiobotocore_codepipeline/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codepipeline-2.5.1/types_aiobotocore_codepipeline/paginator.py` & `types-aiobotocore-codepipeline-2.5.2/types_aiobotocore_codepipeline/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codepipeline-2.5.1/types_aiobotocore_codepipeline/paginator.pyi` & `types-aiobotocore-codepipeline-2.5.2/types_aiobotocore_codepipeline/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codepipeline-2.5.1/types_aiobotocore_codepipeline/type_defs.py` & `types-aiobotocore-codepipeline-2.5.2/types_aiobotocore_codepipeline/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codepipeline-2.5.1/types_aiobotocore_codepipeline/type_defs.pyi` & `types-aiobotocore-codepipeline-2.5.2/types_aiobotocore_codepipeline/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codepipeline-2.5.1/types_aiobotocore_codepipeline.egg-info/PKG-INFO` & `types-aiobotocore-codepipeline-2.5.2/types_aiobotocore_codepipeline.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-codepipeline
-Version: 2.5.1
-Summary: Type annotations for aiobotocore.CodePipeline 2.5.1 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2
+Summary: Type annotations for aiobotocore.CodePipeline 2.5.2 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codepipeline/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-codepipeline.svg?color=blue)](https://pypi.org/project/types-aiobotocore-codepipeline)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codepipeline/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-codepipeline?color=blue)](https://pypistats.org/packages/types-aiobotocore-codepipeline)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.CodePipeline 2.5.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline)
+[aiobotocore.CodePipeline 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-codepipeline-2.5.1/types_aiobotocore_codepipeline.egg-info/SOURCES.txt` & `types-aiobotocore-codepipeline-2.5.2/types_aiobotocore_codepipeline.egg-info/SOURCES.txt`

 * *Files identical despite different names*

