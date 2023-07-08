# Comparing `tmp/nics-2.7.1.tar.gz` & `tmp/nics-2.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/now-i-can-sleep/now-i-can-sleep/dist/.tmp-6r4vqhpq/nics-2.7.1.tar", last modified: Sat Jul  8 12:17:04 2023, max compression
+gzip compressed data, was "/home/runner/work/now-i-can-sleep/now-i-can-sleep/dist/.tmp-5ypn0xps/nics-2.7.2.tar", last modified: Sat Jul  8 14:19:50 2023, max compression
```

## Comparing `nics-2.7.1.tar` & `nics-2.7.2.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 12:17:04.000000 nics-2.7.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-07-08 12:16:56.000000 nics-2.7.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-08 12:16:56.000000 nics-2.7.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-07-08 12:17:04.000000 nics-2.7.1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 12:17:04.000000 nics-2.7.1/nics/
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-08 12:16:56.000000 nics-2.7.1/nics/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 12:17:04.000000 nics-2.7.1/nics/main/
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-07-08 12:16:56.000000 nics-2.7.1/nics/main/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 12:17:04.000000 nics-2.7.1/nics/main/_template/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 12:17:04.000000 nics-2.7.1/nics/main/_template/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-07-08 12:16:56.000000 nics-2.7.1/nics/main/_template/docs/404.md
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-07-08 12:16:56.000000 nics-2.7.1/nics/main/_template/docs/favicon.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 12:17:04.000000 nics-2.7.1/nics/main/_template/docs/tree/
--rw-r--r--   0 runner    (1001) docker     (123)        2 2023-07-08 12:16:56.000000 nics-2.7.1/nics/main/_template/docs/tree/1 - Page1.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 12:17:04.000000 nics-2.7.1/nics/main/_template/docs/tree/2 - Pages/
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-08 12:16:56.000000 nics-2.7.1/nics/main/_template/docs/tree/2 - Pages/baz.md
--rw-r--r--   0 runner    (1001) docker     (123)    25360 2023-07-08 12:16:56.000000 nics-2.7.1/nics/main/_template/docs/tree/2 - Pages/logo200.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 12:17:04.000000 nics-2.7.1/nics/main/_template/docs/tree/7 - FAQs/
--rw-r--r--   0 runner    (1001) docker     (123)        2 2023-07-08 12:16:56.000000 nics-2.7.1/nics/main/_template/docs/tree/7 - FAQs/1 - Question1.md
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-08 12:16:56.000000 nics-2.7.1/nics/main/_template/docs/tree/7 - FAQs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-08 12:16:56.000000 nics-2.7.1/nics/main/_template/docs/tree/8 - Changelog.md
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-08 12:16:56.000000 nics-2.7.1/nics/main/_template/docs/tree/9 - About.md
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-08 12:16:56.000000 nics-2.7.1/nics/main/_template/docs/tree/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 12:17:04.000000 nics-2.7.1/nics/main/_template/web/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 12:17:04.000000 nics-2.7.1/nics/main/_template/web/_layouts/
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-07-08 12:16:56.000000 nics-2.7.1/nics/main/_template/web/_layouts/main.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 12:17:04.000000 nics-2.7.1/nics/main/_template/web/_sass/
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-07-08 12:16:56.000000 nics-2.7.1/nics/main/_template/web/_sass/footer.scss
--rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-07-08 12:16:56.000000 nics-2.7.1/nics/main/_template/web/_sass/header.scss
--rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-07-08 12:16:56.000000 nics-2.7.1/nics/main/_template/web/_sass/main.scss
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 12:17:04.000000 nics-2.7.1/nics/main/_template/web/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-07-08 12:16:56.000000 nics-2.7.1/nics/main/_template/web/scripts/header.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 12:17:04.000000 nics-2.7.1/nics/main/compile/
--rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-07-08 12:16:56.000000 nics-2.7.1/nics/main/compile/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-07-08 12:16:56.000000 nics-2.7.1/nics/main/compile/copying_template.py
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-07-08 12:16:56.000000 nics-2.7.1/nics/main/compile/inspect.py
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-07-08 12:16:56.000000 nics-2.7.1/nics/main/compile/update_404_and_favicon.py
--rw-r--r--   0 runner    (1001) docker     (123)     4442 2023-07-08 12:16:56.000000 nics-2.7.1/nics/main/compile/update_docs_tree.py
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-07-08 12:16:56.000000 nics-2.7.1/nics/main/compile/update_footer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2268 2023-07-08 12:16:56.000000 nics-2.7.1/nics/main/compile/update_header.py
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-07-08 12:16:56.000000 nics-2.7.1/nics/main/compile/update_jekyll_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-07-08 12:16:56.000000 nics-2.7.1/nics/main/compile/update_sass_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-07-08 12:16:56.000000 nics-2.7.1/nics/main/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 12:17:04.000000 nics-2.7.1/nics/main/upgrade/
--rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-07-08 12:16:56.000000 nics-2.7.1/nics/main/upgrade/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 12:17:04.000000 nics-2.7.1/nics/main/wizard/
--rw-r--r--   0 runner    (1001) docker     (123)     3381 2023-07-08 12:16:56.000000 nics-2.7.1/nics/main/wizard/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-07-08 12:16:56.000000 nics-2.7.1/nics/main/wizard/settings_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-07-08 12:16:56.000000 nics-2.7.1/nics/main/wizard/workflow_writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 12:17:04.000000 nics-2.7.1/nics.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-07-08 12:17:04.000000 nics-2.7.1/nics.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-07-08 12:17:04.000000 nics-2.7.1/nics.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 12:17:04.000000 nics-2.7.1/nics.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-08 12:17:04.000000 nics-2.7.1/nics.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-08 12:17:04.000000 nics-2.7.1/nics.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-08 12:17:04.000000 nics-2.7.1/nics.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-07-08 12:16:57.000000 nics-2.7.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-07-08 12:16:56.000000 nics-2.7.1/readme.md
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-08 12:17:04.000000 nics-2.7.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-08 12:16:56.000000 nics-2.7.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:19:50.000000 nics-2.7.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-07-08 14:19:43.000000 nics-2.7.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-08 14:19:43.000000 nics-2.7.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-07-08 14:19:50.000000 nics-2.7.2/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:19:50.000000 nics-2.7.2/nics/
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-08 14:19:43.000000 nics-2.7.2/nics/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:19:50.000000 nics-2.7.2/nics/main/
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-07-08 14:19:43.000000 nics-2.7.2/nics/main/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:19:50.000000 nics-2.7.2/nics/main/_template/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:19:50.000000 nics-2.7.2/nics/main/_template/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-07-08 14:19:43.000000 nics-2.7.2/nics/main/_template/docs/404.md
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-07-08 14:19:43.000000 nics-2.7.2/nics/main/_template/docs/favicon.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:19:50.000000 nics-2.7.2/nics/main/_template/docs/tree/
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-07-08 14:19:43.000000 nics-2.7.2/nics/main/_template/docs/tree/1 - Page1.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:19:50.000000 nics-2.7.2/nics/main/_template/docs/tree/2 - Pages/
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-08 14:19:43.000000 nics-2.7.2/nics/main/_template/docs/tree/2 - Pages/baz.md
+-rw-r--r--   0 runner    (1001) docker     (123)    25360 2023-07-08 14:19:43.000000 nics-2.7.2/nics/main/_template/docs/tree/2 - Pages/logo200.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:19:50.000000 nics-2.7.2/nics/main/_template/docs/tree/7 - FAQs/
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-07-08 14:19:43.000000 nics-2.7.2/nics/main/_template/docs/tree/7 - FAQs/1 - Question1.md
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-08 14:19:43.000000 nics-2.7.2/nics/main/_template/docs/tree/7 - FAQs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-08 14:19:43.000000 nics-2.7.2/nics/main/_template/docs/tree/8 - Changelog.md
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-08 14:19:43.000000 nics-2.7.2/nics/main/_template/docs/tree/9 - About.md
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-08 14:19:43.000000 nics-2.7.2/nics/main/_template/docs/tree/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:19:50.000000 nics-2.7.2/nics/main/_template/web/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:19:50.000000 nics-2.7.2/nics/main/_template/web/_layouts/
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-07-08 14:19:43.000000 nics-2.7.2/nics/main/_template/web/_layouts/main.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:19:50.000000 nics-2.7.2/nics/main/_template/web/_sass/
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-07-08 14:19:43.000000 nics-2.7.2/nics/main/_template/web/_sass/footer.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-07-08 14:19:43.000000 nics-2.7.2/nics/main/_template/web/_sass/header.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-07-08 14:19:43.000000 nics-2.7.2/nics/main/_template/web/_sass/main.scss
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:19:50.000000 nics-2.7.2/nics/main/_template/web/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-07-08 14:19:43.000000 nics-2.7.2/nics/main/_template/web/scripts/header.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:19:50.000000 nics-2.7.2/nics/main/compile/
+-rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-07-08 14:19:43.000000 nics-2.7.2/nics/main/compile/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-07-08 14:19:43.000000 nics-2.7.2/nics/main/compile/copying_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-07-08 14:19:43.000000 nics-2.7.2/nics/main/compile/inspect.py
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-07-08 14:19:43.000000 nics-2.7.2/nics/main/compile/update_404_and_favicon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4442 2023-07-08 14:19:43.000000 nics-2.7.2/nics/main/compile/update_docs_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-07-08 14:19:43.000000 nics-2.7.2/nics/main/compile/update_footer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2268 2023-07-08 14:19:43.000000 nics-2.7.2/nics/main/compile/update_header.py
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-07-08 14:19:43.000000 nics-2.7.2/nics/main/compile/update_jekyll_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-07-08 14:19:43.000000 nics-2.7.2/nics/main/compile/update_sass_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-07-08 14:19:43.000000 nics-2.7.2/nics/main/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:19:50.000000 nics-2.7.2/nics/main/upgrade/
+-rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-07-08 14:19:43.000000 nics-2.7.2/nics/main/upgrade/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:19:50.000000 nics-2.7.2/nics/main/wizard/
+-rw-r--r--   0 runner    (1001) docker     (123)     3381 2023-07-08 14:19:43.000000 nics-2.7.2/nics/main/wizard/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-07-08 14:19:43.000000 nics-2.7.2/nics/main/wizard/settings_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2144 2023-07-08 14:19:43.000000 nics-2.7.2/nics/main/wizard/workflow_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:19:50.000000 nics-2.7.2/nics.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-07-08 14:19:50.000000 nics-2.7.2/nics.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-07-08 14:19:50.000000 nics-2.7.2/nics.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 14:19:50.000000 nics-2.7.2/nics.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-08 14:19:50.000000 nics-2.7.2/nics.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-08 14:19:50.000000 nics-2.7.2/nics.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-08 14:19:50.000000 nics-2.7.2/nics.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-07-08 14:19:44.000000 nics-2.7.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-07-08 14:19:43.000000 nics-2.7.2/readme.md
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-08 14:19:50.000000 nics-2.7.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-08 14:19:43.000000 nics-2.7.2/setup.py
```

### Comparing `nics-2.7.1/LICENSE` & `nics-2.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nics-2.7.1/PKG-INFO` & `nics-2.7.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nics
-Version: 2.7.1
+Version: 2.7.2
 Summary: Automated markdown-based documentation tool
 Home-page: https://nvfp.github.io/now-i-can-sleep
 Author: Nicholas Valentinus
 Author-email: nvfastplease@gmail.com
 License: MIT
 Project-URL: Documentation, https://nvfp.github.io/now-i-can-sleep/docs
 Project-URL: Report bugs, https://github.com/nvfp/now-i-can-sleep/issues
```

### Comparing `nics-2.7.1/nics/main/__init__.py` & `nics-2.7.2/nics/main/__init__.py`

 * *Files identical despite different names*

### Comparing `nics-2.7.1/nics/main/_template/docs/favicon.png` & `nics-2.7.2/nics/main/_template/docs/favicon.png`

 * *Files identical despite different names*

### Comparing `nics-2.7.1/nics/main/_template/docs/tree/2 - Pages/logo200.png` & `nics-2.7.2/nics/main/_template/docs/tree/2 - Pages/logo200.png`

 * *Files identical despite different names*

### Comparing `nics-2.7.1/nics/main/_template/web/_sass/header.scss` & `nics-2.7.2/nics/main/_template/web/_sass/header.scss`

 * *Files identical despite different names*

### Comparing `nics-2.7.1/nics/main/_template/web/_sass/main.scss` & `nics-2.7.2/nics/main/_template/web/_sass/main.scss`

 * *Files identical despite different names*

### Comparing `nics-2.7.1/nics/main/_template/web/scripts/header.js` & `nics-2.7.2/nics/main/_template/web/scripts/header.js`

 * *Files identical despite different names*

### Comparing `nics-2.7.1/nics/main/compile/__init__.py` & `nics-2.7.2/nics/main/compile/__init__.py`

 * *Files identical despite different names*

### Comparing `nics-2.7.1/nics/main/compile/copying_template.py` & `nics-2.7.2/nics/main/compile/copying_template.py`

 * *Files identical despite different names*

### Comparing `nics-2.7.1/nics/main/compile/update_404_and_favicon.py` & `nics-2.7.2/nics/main/compile/update_404_and_favicon.py`

 * *Files identical despite different names*

### Comparing `nics-2.7.1/nics/main/compile/update_docs_tree.py` & `nics-2.7.2/nics/main/compile/update_docs_tree.py`

 * *Files identical despite different names*

### Comparing `nics-2.7.1/nics/main/compile/update_header.py` & `nics-2.7.2/nics/main/compile/update_header.py`

 * *Files identical despite different names*

### Comparing `nics-2.7.1/nics/main/compile/update_jekyll_config.py` & `nics-2.7.2/nics/main/compile/update_jekyll_config.py`

 * *Files identical despite different names*

### Comparing `nics-2.7.1/nics/main/constants.py` & `nics-2.7.2/nics/main/constants.py`

 * *Files identical despite different names*

### Comparing `nics-2.7.1/nics/main/upgrade/__init__.py` & `nics-2.7.2/nics/main/upgrade/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 
     if __version__.split('.')[0] != cfg._nics_version.split('.')[0]:
         printer(f"ERROR: Cannot upgrade across major versions. Please run 'nics init' instead.")
         sys.exit(1)
 
 
     text = the_workflow_writer(cfg.author, cfg._email, cfg._gh_repo, cfg._main_branch_name)
-    with open(WORKFLOW_FILE_PTH, 'w') as f: f.write(text)
+    with open(WORKFLOW_FILE_PTH, 'w', encoding='utf-8') as f: f.write(text)
     printer(f'INFO: Workflow file {repr(WORKFLOW_FILE_PTH)} is updated.')
 
     text = the_settings_writer(
         cfg.author, cfg.color_hue, cfg.lowercase_the_url, cfg.show_credit,
         cfg._email, cfg._gh_username, cfg._gh_repo, cfg._main_branch_name
     )
     with open(SETTINGS_FILE_PTH, 'w') as f: f.write(text)
```

### Comparing `nics-2.7.1/nics/main/wizard/__init__.py` & `nics-2.7.2/nics/main/wizard/__init__.py`

 * *Files identical despite different names*

### Comparing `nics-2.7.1/nics/main/wizard/settings_writer.py` & `nics-2.7.2/nics/main/wizard/settings_writer.py`

 * *Files identical despite different names*

### Comparing `nics-2.7.1/nics/main/wizard/workflow_writer.py` & `nics-2.7.2/nics/main/wizard/workflow_writer.py`

 * *Files 5% similar despite different names*

```diff
@@ -67,22 +67,22 @@
           nics _compile "$(pwd)/docs" "$(pwd)/../{gh_repo}"
 
       - name: Deploy
         run: |
           git config user.name "{author}"
           git config user.email "{email}"
 
-          current_date=$(date +"%b %e, %l:%M %p")
+          current_date=$(date +"%Y %b %e, %l:%M %p")
           git commit -am "NICS rebuilds the docs — $current_date"
 
           git push
 """
 
 
 def workflow_writer(pth, author, email, gh_repo, main_branch_name):
     printer(f'INFO: Writing GitHub workflow file.')
 
     text = _writer(author, email, gh_repo, main_branch_name)
-    with open(pth, 'w') as f:
+    with open(pth, 'w', encoding='utf-8') as f:
         f.write(text)
 
     printer(f'INFO: Done, {repr(pth)} is created.')
```

### Comparing `nics-2.7.1/nics.egg-info/PKG-INFO` & `nics-2.7.2/nics.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nics
-Version: 2.7.1
+Version: 2.7.2
 Summary: Automated markdown-based documentation tool
 Home-page: https://nvfp.github.io/now-i-can-sleep
 Author: Nicholas Valentinus
 Author-email: nvfastplease@gmail.com
 License: MIT
 Project-URL: Documentation, https://nvfp.github.io/now-i-can-sleep/docs
 Project-URL: Report bugs, https://github.com/nvfp/now-i-can-sleep/issues
```

### Comparing `nics-2.7.1/nics.egg-info/SOURCES.txt` & `nics-2.7.2/nics.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nics-2.7.1/pyproject.toml` & `nics-2.7.2/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "nics"
-version = "2.7.1"
+version = "2.7.2"
 description = "Automated markdown-based documentation tool"
 readme = "readme.md"
 requires-python = ">=3.8"
 license = {text = "MIT"}
 authors = [
   	{email = "nvfastplease@gmail.com"},
 ]
```

### Comparing `nics-2.7.1/readme.md` & `nics-2.7.2/readme.md`

 * *Files identical despite different names*

