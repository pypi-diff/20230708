# Comparing `tmp/types-aiobotocore-devops-guru-2.5.1.tar.gz` & `tmp/types-aiobotocore-devops-guru-2.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-devops-guru-2.5.1.tar", last modified: Wed Jun 28 01:43:22 2023, max compression
+gzip compressed data, was "types-aiobotocore-devops-guru-2.5.2.tar", last modified: Sat Jul  8 01:43:30 2023, max compression
```

## Comparing `types-aiobotocore-devops-guru-2.5.1.tar` & `types-aiobotocore-devops-guru-2.5.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 01:43:22.574123 types-aiobotocore-devops-guru-2.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-28 01:29:03.000000 types-aiobotocore-devops-guru-2.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    23414 2023-06-28 01:43:22.570124 types-aiobotocore-devops-guru-2.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    21834 2023-06-28 01:29:03.000000 types-aiobotocore-devops-guru-2.5.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-28 01:43:22.574123 types-aiobotocore-devops-guru-2.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-06-28 01:29:03.000000 types-aiobotocore-devops-guru-2.5.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 01:43:22.562123 types-aiobotocore-devops-guru-2.5.1/types_aiobotocore_devops_guru/
--rw-r--r--   0 runner    (1001) docker     (123)     3882 2023-06-28 01:29:03.000000 types-aiobotocore-devops-guru-2.5.1/types_aiobotocore_devops_guru/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3881 2023-06-28 01:29:03.000000 types-aiobotocore-devops-guru-2.5.1/types_aiobotocore_devops_guru/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-06-28 01:29:03.000000 types-aiobotocore-devops-guru-2.5.1/types_aiobotocore_devops_guru/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    33212 2023-06-28 01:29:03.000000 types-aiobotocore-devops-guru-2.5.1/types_aiobotocore_devops_guru/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    33158 2023-06-28 01:29:03.000000 types-aiobotocore-devops-guru-2.5.1/types_aiobotocore_devops_guru/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    14012 2023-06-28 01:29:04.000000 types-aiobotocore-devops-guru-2.5.1/types_aiobotocore_devops_guru/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    14010 2023-06-28 01:29:04.000000 types-aiobotocore-devops-guru-2.5.1/types_aiobotocore_devops_guru/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    19343 2023-06-28 01:29:03.000000 types-aiobotocore-devops-guru-2.5.1/types_aiobotocore_devops_guru/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    19327 2023-06-28 01:29:03.000000 types-aiobotocore-devops-guru-2.5.1/types_aiobotocore_devops_guru/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 01:29:03.000000 types-aiobotocore-devops-guru-2.5.1/types_aiobotocore_devops_guru/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    62107 2023-06-28 01:29:05.000000 types-aiobotocore-devops-guru-2.5.1/types_aiobotocore_devops_guru/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    62042 2023-06-28 01:29:04.000000 types-aiobotocore-devops-guru-2.5.1/types_aiobotocore_devops_guru/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-28 01:29:03.000000 types-aiobotocore-devops-guru-2.5.1/types_aiobotocore_devops_guru/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 01:43:22.570124 types-aiobotocore-devops-guru-2.5.1/types_aiobotocore_devops_guru.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    23414 2023-06-28 01:43:22.000000 types-aiobotocore-devops-guru-2.5.1/types_aiobotocore_devops_guru.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-06-28 01:43:22.000000 types-aiobotocore-devops-guru-2.5.1/types_aiobotocore_devops_guru.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 01:43:22.000000 types-aiobotocore-devops-guru-2.5.1/types_aiobotocore_devops_guru.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 01:43:22.000000 types-aiobotocore-devops-guru-2.5.1/types_aiobotocore_devops_guru.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-28 01:43:22.000000 types-aiobotocore-devops-guru-2.5.1/types_aiobotocore_devops_guru.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-28 01:43:22.000000 types-aiobotocore-devops-guru-2.5.1/types_aiobotocore_devops_guru.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:30.726001 types-aiobotocore-devops-guru-2.5.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:28:41.000000 types-aiobotocore-devops-guru-2.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    23414 2023-07-08 01:43:30.726001 types-aiobotocore-devops-guru-2.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    21834 2023-07-08 01:28:41.000000 types-aiobotocore-devops-guru-2.5.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:43:30.726001 types-aiobotocore-devops-guru-2.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-07-08 01:28:41.000000 types-aiobotocore-devops-guru-2.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:30.726001 types-aiobotocore-devops-guru-2.5.2/types_aiobotocore_devops_guru/
+-rw-r--r--   0 runner    (1001) docker     (123)     3882 2023-07-08 01:28:41.000000 types-aiobotocore-devops-guru-2.5.2/types_aiobotocore_devops_guru/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3881 2023-07-08 01:28:41.000000 types-aiobotocore-devops-guru-2.5.2/types_aiobotocore_devops_guru/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-07-08 01:28:41.000000 types-aiobotocore-devops-guru-2.5.2/types_aiobotocore_devops_guru/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33212 2023-07-08 01:28:42.000000 types-aiobotocore-devops-guru-2.5.2/types_aiobotocore_devops_guru/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33158 2023-07-08 01:28:41.000000 types-aiobotocore-devops-guru-2.5.2/types_aiobotocore_devops_guru/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    14012 2023-07-08 01:28:42.000000 types-aiobotocore-devops-guru-2.5.2/types_aiobotocore_devops_guru/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14010 2023-07-08 01:28:42.000000 types-aiobotocore-devops-guru-2.5.2/types_aiobotocore_devops_guru/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    19343 2023-07-08 01:28:42.000000 types-aiobotocore-devops-guru-2.5.2/types_aiobotocore_devops_guru/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19327 2023-07-08 01:28:42.000000 types-aiobotocore-devops-guru-2.5.2/types_aiobotocore_devops_guru/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:28:41.000000 types-aiobotocore-devops-guru-2.5.2/types_aiobotocore_devops_guru/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    62107 2023-07-08 01:28:43.000000 types-aiobotocore-devops-guru-2.5.2/types_aiobotocore_devops_guru/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62042 2023-07-08 01:28:43.000000 types-aiobotocore-devops-guru-2.5.2/types_aiobotocore_devops_guru/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:28:41.000000 types-aiobotocore-devops-guru-2.5.2/types_aiobotocore_devops_guru/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:30.726001 types-aiobotocore-devops-guru-2.5.2/types_aiobotocore_devops_guru.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    23414 2023-07-08 01:43:30.000000 types-aiobotocore-devops-guru-2.5.2/types_aiobotocore_devops_guru.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-07-08 01:43:30.000000 types-aiobotocore-devops-guru-2.5.2/types_aiobotocore_devops_guru.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:30.000000 types-aiobotocore-devops-guru-2.5.2/types_aiobotocore_devops_guru.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:30.000000 types-aiobotocore-devops-guru-2.5.2/types_aiobotocore_devops_guru.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:43:30.000000 types-aiobotocore-devops-guru-2.5.2/types_aiobotocore_devops_guru.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-08 01:43:30.000000 types-aiobotocore-devops-guru-2.5.2/types_aiobotocore_devops_guru.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-devops-guru-2.5.1/LICENSE` & `types-aiobotocore-devops-guru-2.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-devops-guru-2.5.1/PKG-INFO` & `types-aiobotocore-devops-guru-2.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-devops-guru
-Version: 2.5.1
-Summary: Type annotations for aiobotocore.DevOpsGuru 2.5.1 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2
+Summary: Type annotations for aiobotocore.DevOpsGuru 2.5.2 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_devops_guru/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-devops-guru.svg?color=blue)](https://pypi.org/project/types-aiobotocore-devops-guru)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_devops_guru/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-devops-guru?color=blue)](https://pypistats.org/packages/types-aiobotocore-devops-guru)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.DevOpsGuru 2.5.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru)
+[aiobotocore.DevOpsGuru 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-devops-guru-2.5.1/README.md` & `types-aiobotocore-devops-guru-2.5.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-devops-guru.svg?color=blue)](https://pypi.org/project/types-aiobotocore-devops-guru)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_devops_guru/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-devops-guru?color=blue)](https://pypistats.org/packages/types-aiobotocore-devops-guru)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.DevOpsGuru 2.5.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru)
+[aiobotocore.DevOpsGuru 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-devops-guru-2.5.1/setup.py` & `types-aiobotocore-devops-guru-2.5.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-devops-guru",
-    version="2.5.1",
+    version="2.5.2",
     packages=["types_aiobotocore_devops_guru"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.DevOpsGuru 2.5.1 service generated with"
+        "Type annotations for aiobotocore.DevOpsGuru 2.5.2 service generated with"
         " mypy-boto3-builder 7.14.5"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-devops-guru-2.5.1/types_aiobotocore_devops_guru/__init__.py` & `types-aiobotocore-devops-guru-2.5.2/types_aiobotocore_devops_guru/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-devops-guru-2.5.1/types_aiobotocore_devops_guru/__init__.pyi` & `types-aiobotocore-devops-guru-2.5.2/types_aiobotocore_devops_guru/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-devops-guru-2.5.1/types_aiobotocore_devops_guru/__main__.py` & `types-aiobotocore-devops-guru-2.5.2/types_aiobotocore_devops_guru/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.DevOpsGuru 2.5.1\nVersion:         2.5.1\nBuilder"
+        "Type annotations for aiobotocore.DevOpsGuru 2.5.2\nVersion:         2.5.2\nBuilder"
         " version: 7.14.5\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_devops_guru//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru\nOther"
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

### Comparing `types-aiobotocore-devops-guru-2.5.1/types_aiobotocore_devops_guru/client.py` & `types-aiobotocore-devops-guru-2.5.2/types_aiobotocore_devops_guru/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-devops-guru-2.5.1/types_aiobotocore_devops_guru/client.pyi` & `types-aiobotocore-devops-guru-2.5.2/types_aiobotocore_devops_guru/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-devops-guru-2.5.1/types_aiobotocore_devops_guru/literals.py` & `types-aiobotocore-devops-guru-2.5.2/types_aiobotocore_devops_guru/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-devops-guru-2.5.1/types_aiobotocore_devops_guru/literals.pyi` & `types-aiobotocore-devops-guru-2.5.2/types_aiobotocore_devops_guru/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-devops-guru-2.5.1/types_aiobotocore_devops_guru/paginator.py` & `types-aiobotocore-devops-guru-2.5.2/types_aiobotocore_devops_guru/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-devops-guru-2.5.1/types_aiobotocore_devops_guru/paginator.pyi` & `types-aiobotocore-devops-guru-2.5.2/types_aiobotocore_devops_guru/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-devops-guru-2.5.1/types_aiobotocore_devops_guru/type_defs.py` & `types-aiobotocore-devops-guru-2.5.2/types_aiobotocore_devops_guru/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-devops-guru-2.5.1/types_aiobotocore_devops_guru/type_defs.pyi` & `types-aiobotocore-devops-guru-2.5.2/types_aiobotocore_devops_guru/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-devops-guru-2.5.1/types_aiobotocore_devops_guru.egg-info/PKG-INFO` & `types-aiobotocore-devops-guru-2.5.2/types_aiobotocore_devops_guru.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-devops-guru
-Version: 2.5.1
-Summary: Type annotations for aiobotocore.DevOpsGuru 2.5.1 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2
+Summary: Type annotations for aiobotocore.DevOpsGuru 2.5.2 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_devops_guru/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-devops-guru.svg?color=blue)](https://pypi.org/project/types-aiobotocore-devops-guru)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_devops_guru/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-devops-guru?color=blue)](https://pypistats.org/packages/types-aiobotocore-devops-guru)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.DevOpsGuru 2.5.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru)
+[aiobotocore.DevOpsGuru 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-devops-guru-2.5.1/types_aiobotocore_devops_guru.egg-info/SOURCES.txt` & `types-aiobotocore-devops-guru-2.5.2/types_aiobotocore_devops_guru.egg-info/SOURCES.txt`

 * *Files identical despite different names*

