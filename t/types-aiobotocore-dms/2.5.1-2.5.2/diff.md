# Comparing `tmp/types-aiobotocore-dms-2.5.1.tar.gz` & `tmp/types-aiobotocore-dms-2.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-dms-2.5.1.tar", last modified: Wed Jun 28 01:43:23 2023, max compression
+gzip compressed data, was "types-aiobotocore-dms-2.5.2.tar", last modified: Sat Jul  8 01:43:32 2023, max compression
```

## Comparing `types-aiobotocore-dms-2.5.1.tar` & `types-aiobotocore-dms-2.5.2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 01:43:23.810126 types-aiobotocore-dms-2.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-28 01:29:12.000000 types-aiobotocore-dms-2.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    28954 2023-06-28 01:43:23.810126 types-aiobotocore-dms-2.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    27384 2023-06-28 01:29:12.000000 types-aiobotocore-dms-2.5.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-28 01:43:23.810126 types-aiobotocore-dms-2.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-06-28 01:29:12.000000 types-aiobotocore-dms-2.5.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 01:43:23.810126 types-aiobotocore-dms-2.5.1/types_aiobotocore_dms/
--rw-r--r--   0 runner    (1001) docker     (123)     5651 2023-06-28 01:29:12.000000 types-aiobotocore-dms-2.5.1/types_aiobotocore_dms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5650 2023-06-28 01:29:12.000000 types-aiobotocore-dms-2.5.1/types_aiobotocore_dms/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      946 2023-06-28 01:29:12.000000 types-aiobotocore-dms-2.5.1/types_aiobotocore_dms/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    69200 2023-06-28 01:29:13.000000 types-aiobotocore-dms-2.5.1/types_aiobotocore_dms/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    69101 2023-06-28 01:29:12.000000 types-aiobotocore-dms-2.5.1/types_aiobotocore_dms/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    14827 2023-06-28 01:29:14.000000 types-aiobotocore-dms-2.5.1/types_aiobotocore_dms/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    14825 2023-06-28 01:29:14.000000 types-aiobotocore-dms-2.5.1/types_aiobotocore_dms/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    17836 2023-06-28 01:29:13.000000 types-aiobotocore-dms-2.5.1/types_aiobotocore_dms/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    17820 2023-06-28 01:29:13.000000 types-aiobotocore-dms-2.5.1/types_aiobotocore_dms/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 01:29:12.000000 types-aiobotocore-dms-2.5.1/types_aiobotocore_dms/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    92980 2023-06-28 01:29:15.000000 types-aiobotocore-dms-2.5.1/types_aiobotocore_dms/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    92929 2023-06-28 01:29:15.000000 types-aiobotocore-dms-2.5.1/types_aiobotocore_dms/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-28 01:29:12.000000 types-aiobotocore-dms-2.5.1/types_aiobotocore_dms/version.py
--rw-r--r--   0 runner    (1001) docker     (123)    10058 2023-06-28 01:29:14.000000 types-aiobotocore-dms-2.5.1/types_aiobotocore_dms/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)    10050 2023-06-28 01:29:13.000000 types-aiobotocore-dms-2.5.1/types_aiobotocore_dms/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 01:43:23.810126 types-aiobotocore-dms-2.5.1/types_aiobotocore_dms.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    28954 2023-06-28 01:43:23.000000 types-aiobotocore-dms-2.5.1/types_aiobotocore_dms.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-06-28 01:43:23.000000 types-aiobotocore-dms-2.5.1/types_aiobotocore_dms.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 01:43:23.000000 types-aiobotocore-dms-2.5.1/types_aiobotocore_dms.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 01:43:23.000000 types-aiobotocore-dms-2.5.1/types_aiobotocore_dms.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-28 01:43:23.000000 types-aiobotocore-dms-2.5.1/types_aiobotocore_dms.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-28 01:43:23.000000 types-aiobotocore-dms-2.5.1/types_aiobotocore_dms.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:32.046026 types-aiobotocore-dms-2.5.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:28:51.000000 types-aiobotocore-dms-2.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    28954 2023-07-08 01:43:32.046026 types-aiobotocore-dms-2.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    27384 2023-07-08 01:28:51.000000 types-aiobotocore-dms-2.5.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:43:32.046026 types-aiobotocore-dms-2.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-07-08 01:28:51.000000 types-aiobotocore-dms-2.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:32.046026 types-aiobotocore-dms-2.5.2/types_aiobotocore_dms/
+-rw-r--r--   0 runner    (1001) docker     (123)     5651 2023-07-08 01:28:51.000000 types-aiobotocore-dms-2.5.2/types_aiobotocore_dms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5650 2023-07-08 01:28:51.000000 types-aiobotocore-dms-2.5.2/types_aiobotocore_dms/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-07-08 01:28:51.000000 types-aiobotocore-dms-2.5.2/types_aiobotocore_dms/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69200 2023-07-08 01:28:52.000000 types-aiobotocore-dms-2.5.2/types_aiobotocore_dms/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69101 2023-07-08 01:28:51.000000 types-aiobotocore-dms-2.5.2/types_aiobotocore_dms/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    14827 2023-07-08 01:28:53.000000 types-aiobotocore-dms-2.5.2/types_aiobotocore_dms/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14825 2023-07-08 01:28:53.000000 types-aiobotocore-dms-2.5.2/types_aiobotocore_dms/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    17836 2023-07-08 01:28:52.000000 types-aiobotocore-dms-2.5.2/types_aiobotocore_dms/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17820 2023-07-08 01:28:52.000000 types-aiobotocore-dms-2.5.2/types_aiobotocore_dms/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:28:51.000000 types-aiobotocore-dms-2.5.2/types_aiobotocore_dms/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    92980 2023-07-08 01:28:55.000000 types-aiobotocore-dms-2.5.2/types_aiobotocore_dms/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    92929 2023-07-08 01:28:54.000000 types-aiobotocore-dms-2.5.2/types_aiobotocore_dms/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:28:51.000000 types-aiobotocore-dms-2.5.2/types_aiobotocore_dms/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10058 2023-07-08 01:28:52.000000 types-aiobotocore-dms-2.5.2/types_aiobotocore_dms/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10050 2023-07-08 01:28:52.000000 types-aiobotocore-dms-2.5.2/types_aiobotocore_dms/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:32.046026 types-aiobotocore-dms-2.5.2/types_aiobotocore_dms.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    28954 2023-07-08 01:43:31.000000 types-aiobotocore-dms-2.5.2/types_aiobotocore_dms.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-07-08 01:43:31.000000 types-aiobotocore-dms-2.5.2/types_aiobotocore_dms.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:31.000000 types-aiobotocore-dms-2.5.2/types_aiobotocore_dms.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:31.000000 types-aiobotocore-dms-2.5.2/types_aiobotocore_dms.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:43:31.000000 types-aiobotocore-dms-2.5.2/types_aiobotocore_dms.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-08 01:43:31.000000 types-aiobotocore-dms-2.5.2/types_aiobotocore_dms.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-dms-2.5.1/LICENSE` & `types-aiobotocore-dms-2.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-dms-2.5.1/PKG-INFO` & `types-aiobotocore-dms-2.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-dms
-Version: 2.5.1
-Summary: Type annotations for aiobotocore.DatabaseMigrationService 2.5.1 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2
+Summary: Type annotations for aiobotocore.DatabaseMigrationService 2.5.2 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-dms.svg?color=blue)](https://pypi.org/project/types-aiobotocore-dms)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-dms?color=blue)](https://pypistats.org/packages/types-aiobotocore-dms)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.DatabaseMigrationService 2.5.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService)
+[aiobotocore.DatabaseMigrationService 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-dms-2.5.1/README.md` & `types-aiobotocore-dms-2.5.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-dms.svg?color=blue)](https://pypi.org/project/types-aiobotocore-dms)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-dms?color=blue)](https://pypistats.org/packages/types-aiobotocore-dms)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.DatabaseMigrationService 2.5.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService)
+[aiobotocore.DatabaseMigrationService 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-dms-2.5.1/setup.py` & `types-aiobotocore-dms-2.5.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-dms",
-    version="2.5.1",
+    version="2.5.2",
     packages=["types_aiobotocore_dms"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.DatabaseMigrationService 2.5.1 service generated with"
+        "Type annotations for aiobotocore.DatabaseMigrationService 2.5.2 service generated with"
         " mypy-boto3-builder 7.14.5"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-dms-2.5.1/types_aiobotocore_dms/__init__.py` & `types-aiobotocore-dms-2.5.2/types_aiobotocore_dms/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-dms-2.5.1/types_aiobotocore_dms/__init__.pyi` & `types-aiobotocore-dms-2.5.2/types_aiobotocore_dms/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-dms-2.5.1/types_aiobotocore_dms/__main__.py` & `types-aiobotocore-dms-2.5.2/types_aiobotocore_dms/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.DatabaseMigrationService 2.5.1\nVersion:        "
-        " 2.5.1\nBuilder version: 7.14.5\nDocs:           "
+        "Type annotations for aiobotocore.DatabaseMigrationService 2.5.2\nVersion:        "
+        " 2.5.2\nBuilder version: 7.14.5\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms//\nBoto3 docs:    "
         "  https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService\nOther"
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

### Comparing `types-aiobotocore-dms-2.5.1/types_aiobotocore_dms/client.py` & `types-aiobotocore-dms-2.5.2/types_aiobotocore_dms/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-dms-2.5.1/types_aiobotocore_dms/client.pyi` & `types-aiobotocore-dms-2.5.2/types_aiobotocore_dms/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-dms-2.5.1/types_aiobotocore_dms/literals.py` & `types-aiobotocore-dms-2.5.2/types_aiobotocore_dms/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-dms-2.5.1/types_aiobotocore_dms/literals.pyi` & `types-aiobotocore-dms-2.5.2/types_aiobotocore_dms/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-dms-2.5.1/types_aiobotocore_dms/paginator.py` & `types-aiobotocore-dms-2.5.2/types_aiobotocore_dms/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-dms-2.5.1/types_aiobotocore_dms/paginator.pyi` & `types-aiobotocore-dms-2.5.2/types_aiobotocore_dms/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-dms-2.5.1/types_aiobotocore_dms/type_defs.py` & `types-aiobotocore-dms-2.5.2/types_aiobotocore_dms/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-dms-2.5.1/types_aiobotocore_dms/type_defs.pyi` & `types-aiobotocore-dms-2.5.2/types_aiobotocore_dms/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-dms-2.5.1/types_aiobotocore_dms/waiter.py` & `types-aiobotocore-dms-2.5.2/types_aiobotocore_dms/waiter.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-dms-2.5.1/types_aiobotocore_dms/waiter.pyi` & `types-aiobotocore-dms-2.5.2/types_aiobotocore_dms/waiter.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-dms-2.5.1/types_aiobotocore_dms.egg-info/PKG-INFO` & `types-aiobotocore-dms-2.5.2/types_aiobotocore_dms.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-dms
-Version: 2.5.1
-Summary: Type annotations for aiobotocore.DatabaseMigrationService 2.5.1 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2
+Summary: Type annotations for aiobotocore.DatabaseMigrationService 2.5.2 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-dms.svg?color=blue)](https://pypi.org/project/types-aiobotocore-dms)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-dms?color=blue)](https://pypistats.org/packages/types-aiobotocore-dms)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.DatabaseMigrationService 2.5.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService)
+[aiobotocore.DatabaseMigrationService 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-dms-2.5.1/types_aiobotocore_dms.egg-info/SOURCES.txt` & `types-aiobotocore-dms-2.5.2/types_aiobotocore_dms.egg-info/SOURCES.txt`

 * *Files identical despite different names*

