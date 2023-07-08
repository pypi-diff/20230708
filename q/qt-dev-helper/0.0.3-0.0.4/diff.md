# Comparing `tmp/qt_dev_helper-0.0.3.tar.gz` & `tmp/qt_dev_helper-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qt_dev_helper-0.0.3.tar", last modified: Mon Sep  5 21:28:58 2022, max compression
+gzip compressed data, was "qt_dev_helper-0.0.4.tar", last modified: Sat Jul  8 01:14:43 2023, max compression
```

## Comparing `qt_dev_helper-0.0.3.tar` & `qt_dev_helper-0.0.4.tar`

### file list

```diff
@@ -1,90 +1,90 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 21:28:58.342424 qt_dev_helper-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (121)     3597 2022-09-05 21:28:55.000000 qt_dev_helper-0.0.3/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (121)      588 2022-09-05 21:28:55.000000 qt_dev_helper-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      240 2022-09-05 21:28:55.000000 qt_dev_helper-0.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     5423 2022-09-05 21:28:58.342424 qt_dev_helper-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4273 2022-09-05 21:28:55.000000 qt_dev_helper-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 21:28:58.338425 qt_dev_helper-0.0.3/docs/
--rw-r--r--   0 runner    (1001) docker     (121)      699 2022-09-05 21:28:55.000000 qt_dev_helper-0.0.3/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 21:28:58.334425 qt_dev_helper-0.0.3/docs/_templates/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 21:28:58.338425 qt_dev_helper-0.0.3/docs/_templates/autosummary/
--rw-r--r--   0 runner    (1001) docker     (121)      970 2022-09-05 21:28:55.000000 qt_dev_helper-0.0.3/docs/_templates/autosummary/class.rst
--rw-r--r--   0 runner    (1001) docker     (121)       68 2022-09-05 21:28:55.000000 qt_dev_helper-0.0.3/docs/_templates/autosummary/exception.rst
--rw-r--r--   0 runner    (1001) docker     (121)       67 2022-09-05 21:28:55.000000 qt_dev_helper-0.0.3/docs/_templates/autosummary/function.rst
--rw-r--r--   0 runner    (1001) docker     (121)       79 2022-09-05 21:28:55.000000 qt_dev_helper-0.0.3/docs/_templates/autosummary/method.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1450 2022-09-05 21:28:55.000000 qt_dev_helper-0.0.3/docs/_templates/autosummary/module.rst
--rw-r--r--   0 runner    (1001) docker     (121)      196 2022-09-05 21:28:55.000000 qt_dev_helper-0.0.3/docs/api_docs.rst
--rw-r--r--   0 runner    (1001) docker     (121)      146 2022-09-05 21:28:55.000000 qt_dev_helper-0.0.3/docs/cli.rst
--rw-r--r--   0 runner    (1001) docker     (121)     5389 2022-09-05 21:28:55.000000 qt_dev_helper-0.0.3/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)       84 2022-09-05 21:28:55.000000 qt_dev_helper-0.0.3/docs/configuration.rst
--rw-r--r--   0 runner    (1001) docker     (121)       33 2022-09-05 21:28:55.000000 qt_dev_helper-0.0.3/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (121)      371 2022-09-05 21:28:55.000000 qt_dev_helper-0.0.3/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1162 2022-09-05 21:28:55.000000 qt_dev_helper-0.0.3/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1042 2022-09-05 21:28:55.000000 qt_dev_helper-0.0.3/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (121)       81 2022-09-05 21:28:55.000000 qt_dev_helper-0.0.3/docs/usage.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1711 2022-09-05 21:28:55.000000 qt_dev_helper-0.0.3/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 21:28:58.338425 qt_dev_helper-0.0.3/qt_dev_helper/
--rw-r--r--   0 runner    (1001) docker     (121)      141 2022-09-05 21:28:55.000000 qt_dev_helper-0.0.3/qt_dev_helper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      143 2022-09-05 21:28:55.000000 qt_dev_helper-0.0.3/qt_dev_helper/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 21:28:58.338425 qt_dev_helper-0.0.3/qt_dev_helper/cli/
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-05 21:28:55.000000 qt_dev_helper-0.0.3/qt_dev_helper/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      181 2022-09-05 21:28:55.000000 qt_dev_helper-0.0.3/qt_dev_helper/cli/_cli_docs.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 21:28:58.338425 qt_dev_helper-0.0.3/qt_dev_helper/cli/commands/
--rw-r--r--   0 runner    (1001) docker     (121)       28 2022-09-05 21:28:55.000000 qt_dev_helper-0.0.3/qt_dev_helper/cli/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4430 2022-09-05 21:28:55.000000 qt_dev_helper-0.0.3/qt_dev_helper/cli/commands/build.py
--rw-r--r--   0 runner    (1001) docker     (121)     1130 2022-09-05 21:28:55.000000 qt_dev_helper-0.0.3/qt_dev_helper/cli/commands/designer.py
--rw-r--r--   0 runner    (1001) docker     (121)      665 2022-09-05 21:28:55.000000 qt_dev_helper-0.0.3/qt_dev_helper/cli/main_app.py
--rw-r--r--   0 runner    (1001) docker     (121)      634 2022-09-05 21:28:55.000000 qt_dev_helper-0.0.3/qt_dev_helper/cli/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)    14673 2022-09-05 21:28:55.000000 qt_dev_helper-0.0.3/qt_dev_helper/config.py
--rw-r--r--   0 runner    (1001) docker     (121)     4039 2022-09-05 21:28:55.000000 qt_dev_helper-0.0.3/qt_dev_helper/qt_tools.py
--rw-r--r--   0 runner    (1001) docker     (121)     9482 2022-09-05 21:28:55.000000 qt_dev_helper-0.0.3/qt_dev_helper/transpiler.py
--rw-r--r--   0 runner    (1001) docker     (121)     2150 2022-09-05 21:28:55.000000 qt_dev_helper-0.0.3/qt_dev_helper/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 21:28:58.338425 qt_dev_helper-0.0.3/qt_dev_helper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     5423 2022-09-05 21:28:58.000000 qt_dev_helper-0.0.3/qt_dev_helper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1937 2022-09-05 21:28:58.000000 qt_dev_helper-0.0.3/qt_dev_helper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-05 21:28:58.000000 qt_dev_helper-0.0.3/qt_dev_helper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       65 2022-09-05 21:28:58.000000 qt_dev_helper-0.0.3/qt_dev_helper.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-05 21:28:58.000000 qt_dev_helper-0.0.3/qt_dev_helper.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      106 2022-09-05 21:28:58.000000 qt_dev_helper-0.0.3/qt_dev_helper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       14 2022-09-05 21:28:58.000000 qt_dev_helper-0.0.3/qt_dev_helper.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1687 2022-09-05 21:28:58.342424 qt_dev_helper-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-05 21:28:55.000000 qt_dev_helper-0.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 21:28:58.338425 qt_dev_helper-0.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (121)      252 2022-09-05 21:28:55.000000 qt_dev_helper-0.0.3/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 21:28:58.338425 qt_dev_helper-0.0.3/tests/cli/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-05 21:28:55.000000 qt_dev_helper-0.0.3/tests/cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 21:28:58.342424 qt_dev_helper-0.0.3/tests/cli/commands/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-05 21:28:55.000000 qt_dev_helper-0.0.3/tests/cli/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2986 2022-09-05 21:28:55.000000 qt_dev_helper-0.0.3/tests/cli/commands/test_build.py
--rw-r--r--   0 runner    (1001) docker     (121)     1693 2022-09-05 21:28:55.000000 qt_dev_helper-0.0.3/tests/cli/commands/test_designer.py
--rw-r--r--   0 runner    (1001) docker     (121)     1025 2022-09-05 21:28:55.000000 qt_dev_helper-0.0.3/tests/cli/test_main_app.py
--rw-r--r--   0 runner    (1001) docker     (121)      548 2022-09-05 21:28:55.000000 qt_dev_helper-0.0.3/tests/cli/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     1941 2022-09-05 21:28:55.000000 qt_dev_helper-0.0.3/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 21:28:58.342424 qt_dev_helper-0.0.3/tests/data/
--rw-r--r--   0 runner    (1001) docker     (121)      166 2022-09-05 21:28:55.000000 qt_dev_helper-0.0.3/tests/data/MANIFEST.in
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 21:28:58.342424 qt_dev_helper-0.0.3/tests/data/assets/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 21:28:58.342424 qt_dev_helper-0.0.3/tests/data/assets/icons/
--rw-r--r--   0 runner    (1001) docker     (121)      105 2022-09-05 21:28:55.000000 qt_dev_helper-0.0.3/tests/data/assets/icons/circle.svg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 21:28:58.342424 qt_dev_helper-0.0.3/tests/data/assets/styles/
--rw-r--r--   0 runner    (1001) docker     (121)       42 2022-09-05 21:28:55.000000 qt_dev_helper-0.0.3/tests/data/assets/styles/_consts.scss
--rw-r--r--   0 runner    (1001) docker     (121)       86 2022-09-05 21:28:55.000000 qt_dev_helper-0.0.3/tests/data/assets/styles/theme.scss
--rw-r--r--   0 runner    (1001) docker     (121)       91 2022-09-05 21:28:55.000000 qt_dev_helper-0.0.3/tests/data/assets/test_resource.qrc
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 21:28:58.342424 qt_dev_helper-0.0.3/tests/data/assets/ui_files/
--rw-r--r--   0 runner    (1001) docker     (121)     1310 2022-09-05 21:28:55.000000 qt_dev_helper-0.0.3/tests/data/assets/ui_files/minimal.ui
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 21:28:58.342424 qt_dev_helper-0.0.3/tests/data/expected/
--rw-r--r--   0 runner    (1001) docker     (121)     2278 2022-09-05 21:28:55.000000 qt_dev_helper-0.0.3/tests/data/expected/Ui_minimal.h
--rw-r--r--   0 runner    (1001) docker     (121)     2188 2022-09-05 21:28:55.000000 qt_dev_helper-0.0.3/tests/data/expected/Ui_minimal.py
--rw-r--r--   0 runner    (1001) docker     (121)     2180 2022-09-05 21:28:55.000000 qt_dev_helper-0.0.3/tests/data/expected/Ui_minimal_no_from_imports.py
--rw-r--r--   0 runner    (1001) docker     (121)     3081 2022-09-05 21:28:55.000000 qt_dev_helper-0.0.3/tests/data/expected/test_resource.h
--rw-r--r--   0 runner    (1001) docker     (121)     1119 2022-09-05 21:28:55.000000 qt_dev_helper-0.0.3/tests/data/expected/test_resource.py
--rw-r--r--   0 runner    (1001) docker     (121)       53 2022-09-05 21:28:55.000000 qt_dev_helper-0.0.3/tests/data/expected/theme.qss
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 21:28:58.342424 qt_dev_helper-0.0.3/tests/data/outputs/
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-09-05 21:28:55.000000 qt_dev_helper-0.0.3/tests/data/outputs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      730 2022-09-05 21:28:55.000000 qt_dev_helper-0.0.3/tests/data/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      458 2022-09-05 21:28:55.000000 qt_dev_helper-0.0.3/tests/data/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      122 2022-09-05 21:28:55.000000 qt_dev_helper-0.0.3/tests/data/setup.py
--rw-r--r--   0 runner    (1001) docker     (121)      423 2022-09-05 21:28:55.000000 qt_dev_helper-0.0.3/tests/test__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8842 2022-09-05 21:28:55.000000 qt_dev_helper-0.0.3/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (121)     3230 2022-09-05 21:28:55.000000 qt_dev_helper-0.0.3/tests/test_qt_tools.py
--rw-r--r--   0 runner    (1001) docker     (121)     8881 2022-09-05 21:28:55.000000 qt_dev_helper-0.0.3/tests/test_transpiler.py
--rw-r--r--   0 runner    (1001) docker     (121)     2055 2022-09-05 21:28:55.000000 qt_dev_helper-0.0.3/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:14:43.448608 qt_dev_helper-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     3597 2023-07-08 01:14:38.000000 qt_dev_helper-0.0.4/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-07-08 01:14:38.000000 qt_dev_helper-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-07-08 01:14:38.000000 qt_dev_helper-0.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5516 2023-07-08 01:14:43.448608 qt_dev_helper-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4315 2023-07-08 01:14:38.000000 qt_dev_helper-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:14:43.440608 qt_dev_helper-0.0.4/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-07-08 01:14:38.000000 qt_dev_helper-0.0.4/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:14:43.432608 qt_dev_helper-0.0.4/docs/_templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:14:43.440608 qt_dev_helper-0.0.4/docs/_templates/autosummary/
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-07-08 01:14:38.000000 qt_dev_helper-0.0.4/docs/_templates/autosummary/class.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-08 01:14:38.000000 qt_dev_helper-0.0.4/docs/_templates/autosummary/exception.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-08 01:14:38.000000 qt_dev_helper-0.0.4/docs/_templates/autosummary/function.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-08 01:14:38.000000 qt_dev_helper-0.0.4/docs/_templates/autosummary/method.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-07-08 01:14:38.000000 qt_dev_helper-0.0.4/docs/_templates/autosummary/module.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-07-08 01:14:38.000000 qt_dev_helper-0.0.4/docs/api_docs.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-07-08 01:14:38.000000 qt_dev_helper-0.0.4/docs/cli.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5389 2023-07-08 01:14:38.000000 qt_dev_helper-0.0.4/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-08 01:14:38.000000 qt_dev_helper-0.0.4/docs/configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-08 01:14:38.000000 qt_dev_helper-0.0.4/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-07-08 01:14:38.000000 qt_dev_helper-0.0.4/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-07-08 01:14:38.000000 qt_dev_helper-0.0.4/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-07-08 01:14:38.000000 qt_dev_helper-0.0.4/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-08 01:14:38.000000 qt_dev_helper-0.0.4/docs/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-07-08 01:14:38.000000 qt_dev_helper-0.0.4/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:14:43.440608 qt_dev_helper-0.0.4/qt_dev_helper/
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-07-08 01:14:38.000000 qt_dev_helper-0.0.4/qt_dev_helper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-07-08 01:14:38.000000 qt_dev_helper-0.0.4/qt_dev_helper/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:14:43.440608 qt_dev_helper-0.0.4/qt_dev_helper/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:14:38.000000 qt_dev_helper-0.0.4/qt_dev_helper/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-07-08 01:14:38.000000 qt_dev_helper-0.0.4/qt_dev_helper/cli/_cli_docs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:14:43.440608 qt_dev_helper-0.0.4/qt_dev_helper/cli/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-08 01:14:38.000000 qt_dev_helper-0.0.4/qt_dev_helper/cli/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4430 2023-07-08 01:14:38.000000 qt_dev_helper-0.0.4/qt_dev_helper/cli/commands/build.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-07-08 01:14:38.000000 qt_dev_helper-0.0.4/qt_dev_helper/cli/commands/designer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-07-08 01:14:38.000000 qt_dev_helper-0.0.4/qt_dev_helper/cli/main_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-07-08 01:14:38.000000 qt_dev_helper-0.0.4/qt_dev_helper/cli/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14673 2023-07-08 01:14:38.000000 qt_dev_helper-0.0.4/qt_dev_helper/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4039 2023-07-08 01:14:38.000000 qt_dev_helper-0.0.4/qt_dev_helper/qt_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9482 2023-07-08 01:14:38.000000 qt_dev_helper-0.0.4/qt_dev_helper/transpiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-07-08 01:14:38.000000 qt_dev_helper-0.0.4/qt_dev_helper/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:14:43.440608 qt_dev_helper-0.0.4/qt_dev_helper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5516 2023-07-08 01:14:43.000000 qt_dev_helper-0.0.4/qt_dev_helper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-07-08 01:14:43.000000 qt_dev_helper-0.0.4/qt_dev_helper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:14:43.000000 qt_dev_helper-0.0.4/qt_dev_helper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-08 01:14:43.000000 qt_dev_helper-0.0.4/qt_dev_helper.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:14:43.000000 qt_dev_helper-0.0.4/qt_dev_helper.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-07-08 01:14:43.000000 qt_dev_helper-0.0.4/qt_dev_helper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-08 01:14:43.000000 qt_dev_helper-0.0.4/qt_dev_helper.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-07-08 01:14:43.448608 qt_dev_helper-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:14:38.000000 qt_dev_helper-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:14:43.444608 qt_dev_helper-0.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-07-08 01:14:38.000000 qt_dev_helper-0.0.4/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:14:43.444608 qt_dev_helper-0.0.4/tests/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:14:38.000000 qt_dev_helper-0.0.4/tests/cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:14:43.444608 qt_dev_helper-0.0.4/tests/cli/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:14:38.000000 qt_dev_helper-0.0.4/tests/cli/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2986 2023-07-08 01:14:38.000000 qt_dev_helper-0.0.4/tests/cli/commands/test_build.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-07-08 01:14:38.000000 qt_dev_helper-0.0.4/tests/cli/commands/test_designer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-07-08 01:14:38.000000 qt_dev_helper-0.0.4/tests/cli/test_main_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-07-08 01:14:38.000000 qt_dev_helper-0.0.4/tests/cli/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-07-08 01:14:38.000000 qt_dev_helper-0.0.4/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:14:43.444608 qt_dev_helper-0.0.4/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-08 01:14:38.000000 qt_dev_helper-0.0.4/tests/data/MANIFEST.in
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:14:43.444608 qt_dev_helper-0.0.4/tests/data/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:14:43.444608 qt_dev_helper-0.0.4/tests/data/assets/icons/
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-08 01:14:38.000000 qt_dev_helper-0.0.4/tests/data/assets/icons/circle.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:14:43.444608 qt_dev_helper-0.0.4/tests/data/assets/styles/
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-08 01:14:38.000000 qt_dev_helper-0.0.4/tests/data/assets/styles/_consts.scss
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-08 01:14:38.000000 qt_dev_helper-0.0.4/tests/data/assets/styles/theme.scss
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-08 01:14:38.000000 qt_dev_helper-0.0.4/tests/data/assets/test_resource.qrc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:14:43.444608 qt_dev_helper-0.0.4/tests/data/assets/ui_files/
+-rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-07-08 01:14:38.000000 qt_dev_helper-0.0.4/tests/data/assets/ui_files/minimal.ui
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:14:43.448608 qt_dev_helper-0.0.4/tests/data/expected/
+-rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-07-08 01:14:38.000000 qt_dev_helper-0.0.4/tests/data/expected/Ui_minimal.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2187 2023-07-08 01:14:38.000000 qt_dev_helper-0.0.4/tests/data/expected/Ui_minimal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-07-08 01:14:38.000000 qt_dev_helper-0.0.4/tests/data/expected/Ui_minimal_no_from_imports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-07-08 01:14:38.000000 qt_dev_helper-0.0.4/tests/data/expected/test_resource.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-07-08 01:14:38.000000 qt_dev_helper-0.0.4/tests/data/expected/test_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-08 01:14:38.000000 qt_dev_helper-0.0.4/tests/data/expected/theme.qss
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:14:43.448608 qt_dev_helper-0.0.4/tests/data/outputs/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-08 01:14:38.000000 qt_dev_helper-0.0.4/tests/data/outputs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-07-08 01:14:38.000000 qt_dev_helper-0.0.4/tests/data/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-07-08 01:14:38.000000 qt_dev_helper-0.0.4/tests/data/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-07-08 01:14:38.000000 qt_dev_helper-0.0.4/tests/data/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-07-08 01:14:38.000000 qt_dev_helper-0.0.4/tests/test__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8842 2023-07-08 01:14:38.000000 qt_dev_helper-0.0.4/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3230 2023-07-08 01:14:38.000000 qt_dev_helper-0.0.4/tests/test_qt_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8881 2023-07-08 01:14:38.000000 qt_dev_helper-0.0.4/tests/test_transpiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2055 2023-07-08 01:14:38.000000 qt_dev_helper-0.0.4/tests/test_utils.py
```

### Comparing `qt_dev_helper-0.0.3/CONTRIBUTING.rst` & `qt_dev_helper-0.0.4/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `qt_dev_helper-0.0.3/LICENSE` & `qt_dev_helper-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `qt_dev_helper-0.0.3/PKG-INFO` & `qt_dev_helper-0.0.4/qt_dev_helper.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: qt_dev_helper
-Version: 0.0.3
+Name: qt-dev-helper
+Version: 0.0.4
 Summary: Tool to help developing Qt applications
 Home-page: https://github.com/s-weigand/qt-dev-helper
 Author: Sebastian Weigand
 Author-email: s.weigand.phy@gmail.com
 License: Apache Software License 2.0
 Project-URL: Documentation, https://qt-dev-helper.readthedocs.io
 Project-URL: Changelog, https://qt-dev-helper.readthedocs.io/en/latest/history.html
@@ -16,40 +16,50 @@
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Provides-Extra: pyside6
 Provides-Extra: cli
+Provides-Extra: pyside6
 License-File: LICENSE
 
 # Qt Dev Helper
 
-<!-- [![PyPi Version](https://img.shields.io/pypi/v/qt_dev_helper.svg)](https://pypi.org/project/qt-dev-helper/)
-[![Supported Python Versions](https://img.shields.io/pypi/pyversions/qt_dev_helper.svg)](https://pypi.org/project/qt-dev-helper/) -->
-
-<!-- [![Conda Version](https://img.shields.io/conda/vn/conda-forge/qt-dev-helper.svg)](https://anaconda.org/conda-forge/qt-dev-helper) -->
-
+[![PyPi Version](https://img.shields.io/pypi/v/qt_dev_helper.svg)](https://pypi.org/project/qt-dev-helper/)
+[![Supported Python Versions](https://img.shields.io/pypi/pyversions/qt_dev_helper.svg)](https://pypi.org/project/qt-dev-helper/)
+[![Conda Version](https://img.shields.io/conda/vn/conda-forge/qt-dev-helper.svg)](https://anaconda.org/conda-forge/qt-dev-helper)
 [![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 
 [![Actions Status](https://github.com/s-weigand/qt-dev-helper/workflows/Tests/badge.svg)](https://github.com/s-weigand/qt-dev-helper/actions)
 [![Documentation Status](https://readthedocs.org/projects/qt-dev-helper/badge/?version=latest)](https://qt-dev-helper.readthedocs.io/en/latest/?badge=latest)
 [![codecov](https://codecov.io/gh/s-weigand/qt-dev-helper/branch/main/graph/badge.svg)](https://codecov.io/gh/s-weigand/qt-dev-helper)
 [![Documentation Coverage](https://raw.githubusercontent.com/s-weigand/qt-dev-helper/main/docs/_static/interrogate_badge.svg)](https://github.com/s-weigand/qt-dev-helper)
+[![Code style Python: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 [![All Contributors](https://img.shields.io/github/all-contributors/s-weigand/qt-dev-helper)](#contributors)
 
-[![Code style Python: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
-
 Toolbox to help develop Qt applications, improving the usability of the existing tooling.
 
+## Installation
+
+```console
+pip install qt-dev-helper
+```
+
+OR
+
+```console
+conda install -c conda-forge qt-dev-helper
+```
+
 ## Features
 
 - Usable as Library and/or CLI tool
 - Compatible with [PEP517](https://peps.python.org/pep-0517/) build system
   ([see test case](https://github.com/s-weigand/qt-dev-helper/blob/main/tests/data/pyproject.toml))
 - CLI auto completion
 - Project wide configuration in `pyproject.toml`
@@ -68,20 +78,14 @@
 ## Planned features
 
 - Stand alone executable for each release (Windows)
 - File watch mode
 - `qss` injection into `*.ui` files
 - [`pre-commit`](https://pre-commit.com/) hooks
 
-## Installation
-
-```console
-pip install qt-dev-helper
-```
-
 ## FAQ
 
 - Q: Why is `PyQt5` not supported?
 
   A: `PyQt5` only ships a python specific version of `uic` and `rcc` breaking the tool API and
   compatibility with cpp projects.
   Use the matching version of `qt5-applications` as Qt tooling supplier.
```

#### html2text {}

```diff
@@ -1,53 +1,59 @@
-Metadata-Version: 2.1 Name: qt_dev_helper Version: 0.0.3 Summary: Tool to help
+Metadata-Version: 2.1 Name: qt-dev-helper Version: 0.0.4 Summary: Tool to help
 developing Qt applications Home-page: https://github.com/s-weigand/qt-dev-
 helper Author: Sebastian Weigand Author-email: s.weigand.phy@gmail.com License:
 Apache Software License 2.0 Project-URL: Documentation, https://qt-dev-
 helper.readthedocs.io Project-URL: Changelog, https://qt-dev-
 helper.readthedocs.io/en/latest/history.html Project-URL: Source, https://
 github.com/s-weigand/qt-dev-helper Project-URL: Tracker, https://github.com/s-
 weigand/qt-dev-helper/issues Keywords: qt_dev_helper Classifier: Development
 Status :: 2 - Pre-Alpha Classifier: Intended Audience :: Developers Classifier:
 License :: OSI Approved :: Apache Software License Classifier: Natural Language
 :: English Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3 :: Only Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
-Programming Language :: Python :: 3.10 Requires-Python: >=3.8 Description-
-Content-Type: text/markdown Provides-Extra: pyside6 Provides-Extra: cli
-License-File: LICENSE # Qt Dev Helper   [![License](https://img.shields.io/
-badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-
-2.0) [![Actions Status](https://github.com/s-weigand/qt-dev-helper/workflows/
-Tests/badge.svg)](https://github.com/s-weigand/qt-dev-helper/actions) [!
-[Documentation Status](https://readthedocs.org/projects/qt-dev-helper/badge/
-?version=latest)](https://qt-dev-helper.readthedocs.io/en/latest/?badge=latest)
-[![codecov](https://codecov.io/gh/s-weigand/qt-dev-helper/branch/main/graph/
-badge.svg)](https://codecov.io/gh/s-weigand/qt-dev-helper) [![Documentation
-Coverage](https://raw.githubusercontent.com/s-weigand/qt-dev-helper/main/docs/
-_static/interrogate_badge.svg)](https://github.com/s-weigand/qt-dev-helper) [!
-[All Contributors](https://img.shields.io/github/all-contributors/s-weigand/qt-
-dev-helper)](#contributors) [![Code style Python: black](https://
-img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/
-black) Toolbox to help develop Qt applications, improving the usability of the
-existing tooling. ## Features - Usable as Library and/or CLI tool - Compatible
-with [PEP517](https://peps.python.org/pep-0517/) build system ([see test case]
-(https://github.com/s-weigand/qt-dev-helper/blob/main/tests/data/
-pyproject.toml)) - CLI auto completion - Project wide configuration in
-`pyproject.toml` - Recursive asset compiler for Qt projects (using `uic` and
-`rcc`): - `*.ui` -> `*.py` - `*.qrc` -> `*.py` - `*.ui` -> `*.h` - `*.qrc` -
-> `*.h` - `*.scss` -> `*.qss` - Support for multiple Qt tooling suppliers -
-`PySide6-Essentials` - `qt6-applications` - `qt5-applications` - Ability to
-open all files in a folder in QtDesigner ## Planned features - Stand alone
-executable for each release (Windows) - File watch mode - `qss` injection into
-`*.ui` files - [`pre-commit`](https://pre-commit.com/) hooks ## Installation
-```console pip install qt-dev-helper ``` ## FAQ - Q: Why is `PyQt5` not
-supported? A: `PyQt5` only ships a python specific version of `uic` and `rcc`
-breaking the tool API and compatibility with cpp projects. Use the matching
-version of `qt5-applications` as Qt tooling supplier. ## Contributors â¨
-Thanks goes out to these wonderful people ([emoji key](https://
-allcontributors.org/docs/en/emoji-key)):
+Programming Language :: Python :: 3.10 Classifier: Programming Language ::
+Python :: 3.11 Requires-Python: >=3.8 Description-Content-Type: text/markdown
+Provides-Extra: cli Provides-Extra: pyside6 License-File: LICENSE # Qt Dev
+Helper [![PyPi Version](https://img.shields.io/pypi/v/qt_dev_helper.svg)]
+(https://pypi.org/project/qt-dev-helper/) [![Supported Python Versions](https:/
+/img.shields.io/pypi/pyversions/qt_dev_helper.svg)](https://pypi.org/project/
+qt-dev-helper/) [![Conda Version](https://img.shields.io/conda/vn/conda-forge/
+qt-dev-helper.svg)](https://anaconda.org/conda-forge/qt-dev-helper) [![License]
+(https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://
+opensource.org/licenses/Apache-2.0) [![Actions Status](https://github.com/s-
+weigand/qt-dev-helper/workflows/Tests/badge.svg)](https://github.com/s-weigand/
+qt-dev-helper/actions) [![Documentation Status](https://readthedocs.org/
+projects/qt-dev-helper/badge/?version=latest)](https://qt-dev-
+helper.readthedocs.io/en/latest/?badge=latest) [![codecov](https://codecov.io/
+gh/s-weigand/qt-dev-helper/branch/main/graph/badge.svg)](https://codecov.io/gh/
+s-weigand/qt-dev-helper) [![Documentation Coverage](https://
+raw.githubusercontent.com/s-weigand/qt-dev-helper/main/docs/_static/
+interrogate_badge.svg)](https://github.com/s-weigand/qt-dev-helper) [![Code
+style Python: black](https://img.shields.io/badge/code%20style-black-
+000000.svg)](https://github.com/psf/black) [![All Contributors](https://
+img.shields.io/github/all-contributors/s-weigand/qt-dev-helper)](#contributors)
+Toolbox to help develop Qt applications, improving the usability of the
+existing tooling. ## Installation ```console pip install qt-dev-helper ``` OR
+```console conda install -c conda-forge qt-dev-helper ``` ## Features - Usable
+as Library and/or CLI tool - Compatible with [PEP517](https://peps.python.org/
+pep-0517/) build system ([see test case](https://github.com/s-weigand/qt-dev-
+helper/blob/main/tests/data/pyproject.toml)) - CLI auto completion - Project
+wide configuration in `pyproject.toml` - Recursive asset compiler for Qt
+projects (using `uic` and `rcc`): - `*.ui` -> `*.py` - `*.qrc` -> `*.py` -
+`*.ui` -> `*.h` - `*.qrc` -> `*.h` - `*.scss` -> `*.qss` - Support for multiple
+Qt tooling suppliers - `PySide6-Essentials` - `qt6-applications` - `qt5-
+applications` - Ability to open all files in a folder in QtDesigner ## Planned
+features - Stand alone executable for each release (Windows) - File watch mode
+- `qss` injection into `*.ui` files - [`pre-commit`](https://pre-commit.com/
+) hooks ## FAQ - Q: Why is `PyQt5` not supported? A: `PyQt5` only ships a
+python specific version of `uic` and `rcc` breaking the tool API and
+compatibility with cpp projects. Use the matching version of `qt5-applications`
+as Qt tooling supplier. ## Contributors â¨ Thanks goes out to these wonderful
+people ([emoji key](https://allcontributors.org/docs/en/emoji-key)):
 
                         Sebastian_Weigand                             Joris
                                                                    Snellenburg
                ð» ð¤ ð§ ð ð â �           �
                                                                       ð
    This project follows the [all-contributors](https://github.com/all-
 contributors/all-contributors) specification. Contributions of any kind are
```

### Comparing `qt_dev_helper-0.0.3/README.md` & `qt_dev_helper-0.0.4/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,36 @@
 # Qt Dev Helper
 
-<!-- [![PyPi Version](https://img.shields.io/pypi/v/qt_dev_helper.svg)](https://pypi.org/project/qt-dev-helper/)
-[![Supported Python Versions](https://img.shields.io/pypi/pyversions/qt_dev_helper.svg)](https://pypi.org/project/qt-dev-helper/) -->
-
-<!-- [![Conda Version](https://img.shields.io/conda/vn/conda-forge/qt-dev-helper.svg)](https://anaconda.org/conda-forge/qt-dev-helper) -->
-
+[![PyPi Version](https://img.shields.io/pypi/v/qt_dev_helper.svg)](https://pypi.org/project/qt-dev-helper/)
+[![Supported Python Versions](https://img.shields.io/pypi/pyversions/qt_dev_helper.svg)](https://pypi.org/project/qt-dev-helper/)
+[![Conda Version](https://img.shields.io/conda/vn/conda-forge/qt-dev-helper.svg)](https://anaconda.org/conda-forge/qt-dev-helper)
 [![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 
 [![Actions Status](https://github.com/s-weigand/qt-dev-helper/workflows/Tests/badge.svg)](https://github.com/s-weigand/qt-dev-helper/actions)
 [![Documentation Status](https://readthedocs.org/projects/qt-dev-helper/badge/?version=latest)](https://qt-dev-helper.readthedocs.io/en/latest/?badge=latest)
 [![codecov](https://codecov.io/gh/s-weigand/qt-dev-helper/branch/main/graph/badge.svg)](https://codecov.io/gh/s-weigand/qt-dev-helper)
 [![Documentation Coverage](https://raw.githubusercontent.com/s-weigand/qt-dev-helper/main/docs/_static/interrogate_badge.svg)](https://github.com/s-weigand/qt-dev-helper)
+[![Code style Python: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 [![All Contributors](https://img.shields.io/github/all-contributors/s-weigand/qt-dev-helper)](#contributors)
 
-[![Code style Python: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
-
 Toolbox to help develop Qt applications, improving the usability of the existing tooling.
 
+## Installation
+
+```console
+pip install qt-dev-helper
+```
+
+OR
+
+```console
+conda install -c conda-forge qt-dev-helper
+```
+
 ## Features
 
 - Usable as Library and/or CLI tool
 - Compatible with [PEP517](https://peps.python.org/pep-0517/) build system
   ([see test case](https://github.com/s-weigand/qt-dev-helper/blob/main/tests/data/pyproject.toml))
 - CLI auto completion
 - Project wide configuration in `pyproject.toml`
@@ -40,20 +49,14 @@
 ## Planned features
 
 - Stand alone executable for each release (Windows)
 - File watch mode
 - `qss` injection into `*.ui` files
 - [`pre-commit`](https://pre-commit.com/) hooks
 
-## Installation
-
-```console
-pip install qt-dev-helper
-```
-
 ## FAQ
 
 - Q: Why is `PyQt5` not supported?
 
   A: `PyQt5` only ships a python specific version of `uic` and `rcc` breaking the tool API and
   compatibility with cpp projects.
   Use the matching version of `qt5-applications` as Qt tooling supplier.
```

#### html2text {}

```diff
@@ -1,34 +1,40 @@
-# Qt Dev Helper   [![License](https://img.shields.io/badge/License-
+# Qt Dev Helper [![PyPi Version](https://img.shields.io/pypi/v/
+qt_dev_helper.svg)](https://pypi.org/project/qt-dev-helper/) [![Supported
+Python Versions](https://img.shields.io/pypi/pyversions/qt_dev_helper.svg)]
+(https://pypi.org/project/qt-dev-helper/) [![Conda Version](https://
+img.shields.io/conda/vn/conda-forge/qt-dev-helper.svg)](https://anaconda.org/
+conda-forge/qt-dev-helper) [![License](https://img.shields.io/badge/License-
 Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0) [![Actions
 Status](https://github.com/s-weigand/qt-dev-helper/workflows/Tests/badge.svg)]
 (https://github.com/s-weigand/qt-dev-helper/actions) [![Documentation Status]
 (https://readthedocs.org/projects/qt-dev-helper/badge/?version=latest)](https:/
 /qt-dev-helper.readthedocs.io/en/latest/?badge=latest) [![codecov](https://
 codecov.io/gh/s-weigand/qt-dev-helper/branch/main/graph/badge.svg)](https://
 codecov.io/gh/s-weigand/qt-dev-helper) [![Documentation Coverage](https://
 raw.githubusercontent.com/s-weigand/qt-dev-helper/main/docs/_static/
-interrogate_badge.svg)](https://github.com/s-weigand/qt-dev-helper) [![All
-Contributors](https://img.shields.io/github/all-contributors/s-weigand/qt-dev-
-helper)](#contributors) [![Code style Python: black](https://img.shields.io/
-badge/code%20style-black-000000.svg)](https://github.com/psf/black) Toolbox to
-help develop Qt applications, improving the usability of the existing tooling.
-## Features - Usable as Library and/or CLI tool - Compatible with [PEP517]
-(https://peps.python.org/pep-0517/) build system ([see test case](https://
-github.com/s-weigand/qt-dev-helper/blob/main/tests/data/pyproject.toml)) - CLI
-auto completion - Project wide configuration in `pyproject.toml` - Recursive
-asset compiler for Qt projects (using `uic` and `rcc`): - `*.ui` -> `*.py` -
-`*.qrc` -> `*.py` - `*.ui` -> `*.h` - `*.qrc` -> `*.h` - `*.scss` -> `*.qss` -
-Support for multiple Qt tooling suppliers - `PySide6-Essentials` - `qt6-
-applications` - `qt5-applications` - Ability to open all files in a folder in
-QtDesigner ## Planned features - Stand alone executable for each release
-(Windows) - File watch mode - `qss` injection into `*.ui` files - [`pre-
-commit`](https://pre-commit.com/) hooks ## Installation ```console pip install
-qt-dev-helper ``` ## FAQ - Q: Why is `PyQt5` not supported? A: `PyQt5` only
-ships a python specific version of `uic` and `rcc` breaking the tool API and
+interrogate_badge.svg)](https://github.com/s-weigand/qt-dev-helper) [![Code
+style Python: black](https://img.shields.io/badge/code%20style-black-
+000000.svg)](https://github.com/psf/black) [![All Contributors](https://
+img.shields.io/github/all-contributors/s-weigand/qt-dev-helper)](#contributors)
+Toolbox to help develop Qt applications, improving the usability of the
+existing tooling. ## Installation ```console pip install qt-dev-helper ``` OR
+```console conda install -c conda-forge qt-dev-helper ``` ## Features - Usable
+as Library and/or CLI tool - Compatible with [PEP517](https://peps.python.org/
+pep-0517/) build system ([see test case](https://github.com/s-weigand/qt-dev-
+helper/blob/main/tests/data/pyproject.toml)) - CLI auto completion - Project
+wide configuration in `pyproject.toml` - Recursive asset compiler for Qt
+projects (using `uic` and `rcc`): - `*.ui` -> `*.py` - `*.qrc` -> `*.py` -
+`*.ui` -> `*.h` - `*.qrc` -> `*.h` - `*.scss` -> `*.qss` - Support for multiple
+Qt tooling suppliers - `PySide6-Essentials` - `qt6-applications` - `qt5-
+applications` - Ability to open all files in a folder in QtDesigner ## Planned
+features - Stand alone executable for each release (Windows) - File watch mode
+- `qss` injection into `*.ui` files - [`pre-commit`](https://pre-commit.com/
+) hooks ## FAQ - Q: Why is `PyQt5` not supported? A: `PyQt5` only ships a
+python specific version of `uic` and `rcc` breaking the tool API and
 compatibility with cpp projects. Use the matching version of `qt5-applications`
 as Qt tooling supplier. ## Contributors â¨ Thanks goes out to these wonderful
 people ([emoji key](https://allcontributors.org/docs/en/emoji-key)):
 
                         Sebastian_Weigand                             Joris
                                                                    Snellenburg
                ð» ð¤ ð§ ð ð â �           �
```

### Comparing `qt_dev_helper-0.0.3/docs/Makefile` & `qt_dev_helper-0.0.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `qt_dev_helper-0.0.3/docs/_templates/autosummary/class.rst` & `qt_dev_helper-0.0.4/docs/_templates/autosummary/class.rst`

 * *Files identical despite different names*

### Comparing `qt_dev_helper-0.0.3/docs/_templates/autosummary/module.rst` & `qt_dev_helper-0.0.4/docs/_templates/autosummary/module.rst`

 * *Files identical despite different names*

### Comparing `qt_dev_helper-0.0.3/docs/conf.py` & `qt_dev_helper-0.0.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `qt_dev_helper-0.0.3/docs/installation.rst` & `qt_dev_helper-0.0.4/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `qt_dev_helper-0.0.3/docs/make.bat` & `qt_dev_helper-0.0.4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `qt_dev_helper-0.0.3/pyproject.toml` & `qt_dev_helper-0.0.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `qt_dev_helper-0.0.3/qt_dev_helper/cli/commands/build.py` & `qt_dev_helper-0.0.4/qt_dev_helper/cli/commands/build.py`

 * *Files identical despite different names*

### Comparing `qt_dev_helper-0.0.3/qt_dev_helper/cli/commands/designer.py` & `qt_dev_helper-0.0.4/qt_dev_helper/cli/commands/designer.py`

 * *Files identical despite different names*

### Comparing `qt_dev_helper-0.0.3/qt_dev_helper/cli/main_app.py` & `qt_dev_helper-0.0.4/qt_dev_helper/cli/main_app.py`

 * *Files identical despite different names*

### Comparing `qt_dev_helper-0.0.3/qt_dev_helper/cli/utils.py` & `qt_dev_helper-0.0.4/qt_dev_helper/cli/utils.py`

 * *Files identical despite different names*

### Comparing `qt_dev_helper-0.0.3/qt_dev_helper/config.py` & `qt_dev_helper-0.0.4/qt_dev_helper/config.py`

 * *Files identical despite different names*

### Comparing `qt_dev_helper-0.0.3/qt_dev_helper/qt_tools.py` & `qt_dev_helper-0.0.4/qt_dev_helper/qt_tools.py`

 * *Files identical despite different names*

### Comparing `qt_dev_helper-0.0.3/qt_dev_helper/transpiler.py` & `qt_dev_helper-0.0.4/qt_dev_helper/transpiler.py`

 * *Files identical despite different names*

### Comparing `qt_dev_helper-0.0.3/qt_dev_helper/utils.py` & `qt_dev_helper-0.0.4/qt_dev_helper/utils.py`

 * *Files identical despite different names*

### Comparing `qt_dev_helper-0.0.3/qt_dev_helper.egg-info/PKG-INFO` & `qt_dev_helper-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: qt-dev-helper
-Version: 0.0.3
+Name: qt_dev_helper
+Version: 0.0.4
 Summary: Tool to help developing Qt applications
 Home-page: https://github.com/s-weigand/qt-dev-helper
 Author: Sebastian Weigand
 Author-email: s.weigand.phy@gmail.com
 License: Apache Software License 2.0
 Project-URL: Documentation, https://qt-dev-helper.readthedocs.io
 Project-URL: Changelog, https://qt-dev-helper.readthedocs.io/en/latest/history.html
@@ -16,40 +16,50 @@
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Provides-Extra: pyside6
 Provides-Extra: cli
+Provides-Extra: pyside6
 License-File: LICENSE
 
 # Qt Dev Helper
 
-<!-- [![PyPi Version](https://img.shields.io/pypi/v/qt_dev_helper.svg)](https://pypi.org/project/qt-dev-helper/)
-[![Supported Python Versions](https://img.shields.io/pypi/pyversions/qt_dev_helper.svg)](https://pypi.org/project/qt-dev-helper/) -->
-
-<!-- [![Conda Version](https://img.shields.io/conda/vn/conda-forge/qt-dev-helper.svg)](https://anaconda.org/conda-forge/qt-dev-helper) -->
-
+[![PyPi Version](https://img.shields.io/pypi/v/qt_dev_helper.svg)](https://pypi.org/project/qt-dev-helper/)
+[![Supported Python Versions](https://img.shields.io/pypi/pyversions/qt_dev_helper.svg)](https://pypi.org/project/qt-dev-helper/)
+[![Conda Version](https://img.shields.io/conda/vn/conda-forge/qt-dev-helper.svg)](https://anaconda.org/conda-forge/qt-dev-helper)
 [![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 
 [![Actions Status](https://github.com/s-weigand/qt-dev-helper/workflows/Tests/badge.svg)](https://github.com/s-weigand/qt-dev-helper/actions)
 [![Documentation Status](https://readthedocs.org/projects/qt-dev-helper/badge/?version=latest)](https://qt-dev-helper.readthedocs.io/en/latest/?badge=latest)
 [![codecov](https://codecov.io/gh/s-weigand/qt-dev-helper/branch/main/graph/badge.svg)](https://codecov.io/gh/s-weigand/qt-dev-helper)
 [![Documentation Coverage](https://raw.githubusercontent.com/s-weigand/qt-dev-helper/main/docs/_static/interrogate_badge.svg)](https://github.com/s-weigand/qt-dev-helper)
+[![Code style Python: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 [![All Contributors](https://img.shields.io/github/all-contributors/s-weigand/qt-dev-helper)](#contributors)
 
-[![Code style Python: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
-
 Toolbox to help develop Qt applications, improving the usability of the existing tooling.
 
+## Installation
+
+```console
+pip install qt-dev-helper
+```
+
+OR
+
+```console
+conda install -c conda-forge qt-dev-helper
+```
+
 ## Features
 
 - Usable as Library and/or CLI tool
 - Compatible with [PEP517](https://peps.python.org/pep-0517/) build system
   ([see test case](https://github.com/s-weigand/qt-dev-helper/blob/main/tests/data/pyproject.toml))
 - CLI auto completion
 - Project wide configuration in `pyproject.toml`
@@ -68,20 +78,14 @@
 ## Planned features
 
 - Stand alone executable for each release (Windows)
 - File watch mode
 - `qss` injection into `*.ui` files
 - [`pre-commit`](https://pre-commit.com/) hooks
 
-## Installation
-
-```console
-pip install qt-dev-helper
-```
-
 ## FAQ
 
 - Q: Why is `PyQt5` not supported?
 
   A: `PyQt5` only ships a python specific version of `uic` and `rcc` breaking the tool API and
   compatibility with cpp projects.
   Use the matching version of `qt5-applications` as Qt tooling supplier.
```

#### html2text {}

```diff
@@ -1,53 +1,59 @@
-Metadata-Version: 2.1 Name: qt-dev-helper Version: 0.0.3 Summary: Tool to help
+Metadata-Version: 2.1 Name: qt_dev_helper Version: 0.0.4 Summary: Tool to help
 developing Qt applications Home-page: https://github.com/s-weigand/qt-dev-
 helper Author: Sebastian Weigand Author-email: s.weigand.phy@gmail.com License:
 Apache Software License 2.0 Project-URL: Documentation, https://qt-dev-
 helper.readthedocs.io Project-URL: Changelog, https://qt-dev-
 helper.readthedocs.io/en/latest/history.html Project-URL: Source, https://
 github.com/s-weigand/qt-dev-helper Project-URL: Tracker, https://github.com/s-
 weigand/qt-dev-helper/issues Keywords: qt_dev_helper Classifier: Development
 Status :: 2 - Pre-Alpha Classifier: Intended Audience :: Developers Classifier:
 License :: OSI Approved :: Apache Software License Classifier: Natural Language
 :: English Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3 :: Only Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
-Programming Language :: Python :: 3.10 Requires-Python: >=3.8 Description-
-Content-Type: text/markdown Provides-Extra: pyside6 Provides-Extra: cli
-License-File: LICENSE # Qt Dev Helper   [![License](https://img.shields.io/
-badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-
-2.0) [![Actions Status](https://github.com/s-weigand/qt-dev-helper/workflows/
-Tests/badge.svg)](https://github.com/s-weigand/qt-dev-helper/actions) [!
-[Documentation Status](https://readthedocs.org/projects/qt-dev-helper/badge/
-?version=latest)](https://qt-dev-helper.readthedocs.io/en/latest/?badge=latest)
-[![codecov](https://codecov.io/gh/s-weigand/qt-dev-helper/branch/main/graph/
-badge.svg)](https://codecov.io/gh/s-weigand/qt-dev-helper) [![Documentation
-Coverage](https://raw.githubusercontent.com/s-weigand/qt-dev-helper/main/docs/
-_static/interrogate_badge.svg)](https://github.com/s-weigand/qt-dev-helper) [!
-[All Contributors](https://img.shields.io/github/all-contributors/s-weigand/qt-
-dev-helper)](#contributors) [![Code style Python: black](https://
-img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/
-black) Toolbox to help develop Qt applications, improving the usability of the
-existing tooling. ## Features - Usable as Library and/or CLI tool - Compatible
-with [PEP517](https://peps.python.org/pep-0517/) build system ([see test case]
-(https://github.com/s-weigand/qt-dev-helper/blob/main/tests/data/
-pyproject.toml)) - CLI auto completion - Project wide configuration in
-`pyproject.toml` - Recursive asset compiler for Qt projects (using `uic` and
-`rcc`): - `*.ui` -> `*.py` - `*.qrc` -> `*.py` - `*.ui` -> `*.h` - `*.qrc` -
-> `*.h` - `*.scss` -> `*.qss` - Support for multiple Qt tooling suppliers -
-`PySide6-Essentials` - `qt6-applications` - `qt5-applications` - Ability to
-open all files in a folder in QtDesigner ## Planned features - Stand alone
-executable for each release (Windows) - File watch mode - `qss` injection into
-`*.ui` files - [`pre-commit`](https://pre-commit.com/) hooks ## Installation
-```console pip install qt-dev-helper ``` ## FAQ - Q: Why is `PyQt5` not
-supported? A: `PyQt5` only ships a python specific version of `uic` and `rcc`
-breaking the tool API and compatibility with cpp projects. Use the matching
-version of `qt5-applications` as Qt tooling supplier. ## Contributors â¨
-Thanks goes out to these wonderful people ([emoji key](https://
-allcontributors.org/docs/en/emoji-key)):
+Programming Language :: Python :: 3.10 Classifier: Programming Language ::
+Python :: 3.11 Requires-Python: >=3.8 Description-Content-Type: text/markdown
+Provides-Extra: cli Provides-Extra: pyside6 License-File: LICENSE # Qt Dev
+Helper [![PyPi Version](https://img.shields.io/pypi/v/qt_dev_helper.svg)]
+(https://pypi.org/project/qt-dev-helper/) [![Supported Python Versions](https:/
+/img.shields.io/pypi/pyversions/qt_dev_helper.svg)](https://pypi.org/project/
+qt-dev-helper/) [![Conda Version](https://img.shields.io/conda/vn/conda-forge/
+qt-dev-helper.svg)](https://anaconda.org/conda-forge/qt-dev-helper) [![License]
+(https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://
+opensource.org/licenses/Apache-2.0) [![Actions Status](https://github.com/s-
+weigand/qt-dev-helper/workflows/Tests/badge.svg)](https://github.com/s-weigand/
+qt-dev-helper/actions) [![Documentation Status](https://readthedocs.org/
+projects/qt-dev-helper/badge/?version=latest)](https://qt-dev-
+helper.readthedocs.io/en/latest/?badge=latest) [![codecov](https://codecov.io/
+gh/s-weigand/qt-dev-helper/branch/main/graph/badge.svg)](https://codecov.io/gh/
+s-weigand/qt-dev-helper) [![Documentation Coverage](https://
+raw.githubusercontent.com/s-weigand/qt-dev-helper/main/docs/_static/
+interrogate_badge.svg)](https://github.com/s-weigand/qt-dev-helper) [![Code
+style Python: black](https://img.shields.io/badge/code%20style-black-
+000000.svg)](https://github.com/psf/black) [![All Contributors](https://
+img.shields.io/github/all-contributors/s-weigand/qt-dev-helper)](#contributors)
+Toolbox to help develop Qt applications, improving the usability of the
+existing tooling. ## Installation ```console pip install qt-dev-helper ``` OR
+```console conda install -c conda-forge qt-dev-helper ``` ## Features - Usable
+as Library and/or CLI tool - Compatible with [PEP517](https://peps.python.org/
+pep-0517/) build system ([see test case](https://github.com/s-weigand/qt-dev-
+helper/blob/main/tests/data/pyproject.toml)) - CLI auto completion - Project
+wide configuration in `pyproject.toml` - Recursive asset compiler for Qt
+projects (using `uic` and `rcc`): - `*.ui` -> `*.py` - `*.qrc` -> `*.py` -
+`*.ui` -> `*.h` - `*.qrc` -> `*.h` - `*.scss` -> `*.qss` - Support for multiple
+Qt tooling suppliers - `PySide6-Essentials` - `qt6-applications` - `qt5-
+applications` - Ability to open all files in a folder in QtDesigner ## Planned
+features - Stand alone executable for each release (Windows) - File watch mode
+- `qss` injection into `*.ui` files - [`pre-commit`](https://pre-commit.com/
+) hooks ## FAQ - Q: Why is `PyQt5` not supported? A: `PyQt5` only ships a
+python specific version of `uic` and `rcc` breaking the tool API and
+compatibility with cpp projects. Use the matching version of `qt5-applications`
+as Qt tooling supplier. ## Contributors â¨ Thanks goes out to these wonderful
+people ([emoji key](https://allcontributors.org/docs/en/emoji-key)):
 
                         Sebastian_Weigand                             Joris
                                                                    Snellenburg
                ð» ð¤ ð§ ð ð â �           �
                                                                       ð
    This project follows the [all-contributors](https://github.com/all-
 contributors/all-contributors) specification. Contributions of any kind are
```

### Comparing `qt_dev_helper-0.0.3/qt_dev_helper.egg-info/SOURCES.txt` & `qt_dev_helper-0.0.4/qt_dev_helper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `qt_dev_helper-0.0.3/setup.cfg` & `qt_dev_helper-0.0.4/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -4,39 +4,40 @@
 description = Tool to help developing Qt applications
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/s-weigand/qt-dev-helper
 author = Sebastian Weigand
 author_email = s.weigand.phy@gmail.com
 license = Apache Software License 2.0
-license_file = LICENSE
+license_files = LICENSE
 classifiers = 
 	Development Status :: 2 - Pre-Alpha
 	Intended Audience :: Developers
 	License :: OSI Approved :: Apache Software License
 	Natural Language :: English
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3 :: Only
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 keywords = qt_dev_helper
 project_urls = 
 	Documentation=https://qt-dev-helper.readthedocs.io
 	Changelog=https://qt-dev-helper.readthedocs.io/en/latest/history.html
 	Source=https://github.com/s-weigand/qt-dev-helper
 	Tracker=https://github.com/s-weigand/qt-dev-helper/issues
 
 [options]
 packages = find:
 install_requires = 
-	pydantic>=1.9.0
+	pydantic>=1.9.0,<2
+	qtsass>=0.3.1
 	rich>=12.0.0
 	tomli>=2.0.1
-	qtsass>=0.3.1
 python_requires = >=3.8
 include_package_data = True
 zip_safe = False
 
 [options.packages.find]
 exclude = 
 	tests*
@@ -45,18 +46,18 @@
 	qt_dev_helper.*
 
 [options.entry_points]
 console_scripts = 
 	qt-dev-helper=qt_dev_helper.cli.main_app:app
 
 [options.extras_require]
-pyside6 = 
-	PySide6-Essentials
 cli = 
 	typer>=0.4.0
+pyside6 = 
+	PySide6-Essentials
 
 [darglint]
 docstring_style = numpy
 ignore_regex = _validate*
 
 [pydocstyle]
 convention = numpy
```

### Comparing `qt_dev_helper-0.0.3/tests/cli/commands/test_build.py` & `qt_dev_helper-0.0.4/tests/cli/commands/test_build.py`

 * *Files identical despite different names*

### Comparing `qt_dev_helper-0.0.3/tests/cli/commands/test_designer.py` & `qt_dev_helper-0.0.4/tests/cli/commands/test_designer.py`

 * *Files identical despite different names*

### Comparing `qt_dev_helper-0.0.3/tests/cli/test_main_app.py` & `qt_dev_helper-0.0.4/tests/cli/test_main_app.py`

 * *Files identical despite different names*

### Comparing `qt_dev_helper-0.0.3/tests/cli/test_utils.py` & `qt_dev_helper-0.0.4/tests/cli/test_utils.py`

 * *Files identical despite different names*

### Comparing `qt_dev_helper-0.0.3/tests/conftest.py` & `qt_dev_helper-0.0.4/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `qt_dev_helper-0.0.3/tests/data/assets/ui_files/minimal.ui` & `qt_dev_helper-0.0.4/tests/data/assets/ui_files/minimal.ui`

 * *Files identical despite different names*

### Comparing `qt_dev_helper-0.0.3/tests/data/expected/Ui_minimal.h` & `qt_dev_helper-0.0.4/tests/data/expected/Ui_minimal.h`

 * *Files 15% similar despite different names*

```diff
@@ -26,31 +26,31 @@
     QLabel *label;
     QMenuBar *menubar;
     QStatusBar *statusbar;
 
     void setupUi(QMainWindow *MainWindow)
     {
         if (MainWindow->objectName().isEmpty())
-            MainWindow->setObjectName(QString::fromUtf8("MainWindow"));
+            MainWindow->setObjectName("MainWindow");
         MainWindow->resize(800, 600);
         centralwidget = new QWidget(MainWindow);
-        centralwidget->setObjectName(QString::fromUtf8("centralwidget"));
+        centralwidget->setObjectName("centralwidget");
         label = new QLabel(centralwidget);
-        label->setObjectName(QString::fromUtf8("label"));
+        label->setObjectName("label");
         label->setGeometry(QRect(310, 130, 221, 221));
         label->setPixmap(QPixmap(QString::fromUtf8(":/icons/icons/circle.svg")));
         label->setScaledContents(true);
         label->setAlignment(Qt::AlignCenter);
         MainWindow->setCentralWidget(centralwidget);
         menubar = new QMenuBar(MainWindow);
-        menubar->setObjectName(QString::fromUtf8("menubar"));
+        menubar->setObjectName("menubar");
         menubar->setGeometry(QRect(0, 0, 800, 22));
         MainWindow->setMenuBar(menubar);
         statusbar = new QStatusBar(MainWindow);
-        statusbar->setObjectName(QString::fromUtf8("statusbar"));
+        statusbar->setObjectName("statusbar");
         MainWindow->setStatusBar(statusbar);
 
         retranslateUi(MainWindow);
 
         QMetaObject::connectSlotsByName(MainWindow);
     } // setupUi
```

### Comparing `qt_dev_helper-0.0.3/tests/data/expected/Ui_minimal.py` & `qt_dev_helper-0.0.4/tests/data/expected/Ui_minimal_no_from_imports.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     QSize, QTime, QUrl, Qt)
 from PySide6.QtGui import (QBrush, QColor, QConicalGradient, QCursor,
     QFont, QFontDatabase, QGradient, QIcon,
     QImage, QKeySequence, QLinearGradient, QPainter,
     QPalette, QPixmap, QRadialGradient, QTransform)
 from PySide6.QtWidgets import (QApplication, QLabel, QMainWindow, QMenuBar,
     QSizePolicy, QStatusBar, QWidget)
-from  . import test_resource_rc
+import test_resource_rc
 
 class Ui_MainWindow(object):
     def setupUi(self, MainWindow):
         if not MainWindow.objectName():
             MainWindow.setObjectName(u"MainWindow")
         MainWindow.resize(800, 600)
         self.centralwidget = QWidget(MainWindow)
```

### Comparing `qt_dev_helper-0.0.3/tests/data/expected/Ui_minimal_no_from_imports.py` & `qt_dev_helper-0.0.4/tests/data/expected/Ui_minimal.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     QSize, QTime, QUrl, Qt)
 from PySide6.QtGui import (QBrush, QColor, QConicalGradient, QCursor,
     QFont, QFontDatabase, QGradient, QIcon,
     QImage, QKeySequence, QLinearGradient, QPainter,
     QPalette, QPixmap, QRadialGradient, QTransform)
 from PySide6.QtWidgets import (QApplication, QLabel, QMainWindow, QMenuBar,
     QSizePolicy, QStatusBar, QWidget)
-import test_resource_rc
+from . import test_resource_rc
 
 class Ui_MainWindow(object):
     def setupUi(self, MainWindow):
         if not MainWindow.objectName():
             MainWindow.setObjectName(u"MainWindow")
         MainWindow.resize(800, 600)
         self.centralwidget = QWidget(MainWindow)
```

### Comparing `qt_dev_helper-0.0.3/tests/data/expected/test_resource.h` & `qt_dev_helper-0.0.4/tests/data/expected/test_resource.h`

 * *Files identical despite different names*

### Comparing `qt_dev_helper-0.0.3/tests/data/expected/test_resource.py` & `qt_dev_helper-0.0.4/tests/data/expected/test_resource.py`

 * *Files identical despite different names*

### Comparing `qt_dev_helper-0.0.3/tests/data/pyproject.toml` & `qt_dev_helper-0.0.4/tests/data/pyproject.toml`

 * *Files identical despite different names*

### Comparing `qt_dev_helper-0.0.3/tests/test_config.py` & `qt_dev_helper-0.0.4/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `qt_dev_helper-0.0.3/tests/test_qt_tools.py` & `qt_dev_helper-0.0.4/tests/test_qt_tools.py`

 * *Files identical despite different names*

### Comparing `qt_dev_helper-0.0.3/tests/test_transpiler.py` & `qt_dev_helper-0.0.4/tests/test_transpiler.py`

 * *Files identical despite different names*

### Comparing `qt_dev_helper-0.0.3/tests/test_utils.py` & `qt_dev_helper-0.0.4/tests/test_utils.py`

 * *Files identical despite different names*

