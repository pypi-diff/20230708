# Comparing `tmp/types-aiobotocore-appstream-2.5.1.tar.gz` & `tmp/types-aiobotocore-appstream-2.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-appstream-2.5.1.tar", last modified: Wed Jun 28 01:43:06 2023, max compression
+gzip compressed data, was "types-aiobotocore-appstream-2.5.2.tar", last modified: Sat Jul  8 01:43:14 2023, max compression
```

## Comparing `types-aiobotocore-appstream-2.5.1.tar` & `types-aiobotocore-appstream-2.5.2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 01:43:06.586094 types-aiobotocore-appstream-2.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-28 01:26:22.000000 types-aiobotocore-appstream-2.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    22699 2023-06-28 01:43:06.586094 types-aiobotocore-appstream-2.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    21126 2023-06-28 01:26:22.000000 types-aiobotocore-appstream-2.5.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-28 01:43:06.586094 types-aiobotocore-appstream-2.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2132 2023-06-28 01:26:22.000000 types-aiobotocore-appstream-2.5.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 01:43:06.578094 types-aiobotocore-appstream-2.5.1/types_aiobotocore_appstream/
--rw-r--r--   0 runner    (1001) docker     (123)     3011 2023-06-28 01:26:22.000000 types-aiobotocore-appstream-2.5.1/types_aiobotocore_appstream/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3010 2023-06-28 01:26:22.000000 types-aiobotocore-appstream-2.5.1/types_aiobotocore_appstream/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-06-28 01:26:22.000000 types-aiobotocore-appstream-2.5.1/types_aiobotocore_appstream/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    53969 2023-06-28 01:26:22.000000 types-aiobotocore-appstream-2.5.1/types_aiobotocore_appstream/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    53883 2023-06-28 01:26:22.000000 types-aiobotocore-appstream-2.5.1/types_aiobotocore_appstream/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    14248 2023-06-28 01:26:23.000000 types-aiobotocore-appstream-2.5.1/types_aiobotocore_appstream/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    14246 2023-06-28 01:26:23.000000 types-aiobotocore-appstream-2.5.1/types_aiobotocore_appstream/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12915 2023-06-28 01:26:23.000000 types-aiobotocore-appstream-2.5.1/types_aiobotocore_appstream/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    12903 2023-06-28 01:26:23.000000 types-aiobotocore-appstream-2.5.1/types_aiobotocore_appstream/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 01:26:22.000000 types-aiobotocore-appstream-2.5.1/types_aiobotocore_appstream/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    60987 2023-06-28 01:26:24.000000 types-aiobotocore-appstream-2.5.1/types_aiobotocore_appstream/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    60900 2023-06-28 01:26:23.000000 types-aiobotocore-appstream-2.5.1/types_aiobotocore_appstream/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-28 01:26:22.000000 types-aiobotocore-appstream-2.5.1/types_aiobotocore_appstream/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2638 2023-06-28 01:26:23.000000 types-aiobotocore-appstream-2.5.1/types_aiobotocore_appstream/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2636 2023-06-28 01:26:23.000000 types-aiobotocore-appstream-2.5.1/types_aiobotocore_appstream/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 01:43:06.586094 types-aiobotocore-appstream-2.5.1/types_aiobotocore_appstream.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    22699 2023-06-28 01:43:06.000000 types-aiobotocore-appstream-2.5.1/types_aiobotocore_appstream.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-06-28 01:43:06.000000 types-aiobotocore-appstream-2.5.1/types_aiobotocore_appstream.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 01:43:06.000000 types-aiobotocore-appstream-2.5.1/types_aiobotocore_appstream.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 01:43:06.000000 types-aiobotocore-appstream-2.5.1/types_aiobotocore_appstream.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-28 01:43:06.000000 types-aiobotocore-appstream-2.5.1/types_aiobotocore_appstream.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-28 01:43:06.000000 types-aiobotocore-appstream-2.5.1/types_aiobotocore_appstream.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:14.685696 types-aiobotocore-appstream-2.5.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:25:57.000000 types-aiobotocore-appstream-2.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    22699 2023-07-08 01:43:14.681696 types-aiobotocore-appstream-2.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    21126 2023-07-08 01:25:57.000000 types-aiobotocore-appstream-2.5.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:43:14.685696 types-aiobotocore-appstream-2.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2132 2023-07-08 01:25:57.000000 types-aiobotocore-appstream-2.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:14.673696 types-aiobotocore-appstream-2.5.2/types_aiobotocore_appstream/
+-rw-r--r--   0 runner    (1001) docker     (123)     3011 2023-07-08 01:25:57.000000 types-aiobotocore-appstream-2.5.2/types_aiobotocore_appstream/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3010 2023-07-08 01:25:57.000000 types-aiobotocore-appstream-2.5.2/types_aiobotocore_appstream/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-07-08 01:25:57.000000 types-aiobotocore-appstream-2.5.2/types_aiobotocore_appstream/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53969 2023-07-08 01:25:57.000000 types-aiobotocore-appstream-2.5.2/types_aiobotocore_appstream/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53883 2023-07-08 01:25:57.000000 types-aiobotocore-appstream-2.5.2/types_aiobotocore_appstream/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    14248 2023-07-08 01:25:58.000000 types-aiobotocore-appstream-2.5.2/types_aiobotocore_appstream/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14246 2023-07-08 01:25:57.000000 types-aiobotocore-appstream-2.5.2/types_aiobotocore_appstream/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12915 2023-07-08 01:25:57.000000 types-aiobotocore-appstream-2.5.2/types_aiobotocore_appstream/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12903 2023-07-08 01:25:57.000000 types-aiobotocore-appstream-2.5.2/types_aiobotocore_appstream/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:25:57.000000 types-aiobotocore-appstream-2.5.2/types_aiobotocore_appstream/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    60987 2023-07-08 01:25:59.000000 types-aiobotocore-appstream-2.5.2/types_aiobotocore_appstream/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60900 2023-07-08 01:25:58.000000 types-aiobotocore-appstream-2.5.2/types_aiobotocore_appstream/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:25:57.000000 types-aiobotocore-appstream-2.5.2/types_aiobotocore_appstream/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2638 2023-07-08 01:25:57.000000 types-aiobotocore-appstream-2.5.2/types_aiobotocore_appstream/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2636 2023-07-08 01:25:57.000000 types-aiobotocore-appstream-2.5.2/types_aiobotocore_appstream/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:14.681696 types-aiobotocore-appstream-2.5.2/types_aiobotocore_appstream.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    22699 2023-07-08 01:43:14.000000 types-aiobotocore-appstream-2.5.2/types_aiobotocore_appstream.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-07-08 01:43:14.000000 types-aiobotocore-appstream-2.5.2/types_aiobotocore_appstream.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:14.000000 types-aiobotocore-appstream-2.5.2/types_aiobotocore_appstream.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:14.000000 types-aiobotocore-appstream-2.5.2/types_aiobotocore_appstream.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:43:14.000000 types-aiobotocore-appstream-2.5.2/types_aiobotocore_appstream.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-08 01:43:14.000000 types-aiobotocore-appstream-2.5.2/types_aiobotocore_appstream.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-appstream-2.5.1/LICENSE` & `types-aiobotocore-appstream-2.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-appstream-2.5.1/PKG-INFO` & `types-aiobotocore-appstream-2.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-appstream
-Version: 2.5.1
-Summary: Type annotations for aiobotocore.AppStream 2.5.1 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2
+Summary: Type annotations for aiobotocore.AppStream 2.5.2 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appstream/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-appstream.svg?color=blue)](https://pypi.org/project/types-aiobotocore-appstream)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appstream/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-appstream?color=blue)](https://pypistats.org/packages/types-aiobotocore-appstream)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.AppStream 2.5.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream)
+[aiobotocore.AppStream 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-appstream-2.5.1/README.md` & `types-aiobotocore-appstream-2.5.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-appstream.svg?color=blue)](https://pypi.org/project/types-aiobotocore-appstream)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appstream/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-appstream?color=blue)](https://pypistats.org/packages/types-aiobotocore-appstream)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.AppStream 2.5.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream)
+[aiobotocore.AppStream 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-appstream-2.5.1/setup.py` & `types-aiobotocore-appstream-2.5.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-appstream",
-    version="2.5.1",
+    version="2.5.2",
     packages=["types_aiobotocore_appstream"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.AppStream 2.5.1 service generated with mypy-boto3-builder"
+        "Type annotations for aiobotocore.AppStream 2.5.2 service generated with mypy-boto3-builder"
         " 7.14.5"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-appstream-2.5.1/types_aiobotocore_appstream/__init__.py` & `types-aiobotocore-appstream-2.5.2/types_aiobotocore_appstream/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-appstream-2.5.1/types_aiobotocore_appstream/__init__.pyi` & `types-aiobotocore-appstream-2.5.2/types_aiobotocore_appstream/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-appstream-2.5.1/types_aiobotocore_appstream/__main__.py` & `types-aiobotocore-appstream-2.5.2/types_aiobotocore_appstream/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.AppStream 2.5.1\nVersion:         2.5.1\nBuilder version:"
+        "Type annotations for aiobotocore.AppStream 2.5.2\nVersion:         2.5.2\nBuilder version:"
         " 7.14.5\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appstream//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream\nOther"
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

### Comparing `types-aiobotocore-appstream-2.5.1/types_aiobotocore_appstream/client.py` & `types-aiobotocore-appstream-2.5.2/types_aiobotocore_appstream/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-appstream-2.5.1/types_aiobotocore_appstream/client.pyi` & `types-aiobotocore-appstream-2.5.2/types_aiobotocore_appstream/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-appstream-2.5.1/types_aiobotocore_appstream/literals.py` & `types-aiobotocore-appstream-2.5.2/types_aiobotocore_appstream/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-appstream-2.5.1/types_aiobotocore_appstream/literals.pyi` & `types-aiobotocore-appstream-2.5.2/types_aiobotocore_appstream/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-appstream-2.5.1/types_aiobotocore_appstream/paginator.py` & `types-aiobotocore-appstream-2.5.2/types_aiobotocore_appstream/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-appstream-2.5.1/types_aiobotocore_appstream/paginator.pyi` & `types-aiobotocore-appstream-2.5.2/types_aiobotocore_appstream/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-appstream-2.5.1/types_aiobotocore_appstream/type_defs.py` & `types-aiobotocore-appstream-2.5.2/types_aiobotocore_appstream/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-appstream-2.5.1/types_aiobotocore_appstream/type_defs.pyi` & `types-aiobotocore-appstream-2.5.2/types_aiobotocore_appstream/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-appstream-2.5.1/types_aiobotocore_appstream/waiter.py` & `types-aiobotocore-appstream-2.5.2/types_aiobotocore_appstream/waiter.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-appstream-2.5.1/types_aiobotocore_appstream/waiter.pyi` & `types-aiobotocore-appstream-2.5.2/types_aiobotocore_appstream/waiter.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-appstream-2.5.1/types_aiobotocore_appstream.egg-info/PKG-INFO` & `types-aiobotocore-appstream-2.5.2/types_aiobotocore_appstream.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-appstream
-Version: 2.5.1
-Summary: Type annotations for aiobotocore.AppStream 2.5.1 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2
+Summary: Type annotations for aiobotocore.AppStream 2.5.2 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appstream/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-appstream.svg?color=blue)](https://pypi.org/project/types-aiobotocore-appstream)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appstream/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-appstream?color=blue)](https://pypistats.org/packages/types-aiobotocore-appstream)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.AppStream 2.5.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream)
+[aiobotocore.AppStream 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-appstream-2.5.1/types_aiobotocore_appstream.egg-info/SOURCES.txt` & `types-aiobotocore-appstream-2.5.2/types_aiobotocore_appstream.egg-info/SOURCES.txt`

 * *Files identical despite different names*

