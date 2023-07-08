# Comparing `tmp/sphinx_basic_ng-1.0.0b1.tar.gz` & `tmp/sphinx_basic_ng-1.0.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sphinx_basic_ng-1.0.0b1.tar", last modified: Thu Sep 29 22:10:48 2022, max compression
+gzip compressed data, was "sphinx_basic_ng-1.0.0b2.tar", last modified: Sat Jul  8 18:40:43 2023, max compression
```

## Comparing `sphinx_basic_ng-1.0.0b1.tar` & `sphinx_basic_ng-1.0.0b2.tar`

### file list

```diff
@@ -1,89 +1,89 @@
-drwxr-xr-x   0 pradyunsg   (501) staff       (20)        0 2022-09-29 22:10:48.720125 sphinx_basic_ng-1.0.0b1/
--rw-r--r--   0 pradyunsg   (501) staff       (20)     1078 2021-07-09 14:03:31.000000 sphinx_basic_ng-1.0.0b1/LICENSE
--rw-r--r--   0 pradyunsg   (501) staff       (20)      331 2021-07-09 14:03:31.000000 sphinx_basic_ng-1.0.0b1/MANIFEST.in
--rw-r--r--   0 pradyunsg   (501) staff       (20)     1211 2022-09-29 22:10:48.720241 sphinx_basic_ng-1.0.0b1/PKG-INFO
--rw-r--r--   0 pradyunsg   (501) staff       (20)      426 2022-06-02 12:17:25.000000 sphinx_basic_ng-1.0.0b1/README.md
-drwxr-xr-x   0 pradyunsg   (501) staff       (20)        0 2022-09-29 22:10:48.700874 sphinx_basic_ng-1.0.0b1/docs/
--rw-r--r--   0 pradyunsg   (501) staff       (20)     2518 2022-06-27 20:54:22.000000 sphinx_basic_ng-1.0.0b1/docs/changelog.md
--rw-r--r--   0 pradyunsg   (501) staff       (20)     1547 2021-07-09 14:03:31.000000 sphinx_basic_ng-1.0.0b1/docs/conf.py
-drwxr-xr-x   0 pradyunsg   (501) staff       (20)        0 2022-09-29 22:10:48.701046 sphinx_basic_ng-1.0.0b1/docs/design/
--rw-r--r--   0 pradyunsg   (501) staff       (20)      178 2022-06-02 12:17:25.000000 sphinx_basic_ng-1.0.0b1/docs/design/index.md
-drwxr-xr-x   0 pradyunsg   (501) staff       (20)        0 2022-09-29 22:10:48.701321 sphinx_basic_ng-1.0.0b1/docs/development/
--rw-r--r--   0 pradyunsg   (501) staff       (20)      153 2022-06-02 12:14:00.000000 sphinx_basic_ng-1.0.0b1/docs/development/index.md
--rw-r--r--   0 pradyunsg   (501) staff       (20)     1838 2022-06-02 11:16:33.000000 sphinx_basic_ng-1.0.0b1/docs/expectations.md
--rw-r--r--   0 pradyunsg   (501) staff       (20)      389 2022-06-02 11:02:22.000000 sphinx_basic_ng-1.0.0b1/docs/glossary.md
--rw-r--r--   0 pradyunsg   (501) staff       (20)     1067 2022-06-27 21:06:06.000000 sphinx_basic_ng-1.0.0b1/docs/goals.md
--rw-r--r--   0 pradyunsg   (501) staff       (20)      456 2022-06-02 11:17:16.000000 sphinx_basic_ng-1.0.0b1/docs/index.md
--rw-r--r--   0 pradyunsg   (501) staff       (20)       66 2021-07-09 14:03:31.000000 sphinx_basic_ng-1.0.0b1/docs/license.rst
-drwxr-xr-x   0 pradyunsg   (501) staff       (20)        0 2022-09-29 22:10:48.701862 sphinx_basic_ng-1.0.0b1/docs/usage/
-drwxr-xr-x   0 pradyunsg   (501) staff       (20)        0 2022-09-29 22:10:48.705084 sphinx_basic_ng-1.0.0b1/docs/usage/components/
--rw-r--r--   0 pradyunsg   (501) staff       (20)     1475 2022-06-02 11:23:59.000000 sphinx_basic_ng-1.0.0b1/docs/usage/components/breadcrumbs.md
--rw-r--r--   0 pradyunsg   (501) staff       (20)     2661 2022-09-29 22:09:16.000000 sphinx_basic_ng-1.0.0b1/docs/usage/components/edit-this-page.md
--rw-r--r--   0 pradyunsg   (501) staff       (20)     1682 2022-06-02 11:41:14.000000 sphinx_basic_ng-1.0.0b1/docs/usage/components/ethical-ads.md
--rw-r--r--   0 pradyunsg   (501) staff       (20)      311 2022-06-02 18:30:08.000000 sphinx_basic_ng-1.0.0b1/docs/usage/components/index.md
--rw-r--r--   0 pradyunsg   (501) staff       (20)      398 2022-06-02 11:41:12.000000 sphinx_basic_ng-1.0.0b1/docs/usage/components/logo.md
--rw-r--r--   0 pradyunsg   (501) staff       (20)     1121 2022-06-03 10:53:54.000000 sphinx_basic_ng-1.0.0b1/docs/usage/components/related-pages.md
--rw-r--r--   0 pradyunsg   (501) staff       (20)      714 2022-06-02 11:41:07.000000 sphinx_basic_ng-1.0.0b1/docs/usage/components/search-hide.md
--rw-r--r--   0 pradyunsg   (501) staff       (20)      620 2022-06-02 11:43:39.000000 sphinx_basic_ng-1.0.0b1/docs/usage/components/search-input.md
--rw-r--r--   0 pradyunsg   (501) staff       (20)      848 2022-06-02 11:51:19.000000 sphinx_basic_ng-1.0.0b1/docs/usage/components/sidebar-toggles.md
--rw-r--r--   0 pradyunsg   (501) staff       (20)     3051 2022-09-29 22:09:16.000000 sphinx_basic_ng-1.0.0b1/docs/usage/components/view-this-page.md
--rw-r--r--   0 pradyunsg   (501) staff       (20)       59 2021-07-10 19:00:14.000000 sphinx_basic_ng-1.0.0b1/docs/usage/getting-started.md
--rw-r--r--   0 pradyunsg   (501) staff       (20)      218 2021-07-09 14:03:31.000000 sphinx_basic_ng-1.0.0b1/docs/usage/skeleton.md
--rw-r--r--   0 pradyunsg   (501) staff       (20)     1088 2022-09-29 22:10:48.720576 sphinx_basic_ng-1.0.0b1/setup.cfg
--rw-r--r--   0 pradyunsg   (501) staff       (20)       38 2021-07-09 14:03:31.000000 sphinx_basic_ng-1.0.0b1/setup.py
-drwxr-xr-x   0 pradyunsg   (501) staff       (20)        0 2022-09-29 22:10:48.697325 sphinx_basic_ng-1.0.0b1/src/
-drwxr-xr-x   0 pradyunsg   (501) staff       (20)        0 2022-09-29 22:10:48.705367 sphinx_basic_ng-1.0.0b1/src/sphinx_basic_ng/
--rw-r--r--   0 pradyunsg   (501) staff       (20)      533 2022-09-29 22:10:44.000000 sphinx_basic_ng-1.0.0b1/src/sphinx_basic_ng/__init__.py
-drwxr-xr-x   0 pradyunsg   (501) staff       (20)        0 2022-09-29 22:10:48.697435 sphinx_basic_ng-1.0.0b1/src/sphinx_basic_ng/theme/
-drwxr-xr-x   0 pradyunsg   (501) staff       (20)        0 2022-09-29 22:10:48.710918 sphinx_basic_ng-1.0.0b1/src/sphinx_basic_ng/theme/basic-ng/
-drwxr-xr-x   0 pradyunsg   (501) staff       (20)        0 2022-09-29 22:10:48.711569 sphinx_basic_ng-1.0.0b1/src/sphinx_basic_ng/theme/basic-ng/changes/
--rw-r--r--   0 pradyunsg   (501) staff       (20)       67 2021-11-21 11:08:51.000000 sphinx_basic_ng-1.0.0b1/src/sphinx_basic_ng/theme/basic-ng/changes/frameset.html
--rw-r--r--   0 pradyunsg   (501) staff       (20)       68 2021-11-21 11:08:51.000000 sphinx_basic_ng-1.0.0b1/src/sphinx_basic_ng/theme/basic-ng/changes/rstsource.html
--rw-r--r--   0 pradyunsg   (501) staff       (20)       73 2021-11-21 11:08:51.000000 sphinx_basic_ng-1.0.0b1/src/sphinx_basic_ng/theme/basic-ng/changes/versionchanges.html
-drwxr-xr-x   0 pradyunsg   (501) staff       (20)        0 2022-09-29 22:10:48.713836 sphinx_basic_ng-1.0.0b1/src/sphinx_basic_ng/theme/basic-ng/components/
--rw-r--r--   0 pradyunsg   (501) staff       (20)      923 2021-11-21 19:25:25.000000 sphinx_basic_ng-1.0.0b1/src/sphinx_basic_ng/theme/basic-ng/components/breadcrumbs.html
--rw-r--r--   0 pradyunsg   (501) staff       (20)     2258 2022-09-29 22:09:16.000000 sphinx_basic_ng-1.0.0b1/src/sphinx_basic_ng/theme/basic-ng/components/edit-this-page.html
--rw-r--r--   0 pradyunsg   (501) staff       (20)      321 2021-07-09 14:03:31.000000 sphinx_basic_ng-1.0.0b1/src/sphinx_basic_ng/theme/basic-ng/components/ethical-ads.html
--rw-r--r--   0 pradyunsg   (501) staff       (20)      103 2022-06-02 11:40:19.000000 sphinx_basic_ng-1.0.0b1/src/sphinx_basic_ng/theme/basic-ng/components/logo.html
--rw-r--r--   0 pradyunsg   (501) staff       (20)      816 2021-07-09 14:03:31.000000 sphinx_basic_ng-1.0.0b1/src/sphinx_basic_ng/theme/basic-ng/components/related-pages.html
--rw-r--r--   0 pradyunsg   (501) staff       (20)       27 2021-07-09 14:03:31.000000 sphinx_basic_ng-1.0.0b1/src/sphinx_basic_ng/theme/basic-ng/components/search-hide.html
--rw-r--r--   0 pradyunsg   (501) staff       (20)      157 2021-07-09 14:03:31.000000 sphinx_basic_ng-1.0.0b1/src/sphinx_basic_ng/theme/basic-ng/components/search-input.html
--rw-r--r--   0 pradyunsg   (501) staff       (20)      561 2022-09-29 22:09:20.000000 sphinx_basic_ng-1.0.0b1/src/sphinx_basic_ng/theme/basic-ng/components/toggle-sidebar-primary.html
--rw-r--r--   0 pradyunsg   (501) staff       (20)      565 2022-09-29 22:09:20.000000 sphinx_basic_ng-1.0.0b1/src/sphinx_basic_ng/theme/basic-ng/components/toggle-sidebar-secondary.html
--rw-r--r--   0 pradyunsg   (501) staff       (20)     2421 2022-09-29 22:09:16.000000 sphinx_basic_ng-1.0.0b1/src/sphinx_basic_ng/theme/basic-ng/components/view-this-page.html
--rw-r--r--   0 pradyunsg   (501) staff       (20)       58 2021-11-21 11:08:51.000000 sphinx_basic_ng-1.0.0b1/src/sphinx_basic_ng/theme/basic-ng/defindex.html
--rw-r--r--   0 pradyunsg   (501) staff       (20)     1910 2022-03-19 09:57:44.000000 sphinx_basic_ng-1.0.0b1/src/sphinx_basic_ng/theme/basic-ng/domainindex.html
--rw-r--r--   0 pradyunsg   (501) staff       (20)     1610 2022-03-19 09:57:59.000000 sphinx_basic_ng-1.0.0b1/src/sphinx_basic_ng/theme/basic-ng/genindex-single.html
--rw-r--r--   0 pradyunsg   (501) staff       (20)      807 2022-03-19 09:58:19.000000 sphinx_basic_ng-1.0.0b1/src/sphinx_basic_ng/theme/basic-ng/genindex-split.html
--rw-r--r--   0 pradyunsg   (501) staff       (20)     1823 2022-03-19 09:58:42.000000 sphinx_basic_ng-1.0.0b1/src/sphinx_basic_ng/theme/basic-ng/genindex.html
--rw-r--r--   0 pradyunsg   (501) staff       (20)       60 2021-11-21 11:08:51.000000 sphinx_basic_ng-1.0.0b1/src/sphinx_basic_ng/theme/basic-ng/globaltoc.html
--rw-r--r--   0 pradyunsg   (501) staff       (20)     2149 2022-01-05 08:21:13.000000 sphinx_basic_ng-1.0.0b1/src/sphinx_basic_ng/theme/basic-ng/layout.html
--rw-r--r--   0 pradyunsg   (501) staff       (20)       59 2021-11-21 11:08:51.000000 sphinx_basic_ng-1.0.0b1/src/sphinx_basic_ng/theme/basic-ng/localtoc.html
--rw-r--r--   0 pradyunsg   (501) staff       (20)     2788 2022-06-27 21:11:48.000000 sphinx_basic_ng-1.0.0b1/src/sphinx_basic_ng/theme/basic-ng/page.html
--rw-r--r--   0 pradyunsg   (501) staff       (20)       60 2021-11-21 11:08:51.000000 sphinx_basic_ng-1.0.0b1/src/sphinx_basic_ng/theme/basic-ng/relations.html
--rw-r--r--   0 pradyunsg   (501) staff       (20)      934 2022-01-23 11:31:12.000000 sphinx_basic_ng-1.0.0b1/src/sphinx_basic_ng/theme/basic-ng/search.html
--rw-r--r--   0 pradyunsg   (501) staff       (20)       60 2021-11-21 11:08:51.000000 sphinx_basic_ng-1.0.0b1/src/sphinx_basic_ng/theme/basic-ng/searchbox.html
-drwxr-xr-x   0 pradyunsg   (501) staff       (20)        0 2022-09-29 22:10:48.719474 sphinx_basic_ng-1.0.0b1/src/sphinx_basic_ng/theme/basic-ng/sections/
--rw-r--r--   0 pradyunsg   (501) staff       (20)       27 2021-07-09 14:03:31.000000 sphinx_basic_ng-1.0.0b1/src/sphinx_basic_ng/theme/basic-ng/sections/announcement.html
--rw-r--r--   0 pradyunsg   (501) staff       (20)      810 2021-07-09 14:03:31.000000 sphinx_basic_ng-1.0.0b1/src/sphinx_basic_ng/theme/basic-ng/sections/article.html
--rw-r--r--   0 pradyunsg   (501) staff       (20)       29 2021-07-09 14:03:31.000000 sphinx_basic_ng-1.0.0b1/src/sphinx_basic_ng/theme/basic-ng/sections/footer-article.html
--rw-r--r--   0 pradyunsg   (501) staff       (20)       29 2021-07-09 14:03:31.000000 sphinx_basic_ng-1.0.0b1/src/sphinx_basic_ng/theme/basic-ng/sections/footer-content.html
--rw-r--r--   0 pradyunsg   (501) staff       (20)       21 2021-07-09 14:03:31.000000 sphinx_basic_ng-1.0.0b1/src/sphinx_basic_ng/theme/basic-ng/sections/footer.html
--rw-r--r--   0 pradyunsg   (501) staff       (20)       29 2021-07-10 19:00:17.000000 sphinx_basic_ng-1.0.0b1/src/sphinx_basic_ng/theme/basic-ng/sections/header-article.html
--rw-r--r--   0 pradyunsg   (501) staff       (20)       29 2022-01-23 11:33:05.000000 sphinx_basic_ng-1.0.0b1/src/sphinx_basic_ng/theme/basic-ng/sections/header-content.html
--rw-r--r--   0 pradyunsg   (501) staff       (20)       31 2021-07-09 14:03:31.000000 sphinx_basic_ng-1.0.0b1/src/sphinx_basic_ng/theme/basic-ng/sections/header-secondary.html
--rw-r--r--   0 pradyunsg   (501) staff       (20)       21 2021-07-11 12:14:07.000000 sphinx_basic_ng-1.0.0b1/src/sphinx_basic_ng/theme/basic-ng/sections/header.html
--rw-r--r--   0 pradyunsg   (501) staff       (20)       30 2021-07-09 14:03:31.000000 sphinx_basic_ng-1.0.0b1/src/sphinx_basic_ng/theme/basic-ng/sections/sidebar-primary.html
--rw-r--r--   0 pradyunsg   (501) staff       (20)       32 2021-07-09 14:03:31.000000 sphinx_basic_ng-1.0.0b1/src/sphinx_basic_ng/theme/basic-ng/sections/sidebar-secondary.html
--rw-r--r--   0 pradyunsg   (501) staff       (20)       61 2021-11-21 11:08:51.000000 sphinx_basic_ng-1.0.0b1/src/sphinx_basic_ng/theme/basic-ng/sourcelink.html
-drwxr-xr-x   0 pradyunsg   (501) staff       (20)        0 2022-09-29 22:10:48.719875 sphinx_basic_ng-1.0.0b1/src/sphinx_basic_ng/theme/basic-ng/static/
--rw-r--r--   0 pradyunsg   (501) staff       (20)     1266 2022-06-27 21:12:25.000000 sphinx_basic_ng-1.0.0b1/src/sphinx_basic_ng/theme/basic-ng/static/debug.css
--rw-r--r--   0 pradyunsg   (501) staff       (20)     6034 2022-06-27 21:11:51.000000 sphinx_basic_ng-1.0.0b1/src/sphinx_basic_ng/theme/basic-ng/static/skeleton.css
--rw-r--r--   0 pradyunsg   (501) staff       (20)       69 2021-07-09 14:03:31.000000 sphinx_basic_ng-1.0.0b1/src/sphinx_basic_ng/theme/basic-ng/theme.conf
-drwxr-xr-x   0 pradyunsg   (501) staff       (20)        0 2022-09-29 22:10:48.706289 sphinx_basic_ng-1.0.0b1/src/sphinx_basic_ng.egg-info/
--rw-r--r--   0 pradyunsg   (501) staff       (20)     1211 2022-09-29 22:10:48.000000 sphinx_basic_ng-1.0.0b1/src/sphinx_basic_ng.egg-info/PKG-INFO
--rw-r--r--   0 pradyunsg   (501) staff       (20)     3246 2022-09-29 22:10:48.000000 sphinx_basic_ng-1.0.0b1/src/sphinx_basic_ng.egg-info/SOURCES.txt
--rw-r--r--   0 pradyunsg   (501) staff       (20)        1 2022-09-29 22:10:48.000000 sphinx_basic_ng-1.0.0b1/src/sphinx_basic_ng.egg-info/dependency_links.txt
--rw-r--r--   0 pradyunsg   (501) staff       (20)       48 2022-09-29 22:10:48.000000 sphinx_basic_ng-1.0.0b1/src/sphinx_basic_ng.egg-info/entry_points.txt
--rw-r--r--   0 pradyunsg   (501) staff       (20)       82 2022-09-29 22:10:48.000000 sphinx_basic_ng-1.0.0b1/src/sphinx_basic_ng.egg-info/requires.txt
--rw-r--r--   0 pradyunsg   (501) staff       (20)       16 2022-09-29 22:10:48.000000 sphinx_basic_ng-1.0.0b1/src/sphinx_basic_ng.egg-info/top_level.txt
+drwxr-xr-x   0 pradyunsg   (501) staff       (20)        0 2023-07-08 18:40:43.703753 sphinx_basic_ng-1.0.0b2/
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     1078 2021-07-09 14:03:31.000000 sphinx_basic_ng-1.0.0b2/LICENSE
+-rw-r--r--   0 pradyunsg   (501) staff       (20)      331 2021-07-09 14:03:31.000000 sphinx_basic_ng-1.0.0b2/MANIFEST.in
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     1211 2023-07-08 18:40:43.703865 sphinx_basic_ng-1.0.0b2/PKG-INFO
+-rw-r--r--   0 pradyunsg   (501) staff       (20)      426 2022-06-02 12:17:25.000000 sphinx_basic_ng-1.0.0b2/README.md
+drwxr-xr-x   0 pradyunsg   (501) staff       (20)        0 2023-07-08 18:40:43.682123 sphinx_basic_ng-1.0.0b2/docs/
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     2518 2022-06-27 20:54:22.000000 sphinx_basic_ng-1.0.0b2/docs/changelog.md
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     1547 2021-07-09 14:03:31.000000 sphinx_basic_ng-1.0.0b2/docs/conf.py
+drwxr-xr-x   0 pradyunsg   (501) staff       (20)        0 2023-07-08 18:40:43.682416 sphinx_basic_ng-1.0.0b2/docs/design/
+-rw-r--r--   0 pradyunsg   (501) staff       (20)      178 2022-06-02 12:17:25.000000 sphinx_basic_ng-1.0.0b2/docs/design/index.md
+drwxr-xr-x   0 pradyunsg   (501) staff       (20)        0 2023-07-08 18:40:43.682727 sphinx_basic_ng-1.0.0b2/docs/development/
+-rw-r--r--   0 pradyunsg   (501) staff       (20)      153 2022-06-02 12:14:00.000000 sphinx_basic_ng-1.0.0b2/docs/development/index.md
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     1838 2022-06-02 11:16:33.000000 sphinx_basic_ng-1.0.0b2/docs/expectations.md
+-rw-r--r--   0 pradyunsg   (501) staff       (20)      389 2022-06-02 11:02:22.000000 sphinx_basic_ng-1.0.0b2/docs/glossary.md
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     1067 2022-06-27 21:06:06.000000 sphinx_basic_ng-1.0.0b2/docs/goals.md
+-rw-r--r--   0 pradyunsg   (501) staff       (20)      456 2022-06-02 11:17:16.000000 sphinx_basic_ng-1.0.0b2/docs/index.md
+-rw-r--r--   0 pradyunsg   (501) staff       (20)       66 2021-07-09 14:03:31.000000 sphinx_basic_ng-1.0.0b2/docs/license.rst
+drwxr-xr-x   0 pradyunsg   (501) staff       (20)        0 2023-07-08 18:40:43.683290 sphinx_basic_ng-1.0.0b2/docs/usage/
+drwxr-xr-x   0 pradyunsg   (501) staff       (20)        0 2023-07-08 18:40:43.686840 sphinx_basic_ng-1.0.0b2/docs/usage/components/
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     1475 2022-06-02 11:23:59.000000 sphinx_basic_ng-1.0.0b2/docs/usage/components/breadcrumbs.md
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     2661 2022-09-29 22:09:16.000000 sphinx_basic_ng-1.0.0b2/docs/usage/components/edit-this-page.md
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     1682 2022-06-02 11:41:14.000000 sphinx_basic_ng-1.0.0b2/docs/usage/components/ethical-ads.md
+-rw-r--r--   0 pradyunsg   (501) staff       (20)      311 2022-06-02 18:30:08.000000 sphinx_basic_ng-1.0.0b2/docs/usage/components/index.md
+-rw-r--r--   0 pradyunsg   (501) staff       (20)      398 2022-06-02 11:41:12.000000 sphinx_basic_ng-1.0.0b2/docs/usage/components/logo.md
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     1121 2022-06-03 10:53:54.000000 sphinx_basic_ng-1.0.0b2/docs/usage/components/related-pages.md
+-rw-r--r--   0 pradyunsg   (501) staff       (20)      714 2022-06-02 11:41:07.000000 sphinx_basic_ng-1.0.0b2/docs/usage/components/search-hide.md
+-rw-r--r--   0 pradyunsg   (501) staff       (20)      620 2022-06-02 11:43:39.000000 sphinx_basic_ng-1.0.0b2/docs/usage/components/search-input.md
+-rw-r--r--   0 pradyunsg   (501) staff       (20)      848 2022-06-02 11:51:19.000000 sphinx_basic_ng-1.0.0b2/docs/usage/components/sidebar-toggles.md
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     3051 2022-09-29 22:09:16.000000 sphinx_basic_ng-1.0.0b2/docs/usage/components/view-this-page.md
+-rw-r--r--   0 pradyunsg   (501) staff       (20)       59 2021-07-10 19:00:14.000000 sphinx_basic_ng-1.0.0b2/docs/usage/getting-started.md
+-rw-r--r--   0 pradyunsg   (501) staff       (20)      218 2021-07-09 14:03:31.000000 sphinx_basic_ng-1.0.0b2/docs/usage/skeleton.md
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     1088 2023-07-08 18:40:43.704445 sphinx_basic_ng-1.0.0b2/setup.cfg
+-rw-r--r--   0 pradyunsg   (501) staff       (20)       38 2021-07-09 14:03:31.000000 sphinx_basic_ng-1.0.0b2/setup.py
+drwxr-xr-x   0 pradyunsg   (501) staff       (20)        0 2023-07-08 18:40:43.677247 sphinx_basic_ng-1.0.0b2/src/
+drwxr-xr-x   0 pradyunsg   (501) staff       (20)        0 2023-07-08 18:40:43.687255 sphinx_basic_ng-1.0.0b2/src/sphinx_basic_ng/
+-rw-r--r--   0 pradyunsg   (501) staff       (20)      533 2023-07-08 18:40:39.000000 sphinx_basic_ng-1.0.0b2/src/sphinx_basic_ng/__init__.py
+drwxr-xr-x   0 pradyunsg   (501) staff       (20)        0 2023-07-08 18:40:43.677476 sphinx_basic_ng-1.0.0b2/src/sphinx_basic_ng/theme/
+drwxr-xr-x   0 pradyunsg   (501) staff       (20)        0 2023-07-08 18:40:43.693700 sphinx_basic_ng-1.0.0b2/src/sphinx_basic_ng/theme/basic-ng/
+drwxr-xr-x   0 pradyunsg   (501) staff       (20)        0 2023-07-08 18:40:43.694751 sphinx_basic_ng-1.0.0b2/src/sphinx_basic_ng/theme/basic-ng/changes/
+-rw-r--r--   0 pradyunsg   (501) staff       (20)       67 2021-11-21 11:08:51.000000 sphinx_basic_ng-1.0.0b2/src/sphinx_basic_ng/theme/basic-ng/changes/frameset.html
+-rw-r--r--   0 pradyunsg   (501) staff       (20)       68 2021-11-21 11:08:51.000000 sphinx_basic_ng-1.0.0b2/src/sphinx_basic_ng/theme/basic-ng/changes/rstsource.html
+-rw-r--r--   0 pradyunsg   (501) staff       (20)       73 2021-11-21 11:08:51.000000 sphinx_basic_ng-1.0.0b2/src/sphinx_basic_ng/theme/basic-ng/changes/versionchanges.html
+drwxr-xr-x   0 pradyunsg   (501) staff       (20)        0 2023-07-08 18:40:43.698634 sphinx_basic_ng-1.0.0b2/src/sphinx_basic_ng/theme/basic-ng/components/
+-rw-r--r--   0 pradyunsg   (501) staff       (20)      923 2021-11-21 19:25:25.000000 sphinx_basic_ng-1.0.0b2/src/sphinx_basic_ng/theme/basic-ng/components/breadcrumbs.html
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     2258 2022-09-29 22:09:16.000000 sphinx_basic_ng-1.0.0b2/src/sphinx_basic_ng/theme/basic-ng/components/edit-this-page.html
+-rw-r--r--   0 pradyunsg   (501) staff       (20)      321 2021-07-09 14:03:31.000000 sphinx_basic_ng-1.0.0b2/src/sphinx_basic_ng/theme/basic-ng/components/ethical-ads.html
+-rw-r--r--   0 pradyunsg   (501) staff       (20)      103 2022-06-02 11:40:19.000000 sphinx_basic_ng-1.0.0b2/src/sphinx_basic_ng/theme/basic-ng/components/logo.html
+-rw-r--r--   0 pradyunsg   (501) staff       (20)      816 2021-07-09 14:03:31.000000 sphinx_basic_ng-1.0.0b2/src/sphinx_basic_ng/theme/basic-ng/components/related-pages.html
+-rw-r--r--   0 pradyunsg   (501) staff       (20)       27 2021-07-09 14:03:31.000000 sphinx_basic_ng-1.0.0b2/src/sphinx_basic_ng/theme/basic-ng/components/search-hide.html
+-rw-r--r--   0 pradyunsg   (501) staff       (20)      157 2021-07-09 14:03:31.000000 sphinx_basic_ng-1.0.0b2/src/sphinx_basic_ng/theme/basic-ng/components/search-input.html
+-rw-r--r--   0 pradyunsg   (501) staff       (20)      561 2022-09-29 22:09:20.000000 sphinx_basic_ng-1.0.0b2/src/sphinx_basic_ng/theme/basic-ng/components/toggle-sidebar-primary.html
+-rw-r--r--   0 pradyunsg   (501) staff       (20)      565 2022-09-29 22:09:20.000000 sphinx_basic_ng-1.0.0b2/src/sphinx_basic_ng/theme/basic-ng/components/toggle-sidebar-secondary.html
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     2405 2022-11-26 14:33:38.000000 sphinx_basic_ng-1.0.0b2/src/sphinx_basic_ng/theme/basic-ng/components/view-this-page.html
+-rw-r--r--   0 pradyunsg   (501) staff       (20)       58 2021-11-21 11:08:51.000000 sphinx_basic_ng-1.0.0b2/src/sphinx_basic_ng/theme/basic-ng/defindex.html
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     1910 2022-03-19 09:57:44.000000 sphinx_basic_ng-1.0.0b2/src/sphinx_basic_ng/theme/basic-ng/domainindex.html
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     1610 2022-03-19 09:57:59.000000 sphinx_basic_ng-1.0.0b2/src/sphinx_basic_ng/theme/basic-ng/genindex-single.html
+-rw-r--r--   0 pradyunsg   (501) staff       (20)      807 2022-03-19 09:58:19.000000 sphinx_basic_ng-1.0.0b2/src/sphinx_basic_ng/theme/basic-ng/genindex-split.html
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     1823 2022-03-19 09:58:42.000000 sphinx_basic_ng-1.0.0b2/src/sphinx_basic_ng/theme/basic-ng/genindex.html
+-rw-r--r--   0 pradyunsg   (501) staff       (20)       60 2021-11-21 11:08:51.000000 sphinx_basic_ng-1.0.0b2/src/sphinx_basic_ng/theme/basic-ng/globaltoc.html
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     2149 2022-01-05 08:21:13.000000 sphinx_basic_ng-1.0.0b2/src/sphinx_basic_ng/theme/basic-ng/layout.html
+-rw-r--r--   0 pradyunsg   (501) staff       (20)       59 2021-11-21 11:08:51.000000 sphinx_basic_ng-1.0.0b2/src/sphinx_basic_ng/theme/basic-ng/localtoc.html
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     2788 2022-06-27 21:11:48.000000 sphinx_basic_ng-1.0.0b2/src/sphinx_basic_ng/theme/basic-ng/page.html
+-rw-r--r--   0 pradyunsg   (501) staff       (20)       60 2021-11-21 11:08:51.000000 sphinx_basic_ng-1.0.0b2/src/sphinx_basic_ng/theme/basic-ng/relations.html
+-rw-r--r--   0 pradyunsg   (501) staff       (20)      934 2022-01-23 11:31:12.000000 sphinx_basic_ng-1.0.0b2/src/sphinx_basic_ng/theme/basic-ng/search.html
+-rw-r--r--   0 pradyunsg   (501) staff       (20)       60 2021-11-21 11:08:51.000000 sphinx_basic_ng-1.0.0b2/src/sphinx_basic_ng/theme/basic-ng/searchbox.html
+drwxr-xr-x   0 pradyunsg   (501) staff       (20)        0 2023-07-08 18:40:43.702021 sphinx_basic_ng-1.0.0b2/src/sphinx_basic_ng/theme/basic-ng/sections/
+-rw-r--r--   0 pradyunsg   (501) staff       (20)       27 2021-07-09 14:03:31.000000 sphinx_basic_ng-1.0.0b2/src/sphinx_basic_ng/theme/basic-ng/sections/announcement.html
+-rw-r--r--   0 pradyunsg   (501) staff       (20)      810 2021-07-09 14:03:31.000000 sphinx_basic_ng-1.0.0b2/src/sphinx_basic_ng/theme/basic-ng/sections/article.html
+-rw-r--r--   0 pradyunsg   (501) staff       (20)       29 2021-07-09 14:03:31.000000 sphinx_basic_ng-1.0.0b2/src/sphinx_basic_ng/theme/basic-ng/sections/footer-article.html
+-rw-r--r--   0 pradyunsg   (501) staff       (20)       29 2021-07-09 14:03:31.000000 sphinx_basic_ng-1.0.0b2/src/sphinx_basic_ng/theme/basic-ng/sections/footer-content.html
+-rw-r--r--   0 pradyunsg   (501) staff       (20)       21 2021-07-09 14:03:31.000000 sphinx_basic_ng-1.0.0b2/src/sphinx_basic_ng/theme/basic-ng/sections/footer.html
+-rw-r--r--   0 pradyunsg   (501) staff       (20)       29 2021-07-10 19:00:17.000000 sphinx_basic_ng-1.0.0b2/src/sphinx_basic_ng/theme/basic-ng/sections/header-article.html
+-rw-r--r--   0 pradyunsg   (501) staff       (20)       29 2022-01-23 11:33:05.000000 sphinx_basic_ng-1.0.0b2/src/sphinx_basic_ng/theme/basic-ng/sections/header-content.html
+-rw-r--r--   0 pradyunsg   (501) staff       (20)       31 2021-07-09 14:03:31.000000 sphinx_basic_ng-1.0.0b2/src/sphinx_basic_ng/theme/basic-ng/sections/header-secondary.html
+-rw-r--r--   0 pradyunsg   (501) staff       (20)       21 2021-07-11 12:14:07.000000 sphinx_basic_ng-1.0.0b2/src/sphinx_basic_ng/theme/basic-ng/sections/header.html
+-rw-r--r--   0 pradyunsg   (501) staff       (20)       30 2021-07-09 14:03:31.000000 sphinx_basic_ng-1.0.0b2/src/sphinx_basic_ng/theme/basic-ng/sections/sidebar-primary.html
+-rw-r--r--   0 pradyunsg   (501) staff       (20)       32 2021-07-09 14:03:31.000000 sphinx_basic_ng-1.0.0b2/src/sphinx_basic_ng/theme/basic-ng/sections/sidebar-secondary.html
+-rw-r--r--   0 pradyunsg   (501) staff       (20)       61 2021-11-21 11:08:51.000000 sphinx_basic_ng-1.0.0b2/src/sphinx_basic_ng/theme/basic-ng/sourcelink.html
+drwxr-xr-x   0 pradyunsg   (501) staff       (20)        0 2023-07-08 18:40:43.703352 sphinx_basic_ng-1.0.0b2/src/sphinx_basic_ng/theme/basic-ng/static/
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     1266 2022-06-27 21:12:25.000000 sphinx_basic_ng-1.0.0b2/src/sphinx_basic_ng/theme/basic-ng/static/debug.css
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     6034 2022-06-27 21:11:51.000000 sphinx_basic_ng-1.0.0b2/src/sphinx_basic_ng/theme/basic-ng/static/skeleton.css
+-rw-r--r--   0 pradyunsg   (501) staff       (20)       69 2021-07-09 14:03:31.000000 sphinx_basic_ng-1.0.0b2/src/sphinx_basic_ng/theme/basic-ng/theme.conf
+drwxr-xr-x   0 pradyunsg   (501) staff       (20)        0 2023-07-08 18:40:43.688406 sphinx_basic_ng-1.0.0b2/src/sphinx_basic_ng.egg-info/
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     1211 2023-07-08 18:40:43.000000 sphinx_basic_ng-1.0.0b2/src/sphinx_basic_ng.egg-info/PKG-INFO
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     3246 2023-07-08 18:40:43.000000 sphinx_basic_ng-1.0.0b2/src/sphinx_basic_ng.egg-info/SOURCES.txt
+-rw-r--r--   0 pradyunsg   (501) staff       (20)        1 2023-07-08 18:40:43.000000 sphinx_basic_ng-1.0.0b2/src/sphinx_basic_ng.egg-info/dependency_links.txt
+-rw-r--r--   0 pradyunsg   (501) staff       (20)       48 2023-07-08 18:40:43.000000 sphinx_basic_ng-1.0.0b2/src/sphinx_basic_ng.egg-info/entry_points.txt
+-rw-r--r--   0 pradyunsg   (501) staff       (20)       82 2023-07-08 18:40:43.000000 sphinx_basic_ng-1.0.0b2/src/sphinx_basic_ng.egg-info/requires.txt
+-rw-r--r--   0 pradyunsg   (501) staff       (20)       16 2023-07-08 18:40:43.000000 sphinx_basic_ng-1.0.0b2/src/sphinx_basic_ng.egg-info/top_level.txt
```

### Comparing `sphinx_basic_ng-1.0.0b1/LICENSE` & `sphinx_basic_ng-1.0.0b2/LICENSE`

 * *Files identical despite different names*

### Comparing `sphinx_basic_ng-1.0.0b1/PKG-INFO` & `sphinx_basic_ng-1.0.0b2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphinx_basic_ng
-Version: 1.0.0b1
+Version: 1.0.0b2
 Summary: A modern skeleton for Sphinx themes.
 Home-page: https://github.com/pradyunsg/sphinx-basic-ng
 Author: Pradyun Gedam
 Author-email: mail@pradyunsg.me
 Project-URL: Documentation, https://rtfd.io/sphinx-basic-ng/
 Classifier: Framework :: Sphinx
 Classifier: Framework :: Sphinx :: Theme
```

### Comparing `sphinx_basic_ng-1.0.0b1/docs/changelog.md` & `sphinx_basic_ng-1.0.0b2/docs/changelog.md`

 * *Files identical despite different names*

### Comparing `sphinx_basic_ng-1.0.0b1/docs/conf.py` & `sphinx_basic_ng-1.0.0b2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `sphinx_basic_ng-1.0.0b1/docs/expectations.md` & `sphinx_basic_ng-1.0.0b2/docs/expectations.md`

 * *Files identical despite different names*

### Comparing `sphinx_basic_ng-1.0.0b1/docs/goals.md` & `sphinx_basic_ng-1.0.0b2/docs/goals.md`

 * *Files identical despite different names*

### Comparing `sphinx_basic_ng-1.0.0b1/docs/usage/components/breadcrumbs.md` & `sphinx_basic_ng-1.0.0b2/docs/usage/components/breadcrumbs.md`

 * *Files identical despite different names*

### Comparing `sphinx_basic_ng-1.0.0b1/docs/usage/components/edit-this-page.md` & `sphinx_basic_ng-1.0.0b2/docs/usage/components/edit-this-page.md`

 * *Files identical despite different names*

### Comparing `sphinx_basic_ng-1.0.0b1/docs/usage/components/ethical-ads.md` & `sphinx_basic_ng-1.0.0b2/docs/usage/components/ethical-ads.md`

 * *Files identical despite different names*

### Comparing `sphinx_basic_ng-1.0.0b1/docs/usage/components/related-pages.md` & `sphinx_basic_ng-1.0.0b2/docs/usage/components/related-pages.md`

 * *Files identical despite different names*

### Comparing `sphinx_basic_ng-1.0.0b1/docs/usage/components/search-hide.md` & `sphinx_basic_ng-1.0.0b2/docs/usage/components/search-hide.md`

 * *Files identical despite different names*

### Comparing `sphinx_basic_ng-1.0.0b1/docs/usage/components/search-input.md` & `sphinx_basic_ng-1.0.0b2/docs/usage/components/search-input.md`

 * *Files identical despite different names*

### Comparing `sphinx_basic_ng-1.0.0b1/docs/usage/components/sidebar-toggles.md` & `sphinx_basic_ng-1.0.0b2/docs/usage/components/sidebar-toggles.md`

 * *Files identical despite different names*

### Comparing `sphinx_basic_ng-1.0.0b1/docs/usage/components/view-this-page.md` & `sphinx_basic_ng-1.0.0b2/docs/usage/components/view-this-page.md`

 * *Files identical despite different names*

### Comparing `sphinx_basic_ng-1.0.0b1/setup.cfg` & `sphinx_basic_ng-1.0.0b2/setup.cfg`

 * *Files identical despite different names*

### Comparing `sphinx_basic_ng-1.0.0b1/src/sphinx_basic_ng/__init__.py` & `sphinx_basic_ng-1.0.0b2/src/sphinx_basic_ng/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """A modern skeleton for Sphinx themes."""
 
-__version__ = "1.0.0.beta1"
+__version__ = "1.0.0.beta2"
 
 from pathlib import Path
 from typing import Any, Dict
 
 from sphinx.application import Sphinx
 
 _THEME_PATH = (Path(__file__).parent / "theme" / "basic-ng").resolve()
```

### Comparing `sphinx_basic_ng-1.0.0b1/src/sphinx_basic_ng/theme/basic-ng/components/breadcrumbs.html` & `sphinx_basic_ng-1.0.0b2/src/sphinx_basic_ng/theme/basic-ng/components/breadcrumbs.html`

 * *Files identical despite different names*

### Comparing `sphinx_basic_ng-1.0.0b1/src/sphinx_basic_ng/theme/basic-ng/components/edit-this-page.html` & `sphinx_basic_ng-1.0.0b2/src/sphinx_basic_ng/theme/basic-ng/components/edit-this-page.html`

 * *Files identical despite different names*

### Comparing `sphinx_basic_ng-1.0.0b1/src/sphinx_basic_ng/theme/basic-ng/components/related-pages.html` & `sphinx_basic_ng-1.0.0b2/src/sphinx_basic_ng/theme/basic-ng/components/related-pages.html`

 * *Files identical despite different names*

### Comparing `sphinx_basic_ng-1.0.0b1/src/sphinx_basic_ng/theme/basic-ng/components/toggle-sidebar-primary.html` & `sphinx_basic_ng-1.0.0b2/src/sphinx_basic_ng/theme/basic-ng/components/toggle-sidebar-primary.html`

 * *Files identical despite different names*

### Comparing `sphinx_basic_ng-1.0.0b1/src/sphinx_basic_ng/theme/basic-ng/components/toggle-sidebar-secondary.html` & `sphinx_basic_ng-1.0.0b2/src/sphinx_basic_ng/theme/basic-ng/components/toggle-sidebar-secondary.html`

 * *Files identical despite different names*

### Comparing `sphinx_basic_ng-1.0.0b1/src/sphinx_basic_ng/theme/basic-ng/components/view-this-page.html` & `sphinx_basic_ng-1.0.0b2/src/sphinx_basic_ng/theme/basic-ng/components/view-this-page.html`

 * *Files 4% similar despite different names*

```diff
@@ -39,15 +39,14 @@
         "Could not understand `source_repository` provided: " + repo + "\n" +
         "You should set `source_view_link`, so that the view link is presented."
       ) }}
     {%- endif -%}
   {%- elif show_source and has_source -%}
     {{ pathto('_sources/' + sourcename, true) }}
   {%- endif -%}
-  {%- endif -%}
 {%- endmacro -%}
 
 
 {%- if page_source_suffix -%}
   {%- set can_find_view_link = (
     (theme_source_view_link and pagename)
     or (show_source and has_source and sourcename)
```

#### html2text {}

```diff
@@ -16,14 +16,14 @@
 { document_path }}?plain=true {%- elif repo.startswith("https://gitlab.com/") -
 %} {{ repo }}/blob/{{ branch }}/{{ document_path }} {%- elif repo.startswith
 ("https://bitbucket.org/") -%} {{ repo }}/src/{{ branch }}/{{ document_path }}
 {#- Fail with a warning -#} {%- else -%} {{ warning( "Could not understand
 `source_repository` provided: " + repo + "\n" + "You should set
 `source_view_link`, so that the view link is presented." ) }} {%- endif -%} {%-
 elif show_source and has_source -%} {{ pathto('_sources/' + sourcename, true)
-}} {%- endif -%} {%- endif -%} {%- endmacro -%} {%- if page_source_suffix -%}
-{%- set can_find_view_link = ( (theme_source_view_link and pagename) or
-(show_source and has_source and sourcename) or (theme_source_repository and
+}} {%- endif -%} {%- endmacro -%} {%- if page_source_suffix -%} {%- set
+can_find_view_link = ( (theme_source_view_link and pagename) or (show_source
+and has_source and sourcename) or (theme_source_repository and
 theme_source_branch) ) -%} {%- if can_find_view_link -%} {%- block
 link_available -%} {{__("View_sources")_}} {%- endblock link_available -%} {%-
 else -%} {%- block link_not_available -%}{%- endblock -%} {%- endif -%} {%-
 endif -%}
```

### Comparing `sphinx_basic_ng-1.0.0b1/src/sphinx_basic_ng/theme/basic-ng/domainindex.html` & `sphinx_basic_ng-1.0.0b2/src/sphinx_basic_ng/theme/basic-ng/domainindex.html`

 * *Files identical despite different names*

### Comparing `sphinx_basic_ng-1.0.0b1/src/sphinx_basic_ng/theme/basic-ng/genindex-single.html` & `sphinx_basic_ng-1.0.0b2/src/sphinx_basic_ng/theme/basic-ng/genindex-single.html`

 * *Files identical despite different names*

### Comparing `sphinx_basic_ng-1.0.0b1/src/sphinx_basic_ng/theme/basic-ng/genindex-split.html` & `sphinx_basic_ng-1.0.0b2/src/sphinx_basic_ng/theme/basic-ng/genindex-split.html`

 * *Files identical despite different names*

### Comparing `sphinx_basic_ng-1.0.0b1/src/sphinx_basic_ng/theme/basic-ng/genindex.html` & `sphinx_basic_ng-1.0.0b2/src/sphinx_basic_ng/theme/basic-ng/genindex.html`

 * *Files identical despite different names*

### Comparing `sphinx_basic_ng-1.0.0b1/src/sphinx_basic_ng/theme/basic-ng/layout.html` & `sphinx_basic_ng-1.0.0b2/src/sphinx_basic_ng/theme/basic-ng/layout.html`

 * *Files identical despite different names*

### Comparing `sphinx_basic_ng-1.0.0b1/src/sphinx_basic_ng/theme/basic-ng/page.html` & `sphinx_basic_ng-1.0.0b2/src/sphinx_basic_ng/theme/basic-ng/page.html`

 * *Files identical despite different names*

### Comparing `sphinx_basic_ng-1.0.0b1/src/sphinx_basic_ng/theme/basic-ng/search.html` & `sphinx_basic_ng-1.0.0b2/src/sphinx_basic_ng/theme/basic-ng/search.html`

 * *Files identical despite different names*

### Comparing `sphinx_basic_ng-1.0.0b1/src/sphinx_basic_ng/theme/basic-ng/sections/article.html` & `sphinx_basic_ng-1.0.0b2/src/sphinx_basic_ng/theme/basic-ng/sections/article.html`

 * *Files identical despite different names*

### Comparing `sphinx_basic_ng-1.0.0b1/src/sphinx_basic_ng/theme/basic-ng/static/debug.css` & `sphinx_basic_ng-1.0.0b2/src/sphinx_basic_ng/theme/basic-ng/static/debug.css`

 * *Files identical despite different names*

### Comparing `sphinx_basic_ng-1.0.0b1/src/sphinx_basic_ng/theme/basic-ng/static/skeleton.css` & `sphinx_basic_ng-1.0.0b2/src/sphinx_basic_ng/theme/basic-ng/static/skeleton.css`

 * *Files identical despite different names*

### Comparing `sphinx_basic_ng-1.0.0b1/src/sphinx_basic_ng.egg-info/PKG-INFO` & `sphinx_basic_ng-1.0.0b2/src/sphinx_basic_ng.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphinx-basic-ng
-Version: 1.0.0b1
+Version: 1.0.0b2
 Summary: A modern skeleton for Sphinx themes.
 Home-page: https://github.com/pradyunsg/sphinx-basic-ng
 Author: Pradyun Gedam
 Author-email: mail@pradyunsg.me
 Project-URL: Documentation, https://rtfd.io/sphinx-basic-ng/
 Classifier: Framework :: Sphinx
 Classifier: Framework :: Sphinx :: Theme
```

### Comparing `sphinx_basic_ng-1.0.0b1/src/sphinx_basic_ng.egg-info/SOURCES.txt` & `sphinx_basic_ng-1.0.0b2/src/sphinx_basic_ng.egg-info/SOURCES.txt`

 * *Files identical despite different names*

