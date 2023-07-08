# Comparing `tmp/redb-odm-1.2.3.tar.gz` & `tmp/redb-odm-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redb-odm-1.2.3.tar", last modified: Wed Jun 21 01:05:07 2023, max compression
+gzip compressed data, was "redb-odm-1.3.0.tar", last modified: Sat Jul  8 20:55:05 2023, max compression
```

## Comparing `redb-odm-1.2.3.tar` & `redb-odm-1.3.0.tar`

### file list

```diff
@@ -1,60 +1,61 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 01:05:07.649717 redb-odm-1.2.3/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-21 01:04:51.000000 redb-odm-1.2.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-06-21 01:05:07.649717 redb-odm-1.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-21 01:04:51.000000 redb-odm-1.2.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 01:05:07.645717 redb-odm-1.2.3/redb/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 01:05:07.645717 redb-odm-1.2.3/redb/behaviors/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-21 01:04:51.000000 redb-odm-1.2.3/redb/behaviors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8041 2023-06-21 01:04:51.000000 redb-odm-1.2.3/redb/behaviors/i_remember.py
--rw-r--r--   0 runner    (1001) docker     (123)     3368 2023-06-21 01:04:51.000000 redb-odm-1.2.3/redb/behaviors/soft_deletion.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 01:05:07.645717 redb-odm-1.2.3/redb/core/
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-06-21 01:04:51.000000 redb-odm-1.2.3/redb/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6838 2023-06-21 01:04:51.000000 redb-odm-1.2.3/redb/core/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    16669 2023-06-21 01:04:51.000000 redb-odm-1.2.3/redb/core/document.py
--rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-06-21 01:04:51.000000 redb-odm-1.2.3/redb/core/instance.py
--rw-r--r--   0 runner    (1001) docker     (123)    12510 2023-06-21 01:04:51.000000 redb-odm-1.2.3/redb/core/transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     3371 2023-06-21 01:04:51.000000 redb-odm-1.2.3/redb/core/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 01:05:07.649717 redb-odm-1.2.3/redb/interface/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 01:04:51.000000 redb-odm-1.2.3/redb/interface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-06-21 01:04:51.000000 redb-odm-1.2.3/redb/interface/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-06-21 01:04:51.000000 redb-odm-1.2.3/redb/interface/collection.py
--rw-r--r--   0 runner    (1001) docker     (123)      845 2023-06-21 01:04:51.000000 redb-odm-1.2.3/redb/interface/configs.py
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-06-21 01:04:51.000000 redb-odm-1.2.3/redb/interface/database.py
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-06-21 01:04:51.000000 redb-odm-1.2.3/redb/interface/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     7950 2023-06-21 01:04:51.000000 redb-odm-1.2.3/redb/interface/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-06-21 01:04:51.000000 redb-odm-1.2.3/redb/interface/results.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 01:05:07.649717 redb-odm-1.2.3/redb/json_system/
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-21 01:04:51.000000 redb-odm-1.2.3/redb/json_system/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-06-21 01:04:51.000000 redb-odm-1.2.3/redb/json_system/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     9302 2023-06-21 01:04:51.000000 redb-odm-1.2.3/redb/json_system/collection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-06-21 01:04:51.000000 redb-odm-1.2.3/redb/json_system/database.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 01:05:07.649717 redb-odm-1.2.3/redb/migo_system/
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-21 01:04:51.000000 redb-odm-1.2.3/redb/migo_system/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-06-21 01:04:51.000000 redb-odm-1.2.3/redb/migo_system/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    11715 2023-06-21 01:04:51.000000 redb-odm-1.2.3/redb/migo_system/collection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-06-21 01:04:51.000000 redb-odm-1.2.3/redb/migo_system/database.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 01:05:07.649717 redb-odm-1.2.3/redb/mongo_system/
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-21 01:04:51.000000 redb-odm-1.2.3/redb/mongo_system/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-06-21 01:04:51.000000 redb-odm-1.2.3/redb/mongo_system/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     6057 2023-06-21 01:04:51.000000 redb-odm-1.2.3/redb/mongo_system/collection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-06-21 01:04:51.000000 redb-odm-1.2.3/redb/mongo_system/database.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 01:05:07.649717 redb-odm-1.2.3/redb_odm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-06-21 01:05:07.000000 redb-odm-1.2.3/redb_odm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-06-21 01:05:07.000000 redb-odm-1.2.3/redb_odm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 01:05:07.000000 redb-odm-1.2.3/redb_odm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-21 01:05:07.000000 redb-odm-1.2.3/redb_odm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-21 01:05:07.000000 redb-odm-1.2.3/redb_odm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-21 01:04:51.000000 redb-odm-1.2.3/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-21 01:04:51.000000 redb-odm-1.2.3/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-21 01:04:51.000000 redb-odm-1.2.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 01:05:07.653717 redb-odm-1.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-06-21 01:04:51.000000 redb-odm-1.2.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 01:05:07.649717 redb-odm-1.2.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-06-21 01:04:51.000000 redb-odm-1.2.3/tests/test_bson_objs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2521 2023-06-21 01:04:51.000000 redb-odm-1.2.3/tests/test_hashing.py
--rw-r--r--   0 runner    (1001) docker     (123)     5326 2023-06-21 01:04:51.000000 redb-odm-1.2.3/tests/test_i_remember.py
--rw-r--r--   0 runner    (1001) docker     (123)     4156 2023-06-21 01:04:51.000000 redb-odm-1.2.3/tests/test_json_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     8216 2023-06-21 01:04:51.000000 redb-odm-1.2.3/tests/test_mongo_system.py
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-06-21 01:04:51.000000 redb-odm-1.2.3/tests/test_return_cls.py
--rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-06-21 01:04:51.000000 redb-odm-1.2.3/tests/test_soft_deletion.py
--rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-06-21 01:04:51.000000 redb-odm-1.2.3/tests/test_unique_constraints.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 20:55:05.043459 redb-odm-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-08 20:54:49.000000 redb-odm-1.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-07-08 20:55:05.043459 redb-odm-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-08 20:54:49.000000 redb-odm-1.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 20:55:05.035459 redb-odm-1.3.0/redb/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 20:55:05.039459 redb-odm-1.3.0/redb/behaviors/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-08 20:54:49.000000 redb-odm-1.3.0/redb/behaviors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8041 2023-07-08 20:54:49.000000 redb-odm-1.3.0/redb/behaviors/i_remember.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3368 2023-07-08 20:54:49.000000 redb-odm-1.3.0/redb/behaviors/soft_deletion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 20:55:05.039459 redb-odm-1.3.0/redb/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-07-08 20:54:49.000000 redb-odm-1.3.0/redb/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6838 2023-07-08 20:54:49.000000 redb-odm-1.3.0/redb/core/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17117 2023-07-08 20:54:49.000000 redb-odm-1.3.0/redb/core/document.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-07-08 20:54:49.000000 redb-odm-1.3.0/redb/core/instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-07-08 20:54:49.000000 redb-odm-1.3.0/redb/core/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12510 2023-07-08 20:54:49.000000 redb-odm-1.3.0/redb/core/transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3371 2023-07-08 20:54:49.000000 redb-odm-1.3.0/redb/core/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 20:55:05.039459 redb-odm-1.3.0/redb/interface/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 20:54:49.000000 redb-odm-1.3.0/redb/interface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-07-08 20:54:49.000000 redb-odm-1.3.0/redb/interface/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-07-08 20:54:49.000000 redb-odm-1.3.0/redb/interface/collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-07-08 20:54:49.000000 redb-odm-1.3.0/redb/interface/configs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-08 20:54:49.000000 redb-odm-1.3.0/redb/interface/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-07-08 20:54:49.000000 redb-odm-1.3.0/redb/interface/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7950 2023-07-08 20:54:49.000000 redb-odm-1.3.0/redb/interface/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-07-08 20:54:49.000000 redb-odm-1.3.0/redb/interface/results.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 20:55:05.039459 redb-odm-1.3.0/redb/json_system/
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-08 20:54:49.000000 redb-odm-1.3.0/redb/json_system/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-07-08 20:54:49.000000 redb-odm-1.3.0/redb/json_system/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9302 2023-07-08 20:54:49.000000 redb-odm-1.3.0/redb/json_system/collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-07-08 20:54:49.000000 redb-odm-1.3.0/redb/json_system/database.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 20:55:05.039459 redb-odm-1.3.0/redb/migo_system/
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-08 20:54:49.000000 redb-odm-1.3.0/redb/migo_system/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-07-08 20:54:49.000000 redb-odm-1.3.0/redb/migo_system/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11715 2023-07-08 20:54:49.000000 redb-odm-1.3.0/redb/migo_system/collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-07-08 20:54:49.000000 redb-odm-1.3.0/redb/migo_system/database.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 20:55:05.039459 redb-odm-1.3.0/redb/mongo_system/
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-08 20:54:49.000000 redb-odm-1.3.0/redb/mongo_system/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-07-08 20:54:49.000000 redb-odm-1.3.0/redb/mongo_system/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6920 2023-07-08 20:54:49.000000 redb-odm-1.3.0/redb/mongo_system/collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-07-08 20:54:49.000000 redb-odm-1.3.0/redb/mongo_system/database.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 20:55:05.043459 redb-odm-1.3.0/redb_odm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-07-08 20:55:05.000000 redb-odm-1.3.0/redb_odm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-07-08 20:55:05.000000 redb-odm-1.3.0/redb_odm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 20:55:05.000000 redb-odm-1.3.0/redb_odm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-08 20:55:05.000000 redb-odm-1.3.0/redb_odm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-08 20:55:05.000000 redb-odm-1.3.0/redb_odm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-08 20:54:49.000000 redb-odm-1.3.0/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-08 20:54:49.000000 redb-odm-1.3.0/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-08 20:54:49.000000 redb-odm-1.3.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 20:55:05.043459 redb-odm-1.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-07-08 20:54:49.000000 redb-odm-1.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 20:55:05.043459 redb-odm-1.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-07-08 20:54:49.000000 redb-odm-1.3.0/tests/test_bson_objs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2521 2023-07-08 20:54:49.000000 redb-odm-1.3.0/tests/test_hashing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5326 2023-07-08 20:54:49.000000 redb-odm-1.3.0/tests/test_i_remember.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4156 2023-07-08 20:54:49.000000 redb-odm-1.3.0/tests/test_json_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8216 2023-07-08 20:54:49.000000 redb-odm-1.3.0/tests/test_mongo_system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-07-08 20:54:49.000000 redb-odm-1.3.0/tests/test_return_cls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-07-08 20:54:49.000000 redb-odm-1.3.0/tests/test_soft_deletion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-07-08 20:54:49.000000 redb-odm-1.3.0/tests/test_unique_constraints.py
```

### Comparing `redb-odm-1.2.3/redb/behaviors/i_remember.py` & `redb-odm-1.3.0/redb/behaviors/i_remember.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.2.3/redb/behaviors/soft_deletion.py` & `redb-odm-1.3.0/redb/behaviors/soft_deletion.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.2.3/redb/core/base.py` & `redb-odm-1.3.0/redb/core/base.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.2.3/redb/core/document.py` & `redb-odm-1.3.0/redb/core/document.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 from datetime import datetime
 from pathlib import Path
 from typing import Any, Dict, Sequence, Type, TypeAlias, TypeVar, Union, cast
 
 import pytz
 from pymongo.errors import DuplicateKeyError
+
 from redb.interface.errors import (
     CannotUpdateIdentifyingField,
     UniqueConstraintViolation,
+    UnsupportedOperation,
 )
 from redb.interface.fields import (
     CompoundIndex,
     DBRef,
     Field,
     IncludeColumn,
     Index,
@@ -49,14 +51,15 @@
             DBRef: lambda ref: dict(ref.as_doc()),
             Path: str,
             ObjectId: str,
         }
         smart_union = True
 
     def __init__(self, **data: Any) -> None:
+        # TODO rewrite this using root_validator(pre=True) and root_validator(pre=False)
         calculate_hash = False
         if "id" in data:
             data["_id"] = data.pop("id")
         if "_id" not in data:
             data["_id"] = None
             calculate_hash = True
 
@@ -113,28 +116,36 @@
     def find_many(
         cls: Type[T],
         filter: OptionalDocumentData = None,
         fields: IncludeColumns = None,
         sort: SortColumns = None,
         skip: int = 0,
         limit: int = 0,
+        iterate: bool = False,
+        batch_size: int | None = None,
     ) -> list[T]:
+        if iterate and batch_size is not None:
+            msg = "'iterate' cannot be used with 'batch_size'. Batched find_many is already an iterable."
+            raise UnsupportedOperation(msg)
+
         collection = Document._get_collection(cls)
         filter = _format_document_data(filter)
         formatted_fields = _format_fields(fields)
         return_cls = _get_return_cls(cls, formatted_fields)
         sort_order = _format_sort(sort)
         return collection.find(
             cls=cls,
             return_cls=return_cls,
             filter=filter,
             fields=formatted_fields,
             sort=sort_order,
             skip=skip,
             limit=limit,
+            iterate=iterate,
+            batch_size=batch_size,
         )
 
     @classmethod
     def distinct(
         cls: Type[T],
         key: str,
         filter: OptionalDocumentData = None,
```

### Comparing `redb-odm-1.2.3/redb/core/instance.py` & `redb-odm-1.3.0/redb/core/instance.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.2.3/redb/core/transaction.py` & `redb-odm-1.3.0/redb/core/transaction.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.2.3/redb/core/utils.py` & `redb-odm-1.3.0/redb/core/utils.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.2.3/redb/interface/client.py` & `redb-odm-1.3.0/redb/interface/client.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.2.3/redb/interface/collection.py` & `redb-odm-1.3.0/redb/interface/collection.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.2.3/redb/interface/configs.py` & `redb-odm-1.3.0/redb/interface/configs.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.2.3/redb/interface/database.py` & `redb-odm-1.3.0/redb/interface/database.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.2.3/redb/interface/errors.py` & `redb-odm-1.3.0/redb/interface/errors.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,7 +22,11 @@
     ) -> None:
         if collection_name:
             msg = f"Duplicate key at collection {collection_name} on: {dup_keys}"
         else:
             msg = f"Duplicate key error on: {dup_keys}"
         super().__init__(msg, *args, collection_name=collection_name)
         self.dup_keys = [dup_keys]
+
+
+class UnsupportedOperation(REDBError):
+    pass
```

### Comparing `redb-odm-1.2.3/redb/interface/fields.py` & `redb-odm-1.3.0/redb/interface/fields.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.2.3/redb/interface/results.py` & `redb-odm-1.3.0/redb/interface/results.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.2.3/redb/json_system/client.py` & `redb-odm-1.3.0/redb/json_system/client.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.2.3/redb/json_system/collection.py` & `redb-odm-1.3.0/redb/json_system/collection.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.2.3/redb/json_system/database.py` & `redb-odm-1.3.0/redb/json_system/database.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.2.3/redb/migo_system/client.py` & `redb-odm-1.3.0/redb/migo_system/client.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.2.3/redb/migo_system/collection.py` & `redb-odm-1.3.0/redb/migo_system/collection.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.2.3/redb/migo_system/database.py` & `redb-odm-1.3.0/redb/migo_system/database.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.2.3/redb/mongo_system/client.py` & `redb-odm-1.3.0/redb/mongo_system/client.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.2.3/redb/mongo_system/collection.py` & `redb-odm-1.3.0/redb/mongo_system/collection.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,25 +1,27 @@
-from typing import Any, Literal, Type
+from typing import Any, Iterator, Type, TypeVar
 
 from pymongo.collection import Collection as PymongoCollection
 
 from redb.core import Document
 from redb.interface.collection import Collection, Json, OptionalJson, ReturnType
+from redb.interface.errors import DocumentNotFound
 from redb.interface.fields import CompoundIndex, PyMongoOperations
 from redb.interface.results import (
     BulkWriteResult,
     DeleteManyResult,
     DeleteOneResult,
     InsertManyResult,
     InsertOneResult,
     ReplaceOneResult,
     UpdateManyResult,
     UpdateOneResult,
 )
-from redb.interface.errors import DocumentNotFound
+
+T = TypeVar("T")
 
 
 class MongoCollection(Collection):
     __client_name__: str = "mongo"
 
     def __init__(self, collection: PymongoCollection) -> None:
         super().__init__()
@@ -56,25 +58,31 @@
         cls: Type[Document],
         return_cls: ReturnType,
         filter: OptionalJson = None,
         fields: dict[str, bool] | None = None,
         sort: list[tuple[str, str | int]] | None = None,
         skip: int = 0,
         limit: int = 0,
-    ) -> list[ReturnType]:
-        return [
-            return_cls(**result)
-            for result in self.__collection.find(
-                filter=filter,
-                projection=fields,
-                sort=sort,
-                skip=skip,
-                limit=limit,
-            )
-        ]
+        iterate: bool = False,
+        batch_size: int | None = None,
+    ) -> list[ReturnType] | Iterator[list[ReturnType]] | Iterator[ReturnType]:
+        cursor = self.__collection.find(
+            filter=filter,
+            projection=fields,
+            sort=sort,
+            skip=skip,
+            limit=limit,
+        )
+        if iterate:
+            return iter(iterate_converted_results(cursor, return_cls))  # type: ignore
+
+        if batch_size is not None:
+            return iter(batch_iterate_converted_results(cursor, batch_size, return_cls))  # type: ignore
+
+        return [return_cls(**result) for result in cursor]
 
     def find_one(
         self,
         cls: Type[Document],
         return_cls: ReturnType,
         filter: OptionalJson = None,
         fields: dict[str, bool] | None = None,
@@ -201,7 +209,27 @@
     def delete_many(
         self,
         cls: Type[Document],
         filter: Json,
     ) -> DeleteManyResult:
         result = self.__collection.delete_many(filter=filter)
         return DeleteManyResult(deleted_count=result.deleted_count)
+
+
+def iterate_converted_results(iterator, clazz: Type[T]) -> T:
+    for result in iterator:
+        yield clazz(**result)  # type: ignore
+
+
+def batch_iterate_converted_results(
+    iterator, batch_size: int, clazz: Type[T]
+) -> list[T]:
+    while True:
+        output = []
+        try:
+            for _ in range(batch_size):
+                output.append(clazz(**next(iterator)))
+        except StopIteration:
+            break
+        finally:
+            if output:
+                yield output
```

### Comparing `redb-odm-1.2.3/redb/mongo_system/database.py` & `redb-odm-1.3.0/redb/mongo_system/database.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.2.3/redb_odm.egg-info/SOURCES.txt` & `redb-odm-1.3.0/redb_odm.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 redb/behaviors/__init__.py
 redb/behaviors/i_remember.py
 redb/behaviors/soft_deletion.py
 redb/core/__init__.py
 redb/core/base.py
 redb/core/document.py
 redb/core/instance.py
+redb/core/mixins.py
 redb/core/transaction.py
 redb/core/utils.py
 redb/interface/__init__.py
 redb/interface/client.py
 redb/interface/collection.py
 redb/interface/configs.py
 redb/interface/database.py
```

### Comparing `redb-odm-1.2.3/setup.py` & `redb-odm-1.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.2.3/tests/test_bson_objs.py` & `redb-odm-1.3.0/tests/test_bson_objs.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.2.3/tests/test_hashing.py` & `redb-odm-1.3.0/tests/test_hashing.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.2.3/tests/test_i_remember.py` & `redb-odm-1.3.0/tests/test_i_remember.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.2.3/tests/test_json_client.py` & `redb-odm-1.3.0/tests/test_json_client.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.2.3/tests/test_mongo_system.py` & `redb-odm-1.3.0/tests/test_mongo_system.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.2.3/tests/test_return_cls.py` & `redb-odm-1.3.0/tests/test_return_cls.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.2.3/tests/test_soft_deletion.py` & `redb-odm-1.3.0/tests/test_soft_deletion.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.2.3/tests/test_unique_constraints.py` & `redb-odm-1.3.0/tests/test_unique_constraints.py`

 * *Files 18% similar despite different names*

```diff
@@ -13,17 +13,21 @@
 def client():
     RedB.setup(
         MongoConfig(
             database_uri=os.environ["MONGODB_URI"],
         )
     )
 
-@pytest.fixture(scope="module", autouse=True)
+
+@pytest.fixture(scope="function", autouse=True)
 def db():
-    return MongoClient(os.environ["MONGODB_URI"]).get_database()
+    db = MongoClient(os.environ["MONGODB_URI"]).get_database()
+    yield db
+    db.drop_collection("cats")
+
 
 class Cat(Document):
     name: str
     breed: str = "Domestic Shorthair"
     created_by: str
 
     @classmethod
@@ -31,22 +35,37 @@
          return [CompoundIndex([cls.name, cls.breed], unique=True)]  # type: ignore
 
     @classmethod
     def collection_name(cls) -> str:
         return "cats"
 
 
-def test_unique_constraints(db: Database):
-    db["cats"].drop()
+def test_unique_constraints():
     Cat.create_indexes()
     cat = Cat(name="Kitty", created_by="me")
     result = Cat.insert_one(cat)
     assert result.inserted_id is not None
     assert cat == Cat.find_one({"_id": result.inserted_id})
-    cat2 = cat = Cat(name="Kitty", created_by="other")
+    cat2 = Cat(name="Kitty", created_by="other")  # avoiding hash collision on _id
     with pytest.raises(UniqueConstraintViolation):
         Cat.insert_one(cat2)
     try:
         Cat.insert_one(cat2)
     except UniqueConstraintViolation as e:
         assert e.collection_name == "cats"
         assert e.dup_keys == [{"name": "Kitty", "breed": "Domestic Shorthair"}]
+
+
+def test_unique_ids():
+    Cat.create_indexes()
+    cat = Cat(name="Kitty", created_by="me")
+    result = Cat.insert_one(cat)
+    assert result.inserted_id is not None
+    assert cat == Cat.find_one({"_id": result.inserted_id})
+    with pytest.raises(UniqueConstraintViolation):
+        Cat.insert_one(cat)
+    try:
+        Cat.insert_one(cat)
+    except UniqueConstraintViolation as e:
+        assert e.collection_name == "cats"
+        assert len(e.dup_keys) == 1
+        assert e.dup_keys[0]["_id"] == result.inserted_id
```

