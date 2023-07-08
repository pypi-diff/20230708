# Comparing `tmp/types-aiobotocore-lex-models-2.5.1.tar.gz` & `tmp/types-aiobotocore-lex-models-2.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-lex-models-2.5.1.tar", last modified: Wed Jun 28 01:43:44 2023, max compression
+gzip compressed data, was "types-aiobotocore-lex-models-2.5.2.tar", last modified: Sat Jul  8 01:43:53 2023, max compression
```

## Comparing `types-aiobotocore-lex-models-2.5.1.tar` & `types-aiobotocore-lex-models-2.5.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 01:43:44.966166 types-aiobotocore-lex-models-2.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-28 01:33:55.000000 types-aiobotocore-lex-models-2.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    19636 2023-06-28 01:43:44.966166 types-aiobotocore-lex-models-2.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    18046 2023-06-28 01:33:55.000000 types-aiobotocore-lex-models-2.5.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-28 01:43:44.966166 types-aiobotocore-lex-models-2.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-06-28 01:33:55.000000 types-aiobotocore-lex-models-2.5.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 01:43:44.966166 types-aiobotocore-lex-models-2.5.1/types_aiobotocore_lex_models/
--rw-r--r--   0 runner    (1001) docker     (123)     2570 2023-06-28 01:33:55.000000 types-aiobotocore-lex-models-2.5.1/types_aiobotocore_lex_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-06-28 01:33:55.000000 types-aiobotocore-lex-models-2.5.1/types_aiobotocore_lex_models/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-06-28 01:33:55.000000 types-aiobotocore-lex-models-2.5.1/types_aiobotocore_lex_models/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    37384 2023-06-28 01:33:56.000000 types-aiobotocore-lex-models-2.5.1/types_aiobotocore_lex_models/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    37323 2023-06-28 01:33:56.000000 types-aiobotocore-lex-models-2.5.1/types_aiobotocore_lex_models/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11150 2023-06-28 01:33:56.000000 types-aiobotocore-lex-models-2.5.1/types_aiobotocore_lex_models/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    11148 2023-06-28 01:33:56.000000 types-aiobotocore-lex-models-2.5.1/types_aiobotocore_lex_models/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12687 2023-06-28 01:33:56.000000 types-aiobotocore-lex-models-2.5.1/types_aiobotocore_lex_models/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    12675 2023-06-28 01:33:56.000000 types-aiobotocore-lex-models-2.5.1/types_aiobotocore_lex_models/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 01:33:55.000000 types-aiobotocore-lex-models-2.5.1/types_aiobotocore_lex_models/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    46093 2023-06-28 01:33:57.000000 types-aiobotocore-lex-models-2.5.1/types_aiobotocore_lex_models/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    46040 2023-06-28 01:33:56.000000 types-aiobotocore-lex-models-2.5.1/types_aiobotocore_lex_models/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-28 01:33:55.000000 types-aiobotocore-lex-models-2.5.1/types_aiobotocore_lex_models/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 01:43:44.966166 types-aiobotocore-lex-models-2.5.1/types_aiobotocore_lex_models.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19636 2023-06-28 01:43:44.000000 types-aiobotocore-lex-models-2.5.1/types_aiobotocore_lex_models.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-06-28 01:43:44.000000 types-aiobotocore-lex-models-2.5.1/types_aiobotocore_lex_models.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 01:43:44.000000 types-aiobotocore-lex-models-2.5.1/types_aiobotocore_lex_models.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 01:43:44.000000 types-aiobotocore-lex-models-2.5.1/types_aiobotocore_lex_models.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-28 01:43:44.000000 types-aiobotocore-lex-models-2.5.1/types_aiobotocore_lex_models.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-28 01:43:44.000000 types-aiobotocore-lex-models-2.5.1/types_aiobotocore_lex_models.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:53.338427 types-aiobotocore-lex-models-2.5.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:33:44.000000 types-aiobotocore-lex-models-2.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    19636 2023-07-08 01:43:53.330427 types-aiobotocore-lex-models-2.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    18046 2023-07-08 01:33:44.000000 types-aiobotocore-lex-models-2.5.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:43:53.338427 types-aiobotocore-lex-models-2.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-07-08 01:33:43.000000 types-aiobotocore-lex-models-2.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:53.330427 types-aiobotocore-lex-models-2.5.2/types_aiobotocore_lex_models/
+-rw-r--r--   0 runner    (1001) docker     (123)     2570 2023-07-08 01:33:44.000000 types-aiobotocore-lex-models-2.5.2/types_aiobotocore_lex_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-07-08 01:33:44.000000 types-aiobotocore-lex-models-2.5.2/types_aiobotocore_lex_models/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-07-08 01:33:44.000000 types-aiobotocore-lex-models-2.5.2/types_aiobotocore_lex_models/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37384 2023-07-08 01:33:44.000000 types-aiobotocore-lex-models-2.5.2/types_aiobotocore_lex_models/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37323 2023-07-08 01:33:44.000000 types-aiobotocore-lex-models-2.5.2/types_aiobotocore_lex_models/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11150 2023-07-08 01:33:44.000000 types-aiobotocore-lex-models-2.5.2/types_aiobotocore_lex_models/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11148 2023-07-08 01:33:44.000000 types-aiobotocore-lex-models-2.5.2/types_aiobotocore_lex_models/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12687 2023-07-08 01:33:44.000000 types-aiobotocore-lex-models-2.5.2/types_aiobotocore_lex_models/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12675 2023-07-08 01:33:44.000000 types-aiobotocore-lex-models-2.5.2/types_aiobotocore_lex_models/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:33:44.000000 types-aiobotocore-lex-models-2.5.2/types_aiobotocore_lex_models/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    46093 2023-07-08 01:33:45.000000 types-aiobotocore-lex-models-2.5.2/types_aiobotocore_lex_models/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46040 2023-07-08 01:33:45.000000 types-aiobotocore-lex-models-2.5.2/types_aiobotocore_lex_models/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:33:44.000000 types-aiobotocore-lex-models-2.5.2/types_aiobotocore_lex_models/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:53.330427 types-aiobotocore-lex-models-2.5.2/types_aiobotocore_lex_models.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19636 2023-07-08 01:43:53.000000 types-aiobotocore-lex-models-2.5.2/types_aiobotocore_lex_models.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-07-08 01:43:53.000000 types-aiobotocore-lex-models-2.5.2/types_aiobotocore_lex_models.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:53.000000 types-aiobotocore-lex-models-2.5.2/types_aiobotocore_lex_models.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:53.000000 types-aiobotocore-lex-models-2.5.2/types_aiobotocore_lex_models.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:43:53.000000 types-aiobotocore-lex-models-2.5.2/types_aiobotocore_lex_models.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-08 01:43:53.000000 types-aiobotocore-lex-models-2.5.2/types_aiobotocore_lex_models.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-lex-models-2.5.1/LICENSE` & `types-aiobotocore-lex-models-2.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-lex-models-2.5.1/PKG-INFO` & `types-aiobotocore-lex-models-2.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-lex-models
-Version: 2.5.1
-Summary: Type annotations for aiobotocore.LexModelBuildingService 2.5.1 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2
+Summary: Type annotations for aiobotocore.LexModelBuildingService 2.5.2 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lex_models/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-lex-models.svg?color=blue)](https://pypi.org/project/types-aiobotocore-lex-models)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lex_models/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-lex-models?color=blue)](https://pypistats.org/packages/types-aiobotocore-lex-models)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.LexModelBuildingService 2.5.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService)
+[aiobotocore.LexModelBuildingService 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-lex-models-2.5.1/README.md` & `types-aiobotocore-lex-models-2.5.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-lex-models.svg?color=blue)](https://pypi.org/project/types-aiobotocore-lex-models)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lex_models/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-lex-models?color=blue)](https://pypistats.org/packages/types-aiobotocore-lex-models)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.LexModelBuildingService 2.5.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService)
+[aiobotocore.LexModelBuildingService 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-lex-models-2.5.1/setup.py` & `types-aiobotocore-lex-models-2.5.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-lex-models",
-    version="2.5.1",
+    version="2.5.2",
     packages=["types_aiobotocore_lex_models"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.LexModelBuildingService 2.5.1 service generated with"
+        "Type annotations for aiobotocore.LexModelBuildingService 2.5.2 service generated with"
         " mypy-boto3-builder 7.14.5"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-lex-models-2.5.1/types_aiobotocore_lex_models/__init__.py` & `types-aiobotocore-lex-models-2.5.2/types_aiobotocore_lex_models/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-lex-models-2.5.1/types_aiobotocore_lex_models/__init__.pyi` & `types-aiobotocore-lex-models-2.5.2/types_aiobotocore_lex_models/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-lex-models-2.5.1/types_aiobotocore_lex_models/client.py` & `types-aiobotocore-lex-models-2.5.2/types_aiobotocore_lex_models/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-lex-models-2.5.1/types_aiobotocore_lex_models/client.pyi` & `types-aiobotocore-lex-models-2.5.2/types_aiobotocore_lex_models/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-lex-models-2.5.1/types_aiobotocore_lex_models/literals.py` & `types-aiobotocore-lex-models-2.5.2/types_aiobotocore_lex_models/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-lex-models-2.5.1/types_aiobotocore_lex_models/literals.pyi` & `types-aiobotocore-lex-models-2.5.2/types_aiobotocore_lex_models/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-lex-models-2.5.1/types_aiobotocore_lex_models/paginator.py` & `types-aiobotocore-lex-models-2.5.2/types_aiobotocore_lex_models/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-lex-models-2.5.1/types_aiobotocore_lex_models/paginator.pyi` & `types-aiobotocore-lex-models-2.5.2/types_aiobotocore_lex_models/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-lex-models-2.5.1/types_aiobotocore_lex_models/type_defs.py` & `types-aiobotocore-lex-models-2.5.2/types_aiobotocore_lex_models/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-lex-models-2.5.1/types_aiobotocore_lex_models/type_defs.pyi` & `types-aiobotocore-lex-models-2.5.2/types_aiobotocore_lex_models/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-lex-models-2.5.1/types_aiobotocore_lex_models.egg-info/PKG-INFO` & `types-aiobotocore-lex-models-2.5.2/types_aiobotocore_lex_models.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-lex-models
-Version: 2.5.1
-Summary: Type annotations for aiobotocore.LexModelBuildingService 2.5.1 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2
+Summary: Type annotations for aiobotocore.LexModelBuildingService 2.5.2 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lex_models/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-lex-models.svg?color=blue)](https://pypi.org/project/types-aiobotocore-lex-models)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lex_models/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-lex-models?color=blue)](https://pypistats.org/packages/types-aiobotocore-lex-models)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.LexModelBuildingService 2.5.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService)
+[aiobotocore.LexModelBuildingService 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-lex-models-2.5.1/types_aiobotocore_lex_models.egg-info/SOURCES.txt` & `types-aiobotocore-lex-models-2.5.2/types_aiobotocore_lex_models.egg-info/SOURCES.txt`

 * *Files identical despite different names*

