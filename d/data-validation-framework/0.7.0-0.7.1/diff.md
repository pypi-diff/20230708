# Comparing `tmp/data-validation-framework-0.7.0.tar.gz` & `tmp/data-validation-framework-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "data-validation-framework-0.7.0.tar", last modified: Fri Mar 10 20:58:19 2023, max compression
+gzip compressed data, was "data-validation-framework-0.7.1.tar", last modified: Fri Jul  7 23:12:56 2023, max compression
```

## Comparing `data-validation-framework-0.7.0.tar` & `data-validation-framework-0.7.1.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 20:58:19.810461 data-validation-framework-0.7.0/
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-03-10 20:58:10.000000 data-validation-framework-0.7.0/.auto-changelog
--rw-r--r--   0 runner    (1001) docker     (123)    10972 2023-03-10 20:58:10.000000 data-validation-framework-0.7.0/.auto-changelog-template.hbs
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-10 20:58:10.000000 data-validation-framework-0.7.0/.codespellignorelines
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-03-10 20:58:10.000000 data-validation-framework-0.7.0/.codespellrc
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-03-10 20:58:10.000000 data-validation-framework-0.7.0/.copier-answers.yml
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-03-10 20:58:10.000000 data-validation-framework-0.7.0/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-03-10 20:58:10.000000 data-validation-framework-0.7.0/.flake8
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-03-10 20:58:10.000000 data-validation-framework-0.7.0/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 20:58:19.806461 data-validation-framework-0.7.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-03-10 20:58:10.000000 data-validation-framework-0.7.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 20:58:19.806461 data-validation-framework-0.7.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2672 2023-03-10 20:58:10.000000 data-validation-framework-0.7.0/.github/workflows/codeql.yml
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-03-10 20:58:10.000000 data-validation-framework-0.7.0/.github/workflows/commitlint.yml
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-03-10 20:58:10.000000 data-validation-framework-0.7.0/.github/workflows/publish-sdist.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2382 2023-03-10 20:58:10.000000 data-validation-framework-0.7.0/.github/workflows/run-tox.yml
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-03-10 20:58:10.000000 data-validation-framework-0.7.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-03-10 20:58:10.000000 data-validation-framework-0.7.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-03-10 20:58:10.000000 data-validation-framework-0.7.0/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-03-10 20:58:10.000000 data-validation-framework-0.7.0/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-03-10 20:58:10.000000 data-validation-framework-0.7.0/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (123)     9996 2023-03-10 20:58:10.000000 data-validation-framework-0.7.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     4988 2023-03-10 20:58:10.000000 data-validation-framework-0.7.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    11354 2023-03-10 20:58:10.000000 data-validation-framework-0.7.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-03-10 20:58:10.000000 data-validation-framework-0.7.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8593 2023-03-10 20:58:19.810461 data-validation-framework-0.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7376 2023-03-10 20:58:10.000000 data-validation-framework-0.7.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-03-10 20:58:10.000000 data-validation-framework-0.7.0/codecov.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3759 2023-03-10 20:58:10.000000 data-validation-framework-0.7.0/commitlint.config.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 20:58:19.806461 data-validation-framework-0.7.0/data_validation_framework/
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-03-10 20:58:10.000000 data-validation-framework-0.7.0/data_validation_framework/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7330 2023-03-10 20:58:10.000000 data-validation-framework-0.7.0/data_validation_framework/report.py
--rw-r--r--   0 runner    (1001) docker     (123)     4698 2023-03-10 20:58:10.000000 data-validation-framework-0.7.0/data_validation_framework/result.py
--rw-r--r--   0 runner    (1001) docker     (123)     7440 2023-03-10 20:58:10.000000 data-validation-framework-0.7.0/data_validation_framework/rst_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-03-10 20:58:10.000000 data-validation-framework-0.7.0/data_validation_framework/target.py
--rw-r--r--   0 runner    (1001) docker     (123)    30156 2023-03-10 20:58:10.000000 data-validation-framework-0.7.0/data_validation_framework/task.py
--rw-r--r--   0 runner    (1001) docker     (123)     7504 2023-03-10 20:58:10.000000 data-validation-framework-0.7.0/data_validation_framework/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 20:58:19.806461 data-validation-framework-0.7.0/data_validation_framework.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8593 2023-03-10 20:58:19.000000 data-validation-framework-0.7.0/data_validation_framework.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-03-10 20:58:19.000000 data-validation-framework-0.7.0/data_validation_framework.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-10 20:58:19.000000 data-validation-framework-0.7.0/data_validation_framework.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-03-10 20:58:19.000000 data-validation-framework-0.7.0/data_validation_framework.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-03-10 20:58:19.000000 data-validation-framework-0.7.0/data_validation_framework.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 20:58:19.806461 data-validation-framework-0.7.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-03-10 20:58:10.000000 data-validation-framework-0.7.0/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 20:58:19.806461 data-validation-framework-0.7.0/docs/source/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-03-10 20:58:10.000000 data-validation-framework-0.7.0/docs/source/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-03-10 20:58:10.000000 data-validation-framework-0.7.0/docs/source/api_ref.rst
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-03-10 20:58:10.000000 data-validation-framework-0.7.0/docs/source/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2763 2023-03-10 20:58:10.000000 data-validation-framework-0.7.0/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-03-10 20:58:10.000000 data-validation-framework-0.7.0/docs/source/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-03-10 20:58:10.000000 data-validation-framework-0.7.0/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-03-10 20:58:10.000000 data-validation-framework-0.7.0/package.json
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-03-10 20:58:10.000000 data-validation-framework-0.7.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-10 20:58:19.810461 data-validation-framework-0.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-03-10 20:58:10.000000 data-validation-framework-0.7.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 20:58:19.806461 data-validation-framework-0.7.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-03-10 20:58:10.000000 data-validation-framework-0.7.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-03-10 20:58:10.000000 data-validation-framework-0.7.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 20:58:19.802461 data-validation-framework-0.7.0/tests/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 20:58:19.810461 data-validation-framework-0.7.0/tests/data/test_report/
--rw-r--r--   0 runner    (1001) docker     (123)    54609 2023-03-10 20:58:10.000000 data-validation-framework-0.7.0/tests/data/test_report/report_latexpdf.pdf
--rw-r--r--   0 runner    (1001) docker     (123)    16224 2023-03-10 20:58:10.000000 data-validation-framework-0.7.0/tests/data/test_report/report_no_exception_rst2pdf.pdf
--rw-r--r--   0 runner    (1001) docker     (123)    17614 2023-03-10 20:58:10.000000 data-validation-framework-0.7.0/tests/data/test_report/report_rst2pdf.pdf
--rw-r--r--   0 runner    (1001) docker     (123)    15033 2023-03-10 20:58:10.000000 data-validation-framework-0.7.0/tests/data/test_report/report_rst2pdf_all_fail.pdf
--rw-r--r--   0 runner    (1001) docker     (123)    13044 2023-03-10 20:58:10.000000 data-validation-framework-0.7.0/tests/data/test_report/report_rst2pdf_all_success.pdf
--rw-r--r--   0 runner    (1001) docker     (123)    15064 2023-03-10 20:58:10.000000 data-validation-framework-0.7.0/tests/data/test_report/report_rst2pdf_warnings.pdf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 20:58:19.810461 data-validation-framework-0.7.0/tests/data/test_report_before_run/
--rw-r--r--   0 runner    (1001) docker     (123)    34465 2023-03-10 20:58:10.000000 data-validation-framework-0.7.0/tests/data/test_report_before_run/report_latexpdf.pdf
--rw-r--r--   0 runner    (1001) docker     (123)    34807 2023-03-10 20:58:10.000000 data-validation-framework-0.7.0/tests/data/test_report_before_run/report_latexpdf_with_config.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     9927 2023-03-10 20:58:10.000000 data-validation-framework-0.7.0/tests/data/test_report_before_run/report_rst2pdf.pdf
--rw-r--r--   0 runner    (1001) docker     (123)    12110 2023-03-10 20:58:10.000000 data-validation-framework-0.7.0/tests/data/test_report_before_run/report_rst2pdf_nested.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     9923 2023-03-10 20:58:10.000000 data-validation-framework-0.7.0/tests/data/test_report_before_run/report_rst2pdf_with_config.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6394 2023-03-10 20:58:10.000000 data-validation-framework-0.7.0/tests/test_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     7196 2023-03-10 20:58:10.000000 data-validation-framework-0.7.0/tests/test_rst_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-03-10 20:58:10.000000 data-validation-framework-0.7.0/tests/test_target.py
--rw-r--r--   0 runner    (1001) docker     (123)   101392 2023-03-10 20:58:10.000000 data-validation-framework-0.7.0/tests/test_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     5194 2023-03-10 20:58:10.000000 data-validation-framework-0.7.0/tests/test_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-03-10 20:58:10.000000 data-validation-framework-0.7.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 23:12:56.137140 data-validation-framework-0.7.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-07-07 23:12:46.000000 data-validation-framework-0.7.1/.auto-changelog
+-rw-r--r--   0 runner    (1001) docker     (123)    10972 2023-07-07 23:12:46.000000 data-validation-framework-0.7.1/.auto-changelog-template.hbs
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 23:12:46.000000 data-validation-framework-0.7.1/.codespellignorelines
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-07 23:12:46.000000 data-validation-framework-0.7.1/.codespellrc
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-07-07 23:12:46.000000 data-validation-framework-0.7.1/.copier-answers.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-07-07 23:12:46.000000 data-validation-framework-0.7.1/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-07-07 23:12:46.000000 data-validation-framework-0.7.1/.flake8
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-07 23:12:46.000000 data-validation-framework-0.7.1/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 23:12:56.133140 data-validation-framework-0.7.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-07-07 23:12:46.000000 data-validation-framework-0.7.1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 23:12:56.133140 data-validation-framework-0.7.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2672 2023-07-07 23:12:46.000000 data-validation-framework-0.7.1/.github/workflows/codeql.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-07-07 23:12:46.000000 data-validation-framework-0.7.1/.github/workflows/commitlint.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-07-07 23:12:46.000000 data-validation-framework-0.7.1/.github/workflows/publish-sdist.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2382 2023-07-07 23:12:46.000000 data-validation-framework-0.7.1/.github/workflows/run-tox.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-07-07 23:12:46.000000 data-validation-framework-0.7.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-07-07 23:12:46.000000 data-validation-framework-0.7.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-07-07 23:12:46.000000 data-validation-framework-0.7.1/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-07-07 23:12:46.000000 data-validation-framework-0.7.1/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-07 23:12:46.000000 data-validation-framework-0.7.1/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10227 2023-07-07 23:12:46.000000 data-validation-framework-0.7.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4988 2023-07-07 23:12:46.000000 data-validation-framework-0.7.1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11354 2023-07-07 23:12:46.000000 data-validation-framework-0.7.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-07 23:12:46.000000 data-validation-framework-0.7.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8593 2023-07-07 23:12:56.137140 data-validation-framework-0.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7376 2023-07-07 23:12:46.000000 data-validation-framework-0.7.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-07 23:12:46.000000 data-validation-framework-0.7.1/codecov.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3759 2023-07-07 23:12:46.000000 data-validation-framework-0.7.1/commitlint.config.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 23:12:56.133140 data-validation-framework-0.7.1/data_validation_framework/
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-07-07 23:12:46.000000 data-validation-framework-0.7.1/data_validation_framework/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7330 2023-07-07 23:12:46.000000 data-validation-framework-0.7.1/data_validation_framework/report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4698 2023-07-07 23:12:46.000000 data-validation-framework-0.7.1/data_validation_framework/result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7440 2023-07-07 23:12:46.000000 data-validation-framework-0.7.1/data_validation_framework/rst_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-07-07 23:12:46.000000 data-validation-framework-0.7.1/data_validation_framework/target.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30156 2023-07-07 23:12:46.000000 data-validation-framework-0.7.1/data_validation_framework/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7504 2023-07-07 23:12:46.000000 data-validation-framework-0.7.1/data_validation_framework/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 23:12:56.133140 data-validation-framework-0.7.1/data_validation_framework.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8593 2023-07-07 23:12:56.000000 data-validation-framework-0.7.1/data_validation_framework.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-07-07 23:12:56.000000 data-validation-framework-0.7.1/data_validation_framework.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 23:12:56.000000 data-validation-framework-0.7.1/data_validation_framework.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-07-07 23:12:56.000000 data-validation-framework-0.7.1/data_validation_framework.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-07 23:12:56.000000 data-validation-framework-0.7.1/data_validation_framework.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 23:12:56.133140 data-validation-framework-0.7.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-07-07 23:12:46.000000 data-validation-framework-0.7.1/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 23:12:56.133140 data-validation-framework-0.7.1/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-07 23:12:46.000000 data-validation-framework-0.7.1/docs/source/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-07-07 23:12:46.000000 data-validation-framework-0.7.1/docs/source/api_ref.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-07 23:12:46.000000 data-validation-framework-0.7.1/docs/source/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2763 2023-07-07 23:12:46.000000 data-validation-framework-0.7.1/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-07 23:12:46.000000 data-validation-framework-0.7.1/docs/source/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-07 23:12:46.000000 data-validation-framework-0.7.1/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-07-07 23:12:46.000000 data-validation-framework-0.7.1/package.json
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-07-07 23:12:46.000000 data-validation-framework-0.7.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 23:12:56.137140 data-validation-framework-0.7.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-07-07 23:12:46.000000 data-validation-framework-0.7.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 23:12:56.137140 data-validation-framework-0.7.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-07-07 23:12:46.000000 data-validation-framework-0.7.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-07-07 23:12:46.000000 data-validation-framework-0.7.1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 23:12:56.129140 data-validation-framework-0.7.1/tests/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 23:12:56.137140 data-validation-framework-0.7.1/tests/data/test_report/
+-rw-r--r--   0 runner    (1001) docker     (123)    54609 2023-07-07 23:12:46.000000 data-validation-framework-0.7.1/tests/data/test_report/report_latexpdf.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)    16224 2023-07-07 23:12:46.000000 data-validation-framework-0.7.1/tests/data/test_report/report_no_exception_rst2pdf.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)    17614 2023-07-07 23:12:46.000000 data-validation-framework-0.7.1/tests/data/test_report/report_rst2pdf.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)    15033 2023-07-07 23:12:46.000000 data-validation-framework-0.7.1/tests/data/test_report/report_rst2pdf_all_fail.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)    13044 2023-07-07 23:12:46.000000 data-validation-framework-0.7.1/tests/data/test_report/report_rst2pdf_all_success.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)    15064 2023-07-07 23:12:46.000000 data-validation-framework-0.7.1/tests/data/test_report/report_rst2pdf_warnings.pdf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 23:12:56.137140 data-validation-framework-0.7.1/tests/data/test_report_before_run/
+-rw-r--r--   0 runner    (1001) docker     (123)    34465 2023-07-07 23:12:46.000000 data-validation-framework-0.7.1/tests/data/test_report_before_run/report_latexpdf.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)    34807 2023-07-07 23:12:46.000000 data-validation-framework-0.7.1/tests/data/test_report_before_run/report_latexpdf_with_config.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     9927 2023-07-07 23:12:46.000000 data-validation-framework-0.7.1/tests/data/test_report_before_run/report_rst2pdf.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)    12110 2023-07-07 23:12:46.000000 data-validation-framework-0.7.1/tests/data/test_report_before_run/report_rst2pdf_nested.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     9923 2023-07-07 23:12:46.000000 data-validation-framework-0.7.1/tests/data/test_report_before_run/report_rst2pdf_with_config.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6394 2023-07-07 23:12:46.000000 data-validation-framework-0.7.1/tests/test_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7196 2023-07-07 23:12:46.000000 data-validation-framework-0.7.1/tests/test_rst_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-07-07 23:12:46.000000 data-validation-framework-0.7.1/tests/test_target.py
+-rw-r--r--   0 runner    (1001) docker     (123)   101392 2023-07-07 23:12:46.000000 data-validation-framework-0.7.1/tests/test_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5194 2023-07-07 23:12:46.000000 data-validation-framework-0.7.1/tests/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-07-07 23:12:46.000000 data-validation-framework-0.7.1/tox.ini
```

### Comparing `data-validation-framework-0.7.0/.auto-changelog` & `data-validation-framework-0.7.1/.auto-changelog`

 * *Files identical despite different names*

### Comparing `data-validation-framework-0.7.0/.auto-changelog-template.hbs` & `data-validation-framework-0.7.1/.auto-changelog-template.hbs`

 * *Files identical despite different names*

### Comparing `data-validation-framework-0.7.0/.copier-answers.yml` & `data-validation-framework-0.7.1/.copier-answers.yml`

 * *Files identical despite different names*

### Comparing `data-validation-framework-0.7.0/.github/dependabot.yml` & `data-validation-framework-0.7.1/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `data-validation-framework-0.7.0/.github/workflows/codeql.yml` & `data-validation-framework-0.7.1/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `data-validation-framework-0.7.0/.github/workflows/commitlint.yml` & `data-validation-framework-0.7.1/.github/workflows/commitlint.yml`

 * *Files identical despite different names*

### Comparing `data-validation-framework-0.7.0/.github/workflows/publish-sdist.yml` & `data-validation-framework-0.7.1/.github/workflows/publish-sdist.yml`

 * *Files identical despite different names*

### Comparing `data-validation-framework-0.7.0/.github/workflows/run-tox.yml` & `data-validation-framework-0.7.1/.github/workflows/run-tox.yml`

 * *Files identical despite different names*

### Comparing `data-validation-framework-0.7.0/.pre-commit-config.yaml` & `data-validation-framework-0.7.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `data-validation-framework-0.7.0/.pylintrc` & `data-validation-framework-0.7.1/.pylintrc`

 * *Files identical despite different names*

### Comparing `data-validation-framework-0.7.0/CHANGELOG.md` & `data-validation-framework-0.7.1/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,17 @@
 # Changelog
 
+## [0.7.1](https://github.com/BlueBrain/data-validation-framework/compare/0.7.0..0.7.1)
+
+> 7 July 2023
+
+### Build
+
+- Bump max Sphinx version (Adrien Berchet - [#43](https://github.com/BlueBrain/data-validation-framework/pull/43))
+
 ## [0.7.0](https://github.com/BlueBrain/data-validation-framework/compare/0.6.4..0.7.0)
 
 > 10 March 2023
 
 ### New Features
 
 - Add a transform_index() method to transform the dataset index (Adrien Berchet - [#41](https://github.com/BlueBrain/data-validation-framework/pull/41))
```

### Comparing `data-validation-framework-0.7.0/CONTRIBUTING.md` & `data-validation-framework-0.7.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `data-validation-framework-0.7.0/LICENSE.txt` & `data-validation-framework-0.7.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `data-validation-framework-0.7.0/PKG-INFO` & `data-validation-framework-0.7.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: data-validation-framework
-Version: 0.7.0
+Version: 0.7.1
 Summary: Simple framework to create data validation workflows.
 Home-page: https://data-validation-framework.readthedocs.io
 Author: Blue Brain Project, EPFL
 License: Apache License 2.0
 Project-URL: Tracker, https://github.com/BlueBrain/data-validation-framework/issues
 Project-URL: Source, https://github.com/BlueBrain/data-validation-framework
 Classifier: Development Status :: 4 - Beta
```

### Comparing `data-validation-framework-0.7.0/README.md` & `data-validation-framework-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `data-validation-framework-0.7.0/commitlint.config.js` & `data-validation-framework-0.7.1/commitlint.config.js`

 * *Files identical despite different names*

### Comparing `data-validation-framework-0.7.0/data_validation_framework/report.py` & `data-validation-framework-0.7.1/data_validation_framework/report.py`

 * *Files identical despite different names*

### Comparing `data-validation-framework-0.7.0/data_validation_framework/result.py` & `data-validation-framework-0.7.1/data_validation_framework/result.py`

 * *Files identical despite different names*

### Comparing `data-validation-framework-0.7.0/data_validation_framework/rst_tools.py` & `data-validation-framework-0.7.1/data_validation_framework/rst_tools.py`

 * *Files identical despite different names*

### Comparing `data-validation-framework-0.7.0/data_validation_framework/target.py` & `data-validation-framework-0.7.1/data_validation_framework/target.py`

 * *Files identical despite different names*

### Comparing `data-validation-framework-0.7.0/data_validation_framework/task.py` & `data-validation-framework-0.7.1/data_validation_framework/task.py`

 * *Files identical despite different names*

### Comparing `data-validation-framework-0.7.0/data_validation_framework/util.py` & `data-validation-framework-0.7.1/data_validation_framework/util.py`

 * *Files identical despite different names*

### Comparing `data-validation-framework-0.7.0/data_validation_framework.egg-info/PKG-INFO` & `data-validation-framework-0.7.1/data_validation_framework.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: data-validation-framework
-Version: 0.7.0
+Version: 0.7.1
 Summary: Simple framework to create data validation workflows.
 Home-page: https://data-validation-framework.readthedocs.io
 Author: Blue Brain Project, EPFL
 License: Apache License 2.0
 Project-URL: Tracker, https://github.com/BlueBrain/data-validation-framework/issues
 Project-URL: Source, https://github.com/BlueBrain/data-validation-framework
 Classifier: Development Status :: 4 - Beta
```

### Comparing `data-validation-framework-0.7.0/data_validation_framework.egg-info/SOURCES.txt` & `data-validation-framework-0.7.1/data_validation_framework.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `data-validation-framework-0.7.0/docs/Makefile` & `data-validation-framework-0.7.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `data-validation-framework-0.7.0/docs/source/conf.py` & `data-validation-framework-0.7.1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `data-validation-framework-0.7.0/package.json` & `data-validation-framework-0.7.1/package.json`

 * *Files identical despite different names*

### Comparing `data-validation-framework-0.7.0/pyproject.toml` & `data-validation-framework-0.7.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `data-validation-framework-0.7.0/setup.py` & `data-validation-framework-0.7.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 reqs = [
     "luigi>=3.1",
     "luigi-tools>=0.0.18",
     "numpy>=1.21",
     "pandas>=1.3",
     "rst2pdf>=0.99",
-    "sphinx>=4,<6",
+    "sphinx>=4,<8",
     "tqdm>=4.40",
 ]
 doc_reqs = [
     "m2r2",
     "sphinx",
     "sphinx-bluebrain-theme",
 ]
```

### Comparing `data-validation-framework-0.7.0/tests/__init__.py` & `data-validation-framework-0.7.1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `data-validation-framework-0.7.0/tests/conftest.py` & `data-validation-framework-0.7.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `data-validation-framework-0.7.0/tests/data/test_report/report_latexpdf.pdf` & `data-validation-framework-0.7.1/tests/data/test_report/report_latexpdf.pdf`

 * *Files identical despite different names*

### Comparing `data-validation-framework-0.7.0/tests/data/test_report/report_no_exception_rst2pdf.pdf` & `data-validation-framework-0.7.1/tests/data/test_report/report_no_exception_rst2pdf.pdf`

 * *Files identical despite different names*

### Comparing `data-validation-framework-0.7.0/tests/data/test_report/report_rst2pdf.pdf` & `data-validation-framework-0.7.1/tests/data/test_report/report_rst2pdf.pdf`

 * *Files identical despite different names*

### Comparing `data-validation-framework-0.7.0/tests/data/test_report/report_rst2pdf_all_fail.pdf` & `data-validation-framework-0.7.1/tests/data/test_report/report_rst2pdf_all_fail.pdf`

 * *Files identical despite different names*

### Comparing `data-validation-framework-0.7.0/tests/data/test_report/report_rst2pdf_all_success.pdf` & `data-validation-framework-0.7.1/tests/data/test_report/report_rst2pdf_all_success.pdf`

 * *Files identical despite different names*

### Comparing `data-validation-framework-0.7.0/tests/data/test_report/report_rst2pdf_warnings.pdf` & `data-validation-framework-0.7.1/tests/data/test_report/report_rst2pdf_warnings.pdf`

 * *Files identical despite different names*

### Comparing `data-validation-framework-0.7.0/tests/data/test_report_before_run/report_latexpdf.pdf` & `data-validation-framework-0.7.1/tests/data/test_report_before_run/report_latexpdf.pdf`

 * *Files identical despite different names*

### Comparing `data-validation-framework-0.7.0/tests/data/test_report_before_run/report_latexpdf_with_config.pdf` & `data-validation-framework-0.7.1/tests/data/test_report_before_run/report_latexpdf_with_config.pdf`

 * *Files identical despite different names*

### Comparing `data-validation-framework-0.7.0/tests/data/test_report_before_run/report_rst2pdf.pdf` & `data-validation-framework-0.7.1/tests/data/test_report_before_run/report_rst2pdf.pdf`

 * *Files identical despite different names*

### Comparing `data-validation-framework-0.7.0/tests/data/test_report_before_run/report_rst2pdf_nested.pdf` & `data-validation-framework-0.7.1/tests/data/test_report_before_run/report_rst2pdf_nested.pdf`

 * *Files identical despite different names*

### Comparing `data-validation-framework-0.7.0/tests/data/test_report_before_run/report_rst2pdf_with_config.pdf` & `data-validation-framework-0.7.1/tests/data/test_report_before_run/report_rst2pdf_with_config.pdf`

 * *Files identical despite different names*

### Comparing `data-validation-framework-0.7.0/tests/test_result.py` & `data-validation-framework-0.7.1/tests/test_result.py`

 * *Files identical despite different names*

### Comparing `data-validation-framework-0.7.0/tests/test_rst_tools.py` & `data-validation-framework-0.7.1/tests/test_rst_tools.py`

 * *Files identical despite different names*

### Comparing `data-validation-framework-0.7.0/tests/test_target.py` & `data-validation-framework-0.7.1/tests/test_target.py`

 * *Files identical despite different names*

### Comparing `data-validation-framework-0.7.0/tests/test_task.py` & `data-validation-framework-0.7.1/tests/test_task.py`

 * *Files identical despite different names*

### Comparing `data-validation-framework-0.7.0/tests/test_util.py` & `data-validation-framework-0.7.1/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `data-validation-framework-0.7.0/tox.ini` & `data-validation-framework-0.7.1/tox.ini`

 * *Files identical despite different names*

