# Comparing `tmp/types-aiobotocore-connect-2.5.1.tar.gz` & `tmp/types-aiobotocore-connect-2.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-connect-2.5.1.tar", last modified: Wed Jun 28 01:43:20 2023, max compression
+gzip compressed data, was "types-aiobotocore-connect-2.5.2.tar", last modified: Sat Jul  8 01:43:28 2023, max compression
```

## Comparing `types-aiobotocore-connect-2.5.1.tar` & `types-aiobotocore-connect-2.5.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 01:43:20.102119 types-aiobotocore-connect-2.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-28 01:28:28.000000 types-aiobotocore-connect-2.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    46080 2023-06-28 01:43:20.102119 types-aiobotocore-connect-2.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    44515 2023-06-28 01:28:28.000000 types-aiobotocore-connect-2.5.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-28 01:43:20.102119 types-aiobotocore-connect-2.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-06-28 01:28:28.000000 types-aiobotocore-connect-2.5.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 01:43:20.102119 types-aiobotocore-connect-2.5.1/types_aiobotocore_connect/
--rw-r--r--   0 runner    (1001) docker     (123)    10331 2023-06-28 01:28:28.000000 types-aiobotocore-connect-2.5.1/types_aiobotocore_connect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10330 2023-06-28 01:28:28.000000 types-aiobotocore-connect-2.5.1/types_aiobotocore_connect/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-06-28 01:28:28.000000 types-aiobotocore-connect-2.5.1/types_aiobotocore_connect/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)   157104 2023-06-28 01:28:30.000000 types-aiobotocore-connect-2.5.1/types_aiobotocore_connect/client.py
--rw-r--r--   0 runner    (1001) docker     (123)   156856 2023-06-28 01:28:30.000000 types-aiobotocore-connect-2.5.1/types_aiobotocore_connect/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    25347 2023-06-28 01:28:31.000000 types-aiobotocore-connect-2.5.1/types_aiobotocore_connect/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    25345 2023-06-28 01:28:31.000000 types-aiobotocore-connect-2.5.1/types_aiobotocore_connect/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    56459 2023-06-28 01:28:30.000000 types-aiobotocore-connect-2.5.1/types_aiobotocore_connect/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    56412 2023-06-28 01:28:30.000000 types-aiobotocore-connect-2.5.1/types_aiobotocore_connect/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 01:28:28.000000 types-aiobotocore-connect-2.5.1/types_aiobotocore_connect/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)   218188 2023-06-28 01:28:36.000000 types-aiobotocore-connect-2.5.1/types_aiobotocore_connect/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)   217857 2023-06-28 01:28:34.000000 types-aiobotocore-connect-2.5.1/types_aiobotocore_connect/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-28 01:28:28.000000 types-aiobotocore-connect-2.5.1/types_aiobotocore_connect/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 01:43:20.102119 types-aiobotocore-connect-2.5.1/types_aiobotocore_connect.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    46080 2023-06-28 01:43:19.000000 types-aiobotocore-connect-2.5.1/types_aiobotocore_connect.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-06-28 01:43:19.000000 types-aiobotocore-connect-2.5.1/types_aiobotocore_connect.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 01:43:19.000000 types-aiobotocore-connect-2.5.1/types_aiobotocore_connect.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 01:43:19.000000 types-aiobotocore-connect-2.5.1/types_aiobotocore_connect.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-28 01:43:19.000000 types-aiobotocore-connect-2.5.1/types_aiobotocore_connect.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-28 01:43:19.000000 types-aiobotocore-connect-2.5.1/types_aiobotocore_connect.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:28.057950 types-aiobotocore-connect-2.5.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:28:06.000000 types-aiobotocore-connect-2.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    46080 2023-07-08 01:43:28.049950 types-aiobotocore-connect-2.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    44515 2023-07-08 01:28:06.000000 types-aiobotocore-connect-2.5.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:43:28.057950 types-aiobotocore-connect-2.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-07-08 01:28:06.000000 types-aiobotocore-connect-2.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:28.049950 types-aiobotocore-connect-2.5.2/types_aiobotocore_connect/
+-rw-r--r--   0 runner    (1001) docker     (123)    10331 2023-07-08 01:28:06.000000 types-aiobotocore-connect-2.5.2/types_aiobotocore_connect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10330 2023-07-08 01:28:06.000000 types-aiobotocore-connect-2.5.2/types_aiobotocore_connect/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-07-08 01:28:06.000000 types-aiobotocore-connect-2.5.2/types_aiobotocore_connect/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   157104 2023-07-08 01:28:08.000000 types-aiobotocore-connect-2.5.2/types_aiobotocore_connect/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)   156856 2023-07-08 01:28:07.000000 types-aiobotocore-connect-2.5.2/types_aiobotocore_connect/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    25347 2023-07-08 01:28:09.000000 types-aiobotocore-connect-2.5.2/types_aiobotocore_connect/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25345 2023-07-08 01:28:09.000000 types-aiobotocore-connect-2.5.2/types_aiobotocore_connect/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    56459 2023-07-08 01:28:08.000000 types-aiobotocore-connect-2.5.2/types_aiobotocore_connect/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56412 2023-07-08 01:28:08.000000 types-aiobotocore-connect-2.5.2/types_aiobotocore_connect/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:28:06.000000 types-aiobotocore-connect-2.5.2/types_aiobotocore_connect/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)   218188 2023-07-08 01:28:15.000000 types-aiobotocore-connect-2.5.2/types_aiobotocore_connect/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   217857 2023-07-08 01:28:12.000000 types-aiobotocore-connect-2.5.2/types_aiobotocore_connect/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:28:06.000000 types-aiobotocore-connect-2.5.2/types_aiobotocore_connect/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:28.049950 types-aiobotocore-connect-2.5.2/types_aiobotocore_connect.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    46080 2023-07-08 01:43:27.000000 types-aiobotocore-connect-2.5.2/types_aiobotocore_connect.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-08 01:43:27.000000 types-aiobotocore-connect-2.5.2/types_aiobotocore_connect.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:27.000000 types-aiobotocore-connect-2.5.2/types_aiobotocore_connect.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:27.000000 types-aiobotocore-connect-2.5.2/types_aiobotocore_connect.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:43:27.000000 types-aiobotocore-connect-2.5.2/types_aiobotocore_connect.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-08 01:43:27.000000 types-aiobotocore-connect-2.5.2/types_aiobotocore_connect.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-connect-2.5.1/LICENSE` & `types-aiobotocore-connect-2.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-connect-2.5.1/PKG-INFO` & `types-aiobotocore-connect-2.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-connect
-Version: 2.5.1
-Summary: Type annotations for aiobotocore.Connect 2.5.1 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2
+Summary: Type annotations for aiobotocore.Connect 2.5.2 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-connect.svg?color=blue)](https://pypi.org/project/types-aiobotocore-connect)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-connect?color=blue)](https://pypistats.org/packages/types-aiobotocore-connect)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Connect 2.5.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect)
+[aiobotocore.Connect 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-connect-2.5.1/README.md` & `types-aiobotocore-connect-2.5.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-connect.svg?color=blue)](https://pypi.org/project/types-aiobotocore-connect)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-connect?color=blue)](https://pypistats.org/packages/types-aiobotocore-connect)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Connect 2.5.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect)
+[aiobotocore.Connect 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-connect-2.5.1/setup.py` & `types-aiobotocore-connect-2.5.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-connect",
-    version="2.5.1",
+    version="2.5.2",
     packages=["types_aiobotocore_connect"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.Connect 2.5.1 service generated with mypy-boto3-builder"
+        "Type annotations for aiobotocore.Connect 2.5.2 service generated with mypy-boto3-builder"
         " 7.14.5"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-connect-2.5.1/types_aiobotocore_connect/__init__.py` & `types-aiobotocore-connect-2.5.2/types_aiobotocore_connect/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-connect-2.5.1/types_aiobotocore_connect/__init__.pyi` & `types-aiobotocore-connect-2.5.2/types_aiobotocore_connect/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-connect-2.5.1/types_aiobotocore_connect/__main__.py` & `types-aiobotocore-connect-2.5.2/types_aiobotocore_connect/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.Connect 2.5.1\nVersion:         2.5.1\nBuilder version:"
+        "Type annotations for aiobotocore.Connect 2.5.2\nVersion:         2.5.2\nBuilder version:"
         " 7.14.5\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect//\nBoto3 docs:"
         "     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect\nOther"
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

### Comparing `types-aiobotocore-connect-2.5.1/types_aiobotocore_connect/client.py` & `types-aiobotocore-connect-2.5.2/types_aiobotocore_connect/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-connect-2.5.1/types_aiobotocore_connect/client.pyi` & `types-aiobotocore-connect-2.5.2/types_aiobotocore_connect/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-connect-2.5.1/types_aiobotocore_connect/literals.py` & `types-aiobotocore-connect-2.5.2/types_aiobotocore_connect/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-connect-2.5.1/types_aiobotocore_connect/literals.pyi` & `types-aiobotocore-connect-2.5.2/types_aiobotocore_connect/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-connect-2.5.1/types_aiobotocore_connect/paginator.py` & `types-aiobotocore-connect-2.5.2/types_aiobotocore_connect/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-connect-2.5.1/types_aiobotocore_connect/paginator.pyi` & `types-aiobotocore-connect-2.5.2/types_aiobotocore_connect/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-connect-2.5.1/types_aiobotocore_connect/type_defs.py` & `types-aiobotocore-connect-2.5.2/types_aiobotocore_connect/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-connect-2.5.1/types_aiobotocore_connect/type_defs.pyi` & `types-aiobotocore-connect-2.5.2/types_aiobotocore_connect/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-connect-2.5.1/types_aiobotocore_connect.egg-info/PKG-INFO` & `types-aiobotocore-connect-2.5.2/types_aiobotocore_connect.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-connect
-Version: 2.5.1
-Summary: Type annotations for aiobotocore.Connect 2.5.1 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2
+Summary: Type annotations for aiobotocore.Connect 2.5.2 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-connect.svg?color=blue)](https://pypi.org/project/types-aiobotocore-connect)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-connect?color=blue)](https://pypistats.org/packages/types-aiobotocore-connect)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Connect 2.5.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect)
+[aiobotocore.Connect 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-connect-2.5.1/types_aiobotocore_connect.egg-info/SOURCES.txt` & `types-aiobotocore-connect-2.5.2/types_aiobotocore_connect.egg-info/SOURCES.txt`

 * *Files identical despite different names*

