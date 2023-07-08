# Comparing `tmp/heatmap_cli-0.1.0.tar.gz` & `tmp/heatmap_cli-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "heatmap_cli-0.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "heatmap_cli-0.1.1.tar", last modified: Sat Jul  8 16:37:06 2023, max compression
```

## Comparing `heatmap_cli-0.1.0.tar` & `heatmap_cli-0.1.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0      143 2023-07-08 15:37:49.950263 heatmap_cli-0.1.0/.coveragerc
--rw-r--r--   0        0        0     3101 2023-07-08 15:39:47.014546 heatmap_cli-0.1.0/.gitignore
--rw-r--r--   0        0        0     2405 2023-07-08 15:37:49.950263 heatmap_cli-0.1.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0       13 2023-07-08 15:37:49.950263 heatmap_cli-0.1.0/.prettierignore
--rw-r--r--   0        0        0       29 2023-07-08 15:37:49.950263 heatmap_cli-0.1.0/.python-version
--rw-r--r--   0        0        0      311 2023-07-08 15:37:49.954263 heatmap_cli-0.1.0/CHANGELOG.md
--rw-r--r--   0        0        0     1738 2023-07-08 15:37:49.982263 heatmap_cli-0.1.0/CONTRIBUTING.md
--rw-r--r--   0        0        0    31956 2023-07-08 15:37:49.954263 heatmap_cli-0.1.0/LICENSE.md
--rw-r--r--   0        0        0      431 2023-07-08 15:48:34.632340 heatmap_cli-0.1.0/Pipfile
--rw-r--r--   0        0        0    69901 2023-07-08 15:47:08.952009 heatmap_cli-0.1.0/Pipfile.lock
--rw-r--r--   0        0        0     1927 2023-07-08 15:53:56.097660 heatmap_cli-0.1.0/README.md
--rw-r--r--   0        0        0      638 2023-07-08 15:37:49.954263 heatmap_cli-0.1.0/docs/Makefile
--rw-r--r--   0        0        0      804 2023-07-08 15:37:49.958263 heatmap_cli-0.1.0/docs/make.bat
-lrwxr-xr-x   0        0        0        0 2023-07-08 15:37:49.958263 heatmap_cli-0.1.0/docs/source/CHANGELOG.md -> ../../CHANGELOG.md
-lrwxr-xr-x   0        0        0        0 2023-07-08 15:37:49.958263 heatmap_cli-0.1.0/docs/source/CONTRIBUTING.md -> ../../CONTRIBUTING.md
-lrwxr-xr-x   0        0        0        0 2023-07-08 15:37:49.958263 heatmap_cli-0.1.0/docs/source/LICENSE.md -> ../../LICENSE.md
-lrwxr-xr-x   0        0        0        0 2023-07-08 15:37:49.958263 heatmap_cli-0.1.0/docs/source/README.md -> ../../README.md
--rw-r--r--   0        0        0    14202 2023-07-08 15:37:49.958263 heatmap_cli-0.1.0/docs/source/_static/logo.jpg
--rw-r--r--   0        0        0     1555 2023-07-08 15:37:49.982263 heatmap_cli-0.1.0/docs/source/conf.py
--rw-r--r--   0        0        0      172 2023-07-08 15:37:49.958263 heatmap_cli-0.1.0/docs/source/index.rst
--rw-r--r--   0        0        0      779 2023-07-08 15:37:49.986263 heatmap_cli-0.1.0/heatmap_cli/__init__.py
--rw-r--r--   0        0        0      837 2023-07-08 15:37:49.986263 heatmap_cli-0.1.0/heatmap_cli/__main__.py
--rw-r--r--   0        0        0     5395 2023-07-08 15:47:19.744050 heatmap_cli-0.1.0/heatmap_cli/cli.py
--rw-r--r--   0        0        0     1012 2023-07-08 15:37:49.986263 heatmap_cli-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-08 15:37:49.966263 heatmap_cli-0.1.0/tests/__init__.py
--rw-r--r--   0        0        0      845 2023-07-08 15:37:49.986263 heatmap_cli-0.1.0/tests/conftest.py
--rw-r--r--   0        0        0     5810 2023-07-08 15:37:49.970263 heatmap_cli-0.1.0/tests/fixtures/sample.csv
--rw-r--r--   0        0        0      303 2023-07-08 15:37:49.970263 heatmap_cli-0.1.0/tests/test_debug_flag.py
--rw-r--r--   0        0        0      326 2023-07-08 15:37:49.970263 heatmap_cli-0.1.0/tests/test_help_flag.py
--rw-r--r--   0        0        0      545 2023-07-08 15:37:49.970263 heatmap_cli-0.1.0/tests/test_verbose_flag.py
--rw-r--r--   0        0        0      306 2023-07-08 15:37:49.986263 heatmap_cli-0.1.0/tests/test_version_flag.py
--rw-r--r--   0        0        0      674 2023-07-08 15:37:49.986263 heatmap_cli-0.1.0/tox.ini
--rw-r--r--   0        0        0     2854 1970-01-01 00:00:00.000000 heatmap_cli-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      143 2023-07-08 15:37:49.950263 heatmap_cli-0.1.1/.coveragerc
+-rw-r--r--   0        0        0     3101 2023-07-08 15:39:47.014546 heatmap_cli-0.1.1/.gitignore
+-rw-r--r--   0        0        0     2411 2023-07-08 16:32:44.037058 heatmap_cli-0.1.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0       13 2023-07-08 15:37:49.950263 heatmap_cli-0.1.1/.prettierignore
+-rw-r--r--   0        0        0       29 2023-07-08 15:37:49.950263 heatmap_cli-0.1.1/.python-version
+-rw-r--r--   0        0        0      447 2023-07-08 16:34:28.286319 heatmap_cli-0.1.1/CHANGELOG.md
+-rw-r--r--   0        0        0     1738 2023-07-08 15:37:49.982263 heatmap_cli-0.1.1/CONTRIBUTING.md
+-rw-r--r--   0        0        0    31956 2023-07-08 15:37:49.954263 heatmap_cli-0.1.1/LICENSE.md
+-rw-r--r--   0        0        0      445 2023-07-08 16:09:00.508282 heatmap_cli-0.1.1/Pipfile
+-rw-r--r--   0        0        0    70216 2023-07-08 16:07:54.727800 heatmap_cli-0.1.1/Pipfile.lock
+-rw-r--r--   0        0        0     1927 2023-07-08 15:53:56.097660 heatmap_cli-0.1.1/README.md
+-rw-r--r--   0        0        0      638 2023-07-08 15:37:49.954263 heatmap_cli-0.1.1/docs/Makefile
+-rw-r--r--   0        0        0      804 2023-07-08 15:37:49.958263 heatmap_cli-0.1.1/docs/make.bat
+lrwxr-xr-x   0        0        0        0 2023-07-08 15:37:49.958263 heatmap_cli-0.1.1/docs/source/CHANGELOG.md -> ../../CHANGELOG.md
+lrwxr-xr-x   0        0        0        0 2023-07-08 15:37:49.958263 heatmap_cli-0.1.1/docs/source/CONTRIBUTING.md -> ../../CONTRIBUTING.md
+lrwxr-xr-x   0        0        0        0 2023-07-08 15:37:49.958263 heatmap_cli-0.1.1/docs/source/LICENSE.md -> ../../LICENSE.md
+lrwxr-xr-x   0        0        0        0 2023-07-08 15:37:49.958263 heatmap_cli-0.1.1/docs/source/README.md -> ../../README.md
+-rw-r--r--   0        0        0    14202 2023-07-08 15:37:49.958263 heatmap_cli-0.1.1/docs/source/_static/logo.jpg
+-rw-r--r--   0        0        0     1555 2023-07-08 15:37:49.982263 heatmap_cli-0.1.1/docs/source/conf.py
+-rw-r--r--   0        0        0      172 2023-07-08 15:37:49.958263 heatmap_cli-0.1.1/docs/source/index.rst
+-rw-r--r--   0        0        0      779 2023-07-08 16:35:06.210774 heatmap_cli-0.1.1/heatmap_cli/__init__.py
+-rw-r--r--   0        0        0      837 2023-07-08 15:37:49.986263 heatmap_cli-0.1.1/heatmap_cli/__main__.py
+-rw-r--r--   0        0        0     5395 2023-07-08 15:47:19.744050 heatmap_cli-0.1.1/heatmap_cli/cli.py
+-rw-r--r--   0        0        0     1077 2023-07-08 16:35:58.655379 heatmap_cli-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-08 15:37:49.966263 heatmap_cli-0.1.1/tests/__init__.py
+-rw-r--r--   0        0        0      845 2023-07-08 15:37:49.986263 heatmap_cli-0.1.1/tests/conftest.py
+-rw-r--r--   0        0        0     5810 2023-07-08 15:37:49.970263 heatmap_cli-0.1.1/tests/fixtures/sample.csv
+-rw-r--r--   0        0        0      303 2023-07-08 15:37:49.970263 heatmap_cli-0.1.1/tests/test_debug_flag.py
+-rw-r--r--   0        0        0      326 2023-07-08 15:37:49.970263 heatmap_cli-0.1.1/tests/test_help_flag.py
+-rw-r--r--   0        0        0      545 2023-07-08 15:37:49.970263 heatmap_cli-0.1.1/tests/test_verbose_flag.py
+-rw-r--r--   0        0        0      306 2023-07-08 15:37:49.986263 heatmap_cli-0.1.1/tests/test_version_flag.py
+-rw-r--r--   0        0        0      674 2023-07-08 15:37:49.986263 heatmap_cli-0.1.1/tox.ini
+-rw-r--r--   0        0        0     2925 1970-01-01 00:00:00.000000 heatmap_cli-0.1.1/PKG-INFO
```

### Comparing `heatmap_cli-0.1.0/.gitignore` & `heatmap_cli-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `heatmap_cli-0.1.0/.pre-commit-config.yaml` & `heatmap_cli-0.1.1/.pre-commit-config.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -73,27 +73,27 @@
           - flake8-docstrings
           - flake8-pytest-style
         args:
           - --docstring-convention=google
           - --show-source
           - --max-line-length=79
           - --exclude=docs/source/conf.py
-          - --per-file-ignores=heatmaps/*:D208 tests/*:D100,D103,D104,E501
+          - --per-file-ignores=heatmap_cli/*:D208 tests/*:D100,D103,D104,E501
 
   - repo: local
     hooks:
       - id: pylint
         name: pylint
         entry: pylint
         language: system
         types:
           - python
         exclude: docs/
         args:
-          - heatmaps
+          - heatmap_cli
           - tests
           - --unsafe-load-any-extension=y
 
   - repo: https://github.com/pre-commit/mirrors-mypy
     rev: v1.4.1
     hooks:
       - id: mypy
```

### Comparing `heatmap_cli-0.1.0/CONTRIBUTING.md` & `heatmap_cli-0.1.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `heatmap_cli-0.1.0/LICENSE.md` & `heatmap_cli-0.1.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `heatmap_cli-0.1.0/Pipfile.lock` & `heatmap_cli-0.1.1/Pipfile.lock`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9803240740740741%*

 * *Differences: {"'_meta'": "{'hash': {'sha256': "*

 * *            "'3ca75a6c9f5bce3c824dd0760065a90f1eeaca903a3e7dc06672fb64b1c2c046'}}",*

 * * "'default'": "{'seaborn': OrderedDict([('hashes', "*

 * *              "['sha256:374645f36509d0dcab895cba5b47daf0586f77bfe3b36c97c607db7da5be0139', "*

 * *              "'sha256:ebf15355a4dba46037dfd65b7350f014ceb1f13c05e814eda2c9f5fd731afc08']), "*

 * *              "('index', 'pypi'), ('version', '==0.12.2')])}"}*

```diff
@@ -1,11 +1,11 @@
 {
     "_meta": {
         "hash": {
-            "sha256": "1e52c887bf86a20c01ae2c7832abdb6a83c6e1f5a4ad873f15ec2b97faca158f"
+            "sha256": "3ca75a6c9f5bce3c824dd0760065a90f1eeaca903a3e7dc06672fb64b1c2c046"
         },
         "pipfile-spec": 6,
         "requires": {
             "python_version": "3.8"
         },
         "sources": [
             {
@@ -394,14 +394,22 @@
         "pytz": {
             "hashes": [
                 "sha256:1d8ce29db189191fb55338ee6d0387d82ab59f3d00eac103412d64e0ebd0c588",
                 "sha256:a151b3abb88eda1d4e34a9814df37de2a80e301e68ba0fd856fb9b46bfbbbffb"
             ],
             "version": "==2023.3"
         },
+        "seaborn": {
+            "hashes": [
+                "sha256:374645f36509d0dcab895cba5b47daf0586f77bfe3b36c97c607db7da5be0139",
+                "sha256:ebf15355a4dba46037dfd65b7350f014ceb1f13c05e814eda2c9f5fd731afc08"
+            ],
+            "index": "pypi",
+            "version": "==0.12.2"
+        },
         "six": {
             "hashes": [
                 "sha256:1e61c37477a1626458e36f7b1d82aa5c9b094fa4802892072e49de9c60c4c926",
                 "sha256:8abb2f1d86890a2dfb989f9a77cfcfd3e47c2a354b01111771326f8aa26e0254"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'",
             "version": "==1.16.0"
```

### Comparing `heatmap_cli-0.1.0/README.md` & `heatmap_cli-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `heatmap_cli-0.1.0/docs/Makefile` & `heatmap_cli-0.1.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `heatmap_cli-0.1.0/docs/make.bat` & `heatmap_cli-0.1.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `heatmap_cli-0.1.0/docs/source/_static/logo.jpg` & `heatmap_cli-0.1.1/docs/source/_static/logo.jpg`

 * *Files identical despite different names*

### Comparing `heatmap_cli-0.1.0/docs/source/conf.py` & `heatmap_cli-0.1.1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `heatmap_cli-0.1.0/heatmap_cli/__init__.py` & `heatmap_cli-0.1.1/heatmap_cli/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,8 +11,8 @@
 # details.
 #
 # You should have received a copy of the GNU Affero General Public License
 # along with this program. If not, see <https://www.gnu.org/licenses/>.
 
 """A console program that generates yearly calendar heatmap."""
 
-__version__ = "0.1.0"
+__version__ = "0.1.1"
```

### Comparing `heatmap_cli-0.1.0/heatmap_cli/__main__.py` & `heatmap_cli-0.1.1/heatmap_cli/__main__.py`

 * *Files identical despite different names*

### Comparing `heatmap_cli-0.1.0/heatmap_cli/cli.py` & `heatmap_cli-0.1.1/heatmap_cli/cli.py`

 * *Files identical despite different names*

### Comparing `heatmap_cli-0.1.0/pyproject.toml` & `heatmap_cli-0.1.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -16,14 +16,19 @@
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python",
 ]
 dynamic = ["version", "description"]
 keywords = ["heatmap", "cli"]
+dependencies = [
+    "matplotlib",
+    "pandas",
+    "seaborn"
+]
 
 [project.urls]
 Issues = "https://github.com/kianmeng/heatmap_cli/issues"
 Source = "https://github.com/kianmeng/heatmap_cli"
 Changelog = "https://github.com/kianmeng/heatmap_cli/blog/master/CHANGELOG.md"
 
 [project.scripts]
```

### Comparing `heatmap_cli-0.1.0/tests/conftest.py` & `heatmap_cli-0.1.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `heatmap_cli-0.1.0/tests/fixtures/sample.csv` & `heatmap_cli-0.1.1/tests/fixtures/sample.csv`

 * *Files identical despite different names*

### Comparing `heatmap_cli-0.1.0/tests/test_verbose_flag.py` & `heatmap_cli-0.1.1/tests/test_verbose_flag.py`

 * *Files identical despite different names*

### Comparing `heatmap_cli-0.1.0/tox.ini` & `heatmap_cli-0.1.1/tox.ini`

 * *Files identical despite different names*

### Comparing `heatmap_cli-0.1.0/PKG-INFO` & `heatmap_cli-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 Metadata-Version: 2.1
 Name: heatmap_cli
-Version: 0.1.0
+Version: 0.1.1
 Summary: A console program that generates yearly calendar heatmap.
 Keywords: heatmap,cli
 Author-email: Kian-Meng Ang <kianmeng@cpan.org>
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python
+Requires-Dist: matplotlib
+Requires-Dist: pandas
+Requires-Dist: seaborn
 Project-URL: Changelog, https://github.com/kianmeng/heatmap_cli/blog/master/CHANGELOG.md
 Project-URL: Issues, https://github.com/kianmeng/heatmap_cli/issues
 Project-URL: Source, https://github.com/kianmeng/heatmap_cli
 
 # heatmap_cli
 
 A console program that generates yearly calendar heatmap.
```

