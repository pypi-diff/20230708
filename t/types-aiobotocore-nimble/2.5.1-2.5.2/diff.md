# Comparing `tmp/types-aiobotocore-nimble-2.5.1.tar.gz` & `tmp/types-aiobotocore-nimble-2.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-nimble-2.5.1.tar", last modified: Wed Jun 28 01:43:54 2023, max compression
+gzip compressed data, was "types-aiobotocore-nimble-2.5.2.tar", last modified: Sat Jul  8 01:44:02 2023, max compression
```

## Comparing `types-aiobotocore-nimble-2.5.1.tar` & `types-aiobotocore-nimble-2.5.2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 01:43:54.422183 types-aiobotocore-nimble-2.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-28 01:35:58.000000 types-aiobotocore-nimble-2.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    25144 2023-06-28 01:43:54.422183 types-aiobotocore-nimble-2.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    23577 2023-06-28 01:35:58.000000 types-aiobotocore-nimble-2.5.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-28 01:43:54.422183 types-aiobotocore-nimble-2.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-06-28 01:35:58.000000 types-aiobotocore-nimble-2.5.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 01:43:54.418183 types-aiobotocore-nimble-2.5.1/types_aiobotocore_nimble/
--rw-r--r--   0 runner    (1001) docker     (123)     5224 2023-06-28 01:35:58.000000 types-aiobotocore-nimble-2.5.1/types_aiobotocore_nimble/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5223 2023-06-28 01:35:58.000000 types-aiobotocore-nimble-2.5.1/types_aiobotocore_nimble/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-06-28 01:35:58.000000 types-aiobotocore-nimble-2.5.1/types_aiobotocore_nimble/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    47143 2023-06-28 01:35:58.000000 types-aiobotocore-nimble-2.5.1/types_aiobotocore_nimble/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    47063 2023-06-28 01:35:58.000000 types-aiobotocore-nimble-2.5.1/types_aiobotocore_nimble/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    18079 2023-06-28 01:35:59.000000 types-aiobotocore-nimble-2.5.1/types_aiobotocore_nimble/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    18077 2023-06-28 01:35:58.000000 types-aiobotocore-nimble-2.5.1/types_aiobotocore_nimble/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12938 2023-06-28 01:35:58.000000 types-aiobotocore-nimble-2.5.1/types_aiobotocore_nimble/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    12926 2023-06-28 01:35:58.000000 types-aiobotocore-nimble-2.5.1/types_aiobotocore_nimble/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 01:35:58.000000 types-aiobotocore-nimble-2.5.1/types_aiobotocore_nimble/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    70126 2023-06-28 01:36:00.000000 types-aiobotocore-nimble-2.5.1/types_aiobotocore_nimble/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    70009 2023-06-28 01:35:59.000000 types-aiobotocore-nimble-2.5.1/types_aiobotocore_nimble/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-28 01:35:58.000000 types-aiobotocore-nimble-2.5.1/types_aiobotocore_nimble/version.py
--rw-r--r--   0 runner    (1001) docker     (123)    13016 2023-06-28 01:35:58.000000 types-aiobotocore-nimble-2.5.1/types_aiobotocore_nimble/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)    13004 2023-06-28 01:35:58.000000 types-aiobotocore-nimble-2.5.1/types_aiobotocore_nimble/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 01:43:54.422183 types-aiobotocore-nimble-2.5.1/types_aiobotocore_nimble.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    25144 2023-06-28 01:43:54.000000 types-aiobotocore-nimble-2.5.1/types_aiobotocore_nimble.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-06-28 01:43:54.000000 types-aiobotocore-nimble-2.5.1/types_aiobotocore_nimble.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 01:43:54.000000 types-aiobotocore-nimble-2.5.1/types_aiobotocore_nimble.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 01:43:54.000000 types-aiobotocore-nimble-2.5.1/types_aiobotocore_nimble.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-28 01:43:54.000000 types-aiobotocore-nimble-2.5.1/types_aiobotocore_nimble.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-28 01:43:54.000000 types-aiobotocore-nimble-2.5.1/types_aiobotocore_nimble.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:02.754603 types-aiobotocore-nimble-2.5.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:35:49.000000 types-aiobotocore-nimble-2.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    25144 2023-07-08 01:44:02.750603 types-aiobotocore-nimble-2.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    23577 2023-07-08 01:35:49.000000 types-aiobotocore-nimble-2.5.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:44:02.754603 types-aiobotocore-nimble-2.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-07-08 01:35:49.000000 types-aiobotocore-nimble-2.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:02.750603 types-aiobotocore-nimble-2.5.2/types_aiobotocore_nimble/
+-rw-r--r--   0 runner    (1001) docker     (123)     5224 2023-07-08 01:35:49.000000 types-aiobotocore-nimble-2.5.2/types_aiobotocore_nimble/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5223 2023-07-08 01:35:49.000000 types-aiobotocore-nimble-2.5.2/types_aiobotocore_nimble/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-07-08 01:35:49.000000 types-aiobotocore-nimble-2.5.2/types_aiobotocore_nimble/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47143 2023-07-08 01:35:51.000000 types-aiobotocore-nimble-2.5.2/types_aiobotocore_nimble/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47063 2023-07-08 01:35:51.000000 types-aiobotocore-nimble-2.5.2/types_aiobotocore_nimble/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    18079 2023-07-08 01:35:51.000000 types-aiobotocore-nimble-2.5.2/types_aiobotocore_nimble/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18077 2023-07-08 01:35:51.000000 types-aiobotocore-nimble-2.5.2/types_aiobotocore_nimble/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12938 2023-07-08 01:35:51.000000 types-aiobotocore-nimble-2.5.2/types_aiobotocore_nimble/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12926 2023-07-08 01:35:51.000000 types-aiobotocore-nimble-2.5.2/types_aiobotocore_nimble/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:35:49.000000 types-aiobotocore-nimble-2.5.2/types_aiobotocore_nimble/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    70126 2023-07-08 01:35:53.000000 types-aiobotocore-nimble-2.5.2/types_aiobotocore_nimble/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    70009 2023-07-08 01:35:52.000000 types-aiobotocore-nimble-2.5.2/types_aiobotocore_nimble/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:35:49.000000 types-aiobotocore-nimble-2.5.2/types_aiobotocore_nimble/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13016 2023-07-08 01:35:51.000000 types-aiobotocore-nimble-2.5.2/types_aiobotocore_nimble/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13004 2023-07-08 01:35:51.000000 types-aiobotocore-nimble-2.5.2/types_aiobotocore_nimble/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:02.750603 types-aiobotocore-nimble-2.5.2/types_aiobotocore_nimble.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    25144 2023-07-08 01:44:02.000000 types-aiobotocore-nimble-2.5.2/types_aiobotocore_nimble.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-07-08 01:44:02.000000 types-aiobotocore-nimble-2.5.2/types_aiobotocore_nimble.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:44:02.000000 types-aiobotocore-nimble-2.5.2/types_aiobotocore_nimble.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:44:02.000000 types-aiobotocore-nimble-2.5.2/types_aiobotocore_nimble.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:44:02.000000 types-aiobotocore-nimble-2.5.2/types_aiobotocore_nimble.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-08 01:44:02.000000 types-aiobotocore-nimble-2.5.2/types_aiobotocore_nimble.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-nimble-2.5.1/LICENSE` & `types-aiobotocore-nimble-2.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-nimble-2.5.1/PKG-INFO` & `types-aiobotocore-nimble-2.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-nimble
-Version: 2.5.1
-Summary: Type annotations for aiobotocore.NimbleStudio 2.5.1 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2
+Summary: Type annotations for aiobotocore.NimbleStudio 2.5.2 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_nimble/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-nimble.svg?color=blue)](https://pypi.org/project/types-aiobotocore-nimble)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_nimble/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-nimble?color=blue)](https://pypistats.org/packages/types-aiobotocore-nimble)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.NimbleStudio 2.5.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/nimble.html#NimbleStudio)
+[aiobotocore.NimbleStudio 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/nimble.html#NimbleStudio)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-nimble-2.5.1/README.md` & `types-aiobotocore-nimble-2.5.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-nimble.svg?color=blue)](https://pypi.org/project/types-aiobotocore-nimble)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_nimble/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-nimble?color=blue)](https://pypistats.org/packages/types-aiobotocore-nimble)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.NimbleStudio 2.5.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/nimble.html#NimbleStudio)
+[aiobotocore.NimbleStudio 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/nimble.html#NimbleStudio)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-nimble-2.5.1/setup.py` & `types-aiobotocore-nimble-2.5.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-nimble",
-    version="2.5.1",
+    version="2.5.2",
     packages=["types_aiobotocore_nimble"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.NimbleStudio 2.5.1 service generated with"
+        "Type annotations for aiobotocore.NimbleStudio 2.5.2 service generated with"
         " mypy-boto3-builder 7.14.5"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-nimble-2.5.1/types_aiobotocore_nimble/__init__.py` & `types-aiobotocore-nimble-2.5.2/types_aiobotocore_nimble/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-nimble-2.5.1/types_aiobotocore_nimble/__init__.pyi` & `types-aiobotocore-nimble-2.5.2/types_aiobotocore_nimble/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-nimble-2.5.1/types_aiobotocore_nimble/__main__.py` & `types-aiobotocore-nimble-2.5.2/types_aiobotocore_nimble/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.NimbleStudio 2.5.1\nVersion:         2.5.1\nBuilder"
+        "Type annotations for aiobotocore.NimbleStudio 2.5.2\nVersion:         2.5.2\nBuilder"
         " version: 7.14.5\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_nimble//\nBoto3 docs: "
         "     https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/nimble.html#NimbleStudio\nOther"
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

### Comparing `types-aiobotocore-nimble-2.5.1/types_aiobotocore_nimble/client.py` & `types-aiobotocore-nimble-2.5.2/types_aiobotocore_nimble/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-nimble-2.5.1/types_aiobotocore_nimble/client.pyi` & `types-aiobotocore-nimble-2.5.2/types_aiobotocore_nimble/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-nimble-2.5.1/types_aiobotocore_nimble/literals.py` & `types-aiobotocore-nimble-2.5.2/types_aiobotocore_nimble/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-nimble-2.5.1/types_aiobotocore_nimble/literals.pyi` & `types-aiobotocore-nimble-2.5.2/types_aiobotocore_nimble/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-nimble-2.5.1/types_aiobotocore_nimble/paginator.py` & `types-aiobotocore-nimble-2.5.2/types_aiobotocore_nimble/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-nimble-2.5.1/types_aiobotocore_nimble/paginator.pyi` & `types-aiobotocore-nimble-2.5.2/types_aiobotocore_nimble/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-nimble-2.5.1/types_aiobotocore_nimble/type_defs.py` & `types-aiobotocore-nimble-2.5.2/types_aiobotocore_nimble/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-nimble-2.5.1/types_aiobotocore_nimble/type_defs.pyi` & `types-aiobotocore-nimble-2.5.2/types_aiobotocore_nimble/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-nimble-2.5.1/types_aiobotocore_nimble/waiter.py` & `types-aiobotocore-nimble-2.5.2/types_aiobotocore_nimble/waiter.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-nimble-2.5.1/types_aiobotocore_nimble/waiter.pyi` & `types-aiobotocore-nimble-2.5.2/types_aiobotocore_nimble/waiter.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-nimble-2.5.1/types_aiobotocore_nimble.egg-info/PKG-INFO` & `types-aiobotocore-nimble-2.5.2/types_aiobotocore_nimble.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-nimble
-Version: 2.5.1
-Summary: Type annotations for aiobotocore.NimbleStudio 2.5.1 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2
+Summary: Type annotations for aiobotocore.NimbleStudio 2.5.2 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_nimble/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-nimble.svg?color=blue)](https://pypi.org/project/types-aiobotocore-nimble)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_nimble/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-nimble?color=blue)](https://pypistats.org/packages/types-aiobotocore-nimble)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.NimbleStudio 2.5.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/nimble.html#NimbleStudio)
+[aiobotocore.NimbleStudio 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/nimble.html#NimbleStudio)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-nimble-2.5.1/types_aiobotocore_nimble.egg-info/SOURCES.txt` & `types-aiobotocore-nimble-2.5.2/types_aiobotocore_nimble.egg-info/SOURCES.txt`

 * *Files identical despite different names*

