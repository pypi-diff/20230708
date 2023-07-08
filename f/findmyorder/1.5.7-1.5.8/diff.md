# Comparing `tmp/findmyorder-1.5.7.tar.gz` & `tmp/findmyorder-1.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "findmyorder-1.5.7.tar", max compression
+gzip compressed data, was "findmyorder-1.5.8.tar", max compression
```

## Comparing `findmyorder-1.5.7.tar` & `findmyorder-1.5.8.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1064 2023-07-08 12:26:42.959852 findmyorder-1.5.7/LICENSE
--rw-r--r--   0        0        0     3046 2023-07-08 12:26:42.959852 findmyorder-1.5.7/README.md
--rw-r--r--   0        0        0      113 2023-07-08 12:26:43.647857 findmyorder-1.5.7/findmyorder/__init__.py
--rw-r--r--   0        0        0      660 2023-07-08 12:26:42.959852 findmyorder-1.5.7/findmyorder/config.py
--rw-r--r--   0        0        0     2495 2023-07-08 12:26:42.959852 findmyorder-1.5.7/findmyorder/default_settings.toml
--rw-r--r--   0        0        0     5779 2023-07-08 12:26:42.959852 findmyorder-1.5.7/findmyorder/main.py
--rw-r--r--   0        0        0     2307 2023-07-08 12:26:43.647857 findmyorder-1.5.7/pyproject.toml
--rw-r--r--   0        0        0     3919 1970-01-01 00:00:00.000000 findmyorder-1.5.7/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-07-08 13:21:03.368658 findmyorder-1.5.8/LICENSE
+-rw-r--r--   0        0        0     3046 2023-07-08 13:21:03.368658 findmyorder-1.5.8/README.md
+-rw-r--r--   0        0        0      113 2023-07-08 13:21:04.172675 findmyorder-1.5.8/findmyorder/__init__.py
+-rw-r--r--   0        0        0      660 2023-07-08 13:21:03.368658 findmyorder-1.5.8/findmyorder/config.py
+-rw-r--r--   0        0        0     2495 2023-07-08 13:21:03.368658 findmyorder-1.5.8/findmyorder/default_settings.toml
+-rw-r--r--   0        0        0     5779 2023-07-08 13:21:03.368658 findmyorder-1.5.8/findmyorder/main.py
+-rw-r--r--   0        0        0     2349 2023-07-08 13:21:04.172675 findmyorder-1.5.8/pyproject.toml
+-rw-r--r--   0        0        0     3919 1970-01-01 00:00:00.000000 findmyorder-1.5.8/PKG-INFO
```

### Comparing `findmyorder-1.5.7/LICENSE` & `findmyorder-1.5.8/LICENSE`

 * *Files identical despite different names*

### Comparing `findmyorder-1.5.7/README.md` & `findmyorder-1.5.8/README.md`

 * *Files identical despite different names*

### Comparing `findmyorder-1.5.7/findmyorder/config.py` & `findmyorder-1.5.8/findmyorder/config.py`

 * *Files identical despite different names*

### Comparing `findmyorder-1.5.7/findmyorder/default_settings.toml` & `findmyorder-1.5.8/findmyorder/default_settings.toml`

 * *Files identical despite different names*

### Comparing `findmyorder-1.5.7/findmyorder/main.py` & `findmyorder-1.5.8/findmyorder/main.py`

 * *Files identical despite different names*

### Comparing `findmyorder-1.5.7/pyproject.toml` & `findmyorder-1.5.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 
 [tool.poetry]
 name = "findmyorder"
-version = "1.5.7"
+version = "1.5.8"
 description = "A python package to identify and parse order for trade execution."
 authors = ["mraniki <8766259+mraniki@users.noreply.github.com>"]
 license = "MIT License"
 readme = "README.md"
 keywords = ["trading", "order", "trade","buy","sell"]
 packages = [
     {include = "findmyorder"}
@@ -42,15 +42,17 @@
 
 [tool.poetry.group.docs.dependencies]
 sphinx = "^7.0.0"
 sphinx_bootstrap_theme = "^0.8.1"
 sphinx-autoapi = "^2.1.1"
 sphinx-copybutton= "^0.5.2"
 myst-parser = "^2.0.0"
-sphinx-notfound-page = "*"
+sphinx-notfound-page = "^0.8.3"
+seed_intersphinx_mapping = "^1.2.1"
+
 
 [tool.pytest.ini_options]
 pythonpath = "."
 testpaths = "tests"
 python_classes = "Test*"
 log_format = "%(asctime)s - %(levelname)s - %(name)s - %(message)s"
 log_level = "DEBUG"
```

### Comparing `findmyorder-1.5.7/PKG-INFO` & `findmyorder-1.5.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: findmyorder
-Version: 1.5.7
+Version: 1.5.8
 Summary: A python package to identify and parse order for trade execution.
 License: MIT
 Keywords: trading,order,trade,buy,sell
 Author: mraniki
 Author-email: 8766259+mraniki@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: findmyorder Version: 1.5.7 Summary: A python
+Metadata-Version: 2.1 Name: findmyorder Version: 1.5.8 Summary: A python
 package to identify and parse order for trade execution. License: MIT Keywords:
 trading,order,trade,buy,sell Author: mraniki Author-email:
 8766259+mraniki@users.noreply.github.com Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Requires-Dist: dynaconf
 (>=3.1.12,<4.0.0) Requires-Dist: emoji (>=2.5.1,<3.0.0) Requires-Dist:
```

