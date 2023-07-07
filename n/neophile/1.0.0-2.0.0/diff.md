# Comparing `tmp/neophile-1.0.0.tar.gz` & `tmp/neophile-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neophile-1.0.0.tar", last modified: Fri Jun 16 22:53:37 2023, max compression
+gzip compressed data, was "neophile-2.0.0.tar", last modified: Fri Jul  7 22:24:50 2023, max compression
```

## Comparing `neophile-1.0.0.tar` & `neophile-2.0.0.tar`

### file list

```diff
@@ -1,108 +1,108 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 22:53:37.385596 neophile-1.0.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 22:53:37.377596 neophile-1.0.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-06-16 22:53:27.000000 neophile-1.0.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 22:53:37.377596 neophile-1.0.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2810 2023-06-16 22:53:27.000000 neophile-1.0.0/.github/workflows/ci.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-06-16 22:53:27.000000 neophile-1.0.0/.github/workflows/dependencies.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2633 2023-06-16 22:53:27.000000 neophile-1.0.0/.github/workflows/periodic.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-06-16 22:53:27.000000 neophile-1.0.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-06-16 22:53:27.000000 neophile-1.0.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4902 2023-06-16 22:53:27.000000 neophile-1.0.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-06-16 22:53:27.000000 neophile-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-16 22:53:27.000000 neophile-1.0.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-06-16 22:53:37.385596 neophile-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-06-16 22:53:27.000000 neophile-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 22:53:37.377596 neophile-1.0.0/changelog.d/
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-16 22:53:27.000000 neophile-1.0.0/changelog.d/_template.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 22:53:37.377596 neophile-1.0.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-06-16 22:53:27.000000 neophile-1.0.0/docs/_rst_epilog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4902 2023-06-16 22:53:27.000000 neophile-1.0.0/docs/changelog.md
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-06-16 22:53:27.000000 neophile-1.0.0/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 22:53:37.377596 neophile-1.0.0/docs/dev/
--rw-r--r--   0 runner    (1001) docker     (123)     5964 2023-06-16 22:53:27.000000 neophile-1.0.0/docs/dev/development.rst
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-06-16 22:53:27.000000 neophile-1.0.0/docs/dev/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-06-16 22:53:27.000000 neophile-1.0.0/docs/dev/internals.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5005 2023-06-16 22:53:27.000000 neophile-1.0.0/docs/dev/release.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-06-16 22:53:27.000000 neophile-1.0.0/docs/documenteer.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-06-16 22:53:27.000000 neophile-1.0.0/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 22:53:37.377596 neophile-1.0.0/docs/user-guide/
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-06-16 22:53:27.000000 neophile-1.0.0/docs/user-guide/cli.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8190 2023-06-16 22:53:27.000000 neophile-1.0.0/docs/user-guide/github-actions.rst
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-06-16 22:53:27.000000 neophile-1.0.0/docs/user-guide/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6040 2023-06-16 22:53:27.000000 neophile-1.0.0/docs/user-guide/managing-dependencies.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3844 2023-06-16 22:53:27.000000 neophile-1.0.0/docs/user-guide/prerequisites.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-06-16 22:53:27.000000 neophile-1.0.0/docs/user-guide/running.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7446 2023-06-16 22:53:27.000000 neophile-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 22:53:37.385596 neophile-1.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 22:53:37.373595 neophile-1.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 22:53:37.377596 neophile-1.0.0/src/neophile/
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-06-16 22:53:27.000000 neophile-1.0.0/src/neophile/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 22:53:37.381595 neophile-1.0.0/src/neophile/analysis/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 22:53:27.000000 neophile-1.0.0/src/neophile/analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-06-16 22:53:27.000000 neophile-1.0.0/src/neophile/analysis/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1947 2023-06-16 22:53:27.000000 neophile-1.0.0/src/neophile/analysis/pre_commit.py
--rw-r--r--   0 runner    (1001) docker     (123)     2519 2023-06-16 22:53:27.000000 neophile-1.0.0/src/neophile/analysis/python.py
--rw-r--r--   0 runner    (1001) docker     (123)     4707 2023-06-16 22:53:27.000000 neophile-1.0.0/src/neophile/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-06-16 22:53:27.000000 neophile-1.0.0/src/neophile/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-06-16 22:53:27.000000 neophile-1.0.0/src/neophile/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3322 2023-06-16 22:53:27.000000 neophile-1.0.0/src/neophile/factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 22:53:37.381595 neophile-1.0.0/src/neophile/inventory/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 22:53:27.000000 neophile-1.0.0/src/neophile/inventory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2546 2023-06-16 22:53:27.000000 neophile-1.0.0/src/neophile/inventory/github.py
--rw-r--r--   0 runner    (1001) docker     (123)     4069 2023-06-16 22:53:27.000000 neophile-1.0.0/src/neophile/inventory/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 22:53:37.381595 neophile-1.0.0/src/neophile/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 22:53:27.000000 neophile-1.0.0/src/neophile/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-06-16 22:53:27.000000 neophile-1.0.0/src/neophile/models/dependencies.py
--rw-r--r--   0 runner    (1001) docker     (123)    12377 2023-06-16 22:53:27.000000 neophile-1.0.0/src/neophile/pr.py
--rw-r--r--   0 runner    (1001) docker     (123)     3003 2023-06-16 22:53:27.000000 neophile-1.0.0/src/neophile/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2216 2023-06-16 22:53:27.000000 neophile-1.0.0/src/neophile/repository.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 22:53:37.381595 neophile-1.0.0/src/neophile/scanner/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 22:53:27.000000 neophile-1.0.0/src/neophile/scanner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-06-16 22:53:27.000000 neophile-1.0.0/src/neophile/scanner/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-06-16 22:53:27.000000 neophile-1.0.0/src/neophile/scanner/pre_commit.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 22:53:37.381595 neophile-1.0.0/src/neophile/update/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 22:53:27.000000 neophile-1.0.0/src/neophile/update/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-06-16 22:53:27.000000 neophile-1.0.0/src/neophile/update/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-06-16 22:53:27.000000 neophile-1.0.0/src/neophile/update/pre_commit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-06-16 22:53:27.000000 neophile-1.0.0/src/neophile/update/python.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 22:53:37.381595 neophile-1.0.0/src/neophile.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-06-16 22:53:37.000000 neophile-1.0.0/src/neophile.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-06-16 22:53:37.000000 neophile-1.0.0/src/neophile.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 22:53:37.000000 neophile-1.0.0/src/neophile.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-16 22:53:37.000000 neophile-1.0.0/src/neophile.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-06-16 22:53:37.000000 neophile-1.0.0/src/neophile.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-16 22:53:37.000000 neophile-1.0.0/src/neophile.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 22:53:37.381595 neophile-1.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 22:53:27.000000 neophile-1.0.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 22:53:37.381595 neophile-1.0.0/tests/analysis/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 22:53:27.000000 neophile-1.0.0/tests/analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-06-16 22:53:27.000000 neophile-1.0.0/tests/analysis/pre_commit_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-06-16 22:53:27.000000 neophile-1.0.0/tests/analysis/python_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6643 2023-06-16 22:53:27.000000 neophile-1.0.0/tests/cli_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-06-16 22:53:27.000000 neophile-1.0.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 22:53:37.373595 neophile-1.0.0/tests/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 22:53:37.381595 neophile-1.0.0/tests/data/python/
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-06-16 22:53:27.000000 neophile-1.0.0/tests/data/python/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-06-16 22:53:27.000000 neophile-1.0.0/tests/data/python/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 22:53:37.385596 neophile-1.0.0/tests/data/python/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-16 22:53:27.000000 neophile-1.0.0/tests/data/python/requirements/main.in
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-06-16 22:53:27.000000 neophile-1.0.0/tests/data/python/requirements/main.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 22:53:37.385596 neophile-1.0.0/tests/inventory/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 22:53:27.000000 neophile-1.0.0/tests/inventory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-06-16 22:53:27.000000 neophile-1.0.0/tests/inventory/github_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-16 22:53:27.000000 neophile-1.0.0/tests/neophile_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8761 2023-06-16 22:53:27.000000 neophile-1.0.0/tests/pr_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6221 2023-06-16 22:53:27.000000 neophile-1.0.0/tests/processor_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-06-16 22:53:27.000000 neophile-1.0.0/tests/repository_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 22:53:37.385596 neophile-1.0.0/tests/scanner/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 22:53:27.000000 neophile-1.0.0/tests/scanner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-06-16 22:53:27.000000 neophile-1.0.0/tests/scanner/pre_commit_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 22:53:37.385596 neophile-1.0.0/tests/support/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 22:53:27.000000 neophile-1.0.0/tests/support/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4587 2023-06-16 22:53:27.000000 neophile-1.0.0/tests/support/github.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 22:53:37.385596 neophile-1.0.0/tests/update/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 22:53:27.000000 neophile-1.0.0/tests/update/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-06-16 22:53:27.000000 neophile-1.0.0/tests/update/pre_commit_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-06-16 22:53:27.000000 neophile-1.0.0/tests/update/python_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-06-16 22:53:27.000000 neophile-1.0.0/tests/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-06-16 22:53:27.000000 neophile-1.0.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 22:24:50.467779 neophile-2.0.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 22:24:50.443779 neophile-2.0.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-07-07 22:24:39.000000 neophile-2.0.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 22:24:50.443779 neophile-2.0.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2810 2023-07-07 22:24:39.000000 neophile-2.0.0/.github/workflows/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-07-07 22:24:39.000000 neophile-2.0.0/.github/workflows/dependencies.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2633 2023-07-07 22:24:39.000000 neophile-2.0.0/.github/workflows/periodic.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-07-07 22:24:39.000000 neophile-2.0.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-07-07 22:24:39.000000 neophile-2.0.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6012 2023-07-07 22:24:39.000000 neophile-2.0.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-07-07 22:24:39.000000 neophile-2.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-07 22:24:39.000000 neophile-2.0.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-07-07 22:24:50.467779 neophile-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-07-07 22:24:39.000000 neophile-2.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 22:24:50.443779 neophile-2.0.0/changelog.d/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-07 22:24:39.000000 neophile-2.0.0/changelog.d/_template.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 22:24:50.447779 neophile-2.0.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-07-07 22:24:39.000000 neophile-2.0.0/docs/_rst_epilog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6012 2023-07-07 22:24:39.000000 neophile-2.0.0/docs/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-07-07 22:24:39.000000 neophile-2.0.0/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 22:24:50.447779 neophile-2.0.0/docs/dev/
+-rw-r--r--   0 runner    (1001) docker     (123)     5964 2023-07-07 22:24:39.000000 neophile-2.0.0/docs/dev/development.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-07-07 22:24:39.000000 neophile-2.0.0/docs/dev/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-07-07 22:24:39.000000 neophile-2.0.0/docs/dev/internals.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5005 2023-07-07 22:24:39.000000 neophile-2.0.0/docs/dev/release.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-07-07 22:24:39.000000 neophile-2.0.0/docs/documenteer.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-07-07 22:24:39.000000 neophile-2.0.0/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 22:24:50.451779 neophile-2.0.0/docs/user-guide/
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-07 22:24:39.000000 neophile-2.0.0/docs/user-guide/cli.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8110 2023-07-07 22:24:39.000000 neophile-2.0.0/docs/user-guide/github-actions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-07-07 22:24:39.000000 neophile-2.0.0/docs/user-guide/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6040 2023-07-07 22:24:39.000000 neophile-2.0.0/docs/user-guide/managing-dependencies.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3844 2023-07-07 22:24:39.000000 neophile-2.0.0/docs/user-guide/prerequisites.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-07-07 22:24:39.000000 neophile-2.0.0/docs/user-guide/running.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7505 2023-07-07 22:24:39.000000 neophile-2.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 22:24:50.467779 neophile-2.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 22:24:50.439779 neophile-2.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 22:24:50.451779 neophile-2.0.0/src/neophile/
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-07-07 22:24:39.000000 neophile-2.0.0/src/neophile/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 22:24:50.455779 neophile-2.0.0/src/neophile/analysis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 22:24:39.000000 neophile-2.0.0/src/neophile/analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-07-07 22:24:39.000000 neophile-2.0.0/src/neophile/analysis/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1947 2023-07-07 22:24:39.000000 neophile-2.0.0/src/neophile/analysis/pre_commit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2519 2023-07-07 22:24:39.000000 neophile-2.0.0/src/neophile/analysis/python.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4707 2023-07-07 22:24:39.000000 neophile-2.0.0/src/neophile/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-07-07 22:24:39.000000 neophile-2.0.0/src/neophile/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-07-07 22:24:39.000000 neophile-2.0.0/src/neophile/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3322 2023-07-07 22:24:39.000000 neophile-2.0.0/src/neophile/factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 22:24:50.455779 neophile-2.0.0/src/neophile/inventory/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 22:24:39.000000 neophile-2.0.0/src/neophile/inventory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2546 2023-07-07 22:24:39.000000 neophile-2.0.0/src/neophile/inventory/github.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4069 2023-07-07 22:24:39.000000 neophile-2.0.0/src/neophile/inventory/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 22:24:50.455779 neophile-2.0.0/src/neophile/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 22:24:39.000000 neophile-2.0.0/src/neophile/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-07-07 22:24:39.000000 neophile-2.0.0/src/neophile/models/dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14537 2023-07-07 22:24:39.000000 neophile-2.0.0/src/neophile/pr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3003 2023-07-07 22:24:39.000000 neophile-2.0.0/src/neophile/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2216 2023-07-07 22:24:39.000000 neophile-2.0.0/src/neophile/repository.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 22:24:50.459779 neophile-2.0.0/src/neophile/scanner/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 22:24:39.000000 neophile-2.0.0/src/neophile/scanner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-07-07 22:24:39.000000 neophile-2.0.0/src/neophile/scanner/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-07-07 22:24:39.000000 neophile-2.0.0/src/neophile/scanner/pre_commit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 22:24:50.459779 neophile-2.0.0/src/neophile/update/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 22:24:39.000000 neophile-2.0.0/src/neophile/update/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-07-07 22:24:39.000000 neophile-2.0.0/src/neophile/update/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-07-07 22:24:39.000000 neophile-2.0.0/src/neophile/update/pre_commit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-07-07 22:24:39.000000 neophile-2.0.0/src/neophile/update/python.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 22:24:50.455779 neophile-2.0.0/src/neophile.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-07-07 22:24:50.000000 neophile-2.0.0/src/neophile.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-07-07 22:24:50.000000 neophile-2.0.0/src/neophile.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 22:24:50.000000 neophile-2.0.0/src/neophile.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-07 22:24:50.000000 neophile-2.0.0/src/neophile.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-07-07 22:24:50.000000 neophile-2.0.0/src/neophile.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-07 22:24:50.000000 neophile-2.0.0/src/neophile.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 22:24:50.463779 neophile-2.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 22:24:39.000000 neophile-2.0.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 22:24:50.463779 neophile-2.0.0/tests/analysis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 22:24:39.000000 neophile-2.0.0/tests/analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-07-07 22:24:39.000000 neophile-2.0.0/tests/analysis/pre_commit_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-07-07 22:24:39.000000 neophile-2.0.0/tests/analysis/python_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6653 2023-07-07 22:24:39.000000 neophile-2.0.0/tests/cli_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-07-07 22:24:39.000000 neophile-2.0.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 22:24:50.439779 neophile-2.0.0/tests/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 22:24:50.463779 neophile-2.0.0/tests/data/python/
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-07-07 22:24:39.000000 neophile-2.0.0/tests/data/python/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-07-07 22:24:39.000000 neophile-2.0.0/tests/data/python/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 22:24:50.463779 neophile-2.0.0/tests/data/python/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-07 22:24:39.000000 neophile-2.0.0/tests/data/python/requirements/main.in
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-07-07 22:24:39.000000 neophile-2.0.0/tests/data/python/requirements/main.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 22:24:50.463779 neophile-2.0.0/tests/inventory/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 22:24:39.000000 neophile-2.0.0/tests/inventory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-07-07 22:24:39.000000 neophile-2.0.0/tests/inventory/github_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-07 22:24:39.000000 neophile-2.0.0/tests/neophile_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10033 2023-07-07 22:24:39.000000 neophile-2.0.0/tests/pr_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6278 2023-07-07 22:24:39.000000 neophile-2.0.0/tests/processor_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-07-07 22:24:39.000000 neophile-2.0.0/tests/repository_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 22:24:50.463779 neophile-2.0.0/tests/scanner/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 22:24:39.000000 neophile-2.0.0/tests/scanner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-07-07 22:24:39.000000 neophile-2.0.0/tests/scanner/pre_commit_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 22:24:50.467779 neophile-2.0.0/tests/support/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 22:24:39.000000 neophile-2.0.0/tests/support/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4587 2023-07-07 22:24:39.000000 neophile-2.0.0/tests/support/github.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 22:24:50.467779 neophile-2.0.0/tests/update/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 22:24:39.000000 neophile-2.0.0/tests/update/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-07-07 22:24:39.000000 neophile-2.0.0/tests/update/pre_commit_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-07-07 22:24:39.000000 neophile-2.0.0/tests/update/python_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-07-07 22:24:39.000000 neophile-2.0.0/tests/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-07-07 22:24:39.000000 neophile-2.0.0/tox.ini
```

### Comparing `neophile-1.0.0/.github/workflows/ci.yaml` & `neophile-2.0.0/.github/workflows/ci.yaml`

 * *Files identical despite different names*

### Comparing `neophile-1.0.0/.github/workflows/dependencies.yaml` & `neophile-2.0.0/.github/workflows/dependencies.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -20,15 +20,14 @@
 
       - name: Install neophile
         run: make init
 
       - name: Run neophile
         run: neophile update --pr pre-commit
         env:
-          NEOPHILE_COMMIT_EMAIL: "24442459+sqrbot@users.noreply.github.com"
           NEOPHILE_GITHUB_APP_ID: ${{ secrets.NEOPHILE_APP_ID }}
           NEOPHILE_GITHUB_PRIVATE_KEY: ${{ secrets.NEOPHILE_PRIVATE_KEY }}
 
       - name: Report status
         if: always()
         uses: ravsamhq/notify-slack-action@v2
         with:
```

### Comparing `neophile-1.0.0/.github/workflows/periodic.yaml` & `neophile-2.0.0/.github/workflows/periodic.yaml`

 * *Files identical despite different names*

### Comparing `neophile-1.0.0/.gitignore` & `neophile-2.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `neophile-1.0.0/.pre-commit-config.yaml` & `neophile-2.0.0/.pre-commit-config.yaml`

 * *Files 17% similar despite different names*

```diff
@@ -5,15 +5,15 @@
       - id: check-merge-conflict
       - id: check-toml
       - id: check-yaml
         args: [--allow-multiple-documents]
       - id: trailing-whitespace
 
   - repo: https://github.com/astral-sh/ruff-pre-commit
-    rev: v0.0.272
+    rev: v0.0.277
     hooks:
       - id: ruff
         args: [--fix, --exit-non-zero-on-fix]
 
   - repo: https://github.com/psf/black
     rev: 23.3.0
     hooks:
```

### Comparing `neophile-1.0.0/CHANGELOG.md` & `neophile-2.0.0/CHANGELOG.md`

 * *Files 19% similar despite different names*

```diff
@@ -7,14 +7,29 @@
 Dependencies are updated to the latest available version during each release. Those changes are not noted here explicitly.
 
 This project uses [scriv](https://scriv.readthedocs.io/en/latest/) to maintain the change log.
 Changes for the upcoming release can be found in [changelog.d](https://github.com/lsst-sqre/neophile/tree/main/changelog.d/).
 
 <!-- scriv-insert-here -->
 
+<a id='changelog-2.0.0'></a>
+## 2.0.0 (2023-07-07)
+
+### Backwards-incompatible changes
+
+- The `NEOPHILE_COMMIT_NAME` environment variable is no longer supported. Instead, `NEOPHILE_USERNAME` configures the GitHub username of the running instantiation of neophile, used as both the name for Git commits and to construct the email address unless `NEOPHILE_COMMIT_EMAIL` is given. `NEOPHILE_USERNAME` defaults to `neophile-square[bot]`, the instantiation of neophile for the lsst-sqre organization.
+
+### New features
+
+- Setting `NEOPHILE_COMMIT_EMAIL` is now optional. If not set, the UID of the GitHub user from `NEOPHILE_USERNAME` is retrieved from the GitHub API and used to form a standard GitHub no-replay email address.
+
+### Bug fixes
+
+- Use the GitHub App installation token when pushing Git changes in preparation for creating a PR rather than using the default GitHub Actions token. If the branch was pushed with the GitHub Actions token, further GitHub Actions refuse to run on that branch to avoid creating a loop, but we need GitHub Actions to run so that the dependency update PR can be automerged.
+
 <a id='changelog-1.0.0'></a>
 ## 1.0.0 (2023-06-16)
 
 ### Backwards-incompatible changes
 
 - neophile is now intended to be run either via GitHub Actions or on a local checkout, and never as a Kubernetes service. The `neophile process` command, the configuration specific to that command (work area, lists of repositories), and support for running inside a virtualenv have been removed.
 - When creating PRs, neophile now must be configured as a GitHub App with a suitable application ID and private key in environment variables.
```

### Comparing `neophile-1.0.0/LICENSE` & `neophile-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `neophile-1.0.0/PKG-INFO` & `neophile-2.0.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neophile
-Version: 1.0.0
+Version: 2.0.0
 Summary: Scan repositories for obsolete versions
 License: MIT License
         
         Copyright 2020-2023 Association of Universities for Research in Astronomy, Inc. (AURA)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `neophile-1.0.0/README.md` & `neophile-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `neophile-1.0.0/docs/changelog.md` & `neophile-2.0.0/docs/changelog.md`

 * *Files 19% similar despite different names*

```diff
@@ -7,14 +7,29 @@
 Dependencies are updated to the latest available version during each release. Those changes are not noted here explicitly.
 
 This project uses [scriv](https://scriv.readthedocs.io/en/latest/) to maintain the change log.
 Changes for the upcoming release can be found in [changelog.d](https://github.com/lsst-sqre/neophile/tree/main/changelog.d/).
 
 <!-- scriv-insert-here -->
 
+<a id='changelog-2.0.0'></a>
+## 2.0.0 (2023-07-07)
+
+### Backwards-incompatible changes
+
+- The `NEOPHILE_COMMIT_NAME` environment variable is no longer supported. Instead, `NEOPHILE_USERNAME` configures the GitHub username of the running instantiation of neophile, used as both the name for Git commits and to construct the email address unless `NEOPHILE_COMMIT_EMAIL` is given. `NEOPHILE_USERNAME` defaults to `neophile-square[bot]`, the instantiation of neophile for the lsst-sqre organization.
+
+### New features
+
+- Setting `NEOPHILE_COMMIT_EMAIL` is now optional. If not set, the UID of the GitHub user from `NEOPHILE_USERNAME` is retrieved from the GitHub API and used to form a standard GitHub no-replay email address.
+
+### Bug fixes
+
+- Use the GitHub App installation token when pushing Git changes in preparation for creating a PR rather than using the default GitHub Actions token. If the branch was pushed with the GitHub Actions token, further GitHub Actions refuse to run on that branch to avoid creating a loop, but we need GitHub Actions to run so that the dependency update PR can be automerged.
+
 <a id='changelog-1.0.0'></a>
 ## 1.0.0 (2023-06-16)
 
 ### Backwards-incompatible changes
 
 - neophile is now intended to be run either via GitHub Actions or on a local checkout, and never as a Kubernetes service. The `neophile process` command, the configuration specific to that command (work area, lists of repositories), and support for running inside a virtualenv have been removed.
 - When creating PRs, neophile now must be configured as a GitHub App with a suitable application ID and private key in environment variables.
```

### Comparing `neophile-1.0.0/docs/dev/development.rst` & `neophile-2.0.0/docs/dev/development.rst`

 * *Files identical despite different names*

### Comparing `neophile-1.0.0/docs/dev/internals.rst` & `neophile-2.0.0/docs/dev/internals.rst`

 * *Files identical despite different names*

### Comparing `neophile-1.0.0/docs/dev/release.rst` & `neophile-2.0.0/docs/dev/release.rst`

 * *Files identical despite different names*

### Comparing `neophile-1.0.0/docs/documenteer.toml` & `neophile-2.0.0/docs/documenteer.toml`

 * *Files identical despite different names*

### Comparing `neophile-1.0.0/docs/index.rst` & `neophile-2.0.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `neophile-1.0.0/docs/user-guide/github-actions.rst` & `neophile-2.0.0/docs/user-guide/github-actions.rst`

 * *Files 4% similar despite different names*

```diff
@@ -79,21 +79,20 @@
 
          - name: Install neophile
            run: pip install neophile
 
          - name: Run neophile
            run: neophile update --pr pre-commit
            env:
-             NEOPHILE_COMMIT_EMAIL: "24442459+sqrbot@users.noreply.github.com"
              NEOPHILE_GITHUB_APP_ID: ${{ secrets.NEOPHILE_APP_ID }}
              NEOPHILE_GITHUB_PRIVATE_KEY: ${{ secrets.NEOPHILE_PRIVATE_KEY }}
 
          - name: Report status
            if: always()
-           uses: ravsamhq/notify-slack-action@v1
+           uses: ravsamhq/notify-slack-action@v2
            with:
              status: ${{ job.status }}
              notify_when: "failure"
              notification_title: "Periodic dependency update for {repo} failed"
            env:
              SLACK_WEBHOOK_URL: ${{ secrets.SLACK_ALERT_WEBHOOK }}
 
@@ -105,22 +104,22 @@
 neophile configuration
 ----------------------
 
 ``NEOPHILE_GITHUB_APP_ID`` and ``NEOPHILE_GITHUB_PRIVATE_KEY`` must be set to the secrets containing the GitHub App credentials for neophile.
 See :ref:`actions-setup` for more information.
 Two more environment variables may be set to customize neophile's behavior:
 
-``NEOPHILE_COMMIT_NAME`` (optional)
-    The name portion of the author and committer for the Git commit updating the dependencies.
-    If not set, defaults to ``neophile``.
-
-``NEOPHILE_COMMIT_EMAIL`` (required)
+``NEOPHILE_COMMIT_EMAIL`` (optional)
     The email address to use for the author and committer of the Git commit updating these dependencies.
-    The value shown in the example above is the GitHub email for the ``sqrbot`` user used by SQuaRE, and is an appropriate setting for SQuaRE-maintained packages.
-    For non-SQuaRE packages, set it to some appropriate value for your organization.
+    If this is not set, a standard GitHub email address will be derived from ``NEOPHILE_USERNAME``.
+
+``NEOPHILE_USERNAME`` (optional)
+    The GitHub username (``login``) of the GitHub App, used as the name portion of the author and committer for Git commits.
+    If ``NEOPHILE_COMMIT_EMAIL`` is not set, this is also used to retrieve the UID of this GitHub user and construct a standard GitHub email address to use for the commit.
+    If not set, defaults to ``neophile-square[bot]``.
 
 .. _slack-alerts:
 
 Slack alerts
 ------------
 
 The final step of this action reports any failures to Slack.
@@ -135,20 +134,19 @@
 When application Python dependencies are not regularly updated (between rounds of development, for example), it is still useful to periodically check if updated dependencies would break the application.
 These problems can then be caught more quickly, when it's easy to understand what has changed and there are a smaller number of issues to fix.
 Addressing upgrade issues regularly avoids having to do a massive round of upgrades as part of the next release, involving possibly confusing and interacting issues from multiple dependency changes.
 
 The recommended approach for doing this is a weekly GitHub Actions workflow that uses neophile to update dependencies and then runs the test suite.
 
 .. code-block:: yaml
+   :caption: periodic.yaml
 
    # This is a separate run of the Python test suite that doesn't cache
-   # the tox environment and runs from a schedule.  The purpose is to test
-   # compatibility with the latest versions of all modules neophile
-   # depends on, since neophile (being a PyPI application) does not pin
-   # its dependencies.
+   # the tox environment and runs from a schedule. The purpose is to test
+   # whether updating pinned dependencies would cause any tests to fail.
 
    name: Periodic CI
 
    "on":
      schedule:
        - cron: "0 12 * * 1"
      workflow_dispatch: {}
@@ -184,15 +182,15 @@
            uses: lsst-sqre/run-tox@v1
            with:
              python-version: ${{ matrix.python }}
              tox-envs: "lint,typing,py"
 
          - name: Report status
            if: always()
-           uses: ravsamhq/notify-slack-action@v1
+           uses: ravsamhq/notify-slack-action@v2
            with:
              status: ${{ job.status }}
              notify_when: "failure"
              notification_title: "Periodic test for {repo} failed"
            env:
              SLACK_WEBHOOK_URL: ${{ secrets.SLACK_ALERT_WEBHOOK }}
```

### Comparing `neophile-1.0.0/docs/user-guide/managing-dependencies.rst` & `neophile-2.0.0/docs/user-guide/managing-dependencies.rst`

 * *Files identical despite different names*

### Comparing `neophile-1.0.0/docs/user-guide/prerequisites.rst` & `neophile-2.0.0/docs/user-guide/prerequisites.rst`

 * *Files identical despite different names*

### Comparing `neophile-1.0.0/docs/user-guide/running.rst` & `neophile-2.0.0/docs/user-guide/running.rst`

 * *Files identical despite different names*

### Comparing `neophile-1.0.0/pyproject.toml` & `neophile-2.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     "Natural Language :: English",
     "Operating System :: POSIX",
     "Typing :: Typed",
 ]
 requires-python = ">=3.11"
 dependencies = [
     "GitPython",
-    "click",
+    "click!=8.1.4",  # see https://github.com/pallets/click/issues/2558
     "gidgethub",
     "httpx",
     "packaging",
     "pydantic",
     "ruamel.yaml",
     "safir",
     "semver",
```

### Comparing `neophile-1.0.0/src/neophile/analysis/base.py` & `neophile-2.0.0/src/neophile/analysis/base.py`

 * *Files identical despite different names*

### Comparing `neophile-1.0.0/src/neophile/analysis/pre_commit.py` & `neophile-2.0.0/src/neophile/analysis/pre_commit.py`

 * *Files identical despite different names*

### Comparing `neophile-1.0.0/src/neophile/analysis/python.py` & `neophile-2.0.0/src/neophile/analysis/python.py`

 * *Files identical despite different names*

### Comparing `neophile-1.0.0/src/neophile/cli.py` & `neophile-2.0.0/src/neophile/cli.py`

 * *Files identical despite different names*

### Comparing `neophile-1.0.0/src/neophile/config.py` & `neophile-2.0.0/src/neophile/config.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,34 +1,38 @@
 """Configuration for neophile."""
 
 from __future__ import annotations
 
-from git.util import Actor
 from pydantic import BaseSettings, Field, SecretStr
 
 __all__ = ["Config"]
 
 
 class Config(BaseSettings):
     """Configuration for neophile."""
 
-    commit_name: str = Field(
-        "neophile", description="Name to use for GitHub commits"
-    )
-
-    commit_email: str | None = Field(
-        None, description="Email address to use for GitHub commits"
-    )
-
     github_app_id: str = Field("", description="GitHub App ID")
 
     github_private_key: SecretStr = Field(
         SecretStr(""), description="GitHub App private key"
     )
 
+    username: str = Field(
+        "neophile-square[bot]",
+        description=(
+            "Username, used as the name for GitHub commits and as part of"
+            " the email address if `commit_email` is not set. In the latter"
+            " case, must be the same as the login attribute in the GitHub"
+            " users API."
+        ),
+    )
+
+    commit_email: str | None = Field(
+        None,
+        description=(
+            "Email address to use for GitHub commits. If `None`, a GitHub"
+            " bot email address will be constructed using `github_app_id`."
+        ),
+    )
+
     class Config:
         env_prefix = "neophile_"
-
-    @property
-    def actor(self) -> Actor:
-        """Git actor to use for commits."""
-        return Actor(self.commit_name, self.commit_email)
```

### Comparing `neophile-1.0.0/src/neophile/exceptions.py` & `neophile-2.0.0/src/neophile/exceptions.py`

 * *Files identical despite different names*

### Comparing `neophile-1.0.0/src/neophile/factory.py` & `neophile-2.0.0/src/neophile/factory.py`

 * *Files identical despite different names*

### Comparing `neophile-1.0.0/src/neophile/inventory/github.py` & `neophile-2.0.0/src/neophile/inventory/github.py`

 * *Files identical despite different names*

### Comparing `neophile-1.0.0/src/neophile/inventory/version.py` & `neophile-2.0.0/src/neophile/inventory/version.py`

 * *Files identical despite different names*

### Comparing `neophile-1.0.0/src/neophile/models/dependencies.py` & `neophile-2.0.0/src/neophile/models/dependencies.py`

 * *Files identical despite different names*

### Comparing `neophile-1.0.0/src/neophile/processor.py` & `neophile-2.0.0/src/neophile/processor.py`

 * *Files identical despite different names*

### Comparing `neophile-1.0.0/src/neophile/repository.py` & `neophile-2.0.0/src/neophile/repository.py`

 * *Files identical despite different names*

### Comparing `neophile-1.0.0/src/neophile/scanner/base.py` & `neophile-2.0.0/src/neophile/scanner/base.py`

 * *Files identical despite different names*

### Comparing `neophile-1.0.0/src/neophile/scanner/pre_commit.py` & `neophile-2.0.0/src/neophile/scanner/pre_commit.py`

 * *Files identical despite different names*

### Comparing `neophile-1.0.0/src/neophile/update/base.py` & `neophile-2.0.0/src/neophile/update/base.py`

 * *Files identical despite different names*

### Comparing `neophile-1.0.0/src/neophile/update/pre_commit.py` & `neophile-2.0.0/src/neophile/update/pre_commit.py`

 * *Files identical despite different names*

### Comparing `neophile-1.0.0/src/neophile/update/python.py` & `neophile-2.0.0/src/neophile/update/python.py`

 * *Files identical despite different names*

### Comparing `neophile-1.0.0/src/neophile.egg-info/PKG-INFO` & `neophile-2.0.0/src/neophile.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neophile
-Version: 1.0.0
+Version: 2.0.0
 Summary: Scan repositories for obsolete versions
 License: MIT License
         
         Copyright 2020-2023 Association of Universities for Research in Astronomy, Inc. (AURA)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `neophile-1.0.0/src/neophile.egg-info/SOURCES.txt` & `neophile-2.0.0/src/neophile.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `neophile-1.0.0/tests/analysis/pre_commit_test.py` & `neophile-2.0.0/tests/analysis/pre_commit_test.py`

 * *Files identical despite different names*

### Comparing `neophile-1.0.0/tests/analysis/python_test.py` & `neophile-2.0.0/tests/analysis/python_test.py`

 * *Files identical despite different names*

### Comparing `neophile-1.0.0/tests/cli_test.py` & `neophile-2.0.0/tests/cli_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -157,16 +157,16 @@
         }
 
         assert repo.head.ref.name == "u/neophile"
         yaml = YAML()
         data = yaml.load(dst)
         assert data["repos"][2]["rev"] == "20.0.0"
         commit = repo.head.commit
-        assert commit.author.name == "neophile"
-        assert commit.author.email == "neophile@example.com"
+        assert commit.author.name == "neophile-square[bot]"
+        assert commit.author.email == "someone@example.com"
         assert commit.message == f"{CommitMessage.title}\n\n- {change}\n"
 
         nonlocal created_pr
         created_pr = True
         return Response(201, json={"number": 42})
 
     mock_github_tags_from_precommit(
@@ -185,16 +185,16 @@
     )
     mock_enable_auto_merge(respx_mock, "foo", "bar", "42")
 
     result = runner.invoke(
         main,
         ["update", "--path", str(tmp_path), "--pr"],
         env={
+            "NEOPHILE_COMMIT_EMAIL": "someone@example.com",
             "NEOPHILE_GITHUB_PRIVATE_KEY": github_key,
-            "NEOPHILE_COMMIT_EMAIL": "neophile@example.com",
         },
     )
     assert result.exit_code == 0
     assert created_pr
     assert mock_push.call_args_list == [
         call("u/neophile:u/neophile", force=True)
     ]
```

### Comparing `neophile-1.0.0/tests/conftest.py` & `neophile-2.0.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `neophile-1.0.0/tests/data/python/.pre-commit-config.yaml` & `neophile-2.0.0/tests/data/python/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `neophile-1.0.0/tests/inventory/github_test.py` & `neophile-2.0.0/tests/inventory/github_test.py`

 * *Files identical despite different names*

### Comparing `neophile-1.0.0/tests/pr_test.py` & `neophile-2.0.0/tests/pr_test.py`

 * *Files 14% similar despite different names*

```diff
@@ -29,27 +29,26 @@
     client: AsyncClient,
     respx_mock: respx.Router,
     github_key: str,
     mock_push: Mock,
 ) -> None:
     repo = setup_python_repo(tmp_path)
     Remote.create(repo, "origin", "https://github.com/foo/bar")
-    config = Config(
-        commit_name="Someone",
-        commit_email="someone@example.com",
-        github_private_key=SecretStr(github_key),
-    )
+    config = Config(github_private_key=SecretStr(github_key))
     update = PreCommitUpdate(
         path=tmp_path / ".pre-commit-config.yaml",
         applied=False,
         repository="https://github.com/ambv/black",
         current="19.10b0",
         latest="23.3.0",
     )
     mock_app_authenticate(respx_mock, "foo/bar")
+    respx_mock.get(f"https://api.github.com/users/{config.username}").mock(
+        return_value=Response(200, json={"id": 123456}),
+    )
     respx_mock.get("https://api.github.com/repos/foo/bar").mock(
         return_value=Response(200, json={"default_branch": "main"})
     )
     pattern = r"https://api.github.com/repos/foo/bar/pulls\?.*base=main.*"
     respx_mock.get(url__regex=pattern).mock(
         return_value=Response(200, json=[])
     )
@@ -66,32 +65,37 @@
 
     assert mock_push.call_args_list == [
         call("u/neophile:u/neophile", force=True)
     ]
     assert not repo.is_dirty()
     assert repo.head.ref.name == "u/neophile"
     commit = repo.head.commit
-    assert commit.author.name == "Someone"
-    assert commit.author.email == "someone@example.com"
-    assert commit.committer.name == "Someone"
-    assert commit.committer.email == "someone@example.com"
+    expected_email = f"123456+{config.username}@users.noreply.github.com"
+    assert commit.author.name == config.username
+    assert commit.author.email == expected_email
+    assert commit.committer.name == config.username
+    assert commit.committer.email == expected_email
     change = "Update ambv/black pre-commit hook from 19.10b0 to 23.3.0"
     assert commit.message == f"{CommitMessage.title}\n\n- {change}\n"
+    assert "tmp-neophile" not in [r.name for r in repo.remotes]
 
 
 @pytest.mark.asyncio
 async def test_pr_push_failure(
     tmp_path: Path,
     client: AsyncClient,
     respx_mock: respx.Router,
     github_key: str,
 ) -> None:
     repo = setup_python_repo(tmp_path)
     Remote.create(repo, "origin", "https://github.com/foo/bar")
-    config = Config(github_private_key=SecretStr(github_key))
+    config = Config(
+        commit_email="someone@example.com",
+        github_private_key=SecretStr(github_key),
+    )
     update = PreCommitUpdate(
         path=tmp_path / ".pre-commit-config.yaml",
         applied=False,
         repository="https://github.com/ambv/black",
         current="19.10b0",
         latest="23.3.0",
     )
@@ -124,15 +128,14 @@
     respx_mock: respx.Router,
     github_key: str,
     mock_push: Mock,
 ) -> None:
     repo = setup_python_repo(tmp_path)
     Remote.create(repo, "origin", "https://github.com/foo/bar")
     config = Config(
-        commit_name="Someone",
         commit_email="someone@example.com",
         github_private_key=SecretStr(github_key),
     )
     update = PreCommitUpdate(
         path=tmp_path / ".pre-commit-config.yaml",
         applied=False,
         repository="https://github.com/ambv/black",
@@ -160,35 +163,36 @@
 
     assert mock_push.call_args_list == [
         call("u/neophile:u/neophile", force=True)
     ]
     assert not repo.is_dirty()
     assert repo.head.ref.name == "u/neophile"
     commit = repo.head.commit
-    assert commit.author.name == "Someone"
+    assert commit.author.name == config.username
     assert commit.author.email == "someone@example.com"
-    assert commit.committer.name == "Someone"
+    assert commit.committer.name == config.username
     assert commit.committer.email == "someone@example.com"
     change = "Update ambv/black pre-commit hook from 19.10b0 to 23.3.0"
     assert commit.message == f"{CommitMessage.title}\n\n- {change}\n"
+    assert "tmp-neophile" not in [r.name for r in repo.remotes]
 
 
 @pytest.mark.asyncio
 async def test_pr_update(
     tmp_path: Path,
     client: AsyncClient,
     respx_mock: respx.Router,
     github_key: str,
     mock_push: Mock,
 ) -> None:
     """Test updating an existing PR."""
     repo = setup_python_repo(tmp_path)
     Remote.create(repo, "origin", "https://github.com/foo/bar")
     config = Config(
-        commit_name="Someone",
+        username="neophile[bot]",
         commit_email="otheremail@example.com",
         github_private_key=SecretStr(github_key),
     )
     update = PreCommitUpdate(
         path=tmp_path / ".pre-commit-config.yaml",
         applied=False,
         repository="https://github.com/ambv/black",
@@ -229,21 +233,45 @@
 
     assert mock_push.call_args_list == [
         call("u/neophile:u/neophile", force=True)
     ]
     assert not repo.is_dirty()
     assert repo.head.ref.name == "u/neophile"
     commit = repo.head.commit
-    assert commit.author.name == "Someone"
+    assert commit.author.name == "neophile[bot]"
     assert commit.author.email == "otheremail@example.com"
-    assert commit.committer.name == "Someone"
+    assert commit.committer.name == "neophile[bot]"
     assert commit.committer.email == "otheremail@example.com"
 
 
 @pytest.mark.asyncio
+async def test_get_authenticated_remote(
+    tmp_path: Path, client: AsyncClient
+) -> None:
+    repo = Repo.init(str(tmp_path), initial_branch="main")
+    pr = PullRequester(Config(), client)
+
+    remote = Remote.create(repo, "origin", "https://github.com/foo/bar")
+    url = pr._get_authenticated_remote(repo, "some-token")
+    assert url == "https://neophile:some-token@github.com/foo/bar"
+
+    remote.set_url("https://foo@github.com:8080/foo/bar")
+    url = pr._get_authenticated_remote(repo, "some-token")
+    assert url == "https://neophile:some-token@github.com:8080/foo/bar"
+
+    remote.set_url("git@github.com:bar/foo")
+    url = pr._get_authenticated_remote(repo, "some-token")
+    assert url == "https://neophile:some-token@github.com/bar/foo"
+
+    remote.set_url("ssh://git:blahblah@github.com/baz/stuff")
+    url = pr._get_authenticated_remote(repo, "some-token")
+    assert url == "https://neophile:some-token@github.com/baz/stuff"
+
+
+@pytest.mark.asyncio
 async def test_get_github_repo(tmp_path: Path, client: AsyncClient) -> None:
     repo = Repo.init(str(tmp_path), initial_branch="main")
     pr = PullRequester(Config(), client)
 
     remote = Remote.create(repo, "origin", "git@github.com:foo/bar.git")
     github_repo = pr._get_github_repo(repo)
     assert github_repo == GitHubRepository(owner="foo", repo="bar")
```

### Comparing `neophile-1.0.0/tests/processor_test.py` & `neophile-2.0.0/tests/processor_test.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 from git import PushInfo, Remote
 from git.repo import Repo
 from git.util import Actor
 from httpx import AsyncClient, Request, Response
 from pydantic import SecretStr
 from ruamel.yaml import YAML
 
+from neophile.config import Config
 from neophile.factory import Factory
 from neophile.pr import CommitMessage
 
 from .support.github import (
     mock_app_authenticate,
     mock_enable_auto_merge,
     mock_github_tags_from_precommit,
@@ -109,15 +110,15 @@
 
         repo = Repo(str(tmp_path / "tmp"))
         assert repo.head.ref.name == "u/neophile"
         yaml = YAML()
         data = yaml.load(tmp_path / "tmp" / ".pre-commit-config.yaml")
         assert data["repos"][2]["rev"] == "20.0.0"
         commit = repo.head.commit
-        assert commit.author.name == "neophile"
+        assert commit.author.name == "neophile-square[bot]"
         assert commit.author.email == "someone@example.com"
         assert commit.message == f"{CommitMessage.title}\n\n{body}"
 
         nonlocal created_pr
         created_pr = True
         return Response(201, json={"number": 42})
 
@@ -138,16 +139,18 @@
         side_effect=check_pr_post
     )
     mock_enable_auto_merge(respx_mock, "foo", "bar", "42")
 
     # Unfortunately, the mock_push fixture can't be used here because we
     # want to use git.Remote.push in create_upstream_git_repository.
     factory = Factory(client)
-    factory._config.commit_email = "someone@example.com"
-    factory._config.github_private_key = SecretStr(github_key)
+    factory._config = Config(
+        commit_email="someone@example.com",
+        github_private_key=SecretStr(github_key),
+    )
     processor = factory.create_processor()
     with patch_clone_from("foo", "bar", upstream_path):
         with patch.object(Remote, "push") as mock_push:
             mock_push.return_value = push_result
             await processor.process_checkout(tmp_path / "tmp")
 
     assert mock_push.call_args_list == [
```

### Comparing `neophile-1.0.0/tests/repository_test.py` & `neophile-2.0.0/tests/repository_test.py`

 * *Files identical despite different names*

### Comparing `neophile-1.0.0/tests/scanner/pre_commit_test.py` & `neophile-2.0.0/tests/scanner/pre_commit_test.py`

 * *Files identical despite different names*

### Comparing `neophile-1.0.0/tests/support/github.py` & `neophile-2.0.0/tests/support/github.py`

 * *Files identical despite different names*

### Comparing `neophile-1.0.0/tests/update/pre_commit_test.py` & `neophile-2.0.0/tests/update/pre_commit_test.py`

 * *Files identical despite different names*

### Comparing `neophile-1.0.0/tests/update/python_test.py` & `neophile-2.0.0/tests/update/python_test.py`

 * *Files identical despite different names*

### Comparing `neophile-1.0.0/tests/util.py` & `neophile-2.0.0/tests/util.py`

 * *Files identical despite different names*

### Comparing `neophile-1.0.0/tox.ini` & `neophile-2.0.0/tox.ini`

 * *Files identical despite different names*

