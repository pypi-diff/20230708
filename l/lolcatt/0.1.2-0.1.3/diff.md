# Comparing `tmp/lolcatt-0.1.2.tar.gz` & `tmp/lolcatt-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lolcatt-0.1.2.tar", last modified: Tue Jul  4 22:04:20 2023, max compression
+gzip compressed data, was "lolcatt-0.1.3.tar", last modified: Sat Jul  8 19:44:58 2023, max compression
```

## Comparing `lolcatt-0.1.2.tar` & `lolcatt-0.1.3.tar`

### file list

```diff
@@ -1,82 +1,63 @@
-drwxrwxr-x   0 atav1st   (1000) atav1st   (1000)        0 2023-07-04 22:04:20.257699 lolcatt-0.1.2/
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)       28 2023-07-02 11:51:34.000000 lolcatt-0.1.2/.coveragerc
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      318 2023-07-02 11:51:34.000000 lolcatt-0.1.2/.editorconfig
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      184 2023-07-02 11:51:34.000000 lolcatt-0.1.2/.flake8
-drwxrwxr-x   0 atav1st   (1000) atav1st   (1000)        0 2023-07-04 22:04:20.253698 lolcatt-0.1.2/.github/
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      324 2023-07-02 11:51:34.000000 lolcatt-0.1.2/.github/ISSUE_TEMPLATE.md
-drwxrwxr-x   0 atav1st   (1000) atav1st   (1000)        0 2023-07-04 22:04:20.253698 lolcatt-0.1.2/.github/workflows/
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     2695 2023-07-02 11:51:34.000000 lolcatt-0.1.2/.github/workflows/ci.yml
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1589 2023-07-02 11:51:34.000000 lolcatt-0.1.2/.github/workflows/coverage.yml
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1707 2023-07-02 11:51:34.000000 lolcatt-0.1.2/.github/workflows/docs.yml
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1221 2023-07-02 11:51:34.000000 lolcatt-0.1.2/.gitignore
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1416 2023-07-02 11:51:34.000000 lolcatt-0.1.2/.pre-commit-config.yaml
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      708 2023-07-02 11:51:34.000000 lolcatt-0.1.2/Dockerfile
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1074 2023-07-02 11:51:34.000000 lolcatt-0.1.2/LICENSE
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      239 2023-07-02 11:51:34.000000 lolcatt-0.1.2/MANIFEST.in
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     3735 2023-07-02 11:51:34.000000 lolcatt-0.1.2/Makefile
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1987 2023-07-04 22:04:20.257699 lolcatt-0.1.2/PKG-INFO
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1308 2023-07-04 17:57:06.000000 lolcatt-0.1.2/README.rst
-drwxrwxr-x   0 atav1st   (1000) atav1st   (1000)        0 2023-07-04 22:04:20.253698 lolcatt-0.1.2/docs/
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      608 2023-07-02 11:51:34.000000 lolcatt-0.1.2/docs/Makefile
-drwxrwxr-x   0 atav1st   (1000) atav1st   (1000)        0 2023-07-04 22:04:20.249698 lolcatt-0.1.2/docs/_build/
-drwxrwxr-x   0 atav1st   (1000) atav1st   (1000)        0 2023-07-04 22:04:20.249698 lolcatt-0.1.2/docs/_build/html/
-drwxrwxr-x   0 atav1st   (1000) atav1st   (1000)        0 2023-07-04 22:04:20.257699 lolcatt-0.1.2/docs/_build/html/_static/
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)    14813 2023-07-04 21:53:55.000000 lolcatt-0.1.2/docs/_build/html/_static/basic.css
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)       84 2023-07-02 11:51:34.000000 lolcatt-0.1.2/docs/_build/html/_static/custom.css
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      286 2023-05-12 22:36:26.000000 lolcatt-0.1.2/docs/_build/html/_static/file.png
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)       90 2023-05-12 22:36:26.000000 lolcatt-0.1.2/docs/_build/html/_static/minus.png
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     4208 2023-07-04 21:53:55.000000 lolcatt-0.1.2/docs/_build/html/_static/nature.css
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)       90 2023-05-12 22:36:26.000000 lolcatt-0.1.2/docs/_build/html/_static/plus.png
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     4956 2023-07-04 21:53:55.000000 lolcatt-0.1.2/docs/_build/html/_static/pygments.css
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)    17073 2023-07-04 18:00:35.000000 lolcatt-0.1.2/docs/_build/html/_static/screenshot.png
-drwxrwxr-x   0 atav1st   (1000) atav1st   (1000)        0 2023-07-04 22:04:20.257699 lolcatt-0.1.2/docs/_static/
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)       84 2023-07-02 11:51:34.000000 lolcatt-0.1.2/docs/_static/custom.css
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)    17073 2023-07-04 18:00:35.000000 lolcatt-0.1.2/docs/_static/screenshot.png
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     4983 2023-07-04 12:57:37.000000 lolcatt-0.1.2/docs/conf.py
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      264 2023-07-02 11:51:34.000000 lolcatt-0.1.2/docs/index.rst
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1138 2023-07-02 11:51:34.000000 lolcatt-0.1.2/docs/installation.rst
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      346 2023-07-04 12:55:04.000000 lolcatt-0.1.2/docs/lolcatt.casting.rst
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      517 2023-07-04 21:53:52.000000 lolcatt-0.1.2/docs/lolcatt.rst
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1232 2023-07-04 12:55:04.000000 lolcatt-0.1.2/docs/lolcatt.ui.rst
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      331 2023-07-04 12:55:04.000000 lolcatt-0.1.2/docs/lolcatt.utils.rst
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      805 2023-07-02 11:51:34.000000 lolcatt-0.1.2/docs/make.bat
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)       58 2023-07-04 21:53:52.000000 lolcatt-0.1.2/docs/modules.rst
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)       27 2023-07-02 11:51:34.000000 lolcatt-0.1.2/docs/readme.rst
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)       69 2023-07-02 11:51:34.000000 lolcatt-0.1.2/docs/usage.rst
-drwxrwxr-x   0 atav1st   (1000) atav1st   (1000)        0 2023-07-04 22:04:20.257699 lolcatt-0.1.2/lolcatt/
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      125 2023-07-04 21:50:56.000000 lolcatt-0.1.2/lolcatt/__init__.py
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1142 2023-07-04 21:40:08.000000 lolcatt-0.1.2/lolcatt/app.py
-drwxrwxr-x   0 atav1st   (1000) atav1st   (1000)        0 2023-07-04 22:04:20.257699 lolcatt-0.1.2/lolcatt/casting/
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)        0 2023-07-04 11:20:23.000000 lolcatt-0.1.2/lolcatt/casting/__init__.py
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     5545 2023-07-04 21:58:28.000000 lolcatt-0.1.2/lolcatt/casting/caster.py
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1072 2023-07-04 21:27:39.000000 lolcatt-0.1.2/lolcatt/cli.py
-drwxrwxr-x   0 atav1st   (1000) atav1st   (1000)        0 2023-07-04 22:04:20.257699 lolcatt-0.1.2/lolcatt/ui/
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)        0 2023-07-04 11:20:23.000000 lolcatt-0.1.2/lolcatt/ui/__init__.py
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      323 2023-07-04 21:27:39.000000 lolcatt-0.1.2/lolcatt/ui/caster_static.py
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1442 2023-07-04 15:41:48.000000 lolcatt-0.1.2/lolcatt/ui/lolcatt.css
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     3616 2023-07-04 16:07:21.000000 lolcatt-0.1.2/lolcatt/ui/lolcatt_controls.py
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1258 2023-07-04 21:27:39.000000 lolcatt-0.1.2/lolcatt/ui/lolcatt_device_info.py
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1548 2023-07-04 21:52:43.000000 lolcatt-0.1.2/lolcatt/ui/lolcatt_playback_info.py
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     2378 2023-07-04 20:17:28.000000 lolcatt-0.1.2/lolcatt/ui/lolcatt_progress.py
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      765 2023-07-04 13:34:42.000000 lolcatt-0.1.2/lolcatt/ui/lolcatt_url_input.py
-drwxrwxr-x   0 atav1st   (1000) atav1st   (1000)        0 2023-07-04 22:04:20.257699 lolcatt-0.1.2/lolcatt/utils/
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)        0 2023-07-04 12:53:13.000000 lolcatt-0.1.2/lolcatt/utils/__init__.py
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1472 2023-07-04 21:45:55.000000 lolcatt-0.1.2/lolcatt/utils/utils.py
-drwxrwxr-x   0 atav1st   (1000) atav1st   (1000)        0 2023-07-04 22:04:20.257699 lolcatt-0.1.2/lolcatt.egg-info/
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1987 2023-07-04 22:04:20.000000 lolcatt-0.1.2/lolcatt.egg-info/PKG-INFO
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1527 2023-07-04 22:04:20.000000 lolcatt-0.1.2/lolcatt.egg-info/SOURCES.txt
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)        1 2023-07-04 22:04:20.000000 lolcatt-0.1.2/lolcatt.egg-info/dependency_links.txt
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)       45 2023-07-04 22:04:20.000000 lolcatt-0.1.2/lolcatt.egg-info/entry_points.txt
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)        1 2023-07-04 22:04:20.000000 lolcatt-0.1.2/lolcatt.egg-info/not-zip-safe
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)       49 2023-07-04 22:04:20.000000 lolcatt-0.1.2/lolcatt.egg-info/requires.txt
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)        8 2023-07-04 22:04:20.000000 lolcatt-0.1.2/lolcatt.egg-info/top_level.txt
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      558 2023-07-04 21:50:56.000000 lolcatt-0.1.2/pyproject.toml
-drwxrwxr-x   0 atav1st   (1000) atav1st   (1000)        0 2023-07-04 22:04:20.257699 lolcatt-0.1.2/requirements/
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      243 2023-07-04 22:01:38.000000 lolcatt-0.1.2/requirements/dev.txt
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)       49 2023-07-04 20:19:58.000000 lolcatt-0.1.2/requirements/prod.txt
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)       44 2023-07-02 11:51:34.000000 lolcatt-0.1.2/requirements/test.txt
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      354 2023-07-04 22:04:20.261699 lolcatt-0.1.2/setup.cfg
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1556 2023-07-04 21:50:56.000000 lolcatt-0.1.2/setup.py
-drwxrwxr-x   0 atav1st   (1000) atav1st   (1000)        0 2023-07-04 22:04:20.257699 lolcatt-0.1.2/tests/
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)       37 2023-07-02 11:51:34.000000 lolcatt-0.1.2/tests/__init__.py
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      211 2023-07-04 21:49:29.000000 lolcatt-0.1.2/tests/test_lolcatt.py
+drwxrwxr-x   0 atav1st   (1000) atav1st   (1000)        0 2023-07-08 19:44:58.191541 lolcatt-0.1.3/
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1074 2023-06-30 16:54:52.000000 lolcatt-0.1.3/LICENSE
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      239 2023-06-30 20:26:17.000000 lolcatt-0.1.3/MANIFEST.in
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1987 2023-07-08 19:44:58.191541 lolcatt-0.1.3/PKG-INFO
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1308 2023-07-07 17:09:03.000000 lolcatt-0.1.3/README.rst
+drwxrwxr-x   0 atav1st   (1000) atav1st   (1000)        0 2023-07-08 19:44:58.135541 lolcatt-0.1.3/docs/
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      608 2023-06-30 16:54:52.000000 lolcatt-0.1.3/docs/Makefile
+drwxrwxr-x   0 atav1st   (1000) atav1st   (1000)        0 2023-07-08 19:44:58.075541 lolcatt-0.1.3/docs/_build/
+drwxrwxr-x   0 atav1st   (1000) atav1st   (1000)        0 2023-07-08 19:44:58.075541 lolcatt-0.1.3/docs/_build/html/
+drwxrwxr-x   0 atav1st   (1000) atav1st   (1000)        0 2023-07-08 19:44:58.151541 lolcatt-0.1.3/docs/_build/html/_static/
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)    14813 2023-07-04 00:19:31.000000 lolcatt-0.1.3/docs/_build/html/_static/basic.css
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)       84 2023-06-30 16:54:52.000000 lolcatt-0.1.3/docs/_build/html/_static/custom.css
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      286 2023-05-12 22:36:26.000000 lolcatt-0.1.3/docs/_build/html/_static/file.png
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)       90 2023-05-12 22:36:26.000000 lolcatt-0.1.3/docs/_build/html/_static/minus.png
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     4208 2023-07-04 00:19:31.000000 lolcatt-0.1.3/docs/_build/html/_static/nature.css
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)       90 2023-05-12 22:36:26.000000 lolcatt-0.1.3/docs/_build/html/_static/plus.png
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     4956 2023-07-04 00:19:31.000000 lolcatt-0.1.3/docs/_build/html/_static/pygments.css
+drwxrwxr-x   0 atav1st   (1000) atav1st   (1000)        0 2023-07-08 19:44:58.159541 lolcatt-0.1.3/docs/_static/
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)       84 2023-06-30 16:54:52.000000 lolcatt-0.1.3/docs/_static/custom.css
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)    17073 2023-07-07 17:09:03.000000 lolcatt-0.1.3/docs/_static/screenshot.png
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     4983 2023-06-30 21:18:35.000000 lolcatt-0.1.3/docs/conf.py
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      264 2023-06-30 16:54:52.000000 lolcatt-0.1.3/docs/index.rst
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1138 2023-06-30 16:54:52.000000 lolcatt-0.1.3/docs/installation.rst
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      346 2023-07-07 17:09:03.000000 lolcatt-0.1.3/docs/lolcatt.casting.rst
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      517 2023-07-07 17:09:03.000000 lolcatt-0.1.3/docs/lolcatt.rst
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1232 2023-07-07 17:09:03.000000 lolcatt-0.1.3/docs/lolcatt.ui.rst
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      331 2023-07-07 17:09:03.000000 lolcatt-0.1.3/docs/lolcatt.utils.rst
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      805 2023-06-30 16:54:52.000000 lolcatt-0.1.3/docs/make.bat
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)       58 2023-07-04 00:19:25.000000 lolcatt-0.1.3/docs/modules.rst
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)       27 2023-06-30 16:54:52.000000 lolcatt-0.1.3/docs/readme.rst
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)       69 2023-06-30 16:54:52.000000 lolcatt-0.1.3/docs/usage.rst
+drwxrwxr-x   0 atav1st   (1000) atav1st   (1000)        0 2023-07-08 19:44:58.183541 lolcatt-0.1.3/lolcatt/
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      125 2023-07-08 19:38:10.000000 lolcatt-0.1.3/lolcatt/__init__.py
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1206 2023-07-08 19:31:59.000000 lolcatt-0.1.3/lolcatt/app.py
+drwxrwxr-x   0 atav1st   (1000) atav1st   (1000)        0 2023-07-08 19:44:58.187541 lolcatt-0.1.3/lolcatt/casting/
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)        0 2023-07-03 23:40:52.000000 lolcatt-0.1.3/lolcatt/casting/__init__.py
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     5421 2023-07-08 19:31:59.000000 lolcatt-0.1.3/lolcatt/casting/caster.py
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1079 2023-07-08 19:35:39.000000 lolcatt-0.1.3/lolcatt/cli.py
+drwxrwxr-x   0 atav1st   (1000) atav1st   (1000)        0 2023-07-08 19:44:58.191541 lolcatt-0.1.3/lolcatt/ui/
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)        0 2023-07-03 23:40:52.000000 lolcatt-0.1.3/lolcatt/ui/__init__.py
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1442 2023-07-08 19:31:59.000000 lolcatt-0.1.3/lolcatt/ui/lolcatt.css
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     3492 2023-07-07 17:09:03.000000 lolcatt-0.1.3/lolcatt/ui/lolcatt_controls.py
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1265 2023-07-07 17:09:03.000000 lolcatt-0.1.3/lolcatt/ui/lolcatt_device_info.py
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1561 2023-07-08 19:31:59.000000 lolcatt-0.1.3/lolcatt/ui/lolcatt_playback_info.py
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     2368 2023-07-07 17:09:03.000000 lolcatt-0.1.3/lolcatt/ui/lolcatt_progress.py
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      746 2023-07-08 19:31:59.000000 lolcatt-0.1.3/lolcatt/ui/lolcatt_url_input.py
+drwxrwxr-x   0 atav1st   (1000) atav1st   (1000)        0 2023-07-08 19:44:58.191541 lolcatt-0.1.3/lolcatt/utils/
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)        0 2023-07-07 17:09:03.000000 lolcatt-0.1.3/lolcatt/utils/__init__.py
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1472 2023-07-07 17:09:03.000000 lolcatt-0.1.3/lolcatt/utils/utils.py
+drwxrwxr-x   0 atav1st   (1000) atav1st   (1000)        0 2023-07-08 19:44:58.187541 lolcatt-0.1.3/lolcatt.egg-info/
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1987 2023-07-08 19:44:57.000000 lolcatt-0.1.3/lolcatt.egg-info/PKG-INFO
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1196 2023-07-08 19:44:58.000000 lolcatt-0.1.3/lolcatt.egg-info/SOURCES.txt
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)        1 2023-07-08 19:44:57.000000 lolcatt-0.1.3/lolcatt.egg-info/dependency_links.txt
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)       45 2023-07-08 19:44:57.000000 lolcatt-0.1.3/lolcatt.egg-info/entry_points.txt
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)        1 2023-07-07 17:15:34.000000 lolcatt-0.1.3/lolcatt.egg-info/not-zip-safe
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)       49 2023-07-08 19:44:57.000000 lolcatt-0.1.3/lolcatt.egg-info/requires.txt
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)        8 2023-07-08 19:44:57.000000 lolcatt-0.1.3/lolcatt.egg-info/top_level.txt
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      558 2023-07-08 19:38:10.000000 lolcatt-0.1.3/pyproject.toml
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      354 2023-07-08 19:44:58.191541 lolcatt-0.1.3/setup.cfg
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1556 2023-07-08 19:38:10.000000 lolcatt-0.1.3/setup.py
+drwxrwxr-x   0 atav1st   (1000) atav1st   (1000)        0 2023-07-08 19:44:58.191541 lolcatt-0.1.3/tests/
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)       37 2023-06-30 16:54:52.000000 lolcatt-0.1.3/tests/__init__.py
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      211 2023-07-07 17:09:03.000000 lolcatt-0.1.3/tests/test_lolcatt.py
```

### Comparing `lolcatt-0.1.2/LICENSE` & `lolcatt-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `lolcatt-0.1.2/PKG-INFO` & `lolcatt-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lolcatt
-Version: 0.1.2
+Version: 0.1.3
 Summary: A TUI wrapper around `catt`.
 Home-page: https://github.com/LokiLuciferase/lolcatt
 Author: Lukas Lüftinger
 Author-email: lukas.lueftinger@outlook.com
 License: MIT license
 Keywords: lolcatt
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `lolcatt-0.1.2/README.rst` & `lolcatt-0.1.3/README.rst`

 * *Files identical despite different names*

### Comparing `lolcatt-0.1.2/docs/Makefile` & `lolcatt-0.1.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `lolcatt-0.1.2/docs/_build/html/_static/basic.css` & `lolcatt-0.1.3/docs/_build/html/_static/basic.css`

 * *Files identical despite different names*

### Comparing `lolcatt-0.1.2/docs/_build/html/_static/nature.css` & `lolcatt-0.1.3/docs/_build/html/_static/nature.css`

 * *Files identical despite different names*

### Comparing `lolcatt-0.1.2/docs/_build/html/_static/pygments.css` & `lolcatt-0.1.3/docs/_build/html/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `lolcatt-0.1.2/docs/_build/html/_static/screenshot.png` & `lolcatt-0.1.3/docs/_static/screenshot.png`

 * *Files identical despite different names*

### Comparing `lolcatt-0.1.2/docs/conf.py` & `lolcatt-0.1.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `lolcatt-0.1.2/docs/installation.rst` & `lolcatt-0.1.3/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `lolcatt-0.1.2/docs/lolcatt.rst` & `lolcatt-0.1.3/docs/lolcatt.rst`

 * *Files identical despite different names*

### Comparing `lolcatt-0.1.2/docs/lolcatt.ui.rst` & `lolcatt-0.1.3/docs/lolcatt.ui.rst`

 * *Files identical despite different names*

### Comparing `lolcatt-0.1.2/docs/make.bat` & `lolcatt-0.1.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `lolcatt-0.1.2/lolcatt/casting/caster.py` & `lolcatt-0.1.3/lolcatt/casting/caster.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 #!/usr/bin/env python3
 import subprocess
-import sys
 import time
 from dataclasses import dataclass
 from typing import List
 from typing import Optional
 
 from catt.api import CattDevice
 from catt.api import discover
@@ -32,46 +31,20 @@
     CAST_ARGS = ['-f']
 
     def __init__(self, name_or_alias: Optional[str] = 'default', update_interval: float = 0.5):
         self._device = None
         self._available_devices = None
         self._catt_call = None
         self._catt_config = get_config_as_dict()
-        if name_or_alias == 'default':
-            self._device_name = self._catt_config['options'].get('device')
-            if self._device_name is None:
-                print(
-                    'No default device set. '
-                    'Scanning for all available devices and picking first...'
-                )
-                print(
-                    'To skip this in the future, either pass a device name '
-                    'or set a default device in the catt config file.'
-                )
-                possible_devices = self.get_available_devices()
-                if len(possible_devices) > 0:
-                    self._device_name = possible_devices[0].name
-        elif name_or_alias is not None:
-            self._device_name = self._catt_config['aliases'].get(name_or_alias, name_or_alias)
-        else:
-            self._device_name = None
-
-        if self._device_name is not None:
-            try:
-                self._device = CattDevice(self._device_name)
-            except CastError:
-                print(f'Selected device "{self._device_name}" was not found on this network.')
-                print('Scan for available devices using "lolcatt --scan".')
-                sys.exit(1)
-
+        self._loading_started = time.time()
+        self._is_loading_cast = True
+        self._loading_timeout = 8
         self._update_interval = update_interval
         self._state_last_updated = time.time()
-        self._loading_started = None
-        self._is_loading_cast = False
-        self._loading_timeout = 8
+        self.change_device(name_or_alias)
 
     def cast(self, url_or_path: str):
         """
         Casts the given url or path to the currently active device.
 
         :param url_or_path: The url or path to cast.
         """
@@ -100,27 +73,49 @@
         Runs Chromecast discovery and returns a list of available CattDevices.
 
         :return: A list of available CattDevices.
         """
         self._available_devices = discover()
         return self._available_devices
 
-    def change_device(self, name_or_alias: str):
+    def change_device(self, name_or_alias: str = None):
         """
         Changes the currently active device to the given name or alias. If the device is not
         available, a ValueError is raised.
 
         :param name_or_alias: The name or alias of the device to change to.
         """
-        self._device_name = self._catt_config['aliases'].get(name_or_alias, name_or_alias)
-        for device in self.get_available_devices():
-            if device.name == self._device_name:
-                self._device = device
-                return
-        raise ValueError('Can\'t change device: Device not found.')
+        if name_or_alias == 'default':
+            self._device_name = self._catt_config['options'].get('device')
+            if self._device_name is None:
+                print(
+                    'No default device set. '
+                    'Scanning for all available devices and picking first...'
+                )
+                print(
+                    'To skip this in the future, either pass a device name '
+                    'or set a default device in the catt config file.'
+                )
+                possible_devices = self.get_available_devices()
+                if len(possible_devices) > 0:
+                    self._device_name = possible_devices[0].name
+        elif name_or_alias is not None:
+            self._device_name = self._catt_config['aliases'].get(name_or_alias, name_or_alias)
+        else:
+            self._device_name = None
+
+        if self._device_name is not None:
+            try:
+                self._device = CattDevice(self._device_name)
+                self._loading_started = None
+                self._is_loading_cast = False
+            except CastError:
+                print(f'Selected device "{self._device_name}" was not found on this network.')
+                print('Scan for available devices using "lolcatt --scan".')
+                raise ValueError(f'No device with name or alias "{name_or_alias}" found.')
 
     def get_device(self) -> CattDevice:
         """
         Returns the currently active CattDevice.
 
         :return: The currently active CattDevice.
         """
```

### Comparing `lolcatt-0.1.2/lolcatt/cli.py` & `lolcatt-0.1.3/lolcatt/cli.py`

 * *Files 10% similar despite different names*

```diff
@@ -33,13 +33,13 @@
     """Cast media from a local file or URL to a Chromecast device."""
     if url_or_path is None and scan:
         do_scan()
         return
 
     lolcatt = LolCatt(device_name=device)
     if url_or_path is not None:
-        lolcatt.cast(url_or_path)
+        lolcatt.caster.cast(url_or_path)
     lolcatt.run()
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `lolcatt-0.1.2/lolcatt/ui/lolcatt.css` & `lolcatt-0.1.3/lolcatt/ui/lolcatt.css`

 * *Files identical despite different names*

### Comparing `lolcatt-0.1.2/lolcatt/ui/lolcatt_controls.py` & `lolcatt-0.1.3/lolcatt/ui/lolcatt_controls.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,27 @@
 from dataclasses import dataclass
-from typing import Callable
 
 from catt.cli import get_config_as_dict
 from catt.error import CastError
 from textual import on
 from textual.app import DEFAULT_COLORS
 from textual.containers import Container
 from textual.widgets import Button
-
-from lolcatt.ui.caster_static import CasterStatic
+from textual.widgets import Static
 
 
 @dataclass
 class ControlsConfig:
     ffwd_secs: int = 30
     rewind_secs: int = 10
     vol_step: float = 0.1
     use_utf8: bool = False
 
 
-class LolCattControls(CasterStatic):
+class LolCattControls(Static):
     CONTROLS = {
         'play_pause': '⏯',
         'stop': '⏹',
         'rewind': '⏪',
         'ffwd': '⏩',
         'vol_down': '',
         'vol_up': '',
@@ -34,27 +32,20 @@
         'stop': 'Stop',
         'rewind': 'RW',
         'ffwd': 'FW',
         'vol_down': 'Vol-',
         'vol_up': 'Vol+',
     }
 
-    def __init__(
-        self,
-        exit_cb: Callable,
-        *args,
-        **kwargs,
-    ):
+    def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self._config = ControlsConfig(
             use_utf8=get_config_as_dict()['options'].get('lolcatt_use_utf8', 'false').lower()
             == 'true'
         )
-        self._exit_func = exit_cb
-
         self._pp_button_colors = [DEFAULT_COLORS['dark'].success, DEFAULT_COLORS['dark'].warning]
         self._pp_button = Button(self._get_control_label('play_pause'), id='play_pause_button')
         self._pp_button.styles.border_bottom = ('tall', self._pp_button_colors[0])
         self._stop_button = Button(self._get_control_label('stop'), id='stop_button')
 
     def _get_control_label(self, control: str) -> str:
         if self._config.use_utf8:
@@ -75,41 +66,41 @@
             with Container(id='volume_buttons'):
                 yield Button(self._get_control_label('vol_down'), id='vol_down_button')
                 yield Button(self._get_control_label('vol_up'), id='vol_up_button')
 
     @on(Button.Pressed, "#play_pause_button")
     def toggle_play_pause(self):
         try:
-            self._caster.get_device().controller.play_toggle()
+            self.app.caster.get_device().controller.play_toggle()
             self._pp_button.styles.border_bottom = ('tall', self._pp_button_colors[-1])
             self._pp_button_colors.reverse()
         except ValueError:
             pass
 
     @on(Button.Pressed, "#stop_button")
     def stop(self):
-        if self._caster.get_cast_state().cast_info.get('player_state') in ['PLAYING', 'PAUSED']:
-            self._caster.get_device().stop()
+        if self.app.caster.get_cast_state().cast_info.get('player_state') in ['PLAYING', 'PAUSED']:
+            self.app.caster.get_device().stop()
         else:
-            self._exit_func()
+            self.app.exit()
 
     @on(Button.Pressed, "#vol_down_button")
     def vol_down(self):
-        self._caster.get_device().volumedown(self._config.vol_step)
+        self.app.caster.get_device().volumedown(self._config.vol_step)
 
     @on(Button.Pressed, "#vol_up_button")
     def vol_up(self):
-        self._caster.get_device().volumeup(self._config.vol_step)
+        self.app.caster.get_device().volumeup(self._config.vol_step)
 
     @on(Button.Pressed, "#ffwd_button")
     def ffwd(self):
         try:
-            self._caster.get_device().ffwd(self._config.ffwd_secs)
+            self.app.caster.get_device().ffwd(self._config.ffwd_secs)
         except CastError:
             pass
 
     @on(Button.Pressed, "#rewind_button")
     def rewind(self):
         try:
-            self._caster.get_device().rewind(self._config.rewind_secs)
+            self.app.caster.get_device().rewind(self._config.rewind_secs)
         except CastError:
             pass
```

### Comparing `lolcatt-0.1.2/lolcatt/ui/lolcatt_device_info.py` & `lolcatt-0.1.3/lolcatt/ui/lolcatt_device_info.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 from textual.containers import Container
 from textual.reactive import reactive
 from textual.widgets import Label
+from textual.widgets import Static
 
-from lolcatt.ui.caster_static import CasterStatic
 from lolcatt.utils.utils import marquee
 
 
-class LolCattDeviceInfo(CasterStatic):
+class LolCattDeviceInfo(Static):
     label_str = reactive('')
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.label = Label('')
         self._marquee_gen = None
 
     def _get_device_info(self) -> str:
-        info = self._caster.get_device_name()
+        info = self.app.caster.get_device_name()
         if info is not None:
             msg = f'Connected to: "{info}"'
         else:
             msg = 'Not connected to a device. Try "lolcatt --scan".'
         return msg
 
     def _update_label(self):
@@ -30,11 +30,13 @@
         self._marquee_gen = marquee(value, self.size.width, 2)
 
     def on_resize(self, value):
         self._marquee_gen = marquee(self.label_str, self.size.width, 2)
 
     def on_mount(self):
         self._update_label()
-        self.set_interval(interval=self._caster.get_update_interval(), callback=self._update_label)
+        self.set_interval(
+            interval=self.app.caster.get_update_interval(), callback=self._update_label
+        )
 
     def compose(self):
         yield Container(self.label, id='device_info')
```

### Comparing `lolcatt-0.1.2/lolcatt/ui/lolcatt_playback_info.py` & `lolcatt-0.1.3/lolcatt/ui/lolcatt_playback_info.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 from textual.containers import Container
 from textual.reactive import reactive
 from textual.widgets import Label
+from textual.widgets import Static
 
-from lolcatt.ui.caster_static import CasterStatic
 from lolcatt.utils.utils import marquee
 
 
-class LolCattPlaybackInfo(CasterStatic):
+class LolCattPlaybackInfo(Static):
     label_str = reactive('')
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.label = Label('', id='title')
         self._marquee_gen = None
 
     def _get_playback_info(self) -> str:
-        playing = self._caster.get_cast_state().cast_info.get('title')
-        display_name = self._caster.get_cast_state().info.get('display_name')
-        is_loading = self._caster.get_cast_state().is_loading
+        playing = self.app.caster.get_cast_state().cast_info.get('title')
+        display_name = self.app.caster.get_cast_state().info.get('display_name')
+        is_loading = self.app.caster.get_cast_state().is_loading
 
         if playing is not None:
             return f'Playing: "{playing}"'
         elif display_name is not None and display_name != 'Backdrop':
             return f'Displaying: "{display_name}"'
         elif is_loading:
             return 'Loading...'
@@ -38,8 +38,10 @@
     def on_resize(self, value):
         self._marquee_gen = marquee(self.label_str, self.size.width, 2)
 
     def compose(self):
         yield Container(self.label, id='playback_info')
 
     def on_mount(self):
-        self.set_interval(interval=self._caster.get_update_interval(), callback=self._update_label)
+        self.set_interval(
+            interval=self.app.caster.get_update_interval(), callback=self._update_label
+        )
```

### Comparing `lolcatt-0.1.2/lolcatt/ui/lolcatt_progress.py` & `lolcatt-0.1.3/lolcatt/ui/lolcatt_progress.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,19 +2,18 @@
 
 from catt.error import CastError
 from textual.containers import Container
 from textual.events import Click
 from textual.reactive import reactive
 from textual.widgets import Label
 from textual.widgets import ProgressBar
+from textual.widgets import Static
 
-from lolcatt.ui.caster_static import CasterStatic
 
-
-class LolCattProgress(CasterStatic):
+class LolCattProgress(Static):
     current = reactive(0)
     duration = reactive(0)
     percent_complete = reactive(0)
 
     @staticmethod
     def _extract_progress(cast_info: dict) -> Tuple[float, float, float]:
         current = cast_info.get('current_time', 0.0)
@@ -31,35 +30,35 @@
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.pb = ProgressBar(total=100, show_percentage=False, show_eta=False, id='progress_bar')
         self.pblabel = Label('(00:00/00:00)', id='progress_label')
 
     def update_progress(self) -> int:
         self.current, self.duration, self.percent_complete = self._extract_progress(
-            self._caster.get_cast_state().cast_info
+            self.app.caster.get_cast_state().cast_info
         )
         self.pb.update(progress=self.percent_complete)
         current_fmt = self._format_time(self.current)
         duration_fmt = self._format_time(self.duration)
         self.pblabel.update(f'({current_fmt}/{duration_fmt})')
 
     def on_mount(self):
         self.update_progress()
         self.set_interval(
-            interval=self._caster.get_update_interval(), callback=self.update_progress
+            interval=self.app.caster.get_update_interval(), callback=self.update_progress
         )
 
     def on_click(self, event: Click):
         min_x, max_x = (
             self.pb.content_region.x,
             self.pb.content_region.x + self.pb.content_region.width,
         )
         click_x = min(max(event.screen_x, min_x), max_x)
         fraction = min(1, (click_x - min_x) / (max_x - min_x))
-        duration = self._caster.get_cast_state().cast_info.get('duration', 0.0)
+        duration = self.app.caster.get_cast_state().cast_info.get('duration', 0.0)
         try:
-            self._caster.get_device().seek(duration * fraction)
+            self.app.caster.get_device().seek(duration * fraction)
         except CastError:
             pass
 
     def compose(self):
         yield Container(self.pb, self.pblabel, id='progress')
```

### Comparing `lolcatt-0.1.2/lolcatt/utils/utils.py` & `lolcatt-0.1.3/lolcatt/utils/utils.py`

 * *Files identical despite different names*

### Comparing `lolcatt-0.1.2/lolcatt.egg-info/PKG-INFO` & `lolcatt-0.1.3/lolcatt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lolcatt
-Version: 0.1.2
+Version: 0.1.3
 Summary: A TUI wrapper around `catt`.
 Home-page: https://github.com/LokiLuciferase/lolcatt
 Author: Lukas Lüftinger
 Author-email: lukas.lueftinger@outlook.com
 License: MIT license
 Keywords: lolcatt
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `lolcatt-0.1.2/lolcatt.egg-info/SOURCES.txt` & `lolcatt-0.1.3/lolcatt.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,13 @@
-.coveragerc
-.editorconfig
-.flake8
-.gitignore
-.pre-commit-config.yaml
-Dockerfile
 LICENSE
 MANIFEST.in
-Makefile
 README.rst
 pyproject.toml
 setup.cfg
 setup.py
-.github/ISSUE_TEMPLATE.md
-.github/workflows/ci.yml
-.github/workflows/coverage.yml
-.github/workflows/docs.yml
 docs/Makefile
 docs/conf.py
 docs/index.rst
 docs/installation.rst
 docs/lolcatt.casting.rst
 docs/lolcatt.rst
 docs/lolcatt.ui.rst
@@ -30,15 +19,14 @@
 docs/_build/html/_static/basic.css
 docs/_build/html/_static/custom.css
 docs/_build/html/_static/file.png
 docs/_build/html/_static/minus.png
 docs/_build/html/_static/nature.css
 docs/_build/html/_static/plus.png
 docs/_build/html/_static/pygments.css
-docs/_build/html/_static/screenshot.png
 docs/_static/custom.css
 docs/_static/screenshot.png
 lolcatt/__init__.py
 lolcatt/app.py
 lolcatt/cli.py
 lolcatt.egg-info/PKG-INFO
 lolcatt.egg-info/SOURCES.txt
@@ -46,21 +34,17 @@
 lolcatt.egg-info/entry_points.txt
 lolcatt.egg-info/not-zip-safe
 lolcatt.egg-info/requires.txt
 lolcatt.egg-info/top_level.txt
 lolcatt/casting/__init__.py
 lolcatt/casting/caster.py
 lolcatt/ui/__init__.py
-lolcatt/ui/caster_static.py
 lolcatt/ui/lolcatt.css
 lolcatt/ui/lolcatt_controls.py
 lolcatt/ui/lolcatt_device_info.py
 lolcatt/ui/lolcatt_playback_info.py
 lolcatt/ui/lolcatt_progress.py
 lolcatt/ui/lolcatt_url_input.py
 lolcatt/utils/__init__.py
 lolcatt/utils/utils.py
-requirements/dev.txt
-requirements/prod.txt
-requirements/test.txt
 tests/__init__.py
 tests/test_lolcatt.py
```

### Comparing `lolcatt-0.1.2/pyproject.toml` & `lolcatt-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
   | buck-out
   | build
   | dist
 )/
 '''
 
 [tool.bumpver]
-current_version = "0.1.2"
+current_version = "0.1.3"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
```

### Comparing `lolcatt-0.1.2/setup.py` & `lolcatt-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,10 +40,10 @@
     include_package_data=True,
     keywords='lolcatt',
     name='lolcatt',
     packages=find_packages(include=['lolcatt', 'lolcatt.*']),
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/LokiLuciferase/lolcatt',
-    version='0.1.2',
+    version='0.1.3',
     zip_safe=False,
 )
```

