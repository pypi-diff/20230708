# Comparing `tmp/crackerjack-0.3.5.tar.gz` & `tmp/crackerjack-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crackerjack-0.3.5.tar", last modified: Fri Jul  7 13:14:10 2023, max compression
+gzip compressed data, was "crackerjack-0.3.6.tar", last modified: Sat Jul  8 10:46:01 2023, max compression
```

## Comparing `crackerjack-0.3.5.tar` & `crackerjack-0.3.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1531 2023-04-13 18:37:22.056785 crackerjack-0.3.5/LICENSE
--rw-r--r--   0        0        0     5917 2023-06-18 16:33:36.904528 crackerjack-0.3.5/README.md
--rw-r--r--   0        0        0        0 2023-07-07 13:13:51.723700 crackerjack-0.3.5/crackerjack/.crackerjack-config.yaml
--rw-r--r--   0        0        0      229 2023-07-07 13:13:51.674755 crackerjack-0.3.5/crackerjack/.gitignore
--rw-r--r--   0        0        0      768 2023-07-07 13:13:51.707759 crackerjack-0.3.5/crackerjack/.libcst.codemod.yaml
--rw-r--r--   0        0        0     2917 2023-07-07 13:13:51.692103 crackerjack-0.3.5/crackerjack/.pre-commit-config.yaml
--rw-r--r--   0        0        0    15547 2023-06-18 10:35:54.994502 crackerjack-0.3.5/crackerjack/.pyanalyze-report.json
--rw-r--r--   0        0        0     8180 2023-06-18 10:35:54.997907 crackerjack-0.3.5/crackerjack/.pyanalyze-report.md
--rw-r--r--   0        0        0        1 2023-04-26 10:06:29.859090 crackerjack-0.3.5/crackerjack/.ruff_cache/.gitignore
--rw-r--r--   0        0        0       43 2023-04-26 10:06:29.858981 crackerjack-0.3.5/crackerjack/.ruff_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      121 2023-04-25 19:43:53.234903 crackerjack-0.3.5/crackerjack/__init__.py
--rw-r--r--   0        0        0     1559 2023-07-07 13:10:39.683493 crackerjack-0.3.5/crackerjack/__main__.py
--rw-r--r--   0        0        0     6145 2023-06-19 10:49:19.257226 crackerjack-0.3.5/crackerjack/crackerjack.py
--rw-r--r--   0        0        0     1659 2023-07-07 13:13:52.445350 crackerjack-0.3.5/crackerjack/pyproject.toml
--rw-r--r--   0        0        0     2010 2023-07-07 13:14:10.111259 crackerjack-0.3.5/pyproject.toml
--rw-r--r--   0        0        0     6910 1970-01-01 00:00:00.000000 crackerjack-0.3.5/PKG-INFO
+-rw-r--r--   0        0        0     1531 2023-04-13 18:37:22.056785 crackerjack-0.3.6/LICENSE
+-rw-r--r--   0        0        0     5917 2023-06-18 16:33:36.904528 crackerjack-0.3.6/README.md
+-rw-r--r--   0        0        0        0 2023-07-08 10:08:28.778621 crackerjack-0.3.6/crackerjack/.crackerjack-config.yaml
+-rw-r--r--   0        0        0      255 2023-07-08 10:08:28.722503 crackerjack-0.3.6/crackerjack/.gitignore
+-rw-r--r--   0        0        0      768 2023-07-08 10:08:28.763421 crackerjack-0.3.6/crackerjack/.libcst.codemod.yaml
+-rw-r--r--   0        0        0     2917 2023-07-08 10:08:28.745489 crackerjack-0.3.6/crackerjack/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    15547 2023-06-18 10:35:54.994502 crackerjack-0.3.6/crackerjack/.pyanalyze-report.json
+-rw-r--r--   0        0        0     8180 2023-06-18 10:35:54.997907 crackerjack-0.3.6/crackerjack/.pyanalyze-report.md
+-rw-r--r--   0        0        0        1 2023-04-26 10:06:29.859090 crackerjack-0.3.6/crackerjack/.ruff_cache/.gitignore
+-rw-r--r--   0        0        0       43 2023-04-26 10:06:29.858981 crackerjack-0.3.6/crackerjack/.ruff_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      121 2023-04-25 19:43:53.234903 crackerjack-0.3.6/crackerjack/__init__.py
+-rw-r--r--   0        0        0     1559 2023-07-07 13:10:39.683493 crackerjack-0.3.6/crackerjack/__main__.py
+-rw-r--r--   0        0        0     6157 2023-07-08 10:44:25.772068 crackerjack-0.3.6/crackerjack/crackerjack.py
+-rw-r--r--   0        0        0     1659 2023-07-08 10:08:29.586215 crackerjack-0.3.6/crackerjack/pyproject.toml
+-rw-r--r--   0        0        0     2010 2023-07-08 10:46:01.423860 crackerjack-0.3.6/pyproject.toml
+-rw-r--r--   0        0        0     6910 1970-01-01 00:00:00.000000 crackerjack-0.3.6/PKG-INFO
```

### Comparing `crackerjack-0.3.5/LICENSE` & `crackerjack-0.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `crackerjack-0.3.5/README.md` & `crackerjack-0.3.6/README.md`

 * *Files identical despite different names*

### Comparing `crackerjack-0.3.5/crackerjack/.libcst.codemod.yaml` & `crackerjack-0.3.6/crackerjack/.libcst.codemod.yaml`

 * *Files identical despite different names*

### Comparing `crackerjack-0.3.5/crackerjack/.pre-commit-config.yaml` & `crackerjack-0.3.6/crackerjack/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `crackerjack-0.3.5/crackerjack/.pyanalyze-report.json` & `crackerjack-0.3.6/crackerjack/.pyanalyze-report.json`

 * *Files identical despite different names*

### Comparing `crackerjack-0.3.5/crackerjack/.pyanalyze-report.md` & `crackerjack-0.3.6/crackerjack/.pyanalyze-report.md`

 * *Files identical despite different names*

### Comparing `crackerjack-0.3.5/crackerjack/__main__.py` & `crackerjack-0.3.6/crackerjack/__main__.py`

 * *Files identical despite different names*

### Comparing `crackerjack-0.3.5/crackerjack/crackerjack.py` & `crackerjack-0.3.6/crackerjack/crackerjack.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from aiopath import AsyncPath
 from inflection import underscore
 from pydantic import BaseModel
 from pydantic import ConfigDict
 
 
 class Crakerjack(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True)
+    model_config: ConfigDict = ConfigDict(arbitrary_types_allowed=True)
     our_path: AsyncPath = AsyncPath(__file__)
     pkg_path: AsyncPath = AsyncPath.cwd()
     pkg_dir: t.Optional[AsyncPath] = None
     pkg_name: str = "crackerjack"
     our_toml: t.Optional[dict] = None
     pkg_toml: t.Optional[dict] = None
     our_toml_path: t.Optional[AsyncPath] = None
```

### Comparing `crackerjack-0.3.5/crackerjack/pyproject.toml` & `crackerjack-0.3.6/crackerjack/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 ]
 reportMissingImports = true
 reportMissingTypeStubs = false
 pythonVersion = "3.11"
 
 [project]
 name = "Crackerjack"
-version = "0.3.5"
+version = "0.3.6"
 description = "Crackerjack code style"
 requires-python = ">=3.11"
 readme = "README.md"
 keywords = [
     "black",
     "ruff",
     "mypy",
```

### Comparing `crackerjack-0.3.5/pyproject.toml` & `crackerjack-0.3.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -59,15 +59,15 @@
 ]
 reportMissingImports = true
 reportMissingTypeStubs = false
 pythonVersion = "3.11"
 
 [project]
 name = "Crackerjack"
-version = "0.3.5"
+version = "0.3.6"
 description = "Crackerjack code style"
 requires-python = ">=3.11"
 readme = "README.md"
 keywords = [
     "black",
     "ruff",
     "mypy",
```

### Comparing `crackerjack-0.3.5/PKG-INFO` & `crackerjack-0.3.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Crackerjack
-Version: 0.3.5
+Version: 0.3.6
 Summary: Crackerjack code style
 Keywords: black ruff mypy creosote refurb
 Home-page: https://github.com/lesleslie/crackerjack
 Author-Email: lesleslie <les@wedgwoodwebworks.com>
 Maintainer-Email: lesleslie <les@wedgwoodwebworks.com>
 License: BSD-3-Clause
 Classifier: Environment :: Console
```

