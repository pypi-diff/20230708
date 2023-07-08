# Comparing `tmp/types-aiobotocore-docdb-elastic-2.5.1.tar.gz` & `tmp/types-aiobotocore-docdb-elastic-2.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-docdb-elastic-2.5.1.tar", last modified: Wed Jun 28 01:43:24 2023, max compression
+gzip compressed data, was "types-aiobotocore-docdb-elastic-2.5.2.tar", last modified: Sat Jul  8 01:43:32 2023, max compression
```

## Comparing `types-aiobotocore-docdb-elastic-2.5.1.tar` & `types-aiobotocore-docdb-elastic-2.5.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 01:43:24.222127 types-aiobotocore-docdb-elastic-2.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-28 01:29:19.000000 types-aiobotocore-docdb-elastic-2.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14529 2023-06-28 01:43:24.222127 types-aiobotocore-docdb-elastic-2.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12941 2023-06-28 01:29:19.000000 types-aiobotocore-docdb-elastic-2.5.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-28 01:43:24.222127 types-aiobotocore-docdb-elastic-2.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-06-28 01:29:19.000000 types-aiobotocore-docdb-elastic-2.5.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 01:43:24.222127 types-aiobotocore-docdb-elastic-2.5.1/types_aiobotocore_docdb_elastic/
--rw-r--r--   0 runner    (1001) docker     (123)      898 2023-06-28 01:29:19.000000 types-aiobotocore-docdb-elastic-2.5.1/types_aiobotocore_docdb_elastic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      897 2023-06-28 01:29:19.000000 types-aiobotocore-docdb-elastic-2.5.1/types_aiobotocore_docdb_elastic/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-06-28 01:29:19.000000 types-aiobotocore-docdb-elastic-2.5.1/types_aiobotocore_docdb_elastic/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14230 2023-06-28 01:29:19.000000 types-aiobotocore-docdb-elastic-2.5.1/types_aiobotocore_docdb_elastic/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    14206 2023-06-28 01:29:19.000000 types-aiobotocore-docdb-elastic-2.5.1/types_aiobotocore_docdb_elastic/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8152 2023-06-28 01:29:20.000000 types-aiobotocore-docdb-elastic-2.5.1/types_aiobotocore_docdb_elastic/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8150 2023-06-28 01:29:19.000000 types-aiobotocore-docdb-elastic-2.5.1/types_aiobotocore_docdb_elastic/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3222 2023-06-28 01:29:19.000000 types-aiobotocore-docdb-elastic-2.5.1/types_aiobotocore_docdb_elastic/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3218 2023-06-28 01:29:19.000000 types-aiobotocore-docdb-elastic-2.5.1/types_aiobotocore_docdb_elastic/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 01:29:19.000000 types-aiobotocore-docdb-elastic-2.5.1/types_aiobotocore_docdb_elastic/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    10313 2023-06-28 01:29:21.000000 types-aiobotocore-docdb-elastic-2.5.1/types_aiobotocore_docdb_elastic/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    10304 2023-06-28 01:29:20.000000 types-aiobotocore-docdb-elastic-2.5.1/types_aiobotocore_docdb_elastic/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-28 01:29:19.000000 types-aiobotocore-docdb-elastic-2.5.1/types_aiobotocore_docdb_elastic/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 01:43:24.222127 types-aiobotocore-docdb-elastic-2.5.1/types_aiobotocore_docdb_elastic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14529 2023-06-28 01:43:24.000000 types-aiobotocore-docdb-elastic-2.5.1/types_aiobotocore_docdb_elastic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-06-28 01:43:24.000000 types-aiobotocore-docdb-elastic-2.5.1/types_aiobotocore_docdb_elastic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 01:43:24.000000 types-aiobotocore-docdb-elastic-2.5.1/types_aiobotocore_docdb_elastic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 01:43:24.000000 types-aiobotocore-docdb-elastic-2.5.1/types_aiobotocore_docdb_elastic.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-28 01:43:24.000000 types-aiobotocore-docdb-elastic-2.5.1/types_aiobotocore_docdb_elastic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-28 01:43:24.000000 types-aiobotocore-docdb-elastic-2.5.1/types_aiobotocore_docdb_elastic.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:32.266030 types-aiobotocore-docdb-elastic-2.5.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:28:58.000000 types-aiobotocore-docdb-elastic-2.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14529 2023-07-08 01:43:32.266030 types-aiobotocore-docdb-elastic-2.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12941 2023-07-08 01:28:58.000000 types-aiobotocore-docdb-elastic-2.5.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:43:32.266030 types-aiobotocore-docdb-elastic-2.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-07-08 01:28:58.000000 types-aiobotocore-docdb-elastic-2.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:32.266030 types-aiobotocore-docdb-elastic-2.5.2/types_aiobotocore_docdb_elastic/
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-07-08 01:28:58.000000 types-aiobotocore-docdb-elastic-2.5.2/types_aiobotocore_docdb_elastic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-07-08 01:28:58.000000 types-aiobotocore-docdb-elastic-2.5.2/types_aiobotocore_docdb_elastic/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-07-08 01:28:58.000000 types-aiobotocore-docdb-elastic-2.5.2/types_aiobotocore_docdb_elastic/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14230 2023-07-08 01:28:59.000000 types-aiobotocore-docdb-elastic-2.5.2/types_aiobotocore_docdb_elastic/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14206 2023-07-08 01:28:59.000000 types-aiobotocore-docdb-elastic-2.5.2/types_aiobotocore_docdb_elastic/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8152 2023-07-08 01:28:59.000000 types-aiobotocore-docdb-elastic-2.5.2/types_aiobotocore_docdb_elastic/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8150 2023-07-08 01:28:59.000000 types-aiobotocore-docdb-elastic-2.5.2/types_aiobotocore_docdb_elastic/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3222 2023-07-08 01:28:59.000000 types-aiobotocore-docdb-elastic-2.5.2/types_aiobotocore_docdb_elastic/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3218 2023-07-08 01:28:59.000000 types-aiobotocore-docdb-elastic-2.5.2/types_aiobotocore_docdb_elastic/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:28:58.000000 types-aiobotocore-docdb-elastic-2.5.2/types_aiobotocore_docdb_elastic/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    10313 2023-07-08 01:28:59.000000 types-aiobotocore-docdb-elastic-2.5.2/types_aiobotocore_docdb_elastic/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10304 2023-07-08 01:28:59.000000 types-aiobotocore-docdb-elastic-2.5.2/types_aiobotocore_docdb_elastic/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:28:58.000000 types-aiobotocore-docdb-elastic-2.5.2/types_aiobotocore_docdb_elastic/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:32.266030 types-aiobotocore-docdb-elastic-2.5.2/types_aiobotocore_docdb_elastic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14529 2023-07-08 01:43:32.000000 types-aiobotocore-docdb-elastic-2.5.2/types_aiobotocore_docdb_elastic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-08 01:43:32.000000 types-aiobotocore-docdb-elastic-2.5.2/types_aiobotocore_docdb_elastic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:32.000000 types-aiobotocore-docdb-elastic-2.5.2/types_aiobotocore_docdb_elastic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:32.000000 types-aiobotocore-docdb-elastic-2.5.2/types_aiobotocore_docdb_elastic.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:43:32.000000 types-aiobotocore-docdb-elastic-2.5.2/types_aiobotocore_docdb_elastic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-08 01:43:32.000000 types-aiobotocore-docdb-elastic-2.5.2/types_aiobotocore_docdb_elastic.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-docdb-elastic-2.5.1/LICENSE` & `types-aiobotocore-docdb-elastic-2.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-docdb-elastic-2.5.1/PKG-INFO` & `types-aiobotocore-docdb-elastic-2.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-docdb-elastic
-Version: 2.5.1
-Summary: Type annotations for aiobotocore.DocDBElastic 2.5.1 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2
+Summary: Type annotations for aiobotocore.DocDBElastic 2.5.2 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_docdb_elastic/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-docdb-elastic.svg?color=blue)](https://pypi.org/project/types-aiobotocore-docdb-elastic)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_docdb_elastic/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-docdb-elastic?color=blue)](https://pypistats.org/packages/types-aiobotocore-docdb-elastic)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.DocDBElastic 2.5.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb-elastic.html#DocDBElastic)
+[aiobotocore.DocDBElastic 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb-elastic.html#DocDBElastic)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-docdb-elastic-2.5.1/README.md` & `types-aiobotocore-docdb-elastic-2.5.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-docdb-elastic.svg?color=blue)](https://pypi.org/project/types-aiobotocore-docdb-elastic)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_docdb_elastic/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-docdb-elastic?color=blue)](https://pypistats.org/packages/types-aiobotocore-docdb-elastic)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.DocDBElastic 2.5.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb-elastic.html#DocDBElastic)
+[aiobotocore.DocDBElastic 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb-elastic.html#DocDBElastic)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-docdb-elastic-2.5.1/setup.py` & `types-aiobotocore-docdb-elastic-2.5.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-docdb-elastic",
-    version="2.5.1",
+    version="2.5.2",
     packages=["types_aiobotocore_docdb_elastic"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.DocDBElastic 2.5.1 service generated with"
+        "Type annotations for aiobotocore.DocDBElastic 2.5.2 service generated with"
         " mypy-boto3-builder 7.14.5"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-docdb-elastic-2.5.1/types_aiobotocore_docdb_elastic/__init__.py` & `types-aiobotocore-docdb-elastic-2.5.2/types_aiobotocore_docdb_elastic/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-docdb-elastic-2.5.1/types_aiobotocore_docdb_elastic/__init__.pyi` & `types-aiobotocore-docdb-elastic-2.5.2/types_aiobotocore_docdb_elastic/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-docdb-elastic-2.5.1/types_aiobotocore_docdb_elastic/__main__.py` & `types-aiobotocore-docdb-elastic-2.5.2/types_aiobotocore_docdb_elastic/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.DocDBElastic 2.5.1\nVersion:         2.5.1\nBuilder"
+        "Type annotations for aiobotocore.DocDBElastic 2.5.2\nVersion:         2.5.2\nBuilder"
         " version: 7.14.5\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_docdb_elastic//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb-elastic.html#DocDBElastic\nOther"
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

### Comparing `types-aiobotocore-docdb-elastic-2.5.1/types_aiobotocore_docdb_elastic/client.py` & `types-aiobotocore-docdb-elastic-2.5.2/types_aiobotocore_docdb_elastic/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-docdb-elastic-2.5.1/types_aiobotocore_docdb_elastic/client.pyi` & `types-aiobotocore-docdb-elastic-2.5.2/types_aiobotocore_docdb_elastic/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-docdb-elastic-2.5.1/types_aiobotocore_docdb_elastic/literals.py` & `types-aiobotocore-docdb-elastic-2.5.2/types_aiobotocore_docdb_elastic/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-docdb-elastic-2.5.1/types_aiobotocore_docdb_elastic/literals.pyi` & `types-aiobotocore-docdb-elastic-2.5.2/types_aiobotocore_docdb_elastic/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-docdb-elastic-2.5.1/types_aiobotocore_docdb_elastic/paginator.py` & `types-aiobotocore-docdb-elastic-2.5.2/types_aiobotocore_docdb_elastic/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-docdb-elastic-2.5.1/types_aiobotocore_docdb_elastic/paginator.pyi` & `types-aiobotocore-docdb-elastic-2.5.2/types_aiobotocore_docdb_elastic/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-docdb-elastic-2.5.1/types_aiobotocore_docdb_elastic/type_defs.py` & `types-aiobotocore-docdb-elastic-2.5.2/types_aiobotocore_docdb_elastic/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-docdb-elastic-2.5.1/types_aiobotocore_docdb_elastic/type_defs.pyi` & `types-aiobotocore-docdb-elastic-2.5.2/types_aiobotocore_docdb_elastic/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-docdb-elastic-2.5.1/types_aiobotocore_docdb_elastic.egg-info/PKG-INFO` & `types-aiobotocore-docdb-elastic-2.5.2/types_aiobotocore_docdb_elastic.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-docdb-elastic
-Version: 2.5.1
-Summary: Type annotations for aiobotocore.DocDBElastic 2.5.1 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2
+Summary: Type annotations for aiobotocore.DocDBElastic 2.5.2 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_docdb_elastic/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-docdb-elastic.svg?color=blue)](https://pypi.org/project/types-aiobotocore-docdb-elastic)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_docdb_elastic/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-docdb-elastic?color=blue)](https://pypistats.org/packages/types-aiobotocore-docdb-elastic)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.DocDBElastic 2.5.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb-elastic.html#DocDBElastic)
+[aiobotocore.DocDBElastic 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb-elastic.html#DocDBElastic)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-docdb-elastic-2.5.1/types_aiobotocore_docdb_elastic.egg-info/SOURCES.txt` & `types-aiobotocore-docdb-elastic-2.5.2/types_aiobotocore_docdb_elastic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

