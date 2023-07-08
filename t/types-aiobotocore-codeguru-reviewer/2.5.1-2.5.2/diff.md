# Comparing `tmp/types-aiobotocore-codeguru-reviewer-2.5.1.tar.gz` & `tmp/types-aiobotocore-codeguru-reviewer-2.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-codeguru-reviewer-2.5.1.tar", last modified: Wed Jun 28 01:43:15 2023, max compression
+gzip compressed data, was "types-aiobotocore-codeguru-reviewer-2.5.2.tar", last modified: Sat Jul  8 01:43:23 2023, max compression
```

## Comparing `types-aiobotocore-codeguru-reviewer-2.5.1.tar` & `types-aiobotocore-codeguru-reviewer-2.5.2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 01:43:15.750111 types-aiobotocore-codeguru-reviewer-2.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-28 01:27:57.000000 types-aiobotocore-codeguru-reviewer-2.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16972 2023-06-28 01:43:15.746111 types-aiobotocore-codeguru-reviewer-2.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15368 2023-06-28 01:27:57.000000 types-aiobotocore-codeguru-reviewer-2.5.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-28 01:43:15.750111 types-aiobotocore-codeguru-reviewer-2.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-06-28 01:27:57.000000 types-aiobotocore-codeguru-reviewer-2.5.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 01:43:15.746111 types-aiobotocore-codeguru-reviewer-2.5.1/types_aiobotocore_codeguru_reviewer/
--rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-06-28 01:27:57.000000 types-aiobotocore-codeguru-reviewer-2.5.1/types_aiobotocore_codeguru_reviewer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-06-28 01:27:57.000000 types-aiobotocore-codeguru-reviewer-2.5.1/types_aiobotocore_codeguru_reviewer/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-06-28 01:27:57.000000 types-aiobotocore-codeguru-reviewer-2.5.1/types_aiobotocore_codeguru_reviewer/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16599 2023-06-28 01:27:57.000000 types-aiobotocore-codeguru-reviewer-2.5.1/types_aiobotocore_codeguru_reviewer/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    16573 2023-06-28 01:27:57.000000 types-aiobotocore-codeguru-reviewer-2.5.1/types_aiobotocore_codeguru_reviewer/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9667 2023-06-28 01:27:57.000000 types-aiobotocore-codeguru-reviewer-2.5.1/types_aiobotocore_codeguru_reviewer/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9665 2023-06-28 01:27:57.000000 types-aiobotocore-codeguru-reviewer-2.5.1/types_aiobotocore_codeguru_reviewer/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2544 2023-06-28 01:27:57.000000 types-aiobotocore-codeguru-reviewer-2.5.1/types_aiobotocore_codeguru_reviewer/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2541 2023-06-28 01:27:57.000000 types-aiobotocore-codeguru-reviewer-2.5.1/types_aiobotocore_codeguru_reviewer/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 01:27:57.000000 types-aiobotocore-codeguru-reviewer-2.5.1/types_aiobotocore_codeguru_reviewer/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    21025 2023-06-28 01:27:58.000000 types-aiobotocore-codeguru-reviewer-2.5.1/types_aiobotocore_codeguru_reviewer/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    21003 2023-06-28 01:27:57.000000 types-aiobotocore-codeguru-reviewer-2.5.1/types_aiobotocore_codeguru_reviewer/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-28 01:27:57.000000 types-aiobotocore-codeguru-reviewer-2.5.1/types_aiobotocore_codeguru_reviewer/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2858 2023-06-28 01:27:57.000000 types-aiobotocore-codeguru-reviewer-2.5.1/types_aiobotocore_codeguru_reviewer/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-06-28 01:27:57.000000 types-aiobotocore-codeguru-reviewer-2.5.1/types_aiobotocore_codeguru_reviewer/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 01:43:15.746111 types-aiobotocore-codeguru-reviewer-2.5.1/types_aiobotocore_codeguru_reviewer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16972 2023-06-28 01:43:15.000000 types-aiobotocore-codeguru-reviewer-2.5.1/types_aiobotocore_codeguru_reviewer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-06-28 01:43:15.000000 types-aiobotocore-codeguru-reviewer-2.5.1/types_aiobotocore_codeguru_reviewer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 01:43:15.000000 types-aiobotocore-codeguru-reviewer-2.5.1/types_aiobotocore_codeguru_reviewer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 01:43:15.000000 types-aiobotocore-codeguru-reviewer-2.5.1/types_aiobotocore_codeguru_reviewer.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-28 01:43:15.000000 types-aiobotocore-codeguru-reviewer-2.5.1/types_aiobotocore_codeguru_reviewer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-28 01:43:15.000000 types-aiobotocore-codeguru-reviewer-2.5.1/types_aiobotocore_codeguru_reviewer.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:23.861869 types-aiobotocore-codeguru-reviewer-2.5.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:27:33.000000 types-aiobotocore-codeguru-reviewer-2.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16972 2023-07-08 01:43:23.857869 types-aiobotocore-codeguru-reviewer-2.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15368 2023-07-08 01:27:33.000000 types-aiobotocore-codeguru-reviewer-2.5.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:43:23.861869 types-aiobotocore-codeguru-reviewer-2.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-07-08 01:27:33.000000 types-aiobotocore-codeguru-reviewer-2.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:23.857869 types-aiobotocore-codeguru-reviewer-2.5.2/types_aiobotocore_codeguru_reviewer/
+-rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-07-08 01:27:33.000000 types-aiobotocore-codeguru-reviewer-2.5.2/types_aiobotocore_codeguru_reviewer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-07-08 01:27:33.000000 types-aiobotocore-codeguru-reviewer-2.5.2/types_aiobotocore_codeguru_reviewer/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-07-08 01:27:33.000000 types-aiobotocore-codeguru-reviewer-2.5.2/types_aiobotocore_codeguru_reviewer/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16599 2023-07-08 01:27:34.000000 types-aiobotocore-codeguru-reviewer-2.5.2/types_aiobotocore_codeguru_reviewer/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16573 2023-07-08 01:27:33.000000 types-aiobotocore-codeguru-reviewer-2.5.2/types_aiobotocore_codeguru_reviewer/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9667 2023-07-08 01:27:34.000000 types-aiobotocore-codeguru-reviewer-2.5.2/types_aiobotocore_codeguru_reviewer/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9665 2023-07-08 01:27:34.000000 types-aiobotocore-codeguru-reviewer-2.5.2/types_aiobotocore_codeguru_reviewer/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2544 2023-07-08 01:27:34.000000 types-aiobotocore-codeguru-reviewer-2.5.2/types_aiobotocore_codeguru_reviewer/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2541 2023-07-08 01:27:34.000000 types-aiobotocore-codeguru-reviewer-2.5.2/types_aiobotocore_codeguru_reviewer/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:27:33.000000 types-aiobotocore-codeguru-reviewer-2.5.2/types_aiobotocore_codeguru_reviewer/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    21025 2023-07-08 01:27:35.000000 types-aiobotocore-codeguru-reviewer-2.5.2/types_aiobotocore_codeguru_reviewer/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21003 2023-07-08 01:27:35.000000 types-aiobotocore-codeguru-reviewer-2.5.2/types_aiobotocore_codeguru_reviewer/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:27:33.000000 types-aiobotocore-codeguru-reviewer-2.5.2/types_aiobotocore_codeguru_reviewer/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2858 2023-07-08 01:27:34.000000 types-aiobotocore-codeguru-reviewer-2.5.2/types_aiobotocore_codeguru_reviewer/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-07-08 01:27:34.000000 types-aiobotocore-codeguru-reviewer-2.5.2/types_aiobotocore_codeguru_reviewer/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:23.857869 types-aiobotocore-codeguru-reviewer-2.5.2/types_aiobotocore_codeguru_reviewer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16972 2023-07-08 01:43:23.000000 types-aiobotocore-codeguru-reviewer-2.5.2/types_aiobotocore_codeguru_reviewer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-07-08 01:43:23.000000 types-aiobotocore-codeguru-reviewer-2.5.2/types_aiobotocore_codeguru_reviewer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:23.000000 types-aiobotocore-codeguru-reviewer-2.5.2/types_aiobotocore_codeguru_reviewer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:23.000000 types-aiobotocore-codeguru-reviewer-2.5.2/types_aiobotocore_codeguru_reviewer.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:43:23.000000 types-aiobotocore-codeguru-reviewer-2.5.2/types_aiobotocore_codeguru_reviewer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-08 01:43:23.000000 types-aiobotocore-codeguru-reviewer-2.5.2/types_aiobotocore_codeguru_reviewer.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-codeguru-reviewer-2.5.1/LICENSE` & `types-aiobotocore-codeguru-reviewer-2.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codeguru-reviewer-2.5.1/PKG-INFO` & `types-aiobotocore-codeguru-reviewer-2.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-codeguru-reviewer
-Version: 2.5.1
-Summary: Type annotations for aiobotocore.CodeGuruReviewer 2.5.1 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2
+Summary: Type annotations for aiobotocore.CodeGuruReviewer 2.5.2 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeguru_reviewer/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-codeguru-reviewer.svg?color=blue)](https://pypi.org/project/types-aiobotocore-codeguru-reviewer)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeguru_reviewer/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-codeguru-reviewer?color=blue)](https://pypistats.org/packages/types-aiobotocore-codeguru-reviewer)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.CodeGuruReviewer 2.5.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-reviewer.html#CodeGuruReviewer)
+[aiobotocore.CodeGuruReviewer 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-reviewer.html#CodeGuruReviewer)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-codeguru-reviewer-2.5.1/README.md` & `types-aiobotocore-codeguru-reviewer-2.5.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-codeguru-reviewer.svg?color=blue)](https://pypi.org/project/types-aiobotocore-codeguru-reviewer)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeguru_reviewer/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-codeguru-reviewer?color=blue)](https://pypistats.org/packages/types-aiobotocore-codeguru-reviewer)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.CodeGuruReviewer 2.5.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-reviewer.html#CodeGuruReviewer)
+[aiobotocore.CodeGuruReviewer 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-reviewer.html#CodeGuruReviewer)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-codeguru-reviewer-2.5.1/setup.py` & `types-aiobotocore-codeguru-reviewer-2.5.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-codeguru-reviewer",
-    version="2.5.1",
+    version="2.5.2",
     packages=["types_aiobotocore_codeguru_reviewer"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.CodeGuruReviewer 2.5.1 service generated with"
+        "Type annotations for aiobotocore.CodeGuruReviewer 2.5.2 service generated with"
         " mypy-boto3-builder 7.14.5"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-codeguru-reviewer-2.5.1/types_aiobotocore_codeguru_reviewer/__init__.py` & `types-aiobotocore-codeguru-reviewer-2.5.2/types_aiobotocore_codeguru_reviewer/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codeguru-reviewer-2.5.1/types_aiobotocore_codeguru_reviewer/__init__.pyi` & `types-aiobotocore-codeguru-reviewer-2.5.2/types_aiobotocore_codeguru_reviewer/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codeguru-reviewer-2.5.1/types_aiobotocore_codeguru_reviewer/__main__.py` & `types-aiobotocore-codeguru-reviewer-2.5.2/types_aiobotocore_codeguru_reviewer/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.CodeGuruReviewer 2.5.1\nVersion:         2.5.1\nBuilder"
+        "Type annotations for aiobotocore.CodeGuruReviewer 2.5.2\nVersion:         2.5.2\nBuilder"
         " version: 7.14.5\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeguru_reviewer//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-reviewer.html#CodeGuruReviewer\nOther"
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

### Comparing `types-aiobotocore-codeguru-reviewer-2.5.1/types_aiobotocore_codeguru_reviewer/client.py` & `types-aiobotocore-codeguru-reviewer-2.5.2/types_aiobotocore_codeguru_reviewer/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codeguru-reviewer-2.5.1/types_aiobotocore_codeguru_reviewer/client.pyi` & `types-aiobotocore-codeguru-reviewer-2.5.2/types_aiobotocore_codeguru_reviewer/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codeguru-reviewer-2.5.1/types_aiobotocore_codeguru_reviewer/literals.py` & `types-aiobotocore-codeguru-reviewer-2.5.2/types_aiobotocore_codeguru_reviewer/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codeguru-reviewer-2.5.1/types_aiobotocore_codeguru_reviewer/literals.pyi` & `types-aiobotocore-codeguru-reviewer-2.5.2/types_aiobotocore_codeguru_reviewer/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codeguru-reviewer-2.5.1/types_aiobotocore_codeguru_reviewer/paginator.py` & `types-aiobotocore-codeguru-reviewer-2.5.2/types_aiobotocore_codeguru_reviewer/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codeguru-reviewer-2.5.1/types_aiobotocore_codeguru_reviewer/paginator.pyi` & `types-aiobotocore-codeguru-reviewer-2.5.2/types_aiobotocore_codeguru_reviewer/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codeguru-reviewer-2.5.1/types_aiobotocore_codeguru_reviewer/type_defs.py` & `types-aiobotocore-codeguru-reviewer-2.5.2/types_aiobotocore_codeguru_reviewer/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codeguru-reviewer-2.5.1/types_aiobotocore_codeguru_reviewer/type_defs.pyi` & `types-aiobotocore-codeguru-reviewer-2.5.2/types_aiobotocore_codeguru_reviewer/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codeguru-reviewer-2.5.1/types_aiobotocore_codeguru_reviewer/waiter.py` & `types-aiobotocore-codeguru-reviewer-2.5.2/types_aiobotocore_codeguru_reviewer/waiter.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codeguru-reviewer-2.5.1/types_aiobotocore_codeguru_reviewer/waiter.pyi` & `types-aiobotocore-codeguru-reviewer-2.5.2/types_aiobotocore_codeguru_reviewer/waiter.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codeguru-reviewer-2.5.1/types_aiobotocore_codeguru_reviewer.egg-info/PKG-INFO` & `types-aiobotocore-codeguru-reviewer-2.5.2/types_aiobotocore_codeguru_reviewer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-codeguru-reviewer
-Version: 2.5.1
-Summary: Type annotations for aiobotocore.CodeGuruReviewer 2.5.1 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2
+Summary: Type annotations for aiobotocore.CodeGuruReviewer 2.5.2 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeguru_reviewer/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-codeguru-reviewer.svg?color=blue)](https://pypi.org/project/types-aiobotocore-codeguru-reviewer)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeguru_reviewer/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-codeguru-reviewer?color=blue)](https://pypistats.org/packages/types-aiobotocore-codeguru-reviewer)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.CodeGuruReviewer 2.5.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-reviewer.html#CodeGuruReviewer)
+[aiobotocore.CodeGuruReviewer 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-reviewer.html#CodeGuruReviewer)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-codeguru-reviewer-2.5.1/types_aiobotocore_codeguru_reviewer.egg-info/SOURCES.txt` & `types-aiobotocore-codeguru-reviewer-2.5.2/types_aiobotocore_codeguru_reviewer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

