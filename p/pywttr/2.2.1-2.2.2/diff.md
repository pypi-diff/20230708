# Comparing `tmp/pywttr-2.2.1.tar.gz` & `tmp/pywttr-2.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pywttr-2.2.1.tar", max compression
+gzip compressed data, was "pywttr-2.2.2.tar", max compression
```

## Comparing `pywttr-2.2.1.tar` & `pywttr-2.2.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1065 2023-07-06 15:59:19.998339 pywttr-2.2.1/LICENSE
--rw-r--r--   0        0        0      570 2023-07-06 15:59:19.998339 pywttr-2.2.1/README.md
--rw-r--r--   0        0        0     3363 2023-07-06 15:59:20.002339 pywttr-2.2.1/pyproject.toml
--rw-r--r--   0        0        0      170 2023-07-06 15:59:20.002339 pywttr-2.2.1/pywttr/__init__.py
--rw-r--r--   0        0        0     5304 2023-07-06 15:59:20.002339 pywttr-2.2.1/pywttr/_wttr.py
--rw-r--r--   0        0        0        0 2023-07-06 15:59:20.002339 pywttr-2.2.1/pywttr/py.typed
--rw-r--r--   0        0        0     2040 1970-01-01 00:00:00.000000 pywttr-2.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-07-08 15:11:56.844981 pywttr-2.2.2/LICENSE
+-rw-r--r--   0        0        0      570 2023-07-08 15:11:56.844981 pywttr-2.2.2/README.md
+-rw-r--r--   0        0        0     3397 2023-07-08 15:11:56.844981 pywttr-2.2.2/pyproject.toml
+-rw-r--r--   0        0        0      170 2023-07-08 15:11:56.844981 pywttr-2.2.2/pywttr/__init__.py
+-rw-r--r--   0        0        0     5277 2023-07-08 15:11:56.844981 pywttr-2.2.2/pywttr/_wttr.py
+-rw-r--r--   0        0        0        0 2023-07-08 15:11:56.844981 pywttr-2.2.2/pywttr/py.typed
+-rw-r--r--   0        0        0     2086 1970-01-01 00:00:00.000000 pywttr-2.2.2/PKG-INFO
```

### Comparing `pywttr-2.2.1/LICENSE` & `pywttr-2.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pywttr-2.2.1/README.md` & `pywttr-2.2.2/README.md`

 * *Files identical despite different names*

### Comparing `pywttr-2.2.1/pyproject.toml` & `pywttr-2.2.2/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pywttr"
-version = "2.2.1"
+version = "2.2.2"
 description = "Wrapper for wttr.in API"
 authors = ["monosans <hsyqixco@protonmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/monosans/pywttr"
 documentation = "https://pywttr.readthedocs.io/"
 keywords = ["forecast", "weather"]
@@ -23,15 +23,15 @@
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Topic :: Software Development :: Libraries",
     "Topic :: Software Development",
     "Typing :: Typed",
 ]
 
 [tool.poetry.dependencies]
-python = "^3.7.2"
+python = "^3.7"
 pywttr-models = "^1.1"
 requests = "^2.28"
 
 [tool.poetry.group.dev.dependencies]
 black = "23.3.0"
 covdefaults = "2.3.0"
 mypy = "1.4.1"
@@ -44,14 +44,15 @@
 
 [tool.poetry.group.docs]
 optional = true
 
 [tool.poetry.group.docs.dependencies]
 mkdocs = "1.4.3"
 mkdocs-material = "9.1.18"
+mkdocs-minify-html-plugin = "0.1.0"
 mkdocstrings = { version = "0.22.0", extras = ["python"] }
 
 [tool.black]
 target-version = ["py37"]
 line-length = 80
 skip-magic-trailing-comma = true
 preview = true
```

### Comparing `pywttr-2.2.1/pywttr/_wttr.py` & `pywttr-2.2.2/pywttr/_wttr.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,19 +9,19 @@
 class Wttr:
     """Wrapper for wttr.in weather forecast API.
 
     Examples:
         Prints the average temperature in New York today:
 
         ```python
-        >>> import pywttr
-        >>>
-        >>> wttr = pywttr.Wttr("New York")
-        >>> forecast = wttr.en()
-        >>> print(forecast.weather[0].avgtemp_c)
+        import pywttr
+
+        wttr = pywttr.Wttr("New York")
+        forecast = wttr.en()
+        print(forecast.weather[0].avgtemp_c)
         ```
     """
 
     __slots__ = ("location", "session")
 
     def __init__(
         self, location: str, session: Optional[Session] = None
```

### Comparing `pywttr-2.2.1/PKG-INFO` & `pywttr-2.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 Metadata-Version: 2.1
 Name: pywttr
-Version: 2.2.1
+Version: 2.2.2
 Summary: Wrapper for wttr.in API
 Home-page: https://github.com/monosans/pywttr
 License: MIT
 Keywords: forecast,weather
 Author: monosans
 Author-email: hsyqixco@protonmail.com
-Requires-Python: >=3.7.2,<4.0.0
+Requires-Python: >=3.7,<4.0
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Pydantic
 Classifier: Framework :: Pydantic :: 1
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Internet
 Classifier: Topic :: Internet :: WWW/HTTP
```

