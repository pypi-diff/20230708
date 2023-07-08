# Comparing `tmp/types-aiobotocore-cloudfront-2.5.1.tar.gz` & `tmp/types-aiobotocore-cloudfront-2.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-cloudfront-2.5.1.tar", last modified: Wed Jun 28 01:43:13 2023, max compression
+gzip compressed data, was "types-aiobotocore-cloudfront-2.5.2.tar", last modified: Sat Jul  8 01:43:21 2023, max compression
```

## Comparing `types-aiobotocore-cloudfront-2.5.1.tar` & `types-aiobotocore-cloudfront-2.5.2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 01:43:13.366107 types-aiobotocore-cloudfront-2.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-28 01:27:26.000000 types-aiobotocore-cloudfront-2.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    31189 2023-06-28 01:43:13.358107 types-aiobotocore-cloudfront-2.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    29612 2023-06-28 01:27:26.000000 types-aiobotocore-cloudfront-2.5.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-28 01:43:13.366107 types-aiobotocore-cloudfront-2.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-06-28 01:27:26.000000 types-aiobotocore-cloudfront-2.5.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 01:43:13.350107 types-aiobotocore-cloudfront-2.5.1/types_aiobotocore_cloudfront/
--rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-06-28 01:27:26.000000 types-aiobotocore-cloudfront-2.5.1/types_aiobotocore_cloudfront/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-06-28 01:27:26.000000 types-aiobotocore-cloudfront-2.5.1/types_aiobotocore_cloudfront/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-06-28 01:27:26.000000 types-aiobotocore-cloudfront-2.5.1/types_aiobotocore_cloudfront/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    83274 2023-06-28 01:27:27.000000 types-aiobotocore-cloudfront-2.5.1/types_aiobotocore_cloudfront/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    83152 2023-06-28 01:27:27.000000 types-aiobotocore-cloudfront-2.5.1/types_aiobotocore_cloudfront/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12472 2023-06-28 01:27:27.000000 types-aiobotocore-cloudfront-2.5.1/types_aiobotocore_cloudfront/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    12470 2023-06-28 01:27:27.000000 types-aiobotocore-cloudfront-2.5.1/types_aiobotocore_cloudfront/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5768 2023-06-28 01:27:27.000000 types-aiobotocore-cloudfront-2.5.1/types_aiobotocore_cloudfront/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5762 2023-06-28 01:27:27.000000 types-aiobotocore-cloudfront-2.5.1/types_aiobotocore_cloudfront/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 01:27:26.000000 types-aiobotocore-cloudfront-2.5.1/types_aiobotocore_cloudfront/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)   138536 2023-06-28 01:27:30.000000 types-aiobotocore-cloudfront-2.5.1/types_aiobotocore_cloudfront/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)   138273 2023-06-28 01:27:29.000000 types-aiobotocore-cloudfront-2.5.1/types_aiobotocore_cloudfront/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-28 01:27:26.000000 types-aiobotocore-cloudfront-2.5.1/types_aiobotocore_cloudfront/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3770 2023-06-28 01:27:27.000000 types-aiobotocore-cloudfront-2.5.1/types_aiobotocore_cloudfront/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3767 2023-06-28 01:27:27.000000 types-aiobotocore-cloudfront-2.5.1/types_aiobotocore_cloudfront/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 01:43:13.358107 types-aiobotocore-cloudfront-2.5.1/types_aiobotocore_cloudfront.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    31189 2023-06-28 01:43:13.000000 types-aiobotocore-cloudfront-2.5.1/types_aiobotocore_cloudfront.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-06-28 01:43:13.000000 types-aiobotocore-cloudfront-2.5.1/types_aiobotocore_cloudfront.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 01:43:13.000000 types-aiobotocore-cloudfront-2.5.1/types_aiobotocore_cloudfront.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 01:43:13.000000 types-aiobotocore-cloudfront-2.5.1/types_aiobotocore_cloudfront.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-28 01:43:13.000000 types-aiobotocore-cloudfront-2.5.1/types_aiobotocore_cloudfront.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-28 01:43:13.000000 types-aiobotocore-cloudfront-2.5.1/types_aiobotocore_cloudfront.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:21.477824 types-aiobotocore-cloudfront-2.5.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:27:02.000000 types-aiobotocore-cloudfront-2.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    31189 2023-07-08 01:43:21.477824 types-aiobotocore-cloudfront-2.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    29612 2023-07-08 01:27:02.000000 types-aiobotocore-cloudfront-2.5.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:43:21.477824 types-aiobotocore-cloudfront-2.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-07-08 01:27:02.000000 types-aiobotocore-cloudfront-2.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:21.477824 types-aiobotocore-cloudfront-2.5.2/types_aiobotocore_cloudfront/
+-rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-07-08 01:27:02.000000 types-aiobotocore-cloudfront-2.5.2/types_aiobotocore_cloudfront/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-07-08 01:27:02.000000 types-aiobotocore-cloudfront-2.5.2/types_aiobotocore_cloudfront/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-07-08 01:27:02.000000 types-aiobotocore-cloudfront-2.5.2/types_aiobotocore_cloudfront/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    83274 2023-07-08 01:27:04.000000 types-aiobotocore-cloudfront-2.5.2/types_aiobotocore_cloudfront/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    83152 2023-07-08 01:27:03.000000 types-aiobotocore-cloudfront-2.5.2/types_aiobotocore_cloudfront/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12472 2023-07-08 01:27:04.000000 types-aiobotocore-cloudfront-2.5.2/types_aiobotocore_cloudfront/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12470 2023-07-08 01:27:04.000000 types-aiobotocore-cloudfront-2.5.2/types_aiobotocore_cloudfront/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5768 2023-07-08 01:27:04.000000 types-aiobotocore-cloudfront-2.5.2/types_aiobotocore_cloudfront/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5762 2023-07-08 01:27:04.000000 types-aiobotocore-cloudfront-2.5.2/types_aiobotocore_cloudfront/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:27:02.000000 types-aiobotocore-cloudfront-2.5.2/types_aiobotocore_cloudfront/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)   138536 2023-07-08 01:27:07.000000 types-aiobotocore-cloudfront-2.5.2/types_aiobotocore_cloudfront/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   138273 2023-07-08 01:27:05.000000 types-aiobotocore-cloudfront-2.5.2/types_aiobotocore_cloudfront/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:27:02.000000 types-aiobotocore-cloudfront-2.5.2/types_aiobotocore_cloudfront/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3770 2023-07-08 01:27:04.000000 types-aiobotocore-cloudfront-2.5.2/types_aiobotocore_cloudfront/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3767 2023-07-08 01:27:04.000000 types-aiobotocore-cloudfront-2.5.2/types_aiobotocore_cloudfront/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:21.477824 types-aiobotocore-cloudfront-2.5.2/types_aiobotocore_cloudfront.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    31189 2023-07-08 01:43:21.000000 types-aiobotocore-cloudfront-2.5.2/types_aiobotocore_cloudfront.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-07-08 01:43:21.000000 types-aiobotocore-cloudfront-2.5.2/types_aiobotocore_cloudfront.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:21.000000 types-aiobotocore-cloudfront-2.5.2/types_aiobotocore_cloudfront.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:21.000000 types-aiobotocore-cloudfront-2.5.2/types_aiobotocore_cloudfront.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:43:21.000000 types-aiobotocore-cloudfront-2.5.2/types_aiobotocore_cloudfront.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-08 01:43:21.000000 types-aiobotocore-cloudfront-2.5.2/types_aiobotocore_cloudfront.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-cloudfront-2.5.1/LICENSE` & `types-aiobotocore-cloudfront-2.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudfront-2.5.1/PKG-INFO` & `types-aiobotocore-cloudfront-2.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-cloudfront
-Version: 2.5.1
-Summary: Type annotations for aiobotocore.CloudFront 2.5.1 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2
+Summary: Type annotations for aiobotocore.CloudFront 2.5.2 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudfront/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-cloudfront.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cloudfront)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudfront/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-cloudfront?color=blue)](https://pypistats.org/packages/types-aiobotocore-cloudfront)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.CloudFront 2.5.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront)
+[aiobotocore.CloudFront 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-cloudfront-2.5.1/README.md` & `types-aiobotocore-cloudfront-2.5.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-cloudfront.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cloudfront)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudfront/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-cloudfront?color=blue)](https://pypistats.org/packages/types-aiobotocore-cloudfront)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.CloudFront 2.5.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront)
+[aiobotocore.CloudFront 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-cloudfront-2.5.1/setup.py` & `types-aiobotocore-cloudfront-2.5.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-cloudfront",
-    version="2.5.1",
+    version="2.5.2",
     packages=["types_aiobotocore_cloudfront"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.CloudFront 2.5.1 service generated with"
+        "Type annotations for aiobotocore.CloudFront 2.5.2 service generated with"
         " mypy-boto3-builder 7.14.5"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-cloudfront-2.5.1/types_aiobotocore_cloudfront/__init__.py` & `types-aiobotocore-cloudfront-2.5.2/types_aiobotocore_cloudfront/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudfront-2.5.1/types_aiobotocore_cloudfront/__init__.pyi` & `types-aiobotocore-cloudfront-2.5.2/types_aiobotocore_cloudfront/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudfront-2.5.1/types_aiobotocore_cloudfront/__main__.py` & `types-aiobotocore-cloudfront-2.5.2/types_aiobotocore_cloudfront/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.CloudFront 2.5.1\nVersion:         2.5.1\nBuilder"
+        "Type annotations for aiobotocore.CloudFront 2.5.2\nVersion:         2.5.2\nBuilder"
         " version: 7.14.5\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudfront//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront\nOther"
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

### Comparing `types-aiobotocore-cloudfront-2.5.1/types_aiobotocore_cloudfront/client.py` & `types-aiobotocore-cloudfront-2.5.2/types_aiobotocore_cloudfront/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudfront-2.5.1/types_aiobotocore_cloudfront/client.pyi` & `types-aiobotocore-cloudfront-2.5.2/types_aiobotocore_cloudfront/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudfront-2.5.1/types_aiobotocore_cloudfront/literals.py` & `types-aiobotocore-cloudfront-2.5.2/types_aiobotocore_cloudfront/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudfront-2.5.1/types_aiobotocore_cloudfront/literals.pyi` & `types-aiobotocore-cloudfront-2.5.2/types_aiobotocore_cloudfront/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudfront-2.5.1/types_aiobotocore_cloudfront/paginator.py` & `types-aiobotocore-cloudfront-2.5.2/types_aiobotocore_cloudfront/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudfront-2.5.1/types_aiobotocore_cloudfront/paginator.pyi` & `types-aiobotocore-cloudfront-2.5.2/types_aiobotocore_cloudfront/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudfront-2.5.1/types_aiobotocore_cloudfront/type_defs.py` & `types-aiobotocore-cloudfront-2.5.2/types_aiobotocore_cloudfront/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudfront-2.5.1/types_aiobotocore_cloudfront/type_defs.pyi` & `types-aiobotocore-cloudfront-2.5.2/types_aiobotocore_cloudfront/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudfront-2.5.1/types_aiobotocore_cloudfront/waiter.py` & `types-aiobotocore-cloudfront-2.5.2/types_aiobotocore_cloudfront/waiter.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudfront-2.5.1/types_aiobotocore_cloudfront/waiter.pyi` & `types-aiobotocore-cloudfront-2.5.2/types_aiobotocore_cloudfront/waiter.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudfront-2.5.1/types_aiobotocore_cloudfront.egg-info/PKG-INFO` & `types-aiobotocore-cloudfront-2.5.2/types_aiobotocore_cloudfront.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-cloudfront
-Version: 2.5.1
-Summary: Type annotations for aiobotocore.CloudFront 2.5.1 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2
+Summary: Type annotations for aiobotocore.CloudFront 2.5.2 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudfront/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-cloudfront.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cloudfront)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudfront/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-cloudfront?color=blue)](https://pypistats.org/packages/types-aiobotocore-cloudfront)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.CloudFront 2.5.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront)
+[aiobotocore.CloudFront 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-cloudfront-2.5.1/types_aiobotocore_cloudfront.egg-info/SOURCES.txt` & `types-aiobotocore-cloudfront-2.5.2/types_aiobotocore_cloudfront.egg-info/SOURCES.txt`

 * *Files identical despite different names*

