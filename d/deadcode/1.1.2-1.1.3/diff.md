# Comparing `tmp/deadcode-1.1.2.tar.gz` & `tmp/deadcode-1.1.3.tar.gz`

## Comparing `deadcode-1.1.2.tar` & `deadcode-1.1.3.tar`

### file list

```diff
@@ -1,29 +1,43 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 deadcode-1.1.2/deadcode/__init__.py
--rw-r--r--   0        0        0     1278 2020-02-02 00:00:00.000000 deadcode-1.1.2/deadcode/cli.py
--rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 deadcode-1.1.2/deadcode/data_types.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 deadcode-1.1.2/deadcode/actions/__init__.py
--rw-r--r--   0        0        0      983 2020-02-02 00:00:00.000000 deadcode-1.1.2/deadcode/actions/find_python_filenames.py
--rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 deadcode-1.1.2/deadcode/actions/find_unused_names.py
--rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 deadcode-1.1.2/deadcode/actions/get_unused_names_error_message.py
--rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 deadcode-1.1.2/deadcode/actions/parse_abstract_syntax_trees.py
--rw-r--r--   0        0        0     3150 2020-02-02 00:00:00.000000 deadcode-1.1.2/deadcode/actions/parse_arguments.py
--rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 deadcode-1.1.2/deadcode/actions/parse_global_names.py
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 deadcode-1.1.2/deadcode/actions/read_files.py
--rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 deadcode-1.1.2/deadcode/tests/base.py
--rw-r--r--   0        0        0     2517 2020-02-02 00:00:00.000000 deadcode-1.1.2/deadcode/tests/test_command_line_argument_parsing.py
--rw-r--r--   0        0        0     3031 2020-02-02 00:00:00.000000 deadcode-1.1.2/deadcode/tests/test_deadcode.py
--rw-r--r--   0        0        0     1373 2020-02-02 00:00:00.000000 deadcode-1.1.2/deadcode/tests/test_ignore_names_by_pattern.py
--rw-r--r--   0        0        0     4109 2020-02-02 00:00:00.000000 deadcode-1.1.2/deadcode/tests/test_output.py
--rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 deadcode-1.1.2/deadcode/tests/files/classes.py
--rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 deadcode-1.1.2/deadcode/tests/files/functions.py
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 deadcode-1.1.2/deadcode/tests/files/variables.py
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 deadcode-1.1.2/deadcode/tests/files/subdir/one_more_file.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 deadcode-1.1.2/deadcode/tests/files/subdir/another_subdir/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 deadcode-1.1.2/deadcode/utils/__init__.py
--rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 deadcode-1.1.2/deadcode/utils/flatten_lists.py
--rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 deadcode-1.1.2/deadcode/utils/path_matching.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 deadcode-1.1.2/.gitignore
--rw-r--r--   0        0        0    34523 2020-02-02 00:00:00.000000 deadcode-1.1.2/LICENSE
--rw-r--r--   0        0        0     2822 2020-02-02 00:00:00.000000 deadcode-1.1.2/README.md
--rw-r--r--   0        0        0     1576 2020-02-02 00:00:00.000000 deadcode-1.1.2/pyproject.toml
--rw-r--r--   0        0        0     3625 2020-02-02 00:00:00.000000 deadcode-1.1.2/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 deadcode-1.1.3/deadcode/__init__.py
+-rw-r--r--   0        0        0     1278 2020-02-02 00:00:00.000000 deadcode-1.1.3/deadcode/cli.py
+-rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 deadcode-1.1.3/deadcode/data_types.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 deadcode-1.1.3/deadcode/actions/__init__.py
+-rw-r--r--   0        0        0      983 2020-02-02 00:00:00.000000 deadcode-1.1.3/deadcode/actions/find_python_filenames.py
+-rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 deadcode-1.1.3/deadcode/actions/find_unused_names.py
+-rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 deadcode-1.1.3/deadcode/actions/get_unused_names_error_message.py
+-rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 deadcode-1.1.3/deadcode/actions/parse_abstract_syntax_trees.py
+-rw-r--r--   0        0        0     3150 2020-02-02 00:00:00.000000 deadcode-1.1.3/deadcode/actions/parse_arguments.py
+-rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 deadcode-1.1.3/deadcode/actions/parse_global_names.py
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 deadcode-1.1.3/deadcode/actions/read_files.py
+-rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 deadcode-1.1.3/deadcode/tests/base.py
+-rw-r--r--   0        0        0     2517 2020-02-02 00:00:00.000000 deadcode-1.1.3/deadcode/tests/test_command_line_argument_parsing.py
+-rw-r--r--   0        0        0     3031 2020-02-02 00:00:00.000000 deadcode-1.1.3/deadcode/tests/test_deadcode.py
+-rw-r--r--   0        0        0     1373 2020-02-02 00:00:00.000000 deadcode-1.1.3/deadcode/tests/test_ignore_names_by_pattern.py
+-rw-r--r--   0        0        0     4109 2020-02-02 00:00:00.000000 deadcode-1.1.3/deadcode/tests/test_output.py
+-rw-r--r--   0        0        0     4693 2020-02-02 00:00:00.000000 deadcode-1.1.3/deadcode/tests/test_parse_variables_with_scopes.py
+-rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 deadcode-1.1.3/deadcode/tests/files/classes.py
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 deadcode-1.1.3/deadcode/tests/files/functions.py
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 deadcode-1.1.3/deadcode/tests/files/variables.py
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 deadcode-1.1.3/deadcode/tests/files/subdir/one_more_file.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 deadcode-1.1.3/deadcode/tests/files/subdir/another_subdir/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 deadcode-1.1.3/deadcode/utils/__init__.py
+-rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 deadcode-1.1.3/deadcode/utils/flatten_lists.py
+-rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 deadcode-1.1.3/deadcode/utils/path_matching.py
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 deadcode-1.1.3/tmp/__init__.py
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 deadcode-1.1.3/tmp/foo.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 deadcode-1.1.3/tmp/sound/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 deadcode-1.1.3/tmp/sound/effects/__init__.py
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 deadcode-1.1.3/tmp/sound/effects/echo.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 deadcode-1.1.3/tmp/sound/filters/__init__.py
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 deadcode-1.1.3/tmp/sound/filters/equalizer.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 deadcode-1.1.3/tmp/sound/formats/__init__.py
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 deadcode-1.1.3/tmp/sound/formats/wavread.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 deadcode-1.1.3/tmp/spam/__init__.py
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 deadcode-1.1.3/tmp/spam/bar.py
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 deadcode-1.1.3/tmp/vulture/code/foo.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 deadcode-1.1.3/tmp/vulture/code/settings.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 deadcode-1.1.3/.gitignore
+-rw-r--r--   0        0        0    34523 2020-02-02 00:00:00.000000 deadcode-1.1.3/LICENSE
+-rw-r--r--   0        0        0     3116 2020-02-02 00:00:00.000000 deadcode-1.1.3/README.md
+-rw-r--r--   0        0        0     1595 2020-02-02 00:00:00.000000 deadcode-1.1.3/pyproject.toml
+-rw-r--r--   0        0        0     3947 2020-02-02 00:00:00.000000 deadcode-1.1.3/PKG-INFO
```

### Comparing `deadcode-1.1.2/deadcode/cli.py` & `deadcode-1.1.3/deadcode/cli.py`

 * *Files identical despite different names*

### Comparing `deadcode-1.1.2/deadcode/actions/find_python_filenames.py` & `deadcode-1.1.3/deadcode/actions/find_python_filenames.py`

 * *Files identical despite different names*

### Comparing `deadcode-1.1.2/deadcode/actions/find_unused_names.py` & `deadcode-1.1.3/deadcode/actions/find_unused_names.py`

 * *Files identical despite different names*

### Comparing `deadcode-1.1.2/deadcode/actions/get_unused_names_error_message.py` & `deadcode-1.1.3/deadcode/actions/get_unused_names_error_message.py`

 * *Files identical despite different names*

### Comparing `deadcode-1.1.2/deadcode/actions/parse_abstract_syntax_trees.py` & `deadcode-1.1.3/deadcode/actions/parse_abstract_syntax_trees.py`

 * *Files identical despite different names*

### Comparing `deadcode-1.1.2/deadcode/actions/parse_arguments.py` & `deadcode-1.1.3/deadcode/actions/parse_arguments.py`

 * *Files identical despite different names*

### Comparing `deadcode-1.1.2/deadcode/actions/parse_global_names.py` & `deadcode-1.1.3/deadcode/actions/parse_global_names.py`

 * *Files identical despite different names*

### Comparing `deadcode-1.1.2/deadcode/tests/test_command_line_argument_parsing.py` & `deadcode-1.1.3/deadcode/tests/test_command_line_argument_parsing.py`

 * *Files identical despite different names*

### Comparing `deadcode-1.1.2/deadcode/tests/test_deadcode.py` & `deadcode-1.1.3/deadcode/tests/test_deadcode.py`

 * *Files identical despite different names*

### Comparing `deadcode-1.1.2/deadcode/tests/test_ignore_names_by_pattern.py` & `deadcode-1.1.3/deadcode/tests/test_ignore_names_by_pattern.py`

 * *Files identical despite different names*

### Comparing `deadcode-1.1.2/deadcode/tests/test_output.py` & `deadcode-1.1.3/deadcode/tests/test_output.py`

 * *Files identical despite different names*

### Comparing `deadcode-1.1.2/deadcode/utils/flatten_lists.py` & `deadcode-1.1.3/deadcode/utils/flatten_lists.py`

 * *Files identical despite different names*

### Comparing `deadcode-1.1.2/.gitignore` & `deadcode-1.1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `deadcode-1.1.2/LICENSE` & `deadcode-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `deadcode-1.1.2/README.md` & `deadcode-1.1.3/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -58,7 +58,12 @@
 If the same unused name is repeated in several files - it wont be detected.
 
 Files with syntax errors will be ignored, because `deadcode` uses `ast` to
 build abstract syntax tree for name usage detection.
 
 It is assumed that `deadcode` will be run using the same Python version as the
 checked code base is implemented in.
+
+## Feature requests
+[ ] Split error codes into DC100, DC200, DC300 for variables, functions, class. It will be possible to disable each check separately.
+[ ] Add unused class method detection DC310 check.
+[ ] Add target python version option, if specified it will be used for code base check.
```

### Comparing `deadcode-1.1.2/pyproject.toml` & `deadcode-1.1.3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "deadcode"
-version = "1.1.2"
+version = "1.1.3"
 authors = [
     {name = "Albertas Gimbutas", email = "albertasgim@gmail.com"},
 ]
 description = "Find and remove dead code."
 readme = "README.md"
 requires-python = ">= 3.8"
 classifiers = [
@@ -15,14 +15,15 @@
     "Programming Language :: Python",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
 dependencies = [
+    "tomli==2.0.1"
 ]
 
 [project.scripts]
 deadcode = "deadcode.cli:main"
 
 [project.urls]
 Homepage = "https://github.com/albertas/deadcode"
@@ -65,8 +66,8 @@
 [tool.black]
 max_line_length = 120
 line_length = 120
 target_version = ["py38"]
 
 
 [tool.pytest.ini_options]
-addopts = "--cov=. --cov-fail-under=92.0"
+addopts = "--cov=. --cov-fail-under=93.0"
```

### Comparing `deadcode-1.1.2/PKG-INFO` & `deadcode-1.1.3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deadcode
-Version: 1.1.2
+Version: 1.1.3
 Summary: Find and remove dead code.
 Project-URL: Homepage, https://github.com/albertas/deadcode
 Project-URL: Documentation, https://deadcode.readthedocs.io/
 Author-email: Albertas Gimbutas <albertasgim@gmail.com>
 License-File: LICENSE
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
@@ -12,14 +12,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
+Requires-Dist: tomli==2.0.1
 Description-Content-Type: text/markdown
 
 # deadcode
 `deadcode` package implements `DC100` - `unused-global-name` check for detecting
 variable/function/class names which are never used in a whole code base.
 Only globally defined names are being checked.
 Unused local names can be detected by other tools like [ruff](https://pypi.org/project/ruff/).
@@ -78,7 +79,12 @@
 If the same unused name is repeated in several files - it wont be detected.
 
 Files with syntax errors will be ignored, because `deadcode` uses `ast` to
 build abstract syntax tree for name usage detection.
 
 It is assumed that `deadcode` will be run using the same Python version as the
 checked code base is implemented in.
+
+## Feature requests
+[ ] Split error codes into DC100, DC200, DC300 for variables, functions, class. It will be possible to disable each check separately.
+[ ] Add unused class method detection DC310 check.
+[ ] Add target python version option, if specified it will be used for code base check.
```

