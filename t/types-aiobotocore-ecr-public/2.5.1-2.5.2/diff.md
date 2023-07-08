# Comparing `tmp/types-aiobotocore-ecr-public-2.5.1.tar.gz` & `tmp/types-aiobotocore-ecr-public-2.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-ecr-public-2.5.1.tar", last modified: Wed Jun 28 01:43:26 2023, max compression
+gzip compressed data, was "types-aiobotocore-ecr-public-2.5.2.tar", last modified: Sat Jul  8 01:43:34 2023, max compression
```

## Comparing `types-aiobotocore-ecr-public-2.5.1.tar` & `types-aiobotocore-ecr-public-2.5.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 01:43:26.386131 types-aiobotocore-ecr-public-2.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-28 01:30:24.000000 types-aiobotocore-ecr-public-2.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16163 2023-06-28 01:43:26.386131 types-aiobotocore-ecr-public-2.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14587 2023-06-28 01:30:24.000000 types-aiobotocore-ecr-public-2.5.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-28 01:43:26.386131 types-aiobotocore-ecr-public-2.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-06-28 01:30:24.000000 types-aiobotocore-ecr-public-2.5.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 01:43:26.374131 types-aiobotocore-ecr-public-2.5.1/types_aiobotocore_ecr_public/
--rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-06-28 01:30:24.000000 types-aiobotocore-ecr-public-2.5.1/types_aiobotocore_ecr_public/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-06-28 01:30:24.000000 types-aiobotocore-ecr-public-2.5.1/types_aiobotocore_ecr_public/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-06-28 01:30:24.000000 types-aiobotocore-ecr-public-2.5.1/types_aiobotocore_ecr_public/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22197 2023-06-28 01:30:24.000000 types-aiobotocore-ecr-public-2.5.1/types_aiobotocore_ecr_public/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    22161 2023-06-28 01:30:24.000000 types-aiobotocore-ecr-public-2.5.1/types_aiobotocore_ecr_public/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8722 2023-06-28 01:30:24.000000 types-aiobotocore-ecr-public-2.5.1/types_aiobotocore_ecr_public/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8720 2023-06-28 01:30:24.000000 types-aiobotocore-ecr-public-2.5.1/types_aiobotocore_ecr_public/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5762 2023-06-28 01:30:24.000000 types-aiobotocore-ecr-public-2.5.1/types_aiobotocore_ecr_public/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5756 2023-06-28 01:30:24.000000 types-aiobotocore-ecr-public-2.5.1/types_aiobotocore_ecr_public/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 01:30:24.000000 types-aiobotocore-ecr-public-2.5.1/types_aiobotocore_ecr_public/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    23781 2023-06-28 01:30:25.000000 types-aiobotocore-ecr-public-2.5.1/types_aiobotocore_ecr_public/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    23746 2023-06-28 01:30:25.000000 types-aiobotocore-ecr-public-2.5.1/types_aiobotocore_ecr_public/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-28 01:30:24.000000 types-aiobotocore-ecr-public-2.5.1/types_aiobotocore_ecr_public/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 01:43:26.386131 types-aiobotocore-ecr-public-2.5.1/types_aiobotocore_ecr_public.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16163 2023-06-28 01:43:26.000000 types-aiobotocore-ecr-public-2.5.1/types_aiobotocore_ecr_public.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-06-28 01:43:26.000000 types-aiobotocore-ecr-public-2.5.1/types_aiobotocore_ecr_public.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 01:43:26.000000 types-aiobotocore-ecr-public-2.5.1/types_aiobotocore_ecr_public.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 01:43:26.000000 types-aiobotocore-ecr-public-2.5.1/types_aiobotocore_ecr_public.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-28 01:43:26.000000 types-aiobotocore-ecr-public-2.5.1/types_aiobotocore_ecr_public.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-28 01:43:26.000000 types-aiobotocore-ecr-public-2.5.1/types_aiobotocore_ecr_public.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:34.466071 types-aiobotocore-ecr-public-2.5.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:30:06.000000 types-aiobotocore-ecr-public-2.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16163 2023-07-08 01:43:34.466071 types-aiobotocore-ecr-public-2.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14587 2023-07-08 01:30:06.000000 types-aiobotocore-ecr-public-2.5.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:43:34.466071 types-aiobotocore-ecr-public-2.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-07-08 01:30:06.000000 types-aiobotocore-ecr-public-2.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:34.466071 types-aiobotocore-ecr-public-2.5.2/types_aiobotocore_ecr_public/
+-rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-07-08 01:30:06.000000 types-aiobotocore-ecr-public-2.5.2/types_aiobotocore_ecr_public/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-07-08 01:30:06.000000 types-aiobotocore-ecr-public-2.5.2/types_aiobotocore_ecr_public/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-07-08 01:30:06.000000 types-aiobotocore-ecr-public-2.5.2/types_aiobotocore_ecr_public/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22197 2023-07-08 01:30:06.000000 types-aiobotocore-ecr-public-2.5.2/types_aiobotocore_ecr_public/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22161 2023-07-08 01:30:06.000000 types-aiobotocore-ecr-public-2.5.2/types_aiobotocore_ecr_public/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8722 2023-07-08 01:30:06.000000 types-aiobotocore-ecr-public-2.5.2/types_aiobotocore_ecr_public/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8720 2023-07-08 01:30:06.000000 types-aiobotocore-ecr-public-2.5.2/types_aiobotocore_ecr_public/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5762 2023-07-08 01:30:06.000000 types-aiobotocore-ecr-public-2.5.2/types_aiobotocore_ecr_public/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5756 2023-07-08 01:30:06.000000 types-aiobotocore-ecr-public-2.5.2/types_aiobotocore_ecr_public/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:30:06.000000 types-aiobotocore-ecr-public-2.5.2/types_aiobotocore_ecr_public/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    23781 2023-07-08 01:30:07.000000 types-aiobotocore-ecr-public-2.5.2/types_aiobotocore_ecr_public/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23746 2023-07-08 01:30:06.000000 types-aiobotocore-ecr-public-2.5.2/types_aiobotocore_ecr_public/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:30:06.000000 types-aiobotocore-ecr-public-2.5.2/types_aiobotocore_ecr_public/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:34.466071 types-aiobotocore-ecr-public-2.5.2/types_aiobotocore_ecr_public.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16163 2023-07-08 01:43:34.000000 types-aiobotocore-ecr-public-2.5.2/types_aiobotocore_ecr_public.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-07-08 01:43:34.000000 types-aiobotocore-ecr-public-2.5.2/types_aiobotocore_ecr_public.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:34.000000 types-aiobotocore-ecr-public-2.5.2/types_aiobotocore_ecr_public.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:34.000000 types-aiobotocore-ecr-public-2.5.2/types_aiobotocore_ecr_public.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:43:34.000000 types-aiobotocore-ecr-public-2.5.2/types_aiobotocore_ecr_public.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-08 01:43:34.000000 types-aiobotocore-ecr-public-2.5.2/types_aiobotocore_ecr_public.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-ecr-public-2.5.1/LICENSE` & `types-aiobotocore-ecr-public-2.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ecr-public-2.5.1/PKG-INFO` & `types-aiobotocore-ecr-public-2.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-ecr-public
-Version: 2.5.1
-Summary: Type annotations for aiobotocore.ECRPublic 2.5.1 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2
+Summary: Type annotations for aiobotocore.ECRPublic 2.5.2 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecr_public/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-ecr-public.svg?color=blue)](https://pypi.org/project/types-aiobotocore-ecr-public)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecr_public/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-ecr-public?color=blue)](https://pypistats.org/packages/types-aiobotocore-ecr-public)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ECRPublic 2.5.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr-public.html#ECRPublic)
+[aiobotocore.ECRPublic 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr-public.html#ECRPublic)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-ecr-public-2.5.1/README.md` & `types-aiobotocore-ecr-public-2.5.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-ecr-public.svg?color=blue)](https://pypi.org/project/types-aiobotocore-ecr-public)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecr_public/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-ecr-public?color=blue)](https://pypistats.org/packages/types-aiobotocore-ecr-public)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ECRPublic 2.5.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr-public.html#ECRPublic)
+[aiobotocore.ECRPublic 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr-public.html#ECRPublic)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-ecr-public-2.5.1/setup.py` & `types-aiobotocore-ecr-public-2.5.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-ecr-public",
-    version="2.5.1",
+    version="2.5.2",
     packages=["types_aiobotocore_ecr_public"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.ECRPublic 2.5.1 service generated with mypy-boto3-builder"
+        "Type annotations for aiobotocore.ECRPublic 2.5.2 service generated with mypy-boto3-builder"
         " 7.14.5"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-ecr-public-2.5.1/types_aiobotocore_ecr_public/__init__.py` & `types-aiobotocore-ecr-public-2.5.2/types_aiobotocore_ecr_public/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ecr-public-2.5.1/types_aiobotocore_ecr_public/__init__.pyi` & `types-aiobotocore-ecr-public-2.5.2/types_aiobotocore_ecr_public/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ecr-public-2.5.1/types_aiobotocore_ecr_public/__main__.py` & `types-aiobotocore-ecr-public-2.5.2/types_aiobotocore_ecr_public/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.ECRPublic 2.5.1\nVersion:         2.5.1\nBuilder version:"
+        "Type annotations for aiobotocore.ECRPublic 2.5.2\nVersion:         2.5.2\nBuilder version:"
         " 7.14.5\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecr_public//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr-public.html#ECRPublic\nOther"
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

### Comparing `types-aiobotocore-ecr-public-2.5.1/types_aiobotocore_ecr_public/client.py` & `types-aiobotocore-ecr-public-2.5.2/types_aiobotocore_ecr_public/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ecr-public-2.5.1/types_aiobotocore_ecr_public/client.pyi` & `types-aiobotocore-ecr-public-2.5.2/types_aiobotocore_ecr_public/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ecr-public-2.5.1/types_aiobotocore_ecr_public/literals.py` & `types-aiobotocore-ecr-public-2.5.2/types_aiobotocore_ecr_public/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ecr-public-2.5.1/types_aiobotocore_ecr_public/literals.pyi` & `types-aiobotocore-ecr-public-2.5.2/types_aiobotocore_ecr_public/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ecr-public-2.5.1/types_aiobotocore_ecr_public/paginator.py` & `types-aiobotocore-ecr-public-2.5.2/types_aiobotocore_ecr_public/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ecr-public-2.5.1/types_aiobotocore_ecr_public/paginator.pyi` & `types-aiobotocore-ecr-public-2.5.2/types_aiobotocore_ecr_public/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ecr-public-2.5.1/types_aiobotocore_ecr_public/type_defs.py` & `types-aiobotocore-ecr-public-2.5.2/types_aiobotocore_ecr_public/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ecr-public-2.5.1/types_aiobotocore_ecr_public/type_defs.pyi` & `types-aiobotocore-ecr-public-2.5.2/types_aiobotocore_ecr_public/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ecr-public-2.5.1/types_aiobotocore_ecr_public.egg-info/PKG-INFO` & `types-aiobotocore-ecr-public-2.5.2/types_aiobotocore_ecr_public.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-ecr-public
-Version: 2.5.1
-Summary: Type annotations for aiobotocore.ECRPublic 2.5.1 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2
+Summary: Type annotations for aiobotocore.ECRPublic 2.5.2 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecr_public/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-ecr-public.svg?color=blue)](https://pypi.org/project/types-aiobotocore-ecr-public)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecr_public/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-ecr-public?color=blue)](https://pypistats.org/packages/types-aiobotocore-ecr-public)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ECRPublic 2.5.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr-public.html#ECRPublic)
+[aiobotocore.ECRPublic 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr-public.html#ECRPublic)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-ecr-public-2.5.1/types_aiobotocore_ecr_public.egg-info/SOURCES.txt` & `types-aiobotocore-ecr-public-2.5.2/types_aiobotocore_ecr_public.egg-info/SOURCES.txt`

 * *Files identical despite different names*

