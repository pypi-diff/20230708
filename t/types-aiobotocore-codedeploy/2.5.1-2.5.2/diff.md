# Comparing `tmp/types-aiobotocore-codedeploy-2.5.1.tar.gz` & `tmp/types-aiobotocore-codedeploy-2.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-codedeploy-2.5.1.tar", last modified: Wed Jun 28 01:43:15 2023, max compression
+gzip compressed data, was "types-aiobotocore-codedeploy-2.5.2.tar", last modified: Sat Jul  8 01:43:23 2023, max compression
```

## Comparing `types-aiobotocore-codedeploy-2.5.1.tar` & `types-aiobotocore-codedeploy-2.5.2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 01:43:15.738111 types-aiobotocore-codedeploy-2.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-28 01:27:54.000000 types-aiobotocore-codedeploy-2.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    22218 2023-06-28 01:43:15.738111 types-aiobotocore-codedeploy-2.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    20641 2023-06-28 01:27:54.000000 types-aiobotocore-codedeploy-2.5.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-28 01:43:15.738111 types-aiobotocore-codedeploy-2.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-06-28 01:27:54.000000 types-aiobotocore-codedeploy-2.5.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 01:43:15.738111 types-aiobotocore-codedeploy-2.5.1/types_aiobotocore_codedeploy/
--rw-r--r--   0 runner    (1001) docker     (123)     2845 2023-06-28 01:27:54.000000 types-aiobotocore-codedeploy-2.5.1/types_aiobotocore_codedeploy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-06-28 01:27:54.000000 types-aiobotocore-codedeploy-2.5.1/types_aiobotocore_codedeploy/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-06-28 01:27:54.000000 types-aiobotocore-codedeploy-2.5.1/types_aiobotocore_codedeploy/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    48531 2023-06-28 01:27:54.000000 types-aiobotocore-codedeploy-2.5.1/types_aiobotocore_codedeploy/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    48465 2023-06-28 01:27:54.000000 types-aiobotocore-codedeploy-2.5.1/types_aiobotocore_codedeploy/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    14449 2023-06-28 01:27:55.000000 types-aiobotocore-codedeploy-2.5.1/types_aiobotocore_codedeploy/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    14447 2023-06-28 01:27:55.000000 types-aiobotocore-codedeploy-2.5.1/types_aiobotocore_codedeploy/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12652 2023-06-28 01:27:55.000000 types-aiobotocore-codedeploy-2.5.1/types_aiobotocore_codedeploy/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    12641 2023-06-28 01:27:54.000000 types-aiobotocore-codedeploy-2.5.1/types_aiobotocore_codedeploy/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 01:27:54.000000 types-aiobotocore-codedeploy-2.5.1/types_aiobotocore_codedeploy/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    50701 2023-06-28 01:27:56.000000 types-aiobotocore-codedeploy-2.5.1/types_aiobotocore_codedeploy/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    50668 2023-06-28 01:27:55.000000 types-aiobotocore-codedeploy-2.5.1/types_aiobotocore_codedeploy/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-28 01:27:54.000000 types-aiobotocore-codedeploy-2.5.1/types_aiobotocore_codedeploy/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-06-28 01:27:55.000000 types-aiobotocore-codedeploy-2.5.1/types_aiobotocore_codedeploy/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-06-28 01:27:55.000000 types-aiobotocore-codedeploy-2.5.1/types_aiobotocore_codedeploy/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 01:43:15.738111 types-aiobotocore-codedeploy-2.5.1/types_aiobotocore_codedeploy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    22218 2023-06-28 01:43:15.000000 types-aiobotocore-codedeploy-2.5.1/types_aiobotocore_codedeploy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-06-28 01:43:15.000000 types-aiobotocore-codedeploy-2.5.1/types_aiobotocore_codedeploy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 01:43:15.000000 types-aiobotocore-codedeploy-2.5.1/types_aiobotocore_codedeploy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 01:43:15.000000 types-aiobotocore-codedeploy-2.5.1/types_aiobotocore_codedeploy.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-28 01:43:15.000000 types-aiobotocore-codedeploy-2.5.1/types_aiobotocore_codedeploy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-28 01:43:15.000000 types-aiobotocore-codedeploy-2.5.1/types_aiobotocore_codedeploy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:23.861869 types-aiobotocore-codedeploy-2.5.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:27:31.000000 types-aiobotocore-codedeploy-2.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    22218 2023-07-08 01:43:23.861869 types-aiobotocore-codedeploy-2.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    20641 2023-07-08 01:27:31.000000 types-aiobotocore-codedeploy-2.5.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:43:23.861869 types-aiobotocore-codedeploy-2.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-07-08 01:27:31.000000 types-aiobotocore-codedeploy-2.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:23.857869 types-aiobotocore-codedeploy-2.5.2/types_aiobotocore_codedeploy/
+-rw-r--r--   0 runner    (1001) docker     (123)     2845 2023-07-08 01:27:31.000000 types-aiobotocore-codedeploy-2.5.2/types_aiobotocore_codedeploy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-07-08 01:27:31.000000 types-aiobotocore-codedeploy-2.5.2/types_aiobotocore_codedeploy/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-07-08 01:27:31.000000 types-aiobotocore-codedeploy-2.5.2/types_aiobotocore_codedeploy/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48531 2023-07-08 01:27:32.000000 types-aiobotocore-codedeploy-2.5.2/types_aiobotocore_codedeploy/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48465 2023-07-08 01:27:31.000000 types-aiobotocore-codedeploy-2.5.2/types_aiobotocore_codedeploy/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    14449 2023-07-08 01:27:32.000000 types-aiobotocore-codedeploy-2.5.2/types_aiobotocore_codedeploy/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14447 2023-07-08 01:27:32.000000 types-aiobotocore-codedeploy-2.5.2/types_aiobotocore_codedeploy/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12652 2023-07-08 01:27:32.000000 types-aiobotocore-codedeploy-2.5.2/types_aiobotocore_codedeploy/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12641 2023-07-08 01:27:32.000000 types-aiobotocore-codedeploy-2.5.2/types_aiobotocore_codedeploy/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:27:31.000000 types-aiobotocore-codedeploy-2.5.2/types_aiobotocore_codedeploy/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    50701 2023-07-08 01:27:33.000000 types-aiobotocore-codedeploy-2.5.2/types_aiobotocore_codedeploy/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50668 2023-07-08 01:27:32.000000 types-aiobotocore-codedeploy-2.5.2/types_aiobotocore_codedeploy/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:27:31.000000 types-aiobotocore-codedeploy-2.5.2/types_aiobotocore_codedeploy/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-07-08 01:27:32.000000 types-aiobotocore-codedeploy-2.5.2/types_aiobotocore_codedeploy/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-07-08 01:27:32.000000 types-aiobotocore-codedeploy-2.5.2/types_aiobotocore_codedeploy/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:23.861869 types-aiobotocore-codedeploy-2.5.2/types_aiobotocore_codedeploy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    22218 2023-07-08 01:43:23.000000 types-aiobotocore-codedeploy-2.5.2/types_aiobotocore_codedeploy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-07-08 01:43:23.000000 types-aiobotocore-codedeploy-2.5.2/types_aiobotocore_codedeploy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:23.000000 types-aiobotocore-codedeploy-2.5.2/types_aiobotocore_codedeploy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:23.000000 types-aiobotocore-codedeploy-2.5.2/types_aiobotocore_codedeploy.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:43:23.000000 types-aiobotocore-codedeploy-2.5.2/types_aiobotocore_codedeploy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-08 01:43:23.000000 types-aiobotocore-codedeploy-2.5.2/types_aiobotocore_codedeploy.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-codedeploy-2.5.1/LICENSE` & `types-aiobotocore-codedeploy-2.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codedeploy-2.5.1/PKG-INFO` & `types-aiobotocore-codedeploy-2.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-codedeploy
-Version: 2.5.1
-Summary: Type annotations for aiobotocore.CodeDeploy 2.5.1 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2
+Summary: Type annotations for aiobotocore.CodeDeploy 2.5.2 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codedeploy/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-codedeploy.svg?color=blue)](https://pypi.org/project/types-aiobotocore-codedeploy)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codedeploy/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-codedeploy?color=blue)](https://pypistats.org/packages/types-aiobotocore-codedeploy)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.CodeDeploy 2.5.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#CodeDeploy)
+[aiobotocore.CodeDeploy 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#CodeDeploy)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-codedeploy-2.5.1/README.md` & `types-aiobotocore-codedeploy-2.5.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-codedeploy.svg?color=blue)](https://pypi.org/project/types-aiobotocore-codedeploy)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codedeploy/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-codedeploy?color=blue)](https://pypistats.org/packages/types-aiobotocore-codedeploy)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.CodeDeploy 2.5.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#CodeDeploy)
+[aiobotocore.CodeDeploy 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#CodeDeploy)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-codedeploy-2.5.1/setup.py` & `types-aiobotocore-codedeploy-2.5.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-codedeploy",
-    version="2.5.1",
+    version="2.5.2",
     packages=["types_aiobotocore_codedeploy"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.CodeDeploy 2.5.1 service generated with"
+        "Type annotations for aiobotocore.CodeDeploy 2.5.2 service generated with"
         " mypy-boto3-builder 7.14.5"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-codedeploy-2.5.1/types_aiobotocore_codedeploy/__init__.py` & `types-aiobotocore-codedeploy-2.5.2/types_aiobotocore_codedeploy/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codedeploy-2.5.1/types_aiobotocore_codedeploy/__init__.pyi` & `types-aiobotocore-codedeploy-2.5.2/types_aiobotocore_codedeploy/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codedeploy-2.5.1/types_aiobotocore_codedeploy/__main__.py` & `types-aiobotocore-codedeploy-2.5.2/types_aiobotocore_codedeploy/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.CodeDeploy 2.5.1\nVersion:         2.5.1\nBuilder"
+        "Type annotations for aiobotocore.CodeDeploy 2.5.2\nVersion:         2.5.2\nBuilder"
         " version: 7.14.5\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codedeploy//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#CodeDeploy\nOther"
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

### Comparing `types-aiobotocore-codedeploy-2.5.1/types_aiobotocore_codedeploy/client.py` & `types-aiobotocore-codedeploy-2.5.2/types_aiobotocore_codedeploy/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codedeploy-2.5.1/types_aiobotocore_codedeploy/client.pyi` & `types-aiobotocore-codedeploy-2.5.2/types_aiobotocore_codedeploy/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codedeploy-2.5.1/types_aiobotocore_codedeploy/literals.py` & `types-aiobotocore-codedeploy-2.5.2/types_aiobotocore_codedeploy/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codedeploy-2.5.1/types_aiobotocore_codedeploy/literals.pyi` & `types-aiobotocore-codedeploy-2.5.2/types_aiobotocore_codedeploy/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codedeploy-2.5.1/types_aiobotocore_codedeploy/paginator.py` & `types-aiobotocore-codedeploy-2.5.2/types_aiobotocore_codedeploy/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codedeploy-2.5.1/types_aiobotocore_codedeploy/paginator.pyi` & `types-aiobotocore-codedeploy-2.5.2/types_aiobotocore_codedeploy/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codedeploy-2.5.1/types_aiobotocore_codedeploy/type_defs.py` & `types-aiobotocore-codedeploy-2.5.2/types_aiobotocore_codedeploy/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codedeploy-2.5.1/types_aiobotocore_codedeploy/type_defs.pyi` & `types-aiobotocore-codedeploy-2.5.2/types_aiobotocore_codedeploy/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codedeploy-2.5.1/types_aiobotocore_codedeploy/waiter.py` & `types-aiobotocore-codedeploy-2.5.2/types_aiobotocore_codedeploy/waiter.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codedeploy-2.5.1/types_aiobotocore_codedeploy/waiter.pyi` & `types-aiobotocore-codedeploy-2.5.2/types_aiobotocore_codedeploy/waiter.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codedeploy-2.5.1/types_aiobotocore_codedeploy.egg-info/PKG-INFO` & `types-aiobotocore-codedeploy-2.5.2/types_aiobotocore_codedeploy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-codedeploy
-Version: 2.5.1
-Summary: Type annotations for aiobotocore.CodeDeploy 2.5.1 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2
+Summary: Type annotations for aiobotocore.CodeDeploy 2.5.2 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codedeploy/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-codedeploy.svg?color=blue)](https://pypi.org/project/types-aiobotocore-codedeploy)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codedeploy/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-codedeploy?color=blue)](https://pypistats.org/packages/types-aiobotocore-codedeploy)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.CodeDeploy 2.5.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#CodeDeploy)
+[aiobotocore.CodeDeploy 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#CodeDeploy)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-codedeploy-2.5.1/types_aiobotocore_codedeploy.egg-info/SOURCES.txt` & `types-aiobotocore-codedeploy-2.5.2/types_aiobotocore_codedeploy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

