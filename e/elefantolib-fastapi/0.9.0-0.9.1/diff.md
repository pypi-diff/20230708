# Comparing `tmp/elefantolib_fastapi-0.9.0.tar.gz` & `tmp/elefantolib_fastapi-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "elefantolib_fastapi-0.9.0.tar", max compression
+gzip compressed data, was "elefantolib_fastapi-0.9.1.tar", max compression
```

## Comparing `elefantolib_fastapi-0.9.0.tar` & `elefantolib_fastapi-0.9.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      878 2023-07-08 07:52:26.079350 elefantolib_fastapi-0.9.0/README.md
--rw-r--r--   0        0        0       22 2023-07-08 07:52:26.079350 elefantolib_fastapi-0.9.0/elefantolib_fastapi/__init__.py
--rw-r--r--   0        0        0     1018 2023-07-08 07:52:26.079350 elefantolib_fastapi-0.9.0/elefantolib_fastapi/connection.py
--rw-r--r--   0        0        0      878 2023-07-08 07:52:26.079350 elefantolib_fastapi-0.9.0/elefantolib_fastapi/depends.py
--rw-r--r--   0        0        0      934 2023-07-08 07:52:26.079350 elefantolib_fastapi-0.9.0/elefantolib_fastapi/exceptions.py
--rw-r--r--   0        0        0     1337 2023-07-08 07:52:26.079350 elefantolib_fastapi-0.9.0/elefantolib_fastapi/pagination.py
--rw-r--r--   0        0        0      209 2023-07-08 07:52:26.079350 elefantolib_fastapi-0.9.0/elefantolib_fastapi/requests.py
--rw-r--r--   0        0        0      721 2023-07-08 07:52:26.079350 elefantolib_fastapi-0.9.0/elefantolib_fastapi/routes.py
--rw-r--r--   0        0        0      217 2023-07-08 07:52:26.079350 elefantolib_fastapi-0.9.0/elefantolib_fastapi/schemas.py
--rw-r--r--   0        0        0      933 2023-07-08 07:52:39.467359 elefantolib_fastapi-0.9.0/pyproject.toml
--rw-r--r--   0        0        0     1667 1970-01-01 00:00:00.000000 elefantolib_fastapi-0.9.0/setup.py
--rw-r--r--   0        0        0     1438 1970-01-01 00:00:00.000000 elefantolib_fastapi-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0      878 2023-07-08 08:23:10.014035 elefantolib_fastapi-0.9.1/README.md
+-rw-r--r--   0        0        0       22 2023-07-08 08:23:10.014035 elefantolib_fastapi-0.9.1/elefantolib_fastapi/__init__.py
+-rw-r--r--   0        0        0     1018 2023-07-08 08:23:10.014035 elefantolib_fastapi-0.9.1/elefantolib_fastapi/connection.py
+-rw-r--r--   0        0        0      878 2023-07-08 08:23:10.014035 elefantolib_fastapi-0.9.1/elefantolib_fastapi/depends.py
+-rw-r--r--   0        0        0      934 2023-07-08 08:23:10.014035 elefantolib_fastapi-0.9.1/elefantolib_fastapi/exceptions.py
+-rw-r--r--   0        0        0     1337 2023-07-08 08:23:10.014035 elefantolib_fastapi-0.9.1/elefantolib_fastapi/pagination.py
+-rw-r--r--   0        0        0      209 2023-07-08 08:23:10.014035 elefantolib_fastapi-0.9.1/elefantolib_fastapi/requests.py
+-rw-r--r--   0        0        0      721 2023-07-08 08:23:10.014035 elefantolib_fastapi-0.9.1/elefantolib_fastapi/routes.py
+-rw-r--r--   0        0        0      188 2023-07-08 08:23:10.014035 elefantolib_fastapi-0.9.1/elefantolib_fastapi/schemas.py
+-rw-r--r--   0        0        0      933 2023-07-08 08:23:24.982049 elefantolib_fastapi-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0     1667 1970-01-01 00:00:00.000000 elefantolib_fastapi-0.9.1/setup.py
+-rw-r--r--   0        0        0     1438 1970-01-01 00:00:00.000000 elefantolib_fastapi-0.9.1/PKG-INFO
```

### Comparing `elefantolib_fastapi-0.9.0/README.md` & `elefantolib_fastapi-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `elefantolib_fastapi-0.9.0/elefantolib_fastapi/connection.py` & `elefantolib_fastapi-0.9.1/elefantolib_fastapi/connection.py`

 * *Files identical despite different names*

### Comparing `elefantolib_fastapi-0.9.0/elefantolib_fastapi/depends.py` & `elefantolib_fastapi-0.9.1/elefantolib_fastapi/depends.py`

 * *Files identical despite different names*

### Comparing `elefantolib_fastapi-0.9.0/elefantolib_fastapi/exceptions.py` & `elefantolib_fastapi-0.9.1/elefantolib_fastapi/exceptions.py`

 * *Files identical despite different names*

### Comparing `elefantolib_fastapi-0.9.0/elefantolib_fastapi/pagination.py` & `elefantolib_fastapi-0.9.1/elefantolib_fastapi/pagination.py`

 * *Files identical despite different names*

### Comparing `elefantolib_fastapi-0.9.0/elefantolib_fastapi/routes.py` & `elefantolib_fastapi-0.9.1/elefantolib_fastapi/routes.py`

 * *Files identical despite different names*

### Comparing `elefantolib_fastapi-0.9.0/pyproject.toml` & `elefantolib_fastapi-0.9.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "elefantolib-fastapi"
-version = "0.9.0"
+version = "0.9.1"
 description = ""
 authors = ["gglassota <gglassota2@gmail.com>"]
 readme = "README.md"
 packages = [{include = "elefantolib_fastapi"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `elefantolib_fastapi-0.9.0/setup.py` & `elefantolib_fastapi-0.9.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,15 +12,15 @@
  'fastapi>=0.100.0,<0.101.0',
  'pydantic>=2.0.2,<3.0.0',
  'redis>=4.6.0,<5.0.0',
  'sqlalchemy>=2.0.18,<3.0.0']
 
 setup_kwargs = {
     'name': 'elefantolib-fastapi',
-    'version': '0.9.0',
+    'version': '0.9.1',
     'description': '',
     'long_description': '## Elefantolib for FastAPI\n\n> **_NOTE:_**  Only for this library developers. After clone this repository you should run command:\n> \n\n ```console \ngit config core.hooksPath .githooks\n```\n\n\n## Installation\n\n<div class="termy">\n\n```console\npoetry add elefantolib-fastapi\n```\n</div>\n\n## Example\n\n### Prepare\n\n* Add environmental variables\n\n```\nSECRET=\nALGORITHM=\nISSUER=\n```\n* Defaults:\n    \n    - SECRET - not set, this is required\n    - ALGORITHM=HS256\n    - ISSUER=Consumer\n\n### Create it\n\n* Create a file `main.py` with:\n\n```Python\nfrom elefantolib_fastapi.requests import Request\nfrom elefantolib_fastapi.routes import APIRoute\n\nfrom fastapi import FastAPI\n\napp = FastAPI()\n\napp.router.route_class = APIRoute\n\n\n@app.get(\'/\')\ndef index(request: Request):\n    # TODO something\n    response = request.pfm.services.some_service_name.get(\'path-to-endpoint\')\n    return response\n\n```',
     'author': 'gglassota',
     'author_email': 'gglassota2@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `elefantolib_fastapi-0.9.0/PKG-INFO` & `elefantolib_fastapi-0.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elefantolib-fastapi
-Version: 0.9.0
+Version: 0.9.1
 Summary: 
 Author: gglassota
 Author-email: gglassota2@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

