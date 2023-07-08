# Comparing `tmp/pymultithreading-0.2.6.tar.gz` & `tmp/pymultithreading-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymultithreading-0.2.6.tar", last modified: Mon Jul  3 16:16:38 2023, max compression
+gzip compressed data, was "pymultithreading-1.0.0.tar", last modified: Sat Jul  8 21:11:13 2023, max compression
```

## Comparing `pymultithreading-0.2.6.tar` & `pymultithreading-1.0.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-07-03 16:16:38.221646 pymultithreading-0.2.6/
--rw-rw-rw-   0        0        0       98 2023-07-03 16:16:37.000000 pymultithreading-0.2.6/MANIFEST.in
--rw-rw-rw-   0        0        0     2019 2023-07-03 16:16:38.220647 pymultithreading-0.2.6/PKG-INFO
--rw-rw-rw-   0        0        0     1217 2023-07-01 08:57:20.000000 pymultithreading-0.2.6/README.md
--rw-rw-rw-   0        0        0    12920 2023-03-17 11:12:17.000000 pymultithreading-0.2.6/build.py
-drwxrwxrwx   0        0        0        0 2023-07-03 16:16:38.205097 pymultithreading-0.2.6/multithreading/
--rw-rw-rw-   0        0        0       53 2023-06-17 10:18:28.000000 pymultithreading-0.2.6/multithreading/__init__.py
--rw-rw-rw-   0        0        0    11708 2023-07-03 16:16:05.000000 pymultithreading-0.2.6/multithreading/process.py
-drwxrwxrwx   0        0        0        0 2023-07-03 16:16:38.219676 pymultithreading-0.2.6/pymultithreading.egg-info/
--rw-rw-rw-   0        0        0     2019 2023-07-03 16:16:38.000000 pymultithreading-0.2.6/pymultithreading.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      344 2023-07-03 16:16:38.000000 pymultithreading-0.2.6/pymultithreading.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-03 16:16:38.000000 pymultithreading-0.2.6/pymultithreading.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2023-07-03 16:16:38.000000 pymultithreading-0.2.6/pymultithreading.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-07-03 16:16:38.000000 pymultithreading-0.2.6/pymultithreading.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      635 2023-07-03 16:16:37.000000 pymultithreading-0.2.6/pyproject.toml
--rw-rw-rw-   0        0        0       20 2023-05-30 09:10:35.000000 pymultithreading-0.2.6/requirements-dev.txt
--rw-rw-rw-   0        0        0       11 2023-05-30 09:09:27.000000 pymultithreading-0.2.6/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-07-03 16:16:38.221646 pymultithreading-0.2.6/setup.cfg
--rw-rw-rw-   0        0        0     1561 2023-07-03 16:16:27.000000 pymultithreading-0.2.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-08 21:11:13.758590 pymultithreading-1.0.0/
+-rw-rw-rw-   0        0        0       98 2023-07-08 21:11:13.000000 pymultithreading-1.0.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     2019 2023-07-08 21:11:13.758590 pymultithreading-1.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1217 2023-07-01 08:57:20.000000 pymultithreading-1.0.0/README.md
+-rw-rw-rw-   0        0        0    12920 2023-03-17 11:12:17.000000 pymultithreading-1.0.0/build.py
+drwxrwxrwx   0        0        0        0 2023-07-08 21:11:13.743572 pymultithreading-1.0.0/multithreading/
+-rw-rw-rw-   0        0        0       53 2023-06-17 10:18:28.000000 pymultithreading-1.0.0/multithreading/__init__.py
+-rw-rw-rw-   0        0        0    11589 2023-07-08 21:10:47.000000 pymultithreading-1.0.0/multithreading/process.py
+drwxrwxrwx   0        0        0        0 2023-07-08 21:11:13.757598 pymultithreading-1.0.0/pymultithreading.egg-info/
+-rw-rw-rw-   0        0        0     2019 2023-07-08 21:11:13.000000 pymultithreading-1.0.0/pymultithreading.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      344 2023-07-08 21:11:13.000000 pymultithreading-1.0.0/pymultithreading.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-08 21:11:13.000000 pymultithreading-1.0.0/pymultithreading.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       31 2023-07-08 21:11:13.000000 pymultithreading-1.0.0/pymultithreading.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-07-08 21:11:13.000000 pymultithreading-1.0.0/pymultithreading.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      635 2023-07-08 21:11:13.000000 pymultithreading-1.0.0/pyproject.toml
+-rw-rw-rw-   0        0        0       29 2023-07-08 21:08:12.000000 pymultithreading-1.0.0/requirements-dev.txt
+-rw-rw-rw-   0        0        0       20 2023-07-08 21:08:06.000000 pymultithreading-1.0.0/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-07-08 21:11:13.758590 pymultithreading-1.0.0/setup.cfg
+-rw-rw-rw-   0        0        0     1561 2023-07-08 21:11:08.000000 pymultithreading-1.0.0/setup.py
```

### Comparing `pymultithreading-0.2.6/PKG-INFO` & `pymultithreading-1.0.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymultithreading
-Version: 0.2.6
+Version: 1.0.0
 Summary: A python module for creating multithreading processes easily, in a more Pythonic way.
 Home-page: https://github.com/Shahaf-F-S/multithreading
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pymultithreading-0.2.6/README.md` & `pymultithreading-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `pymultithreading-0.2.6/build.py` & `pymultithreading-1.0.0/build.py`

 * *Files identical despite different names*

### Comparing `pymultithreading-0.2.6/multithreading/process.py` & `pymultithreading-1.0.0/multithreading/process.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 # process.py
 
 import datetime as dt
-from dataclasses import dataclass
 import threading
 import time
 from abc import ABCMeta
 from typing import (
     Any, Optional, Dict, Callable, ClassVar,
     Iterable, Union, TypeVar, Generic
 )
 
+from attrs import define
+
 from represent import represent, Modifiers
 
 __all__ = [
     "Caller",
     "CallDefinition",
     "CallsResults",
     "multi_threaded_call",
@@ -21,15 +22,15 @@
     "wait_call_completion",
     "ProcessTime",
     "ProcessInfo",
     "find_caller",
     "CallResults"
 ]
 
-@dataclass(repr=False, slots=True)
+@define(repr=False)
 @represent
 class ProcessInfo(metaclass=ABCMeta):
     """A class to contain the info of a call to the callers."""
 
     start: dt.datetime
     end: dt.datetime
 
@@ -49,15 +50,15 @@
 
 class ProcessTime(ProcessInfo):
     """A class to contain the info of a call to the callers."""
 # end ProcessTime
 
 _ReturnType = TypeVar("_ReturnType")
 
-@dataclass(repr=False, slots=True)
+@define(repr=False)
 @represent
 class CallResults(Generic[_ReturnType]):
     """A class to represent a container for the call results."""
 
     returns: Optional[_ReturnType] = None
     thread: Optional[threading.Thread] = None
     start: Optional[dt.datetime] = None
@@ -241,21 +242,19 @@
         self.wait = wait
         self.reset_before = reset_before
         self.reset_after = reset_after
         self.sleep = sleep
     # end __init__
 # end CallDefinition
 
-@dataclass(repr=False, slots=True)
+@define(repr=False)
 @represent
 class CallsResults:
     """A class to contain the info of a call to the callers."""
 
-    # __modifiers__ = Modifiers(excluded=["tread"], force=True)
-
     callers: Dict[Caller, CallResults]
     total: ProcessTime
     waiting: ProcessTime
     definition: CallDefinition
 
     def caller(self, identifier: Any) -> Caller:
         """
```

### Comparing `pymultithreading-0.2.6/pymultithreading.egg-info/PKG-INFO` & `pymultithreading-1.0.0/pymultithreading.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymultithreading
-Version: 0.2.6
+Version: 1.0.0
 Summary: A python module for creating multithreading processes easily, in a more Pythonic way.
 Home-page: https://github.com/Shahaf-F-S/multithreading
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pymultithreading-0.2.6/pyproject.toml` & `pymultithreading-1.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = 'pymultithreading'
-version = '0.2.6'
+version = '1.0.0'
 description = 'A python module for creating multithreading processes easily, in a more Pythonic way.'
 classifiers = [
 	'Intended Audience :: Developers',
 	'License :: OSI Approved :: MIT License',
 	'Programming Language :: Python',
 	'Programming Language :: Python :: 3',
 	'Programming Language :: Python :: 3.8',
```

### Comparing `pymultithreading-0.2.6/setup.py` & `pymultithreading-1.0.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,15 +21,15 @@
             "__pycache__",
             "*.pyc"
         ],
         include=[],
         requirements="requirements.txt",
         dev_requirements="requirements-dev.txt",
         name='pymultithreading',
-        version='0.2.6',
+        version='1.0.0',
         description=(
             "A python module for creating multithreading "
             "processes easily, in a more Pythonic way."
         ),
         license='MIT',
         author="Shahaf Frank-Shapir",
         author_email='shahaffrs@gmail.com',
```

