# Comparing `tmp/types-aiobotocore-appflow-2.5.1.tar.gz` & `tmp/types-aiobotocore-appflow-2.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-appflow-2.5.1.tar", last modified: Wed Jun 28 01:43:04 2023, max compression
+gzip compressed data, was "types-aiobotocore-appflow-2.5.2.tar", last modified: Sat Jul  8 01:43:12 2023, max compression
```

## Comparing `types-aiobotocore-appflow-2.5.1.tar` & `types-aiobotocore-appflow-2.5.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 01:43:04.262090 types-aiobotocore-appflow-2.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-28 01:26:08.000000 types-aiobotocore-appflow-2.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    19966 2023-06-28 01:43:04.262090 types-aiobotocore-appflow-2.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    18401 2023-06-28 01:26:08.000000 types-aiobotocore-appflow-2.5.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-28 01:43:04.262090 types-aiobotocore-appflow-2.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-06-28 01:26:08.000000 types-aiobotocore-appflow-2.5.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 01:43:04.262090 types-aiobotocore-appflow-2.5.1/types_aiobotocore_appflow/
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-06-28 01:26:08.000000 types-aiobotocore-appflow-2.5.1/types_aiobotocore_appflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-06-28 01:26:08.000000 types-aiobotocore-appflow-2.5.1/types_aiobotocore_appflow/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-06-28 01:26:08.000000 types-aiobotocore-appflow-2.5.1/types_aiobotocore_appflow/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21145 2023-06-28 01:26:09.000000 types-aiobotocore-appflow-2.5.1/types_aiobotocore_appflow/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    21111 2023-06-28 01:26:09.000000 types-aiobotocore-appflow-2.5.1/types_aiobotocore_appflow/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    18362 2023-06-28 01:26:09.000000 types-aiobotocore-appflow-2.5.1/types_aiobotocore_appflow/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    18360 2023-06-28 01:26:09.000000 types-aiobotocore-appflow-2.5.1/types_aiobotocore_appflow/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 01:26:08.000000 types-aiobotocore-appflow-2.5.1/types_aiobotocore_appflow/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    71147 2023-06-28 01:26:10.000000 types-aiobotocore-appflow-2.5.1/types_aiobotocore_appflow/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    71045 2023-06-28 01:26:10.000000 types-aiobotocore-appflow-2.5.1/types_aiobotocore_appflow/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-28 01:26:08.000000 types-aiobotocore-appflow-2.5.1/types_aiobotocore_appflow/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 01:43:04.262090 types-aiobotocore-appflow-2.5.1/types_aiobotocore_appflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19966 2023-06-28 01:43:04.000000 types-aiobotocore-appflow-2.5.1/types_aiobotocore_appflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-06-28 01:43:04.000000 types-aiobotocore-appflow-2.5.1/types_aiobotocore_appflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 01:43:04.000000 types-aiobotocore-appflow-2.5.1/types_aiobotocore_appflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 01:43:04.000000 types-aiobotocore-appflow-2.5.1/types_aiobotocore_appflow.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-28 01:43:04.000000 types-aiobotocore-appflow-2.5.1/types_aiobotocore_appflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-28 01:43:04.000000 types-aiobotocore-appflow-2.5.1/types_aiobotocore_appflow.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:12.369652 types-aiobotocore-appflow-2.5.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:25:43.000000 types-aiobotocore-appflow-2.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    19966 2023-07-08 01:43:12.369652 types-aiobotocore-appflow-2.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    18401 2023-07-08 01:25:43.000000 types-aiobotocore-appflow-2.5.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:43:12.389653 types-aiobotocore-appflow-2.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-07-08 01:25:43.000000 types-aiobotocore-appflow-2.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:12.369652 types-aiobotocore-appflow-2.5.2/types_aiobotocore_appflow/
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-07-08 01:25:43.000000 types-aiobotocore-appflow-2.5.2/types_aiobotocore_appflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-07-08 01:25:43.000000 types-aiobotocore-appflow-2.5.2/types_aiobotocore_appflow/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-07-08 01:25:43.000000 types-aiobotocore-appflow-2.5.2/types_aiobotocore_appflow/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21145 2023-07-08 01:25:43.000000 types-aiobotocore-appflow-2.5.2/types_aiobotocore_appflow/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21111 2023-07-08 01:25:43.000000 types-aiobotocore-appflow-2.5.2/types_aiobotocore_appflow/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    18362 2023-07-08 01:25:43.000000 types-aiobotocore-appflow-2.5.2/types_aiobotocore_appflow/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18360 2023-07-08 01:25:43.000000 types-aiobotocore-appflow-2.5.2/types_aiobotocore_appflow/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:25:43.000000 types-aiobotocore-appflow-2.5.2/types_aiobotocore_appflow/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    71147 2023-07-08 01:25:45.000000 types-aiobotocore-appflow-2.5.2/types_aiobotocore_appflow/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71045 2023-07-08 01:25:44.000000 types-aiobotocore-appflow-2.5.2/types_aiobotocore_appflow/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:25:43.000000 types-aiobotocore-appflow-2.5.2/types_aiobotocore_appflow/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:12.369652 types-aiobotocore-appflow-2.5.2/types_aiobotocore_appflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19966 2023-07-08 01:43:12.000000 types-aiobotocore-appflow-2.5.2/types_aiobotocore_appflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-07-08 01:43:12.000000 types-aiobotocore-appflow-2.5.2/types_aiobotocore_appflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:12.000000 types-aiobotocore-appflow-2.5.2/types_aiobotocore_appflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:12.000000 types-aiobotocore-appflow-2.5.2/types_aiobotocore_appflow.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:43:12.000000 types-aiobotocore-appflow-2.5.2/types_aiobotocore_appflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-08 01:43:12.000000 types-aiobotocore-appflow-2.5.2/types_aiobotocore_appflow.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-appflow-2.5.1/LICENSE` & `types-aiobotocore-appflow-2.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-appflow-2.5.1/PKG-INFO` & `types-aiobotocore-appflow-2.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-appflow
-Version: 2.5.1
-Summary: Type annotations for aiobotocore.Appflow 2.5.1 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2
+Summary: Type annotations for aiobotocore.Appflow 2.5.2 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appflow/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-appflow.svg?color=blue)](https://pypi.org/project/types-aiobotocore-appflow)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appflow/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-appflow?color=blue)](https://pypistats.org/packages/types-aiobotocore-appflow)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Appflow 2.5.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow)
+[aiobotocore.Appflow 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-appflow-2.5.1/README.md` & `types-aiobotocore-appflow-2.5.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-appflow.svg?color=blue)](https://pypi.org/project/types-aiobotocore-appflow)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appflow/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-appflow?color=blue)](https://pypistats.org/packages/types-aiobotocore-appflow)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Appflow 2.5.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow)
+[aiobotocore.Appflow 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-appflow-2.5.1/setup.py` & `types-aiobotocore-appflow-2.5.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-appflow",
-    version="2.5.1",
+    version="2.5.2",
     packages=["types_aiobotocore_appflow"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.Appflow 2.5.1 service generated with mypy-boto3-builder"
+        "Type annotations for aiobotocore.Appflow 2.5.2 service generated with mypy-boto3-builder"
         " 7.14.5"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-appflow-2.5.1/types_aiobotocore_appflow/__main__.py` & `types-aiobotocore-appflow-2.5.2/types_aiobotocore_appflow/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.Appflow 2.5.1\nVersion:         2.5.1\nBuilder version:"
+        "Type annotations for aiobotocore.Appflow 2.5.2\nVersion:         2.5.2\nBuilder version:"
         " 7.14.5\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appflow//\nBoto3 docs:"
         "     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow\nOther"
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

### Comparing `types-aiobotocore-appflow-2.5.1/types_aiobotocore_appflow/client.py` & `types-aiobotocore-appflow-2.5.2/types_aiobotocore_appflow/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-appflow-2.5.1/types_aiobotocore_appflow/client.pyi` & `types-aiobotocore-appflow-2.5.2/types_aiobotocore_appflow/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-appflow-2.5.1/types_aiobotocore_appflow/literals.py` & `types-aiobotocore-appflow-2.5.2/types_aiobotocore_appflow/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-appflow-2.5.1/types_aiobotocore_appflow/literals.pyi` & `types-aiobotocore-appflow-2.5.2/types_aiobotocore_appflow/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-appflow-2.5.1/types_aiobotocore_appflow/type_defs.py` & `types-aiobotocore-appflow-2.5.2/types_aiobotocore_appflow/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-appflow-2.5.1/types_aiobotocore_appflow/type_defs.pyi` & `types-aiobotocore-appflow-2.5.2/types_aiobotocore_appflow/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-appflow-2.5.1/types_aiobotocore_appflow.egg-info/PKG-INFO` & `types-aiobotocore-appflow-2.5.2/types_aiobotocore_appflow.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-appflow
-Version: 2.5.1
-Summary: Type annotations for aiobotocore.Appflow 2.5.1 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2
+Summary: Type annotations for aiobotocore.Appflow 2.5.2 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appflow/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-appflow.svg?color=blue)](https://pypi.org/project/types-aiobotocore-appflow)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appflow/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-appflow?color=blue)](https://pypistats.org/packages/types-aiobotocore-appflow)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Appflow 2.5.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow)
+[aiobotocore.Appflow 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-appflow-2.5.1/types_aiobotocore_appflow.egg-info/SOURCES.txt` & `types-aiobotocore-appflow-2.5.2/types_aiobotocore_appflow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

