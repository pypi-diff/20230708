# Comparing `tmp/pyams_thesaurus-1.3.4.tar.gz` & `tmp/pyams_thesaurus-1.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyams_thesaurus-1.3.4.tar", last modified: Thu Apr 13 12:51:07 2023, max compression
+gzip compressed data, was "dist/pyams_thesaurus-1.3.5.tar", last modified: Fri Jul  7 22:13:54 2023, max compression
```

## Comparing `pyams_thesaurus-1.3.4.tar` & `pyams_thesaurus-1.3.5.tar`

### file list

```diff
@@ -1,90 +1,90 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 12:51:07.000000 pyams_thesaurus-1.3.4/
--rw-rw-rw-   0 root         (0) root         (0)     2191 2023-04-13 12:50:45.000000 pyams_thesaurus-1.3.4/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      104 2023-04-13 12:50:45.000000 pyams_thesaurus-1.3.4/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     3083 2023-04-13 12:51:07.000000 pyams_thesaurus-1.3.4/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 12:51:07.000000 pyams_thesaurus-1.3.4/docs/
--rwxrwxrwx   0 root         (0) root         (0)     1297 2023-04-13 12:50:45.000000 pyams_thesaurus-1.3.4/docs/HISTORY.rst
--rw-rw-rw-   0 root         (0) root         (0)     1233 2023-04-13 12:50:45.000000 pyams_thesaurus-1.3.4/docs/README.rst
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-13 12:51:07.000000 pyams_thesaurus-1.3.4/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     2876 2023-04-13 12:50:45.000000 pyams_thesaurus-1.3.4/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 12:51:07.000000 pyams_thesaurus-1.3.4/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 12:51:07.000000 pyams_thesaurus-1.3.4/src/pyams_thesaurus/
--rw-rw-rw-   0 root         (0) root         (0)      873 2023-04-13 12:50:45.000000 pyams_thesaurus-1.3.4/src/pyams_thesaurus/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 12:51:07.000000 pyams_thesaurus-1.3.4/src/pyams_thesaurus/api/
--rw-rw-rw-   0 root         (0) root         (0)     1717 2023-04-13 12:50:45.000000 pyams_thesaurus-1.3.4/src/pyams_thesaurus/api/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7316 2023-04-13 12:50:45.000000 pyams_thesaurus-1.3.4/src/pyams_thesaurus/api/rest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 12:51:07.000000 pyams_thesaurus-1.3.4/src/pyams_thesaurus/doctests/
--rw-rw-rw-   0 root         (0) root         (0)    20142 2023-04-13 12:50:45.000000 pyams_thesaurus-1.3.4/src/pyams_thesaurus/doctests/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 12:51:07.000000 pyams_thesaurus-1.3.4/src/pyams_thesaurus/doctests/data/
--rw-rw-rw-   0 root         (0) root         (0)  2939491 2023-04-13 12:50:45.000000 pyams_thesaurus-1.3.4/src/pyams_thesaurus/doctests/data/SAMPLE-SKOS.xml
--rw-rw-rw-   0 root         (0) root         (0)  2735784 2023-04-13 12:50:45.000000 pyams_thesaurus-1.3.4/src/pyams_thesaurus/doctests/data/SAMPLE-Superdoc.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 12:51:07.000000 pyams_thesaurus-1.3.4/src/pyams_thesaurus/extension/
--rw-rw-rw-   0 root         (0) root         (0)      550 2023-04-13 12:50:45.000000 pyams_thesaurus-1.3.4/src/pyams_thesaurus/extension/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 12:51:07.000000 pyams_thesaurus-1.3.4/src/pyams_thesaurus/extension/html/
--rw-rw-rw-   0 root         (0) root         (0)     2049 2023-04-13 12:50:45.000000 pyams_thesaurus-1.3.4/src/pyams_thesaurus/extension/html/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1217 2023-04-13 12:50:45.000000 pyams_thesaurus-1.3.4/src/pyams_thesaurus/extension/html/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 12:51:07.000000 pyams_thesaurus-1.3.4/src/pyams_thesaurus/extension/html/zmi/
--rw-rw-rw-   0 root         (0) root         (0)     1535 2023-04-13 12:50:45.000000 pyams_thesaurus-1.3.4/src/pyams_thesaurus/extension/html/zmi/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 12:51:07.000000 pyams_thesaurus-1.3.4/src/pyams_thesaurus/generations/
--rw-rw-rw-   0 root         (0) root         (0)     1380 2023-04-13 12:50:45.000000 pyams_thesaurus-1.3.4/src/pyams_thesaurus/generations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4274 2023-04-13 12:50:45.000000 pyams_thesaurus-1.3.4/src/pyams_thesaurus/include.py
--rw-rw-rw-   0 root         (0) root         (0)     4277 2023-04-13 12:50:45.000000 pyams_thesaurus-1.3.4/src/pyams_thesaurus/index.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 12:51:07.000000 pyams_thesaurus-1.3.4/src/pyams_thesaurus/interfaces/
--rw-rw-rw-   0 root         (0) root         (0)     1862 2023-04-13 12:50:45.000000 pyams_thesaurus-1.3.4/src/pyams_thesaurus/interfaces/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1632 2023-04-13 12:50:45.000000 pyams_thesaurus-1.3.4/src/pyams_thesaurus/interfaces/extension.py
--rw-rw-rw-   0 root         (0) root         (0)     1317 2023-04-13 12:50:45.000000 pyams_thesaurus-1.3.4/src/pyams_thesaurus/interfaces/index.py
--rw-rw-rw-   0 root         (0) root         (0)     5471 2023-04-13 12:50:45.000000 pyams_thesaurus-1.3.4/src/pyams_thesaurus/interfaces/loader.py
--rw-rw-rw-   0 root         (0) root         (0)     7494 2023-04-13 12:50:45.000000 pyams_thesaurus-1.3.4/src/pyams_thesaurus/interfaces/term.py
--rw-rw-rw-   0 root         (0) root         (0)     8247 2023-04-13 12:50:45.000000 pyams_thesaurus-1.3.4/src/pyams_thesaurus/interfaces/thesaurus.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 12:51:07.000000 pyams_thesaurus-1.3.4/src/pyams_thesaurus/loader/
--rw-rw-rw-   0 root         (0) root         (0)    10069 2023-04-13 12:50:45.000000 pyams_thesaurus-1.3.4/src/pyams_thesaurus/loader/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2844 2023-04-13 12:50:45.000000 pyams_thesaurus-1.3.4/src/pyams_thesaurus/loader/config.py
--rw-rw-rw-   0 root         (0) root         (0)    10638 2023-04-13 12:50:45.000000 pyams_thesaurus-1.3.4/src/pyams_thesaurus/loader/skos.py
--rw-rw-rw-   0 root         (0) root         (0)     8442 2023-04-13 12:50:45.000000 pyams_thesaurus-1.3.4/src/pyams_thesaurus/loader/superdoc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 12:51:07.000000 pyams_thesaurus-1.3.4/src/pyams_thesaurus/locales/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 12:51:07.000000 pyams_thesaurus-1.3.4/src/pyams_thesaurus/locales/fr/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 12:51:07.000000 pyams_thesaurus-1.3.4/src/pyams_thesaurus/locales/fr/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)    13065 2023-04-13 12:50:45.000000 pyams_thesaurus-1.3.4/src/pyams_thesaurus/locales/fr/LC_MESSAGES/pyams_thesaurus.mo
--rw-rw-rw-   0 root         (0) root         (0)    21065 2023-04-13 12:50:45.000000 pyams_thesaurus-1.3.4/src/pyams_thesaurus/locales/fr/LC_MESSAGES/pyams_thesaurus.po
--rw-rw-rw-   0 root         (0) root         (0)    15976 2023-04-13 12:50:45.000000 pyams_thesaurus-1.3.4/src/pyams_thesaurus/locales/pyams_thesaurus.pot
--rw-rw-rw-   0 root         (0) root         (0)     1042 2023-04-13 12:50:45.000000 pyams_thesaurus-1.3.4/src/pyams_thesaurus/manager.py
--rw-rw-rw-   0 root         (0) root         (0)     2727 2023-04-13 12:50:45.000000 pyams_thesaurus-1.3.4/src/pyams_thesaurus/schema.py
--rw-rw-rw-   0 root         (0) root         (0)    19509 2023-04-13 12:50:45.000000 pyams_thesaurus-1.3.4/src/pyams_thesaurus/term.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 12:51:07.000000 pyams_thesaurus-1.3.4/src/pyams_thesaurus/tests/
--rw-rw-rw-   0 root         (0) root         (0)      804 2023-04-13 12:50:45.000000 pyams_thesaurus-1.3.4/src/pyams_thesaurus/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1833 2023-04-13 12:50:45.000000 pyams_thesaurus-1.3.4/src/pyams_thesaurus/tests/test_utilsdocs.py
--rw-rw-rw-   0 root         (0) root         (0)     1870 2023-04-13 12:50:45.000000 pyams_thesaurus-1.3.4/src/pyams_thesaurus/tests/test_utilsdocstrings.py
--rw-rw-rw-   0 root         (0) root         (0)    21783 2023-04-13 12:50:45.000000 pyams_thesaurus-1.3.4/src/pyams_thesaurus/thesaurus.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 12:51:07.000000 pyams_thesaurus-1.3.4/src/pyams_thesaurus/zmi/
--rw-rw-rw-   0 root         (0) root         (0)     7876 2023-04-13 12:50:45.000000 pyams_thesaurus-1.3.4/src/pyams_thesaurus/zmi/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1460 2023-04-13 12:50:45.000000 pyams_thesaurus-1.3.4/src/pyams_thesaurus/zmi/extension.py
--rw-rw-rw-   0 root         (0) root         (0)    15093 2023-04-13 12:50:45.000000 pyams_thesaurus-1.3.4/src/pyams_thesaurus/zmi/extract.py
--rw-rw-rw-   0 root         (0) root         (0)     1901 2023-04-13 12:50:45.000000 pyams_thesaurus-1.3.4/src/pyams_thesaurus/zmi/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 12:51:07.000000 pyams_thesaurus-1.3.4/src/pyams_thesaurus/zmi/resources/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 12:51:07.000000 pyams_thesaurus-1.3.4/src/pyams_thesaurus/zmi/resources/css/
--rw-rw-rw-   0 root         (0) root         (0)      425 2023-04-13 12:50:45.000000 pyams_thesaurus-1.3.4/src/pyams_thesaurus/zmi/resources/css/thesaurus.css
--rw-rw-rw-   0 root         (0) root         (0)      351 2023-04-13 12:50:45.000000 pyams_thesaurus-1.3.4/src/pyams_thesaurus/zmi/resources/css/thesaurus.min.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 12:51:07.000000 pyams_thesaurus-1.3.4/src/pyams_thesaurus/zmi/resources/js/
--rw-rw-rw-   0 root         (0) root         (0)    16738 2023-04-13 12:50:45.000000 pyams_thesaurus-1.3.4/src/pyams_thesaurus/zmi/resources/js/thesaurus.js
--rw-rw-rw-   0 root         (0) root         (0)     7147 2023-04-13 12:50:45.000000 pyams_thesaurus-1.3.4/src/pyams_thesaurus/zmi/resources/js/thesaurus.min.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 12:51:07.000000 pyams_thesaurus-1.3.4/src/pyams_thesaurus/zmi/resources/sass/
--rw-rw-rw-   0 root         (0) root         (0)      453 2023-04-13 12:50:45.000000 pyams_thesaurus-1.3.4/src/pyams_thesaurus/zmi/resources/sass/thesaurus.scss
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 12:51:07.000000 pyams_thesaurus-1.3.4/src/pyams_thesaurus/zmi/templates/
--rw-rw-rw-   0 root         (0) root         (0)      643 2023-04-13 12:50:45.000000 pyams_thesaurus-1.3.4/src/pyams_thesaurus/zmi/templates/extract-terms.pt
--rw-rw-rw-   0 root         (0) root         (0)     2263 2023-04-13 12:50:45.000000 pyams_thesaurus-1.3.4/src/pyams_thesaurus/zmi/templates/terms-tree.pt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 12:51:07.000000 pyams_thesaurus-1.3.4/src/pyams_thesaurus/zmi/templates/widget/
--rw-rw-rw-   0 root         (0) root         (0)     2308 2023-04-13 12:50:45.000000 pyams_thesaurus-1.3.4/src/pyams_thesaurus/zmi/templates/widget/terms-tree-input.pt
--rw-rw-rw-   0 root         (0) root         (0)    13424 2023-04-13 12:50:45.000000 pyams_thesaurus-1.3.4/src/pyams_thesaurus/zmi/term.py
--rw-rw-rw-   0 root         (0) root         (0)     3798 2023-04-13 12:50:45.000000 pyams_thesaurus-1.3.4/src/pyams_thesaurus/zmi/test.py
--rw-rw-rw-   0 root         (0) root         (0)     8168 2023-04-13 12:50:45.000000 pyams_thesaurus-1.3.4/src/pyams_thesaurus/zmi/thesaurus.py
--rw-rw-rw-   0 root         (0) root         (0)    13892 2023-04-13 12:50:45.000000 pyams_thesaurus-1.3.4/src/pyams_thesaurus/zmi/tree.py
--rw-rw-rw-   0 root         (0) root         (0)     9096 2023-04-13 12:50:45.000000 pyams_thesaurus-1.3.4/src/pyams_thesaurus/zmi/widget.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 12:51:07.000000 pyams_thesaurus-1.3.4/src/pyams_thesaurus.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3083 2023-04-13 12:51:07.000000 pyams_thesaurus-1.3.4/src/pyams_thesaurus.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2518 2023-04-13 12:51:07.000000 pyams_thesaurus-1.3.4/src/pyams_thesaurus.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-13 12:51:07.000000 pyams_thesaurus-1.3.4/src/pyams_thesaurus.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       69 2023-04-13 12:51:07.000000 pyams_thesaurus-1.3.4/src/pyams_thesaurus.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-13 12:51:07.000000 pyams_thesaurus-1.3.4/src/pyams_thesaurus.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-13 12:51:07.000000 pyams_thesaurus-1.3.4/src/pyams_thesaurus.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      345 2023-04-13 12:51:07.000000 pyams_thesaurus-1.3.4/src/pyams_thesaurus.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2023-04-13 12:51:07.000000 pyams_thesaurus-1.3.4/src/pyams_thesaurus.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 22:13:54.000000 pyams_thesaurus-1.3.5/
+-rw-rw-rw-   0 root         (0) root         (0)     2191 2023-07-07 22:13:36.000000 pyams_thesaurus-1.3.5/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      104 2023-07-07 22:13:36.000000 pyams_thesaurus-1.3.5/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     3215 2023-07-07 22:13:54.000000 pyams_thesaurus-1.3.5/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 22:13:54.000000 pyams_thesaurus-1.3.5/docs/
+-rwxrwxrwx   0 root         (0) root         (0)     1429 2023-07-07 22:13:36.000000 pyams_thesaurus-1.3.5/docs/HISTORY.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1233 2023-07-07 22:13:36.000000 pyams_thesaurus-1.3.5/docs/README.rst
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-07 22:13:54.000000 pyams_thesaurus-1.3.5/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     2876 2023-07-07 22:13:36.000000 pyams_thesaurus-1.3.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 22:13:54.000000 pyams_thesaurus-1.3.5/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 22:13:54.000000 pyams_thesaurus-1.3.5/src/pyams_thesaurus/
+-rw-rw-rw-   0 root         (0) root         (0)      873 2023-07-07 22:13:36.000000 pyams_thesaurus-1.3.5/src/pyams_thesaurus/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 22:13:54.000000 pyams_thesaurus-1.3.5/src/pyams_thesaurus/api/
+-rw-rw-rw-   0 root         (0) root         (0)     1717 2023-07-07 22:13:36.000000 pyams_thesaurus-1.3.5/src/pyams_thesaurus/api/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7525 2023-07-07 22:13:36.000000 pyams_thesaurus-1.3.5/src/pyams_thesaurus/api/rest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 22:13:54.000000 pyams_thesaurus-1.3.5/src/pyams_thesaurus/doctests/
+-rw-rw-rw-   0 root         (0) root         (0)    20142 2023-07-07 22:13:36.000000 pyams_thesaurus-1.3.5/src/pyams_thesaurus/doctests/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 22:13:54.000000 pyams_thesaurus-1.3.5/src/pyams_thesaurus/doctests/data/
+-rw-rw-rw-   0 root         (0) root         (0)  2939491 2023-07-07 22:13:36.000000 pyams_thesaurus-1.3.5/src/pyams_thesaurus/doctests/data/SAMPLE-SKOS.xml
+-rw-rw-rw-   0 root         (0) root         (0)  2735784 2023-07-07 22:13:36.000000 pyams_thesaurus-1.3.5/src/pyams_thesaurus/doctests/data/SAMPLE-Superdoc.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 22:13:54.000000 pyams_thesaurus-1.3.5/src/pyams_thesaurus/extension/
+-rw-rw-rw-   0 root         (0) root         (0)      550 2023-07-07 22:13:36.000000 pyams_thesaurus-1.3.5/src/pyams_thesaurus/extension/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 22:13:54.000000 pyams_thesaurus-1.3.5/src/pyams_thesaurus/extension/html/
+-rw-rw-rw-   0 root         (0) root         (0)     2049 2023-07-07 22:13:36.000000 pyams_thesaurus-1.3.5/src/pyams_thesaurus/extension/html/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1217 2023-07-07 22:13:36.000000 pyams_thesaurus-1.3.5/src/pyams_thesaurus/extension/html/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 22:13:54.000000 pyams_thesaurus-1.3.5/src/pyams_thesaurus/extension/html/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)     1535 2023-07-07 22:13:36.000000 pyams_thesaurus-1.3.5/src/pyams_thesaurus/extension/html/zmi/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 22:13:54.000000 pyams_thesaurus-1.3.5/src/pyams_thesaurus/generations/
+-rw-rw-rw-   0 root         (0) root         (0)     1380 2023-07-07 22:13:36.000000 pyams_thesaurus-1.3.5/src/pyams_thesaurus/generations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4274 2023-07-07 22:13:36.000000 pyams_thesaurus-1.3.5/src/pyams_thesaurus/include.py
+-rw-rw-rw-   0 root         (0) root         (0)     4277 2023-07-07 22:13:36.000000 pyams_thesaurus-1.3.5/src/pyams_thesaurus/index.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 22:13:54.000000 pyams_thesaurus-1.3.5/src/pyams_thesaurus/interfaces/
+-rw-rw-rw-   0 root         (0) root         (0)     1862 2023-07-07 22:13:36.000000 pyams_thesaurus-1.3.5/src/pyams_thesaurus/interfaces/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1632 2023-07-07 22:13:36.000000 pyams_thesaurus-1.3.5/src/pyams_thesaurus/interfaces/extension.py
+-rw-rw-rw-   0 root         (0) root         (0)     1317 2023-07-07 22:13:36.000000 pyams_thesaurus-1.3.5/src/pyams_thesaurus/interfaces/index.py
+-rw-rw-rw-   0 root         (0) root         (0)     5471 2023-07-07 22:13:36.000000 pyams_thesaurus-1.3.5/src/pyams_thesaurus/interfaces/loader.py
+-rw-rw-rw-   0 root         (0) root         (0)     7494 2023-07-07 22:13:36.000000 pyams_thesaurus-1.3.5/src/pyams_thesaurus/interfaces/term.py
+-rw-rw-rw-   0 root         (0) root         (0)     8247 2023-07-07 22:13:36.000000 pyams_thesaurus-1.3.5/src/pyams_thesaurus/interfaces/thesaurus.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 22:13:54.000000 pyams_thesaurus-1.3.5/src/pyams_thesaurus/loader/
+-rw-rw-rw-   0 root         (0) root         (0)    10069 2023-07-07 22:13:36.000000 pyams_thesaurus-1.3.5/src/pyams_thesaurus/loader/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2844 2023-07-07 22:13:36.000000 pyams_thesaurus-1.3.5/src/pyams_thesaurus/loader/config.py
+-rw-rw-rw-   0 root         (0) root         (0)    10638 2023-07-07 22:13:36.000000 pyams_thesaurus-1.3.5/src/pyams_thesaurus/loader/skos.py
+-rw-rw-rw-   0 root         (0) root         (0)     8442 2023-07-07 22:13:36.000000 pyams_thesaurus-1.3.5/src/pyams_thesaurus/loader/superdoc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 22:13:54.000000 pyams_thesaurus-1.3.5/src/pyams_thesaurus/locales/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 22:13:54.000000 pyams_thesaurus-1.3.5/src/pyams_thesaurus/locales/fr/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 22:13:54.000000 pyams_thesaurus-1.3.5/src/pyams_thesaurus/locales/fr/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)    13065 2023-07-07 22:13:36.000000 pyams_thesaurus-1.3.5/src/pyams_thesaurus/locales/fr/LC_MESSAGES/pyams_thesaurus.mo
+-rw-rw-rw-   0 root         (0) root         (0)    21065 2023-07-07 22:13:36.000000 pyams_thesaurus-1.3.5/src/pyams_thesaurus/locales/fr/LC_MESSAGES/pyams_thesaurus.po
+-rw-rw-rw-   0 root         (0) root         (0)    15976 2023-07-07 22:13:36.000000 pyams_thesaurus-1.3.5/src/pyams_thesaurus/locales/pyams_thesaurus.pot
+-rw-rw-rw-   0 root         (0) root         (0)     1042 2023-07-07 22:13:36.000000 pyams_thesaurus-1.3.5/src/pyams_thesaurus/manager.py
+-rw-rw-rw-   0 root         (0) root         (0)     2727 2023-07-07 22:13:36.000000 pyams_thesaurus-1.3.5/src/pyams_thesaurus/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)    19509 2023-07-07 22:13:36.000000 pyams_thesaurus-1.3.5/src/pyams_thesaurus/term.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 22:13:54.000000 pyams_thesaurus-1.3.5/src/pyams_thesaurus/tests/
+-rw-rw-rw-   0 root         (0) root         (0)      804 2023-07-07 22:13:36.000000 pyams_thesaurus-1.3.5/src/pyams_thesaurus/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1833 2023-07-07 22:13:36.000000 pyams_thesaurus-1.3.5/src/pyams_thesaurus/tests/test_utilsdocs.py
+-rw-rw-rw-   0 root         (0) root         (0)     1870 2023-07-07 22:13:36.000000 pyams_thesaurus-1.3.5/src/pyams_thesaurus/tests/test_utilsdocstrings.py
+-rw-rw-rw-   0 root         (0) root         (0)    21904 2023-07-07 22:13:36.000000 pyams_thesaurus-1.3.5/src/pyams_thesaurus/thesaurus.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 22:13:54.000000 pyams_thesaurus-1.3.5/src/pyams_thesaurus/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)     7876 2023-07-07 22:13:36.000000 pyams_thesaurus-1.3.5/src/pyams_thesaurus/zmi/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1460 2023-07-07 22:13:36.000000 pyams_thesaurus-1.3.5/src/pyams_thesaurus/zmi/extension.py
+-rw-rw-rw-   0 root         (0) root         (0)    15093 2023-07-07 22:13:36.000000 pyams_thesaurus-1.3.5/src/pyams_thesaurus/zmi/extract.py
+-rw-rw-rw-   0 root         (0) root         (0)     1901 2023-07-07 22:13:36.000000 pyams_thesaurus-1.3.5/src/pyams_thesaurus/zmi/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 22:13:54.000000 pyams_thesaurus-1.3.5/src/pyams_thesaurus/zmi/resources/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 22:13:54.000000 pyams_thesaurus-1.3.5/src/pyams_thesaurus/zmi/resources/css/
+-rw-rw-rw-   0 root         (0) root         (0)      425 2023-07-07 22:13:36.000000 pyams_thesaurus-1.3.5/src/pyams_thesaurus/zmi/resources/css/thesaurus.css
+-rw-rw-rw-   0 root         (0) root         (0)      351 2023-07-07 22:13:36.000000 pyams_thesaurus-1.3.5/src/pyams_thesaurus/zmi/resources/css/thesaurus.min.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 22:13:54.000000 pyams_thesaurus-1.3.5/src/pyams_thesaurus/zmi/resources/js/
+-rw-rw-rw-   0 root         (0) root         (0)    16738 2023-07-07 22:13:36.000000 pyams_thesaurus-1.3.5/src/pyams_thesaurus/zmi/resources/js/thesaurus.js
+-rw-rw-rw-   0 root         (0) root         (0)     7147 2023-07-07 22:13:36.000000 pyams_thesaurus-1.3.5/src/pyams_thesaurus/zmi/resources/js/thesaurus.min.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 22:13:54.000000 pyams_thesaurus-1.3.5/src/pyams_thesaurus/zmi/resources/sass/
+-rw-rw-rw-   0 root         (0) root         (0)      453 2023-07-07 22:13:36.000000 pyams_thesaurus-1.3.5/src/pyams_thesaurus/zmi/resources/sass/thesaurus.scss
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 22:13:54.000000 pyams_thesaurus-1.3.5/src/pyams_thesaurus/zmi/templates/
+-rw-rw-rw-   0 root         (0) root         (0)      643 2023-07-07 22:13:36.000000 pyams_thesaurus-1.3.5/src/pyams_thesaurus/zmi/templates/extract-terms.pt
+-rw-rw-rw-   0 root         (0) root         (0)     2263 2023-07-07 22:13:36.000000 pyams_thesaurus-1.3.5/src/pyams_thesaurus/zmi/templates/terms-tree.pt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 22:13:54.000000 pyams_thesaurus-1.3.5/src/pyams_thesaurus/zmi/templates/widget/
+-rw-rw-rw-   0 root         (0) root         (0)     2308 2023-07-07 22:13:36.000000 pyams_thesaurus-1.3.5/src/pyams_thesaurus/zmi/templates/widget/terms-tree-input.pt
+-rw-rw-rw-   0 root         (0) root         (0)    13424 2023-07-07 22:13:36.000000 pyams_thesaurus-1.3.5/src/pyams_thesaurus/zmi/term.py
+-rw-rw-rw-   0 root         (0) root         (0)     3798 2023-07-07 22:13:36.000000 pyams_thesaurus-1.3.5/src/pyams_thesaurus/zmi/test.py
+-rw-rw-rw-   0 root         (0) root         (0)     8168 2023-07-07 22:13:36.000000 pyams_thesaurus-1.3.5/src/pyams_thesaurus/zmi/thesaurus.py
+-rw-rw-rw-   0 root         (0) root         (0)    13907 2023-07-07 22:13:36.000000 pyams_thesaurus-1.3.5/src/pyams_thesaurus/zmi/tree.py
+-rw-rw-rw-   0 root         (0) root         (0)     9096 2023-07-07 22:13:36.000000 pyams_thesaurus-1.3.5/src/pyams_thesaurus/zmi/widget.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 22:13:54.000000 pyams_thesaurus-1.3.5/src/pyams_thesaurus.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3215 2023-07-07 22:13:54.000000 pyams_thesaurus-1.3.5/src/pyams_thesaurus.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2518 2023-07-07 22:13:54.000000 pyams_thesaurus-1.3.5/src/pyams_thesaurus.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-07 22:13:54.000000 pyams_thesaurus-1.3.5/src/pyams_thesaurus.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       69 2023-07-07 22:13:54.000000 pyams_thesaurus-1.3.5/src/pyams_thesaurus.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-07 22:13:54.000000 pyams_thesaurus-1.3.5/src/pyams_thesaurus.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-07 22:13:54.000000 pyams_thesaurus-1.3.5/src/pyams_thesaurus.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      345 2023-07-07 22:13:54.000000 pyams_thesaurus-1.3.5/src/pyams_thesaurus.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2023-07-07 22:13:54.000000 pyams_thesaurus-1.3.5/src/pyams_thesaurus.egg-info/top_level.txt
```

### Comparing `pyams_thesaurus-1.3.4/LICENSE` & `pyams_thesaurus-1.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pyams_thesaurus-1.3.4/PKG-INFO` & `pyams_thesaurus-1.3.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyams_thesaurus
-Version: 1.3.4
+Version: 1.3.5
 Summary: PyAMS thesaurus management package
 Home-page: https://pyams.readthedocs.io
 Author: Thierry Florac
 Author-email: tflorac@ulthar.net
 License: ZPL
 Keywords: Pyramid PyAMS
 Platform: UNKNOWN
@@ -49,14 +49,20 @@
 Thesaurus terms can be entered manually, but also loaded from external sources like XML files
 using SKOS/RDF namespace.
 
 
 Changelog
 =========
 
+1.3.5
+-----
+ - updated API usage permission
+ - updated context actions viewlet manager name
+ - added thesaurus names title factory
+
 1.3.4
 -----
  - updated Colander API schemas for better OpenAPI specifications
 
 1.3.3
 -----
  - version mismatch
```

### Comparing `pyams_thesaurus-1.3.4/docs/HISTORY.rst` & `pyams_thesaurus-1.3.5/docs/HISTORY.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,16 @@
 Changelog
 =========
 
+1.3.5
+-----
+ - updated API usage permission
+ - updated context actions viewlet manager name
+ - added thesaurus names title factory
+
 1.3.4
 -----
  - updated Colander API schemas for better OpenAPI specifications
 
 1.3.3
 -----
  - version mismatch
```

### Comparing `pyams_thesaurus-1.3.4/docs/README.rst` & `pyams_thesaurus-1.3.5/docs/README.rst`

 * *Files identical despite different names*

### Comparing `pyams_thesaurus-1.3.4/setup.py` & `pyams_thesaurus-1.3.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 DOCS = os.path.join(os.path.dirname(__file__),
                     'docs')
 
 README = os.path.join(DOCS, 'README.rst')
 HISTORY = os.path.join(DOCS, 'HISTORY.rst')
 
-version = '1.3.4'
+version = '1.3.5'
 long_description = open(README).read() + '\n\n' + open(HISTORY).read()
 
 tests_require = [
     'pyams_zmi',
     'pyramid_zcml',
     'zope.exceptions'
 ]
```

### Comparing `pyams_thesaurus-1.3.4/src/pyams_thesaurus/__init__.py` & `pyams_thesaurus-1.3.5/src/pyams_thesaurus/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_thesaurus-1.3.4/src/pyams_thesaurus/api/__init__.py` & `pyams_thesaurus-1.3.5/src/pyams_thesaurus/api/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_thesaurus-1.3.4/src/pyams_thesaurus/api/rest.py` & `pyams_thesaurus-1.3.5/src/pyams_thesaurus/api/rest.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,24 +19,24 @@
 
 from colander import MappingSchema, SchemaNode, SequenceSchema, String, drop
 from cornice import Service
 from cornice.validators import colander_validator
 from hypatia.text import ParseError
 from pyramid.httpexceptions import HTTPBadRequest, HTTPOk
 
-from pyams_security.interfaces.base import VIEW_SYSTEM_PERMISSION
+from pyams_security.interfaces.base import USE_INTERNAL_API_PERMISSION
 from pyams_security.rest import check_cors_origin, set_cors_headers
 from pyams_thesaurus.interfaces import REST_EXTRACTS_GETTER_ROUTE, REST_TERMS_SEARCH_ROUTE
 from pyams_thesaurus.interfaces.term import STATUS_ARCHIVED
 from pyams_thesaurus.interfaces.thesaurus import IThesaurus, IThesaurusExtracts
+from pyams_utils.interfaces.form import NO_VALUE_STRING
 from pyams_utils.list import unique
 from pyams_utils.registry import query_utility
 from pyams_utils.rest import BaseResponseSchema, BaseStatusSchema, STATUS, http_error, rest_responses
 
-
 __docformat__ = 'restructuredtext'
 
 
 TEST_MODE = sys.argv[-1].endswith('/test')
 
 
 #
@@ -90,24 +90,29 @@
 
 
 extracts_get_responses = rest_responses.copy()
 extracts_get_responses[HTTPOk.code] = ThesaurusExtractsResponse(
     description="Thesaurus extracts query response")
 
 
-@extracts_service.get(permission=VIEW_SYSTEM_PERMISSION,
+@extracts_service.get(permission=USE_INTERNAL_API_PERMISSION,
                       schema=ThesaurusExtractsRequest(),
                       validators=(check_cors_origin, colander_validator, set_cors_headers),
                       response_schemas=extracts_get_responses)
 def get_extracts(request):
     """Get thesaurus extracts list"""
     params = request.params if TEST_MODE else request.validated.get('querystring', {})
     thesaurus_name = params.get('thesaurus_name')
     if not thesaurus_name:
         return http_error(request, HTTPBadRequest, 'missing argument')
+    if thesaurus_name == NO_VALUE_STRING:
+        return {
+            'status': STATUS.SUCCESS.value,
+            'results': []
+        }
     thesaurus = query_utility(IThesaurus, name=thesaurus_name)
     if thesaurus is None:
         return http_error(request, HTTPBadRequest, 'bad thesaurus name')
     extracts = IThesaurusExtracts(thesaurus)
     return {
         'status': STATUS.SUCCESS.value,
         'results': [
@@ -176,15 +181,15 @@
 
 
 terms_get_responses = rest_responses.copy()
 terms_get_responses[HTTPOk.code] = ThesaurusTermsResponse(
     description="List of terms matching given query")
 
 
-@terms_service.get(permission=VIEW_SYSTEM_PERMISSION,
+@terms_service.get(permission=USE_INTERNAL_API_PERMISSION,
                    schema=ThesaurusTermsRequest(),
                    validators=(check_cors_origin, colander_validator, set_cors_headers),
                    response_schemas=terms_get_responses)
 def get_terms(request):
     """Returns list of terms matching given query"""
     params = request.params if TEST_MODE else request.validated.get('querystring', {})
     thesaurus_name = params.get('thesaurus_name')
```

### Comparing `pyams_thesaurus-1.3.4/src/pyams_thesaurus/doctests/README.rst` & `pyams_thesaurus-1.3.5/src/pyams_thesaurus/doctests/README.rst`

 * *Files identical despite different names*

### Comparing `pyams_thesaurus-1.3.4/src/pyams_thesaurus/doctests/data/SAMPLE-SKOS.xml` & `pyams_thesaurus-1.3.5/src/pyams_thesaurus/doctests/data/SAMPLE-SKOS.xml`

 * *Files identical despite different names*

### Comparing `pyams_thesaurus-1.3.4/src/pyams_thesaurus/doctests/data/SAMPLE-Superdoc.xml` & `pyams_thesaurus-1.3.5/src/pyams_thesaurus/doctests/data/SAMPLE-Superdoc.xml`

 * *Files identical despite different names*

### Comparing `pyams_thesaurus-1.3.4/src/pyams_thesaurus/extension/__init__.py` & `pyams_thesaurus-1.3.5/src/pyams_thesaurus/extension/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_thesaurus-1.3.4/src/pyams_thesaurus/extension/html/__init__.py` & `pyams_thesaurus-1.3.5/src/pyams_thesaurus/extension/html/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_thesaurus-1.3.4/src/pyams_thesaurus/extension/html/interfaces.py` & `pyams_thesaurus-1.3.5/src/pyams_thesaurus/extension/html/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_thesaurus-1.3.4/src/pyams_thesaurus/extension/html/zmi/__init__.py` & `pyams_thesaurus-1.3.5/src/pyams_thesaurus/extension/html/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_thesaurus-1.3.4/src/pyams_thesaurus/generations/__init__.py` & `pyams_thesaurus-1.3.5/src/pyams_thesaurus/generations/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_thesaurus-1.3.4/src/pyams_thesaurus/include.py` & `pyams_thesaurus-1.3.5/src/pyams_thesaurus/include.py`

 * *Files identical despite different names*

### Comparing `pyams_thesaurus-1.3.4/src/pyams_thesaurus/index.py` & `pyams_thesaurus-1.3.5/src/pyams_thesaurus/index.py`

 * *Files identical despite different names*

### Comparing `pyams_thesaurus-1.3.4/src/pyams_thesaurus/interfaces/__init__.py` & `pyams_thesaurus-1.3.5/src/pyams_thesaurus/interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_thesaurus-1.3.4/src/pyams_thesaurus/interfaces/extension.py` & `pyams_thesaurus-1.3.5/src/pyams_thesaurus/interfaces/extension.py`

 * *Files identical despite different names*

### Comparing `pyams_thesaurus-1.3.4/src/pyams_thesaurus/interfaces/index.py` & `pyams_thesaurus-1.3.5/src/pyams_thesaurus/interfaces/index.py`

 * *Files identical despite different names*

### Comparing `pyams_thesaurus-1.3.4/src/pyams_thesaurus/interfaces/loader.py` & `pyams_thesaurus-1.3.5/src/pyams_thesaurus/interfaces/loader.py`

 * *Files identical despite different names*

### Comparing `pyams_thesaurus-1.3.4/src/pyams_thesaurus/interfaces/term.py` & `pyams_thesaurus-1.3.5/src/pyams_thesaurus/interfaces/term.py`

 * *Files identical despite different names*

### Comparing `pyams_thesaurus-1.3.4/src/pyams_thesaurus/interfaces/thesaurus.py` & `pyams_thesaurus-1.3.5/src/pyams_thesaurus/interfaces/thesaurus.py`

 * *Files identical despite different names*

### Comparing `pyams_thesaurus-1.3.4/src/pyams_thesaurus/loader/__init__.py` & `pyams_thesaurus-1.3.5/src/pyams_thesaurus/loader/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_thesaurus-1.3.4/src/pyams_thesaurus/loader/config.py` & `pyams_thesaurus-1.3.5/src/pyams_thesaurus/loader/config.py`

 * *Files identical despite different names*

### Comparing `pyams_thesaurus-1.3.4/src/pyams_thesaurus/loader/skos.py` & `pyams_thesaurus-1.3.5/src/pyams_thesaurus/loader/skos.py`

 * *Files identical despite different names*

### Comparing `pyams_thesaurus-1.3.4/src/pyams_thesaurus/loader/superdoc.py` & `pyams_thesaurus-1.3.5/src/pyams_thesaurus/loader/superdoc.py`

 * *Files identical despite different names*

### Comparing `pyams_thesaurus-1.3.4/src/pyams_thesaurus/locales/fr/LC_MESSAGES/pyams_thesaurus.mo` & `pyams_thesaurus-1.3.5/src/pyams_thesaurus/locales/fr/LC_MESSAGES/pyams_thesaurus.mo`

 * *Files identical despite different names*

### Comparing `pyams_thesaurus-1.3.4/src/pyams_thesaurus/locales/fr/LC_MESSAGES/pyams_thesaurus.po` & `pyams_thesaurus-1.3.5/src/pyams_thesaurus/locales/fr/LC_MESSAGES/pyams_thesaurus.po`

 * *Files identical despite different names*

### Comparing `pyams_thesaurus-1.3.4/src/pyams_thesaurus/locales/pyams_thesaurus.pot` & `pyams_thesaurus-1.3.5/src/pyams_thesaurus/locales/pyams_thesaurus.pot`

 * *Files identical despite different names*

### Comparing `pyams_thesaurus-1.3.4/src/pyams_thesaurus/manager.py` & `pyams_thesaurus-1.3.5/src/pyams_thesaurus/manager.py`

 * *Files identical despite different names*

### Comparing `pyams_thesaurus-1.3.4/src/pyams_thesaurus/schema.py` & `pyams_thesaurus-1.3.5/src/pyams_thesaurus/schema.py`

 * *Files identical despite different names*

### Comparing `pyams_thesaurus-1.3.4/src/pyams_thesaurus/term.py` & `pyams_thesaurus-1.3.5/src/pyams_thesaurus/term.py`

 * *Files identical despite different names*

### Comparing `pyams_thesaurus-1.3.4/src/pyams_thesaurus/tests/__init__.py` & `pyams_thesaurus-1.3.5/src/pyams_thesaurus/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_thesaurus-1.3.4/src/pyams_thesaurus/tests/test_utilsdocs.py` & `pyams_thesaurus-1.3.5/src/pyams_thesaurus/tests/test_utilsdocs.py`

 * *Files identical despite different names*

### Comparing `pyams_thesaurus-1.3.4/src/pyams_thesaurus/tests/test_utilsdocstrings.py` & `pyams_thesaurus-1.3.5/src/pyams_thesaurus/tests/test_utilsdocstrings.py`

 * *Files identical despite different names*

### Comparing `pyams_thesaurus-1.3.4/src/pyams_thesaurus/thesaurus.py` & `pyams_thesaurus-1.3.5/src/pyams_thesaurus/thesaurus.py`

 * *Files 0% similar despite different names*

```diff
@@ -533,14 +533,19 @@
 
 @vocabulary_config(name=THESAURUS_NAMES_VOCABULARY)
 class ThesaurusNamesVocabulary(LocalUtilitiesVocabulary):
     """Thesaurus names utilities vocabulary"""
 
     interface = IThesaurus
 
+    @staticmethod
+    def title_factory(thesaurus):
+        """Thesaurus title getter"""
+        return thesaurus.title
+
 
 @vocabulary_config(name=THESAURUS_EXTRACTS_VOCABULARY)
 class ThesaurusExtractsVocabulary(SimpleVocabulary):
     """Thesaurus extracts vocabulary"""
 
     def __init__(self, context=None):
         terms = []
```

### Comparing `pyams_thesaurus-1.3.4/src/pyams_thesaurus/zmi/__init__.py` & `pyams_thesaurus-1.3.5/src/pyams_thesaurus/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_thesaurus-1.3.4/src/pyams_thesaurus/zmi/extension.py` & `pyams_thesaurus-1.3.5/src/pyams_thesaurus/zmi/extension.py`

 * *Files identical despite different names*

### Comparing `pyams_thesaurus-1.3.4/src/pyams_thesaurus/zmi/extract.py` & `pyams_thesaurus-1.3.5/src/pyams_thesaurus/zmi/extract.py`

 * *Files identical despite different names*

### Comparing `pyams_thesaurus-1.3.4/src/pyams_thesaurus/zmi/interfaces.py` & `pyams_thesaurus-1.3.5/src/pyams_thesaurus/zmi/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_thesaurus-1.3.4/src/pyams_thesaurus/zmi/resources/js/thesaurus.js` & `pyams_thesaurus-1.3.5/src/pyams_thesaurus/zmi/resources/js/thesaurus.js`

 * *Files identical despite different names*

### Comparing `pyams_thesaurus-1.3.4/src/pyams_thesaurus/zmi/resources/js/thesaurus.min.js` & `pyams_thesaurus-1.3.5/src/pyams_thesaurus/zmi/resources/js/thesaurus.min.js`

 * *Files identical despite different names*

### Comparing `pyams_thesaurus-1.3.4/src/pyams_thesaurus/zmi/templates/extract-terms.pt` & `pyams_thesaurus-1.3.5/src/pyams_thesaurus/zmi/templates/extract-terms.pt`

 * *Files identical despite different names*

### Comparing `pyams_thesaurus-1.3.4/src/pyams_thesaurus/zmi/templates/terms-tree.pt` & `pyams_thesaurus-1.3.5/src/pyams_thesaurus/zmi/templates/terms-tree.pt`

 * *Files identical despite different names*

### Comparing `pyams_thesaurus-1.3.4/src/pyams_thesaurus/zmi/templates/widget/terms-tree-input.pt` & `pyams_thesaurus-1.3.5/src/pyams_thesaurus/zmi/templates/widget/terms-tree-input.pt`

 * *Files identical despite different names*

### Comparing `pyams_thesaurus-1.3.4/src/pyams_thesaurus/zmi/term.py` & `pyams_thesaurus-1.3.5/src/pyams_thesaurus/zmi/term.py`

 * *Files identical despite different names*

### Comparing `pyams_thesaurus-1.3.4/src/pyams_thesaurus/zmi/test.py` & `pyams_thesaurus-1.3.5/src/pyams_thesaurus/zmi/test.py`

 * *Files identical despite different names*

### Comparing `pyams_thesaurus-1.3.4/src/pyams_thesaurus/zmi/thesaurus.py` & `pyams_thesaurus-1.3.5/src/pyams_thesaurus/zmi/thesaurus.py`

 * *Files identical despite different names*

### Comparing `pyams_thesaurus-1.3.4/src/pyams_thesaurus/zmi/tree.py` & `pyams_thesaurus-1.3.5/src/pyams_thesaurus/zmi/tree.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,15 +46,15 @@
 from pyams_utils.interfaces.tree import INode, ITree
 from pyams_utils.registry import get_utility, query_utility
 from pyams_utils.url import absolute_url
 from pyams_viewlet.manager import viewletmanager_config
 from pyams_viewlet.viewlet import ViewContentProvider, viewlet_config
 from pyams_zmi.form import AdminModalAddForm
 from pyams_zmi.interfaces import IAdminLayer, ICompositeView
-from pyams_zmi.interfaces.viewlet import IActionsViewletManager, IContentManagementMenu
+from pyams_zmi.interfaces.viewlet import IContextActionsDropdownMenu, IContentManagementMenu
 from pyams_zmi.view import CompositeAdminView
 from pyams_zmi.zmi.viewlet.menu import NavigationMenuItem
 
 
 __docformat__ = 'restructuredtext'
 
 from pyams_thesaurus import _  # pylint: disable=ungrouped-imports
@@ -226,15 +226,15 @@
 
 #
 # Import menu
 #
 
 @viewlet_config(name='import-terms.action',
                 context=IThesaurus, layer=IAdminLayer, view=ThesaurusTermsTreeView,
-                manager=IActionsViewletManager, weight=10,
+                manager=IContextActionsDropdownMenu, weight=10,
                 permission=MANAGE_THESAURUS_CONTENT_PERMISSION)
 class ThesaurusImportAction(MenuItem):
     """Thesaurus import action"""
 
     label = _("Import terms")
     icon_class = 'fas fa-upload'
 
@@ -315,15 +315,15 @@
 
 #
 # Thesaurus export form
 #
 
 @viewlet_config(name='export-terms.action',
                 context=IThesaurus, layer=IAdminLayer, view=ThesaurusTermsTreeView,
-                manager=IActionsViewletManager, weight=20,
+                manager=IContextActionsDropdownMenu, weight=20,
                 permission=MANAGE_THESAURUS_CONTENT_PERMISSION)
 class ThesaurusExportAction(MenuItem):
     """Thesaurus export action"""
 
     label = _("Export terms")
     icon_class = 'fas fa-download'
```

### Comparing `pyams_thesaurus-1.3.4/src/pyams_thesaurus/zmi/widget.py` & `pyams_thesaurus-1.3.5/src/pyams_thesaurus/zmi/widget.py`

 * *Files identical despite different names*

### Comparing `pyams_thesaurus-1.3.4/src/pyams_thesaurus.egg-info/PKG-INFO` & `pyams_thesaurus-1.3.5/src/pyams_thesaurus.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyams-thesaurus
-Version: 1.3.4
+Version: 1.3.5
 Summary: PyAMS thesaurus management package
 Home-page: https://pyams.readthedocs.io
 Author: Thierry Florac
 Author-email: tflorac@ulthar.net
 License: ZPL
 Keywords: Pyramid PyAMS
 Platform: UNKNOWN
@@ -49,14 +49,20 @@
 Thesaurus terms can be entered manually, but also loaded from external sources like XML files
 using SKOS/RDF namespace.
 
 
 Changelog
 =========
 
+1.3.5
+-----
+ - updated API usage permission
+ - updated context actions viewlet manager name
+ - added thesaurus names title factory
+
 1.3.4
 -----
  - updated Colander API schemas for better OpenAPI specifications
 
 1.3.3
 -----
  - version mismatch
```

### Comparing `pyams_thesaurus-1.3.4/src/pyams_thesaurus.egg-info/SOURCES.txt` & `pyams_thesaurus-1.3.5/src/pyams_thesaurus.egg-info/SOURCES.txt`

 * *Files identical despite different names*

