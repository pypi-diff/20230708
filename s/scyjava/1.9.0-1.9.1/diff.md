# Comparing `tmp/scyjava-1.9.0.tar.gz` & `tmp/scyjava-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scyjava-1.9.0.tar", last modified: Tue Feb 21 00:30:50 2023, max compression
+gzip compressed data, was "scyjava-1.9.1.tar", last modified: Fri Jul  7 23:09:03 2023, max compression
```

## Comparing `scyjava-1.9.0.tar` & `scyjava-1.9.1.tar`

### file list

```diff
@@ -1,27 +1,40 @@
-drwxrwxr-x   0 curtis    (1000) curtis    (1000)        0 2023-02-21 00:30:50.429279 scyjava-1.9.0/
--rw-rw-r--   0 curtis    (1000) curtis    (1000)    20107 2023-02-21 00:30:50.429279 scyjava-1.9.0/PKG-INFO
--rw-rw-r--   0 curtis    (1000) curtis    (1000)    18632 2023-02-17 01:16:56.000000 scyjava-1.9.0/README.md
--rw-rw-r--   0 curtis    (1000) curtis    (1000)     2041 2023-02-21 00:30:29.000000 scyjava-1.9.0/pyproject.toml
--rw-rw-r--   0 curtis    (1000) curtis    (1000)      117 2023-02-21 00:30:50.429279 scyjava-1.9.0/setup.cfg
-drwxrwxr-x   0 curtis    (1000) curtis    (1000)        0 2023-02-21 00:30:50.429279 scyjava-1.9.0/src/
-drwxrwxr-x   0 curtis    (1000) curtis    (1000)        0 2023-02-21 00:30:50.429279 scyjava-1.9.0/src/scyjava/
--rw-rw-r--   0 curtis    (1000) curtis    (1000)     5608 2023-02-17 01:16:56.000000 scyjava-1.9.0/src/scyjava/__init__.py
--rw-rw-r--   0 curtis    (1000) curtis    (1000)     1401 2022-11-08 03:57:25.000000 scyjava-1.9.0/src/scyjava/_arrays.py
--rw-rw-r--   0 curtis    (1000) curtis    (1000)    30342 2022-11-18 19:17:24.000000 scyjava-1.9.0/src/scyjava/_convert.py
--rw-rw-r--   0 curtis    (1000) curtis    (1000)    18953 2023-02-17 01:16:56.000000 scyjava-1.9.0/src/scyjava/_java.py
--rw-rw-r--   0 curtis    (1000) curtis    (1000)     4334 2023-02-17 01:16:56.000000 scyjava-1.9.0/src/scyjava/_script.py
--rw-rw-r--   0 curtis    (1000) curtis    (1000)     2527 2022-11-08 03:57:25.000000 scyjava-1.9.0/src/scyjava/_versions.py
--rw-rw-r--   0 curtis    (1000) curtis    (1000)     4695 2022-11-18 15:46:05.000000 scyjava-1.9.0/src/scyjava/config.py
-drwxrwxr-x   0 curtis    (1000) curtis    (1000)        0 2023-02-21 00:30:50.429279 scyjava-1.9.0/src/scyjava.egg-info/
--rw-rw-r--   0 curtis    (1000) curtis    (1000)    20107 2023-02-21 00:30:50.000000 scyjava-1.9.0/src/scyjava.egg-info/PKG-INFO
--rw-rw-r--   0 curtis    (1000) curtis    (1000)      495 2023-02-21 00:30:50.000000 scyjava-1.9.0/src/scyjava.egg-info/SOURCES.txt
--rw-rw-r--   0 curtis    (1000) curtis    (1000)        1 2023-02-21 00:30:50.000000 scyjava-1.9.0/src/scyjava.egg-info/dependency_links.txt
--rw-rw-r--   0 curtis    (1000) curtis    (1000)      123 2023-02-21 00:30:50.000000 scyjava-1.9.0/src/scyjava.egg-info/requires.txt
--rw-rw-r--   0 curtis    (1000) curtis    (1000)        8 2023-02-21 00:30:50.000000 scyjava-1.9.0/src/scyjava.egg-info/top_level.txt
-drwxrwxr-x   0 curtis    (1000) curtis    (1000)        0 2023-02-21 00:30:50.429279 scyjava-1.9.0/tests/
--rw-rw-r--   0 curtis    (1000) curtis    (1000)     4425 2022-11-18 15:46:05.000000 scyjava-1.9.0/tests/test_arrays.py
--rw-rw-r--   0 curtis    (1000) curtis    (1000)     1411 2022-11-18 15:46:05.000000 scyjava-1.9.0/tests/test_basics.py
--rw-rw-r--   0 curtis    (1000) curtis    (1000)    11816 2022-11-18 15:46:05.000000 scyjava-1.9.0/tests/test_convert.py
--rw-rw-r--   0 curtis    (1000) curtis    (1000)      668 2022-06-08 01:42:46.000000 scyjava-1.9.0/tests/test_jvm.py
--rw-rw-r--   0 curtis    (1000) curtis    (1000)     5360 2022-11-18 15:46:05.000000 scyjava-1.9.0/tests/test_pandas.py
--rw-rw-r--   0 curtis    (1000) curtis    (1000)      518 2022-11-18 16:20:45.000000 scyjava-1.9.0/tests/test_version.py
+drwxrwxr-x   0 curtis    (1000) curtis    (1000)        0 2023-07-07 23:09:03.986823 scyjava-1.9.1/
+-rw-rw-r--   0 curtis    (1000) curtis    (1000)      311 2023-07-07 23:08:37.000000 scyjava-1.9.1/MANIFEST.in
+-rw-rw-r--   0 curtis    (1000) curtis    (1000)      478 2022-11-04 17:57:45.000000 scyjava-1.9.1/Makefile
+-rw-rw-r--   0 curtis    (1000) curtis    (1000)    20107 2023-07-07 23:09:03.986823 scyjava-1.9.1/PKG-INFO
+-rw-rw-r--   0 curtis    (1000) curtis    (1000)    18632 2023-02-17 01:16:56.000000 scyjava-1.9.1/README.md
+-rw-rw-r--   0 curtis    (1000) curtis    (1000)     1211 2020-11-27 06:32:00.000000 scyjava-1.9.1/UNLICENSE
+drwxrwxr-x   0 curtis    (1000) curtis    (1000)        0 2023-07-07 23:09:03.982823 scyjava-1.9.1/bin/
+-rwxrwxr-x   0 curtis    (1000) curtis    (1000)      167 2022-10-14 14:17:55.000000 scyjava-1.9.1/bin/check.sh
+-rwxrwxr-x   0 curtis    (1000) curtis    (1000)      164 2022-10-31 15:12:31.000000 scyjava-1.9.1/bin/clean.sh
+-rwxrwxr-x   0 curtis    (1000) curtis    (1000)      340 2023-07-07 23:08:37.000000 scyjava-1.9.1/bin/lint.sh
+-rwxrwxr-x   0 curtis    (1000) curtis    (1000)       85 2022-10-14 14:17:55.000000 scyjava-1.9.1/bin/setup.sh
+-rwxrwxr-x   0 curtis    (1000) curtis    (1000)     2742 2023-07-07 23:07:35.000000 scyjava-1.9.1/bin/test.sh
+-rw-rw-r--   0 curtis    (1000) curtis    (1000)     1047 2023-07-07 23:07:35.000000 scyjava-1.9.1/dev-environment.yml
+-rw-rw-r--   0 curtis    (1000) curtis    (1000)      750 2022-11-04 17:57:45.000000 scyjava-1.9.1/environment.yml
+-rw-rw-r--   0 curtis    (1000) curtis    (1000)     2370 2023-07-07 23:08:44.000000 scyjava-1.9.1/pyproject.toml
+-rw-rw-r--   0 curtis    (1000) curtis    (1000)       38 2023-07-07 23:09:03.986823 scyjava-1.9.1/setup.cfg
+drwxrwxr-x   0 curtis    (1000) curtis    (1000)        0 2023-07-07 23:09:03.982823 scyjava-1.9.1/src/
+drwxrwxr-x   0 curtis    (1000) curtis    (1000)        0 2023-07-07 23:09:03.982823 scyjava-1.9.1/src/scyjava/
+-rw-rw-r--   0 curtis    (1000) curtis    (1000)     5794 2023-05-31 20:38:13.000000 scyjava-1.9.1/src/scyjava/__init__.py
+-rw-rw-r--   0 curtis    (1000) curtis    (1000)     1401 2022-11-08 03:57:25.000000 scyjava-1.9.1/src/scyjava/_arrays.py
+-rw-rw-r--   0 curtis    (1000) curtis    (1000)    32086 2023-05-31 20:38:13.000000 scyjava-1.9.1/src/scyjava/_convert.py
+-rw-rw-r--   0 curtis    (1000) curtis    (1000)    18953 2023-05-31 19:33:54.000000 scyjava-1.9.1/src/scyjava/_java.py
+-rw-rw-r--   0 curtis    (1000) curtis    (1000)     4404 2023-07-07 19:51:00.000000 scyjava-1.9.1/src/scyjava/_script.py
+-rw-rw-r--   0 curtis    (1000) curtis    (1000)     2527 2022-11-08 03:57:25.000000 scyjava-1.9.1/src/scyjava/_versions.py
+-rw-rw-r--   0 curtis    (1000) curtis    (1000)     4695 2022-11-18 15:46:05.000000 scyjava-1.9.1/src/scyjava/config.py
+drwxrwxr-x   0 curtis    (1000) curtis    (1000)        0 2023-07-07 23:09:03.986823 scyjava-1.9.1/src/scyjava.egg-info/
+-rw-rw-r--   0 curtis    (1000) curtis    (1000)    20107 2023-07-07 23:09:03.000000 scyjava-1.9.1/src/scyjava.egg-info/PKG-INFO
+-rw-rw-r--   0 curtis    (1000) curtis    (1000)      637 2023-07-07 23:09:03.000000 scyjava-1.9.1/src/scyjava.egg-info/SOURCES.txt
+-rw-rw-r--   0 curtis    (1000) curtis    (1000)        1 2023-07-07 23:09:03.000000 scyjava-1.9.1/src/scyjava.egg-info/dependency_links.txt
+-rw-rw-r--   0 curtis    (1000) curtis    (1000)      162 2023-07-07 23:09:03.000000 scyjava-1.9.1/src/scyjava.egg-info/requires.txt
+-rw-rw-r--   0 curtis    (1000) curtis    (1000)        8 2023-07-07 23:09:03.000000 scyjava-1.9.1/src/scyjava.egg-info/top_level.txt
+drwxrwxr-x   0 curtis    (1000) curtis    (1000)        0 2023-07-07 23:09:03.986823 scyjava-1.9.1/tests/
+drwxrwxr-x   0 curtis    (1000) curtis    (1000)        0 2023-07-07 23:09:03.986823 scyjava-1.9.1/tests/it/
+-rw-rw-r--   0 curtis    (1000) curtis    (1000)     1901 2023-07-07 23:07:35.000000 scyjava-1.9.1/tests/it/scripting.py
+-rw-rw-r--   0 curtis    (1000) curtis    (1000)     4425 2022-11-18 15:46:05.000000 scyjava-1.9.1/tests/test_arrays.py
+-rw-rw-r--   0 curtis    (1000) curtis    (1000)     1411 2022-11-18 15:46:05.000000 scyjava-1.9.1/tests/test_basics.py
+-rw-rw-r--   0 curtis    (1000) curtis    (1000)    12131 2023-05-31 20:38:13.000000 scyjava-1.9.1/tests/test_convert.py
+-rw-rw-r--   0 curtis    (1000) curtis    (1000)      668 2022-06-08 01:42:46.000000 scyjava-1.9.1/tests/test_jvm.py
+-rw-rw-r--   0 curtis    (1000) curtis    (1000)     5360 2023-05-04 18:27:37.000000 scyjava-1.9.1/tests/test_pandas.py
+-rw-rw-r--   0 curtis    (1000) curtis    (1000)      518 2022-11-18 16:20:45.000000 scyjava-1.9.1/tests/test_version.py
```

### Comparing `scyjava-1.9.0/PKG-INFO` & `scyjava-1.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scyjava
-Version: 1.9.0
+Version: 1.9.1
 Summary: Supercharged Java access from Python
 Author-email: SciJava developers <ctrueden@wisc.edu>
 License: The Unlicense
 Project-URL: homepage, https://github.com/scijava/scyjava
 Project-URL: documentation, https://github.com/scijava/scyjava/blob/main/README.md
 Project-URL: source, https://github.com/scijava/scyjava
 Project-URL: download, https://pypi.org/project/scyjava/
```

### Comparing `scyjava-1.9.0/README.md` & `scyjava-1.9.1/README.md`

 * *Files identical despite different names*

### Comparing `scyjava-1.9.0/pyproject.toml` & `scyjava-1.9.1/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.2"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "scyjava"
-version = "1.9.0"
+version = "1.9.1"
 description = "Supercharged Java access from Python"
 license = {text = "The Unlicense"}
 authors = [{name = "SciJava developers", email = "ctrueden@wisc.edu"}]
 readme = "README.md"
 keywords = ["java", "maven", "cross-language"]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
@@ -40,14 +40,16 @@
 [project.optional-dependencies]
 # NB: Keep this in sync with dev-environment.yml!
 dev = [
     "autopep8",
     "black",
     "build",
     "flake8",
+    "flake8-pyproject",
+    "flake8-typing-imports",
     "isort",
     "jep",
     "pytest",
     "pytest-cov",
     "numpy",
     "pandas",
     "toml",
@@ -65,9 +67,17 @@
 package-dir = {"" = "src"}
 include-package-data = false
 
 [tool.setuptools.packages.find]
 where = ["src"]
 namespaces = false
 
+# Thanks to Flake8-pyproject, we can configure flake8 here!
+[tool.flake8]
+exclude = ["bin", "build", "dist"]
+extend-ignore = ["E203"]
+# See https://black.readthedocs.io/en/stable/guides/using_black_with_other_tools.html#flake8
+max-line-length = 88
+min_python_version = "3.7"
+
 [tool.isort]
 profile = "black"
```

### Comparing `scyjava-1.9.0/src/scyjava/__init__.py` & `scyjava-1.9.1/src/scyjava/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -170,14 +170,19 @@
 # JVM is already running -- for example, if we are running in Jep mode, where
 # Python is started from inside the JVM -- then these functions execute the
 # callbacks immediately, which means the involved functions must be defined and
 # functional at this point.
 
 
 def _initialize_converters():
+    _logger.debug("Initializing type converters")
+
     for converter in _stock_java_converters():
         add_java_converter(converter)
+    _logger.debug("Java converters:{'\n-'.join(java_converters)}")
+
     for converter in _stock_py_converters():
         add_py_converter(converter)
+    _logger.debug("Python converters:{'\n-'.join(py_converters)}")
 
 
 when_jvm_starts(_initialize_converters)
```

### Comparing `scyjava-1.9.0/src/scyjava/_arrays.py` & `scyjava-1.9.1/src/scyjava/_arrays.py`

 * *Files identical despite different names*

### Comparing `scyjava-1.9.0/src/scyjava/_convert.py` & `scyjava-1.9.1/src/scyjava/_convert.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 """
 The scyjava conversion subsystem, and built-in conversion functions.
 """
 
 import collections
 import inspect
+import logging
 import math
+from bisect import insort
 from pathlib import Path
 from typing import Any, Callable, Dict, List, NamedTuple
 
 from jpype import JBoolean, JByte, JChar, JDouble, JFloat, JInt, JLong, JShort
 
 from ._java import (
     JavaClasses,
@@ -19,14 +21,16 @@
     jclass,
     jimport,
     jinstance,
     mode,
     start_jvm,
 )
 
+_logger = logging.getLogger(__name__)
+
 
 # NB: We cannot use org.scijava.priority.Priority or other Java-side class
 # here because we don't want to impose Java-side dependencies, and we don't
 # want to require Java to be started before reasoning about priorities.
 class Priority:
     FIRST = 1e300
     EXTREMELY_HIGH = 1e6
@@ -35,25 +39,30 @@
     NORMAL = 0
     LOW = -1e2
     VERY_LOW = -1e4
     EXTREMELY_LOW = -1e6
     LAST = -1e300
 
 
+def _priority(thing):
+    return getattr(thing, "priority", Priority.NORMAL)
+
+
 def _has_kwargs(f):
     return not isjava(f) and any(
         p.kind == inspect.Parameter.VAR_KEYWORD
         for p in inspect.signature(f).parameters.values()
     )
 
 
 class Converter(NamedTuple):
     predicate: Callable[[Any], bool]
     converter: Callable[[Any], Any]
     priority: float = Priority.NORMAL
+    name: str = "<unnamed>"
 
     def supports(self, obj: Any, **hints: Dict) -> bool:
         return (
             self.predicate(obj, **hints)
             if _has_kwargs(self.predicate)
             else self.predicate(obj)
         )
@@ -61,19 +70,43 @@
     def convert(self, obj: Any, **hints: Dict) -> Any:
         return (
             self.converter(obj, **hints)
             if _has_kwargs(self.converter)
             else self.converter(obj)
         )
 
+    def __lt__(self, other):
+        return self.priority < _priority(other)
+
+    def __le__(self, other):
+        return self.priority <= _priority(other)
+
+    def __gt__(self, other):
+        return self.priority > _priority(other)
+
+    def __ge__(self, other):
+        return self.priority >= _priority(other)
+
+    def __str__(self):
+        return self.name
+
 
 def _convert(obj: Any, converters: List[Converter], **hints: Dict) -> Any:
-    suitable_converters = [c for c in converters if c.supports(obj, **hints)]
-    prioritized = max(suitable_converters, key=lambda c: c.priority)
-    return prioritized.convert(obj, **hints)
+    # NB: The given converters are assumed to be sorted ascending by priority,
+    # meaning lower-priority items appear earlier than higher-priority ones.
+    # But we want to try the higher priority converters first, so we
+    # need to iterate the given converters list starting at the end.
+    debug = hints.get("debug", False)
+    log = _logger.info if debug else _logger.debug
+    log(f"Converting object of type {type(obj)} with hints {hints}")
+    for converter in reversed(converters):
+        if converter.supports(obj, **hints):
+            log(f"- {converter} supports")
+            return converter.convert(obj, **hints)
+        log(f"- {converter} does not support")
 
 
 # -- Python to Java --
 
 # Adapted from code posted by vslotman on GitHub:
 # https://github.com/kivy/pyjnius/issues/217#issue-145981070
 
@@ -111,15 +144,15 @@
 
 
 def add_java_converter(converter: Converter) -> None:
     """
     Add a converter to the list used by to_java.
     :param converter: A Converter going from python to java
     """
-    java_converters.append(converter)
+    insort(java_converters, converter)
 
 
 def to_java(obj: Any, **hints: Dict) -> Any:
     """
     Recursively convert a Python object to a Java object.
 
     Supported types include:
@@ -173,141 +206,144 @@
 def _stock_java_converters() -> List[Converter]:
     """
     Construct the Python-to-Java converters supported out of the box.
     :returns: A list of Converters
     """
     start_jvm()
     return [
-        # Other (Exceptional) converter
         Converter(
+            name="Other (Exceptional) converter",
             predicate=lambda obj: True,
             converter=_raise_type_exception,
             priority=Priority.EXTREMELY_LOW - 1,
         ),
-        # None -> None
         Converter(
+            name="None -> None",
             predicate=lambda obj: obj is None,
             converter=lambda obj: None,
             priority=Priority.EXTREMELY_HIGH + 1,
         ),
-        # Java object identity
         Converter(
+            name="Java object identity",
             predicate=isjava,
             converter=lambda obj: obj,
             priority=Priority.EXTREMELY_HIGH,
         ),
-        # str -> java.lang.String
         Converter(
+            name="str -> java.lang.String",
             predicate=lambda obj: isinstance(obj, str),
             converter=lambda obj: _jc.String(obj.encode("utf-8"), "utf-8"),
         ),
-        # bool -> java.lang.Boolean
         Converter(
+            name="bool -> java.lang.Boolean",
             predicate=lambda obj: isinstance(obj, bool),
             converter=_jc.Boolean,
+            # NB: Must be higher priority than the int converters,
+            # because the bool type extends the int type!
+            priority=Priority.NORMAL + 1,
         ),
-        # int -> java.lang.Byte
         Converter(
+            name="int -> java.lang.Byte",
             predicate=lambda obj, **hints: isinstance(obj, int)
             and ("type" in hints and hints["type"] in ("b", "byte", "Byte"))
             and _jc.Byte.MIN_VALUE <= obj <= _jc.Byte.MAX_VALUE,
             converter=_jc.Byte,
             priority=Priority.HIGH,
         ),
-        # int -> java.lang.Short
         Converter(
+            name="int -> java.lang.Short",
             predicate=lambda obj, **hints: isinstance(obj, int)
             and ("type" in hints and hints["type"] in ("s", "short", "Short"))
             and _jc.Short.MIN_VALUE <= obj <= _jc.Short.MAX_VALUE,
             converter=_jc.Short,
             priority=Priority.HIGH,
         ),
-        # int -> java.lang.Integer
         Converter(
+            name="int -> java.lang.Integer",
             predicate=lambda obj, **hints: isinstance(obj, int)
             and ("type" not in hints or hints["type"] in ("i", "int", "Integer"))
             and _jc.Integer.MIN_VALUE <= obj <= _jc.Integer.MAX_VALUE,
             converter=_jc.Integer,
         ),
-        # int -> java.lang.Long
         Converter(
+            name="int -> java.lang.Long",
             predicate=lambda obj, **hints: isinstance(obj, int)
             and ("type" not in hints or hints["type"] in ("j", "l", "long", "Long"))
             and _jc.Long.MIN_VALUE <= obj <= _jc.Long.MAX_VALUE,
             converter=_jc.Long,
             priority=Priority.NORMAL - 1,
         ),
-        # int -> java.math.BigInteger
         Converter(
+            name="int -> java.math.BigInteger",
             predicate=lambda obj, **hints: isinstance(obj, int)
             and (
                 "type" not in hints or hints["type"] in ("bi", "bigint", "BigInteger")
             ),
             converter=lambda obj: _jc.BigInteger(str(obj)),
             priority=Priority.NORMAL - 2,
         ),
-        # float -> java.lang.Float
         Converter(
+            name="float -> java.lang.Float",
             predicate=lambda obj, **hints: isinstance(obj, float)
             and ("type" not in hints or hints["type"] in ("f", "float", "Float"))
             and (
                 math.isinf(obj)
                 or math.isnan(obj)
                 or -_jc.Float.MAX_VALUE <= obj <= _jc.Float.MAX_VALUE
             ),
             converter=_jc.Float,
         ),
-        # float -> java.lang.Double
         Converter(
+            name="float -> java.lang.Double",
             predicate=lambda obj, **hints: isinstance(obj, float)
             and ("type" not in hints or hints["type"] in ("d", "double", "Double"))
             and (
                 math.isinf(obj)
                 or math.isnan(obj)
                 or -_jc.Double.MAX_VALUE <= obj <= _jc.Double.MAX_VALUE
             ),
             converter=_jc.Double,
             priority=Priority.NORMAL - 1,
         ),
-        # float -> java.math.BigDecimal
         Converter(
+            name="float -> java.math.BigDecimal",
             predicate=lambda obj, **hints: isinstance(obj, float)
             and (
                 "type" not in hints or hints["type"] in ("bd", "bigdec", "BigDecimal")
             ),
             converter=lambda obj: _jc.BigDecimal(str(obj)),
             priority=Priority.NORMAL - 2,
         ),
-        # pathlib.Path -> java.nio.file.Path
         Converter(
+            name="pathlib.Path -> java.nio.file.Path",
             predicate=lambda obj: isinstance(obj, Path),
             # Pass an empty String array in addition to our path
             # To make it clear to jep that we want the string-args version
             # JPype is smart enough to know that, but it doesn't mind the extra args
             converter=lambda obj: _jc.Paths.get(str(obj), jarray(_jc.String, [0])),
             priority=Priority.NORMAL + 1,
         ),
-        # pandas.DataFrame -> org.scijava.table.Table
         Converter(
+            name="pandas.DataFrame -> org.scijava.table.Table",
             predicate=lambda obj: type(obj).__name__ == "DataFrame",
             converter=_pandas_to_table,
             priority=Priority.NORMAL + 1,
         ),
-        # collections.abc.Mapping -> java.util.Map
         Converter(
+            name="collections.abc.Mapping -> java.util.Map",
             predicate=lambda obj: isinstance(obj, collections.abc.Mapping),
             converter=_convertMap,
         ),
-        # collections.abc.Set -> java.util.Set
         Converter(
+            name="collections.abc.Set -> java.util.Set",
             predicate=lambda obj: isinstance(obj, collections.abc.Set),
             converter=_convertSet,
         ),
-        # collections.abc.Iterable -> java.util.Iterable
         Converter(
+            name="collections.abc.Iterable -> java.util.Iterable",
             predicate=lambda obj: isinstance(obj, collections.abc.Iterable),
             converter=_convertIterable,
             priority=Priority.NORMAL - 1,
         ),
     ]
 
 
@@ -482,15 +518,15 @@
 
 
 def add_py_converter(converter: Converter) -> None:
     """
     Add a converter to the list used by to_python.
     :param converter: A Converter from java to python
     """
-    py_converters.append(converter)
+    insort(py_converters, converter)
 
 
 def to_python(data: Any, gentle: bool = False) -> Any:
     """
     Recursively convert a Java object to a Python object.
 
     Supported types include:
@@ -525,168 +561,173 @@
     """
     Construct the Java-to-Python converters supported out of the box.
     :returns: A list of Converters
     """
     start_jvm()
 
     converters = [
-        # Other (Exceptional) converter
         Converter(
+            name="Other (Exceptional) converter",
             predicate=lambda obj: True,
             converter=_raise_type_exception,
             priority=Priority.EXTREMELY_LOW - 1,
         ),
-        # Python object identity
         Converter(
+            name="Python object identity",
             predicate=lambda obj: not isjava(obj),
             converter=lambda obj: obj,
             priority=Priority.EXTREMELY_HIGH,
         ),
-        # java.lang.Boolean -> bool
         Converter(
+            name="java.lang.Boolean -> bool",
             predicate=lambda obj: jinstance(obj, _jc.Boolean),
             converter=lambda obj: obj.booleanValue(),
         ),
-        # java.lang.Byte -> int
         Converter(
+            name="java.lang.Byte -> int",
             predicate=lambda obj: jinstance(obj, _jc.Byte),
             converter=lambda obj: int(obj.byteValue()),
         ),
-        # java.lang.Character -> str
         Converter(
+            name="java.lang.Character -> str",
             predicate=lambda obj: jinstance(obj, _jc.Character),
             converter=lambda obj: str,
         ),
-        # java.lang.Double -> float
         Converter(
+            name="java.lang.Double -> float",
             predicate=lambda obj: jinstance(obj, _jc.Double),
             converter=lambda obj: float(obj.doubleValue()),
         ),
-        # java.lang.Float -> float
         Converter(
+            name="java.lang.Float -> float",
             predicate=lambda obj: jinstance(obj, _jc.Float),
             converter=lambda obj: float(obj.floatValue()),
         ),
-        # java.lang.Integer -> int
         Converter(
+            name="java.lang.Integer -> int",
             predicate=lambda obj: jinstance(obj, _jc.Integer),
             converter=lambda obj: int(obj.intValue()),
         ),
-        # java.lang.Long -> int
         Converter(
+            name="java.lang.Long -> int",
             predicate=lambda obj: jinstance(obj, _jc.Long),
             converter=lambda obj: int(obj.longValue()),
         ),
-        # java.lang.Short -> int
         Converter(
+            name="java.lang.Short -> int",
             predicate=lambda obj: jinstance(obj, _jc.Short),
             converter=lambda obj: int(obj.shortValue()),
         ),
-        # java.lang.String -> str
         Converter(
+            name="java.lang.String -> str",
             predicate=lambda obj: jinstance(obj, _jc.String),
             converter=lambda obj: str(obj),
         ),
-        # java.math.BigInteger -> int
         Converter(
+            name="java.math.BigInteger -> int",
             predicate=lambda obj: jinstance(obj, _jc.BigInteger),
             converter=lambda obj: int(str(obj)),
         ),
-        # java.math.BigDecimal -> float
         Converter(
+            name="java.math.BigDecimal -> float",
             predicate=lambda obj: jinstance(obj, _jc.BigDecimal),
             converter=lambda obj: float(str(obj)),
         ),
-        # java.util.List -> scyjava.JavaList (list-like)
         Converter(
+            name="java.util.List -> scyjava.JavaList (list-like)",
             predicate=lambda obj: jinstance(obj, _jc.List),
             converter=JavaList,
         ),
-        # java.util.Map -> scyjava.JavaMap (dict-like)
         Converter(
+            name="java.util.Map -> scyjava.JavaMap (dict-like)",
             predicate=lambda obj: jinstance(obj, _jc.Map),
             converter=JavaMap,
         ),
-        # java.util.Set -> scyjava.JavaSet (set-like)
         Converter(
+            name="java.util.Set -> scyjava.JavaSet (set-like)",
             predicate=lambda obj: jinstance(obj, _jc.Set),
             converter=JavaSet,
         ),
-        # java.util.Collection -> scyjava.JavaCollection (collections.abc.Collection)
         Converter(
+            name="java.util.Collection -> "
+            "scyjava.JavaCollection (collections.abc.Collection)",
             predicate=lambda obj: jinstance(obj, _jc.Collection),
             converter=JavaCollection,
             priority=Priority.NORMAL - 1,
         ),
-        # java.lang.Iterable -> scyjava.JavaIterable (collections.abc.Iterable)
         Converter(
+            name="java.lang.Iterable -> "
+            "scyjava.JavaIterable (collections.abc.Iterable)",
             predicate=lambda obj: jinstance(obj, _jc.Iterable),
             converter=JavaIterable,
             priority=Priority.NORMAL - 1,
         ),
-        # java.util.Iterator -> scyjava.JavaIterator (collections.abc.Iterator)
         Converter(
+            name="java.util.Iterator -> "
+            "scyjava.JavaIterator (collections.abc.Iterator)",
             predicate=lambda obj: jinstance(obj, _jc.Iterator),
             converter=JavaIterator,
             priority=Priority.NORMAL - 1,
         ),
-        # java.nio.file.Path -> pathlib.Path
         Converter(
+            name="java.nio.file.Path -> pathlib.Path",
             predicate=lambda obj: jinstance(obj, _jc.Path),
             converter=lambda obj: Path(str(obj)),
             priority=Priority.NORMAL + 1,
         ),
-        # jarray -> list
         Converter(
+            name="jarray -> list",
             predicate=lambda obj: is_jarray(obj),
             converter=lambda obj: [to_python(o) for o in obj],
             priority=Priority.VERY_LOW,
         ),
     ]
     if _import_pandas(required=False):
-        # org.scijava.table.Table -> pandas.DataFrame
         converters.append(
             Converter(
-                predicate=_is_table, converter=_convert_table, priority=Priority.HIGH
+                name="org.scijava.table.Table -> pandas.DataFrame",
+                predicate=_is_table,
+                converter=_convert_table,
+                priority=Priority.HIGH,
             )
         )
 
     if mode == Mode.JPYPE:
         converters.extend(
             [
-                # JBoolean -> bool
                 Converter(
+                    name="JBoolean -> bool",
                     predicate=lambda obj: isinstance(obj, JBoolean),
                     converter=bool,
                     priority=Priority.NORMAL + 1,
                 ),
-                # JByte/JInt/JLong/JShort -> int
                 Converter(
+                    name="JByte/JInt/JLong/JShort -> int",
                     predicate=lambda obj: isinstance(obj, (JByte, JInt, JLong, JShort)),
                     converter=int,
                     priority=Priority.NORMAL + 1,
                 ),
-                # JDouble/JFloat -> float
                 Converter(
+                    name="JDouble/JFloat -> float",
                     predicate=lambda obj: isinstance(obj, (JDouble, JFloat)),
                     converter=float,
                     priority=Priority.NORMAL + 1,
                 ),
-                # JChar -> str
                 Converter(
+                    name="JChar -> str",
                     predicate=lambda obj: isinstance(obj, JChar),
                     converter=str,
                     priority=Priority.NORMAL + 1,
                 ),
             ]
         )
         if _import_numpy(required=False):
-            # primitive array -> numpy.ndarray
             converters.append(
                 Converter(
+                    name="primitive array -> numpy.ndarray",
                     predicate=_supports_jarray_to_ndarray,
                     converter=_jarray_to_ndarray,
                 )
             )
 
     return converters
 
@@ -704,15 +745,15 @@
     :return: The converted NumPy ndarray
     """
     np = _import_numpy()
     assert _supports_jarray_to_ndarray(jarr)
     element_type = _jarray_element_type(jarr)
     # fmt: off
     jarraytype_map = {
-        JBoolean: np.bool8,
+        JBoolean: np.bool_,
         JByte:    np.int8,
         # JChar:  np.???,
         JDouble:  np.float64,
         JFloat:   np.float32,
         JInt:     np.int32,
         JLong:    np.int64,
         JShort:   np.int16,
```

### Comparing `scyjava-1.9.0/src/scyjava/_java.py` & `scyjava-1.9.1/src/scyjava/_java.py`

 * *Files identical despite different names*

### Comparing `scyjava-1.9.0/src/scyjava/_script.py` & `scyjava-1.9.1/src/scyjava/_script.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 https://github.com/scijava/scripting-python.
 """
 
 import ast
 import sys
 import threading
 import traceback
+from contextlib import redirect_stdout
 
 from jpype import JImplements, JOverride
 
 from ._convert import to_java
 from ._java import jimport
 
 
@@ -36,27 +37,25 @@
             self._thread_to_context[thread] = scriptContext
 
         def removeScriptContext(self, thread):
             if thread in self._thread_to_context:
                 del self._thread_to_context[thread]
 
         def flush(self):
-            self._std_default.flush()
+            self._writer().flush()
 
         def write(self, s):
-            if threading.currentThread() in self._thread_to_context:
-                self._thread_to_context[threading.currentThread()].getWriter().write(
-                    to_java(s)
-                )
-            else:
-                self._std_default.write(s)
+            self._writer().write(s)
+
+        def _writer(self):
+            return self._thread_to_context.get(
+                threading.currentThread(), self._std_default
+            )
 
-    # Q: Is there a better way to manage stdout in conjunction with the script runner?
     stdoutContextWriter = ScriptContextWriter(sys.stdout)
-    sys.stdout = stdoutContextWriter
 
     @JImplements("java.util.function.Supplier")
     class PythonObjectSupplier:
         def __init__(self, obj):
             self.obj = obj
 
         @JOverride
@@ -73,39 +72,44 @@
                 script_locals[key] = arg.vars[key]
 
             stdoutContextWriter.addScriptContext(
                 threading.currentThread(), arg.scriptContext
             )
 
             return_value = None
-            try:
-                # NB: Execute the block, except for the last statement,
-                # which we evaluate instead to get its return value.
-                # Credit: https://stackoverflow.com/a/39381428/1207769
-
-                block = ast.parse(str(arg.script), mode="exec")
-                last = None
-                if (
-                    len(block.body) > 0
-                    and hasattr(block.body[-1], "value")
-                    and not isinstance(block.body[-1], ast.Assign)
-                ):
-                    # Last statement of the script looks like an expression. Evaluate!
-                    last = ast.Expression(block.body.pop().value)
-
-                _globals = {}
-                exec(compile(block, "<string>", mode="exec"), _globals, script_locals)
-                if last is not None:
-                    return_value = eval(
-                        compile(last, "<string>", mode="eval"), _globals, script_locals
+            with redirect_stdout(stdoutContextWriter):
+                try:
+                    # NB: Execute the block, except for the last statement,
+                    # which we evaluate instead to get its return value.
+                    # Credit: https://stackoverflow.com/a/39381428/1207769
+
+                    block = ast.parse(str(arg.script), mode="exec")
+                    last = None
+                    if (
+                        len(block.body) > 0
+                        and hasattr(block.body[-1], "value")
+                        and not isinstance(block.body[-1], ast.Assign)
+                    ):
+                        # Last statement looks like an expression. Evaluate!
+                        last = ast.Expression(block.body.pop().value)
+
+                    _globals = {}
+                    exec(
+                        compile(block, "<string>", mode="exec"), _globals, script_locals
                     )
-            except Exception:
-                error_writer = arg.scriptContext.getErrorWriter()
-                if error_writer is not None:
-                    error_writer.write(to_java(traceback.format_exc()))
+                    if last is not None:
+                        return_value = eval(
+                            compile(last, "<string>", mode="eval"),
+                            _globals,
+                            script_locals,
+                        )
+                except Exception:
+                    error_writer = arg.scriptContext.getErrorWriter()
+                    if error_writer is not None:
+                        error_writer.write(to_java(traceback.format_exc()))
 
             stdoutContextWriter.removeScriptContext(threading.currentThread())
 
             # Copy script locals back into script bindings/vars.
             for key in script_locals.keys():
                 try:
                     arg.vars[key] = to_java(script_locals[key])
```

### Comparing `scyjava-1.9.0/src/scyjava/_versions.py` & `scyjava-1.9.1/src/scyjava/_versions.py`

 * *Files identical despite different names*

### Comparing `scyjava-1.9.0/src/scyjava/config.py` & `scyjava-1.9.1/src/scyjava/config.py`

 * *Files identical despite different names*

### Comparing `scyjava-1.9.0/src/scyjava.egg-info/PKG-INFO` & `scyjava-1.9.1/src/scyjava.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scyjava
-Version: 1.9.0
+Version: 1.9.1
 Summary: Supercharged Java access from Python
 Author-email: SciJava developers <ctrueden@wisc.edu>
 License: The Unlicense
 Project-URL: homepage, https://github.com/scijava/scyjava
 Project-URL: documentation, https://github.com/scijava/scyjava/blob/main/README.md
 Project-URL: source, https://github.com/scijava/scyjava
 Project-URL: download, https://pypi.org/project/scyjava/
```

### Comparing `scyjava-1.9.0/tests/test_arrays.py` & `scyjava-1.9.1/tests/test_arrays.py`

 * *Files identical despite different names*

### Comparing `scyjava-1.9.0/tests/test_basics.py` & `scyjava-1.9.1/tests/test_basics.py`

 * *Files identical despite different names*

### Comparing `scyjava-1.9.0/tests/test_convert.py` & `scyjava-1.9.1/tests/test_convert.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,14 +10,15 @@
     add_java_converter,
     config,
     jarray,
     java_converters,
     jclass,
     jimport,
     jinstance,
+    py_converters,
     to_java,
     to_python,
 )
 from scyjava.config import Mode, mode
 
 config.endpoints.append("org.scijava:scijava-table")
 config.add_option("-Djava.awt.headless=true")
@@ -338,20 +339,27 @@
 
     def test_conversion_priority(self):
         # Add a converter prioritized over the default converter
         String = jimport("java.lang.String")
         invader = "Not Hello World"
 
         bad_converter = Converter(
+            name=f"test_conversion_priority: str -> '{invader}'",
             predicate=lambda obj: isinstance(obj, str),
             converter=lambda obj: String(invader.encode("utf-8"), "utf-8"),
             priority=100,
         )
         add_java_converter(bad_converter)
 
         # Ensure that the conversion uses our new converter
         s = "Hello world!"
         js = to_java(s)
         for e, a in zip(invader, js.toCharArray()):
             assert e == a
 
         java_converters.remove(bad_converter)
+
+    def test_converter_priority(self):
+        assert len(java_converters) > 0
+        assert sorted(java_converters) == java_converters
+        assert len(py_converters) > 0
+        assert sorted(py_converters) == py_converters
```

### Comparing `scyjava-1.9.0/tests/test_jvm.py` & `scyjava-1.9.1/tests/test_jvm.py`

 * *Files identical despite different names*

### Comparing `scyjava-1.9.0/tests/test_pandas.py` & `scyjava-1.9.1/tests/test_pandas.py`

 * *Files 0% similar despite different names*

```diff
@@ -113,15 +113,15 @@
         array = np.random.random(size=(7, 5)) > 0.5
 
         table = self._fill_table(table, array, lambda v: Boolean(bool(v)))
         df = to_python(table)
 
         assert_same_table(table, df)
         for col in df.columns:
-            assert df.dtypes[col] == np.bool8
+            assert df.dtypes[col] == np.bool_
 
         # Mixed table
         table = jimport("org.scijava.table.DefaultGenericTable")()
         table.appendColumns(columns)
         table.setRowCount(7)
         array_float = np.random.random(size=(7, 1))
         array_int = np.random.random(size=(7, 1)) * 100
```

### Comparing `scyjava-1.9.0/tests/test_version.py` & `scyjava-1.9.1/tests/test_version.py`

 * *Files identical despite different names*

