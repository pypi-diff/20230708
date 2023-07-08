# Comparing `tmp/aiopywttr-2.2.1.tar.gz` & `tmp/aiopywttr-2.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiopywttr-2.2.1.tar", max compression
+gzip compressed data, was "aiopywttr-2.2.2.tar", max compression
```

## Comparing `aiopywttr-2.2.1.tar` & `aiopywttr-2.2.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1065 2023-07-06 15:59:22.689695 aiopywttr-2.2.1/LICENSE
--rw-r--r--   0        0        0      603 2023-07-06 15:59:22.689695 aiopywttr-2.2.1/README.md
--rw-r--r--   0        0        0      183 2023-07-06 15:59:22.689695 aiopywttr-2.2.1/aiopywttr/__init__.py
--rw-r--r--   0        0        0     6104 2023-07-06 15:59:22.689695 aiopywttr-2.2.1/aiopywttr/_wttr.py
--rw-r--r--   0        0        0        0 2023-07-06 15:59:22.689695 aiopywttr-2.2.1/aiopywttr/py.typed
--rw-r--r--   0        0        0     3431 2023-07-06 15:59:22.689695 aiopywttr-2.2.1/pyproject.toml
--rw-r--r--   0        0        0     2129 1970-01-01 00:00:00.000000 aiopywttr-2.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-07-08 15:11:55.668154 aiopywttr-2.2.2/LICENSE
+-rw-r--r--   0        0        0      603 2023-07-08 15:11:55.668154 aiopywttr-2.2.2/README.md
+-rw-r--r--   0        0        0      183 2023-07-08 15:11:55.668154 aiopywttr-2.2.2/aiopywttr/__init__.py
+-rw-r--r--   0        0        0     6021 2023-07-08 15:11:55.668154 aiopywttr-2.2.2/aiopywttr/_wttr.py
+-rw-r--r--   0        0        0        0 2023-07-08 15:11:55.668154 aiopywttr-2.2.2/aiopywttr/py.typed
+-rw-r--r--   0        0        0     3465 2023-07-08 15:11:55.668154 aiopywttr-2.2.2/pyproject.toml
+-rw-r--r--   0        0        0     2175 1970-01-01 00:00:00.000000 aiopywttr-2.2.2/PKG-INFO
```

### Comparing `aiopywttr-2.2.1/LICENSE` & `aiopywttr-2.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `aiopywttr-2.2.1/README.md` & `aiopywttr-2.2.2/README.md`

 * *Files identical despite different names*

### Comparing `aiopywttr-2.2.1/aiopywttr/_wttr.py` & `aiopywttr-2.2.2/aiopywttr/_wttr.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,26 +9,26 @@
 class Wttr:
     """Asynchronous wrapper for wttr.in weather forecast API.
 
     Examples:
         Prints the average temperature in New York today:
 
         ```python
-        >>> import asyncio
-        >>>
-        >>> import aiopywttr
-        >>>
-        >>>
-        >>> async def main():
-        ...     wttr = aiopywttr.Wttr("New York")
-        ...     forecast = await wttr.en()
-        ...     print(forecast.weather[0].avgtemp_c)
-        >>>
-        >>>
-        >>> asyncio.run(main())
+        import asyncio
+
+        import aiopywttr
+
+
+        async def main():
+            wttr = aiopywttr.Wttr("New York")
+            forecast = await wttr.en()
+            print(forecast.weather[0].avgtemp_c)
+
+
+        asyncio.run(main())
         ```
     """
 
     __slots__ = ("location", "session")
 
     def __init__(
         self, location: str, session: Optional[ClientSession] = None
```

### Comparing `aiopywttr-2.2.1/pyproject.toml` & `aiopywttr-2.2.2/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aiopywttr"
-version = "2.2.1"
+version = "2.2.2"
 description = "Asynchronous wrapper for wttr.in API"
 authors = ["monosans <hsyqixco@protonmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/monosans/aiopywttr"
 documentation = "https://aiopywttr.readthedocs.io/"
 keywords = ["forecast", "weather"]
@@ -24,15 +24,15 @@
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Topic :: Software Development :: Libraries",
     "Topic :: Software Development",
     "Typing :: Typed",
 ]
 
 [tool.poetry.dependencies]
-python = "^3.7.2"
+python = "^3.7"
 aiohttp = "^3.8"
 pywttr-models = "^1.1"
 
 [tool.poetry.group.dev.dependencies]
 black = "23.3.0"
 covdefaults = "2.3.0"
 mypy = "1.4.1"
@@ -45,14 +45,15 @@
 
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

### Comparing `aiopywttr-2.2.1/PKG-INFO` & `aiopywttr-2.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 Metadata-Version: 2.1
 Name: aiopywttr
-Version: 2.2.1
+Version: 2.2.2
 Summary: Asynchronous wrapper for wttr.in API
 Home-page: https://github.com/monosans/aiopywttr
 License: MIT
 Keywords: forecast,weather
 Author: monosans
 Author-email: hsyqixco@protonmail.com
-Requires-Python: >=3.7.2,<4.0.0
+Requires-Python: >=3.7,<4.0
 Classifier: Environment :: Web Environment
 Classifier: Framework :: AsyncIO
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

