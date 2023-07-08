# Comparing `tmp/mailpit-api-client-0.11.0.tar.gz` & `tmp/mailpit-api-client-0.12.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mailpit-api-client-0.11.0.tar", last modified: Sat Jul  8 15:48:08 2023, max compression
+gzip compressed data, was "mailpit-api-client-0.12.0.tar", last modified: Sat Jul  8 17:00:49 2023, max compression
```

## Comparing `mailpit-api-client-0.11.0.tar` & `mailpit-api-client-0.12.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:48:08.113917 mailpit-api-client-0.11.0/
--rw-r--r--   0 runner    (1001) docker     (123)     7633 2023-07-08 15:47:57.000000 mailpit-api-client-0.11.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13071 2023-07-08 15:48:08.113917 mailpit-api-client-0.11.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3035 2023-07-08 15:47:57.000000 mailpit-api-client-0.11.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:48:08.113917 mailpit-api-client-0.11.0/mailpit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 15:47:57.000000 mailpit-api-client-0.11.0/mailpit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:48:08.113917 mailpit-api-client-0.11.0/mailpit/client/
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-08 15:47:57.000000 mailpit-api-client-0.11.0/mailpit/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3857 2023-07-08 15:47:57.000000 mailpit-api-client-0.11.0/mailpit/client/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    11974 2023-07-08 15:47:57.000000 mailpit-api-client-0.11.0/mailpit/client/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-08 15:47:57.000000 mailpit-api-client-0.11.0/mailpit/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:48:08.113917 mailpit-api-client-0.11.0/mailpit/testing/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 15:47:57.000000 mailpit-api-client-0.11.0/mailpit/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-07-08 15:47:57.000000 mailpit-api-client-0.11.0/mailpit/testing/pytest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-07-08 15:47:57.000000 mailpit-api-client-0.11.0/mailpit/testing/unittest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:48:08.113917 mailpit-api-client-0.11.0/mailpit_api_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13071 2023-07-08 15:48:08.000000 mailpit-api-client-0.11.0/mailpit_api_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-07-08 15:48:08.000000 mailpit-api-client-0.11.0/mailpit_api_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 15:48:08.000000 mailpit-api-client-0.11.0/mailpit_api_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-07-08 15:48:08.000000 mailpit-api-client-0.11.0/mailpit_api_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-08 15:48:08.000000 mailpit-api-client-0.11.0/mailpit_api_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2683 2023-07-08 15:47:57.000000 mailpit-api-client-0.11.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 15:48:08.113917 mailpit-api-client-0.11.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 17:00:49.784160 mailpit-api-client-0.12.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     7633 2023-07-08 17:00:37.000000 mailpit-api-client-0.12.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13208 2023-07-08 17:00:49.784160 mailpit-api-client-0.12.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3099 2023-07-08 17:00:37.000000 mailpit-api-client-0.12.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 17:00:49.780160 mailpit-api-client-0.12.0/mailpit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 17:00:37.000000 mailpit-api-client-0.12.0/mailpit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 17:00:49.780160 mailpit-api-client-0.12.0/mailpit/client/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-08 17:00:37.000000 mailpit-api-client-0.12.0/mailpit/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3857 2023-07-08 17:00:37.000000 mailpit-api-client-0.12.0/mailpit/client/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11974 2023-07-08 17:00:37.000000 mailpit-api-client-0.12.0/mailpit/client/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-08 17:00:37.000000 mailpit-api-client-0.12.0/mailpit/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 17:00:49.780160 mailpit-api-client-0.12.0/mailpit/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 17:00:37.000000 mailpit-api-client-0.12.0/mailpit/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-07-08 17:00:37.000000 mailpit-api-client-0.12.0/mailpit/testing/pytest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-07-08 17:00:37.000000 mailpit-api-client-0.12.0/mailpit/testing/unittest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 17:00:49.784160 mailpit-api-client-0.12.0/mailpit_api_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13208 2023-07-08 17:00:49.000000 mailpit-api-client-0.12.0/mailpit_api_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-07-08 17:00:49.000000 mailpit-api-client-0.12.0/mailpit_api_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 17:00:49.000000 mailpit-api-client-0.12.0/mailpit_api_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-07-08 17:00:49.000000 mailpit-api-client-0.12.0/mailpit_api_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-08 17:00:49.000000 mailpit-api-client-0.12.0/mailpit_api_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-07-08 17:00:37.000000 mailpit-api-client-0.12.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 17:00:49.784160 mailpit-api-client-0.12.0/setup.cfg
```

### Comparing `mailpit-api-client-0.11.0/LICENSE` & `mailpit-api-client-0.12.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mailpit-api-client-0.11.0/PKG-INFO` & `mailpit-api-client-0.12.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mailpit-api-client
-Version: 0.11.0
+Version: 0.12.0
 Summary: A Mailpit API Client
 Author-email: Lars Liedtke <lars@familie-liedtke.net>
 License: GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -166,14 +166,15 @@
           If the Library as you received it specifies that a proxy can decide
         whether future versions of the GNU Lesser General Public License shall
         apply, that proxy's public statement of acceptance of any version is
         permanent authorization for you to choose that version for the
         Library.
         
 Project-URL: repository, https://github.com/Corvan/mailpit-api-client
+Project-URL: Documentation, https://corvan.github.io/mailpit-api-client/
 Classifier: Framework :: Pytest
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -195,17 +196,19 @@
 mailpit-api-client
 ==================
 -------------------------------------------------------------------
 API-client for https://github.com/axllent/mailpit written in Python
 -------------------------------------------------------------------
 
 :Authors:
-    Lars Liedtke <lars@familie-liedtke.net>
+    Lars Liedtke <corvan@gmx.de>
 :Version:
-    0.11.0
+    0.12.0
+
+Go to the `documentation <https://corvan.github.io/mailpit-api-client/>`_
 
 ----------
 Motivation
 ----------
 For work, I thought about introducing integration testing.
 We are working with `Odoo <https://github.com/odoo/odoo>`_  and I wanted to test if e-mails created by Odoo really were sent.
 I remembered `mailhog <https://github.com/mailhog/MailHog>`_, which I discovered to be abandoned.
```

### Comparing `mailpit-api-client-0.11.0/README.rst` & `mailpit-api-client-0.12.0/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -2,17 +2,19 @@
 mailpit-api-client
 ==================
 -------------------------------------------------------------------
 API-client for https://github.com/axllent/mailpit written in Python
 -------------------------------------------------------------------
 
 :Authors:
-    Lars Liedtke <lars@familie-liedtke.net>
+    Lars Liedtke <corvan@gmx.de>
 :Version:
-    0.11.0
+    0.12.0
+
+Go to the `documentation <https://corvan.github.io/mailpit-api-client/>`_
 
 ----------
 Motivation
 ----------
 For work, I thought about introducing integration testing.
 We are working with `Odoo <https://github.com/odoo/odoo>`_  and I wanted to test if e-mails created by Odoo really were sent.
 I remembered `mailhog <https://github.com/mailhog/MailHog>`_, which I discovered to be abandoned.
```

### Comparing `mailpit-api-client-0.11.0/mailpit/client/api.py` & `mailpit-api-client-0.12.0/mailpit/client/api.py`

 * *Files identical despite different names*

### Comparing `mailpit-api-client-0.11.0/mailpit/client/models.py` & `mailpit-api-client-0.12.0/mailpit/client/models.py`

 * *Files identical despite different names*

### Comparing `mailpit-api-client-0.11.0/mailpit/testing/pytest.py` & `mailpit-api-client-0.12.0/mailpit/testing/pytest.py`

 * *Files identical despite different names*

### Comparing `mailpit-api-client-0.11.0/mailpit/testing/unittest.py` & `mailpit-api-client-0.12.0/mailpit/testing/unittest.py`

 * *Files identical despite different names*

### Comparing `mailpit-api-client-0.11.0/mailpit_api_client.egg-info/PKG-INFO` & `mailpit-api-client-0.12.0/mailpit_api_client.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mailpit-api-client
-Version: 0.11.0
+Version: 0.12.0
 Summary: A Mailpit API Client
 Author-email: Lars Liedtke <lars@familie-liedtke.net>
 License: GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -166,14 +166,15 @@
           If the Library as you received it specifies that a proxy can decide
         whether future versions of the GNU Lesser General Public License shall
         apply, that proxy's public statement of acceptance of any version is
         permanent authorization for you to choose that version for the
         Library.
         
 Project-URL: repository, https://github.com/Corvan/mailpit-api-client
+Project-URL: Documentation, https://corvan.github.io/mailpit-api-client/
 Classifier: Framework :: Pytest
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -195,17 +196,19 @@
 mailpit-api-client
 ==================
 -------------------------------------------------------------------
 API-client for https://github.com/axllent/mailpit written in Python
 -------------------------------------------------------------------
 
 :Authors:
-    Lars Liedtke <lars@familie-liedtke.net>
+    Lars Liedtke <corvan@gmx.de>
 :Version:
-    0.11.0
+    0.12.0
+
+Go to the `documentation <https://corvan.github.io/mailpit-api-client/>`_
 
 ----------
 Motivation
 ----------
 For work, I thought about introducing integration testing.
 We are working with `Odoo <https://github.com/odoo/odoo>`_  and I wanted to test if e-mails created by Odoo really were sent.
 I remembered `mailhog <https://github.com/mailhog/MailHog>`_, which I discovered to be abandoned.
```

### Comparing `mailpit-api-client-0.11.0/pyproject.toml` & `mailpit-api-client-0.12.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "mailpit-api-client"
-version = "0.11.0"
+version = "0.12.0"
 description = "A Mailpit API Client"
 authors = [{name = "Lars Liedtke", email = "lars@familie-liedtke.net"}]
 requires-python = ">=3.8"
 readme = "README.rst"
 license = {file = "LICENSE"}
 classifiers = [
     "Framework :: Pytest",
@@ -28,15 +28,15 @@
     "ruff",
     "invoke >= 2.0.0",
     "logging518 >= 1.0.0",
 ]
 
 [project.optional-dependencies]
 docs = [
-    "sphinx",
+    "Sphinx",
 ]
 test = [
     "black",
     "mypy>=1.1.1",
     "pylint",
     "respx",
     "pytest>=7",
@@ -47,19 +47,19 @@
 build = [
     "build",
     "twine",
 ]
 
 [project.urls]
 repository = "https://github.com/Corvan/mailpit-api-client"
-
+Documentation = "https://corvan.github.io/mailpit-api-client/"
 
 [tool.poetry]
 name = "mailpit-api-client"
-version = "0.11.0"
+version = "0.12.0"
 description = ""
 authors = ["Lars Liedtke <lars@familie-liedtke.net>"]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 dataclasses_json = "*"
 httpx = "*"
```

