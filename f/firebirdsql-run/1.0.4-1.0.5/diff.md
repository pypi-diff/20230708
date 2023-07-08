# Comparing `tmp/firebirdsql_run-1.0.4.tar.gz` & `tmp/firebirdsql_run-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "firebirdsql_run-1.0.4.tar", max compression
+gzip compressed data, was "firebirdsql_run-1.0.5.tar", max compression
```

## Comparing `firebirdsql_run-1.0.4.tar` & `firebirdsql_run-1.0.5.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1065 2023-05-30 19:49:31.605746 firebirdsql_run-1.0.4/LICENSE
--rw-r--r--   0        0        0     2152 2023-05-30 19:49:31.605746 firebirdsql_run-1.0.4/README.md
--rw-r--r--   0        0        0     2239 2023-05-30 19:49:44.869787 firebirdsql_run-1.0.4/pyproject.toml
--rw-r--r--   0        0        0      241 2023-05-30 19:49:31.605746 firebirdsql_run-1.0.4/src/firebirdsql_run/__init__.py
--rw-r--r--   0        0        0     2851 2023-05-30 19:49:31.605746 firebirdsql_run-1.0.4/src/firebirdsql_run/main.py
--rw-r--r--   0        0        0      429 2023-05-30 19:49:31.605746 firebirdsql_run-1.0.4/src/firebirdsql_run/type.py
--rw-r--r--   0        0        0      357 2023-05-30 19:49:31.605746 firebirdsql_run-1.0.4/src/firebirdsql_run/util.py
--rw-r--r--   0        0        0     2877 1970-01-01 00:00:00.000000 firebirdsql_run-1.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-07-08 11:18:43.999279 firebirdsql_run-1.0.5/LICENSE
+-rw-r--r--   0        0        0     2152 2023-07-08 11:18:43.999279 firebirdsql_run-1.0.5/README.md
+-rw-r--r--   0        0        0     2295 2023-07-08 11:19:00.471922 firebirdsql_run-1.0.5/pyproject.toml
+-rw-r--r--   0        0        0      241 2023-07-08 11:18:43.999279 firebirdsql_run-1.0.5/src/firebirdsql_run/__init__.py
+-rw-r--r--   0        0        0     2807 2023-07-08 11:18:43.999279 firebirdsql_run-1.0.5/src/firebirdsql_run/main.py
+-rw-r--r--   0        0        0      521 2023-07-08 11:18:43.999279 firebirdsql_run-1.0.5/src/firebirdsql_run/type.py
+-rw-r--r--   0        0        0      357 2023-07-08 11:18:43.999279 firebirdsql_run-1.0.5/src/firebirdsql_run/util.py
+-rw-r--r--   0        0        0     2877 1970-01-01 00:00:00.000000 firebirdsql_run-1.0.5/PKG-INFO
```

### Comparing `firebirdsql_run-1.0.4/LICENSE` & `firebirdsql_run-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `firebirdsql_run-1.0.4/README.md` & `firebirdsql_run-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `firebirdsql_run-1.0.4/pyproject.toml` & `firebirdsql_run-1.0.5/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning"]
 build-backend = "poetry_dynamic_versioning.backend"
 
 [tool.poetry]
 name = "firebirdsql-run"
-version = "1.0.4"
+version = "1.0.5"
 description = "Firebirdsql wrapper inspired by subprocess.run"
 authors = ["DeadNews <aurczpbgr@mozmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/DeadNews/firebirdsql-run"
 repository = "https://github.com/DeadNews/firebirdsql-run"
 keywords = ["firebird", "sql", "api"]
@@ -16,21 +16,21 @@
 
 [tool.poetry.dependencies]
 python = "^3.10"
 firebirdsql = "^1.2.2"
 
 [tool.poetry.group.lint.dependencies]
 black = "^23.3.0"
-mypy = "^1.2.0"
+mypy = "^1.4.1"
 poethepoet = "^0.20.0"
-ruff = "^0.0.270"
+ruff = "^0.0.275"
 
 [tool.poetry.group.test.dependencies]
-pytest = "^7.3.1"
-pytest-cov = "^4.0.0"
+pytest = "^7.4.0"
+pytest-cov = "^4.1.0"
 
 [tool.poe.tasks]
 ruff = "ruff check ."
 black = "black --check ."
 mypy = "mypy ."
 lint.sequence = ["ruff", "black", "mypy"]
 
@@ -56,34 +56,36 @@
 
 [tool.pytest.ini_options]
 addopts = "--verbose --cov=./src"
 testpaths = ["tests"]
 markers = ["docker", "key_required"]
 
 [tool.coverage.report]
-exclude_lines = ["if TYPE_CHECKING:", "if __name__ == .__main__.:"]
+exclude_lines = [
+  "# pragma: no cover",
+  "if __name__ == .__main__.:",
+  "if TYPE_CHECKING:",
+]
 
 [tool.ruff]
 line-length = 99
 select = ["ALL"]
 ignore = [
-  "COM812", # Trailing comma missing
-  "D203",   # 1 blank line required before class docstring
-  "D212",   # Multi-line docstring summary should start at the first line
-  "E501",   # Line too long
-  "EXE001", # Shebang is present but file is not executable
-  "FBT001", # Boolean positional arg in function definition
-  "FBT002", # Boolean default value in function definition
+  "COM812",  # Trailing comma missing
+  "D203",    # 1 blank line required before class docstring
+  "D212",    # Multi-line docstring summary should start at the first line
+  "E501",    # Line too long
+  "EXE001",  # Shebang is present but file is not executable
+  "FBT001",  # Boolean positional arg in function definition
+  "FBT002",  # Boolean default value in function definition
+  "PLR0913", # Too many arguments to function call
 ]
 
 [tool.ruff.per-file-ignores]
 "__init__.py" = ["F401"]
 "tests/*" = ["ANN", "D", "PLC1901", "PLR2004", "S"]
 
 [tool.ruff.flake8-comprehensions]
 allow-dict-calls-with-keyword-arguments = false
 
 [tool.ruff.flake8-tidy-imports]
 ban-relative-imports = "all"
-
-[tool.ruff.pylint]
-max-args = 8
```

### Comparing `firebirdsql_run-1.0.4/src/firebirdsql_run/main.py` & `firebirdsql_run-1.0.5/src/firebirdsql_run/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,18 +5,14 @@
 
 from firebirdsql import Connection, connect
 
 from firebirdsql_run.type import CompletedTransaction
 from firebirdsql_run.util import get_env
 
 
-class ExecuteError(Exception):
-    """Exception raised for execute transaction errors."""
-
-
 def connection(
     db: Path | str,
     host: str = "localhost",
     port: int = 3050,
     user: str = "TWUSER",
     passwd: str | None = None,
 ) -> Connection:
@@ -54,31 +50,31 @@
             connection(host=host, db=db, port=port, user=user, passwd=passwd)
             if use_conn is None
             else use_conn
         )
         conn_success = True
 
         cur = conn.cursor()
-
         cur.execute(query=query, params=params)
 
         lines = cur.fetchall()
         columns = [f"{col[0]}".lower() for col in cur.description]
-        conn.commit()
-
-        if use_conn is None:
-            conn.close()
     except Exception as e:  # noqa: BLE001
         data = []
         returncode = 1
         error = f"{e}"
     else:
         data = [dict(zip(columns, line, strict=True)) for line in lines]
         returncode = 0
         error = ""
+    finally:
+        if conn_success:
+            conn.commit()
+            if use_conn is None:
+                conn.close()
 
     return CompletedTransaction(
         host=conn.hostname if conn_success else host,
         db=conn.filename if conn_success else db,
         user=conn.user if conn_success else user,
         returncode=returncode,
         error=error,
```

### Comparing `firebirdsql_run-1.0.4/PKG-INFO` & `firebirdsql_run-1.0.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: firebirdsql-run
-Version: 1.0.4
+Version: 1.0.5
 Summary: Firebirdsql wrapper inspired by subprocess.run
 Home-page: https://github.com/DeadNews/firebirdsql-run
 License: MIT
 Keywords: firebird,sql,api
 Author: DeadNews
 Author-email: aurczpbgr@mozmail.com
 Requires-Python: >=3.10,<4.0
```

