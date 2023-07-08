# Comparing `tmp/types-aiobotocore-apigateway-2.5.1.tar.gz` & `tmp/types-aiobotocore-apigateway-2.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-apigateway-2.5.1.tar", last modified: Wed Jun 28 01:43:04 2023, max compression
+gzip compressed data, was "types-aiobotocore-apigateway-2.5.2.tar", last modified: Sat Jul  8 01:43:12 2023, max compression
```

## Comparing `types-aiobotocore-apigateway-2.5.1.tar` & `types-aiobotocore-apigateway-2.5.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 01:43:04.334090 types-aiobotocore-apigateway-2.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-28 01:25:57.000000 types-aiobotocore-apigateway-2.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    25179 2023-06-28 01:43:04.326090 types-aiobotocore-apigateway-2.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    23602 2023-06-28 01:25:57.000000 types-aiobotocore-apigateway-2.5.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-28 01:43:04.334090 types-aiobotocore-apigateway-2.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-06-28 01:25:57.000000 types-aiobotocore-apigateway-2.5.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 01:43:04.326090 types-aiobotocore-apigateway-2.5.1/types_aiobotocore_apigateway/
--rw-r--r--   0 runner    (1001) docker     (123)     4045 2023-06-28 01:25:57.000000 types-aiobotocore-apigateway-2.5.1/types_aiobotocore_apigateway/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4044 2023-06-28 01:25:57.000000 types-aiobotocore-apigateway-2.5.1/types_aiobotocore_apigateway/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-06-28 01:25:57.000000 types-aiobotocore-apigateway-2.5.1/types_aiobotocore_apigateway/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    87448 2023-06-28 01:25:58.000000 types-aiobotocore-apigateway-2.5.1/types_aiobotocore_apigateway/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    87301 2023-06-28 01:25:58.000000 types-aiobotocore-apigateway-2.5.1/types_aiobotocore_apigateway/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12970 2023-06-28 01:25:58.000000 types-aiobotocore-apigateway-2.5.1/types_aiobotocore_apigateway/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    12968 2023-06-28 01:25:58.000000 types-aiobotocore-apigateway-2.5.1/types_aiobotocore_apigateway/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    20962 2023-06-28 01:25:58.000000 types-aiobotocore-apigateway-2.5.1/types_aiobotocore_apigateway/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    20942 2023-06-28 01:25:58.000000 types-aiobotocore-apigateway-2.5.1/types_aiobotocore_apigateway/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 01:25:57.000000 types-aiobotocore-apigateway-2.5.1/types_aiobotocore_apigateway/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    93141 2023-06-28 01:26:01.000000 types-aiobotocore-apigateway-2.5.1/types_aiobotocore_apigateway/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    92992 2023-06-28 01:25:59.000000 types-aiobotocore-apigateway-2.5.1/types_aiobotocore_apigateway/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-28 01:25:57.000000 types-aiobotocore-apigateway-2.5.1/types_aiobotocore_apigateway/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 01:43:04.326090 types-aiobotocore-apigateway-2.5.1/types_aiobotocore_apigateway.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    25179 2023-06-28 01:43:04.000000 types-aiobotocore-apigateway-2.5.1/types_aiobotocore_apigateway.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-06-28 01:43:04.000000 types-aiobotocore-apigateway-2.5.1/types_aiobotocore_apigateway.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 01:43:04.000000 types-aiobotocore-apigateway-2.5.1/types_aiobotocore_apigateway.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 01:43:04.000000 types-aiobotocore-apigateway-2.5.1/types_aiobotocore_apigateway.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-28 01:43:04.000000 types-aiobotocore-apigateway-2.5.1/types_aiobotocore_apigateway.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-28 01:43:04.000000 types-aiobotocore-apigateway-2.5.1/types_aiobotocore_apigateway.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:12.377653 types-aiobotocore-apigateway-2.5.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:25:31.000000 types-aiobotocore-apigateway-2.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    25179 2023-07-08 01:43:12.369652 types-aiobotocore-apigateway-2.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    23602 2023-07-08 01:25:31.000000 types-aiobotocore-apigateway-2.5.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:43:12.377653 types-aiobotocore-apigateway-2.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-07-08 01:25:31.000000 types-aiobotocore-apigateway-2.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:12.369652 types-aiobotocore-apigateway-2.5.2/types_aiobotocore_apigateway/
+-rw-r--r--   0 runner    (1001) docker     (123)     4045 2023-07-08 01:25:31.000000 types-aiobotocore-apigateway-2.5.2/types_aiobotocore_apigateway/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4044 2023-07-08 01:25:31.000000 types-aiobotocore-apigateway-2.5.2/types_aiobotocore_apigateway/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-07-08 01:25:31.000000 types-aiobotocore-apigateway-2.5.2/types_aiobotocore_apigateway/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    87448 2023-07-08 01:25:32.000000 types-aiobotocore-apigateway-2.5.2/types_aiobotocore_apigateway/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    87301 2023-07-08 01:25:32.000000 types-aiobotocore-apigateway-2.5.2/types_aiobotocore_apigateway/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12970 2023-07-08 01:25:33.000000 types-aiobotocore-apigateway-2.5.2/types_aiobotocore_apigateway/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12968 2023-07-08 01:25:32.000000 types-aiobotocore-apigateway-2.5.2/types_aiobotocore_apigateway/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    20962 2023-07-08 01:25:32.000000 types-aiobotocore-apigateway-2.5.2/types_aiobotocore_apigateway/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20942 2023-07-08 01:25:32.000000 types-aiobotocore-apigateway-2.5.2/types_aiobotocore_apigateway/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:25:31.000000 types-aiobotocore-apigateway-2.5.2/types_aiobotocore_apigateway/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    93141 2023-07-08 01:25:35.000000 types-aiobotocore-apigateway-2.5.2/types_aiobotocore_apigateway/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    92992 2023-07-08 01:25:33.000000 types-aiobotocore-apigateway-2.5.2/types_aiobotocore_apigateway/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:25:31.000000 types-aiobotocore-apigateway-2.5.2/types_aiobotocore_apigateway/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:12.369652 types-aiobotocore-apigateway-2.5.2/types_aiobotocore_apigateway.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    25179 2023-07-08 01:43:12.000000 types-aiobotocore-apigateway-2.5.2/types_aiobotocore_apigateway.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-07-08 01:43:12.000000 types-aiobotocore-apigateway-2.5.2/types_aiobotocore_apigateway.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:12.000000 types-aiobotocore-apigateway-2.5.2/types_aiobotocore_apigateway.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:12.000000 types-aiobotocore-apigateway-2.5.2/types_aiobotocore_apigateway.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:43:12.000000 types-aiobotocore-apigateway-2.5.2/types_aiobotocore_apigateway.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-08 01:43:12.000000 types-aiobotocore-apigateway-2.5.2/types_aiobotocore_apigateway.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-apigateway-2.5.1/LICENSE` & `types-aiobotocore-apigateway-2.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-apigateway-2.5.1/PKG-INFO` & `types-aiobotocore-apigateway-2.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-apigateway
-Version: 2.5.1
-Summary: Type annotations for aiobotocore.APIGateway 2.5.1 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2
+Summary: Type annotations for aiobotocore.APIGateway 2.5.2 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigateway/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-apigateway.svg?color=blue)](https://pypi.org/project/types-aiobotocore-apigateway)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigateway/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-apigateway?color=blue)](https://pypistats.org/packages/types-aiobotocore-apigateway)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.APIGateway 2.5.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway)
+[aiobotocore.APIGateway 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-apigateway-2.5.1/README.md` & `types-aiobotocore-apigateway-2.5.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-apigateway.svg?color=blue)](https://pypi.org/project/types-aiobotocore-apigateway)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigateway/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-apigateway?color=blue)](https://pypistats.org/packages/types-aiobotocore-apigateway)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.APIGateway 2.5.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway)
+[aiobotocore.APIGateway 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-apigateway-2.5.1/setup.py` & `types-aiobotocore-apigateway-2.5.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-apigateway",
-    version="2.5.1",
+    version="2.5.2",
     packages=["types_aiobotocore_apigateway"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.APIGateway 2.5.1 service generated with"
+        "Type annotations for aiobotocore.APIGateway 2.5.2 service generated with"
         " mypy-boto3-builder 7.14.5"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-apigateway-2.5.1/types_aiobotocore_apigateway/__init__.py` & `types-aiobotocore-apigateway-2.5.2/types_aiobotocore_apigateway/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-apigateway-2.5.1/types_aiobotocore_apigateway/__init__.pyi` & `types-aiobotocore-apigateway-2.5.2/types_aiobotocore_apigateway/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-apigateway-2.5.1/types_aiobotocore_apigateway/__main__.py` & `types-aiobotocore-apigateway-2.5.2/types_aiobotocore_apigateway/__main__.py`

 * *Files 26% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.APIGateway 2.5.1\nVersion:         2.5.1\nBuilder"
+        "Type annotations for aiobotocore.APIGateway 2.5.2\nVersion:         2.5.2\nBuilder"
         " version: 7.14.5\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigateway//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway\nOther"
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

### Comparing `types-aiobotocore-apigateway-2.5.1/types_aiobotocore_apigateway/client.py` & `types-aiobotocore-apigateway-2.5.2/types_aiobotocore_apigateway/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-apigateway-2.5.1/types_aiobotocore_apigateway/client.pyi` & `types-aiobotocore-apigateway-2.5.2/types_aiobotocore_apigateway/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-apigateway-2.5.1/types_aiobotocore_apigateway/literals.py` & `types-aiobotocore-apigateway-2.5.2/types_aiobotocore_apigateway/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-apigateway-2.5.1/types_aiobotocore_apigateway/literals.pyi` & `types-aiobotocore-apigateway-2.5.2/types_aiobotocore_apigateway/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-apigateway-2.5.1/types_aiobotocore_apigateway/paginator.py` & `types-aiobotocore-apigateway-2.5.2/types_aiobotocore_apigateway/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-apigateway-2.5.1/types_aiobotocore_apigateway/paginator.pyi` & `types-aiobotocore-apigateway-2.5.2/types_aiobotocore_apigateway/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-apigateway-2.5.1/types_aiobotocore_apigateway/type_defs.py` & `types-aiobotocore-apigateway-2.5.2/types_aiobotocore_apigateway/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-apigateway-2.5.1/types_aiobotocore_apigateway/type_defs.pyi` & `types-aiobotocore-apigateway-2.5.2/types_aiobotocore_apigateway/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-apigateway-2.5.1/types_aiobotocore_apigateway.egg-info/PKG-INFO` & `types-aiobotocore-apigateway-2.5.2/types_aiobotocore_apigateway.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-apigateway
-Version: 2.5.1
-Summary: Type annotations for aiobotocore.APIGateway 2.5.1 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2
+Summary: Type annotations for aiobotocore.APIGateway 2.5.2 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigateway/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-apigateway.svg?color=blue)](https://pypi.org/project/types-aiobotocore-apigateway)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigateway/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-apigateway?color=blue)](https://pypistats.org/packages/types-aiobotocore-apigateway)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.APIGateway 2.5.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway)
+[aiobotocore.APIGateway 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-apigateway-2.5.1/types_aiobotocore_apigateway.egg-info/SOURCES.txt` & `types-aiobotocore-apigateway-2.5.2/types_aiobotocore_apigateway.egg-info/SOURCES.txt`

 * *Files identical despite different names*

