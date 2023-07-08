# Comparing `tmp/types-aiobotocore-budgets-2.5.1.tar.gz` & `tmp/types-aiobotocore-budgets-2.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-budgets-2.5.1.tar", last modified: Wed Jun 28 01:43:10 2023, max compression
+gzip compressed data, was "types-aiobotocore-budgets-2.5.2.tar", last modified: Sat Jul  8 01:43:18 2023, max compression
```

## Comparing `types-aiobotocore-budgets-2.5.1.tar` & `types-aiobotocore-budgets-2.5.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 01:43:10.978103 types-aiobotocore-budgets-2.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-28 01:26:51.000000 types-aiobotocore-budgets-2.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18074 2023-06-28 01:43:10.974102 types-aiobotocore-budgets-2.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16509 2023-06-28 01:26:51.000000 types-aiobotocore-budgets-2.5.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-28 01:43:10.978103 types-aiobotocore-budgets-2.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-06-28 01:26:51.000000 types-aiobotocore-budgets-2.5.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 01:43:10.974102 types-aiobotocore-budgets-2.5.1/types_aiobotocore_budgets/
--rw-r--r--   0 runner    (1001) docker     (123)     2791 2023-06-28 01:26:51.000000 types-aiobotocore-budgets-2.5.1/types_aiobotocore_budgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-06-28 01:26:51.000000 types-aiobotocore-budgets-2.5.1/types_aiobotocore_budgets/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-06-28 01:26:51.000000 types-aiobotocore-budgets-2.5.1/types_aiobotocore_budgets/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23639 2023-06-28 01:26:51.000000 types-aiobotocore-budgets-2.5.1/types_aiobotocore_budgets/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    23599 2023-06-28 01:26:51.000000 types-aiobotocore-budgets-2.5.1/types_aiobotocore_budgets/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10657 2023-06-28 01:26:51.000000 types-aiobotocore-budgets-2.5.1/types_aiobotocore_budgets/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10655 2023-06-28 01:26:51.000000 types-aiobotocore-budgets-2.5.1/types_aiobotocore_budgets/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11479 2023-06-28 01:26:51.000000 types-aiobotocore-budgets-2.5.1/types_aiobotocore_budgets/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    11469 2023-06-28 01:26:51.000000 types-aiobotocore-budgets-2.5.1/types_aiobotocore_budgets/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 01:26:51.000000 types-aiobotocore-budgets-2.5.1/types_aiobotocore_budgets/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    31392 2023-06-28 01:26:52.000000 types-aiobotocore-budgets-2.5.1/types_aiobotocore_budgets/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    31343 2023-06-28 01:26:52.000000 types-aiobotocore-budgets-2.5.1/types_aiobotocore_budgets/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-28 01:26:51.000000 types-aiobotocore-budgets-2.5.1/types_aiobotocore_budgets/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 01:43:10.974102 types-aiobotocore-budgets-2.5.1/types_aiobotocore_budgets.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18074 2023-06-28 01:43:10.000000 types-aiobotocore-budgets-2.5.1/types_aiobotocore_budgets.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-06-28 01:43:10.000000 types-aiobotocore-budgets-2.5.1/types_aiobotocore_budgets.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 01:43:10.000000 types-aiobotocore-budgets-2.5.1/types_aiobotocore_budgets.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 01:43:10.000000 types-aiobotocore-budgets-2.5.1/types_aiobotocore_budgets.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-28 01:43:10.000000 types-aiobotocore-budgets-2.5.1/types_aiobotocore_budgets.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-28 01:43:10.000000 types-aiobotocore-budgets-2.5.1/types_aiobotocore_budgets.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:18.941776 types-aiobotocore-budgets-2.5.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:26:26.000000 types-aiobotocore-budgets-2.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18074 2023-07-08 01:43:18.937776 types-aiobotocore-budgets-2.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16509 2023-07-08 01:26:26.000000 types-aiobotocore-budgets-2.5.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:43:18.941776 types-aiobotocore-budgets-2.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-07-08 01:26:26.000000 types-aiobotocore-budgets-2.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:18.933776 types-aiobotocore-budgets-2.5.2/types_aiobotocore_budgets/
+-rw-r--r--   0 runner    (1001) docker     (123)     2791 2023-07-08 01:26:26.000000 types-aiobotocore-budgets-2.5.2/types_aiobotocore_budgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-07-08 01:26:26.000000 types-aiobotocore-budgets-2.5.2/types_aiobotocore_budgets/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-07-08 01:26:26.000000 types-aiobotocore-budgets-2.5.2/types_aiobotocore_budgets/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23639 2023-07-08 01:26:26.000000 types-aiobotocore-budgets-2.5.2/types_aiobotocore_budgets/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23599 2023-07-08 01:26:26.000000 types-aiobotocore-budgets-2.5.2/types_aiobotocore_budgets/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10657 2023-07-08 01:26:27.000000 types-aiobotocore-budgets-2.5.2/types_aiobotocore_budgets/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10655 2023-07-08 01:26:27.000000 types-aiobotocore-budgets-2.5.2/types_aiobotocore_budgets/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11479 2023-07-08 01:26:27.000000 types-aiobotocore-budgets-2.5.2/types_aiobotocore_budgets/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11469 2023-07-08 01:26:27.000000 types-aiobotocore-budgets-2.5.2/types_aiobotocore_budgets/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:26:26.000000 types-aiobotocore-budgets-2.5.2/types_aiobotocore_budgets/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    31392 2023-07-08 01:26:27.000000 types-aiobotocore-budgets-2.5.2/types_aiobotocore_budgets/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31343 2023-07-08 01:26:27.000000 types-aiobotocore-budgets-2.5.2/types_aiobotocore_budgets/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:26:26.000000 types-aiobotocore-budgets-2.5.2/types_aiobotocore_budgets/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:18.937776 types-aiobotocore-budgets-2.5.2/types_aiobotocore_budgets.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18074 2023-07-08 01:43:18.000000 types-aiobotocore-budgets-2.5.2/types_aiobotocore_budgets.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-08 01:43:18.000000 types-aiobotocore-budgets-2.5.2/types_aiobotocore_budgets.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:18.000000 types-aiobotocore-budgets-2.5.2/types_aiobotocore_budgets.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:18.000000 types-aiobotocore-budgets-2.5.2/types_aiobotocore_budgets.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:43:18.000000 types-aiobotocore-budgets-2.5.2/types_aiobotocore_budgets.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-08 01:43:18.000000 types-aiobotocore-budgets-2.5.2/types_aiobotocore_budgets.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-budgets-2.5.1/LICENSE` & `types-aiobotocore-budgets-2.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-budgets-2.5.1/PKG-INFO` & `types-aiobotocore-budgets-2.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-budgets
-Version: 2.5.1
-Summary: Type annotations for aiobotocore.Budgets 2.5.1 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2
+Summary: Type annotations for aiobotocore.Budgets 2.5.2 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_budgets/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-budgets.svg?color=blue)](https://pypi.org/project/types-aiobotocore-budgets)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_budgets/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-budgets?color=blue)](https://pypistats.org/packages/types-aiobotocore-budgets)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Budgets 2.5.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets)
+[aiobotocore.Budgets 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-budgets-2.5.1/README.md` & `types-aiobotocore-budgets-2.5.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-budgets.svg?color=blue)](https://pypi.org/project/types-aiobotocore-budgets)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_budgets/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-budgets?color=blue)](https://pypistats.org/packages/types-aiobotocore-budgets)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Budgets 2.5.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets)
+[aiobotocore.Budgets 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-budgets-2.5.1/setup.py` & `types-aiobotocore-budgets-2.5.2/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-budgets",
-    version="2.5.1",
+    version="2.5.2",
     packages=["types_aiobotocore_budgets"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.Budgets 2.5.1 service generated with mypy-boto3-builder"
+        "Type annotations for aiobotocore.Budgets 2.5.2 service generated with mypy-boto3-builder"
         " 7.14.5"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-budgets-2.5.1/types_aiobotocore_budgets/__init__.py` & `types-aiobotocore-budgets-2.5.2/types_aiobotocore_budgets/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-budgets-2.5.1/types_aiobotocore_budgets/__init__.pyi` & `types-aiobotocore-budgets-2.5.2/types_aiobotocore_budgets/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-budgets-2.5.1/types_aiobotocore_budgets/__main__.py` & `types-aiobotocore-budgets-2.5.2/types_aiobotocore_budgets/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.Budgets 2.5.1\nVersion:         2.5.1\nBuilder version:"
+        "Type annotations for aiobotocore.Budgets 2.5.2\nVersion:         2.5.2\nBuilder version:"
         " 7.14.5\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_budgets//\nBoto3 docs:"
         "     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets\nOther"
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

### Comparing `types-aiobotocore-budgets-2.5.1/types_aiobotocore_budgets/client.py` & `types-aiobotocore-budgets-2.5.2/types_aiobotocore_budgets/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-budgets-2.5.1/types_aiobotocore_budgets/client.pyi` & `types-aiobotocore-budgets-2.5.2/types_aiobotocore_budgets/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-budgets-2.5.1/types_aiobotocore_budgets/literals.py` & `types-aiobotocore-budgets-2.5.2/types_aiobotocore_budgets/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-budgets-2.5.1/types_aiobotocore_budgets/literals.pyi` & `types-aiobotocore-budgets-2.5.2/types_aiobotocore_budgets/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-budgets-2.5.1/types_aiobotocore_budgets/paginator.py` & `types-aiobotocore-budgets-2.5.2/types_aiobotocore_budgets/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-budgets-2.5.1/types_aiobotocore_budgets/paginator.pyi` & `types-aiobotocore-budgets-2.5.2/types_aiobotocore_budgets/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-budgets-2.5.1/types_aiobotocore_budgets/type_defs.py` & `types-aiobotocore-budgets-2.5.2/types_aiobotocore_budgets/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-budgets-2.5.1/types_aiobotocore_budgets/type_defs.pyi` & `types-aiobotocore-budgets-2.5.2/types_aiobotocore_budgets/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-budgets-2.5.1/types_aiobotocore_budgets.egg-info/PKG-INFO` & `types-aiobotocore-budgets-2.5.2/types_aiobotocore_budgets.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-budgets
-Version: 2.5.1
-Summary: Type annotations for aiobotocore.Budgets 2.5.1 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2
+Summary: Type annotations for aiobotocore.Budgets 2.5.2 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_budgets/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-budgets.svg?color=blue)](https://pypi.org/project/types-aiobotocore-budgets)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_budgets/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-budgets?color=blue)](https://pypistats.org/packages/types-aiobotocore-budgets)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Budgets 2.5.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets)
+[aiobotocore.Budgets 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-budgets-2.5.1/types_aiobotocore_budgets.egg-info/SOURCES.txt` & `types-aiobotocore-budgets-2.5.2/types_aiobotocore_budgets.egg-info/SOURCES.txt`

 * *Files identical despite different names*

