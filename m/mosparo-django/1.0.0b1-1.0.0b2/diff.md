# Comparing `tmp/mosparo_django-1.0.0b1.tar.gz` & `tmp/mosparo_django-1.0.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mosparo_django-1.0.0b1.tar", last modified: Sun Apr 30 13:21:27 2023, max compression
+gzip compressed data, was "mosparo_django-1.0.0b2.tar", last modified: Sat Jul  8 09:22:36 2023, max compression
```

## Comparing `mosparo_django-1.0.0b1.tar` & `mosparo_django-1.0.0b2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxr-x   0 mzo       (5678) mzo       (5678)        0 2023-04-30 13:21:27.341977 mosparo_django-1.0.0b1/
--rw-rw-r--   0 mzo       (5678) mzo       (5678)     1102 2023-04-30 13:21:16.000000 mosparo_django-1.0.0b1/LICENSE
--rw-rw-r--   0 mzo       (5678) mzo       (5678)       44 2023-04-30 13:21:16.000000 mosparo_django-1.0.0b1/MANIFEST.in
--rw-rw-r--   0 mzo       (5678) mzo       (5678)     7617 2023-04-30 13:21:27.341977 mosparo_django-1.0.0b1/PKG-INFO
--rw-rw-r--   0 mzo       (5678) mzo       (5678)     5080 2023-04-30 13:21:16.000000 mosparo_django-1.0.0b1/README.md
-drwxrwxr-x   0 mzo       (5678) mzo       (5678)        0 2023-04-30 13:21:27.337977 mosparo_django-1.0.0b1/mosparo_django/
--rw-rw-r--   0 mzo       (5678) mzo       (5678)      800 2023-04-30 13:21:16.000000 mosparo_django-1.0.0b1/mosparo_django/__init__.py
--rw-rw-r--   0 mzo       (5678) mzo       (5678)      142 2023-04-30 13:21:16.000000 mosparo_django-1.0.0b1/mosparo_django/apps.py
--rw-rw-r--   0 mzo       (5678) mzo       (5678)      403 2023-04-30 13:21:16.000000 mosparo_django-1.0.0b1/mosparo_django/config.py
--rw-rw-r--   0 mzo       (5678) mzo       (5678)     5459 2023-04-30 13:21:16.000000 mosparo_django-1.0.0b1/mosparo_django/fields.py
--rw-rw-r--   0 mzo       (5678) mzo       (5678)      524 2023-04-30 13:21:16.000000 mosparo_django-1.0.0b1/mosparo_django/forms.py
-drwxrwxr-x   0 mzo       (5678) mzo       (5678)        0 2023-04-30 13:21:27.337977 mosparo_django-1.0.0b1/mosparo_django/templates/
-drwxrwxr-x   0 mzo       (5678) mzo       (5678)        0 2023-04-30 13:21:27.341977 mosparo_django-1.0.0b1/mosparo_django/templates/mosparo/
--rw-rw-r--   0 mzo       (5678) mzo       (5678)      331 2023-04-30 13:21:16.000000 mosparo_django-1.0.0b1/mosparo_django/templates/mosparo/box.html
--rw-rw-r--   0 mzo       (5678) mzo       (5678)      878 2023-04-30 13:21:16.000000 mosparo_django-1.0.0b1/mosparo_django/widgets.py
-drwxrwxr-x   0 mzo       (5678) mzo       (5678)        0 2023-04-30 13:21:27.341977 mosparo_django-1.0.0b1/mosparo_django.egg-info/
--rw-rw-r--   0 mzo       (5678) mzo       (5678)     7617 2023-04-30 13:21:27.000000 mosparo_django-1.0.0b1/mosparo_django.egg-info/PKG-INFO
--rw-rw-r--   0 mzo       (5678) mzo       (5678)      535 2023-04-30 13:21:27.000000 mosparo_django-1.0.0b1/mosparo_django.egg-info/SOURCES.txt
--rw-rw-r--   0 mzo       (5678) mzo       (5678)        1 2023-04-30 13:21:27.000000 mosparo_django-1.0.0b1/mosparo_django.egg-info/dependency_links.txt
--rw-rw-r--   0 mzo       (5678) mzo       (5678)       80 2023-04-30 13:21:27.000000 mosparo_django-1.0.0b1/mosparo_django.egg-info/requires.txt
--rw-rw-r--   0 mzo       (5678) mzo       (5678)       15 2023-04-30 13:21:27.000000 mosparo_django-1.0.0b1/mosparo_django.egg-info/top_level.txt
--rw-rw-r--   0 mzo       (5678) mzo       (5678)     1447 2023-04-30 13:21:16.000000 mosparo_django-1.0.0b1/pyproject.toml
--rw-rw-r--   0 mzo       (5678) mzo       (5678)       38 2023-04-30 13:21:27.341977 mosparo_django-1.0.0b1/setup.cfg
-drwxrwxr-x   0 mzo       (5678) mzo       (5678)        0 2023-04-30 13:21:27.341977 mosparo_django-1.0.0b1/tests/
--rw-rw-r--   0 mzo       (5678) mzo       (5678)      297 2023-04-30 13:21:16.000000 mosparo_django-1.0.0b1/tests/test_FrontendConfig.py
--rw-rw-r--   0 mzo       (5678) mzo       (5678)     9907 2023-04-30 13:21:16.000000 mosparo_django-1.0.0b1/tests/test_MosparoField.py
--rw-rw-r--   0 mzo       (5678) mzo       (5678)      879 2023-04-30 13:21:16.000000 mosparo_django-1.0.0b1/tests/test_MosparoForm.py
--rw-rw-r--   0 mzo       (5678) mzo       (5678)      529 2023-04-30 13:21:16.000000 mosparo_django-1.0.0b1/tests/test_MosparoWidget.py
+drwxrwxr-x   0 mzo       (5678) mzo       (5678)        0 2023-07-08 09:22:36.945964 mosparo_django-1.0.0b2/
+-rw-rw-r--   0 mzo       (5678) mzo       (5678)     1102 2023-07-08 09:22:29.000000 mosparo_django-1.0.0b2/LICENSE
+-rw-rw-r--   0 mzo       (5678) mzo       (5678)       44 2023-07-08 09:22:29.000000 mosparo_django-1.0.0b2/MANIFEST.in
+-rw-rw-r--   0 mzo       (5678) mzo       (5678)     7692 2023-07-08 09:22:36.945964 mosparo_django-1.0.0b2/PKG-INFO
+-rw-rw-r--   0 mzo       (5678) mzo       (5678)     5155 2023-07-08 09:22:29.000000 mosparo_django-1.0.0b2/README.md
+drwxrwxr-x   0 mzo       (5678) mzo       (5678)        0 2023-07-08 09:22:36.945964 mosparo_django-1.0.0b2/mosparo_django/
+-rw-rw-r--   0 mzo       (5678) mzo       (5678)      800 2023-07-08 09:22:29.000000 mosparo_django-1.0.0b2/mosparo_django/__init__.py
+-rw-rw-r--   0 mzo       (5678) mzo       (5678)      142 2023-07-08 09:22:29.000000 mosparo_django-1.0.0b2/mosparo_django/apps.py
+-rw-rw-r--   0 mzo       (5678) mzo       (5678)      403 2023-07-08 09:22:29.000000 mosparo_django-1.0.0b2/mosparo_django/config.py
+-rw-rw-r--   0 mzo       (5678) mzo       (5678)     5558 2023-07-08 09:22:29.000000 mosparo_django-1.0.0b2/mosparo_django/fields.py
+-rw-rw-r--   0 mzo       (5678) mzo       (5678)      524 2023-07-08 09:22:29.000000 mosparo_django-1.0.0b2/mosparo_django/forms.py
+drwxrwxr-x   0 mzo       (5678) mzo       (5678)        0 2023-07-08 09:22:36.945964 mosparo_django-1.0.0b2/mosparo_django/templates/
+drwxrwxr-x   0 mzo       (5678) mzo       (5678)        0 2023-07-08 09:22:36.945964 mosparo_django-1.0.0b2/mosparo_django/templates/mosparo/
+-rw-rw-r--   0 mzo       (5678) mzo       (5678)      331 2023-07-08 09:22:29.000000 mosparo_django-1.0.0b2/mosparo_django/templates/mosparo/box.html
+-rw-rw-r--   0 mzo       (5678) mzo       (5678)      878 2023-07-08 09:22:29.000000 mosparo_django-1.0.0b2/mosparo_django/widgets.py
+drwxrwxr-x   0 mzo       (5678) mzo       (5678)        0 2023-07-08 09:22:36.945964 mosparo_django-1.0.0b2/mosparo_django.egg-info/
+-rw-rw-r--   0 mzo       (5678) mzo       (5678)     7692 2023-07-08 09:22:36.000000 mosparo_django-1.0.0b2/mosparo_django.egg-info/PKG-INFO
+-rw-rw-r--   0 mzo       (5678) mzo       (5678)      535 2023-07-08 09:22:36.000000 mosparo_django-1.0.0b2/mosparo_django.egg-info/SOURCES.txt
+-rw-rw-r--   0 mzo       (5678) mzo       (5678)        1 2023-07-08 09:22:36.000000 mosparo_django-1.0.0b2/mosparo_django.egg-info/dependency_links.txt
+-rw-rw-r--   0 mzo       (5678) mzo       (5678)       87 2023-07-08 09:22:36.000000 mosparo_django-1.0.0b2/mosparo_django.egg-info/requires.txt
+-rw-rw-r--   0 mzo       (5678) mzo       (5678)       15 2023-07-08 09:22:36.000000 mosparo_django-1.0.0b2/mosparo_django.egg-info/top_level.txt
+-rw-rw-r--   0 mzo       (5678) mzo       (5678)     1453 2023-07-08 09:22:29.000000 mosparo_django-1.0.0b2/pyproject.toml
+-rw-rw-r--   0 mzo       (5678) mzo       (5678)       38 2023-07-08 09:22:36.945964 mosparo_django-1.0.0b2/setup.cfg
+drwxrwxr-x   0 mzo       (5678) mzo       (5678)        0 2023-07-08 09:22:36.945964 mosparo_django-1.0.0b2/tests/
+-rw-rw-r--   0 mzo       (5678) mzo       (5678)      297 2023-07-08 09:22:29.000000 mosparo_django-1.0.0b2/tests/test_FrontendConfig.py
+-rw-rw-r--   0 mzo       (5678) mzo       (5678)     9907 2023-07-08 09:22:29.000000 mosparo_django-1.0.0b2/tests/test_MosparoField.py
+-rw-rw-r--   0 mzo       (5678) mzo       (5678)      879 2023-07-08 09:22:29.000000 mosparo_django-1.0.0b2/tests/test_MosparoForm.py
+-rw-rw-r--   0 mzo       (5678) mzo       (5678)      529 2023-07-08 09:22:29.000000 mosparo_django-1.0.0b2/tests/test_MosparoWidget.py
```

### Comparing `mosparo_django-1.0.0b1/LICENSE` & `mosparo_django-1.0.0b2/LICENSE`

 * *Files identical despite different names*

### Comparing `mosparo_django-1.0.0b1/PKG-INFO` & `mosparo_django-1.0.0b2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mosparo_django
-Version: 1.0.0b1
+Version: 1.0.0b2
 Summary: A Django app to integrate mosparo into your forms.
 Author-email: mosparo Core Developers <info@mosparo.io>
 License: The MIT License (MIT)
         
         Copyright 2023 mosparo Core Developers and contributors
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -75,21 +75,24 @@
 
 ```commandline
 pip install mosparo_django
 ```
 
 ### Build from source
 
-1. Build the package
+You need the module `build` to build the module from source.
+
+1. Clone the repository
+2. Build the package
 ```commandline
-python setup.py bdist_wheel 
+python -m build
 ```
-2. Install the package
+3. Install the package
 ```commandline
-pip install dist/mosparo_django-1.0.0-py3-none-any.whl
+pip install dist/mosparo_django-1.0.0b1-py3-none-any.whl
 ```
 
 ## Usage
 1. Create a project in your mosparo installation
 2. Edit the `settings.py` file of your project
 2. Add the mosparo integration to the list of enabled apps:
 ```python
```

### Comparing `mosparo_django-1.0.0b1/README.md` & `mosparo_django-1.0.0b2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -23,21 +23,24 @@
 
 ```commandline
 pip install mosparo_django
 ```
 
 ### Build from source
 
-1. Build the package
+You need the module `build` to build the module from source.
+
+1. Clone the repository
+2. Build the package
 ```commandline
-python setup.py bdist_wheel 
+python -m build
 ```
-2. Install the package
+3. Install the package
 ```commandline
-pip install dist/mosparo_django-1.0.0-py3-none-any.whl
+pip install dist/mosparo_django-1.0.0b1-py3-none-any.whl
 ```
 
 ## Usage
 1. Create a project in your mosparo installation
 2. Edit the `settings.py` file of your project
 2. Add the mosparo integration to the list of enabled apps:
 ```python
```

### Comparing `mosparo_django-1.0.0b1/mosparo_django/__init__.py` & `mosparo_django-1.0.0b2/mosparo_django/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from django.conf import settings
 from django.core.exceptions import ImproperlyConfigured
 
 __project__ = 'mosparo_django'
-__version__ = "1.0.0b1"
+__version__ = "1.0.0b2"
 
 settings_types = {
     'MOSPARO_HOST': str,
     'MOSPARO_UUID': str,
     'MOSPARO_PUBLIC_KEY': str,
     'MOSPARO_PRIVATE_KEY': str,
     'MOSPARO_VERIFY_SSL': bool
```

### Comparing `mosparo_django-1.0.0b1/mosparo_django/fields.py` & `mosparo_django-1.0.0b2/mosparo_django/fields.py`

 * *Files 4% similar despite different names*

```diff
@@ -50,14 +50,17 @@
         self.callback_ignored_field_types = callback_ignored_field_types
         self.callback_verifiable_field_types = callback_verifiable_field_types
         self.callback_after_prepare_form_data = callback_after_prepare_form_data
 
         frontend_config = FrontendConfig(self.mosparo_host, self.mosparo_uuid, self.mosparo_public_key)
         self.widget.set_frontend_config(frontend_config)
 
+        # Hide the label for the field, important for the invisible mode.
+        self.label = ''
+
     def validate(self, value):
         return True
 
     def verify_data(self, form: forms.Form):
         api_client = Client(
             self.mosparo_host,
             self.mosparo_public_key,
```

### Comparing `mosparo_django-1.0.0b1/mosparo_django/forms.py` & `mosparo_django-1.0.0b2/mosparo_django/forms.py`

 * *Files identical despite different names*

### Comparing `mosparo_django-1.0.0b1/mosparo_django/widgets.py` & `mosparo_django-1.0.0b2/mosparo_django/widgets.py`

 * *Files identical despite different names*

### Comparing `mosparo_django-1.0.0b1/mosparo_django.egg-info/PKG-INFO` & `mosparo_django-1.0.0b2/mosparo_django.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mosparo-django
-Version: 1.0.0b1
+Version: 1.0.0b2
 Summary: A Django app to integrate mosparo into your forms.
 Author-email: mosparo Core Developers <info@mosparo.io>
 License: The MIT License (MIT)
         
         Copyright 2023 mosparo Core Developers and contributors
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -75,21 +75,24 @@
 
 ```commandline
 pip install mosparo_django
 ```
 
 ### Build from source
 
-1. Build the package
+You need the module `build` to build the module from source.
+
+1. Clone the repository
+2. Build the package
 ```commandline
-python setup.py bdist_wheel 
+python -m build
 ```
-2. Install the package
+3. Install the package
 ```commandline
-pip install dist/mosparo_django-1.0.0-py3-none-any.whl
+pip install dist/mosparo_django-1.0.0b1-py3-none-any.whl
 ```
 
 ## Usage
 1. Create a project in your mosparo installation
 2. Edit the `settings.py` file of your project
 2. Add the mosparo integration to the list of enabled apps:
 ```python
```

### Comparing `mosparo_django-1.0.0b1/mosparo_django.egg-info/SOURCES.txt` & `mosparo_django-1.0.0b2/mosparo_django.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mosparo_django-1.0.0b1/pyproject.toml` & `mosparo_django-1.0.0b2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mosparo_django"
-version = "1.0.0b1"
+version = "1.0.0b2"
 description = "A Django app to integrate mosparo into your forms."
 readme = "README.md"
 authors = [{ name = "mosparo Core Developers", email = "info@mosparo.io" }]
 license = { file = "LICENSE" }
 classifiers = [
     "Development Status :: 4 - Beta",
     "Environment :: Web Environment",
@@ -27,15 +27,15 @@
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "Topic :: Internet",
     "Topic :: Internet :: WWW/HTTP",
 ]
 keywords = ["mosparo", "spam-protection", "accessibility", "captcha", "django", "app"]
 dependencies = [
-    "mosparo_api_client", 
+    "mosparo_api_client>=1.0.1",
     "Django>=3.2"
 ]
 requires-python = ">=3.6"
 
 [project.optional-dependencies]
 dev = ["pytest-runner", "requests-mock", "pytest-django"]
```

### Comparing `mosparo_django-1.0.0b1/tests/test_MosparoField.py` & `mosparo_django-1.0.0b2/tests/test_MosparoField.py`

 * *Files identical despite different names*

### Comparing `mosparo_django-1.0.0b1/tests/test_MosparoForm.py` & `mosparo_django-1.0.0b2/tests/test_MosparoForm.py`

 * *Files identical despite different names*

### Comparing `mosparo_django-1.0.0b1/tests/test_MosparoWidget.py` & `mosparo_django-1.0.0b2/tests/test_MosparoWidget.py`

 * *Files identical despite different names*

