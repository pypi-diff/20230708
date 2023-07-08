# Comparing `tmp/nics-2.6.1.tar.gz` & `tmp/nics-2.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/now-i-can-sleep/now-i-can-sleep/dist/.tmp-u_y13uar/nics-2.6.1.tar", last modified: Sat Jul  1 19:47:39 2023, max compression
+gzip compressed data, was "/home/runner/work/now-i-can-sleep/now-i-can-sleep/dist/.tmp-6r4vqhpq/nics-2.7.1.tar", last modified: Sat Jul  8 12:17:04 2023, max compression
```

## Comparing `nics-2.6.1.tar` & `nics-2.7.1.tar`

### file list

```diff
@@ -1,64 +1,60 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 19:47:39.000000 nics-2.6.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-07-01 19:47:22.000000 nics-2.6.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-01 19:47:22.000000 nics-2.6.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-07-01 19:47:39.000000 nics-2.6.1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 19:47:39.000000 nics-2.6.1/nics/
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-01 19:47:22.000000 nics-2.6.1/nics/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 19:47:39.000000 nics-2.6.1/nics/main/
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-07-01 19:47:22.000000 nics-2.6.1/nics/main/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 19:47:39.000000 nics-2.6.1/nics/main/_template/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 19:47:39.000000 nics-2.6.1/nics/main/_template/docs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 19:47:22.000000 nics-2.6.1/nics/main/_template/docs/404.md
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-07-01 19:47:22.000000 nics-2.6.1/nics/main/_template/docs/favicon.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 19:47:39.000000 nics-2.6.1/nics/main/_template/docs/tree/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 19:47:22.000000 nics-2.6.1/nics/main/_template/docs/tree/1 -- THIS-IS-TITLE -- THIS-IS-URL.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 19:47:39.000000 nics-2.6.1/nics/main/_template/docs/tree/2 -- Bar -- bar/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-01 19:47:22.000000 nics-2.6.1/nics/main/_template/docs/tree/2 -- Bar -- bar/Hello -- world.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 19:47:22.000000 nics-2.6.1/nics/main/_template/docs/tree/2 -- Bar -- bar/Without Numbering -- Without-Numbering.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 19:47:22.000000 nics-2.6.1/nics/main/_template/docs/tree/2 -- Bar -- bar/index.md
--rw-r--r--   0 runner    (1001) docker     (123)    16526 2023-07-01 19:47:22.000000 nics-2.6.1/nics/main/_template/docs/tree/2 -- Bar -- bar/nics-logo500.jpg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 19:47:39.000000 nics-2.6.1/nics/main/_template/docs/tree/3 -- Foo Bar Baz -- foo-bar-baz/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 19:47:39.000000 nics-2.6.1/nics/main/_template/docs/tree/3 -- Foo Bar Baz -- foo-bar-baz/01 -- Nested -- nested/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 19:47:22.000000 nics-2.6.1/nics/main/_template/docs/tree/3 -- Foo Bar Baz -- foo-bar-baz/01 -- Nested -- nested/Without index.md -- without-index-md.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 19:47:22.000000 nics-2.6.1/nics/main/_template/docs/tree/3 -- Foo Bar Baz -- foo-bar-baz/02 -- bar -- bar.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 19:47:22.000000 nics-2.6.1/nics/main/_template/docs/tree/3 -- Foo Bar Baz -- foo-bar-baz/index.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 19:47:22.000000 nics-2.6.1/nics/main/_template/docs/tree/4 -- About -- about.md
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-01 19:47:22.000000 nics-2.6.1/nics/main/_template/docs/tree/5 -- This is a demo -- This-Is-A-Demo.md
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-01 19:47:22.000000 nics-2.6.1/nics/main/_template/docs/tree/index.md
--rw-r--r--   0 runner    (1001) docker     (123)    16526 2023-07-01 19:47:22.000000 nics-2.6.1/nics/main/_template/docs/tree/nics-logo500.jpg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 19:47:39.000000 nics-2.6.1/nics/main/_template/web/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 19:47:39.000000 nics-2.6.1/nics/main/_template/web/_layouts/
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-07-01 19:47:22.000000 nics-2.6.1/nics/main/_template/web/_layouts/main.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 19:47:39.000000 nics-2.6.1/nics/main/_template/web/_sass/
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-07-01 19:47:22.000000 nics-2.6.1/nics/main/_template/web/_sass/footer.scss
--rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-07-01 19:47:22.000000 nics-2.6.1/nics/main/_template/web/_sass/header.scss
--rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-07-01 19:47:22.000000 nics-2.6.1/nics/main/_template/web/_sass/main.scss
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 19:47:39.000000 nics-2.6.1/nics/main/_template/web/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-07-01 19:47:22.000000 nics-2.6.1/nics/main/_template/web/scripts/header.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 19:47:39.000000 nics-2.6.1/nics/main/compile/
--rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-07-01 19:47:22.000000 nics-2.6.1/nics/main/compile/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-07-01 19:47:22.000000 nics-2.6.1/nics/main/compile/copying_template.py
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-07-01 19:47:22.000000 nics-2.6.1/nics/main/compile/inspect.py
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-07-01 19:47:22.000000 nics-2.6.1/nics/main/compile/update_404_and_favicon.py
--rw-r--r--   0 runner    (1001) docker     (123)     4442 2023-07-01 19:47:22.000000 nics-2.6.1/nics/main/compile/update_docs_tree.py
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-07-01 19:47:22.000000 nics-2.6.1/nics/main/compile/update_footer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2268 2023-07-01 19:47:22.000000 nics-2.6.1/nics/main/compile/update_header.py
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-07-01 19:47:22.000000 nics-2.6.1/nics/main/compile/update_jekyll_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-07-01 19:47:22.000000 nics-2.6.1/nics/main/compile/update_sass_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-07-01 19:47:22.000000 nics-2.6.1/nics/main/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 19:47:39.000000 nics-2.6.1/nics/main/upgrade/
--rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-07-01 19:47:22.000000 nics-2.6.1/nics/main/upgrade/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 19:47:39.000000 nics-2.6.1/nics/main/wizard/
--rw-r--r--   0 runner    (1001) docker     (123)     3381 2023-07-01 19:47:22.000000 nics-2.6.1/nics/main/wizard/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-07-01 19:47:22.000000 nics-2.6.1/nics/main/wizard/settings_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-07-01 19:47:22.000000 nics-2.6.1/nics/main/wizard/workflow_writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 19:47:39.000000 nics-2.6.1/nics.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-07-01 19:47:39.000000 nics-2.6.1/nics.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-07-01 19:47:39.000000 nics-2.6.1/nics.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 19:47:39.000000 nics-2.6.1/nics.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-01 19:47:39.000000 nics-2.6.1/nics.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-01 19:47:39.000000 nics-2.6.1/nics.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-01 19:47:39.000000 nics-2.6.1/nics.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-07-01 19:47:22.000000 nics-2.6.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-01 19:47:39.000000 nics-2.6.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-01 19:47:22.000000 nics-2.6.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 12:17:04.000000 nics-2.7.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-07-08 12:16:56.000000 nics-2.7.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-08 12:16:56.000000 nics-2.7.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-07-08 12:17:04.000000 nics-2.7.1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 12:17:04.000000 nics-2.7.1/nics/
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-08 12:16:56.000000 nics-2.7.1/nics/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 12:17:04.000000 nics-2.7.1/nics/main/
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-07-08 12:16:56.000000 nics-2.7.1/nics/main/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 12:17:04.000000 nics-2.7.1/nics/main/_template/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 12:17:04.000000 nics-2.7.1/nics/main/_template/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-07-08 12:16:56.000000 nics-2.7.1/nics/main/_template/docs/404.md
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-07-08 12:16:56.000000 nics-2.7.1/nics/main/_template/docs/favicon.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 12:17:04.000000 nics-2.7.1/nics/main/_template/docs/tree/
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-07-08 12:16:56.000000 nics-2.7.1/nics/main/_template/docs/tree/1 - Page1.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 12:17:04.000000 nics-2.7.1/nics/main/_template/docs/tree/2 - Pages/
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-08 12:16:56.000000 nics-2.7.1/nics/main/_template/docs/tree/2 - Pages/baz.md
+-rw-r--r--   0 runner    (1001) docker     (123)    25360 2023-07-08 12:16:56.000000 nics-2.7.1/nics/main/_template/docs/tree/2 - Pages/logo200.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 12:17:04.000000 nics-2.7.1/nics/main/_template/docs/tree/7 - FAQs/
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-07-08 12:16:56.000000 nics-2.7.1/nics/main/_template/docs/tree/7 - FAQs/1 - Question1.md
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-08 12:16:56.000000 nics-2.7.1/nics/main/_template/docs/tree/7 - FAQs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-08 12:16:56.000000 nics-2.7.1/nics/main/_template/docs/tree/8 - Changelog.md
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-08 12:16:56.000000 nics-2.7.1/nics/main/_template/docs/tree/9 - About.md
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-08 12:16:56.000000 nics-2.7.1/nics/main/_template/docs/tree/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 12:17:04.000000 nics-2.7.1/nics/main/_template/web/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 12:17:04.000000 nics-2.7.1/nics/main/_template/web/_layouts/
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-07-08 12:16:56.000000 nics-2.7.1/nics/main/_template/web/_layouts/main.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 12:17:04.000000 nics-2.7.1/nics/main/_template/web/_sass/
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-07-08 12:16:56.000000 nics-2.7.1/nics/main/_template/web/_sass/footer.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-07-08 12:16:56.000000 nics-2.7.1/nics/main/_template/web/_sass/header.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-07-08 12:16:56.000000 nics-2.7.1/nics/main/_template/web/_sass/main.scss
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 12:17:04.000000 nics-2.7.1/nics/main/_template/web/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-07-08 12:16:56.000000 nics-2.7.1/nics/main/_template/web/scripts/header.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 12:17:04.000000 nics-2.7.1/nics/main/compile/
+-rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-07-08 12:16:56.000000 nics-2.7.1/nics/main/compile/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-07-08 12:16:56.000000 nics-2.7.1/nics/main/compile/copying_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-07-08 12:16:56.000000 nics-2.7.1/nics/main/compile/inspect.py
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-07-08 12:16:56.000000 nics-2.7.1/nics/main/compile/update_404_and_favicon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4442 2023-07-08 12:16:56.000000 nics-2.7.1/nics/main/compile/update_docs_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-07-08 12:16:56.000000 nics-2.7.1/nics/main/compile/update_footer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2268 2023-07-08 12:16:56.000000 nics-2.7.1/nics/main/compile/update_header.py
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-07-08 12:16:56.000000 nics-2.7.1/nics/main/compile/update_jekyll_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-07-08 12:16:56.000000 nics-2.7.1/nics/main/compile/update_sass_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-07-08 12:16:56.000000 nics-2.7.1/nics/main/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 12:17:04.000000 nics-2.7.1/nics/main/upgrade/
+-rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-07-08 12:16:56.000000 nics-2.7.1/nics/main/upgrade/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 12:17:04.000000 nics-2.7.1/nics/main/wizard/
+-rw-r--r--   0 runner    (1001) docker     (123)     3381 2023-07-08 12:16:56.000000 nics-2.7.1/nics/main/wizard/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-07-08 12:16:56.000000 nics-2.7.1/nics/main/wizard/settings_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-07-08 12:16:56.000000 nics-2.7.1/nics/main/wizard/workflow_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 12:17:04.000000 nics-2.7.1/nics.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-07-08 12:17:04.000000 nics-2.7.1/nics.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-07-08 12:17:04.000000 nics-2.7.1/nics.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 12:17:04.000000 nics-2.7.1/nics.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-08 12:17:04.000000 nics-2.7.1/nics.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-08 12:17:04.000000 nics-2.7.1/nics.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-08 12:17:04.000000 nics-2.7.1/nics.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-07-08 12:16:57.000000 nics-2.7.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-07-08 12:16:56.000000 nics-2.7.1/readme.md
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-08 12:17:04.000000 nics-2.7.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-08 12:16:56.000000 nics-2.7.1/setup.py
```

### Comparing `nics-2.6.1/LICENSE` & `nics-2.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nics-2.6.1/nics/main/__init__.py` & `nics-2.7.1/nics/main/__init__.py`

 * *Files identical despite different names*

### Comparing `nics-2.6.1/nics/main/_template/web/_sass/header.scss` & `nics-2.7.1/nics/main/_template/web/_sass/header.scss`

 * *Files identical despite different names*

### Comparing `nics-2.6.1/nics/main/_template/web/_sass/main.scss` & `nics-2.7.1/nics/main/_template/web/_sass/main.scss`

 * *Files identical despite different names*

### Comparing `nics-2.6.1/nics/main/_template/web/scripts/header.js` & `nics-2.7.1/nics/main/_template/web/scripts/header.js`

 * *Files identical despite different names*

### Comparing `nics-2.6.1/nics/main/compile/__init__.py` & `nics-2.7.1/nics/main/compile/__init__.py`

 * *Files identical despite different names*

### Comparing `nics-2.6.1/nics/main/compile/copying_template.py` & `nics-2.7.1/nics/main/compile/copying_template.py`

 * *Files identical despite different names*

### Comparing `nics-2.6.1/nics/main/compile/update_404_and_favicon.py` & `nics-2.7.1/nics/main/compile/update_404_and_favicon.py`

 * *Files identical despite different names*

### Comparing `nics-2.6.1/nics/main/compile/update_docs_tree.py` & `nics-2.7.1/nics/main/compile/update_docs_tree.py`

 * *Files identical despite different names*

### Comparing `nics-2.6.1/nics/main/compile/update_header.py` & `nics-2.7.1/nics/main/compile/update_header.py`

 * *Files identical despite different names*

### Comparing `nics-2.6.1/nics/main/compile/update_jekyll_config.py` & `nics-2.7.1/nics/main/compile/update_jekyll_config.py`

 * *Files identical despite different names*

### Comparing `nics-2.6.1/nics/main/constants.py` & `nics-2.7.1/nics/main/constants.py`

 * *Files identical despite different names*

### Comparing `nics-2.6.1/nics/main/upgrade/__init__.py` & `nics-2.7.1/nics/main/upgrade/__init__.py`

 * *Files identical despite different names*

### Comparing `nics-2.6.1/nics/main/wizard/__init__.py` & `nics-2.7.1/nics/main/wizard/__init__.py`

 * *Files identical despite different names*

### Comparing `nics-2.6.1/nics/main/wizard/settings_writer.py` & `nics-2.7.1/nics/main/wizard/settings_writer.py`

 * *Files identical despite different names*

### Comparing `nics-2.6.1/nics/main/wizard/workflow_writer.py` & `nics-2.7.1/nics/main/wizard/workflow_writer.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,41 +1,39 @@
 from mykit.kit.utils import printer
 
 from ..constants import __version__, SOFTWARE_DIST_NAME, SOFTWARE_REPO
 
 
 def _writer(author, email, gh_repo, main_branch_name):
     return f"""
-
 # This file was generated by {SOFTWARE_DIST_NAME}-v{__version__} .
-# Please make sure to be careful when modifying the values below. For more information, visit: {SOFTWARE_REPO}
+# Be careful when changing the values below, visit {SOFTWARE_REPO} for more info.
 
 name: Rebuild docs
 
 on:
   push:
     branches:
       - {main_branch_name}
 
     paths:
-      - 'docs/**'  # only rebuild if 'docs/' folder is modified
+      - 'docs/**'  # Only rebuild if 'docs/' folder is modified
 
-      # if using `use-repo-readme` keyword in 'tree/index.md'
+      # When using 'use-repo-readme' keyword in 'tree/index.md'
       - README.md
       - readme.md
 
   # Allows you to run this workflow manually from the Actions tab
   workflow_dispatch:
 
-permissions:
-  contents: write
-
 jobs:
-  deploy:
+  rebuild:
     runs-on: ubuntu-latest
+    permissions:
+      contents: write
 
     steps:
 
       - name: Checkout {main_branch_name} branch
         uses: actions/checkout@v3
         with:
           ref: {main_branch_name}
@@ -66,18 +64,20 @@
         run: |
           cd ..
           cd __nics_work_dir__
           nics _compile "$(pwd)/docs" "$(pwd)/../{gh_repo}"
 
       - name: Deploy
         run: |
-          git config user.name "{author} (via NICS)"
+          git config user.name "{author}"
           git config user.email "{email}"
-          git add .
-          git commit -m "NICS rebuilds the docs"
+
+          current_date=$(date +"%b %e, %l:%M %p")
+          git commit -am "NICS rebuilds the docs — $current_date"
+
           git push
 """
 
 
 def workflow_writer(pth, author, email, gh_repo, main_branch_name):
     printer(f'INFO: Writing GitHub workflow file.')
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `nics-2.6.1/nics.egg-info/SOURCES.txt` & `nics-2.7.1/nics.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,35 +1,32 @@
 LICENSE
 MANIFEST.in
 pyproject.toml
+readme.md
 setup.cfg
 setup.py
 nics/__main__.py
 nics.egg-info/PKG-INFO
 nics.egg-info/SOURCES.txt
 nics.egg-info/dependency_links.txt
 nics.egg-info/entry_points.txt
 nics.egg-info/requires.txt
 nics.egg-info/top_level.txt
 nics/main/__init__.py
 nics/main/constants.py
 nics/main/_template/docs/404.md
 nics/main/_template/docs/favicon.png
-nics/main/_template/docs/tree/1 -- THIS-IS-TITLE -- THIS-IS-URL.md
-nics/main/_template/docs/tree/4 -- About -- about.md
-nics/main/_template/docs/tree/5 -- This is a demo -- This-Is-A-Demo.md
+nics/main/_template/docs/tree/1 - Page1.md
+nics/main/_template/docs/tree/8 - Changelog.md
+nics/main/_template/docs/tree/9 - About.md
 nics/main/_template/docs/tree/index.md
-nics/main/_template/docs/tree/nics-logo500.jpg
-nics/main/_template/docs/tree/2 -- Bar -- bar/Hello -- world.md
-nics/main/_template/docs/tree/2 -- Bar -- bar/Without Numbering -- Without-Numbering.md
-nics/main/_template/docs/tree/2 -- Bar -- bar/index.md
-nics/main/_template/docs/tree/2 -- Bar -- bar/nics-logo500.jpg
-nics/main/_template/docs/tree/3 -- Foo Bar Baz -- foo-bar-baz/02 -- bar -- bar.md
-nics/main/_template/docs/tree/3 -- Foo Bar Baz -- foo-bar-baz/index.md
-nics/main/_template/docs/tree/3 -- Foo Bar Baz -- foo-bar-baz/01 -- Nested -- nested/Without index.md -- without-index-md.md
+nics/main/_template/docs/tree/2 - Pages/baz.md
+nics/main/_template/docs/tree/2 - Pages/logo200.png
+nics/main/_template/docs/tree/7 - FAQs/1 - Question1.md
+nics/main/_template/docs/tree/7 - FAQs/index.md
 nics/main/_template/web/_layouts/main.html
 nics/main/_template/web/_sass/footer.scss
 nics/main/_template/web/_sass/header.scss
 nics/main/_template/web/_sass/main.scss
 nics/main/_template/web/scripts/header.js
 nics/main/compile/__init__.py
 nics/main/compile/copying_template.py
```

### Comparing `nics-2.6.1/pyproject.toml` & `nics-2.7.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "nics"
-version = "2.6.1"
+version = "2.7.1"
 description = "Automated markdown-based documentation tool"
-readme = "README.md"
+readme = "readme.md"
 requires-python = ">=3.8"
 license = {text = "MIT"}
 authors = [
   	{email = "nvfastplease@gmail.com"},
 ]
 keywords = ["python", "toolkit", "mykit"]
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Natural Language :: English",
     "Operating System :: OS Independent",
     "Programming Language :: Python",
     "Topic :: Scientific/Engineering",
 ]
 dependencies = [
-    "mykit==4.1.0",
+    "mykit==6.0.0",
     "requests>=2.31.0",
 ]
 
 
 [tool.setuptools.packages.find]
 exclude = [
     "archive*",
```

