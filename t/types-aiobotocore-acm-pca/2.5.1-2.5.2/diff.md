# Comparing `tmp/types-aiobotocore-acm-pca-2.5.1.tar.gz` & `tmp/types-aiobotocore-acm-pca-2.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-acm-pca-2.5.1.tar", last modified: Wed Jun 28 01:43:01 2023, max compression
+gzip compressed data, was "types-aiobotocore-acm-pca-2.5.2.tar", last modified: Sat Jul  8 01:43:09 2023, max compression
```

## Comparing `types-aiobotocore-acm-pca-2.5.1.tar` & `types-aiobotocore-acm-pca-2.5.2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 01:43:01.682085 types-aiobotocore-acm-pca-2.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-28 01:25:43.000000 types-aiobotocore-acm-pca-2.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    17633 2023-06-28 01:43:01.682085 types-aiobotocore-acm-pca-2.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16069 2023-06-28 01:25:43.000000 types-aiobotocore-acm-pca-2.5.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-28 01:43:01.682085 types-aiobotocore-acm-pca-2.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-06-28 01:25:43.000000 types-aiobotocore-acm-pca-2.5.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 01:43:01.678085 types-aiobotocore-acm-pca-2.5.1/types_aiobotocore_acm_pca/
--rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-06-28 01:25:43.000000 types-aiobotocore-acm-pca-2.5.1/types_aiobotocore_acm_pca/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-06-28 01:25:43.000000 types-aiobotocore-acm-pca-2.5.1/types_aiobotocore_acm_pca/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-06-28 01:25:43.000000 types-aiobotocore-acm-pca-2.5.1/types_aiobotocore_acm_pca/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24003 2023-06-28 01:25:43.000000 types-aiobotocore-acm-pca-2.5.1/types_aiobotocore_acm_pca/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    23965 2023-06-28 01:25:43.000000 types-aiobotocore-acm-pca-2.5.1/types_aiobotocore_acm_pca/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11219 2023-06-28 01:25:43.000000 types-aiobotocore-acm-pca-2.5.1/types_aiobotocore_acm_pca/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    11217 2023-06-28 01:25:43.000000 types-aiobotocore-acm-pca-2.5.1/types_aiobotocore_acm_pca/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4341 2023-06-28 01:25:43.000000 types-aiobotocore-acm-pca-2.5.1/types_aiobotocore_acm_pca/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4336 2023-06-28 01:25:43.000000 types-aiobotocore-acm-pca-2.5.1/types_aiobotocore_acm_pca/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 01:25:43.000000 types-aiobotocore-acm-pca-2.5.1/types_aiobotocore_acm_pca/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    27365 2023-06-28 01:25:44.000000 types-aiobotocore-acm-pca-2.5.1/types_aiobotocore_acm_pca/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    27322 2023-06-28 01:25:43.000000 types-aiobotocore-acm-pca-2.5.1/types_aiobotocore_acm_pca/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-28 01:25:43.000000 types-aiobotocore-acm-pca-2.5.1/types_aiobotocore_acm_pca/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3816 2023-06-28 01:25:43.000000 types-aiobotocore-acm-pca-2.5.1/types_aiobotocore_acm_pca/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3813 2023-06-28 01:25:43.000000 types-aiobotocore-acm-pca-2.5.1/types_aiobotocore_acm_pca/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 01:43:01.682085 types-aiobotocore-acm-pca-2.5.1/types_aiobotocore_acm_pca.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17633 2023-06-28 01:43:01.000000 types-aiobotocore-acm-pca-2.5.1/types_aiobotocore_acm_pca.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-06-28 01:43:01.000000 types-aiobotocore-acm-pca-2.5.1/types_aiobotocore_acm_pca.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 01:43:01.000000 types-aiobotocore-acm-pca-2.5.1/types_aiobotocore_acm_pca.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 01:43:01.000000 types-aiobotocore-acm-pca-2.5.1/types_aiobotocore_acm_pca.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-28 01:43:01.000000 types-aiobotocore-acm-pca-2.5.1/types_aiobotocore_acm_pca.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-28 01:43:01.000000 types-aiobotocore-acm-pca-2.5.1/types_aiobotocore_acm_pca.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:09.829605 types-aiobotocore-acm-pca-2.5.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:25:16.000000 types-aiobotocore-acm-pca-2.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    17633 2023-07-08 01:43:09.829605 types-aiobotocore-acm-pca-2.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16069 2023-07-08 01:25:16.000000 types-aiobotocore-acm-pca-2.5.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:43:09.829605 types-aiobotocore-acm-pca-2.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-07-08 01:25:16.000000 types-aiobotocore-acm-pca-2.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:09.829605 types-aiobotocore-acm-pca-2.5.2/types_aiobotocore_acm_pca/
+-rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-07-08 01:25:16.000000 types-aiobotocore-acm-pca-2.5.2/types_aiobotocore_acm_pca/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-07-08 01:25:16.000000 types-aiobotocore-acm-pca-2.5.2/types_aiobotocore_acm_pca/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-07-08 01:25:16.000000 types-aiobotocore-acm-pca-2.5.2/types_aiobotocore_acm_pca/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24003 2023-07-08 01:25:17.000000 types-aiobotocore-acm-pca-2.5.2/types_aiobotocore_acm_pca/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23965 2023-07-08 01:25:16.000000 types-aiobotocore-acm-pca-2.5.2/types_aiobotocore_acm_pca/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11219 2023-07-08 01:25:17.000000 types-aiobotocore-acm-pca-2.5.2/types_aiobotocore_acm_pca/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11217 2023-07-08 01:25:17.000000 types-aiobotocore-acm-pca-2.5.2/types_aiobotocore_acm_pca/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4341 2023-07-08 01:25:17.000000 types-aiobotocore-acm-pca-2.5.2/types_aiobotocore_acm_pca/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4336 2023-07-08 01:25:17.000000 types-aiobotocore-acm-pca-2.5.2/types_aiobotocore_acm_pca/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:25:16.000000 types-aiobotocore-acm-pca-2.5.2/types_aiobotocore_acm_pca/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    27365 2023-07-08 01:25:17.000000 types-aiobotocore-acm-pca-2.5.2/types_aiobotocore_acm_pca/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27322 2023-07-08 01:25:17.000000 types-aiobotocore-acm-pca-2.5.2/types_aiobotocore_acm_pca/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:25:16.000000 types-aiobotocore-acm-pca-2.5.2/types_aiobotocore_acm_pca/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3816 2023-07-08 01:25:17.000000 types-aiobotocore-acm-pca-2.5.2/types_aiobotocore_acm_pca/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3813 2023-07-08 01:25:17.000000 types-aiobotocore-acm-pca-2.5.2/types_aiobotocore_acm_pca/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:09.829605 types-aiobotocore-acm-pca-2.5.2/types_aiobotocore_acm_pca.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17633 2023-07-08 01:43:09.000000 types-aiobotocore-acm-pca-2.5.2/types_aiobotocore_acm_pca.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-07-08 01:43:09.000000 types-aiobotocore-acm-pca-2.5.2/types_aiobotocore_acm_pca.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:09.000000 types-aiobotocore-acm-pca-2.5.2/types_aiobotocore_acm_pca.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:09.000000 types-aiobotocore-acm-pca-2.5.2/types_aiobotocore_acm_pca.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:43:09.000000 types-aiobotocore-acm-pca-2.5.2/types_aiobotocore_acm_pca.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-08 01:43:09.000000 types-aiobotocore-acm-pca-2.5.2/types_aiobotocore_acm_pca.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-acm-pca-2.5.1/LICENSE` & `types-aiobotocore-acm-pca-2.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-acm-pca-2.5.1/PKG-INFO` & `types-aiobotocore-acm-pca-2.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-acm-pca
-Version: 2.5.1
-Summary: Type annotations for aiobotocore.ACMPCA 2.5.1 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2
+Summary: Type annotations for aiobotocore.ACMPCA 2.5.2 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_acm_pca/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-acm-pca.svg?color=blue)](https://pypi.org/project/types-aiobotocore-acm-pca)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_acm_pca/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-acm-pca?color=blue)](https://pypistats.org/packages/types-aiobotocore-acm-pca)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ACMPCA 2.5.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm-pca.html#ACMPCA)
+[aiobotocore.ACMPCA 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm-pca.html#ACMPCA)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-acm-pca-2.5.1/README.md` & `types-aiobotocore-acm-pca-2.5.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-acm-pca.svg?color=blue)](https://pypi.org/project/types-aiobotocore-acm-pca)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_acm_pca/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-acm-pca?color=blue)](https://pypistats.org/packages/types-aiobotocore-acm-pca)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ACMPCA 2.5.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm-pca.html#ACMPCA)
+[aiobotocore.ACMPCA 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm-pca.html#ACMPCA)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-acm-pca-2.5.1/setup.py` & `types-aiobotocore-acm-pca-2.5.2/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-acm-pca",
-    version="2.5.1",
+    version="2.5.2",
     packages=["types_aiobotocore_acm_pca"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.ACMPCA 2.5.1 service generated with mypy-boto3-builder"
+        "Type annotations for aiobotocore.ACMPCA 2.5.2 service generated with mypy-boto3-builder"
         " 7.14.5"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-acm-pca-2.5.1/types_aiobotocore_acm_pca/__init__.py` & `types-aiobotocore-acm-pca-2.5.2/types_aiobotocore_acm_pca/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-acm-pca-2.5.1/types_aiobotocore_acm_pca/__init__.pyi` & `types-aiobotocore-acm-pca-2.5.2/types_aiobotocore_acm_pca/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-acm-pca-2.5.1/types_aiobotocore_acm_pca/__main__.py` & `types-aiobotocore-acm-pca-2.5.2/types_aiobotocore_acm_pca/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.ACMPCA 2.5.1\nVersion:         2.5.1\nBuilder version:"
+        "Type annotations for aiobotocore.ACMPCA 2.5.2\nVersion:         2.5.2\nBuilder version:"
         " 7.14.5\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_acm_pca//\nBoto3 docs:"
         "     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm-pca.html#ACMPCA\nOther"
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

### Comparing `types-aiobotocore-acm-pca-2.5.1/types_aiobotocore_acm_pca/client.py` & `types-aiobotocore-acm-pca-2.5.2/types_aiobotocore_acm_pca/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-acm-pca-2.5.1/types_aiobotocore_acm_pca/client.pyi` & `types-aiobotocore-acm-pca-2.5.2/types_aiobotocore_acm_pca/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-acm-pca-2.5.1/types_aiobotocore_acm_pca/literals.py` & `types-aiobotocore-acm-pca-2.5.2/types_aiobotocore_acm_pca/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-acm-pca-2.5.1/types_aiobotocore_acm_pca/literals.pyi` & `types-aiobotocore-acm-pca-2.5.2/types_aiobotocore_acm_pca/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-acm-pca-2.5.1/types_aiobotocore_acm_pca/paginator.py` & `types-aiobotocore-acm-pca-2.5.2/types_aiobotocore_acm_pca/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-acm-pca-2.5.1/types_aiobotocore_acm_pca/paginator.pyi` & `types-aiobotocore-acm-pca-2.5.2/types_aiobotocore_acm_pca/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-acm-pca-2.5.1/types_aiobotocore_acm_pca/type_defs.py` & `types-aiobotocore-acm-pca-2.5.2/types_aiobotocore_acm_pca/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-acm-pca-2.5.1/types_aiobotocore_acm_pca/type_defs.pyi` & `types-aiobotocore-acm-pca-2.5.2/types_aiobotocore_acm_pca/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-acm-pca-2.5.1/types_aiobotocore_acm_pca/waiter.py` & `types-aiobotocore-acm-pca-2.5.2/types_aiobotocore_acm_pca/waiter.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-acm-pca-2.5.1/types_aiobotocore_acm_pca/waiter.pyi` & `types-aiobotocore-acm-pca-2.5.2/types_aiobotocore_acm_pca/waiter.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-acm-pca-2.5.1/types_aiobotocore_acm_pca.egg-info/PKG-INFO` & `types-aiobotocore-acm-pca-2.5.2/types_aiobotocore_acm_pca.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-acm-pca
-Version: 2.5.1
-Summary: Type annotations for aiobotocore.ACMPCA 2.5.1 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2
+Summary: Type annotations for aiobotocore.ACMPCA 2.5.2 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_acm_pca/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-acm-pca.svg?color=blue)](https://pypi.org/project/types-aiobotocore-acm-pca)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_acm_pca/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-acm-pca?color=blue)](https://pypistats.org/packages/types-aiobotocore-acm-pca)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ACMPCA 2.5.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm-pca.html#ACMPCA)
+[aiobotocore.ACMPCA 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm-pca.html#ACMPCA)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-acm-pca-2.5.1/types_aiobotocore_acm_pca.egg-info/SOURCES.txt` & `types-aiobotocore-acm-pca-2.5.2/types_aiobotocore_acm_pca.egg-info/SOURCES.txt`

 * *Files identical despite different names*

