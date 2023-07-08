# Comparing `tmp/types-aiobotocore-apprunner-2.5.1.tar.gz` & `tmp/types-aiobotocore-apprunner-2.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-apprunner-2.5.1.tar", last modified: Wed Jun 28 01:43:06 2023, max compression
+gzip compressed data, was "types-aiobotocore-apprunner-2.5.2.tar", last modified: Sat Jul  8 01:43:14 2023, max compression
```

## Comparing `types-aiobotocore-apprunner-2.5.1.tar` & `types-aiobotocore-apprunner-2.5.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 01:43:06.550094 types-aiobotocore-apprunner-2.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-28 01:26:20.000000 types-aiobotocore-apprunner-2.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16894 2023-06-28 01:43:06.550094 types-aiobotocore-apprunner-2.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15321 2023-06-28 01:26:20.000000 types-aiobotocore-apprunner-2.5.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-28 01:43:06.550094 types-aiobotocore-apprunner-2.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2132 2023-06-28 01:26:20.000000 types-aiobotocore-apprunner-2.5.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 01:43:06.546094 types-aiobotocore-apprunner-2.5.1/types_aiobotocore_apprunner/
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-06-28 01:26:20.000000 types-aiobotocore-apprunner-2.5.1/types_aiobotocore_apprunner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-06-28 01:26:20.000000 types-aiobotocore-apprunner-2.5.1/types_aiobotocore_apprunner/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-06-28 01:26:20.000000 types-aiobotocore-apprunner-2.5.1/types_aiobotocore_apprunner/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27528 2023-06-28 01:26:20.000000 types-aiobotocore-apprunner-2.5.1/types_aiobotocore_apprunner/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    27484 2023-06-28 01:26:20.000000 types-aiobotocore-apprunner-2.5.1/types_aiobotocore_apprunner/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10078 2023-06-28 01:26:20.000000 types-aiobotocore-apprunner-2.5.1/types_aiobotocore_apprunner/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10076 2023-06-28 01:26:20.000000 types-aiobotocore-apprunner-2.5.1/types_aiobotocore_apprunner/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 01:26:20.000000 types-aiobotocore-apprunner-2.5.1/types_aiobotocore_apprunner/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    35667 2023-06-28 01:26:21.000000 types-aiobotocore-apprunner-2.5.1/types_aiobotocore_apprunner/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    35632 2023-06-28 01:26:21.000000 types-aiobotocore-apprunner-2.5.1/types_aiobotocore_apprunner/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-28 01:26:20.000000 types-aiobotocore-apprunner-2.5.1/types_aiobotocore_apprunner/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 01:43:06.550094 types-aiobotocore-apprunner-2.5.1/types_aiobotocore_apprunner.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16894 2023-06-28 01:43:06.000000 types-aiobotocore-apprunner-2.5.1/types_aiobotocore_apprunner.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-06-28 01:43:06.000000 types-aiobotocore-apprunner-2.5.1/types_aiobotocore_apprunner.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 01:43:06.000000 types-aiobotocore-apprunner-2.5.1/types_aiobotocore_apprunner.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 01:43:06.000000 types-aiobotocore-apprunner-2.5.1/types_aiobotocore_apprunner.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-28 01:43:06.000000 types-aiobotocore-apprunner-2.5.1/types_aiobotocore_apprunner.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-28 01:43:06.000000 types-aiobotocore-apprunner-2.5.1/types_aiobotocore_apprunner.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:14.681696 types-aiobotocore-apprunner-2.5.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:25:55.000000 types-aiobotocore-apprunner-2.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16894 2023-07-08 01:43:14.677696 types-aiobotocore-apprunner-2.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15321 2023-07-08 01:25:55.000000 types-aiobotocore-apprunner-2.5.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:43:14.681696 types-aiobotocore-apprunner-2.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2132 2023-07-08 01:25:54.000000 types-aiobotocore-apprunner-2.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:14.673696 types-aiobotocore-apprunner-2.5.2/types_aiobotocore_apprunner/
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-07-08 01:25:55.000000 types-aiobotocore-apprunner-2.5.2/types_aiobotocore_apprunner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-07-08 01:25:55.000000 types-aiobotocore-apprunner-2.5.2/types_aiobotocore_apprunner/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-07-08 01:25:55.000000 types-aiobotocore-apprunner-2.5.2/types_aiobotocore_apprunner/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27528 2023-07-08 01:25:55.000000 types-aiobotocore-apprunner-2.5.2/types_aiobotocore_apprunner/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27484 2023-07-08 01:25:55.000000 types-aiobotocore-apprunner-2.5.2/types_aiobotocore_apprunner/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10078 2023-07-08 01:25:55.000000 types-aiobotocore-apprunner-2.5.2/types_aiobotocore_apprunner/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10076 2023-07-08 01:25:55.000000 types-aiobotocore-apprunner-2.5.2/types_aiobotocore_apprunner/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:25:55.000000 types-aiobotocore-apprunner-2.5.2/types_aiobotocore_apprunner/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    35667 2023-07-08 01:25:56.000000 types-aiobotocore-apprunner-2.5.2/types_aiobotocore_apprunner/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35632 2023-07-08 01:25:55.000000 types-aiobotocore-apprunner-2.5.2/types_aiobotocore_apprunner/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:25:55.000000 types-aiobotocore-apprunner-2.5.2/types_aiobotocore_apprunner/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:14.677696 types-aiobotocore-apprunner-2.5.2/types_aiobotocore_apprunner.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16894 2023-07-08 01:43:14.000000 types-aiobotocore-apprunner-2.5.2/types_aiobotocore_apprunner.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-07-08 01:43:14.000000 types-aiobotocore-apprunner-2.5.2/types_aiobotocore_apprunner.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:14.000000 types-aiobotocore-apprunner-2.5.2/types_aiobotocore_apprunner.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:14.000000 types-aiobotocore-apprunner-2.5.2/types_aiobotocore_apprunner.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:43:14.000000 types-aiobotocore-apprunner-2.5.2/types_aiobotocore_apprunner.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-08 01:43:14.000000 types-aiobotocore-apprunner-2.5.2/types_aiobotocore_apprunner.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-apprunner-2.5.1/LICENSE` & `types-aiobotocore-apprunner-2.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-apprunner-2.5.1/PKG-INFO` & `types-aiobotocore-apprunner-2.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-apprunner
-Version: 2.5.1
-Summary: Type annotations for aiobotocore.AppRunner 2.5.1 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2
+Summary: Type annotations for aiobotocore.AppRunner 2.5.2 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apprunner/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-apprunner.svg?color=blue)](https://pypi.org/project/types-aiobotocore-apprunner)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apprunner/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-apprunner?color=blue)](https://pypistats.org/packages/types-aiobotocore-apprunner)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.AppRunner 2.5.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apprunner.html#AppRunner)
+[aiobotocore.AppRunner 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apprunner.html#AppRunner)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-apprunner-2.5.1/README.md` & `types-aiobotocore-apprunner-2.5.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-apprunner.svg?color=blue)](https://pypi.org/project/types-aiobotocore-apprunner)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apprunner/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-apprunner?color=blue)](https://pypistats.org/packages/types-aiobotocore-apprunner)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.AppRunner 2.5.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apprunner.html#AppRunner)
+[aiobotocore.AppRunner 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apprunner.html#AppRunner)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-apprunner-2.5.1/setup.py` & `types-aiobotocore-apprunner-2.5.2/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-apprunner",
-    version="2.5.1",
+    version="2.5.2",
     packages=["types_aiobotocore_apprunner"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.AppRunner 2.5.1 service generated with mypy-boto3-builder"
+        "Type annotations for aiobotocore.AppRunner 2.5.2 service generated with mypy-boto3-builder"
         " 7.14.5"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-apprunner-2.5.1/types_aiobotocore_apprunner/__main__.py` & `types-aiobotocore-apprunner-2.5.2/types_aiobotocore_apprunner/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.AppRunner 2.5.1\nVersion:         2.5.1\nBuilder version:"
+        "Type annotations for aiobotocore.AppRunner 2.5.2\nVersion:         2.5.2\nBuilder version:"
         " 7.14.5\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apprunner//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apprunner.html#AppRunner\nOther"
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

### Comparing `types-aiobotocore-apprunner-2.5.1/types_aiobotocore_apprunner/client.py` & `types-aiobotocore-apprunner-2.5.2/types_aiobotocore_apprunner/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-apprunner-2.5.1/types_aiobotocore_apprunner/client.pyi` & `types-aiobotocore-apprunner-2.5.2/types_aiobotocore_apprunner/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-apprunner-2.5.1/types_aiobotocore_apprunner/literals.py` & `types-aiobotocore-apprunner-2.5.2/types_aiobotocore_apprunner/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-apprunner-2.5.1/types_aiobotocore_apprunner/literals.pyi` & `types-aiobotocore-apprunner-2.5.2/types_aiobotocore_apprunner/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-apprunner-2.5.1/types_aiobotocore_apprunner/type_defs.py` & `types-aiobotocore-apprunner-2.5.2/types_aiobotocore_apprunner/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-apprunner-2.5.1/types_aiobotocore_apprunner/type_defs.pyi` & `types-aiobotocore-apprunner-2.5.2/types_aiobotocore_apprunner/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-apprunner-2.5.1/types_aiobotocore_apprunner.egg-info/PKG-INFO` & `types-aiobotocore-apprunner-2.5.2/types_aiobotocore_apprunner.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-apprunner
-Version: 2.5.1
-Summary: Type annotations for aiobotocore.AppRunner 2.5.1 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2
+Summary: Type annotations for aiobotocore.AppRunner 2.5.2 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apprunner/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-apprunner.svg?color=blue)](https://pypi.org/project/types-aiobotocore-apprunner)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apprunner/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-apprunner?color=blue)](https://pypistats.org/packages/types-aiobotocore-apprunner)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.AppRunner 2.5.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apprunner.html#AppRunner)
+[aiobotocore.AppRunner 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apprunner.html#AppRunner)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-apprunner-2.5.1/types_aiobotocore_apprunner.egg-info/SOURCES.txt` & `types-aiobotocore-apprunner-2.5.2/types_aiobotocore_apprunner.egg-info/SOURCES.txt`

 * *Files identical despite different names*

