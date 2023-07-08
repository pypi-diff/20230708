# Comparing `tmp/atomlite-1.3.1.tar.gz` & `tmp/atomlite-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atomlite-1.3.1.tar", last modified: Thu Jul  6 10:37:48 2023, max compression
+gzip compressed data, was "atomlite-1.3.2.tar", last modified: Sat Jul  8 10:18:25 2023, max compression
```

## Comparing `atomlite-1.3.1.tar` & `atomlite-1.3.2.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:37:48.787756 atomlite-1.3.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:37:48.783756 atomlite-1.3.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:37:48.783756 atomlite-1.3.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-07-06 10:37:05.000000 atomlite-1.3.1/.github/workflows/publish_release.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-07-06 10:37:05.000000 atomlite-1.3.1/.github/workflows/tests.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-06 10:37:05.000000 atomlite-1.3.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-06 10:37:05.000000 atomlite-1.3.1/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-07-06 10:37:48.787756 atomlite-1.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-07-06 10:37:05.000000 atomlite-1.3.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:37:48.783756 atomlite-1.3.1/docker_testing_environment/
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-07-06 10:37:05.000000 atomlite-1.3.1/docker_testing_environment/Dockerfile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:37:48.783756 atomlite-1.3.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-07-06 10:37:05.000000 atomlite-1.3.1/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:37:48.787756 atomlite-1.3.1/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:37:48.787756 atomlite-1.3.1/docs/source/_static/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 10:37:05.000000 atomlite-1.3.1/docs/source/_static/empty
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:37:48.787756 atomlite-1.3.1/docs/source/_templates/
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-07-06 10:37:05.000000 atomlite-1.3.1/docs/source/_templates/class.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-07-06 10:37:05.000000 atomlite-1.3.1/docs/source/_templates/module.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-07-06 10:37:05.000000 atomlite-1.3.1/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)    12883 2023-07-06 10:37:05.000000 atomlite-1.3.1/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-06 10:37:05.000000 atomlite-1.3.1/docs/source/modules.rst
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-07-06 10:37:05.000000 atomlite-1.3.1/justfile
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-07-06 10:37:05.000000 atomlite-1.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 10:37:48.787756 atomlite-1.3.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:37:48.783756 atomlite-1.3.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:37:48.787756 atomlite-1.3.1/src/atomlite/
--rw-r--r--   0 runner    (1001) docker     (123)      473 2023-07-06 10:37:05.000000 atomlite-1.3.1/src/atomlite/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:37:48.787756 atomlite-1.3.1/src/atomlite/_internal/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 10:37:05.000000 atomlite-1.3.1/src/atomlite/_internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11418 2023-07-06 10:37:05.000000 atomlite-1.3.1/src/atomlite/_internal/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     5639 2023-07-06 10:37:05.000000 atomlite-1.3.1/src/atomlite/_internal/json.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 10:37:05.000000 atomlite-1.3.1/src/atomlite/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:37:48.787756 atomlite-1.3.1/src/atomlite.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-07-06 10:37:48.000000 atomlite-1.3.1/src/atomlite.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-07-06 10:37:48.000000 atomlite-1.3.1/src/atomlite.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 10:37:48.000000 atomlite-1.3.1/src/atomlite.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-06 10:37:48.000000 atomlite-1.3.1/src/atomlite.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-06 10:37:48.000000 atomlite-1.3.1/src/atomlite.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:37:48.787756 atomlite-1.3.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    10139 2023-07-06 10:37:05.000000 atomlite-1.3.1/tests/test_database.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 10:18:25.506720 atomlite-1.3.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 10:18:25.506720 atomlite-1.3.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 10:18:25.506720 atomlite-1.3.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-07-08 10:17:48.000000 atomlite-1.3.2/.github/workflows/publish_release.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-07-08 10:17:48.000000 atomlite-1.3.2/.github/workflows/tests.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-08 10:17:48.000000 atomlite-1.3.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-08 10:17:48.000000 atomlite-1.3.2/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-07-08 10:18:25.506720 atomlite-1.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-07-08 10:17:48.000000 atomlite-1.3.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 10:18:25.506720 atomlite-1.3.2/docker_testing_environment/
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-07-08 10:17:48.000000 atomlite-1.3.2/docker_testing_environment/Dockerfile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 10:18:25.506720 atomlite-1.3.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-07-08 10:17:48.000000 atomlite-1.3.2/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 10:18:25.506720 atomlite-1.3.2/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 10:18:25.506720 atomlite-1.3.2/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 10:17:48.000000 atomlite-1.3.2/docs/source/_static/empty
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 10:18:25.506720 atomlite-1.3.2/docs/source/_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-07-08 10:17:48.000000 atomlite-1.3.2/docs/source/_templates/class.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-07-08 10:17:48.000000 atomlite-1.3.2/docs/source/_templates/module.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-07-08 10:17:48.000000 atomlite-1.3.2/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12883 2023-07-08 10:17:48.000000 atomlite-1.3.2/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-08 10:17:48.000000 atomlite-1.3.2/docs/source/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-07-08 10:17:48.000000 atomlite-1.3.2/justfile
+-rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-07-08 10:17:48.000000 atomlite-1.3.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 10:18:25.506720 atomlite-1.3.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 10:18:25.506720 atomlite-1.3.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 10:18:25.506720 atomlite-1.3.2/src/atomlite/
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-07-08 10:17:48.000000 atomlite-1.3.2/src/atomlite/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 10:18:25.506720 atomlite-1.3.2/src/atomlite/_internal/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 10:17:48.000000 atomlite-1.3.2/src/atomlite/_internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11440 2023-07-08 10:17:48.000000 atomlite-1.3.2/src/atomlite/_internal/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5633 2023-07-08 10:17:48.000000 atomlite-1.3.2/src/atomlite/_internal/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 10:17:48.000000 atomlite-1.3.2/src/atomlite/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 10:18:25.506720 atomlite-1.3.2/src/atomlite.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-07-08 10:18:25.000000 atomlite-1.3.2/src/atomlite.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-07-08 10:18:25.000000 atomlite-1.3.2/src/atomlite.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 10:18:25.000000 atomlite-1.3.2/src/atomlite.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-08 10:18:25.000000 atomlite-1.3.2/src/atomlite.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-08 10:18:25.000000 atomlite-1.3.2/src/atomlite.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 10:18:25.506720 atomlite-1.3.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    10179 2023-07-08 10:17:48.000000 atomlite-1.3.2/tests/test_database.py
```

### Comparing `atomlite-1.3.1/.github/workflows/publish_release.yaml` & `atomlite-1.3.2/.github/workflows/publish_release.yaml`

 * *Files identical despite different names*

### Comparing `atomlite-1.3.1/.github/workflows/tests.yaml` & `atomlite-1.3.2/.github/workflows/tests.yaml`

 * *Files identical despite different names*

### Comparing `atomlite-1.3.1/PKG-INFO` & `atomlite-1.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atomlite
-Version: 1.3.1
+Version: 1.3.2
 Maintainer-email: Lukas Turcani <lukasturcani93@gmail.com>
 Project-URL: github, https://github.com/lukasturcani/atomlite
 Project-URL: documentation, https://atomlite.readthedocs.io
 Requires-Python: >=3.11
 Description-Content-Type: text/x-rst
 Provides-Extra: dev
```

### Comparing `atomlite-1.3.1/README.rst` & `atomlite-1.3.2/README.rst`

 * *Files identical despite different names*

### Comparing `atomlite-1.3.1/docs/Makefile` & `atomlite-1.3.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `atomlite-1.3.1/docs/source/_templates/class.rst` & `atomlite-1.3.2/docs/source/_templates/class.rst`

 * *Files identical despite different names*

### Comparing `atomlite-1.3.1/docs/source/_templates/module.rst` & `atomlite-1.3.2/docs/source/_templates/module.rst`

 * *Files identical despite different names*

### Comparing `atomlite-1.3.1/docs/source/conf.py` & `atomlite-1.3.2/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `atomlite-1.3.1/docs/source/index.rst` & `atomlite-1.3.2/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `atomlite-1.3.1/justfile` & `atomlite-1.3.2/justfile`

 * *Files identical despite different names*

### Comparing `atomlite-1.3.1/pyproject.toml` & `atomlite-1.3.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -57,13 +57,14 @@
 warn_no_return = true
 strict_optional = true
 disallow_untyped_defs = true
 disallow_incomplete_defs = true
 check_untyped_defs = true
 disallow_untyped_decorators = true
 warn_unreachable = true
+disallow_any_generics = true
 
 [[tool.mypy.overrides]]
 module = [
   "rdkit.*"
 ]
 ignore_missing_imports = true
```

### Comparing `atomlite-1.3.1/src/atomlite/_internal/database.py` & `atomlite-1.3.2/src/atomlite/_internal/database.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,15 +52,15 @@
             The entry.
         """
         if properties is None:
             properties = {}
         return Entry(key, json_from_rdkit(molecule), properties)
 
 
-def _entry_to_sqlite(entry: Entry) -> dict:
+def _entry_to_sqlite(entry: Entry) -> dict[str, Json]:
     d = asdict(entry)
     d["molecule"] = json.dumps(d["molecule"])
     d["properties"] = json.dumps(d["properties"])
     return d
 
 
 @dataclass(frozen=True, slots=True)
@@ -75,15 +75,15 @@
 
     key: str
     """Key used to uniquely identify the molecule."""
     properties: "dict[str, Json]"
     """User-defined molecular properties."""
 
 
-def _property_entry_to_sqlite(entry: PropertyEntry) -> dict:
+def _property_entry_to_sqlite(entry: PropertyEntry) -> dict[str, Json]:
     d = asdict(entry)
     d["properties"] = json.dumps(d["properties"])
     return d
 
 
 class MoleculeNotFound(Exception):
     """
```

### Comparing `atomlite-1.3.1/src/atomlite/_internal/json.py` & `atomlite-1.3.2/src/atomlite/_internal/json.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import typing
 
 import rdkit.Chem as rdkit
 
 Json: typing.TypeAlias = (
-    bool | int | float | str | None | list["Json"] | dict[str, "Json"]
+    bool | float | str | None | list["Json"] | dict[str, "Json"]
 )
 Conformer: typing.TypeAlias = list[list[float]]
 
 
 class Bonds(typing.TypedDict):
     """
     JSON representation of bonds.
```

### Comparing `atomlite-1.3.1/src/atomlite.egg-info/PKG-INFO` & `atomlite-1.3.2/src/atomlite.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atomlite
-Version: 1.3.1
+Version: 1.3.2
 Maintainer-email: Lukas Turcani <lukasturcani93@gmail.com>
 Project-URL: github, https://github.com/lukasturcani/atomlite
 Project-URL: documentation, https://atomlite.readthedocs.io
 Requires-Python: >=3.11
 Description-Content-Type: text/x-rst
 Provides-Extra: dev
```

### Comparing `atomlite-1.3.1/src/atomlite.egg-info/SOURCES.txt` & `atomlite-1.3.2/src/atomlite.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `atomlite-1.3.1/tests/test_database.py` & `atomlite-1.3.2/tests/test_database.py`

 * *Files 0% similar despite different names*

```diff
@@ -236,16 +236,16 @@
     ):
         assert atom1.GetTotalNumHs() == atom2.GetTotalNumHs()
         assert atom1.GetNumExplicitHs() == atom2.GetNumExplicitHs()
         assert atom1.GetNumImplicitHs() == atom2.GetNumImplicitHs()
 
 
 def _assert_properties_match(
-    expected: dict | None,
-    actual: dict | None,
+    expected: dict[str, atomlite.Json] | None,
+    actual: dict[str, atomlite.Json] | None,
 ) -> None:
     assert json.dumps(expected) == json.dumps(actual)
 
 
 def _embed_molecule(molecule: rdkit.Mol) -> rdkit.Mol:
     rdkit.EmbedMultipleConfs(molecule, 10, rdkit.ETKDGv3())
     return molecule
```

