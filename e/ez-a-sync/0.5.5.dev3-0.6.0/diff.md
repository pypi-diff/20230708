# Comparing `tmp/ez-a-sync-0.5.5.dev3.tar.gz` & `tmp/ez-a-sync-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ez-a-sync-0.5.5.dev3.tar", last modified: Thu Jul  6 00:31:13 2023, max compression
+gzip compressed data, was "ez-a-sync-0.6.0.tar", last modified: Sat Jul  8 08:33:10 2023, max compression
```

## Comparing `ez-a-sync-0.5.5.dev3.tar` & `ez-a-sync-0.6.0.tar`

### file list

```diff
@@ -1,71 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 00:31:13.783134 ez-a-sync-0.5.5.dev3/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 00:31:13.779134 ez-a-sync-0.5.5.dev3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 00:31:13.779134 ez-a-sync-0.5.5.dev3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (122)     2467 2023-07-06 00:31:03.000000 ez-a-sync-0.5.5.dev3/.github/workflows/codeql.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      575 2023-07-06 00:31:03.000000 ez-a-sync-0.5.5.dev3/.github/workflows/mypy.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      948 2023-07-06 00:31:03.000000 ez-a-sync-0.5.5.dev3/.github/workflows/pytest.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      632 2023-07-06 00:31:03.000000 ez-a-sync-0.5.5.dev3/.github/workflows/release.yaml
--rw-r--r--   0 runner    (1001) docker     (122)       84 2023-07-06 00:31:03.000000 ez-a-sync-0.5.5.dev3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)     1075 2023-07-06 00:31:03.000000 ez-a-sync-0.5.5.dev3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (122)      320 2023-07-06 00:31:13.783134 ez-a-sync-0.5.5.dev3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     6139 2023-07-06 00:31:03.000000 ez-a-sync-0.5.5.dev3/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       61 2023-07-06 00:31:03.000000 ez-a-sync-0.5.5.dev3/TODO
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 00:31:13.779134 ez-a-sync-0.5.5.dev3/a_sync/
--rw-r--r--   0 runner    (1001) docker     (122)      462 2023-07-06 00:31:03.000000 ez-a-sync-0.5.5.dev3/a_sync/ENVIRONMENT_VARIABLES.py
--rw-r--r--   0 runner    (1001) docker     (122)      566 2023-07-06 00:31:03.000000 ez-a-sync-0.5.5.dev3/a_sync/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4513 2023-07-06 00:31:03.000000 ez-a-sync-0.5.5.dev3/a_sync/_bound.py
--rw-r--r--   0 runner    (1001) docker     (122)      801 2023-07-06 00:31:03.000000 ez-a-sync-0.5.5.dev3/a_sync/_flags.py
--rw-r--r--   0 runner    (1001) docker     (122)     2082 2023-07-06 00:31:03.000000 ez-a-sync-0.5.5.dev3/a_sync/_helpers.py
--rw-r--r--   0 runner    (1001) docker     (122)      588 2023-07-06 00:31:03.000000 ez-a-sync-0.5.5.dev3/a_sync/_kwargs.py
--rw-r--r--   0 runner    (1001) docker     (122)     5343 2023-07-06 00:31:03.000000 ez-a-sync-0.5.5.dev3/a_sync/_meta.py
--rw-r--r--   0 runner    (1001) docker     (122)     1480 2023-07-06 00:31:03.000000 ez-a-sync-0.5.5.dev3/a_sync/_typing.py
--rw-r--r--   0 runner    (1001) docker     (122)     2625 2023-07-06 00:31:03.000000 ez-a-sync-0.5.5.dev3/a_sync/abstract.py
--rw-r--r--   0 runner    (1001) docker     (122)      192 2023-07-06 00:31:03.000000 ez-a-sync-0.5.5.dev3/a_sync/aliases.py
--rw-r--r--   0 runner    (1001) docker     (122)     4068 2023-07-06 00:31:03.000000 ez-a-sync-0.5.5.dev3/a_sync/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     2214 2023-07-06 00:31:03.000000 ez-a-sync-0.5.5.dev3/a_sync/config.py
--rw-r--r--   0 runner    (1001) docker     (122)     6097 2023-07-06 00:31:03.000000 ez-a-sync-0.5.5.dev3/a_sync/decorator.py
--rw-r--r--   0 runner    (1001) docker     (122)     2601 2023-07-06 00:31:03.000000 ez-a-sync-0.5.5.dev3/a_sync/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)     5019 2023-07-06 00:31:03.000000 ez-a-sync-0.5.5.dev3/a_sync/modified.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 00:31:13.783134 ez-a-sync-0.5.5.dev3/a_sync/modifiers/
--rw-r--r--   0 runner    (1001) docker     (122)     1030 2023-07-06 00:31:03.000000 ez-a-sync-0.5.5.dev3/a_sync/modifiers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 00:31:13.783134 ez-a-sync-0.5.5.dev3/a_sync/modifiers/cache/
--rw-r--r--   0 runner    (1001) docker     (122)     1795 2023-07-06 00:31:03.000000 ez-a-sync-0.5.5.dev3/a_sync/modifiers/cache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1612 2023-07-06 00:31:03.000000 ez-a-sync-0.5.5.dev3/a_sync/modifiers/cache/memory.py
--rw-r--r--   0 runner    (1001) docker     (122)     1727 2023-07-06 00:31:03.000000 ez-a-sync-0.5.5.dev3/a_sync/modifiers/limiter.py
--rw-r--r--   0 runner    (1001) docker     (122)     3473 2023-07-06 00:31:03.000000 ez-a-sync-0.5.5.dev3/a_sync/modifiers/manager.py
--rw-r--r--   0 runner    (1001) docker     (122)     2405 2023-07-06 00:31:03.000000 ez-a-sync-0.5.5.dev3/a_sync/modifiers/semaphores.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 00:31:13.783134 ez-a-sync-0.5.5.dev3/a_sync/primitives/
--rw-r--r--   0 runner    (1001) docker     (122)      500 2023-07-06 00:31:03.000000 ez-a-sync-0.5.5.dev3/a_sync/primitives/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1292 2023-07-06 00:31:03.000000 ez-a-sync-0.5.5.dev3/a_sync/primitives/_debug.py
--rw-r--r--   0 runner    (1001) docker     (122)      467 2023-07-06 00:31:03.000000 ez-a-sync-0.5.5.dev3/a_sync/primitives/_loggable.py
--rw-r--r--   0 runner    (1001) docker     (122)     7252 2023-07-06 00:31:03.000000 ez-a-sync-0.5.5.dev3/a_sync/primitives/executor.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 00:31:13.783134 ez-a-sync-0.5.5.dev3/a_sync/primitives/locks/
--rw-r--r--   0 runner    (1001) docker     (122)      198 2023-07-06 00:31:03.000000 ez-a-sync-0.5.5.dev3/a_sync/primitives/locks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2410 2023-07-06 00:31:03.000000 ez-a-sync-0.5.5.dev3/a_sync/primitives/locks/counter.py
--rw-r--r--   0 runner    (1001) docker     (122)      538 2023-07-06 00:31:03.000000 ez-a-sync-0.5.5.dev3/a_sync/primitives/locks/event.py
--rw-r--r--   0 runner    (1001) docker     (122)     3899 2023-07-06 00:31:03.000000 ez-a-sync-0.5.5.dev3/a_sync/primitives/locks/semaphore.py
--rw-r--r--   0 runner    (1001) docker     (122)     2896 2023-07-06 00:31:03.000000 ez-a-sync-0.5.5.dev3/a_sync/property.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-06 00:31:03.000000 ez-a-sync-0.5.5.dev3/a_sync/py.typed
--rw-r--r--   0 runner    (1001) docker     (122)      407 2023-07-06 00:31:03.000000 ez-a-sync-0.5.5.dev3/a_sync/singleton.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 00:31:13.783134 ez-a-sync-0.5.5.dev3/ez_a_sync.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      320 2023-07-06 00:31:13.000000 ez-a-sync-0.5.5.dev3/ez_a_sync.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1384 2023-07-06 00:31:13.000000 ez-a-sync-0.5.5.dev3/ez_a_sync.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-06 00:31:13.000000 ez-a-sync-0.5.5.dev3/ez_a_sync.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      100 2023-07-06 00:31:13.000000 ez-a-sync-0.5.5.dev3/ez_a_sync.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       13 2023-07-06 00:31:13.000000 ez-a-sync-0.5.5.dev3/ez_a_sync.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       26 2023-07-06 00:31:03.000000 ez-a-sync-0.5.5.dev3/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (122)      152 2023-07-06 00:31:03.000000 ez-a-sync-0.5.5.dev3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       79 2023-07-06 00:31:13.783134 ez-a-sync-0.5.5.dev3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)      807 2023-07-06 00:31:03.000000 ez-a-sync-0.5.5.dev3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 00:31:13.783134 ez-a-sync-0.5.5.dev3/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-06 00:31:03.000000 ez-a-sync-0.5.5.dev3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)       57 2023-07-06 00:31:03.000000 ez-a-sync-0.5.5.dev3/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (122)      239 2023-07-06 00:31:03.000000 ez-a-sync-0.5.5.dev3/tests/executor.py
--rw-r--r--   0 runner    (1001) docker     (122)     5065 2023-07-06 00:31:03.000000 ez-a-sync-0.5.5.dev3/tests/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (122)     2954 2023-07-06 00:31:03.000000 ez-a-sync-0.5.5.dev3/tests/test_base.py
--rw-r--r--   0 runner    (1001) docker     (122)     2388 2023-07-06 00:31:03.000000 ez-a-sync-0.5.5.dev3/tests/test_cache.py
--rw-r--r--   0 runner    (1001) docker     (122)     3684 2023-07-06 00:31:03.000000 ez-a-sync-0.5.5.dev3/tests/test_decorator.py
--rw-r--r--   0 runner    (1001) docker     (122)     1175 2023-07-06 00:31:03.000000 ez-a-sync-0.5.5.dev3/tests/test_executor.py
--rw-r--r--   0 runner    (1001) docker     (122)      835 2023-07-06 00:31:03.000000 ez-a-sync-0.5.5.dev3/tests/test_limiter.py
--rw-r--r--   0 runner    (1001) docker     (122)     3213 2023-07-06 00:31:03.000000 ez-a-sync-0.5.5.dev3/tests/test_meta.py
--rw-r--r--   0 runner    (1001) docker     (122)     1628 2023-07-06 00:31:03.000000 ez-a-sync-0.5.5.dev3/tests/test_semaphore.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-08 08:33:10.176240 ez-a-sync-0.6.0/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-08 08:33:10.164240 ez-a-sync-0.6.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-08 08:33:10.164240 ez-a-sync-0.6.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (122)     2467 2023-07-08 08:32:47.000000 ez-a-sync-0.6.0/.github/workflows/codeql.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      575 2023-07-08 08:32:47.000000 ez-a-sync-0.6.0/.github/workflows/mypy.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      948 2023-07-08 08:32:47.000000 ez-a-sync-0.6.0/.github/workflows/pytest.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      632 2023-07-08 08:32:47.000000 ez-a-sync-0.6.0/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)       84 2023-07-08 08:32:47.000000 ez-a-sync-0.6.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)     1075 2023-07-08 08:32:47.000000 ez-a-sync-0.6.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      315 2023-07-08 08:33:10.180240 ez-a-sync-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     6139 2023-07-08 08:32:47.000000 ez-a-sync-0.6.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       61 2023-07-08 08:32:47.000000 ez-a-sync-0.6.0/TODO
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-08 08:33:10.168240 ez-a-sync-0.6.0/a_sync/
+-rw-r--r--   0 runner    (1001) docker     (122)      462 2023-07-08 08:32:47.000000 ez-a-sync-0.6.0/a_sync/ENVIRONMENT_VARIABLES.py
+-rw-r--r--   0 runner    (1001) docker     (122)      566 2023-07-08 08:32:47.000000 ez-a-sync-0.6.0/a_sync/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4982 2023-07-08 08:32:47.000000 ez-a-sync-0.6.0/a_sync/_bound.py
+-rw-r--r--   0 runner    (1001) docker     (122)      801 2023-07-08 08:32:47.000000 ez-a-sync-0.6.0/a_sync/_flags.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2082 2023-07-08 08:32:47.000000 ez-a-sync-0.6.0/a_sync/_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (122)      588 2023-07-08 08:32:47.000000 ez-a-sync-0.6.0/a_sync/_kwargs.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5343 2023-07-08 08:32:47.000000 ez-a-sync-0.6.0/a_sync/_meta.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1480 2023-07-08 08:32:47.000000 ez-a-sync-0.6.0/a_sync/_typing.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2625 2023-07-08 08:32:47.000000 ez-a-sync-0.6.0/a_sync/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (122)      192 2023-07-08 08:32:47.000000 ez-a-sync-0.6.0/a_sync/aliases.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4068 2023-07-08 08:32:47.000000 ez-a-sync-0.6.0/a_sync/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2214 2023-07-08 08:32:47.000000 ez-a-sync-0.6.0/a_sync/config.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6133 2023-07-08 08:32:47.000000 ez-a-sync-0.6.0/a_sync/decorator.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2601 2023-07-08 08:32:47.000000 ez-a-sync-0.6.0/a_sync/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5055 2023-07-08 08:32:47.000000 ez-a-sync-0.6.0/a_sync/modified.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-08 08:33:10.168240 ez-a-sync-0.6.0/a_sync/modifiers/
+-rw-r--r--   0 runner    (1001) docker     (122)     1030 2023-07-08 08:32:47.000000 ez-a-sync-0.6.0/a_sync/modifiers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-08 08:33:10.168240 ez-a-sync-0.6.0/a_sync/modifiers/cache/
+-rw-r--r--   0 runner    (1001) docker     (122)     1831 2023-07-08 08:32:47.000000 ez-a-sync-0.6.0/a_sync/modifiers/cache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1648 2023-07-08 08:32:47.000000 ez-a-sync-0.6.0/a_sync/modifiers/cache/memory.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1763 2023-07-08 08:32:47.000000 ez-a-sync-0.6.0/a_sync/modifiers/limiter.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3483 2023-07-08 08:32:47.000000 ez-a-sync-0.6.0/a_sync/modifiers/manager.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2441 2023-07-08 08:32:47.000000 ez-a-sync-0.6.0/a_sync/modifiers/semaphores.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-08 08:33:10.172240 ez-a-sync-0.6.0/a_sync/primitives/
+-rw-r--r--   0 runner    (1001) docker     (122)      500 2023-07-08 08:32:47.000000 ez-a-sync-0.6.0/a_sync/primitives/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1292 2023-07-08 08:32:47.000000 ez-a-sync-0.6.0/a_sync/primitives/_debug.py
+-rw-r--r--   0 runner    (1001) docker     (122)      467 2023-07-08 08:32:47.000000 ez-a-sync-0.6.0/a_sync/primitives/_loggable.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7252 2023-07-08 08:32:47.000000 ez-a-sync-0.6.0/a_sync/primitives/executor.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-08 08:33:10.172240 ez-a-sync-0.6.0/a_sync/primitives/locks/
+-rw-r--r--   0 runner    (1001) docker     (122)      198 2023-07-08 08:32:47.000000 ez-a-sync-0.6.0/a_sync/primitives/locks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2410 2023-07-08 08:32:47.000000 ez-a-sync-0.6.0/a_sync/primitives/locks/counter.py
+-rw-r--r--   0 runner    (1001) docker     (122)      538 2023-07-08 08:32:47.000000 ez-a-sync-0.6.0/a_sync/primitives/locks/event.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5212 2023-07-08 08:32:47.000000 ez-a-sync-0.6.0/a_sync/primitives/locks/prio_semaphore.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3899 2023-07-08 08:32:47.000000 ez-a-sync-0.6.0/a_sync/primitives/locks/semaphore.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3060 2023-07-08 08:32:47.000000 ez-a-sync-0.6.0/a_sync/property.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-08 08:32:47.000000 ez-a-sync-0.6.0/a_sync/py.typed
+-rw-r--r--   0 runner    (1001) docker     (122)      407 2023-07-08 08:32:47.000000 ez-a-sync-0.6.0/a_sync/singleton.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-08 08:33:10.176240 ez-a-sync-0.6.0/ez_a_sync.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      315 2023-07-08 08:33:10.000000 ez-a-sync-0.6.0/ez_a_sync.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1426 2023-07-08 08:33:10.000000 ez-a-sync-0.6.0/ez_a_sync.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-08 08:33:10.000000 ez-a-sync-0.6.0/ez_a_sync.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      100 2023-07-08 08:33:10.000000 ez-a-sync-0.6.0/ez_a_sync.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       13 2023-07-08 08:33:10.000000 ez-a-sync-0.6.0/ez_a_sync.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       26 2023-07-08 08:32:47.000000 ez-a-sync-0.6.0/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      152 2023-07-08 08:32:47.000000 ez-a-sync-0.6.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       79 2023-07-08 08:33:10.180240 ez-a-sync-0.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      807 2023-07-08 08:32:47.000000 ez-a-sync-0.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-08 08:33:10.176240 ez-a-sync-0.6.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-08 08:32:47.000000 ez-a-sync-0.6.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)       57 2023-07-08 08:32:47.000000 ez-a-sync-0.6.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (122)      239 2023-07-08 08:32:47.000000 ez-a-sync-0.6.0/tests/executor.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5065 2023-07-08 08:32:47.000000 ez-a-sync-0.6.0/tests/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2954 2023-07-08 08:32:47.000000 ez-a-sync-0.6.0/tests/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2388 2023-07-08 08:32:47.000000 ez-a-sync-0.6.0/tests/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3684 2023-07-08 08:32:47.000000 ez-a-sync-0.6.0/tests/test_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1175 2023-07-08 08:32:47.000000 ez-a-sync-0.6.0/tests/test_executor.py
+-rw-r--r--   0 runner    (1001) docker     (122)      835 2023-07-08 08:32:47.000000 ez-a-sync-0.6.0/tests/test_limiter.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3213 2023-07-08 08:32:47.000000 ez-a-sync-0.6.0/tests/test_meta.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1628 2023-07-08 08:32:47.000000 ez-a-sync-0.6.0/tests/test_semaphore.py
```

### Comparing `ez-a-sync-0.5.5.dev3/.github/workflows/codeql.yaml` & `ez-a-sync-0.6.0/.github/workflows/codeql.yaml`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.5.5.dev3/.github/workflows/mypy.yaml` & `ez-a-sync-0.6.0/.github/workflows/mypy.yaml`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.5.5.dev3/.github/workflows/pytest.yaml` & `ez-a-sync-0.6.0/.github/workflows/pytest.yaml`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.5.5.dev3/.github/workflows/release.yaml` & `ez-a-sync-0.6.0/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.5.5.dev3/LICENSE.txt` & `ez-a-sync-0.6.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.5.5.dev3/README.md` & `ez-a-sync-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.5.5.dev3/a_sync/__init__.py` & `ez-a-sync-0.6.0/a_sync/__init__.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.5.5.dev3/a_sync/_bound.py` & `ez-a-sync-0.6.0/a_sync/_bound.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-# type: ignore [valid-type, misc]
+# mypy: disable-error-code=valid-type
+# mypy: disable-error-code=misc
 import functools
 from inspect import isawaitable
 
 from a_sync import _helpers
 from a_sync._typing import *
 from a_sync.decorator import a_sync as unbound_a_sync
 from a_sync.modified import ASyncFunction
@@ -52,14 +53,22 @@
             # The coroutine was already awaited due to the use of an overriding flag kwarg.
             # We can return the value.
             return retval  # type: ignore [return-value]
         # The awaitable was not awaited, so now we need to check the flag as defined on 'self' and await if appropriate.
         return _helpers._await(coro) if self.__a_sync_should_await__(kwargs, force=_force_await) else coro  # type: ignore [call-overload, return-value]
     return bound_a_sync_wrap
 
+class _PropertyGetter(Awaitable[T]):
+    def __init__(self, coro: Awaitable[T], property: Union[AsyncPropertyDescriptor[T], AsyncCachedPropertyDescriptor[T]]):
+        self._coro = coro
+        self._property = property
+    def __repr__(self) -> str:
+        return f"<_PropertyGetter for {self._property}._get at {hex(id(self))}>"
+    def __await__(self) -> T:
+        return self._coro.__await__()
 
 @overload
 def _wrap_property(
     async_property: AsyncPropertyDescriptor[T],
     **modifiers: Unpack[ModifierKwargs]
 ) -> AsyncPropertyDescriptor[T]:...
 
@@ -86,15 +95,15 @@
     async def _get(instance: ASyncABC):
         return await async_property.__get__(instance, async_property)
     
     @functools.wraps(async_property)
     def a_sync_method(self: ASyncABC, **kwargs) -> T:
         if not isinstance(self, ASyncABC):
             raise RuntimeError(f"{self} must be an instance of a class that inherits from ASyncABC.")
-        awaitable = _get(self)
+        awaitable = _PropertyGetter(_get(self), async_property)
         return _helpers._await(awaitable) if self.__a_sync_should_await__(kwargs, force=_force_await) else awaitable
     
     @property  # type: ignore [misc]
     @functools.wraps(async_property)
     def a_sync_property(self: ASyncABC) -> T:
         coro = getattr(self, async_property.hidden_method_name)(sync=False)
         return _helpers._await(coro) if self.__a_sync_should_await__({}, force=_force_await) else coro
```

### Comparing `ez-a-sync-0.5.5.dev3/a_sync/_flags.py` & `ez-a-sync-0.6.0/a_sync/_flags.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.5.5.dev3/a_sync/_helpers.py` & `ez-a-sync-0.6.0/a_sync/_helpers.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.5.5.dev3/a_sync/_kwargs.py` & `ez-a-sync-0.6.0/a_sync/_kwargs.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.5.5.dev3/a_sync/_meta.py` & `ez-a-sync-0.6.0/a_sync/_meta.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.5.5.dev3/a_sync/_typing.py` & `ez-a-sync-0.6.0/a_sync/_typing.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.5.5.dev3/a_sync/abstract.py` & `ez-a-sync-0.6.0/a_sync/abstract.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.5.5.dev3/a_sync/base.py` & `ez-a-sync-0.6.0/a_sync/base.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.5.5.dev3/a_sync/config.py` & `ez-a-sync-0.6.0/a_sync/config.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.5.5.dev3/a_sync/decorator.py` & `ez-a-sync-0.6.0/a_sync/decorator.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-# type: ignore [valid-type, misc]
+# mypy: disable-error-code=valid-type
+# mypy: disable-error-code=misc
 from a_sync import _flags, config
 from a_sync._typing import *
 from a_sync.modified import ASyncDecorator, ASyncFunction
 
 ########################
 # The a_sync decorator #
 ########################
```

### Comparing `ez-a-sync-0.5.5.dev3/a_sync/exceptions.py` & `ez-a-sync-0.6.0/a_sync/exceptions.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.5.5.dev3/a_sync/modified.py` & `ez-a-sync-0.6.0/a_sync/modified.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-# type: ignore [valid-type, misc]
+# mypy: disable-error-code=valid-type
+# mypy: disable-error-code=misc
 import functools
 import sys
 
 from a_sync import _helpers, _kwargs, exceptions
 from a_sync._typing import *
 from a_sync.modifiers.manager import ModifierManager
```

### Comparing `ez-a-sync-0.5.5.dev3/a_sync/modifiers/__init__.py` & `ez-a-sync-0.6.0/a_sync/modifiers/__init__.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.5.5.dev3/a_sync/modifiers/cache/__init__.py` & `ez-a-sync-0.6.0/a_sync/modifiers/cache/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-# type: ignore [valid-type, misc]
+# mypy: disable-error-code=valid-type
+# mypy: disable-error-code=misc
 import asyncio
 
 from a_sync import exceptions
 from a_sync._typing import *
 from a_sync.modifiers.cache.memory import apply_async_memory_cache
```

### Comparing `ez-a-sync-0.5.5.dev3/a_sync/modifiers/cache/memory.py` & `ez-a-sync-0.6.0/a_sync/modifiers/cache/memory.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-# type: ignore [valid-type, misc]
+# mypy: disable-error-code=valid-type
+# mypy: disable-error-code=misc
 import asyncio
 
 from async_lru import alru_cache
 
 from a_sync import exceptions
 from a_sync._typing import *
```

### Comparing `ez-a-sync-0.5.5.dev3/a_sync/modifiers/limiter.py` & `ez-a-sync-0.6.0/a_sync/modifiers/limiter.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-# type: ignore [valid-type, misc]
+# mypy: disable-error-code=valid-type
+# mypy: disable-error-code=misc
 import asyncio
 
 from aiolimiter import AsyncLimiter
 
 from a_sync import aliases, exceptions
 from a_sync._typing import *
```

### Comparing `ez-a-sync-0.5.5.dev3/a_sync/modifiers/manager.py` & `ez-a-sync-0.6.0/a_sync/modifiers/manager.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# type: ignore [valid-type]
+# mypy: disable-error-code=valid-type
 import functools
 
 from a_sync._typing import *
 from a_sync.config import user_set_default_modifiers, null_modifiers
 from a_sync.modifiers import cache, limiter, semaphores
 
 valid_modifiers = [key for key in ModifierKwargs.__annotations__ if not key.startswith('_') and not key.endswith('_')]
```

### Comparing `ez-a-sync-0.5.5.dev3/a_sync/modifiers/semaphores.py` & `ez-a-sync-0.6.0/a_sync/modifiers/semaphores.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-# type: ignore [valid-type, misc]
+# mypy: disable-error-code=valid-type
+# mypy: disable-error-code=misc
 import asyncio
 import functools
 
 from a_sync import exceptions, primitives
 from a_sync._typing import *
 
 # We keep this here for now so we don't break downstream deps. Eventually will be removed.
```

### Comparing `ez-a-sync-0.5.5.dev3/a_sync/primitives/_debug.py` & `ez-a-sync-0.6.0/a_sync/primitives/_debug.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.5.5.dev3/a_sync/primitives/executor.py` & `ez-a-sync-0.6.0/a_sync/primitives/executor.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.5.5.dev3/a_sync/primitives/locks/counter.py` & `ez-a-sync-0.6.0/a_sync/primitives/locks/counter.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.5.5.dev3/a_sync/primitives/locks/event.py` & `ez-a-sync-0.6.0/a_sync/primitives/locks/event.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.5.5.dev3/a_sync/primitives/locks/semaphore.py` & `ez-a-sync-0.6.0/a_sync/primitives/locks/semaphore.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.5.5.dev3/a_sync/property.py` & `ez-a-sync-0.6.0/a_sync/property.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,16 +10,19 @@
 
 
 class PropertyDescriptor(Modified[T]):
     def __init__(self, _fget: Callable[..., T], field_name=None, **modifiers: ModifierKwargs):
         if not callable(_fget):
             raise ValueError(f'Unable to decorate {_fget}')
         self.modifiers = ModifierManager(**modifiers)
+        self._fn = _fget
         _fget = self.modifiers.apply_async_modifiers(_fget) if asyncio.iscoroutinefunction(_fget) else self._asyncify(_fget)
         super().__init__(_fget, field_name=field_name)  # type: ignore [call-arg]
+    def __repr__(self) -> str:
+        return f"<{self.__class__.__module__}.{self.__class__.__name__} for {self._fn} at {hex(id(self))}>"
     
 class AsyncPropertyDescriptor(PropertyDescriptor[T], ap.base.AsyncPropertyDescriptor):
     pass
         
 class AsyncCachedPropertyDescriptor(PropertyDescriptor[T], ap.cached.AsyncCachedPropertyDescriptor):
     pass
```

### Comparing `ez-a-sync-0.5.5.dev3/ez_a_sync.egg-info/SOURCES.txt` & `ez-a-sync-0.6.0/ez_a_sync.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -37,14 +37,15 @@
 a_sync/primitives/__init__.py
 a_sync/primitives/_debug.py
 a_sync/primitives/_loggable.py
 a_sync/primitives/executor.py
 a_sync/primitives/locks/__init__.py
 a_sync/primitives/locks/counter.py
 a_sync/primitives/locks/event.py
+a_sync/primitives/locks/prio_semaphore.py
 a_sync/primitives/locks/semaphore.py
 ez_a_sync.egg-info/PKG-INFO
 ez_a_sync.egg-info/SOURCES.txt
 ez_a_sync.egg-info/dependency_links.txt
 ez_a_sync.egg-info/requires.txt
 ez_a_sync.egg-info/top_level.txt
 tests/__init__.py
```

### Comparing `ez-a-sync-0.5.5.dev3/setup.py` & `ez-a-sync-0.6.0/setup.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.5.5.dev3/tests/fixtures.py` & `ez-a-sync-0.6.0/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.5.5.dev3/tests/test_base.py` & `ez-a-sync-0.6.0/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.5.5.dev3/tests/test_cache.py` & `ez-a-sync-0.6.0/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.5.5.dev3/tests/test_decorator.py` & `ez-a-sync-0.6.0/tests/test_decorator.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.5.5.dev3/tests/test_executor.py` & `ez-a-sync-0.6.0/tests/test_executor.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.5.5.dev3/tests/test_limiter.py` & `ez-a-sync-0.6.0/tests/test_limiter.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.5.5.dev3/tests/test_meta.py` & `ez-a-sync-0.6.0/tests/test_meta.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.5.5.dev3/tests/test_semaphore.py` & `ez-a-sync-0.6.0/tests/test_semaphore.py`

 * *Files identical despite different names*

