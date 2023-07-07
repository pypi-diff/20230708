# Comparing `tmp/pyprojectsort-0.2.1.tar.gz` & `tmp/pyprojectsort-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyprojectsort-0.2.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "pyprojectsort-0.2.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `pyprojectsort-0.2.1.tar` & `pyprojectsort-0.2.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     3098 2023-07-05 19:46:27.094709 pyprojectsort-0.2.1/README.md
--rw-r--r--   0        0        0     2034 2023-07-05 19:46:27.094709 pyprojectsort-0.2.1/pyproject.toml
--rw-r--r--   0        0        0      203 2023-07-05 19:46:27.094709 pyprojectsort-0.2.1/pyprojectsort/__init__.py
--rw-r--r--   0        0        0      138 2023-07-05 19:46:27.094709 pyprojectsort-0.2.1/pyprojectsort/__main__.py
--rw-r--r--   0        0        0      197 2023-07-05 19:46:27.094709 pyprojectsort-0.2.1/pyprojectsort/__version__.py
--rw-r--r--   0        0        0     2991 2023-07-05 19:46:27.094709 pyprojectsort-0.2.1/pyprojectsort/main.py
--rw-r--r--   0        0        0     3872 1970-01-01 00:00:00.000000 pyprojectsort-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     3200 2023-07-07 23:35:34.349272 pyprojectsort-0.2.2/README.md
+-rw-r--r--   0        0        0     2022 2023-07-07 23:35:34.349272 pyprojectsort-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0      203 2023-07-07 23:35:34.349272 pyprojectsort-0.2.2/pyprojectsort/__init__.py
+-rw-r--r--   0        0        0      138 2023-07-07 23:35:34.349272 pyprojectsort-0.2.2/pyprojectsort/__main__.py
+-rw-r--r--   0        0        0      197 2023-07-07 23:35:34.349272 pyprojectsort-0.2.2/pyprojectsort/__version__.py
+-rw-r--r--   0        0        0     3099 2023-07-07 23:35:34.349272 pyprojectsort-0.2.2/pyprojectsort/main.py
+-rw-r--r--   0        0        0     3974 1970-01-01 00:00:00.000000 pyprojectsort-0.2.2/PKG-INFO
```

### Comparing `pyprojectsort-0.2.1/pyproject.toml` & `pyprojectsort-0.2.2/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -4,117 +4,116 @@
     "flit",
 ]
 
 [project]
 authors = [
     { name = "Kieran Ryan" },
 ]
-name = "pyprojectsort"
-description = "Formatter for pyproject.toml files"
-readme = "README.md"
 classifiers = [
-    "License :: OSI Approved :: MIT License",
     "Intended Audience :: Developers",
+    "License :: OSI Approved :: MIT License",
     "Operating System :: MacOS",
     "Operating System :: Microsoft :: Windows",
     "Operating System :: POSIX :: Linux",
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.10",
 ]
 dependencies = [
-    "tomli==2.0.1",
     "tomli-w==1.0.0",
+    "tomli==2.0.1",
 ]
+description = "Formatter for pyproject.toml files"
 dynamic = [
     "version",
 ]
+name = "pyprojectsort"
+readme = "README.md"
 
 [project.scripts]
 pyprojectsort = "pyprojectsort.main:main"
 
 [project.urls]
 Documentation = "https://kieran-ryan.github.io/pyprojectsort/"
 Source = "https://github.com/kieran-ryan/pyprojectsort"
 Tracker = "https://github.com/kieran-ryan/pyprojectsort/issues"
 
-[tool.flit.module]
-name = "pyprojectsort"
-
 [tool.bandit]
 exclude_dirs = [
     "tests",
     "venv",
 ]
 
 [tool.coverage.html]
 directory = "docs/coverage"
 
+[tool.coverage.report]
+fail_under = 75.0
+show_missing = true
+
 [tool.coverage.run]
 branch = true
 omit = [
     "*/tests/*",
     "*/venv/*",
 ]
 
-[tool.coverage.report]
-fail_under = 75.0
-show_missing = true
-
 [tool.coverage.xml]
 output = "docs/coverage/coverage.xml"
 
+[tool.flit.module]
+name = "pyprojectsort"
+
 [tool.isort]
 profile = "black"
 src_paths = "pyprojectsort"
 
+[tool.mypy]
+exclude = "__init__.py|docs|tests|venv"
+files = "."
+mypy_path = "pyprojectsort"
+
+[tool.pylint]
+ignore = [
+    "docs",
+    "tests",
+    "venv",
+]
+recursive = true
+
+[tool.pytest.ini_options]
+addopts = "--doctest-modules -rA --verbose"
+testpaths = [
+    "pyprojectsort",
+    "tests",
+]
+
 [tool.radon]
 exclude = "tests/*,venv/*"
 show_complexity = true
 show_mi = true
 total_average = true
 
 [tool.ruff]
-select = [
-    "ALL",
-    "I002",
-]
 ignore = [
     "ANN",
     "ARG",
-    "DTZ005",
     "D203",
     "D213",
+    "DTZ005",
     "FIX002",
     "G004",
     "INP001",
     "S101",
     "T201",
     "TD003",
 ]
+select = [
+    "ALL",
+]
 
 [tool.ruff.isort]
 required-imports = [
     "from __future__ import annotations",
 ]
 
 [tool.ruff.pydocstyle]
 convention = "google"
-
-[tool.mypy]
-mypy_path = "pyprojectsort"
-files = "."
-exclude = "__init__.py|docs|tests|venv"
-
-[tool.pylint]
-recursive = true
-ignore = [
-    "docs",
-    "tests",
-    "venv",
-]
-
-[tool.pytest.ini_options]
-addopts = "--doctest-modules -rA --verbose"
-testpaths = [
-    "pyprojectsort",
-    "tests",
-]
```

### Comparing `pyprojectsort-0.2.1/pyprojectsort/main.py` & `pyprojectsort-0.2.2/pyprojectsort/main.py`

 * *Files 24% similar despite different names*

```diff
@@ -44,57 +44,60 @@
         print(f"No pyproject.toml detected at path: '{config}'")
         sys.exit(1)
     return config
 
 
 def _parse_pyproject_toml(file: pathlib.Path) -> dict[str, Any]:
     """Parse pyproject.toml file."""
-    with file.open("rb") as pyproject_file:
-        return tomllib.load(pyproject_file)
+    with file.open("r") as pyproject_file:
+        return pyproject_file.read()
 
 
 def reformat_pyproject(pyproject: dict | list) -> dict:
     """Reformat pyproject toml file."""
     if isinstance(pyproject, dict):
         return {
             key: reformat_pyproject(value)
             for key, value in sorted(pyproject.items(), key=lambda item: item[0])
         }
     if isinstance(pyproject, list):
         return sorted(reformat_pyproject(item) for item in pyproject)
     return pyproject
 
 
-def _check_format_needed(original: dict, reformatted: dict) -> bool:
+def _check_format_needed(original: str, reformatted: str) -> bool:
     """Check if there are any differences between original and reformatted."""
     return original != reformatted
 
 
 def _save_pyproject(file: pathlib.Path, pyproject: dict) -> None:
     """Write changes to pyproject.toml."""
     with file.open("wb") as pyproject_file:
         tomli_w.dump(pyproject, pyproject_file)
 
 
 def main() -> None:
     """Run application."""
     args = _read_cli(sys.argv[1:])
     pyproject_file = _read_config_file(pathlib.Path(args.file))
-    pyproject_toml = _parse_pyproject_toml(pyproject_file)
-    reformatted_pyproject = reformat_pyproject(pyproject_toml)
 
-    will_reformat = _check_format_needed(pyproject_toml, reformatted_pyproject)
+    pyproject_toml: str = _parse_pyproject_toml(pyproject_file)
+    pyproject: dict = tomllib.loads(pyproject_toml)
+    reformatted_pyproject: dict = reformat_pyproject(pyproject)
+    reformatted_pyproject_toml: str = tomli_w.dumps(reformatted_pyproject)
+
+    will_reformat = _check_format_needed(pyproject_toml, reformatted_pyproject_toml)
 
     if args.check:
         if will_reformat:
             print(f"'{args.file}' would be reformatted")
             sys.exit(1)
-        else:
-            print(f"'{args.file}' would be left unchanged")
-            return
+
+        print(f"'{args.file}' would be left unchanged")
+        return
 
     if will_reformat:
         _save_pyproject(pyproject_file, reformatted_pyproject)
         print(f"Reformatted '{args.file}'")
         sys.exit(1)
 
     print(f"'{args.file}' left unchanged")
```

### Comparing `pyprojectsort-0.2.1/PKG-INFO` & `pyprojectsort-0.2.2/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,68 +1,79 @@
 Metadata-Version: 2.1
 Name: pyprojectsort
-Version: 0.2.1
+Version: 0.2.2
 Summary: Formatter for pyproject.toml files
 Author: Kieran Ryan
 Description-Content-Type: text/markdown
-Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10
-Requires-Dist: tomli==2.0.1
 Requires-Dist: tomli-w==1.0.0
+Requires-Dist: tomli==2.0.1
 Project-URL: Documentation, https://kieran-ryan.github.io/pyprojectsort/
 Project-URL: Source, https://github.com/kieran-ryan/pyprojectsort
 Project-URL: Tracker, https://github.com/kieran-ryan/pyprojectsort/issues
 
 # pyprojectsort
 
-[![Release version](https://badge.fury.io/py/pyprojectsort.svg)](https://pypi.org/project/pyprojectsort/)
-![License](https://img.shields.io/badge/license-MIT-blue)
-![Python version](https://img.shields.io/badge/python-3.10-blue)
+[![image](https://badge.fury.io/py/pyprojectsort.svg)](https://pypi.org/project/pyprojectsort/)
+![image](https://img.shields.io/badge/license-MIT-blue)
+[![image](https://img.shields.io/pypi/pyversions/pyprojectsort.svg)](https://pypi.python.org/pypi/pyprojectsort)
 ![Supported platforms](https://img.shields.io/badge/platforms-macOS%20%7C%20Windows%20%7C%20Linux-green)
 ![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)
 [![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
 ![Pipeline status](https://github.com/kieran-ryan/python-package-template/actions/workflows/main.yml/badge.svg)
 
 Formatter for pyproject.toml files.
 
-This package enforces consistent formatting of pyproject.toml files, reducing merge request conflicts and saving time that would otherwise be spent on manual formatting. It also contributes to a cleaner git history and more readable code; enhancing overall project organisation and maintainability. Experience a streamlined workflow, reduced errors, and improved code readability with `pyprojectsort`.
+This package enforces consistent formatting of pyproject.toml files, reducing merge request conflicts and saving time otherwise spent to format manually. It also contributes to a cleaner git history and more readable code; enhancing overall project organisation and maintainability. Experience a streamlined workflow, reduced errors, and improved code readability with `pyprojectsort`.
 
 ## Features
 
 - Alphabetically sorts pyproject.toml by:
   - section
   - section key
   - list value
 - Reformats pyproject.toml to a standardised style
-  - Double quotations
-  - Trailing commas
-  - Line per value for list length above three
-    - or less with explicit trailing commas
+  - line per list value
+  - double quotations
+  - trailing commas
+  - indentation
+  - end of file newline
 
 ## Installation
 
-`pyprojectsort` is available via PyPI (via [Platform Wheels](https://packaging.python.org/guides/distributing-packages-using-setuptools/#platform-wheels)):
+`pyprojectsort` is available via [PyPI](https://pypi.org/project/pyprojectsort/):
 
 ```console
 pip install pyprojectsort
 ```
 
+### Using pyprojectsort with [pre-commit](https://pre-commit.com)
+
+To use as an automated git hook, add this to your `.pre-commit-config.yaml`:
+
+```yaml
+- repo: https://github.com/kieran-ryan/pyprojectsort
+  rev: v0.2.1
+  hooks:
+    - id: pyprojectsort
+```
+
 ## Examples
 
-With the following `pyproject.toml` contained inside a directory:
+With the following `pyproject.toml`:
 
 ```toml
 [tool.ruff]
-ignore = [
-    "G004",
+ignore = ["G004",
 "T201",
     "ANN"
 ]
 
 [project]
 name = 'pyprojectsort'
 
@@ -73,26 +84,28 @@
 show_complexity = true
 
 [build-system]
 build-backend = "flit.buildapi"
 requires = ["flit"]
 ```
 
-Run the package from within the directory of the pyproject toml file:
+Run the package from within its directory:
 
 ```console
 pyprojectsort
 ```
 
 The configuration will be reformatted as follows:
 
 ```toml
 [build-system]
 build-backend = "flit.buildapi"
-requires = ["flit"]
+requires = [
+    "flit",
+]
 
 [project]
 name = "pyprojectsort"
 
 [tool.radon]
 exclude = "tests/*,venv/*"
 show_complexity = true
@@ -103,29 +116,27 @@
 ignore = [
     "ANN",
     "G004",
     "T201",
 ]
 ```
 
-The path to the pyproject toml file can also be specified from the command line:
+The pyproject file path can alternatively be specified:
 
 ```console
 pyprojectsort ../pyproject.toml
 ```
 
 ### Check formatting
 
-To check whether formatting would be applied to your file you may use the **--check** option.
+The **--check** option can be used to determine whether your file would be reformatted.
 
 ```console
 pyprojectsort --check
 ```
 
-When the file would be reformatted, the output message `'{file_path}' would be reformatted` displays and the program terminates with exit code 1.
-
-If the given file matches the style of `pyprojectsort`, the output message `'{file_path}' would be left unchanged` displays and the program terminates successfully.
+If the file needs reformatting, the program exits with code 1. This is useful for [pipeline integration](https://github.com/kieran-ryan/pyprojectsort/blob/d9cf5e1e646e1e5260f7cf0168ecd0a05ce8ed11/.github/workflows/main.yml#L30) as it prevents writing back changes so a clean repository is maintained for subsequent jobs.
 
 ## License
 
-`pyprojectsort` is licensed under the [MIT License](https://opensource.org/licenses/MIT)
+`pyprojectsort` is licensed under the [MIT License](https://opensource.org/licenses/MIT).
```

