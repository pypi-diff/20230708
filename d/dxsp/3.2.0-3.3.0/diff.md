# Comparing `tmp/dxsp-3.2.0.tar.gz` & `tmp/dxsp-3.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dxsp-3.2.0.tar", max compression
+gzip compressed data, was "dxsp-3.3.0.tar", max compression
```

## Comparing `dxsp-3.2.0.tar` & `dxsp-3.3.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1064 2023-07-03 15:28:45.419052 dxsp-3.2.0/LICENSE
--rw-r--r--   0        0        0     2395 2023-07-03 15:28:45.419052 dxsp-3.2.0/README.md
--rw-r--r--   0        0        0      114 2023-07-03 15:28:46.371094 dxsp-3.2.0/dxsp/__init__.py
--rw-r--r--   0        0        0      418 2023-07-03 15:28:45.419052 dxsp-3.2.0/dxsp/config.py
--rw-r--r--   0        0        0    10489 2023-07-03 15:28:45.419052 dxsp-3.2.0/dxsp/default_settings.toml
--rw-r--r--   0        0        0    14284 2023-07-03 15:28:45.419052 dxsp-3.2.0/dxsp/main.py
--rw-r--r--   0        0        0      103 2023-07-03 15:28:45.419052 dxsp-3.2.0/dxsp/protocols/__init__.py
--rw-r--r--   0        0        0     3536 2023-07-03 15:28:45.419052 dxsp-3.2.0/dxsp/protocols/oneinch.py
--rw-r--r--   0        0        0     1773 2023-07-03 15:28:45.419052 dxsp-3.2.0/dxsp/protocols/uniswap.py
--rw-r--r--   0        0        0      990 2023-07-03 15:28:45.419052 dxsp-3.2.0/dxsp/protocols/zerox.py
--rw-r--r--   0        0        0     2144 2023-07-03 15:28:46.371094 dxsp-3.2.0/pyproject.toml
--rw-r--r--   0        0        0     3244 1970-01-01 00:00:00.000000 dxsp-3.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-07-08 08:01:21.330985 dxsp-3.3.0/LICENSE
+-rw-r--r--   0        0        0     2688 2023-07-08 08:01:21.330985 dxsp-3.3.0/README.md
+-rw-r--r--   0        0        0      115 2023-07-08 08:01:22.230990 dxsp-3.3.0/dxsp/__init__.py
+-rw-r--r--   0        0        0      417 2023-07-08 08:01:21.334985 dxsp-3.3.0/dxsp/config.py
+-rw-r--r--   0        0        0    10489 2023-07-08 08:01:21.334985 dxsp-3.3.0/dxsp/default_settings.toml
+-rw-r--r--   0        0        0    17240 2023-07-08 08:01:21.334985 dxsp-3.3.0/dxsp/main.py
+-rw-r--r--   0        0        0      103 2023-07-08 08:01:21.334985 dxsp-3.3.0/dxsp/protocols/__init__.py
+-rw-r--r--   0        0        0     3536 2023-07-08 08:01:21.334985 dxsp-3.3.0/dxsp/protocols/oneinch.py
+-rw-r--r--   0        0        0     1773 2023-07-08 08:01:21.334985 dxsp-3.3.0/dxsp/protocols/uniswap.py
+-rw-r--r--   0        0        0      990 2023-07-08 08:01:21.334985 dxsp-3.3.0/dxsp/protocols/zerox.py
+-rw-r--r--   0        0        0     2255 2023-07-08 08:01:22.230990 dxsp-3.3.0/pyproject.toml
+-rw-r--r--   0        0        0     3537 1970-01-01 00:00:00.000000 dxsp-3.3.0/PKG-INFO
```

### Comparing `dxsp-3.2.0/LICENSE` & `dxsp-3.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dxsp-3.2.0/dxsp/default_settings.toml` & `dxsp-3.3.0/dxsp/default_settings.toml`

 * *Files identical despite different names*

### Comparing `dxsp-3.2.0/dxsp/protocols/oneinch.py` & `dxsp-3.3.0/dxsp/protocols/oneinch.py`

 * *Files identical despite different names*

### Comparing `dxsp-3.2.0/dxsp/protocols/uniswap.py` & `dxsp-3.3.0/dxsp/protocols/uniswap.py`

 * *Files identical despite different names*

### Comparing `dxsp-3.2.0/dxsp/protocols/zerox.py` & `dxsp-3.3.0/dxsp/protocols/zerox.py`

 * *Files identical despite different names*

### Comparing `dxsp-3.2.0/pyproject.toml` & `dxsp-3.3.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,15 @@
+
+[build-system]
+requires = ["poetry-core"]
+build-backend = "poetry.core.masonry.api"
+
 [tool.poetry]
 name = "dxsp"
-version = "3.2.0"
+version = "3.3.0"
 description = "DXSP (DeX SwaP), A defi swap helper package. Swap made easy."
 authors = ["mraniki <8766259+mraniki@users.noreply.github.com>"]
 license = "MIT License"
 readme = "README.md"
 packages = [
     {include = "dxsp"}
 ]
@@ -16,25 +21,38 @@
 
 [tool.poetry.dependencies]
 python = "^3.10"
 dynaconf = "^3.1.12"
 web3 = "^6.4.0"
 pycoingecko = "^3.1.0"
 uniswap-python = "^0.7.0"
-#eip712 = "^0.2.1"
-#eth-ape'[recommended-plugins]' = "^0.6.11"
 
 [tool.poetry.dev-dependencies]
 python-semantic-release = "^7.34.3"
+
+
+[tool.poetry.group.test.dependencies]
 pytest = "^7.0"
 pytest-cov = "^4.1"
 pytest-asyncio = "^0.21.0"
 pytest-mock = "^3.11.1"
 eth_tester = "^0.9.0b2"
 
+[tool.poetry.group.docs]
+optional = true
+
+[tool.poetry.group.docs.dependencies]
+sphinx = "^6.0.0"
+sphinx_bootstrap_theme = "^0.8.1"
+sphinx-autoapi = "^2.1.1"
+sphinx-copybutton= "^0.5.2"
+myst-parser = "^2.0.0"
+sphinx-notfound-page = "*"
+
+
 [tool.pytest.ini_options]
 pythonpath = "."
 testpaths = "tests"
 python_classes = "Test*"
 log_format = "%(asctime)s - %(levelname)s - %(name)s - %(message)s"
 log_level = "DEBUG"
 
@@ -42,25 +60,14 @@
 omit = [
     "tests/*",
     "examples/*",
     "docs/*",
     "*/config.py"
 ]
 
-[tool.poetry.group.docs.dependencies]
-sphinx = "^7.0.1"
-sphinx-autoapi = "^2.1.0"
-furo = "^2023.5.20"
-
-
-[build-system]
-requires = ["poetry-core"]
-build-backend = "poetry.core.masonry.api"
-
-
 [tool.semantic_release]
 version_variable = ["pyproject.toml:version","dxsp/__init__.py:__version__"]
 branch = "main"
 upload_to_pypi = true
 upload_to_release = true
 build_command = "pip install poetry && poetry build"
 commit_parser = "semantic_release.history.emoji_parser"
```

