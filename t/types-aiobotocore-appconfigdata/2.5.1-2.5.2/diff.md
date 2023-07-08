# Comparing `tmp/types-aiobotocore-appconfigdata-2.5.1.tar.gz` & `tmp/types-aiobotocore-appconfigdata-2.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-appconfigdata-2.5.1.tar", last modified: Wed Jun 28 01:43:04 2023, max compression
+gzip compressed data, was "types-aiobotocore-appconfigdata-2.5.2.tar", last modified: Sat Jul  8 01:43:12 2023, max compression
```

## Comparing `types-aiobotocore-appconfigdata-2.5.1.tar` & `types-aiobotocore-appconfigdata-2.5.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 01:43:04.346090 types-aiobotocore-appconfigdata-2.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-28 01:26:07.000000 types-aiobotocore-appconfigdata-2.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    12561 2023-06-28 01:43:04.342090 types-aiobotocore-appconfigdata-2.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10972 2023-06-28 01:26:07.000000 types-aiobotocore-appconfigdata-2.5.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-28 01:43:04.346090 types-aiobotocore-appconfigdata-2.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2160 2023-06-28 01:26:07.000000 types-aiobotocore-appconfigdata-2.5.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 01:43:04.342090 types-aiobotocore-appconfigdata-2.5.1/types_aiobotocore_appconfigdata/
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-06-28 01:26:07.000000 types-aiobotocore-appconfigdata-2.5.1/types_aiobotocore_appconfigdata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-06-28 01:26:07.000000 types-aiobotocore-appconfigdata-2.5.1/types_aiobotocore_appconfigdata/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-06-28 01:26:07.000000 types-aiobotocore-appconfigdata-2.5.1/types_aiobotocore_appconfigdata/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5572 2023-06-28 01:26:07.000000 types-aiobotocore-appconfigdata-2.5.1/types_aiobotocore_appconfigdata/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     5562 2023-06-28 01:26:07.000000 types-aiobotocore-appconfigdata-2.5.1/types_aiobotocore_appconfigdata/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8110 2023-06-28 01:26:07.000000 types-aiobotocore-appconfigdata-2.5.1/types_aiobotocore_appconfigdata/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8108 2023-06-28 01:26:07.000000 types-aiobotocore-appconfigdata-2.5.1/types_aiobotocore_appconfigdata/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 01:26:07.000000 types-aiobotocore-appconfigdata-2.5.1/types_aiobotocore_appconfigdata/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-06-28 01:26:07.000000 types-aiobotocore-appconfigdata-2.5.1/types_aiobotocore_appconfigdata/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-06-28 01:26:07.000000 types-aiobotocore-appconfigdata-2.5.1/types_aiobotocore_appconfigdata/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-28 01:26:07.000000 types-aiobotocore-appconfigdata-2.5.1/types_aiobotocore_appconfigdata/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 01:43:04.342090 types-aiobotocore-appconfigdata-2.5.1/types_aiobotocore_appconfigdata.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12561 2023-06-28 01:43:04.000000 types-aiobotocore-appconfigdata-2.5.1/types_aiobotocore_appconfigdata.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-06-28 01:43:04.000000 types-aiobotocore-appconfigdata-2.5.1/types_aiobotocore_appconfigdata.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 01:43:04.000000 types-aiobotocore-appconfigdata-2.5.1/types_aiobotocore_appconfigdata.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 01:43:04.000000 types-aiobotocore-appconfigdata-2.5.1/types_aiobotocore_appconfigdata.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-28 01:43:04.000000 types-aiobotocore-appconfigdata-2.5.1/types_aiobotocore_appconfigdata.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-28 01:43:04.000000 types-aiobotocore-appconfigdata-2.5.1/types_aiobotocore_appconfigdata.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:12.433654 types-aiobotocore-appconfigdata-2.5.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:25:41.000000 types-aiobotocore-appconfigdata-2.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12561 2023-07-08 01:43:12.433654 types-aiobotocore-appconfigdata-2.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10972 2023-07-08 01:25:41.000000 types-aiobotocore-appconfigdata-2.5.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:43:12.433654 types-aiobotocore-appconfigdata-2.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2160 2023-07-08 01:25:41.000000 types-aiobotocore-appconfigdata-2.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:12.425654 types-aiobotocore-appconfigdata-2.5.2/types_aiobotocore_appconfigdata/
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-07-08 01:25:41.000000 types-aiobotocore-appconfigdata-2.5.2/types_aiobotocore_appconfigdata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-07-08 01:25:41.000000 types-aiobotocore-appconfigdata-2.5.2/types_aiobotocore_appconfigdata/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-07-08 01:25:41.000000 types-aiobotocore-appconfigdata-2.5.2/types_aiobotocore_appconfigdata/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5572 2023-07-08 01:25:41.000000 types-aiobotocore-appconfigdata-2.5.2/types_aiobotocore_appconfigdata/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5562 2023-07-08 01:25:41.000000 types-aiobotocore-appconfigdata-2.5.2/types_aiobotocore_appconfigdata/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8110 2023-07-08 01:25:42.000000 types-aiobotocore-appconfigdata-2.5.2/types_aiobotocore_appconfigdata/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8108 2023-07-08 01:25:42.000000 types-aiobotocore-appconfigdata-2.5.2/types_aiobotocore_appconfigdata/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:25:41.000000 types-aiobotocore-appconfigdata-2.5.2/types_aiobotocore_appconfigdata/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-07-08 01:25:42.000000 types-aiobotocore-appconfigdata-2.5.2/types_aiobotocore_appconfigdata/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-07-08 01:25:42.000000 types-aiobotocore-appconfigdata-2.5.2/types_aiobotocore_appconfigdata/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:25:41.000000 types-aiobotocore-appconfigdata-2.5.2/types_aiobotocore_appconfigdata/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:12.433654 types-aiobotocore-appconfigdata-2.5.2/types_aiobotocore_appconfigdata.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12561 2023-07-08 01:43:12.000000 types-aiobotocore-appconfigdata-2.5.2/types_aiobotocore_appconfigdata.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-07-08 01:43:12.000000 types-aiobotocore-appconfigdata-2.5.2/types_aiobotocore_appconfigdata.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:12.000000 types-aiobotocore-appconfigdata-2.5.2/types_aiobotocore_appconfigdata.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:12.000000 types-aiobotocore-appconfigdata-2.5.2/types_aiobotocore_appconfigdata.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:43:12.000000 types-aiobotocore-appconfigdata-2.5.2/types_aiobotocore_appconfigdata.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-08 01:43:12.000000 types-aiobotocore-appconfigdata-2.5.2/types_aiobotocore_appconfigdata.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-appconfigdata-2.5.1/LICENSE` & `types-aiobotocore-appconfigdata-2.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-appconfigdata-2.5.1/PKG-INFO` & `types-aiobotocore-appconfigdata-2.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-appconfigdata
-Version: 2.5.1
-Summary: Type annotations for aiobotocore.AppConfigData 2.5.1 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2
+Summary: Type annotations for aiobotocore.AppConfigData 2.5.2 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appconfigdata/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-appconfigdata.svg?color=blue)](https://pypi.org/project/types-aiobotocore-appconfigdata)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appconfigdata/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-appconfigdata?color=blue)](https://pypistats.org/packages/types-aiobotocore-appconfigdata)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.AppConfigData 2.5.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfigdata.html#AppConfigData)
+[aiobotocore.AppConfigData 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfigdata.html#AppConfigData)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-appconfigdata-2.5.1/README.md` & `types-aiobotocore-appconfigdata-2.5.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-appconfigdata.svg?color=blue)](https://pypi.org/project/types-aiobotocore-appconfigdata)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appconfigdata/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-appconfigdata?color=blue)](https://pypistats.org/packages/types-aiobotocore-appconfigdata)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.AppConfigData 2.5.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfigdata.html#AppConfigData)
+[aiobotocore.AppConfigData 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfigdata.html#AppConfigData)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-appconfigdata-2.5.1/setup.py` & `types-aiobotocore-appconfigdata-2.5.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-appconfigdata",
-    version="2.5.1",
+    version="2.5.2",
     packages=["types_aiobotocore_appconfigdata"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.AppConfigData 2.5.1 service generated with"
+        "Type annotations for aiobotocore.AppConfigData 2.5.2 service generated with"
         " mypy-boto3-builder 7.14.5"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-appconfigdata-2.5.1/types_aiobotocore_appconfigdata/__main__.py` & `types-aiobotocore-appconfigdata-2.5.2/types_aiobotocore_appconfigdata/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.AppConfigData 2.5.1\nVersion:         2.5.1\nBuilder"
+        "Type annotations for aiobotocore.AppConfigData 2.5.2\nVersion:         2.5.2\nBuilder"
         " version: 7.14.5\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appconfigdata//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfigdata.html#AppConfigData\nOther"
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

### Comparing `types-aiobotocore-appconfigdata-2.5.1/types_aiobotocore_appconfigdata/client.py` & `types-aiobotocore-appconfigdata-2.5.2/types_aiobotocore_appconfigdata/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-appconfigdata-2.5.1/types_aiobotocore_appconfigdata/client.pyi` & `types-aiobotocore-appconfigdata-2.5.2/types_aiobotocore_appconfigdata/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-appconfigdata-2.5.1/types_aiobotocore_appconfigdata/literals.py` & `types-aiobotocore-appconfigdata-2.5.2/types_aiobotocore_appconfigdata/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-appconfigdata-2.5.1/types_aiobotocore_appconfigdata/literals.pyi` & `types-aiobotocore-appconfigdata-2.5.2/types_aiobotocore_appconfigdata/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-appconfigdata-2.5.1/types_aiobotocore_appconfigdata/type_defs.py` & `types-aiobotocore-appconfigdata-2.5.2/types_aiobotocore_appconfigdata/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-appconfigdata-2.5.1/types_aiobotocore_appconfigdata/type_defs.pyi` & `types-aiobotocore-appconfigdata-2.5.2/types_aiobotocore_appconfigdata/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-appconfigdata-2.5.1/types_aiobotocore_appconfigdata.egg-info/PKG-INFO` & `types-aiobotocore-appconfigdata-2.5.2/types_aiobotocore_appconfigdata.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-appconfigdata
-Version: 2.5.1
-Summary: Type annotations for aiobotocore.AppConfigData 2.5.1 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2
+Summary: Type annotations for aiobotocore.AppConfigData 2.5.2 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appconfigdata/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-appconfigdata.svg?color=blue)](https://pypi.org/project/types-aiobotocore-appconfigdata)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appconfigdata/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-appconfigdata?color=blue)](https://pypistats.org/packages/types-aiobotocore-appconfigdata)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.AppConfigData 2.5.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfigdata.html#AppConfigData)
+[aiobotocore.AppConfigData 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfigdata.html#AppConfigData)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-appconfigdata-2.5.1/types_aiobotocore_appconfigdata.egg-info/SOURCES.txt` & `types-aiobotocore-appconfigdata-2.5.2/types_aiobotocore_appconfigdata.egg-info/SOURCES.txt`

 * *Files identical despite different names*

