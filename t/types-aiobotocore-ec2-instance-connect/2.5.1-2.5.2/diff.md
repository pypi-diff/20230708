# Comparing `tmp/types-aiobotocore-ec2-instance-connect-2.5.1.tar.gz` & `tmp/types-aiobotocore-ec2-instance-connect-2.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-ec2-instance-connect-2.5.1.tar", last modified: Wed Jun 28 01:43:24 2023, max compression
+gzip compressed data, was "types-aiobotocore-ec2-instance-connect-2.5.2.tar", last modified: Sat Jul  8 01:43:33 2023, max compression
```

## Comparing `types-aiobotocore-ec2-instance-connect-2.5.1.tar` & `types-aiobotocore-ec2-instance-connect-2.5.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 01:43:24.942128 types-aiobotocore-ec2-instance-connect-2.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-28 01:30:21.000000 types-aiobotocore-ec2-instance-connect-2.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    12860 2023-06-28 01:43:24.938128 types-aiobotocore-ec2-instance-connect-2.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11245 2023-06-28 01:30:21.000000 types-aiobotocore-ec2-instance-connect-2.5.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-28 01:43:24.942128 types-aiobotocore-ec2-instance-connect-2.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-06-28 01:30:21.000000 types-aiobotocore-ec2-instance-connect-2.5.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 01:43:24.930128 types-aiobotocore-ec2-instance-connect-2.5.1/types_aiobotocore_ec2_instance_connect/
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-06-28 01:30:21.000000 types-aiobotocore-ec2-instance-connect-2.5.1/types_aiobotocore_ec2_instance_connect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-06-28 01:30:21.000000 types-aiobotocore-ec2-instance-connect-2.5.1/types_aiobotocore_ec2_instance_connect/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-06-28 01:30:21.000000 types-aiobotocore-ec2-instance-connect-2.5.1/types_aiobotocore_ec2_instance_connect/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6245 2023-06-28 01:30:21.000000 types-aiobotocore-ec2-instance-connect-2.5.1/types_aiobotocore_ec2_instance_connect/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     6235 2023-06-28 01:30:21.000000 types-aiobotocore-ec2-instance-connect-2.5.1/types_aiobotocore_ec2_instance_connect/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7614 2023-06-28 01:30:21.000000 types-aiobotocore-ec2-instance-connect-2.5.1/types_aiobotocore_ec2_instance_connect/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     7612 2023-06-28 01:30:21.000000 types-aiobotocore-ec2-instance-connect-2.5.1/types_aiobotocore_ec2_instance_connect/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 01:30:21.000000 types-aiobotocore-ec2-instance-connect-2.5.1/types_aiobotocore_ec2_instance_connect/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     2593 2023-06-28 01:30:21.000000 types-aiobotocore-ec2-instance-connect-2.5.1/types_aiobotocore_ec2_instance_connect/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2588 2023-06-28 01:30:21.000000 types-aiobotocore-ec2-instance-connect-2.5.1/types_aiobotocore_ec2_instance_connect/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-28 01:30:21.000000 types-aiobotocore-ec2-instance-connect-2.5.1/types_aiobotocore_ec2_instance_connect/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 01:43:24.938128 types-aiobotocore-ec2-instance-connect-2.5.1/types_aiobotocore_ec2_instance_connect.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12860 2023-06-28 01:43:24.000000 types-aiobotocore-ec2-instance-connect-2.5.1/types_aiobotocore_ec2_instance_connect.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-06-28 01:43:24.000000 types-aiobotocore-ec2-instance-connect-2.5.1/types_aiobotocore_ec2_instance_connect.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 01:43:24.000000 types-aiobotocore-ec2-instance-connect-2.5.1/types_aiobotocore_ec2_instance_connect.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 01:43:24.000000 types-aiobotocore-ec2-instance-connect-2.5.1/types_aiobotocore_ec2_instance_connect.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-28 01:43:24.000000 types-aiobotocore-ec2-instance-connect-2.5.1/types_aiobotocore_ec2_instance_connect.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-28 01:43:24.000000 types-aiobotocore-ec2-instance-connect-2.5.1/types_aiobotocore_ec2_instance_connect.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:33.158047 types-aiobotocore-ec2-instance-connect-2.5.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:30:03.000000 types-aiobotocore-ec2-instance-connect-2.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12860 2023-07-08 01:43:33.158047 types-aiobotocore-ec2-instance-connect-2.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11245 2023-07-08 01:30:03.000000 types-aiobotocore-ec2-instance-connect-2.5.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:43:33.158047 types-aiobotocore-ec2-instance-connect-2.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-07-08 01:30:03.000000 types-aiobotocore-ec2-instance-connect-2.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:33.158047 types-aiobotocore-ec2-instance-connect-2.5.2/types_aiobotocore_ec2_instance_connect/
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-07-08 01:30:03.000000 types-aiobotocore-ec2-instance-connect-2.5.2/types_aiobotocore_ec2_instance_connect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-07-08 01:30:03.000000 types-aiobotocore-ec2-instance-connect-2.5.2/types_aiobotocore_ec2_instance_connect/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-07-08 01:30:03.000000 types-aiobotocore-ec2-instance-connect-2.5.2/types_aiobotocore_ec2_instance_connect/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6245 2023-07-08 01:30:03.000000 types-aiobotocore-ec2-instance-connect-2.5.2/types_aiobotocore_ec2_instance_connect/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6235 2023-07-08 01:30:03.000000 types-aiobotocore-ec2-instance-connect-2.5.2/types_aiobotocore_ec2_instance_connect/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7614 2023-07-08 01:30:03.000000 types-aiobotocore-ec2-instance-connect-2.5.2/types_aiobotocore_ec2_instance_connect/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7612 2023-07-08 01:30:03.000000 types-aiobotocore-ec2-instance-connect-2.5.2/types_aiobotocore_ec2_instance_connect/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:30:03.000000 types-aiobotocore-ec2-instance-connect-2.5.2/types_aiobotocore_ec2_instance_connect/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     2593 2023-07-08 01:30:03.000000 types-aiobotocore-ec2-instance-connect-2.5.2/types_aiobotocore_ec2_instance_connect/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2588 2023-07-08 01:30:03.000000 types-aiobotocore-ec2-instance-connect-2.5.2/types_aiobotocore_ec2_instance_connect/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:30:03.000000 types-aiobotocore-ec2-instance-connect-2.5.2/types_aiobotocore_ec2_instance_connect/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:33.158047 types-aiobotocore-ec2-instance-connect-2.5.2/types_aiobotocore_ec2_instance_connect.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12860 2023-07-08 01:43:33.000000 types-aiobotocore-ec2-instance-connect-2.5.2/types_aiobotocore_ec2_instance_connect.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-07-08 01:43:33.000000 types-aiobotocore-ec2-instance-connect-2.5.2/types_aiobotocore_ec2_instance_connect.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:33.000000 types-aiobotocore-ec2-instance-connect-2.5.2/types_aiobotocore_ec2_instance_connect.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:33.000000 types-aiobotocore-ec2-instance-connect-2.5.2/types_aiobotocore_ec2_instance_connect.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:43:33.000000 types-aiobotocore-ec2-instance-connect-2.5.2/types_aiobotocore_ec2_instance_connect.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-08 01:43:33.000000 types-aiobotocore-ec2-instance-connect-2.5.2/types_aiobotocore_ec2_instance_connect.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-ec2-instance-connect-2.5.1/LICENSE` & `types-aiobotocore-ec2-instance-connect-2.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ec2-instance-connect-2.5.1/PKG-INFO` & `types-aiobotocore-ec2-instance-connect-2.5.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-ec2-instance-connect
-Version: 2.5.1
-Summary: Type annotations for aiobotocore.EC2InstanceConnect 2.5.1 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2
+Summary: Type annotations for aiobotocore.EC2InstanceConnect 2.5.2 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2_instance_connect/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-ec2-instance-connect.svg?color=blue)](https://pypi.org/project/types-aiobotocore-ec2-instance-connect)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2_instance_connect/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-ec2-instance-connect?color=blue)](https://pypistats.org/packages/types-aiobotocore-ec2-instance-connect)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.EC2InstanceConnect 2.5.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2-instance-connect.html#EC2InstanceConnect)
+[aiobotocore.EC2InstanceConnect 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2-instance-connect.html#EC2InstanceConnect)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-ec2-instance-connect-2.5.1/README.md` & `types-aiobotocore-ec2-instance-connect-2.5.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-ec2-instance-connect.svg?color=blue)](https://pypi.org/project/types-aiobotocore-ec2-instance-connect)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2_instance_connect/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-ec2-instance-connect?color=blue)](https://pypistats.org/packages/types-aiobotocore-ec2-instance-connect)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.EC2InstanceConnect 2.5.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2-instance-connect.html#EC2InstanceConnect)
+[aiobotocore.EC2InstanceConnect 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2-instance-connect.html#EC2InstanceConnect)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-ec2-instance-connect-2.5.1/setup.py` & `types-aiobotocore-ec2-instance-connect-2.5.2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-ec2-instance-connect",
-    version="2.5.1",
+    version="2.5.2",
     packages=["types_aiobotocore_ec2_instance_connect"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.EC2InstanceConnect 2.5.1 service generated with"
+        "Type annotations for aiobotocore.EC2InstanceConnect 2.5.2 service generated with"
         " mypy-boto3-builder 7.14.5"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-ec2-instance-connect-2.5.1/types_aiobotocore_ec2_instance_connect/__init__.py` & `types-aiobotocore-ec2-instance-connect-2.5.2/types_aiobotocore_ec2_instance_connect/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ec2-instance-connect-2.5.1/types_aiobotocore_ec2_instance_connect/__init__.pyi` & `types-aiobotocore-ec2-instance-connect-2.5.2/types_aiobotocore_ec2_instance_connect/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ec2-instance-connect-2.5.1/types_aiobotocore_ec2_instance_connect/__main__.py` & `types-aiobotocore-ec2-instance-connect-2.5.2/types_aiobotocore_ec2_instance_connect/__main__.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.EC2InstanceConnect 2.5.1\nVersion:         2.5.1\nBuilder"
+        "Type annotations for aiobotocore.EC2InstanceConnect 2.5.2\nVersion:         2.5.2\nBuilder"
         " version: 7.14.5\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2_instance_connect//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2-instance-connect.html#EC2InstanceConnect\nOther"
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

### Comparing `types-aiobotocore-ec2-instance-connect-2.5.1/types_aiobotocore_ec2_instance_connect/client.py` & `types-aiobotocore-ec2-instance-connect-2.5.2/types_aiobotocore_ec2_instance_connect/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ec2-instance-connect-2.5.1/types_aiobotocore_ec2_instance_connect/client.pyi` & `types-aiobotocore-ec2-instance-connect-2.5.2/types_aiobotocore_ec2_instance_connect/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ec2-instance-connect-2.5.1/types_aiobotocore_ec2_instance_connect/literals.py` & `types-aiobotocore-ec2-instance-connect-2.5.2/types_aiobotocore_ec2_instance_connect/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ec2-instance-connect-2.5.1/types_aiobotocore_ec2_instance_connect/literals.pyi` & `types-aiobotocore-ec2-instance-connect-2.5.2/types_aiobotocore_ec2_instance_connect/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ec2-instance-connect-2.5.1/types_aiobotocore_ec2_instance_connect/type_defs.py` & `types-aiobotocore-ec2-instance-connect-2.5.2/types_aiobotocore_ec2_instance_connect/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ec2-instance-connect-2.5.1/types_aiobotocore_ec2_instance_connect/type_defs.pyi` & `types-aiobotocore-ec2-instance-connect-2.5.2/types_aiobotocore_ec2_instance_connect/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ec2-instance-connect-2.5.1/types_aiobotocore_ec2_instance_connect.egg-info/PKG-INFO` & `types-aiobotocore-ec2-instance-connect-2.5.2/types_aiobotocore_ec2_instance_connect.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-ec2-instance-connect
-Version: 2.5.1
-Summary: Type annotations for aiobotocore.EC2InstanceConnect 2.5.1 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2
+Summary: Type annotations for aiobotocore.EC2InstanceConnect 2.5.2 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2_instance_connect/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-ec2-instance-connect.svg?color=blue)](https://pypi.org/project/types-aiobotocore-ec2-instance-connect)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2_instance_connect/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-ec2-instance-connect?color=blue)](https://pypistats.org/packages/types-aiobotocore-ec2-instance-connect)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.EC2InstanceConnect 2.5.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2-instance-connect.html#EC2InstanceConnect)
+[aiobotocore.EC2InstanceConnect 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2-instance-connect.html#EC2InstanceConnect)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-ec2-instance-connect-2.5.1/types_aiobotocore_ec2_instance_connect.egg-info/SOURCES.txt` & `types-aiobotocore-ec2-instance-connect-2.5.2/types_aiobotocore_ec2_instance_connect.egg-info/SOURCES.txt`

 * *Files identical despite different names*

