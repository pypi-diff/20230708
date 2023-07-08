# Comparing `tmp/ocdsextensionregistry-0.3.2.tar.gz` & `tmp/ocdsextensionregistry-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ocdsextensionregistry-0.3.2.tar", last modified: Fri Jul  7 21:32:02 2023, max compression
+gzip compressed data, was "ocdsextensionregistry-0.3.3.tar", last modified: Sat Jul  8 03:36:45 2023, max compression
```

## Comparing `ocdsextensionregistry-0.3.2.tar` & `ocdsextensionregistry-0.3.3.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 21:32:02.539585 ocdsextensionregistry-0.3.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-07-07 21:31:53.000000 ocdsextensionregistry-0.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-07-07 21:31:53.000000 ocdsextensionregistry-0.3.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-07-07 21:32:02.539585 ocdsextensionregistry-0.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-07-07 21:31:53.000000 ocdsextensionregistry-0.3.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 21:32:02.535585 ocdsextensionregistry-0.3.2/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-07-07 21:31:53.000000 ocdsextensionregistry-0.3.2/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 21:32:02.535585 ocdsextensionregistry-0.3.2/docs/api/
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-07 21:31:53.000000 ocdsextensionregistry-0.3.2/docs/api/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-07-07 21:31:53.000000 ocdsextensionregistry-0.3.2/docs/api/codelist.rst
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-07-07 21:31:53.000000 ocdsextensionregistry-0.3.2/docs/api/codelist_code.rst
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-07-07 21:31:53.000000 ocdsextensionregistry-0.3.2/docs/api/exceptions.rst
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-07 21:31:53.000000 ocdsextensionregistry-0.3.2/docs/api/extension.rst
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-07-07 21:31:53.000000 ocdsextensionregistry-0.3.2/docs/api/extension_registry.rst
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-07-07 21:31:53.000000 ocdsextensionregistry-0.3.2/docs/api/extension_version.rst
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-07-07 21:31:53.000000 ocdsextensionregistry-0.3.2/docs/api/profile_builder.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-07 21:31:53.000000 ocdsextensionregistry-0.3.2/docs/api/util.rst
--rw-r--r--   0 runner    (1001) docker     (123)    16981 2023-07-07 21:31:53.000000 ocdsextensionregistry-0.3.2/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7430 2023-07-07 21:31:53.000000 ocdsextensionregistry-0.3.2/docs/cli.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-07-07 21:31:53.000000 ocdsextensionregistry-0.3.2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-07-07 21:31:53.000000 ocdsextensionregistry-0.3.2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-07-07 21:31:53.000000 ocdsextensionregistry-0.3.2/docs/library.rst
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-07 21:31:53.000000 ocdsextensionregistry-0.3.2/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2601 2023-07-07 21:31:53.000000 ocdsextensionregistry-0.3.2/docs/translation.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 21:32:02.535585 ocdsextensionregistry-0.3.2/ocdsextensionregistry/
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-07-07 21:31:53.000000 ocdsextensionregistry-0.3.2/ocdsextensionregistry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-07-07 21:31:53.000000 ocdsextensionregistry-0.3.2/ocdsextensionregistry/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5800 2023-07-07 21:31:53.000000 ocdsextensionregistry-0.3.2/ocdsextensionregistry/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     3737 2023-07-07 21:31:53.000000 ocdsextensionregistry-0.3.2/ocdsextensionregistry/codelist.py
--rw-r--r--   0 runner    (1001) docker     (123)      992 2023-07-07 21:31:53.000000 ocdsextensionregistry-0.3.2/ocdsextensionregistry/codelist_code.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 21:32:02.539585 ocdsextensionregistry-0.3.2/ocdsextensionregistry/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 21:31:53.000000 ocdsextensionregistry-0.3.2/ocdsextensionregistry/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1662 2023-07-07 21:31:53.000000 ocdsextensionregistry-0.3.2/ocdsextensionregistry/commands/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2804 2023-07-07 21:31:53.000000 ocdsextensionregistry-0.3.2/ocdsextensionregistry/commands/download.py
--rw-r--r--   0 runner    (1001) docker     (123)     7784 2023-07-07 21:31:53.000000 ocdsextensionregistry-0.3.2/ocdsextensionregistry/commands/generate_data_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     9256 2023-07-07 21:31:53.000000 ocdsextensionregistry-0.3.2/ocdsextensionregistry/commands/generate_pot_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-07-07 21:31:53.000000 ocdsextensionregistry-0.3.2/ocdsextensionregistry/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-07-07 21:31:53.000000 ocdsextensionregistry-0.3.2/ocdsextensionregistry/extension.py
--rw-r--r--   0 runner    (1001) docker     (123)     5472 2023-07-07 21:31:53.000000 ocdsextensionregistry-0.3.2/ocdsextensionregistry/extension_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)    15016 2023-07-07 21:31:53.000000 ocdsextensionregistry-0.3.2/ocdsextensionregistry/extension_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    16386 2023-07-07 21:31:53.000000 ocdsextensionregistry-0.3.2/ocdsextensionregistry/profile_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3146 2023-07-07 21:31:53.000000 ocdsextensionregistry-0.3.2/ocdsextensionregistry/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 21:32:02.539585 ocdsextensionregistry-0.3.2/ocdsextensionregistry.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-07-07 21:32:02.000000 ocdsextensionregistry-0.3.2/ocdsextensionregistry.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-07-07 21:32:02.000000 ocdsextensionregistry-0.3.2/ocdsextensionregistry.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 21:32:02.000000 ocdsextensionregistry-0.3.2/ocdsextensionregistry.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-07 21:32:02.000000 ocdsextensionregistry-0.3.2/ocdsextensionregistry.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-07 21:32:02.000000 ocdsextensionregistry-0.3.2/ocdsextensionregistry.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-07 21:32:02.000000 ocdsextensionregistry-0.3.2/ocdsextensionregistry.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-07 21:31:53.000000 ocdsextensionregistry-0.3.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-07-07 21:32:02.539585 ocdsextensionregistry-0.3.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 21:32:02.539585 ocdsextensionregistry-0.3.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-07-07 21:31:53.000000 ocdsextensionregistry-0.3.2/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 21:32:02.539585 ocdsextensionregistry-0.3.2/tests/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 21:31:53.000000 ocdsextensionregistry-0.3.2/tests/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4853 2023-07-07 21:31:53.000000 ocdsextensionregistry-0.3.2/tests/commands/test_download.py
--rw-r--r--   0 runner    (1001) docker     (123)     7243 2023-07-07 21:31:53.000000 ocdsextensionregistry-0.3.2/tests/commands/test_generate_data_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     2883 2023-07-07 21:31:53.000000 ocdsextensionregistry-0.3.2/tests/commands/test_generate_pot_files.py
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-07-07 21:31:53.000000 ocdsextensionregistry-0.3.2/tests/commands/test_none.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 21:32:02.539585 ocdsextensionregistry-0.3.2/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)    17612 2023-07-07 21:31:53.000000 ocdsextensionregistry-0.3.2/tests/fixtures/location-v1.1.4.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 21:32:02.539585 ocdsextensionregistry-0.3.2/tests/fixtures/ocds_coveredBy_extension/
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-07-07 21:31:53.000000 ocdsextensionregistry-0.3.2/tests/fixtures/ocds_coveredBy_extension/release-schema.json
--rw-r--r--   0 runner    (1001) docker     (123)     2824 2023-07-07 21:31:53.000000 ocdsextensionregistry-0.3.2/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5874 2023-07-07 21:31:53.000000 ocdsextensionregistry-0.3.2/tests/test_codelist.py
--rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-07-07 21:31:53.000000 ocdsextensionregistry-0.3.2/tests/test_codelist_code.py
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-07-07 21:31:53.000000 ocdsextensionregistry-0.3.2/tests/test_extension.py
--rw-r--r--   0 runner    (1001) docker     (123)    10484 2023-07-07 21:31:53.000000 ocdsextensionregistry-0.3.2/tests/test_extension_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)    13099 2023-07-07 21:31:53.000000 ocdsextensionregistry-0.3.2/tests/test_extension_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    15543 2023-07-07 21:31:53.000000 ocdsextensionregistry-0.3.2/tests/test_profile_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-07-07 21:31:53.000000 ocdsextensionregistry-0.3.2/tests/test_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-07-07 21:31:53.000000 ocdsextensionregistry-0.3.2/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 03:36:45.454204 ocdsextensionregistry-0.3.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-07-08 03:36:36.000000 ocdsextensionregistry-0.3.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-07-08 03:36:36.000000 ocdsextensionregistry-0.3.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-07-08 03:36:45.454204 ocdsextensionregistry-0.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-07-08 03:36:36.000000 ocdsextensionregistry-0.3.3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 03:36:45.450204 ocdsextensionregistry-0.3.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-07-08 03:36:36.000000 ocdsextensionregistry-0.3.3/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 03:36:45.450204 ocdsextensionregistry-0.3.3/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-08 03:36:36.000000 ocdsextensionregistry-0.3.3/docs/api/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-07-08 03:36:36.000000 ocdsextensionregistry-0.3.3/docs/api/codelist.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-07-08 03:36:36.000000 ocdsextensionregistry-0.3.3/docs/api/codelist_code.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-07-08 03:36:36.000000 ocdsextensionregistry-0.3.3/docs/api/exceptions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-08 03:36:36.000000 ocdsextensionregistry-0.3.3/docs/api/extension.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-07-08 03:36:36.000000 ocdsextensionregistry-0.3.3/docs/api/extension_registry.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-07-08 03:36:36.000000 ocdsextensionregistry-0.3.3/docs/api/extension_version.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-07-08 03:36:36.000000 ocdsextensionregistry-0.3.3/docs/api/profile_builder.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-08 03:36:36.000000 ocdsextensionregistry-0.3.3/docs/api/util.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    18292 2023-07-08 03:36:36.000000 ocdsextensionregistry-0.3.3/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7430 2023-07-08 03:36:36.000000 ocdsextensionregistry-0.3.3/docs/cli.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-07-08 03:36:36.000000 ocdsextensionregistry-0.3.3/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-07-08 03:36:36.000000 ocdsextensionregistry-0.3.3/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-07-08 03:36:36.000000 ocdsextensionregistry-0.3.3/docs/library.rst
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-08 03:36:36.000000 ocdsextensionregistry-0.3.3/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2601 2023-07-08 03:36:36.000000 ocdsextensionregistry-0.3.3/docs/translation.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 03:36:45.450204 ocdsextensionregistry-0.3.3/ocdsextensionregistry/
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-07-08 03:36:36.000000 ocdsextensionregistry-0.3.3/ocdsextensionregistry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-07-08 03:36:36.000000 ocdsextensionregistry-0.3.3/ocdsextensionregistry/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5800 2023-07-08 03:36:36.000000 ocdsextensionregistry-0.3.3/ocdsextensionregistry/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3737 2023-07-08 03:36:36.000000 ocdsextensionregistry-0.3.3/ocdsextensionregistry/codelist.py
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2023-07-08 03:36:36.000000 ocdsextensionregistry-0.3.3/ocdsextensionregistry/codelist_code.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 03:36:45.450204 ocdsextensionregistry-0.3.3/ocdsextensionregistry/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 03:36:36.000000 ocdsextensionregistry-0.3.3/ocdsextensionregistry/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1662 2023-07-08 03:36:36.000000 ocdsextensionregistry-0.3.3/ocdsextensionregistry/commands/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2804 2023-07-08 03:36:36.000000 ocdsextensionregistry-0.3.3/ocdsextensionregistry/commands/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7784 2023-07-08 03:36:36.000000 ocdsextensionregistry-0.3.3/ocdsextensionregistry/commands/generate_data_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9256 2023-07-08 03:36:36.000000 ocdsextensionregistry-0.3.3/ocdsextensionregistry/commands/generate_pot_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-07-08 03:36:36.000000 ocdsextensionregistry-0.3.3/ocdsextensionregistry/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-07-08 03:36:36.000000 ocdsextensionregistry-0.3.3/ocdsextensionregistry/extension.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5472 2023-07-08 03:36:36.000000 ocdsextensionregistry-0.3.3/ocdsextensionregistry/extension_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15708 2023-07-08 03:36:36.000000 ocdsextensionregistry-0.3.3/ocdsextensionregistry/extension_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16382 2023-07-08 03:36:36.000000 ocdsextensionregistry-0.3.3/ocdsextensionregistry/profile_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3146 2023-07-08 03:36:36.000000 ocdsextensionregistry-0.3.3/ocdsextensionregistry/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 03:36:45.450204 ocdsextensionregistry-0.3.3/ocdsextensionregistry.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-07-08 03:36:45.000000 ocdsextensionregistry-0.3.3/ocdsextensionregistry.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-07-08 03:36:45.000000 ocdsextensionregistry-0.3.3/ocdsextensionregistry.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 03:36:45.000000 ocdsextensionregistry-0.3.3/ocdsextensionregistry.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-08 03:36:45.000000 ocdsextensionregistry-0.3.3/ocdsextensionregistry.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-08 03:36:45.000000 ocdsextensionregistry-0.3.3/ocdsextensionregistry.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-08 03:36:45.000000 ocdsextensionregistry-0.3.3/ocdsextensionregistry.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-08 03:36:36.000000 ocdsextensionregistry-0.3.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-07-08 03:36:45.454204 ocdsextensionregistry-0.3.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 03:36:45.454204 ocdsextensionregistry-0.3.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-07-08 03:36:36.000000 ocdsextensionregistry-0.3.3/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 03:36:45.454204 ocdsextensionregistry-0.3.3/tests/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 03:36:36.000000 ocdsextensionregistry-0.3.3/tests/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4853 2023-07-08 03:36:36.000000 ocdsextensionregistry-0.3.3/tests/commands/test_download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7243 2023-07-08 03:36:36.000000 ocdsextensionregistry-0.3.3/tests/commands/test_generate_data_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2883 2023-07-08 03:36:36.000000 ocdsextensionregistry-0.3.3/tests/commands/test_generate_pot_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-07-08 03:36:36.000000 ocdsextensionregistry-0.3.3/tests/commands/test_none.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 03:36:45.454204 ocdsextensionregistry-0.3.3/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)    17612 2023-07-08 03:36:36.000000 ocdsextensionregistry-0.3.3/tests/fixtures/location-v1.1.4.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 03:36:45.454204 ocdsextensionregistry-0.3.3/tests/fixtures/ocds_coveredBy_extension/
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-07-08 03:36:36.000000 ocdsextensionregistry-0.3.3/tests/fixtures/ocds_coveredBy_extension/release-schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2824 2023-07-08 03:36:36.000000 ocdsextensionregistry-0.3.3/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5874 2023-07-08 03:36:36.000000 ocdsextensionregistry-0.3.3/tests/test_codelist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-07-08 03:36:36.000000 ocdsextensionregistry-0.3.3/tests/test_codelist_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-07-08 03:36:36.000000 ocdsextensionregistry-0.3.3/tests/test_extension.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10484 2023-07-08 03:36:36.000000 ocdsextensionregistry-0.3.3/tests/test_extension_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13103 2023-07-08 03:36:36.000000 ocdsextensionregistry-0.3.3/tests/test_extension_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15543 2023-07-08 03:36:36.000000 ocdsextensionregistry-0.3.3/tests/test_profile_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-07-08 03:36:36.000000 ocdsextensionregistry-0.3.3/tests/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-07-08 03:36:36.000000 ocdsextensionregistry-0.3.3/tox.ini
```

### Comparing `ocdsextensionregistry-0.3.2/LICENSE` & `ocdsextensionregistry-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.3.2/PKG-INFO` & `ocdsextensionregistry-0.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ocdsextensionregistry
-Version: 0.3.2
+Version: 0.3.3
 Summary: Eases access to information from the extension registry of the Open Contracting Data Standard
 Home-page: https://github.com/open-contracting/extension_registry.py
 Author: Open Contracting Partnership
 Author-email: data@open-contracting.org
 License: BSD
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
```

### Comparing `ocdsextensionregistry-0.3.2/README.rst` & `ocdsextensionregistry-0.3.3/README.rst`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.3.2/docs/Makefile` & `ocdsextensionregistry-0.3.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.3.2/docs/changelog.rst` & `ocdsextensionregistry-0.3.3/docs/changelog.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,42 +1,66 @@
 Changelog
 =========
 
+0.3.3 (2023-07-07)
+------------------
+
+-  feat: Make ExtensionVersion more robust to bad data, when using a package's ``extensions`` field as input.
+
+   -  Warn if the request errors for an extension's codelist file (unreachable host, request timeout, HTTP error, too many redirects, etc.), if the bulk file is not a ZIP file, or if the codelist is not UTF-8.
+
+      The previous behavior of raising an exception can be restored with:
+
+      .. code-block:: python
+
+         import warnings
+
+         from ocdsextensionregistry.exceptions import ExtensionCodelistWarning
+
+
+         with warnings.catch_warnings():
+             warnings.filterwarnings('error', category=ExtensionCodelistWarning)
+             # Use of ExtensionVersion.codelist that warns.
+
+-  feat: Warn if the extension's release schema patch or codelist file is not UTF-8.
+-  feat: Add :attr:`ocdsextensionregistry.extension_version.ExtensionVersion.input_url` for the URL that was provided in a list to :meth:`ocdsextensionregistry.profile_builder.ProfileBuilder.extensions`.
+-  fix: :attr:`ocdsextensionregistry.extension_version.ExtensionVersion.repository_ref` only matches if the extension's files are in the repository's root – which is required by :attr:`~ocdsextensionregistry.extension_version.ExtensionVersion.repository_ref_download_url`.
+
 0.3.2 (2023-07-07)
 ------------------
 
 -  feat: Add :attr:`ocdsextensionregistry.extension_version.ExtensionVersion.repository_ref` and :attr:`~ocdsextensionregistry.extension_version.ExtensionVersion.repository_ref_download_url`.
--  feat: Set :meth:`ocdsextensionregistry.extension_version.ExtensionVersion.download_url` to :attr:`~ocdsextensionregistry.extension_version.ExtensionVersion.repository_ref_download_url` on initialization, if possible.
+-  feat: Set :attr:`ocdsextensionregistry.extension_version.ExtensionVersion.download_url` to :attr:`~ocdsextensionregistry.extension_version.ExtensionVersion.repository_ref_download_url` on initialization, if possible.
 
 0.3.1 (2023-07-07)
 ------------------
 
 -  fix: :meth:`~ocdsextensionregistry.profile_builder.ProfileBuilder.extensions`: Support retrieval of the metadata file, if the ``extension_versions`` argument is a list of extensions' metadata files served via API.
 
 0.3.0 (2023-07-06)
 ------------------
 
 -  feat: Make ProfileBuilder more robust to bad data, when using a package's ``extensions`` field as input.
 
    -  Skip a package's ``extensions`` field if it is not an array.
    -  Skip an entry in the package's ``extensions`` array if it is blank or is not a string.
-   -  Warn if an extension's ``release-schema.json`` file is not available in bulk, if the request errors (unreachable host, request timeout, HTTP error, too many redirects, etc.), if the bulk file is not a ZIP file, or if the release schema is not a JSON file.
+   -  Warn if the request errors for the extension's release schema patch (unreachable host, request timeout, HTTP error, too many redirects, etc.), if the bulk file is not a ZIP file, or if the release schema is not a JSON file.
 
       The previous behavior of raising an exception can be restored with:
 
       .. code-block:: python
 
          import warnings
 
          from ocdsextensionregistry.exceptions import ExtensionWarning
 
 
          with warnings.catch_warnings():
              warnings.filterwarnings('error', category=ExtensionWarning)
-             # Use of ProfileBuilder that warns.
+             # Use of ProfileBuilder.release_schema_path() that warns.
 
 -  feat: Configure the expiration behavior of the responses cache using a ``REQUESTS_CACHE_EXPIRE_AFTER`` environment variable. See `requests-cache's documentation <https://requests-cache.readthedocs.io/en/stable/user_guide/expiration.html>`__ (``NEVER_EXPIRE`` is ``-1`` and ``EXPIRE_IMMEDIATELY`` is ``0``, in the `source <https://github.com/requests-cache/requests-cache/blob/main/requests_cache/policy/expiration.py>`__).
 -  fix: :meth:`ocdsextensionregistry.extension_version.ExtensionVersion.__repr__`: No longer errors if initialized with ``file_urls`` only.
 -  fix: :meth:`ocdsextensionregistry.extension_version.ExtensionVersion.get_url`: Raises clearer error if initialized with a Download URL only.
 -  Add support for Sphinx 6.2 on Python 3.11.
 
 0.2.2 (2023-06-05)
```

### Comparing `ocdsextensionregistry-0.3.2/docs/cli.rst` & `ocdsextensionregistry-0.3.3/docs/cli.rst`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.3.2/docs/conf.py` & `ocdsextensionregistry-0.3.3/docs/conf.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 # -- Project information -----------------------------------------------------
 
 project = "OCDS Extension Registry Python Package"
 copyright = "2018, Open Contracting Partnership"
 author = "Open Contracting Partnership"
 
 # The short X.Y version
-version = "0.3.2"
+version = "0.3.3"
 # The full version, including alpha/beta/rc tags
 release = version
 
 
 # -- General configuration ---------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
```

### Comparing `ocdsextensionregistry-0.3.2/docs/index.rst` & `ocdsextensionregistry-0.3.3/docs/index.rst`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.3.2/docs/translation.rst` & `ocdsextensionregistry-0.3.3/docs/translation.rst`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.3.2/ocdsextensionregistry/__init__.py` & `ocdsextensionregistry-0.3.3/ocdsextensionregistry/__init__.py`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.3.2/ocdsextensionregistry/__main__.py` & `ocdsextensionregistry-0.3.3/ocdsextensionregistry/__main__.py`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.3.2/ocdsextensionregistry/api.py` & `ocdsextensionregistry-0.3.3/ocdsextensionregistry/api.py`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.3.2/ocdsextensionregistry/codelist.py` & `ocdsextensionregistry-0.3.3/ocdsextensionregistry/codelist.py`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.3.2/ocdsextensionregistry/codelist_code.py` & `ocdsextensionregistry-0.3.3/ocdsextensionregistry/codelist_code.py`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.3.2/ocdsextensionregistry/commands/base.py` & `ocdsextensionregistry-0.3.3/ocdsextensionregistry/commands/base.py`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.3.2/ocdsextensionregistry/commands/download.py` & `ocdsextensionregistry-0.3.3/ocdsextensionregistry/commands/download.py`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.3.2/ocdsextensionregistry/commands/generate_data_file.py` & `ocdsextensionregistry-0.3.3/ocdsextensionregistry/commands/generate_data_file.py`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.3.2/ocdsextensionregistry/commands/generate_pot_files.py` & `ocdsextensionregistry-0.3.3/ocdsextensionregistry/commands/generate_pot_files.py`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.3.2/ocdsextensionregistry/exceptions.py` & `ocdsextensionregistry-0.3.3/ocdsextensionregistry/exceptions.py`

 * *Files 24% similar despite different names*

```diff
@@ -23,15 +23,29 @@
 
 
 class OCDSExtensionRegistryWarning(UserWarning):
     """Base class for warnings from within this package"""
 
 
 class ExtensionWarning(OCDSExtensionRegistryWarning):
-    """Used when an extension can't be retrieved or merged."""
+    """Used when an extension file can't be read."""
 
     def __init__(self, extension, exc):
         self.extension = extension
         self.exc = exc
 
     def __str__(self):
-        return f"{self.extension}: {self.exc.__class__.__module__}.{self.exc.__class__.__name__}: {self.exc}"
+        klass = self.exc.__class__
+        return f"{self.extension}: {klass.__module__}.{klass.__name__}: {self.exc}"
+
+
+class ExtensionCodelistWarning(OCDSExtensionRegistryWarning):
+    """Used when a codelist file can't be read."""
+
+    def __init__(self, extension, codelist, exc):
+        self.extension = extension
+        self.codelist = codelist
+        self.exc = exc
+
+    def __str__(self):
+        klass = self.exc.__class__
+        return f"{self.extension}({self.codelist}): {klass.__module__}.{klass.__name__}: {self.exc}"
```

### Comparing `ocdsextensionregistry-0.3.2/ocdsextensionregistry/extension.py` & `ocdsextensionregistry-0.3.3/ocdsextensionregistry/extension.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 class Extension:
     def __init__(self, data):
         """
         Accepts a row from extensions.csv and assigns values to properties.
         """
+        #: The Id cell.
         self.id = data['Id']
+        #: The Category cell.
         self.category = data['Category']
+        #: The Core cell.
         self.core = data['Core'] == 'true'
 
     def __repr__(self):
         return self.id
 
     def as_dict(self):
         """
```

### Comparing `ocdsextensionregistry-0.3.2/ocdsextensionregistry/extension_registry.py` & `ocdsextensionregistry-0.3.3/ocdsextensionregistry/extension_registry.py`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.3.2/ocdsextensionregistry/extension_version.py` & `ocdsextensionregistry-0.3.3/ocdsextensionregistry/extension_version.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,48 +1,59 @@
 import csv
 import json
 import os
 import re
+import warnings
+import zipfile
 from contextlib import closing
 from io import StringIO
 from urllib.parse import urlsplit
 
 import requests
 
 from .codelist import Codelist
-from .exceptions import DoesNotExist, NotAvailableInBulk
+from .exceptions import DoesNotExist, ExtensionCodelistWarning, NotAvailableInBulk
 from .util import _resolve_zip, session
 
 SCHEMAS = ('record-package-schema.json', 'release-package-schema.json', 'release-schema.json')
 FIELD_NAME = '4F434453'  # OCDS in hexidecimal
 FIELD = f'{{{FIELD_NAME}}}'
 
 
 class ExtensionVersion:
-    def __init__(self, data, file_urls=None, url_pattern=None):
+    def __init__(self, data, input_url=None, url_pattern=None, file_urls=None):
         """
         Accepts a row from extension_versions.csv and assigns values to properties.
         """
+        #: The Id cell.
         self.id = data['Id']
+        #: The Date cell.
         self.date = data['Date']
+        #: The Version cell.
         self.version = data['Version']
+        #: The Base URL cell.
         self.base_url = data['Base URL']
+        #: The Download URL cell.
         self.download_url = data['Download URL']
+        #: The URL that was provided in a list to
+        # :meth:`ocdsextensionregistry.profile_builder.ProfileBuilder.extensions`.
+        self.input_url = input_url
 
         self._url_pattern = url_pattern
         self._file_urls = file_urls or {}
         self._files = None
         self._metadata = None
         self._schemas = None
         self._codelists = None
 
         # This runs only when using this class outside the context of the extension registry.
         if not self.download_url:
             try:
                 self.download_url = self.repository_ref_download_url
+            # The URL is malformed or unsupported.
             except (AttributeError, NotImplementedError):
                 pass
 
     def __repr__(self):
         if self.id and self.version:
             return f'{self.id}=={self.version}'
         elif self.base_url:
@@ -60,15 +71,15 @@
         for k, v in other.as_dict().items():
             setattr(self, k, v)
 
     def as_dict(self):
         """
         Returns the object's public properties as a dictionary.
         """
-        return {key: value for key, value in self.__dict__.items() if not key.startswith('_')}
+        return {key: value for key, value in self.__dict__.items() if not key.startswith(('_', 'input_url'))}
 
     def get_url(self, basename):
         """
         Returns the URL of the file within the extension.
 
         :raises NotImplementedError: if the basename is not in the file URLs and the base URL is not set
         """
@@ -92,15 +103,15 @@
         :raises zipfile.BadZipFile: if the download URL is not a ZIP file
         """
         if basename not in self.files:
             if not self.download_url:
                 response = session.get(self.get_url(basename))
                 if default is None or response.status_code != requests.codes.not_found:
                     response.raise_for_status()
-                    self._files[basename] = response.text
+                    self._files[basename] = response.content.decode('utf-8')
 
         if default is not None:
             return self.files.get(basename, default)
         elif basename not in self.files:
             raise DoesNotExist(f'File {basename!r} does not exist in {self}')
         return self.files[basename]
 
@@ -182,15 +193,15 @@
             else:
                 names = SCHEMAS
 
             for name in names:
                 try:
                     self._schemas[name] = json.loads(self.remote(name))
                 except requests.exceptions.HTTPError:
-                    if 'schemas' in self.metadata:
+                    if 'schemas' in self.metadata:  # avoid raising if using SCHEMAS
                         raise
 
         return self._schemas
 
     @property
     def codelists(self):
         """
@@ -210,17 +221,21 @@
 
             for name in names:
                 try:
                     self._codelists[name] = Codelist(name)
                     # Use universal newlines mode, to avoid parsing errors.
                     io = StringIO(self.remote('codelists/' + name), newline='')
                     self._codelists[name].extend(csv.DictReader(io))
-                except requests.exceptions.HTTPError:
-                    if 'codelists' in self.metadata:
-                        raise
+                except (
+                    UnicodeDecodeError,
+                    requests.RequestException,
+                    zipfile.BadZipFile,
+                ) as e:
+                    warnings.warn(ExtensionCodelistWarning(self, name, e))
+                    continue
 
         return self._codelists
 
     @property
     def repository_full_name(self):
         """
         Returns the full name of the extension's repository, which should be a unique identifier on the hosting
@@ -242,15 +257,15 @@
         Returns the user or organization to which the extension's repository belongs, e.g. open-contracting-extensions
         """
         return self._repository_property('user')
 
     @property
     def repository_ref(self):
         """
-        Returns the ref in the extension's URL, e.g. the commit, tag or branch, like v1.1.5
+        Returns the ref in the extension's URL if the extension's files are in the repository's root, like v1.1.5
         """
         return self._repository_property('ref')
 
     @property
     def repository_user_page(self):
         """
         Returns the URL to the landing page of the user or organization to which the extension's repository belongs,
@@ -340,37 +355,37 @@
         netloc = parsed.netloc
         if netloc == 'raw.githubusercontent.com':
             # Sample base URL: https://raw.githubusercontent.com/open-contracting-extensions/ocds_bid_extension/v1.1.4/
             return {
                 'full_name:pattern': r'\A/([^/]+/[^/]+)',
                 'name:pattern': r'\A/[^/]+/([^/]+)',
                 'user:pattern': r'\A/([^/]+)',
-                'ref:pattern': r'\A/[^/]+/[^/]+/([^/]+)',
+                'ref:pattern': r'\A/[^/]+/[^/]+/([^/]+)/[^/]*\Z',
                 'html_page:prefix': 'https://github.com/',
                 'url:prefix': 'git@github.com:',
                 'url:suffix': '.git',
                 'download:format': 'https://github.com/{full_name}/archive/{ref}.zip',
             }
         if netloc == 'bitbucket.org':
             # A base URL may look like: https://bitbucket.org/facebook/hgsql/raw/default/
             return {
                 'full_name:pattern': r'\A/([^/]+/[^/]+)',
                 'name:pattern': r'\A/[^/]+/([^/]+)',
                 'user:pattern': r'\A/([^/]+)',
-                'ref:pattern': r'\A/[^/]+/[^/]+/raw/([^/]+)',
+                'ref:pattern': r'\A/[^/]+/[^/]+/raw/([^/]+)/[^/]*\Z',
                 'html_page:prefix': 'https://bitbucket.org/',
                 'url:prefix': 'https://bitbucket.org/',
                 'url:suffix': '.git',  # assumes Git not Mercurial, which can't be disambiguated using the base URL
                 'download:format': 'https://bitbucket.org/{full_name}/get/{ref}.zip',
             }
         if netloc == 'gitlab.com':
             # A base URL may look like: https://gitlab.com/gitlab-org/gitter/env/raw/master/
             return {
                 'full_name:pattern': r'\A/(.+)/-/raw/',
                 'name:pattern': r'/([^/]+)/-/raw/',
                 'user:pattern': r'\A/([^/]+)',
-                'ref:pattern': r'/-/raw/([^/]+)',
+                'ref:pattern': r'/-/raw/([^/]+)/[^/]*\Z',
                 'html_page:prefix': 'https://gitlab.com/',
                 'url:prefix': 'https://gitlab.com/',
                 'url:suffix': '.git',
                 'download:format': 'https://gitlab.com/{full_name}/-/archive/{ref}.zip',
             }
```

### Comparing `ocdsextensionregistry-0.3.2/ocdsextensionregistry/profile_builder.py` & `ocdsextensionregistry-0.3.3/ocdsextensionregistry/profile_builder.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 from urllib.parse import urljoin, urlsplit
 
 import json_merge_patch
 import jsonref
 import requests
 
 from .codelist import Codelist
-from .exceptions import ExtensionWarning, NotAvailableInBulk
+from .exceptions import ExtensionWarning
 from .extension_registry import ExtensionRegistry
 from .extension_version import FIELD, ExtensionVersion
 from .util import _resolve_zip
 
 logger = logging.getLogger('ocdsextensionregistry')
 
 
@@ -100,15 +100,15 @@
                 yield self.registry.get(id=identifier, version=version)
         elif isinstance(self.extension_versions, Iterable):
             for url in self.extension_versions:
                 if not url or not isinstance(url, str):
                     continue
                 parsed = urlsplit(url)
                 data = dict.fromkeys(['Id', 'Date', 'Version', 'Base URL', 'Download URL'])
-                kwargs = {}
+                kwargs = {'input_url': url}
                 if parsed.scheme == 'file':
                     data['Download URL'] = url
                 elif url.endswith('/extension.json'):
                     data['Base URL'] = url[:-14]
                 elif url.endswith('/'):
                     data['Base URL'] = url
                 # If the files are served via API, with the filename as a query string parameter.
@@ -134,15 +134,15 @@
 
         # Replaces `null` with sentinel values, to preserve the null'ing of fields by extensions in the final patch.
         for extension in self.extensions():
             try:
                 patch = extension.remote('release-schema.json', default='{}')
                 patch = json.loads(re.sub(r':\s*null\b', ':"REPLACE_WITH_NULL"', patch))
             except (
-                NotAvailableInBulk,
+                UnicodeDecodeError,
                 json.JSONDecodeError,
                 requests.RequestException,
                 zipfile.BadZipFile,
             ) as e:
                 warnings.warn(ExtensionWarning(extension, e))
                 continue
             if extension_field:
```

### Comparing `ocdsextensionregistry-0.3.2/ocdsextensionregistry/util.py` & `ocdsextensionregistry-0.3.3/ocdsextensionregistry/util.py`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.3.2/ocdsextensionregistry.egg-info/PKG-INFO` & `ocdsextensionregistry-0.3.3/ocdsextensionregistry.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ocdsextensionregistry
-Version: 0.3.2
+Version: 0.3.3
 Summary: Eases access to information from the extension registry of the Open Contracting Data Standard
 Home-page: https://github.com/open-contracting/extension_registry.py
 Author: Open Contracting Partnership
 Author-email: data@open-contracting.org
 License: BSD
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
```

### Comparing `ocdsextensionregistry-0.3.2/ocdsextensionregistry.egg-info/SOURCES.txt` & `ocdsextensionregistry-0.3.3/ocdsextensionregistry.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.3.2/setup.cfg` & `ocdsextensionregistry-0.3.3/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ocdsextensionregistry
-version = 0.3.2
+version = 0.3.3
 author = Open Contracting Partnership
 author_email = data@open-contracting.org
 license = BSD
 description = Eases access to information from the extension registry of the Open Contracting Data Standard
 url = https://github.com/open-contracting/extension_registry.py
 long_description = file: README.rst
 long_description_content_type = text/x-rst
```

### Comparing `ocdsextensionregistry-0.3.2/tests/commands/test_download.py` & `ocdsextensionregistry-0.3.3/tests/commands/test_download.py`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.3.2/tests/commands/test_generate_data_file.py` & `ocdsextensionregistry-0.3.3/tests/commands/test_generate_data_file.py`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.3.2/tests/commands/test_generate_pot_files.py` & `ocdsextensionregistry-0.3.3/tests/commands/test_generate_pot_files.py`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.3.2/tests/fixtures/location-v1.1.4.json` & `ocdsextensionregistry-0.3.3/tests/fixtures/location-v1.1.4.json`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.3.2/tests/fixtures/ocds_coveredBy_extension/release-schema.json` & `ocdsextensionregistry-0.3.3/tests/fixtures/ocds_coveredBy_extension/release-schema.json`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.3.2/tests/test_api.py` & `ocdsextensionregistry-0.3.3/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.3.2/tests/test_codelist.py` & `ocdsextensionregistry-0.3.3/tests/test_codelist.py`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.3.2/tests/test_codelist_code.py` & `ocdsextensionregistry-0.3.3/tests/test_codelist_code.py`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.3.2/tests/test_extension.py` & `ocdsextensionregistry-0.3.3/tests/test_extension.py`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.3.2/tests/test_extension_registry.py` & `ocdsextensionregistry-0.3.3/tests/test_extension_registry.py`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.3.2/tests/test_extension_version.py` & `ocdsextensionregistry-0.3.3/tests/test_extension_version.py`

 * *Files 0% similar despite different names*

```diff
@@ -256,46 +256,50 @@
 
     assert result['codelists'] == ['locationGazetteers.csv', 'geometryType.csv']
 
 
 def test_metadata_old_format():
     # See https://raw.githubusercontent.com/open-contracting-extensions/ocds_location_extension/v1.1/extension.json
     download_url = 'https://api.github.com/repos/open-contracting-extensions/ocds_location_extension/zipball/v1.1'
+
     obj = ExtensionVersion(arguments(**{'Download URL': download_url}))
     result = obj.metadata
 
     assert result['name']['en'] == 'Location'
     assert result['description']['en'] == 'Communicates the location of proposed or executed contract delivery.'
     assert result['documentationUrl'] == {}
     assert result['compatibility'] == ['1.1']
 
 
 def test_schemas():
     download_url = 'https://github.com/open-contracting-extensions/ocds_location_extension/archive/master.zip'
+
     obj = ExtensionVersion(arguments(**{'Download URL': download_url}))
     result = obj.schemas
 
     assert len(result) == 1
     assert 'Location' in result['release-schema.json']['definitions']
 
 
 def test_schemas_without_metadata():
     download_url = 'https://api.github.com/repos/open-contracting-extensions/ocds_location_extension/zipball/v1.1'
+
     obj = ExtensionVersion(arguments(**{'Download URL': download_url}))
     result = obj.schemas
 
     assert len(result) == 3
     assert result['record-package-schema.json'] == {}
     assert result['release-package-schema.json'] == {}
     assert 'Location' in result['release-schema.json']['definitions']
 
 
 def test_schemas_without_metadata_or_download_url():
     base_url = 'https://raw.githubusercontent.com/open-contracting-extensions/ocds_location_extension/v1.1/'
     download_url = None
+
     obj = ExtensionVersion(arguments(**{'Base URL': base_url, 'Download URL': download_url}))
     result = obj.schemas
 
     assert len(result) == 3
     assert result['record-package-schema.json'] == {}
     assert result['release-package-schema.json'] == {}
     assert 'Location' in result['release-schema.json']['definitions']
```

### Comparing `ocdsextensionregistry-0.3.2/tests/test_profile_builder.py` & `ocdsextensionregistry-0.3.3/tests/test_profile_builder.py`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.3.2/tests/test_util.py` & `ocdsextensionregistry-0.3.3/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.3.2/tox.ini` & `ocdsextensionregistry-0.3.3/tox.ini`

 * *Files identical despite different names*

