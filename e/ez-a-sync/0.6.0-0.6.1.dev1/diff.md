# Comparing `tmp/ez-a-sync-0.6.0.tar.gz` & `tmp/ez-a-sync-0.6.1.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ez-a-sync-0.6.0.tar", last modified: Sat Jul  8 08:33:10 2023, max compression
+gzip compressed data, was "ez-a-sync-0.6.1.dev1.tar", last modified: Sat Jul  8 09:14:35 2023, max compression
```

## Comparing `ez-a-sync-0.6.0.tar` & `ez-a-sync-0.6.1.dev1.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-08 08:33:10.176240 ez-a-sync-0.6.0/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-08 08:33:10.164240 ez-a-sync-0.6.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-08 08:33:10.164240 ez-a-sync-0.6.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (122)     2467 2023-07-08 08:32:47.000000 ez-a-sync-0.6.0/.github/workflows/codeql.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      575 2023-07-08 08:32:47.000000 ez-a-sync-0.6.0/.github/workflows/mypy.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      948 2023-07-08 08:32:47.000000 ez-a-sync-0.6.0/.github/workflows/pytest.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      632 2023-07-08 08:32:47.000000 ez-a-sync-0.6.0/.github/workflows/release.yaml
--rw-r--r--   0 runner    (1001) docker     (122)       84 2023-07-08 08:32:47.000000 ez-a-sync-0.6.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)     1075 2023-07-08 08:32:47.000000 ez-a-sync-0.6.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (122)      315 2023-07-08 08:33:10.180240 ez-a-sync-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     6139 2023-07-08 08:32:47.000000 ez-a-sync-0.6.0/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       61 2023-07-08 08:32:47.000000 ez-a-sync-0.6.0/TODO
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-08 08:33:10.168240 ez-a-sync-0.6.0/a_sync/
--rw-r--r--   0 runner    (1001) docker     (122)      462 2023-07-08 08:32:47.000000 ez-a-sync-0.6.0/a_sync/ENVIRONMENT_VARIABLES.py
--rw-r--r--   0 runner    (1001) docker     (122)      566 2023-07-08 08:32:47.000000 ez-a-sync-0.6.0/a_sync/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4982 2023-07-08 08:32:47.000000 ez-a-sync-0.6.0/a_sync/_bound.py
--rw-r--r--   0 runner    (1001) docker     (122)      801 2023-07-08 08:32:47.000000 ez-a-sync-0.6.0/a_sync/_flags.py
--rw-r--r--   0 runner    (1001) docker     (122)     2082 2023-07-08 08:32:47.000000 ez-a-sync-0.6.0/a_sync/_helpers.py
--rw-r--r--   0 runner    (1001) docker     (122)      588 2023-07-08 08:32:47.000000 ez-a-sync-0.6.0/a_sync/_kwargs.py
--rw-r--r--   0 runner    (1001) docker     (122)     5343 2023-07-08 08:32:47.000000 ez-a-sync-0.6.0/a_sync/_meta.py
--rw-r--r--   0 runner    (1001) docker     (122)     1480 2023-07-08 08:32:47.000000 ez-a-sync-0.6.0/a_sync/_typing.py
--rw-r--r--   0 runner    (1001) docker     (122)     2625 2023-07-08 08:32:47.000000 ez-a-sync-0.6.0/a_sync/abstract.py
--rw-r--r--   0 runner    (1001) docker     (122)      192 2023-07-08 08:32:47.000000 ez-a-sync-0.6.0/a_sync/aliases.py
--rw-r--r--   0 runner    (1001) docker     (122)     4068 2023-07-08 08:32:47.000000 ez-a-sync-0.6.0/a_sync/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     2214 2023-07-08 08:32:47.000000 ez-a-sync-0.6.0/a_sync/config.py
--rw-r--r--   0 runner    (1001) docker     (122)     6133 2023-07-08 08:32:47.000000 ez-a-sync-0.6.0/a_sync/decorator.py
--rw-r--r--   0 runner    (1001) docker     (122)     2601 2023-07-08 08:32:47.000000 ez-a-sync-0.6.0/a_sync/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)     5055 2023-07-08 08:32:47.000000 ez-a-sync-0.6.0/a_sync/modified.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-08 08:33:10.168240 ez-a-sync-0.6.0/a_sync/modifiers/
--rw-r--r--   0 runner    (1001) docker     (122)     1030 2023-07-08 08:32:47.000000 ez-a-sync-0.6.0/a_sync/modifiers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-08 08:33:10.168240 ez-a-sync-0.6.0/a_sync/modifiers/cache/
--rw-r--r--   0 runner    (1001) docker     (122)     1831 2023-07-08 08:32:47.000000 ez-a-sync-0.6.0/a_sync/modifiers/cache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1648 2023-07-08 08:32:47.000000 ez-a-sync-0.6.0/a_sync/modifiers/cache/memory.py
--rw-r--r--   0 runner    (1001) docker     (122)     1763 2023-07-08 08:32:47.000000 ez-a-sync-0.6.0/a_sync/modifiers/limiter.py
--rw-r--r--   0 runner    (1001) docker     (122)     3483 2023-07-08 08:32:47.000000 ez-a-sync-0.6.0/a_sync/modifiers/manager.py
--rw-r--r--   0 runner    (1001) docker     (122)     2441 2023-07-08 08:32:47.000000 ez-a-sync-0.6.0/a_sync/modifiers/semaphores.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-08 08:33:10.172240 ez-a-sync-0.6.0/a_sync/primitives/
--rw-r--r--   0 runner    (1001) docker     (122)      500 2023-07-08 08:32:47.000000 ez-a-sync-0.6.0/a_sync/primitives/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1292 2023-07-08 08:32:47.000000 ez-a-sync-0.6.0/a_sync/primitives/_debug.py
--rw-r--r--   0 runner    (1001) docker     (122)      467 2023-07-08 08:32:47.000000 ez-a-sync-0.6.0/a_sync/primitives/_loggable.py
--rw-r--r--   0 runner    (1001) docker     (122)     7252 2023-07-08 08:32:47.000000 ez-a-sync-0.6.0/a_sync/primitives/executor.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-08 08:33:10.172240 ez-a-sync-0.6.0/a_sync/primitives/locks/
--rw-r--r--   0 runner    (1001) docker     (122)      198 2023-07-08 08:32:47.000000 ez-a-sync-0.6.0/a_sync/primitives/locks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2410 2023-07-08 08:32:47.000000 ez-a-sync-0.6.0/a_sync/primitives/locks/counter.py
--rw-r--r--   0 runner    (1001) docker     (122)      538 2023-07-08 08:32:47.000000 ez-a-sync-0.6.0/a_sync/primitives/locks/event.py
--rw-r--r--   0 runner    (1001) docker     (122)     5212 2023-07-08 08:32:47.000000 ez-a-sync-0.6.0/a_sync/primitives/locks/prio_semaphore.py
--rw-r--r--   0 runner    (1001) docker     (122)     3899 2023-07-08 08:32:47.000000 ez-a-sync-0.6.0/a_sync/primitives/locks/semaphore.py
--rw-r--r--   0 runner    (1001) docker     (122)     3060 2023-07-08 08:32:47.000000 ez-a-sync-0.6.0/a_sync/property.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-08 08:32:47.000000 ez-a-sync-0.6.0/a_sync/py.typed
--rw-r--r--   0 runner    (1001) docker     (122)      407 2023-07-08 08:32:47.000000 ez-a-sync-0.6.0/a_sync/singleton.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-08 08:33:10.176240 ez-a-sync-0.6.0/ez_a_sync.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      315 2023-07-08 08:33:10.000000 ez-a-sync-0.6.0/ez_a_sync.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1426 2023-07-08 08:33:10.000000 ez-a-sync-0.6.0/ez_a_sync.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-08 08:33:10.000000 ez-a-sync-0.6.0/ez_a_sync.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      100 2023-07-08 08:33:10.000000 ez-a-sync-0.6.0/ez_a_sync.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       13 2023-07-08 08:33:10.000000 ez-a-sync-0.6.0/ez_a_sync.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       26 2023-07-08 08:32:47.000000 ez-a-sync-0.6.0/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (122)      152 2023-07-08 08:32:47.000000 ez-a-sync-0.6.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       79 2023-07-08 08:33:10.180240 ez-a-sync-0.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)      807 2023-07-08 08:32:47.000000 ez-a-sync-0.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-08 08:33:10.176240 ez-a-sync-0.6.0/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-08 08:32:47.000000 ez-a-sync-0.6.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)       57 2023-07-08 08:32:47.000000 ez-a-sync-0.6.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (122)      239 2023-07-08 08:32:47.000000 ez-a-sync-0.6.0/tests/executor.py
--rw-r--r--   0 runner    (1001) docker     (122)     5065 2023-07-08 08:32:47.000000 ez-a-sync-0.6.0/tests/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (122)     2954 2023-07-08 08:32:47.000000 ez-a-sync-0.6.0/tests/test_base.py
--rw-r--r--   0 runner    (1001) docker     (122)     2388 2023-07-08 08:32:47.000000 ez-a-sync-0.6.0/tests/test_cache.py
--rw-r--r--   0 runner    (1001) docker     (122)     3684 2023-07-08 08:32:47.000000 ez-a-sync-0.6.0/tests/test_decorator.py
--rw-r--r--   0 runner    (1001) docker     (122)     1175 2023-07-08 08:32:47.000000 ez-a-sync-0.6.0/tests/test_executor.py
--rw-r--r--   0 runner    (1001) docker     (122)      835 2023-07-08 08:32:47.000000 ez-a-sync-0.6.0/tests/test_limiter.py
--rw-r--r--   0 runner    (1001) docker     (122)     3213 2023-07-08 08:32:47.000000 ez-a-sync-0.6.0/tests/test_meta.py
--rw-r--r--   0 runner    (1001) docker     (122)     1628 2023-07-08 08:32:47.000000 ez-a-sync-0.6.0/tests/test_semaphore.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-08 09:14:35.368591 ez-a-sync-0.6.1.dev1/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-08 09:14:35.352595 ez-a-sync-0.6.1.dev1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-08 09:14:35.356594 ez-a-sync-0.6.1.dev1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (122)     2467 2023-07-08 09:14:20.000000 ez-a-sync-0.6.1.dev1/.github/workflows/codeql.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      575 2023-07-08 09:14:20.000000 ez-a-sync-0.6.1.dev1/.github/workflows/mypy.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      948 2023-07-08 09:14:20.000000 ez-a-sync-0.6.1.dev1/.github/workflows/pytest.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      632 2023-07-08 09:14:20.000000 ez-a-sync-0.6.1.dev1/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)       84 2023-07-08 09:14:20.000000 ez-a-sync-0.6.1.dev1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)     1075 2023-07-08 09:14:20.000000 ez-a-sync-0.6.1.dev1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      320 2023-07-08 09:14:35.368591 ez-a-sync-0.6.1.dev1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     6139 2023-07-08 09:14:20.000000 ez-a-sync-0.6.1.dev1/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       61 2023-07-08 09:14:20.000000 ez-a-sync-0.6.1.dev1/TODO
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-08 09:14:35.360593 ez-a-sync-0.6.1.dev1/a_sync/
+-rw-r--r--   0 runner    (1001) docker     (122)      462 2023-07-08 09:14:20.000000 ez-a-sync-0.6.1.dev1/a_sync/ENVIRONMENT_VARIABLES.py
+-rw-r--r--   0 runner    (1001) docker     (122)      566 2023-07-08 09:14:20.000000 ez-a-sync-0.6.1.dev1/a_sync/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4982 2023-07-08 09:14:20.000000 ez-a-sync-0.6.1.dev1/a_sync/_bound.py
+-rw-r--r--   0 runner    (1001) docker     (122)      801 2023-07-08 09:14:20.000000 ez-a-sync-0.6.1.dev1/a_sync/_flags.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2082 2023-07-08 09:14:20.000000 ez-a-sync-0.6.1.dev1/a_sync/_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (122)      588 2023-07-08 09:14:20.000000 ez-a-sync-0.6.1.dev1/a_sync/_kwargs.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5343 2023-07-08 09:14:20.000000 ez-a-sync-0.6.1.dev1/a_sync/_meta.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1480 2023-07-08 09:14:20.000000 ez-a-sync-0.6.1.dev1/a_sync/_typing.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2625 2023-07-08 09:14:20.000000 ez-a-sync-0.6.1.dev1/a_sync/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (122)      192 2023-07-08 09:14:20.000000 ez-a-sync-0.6.1.dev1/a_sync/aliases.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4068 2023-07-08 09:14:20.000000 ez-a-sync-0.6.1.dev1/a_sync/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2214 2023-07-08 09:14:20.000000 ez-a-sync-0.6.1.dev1/a_sync/config.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6133 2023-07-08 09:14:20.000000 ez-a-sync-0.6.1.dev1/a_sync/decorator.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2601 2023-07-08 09:14:20.000000 ez-a-sync-0.6.1.dev1/a_sync/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5055 2023-07-08 09:14:20.000000 ez-a-sync-0.6.1.dev1/a_sync/modified.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-08 09:14:35.360593 ez-a-sync-0.6.1.dev1/a_sync/modifiers/
+-rw-r--r--   0 runner    (1001) docker     (122)     1030 2023-07-08 09:14:20.000000 ez-a-sync-0.6.1.dev1/a_sync/modifiers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-08 09:14:35.360593 ez-a-sync-0.6.1.dev1/a_sync/modifiers/cache/
+-rw-r--r--   0 runner    (1001) docker     (122)     1831 2023-07-08 09:14:20.000000 ez-a-sync-0.6.1.dev1/a_sync/modifiers/cache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1648 2023-07-08 09:14:20.000000 ez-a-sync-0.6.1.dev1/a_sync/modifiers/cache/memory.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1763 2023-07-08 09:14:20.000000 ez-a-sync-0.6.1.dev1/a_sync/modifiers/limiter.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3483 2023-07-08 09:14:20.000000 ez-a-sync-0.6.1.dev1/a_sync/modifiers/manager.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2441 2023-07-08 09:14:20.000000 ez-a-sync-0.6.1.dev1/a_sync/modifiers/semaphores.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-08 09:14:35.364592 ez-a-sync-0.6.1.dev1/a_sync/primitives/
+-rw-r--r--   0 runner    (1001) docker     (122)      500 2023-07-08 09:14:20.000000 ez-a-sync-0.6.1.dev1/a_sync/primitives/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1292 2023-07-08 09:14:20.000000 ez-a-sync-0.6.1.dev1/a_sync/primitives/_debug.py
+-rw-r--r--   0 runner    (1001) docker     (122)      467 2023-07-08 09:14:20.000000 ez-a-sync-0.6.1.dev1/a_sync/primitives/_loggable.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7252 2023-07-08 09:14:20.000000 ez-a-sync-0.6.1.dev1/a_sync/primitives/executor.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-08 09:14:35.364592 ez-a-sync-0.6.1.dev1/a_sync/primitives/locks/
+-rw-r--r--   0 runner    (1001) docker     (122)      198 2023-07-08 09:14:20.000000 ez-a-sync-0.6.1.dev1/a_sync/primitives/locks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2410 2023-07-08 09:14:20.000000 ez-a-sync-0.6.1.dev1/a_sync/primitives/locks/counter.py
+-rw-r--r--   0 runner    (1001) docker     (122)      538 2023-07-08 09:14:20.000000 ez-a-sync-0.6.1.dev1/a_sync/primitives/locks/event.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5182 2023-07-08 09:14:20.000000 ez-a-sync-0.6.1.dev1/a_sync/primitives/locks/prio_semaphore.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3923 2023-07-08 09:14:20.000000 ez-a-sync-0.6.1.dev1/a_sync/primitives/locks/semaphore.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3060 2023-07-08 09:14:20.000000 ez-a-sync-0.6.1.dev1/a_sync/property.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-08 09:14:20.000000 ez-a-sync-0.6.1.dev1/a_sync/py.typed
+-rw-r--r--   0 runner    (1001) docker     (122)      407 2023-07-08 09:14:20.000000 ez-a-sync-0.6.1.dev1/a_sync/singleton.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-08 09:14:35.364592 ez-a-sync-0.6.1.dev1/ez_a_sync.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      320 2023-07-08 09:14:35.000000 ez-a-sync-0.6.1.dev1/ez_a_sync.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1426 2023-07-08 09:14:35.000000 ez-a-sync-0.6.1.dev1/ez_a_sync.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-08 09:14:35.000000 ez-a-sync-0.6.1.dev1/ez_a_sync.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      100 2023-07-08 09:14:35.000000 ez-a-sync-0.6.1.dev1/ez_a_sync.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       13 2023-07-08 09:14:35.000000 ez-a-sync-0.6.1.dev1/ez_a_sync.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       26 2023-07-08 09:14:20.000000 ez-a-sync-0.6.1.dev1/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      152 2023-07-08 09:14:20.000000 ez-a-sync-0.6.1.dev1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       79 2023-07-08 09:14:35.368591 ez-a-sync-0.6.1.dev1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      807 2023-07-08 09:14:20.000000 ez-a-sync-0.6.1.dev1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-08 09:14:35.368591 ez-a-sync-0.6.1.dev1/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-08 09:14:20.000000 ez-a-sync-0.6.1.dev1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)       57 2023-07-08 09:14:20.000000 ez-a-sync-0.6.1.dev1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (122)      239 2023-07-08 09:14:20.000000 ez-a-sync-0.6.1.dev1/tests/executor.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5065 2023-07-08 09:14:20.000000 ez-a-sync-0.6.1.dev1/tests/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2954 2023-07-08 09:14:20.000000 ez-a-sync-0.6.1.dev1/tests/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2388 2023-07-08 09:14:20.000000 ez-a-sync-0.6.1.dev1/tests/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3684 2023-07-08 09:14:20.000000 ez-a-sync-0.6.1.dev1/tests/test_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1175 2023-07-08 09:14:20.000000 ez-a-sync-0.6.1.dev1/tests/test_executor.py
+-rw-r--r--   0 runner    (1001) docker     (122)      835 2023-07-08 09:14:20.000000 ez-a-sync-0.6.1.dev1/tests/test_limiter.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3213 2023-07-08 09:14:20.000000 ez-a-sync-0.6.1.dev1/tests/test_meta.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1628 2023-07-08 09:14:20.000000 ez-a-sync-0.6.1.dev1/tests/test_semaphore.py
```

### Comparing `ez-a-sync-0.6.0/.github/workflows/codeql.yaml` & `ez-a-sync-0.6.1.dev1/.github/workflows/codeql.yaml`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.6.0/.github/workflows/mypy.yaml` & `ez-a-sync-0.6.1.dev1/.github/workflows/mypy.yaml`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.6.0/.github/workflows/pytest.yaml` & `ez-a-sync-0.6.1.dev1/.github/workflows/pytest.yaml`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.6.0/.github/workflows/release.yaml` & `ez-a-sync-0.6.1.dev1/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.6.0/LICENSE.txt` & `ez-a-sync-0.6.1.dev1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.6.0/README.md` & `ez-a-sync-0.6.1.dev1/README.md`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.6.0/a_sync/__init__.py` & `ez-a-sync-0.6.1.dev1/a_sync/__init__.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.6.0/a_sync/_bound.py` & `ez-a-sync-0.6.1.dev1/a_sync/_bound.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.6.0/a_sync/_flags.py` & `ez-a-sync-0.6.1.dev1/a_sync/_flags.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.6.0/a_sync/_helpers.py` & `ez-a-sync-0.6.1.dev1/a_sync/_helpers.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.6.0/a_sync/_kwargs.py` & `ez-a-sync-0.6.1.dev1/a_sync/_kwargs.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.6.0/a_sync/_meta.py` & `ez-a-sync-0.6.1.dev1/a_sync/_meta.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.6.0/a_sync/_typing.py` & `ez-a-sync-0.6.1.dev1/a_sync/_typing.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.6.0/a_sync/abstract.py` & `ez-a-sync-0.6.1.dev1/a_sync/abstract.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.6.0/a_sync/base.py` & `ez-a-sync-0.6.1.dev1/a_sync/base.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.6.0/a_sync/config.py` & `ez-a-sync-0.6.1.dev1/a_sync/config.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.6.0/a_sync/decorator.py` & `ez-a-sync-0.6.1.dev1/a_sync/decorator.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.6.0/a_sync/exceptions.py` & `ez-a-sync-0.6.1.dev1/a_sync/exceptions.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.6.0/a_sync/modified.py` & `ez-a-sync-0.6.1.dev1/a_sync/modified.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.6.0/a_sync/modifiers/__init__.py` & `ez-a-sync-0.6.1.dev1/a_sync/modifiers/__init__.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.6.0/a_sync/modifiers/cache/__init__.py` & `ez-a-sync-0.6.1.dev1/a_sync/modifiers/cache/__init__.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.6.0/a_sync/modifiers/cache/memory.py` & `ez-a-sync-0.6.1.dev1/a_sync/modifiers/cache/memory.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.6.0/a_sync/modifiers/limiter.py` & `ez-a-sync-0.6.1.dev1/a_sync/modifiers/limiter.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.6.0/a_sync/modifiers/manager.py` & `ez-a-sync-0.6.1.dev1/a_sync/modifiers/manager.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.6.0/a_sync/modifiers/semaphores.py` & `ez-a-sync-0.6.1.dev1/a_sync/modifiers/semaphores.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.6.0/a_sync/primitives/_debug.py` & `ez-a-sync-0.6.1.dev1/a_sync/primitives/_debug.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.6.0/a_sync/primitives/executor.py` & `ez-a-sync-0.6.1.dev1/a_sync/primitives/executor.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.6.0/a_sync/primitives/locks/counter.py` & `ez-a-sync-0.6.1.dev1/a_sync/primitives/locks/counter.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.6.0/a_sync/primitives/locks/event.py` & `ez-a-sync-0.6.1.dev1/a_sync/primitives/locks/event.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.6.0/a_sync/primitives/locks/prio_semaphore.py` & `ez-a-sync-0.6.1.dev1/a_sync/primitives/locks/prio_semaphore.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 
 import asyncio
 import heapq
 from typing import (Dict, Generic, List, Literal, Optional, Protocol, Type,
                     TypeVar)
 
 from a_sync import Semaphore
-from hexbytes import HexBytes
 
 
 T = TypeVar('T', covariant=True)
 
 class Priority(Protocol):
     def __lt__(self, other) -> bool:
         ...
```

### Comparing `ez-a-sync-0.6.0/a_sync/primitives/locks/semaphore.py` & `ez-a-sync-0.6.1.dev1/a_sync/primitives/locks/semaphore.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     def __repr__(self) -> str:
         representation = f"<{self.__class__.__name__} name={self.name} value={self._value} waiters={len(self)}>"
         if self._decorated:
             representation = f"{representation[:-1]} decorates={self._decorated}"
         return representation
     
     def __len__(self) -> int:
-        return len(self._waiters)
+        return len(self._waiters) if self._waiters else 0
     
     def decorate(self, fn: Callable[P, T]) -> Callable[P, T]:
         if not asyncio.iscoroutinefunction(fn):
             raise TypeError(f"{fn} must be a coroutine function")
         @functools.wraps(fn)
         async def semaphore_wrapper(*args: P.args, **kwargs: P.kwargs) -> T:
             async with self:
```

### Comparing `ez-a-sync-0.6.0/a_sync/property.py` & `ez-a-sync-0.6.1.dev1/a_sync/property.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.6.0/ez_a_sync.egg-info/SOURCES.txt` & `ez-a-sync-0.6.1.dev1/ez_a_sync.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.6.0/setup.py` & `ez-a-sync-0.6.1.dev1/setup.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.6.0/tests/fixtures.py` & `ez-a-sync-0.6.1.dev1/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.6.0/tests/test_base.py` & `ez-a-sync-0.6.1.dev1/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.6.0/tests/test_cache.py` & `ez-a-sync-0.6.1.dev1/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.6.0/tests/test_decorator.py` & `ez-a-sync-0.6.1.dev1/tests/test_decorator.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.6.0/tests/test_executor.py` & `ez-a-sync-0.6.1.dev1/tests/test_executor.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.6.0/tests/test_limiter.py` & `ez-a-sync-0.6.1.dev1/tests/test_limiter.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.6.0/tests/test_meta.py` & `ez-a-sync-0.6.1.dev1/tests/test_meta.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.6.0/tests/test_semaphore.py` & `ez-a-sync-0.6.1.dev1/tests/test_semaphore.py`

 * *Files identical despite different names*

