# Comparing `tmp/fuisce-0.0.0.tar.gz` & `tmp/fuisce-1.0.0.tar.gz`

## Comparing `fuisce-0.0.0.tar` & `fuisce-1.0.0.tar`

### file list

```diff
@@ -1,24 +1,26 @@
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 fuisce-0.0.0/CHANGELOG.md
--rw-r--r--   0        0        0     2017 2020-02-02 00:00:00.000000 fuisce-0.0.0/Makefile
--rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 fuisce-0.0.0/README.md
--rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 fuisce-0.0.0/_vimrc_local.vim
--rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 fuisce-0.0.0/config.mk
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 fuisce-0.0.0/requirements.txt
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 fuisce-0.0.0/docs/Makefile
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 fuisce-0.0.0/docs/make.bat
--rw-r--r--   0        0        0     1276 2020-02-02 00:00:00.000000 fuisce-0.0.0/docs/source/conf.py
--rw-r--r--   0        0        0      418 2020-02-02 00:00:00.000000 fuisce-0.0.0/docs/source/index.rst
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 fuisce-0.0.0/src/fuisce/_version.py
--rw-r--r--   0        0        0     5080 2020-02-02 00:00:00.000000 fuisce-0.0.0/src/fuisce/database/__init__.py
--rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 fuisce-0.0.0/src/fuisce/database/utils.py
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 fuisce-0.0.0/src/fuisce/testing/__init__.py
--rw-r--r--   0        0        0     8093 2020-02-02 00:00:00.000000 fuisce-0.0.0/src/fuisce/testing/helpers.py
--rw-r--r--   0        0        0     1548 2020-02-02 00:00:00.000000 fuisce-0.0.0/tests/conftest.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 fuisce-0.0.0/tests/database/test_db.py
--rw-r--r--   0        0        0      787 2020-02-02 00:00:00.000000 fuisce-0.0.0/tests/database/test_utils.py
--rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 fuisce-0.0.0/tests/helpers/testing_helpers.py
--rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 fuisce-0.0.0/.gitignore
--rw-r--r--   0        0        0    35150 2020-02-02 00:00:00.000000 fuisce-0.0.0/COPYING
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 fuisce-0.0.0/LICENSE
--rw-r--r--   0        0        0     2183 2020-02-02 00:00:00.000000 fuisce-0.0.0/pyproject.toml
--rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 fuisce-0.0.0/PKG-INFO
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 fuisce-1.0.0/CHANGELOG.md
+-rw-r--r--   0        0        0     2019 2020-02-02 00:00:00.000000 fuisce-1.0.0/Makefile
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 fuisce-1.0.0/README.md -> docs/source/README.md
+-rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 fuisce-1.0.0/_vimrc_local.vim
+-rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 fuisce-1.0.0/config.mk
+-rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 fuisce-1.0.0/requirements.txt
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 fuisce-1.0.0/docs/Makefile
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 fuisce-1.0.0/docs/make.bat
+-rw-r--r--   0        0        0     2627 2020-02-02 00:00:00.000000 fuisce-1.0.0/docs/source/README.md
+-rw-r--r--   0        0        0     1296 2020-02-02 00:00:00.000000 fuisce-1.0.0/docs/source/conf.py
+-rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 fuisce-1.0.0/docs/source/index.rst
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 fuisce-1.0.0/src/fuisce/_version.py
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 fuisce-1.0.0/src/fuisce/database/__init__.py
+-rw-r--r--   0        0        0     5231 2020-02-02 00:00:00.000000 fuisce-1.0.0/src/fuisce/database/interface.py
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 fuisce-1.0.0/src/fuisce/testing/__init__.py
+-rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 fuisce-1.0.0/src/fuisce/testing/config.py
+-rw-r--r--   0        0        0     8162 2020-02-02 00:00:00.000000 fuisce-1.0.0/src/fuisce/testing/manager.py
+-rw-r--r--   0        0        0     1286 2020-02-02 00:00:00.000000 fuisce-1.0.0/tests/conftest.py
+-rw-r--r--   0        0        0     2093 2020-02-02 00:00:00.000000 fuisce-1.0.0/tests/database/test_interface.py
+-rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 fuisce-1.0.0/tests/helpers/testing_helpers.py
+-rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 fuisce-1.0.0/tests/testing/test_manager.py
+-rw-r--r--   0        0        0      927 2020-02-02 00:00:00.000000 fuisce-1.0.0/.gitignore
+-rw-r--r--   0        0        0    35150 2020-02-02 00:00:00.000000 fuisce-1.0.0/COPYING
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 fuisce-1.0.0/LICENSE
+-rw-r--r--   0        0        0     2376 2020-02-02 00:00:00.000000 fuisce-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     3657 2020-02-02 00:00:00.000000 fuisce-1.0.0/PKG-INFO
```

### Comparing `fuisce-0.0.0/Makefile` & `fuisce-1.0.0/Makefile`

 * *Files 4% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 
 
 ## docs 		: Build documentation
 .PHONY: docs
 docs : env
 	@rm -rf $(DOCS_SRC_API)
 	@. $(ENV_ACTIVATE); \
-	sphinx-apidoc -f -o $(DOCS_SRC_API) $(PACKAGE_DIR);
+	sphinx-apidoc -f -o $(DOCS_SRC_API) $(PACKAGE_DIR); \
 	sphinx-build -b html $(DOCS_SRC) $(DOCS_HTML)
 
 
 ## test		: Run tests
 .PHONY: test
 test : env
 	@. $(ENV_ACTIVATE); \
```

### Comparing `fuisce-0.0.0/config.mk` & `fuisce-1.0.0/config.mk`

 * *Files identical despite different names*

### Comparing `fuisce-0.0.0/docs/Makefile` & `fuisce-1.0.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `fuisce-0.0.0/docs/make.bat` & `fuisce-1.0.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `fuisce-0.0.0/docs/source/conf.py` & `fuisce-1.0.0/docs/source/conf.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # Configuration file for the Sphinx documentation builder.
 #
 # For the full list of built-in configuration values, see the documentation:
 # https://www.sphinx-doc.org/en/master/usage/configuration.html
 import sys
 from pathlib import Path
 
+
 # -- Project information -----------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#project-information
 
 project = 'Fuisce'
 copyright = '2023, Mitch Negus'
 author = 'Mitch Negus'
 
@@ -16,25 +17,26 @@
 from importlib import metadata
 version = metadata.version('fuisce')
 release = version.split("+")[0]
 
 package_path = Path(__file__).parents[2] / "src/fuisce"
 sys.path.insert(0, str(package_path.absolute()))
 
+
 # -- General configuration ---------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#general-configuration
 
 extensions = [
     'sphinx.ext.autodoc',
     'sphinx.ext.napoleon',
+    'myst_parser',
 ]
 
 templates_path = ['_templates']
 exclude_patterns = []
 
 
-
 # -- Options for HTML output -------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#options-for-html-output
 
 html_theme = 'furo'
 html_static_path = ['_static']
```

### Comparing `fuisce-0.0.0/src/fuisce/database/__init__.py` & `fuisce-1.0.0/src/fuisce/database/interface.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,40 +1,33 @@
 """
-Tools for connecting to and working with the SQLite database.
+An interface for connecting to and working with the SQLite database.
 """
 import functools
 
-from sqlalchemy import create_engine, event
+from flask import current_app
+from sqlalchemy import MetaData, create_engine, event
 from sqlalchemy.engine import Engine
 from sqlalchemy.orm import DeclarativeBase, scoped_session, sessionmaker
 
 DIALECT = "sqlite"
 DBAPI = "pysqlite"
 
 
-class Model(DeclarativeBase):
-    pass
-
-
 class SQLAlchemy:
     """Store an interface to SQLAlchemy database objects."""
 
-    _base = Model
+    metadata = MetaData()
     default_interface = None
 
     def __init__(self, echo_engine=False):
         self.engine = None
         self.scoped_session = None
         self.echo_engine = echo_engine
 
     @property
-    def metadata(self):
-        return self._base.metadata
-
-    @property
     def tables(self):
         return self.metadata.tables
 
     @property
     def session(self):
         # Returns the current `Session` object
         return self.scoped_session()
@@ -55,15 +48,14 @@
         # Use a session factory to generate sessions
         session_factory = sessionmaker(
             bind=self.engine,
             autoflush=False,
             future=True,
         )
         self.scoped_session = scoped_session(session_factory)
-        self._base.query = self.scoped_session.query_property()
 
     def initialize(self, app):
         """
         Initialize the database.
 
         Initialize the database, possibly using any additional arguments
         necessary. This method is designed to be extended by
@@ -142,12 +134,23 @@
             # (otherwise, database initialization is typically executed via the CLI)
             if app.testing:
                 app.db.initialize(app)
 
         return wrapper
 
 
+def db_transaction(func):
+    """A decorator denoting the wrapped function as a database transaction."""
+
+    @functools.wraps(func)
+    def wrapper(*args, **kwargs):
+        with current_app.db.session.begin():
+            return func(*args, **kwargs)
+
+    return wrapper
+
+
 @event.listens_for(Engine, "connect")
 def set_sqlite_pragma(dbapi_connection, connection_record):
     cursor = dbapi_connection.cursor()
     cursor.execute("PRAGMA foreign_keys=ON")
     cursor.close()
```

### Comparing `fuisce-0.0.0/src/fuisce/testing/helpers.py` & `fuisce-1.0.0/src/fuisce/testing/manager.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,36 +1,21 @@
 """
 Helper tools to improve testing of authorized database interactions.
 """
 import functools
 import os
 import tempfile
-import textwrap
 from collections import namedtuple
 from contextlib import contextmanager
-from pprint import pformat
 
 import pytest
-from sqlalchemy import inspect, select
-from sqlalchemy.sql.expression import func
-from werkzeug.exceptions import NotFound
 
-registry = {"app_manager": None}
-
-
-class DefaultTestingConfig:
-    """A Flask configuration designed for testing."""
+from .config import DefaultTestingConfig
 
-    TESTING = True
-    SECRET_KEY = "testing key"
-    DATABASE_INTERFACE_ARGS = ()
-    DATABASE_INTERFACE_KWARGS = {}
-
-    def __init__(self, db_path=None):
-        self.DATABASE = db_path
+registry = {"app_manager": None}
 
 
 class AppTestManager:
     """
     An object for managing apps during testing.
 
     Flask tests require access to an app, and this app provides access
@@ -112,15 +97,16 @@
         app : flask.Flask
             An app instance to be managed by this `AppTestManager`
             object.
         """
         config_kwargs = self._test_config_kwargs | kwargs
         test_config = self._test_config_cls(test_database_path, *args, **config_kwargs)
         app = self._app_factory(test_config)
-        self.setup_test_database(app)
+        if getattr(app, "db", None):
+            self.prepare_test_database(app.db)
         return app
 
     def persistent_context(self):
         return self.app_test_context("persistent_app")
 
     def ephemeral_context(self):
         return self.app_test_context("ephemeral_app")
@@ -156,16 +142,28 @@
         """
         db_fd, db_path = tempfile.mkstemp()
         yield namedtuple("TemporaryFile", ["fd", "path"])(db_fd, db_path)
         # After function execution, close the file and remove it
         os.close(db_fd)
         os.unlink(db_path)
 
-    @staticmethod
-    def setup_test_database(app):
+    def prepare_test_database(self, app):
+        """
+        Set up a database for testing.
+
+        This method prepares a test database (e.g., by preloading data)
+        for use in all tests. The base implementation contains no
+        functionality, and it exists exclusively to be extended by
+        app-specific AppTestManager subclasses.
+
+        Parameters
+        ----------
+        db : SQLAlchemy
+            The app object’s database interface.
+        """
         pass
 
 
 def transaction_lifetime(test_function):
     """
     Create a decorator to use an "ephemeral" app.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `fuisce-0.0.0/.gitignore` & `fuisce-1.0.0/.gitignore`

 * *Files 12% similar despite different names*

```diff
@@ -58,14 +58,15 @@
 *.log
 *.out
 *.synctex.gz
 *.bib
 
 # Sphinx documentation
 docs/_build/
+docs/source/api
 
 # PyBuilder
 target/
 
 # Mac custom attributes file
 .DS_Store
```

### Comparing `fuisce-0.0.0/COPYING` & `fuisce-1.0.0/COPYING`

 * *Files identical despite different names*

### Comparing `fuisce-0.0.0/pyproject.toml` & `fuisce-1.0.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = 'hatchling.build'
 
 [project]
 name = 'fuisce'
 authors = [
     { name = 'Mitch Negus', email = 'mitchnegus57@gmail.com' },
 ]
-description = '...'
+description = 'Database management and testing for SQLAlchemy-based Flask apps.'
 license = { text = 'GNU GPLv3' }
 requires-python = '>=3.9,<3.11'
 dependencies = [
     'flask>=2.2.2',
     'sqlalchemy>=2.0.0',
     'sqlalchemy-views>=0.3.2',
 ]
@@ -30,16 +30,17 @@
 
 [project.urls]
 Download = 'https://pypi.org/project/fuisce'
 Homepage = 'https://github.com/mitchnegus/fuisce'
 Repository = 'https://github.com/mitchnegus/fuisce'
 Changelog = 'https://github.com/mitchnegus/fuisce/blob/main/CHANGELOG.md'
 
+# Set Fuisce as a pytest plugin to use the `AppTestManager` functionality
 [project.entry-points.pytest11]
-fuisce = "fuisce.testing.helpers"
+fuisce = "fuisce.testing.manager"
 
 [tool.hatch.version]
 source = 'vcs'
 
 [tool.hatch.build.targets.wheel]
 packages = [
   'src/fuisce',
@@ -68,15 +69,16 @@
 ]
 pythonpath = ["tests/helpers"]
 norecursedirs = ["tests/helpers"]
 
 [tool.coverage.run]
 omit = [
   'tests/*',
-  'src/fuisce/testing/helpers.py',
+  # Plugin objects are used for testing and are not evaluated well
+  'src/fuisce/testing/*',
 ]
 
 [tool.coverage.report]
 exclude_lines = [
   'raise NotImplementedError',
 ]
```

