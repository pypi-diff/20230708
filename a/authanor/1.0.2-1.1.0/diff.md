# Comparing `tmp/authanor-1.0.2.tar.gz` & `tmp/authanor-1.1.0.tar.gz`

## Comparing `authanor-1.0.2.tar` & `authanor-1.1.0.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 authanor-1.0.2/CHANGELOG.md
--rw-r--r--   0        0        0     2017 2020-02-02 00:00:00.000000 authanor-1.0.2/Makefile
--rw-r--r--   0        0        0     3686 2020-02-02 00:00:00.000000 authanor-1.0.2/README.md
--rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 authanor-1.0.2/_vimrc_local.vim
--rw-r--r--   0        0        0      825 2020-02-02 00:00:00.000000 authanor-1.0.2/config.mk
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 authanor-1.0.2/requirements.txt
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 authanor-1.0.2/.pytest_cache/.gitignore
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 authanor-1.0.2/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 authanor-1.0.2/.pytest_cache/README.md
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 authanor-1.0.2/.pytest_cache/v/cache/lastfailed
--rw-r--r--   0        0        0    10575 2020-02-02 00:00:00.000000 authanor-1.0.2/.pytest_cache/v/cache/nodeids
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 authanor-1.0.2/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 authanor-1.0.2/docs/Makefile
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 authanor-1.0.2/docs/make.bat
--rw-r--r--   0        0        0     1282 2020-02-02 00:00:00.000000 authanor-1.0.2/docs/source/conf.py
--rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 authanor-1.0.2/docs/source/index.rst
--rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 authanor-1.0.2/docs/source/api/database.rst
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 authanor-1.0.2/docs/source/api/modules.rst
--rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 authanor-1.0.2/docs/source/api/testing.rst
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 authanor-1.0.2/src/authanor/_version.py
--rw-r--r--   0        0        0     4022 2020-02-02 00:00:00.000000 authanor-1.0.2/src/authanor/database/__init__.py
--rw-r--r--   0        0        0    18064 2020-02-02 00:00:00.000000 authanor-1.0.2/src/authanor/database/handler.py
--rw-r--r--   0        0        0     5546 2020-02-02 00:00:00.000000 authanor-1.0.2/src/authanor/database/models.py
--rw-r--r--   0        0        0      896 2020-02-02 00:00:00.000000 authanor-1.0.2/src/authanor/database/utils.py
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 authanor-1.0.2/src/authanor/testing/__init__.py
--rw-r--r--   0        0        0    11617 2020-02-02 00:00:00.000000 authanor-1.0.2/src/authanor/testing/helpers.py
--rw-r--r--   0        0        0     1955 2020-02-02 00:00:00.000000 authanor-1.0.2/tests/conftest.py
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 authanor-1.0.2/tests/database/test_db.py
--rw-r--r--   0        0        0    22059 2020-02-02 00:00:00.000000 authanor-1.0.2/tests/database/test_handler.py
--rw-r--r--   0        0        0     3555 2020-02-02 00:00:00.000000 authanor-1.0.2/tests/database/test_models.py
--rw-r--r--   0        0        0     1184 2020-02-02 00:00:00.000000 authanor-1.0.2/tests/database/test_utils.py
--rw-r--r--   0        0        0     1985 2020-02-02 00:00:00.000000 authanor-1.0.2/tests/helpers/test_helpers.py
--rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 authanor-1.0.2/.gitignore
--rw-r--r--   0        0        0    35150 2020-02-02 00:00:00.000000 authanor-1.0.2/COPYING
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 authanor-1.0.2/LICENSE
--rw-r--r--   0        0        0     2271 2020-02-02 00:00:00.000000 authanor-1.0.2/pyproject.toml
--rw-r--r--   0        0        0     4730 2020-02-02 00:00:00.000000 authanor-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 authanor-1.1.0/CHANGELOG.md
+-rw-r--r--   0        0        0     2017 2020-02-02 00:00:00.000000 authanor-1.1.0/Makefile
+-rw-r--r--   0        0        0     2590 2020-02-02 00:00:00.000000 authanor-1.1.0/README.md
+-rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 authanor-1.1.0/_vimrc_local.vim
+-rw-r--r--   0        0        0      825 2020-02-02 00:00:00.000000 authanor-1.1.0/config.mk
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 authanor-1.1.0/requirements.txt
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 authanor-1.1.0/.pytest_cache/.gitignore
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 authanor-1.1.0/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 authanor-1.1.0/.pytest_cache/README.md
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 authanor-1.1.0/.pytest_cache/v/cache/lastfailed
+-rw-r--r--   0        0        0    10575 2020-02-02 00:00:00.000000 authanor-1.1.0/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 authanor-1.1.0/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 authanor-1.1.0/docs/Makefile
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 authanor-1.1.0/docs/make.bat
+-rw-r--r--   0        0        0     1282 2020-02-02 00:00:00.000000 authanor-1.1.0/docs/source/conf.py
+-rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 authanor-1.1.0/docs/source/index.rst
+-rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 authanor-1.1.0/docs/source/api/database.rst
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 authanor-1.1.0/docs/source/api/modules.rst
+-rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 authanor-1.1.0/docs/source/api/testing.rst
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 authanor-1.1.0/src/authanor/_version.py
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 authanor-1.1.0/src/authanor/database/__init__.py
+-rw-r--r--   0        0        0    18064 2020-02-02 00:00:00.000000 authanor-1.1.0/src/authanor/database/handler.py
+-rw-r--r--   0        0        0     5620 2020-02-02 00:00:00.000000 authanor-1.1.0/src/authanor/database/models.py
+-rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 authanor-1.1.0/src/authanor/database/utils.py
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 authanor-1.1.0/src/authanor/testing/__init__.py
+-rw-r--r--   0        0        0     3844 2020-02-02 00:00:00.000000 authanor-1.1.0/src/authanor/testing/helpers.py
+-rw-r--r--   0        0        0     1839 2020-02-02 00:00:00.000000 authanor-1.1.0/tests/conftest.py
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 authanor-1.1.0/tests/database/test_db.py
+-rw-r--r--   0        0        0    22101 2020-02-02 00:00:00.000000 authanor-1.1.0/tests/database/test_handler.py
+-rw-r--r--   0        0        0     3558 2020-02-02 00:00:00.000000 authanor-1.1.0/tests/database/test_models.py
+-rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 authanor-1.1.0/tests/database/test_utils.py
+-rw-r--r--   0        0        0     1985 2020-02-02 00:00:00.000000 authanor-1.1.0/tests/helpers/testing_helpers.py
+-rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 authanor-1.1.0/.gitignore
+-rw-r--r--   0        0        0    35150 2020-02-02 00:00:00.000000 authanor-1.1.0/COPYING
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 authanor-1.1.0/LICENSE
+-rw-r--r--   0        0        0     2288 2020-02-02 00:00:00.000000 authanor-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     3656 2020-02-02 00:00:00.000000 authanor-1.1.0/PKG-INFO
```

### Comparing `authanor-1.0.2/Makefile` & `authanor-1.1.0/Makefile`

 * *Files identical despite different names*

### Comparing `authanor-1.0.2/README.md` & `authanor-1.1.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -18,24 +18,14 @@
 It's possible I'm missing a key functionality of SQLAlchemy that enables this behavior elegantly, but I haven't found a satisfiably clean way to do it yet.
 Until I become so enlightened, this package creates an interface where each model may define the chain of joins required to establish whether it belongs to an authorized user, and then a handler to query the database and perform those joins for each query.
 This is designed to be extensible, since I often want this behavior available for the majority of ORM models in my application.
 
 If you read this and think "This dude's dumb; why on Earth didn't he use _this_ functionality baked into SQLAlchemy?" drop me a line because I'm interested to know what I'm missing.
 
 
-### Testing Tools
-
-Separately, the package also includes tools for testing database interactions via `pytest`.
-This includes fixtures for testing the handler objects mentioned above, but also for generally handling test setup and teardown.
-Perhaps most consequentially in that regard are the `AppTestManager` object and `@transaction_lifetime` decorator in the `testing` module.
-The `AppTestManager` intelligently uses an existing "persistent" database for the majority of an application's tests (created just once, and prefilled as necessary), unless the app is run within the context of a SQLAlchemy transaction in which case an "ephemeral" database is created for just the lifetime of a single test.
-Tests are denoted as consisting of SQLAlchemy transactions by decorating them with the `@transaction_lifetime` generator.
-This structure allows a single global database to be created once at the beginning of testing to serve any test that only accesses the database, but then database copies are only ever generated when explicitly required (e.g., for testing create/update/delete actions).
-
-
 ## Installation
 
 The _Authanor_ package is registered on the [Python Package Index (PyPI)](https://pypi.org/project/authanor) for easy installation.
 To install the package, simply run
 
 ```
 $ pip install authanor
```

### Comparing `authanor-1.0.2/config.mk` & `authanor-1.1.0/config.mk`

 * *Files identical despite different names*

### Comparing `authanor-1.0.2/.pytest_cache/v/cache/nodeids` & `authanor-1.1.0/.pytest_cache/v/cache/nodeids`

 * *Files identical despite different names*

### Comparing `authanor-1.0.2/docs/Makefile` & `authanor-1.1.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `authanor-1.0.2/docs/make.bat` & `authanor-1.1.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `authanor-1.0.2/docs/source/conf.py` & `authanor-1.1.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `authanor-1.0.2/docs/source/api/database.rst` & `authanor-1.1.0/docs/source/api/database.rst`

 * *Files identical despite different names*

### Comparing `authanor-1.0.2/src/authanor/database/handler.py` & `authanor-1.1.0/src/authanor/database/handler.py`

 * *Files identical despite different names*

### Comparing `authanor-1.0.2/src/authanor/database/models.py` & `authanor-1.1.0/src/authanor/database/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 """
 ORM model definitions corresponding to tables in the SQLite database.
 """
 from datetime import date
 
 from flask import g
+from fuisce.database import SQLAlchemy
 from sqlalchemy import event, inspect, select
 from sqlalchemy.ext.hybrid import hybrid_property
 from sqlalchemy.orm import DeclarativeBase, declared_attr
 from sqlalchemy.sql.expression import TableClause
 from sqlalchemy_views import CreateView as _CreateView
 
 
 class Model(DeclarativeBase):
     """A declarative base for all models."""
+    metadata = SQLAlchemy.metadata
 
     def _format_repr_attr(self, name):
         value = getattr(self, name)
         value_str = f"{value}"
         # Abbreviate the string if it is longer than a set length
         abbrev_len = 25
         if len(value_str) > abbrev_len:
```

### Comparing `authanor-1.0.2/tests/conftest.py` & `authanor-1.1.0/tests/conftest.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,61 +1,55 @@
 from unittest.mock import Mock, patch
 
 import pytest
 from flask import Flask
-from sqlalchemy import create_engine
+from fuisce.database import SQLAlchemy
+from fuisce.testing import AppTestManager
 
-from authanor.database import SQLAlchemy as _SQLAlchemy
-from authanor.testing.helpers import AppTestManager
+from testing_helpers import AlternateAuthorizedEntry, AuthorizedEntry, Entry
 
-from test_helpers import AlternateAuthorizedEntry, AuthorizedEntry, Entry
 
+class AuthanorAppTestManager(AppTestManager):
+    """A test manager for the Authanor app."""
 
-class SQLAlchemy(_SQLAlchemy):
-    def initialize(self, app):
-        """Initialize (and prepopulate) the database for testing."""
-        super().initialize(app)
-        _preload_database(app)
-
-
-def _preload_database(app):
-    with app.db.session.begin():
-        entries = [
-            Entry(x=1, y="ten", user_id=1),
-            Entry(x=2, y="eleven", user_id=1),
-            Entry(x=3, y="twelve", user_id=1),
-            Entry(x=4, y="twenty", user_id=2),
-            AuthorizedEntry(a=1, b="one", c=1),
-            AuthorizedEntry(a=2, b="two", c=1),
-            AuthorizedEntry(a=3, b="three", c=4),
-            AlternateAuthorizedEntry(p=1, q=1),
-            AlternateAuthorizedEntry(p=2, q=2),
-            AlternateAuthorizedEntry(p=3, q=2),
-            AlternateAuthorizedEntry(p=4, q=3),
-        ]
-        app.db.session.add_all(entries)
+    def prepare_test_database(self, db):
+        with db.session.begin():
+            entries = [
+                Entry(x=1, y="ten", user_id=1),
+                Entry(x=2, y="eleven", user_id=1),
+                Entry(x=3, y="twelve", user_id=1),
+                Entry(x=4, y="twenty", user_id=2),
+                AuthorizedEntry(a=1, b="one", c=1),
+                AuthorizedEntry(a=2, b="two", c=1),
+                AuthorizedEntry(a=3, b="three", c=4),
+                AlternateAuthorizedEntry(p=1, q=1),
+                AlternateAuthorizedEntry(p=2, q=2),
+                AlternateAuthorizedEntry(p=3, q=2),
+                AlternateAuthorizedEntry(p=4, q=3),
+            ]
+            db.session.add_all(entries)
 
 
 def create_test_app(test_config):
     # Create and configure the test app
     app = Flask("test")
     app.config.from_object(test_config)
     init_app(app)
     return app
 
 
-@SQLAlchemy.interface_selector(interface_instance=None)
+@SQLAlchemy.interface_selector
 def init_app(app):
     # Initialize the app
     # * The decorator performs all necessary actions in this minimal test example
     pass
 
 
 # Instantiate the app manager to determine the correct app (persistent/ephemeral)
-app_manager = AppTestManager(factory=create_test_app)
+app_manager = AuthanorAppTestManager(factory=create_test_app)
 
 
 @pytest.fixture
 def app():
     yield app_manager.get_app()
```

### Comparing `authanor-1.0.2/tests/database/test_handler.py` & `authanor-1.1.0/tests/database/test_handler.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,20 +9,21 @@
 from authanor.database.handler import (
     DatabaseHandler,
     DatabaseViewHandler,
     QueryCriteria,
 )
 from authanor.testing.helpers import TestHandler
 
-from test_helpers import (
+from testing_helpers import (
     AlternateAuthorizedEntry,
     AlternateAuthorizedEntryView,
     AuthorizedEntry,
     Entry,
 )
+from fuisce.database import SQLAlchemy
 
 
 @contextmanager
 def mocked_user(user_id):
     with patch("authanor.database.handler.g") as mock_global_namespace:
         with patch("authanor.database.models.g", new=mock_global_namespace):
             mock_global_namespace.user = Mock(id=1)
```

### Comparing `authanor-1.0.2/tests/database/test_models.py` & `authanor-1.1.0/tests/database/test_models.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Tests for the specialized authorization models."""
 from unittest.mock import Mock, call, patch
 
 import pytest
 
 from authanor.database.models import AuthorizedAccessMixin, Model
 
-from test_helpers import AuthorizedEntry, Entry
+from testing_helpers import AuthorizedEntry, Entry
 
 
 class TestModels:
     def test_model_initialization(self):
         mapping = {
             "x": 1,
             "y": "test1",
```

### Comparing `authanor-1.0.2/tests/helpers/test_helpers.py` & `authanor-1.1.0/tests/helpers/testing_helpers.py`

 * *Files identical despite different names*

### Comparing `authanor-1.0.2/.gitignore` & `authanor-1.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `authanor-1.0.2/COPYING` & `authanor-1.1.0/COPYING`

 * *Files identical despite different names*

### Comparing `authanor-1.0.2/pyproject.toml` & `authanor-1.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -8,14 +8,15 @@
     { name = 'Mitch Negus', email = 'mitchnegus57@gmail.com' },
 ]
 description = 'A Pythonic SQLALchemy interface to enforce authorization criteria.'
 license = { text = 'GNU GPLv3' }
 requires-python = '>=3.9,<3.11'
 dependencies = [
     'flask>=2.2.2',
+    'fuisce',
     'sqlalchemy>=2.0.0',
     'sqlalchemy-views>=0.3.2',
 ]
 keywords = [
 ]
 classifiers = [
   'Development Status :: 3 - Alpha',
@@ -82,8 +83,8 @@
 
 [tool.black]
 force-exclude = 'src/authanor/_version.py'
 
 [tool.isort]
 profile = 'black'
 src_paths = ['src/authanor', 'tests']
-known_local_folder = ["test_helpers"]
+known_local_folder = ["testing_helpers"]
```

### Comparing `authanor-1.0.2/PKG-INFO` & `authanor-1.1.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: authanor
-Version: 1.0.2
+Version: 1.1.0
 Summary: A Pythonic SQLALchemy interface to enforce authorization criteria.
 Project-URL: Download, https://pypi.org/project/authanor
 Project-URL: Homepage, https://github.com/mitchnegus/authanor
 Project-URL: Repository, https://github.com/mitchnegus/authanor
 Project-URL: Changelog, https://github.com/mitchnegus/authanor/blob/main/CHANGELOG.md
 Author-email: Mitch Negus <mitchnegus57@gmail.com>
 License: GNU GPLv3
@@ -15,14 +15,15 @@
 Classifier: Framework :: Pytest
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Requires-Python: <3.11,>=3.9
 Requires-Dist: flask>=2.2.2
+Requires-Dist: fuisce
 Requires-Dist: sqlalchemy-views>=0.3.2
 Requires-Dist: sqlalchemy>=2.0.0
 Description-Content-Type: text/markdown
 
 # Authanor
 
 <img src="https://upload.wikimedia.org/wikipedia/commons/1/10/Athanor.jpg" alt="Athanor" />
@@ -43,24 +44,14 @@
 It's possible I'm missing a key functionality of SQLAlchemy that enables this behavior elegantly, but I haven't found a satisfiably clean way to do it yet.
 Until I become so enlightened, this package creates an interface where each model may define the chain of joins required to establish whether it belongs to an authorized user, and then a handler to query the database and perform those joins for each query.
 This is designed to be extensible, since I often want this behavior available for the majority of ORM models in my application.
 
 If you read this and think "This dude's dumb; why on Earth didn't he use _this_ functionality baked into SQLAlchemy?" drop me a line because I'm interested to know what I'm missing.
 
 
-### Testing Tools
-
-Separately, the package also includes tools for testing database interactions via `pytest`.
-This includes fixtures for testing the handler objects mentioned above, but also for generally handling test setup and teardown.
-Perhaps most consequentially in that regard are the `AppTestManager` object and `@transaction_lifetime` decorator in the `testing` module.
-The `AppTestManager` intelligently uses an existing "persistent" database for the majority of an application's tests (created just once, and prefilled as necessary), unless the app is run within the context of a SQLAlchemy transaction in which case an "ephemeral" database is created for just the lifetime of a single test.
-Tests are denoted as consisting of SQLAlchemy transactions by decorating them with the `@transaction_lifetime` generator.
-This structure allows a single global database to be created once at the beginning of testing to serve any test that only accesses the database, but then database copies are only ever generated when explicitly required (e.g., for testing create/update/delete actions).
-
-
 ## Installation
 
 The _Authanor_ package is registered on the [Python Package Index (PyPI)](https://pypi.org/project/authanor) for easy installation.
 To install the package, simply run
 
 ```
 $ pip install authanor
```

