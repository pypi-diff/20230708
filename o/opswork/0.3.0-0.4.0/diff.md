# Comparing `tmp/opswork-0.3.0.tar.gz` & `tmp/opswork-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opswork-0.3.0.tar", last modified: Tue Jul  4 10:47:13 2023, max compression
+gzip compressed data, was "opswork-0.4.0.tar", last modified: Fri Jul  7 23:43:38 2023, max compression
```

## Comparing `opswork-0.3.0.tar` & `opswork-0.4.0.tar`

### file list

```diff
@@ -1,72 +1,75 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:47:13.745717 opswork-0.3.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:47:13.741717 opswork-0.3.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-07-04 10:46:47.000000 opswork-0.3.0/.github/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-04 10:46:47.000000 opswork-0.3.0/.github/FUNDING.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:47:13.741717 opswork-0.3.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-07-04 10:46:47.000000 opswork-0.3.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-07-04 10:46:47.000000 opswork-0.3.0/.github/ISSUE_TEMPLATE/feature_request.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:47:13.745717 opswork-0.3.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-07-04 10:46:47.000000 opswork-0.3.0/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-04 10:46:47.000000 opswork-0.3.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-07-04 10:46:47.000000 opswork-0.3.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-04 10:46:47.000000 opswork-0.3.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-07-04 10:46:47.000000 opswork-0.3.0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5219 2023-07-04 10:46:47.000000 opswork-0.3.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)      742 2023-07-04 10:46:47.000000 opswork-0.3.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-04 10:46:47.000000 opswork-0.3.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-07-04 10:46:47.000000 opswork-0.3.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     3121 2023-07-04 10:47:13.749717 opswork-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-07-04 10:46:47.000000 opswork-0.3.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:47:13.745717 opswork-0.3.0/cache/
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-04 10:46:47.000000 opswork-0.3.0/cache/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-07-04 10:46:47.000000 opswork-0.3.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:47:13.741717 opswork-0.3.0/recipe/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:47:13.745717 opswork-0.3.0/recipe/motd/
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-07-04 10:46:47.000000 opswork-0.3.0/recipe/motd/motd.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-07-04 10:46:47.000000 opswork-0.3.0/recipe/motd/recipe.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:47:13.745717 opswork-0.3.0/recipe/nginx/
--rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-07-04 10:46:47.000000 opswork-0.3.0/recipe/nginx/recipe.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:47:13.745717 opswork-0.3.0/recipe/ping/
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-07-04 10:46:47.000000 opswork-0.3.0/recipe/ping/recipe.yml
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-04 10:46:47.000000 opswork-0.3.0/renovate.json
--rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-07-04 10:47:13.749717 opswork-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-07-04 10:46:47.000000 opswork-0.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:47:13.741717 opswork-0.3.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:47:13.745717 opswork-0.3.0/src/opswork/
--rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-07-04 10:46:47.000000 opswork-0.3.0/src/opswork/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6769 2023-07-04 10:46:47.000000 opswork-0.3.0/src/opswork/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:47:13.745717 opswork-0.3.0/src/opswork/command/
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-07-04 10:46:47.000000 opswork-0.3.0/src/opswork/command/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3226 2023-07-04 10:46:47.000000 opswork-0.3.0/src/opswork/command/configs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4924 2023-07-04 10:46:47.000000 opswork-0.3.0/src/opswork/command/hosts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-07-04 10:46:47.000000 opswork-0.3.0/src/opswork/command/random.py
--rw-r--r--   0 runner    (1001) docker     (123)     6296 2023-07-04 10:46:47.000000 opswork-0.3.0/src/opswork/command/recipes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:47:13.745717 opswork-0.3.0/src/opswork/exception/
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-07-04 10:46:47.000000 opswork-0.3.0/src/opswork/exception/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:47:13.745717 opswork-0.3.0/src/opswork/model/
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-07-04 10:46:47.000000 opswork-0.3.0/src/opswork/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-07-04 10:46:47.000000 opswork-0.3.0/src/opswork/model/host.py
--rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-07-04 10:46:47.000000 opswork-0.3.0/src/opswork/model/recipe.py
--rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-07-04 10:46:47.000000 opswork-0.3.0/src/opswork/model/task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:47:13.745717 opswork-0.3.0/src/opswork/module/
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-07-04 10:46:47.000000 opswork-0.3.0/src/opswork/module/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-07-04 10:46:47.000000 opswork-0.3.0/src/opswork/module/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     7053 2023-07-04 10:46:47.000000 opswork-0.3.0/src/opswork/module/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     3441 2023-07-04 10:46:47.000000 opswork-0.3.0/src/opswork/module/file_system.py
--rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-07-04 10:46:47.000000 opswork-0.3.0/src/opswork/module/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-07-04 10:46:47.000000 opswork-0.3.0/src/opswork/module/output.py
--rw-r--r--   0 runner    (1001) docker     (123)     4470 2023-07-04 10:46:47.000000 opswork-0.3.0/src/opswork/module/playbook.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:47:13.745717 opswork-0.3.0/src/opswork.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3121 2023-07-04 10:47:13.000000 opswork-0.3.0/src/opswork.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-07-04 10:47:13.000000 opswork-0.3.0/src/opswork.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 10:47:13.000000 opswork-0.3.0/src/opswork.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-04 10:47:13.000000 opswork-0.3.0/src/opswork.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 10:47:13.000000 opswork-0.3.0/src/opswork.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-04 10:47:13.000000 opswork-0.3.0/src/opswork.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-04 10:47:13.000000 opswork-0.3.0/src/opswork.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:47:13.745717 opswork-0.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-07-04 10:46:47.000000 opswork-0.3.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:47:13.745717 opswork-0.3.0/tests/module/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 10:46:47.000000 opswork-0.3.0/tests/module/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-07-04 10:46:47.000000 opswork-0.3.0/tests/module/test_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-07-04 10:46:47.000000 opswork-0.3.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 23:43:38.070668 opswork-0.4.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 23:43:38.050668 opswork-0.4.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-07-07 23:43:17.000000 opswork-0.4.0/.github/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-07 23:43:17.000000 opswork-0.4.0/.github/FUNDING.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 23:43:38.050668 opswork-0.4.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-07-07 23:43:17.000000 opswork-0.4.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-07-07 23:43:17.000000 opswork-0.4.0/.github/ISSUE_TEMPLATE/feature_request.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 23:43:38.050668 opswork-0.4.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-07-07 23:43:17.000000 opswork-0.4.0/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-07 23:43:17.000000 opswork-0.4.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-07-07 23:43:17.000000 opswork-0.4.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-07 23:43:17.000000 opswork-0.4.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-07-07 23:43:17.000000 opswork-0.4.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5219 2023-07-07 23:43:17.000000 opswork-0.4.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-07-07 23:43:17.000000 opswork-0.4.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-07 23:43:17.000000 opswork-0.4.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-07-07 23:43:17.000000 opswork-0.4.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     3121 2023-07-07 23:43:38.070668 opswork-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-07-07 23:43:17.000000 opswork-0.4.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 23:43:38.054668 opswork-0.4.0/cache/
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-07 23:43:17.000000 opswork-0.4.0/cache/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-07-07 23:43:17.000000 opswork-0.4.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 23:43:38.042668 opswork-0.4.0/recipe/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 23:43:38.054668 opswork-0.4.0/recipe/motd/
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-07-07 23:43:17.000000 opswork-0.4.0/recipe/motd/motd.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-07-07 23:43:17.000000 opswork-0.4.0/recipe/motd/recipe.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 23:43:38.054668 opswork-0.4.0/recipe/nginx/
+-rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-07-07 23:43:17.000000 opswork-0.4.0/recipe/nginx/recipe.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 23:43:38.054668 opswork-0.4.0/recipe/ping/
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-07-07 23:43:17.000000 opswork-0.4.0/recipe/ping/recipe.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-07 23:43:17.000000 opswork-0.4.0/renovate.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-07-07 23:43:38.070668 opswork-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-07-07 23:43:17.000000 opswork-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 23:43:38.042668 opswork-0.4.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 23:43:38.054668 opswork-0.4.0/src/opswork/
+-rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-07-07 23:43:17.000000 opswork-0.4.0/src/opswork/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8224 2023-07-07 23:43:17.000000 opswork-0.4.0/src/opswork/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 23:43:38.062668 opswork-0.4.0/src/opswork/command/
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-07-07 23:43:17.000000 opswork-0.4.0/src/opswork/command/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3530 2023-07-07 23:43:17.000000 opswork-0.4.0/src/opswork/command/configs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4924 2023-07-07 23:43:17.000000 opswork-0.4.0/src/opswork/command/hosts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-07-07 23:43:17.000000 opswork-0.4.0/src/opswork/command/random.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6296 2023-07-07 23:43:17.000000 opswork-0.4.0/src/opswork/command/recipes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4332 2023-07-07 23:43:17.000000 opswork-0.4.0/src/opswork/command/secret.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 23:43:38.062668 opswork-0.4.0/src/opswork/exception/
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-07-07 23:43:17.000000 opswork-0.4.0/src/opswork/exception/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 23:43:38.062668 opswork-0.4.0/src/opswork/model/
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-07-07 23:43:17.000000 opswork-0.4.0/src/opswork/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-07-07 23:43:17.000000 opswork-0.4.0/src/opswork/model/host.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-07-07 23:43:17.000000 opswork-0.4.0/src/opswork/model/recipe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-07-07 23:43:17.000000 opswork-0.4.0/src/opswork/model/secret.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-07-07 23:43:17.000000 opswork-0.4.0/src/opswork/model/task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 23:43:38.066668 opswork-0.4.0/src/opswork/module/
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-07-07 23:43:17.000000 opswork-0.4.0/src/opswork/module/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-07-07 23:43:17.000000 opswork-0.4.0/src/opswork/module/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9406 2023-07-07 23:43:17.000000 opswork-0.4.0/src/opswork/module/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-07-07 23:43:17.000000 opswork-0.4.0/src/opswork/module/encrypt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3441 2023-07-07 23:43:17.000000 opswork-0.4.0/src/opswork/module/file_system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-07-07 23:43:17.000000 opswork-0.4.0/src/opswork/module/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-07-07 23:43:17.000000 opswork-0.4.0/src/opswork/module/output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4470 2023-07-07 23:43:17.000000 opswork-0.4.0/src/opswork/module/playbook.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 23:43:38.058668 opswork-0.4.0/src/opswork.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3121 2023-07-07 23:43:38.000000 opswork-0.4.0/src/opswork.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-07-07 23:43:38.000000 opswork-0.4.0/src/opswork.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 23:43:38.000000 opswork-0.4.0/src/opswork.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-07 23:43:38.000000 opswork-0.4.0/src/opswork.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 23:43:37.000000 opswork-0.4.0/src/opswork.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-07-07 23:43:38.000000 opswork-0.4.0/src/opswork.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-07 23:43:38.000000 opswork-0.4.0/src/opswork.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 23:43:38.070668 opswork-0.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-07-07 23:43:17.000000 opswork-0.4.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 23:43:38.070668 opswork-0.4.0/tests/module/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 23:43:17.000000 opswork-0.4.0/tests/module/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-07-07 23:43:17.000000 opswork-0.4.0/tests/module/test_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-07-07 23:43:17.000000 opswork-0.4.0/tox.ini
```

### Comparing `opswork-0.3.0/.github/workflows/release.yml` & `opswork-0.4.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `opswork-0.3.0/.gitignore` & `opswork-0.4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `opswork-0.3.0/CODE_OF_CONDUCT.md` & `opswork-0.4.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `opswork-0.3.0/CONTRIBUTING.rst` & `opswork-0.4.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `opswork-0.3.0/LICENSE.txt` & `opswork-0.4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `opswork-0.3.0/Makefile` & `opswork-0.4.0/Makefile`

 * *Files identical despite different names*

### Comparing `opswork-0.3.0/PKG-INFO` & `opswork-0.4.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: opswork
-Version: 0.3.0
+Version: 0.4.0
 Summary: OpsWork Swiss Knife.
-Home-page: https://github.com/clivern/opswork/
+Home-page: https://github.com/Clivern/OpsWork/
 Author: Clivern
 Author-email: hello@clivern.com
 License: MIT
-Project-URL: Documentation, https://github.com/clivern/opswork/
-Project-URL: Source, https://github.com/clivern/opswork/
-Project-URL: Changelog, https://github.com/clivern/opswork/blob/main/CHANGELOG.rst
-Project-URL: Tracker, https://github.com/clivern/opswork/issues
-Project-URL: Download, https://pypi.org/project/opswork/#files
+Project-URL: Documentation, https://github.com/Clivern/OpsWork/
+Project-URL: Source, https://github.com/Clivern/OpsWork/
+Project-URL: Changelog, https://github.com/Clivern/OpsWork/blob/main/CHANGELOG.rst
+Project-URL: Tracker, https://github.com/Clivern/OpsWork/issues
+Project-URL: Download, https://pypi.org/project/OpsWork/#files
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/x-rst; charset=UTF-8
 License-File: LICENSE.txt
```

### Comparing `opswork-0.3.0/README.rst` & `opswork-0.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `opswork-0.3.0/recipe/motd/recipe.yml` & `opswork-0.4.0/recipe/motd/recipe.yml`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 
 vars:
-  version: v0.3
+  version: v0.4
 
 templates:
   motd.j2: motd.j2
 
 tasks:
   - name: check mandatory variables
     assert:
```

### Comparing `opswork-0.3.0/recipe/nginx/recipe.yml` & `opswork-0.4.0/recipe/nginx/recipe.yml`

 * *Files identical despite different names*

### Comparing `opswork-0.3.0/recipe/ping/recipe.yml` & `opswork-0.4.0/recipe/ping/recipe.yml`

 * *Files identical despite different names*

### Comparing `opswork-0.3.0/setup.cfg` & `opswork-0.4.0/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -3,39 +3,40 @@
 description = OpsWork Swiss Knife.
 author = Clivern
 author_email = hello@clivern.com
 license = MIT
 license_files = LICENSE.txt
 long_description = file: README.rst
 long_description_content_type = text/x-rst; charset=UTF-8
-url = https://github.com/clivern/opswork/
+url = https://github.com/Clivern/OpsWork/
 project_urls = 
-	Documentation = https://github.com/clivern/opswork/
-	Source = https://github.com/clivern/opswork/
-	Changelog = https://github.com/clivern/opswork/blob/main/CHANGELOG.rst
-	Tracker = https://github.com/clivern/opswork/issues
-	Download = https://pypi.org/project/opswork/#files
+	Documentation = https://github.com/Clivern/OpsWork/
+	Source = https://github.com/Clivern/OpsWork/
+	Changelog = https://github.com/Clivern/OpsWork/blob/main/CHANGELOG.rst
+	Tracker = https://github.com/Clivern/OpsWork/issues
+	Download = https://pypi.org/project/OpsWork/#files
 platforms = any
 classifiers = 
 	Development Status :: 5 - Production/Stable
 	Programming Language :: Python
 	License :: OSI Approved :: MIT License
 
 [options]
 zip_safe = False
 packages = find_namespace:
 include_package_data = True
 package_dir = 
 	=src
 install_requires = 
-	click<=8.1.3
+	click<=8.1.4
 	ansible-runner<=2.3.3
 	prettytable<=3.8.0
 	PyYAML<=6.0
-	importlib-metadata<=6.7.0; python_version<"3.8"
+	cryptography<=41.0.1
+	importlib-metadata<=6.8.0; python_version<"3.8"
 
 [options.packages.find]
 where = src
 exclude = 
 	tests
 	recipe
 	cache
```

### Comparing `opswork-0.3.0/setup.py` & `opswork-0.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `opswork-0.3.0/src/opswork/__init__.py` & `opswork-0.4.0/src/opswork/__init__.py`

 * *Files identical despite different names*

### Comparing `opswork-0.3.0/src/opswork/cli.py` & `opswork-0.4.0/src/opswork/cli.py`

 * *Files 20% similar despite different names*

```diff
@@ -22,17 +22,19 @@
 
 import uuid
 import click
 import logging, json, sys
 
 from opswork import __version__
 from opswork.model.host import Host
+from opswork.model.secret import Secret
 from opswork.command.hosts import Hosts
 from opswork.command.configs import Configs
 from opswork.command.recipes import Recipes
+from opswork.command.secret import Secrets
 from opswork.command.random import Random
 
 
 @click.group(help="🐺 OpsWork Swiss Knife")
 @click.version_option(version=__version__, help="Show the current version")
 def main():
     pass
@@ -247,14 +249,66 @@
 
 # Show configs sub command
 @config.command(help="Show configurations")
 def dump():
     return Configs().dump()
 
 
+# Secrets command
+@click.group(help="Manage secrets")
+def secret():
+    pass
+
+
+# Add secrets sub command
+@secret.command(help="Add a secret")
+@click.argument("name")
+@click.argument("value")
+@click.option("-t", "--tags", "tags", type=click.STRING, default="", help="Secret tags")
+@click.option("-f", "--force", "force", is_flag=True, default=False, help="Force add")
+def add(name, value, tags, force):
+    secret = Secret(
+        str(uuid.uuid4()),
+        name,
+        value,
+        tags.split(",") if tags != "" else [],
+        None,
+        None,
+    )
+
+    return Secrets().init().add(secret, force)
+
+
+# List secrets sub command
+@secret.command(help="List all secrets")
+@click.option("-t", "--tag", "tag", type=click.STRING, default="", help="Secret tag")
+@click.option(
+    "-o", "--output", "output", type=click.STRING, default="", help="Output format"
+)
+def list(tag, output):
+    return Secrets().init().list(tag, output)
+
+
+# Get secret sub command
+@secret.command(help="Get a secret")
+@click.argument("name")
+@click.option(
+    "-o", "--output", "output", type=click.STRING, default="", help="Output format"
+)
+def get(name, output):
+    return Secrets().init().get(name, output)
+
+
+# Delete secret sub command
+@secret.command(help="Delete a secret")
+@click.argument("name")
+def delete(name):
+    return Secrets().init().delete(name)
+
+
 # Random data command
 @click.group(help="Random data")
 def random():
     pass
 
 
 # Init random sub command
@@ -264,12 +318,13 @@
     return Random().password(int(length))
 
 
 # Register Commands
 main.add_command(host)
 main.add_command(recipe)
 main.add_command(config)
+main.add_command(secret)
 main.add_command(random)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `opswork-0.3.0/src/opswork/command/__init__.py` & `opswork-0.4.0/src/opswork/command/__init__.py`

 * *Files identical despite different names*

### Comparing `opswork-0.3.0/src/opswork/command/configs.py` & `opswork-0.4.0/src/opswork/command/configs.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,69 +24,78 @@
 import yaml
 import click
 
 from opswork.module.logger import Logger
 from opswork.module.output import Output
 from opswork.module.database import Database
 from opswork.module.file_system import FileSystem
+from opswork.module.encrypt import Encrypt
 
 
 class Configs:
     """Configs Class"""
 
     FILE = ".opswork.yml"
 
     def __init__(self):
         self.database = Database()
         self.file_system = FileSystem()
-        self._home = os.getenv("HOME", "")
+        self.home = os.getenv("HOME", "")
+        self.encrypt = Encrypt()
         self.logger = Logger().get_logger(__name__)
 
     def init(self):
         """Init Configs"""
-        if self._home == "":
+        if self.home == "":
             raise click.ClickException("User home path is not defined")
 
+        if self.file_system.file_exists("{}/{}".format(self.home, Configs.FILE)):
+            raise click.ClickException("Config file exists!")
+
         base = {
-            "database": {"type": "file", "path": "{}/opswork.db".format(self._home)},
+            "database": {
+                "type": "file",
+                "path": "{}/opswork.db".format(self.home),
+                "token": self.encrypt.get_key(),
+            },
             "cache": {"path": "/tmp"},
         }
 
-        self.database.connect("{}/opswork.db".format(self._home))
+        self.database.connect("{}/opswork.db".format(self.home))
         self.database.migrate()
 
         self.file_system.write_file(
-            "{}/{}".format(self._home, Configs.FILE), yaml.dump(base)
+            "{}/{}".format(self.home, Configs.FILE), yaml.dump(base)
         )
 
         click.echo(
             "Config file {} got created!".format(
-                click.format_filename("{}/{}".format(self._home, Configs.FILE))
+                click.format_filename("{}/{}".format(self.home, Configs.FILE))
             )
         )
 
     def edit(self):
         """Edit Configs"""
-        if self._home == "":
+        if self.home == "":
             raise click.ClickException("User home path is not defined")
 
-        if not self.file_system.file_exists("{}/{}".format(self._home, Configs.FILE)):
+        if not self.file_system.file_exists("{}/{}".format(self.home, Configs.FILE)):
             raise click.ClickException("Config file is missing")
 
-        click.edit(filename="{}/{}".format(self._home, Configs.FILE))
+        click.edit(filename="{}/{}".format(self.home, Configs.FILE))
 
         click.echo(
             "Config file {} got updated!".format(
-                click.format_filename("{}/{}".format(self._home, Configs.FILE))
+                click.format_filename("{}/{}".format(self.home, Configs.FILE))
             )
         )
 
     def dump(self):
         """Dump Configs"""
-        if self._home == "":
+        if self.home == "":
             raise click.ClickException("User home path is not defined")
 
-        if not self.file_system.file_exists("{}/{}".format(self._home, Configs.FILE)):
+        if not self.file_system.file_exists("{}/{}".format(self.home, Configs.FILE)):
             raise click.ClickException("Config file is missing")
 
         print("")
-        print(self.file_system.read_file("{}/{}".format(self._home, Configs.FILE)))
+        print(self.file_system.read_file("{}/{}".format(self.home, Configs.FILE)))
```

### Comparing `opswork-0.3.0/src/opswork/command/hosts.py` & `opswork-0.4.0/src/opswork/command/hosts.py`

 * *Files identical despite different names*

### Comparing `opswork-0.3.0/src/opswork/command/random.py` & `opswork-0.4.0/src/opswork/command/random.py`

 * *Files identical despite different names*

### Comparing `opswork-0.3.0/src/opswork/command/recipes.py` & `opswork-0.4.0/src/opswork/command/recipes.py`

 * *Files identical despite different names*

### Comparing `opswork-0.3.0/src/opswork/exception/__init__.py` & `opswork-0.4.0/src/opswork/exception/__init__.py`

 * *Files identical despite different names*

### Comparing `opswork-0.3.0/src/opswork/model/__init__.py` & `opswork-0.4.0/src/opswork/model/__init__.py`

 * *Files identical despite different names*

### Comparing `opswork-0.3.0/src/opswork/model/host.py` & `opswork-0.4.0/src/opswork/model/host.py`

 * *Files identical despite different names*

### Comparing `opswork-0.3.0/src/opswork/model/recipe.py` & `opswork-0.4.0/src/opswork/model/recipe.py`

 * *Files identical despite different names*

### Comparing `opswork-0.3.0/src/opswork/model/task.py` & `opswork-0.4.0/src/opswork/model/task.py`

 * *Files identical despite different names*

### Comparing `opswork-0.3.0/src/opswork/module/__init__.py` & `opswork-0.4.0/src/opswork/module/__init__.py`

 * *Files identical despite different names*

### Comparing `opswork-0.3.0/src/opswork/module/config.py` & `opswork-0.4.0/src/opswork/module/config.py`

 * *Files identical despite different names*

### Comparing `opswork-0.3.0/src/opswork/module/database.py` & `opswork-0.4.0/src/opswork/module/database.py`

 * *Files 22% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 # SOFTWARE.
 
 import json
 import sqlite3
 
 from opswork.model.host import Host
 from opswork.model.recipe import Recipe
+from opswork.model.secret import Secret
 
 
 class Database:
     """Database Class"""
 
     def connect(self, path):
         """Connect into a database"""
@@ -46,28 +47,21 @@
         )
         cursor.execute(
             "CREATE TABLE IF NOT EXISTS recipe (id TEXT, name TEXT, config TEXT, createdAt TEXT, updatedAt TEXT)"
         )
         cursor.execute(
             "CREATE TABLE IF NOT EXISTS task (id TEXT, name TEXT, payload TEXT, result TEXT, createdAt TEXT, updatedAt TEXT)"
         )
+        cursor.execute(
+            "CREATE TABLE IF NOT EXISTS secret (id TEXT, name TEXT, value TEXT, createdAt TEXT, updatedAt TEXT)"
+        )
 
         cursor.close()
         self._connection.commit()
 
-    def delete_host(self, name):
-        """Delete a row by host name"""
-        cursor = self._connection.cursor()
-
-        cursor.execute("DELETE FROM host WHERE name = ?", (name,))
-
-        cursor.close()
-
-        self._connection.commit()
-
     def get_host(self, name):
         """Get a row by host name"""
         cursor = self._connection.cursor()
 
         rows = cursor.execute(
             "SELECT id, name, config, createdAt, updatedAt FROM host WHERE name = '{}'".format(
                 name
@@ -153,19 +147,19 @@
                 row[4],
             )
 
             result.append(host)
 
         return result
 
-    def delete_recipe(self, name):
-        """Delete a row by recipe name"""
+    def delete_host(self, name):
+        """Delete a row by host name"""
         cursor = self._connection.cursor()
 
-        cursor.execute("DELETE FROM recipe WHERE name = ?", (name,))
+        cursor.execute("DELETE FROM host WHERE name = ?", (name,))
 
         cursor.close()
 
         self._connection.commit()
 
     def get_recipe(self, name):
         """Get a row by recipe name"""
@@ -239,7 +233,107 @@
                 data["tags"],
                 row[3],
                 row[4],
             )
             result.append(recipe)
 
         return result
+
+    def delete_recipe(self, name):
+        """Delete a row by recipe name"""
+        cursor = self._connection.cursor()
+
+        cursor.execute("DELETE FROM recipe WHERE name = ?", (name,))
+
+        cursor.close()
+
+        self._connection.commit()
+
+    def get_secret(self, name):
+        """Get a row by secret name"""
+        cursor = self._connection.cursor()
+
+        rows = cursor.execute(
+            "SELECT id, name, value, createdAt, updatedAt FROM secret WHERE name = '{}'".format(
+                name
+            )
+        ).fetchall()
+
+        cursor.close()
+
+        if len(rows) > 0:
+            for row in rows:
+                data = json.loads(row[2])
+
+                secret = Secret(
+                    row[0],
+                    row[1],
+                    data["value"],
+                    data["tags"],
+                    row[3],
+                    row[4],
+                )
+
+                return secret
+        else:
+            return None
+
+    def list_secrets(self):
+        """List all rows"""
+        result = []
+
+        cursor = self._connection.cursor()
+
+        rows = cursor.execute(
+            "SELECT id, name, value, createdAt, updatedAt FROM secret"
+        ).fetchall()
+
+        cursor.close()
+
+        for row in rows:
+            data = json.loads(row[2])
+
+            secret = Vault(
+                row[0],
+                row[1],
+                data["value"],
+                data["tags"],
+                row[3],
+                row[4],
+            )
+
+            result.append(secret)
+
+        return result
+
+    def insert_secret(self, secret):
+        """Insert a new row"""
+        cursor = self._connection.cursor()
+
+        result = cursor.execute(
+            "INSERT INTO secret VALUES ('{}', '{}', '{}', datetime('now'), datetime('now'))".format(
+                secret.id,
+                secret.name,
+                json.dumps(
+                    {
+                        "value": secret.value,
+                        "tags": secret.tags,
+                    }
+                ),
+            )
+        )
+
+        cursor.close()
+
+        self._connection.commit()
+
+        return result.rowcount
+
+    def delete_secret(self, name):
+        """Delete a row by secret name"""
+        cursor = self._connection.cursor()
+
+        cursor.execute("DELETE FROM secret WHERE name = ?", (name,))
+
+        cursor.close()
+
+        self._connection.commit()
```

### Comparing `opswork-0.3.0/src/opswork/module/file_system.py` & `opswork-0.4.0/src/opswork/module/file_system.py`

 * *Files identical despite different names*

### Comparing `opswork-0.3.0/src/opswork/module/logger.py` & `opswork-0.4.0/src/opswork/module/logger.py`

 * *Files identical despite different names*

### Comparing `opswork-0.3.0/src/opswork/module/output.py` & `opswork-0.4.0/src/opswork/module/output.py`

 * *Files identical despite different names*

### Comparing `opswork-0.3.0/src/opswork/module/playbook.py` & `opswork-0.4.0/src/opswork/module/playbook.py`

 * *Files identical despite different names*

### Comparing `opswork-0.3.0/src/opswork.egg-info/PKG-INFO` & `opswork-0.4.0/src/opswork.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: opswork
-Version: 0.3.0
+Version: 0.4.0
 Summary: OpsWork Swiss Knife.
-Home-page: https://github.com/clivern/opswork/
+Home-page: https://github.com/Clivern/OpsWork/
 Author: Clivern
 Author-email: hello@clivern.com
 License: MIT
-Project-URL: Documentation, https://github.com/clivern/opswork/
-Project-URL: Source, https://github.com/clivern/opswork/
-Project-URL: Changelog, https://github.com/clivern/opswork/blob/main/CHANGELOG.rst
-Project-URL: Tracker, https://github.com/clivern/opswork/issues
-Project-URL: Download, https://pypi.org/project/opswork/#files
+Project-URL: Documentation, https://github.com/Clivern/OpsWork/
+Project-URL: Source, https://github.com/Clivern/OpsWork/
+Project-URL: Changelog, https://github.com/Clivern/OpsWork/blob/main/CHANGELOG.rst
+Project-URL: Tracker, https://github.com/Clivern/OpsWork/issues
+Project-URL: Download, https://pypi.org/project/OpsWork/#files
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/x-rst; charset=UTF-8
 License-File: LICENSE.txt
```

### Comparing `opswork-0.3.0/src/opswork.egg-info/SOURCES.txt` & `opswork-0.4.0/src/opswork.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -32,22 +32,25 @@
 src/opswork.egg-info/requires.txt
 src/opswork.egg-info/top_level.txt
 src/opswork/command/__init__.py
 src/opswork/command/configs.py
 src/opswork/command/hosts.py
 src/opswork/command/random.py
 src/opswork/command/recipes.py
+src/opswork/command/secret.py
 src/opswork/exception/__init__.py
 src/opswork/model/__init__.py
 src/opswork/model/host.py
 src/opswork/model/recipe.py
+src/opswork/model/secret.py
 src/opswork/model/task.py
 src/opswork/module/__init__.py
 src/opswork/module/config.py
 src/opswork/module/database.py
+src/opswork/module/encrypt.py
 src/opswork/module/file_system.py
 src/opswork/module/logger.py
 src/opswork/module/output.py
 src/opswork/module/playbook.py
 tests/__init__.py
 tests/module/__init__.py
 tests/module/test_logger.py
```

### Comparing `opswork-0.3.0/tests/__init__.py` & `opswork-0.4.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `opswork-0.3.0/tests/module/test_logger.py` & `opswork-0.4.0/tests/module/test_logger.py`

 * *Files identical despite different names*

### Comparing `opswork-0.3.0/tox.ini` & `opswork-0.4.0/tox.ini`

 * *Files identical despite different names*

