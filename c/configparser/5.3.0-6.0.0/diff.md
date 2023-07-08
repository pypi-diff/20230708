# Comparing `tmp/configparser-5.3.0.tar.gz` & `tmp/configparser-6.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "configparser-5.3.0.tar", last modified: Fri Aug 19 17:45:07 2022, max compression
+gzip compressed data, was "configparser-6.0.0.tar", last modified: Sat Jul  8 20:03:52 2023, max compression
```

## Comparing `configparser-5.3.0.tar` & `configparser-6.0.0.tar`

### file list

```diff
@@ -1,44 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-19 17:45:07.274403 configparser-5.3.0/
--rw-r--r--   0 runner    (1001) docker     (121)      121 2022-08-19 17:44:31.000000 configparser-5.3.0/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (121)      246 2022-08-19 17:44:31.000000 configparser-5.3.0/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (121)      136 2022-08-19 17:44:31.000000 configparser-5.3.0/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-19 17:45:07.266403 configparser-5.3.0/.github/
--rw-r--r--   0 runner    (1001) docker     (121)       28 2022-08-19 17:44:31.000000 configparser-5.3.0/.github/FUNDING.yml
--rw-r--r--   0 runner    (1001) docker     (121)      148 2022-08-19 17:44:31.000000 configparser-5.3.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-19 17:45:07.266403 configparser-5.3.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     1450 2022-08-19 17:44:31.000000 configparser-5.3.0/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (121)       81 2022-08-19 17:44:31.000000 configparser-5.3.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)       79 2022-08-19 17:44:31.000000 configparser-5.3.0/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (121)     5194 2022-08-19 17:44:31.000000 configparser-5.3.0/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1050 2022-08-19 17:44:31.000000 configparser-5.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)    10257 2022-08-19 17:45:07.274403 configparser-5.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     9548 2022-08-19 17:44:31.000000 configparser-5.3.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)    51057 2022-08-19 17:44:31.000000 configparser-5.3.0/configparser.rst
--rw-r--r--   0 runner    (1001) docker     (121)       89 2022-08-19 17:44:31.000000 configparser-5.3.0/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-19 17:45:07.266403 configparser-5.3.0/docs/
--rw-r--r--   0 runner    (1001) docker     (121)     1184 2022-08-19 17:44:31.000000 configparser-5.3.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)       81 2022-08-19 17:44:31.000000 configparser-5.3.0/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (121)      325 2022-08-19 17:44:31.000000 configparser-5.3.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)       37 2022-08-19 17:44:31.000000 configparser-5.3.0/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (121)      378 2022-08-19 17:44:31.000000 configparser-5.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)     1261 2022-08-19 17:44:31.000000 configparser-5.3.0/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (121)     1248 2022-08-19 17:45:07.274403 configparser-5.3.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-19 17:45:07.270403 configparser-5.3.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-19 17:45:07.254403 configparser-5.3.0/src/backports/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-19 17:45:07.270403 configparser-5.3.0/src/backports/configparser/
--rw-r--r--   0 runner    (1001) docker     (121)    55291 2022-08-19 17:44:31.000000 configparser-5.3.0/src/backports/configparser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      404 2022-08-19 17:44:31.000000 configparser-5.3.0/src/backports/configparser/compat.py
--rw-r--r--   0 runner    (1001) docker     (121)       67 2022-08-19 17:44:31.000000 configparser-5.3.0/src/cfgparser.1
--rw-r--r--   0 runner    (1001) docker     (121)    19472 2022-08-19 17:44:31.000000 configparser-5.3.0/src/cfgparser.2
--rw-r--r--   0 runner    (1001) docker     (121)     1587 2022-08-19 17:44:31.000000 configparser-5.3.0/src/cfgparser.3
--rw-r--r--   0 runner    (1001) docker     (121)      519 2022-08-19 17:44:31.000000 configparser-5.3.0/src/compat.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-19 17:45:07.274403 configparser-5.3.0/src/configparser.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    10257 2022-08-19 17:45:07.000000 configparser-5.3.0/src/configparser.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      705 2022-08-19 17:45:07.000000 configparser-5.3.0/src/configparser.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-19 17:45:07.000000 configparser-5.3.0/src/configparser.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      276 2022-08-19 17:45:07.000000 configparser-5.3.0/src/configparser.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       23 2022-08-19 17:45:07.000000 configparser-5.3.0/src/configparser.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1546 2022-08-19 17:44:31.000000 configparser-5.3.0/src/configparser.py
--rw-r--r--   0 runner    (1001) docker     (121)     2911 2022-08-19 17:44:31.000000 configparser-5.3.0/src/test_backport.py
--rw-r--r--   0 runner    (1001) docker     (121)    89826 2022-08-19 17:44:31.000000 configparser-5.3.0/src/test_configparser.py
--rw-r--r--   0 runner    (1001) docker     (121)      732 2022-08-19 17:44:31.000000 configparser-5.3.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 20:03:52.365180 configparser-6.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-08 20:03:24.000000 configparser-6.0.0/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-08 20:03:24.000000 configparser-6.0.0/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 20:03:52.361180 configparser-6.0.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-08 20:03:24.000000 configparser-6.0.0/.github/FUNDING.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-08 20:03:24.000000 configparser-6.0.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 20:03:52.361180 configparser-6.0.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     3146 2023-07-08 20:03:24.000000 configparser-6.0.0/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-08 20:03:24.000000 configparser-6.0.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-08 20:03:24.000000 configparser-6.0.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-07-08 20:03:24.000000 configparser-6.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5405 2023-07-08 20:03:24.000000 configparser-6.0.0/NEWS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10194 2023-07-08 20:03:52.365180 configparser-6.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9485 2023-07-08 20:03:24.000000 configparser-6.0.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-07-08 20:03:24.000000 configparser-6.0.0/SECURITY.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 20:03:52.353180 configparser-6.0.0/backports/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 20:03:52.361180 configparser-6.0.0/backports/configparser/
+-rw-r--r--   0 runner    (1001) docker     (123)    53363 2023-07-08 20:03:24.000000 configparser-6.0.0/backports/configparser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-07-08 20:03:24.000000 configparser-6.0.0/backports/configparser/compat.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 20:03:52.361180 configparser-6.0.0/configparser/
+-rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-07-08 20:03:24.000000 configparser-6.0.0/configparser/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 20:03:52.361180 configparser-6.0.0/configparser.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10194 2023-07-08 20:03:52.000000 configparser-6.0.0/configparser.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-07-08 20:03:52.000000 configparser-6.0.0/configparser.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 20:03:52.000000 configparser-6.0.0/configparser.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-07-08 20:03:52.000000 configparser-6.0.0/configparser.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-08 20:03:52.000000 configparser-6.0.0/configparser.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    50659 2023-07-08 20:03:24.000000 configparser-6.0.0/configparser.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-08 20:03:24.000000 configparser-6.0.0/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 20:03:52.365180 configparser-6.0.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-07-08 20:03:24.000000 configparser-6.0.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-08 20:03:24.000000 configparser-6.0.0/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-07-08 20:03:24.000000 configparser-6.0.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-08 20:03:24.000000 configparser-6.0.0/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-08 20:03:24.000000 configparser-6.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-07-08 20:03:24.000000 configparser-6.0.0/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-07-08 20:03:52.365180 configparser-6.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 20:03:52.365180 configparser-6.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-08 20:03:24.000000 configparser-6.0.0/tests/cfgparser.1
+-rw-r--r--   0 runner    (1001) docker     (123)    19472 2023-07-08 20:03:24.000000 configparser-6.0.0/tests/cfgparser.2
+-rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-07-08 20:03:24.000000 configparser-6.0.0/tests/cfgparser.3
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-07-08 20:03:24.000000 configparser-6.0.0/tests/compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2906 2023-07-08 20:03:24.000000 configparser-6.0.0/tests/test_backport.py
+-rw-r--r--   0 runner    (1001) docker     (123)    88295 2023-07-08 20:03:24.000000 configparser-6.0.0/tests/test_configparser.py
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-08 20:03:24.000000 configparser-6.0.0/towncrier.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      905 2023-07-08 20:03:24.000000 configparser-6.0.0/tox.ini
```

### Comparing `configparser-5.3.0/CHANGES.rst` & `configparser-6.0.0/NEWS.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+v6.0.0
+======
+
+Features
+--------
+
+- Require Python 3.8 or later.
+
+
+Deprecations and Removals
+-------------------------
+
+- Synced with CPython 3.12.0b2. Removes ``SafeConfigParser`` and ``filename`` parameter.
+
+
 v5.3.0
 ======
 
 * Synced with Python 3.11.0rc1.
 * Packaging refresh.
 * Requires Python 3.7 or later.
```

### Comparing `configparser-5.3.0/LICENSE` & `configparser-6.0.0/LICENSE`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-Copyright Jason R. Coombs
-
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to
 deal in the Software without restriction, including without limitation the
 rights to use, copy, modify, merge, publish, distribute, sublicense, and/or
 sell copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `configparser-5.3.0/PKG-INFO` & `configparser-6.0.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,48 +1,49 @@
 Metadata-Version: 2.1
 Name: configparser
-Version: 5.3.0
+Version: 6.0.0
 Summary: Updated configparser from stdlib for earlier Pythons.
 Home-page: https://github.com/jaraco/configparser/
 Author: Łukasz Langa
 Author-email: lukasz@langa.pl
 Maintainer: Jason R. Coombs
 Maintainer-email: jaraco@jaraco.com
 Keywords: configparser ini parsing conf cfg configuration file
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Provides-Extra: testing
 Provides-Extra: docs
 License-File: LICENSE
 
 .. image:: https://img.shields.io/pypi/v/configparser.svg
-   :target: `PyPI link`_
+   :target: https://pypi.org/project/configparser
 
 .. image:: https://img.shields.io/pypi/pyversions/configparser.svg
-   :target: `PyPI link`_
-
-.. _PyPI link: https://pypi.org/project/configparser
 
 .. image:: https://github.com/jaraco/configparser/workflows/tests/badge.svg
    :target: https://github.com/jaraco/configparser/actions?query=workflow%3A%22tests%22
    :alt: tests
 
+.. image:: https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json
+    :target: https://github.com/astral-sh/ruff
+    :alt: Ruff
+
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
    :target: https://github.com/psf/black
    :alt: Code style: Black
 
 .. image:: https://readthedocs.org/projects/configparser/badge/?version=latest
    :target: https://configparser.readthedocs.io/en/latest/?badge=latest
 
-.. image:: https://img.shields.io/badge/skeleton-2022-informational
+.. image:: https://img.shields.io/badge/skeleton-2023-informational
    :target: https://blog.jaraco.com/skeleton
 
 .. image:: https://tidelift.com/badges/package/pypi/configparser
    :target: https://tidelift.com/subscription/pkg/pypi-configparser?utm_source=pypi-configparser&utm_medium=readme
 
 
 This package is a backport of the refreshed and enhanced ConfigParser from
@@ -56,15 +57,15 @@
 
   import configparser
 
 For detailed documentation consult the vanilla version at
 http://docs.python.org/3/library/configparser.html.
 
 Why you'll love ``configparser``
---------------------------------
+================================
 
 Whereas almost completely compatible with its older brother, ``configparser``
 sports a bunch of interesting new features:
 
 * full mapping protocol access (`more info
   <http://docs.python.org/3/library/configparser.html#mapping-protocol-access>`_)::
 
@@ -128,15 +129,15 @@
   the whole configuration (multiple sections) is now a single line of code. Same
   goes for copying data from another ``ConfigParser`` instance, thanks to its
   mapping protocol support.
 
 * many smaller tweaks, updates and fixes
 
 A few words about Unicode
--------------------------
+=========================
 
 ``configparser`` comes from Python 3 and as such it works well with Unicode.
 The library is generally cleaned up in terms of internal data storage and
 reading/writing files.  There are a couple of incompatibilities with the old
 ``ConfigParser`` due to that. However, the work required to migrate is well
 worth it as it shows the issues that would likely come up during migration of
 your project to Python 3.
@@ -145,56 +146,40 @@
 gives you the certainty that what's stored in a configuration object is text.
 Once your configuration is read, the rest of your application doesn't have to
 deal with encoding issues. All you have is text [2]_. The only two phases when
 you should explicitly state encoding is when you either read from an external
 source (e.g. a file) or write back.
 
 Versioning
-----------
+==========
 
 This project uses `semver <https://semver.org/spec/v2.0.0.html>`_ to
 communicate the impact of various releases while periodically syncing
 with the upstream implementation in CPython.
 The `history <https://configparser.readthedocs.io/en/latest/history.html>`_
 serves as a reference indicating which versions incorporate
 which upstream functionality.
 
 Prior to the ``4.0.0`` release, `another scheme
 <https://github.com/jaraco/configparser/blob/3.8.1/README.rst#versioning>`_
 was used to associate the CPython and backports releases.
 
 Maintenance
------------
+===========
 
 This backport was originally authored by Łukasz Langa, the current vanilla
 ``configparser`` maintainer for CPython and is currently maintained by
 Jason R. Coombs:
 
 * `configparser repository <https://github.com/jaraco/configparser>`_
 
 * `configparser issue tracker <https://github.com/jaraco/configparser/issues>`_
 
-For Enterprise
-==============
-
-Available as part of the Tidelift Subscription.
-
-This project and the maintainers of thousands of other packages are working with Tidelift to deliver one enterprise subscription that covers all of the open source you use.
-
-`Learn more <https://tidelift.com/subscription/pkg/pypi-configparser?utm_source=pypi-configparser&utm_medium=referral&utm_campaign=github>`_.
-
-Security Contact
-----------------
-
-To report a security vulnerability, please use the
-`Tidelift security contact <https://tidelift.com/security>`_.
-Tidelift will coordinate the fix and disclosure.
-
 Conversion Process
-------------------
+==================
 
 This section is technical and should bother you only if you are wondering how
 this backport is produced. If the implementation details of this backport are
 not important for you, feel free to ignore the following content.
 
 The project takes the following branching approach:
 
@@ -220,15 +205,15 @@
 
 4. Make any compatibility changes on ``main``. Run tests. Commit.
 
 5. Update the docs and release the new version.
 
 
 Footnotes
----------
+=========
 
 .. [1] To somewhat ease migration, passing bytestrings is still supported but
        they are converted to Unicode for internal storage anyway. This means
        that for the vast majority of strings used in configuration files, it
        won't matter if you pass them as bytestrings or Unicode. However, if you
        pass a bytestring that cannot be converted to Unicode using the naive
        ASCII codec, a ``UnicodeDecodeError`` will be raised. This is purposeful
@@ -245,7 +230,16 @@
        once the bytes are read and properly decoded, all you have is text.  This
        is especially powerful when you start interacting with multiple data
        sources.  Even if each of them uses a different encoding, inside your
        application data is held in abstract text form.  You can program your
        business logic without worrying about which data came from which source.
        You can freely exchange the data you store between sources.  Only
        reading/writing files requires encoding your text to bytes.
+
+For Enterprise
+==============
+
+Available as part of the Tidelift Subscription.
+
+This project and the maintainers of thousands of other packages are working with Tidelift to deliver one enterprise subscription that covers all of the open source you use.
+
+`Learn more <https://tidelift.com/subscription/pkg/pypi-configparser?utm_source=pypi-configparser&utm_medium=referral&utm_campaign=github>`_.
```

### Comparing `configparser-5.3.0/README.rst` & `configparser-6.0.0/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 .. image:: https://img.shields.io/pypi/v/configparser.svg
-   :target: `PyPI link`_
+   :target: https://pypi.org/project/configparser
 
 .. image:: https://img.shields.io/pypi/pyversions/configparser.svg
-   :target: `PyPI link`_
-
-.. _PyPI link: https://pypi.org/project/configparser
 
 .. image:: https://github.com/jaraco/configparser/workflows/tests/badge.svg
    :target: https://github.com/jaraco/configparser/actions?query=workflow%3A%22tests%22
    :alt: tests
 
+.. image:: https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json
+    :target: https://github.com/astral-sh/ruff
+    :alt: Ruff
+
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
    :target: https://github.com/psf/black
    :alt: Code style: Black
 
 .. image:: https://readthedocs.org/projects/configparser/badge/?version=latest
    :target: https://configparser.readthedocs.io/en/latest/?badge=latest
 
-.. image:: https://img.shields.io/badge/skeleton-2022-informational
+.. image:: https://img.shields.io/badge/skeleton-2023-informational
    :target: https://blog.jaraco.com/skeleton
 
 .. image:: https://tidelift.com/badges/package/pypi/configparser
    :target: https://tidelift.com/subscription/pkg/pypi-configparser?utm_source=pypi-configparser&utm_medium=readme
 
 
 This package is a backport of the refreshed and enhanced ConfigParser from
@@ -35,15 +36,15 @@
 
   import configparser
 
 For detailed documentation consult the vanilla version at
 http://docs.python.org/3/library/configparser.html.
 
 Why you'll love ``configparser``
---------------------------------
+================================
 
 Whereas almost completely compatible with its older brother, ``configparser``
 sports a bunch of interesting new features:
 
 * full mapping protocol access (`more info
   <http://docs.python.org/3/library/configparser.html#mapping-protocol-access>`_)::
 
@@ -107,15 +108,15 @@
   the whole configuration (multiple sections) is now a single line of code. Same
   goes for copying data from another ``ConfigParser`` instance, thanks to its
   mapping protocol support.
 
 * many smaller tweaks, updates and fixes
 
 A few words about Unicode
--------------------------
+=========================
 
 ``configparser`` comes from Python 3 and as such it works well with Unicode.
 The library is generally cleaned up in terms of internal data storage and
 reading/writing files.  There are a couple of incompatibilities with the old
 ``ConfigParser`` due to that. However, the work required to migrate is well
 worth it as it shows the issues that would likely come up during migration of
 your project to Python 3.
@@ -124,56 +125,40 @@
 gives you the certainty that what's stored in a configuration object is text.
 Once your configuration is read, the rest of your application doesn't have to
 deal with encoding issues. All you have is text [2]_. The only two phases when
 you should explicitly state encoding is when you either read from an external
 source (e.g. a file) or write back.
 
 Versioning
-----------
+==========
 
 This project uses `semver <https://semver.org/spec/v2.0.0.html>`_ to
 communicate the impact of various releases while periodically syncing
 with the upstream implementation in CPython.
 The `history <https://configparser.readthedocs.io/en/latest/history.html>`_
 serves as a reference indicating which versions incorporate
 which upstream functionality.
 
 Prior to the ``4.0.0`` release, `another scheme
 <https://github.com/jaraco/configparser/blob/3.8.1/README.rst#versioning>`_
 was used to associate the CPython and backports releases.
 
 Maintenance
------------
+===========
 
 This backport was originally authored by Łukasz Langa, the current vanilla
 ``configparser`` maintainer for CPython and is currently maintained by
 Jason R. Coombs:
 
 * `configparser repository <https://github.com/jaraco/configparser>`_
 
 * `configparser issue tracker <https://github.com/jaraco/configparser/issues>`_
 
-For Enterprise
-==============
-
-Available as part of the Tidelift Subscription.
-
-This project and the maintainers of thousands of other packages are working with Tidelift to deliver one enterprise subscription that covers all of the open source you use.
-
-`Learn more <https://tidelift.com/subscription/pkg/pypi-configparser?utm_source=pypi-configparser&utm_medium=referral&utm_campaign=github>`_.
-
-Security Contact
-----------------
-
-To report a security vulnerability, please use the
-`Tidelift security contact <https://tidelift.com/security>`_.
-Tidelift will coordinate the fix and disclosure.
-
 Conversion Process
-------------------
+==================
 
 This section is technical and should bother you only if you are wondering how
 this backport is produced. If the implementation details of this backport are
 not important for you, feel free to ignore the following content.
 
 The project takes the following branching approach:
 
@@ -199,15 +184,15 @@
 
 4. Make any compatibility changes on ``main``. Run tests. Commit.
 
 5. Update the docs and release the new version.
 
 
 Footnotes
----------
+=========
 
 .. [1] To somewhat ease migration, passing bytestrings is still supported but
        they are converted to Unicode for internal storage anyway. This means
        that for the vast majority of strings used in configuration files, it
        won't matter if you pass them as bytestrings or Unicode. However, if you
        pass a bytestring that cannot be converted to Unicode using the naive
        ASCII codec, a ``UnicodeDecodeError`` will be raised. This is purposeful
@@ -224,7 +209,16 @@
        once the bytes are read and properly decoded, all you have is text.  This
        is especially powerful when you start interacting with multiple data
        sources.  Even if each of them uses a different encoding, inside your
        application data is held in abstract text form.  You can program your
        business logic without worrying about which data came from which source.
        You can freely exchange the data you store between sources.  Only
        reading/writing files requires encoding your text to bytes.
+
+For Enterprise
+==============
+
+Available as part of the Tidelift Subscription.
+
+This project and the maintainers of thousands of other packages are working with Tidelift to deliver one enterprise subscription that covers all of the open source you use.
+
+`Learn more <https://tidelift.com/subscription/pkg/pypi-configparser?utm_source=pypi-configparser&utm_medium=referral&utm_campaign=github>`_.
```

### Comparing `configparser-5.3.0/configparser.rst` & `configparser-6.0.0/configparser.rst`

 * *Files 4% similar despite different names*

```diff
@@ -29,21 +29,25 @@
 .. note::
 
    This library does *not* interpret or write the value-type prefixes used in
    the Windows Registry extended version of INI syntax.
 
 .. seealso::
 
+   Module :mod:`tomllib`
+      TOML is a well-specified format for application configuration files.
+      It is specifically designed to be an improved version of INI.
+
    Module :mod:`shlex`
-      Support for creating Unix shell-like mini-languages which can be used as
-      an alternate format for application configuration files.
+      Support for creating Unix shell-like mini-languages which can also
+      be used for application configuration files.
 
    Module :mod:`json`
-      The json module implements a subset of JavaScript syntax which can also
-      be used for this purpose.
+      The ``json`` module implements a subset of JavaScript syntax which is
+      sometimes used for configuration, but does not support comments.
 
 
 .. testsetup::
 
    import configparser
 
 .. testcleanup::
@@ -61,18 +65,18 @@
 
    [DEFAULT]
    ServerAliveInterval = 45
    Compression = yes
    CompressionLevel = 9
    ForwardX11 = yes
 
-   [bitbucket.org]
+   [forge.example]
    User = hg
 
-   [topsecret.server.com]
+   [topsecret.server.example]
    Port = 50022
    ForwardX11 = no
 
 The structure of INI files is described `in the following section
 <#supported-ini-file-structure>`_.  Essentially, the file
 consists of sections, each of which contains keys with values.
 :mod:`configparser` classes can read and write such files.  Let's start by
@@ -81,18 +85,18 @@
 .. doctest::
 
    >>> import configparser
    >>> config = configparser.ConfigParser()
    >>> config['DEFAULT'] = {'ServerAliveInterval': '45',
    ...                      'Compression': 'yes',
    ...                      'CompressionLevel': '9'}
-   >>> config['bitbucket.org'] = {}
-   >>> config['bitbucket.org']['User'] = 'hg'
-   >>> config['topsecret.server.com'] = {}
-   >>> topsecret = config['topsecret.server.com']
+   >>> config['forge.example'] = {}
+   >>> config['forge.example']['User'] = 'hg'
+   >>> config['topsecret.server.example'] = {}
+   >>> topsecret = config['topsecret.server.example']
    >>> topsecret['Port'] = '50022'     # mutates the parser
    >>> topsecret['ForwardX11'] = 'no'  # same here
    >>> config['DEFAULT']['ForwardX11'] = 'yes'
    >>> with open('example.ini', 'w') as configfile:
    ...   config.write(configfile)
    ...
 
@@ -107,36 +111,36 @@
 
    >>> config = configparser.ConfigParser()
    >>> config.sections()
    []
    >>> config.read('example.ini')
    ['example.ini']
    >>> config.sections()
-   ['bitbucket.org', 'topsecret.server.com']
-   >>> 'bitbucket.org' in config
+   ['forge.example', 'topsecret.server.example']
+   >>> 'forge.example' in config
    True
-   >>> 'bytebong.com' in config
+   >>> 'python.org' in config
    False
-   >>> config['bitbucket.org']['User']
+   >>> config['forge.example']['User']
    'hg'
    >>> config['DEFAULT']['Compression']
    'yes'
-   >>> topsecret = config['topsecret.server.com']
+   >>> topsecret = config['topsecret.server.example']
    >>> topsecret['ForwardX11']
    'no'
    >>> topsecret['Port']
    '50022'
-   >>> for key in config['bitbucket.org']:  # doctest: +SKIP
+   >>> for key in config['forge.example']:  # doctest: +SKIP
    ...     print(key)
    user
    compressionlevel
    serveraliveinterval
    compression
    forwardx11
-   >>> config['bitbucket.org']['ForwardX11']
+   >>> config['forge.example']['ForwardX11']
    'yes'
 
 As we can see above, the API is pretty straightforward.  The only bit of magic
 involves the ``DEFAULT`` section which provides default values for all other
 sections [1]_.  Note also that keys in sections are
 case-insensitive and stored in lowercase [1]_.
 
@@ -146,23 +150,23 @@
 configuration while the previously existing keys are retained.
 
 .. doctest::
 
    >>> another_config = configparser.ConfigParser()
    >>> another_config.read('example.ini')
    ['example.ini']
-   >>> another_config['topsecret.server.com']['Port']
+   >>> another_config['topsecret.server.example']['Port']
    '50022'
-   >>> another_config.read_string("[topsecret.server.com]\nPort=48484")
-   >>> another_config['topsecret.server.com']['Port']
+   >>> another_config.read_string("[topsecret.server.example]\nPort=48484")
+   >>> another_config['topsecret.server.example']['Port']
    '48484'
-   >>> another_config.read_dict({"topsecret.server.com": {"Port": 21212}})
-   >>> another_config['topsecret.server.com']['Port']
+   >>> another_config.read_dict({"topsecret.server.example": {"Port": 21212}})
+   >>> another_config['topsecret.server.example']['Port']
    '21212'
-   >>> another_config['topsecret.server.com']['ForwardX11']
+   >>> another_config['topsecret.server.example']['ForwardX11']
    'no'
 
 This behaviour is equivalent to a :meth:`ConfigParser.read` call with several
 files passed to the *filenames* parameter.
 
 
 Supported Datatypes
@@ -187,17 +191,17 @@
 recognizes Boolean values from ``'yes'``/``'no'``, ``'on'``/``'off'``,
 ``'true'``/``'false'`` and ``'1'``/``'0'`` [1]_.  For example:
 
 .. doctest::
 
    >>> topsecret.getboolean('ForwardX11')
    False
-   >>> config['bitbucket.org'].getboolean('ForwardX11')
+   >>> config['forge.example'].getboolean('ForwardX11')
    True
-   >>> config.getboolean('bitbucket.org', 'Compression')
+   >>> config.getboolean('forge.example', 'Compression')
    True
 
 Apart from :meth:`~ConfigParser.getboolean`, config parsers also
 provide equivalent :meth:`~ConfigParser.getint` and
 :meth:`~ConfigParser.getfloat` methods.  You can register your own
 converters and customize the provided ones. [1]_
 
@@ -216,30 +220,30 @@
    >>> topsecret.get('Cipher')
    >>> topsecret.get('Cipher', '3des-cbc')
    '3des-cbc'
 
 Please note that default values have precedence over fallback values.
 For instance, in our example the ``'CompressionLevel'`` key was
 specified only in the ``'DEFAULT'`` section.  If we try to get it from
-the section ``'topsecret.server.com'``, we will always get the default,
+the section ``'topsecret.server.example'``, we will always get the default,
 even if we specify a fallback:
 
 .. doctest::
 
    >>> topsecret.get('CompressionLevel', '3')
    '9'
 
 One more thing to be aware of is that the parser-level :meth:`get` method
 provides a custom, more complex interface, maintained for backwards
 compatibility.  When using this method, a fallback value can be provided via
 the ``fallback`` keyword-only argument:
 
 .. doctest::
 
-   >>> config.get('bitbucket.org', 'monster',
+   >>> config.get('forge.example', 'monster',
    ...            fallback='No such things as monsters')
    'No such things as monsters'
 
 The same ``fallback`` argument can be used with the
 :meth:`~ConfigParser.getint`, :meth:`~ConfigParser.getfloat` and
 :meth:`~ConfigParser.getboolean` methods, for example:
 
@@ -1202,36 +1206,14 @@
          cfgparser = ConfigParser()
          cfgparser.optionxform = str
 
       Note that when reading configuration files, whitespace around the option
       names is stripped before :meth:`optionxform` is called.
 
 
-   .. method:: readfp(fp, filename=None)
-
-      .. deprecated:: 3.2
-         Use :meth:`read_file` instead.
-
-      .. versionchanged:: 3.2
-         :meth:`readfp` now iterates on *fp* instead of calling ``fp.readline()``.
-
-      For existing code calling :meth:`readfp` with arguments which don't
-      support iteration, the following generator may be used as a wrapper
-      around the file-like object::
-
-         def readline_generator(fp):
-             line = fp.readline()
-             while line:
-                 yield line
-                 line = fp.readline()
-
-      Instead of ``parser.readfp(fp)`` use
-      ``parser.read_file(readline_generator(fp))``.
-
-
 .. data:: MAX_INTERPOLATION_DEPTH
 
    The maximum depth for recursive interpolation for :meth:`get` when the *raw*
    parameter is false.  This is relevant only when the default *interpolation*
    is used.
 
 
@@ -1357,17 +1339,16 @@
    headers.
 
 
 .. exception:: ParsingError
 
    Exception raised when errors occur attempting to parse a file.
 
-   .. versionchanged:: 3.2
-      The ``filename`` attribute and :meth:`__init__` argument were renamed to
-      ``source`` for consistency.
-
+.. versionchanged:: 3.12
+   The ``filename`` attribute and :meth:`__init__` constructor argument were
+   removed.  They have been available using the name ``source`` since 3.2.
 
 .. rubric:: Footnotes
 
 .. [1] Config parsers allow for heavy customization.  If you are interested in
        changing the behaviour outlined by the footnote reference, consult the
        `Customizing Parser Behaviour`_ section.
```

### Comparing `configparser-5.3.0/docs/conf.py` & `configparser-6.0.0/docs/conf.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,19 @@
-#!/usr/bin/env python3
-# -*- coding: utf-8 -*-
-
-extensions = ['sphinx.ext.autodoc', 'jaraco.packaging.sphinx', 'rst.linker']
+extensions = [
+    'sphinx.ext.autodoc',
+    'jaraco.packaging.sphinx',
+]
 
 master_doc = "index"
+html_theme = "furo"
 
+# Link dates and other references in the changelog
+extensions += ['rst.linker']
 link_files = {
-    '../CHANGES.rst': dict(
+    '../NEWS.rst': dict(
         using=dict(GH='https://github.com'),
         replace=[
             dict(
                 pattern=r'(Issue #|\B#)(?P<issue>\d+)',
                 url='{package_url}/issues/{issue}',
             ),
             dict(
@@ -25,18 +28,21 @@
                 pattern=r'Python #(?P<python>\d+)',
                 url='https://bugs.python.org/issue{python}',
             ),
         ],
     )
 }
 
-# Be strict about any broken references:
+# Be strict about any broken references
 nitpicky = True
 
 # Include Python intersphinx mapping to prevent failures
 # jaraco/skeleton#51
 extensions += ['sphinx.ext.intersphinx']
 intersphinx_mapping = {
     'python': ('https://docs.python.org/3', None),
 }
 
+# Preserve authored syntax for defaults
+autodoc_preserve_defaults = True
+
 extensions += ['jaraco.tidelift']
```

### Comparing `configparser-5.3.0/setup.cfg` & `configparser-6.0.0/setup.cfg`

 * *Files 26% similar despite different names*

```diff
@@ -14,47 +14,45 @@
 	Intended Audience :: Developers
 	License :: OSI Approved :: MIT License
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3 :: Only
 
 [options]
 packages = find_namespace:
-package_dir = 
-	=src
-py_modules = configparser
 include_package_data = true
-python_requires = >=3.7
+python_requires = >=3.8
 install_requires = 
 
 [options.packages.find]
-where = src
 exclude = 
 	build*
 	dist*
 	docs*
 	tests*
 
 [options.extras_require]
 testing = 
 	pytest >= 6
 	pytest-checkdocs >= 2.4
-	pytest-flake8
-	flake8 < 5
 	pytest-black >= 0.3.7; \
 	python_implementation != "PyPy"
 	pytest-cov
 	pytest-mypy >= 0.9.1; \
 	python_implementation != "PyPy"
-	pytest-enabler >= 1.3
+	pytest-enabler >= 2.2
+	pytest-ruff
 	
 	types-backports
 docs = 
-	sphinx
-	jaraco.packaging >= 9
+	sphinx >= 3.5
+	jaraco.packaging >= 9.3
 	rst.linker >= 1.9
+	furo
+	sphinx-lint
+	
 	jaraco.tidelift >= 1.4
 
 [options.entry_points]
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `configparser-5.3.0/src/backports/configparser/__init__.py` & `configparser-6.0.0/backports/configparser/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,54 +15,55 @@
     methods:
 
     __init__(defaults=None, dict_type=_default_dict, allow_no_value=False,
              delimiters=('=', ':'), comment_prefixes=('#', ';'),
              inline_comment_prefixes=None, strict=True,
              empty_lines_in_values=True, default_section='DEFAULT',
              interpolation=<unset>, converters=<unset>):
-        Create the parser. When `defaults' is given, it is initialized into the
+
+        Create the parser. When `defaults` is given, it is initialized into the
         dictionary or intrinsic defaults. The keys must be strings, the values
         must be appropriate for %()s string interpolation.
 
-        When `dict_type' is given, it will be used to create the dictionary
+        When `dict_type` is given, it will be used to create the dictionary
         objects for the list of sections, for the options within a section, and
         for the default values.
 
-        When `delimiters' is given, it will be used as the set of substrings
+        When `delimiters` is given, it will be used as the set of substrings
         that divide keys from values.
 
-        When `comment_prefixes' is given, it will be used as the set of
+        When `comment_prefixes` is given, it will be used as the set of
         substrings that prefix comments in empty lines. Comments can be
         indented.
 
-        When `inline_comment_prefixes' is given, it will be used as the set of
+        When `inline_comment_prefixes` is given, it will be used as the set of
         substrings that prefix comments in non-empty lines.
 
         When `strict` is True, the parser won't allow for any section or option
         duplicates while reading from a single source (file, string or
         dictionary). Default is True.
 
-        When `empty_lines_in_values' is False (default: True), each empty line
+        When `empty_lines_in_values` is False (default: True), each empty line
         marks the end of an option. Otherwise, internal empty lines of
         a multiline option are kept as part of the value.
 
-        When `allow_no_value' is True (default: False), options without
+        When `allow_no_value` is True (default: False), options without
         values are accepted; the value presented for these is None.
 
-        When `default_section' is given, the name of the special section is
+        When `default_section` is given, the name of the special section is
         named accordingly. By default it is called ``"DEFAULT"`` but this can
         be customized to point to any other valid section name. Its current
         value can be retrieved using the ``parser_instance.default_section``
         attribute and may be modified at runtime.
 
         When `interpolation` is given, it should be an Interpolation subclass
         instance. It will be used as the handler for option value
         pre-processing when using getters. RawConfigParser objects don't do
         any sort of interpolation, whereas ConfigParser uses an instance of
-        BasicInterpolation. The library also provides a ``zc.buildbot``
+        BasicInterpolation. The library also provides a ``zc.buildout``
         inspired ExtendedInterpolation implementation.
 
         When `converters` is given, it should be a dictionary where each key
         represents the name of a type converter and each value is a callable
         implementing the conversion from string to the desired datatype. Every
         converter gets its corresponding get*() method on the parser object and
         section proxies.
@@ -83,15 +84,15 @@
         Read and parse the iterable of named configuration files, given by
         name.  A single filename is also allowed.  Non-existing files
         are ignored.  Return list of successfully read files.
 
     read_file(f, filename=None)
         Read and parse one configuration file, given as a file object.
         The filename defaults to f.name; it is only used in error
-        messages (if f has no `name' attribute, the string `<???>' is used).
+        messages (if f has no `name` attribute, the string `<???>` is used).
 
     read_string(string)
         Read configuration from a given string.
 
     read_dict(dictionary)
         Read configuration from a dictionary. Keys are section names,
         values are dictionaries with keys and values that should be present
@@ -99,17 +100,17 @@
         and their keys will be added in order. Values are automatically
         converted to strings.
 
     get(section, option, raw=False, vars=None, fallback=_UNSET)
         Return a string value for the named option.  All % interpolations are
         expanded in the return values, based on the defaults passed into the
         constructor and the DEFAULT section.  Additional substitutions may be
-        provided using the `vars' argument, which must be a dictionary whose
-        contents override any pre-existing defaults. If `option' is a key in
-        `vars', the value from `vars' is used.
+        provided using the `vars` argument, which must be a dictionary whose
+        contents override any pre-existing defaults. If `option` is a key in
+        `vars`, the value from `vars` is used.
 
     getint(section, options, raw=False, vars=None, fallback=_UNSET)
         Like get(), but convert value to an integer.
 
     getfloat(section, options, raw=False, vars=None, fallback=_UNSET)
         Like get(), but convert value to a float.
 
@@ -130,52 +131,51 @@
         Remove the given option from the given section.
 
     set(section, option, value)
         Set the given option.
 
     write(fp, space_around_delimiters=True)
         Write the configuration state in .ini format. If
-        `space_around_delimiters' is True (the default), delimiters
+        `space_around_delimiters` is True (the default), delimiters
         between keys and values are surrounded by spaces.
 """
 
 from collections.abc import MutableMapping
 from collections import ChainMap as _ChainMap
 import functools
 from .compat import io
 import itertools
 import os
 import re
 import sys
 import warnings
 
 
-__all__ = [
+__all__ = (
     "NoSectionError",
     "DuplicateOptionError",
     "DuplicateSectionError",
     "NoOptionError",
     "InterpolationError",
     "InterpolationDepthError",
     "InterpolationMissingOptionError",
     "InterpolationSyntaxError",
     "ParsingError",
     "MissingSectionHeaderError",
     "ConfigParser",
-    "SafeConfigParser",
     "RawConfigParser",
     "Interpolation",
     "BasicInterpolation",
     "ExtendedInterpolation",
     "LegacyInterpolation",
     "SectionProxy",
     "ConverterMapping",
     "DEFAULTSECT",
     "MAX_INTERPOLATION_DEPTH",
-]
+)
 
 _default_dict = dict
 DEFAULTSECT = "DEFAULT"
 
 MAX_INTERPOLATION_DEPTH = 10
 
 
@@ -309,52 +309,20 @@
         InterpolationError.__init__(self, option, section, msg)
         self.args = (option, section, rawval)
 
 
 class ParsingError(Error):
     """Raised when a configuration file does not follow legal syntax."""
 
-    def __init__(self, source=None, filename=None):
-        # Exactly one of `source'/`filename' arguments has to be given.
-        # `filename' kept for compatibility.
-        if filename and source:
-            raise ValueError(
-                "Cannot specify both `filename' and `source'. " "Use `source'."
-            )
-        elif not filename and not source:
-            raise ValueError("Required argument `source' not given.")
-        elif filename:
-            source = filename
-        Error.__init__(self, 'Source contains parsing errors: %r' % source)
+    def __init__(self, source):
+        super().__init__(f'Source contains parsing errors: {source!r}')
         self.source = source
         self.errors = []
         self.args = (source,)
 
-    @property
-    def filename(self):
-        """Deprecated, use `source'."""
-        warnings.warn(
-            "The 'filename' attribute will be removed in Python 3.12. "
-            "Use 'source' instead.",
-            DeprecationWarning,
-            stacklevel=2,
-        )
-        return self.source
-
-    @filename.setter
-    def filename(self, value):
-        """Deprecated, user `source'."""
-        warnings.warn(
-            "The 'filename' attribute will be removed in Python 3.12. "
-            "Use 'source' instead.",
-            DeprecationWarning,
-            stacklevel=2,
-        )
-        self.source = value
-
     def append(self, lineno, line):
         self.errors.append((lineno, line))
         self.message += '\n\t[line %2d]: %s' % (lineno, line)
 
 
 class MissingSectionHeaderError(ParsingError):
     """Raised when a key-value pair is found before any section header."""
@@ -368,15 +336,15 @@
         self.source = filename
         self.lineno = lineno
         self.line = line
         self.args = (filename, lineno, line)
 
 
 # Used in parser getters to indicate the default behaviour when a specific
-# option is not found it to raise an exception. Created to enable `None' as
+# option is not found it to raise an exception. Created to enable `None` as
 # a valid fallback value.
 _UNSET = object()
 
 
 class Interpolation:
     """Dummy interpolation that passes the value through with no changes."""
 
@@ -402,15 +370,15 @@
     For example:
 
         something: %(dir)s/whatever
 
     would resolve the "%(dir)s" to the value of dir.  All reference
     expansions are done late, on demand. If a user needs to use a bare % in
     a configuration file, she can escape it by writing %%. Other % usage
-    is considered a user error and raises `InterpolationSyntaxError'."""
+    is considered a user error and raises `InterpolationSyntaxError`."""
 
     _KEYCRE = re.compile(r"%\(([^)]+)\)s")
 
     def before_get(self, parser, section, option, value, defaults):
         L = []
         self._interpolate_some(parser, option, L, value, section, defaults, 1)
         return ''.join(L)
@@ -472,15 +440,15 @@
                     section,
                     "'%%' must be followed by '%%' or '(', " "found: %r" % (rest,),
                 )
 
 
 class ExtendedInterpolation(Interpolation):
     """Advanced variant of interpolation, supports the syntax used by
-    `zc.buildout'. Enables interpolation between sections."""
+    `zc.buildout`. Enables interpolation between sections."""
 
     _KEYCRE = re.compile(r"\$\{([^}]+)\}")
 
     def before_get(self, parser, section, option, value, defaults):
         L = []
         self._interpolate_some(parser, option, L, value, section, defaults, 1)
         return ''.join(L)
@@ -670,15 +638,14 @@
         inline_comment_prefixes=None,
         strict=True,
         empty_lines_in_values=True,
         default_section=DEFAULTSECT,
         interpolation=_UNSET,
         converters=_UNSET,
     ):
-
         self._dict = dict_type
         self._sections = self._dict()
         self._defaults = self._dict()
         self._converters = ConverterMapping(self)
         self._proxies = self._dict()
         self._proxies[default_section] = SectionProxy(self, default_section)
         self._delimiters = tuple(delimiters)
@@ -775,18 +742,18 @@
                 filename = os.fspath(filename)
             read_ok.append(filename)
         return read_ok
 
     def read_file(self, f, source=None):
         """Like read() but the argument must be a file-like object.
 
-        The `f' argument must be iterable, returning one line at a time.
-        Optional second argument is the `source' specifying the name of the
-        file being read. If not given, it is taken from f.name. If `f' has no
-        `name' attribute, `<???>' is used.
+        The `f` argument must be iterable, returning one line at a time.
+        Optional second argument is the `source` specifying the name of the
+        file being read. If not given, it is taken from f.name. If `f` has no
+        `name` attribute, `<???>` is used.
         """
         if source is None:
             try:
                 source = f.name
             except AttributeError:
                 source = '<???>'
         self._read(f, source)
@@ -802,15 +769,15 @@
         Keys are section names, values are dictionaries with keys and values
         that should be present in the section. If the used dictionary type
         preserves order, sections and their keys will be added in order.
 
         All types held in the dictionary are converted to strings during
         reading, including section names, option names and keys.
 
-        Optional second argument is the `source' specifying the name of the
+        Optional second argument is the `source` specifying the name of the
         dictionary being read.
         """
         elements_added = set()
         for section, keys in dictionary.items():
             section = str(section)
             try:
                 self.add_section(section)
@@ -823,36 +790,26 @@
                 if value is not None:
                     value = str(value)
                 if self._strict and (section, key) in elements_added:
                     raise DuplicateOptionError(section, key, source)
                 elements_added.add((section, key))
                 self.set(section, key, value)
 
-    def readfp(self, fp, filename=None):
-        """Deprecated, use read_file instead."""
-        warnings.warn(
-            "This method will be removed in Python 3.12. "
-            "Use 'parser.read_file()' instead.",
-            DeprecationWarning,
-            stacklevel=2,
-        )
-        self.read_file(fp, source=filename)
-
     def get(self, section, option, *, raw=False, vars=None, fallback=_UNSET):
         """Get an option value for a given section.
 
-        If `vars' is provided, it must be a dictionary. The option is looked up
-        in `vars' (if provided), `section', and in `DEFAULTSECT' in that order.
-        If the key is not found and `fallback' is provided, it is used as
-        a fallback value. `None' can be provided as a `fallback' value.
+        If `vars` is provided, it must be a dictionary. The option is looked up
+        in `vars` (if provided), `section`, and in `DEFAULTSECT` in that order.
+        If the key is not found and `fallback` is provided, it is used as
+        a fallback value. `None` can be provided as a `fallback` value.
 
-        If interpolation is enabled and the optional argument `raw' is False,
+        If interpolation is enabled and the optional argument `raw` is False,
         all interpolations are expanded in the return values.
 
-        Arguments `raw', `vars', and `fallback' are keyword only.
+        Arguments `raw`, `vars`, and `fallback` are keyword only.
 
         The section DEFAULT is special.
         """
         try:
             d = self._unify_values(section, vars)
         except NoSectionError:
             if fallback is _UNSET:
@@ -915,16 +872,16 @@
         )
 
     def items(self, section=_UNSET, raw=False, vars=None):
         """Return a list of (name, value) tuples for each option in a section.
 
         All % interpolations are expanded in the return values, based on the
         defaults passed into the constructor, unless the optional argument
-        `raw' is true.  Additional substitutions may be provided using the
-        `vars' argument, which must be a dictionary whose contents overrides
+        `raw` is true.  Additional substitutions may be provided using the
+        `vars` argument, which must be a dictionary whose contents overrides
         any pre-existing defaults.
 
         The section DEFAULT is special.
         """
         if section is _UNSET:
             return super(RawConfigParser, self).items()
         d = self._defaults.copy()
@@ -963,16 +920,16 @@
         raise KeyError
 
     def optionxform(self, optionstr):
         return optionstr.lower()
 
     def has_option(self, section, option):
         """Check for the existence of a given option in a given section.
-        If the specified `section' is None or an empty string, DEFAULT is
-        assumed. If the specified `section' does not exist, returns False."""
+        If the specified `section` is None or an empty string, DEFAULT is
+        assumed. If the specified `section` does not exist, returns False."""
         if not section or section == self.default_section:
             option = self.optionxform(option)
             return option in self._defaults
         elif section not in self._sections:
             return False
         else:
             option = self.optionxform(option)
@@ -990,15 +947,15 @@
             except KeyError:
                 raise NoSectionError(section) from None
         sectdict[self.optionxform(option)] = value
 
     def write(self, fp, space_around_delimiters=True):
         """Write an .ini-format representation of the configuration state.
 
-        If `space_around_delimiters' is True (the default), delimiters
+        If `space_around_delimiters` is True (the default), delimiters
         between keys and values are surrounded by spaces.
 
         Please note that comments in the original configuration file are not
         preserved when writing the configuration back.
         """
         if space_around_delimiters:
             d = " {} ".format(self._delimiters[0])
@@ -1006,15 +963,15 @@
             d = self._delimiters[0]
         if self._defaults:
             self._write_section(fp, self.default_section, self._defaults.items(), d)
         for section in self._sections:
             self._write_section(fp, section, self._sections[section].items(), d)
 
     def _write_section(self, fp, section_name, section_items, delimiter):
-        """Write a single section to the specified `fp'."""
+        """Write a single section to the specified `fp`."""
         fp.write("[{}]\n".format(section_name))
         for key, value in section_items:
             value = self._interpolation.before_write(self, section_name, key, value)
             if value is not None or not self._allow_no_value:
                 value = delimiter + str(value).replace('\n', '\n\t')
             else:
                 value = ""
@@ -1079,24 +1036,24 @@
         # XXX does it break when underlying container state changed?
         return itertools.chain((self.default_section,), self._sections.keys())
 
     def _read(self, fp, fpname):  # noqa: C901
         """Parse a sectioned configuration file.
 
         Each section in a configuration file contains a header, indicated by
-        a name in square brackets (`[]'), plus key/value options, indicated by
-        `name' and `value' delimited with a specific substring (`=' or `:' by
+        a name in square brackets (`[]`), plus key/value options, indicated by
+        `name` and `value` delimited with a specific substring (`=` or `:` by
         default).
 
         Values can span multiple lines, as long as they are indented deeper
         than the first line of the value. Depending on the parser's mode, blank
         lines may be treated as parts of multiline values or ignored.
 
         Configuration files may include comments, prefixed by specific
-        characters (`#' and `;' by default). Comments may appear on their own
+        characters (`#` and `;` by default). Comments may appear on their own
         in an otherwise empty line or may be entered in lines holding values or
         section names. Please note that comments get stripped off when reading
         configuration files.
         """
         elements_added = set()
         cursect = None  # None, or a dictionary
         sectname = None
@@ -1305,28 +1262,14 @@
             hold_interpolation = self._interpolation
             self._interpolation = Interpolation()
             self.read_dict({self.default_section: defaults})
         finally:
             self._interpolation = hold_interpolation
 
 
-class SafeConfigParser(ConfigParser):
-    """ConfigParser alias for backwards compatibility purposes."""
-
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-        warnings.warn(
-            "The SafeConfigParser class has been renamed to ConfigParser "
-            "in Python 3.2. This alias will be removed in Python 3.12."
-            " Use ConfigParser directly instead.",
-            DeprecationWarning,
-            stacklevel=2,
-        )
-
-
 class SectionProxy(MutableMapping):
     """A proxy for a single section from a parser."""
 
     def __init__(self, parser, name):
         """Creates a view on a section of the specified `name` in `parser`."""
         self._parser = parser
         self._name = name
```

### Comparing `configparser-5.3.0/src/cfgparser.2` & `configparser-6.0.0/tests/cfgparser.2`

 * *Files identical despite different names*

### Comparing `configparser-5.3.0/src/cfgparser.3` & `configparser-6.0.0/tests/cfgparser.3`

 * *Files identical despite different names*

### Comparing `configparser-5.3.0/src/compat.py` & `configparser-6.0.0/tests/compat.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import test.support
 import contextlib
 import sys
 import types
 
 
 def check__all__(*args, **kwargs):
-    if sys.version_info < (3, 10):
+    if sys.version_info < (3, 10):  # pragma: no cover
         with contextlib.suppress(KeyError):
             kwargs.update(blacklist=kwargs.pop('not_exported'))
     return test.support.check__all__(*args, **kwargs)
 
 
 support = types.SimpleNamespace(**dict(vars(test.support), check__all__=check__all__))
 
 
 try:
     from test.support import os_helper
-except ImportError:
+except ImportError:  # pragma: no cover
     # Python 3.9
     import test.support as os_helper  # noqa: F401
```

### Comparing `configparser-5.3.0/src/configparser.egg-info/PKG-INFO` & `configparser-6.0.0/configparser.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,48 +1,49 @@
 Metadata-Version: 2.1
 Name: configparser
-Version: 5.3.0
+Version: 6.0.0
 Summary: Updated configparser from stdlib for earlier Pythons.
 Home-page: https://github.com/jaraco/configparser/
 Author: Łukasz Langa
 Author-email: lukasz@langa.pl
 Maintainer: Jason R. Coombs
 Maintainer-email: jaraco@jaraco.com
 Keywords: configparser ini parsing conf cfg configuration file
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Provides-Extra: testing
 Provides-Extra: docs
 License-File: LICENSE
 
 .. image:: https://img.shields.io/pypi/v/configparser.svg
-   :target: `PyPI link`_
+   :target: https://pypi.org/project/configparser
 
 .. image:: https://img.shields.io/pypi/pyversions/configparser.svg
-   :target: `PyPI link`_
-
-.. _PyPI link: https://pypi.org/project/configparser
 
 .. image:: https://github.com/jaraco/configparser/workflows/tests/badge.svg
    :target: https://github.com/jaraco/configparser/actions?query=workflow%3A%22tests%22
    :alt: tests
 
+.. image:: https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json
+    :target: https://github.com/astral-sh/ruff
+    :alt: Ruff
+
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
    :target: https://github.com/psf/black
    :alt: Code style: Black
 
 .. image:: https://readthedocs.org/projects/configparser/badge/?version=latest
    :target: https://configparser.readthedocs.io/en/latest/?badge=latest
 
-.. image:: https://img.shields.io/badge/skeleton-2022-informational
+.. image:: https://img.shields.io/badge/skeleton-2023-informational
    :target: https://blog.jaraco.com/skeleton
 
 .. image:: https://tidelift.com/badges/package/pypi/configparser
    :target: https://tidelift.com/subscription/pkg/pypi-configparser?utm_source=pypi-configparser&utm_medium=readme
 
 
 This package is a backport of the refreshed and enhanced ConfigParser from
@@ -56,15 +57,15 @@
 
   import configparser
 
 For detailed documentation consult the vanilla version at
 http://docs.python.org/3/library/configparser.html.
 
 Why you'll love ``configparser``
---------------------------------
+================================
 
 Whereas almost completely compatible with its older brother, ``configparser``
 sports a bunch of interesting new features:
 
 * full mapping protocol access (`more info
   <http://docs.python.org/3/library/configparser.html#mapping-protocol-access>`_)::
 
@@ -128,15 +129,15 @@
   the whole configuration (multiple sections) is now a single line of code. Same
   goes for copying data from another ``ConfigParser`` instance, thanks to its
   mapping protocol support.
 
 * many smaller tweaks, updates and fixes
 
 A few words about Unicode
--------------------------
+=========================
 
 ``configparser`` comes from Python 3 and as such it works well with Unicode.
 The library is generally cleaned up in terms of internal data storage and
 reading/writing files.  There are a couple of incompatibilities with the old
 ``ConfigParser`` due to that. However, the work required to migrate is well
 worth it as it shows the issues that would likely come up during migration of
 your project to Python 3.
@@ -145,56 +146,40 @@
 gives you the certainty that what's stored in a configuration object is text.
 Once your configuration is read, the rest of your application doesn't have to
 deal with encoding issues. All you have is text [2]_. The only two phases when
 you should explicitly state encoding is when you either read from an external
 source (e.g. a file) or write back.
 
 Versioning
-----------
+==========
 
 This project uses `semver <https://semver.org/spec/v2.0.0.html>`_ to
 communicate the impact of various releases while periodically syncing
 with the upstream implementation in CPython.
 The `history <https://configparser.readthedocs.io/en/latest/history.html>`_
 serves as a reference indicating which versions incorporate
 which upstream functionality.
 
 Prior to the ``4.0.0`` release, `another scheme
 <https://github.com/jaraco/configparser/blob/3.8.1/README.rst#versioning>`_
 was used to associate the CPython and backports releases.
 
 Maintenance
------------
+===========
 
 This backport was originally authored by Łukasz Langa, the current vanilla
 ``configparser`` maintainer for CPython and is currently maintained by
 Jason R. Coombs:
 
 * `configparser repository <https://github.com/jaraco/configparser>`_
 
 * `configparser issue tracker <https://github.com/jaraco/configparser/issues>`_
 
-For Enterprise
-==============
-
-Available as part of the Tidelift Subscription.
-
-This project and the maintainers of thousands of other packages are working with Tidelift to deliver one enterprise subscription that covers all of the open source you use.
-
-`Learn more <https://tidelift.com/subscription/pkg/pypi-configparser?utm_source=pypi-configparser&utm_medium=referral&utm_campaign=github>`_.
-
-Security Contact
-----------------
-
-To report a security vulnerability, please use the
-`Tidelift security contact <https://tidelift.com/security>`_.
-Tidelift will coordinate the fix and disclosure.
-
 Conversion Process
-------------------
+==================
 
 This section is technical and should bother you only if you are wondering how
 this backport is produced. If the implementation details of this backport are
 not important for you, feel free to ignore the following content.
 
 The project takes the following branching approach:
 
@@ -220,15 +205,15 @@
 
 4. Make any compatibility changes on ``main``. Run tests. Commit.
 
 5. Update the docs and release the new version.
 
 
 Footnotes
----------
+=========
 
 .. [1] To somewhat ease migration, passing bytestrings is still supported but
        they are converted to Unicode for internal storage anyway. This means
        that for the vast majority of strings used in configuration files, it
        won't matter if you pass them as bytestrings or Unicode. However, if you
        pass a bytestring that cannot be converted to Unicode using the naive
        ASCII codec, a ``UnicodeDecodeError`` will be raised. This is purposeful
@@ -245,7 +230,16 @@
        once the bytes are read and properly decoded, all you have is text.  This
        is especially powerful when you start interacting with multiple data
        sources.  Even if each of them uses a different encoding, inside your
        application data is held in abstract text form.  You can program your
        business logic without worrying about which data came from which source.
        You can freely exchange the data you store between sources.  Only
        reading/writing files requires encoding your text to bytes.
+
+For Enterprise
+==============
+
+Available as part of the Tidelift Subscription.
+
+This project and the maintainers of thousands of other packages are working with Tidelift to deliver one enterprise subscription that covers all of the open source you use.
+
+`Learn more <https://tidelift.com/subscription/pkg/pypi-configparser?utm_source=pypi-configparser&utm_medium=referral&utm_campaign=github>`_.
```

### Comparing `configparser-5.3.0/src/test_backport.py` & `configparser-6.0.0/tests/test_backport.py`

 * *Files 0% similar despite different names*

```diff
@@ -50,15 +50,15 @@
     def test_unicode_extended_characters(self):
         cp = configparser.ConfigParser()
         cp.add_section('section')
         cp.add_section('łąka1')
         cp['łąka2'] = {}
         cp.set('section', 'łąka1', 'value')
         cp['section']['łąka2'] = 'value'
-        self.assertEqual(set(cp['section']), set(['łąka1', 'łąka2']))
+        self.assertEqual(set(cp['section']), {'łąka1', 'łąka2'})
         cp['new'] = {'łąka': 'value'}
         cp.set('section', 'key', 'łąka')
         cp['section']['key'] = 'łąka'
         self.assertEqual(cp['section']['key'], 'łąka')
         cp['new'] = {'key': 'łąka'}
 
     def assertIsAlright(self, cp, optvalue):
```

### Comparing `configparser-5.3.0/src/test_configparser.py` & `configparser-6.0.0/tests/test_configparser.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import pathlib
 import textwrap
 import unittest
 import warnings
 
 from typing import Type, Iterable
 
-from compat import support, os_helper
+from .compat import support, os_helper
 
 from backports import configparser
 
 
 def nice_literals(str):
     "Remove b and u prefixes from reprs"
     return str.replace("b'", "'").replace("u'", "'")
@@ -38,19 +38,19 @@
         return iter(self.values())
 
     __iter__ = iterkeys
 
 
 class CfgParserTestCaseClass:
     allow_no_value = False
-    delimiters = ('=', ':')  # type: Iterable[str]
-    comment_prefixes = (';', '#')  # type: Iterable[str]
-    inline_comment_prefixes = (';', '#')  # type: Iterable[str]
+    delimiters: Iterable[str] = ('=', ':')
+    comment_prefixes: Iterable[str] = (';', '#')
+    inline_comment_prefixes: Iterable[str] = (';', '#')
     empty_lines_in_values = True
-    dict_type = configparser._default_dict  # type: Type[collections.abc.Mapping]
+    dict_type: Type[collections.abc.Mapping] = configparser._default_dict
     strict = False
     default_section = configparser.DEFAULTSECT
     interpolation = configparser._UNSET
 
     def newconfig(self, defaults=None):
         arguments = dict(
             defaults=defaults,
@@ -116,15 +116,15 @@
         self.assertEqual(len(L), len(E))
         for name, section in L:
             eq(name, section.name)
         eq(cf.defaults(), cf[self.default_section])
 
         # The use of spaces in the section names serves as a
         # regression test for SourceForge bug #583248:
-        # http://www.python.org/sf/583248
+        # https://bugs.python.org/issue583248
 
         # API access
         eq(cf.get('Foo Bar', 'foo'), 'bar1')
         eq(cf.get('Spacey Bar', 'foo'), 'bar2')
         eq(cf.get('Spacey Bar From The Beginning', 'foo'), 'bar3')
         eq(cf.get('Spacey Bar From The Beginning', 'baz'), 'qwe')
         eq(cf.get('Commented Bar', 'foo'), 'bar4')
@@ -1017,15 +1017,15 @@
                 ('getdefault', '|<default>|'),
                 ('key', '|value|'),
                 ('name', 'value'),
             ]
         )
 
     def test_safe_interpolation(self):
-        # See http://www.python.org/sf/511737
+        # See https://bugs.python.org/issue511737
         cf = self.fromstring(
             "[section]\n"
             "option1{eq}xxx\n"
             "option2{eq}%(option1)s/xxx\n"
             "ok{eq}%(option1)s/%%s\n"
             "not_ok{eq}%(option2)s/%%s".format(eq=self.delimiters[0])
         )
@@ -1767,32 +1767,20 @@
     def test_interpolation_depth_error(self):
         error = configparser.InterpolationDepthError('option', 'section', 'rawval')
         self.assertEqual(error.args, ('option', 'section', 'rawval'))
         self.assertEqual(error.option, 'option')
         self.assertEqual(error.section, 'section')
 
     def test_parsing_error(self):
-        with self.assertRaises(ValueError) as cm:
+        with self.assertRaises(TypeError):
             configparser.ParsingError()
-        self.assertEqual(str(cm.exception), "Required argument `source' not " "given.")
-        with self.assertRaises(ValueError) as cm:
-            configparser.ParsingError(source='source', filename='filename')
-        self.assertEqual(
-            str(cm.exception),
-            "Cannot specify both `filename' " "and `source'. Use `source'.",
-        )
-        error = configparser.ParsingError(filename='source')
+        error = configparser.ParsingError(source='source')
+        self.assertEqual(error.source, 'source')
+        error = configparser.ParsingError('source')
         self.assertEqual(error.source, 'source')
-        with warnings.catch_warnings(record=True) as w:
-            warnings.simplefilter("always", DeprecationWarning)
-            self.assertEqual(error.filename, 'source')
-            error.filename = 'filename'
-            self.assertEqual(error.source, 'filename')
-        for warning in w:
-            self.assertTrue(warning.category is DeprecationWarning)
 
     def test_interpolation_validation(self):
         parser = configparser.ConfigParser()
         parser.read_string(
             """
             [section]
             invalid_percent = %
@@ -1809,37 +1797,14 @@
         with self.assertRaises(configparser.InterpolationSyntaxError) as cm:
             parser['section']['invalid_reference']
         self.assertEqual(
             str(cm.exception),
             "bad interpolation variable " "reference {0!r}".format('%(()'),
         )
 
-    def test_readfp_deprecation(self):
-        sio = io.StringIO(
-            """
-        [section]
-        option = value
-        """
-        )
-        parser = configparser.ConfigParser()
-        with warnings.catch_warnings(record=True) as w:
-            warnings.simplefilter("always", DeprecationWarning)
-            parser.readfp(sio, filename='StringIO')
-        for warning in w:
-            self.assertTrue(warning.category is DeprecationWarning)
-        self.assertEqual(len(parser), 2)
-        self.assertEqual(parser['section']['option'], 'value')
-
-    def test_safeconfigparser_deprecation(self):
-        with warnings.catch_warnings(record=True) as w:
-            warnings.simplefilter("always", DeprecationWarning)
-            configparser.SafeConfigParser()
-        for warning in w:
-            self.assertTrue(warning.category is DeprecationWarning)
-
     def test_legacyinterpolation_deprecation(self):
         with warnings.catch_warnings(record=True) as w:
             warnings.simplefilter("always", DeprecationWarning)
             configparser.LegacyInterpolation()
         self.assertGreaterEqual(len(w), 1)
         for warning in w:
             self.assertIs(warning.category, DeprecationWarning)
@@ -2019,15 +1984,15 @@
             pickled = pickle.dumps(e1, proto)
             e2 = pickle.loads(pickled)
             self.assertEqual(e1.message, e2.message)
             self.assertEqual(e1.args, e2.args)
             self.assertEqual(e1.source, e2.source)
             self.assertEqual(e1.errors, e2.errors)
             self.assertEqual(repr(e1), repr(e2))
-        e1 = configparser.ParsingError(filename='filename')
+        e1 = configparser.ParsingError('filename')
         e1.append(1, 'line1')
         e1.append(2, 'line2')
         e1.append(3, 'line3')
         for proto in range(pickle.HIGHEST_PROTOCOL + 1):
             pickled = pickle.dumps(e1, proto)
             e2 = pickle.loads(pickled)
             self.assertEqual(e1.message, e2.message)
```

### Comparing `configparser-5.3.0/tox.ini` & `configparser-6.0.0/tox.ini`

 * *Files 13% similar despite different names*

```diff
@@ -1,29 +1,41 @@
 [tox]
-envlist = python
-minversion = 3.2
-# https://github.com/jaraco/skeleton/issues/6
-tox_pip_extensions_ext_venv_update = true
 toxworkdir={env:TOX_WORK_DIR:.tox}
 
 
 [testenv]
 deps =
+	# workaround for #67
+	virtualenv; platform_system == "Windows" and python_version < "3.9"
+setenv =
+	PYTHONWARNDEFAULTENCODING = 1
 commands =
 	pytest {posargs}
 usedevelop = True
-extras = testing
+extras =
+	testing
 
 [testenv:docs]
 extras =
 	docs
 	testing
 changedir = docs
 commands =
 	python -m sphinx -W --keep-going . {toxinidir}/build/html
+	python -m sphinxlint
+
+[testenv:finalize]
+skip_install = True
+deps =
+	towncrier
+	jaraco.develop >= 7.23
+passenv = *
+commands =
+	python -m jaraco.develop.finalize
+
 
 [testenv:release]
 skip_install = True
 deps =
 	build
 	twine>=3
 	jaraco.develop>=7.1
```

