# Comparing `tmp/django-authorization-1.0.1.tar.gz` & `tmp/django-authorization-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-authorization-1.0.1.tar", last modified: Thu Sep  8 01:26:35 2022, max compression
+gzip compressed data, was "django-authorization-1.0.2.tar", last modified: Sat Jul  8 14:35:51 2023, max compression
```

## Comparing `django-authorization-1.0.1.tar` & `django-authorization-1.0.2.tar`

### file list

```diff
@@ -1,39 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-08 01:26:35.583191 django-authorization-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (121)    11357 2022-09-08 01:26:00.000000 django-authorization-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     5912 2022-09-08 01:26:35.583191 django-authorization-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     5084 2022-09-08 01:26:00.000000 django-authorization-1.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-08 01:26:35.579191 django-authorization-1.0.1/dauthz/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-08 01:26:00.000000 django-authorization-1.0.1/dauthz/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-08 01:26:35.579191 django-authorization-1.0.1/dauthz/adapters/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-08 01:26:00.000000 django-authorization-1.0.1/dauthz/adapters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       87 2022-09-08 01:26:00.000000 django-authorization-1.0.1/dauthz/apps.py
--rw-r--r--   0 runner    (1001) docker     (121)     1486 2022-09-08 01:26:00.000000 django-authorization-1.0.1/dauthz/core.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-08 01:26:35.579191 django-authorization-1.0.1/dauthz/decorators/
--rw-r--r--   0 runner    (1001) docker     (121)      102 2022-09-08 01:26:00.000000 django-authorization-1.0.1/dauthz/decorators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      221 2022-09-08 01:26:00.000000 django-authorization-1.0.1/dauthz/decorators/_enforcer_decorator.py
--rw-r--r--   0 runner    (1001) docker     (121)      197 2022-09-08 01:26:00.000000 django-authorization-1.0.1/dauthz/decorators/_request_decorator.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-08 01:26:35.579191 django-authorization-1.0.1/dauthz/management/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-08 01:26:00.000000 django-authorization-1.0.1/dauthz/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-08 01:26:35.583191 django-authorization-1.0.1/dauthz/management/commands/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-08 01:26:00.000000 django-authorization-1.0.1/dauthz/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2490 2022-09-08 01:26:00.000000 django-authorization-1.0.1/dauthz/management/commands/group.py
--rw-r--r--   0 runner    (1001) docker     (121)     1773 2022-09-08 01:26:00.000000 django-authorization-1.0.1/dauthz/management/commands/policy.py
--rw-r--r--   0 runner    (1001) docker     (121)     1858 2022-09-08 01:26:00.000000 django-authorization-1.0.1/dauthz/management/commands/role.py
--rw-r--r--   0 runner    (1001) docker     (121)       40 2022-09-08 01:26:00.000000 django-authorization-1.0.1/dauthz/management/commands/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-08 01:26:35.583191 django-authorization-1.0.1/dauthz/middlewares/
--rw-r--r--   0 runner    (1001) docker     (121)      177 2022-09-08 01:26:00.000000 django-authorization-1.0.1/dauthz/middlewares/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1175 2022-09-08 01:26:00.000000 django-authorization-1.0.1/dauthz/middlewares/enforcer_middleware.py
--rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-09-08 01:26:00.000000 django-authorization-1.0.1/dauthz/middlewares/request_middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-08 01:26:35.583191 django-authorization-1.0.1/dauthz/migrations/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-08 01:26:00.000000 django-authorization-1.0.1/dauthz/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      656 2022-09-08 01:26:00.000000 django-authorization-1.0.1/dauthz/settings.py
--rw-r--r--   0 runner    (1001) docker     (121)      369 2022-09-08 01:26:00.000000 django-authorization-1.0.1/dauthz/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-08 01:26:35.583191 django-authorization-1.0.1/django_authorization.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     5912 2022-09-08 01:26:35.000000 django-authorization-1.0.1/django_authorization.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      850 2022-09-08 01:26:35.000000 django-authorization-1.0.1/django_authorization.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-08 01:26:35.000000 django-authorization-1.0.1/django_authorization.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       29 2022-09-08 01:26:35.000000 django-authorization-1.0.1/django_authorization.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2022-09-08 01:26:35.000000 django-authorization-1.0.1/django_authorization.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       30 2022-09-08 01:26:00.000000 django-authorization-1.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       66 2022-09-08 01:26:35.583191 django-authorization-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2158 2022-09-08 01:26:00.000000 django-authorization-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:35:51.782308 django-authorization-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-08 14:35:14.000000 django-authorization-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6215 2023-07-08 14:35:51.782308 django-authorization-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5387 2023-07-08 14:35:14.000000 django-authorization-1.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:35:51.778308 django-authorization-1.0.2/dauthz/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 14:35:14.000000 django-authorization-1.0.2/dauthz/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:35:51.778308 django-authorization-1.0.2/dauthz/adapters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 14:35:14.000000 django-authorization-1.0.2/dauthz/adapters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-08 14:35:14.000000 django-authorization-1.0.2/dauthz/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-07-08 14:35:14.000000 django-authorization-1.0.2/dauthz/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:35:51.778308 django-authorization-1.0.2/dauthz/decorators/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-08 14:35:14.000000 django-authorization-1.0.2/dauthz/decorators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-07-08 14:35:14.000000 django-authorization-1.0.2/dauthz/decorators/_enforcer_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-07-08 14:35:14.000000 django-authorization-1.0.2/dauthz/decorators/_request_decorator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:35:51.778308 django-authorization-1.0.2/dauthz/management/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 14:35:14.000000 django-authorization-1.0.2/dauthz/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:35:51.778308 django-authorization-1.0.2/dauthz/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 14:35:14.000000 django-authorization-1.0.2/dauthz/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-07-08 14:35:14.000000 django-authorization-1.0.2/dauthz/management/commands/group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-07-08 14:35:14.000000 django-authorization-1.0.2/dauthz/management/commands/policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-07-08 14:35:14.000000 django-authorization-1.0.2/dauthz/management/commands/role.py
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-08 14:35:14.000000 django-authorization-1.0.2/dauthz/management/commands/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:35:51.778308 django-authorization-1.0.2/dauthz/middlewares/
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-07-08 14:35:14.000000 django-authorization-1.0.2/dauthz/middlewares/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-07-08 14:35:14.000000 django-authorization-1.0.2/dauthz/middlewares/enforcer_middleware.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-07-08 14:35:14.000000 django-authorization-1.0.2/dauthz/middlewares/request_middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:35:51.782308 django-authorization-1.0.2/dauthz/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 14:35:14.000000 django-authorization-1.0.2/dauthz/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-07-08 14:35:14.000000 django-authorization-1.0.2/dauthz/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-07-08 14:35:14.000000 django-authorization-1.0.2/dauthz/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:35:51.782308 django-authorization-1.0.2/django_authorization.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6215 2023-07-08 14:35:51.000000 django-authorization-1.0.2/django_authorization.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-07-08 14:35:51.000000 django-authorization-1.0.2/django_authorization.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 14:35:51.000000 django-authorization-1.0.2/django_authorization.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-08 14:35:51.000000 django-authorization-1.0.2/django_authorization.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-08 14:35:51.000000 django-authorization-1.0.2/django_authorization.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-08 14:35:14.000000 django-authorization-1.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-08 14:35:51.790308 django-authorization-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-07-08 14:35:14.000000 django-authorization-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:35:51.782308 django-authorization-1.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-07-08 14:35:14.000000 django-authorization-1.0.2/tests/test_basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-07-08 14:35:14.000000 django-authorization-1.0.2/tests/test_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-07-08 14:35:14.000000 django-authorization-1.0.2/tests/test_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-07-08 14:35:14.000000 django-authorization-1.0.2/tests/test_middleware.py
```

### Comparing `django-authorization-1.0.1/LICENSE` & `django-authorization-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `django-authorization-1.0.1/PKG-INFO` & `django-authorization-1.0.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-authorization
-Version: 1.0.1
+Version: 1.0.2
 Summary: An authorization library that supports access control models like ACL, RBAC, ABAC in Django
 Home-page: https://github.com/pycasbin/django-authorization
 Author: JonLee
 Author-email: leeqvip@gmail.com
 License: Apache 2.0
 Keywords: casbin,django,acl,rbac,abac,auth,authz,authorization,access control,permission
 Classifier: Programming Language :: Python :: 3.6
@@ -16,17 +16,21 @@
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Django Authorization
 
+English | [中文](README_zh.md)
+
+
+
 Django-authorization is an authorization library for Django framework.
 
-[![tests](https://github.com/pycasbin/django-authorization/actions/workflows/release.yml/badge.svg)](https://github.com/pycasbin/django-authorization/actions/workflows/release.yml) [![Coverage Status](https://coveralls.io/repos/github/pycasbin/django-authorization/badge.svg)](https://coveralls.io/github/pycasbin/django-authorization) [![Version](https://img.shields.io/pypi/v/django-authorization.svg)](https://pypi.org/project/django-authorization/) [![Download](https://img.shields.io/pypi/dm/django-authorization.svg)](https://pypi.org/project/django-authorization/) [![Gitter](https://badges.gitter.im/Join%20Chat.svg)](https://gitter.im/casbin/lobby)
+[![tests](https://github.com/pycasbin/django-authorization/actions/workflows/release.yml/badge.svg)](https://github.com/pycasbin/django-authorization/actions/workflows/release.yml) [![Coverage Status](https://coveralls.io/repos/github/pycasbin/django-authorization/badge.svg)](https://coveralls.io/github/pycasbin/django-authorization) [![Version](https://img.shields.io/pypi/v/django-authorization.svg)](https://pypi.org/project/django-authorization/) [![Download](https://img.shields.io/pypi/dm/django-authorization.svg)](https://pypi.org/project/django-authorization/) [![Discord](https://img.shields.io/discord/1022748306096537660?logo=discord&label=discord&color=5865F2)](https://discord.gg/S5UjpzGZjN)
 
 Based on [Casbin](https://github.com/casbin/pycasbin) and [Django-casbin ](https://github.com/pycasbin/django-casbin) (middleware, light weight of this plugin), an authorization library that that supports access control models like ACL, RBAC, ABAC.
 
 ![image](https://user-images.githubusercontent.com/75596353/188881538-a6a99cb1-c88b-4738-bf4f-452be4fb7c2d.png)
 
 
 - [Django Authorization](#django-authorization)
@@ -82,14 +86,16 @@
             # Changes whether Dauthz will log messages to the Logger.
             "ENABLED": False,
         },
     },
 }
 ```
 
+to better prompt the configure method of django-authorization, we made a django-app based on django-authorization, you can see it in [django-authorization-example](https://github.com/pycasbin/django-authorization-example)
+
 ## Usage
 
 ### Some Important Concepts:
 
 such as .conf file, policy, sub, obj, act, please refer to the [casbin website](https://casbin.io/)
 
 ### Middleware Usage
@@ -136,16 +142,16 @@
 The command line operation allows you to operate directly on the enforcer's database. Three sets of commands are available: policy commands, group commands and role commands.
 
 ```shell
 Add/Get policy, usage: 
 python manage.py policy [opt: --enforcer=<enforcer_name>] add <sub> <obj> <act>
 python manage.py policy [opt: --enforcer=<enforcer_name>] get <sub> <obj> <act>
 
-Assign/Get role to user, usage: 
-python manage.py role [opt: --enforcer=<enforcer_name>] assign <user> <role>
+Add/Get role to user, usage: 
+python manage.py role [opt: --enforcer=<enforcer_name>] add <user> <role>
 python manage.py role [opt: --enforcer=<enforcer_name>] get <user>
 
 Add/Get group policy, usage:
 python manage.py group [opt: --enforcer=<enforcer_name>] add <user> <role> [opt:<domain>]
 python manage.py group [opt: --enforcer=<enforcer_name>] get <user> <role> [opt:<domain>]
 ```
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `django-authorization-1.0.1/README.md` & `django-authorization-1.0.2/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 # Django Authorization
 
+English | [中文](README_zh.md)
+
+
+
 Django-authorization is an authorization library for Django framework.
 
-[![tests](https://github.com/pycasbin/django-authorization/actions/workflows/release.yml/badge.svg)](https://github.com/pycasbin/django-authorization/actions/workflows/release.yml) [![Coverage Status](https://coveralls.io/repos/github/pycasbin/django-authorization/badge.svg)](https://coveralls.io/github/pycasbin/django-authorization) [![Version](https://img.shields.io/pypi/v/django-authorization.svg)](https://pypi.org/project/django-authorization/) [![Download](https://img.shields.io/pypi/dm/django-authorization.svg)](https://pypi.org/project/django-authorization/) [![Gitter](https://badges.gitter.im/Join%20Chat.svg)](https://gitter.im/casbin/lobby)
+[![tests](https://github.com/pycasbin/django-authorization/actions/workflows/release.yml/badge.svg)](https://github.com/pycasbin/django-authorization/actions/workflows/release.yml) [![Coverage Status](https://coveralls.io/repos/github/pycasbin/django-authorization/badge.svg)](https://coveralls.io/github/pycasbin/django-authorization) [![Version](https://img.shields.io/pypi/v/django-authorization.svg)](https://pypi.org/project/django-authorization/) [![Download](https://img.shields.io/pypi/dm/django-authorization.svg)](https://pypi.org/project/django-authorization/) [![Discord](https://img.shields.io/discord/1022748306096537660?logo=discord&label=discord&color=5865F2)](https://discord.gg/S5UjpzGZjN)
 
 Based on [Casbin](https://github.com/casbin/pycasbin) and [Django-casbin ](https://github.com/pycasbin/django-casbin) (middleware, light weight of this plugin), an authorization library that that supports access control models like ACL, RBAC, ABAC.
 
 ![image](https://user-images.githubusercontent.com/75596353/188881538-a6a99cb1-c88b-4738-bf4f-452be4fb7c2d.png)
 
 
 - [Django Authorization](#django-authorization)
@@ -62,14 +66,16 @@
             # Changes whether Dauthz will log messages to the Logger.
             "ENABLED": False,
         },
     },
 }
 ```
 
+to better prompt the configure method of django-authorization, we made a django-app based on django-authorization, you can see it in [django-authorization-example](https://github.com/pycasbin/django-authorization-example)
+
 ## Usage
 
 ### Some Important Concepts:
 
 such as .conf file, policy, sub, obj, act, please refer to the [casbin website](https://casbin.io/)
 
 ### Middleware Usage
@@ -116,16 +122,16 @@
 The command line operation allows you to operate directly on the enforcer's database. Three sets of commands are available: policy commands, group commands and role commands.
 
 ```shell
 Add/Get policy, usage: 
 python manage.py policy [opt: --enforcer=<enforcer_name>] add <sub> <obj> <act>
 python manage.py policy [opt: --enforcer=<enforcer_name>] get <sub> <obj> <act>
 
-Assign/Get role to user, usage: 
-python manage.py role [opt: --enforcer=<enforcer_name>] assign <user> <role>
+Add/Get role to user, usage: 
+python manage.py role [opt: --enforcer=<enforcer_name>] add <user> <role>
 python manage.py role [opt: --enforcer=<enforcer_name>] get <user>
 
 Add/Get group policy, usage:
 python manage.py group [opt: --enforcer=<enforcer_name>] add <user> <role> [opt:<domain>]
 python manage.py group [opt: --enforcer=<enforcer_name>] get <user> <role> [opt:<domain>]
 ```
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `django-authorization-1.0.1/dauthz/core.py` & `django-authorization-1.0.2/dauthz/core.py`

 * *Files identical despite different names*

### Comparing `django-authorization-1.0.1/dauthz/management/commands/group.py` & `django-authorization-1.0.2/dauthz/management/commands/group.py`

 * *Files identical despite different names*

### Comparing `django-authorization-1.0.1/dauthz/management/commands/policy.py` & `django-authorization-1.0.2/dauthz/management/commands/policy.py`

 * *Files identical despite different names*

### Comparing `django-authorization-1.0.1/dauthz/management/commands/role.py` & `django-authorization-1.0.2/dauthz/management/commands/role.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from .utils import enforcers
 
 
 class Command(BaseCommand):
     help = """
     Assign/Get role to user,
     usage: 
-        add role for user: python manage.py role [optional: --enforcer=<enforcer_name>] assign <user> <role>
+        add role for user: python manage.py role [optional: --enforcer=<enforcer_name>] add <user> <role>
         get roles of user: python manage.py role [optional: --enforcer=<enforcer_name>] get <user>
     """
 
     def add_arguments(self, parser):
         parser.add_argument("action", type=str, help="ADD/GET role policy")
         parser.add_argument("--enforcer", type=str, help="Name of Enforcer")
         parser.add_argument("user", type=str)
```

### Comparing `django-authorization-1.0.1/dauthz/middlewares/enforcer_middleware.py` & `django-authorization-1.0.2/dauthz/middlewares/enforcer_middleware.py`

 * *Files identical despite different names*

### Comparing `django-authorization-1.0.1/dauthz/middlewares/request_middleware.py` & `django-authorization-1.0.2/dauthz/middlewares/request_middleware.py`

 * *Files identical despite different names*

### Comparing `django-authorization-1.0.1/dauthz/settings.py` & `django-authorization-1.0.2/dauthz/settings.py`

 * *Files identical despite different names*

### Comparing `django-authorization-1.0.1/django_authorization.egg-info/PKG-INFO` & `django-authorization-1.0.2/django_authorization.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-authorization
-Version: 1.0.1
+Version: 1.0.2
 Summary: An authorization library that supports access control models like ACL, RBAC, ABAC in Django
 Home-page: https://github.com/pycasbin/django-authorization
 Author: JonLee
 Author-email: leeqvip@gmail.com
 License: Apache 2.0
 Keywords: casbin,django,acl,rbac,abac,auth,authz,authorization,access control,permission
 Classifier: Programming Language :: Python :: 3.6
@@ -16,17 +16,21 @@
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Django Authorization
 
+English | [中文](README_zh.md)
+
+
+
 Django-authorization is an authorization library for Django framework.
 
-[![tests](https://github.com/pycasbin/django-authorization/actions/workflows/release.yml/badge.svg)](https://github.com/pycasbin/django-authorization/actions/workflows/release.yml) [![Coverage Status](https://coveralls.io/repos/github/pycasbin/django-authorization/badge.svg)](https://coveralls.io/github/pycasbin/django-authorization) [![Version](https://img.shields.io/pypi/v/django-authorization.svg)](https://pypi.org/project/django-authorization/) [![Download](https://img.shields.io/pypi/dm/django-authorization.svg)](https://pypi.org/project/django-authorization/) [![Gitter](https://badges.gitter.im/Join%20Chat.svg)](https://gitter.im/casbin/lobby)
+[![tests](https://github.com/pycasbin/django-authorization/actions/workflows/release.yml/badge.svg)](https://github.com/pycasbin/django-authorization/actions/workflows/release.yml) [![Coverage Status](https://coveralls.io/repos/github/pycasbin/django-authorization/badge.svg)](https://coveralls.io/github/pycasbin/django-authorization) [![Version](https://img.shields.io/pypi/v/django-authorization.svg)](https://pypi.org/project/django-authorization/) [![Download](https://img.shields.io/pypi/dm/django-authorization.svg)](https://pypi.org/project/django-authorization/) [![Discord](https://img.shields.io/discord/1022748306096537660?logo=discord&label=discord&color=5865F2)](https://discord.gg/S5UjpzGZjN)
 
 Based on [Casbin](https://github.com/casbin/pycasbin) and [Django-casbin ](https://github.com/pycasbin/django-casbin) (middleware, light weight of this plugin), an authorization library that that supports access control models like ACL, RBAC, ABAC.
 
 ![image](https://user-images.githubusercontent.com/75596353/188881538-a6a99cb1-c88b-4738-bf4f-452be4fb7c2d.png)
 
 
 - [Django Authorization](#django-authorization)
@@ -82,14 +86,16 @@
             # Changes whether Dauthz will log messages to the Logger.
             "ENABLED": False,
         },
     },
 }
 ```
 
+to better prompt the configure method of django-authorization, we made a django-app based on django-authorization, you can see it in [django-authorization-example](https://github.com/pycasbin/django-authorization-example)
+
 ## Usage
 
 ### Some Important Concepts:
 
 such as .conf file, policy, sub, obj, act, please refer to the [casbin website](https://casbin.io/)
 
 ### Middleware Usage
@@ -136,16 +142,16 @@
 The command line operation allows you to operate directly on the enforcer's database. Three sets of commands are available: policy commands, group commands and role commands.
 
 ```shell
 Add/Get policy, usage: 
 python manage.py policy [opt: --enforcer=<enforcer_name>] add <sub> <obj> <act>
 python manage.py policy [opt: --enforcer=<enforcer_name>] get <sub> <obj> <act>
 
-Assign/Get role to user, usage: 
-python manage.py role [opt: --enforcer=<enforcer_name>] assign <user> <role>
+Add/Get role to user, usage: 
+python manage.py role [opt: --enforcer=<enforcer_name>] add <user> <role>
 python manage.py role [opt: --enforcer=<enforcer_name>] get <user>
 
 Add/Get group policy, usage:
 python manage.py group [opt: --enforcer=<enforcer_name>] add <user> <role> [opt:<domain>]
 python manage.py group [opt: --enforcer=<enforcer_name>] get <user> <role> [opt:<domain>]
 ```
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `django-authorization-1.0.1/django_authorization.egg-info/SOURCES.txt` & `django-authorization-1.0.2/django_authorization.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -22,8 +22,12 @@
 dauthz/middlewares/enforcer_middleware.py
 dauthz/middlewares/request_middleware.py
 dauthz/migrations/__init__.py
 django_authorization.egg-info/PKG-INFO
 django_authorization.egg-info/SOURCES.txt
 django_authorization.egg-info/dependency_links.txt
 django_authorization.egg-info/requires.txt
-django_authorization.egg-info/top_level.txt
+django_authorization.egg-info/top_level.txt
+tests/test_basic.py
+tests/test_command.py
+tests/test_decorator.py
+tests/test_middleware.py
```

### Comparing `django-authorization-1.0.1/setup.py` & `django-authorization-1.0.2/setup.py`

 * *Files identical despite different names*

