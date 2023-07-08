# Comparing `tmp/types-aiobotocore-ds-2.5.1.tar.gz` & `tmp/types-aiobotocore-ds-2.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-ds-2.5.1.tar", last modified: Wed Jun 28 01:43:24 2023, max compression
+gzip compressed data, was "types-aiobotocore-ds-2.5.2.tar", last modified: Sat Jul  8 01:43:32 2023, max compression
```

## Comparing `types-aiobotocore-ds-2.5.1.tar` & `types-aiobotocore-ds-2.5.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 01:43:24.678127 types-aiobotocore-ds-2.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-28 01:29:23.000000 types-aiobotocore-ds-2.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    22522 2023-06-28 01:43:24.678127 types-aiobotocore-ds-2.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    20963 2023-06-28 01:29:23.000000 types-aiobotocore-ds-2.5.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-28 01:43:24.678127 types-aiobotocore-ds-2.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-06-28 01:29:23.000000 types-aiobotocore-ds-2.5.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 01:43:24.674127 types-aiobotocore-ds-2.5.1/types_aiobotocore_ds/
--rw-r--r--   0 runner    (1001) docker     (123)     3709 2023-06-28 01:29:23.000000 types-aiobotocore-ds-2.5.1/types_aiobotocore_ds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3708 2023-06-28 01:29:23.000000 types-aiobotocore-ds-2.5.1/types_aiobotocore_ds/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-06-28 01:29:23.000000 types-aiobotocore-ds-2.5.1/types_aiobotocore_ds/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    54551 2023-06-28 01:29:25.000000 types-aiobotocore-ds-2.5.1/types_aiobotocore_ds/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    54461 2023-06-28 01:29:24.000000 types-aiobotocore-ds-2.5.1/types_aiobotocore_ds/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    13611 2023-06-28 01:29:25.000000 types-aiobotocore-ds-2.5.1/types_aiobotocore_ds/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    13609 2023-06-28 01:29:25.000000 types-aiobotocore-ds-2.5.1/types_aiobotocore_ds/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    17776 2023-06-28 01:29:25.000000 types-aiobotocore-ds-2.5.1/types_aiobotocore_ds/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    17759 2023-06-28 01:29:25.000000 types-aiobotocore-ds-2.5.1/types_aiobotocore_ds/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 01:29:23.000000 types-aiobotocore-ds-2.5.1/types_aiobotocore_ds/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    57753 2023-06-28 01:29:26.000000 types-aiobotocore-ds-2.5.1/types_aiobotocore_ds/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    57680 2023-06-28 01:29:26.000000 types-aiobotocore-ds-2.5.1/types_aiobotocore_ds/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-28 01:29:23.000000 types-aiobotocore-ds-2.5.1/types_aiobotocore_ds/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 01:43:24.678127 types-aiobotocore-ds-2.5.1/types_aiobotocore_ds.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    22522 2023-06-28 01:43:24.000000 types-aiobotocore-ds-2.5.1/types_aiobotocore_ds.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-06-28 01:43:24.000000 types-aiobotocore-ds-2.5.1/types_aiobotocore_ds.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 01:43:24.000000 types-aiobotocore-ds-2.5.1/types_aiobotocore_ds.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 01:43:24.000000 types-aiobotocore-ds-2.5.1/types_aiobotocore_ds.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-28 01:43:24.000000 types-aiobotocore-ds-2.5.1/types_aiobotocore_ds.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-28 01:43:24.000000 types-aiobotocore-ds-2.5.1/types_aiobotocore_ds.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:32.898042 types-aiobotocore-ds-2.5.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:29:03.000000 types-aiobotocore-ds-2.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    22522 2023-07-08 01:43:32.894042 types-aiobotocore-ds-2.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    20963 2023-07-08 01:29:03.000000 types-aiobotocore-ds-2.5.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:43:32.898042 types-aiobotocore-ds-2.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-07-08 01:29:03.000000 types-aiobotocore-ds-2.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:32.894042 types-aiobotocore-ds-2.5.2/types_aiobotocore_ds/
+-rw-r--r--   0 runner    (1001) docker     (123)     3709 2023-07-08 01:29:03.000000 types-aiobotocore-ds-2.5.2/types_aiobotocore_ds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3708 2023-07-08 01:29:03.000000 types-aiobotocore-ds-2.5.2/types_aiobotocore_ds/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-07-08 01:29:03.000000 types-aiobotocore-ds-2.5.2/types_aiobotocore_ds/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54551 2023-07-08 01:29:04.000000 types-aiobotocore-ds-2.5.2/types_aiobotocore_ds/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54461 2023-07-08 01:29:03.000000 types-aiobotocore-ds-2.5.2/types_aiobotocore_ds/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    13611 2023-07-08 01:29:04.000000 types-aiobotocore-ds-2.5.2/types_aiobotocore_ds/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13609 2023-07-08 01:29:04.000000 types-aiobotocore-ds-2.5.2/types_aiobotocore_ds/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    17776 2023-07-08 01:29:04.000000 types-aiobotocore-ds-2.5.2/types_aiobotocore_ds/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17759 2023-07-08 01:29:04.000000 types-aiobotocore-ds-2.5.2/types_aiobotocore_ds/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:29:03.000000 types-aiobotocore-ds-2.5.2/types_aiobotocore_ds/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    57753 2023-07-08 01:29:05.000000 types-aiobotocore-ds-2.5.2/types_aiobotocore_ds/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57680 2023-07-08 01:29:05.000000 types-aiobotocore-ds-2.5.2/types_aiobotocore_ds/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:29:03.000000 types-aiobotocore-ds-2.5.2/types_aiobotocore_ds/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:32.894042 types-aiobotocore-ds-2.5.2/types_aiobotocore_ds.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    22522 2023-07-08 01:43:32.000000 types-aiobotocore-ds-2.5.2/types_aiobotocore_ds.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-08 01:43:32.000000 types-aiobotocore-ds-2.5.2/types_aiobotocore_ds.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:32.000000 types-aiobotocore-ds-2.5.2/types_aiobotocore_ds.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:32.000000 types-aiobotocore-ds-2.5.2/types_aiobotocore_ds.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:43:32.000000 types-aiobotocore-ds-2.5.2/types_aiobotocore_ds.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-08 01:43:32.000000 types-aiobotocore-ds-2.5.2/types_aiobotocore_ds.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-ds-2.5.1/LICENSE` & `types-aiobotocore-ds-2.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ds-2.5.1/PKG-INFO` & `types-aiobotocore-ds-2.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-ds
-Version: 2.5.1
-Summary: Type annotations for aiobotocore.DirectoryService 2.5.1 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2
+Summary: Type annotations for aiobotocore.DirectoryService 2.5.2 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ds/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-ds.svg?color=blue)](https://pypi.org/project/types-aiobotocore-ds)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ds/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-ds?color=blue)](https://pypistats.org/packages/types-aiobotocore-ds)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.DirectoryService 2.5.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService)
+[aiobotocore.DirectoryService 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-ds-2.5.1/README.md` & `types-aiobotocore-ds-2.5.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-ds.svg?color=blue)](https://pypi.org/project/types-aiobotocore-ds)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ds/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-ds?color=blue)](https://pypistats.org/packages/types-aiobotocore-ds)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.DirectoryService 2.5.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService)
+[aiobotocore.DirectoryService 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-ds-2.5.1/setup.py` & `types-aiobotocore-ds-2.5.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-ds",
-    version="2.5.1",
+    version="2.5.2",
     packages=["types_aiobotocore_ds"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.DirectoryService 2.5.1 service generated with"
+        "Type annotations for aiobotocore.DirectoryService 2.5.2 service generated with"
         " mypy-boto3-builder 7.14.5"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-ds-2.5.1/types_aiobotocore_ds/__init__.py` & `types-aiobotocore-ds-2.5.2/types_aiobotocore_ds/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ds-2.5.1/types_aiobotocore_ds/__init__.pyi` & `types-aiobotocore-ds-2.5.2/types_aiobotocore_ds/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ds-2.5.1/types_aiobotocore_ds/__main__.py` & `types-aiobotocore-ds-2.5.2/types_aiobotocore_ds/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.DirectoryService 2.5.1\nVersion:         2.5.1\nBuilder"
+        "Type annotations for aiobotocore.DirectoryService 2.5.2\nVersion:         2.5.2\nBuilder"
         " version: 7.14.5\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ds//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService\nOther"
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

### Comparing `types-aiobotocore-ds-2.5.1/types_aiobotocore_ds/client.py` & `types-aiobotocore-ds-2.5.2/types_aiobotocore_ds/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ds-2.5.1/types_aiobotocore_ds/client.pyi` & `types-aiobotocore-ds-2.5.2/types_aiobotocore_ds/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ds-2.5.1/types_aiobotocore_ds/literals.py` & `types-aiobotocore-ds-2.5.2/types_aiobotocore_ds/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ds-2.5.1/types_aiobotocore_ds/literals.pyi` & `types-aiobotocore-ds-2.5.2/types_aiobotocore_ds/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ds-2.5.1/types_aiobotocore_ds/paginator.py` & `types-aiobotocore-ds-2.5.2/types_aiobotocore_ds/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ds-2.5.1/types_aiobotocore_ds/paginator.pyi` & `types-aiobotocore-ds-2.5.2/types_aiobotocore_ds/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ds-2.5.1/types_aiobotocore_ds/type_defs.py` & `types-aiobotocore-ds-2.5.2/types_aiobotocore_ds/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ds-2.5.1/types_aiobotocore_ds/type_defs.pyi` & `types-aiobotocore-ds-2.5.2/types_aiobotocore_ds/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ds-2.5.1/types_aiobotocore_ds.egg-info/PKG-INFO` & `types-aiobotocore-ds-2.5.2/types_aiobotocore_ds.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-ds
-Version: 2.5.1
-Summary: Type annotations for aiobotocore.DirectoryService 2.5.1 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2
+Summary: Type annotations for aiobotocore.DirectoryService 2.5.2 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ds/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-ds.svg?color=blue)](https://pypi.org/project/types-aiobotocore-ds)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ds/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-ds?color=blue)](https://pypistats.org/packages/types-aiobotocore-ds)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.DirectoryService 2.5.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService)
+[aiobotocore.DirectoryService 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-ds-2.5.1/types_aiobotocore_ds.egg-info/SOURCES.txt` & `types-aiobotocore-ds-2.5.2/types_aiobotocore_ds.egg-info/SOURCES.txt`

 * *Files identical despite different names*

