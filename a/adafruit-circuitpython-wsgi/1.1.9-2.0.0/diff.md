# Comparing `tmp/adafruit-circuitpython-wsgi-1.1.9.tar.gz` & `tmp/adafruit-circuitpython-wsgi-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-wsgi-1.1.9.tar", last modified: Thu Mar 17 12:52:22 2022, max compression
+gzip compressed data, was "adafruit-circuitpython-wsgi-2.0.0.tar", last modified: Sat Jul  8 14:18:41 2023, max compression
```

## Comparing `adafruit-circuitpython-wsgi-1.1.9.tar` & `adafruit-circuitpython-wsgi-2.0.0.tar`

### file list

```diff
@@ -1,48 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-17 12:52:22.225511 adafruit-circuitpython-wsgi-1.1.9/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-17 12:52:22.217512 adafruit-circuitpython-wsgi-1.1.9/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-17 12:52:22.221511 adafruit-circuitpython-wsgi-1.1.9/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (121)      880 2022-03-17 12:52:09.000000 adafruit-circuitpython-wsgi-1.1.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-17 12:52:22.221511 adafruit-circuitpython-wsgi-1.1.9/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     2424 2022-03-17 12:52:09.000000 adafruit-circuitpython-wsgi-1.1.9/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (121)      479 2022-03-17 12:52:09.000000 adafruit-circuitpython-wsgi-1.1.9/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2714 2022-03-17 12:52:09.000000 adafruit-circuitpython-wsgi-1.1.9/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (121)      205 2022-03-17 12:52:09.000000 adafruit-circuitpython-wsgi-1.1.9/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1231 2022-03-17 12:52:09.000000 adafruit-circuitpython-wsgi-1.1.9/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    16243 2022-03-17 12:52:09.000000 adafruit-circuitpython-wsgi-1.1.9/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (121)      388 2022-03-17 12:52:09.000000 adafruit-circuitpython-wsgi-1.1.9/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     6147 2022-03-17 12:52:09.000000 adafruit-circuitpython-wsgi-1.1.9/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (121)     1104 2022-03-17 12:52:09.000000 adafruit-circuitpython-wsgi-1.1.9/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-17 12:52:22.221511 adafruit-circuitpython-wsgi-1.1.9/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (121)    16814 2022-03-17 12:52:09.000000 adafruit-circuitpython-wsgi-1.1.9/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-03-17 12:52:09.000000 adafruit-circuitpython-wsgi-1.1.9/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-03-17 12:52:09.000000 adafruit-circuitpython-wsgi-1.1.9/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (121)     3862 2022-03-17 12:52:22.225511 adafruit-circuitpython-wsgi-1.1.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3077 2022-03-17 12:52:09.000000 adafruit-circuitpython-wsgi-1.1.9/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-03-17 12:52:09.000000 adafruit-circuitpython-wsgi-1.1.9/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-17 12:52:22.221511 adafruit-circuitpython-wsgi-1.1.9/adafruit_circuitpython_wsgi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3862 2022-03-17 12:52:22.000000 adafruit-circuitpython-wsgi-1.1.9/adafruit_circuitpython_wsgi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      933 2022-03-17 12:52:22.000000 adafruit-circuitpython-wsgi-1.1.9/adafruit_circuitpython_wsgi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-17 12:52:22.000000 adafruit-circuitpython-wsgi-1.1.9/adafruit_circuitpython_wsgi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       16 2022-03-17 12:52:22.000000 adafruit-circuitpython-wsgi-1.1.9/adafruit_circuitpython_wsgi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       14 2022-03-17 12:52:22.000000 adafruit-circuitpython-wsgi-1.1.9/adafruit_circuitpython_wsgi.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-17 12:52:22.225511 adafruit-circuitpython-wsgi-1.1.9/adafruit_wsgi/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-17 12:52:09.000000 adafruit-circuitpython-wsgi-1.1.9/adafruit_wsgi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2814 2022-03-17 12:52:09.000000 adafruit-circuitpython-wsgi-1.1.9/adafruit_wsgi/request.py
--rw-r--r--   0 runner    (1001) docker     (121)     4218 2022-03-17 12:52:09.000000 adafruit-circuitpython-wsgi-1.1.9/adafruit_wsgi/wsgi_app.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-17 12:52:22.225511 adafruit-circuitpython-wsgi-1.1.9/docs/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-17 12:52:22.225511 adafruit-circuitpython-wsgi-1.1.9/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-03-17 12:52:09.000000 adafruit-circuitpython-wsgi-1.1.9/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (121)      105 2022-03-17 12:52:09.000000 adafruit-circuitpython-wsgi-1.1.9/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (121)      272 2022-03-17 12:52:09.000000 adafruit-circuitpython-wsgi-1.1.9/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-03-17 12:52:09.000000 adafruit-circuitpython-wsgi-1.1.9/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     5405 2022-03-17 12:52:09.000000 adafruit-circuitpython-wsgi-1.1.9/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      182 2022-03-17 12:52:09.000000 adafruit-circuitpython-wsgi-1.1.9/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-03-17 12:52:09.000000 adafruit-circuitpython-wsgi-1.1.9/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)      892 2022-03-17 12:52:09.000000 adafruit-circuitpython-wsgi-1.1.9/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-03-17 12:52:09.000000 adafruit-circuitpython-wsgi-1.1.9/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)      123 2022-03-17 12:52:09.000000 adafruit-circuitpython-wsgi-1.1.9/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-17 12:52:22.225511 adafruit-circuitpython-wsgi-1.1.9/examples/
--rw-r--r--   0 runner    (1001) docker     (121)     3274 2022-03-17 12:52:09.000000 adafruit-circuitpython-wsgi-1.1.9/examples/wsgi_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (121)      119 2022-03-17 12:52:09.000000 adafruit-circuitpython-wsgi-1.1.9/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-03-17 12:52:22.225511 adafruit-circuitpython-wsgi-1.1.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1942 2022-03-17 12:52:09.000000 adafruit-circuitpython-wsgi-1.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:18:41.632836 adafruit-circuitpython-wsgi-2.0.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:18:41.616836 adafruit-circuitpython-wsgi-2.0.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:18:41.624836 adafruit-circuitpython-wsgi-2.0.0/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-07-08 14:18:20.000000 adafruit-circuitpython-wsgi-2.0.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:18:41.624836 adafruit-circuitpython-wsgi-2.0.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-07-08 14:18:20.000000 adafruit-circuitpython-wsgi-2.0.0/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-07-08 14:18:20.000000 adafruit-circuitpython-wsgi-2.0.0/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-07-08 14:18:20.000000 adafruit-circuitpython-wsgi-2.0.0/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-07-08 14:18:20.000000 adafruit-circuitpython-wsgi-2.0.0/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-07-08 14:18:20.000000 adafruit-circuitpython-wsgi-2.0.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-07-08 14:18:20.000000 adafruit-circuitpython-wsgi-2.0.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13078 2023-07-08 14:18:20.000000 adafruit-circuitpython-wsgi-2.0.0/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-07-08 14:18:20.000000 adafruit-circuitpython-wsgi-2.0.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6147 2023-07-08 14:18:20.000000 adafruit-circuitpython-wsgi-2.0.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-07-08 14:18:20.000000 adafruit-circuitpython-wsgi-2.0.0/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:18:41.624836 adafruit-circuitpython-wsgi-2.0.0/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-07-08 14:18:20.000000 adafruit-circuitpython-wsgi-2.0.0/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-07-08 14:18:20.000000 adafruit-circuitpython-wsgi-2.0.0/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-07-08 14:18:20.000000 adafruit-circuitpython-wsgi-2.0.0/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4088 2023-07-08 14:18:41.632836 adafruit-circuitpython-wsgi-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3274 2023-07-08 14:18:20.000000 adafruit-circuitpython-wsgi-2.0.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-08 14:18:20.000000 adafruit-circuitpython-wsgi-2.0.0/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:18:41.628836 adafruit-circuitpython-wsgi-2.0.0/adafruit_circuitpython_wsgi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4088 2023-07-08 14:18:41.000000 adafruit-circuitpython-wsgi-2.0.0/adafruit_circuitpython_wsgi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-07-08 14:18:41.000000 adafruit-circuitpython-wsgi-2.0.0/adafruit_circuitpython_wsgi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 14:18:41.000000 adafruit-circuitpython-wsgi-2.0.0/adafruit_circuitpython_wsgi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-08 14:18:41.000000 adafruit-circuitpython-wsgi-2.0.0/adafruit_circuitpython_wsgi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-08 14:18:41.000000 adafruit-circuitpython-wsgi-2.0.0/adafruit_circuitpython_wsgi.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:18:41.628836 adafruit-circuitpython-wsgi-2.0.0/adafruit_wsgi/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 14:18:33.000000 adafruit-circuitpython-wsgi-2.0.0/adafruit_wsgi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9588 2023-07-08 14:18:33.000000 adafruit-circuitpython-wsgi-2.0.0/adafruit_wsgi/esp32spi_wsgiserver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2814 2023-07-08 14:18:33.000000 adafruit-circuitpython-wsgi-2.0.0/adafruit_wsgi/request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4176 2023-07-08 14:18:33.000000 adafruit-circuitpython-wsgi-2.0.0/adafruit_wsgi/wsgi_app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:18:41.628836 adafruit-circuitpython-wsgi-2.0.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:18:41.632836 adafruit-circuitpython-wsgi-2.0.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-07-08 14:18:20.000000 adafruit-circuitpython-wsgi-2.0.0/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-08 14:18:20.000000 adafruit-circuitpython-wsgi-2.0.0/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-07-08 14:18:20.000000 adafruit-circuitpython-wsgi-2.0.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-08 14:18:20.000000 adafruit-circuitpython-wsgi-2.0.0/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5653 2023-07-08 14:18:20.000000 adafruit-circuitpython-wsgi-2.0.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-07-08 14:18:20.000000 adafruit-circuitpython-wsgi-2.0.0/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-08 14:18:20.000000 adafruit-circuitpython-wsgi-2.0.0/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-07-08 14:18:20.000000 adafruit-circuitpython-wsgi-2.0.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-08 14:18:20.000000 adafruit-circuitpython-wsgi-2.0.0/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-08 14:18:20.000000 adafruit-circuitpython-wsgi-2.0.0/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:18:41.632836 adafruit-circuitpython-wsgi-2.0.0/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:18:41.632836 adafruit-circuitpython-wsgi-2.0.0/examples/static/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      356 2023-07-08 14:18:20.000000 adafruit-circuitpython-wsgi-2.0.0/examples/static/index.html
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3862 2023-07-08 14:18:20.000000 adafruit-circuitpython-wsgi-2.0.0/examples/static/led_color_picker_example.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3261 2023-07-08 14:18:33.000000 adafruit-circuitpython-wsgi-2.0.0/examples/wsgi_simpletest.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8387 2023-07-08 14:18:33.000000 adafruit-circuitpython-wsgi-2.0.0/examples/wsgi_static_files_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-08 14:18:20.000000 adafruit-circuitpython-wsgi-2.0.0/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-07-08 14:18:33.000000 adafruit-circuitpython-wsgi-2.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-07-08 14:18:20.000000 adafruit-circuitpython-wsgi-2.0.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 14:18:41.632836 adafruit-circuitpython-wsgi-2.0.0/setup.cfg
```

### Comparing `adafruit-circuitpython-wsgi-1.1.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-wsgi-2.0.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-wsgi-1.1.9/.pre-commit-config.yaml` & `adafruit-circuitpython-wsgi-2.0.0/.pre-commit-config.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 # SPDX-FileCopyrightText: 2020 Diego Elio Pettenò
 #
 # SPDX-License-Identifier: Unlicense
 
 repos:
--   repo: https://github.com/python/black
-    rev: 20.8b1
+  - repo: https://github.com/python/black
+    rev: 23.3.0
     hooks:
-    - id: black
--   repo: https://github.com/fsfe/reuse-tool
-    rev: v0.12.1
+      - id: black
+  - repo: https://github.com/fsfe/reuse-tool
+    rev: v1.1.2
     hooks:
-    - id: reuse
--   repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v2.3.0
+      - id: reuse
+  - repo: https://github.com/pre-commit/pre-commit-hooks
+    rev: v4.4.0
     hooks:
-    -   id: check-yaml
-    -   id: end-of-file-fixer
-    -   id: trailing-whitespace
--   repo: https://github.com/pycqa/pylint
-    rev: v2.11.1
+      - id: check-yaml
+      - id: end-of-file-fixer
+      - id: trailing-whitespace
+  - repo: https://github.com/pycqa/pylint
+    rev: v2.17.4
     hooks:
-    -   id: pylint
+      - id: pylint
         name: pylint (library code)
         types: [python]
         args:
           - --disable=consider-using-f-string
         exclude: "^(docs/|examples/|tests/|setup.py$)"
-    -   id: pylint
+      - id: pylint
         name: pylint (example code)
         description: Run pylint rules on "examples/*.py" files
         types: [python]
         files: "^examples/"
         args:
-        - --disable=missing-docstring,invalid-name,consider-using-f-string,duplicate-code
-    -   id: pylint
+          - --disable=missing-docstring,invalid-name,consider-using-f-string,duplicate-code
+      - id: pylint
         name: pylint (test code)
         description: Run pylint rules on "tests/*.py" files
         types: [python]
         files: "^tests/"
         args:
-        - --disable=missing-docstring,consider-using-f-string,duplicate-code
+          - --disable=missing-docstring,consider-using-f-string,duplicate-code
```

### Comparing `adafruit-circuitpython-wsgi-1.1.9/.pylintrc` & `adafruit-circuitpython-wsgi-2.0.0/.pylintrc`

 * *Files 24% similar despite different names*

```diff
@@ -1,36 +1,36 @@
-# SPDX-FileCopyrightText: 2021 ladyada for Adafruit Industries
+# SPDX-FileCopyrightText: 2017 Scott Shawcroft, written for Adafruit Industries
 #
 # SPDX-License-Identifier: Unlicense
 
 [MASTER]
 
 # A comma-separated list of package or module names from where C extensions may
 # be loaded. Extensions are loading into the active Python interpreter and may
 # run arbitrary code
 extension-pkg-whitelist=
 
-# Add files or directories to the blacklist. They should be base names, not
+# Add files or directories to the ignore-list. They should be base names, not
 # paths.
 ignore=CVS
 
-# Add files or directories matching the regex patterns to the blacklist. The
+# Add files or directories matching the regex patterns to the ignore-list. The
 # regex matches against base names, not paths.
 ignore-patterns=
 
 # Python code to execute, usually for sys.path manipulation such as
 # pygtk.require().
 #init-hook=
 
 # Use multiple processes to speed up Pylint.
 jobs=1
 
 # List of plugins (as comma separated values of python modules names) to load,
 # usually to register additional checkers.
-load-plugins=
+load-plugins=pylint.extensions.no_self_use
 
 # Pickle collected data for later comparisons.
 persistent=yes
 
 # Specify a configuration file.
 #rcfile=
 
@@ -50,16 +50,16 @@
 # option multiple times (only on the command line, not in the configuration
 # file where it should appear only once).You can also use "--disable=all" to
 # disable everything first and then reenable specific checks. For example, if
 # you want to run only the similarities checker, you can use "--disable=all
 # --enable=similarities". If you want to run only the classes checker, but have
 # no Warning level messages displayed, use"--disable=all --enable=classes
 # --disable=W"
-# disable=import-error,print-statement,parameter-unpacking,unpacking-in-except,old-raise-syntax,backtick,long-suffix,old-ne-operator,old-octal-literal,import-star-module-level,raw-checker-failed,bad-inline-option,locally-disabled,locally-enabled,file-ignored,suppressed-message,useless-suppression,deprecated-pragma,apply-builtin,basestring-builtin,buffer-builtin,cmp-builtin,coerce-builtin,execfile-builtin,file-builtin,long-builtin,raw_input-builtin,reduce-builtin,standarderror-builtin,unicode-builtin,xrange-builtin,coerce-method,delslice-method,getslice-method,setslice-method,no-absolute-import,old-division,dict-iter-method,dict-view-method,next-method-called,metaclass-assignment,indexing-exception,raising-string,reload-builtin,oct-method,hex-method,nonzero-method,cmp-method,input-builtin,round-builtin,intern-builtin,unichr-builtin,map-builtin-not-iterating,zip-builtin-not-iterating,range-builtin-not-iterating,filter-builtin-not-iterating,using-cmp-argument,eq-without-hash,div-method,idiv-method,rdiv-method,exception-message-attribute,invalid-str-codec,sys-max-int,bad-python3-import,deprecated-string-function,deprecated-str-translate-call
-disable=print-statement,parameter-unpacking,unpacking-in-except,old-raise-syntax,backtick,long-suffix,old-ne-operator,old-octal-literal,import-star-module-level,raw-checker-failed,bad-inline-option,locally-disabled,locally-enabled,file-ignored,suppressed-message,useless-suppression,deprecated-pragma,apply-builtin,basestring-builtin,buffer-builtin,cmp-builtin,coerce-builtin,execfile-builtin,file-builtin,long-builtin,raw_input-builtin,reduce-builtin,standarderror-builtin,unicode-builtin,xrange-builtin,coerce-method,delslice-method,getslice-method,setslice-method,no-absolute-import,old-division,dict-iter-method,dict-view-method,next-method-called,metaclass-assignment,indexing-exception,raising-string,reload-builtin,oct-method,hex-method,nonzero-method,cmp-method,input-builtin,round-builtin,intern-builtin,unichr-builtin,map-builtin-not-iterating,zip-builtin-not-iterating,range-builtin-not-iterating,filter-builtin-not-iterating,using-cmp-argument,eq-without-hash,div-method,idiv-method,rdiv-method,exception-message-attribute,invalid-str-codec,sys-max-int,bad-python3-import,deprecated-string-function,deprecated-str-translate-call,import-error,bad-continuation,unspecified-encoding
+# disable=import-error,raw-checker-failed,bad-inline-option,locally-disabled,file-ignored,suppressed-message,useless-suppression,deprecated-pragma,deprecated-str-translate-call
+disable=raw-checker-failed,bad-inline-option,locally-disabled,file-ignored,suppressed-message,useless-suppression,deprecated-pragma,import-error,pointless-string-statement,unspecified-encoding
 
 # Enable the message, report, category or checker with the given id(s). You can
 # either give multiple identifier separated by comma (,) or put this option
 # multiple time (only on the command line, not in the configuration file where
 # it should appear only once). See also the "--disable" option for examples.
 enable=
 
@@ -221,20 +221,14 @@
 
 # Maximum number of characters on a single line.
 max-line-length=100
 
 # Maximum number of lines in a module
 max-module-lines=1000
 
-# List of optional constructs for which whitespace checking is disabled. `dict-
-# separator` is used to allow tabulation in dicts, etc.: {1  : 1,\n222: 2}.
-# `trailing-comma` allows a space between comma and closing bracket: (a, ).
-# `empty-line` allows space-only lines.
-no-space-check=trailing-comma,dict-separator
-
 # Allow the body of a class to be on the same line as the declaration if body
 # contains single statement.
 single-line-class-stmt=no
 
 # Allow the body of an if to be on the same line as the test if there is no
 # else.
 single-line-if-stmt=no
@@ -248,86 +242,58 @@
 # Ignore docstrings when computing similarities.
 ignore-docstrings=yes
 
 # Ignore imports when computing similarities.
 ignore-imports=yes
 
 # Minimum lines number of a similarity.
-min-similarity-lines=4
+min-similarity-lines=12
 
 
 [BASIC]
 
-# Naming hint for argument names
-argument-name-hint=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
-
 # Regular expression matching correct argument names
 argument-rgx=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
 
-# Naming hint for attribute names
-attr-name-hint=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
-
 # Regular expression matching correct attribute names
 attr-rgx=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
 
 # Bad variable names which should always be refused, separated by a comma
 bad-names=foo,bar,baz,toto,tutu,tata
 
-# Naming hint for class attribute names
-class-attribute-name-hint=([A-Za-z_][A-Za-z0-9_]{2,30}|(__.*__))$
-
 # Regular expression matching correct class attribute names
 class-attribute-rgx=([A-Za-z_][A-Za-z0-9_]{2,30}|(__.*__))$
 
-# Naming hint for class names
-# class-name-hint=[A-Z_][a-zA-Z0-9]+$
-class-name-hint=[A-Z_][a-zA-Z0-9_]+$
-
 # Regular expression matching correct class names
 # class-rgx=[A-Z_][a-zA-Z0-9]+$
 class-rgx=[A-Z_][a-zA-Z0-9_]+$
 
-# Naming hint for constant names
-const-name-hint=(([A-Z_][A-Z0-9_]*)|(__.*__))$
-
 # Regular expression matching correct constant names
 const-rgx=(([A-Z_][A-Z0-9_]*)|(__.*__))$
 
 # Minimum line length for functions/classes that require docstrings, shorter
 # ones are exempt.
 docstring-min-length=-1
 
-# Naming hint for function names
-function-name-hint=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
-
 # Regular expression matching correct function names
 function-rgx=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
 
 # Good variable names which should always be accepted, separated by a comma
 # good-names=i,j,k,ex,Run,_
 good-names=r,g,b,w,i,j,k,n,x,y,z,ex,ok,Run,_
 
 # Include a hint for the correct naming format with invalid-name
 include-naming-hint=no
 
-# Naming hint for inline iteration names
-inlinevar-name-hint=[A-Za-z_][A-Za-z0-9_]*$
-
 # Regular expression matching correct inline iteration names
 inlinevar-rgx=[A-Za-z_][A-Za-z0-9_]*$
 
-# Naming hint for method names
-method-name-hint=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
-
 # Regular expression matching correct method names
 method-rgx=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
 
-# Naming hint for module names
-module-name-hint=(([a-z_][a-z0-9_]*)|([A-Z][a-zA-Z0-9]+))$
-
 # Regular expression matching correct module names
 module-rgx=(([a-z_][a-z0-9_]*)|([A-Z][a-zA-Z0-9]+))$
 
 # Colon-delimited sets of names that determine each other's naming style when
 # the name regexes allow several styles.
 name-group=
 
@@ -335,17 +301,14 @@
 # not require a docstring.
 no-docstring-rgx=^_
 
 # List of decorators that produce properties, such as abc.abstractproperty. Add
 # to this list to register other decorators that produce valid properties.
 property-classes=abc.abstractproperty
 
-# Naming hint for variable names
-variable-name-hint=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
-
 # Regular expression matching correct variable names
 variable-rgx=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
 
 
 [IMPORTS]
 
 # Allow wildcard imports from modules that define __all__.
@@ -429,8 +392,8 @@
 min-public-methods=1
 
 
 [EXCEPTIONS]
 
 # Exceptions that will emit a warning when being caught. Defaults to
 # "Exception"
-overgeneral-exceptions=Exception
+overgeneral-exceptions=builtins.Exception
```

### Comparing `adafruit-circuitpython-wsgi-1.1.9/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-wsgi-2.0.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-wsgi-1.1.9/LICENSE` & `adafruit-circuitpython-wsgi-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-wsgi-1.1.9/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-wsgi-2.0.0/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-wsgi-1.1.9/LICENSES/MIT.txt` & `adafruit-circuitpython-wsgi-2.0.0/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-wsgi-1.1.9/LICENSES/Unlicense.txt` & `adafruit-circuitpython-wsgi-2.0.0/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-wsgi-1.1.9/PKG-INFO` & `adafruit-circuitpython-wsgi-2.0.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,41 +1,44 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-wsgi
-Version: 1.1.9
+Version: 2.0.0
 Summary: CircuitPython framework for creating WSGI compatible web server applications.
-Home-page: https://github.com/adafruit/Adafruit_CircuitPython_WSGI
-Author: Adafruit Industries
-Author-email: circuitpython@adafruit.com
+Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
-Keywords: adafruit blinka circuitpython micropython wsgi web server webserver app webapp framework http https flask
-Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
+Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_WSGI
+Keywords: adafruit,blinka,circuitpython,micropython,wsgi,web,server,webserver,app,webapp,framework,http,https,flask
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
+Classifier: Topic :: Software Development :: Embedded Systems
 Classifier: Topic :: System :: Hardware
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/x-rst
+Provides-Extra: optional
 License-File: LICENSE
 
 Introduction
 ============
 
 .. image:: https://readthedocs.org/projects/adafruit-circuitpython-wsgi/badge/?version=latest
     :target: https://docs.circuitpython.org/projects/wsgi/en/latest/
     :alt: Documentation Status
 
-.. image:: https://img.shields.io/discord/327254708534116352.svg
+.. image:: https://raw.githubusercontent.com/adafruit/Adafruit_CircuitPython_Bundle/main/badges/adafruit_discord.svg
     :target: https://adafru.it/discord
     :alt: Discord
 
 .. image:: https://github.com/adafruit/Adafruit_CircuitPython_WSGI/workflows/Build%20CI/badge.svg
     :target: https://github.com/adafruit/Adafruit_CircuitPython_WSGI/actions
     :alt: Build Status
 
+.. image:: https://img.shields.io/badge/code%20style-black-000000.svg
+    :target: https://github.com/psf/black
+    :alt: Code Style: Black
+
 CircuitPython framework for creating WSGI compatible web server applications.
 
 
 Dependencies
 =============
 This driver depends on:
 
@@ -64,16 +67,16 @@
     sudo pip3 install adafruit-circuitpython-wsgi
 
 To install in a virtual environment in your current project:
 
 .. code-block:: shell
 
     mkdir project-name && cd project-name
-    python3 -m venv .env
-    source .env/bin/activate
+    python3 -m venv .venv
+    source .venv/bin/activate
     pip3 install adafruit-circuitpython-wsgi
 
 
 Documentation
 =============
 
 API documentation for this library can be found on `Read the Docs <https://docs.circuitpython.org/projects/wsgi/en/latest/>`_.
@@ -91,23 +94,21 @@
 -----------------------
 
 Sphinx is used to build the documentation based on rST files and comments in the code. First,
 install dependencies (feel free to reuse the virtual environment from above):
 
 .. code-block:: shell
 
-    python3 -m venv .env
-    source .env/bin/activate
+    python3 -m venv .venv
+    source .venv/bin/activate
     pip install Sphinx sphinx-rtd-theme
 
 Now, once you have the virtual environment activated:
 
 .. code-block:: shell
 
     cd docs
     sphinx-build -E -W -b html . _build/html
 
 This will output the documentation to ``docs/_build/html``. Open the index.html in your browser to
 view them. It will also (due to -W) error out on any warning like Travis will. This is a good way to
 locally verify it will pass.
-
-
```

### Comparing `adafruit-circuitpython-wsgi-1.1.9/README.rst` & `adafruit-circuitpython-wsgi-2.0.0/README.rst`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 Introduction
 ============
 
 .. image:: https://readthedocs.org/projects/adafruit-circuitpython-wsgi/badge/?version=latest
     :target: https://docs.circuitpython.org/projects/wsgi/en/latest/
     :alt: Documentation Status
 
-.. image:: https://img.shields.io/discord/327254708534116352.svg
+.. image:: https://raw.githubusercontent.com/adafruit/Adafruit_CircuitPython_Bundle/main/badges/adafruit_discord.svg
     :target: https://adafru.it/discord
     :alt: Discord
 
 .. image:: https://github.com/adafruit/Adafruit_CircuitPython_WSGI/workflows/Build%20CI/badge.svg
     :target: https://github.com/adafruit/Adafruit_CircuitPython_WSGI/actions
     :alt: Build Status
 
+.. image:: https://img.shields.io/badge/code%20style-black-000000.svg
+    :target: https://github.com/psf/black
+    :alt: Code Style: Black
+
 CircuitPython framework for creating WSGI compatible web server applications.
 
 
 Dependencies
 =============
 This driver depends on:
 
@@ -45,16 +49,16 @@
     sudo pip3 install adafruit-circuitpython-wsgi
 
 To install in a virtual environment in your current project:
 
 .. code-block:: shell
 
     mkdir project-name && cd project-name
-    python3 -m venv .env
-    source .env/bin/activate
+    python3 -m venv .venv
+    source .venv/bin/activate
     pip3 install adafruit-circuitpython-wsgi
 
 
 Documentation
 =============
 
 API documentation for this library can be found on `Read the Docs <https://docs.circuitpython.org/projects/wsgi/en/latest/>`_.
@@ -72,16 +76,16 @@
 -----------------------
 
 Sphinx is used to build the documentation based on rST files and comments in the code. First,
 install dependencies (feel free to reuse the virtual environment from above):
 
 .. code-block:: shell
 
-    python3 -m venv .env
-    source .env/bin/activate
+    python3 -m venv .venv
+    source .venv/bin/activate
     pip install Sphinx sphinx-rtd-theme
 
 Now, once you have the virtual environment activated:
 
 .. code-block:: shell
 
     cd docs
```

### Comparing `adafruit-circuitpython-wsgi-1.1.9/adafruit_circuitpython_wsgi.egg-info/PKG-INFO` & `adafruit-circuitpython-wsgi-2.0.0/adafruit_circuitpython_wsgi.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,41 +1,44 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-wsgi
-Version: 1.1.9
+Version: 2.0.0
 Summary: CircuitPython framework for creating WSGI compatible web server applications.
-Home-page: https://github.com/adafruit/Adafruit_CircuitPython_WSGI
-Author: Adafruit Industries
-Author-email: circuitpython@adafruit.com
+Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
-Keywords: adafruit blinka circuitpython micropython wsgi web server webserver app webapp framework http https flask
-Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
+Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_WSGI
+Keywords: adafruit,blinka,circuitpython,micropython,wsgi,web,server,webserver,app,webapp,framework,http,https,flask
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
+Classifier: Topic :: Software Development :: Embedded Systems
 Classifier: Topic :: System :: Hardware
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/x-rst
+Provides-Extra: optional
 License-File: LICENSE
 
 Introduction
 ============
 
 .. image:: https://readthedocs.org/projects/adafruit-circuitpython-wsgi/badge/?version=latest
     :target: https://docs.circuitpython.org/projects/wsgi/en/latest/
     :alt: Documentation Status
 
-.. image:: https://img.shields.io/discord/327254708534116352.svg
+.. image:: https://raw.githubusercontent.com/adafruit/Adafruit_CircuitPython_Bundle/main/badges/adafruit_discord.svg
     :target: https://adafru.it/discord
     :alt: Discord
 
 .. image:: https://github.com/adafruit/Adafruit_CircuitPython_WSGI/workflows/Build%20CI/badge.svg
     :target: https://github.com/adafruit/Adafruit_CircuitPython_WSGI/actions
     :alt: Build Status
 
+.. image:: https://img.shields.io/badge/code%20style-black-000000.svg
+    :target: https://github.com/psf/black
+    :alt: Code Style: Black
+
 CircuitPython framework for creating WSGI compatible web server applications.
 
 
 Dependencies
 =============
 This driver depends on:
 
@@ -64,16 +67,16 @@
     sudo pip3 install adafruit-circuitpython-wsgi
 
 To install in a virtual environment in your current project:
 
 .. code-block:: shell
 
     mkdir project-name && cd project-name
-    python3 -m venv .env
-    source .env/bin/activate
+    python3 -m venv .venv
+    source .venv/bin/activate
     pip3 install adafruit-circuitpython-wsgi
 
 
 Documentation
 =============
 
 API documentation for this library can be found on `Read the Docs <https://docs.circuitpython.org/projects/wsgi/en/latest/>`_.
@@ -91,23 +94,21 @@
 -----------------------
 
 Sphinx is used to build the documentation based on rST files and comments in the code. First,
 install dependencies (feel free to reuse the virtual environment from above):
 
 .. code-block:: shell
 
-    python3 -m venv .env
-    source .env/bin/activate
+    python3 -m venv .venv
+    source .venv/bin/activate
     pip install Sphinx sphinx-rtd-theme
 
 Now, once you have the virtual environment activated:
 
 .. code-block:: shell
 
     cd docs
     sphinx-build -E -W -b html . _build/html
 
 This will output the documentation to ``docs/_build/html``. Open the index.html in your browser to
 view them. It will also (due to -W) error out on any warning like Travis will. This is a good way to
 locally verify it will pass.
-
-
```

### Comparing `adafruit-circuitpython-wsgi-1.1.9/adafruit_circuitpython_wsgi.egg-info/SOURCES.txt` & `adafruit-circuitpython-wsgi-2.0.0/adafruit_circuitpython_wsgi.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -2,35 +2,41 @@
 .pre-commit-config.yaml
 .pylintrc
 .readthedocs.yaml
 CODE_OF_CONDUCT.md
 LICENSE
 README.rst
 README.rst.license
+optional_requirements.txt
+pyproject.toml
 requirements.txt
-setup.py
 .github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
 .github/workflows/build.yml
 .github/workflows/failure-help-text.yml
-.github/workflows/release.yml
+.github/workflows/release_gh.yml
+.github/workflows/release_pypi.yml
 LICENSES/CC-BY-4.0.txt
 LICENSES/MIT.txt
 LICENSES/Unlicense.txt
 adafruit_circuitpython_wsgi.egg-info/PKG-INFO
 adafruit_circuitpython_wsgi.egg-info/SOURCES.txt
 adafruit_circuitpython_wsgi.egg-info/dependency_links.txt
 adafruit_circuitpython_wsgi.egg-info/requires.txt
 adafruit_circuitpython_wsgi.egg-info/top_level.txt
 adafruit_wsgi/__init__.py
+adafruit_wsgi/esp32spi_wsgiserver.py
 adafruit_wsgi/request.py
 adafruit_wsgi/wsgi_app.py
 docs/api.rst
 docs/api.rst.license
 docs/conf.py
 docs/examples.rst
 docs/examples.rst.license
 docs/index.rst
 docs/index.rst.license
 docs/requirements.txt
 docs/_static/favicon.ico
 docs/_static/favicon.ico.license
-examples/wsgi_simpletest.py
+examples/wsgi_simpletest.py
+examples/wsgi_static_files_server.py
+examples/static/index.html
+examples/static/led_color_picker_example.js
```

### Comparing `adafruit-circuitpython-wsgi-1.1.9/adafruit_wsgi/request.py` & `adafruit-circuitpython-wsgi-2.0.0/adafruit_wsgi/request.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-wsgi-1.1.9/adafruit_wsgi/wsgi_app.py` & `adafruit-circuitpython-wsgi-2.0.0/adafruit_wsgi/wsgi_app.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 try:
     from typing import Any, AnyStr, Callable, Dict, List, Optional, Sequence, Tuple
 except ImportError:
     pass
 
 from adafruit_wsgi.request import Request
 
-__version__ = "0.0.0-auto.0"
+__version__ = "2.0.0"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_WSGI.git"
 
 
 class WSGIApp:
     """
     The base WSGI Application class.
     """
@@ -66,17 +66,16 @@
 
         if match:
             args, route = match
             try:
                 status, headers, resp_data = route["func"](request, *args)
             except (ValueError, TypeError) as err:
                 raise RuntimeError(
-                    "Proper HTTP response return not given for request handler '{}'".format(
-                        route["func"].__name__
-                    )
+                    "Proper HTTP response not returned by request handler for path "
+                    + f"'{request.path}'"
                 ) from err
         start_response(status, headers)
         return resp_data
 
     def on_request(self, methods: List[str], rule: str, request_handler: Callable):
         """
         Register a Request Handler for a particular HTTP method and path.
```

### Comparing `adafruit-circuitpython-wsgi-1.1.9/docs/_static/favicon.ico` & `adafruit-circuitpython-wsgi-2.0.0/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-wsgi-1.1.9/docs/conf.py` & `adafruit-circuitpython-wsgi-2.0.0/docs/conf.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,24 +2,26 @@
 
 # SPDX-FileCopyrightText: 2021 ladyada for Adafruit Industries
 #
 # SPDX-License-Identifier: MIT
 
 import os
 import sys
+import datetime
 
 sys.path.insert(0, os.path.abspath(".."))
 
 # -- General configuration ------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
 extensions = [
     "sphinx.ext.autodoc",
+    "sphinxcontrib.jquery",
     "sphinx.ext.intersphinx",
     "sphinx.ext.napoleon",
     "sphinx.ext.todo",
 ]
 
 # TODO: Please Read!
 # Uncomment the below if you use native CircuitPython modules such as
@@ -39,15 +41,22 @@
 source_suffix = ".rst"
 
 # The master toctree document.
 master_doc = "index"
 
 # General information about the project.
 project = "Adafruit WSGI Library"
-copyright = "2019 Matthew Costi"
+creation_year = "2019"
+current_year = str(datetime.datetime.now().year)
+year_duration = (
+    current_year
+    if current_year == creation_year
+    else creation_year + " - " + current_year
+)
+copyright = year_duration + " Matthew Costi"
 author = "Matthew Costi"
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 # The short X.Y version.
@@ -56,15 +65,15 @@
 release = "1.0"
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #
 # This is also used if you do content translation via gettext catalogs.
 # Usually you set "language" from the command line for these cases.
-language = None
+language = "en"
 
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
 # This patterns also effect to html_static_path and html_extra_path
 exclude_patterns = ["_build", "Thumbs.db", ".DS_Store", ".env", "CODE_OF_CONDUCT.md"]
 
 # The reST default role (used for this markup: `text`) to use for all
```

### Comparing `adafruit-circuitpython-wsgi-1.1.9/docs/index.rst` & `adafruit-circuitpython-wsgi-2.0.0/docs/index.rst`

 * *Files 12% similar despite different names*

```diff
@@ -26,15 +26,16 @@
 .. toctree::
     :caption: Related Products
 
 
 .. toctree::
     :caption: Other Links
 
-    Download <https://github.com/adafruit/Adafruit_CircuitPython_WSGI/releases/latest>
+    Download from GitHub <https://github.com/adafruit/Adafruit_CircuitPython_WSGI/releases/latest>
+    Download Library Bundle <https://circuitpython.org/libraries>
     CircuitPython Reference Documentation <https://docs.circuitpython.org>
     CircuitPython Support Forum <https://forums.adafruit.com/viewforum.php?f=60>
     Discord Chat <https://adafru.it/discord>
     Adafruit Learning System <https://learn.adafruit.com>
     Adafruit Blog <https://blog.adafruit.com>
     Adafruit Store <https://www.adafruit.com>
```

### Comparing `adafruit-circuitpython-wsgi-1.1.9/examples/wsgi_simpletest.py` & `adafruit-circuitpython-wsgi-2.0.0/examples/wsgi_simpletest.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import board
 import busio
 from digitalio import DigitalInOut
 import neopixel
 
 from adafruit_esp32spi import adafruit_esp32spi
 import adafruit_esp32spi.adafruit_esp32spi_wifimanager as wifimanager
-import adafruit_esp32spi.adafruit_esp32spi_wsgiserver as server
+import adafruit_wsgi.esp32spi_wsgiserver as server
 from adafruit_wsgi.wsgi_app import WSGIApp
 
 # Get wifi details and more from a secrets.py file
 try:
     from secrets import secrets
 except ImportError:
     print("WiFi secrets are kept in secrets.py, please add them there!")
```

