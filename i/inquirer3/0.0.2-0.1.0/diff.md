# Comparing `tmp/inquirer3-0.0.2.tar.gz` & `tmp/inquirer3-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inquirer3-0.0.2.tar", max compression
+gzip compressed data, was "inquirer3-0.1.0.tar", max compression
```

## Comparing `inquirer3-0.0.2.tar` & `inquirer3-0.1.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     1088 2023-06-22 01:11:34.718871 inquirer3-0.0.2/LICENSE
--rw-r--r--   0        0        0     5467 2023-06-22 01:11:34.718871 inquirer3-0.0.2/README.md
--rw-r--r--   0        0        0     1807 2023-06-22 01:11:46.971066 inquirer3-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      974 2023-06-22 01:11:34.722871 inquirer3-0.0.2/src/inquirer3/__init__.py
--rw-r--r--   0        0        0      412 2023-06-22 01:11:34.722871 inquirer3-0.0.2/src/inquirer3/errors.py
--rw-r--r--   0        0        0      351 2023-06-22 01:11:34.722871 inquirer3-0.0.2/src/inquirer3/events.py
--rw-r--r--   0        0        0      565 2023-06-22 01:11:34.722871 inquirer3-0.0.2/src/inquirer3/prompt.py
--rw-r--r--   0        0        0     9746 2023-06-22 01:11:34.726871 inquirer3-0.0.2/src/inquirer3/questions.py
--rw-r--r--   0        0        0      315 2023-06-22 01:11:34.726871 inquirer3-0.0.2/src/inquirer3/render/__init__.py
--rw-r--r--   0        0        0     6156 2023-06-22 01:11:34.726871 inquirer3-0.0.2/src/inquirer3/render/console/__init__.py
--rw-r--r--   0        0        0     5368 2023-06-22 01:11:34.726871 inquirer3-0.0.2/src/inquirer3/render/console/_checkbox.py
--rw-r--r--   0        0        0      726 2023-06-22 01:11:34.726871 inquirer3-0.0.2/src/inquirer3/render/console/_confirm.py
--rw-r--r--   0        0        0     1091 2023-06-22 01:11:34.726871 inquirer3-0.0.2/src/inquirer3/render/console/_editor.py
--rw-r--r--   0        0        0     3550 2023-06-22 01:11:34.726871 inquirer3-0.0.2/src/inquirer3/render/console/_list.py
--rw-r--r--   0        0        0      103 2023-06-22 01:11:34.726871 inquirer3-0.0.2/src/inquirer3/render/console/_other.py
--rw-r--r--   0        0        0      382 2023-06-22 01:11:34.726871 inquirer3-0.0.2/src/inquirer3/render/console/_password.py
--rw-r--r--   0        0        0       77 2023-06-22 01:11:34.726871 inquirer3-0.0.2/src/inquirer3/render/console/_path.py
--rw-r--r--   0        0        0     2483 2023-06-22 01:11:34.726871 inquirer3-0.0.2/src/inquirer3/render/console/_text.py
--rw-r--r--   0        0        0     1314 2023-06-22 01:11:34.726871 inquirer3-0.0.2/src/inquirer3/render/console/base.py
--rw-r--r--   0        0        0     1457 2023-06-22 01:11:34.726871 inquirer3-0.0.2/src/inquirer3/shortcuts.py
--rw-r--r--   0        0        0     4484 2023-06-22 01:11:34.726871 inquirer3-0.0.2/src/inquirer3/themes.py
--rw-r--r--   0        0        0     6881 1970-01-01 00:00:00.000000 inquirer3-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1088 2023-07-08 18:57:19.916773 inquirer3-0.1.0/LICENSE
+-rw-r--r--   0        0        0     5331 2023-07-08 18:57:19.916773 inquirer3-0.1.0/README.md
+-rw-r--r--   0        0        0     1829 2023-07-08 18:57:31.660991 inquirer3-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0      974 2023-07-08 18:57:19.920774 inquirer3-0.1.0/src/inquirer3/__init__.py
+-rw-r--r--   0        0        0      412 2023-07-08 18:57:19.920774 inquirer3-0.1.0/src/inquirer3/errors.py
+-rw-r--r--   0        0        0      351 2023-07-08 18:57:19.920774 inquirer3-0.1.0/src/inquirer3/events.py
+-rw-r--r--   0        0        0      565 2023-07-08 18:57:19.920774 inquirer3-0.1.0/src/inquirer3/prompt.py
+-rw-r--r--   0        0        0     9746 2023-07-08 18:57:19.920774 inquirer3-0.1.0/src/inquirer3/questions.py
+-rw-r--r--   0        0        0      315 2023-07-08 18:57:19.920774 inquirer3-0.1.0/src/inquirer3/render/__init__.py
+-rw-r--r--   0        0        0     6156 2023-07-08 18:57:19.920774 inquirer3-0.1.0/src/inquirer3/render/console/__init__.py
+-rw-r--r--   0        0        0     5368 2023-07-08 18:57:19.920774 inquirer3-0.1.0/src/inquirer3/render/console/_checkbox.py
+-rw-r--r--   0        0        0      726 2023-07-08 18:57:19.920774 inquirer3-0.1.0/src/inquirer3/render/console/_confirm.py
+-rw-r--r--   0        0        0     1091 2023-07-08 18:57:19.920774 inquirer3-0.1.0/src/inquirer3/render/console/_editor.py
+-rw-r--r--   0        0        0     3550 2023-07-08 18:57:19.920774 inquirer3-0.1.0/src/inquirer3/render/console/_list.py
+-rw-r--r--   0        0        0      103 2023-07-08 18:57:19.920774 inquirer3-0.1.0/src/inquirer3/render/console/_other.py
+-rw-r--r--   0        0        0      382 2023-07-08 18:57:19.920774 inquirer3-0.1.0/src/inquirer3/render/console/_password.py
+-rw-r--r--   0        0        0       77 2023-07-08 18:57:19.920774 inquirer3-0.1.0/src/inquirer3/render/console/_path.py
+-rw-r--r--   0        0        0     2483 2023-07-08 18:57:19.920774 inquirer3-0.1.0/src/inquirer3/render/console/_text.py
+-rw-r--r--   0        0        0     1314 2023-07-08 18:57:19.920774 inquirer3-0.1.0/src/inquirer3/render/console/base.py
+-rw-r--r--   0        0        0     1457 2023-07-08 18:57:19.920774 inquirer3-0.1.0/src/inquirer3/shortcuts.py
+-rw-r--r--   0        0        0     4484 2023-07-08 18:57:19.920774 inquirer3-0.1.0/src/inquirer3/themes.py
+-rw-r--r--   0        0        0     6569 1970-01-01 00:00:00.000000 inquirer3-0.1.0/PKG-INFO
```

### Comparing `inquirer3-0.0.2/LICENSE` & `inquirer3-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `inquirer3-0.0.2/README.md` & `inquirer3-0.1.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -14,34 +14,36 @@
 [tests]: https://github.com/guysalt/python-inquirer3/actions?workflow=Tests
 [codecov]: https://app.codecov.io/gh/guysalt/python-inquirer3
 [pre-commit]: https://github.com/pre-commit/pre-commit
 [black]: https://github.com/psf/black
 
 # python-inquirer3
 
-Collection of common interactive command line user interfaces, based on [Inquirer.js].
+This is a fork of [magmax/python-inquirer]. This one is hopefully more responsive (Issues/PRs/...).
 
-## Goal and Philosophy
+Collection of common interactive command line user interfaces, based on [magmax/python-inquirer].
 
-Born as a [Inquirer.js] clone, it shares part of the goals and philosophy.
+### Goal and Philosophy
 
-So, **Inquirer** should ease the process of asking end user **questions**, **parsing**, **validating** answers, managing **hierarchical prompts** and providing **error feedback**.
+**inquirer3** should ease the process of asking end user **questions**, **parsing**, **validating** answers, managing **hierarchical prompts** and providing **error feedback**.
 
-You can [download the python-inquirer code from GitHub] or [download the wheel from Pypi].
-
-### Platforms support
+## Platforms support
 
 Python-inquirer supports mainly UNIX-based platforms (eq. Mac OS, Linux, etc.). Windows has experimental support, please let us know if there are any problems!
 
 ## Installation
 
+Install the last released version using pip:
+
 ```sh
 pip install inquirer3
 ```
 
+Also, you can [download the python-inquirer code from GitHub] or [download the wheel from Pypi].
+
 ## Documentation
 
 ### Text
 
 ```python
 import re
 
@@ -139,21 +141,18 @@
 ## Contributing
 
 Contributions are very welcome.
 To learn more, see the [Contributor Guide].
 
 ## License
 
-Copyright (c) 2014-2023 Miguel Ángel García ([@magmax_en]), based on [Inquirer.js], by Simon Boudrias ([@vaxilart])
+Copyright (c) 2014-2023 Miguel Ángel García
 
 Distributed under the terms of the [MIT license][license].
 
 <!-- github-only -->
 
 [license]: https://github.com/guysalt/python-inquirer3/blob/main/LICENSE
-[@magmax_en]: https://twitter.com/magmax_en
-[@vaxilart]: https://twitter.com/vaxilart
 [contributor guide]: CONTRIBUTING.md
 [download the python-inquirer code from github]: https://github.com/guysalt/python-inquirer3
-[download the wheel from pypi]: https://pypi.python.org/pypi/inquirer3
-[examples/]: https://github.com/guysalt/python-inquirer3/tree/master/examples
-[inquirer.js]: https://github.com/SBoudrias/Inquirer.js
+[download the wheel from pypi]: https://pypi.org/project/inquirer3/#files
+[magmax/python-inquirer]: https://github.com/magmax/python-inquirer
```

### Comparing `inquirer3-0.0.2/pyproject.toml` & `inquirer3-0.1.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "inquirer3"
-version = "0.0.2"
+version = "0.1.0"
 description = "Collection of common interactive command line user interfaces, based on Inquirer.js"
 authors = ["Guy Salton <guy123121@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/guysalt/python-inquirer3"
 repository = "https://github.com/guysalt/python-inquirer3"
 documentation = "https://python-inquirer3.readthedocs.io/en/latest/"
@@ -19,32 +19,34 @@
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Topic :: Software Development :: User Interfaces",
     "Topic :: Software Development :: Libraries :: Application Frameworks",
 ]
 
 [tool.poetry.dependencies]
-python = ">=3.8"
-blessed = ">=1.19.0"
-readchar = ">=3.0.6"
-python-editor = ">=1.0.4"
+python = "^3.8"
+blessed = "^1.20.0"
+readchar = "^4.0.5"
+python-editor = "^1.0.4"
 
-[tool.poetry.dev-dependencies]
-bandit = ">=1.7.4"
-flake8 = ">=4.0.1,<6.0.0"
-flake8-docstrings = ">=1.6.0"
-furo = ">=2022.9.29"
-isort = ">=5.10.1"
-pexpect = ">=4.8.0"
-pre-commit = ">=2.17.0"
-pre-commit-hooks = ">=4.3.0"
-pyupgrade = ">=2.31.1"
-safety = ">=2.3.1"
-sphinx = ">=5.3.0"
-sphinx-autobuild = ">=2021.3.14"
+[tool.poetry.group.dev.dependencies]
+bandit = "^1.7.5"
+flake8 = "^5.0.0"
+flake8-docstrings = "^1.7.0"
+furo = "^2023.5.20"
+isort = "^5.12.0"
+pexpect = "^4.8.0"
+pre-commit = "^3.3.3"
+pre-commit-hooks = "^4.4.0"
+pyupgrade = "^3.8.0"
+safety = "^2.3.5"
+sphinx = "^7.0.1"
+sphinx-autobuild = "^2021.3.14"
+nox = "^2023.4.22"
+nox-poetry = "^1.0.2"
 
 [tool.coverage.paths]
 source = ["src", "*/site-packages"]
 tests = ["tests", "*/tests"]
 
 [tool.coverage.run]
 branch = true
```

### Comparing `inquirer3-0.0.2/src/inquirer3/__init__.py` & `inquirer3-0.1.0/src/inquirer3/__init__.py`

 * *Files identical despite different names*

### Comparing `inquirer3-0.0.2/src/inquirer3/prompt.py` & `inquirer3-0.1.0/src/inquirer3/prompt.py`

 * *Files identical despite different names*

### Comparing `inquirer3-0.0.2/src/inquirer3/questions.py` & `inquirer3-0.1.0/src/inquirer3/questions.py`

 * *Files identical despite different names*

### Comparing `inquirer3-0.0.2/src/inquirer3/render/console/__init__.py` & `inquirer3-0.1.0/src/inquirer3/render/console/__init__.py`

 * *Files identical despite different names*

### Comparing `inquirer3-0.0.2/src/inquirer3/render/console/_checkbox.py` & `inquirer3-0.1.0/src/inquirer3/render/console/_checkbox.py`

 * *Files identical despite different names*

### Comparing `inquirer3-0.0.2/src/inquirer3/render/console/_confirm.py` & `inquirer3-0.1.0/src/inquirer3/render/console/_confirm.py`

 * *Files identical despite different names*

### Comparing `inquirer3-0.0.2/src/inquirer3/render/console/_editor.py` & `inquirer3-0.1.0/src/inquirer3/render/console/_editor.py`

 * *Files identical despite different names*

### Comparing `inquirer3-0.0.2/src/inquirer3/render/console/_list.py` & `inquirer3-0.1.0/src/inquirer3/render/console/_list.py`

 * *Files identical despite different names*

### Comparing `inquirer3-0.0.2/src/inquirer3/render/console/_text.py` & `inquirer3-0.1.0/src/inquirer3/render/console/_text.py`

 * *Files identical despite different names*

### Comparing `inquirer3-0.0.2/src/inquirer3/render/console/base.py` & `inquirer3-0.1.0/src/inquirer3/render/console/base.py`

 * *Files identical despite different names*

### Comparing `inquirer3-0.0.2/src/inquirer3/shortcuts.py` & `inquirer3-0.1.0/src/inquirer3/shortcuts.py`

 * *Files identical despite different names*

### Comparing `inquirer3-0.0.2/src/inquirer3/themes.py` & `inquirer3-0.1.0/src/inquirer3/themes.py`

 * *Files identical despite different names*

### Comparing `inquirer3-0.0.2/PKG-INFO` & `inquirer3-0.1.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,35 +1,31 @@
 Metadata-Version: 2.1
 Name: inquirer3
-Version: 0.0.2
+Version: 0.1.0
 Summary: Collection of common interactive command line user interfaces, based on Inquirer.js
 Home-page: https://github.com/guysalt/python-inquirer3
 License: MIT
 Author: Guy Salton
 Author-email: guy123121@gmail.com
-Requires-Python: >=3.8
+Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: User Interfaces
-Requires-Dist: blessed (>=1.19.0)
-Requires-Dist: python-editor (>=1.0.4)
-Requires-Dist: readchar (>=3.0.6)
+Requires-Dist: blessed (>=1.20.0,<2.0.0)
+Requires-Dist: python-editor (>=1.0.4,<2.0.0)
+Requires-Dist: readchar (>=4.0.5,<5.0.0)
 Project-URL: Documentation, https://python-inquirer3.readthedocs.io/en/latest/
 Project-URL: Repository, https://github.com/guysalt/python-inquirer3
 Description-Content-Type: text/markdown
 
 [![PyPI](https://img.shields.io/pypi/v/inquirer3.svg)][pypi status]
 [![Status](https://img.shields.io/pypi/status/inquirer3.svg)][pypi status]
 [![Python Version](https://img.shields.io/pypi/pyversions/inquirer3.svg)][pypi status]
@@ -46,34 +42,36 @@
 [tests]: https://github.com/guysalt/python-inquirer3/actions?workflow=Tests
 [codecov]: https://app.codecov.io/gh/guysalt/python-inquirer3
 [pre-commit]: https://github.com/pre-commit/pre-commit
 [black]: https://github.com/psf/black
 
 # python-inquirer3
 
-Collection of common interactive command line user interfaces, based on [Inquirer.js].
+This is a fork of [magmax/python-inquirer]. This one is hopefully more responsive (Issues/PRs/...).
 
-## Goal and Philosophy
+Collection of common interactive command line user interfaces, based on [magmax/python-inquirer].
 
-Born as a [Inquirer.js] clone, it shares part of the goals and philosophy.
+### Goal and Philosophy
 
-So, **Inquirer** should ease the process of asking end user **questions**, **parsing**, **validating** answers, managing **hierarchical prompts** and providing **error feedback**.
+**inquirer3** should ease the process of asking end user **questions**, **parsing**, **validating** answers, managing **hierarchical prompts** and providing **error feedback**.
 
-You can [download the python-inquirer code from GitHub] or [download the wheel from Pypi].
-
-### Platforms support
+## Platforms support
 
 Python-inquirer supports mainly UNIX-based platforms (eq. Mac OS, Linux, etc.). Windows has experimental support, please let us know if there are any problems!
 
 ## Installation
 
+Install the last released version using pip:
+
 ```sh
 pip install inquirer3
 ```
 
+Also, you can [download the python-inquirer code from GitHub] or [download the wheel from Pypi].
+
 ## Documentation
 
 ### Text
 
 ```python
 import re
 
@@ -171,22 +169,19 @@
 ## Contributing
 
 Contributions are very welcome.
 To learn more, see the [Contributor Guide].
 
 ## License
 
-Copyright (c) 2014-2023 Miguel Ángel García ([@magmax_en]), based on [Inquirer.js], by Simon Boudrias ([@vaxilart])
+Copyright (c) 2014-2023 Miguel Ángel García
 
 Distributed under the terms of the [MIT license][license].
 
 <!-- github-only -->
 
 [license]: https://github.com/guysalt/python-inquirer3/blob/main/LICENSE
-[@magmax_en]: https://twitter.com/magmax_en
-[@vaxilart]: https://twitter.com/vaxilart
 [contributor guide]: CONTRIBUTING.md
 [download the python-inquirer code from github]: https://github.com/guysalt/python-inquirer3
-[download the wheel from pypi]: https://pypi.python.org/pypi/inquirer3
-[examples/]: https://github.com/guysalt/python-inquirer3/tree/master/examples
-[inquirer.js]: https://github.com/SBoudrias/Inquirer.js
+[download the wheel from pypi]: https://pypi.org/project/inquirer3/#files
+[magmax/python-inquirer]: https://github.com/magmax/python-inquirer
```

