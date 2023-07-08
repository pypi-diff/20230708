# Comparing `tmp/types-Flask-Migrate-4.0.0.4.tar.gz` & `tmp/types-Flask-Migrate-4.0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-Flask-Migrate-4.0.0.4.tar", last modified: Wed May 10 15:23:58 2023, max compression
+gzip compressed data, was "types-Flask-Migrate-4.0.0.5.tar", last modified: Sat Jul  8 12:30:40 2023, max compression
```

## Comparing `types-Flask-Migrate-4.0.0.4.tar` & `types-Flask-Migrate-4.0.0.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:23:58.195036 types-Flask-Migrate-4.0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-05-10 15:23:57.000000 types-Flask-Migrate-4.0.0.4/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-10 15:23:57.000000 types-Flask-Migrate-4.0.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-05-10 15:23:58.195036 types-Flask-Migrate-4.0.0.4/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:23:58.195036 types-Flask-Migrate-4.0.0.4/flask_migrate-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-10 15:23:57.000000 types-Flask-Migrate-4.0.0.4/flask_migrate-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)     3709 2023-05-10 15:19:44.000000 types-Flask-Migrate-4.0.0.4/flask_migrate-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 15:23:58.195036 types-Flask-Migrate-4.0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-05-10 15:23:57.000000 types-Flask-Migrate-4.0.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:23:58.195036 types-Flask-Migrate-4.0.0.4/types_Flask_Migrate.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-05-10 15:23:58.000000 types-Flask-Migrate-4.0.0.4/types_Flask_Migrate.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-05-10 15:23:58.000000 types-Flask-Migrate-4.0.0.4/types_Flask_Migrate.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 15:23:58.000000 types-Flask-Migrate-4.0.0.4/types_Flask_Migrate.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-10 15:23:58.000000 types-Flask-Migrate-4.0.0.4/types_Flask_Migrate.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-10 15:23:58.000000 types-Flask-Migrate-4.0.0.4/types_Flask_Migrate.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 12:30:40.713183 types-Flask-Migrate-4.0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-07-08 12:30:37.000000 types-Flask-Migrate-4.0.0.5/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-08 12:30:37.000000 types-Flask-Migrate-4.0.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-07-08 12:30:40.713183 types-Flask-Migrate-4.0.0.5/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 12:30:40.709183 types-Flask-Migrate-4.0.0.5/flask_migrate-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-07-08 12:30:37.000000 types-Flask-Migrate-4.0.0.5/flask_migrate-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     3709 2023-07-08 12:30:21.000000 types-Flask-Migrate-4.0.0.5/flask_migrate-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 12:30:40.713183 types-Flask-Migrate-4.0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-07-08 12:30:37.000000 types-Flask-Migrate-4.0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 12:30:40.713183 types-Flask-Migrate-4.0.0.5/types_Flask_Migrate.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-07-08 12:30:40.000000 types-Flask-Migrate-4.0.0.5/types_Flask_Migrate.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-08 12:30:40.000000 types-Flask-Migrate-4.0.0.5/types_Flask_Migrate.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 12:30:40.000000 types-Flask-Migrate-4.0.0.5/types_Flask_Migrate.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-08 12:30:40.000000 types-Flask-Migrate-4.0.0.5/types_Flask_Migrate.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-08 12:30:40.000000 types-Flask-Migrate-4.0.0.5/types_Flask_Migrate.egg-info/top_level.txt
```

### Comparing `types-Flask-Migrate-4.0.0.4/CHANGELOG.md` & `types-Flask-Migrate-4.0.0.5/CHANGELOG.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+## 4.0.0.5 (2023-07-08)
+
+Remove `SQLAlchemy` stubs (#10389)
+
+Co-authored-by: AlexWaygood <alex.waygood@gmail.com>
+
 ## 4.0.0.4 (2023-05-10)
 
 Add `partial_stub` metadata field (#10157)
 
 ## 4.0.0.3 (2023-03-27)
 
 Add defaults for third-party stubs E-H (#9954)
```

### Comparing `types-Flask-Migrate-4.0.0.4/PKG-INFO` & `types-Flask-Migrate-4.0.0.5/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-Flask-Migrate
-Version: 4.0.0.4
+Version: 4.0.0.5
 Summary: Typing stubs for Flask-Migrate
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/Flask-Migrate.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -21,9 +21,15 @@
 [pyright](https://github.com/microsoft/pyright),
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `Flask-Migrate`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/Flask-Migrate. All fixes for
 types and metadata should be contributed there.
 
+This stub package is marked as [partial](https://peps.python.org/pep-0561/#partial-stub-packages).
+If you find that annotations are missing, feel free to contribute and help complete them.
+
+
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `d1bfd08b4bc843227d097decfd99d70272a1f804`.
+This package was generated from typeshed commit `aed8c3fe1c7e8a4e720cd2cebb610d7ce186dc1b` and was tested
+with mypy 1.4.1, pyright 1.1.316, and
+pytype 2023.6.16.
```

### Comparing `types-Flask-Migrate-4.0.0.4/flask_migrate-stubs/__init__.pyi` & `types-Flask-Migrate-4.0.0.5/flask_migrate-stubs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-Flask-Migrate-4.0.0.4/setup.py` & `types-Flask-Migrate-4.0.0.5/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -11,33 +11,39 @@
 [pyright](https://github.com/microsoft/pyright),
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `Flask-Migrate`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/Flask-Migrate. All fixes for
 types and metadata should be contributed there.
 
+This stub package is marked as [partial](https://peps.python.org/pep-0561/#partial-stub-packages).
+If you find that annotations are missing, feel free to contribute and help complete them.
+
+
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `d1bfd08b4bc843227d097decfd99d70272a1f804`.
+This package was generated from typeshed commit `aed8c3fe1c7e8a4e720cd2cebb610d7ce186dc1b` and was tested
+with mypy 1.4.1, pyright 1.1.316, and
+pytype 2023.6.16.
 '''.lstrip()
 
 setup(name=name,
-      version="4.0.0.4",
+      version="4.0.0.5",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/Flask-Migrate.md",
           "Issue tracker": "https://github.com/python/typeshed/issues",
           "Chat": "https://gitter.im/python/typing",
       },
-      install_requires=['types-Flask-SQLAlchemy', 'Flask>=2.0.0'],
+      install_requires=['Flask>=2.0.0', 'Flask-SQLAlchemy>=3.0.1'],
       packages=['flask_migrate-stubs'],
-      package_data={'flask_migrate-stubs': ['__init__.pyi', 'METADATA.toml']},
+      package_data={'flask_migrate-stubs': ['__init__.pyi', 'METADATA.toml', 'py.typed']},
       license="Apache-2.0 license",
       classifiers=[
           "License :: OSI Approved :: Apache Software License",
           "Programming Language :: Python :: 3",
           "Typing :: Stubs Only",
       ]
 )
```

### Comparing `types-Flask-Migrate-4.0.0.4/types_Flask_Migrate.egg-info/PKG-INFO` & `types-Flask-Migrate-4.0.0.5/types_Flask_Migrate.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-Flask-Migrate
-Version: 4.0.0.4
+Version: 4.0.0.5
 Summary: Typing stubs for Flask-Migrate
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/Flask-Migrate.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -21,9 +21,15 @@
 [pyright](https://github.com/microsoft/pyright),
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `Flask-Migrate`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/Flask-Migrate. All fixes for
 types and metadata should be contributed there.
 
+This stub package is marked as [partial](https://peps.python.org/pep-0561/#partial-stub-packages).
+If you find that annotations are missing, feel free to contribute and help complete them.
+
+
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `d1bfd08b4bc843227d097decfd99d70272a1f804`.
+This package was generated from typeshed commit `aed8c3fe1c7e8a4e720cd2cebb610d7ce186dc1b` and was tested
+with mypy 1.4.1, pyright 1.1.316, and
+pytype 2023.6.16.
```

