# Comparing `tmp/fractal_repositories-0.0.4.tar.gz` & `tmp/fractal_repositories-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fractal_repositories-0.0.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "fractal_repositories-0.0.5.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `fractal_repositories-0.0.4.tar` & `fractal_repositories-0.0.5.tar`

### file list

```diff
@@ -1,71 +1,71 @@
--rw-r--r--   0        0        0      187 2023-06-27 11:43:15.526687 fractal_repositories-0.0.4/.coveragerc
--rw-r--r--   0        0        0      100 2023-06-27 11:43:15.526687 fractal_repositories-0.0.4/.flake8
--rw-r--r--   0        0        0      945 2023-06-27 11:43:15.526687 fractal_repositories-0.0.4/.github/workflows/build.yml
--rw-r--r--   0        0        0      662 2023-06-27 11:43:15.526687 fractal_repositories-0.0.4/.github/workflows/publish.yml
--rw-r--r--   0        0        0      832 2023-06-27 11:43:15.526687 fractal_repositories-0.0.4/.gitignore
--rw-r--r--   0        0        0      161 2023-06-27 11:43:15.526687 fractal_repositories-0.0.4/.isort.cfg
--rw-r--r--   0        0        0       43 2023-06-27 11:43:15.526687 fractal_repositories-0.0.4/.mypy.ini
--rw-r--r--   0        0        0     1691 2023-06-27 11:43:15.526687 fractal_repositories-0.0.4/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1075 2023-06-27 11:43:15.526687 fractal_repositories-0.0.4/LICENSE
--rw-r--r--   0        0        0     1557 2023-06-27 11:43:15.526687 fractal_repositories-0.0.4/Makefile
--rw-r--r--   0        0        0     2276 2023-06-27 11:43:15.526687 fractal_repositories-0.0.4/README.md
--rw-r--r--   0        0        0      780 2023-06-27 11:43:15.526687 fractal_repositories-0.0.4/align_version.py
--rw-r--r--   0        0        0      182 2023-06-27 11:43:15.526687 fractal_repositories-0.0.4/fractal_repositories/__init__.py
--rw-r--r--   0        0        0        0 2023-06-27 11:43:15.526687 fractal_repositories-0.0.4/fractal_repositories/contrib/__init__.py
--rw-r--r--   0        0        0        0 2023-06-27 11:43:15.526687 fractal_repositories-0.0.4/fractal_repositories/contrib/django/__init__.py
--rw-r--r--   0        0        0     3291 2023-06-27 11:43:15.526687 fractal_repositories-0.0.4/fractal_repositories/contrib/django/mixins.py
--rw-r--r--   0        0        0        0 2023-06-27 11:43:15.526687 fractal_repositories-0.0.4/fractal_repositories/contrib/elastic/__init__.py
--rw-r--r--   0        0        0        0 2023-06-27 11:43:15.526687 fractal_repositories-0.0.4/fractal_repositories/contrib/gcp/__init__.py
--rw-r--r--   0        0        0        0 2023-06-27 11:43:15.526687 fractal_repositories-0.0.4/fractal_repositories/contrib/gcp/firestore/__init__.py
--rw-r--r--   0        0        0     5318 2023-06-27 11:43:15.526687 fractal_repositories-0.0.4/fractal_repositories/contrib/gcp/firestore/mixins.py
--rw-r--r--   0        0        0        0 2023-06-27 11:43:15.526687 fractal_repositories-0.0.4/fractal_repositories/contrib/mongo/__init__.py
--rw-r--r--   0        0        0     3253 2023-06-27 11:43:15.526687 fractal_repositories-0.0.4/fractal_repositories/contrib/mongo/mixins.py
--rw-r--r--   0        0        0        0 2023-06-27 11:43:15.526687 fractal_repositories-0.0.4/fractal_repositories/contrib/sqlalchemy/__init__.py
--rw-r--r--   0        0        0    11960 2023-06-27 11:43:15.526687 fractal_repositories-0.0.4/fractal_repositories/contrib/sqlalchemy/mixins.py
--rw-r--r--   0        0        0        0 2023-06-27 11:43:15.526687 fractal_repositories-0.0.4/fractal_repositories/core/__init__.py
--rw-r--r--   0        0        0     1466 2023-06-27 11:43:15.526687 fractal_repositories-0.0.4/fractal_repositories/core/entity.py
--rw-r--r--   0        0        0     2434 2023-06-27 11:43:15.526687 fractal_repositories-0.0.4/fractal_repositories/core/repositories.py
--rw-r--r--   0        0        0      343 2023-06-27 11:43:15.526687 fractal_repositories-0.0.4/fractal_repositories/exceptions.py
--rw-r--r--   0        0        0        0 2023-06-27 11:43:15.526687 fractal_repositories-0.0.4/fractal_repositories/mixins/__init__.py
--rw-r--r--   0        0        0     1219 2023-06-27 11:43:15.526687 fractal_repositories-0.0.4/fractal_repositories/mixins/external_data_inmemory_repository_mixin.py
--rw-r--r--   0        0        0     2965 2023-06-27 11:43:15.526687 fractal_repositories-0.0.4/fractal_repositories/mixins/file_repository_mixin.py
--rw-r--r--   0        0        0      957 2023-06-27 11:43:15.526687 fractal_repositories-0.0.4/fractal_repositories/mixins/filter_repository_mixin.py
--rw-r--r--   0        0        0     3088 2023-06-27 11:43:15.526687 fractal_repositories-0.0.4/fractal_repositories/mixins/inmemory_repository_mixin.py
--rw-r--r--   0        0        0       77 2023-06-27 11:43:15.526687 fractal_repositories-0.0.4/fractal_repositories/py.typed
--rw-r--r--   0        0        0        0 2023-06-27 11:43:15.526687 fractal_repositories-0.0.4/fractal_repositories/utils/__init__.py
--rw-r--r--   0        0        0     2299 2023-06-27 11:43:15.526687 fractal_repositories-0.0.4/fractal_repositories/utils/cached_repository.py
--rw-r--r--   0        0        0     2381 2023-06-27 11:43:15.526687 fractal_repositories-0.0.4/fractal_repositories/utils/distributed_read_repository.py
--rw-r--r--   0        0        0      636 2023-06-27 11:43:15.526687 fractal_repositories-0.0.4/fractal_repositories/utils/json_encoder.py
--rw-r--r--   0        0        0      235 2023-06-27 11:43:15.526687 fractal_repositories-0.0.4/poetry.lock
--rw-r--r--   0        0        0     1667 2023-06-27 11:43:15.526687 fractal_repositories-0.0.4/pyproject.toml
--rw-r--r--   0        0        0       69 2023-06-27 11:43:15.526687 fractal_repositories-0.0.4/setup.py
--rw-r--r--   0        0        0        0 2023-06-27 11:43:15.526687 fractal_repositories-0.0.4/tests/__init__.py
--rw-r--r--   0        0        0       37 2023-06-27 11:43:15.526687 fractal_repositories-0.0.4/tests/conftest.py
--rw-r--r--   0        0        0        0 2023-06-27 11:43:15.526687 fractal_repositories-0.0.4/tests/contrib/__init__.py
--rw-r--r--   0        0        0     4177 2023-06-27 11:43:15.526687 fractal_repositories-0.0.4/tests/contrib/test_django.py
--rw-r--r--   0        0        0     4438 2023-06-27 11:43:15.526687 fractal_repositories-0.0.4/tests/contrib/test_firestore.py
--rw-r--r--   0        0        0     4100 2023-06-27 11:43:15.526687 fractal_repositories-0.0.4/tests/contrib/test_mongo.py
--rw-r--r--   0        0        0    12220 2023-06-27 11:43:15.526687 fractal_repositories-0.0.4/tests/contrib/test_sqlalchemy.py
--rw-r--r--   0        0        0        0 2023-06-27 11:43:15.526687 fractal_repositories-0.0.4/tests/core/__init__.py
--rw-r--r--   0        0        0     3168 2023-06-27 11:43:15.526687 fractal_repositories-0.0.4/tests/core/test_models.py
--rw-r--r--   0        0        0     1046 2023-06-27 11:43:15.526687 fractal_repositories-0.0.4/tests/core/test_repositories.py
--rw-r--r--   0        0        0      232 2023-06-27 11:43:15.526687 fractal_repositories-0.0.4/tests/fixtures/__init__.py
--rw-r--r--   0        0        0     2164 2023-06-27 11:43:15.526687 fractal_repositories-0.0.4/tests/fixtures/django/__init__.py
--rw-r--r--   0        0        0      643 2023-06-27 11:43:15.526687 fractal_repositories-0.0.4/tests/fixtures/django/models.py
--rw-r--r--   0        0        0     1144 2023-06-27 11:43:15.526687 fractal_repositories-0.0.4/tests/fixtures/firestore.py
--rw-r--r--   0        0        0      898 2023-06-27 11:43:15.530687 fractal_repositories-0.0.4/tests/fixtures/mongo.py
--rw-r--r--   0        0        0     6786 2023-06-27 11:43:15.530687 fractal_repositories-0.0.4/tests/fixtures/repositories.py
--rw-r--r--   0        0        0     7674 2023-06-27 11:43:15.530687 fractal_repositories-0.0.4/tests/fixtures/sqlalchemy.py
--rw-r--r--   0        0        0        0 2023-06-27 11:43:15.530687 fractal_repositories-0.0.4/tests/mixins/__init__.py
--rw-r--r--   0        0        0     1154 2023-06-27 11:43:15.530687 fractal_repositories-0.0.4/tests/mixins/test_external_data_inmemory_repository_mixin.py
--rw-r--r--   0        0        0      601 2023-06-27 11:43:15.530687 fractal_repositories-0.0.4/tests/mixins/test_file_file_repository_mixin.py
--rw-r--r--   0        0        0     3764 2023-06-27 11:43:15.530687 fractal_repositories-0.0.4/tests/mixins/test_file_repository_mixin.py
--rw-r--r--   0        0        0     3542 2023-06-27 11:43:15.530687 fractal_repositories-0.0.4/tests/mixins/test_filter_repository_mixin.py
--rw-r--r--   0        0        0      827 2023-06-27 11:43:15.530687 fractal_repositories-0.0.4/tests/mixins/test_inmemory_file_repository_mixin.py
--rw-r--r--   0        0        0     3150 2023-06-27 11:43:15.530687 fractal_repositories-0.0.4/tests/mixins/test_inmemory_repository_mixin.py
--rw-r--r--   0        0        0        0 2023-06-27 11:43:15.530687 fractal_repositories-0.0.4/tests/utils/__init__.py
--rw-r--r--   0        0        0     4025 2023-06-27 11:43:15.530687 fractal_repositories-0.0.4/tests/utils/test_cached_repository.py
--rw-r--r--   0        0        0     2381 2023-06-27 11:43:15.530687 fractal_repositories-0.0.4/tests/utils/test_distributed_read_repository.py
--rw-r--r--   0        0        0      996 2023-06-27 11:43:15.530687 fractal_repositories-0.0.4/tests/utils/test_json_encoder.py
--rw-r--r--   0        0        0      826 2023-06-27 11:43:15.530687 fractal_repositories-0.0.4/tox.ini
--rw-r--r--   0        0        0     3195 1970-01-01 00:00:00.000000 fractal_repositories-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0      187 2023-07-08 08:35:05.060040 fractal_repositories-0.0.5/.coveragerc
+-rw-r--r--   0        0        0      100 2023-07-08 08:35:05.060040 fractal_repositories-0.0.5/.flake8
+-rw-r--r--   0        0        0      945 2023-07-08 08:35:05.060040 fractal_repositories-0.0.5/.github/workflows/build.yml
+-rw-r--r--   0        0        0      662 2023-07-08 08:35:05.060040 fractal_repositories-0.0.5/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      832 2023-07-08 08:35:05.060040 fractal_repositories-0.0.5/.gitignore
+-rw-r--r--   0        0        0      161 2023-07-08 08:35:05.060040 fractal_repositories-0.0.5/.isort.cfg
+-rw-r--r--   0        0        0       43 2023-07-08 08:35:05.060040 fractal_repositories-0.0.5/.mypy.ini
+-rw-r--r--   0        0        0     1691 2023-07-08 08:35:05.060040 fractal_repositories-0.0.5/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1075 2023-07-08 08:35:05.064040 fractal_repositories-0.0.5/LICENSE
+-rw-r--r--   0        0        0     1557 2023-07-08 08:35:05.064040 fractal_repositories-0.0.5/Makefile
+-rw-r--r--   0        0        0     2276 2023-07-08 08:35:05.064040 fractal_repositories-0.0.5/README.md
+-rw-r--r--   0        0        0      780 2023-07-08 08:35:05.064040 fractal_repositories-0.0.5/align_version.py
+-rw-r--r--   0        0        0      182 2023-07-08 08:35:05.064040 fractal_repositories-0.0.5/fractal_repositories/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-08 08:35:05.064040 fractal_repositories-0.0.5/fractal_repositories/contrib/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-08 08:35:05.064040 fractal_repositories-0.0.5/fractal_repositories/contrib/django/__init__.py
+-rw-r--r--   0        0        0     3291 2023-07-08 08:35:05.064040 fractal_repositories-0.0.5/fractal_repositories/contrib/django/mixins.py
+-rw-r--r--   0        0        0        0 2023-07-08 08:35:05.064040 fractal_repositories-0.0.5/fractal_repositories/contrib/elastic/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-08 08:35:05.064040 fractal_repositories-0.0.5/fractal_repositories/contrib/gcp/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-08 08:35:05.064040 fractal_repositories-0.0.5/fractal_repositories/contrib/gcp/firestore/__init__.py
+-rw-r--r--   0        0        0     5318 2023-07-08 08:35:05.064040 fractal_repositories-0.0.5/fractal_repositories/contrib/gcp/firestore/mixins.py
+-rw-r--r--   0        0        0        0 2023-07-08 08:35:05.064040 fractal_repositories-0.0.5/fractal_repositories/contrib/mongo/__init__.py
+-rw-r--r--   0        0        0     3253 2023-07-08 08:35:05.064040 fractal_repositories-0.0.5/fractal_repositories/contrib/mongo/mixins.py
+-rw-r--r--   0        0        0        0 2023-07-08 08:35:05.064040 fractal_repositories-0.0.5/fractal_repositories/contrib/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0    11960 2023-07-08 08:35:05.064040 fractal_repositories-0.0.5/fractal_repositories/contrib/sqlalchemy/mixins.py
+-rw-r--r--   0        0        0        0 2023-07-08 08:35:05.064040 fractal_repositories-0.0.5/fractal_repositories/core/__init__.py
+-rw-r--r--   0        0        0     1680 2023-07-08 08:35:05.064040 fractal_repositories-0.0.5/fractal_repositories/core/entity.py
+-rw-r--r--   0        0        0     2434 2023-07-08 08:35:05.064040 fractal_repositories-0.0.5/fractal_repositories/core/repositories.py
+-rw-r--r--   0        0        0      343 2023-07-08 08:35:05.064040 fractal_repositories-0.0.5/fractal_repositories/exceptions.py
+-rw-r--r--   0        0        0        0 2023-07-08 08:35:05.064040 fractal_repositories-0.0.5/fractal_repositories/mixins/__init__.py
+-rw-r--r--   0        0        0     1219 2023-07-08 08:35:05.064040 fractal_repositories-0.0.5/fractal_repositories/mixins/external_data_inmemory_repository_mixin.py
+-rw-r--r--   0        0        0     2965 2023-07-08 08:35:05.064040 fractal_repositories-0.0.5/fractal_repositories/mixins/file_repository_mixin.py
+-rw-r--r--   0        0        0      957 2023-07-08 08:35:05.064040 fractal_repositories-0.0.5/fractal_repositories/mixins/filter_repository_mixin.py
+-rw-r--r--   0        0        0     3088 2023-07-08 08:35:05.064040 fractal_repositories-0.0.5/fractal_repositories/mixins/inmemory_repository_mixin.py
+-rw-r--r--   0        0        0       77 2023-07-08 08:35:05.064040 fractal_repositories-0.0.5/fractal_repositories/py.typed
+-rw-r--r--   0        0        0        0 2023-07-08 08:35:05.064040 fractal_repositories-0.0.5/fractal_repositories/utils/__init__.py
+-rw-r--r--   0        0        0     2299 2023-07-08 08:35:05.064040 fractal_repositories-0.0.5/fractal_repositories/utils/cached_repository.py
+-rw-r--r--   0        0        0     2381 2023-07-08 08:35:05.064040 fractal_repositories-0.0.5/fractal_repositories/utils/distributed_read_repository.py
+-rw-r--r--   0        0        0      636 2023-07-08 08:35:05.064040 fractal_repositories-0.0.5/fractal_repositories/utils/json_encoder.py
+-rw-r--r--   0        0        0      235 2023-07-08 08:35:05.064040 fractal_repositories-0.0.5/poetry.lock
+-rw-r--r--   0        0        0     1667 2023-07-08 08:35:05.064040 fractal_repositories-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0       69 2023-07-08 08:35:05.064040 fractal_repositories-0.0.5/setup.py
+-rw-r--r--   0        0        0        0 2023-07-08 08:35:05.064040 fractal_repositories-0.0.5/tests/__init__.py
+-rw-r--r--   0        0        0       37 2023-07-08 08:35:05.064040 fractal_repositories-0.0.5/tests/conftest.py
+-rw-r--r--   0        0        0        0 2023-07-08 08:35:05.064040 fractal_repositories-0.0.5/tests/contrib/__init__.py
+-rw-r--r--   0        0        0     4177 2023-07-08 08:35:05.064040 fractal_repositories-0.0.5/tests/contrib/test_django.py
+-rw-r--r--   0        0        0     4438 2023-07-08 08:35:05.064040 fractal_repositories-0.0.5/tests/contrib/test_firestore.py
+-rw-r--r--   0        0        0     4100 2023-07-08 08:35:05.064040 fractal_repositories-0.0.5/tests/contrib/test_mongo.py
+-rw-r--r--   0        0        0    12220 2023-07-08 08:35:05.064040 fractal_repositories-0.0.5/tests/contrib/test_sqlalchemy.py
+-rw-r--r--   0        0        0        0 2023-07-08 08:35:05.064040 fractal_repositories-0.0.5/tests/core/__init__.py
+-rw-r--r--   0        0        0     3231 2023-07-08 08:35:05.064040 fractal_repositories-0.0.5/tests/core/test_models.py
+-rw-r--r--   0        0        0     1046 2023-07-08 08:35:05.064040 fractal_repositories-0.0.5/tests/core/test_repositories.py
+-rw-r--r--   0        0        0      232 2023-07-08 08:35:05.064040 fractal_repositories-0.0.5/tests/fixtures/__init__.py
+-rw-r--r--   0        0        0     2164 2023-07-08 08:35:05.064040 fractal_repositories-0.0.5/tests/fixtures/django/__init__.py
+-rw-r--r--   0        0        0      643 2023-07-08 08:35:05.064040 fractal_repositories-0.0.5/tests/fixtures/django/models.py
+-rw-r--r--   0        0        0     1144 2023-07-08 08:35:05.064040 fractal_repositories-0.0.5/tests/fixtures/firestore.py
+-rw-r--r--   0        0        0      898 2023-07-08 08:35:05.064040 fractal_repositories-0.0.5/tests/fixtures/mongo.py
+-rw-r--r--   0        0        0     6786 2023-07-08 08:35:05.064040 fractal_repositories-0.0.5/tests/fixtures/repositories.py
+-rw-r--r--   0        0        0     7674 2023-07-08 08:35:05.064040 fractal_repositories-0.0.5/tests/fixtures/sqlalchemy.py
+-rw-r--r--   0        0        0        0 2023-07-08 08:35:05.064040 fractal_repositories-0.0.5/tests/mixins/__init__.py
+-rw-r--r--   0        0        0     1154 2023-07-08 08:35:05.064040 fractal_repositories-0.0.5/tests/mixins/test_external_data_inmemory_repository_mixin.py
+-rw-r--r--   0        0        0      601 2023-07-08 08:35:05.064040 fractal_repositories-0.0.5/tests/mixins/test_file_file_repository_mixin.py
+-rw-r--r--   0        0        0     3764 2023-07-08 08:35:05.064040 fractal_repositories-0.0.5/tests/mixins/test_file_repository_mixin.py
+-rw-r--r--   0        0        0     3542 2023-07-08 08:35:05.064040 fractal_repositories-0.0.5/tests/mixins/test_filter_repository_mixin.py
+-rw-r--r--   0        0        0      827 2023-07-08 08:35:05.064040 fractal_repositories-0.0.5/tests/mixins/test_inmemory_file_repository_mixin.py
+-rw-r--r--   0        0        0     3150 2023-07-08 08:35:05.064040 fractal_repositories-0.0.5/tests/mixins/test_inmemory_repository_mixin.py
+-rw-r--r--   0        0        0        0 2023-07-08 08:35:05.064040 fractal_repositories-0.0.5/tests/utils/__init__.py
+-rw-r--r--   0        0        0     4025 2023-07-08 08:35:05.064040 fractal_repositories-0.0.5/tests/utils/test_cached_repository.py
+-rw-r--r--   0        0        0     2381 2023-07-08 08:35:05.064040 fractal_repositories-0.0.5/tests/utils/test_distributed_read_repository.py
+-rw-r--r--   0        0        0      996 2023-07-08 08:35:05.064040 fractal_repositories-0.0.5/tests/utils/test_json_encoder.py
+-rw-r--r--   0        0        0      826 2023-07-08 08:35:05.064040 fractal_repositories-0.0.5/tox.ini
+-rw-r--r--   0        0        0     3195 1970-01-01 00:00:00.000000 fractal_repositories-0.0.5/PKG-INFO
```

### Comparing `fractal_repositories-0.0.4/.github/workflows/build.yml` & `fractal_repositories-0.0.5/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `fractal_repositories-0.0.4/.github/workflows/publish.yml` & `fractal_repositories-0.0.5/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `fractal_repositories-0.0.4/.gitignore` & `fractal_repositories-0.0.5/.gitignore`

 * *Files identical despite different names*

### Comparing `fractal_repositories-0.0.4/.pre-commit-config.yaml` & `fractal_repositories-0.0.5/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `fractal_repositories-0.0.4/LICENSE` & `fractal_repositories-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `fractal_repositories-0.0.4/Makefile` & `fractal_repositories-0.0.5/Makefile`

 * *Files identical despite different names*

### Comparing `fractal_repositories-0.0.4/README.md` & `fractal_repositories-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `fractal_repositories-0.0.4/align_version.py` & `fractal_repositories-0.0.5/align_version.py`

 * *Files identical despite different names*

### Comparing `fractal_repositories-0.0.4/fractal_repositories/contrib/django/mixins.py` & `fractal_repositories-0.0.5/fractal_repositories/contrib/django/mixins.py`

 * *Files identical despite different names*

### Comparing `fractal_repositories-0.0.4/fractal_repositories/contrib/gcp/firestore/mixins.py` & `fractal_repositories-0.0.5/fractal_repositories/contrib/gcp/firestore/mixins.py`

 * *Files identical despite different names*

### Comparing `fractal_repositories-0.0.4/fractal_repositories/contrib/mongo/mixins.py` & `fractal_repositories-0.0.5/fractal_repositories/contrib/mongo/mixins.py`

 * *Files identical despite different names*

### Comparing `fractal_repositories-0.0.4/fractal_repositories/contrib/sqlalchemy/mixins.py` & `fractal_repositories-0.0.5/fractal_repositories/contrib/sqlalchemy/mixins.py`

 * *Files identical despite different names*

### Comparing `fractal_repositories-0.0.4/fractal_repositories/core/entity.py` & `fractal_repositories-0.0.5/fractal_repositories/core/entity.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from dataclasses import dataclass, fields
-from datetime import date
+from datetime import date, datetime
 from decimal import Decimal
 from typing import Any, Dict
 
 
 @dataclass
 class Model:
     @classmethod
@@ -16,30 +16,34 @@
         return cls.clean(**data)
 
     def update(self, model: Dict):
         current = self.asdict()
         current.update(model)
         return self.from_dict(current)
 
-    def asdict(self, *, skip_types=None):
+    def asdict(self, *, skip_types=None, use_timezone_z=True):
         if skip_types is None:
             skip_types = []
         field_names = set(
             f.name for f in fields(self) if f.name not in self.calculated_fields()
         )
 
         def _asdict(v):
             if issubclass(type(v), (Model, Entity)):
-                return v.asdict(skip_types=skip_types)
+                return v.asdict(skip_types=skip_types, use_timezone_z=use_timezone_z)
             elif isinstance(v, list) and list not in skip_types:
                 return [_asdict(i) for i in v]
             elif isinstance(v, Decimal) and Decimal not in skip_types:
                 return f"{v:.2f}"
-            elif isinstance(v, date) and date not in skip_types:
-                return v.isoformat()
+            elif isinstance(v, (date, datetime)) and date not in skip_types:
+                return (
+                    v.isoformat().replace("+00:00", "Z")
+                    if use_timezone_z
+                    else v.isoformat()
+                )
             return v
 
         ret = {k: _asdict(v) for k, v in self.__dict__.items() if k in field_names}
         return ret
 
     @staticmethod
     def calculated_fields():
```

### Comparing `fractal_repositories-0.0.4/fractal_repositories/core/repositories.py` & `fractal_repositories-0.0.5/fractal_repositories/core/repositories.py`

 * *Files identical despite different names*

### Comparing `fractal_repositories-0.0.4/fractal_repositories/mixins/external_data_inmemory_repository_mixin.py` & `fractal_repositories-0.0.5/fractal_repositories/mixins/external_data_inmemory_repository_mixin.py`

 * *Files identical despite different names*

### Comparing `fractal_repositories-0.0.4/fractal_repositories/mixins/file_repository_mixin.py` & `fractal_repositories-0.0.5/fractal_repositories/mixins/file_repository_mixin.py`

 * *Files identical despite different names*

### Comparing `fractal_repositories-0.0.4/fractal_repositories/mixins/filter_repository_mixin.py` & `fractal_repositories-0.0.5/fractal_repositories/mixins/filter_repository_mixin.py`

 * *Files identical despite different names*

### Comparing `fractal_repositories-0.0.4/fractal_repositories/mixins/inmemory_repository_mixin.py` & `fractal_repositories-0.0.5/fractal_repositories/mixins/inmemory_repository_mixin.py`

 * *Files identical despite different names*

### Comparing `fractal_repositories-0.0.4/fractal_repositories/utils/cached_repository.py` & `fractal_repositories-0.0.5/fractal_repositories/utils/cached_repository.py`

 * *Files identical despite different names*

### Comparing `fractal_repositories-0.0.4/fractal_repositories/utils/distributed_read_repository.py` & `fractal_repositories-0.0.5/fractal_repositories/utils/distributed_read_repository.py`

 * *Files identical despite different names*

### Comparing `fractal_repositories-0.0.4/fractal_repositories/utils/json_encoder.py` & `fractal_repositories-0.0.5/fractal_repositories/utils/json_encoder.py`

 * *Files identical despite different names*

### Comparing `fractal_repositories-0.0.4/pyproject.toml` & `fractal_repositories-0.0.5/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fractal-repositories"
-version = "0.0.4"
+version = "0.0.5"
 description = "Fractal Repositories is an implementation of the repository pattern for building SOLID logic for your Python applications."
 authors = ["Douwe van der Meij <douwe@karibu-online.nl>"]
 
 [build-system]
 requires = ["flit_core >=2,<4"]
 build-backend = "flit_core.buildapi"
```

### Comparing `fractal_repositories-0.0.4/tests/contrib/test_django.py` & `fractal_repositories-0.0.5/tests/contrib/test_django.py`

 * *Files identical despite different names*

### Comparing `fractal_repositories-0.0.4/tests/contrib/test_firestore.py` & `fractal_repositories-0.0.5/tests/contrib/test_firestore.py`

 * *Files identical despite different names*

### Comparing `fractal_repositories-0.0.4/tests/contrib/test_mongo.py` & `fractal_repositories-0.0.5/tests/contrib/test_mongo.py`

 * *Files identical despite different names*

### Comparing `fractal_repositories-0.0.4/tests/contrib/test_sqlalchemy.py` & `fractal_repositories-0.0.5/tests/contrib/test_sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `fractal_repositories-0.0.4/tests/core/test_models.py` & `fractal_repositories-0.0.5/tests/core/test_models.py`

 * *Files 4% similar despite different names*

```diff
@@ -49,15 +49,15 @@
             if not self.nested_list:
                 self.nested_list = [model_instance]
 
     return M(id="1")
 
 
 def test_model(model_instance, now, decimal):
-    assert model_instance.asdict() == {
+    assert model_instance.asdict(use_timezone_z=False) == {
         "id": "1",
         "string": "name",
         "number": 1,
         "string_list": ["a", "b"],
         "now": now.isoformat(),
         "decimal_number": f"{decimal:.2f}",
     }
@@ -68,15 +68,15 @@
         "id": "1",
         "string": "new_name",
         "number": 2,
         "string_list": ["c", "d"],
     }
     assert model_instance.update(some_new_values).asdict() == {
         **some_new_values,
-        "now": now.isoformat(),
+        "now": now.isoformat().replace("+00:00", "Z"),
         "decimal_number": f"{decimal:.2f}",
     }
 
 
 def test_model_skip_types(model_instance, now, decimal):
     assert model_instance.asdict(skip_types=(list, date, Decimal,)) == {
         "id": "1",
@@ -85,15 +85,15 @@
         "string_list": ["a", "b"],
         "now": now,
         "decimal_number": decimal,
     }
 
 
 def test_model_nested(nested_model_instance, now, decimal):
-    assert nested_model_instance.asdict() == {
+    assert nested_model_instance.asdict(use_timezone_z=False) == {
         "id": "1",
         "nested_list": [
             {
                 "id": "1",
                 "string": "name",
                 "number": 1,
                 "string_list": ["a", "b"],
```

### Comparing `fractal_repositories-0.0.4/tests/core/test_repositories.py` & `fractal_repositories-0.0.5/tests/core/test_repositories.py`

 * *Files identical despite different names*

### Comparing `fractal_repositories-0.0.4/tests/fixtures/django/__init__.py` & `fractal_repositories-0.0.5/tests/fixtures/django/__init__.py`

 * *Files identical despite different names*

### Comparing `fractal_repositories-0.0.4/tests/fixtures/django/models.py` & `fractal_repositories-0.0.5/tests/fixtures/django/models.py`

 * *Files identical despite different names*

### Comparing `fractal_repositories-0.0.4/tests/fixtures/firestore.py` & `fractal_repositories-0.0.5/tests/fixtures/firestore.py`

 * *Files identical despite different names*

### Comparing `fractal_repositories-0.0.4/tests/fixtures/mongo.py` & `fractal_repositories-0.0.5/tests/fixtures/mongo.py`

 * *Files identical despite different names*

### Comparing `fractal_repositories-0.0.4/tests/fixtures/repositories.py` & `fractal_repositories-0.0.5/tests/fixtures/repositories.py`

 * *Files identical despite different names*

### Comparing `fractal_repositories-0.0.4/tests/fixtures/sqlalchemy.py` & `fractal_repositories-0.0.5/tests/fixtures/sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `fractal_repositories-0.0.4/tests/mixins/test_external_data_inmemory_repository_mixin.py` & `fractal_repositories-0.0.5/tests/mixins/test_external_data_inmemory_repository_mixin.py`

 * *Files identical despite different names*

### Comparing `fractal_repositories-0.0.4/tests/mixins/test_file_file_repository_mixin.py` & `fractal_repositories-0.0.5/tests/mixins/test_file_file_repository_mixin.py`

 * *Files identical despite different names*

### Comparing `fractal_repositories-0.0.4/tests/mixins/test_file_repository_mixin.py` & `fractal_repositories-0.0.5/tests/mixins/test_file_repository_mixin.py`

 * *Files identical despite different names*

### Comparing `fractal_repositories-0.0.4/tests/mixins/test_filter_repository_mixin.py` & `fractal_repositories-0.0.5/tests/mixins/test_filter_repository_mixin.py`

 * *Files identical despite different names*

### Comparing `fractal_repositories-0.0.4/tests/mixins/test_inmemory_file_repository_mixin.py` & `fractal_repositories-0.0.5/tests/mixins/test_inmemory_file_repository_mixin.py`

 * *Files identical despite different names*

### Comparing `fractal_repositories-0.0.4/tests/mixins/test_inmemory_repository_mixin.py` & `fractal_repositories-0.0.5/tests/mixins/test_inmemory_repository_mixin.py`

 * *Files identical despite different names*

### Comparing `fractal_repositories-0.0.4/tests/utils/test_cached_repository.py` & `fractal_repositories-0.0.5/tests/utils/test_cached_repository.py`

 * *Files identical despite different names*

### Comparing `fractal_repositories-0.0.4/tests/utils/test_distributed_read_repository.py` & `fractal_repositories-0.0.5/tests/utils/test_distributed_read_repository.py`

 * *Files identical despite different names*

### Comparing `fractal_repositories-0.0.4/tests/utils/test_json_encoder.py` & `fractal_repositories-0.0.5/tests/utils/test_json_encoder.py`

 * *Files identical despite different names*

### Comparing `fractal_repositories-0.0.4/tox.ini` & `fractal_repositories-0.0.5/tox.ini`

 * *Files identical despite different names*

### Comparing `fractal_repositories-0.0.4/PKG-INFO` & `fractal_repositories-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fractal-repositories
-Version: 0.0.4
+Version: 0.0.5
 Summary: Fractal Repositories is an implementation of the repository pattern of Domain Driven Design (DDD) for building SOLID logic for your Python applications.
 Home-page: https://github.com/douwevandermeij/fractal-repositories
 Author: Douwe van der Meij
 Author-email: douwe@karibu-online.nl
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
```

