# Comparing `tmp/jaraco.develop-8.0.0.tar.gz` & `tmp/jaraco.develop-8.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jaraco.develop-8.0.0.tar", last modified: Thu Jul  6 22:28:16 2023, max compression
+gzip compressed data, was "jaraco.develop-8.1.0.tar", last modified: Sat Jul  8 03:15:02 2023, max compression
```

## Comparing `jaraco.develop-8.0.0.tar` & `jaraco.develop-8.1.0.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 22:28:16.254268 jaraco.develop-8.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-06 22:27:53.000000 jaraco.develop-8.0.0/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-06 22:27:53.000000 jaraco.develop-8.0.0/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 22:28:16.242268 jaraco.develop-8.0.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-06 22:27:53.000000 jaraco.develop-8.0.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 22:28:16.242268 jaraco.develop-8.0.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     3104 2023-07-06 22:27:53.000000 jaraco.develop-8.0.0/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-06 22:27:53.000000 jaraco.develop-8.0.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-06 22:27:53.000000 jaraco.develop-8.0.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-07-06 22:27:53.000000 jaraco.develop-8.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7820 2023-07-06 22:27:53.000000 jaraco.develop-8.0.0/NEWS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-07-06 22:28:16.254268 jaraco.develop-8.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      962 2023-07-06 22:27:53.000000 jaraco.develop-8.0.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-07-06 22:27:53.000000 jaraco.develop-8.0.0/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 22:28:16.242268 jaraco.develop-8.0.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-07-06 22:27:53.000000 jaraco.develop-8.0.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-06 22:27:53.000000 jaraco.develop-8.0.0/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-06 22:27:53.000000 jaraco.develop-8.0.0/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 22:28:16.238268 jaraco.develop-8.0.0/jaraco/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 22:28:16.254268 jaraco.develop-8.0.0/jaraco/develop/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 22:27:53.000000 jaraco.develop-8.0.0/jaraco/develop/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-07-06 22:27:53.000000 jaraco.develop-8.0.0/jaraco/develop/add-github-secret.py
--rw-r--r--   0 runner    (1001) docker     (123)      913 2023-07-06 22:27:53.000000 jaraco.develop-8.0.0/jaraco/develop/add-github-secrets.py
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-07-06 22:27:53.000000 jaraco.develop-8.0.0/jaraco/develop/checkout-all.py
--rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-07-06 22:27:53.000000 jaraco.develop-8.0.0/jaraco/develop/compiler.py
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-07-06 22:27:53.000000 jaraco.develop-8.0.0/jaraco/develop/create-github-release.py
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-07-06 22:27:53.000000 jaraco.develop-8.0.0/jaraco/develop/finalize.py
--rw-r--r--   0 runner    (1001) docker     (123)     4999 2023-07-06 22:27:53.000000 jaraco.develop-8.0.0/jaraco/develop/git.py
--rw-r--r--   0 runner    (1001) docker     (123)     2712 2023-07-06 22:27:53.000000 jaraco.develop-8.0.0/jaraco/develop/github.py
--rw-r--r--   0 runner    (1001) docker     (123)     2545 2023-07-06 22:27:53.000000 jaraco.develop-8.0.0/jaraco/develop/indent.py
--rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-07-06 22:27:53.000000 jaraco.develop-8.0.0/jaraco/develop/init-azure.py
--rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-07-06 22:27:53.000000 jaraco.develop-8.0.0/jaraco/develop/macos-build-python.py
--rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-07-06 22:27:53.000000 jaraco.develop-8.0.0/jaraco/develop/merge.py
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-07-06 22:27:53.000000 jaraco.develop-8.0.0/jaraco/develop/print-meta.py
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-07-06 22:27:53.000000 jaraco.develop-8.0.0/jaraco/develop/pypi.py
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-07-06 22:27:53.000000 jaraco.develop-8.0.0/jaraco/develop/repo.py
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-07-06 22:27:53.000000 jaraco.develop-8.0.0/jaraco/develop/rst-header-replace.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-06 22:27:53.000000 jaraco.develop-8.0.0/jaraco/develop/rtd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-07-06 22:27:53.000000 jaraco.develop-8.0.0/jaraco/develop/towncrier.py
--rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-07-06 22:27:53.000000 jaraco.develop-8.0.0/jaraco/develop/update-projects.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 22:28:16.242268 jaraco.develop-8.0.0/jaraco.develop.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-07-06 22:28:16.000000 jaraco.develop-8.0.0/jaraco.develop.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-07-06 22:28:16.000000 jaraco.develop-8.0.0/jaraco.develop.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 22:28:16.000000 jaraco.develop-8.0.0/jaraco.develop.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-07-06 22:28:16.000000 jaraco.develop-8.0.0/jaraco.develop.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-06 22:28:16.000000 jaraco.develop-8.0.0/jaraco.develop.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-06 22:27:53.000000 jaraco.develop-8.0.0/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-06 22:27:53.000000 jaraco.develop-8.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-07-06 22:27:53.000000 jaraco.develop-8.0.0/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-07-06 22:28:16.258268 jaraco.develop-8.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-07-06 22:27:53.000000 jaraco.develop-8.0.0/todo.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-06 22:27:53.000000 jaraco.develop-8.0.0/towncrier.toml
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-07-06 22:27:53.000000 jaraco.develop-8.0.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 03:15:02.054677 jaraco.develop-8.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-08 03:14:40.000000 jaraco.develop-8.1.0/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-08 03:14:40.000000 jaraco.develop-8.1.0/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 03:15:02.038677 jaraco.develop-8.1.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-08 03:14:40.000000 jaraco.develop-8.1.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 03:15:02.042677 jaraco.develop-8.1.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     3088 2023-07-08 03:14:40.000000 jaraco.develop-8.1.0/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-08 03:14:40.000000 jaraco.develop-8.1.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-08 03:14:40.000000 jaraco.develop-8.1.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-07-08 03:14:40.000000 jaraco.develop-8.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7960 2023-07-08 03:14:40.000000 jaraco.develop-8.1.0/NEWS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-07-08 03:15:02.054677 jaraco.develop-8.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      962 2023-07-08 03:14:40.000000 jaraco.develop-8.1.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-07-08 03:14:40.000000 jaraco.develop-8.1.0/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 03:15:02.042677 jaraco.develop-8.1.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-07-08 03:14:40.000000 jaraco.develop-8.1.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-08 03:14:40.000000 jaraco.develop-8.1.0/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-07-08 03:14:40.000000 jaraco.develop-8.1.0/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 03:15:02.030677 jaraco.develop-8.1.0/jaraco/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 03:15:02.054677 jaraco.develop-8.1.0/jaraco/develop/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 03:14:40.000000 jaraco.develop-8.1.0/jaraco/develop/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-07-08 03:14:40.000000 jaraco.develop-8.1.0/jaraco/develop/add-github-secret.py
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-07-08 03:14:40.000000 jaraco.develop-8.1.0/jaraco/develop/add-github-secrets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-07-08 03:14:40.000000 jaraco.develop-8.1.0/jaraco/develop/checkout-all.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-07-08 03:14:40.000000 jaraco.develop-8.1.0/jaraco/develop/compiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-07-08 03:14:40.000000 jaraco.develop-8.1.0/jaraco/develop/create-github-release.py
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-07-08 03:14:40.000000 jaraco.develop-8.1.0/jaraco/develop/finalize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4999 2023-07-08 03:14:40.000000 jaraco.develop-8.1.0/jaraco/develop/git.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2712 2023-07-08 03:14:40.000000 jaraco.develop-8.1.0/jaraco/develop/github.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2545 2023-07-08 03:14:40.000000 jaraco.develop-8.1.0/jaraco/develop/indent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-07-08 03:14:40.000000 jaraco.develop-8.1.0/jaraco/develop/init-azure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-07-08 03:14:40.000000 jaraco.develop-8.1.0/jaraco/develop/macos-build-python.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-07-08 03:14:40.000000 jaraco.develop-8.1.0/jaraco/develop/merge.py
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-07-08 03:14:40.000000 jaraco.develop-8.1.0/jaraco/develop/print-meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-07-08 03:14:40.000000 jaraco.develop-8.1.0/jaraco/develop/pypi.py
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-07-08 03:14:40.000000 jaraco.develop-8.1.0/jaraco/develop/repo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-07-08 03:14:40.000000 jaraco.develop-8.1.0/jaraco/develop/rst-header-replace.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-08 03:14:40.000000 jaraco.develop-8.1.0/jaraco/develop/rtd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-07-08 03:14:40.000000 jaraco.develop-8.1.0/jaraco/develop/towncrier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2275 2023-07-08 03:14:40.000000 jaraco.develop-8.1.0/jaraco/develop/update-projects.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 03:15:02.042677 jaraco.develop-8.1.0/jaraco.develop.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-07-08 03:15:02.000000 jaraco.develop-8.1.0/jaraco.develop.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-07-08 03:15:02.000000 jaraco.develop-8.1.0/jaraco.develop.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 03:15:02.000000 jaraco.develop-8.1.0/jaraco.develop.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-07-08 03:15:02.000000 jaraco.develop-8.1.0/jaraco.develop.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-08 03:15:02.000000 jaraco.develop-8.1.0/jaraco.develop.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-08 03:14:40.000000 jaraco.develop-8.1.0/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-08 03:14:40.000000 jaraco.develop-8.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-07-08 03:14:40.000000 jaraco.develop-8.1.0/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-07-08 03:15:02.054677 jaraco.develop-8.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-07-08 03:14:40.000000 jaraco.develop-8.1.0/todo.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-08 03:14:40.000000 jaraco.develop-8.1.0/towncrier.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-07-08 03:14:40.000000 jaraco.develop-8.1.0/tox.ini
```

### Comparing `jaraco.develop-8.0.0/.github/workflows/main.yml` & `jaraco.develop-8.1.0/.github/workflows/main.yml`

 * *Files 2% similar despite different names*

```diff
@@ -62,29 +62,29 @@
         uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python }}
           allow-prereleases: true
       - name: Install tox
         run: |
           python -m pip install tox
-      - name: Run tests
+      - name: Run
         run: tox
 
   docs:
     runs-on: ubuntu-latest
     env:
       TOXENV: docs
     steps:
       - uses: actions/checkout@v3
       - name: Setup Python
         uses: actions/setup-python@v4
       - name: Install tox
         run: |
           python -m pip install tox
-      - name: Run tests
+      - name: Run
         run: tox
 
   check:  # This job does nothing and is only used for the branch protection
     if: always()
 
     needs:
     - test
@@ -111,12 +111,12 @@
       - name: Setup Python
         uses: actions/setup-python@v4
         with:
           python-version: 3.x
       - name: Install tox
         run: |
           python -m pip install tox
-      - name: Release
+      - name: Run
         run: tox -e release
         env:
           TWINE_PASSWORD: ${{ secrets.PYPI_TOKEN }}
           GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
```

### Comparing `jaraco.develop-8.0.0/LICENSE` & `jaraco.develop-8.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jaraco.develop-8.0.0/NEWS.rst` & `jaraco.develop-8.1.0/NEWS.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,16 @@
+v8.1.0
+======
+
+Features
+--------
+
+- Improved handling of unrelated histories and correctly reporting projects updated in update-projects.
+
+
 v8.0.0
 ======
 
 Deprecations and Removals
 -------------------------
 
 - Replace ``pep517`` with ``build``. ``repo.get_project_metadata`` no longer includes the ``dist``.
```

### Comparing `jaraco.develop-8.0.0/PKG-INFO` & `jaraco.develop-8.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaraco.develop
-Version: 8.0.0
+Version: 8.1.0
 Summary: Development utilities by jaraco
 Home-page: https://github.com/jaraco/jaraco.develop
 Author: Jason R. Coombs
 Author-email: jaraco@jaraco.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `jaraco.develop-8.0.0/README.rst` & `jaraco.develop-8.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `jaraco.develop-8.0.0/conftest.py` & `jaraco.develop-8.1.0/conftest.py`

 * *Files identical despite different names*

### Comparing `jaraco.develop-8.0.0/docs/conf.py` & `jaraco.develop-8.1.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `jaraco.develop-8.0.0/jaraco/develop/add-github-secrets.py` & `jaraco.develop-8.1.0/jaraco/develop/add-github-secrets.py`

 * *Files identical despite different names*

### Comparing `jaraco.develop-8.0.0/jaraco/develop/compiler.py` & `jaraco.develop-8.1.0/jaraco/develop/compiler.py`

 * *Files identical despite different names*

### Comparing `jaraco.develop-8.0.0/jaraco/develop/git.py` & `jaraco.develop-8.1.0/jaraco/develop/git.py`

 * *Files identical despite different names*

### Comparing `jaraco.develop-8.0.0/jaraco/develop/github.py` & `jaraco.develop-8.1.0/jaraco/develop/github.py`

 * *Files identical despite different names*

### Comparing `jaraco.develop-8.0.0/jaraco/develop/indent.py` & `jaraco.develop-8.1.0/jaraco/develop/indent.py`

 * *Files identical despite different names*

### Comparing `jaraco.develop-8.0.0/jaraco/develop/init-azure.py` & `jaraco.develop-8.1.0/jaraco/develop/init-azure.py`

 * *Files identical despite different names*

### Comparing `jaraco.develop-8.0.0/jaraco/develop/macos-build-python.py` & `jaraco.develop-8.1.0/jaraco/develop/macos-build-python.py`

 * *Files identical despite different names*

### Comparing `jaraco.develop-8.0.0/jaraco/develop/merge.py` & `jaraco.develop-8.1.0/jaraco/develop/merge.py`

 * *Files identical despite different names*

### Comparing `jaraco.develop-8.0.0/jaraco/develop/rst-header-replace.py` & `jaraco.develop-8.1.0/jaraco/develop/rst-header-replace.py`

 * *Files identical despite different names*

### Comparing `jaraco.develop-8.0.0/jaraco/develop/towncrier.py` & `jaraco.develop-8.1.0/jaraco/develop/towncrier.py`

 * *Files identical despite different names*

### Comparing `jaraco.develop-8.0.0/jaraco/develop/update-projects.py` & `jaraco.develop-8.1.0/jaraco/develop/update-projects.py`

 * *Files 13% similar despite different names*

```diff
@@ -9,64 +9,57 @@
 trustExitCode = true
 """
 
 import contextlib
 import subprocess
 import functools
 import shutil
-import itertools
 
 import path
 import autocommand
-import jaraco.context
-from more_itertools import consume
+import subprocess_tee
 
 from . import git
 
 
 @contextlib.contextmanager
 def temp_checkout(project):
     with path.TempDir() as dir:
         repo = git.checkout(project, dir, depth=50)
         with repo:
             yield
 
 
-@jaraco.context.suppress(FileNotFoundError)
-def is_skeleton():
-    return 'badge/skeleton' in path.Path('README.rst').read_text()
-
-
 def handle_rename(old_name, new_name):
     status = subprocess.check_output(['git', 'status', '--porcelain'], text=True)
     if f'UD {old_name}' not in status:
         return
     shutil.copyfile(old_name, new_name)
     subprocess.check_call(['git', 'rm', old_name])
     subprocess.check_call(['git', 'add', new_name])
 
 
 def update_project(name, base, branch=None):
     if set(name.tags) & {'fork', 'base'}:
         return
     print('\nupdating', name)
     with temp_checkout(name):
-        if not is_skeleton():
-            return
         cmd = ['git', 'pull', base, branch, '--no-edit']
-        proc = subprocess.Popen(list(filter(None, cmd)))
-        code = proc.wait()
-        if code:
+        proc = subprocess_tee.run(list(filter(None, cmd)))
+        if proc.returncode:
+            if 'unrelated histories' in proc.stderr:
+                return
             handle_rename('CHANGES.rst', 'NEWS.rst')
             try:
                 subprocess.check_call(['git', 'mergetool', '-t', 'known-merge'])
             except subprocess.CalledProcessError:
                 subprocess.check_call(['git', 'mergetool'])
             subprocess.check_call(['git', 'commit', '--no-edit'])
         subprocess.check_call(['git', 'push'])
+        return name
 
 
 class KeywordFilter(str):
     def __call__(self, other):
         return self in other
 
 
@@ -79,11 +72,10 @@
 def main(
     keyword: KeywordFilter = None,  # type: ignore
     tag: TagFilter = None,  # type: ignore
     base='gh://jaraco/skeleton',
     branch=None,
 ):
     update = functools.partial(update_project, base=base, branch=branch)
-    counter = itertools.count()
     updates = map(update, filter(tag, filter(keyword, git.projects())))
-    consume(zip(counter, updates))
-    print(f"Updated {next(counter)} projects.")
+    total = len(list(filter(None, updates)))
+    print(f"Updated {total} projects.")
```

### Comparing `jaraco.develop-8.0.0/jaraco.develop.egg-info/PKG-INFO` & `jaraco.develop-8.1.0/jaraco.develop.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaraco.develop
-Version: 8.0.0
+Version: 8.1.0
 Summary: Development utilities by jaraco
 Home-page: https://github.com/jaraco/jaraco.develop
 Author: Jason R. Coombs
 Author-email: jaraco@jaraco.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `jaraco.develop-8.0.0/jaraco.develop.egg-info/SOURCES.txt` & `jaraco.develop-8.1.0/jaraco.develop.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jaraco.develop-8.0.0/pytest.ini` & `jaraco.develop-8.1.0/pytest.ini`

 * *Files identical despite different names*

### Comparing `jaraco.develop-8.0.0/setup.cfg` & `jaraco.develop-8.1.0/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 	requests-toolbelt
 	PyNaCl
 	packaging
 	setuptools
 	path
 	jaraco.vcs >= 1.1
 	build
+	subprocess-tee
 
 [options.packages.find]
 exclude = 
 	build*
 	dist*
 	docs*
 	tests*
@@ -49,15 +50,15 @@
 	pytest-enabler >= 2.2
 	pytest-ruff
 	
 	pytest-subprocess
 	types-requests
 docs = 
 	sphinx >= 3.5
-	jaraco.packaging >= 9
+	jaraco.packaging >= 9.3
 	rst.linker >= 1.9
 	furo
 	sphinx-lint
 
 [options.entry_points]
 
 [egg_info]
```

### Comparing `jaraco.develop-8.0.0/tox.ini` & `jaraco.develop-8.1.0/tox.ini`

 * *Files identical despite different names*

