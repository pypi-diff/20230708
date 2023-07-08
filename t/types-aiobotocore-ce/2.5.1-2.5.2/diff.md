# Comparing `tmp/types-aiobotocore-ce-2.5.1.tar.gz` & `tmp/types-aiobotocore-ce-2.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-ce-2.5.1.tar", last modified: Wed Jun 28 01:43:11 2023, max compression
+gzip compressed data, was "types-aiobotocore-ce-2.5.2.tar", last modified: Sat Jul  8 01:43:19 2023, max compression
```

## Comparing `types-aiobotocore-ce-2.5.1.tar` & `types-aiobotocore-ce-2.5.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 01:43:10.994103 types-aiobotocore-ce-2.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-28 01:26:53.000000 types-aiobotocore-ce-2.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18996 2023-06-28 01:43:10.994103 types-aiobotocore-ce-2.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17441 2023-06-28 01:26:53.000000 types-aiobotocore-ce-2.5.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-28 01:43:10.994103 types-aiobotocore-ce-2.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-06-28 01:26:53.000000 types-aiobotocore-ce-2.5.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 01:43:10.990102 types-aiobotocore-ce-2.5.1/types_aiobotocore_ce/
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-06-28 01:26:53.000000 types-aiobotocore-ce-2.5.1/types_aiobotocore_ce/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-06-28 01:26:53.000000 types-aiobotocore-ce-2.5.1/types_aiobotocore_ce/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-06-28 01:26:53.000000 types-aiobotocore-ce-2.5.1/types_aiobotocore_ce/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    33821 2023-06-28 01:26:53.000000 types-aiobotocore-ce-2.5.1/types_aiobotocore_ce/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    33775 2023-06-28 01:26:53.000000 types-aiobotocore-ce-2.5.1/types_aiobotocore_ce/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12638 2023-06-28 01:26:54.000000 types-aiobotocore-ce-2.5.1/types_aiobotocore_ce/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    12636 2023-06-28 01:26:54.000000 types-aiobotocore-ce-2.5.1/types_aiobotocore_ce/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 01:26:53.000000 types-aiobotocore-ce-2.5.1/types_aiobotocore_ce/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    63460 2023-06-28 01:26:55.000000 types-aiobotocore-ce-2.5.1/types_aiobotocore_ce/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    63391 2023-06-28 01:26:54.000000 types-aiobotocore-ce-2.5.1/types_aiobotocore_ce/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-28 01:26:53.000000 types-aiobotocore-ce-2.5.1/types_aiobotocore_ce/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 01:43:10.994103 types-aiobotocore-ce-2.5.1/types_aiobotocore_ce.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18996 2023-06-28 01:43:10.000000 types-aiobotocore-ce-2.5.1/types_aiobotocore_ce.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-06-28 01:43:10.000000 types-aiobotocore-ce-2.5.1/types_aiobotocore_ce.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 01:43:10.000000 types-aiobotocore-ce-2.5.1/types_aiobotocore_ce.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 01:43:10.000000 types-aiobotocore-ce-2.5.1/types_aiobotocore_ce.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-28 01:43:10.000000 types-aiobotocore-ce-2.5.1/types_aiobotocore_ce.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-28 01:43:10.000000 types-aiobotocore-ce-2.5.1/types_aiobotocore_ce.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:18.993777 types-aiobotocore-ce-2.5.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:26:29.000000 types-aiobotocore-ce-2.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18996 2023-07-08 01:43:18.993777 types-aiobotocore-ce-2.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17441 2023-07-08 01:26:29.000000 types-aiobotocore-ce-2.5.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:43:18.993777 types-aiobotocore-ce-2.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-07-08 01:26:29.000000 types-aiobotocore-ce-2.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:18.993777 types-aiobotocore-ce-2.5.2/types_aiobotocore_ce/
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-07-08 01:26:29.000000 types-aiobotocore-ce-2.5.2/types_aiobotocore_ce/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-07-08 01:26:29.000000 types-aiobotocore-ce-2.5.2/types_aiobotocore_ce/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-07-08 01:26:29.000000 types-aiobotocore-ce-2.5.2/types_aiobotocore_ce/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33821 2023-07-08 01:26:29.000000 types-aiobotocore-ce-2.5.2/types_aiobotocore_ce/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33775 2023-07-08 01:26:29.000000 types-aiobotocore-ce-2.5.2/types_aiobotocore_ce/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12638 2023-07-08 01:26:29.000000 types-aiobotocore-ce-2.5.2/types_aiobotocore_ce/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12636 2023-07-08 01:26:29.000000 types-aiobotocore-ce-2.5.2/types_aiobotocore_ce/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:26:29.000000 types-aiobotocore-ce-2.5.2/types_aiobotocore_ce/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    63460 2023-07-08 01:26:30.000000 types-aiobotocore-ce-2.5.2/types_aiobotocore_ce/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63391 2023-07-08 01:26:30.000000 types-aiobotocore-ce-2.5.2/types_aiobotocore_ce/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:26:29.000000 types-aiobotocore-ce-2.5.2/types_aiobotocore_ce/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:18.993777 types-aiobotocore-ce-2.5.2/types_aiobotocore_ce.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18996 2023-07-08 01:43:18.000000 types-aiobotocore-ce-2.5.2/types_aiobotocore_ce.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-07-08 01:43:18.000000 types-aiobotocore-ce-2.5.2/types_aiobotocore_ce.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:18.000000 types-aiobotocore-ce-2.5.2/types_aiobotocore_ce.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:18.000000 types-aiobotocore-ce-2.5.2/types_aiobotocore_ce.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:43:18.000000 types-aiobotocore-ce-2.5.2/types_aiobotocore_ce.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-08 01:43:18.000000 types-aiobotocore-ce-2.5.2/types_aiobotocore_ce.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-ce-2.5.1/LICENSE` & `types-aiobotocore-ce-2.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ce-2.5.1/PKG-INFO` & `types-aiobotocore-ce-2.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-ce
-Version: 2.5.1
-Summary: Type annotations for aiobotocore.CostExplorer 2.5.1 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2
+Summary: Type annotations for aiobotocore.CostExplorer 2.5.2 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ce/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-ce.svg?color=blue)](https://pypi.org/project/types-aiobotocore-ce)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ce/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-ce?color=blue)](https://pypistats.org/packages/types-aiobotocore-ce)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.CostExplorer 2.5.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer)
+[aiobotocore.CostExplorer 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-ce-2.5.1/README.md` & `types-aiobotocore-ce-2.5.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-ce.svg?color=blue)](https://pypi.org/project/types-aiobotocore-ce)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ce/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-ce?color=blue)](https://pypistats.org/packages/types-aiobotocore-ce)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.CostExplorer 2.5.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer)
+[aiobotocore.CostExplorer 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-ce-2.5.1/setup.py` & `types-aiobotocore-ce-2.5.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-ce",
-    version="2.5.1",
+    version="2.5.2",
     packages=["types_aiobotocore_ce"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.CostExplorer 2.5.1 service generated with"
+        "Type annotations for aiobotocore.CostExplorer 2.5.2 service generated with"
         " mypy-boto3-builder 7.14.5"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-ce-2.5.1/types_aiobotocore_ce/__main__.py` & `types-aiobotocore-ce-2.5.2/types_aiobotocore_ce/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.CostExplorer 2.5.1\nVersion:         2.5.1\nBuilder"
+        "Type annotations for aiobotocore.CostExplorer 2.5.2\nVersion:         2.5.2\nBuilder"
         " version: 7.14.5\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ce//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer\nOther"
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

### Comparing `types-aiobotocore-ce-2.5.1/types_aiobotocore_ce/client.py` & `types-aiobotocore-ce-2.5.2/types_aiobotocore_ce/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ce-2.5.1/types_aiobotocore_ce/client.pyi` & `types-aiobotocore-ce-2.5.2/types_aiobotocore_ce/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ce-2.5.1/types_aiobotocore_ce/literals.py` & `types-aiobotocore-ce-2.5.2/types_aiobotocore_ce/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ce-2.5.1/types_aiobotocore_ce/literals.pyi` & `types-aiobotocore-ce-2.5.2/types_aiobotocore_ce/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ce-2.5.1/types_aiobotocore_ce/type_defs.py` & `types-aiobotocore-ce-2.5.2/types_aiobotocore_ce/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ce-2.5.1/types_aiobotocore_ce/type_defs.pyi` & `types-aiobotocore-ce-2.5.2/types_aiobotocore_ce/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ce-2.5.1/types_aiobotocore_ce.egg-info/PKG-INFO` & `types-aiobotocore-ce-2.5.2/types_aiobotocore_ce.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-ce
-Version: 2.5.1
-Summary: Type annotations for aiobotocore.CostExplorer 2.5.1 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2
+Summary: Type annotations for aiobotocore.CostExplorer 2.5.2 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ce/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-ce.svg?color=blue)](https://pypi.org/project/types-aiobotocore-ce)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ce/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-ce?color=blue)](https://pypistats.org/packages/types-aiobotocore-ce)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.CostExplorer 2.5.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer)
+[aiobotocore.CostExplorer 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-ce-2.5.1/types_aiobotocore_ce.egg-info/SOURCES.txt` & `types-aiobotocore-ce-2.5.2/types_aiobotocore_ce.egg-info/SOURCES.txt`

 * *Files identical despite different names*

