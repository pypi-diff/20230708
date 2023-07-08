# Comparing `tmp/dxsp-3.3.0.tar.gz` & `tmp/dxsp-3.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dxsp-3.3.0.tar", max compression
+gzip compressed data, was "dxsp-3.3.1.tar", max compression
```

## Comparing `dxsp-3.3.0.tar` & `dxsp-3.3.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1064 2023-07-08 08:01:21.330985 dxsp-3.3.0/LICENSE
--rw-r--r--   0        0        0     2688 2023-07-08 08:01:21.330985 dxsp-3.3.0/README.md
--rw-r--r--   0        0        0      115 2023-07-08 08:01:22.230990 dxsp-3.3.0/dxsp/__init__.py
--rw-r--r--   0        0        0      417 2023-07-08 08:01:21.334985 dxsp-3.3.0/dxsp/config.py
--rw-r--r--   0        0        0    10489 2023-07-08 08:01:21.334985 dxsp-3.3.0/dxsp/default_settings.toml
--rw-r--r--   0        0        0    17240 2023-07-08 08:01:21.334985 dxsp-3.3.0/dxsp/main.py
--rw-r--r--   0        0        0      103 2023-07-08 08:01:21.334985 dxsp-3.3.0/dxsp/protocols/__init__.py
--rw-r--r--   0        0        0     3536 2023-07-08 08:01:21.334985 dxsp-3.3.0/dxsp/protocols/oneinch.py
--rw-r--r--   0        0        0     1773 2023-07-08 08:01:21.334985 dxsp-3.3.0/dxsp/protocols/uniswap.py
--rw-r--r--   0        0        0      990 2023-07-08 08:01:21.334985 dxsp-3.3.0/dxsp/protocols/zerox.py
--rw-r--r--   0        0        0     2255 2023-07-08 08:01:22.230990 dxsp-3.3.0/pyproject.toml
--rw-r--r--   0        0        0     3537 1970-01-01 00:00:00.000000 dxsp-3.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-07-08 09:28:56.315778 dxsp-3.3.1/LICENSE
+-rw-r--r--   0        0        0     2688 2023-07-08 09:28:56.315778 dxsp-3.3.1/README.md
+-rw-r--r--   0        0        0      115 2023-07-08 09:28:57.183817 dxsp-3.3.1/dxsp/__init__.py
+-rw-r--r--   0        0        0      417 2023-07-08 09:28:56.319778 dxsp-3.3.1/dxsp/config.py
+-rw-r--r--   0        0        0    10489 2023-07-08 09:28:56.319778 dxsp-3.3.1/dxsp/default_settings.toml
+-rw-r--r--   0        0        0    17240 2023-07-08 09:28:56.319778 dxsp-3.3.1/dxsp/main.py
+-rw-r--r--   0        0        0      103 2023-07-08 09:28:56.319778 dxsp-3.3.1/dxsp/protocols/__init__.py
+-rw-r--r--   0        0        0     3536 2023-07-08 09:28:56.319778 dxsp-3.3.1/dxsp/protocols/oneinch.py
+-rw-r--r--   0        0        0     1773 2023-07-08 09:28:56.319778 dxsp-3.3.1/dxsp/protocols/uniswap.py
+-rw-r--r--   0        0        0      990 2023-07-08 09:28:56.319778 dxsp-3.3.1/dxsp/protocols/zerox.py
+-rw-r--r--   0        0        0     2255 2023-07-08 09:28:57.179817 dxsp-3.3.1/pyproject.toml
+-rw-r--r--   0        0        0     3537 1970-01-01 00:00:00.000000 dxsp-3.3.1/PKG-INFO
```

### Comparing `dxsp-3.3.0/LICENSE` & `dxsp-3.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dxsp-3.3.0/README.md` & `dxsp-3.3.1/README.md`

 * *Files identical despite different names*

### Comparing `dxsp-3.3.0/dxsp/default_settings.toml` & `dxsp-3.3.1/dxsp/default_settings.toml`

 * *Files identical despite different names*

### Comparing `dxsp-3.3.0/dxsp/main.py` & `dxsp-3.3.1/dxsp/main.py`

 * *Files identical despite different names*

### Comparing `dxsp-3.3.0/dxsp/protocols/oneinch.py` & `dxsp-3.3.1/dxsp/protocols/oneinch.py`

 * *Files identical despite different names*

### Comparing `dxsp-3.3.0/dxsp/protocols/uniswap.py` & `dxsp-3.3.1/dxsp/protocols/uniswap.py`

 * *Files identical despite different names*

### Comparing `dxsp-3.3.0/dxsp/protocols/zerox.py` & `dxsp-3.3.1/dxsp/protocols/zerox.py`

 * *Files identical despite different names*

### Comparing `dxsp-3.3.0/pyproject.toml` & `dxsp-3.3.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "dxsp"
-version = "3.3.0"
+version = "3.3.1"
 description = "DXSP (DeX SwaP), A defi swap helper package. Swap made easy."
 authors = ["mraniki <8766259+mraniki@users.noreply.github.com>"]
 license = "MIT License"
 readme = "README.md"
 packages = [
     {include = "dxsp"}
 ]
@@ -37,15 +37,15 @@
 pytest-mock = "^3.11.1"
 eth_tester = "^0.9.0b2"
 
 [tool.poetry.group.docs]
 optional = true
 
 [tool.poetry.group.docs.dependencies]
-sphinx = "^6.0.0"
+sphinx = "^7.0.0"
 sphinx_bootstrap_theme = "^0.8.1"
 sphinx-autoapi = "^2.1.1"
 sphinx-copybutton= "^0.5.2"
 myst-parser = "^2.0.0"
 sphinx-notfound-page = "*"
```

### Comparing `dxsp-3.3.0/PKG-INFO` & `dxsp-3.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dxsp
-Version: 3.3.0
+Version: 3.3.1
 Summary: DXSP (DeX SwaP), A defi swap helper package. Swap made easy.
 License: MIT
 Author: mraniki
 Author-email: 8766259+mraniki@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dxsp Version: 3.3.0 Summary: DXSP (DeX SwaP), A
+Metadata-Version: 2.1 Name: dxsp Version: 3.3.1 Summary: DXSP (DeX SwaP), A
 defi swap helper package. Swap made easy. License: MIT Author: mraniki Author-
 email: 8766259+mraniki@users.noreply.github.com Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Requires-Dist: dynaconf
 (>=3.1.12,<4.0.0) Requires-Dist: pycoingecko (>=3.1.0,<4.0.0) Requires-Dist:
 uniswap-python (>=0.7.0,<0.8.0) Requires-Dist: web3 (>=6.4.0,<7.0.0) Project-
```

