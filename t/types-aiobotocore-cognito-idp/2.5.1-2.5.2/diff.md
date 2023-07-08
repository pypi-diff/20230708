# Comparing `tmp/types-aiobotocore-cognito-idp-2.5.1.tar.gz` & `tmp/types-aiobotocore-cognito-idp-2.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-cognito-idp-2.5.1.tar", last modified: Wed Jun 28 01:43:18 2023, max compression
+gzip compressed data, was "types-aiobotocore-cognito-idp-2.5.2.tar", last modified: Sat Jul  8 01:43:26 2023, max compression
```

## Comparing `types-aiobotocore-cognito-idp-2.5.1.tar` & `types-aiobotocore-cognito-idp-2.5.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 01:43:18.010115 types-aiobotocore-cognito-idp-2.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-28 01:28:09.000000 types-aiobotocore-cognito-idp-2.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    25561 2023-06-28 01:43:18.010115 types-aiobotocore-cognito-idp-2.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    23968 2023-06-28 01:28:09.000000 types-aiobotocore-cognito-idp-2.5.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-28 01:43:18.010115 types-aiobotocore-cognito-idp-2.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-06-28 01:28:09.000000 types-aiobotocore-cognito-idp-2.5.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 01:43:18.002115 types-aiobotocore-cognito-idp-2.5.1/types_aiobotocore_cognito_idp/
--rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-06-28 01:28:09.000000 types-aiobotocore-cognito-idp-2.5.1/types_aiobotocore_cognito_idp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-06-28 01:28:09.000000 types-aiobotocore-cognito-idp-2.5.1/types_aiobotocore_cognito_idp/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-06-28 01:28:09.000000 types-aiobotocore-cognito-idp-2.5.1/types_aiobotocore_cognito_idp/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    82577 2023-06-28 01:28:09.000000 types-aiobotocore-cognito-idp-2.5.1/types_aiobotocore_cognito_idp/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    82458 2023-06-28 01:28:09.000000 types-aiobotocore-cognito-idp-2.5.1/types_aiobotocore_cognito_idp/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    13626 2023-06-28 01:28:10.000000 types-aiobotocore-cognito-idp-2.5.1/types_aiobotocore_cognito_idp/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    13624 2023-06-28 01:28:10.000000 types-aiobotocore-cognito-idp-2.5.1/types_aiobotocore_cognito_idp/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11591 2023-06-28 01:28:09.000000 types-aiobotocore-cognito-idp-2.5.1/types_aiobotocore_cognito_idp/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    11580 2023-06-28 01:28:09.000000 types-aiobotocore-cognito-idp-2.5.1/types_aiobotocore_cognito_idp/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 01:28:09.000000 types-aiobotocore-cognito-idp-2.5.1/types_aiobotocore_cognito_idp/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    97467 2023-06-28 01:28:12.000000 types-aiobotocore-cognito-idp-2.5.1/types_aiobotocore_cognito_idp/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    97328 2023-06-28 01:28:11.000000 types-aiobotocore-cognito-idp-2.5.1/types_aiobotocore_cognito_idp/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-28 01:28:09.000000 types-aiobotocore-cognito-idp-2.5.1/types_aiobotocore_cognito_idp/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 01:43:18.010115 types-aiobotocore-cognito-idp-2.5.1/types_aiobotocore_cognito_idp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    25561 2023-06-28 01:43:17.000000 types-aiobotocore-cognito-idp-2.5.1/types_aiobotocore_cognito_idp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-06-28 01:43:17.000000 types-aiobotocore-cognito-idp-2.5.1/types_aiobotocore_cognito_idp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 01:43:17.000000 types-aiobotocore-cognito-idp-2.5.1/types_aiobotocore_cognito_idp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 01:43:17.000000 types-aiobotocore-cognito-idp-2.5.1/types_aiobotocore_cognito_idp.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-28 01:43:17.000000 types-aiobotocore-cognito-idp-2.5.1/types_aiobotocore_cognito_idp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-28 01:43:17.000000 types-aiobotocore-cognito-idp-2.5.1/types_aiobotocore_cognito_idp.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:26.137913 types-aiobotocore-cognito-idp-2.5.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:27:45.000000 types-aiobotocore-cognito-idp-2.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    25561 2023-07-08 01:43:26.133913 types-aiobotocore-cognito-idp-2.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    23968 2023-07-08 01:27:45.000000 types-aiobotocore-cognito-idp-2.5.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:43:26.137913 types-aiobotocore-cognito-idp-2.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-07-08 01:27:45.000000 types-aiobotocore-cognito-idp-2.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:26.129913 types-aiobotocore-cognito-idp-2.5.2/types_aiobotocore_cognito_idp/
+-rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-07-08 01:27:45.000000 types-aiobotocore-cognito-idp-2.5.2/types_aiobotocore_cognito_idp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-07-08 01:27:45.000000 types-aiobotocore-cognito-idp-2.5.2/types_aiobotocore_cognito_idp/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-07-08 01:27:45.000000 types-aiobotocore-cognito-idp-2.5.2/types_aiobotocore_cognito_idp/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    82577 2023-07-08 01:27:47.000000 types-aiobotocore-cognito-idp-2.5.2/types_aiobotocore_cognito_idp/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    82458 2023-07-08 01:27:46.000000 types-aiobotocore-cognito-idp-2.5.2/types_aiobotocore_cognito_idp/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    13626 2023-07-08 01:27:47.000000 types-aiobotocore-cognito-idp-2.5.2/types_aiobotocore_cognito_idp/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13624 2023-07-08 01:27:47.000000 types-aiobotocore-cognito-idp-2.5.2/types_aiobotocore_cognito_idp/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11591 2023-07-08 01:27:47.000000 types-aiobotocore-cognito-idp-2.5.2/types_aiobotocore_cognito_idp/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11580 2023-07-08 01:27:47.000000 types-aiobotocore-cognito-idp-2.5.2/types_aiobotocore_cognito_idp/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:27:45.000000 types-aiobotocore-cognito-idp-2.5.2/types_aiobotocore_cognito_idp/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    97467 2023-07-08 01:27:50.000000 types-aiobotocore-cognito-idp-2.5.2/types_aiobotocore_cognito_idp/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    97328 2023-07-08 01:27:48.000000 types-aiobotocore-cognito-idp-2.5.2/types_aiobotocore_cognito_idp/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:27:45.000000 types-aiobotocore-cognito-idp-2.5.2/types_aiobotocore_cognito_idp/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:26.133913 types-aiobotocore-cognito-idp-2.5.2/types_aiobotocore_cognito_idp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    25561 2023-07-08 01:43:25.000000 types-aiobotocore-cognito-idp-2.5.2/types_aiobotocore_cognito_idp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-07-08 01:43:25.000000 types-aiobotocore-cognito-idp-2.5.2/types_aiobotocore_cognito_idp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:25.000000 types-aiobotocore-cognito-idp-2.5.2/types_aiobotocore_cognito_idp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:25.000000 types-aiobotocore-cognito-idp-2.5.2/types_aiobotocore_cognito_idp.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:43:25.000000 types-aiobotocore-cognito-idp-2.5.2/types_aiobotocore_cognito_idp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-08 01:43:25.000000 types-aiobotocore-cognito-idp-2.5.2/types_aiobotocore_cognito_idp.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-cognito-idp-2.5.1/LICENSE` & `types-aiobotocore-cognito-idp-2.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cognito-idp-2.5.1/PKG-INFO` & `types-aiobotocore-cognito-idp-2.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-cognito-idp
-Version: 2.5.1
-Summary: Type annotations for aiobotocore.CognitoIdentityProvider 2.5.1 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2
+Summary: Type annotations for aiobotocore.CognitoIdentityProvider 2.5.2 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_idp/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-cognito-idp.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cognito-idp)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_idp/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-cognito-idp?color=blue)](https://pypistats.org/packages/types-aiobotocore-cognito-idp)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.CognitoIdentityProvider 2.5.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider)
+[aiobotocore.CognitoIdentityProvider 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-cognito-idp-2.5.1/README.md` & `types-aiobotocore-cognito-idp-2.5.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-cognito-idp.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cognito-idp)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_idp/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-cognito-idp?color=blue)](https://pypistats.org/packages/types-aiobotocore-cognito-idp)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.CognitoIdentityProvider 2.5.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider)
+[aiobotocore.CognitoIdentityProvider 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-cognito-idp-2.5.1/setup.py` & `types-aiobotocore-cognito-idp-2.5.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-cognito-idp",
-    version="2.5.1",
+    version="2.5.2",
     packages=["types_aiobotocore_cognito_idp"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.CognitoIdentityProvider 2.5.1 service generated with"
+        "Type annotations for aiobotocore.CognitoIdentityProvider 2.5.2 service generated with"
         " mypy-boto3-builder 7.14.5"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-cognito-idp-2.5.1/types_aiobotocore_cognito_idp/__init__.py` & `types-aiobotocore-cognito-idp-2.5.2/types_aiobotocore_cognito_idp/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cognito-idp-2.5.1/types_aiobotocore_cognito_idp/__init__.pyi` & `types-aiobotocore-cognito-idp-2.5.2/types_aiobotocore_cognito_idp/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cognito-idp-2.5.1/types_aiobotocore_cognito_idp/__main__.py` & `types-aiobotocore-cognito-idp-2.5.2/types_aiobotocore_cognito_idp/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.CognitoIdentityProvider 2.5.1\nVersion:        "
-        " 2.5.1\nBuilder version: 7.14.5\nDocs:           "
+        "Type annotations for aiobotocore.CognitoIdentityProvider 2.5.2\nVersion:        "
+        " 2.5.2\nBuilder version: 7.14.5\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_idp//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider\nOther"
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

### Comparing `types-aiobotocore-cognito-idp-2.5.1/types_aiobotocore_cognito_idp/client.py` & `types-aiobotocore-cognito-idp-2.5.2/types_aiobotocore_cognito_idp/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cognito-idp-2.5.1/types_aiobotocore_cognito_idp/client.pyi` & `types-aiobotocore-cognito-idp-2.5.2/types_aiobotocore_cognito_idp/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cognito-idp-2.5.1/types_aiobotocore_cognito_idp/literals.py` & `types-aiobotocore-cognito-idp-2.5.2/types_aiobotocore_cognito_idp/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cognito-idp-2.5.1/types_aiobotocore_cognito_idp/literals.pyi` & `types-aiobotocore-cognito-idp-2.5.2/types_aiobotocore_cognito_idp/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cognito-idp-2.5.1/types_aiobotocore_cognito_idp/paginator.py` & `types-aiobotocore-cognito-idp-2.5.2/types_aiobotocore_cognito_idp/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cognito-idp-2.5.1/types_aiobotocore_cognito_idp/paginator.pyi` & `types-aiobotocore-cognito-idp-2.5.2/types_aiobotocore_cognito_idp/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cognito-idp-2.5.1/types_aiobotocore_cognito_idp/type_defs.py` & `types-aiobotocore-cognito-idp-2.5.2/types_aiobotocore_cognito_idp/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cognito-idp-2.5.1/types_aiobotocore_cognito_idp/type_defs.pyi` & `types-aiobotocore-cognito-idp-2.5.2/types_aiobotocore_cognito_idp/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cognito-idp-2.5.1/types_aiobotocore_cognito_idp.egg-info/PKG-INFO` & `types-aiobotocore-cognito-idp-2.5.2/types_aiobotocore_cognito_idp.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-cognito-idp
-Version: 2.5.1
-Summary: Type annotations for aiobotocore.CognitoIdentityProvider 2.5.1 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2
+Summary: Type annotations for aiobotocore.CognitoIdentityProvider 2.5.2 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_idp/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-cognito-idp.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cognito-idp)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_idp/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-cognito-idp?color=blue)](https://pypistats.org/packages/types-aiobotocore-cognito-idp)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.CognitoIdentityProvider 2.5.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider)
+[aiobotocore.CognitoIdentityProvider 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-cognito-idp-2.5.1/types_aiobotocore_cognito_idp.egg-info/SOURCES.txt` & `types-aiobotocore-cognito-idp-2.5.2/types_aiobotocore_cognito_idp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

