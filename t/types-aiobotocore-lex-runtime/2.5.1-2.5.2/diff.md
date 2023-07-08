# Comparing `tmp/types-aiobotocore-lex-runtime-2.5.1.tar.gz` & `tmp/types-aiobotocore-lex-runtime-2.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-lex-runtime-2.5.1.tar", last modified: Wed Jun 28 01:43:45 2023, max compression
+gzip compressed data, was "types-aiobotocore-lex-runtime-2.5.2.tar", last modified: Sat Jul  8 01:43:53 2023, max compression
```

## Comparing `types-aiobotocore-lex-runtime-2.5.1.tar` & `types-aiobotocore-lex-runtime-2.5.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 01:43:45.002166 types-aiobotocore-lex-runtime-2.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-28 01:33:57.000000 types-aiobotocore-lex-runtime-2.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13071 2023-06-28 01:43:45.002166 types-aiobotocore-lex-runtime-2.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11484 2023-06-28 01:33:57.000000 types-aiobotocore-lex-runtime-2.5.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-28 01:43:45.002166 types-aiobotocore-lex-runtime-2.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-06-28 01:33:57.000000 types-aiobotocore-lex-runtime-2.5.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 01:43:44.998166 types-aiobotocore-lex-runtime-2.5.1/types_aiobotocore_lex_runtime/
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-06-28 01:33:57.000000 types-aiobotocore-lex-runtime-2.5.1/types_aiobotocore_lex_runtime/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-06-28 01:33:57.000000 types-aiobotocore-lex-runtime-2.5.1/types_aiobotocore_lex_runtime/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-06-28 01:33:57.000000 types-aiobotocore-lex-runtime-2.5.1/types_aiobotocore_lex_runtime/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8336 2023-06-28 01:33:57.000000 types-aiobotocore-lex-runtime-2.5.1/types_aiobotocore_lex_runtime/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     8323 2023-06-28 01:33:57.000000 types-aiobotocore-lex-runtime-2.5.1/types_aiobotocore_lex_runtime/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8439 2023-06-28 01:33:58.000000 types-aiobotocore-lex-runtime-2.5.1/types_aiobotocore_lex_runtime/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8437 2023-06-28 01:33:57.000000 types-aiobotocore-lex-runtime-2.5.1/types_aiobotocore_lex_runtime/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 01:33:57.000000 types-aiobotocore-lex-runtime-2.5.1/types_aiobotocore_lex_runtime/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     9696 2023-06-28 01:33:59.000000 types-aiobotocore-lex-runtime-2.5.1/types_aiobotocore_lex_runtime/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     9683 2023-06-28 01:33:58.000000 types-aiobotocore-lex-runtime-2.5.1/types_aiobotocore_lex_runtime/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-28 01:33:57.000000 types-aiobotocore-lex-runtime-2.5.1/types_aiobotocore_lex_runtime/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 01:43:45.002166 types-aiobotocore-lex-runtime-2.5.1/types_aiobotocore_lex_runtime.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13071 2023-06-28 01:43:44.000000 types-aiobotocore-lex-runtime-2.5.1/types_aiobotocore_lex_runtime.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-06-28 01:43:44.000000 types-aiobotocore-lex-runtime-2.5.1/types_aiobotocore_lex_runtime.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 01:43:44.000000 types-aiobotocore-lex-runtime-2.5.1/types_aiobotocore_lex_runtime.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 01:43:44.000000 types-aiobotocore-lex-runtime-2.5.1/types_aiobotocore_lex_runtime.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-28 01:43:44.000000 types-aiobotocore-lex-runtime-2.5.1/types_aiobotocore_lex_runtime.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-28 01:43:44.000000 types-aiobotocore-lex-runtime-2.5.1/types_aiobotocore_lex_runtime.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:53.354428 types-aiobotocore-lex-runtime-2.5.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:33:45.000000 types-aiobotocore-lex-runtime-2.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13071 2023-07-08 01:43:53.354428 types-aiobotocore-lex-runtime-2.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11484 2023-07-08 01:33:45.000000 types-aiobotocore-lex-runtime-2.5.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:43:53.354428 types-aiobotocore-lex-runtime-2.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-07-08 01:33:45.000000 types-aiobotocore-lex-runtime-2.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:53.354428 types-aiobotocore-lex-runtime-2.5.2/types_aiobotocore_lex_runtime/
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-07-08 01:33:45.000000 types-aiobotocore-lex-runtime-2.5.2/types_aiobotocore_lex_runtime/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-07-08 01:33:45.000000 types-aiobotocore-lex-runtime-2.5.2/types_aiobotocore_lex_runtime/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-07-08 01:33:45.000000 types-aiobotocore-lex-runtime-2.5.2/types_aiobotocore_lex_runtime/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8336 2023-07-08 01:33:45.000000 types-aiobotocore-lex-runtime-2.5.2/types_aiobotocore_lex_runtime/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8323 2023-07-08 01:33:45.000000 types-aiobotocore-lex-runtime-2.5.2/types_aiobotocore_lex_runtime/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8439 2023-07-08 01:33:46.000000 types-aiobotocore-lex-runtime-2.5.2/types_aiobotocore_lex_runtime/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8437 2023-07-08 01:33:46.000000 types-aiobotocore-lex-runtime-2.5.2/types_aiobotocore_lex_runtime/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:33:45.000000 types-aiobotocore-lex-runtime-2.5.2/types_aiobotocore_lex_runtime/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     9696 2023-07-08 01:33:46.000000 types-aiobotocore-lex-runtime-2.5.2/types_aiobotocore_lex_runtime/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9683 2023-07-08 01:33:46.000000 types-aiobotocore-lex-runtime-2.5.2/types_aiobotocore_lex_runtime/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:33:45.000000 types-aiobotocore-lex-runtime-2.5.2/types_aiobotocore_lex_runtime/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:53.354428 types-aiobotocore-lex-runtime-2.5.2/types_aiobotocore_lex_runtime.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13071 2023-07-08 01:43:53.000000 types-aiobotocore-lex-runtime-2.5.2/types_aiobotocore_lex_runtime.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-07-08 01:43:53.000000 types-aiobotocore-lex-runtime-2.5.2/types_aiobotocore_lex_runtime.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:53.000000 types-aiobotocore-lex-runtime-2.5.2/types_aiobotocore_lex_runtime.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:53.000000 types-aiobotocore-lex-runtime-2.5.2/types_aiobotocore_lex_runtime.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:43:53.000000 types-aiobotocore-lex-runtime-2.5.2/types_aiobotocore_lex_runtime.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-08 01:43:53.000000 types-aiobotocore-lex-runtime-2.5.2/types_aiobotocore_lex_runtime.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-lex-runtime-2.5.1/LICENSE` & `types-aiobotocore-lex-runtime-2.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-lex-runtime-2.5.1/PKG-INFO` & `types-aiobotocore-lex-runtime-2.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-lex-runtime
-Version: 2.5.1
-Summary: Type annotations for aiobotocore.LexRuntimeService 2.5.1 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2
+Summary: Type annotations for aiobotocore.LexRuntimeService 2.5.2 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lex_runtime/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-lex-runtime.svg?color=blue)](https://pypi.org/project/types-aiobotocore-lex-runtime)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lex_runtime/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-lex-runtime?color=blue)](https://pypistats.org/packages/types-aiobotocore-lex-runtime)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.LexRuntimeService 2.5.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-runtime.html#LexRuntimeService)
+[aiobotocore.LexRuntimeService 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-runtime.html#LexRuntimeService)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-lex-runtime-2.5.1/README.md` & `types-aiobotocore-lex-runtime-2.5.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-lex-runtime.svg?color=blue)](https://pypi.org/project/types-aiobotocore-lex-runtime)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lex_runtime/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-lex-runtime?color=blue)](https://pypistats.org/packages/types-aiobotocore-lex-runtime)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.LexRuntimeService 2.5.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-runtime.html#LexRuntimeService)
+[aiobotocore.LexRuntimeService 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-runtime.html#LexRuntimeService)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-lex-runtime-2.5.1/setup.py` & `types-aiobotocore-lex-runtime-2.5.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-lex-runtime",
-    version="2.5.1",
+    version="2.5.2",
     packages=["types_aiobotocore_lex_runtime"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.LexRuntimeService 2.5.1 service generated with"
+        "Type annotations for aiobotocore.LexRuntimeService 2.5.2 service generated with"
         " mypy-boto3-builder 7.14.5"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-lex-runtime-2.5.1/types_aiobotocore_lex_runtime/__main__.py` & `types-aiobotocore-lex-runtime-2.5.2/types_aiobotocore_lex_runtime/__main__.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.LexRuntimeService 2.5.1\nVersion:         2.5.1\nBuilder"
+        "Type annotations for aiobotocore.LexRuntimeService 2.5.2\nVersion:         2.5.2\nBuilder"
         " version: 7.14.5\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lex_runtime//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-runtime.html#LexRuntimeService\nOther"
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

### Comparing `types-aiobotocore-lex-runtime-2.5.1/types_aiobotocore_lex_runtime/client.py` & `types-aiobotocore-lex-runtime-2.5.2/types_aiobotocore_lex_runtime/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-lex-runtime-2.5.1/types_aiobotocore_lex_runtime/client.pyi` & `types-aiobotocore-lex-runtime-2.5.2/types_aiobotocore_lex_runtime/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-lex-runtime-2.5.1/types_aiobotocore_lex_runtime/literals.py` & `types-aiobotocore-lex-runtime-2.5.2/types_aiobotocore_lex_runtime/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-lex-runtime-2.5.1/types_aiobotocore_lex_runtime/literals.pyi` & `types-aiobotocore-lex-runtime-2.5.2/types_aiobotocore_lex_runtime/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-lex-runtime-2.5.1/types_aiobotocore_lex_runtime/type_defs.py` & `types-aiobotocore-lex-runtime-2.5.2/types_aiobotocore_lex_runtime/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-lex-runtime-2.5.1/types_aiobotocore_lex_runtime/type_defs.pyi` & `types-aiobotocore-lex-runtime-2.5.2/types_aiobotocore_lex_runtime/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-lex-runtime-2.5.1/types_aiobotocore_lex_runtime.egg-info/PKG-INFO` & `types-aiobotocore-lex-runtime-2.5.2/types_aiobotocore_lex_runtime.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-lex-runtime
-Version: 2.5.1
-Summary: Type annotations for aiobotocore.LexRuntimeService 2.5.1 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2
+Summary: Type annotations for aiobotocore.LexRuntimeService 2.5.2 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lex_runtime/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-lex-runtime.svg?color=blue)](https://pypi.org/project/types-aiobotocore-lex-runtime)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lex_runtime/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-lex-runtime?color=blue)](https://pypistats.org/packages/types-aiobotocore-lex-runtime)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.LexRuntimeService 2.5.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-runtime.html#LexRuntimeService)
+[aiobotocore.LexRuntimeService 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-runtime.html#LexRuntimeService)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-lex-runtime-2.5.1/types_aiobotocore_lex_runtime.egg-info/SOURCES.txt` & `types-aiobotocore-lex-runtime-2.5.2/types_aiobotocore_lex_runtime.egg-info/SOURCES.txt`

 * *Files identical despite different names*

