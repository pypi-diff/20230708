# Comparing `tmp/elefantolib_django-0.1.0.tar.gz` & `tmp/elefantolib_django-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "elefantolib_django-0.1.0.tar", max compression
+gzip compressed data, was "elefantolib_django-0.2.0.tar", max compression
```

## Comparing `elefantolib_django-0.1.0.tar` & `elefantolib_django-0.2.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0        0 2023-06-01 13:24:14.035545 elefantolib_django-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-06-01 13:24:14.035545 elefantolib_django-0.1.0/elefantolib_django/__init__.py
--rw-r--r--   0        0        0     1444 2023-06-01 13:24:14.035545 elefantolib_django-0.1.0/elefantolib_django/middleware.py
--rw-r--r--   0        0        0      145 2023-06-01 13:24:14.035545 elefantolib_django-0.1.0/elefantolib_django/pagination.py
--rw-r--r--   0        0        0      420 2023-06-01 13:24:14.035545 elefantolib_django-0.1.0/elefantolib_django/permissions.py
--rw-r--r--   0        0        0        0 2023-06-01 13:24:14.035545 elefantolib_django-0.1.0/elefantolib_django/serializers/__init__.py
--rw-r--r--   0        0        0      182 2023-06-01 13:24:14.035545 elefantolib_django-0.1.0/elefantolib_django/serializers/mixins.py
--rw-r--r--   0        0        0      835 2023-06-01 13:24:26.971714 elefantolib_django-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      707 1970-01-01 00:00:00.000000 elefantolib_django-0.1.0/setup.py
--rw-r--r--   0        0        0      478 1970-01-01 00:00:00.000000 elefantolib_django-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-07-08 05:56:38.790601 elefantolib_django-0.2.0/README.md
+-rw-r--r--   0        0        0        0 2023-07-08 05:56:38.790601 elefantolib_django-0.2.0/elefantolib_django/__init__.py
+-rw-r--r--   0        0        0     1444 2023-07-08 05:56:38.790601 elefantolib_django-0.2.0/elefantolib_django/middleware.py
+-rw-r--r--   0        0        0      621 2023-07-08 05:56:38.790601 elefantolib_django-0.2.0/elefantolib_django/pagination.py
+-rw-r--r--   0        0        0      420 2023-07-08 05:56:38.790601 elefantolib_django-0.2.0/elefantolib_django/permissions.py
+-rw-r--r--   0        0        0        0 2023-07-08 05:56:38.790601 elefantolib_django-0.2.0/elefantolib_django/serializers/__init__.py
+-rw-r--r--   0        0        0      182 2023-07-08 05:56:38.790601 elefantolib_django-0.2.0/elefantolib_django/serializers/mixins.py
+-rw-r--r--   0        0        0      835 2023-07-08 05:56:56.467125 elefantolib_django-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      707 1970-01-01 00:00:00.000000 elefantolib_django-0.2.0/setup.py
+-rw-r--r--   0        0        0      478 1970-01-01 00:00:00.000000 elefantolib_django-0.2.0/PKG-INFO
```

### Comparing `elefantolib_django-0.1.0/elefantolib_django/middleware.py` & `elefantolib_django-0.2.0/elefantolib_django/middleware.py`

 * *Files identical despite different names*

### Comparing `elefantolib_django-0.1.0/pyproject.toml` & `elefantolib_django-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [tool.poetry]
 name = "elefantolib-django"
-version = "0.1.0"
+version = "0.2.0"
 description = ""
 authors = ["Aibar <bekaybar@gmail.com>"]
 readme = "README.md"
 packages = [{include = "elefantolib_django"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
-django = "^4.2.1"
+django = "^4.2.3"
 djangorestframework = "^3.14.0"
 elefantolib = "^0.12.1"
 
 
 [tool.poetry.group.test.dependencies]
 pytest = "^7.3.1"
 pytest-flake8 = "^1.1.1"
```

### Comparing `elefantolib_django-0.1.0/setup.py` & `elefantolib_django-0.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,21 +4,21 @@
 packages = \
 ['elefantolib_django', 'elefantolib_django.serializers']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['django>=4.2.1,<5.0.0',
+['django>=4.2.3,<5.0.0',
  'djangorestframework>=3.14.0,<4.0.0',
  'elefantolib>=0.12.1,<0.13.0']
 
 setup_kwargs = {
     'name': 'elefantolib-django',
-    'version': '0.1.0',
+    'version': '0.2.0',
     'description': '',
     'long_description': '',
     'author': 'Aibar',
     'author_email': 'bekaybar@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

