# Comparing `tmp/types-aiobotocore-kinesis-video-media-2.5.0.post1.tar.gz` & `tmp/types-aiobotocore-kinesis-video-media-2.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-kinesis-video-media-2.5.0.post1.tar", last modified: Sat Mar 11 12:26:51 2023, max compression
+gzip compressed data, was "types-aiobotocore-kinesis-video-media-2.5.1.tar", last modified: Wed Jun 28 01:43:42 2023, max compression
```

## Comparing `types-aiobotocore-kinesis-video-media-2.5.0.post1.tar` & `types-aiobotocore-kinesis-video-media-2.5.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 12:26:51.463344 types-aiobotocore-kinesis-video-media-2.5.0.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-03-11 12:16:56.000000 types-aiobotocore-kinesis-video-media-2.5.0.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    12738 2023-03-11 12:26:51.463344 types-aiobotocore-kinesis-video-media-2.5.0.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11121 2023-03-11 12:16:56.000000 types-aiobotocore-kinesis-video-media-2.5.0.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-11 12:26:51.463344 types-aiobotocore-kinesis-video-media-2.5.0.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-03-11 12:16:56.000000 types-aiobotocore-kinesis-video-media-2.5.0.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 12:26:51.463344 types-aiobotocore-kinesis-video-media-2.5.0.post1/types_aiobotocore_kinesis_video_media/
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-03-11 12:16:56.000000 types-aiobotocore-kinesis-video-media-2.5.0.post1/types_aiobotocore_kinesis_video_media/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-03-11 12:16:56.000000 types-aiobotocore-kinesis-video-media-2.5.0.post1/types_aiobotocore_kinesis_video_media/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      987 2023-03-11 12:16:56.000000 types-aiobotocore-kinesis-video-media-2.5.0.post1/types_aiobotocore_kinesis_video_media/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5107 2023-03-11 12:16:56.000000 types-aiobotocore-kinesis-video-media-2.5.0.post1/types_aiobotocore_kinesis_video_media/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     5098 2023-03-11 12:16:56.000000 types-aiobotocore-kinesis-video-media-2.5.0.post1/types_aiobotocore_kinesis_video_media/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7928 2023-03-11 12:16:56.000000 types-aiobotocore-kinesis-video-media-2.5.0.post1/types_aiobotocore_kinesis_video_media/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     7926 2023-03-11 12:16:56.000000 types-aiobotocore-kinesis-video-media-2.5.0.post1/types_aiobotocore_kinesis_video_media/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-11 12:16:56.000000 types-aiobotocore-kinesis-video-media-2.5.0.post1/types_aiobotocore_kinesis_video_media/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-03-11 12:16:56.000000 types-aiobotocore-kinesis-video-media-2.5.0.post1/types_aiobotocore_kinesis_video_media/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-03-11 12:16:56.000000 types-aiobotocore-kinesis-video-media-2.5.0.post1/types_aiobotocore_kinesis_video_media/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-03-11 12:16:56.000000 types-aiobotocore-kinesis-video-media-2.5.0.post1/types_aiobotocore_kinesis_video_media/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 12:26:51.463344 types-aiobotocore-kinesis-video-media-2.5.0.post1/types_aiobotocore_kinesis_video_media.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12738 2023-03-11 12:26:51.000000 types-aiobotocore-kinesis-video-media-2.5.0.post1/types_aiobotocore_kinesis_video_media.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-03-11 12:26:51.000000 types-aiobotocore-kinesis-video-media-2.5.0.post1/types_aiobotocore_kinesis_video_media.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-11 12:26:51.000000 types-aiobotocore-kinesis-video-media-2.5.0.post1/types_aiobotocore_kinesis_video_media.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-11 12:26:51.000000 types-aiobotocore-kinesis-video-media-2.5.0.post1/types_aiobotocore_kinesis_video_media.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-03-11 12:26:51.000000 types-aiobotocore-kinesis-video-media-2.5.0.post1/types_aiobotocore_kinesis_video_media.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-11 12:26:51.000000 types-aiobotocore-kinesis-video-media-2.5.0.post1/types_aiobotocore_kinesis_video_media.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 01:43:42.754161 types-aiobotocore-kinesis-video-media-2.5.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-28 01:33:37.000000 types-aiobotocore-kinesis-video-media-2.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12742 2023-06-28 01:43:42.754161 types-aiobotocore-kinesis-video-media-2.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11131 2023-06-28 01:33:37.000000 types-aiobotocore-kinesis-video-media-2.5.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-28 01:43:42.754161 types-aiobotocore-kinesis-video-media-2.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-06-28 01:33:36.000000 types-aiobotocore-kinesis-video-media-2.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 01:43:42.754161 types-aiobotocore-kinesis-video-media-2.5.1/types_aiobotocore_kinesis_video_media/
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-06-28 01:33:37.000000 types-aiobotocore-kinesis-video-media-2.5.1/types_aiobotocore_kinesis_video_media/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-06-28 01:33:37.000000 types-aiobotocore-kinesis-video-media-2.5.1/types_aiobotocore_kinesis_video_media/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-06-28 01:33:37.000000 types-aiobotocore-kinesis-video-media-2.5.1/types_aiobotocore_kinesis_video_media/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5107 2023-06-28 01:33:37.000000 types-aiobotocore-kinesis-video-media-2.5.1/types_aiobotocore_kinesis_video_media/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5098 2023-06-28 01:33:37.000000 types-aiobotocore-kinesis-video-media-2.5.1/types_aiobotocore_kinesis_video_media/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8137 2023-06-28 01:33:37.000000 types-aiobotocore-kinesis-video-media-2.5.1/types_aiobotocore_kinesis_video_media/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8135 2023-06-28 01:33:37.000000 types-aiobotocore-kinesis-video-media-2.5.1/types_aiobotocore_kinesis_video_media/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 01:33:37.000000 types-aiobotocore-kinesis-video-media-2.5.1/types_aiobotocore_kinesis_video_media/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-06-28 01:33:37.000000 types-aiobotocore-kinesis-video-media-2.5.1/types_aiobotocore_kinesis_video_media/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-06-28 01:33:37.000000 types-aiobotocore-kinesis-video-media-2.5.1/types_aiobotocore_kinesis_video_media/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-28 01:33:37.000000 types-aiobotocore-kinesis-video-media-2.5.1/types_aiobotocore_kinesis_video_media/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 01:43:42.754161 types-aiobotocore-kinesis-video-media-2.5.1/types_aiobotocore_kinesis_video_media.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12742 2023-06-28 01:43:42.000000 types-aiobotocore-kinesis-video-media-2.5.1/types_aiobotocore_kinesis_video_media.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-06-28 01:43:42.000000 types-aiobotocore-kinesis-video-media-2.5.1/types_aiobotocore_kinesis_video_media.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 01:43:42.000000 types-aiobotocore-kinesis-video-media-2.5.1/types_aiobotocore_kinesis_video_media.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 01:43:42.000000 types-aiobotocore-kinesis-video-media-2.5.1/types_aiobotocore_kinesis_video_media.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-28 01:43:42.000000 types-aiobotocore-kinesis-video-media-2.5.1/types_aiobotocore_kinesis_video_media.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-28 01:43:42.000000 types-aiobotocore-kinesis-video-media-2.5.1/types_aiobotocore_kinesis_video_media.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-kinesis-video-media-2.5.0.post1/LICENSE` & `types-aiobotocore-kinesis-video-media-2.5.1/LICENSE`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2022 Vlad Emelianov
+Copyright (c) 2023 Vlad Emelianov
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `types-aiobotocore-kinesis-video-media-2.5.0.post1/PKG-INFO` & `types-aiobotocore-kinesis-video-media-2.5.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-kinesis-video-media
-Version: 2.5.0.post1
-Summary: Type annotations for aiobotocore.KinesisVideoMedia 2.5.0 service generated with mypy-boto3-builder 7.13.0
+Version: 2.5.1
+Summary: Type annotations for aiobotocore.KinesisVideoMedia 2.5.1 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesis_video_media/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,30 +33,30 @@
 
 <a id="types-aiobotocore-kinesis-video-media"></a>
 
 # types-aiobotocore-kinesis-video-media
 
 [![PyPI - types-aiobotocore-kinesis-video-media](https://img.shields.io/pypi/v/types-aiobotocore-kinesis-video-media.svg?color=blue)](https://pypi.org/project/types-aiobotocore-kinesis-video-media)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-kinesis-video-media.svg?color=blue)](https://pypi.org/project/types-aiobotocore-kinesis-video-media)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesis_video_media/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-kinesis-video-media?color=blue)](https://pypistats.org/packages/types-aiobotocore-kinesis-video-media)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.KinesisVideoMedia 2.5.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis-video-media.html#KinesisVideoMedia)
+[aiobotocore.KinesisVideoMedia 2.5.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis-video-media.html#KinesisVideoMedia)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.13.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [types-aiobotocore](https://pypi.org/project/types-aiobotocore/) page and in
 [types-aiobotocore-kinesis-video-media docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesis_video_media/).
 
 See how it helps to find and fix potential bugs:
 
@@ -291,60 +291,60 @@
 
 `types_aiobotocore_kinesis_video_media.type_defs` module contains structures
 and shapes assembled to typed dictionaries for additional type checking.
 
 ```python
 from types_aiobotocore_kinesis_video_media.type_defs import (
     StartSelectorTypeDef,
+    GetMediaOutputTypeDef,
     ResponseMetadataTypeDef,
     GetMediaInputRequestTypeDef,
-    GetMediaOutputTypeDef,
 )
 
 
 def get_structure() -> StartSelectorTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
 
 Fully automated
 [mypy-boto3-builder](https://github.com/youtype/mypy_boto3_builder) carefully
 generates type annotations for each service, patiently waiting for
-`aiobotocore` updates. It delivers a drop-in type annotations for you and makes
+`aiobotocore` updates. It delivers drop-in type annotations for you and makes
 sure that:
 
 - All available `aiobotocore` services are covered.
 - Each public class and method of every `aiobotocore` service gets valid type
-  annotations extracted from the documentation (blame `botocore` docs if types
-  are incorrect).
+  annotations extracted from `botocore` schemas.
 - Type annotations include up-to-date documentation.
 - Link to documentation is provided for every method.
 - Code is processed by [black](https://github.com/psf/black) and
   [isort](https://github.com/PyCQA/isort) for readability.
 
 <a id="what's-new"></a>
 
 ## What's new
 
 <a id="implemented-features"></a>
 
 ### Implemented features
 
-- Fully type annotated `boto3`, `botocore` and `aiobotocore` libraries
+- Fully type annotated `boto3`, `botocore`, `aiobotocore` and `aioboto3`
+  libraries
 - `mypy`, `pyright`, `VSCode`, `PyCharm`, `Sublime Text` and `Emacs`
   compatibility
 - `Client`, `ServiceResource`, `Resource`, `Waiter` `Paginator` type
   annotations for each service
 - Generated `TypeDefs` for each service
 - Generated `Literals` for each service
-- Auto discovery of types for `boto3.client` and `boto3.session` calls
-- Auto discovery of types for `session.client` and `session.session` calls
+- Auto discovery of types for `boto3.client` and `boto3.resource` calls
+- Auto discovery of types for `session.client` and `session.resource` calls
 - Auto discovery of types for `client.get_waiter` and `client.get_paginator`
   calls
 - Auto discovery of types for `ServiceResource` and `Resource` collections
 - Auto discovery of types for `aiobotocore.Session.create_client` calls
 
 <a id="latest-changes"></a>
```

### Comparing `types-aiobotocore-kinesis-video-media-2.5.0.post1/README.md` & `types-aiobotocore-kinesis-video-media-2.5.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="types-aiobotocore-kinesis-video-media"></a>
 
 # types-aiobotocore-kinesis-video-media
 
 [![PyPI - types-aiobotocore-kinesis-video-media](https://img.shields.io/pypi/v/types-aiobotocore-kinesis-video-media.svg?color=blue)](https://pypi.org/project/types-aiobotocore-kinesis-video-media)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-kinesis-video-media.svg?color=blue)](https://pypi.org/project/types-aiobotocore-kinesis-video-media)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesis_video_media/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-kinesis-video-media?color=blue)](https://pypistats.org/packages/types-aiobotocore-kinesis-video-media)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.KinesisVideoMedia 2.5.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis-video-media.html#KinesisVideoMedia)
+[aiobotocore.KinesisVideoMedia 2.5.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis-video-media.html#KinesisVideoMedia)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.13.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [types-aiobotocore](https://pypi.org/project/types-aiobotocore/) page and in
 [types-aiobotocore-kinesis-video-media docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesis_video_media/).
 
 See how it helps to find and fix potential bugs:
 
@@ -258,60 +258,60 @@
 
 `types_aiobotocore_kinesis_video_media.type_defs` module contains structures
 and shapes assembled to typed dictionaries for additional type checking.
 
 ```python
 from types_aiobotocore_kinesis_video_media.type_defs import (
     StartSelectorTypeDef,
+    GetMediaOutputTypeDef,
     ResponseMetadataTypeDef,
     GetMediaInputRequestTypeDef,
-    GetMediaOutputTypeDef,
 )
 
 
 def get_structure() -> StartSelectorTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
 
 Fully automated
 [mypy-boto3-builder](https://github.com/youtype/mypy_boto3_builder) carefully
 generates type annotations for each service, patiently waiting for
-`aiobotocore` updates. It delivers a drop-in type annotations for you and makes
+`aiobotocore` updates. It delivers drop-in type annotations for you and makes
 sure that:
 
 - All available `aiobotocore` services are covered.
 - Each public class and method of every `aiobotocore` service gets valid type
-  annotations extracted from the documentation (blame `botocore` docs if types
-  are incorrect).
+  annotations extracted from `botocore` schemas.
 - Type annotations include up-to-date documentation.
 - Link to documentation is provided for every method.
 - Code is processed by [black](https://github.com/psf/black) and
   [isort](https://github.com/PyCQA/isort) for readability.
 
 <a id="what's-new"></a>
 
 ## What's new
 
 <a id="implemented-features"></a>
 
 ### Implemented features
 
-- Fully type annotated `boto3`, `botocore` and `aiobotocore` libraries
+- Fully type annotated `boto3`, `botocore`, `aiobotocore` and `aioboto3`
+  libraries
 - `mypy`, `pyright`, `VSCode`, `PyCharm`, `Sublime Text` and `Emacs`
   compatibility
 - `Client`, `ServiceResource`, `Resource`, `Waiter` `Paginator` type
   annotations for each service
 - Generated `TypeDefs` for each service
 - Generated `Literals` for each service
-- Auto discovery of types for `boto3.client` and `boto3.session` calls
-- Auto discovery of types for `session.client` and `session.session` calls
+- Auto discovery of types for `boto3.client` and `boto3.resource` calls
+- Auto discovery of types for `session.client` and `session.resource` calls
 - Auto discovery of types for `client.get_waiter` and `client.get_paginator`
   calls
 - Auto discovery of types for `ServiceResource` and `Resource` collections
 - Auto discovery of types for `aiobotocore.Session.create_client` calls
 
 <a id="latest-changes"></a>
```

### Comparing `types-aiobotocore-kinesis-video-media-2.5.0.post1/setup.py` & `types-aiobotocore-kinesis-video-media-2.5.1/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 """
 Setup script for types-aiobotocore-kinesis-video-media.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-kinesis-video-media",
-    version="2.5.0.post1",
+    version="2.5.1",
     packages=["types_aiobotocore_kinesis_video_media"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.KinesisVideoMedia 2.5.0 service generated with"
-        " mypy-boto3-builder 7.13.0"
+        "Type annotations for aiobotocore.KinesisVideoMedia 2.5.1 service generated with"
+        " mypy-boto3-builder 7.14.5"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
@@ -48,11 +48,11 @@
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesis_video_media/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
     install_requires=[
-        "typing-extensions>=4.1.0",
+        'typing-extensions>=4.1.0; python_version<"3.9"',
     ],
     zip_safe=False,
 )
```

### Comparing `types-aiobotocore-kinesis-video-media-2.5.0.post1/types_aiobotocore_kinesis_video_media/__init__.py` & `types-aiobotocore-kinesis-video-media-2.5.1/types_aiobotocore_kinesis_video_media/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-kinesis-video-media-2.5.0.post1/types_aiobotocore_kinesis_video_media/__init__.pyi` & `types-aiobotocore-kinesis-video-media-2.5.1/types_aiobotocore_kinesis_video_media/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-kinesis-video-media-2.5.0.post1/types_aiobotocore_kinesis_video_media/__main__.py` & `types-aiobotocore-kinesis-video-media-2.5.1/types_aiobotocore_kinesis_video_media/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.KinesisVideoMedia 2.5.0\nVersion:        "
-        " 2.5.0.post1\nBuilder version: 7.13.0\nDocs:           "
+        "Type annotations for aiobotocore.KinesisVideoMedia 2.5.1\nVersion:         2.5.1\nBuilder"
+        " version: 7.14.5\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesis_video_media//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis-video-media.html#KinesisVideoMedia\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("2.5.0.post1")
+    print("2.5.1")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `types-aiobotocore-kinesis-video-media-2.5.0.post1/types_aiobotocore_kinesis_video_media/client.py` & `types-aiobotocore-kinesis-video-media-2.5.1/types_aiobotocore_kinesis_video_media/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-kinesis-video-media-2.5.0.post1/types_aiobotocore_kinesis_video_media/client.pyi` & `types-aiobotocore-kinesis-video-media-2.5.1/types_aiobotocore_kinesis_video_media/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-kinesis-video-media-2.5.0.post1/types_aiobotocore_kinesis_video_media/literals.py` & `types-aiobotocore-kinesis-video-media-2.5.1/types_aiobotocore_kinesis_video_media/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -14,24 +14,22 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "StartSelectorTypeType",
     "KinesisVideoMediaServiceName",
     "ServiceName",
     "ResourceServiceName",
     "RegionName",
 )
 
-
 StartSelectorTypeType = Literal[
     "CONTINUATION_TOKEN",
     "EARLIEST",
     "FRAGMENT_NUMBER",
     "NOW",
     "PRODUCER_TIMESTAMP",
     "SERVER_TIMESTAMP",
@@ -95,14 +93,15 @@
     "cloudwatch",
     "codeartifact",
     "codebuild",
     "codecatalyst",
     "codecommit",
     "codedeploy",
     "codeguru-reviewer",
+    "codeguru-security",
     "codeguruprofiler",
     "codepipeline",
     "codestar",
     "codestar-connections",
     "codestar-notifications",
     "cognito-identity",
     "cognito-idp",
@@ -181,14 +180,15 @@
     "honeycode",
     "iam",
     "identitystore",
     "imagebuilder",
     "importexport",
     "inspector",
     "inspector2",
+    "internetmonitor",
     "iot",
     "iot-data",
     "iot-jobs-data",
     "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
@@ -199,14 +199,15 @@
     "iotfleetwise",
     "iotsecuretunneling",
     "iotsitewise",
     "iotthingsgraph",
     "iottwinmaker",
     "iotwireless",
     "ivs",
+    "ivs-realtime",
     "ivschat",
     "kafka",
     "kafkaconnect",
     "kendra",
     "kendra-ranking",
     "keyspaces",
     "kinesis",
@@ -242,14 +243,15 @@
     "marketplace-entitlement",
     "marketplacecommerceanalytics",
     "mediaconnect",
     "mediaconvert",
     "medialive",
     "mediapackage",
     "mediapackage-vod",
+    "mediapackagev2",
     "mediastore",
     "mediastore-data",
     "mediatailor",
     "memorydb",
     "meteringmarketplace",
     "mgh",
     "mgn",
@@ -268,16 +270,19 @@
     "oam",
     "omics",
     "opensearch",
     "opensearchserverless",
     "opsworks",
     "opsworkscm",
     "organizations",
+    "osis",
     "outposts",
     "panorama",
+    "payment-cryptography",
+    "payment-cryptography-data",
     "personalize",
     "personalize-events",
     "personalize-runtime",
     "pi",
     "pinpoint",
     "pinpoint-email",
     "pinpoint-sms-voice",
@@ -361,15 +366,17 @@
     "textract",
     "timestream-query",
     "timestream-write",
     "tnb",
     "transcribe",
     "transfer",
     "translate",
+    "verifiedpermissions",
     "voice-id",
+    "vpc-lattice",
     "waf",
     "waf-regional",
     "wafv2",
     "wellarchitected",
     "wisdom",
     "workdocs",
     "worklink",
```

### Comparing `types-aiobotocore-kinesis-video-media-2.5.0.post1/types_aiobotocore_kinesis_video_media/literals.pyi` & `types-aiobotocore-kinesis-video-media-2.5.1/types_aiobotocore_kinesis_video_media/literals.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,22 +14,24 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = (
     "StartSelectorTypeType",
     "KinesisVideoMediaServiceName",
     "ServiceName",
     "ResourceServiceName",
     "RegionName",
 )
 
+
 StartSelectorTypeType = Literal[
     "CONTINUATION_TOKEN",
     "EARLIEST",
     "FRAGMENT_NUMBER",
     "NOW",
     "PRODUCER_TIMESTAMP",
     "SERVER_TIMESTAMP",
@@ -93,14 +95,15 @@
     "cloudwatch",
     "codeartifact",
     "codebuild",
     "codecatalyst",
     "codecommit",
     "codedeploy",
     "codeguru-reviewer",
+    "codeguru-security",
     "codeguruprofiler",
     "codepipeline",
     "codestar",
     "codestar-connections",
     "codestar-notifications",
     "cognito-identity",
     "cognito-idp",
@@ -179,14 +182,15 @@
     "honeycode",
     "iam",
     "identitystore",
     "imagebuilder",
     "importexport",
     "inspector",
     "inspector2",
+    "internetmonitor",
     "iot",
     "iot-data",
     "iot-jobs-data",
     "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
@@ -197,14 +201,15 @@
     "iotfleetwise",
     "iotsecuretunneling",
     "iotsitewise",
     "iotthingsgraph",
     "iottwinmaker",
     "iotwireless",
     "ivs",
+    "ivs-realtime",
     "ivschat",
     "kafka",
     "kafkaconnect",
     "kendra",
     "kendra-ranking",
     "keyspaces",
     "kinesis",
@@ -240,14 +245,15 @@
     "marketplace-entitlement",
     "marketplacecommerceanalytics",
     "mediaconnect",
     "mediaconvert",
     "medialive",
     "mediapackage",
     "mediapackage-vod",
+    "mediapackagev2",
     "mediastore",
     "mediastore-data",
     "mediatailor",
     "memorydb",
     "meteringmarketplace",
     "mgh",
     "mgn",
@@ -266,16 +272,19 @@
     "oam",
     "omics",
     "opensearch",
     "opensearchserverless",
     "opsworks",
     "opsworkscm",
     "organizations",
+    "osis",
     "outposts",
     "panorama",
+    "payment-cryptography",
+    "payment-cryptography-data",
     "personalize",
     "personalize-events",
     "personalize-runtime",
     "pi",
     "pinpoint",
     "pinpoint-email",
     "pinpoint-sms-voice",
@@ -359,15 +368,17 @@
     "textract",
     "timestream-query",
     "timestream-write",
     "tnb",
     "transcribe",
     "transfer",
     "translate",
+    "verifiedpermissions",
     "voice-id",
+    "vpc-lattice",
     "waf",
     "waf-regional",
     "wafv2",
     "wellarchitected",
     "wisdom",
     "workdocs",
     "worklink",
```

### Comparing `types-aiobotocore-kinesis-video-media-2.5.0.post1/types_aiobotocore_kinesis_video_media/type_defs.py` & `types-aiobotocore-kinesis-video-media-2.5.1/types_aiobotocore_kinesis_video_media/type_defs.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -20,20 +20,19 @@
 from .literals import StartSelectorTypeType
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "StartSelectorTypeDef",
+    "GetMediaOutputTypeDef",
     "ResponseMetadataTypeDef",
     "GetMediaInputRequestTypeDef",
-    "GetMediaOutputTypeDef",
 )
 
 _RequiredStartSelectorTypeDef = TypedDict(
     "_RequiredStartSelectorTypeDef",
     {
         "StartSelectorType": StartSelectorTypeType,
     },
@@ -44,18 +43,25 @@
         "AfterFragmentNumber": str,
         "StartTimestamp": Union[datetime, str],
         "ContinuationToken": str,
     },
     total=False,
 )
 
-
 class StartSelectorTypeDef(_RequiredStartSelectorTypeDef, _OptionalStartSelectorTypeDef):
     pass
 
+GetMediaOutputTypeDef = TypedDict(
+    "GetMediaOutputTypeDef",
+    {
+        "ContentType": str,
+        "Payload": StreamingBody,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
 
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
         "HostId": str,
         "HTTPStatusCode": int,
@@ -75,22 +81,11 @@
     {
         "StreamName": str,
         "StreamARN": str,
     },
     total=False,
 )
 
-
 class GetMediaInputRequestTypeDef(
     _RequiredGetMediaInputRequestTypeDef, _OptionalGetMediaInputRequestTypeDef
 ):
     pass
-
-
-GetMediaOutputTypeDef = TypedDict(
-    "GetMediaOutputTypeDef",
-    {
-        "ContentType": str,
-        "Payload": StreamingBody,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
```

### Comparing `types-aiobotocore-kinesis-video-media-2.5.0.post1/types_aiobotocore_kinesis_video_media/type_defs.pyi` & `types-aiobotocore-kinesis-video-media-2.5.1/types_aiobotocore_kinesis_video_media/type_defs.py`

 * *Files 12% similar despite different names*

```diff
@@ -20,19 +20,20 @@
 from .literals import StartSelectorTypeType
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "StartSelectorTypeDef",
+    "GetMediaOutputTypeDef",
     "ResponseMetadataTypeDef",
     "GetMediaInputRequestTypeDef",
-    "GetMediaOutputTypeDef",
 )
 
 _RequiredStartSelectorTypeDef = TypedDict(
     "_RequiredStartSelectorTypeDef",
     {
         "StartSelectorType": StartSelectorTypeType,
     },
@@ -43,17 +44,28 @@
         "AfterFragmentNumber": str,
         "StartTimestamp": Union[datetime, str],
         "ContinuationToken": str,
     },
     total=False,
 )
 
+
 class StartSelectorTypeDef(_RequiredStartSelectorTypeDef, _OptionalStartSelectorTypeDef):
     pass
 
+
+GetMediaOutputTypeDef = TypedDict(
+    "GetMediaOutputTypeDef",
+    {
+        "ContentType": str,
+        "Payload": StreamingBody,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
@@ -72,20 +84,12 @@
     {
         "StreamName": str,
         "StreamARN": str,
     },
     total=False,
 )
 
+
 class GetMediaInputRequestTypeDef(
     _RequiredGetMediaInputRequestTypeDef, _OptionalGetMediaInputRequestTypeDef
 ):
     pass
-
-GetMediaOutputTypeDef = TypedDict(
-    "GetMediaOutputTypeDef",
-    {
-        "ContentType": str,
-        "Payload": StreamingBody,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
```

### Comparing `types-aiobotocore-kinesis-video-media-2.5.0.post1/types_aiobotocore_kinesis_video_media.egg-info/PKG-INFO` & `types-aiobotocore-kinesis-video-media-2.5.1/types_aiobotocore_kinesis_video_media.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-kinesis-video-media
-Version: 2.5.0.post1
-Summary: Type annotations for aiobotocore.KinesisVideoMedia 2.5.0 service generated with mypy-boto3-builder 7.13.0
+Version: 2.5.1
+Summary: Type annotations for aiobotocore.KinesisVideoMedia 2.5.1 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesis_video_media/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,30 +33,30 @@
 
 <a id="types-aiobotocore-kinesis-video-media"></a>
 
 # types-aiobotocore-kinesis-video-media
 
 [![PyPI - types-aiobotocore-kinesis-video-media](https://img.shields.io/pypi/v/types-aiobotocore-kinesis-video-media.svg?color=blue)](https://pypi.org/project/types-aiobotocore-kinesis-video-media)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-kinesis-video-media.svg?color=blue)](https://pypi.org/project/types-aiobotocore-kinesis-video-media)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesis_video_media/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-kinesis-video-media?color=blue)](https://pypistats.org/packages/types-aiobotocore-kinesis-video-media)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.KinesisVideoMedia 2.5.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis-video-media.html#KinesisVideoMedia)
+[aiobotocore.KinesisVideoMedia 2.5.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis-video-media.html#KinesisVideoMedia)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.13.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [types-aiobotocore](https://pypi.org/project/types-aiobotocore/) page and in
 [types-aiobotocore-kinesis-video-media docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesis_video_media/).
 
 See how it helps to find and fix potential bugs:
 
@@ -291,60 +291,60 @@
 
 `types_aiobotocore_kinesis_video_media.type_defs` module contains structures
 and shapes assembled to typed dictionaries for additional type checking.
 
 ```python
 from types_aiobotocore_kinesis_video_media.type_defs import (
     StartSelectorTypeDef,
+    GetMediaOutputTypeDef,
     ResponseMetadataTypeDef,
     GetMediaInputRequestTypeDef,
-    GetMediaOutputTypeDef,
 )
 
 
 def get_structure() -> StartSelectorTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
 
 Fully automated
 [mypy-boto3-builder](https://github.com/youtype/mypy_boto3_builder) carefully
 generates type annotations for each service, patiently waiting for
-`aiobotocore` updates. It delivers a drop-in type annotations for you and makes
+`aiobotocore` updates. It delivers drop-in type annotations for you and makes
 sure that:
 
 - All available `aiobotocore` services are covered.
 - Each public class and method of every `aiobotocore` service gets valid type
-  annotations extracted from the documentation (blame `botocore` docs if types
-  are incorrect).
+  annotations extracted from `botocore` schemas.
 - Type annotations include up-to-date documentation.
 - Link to documentation is provided for every method.
 - Code is processed by [black](https://github.com/psf/black) and
   [isort](https://github.com/PyCQA/isort) for readability.
 
 <a id="what's-new"></a>
 
 ## What's new
 
 <a id="implemented-features"></a>
 
 ### Implemented features
 
-- Fully type annotated `boto3`, `botocore` and `aiobotocore` libraries
+- Fully type annotated `boto3`, `botocore`, `aiobotocore` and `aioboto3`
+  libraries
 - `mypy`, `pyright`, `VSCode`, `PyCharm`, `Sublime Text` and `Emacs`
   compatibility
 - `Client`, `ServiceResource`, `Resource`, `Waiter` `Paginator` type
   annotations for each service
 - Generated `TypeDefs` for each service
 - Generated `Literals` for each service
-- Auto discovery of types for `boto3.client` and `boto3.session` calls
-- Auto discovery of types for `session.client` and `session.session` calls
+- Auto discovery of types for `boto3.client` and `boto3.resource` calls
+- Auto discovery of types for `session.client` and `session.resource` calls
 - Auto discovery of types for `client.get_waiter` and `client.get_paginator`
   calls
 - Auto discovery of types for `ServiceResource` and `Resource` collections
 - Auto discovery of types for `aiobotocore.Session.create_client` calls
 
 <a id="latest-changes"></a>
```

### Comparing `types-aiobotocore-kinesis-video-media-2.5.0.post1/types_aiobotocore_kinesis_video_media.egg-info/SOURCES.txt` & `types-aiobotocore-kinesis-video-media-2.5.1/types_aiobotocore_kinesis_video_media.egg-info/SOURCES.txt`

 * *Files identical despite different names*

