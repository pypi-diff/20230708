# Comparing `tmp/django-rest-batteries-1.3.0.tar.gz` & `tmp/django_rest_batteries-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-rest-batteries-1.3.0.tar", last modified: Tue Oct  6 04:22:10 2020, max compression
+gzip compressed data, was "django_rest_batteries-1.4.0.tar", max compression
```

## Comparing `django-rest-batteries-1.3.0.tar` & `django_rest_batteries-1.4.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1073 2020-08-02 08:11:04.860041 django-rest-batteries-1.3.0/LICENSE
--rw-r--r--   0        0        0     4156 2020-09-05 07:23:39.972741 django-rest-batteries-1.3.0/README.md
--rw-r--r--   0        0        0      928 2020-10-06 04:08:33.116521 django-rest-batteries-1.3.0/pyproject.toml
--rw-r--r--   0        0        0        0 2020-08-09 04:47:40.887267 django-rest-batteries-1.3.0/rest_batteries/__init__.py
--rw-r--r--   0        0        0     4628 2020-09-20 07:53:49.824337 django-rest-batteries-1.3.0/rest_batteries/errors_formatter.py
--rw-r--r--   0        0        0      397 2020-08-03 04:56:19.881097 django-rest-batteries-1.3.0/rest_batteries/exception_handlers.py
--rw-r--r--   0        0        0     6572 2020-10-06 04:08:11.360355 django-rest-batteries-1.3.0/rest_batteries/generics.py
--rw-r--r--   0        0        0     4479 2020-10-06 04:08:11.360355 django-rest-batteries-1.3.0/rest_batteries/mixins.py
--rw-r--r--   0        0        0      168 2020-10-06 04:08:11.360355 django-rest-batteries-1.3.0/rest_batteries/views.py
--rw-r--r--   0        0        0     3926 2020-09-05 07:23:39.972741 django-rest-batteries-1.3.0/rest_batteries/viewsets.py
--rw-r--r--   0        0        0     5058 2020-10-06 04:22:10.820744 django-rest-batteries-1.3.0/setup.py
--rw-r--r--   0        0        0     4955 2020-10-06 04:22:10.821156 django-rest-batteries-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-07-08 06:14:38.588960 django_rest_batteries-1.4.0/LICENSE
+-rw-r--r--   0        0        0     4169 2023-07-08 06:14:38.588960 django_rest_batteries-1.4.0/README.md
+-rw-r--r--   0        0        0     1271 2023-07-08 06:14:38.588960 django_rest_batteries-1.4.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-08 06:14:38.588960 django_rest_batteries-1.4.0/rest_batteries/__init__.py
+-rw-r--r--   0        0        0     4628 2023-07-08 06:14:38.588960 django_rest_batteries-1.4.0/rest_batteries/errors_formatter.py
+-rw-r--r--   0        0        0      397 2023-07-08 06:14:38.588960 django_rest_batteries-1.4.0/rest_batteries/exception_handlers.py
+-rw-r--r--   0        0        0     6572 2023-07-08 06:14:38.588960 django_rest_batteries-1.4.0/rest_batteries/generics.py
+-rw-r--r--   0        0        0     4479 2023-07-08 06:14:38.588960 django_rest_batteries-1.4.0/rest_batteries/mixins.py
+-rw-r--r--   0        0        0      168 2023-07-08 06:14:38.588960 django_rest_batteries-1.4.0/rest_batteries/views.py
+-rw-r--r--   0        0        0     3926 2023-07-08 06:14:38.588960 django_rest_batteries-1.4.0/rest_batteries/viewsets.py
+-rw-r--r--   0        0        0     5071 1970-01-01 00:00:00.000000 django_rest_batteries-1.4.0/setup.py
+-rw-r--r--   0        0        0     5016 1970-01-01 00:00:00.000000 django_rest_batteries-1.4.0/PKG-INFO
```

### Comparing `django-rest-batteries-1.3.0/LICENSE` & `django_rest_batteries-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-rest-batteries-1.3.0/README.md` & `django_rest_batteries-1.4.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-[![Build Status](https://travis-ci.org/defineimpossible/django-rest-batteries.svg?branch=master)](https://travis-ci.org/github/defineimpossible/django-rest-batteries)
+[![Test](https://github.com/defineimpossible/django-rest-batteries/actions/workflows/test.yml/badge.svg)](https://github.com/defineimpossible/django-rest-batteries/actions/workflows/test.yml)
 [![Coverage](https://codecov.io/gh/defineimpossible/django-rest-batteries/branch/master/graph/badge.svg)](https://codecov.io/gh/defineimpossible/django-rest-batteries)
 
 # Django REST Framework Batteries
 
 Build clean APIs with DRF faster.
 
 # Overview
@@ -12,17 +12,17 @@
 - Action-based serializers for ViewSets
 - Two serializers per request/response cycle for ViewSets and GenericAPIViews
 - Action-based permissions for ViewSets
 - Single format for all errors
 
 # Requirements
 
-- Python ≥ 3.6
-- Django (2.2, 3.0)
-- Django REST Framework (3.9, 3.10, 3.11)
+- Python ≥ 3.8
+- Django ≥ 3.2
+- Django REST Framework ≥ 3.12
 
 # Installation
 
 ```bash
 $ pip install django-rest-batteries
 ```
```

### Comparing `django-rest-batteries-1.3.0/rest_batteries/errors_formatter.py` & `django_rest_batteries-1.4.0/rest_batteries/errors_formatter.py`

 * *Files identical despite different names*

### Comparing `django-rest-batteries-1.3.0/rest_batteries/generics.py` & `django_rest_batteries-1.4.0/rest_batteries/generics.py`

 * *Files identical despite different names*

### Comparing `django-rest-batteries-1.3.0/rest_batteries/mixins.py` & `django_rest_batteries-1.4.0/rest_batteries/mixins.py`

 * *Files identical despite different names*

### Comparing `django-rest-batteries-1.3.0/rest_batteries/viewsets.py` & `django_rest_batteries-1.4.0/rest_batteries/viewsets.py`

 * *Files identical despite different names*

### Comparing `django-rest-batteries-1.3.0/setup.py` & `django_rest_batteries-1.4.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,27 +4,27 @@
 packages = \
 ['rest_batteries']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['django>=3.0.8,<4.0.0', 'djangorestframework>=3.11.0,<4.0.0']
+['django>=3.2,<4.0', 'djangorestframework>=3.12.2,<4.0.0']
 
 setup_kwargs = {
     'name': 'django-rest-batteries',
-    'version': '1.3.0',
+    'version': '1.4.0',
     'description': 'Build clean APIs with DRF faster',
-    'long_description': '[![Build Status](https://travis-ci.org/defineimpossible/django-rest-batteries.svg?branch=master)](https://travis-ci.org/github/defineimpossible/django-rest-batteries)\n[![Coverage](https://codecov.io/gh/defineimpossible/django-rest-batteries/branch/master/graph/badge.svg)](https://codecov.io/gh/defineimpossible/django-rest-batteries)\n\n# Django REST Framework Batteries\n\nBuild clean APIs with DRF faster.\n\n# Overview\n\nHere\'s a quick overview of what the library has at the moment:\n\n- Action-based serializers for ViewSets\n- Two serializers per request/response cycle for ViewSets and GenericAPIViews\n- Action-based permissions for ViewSets\n- Single format for all errors\n\n# Requirements\n\n- Python ≥ 3.6\n- Django (2.2, 3.0)\n- Django REST Framework (3.9, 3.10, 3.11)\n\n# Installation\n\n```bash\n$ pip install django-rest-batteries\n```\n\n# Usage\n\n## Action-based serializers for ViewSets\n\nEach action can have a separate serializer:\n\n```python\nfrom rest_batteries.mixins import RetrieveModelMixin, ListModelMixin\nfrom rest_batteries.viewsets import GenericViewSet\n...\n\nclass OrderViewSet(RetrieveModelMixin,\n                   ListModelMixin,\n                   GenericViewSet):\n    response_action_serializer_classes = {\n        \'retrieve\': OrderSerializer,\n        \'list\': OrderListSerializer,\n    }\n```\n\n## Two serializers per request/response cycle\n\nWe found that more often than not we need a separate serializer for handling request payload and a separate serializer for generating response data.\n\nHow to achieve it in ViewSet:\n\n```python\nfrom rest_batteries.mixins import CreateModelMixin, ListModelMixin\nfrom rest_batteries.viewsets import GenericViewSet\n...\n\nclass OrderViewSet(CreateModelMixin,\n                   ListModelMixin,\n                   GenericViewSet):\n    request_action_serializer_classes = {\n        \'create\': OrderCreateSerializer,\n    }\n    response_action_serializer_classes = {\n        \'create\': OrderResponseSerializer,\n        \'list\': OrderResponseSerializer,\n        \'cancel\': OrderResponseSerializer,\n    }\n```\n\nHow to achieve it in GenericAPIView:\n\n```python\nfrom rest_batteries.generics import CreateAPIView\n...\n\n\nclass OrderCreateView(CreateAPIView):\n    request_serializer_class = OrderCreateSerializer\n    response_serializer_class = OrderResponseSerializer\n```\n\n## Action-based permissions for ViewSets\n\nEach action can have a separate set of permissions:\n\n```python\nfrom rest_batteries.mixins import CreateModelMixin, UpdateModelMixin, ListModelMixin\nfrom rest_batteries.viewsets import GenericViewSet\nfrom rest_framework.permissions import AllowAny, IsAuthenticated\n...\n\nclass OrderViewSet(CreateModelMixin,\n                   UpdateModelMixin,\n                   ListModelMixin,\n                   GenericViewSet):\n    action_permission_classes = {\n        \'create\': IsAuthenticated,\n        \'update\': [IsAuthenticated, IsOrderOwner],\n        \'list\': AllowAny,\n    }\n```\n\n## Single format for all errors\n\nWe believe that having a single format for all errors is good practice. This will make the process of displaying and handling errors much simpler for clients that use your APIs.\n\nAny error always will be a JSON object with a message, code (identifier of the error), and field if the error is specific to a particular field. How your response could look like:\n\n```python\n{\n    "errors": [\n        {\n            "message": "Delete or cancel all reservations first.",\n            "code": "invalid"\n        },\n        {\n            "message": "Ensure this field has no more than 21 characters.",\n            "code": "max_length",\n            "field": "address.work_phone"\n        },\n        {\n            "message": "This email already exists",\n            "code": "unique",\n            "field": "login_email"\n        }\n    ]\n}\n```\n\nYou will not have a single format out-of-the-box after installation. You need to add an exception handler to your DRF settings:\n\n```python\nREST_FRAMEWORK = {\n    ...\n    \'EXCEPTION_HANDLER\': \'rest_batteries.exception_handlers.errors_formatter_exception_handler\',\n}\n```\n\n# Credits\n\n- [Django-Styleguide by HackSoftware](https://github.com/HackSoftware/Django-Styleguide) - inspiration\n',
+    'long_description': '[![Test](https://github.com/defineimpossible/django-rest-batteries/actions/workflows/test.yml/badge.svg)](https://github.com/defineimpossible/django-rest-batteries/actions/workflows/test.yml)\n[![Coverage](https://codecov.io/gh/defineimpossible/django-rest-batteries/branch/master/graph/badge.svg)](https://codecov.io/gh/defineimpossible/django-rest-batteries)\n\n# Django REST Framework Batteries\n\nBuild clean APIs with DRF faster.\n\n# Overview\n\nHere\'s a quick overview of what the library has at the moment:\n\n- Action-based serializers for ViewSets\n- Two serializers per request/response cycle for ViewSets and GenericAPIViews\n- Action-based permissions for ViewSets\n- Single format for all errors\n\n# Requirements\n\n- Python ≥ 3.8\n- Django ≥ 3.2\n- Django REST Framework ≥ 3.12\n\n# Installation\n\n```bash\n$ pip install django-rest-batteries\n```\n\n# Usage\n\n## Action-based serializers for ViewSets\n\nEach action can have a separate serializer:\n\n```python\nfrom rest_batteries.mixins import RetrieveModelMixin, ListModelMixin\nfrom rest_batteries.viewsets import GenericViewSet\n...\n\nclass OrderViewSet(RetrieveModelMixin,\n                   ListModelMixin,\n                   GenericViewSet):\n    response_action_serializer_classes = {\n        \'retrieve\': OrderSerializer,\n        \'list\': OrderListSerializer,\n    }\n```\n\n## Two serializers per request/response cycle\n\nWe found that more often than not we need a separate serializer for handling request payload and a separate serializer for generating response data.\n\nHow to achieve it in ViewSet:\n\n```python\nfrom rest_batteries.mixins import CreateModelMixin, ListModelMixin\nfrom rest_batteries.viewsets import GenericViewSet\n...\n\nclass OrderViewSet(CreateModelMixin,\n                   ListModelMixin,\n                   GenericViewSet):\n    request_action_serializer_classes = {\n        \'create\': OrderCreateSerializer,\n    }\n    response_action_serializer_classes = {\n        \'create\': OrderResponseSerializer,\n        \'list\': OrderResponseSerializer,\n        \'cancel\': OrderResponseSerializer,\n    }\n```\n\nHow to achieve it in GenericAPIView:\n\n```python\nfrom rest_batteries.generics import CreateAPIView\n...\n\n\nclass OrderCreateView(CreateAPIView):\n    request_serializer_class = OrderCreateSerializer\n    response_serializer_class = OrderResponseSerializer\n```\n\n## Action-based permissions for ViewSets\n\nEach action can have a separate set of permissions:\n\n```python\nfrom rest_batteries.mixins import CreateModelMixin, UpdateModelMixin, ListModelMixin\nfrom rest_batteries.viewsets import GenericViewSet\nfrom rest_framework.permissions import AllowAny, IsAuthenticated\n...\n\nclass OrderViewSet(CreateModelMixin,\n                   UpdateModelMixin,\n                   ListModelMixin,\n                   GenericViewSet):\n    action_permission_classes = {\n        \'create\': IsAuthenticated,\n        \'update\': [IsAuthenticated, IsOrderOwner],\n        \'list\': AllowAny,\n    }\n```\n\n## Single format for all errors\n\nWe believe that having a single format for all errors is good practice. This will make the process of displaying and handling errors much simpler for clients that use your APIs.\n\nAny error always will be a JSON object with a message, code (identifier of the error), and field if the error is specific to a particular field. How your response could look like:\n\n```python\n{\n    "errors": [\n        {\n            "message": "Delete or cancel all reservations first.",\n            "code": "invalid"\n        },\n        {\n            "message": "Ensure this field has no more than 21 characters.",\n            "code": "max_length",\n            "field": "address.work_phone"\n        },\n        {\n            "message": "This email already exists",\n            "code": "unique",\n            "field": "login_email"\n        }\n    ]\n}\n```\n\nYou will not have a single format out-of-the-box after installation. You need to add an exception handler to your DRF settings:\n\n```python\nREST_FRAMEWORK = {\n    ...\n    \'EXCEPTION_HANDLER\': \'rest_batteries.exception_handlers.errors_formatter_exception_handler\',\n}\n```\n\n# Credits\n\n- [Django-Styleguide by HackSoftware](https://github.com/HackSoftware/Django-Styleguide) - inspiration\n',
     'author': 'Define Impossible',
     'author_email': 'hi@defineimpossible.io',
-    'maintainer': None,
-    'maintainer_email': None,
+    'maintainer': 'None',
+    'maintainer_email': 'None',
     'url': 'https://github.com/defineimpossible/django-rest-batteries',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
-    'python_requires': '>=3.6,<4.0',
+    'python_requires': '>=3.8,<4.0',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `django-rest-batteries-1.3.0/PKG-INFO` & `django_rest_batteries-1.4.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 Metadata-Version: 2.1
 Name: django-rest-batteries
-Version: 1.3.0
+Version: 1.4.0
 Summary: Build clean APIs with DRF faster
 Home-page: https://github.com/defineimpossible/django-rest-batteries
 License: MIT
 Keywords: django rest framework,drf,django,batteries
 Author: Define Impossible
 Author-email: hi@defineimpossible.io
-Requires-Python: >=3.6,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
-Requires-Dist: django (>=3.0.8,<4.0.0)
-Requires-Dist: djangorestframework (>=3.11.0,<4.0.0)
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: django (>=3.2,<4.0)
+Requires-Dist: djangorestframework (>=3.12.2,<4.0.0)
 Project-URL: Repository, https://github.com/defineimpossible/django-rest-batteries
 Description-Content-Type: text/markdown
 
-[![Build Status](https://travis-ci.org/defineimpossible/django-rest-batteries.svg?branch=master)](https://travis-ci.org/github/defineimpossible/django-rest-batteries)
+[![Test](https://github.com/defineimpossible/django-rest-batteries/actions/workflows/test.yml/badge.svg)](https://github.com/defineimpossible/django-rest-batteries/actions/workflows/test.yml)
 [![Coverage](https://codecov.io/gh/defineimpossible/django-rest-batteries/branch/master/graph/badge.svg)](https://codecov.io/gh/defineimpossible/django-rest-batteries)
 
 # Django REST Framework Batteries
 
 Build clean APIs with DRF faster.
 
 # Overview
@@ -32,17 +33,17 @@
 - Action-based serializers for ViewSets
 - Two serializers per request/response cycle for ViewSets and GenericAPIViews
 - Action-based permissions for ViewSets
 - Single format for all errors
 
 # Requirements
 
-- Python ≥ 3.6
-- Django (2.2, 3.0)
-- Django REST Framework (3.9, 3.10, 3.11)
+- Python ≥ 3.8
+- Django ≥ 3.2
+- Django REST Framework ≥ 3.12
 
 # Installation
 
 ```bash
 $ pip install django-rest-batteries
 ```
```

