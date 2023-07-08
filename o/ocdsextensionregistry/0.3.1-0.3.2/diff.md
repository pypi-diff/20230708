# Comparing `tmp/ocdsextensionregistry-0.3.1.tar.gz` & `tmp/ocdsextensionregistry-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ocdsextensionregistry-0.3.1.tar", last modified: Fri Jul  7 17:40:58 2023, max compression
+gzip compressed data, was "ocdsextensionregistry-0.3.2.tar", last modified: Fri Jul  7 21:32:02 2023, max compression
```

## Comparing `ocdsextensionregistry-0.3.1.tar` & `ocdsextensionregistry-0.3.2.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 17:40:58.269346 ocdsextensionregistry-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-07-07 17:40:46.000000 ocdsextensionregistry-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-07-07 17:40:46.000000 ocdsextensionregistry-0.3.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-07-07 17:40:58.269346 ocdsextensionregistry-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-07-07 17:40:46.000000 ocdsextensionregistry-0.3.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 17:40:58.261345 ocdsextensionregistry-0.3.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-07-07 17:40:46.000000 ocdsextensionregistry-0.3.1/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 17:40:58.261345 ocdsextensionregistry-0.3.1/docs/api/
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-07 17:40:46.000000 ocdsextensionregistry-0.3.1/docs/api/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-07-07 17:40:46.000000 ocdsextensionregistry-0.3.1/docs/api/codelist.rst
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-07-07 17:40:46.000000 ocdsextensionregistry-0.3.1/docs/api/codelist_code.rst
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-07-07 17:40:46.000000 ocdsextensionregistry-0.3.1/docs/api/exceptions.rst
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-07 17:40:46.000000 ocdsextensionregistry-0.3.1/docs/api/extension.rst
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-07-07 17:40:46.000000 ocdsextensionregistry-0.3.1/docs/api/extension_registry.rst
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-07-07 17:40:46.000000 ocdsextensionregistry-0.3.1/docs/api/extension_version.rst
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-07-07 17:40:46.000000 ocdsextensionregistry-0.3.1/docs/api/profile_builder.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-07 17:40:46.000000 ocdsextensionregistry-0.3.1/docs/api/util.rst
--rw-r--r--   0 runner    (1001) docker     (123)    16529 2023-07-07 17:40:46.000000 ocdsextensionregistry-0.3.1/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7430 2023-07-07 17:40:46.000000 ocdsextensionregistry-0.3.1/docs/cli.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-07-07 17:40:46.000000 ocdsextensionregistry-0.3.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-07-07 17:40:46.000000 ocdsextensionregistry-0.3.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-07-07 17:40:46.000000 ocdsextensionregistry-0.3.1/docs/library.rst
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-07 17:40:46.000000 ocdsextensionregistry-0.3.1/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2601 2023-07-07 17:40:46.000000 ocdsextensionregistry-0.3.1/docs/translation.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 17:40:58.265345 ocdsextensionregistry-0.3.1/ocdsextensionregistry/
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-07-07 17:40:46.000000 ocdsextensionregistry-0.3.1/ocdsextensionregistry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-07-07 17:40:46.000000 ocdsextensionregistry-0.3.1/ocdsextensionregistry/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5800 2023-07-07 17:40:46.000000 ocdsextensionregistry-0.3.1/ocdsextensionregistry/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     3737 2023-07-07 17:40:46.000000 ocdsextensionregistry-0.3.1/ocdsextensionregistry/codelist.py
--rw-r--r--   0 runner    (1001) docker     (123)      992 2023-07-07 17:40:46.000000 ocdsextensionregistry-0.3.1/ocdsextensionregistry/codelist_code.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 17:40:58.265345 ocdsextensionregistry-0.3.1/ocdsextensionregistry/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 17:40:46.000000 ocdsextensionregistry-0.3.1/ocdsextensionregistry/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1662 2023-07-07 17:40:46.000000 ocdsextensionregistry-0.3.1/ocdsextensionregistry/commands/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2804 2023-07-07 17:40:46.000000 ocdsextensionregistry-0.3.1/ocdsextensionregistry/commands/download.py
--rw-r--r--   0 runner    (1001) docker     (123)     7784 2023-07-07 17:40:46.000000 ocdsextensionregistry-0.3.1/ocdsextensionregistry/commands/generate_data_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     9256 2023-07-07 17:40:46.000000 ocdsextensionregistry-0.3.1/ocdsextensionregistry/commands/generate_pot_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-07-07 17:40:46.000000 ocdsextensionregistry-0.3.1/ocdsextensionregistry/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-07-07 17:40:46.000000 ocdsextensionregistry-0.3.1/ocdsextensionregistry/extension.py
--rw-r--r--   0 runner    (1001) docker     (123)     5472 2023-07-07 17:40:46.000000 ocdsextensionregistry-0.3.1/ocdsextensionregistry/extension_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)    13123 2023-07-07 17:40:46.000000 ocdsextensionregistry-0.3.1/ocdsextensionregistry/extension_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    16375 2023-07-07 17:40:46.000000 ocdsextensionregistry-0.3.1/ocdsextensionregistry/profile_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3146 2023-07-07 17:40:46.000000 ocdsextensionregistry-0.3.1/ocdsextensionregistry/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 17:40:58.265345 ocdsextensionregistry-0.3.1/ocdsextensionregistry.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-07-07 17:40:58.000000 ocdsextensionregistry-0.3.1/ocdsextensionregistry.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-07-07 17:40:58.000000 ocdsextensionregistry-0.3.1/ocdsextensionregistry.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 17:40:58.000000 ocdsextensionregistry-0.3.1/ocdsextensionregistry.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-07 17:40:58.000000 ocdsextensionregistry-0.3.1/ocdsextensionregistry.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-07 17:40:58.000000 ocdsextensionregistry-0.3.1/ocdsextensionregistry.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-07 17:40:58.000000 ocdsextensionregistry-0.3.1/ocdsextensionregistry.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-07 17:40:46.000000 ocdsextensionregistry-0.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-07-07 17:40:58.273346 ocdsextensionregistry-0.3.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 17:40:58.269346 ocdsextensionregistry-0.3.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-07-07 17:40:46.000000 ocdsextensionregistry-0.3.1/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 17:40:58.269346 ocdsextensionregistry-0.3.1/tests/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 17:40:46.000000 ocdsextensionregistry-0.3.1/tests/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4853 2023-07-07 17:40:46.000000 ocdsextensionregistry-0.3.1/tests/commands/test_download.py
--rw-r--r--   0 runner    (1001) docker     (123)     7243 2023-07-07 17:40:46.000000 ocdsextensionregistry-0.3.1/tests/commands/test_generate_data_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     2883 2023-07-07 17:40:46.000000 ocdsextensionregistry-0.3.1/tests/commands/test_generate_pot_files.py
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-07-07 17:40:46.000000 ocdsextensionregistry-0.3.1/tests/commands/test_none.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 17:40:58.269346 ocdsextensionregistry-0.3.1/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)    17612 2023-07-07 17:40:46.000000 ocdsextensionregistry-0.3.1/tests/fixtures/location-v1.1.4.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 17:40:58.269346 ocdsextensionregistry-0.3.1/tests/fixtures/ocds_coveredBy_extension/
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-07-07 17:40:46.000000 ocdsextensionregistry-0.3.1/tests/fixtures/ocds_coveredBy_extension/release-schema.json
--rw-r--r--   0 runner    (1001) docker     (123)     2824 2023-07-07 17:40:46.000000 ocdsextensionregistry-0.3.1/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5874 2023-07-07 17:40:46.000000 ocdsextensionregistry-0.3.1/tests/test_codelist.py
--rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-07-07 17:40:46.000000 ocdsextensionregistry-0.3.1/tests/test_codelist_code.py
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-07-07 17:40:46.000000 ocdsextensionregistry-0.3.1/tests/test_extension.py
--rw-r--r--   0 runner    (1001) docker     (123)    10484 2023-07-07 17:40:46.000000 ocdsextensionregistry-0.3.1/tests/test_extension_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)    12160 2023-07-07 17:40:46.000000 ocdsextensionregistry-0.3.1/tests/test_extension_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    15543 2023-07-07 17:40:46.000000 ocdsextensionregistry-0.3.1/tests/test_profile_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-07-07 17:40:46.000000 ocdsextensionregistry-0.3.1/tests/test_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-07-07 17:40:46.000000 ocdsextensionregistry-0.3.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 21:32:02.539585 ocdsextensionregistry-0.3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-07-07 21:31:53.000000 ocdsextensionregistry-0.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-07-07 21:31:53.000000 ocdsextensionregistry-0.3.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-07-07 21:32:02.539585 ocdsextensionregistry-0.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-07-07 21:31:53.000000 ocdsextensionregistry-0.3.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 21:32:02.535585 ocdsextensionregistry-0.3.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-07-07 21:31:53.000000 ocdsextensionregistry-0.3.2/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 21:32:02.535585 ocdsextensionregistry-0.3.2/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-07 21:31:53.000000 ocdsextensionregistry-0.3.2/docs/api/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-07-07 21:31:53.000000 ocdsextensionregistry-0.3.2/docs/api/codelist.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-07-07 21:31:53.000000 ocdsextensionregistry-0.3.2/docs/api/codelist_code.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-07-07 21:31:53.000000 ocdsextensionregistry-0.3.2/docs/api/exceptions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-07 21:31:53.000000 ocdsextensionregistry-0.3.2/docs/api/extension.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-07-07 21:31:53.000000 ocdsextensionregistry-0.3.2/docs/api/extension_registry.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-07-07 21:31:53.000000 ocdsextensionregistry-0.3.2/docs/api/extension_version.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-07-07 21:31:53.000000 ocdsextensionregistry-0.3.2/docs/api/profile_builder.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-07 21:31:53.000000 ocdsextensionregistry-0.3.2/docs/api/util.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    16981 2023-07-07 21:31:53.000000 ocdsextensionregistry-0.3.2/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7430 2023-07-07 21:31:53.000000 ocdsextensionregistry-0.3.2/docs/cli.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-07-07 21:31:53.000000 ocdsextensionregistry-0.3.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-07-07 21:31:53.000000 ocdsextensionregistry-0.3.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-07-07 21:31:53.000000 ocdsextensionregistry-0.3.2/docs/library.rst
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-07 21:31:53.000000 ocdsextensionregistry-0.3.2/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2601 2023-07-07 21:31:53.000000 ocdsextensionregistry-0.3.2/docs/translation.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 21:32:02.535585 ocdsextensionregistry-0.3.2/ocdsextensionregistry/
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-07-07 21:31:53.000000 ocdsextensionregistry-0.3.2/ocdsextensionregistry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-07-07 21:31:53.000000 ocdsextensionregistry-0.3.2/ocdsextensionregistry/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5800 2023-07-07 21:31:53.000000 ocdsextensionregistry-0.3.2/ocdsextensionregistry/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3737 2023-07-07 21:31:53.000000 ocdsextensionregistry-0.3.2/ocdsextensionregistry/codelist.py
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2023-07-07 21:31:53.000000 ocdsextensionregistry-0.3.2/ocdsextensionregistry/codelist_code.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 21:32:02.539585 ocdsextensionregistry-0.3.2/ocdsextensionregistry/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 21:31:53.000000 ocdsextensionregistry-0.3.2/ocdsextensionregistry/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1662 2023-07-07 21:31:53.000000 ocdsextensionregistry-0.3.2/ocdsextensionregistry/commands/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2804 2023-07-07 21:31:53.000000 ocdsextensionregistry-0.3.2/ocdsextensionregistry/commands/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7784 2023-07-07 21:31:53.000000 ocdsextensionregistry-0.3.2/ocdsextensionregistry/commands/generate_data_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9256 2023-07-07 21:31:53.000000 ocdsextensionregistry-0.3.2/ocdsextensionregistry/commands/generate_pot_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-07-07 21:31:53.000000 ocdsextensionregistry-0.3.2/ocdsextensionregistry/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-07-07 21:31:53.000000 ocdsextensionregistry-0.3.2/ocdsextensionregistry/extension.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5472 2023-07-07 21:31:53.000000 ocdsextensionregistry-0.3.2/ocdsextensionregistry/extension_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15016 2023-07-07 21:31:53.000000 ocdsextensionregistry-0.3.2/ocdsextensionregistry/extension_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16386 2023-07-07 21:31:53.000000 ocdsextensionregistry-0.3.2/ocdsextensionregistry/profile_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3146 2023-07-07 21:31:53.000000 ocdsextensionregistry-0.3.2/ocdsextensionregistry/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 21:32:02.539585 ocdsextensionregistry-0.3.2/ocdsextensionregistry.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-07-07 21:32:02.000000 ocdsextensionregistry-0.3.2/ocdsextensionregistry.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-07-07 21:32:02.000000 ocdsextensionregistry-0.3.2/ocdsextensionregistry.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 21:32:02.000000 ocdsextensionregistry-0.3.2/ocdsextensionregistry.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-07 21:32:02.000000 ocdsextensionregistry-0.3.2/ocdsextensionregistry.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-07 21:32:02.000000 ocdsextensionregistry-0.3.2/ocdsextensionregistry.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-07 21:32:02.000000 ocdsextensionregistry-0.3.2/ocdsextensionregistry.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-07 21:31:53.000000 ocdsextensionregistry-0.3.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-07-07 21:32:02.539585 ocdsextensionregistry-0.3.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 21:32:02.539585 ocdsextensionregistry-0.3.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-07-07 21:31:53.000000 ocdsextensionregistry-0.3.2/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 21:32:02.539585 ocdsextensionregistry-0.3.2/tests/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 21:31:53.000000 ocdsextensionregistry-0.3.2/tests/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4853 2023-07-07 21:31:53.000000 ocdsextensionregistry-0.3.2/tests/commands/test_download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7243 2023-07-07 21:31:53.000000 ocdsextensionregistry-0.3.2/tests/commands/test_generate_data_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2883 2023-07-07 21:31:53.000000 ocdsextensionregistry-0.3.2/tests/commands/test_generate_pot_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-07-07 21:31:53.000000 ocdsextensionregistry-0.3.2/tests/commands/test_none.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 21:32:02.539585 ocdsextensionregistry-0.3.2/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)    17612 2023-07-07 21:31:53.000000 ocdsextensionregistry-0.3.2/tests/fixtures/location-v1.1.4.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 21:32:02.539585 ocdsextensionregistry-0.3.2/tests/fixtures/ocds_coveredBy_extension/
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-07-07 21:31:53.000000 ocdsextensionregistry-0.3.2/tests/fixtures/ocds_coveredBy_extension/release-schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2824 2023-07-07 21:31:53.000000 ocdsextensionregistry-0.3.2/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5874 2023-07-07 21:31:53.000000 ocdsextensionregistry-0.3.2/tests/test_codelist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-07-07 21:31:53.000000 ocdsextensionregistry-0.3.2/tests/test_codelist_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-07-07 21:31:53.000000 ocdsextensionregistry-0.3.2/tests/test_extension.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10484 2023-07-07 21:31:53.000000 ocdsextensionregistry-0.3.2/tests/test_extension_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13099 2023-07-07 21:31:53.000000 ocdsextensionregistry-0.3.2/tests/test_extension_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15543 2023-07-07 21:31:53.000000 ocdsextensionregistry-0.3.2/tests/test_profile_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-07-07 21:31:53.000000 ocdsextensionregistry-0.3.2/tests/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-07-07 21:31:53.000000 ocdsextensionregistry-0.3.2/tox.ini
```

### Comparing `ocdsextensionregistry-0.3.1/LICENSE` & `ocdsextensionregistry-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.3.1/PKG-INFO` & `ocdsextensionregistry-0.3.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ocdsextensionregistry
-Version: 0.3.1
+Version: 0.3.2
 Summary: Eases access to information from the extension registry of the Open Contracting Data Standard
 Home-page: https://github.com/open-contracting/extension_registry.py
 Author: Open Contracting Partnership
 Author-email: data@open-contracting.org
 License: BSD
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
```

### Comparing `ocdsextensionregistry-0.3.1/README.rst` & `ocdsextensionregistry-0.3.2/README.rst`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.3.1/docs/Makefile` & `ocdsextensionregistry-0.3.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.3.1/docs/changelog.rst` & `ocdsextensionregistry-0.3.2/docs/changelog.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,16 @@
 Changelog
 =========
 
+0.3.2 (2023-07-07)
+------------------
+
+-  feat: Add :attr:`ocdsextensionregistry.extension_version.ExtensionVersion.repository_ref` and :attr:`~ocdsextensionregistry.extension_version.ExtensionVersion.repository_ref_download_url`.
+-  feat: Set :meth:`ocdsextensionregistry.extension_version.ExtensionVersion.download_url` to :attr:`~ocdsextensionregistry.extension_version.ExtensionVersion.repository_ref_download_url` on initialization, if possible.
+
 0.3.1 (2023-07-07)
 ------------------
 
 -  fix: :meth:`~ocdsextensionregistry.profile_builder.ProfileBuilder.extensions`: Support retrieval of the metadata file, if the ``extension_versions`` argument is a list of extensions' metadata files served via API.
 
 0.3.0 (2023-07-06)
 ------------------
@@ -32,16 +38,16 @@
 -  fix: :meth:`ocdsextensionregistry.extension_version.ExtensionVersion.__repr__`: No longer errors if initialized with ``file_urls`` only.
 -  fix: :meth:`ocdsextensionregistry.extension_version.ExtensionVersion.get_url`: Raises clearer error if initialized with a Download URL only.
 -  Add support for Sphinx 6.2 on Python 3.11.
 
 0.2.2 (2023-06-05)
 ------------------
 
--  fix: :meth:`~ocdsextensionregistry.extension_version.ExtensionVersion.repository_full_name` and :meth:`~ocdsextensionregistry.extension_version.ExtensionVersion.repository_name` return the correct name for GitLab URLs.
--  fix: Clarify error message for ``AttributeError`` on :meth:`~ocdsextensionregistry.extension_version.ExtensionVersion.repository_full_name`, :meth:`~ocdsextensionregistry.extension_version.ExtensionVersion.repository_name`, and :meth:`~ocdsextensionregistry.extension_version.ExtensionVersion.repository_user`.
+-  fix: :attr:`~ocdsextensionregistry.extension_version.ExtensionVersion.repository_full_name` and :attr:`~ocdsextensionregistry.extension_version.ExtensionVersion.repository_name` return the correct name for GitLab URLs.
+-  fix: Clarify error message for ``AttributeError`` on :attr:`~ocdsextensionregistry.extension_version.ExtensionVersion.repository_full_name`, :attr:`~ocdsextensionregistry.extension_version.ExtensionVersion.repository_name`, and :attr:`~ocdsextensionregistry.extension_version.ExtensionVersion.repository_user`.
 
 0.2.1 (2023-05-24)
 ------------------
 
 -  feat: Add a ``--no-frozen`` option to all commands.
 -  Drop support for Python 3.7.
```

### Comparing `ocdsextensionregistry-0.3.1/docs/cli.rst` & `ocdsextensionregistry-0.3.2/docs/cli.rst`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.3.1/docs/conf.py` & `ocdsextensionregistry-0.3.2/docs/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 # -- Project information -----------------------------------------------------
 
 project = "OCDS Extension Registry Python Package"
 copyright = "2018, Open Contracting Partnership"
 author = "Open Contracting Partnership"
 
 # The short X.Y version
-version = "0.3.1"
+version = "0.3.2"
 # The full version, including alpha/beta/rc tags
 release = version
 
 
 # -- General configuration ---------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
```

### Comparing `ocdsextensionregistry-0.3.1/docs/index.rst` & `ocdsextensionregistry-0.3.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.3.1/docs/translation.rst` & `ocdsextensionregistry-0.3.2/docs/translation.rst`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.3.1/ocdsextensionregistry/__init__.py` & `ocdsextensionregistry-0.3.2/ocdsextensionregistry/__init__.py`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.3.1/ocdsextensionregistry/__main__.py` & `ocdsextensionregistry-0.3.2/ocdsextensionregistry/__main__.py`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.3.1/ocdsextensionregistry/api.py` & `ocdsextensionregistry-0.3.2/ocdsextensionregistry/api.py`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.3.1/ocdsextensionregistry/codelist.py` & `ocdsextensionregistry-0.3.2/ocdsextensionregistry/codelist.py`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.3.1/ocdsextensionregistry/codelist_code.py` & `ocdsextensionregistry-0.3.2/ocdsextensionregistry/codelist_code.py`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.3.1/ocdsextensionregistry/commands/base.py` & `ocdsextensionregistry-0.3.2/ocdsextensionregistry/commands/base.py`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.3.1/ocdsextensionregistry/commands/download.py` & `ocdsextensionregistry-0.3.2/ocdsextensionregistry/commands/download.py`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.3.1/ocdsextensionregistry/commands/generate_data_file.py` & `ocdsextensionregistry-0.3.2/ocdsextensionregistry/commands/generate_data_file.py`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.3.1/ocdsextensionregistry/commands/generate_pot_files.py` & `ocdsextensionregistry-0.3.2/ocdsextensionregistry/commands/generate_pot_files.py`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.3.1/ocdsextensionregistry/exceptions.py` & `ocdsextensionregistry-0.3.2/ocdsextensionregistry/exceptions.py`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.3.1/ocdsextensionregistry/extension.py` & `ocdsextensionregistry-0.3.2/ocdsextensionregistry/extension.py`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.3.1/ocdsextensionregistry/extension_registry.py` & `ocdsextensionregistry-0.3.2/ocdsextensionregistry/extension_registry.py`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.3.1/ocdsextensionregistry/extension_version.py` & `ocdsextensionregistry-0.3.2/ocdsextensionregistry/extension_version.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,39 +9,52 @@
 import requests
 
 from .codelist import Codelist
 from .exceptions import DoesNotExist, NotAvailableInBulk
 from .util import _resolve_zip, session
 
 SCHEMAS = ('record-package-schema.json', 'release-package-schema.json', 'release-schema.json')
+FIELD_NAME = '4F434453'  # OCDS in hexidecimal
+FIELD = f'{{{FIELD_NAME}}}'
 
 
 class ExtensionVersion:
-    def __init__(self, data, file_urls=None):
+    def __init__(self, data, file_urls=None, url_pattern=None):
         """
         Accepts a row from extension_versions.csv and assigns values to properties.
         """
         self.id = data['Id']
         self.date = data['Date']
         self.version = data['Version']
         self.base_url = data['Base URL']
         self.download_url = data['Download URL']
+
+        self._url_pattern = url_pattern
         self._file_urls = file_urls or {}
         self._files = None
         self._metadata = None
         self._schemas = None
         self._codelists = None
 
+        # This runs only when using this class outside the context of the extension registry.
+        if not self.download_url:
+            try:
+                self.download_url = self.repository_ref_download_url
+            except (AttributeError, NotImplementedError):
+                pass
+
     def __repr__(self):
         if self.id and self.version:
             return f'{self.id}=={self.version}'
         elif self.base_url:
             return self.base_url
         elif self.download_url:
             return self.download_url
+        elif self._url_pattern:
+            return self._url_pattern
         return self._file_urls['release-schema.json']
 
     def update(self, other):
         """
         Merges in the properties of another Extension or ExtensionVersion object.
         """
         for k, v in other.as_dict().items():
@@ -59,14 +72,16 @@
 
         :raises NotImplementedError: if the basename is not in the file URLs and the base URL is not set
         """
         if basename in self._file_urls:
             return self._file_urls[basename]
         if self.base_url:
             return self.base_url + basename
+        if self._url_pattern:
+            return self._url_pattern.format(**{FIELD_NAME: basename})
         raise NotImplementedError("get_url() with no base URL or matching file URL is not implemented")
 
     def remote(self, basename, default=None):
         """
         Returns the contents of the file within the extension. If the ``default`` is set and the file does not exist,
         returns the provided ``default`` value.
 
@@ -206,68 +221,71 @@
         return self._codelists
 
     @property
     def repository_full_name(self):
         """
         Returns the full name of the extension's repository, which should be a unique identifier on the hosting
         service, e.g. open-contracting-extensions/ocds_bid_extension
-
-        Experimental
         """
         return self._repository_property('full_name')
 
     @property
     def repository_name(self):
         """
         Returns the short name of the extension's repository, i.e. omitting any organizational prefix, which can be
         used to create directories, e.g. ocds_bid_extension
-
-        Experimental
         """
         return self._repository_property('name')
 
     @property
     def repository_user(self):
         """
         Returns the user or organization to which the extension's repository belongs, e.g. open-contracting-extensions
-
-        Experimental
         """
         return self._repository_property('user')
 
     @property
+    def repository_ref(self):
+        """
+        Returns the ref in the extension's URL, e.g. the commit, tag or branch, like v1.1.5
+        """
+        return self._repository_property('ref')
+
+    @property
     def repository_user_page(self):
         """
         Returns the URL to the landing page of the user or organization to which the extension's repository belongs,
         e.g. https://github.com/open-contracting-extensions
-
-        Experimental
         """
         return self._repository_property('user_page')
 
     @property
     def repository_html_page(self):
         """
         Returns the URL to the landing page of the extension's repository, e.g.
         https://github.com/open-contracting-extensions/ocds_bid_extension
-
-        Experimental
         """
         return self._repository_property('html_page')
 
     @property
     def repository_url(self):
         """
         Returns the URL of the extension's repository, in a format that can be input to a VCS program without
         modification, e.g. https://github.com/open-contracting-extensions/ocds_bid_extension.git
-
-        Experimental
         """
         return self._repository_property('url')
 
+    @property
+    def repository_ref_download_url(self):
+        """
+        Returns the download URL for the ref in the extensions's URL, e.g.
+        https://github.com/open-contracting-extensions/ocds_bid_extension/archive/v1.1.5.zip
+        """
+        return self._repository_property('ref_download_url')
+
     def _repository_full_name(self, parsed, config):
         match = re.search(config['full_name:pattern'], parsed.path)
         if match:
             return match.group(1)
         raise AttributeError(f"{parsed.path} !~ {config['full_name:pattern']}")
 
     def _repository_name(self, parsed, config):
@@ -278,23 +296,35 @@
 
     def _repository_user(self, parsed, config):
         match = re.search(config['user:pattern'], parsed.path)
         if match:
             return match.group(1)
         raise AttributeError(f"{parsed.path} !~ {config['user:pattern']}")
 
+    def _repository_ref(self, parsed, config):
+        match = re.search(config['ref:pattern'], parsed.path)
+        if match:
+            return match.group(1)
+        raise AttributeError(f"{parsed.path} !~ {config['ref:pattern']}")
+
     def _repository_user_page(self, parsed, config):
         return config['html_page:prefix'] + self._repository_user(parsed, config)
 
     def _repository_html_page(self, parsed, config):
         return config['html_page:prefix'] + self._repository_full_name(parsed, config)
 
     def _repository_url(self, parsed, config):
         return config['url:prefix'] + self._repository_full_name(parsed, config) + config['url:suffix']
 
+    def _repository_ref_download_url(self, parsed, config):
+        return config['download:format'].format(
+            full_name=self._repository_full_name(parsed, config),
+            ref=self._repository_ref(parsed, config),
+        )
+
     def _repository_property(self, prop):
         parsed = urlsplit(self.base_url)
         config = self._configuration(parsed)
         if config:
             return getattr(self, '_repository_' + prop)(parsed, config)
         raise NotImplementedError(f"can't determine {prop} from {self.base_url}")
 
@@ -310,31 +340,37 @@
         netloc = parsed.netloc
         if netloc == 'raw.githubusercontent.com':
             # Sample base URL: https://raw.githubusercontent.com/open-contracting-extensions/ocds_bid_extension/v1.1.4/
             return {
                 'full_name:pattern': r'\A/([^/]+/[^/]+)',
                 'name:pattern': r'\A/[^/]+/([^/]+)',
                 'user:pattern': r'\A/([^/]+)',
+                'ref:pattern': r'\A/[^/]+/[^/]+/([^/]+)',
                 'html_page:prefix': 'https://github.com/',
                 'url:prefix': 'git@github.com:',
                 'url:suffix': '.git',
+                'download:format': 'https://github.com/{full_name}/archive/{ref}.zip',
             }
         if netloc == 'bitbucket.org':
             # A base URL may look like: https://bitbucket.org/facebook/hgsql/raw/default/
             return {
                 'full_name:pattern': r'\A/([^/]+/[^/]+)',
                 'name:pattern': r'\A/[^/]+/([^/]+)',
                 'user:pattern': r'\A/([^/]+)',
+                'ref:pattern': r'\A/[^/]+/[^/]+/raw/([^/]+)',
                 'html_page:prefix': 'https://bitbucket.org/',
                 'url:prefix': 'https://bitbucket.org/',
                 'url:suffix': '.git',  # assumes Git not Mercurial, which can't be disambiguated using the base URL
+                'download:format': 'https://bitbucket.org/{full_name}/get/{ref}.zip',
             }
         if netloc == 'gitlab.com':
             # A base URL may look like: https://gitlab.com/gitlab-org/gitter/env/raw/master/
             return {
                 'full_name:pattern': r'\A/(.+)/-/raw/',
                 'name:pattern': r'/([^/]+)/-/raw/',
                 'user:pattern': r'\A/([^/]+)',
+                'ref:pattern': r'/-/raw/([^/]+)',
                 'html_page:prefix': 'https://gitlab.com/',
                 'url:prefix': 'https://gitlab.com/',
                 'url:suffix': '.git',
+                'download:format': 'https://gitlab.com/{full_name}/-/archive/{ref}.zip',
             }
```

### Comparing `ocdsextensionregistry-0.3.1/ocdsextensionregistry/profile_builder.py` & `ocdsextensionregistry-0.3.2/ocdsextensionregistry/profile_builder.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 import json_merge_patch
 import jsonref
 import requests
 
 from .codelist import Codelist
 from .exceptions import ExtensionWarning, NotAvailableInBulk
 from .extension_registry import ExtensionRegistry
-from .extension_version import ExtensionVersion
+from .extension_version import FIELD, ExtensionVersion
 from .util import _resolve_zip
 
 logger = logging.getLogger('ocdsextensionregistry')
 
 
 class ProfileBuilder:
     def __init__(self, standard_tag, extension_versions, registry_base_url=None, standard_base_url=None,
@@ -107,22 +107,21 @@
                 kwargs = {}
                 if parsed.scheme == 'file':
                     data['Download URL'] = url
                 elif url.endswith('/extension.json'):
                     data['Base URL'] = url[:-14]
                 elif url.endswith('/'):
                     data['Base URL'] = url
-                elif parsed.path.endswith('.json'):
-                    kwargs['file_urls'] = {'release-schema.json': url}
                 # If the files are served via API, with the filename as a query string parameter.
                 elif 'extension.json' in url:
-                    kwargs['file_urls'] = {
-                        'extension.json': url,
-                        'release-schema.json': url.replace('extension.json', 'release-schema.json'),
-                    }
+                    kwargs['url_pattern'] = url.replace('extension.json', FIELD)
+                elif 'release-schema.json' in url:
+                    kwargs['url_pattern'] = url.replace('release-schema.json', FIELD)
+                elif parsed.path.endswith('.json'):
+                    kwargs['file_urls'] = {'release-schema.json': url}
                 else:
                     data['Download URL'] = url
                 yield ExtensionVersion(data, **kwargs)
 
     def release_schema_patch(self, extension_field=None, language='en'):
         """
         Returns the consolidated release schema patch.
```

### Comparing `ocdsextensionregistry-0.3.1/ocdsextensionregistry/util.py` & `ocdsextensionregistry-0.3.2/ocdsextensionregistry/util.py`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.3.1/ocdsextensionregistry.egg-info/PKG-INFO` & `ocdsextensionregistry-0.3.2/ocdsextensionregistry.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ocdsextensionregistry
-Version: 0.3.1
+Version: 0.3.2
 Summary: Eases access to information from the extension registry of the Open Contracting Data Standard
 Home-page: https://github.com/open-contracting/extension_registry.py
 Author: Open Contracting Partnership
 Author-email: data@open-contracting.org
 License: BSD
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
```

### Comparing `ocdsextensionregistry-0.3.1/ocdsextensionregistry.egg-info/SOURCES.txt` & `ocdsextensionregistry-0.3.2/ocdsextensionregistry.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.3.1/setup.cfg` & `ocdsextensionregistry-0.3.2/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ocdsextensionregistry
-version = 0.3.1
+version = 0.3.2
 author = Open Contracting Partnership
 author_email = data@open-contracting.org
 license = BSD
 description = Eases access to information from the extension registry of the Open Contracting Data Standard
 url = https://github.com/open-contracting/extension_registry.py
 long_description = file: README.rst
 long_description_content_type = text/x-rst
```

### Comparing `ocdsextensionregistry-0.3.1/tests/commands/test_download.py` & `ocdsextensionregistry-0.3.2/tests/commands/test_download.py`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.3.1/tests/commands/test_generate_data_file.py` & `ocdsextensionregistry-0.3.2/tests/commands/test_generate_data_file.py`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.3.1/tests/commands/test_generate_pot_files.py` & `ocdsextensionregistry-0.3.2/tests/commands/test_generate_pot_files.py`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.3.1/tests/fixtures/location-v1.1.4.json` & `ocdsextensionregistry-0.3.2/tests/fixtures/location-v1.1.4.json`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.3.1/tests/fixtures/ocds_coveredBy_extension/release-schema.json` & `ocdsextensionregistry-0.3.2/tests/fixtures/ocds_coveredBy_extension/release-schema.json`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.3.1/tests/test_api.py` & `ocdsextensionregistry-0.3.2/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.3.1/tests/test_codelist.py` & `ocdsextensionregistry-0.3.2/tests/test_codelist.py`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.3.1/tests/test_codelist_code.py` & `ocdsextensionregistry-0.3.2/tests/test_codelist_code.py`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.3.1/tests/test_extension.py` & `ocdsextensionregistry-0.3.2/tests/test_extension.py`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.3.1/tests/test_extension_registry.py` & `ocdsextensionregistry-0.3.2/tests/test_extension_registry.py`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.3.1/tests/test_extension_version.py` & `ocdsextensionregistry-0.3.2/tests/test_extension_version.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,14 +54,21 @@
 def test_repr_file_urls():
     data = dict.fromkeys(['Id', 'Date', 'Version', 'Base URL', 'Download URL'])
     obj = ExtensionVersion(data, file_urls={'release-schema.json': 'https://example.com/release-schema.json'})
 
     assert repr(obj) == 'https://example.com/release-schema.json'
 
 
+def test_repr_url_pattern():
+    data = dict.fromkeys(['Id', 'Date', 'Version', 'Base URL', 'Download URL'])
+    obj = ExtensionVersion(data, url_pattern='https://example.com/?file={4F434453}&key=value')
+
+    assert repr(obj) == 'https://example.com/?file={4F434453}&key=value'
+
+
 def test_update():
     obj = ExtensionVersion(arguments())
     obj.update(Extension({'Id': 'location', 'Category': 'item', 'Core': 'true'}))
 
     assert obj.id == 'location'
     assert obj.category == 'item'
     assert obj.core is True
@@ -99,35 +106,44 @@
 ])
 def test_get_url(args, expected):
     obj = ExtensionVersion(args)
 
     assert obj.get_url('extension.json') == expected
 
 
+def test_get_url_file_urls():
+    url = 'https://example.com/release-schema.json'
+
+    obj = ExtensionVersion(arguments(), file_urls={'release-schema.json': url})
+
+    assert obj.get_url('release-schema.json') == url
+
+
+def test_get_url_url_pattern():
+    obj = ExtensionVersion(arguments(**{
+        'Id': None,
+        'Base URL': None,
+    }), url_pattern='https://example.com/?file={4F434453}&key=value')
+
+    assert obj.get_url('release-schema.json') == 'https://example.com/?file=release-schema.json&key=value'
+
+
 def test_get_url_download_url():
     args = arguments(**{
         'Id': None,
         'Base URL': None,
         'Download URL': 'https://api.github.com/repos/open-contracting-extensions/ocds_location_extension/zipball/v1.1.3',  # noqa: E501
     })
 
     with pytest.raises(NotImplementedError) as excinfo:
         ExtensionVersion(args).get_url('extension.json')
 
     assert str(excinfo.value) == 'get_url() with no base URL or matching file URL is not implemented'
 
 
-def test_get_url_file_urls():
-    url = 'https://example.com/release-schema.json'
-
-    obj = ExtensionVersion(arguments(), file_urls={'release-schema.json': url})
-
-    assert obj.get_url('release-schema.json') == url
-
-
 def test_remote():
     obj = ExtensionVersion(arguments(**{'Download URL': None}))
 
     data = obj.remote('extension.json')
     # Repeat requests should return the same result.
     data = obj.remote('extension.json')
 
@@ -157,26 +173,27 @@
 
     assert json.loads(data) == {'key': 'value'}
 
 
 def test_remote_file_urls():
     url = 'https://raw.githubusercontent.com/open-contracting-extensions/ocds_coveredBy_extension/master/release-schema.json'  # noqa: E501
 
-    obj = ExtensionVersion(arguments(**{'Download URL': None}), file_urls={'release-schema.json': url})
+    obj = ExtensionVersion(arguments(), file_urls={'release-schema.json': url})
+    obj.download_url = None
 
     data = obj.remote('release-schema.json')
     # Repeat requests should return the same result.
     data = obj.remote('release-schema.json')
 
-    print(data)
     assert 'coveredBy' in json.loads(data)['definitions']['Tender']['properties']
 
 
 def test_remote_nonexistent():
-    obj = ExtensionVersion(arguments(**{'Download URL': None}))
+    obj = ExtensionVersion(arguments())
+    obj.download_url = None
     with pytest.raises(requests.exceptions.HTTPError) as excinfo:
         obj.remote('nonexistent')
 
     assert str(excinfo.value) == "404 Client Error: Not Found for url: https://raw.githubusercontent.com/open-contracting-extensions/ocds_location_extension/v1.1.3/nonexistent"  # noqa: E501
 
 
 def test_remote_download_url_nonexistent():
@@ -184,15 +201,16 @@
     with pytest.raises(DoesNotExist) as excinfo:
         obj.remote('nonexistent')
 
     assert str(excinfo.value) == "File 'nonexistent' does not exist in location==v1.1.3"
 
 
 def test_zipfile_not_available_in_bulk():
-    obj = ExtensionVersion(arguments(**{'Download URL': None}))
+    obj = ExtensionVersion(arguments())
+    obj.download_url = None
     with pytest.raises(NotAvailableInBulk) as excinfo:
         obj.zipfile()
 
     assert str(excinfo.value) == "ExtensionVersion.zipfile() requires a download_url."
 
 
 def test_remote_codelists_only_base_url():
@@ -211,28 +229,29 @@
     obj = ExtensionVersion(args)
 
     assert obj.remote('release-schema.json', default='{}') == '{}'
 
 
 def test_files():
     obj = ExtensionVersion(arguments())
-    data = obj.files
+    result = obj.files
 
-    assert 'LICENSE' in data
+    assert 'LICENSE' in result
 
     # This method should not parse file contents.
-    for value in data.values():
+    for value in result.values():
         assert isinstance(value, (bytes, str))
 
 
 def test_files_without_download_url():
-    obj = ExtensionVersion(arguments(**{'Download URL': None}))
-    data = obj.files
+    obj = ExtensionVersion(arguments())
+    obj.download_url = None
+    result = obj.files
 
-    assert data == {}
+    assert result == {}
 
 
 def test_metadata():
     obj = ExtensionVersion(arguments())
     result = obj.metadata
 
     assert result['codelists'] == ['locationGazetteers.csv', 'geometryType.csv']
@@ -289,33 +308,36 @@
     assert len(result) == 2
     assert result['locationGazetteers.csv'].fieldnames == ['Category', 'Code', 'Title', 'Description', 'Source',
                                                            'URI Pattern']
 
 
 def test_codelists_without_metadata():
     download_url = 'https://api.github.com/repos/open-contracting-extensions/ocds_location_extension/zipball/v1.1'
+
     obj = ExtensionVersion(arguments(**{'Download URL': download_url}))
     result = obj.codelists
 
     assert len(result) == 1
     assert result['locationGazeteers.csv'].fieldnames == ['Category', 'Code', 'Title', 'Description', 'Source',
                                                           'URI_Pattern']
 
 
 def test_codelists_without_metadata_or_download_url():
     base_url = 'https://raw.githubusercontent.com/open-contracting-extensions/ocds_location_extension/v1.1/'
-    download_url = None
-    obj = ExtensionVersion(arguments(**{'Base URL': base_url, 'Download URL': download_url}))
+
+    obj = ExtensionVersion(arguments(**{'Base URL': base_url}))
+    obj.download_url = None
     result = obj.codelists
 
     assert result == {}
 
 
 def test_codelists_with_CR_newlines():
     download_url = 'https://api.github.com/repos/open-contracting-extensions/ocds_bid_extension/zipball/v1.1'
+
     obj = ExtensionVersion(arguments(**{'Download URL': download_url}))
     result = obj.codelists
 
     assert len(result) == 2
     assert result['bidStatistics.csv'].fieldnames == ['Category', 'Code', 'Title', 'Description', 'Min', 'Max',
                                                       'Required by']
 
@@ -337,14 +359,21 @@
 def test_repository_user():
     obj = ExtensionVersion(arguments())
     result = obj.repository_user
 
     assert result == 'open-contracting-extensions'
 
 
+def test_repository_ref():
+    obj = ExtensionVersion(arguments())
+    result = obj.repository_ref
+
+    assert result == 'v1.1.3'
+
+
 def test_repository_user_page():
     obj = ExtensionVersion(arguments())
     result = obj.repository_user_page
 
     assert result == 'https://github.com/open-contracting-extensions'
 
 
@@ -356,7 +385,14 @@
 
 
 def test_repository_url():
     obj = ExtensionVersion(arguments())
     result = obj.repository_url
 
     assert result == 'git@github.com:open-contracting-extensions/ocds_location_extension.git'
+
+
+def test_repository_ref_download_url():
+    obj = ExtensionVersion(arguments())
+    result = obj.repository_ref_download_url
+
+    assert result == 'https://github.com/open-contracting-extensions/ocds_location_extension/archive/v1.1.3.zip'
```

### Comparing `ocdsextensionregistry-0.3.1/tests/test_profile_builder.py` & `ocdsextensionregistry-0.3.2/tests/test_profile_builder.py`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.3.1/tests/test_util.py` & `ocdsextensionregistry-0.3.2/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.3.1/tox.ini` & `ocdsextensionregistry-0.3.2/tox.ini`

 * *Files identical despite different names*

