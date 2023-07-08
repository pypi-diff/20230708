# Comparing `tmp/types-aiobotocore-drs-2.5.1.tar.gz` & `tmp/types-aiobotocore-drs-2.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-drs-2.5.1.tar", last modified: Wed Jun 28 01:43:24 2023, max compression
+gzip compressed data, was "types-aiobotocore-drs-2.5.2.tar", last modified: Sat Jul  8 01:43:32 2023, max compression
```

## Comparing `types-aiobotocore-drs-2.5.1.tar` & `types-aiobotocore-drs-2.5.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 01:43:24.654127 types-aiobotocore-drs-2.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-28 01:29:21.000000 types-aiobotocore-drs-2.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    22218 2023-06-28 01:43:24.654127 types-aiobotocore-drs-2.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    20669 2023-06-28 01:29:21.000000 types-aiobotocore-drs-2.5.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-28 01:43:24.654127 types-aiobotocore-drs-2.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-06-28 01:29:21.000000 types-aiobotocore-drs-2.5.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 01:43:24.650127 types-aiobotocore-drs-2.5.1/types_aiobotocore_drs/
--rw-r--r--   0 runner    (1001) docker     (123)     3017 2023-06-28 01:29:21.000000 types-aiobotocore-drs-2.5.1/types_aiobotocore_drs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3016 2023-06-28 01:29:21.000000 types-aiobotocore-drs-2.5.1/types_aiobotocore_drs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      904 2023-06-28 01:29:21.000000 types-aiobotocore-drs-2.5.1/types_aiobotocore_drs/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    42020 2023-06-28 01:29:22.000000 types-aiobotocore-drs-2.5.1/types_aiobotocore_drs/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    41954 2023-06-28 01:29:21.000000 types-aiobotocore-drs-2.5.1/types_aiobotocore_drs/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    17043 2023-06-28 01:29:22.000000 types-aiobotocore-drs-2.5.1/types_aiobotocore_drs/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    17041 2023-06-28 01:29:22.000000 types-aiobotocore-drs-2.5.1/types_aiobotocore_drs/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    13568 2023-06-28 01:29:22.000000 types-aiobotocore-drs-2.5.1/types_aiobotocore_drs/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    13556 2023-06-28 01:29:22.000000 types-aiobotocore-drs-2.5.1/types_aiobotocore_drs/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 01:29:21.000000 types-aiobotocore-drs-2.5.1/types_aiobotocore_drs/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    56978 2023-06-28 01:29:23.000000 types-aiobotocore-drs-2.5.1/types_aiobotocore_drs/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    56931 2023-06-28 01:29:22.000000 types-aiobotocore-drs-2.5.1/types_aiobotocore_drs/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-28 01:29:21.000000 types-aiobotocore-drs-2.5.1/types_aiobotocore_drs/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 01:43:24.654127 types-aiobotocore-drs-2.5.1/types_aiobotocore_drs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    22218 2023-06-28 01:43:24.000000 types-aiobotocore-drs-2.5.1/types_aiobotocore_drs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-06-28 01:43:24.000000 types-aiobotocore-drs-2.5.1/types_aiobotocore_drs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 01:43:24.000000 types-aiobotocore-drs-2.5.1/types_aiobotocore_drs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 01:43:24.000000 types-aiobotocore-drs-2.5.1/types_aiobotocore_drs.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-28 01:43:24.000000 types-aiobotocore-drs-2.5.1/types_aiobotocore_drs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-28 01:43:24.000000 types-aiobotocore-drs-2.5.1/types_aiobotocore_drs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:32.882042 types-aiobotocore-drs-2.5.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:29:00.000000 types-aiobotocore-drs-2.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    22218 2023-07-08 01:43:32.882042 types-aiobotocore-drs-2.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    20669 2023-07-08 01:29:00.000000 types-aiobotocore-drs-2.5.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:43:32.882042 types-aiobotocore-drs-2.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-07-08 01:29:00.000000 types-aiobotocore-drs-2.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:32.882042 types-aiobotocore-drs-2.5.2/types_aiobotocore_drs/
+-rw-r--r--   0 runner    (1001) docker     (123)     3017 2023-07-08 01:29:00.000000 types-aiobotocore-drs-2.5.2/types_aiobotocore_drs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3016 2023-07-08 01:29:00.000000 types-aiobotocore-drs-2.5.2/types_aiobotocore_drs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-07-08 01:29:00.000000 types-aiobotocore-drs-2.5.2/types_aiobotocore_drs/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42020 2023-07-08 01:29:01.000000 types-aiobotocore-drs-2.5.2/types_aiobotocore_drs/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41954 2023-07-08 01:29:01.000000 types-aiobotocore-drs-2.5.2/types_aiobotocore_drs/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    17043 2023-07-08 01:29:01.000000 types-aiobotocore-drs-2.5.2/types_aiobotocore_drs/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17041 2023-07-08 01:29:01.000000 types-aiobotocore-drs-2.5.2/types_aiobotocore_drs/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    13568 2023-07-08 01:29:01.000000 types-aiobotocore-drs-2.5.2/types_aiobotocore_drs/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13556 2023-07-08 01:29:01.000000 types-aiobotocore-drs-2.5.2/types_aiobotocore_drs/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:29:00.000000 types-aiobotocore-drs-2.5.2/types_aiobotocore_drs/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    56978 2023-07-08 01:29:02.000000 types-aiobotocore-drs-2.5.2/types_aiobotocore_drs/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56931 2023-07-08 01:29:02.000000 types-aiobotocore-drs-2.5.2/types_aiobotocore_drs/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:29:00.000000 types-aiobotocore-drs-2.5.2/types_aiobotocore_drs/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:32.882042 types-aiobotocore-drs-2.5.2/types_aiobotocore_drs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    22218 2023-07-08 01:43:32.000000 types-aiobotocore-drs-2.5.2/types_aiobotocore_drs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-08 01:43:32.000000 types-aiobotocore-drs-2.5.2/types_aiobotocore_drs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:32.000000 types-aiobotocore-drs-2.5.2/types_aiobotocore_drs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:32.000000 types-aiobotocore-drs-2.5.2/types_aiobotocore_drs.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:43:32.000000 types-aiobotocore-drs-2.5.2/types_aiobotocore_drs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-08 01:43:32.000000 types-aiobotocore-drs-2.5.2/types_aiobotocore_drs.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-drs-2.5.1/LICENSE` & `types-aiobotocore-drs-2.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-drs-2.5.1/PKG-INFO` & `types-aiobotocore-drs-2.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-drs
-Version: 2.5.1
-Summary: Type annotations for aiobotocore.drs 2.5.1 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2
+Summary: Type annotations for aiobotocore.drs 2.5.2 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_drs/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-drs.svg?color=blue)](https://pypi.org/project/types-aiobotocore-drs)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_drs/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-drs?color=blue)](https://pypistats.org/packages/types-aiobotocore-drs)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.drs 2.5.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs)
+[aiobotocore.drs 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-drs-2.5.1/README.md` & `types-aiobotocore-drs-2.5.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-drs.svg?color=blue)](https://pypi.org/project/types-aiobotocore-drs)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_drs/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-drs?color=blue)](https://pypistats.org/packages/types-aiobotocore-drs)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.drs 2.5.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs)
+[aiobotocore.drs 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-drs-2.5.1/setup.py` & `types-aiobotocore-drs-2.5.2/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-drs",
-    version="2.5.1",
+    version="2.5.2",
     packages=["types_aiobotocore_drs"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.drs 2.5.1 service generated with mypy-boto3-builder"
+        "Type annotations for aiobotocore.drs 2.5.2 service generated with mypy-boto3-builder"
         " 7.14.5"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-drs-2.5.1/types_aiobotocore_drs/__init__.py` & `types-aiobotocore-drs-2.5.2/types_aiobotocore_drs/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-drs-2.5.1/types_aiobotocore_drs/__init__.pyi` & `types-aiobotocore-drs-2.5.2/types_aiobotocore_drs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-drs-2.5.1/types_aiobotocore_drs/__main__.py` & `types-aiobotocore-drs-2.5.2/types_aiobotocore_drs/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.drs 2.5.1\nVersion:         2.5.1\nBuilder version:"
+        "Type annotations for aiobotocore.drs 2.5.2\nVersion:         2.5.2\nBuilder version:"
         " 7.14.5\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_drs//\nBoto3 docs:    "
         "  https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs\nOther"
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

### Comparing `types-aiobotocore-drs-2.5.1/types_aiobotocore_drs/client.py` & `types-aiobotocore-drs-2.5.2/types_aiobotocore_drs/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-drs-2.5.1/types_aiobotocore_drs/client.pyi` & `types-aiobotocore-drs-2.5.2/types_aiobotocore_drs/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-drs-2.5.1/types_aiobotocore_drs/literals.py` & `types-aiobotocore-drs-2.5.2/types_aiobotocore_drs/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-drs-2.5.1/types_aiobotocore_drs/literals.pyi` & `types-aiobotocore-drs-2.5.2/types_aiobotocore_drs/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-drs-2.5.1/types_aiobotocore_drs/paginator.py` & `types-aiobotocore-drs-2.5.2/types_aiobotocore_drs/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-drs-2.5.1/types_aiobotocore_drs/paginator.pyi` & `types-aiobotocore-drs-2.5.2/types_aiobotocore_drs/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-drs-2.5.1/types_aiobotocore_drs/type_defs.py` & `types-aiobotocore-drs-2.5.2/types_aiobotocore_drs/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-drs-2.5.1/types_aiobotocore_drs/type_defs.pyi` & `types-aiobotocore-drs-2.5.2/types_aiobotocore_drs/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-drs-2.5.1/types_aiobotocore_drs.egg-info/PKG-INFO` & `types-aiobotocore-drs-2.5.2/types_aiobotocore_drs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-drs
-Version: 2.5.1
-Summary: Type annotations for aiobotocore.drs 2.5.1 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2
+Summary: Type annotations for aiobotocore.drs 2.5.2 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_drs/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-drs.svg?color=blue)](https://pypi.org/project/types-aiobotocore-drs)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_drs/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-drs?color=blue)](https://pypistats.org/packages/types-aiobotocore-drs)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.drs 2.5.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs)
+[aiobotocore.drs 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-drs-2.5.1/types_aiobotocore_drs.egg-info/SOURCES.txt` & `types-aiobotocore-drs-2.5.2/types_aiobotocore_drs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

