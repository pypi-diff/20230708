# Comparing `tmp/types-aiobotocore-elastictranscoder-2.5.1.tar.gz` & `tmp/types-aiobotocore-elastictranscoder-2.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-elastictranscoder-2.5.1.tar", last modified: Wed Jun 28 01:43:27 2023, max compression
+gzip compressed data, was "types-aiobotocore-elastictranscoder-2.5.2.tar", last modified: Sat Jul  8 01:43:35 2023, max compression
```

## Comparing `types-aiobotocore-elastictranscoder-2.5.1.tar` & `types-aiobotocore-elastictranscoder-2.5.2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 01:43:27.258132 types-aiobotocore-elastictranscoder-2.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-28 01:30:46.000000 types-aiobotocore-elastictranscoder-2.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16920 2023-06-28 01:43:27.250132 types-aiobotocore-elastictranscoder-2.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15315 2023-06-28 01:30:46.000000 types-aiobotocore-elastictranscoder-2.5.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-28 01:43:27.258132 types-aiobotocore-elastictranscoder-2.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-06-28 01:30:46.000000 types-aiobotocore-elastictranscoder-2.5.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 01:43:27.250132 types-aiobotocore-elastictranscoder-2.5.1/types_aiobotocore_elastictranscoder/
--rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-06-28 01:30:46.000000 types-aiobotocore-elastictranscoder-2.5.1/types_aiobotocore_elastictranscoder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-06-28 01:30:46.000000 types-aiobotocore-elastictranscoder-2.5.1/types_aiobotocore_elastictranscoder/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-06-28 01:30:46.000000 types-aiobotocore-elastictranscoder-2.5.1/types_aiobotocore_elastictranscoder/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18560 2023-06-28 01:30:46.000000 types-aiobotocore-elastictranscoder-2.5.1/types_aiobotocore_elastictranscoder/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    18529 2023-06-28 01:30:46.000000 types-aiobotocore-elastictranscoder-2.5.1/types_aiobotocore_elastictranscoder/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8428 2023-06-28 01:30:46.000000 types-aiobotocore-elastictranscoder-2.5.1/types_aiobotocore_elastictranscoder/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8426 2023-06-28 01:30:46.000000 types-aiobotocore-elastictranscoder-2.5.1/types_aiobotocore_elastictranscoder/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5672 2023-06-28 01:30:46.000000 types-aiobotocore-elastictranscoder-2.5.1/types_aiobotocore_elastictranscoder/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5666 2023-06-28 01:30:46.000000 types-aiobotocore-elastictranscoder-2.5.1/types_aiobotocore_elastictranscoder/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 01:30:46.000000 types-aiobotocore-elastictranscoder-2.5.1/types_aiobotocore_elastictranscoder/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    22891 2023-06-28 01:30:47.000000 types-aiobotocore-elastictranscoder-2.5.1/types_aiobotocore_elastictranscoder/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    22872 2023-06-28 01:30:47.000000 types-aiobotocore-elastictranscoder-2.5.1/types_aiobotocore_elastictranscoder/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-28 01:30:46.000000 types-aiobotocore-elastictranscoder-2.5.1/types_aiobotocore_elastictranscoder/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-06-28 01:30:46.000000 types-aiobotocore-elastictranscoder-2.5.1/types_aiobotocore_elastictranscoder/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-06-28 01:30:46.000000 types-aiobotocore-elastictranscoder-2.5.1/types_aiobotocore_elastictranscoder/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 01:43:27.250132 types-aiobotocore-elastictranscoder-2.5.1/types_aiobotocore_elastictranscoder.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16920 2023-06-28 01:43:27.000000 types-aiobotocore-elastictranscoder-2.5.1/types_aiobotocore_elastictranscoder.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-06-28 01:43:27.000000 types-aiobotocore-elastictranscoder-2.5.1/types_aiobotocore_elastictranscoder.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 01:43:27.000000 types-aiobotocore-elastictranscoder-2.5.1/types_aiobotocore_elastictranscoder.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 01:43:27.000000 types-aiobotocore-elastictranscoder-2.5.1/types_aiobotocore_elastictranscoder.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-28 01:43:27.000000 types-aiobotocore-elastictranscoder-2.5.1/types_aiobotocore_elastictranscoder.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-28 01:43:27.000000 types-aiobotocore-elastictranscoder-2.5.1/types_aiobotocore_elastictranscoder.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:35.542092 types-aiobotocore-elastictranscoder-2.5.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:30:28.000000 types-aiobotocore-elastictranscoder-2.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16920 2023-07-08 01:43:35.534092 types-aiobotocore-elastictranscoder-2.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15315 2023-07-08 01:30:28.000000 types-aiobotocore-elastictranscoder-2.5.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:43:35.542092 types-aiobotocore-elastictranscoder-2.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-07-08 01:30:28.000000 types-aiobotocore-elastictranscoder-2.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:35.526092 types-aiobotocore-elastictranscoder-2.5.2/types_aiobotocore_elastictranscoder/
+-rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-07-08 01:30:28.000000 types-aiobotocore-elastictranscoder-2.5.2/types_aiobotocore_elastictranscoder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-07-08 01:30:28.000000 types-aiobotocore-elastictranscoder-2.5.2/types_aiobotocore_elastictranscoder/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-07-08 01:30:29.000000 types-aiobotocore-elastictranscoder-2.5.2/types_aiobotocore_elastictranscoder/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18560 2023-07-08 01:30:29.000000 types-aiobotocore-elastictranscoder-2.5.2/types_aiobotocore_elastictranscoder/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18529 2023-07-08 01:30:29.000000 types-aiobotocore-elastictranscoder-2.5.2/types_aiobotocore_elastictranscoder/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8428 2023-07-08 01:30:29.000000 types-aiobotocore-elastictranscoder-2.5.2/types_aiobotocore_elastictranscoder/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8426 2023-07-08 01:30:29.000000 types-aiobotocore-elastictranscoder-2.5.2/types_aiobotocore_elastictranscoder/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5672 2023-07-08 01:30:29.000000 types-aiobotocore-elastictranscoder-2.5.2/types_aiobotocore_elastictranscoder/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5666 2023-07-08 01:30:29.000000 types-aiobotocore-elastictranscoder-2.5.2/types_aiobotocore_elastictranscoder/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:30:29.000000 types-aiobotocore-elastictranscoder-2.5.2/types_aiobotocore_elastictranscoder/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    22891 2023-07-08 01:30:29.000000 types-aiobotocore-elastictranscoder-2.5.2/types_aiobotocore_elastictranscoder/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22872 2023-07-08 01:30:29.000000 types-aiobotocore-elastictranscoder-2.5.2/types_aiobotocore_elastictranscoder/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:30:28.000000 types-aiobotocore-elastictranscoder-2.5.2/types_aiobotocore_elastictranscoder/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-07-08 01:30:29.000000 types-aiobotocore-elastictranscoder-2.5.2/types_aiobotocore_elastictranscoder/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-07-08 01:30:29.000000 types-aiobotocore-elastictranscoder-2.5.2/types_aiobotocore_elastictranscoder/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:35.534092 types-aiobotocore-elastictranscoder-2.5.2/types_aiobotocore_elastictranscoder.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16920 2023-07-08 01:43:35.000000 types-aiobotocore-elastictranscoder-2.5.2/types_aiobotocore_elastictranscoder.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-07-08 01:43:35.000000 types-aiobotocore-elastictranscoder-2.5.2/types_aiobotocore_elastictranscoder.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:35.000000 types-aiobotocore-elastictranscoder-2.5.2/types_aiobotocore_elastictranscoder.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:35.000000 types-aiobotocore-elastictranscoder-2.5.2/types_aiobotocore_elastictranscoder.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:43:35.000000 types-aiobotocore-elastictranscoder-2.5.2/types_aiobotocore_elastictranscoder.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-08 01:43:35.000000 types-aiobotocore-elastictranscoder-2.5.2/types_aiobotocore_elastictranscoder.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-elastictranscoder-2.5.1/LICENSE` & `types-aiobotocore-elastictranscoder-2.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-elastictranscoder-2.5.1/PKG-INFO` & `types-aiobotocore-elastictranscoder-2.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-elastictranscoder
-Version: 2.5.1
-Summary: Type annotations for aiobotocore.ElasticTranscoder 2.5.1 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2
+Summary: Type annotations for aiobotocore.ElasticTranscoder 2.5.2 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elastictranscoder/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-elastictranscoder.svg?color=blue)](https://pypi.org/project/types-aiobotocore-elastictranscoder)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elastictranscoder/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-elastictranscoder?color=blue)](https://pypistats.org/packages/types-aiobotocore-elastictranscoder)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ElasticTranscoder 2.5.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastictranscoder.html#ElasticTranscoder)
+[aiobotocore.ElasticTranscoder 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastictranscoder.html#ElasticTranscoder)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-elastictranscoder-2.5.1/README.md` & `types-aiobotocore-elastictranscoder-2.5.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-elastictranscoder.svg?color=blue)](https://pypi.org/project/types-aiobotocore-elastictranscoder)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elastictranscoder/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-elastictranscoder?color=blue)](https://pypistats.org/packages/types-aiobotocore-elastictranscoder)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ElasticTranscoder 2.5.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastictranscoder.html#ElasticTranscoder)
+[aiobotocore.ElasticTranscoder 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastictranscoder.html#ElasticTranscoder)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-elastictranscoder-2.5.1/setup.py` & `types-aiobotocore-elastictranscoder-2.5.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-elastictranscoder",
-    version="2.5.1",
+    version="2.5.2",
     packages=["types_aiobotocore_elastictranscoder"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.ElasticTranscoder 2.5.1 service generated with"
+        "Type annotations for aiobotocore.ElasticTranscoder 2.5.2 service generated with"
         " mypy-boto3-builder 7.14.5"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-elastictranscoder-2.5.1/types_aiobotocore_elastictranscoder/__init__.py` & `types-aiobotocore-elastictranscoder-2.5.2/types_aiobotocore_elastictranscoder/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-elastictranscoder-2.5.1/types_aiobotocore_elastictranscoder/__init__.pyi` & `types-aiobotocore-elastictranscoder-2.5.2/types_aiobotocore_elastictranscoder/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-elastictranscoder-2.5.1/types_aiobotocore_elastictranscoder/__main__.py` & `types-aiobotocore-elastictranscoder-2.5.2/types_aiobotocore_elastictranscoder/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.ElasticTranscoder 2.5.1\nVersion:         2.5.1\nBuilder"
+        "Type annotations for aiobotocore.ElasticTranscoder 2.5.2\nVersion:         2.5.2\nBuilder"
         " version: 7.14.5\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elastictranscoder//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastictranscoder.html#ElasticTranscoder\nOther"
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

### Comparing `types-aiobotocore-elastictranscoder-2.5.1/types_aiobotocore_elastictranscoder/client.py` & `types-aiobotocore-elastictranscoder-2.5.2/types_aiobotocore_elastictranscoder/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-elastictranscoder-2.5.1/types_aiobotocore_elastictranscoder/client.pyi` & `types-aiobotocore-elastictranscoder-2.5.2/types_aiobotocore_elastictranscoder/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-elastictranscoder-2.5.1/types_aiobotocore_elastictranscoder/literals.py` & `types-aiobotocore-elastictranscoder-2.5.2/types_aiobotocore_elastictranscoder/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-elastictranscoder-2.5.1/types_aiobotocore_elastictranscoder/literals.pyi` & `types-aiobotocore-elastictranscoder-2.5.2/types_aiobotocore_elastictranscoder/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-elastictranscoder-2.5.1/types_aiobotocore_elastictranscoder/paginator.py` & `types-aiobotocore-elastictranscoder-2.5.2/types_aiobotocore_elastictranscoder/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-elastictranscoder-2.5.1/types_aiobotocore_elastictranscoder/paginator.pyi` & `types-aiobotocore-elastictranscoder-2.5.2/types_aiobotocore_elastictranscoder/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-elastictranscoder-2.5.1/types_aiobotocore_elastictranscoder/type_defs.py` & `types-aiobotocore-elastictranscoder-2.5.2/types_aiobotocore_elastictranscoder/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-elastictranscoder-2.5.1/types_aiobotocore_elastictranscoder/type_defs.pyi` & `types-aiobotocore-elastictranscoder-2.5.2/types_aiobotocore_elastictranscoder/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-elastictranscoder-2.5.1/types_aiobotocore_elastictranscoder/waiter.py` & `types-aiobotocore-elastictranscoder-2.5.2/types_aiobotocore_elastictranscoder/waiter.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-elastictranscoder-2.5.1/types_aiobotocore_elastictranscoder/waiter.pyi` & `types-aiobotocore-elastictranscoder-2.5.2/types_aiobotocore_elastictranscoder/waiter.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-elastictranscoder-2.5.1/types_aiobotocore_elastictranscoder.egg-info/PKG-INFO` & `types-aiobotocore-elastictranscoder-2.5.2/types_aiobotocore_elastictranscoder.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-elastictranscoder
-Version: 2.5.1
-Summary: Type annotations for aiobotocore.ElasticTranscoder 2.5.1 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2
+Summary: Type annotations for aiobotocore.ElasticTranscoder 2.5.2 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elastictranscoder/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-elastictranscoder.svg?color=blue)](https://pypi.org/project/types-aiobotocore-elastictranscoder)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elastictranscoder/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-elastictranscoder?color=blue)](https://pypistats.org/packages/types-aiobotocore-elastictranscoder)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ElasticTranscoder 2.5.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastictranscoder.html#ElasticTranscoder)
+[aiobotocore.ElasticTranscoder 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastictranscoder.html#ElasticTranscoder)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-elastictranscoder-2.5.1/types_aiobotocore_elastictranscoder.egg-info/SOURCES.txt` & `types-aiobotocore-elastictranscoder-2.5.2/types_aiobotocore_elastictranscoder.egg-info/SOURCES.txt`

 * *Files identical despite different names*

