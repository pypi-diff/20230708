# Comparing `tmp/jsonschema_spec-0.2.2.tar.gz` & `tmp/jsonschema_spec-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jsonschema_spec-0.2.2.tar", max compression
+gzip compressed data, was "jsonschema_spec-0.2.3.tar", max compression
```

## Comparing `jsonschema_spec-0.2.2.tar` & `jsonschema_spec-0.2.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0    11357 2023-06-15 07:44:42.482506 jsonschema_spec-0.2.2/LICENSE
--rw-r--r--   0        0        0     3121 2023-06-15 07:44:42.482506 jsonschema_spec-0.2.2/README.rst
--rw-r--r--   0        0        0      431 2023-06-15 07:44:42.486507 jsonschema_spec-0.2.2/jsonschema_spec/__init__.py
--rw-r--r--   0        0        0     2918 2023-06-15 07:44:42.486507 jsonschema_spec-0.2.2/jsonschema_spec/accessors.py
--rw-r--r--   0        0        0      761 2023-06-15 07:44:42.486507 jsonschema_spec-0.2.2/jsonschema_spec/handlers/__init__.py
--rw-r--r--   0        0        0     1557 2023-06-15 07:44:42.486507 jsonschema_spec-0.2.2/jsonschema_spec/handlers/file.py
--rw-r--r--   0        0        0      210 2023-06-15 07:44:42.486507 jsonschema_spec-0.2.2/jsonschema_spec/handlers/protocols.py
--rw-r--r--   0        0        0      747 2023-06-15 07:44:42.486507 jsonschema_spec-0.2.2/jsonschema_spec/handlers/requests.py
--rw-r--r--   0        0        0      587 2023-06-15 07:44:42.486507 jsonschema_spec-0.2.2/jsonschema_spec/handlers/urllib.py
--rw-r--r--   0        0        0      361 2023-06-15 07:44:42.486507 jsonschema_spec-0.2.2/jsonschema_spec/handlers/utils.py
--rw-r--r--   0        0        0     1392 2023-06-15 07:44:42.486507 jsonschema_spec-0.2.2/jsonschema_spec/loaders.py
--rw-r--r--   0        0        0     3985 2023-06-15 07:44:42.486507 jsonschema_spec-0.2.2/jsonschema_spec/paths.py
--rw-r--r--   0        0        0        0 2023-06-15 07:44:42.486507 jsonschema_spec-0.2.2/jsonschema_spec/py.typed
--rw-r--r--   0        0        0     1116 2023-06-15 07:44:42.486507 jsonschema_spec-0.2.2/jsonschema_spec/readers.py
--rw-r--r--   0        0        0     1471 2023-06-15 07:44:42.486507 jsonschema_spec-0.2.2/jsonschema_spec/retrievers.py
--rw-r--r--   0        0        0      181 2023-06-15 07:44:42.486507 jsonschema_spec-0.2.2/jsonschema_spec/typing.py
--rw-r--r--   0        0        0      247 2023-06-15 07:44:42.486507 jsonschema_spec-0.2.2/jsonschema_spec/utils.py
--rw-r--r--   0        0        0     1867 2023-06-15 07:44:42.486507 jsonschema_spec-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     4267 1970-01-01 00:00:00.000000 jsonschema_spec-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-07-08 15:48:38.553216 jsonschema_spec-0.2.3/LICENSE
+-rw-r--r--   0        0        0     3121 2023-07-08 15:48:38.553216 jsonschema_spec-0.2.3/README.rst
+-rw-r--r--   0        0        0      431 2023-07-08 15:48:38.553216 jsonschema_spec-0.2.3/jsonschema_spec/__init__.py
+-rw-r--r--   0        0        0     2918 2023-07-08 15:48:38.553216 jsonschema_spec-0.2.3/jsonschema_spec/accessors.py
+-rw-r--r--   0        0        0      761 2023-07-08 15:48:38.553216 jsonschema_spec-0.2.3/jsonschema_spec/handlers/__init__.py
+-rw-r--r--   0        0        0     1557 2023-07-08 15:48:38.553216 jsonschema_spec-0.2.3/jsonschema_spec/handlers/file.py
+-rw-r--r--   0        0        0      210 2023-07-08 15:48:38.553216 jsonschema_spec-0.2.3/jsonschema_spec/handlers/protocols.py
+-rw-r--r--   0        0        0      747 2023-07-08 15:48:38.553216 jsonschema_spec-0.2.3/jsonschema_spec/handlers/requests.py
+-rw-r--r--   0        0        0      587 2023-07-08 15:48:38.553216 jsonschema_spec-0.2.3/jsonschema_spec/handlers/urllib.py
+-rw-r--r--   0        0        0      361 2023-07-08 15:48:38.553216 jsonschema_spec-0.2.3/jsonschema_spec/handlers/utils.py
+-rw-r--r--   0        0        0     1392 2023-07-08 15:48:38.553216 jsonschema_spec-0.2.3/jsonschema_spec/loaders.py
+-rw-r--r--   0        0        0     3985 2023-07-08 15:48:38.553216 jsonschema_spec-0.2.3/jsonschema_spec/paths.py
+-rw-r--r--   0        0        0        0 2023-07-08 15:48:38.553216 jsonschema_spec-0.2.3/jsonschema_spec/py.typed
+-rw-r--r--   0        0        0     1127 2023-07-08 15:48:38.553216 jsonschema_spec-0.2.3/jsonschema_spec/readers.py
+-rw-r--r--   0        0        0     1471 2023-07-08 15:48:38.553216 jsonschema_spec-0.2.3/jsonschema_spec/retrievers.py
+-rw-r--r--   0        0        0      181 2023-07-08 15:48:38.553216 jsonschema_spec-0.2.3/jsonschema_spec/typing.py
+-rw-r--r--   0        0        0      247 2023-07-08 15:48:38.553216 jsonschema_spec-0.2.3/jsonschema_spec/utils.py
+-rw-r--r--   0        0        0     1867 2023-07-08 15:48:38.557216 jsonschema_spec-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0     4267 1970-01-01 00:00:00.000000 jsonschema_spec-0.2.3/PKG-INFO
```

### Comparing `jsonschema_spec-0.2.2/LICENSE` & `jsonschema_spec-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `jsonschema_spec-0.2.2/README.rst` & `jsonschema_spec-0.2.3/README.rst`

 * *Files identical despite different names*

### Comparing `jsonschema_spec-0.2.2/jsonschema_spec/accessors.py` & `jsonschema_spec-0.2.3/jsonschema_spec/accessors.py`

 * *Files identical despite different names*

### Comparing `jsonschema_spec-0.2.2/jsonschema_spec/handlers/__init__.py` & `jsonschema_spec-0.2.3/jsonschema_spec/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `jsonschema_spec-0.2.2/jsonschema_spec/handlers/file.py` & `jsonschema_spec-0.2.3/jsonschema_spec/handlers/file.py`

 * *Files identical despite different names*

### Comparing `jsonschema_spec-0.2.2/jsonschema_spec/handlers/requests.py` & `jsonschema_spec-0.2.3/jsonschema_spec/handlers/requests.py`

 * *Files identical despite different names*

### Comparing `jsonschema_spec-0.2.2/jsonschema_spec/handlers/urllib.py` & `jsonschema_spec-0.2.3/jsonschema_spec/handlers/urllib.py`

 * *Files identical despite different names*

### Comparing `jsonschema_spec-0.2.2/jsonschema_spec/loaders.py` & `jsonschema_spec-0.2.3/jsonschema_spec/loaders.py`

 * *Files identical despite different names*

### Comparing `jsonschema_spec-0.2.2/jsonschema_spec/paths.py` & `jsonschema_spec-0.2.3/jsonschema_spec/paths.py`

 * *Files identical despite different names*

### Comparing `jsonschema_spec-0.2.2/jsonschema_spec/readers.py` & `jsonschema_spec-0.2.3/jsonschema_spec/readers.py`

 * *Files 12% similar despite different names*

```diff
@@ -33,9 +33,9 @@
 
         uri = self.path.as_uri()
         return all_urls_handler(uri), uri
 
 
 class FilePathReader(PathReader):
     def __init__(self, file_path: str):
-        path = Path(file_path)
+        path = Path(file_path).absolute()
         super().__init__(path)
```

### Comparing `jsonschema_spec-0.2.2/jsonschema_spec/retrievers.py` & `jsonschema_spec-0.2.3/jsonschema_spec/retrievers.py`

 * *Files identical despite different names*

### Comparing `jsonschema_spec-0.2.2/pyproject.toml` & `jsonschema_spec-0.2.3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 [[tool.mypy.overrides]]
 module = "jsonschema_specifications"
 ignore_missing_imports = true
 
 [tool.poetry]
 name = "jsonschema-spec"
-version = "0.2.2"
+version = "0.2.3"
 description = "JSONSchema Spec with object-oriented paths"
 authors = ["Artur Maciag <maciag.artur@gmail.com>"]
 license = "Apache-2.0"
 readme = "README.rst"
 repository = "https://github.com/p1c2u/jsonschema-spec"
 keywords = ["jsonschema", "swagger", "spec"]
 classifiers = [
@@ -44,25 +44,25 @@
 python = "^3.8.0"
 PyYAML = ">=5.1"
 requests = {version = "^2.31.0", optional = true}
 referencing = ">=0.28.0,<0.30.0"
 
 [tool.poetry.dev-dependencies]
 pre-commit = "*"
-pytest = "^7.3.1"
-pytest-flake8 = "=1.1.0"
+pytest = "^7.4.0"
+pytest-flake8 = "=1.1.1"
 pytest-cov = "^4.1.0"
 isort = "^5.12.0"
 black = "^23.3.0"
 flynt = "0.78"
-mypy = "^1.3.0"
-types-PyYAML = "^6.0.11"
+mypy = "^1.4.1"
+types-PyYAML = "^6.0.12"
 types-requests = "^2.31.0"
 responses = "^0.23.1"
-deptry = "^0.11.0"
+deptry = "^0.12.0"
 
 [tool.pytest.ini_options]
 addopts = """
 --capture=no
 --verbose
 --showlocals
 --junitxml=reports/junit.xml
```

### Comparing `jsonschema_spec-0.2.2/PKG-INFO` & `jsonschema_spec-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jsonschema-spec
-Version: 0.2.2
+Version: 0.2.3
 Summary: JSONSchema Spec with object-oriented paths
 Home-page: https://github.com/p1c2u/jsonschema-spec
 License: Apache-2.0
 Keywords: jsonschema,swagger,spec
 Author: Artur Maciag
 Author-email: maciag.artur@gmail.com
 Requires-Python: >=3.8.0,<4.0.0
```

