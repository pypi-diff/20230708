# Comparing `tmp/types-aiobotocore-polly-2.5.1.tar.gz` & `tmp/types-aiobotocore-polly-2.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-polly-2.5.1.tar", last modified: Wed Jun 28 01:44:00 2023, max compression
+gzip compressed data, was "types-aiobotocore-polly-2.5.2.tar", last modified: Sat Jul  8 01:44:08 2023, max compression
```

## Comparing `types-aiobotocore-polly-2.5.1.tar` & `types-aiobotocore-polly-2.5.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 01:44:00.206194 types-aiobotocore-polly-2.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-28 01:36:51.000000 types-aiobotocore-polly-2.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14208 2023-06-28 01:44:00.206194 types-aiobotocore-polly-2.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12651 2023-06-28 01:36:51.000000 types-aiobotocore-polly-2.5.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-28 01:44:00.206194 types-aiobotocore-polly-2.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-06-28 01:36:50.000000 types-aiobotocore-polly-2.5.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 01:44:00.202194 types-aiobotocore-polly-2.5.1/types_aiobotocore_polly/
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-06-28 01:36:51.000000 types-aiobotocore-polly-2.5.1/types_aiobotocore_polly/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-06-28 01:36:51.000000 types-aiobotocore-polly-2.5.1/types_aiobotocore_polly/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-06-28 01:36:51.000000 types-aiobotocore-polly-2.5.1/types_aiobotocore_polly/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12645 2023-06-28 01:36:51.000000 types-aiobotocore-polly-2.5.1/types_aiobotocore_polly/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    12624 2023-06-28 01:36:51.000000 types-aiobotocore-polly-2.5.1/types_aiobotocore_polly/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10609 2023-06-28 01:36:51.000000 types-aiobotocore-polly-2.5.1/types_aiobotocore_polly/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10607 2023-06-28 01:36:51.000000 types-aiobotocore-polly-2.5.1/types_aiobotocore_polly/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4388 2023-06-28 01:36:51.000000 types-aiobotocore-polly-2.5.1/types_aiobotocore_polly/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4383 2023-06-28 01:36:51.000000 types-aiobotocore-polly-2.5.1/types_aiobotocore_polly/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 01:36:51.000000 types-aiobotocore-polly-2.5.1/types_aiobotocore_polly/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     8943 2023-06-28 01:36:51.000000 types-aiobotocore-polly-2.5.1/types_aiobotocore_polly/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8938 2023-06-28 01:36:51.000000 types-aiobotocore-polly-2.5.1/types_aiobotocore_polly/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-28 01:36:51.000000 types-aiobotocore-polly-2.5.1/types_aiobotocore_polly/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 01:44:00.202194 types-aiobotocore-polly-2.5.1/types_aiobotocore_polly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14208 2023-06-28 01:44:00.000000 types-aiobotocore-polly-2.5.1/types_aiobotocore_polly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-06-28 01:44:00.000000 types-aiobotocore-polly-2.5.1/types_aiobotocore_polly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 01:44:00.000000 types-aiobotocore-polly-2.5.1/types_aiobotocore_polly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 01:44:00.000000 types-aiobotocore-polly-2.5.1/types_aiobotocore_polly.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-28 01:44:00.000000 types-aiobotocore-polly-2.5.1/types_aiobotocore_polly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-28 01:44:00.000000 types-aiobotocore-polly-2.5.1/types_aiobotocore_polly.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:08.386708 types-aiobotocore-polly-2.5.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:36:43.000000 types-aiobotocore-polly-2.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14208 2023-07-08 01:44:08.386708 types-aiobotocore-polly-2.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12651 2023-07-08 01:36:43.000000 types-aiobotocore-polly-2.5.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:44:08.386708 types-aiobotocore-polly-2.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-07-08 01:36:43.000000 types-aiobotocore-polly-2.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:08.378708 types-aiobotocore-polly-2.5.2/types_aiobotocore_polly/
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-07-08 01:36:43.000000 types-aiobotocore-polly-2.5.2/types_aiobotocore_polly/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-07-08 01:36:43.000000 types-aiobotocore-polly-2.5.2/types_aiobotocore_polly/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-07-08 01:36:43.000000 types-aiobotocore-polly-2.5.2/types_aiobotocore_polly/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12645 2023-07-08 01:36:43.000000 types-aiobotocore-polly-2.5.2/types_aiobotocore_polly/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12624 2023-07-08 01:36:43.000000 types-aiobotocore-polly-2.5.2/types_aiobotocore_polly/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10609 2023-07-08 01:36:45.000000 types-aiobotocore-polly-2.5.2/types_aiobotocore_polly/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10607 2023-07-08 01:36:45.000000 types-aiobotocore-polly-2.5.2/types_aiobotocore_polly/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4388 2023-07-08 01:36:43.000000 types-aiobotocore-polly-2.5.2/types_aiobotocore_polly/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4383 2023-07-08 01:36:43.000000 types-aiobotocore-polly-2.5.2/types_aiobotocore_polly/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:36:43.000000 types-aiobotocore-polly-2.5.2/types_aiobotocore_polly/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     8943 2023-07-08 01:36:45.000000 types-aiobotocore-polly-2.5.2/types_aiobotocore_polly/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8938 2023-07-08 01:36:45.000000 types-aiobotocore-polly-2.5.2/types_aiobotocore_polly/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:36:43.000000 types-aiobotocore-polly-2.5.2/types_aiobotocore_polly/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:08.386708 types-aiobotocore-polly-2.5.2/types_aiobotocore_polly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14208 2023-07-08 01:44:08.000000 types-aiobotocore-polly-2.5.2/types_aiobotocore_polly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-08 01:44:08.000000 types-aiobotocore-polly-2.5.2/types_aiobotocore_polly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:44:08.000000 types-aiobotocore-polly-2.5.2/types_aiobotocore_polly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:44:08.000000 types-aiobotocore-polly-2.5.2/types_aiobotocore_polly.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:44:08.000000 types-aiobotocore-polly-2.5.2/types_aiobotocore_polly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-08 01:44:08.000000 types-aiobotocore-polly-2.5.2/types_aiobotocore_polly.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-polly-2.5.1/LICENSE` & `types-aiobotocore-polly-2.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-polly-2.5.1/PKG-INFO` & `types-aiobotocore-polly-2.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-polly
-Version: 2.5.1
-Summary: Type annotations for aiobotocore.Polly 2.5.1 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2
+Summary: Type annotations for aiobotocore.Polly 2.5.2 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_polly/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-polly.svg?color=blue)](https://pypi.org/project/types-aiobotocore-polly)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_polly/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-polly?color=blue)](https://pypistats.org/packages/types-aiobotocore-polly)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Polly 2.5.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/polly.html#Polly)
+[aiobotocore.Polly 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/polly.html#Polly)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-polly-2.5.1/README.md` & `types-aiobotocore-polly-2.5.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-polly.svg?color=blue)](https://pypi.org/project/types-aiobotocore-polly)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_polly/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-polly?color=blue)](https://pypistats.org/packages/types-aiobotocore-polly)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Polly 2.5.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/polly.html#Polly)
+[aiobotocore.Polly 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/polly.html#Polly)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-polly-2.5.1/setup.py` & `types-aiobotocore-polly-2.5.2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-polly",
-    version="2.5.1",
+    version="2.5.2",
     packages=["types_aiobotocore_polly"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.Polly 2.5.1 service generated with mypy-boto3-builder"
+        "Type annotations for aiobotocore.Polly 2.5.2 service generated with mypy-boto3-builder"
         " 7.14.5"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-polly-2.5.1/types_aiobotocore_polly/__init__.py` & `types-aiobotocore-polly-2.5.2/types_aiobotocore_polly/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-polly-2.5.1/types_aiobotocore_polly/__init__.pyi` & `types-aiobotocore-polly-2.5.2/types_aiobotocore_polly/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-polly-2.5.1/types_aiobotocore_polly/__main__.py` & `types-aiobotocore-polly-2.5.2/types_aiobotocore_polly/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.Polly 2.5.1\nVersion:         2.5.1\nBuilder version:"
+        "Type annotations for aiobotocore.Polly 2.5.2\nVersion:         2.5.2\nBuilder version:"
         " 7.14.5\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_polly//\nBoto3 docs:  "
         "    https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/polly.html#Polly\nOther"
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

### Comparing `types-aiobotocore-polly-2.5.1/types_aiobotocore_polly/client.py` & `types-aiobotocore-polly-2.5.2/types_aiobotocore_polly/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-polly-2.5.1/types_aiobotocore_polly/client.pyi` & `types-aiobotocore-polly-2.5.2/types_aiobotocore_polly/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-polly-2.5.1/types_aiobotocore_polly/literals.py` & `types-aiobotocore-polly-2.5.2/types_aiobotocore_polly/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-polly-2.5.1/types_aiobotocore_polly/literals.pyi` & `types-aiobotocore-polly-2.5.2/types_aiobotocore_polly/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-polly-2.5.1/types_aiobotocore_polly/paginator.py` & `types-aiobotocore-polly-2.5.2/types_aiobotocore_polly/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-polly-2.5.1/types_aiobotocore_polly/paginator.pyi` & `types-aiobotocore-polly-2.5.2/types_aiobotocore_polly/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-polly-2.5.1/types_aiobotocore_polly/type_defs.py` & `types-aiobotocore-polly-2.5.2/types_aiobotocore_polly/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-polly-2.5.1/types_aiobotocore_polly/type_defs.pyi` & `types-aiobotocore-polly-2.5.2/types_aiobotocore_polly/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-polly-2.5.1/types_aiobotocore_polly.egg-info/PKG-INFO` & `types-aiobotocore-polly-2.5.2/types_aiobotocore_polly.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-polly
-Version: 2.5.1
-Summary: Type annotations for aiobotocore.Polly 2.5.1 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2
+Summary: Type annotations for aiobotocore.Polly 2.5.2 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_polly/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-polly.svg?color=blue)](https://pypi.org/project/types-aiobotocore-polly)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_polly/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-polly?color=blue)](https://pypistats.org/packages/types-aiobotocore-polly)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Polly 2.5.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/polly.html#Polly)
+[aiobotocore.Polly 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/polly.html#Polly)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-polly-2.5.1/types_aiobotocore_polly.egg-info/SOURCES.txt` & `types-aiobotocore-polly-2.5.2/types_aiobotocore_polly.egg-info/SOURCES.txt`

 * *Files identical despite different names*

