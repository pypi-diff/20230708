# Comparing `tmp/types-aiobotocore-cloudhsmv2-2.5.1.tar.gz` & `tmp/types-aiobotocore-cloudhsmv2-2.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-cloudhsmv2-2.5.1.tar", last modified: Wed Jun 28 01:43:13 2023, max compression
+gzip compressed data, was "types-aiobotocore-cloudhsmv2-2.5.2.tar", last modified: Sat Jul  8 01:43:21 2023, max compression
```

## Comparing `types-aiobotocore-cloudhsmv2-2.5.1.tar` & `types-aiobotocore-cloudhsmv2-2.5.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 01:43:13.502107 types-aiobotocore-cloudhsmv2-2.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-28 01:27:32.000000 types-aiobotocore-cloudhsmv2-2.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14825 2023-06-28 01:43:13.498107 types-aiobotocore-cloudhsmv2-2.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13248 2023-06-28 01:27:32.000000 types-aiobotocore-cloudhsmv2-2.5.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-28 01:43:13.502107 types-aiobotocore-cloudhsmv2-2.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-06-28 01:27:32.000000 types-aiobotocore-cloudhsmv2-2.5.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 01:43:13.490107 types-aiobotocore-cloudhsmv2-2.5.1/types_aiobotocore_cloudhsmv2/
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-06-28 01:27:32.000000 types-aiobotocore-cloudhsmv2-2.5.1/types_aiobotocore_cloudhsmv2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-06-28 01:27:32.000000 types-aiobotocore-cloudhsmv2-2.5.1/types_aiobotocore_cloudhsmv2/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-06-28 01:27:32.000000 types-aiobotocore-cloudhsmv2-2.5.1/types_aiobotocore_cloudhsmv2/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14707 2023-06-28 01:27:32.000000 types-aiobotocore-cloudhsmv2-2.5.1/types_aiobotocore_cloudhsmv2/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    14680 2023-06-28 01:27:32.000000 types-aiobotocore-cloudhsmv2-2.5.1/types_aiobotocore_cloudhsmv2/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9010 2023-06-28 01:27:32.000000 types-aiobotocore-cloudhsmv2-2.5.1/types_aiobotocore_cloudhsmv2/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9008 2023-06-28 01:27:32.000000 types-aiobotocore-cloudhsmv2-2.5.1/types_aiobotocore_cloudhsmv2/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4351 2023-06-28 01:27:32.000000 types-aiobotocore-cloudhsmv2-2.5.1/types_aiobotocore_cloudhsmv2/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4346 2023-06-28 01:27:32.000000 types-aiobotocore-cloudhsmv2-2.5.1/types_aiobotocore_cloudhsmv2/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 01:27:32.000000 types-aiobotocore-cloudhsmv2-2.5.1/types_aiobotocore_cloudhsmv2/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    13082 2023-06-28 01:27:32.000000 types-aiobotocore-cloudhsmv2-2.5.1/types_aiobotocore_cloudhsmv2/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    13065 2023-06-28 01:27:32.000000 types-aiobotocore-cloudhsmv2-2.5.1/types_aiobotocore_cloudhsmv2/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-28 01:27:32.000000 types-aiobotocore-cloudhsmv2-2.5.1/types_aiobotocore_cloudhsmv2/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 01:43:13.498107 types-aiobotocore-cloudhsmv2-2.5.1/types_aiobotocore_cloudhsmv2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14825 2023-06-28 01:43:13.000000 types-aiobotocore-cloudhsmv2-2.5.1/types_aiobotocore_cloudhsmv2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-06-28 01:43:13.000000 types-aiobotocore-cloudhsmv2-2.5.1/types_aiobotocore_cloudhsmv2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 01:43:13.000000 types-aiobotocore-cloudhsmv2-2.5.1/types_aiobotocore_cloudhsmv2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 01:43:13.000000 types-aiobotocore-cloudhsmv2-2.5.1/types_aiobotocore_cloudhsmv2.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-28 01:43:13.000000 types-aiobotocore-cloudhsmv2-2.5.1/types_aiobotocore_cloudhsmv2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-28 01:43:13.000000 types-aiobotocore-cloudhsmv2-2.5.1/types_aiobotocore_cloudhsmv2.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:21.569826 types-aiobotocore-cloudhsmv2-2.5.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:27:08.000000 types-aiobotocore-cloudhsmv2-2.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14825 2023-07-08 01:43:21.565826 types-aiobotocore-cloudhsmv2-2.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13248 2023-07-08 01:27:08.000000 types-aiobotocore-cloudhsmv2-2.5.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:43:21.569826 types-aiobotocore-cloudhsmv2-2.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-07-08 01:27:08.000000 types-aiobotocore-cloudhsmv2-2.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:21.557826 types-aiobotocore-cloudhsmv2-2.5.2/types_aiobotocore_cloudhsmv2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-07-08 01:27:08.000000 types-aiobotocore-cloudhsmv2-2.5.2/types_aiobotocore_cloudhsmv2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-07-08 01:27:08.000000 types-aiobotocore-cloudhsmv2-2.5.2/types_aiobotocore_cloudhsmv2/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-07-08 01:27:08.000000 types-aiobotocore-cloudhsmv2-2.5.2/types_aiobotocore_cloudhsmv2/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14707 2023-07-08 01:27:09.000000 types-aiobotocore-cloudhsmv2-2.5.2/types_aiobotocore_cloudhsmv2/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14680 2023-07-08 01:27:08.000000 types-aiobotocore-cloudhsmv2-2.5.2/types_aiobotocore_cloudhsmv2/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9010 2023-07-08 01:27:09.000000 types-aiobotocore-cloudhsmv2-2.5.2/types_aiobotocore_cloudhsmv2/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9008 2023-07-08 01:27:09.000000 types-aiobotocore-cloudhsmv2-2.5.2/types_aiobotocore_cloudhsmv2/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4351 2023-07-08 01:27:09.000000 types-aiobotocore-cloudhsmv2-2.5.2/types_aiobotocore_cloudhsmv2/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4346 2023-07-08 01:27:09.000000 types-aiobotocore-cloudhsmv2-2.5.2/types_aiobotocore_cloudhsmv2/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:27:08.000000 types-aiobotocore-cloudhsmv2-2.5.2/types_aiobotocore_cloudhsmv2/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    13082 2023-07-08 01:27:09.000000 types-aiobotocore-cloudhsmv2-2.5.2/types_aiobotocore_cloudhsmv2/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13065 2023-07-08 01:27:09.000000 types-aiobotocore-cloudhsmv2-2.5.2/types_aiobotocore_cloudhsmv2/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:27:08.000000 types-aiobotocore-cloudhsmv2-2.5.2/types_aiobotocore_cloudhsmv2/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:21.565826 types-aiobotocore-cloudhsmv2-2.5.2/types_aiobotocore_cloudhsmv2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14825 2023-07-08 01:43:21.000000 types-aiobotocore-cloudhsmv2-2.5.2/types_aiobotocore_cloudhsmv2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-07-08 01:43:21.000000 types-aiobotocore-cloudhsmv2-2.5.2/types_aiobotocore_cloudhsmv2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:21.000000 types-aiobotocore-cloudhsmv2-2.5.2/types_aiobotocore_cloudhsmv2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:21.000000 types-aiobotocore-cloudhsmv2-2.5.2/types_aiobotocore_cloudhsmv2.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:43:21.000000 types-aiobotocore-cloudhsmv2-2.5.2/types_aiobotocore_cloudhsmv2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-08 01:43:21.000000 types-aiobotocore-cloudhsmv2-2.5.2/types_aiobotocore_cloudhsmv2.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-cloudhsmv2-2.5.1/LICENSE` & `types-aiobotocore-cloudhsmv2-2.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudhsmv2-2.5.1/PKG-INFO` & `types-aiobotocore-cloudhsmv2-2.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-cloudhsmv2
-Version: 2.5.1
-Summary: Type annotations for aiobotocore.CloudHSMV2 2.5.1 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2
+Summary: Type annotations for aiobotocore.CloudHSMV2 2.5.2 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudhsmv2/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-cloudhsmv2.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cloudhsmv2)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudhsmv2/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-cloudhsmv2?color=blue)](https://pypistats.org/packages/types-aiobotocore-cloudhsmv2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.CloudHSMV2 2.5.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsmv2.html#CloudHSMV2)
+[aiobotocore.CloudHSMV2 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsmv2.html#CloudHSMV2)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-cloudhsmv2-2.5.1/README.md` & `types-aiobotocore-cloudhsmv2-2.5.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-cloudhsmv2.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cloudhsmv2)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudhsmv2/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-cloudhsmv2?color=blue)](https://pypistats.org/packages/types-aiobotocore-cloudhsmv2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.CloudHSMV2 2.5.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsmv2.html#CloudHSMV2)
+[aiobotocore.CloudHSMV2 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsmv2.html#CloudHSMV2)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-cloudhsmv2-2.5.1/setup.py` & `types-aiobotocore-cloudhsmv2-2.5.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-cloudhsmv2",
-    version="2.5.1",
+    version="2.5.2",
     packages=["types_aiobotocore_cloudhsmv2"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.CloudHSMV2 2.5.1 service generated with"
+        "Type annotations for aiobotocore.CloudHSMV2 2.5.2 service generated with"
         " mypy-boto3-builder 7.14.5"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-cloudhsmv2-2.5.1/types_aiobotocore_cloudhsmv2/__init__.py` & `types-aiobotocore-cloudhsmv2-2.5.2/types_aiobotocore_cloudhsmv2/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudhsmv2-2.5.1/types_aiobotocore_cloudhsmv2/__init__.pyi` & `types-aiobotocore-cloudhsmv2-2.5.2/types_aiobotocore_cloudhsmv2/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudhsmv2-2.5.1/types_aiobotocore_cloudhsmv2/__main__.py` & `types-aiobotocore-cloudhsmv2-2.5.2/types_aiobotocore_cloudhsmv2/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.CloudHSMV2 2.5.1\nVersion:         2.5.1\nBuilder"
+        "Type annotations for aiobotocore.CloudHSMV2 2.5.2\nVersion:         2.5.2\nBuilder"
         " version: 7.14.5\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudhsmv2//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsmv2.html#CloudHSMV2\nOther"
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

### Comparing `types-aiobotocore-cloudhsmv2-2.5.1/types_aiobotocore_cloudhsmv2/client.py` & `types-aiobotocore-cloudhsmv2-2.5.2/types_aiobotocore_cloudhsmv2/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudhsmv2-2.5.1/types_aiobotocore_cloudhsmv2/client.pyi` & `types-aiobotocore-cloudhsmv2-2.5.2/types_aiobotocore_cloudhsmv2/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudhsmv2-2.5.1/types_aiobotocore_cloudhsmv2/literals.py` & `types-aiobotocore-cloudhsmv2-2.5.2/types_aiobotocore_cloudhsmv2/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudhsmv2-2.5.1/types_aiobotocore_cloudhsmv2/literals.pyi` & `types-aiobotocore-cloudhsmv2-2.5.2/types_aiobotocore_cloudhsmv2/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudhsmv2-2.5.1/types_aiobotocore_cloudhsmv2/paginator.py` & `types-aiobotocore-cloudhsmv2-2.5.2/types_aiobotocore_cloudhsmv2/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudhsmv2-2.5.1/types_aiobotocore_cloudhsmv2/paginator.pyi` & `types-aiobotocore-cloudhsmv2-2.5.2/types_aiobotocore_cloudhsmv2/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudhsmv2-2.5.1/types_aiobotocore_cloudhsmv2/type_defs.py` & `types-aiobotocore-cloudhsmv2-2.5.2/types_aiobotocore_cloudhsmv2/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudhsmv2-2.5.1/types_aiobotocore_cloudhsmv2/type_defs.pyi` & `types-aiobotocore-cloudhsmv2-2.5.2/types_aiobotocore_cloudhsmv2/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudhsmv2-2.5.1/types_aiobotocore_cloudhsmv2.egg-info/PKG-INFO` & `types-aiobotocore-cloudhsmv2-2.5.2/types_aiobotocore_cloudhsmv2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-cloudhsmv2
-Version: 2.5.1
-Summary: Type annotations for aiobotocore.CloudHSMV2 2.5.1 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2
+Summary: Type annotations for aiobotocore.CloudHSMV2 2.5.2 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudhsmv2/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-cloudhsmv2.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cloudhsmv2)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudhsmv2/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-cloudhsmv2?color=blue)](https://pypistats.org/packages/types-aiobotocore-cloudhsmv2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.CloudHSMV2 2.5.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsmv2.html#CloudHSMV2)
+[aiobotocore.CloudHSMV2 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsmv2.html#CloudHSMV2)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-cloudhsmv2-2.5.1/types_aiobotocore_cloudhsmv2.egg-info/SOURCES.txt` & `types-aiobotocore-cloudhsmv2-2.5.2/types_aiobotocore_cloudhsmv2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

