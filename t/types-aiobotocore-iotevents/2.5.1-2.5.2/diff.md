# Comparing `tmp/types-aiobotocore-iotevents-2.5.1.tar.gz` & `tmp/types-aiobotocore-iotevents-2.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-iotevents-2.5.1.tar", last modified: Wed Jun 28 01:43:38 2023, max compression
+gzip compressed data, was "types-aiobotocore-iotevents-2.5.2.tar", last modified: Sat Jul  8 01:43:46 2023, max compression
```

## Comparing `types-aiobotocore-iotevents-2.5.1.tar` & `types-aiobotocore-iotevents-2.5.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 01:43:38.418153 types-aiobotocore-iotevents-2.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-28 01:32:56.000000 types-aiobotocore-iotevents-2.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16148 2023-06-28 01:43:38.410153 types-aiobotocore-iotevents-2.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14575 2023-06-28 01:32:56.000000 types-aiobotocore-iotevents-2.5.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-28 01:43:38.418153 types-aiobotocore-iotevents-2.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2132 2023-06-28 01:32:56.000000 types-aiobotocore-iotevents-2.5.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 01:43:38.406153 types-aiobotocore-iotevents-2.5.1/types_aiobotocore_iotevents/
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-06-28 01:32:56.000000 types-aiobotocore-iotevents-2.5.1/types_aiobotocore_iotevents/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-06-28 01:32:56.000000 types-aiobotocore-iotevents-2.5.1/types_aiobotocore_iotevents/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-06-28 01:32:56.000000 types-aiobotocore-iotevents-2.5.1/types_aiobotocore_iotevents/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20395 2023-06-28 01:32:56.000000 types-aiobotocore-iotevents-2.5.1/types_aiobotocore_iotevents/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    20361 2023-06-28 01:32:56.000000 types-aiobotocore-iotevents-2.5.1/types_aiobotocore_iotevents/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8754 2023-06-28 01:32:56.000000 types-aiobotocore-iotevents-2.5.1/types_aiobotocore_iotevents/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8752 2023-06-28 01:32:56.000000 types-aiobotocore-iotevents-2.5.1/types_aiobotocore_iotevents/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 01:32:56.000000 types-aiobotocore-iotevents-2.5.1/types_aiobotocore_iotevents/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    37414 2023-06-28 01:32:58.000000 types-aiobotocore-iotevents-2.5.1/types_aiobotocore_iotevents/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    37349 2023-06-28 01:32:57.000000 types-aiobotocore-iotevents-2.5.1/types_aiobotocore_iotevents/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-28 01:32:56.000000 types-aiobotocore-iotevents-2.5.1/types_aiobotocore_iotevents/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 01:43:38.410153 types-aiobotocore-iotevents-2.5.1/types_aiobotocore_iotevents.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16148 2023-06-28 01:43:38.000000 types-aiobotocore-iotevents-2.5.1/types_aiobotocore_iotevents.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-06-28 01:43:38.000000 types-aiobotocore-iotevents-2.5.1/types_aiobotocore_iotevents.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 01:43:38.000000 types-aiobotocore-iotevents-2.5.1/types_aiobotocore_iotevents.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 01:43:38.000000 types-aiobotocore-iotevents-2.5.1/types_aiobotocore_iotevents.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-28 01:43:38.000000 types-aiobotocore-iotevents-2.5.1/types_aiobotocore_iotevents.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-28 01:43:38.000000 types-aiobotocore-iotevents-2.5.1/types_aiobotocore_iotevents.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:46.722303 types-aiobotocore-iotevents-2.5.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:32:43.000000 types-aiobotocore-iotevents-2.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16148 2023-07-08 01:43:46.722303 types-aiobotocore-iotevents-2.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14575 2023-07-08 01:32:43.000000 types-aiobotocore-iotevents-2.5.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:43:46.722303 types-aiobotocore-iotevents-2.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2132 2023-07-08 01:32:43.000000 types-aiobotocore-iotevents-2.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:46.722303 types-aiobotocore-iotevents-2.5.2/types_aiobotocore_iotevents/
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-07-08 01:32:43.000000 types-aiobotocore-iotevents-2.5.2/types_aiobotocore_iotevents/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-07-08 01:32:43.000000 types-aiobotocore-iotevents-2.5.2/types_aiobotocore_iotevents/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-07-08 01:32:43.000000 types-aiobotocore-iotevents-2.5.2/types_aiobotocore_iotevents/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20395 2023-07-08 01:32:43.000000 types-aiobotocore-iotevents-2.5.2/types_aiobotocore_iotevents/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20361 2023-07-08 01:32:43.000000 types-aiobotocore-iotevents-2.5.2/types_aiobotocore_iotevents/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8754 2023-07-08 01:32:43.000000 types-aiobotocore-iotevents-2.5.2/types_aiobotocore_iotevents/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8752 2023-07-08 01:32:43.000000 types-aiobotocore-iotevents-2.5.2/types_aiobotocore_iotevents/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:32:43.000000 types-aiobotocore-iotevents-2.5.2/types_aiobotocore_iotevents/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    37414 2023-07-08 01:32:44.000000 types-aiobotocore-iotevents-2.5.2/types_aiobotocore_iotevents/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37349 2023-07-08 01:32:43.000000 types-aiobotocore-iotevents-2.5.2/types_aiobotocore_iotevents/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:32:43.000000 types-aiobotocore-iotevents-2.5.2/types_aiobotocore_iotevents/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:46.722303 types-aiobotocore-iotevents-2.5.2/types_aiobotocore_iotevents.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16148 2023-07-08 01:43:46.000000 types-aiobotocore-iotevents-2.5.2/types_aiobotocore_iotevents.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-07-08 01:43:46.000000 types-aiobotocore-iotevents-2.5.2/types_aiobotocore_iotevents.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:46.000000 types-aiobotocore-iotevents-2.5.2/types_aiobotocore_iotevents.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:46.000000 types-aiobotocore-iotevents-2.5.2/types_aiobotocore_iotevents.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:43:46.000000 types-aiobotocore-iotevents-2.5.2/types_aiobotocore_iotevents.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-08 01:43:46.000000 types-aiobotocore-iotevents-2.5.2/types_aiobotocore_iotevents.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-iotevents-2.5.1/LICENSE` & `types-aiobotocore-iotevents-2.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iotevents-2.5.1/PKG-INFO` & `types-aiobotocore-iotevents-2.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-iotevents
-Version: 2.5.1
-Summary: Type annotations for aiobotocore.IoTEvents 2.5.1 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2
+Summary: Type annotations for aiobotocore.IoTEvents 2.5.2 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotevents/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-iotevents.svg?color=blue)](https://pypi.org/project/types-aiobotocore-iotevents)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotevents/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-iotevents?color=blue)](https://pypistats.org/packages/types-aiobotocore-iotevents)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.IoTEvents 2.5.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents.html#IoTEvents)
+[aiobotocore.IoTEvents 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents.html#IoTEvents)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-iotevents-2.5.1/README.md` & `types-aiobotocore-iotevents-2.5.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-iotevents.svg?color=blue)](https://pypi.org/project/types-aiobotocore-iotevents)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotevents/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-iotevents?color=blue)](https://pypistats.org/packages/types-aiobotocore-iotevents)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.IoTEvents 2.5.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents.html#IoTEvents)
+[aiobotocore.IoTEvents 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents.html#IoTEvents)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-iotevents-2.5.1/setup.py` & `types-aiobotocore-iotevents-2.5.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-iotevents",
-    version="2.5.1",
+    version="2.5.2",
     packages=["types_aiobotocore_iotevents"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.IoTEvents 2.5.1 service generated with mypy-boto3-builder"
+        "Type annotations for aiobotocore.IoTEvents 2.5.2 service generated with mypy-boto3-builder"
         " 7.14.5"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-iotevents-2.5.1/types_aiobotocore_iotevents/__main__.py` & `types-aiobotocore-iotevents-2.5.2/types_aiobotocore_iotevents/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.IoTEvents 2.5.1\nVersion:         2.5.1\nBuilder version:"
+        "Type annotations for aiobotocore.IoTEvents 2.5.2\nVersion:         2.5.2\nBuilder version:"
         " 7.14.5\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotevents//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents.html#IoTEvents\nOther"
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

### Comparing `types-aiobotocore-iotevents-2.5.1/types_aiobotocore_iotevents/client.py` & `types-aiobotocore-iotevents-2.5.2/types_aiobotocore_iotevents/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iotevents-2.5.1/types_aiobotocore_iotevents/client.pyi` & `types-aiobotocore-iotevents-2.5.2/types_aiobotocore_iotevents/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iotevents-2.5.1/types_aiobotocore_iotevents/literals.py` & `types-aiobotocore-iotevents-2.5.2/types_aiobotocore_iotevents/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iotevents-2.5.1/types_aiobotocore_iotevents/literals.pyi` & `types-aiobotocore-iotevents-2.5.2/types_aiobotocore_iotevents/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iotevents-2.5.1/types_aiobotocore_iotevents/type_defs.py` & `types-aiobotocore-iotevents-2.5.2/types_aiobotocore_iotevents/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iotevents-2.5.1/types_aiobotocore_iotevents/type_defs.pyi` & `types-aiobotocore-iotevents-2.5.2/types_aiobotocore_iotevents/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iotevents-2.5.1/types_aiobotocore_iotevents.egg-info/PKG-INFO` & `types-aiobotocore-iotevents-2.5.2/types_aiobotocore_iotevents.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-iotevents
-Version: 2.5.1
-Summary: Type annotations for aiobotocore.IoTEvents 2.5.1 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2
+Summary: Type annotations for aiobotocore.IoTEvents 2.5.2 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotevents/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-iotevents.svg?color=blue)](https://pypi.org/project/types-aiobotocore-iotevents)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotevents/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-iotevents?color=blue)](https://pypistats.org/packages/types-aiobotocore-iotevents)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.IoTEvents 2.5.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents.html#IoTEvents)
+[aiobotocore.IoTEvents 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents.html#IoTEvents)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-iotevents-2.5.1/types_aiobotocore_iotevents.egg-info/SOURCES.txt` & `types-aiobotocore-iotevents-2.5.2/types_aiobotocore_iotevents.egg-info/SOURCES.txt`

 * *Files identical despite different names*

