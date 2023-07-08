# Comparing `tmp/sqlalchemy_bind_manager-0.5.0.tar.gz` & `tmp/sqlalchemy_bind_manager-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlalchemy_bind_manager-0.5.0.tar", max compression
+gzip compressed data, was "sqlalchemy_bind_manager-0.6.0.tar", max compression
```

## Comparing `sqlalchemy_bind_manager-0.5.0.tar` & `sqlalchemy_bind_manager-0.6.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1073 2023-07-05 11:28:57.377510 sqlalchemy_bind_manager-0.5.0/LICENSE
--rw-r--r--   0        0        0     8733 2023-07-05 11:28:57.377510 sqlalchemy_bind_manager-0.5.0/README.md
--rw-r--r--   0        0        0     2375 2023-07-05 11:29:12.981766 sqlalchemy_bind_manager-0.5.0/pyproject.toml
--rw-r--r--   0        0        0      107 2023-07-05 11:28:57.377510 sqlalchemy_bind_manager-0.5.0/sqlalchemy_bind_manager/__init__.py
--rw-r--r--   0        0        0     5241 2023-07-05 11:28:57.377510 sqlalchemy_bind_manager-0.5.0/sqlalchemy_bind_manager/_bind_manager.py
--rw-r--r--   0        0        0      197 2023-07-05 11:28:57.377510 sqlalchemy_bind_manager-0.5.0/sqlalchemy_bind_manager/_repository/__init__.py
--rw-r--r--   0        0        0     6080 2023-07-05 11:28:57.377510 sqlalchemy_bind_manager-0.5.0/sqlalchemy_bind_manager/_repository/async_.py
--rw-r--r--   0        0        0    11340 2023-07-05 11:28:57.377510 sqlalchemy_bind_manager-0.5.0/sqlalchemy_bind_manager/_repository/base_repository.py
--rw-r--r--   0        0        0     1099 2023-07-05 11:28:57.377510 sqlalchemy_bind_manager-0.5.0/sqlalchemy_bind_manager/_repository/common.py
--rw-r--r--   0        0        0     7429 2023-07-05 11:28:57.377510 sqlalchemy_bind_manager-0.5.0/sqlalchemy_bind_manager/_repository/result_presenters.py
--rw-r--r--   0        0        0     5376 2023-07-05 11:28:57.377510 sqlalchemy_bind_manager-0.5.0/sqlalchemy_bind_manager/_repository/sync.py
--rw-r--r--   0        0        0     3118 2023-07-05 11:28:57.377510 sqlalchemy_bind_manager-0.5.0/sqlalchemy_bind_manager/_session_handler.py
--rw-r--r--   0        0        0     1704 2023-07-05 11:28:57.377510 sqlalchemy_bind_manager-0.5.0/sqlalchemy_bind_manager/_unit_of_work/__init__.py
--rw-r--r--   0        0        0      310 2023-07-05 11:28:57.377510 sqlalchemy_bind_manager-0.5.0/sqlalchemy_bind_manager/exceptions.py
--rw-r--r--   0        0        0    11155 2023-07-05 11:28:57.377510 sqlalchemy_bind_manager-0.5.0/sqlalchemy_bind_manager/protocols.py
--rw-r--r--   0        0        0        0 2023-07-05 11:28:57.377510 sqlalchemy_bind_manager-0.5.0/sqlalchemy_bind_manager/py.typed
--rw-r--r--   0        0        0      242 2023-07-05 11:28:57.377510 sqlalchemy_bind_manager-0.5.0/sqlalchemy_bind_manager/repository.py
--rw-r--r--   0        0        0    10126 1970-01-01 00:00:00.000000 sqlalchemy_bind_manager-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-07-08 11:01:18.572363 sqlalchemy_bind_manager-0.6.0/LICENSE
+-rw-r--r--   0        0        0     8778 2023-07-08 11:01:18.572363 sqlalchemy_bind_manager-0.6.0/README.md
+-rw-r--r--   0        0        0     2375 2023-07-08 11:01:31.344604 sqlalchemy_bind_manager-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0      107 2023-07-08 11:01:18.576363 sqlalchemy_bind_manager-0.6.0/sqlalchemy_bind_manager/__init__.py
+-rw-r--r--   0        0        0     5241 2023-07-08 11:01:18.576363 sqlalchemy_bind_manager-0.6.0/sqlalchemy_bind_manager/_bind_manager.py
+-rw-r--r--   0        0        0      197 2023-07-08 11:01:18.576363 sqlalchemy_bind_manager-0.6.0/sqlalchemy_bind_manager/_repository/__init__.py
+-rw-r--r--   0        0        0     6080 2023-07-08 11:01:18.576363 sqlalchemy_bind_manager-0.6.0/sqlalchemy_bind_manager/_repository/async_.py
+-rw-r--r--   0        0        0    11340 2023-07-08 11:01:18.576363 sqlalchemy_bind_manager-0.6.0/sqlalchemy_bind_manager/_repository/base_repository.py
+-rw-r--r--   0        0        0     1099 2023-07-08 11:01:18.576363 sqlalchemy_bind_manager-0.6.0/sqlalchemy_bind_manager/_repository/common.py
+-rw-r--r--   0        0        0     7429 2023-07-08 11:01:18.576363 sqlalchemy_bind_manager-0.6.0/sqlalchemy_bind_manager/_repository/result_presenters.py
+-rw-r--r--   0        0        0     5376 2023-07-08 11:01:18.576363 sqlalchemy_bind_manager-0.6.0/sqlalchemy_bind_manager/_repository/sync.py
+-rw-r--r--   0        0        0     3118 2023-07-08 11:01:18.576363 sqlalchemy_bind_manager-0.6.0/sqlalchemy_bind_manager/_session_handler.py
+-rw-r--r--   0        0        0     2507 2023-07-08 11:01:18.576363 sqlalchemy_bind_manager-0.6.0/sqlalchemy_bind_manager/_unit_of_work/__init__.py
+-rw-r--r--   0        0        0      358 2023-07-08 11:01:18.576363 sqlalchemy_bind_manager-0.6.0/sqlalchemy_bind_manager/exceptions.py
+-rw-r--r--   0        0        0    11155 2023-07-08 11:01:18.576363 sqlalchemy_bind_manager-0.6.0/sqlalchemy_bind_manager/protocols.py
+-rw-r--r--   0        0        0        0 2023-07-08 11:01:18.576363 sqlalchemy_bind_manager-0.6.0/sqlalchemy_bind_manager/py.typed
+-rw-r--r--   0        0        0      242 2023-07-08 11:01:18.576363 sqlalchemy_bind_manager-0.6.0/sqlalchemy_bind_manager/repository.py
+-rw-r--r--   0        0        0    10171 1970-01-01 00:00:00.000000 sqlalchemy_bind_manager-0.6.0/PKG-INFO
```

### Comparing `sqlalchemy_bind_manager-0.5.0/LICENSE` & `sqlalchemy_bind_manager-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sqlalchemy_bind_manager-0.5.0/README.md` & `sqlalchemy_bind_manager-0.6.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -178,17 +178,17 @@
 
 We can use the `UnitOfWork` or the `AsyncUnitOfWork` class to provide a shared session to
 be used for repository operations, **assumed the same bind is used for all the repositories**.
 
 ```python
 class MyRepo(SQLAlchemyRepository):
     _model = MyModel
-class MyOtherRepo(SQLAlchemyRepository):
-    _model = MyOtherModel
 
 bind = sa_manager.get_bind()
-uow = UnitOfWork(bind, (MyRepo, MyOtherRepo))
+uow = UnitOfWork(bind)
+uow.register_repository("repo_a", MyRepo)
+uow.register_repository("repo_b", SQLAlchemyRepository, MyOtherModel)
 
 with uow.transaction():
-    uow.MyRepo.save(some_model)
-    uow.MyOtherRepo.save(some_other_model)
+    uow.repository("repo_a").save(some_model)
+    uow.repository("repo_b").save(some_other_model)
 ```
```

### Comparing `sqlalchemy_bind_manager-0.5.0/pyproject.toml` & `sqlalchemy_bind_manager-0.6.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sqlalchemy-bind-manager"
-version = "0.5.0"
+version = "0.6.0"
 description = "A manager to easily handle multiple SQLAlchemy configurations"
 license = "MIT"
 authors = ["Federico Busetti <729029+febus982@users.noreply.github.com>"]
 repository = "https://github.com/febus982/sqlalchemy-bind-manager"
 homepage = "https://febus982.github.io/sqlalchemy-bind-manager"
 readme = "README.md"
 packages = [{include = "sqlalchemy_bind_manager"}]
```

### Comparing `sqlalchemy_bind_manager-0.5.0/sqlalchemy_bind_manager/_bind_manager.py` & `sqlalchemy_bind_manager-0.6.0/sqlalchemy_bind_manager/_bind_manager.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_bind_manager-0.5.0/sqlalchemy_bind_manager/_repository/async_.py` & `sqlalchemy_bind_manager-0.6.0/sqlalchemy_bind_manager/_repository/async_.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_bind_manager-0.5.0/sqlalchemy_bind_manager/_repository/base_repository.py` & `sqlalchemy_bind_manager-0.6.0/sqlalchemy_bind_manager/_repository/base_repository.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_bind_manager-0.5.0/sqlalchemy_bind_manager/_repository/common.py` & `sqlalchemy_bind_manager-0.6.0/sqlalchemy_bind_manager/_repository/common.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_bind_manager-0.5.0/sqlalchemy_bind_manager/_repository/result_presenters.py` & `sqlalchemy_bind_manager-0.6.0/sqlalchemy_bind_manager/_repository/result_presenters.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_bind_manager-0.5.0/sqlalchemy_bind_manager/_repository/sync.py` & `sqlalchemy_bind_manager-0.6.0/sqlalchemy_bind_manager/_repository/sync.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_bind_manager-0.5.0/sqlalchemy_bind_manager/_session_handler.py` & `sqlalchemy_bind_manager-0.6.0/sqlalchemy_bind_manager/_session_handler.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_bind_manager-0.5.0/sqlalchemy_bind_manager/protocols.py` & `sqlalchemy_bind_manager-0.6.0/sqlalchemy_bind_manager/protocols.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_bind_manager-0.5.0/PKG-INFO` & `sqlalchemy_bind_manager-0.6.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlalchemy-bind-manager
-Version: 0.5.0
+Version: 0.6.0
 Summary: A manager to easily handle multiple SQLAlchemy configurations
 Home-page: https://febus982.github.io/sqlalchemy-bind-manager
 License: MIT
 Keywords: sqlalchemy,config,manager
 Author: Federico Busetti
 Author-email: 729029+febus982@users.noreply.github.com
 Requires-Python: >=3.8,<3.12
@@ -211,18 +211,18 @@
 
 We can use the `UnitOfWork` or the `AsyncUnitOfWork` class to provide a shared session to
 be used for repository operations, **assumed the same bind is used for all the repositories**.
 
 ```python
 class MyRepo(SQLAlchemyRepository):
     _model = MyModel
-class MyOtherRepo(SQLAlchemyRepository):
-    _model = MyOtherModel
 
 bind = sa_manager.get_bind()
-uow = UnitOfWork(bind, (MyRepo, MyOtherRepo))
+uow = UnitOfWork(bind)
+uow.register_repository("repo_a", MyRepo)
+uow.register_repository("repo_b", SQLAlchemyRepository, MyOtherModel)
 
 with uow.transaction():
-    uow.MyRepo.save(some_model)
-    uow.MyOtherRepo.save(some_other_model)
+    uow.repository("repo_a").save(some_model)
+    uow.repository("repo_b").save(some_other_model)
 ```
```

