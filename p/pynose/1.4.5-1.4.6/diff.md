# Comparing `tmp/pynose-1.4.5.tar.gz` & `tmp/pynose-1.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynose-1.4.5.tar", last modified: Wed May 24 22:17:19 2023, max compression
+gzip compressed data, was "pynose-1.4.6.tar", last modified: Sat Jul  8 03:29:15 2023, max compression
```

## Comparing `pynose-1.4.5.tar` & `pynose-1.4.6.tar`

### file list

```diff
@@ -1,70 +1,71 @@
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-24 22:17:19.465227 pynose-1.4.5/
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-24 22:17:19.456223 pynose-1.4.5/.github/
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-24 22:17:19.457916 pynose-1.4.5/.github/workflows/
--rw-r--r--   0 michael    (501) staff       (20)     1332 2023-03-01 21:40:49.000000 pynose-1.4.5/.github/workflows/python-package-legacy.yml
--rw-r--r--   0 michael    (501) staff       (20)     1357 2023-03-01 21:40:46.000000 pynose-1.4.5/.github/workflows/python-package.yml
--rw-r--r--   0 michael    (501) staff       (20)     1799 2023-02-28 01:46:25.000000 pynose-1.4.5/.gitignore
--rw-r--r--   0 michael    (501) staff       (20)     1070 2023-02-28 01:46:25.000000 pynose-1.4.5/LICENSE
--rw-r--r--   0 michael    (501) staff       (20)      135 2023-02-28 03:14:47.000000 pynose-1.4.5/MANIFEST.in
--rw-r--r--   0 michael    (501) staff       (20)    18449 2023-05-24 22:17:19.465311 pynose-1.4.5/PKG-INFO
--rw-r--r--   0 michael    (501) staff       (20)    16992 2023-05-24 22:14:10.000000 pynose-1.4.5/README.md
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-24 22:17:19.458377 pynose-1.4.5/bin/
--rwxr-xr-x   0 michael    (501) staff       (20)       84 2012-09-29 08:18:54.000000 pynose-1.4.5/bin/nosetests
--rwxr-xr-x   0 michael    (501) staff       (20)       84 2012-09-29 08:18:54.000000 pynose-1.4.5/bin/pynose
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-24 22:17:19.461132 pynose-1.4.5/nose/
--rw-r--r--   0 michael    (501) staff       (20)      643 2023-03-02 04:16:39.000000 pynose-1.4.5/nose/__init__.py
--rw-r--r--   0 michael    (501) staff       (20)      144 2022-11-25 20:24:40.000000 pynose-1.4.5/nose/__main__.py
--rwxr-xr-x   0 michael    (501) staff       (20)       44 2023-05-24 22:14:10.000000 pynose-1.4.5/nose/__version__.py
--rw-r--r--   0 michael    (501) staff       (20)    11881 2023-05-02 02:01:52.000000 pynose-1.4.5/nose/case.py
--rw-r--r--   0 michael    (501) staff       (20)     5538 2023-03-02 14:29:59.000000 pynose-1.4.5/nose/commands.py
--rw-r--r--   0 michael    (501) staff       (20)    24529 2023-03-02 15:02:07.000000 pynose-1.4.5/nose/config.py
--rw-r--r--   0 michael    (501) staff       (20)    12087 2023-03-02 13:46:19.000000 pynose-1.4.5/nose/core.py
--rw-r--r--   0 michael    (501) staff       (20)      390 2023-02-26 21:55:15.000000 pynose-1.4.5/nose/exc.py
--rw-r--r--   0 michael    (501) staff       (20)     1258 2023-02-26 21:54:35.000000 pynose-1.4.5/nose/failure.py
--rw-r--r--   0 michael    (501) staff       (20)     9007 2023-05-02 02:01:52.000000 pynose-1.4.5/nose/importer.py
--rw-r--r--   0 michael    (501) staff       (20)     5535 2023-03-02 04:00:31.000000 pynose-1.4.5/nose/inspector.py
--rw-r--r--   0 michael    (501) staff       (20)    21758 2023-03-02 14:53:46.000000 pynose-1.4.5/nose/loader.py
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-24 22:17:19.463871 pynose-1.4.5/nose/plugins/
--rw-r--r--   0 michael    (501) staff       (20)     5421 2023-03-02 16:20:15.000000 pynose-1.4.5/nose/plugins/__init__.py
--rw-r--r--   0 michael    (501) staff       (20)     1007 2023-03-02 15:57:56.000000 pynose-1.4.5/nose/plugins/allmodules.py
--rw-r--r--   0 michael    (501) staff       (20)     8189 2023-03-02 16:10:06.000000 pynose-1.4.5/nose/plugins/attrib.py
--rw-r--r--   0 michael    (501) staff       (20)    23205 2023-04-30 16:29:19.000000 pynose-1.4.5/nose/plugins/base.py
--rw-r--r--   0 michael    (501) staff       (20)     1024 2023-02-26 20:00:18.000000 pynose-1.4.5/nose/plugins/builtin.py
--rw-r--r--   0 michael    (501) staff       (20)     3280 2023-05-03 01:50:30.000000 pynose-1.4.5/nose/plugins/capture.py
--rw-r--r--   0 michael    (501) staff       (20)     2739 2023-03-02 15:58:25.000000 pynose-1.4.5/nose/plugins/collect.py
--rw-r--r--   0 michael    (501) staff       (20)    10668 2023-03-02 16:16:16.000000 pynose-1.4.5/nose/plugins/cover.py
--rw-r--r--   0 michael    (501) staff       (20)     2163 2023-03-02 15:14:11.000000 pynose-1.4.5/nose/plugins/debug.py
--rw-r--r--   0 michael    (501) staff       (20)     1435 2023-03-02 15:57:16.000000 pynose-1.4.5/nose/plugins/deprecated.py
--rw-r--r--   0 michael    (501) staff       (20)    16001 2023-03-02 16:44:33.000000 pynose-1.4.5/nose/plugins/doctests.py
--rw-r--r--   0 michael    (501) staff       (20)     6390 2023-03-02 15:59:48.000000 pynose-1.4.5/nose/plugins/errorclass.py
--rw-r--r--   0 michael    (501) staff       (20)     1495 2023-03-02 15:59:22.000000 pynose-1.4.5/nose/plugins/failuredetail.py
--rw-r--r--   0 michael    (501) staff       (20)     3401 2023-02-28 06:09:15.000000 pynose-1.4.5/nose/plugins/isolate.py
--rw-r--r--   0 michael    (501) staff       (20)     8666 2023-03-02 15:25:15.000000 pynose-1.4.5/nose/plugins/logcapture.py
--rw-r--r--   0 michael    (501) staff       (20)    14331 2023-05-24 22:14:10.000000 pynose-1.4.5/nose/plugins/manager.py
--rw-r--r--   0 michael    (501) staff       (20)    31375 2023-03-02 19:07:14.000000 pynose-1.4.5/nose/plugins/multiprocess.py
--rw-r--r--   0 michael    (501) staff       (20)    13083 2023-03-02 15:51:36.000000 pynose-1.4.5/nose/plugins/plugintest.py
--rw-r--r--   0 michael    (501) staff       (20)     1487 2023-03-02 16:00:21.000000 pynose-1.4.5/nose/plugins/skip.py
--rw-r--r--   0 michael    (501) staff       (20)     9318 2023-03-02 16:04:30.000000 pynose-1.4.5/nose/plugins/testid.py
--rw-r--r--   0 michael    (501) staff       (20)    11044 2023-03-02 15:37:08.000000 pynose-1.4.5/nose/plugins/xunit.py
--rw-r--r--   0 michael    (501) staff       (20)     5964 2023-02-28 05:29:54.000000 pynose-1.4.5/nose/proxy.py
--rw-r--r--   0 michael    (501) staff       (20)     3665 2023-03-02 14:54:42.000000 pynose-1.4.5/nose/pyversion.py
--rw-r--r--   0 michael    (501) staff       (20)     5808 2023-05-02 02:01:52.000000 pynose-1.4.5/nose/result.py
--rw-r--r--   0 michael    (501) staff       (20)     9081 2023-03-02 14:46:58.000000 pynose-1.4.5/nose/selector.py
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-24 22:17:19.464105 pynose-1.4.5/nose/sphinx/
--rw-r--r--   0 michael    (501) staff       (20)        5 2022-11-25 20:24:40.000000 pynose-1.4.5/nose/sphinx/__init__.py
--rw-r--r--   0 michael    (501) staff       (20)     5348 2023-03-02 17:41:29.000000 pynose-1.4.5/nose/sphinx/pluginopts.py
--rw-r--r--   0 michael    (501) staff       (20)    18253 2023-03-02 15:00:20.000000 pynose-1.4.5/nose/suite.py
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-24 22:17:19.464576 pynose-1.4.5/nose/tools/
--rw-r--r--   0 michael    (501) staff       (20)      465 2023-02-26 23:14:39.000000 pynose-1.4.5/nose/tools/__init__.py
--rw-r--r--   0 michael    (501) staff       (20)     4080 2023-02-28 03:39:28.000000 pynose-1.4.5/nose/tools/nontrivial.py
--rw-r--r--   0 michael    (501) staff       (20)     1083 2023-02-28 03:40:01.000000 pynose-1.4.5/nose/tools/trivial.py
--rw-r--r--   0 michael    (501) staff       (20)     4981 2023-03-02 14:56:46.000000 pynose-1.4.5/nose/twistedtools.py
--rw-r--r--   0 michael    (501) staff       (20)     3698 2023-02-28 06:39:10.000000 pynose-1.4.5/nose/usage.txt
--rw-r--r--   0 michael    (501) staff       (20)    18927 2023-05-24 22:14:10.000000 pynose-1.4.5/nose/util.py
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-24 22:17:19.465114 pynose-1.4.5/pynose.egg-info/
--rw-r--r--   0 michael    (501) staff       (20)    18449 2023-05-24 22:17:19.000000 pynose-1.4.5/pynose.egg-info/PKG-INFO
--rw-r--r--   0 michael    (501) staff       (20)     1240 2023-05-24 22:17:19.000000 pynose-1.4.5/pynose.egg-info/SOURCES.txt
--rw-r--r--   0 michael    (501) staff       (20)        1 2023-05-24 22:17:19.000000 pynose-1.4.5/pynose.egg-info/dependency_links.txt
--rw-r--r--   0 michael    (501) staff       (20)        5 2023-05-24 22:17:19.000000 pynose-1.4.5/pynose.egg-info/top_level.txt
--rw-r--r--   0 michael    (501) staff       (20)       86 2023-05-24 22:17:19.465774 pynose-1.4.5/setup.cfg
--rw-r--r--   0 michael    (501) staff       (20)     4567 2023-03-02 17:36:06.000000 pynose-1.4.5/setup.py
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-07-08 03:29:15.554846 pynose-1.4.6/
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-07-08 03:29:15.546500 pynose-1.4.6/.github/
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-07-08 03:29:15.548050 pynose-1.4.6/.github/workflows/
+-rw-r--r--   0 michael    (501) staff       (20)     1332 2023-03-01 21:40:49.000000 pynose-1.4.6/.github/workflows/python-package-legacy.yml
+-rw-r--r--   0 michael    (501) staff       (20)     1357 2023-03-01 21:40:46.000000 pynose-1.4.6/.github/workflows/python-package.yml
+-rw-r--r--   0 michael    (501) staff       (20)     1799 2023-02-28 01:46:25.000000 pynose-1.4.6/.gitignore
+-rw-r--r--   0 michael    (501) staff       (20)     1070 2023-02-28 01:46:25.000000 pynose-1.4.6/LICENSE
+-rw-r--r--   0 michael    (501) staff       (20)      135 2023-02-28 03:14:47.000000 pynose-1.4.6/MANIFEST.in
+-rw-r--r--   0 michael    (501) staff       (20)    18543 2023-07-08 03:29:15.554941 pynose-1.4.6/PKG-INFO
+-rw-r--r--   0 michael    (501) staff       (20)    17086 2023-07-08 03:28:10.000000 pynose-1.4.6/README.md
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-07-08 03:29:15.548629 pynose-1.4.6/bin/
+-rwxr-xr-x   0 michael    (501) staff       (20)       84 2012-09-29 08:18:54.000000 pynose-1.4.6/bin/nosetests
+-rwxr-xr-x   0 michael    (501) staff       (20)       84 2012-09-29 08:18:54.000000 pynose-1.4.6/bin/pynose
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-07-08 03:29:15.551184 pynose-1.4.6/nose/
+-rw-r--r--   0 michael    (501) staff       (20)      643 2023-07-07 23:53:47.000000 pynose-1.4.6/nose/__init__.py
+-rw-r--r--   0 michael    (501) staff       (20)      144 2023-07-07 23:40:25.000000 pynose-1.4.6/nose/__main__.py
+-rwxr-xr-x   0 michael    (501) staff       (20)       44 2023-07-08 03:28:10.000000 pynose-1.4.6/nose/__version__.py
+-rw-r--r--   0 michael    (501) staff       (20)    11881 2023-05-02 02:01:52.000000 pynose-1.4.6/nose/case.py
+-rw-r--r--   0 michael    (501) staff       (20)     5538 2023-03-02 14:29:59.000000 pynose-1.4.6/nose/commands.py
+-rw-r--r--   0 michael    (501) staff       (20)    24529 2023-03-02 15:02:07.000000 pynose-1.4.6/nose/config.py
+-rw-r--r--   0 michael    (501) staff       (20)    12087 2023-03-02 13:46:19.000000 pynose-1.4.6/nose/core.py
+-rw-r--r--   0 michael    (501) staff       (20)      390 2023-02-26 21:55:15.000000 pynose-1.4.6/nose/exc.py
+-rw-r--r--   0 michael    (501) staff       (20)     1258 2023-02-26 21:54:35.000000 pynose-1.4.6/nose/failure.py
+-rw-r--r--   0 michael    (501) staff       (20)     9007 2023-05-02 02:01:52.000000 pynose-1.4.6/nose/importer.py
+-rw-r--r--   0 michael    (501) staff       (20)     5535 2023-03-02 04:00:31.000000 pynose-1.4.6/nose/inspector.py
+-rw-r--r--   0 michael    (501) staff       (20)    21758 2023-03-02 14:53:46.000000 pynose-1.4.6/nose/loader.py
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-07-08 03:29:15.553593 pynose-1.4.6/nose/plugins/
+-rw-r--r--   0 michael    (501) staff       (20)     5421 2023-03-02 16:20:15.000000 pynose-1.4.6/nose/plugins/__init__.py
+-rw-r--r--   0 michael    (501) staff       (20)     1007 2023-03-02 15:57:56.000000 pynose-1.4.6/nose/plugins/allmodules.py
+-rw-r--r--   0 michael    (501) staff       (20)     8189 2023-03-02 16:10:06.000000 pynose-1.4.6/nose/plugins/attrib.py
+-rw-r--r--   0 michael    (501) staff       (20)    23205 2023-04-30 16:29:19.000000 pynose-1.4.6/nose/plugins/base.py
+-rw-r--r--   0 michael    (501) staff       (20)     1024 2023-02-26 20:00:18.000000 pynose-1.4.6/nose/plugins/builtin.py
+-rw-r--r--   0 michael    (501) staff       (20)     3280 2023-05-03 01:50:30.000000 pynose-1.4.6/nose/plugins/capture.py
+-rw-r--r--   0 michael    (501) staff       (20)     2739 2023-03-02 15:58:25.000000 pynose-1.4.6/nose/plugins/collect.py
+-rw-r--r--   0 michael    (501) staff       (20)    10668 2023-03-02 16:16:16.000000 pynose-1.4.6/nose/plugins/cover.py
+-rw-r--r--   0 michael    (501) staff       (20)     2163 2023-03-02 15:14:11.000000 pynose-1.4.6/nose/plugins/debug.py
+-rw-r--r--   0 michael    (501) staff       (20)     1435 2023-03-02 15:57:16.000000 pynose-1.4.6/nose/plugins/deprecated.py
+-rw-r--r--   0 michael    (501) staff       (20)    16001 2023-03-02 16:44:33.000000 pynose-1.4.6/nose/plugins/doctests.py
+-rw-r--r--   0 michael    (501) staff       (20)     6390 2023-03-02 15:59:48.000000 pynose-1.4.6/nose/plugins/errorclass.py
+-rw-r--r--   0 michael    (501) staff       (20)     1495 2023-03-02 15:59:22.000000 pynose-1.4.6/nose/plugins/failuredetail.py
+-rw-r--r--   0 michael    (501) staff       (20)     3401 2023-02-28 06:09:15.000000 pynose-1.4.6/nose/plugins/isolate.py
+-rw-r--r--   0 michael    (501) staff       (20)     8666 2023-03-02 15:25:15.000000 pynose-1.4.6/nose/plugins/logcapture.py
+-rw-r--r--   0 michael    (501) staff       (20)    15004 2023-07-08 03:28:10.000000 pynose-1.4.6/nose/plugins/manager.py
+-rw-r--r--   0 michael    (501) staff       (20)    31375 2023-03-02 19:07:14.000000 pynose-1.4.6/nose/plugins/multiprocess.py
+-rw-r--r--   0 michael    (501) staff       (20)    13083 2023-03-02 15:51:36.000000 pynose-1.4.6/nose/plugins/plugintest.py
+-rw-r--r--   0 michael    (501) staff       (20)     1487 2023-03-02 16:00:21.000000 pynose-1.4.6/nose/plugins/skip.py
+-rw-r--r--   0 michael    (501) staff       (20)     9318 2023-03-02 16:04:30.000000 pynose-1.4.6/nose/plugins/testid.py
+-rw-r--r--   0 michael    (501) staff       (20)    11044 2023-03-02 15:37:08.000000 pynose-1.4.6/nose/plugins/xunit.py
+-rw-r--r--   0 michael    (501) staff       (20)     5964 2023-02-28 05:29:54.000000 pynose-1.4.6/nose/proxy.py
+-rw-r--r--   0 michael    (501) staff       (20)     3665 2023-03-02 14:54:42.000000 pynose-1.4.6/nose/pyversion.py
+-rw-r--r--   0 michael    (501) staff       (20)     5808 2023-05-02 02:01:52.000000 pynose-1.4.6/nose/result.py
+-rw-r--r--   0 michael    (501) staff       (20)     9081 2023-03-02 14:46:58.000000 pynose-1.4.6/nose/selector.py
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-07-08 03:29:15.553828 pynose-1.4.6/nose/sphinx/
+-rw-r--r--   0 michael    (501) staff       (20)        5 2022-11-25 20:24:40.000000 pynose-1.4.6/nose/sphinx/__init__.py
+-rw-r--r--   0 michael    (501) staff       (20)     5348 2023-03-02 17:41:29.000000 pynose-1.4.6/nose/sphinx/pluginopts.py
+-rw-r--r--   0 michael    (501) staff       (20)    18253 2023-03-02 15:00:20.000000 pynose-1.4.6/nose/suite.py
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-07-08 03:29:15.554164 pynose-1.4.6/nose/tools/
+-rw-r--r--   0 michael    (501) staff       (20)      465 2023-02-26 23:14:39.000000 pynose-1.4.6/nose/tools/__init__.py
+-rw-r--r--   0 michael    (501) staff       (20)     4080 2023-02-28 03:39:28.000000 pynose-1.4.6/nose/tools/nontrivial.py
+-rw-r--r--   0 michael    (501) staff       (20)     1083 2023-02-28 03:40:01.000000 pynose-1.4.6/nose/tools/trivial.py
+-rw-r--r--   0 michael    (501) staff       (20)     4981 2023-03-02 14:56:46.000000 pynose-1.4.6/nose/twistedtools.py
+-rw-r--r--   0 michael    (501) staff       (20)     3698 2023-02-28 06:39:10.000000 pynose-1.4.6/nose/usage.txt
+-rw-r--r--   0 michael    (501) staff       (20)    18927 2023-05-24 22:14:10.000000 pynose-1.4.6/nose/util.py
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-07-08 03:29:15.554739 pynose-1.4.6/pynose.egg-info/
+-rw-r--r--   0 michael    (501) staff       (20)    18543 2023-07-08 03:29:15.000000 pynose-1.4.6/pynose.egg-info/PKG-INFO
+-rw-r--r--   0 michael    (501) staff       (20)     1273 2023-07-08 03:29:15.000000 pynose-1.4.6/pynose.egg-info/SOURCES.txt
+-rw-r--r--   0 michael    (501) staff       (20)        1 2023-07-08 03:29:15.000000 pynose-1.4.6/pynose.egg-info/dependency_links.txt
+-rw-r--r--   0 michael    (501) staff       (20)       77 2023-07-08 03:29:15.000000 pynose-1.4.6/pynose.egg-info/entry_points.txt
+-rw-r--r--   0 michael    (501) staff       (20)        5 2023-07-08 03:29:15.000000 pynose-1.4.6/pynose.egg-info/top_level.txt
+-rw-r--r--   0 michael    (501) staff       (20)       86 2023-07-08 03:29:15.555207 pynose-1.4.6/setup.cfg
+-rw-r--r--   0 michael    (501) staff       (20)     4838 2023-07-08 03:28:10.000000 pynose-1.4.6/setup.py
```

### Comparing `pynose-1.4.5/.github/workflows/python-package-legacy.yml` & `pynose-1.4.6/.github/workflows/python-package-legacy.yml`

 * *Files identical despite different names*

### Comparing `pynose-1.4.5/.github/workflows/python-package.yml` & `pynose-1.4.6/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `pynose-1.4.5/.gitignore` & `pynose-1.4.6/.gitignore`

 * *Files identical despite different names*

### Comparing `pynose-1.4.5/LICENSE` & `pynose-1.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pynose-1.4.5/PKG-INFO` & `pynose-1.4.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 7079 6e6f  : 2.1.Name: pyno
 00000020: 7365 0a56 6572 7369 6f6e 3a20 312e 342e  se.Version: 1.4.
-00000030: 350a 5375 6d6d 6172 793a 2070 796e 6f73  5.Summary: pynos
+00000030: 360a 5375 6d6d 6172 793a 2070 796e 6f73  6.Summary: pynos
 00000040: 6520 6669 7865 7320 6e6f 7365 2074 6f20  e fixes nose to 
 00000050: 6578 7465 6e64 2075 6e69 7474 6573 7420  extend unittest 
 00000060: 616e 6420 6d61 6b65 2074 6573 7469 6e67  and make testing
 00000070: 2065 6173 6965 720a 486f 6d65 2d70 6167   easier.Home-pag
 00000080: 653a 2068 7474 7073 3a2f 2f67 6974 6875  e: https://githu
 00000090: 622e 636f 6d2f 6d64 6d69 6e74 7a2f 7079  b.com/mdmintz/py
 000000a0: 6e6f 7365 0a41 7574 686f 723a 204d 6963  nose.Author: Mic
@@ -85,1070 +85,1075 @@
 00000540: 6172 6520 4465 7665 6c6f 706d 656e 7420  are Development 
 00000550: 3a3a 2054 6573 7469 6e67 0a52 6571 7569  :: Testing.Requi
 00000560: 7265 732d 5079 7468 6f6e 3a20 3e3d 332e  res-Python: >=3.
 00000570: 360a 4465 7363 7269 7074 696f 6e2d 436f  6.Description-Co
 00000580: 6e74 656e 742d 5479 7065 3a20 7465 7874  ntent-Type: text
 00000590: 2f6d 6172 6b64 6f77 6e0a 4c69 6365 6e73  /markdown.Licens
 000005a0: 652d 4669 6c65 3a20 4c49 4345 4e53 450a  e-File: LICENSE.
-000005b0: 0a23 2070 796e 6f73 650a 0a23 2323 2060  .# pynose..### `
-000005c0: 6070 796e 6f73 6560 6020 6669 7865 7320  `pynose`` fixes 
-000005d0: 6060 6e6f 7365 6060 2074 6f20 6578 7465  ``nose`` to exte
-000005e0: 6e64 205b 756e 6974 7465 7374 5d28 6874  nd [unittest](ht
-000005f0: 7470 733a 2f2f 646f 6373 2e70 7974 686f  tps://docs.pytho
-00000600: 6e2e 6f72 672f 332f 6c69 6272 6172 792f  n.org/3/library/
-00000610: 756e 6974 7465 7374 2e68 746d 6c29 2061  unittest.html) a
-00000620: 6e64 206d 616b 6520 7465 7374 696e 6720  nd make testing 
-00000630: 6561 7369 6572 2e0a 0a28 4e4f 5445 3a20  easier...(NOTE: 
-00000640: 4966 2079 6f75 2063 616e 2c20 7573 6520  If you can, use 
-00000650: 2a2a 5b70 7974 6573 745d 2868 7474 7073  **[pytest](https
-00000660: 3a2f 2f64 6f63 732e 7079 7465 7374 2e6f  ://docs.pytest.o
-00000670: 7267 2f29 2a2a 2069 6e73 7465 6164 2e20  rg/)** instead. 
-00000680: 2a2a 5b70 796e 6f73 655d 2868 7474 7073  **[pynose](https
-00000690: 3a2f 2f67 6974 6875 622e 636f 6d2f 6d64  ://github.com/md
-000006a0: 6d69 6e74 7a2f 7079 6e6f 7365 292a 2a20  mintz/pynose)** 
-000006b0: 7761 7320 6275 696c 7420 746f 206d 6169  was built to mai
-000006c0: 6e74 6169 6e20 2a2a 5b6e 6f73 655d 2868  ntain **[nose](h
-000006d0: 7474 7073 3a2f 2f6e 6f73 652e 7265 6164  ttps://nose.read
-000006e0: 7468 6564 6f63 732e 696f 2f65 6e2f 6c61  thedocs.io/en/la
-000006f0: 7465 7374 2f29 2a2a 2066 6f72 2064 6576  test/)** for dev
-00000700: 656c 6f70 6572 7320 7768 6f20 7374 696c  elopers who stil
-00000710: 6c20 7573 6520 6974 2e29 0a0a 2d2d 2d2d  l use it.)..----
-00000720: 2d2d 2d2d 0a0a 6060 7079 6e6f 7365 6060  ----..``pynose``
-00000730: 2069 7320 616e 2075 7064 6174 6564 2076   is an updated v
-00000740: 6572 7369 6f6e 206f 6620 6060 6e6f 7365  ersion of ``nose
-00000750: 6060 2c20 6f72 6967 696e 616c 6c79 206d  ``, originally m
-00000760: 6164 6520 6279 204a 6173 6f6e 2050 656c  ade by Jason Pel
-00000770: 6c65 7269 6e2e 0a0a 5468 6973 2076 6572  lerin...This ver
-00000780: 7369 6f6e 206f 6620 6060 6e6f 7365 6060  sion of ``nose``
-00000790: 2069 7320 636f 6d70 6174 6962 6c65 2077   is compatible w
-000007a0: 6974 6820 5079 7468 6f6e 2033 2e36 2b20  ith Python 3.6+ 
-000007b0: 2869 6e63 6c75 6469 6e67 2033 2e31 3220  (including 3.12 
-000007c0: 2620 7570 292e 0a0a 4368 616e 6765 7320  & up)...Changes 
-000007d0: 696e 2060 6070 796e 6f73 6560 6020 6672  in ``pynose`` fr
-000007e0: 6f6d 206c 6567 6163 7920 6060 6e6f 7365  om legacy ``nose
-000007f0: 6060 2069 6e63 6c75 6465 3a0a 2a20 4669  `` include:.* Fi
-00000800: 7865 7320 2241 7474 7269 6275 7465 4572  xes "AttributeEr
-00000810: 726f 723a 206d 6f64 756c 6520 2763 6f6c  ror: module 'col
-00000820: 6c65 6374 696f 6e73 2720 6861 7320 6e6f  lections' has no
-00000830: 2061 7474 7269 6275 7465 2027 4361 6c6c   attribute 'Call
-00000840: 6162 6c65 272e 220a 2a20 4669 7865 7320  able'.".* Fixes 
-00000850: 2241 7474 7269 6275 7465 4572 726f 723a  "AttributeError:
-00000860: 206d 6f64 756c 6520 2769 6e73 7065 6374   module 'inspect
-00000870: 2720 6861 7320 6e6f 2061 7474 7269 6275  ' has no attribu
-00000880: 7465 2027 6765 7461 7267 7370 6563 272e  te 'getargspec'.
-00000890: 220a 2a20 4669 7865 7320 2249 6d70 6f72  ".* Fixes "Impor
-000008a0: 7445 7272 6f72 3a20 6361 6e6e 6f74 2069  tError: cannot i
-000008b0: 6d70 6f72 7420 6e61 6d65 2027 5f54 6578  mport name '_Tex
-000008c0: 7454 6573 7452 6573 756c 7427 2066 726f  tTestResult' fro
-000008d0: 6d20 2775 6e69 7474 6573 7427 2e22 0a2a  m 'unittest'.".*
-000008e0: 2046 6978 6573 2022 5275 6e74 696d 6557   Fixes "RuntimeW
-000008f0: 6172 6e69 6e67 3a20 5465 7374 5265 7375  arning: TestResu
-00000900: 6c74 2068 6173 206e 6f20 6164 6444 7572  lt has no addDur
-00000910: 6174 696f 6e20 6d65 7468 6f64 2e22 0a2a  ation method.".*
-00000920: 2046 6978 6573 2061 6c6c 2060 6066 6c61   Fixes all ``fla
-00000930: 6b65 3860 6020 6973 7375 6573 2066 726f  ke8`` issues fro
-00000940: 6d20 7468 6520 6f72 6967 696e 616c 2060  m the original `
-00000950: 606e 6f73 6560 602e 0a2a 2052 6570 6c61  `nose``..* Repla
-00000960: 6365 7320 7468 6520 6060 696d 7060 6020  ces the ``imp`` 
-00000970: 6d6f 6475 6c65 2077 6974 6820 7468 6520  module with the 
-00000980: 6e65 7765 7220 6060 696d 706f 7274 6c69  newer ``importli
-00000990: 6260 6020 6d6f 6475 6c65 2e0a 2a20 5468  b`` module..* Th
-000009a0: 6520 6465 6661 756c 7420 6c6f 6767 696e  e default loggin
-000009b0: 6720 6c65 7665 6c20 6e6f 7720 6869 6465  g level now hide
-000009c0: 7320 2264 6562 7567 2220 6c6f 6773 2066  s "debug" logs f
-000009d0: 6f72 206c 6573 7320 6e6f 6973 652e 0a2a  or less noise..*
-000009e0: 2054 6865 2060 602d 7360 6020 6f70 7469   The ``-s`` opti
-000009f0: 6f6e 2069 7320 616c 7761 7973 2061 6374  on is always act
-00000a00: 6976 6520 746f 2073 6565 2074 6865 206f  ive to see the o
-00000a10: 7574 7075 7420 6f66 2060 6070 7269 6e74  utput of ``print
-00000a20: 2829 6060 2e0a 2a20 4164 6473 2060 602d  ()``..* Adds ``-
-00000a30: 2d63 6f60 6020 6173 2061 2073 686f 7274  -co`` as a short
-00000a40: 6375 7420 746f 2075 7369 6e67 2060 602d  cut to using ``-
-00000a50: 2d63 6f6c 6c65 6374 2d6f 6e6c 7960 602e  -collect-only``.
-00000a60: 0a0a 2d2d 2d2d 2d2d 2d2d 0a0a 5468 6520  ..--------..The 
-00000a70: 6f72 6967 696e 616c 2064 6573 6372 6970  original descrip
-00000a80: 7469 6f6e 206f 6620 6060 6e6f 7365 6060  tion of ``nose``
-00000a90: 3a0a 0a3e 6e6f 7365 2065 7874 656e 6473  :..>nose extends
-00000aa0: 2074 6865 2074 6573 7420 6c6f 6164 696e   the test loadin
-00000ab0: 6720 616e 6420 7275 6e6e 696e 6720 6665  g and running fe
-00000ac0: 6174 7572 6573 206f 6620 756e 6974 7465  atures of unitte
-00000ad0: 7374 2c20 6d61 6b69 6e67 0a69 7420 6561  st, making.it ea
-00000ae0: 7369 6572 2074 6f20 7772 6974 652c 2066  sier to write, f
-00000af0: 696e 6420 616e 6420 7275 6e20 7465 7374  ind and run test
-00000b00: 732e 0a0a 3e42 7920 6465 6661 756c 742c  s...>By default,
-00000b10: 206e 6f73 6520 7275 6e73 2074 6573 7473   nose runs tests
-00000b20: 2069 6e20 6669 6c65 7320 6f72 2064 6972   in files or dir
-00000b30: 6563 746f 7269 6573 2075 6e64 6572 2074  ectories under t
-00000b40: 6865 2063 7572 7265 6e74 0a77 6f72 6b69  he current.worki
-00000b50: 6e67 2064 6972 6563 746f 7279 2077 686f  ng directory who
-00000b60: 7365 206e 616d 6573 2069 6e63 6c75 6465  se names include
-00000b70: 2022 7465 7374 2220 6f72 2022 5465 7374   "test" or "Test
-00000b80: 2220 6174 2061 2077 6f72 640a 626f 756e  " at a word.boun
-00000b90: 6461 7279 2028 6c69 6b65 2022 7465 7374  dary (like "test
-00000ba0: 5f74 6869 7322 206f 7220 2266 756e 6374  _this" or "funct
-00000bb0: 696f 6e61 6c5f 7465 7374 2220 6f72 2022  ional_test" or "
-00000bc0: 5465 7374 436c 6173 7322 2062 7574 206e  TestClass" but n
-00000bd0: 6f74 0a22 6c69 6274 6573 7422 292e 2054  ot."libtest"). T
-00000be0: 6573 7420 6f75 7470 7574 2069 7320 7369  est output is si
-00000bf0: 6d69 6c61 7220 746f 2074 6861 7420 6f66  milar to that of
-00000c00: 2075 6e69 7474 6573 742c 2062 7574 2061   unittest, but a
-00000c10: 6c73 6f20 696e 636c 7564 6573 0a63 6170  lso includes.cap
-00000c20: 7475 7265 6420 7374 646f 7574 206f 7574  tured stdout out
-00000c30: 7075 7420 6672 6f6d 2066 6169 6c69 6e67  put from failing
-00000c40: 2074 6573 7473 2c20 666f 7220 6561 7379   tests, for easy
-00000c50: 2070 7269 6e74 2d73 7479 6c65 2064 6562   print-style deb
-00000c60: 7567 6769 6e67 2e0a 0a3e 5468 6573 6520  ugging...>These 
-00000c70: 6665 6174 7572 6573 2c20 616e 6420 6d61  features, and ma
-00000c80: 6e79 206d 6f72 652c 2061 7265 2063 7573  ny more, are cus
-00000c90: 746f 6d69 7a61 626c 6520 7468 726f 7567  tomizable throug
-00000ca0: 6820 7468 6520 7573 6520 6f66 0a70 6c75  h the use of.plu
-00000cb0: 6769 6e73 2e20 506c 7567 696e 7320 696e  gins. Plugins in
-00000cc0: 636c 7564 6564 2077 6974 6820 6e6f 7365  cluded with nose
-00000cd0: 2070 726f 7669 6465 2073 7570 706f 7274   provide support
-00000ce0: 2066 6f72 2064 6f63 7465 7374 2c20 636f   for doctest, co
-00000cf0: 6465 0a63 6f76 6572 6167 6520 616e 6420  de.coverage and 
-00000d00: 7072 6f66 696c 696e 672c 2066 6c65 7869  profiling, flexi
-00000d10: 626c 6520 6174 7472 6962 7574 652d 6261  ble attribute-ba
-00000d20: 7365 6420 7465 7374 2073 656c 6563 7469  sed test selecti
-00000d30: 6f6e 2c0a 6f75 7470 7574 2063 6170 7475  on,.output captu
-00000d40: 7265 2061 6e64 206d 6f72 652e 204d 6f72  re and more. Mor
-00000d50: 6520 696e 666f 726d 6174 696f 6e20 6162  e information ab
-00000d60: 6f75 7420 7772 6974 696e 6720 706c 7567  out writing plug
-00000d70: 696e 730a 6d61 7920 6265 2066 6f75 6e64  ins.may be found
-00000d80: 206f 6e20 696e 2074 6865 206e 6f73 6520   on in the nose 
-00000d90: 4150 4920 646f 6375 6d65 6e74 6174 696f  API documentatio
-00000da0: 6e2c 2068 6572 653a 0a68 7474 7073 3a2f  n, here:.https:/
-00000db0: 2f6e 6f73 652e 7265 6164 7468 6564 6f63  /nose.readthedoc
-00000dc0: 732e 696f 2f65 6e2f 6c61 7465 7374 2f0a  s.io/en/latest/.
-00000dd0: 0a2d 2d2d 2d2d 2d2d 2d0a 0a60 6060 6261  .--------..```ba
-00000de0: 7368 0a0a 4261 7369 6320 7573 6167 650a  sh..Basic usage.
-00000df0: 2a2a 2a2a 2a2a 2a2a 2a2a 2a0a 0a55 7365  ***********..Use
-00000e00: 2022 7079 6e6f 7365 2220 4f52 2022 6e6f   "pynose" OR "no
-00000e10: 7365 7465 7374 7322 2074 6f20 7275 6e20  setests" to run 
-00000e20: 7465 7374 733a 0a0a 2020 2020 7079 6e6f  tests:..    pyno
-00000e30: 7365 205b 6f70 7469 6f6e 735d 205b 286f  se [options] [(o
-00000e40: 7074 696f 6e61 6c29 2074 6573 7420 6669  ptional) test fi
-00000e50: 6c65 7320 6f72 2064 6972 6563 746f 7269  les or directori
-00000e60: 6573 5d0a 0a20 2020 206e 6f73 6574 6573  es]..    nosetes
-00000e70: 7473 205b 6f70 7469 6f6e 735d 205b 286f  ts [options] [(o
-00000e80: 7074 696f 6e61 6c29 2074 6573 7420 6669  ptional) test fi
-00000e90: 6c65 7320 6f72 2064 6972 6563 746f 7269  les or directori
-00000ea0: 6573 5d0a 0a49 6e20 6164 6469 7469 6f6e  es]..In addition
-00000eb0: 2074 6f20 7061 7373 696e 6720 636f 6d6d   to passing comm
-00000ec0: 616e 642d 6c69 6e65 206f 7074 696f 6e73  and-line options
-00000ed0: 2c20 796f 7520 6d61 7920 616c 736f 2070  , you may also p
-00000ee0: 7574 0a63 6f6e 6669 6775 7261 7469 6f6e  ut.configuration
-00000ef0: 206f 7074 696f 6e73 2069 6e20 6120 2e6e   options in a .n
-00000f00: 6f73 6572 6320 6f72 206e 6f73 652e 6366  oserc or nose.cf
-00000f10: 6720 6669 6c65 2069 6e20 796f 7572 2068  g file in your h
-00000f20: 6f6d 650a 6469 7265 6374 6f72 792e 2054  ome.directory. T
-00000f30: 6865 7365 2061 7265 2073 7461 6e64 6172  hese are standar
-00000f40: 6420 2e69 6e69 2d73 7479 6c65 2063 6f6e  d .ini-style con
-00000f50: 6669 6720 6669 6c65 732e 2050 7574 2079  fig files. Put y
-00000f60: 6f75 720a 6e6f 7365 7465 7374 7320 636f  our.nosetests co
-00000f70: 6e66 6967 7572 6174 696f 6e20 696e 2061  nfiguration in a
-00000f80: 205b 6e6f 7365 7465 7374 735d 2073 6563   [nosetests] sec
-00000f90: 7469 6f6e 2c20 7769 7468 2074 6865 202d  tion, with the -
-00000fa0: 2d20 7072 6566 6978 0a72 656d 6f76 6564  - prefix.removed
-00000fb0: 3a0a 0a20 2020 5b6e 6f73 6574 6573 7473  :..   [nosetests
-00000fc0: 5d0a 2020 2076 6572 626f 7369 7479 3d33  ].   verbosity=3
-00000fd0: 0a20 2020 7769 7468 2d64 6f63 7465 7374  .   with-doctest
-00000fe0: 3d31 0a0a 5468 6572 6520 6973 2061 6c73  =1..There is als
-00000ff0: 6f20 706f 7373 6962 6c69 7479 2074 6f20  o possiblity to 
-00001000: 6469 7361 626c 6520 636f 6e66 6967 7572  disable configur
-00001010: 6174 696f 6e20 6669 6c65 7320 6c6f 6164  ation files load
-00001020: 696e 6720 286d 6967 6874 0a62 6520 7573  ing (might.be us
-00001030: 6566 756c 2077 6865 6e20 7275 6e6e 6967  eful when runnig
-00001040: 2069 2e65 2e20 746f 7820 616e 6420 796f   i.e. tox and yo
-00001050: 7520 646f 206e 6f74 2077 616e 7420 796f  u do not want yo
-00001060: 7572 2067 6c6f 6261 6c20 6e6f 7365 0a63  ur global nose.c
-00001070: 6f6e 6669 6720 6669 6c65 2074 6f20 6265  onfig file to be
-00001080: 2075 7365 6420 6279 2074 6f78 292e 2049   used by tox). I
-00001090: 6e20 6f72 6465 7220 746f 2069 676e 6f72  n order to ignor
-000010a0: 6520 7468 6f73 6520 636f 6e66 6967 7572  e those configur
-000010b0: 6174 696f 6e0a 6669 6c65 7320 7369 6d70  ation.files simp
-000010c0: 6c79 2073 6574 2061 6e20 656e 7669 726f  ly set an enviro
-000010d0: 6e6d 656e 7420 7661 7269 6162 6c65 2022  nment variable "
-000010e0: 4e4f 5345 5f49 474e 4f52 455f 434f 4e46  NOSE_IGNORE_CONF
-000010f0: 4947 5f46 494c 4553 222e 0a0a 5468 6572  IG_FILES"...Ther
-00001100: 6520 6172 6520 7365 7665 7261 6c20 6f74  e are several ot
-00001110: 6865 7220 7761 7973 2074 6f20 7573 6520  her ways to use 
-00001120: 7468 6520 6e6f 7365 2074 6573 7420 7275  the nose test ru
-00001130: 6e6e 6572 2062 6573 6964 6573 2074 6865  nner besides the
-00001140: 0a2a 6e6f 7365 7465 7374 732a 2073 6372  .*nosetests* scr
-00001150: 6970 742e 2059 6f75 206d 6179 2075 7365  ipt. You may use
-00001160: 206e 6f73 6520 696e 2061 2074 6573 7420   nose in a test 
-00001170: 7363 7269 7074 3a0a 0a20 2020 696d 706f  script:..   impo
-00001180: 7274 206e 6f73 650a 2020 206e 6f73 652e  rt nose.   nose.
-00001190: 6d61 696e 2829 0a0a 4966 2079 6f75 2064  main()..If you d
-000011a0: 6f20 6e6f 7420 7761 6e74 2074 6865 2074  o not want the t
-000011b0: 6573 7420 7363 7269 7074 2074 6f20 6578  est script to ex
-000011c0: 6974 2077 6974 6820 3020 6f6e 2073 7563  it with 0 on suc
-000011d0: 6365 7373 2061 6e64 2031 206f 6e0a 6661  cess and 1 on.fa
-000011e0: 696c 7572 6520 286c 696b 6520 756e 6974  ilure (like unit
-000011f0: 7465 7374 2e6d 6169 6e29 2c20 7573 6520  test.main), use 
-00001200: 6e6f 7365 2e72 756e 2829 2069 6e73 7465  nose.run() inste
-00001210: 6164 3a0a 0a20 2020 696d 706f 7274 206e  ad:..   import n
-00001220: 6f73 650a 2020 2072 6573 756c 7420 3d20  ose.   result = 
-00001230: 6e6f 7365 2e72 756e 2829 0a0a 2a72 6573  nose.run()..*res
-00001240: 756c 742a 2077 696c 6c20 6265 2074 7275  ult* will be tru
-00001250: 6520 6966 2074 6865 2074 6573 7420 7275  e if the test ru
-00001260: 6e20 7375 6363 6565 6465 642c 206f 7220  n succeeded, or 
-00001270: 6661 6c73 6520 6966 2061 6e79 2074 6573  false if any tes
-00001280: 740a 6661 696c 6564 206f 7220 7261 6973  t.failed or rais
-00001290: 6564 2061 6e20 756e 6361 7567 6874 2065  ed an uncaught e
-000012a0: 7863 6570 7469 6f6e 2e20 4c61 7374 6c79  xception. Lastly
-000012b0: 2c20 796f 7520 6361 6e20 7275 6e20 6e6f  , you can run no
-000012c0: 7365 2e63 6f72 650a 6469 7265 6374 6c79  se.core.directly
-000012d0: 2c20 7768 6963 6820 7769 6c6c 2072 756e  , which will run
-000012e0: 206e 6f73 652e 6d61 696e 2829 3a0a 0a20   nose.main():.. 
-000012f0: 2020 7079 7468 6f6e 202f 7061 7468 2f74    python /path/t
-00001300: 6f2f 6e6f 7365 2f63 6f72 652e 7079 0a0a  o/nose/core.py..
-00001310: 506c 6561 7365 2073 6565 2074 6865 2075  Please see the u
-00001320: 7361 6765 206d 6573 7361 6765 2066 6f72  sage message for
-00001330: 2074 6865 206e 6f73 6574 6573 7473 2073   the nosetests s
-00001340: 6372 6970 7420 666f 7220 696e 666f 726d  cript for inform
-00001350: 6174 696f 6e0a 6162 6f75 7420 686f 7720  ation.about how 
-00001360: 746f 2063 6f6e 7472 6f6c 2077 6869 6368  to control which
-00001370: 2074 6573 7473 206e 6f73 6520 7275 6e73   tests nose runs
-00001380: 2c20 7768 6963 6820 706c 7567 696e 7320  , which plugins 
-00001390: 6172 6520 6c6f 6164 6564 2c0a 616e 6420  are loaded,.and 
-000013a0: 7468 6520 7465 7374 206f 7574 7075 742e  the test output.
-000013b0: 0a0a 0a45 7874 656e 6465 6420 7573 6167  ...Extended usag
-000013c0: 650a 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  e.==============
-000013d0: 0a0a 6e6f 7365 2063 6f6c 6c65 6374 7320  ..nose collects 
-000013e0: 7465 7374 7320 6175 746f 6d61 7469 6361  tests automatica
-000013f0: 6c6c 7920 6672 6f6d 2070 7974 686f 6e20  lly from python 
-00001400: 736f 7572 6365 2066 696c 6573 2c0a 6469  source files,.di
-00001410: 7265 6374 6f72 6965 7320 616e 6420 7061  rectories and pa
-00001420: 636b 6167 6573 2066 6f75 6e64 2069 6e20  ckages found in 
-00001430: 6974 7320 776f 726b 696e 6720 6469 7265  its working dire
-00001440: 6374 6f72 7920 2877 6869 6368 0a64 6566  ctory (which.def
-00001450: 6175 6c74 7320 746f 2074 6865 2063 7572  aults to the cur
-00001460: 7265 6e74 2077 6f72 6b69 6e67 2064 6972  rent working dir
-00001470: 6563 746f 7279 292e 2041 6e79 2070 7974  ectory). Any pyt
-00001480: 686f 6e20 736f 7572 6365 2066 696c 652c  hon source file,
-00001490: 0a64 6972 6563 746f 7279 206f 7220 7061  .directory or pa
-000014a0: 636b 6167 6520 7468 6174 206d 6174 6368  ckage that match
-000014b0: 6573 2074 6865 2074 6573 744d 6174 6368  es the testMatch
-000014c0: 2072 6567 756c 6172 2065 7870 7265 7373   regular express
-000014d0: 696f 6e20 2862 790a 6465 6661 756c 743a  ion (by.default:
-000014e0: 202a 283f 3a5e 7c5b 625f 2e2d 5d29 5b54   *(?:^|[b_.-])[T
-000014f0: 745d 6573 7429 2a20 7769 6c6c 2062 6520  t]est)* will be 
-00001500: 636f 6c6c 6563 7465 6420 6173 2061 2074  collected as a t
-00001510: 6573 7420 286f 7220 736f 7572 6365 0a66  est (or source.f
-00001520: 6f72 2063 6f6c 6c65 6374 696f 6e20 6f66  or collection of
-00001530: 2074 6573 7473 292e 2049 6e20 6164 6469   tests). In addi
-00001540: 7469 6f6e 2c20 616c 6c20 6f74 6865 7220  tion, all other 
-00001550: 7061 636b 6167 6573 2066 6f75 6e64 2069  packages found i
-00001560: 6e20 7468 650a 776f 726b 696e 6720 6469  n the.working di
-00001570: 7265 6374 6f72 7920 7769 6c6c 2062 6520  rectory will be 
-00001580: 6578 616d 696e 6564 2066 6f72 2070 7974  examined for pyt
-00001590: 686f 6e20 736f 7572 6365 2066 696c 6573  hon source files
-000015a0: 206f 720a 6469 7265 6374 6f72 6965 7320   or.directories 
-000015b0: 7468 6174 206d 6174 6368 2074 6573 744d  that match testM
-000015c0: 6174 6368 2e20 5061 636b 6167 6520 6469  atch. Package di
-000015d0: 7363 6f76 6572 7920 6465 7363 656e 6473  scovery descends
-000015e0: 2061 6c6c 2074 6865 0a77 6179 2064 6f77   all the.way dow
-000015f0: 6e20 7468 6520 7472 6565 2c20 736f 2070  n the tree, so p
-00001600: 6163 6b61 6765 2e74 6573 7473 2061 6e64  ackage.tests and
-00001610: 2070 6163 6b61 6765 2e73 7562 2e74 6573   package.sub.tes
-00001620: 7473 2061 6e64 0a70 6163 6b61 6765 2e73  ts and.package.s
-00001630: 7562 2e73 7562 322e 7465 7374 7320 7769  ub.sub2.tests wi
-00001640: 6c6c 2061 6c6c 2062 6520 636f 6c6c 6563  ll all be collec
-00001650: 7465 642e 0a0a 5769 7468 696e 2061 2074  ted...Within a t
-00001660: 6573 7420 6469 7265 6374 6f72 7920 6f72  est directory or
-00001670: 2070 6163 6b61 6765 2c20 616e 7920 7079   package, any py
-00001680: 7468 6f6e 2073 6f75 7263 6520 6669 6c65  thon source file
-00001690: 206d 6174 6368 696e 670a 7465 7374 4d61   matching.testMa
-000016a0: 7463 6820 7769 6c6c 2062 6520 6578 616d  tch will be exam
-000016b0: 696e 6564 2066 6f72 2074 6573 7420 6361  ined for test ca
-000016c0: 7365 732e 2057 6974 6869 6e20 6120 7465  ses. Within a te
-000016d0: 7374 206d 6f64 756c 652c 0a66 756e 6374  st module,.funct
-000016e0: 696f 6e73 2061 6e64 2063 6c61 7373 6573  ions and classes
-000016f0: 2077 686f 7365 206e 616d 6573 206d 6174   whose names mat
-00001700: 6368 2074 6573 744d 6174 6368 2061 6e64  ch testMatch and
-00001710: 2054 6573 7443 6173 650a 7375 6263 6c61   TestCase.subcla
-00001720: 7373 6573 2077 6974 6820 616e 7920 6e61  sses with any na
-00001730: 6d65 2077 696c 6c20 6265 206c 6f61 6465  me will be loade
-00001740: 6420 616e 6420 6578 6563 7574 6564 2061  d and executed a
-00001750: 7320 7465 7374 732e 2054 6573 7473 0a6d  s tests. Tests.m
-00001760: 6179 2075 7365 2074 6865 2061 7373 6572  ay use the asser
-00001770: 7420 6b65 7977 6f72 6420 6f72 2072 6169  t keyword or rai
-00001780: 7365 2041 7373 6572 7469 6f6e 4572 726f  se AssertionErro
-00001790: 7273 2074 6f20 696e 6469 6361 7465 2074  rs to indicate t
-000017a0: 6573 740a 6661 696c 7572 652e 2054 6573  est.failure. Tes
-000017b0: 7443 6173 6520 7375 6263 6c61 7373 6573  tCase subclasses
-000017c0: 206d 6179 2064 6f20 7468 6520 7361 6d65   may do the same
-000017d0: 206f 7220 7573 6520 7468 6520 7661 7269   or use the vari
-000017e0: 6f75 730a 5465 7374 4361 7365 206d 6574  ous.TestCase met
-000017f0: 686f 6473 2061 7661 696c 6162 6c65 2e0a  hods available..
-00001800: 0a2a 2a49 7420 6973 2069 6d70 6f72 7461  .**It is importa
-00001810: 6e74 2074 6f20 6e6f 7465 2074 6861 7420  nt to note that 
-00001820: 7468 6520 6465 6661 756c 7420 6265 6861  the default beha
-00001830: 7669 6f72 206f 6620 6e6f 7365 2069 7320  vior of nose is 
-00001840: 746f 206e 6f74 0a69 6e63 6c75 6465 2074  to not.include t
-00001850: 6573 7473 2066 726f 6d20 6669 6c65 7320  ests from files 
-00001860: 7768 6963 6820 6172 6520 6578 6563 7574  which are execut
-00001870: 6162 6c65 2e2a 2a20 2054 6f20 696e 636c  able.**  To incl
-00001880: 7564 6520 7465 7374 730a 6672 6f6d 2073  ude tests.from s
-00001890: 7563 6820 6669 6c65 732c 2072 656d 6f76  uch files, remov
-000018a0: 6520 7468 6569 7220 6578 6563 7574 6162  e their executab
-000018b0: 6c65 2062 6974 206f 7220 7573 6520 7468  le bit or use th
-000018c0: 6520 2d2d 6578 6520 666c 6167 0a28 7365  e --exe flag.(se
-000018d0: 6520 274f 7074 696f 6e73 2720 7365 6374  e 'Options' sect
-000018e0: 696f 6e20 6265 6c6f 7729 2e0a 0a0a 5365  ion below)....Se
-000018f0: 6c65 6374 696e 6720 5465 7374 730a 2d2d  lecting Tests.--
-00001900: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a 0a54  -------------..T
-00001910: 6f20 7370 6563 6966 7920 7768 6963 6820  o specify which 
-00001920: 7465 7374 7320 746f 2072 756e 2c20 7061  tests to run, pa
-00001930: 7373 2074 6573 7420 6e61 6d65 7320 6f6e  ss test names on
-00001940: 2074 6865 2063 6f6d 6d61 6e64 206c 696e   the command lin
-00001950: 653a 0a0a 2020 206e 6f73 6574 6573 7473  e:..   nosetests
-00001960: 206f 6e6c 795f 7465 7374 5f74 6869 732e   only_test_this.
-00001970: 7079 0a0a 5465 7374 206e 616d 6573 2073  py..Test names s
-00001980: 7065 6369 6669 6564 206d 6179 2062 6520  pecified may be 
-00001990: 6669 6c65 206f 7220 6d6f 6475 6c65 206e  file or module n
-000019a0: 616d 6573 2c20 616e 6420 6d61 7920 6f70  ames, and may op
-000019b0: 7469 6f6e 616c 6c79 0a69 6e64 6963 6174  tionally.indicat
-000019c0: 6520 7468 6520 7465 7374 2063 6173 6520  e the test case 
-000019d0: 746f 2072 756e 2062 7920 7365 7061 7261  to run by separa
-000019e0: 7469 6e67 2074 6865 206d 6f64 756c 6520  ting the module 
-000019f0: 6f72 2066 696c 6520 6e61 6d65 0a66 726f  or file name.fro
-00001a00: 6d20 7468 6520 7465 7374 2063 6173 6520  m the test case 
-00001a10: 6e61 6d65 2077 6974 6820 6120 636f 6c6f  name with a colo
-00001a20: 6e2e 2046 696c 656e 616d 6573 206d 6179  n. Filenames may
-00001a30: 2062 6520 7265 6c61 7469 7665 206f 720a   be relative or.
-00001a40: 6162 736f 6c75 7465 2e20 4578 616d 706c  absolute. Exampl
-00001a50: 6573 3a0a 0a20 2020 6e6f 7365 7465 7374  es:..   nosetest
-00001a60: 7320 7465 7374 2e6d 6f64 756c 650a 2020  s test.module.  
-00001a70: 206e 6f73 6574 6573 7473 2061 6e6f 7468   nosetests anoth
-00001a80: 6572 2e74 6573 743a 5465 7374 4361 7365  er.test:TestCase
-00001a90: 2e74 6573 745f 6d65 7468 6f64 0a20 2020  .test_method.   
-00001aa0: 6e6f 7365 7465 7374 7320 612e 7465 7374  nosetests a.test
-00001ab0: 3a54 6573 7443 6173 650a 2020 206e 6f73  :TestCase.   nos
-00001ac0: 6574 6573 7473 202f 7061 7468 2f74 6f2f  etests /path/to/
-00001ad0: 7465 7374 2f66 696c 652e 7079 3a74 6573  test/file.py:tes
-00001ae0: 745f 6675 6e63 7469 6f6e 0a0a 596f 7520  t_function..You 
-00001af0: 6d61 7920 616c 736f 2063 6861 6e67 6520  may also change 
-00001b00: 7468 6520 776f 726b 696e 6720 6469 7265  the working dire
-00001b10: 6374 6f72 7920 7768 6572 6520 6e6f 7365  ctory where nose
-00001b20: 206c 6f6f 6b73 2066 6f72 2074 6573 7473   looks for tests
-00001b30: 0a62 7920 7573 696e 6720 7468 6520 2d77  .by using the -w
-00001b40: 2073 7769 7463 683a 0a0a 2020 206e 6f73   switch:..   nos
-00001b50: 6574 6573 7473 202d 7720 2f70 6174 682f  etests -w /path/
-00001b60: 746f 2f74 6573 7473 0a0a 4e6f 7465 2c20  to/tests..Note, 
-00001b70: 686f 7765 7665 722c 2074 6861 7420 7375  however, that su
-00001b80: 7070 6f72 7420 666f 7220 6d75 6c74 6970  pport for multip
-00001b90: 6c65 202d 7720 6172 6775 6d65 6e74 7320  le -w arguments 
-00001ba0: 6973 206e 6f77 0a64 6570 7265 6361 7465  is now.deprecate
-00001bb0: 6420 616e 6420 7769 6c6c 2062 6520 7265  d and will be re
-00001bc0: 6d6f 7665 6420 696e 2061 2066 7574 7572  moved in a futur
-00001bd0: 6520 7265 6c65 6173 652e 2041 7320 6f66  e release. As of
-00001be0: 206e 6f73 6520 302e 3130 2c0a 796f 7520   nose 0.10,.you 
-00001bf0: 6361 6e20 6765 7420 7468 6520 7361 6d65  can get the same
-00001c00: 2062 6568 6176 696f 7220 6279 2073 7065   behavior by spe
-00001c10: 6369 6679 696e 6720 7468 6520 7461 7267  cifying the targ
-00001c20: 6574 2064 6972 6563 746f 7269 6573 0a2a  et directories.*
-00001c30: 7769 7468 6f75 742a 2074 6865 202d 7720  without* the -w 
-00001c40: 7377 6974 6368 3a0a 0a20 2020 6e6f 7365  switch:..   nose
-00001c50: 7465 7374 7320 2f70 6174 682f 746f 2f74  tests /path/to/t
-00001c60: 6573 7473 202f 616e 6f74 6865 722f 7061  ests /another/pa
-00001c70: 7468 2f74 6f2f 7465 7374 730a 0a46 7572  th/to/tests..Fur
-00001c80: 7468 6572 2063 7573 746f 6d69 7a61 7469  ther customizati
-00001c90: 6f6e 206f 6620 7465 7374 2073 656c 6563  on of test selec
-00001ca0: 7469 6f6e 2061 6e64 206c 6f61 6469 6e67  tion and loading
-00001cb0: 2069 7320 706f 7373 6962 6c65 0a74 6872   is possible.thr
-00001cc0: 6f75 6768 2074 6865 2075 7365 206f 6620  ough the use of 
-00001cd0: 706c 7567 696e 732e 0a0a 5465 7374 2072  plugins...Test r
-00001ce0: 6573 756c 7420 6f75 7470 7574 2069 7320  esult output is 
-00001cf0: 6964 656e 7469 6361 6c20 746f 2074 6861  identical to tha
-00001d00: 7420 6f66 2075 6e69 7474 6573 742c 2065  t of unittest, e
-00001d10: 7863 6570 7420 666f 7220 7468 650a 6164  xcept for the.ad
-00001d20: 6469 7469 6f6e 616c 2066 6561 7475 7265  ditional feature
-00001d30: 7320 2865 7272 6f72 2063 6c61 7373 6573  s (error classes
-00001d40: 2c20 616e 6420 706c 7567 696e 2d73 7570  , and plugin-sup
-00001d50: 706c 6965 6420 6665 6174 7572 6573 2073  plied features s
-00001d60: 7563 680a 6173 206f 7574 7075 7420 6361  uch.as output ca
-00001d70: 7074 7572 6520 616e 6420 6173 7365 7274  pture and assert
-00001d80: 2069 6e74 726f 7370 6563 7469 6f6e 2920   introspection) 
-00001d90: 6465 7461 696c 6564 2069 6e20 7468 6520  detailed in the 
-00001da0: 6f70 7469 6f6e 730a 6265 6c6f 772e 0a0a  options.below...
-00001db0: 0a43 6f6e 6669 6775 7261 7469 6f6e 0a2d  .Configuration.-
-00001dc0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0a0a 496e  ------------..In
-00001dd0: 2061 6464 6974 696f 6e20 746f 2070 6173   addition to pas
-00001de0: 7369 6e67 2063 6f6d 6d61 6e64 2d6c 696e  sing command-lin
-00001df0: 6520 6f70 7469 6f6e 732c 2079 6f75 206d  e options, you m
-00001e00: 6179 2061 6c73 6f20 7075 740a 636f 6e66  ay also put.conf
-00001e10: 6967 7572 6174 696f 6e20 6f70 7469 6f6e  iguration option
-00001e20: 7320 696e 2079 6f75 7220 7072 6f6a 6563  s in your projec
-00001e30: 7420 2a73 6574 7570 2e63 6667 2a20 6669  t *setup.cfg* fi
-00001e40: 6c65 2c20 6f72 2061 202e 6e6f 7365 7263  le, or a .noserc
-00001e50: 0a6f 7220 6e6f 7365 2e63 6667 2066 696c  .or nose.cfg fil
-00001e60: 6520 696e 2079 6f75 7220 686f 6d65 2064  e in your home d
-00001e70: 6972 6563 746f 7279 2e20 496e 2061 6e79  irectory. In any
-00001e80: 206f 6620 7468 6573 6520 7374 616e 6461   of these standa
-00001e90: 7264 2069 6e69 2d0a 7374 796c 6520 636f  rd ini-.style co
-00001ea0: 6e66 6967 2066 696c 6573 2c20 796f 7520  nfig files, you 
-00001eb0: 7075 7420 796f 7572 206e 6f73 6574 6573  put your nosetes
-00001ec0: 7473 2063 6f6e 6669 6775 7261 7469 6f6e  ts configuration
-00001ed0: 2069 6e20 610a 225b 6e6f 7365 7465 7374   in a."[nosetest
-00001ee0: 735d 2220 7365 6374 696f 6e2e 204f 7074  s]" section. Opt
-00001ef0: 696f 6e73 2061 7265 2074 6865 2073 616d  ions are the sam
-00001f00: 6520 6173 206f 6e20 7468 6520 636f 6d6d  e as on the comm
-00001f10: 616e 6420 6c69 6e65 2c0a 7769 7468 2074  and line,.with t
-00001f20: 6865 202d 2d20 7072 6566 6978 2072 656d  he -- prefix rem
-00001f30: 6f76 6564 2e20 466f 7220 6f70 7469 6f6e  oved. For option
-00001f40: 7320 7468 6174 2061 7265 2073 696d 706c  s that are simpl
-00001f50: 6520 7377 6974 6368 6573 2c20 796f 750a  e switches, you.
-00001f60: 6d75 7374 2073 7570 706c 7920 6120 7661  must supply a va
-00001f70: 6c75 653a 0a0a 2020 205b 6e6f 7365 7465  lue:..   [nosete
-00001f80: 7374 735d 0a20 2020 7665 7262 6f73 6974  sts].   verbosit
-00001f90: 793d 330a 2020 2077 6974 682d 646f 6374  y=3.   with-doct
-00001fa0: 6573 743d 310a 0a41 6c6c 2063 6f6e 6669  est=1..All confi
-00001fb0: 6775 7261 7469 6f6e 2066 696c 6573 2074  guration files t
-00001fc0: 6861 7420 6172 6520 666f 756e 6420 7769  hat are found wi
-00001fd0: 6c6c 2062 6520 6c6f 6164 6564 2061 6e64  ll be loaded and
-00001fe0: 2074 6865 6972 0a6f 7074 696f 6e73 2063   their.options c
-00001ff0: 6f6d 6269 6e65 642e 2059 6f75 2063 616e  ombined. You can
-00002000: 206f 7665 7272 6964 6520 7468 6520 7374   override the st
-00002010: 616e 6461 7264 2063 6f6e 6669 6720 6669  andard config fi
-00002020: 6c65 206c 6f61 6469 6e67 0a77 6974 6820  le loading.with 
-00002030: 7468 6520 222d 6322 206f 7074 696f 6e2e  the "-c" option.
-00002040: 0a0a 0a55 7369 6e67 2050 6c75 6769 6e73  ...Using Plugins
-00002050: 0a2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0a0a  .-------------..
-00002060: 5468 6572 6520 6172 6520 6e75 6d65 726f  There are numero
-00002070: 7573 206e 6f73 6520 706c 7567 696e 7320  us nose plugins 
-00002080: 6176 6169 6c61 626c 6520 7669 6120 6561  available via ea
-00002090: 7379 5f69 6e73 7461 6c6c 2061 6e64 0a65  sy_install and.e
-000020a0: 6c73 6577 6865 7265 2e20 546f 2075 7365  lsewhere. To use
-000020b0: 2061 2070 6c75 6769 6e2c 206a 7573 7420   a plugin, just 
-000020c0: 696e 7374 616c 6c20 6974 2e20 5468 6520  install it. The 
-000020d0: 706c 7567 696e 2077 696c 6c20 6164 640a  plugin will add.
-000020e0: 636f 6d6d 616e 6420 6c69 6e65 206f 7074  command line opt
-000020f0: 696f 6e73 2074 6f20 6e6f 7365 7465 7374  ions to nosetest
-00002100: 732e 2054 6f20 7665 7269 6679 2074 6861  s. To verify tha
-00002110: 7420 7468 6520 706c 7567 696e 2069 730a  t the plugin is.
-00002120: 696e 7374 616c 6c65 642c 2072 756e 3a0a  installed, run:.
-00002130: 0a20 2020 6e6f 7365 7465 7374 7320 2d2d  .   nosetests --
-00002140: 706c 7567 696e 730a 0a59 6f75 2063 616e  plugins..You can
-00002150: 2061 6464 202d 7620 6f72 202d 7676 2074   add -v or -vv t
-00002160: 6f20 7468 6174 2063 6f6d 6d61 6e64 2074  o that command t
-00002170: 6f20 7368 6f77 206d 6f72 6520 696e 666f  o show more info
-00002180: 726d 6174 696f 6e20 6162 6f75 740a 6561  rmation about.ea
-00002190: 6368 2070 6c75 6769 6e2e 0a0a 4966 2079  ch plugin...If y
-000021a0: 6f75 2061 7265 2072 756e 6e69 6e67 206e  ou are running n
-000021b0: 6f73 652e 6d61 696e 2829 206f 7220 6e6f  ose.main() or no
-000021c0: 7365 2e72 756e 2829 2066 726f 6d20 6120  se.run() from a 
-000021d0: 7363 7269 7074 2c20 796f 7520 6361 6e0a  script, you can.
-000021e0: 7370 6563 6966 7920 6120 6c69 7374 206f  specify a list o
-000021f0: 6620 706c 7567 696e 7320 746f 2075 7365  f plugins to use
-00002200: 2062 7920 7061 7373 696e 6720 6120 6c69   by passing a li
-00002210: 7374 206f 6620 706c 7567 696e 7320 7769  st of plugins wi
-00002220: 7468 2074 6865 0a70 6c75 6769 6e73 206b  th the.plugins k
-00002230: 6579 776f 7264 2061 7267 756d 656e 742e  eyword argument.
-00002240: 0a0a 0a4f 7074 696f 6e73 0a2d 2d2d 2d2d  ...Options.-----
-00002250: 2d2d 0a0a 2d56 2c20 2d2d 7665 7273 696f  --..-V, --versio
-00002260: 6e0a 0a20 2020 4f75 7470 7574 206e 6f73  n..   Output nos
-00002270: 6520 7665 7273 696f 6e20 616e 6420 6578  e version and ex
-00002280: 6974 0a0a 2d70 2c20 2d2d 706c 7567 696e  it..-p, --plugin
-00002290: 730a 0a20 2020 4f75 7470 7574 206c 6973  s..   Output lis
-000022a0: 7420 6f66 2061 7661 696c 6162 6c65 2070  t of available p
-000022b0: 6c75 6769 6e73 2061 6e64 2065 7869 742e  lugins and exit.
-000022c0: 2043 6f6d 6269 6e65 2077 6974 6820 6869   Combine with hi
-000022d0: 6768 6572 0a20 2020 7665 7262 6f73 6974  gher.   verbosit
-000022e0: 7920 666f 7220 6772 6561 7465 7220 6465  y for greater de
-000022f0: 7461 696c 0a0a 2d76 3d44 4546 4155 4c54  tail..-v=DEFAULT
-00002300: 2c20 2d2d 7665 7262 6f73 653d 4445 4641  , --verbose=DEFA
-00002310: 554c 540a 0a20 2020 4265 206d 6f72 6520  ULT..   Be more 
-00002320: 7665 7262 6f73 652e 205b 4e4f 5345 5f56  verbose. [NOSE_V
-00002330: 4552 424f 5345 5d0a 0a2d 2d76 6572 626f  ERBOSE]..--verbo
-00002340: 7369 7479 3d56 4552 424f 5349 5459 0a0a  sity=VERBOSITY..
-00002350: 2020 2053 6574 2076 6572 626f 7369 7479     Set verbosity
-00002360: 3b20 2d2d 7665 7262 6f73 6974 793d 3220  ; --verbosity=2 
-00002370: 6973 2074 6865 2073 616d 6520 6173 202d  is the same as -
-00002380: 760a 0a2d 713d 4445 4641 554c 542c 202d  v..-q=DEFAULT, -
-00002390: 2d71 7569 6574 3d44 4546 4155 4c54 0a0a  -quiet=DEFAULT..
-000023a0: 2020 2042 6520 6c65 7373 2076 6572 626f     Be less verbo
-000023b0: 7365 0a0a 2d63 3d46 494c 4553 2c20 2d2d  se..-c=FILES, --
-000023c0: 636f 6e66 6967 3d46 494c 4553 0a0a 2020  config=FILES..  
-000023d0: 204c 6f61 6420 636f 6e66 6967 7572 6174   Load configurat
-000023e0: 696f 6e20 6672 6f6d 2063 6f6e 6669 6720  ion from config 
-000023f0: 6669 6c65 2873 292e 204d 6179 2062 6520  file(s). May be 
-00002400: 7370 6563 6966 6965 6420 6d75 6c74 6970  specified multip
-00002410: 6c65 0a20 2020 7469 6d65 733b 2069 6e20  le.   times; in 
-00002420: 7468 6174 2063 6173 652c 2061 6c6c 2063  that case, all c
-00002430: 6f6e 6669 6720 6669 6c65 7320 7769 6c6c  onfig files will
-00002440: 2062 6520 6c6f 6164 6564 2061 6e64 2063   be loaded and c
-00002450: 6f6d 6269 6e65 640a 0a2d 773d 5748 4552  ombined..-w=WHER
-00002460: 452c 202d 2d77 6865 7265 3d57 4845 5245  E, --where=WHERE
-00002470: 0a0a 2020 204c 6f6f 6b20 666f 7220 7465  ..   Look for te
-00002480: 7374 7320 696e 2074 6869 7320 6469 7265  sts in this dire
-00002490: 6374 6f72 792e 204d 6179 2062 6520 7370  ctory. May be sp
-000024a0: 6563 6966 6965 6420 6d75 6c74 6970 6c65  ecified multiple
-000024b0: 2074 696d 6573 2e0a 2020 2054 6865 2066   times..   The f
-000024c0: 6972 7374 2064 6972 6563 746f 7279 2070  irst directory p
-000024d0: 6173 7365 6420 7769 6c6c 2062 6520 7573  assed will be us
-000024e0: 6564 2061 7320 7468 6520 776f 726b 696e  ed as the workin
-000024f0: 6720 6469 7265 6374 6f72 792c 0a20 2020  g directory,.   
-00002500: 696e 2070 6c61 6365 206f 6620 7468 6520  in place of the 
-00002510: 6375 7272 656e 7420 776f 726b 696e 6720  current working 
-00002520: 6469 7265 6374 6f72 792c 2077 6869 6368  directory, which
-00002530: 2069 7320 7468 6520 6465 6661 756c 742e   is the default.
-00002540: 0a20 2020 4f74 6865 7273 2077 696c 6c20  .   Others will 
-00002550: 6265 2061 6464 6564 2074 6f20 7468 6520  be added to the 
-00002560: 6c69 7374 206f 6620 7465 7374 7320 746f  list of tests to
-00002570: 2065 7865 6375 7465 2e20 5b4e 4f53 455f   execute. [NOSE_
-00002580: 5748 4552 455d 0a0a 2d2d 7079 3377 6865  WHERE]..--py3whe
-00002590: 7265 3d50 5933 5748 4552 450a 0a20 2020  re=PY3WHERE..   
-000025a0: 4c6f 6f6b 2066 6f72 2074 6573 7473 2069  Look for tests i
-000025b0: 6e20 7468 6973 2064 6972 6563 746f 7279  n this directory
-000025c0: 2075 6e64 6572 2050 7974 686f 6e20 332e   under Python 3.
-000025d0: 782e 2046 756e 6374 696f 6e73 2074 6865  x. Functions the
-000025e0: 0a20 2020 7361 6d65 2061 7320 2777 6865  .   same as 'whe
-000025f0: 7265 272c 2062 7574 206f 6e6c 7920 6170  re', but only ap
-00002600: 706c 6965 7320 6966 2072 756e 6e69 6e67  plies if running
-00002610: 2075 6e64 6572 2050 7974 686f 6e20 332e   under Python 3.
-00002620: 7820 6f72 0a20 2020 6162 6f76 652e 2020  x or.   above.  
-00002630: 4e6f 7465 2074 6861 742c 2069 6620 7072  Note that, if pr
-00002640: 6573 656e 7420 756e 6465 7220 332e 782c  esent under 3.x,
-00002650: 2074 6869 7320 6f70 7469 6f6e 2063 6f6d   this option com
-00002660: 706c 6574 656c 790a 2020 2072 6570 6c61  pletely.   repla
-00002670: 6365 7320 616e 7920 6469 7265 6374 6f72  ces any director
-00002680: 6965 7320 7370 6563 6966 6965 6420 7769  ies specified wi
-00002690: 7468 2027 7768 6572 6527 2c20 736f 2074  th 'where', so t
-000026a0: 6865 2027 7768 6572 6527 0a20 2020 6f70  he 'where'.   op
-000026b0: 7469 6f6e 2062 6563 6f6d 6573 2069 6e65  tion becomes ine
-000026c0: 6666 6563 7469 7665 2e20 5b4e 4f53 455f  ffective. [NOSE_
-000026d0: 5059 3357 4845 5245 5d0a 0a2d 6d3d 5245  PY3WHERE]..-m=RE
-000026e0: 4745 582c 202d 2d6d 6174 6368 3d52 4547  GEX, --match=REG
-000026f0: 4558 2c20 2d2d 7465 7374 6d61 7463 683d  EX, --testmatch=
-00002700: 5245 4745 580a 0a20 2020 4669 6c65 732c  REGEX..   Files,
-00002710: 2064 6972 6563 746f 7269 6573 2c20 6675   directories, fu
-00002720: 6e63 7469 6f6e 206e 616d 6573 2c20 616e  nction names, an
-00002730: 6420 636c 6173 7320 6e61 6d65 7320 7468  d class names th
-00002740: 6174 206d 6174 6368 2074 6869 730a 2020  at match this.  
-00002750: 2072 6567 756c 6172 2065 7870 7265 7373   regular express
-00002760: 696f 6e20 6172 6520 636f 6e73 6964 6572  ion are consider
-00002770: 6564 2074 6573 7473 2e20 2044 6566 6175  ed tests.  Defau
-00002780: 6c74 3a0a 2020 2028 3f3a 5e7c 5b62 5f2e  lt:.   (?:^|[b_.
-00002790: 2f2d 5d29 5b54 745d 6573 7420 5b4e 4f53  /-])[Tt]est [NOS
-000027a0: 455f 5445 5354 4d41 5443 485d 0a0a 2d2d  E_TESTMATCH]..--
-000027b0: 7465 7374 733d 4e41 4d45 530a 0a20 2020  tests=NAMES..   
-000027c0: 5275 6e20 7468 6573 6520 7465 7374 7320  Run these tests 
-000027d0: 2863 6f6d 6d61 2d73 6570 6172 6174 6564  (comma-separated
-000027e0: 206c 6973 7429 2e20 5468 6973 2061 7267   list). This arg
-000027f0: 756d 656e 7420 6973 2075 7365 6675 6c0a  ument is useful.
-00002800: 2020 206d 6169 6e6c 7920 6672 6f6d 2063     mainly from c
-00002810: 6f6e 6669 6775 7261 7469 6f6e 2066 696c  onfiguration fil
-00002820: 6573 3b20 6f6e 2074 6865 2063 6f6d 6d61  es; on the comma
-00002830: 6e64 206c 696e 652c 206a 7573 7420 7061  nd line, just pa
-00002840: 7373 2074 6865 0a20 2020 7465 7374 7320  ss the.   tests 
-00002850: 746f 2072 756e 2061 7320 6164 6469 7469  to run as additi
-00002860: 6f6e 616c 2061 7267 756d 656e 7473 2077  onal arguments w
-00002870: 6974 6820 6e6f 2073 7769 7463 682e 0a0a  ith no switch...
-00002880: 2d6c 3d44 4546 4155 4c54 2c20 2d2d 6465  -l=DEFAULT, --de
-00002890: 6275 673d 4445 4641 554c 540a 0a20 2020  bug=DEFAULT..   
-000028a0: 4163 7469 7661 7465 2064 6562 7567 206c  Activate debug l
-000028b0: 6f67 6769 6e67 2066 6f72 206f 6e65 206f  ogging for one o
-000028c0: 7220 6d6f 7265 2073 7973 7465 6d73 2e20  r more systems. 
-000028d0: 4176 6169 6c61 626c 6520 6465 6275 670a  Available debug.
-000028e0: 2020 206c 6f67 6765 7273 3a20 6e6f 7365     loggers: nose
-000028f0: 2c20 6e6f 7365 2e69 6d70 6f72 7465 722c  , nose.importer,
-00002900: 206e 6f73 652e 696e 7370 6563 746f 722c   nose.inspector,
-00002910: 206e 6f73 652e 706c 7567 696e 732c 0a20   nose.plugins,. 
-00002920: 2020 6e6f 7365 2e72 6573 756c 7420 616e    nose.result an
-00002930: 6420 6e6f 7365 2e73 656c 6563 746f 722e  d nose.selector.
-00002940: 2053 6570 6172 6174 6520 6d75 6c74 6970   Separate multip
-00002950: 6c65 206e 616d 6573 2077 6974 6820 610a  le names with a.
-00002960: 2020 2063 6f6d 6d61 2e0a 0a2d 2d64 6562     comma...--deb
-00002970: 7567 2d6c 6f67 3d46 494c 450a 0a20 2020  ug-log=FILE..   
-00002980: 4c6f 6720 6465 6275 6720 6d65 7373 6167  Log debug messag
-00002990: 6573 2074 6f20 7468 6973 2066 696c 6520  es to this file 
-000029a0: 2864 6566 6175 6c74 3a20 7379 732e 7374  (default: sys.st
-000029b0: 6465 7272 290a 0a2d 2d6c 6f67 6769 6e67  derr)..--logging
-000029c0: 2d63 6f6e 6669 673d 4649 4c45 2c20 2d2d  -config=FILE, --
-000029d0: 6c6f 672d 636f 6e66 6967 3d46 494c 450a  log-config=FILE.
-000029e0: 0a20 2020 4c6f 6164 206c 6f67 6769 6e67  .   Load logging
-000029f0: 2063 6f6e 6669 6720 6672 6f6d 2074 6869   config from thi
-00002a00: 7320 6669 6c65 202d 2d20 6279 7061 7373  s file -- bypass
-00002a10: 6573 2061 6c6c 206f 7468 6572 206c 6f67  es all other log
-00002a20: 6769 6e67 0a20 2020 636f 6e66 6967 2073  ging.   config s
-00002a30: 6574 7469 6e67 732e 0a0a 2d49 3d52 4547  ettings...-I=REG
-00002a40: 4558 2c20 2d2d 6967 6e6f 7265 2d66 696c  EX, --ignore-fil
-00002a50: 6573 3d52 4547 4558 0a0a 2020 2043 6f6d  es=REGEX..   Com
-00002a60: 706c 6574 656c 7920 6967 6e6f 7265 2061  pletely ignore a
-00002a70: 6e79 2066 696c 6520 7468 6174 206d 6174  ny file that mat
-00002a80: 6368 6573 2074 6869 7320 7265 6775 6c61  ches this regula
-00002a90: 7220 6578 7072 6573 7369 6f6e 2e0a 2020  r expression..  
-00002aa0: 2054 616b 6573 2070 7265 6365 6465 6e63   Takes precedenc
-00002ab0: 6520 6f76 6572 2061 6e79 206f 7468 6572  e over any other
-00002ac0: 2073 6574 7469 6e67 7320 6f72 2070 6c75   settings or plu
-00002ad0: 6769 6e73 2e20 5370 6563 6966 7969 6e67  gins. Specifying
-00002ae0: 0a20 2020 7468 6973 206f 7074 696f 6e20  .   this option 
-00002af0: 7769 6c6c 2072 6570 6c61 6365 2074 6865  will replace the
-00002b00: 2064 6566 6175 6c74 2073 6574 7469 6e67   default setting
-00002b10: 2e20 5370 6563 6966 7920 7468 6973 206f  . Specify this o
-00002b20: 7074 696f 6e0a 2020 206d 756c 7469 706c  ption.   multipl
-00002b30: 6520 7469 6d65 7320 746f 2061 6464 206d  e times to add m
-00002b40: 6f72 6520 7265 6775 6c61 7220 6578 7072  ore regular expr
-00002b50: 6573 7369 6f6e 7320 5b4e 4f53 455f 4947  essions [NOSE_IG
-00002b60: 4e4f 5245 5f46 494c 4553 5d0a 0a2d 653d  NORE_FILES]..-e=
-00002b70: 5245 4745 582c 202d 2d65 7863 6c75 6465  REGEX, --exclude
-00002b80: 3d52 4547 4558 0a0a 2020 2044 6f20 6e6f  =REGEX..   Do no
-00002b90: 7420 7275 6e20 7465 7374 7320 7468 6174  t run tests that
-00002ba0: 206d 6174 6368 2072 6567 756c 6172 2065   match regular e
-00002bb0: 7870 7265 7373 696f 6e20 5b4e 4f53 455f  xpression [NOSE_
-00002bc0: 4558 434c 5544 455d 0a0a 2d69 3d52 4547  EXCLUDE]..-i=REG
-00002bd0: 4558 2c20 2d2d 696e 636c 7564 653d 5245  EX, --include=RE
-00002be0: 4745 580a 0a20 2020 5468 6973 2072 6567  GEX..   This reg
-00002bf0: 756c 6172 2065 7870 7265 7373 696f 6e20  ular expression 
-00002c00: 7769 6c6c 2062 6520 6170 706c 6965 6420  will be applied 
-00002c10: 746f 2066 696c 6573 2c20 6469 7265 6374  to files, direct
-00002c20: 6f72 6965 732c 0a20 2020 6675 6e63 7469  ories,.   functi
-00002c30: 6f6e 206e 616d 6573 2c20 616e 6420 636c  on names, and cl
-00002c40: 6173 7320 6e61 6d65 7320 666f 7220 6120  ass names for a 
-00002c50: 6368 616e 6365 2074 6f20 696e 636c 7564  chance to includ
-00002c60: 6520 6164 6469 7469 6f6e 616c 0a20 2020  e additional.   
-00002c70: 7465 7374 7320 7468 6174 2064 6f20 6e6f  tests that do no
-00002c80: 7420 6d61 7463 6820 5445 5354 4d41 5443  t match TESTMATC
-00002c90: 482e 2020 5370 6563 6966 7920 7468 6973  H.  Specify this
-00002ca0: 206f 7074 696f 6e20 6d75 6c74 6970 6c65   option multiple
-00002cb0: 0a20 2020 7469 6d65 7320 746f 2061 6464  .   times to add
-00002cc0: 206d 6f72 6520 7265 6775 6c61 7220 6578   more regular ex
-00002cd0: 7072 6573 7369 6f6e 7320 5b4e 4f53 455f  pressions [NOSE_
-00002ce0: 494e 434c 5544 455d 0a0a 2d78 2c20 2d2d  INCLUDE]..-x, --
-00002cf0: 7374 6f70 0a0a 2020 2053 746f 7020 7275  stop..   Stop ru
-00002d00: 6e6e 696e 6720 7465 7374 7320 6166 7465  nning tests afte
-00002d10: 7220 7468 6520 6669 7273 7420 6572 726f  r the first erro
-00002d20: 7220 6f72 2066 6169 6c75 7265 0a0a 2d50  r or failure..-P
-00002d30: 2c20 2d2d 6e6f 2d70 6174 682d 6164 6a75  , --no-path-adju
-00002d40: 7374 6d65 6e74 0a0a 2020 2044 6f20 6e6f  stment..   Do no
-00002d50: 7420 6d61 6b65 2061 6e79 2063 6861 6e67  t make any chang
-00002d60: 6573 2074 6f20 7379 732e 7061 7468 2077  es to sys.path w
-00002d70: 6865 6e20 6c6f 6164 696e 6720 7465 7374  hen loading test
-00002d80: 7320 5b4e 4f53 455f 4e4f 5041 5448 5d0a  s [NOSE_NOPATH].
-00002d90: 0a2d 2d65 7865 0a0a 2020 204c 6f6f 6b20  .--exe..   Look 
-00002da0: 666f 7220 7465 7374 7320 696e 2070 7974  for tests in pyt
-00002db0: 686f 6e20 6d6f 6475 6c65 7320 7468 6174  hon modules that
-00002dc0: 2061 7265 2065 7865 6375 7461 626c 652e   are executable.
-00002dd0: 204e 6f72 6d61 6c0a 2020 2062 6568 6176   Normal.   behav
-00002de0: 696f 7220 6973 2074 6f20 6578 636c 7564  ior is to exclud
-00002df0: 6520 6578 6563 7574 6162 6c65 206d 6f64  e executable mod
-00002e00: 756c 6573 2c20 7369 6e63 6520 7468 6579  ules, since they
-00002e10: 206d 6179 206e 6f74 2062 650a 2020 2069   may not be.   i
-00002e20: 6d70 6f72 742d 7361 6665 205b 4e4f 5345  mport-safe [NOSE
-00002e30: 5f49 4e43 4c55 4445 5f45 5845 5d0a 0a2d  _INCLUDE_EXE]..-
-00002e40: 2d6e 6f65 7865 0a0a 2020 2044 4f20 4e4f  -noexe..   DO NO
-00002e50: 5420 6c6f 6f6b 2066 6f72 2074 6573 7473  T look for tests
-00002e60: 2069 6e20 7079 7468 6f6e 206d 6f64 756c   in python modul
-00002e70: 6573 2074 6861 7420 6172 6520 6578 6563  es that are exec
-00002e80: 7574 6162 6c65 2e20 2854 6865 0a20 2020  utable. (The.   
-00002e90: 6465 6661 756c 7420 6f6e 2074 6865 2077  default on the w
-00002ea0: 696e 646f 7773 2070 6c61 7466 6f72 6d20  indows platform 
-00002eb0: 6973 2074 6f20 646f 2073 6f2e 290a 0a2d  is to do so.)..-
-00002ec0: 2d74 7261 7665 7273 652d 6e61 6d65 7370  -traverse-namesp
-00002ed0: 6163 650a 0a20 2020 5472 6176 6572 7365  ace..   Traverse
-00002ee0: 2074 6872 6f75 6768 2061 6c6c 2070 6174   through all pat
-00002ef0: 6820 656e 7472 6965 7320 6f66 2061 206e  h entries of a n
-00002f00: 616d 6573 7061 6365 2070 6163 6b61 6765  amespace package
-00002f10: 0a0a 2d2d 6669 7273 742d 7061 636b 6167  ..--first-packag
-00002f20: 652d 7769 6e73 2c20 2d2d 6669 7273 742d  e-wins, --first-
-00002f30: 706b 672d 7769 6e73 2c20 2d2d 3173 742d  pkg-wins, --1st-
-00002f40: 706b 672d 7769 6e73 0a0a 2020 2054 6865  pkg-wins..   The
-00002f50: 206e 6f73 6520 696d 706f 7274 6572 2077   nose importer w
-00002f60: 696c 6c20 6e6f 726d 616c 6c79 2065 7669  ill normally evi
-00002f70: 6374 2061 2070 6163 6b61 6765 2066 726f  ct a package fro
-00002f80: 6d20 7379 732e 6d6f 6475 6c65 7320 6966  m sys.modules if
-00002f90: 0a20 2020 6974 2073 6565 7320 6120 7061  .   it sees a pa
-00002fa0: 636b 6167 6520 7769 7468 2074 6865 2073  ckage with the s
-00002fb0: 616d 6520 6e61 6d65 2069 6e20 6120 6469  ame name in a di
-00002fc0: 6666 6572 656e 7420 6c6f 6361 7469 6f6e  fferent location
-00002fd0: 2e20 5365 740a 2020 2074 6869 7320 6f70  . Set.   this op
-00002fe0: 7469 6f6e 2074 6f20 6469 7361 626c 6520  tion to disable 
-00002ff0: 7468 6174 2062 6568 6176 696f 722e 0a0a  that behavior...
-00003000: 2d2d 6e6f 2d62 7974 652d 636f 6d70 696c  --no-byte-compil
-00003010: 650a 0a20 2020 5072 6576 656e 7420 6e6f  e..   Prevent no
-00003020: 7365 2066 726f 6d20 6279 7465 2d63 6f6d  se from byte-com
-00003030: 7069 6c69 6e67 2074 6865 2073 6f75 7263  piling the sourc
-00003040: 6520 696e 746f 202e 7079 6320 6669 6c65  e into .pyc file
-00003050: 7320 7768 696c 650a 2020 206e 6f73 6520  s while.   nose 
-00003060: 6973 2073 6361 6e6e 696e 6720 666f 7220  is scanning for 
-00003070: 616e 6420 7275 6e6e 696e 6720 7465 7374  and running test
-00003080: 732e 0a0a 2d61 3d41 5454 522c 202d 2d61  s...-a=ATTR, --a
-00003090: 7474 723d 4154 5452 0a0a 2020 2052 756e  ttr=ATTR..   Run
-000030a0: 206f 6e6c 7920 7465 7374 7320 7468 6174   only tests that
-000030b0: 2068 6176 6520 6174 7472 6962 7574 6573   have attributes
-000030c0: 2073 7065 6369 6669 6564 2062 7920 4154   specified by AT
-000030d0: 5452 205b 4e4f 5345 5f41 5454 525d 0a0a  TR [NOSE_ATTR]..
-000030e0: 2d41 3d45 5850 522c 202d 2d65 7661 6c2d  -A=EXPR, --eval-
-000030f0: 6174 7472 3d45 5850 520a 0a20 2020 5275  attr=EXPR..   Ru
-00003100: 6e20 6f6e 6c79 2074 6573 7473 2066 6f72  n only tests for
-00003110: 2077 686f 7365 2061 7474 7269 6275 7465   whose attribute
-00003120: 7320 7468 6520 5079 7468 6f6e 2065 7870  s the Python exp
-00003130: 7265 7373 696f 6e20 4558 5052 0a20 2020  ression EXPR.   
-00003140: 6576 616c 7561 7465 7320 746f 2054 7275  evaluates to Tru
-00003150: 6520 5b4e 4f53 455f 4556 414c 5f41 5454  e [NOSE_EVAL_ATT
-00003160: 525d 0a0a 2d73 2c20 2d2d 6e6f 6361 7074  R]..-s, --nocapt
-00003170: 7572 650a 0a20 2020 446f 206e 6f74 2063  ure..   Do not c
-00003180: 6170 7475 7265 2073 7464 6f75 7420 2861  apture stdout (a
-00003190: 6e79 2073 7464 6f75 7420 6f75 7470 7574  ny stdout output
-000031a0: 2077 696c 6c20 6265 2070 7269 6e74 6564   will be printed
-000031b0: 0a20 2020 696d 6d65 6469 6174 656c 7929  .   immediately)
-000031c0: 205b 4e4f 5345 5f4e 4f43 4150 5455 5245   [NOSE_NOCAPTURE
-000031d0: 5d0a 0a2d 2d6e 6f6c 6f67 6361 7074 7572  ]..--nologcaptur
-000031e0: 650a 0a20 2020 4469 7361 626c 6520 6c6f  e..   Disable lo
-000031f0: 6767 696e 6720 6361 7074 7572 6520 706c  gging capture pl
-00003200: 7567 696e 2e20 4c6f 6767 696e 6720 636f  ugin. Logging co
-00003210: 6e66 6967 7572 6174 696f 6e20 7769 6c6c  nfiguration will
-00003220: 2062 6520 6c65 6674 0a20 2020 696e 7461   be left.   inta
-00003230: 6374 2e20 5b4e 4f53 455f 4e4f 4c4f 4743  ct. [NOSE_NOLOGC
-00003240: 4150 5455 5245 5d0a 0a2d 2d6c 6f67 6769  APTURE]..--loggi
-00003250: 6e67 2d66 6f72 6d61 743d 464f 524d 4154  ng-format=FORMAT
-00003260: 0a0a 2020 2053 7065 6369 6679 2063 7573  ..   Specify cus
-00003270: 746f 6d20 666f 726d 6174 2074 6f20 7072  tom format to pr
-00003280: 696e 7420 7374 6174 656d 656e 7473 2e20  int statements. 
-00003290: 5573 6573 2074 6865 2073 616d 6520 666f  Uses the same fo
-000032a0: 726d 6174 2061 730a 2020 2075 7365 6420  rmat as.   used 
-000032b0: 6279 2073 7461 6e64 6172 6420 6c6f 6767  by standard logg
-000032c0: 696e 6720 6861 6e64 6c65 7273 2e20 5b4e  ing handlers. [N
-000032d0: 4f53 455f 4c4f 4746 4f52 4d41 545d 0a0a  OSE_LOGFORMAT]..
-000032e0: 2d2d 6c6f 6767 696e 672d 6461 7465 666d  --logging-datefm
-000032f0: 743d 464f 524d 4154 0a0a 2020 2053 7065  t=FORMAT..   Spe
-00003300: 6369 6679 2063 7573 746f 6d20 6461 7465  cify custom date
-00003310: 2f74 696d 6520 666f 726d 6174 2074 6f20  /time format to 
-00003320: 7072 696e 7420 7374 6174 656d 656e 7473  print statements
-00003330: 2e20 5573 6573 2074 6865 2073 616d 650a  . Uses the same.
-00003340: 2020 2066 6f72 6d61 7420 6173 2075 7365     format as use
-00003350: 6420 6279 2073 7461 6e64 6172 6420 6c6f  d by standard lo
-00003360: 6767 696e 6720 6861 6e64 6c65 7273 2e20  gging handlers. 
-00003370: 5b4e 4f53 455f 4c4f 4744 4154 4546 4d54  [NOSE_LOGDATEFMT
-00003380: 5d0a 0a2d 2d6c 6f67 6769 6e67 2d66 696c  ]..--logging-fil
-00003390: 7465 723d 4649 4c54 4552 0a0a 2020 2053  ter=FILTER..   S
-000033a0: 7065 6369 6679 2077 6869 6368 2073 7461  pecify which sta
-000033b0: 7465 6d65 6e74 7320 746f 2066 696c 7465  tements to filte
-000033c0: 7220 696e 2f6f 7574 2e20 4279 2064 6566  r in/out. By def
-000033d0: 6175 6c74 2c20 6576 6572 7974 6869 6e67  ault, everything
-000033e0: 0a20 2020 6973 2063 6170 7475 7265 642e  .   is captured.
-000033f0: 2049 6620 7468 6520 6f75 7470 7574 2069   If the output i
-00003400: 7320 746f 6f20 7665 7262 6f73 652c 2075  s too verbose, u
-00003410: 7365 2074 6869 7320 6f70 7469 6f6e 2074  se this option t
-00003420: 6f0a 2020 2066 696c 7465 7220 6f75 7420  o.   filter out 
-00003430: 6e65 6564 6c65 7373 206f 7574 7075 742e  needless output.
-00003440: 2045 7861 6d70 6c65 3a20 6669 6c74 6572   Example: filter
-00003450: 3d66 6f6f 2077 696c 6c20 6361 7074 7572  =foo will captur
-00003460: 650a 2020 2073 7461 7465 6d65 6e74 7320  e.   statements 
-00003470: 6973 7375 6564 204f 4e4c 5920 746f 2020  issued ONLY to  
-00003480: 666f 6f20 6f72 2066 6f6f 2e77 6861 742e  foo or foo.what.
-00003490: 6576 6572 2e73 7562 2062 7574 206e 6f74  ever.sub but not
-000034a0: 2066 6f6f 6261 720a 2020 206f 7220 6f74   foobar.   or ot
-000034b0: 6865 7220 6c6f 6767 6572 2e20 5370 6563  her logger. Spec
-000034c0: 6966 7920 6d75 6c74 6970 6c65 206c 6f67  ify multiple log
-000034d0: 6765 7273 2077 6974 6820 636f 6d6d 613a  gers with comma:
-000034e0: 0a20 2020 6669 6c74 6572 3d66 6f6f 2c62  .   filter=foo,b
-000034f0: 6172 2c62 617a 2e20 4966 2061 6e79 206c  ar,baz. If any l
-00003500: 6f67 6765 7220 6e61 6d65 2069 7320 7072  ogger name is pr
-00003510: 6566 6978 6564 2077 6974 6820 6120 6d69  efixed with a mi
-00003520: 6e75 732c 2065 670a 2020 2066 696c 7465  nus, eg.   filte
-00003530: 723d 2d66 6f6f 2c20 6974 2077 696c 6c20  r=-foo, it will 
-00003540: 6265 2065 7863 6c75 6465 6420 7261 7468  be excluded rath
-00003550: 6572 2074 6861 6e20 696e 636c 7564 6564  er than included
-00003560: 2e20 4465 6661 756c 743a 0a20 2020 6578  . Default:.   ex
-00003570: 636c 7564 6520 6c6f 6767 696e 6720 6d65  clude logging me
-00003580: 7373 6167 6573 2066 726f 6d20 6e6f 7365  ssages from nose
-00003590: 2069 7473 656c 6620 282d 6e6f 7365 292e   itself (-nose).
-000035a0: 205b 4e4f 5345 5f4c 4f47 4649 4c54 4552   [NOSE_LOGFILTER
-000035b0: 5d0a 0a2d 2d6c 6f67 6769 6e67 2d63 6c65  ]..--logging-cle
-000035c0: 6172 2d68 616e 646c 6572 730a 0a20 2020  ar-handlers..   
-000035d0: 436c 6561 7220 616c 6c20 6f74 6865 7220  Clear all other 
-000035e0: 6c6f 6767 696e 6720 6861 6e64 6c65 7273  logging handlers
-000035f0: 0a0a 2d2d 6c6f 6767 696e 672d 6c65 7665  ..--logging-leve
-00003600: 6c3d 4445 4641 554c 540a 0a20 2020 5365  l=DEFAULT..   Se
-00003610: 7420 7468 6520 6c6f 6720 6c65 7665 6c20  t the log level 
-00003620: 746f 2063 6170 7475 7265 0a0a 2d2d 7769  to capture..--wi
-00003630: 7468 2d63 6f76 6572 6167 650a 0a20 2020  th-coverage..   
-00003640: 456e 6162 6c65 2070 6c75 6769 6e20 436f  Enable plugin Co
-00003650: 7665 7261 6765 3a20 4163 7469 7661 7465  verage: Activate
-00003660: 2061 2063 6f76 6572 6167 6520 7265 706f   a coverage repo
-00003670: 7274 2075 7369 6e67 2074 6865 0a20 2020  rt using the.   
-00003680: 4e65 6420 4261 7463 6865 6c64 6572 2063  Ned Batchelder c
-00003690: 6f76 6572 6167 6520 6d6f 6475 6c65 2e20  overage module. 
-000036a0: 5b4e 4f53 455f 5749 5448 5f43 4f56 4552  [NOSE_WITH_COVER
-000036b0: 4147 455d 0a0a 2d2d 636f 7665 722d 7061  AGE]..--cover-pa
-000036c0: 636b 6167 653d 5041 434b 4147 450a 0a20  ckage=PACKAGE.. 
-000036d0: 2020 5265 7374 7269 6374 2063 6f76 6572    Restrict cover
-000036e0: 6167 6520 6f75 7470 7574 2074 6f20 7365  age output to se
-000036f0: 6c65 6374 6564 2070 6163 6b61 6765 7320  lected packages 
-00003700: 5b4e 4f53 455f 434f 5645 525f 5041 434b  [NOSE_COVER_PACK
-00003710: 4147 455d 0a0a 2d2d 636f 7665 722d 6572  AGE]..--cover-er
-00003720: 6173 650a 0a20 2020 4572 6173 6520 7072  ase..   Erase pr
-00003730: 6576 696f 7573 6c79 2063 6f6c 6c65 6374  eviously collect
-00003740: 6564 2063 6f76 6572 6167 6520 7374 6174  ed coverage stat
-00003750: 6973 7469 6373 2062 6566 6f72 6520 7275  istics before ru
-00003760: 6e0a 0a2d 2d63 6f76 6572 2d74 6573 7473  n..--cover-tests
-00003770: 0a0a 2020 2049 6e63 6c75 6465 2074 6573  ..   Include tes
-00003780: 7420 6d6f 6475 6c65 7320 696e 2063 6f76  t modules in cov
-00003790: 6572 6167 6520 7265 706f 7274 205b 4e4f  erage report [NO
-000037a0: 5345 5f43 4f56 4552 5f54 4553 5453 5d0a  SE_COVER_TESTS].
-000037b0: 0a2d 2d63 6f76 6572 2d6d 696e 2d70 6572  .--cover-min-per
-000037c0: 6365 6e74 6167 653d 4445 4641 554c 540a  centage=DEFAULT.
-000037d0: 0a20 2020 4d69 6e69 6d75 6d20 7065 7263  .   Minimum perc
-000037e0: 656e 7461 6765 206f 6620 636f 7665 7261  entage of covera
-000037f0: 6765 2066 6f72 2074 6573 7473 2074 6f20  ge for tests to 
-00003800: 7061 7373 0a20 2020 5b4e 4f53 455f 434f  pass.   [NOSE_CO
-00003810: 5645 525f 4d49 4e5f 5045 5243 454e 5441  VER_MIN_PERCENTA
-00003820: 4745 5d0a 0a2d 2d63 6f76 6572 2d69 6e63  GE]..--cover-inc
-00003830: 6c75 7369 7665 0a0a 2020 2049 6e63 6c75  lusive..   Inclu
-00003840: 6465 2061 6c6c 2070 7974 686f 6e20 6669  de all python fi
-00003850: 6c65 7320 756e 6465 7220 776f 726b 696e  les under workin
-00003860: 6720 6469 7265 6374 6f72 7920 696e 2063  g directory in c
-00003870: 6f76 6572 6167 650a 2020 2072 6570 6f72  overage.   repor
-00003880: 742e 2020 5573 6566 756c 2066 6f72 2064  t.  Useful for d
-00003890: 6973 636f 7665 7269 6e67 2068 6f6c 6573  iscovering holes
-000038a0: 2069 6e20 7465 7374 2063 6f76 6572 6167   in test coverag
-000038b0: 6520 6966 206e 6f74 2061 6c6c 0a20 2020  e if not all.   
-000038c0: 6669 6c65 7320 6172 6520 696d 706f 7274  files are import
-000038d0: 6564 2062 7920 7468 6520 7465 7374 2073  ed by the test s
-000038e0: 7569 7465 2e20 5b4e 4f53 455f 434f 5645  uite. [NOSE_COVE
-000038f0: 525f 494e 434c 5553 4956 455d 0a0a 2d2d  R_INCLUSIVE]..--
-00003900: 636f 7665 722d 6874 6d6c 0a0a 2020 2050  cover-html..   P
-00003910: 726f 6475 6365 2048 544d 4c20 636f 7665  roduce HTML cove
-00003920: 7261 6765 2069 6e66 6f72 6d61 7469 6f6e  rage information
-00003930: 0a0a 2d2d 636f 7665 722d 6874 6d6c 2d64  ..--cover-html-d
-00003940: 6972 3d44 4952 0a0a 2020 2050 726f 6475  ir=DIR..   Produ
-00003950: 6365 2048 544d 4c20 636f 7665 7261 6765  ce HTML coverage
-00003960: 2069 6e66 6f72 6d61 7469 6f6e 2069 6e20   information in 
-00003970: 6469 720a 0a2d 2d63 6f76 6572 2d62 7261  dir..--cover-bra
-00003980: 6e63 6865 730a 0a20 2020 496e 636c 7564  nches..   Includ
-00003990: 6520 6272 616e 6368 2063 6f76 6572 6167  e branch coverag
-000039a0: 6520 696e 2063 6f76 6572 6167 6520 7265  e in coverage re
-000039b0: 706f 7274 205b 4e4f 5345 5f43 4f56 4552  port [NOSE_COVER
-000039c0: 5f42 5241 4e43 4845 535d 0a0a 2d2d 636f  _BRANCHES]..--co
-000039d0: 7665 722d 786d 6c0a 0a20 2020 5072 6f64  ver-xml..   Prod
-000039e0: 7563 6520 584d 4c20 636f 7665 7261 6765  uce XML coverage
-000039f0: 2069 6e66 6f72 6d61 7469 6f6e 0a0a 2d2d   information..--
-00003a00: 636f 7665 722d 786d 6c2d 6669 6c65 3d46  cover-xml-file=F
-00003a10: 494c 450a 0a20 2020 5072 6f64 7563 6520  ILE..   Produce 
-00003a20: 584d 4c20 636f 7665 7261 6765 2069 6e66  XML coverage inf
-00003a30: 6f72 6d61 7469 6f6e 2069 6e20 6669 6c65  ormation in file
-00003a40: 0a0a 2d2d 7064 620a 0a20 2020 4472 6f70  ..--pdb..   Drop
-00003a50: 2069 6e74 6f20 6465 6275 6767 6572 206f   into debugger o
-00003a60: 6e20 6661 696c 7572 6573 206f 7220 6572  n failures or er
-00003a70: 726f 7273 0a0a 2d2d 7064 622d 6661 696c  rors..--pdb-fail
-00003a80: 7572 6573 0a0a 2020 2044 726f 7020 696e  ures..   Drop in
-00003a90: 746f 2064 6562 7567 6765 7220 6f6e 2066  to debugger on f
-00003aa0: 6169 6c75 7265 730a 0a2d 2d70 6462 2d65  ailures..--pdb-e
-00003ab0: 7272 6f72 730a 0a20 2020 4472 6f70 2069  rrors..   Drop i
-00003ac0: 6e74 6f20 6465 6275 6767 6572 206f 6e20  nto debugger on 
-00003ad0: 6572 726f 7273 0a0a 2d2d 6e6f 2d64 6570  errors..--no-dep
-00003ae0: 7265 6361 7465 640a 0a20 2020 4469 7361  recated..   Disa
-00003af0: 626c 6520 7370 6563 6961 6c20 6861 6e64  ble special hand
-00003b00: 6c69 6e67 206f 6620 4465 7072 6563 6174  ling of Deprecat
-00003b10: 6564 5465 7374 2065 7863 6570 7469 6f6e  edTest exception
-00003b20: 732e 0a0a 2d2d 7769 7468 2d64 6f63 7465  s...--with-docte
-00003b30: 7374 0a0a 2020 2045 6e61 626c 6520 706c  st..   Enable pl
-00003b40: 7567 696e 2044 6f63 7465 7374 3a20 4163  ugin Doctest: Ac
-00003b50: 7469 7661 7465 2064 6f63 7465 7374 2070  tivate doctest p
-00003b60: 6c75 6769 6e20 746f 2066 696e 6420 616e  lugin to find an
-00003b70: 6420 7275 6e0a 2020 2064 6f63 7465 7374  d run.   doctest
-00003b80: 7320 696e 206e 6f6e 2d74 6573 7420 6d6f  s in non-test mo
-00003b90: 6475 6c65 732e 205b 4e4f 5345 5f57 4954  dules. [NOSE_WIT
-00003ba0: 485f 444f 4354 4553 545d 0a0a 2d2d 646f  H_DOCTEST]..--do
-00003bb0: 6374 6573 742d 7465 7374 730a 0a20 2020  ctest-tests..   
-00003bc0: 416c 736f 206c 6f6f 6b20 666f 7220 646f  Also look for do
-00003bd0: 6374 6573 7473 2069 6e20 7465 7374 206d  ctests in test m
-00003be0: 6f64 756c 6573 2e20 4e6f 7465 2074 6861  odules. Note tha
-00003bf0: 7420 636c 6173 7365 732c 206d 6574 686f  t classes, metho
-00003c00: 6473 0a20 2020 616e 6420 6675 6e63 7469  ds.   and functi
-00003c10: 6f6e 7320 7368 6f75 6c64 2068 6176 6520  ons should have 
-00003c20: 6569 7468 6572 2064 6f63 7465 7374 7320  either doctests 
-00003c30: 6f72 206e 6f6e 2d64 6f63 7465 7374 2074  or non-doctest t
-00003c40: 6573 7473 2c20 6e6f 740a 2020 2062 6f74  ests, not.   bot
-00003c50: 682e 205b 4e4f 5345 5f44 4f43 5445 5354  h. [NOSE_DOCTEST
-00003c60: 5f54 4553 5453 5d0a 0a2d 2d64 6f63 7465  _TESTS]..--docte
-00003c70: 7374 2d65 7874 656e 7369 6f6e 3d45 5854  st-extension=EXT
-00003c80: 0a0a 2020 2041 6c73 6f20 6c6f 6f6b 2066  ..   Also look f
-00003c90: 6f72 2064 6f63 7465 7374 7320 696e 2066  or doctests in f
-00003ca0: 696c 6573 2077 6974 6820 7468 6973 2065  iles with this e
-00003cb0: 7874 656e 7369 6f6e 0a20 2020 5b4e 4f53  xtension.   [NOS
-00003cc0: 455f 444f 4354 4553 545f 4558 5445 4e53  E_DOCTEST_EXTENS
-00003cd0: 494f 4e5d 0a0a 2d2d 646f 6374 6573 742d  ION]..--doctest-
-00003ce0: 7265 7375 6c74 2d76 6172 6961 626c 653d  result-variable=
-00003cf0: 5641 520a 0a20 2020 4368 616e 6765 2074  VAR..   Change t
-00003d00: 6865 2076 6172 6961 626c 6520 6e61 6d65  he variable name
-00003d10: 2073 6574 2074 6f20 7468 6520 7265 7375   set to the resu
-00003d20: 6c74 206f 6620 7468 6520 6c61 7374 2069  lt of the last i
-00003d30: 6e74 6572 7072 6574 6572 0a20 2020 636f  nterpreter.   co
-00003d40: 6d6d 616e 6420 6672 6f6d 2074 6865 2064  mmand from the d
-00003d50: 6566 6175 6c74 2027 5f27 2e20 4361 6e20  efault '_'. Can 
-00003d60: 6265 2075 7365 6420 746f 2061 766f 6964  be used to avoid
-00003d70: 2063 6f6e 666c 6963 7473 2077 6974 680a   conflicts with.
-00003d80: 2020 2074 6865 205f 2829 2066 756e 6374     the _() funct
-00003d90: 696f 6e20 7573 6564 2066 6f72 2074 6578  ion used for tex
-00003da0: 7420 7472 616e 736c 6174 696f 6e2e 0a20  t translation.. 
-00003db0: 2020 5b4e 4f53 455f 444f 4354 4553 545f    [NOSE_DOCTEST_
-00003dc0: 5245 5355 4c54 5f56 4152 5d0a 0a2d 2d64  RESULT_VAR]..--d
-00003dd0: 6f63 7465 7374 2d66 6978 7475 7265 733d  octest-fixtures=
-00003de0: 5355 4646 4958 0a0a 2020 2046 696e 6420  SUFFIX..   Find 
-00003df0: 6669 7874 7572 6573 2066 6f72 2061 2064  fixtures for a d
-00003e00: 6f63 7465 7374 2066 696c 6520 696e 206d  octest file in m
-00003e10: 6f64 756c 6520 7769 7468 2074 6869 7320  odule with this 
-00003e20: 6e61 6d65 2061 7070 656e 6465 640a 2020  name appended.  
-00003e30: 2074 6f20 7468 6520 6261 7365 206e 616d   to the base nam
-00003e40: 6520 6f66 2074 6865 2064 6f63 7465 7374  e of the doctest
-00003e50: 2066 696c 650a 0a2d 2d64 6f63 7465 7374   file..--doctest
-00003e60: 2d6f 7074 696f 6e73 3d4f 5054 494f 4e53  -options=OPTIONS
-00003e70: 0a0a 2020 2053 7065 6369 6679 206f 7074  ..   Specify opt
-00003e80: 696f 6e73 2074 6f20 7061 7373 2074 6f20  ions to pass to 
-00003e90: 646f 6374 6573 742e 2045 672e 0a20 2020  doctest. Eg..   
-00003ea0: 272b 454c 4c49 5053 4953 2c2b 4e4f 524d  '+ELLIPSIS,+NORM
-00003eb0: 414c 495a 455f 5748 4954 4553 5041 4345  ALIZE_WHITESPACE
-00003ec0: 270a 0a2d 2d77 6974 682d 6973 6f6c 6174  '..--with-isolat
-00003ed0: 696f 6e0a 0a20 2020 456e 6162 6c65 2070  ion..   Enable p
-00003ee0: 6c75 6769 6e20 4973 6f6c 6174 696f 6e50  lugin IsolationP
-00003ef0: 6c75 6769 6e3a 2041 6374 6976 6174 6520  lugin: Activate 
-00003f00: 7468 6520 6973 6f6c 6174 696f 6e20 706c  the isolation pl
-00003f10: 7567 696e 2074 6f0a 2020 2069 736f 6c61  ugin to.   isola
-00003f20: 7465 2063 6861 6e67 6573 2074 6f20 6578  te changes to ex
-00003f30: 7465 726e 616c 206d 6f64 756c 6573 2074  ternal modules t
-00003f40: 6f20 6120 7369 6e67 6c65 2074 6573 7420  o a single test 
-00003f50: 6d6f 6475 6c65 206f 720a 2020 2070 6163  module or.   pac
-00003f60: 6b61 6765 2e20 5468 6520 6973 6f6c 6174  kage. The isolat
-00003f70: 696f 6e20 706c 7567 696e 2072 6573 6574  ion plugin reset
-00003f80: 7320 7468 6520 636f 6e74 656e 7473 206f  s the contents o
-00003f90: 6620 7379 732e 6d6f 6475 6c65 730a 2020  f sys.modules.  
-00003fa0: 2061 6674 6572 2065 6163 6820 7465 7374   after each test
-00003fb0: 206d 6f64 756c 6520 6f72 2070 6163 6b61   module or packa
-00003fc0: 6765 2072 756e 7320 746f 2069 7473 2073  ge runs to its s
-00003fd0: 7461 7465 2062 6566 6f72 6520 7468 650a  tate before the.
-00003fe0: 2020 2074 6573 742e 2050 4c45 4153 4520     test. PLEASE 
-00003ff0: 4e4f 5445 2074 6861 7420 7468 6973 2070  NOTE that this p
-00004000: 6c75 6769 6e20 7368 6f75 6c64 206e 6f74  lugin should not
-00004010: 2062 6520 7573 6564 2077 6974 6820 7468   be used with th
-00004020: 650a 2020 2063 6f76 6572 6167 6520 706c  e.   coverage pl
-00004030: 7567 696e 2c20 6f72 2069 6e20 616e 7920  ugin, or in any 
-00004040: 6f74 6865 7220 6361 7365 2077 6865 7265  other case where
-00004050: 206d 6f64 756c 6520 7265 6c6f 6164 696e   module reloadin
-00004060: 6720 6d61 790a 2020 2070 726f 6475 6365  g may.   produce
-00004070: 2075 6e64 6573 6972 6162 6c65 2073 6964   undesirable sid
-00004080: 652d 6566 6665 6374 732e 205b 4e4f 5345  e-effects. [NOSE
-00004090: 5f57 4954 485f 4953 4f4c 4154 494f 4e5d  _WITH_ISOLATION]
-000040a0: 0a0a 2d64 2c20 2d2d 6465 7461 696c 6564  ..-d, --detailed
-000040b0: 2d65 7272 6f72 732c 202d 2d66 6169 6c75  -errors, --failu
-000040c0: 7265 2d64 6574 6169 6c0a 0a20 2020 4164  re-detail..   Ad
-000040d0: 6420 6465 7461 696c 2074 6f20 6572 726f  d detail to erro
-000040e0: 7220 6f75 7470 7574 2062 7920 6174 7465  r output by atte
-000040f0: 6d70 7469 6e67 2074 6f20 6576 616c 7561  mpting to evalua
-00004100: 7465 2066 6169 6c65 6420 6173 7365 7274  te failed assert
-00004110: 730a 2020 205b 4e4f 5345 5f44 4554 4149  s.   [NOSE_DETAI
-00004120: 4c45 445f 4552 524f 5253 5d0a 0a2d 2d6e  LED_ERRORS]..--n
-00004130: 6f2d 736b 6970 0a0a 2020 2044 6973 6162  o-skip..   Disab
-00004140: 6c65 2073 7065 6369 616c 2068 616e 646c  le special handl
-00004150: 696e 6720 6f66 2053 6b69 7054 6573 7420  ing of SkipTest 
-00004160: 6578 6365 7074 696f 6e73 2e0a 0a2d 2d77  exceptions...--w
-00004170: 6974 682d 6964 0a0a 2020 2045 6e61 626c  ith-id..   Enabl
-00004180: 6520 706c 7567 696e 2054 6573 7449 643a  e plugin TestId:
-00004190: 2041 6374 6976 6174 6520 746f 2061 6464   Activate to add
-000041a0: 2061 2074 6573 7420 6964 2028 6c69 6b65   a test id (like
-000041b0: 2023 3129 2074 6f20 6561 6368 0a20 2020   #1) to each.   
-000041c0: 7465 7374 206e 616d 6520 6f75 7470 7574  test name output
-000041d0: 2e20 4163 7469 7661 7465 2077 6974 6820  . Activate with 
-000041e0: 2d2d 6661 696c 6564 2074 6f20 7265 7275  --failed to reru
-000041f0: 6e20 6661 696c 696e 6720 7465 7374 730a  n failing tests.
-00004200: 2020 206f 6e6c 792e 205b 4e4f 5345 5f57     only. [NOSE_W
-00004210: 4954 485f 4944 5d0a 0a2d 2d69 642d 6669  ITH_ID]..--id-fi
-00004220: 6c65 3d46 494c 450a 0a20 2020 5374 6f72  le=FILE..   Stor
-00004230: 6520 7465 7374 2069 6473 2066 6f75 6e64  e test ids found
-00004240: 2069 6e20 7465 7374 2072 756e 7320 696e   in test runs in
-00004250: 2074 6869 7320 6669 6c65 2e20 4465 6661   this file. Defa
-00004260: 756c 7420 6973 2074 6865 2066 696c 650a  ult is the file.
-00004270: 2020 202e 6e6f 7365 6964 7320 696e 2074     .noseids in t
-00004280: 6865 2077 6f72 6b69 6e67 2064 6972 6563  he working direc
-00004290: 746f 7279 2e0a 0a2d 2d66 6169 6c65 640a  tory...--failed.
-000042a0: 0a20 2020 5275 6e20 7468 6520 7465 7374  .   Run the test
-000042b0: 7320 7468 6174 2066 6169 6c65 6420 696e  s that failed in
-000042c0: 2074 6865 206c 6173 7420 7465 7374 2072   the last test r
-000042d0: 756e 2e0a 0a2d 2d70 726f 6365 7373 6573  un...--processes
-000042e0: 3d4e 554d 0a0a 2020 2053 7072 6561 6420  =NUM..   Spread 
-000042f0: 7465 7374 2072 756e 2061 6d6f 6e67 2074  test run among t
-00004300: 6869 7320 6d61 6e79 2070 726f 6365 7373  his many process
-00004310: 6573 2e20 5365 7420 6120 6e75 6d62 6572  es. Set a number
-00004320: 2065 7175 616c 2074 6f0a 2020 2074 6865   equal to.   the
-00004330: 206e 756d 6265 7220 6f66 2070 726f 6365   number of proce
-00004340: 7373 6f72 7320 6f72 2063 6f72 6573 2069  ssors or cores i
-00004350: 6e20 796f 7572 206d 6163 6869 6e65 2066  n your machine f
-00004360: 6f72 2062 6573 7420 7265 7375 6c74 732e  or best results.
-00004370: 0a20 2020 5061 7373 2061 206e 6567 6174  .   Pass a negat
-00004380: 6976 6520 6e75 6d62 6572 2074 6f20 6861  ive number to ha
-00004390: 7665 2074 6865 206e 756d 6265 7220 6f66  ve the number of
-000043a0: 2070 726f 6365 7373 6573 0a20 2020 6175   processes.   au
-000043b0: 746f 6d61 7469 6361 6c6c 7920 7365 7420  tomatically set 
-000043c0: 746f 2074 6865 206e 756d 6265 7220 6f66  to the number of
-000043d0: 2063 6f72 6573 2e20 5061 7373 696e 6720   cores. Passing 
-000043e0: 3020 6d65 616e 7320 746f 0a20 2020 6469  0 means to.   di
-000043f0: 7361 626c 6520 7061 7261 6c6c 656c 2074  sable parallel t
-00004400: 6573 7469 6e67 2e20 4465 6661 756c 7420  esting. Default 
-00004410: 6973 2030 2075 6e6c 6573 7320 4e4f 5345  is 0 unless NOSE
-00004420: 5f50 524f 4345 5353 4553 2069 730a 2020  _PROCESSES is.  
-00004430: 2073 6574 2e20 5b4e 4f53 455f 5052 4f43   set. [NOSE_PROC
-00004440: 4553 5345 535d 0a0a 2d2d 7072 6f63 6573  ESSES]..--proces
-00004450: 732d 7469 6d65 6f75 743d 5345 434f 4e44  s-timeout=SECOND
-00004460: 530a 0a20 2020 5365 7420 7469 6d65 6f75  S..   Set timeou
-00004470: 7420 666f 7220 7265 7475 726e 206f 6620  t for return of 
-00004480: 7265 7375 6c74 7320 6672 6f6d 2065 6163  results from eac
-00004490: 6820 7465 7374 2072 756e 6e65 7220 7072  h test runner pr
-000044a0: 6f63 6573 732e 0a20 2020 4465 6661 756c  ocess..   Defaul
-000044b0: 7420 6973 2031 302e 205b 4e4f 5345 5f50  t is 10. [NOSE_P
-000044c0: 524f 4345 5353 5f54 494d 454f 5554 5d0a  ROCESS_TIMEOUT].
-000044d0: 0a2d 2d70 726f 6365 7373 2d72 6573 7461  .--process-resta
-000044e0: 7274 776f 726b 6572 0a0a 2020 2049 6620  rtworker..   If 
-000044f0: 7365 742c 2077 696c 6c20 7265 7374 6172  set, will restar
-00004500: 7420 6561 6368 2077 6f72 6b65 7220 7072  t each worker pr
-00004510: 6f63 6573 7320 6f6e 6365 2074 6865 6972  ocess once their
-00004520: 2074 6573 7473 2061 7265 2064 6f6e 652c   tests are done,
-00004530: 0a20 2020 7468 6973 2068 656c 7073 2063  .   this helps c
-00004540: 6f6e 7472 6f6c 206d 656d 6f72 7920 6c65  ontrol memory le
-00004550: 616b 7320 6672 6f6d 206b 696c 6c69 6e67  aks from killing
-00004560: 2074 6865 2073 7973 7465 6d2e 0a20 2020   the system..   
-00004570: 5b4e 4f53 455f 5052 4f43 4553 535f 5245  [NOSE_PROCESS_RE
-00004580: 5354 4152 5457 4f52 4b45 525d 0a0a 2d2d  STARTWORKER]..--
-00004590: 7769 7468 2d78 756e 6974 0a0a 2020 2045  with-xunit..   E
-000045a0: 6e61 626c 6520 706c 7567 696e 2058 756e  nable plugin Xun
-000045b0: 6974 3a20 5468 6973 2070 6c75 6769 6e20  it: This plugin 
-000045c0: 7072 6f76 6964 6573 2074 6573 7420 7265  provides test re
-000045d0: 7375 6c74 7320 696e 2074 6865 0a20 2020  sults in the.   
-000045e0: 7374 616e 6461 7264 2058 556e 6974 2058  standard XUnit X
-000045f0: 4d4c 2066 6f72 6d61 742e 205b 4e4f 5345  ML format. [NOSE
-00004600: 5f57 4954 485f 5855 4e49 545d 0a0a 2d2d  _WITH_XUNIT]..--
-00004610: 7875 6e69 742d 6669 6c65 3d46 494c 450a  xunit-file=FILE.
-00004620: 0a20 2020 5061 7468 2074 6f20 786d 6c20  .   Path to xml 
-00004630: 6669 6c65 2074 6f20 7374 6f72 6520 7468  file to store th
-00004640: 6520 7875 6e69 7420 7265 706f 7274 2069  e xunit report i
-00004650: 6e2e 2044 6566 6175 6c74 2069 730a 2020  n. Default is.  
-00004660: 206e 6f73 6574 6573 7473 2e78 6d6c 2069   nosetests.xml i
-00004670: 6e20 7468 6520 776f 726b 696e 6720 6469  n the working di
-00004680: 7265 6374 6f72 7920 5b4e 4f53 455f 5855  rectory [NOSE_XU
-00004690: 4e49 545f 4649 4c45 5d0a 0a2d 2d78 756e  NIT_FILE]..--xun
-000046a0: 6974 2d74 6573 7473 7569 7465 2d6e 616d  it-testsuite-nam
-000046b0: 653d 5041 434b 4147 450a 0a20 2020 4e61  e=PACKAGE..   Na
-000046c0: 6d65 206f 6620 7468 6520 7465 7374 7375  me of the testsu
-000046d0: 6974 6520 696e 2074 6865 2078 756e 6974  ite in the xunit
-000046e0: 2078 6d6c 2c20 6765 6e65 7261 7465 6420   xml, generated 
-000046f0: 6279 2070 6c75 6769 6e2e 0a20 2020 4465  by plugin..   De
-00004700: 6661 756c 7420 7465 7374 2073 7569 7465  fault test suite
-00004710: 206e 616d 6520 6973 206e 6f73 6574 6573   name is nosetes
-00004720: 7473 2e0a 0a2d 2d61 6c6c 2d6d 6f64 756c  ts...--all-modul
-00004730: 6573 0a0a 2020 2045 6e61 626c 6520 706c  es..   Enable pl
-00004740: 7567 696e 2041 6c6c 4d6f 6475 6c65 733a  ugin AllModules:
-00004750: 2043 6f6c 6c65 6374 2074 6573 7473 2066   Collect tests f
-00004760: 726f 6d20 616c 6c20 7079 7468 6f6e 206d  rom all python m
-00004770: 6f64 756c 6573 2e0a 2020 205b 4e4f 5345  odules..   [NOSE
-00004780: 5f41 4c4c 5f4d 4f44 554c 4553 5d0a 0a2d  _ALL_MODULES]..-
-00004790: 2d63 6f2c 202d 2d63 6f6c 6c65 6374 2d6f  -co, --collect-o
-000047a0: 6e6c 790a 0a20 2020 456e 6162 6c65 2063  nly..   Enable c
-000047b0: 6f6c 6c65 6374 2d6f 6e6c 793a 2043 6f6c  ollect-only: Col
-000047c0: 6c65 6374 2061 6e64 206f 7574 7075 7420  lect and output 
-000047d0: 7465 7374 206e 616d 6573 206f 6e6c 792c  test names only,
-000047e0: 0a20 2020 6275 7420 646f 206e 6f74 2072  .   but do not r
-000047f0: 756e 2061 6e79 2074 6573 7473 2e20 5b43  un any tests. [C
-00004800: 4f4c 4c45 4354 5f4f 4e4c 595d 0a60 6060  OLLECT_ONLY].```
-00004810: 0a                                       .
+000005b0: 0a3c 6831 3e70 796e 6f73 6520 f09f 908d  .<h1>pynose ....
+000005c0: f09f 9183 203c 6120 6872 6566 3d22 6874  .... <a href="ht
+000005d0: 7470 733a 2f2f 7079 7069 2e70 7974 686f  tps://pypi.pytho
+000005e0: 6e2e 6f72 672f 7079 7069 2f70 796e 6f73  n.org/pypi/pynos
+000005f0: 6522 2074 6172 6765 743d 225f 626c 616e  e" target="_blan
+00000600: 6b22 3e3c 696d 6720 7372 633d 2268 7474  k"><img src="htt
+00000610: 7073 3a2f 2f69 6d67 2e73 6869 656c 6473  ps://img.shields
+00000620: 2e69 6f2f 7079 7069 2f76 2f70 796e 6f73  .io/pypi/v/pynos
+00000630: 652e 7376 673f 636f 6c6f 723d 3333 3939  e.svg?color=3399
+00000640: 4545 2220 616c 743d 2250 7950 4920 7665  EE" alt="PyPI ve
+00000650: 7273 696f 6e22 202f 3e3c 2f61 3e3c 2f68  rsion" /></a></h
+00000660: 313e 0a0a 2323 2320 2a2a 5b70 796e 6f73  1>..### **[pynos
+00000670: 655d 2868 7474 7073 3a2f 2f67 6974 6875  e](https://githu
+00000680: 622e 636f 6d2f 6d64 6d69 6e74 7a2f 7079  b.com/mdmintz/py
+00000690: 6e6f 7365 292a 2a20 6669 7865 7320 2a2a  nose)** fixes **
+000006a0: 5b6e 6f73 655d 2868 7474 7073 3a2f 2f6e  [nose](https://n
+000006b0: 6f73 652e 7265 6164 7468 6564 6f63 732e  ose.readthedocs.
+000006c0: 696f 2f65 6e2f 6c61 7465 7374 2f29 2a2a  io/en/latest/)**
+000006d0: 2074 6f20 6578 7465 6e64 205b 756e 6974   to extend [unit
+000006e0: 7465 7374 5d28 6874 7470 733a 2f2f 646f  test](https://do
+000006f0: 6373 2e70 7974 686f 6e2e 6f72 672f 332f  cs.python.org/3/
+00000700: 6c69 6272 6172 792f 756e 6974 7465 7374  library/unittest
+00000710: 2e68 746d 6c29 2061 6e64 206d 616b 6520  .html) and make 
+00000720: 7465 7374 696e 6720 6561 7369 6572 2e0a  testing easier..
+00000730: 0a2d 2d2d 2d2d 2d2d 2d0a 0a60 6070 796e  .--------..``pyn
+00000740: 6f73 6560 6020 6973 2061 6e20 7570 6461  ose`` is an upda
+00000750: 7465 6420 7665 7273 696f 6e20 6f66 2060  ted version of `
+00000760: 606e 6f73 6560 602c 206f 7269 6769 6e61  `nose``, origina
+00000770: 6c6c 7920 6d61 6465 2062 7920 4a61 736f  lly made by Jaso
+00000780: 6e20 5065 6c6c 6572 696e 2e0a 0a54 6869  n Pellerin...Thi
+00000790: 7320 7665 7273 696f 6e20 6f66 2060 606e  s version of ``n
+000007a0: 6f73 6560 6020 6973 2063 6f6d 7061 7469  ose`` is compati
+000007b0: 626c 6520 7769 7468 2060 6050 7974 686f  ble with ``Pytho
+000007c0: 6e20 332e 362b 6060 2028 696e 636c 7564  n 3.6+`` (includ
+000007d0: 696e 6720 6060 332e 3132 2b60 6029 2e0a  ing ``3.12+``)..
+000007e0: 0a43 6861 6e67 6573 2069 6e20 6060 7079  .Changes in ``py
+000007f0: 6e6f 7365 6060 2066 726f 6d20 6c65 6761  nose`` from lega
+00000800: 6379 2060 606e 6f73 6560 6020 696e 636c  cy ``nose`` incl
+00000810: 7564 653a 0a2a 2046 6978 6573 2022 4174  ude:.* Fixes "At
+00000820: 7472 6962 7574 6545 7272 6f72 3a20 6d6f  tributeError: mo
+00000830: 6475 6c65 2027 636f 6c6c 6563 7469 6f6e  dule 'collection
+00000840: 7327 2068 6173 206e 6f20 6174 7472 6962  s' has no attrib
+00000850: 7574 6520 2743 616c 6c61 626c 6527 2e22  ute 'Callable'."
+00000860: 0a2a 2046 6978 6573 2022 4174 7472 6962  .* Fixes "Attrib
+00000870: 7574 6545 7272 6f72 3a20 6d6f 6475 6c65  uteError: module
+00000880: 2027 696e 7370 6563 7427 2068 6173 206e   'inspect' has n
+00000890: 6f20 6174 7472 6962 7574 6520 2767 6574  o attribute 'get
+000008a0: 6172 6773 7065 6327 2e22 0a2a 2046 6978  argspec'.".* Fix
+000008b0: 6573 2022 496d 706f 7274 4572 726f 723a  es "ImportError:
+000008c0: 2063 616e 6e6f 7420 696d 706f 7274 206e   cannot import n
+000008d0: 616d 6520 275f 5465 7874 5465 7374 5265  ame '_TextTestRe
+000008e0: 7375 6c74 2720 6672 6f6d 2027 756e 6974  sult' from 'unit
+000008f0: 7465 7374 272e 220a 2a20 4669 7865 7320  test'.".* Fixes 
+00000900: 2252 756e 7469 6d65 5761 726e 696e 673a  "RuntimeWarning:
+00000910: 2054 6573 7452 6573 756c 7420 6861 7320   TestResult has 
+00000920: 6e6f 2061 6464 4475 7261 7469 6f6e 206d  no addDuration m
+00000930: 6574 686f 642e 220a 2a20 4669 7865 7320  ethod.".* Fixes 
+00000940: 2244 6570 7265 6361 7469 6f6e 5761 726e  "DeprecationWarn
+00000950: 696e 673a 2070 6b67 5f72 6573 6f75 7263  ing: pkg_resourc
+00000960: 6573 2069 7320 6465 7072 6563 6174 6564  es is deprecated
+00000970: 2061 7320 616e 2041 5049 2e22 0a2a 2046   as an API.".* F
+00000980: 6978 6573 2061 6c6c 2060 6066 6c61 6b65  ixes all ``flake
+00000990: 3860 6020 6973 7375 6573 2066 726f 6d20  8`` issues from 
+000009a0: 7468 6520 6f72 6967 696e 616c 2060 606e  the original ``n
+000009b0: 6f73 6560 602e 0a2a 2052 6570 6c61 6365  ose``..* Replace
+000009c0: 7320 7468 6520 6060 696d 7060 6020 6d6f  s the ``imp`` mo
+000009d0: 6475 6c65 2077 6974 6820 7468 6520 6e65  dule with the ne
+000009e0: 7765 7220 6060 696d 706f 7274 6c69 6260  wer ``importlib`
+000009f0: 6020 6d6f 6475 6c65 2e0a 2a20 5468 6520  ` module..* The 
+00000a00: 6465 6661 756c 7420 6c6f 6767 696e 6720  default logging 
+00000a10: 6c65 7665 6c20 6e6f 7720 6869 6465 7320  level now hides 
+00000a20: 2264 6562 7567 2220 6c6f 6773 2066 6f72  "debug" logs for
+00000a30: 206c 6573 7320 6e6f 6973 652e 0a2a 2054   less noise..* T
+00000a40: 6865 2060 602d 7360 6020 6f70 7469 6f6e  he ``-s`` option
+00000a50: 2069 7320 616c 7761 7973 2061 6374 6976   is always activ
+00000a60: 6520 746f 2073 6565 2074 6865 206f 7574  e to see the out
+00000a70: 7075 7420 6f66 2060 6070 7269 6e74 2829  put of ``print()
+00000a80: 6060 2e0a 2a20 4164 6473 2060 602d 2d63  ``..* Adds ``--c
+00000a90: 6f60 6020 6173 2061 2073 686f 7274 6375  o`` as a shortcu
+00000aa0: 7420 746f 2075 7369 6e67 2060 602d 2d63  t to using ``--c
+00000ab0: 6f6c 6c65 6374 2d6f 6e6c 7960 602e 0a0a  ollect-only``...
+00000ac0: 2d2d 2d2d 2d2d 2d2d 0a0a 5468 6520 6f72  --------..The or
+00000ad0: 6967 696e 616c 2064 6573 6372 6970 7469  iginal descripti
+00000ae0: 6f6e 206f 6620 6060 6e6f 7365 6060 3a0a  on of ``nose``:.
+00000af0: 0a3e 6e6f 7365 2065 7874 656e 6473 2074  .>nose extends t
+00000b00: 6865 2074 6573 7420 6c6f 6164 696e 6720  he test loading 
+00000b10: 616e 6420 7275 6e6e 696e 6720 6665 6174  and running feat
+00000b20: 7572 6573 206f 6620 756e 6974 7465 7374  ures of unittest
+00000b30: 2c20 6d61 6b69 6e67 0a69 7420 6561 7369  , making.it easi
+00000b40: 6572 2074 6f20 7772 6974 652c 2066 696e  er to write, fin
+00000b50: 6420 616e 6420 7275 6e20 7465 7374 732e  d and run tests.
+00000b60: 0a0a 3e42 7920 6465 6661 756c 742c 206e  ..>By default, n
+00000b70: 6f73 6520 7275 6e73 2074 6573 7473 2069  ose runs tests i
+00000b80: 6e20 6669 6c65 7320 6f72 2064 6972 6563  n files or direc
+00000b90: 746f 7269 6573 2075 6e64 6572 2074 6865  tories under the
+00000ba0: 2063 7572 7265 6e74 0a77 6f72 6b69 6e67   current.working
+00000bb0: 2064 6972 6563 746f 7279 2077 686f 7365   directory whose
+00000bc0: 206e 616d 6573 2069 6e63 6c75 6465 2022   names include "
+00000bd0: 7465 7374 2220 6f72 2022 5465 7374 2220  test" or "Test" 
+00000be0: 6174 2061 2077 6f72 640a 626f 756e 6461  at a word.bounda
+00000bf0: 7279 2028 6c69 6b65 2022 7465 7374 5f74  ry (like "test_t
+00000c00: 6869 7322 206f 7220 2266 756e 6374 696f  his" or "functio
+00000c10: 6e61 6c5f 7465 7374 2220 6f72 2022 5465  nal_test" or "Te
+00000c20: 7374 436c 6173 7322 2062 7574 206e 6f74  stClass" but not
+00000c30: 0a22 6c69 6274 6573 7422 292e 2054 6573  ."libtest"). Tes
+00000c40: 7420 6f75 7470 7574 2069 7320 7369 6d69  t output is simi
+00000c50: 6c61 7220 746f 2074 6861 7420 6f66 2075  lar to that of u
+00000c60: 6e69 7474 6573 742c 2062 7574 2061 6c73  nittest, but als
+00000c70: 6f20 696e 636c 7564 6573 0a63 6170 7475  o includes.captu
+00000c80: 7265 6420 7374 646f 7574 206f 7574 7075  red stdout outpu
+00000c90: 7420 6672 6f6d 2066 6169 6c69 6e67 2074  t from failing t
+00000ca0: 6573 7473 2c20 666f 7220 6561 7379 2070  ests, for easy p
+00000cb0: 7269 6e74 2d73 7479 6c65 2064 6562 7567  rint-style debug
+00000cc0: 6769 6e67 2e0a 0a3e 5468 6573 6520 6665  ging...>These fe
+00000cd0: 6174 7572 6573 2c20 616e 6420 6d61 6e79  atures, and many
+00000ce0: 206d 6f72 652c 2061 7265 2063 7573 746f   more, are custo
+00000cf0: 6d69 7a61 626c 6520 7468 726f 7567 6820  mizable through 
+00000d00: 7468 6520 7573 6520 6f66 0a70 6c75 6769  the use of.plugi
+00000d10: 6e73 2e20 506c 7567 696e 7320 696e 636c  ns. Plugins incl
+00000d20: 7564 6564 2077 6974 6820 6e6f 7365 2070  uded with nose p
+00000d30: 726f 7669 6465 2073 7570 706f 7274 2066  rovide support f
+00000d40: 6f72 2064 6f63 7465 7374 2c20 636f 6465  or doctest, code
+00000d50: 0a63 6f76 6572 6167 6520 616e 6420 7072  .coverage and pr
+00000d60: 6f66 696c 696e 672c 2066 6c65 7869 626c  ofiling, flexibl
+00000d70: 6520 6174 7472 6962 7574 652d 6261 7365  e attribute-base
+00000d80: 6420 7465 7374 2073 656c 6563 7469 6f6e  d test selection
+00000d90: 2c0a 6f75 7470 7574 2063 6170 7475 7265  ,.output capture
+00000da0: 2061 6e64 206d 6f72 652e 204d 6f72 6520   and more. More 
+00000db0: 696e 666f 726d 6174 696f 6e20 6162 6f75  information abou
+00000dc0: 7420 7772 6974 696e 6720 706c 7567 696e  t writing plugin
+00000dd0: 730a 6d61 7920 6265 2066 6f75 6e64 206f  s.may be found o
+00000de0: 6e20 696e 2074 6865 206e 6f73 6520 4150  n in the nose AP
+00000df0: 4920 646f 6375 6d65 6e74 6174 696f 6e2c  I documentation,
+00000e00: 2068 6572 653a 0a68 7474 7073 3a2f 2f6e   here:.https://n
+00000e10: 6f73 652e 7265 6164 7468 6564 6f63 732e  ose.readthedocs.
+00000e20: 696f 2f65 6e2f 6c61 7465 7374 2f0a 0a2d  io/en/latest/..-
+00000e30: 2d2d 2d2d 2d2d 2d0a 0a60 6060 6261 7368  -------..```bash
+00000e40: 0a0a 4261 7369 6320 7573 6167 650a 2a2a  ..Basic usage.**
+00000e50: 2a2a 2a2a 2a2a 2a2a 2a0a 0a55 7365 2022  *********..Use "
+00000e60: 7079 6e6f 7365 2220 4f52 2022 6e6f 7365  pynose" OR "nose
+00000e70: 7465 7374 7322 2074 6f20 7275 6e20 7465  tests" to run te
+00000e80: 7374 733a 0a0a 2020 2020 7079 6e6f 7365  sts:..    pynose
+00000e90: 205b 6f70 7469 6f6e 735d 205b 286f 7074   [options] [(opt
+00000ea0: 696f 6e61 6c29 2074 6573 7420 6669 6c65  ional) test file
+00000eb0: 7320 6f72 2064 6972 6563 746f 7269 6573  s or directories
+00000ec0: 5d0a 0a20 2020 206e 6f73 6574 6573 7473  ]..    nosetests
+00000ed0: 205b 6f70 7469 6f6e 735d 205b 286f 7074   [options] [(opt
+00000ee0: 696f 6e61 6c29 2074 6573 7420 6669 6c65  ional) test file
+00000ef0: 7320 6f72 2064 6972 6563 746f 7269 6573  s or directories
+00000f00: 5d0a 0a49 6e20 6164 6469 7469 6f6e 2074  ]..In addition t
+00000f10: 6f20 7061 7373 696e 6720 636f 6d6d 616e  o passing comman
+00000f20: 642d 6c69 6e65 206f 7074 696f 6e73 2c20  d-line options, 
+00000f30: 796f 7520 6d61 7920 616c 736f 2070 7574  you may also put
+00000f40: 0a63 6f6e 6669 6775 7261 7469 6f6e 206f  .configuration o
+00000f50: 7074 696f 6e73 2069 6e20 6120 2e6e 6f73  ptions in a .nos
+00000f60: 6572 6320 6f72 206e 6f73 652e 6366 6720  erc or nose.cfg 
+00000f70: 6669 6c65 2069 6e20 796f 7572 2068 6f6d  file in your hom
+00000f80: 650a 6469 7265 6374 6f72 792e 2054 6865  e.directory. The
+00000f90: 7365 2061 7265 2073 7461 6e64 6172 6420  se are standard 
+00000fa0: 2e69 6e69 2d73 7479 6c65 2063 6f6e 6669  .ini-style confi
+00000fb0: 6720 6669 6c65 732e 2050 7574 2079 6f75  g files. Put you
+00000fc0: 720a 6e6f 7365 7465 7374 7320 636f 6e66  r.nosetests conf
+00000fd0: 6967 7572 6174 696f 6e20 696e 2061 205b  iguration in a [
+00000fe0: 6e6f 7365 7465 7374 735d 2073 6563 7469  nosetests] secti
+00000ff0: 6f6e 2c20 7769 7468 2074 6865 202d 2d20  on, with the -- 
+00001000: 7072 6566 6978 0a72 656d 6f76 6564 3a0a  prefix.removed:.
+00001010: 0a20 2020 5b6e 6f73 6574 6573 7473 5d0a  .   [nosetests].
+00001020: 2020 2076 6572 626f 7369 7479 3d33 0a20     verbosity=3. 
+00001030: 2020 7769 7468 2d64 6f63 7465 7374 3d31    with-doctest=1
+00001040: 0a0a 5468 6572 6520 6973 2061 6c73 6f20  ..There is also 
+00001050: 706f 7373 6962 6c69 7479 2074 6f20 6469  possiblity to di
+00001060: 7361 626c 6520 636f 6e66 6967 7572 6174  sable configurat
+00001070: 696f 6e20 6669 6c65 7320 6c6f 6164 696e  ion files loadin
+00001080: 6720 286d 6967 6874 0a62 6520 7573 6566  g (might.be usef
+00001090: 756c 2077 6865 6e20 7275 6e6e 6967 2069  ul when runnig i
+000010a0: 2e65 2e20 746f 7820 616e 6420 796f 7520  .e. tox and you 
+000010b0: 646f 206e 6f74 2077 616e 7420 796f 7572  do not want your
+000010c0: 2067 6c6f 6261 6c20 6e6f 7365 0a63 6f6e   global nose.con
+000010d0: 6669 6720 6669 6c65 2074 6f20 6265 2075  fig file to be u
+000010e0: 7365 6420 6279 2074 6f78 292e 2049 6e20  sed by tox). In 
+000010f0: 6f72 6465 7220 746f 2069 676e 6f72 6520  order to ignore 
+00001100: 7468 6f73 6520 636f 6e66 6967 7572 6174  those configurat
+00001110: 696f 6e0a 6669 6c65 7320 7369 6d70 6c79  ion.files simply
+00001120: 2073 6574 2061 6e20 656e 7669 726f 6e6d   set an environm
+00001130: 656e 7420 7661 7269 6162 6c65 2022 4e4f  ent variable "NO
+00001140: 5345 5f49 474e 4f52 455f 434f 4e46 4947  SE_IGNORE_CONFIG
+00001150: 5f46 494c 4553 222e 0a0a 5468 6572 6520  _FILES"...There 
+00001160: 6172 6520 7365 7665 7261 6c20 6f74 6865  are several othe
+00001170: 7220 7761 7973 2074 6f20 7573 6520 7468  r ways to use th
+00001180: 6520 6e6f 7365 2074 6573 7420 7275 6e6e  e nose test runn
+00001190: 6572 2062 6573 6964 6573 2074 6865 0a2a  er besides the.*
+000011a0: 6e6f 7365 7465 7374 732a 2073 6372 6970  nosetests* scrip
+000011b0: 742e 2059 6f75 206d 6179 2075 7365 206e  t. You may use n
+000011c0: 6f73 6520 696e 2061 2074 6573 7420 7363  ose in a test sc
+000011d0: 7269 7074 3a0a 0a20 2020 696d 706f 7274  ript:..   import
+000011e0: 206e 6f73 650a 2020 206e 6f73 652e 6d61   nose.   nose.ma
+000011f0: 696e 2829 0a0a 4966 2079 6f75 2064 6f20  in()..If you do 
+00001200: 6e6f 7420 7761 6e74 2074 6865 2074 6573  not want the tes
+00001210: 7420 7363 7269 7074 2074 6f20 6578 6974  t script to exit
+00001220: 2077 6974 6820 3020 6f6e 2073 7563 6365   with 0 on succe
+00001230: 7373 2061 6e64 2031 206f 6e0a 6661 696c  ss and 1 on.fail
+00001240: 7572 6520 286c 696b 6520 756e 6974 7465  ure (like unitte
+00001250: 7374 2e6d 6169 6e29 2c20 7573 6520 6e6f  st.main), use no
+00001260: 7365 2e72 756e 2829 2069 6e73 7465 6164  se.run() instead
+00001270: 3a0a 0a20 2020 696d 706f 7274 206e 6f73  :..   import nos
+00001280: 650a 2020 2072 6573 756c 7420 3d20 6e6f  e.   result = no
+00001290: 7365 2e72 756e 2829 0a0a 2a72 6573 756c  se.run()..*resul
+000012a0: 742a 2077 696c 6c20 6265 2074 7275 6520  t* will be true 
+000012b0: 6966 2074 6865 2074 6573 7420 7275 6e20  if the test run 
+000012c0: 7375 6363 6565 6465 642c 206f 7220 6661  succeeded, or fa
+000012d0: 6c73 6520 6966 2061 6e79 2074 6573 740a  lse if any test.
+000012e0: 6661 696c 6564 206f 7220 7261 6973 6564  failed or raised
+000012f0: 2061 6e20 756e 6361 7567 6874 2065 7863   an uncaught exc
+00001300: 6570 7469 6f6e 2e20 4c61 7374 6c79 2c20  eption. Lastly, 
+00001310: 796f 7520 6361 6e20 7275 6e20 6e6f 7365  you can run nose
+00001320: 2e63 6f72 650a 6469 7265 6374 6c79 2c20  .core.directly, 
+00001330: 7768 6963 6820 7769 6c6c 2072 756e 206e  which will run n
+00001340: 6f73 652e 6d61 696e 2829 3a0a 0a20 2020  ose.main():..   
+00001350: 7079 7468 6f6e 202f 7061 7468 2f74 6f2f  python /path/to/
+00001360: 6e6f 7365 2f63 6f72 652e 7079 0a0a 506c  nose/core.py..Pl
+00001370: 6561 7365 2073 6565 2074 6865 2075 7361  ease see the usa
+00001380: 6765 206d 6573 7361 6765 2066 6f72 2074  ge message for t
+00001390: 6865 206e 6f73 6574 6573 7473 2073 6372  he nosetests scr
+000013a0: 6970 7420 666f 7220 696e 666f 726d 6174  ipt for informat
+000013b0: 696f 6e0a 6162 6f75 7420 686f 7720 746f  ion.about how to
+000013c0: 2063 6f6e 7472 6f6c 2077 6869 6368 2074   control which t
+000013d0: 6573 7473 206e 6f73 6520 7275 6e73 2c20  ests nose runs, 
+000013e0: 7768 6963 6820 706c 7567 696e 7320 6172  which plugins ar
+000013f0: 6520 6c6f 6164 6564 2c0a 616e 6420 7468  e loaded,.and th
+00001400: 6520 7465 7374 206f 7574 7075 742e 0a0a  e test output...
+00001410: 0a45 7874 656e 6465 6420 7573 6167 650a  .Extended usage.
+00001420: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 0a0a  ==============..
+00001430: 6e6f 7365 2063 6f6c 6c65 6374 7320 7465  nose collects te
+00001440: 7374 7320 6175 746f 6d61 7469 6361 6c6c  sts automaticall
+00001450: 7920 6672 6f6d 2070 7974 686f 6e20 736f  y from python so
+00001460: 7572 6365 2066 696c 6573 2c0a 6469 7265  urce files,.dire
+00001470: 6374 6f72 6965 7320 616e 6420 7061 636b  ctories and pack
+00001480: 6167 6573 2066 6f75 6e64 2069 6e20 6974  ages found in it
+00001490: 7320 776f 726b 696e 6720 6469 7265 6374  s working direct
+000014a0: 6f72 7920 2877 6869 6368 0a64 6566 6175  ory (which.defau
+000014b0: 6c74 7320 746f 2074 6865 2063 7572 7265  lts to the curre
+000014c0: 6e74 2077 6f72 6b69 6e67 2064 6972 6563  nt working direc
+000014d0: 746f 7279 292e 2041 6e79 2070 7974 686f  tory). Any pytho
+000014e0: 6e20 736f 7572 6365 2066 696c 652c 0a64  n source file,.d
+000014f0: 6972 6563 746f 7279 206f 7220 7061 636b  irectory or pack
+00001500: 6167 6520 7468 6174 206d 6174 6368 6573  age that matches
+00001510: 2074 6865 2074 6573 744d 6174 6368 2072   the testMatch r
+00001520: 6567 756c 6172 2065 7870 7265 7373 696f  egular expressio
+00001530: 6e20 2862 790a 6465 6661 756c 743a 202a  n (by.default: *
+00001540: 283f 3a5e 7c5b 625f 2e2d 5d29 5b54 745d  (?:^|[b_.-])[Tt]
+00001550: 6573 7429 2a20 7769 6c6c 2062 6520 636f  est)* will be co
+00001560: 6c6c 6563 7465 6420 6173 2061 2074 6573  llected as a tes
+00001570: 7420 286f 7220 736f 7572 6365 0a66 6f72  t (or source.for
+00001580: 2063 6f6c 6c65 6374 696f 6e20 6f66 2074   collection of t
+00001590: 6573 7473 292e 2049 6e20 6164 6469 7469  ests). In additi
+000015a0: 6f6e 2c20 616c 6c20 6f74 6865 7220 7061  on, all other pa
+000015b0: 636b 6167 6573 2066 6f75 6e64 2069 6e20  ckages found in 
+000015c0: 7468 650a 776f 726b 696e 6720 6469 7265  the.working dire
+000015d0: 6374 6f72 7920 7769 6c6c 2062 6520 6578  ctory will be ex
+000015e0: 616d 696e 6564 2066 6f72 2070 7974 686f  amined for pytho
+000015f0: 6e20 736f 7572 6365 2066 696c 6573 206f  n source files o
+00001600: 720a 6469 7265 6374 6f72 6965 7320 7468  r.directories th
+00001610: 6174 206d 6174 6368 2074 6573 744d 6174  at match testMat
+00001620: 6368 2e20 5061 636b 6167 6520 6469 7363  ch. Package disc
+00001630: 6f76 6572 7920 6465 7363 656e 6473 2061  overy descends a
+00001640: 6c6c 2074 6865 0a77 6179 2064 6f77 6e20  ll the.way down 
+00001650: 7468 6520 7472 6565 2c20 736f 2070 6163  the tree, so pac
+00001660: 6b61 6765 2e74 6573 7473 2061 6e64 2070  kage.tests and p
+00001670: 6163 6b61 6765 2e73 7562 2e74 6573 7473  ackage.sub.tests
+00001680: 2061 6e64 0a70 6163 6b61 6765 2e73 7562   and.package.sub
+00001690: 2e73 7562 322e 7465 7374 7320 7769 6c6c  .sub2.tests will
+000016a0: 2061 6c6c 2062 6520 636f 6c6c 6563 7465   all be collecte
+000016b0: 642e 0a0a 5769 7468 696e 2061 2074 6573  d...Within a tes
+000016c0: 7420 6469 7265 6374 6f72 7920 6f72 2070  t directory or p
+000016d0: 6163 6b61 6765 2c20 616e 7920 7079 7468  ackage, any pyth
+000016e0: 6f6e 2073 6f75 7263 6520 6669 6c65 206d  on source file m
+000016f0: 6174 6368 696e 670a 7465 7374 4d61 7463  atching.testMatc
+00001700: 6820 7769 6c6c 2062 6520 6578 616d 696e  h will be examin
+00001710: 6564 2066 6f72 2074 6573 7420 6361 7365  ed for test case
+00001720: 732e 2057 6974 6869 6e20 6120 7465 7374  s. Within a test
+00001730: 206d 6f64 756c 652c 0a66 756e 6374 696f   module,.functio
+00001740: 6e73 2061 6e64 2063 6c61 7373 6573 2077  ns and classes w
+00001750: 686f 7365 206e 616d 6573 206d 6174 6368  hose names match
+00001760: 2074 6573 744d 6174 6368 2061 6e64 2054   testMatch and T
+00001770: 6573 7443 6173 650a 7375 6263 6c61 7373  estCase.subclass
+00001780: 6573 2077 6974 6820 616e 7920 6e61 6d65  es with any name
+00001790: 2077 696c 6c20 6265 206c 6f61 6465 6420   will be loaded 
+000017a0: 616e 6420 6578 6563 7574 6564 2061 7320  and executed as 
+000017b0: 7465 7374 732e 2054 6573 7473 0a6d 6179  tests. Tests.may
+000017c0: 2075 7365 2074 6865 2061 7373 6572 7420   use the assert 
+000017d0: 6b65 7977 6f72 6420 6f72 2072 6169 7365  keyword or raise
+000017e0: 2041 7373 6572 7469 6f6e 4572 726f 7273   AssertionErrors
+000017f0: 2074 6f20 696e 6469 6361 7465 2074 6573   to indicate tes
+00001800: 740a 6661 696c 7572 652e 2054 6573 7443  t.failure. TestC
+00001810: 6173 6520 7375 6263 6c61 7373 6573 206d  ase subclasses m
+00001820: 6179 2064 6f20 7468 6520 7361 6d65 206f  ay do the same o
+00001830: 7220 7573 6520 7468 6520 7661 7269 6f75  r use the variou
+00001840: 730a 5465 7374 4361 7365 206d 6574 686f  s.TestCase metho
+00001850: 6473 2061 7661 696c 6162 6c65 2e0a 0a2a  ds available...*
+00001860: 2a49 7420 6973 2069 6d70 6f72 7461 6e74  *It is important
+00001870: 2074 6f20 6e6f 7465 2074 6861 7420 7468   to note that th
+00001880: 6520 6465 6661 756c 7420 6265 6861 7669  e default behavi
+00001890: 6f72 206f 6620 6e6f 7365 2069 7320 746f  or of nose is to
+000018a0: 206e 6f74 0a69 6e63 6c75 6465 2074 6573   not.include tes
+000018b0: 7473 2066 726f 6d20 6669 6c65 7320 7768  ts from files wh
+000018c0: 6963 6820 6172 6520 6578 6563 7574 6162  ich are executab
+000018d0: 6c65 2e2a 2a20 2054 6f20 696e 636c 7564  le.**  To includ
+000018e0: 6520 7465 7374 730a 6672 6f6d 2073 7563  e tests.from suc
+000018f0: 6820 6669 6c65 732c 2072 656d 6f76 6520  h files, remove 
+00001900: 7468 6569 7220 6578 6563 7574 6162 6c65  their executable
+00001910: 2062 6974 206f 7220 7573 6520 7468 6520   bit or use the 
+00001920: 2d2d 6578 6520 666c 6167 0a28 7365 6520  --exe flag.(see 
+00001930: 274f 7074 696f 6e73 2720 7365 6374 696f  'Options' sectio
+00001940: 6e20 6265 6c6f 7729 2e0a 0a0a 5365 6c65  n below)....Sele
+00001950: 6374 696e 6720 5465 7374 730a 2d2d 2d2d  cting Tests.----
+00001960: 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a 0a54 6f20  -----------..To 
+00001970: 7370 6563 6966 7920 7768 6963 6820 7465  specify which te
+00001980: 7374 7320 746f 2072 756e 2c20 7061 7373  sts to run, pass
+00001990: 2074 6573 7420 6e61 6d65 7320 6f6e 2074   test names on t
+000019a0: 6865 2063 6f6d 6d61 6e64 206c 696e 653a  he command line:
+000019b0: 0a0a 2020 206e 6f73 6574 6573 7473 206f  ..   nosetests o
+000019c0: 6e6c 795f 7465 7374 5f74 6869 732e 7079  nly_test_this.py
+000019d0: 0a0a 5465 7374 206e 616d 6573 2073 7065  ..Test names spe
+000019e0: 6369 6669 6564 206d 6179 2062 6520 6669  cified may be fi
+000019f0: 6c65 206f 7220 6d6f 6475 6c65 206e 616d  le or module nam
+00001a00: 6573 2c20 616e 6420 6d61 7920 6f70 7469  es, and may opti
+00001a10: 6f6e 616c 6c79 0a69 6e64 6963 6174 6520  onally.indicate 
+00001a20: 7468 6520 7465 7374 2063 6173 6520 746f  the test case to
+00001a30: 2072 756e 2062 7920 7365 7061 7261 7469   run by separati
+00001a40: 6e67 2074 6865 206d 6f64 756c 6520 6f72  ng the module or
+00001a50: 2066 696c 6520 6e61 6d65 0a66 726f 6d20   file name.from 
+00001a60: 7468 6520 7465 7374 2063 6173 6520 6e61  the test case na
+00001a70: 6d65 2077 6974 6820 6120 636f 6c6f 6e2e  me with a colon.
+00001a80: 2046 696c 656e 616d 6573 206d 6179 2062   Filenames may b
+00001a90: 6520 7265 6c61 7469 7665 206f 720a 6162  e relative or.ab
+00001aa0: 736f 6c75 7465 2e20 4578 616d 706c 6573  solute. Examples
+00001ab0: 3a0a 0a20 2020 6e6f 7365 7465 7374 7320  :..   nosetests 
+00001ac0: 7465 7374 2e6d 6f64 756c 650a 2020 206e  test.module.   n
+00001ad0: 6f73 6574 6573 7473 2061 6e6f 7468 6572  osetests another
+00001ae0: 2e74 6573 743a 5465 7374 4361 7365 2e74  .test:TestCase.t
+00001af0: 6573 745f 6d65 7468 6f64 0a20 2020 6e6f  est_method.   no
+00001b00: 7365 7465 7374 7320 612e 7465 7374 3a54  setests a.test:T
+00001b10: 6573 7443 6173 650a 2020 206e 6f73 6574  estCase.   noset
+00001b20: 6573 7473 202f 7061 7468 2f74 6f2f 7465  ests /path/to/te
+00001b30: 7374 2f66 696c 652e 7079 3a74 6573 745f  st/file.py:test_
+00001b40: 6675 6e63 7469 6f6e 0a0a 596f 7520 6d61  function..You ma
+00001b50: 7920 616c 736f 2063 6861 6e67 6520 7468  y also change th
+00001b60: 6520 776f 726b 696e 6720 6469 7265 6374  e working direct
+00001b70: 6f72 7920 7768 6572 6520 6e6f 7365 206c  ory where nose l
+00001b80: 6f6f 6b73 2066 6f72 2074 6573 7473 0a62  ooks for tests.b
+00001b90: 7920 7573 696e 6720 7468 6520 2d77 2073  y using the -w s
+00001ba0: 7769 7463 683a 0a0a 2020 206e 6f73 6574  witch:..   noset
+00001bb0: 6573 7473 202d 7720 2f70 6174 682f 746f  ests -w /path/to
+00001bc0: 2f74 6573 7473 0a0a 4e6f 7465 2c20 686f  /tests..Note, ho
+00001bd0: 7765 7665 722c 2074 6861 7420 7375 7070  wever, that supp
+00001be0: 6f72 7420 666f 7220 6d75 6c74 6970 6c65  ort for multiple
+00001bf0: 202d 7720 6172 6775 6d65 6e74 7320 6973   -w arguments is
+00001c00: 206e 6f77 0a64 6570 7265 6361 7465 6420   now.deprecated 
+00001c10: 616e 6420 7769 6c6c 2062 6520 7265 6d6f  and will be remo
+00001c20: 7665 6420 696e 2061 2066 7574 7572 6520  ved in a future 
+00001c30: 7265 6c65 6173 652e 2041 7320 6f66 206e  release. As of n
+00001c40: 6f73 6520 302e 3130 2c0a 796f 7520 6361  ose 0.10,.you ca
+00001c50: 6e20 6765 7420 7468 6520 7361 6d65 2062  n get the same b
+00001c60: 6568 6176 696f 7220 6279 2073 7065 6369  ehavior by speci
+00001c70: 6679 696e 6720 7468 6520 7461 7267 6574  fying the target
+00001c80: 2064 6972 6563 746f 7269 6573 0a2a 7769   directories.*wi
+00001c90: 7468 6f75 742a 2074 6865 202d 7720 7377  thout* the -w sw
+00001ca0: 6974 6368 3a0a 0a20 2020 6e6f 7365 7465  itch:..   nosete
+00001cb0: 7374 7320 2f70 6174 682f 746f 2f74 6573  sts /path/to/tes
+00001cc0: 7473 202f 616e 6f74 6865 722f 7061 7468  ts /another/path
+00001cd0: 2f74 6f2f 7465 7374 730a 0a46 7572 7468  /to/tests..Furth
+00001ce0: 6572 2063 7573 746f 6d69 7a61 7469 6f6e  er customization
+00001cf0: 206f 6620 7465 7374 2073 656c 6563 7469   of test selecti
+00001d00: 6f6e 2061 6e64 206c 6f61 6469 6e67 2069  on and loading i
+00001d10: 7320 706f 7373 6962 6c65 0a74 6872 6f75  s possible.throu
+00001d20: 6768 2074 6865 2075 7365 206f 6620 706c  gh the use of pl
+00001d30: 7567 696e 732e 0a0a 5465 7374 2072 6573  ugins...Test res
+00001d40: 756c 7420 6f75 7470 7574 2069 7320 6964  ult output is id
+00001d50: 656e 7469 6361 6c20 746f 2074 6861 7420  entical to that 
+00001d60: 6f66 2075 6e69 7474 6573 742c 2065 7863  of unittest, exc
+00001d70: 6570 7420 666f 7220 7468 650a 6164 6469  ept for the.addi
+00001d80: 7469 6f6e 616c 2066 6561 7475 7265 7320  tional features 
+00001d90: 2865 7272 6f72 2063 6c61 7373 6573 2c20  (error classes, 
+00001da0: 616e 6420 706c 7567 696e 2d73 7570 706c  and plugin-suppl
+00001db0: 6965 6420 6665 6174 7572 6573 2073 7563  ied features suc
+00001dc0: 680a 6173 206f 7574 7075 7420 6361 7074  h.as output capt
+00001dd0: 7572 6520 616e 6420 6173 7365 7274 2069  ure and assert i
+00001de0: 6e74 726f 7370 6563 7469 6f6e 2920 6465  ntrospection) de
+00001df0: 7461 696c 6564 2069 6e20 7468 6520 6f70  tailed in the op
+00001e00: 7469 6f6e 730a 6265 6c6f 772e 0a0a 0a43  tions.below....C
+00001e10: 6f6e 6669 6775 7261 7469 6f6e 0a2d 2d2d  onfiguration.---
+00001e20: 2d2d 2d2d 2d2d 2d2d 2d2d 0a0a 496e 2061  ----------..In a
+00001e30: 6464 6974 696f 6e20 746f 2070 6173 7369  ddition to passi
+00001e40: 6e67 2063 6f6d 6d61 6e64 2d6c 696e 6520  ng command-line 
+00001e50: 6f70 7469 6f6e 732c 2079 6f75 206d 6179  options, you may
+00001e60: 2061 6c73 6f20 7075 740a 636f 6e66 6967   also put.config
+00001e70: 7572 6174 696f 6e20 6f70 7469 6f6e 7320  uration options 
+00001e80: 696e 2079 6f75 7220 7072 6f6a 6563 7420  in your project 
+00001e90: 2a73 6574 7570 2e63 6667 2a20 6669 6c65  *setup.cfg* file
+00001ea0: 2c20 6f72 2061 202e 6e6f 7365 7263 0a6f  , or a .noserc.o
+00001eb0: 7220 6e6f 7365 2e63 6667 2066 696c 6520  r nose.cfg file 
+00001ec0: 696e 2079 6f75 7220 686f 6d65 2064 6972  in your home dir
+00001ed0: 6563 746f 7279 2e20 496e 2061 6e79 206f  ectory. In any o
+00001ee0: 6620 7468 6573 6520 7374 616e 6461 7264  f these standard
+00001ef0: 2069 6e69 2d0a 7374 796c 6520 636f 6e66   ini-.style conf
+00001f00: 6967 2066 696c 6573 2c20 796f 7520 7075  ig files, you pu
+00001f10: 7420 796f 7572 206e 6f73 6574 6573 7473  t your nosetests
+00001f20: 2063 6f6e 6669 6775 7261 7469 6f6e 2069   configuration i
+00001f30: 6e20 610a 225b 6e6f 7365 7465 7374 735d  n a."[nosetests]
+00001f40: 2220 7365 6374 696f 6e2e 204f 7074 696f  " section. Optio
+00001f50: 6e73 2061 7265 2074 6865 2073 616d 6520  ns are the same 
+00001f60: 6173 206f 6e20 7468 6520 636f 6d6d 616e  as on the comman
+00001f70: 6420 6c69 6e65 2c0a 7769 7468 2074 6865  d line,.with the
+00001f80: 202d 2d20 7072 6566 6978 2072 656d 6f76   -- prefix remov
+00001f90: 6564 2e20 466f 7220 6f70 7469 6f6e 7320  ed. For options 
+00001fa0: 7468 6174 2061 7265 2073 696d 706c 6520  that are simple 
+00001fb0: 7377 6974 6368 6573 2c20 796f 750a 6d75  switches, you.mu
+00001fc0: 7374 2073 7570 706c 7920 6120 7661 6c75  st supply a valu
+00001fd0: 653a 0a0a 2020 205b 6e6f 7365 7465 7374  e:..   [nosetest
+00001fe0: 735d 0a20 2020 7665 7262 6f73 6974 793d  s].   verbosity=
+00001ff0: 330a 2020 2077 6974 682d 646f 6374 6573  3.   with-doctes
+00002000: 743d 310a 0a41 6c6c 2063 6f6e 6669 6775  t=1..All configu
+00002010: 7261 7469 6f6e 2066 696c 6573 2074 6861  ration files tha
+00002020: 7420 6172 6520 666f 756e 6420 7769 6c6c  t are found will
+00002030: 2062 6520 6c6f 6164 6564 2061 6e64 2074   be loaded and t
+00002040: 6865 6972 0a6f 7074 696f 6e73 2063 6f6d  heir.options com
+00002050: 6269 6e65 642e 2059 6f75 2063 616e 206f  bined. You can o
+00002060: 7665 7272 6964 6520 7468 6520 7374 616e  verride the stan
+00002070: 6461 7264 2063 6f6e 6669 6720 6669 6c65  dard config file
+00002080: 206c 6f61 6469 6e67 0a77 6974 6820 7468   loading.with th
+00002090: 6520 222d 6322 206f 7074 696f 6e2e 0a0a  e "-c" option...
+000020a0: 0a55 7369 6e67 2050 6c75 6769 6e73 0a2d  .Using Plugins.-
+000020b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0a0a 5468  ------------..Th
+000020c0: 6572 6520 6172 6520 6e75 6d65 726f 7573  ere are numerous
+000020d0: 206e 6f73 6520 706c 7567 696e 7320 6176   nose plugins av
+000020e0: 6169 6c61 626c 6520 7669 6120 6561 7379  ailable via easy
+000020f0: 5f69 6e73 7461 6c6c 2061 6e64 0a65 6c73  _install and.els
+00002100: 6577 6865 7265 2e20 546f 2075 7365 2061  ewhere. To use a
+00002110: 2070 6c75 6769 6e2c 206a 7573 7420 696e   plugin, just in
+00002120: 7374 616c 6c20 6974 2e20 5468 6520 706c  stall it. The pl
+00002130: 7567 696e 2077 696c 6c20 6164 640a 636f  ugin will add.co
+00002140: 6d6d 616e 6420 6c69 6e65 206f 7074 696f  mmand line optio
+00002150: 6e73 2074 6f20 6e6f 7365 7465 7374 732e  ns to nosetests.
+00002160: 2054 6f20 7665 7269 6679 2074 6861 7420   To verify that 
+00002170: 7468 6520 706c 7567 696e 2069 730a 696e  the plugin is.in
+00002180: 7374 616c 6c65 642c 2072 756e 3a0a 0a20  stalled, run:.. 
+00002190: 2020 6e6f 7365 7465 7374 7320 2d2d 706c    nosetests --pl
+000021a0: 7567 696e 730a 0a59 6f75 2063 616e 2061  ugins..You can a
+000021b0: 6464 202d 7620 6f72 202d 7676 2074 6f20  dd -v or -vv to 
+000021c0: 7468 6174 2063 6f6d 6d61 6e64 2074 6f20  that command to 
+000021d0: 7368 6f77 206d 6f72 6520 696e 666f 726d  show more inform
+000021e0: 6174 696f 6e20 6162 6f75 740a 6561 6368  ation about.each
+000021f0: 2070 6c75 6769 6e2e 0a0a 4966 2079 6f75   plugin...If you
+00002200: 2061 7265 2072 756e 6e69 6e67 206e 6f73   are running nos
+00002210: 652e 6d61 696e 2829 206f 7220 6e6f 7365  e.main() or nose
+00002220: 2e72 756e 2829 2066 726f 6d20 6120 7363  .run() from a sc
+00002230: 7269 7074 2c20 796f 7520 6361 6e0a 7370  ript, you can.sp
+00002240: 6563 6966 7920 6120 6c69 7374 206f 6620  ecify a list of 
+00002250: 706c 7567 696e 7320 746f 2075 7365 2062  plugins to use b
+00002260: 7920 7061 7373 696e 6720 6120 6c69 7374  y passing a list
+00002270: 206f 6620 706c 7567 696e 7320 7769 7468   of plugins with
+00002280: 2074 6865 0a70 6c75 6769 6e73 206b 6579   the.plugins key
+00002290: 776f 7264 2061 7267 756d 656e 742e 0a0a  word argument...
+000022a0: 0a4f 7074 696f 6e73 0a2d 2d2d 2d2d 2d2d  .Options.-------
+000022b0: 0a0a 2d56 2c20 2d2d 7665 7273 696f 6e0a  ..-V, --version.
+000022c0: 0a20 2020 4f75 7470 7574 206e 6f73 6520  .   Output nose 
+000022d0: 7665 7273 696f 6e20 616e 6420 6578 6974  version and exit
+000022e0: 0a0a 2d70 2c20 2d2d 706c 7567 696e 730a  ..-p, --plugins.
+000022f0: 0a20 2020 4f75 7470 7574 206c 6973 7420  .   Output list 
+00002300: 6f66 2061 7661 696c 6162 6c65 2070 6c75  of available plu
+00002310: 6769 6e73 2061 6e64 2065 7869 742e 2043  gins and exit. C
+00002320: 6f6d 6269 6e65 2077 6974 6820 6869 6768  ombine with high
+00002330: 6572 0a20 2020 7665 7262 6f73 6974 7920  er.   verbosity 
+00002340: 666f 7220 6772 6561 7465 7220 6465 7461  for greater deta
+00002350: 696c 0a0a 2d76 3d44 4546 4155 4c54 2c20  il..-v=DEFAULT, 
+00002360: 2d2d 7665 7262 6f73 653d 4445 4641 554c  --verbose=DEFAUL
+00002370: 540a 0a20 2020 4265 206d 6f72 6520 7665  T..   Be more ve
+00002380: 7262 6f73 652e 205b 4e4f 5345 5f56 4552  rbose. [NOSE_VER
+00002390: 424f 5345 5d0a 0a2d 2d76 6572 626f 7369  BOSE]..--verbosi
+000023a0: 7479 3d56 4552 424f 5349 5459 0a0a 2020  ty=VERBOSITY..  
+000023b0: 2053 6574 2076 6572 626f 7369 7479 3b20   Set verbosity; 
+000023c0: 2d2d 7665 7262 6f73 6974 793d 3220 6973  --verbosity=2 is
+000023d0: 2074 6865 2073 616d 6520 6173 202d 760a   the same as -v.
+000023e0: 0a2d 713d 4445 4641 554c 542c 202d 2d71  .-q=DEFAULT, --q
+000023f0: 7569 6574 3d44 4546 4155 4c54 0a0a 2020  uiet=DEFAULT..  
+00002400: 2042 6520 6c65 7373 2076 6572 626f 7365   Be less verbose
+00002410: 0a0a 2d63 3d46 494c 4553 2c20 2d2d 636f  ..-c=FILES, --co
+00002420: 6e66 6967 3d46 494c 4553 0a0a 2020 204c  nfig=FILES..   L
+00002430: 6f61 6420 636f 6e66 6967 7572 6174 696f  oad configuratio
+00002440: 6e20 6672 6f6d 2063 6f6e 6669 6720 6669  n from config fi
+00002450: 6c65 2873 292e 204d 6179 2062 6520 7370  le(s). May be sp
+00002460: 6563 6966 6965 6420 6d75 6c74 6970 6c65  ecified multiple
+00002470: 0a20 2020 7469 6d65 733b 2069 6e20 7468  .   times; in th
+00002480: 6174 2063 6173 652c 2061 6c6c 2063 6f6e  at case, all con
+00002490: 6669 6720 6669 6c65 7320 7769 6c6c 2062  fig files will b
+000024a0: 6520 6c6f 6164 6564 2061 6e64 2063 6f6d  e loaded and com
+000024b0: 6269 6e65 640a 0a2d 773d 5748 4552 452c  bined..-w=WHERE,
+000024c0: 202d 2d77 6865 7265 3d57 4845 5245 0a0a   --where=WHERE..
+000024d0: 2020 204c 6f6f 6b20 666f 7220 7465 7374     Look for test
+000024e0: 7320 696e 2074 6869 7320 6469 7265 6374  s in this direct
+000024f0: 6f72 792e 204d 6179 2062 6520 7370 6563  ory. May be spec
+00002500: 6966 6965 6420 6d75 6c74 6970 6c65 2074  ified multiple t
+00002510: 696d 6573 2e0a 2020 2054 6865 2066 6972  imes..   The fir
+00002520: 7374 2064 6972 6563 746f 7279 2070 6173  st directory pas
+00002530: 7365 6420 7769 6c6c 2062 6520 7573 6564  sed will be used
+00002540: 2061 7320 7468 6520 776f 726b 696e 6720   as the working 
+00002550: 6469 7265 6374 6f72 792c 0a20 2020 696e  directory,.   in
+00002560: 2070 6c61 6365 206f 6620 7468 6520 6375   place of the cu
+00002570: 7272 656e 7420 776f 726b 696e 6720 6469  rrent working di
+00002580: 7265 6374 6f72 792c 2077 6869 6368 2069  rectory, which i
+00002590: 7320 7468 6520 6465 6661 756c 742e 0a20  s the default.. 
+000025a0: 2020 4f74 6865 7273 2077 696c 6c20 6265    Others will be
+000025b0: 2061 6464 6564 2074 6f20 7468 6520 6c69   added to the li
+000025c0: 7374 206f 6620 7465 7374 7320 746f 2065  st of tests to e
+000025d0: 7865 6375 7465 2e20 5b4e 4f53 455f 5748  xecute. [NOSE_WH
+000025e0: 4552 455d 0a0a 2d2d 7079 3377 6865 7265  ERE]..--py3where
+000025f0: 3d50 5933 5748 4552 450a 0a20 2020 4c6f  =PY3WHERE..   Lo
+00002600: 6f6b 2066 6f72 2074 6573 7473 2069 6e20  ok for tests in 
+00002610: 7468 6973 2064 6972 6563 746f 7279 2075  this directory u
+00002620: 6e64 6572 2050 7974 686f 6e20 332e 782e  nder Python 3.x.
+00002630: 2046 756e 6374 696f 6e73 2074 6865 0a20   Functions the. 
+00002640: 2020 7361 6d65 2061 7320 2777 6865 7265    same as 'where
+00002650: 272c 2062 7574 206f 6e6c 7920 6170 706c  ', but only appl
+00002660: 6965 7320 6966 2072 756e 6e69 6e67 2075  ies if running u
+00002670: 6e64 6572 2050 7974 686f 6e20 332e 7820  nder Python 3.x 
+00002680: 6f72 0a20 2020 6162 6f76 652e 2020 4e6f  or.   above.  No
+00002690: 7465 2074 6861 742c 2069 6620 7072 6573  te that, if pres
+000026a0: 656e 7420 756e 6465 7220 332e 782c 2074  ent under 3.x, t
+000026b0: 6869 7320 6f70 7469 6f6e 2063 6f6d 706c  his option compl
+000026c0: 6574 656c 790a 2020 2072 6570 6c61 6365  etely.   replace
+000026d0: 7320 616e 7920 6469 7265 6374 6f72 6965  s any directorie
+000026e0: 7320 7370 6563 6966 6965 6420 7769 7468  s specified with
+000026f0: 2027 7768 6572 6527 2c20 736f 2074 6865   'where', so the
+00002700: 2027 7768 6572 6527 0a20 2020 6f70 7469   'where'.   opti
+00002710: 6f6e 2062 6563 6f6d 6573 2069 6e65 6666  on becomes ineff
+00002720: 6563 7469 7665 2e20 5b4e 4f53 455f 5059  ective. [NOSE_PY
+00002730: 3357 4845 5245 5d0a 0a2d 6d3d 5245 4745  3WHERE]..-m=REGE
+00002740: 582c 202d 2d6d 6174 6368 3d52 4547 4558  X, --match=REGEX
+00002750: 2c20 2d2d 7465 7374 6d61 7463 683d 5245  , --testmatch=RE
+00002760: 4745 580a 0a20 2020 4669 6c65 732c 2064  GEX..   Files, d
+00002770: 6972 6563 746f 7269 6573 2c20 6675 6e63  irectories, func
+00002780: 7469 6f6e 206e 616d 6573 2c20 616e 6420  tion names, and 
+00002790: 636c 6173 7320 6e61 6d65 7320 7468 6174  class names that
+000027a0: 206d 6174 6368 2074 6869 730a 2020 2072   match this.   r
+000027b0: 6567 756c 6172 2065 7870 7265 7373 696f  egular expressio
+000027c0: 6e20 6172 6520 636f 6e73 6964 6572 6564  n are considered
+000027d0: 2074 6573 7473 2e20 2044 6566 6175 6c74   tests.  Default
+000027e0: 3a0a 2020 2028 3f3a 5e7c 5b62 5f2e 2f2d  :.   (?:^|[b_./-
+000027f0: 5d29 5b54 745d 6573 7420 5b4e 4f53 455f  ])[Tt]est [NOSE_
+00002800: 5445 5354 4d41 5443 485d 0a0a 2d2d 7465  TESTMATCH]..--te
+00002810: 7374 733d 4e41 4d45 530a 0a20 2020 5275  sts=NAMES..   Ru
+00002820: 6e20 7468 6573 6520 7465 7374 7320 2863  n these tests (c
+00002830: 6f6d 6d61 2d73 6570 6172 6174 6564 206c  omma-separated l
+00002840: 6973 7429 2e20 5468 6973 2061 7267 756d  ist). This argum
+00002850: 656e 7420 6973 2075 7365 6675 6c0a 2020  ent is useful.  
+00002860: 206d 6169 6e6c 7920 6672 6f6d 2063 6f6e   mainly from con
+00002870: 6669 6775 7261 7469 6f6e 2066 696c 6573  figuration files
+00002880: 3b20 6f6e 2074 6865 2063 6f6d 6d61 6e64  ; on the command
+00002890: 206c 696e 652c 206a 7573 7420 7061 7373   line, just pass
+000028a0: 2074 6865 0a20 2020 7465 7374 7320 746f   the.   tests to
+000028b0: 2072 756e 2061 7320 6164 6469 7469 6f6e   run as addition
+000028c0: 616c 2061 7267 756d 656e 7473 2077 6974  al arguments wit
+000028d0: 6820 6e6f 2073 7769 7463 682e 0a0a 2d6c  h no switch...-l
+000028e0: 3d44 4546 4155 4c54 2c20 2d2d 6465 6275  =DEFAULT, --debu
+000028f0: 673d 4445 4641 554c 540a 0a20 2020 4163  g=DEFAULT..   Ac
+00002900: 7469 7661 7465 2064 6562 7567 206c 6f67  tivate debug log
+00002910: 6769 6e67 2066 6f72 206f 6e65 206f 7220  ging for one or 
+00002920: 6d6f 7265 2073 7973 7465 6d73 2e20 4176  more systems. Av
+00002930: 6169 6c61 626c 6520 6465 6275 670a 2020  ailable debug.  
+00002940: 206c 6f67 6765 7273 3a20 6e6f 7365 2c20   loggers: nose, 
+00002950: 6e6f 7365 2e69 6d70 6f72 7465 722c 206e  nose.importer, n
+00002960: 6f73 652e 696e 7370 6563 746f 722c 206e  ose.inspector, n
+00002970: 6f73 652e 706c 7567 696e 732c 0a20 2020  ose.plugins,.   
+00002980: 6e6f 7365 2e72 6573 756c 7420 616e 6420  nose.result and 
+00002990: 6e6f 7365 2e73 656c 6563 746f 722e 2053  nose.selector. S
+000029a0: 6570 6172 6174 6520 6d75 6c74 6970 6c65  eparate multiple
+000029b0: 206e 616d 6573 2077 6974 6820 610a 2020   names with a.  
+000029c0: 2063 6f6d 6d61 2e0a 0a2d 2d64 6562 7567   comma...--debug
+000029d0: 2d6c 6f67 3d46 494c 450a 0a20 2020 4c6f  -log=FILE..   Lo
+000029e0: 6720 6465 6275 6720 6d65 7373 6167 6573  g debug messages
+000029f0: 2074 6f20 7468 6973 2066 696c 6520 2864   to this file (d
+00002a00: 6566 6175 6c74 3a20 7379 732e 7374 6465  efault: sys.stde
+00002a10: 7272 290a 0a2d 2d6c 6f67 6769 6e67 2d63  rr)..--logging-c
+00002a20: 6f6e 6669 673d 4649 4c45 2c20 2d2d 6c6f  onfig=FILE, --lo
+00002a30: 672d 636f 6e66 6967 3d46 494c 450a 0a20  g-config=FILE.. 
+00002a40: 2020 4c6f 6164 206c 6f67 6769 6e67 2063    Load logging c
+00002a50: 6f6e 6669 6720 6672 6f6d 2074 6869 7320  onfig from this 
+00002a60: 6669 6c65 202d 2d20 6279 7061 7373 6573  file -- bypasses
+00002a70: 2061 6c6c 206f 7468 6572 206c 6f67 6769   all other loggi
+00002a80: 6e67 0a20 2020 636f 6e66 6967 2073 6574  ng.   config set
+00002a90: 7469 6e67 732e 0a0a 2d49 3d52 4547 4558  tings...-I=REGEX
+00002aa0: 2c20 2d2d 6967 6e6f 7265 2d66 696c 6573  , --ignore-files
+00002ab0: 3d52 4547 4558 0a0a 2020 2043 6f6d 706c  =REGEX..   Compl
+00002ac0: 6574 656c 7920 6967 6e6f 7265 2061 6e79  etely ignore any
+00002ad0: 2066 696c 6520 7468 6174 206d 6174 6368   file that match
+00002ae0: 6573 2074 6869 7320 7265 6775 6c61 7220  es this regular 
+00002af0: 6578 7072 6573 7369 6f6e 2e0a 2020 2054  expression..   T
+00002b00: 616b 6573 2070 7265 6365 6465 6e63 6520  akes precedence 
+00002b10: 6f76 6572 2061 6e79 206f 7468 6572 2073  over any other s
+00002b20: 6574 7469 6e67 7320 6f72 2070 6c75 6769  ettings or plugi
+00002b30: 6e73 2e20 5370 6563 6966 7969 6e67 0a20  ns. Specifying. 
+00002b40: 2020 7468 6973 206f 7074 696f 6e20 7769    this option wi
+00002b50: 6c6c 2072 6570 6c61 6365 2074 6865 2064  ll replace the d
+00002b60: 6566 6175 6c74 2073 6574 7469 6e67 2e20  efault setting. 
+00002b70: 5370 6563 6966 7920 7468 6973 206f 7074  Specify this opt
+00002b80: 696f 6e0a 2020 206d 756c 7469 706c 6520  ion.   multiple 
+00002b90: 7469 6d65 7320 746f 2061 6464 206d 6f72  times to add mor
+00002ba0: 6520 7265 6775 6c61 7220 6578 7072 6573  e regular expres
+00002bb0: 7369 6f6e 7320 5b4e 4f53 455f 4947 4e4f  sions [NOSE_IGNO
+00002bc0: 5245 5f46 494c 4553 5d0a 0a2d 653d 5245  RE_FILES]..-e=RE
+00002bd0: 4745 582c 202d 2d65 7863 6c75 6465 3d52  GEX, --exclude=R
+00002be0: 4547 4558 0a0a 2020 2044 6f20 6e6f 7420  EGEX..   Do not 
+00002bf0: 7275 6e20 7465 7374 7320 7468 6174 206d  run tests that m
+00002c00: 6174 6368 2072 6567 756c 6172 2065 7870  atch regular exp
+00002c10: 7265 7373 696f 6e20 5b4e 4f53 455f 4558  ression [NOSE_EX
+00002c20: 434c 5544 455d 0a0a 2d69 3d52 4547 4558  CLUDE]..-i=REGEX
+00002c30: 2c20 2d2d 696e 636c 7564 653d 5245 4745  , --include=REGE
+00002c40: 580a 0a20 2020 5468 6973 2072 6567 756c  X..   This regul
+00002c50: 6172 2065 7870 7265 7373 696f 6e20 7769  ar expression wi
+00002c60: 6c6c 2062 6520 6170 706c 6965 6420 746f  ll be applied to
+00002c70: 2066 696c 6573 2c20 6469 7265 6374 6f72   files, director
+00002c80: 6965 732c 0a20 2020 6675 6e63 7469 6f6e  ies,.   function
+00002c90: 206e 616d 6573 2c20 616e 6420 636c 6173   names, and clas
+00002ca0: 7320 6e61 6d65 7320 666f 7220 6120 6368  s names for a ch
+00002cb0: 616e 6365 2074 6f20 696e 636c 7564 6520  ance to include 
+00002cc0: 6164 6469 7469 6f6e 616c 0a20 2020 7465  additional.   te
+00002cd0: 7374 7320 7468 6174 2064 6f20 6e6f 7420  sts that do not 
+00002ce0: 6d61 7463 6820 5445 5354 4d41 5443 482e  match TESTMATCH.
+00002cf0: 2020 5370 6563 6966 7920 7468 6973 206f    Specify this o
+00002d00: 7074 696f 6e20 6d75 6c74 6970 6c65 0a20  ption multiple. 
+00002d10: 2020 7469 6d65 7320 746f 2061 6464 206d    times to add m
+00002d20: 6f72 6520 7265 6775 6c61 7220 6578 7072  ore regular expr
+00002d30: 6573 7369 6f6e 7320 5b4e 4f53 455f 494e  essions [NOSE_IN
+00002d40: 434c 5544 455d 0a0a 2d78 2c20 2d2d 7374  CLUDE]..-x, --st
+00002d50: 6f70 0a0a 2020 2053 746f 7020 7275 6e6e  op..   Stop runn
+00002d60: 696e 6720 7465 7374 7320 6166 7465 7220  ing tests after 
+00002d70: 7468 6520 6669 7273 7420 6572 726f 7220  the first error 
+00002d80: 6f72 2066 6169 6c75 7265 0a0a 2d50 2c20  or failure..-P, 
+00002d90: 2d2d 6e6f 2d70 6174 682d 6164 6a75 7374  --no-path-adjust
+00002da0: 6d65 6e74 0a0a 2020 2044 6f20 6e6f 7420  ment..   Do not 
+00002db0: 6d61 6b65 2061 6e79 2063 6861 6e67 6573  make any changes
+00002dc0: 2074 6f20 7379 732e 7061 7468 2077 6865   to sys.path whe
+00002dd0: 6e20 6c6f 6164 696e 6720 7465 7374 7320  n loading tests 
+00002de0: 5b4e 4f53 455f 4e4f 5041 5448 5d0a 0a2d  [NOSE_NOPATH]..-
+00002df0: 2d65 7865 0a0a 2020 204c 6f6f 6b20 666f  -exe..   Look fo
+00002e00: 7220 7465 7374 7320 696e 2070 7974 686f  r tests in pytho
+00002e10: 6e20 6d6f 6475 6c65 7320 7468 6174 2061  n modules that a
+00002e20: 7265 2065 7865 6375 7461 626c 652e 204e  re executable. N
+00002e30: 6f72 6d61 6c0a 2020 2062 6568 6176 696f  ormal.   behavio
+00002e40: 7220 6973 2074 6f20 6578 636c 7564 6520  r is to exclude 
+00002e50: 6578 6563 7574 6162 6c65 206d 6f64 756c  executable modul
+00002e60: 6573 2c20 7369 6e63 6520 7468 6579 206d  es, since they m
+00002e70: 6179 206e 6f74 2062 650a 2020 2069 6d70  ay not be.   imp
+00002e80: 6f72 742d 7361 6665 205b 4e4f 5345 5f49  ort-safe [NOSE_I
+00002e90: 4e43 4c55 4445 5f45 5845 5d0a 0a2d 2d6e  NCLUDE_EXE]..--n
+00002ea0: 6f65 7865 0a0a 2020 2044 4f20 4e4f 5420  oexe..   DO NOT 
+00002eb0: 6c6f 6f6b 2066 6f72 2074 6573 7473 2069  look for tests i
+00002ec0: 6e20 7079 7468 6f6e 206d 6f64 756c 6573  n python modules
+00002ed0: 2074 6861 7420 6172 6520 6578 6563 7574   that are execut
+00002ee0: 6162 6c65 2e20 2854 6865 0a20 2020 6465  able. (The.   de
+00002ef0: 6661 756c 7420 6f6e 2074 6865 2077 696e  fault on the win
+00002f00: 646f 7773 2070 6c61 7466 6f72 6d20 6973  dows platform is
+00002f10: 2074 6f20 646f 2073 6f2e 290a 0a2d 2d74   to do so.)..--t
+00002f20: 7261 7665 7273 652d 6e61 6d65 7370 6163  raverse-namespac
+00002f30: 650a 0a20 2020 5472 6176 6572 7365 2074  e..   Traverse t
+00002f40: 6872 6f75 6768 2061 6c6c 2070 6174 6820  hrough all path 
+00002f50: 656e 7472 6965 7320 6f66 2061 206e 616d  entries of a nam
+00002f60: 6573 7061 6365 2070 6163 6b61 6765 0a0a  espace package..
+00002f70: 2d2d 6669 7273 742d 7061 636b 6167 652d  --first-package-
+00002f80: 7769 6e73 2c20 2d2d 6669 7273 742d 706b  wins, --first-pk
+00002f90: 672d 7769 6e73 2c20 2d2d 3173 742d 706b  g-wins, --1st-pk
+00002fa0: 672d 7769 6e73 0a0a 2020 2054 6865 206e  g-wins..   The n
+00002fb0: 6f73 6520 696d 706f 7274 6572 2077 696c  ose importer wil
+00002fc0: 6c20 6e6f 726d 616c 6c79 2065 7669 6374  l normally evict
+00002fd0: 2061 2070 6163 6b61 6765 2066 726f 6d20   a package from 
+00002fe0: 7379 732e 6d6f 6475 6c65 7320 6966 0a20  sys.modules if. 
+00002ff0: 2020 6974 2073 6565 7320 6120 7061 636b    it sees a pack
+00003000: 6167 6520 7769 7468 2074 6865 2073 616d  age with the sam
+00003010: 6520 6e61 6d65 2069 6e20 6120 6469 6666  e name in a diff
+00003020: 6572 656e 7420 6c6f 6361 7469 6f6e 2e20  erent location. 
+00003030: 5365 740a 2020 2074 6869 7320 6f70 7469  Set.   this opti
+00003040: 6f6e 2074 6f20 6469 7361 626c 6520 7468  on to disable th
+00003050: 6174 2062 6568 6176 696f 722e 0a0a 2d2d  at behavior...--
+00003060: 6e6f 2d62 7974 652d 636f 6d70 696c 650a  no-byte-compile.
+00003070: 0a20 2020 5072 6576 656e 7420 6e6f 7365  .   Prevent nose
+00003080: 2066 726f 6d20 6279 7465 2d63 6f6d 7069   from byte-compi
+00003090: 6c69 6e67 2074 6865 2073 6f75 7263 6520  ling the source 
+000030a0: 696e 746f 202e 7079 6320 6669 6c65 7320  into .pyc files 
+000030b0: 7768 696c 650a 2020 206e 6f73 6520 6973  while.   nose is
+000030c0: 2073 6361 6e6e 696e 6720 666f 7220 616e   scanning for an
+000030d0: 6420 7275 6e6e 696e 6720 7465 7374 732e  d running tests.
+000030e0: 0a0a 2d61 3d41 5454 522c 202d 2d61 7474  ..-a=ATTR, --att
+000030f0: 723d 4154 5452 0a0a 2020 2052 756e 206f  r=ATTR..   Run o
+00003100: 6e6c 7920 7465 7374 7320 7468 6174 2068  nly tests that h
+00003110: 6176 6520 6174 7472 6962 7574 6573 2073  ave attributes s
+00003120: 7065 6369 6669 6564 2062 7920 4154 5452  pecified by ATTR
+00003130: 205b 4e4f 5345 5f41 5454 525d 0a0a 2d41   [NOSE_ATTR]..-A
+00003140: 3d45 5850 522c 202d 2d65 7661 6c2d 6174  =EXPR, --eval-at
+00003150: 7472 3d45 5850 520a 0a20 2020 5275 6e20  tr=EXPR..   Run 
+00003160: 6f6e 6c79 2074 6573 7473 2066 6f72 2077  only tests for w
+00003170: 686f 7365 2061 7474 7269 6275 7465 7320  hose attributes 
+00003180: 7468 6520 5079 7468 6f6e 2065 7870 7265  the Python expre
+00003190: 7373 696f 6e20 4558 5052 0a20 2020 6576  ssion EXPR.   ev
+000031a0: 616c 7561 7465 7320 746f 2054 7275 6520  aluates to True 
+000031b0: 5b4e 4f53 455f 4556 414c 5f41 5454 525d  [NOSE_EVAL_ATTR]
+000031c0: 0a0a 2d73 2c20 2d2d 6e6f 6361 7074 7572  ..-s, --nocaptur
+000031d0: 650a 0a20 2020 446f 206e 6f74 2063 6170  e..   Do not cap
+000031e0: 7475 7265 2073 7464 6f75 7420 2861 6e79  ture stdout (any
+000031f0: 2073 7464 6f75 7420 6f75 7470 7574 2077   stdout output w
+00003200: 696c 6c20 6265 2070 7269 6e74 6564 0a20  ill be printed. 
+00003210: 2020 696d 6d65 6469 6174 656c 7929 205b    immediately) [
+00003220: 4e4f 5345 5f4e 4f43 4150 5455 5245 5d0a  NOSE_NOCAPTURE].
+00003230: 0a2d 2d6e 6f6c 6f67 6361 7074 7572 650a  .--nologcapture.
+00003240: 0a20 2020 4469 7361 626c 6520 6c6f 6767  .   Disable logg
+00003250: 696e 6720 6361 7074 7572 6520 706c 7567  ing capture plug
+00003260: 696e 2e20 4c6f 6767 696e 6720 636f 6e66  in. Logging conf
+00003270: 6967 7572 6174 696f 6e20 7769 6c6c 2062  iguration will b
+00003280: 6520 6c65 6674 0a20 2020 696e 7461 6374  e left.   intact
+00003290: 2e20 5b4e 4f53 455f 4e4f 4c4f 4743 4150  . [NOSE_NOLOGCAP
+000032a0: 5455 5245 5d0a 0a2d 2d6c 6f67 6769 6e67  TURE]..--logging
+000032b0: 2d66 6f72 6d61 743d 464f 524d 4154 0a0a  -format=FORMAT..
+000032c0: 2020 2053 7065 6369 6679 2063 7573 746f     Specify custo
+000032d0: 6d20 666f 726d 6174 2074 6f20 7072 696e  m format to prin
+000032e0: 7420 7374 6174 656d 656e 7473 2e20 5573  t statements. Us
+000032f0: 6573 2074 6865 2073 616d 6520 666f 726d  es the same form
+00003300: 6174 2061 730a 2020 2075 7365 6420 6279  at as.   used by
+00003310: 2073 7461 6e64 6172 6420 6c6f 6767 696e   standard loggin
+00003320: 6720 6861 6e64 6c65 7273 2e20 5b4e 4f53  g handlers. [NOS
+00003330: 455f 4c4f 4746 4f52 4d41 545d 0a0a 2d2d  E_LOGFORMAT]..--
+00003340: 6c6f 6767 696e 672d 6461 7465 666d 743d  logging-datefmt=
+00003350: 464f 524d 4154 0a0a 2020 2053 7065 6369  FORMAT..   Speci
+00003360: 6679 2063 7573 746f 6d20 6461 7465 2f74  fy custom date/t
+00003370: 696d 6520 666f 726d 6174 2074 6f20 7072  ime format to pr
+00003380: 696e 7420 7374 6174 656d 656e 7473 2e20  int statements. 
+00003390: 5573 6573 2074 6865 2073 616d 650a 2020  Uses the same.  
+000033a0: 2066 6f72 6d61 7420 6173 2075 7365 6420   format as used 
+000033b0: 6279 2073 7461 6e64 6172 6420 6c6f 6767  by standard logg
+000033c0: 696e 6720 6861 6e64 6c65 7273 2e20 5b4e  ing handlers. [N
+000033d0: 4f53 455f 4c4f 4744 4154 4546 4d54 5d0a  OSE_LOGDATEFMT].
+000033e0: 0a2d 2d6c 6f67 6769 6e67 2d66 696c 7465  .--logging-filte
+000033f0: 723d 4649 4c54 4552 0a0a 2020 2053 7065  r=FILTER..   Spe
+00003400: 6369 6679 2077 6869 6368 2073 7461 7465  cify which state
+00003410: 6d65 6e74 7320 746f 2066 696c 7465 7220  ments to filter 
+00003420: 696e 2f6f 7574 2e20 4279 2064 6566 6175  in/out. By defau
+00003430: 6c74 2c20 6576 6572 7974 6869 6e67 0a20  lt, everything. 
+00003440: 2020 6973 2063 6170 7475 7265 642e 2049    is captured. I
+00003450: 6620 7468 6520 6f75 7470 7574 2069 7320  f the output is 
+00003460: 746f 6f20 7665 7262 6f73 652c 2075 7365  too verbose, use
+00003470: 2074 6869 7320 6f70 7469 6f6e 2074 6f0a   this option to.
+00003480: 2020 2066 696c 7465 7220 6f75 7420 6e65     filter out ne
+00003490: 6564 6c65 7373 206f 7574 7075 742e 2045  edless output. E
+000034a0: 7861 6d70 6c65 3a20 6669 6c74 6572 3d66  xample: filter=f
+000034b0: 6f6f 2077 696c 6c20 6361 7074 7572 650a  oo will capture.
+000034c0: 2020 2073 7461 7465 6d65 6e74 7320 6973     statements is
+000034d0: 7375 6564 204f 4e4c 5920 746f 2020 666f  sued ONLY to  fo
+000034e0: 6f20 6f72 2066 6f6f 2e77 6861 742e 6576  o or foo.what.ev
+000034f0: 6572 2e73 7562 2062 7574 206e 6f74 2066  er.sub but not f
+00003500: 6f6f 6261 720a 2020 206f 7220 6f74 6865  oobar.   or othe
+00003510: 7220 6c6f 6767 6572 2e20 5370 6563 6966  r logger. Specif
+00003520: 7920 6d75 6c74 6970 6c65 206c 6f67 6765  y multiple logge
+00003530: 7273 2077 6974 6820 636f 6d6d 613a 0a20  rs with comma:. 
+00003540: 2020 6669 6c74 6572 3d66 6f6f 2c62 6172    filter=foo,bar
+00003550: 2c62 617a 2e20 4966 2061 6e79 206c 6f67  ,baz. If any log
+00003560: 6765 7220 6e61 6d65 2069 7320 7072 6566  ger name is pref
+00003570: 6978 6564 2077 6974 6820 6120 6d69 6e75  ixed with a minu
+00003580: 732c 2065 670a 2020 2066 696c 7465 723d  s, eg.   filter=
+00003590: 2d66 6f6f 2c20 6974 2077 696c 6c20 6265  -foo, it will be
+000035a0: 2065 7863 6c75 6465 6420 7261 7468 6572   excluded rather
+000035b0: 2074 6861 6e20 696e 636c 7564 6564 2e20   than included. 
+000035c0: 4465 6661 756c 743a 0a20 2020 6578 636c  Default:.   excl
+000035d0: 7564 6520 6c6f 6767 696e 6720 6d65 7373  ude logging mess
+000035e0: 6167 6573 2066 726f 6d20 6e6f 7365 2069  ages from nose i
+000035f0: 7473 656c 6620 282d 6e6f 7365 292e 205b  tself (-nose). [
+00003600: 4e4f 5345 5f4c 4f47 4649 4c54 4552 5d0a  NOSE_LOGFILTER].
+00003610: 0a2d 2d6c 6f67 6769 6e67 2d63 6c65 6172  .--logging-clear
+00003620: 2d68 616e 646c 6572 730a 0a20 2020 436c  -handlers..   Cl
+00003630: 6561 7220 616c 6c20 6f74 6865 7220 6c6f  ear all other lo
+00003640: 6767 696e 6720 6861 6e64 6c65 7273 0a0a  gging handlers..
+00003650: 2d2d 6c6f 6767 696e 672d 6c65 7665 6c3d  --logging-level=
+00003660: 4445 4641 554c 540a 0a20 2020 5365 7420  DEFAULT..   Set 
+00003670: 7468 6520 6c6f 6720 6c65 7665 6c20 746f  the log level to
+00003680: 2063 6170 7475 7265 0a0a 2d2d 7769 7468   capture..--with
+00003690: 2d63 6f76 6572 6167 650a 0a20 2020 456e  -coverage..   En
+000036a0: 6162 6c65 2070 6c75 6769 6e20 436f 7665  able plugin Cove
+000036b0: 7261 6765 3a20 4163 7469 7661 7465 2061  rage: Activate a
+000036c0: 2063 6f76 6572 6167 6520 7265 706f 7274   coverage report
+000036d0: 2075 7369 6e67 2074 6865 0a20 2020 4e65   using the.   Ne
+000036e0: 6420 4261 7463 6865 6c64 6572 2063 6f76  d Batchelder cov
+000036f0: 6572 6167 6520 6d6f 6475 6c65 2e20 5b4e  erage module. [N
+00003700: 4f53 455f 5749 5448 5f43 4f56 4552 4147  OSE_WITH_COVERAG
+00003710: 455d 0a0a 2d2d 636f 7665 722d 7061 636b  E]..--cover-pack
+00003720: 6167 653d 5041 434b 4147 450a 0a20 2020  age=PACKAGE..   
+00003730: 5265 7374 7269 6374 2063 6f76 6572 6167  Restrict coverag
+00003740: 6520 6f75 7470 7574 2074 6f20 7365 6c65  e output to sele
+00003750: 6374 6564 2070 6163 6b61 6765 7320 5b4e  cted packages [N
+00003760: 4f53 455f 434f 5645 525f 5041 434b 4147  OSE_COVER_PACKAG
+00003770: 455d 0a0a 2d2d 636f 7665 722d 6572 6173  E]..--cover-eras
+00003780: 650a 0a20 2020 4572 6173 6520 7072 6576  e..   Erase prev
+00003790: 696f 7573 6c79 2063 6f6c 6c65 6374 6564  iously collected
+000037a0: 2063 6f76 6572 6167 6520 7374 6174 6973   coverage statis
+000037b0: 7469 6373 2062 6566 6f72 6520 7275 6e0a  tics before run.
+000037c0: 0a2d 2d63 6f76 6572 2d74 6573 7473 0a0a  .--cover-tests..
+000037d0: 2020 2049 6e63 6c75 6465 2074 6573 7420     Include test 
+000037e0: 6d6f 6475 6c65 7320 696e 2063 6f76 6572  modules in cover
+000037f0: 6167 6520 7265 706f 7274 205b 4e4f 5345  age report [NOSE
+00003800: 5f43 4f56 4552 5f54 4553 5453 5d0a 0a2d  _COVER_TESTS]..-
+00003810: 2d63 6f76 6572 2d6d 696e 2d70 6572 6365  -cover-min-perce
+00003820: 6e74 6167 653d 4445 4641 554c 540a 0a20  ntage=DEFAULT.. 
+00003830: 2020 4d69 6e69 6d75 6d20 7065 7263 656e    Minimum percen
+00003840: 7461 6765 206f 6620 636f 7665 7261 6765  tage of coverage
+00003850: 2066 6f72 2074 6573 7473 2074 6f20 7061   for tests to pa
+00003860: 7373 0a20 2020 5b4e 4f53 455f 434f 5645  ss.   [NOSE_COVE
+00003870: 525f 4d49 4e5f 5045 5243 454e 5441 4745  R_MIN_PERCENTAGE
+00003880: 5d0a 0a2d 2d63 6f76 6572 2d69 6e63 6c75  ]..--cover-inclu
+00003890: 7369 7665 0a0a 2020 2049 6e63 6c75 6465  sive..   Include
+000038a0: 2061 6c6c 2070 7974 686f 6e20 6669 6c65   all python file
+000038b0: 7320 756e 6465 7220 776f 726b 696e 6720  s under working 
+000038c0: 6469 7265 6374 6f72 7920 696e 2063 6f76  directory in cov
+000038d0: 6572 6167 650a 2020 2072 6570 6f72 742e  erage.   report.
+000038e0: 2020 5573 6566 756c 2066 6f72 2064 6973    Useful for dis
+000038f0: 636f 7665 7269 6e67 2068 6f6c 6573 2069  covering holes i
+00003900: 6e20 7465 7374 2063 6f76 6572 6167 6520  n test coverage 
+00003910: 6966 206e 6f74 2061 6c6c 0a20 2020 6669  if not all.   fi
+00003920: 6c65 7320 6172 6520 696d 706f 7274 6564  les are imported
+00003930: 2062 7920 7468 6520 7465 7374 2073 7569   by the test sui
+00003940: 7465 2e20 5b4e 4f53 455f 434f 5645 525f  te. [NOSE_COVER_
+00003950: 494e 434c 5553 4956 455d 0a0a 2d2d 636f  INCLUSIVE]..--co
+00003960: 7665 722d 6874 6d6c 0a0a 2020 2050 726f  ver-html..   Pro
+00003970: 6475 6365 2048 544d 4c20 636f 7665 7261  duce HTML covera
+00003980: 6765 2069 6e66 6f72 6d61 7469 6f6e 0a0a  ge information..
+00003990: 2d2d 636f 7665 722d 6874 6d6c 2d64 6972  --cover-html-dir
+000039a0: 3d44 4952 0a0a 2020 2050 726f 6475 6365  =DIR..   Produce
+000039b0: 2048 544d 4c20 636f 7665 7261 6765 2069   HTML coverage i
+000039c0: 6e66 6f72 6d61 7469 6f6e 2069 6e20 6469  nformation in di
+000039d0: 720a 0a2d 2d63 6f76 6572 2d62 7261 6e63  r..--cover-branc
+000039e0: 6865 730a 0a20 2020 496e 636c 7564 6520  hes..   Include 
+000039f0: 6272 616e 6368 2063 6f76 6572 6167 6520  branch coverage 
+00003a00: 696e 2063 6f76 6572 6167 6520 7265 706f  in coverage repo
+00003a10: 7274 205b 4e4f 5345 5f43 4f56 4552 5f42  rt [NOSE_COVER_B
+00003a20: 5241 4e43 4845 535d 0a0a 2d2d 636f 7665  RANCHES]..--cove
+00003a30: 722d 786d 6c0a 0a20 2020 5072 6f64 7563  r-xml..   Produc
+00003a40: 6520 584d 4c20 636f 7665 7261 6765 2069  e XML coverage i
+00003a50: 6e66 6f72 6d61 7469 6f6e 0a0a 2d2d 636f  nformation..--co
+00003a60: 7665 722d 786d 6c2d 6669 6c65 3d46 494c  ver-xml-file=FIL
+00003a70: 450a 0a20 2020 5072 6f64 7563 6520 584d  E..   Produce XM
+00003a80: 4c20 636f 7665 7261 6765 2069 6e66 6f72  L coverage infor
+00003a90: 6d61 7469 6f6e 2069 6e20 6669 6c65 0a0a  mation in file..
+00003aa0: 2d2d 7064 620a 0a20 2020 4472 6f70 2069  --pdb..   Drop i
+00003ab0: 6e74 6f20 6465 6275 6767 6572 206f 6e20  nto debugger on 
+00003ac0: 6661 696c 7572 6573 206f 7220 6572 726f  failures or erro
+00003ad0: 7273 0a0a 2d2d 7064 622d 6661 696c 7572  rs..--pdb-failur
+00003ae0: 6573 0a0a 2020 2044 726f 7020 696e 746f  es..   Drop into
+00003af0: 2064 6562 7567 6765 7220 6f6e 2066 6169   debugger on fai
+00003b00: 6c75 7265 730a 0a2d 2d70 6462 2d65 7272  lures..--pdb-err
+00003b10: 6f72 730a 0a20 2020 4472 6f70 2069 6e74  ors..   Drop int
+00003b20: 6f20 6465 6275 6767 6572 206f 6e20 6572  o debugger on er
+00003b30: 726f 7273 0a0a 2d2d 6e6f 2d64 6570 7265  rors..--no-depre
+00003b40: 6361 7465 640a 0a20 2020 4469 7361 626c  cated..   Disabl
+00003b50: 6520 7370 6563 6961 6c20 6861 6e64 6c69  e special handli
+00003b60: 6e67 206f 6620 4465 7072 6563 6174 6564  ng of Deprecated
+00003b70: 5465 7374 2065 7863 6570 7469 6f6e 732e  Test exceptions.
+00003b80: 0a0a 2d2d 7769 7468 2d64 6f63 7465 7374  ..--with-doctest
+00003b90: 0a0a 2020 2045 6e61 626c 6520 706c 7567  ..   Enable plug
+00003ba0: 696e 2044 6f63 7465 7374 3a20 4163 7469  in Doctest: Acti
+00003bb0: 7661 7465 2064 6f63 7465 7374 2070 6c75  vate doctest plu
+00003bc0: 6769 6e20 746f 2066 696e 6420 616e 6420  gin to find and 
+00003bd0: 7275 6e0a 2020 2064 6f63 7465 7374 7320  run.   doctests 
+00003be0: 696e 206e 6f6e 2d74 6573 7420 6d6f 6475  in non-test modu
+00003bf0: 6c65 732e 205b 4e4f 5345 5f57 4954 485f  les. [NOSE_WITH_
+00003c00: 444f 4354 4553 545d 0a0a 2d2d 646f 6374  DOCTEST]..--doct
+00003c10: 6573 742d 7465 7374 730a 0a20 2020 416c  est-tests..   Al
+00003c20: 736f 206c 6f6f 6b20 666f 7220 646f 6374  so look for doct
+00003c30: 6573 7473 2069 6e20 7465 7374 206d 6f64  ests in test mod
+00003c40: 756c 6573 2e20 4e6f 7465 2074 6861 7420  ules. Note that 
+00003c50: 636c 6173 7365 732c 206d 6574 686f 6473  classes, methods
+00003c60: 0a20 2020 616e 6420 6675 6e63 7469 6f6e  .   and function
+00003c70: 7320 7368 6f75 6c64 2068 6176 6520 6569  s should have ei
+00003c80: 7468 6572 2064 6f63 7465 7374 7320 6f72  ther doctests or
+00003c90: 206e 6f6e 2d64 6f63 7465 7374 2074 6573   non-doctest tes
+00003ca0: 7473 2c20 6e6f 740a 2020 2062 6f74 682e  ts, not.   both.
+00003cb0: 205b 4e4f 5345 5f44 4f43 5445 5354 5f54   [NOSE_DOCTEST_T
+00003cc0: 4553 5453 5d0a 0a2d 2d64 6f63 7465 7374  ESTS]..--doctest
+00003cd0: 2d65 7874 656e 7369 6f6e 3d45 5854 0a0a  -extension=EXT..
+00003ce0: 2020 2041 6c73 6f20 6c6f 6f6b 2066 6f72     Also look for
+00003cf0: 2064 6f63 7465 7374 7320 696e 2066 696c   doctests in fil
+00003d00: 6573 2077 6974 6820 7468 6973 2065 7874  es with this ext
+00003d10: 656e 7369 6f6e 0a20 2020 5b4e 4f53 455f  ension.   [NOSE_
+00003d20: 444f 4354 4553 545f 4558 5445 4e53 494f  DOCTEST_EXTENSIO
+00003d30: 4e5d 0a0a 2d2d 646f 6374 6573 742d 7265  N]..--doctest-re
+00003d40: 7375 6c74 2d76 6172 6961 626c 653d 5641  sult-variable=VA
+00003d50: 520a 0a20 2020 4368 616e 6765 2074 6865  R..   Change the
+00003d60: 2076 6172 6961 626c 6520 6e61 6d65 2073   variable name s
+00003d70: 6574 2074 6f20 7468 6520 7265 7375 6c74  et to the result
+00003d80: 206f 6620 7468 6520 6c61 7374 2069 6e74   of the last int
+00003d90: 6572 7072 6574 6572 0a20 2020 636f 6d6d  erpreter.   comm
+00003da0: 616e 6420 6672 6f6d 2074 6865 2064 6566  and from the def
+00003db0: 6175 6c74 2027 5f27 2e20 4361 6e20 6265  ault '_'. Can be
+00003dc0: 2075 7365 6420 746f 2061 766f 6964 2063   used to avoid c
+00003dd0: 6f6e 666c 6963 7473 2077 6974 680a 2020  onflicts with.  
+00003de0: 2074 6865 205f 2829 2066 756e 6374 696f   the _() functio
+00003df0: 6e20 7573 6564 2066 6f72 2074 6578 7420  n used for text 
+00003e00: 7472 616e 736c 6174 696f 6e2e 0a20 2020  translation..   
+00003e10: 5b4e 4f53 455f 444f 4354 4553 545f 5245  [NOSE_DOCTEST_RE
+00003e20: 5355 4c54 5f56 4152 5d0a 0a2d 2d64 6f63  SULT_VAR]..--doc
+00003e30: 7465 7374 2d66 6978 7475 7265 733d 5355  test-fixtures=SU
+00003e40: 4646 4958 0a0a 2020 2046 696e 6420 6669  FFIX..   Find fi
+00003e50: 7874 7572 6573 2066 6f72 2061 2064 6f63  xtures for a doc
+00003e60: 7465 7374 2066 696c 6520 696e 206d 6f64  test file in mod
+00003e70: 756c 6520 7769 7468 2074 6869 7320 6e61  ule with this na
+00003e80: 6d65 2061 7070 656e 6465 640a 2020 2074  me appended.   t
+00003e90: 6f20 7468 6520 6261 7365 206e 616d 6520  o the base name 
+00003ea0: 6f66 2074 6865 2064 6f63 7465 7374 2066  of the doctest f
+00003eb0: 696c 650a 0a2d 2d64 6f63 7465 7374 2d6f  ile..--doctest-o
+00003ec0: 7074 696f 6e73 3d4f 5054 494f 4e53 0a0a  ptions=OPTIONS..
+00003ed0: 2020 2053 7065 6369 6679 206f 7074 696f     Specify optio
+00003ee0: 6e73 2074 6f20 7061 7373 2074 6f20 646f  ns to pass to do
+00003ef0: 6374 6573 742e 2045 672e 0a20 2020 272b  ctest. Eg..   '+
+00003f00: 454c 4c49 5053 4953 2c2b 4e4f 524d 414c  ELLIPSIS,+NORMAL
+00003f10: 495a 455f 5748 4954 4553 5041 4345 270a  IZE_WHITESPACE'.
+00003f20: 0a2d 2d77 6974 682d 6973 6f6c 6174 696f  .--with-isolatio
+00003f30: 6e0a 0a20 2020 456e 6162 6c65 2070 6c75  n..   Enable plu
+00003f40: 6769 6e20 4973 6f6c 6174 696f 6e50 6c75  gin IsolationPlu
+00003f50: 6769 6e3a 2041 6374 6976 6174 6520 7468  gin: Activate th
+00003f60: 6520 6973 6f6c 6174 696f 6e20 706c 7567  e isolation plug
+00003f70: 696e 2074 6f0a 2020 2069 736f 6c61 7465  in to.   isolate
+00003f80: 2063 6861 6e67 6573 2074 6f20 6578 7465   changes to exte
+00003f90: 726e 616c 206d 6f64 756c 6573 2074 6f20  rnal modules to 
+00003fa0: 6120 7369 6e67 6c65 2074 6573 7420 6d6f  a single test mo
+00003fb0: 6475 6c65 206f 720a 2020 2070 6163 6b61  dule or.   packa
+00003fc0: 6765 2e20 5468 6520 6973 6f6c 6174 696f  ge. The isolatio
+00003fd0: 6e20 706c 7567 696e 2072 6573 6574 7320  n plugin resets 
+00003fe0: 7468 6520 636f 6e74 656e 7473 206f 6620  the contents of 
+00003ff0: 7379 732e 6d6f 6475 6c65 730a 2020 2061  sys.modules.   a
+00004000: 6674 6572 2065 6163 6820 7465 7374 206d  fter each test m
+00004010: 6f64 756c 6520 6f72 2070 6163 6b61 6765  odule or package
+00004020: 2072 756e 7320 746f 2069 7473 2073 7461   runs to its sta
+00004030: 7465 2062 6566 6f72 6520 7468 650a 2020  te before the.  
+00004040: 2074 6573 742e 2050 4c45 4153 4520 4e4f   test. PLEASE NO
+00004050: 5445 2074 6861 7420 7468 6973 2070 6c75  TE that this plu
+00004060: 6769 6e20 7368 6f75 6c64 206e 6f74 2062  gin should not b
+00004070: 6520 7573 6564 2077 6974 6820 7468 650a  e used with the.
+00004080: 2020 2063 6f76 6572 6167 6520 706c 7567     coverage plug
+00004090: 696e 2c20 6f72 2069 6e20 616e 7920 6f74  in, or in any ot
+000040a0: 6865 7220 6361 7365 2077 6865 7265 206d  her case where m
+000040b0: 6f64 756c 6520 7265 6c6f 6164 696e 6720  odule reloading 
+000040c0: 6d61 790a 2020 2070 726f 6475 6365 2075  may.   produce u
+000040d0: 6e64 6573 6972 6162 6c65 2073 6964 652d  ndesirable side-
+000040e0: 6566 6665 6374 732e 205b 4e4f 5345 5f57  effects. [NOSE_W
+000040f0: 4954 485f 4953 4f4c 4154 494f 4e5d 0a0a  ITH_ISOLATION]..
+00004100: 2d64 2c20 2d2d 6465 7461 696c 6564 2d65  -d, --detailed-e
+00004110: 7272 6f72 732c 202d 2d66 6169 6c75 7265  rrors, --failure
+00004120: 2d64 6574 6169 6c0a 0a20 2020 4164 6420  -detail..   Add 
+00004130: 6465 7461 696c 2074 6f20 6572 726f 7220  detail to error 
+00004140: 6f75 7470 7574 2062 7920 6174 7465 6d70  output by attemp
+00004150: 7469 6e67 2074 6f20 6576 616c 7561 7465  ting to evaluate
+00004160: 2066 6169 6c65 6420 6173 7365 7274 730a   failed asserts.
+00004170: 2020 205b 4e4f 5345 5f44 4554 4149 4c45     [NOSE_DETAILE
+00004180: 445f 4552 524f 5253 5d0a 0a2d 2d6e 6f2d  D_ERRORS]..--no-
+00004190: 736b 6970 0a0a 2020 2044 6973 6162 6c65  skip..   Disable
+000041a0: 2073 7065 6369 616c 2068 616e 646c 696e   special handlin
+000041b0: 6720 6f66 2053 6b69 7054 6573 7420 6578  g of SkipTest ex
+000041c0: 6365 7074 696f 6e73 2e0a 0a2d 2d77 6974  ceptions...--wit
+000041d0: 682d 6964 0a0a 2020 2045 6e61 626c 6520  h-id..   Enable 
+000041e0: 706c 7567 696e 2054 6573 7449 643a 2041  plugin TestId: A
+000041f0: 6374 6976 6174 6520 746f 2061 6464 2061  ctivate to add a
+00004200: 2074 6573 7420 6964 2028 6c69 6b65 2023   test id (like #
+00004210: 3129 2074 6f20 6561 6368 0a20 2020 7465  1) to each.   te
+00004220: 7374 206e 616d 6520 6f75 7470 7574 2e20  st name output. 
+00004230: 4163 7469 7661 7465 2077 6974 6820 2d2d  Activate with --
+00004240: 6661 696c 6564 2074 6f20 7265 7275 6e20  failed to rerun 
+00004250: 6661 696c 696e 6720 7465 7374 730a 2020  failing tests.  
+00004260: 206f 6e6c 792e 205b 4e4f 5345 5f57 4954   only. [NOSE_WIT
+00004270: 485f 4944 5d0a 0a2d 2d69 642d 6669 6c65  H_ID]..--id-file
+00004280: 3d46 494c 450a 0a20 2020 5374 6f72 6520  =FILE..   Store 
+00004290: 7465 7374 2069 6473 2066 6f75 6e64 2069  test ids found i
+000042a0: 6e20 7465 7374 2072 756e 7320 696e 2074  n test runs in t
+000042b0: 6869 7320 6669 6c65 2e20 4465 6661 756c  his file. Defaul
+000042c0: 7420 6973 2074 6865 2066 696c 650a 2020  t is the file.  
+000042d0: 202e 6e6f 7365 6964 7320 696e 2074 6865   .noseids in the
+000042e0: 2077 6f72 6b69 6e67 2064 6972 6563 746f   working directo
+000042f0: 7279 2e0a 0a2d 2d66 6169 6c65 640a 0a20  ry...--failed.. 
+00004300: 2020 5275 6e20 7468 6520 7465 7374 7320    Run the tests 
+00004310: 7468 6174 2066 6169 6c65 6420 696e 2074  that failed in t
+00004320: 6865 206c 6173 7420 7465 7374 2072 756e  he last test run
+00004330: 2e0a 0a2d 2d70 726f 6365 7373 6573 3d4e  ...--processes=N
+00004340: 554d 0a0a 2020 2053 7072 6561 6420 7465  UM..   Spread te
+00004350: 7374 2072 756e 2061 6d6f 6e67 2074 6869  st run among thi
+00004360: 7320 6d61 6e79 2070 726f 6365 7373 6573  s many processes
+00004370: 2e20 5365 7420 6120 6e75 6d62 6572 2065  . Set a number e
+00004380: 7175 616c 2074 6f0a 2020 2074 6865 206e  qual to.   the n
+00004390: 756d 6265 7220 6f66 2070 726f 6365 7373  umber of process
+000043a0: 6f72 7320 6f72 2063 6f72 6573 2069 6e20  ors or cores in 
+000043b0: 796f 7572 206d 6163 6869 6e65 2066 6f72  your machine for
+000043c0: 2062 6573 7420 7265 7375 6c74 732e 0a20   best results.. 
+000043d0: 2020 5061 7373 2061 206e 6567 6174 6976    Pass a negativ
+000043e0: 6520 6e75 6d62 6572 2074 6f20 6861 7665  e number to have
+000043f0: 2074 6865 206e 756d 6265 7220 6f66 2070   the number of p
+00004400: 726f 6365 7373 6573 0a20 2020 6175 746f  rocesses.   auto
+00004410: 6d61 7469 6361 6c6c 7920 7365 7420 746f  matically set to
+00004420: 2074 6865 206e 756d 6265 7220 6f66 2063   the number of c
+00004430: 6f72 6573 2e20 5061 7373 696e 6720 3020  ores. Passing 0 
+00004440: 6d65 616e 7320 746f 0a20 2020 6469 7361  means to.   disa
+00004450: 626c 6520 7061 7261 6c6c 656c 2074 6573  ble parallel tes
+00004460: 7469 6e67 2e20 4465 6661 756c 7420 6973  ting. Default is
+00004470: 2030 2075 6e6c 6573 7320 4e4f 5345 5f50   0 unless NOSE_P
+00004480: 524f 4345 5353 4553 2069 730a 2020 2073  ROCESSES is.   s
+00004490: 6574 2e20 5b4e 4f53 455f 5052 4f43 4553  et. [NOSE_PROCES
+000044a0: 5345 535d 0a0a 2d2d 7072 6f63 6573 732d  SES]..--process-
+000044b0: 7469 6d65 6f75 743d 5345 434f 4e44 530a  timeout=SECONDS.
+000044c0: 0a20 2020 5365 7420 7469 6d65 6f75 7420  .   Set timeout 
+000044d0: 666f 7220 7265 7475 726e 206f 6620 7265  for return of re
+000044e0: 7375 6c74 7320 6672 6f6d 2065 6163 6820  sults from each 
+000044f0: 7465 7374 2072 756e 6e65 7220 7072 6f63  test runner proc
+00004500: 6573 732e 0a20 2020 4465 6661 756c 7420  ess..   Default 
+00004510: 6973 2031 302e 205b 4e4f 5345 5f50 524f  is 10. [NOSE_PRO
+00004520: 4345 5353 5f54 494d 454f 5554 5d0a 0a2d  CESS_TIMEOUT]..-
+00004530: 2d70 726f 6365 7373 2d72 6573 7461 7274  -process-restart
+00004540: 776f 726b 6572 0a0a 2020 2049 6620 7365  worker..   If se
+00004550: 742c 2077 696c 6c20 7265 7374 6172 7420  t, will restart 
+00004560: 6561 6368 2077 6f72 6b65 7220 7072 6f63  each worker proc
+00004570: 6573 7320 6f6e 6365 2074 6865 6972 2074  ess once their t
+00004580: 6573 7473 2061 7265 2064 6f6e 652c 0a20  ests are done,. 
+00004590: 2020 7468 6973 2068 656c 7073 2063 6f6e    this helps con
+000045a0: 7472 6f6c 206d 656d 6f72 7920 6c65 616b  trol memory leak
+000045b0: 7320 6672 6f6d 206b 696c 6c69 6e67 2074  s from killing t
+000045c0: 6865 2073 7973 7465 6d2e 0a20 2020 5b4e  he system..   [N
+000045d0: 4f53 455f 5052 4f43 4553 535f 5245 5354  OSE_PROCESS_REST
+000045e0: 4152 5457 4f52 4b45 525d 0a0a 2d2d 7769  ARTWORKER]..--wi
+000045f0: 7468 2d78 756e 6974 0a0a 2020 2045 6e61  th-xunit..   Ena
+00004600: 626c 6520 706c 7567 696e 2058 756e 6974  ble plugin Xunit
+00004610: 3a20 5468 6973 2070 6c75 6769 6e20 7072  : This plugin pr
+00004620: 6f76 6964 6573 2074 6573 7420 7265 7375  ovides test resu
+00004630: 6c74 7320 696e 2074 6865 0a20 2020 7374  lts in the.   st
+00004640: 616e 6461 7264 2058 556e 6974 2058 4d4c  andard XUnit XML
+00004650: 2066 6f72 6d61 742e 205b 4e4f 5345 5f57   format. [NOSE_W
+00004660: 4954 485f 5855 4e49 545d 0a0a 2d2d 7875  ITH_XUNIT]..--xu
+00004670: 6e69 742d 6669 6c65 3d46 494c 450a 0a20  nit-file=FILE.. 
+00004680: 2020 5061 7468 2074 6f20 786d 6c20 6669    Path to xml fi
+00004690: 6c65 2074 6f20 7374 6f72 6520 7468 6520  le to store the 
+000046a0: 7875 6e69 7420 7265 706f 7274 2069 6e2e  xunit report in.
+000046b0: 2044 6566 6175 6c74 2069 730a 2020 206e   Default is.   n
+000046c0: 6f73 6574 6573 7473 2e78 6d6c 2069 6e20  osetests.xml in 
+000046d0: 7468 6520 776f 726b 696e 6720 6469 7265  the working dire
+000046e0: 6374 6f72 7920 5b4e 4f53 455f 5855 4e49  ctory [NOSE_XUNI
+000046f0: 545f 4649 4c45 5d0a 0a2d 2d78 756e 6974  T_FILE]..--xunit
+00004700: 2d74 6573 7473 7569 7465 2d6e 616d 653d  -testsuite-name=
+00004710: 5041 434b 4147 450a 0a20 2020 4e61 6d65  PACKAGE..   Name
+00004720: 206f 6620 7468 6520 7465 7374 7375 6974   of the testsuit
+00004730: 6520 696e 2074 6865 2078 756e 6974 2078  e in the xunit x
+00004740: 6d6c 2c20 6765 6e65 7261 7465 6420 6279  ml, generated by
+00004750: 2070 6c75 6769 6e2e 0a20 2020 4465 6661   plugin..   Defa
+00004760: 756c 7420 7465 7374 2073 7569 7465 206e  ult test suite n
+00004770: 616d 6520 6973 206e 6f73 6574 6573 7473  ame is nosetests
+00004780: 2e0a 0a2d 2d61 6c6c 2d6d 6f64 756c 6573  ...--all-modules
+00004790: 0a0a 2020 2045 6e61 626c 6520 706c 7567  ..   Enable plug
+000047a0: 696e 2041 6c6c 4d6f 6475 6c65 733a 2043  in AllModules: C
+000047b0: 6f6c 6c65 6374 2074 6573 7473 2066 726f  ollect tests fro
+000047c0: 6d20 616c 6c20 7079 7468 6f6e 206d 6f64  m all python mod
+000047d0: 756c 6573 2e0a 2020 205b 4e4f 5345 5f41  ules..   [NOSE_A
+000047e0: 4c4c 5f4d 4f44 554c 4553 5d0a 0a2d 2d63  LL_MODULES]..--c
+000047f0: 6f2c 202d 2d63 6f6c 6c65 6374 2d6f 6e6c  o, --collect-onl
+00004800: 790a 0a20 2020 456e 6162 6c65 2063 6f6c  y..   Enable col
+00004810: 6c65 6374 2d6f 6e6c 793a 2043 6f6c 6c65  lect-only: Colle
+00004820: 6374 2061 6e64 206f 7574 7075 7420 7465  ct and output te
+00004830: 7374 206e 616d 6573 206f 6e6c 792c 0a20  st names only,. 
+00004840: 2020 6275 7420 646f 206e 6f74 2072 756e    but do not run
+00004850: 2061 6e79 2074 6573 7473 2e20 5b43 4f4c   any tests. [COL
+00004860: 4c45 4354 5f4f 4e4c 595d 0a60 6060 0a    LECT_ONLY].```.
```

### Comparing `pynose-1.4.5/README.md` & `pynose-1.4.6/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,1062 +1,1068 @@
-00000000: 2320 7079 6e6f 7365 0a0a 2323 2320 6060  # pynose..### ``
-00000010: 7079 6e6f 7365 6060 2066 6978 6573 2060  pynose`` fixes `
-00000020: 606e 6f73 6560 6020 746f 2065 7874 656e  `nose`` to exten
-00000030: 6420 5b75 6e69 7474 6573 745d 2868 7474  d [unittest](htt
-00000040: 7073 3a2f 2f64 6f63 732e 7079 7468 6f6e  ps://docs.python
-00000050: 2e6f 7267 2f33 2f6c 6962 7261 7279 2f75  .org/3/library/u
-00000060: 6e69 7474 6573 742e 6874 6d6c 2920 616e  nittest.html) an
-00000070: 6420 6d61 6b65 2074 6573 7469 6e67 2065  d make testing e
-00000080: 6173 6965 722e 0a0a 284e 4f54 453a 2049  asier...(NOTE: I
-00000090: 6620 796f 7520 6361 6e2c 2075 7365 202a  f you can, use *
-000000a0: 2a5b 7079 7465 7374 5d28 6874 7470 733a  *[pytest](https:
-000000b0: 2f2f 646f 6373 2e70 7974 6573 742e 6f72  //docs.pytest.or
-000000c0: 672f 292a 2a20 696e 7374 6561 642e 202a  g/)** instead. *
-000000d0: 2a5b 7079 6e6f 7365 5d28 6874 7470 733a  *[pynose](https:
-000000e0: 2f2f 6769 7468 7562 2e63 6f6d 2f6d 646d  //github.com/mdm
-000000f0: 696e 747a 2f70 796e 6f73 6529 2a2a 2077  intz/pynose)** w
-00000100: 6173 2062 7569 6c74 2074 6f20 6d61 696e  as built to main
-00000110: 7461 696e 202a 2a5b 6e6f 7365 5d28 6874  tain **[nose](ht
-00000120: 7470 733a 2f2f 6e6f 7365 2e72 6561 6474  tps://nose.readt
-00000130: 6865 646f 6373 2e69 6f2f 656e 2f6c 6174  hedocs.io/en/lat
-00000140: 6573 742f 292a 2a20 666f 7220 6465 7665  est/)** for deve
-00000150: 6c6f 7065 7273 2077 686f 2073 7469 6c6c  lopers who still
-00000160: 2075 7365 2069 742e 290a 0a2d 2d2d 2d2d   use it.)..-----
-00000170: 2d2d 2d0a 0a60 6070 796e 6f73 6560 6020  ---..``pynose`` 
-00000180: 6973 2061 6e20 7570 6461 7465 6420 7665  is an updated ve
-00000190: 7273 696f 6e20 6f66 2060 606e 6f73 6560  rsion of ``nose`
-000001a0: 602c 206f 7269 6769 6e61 6c6c 7920 6d61  `, originally ma
-000001b0: 6465 2062 7920 4a61 736f 6e20 5065 6c6c  de by Jason Pell
-000001c0: 6572 696e 2e0a 0a54 6869 7320 7665 7273  erin...This vers
-000001d0: 696f 6e20 6f66 2060 606e 6f73 6560 6020  ion of ``nose`` 
-000001e0: 6973 2063 6f6d 7061 7469 626c 6520 7769  is compatible wi
-000001f0: 7468 2050 7974 686f 6e20 332e 362b 2028  th Python 3.6+ (
-00000200: 696e 636c 7564 696e 6720 332e 3132 2026  including 3.12 &
-00000210: 2075 7029 2e0a 0a43 6861 6e67 6573 2069   up)...Changes i
-00000220: 6e20 6060 7079 6e6f 7365 6060 2066 726f  n ``pynose`` fro
-00000230: 6d20 6c65 6761 6379 2060 606e 6f73 6560  m legacy ``nose`
-00000240: 6020 696e 636c 7564 653a 0a2a 2046 6978  ` include:.* Fix
-00000250: 6573 2022 4174 7472 6962 7574 6545 7272  es "AttributeErr
-00000260: 6f72 3a20 6d6f 6475 6c65 2027 636f 6c6c  or: module 'coll
-00000270: 6563 7469 6f6e 7327 2068 6173 206e 6f20  ections' has no 
-00000280: 6174 7472 6962 7574 6520 2743 616c 6c61  attribute 'Calla
-00000290: 626c 6527 2e22 0a2a 2046 6978 6573 2022  ble'.".* Fixes "
-000002a0: 4174 7472 6962 7574 6545 7272 6f72 3a20  AttributeError: 
-000002b0: 6d6f 6475 6c65 2027 696e 7370 6563 7427  module 'inspect'
-000002c0: 2068 6173 206e 6f20 6174 7472 6962 7574   has no attribut
-000002d0: 6520 2767 6574 6172 6773 7065 6327 2e22  e 'getargspec'."
-000002e0: 0a2a 2046 6978 6573 2022 496d 706f 7274  .* Fixes "Import
-000002f0: 4572 726f 723a 2063 616e 6e6f 7420 696d  Error: cannot im
-00000300: 706f 7274 206e 616d 6520 275f 5465 7874  port name '_Text
-00000310: 5465 7374 5265 7375 6c74 2720 6672 6f6d  TestResult' from
-00000320: 2027 756e 6974 7465 7374 272e 220a 2a20   'unittest'.".* 
-00000330: 4669 7865 7320 2252 756e 7469 6d65 5761  Fixes "RuntimeWa
-00000340: 726e 696e 673a 2054 6573 7452 6573 756c  rning: TestResul
-00000350: 7420 6861 7320 6e6f 2061 6464 4475 7261  t has no addDura
-00000360: 7469 6f6e 206d 6574 686f 642e 220a 2a20  tion method.".* 
-00000370: 4669 7865 7320 616c 6c20 6060 666c 616b  Fixes all ``flak
-00000380: 6538 6060 2069 7373 7565 7320 6672 6f6d  e8`` issues from
-00000390: 2074 6865 206f 7269 6769 6e61 6c20 6060   the original ``
-000003a0: 6e6f 7365 6060 2e0a 2a20 5265 706c 6163  nose``..* Replac
-000003b0: 6573 2074 6865 2060 6069 6d70 6060 206d  es the ``imp`` m
-000003c0: 6f64 756c 6520 7769 7468 2074 6865 206e  odule with the n
-000003d0: 6577 6572 2060 6069 6d70 6f72 746c 6962  ewer ``importlib
-000003e0: 6060 206d 6f64 756c 652e 0a2a 2054 6865  `` module..* The
-000003f0: 2064 6566 6175 6c74 206c 6f67 6769 6e67   default logging
-00000400: 206c 6576 656c 206e 6f77 2068 6964 6573   level now hides
-00000410: 2022 6465 6275 6722 206c 6f67 7320 666f   "debug" logs fo
-00000420: 7220 6c65 7373 206e 6f69 7365 2e0a 2a20  r less noise..* 
-00000430: 5468 6520 6060 2d73 6060 206f 7074 696f  The ``-s`` optio
-00000440: 6e20 6973 2061 6c77 6179 7320 6163 7469  n is always acti
-00000450: 7665 2074 6f20 7365 6520 7468 6520 6f75  ve to see the ou
-00000460: 7470 7574 206f 6620 6060 7072 696e 7428  tput of ``print(
-00000470: 2960 602e 0a2a 2041 6464 7320 6060 2d2d  )``..* Adds ``--
-00000480: 636f 6060 2061 7320 6120 7368 6f72 7463  co`` as a shortc
-00000490: 7574 2074 6f20 7573 696e 6720 6060 2d2d  ut to using ``--
-000004a0: 636f 6c6c 6563 742d 6f6e 6c79 6060 2e0a  collect-only``..
-000004b0: 0a2d 2d2d 2d2d 2d2d 2d0a 0a54 6865 206f  .--------..The o
-000004c0: 7269 6769 6e61 6c20 6465 7363 7269 7074  riginal descript
-000004d0: 696f 6e20 6f66 2060 606e 6f73 6560 603a  ion of ``nose``:
-000004e0: 0a0a 3e6e 6f73 6520 6578 7465 6e64 7320  ..>nose extends 
-000004f0: 7468 6520 7465 7374 206c 6f61 6469 6e67  the test loading
-00000500: 2061 6e64 2072 756e 6e69 6e67 2066 6561   and running fea
-00000510: 7475 7265 7320 6f66 2075 6e69 7474 6573  tures of unittes
-00000520: 742c 206d 616b 696e 670a 6974 2065 6173  t, making.it eas
-00000530: 6965 7220 746f 2077 7269 7465 2c20 6669  ier to write, fi
-00000540: 6e64 2061 6e64 2072 756e 2074 6573 7473  nd and run tests
-00000550: 2e0a 0a3e 4279 2064 6566 6175 6c74 2c20  ...>By default, 
-00000560: 6e6f 7365 2072 756e 7320 7465 7374 7320  nose runs tests 
-00000570: 696e 2066 696c 6573 206f 7220 6469 7265  in files or dire
-00000580: 6374 6f72 6965 7320 756e 6465 7220 7468  ctories under th
-00000590: 6520 6375 7272 656e 740a 776f 726b 696e  e current.workin
-000005a0: 6720 6469 7265 6374 6f72 7920 7768 6f73  g directory whos
-000005b0: 6520 6e61 6d65 7320 696e 636c 7564 6520  e names include 
-000005c0: 2274 6573 7422 206f 7220 2254 6573 7422  "test" or "Test"
-000005d0: 2061 7420 6120 776f 7264 0a62 6f75 6e64   at a word.bound
-000005e0: 6172 7920 286c 696b 6520 2274 6573 745f  ary (like "test_
-000005f0: 7468 6973 2220 6f72 2022 6675 6e63 7469  this" or "functi
-00000600: 6f6e 616c 5f74 6573 7422 206f 7220 2254  onal_test" or "T
-00000610: 6573 7443 6c61 7373 2220 6275 7420 6e6f  estClass" but no
-00000620: 740a 226c 6962 7465 7374 2229 2e20 5465  t."libtest"). Te
-00000630: 7374 206f 7574 7075 7420 6973 2073 696d  st output is sim
-00000640: 696c 6172 2074 6f20 7468 6174 206f 6620  ilar to that of 
-00000650: 756e 6974 7465 7374 2c20 6275 7420 616c  unittest, but al
-00000660: 736f 2069 6e63 6c75 6465 730a 6361 7074  so includes.capt
-00000670: 7572 6564 2073 7464 6f75 7420 6f75 7470  ured stdout outp
-00000680: 7574 2066 726f 6d20 6661 696c 696e 6720  ut from failing 
-00000690: 7465 7374 732c 2066 6f72 2065 6173 7920  tests, for easy 
-000006a0: 7072 696e 742d 7374 796c 6520 6465 6275  print-style debu
-000006b0: 6767 696e 672e 0a0a 3e54 6865 7365 2066  gging...>These f
-000006c0: 6561 7475 7265 732c 2061 6e64 206d 616e  eatures, and man
-000006d0: 7920 6d6f 7265 2c20 6172 6520 6375 7374  y more, are cust
-000006e0: 6f6d 697a 6162 6c65 2074 6872 6f75 6768  omizable through
-000006f0: 2074 6865 2075 7365 206f 660a 706c 7567   the use of.plug
-00000700: 696e 732e 2050 6c75 6769 6e73 2069 6e63  ins. Plugins inc
-00000710: 6c75 6465 6420 7769 7468 206e 6f73 6520  luded with nose 
-00000720: 7072 6f76 6964 6520 7375 7070 6f72 7420  provide support 
-00000730: 666f 7220 646f 6374 6573 742c 2063 6f64  for doctest, cod
-00000740: 650a 636f 7665 7261 6765 2061 6e64 2070  e.coverage and p
-00000750: 726f 6669 6c69 6e67 2c20 666c 6578 6962  rofiling, flexib
-00000760: 6c65 2061 7474 7269 6275 7465 2d62 6173  le attribute-bas
-00000770: 6564 2074 6573 7420 7365 6c65 6374 696f  ed test selectio
-00000780: 6e2c 0a6f 7574 7075 7420 6361 7074 7572  n,.output captur
-00000790: 6520 616e 6420 6d6f 7265 2e20 4d6f 7265  e and more. More
-000007a0: 2069 6e66 6f72 6d61 7469 6f6e 2061 626f   information abo
-000007b0: 7574 2077 7269 7469 6e67 2070 6c75 6769  ut writing plugi
-000007c0: 6e73 0a6d 6179 2062 6520 666f 756e 6420  ns.may be found 
-000007d0: 6f6e 2069 6e20 7468 6520 6e6f 7365 2041  on in the nose A
-000007e0: 5049 2064 6f63 756d 656e 7461 7469 6f6e  PI documentation
-000007f0: 2c20 6865 7265 3a0a 6874 7470 733a 2f2f  , here:.https://
-00000800: 6e6f 7365 2e72 6561 6474 6865 646f 6373  nose.readthedocs
-00000810: 2e69 6f2f 656e 2f6c 6174 6573 742f 0a0a  .io/en/latest/..
-00000820: 2d2d 2d2d 2d2d 2d2d 0a0a 6060 6062 6173  --------..```bas
-00000830: 680a 0a42 6173 6963 2075 7361 6765 0a2a  h..Basic usage.*
-00000840: 2a2a 2a2a 2a2a 2a2a 2a2a 0a0a 5573 6520  **********..Use 
-00000850: 2270 796e 6f73 6522 204f 5220 226e 6f73  "pynose" OR "nos
-00000860: 6574 6573 7473 2220 746f 2072 756e 2074  etests" to run t
-00000870: 6573 7473 3a0a 0a20 2020 2070 796e 6f73  ests:..    pynos
-00000880: 6520 5b6f 7074 696f 6e73 5d20 5b28 6f70  e [options] [(op
-00000890: 7469 6f6e 616c 2920 7465 7374 2066 696c  tional) test fil
-000008a0: 6573 206f 7220 6469 7265 6374 6f72 6965  es or directorie
-000008b0: 735d 0a0a 2020 2020 6e6f 7365 7465 7374  s]..    nosetest
-000008c0: 7320 5b6f 7074 696f 6e73 5d20 5b28 6f70  s [options] [(op
-000008d0: 7469 6f6e 616c 2920 7465 7374 2066 696c  tional) test fil
-000008e0: 6573 206f 7220 6469 7265 6374 6f72 6965  es or directorie
-000008f0: 735d 0a0a 496e 2061 6464 6974 696f 6e20  s]..In addition 
-00000900: 746f 2070 6173 7369 6e67 2063 6f6d 6d61  to passing comma
-00000910: 6e64 2d6c 696e 6520 6f70 7469 6f6e 732c  nd-line options,
-00000920: 2079 6f75 206d 6179 2061 6c73 6f20 7075   you may also pu
-00000930: 740a 636f 6e66 6967 7572 6174 696f 6e20  t.configuration 
-00000940: 6f70 7469 6f6e 7320 696e 2061 202e 6e6f  options in a .no
-00000950: 7365 7263 206f 7220 6e6f 7365 2e63 6667  serc or nose.cfg
-00000960: 2066 696c 6520 696e 2079 6f75 7220 686f   file in your ho
-00000970: 6d65 0a64 6972 6563 746f 7279 2e20 5468  me.directory. Th
-00000980: 6573 6520 6172 6520 7374 616e 6461 7264  ese are standard
-00000990: 202e 696e 692d 7374 796c 6520 636f 6e66   .ini-style conf
-000009a0: 6967 2066 696c 6573 2e20 5075 7420 796f  ig files. Put yo
-000009b0: 7572 0a6e 6f73 6574 6573 7473 2063 6f6e  ur.nosetests con
-000009c0: 6669 6775 7261 7469 6f6e 2069 6e20 6120  figuration in a 
-000009d0: 5b6e 6f73 6574 6573 7473 5d20 7365 6374  [nosetests] sect
-000009e0: 696f 6e2c 2077 6974 6820 7468 6520 2d2d  ion, with the --
-000009f0: 2070 7265 6669 780a 7265 6d6f 7665 643a   prefix.removed:
-00000a00: 0a0a 2020 205b 6e6f 7365 7465 7374 735d  ..   [nosetests]
-00000a10: 0a20 2020 7665 7262 6f73 6974 793d 330a  .   verbosity=3.
-00000a20: 2020 2077 6974 682d 646f 6374 6573 743d     with-doctest=
-00000a30: 310a 0a54 6865 7265 2069 7320 616c 736f  1..There is also
-00000a40: 2070 6f73 7369 626c 6974 7920 746f 2064   possiblity to d
-00000a50: 6973 6162 6c65 2063 6f6e 6669 6775 7261  isable configura
-00000a60: 7469 6f6e 2066 696c 6573 206c 6f61 6469  tion files loadi
-00000a70: 6e67 2028 6d69 6768 740a 6265 2075 7365  ng (might.be use
-00000a80: 6675 6c20 7768 656e 2072 756e 6e69 6720  ful when runnig 
-00000a90: 692e 652e 2074 6f78 2061 6e64 2079 6f75  i.e. tox and you
-00000aa0: 2064 6f20 6e6f 7420 7761 6e74 2079 6f75   do not want you
-00000ab0: 7220 676c 6f62 616c 206e 6f73 650a 636f  r global nose.co
-00000ac0: 6e66 6967 2066 696c 6520 746f 2062 6520  nfig file to be 
-00000ad0: 7573 6564 2062 7920 746f 7829 2e20 496e  used by tox). In
-00000ae0: 206f 7264 6572 2074 6f20 6967 6e6f 7265   order to ignore
-00000af0: 2074 686f 7365 2063 6f6e 6669 6775 7261   those configura
-00000b00: 7469 6f6e 0a66 696c 6573 2073 696d 706c  tion.files simpl
-00000b10: 7920 7365 7420 616e 2065 6e76 6972 6f6e  y set an environ
-00000b20: 6d65 6e74 2076 6172 6961 626c 6520 224e  ment variable "N
-00000b30: 4f53 455f 4947 4e4f 5245 5f43 4f4e 4649  OSE_IGNORE_CONFI
-00000b40: 475f 4649 4c45 5322 2e0a 0a54 6865 7265  G_FILES"...There
-00000b50: 2061 7265 2073 6576 6572 616c 206f 7468   are several oth
-00000b60: 6572 2077 6179 7320 746f 2075 7365 2074  er ways to use t
-00000b70: 6865 206e 6f73 6520 7465 7374 2072 756e  he nose test run
-00000b80: 6e65 7220 6265 7369 6465 7320 7468 650a  ner besides the.
-00000b90: 2a6e 6f73 6574 6573 7473 2a20 7363 7269  *nosetests* scri
-00000ba0: 7074 2e20 596f 7520 6d61 7920 7573 6520  pt. You may use 
-00000bb0: 6e6f 7365 2069 6e20 6120 7465 7374 2073  nose in a test s
-00000bc0: 6372 6970 743a 0a0a 2020 2069 6d70 6f72  cript:..   impor
-00000bd0: 7420 6e6f 7365 0a20 2020 6e6f 7365 2e6d  t nose.   nose.m
-00000be0: 6169 6e28 290a 0a49 6620 796f 7520 646f  ain()..If you do
-00000bf0: 206e 6f74 2077 616e 7420 7468 6520 7465   not want the te
-00000c00: 7374 2073 6372 6970 7420 746f 2065 7869  st script to exi
-00000c10: 7420 7769 7468 2030 206f 6e20 7375 6363  t with 0 on succ
-00000c20: 6573 7320 616e 6420 3120 6f6e 0a66 6169  ess and 1 on.fai
-00000c30: 6c75 7265 2028 6c69 6b65 2075 6e69 7474  lure (like unitt
-00000c40: 6573 742e 6d61 696e 292c 2075 7365 206e  est.main), use n
-00000c50: 6f73 652e 7275 6e28 2920 696e 7374 6561  ose.run() instea
-00000c60: 643a 0a0a 2020 2069 6d70 6f72 7420 6e6f  d:..   import no
-00000c70: 7365 0a20 2020 7265 7375 6c74 203d 206e  se.   result = n
-00000c80: 6f73 652e 7275 6e28 290a 0a2a 7265 7375  ose.run()..*resu
-00000c90: 6c74 2a20 7769 6c6c 2062 6520 7472 7565  lt* will be true
-00000ca0: 2069 6620 7468 6520 7465 7374 2072 756e   if the test run
-00000cb0: 2073 7563 6365 6564 6564 2c20 6f72 2066   succeeded, or f
-00000cc0: 616c 7365 2069 6620 616e 7920 7465 7374  alse if any test
-00000cd0: 0a66 6169 6c65 6420 6f72 2072 6169 7365  .failed or raise
-00000ce0: 6420 616e 2075 6e63 6175 6768 7420 6578  d an uncaught ex
-00000cf0: 6365 7074 696f 6e2e 204c 6173 746c 792c  ception. Lastly,
-00000d00: 2079 6f75 2063 616e 2072 756e 206e 6f73   you can run nos
-00000d10: 652e 636f 7265 0a64 6972 6563 746c 792c  e.core.directly,
-00000d20: 2077 6869 6368 2077 696c 6c20 7275 6e20   which will run 
-00000d30: 6e6f 7365 2e6d 6169 6e28 293a 0a0a 2020  nose.main():..  
-00000d40: 2070 7974 686f 6e20 2f70 6174 682f 746f   python /path/to
-00000d50: 2f6e 6f73 652f 636f 7265 2e70 790a 0a50  /nose/core.py..P
-00000d60: 6c65 6173 6520 7365 6520 7468 6520 7573  lease see the us
-00000d70: 6167 6520 6d65 7373 6167 6520 666f 7220  age message for 
-00000d80: 7468 6520 6e6f 7365 7465 7374 7320 7363  the nosetests sc
-00000d90: 7269 7074 2066 6f72 2069 6e66 6f72 6d61  ript for informa
-00000da0: 7469 6f6e 0a61 626f 7574 2068 6f77 2074  tion.about how t
-00000db0: 6f20 636f 6e74 726f 6c20 7768 6963 6820  o control which 
-00000dc0: 7465 7374 7320 6e6f 7365 2072 756e 732c  tests nose runs,
-00000dd0: 2077 6869 6368 2070 6c75 6769 6e73 2061   which plugins a
-00000de0: 7265 206c 6f61 6465 642c 0a61 6e64 2074  re loaded,.and t
-00000df0: 6865 2074 6573 7420 6f75 7470 7574 2e0a  he test output..
-00000e00: 0a0a 4578 7465 6e64 6564 2075 7361 6765  ..Extended usage
-00000e10: 0a3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d0a  .==============.
-00000e20: 0a6e 6f73 6520 636f 6c6c 6563 7473 2074  .nose collects t
-00000e30: 6573 7473 2061 7574 6f6d 6174 6963 616c  ests automatical
-00000e40: 6c79 2066 726f 6d20 7079 7468 6f6e 2073  ly from python s
-00000e50: 6f75 7263 6520 6669 6c65 732c 0a64 6972  ource files,.dir
-00000e60: 6563 746f 7269 6573 2061 6e64 2070 6163  ectories and pac
-00000e70: 6b61 6765 7320 666f 756e 6420 696e 2069  kages found in i
-00000e80: 7473 2077 6f72 6b69 6e67 2064 6972 6563  ts working direc
-00000e90: 746f 7279 2028 7768 6963 680a 6465 6661  tory (which.defa
-00000ea0: 756c 7473 2074 6f20 7468 6520 6375 7272  ults to the curr
-00000eb0: 656e 7420 776f 726b 696e 6720 6469 7265  ent working dire
-00000ec0: 6374 6f72 7929 2e20 416e 7920 7079 7468  ctory). Any pyth
-00000ed0: 6f6e 2073 6f75 7263 6520 6669 6c65 2c0a  on source file,.
-00000ee0: 6469 7265 6374 6f72 7920 6f72 2070 6163  directory or pac
-00000ef0: 6b61 6765 2074 6861 7420 6d61 7463 6865  kage that matche
-00000f00: 7320 7468 6520 7465 7374 4d61 7463 6820  s the testMatch 
-00000f10: 7265 6775 6c61 7220 6578 7072 6573 7369  regular expressi
-00000f20: 6f6e 2028 6279 0a64 6566 6175 6c74 3a20  on (by.default: 
-00000f30: 2a28 3f3a 5e7c 5b62 5f2e 2d5d 295b 5474  *(?:^|[b_.-])[Tt
-00000f40: 5d65 7374 292a 2077 696c 6c20 6265 2063  ]est)* will be c
-00000f50: 6f6c 6c65 6374 6564 2061 7320 6120 7465  ollected as a te
-00000f60: 7374 2028 6f72 2073 6f75 7263 650a 666f  st (or source.fo
-00000f70: 7220 636f 6c6c 6563 7469 6f6e 206f 6620  r collection of 
-00000f80: 7465 7374 7329 2e20 496e 2061 6464 6974  tests). In addit
-00000f90: 696f 6e2c 2061 6c6c 206f 7468 6572 2070  ion, all other p
-00000fa0: 6163 6b61 6765 7320 666f 756e 6420 696e  ackages found in
-00000fb0: 2074 6865 0a77 6f72 6b69 6e67 2064 6972   the.working dir
-00000fc0: 6563 746f 7279 2077 696c 6c20 6265 2065  ectory will be e
-00000fd0: 7861 6d69 6e65 6420 666f 7220 7079 7468  xamined for pyth
-00000fe0: 6f6e 2073 6f75 7263 6520 6669 6c65 7320  on source files 
-00000ff0: 6f72 0a64 6972 6563 746f 7269 6573 2074  or.directories t
-00001000: 6861 7420 6d61 7463 6820 7465 7374 4d61  hat match testMa
-00001010: 7463 682e 2050 6163 6b61 6765 2064 6973  tch. Package dis
-00001020: 636f 7665 7279 2064 6573 6365 6e64 7320  covery descends 
-00001030: 616c 6c20 7468 650a 7761 7920 646f 776e  all the.way down
-00001040: 2074 6865 2074 7265 652c 2073 6f20 7061   the tree, so pa
-00001050: 636b 6167 652e 7465 7374 7320 616e 6420  ckage.tests and 
-00001060: 7061 636b 6167 652e 7375 622e 7465 7374  package.sub.test
-00001070: 7320 616e 640a 7061 636b 6167 652e 7375  s and.package.su
-00001080: 622e 7375 6232 2e74 6573 7473 2077 696c  b.sub2.tests wil
-00001090: 6c20 616c 6c20 6265 2063 6f6c 6c65 6374  l all be collect
-000010a0: 6564 2e0a 0a57 6974 6869 6e20 6120 7465  ed...Within a te
-000010b0: 7374 2064 6972 6563 746f 7279 206f 7220  st directory or 
-000010c0: 7061 636b 6167 652c 2061 6e79 2070 7974  package, any pyt
-000010d0: 686f 6e20 736f 7572 6365 2066 696c 6520  hon source file 
-000010e0: 6d61 7463 6869 6e67 0a74 6573 744d 6174  matching.testMat
-000010f0: 6368 2077 696c 6c20 6265 2065 7861 6d69  ch will be exami
-00001100: 6e65 6420 666f 7220 7465 7374 2063 6173  ned for test cas
-00001110: 6573 2e20 5769 7468 696e 2061 2074 6573  es. Within a tes
-00001120: 7420 6d6f 6475 6c65 2c0a 6675 6e63 7469  t module,.functi
-00001130: 6f6e 7320 616e 6420 636c 6173 7365 7320  ons and classes 
-00001140: 7768 6f73 6520 6e61 6d65 7320 6d61 7463  whose names matc
-00001150: 6820 7465 7374 4d61 7463 6820 616e 6420  h testMatch and 
-00001160: 5465 7374 4361 7365 0a73 7562 636c 6173  TestCase.subclas
-00001170: 7365 7320 7769 7468 2061 6e79 206e 616d  ses with any nam
-00001180: 6520 7769 6c6c 2062 6520 6c6f 6164 6564  e will be loaded
-00001190: 2061 6e64 2065 7865 6375 7465 6420 6173   and executed as
-000011a0: 2074 6573 7473 2e20 5465 7374 730a 6d61   tests. Tests.ma
-000011b0: 7920 7573 6520 7468 6520 6173 7365 7274  y use the assert
-000011c0: 206b 6579 776f 7264 206f 7220 7261 6973   keyword or rais
-000011d0: 6520 4173 7365 7274 696f 6e45 7272 6f72  e AssertionError
-000011e0: 7320 746f 2069 6e64 6963 6174 6520 7465  s to indicate te
-000011f0: 7374 0a66 6169 6c75 7265 2e20 5465 7374  st.failure. Test
-00001200: 4361 7365 2073 7562 636c 6173 7365 7320  Case subclasses 
-00001210: 6d61 7920 646f 2074 6865 2073 616d 6520  may do the same 
-00001220: 6f72 2075 7365 2074 6865 2076 6172 696f  or use the vario
-00001230: 7573 0a54 6573 7443 6173 6520 6d65 7468  us.TestCase meth
-00001240: 6f64 7320 6176 6169 6c61 626c 652e 0a0a  ods available...
-00001250: 2a2a 4974 2069 7320 696d 706f 7274 616e  **It is importan
-00001260: 7420 746f 206e 6f74 6520 7468 6174 2074  t to note that t
-00001270: 6865 2064 6566 6175 6c74 2062 6568 6176  he default behav
-00001280: 696f 7220 6f66 206e 6f73 6520 6973 2074  ior of nose is t
-00001290: 6f20 6e6f 740a 696e 636c 7564 6520 7465  o not.include te
-000012a0: 7374 7320 6672 6f6d 2066 696c 6573 2077  sts from files w
-000012b0: 6869 6368 2061 7265 2065 7865 6375 7461  hich are executa
-000012c0: 626c 652e 2a2a 2020 546f 2069 6e63 6c75  ble.**  To inclu
-000012d0: 6465 2074 6573 7473 0a66 726f 6d20 7375  de tests.from su
-000012e0: 6368 2066 696c 6573 2c20 7265 6d6f 7665  ch files, remove
-000012f0: 2074 6865 6972 2065 7865 6375 7461 626c   their executabl
-00001300: 6520 6269 7420 6f72 2075 7365 2074 6865  e bit or use the
-00001310: 202d 2d65 7865 2066 6c61 670a 2873 6565   --exe flag.(see
-00001320: 2027 4f70 7469 6f6e 7327 2073 6563 7469   'Options' secti
-00001330: 6f6e 2062 656c 6f77 292e 0a0a 0a53 656c  on below)....Sel
-00001340: 6563 7469 6e67 2054 6573 7473 0a2d 2d2d  ecting Tests.---
-00001350: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0a0a 546f  ------------..To
-00001360: 2073 7065 6369 6679 2077 6869 6368 2074   specify which t
-00001370: 6573 7473 2074 6f20 7275 6e2c 2070 6173  ests to run, pas
-00001380: 7320 7465 7374 206e 616d 6573 206f 6e20  s test names on 
-00001390: 7468 6520 636f 6d6d 616e 6420 6c69 6e65  the command line
-000013a0: 3a0a 0a20 2020 6e6f 7365 7465 7374 7320  :..   nosetests 
-000013b0: 6f6e 6c79 5f74 6573 745f 7468 6973 2e70  only_test_this.p
-000013c0: 790a 0a54 6573 7420 6e61 6d65 7320 7370  y..Test names sp
-000013d0: 6563 6966 6965 6420 6d61 7920 6265 2066  ecified may be f
-000013e0: 696c 6520 6f72 206d 6f64 756c 6520 6e61  ile or module na
-000013f0: 6d65 732c 2061 6e64 206d 6179 206f 7074  mes, and may opt
-00001400: 696f 6e61 6c6c 790a 696e 6469 6361 7465  ionally.indicate
-00001410: 2074 6865 2074 6573 7420 6361 7365 2074   the test case t
-00001420: 6f20 7275 6e20 6279 2073 6570 6172 6174  o run by separat
-00001430: 696e 6720 7468 6520 6d6f 6475 6c65 206f  ing the module o
-00001440: 7220 6669 6c65 206e 616d 650a 6672 6f6d  r file name.from
-00001450: 2074 6865 2074 6573 7420 6361 7365 206e   the test case n
-00001460: 616d 6520 7769 7468 2061 2063 6f6c 6f6e  ame with a colon
-00001470: 2e20 4669 6c65 6e61 6d65 7320 6d61 7920  . Filenames may 
-00001480: 6265 2072 656c 6174 6976 6520 6f72 0a61  be relative or.a
-00001490: 6273 6f6c 7574 652e 2045 7861 6d70 6c65  bsolute. Example
-000014a0: 733a 0a0a 2020 206e 6f73 6574 6573 7473  s:..   nosetests
-000014b0: 2074 6573 742e 6d6f 6475 6c65 0a20 2020   test.module.   
-000014c0: 6e6f 7365 7465 7374 7320 616e 6f74 6865  nosetests anothe
-000014d0: 722e 7465 7374 3a54 6573 7443 6173 652e  r.test:TestCase.
-000014e0: 7465 7374 5f6d 6574 686f 640a 2020 206e  test_method.   n
-000014f0: 6f73 6574 6573 7473 2061 2e74 6573 743a  osetests a.test:
-00001500: 5465 7374 4361 7365 0a20 2020 6e6f 7365  TestCase.   nose
-00001510: 7465 7374 7320 2f70 6174 682f 746f 2f74  tests /path/to/t
-00001520: 6573 742f 6669 6c65 2e70 793a 7465 7374  est/file.py:test
-00001530: 5f66 756e 6374 696f 6e0a 0a59 6f75 206d  _function..You m
-00001540: 6179 2061 6c73 6f20 6368 616e 6765 2074  ay also change t
-00001550: 6865 2077 6f72 6b69 6e67 2064 6972 6563  he working direc
-00001560: 746f 7279 2077 6865 7265 206e 6f73 6520  tory where nose 
-00001570: 6c6f 6f6b 7320 666f 7220 7465 7374 730a  looks for tests.
-00001580: 6279 2075 7369 6e67 2074 6865 202d 7720  by using the -w 
-00001590: 7377 6974 6368 3a0a 0a20 2020 6e6f 7365  switch:..   nose
-000015a0: 7465 7374 7320 2d77 202f 7061 7468 2f74  tests -w /path/t
-000015b0: 6f2f 7465 7374 730a 0a4e 6f74 652c 2068  o/tests..Note, h
-000015c0: 6f77 6576 6572 2c20 7468 6174 2073 7570  owever, that sup
-000015d0: 706f 7274 2066 6f72 206d 756c 7469 706c  port for multipl
-000015e0: 6520 2d77 2061 7267 756d 656e 7473 2069  e -w arguments i
-000015f0: 7320 6e6f 770a 6465 7072 6563 6174 6564  s now.deprecated
-00001600: 2061 6e64 2077 696c 6c20 6265 2072 656d   and will be rem
-00001610: 6f76 6564 2069 6e20 6120 6675 7475 7265  oved in a future
-00001620: 2072 656c 6561 7365 2e20 4173 206f 6620   release. As of 
-00001630: 6e6f 7365 2030 2e31 302c 0a79 6f75 2063  nose 0.10,.you c
-00001640: 616e 2067 6574 2074 6865 2073 616d 6520  an get the same 
-00001650: 6265 6861 7669 6f72 2062 7920 7370 6563  behavior by spec
-00001660: 6966 7969 6e67 2074 6865 2074 6172 6765  ifying the targe
-00001670: 7420 6469 7265 6374 6f72 6965 730a 2a77  t directories.*w
-00001680: 6974 686f 7574 2a20 7468 6520 2d77 2073  ithout* the -w s
-00001690: 7769 7463 683a 0a0a 2020 206e 6f73 6574  witch:..   noset
-000016a0: 6573 7473 202f 7061 7468 2f74 6f2f 7465  ests /path/to/te
-000016b0: 7374 7320 2f61 6e6f 7468 6572 2f70 6174  sts /another/pat
-000016c0: 682f 746f 2f74 6573 7473 0a0a 4675 7274  h/to/tests..Furt
-000016d0: 6865 7220 6375 7374 6f6d 697a 6174 696f  her customizatio
-000016e0: 6e20 6f66 2074 6573 7420 7365 6c65 6374  n of test select
-000016f0: 696f 6e20 616e 6420 6c6f 6164 696e 6720  ion and loading 
-00001700: 6973 2070 6f73 7369 626c 650a 7468 726f  is possible.thro
-00001710: 7567 6820 7468 6520 7573 6520 6f66 2070  ugh the use of p
-00001720: 6c75 6769 6e73 2e0a 0a54 6573 7420 7265  lugins...Test re
-00001730: 7375 6c74 206f 7574 7075 7420 6973 2069  sult output is i
-00001740: 6465 6e74 6963 616c 2074 6f20 7468 6174  dentical to that
-00001750: 206f 6620 756e 6974 7465 7374 2c20 6578   of unittest, ex
-00001760: 6365 7074 2066 6f72 2074 6865 0a61 6464  cept for the.add
-00001770: 6974 696f 6e61 6c20 6665 6174 7572 6573  itional features
-00001780: 2028 6572 726f 7220 636c 6173 7365 732c   (error classes,
-00001790: 2061 6e64 2070 6c75 6769 6e2d 7375 7070   and plugin-supp
-000017a0: 6c69 6564 2066 6561 7475 7265 7320 7375  lied features su
-000017b0: 6368 0a61 7320 6f75 7470 7574 2063 6170  ch.as output cap
-000017c0: 7475 7265 2061 6e64 2061 7373 6572 7420  ture and assert 
-000017d0: 696e 7472 6f73 7065 6374 696f 6e29 2064  introspection) d
-000017e0: 6574 6169 6c65 6420 696e 2074 6865 206f  etailed in the o
-000017f0: 7074 696f 6e73 0a62 656c 6f77 2e0a 0a0a  ptions.below....
-00001800: 436f 6e66 6967 7572 6174 696f 6e0a 2d2d  Configuration.--
-00001810: 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a 0a49 6e20  -----------..In 
-00001820: 6164 6469 7469 6f6e 2074 6f20 7061 7373  addition to pass
-00001830: 696e 6720 636f 6d6d 616e 642d 6c69 6e65  ing command-line
-00001840: 206f 7074 696f 6e73 2c20 796f 7520 6d61   options, you ma
-00001850: 7920 616c 736f 2070 7574 0a63 6f6e 6669  y also put.confi
-00001860: 6775 7261 7469 6f6e 206f 7074 696f 6e73  guration options
-00001870: 2069 6e20 796f 7572 2070 726f 6a65 6374   in your project
-00001880: 202a 7365 7475 702e 6366 672a 2066 696c   *setup.cfg* fil
-00001890: 652c 206f 7220 6120 2e6e 6f73 6572 630a  e, or a .noserc.
-000018a0: 6f72 206e 6f73 652e 6366 6720 6669 6c65  or nose.cfg file
-000018b0: 2069 6e20 796f 7572 2068 6f6d 6520 6469   in your home di
-000018c0: 7265 6374 6f72 792e 2049 6e20 616e 7920  rectory. In any 
-000018d0: 6f66 2074 6865 7365 2073 7461 6e64 6172  of these standar
-000018e0: 6420 696e 692d 0a73 7479 6c65 2063 6f6e  d ini-.style con
-000018f0: 6669 6720 6669 6c65 732c 2079 6f75 2070  fig files, you p
-00001900: 7574 2079 6f75 7220 6e6f 7365 7465 7374  ut your nosetest
-00001910: 7320 636f 6e66 6967 7572 6174 696f 6e20  s configuration 
-00001920: 696e 2061 0a22 5b6e 6f73 6574 6573 7473  in a."[nosetests
-00001930: 5d22 2073 6563 7469 6f6e 2e20 4f70 7469  ]" section. Opti
-00001940: 6f6e 7320 6172 6520 7468 6520 7361 6d65  ons are the same
-00001950: 2061 7320 6f6e 2074 6865 2063 6f6d 6d61   as on the comma
-00001960: 6e64 206c 696e 652c 0a77 6974 6820 7468  nd line,.with th
-00001970: 6520 2d2d 2070 7265 6669 7820 7265 6d6f  e -- prefix remo
-00001980: 7665 642e 2046 6f72 206f 7074 696f 6e73  ved. For options
-00001990: 2074 6861 7420 6172 6520 7369 6d70 6c65   that are simple
-000019a0: 2073 7769 7463 6865 732c 2079 6f75 0a6d   switches, you.m
-000019b0: 7573 7420 7375 7070 6c79 2061 2076 616c  ust supply a val
-000019c0: 7565 3a0a 0a20 2020 5b6e 6f73 6574 6573  ue:..   [nosetes
-000019d0: 7473 5d0a 2020 2076 6572 626f 7369 7479  ts].   verbosity
-000019e0: 3d33 0a20 2020 7769 7468 2d64 6f63 7465  =3.   with-docte
-000019f0: 7374 3d31 0a0a 416c 6c20 636f 6e66 6967  st=1..All config
-00001a00: 7572 6174 696f 6e20 6669 6c65 7320 7468  uration files th
-00001a10: 6174 2061 7265 2066 6f75 6e64 2077 696c  at are found wil
-00001a20: 6c20 6265 206c 6f61 6465 6420 616e 6420  l be loaded and 
-00001a30: 7468 6569 720a 6f70 7469 6f6e 7320 636f  their.options co
-00001a40: 6d62 696e 6564 2e20 596f 7520 6361 6e20  mbined. You can 
-00001a50: 6f76 6572 7269 6465 2074 6865 2073 7461  override the sta
-00001a60: 6e64 6172 6420 636f 6e66 6967 2066 696c  ndard config fil
-00001a70: 6520 6c6f 6164 696e 670a 7769 7468 2074  e loading.with t
-00001a80: 6865 2022 2d63 2220 6f70 7469 6f6e 2e0a  he "-c" option..
-00001a90: 0a0a 5573 696e 6720 506c 7567 696e 730a  ..Using Plugins.
-00001aa0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a 0a54  -------------..T
-00001ab0: 6865 7265 2061 7265 206e 756d 6572 6f75  here are numerou
-00001ac0: 7320 6e6f 7365 2070 6c75 6769 6e73 2061  s nose plugins a
-00001ad0: 7661 696c 6162 6c65 2076 6961 2065 6173  vailable via eas
-00001ae0: 795f 696e 7374 616c 6c20 616e 640a 656c  y_install and.el
-00001af0: 7365 7768 6572 652e 2054 6f20 7573 6520  sewhere. To use 
-00001b00: 6120 706c 7567 696e 2c20 6a75 7374 2069  a plugin, just i
-00001b10: 6e73 7461 6c6c 2069 742e 2054 6865 2070  nstall it. The p
-00001b20: 6c75 6769 6e20 7769 6c6c 2061 6464 0a63  lugin will add.c
-00001b30: 6f6d 6d61 6e64 206c 696e 6520 6f70 7469  ommand line opti
-00001b40: 6f6e 7320 746f 206e 6f73 6574 6573 7473  ons to nosetests
-00001b50: 2e20 546f 2076 6572 6966 7920 7468 6174  . To verify that
-00001b60: 2074 6865 2070 6c75 6769 6e20 6973 0a69   the plugin is.i
-00001b70: 6e73 7461 6c6c 6564 2c20 7275 6e3a 0a0a  nstalled, run:..
-00001b80: 2020 206e 6f73 6574 6573 7473 202d 2d70     nosetests --p
-00001b90: 6c75 6769 6e73 0a0a 596f 7520 6361 6e20  lugins..You can 
-00001ba0: 6164 6420 2d76 206f 7220 2d76 7620 746f  add -v or -vv to
-00001bb0: 2074 6861 7420 636f 6d6d 616e 6420 746f   that command to
-00001bc0: 2073 686f 7720 6d6f 7265 2069 6e66 6f72   show more infor
-00001bd0: 6d61 7469 6f6e 2061 626f 7574 0a65 6163  mation about.eac
-00001be0: 6820 706c 7567 696e 2e0a 0a49 6620 796f  h plugin...If yo
-00001bf0: 7520 6172 6520 7275 6e6e 696e 6720 6e6f  u are running no
-00001c00: 7365 2e6d 6169 6e28 2920 6f72 206e 6f73  se.main() or nos
-00001c10: 652e 7275 6e28 2920 6672 6f6d 2061 2073  e.run() from a s
-00001c20: 6372 6970 742c 2079 6f75 2063 616e 0a73  cript, you can.s
-00001c30: 7065 6369 6679 2061 206c 6973 7420 6f66  pecify a list of
-00001c40: 2070 6c75 6769 6e73 2074 6f20 7573 6520   plugins to use 
-00001c50: 6279 2070 6173 7369 6e67 2061 206c 6973  by passing a lis
-00001c60: 7420 6f66 2070 6c75 6769 6e73 2077 6974  t of plugins wit
-00001c70: 6820 7468 650a 706c 7567 696e 7320 6b65  h the.plugins ke
-00001c80: 7977 6f72 6420 6172 6775 6d65 6e74 2e0a  yword argument..
-00001c90: 0a0a 4f70 7469 6f6e 730a 2d2d 2d2d 2d2d  ..Options.------
-00001ca0: 2d0a 0a2d 562c 202d 2d76 6572 7369 6f6e  -..-V, --version
-00001cb0: 0a0a 2020 204f 7574 7075 7420 6e6f 7365  ..   Output nose
-00001cc0: 2076 6572 7369 6f6e 2061 6e64 2065 7869   version and exi
-00001cd0: 740a 0a2d 702c 202d 2d70 6c75 6769 6e73  t..-p, --plugins
-00001ce0: 0a0a 2020 204f 7574 7075 7420 6c69 7374  ..   Output list
-00001cf0: 206f 6620 6176 6169 6c61 626c 6520 706c   of available pl
-00001d00: 7567 696e 7320 616e 6420 6578 6974 2e20  ugins and exit. 
-00001d10: 436f 6d62 696e 6520 7769 7468 2068 6967  Combine with hig
-00001d20: 6865 720a 2020 2076 6572 626f 7369 7479  her.   verbosity
-00001d30: 2066 6f72 2067 7265 6174 6572 2064 6574   for greater det
-00001d40: 6169 6c0a 0a2d 763d 4445 4641 554c 542c  ail..-v=DEFAULT,
-00001d50: 202d 2d76 6572 626f 7365 3d44 4546 4155   --verbose=DEFAU
-00001d60: 4c54 0a0a 2020 2042 6520 6d6f 7265 2076  LT..   Be more v
-00001d70: 6572 626f 7365 2e20 5b4e 4f53 455f 5645  erbose. [NOSE_VE
-00001d80: 5242 4f53 455d 0a0a 2d2d 7665 7262 6f73  RBOSE]..--verbos
-00001d90: 6974 793d 5645 5242 4f53 4954 590a 0a20  ity=VERBOSITY.. 
-00001da0: 2020 5365 7420 7665 7262 6f73 6974 793b    Set verbosity;
-00001db0: 202d 2d76 6572 626f 7369 7479 3d32 2069   --verbosity=2 i
-00001dc0: 7320 7468 6520 7361 6d65 2061 7320 2d76  s the same as -v
-00001dd0: 0a0a 2d71 3d44 4546 4155 4c54 2c20 2d2d  ..-q=DEFAULT, --
-00001de0: 7175 6965 743d 4445 4641 554c 540a 0a20  quiet=DEFAULT.. 
-00001df0: 2020 4265 206c 6573 7320 7665 7262 6f73    Be less verbos
-00001e00: 650a 0a2d 633d 4649 4c45 532c 202d 2d63  e..-c=FILES, --c
-00001e10: 6f6e 6669 673d 4649 4c45 530a 0a20 2020  onfig=FILES..   
-00001e20: 4c6f 6164 2063 6f6e 6669 6775 7261 7469  Load configurati
-00001e30: 6f6e 2066 726f 6d20 636f 6e66 6967 2066  on from config f
-00001e40: 696c 6528 7329 2e20 4d61 7920 6265 2073  ile(s). May be s
-00001e50: 7065 6369 6669 6564 206d 756c 7469 706c  pecified multipl
-00001e60: 650a 2020 2074 696d 6573 3b20 696e 2074  e.   times; in t
-00001e70: 6861 7420 6361 7365 2c20 616c 6c20 636f  hat case, all co
-00001e80: 6e66 6967 2066 696c 6573 2077 696c 6c20  nfig files will 
-00001e90: 6265 206c 6f61 6465 6420 616e 6420 636f  be loaded and co
-00001ea0: 6d62 696e 6564 0a0a 2d77 3d57 4845 5245  mbined..-w=WHERE
-00001eb0: 2c20 2d2d 7768 6572 653d 5748 4552 450a  , --where=WHERE.
-00001ec0: 0a20 2020 4c6f 6f6b 2066 6f72 2074 6573  .   Look for tes
-00001ed0: 7473 2069 6e20 7468 6973 2064 6972 6563  ts in this direc
-00001ee0: 746f 7279 2e20 4d61 7920 6265 2073 7065  tory. May be spe
-00001ef0: 6369 6669 6564 206d 756c 7469 706c 6520  cified multiple 
-00001f00: 7469 6d65 732e 0a20 2020 5468 6520 6669  times..   The fi
-00001f10: 7273 7420 6469 7265 6374 6f72 7920 7061  rst directory pa
-00001f20: 7373 6564 2077 696c 6c20 6265 2075 7365  ssed will be use
-00001f30: 6420 6173 2074 6865 2077 6f72 6b69 6e67  d as the working
-00001f40: 2064 6972 6563 746f 7279 2c0a 2020 2069   directory,.   i
-00001f50: 6e20 706c 6163 6520 6f66 2074 6865 2063  n place of the c
-00001f60: 7572 7265 6e74 2077 6f72 6b69 6e67 2064  urrent working d
-00001f70: 6972 6563 746f 7279 2c20 7768 6963 6820  irectory, which 
-00001f80: 6973 2074 6865 2064 6566 6175 6c74 2e0a  is the default..
-00001f90: 2020 204f 7468 6572 7320 7769 6c6c 2062     Others will b
-00001fa0: 6520 6164 6465 6420 746f 2074 6865 206c  e added to the l
-00001fb0: 6973 7420 6f66 2074 6573 7473 2074 6f20  ist of tests to 
-00001fc0: 6578 6563 7574 652e 205b 4e4f 5345 5f57  execute. [NOSE_W
-00001fd0: 4845 5245 5d0a 0a2d 2d70 7933 7768 6572  HERE]..--py3wher
-00001fe0: 653d 5059 3357 4845 5245 0a0a 2020 204c  e=PY3WHERE..   L
-00001ff0: 6f6f 6b20 666f 7220 7465 7374 7320 696e  ook for tests in
-00002000: 2074 6869 7320 6469 7265 6374 6f72 7920   this directory 
-00002010: 756e 6465 7220 5079 7468 6f6e 2033 2e78  under Python 3.x
-00002020: 2e20 4675 6e63 7469 6f6e 7320 7468 650a  . Functions the.
-00002030: 2020 2073 616d 6520 6173 2027 7768 6572     same as 'wher
-00002040: 6527 2c20 6275 7420 6f6e 6c79 2061 7070  e', but only app
-00002050: 6c69 6573 2069 6620 7275 6e6e 696e 6720  lies if running 
-00002060: 756e 6465 7220 5079 7468 6f6e 2033 2e78  under Python 3.x
-00002070: 206f 720a 2020 2061 626f 7665 2e20 204e   or.   above.  N
-00002080: 6f74 6520 7468 6174 2c20 6966 2070 7265  ote that, if pre
-00002090: 7365 6e74 2075 6e64 6572 2033 2e78 2c20  sent under 3.x, 
-000020a0: 7468 6973 206f 7074 696f 6e20 636f 6d70  this option comp
-000020b0: 6c65 7465 6c79 0a20 2020 7265 706c 6163  letely.   replac
-000020c0: 6573 2061 6e79 2064 6972 6563 746f 7269  es any directori
-000020d0: 6573 2073 7065 6369 6669 6564 2077 6974  es specified wit
-000020e0: 6820 2777 6865 7265 272c 2073 6f20 7468  h 'where', so th
-000020f0: 6520 2777 6865 7265 270a 2020 206f 7074  e 'where'.   opt
-00002100: 696f 6e20 6265 636f 6d65 7320 696e 6566  ion becomes inef
-00002110: 6665 6374 6976 652e 205b 4e4f 5345 5f50  fective. [NOSE_P
-00002120: 5933 5748 4552 455d 0a0a 2d6d 3d52 4547  Y3WHERE]..-m=REG
-00002130: 4558 2c20 2d2d 6d61 7463 683d 5245 4745  EX, --match=REGE
-00002140: 582c 202d 2d74 6573 746d 6174 6368 3d52  X, --testmatch=R
-00002150: 4547 4558 0a0a 2020 2046 696c 6573 2c20  EGEX..   Files, 
-00002160: 6469 7265 6374 6f72 6965 732c 2066 756e  directories, fun
-00002170: 6374 696f 6e20 6e61 6d65 732c 2061 6e64  ction names, and
-00002180: 2063 6c61 7373 206e 616d 6573 2074 6861   class names tha
-00002190: 7420 6d61 7463 6820 7468 6973 0a20 2020  t match this.   
-000021a0: 7265 6775 6c61 7220 6578 7072 6573 7369  regular expressi
-000021b0: 6f6e 2061 7265 2063 6f6e 7369 6465 7265  on are considere
-000021c0: 6420 7465 7374 732e 2020 4465 6661 756c  d tests.  Defaul
-000021d0: 743a 0a20 2020 283f 3a5e 7c5b 625f 2e2f  t:.   (?:^|[b_./
-000021e0: 2d5d 295b 5474 5d65 7374 205b 4e4f 5345  -])[Tt]est [NOSE
-000021f0: 5f54 4553 544d 4154 4348 5d0a 0a2d 2d74  _TESTMATCH]..--t
-00002200: 6573 7473 3d4e 414d 4553 0a0a 2020 2052  ests=NAMES..   R
-00002210: 756e 2074 6865 7365 2074 6573 7473 2028  un these tests (
-00002220: 636f 6d6d 612d 7365 7061 7261 7465 6420  comma-separated 
-00002230: 6c69 7374 292e 2054 6869 7320 6172 6775  list). This argu
-00002240: 6d65 6e74 2069 7320 7573 6566 756c 0a20  ment is useful. 
-00002250: 2020 6d61 696e 6c79 2066 726f 6d20 636f    mainly from co
-00002260: 6e66 6967 7572 6174 696f 6e20 6669 6c65  nfiguration file
-00002270: 733b 206f 6e20 7468 6520 636f 6d6d 616e  s; on the comman
-00002280: 6420 6c69 6e65 2c20 6a75 7374 2070 6173  d line, just pas
-00002290: 7320 7468 650a 2020 2074 6573 7473 2074  s the.   tests t
-000022a0: 6f20 7275 6e20 6173 2061 6464 6974 696f  o run as additio
-000022b0: 6e61 6c20 6172 6775 6d65 6e74 7320 7769  nal arguments wi
-000022c0: 7468 206e 6f20 7377 6974 6368 2e0a 0a2d  th no switch...-
-000022d0: 6c3d 4445 4641 554c 542c 202d 2d64 6562  l=DEFAULT, --deb
-000022e0: 7567 3d44 4546 4155 4c54 0a0a 2020 2041  ug=DEFAULT..   A
-000022f0: 6374 6976 6174 6520 6465 6275 6720 6c6f  ctivate debug lo
-00002300: 6767 696e 6720 666f 7220 6f6e 6520 6f72  gging for one or
-00002310: 206d 6f72 6520 7379 7374 656d 732e 2041   more systems. A
-00002320: 7661 696c 6162 6c65 2064 6562 7567 0a20  vailable debug. 
-00002330: 2020 6c6f 6767 6572 733a 206e 6f73 652c    loggers: nose,
-00002340: 206e 6f73 652e 696d 706f 7274 6572 2c20   nose.importer, 
-00002350: 6e6f 7365 2e69 6e73 7065 6374 6f72 2c20  nose.inspector, 
-00002360: 6e6f 7365 2e70 6c75 6769 6e73 2c0a 2020  nose.plugins,.  
-00002370: 206e 6f73 652e 7265 7375 6c74 2061 6e64   nose.result and
-00002380: 206e 6f73 652e 7365 6c65 6374 6f72 2e20   nose.selector. 
-00002390: 5365 7061 7261 7465 206d 756c 7469 706c  Separate multipl
-000023a0: 6520 6e61 6d65 7320 7769 7468 2061 0a20  e names with a. 
-000023b0: 2020 636f 6d6d 612e 0a0a 2d2d 6465 6275    comma...--debu
-000023c0: 672d 6c6f 673d 4649 4c45 0a0a 2020 204c  g-log=FILE..   L
-000023d0: 6f67 2064 6562 7567 206d 6573 7361 6765  og debug message
-000023e0: 7320 746f 2074 6869 7320 6669 6c65 2028  s to this file (
-000023f0: 6465 6661 756c 743a 2073 7973 2e73 7464  default: sys.std
-00002400: 6572 7229 0a0a 2d2d 6c6f 6767 696e 672d  err)..--logging-
-00002410: 636f 6e66 6967 3d46 494c 452c 202d 2d6c  config=FILE, --l
-00002420: 6f67 2d63 6f6e 6669 673d 4649 4c45 0a0a  og-config=FILE..
-00002430: 2020 204c 6f61 6420 6c6f 6767 696e 6720     Load logging 
-00002440: 636f 6e66 6967 2066 726f 6d20 7468 6973  config from this
-00002450: 2066 696c 6520 2d2d 2062 7970 6173 7365   file -- bypasse
-00002460: 7320 616c 6c20 6f74 6865 7220 6c6f 6767  s all other logg
-00002470: 696e 670a 2020 2063 6f6e 6669 6720 7365  ing.   config se
-00002480: 7474 696e 6773 2e0a 0a2d 493d 5245 4745  ttings...-I=REGE
-00002490: 582c 202d 2d69 676e 6f72 652d 6669 6c65  X, --ignore-file
-000024a0: 733d 5245 4745 580a 0a20 2020 436f 6d70  s=REGEX..   Comp
-000024b0: 6c65 7465 6c79 2069 676e 6f72 6520 616e  letely ignore an
-000024c0: 7920 6669 6c65 2074 6861 7420 6d61 7463  y file that matc
-000024d0: 6865 7320 7468 6973 2072 6567 756c 6172  hes this regular
-000024e0: 2065 7870 7265 7373 696f 6e2e 0a20 2020   expression..   
-000024f0: 5461 6b65 7320 7072 6563 6564 656e 6365  Takes precedence
-00002500: 206f 7665 7220 616e 7920 6f74 6865 7220   over any other 
-00002510: 7365 7474 696e 6773 206f 7220 706c 7567  settings or plug
-00002520: 696e 732e 2053 7065 6369 6679 696e 670a  ins. Specifying.
-00002530: 2020 2074 6869 7320 6f70 7469 6f6e 2077     this option w
-00002540: 696c 6c20 7265 706c 6163 6520 7468 6520  ill replace the 
-00002550: 6465 6661 756c 7420 7365 7474 696e 672e  default setting.
-00002560: 2053 7065 6369 6679 2074 6869 7320 6f70   Specify this op
-00002570: 7469 6f6e 0a20 2020 6d75 6c74 6970 6c65  tion.   multiple
-00002580: 2074 696d 6573 2074 6f20 6164 6420 6d6f   times to add mo
-00002590: 7265 2072 6567 756c 6172 2065 7870 7265  re regular expre
-000025a0: 7373 696f 6e73 205b 4e4f 5345 5f49 474e  ssions [NOSE_IGN
-000025b0: 4f52 455f 4649 4c45 535d 0a0a 2d65 3d52  ORE_FILES]..-e=R
-000025c0: 4547 4558 2c20 2d2d 6578 636c 7564 653d  EGEX, --exclude=
-000025d0: 5245 4745 580a 0a20 2020 446f 206e 6f74  REGEX..   Do not
-000025e0: 2072 756e 2074 6573 7473 2074 6861 7420   run tests that 
-000025f0: 6d61 7463 6820 7265 6775 6c61 7220 6578  match regular ex
-00002600: 7072 6573 7369 6f6e 205b 4e4f 5345 5f45  pression [NOSE_E
-00002610: 5843 4c55 4445 5d0a 0a2d 693d 5245 4745  XCLUDE]..-i=REGE
-00002620: 582c 202d 2d69 6e63 6c75 6465 3d52 4547  X, --include=REG
-00002630: 4558 0a0a 2020 2054 6869 7320 7265 6775  EX..   This regu
-00002640: 6c61 7220 6578 7072 6573 7369 6f6e 2077  lar expression w
-00002650: 696c 6c20 6265 2061 7070 6c69 6564 2074  ill be applied t
-00002660: 6f20 6669 6c65 732c 2064 6972 6563 746f  o files, directo
-00002670: 7269 6573 2c0a 2020 2066 756e 6374 696f  ries,.   functio
-00002680: 6e20 6e61 6d65 732c 2061 6e64 2063 6c61  n names, and cla
-00002690: 7373 206e 616d 6573 2066 6f72 2061 2063  ss names for a c
-000026a0: 6861 6e63 6520 746f 2069 6e63 6c75 6465  hance to include
-000026b0: 2061 6464 6974 696f 6e61 6c0a 2020 2074   additional.   t
-000026c0: 6573 7473 2074 6861 7420 646f 206e 6f74  ests that do not
-000026d0: 206d 6174 6368 2054 4553 544d 4154 4348   match TESTMATCH
-000026e0: 2e20 2053 7065 6369 6679 2074 6869 7320  .  Specify this 
-000026f0: 6f70 7469 6f6e 206d 756c 7469 706c 650a  option multiple.
-00002700: 2020 2074 696d 6573 2074 6f20 6164 6420     times to add 
-00002710: 6d6f 7265 2072 6567 756c 6172 2065 7870  more regular exp
-00002720: 7265 7373 696f 6e73 205b 4e4f 5345 5f49  ressions [NOSE_I
-00002730: 4e43 4c55 4445 5d0a 0a2d 782c 202d 2d73  NCLUDE]..-x, --s
-00002740: 746f 700a 0a20 2020 5374 6f70 2072 756e  top..   Stop run
-00002750: 6e69 6e67 2074 6573 7473 2061 6674 6572  ning tests after
-00002760: 2074 6865 2066 6972 7374 2065 7272 6f72   the first error
-00002770: 206f 7220 6661 696c 7572 650a 0a2d 502c   or failure..-P,
-00002780: 202d 2d6e 6f2d 7061 7468 2d61 646a 7573   --no-path-adjus
-00002790: 746d 656e 740a 0a20 2020 446f 206e 6f74  tment..   Do not
-000027a0: 206d 616b 6520 616e 7920 6368 616e 6765   make any change
-000027b0: 7320 746f 2073 7973 2e70 6174 6820 7768  s to sys.path wh
-000027c0: 656e 206c 6f61 6469 6e67 2074 6573 7473  en loading tests
-000027d0: 205b 4e4f 5345 5f4e 4f50 4154 485d 0a0a   [NOSE_NOPATH]..
-000027e0: 2d2d 6578 650a 0a20 2020 4c6f 6f6b 2066  --exe..   Look f
-000027f0: 6f72 2074 6573 7473 2069 6e20 7079 7468  or tests in pyth
-00002800: 6f6e 206d 6f64 756c 6573 2074 6861 7420  on modules that 
-00002810: 6172 6520 6578 6563 7574 6162 6c65 2e20  are executable. 
-00002820: 4e6f 726d 616c 0a20 2020 6265 6861 7669  Normal.   behavi
-00002830: 6f72 2069 7320 746f 2065 7863 6c75 6465  or is to exclude
-00002840: 2065 7865 6375 7461 626c 6520 6d6f 6475   executable modu
-00002850: 6c65 732c 2073 696e 6365 2074 6865 7920  les, since they 
-00002860: 6d61 7920 6e6f 7420 6265 0a20 2020 696d  may not be.   im
-00002870: 706f 7274 2d73 6166 6520 5b4e 4f53 455f  port-safe [NOSE_
-00002880: 494e 434c 5544 455f 4558 455d 0a0a 2d2d  INCLUDE_EXE]..--
-00002890: 6e6f 6578 650a 0a20 2020 444f 204e 4f54  noexe..   DO NOT
-000028a0: 206c 6f6f 6b20 666f 7220 7465 7374 7320   look for tests 
-000028b0: 696e 2070 7974 686f 6e20 6d6f 6475 6c65  in python module
-000028c0: 7320 7468 6174 2061 7265 2065 7865 6375  s that are execu
-000028d0: 7461 626c 652e 2028 5468 650a 2020 2064  table. (The.   d
-000028e0: 6566 6175 6c74 206f 6e20 7468 6520 7769  efault on the wi
-000028f0: 6e64 6f77 7320 706c 6174 666f 726d 2069  ndows platform i
-00002900: 7320 746f 2064 6f20 736f 2e29 0a0a 2d2d  s to do so.)..--
-00002910: 7472 6176 6572 7365 2d6e 616d 6573 7061  traverse-namespa
-00002920: 6365 0a0a 2020 2054 7261 7665 7273 6520  ce..   Traverse 
-00002930: 7468 726f 7567 6820 616c 6c20 7061 7468  through all path
-00002940: 2065 6e74 7269 6573 206f 6620 6120 6e61   entries of a na
-00002950: 6d65 7370 6163 6520 7061 636b 6167 650a  mespace package.
-00002960: 0a2d 2d66 6972 7374 2d70 6163 6b61 6765  .--first-package
-00002970: 2d77 696e 732c 202d 2d66 6972 7374 2d70  -wins, --first-p
-00002980: 6b67 2d77 696e 732c 202d 2d31 7374 2d70  kg-wins, --1st-p
-00002990: 6b67 2d77 696e 730a 0a20 2020 5468 6520  kg-wins..   The 
-000029a0: 6e6f 7365 2069 6d70 6f72 7465 7220 7769  nose importer wi
-000029b0: 6c6c 206e 6f72 6d61 6c6c 7920 6576 6963  ll normally evic
-000029c0: 7420 6120 7061 636b 6167 6520 6672 6f6d  t a package from
-000029d0: 2073 7973 2e6d 6f64 756c 6573 2069 660a   sys.modules if.
-000029e0: 2020 2069 7420 7365 6573 2061 2070 6163     it sees a pac
-000029f0: 6b61 6765 2077 6974 6820 7468 6520 7361  kage with the sa
-00002a00: 6d65 206e 616d 6520 696e 2061 2064 6966  me name in a dif
-00002a10: 6665 7265 6e74 206c 6f63 6174 696f 6e2e  ferent location.
-00002a20: 2053 6574 0a20 2020 7468 6973 206f 7074   Set.   this opt
-00002a30: 696f 6e20 746f 2064 6973 6162 6c65 2074  ion to disable t
-00002a40: 6861 7420 6265 6861 7669 6f72 2e0a 0a2d  hat behavior...-
-00002a50: 2d6e 6f2d 6279 7465 2d63 6f6d 7069 6c65  -no-byte-compile
-00002a60: 0a0a 2020 2050 7265 7665 6e74 206e 6f73  ..   Prevent nos
-00002a70: 6520 6672 6f6d 2062 7974 652d 636f 6d70  e from byte-comp
-00002a80: 696c 696e 6720 7468 6520 736f 7572 6365  iling the source
-00002a90: 2069 6e74 6f20 2e70 7963 2066 696c 6573   into .pyc files
-00002aa0: 2077 6869 6c65 0a20 2020 6e6f 7365 2069   while.   nose i
-00002ab0: 7320 7363 616e 6e69 6e67 2066 6f72 2061  s scanning for a
-00002ac0: 6e64 2072 756e 6e69 6e67 2074 6573 7473  nd running tests
-00002ad0: 2e0a 0a2d 613d 4154 5452 2c20 2d2d 6174  ...-a=ATTR, --at
-00002ae0: 7472 3d41 5454 520a 0a20 2020 5275 6e20  tr=ATTR..   Run 
-00002af0: 6f6e 6c79 2074 6573 7473 2074 6861 7420  only tests that 
-00002b00: 6861 7665 2061 7474 7269 6275 7465 7320  have attributes 
-00002b10: 7370 6563 6966 6965 6420 6279 2041 5454  specified by ATT
-00002b20: 5220 5b4e 4f53 455f 4154 5452 5d0a 0a2d  R [NOSE_ATTR]..-
-00002b30: 413d 4558 5052 2c20 2d2d 6576 616c 2d61  A=EXPR, --eval-a
-00002b40: 7474 723d 4558 5052 0a0a 2020 2052 756e  ttr=EXPR..   Run
-00002b50: 206f 6e6c 7920 7465 7374 7320 666f 7220   only tests for 
-00002b60: 7768 6f73 6520 6174 7472 6962 7574 6573  whose attributes
-00002b70: 2074 6865 2050 7974 686f 6e20 6578 7072   the Python expr
-00002b80: 6573 7369 6f6e 2045 5850 520a 2020 2065  ession EXPR.   e
-00002b90: 7661 6c75 6174 6573 2074 6f20 5472 7565  valuates to True
-00002ba0: 205b 4e4f 5345 5f45 5641 4c5f 4154 5452   [NOSE_EVAL_ATTR
-00002bb0: 5d0a 0a2d 732c 202d 2d6e 6f63 6170 7475  ]..-s, --nocaptu
-00002bc0: 7265 0a0a 2020 2044 6f20 6e6f 7420 6361  re..   Do not ca
-00002bd0: 7074 7572 6520 7374 646f 7574 2028 616e  pture stdout (an
-00002be0: 7920 7374 646f 7574 206f 7574 7075 7420  y stdout output 
-00002bf0: 7769 6c6c 2062 6520 7072 696e 7465 640a  will be printed.
-00002c00: 2020 2069 6d6d 6564 6961 7465 6c79 2920     immediately) 
-00002c10: 5b4e 4f53 455f 4e4f 4341 5054 5552 455d  [NOSE_NOCAPTURE]
-00002c20: 0a0a 2d2d 6e6f 6c6f 6763 6170 7475 7265  ..--nologcapture
-00002c30: 0a0a 2020 2044 6973 6162 6c65 206c 6f67  ..   Disable log
-00002c40: 6769 6e67 2063 6170 7475 7265 2070 6c75  ging capture plu
-00002c50: 6769 6e2e 204c 6f67 6769 6e67 2063 6f6e  gin. Logging con
-00002c60: 6669 6775 7261 7469 6f6e 2077 696c 6c20  figuration will 
-00002c70: 6265 206c 6566 740a 2020 2069 6e74 6163  be left.   intac
-00002c80: 742e 205b 4e4f 5345 5f4e 4f4c 4f47 4341  t. [NOSE_NOLOGCA
-00002c90: 5054 5552 455d 0a0a 2d2d 6c6f 6767 696e  PTURE]..--loggin
-00002ca0: 672d 666f 726d 6174 3d46 4f52 4d41 540a  g-format=FORMAT.
-00002cb0: 0a20 2020 5370 6563 6966 7920 6375 7374  .   Specify cust
-00002cc0: 6f6d 2066 6f72 6d61 7420 746f 2070 7269  om format to pri
-00002cd0: 6e74 2073 7461 7465 6d65 6e74 732e 2055  nt statements. U
-00002ce0: 7365 7320 7468 6520 7361 6d65 2066 6f72  ses the same for
-00002cf0: 6d61 7420 6173 0a20 2020 7573 6564 2062  mat as.   used b
-00002d00: 7920 7374 616e 6461 7264 206c 6f67 6769  y standard loggi
-00002d10: 6e67 2068 616e 646c 6572 732e 205b 4e4f  ng handlers. [NO
-00002d20: 5345 5f4c 4f47 464f 524d 4154 5d0a 0a2d  SE_LOGFORMAT]..-
-00002d30: 2d6c 6f67 6769 6e67 2d64 6174 6566 6d74  -logging-datefmt
-00002d40: 3d46 4f52 4d41 540a 0a20 2020 5370 6563  =FORMAT..   Spec
-00002d50: 6966 7920 6375 7374 6f6d 2064 6174 652f  ify custom date/
-00002d60: 7469 6d65 2066 6f72 6d61 7420 746f 2070  time format to p
-00002d70: 7269 6e74 2073 7461 7465 6d65 6e74 732e  rint statements.
-00002d80: 2055 7365 7320 7468 6520 7361 6d65 0a20   Uses the same. 
-00002d90: 2020 666f 726d 6174 2061 7320 7573 6564    format as used
-00002da0: 2062 7920 7374 616e 6461 7264 206c 6f67   by standard log
-00002db0: 6769 6e67 2068 616e 646c 6572 732e 205b  ging handlers. [
-00002dc0: 4e4f 5345 5f4c 4f47 4441 5445 464d 545d  NOSE_LOGDATEFMT]
-00002dd0: 0a0a 2d2d 6c6f 6767 696e 672d 6669 6c74  ..--logging-filt
-00002de0: 6572 3d46 494c 5445 520a 0a20 2020 5370  er=FILTER..   Sp
-00002df0: 6563 6966 7920 7768 6963 6820 7374 6174  ecify which stat
-00002e00: 656d 656e 7473 2074 6f20 6669 6c74 6572  ements to filter
-00002e10: 2069 6e2f 6f75 742e 2042 7920 6465 6661   in/out. By defa
-00002e20: 756c 742c 2065 7665 7279 7468 696e 670a  ult, everything.
-00002e30: 2020 2069 7320 6361 7074 7572 6564 2e20     is captured. 
-00002e40: 4966 2074 6865 206f 7574 7075 7420 6973  If the output is
-00002e50: 2074 6f6f 2076 6572 626f 7365 2c20 7573   too verbose, us
-00002e60: 6520 7468 6973 206f 7074 696f 6e20 746f  e this option to
-00002e70: 0a20 2020 6669 6c74 6572 206f 7574 206e  .   filter out n
-00002e80: 6565 646c 6573 7320 6f75 7470 7574 2e20  eedless output. 
-00002e90: 4578 616d 706c 653a 2066 696c 7465 723d  Example: filter=
-00002ea0: 666f 6f20 7769 6c6c 2063 6170 7475 7265  foo will capture
-00002eb0: 0a20 2020 7374 6174 656d 656e 7473 2069  .   statements i
-00002ec0: 7373 7565 6420 4f4e 4c59 2074 6f20 2066  ssued ONLY to  f
-00002ed0: 6f6f 206f 7220 666f 6f2e 7768 6174 2e65  oo or foo.what.e
-00002ee0: 7665 722e 7375 6220 6275 7420 6e6f 7420  ver.sub but not 
-00002ef0: 666f 6f62 6172 0a20 2020 6f72 206f 7468  foobar.   or oth
-00002f00: 6572 206c 6f67 6765 722e 2053 7065 6369  er logger. Speci
-00002f10: 6679 206d 756c 7469 706c 6520 6c6f 6767  fy multiple logg
-00002f20: 6572 7320 7769 7468 2063 6f6d 6d61 3a0a  ers with comma:.
-00002f30: 2020 2066 696c 7465 723d 666f 6f2c 6261     filter=foo,ba
-00002f40: 722c 6261 7a2e 2049 6620 616e 7920 6c6f  r,baz. If any lo
-00002f50: 6767 6572 206e 616d 6520 6973 2070 7265  gger name is pre
-00002f60: 6669 7865 6420 7769 7468 2061 206d 696e  fixed with a min
-00002f70: 7573 2c20 6567 0a20 2020 6669 6c74 6572  us, eg.   filter
-00002f80: 3d2d 666f 6f2c 2069 7420 7769 6c6c 2062  =-foo, it will b
-00002f90: 6520 6578 636c 7564 6564 2072 6174 6865  e excluded rathe
-00002fa0: 7220 7468 616e 2069 6e63 6c75 6465 642e  r than included.
-00002fb0: 2044 6566 6175 6c74 3a0a 2020 2065 7863   Default:.   exc
-00002fc0: 6c75 6465 206c 6f67 6769 6e67 206d 6573  lude logging mes
-00002fd0: 7361 6765 7320 6672 6f6d 206e 6f73 6520  sages from nose 
-00002fe0: 6974 7365 6c66 2028 2d6e 6f73 6529 2e20  itself (-nose). 
-00002ff0: 5b4e 4f53 455f 4c4f 4746 494c 5445 525d  [NOSE_LOGFILTER]
-00003000: 0a0a 2d2d 6c6f 6767 696e 672d 636c 6561  ..--logging-clea
-00003010: 722d 6861 6e64 6c65 7273 0a0a 2020 2043  r-handlers..   C
-00003020: 6c65 6172 2061 6c6c 206f 7468 6572 206c  lear all other l
-00003030: 6f67 6769 6e67 2068 616e 646c 6572 730a  ogging handlers.
-00003040: 0a2d 2d6c 6f67 6769 6e67 2d6c 6576 656c  .--logging-level
-00003050: 3d44 4546 4155 4c54 0a0a 2020 2053 6574  =DEFAULT..   Set
-00003060: 2074 6865 206c 6f67 206c 6576 656c 2074   the log level t
-00003070: 6f20 6361 7074 7572 650a 0a2d 2d77 6974  o capture..--wit
-00003080: 682d 636f 7665 7261 6765 0a0a 2020 2045  h-coverage..   E
-00003090: 6e61 626c 6520 706c 7567 696e 2043 6f76  nable plugin Cov
-000030a0: 6572 6167 653a 2041 6374 6976 6174 6520  erage: Activate 
-000030b0: 6120 636f 7665 7261 6765 2072 6570 6f72  a coverage repor
-000030c0: 7420 7573 696e 6720 7468 650a 2020 204e  t using the.   N
-000030d0: 6564 2042 6174 6368 656c 6465 7220 636f  ed Batchelder co
-000030e0: 7665 7261 6765 206d 6f64 756c 652e 205b  verage module. [
-000030f0: 4e4f 5345 5f57 4954 485f 434f 5645 5241  NOSE_WITH_COVERA
-00003100: 4745 5d0a 0a2d 2d63 6f76 6572 2d70 6163  GE]..--cover-pac
-00003110: 6b61 6765 3d50 4143 4b41 4745 0a0a 2020  kage=PACKAGE..  
-00003120: 2052 6573 7472 6963 7420 636f 7665 7261   Restrict covera
-00003130: 6765 206f 7574 7075 7420 746f 2073 656c  ge output to sel
-00003140: 6563 7465 6420 7061 636b 6167 6573 205b  ected packages [
-00003150: 4e4f 5345 5f43 4f56 4552 5f50 4143 4b41  NOSE_COVER_PACKA
-00003160: 4745 5d0a 0a2d 2d63 6f76 6572 2d65 7261  GE]..--cover-era
-00003170: 7365 0a0a 2020 2045 7261 7365 2070 7265  se..   Erase pre
-00003180: 7669 6f75 736c 7920 636f 6c6c 6563 7465  viously collecte
-00003190: 6420 636f 7665 7261 6765 2073 7461 7469  d coverage stati
-000031a0: 7374 6963 7320 6265 666f 7265 2072 756e  stics before run
-000031b0: 0a0a 2d2d 636f 7665 722d 7465 7374 730a  ..--cover-tests.
-000031c0: 0a20 2020 496e 636c 7564 6520 7465 7374  .   Include test
-000031d0: 206d 6f64 756c 6573 2069 6e20 636f 7665   modules in cove
-000031e0: 7261 6765 2072 6570 6f72 7420 5b4e 4f53  rage report [NOS
-000031f0: 455f 434f 5645 525f 5445 5354 535d 0a0a  E_COVER_TESTS]..
-00003200: 2d2d 636f 7665 722d 6d69 6e2d 7065 7263  --cover-min-perc
-00003210: 656e 7461 6765 3d44 4546 4155 4c54 0a0a  entage=DEFAULT..
-00003220: 2020 204d 696e 696d 756d 2070 6572 6365     Minimum perce
-00003230: 6e74 6167 6520 6f66 2063 6f76 6572 6167  ntage of coverag
-00003240: 6520 666f 7220 7465 7374 7320 746f 2070  e for tests to p
-00003250: 6173 730a 2020 205b 4e4f 5345 5f43 4f56  ass.   [NOSE_COV
-00003260: 4552 5f4d 494e 5f50 4552 4345 4e54 4147  ER_MIN_PERCENTAG
-00003270: 455d 0a0a 2d2d 636f 7665 722d 696e 636c  E]..--cover-incl
-00003280: 7573 6976 650a 0a20 2020 496e 636c 7564  usive..   Includ
-00003290: 6520 616c 6c20 7079 7468 6f6e 2066 696c  e all python fil
-000032a0: 6573 2075 6e64 6572 2077 6f72 6b69 6e67  es under working
-000032b0: 2064 6972 6563 746f 7279 2069 6e20 636f   directory in co
-000032c0: 7665 7261 6765 0a20 2020 7265 706f 7274  verage.   report
-000032d0: 2e20 2055 7365 6675 6c20 666f 7220 6469  .  Useful for di
-000032e0: 7363 6f76 6572 696e 6720 686f 6c65 7320  scovering holes 
-000032f0: 696e 2074 6573 7420 636f 7665 7261 6765  in test coverage
-00003300: 2069 6620 6e6f 7420 616c 6c0a 2020 2066   if not all.   f
-00003310: 696c 6573 2061 7265 2069 6d70 6f72 7465  iles are importe
-00003320: 6420 6279 2074 6865 2074 6573 7420 7375  d by the test su
-00003330: 6974 652e 205b 4e4f 5345 5f43 4f56 4552  ite. [NOSE_COVER
-00003340: 5f49 4e43 4c55 5349 5645 5d0a 0a2d 2d63  _INCLUSIVE]..--c
-00003350: 6f76 6572 2d68 746d 6c0a 0a20 2020 5072  over-html..   Pr
-00003360: 6f64 7563 6520 4854 4d4c 2063 6f76 6572  oduce HTML cover
-00003370: 6167 6520 696e 666f 726d 6174 696f 6e0a  age information.
-00003380: 0a2d 2d63 6f76 6572 2d68 746d 6c2d 6469  .--cover-html-di
-00003390: 723d 4449 520a 0a20 2020 5072 6f64 7563  r=DIR..   Produc
-000033a0: 6520 4854 4d4c 2063 6f76 6572 6167 6520  e HTML coverage 
-000033b0: 696e 666f 726d 6174 696f 6e20 696e 2064  information in d
-000033c0: 6972 0a0a 2d2d 636f 7665 722d 6272 616e  ir..--cover-bran
-000033d0: 6368 6573 0a0a 2020 2049 6e63 6c75 6465  ches..   Include
-000033e0: 2062 7261 6e63 6820 636f 7665 7261 6765   branch coverage
-000033f0: 2069 6e20 636f 7665 7261 6765 2072 6570   in coverage rep
-00003400: 6f72 7420 5b4e 4f53 455f 434f 5645 525f  ort [NOSE_COVER_
-00003410: 4252 414e 4348 4553 5d0a 0a2d 2d63 6f76  BRANCHES]..--cov
-00003420: 6572 2d78 6d6c 0a0a 2020 2050 726f 6475  er-xml..   Produ
-00003430: 6365 2058 4d4c 2063 6f76 6572 6167 6520  ce XML coverage 
-00003440: 696e 666f 726d 6174 696f 6e0a 0a2d 2d63  information..--c
-00003450: 6f76 6572 2d78 6d6c 2d66 696c 653d 4649  over-xml-file=FI
-00003460: 4c45 0a0a 2020 2050 726f 6475 6365 2058  LE..   Produce X
-00003470: 4d4c 2063 6f76 6572 6167 6520 696e 666f  ML coverage info
-00003480: 726d 6174 696f 6e20 696e 2066 696c 650a  rmation in file.
-00003490: 0a2d 2d70 6462 0a0a 2020 2044 726f 7020  .--pdb..   Drop 
-000034a0: 696e 746f 2064 6562 7567 6765 7220 6f6e  into debugger on
-000034b0: 2066 6169 6c75 7265 7320 6f72 2065 7272   failures or err
-000034c0: 6f72 730a 0a2d 2d70 6462 2d66 6169 6c75  ors..--pdb-failu
-000034d0: 7265 730a 0a20 2020 4472 6f70 2069 6e74  res..   Drop int
-000034e0: 6f20 6465 6275 6767 6572 206f 6e20 6661  o debugger on fa
-000034f0: 696c 7572 6573 0a0a 2d2d 7064 622d 6572  ilures..--pdb-er
-00003500: 726f 7273 0a0a 2020 2044 726f 7020 696e  rors..   Drop in
-00003510: 746f 2064 6562 7567 6765 7220 6f6e 2065  to debugger on e
-00003520: 7272 6f72 730a 0a2d 2d6e 6f2d 6465 7072  rrors..--no-depr
-00003530: 6563 6174 6564 0a0a 2020 2044 6973 6162  ecated..   Disab
-00003540: 6c65 2073 7065 6369 616c 2068 616e 646c  le special handl
-00003550: 696e 6720 6f66 2044 6570 7265 6361 7465  ing of Deprecate
-00003560: 6454 6573 7420 6578 6365 7074 696f 6e73  dTest exceptions
-00003570: 2e0a 0a2d 2d77 6974 682d 646f 6374 6573  ...--with-doctes
-00003580: 740a 0a20 2020 456e 6162 6c65 2070 6c75  t..   Enable plu
-00003590: 6769 6e20 446f 6374 6573 743a 2041 6374  gin Doctest: Act
-000035a0: 6976 6174 6520 646f 6374 6573 7420 706c  ivate doctest pl
-000035b0: 7567 696e 2074 6f20 6669 6e64 2061 6e64  ugin to find and
-000035c0: 2072 756e 0a20 2020 646f 6374 6573 7473   run.   doctests
-000035d0: 2069 6e20 6e6f 6e2d 7465 7374 206d 6f64   in non-test mod
-000035e0: 756c 6573 2e20 5b4e 4f53 455f 5749 5448  ules. [NOSE_WITH
-000035f0: 5f44 4f43 5445 5354 5d0a 0a2d 2d64 6f63  _DOCTEST]..--doc
-00003600: 7465 7374 2d74 6573 7473 0a0a 2020 2041  test-tests..   A
-00003610: 6c73 6f20 6c6f 6f6b 2066 6f72 2064 6f63  lso look for doc
-00003620: 7465 7374 7320 696e 2074 6573 7420 6d6f  tests in test mo
-00003630: 6475 6c65 732e 204e 6f74 6520 7468 6174  dules. Note that
-00003640: 2063 6c61 7373 6573 2c20 6d65 7468 6f64   classes, method
-00003650: 730a 2020 2061 6e64 2066 756e 6374 696f  s.   and functio
-00003660: 6e73 2073 686f 756c 6420 6861 7665 2065  ns should have e
-00003670: 6974 6865 7220 646f 6374 6573 7473 206f  ither doctests o
-00003680: 7220 6e6f 6e2d 646f 6374 6573 7420 7465  r non-doctest te
-00003690: 7374 732c 206e 6f74 0a20 2020 626f 7468  sts, not.   both
-000036a0: 2e20 5b4e 4f53 455f 444f 4354 4553 545f  . [NOSE_DOCTEST_
-000036b0: 5445 5354 535d 0a0a 2d2d 646f 6374 6573  TESTS]..--doctes
-000036c0: 742d 6578 7465 6e73 696f 6e3d 4558 540a  t-extension=EXT.
-000036d0: 0a20 2020 416c 736f 206c 6f6f 6b20 666f  .   Also look fo
-000036e0: 7220 646f 6374 6573 7473 2069 6e20 6669  r doctests in fi
-000036f0: 6c65 7320 7769 7468 2074 6869 7320 6578  les with this ex
-00003700: 7465 6e73 696f 6e0a 2020 205b 4e4f 5345  tension.   [NOSE
-00003710: 5f44 4f43 5445 5354 5f45 5854 454e 5349  _DOCTEST_EXTENSI
-00003720: 4f4e 5d0a 0a2d 2d64 6f63 7465 7374 2d72  ON]..--doctest-r
-00003730: 6573 756c 742d 7661 7269 6162 6c65 3d56  esult-variable=V
-00003740: 4152 0a0a 2020 2043 6861 6e67 6520 7468  AR..   Change th
-00003750: 6520 7661 7269 6162 6c65 206e 616d 6520  e variable name 
-00003760: 7365 7420 746f 2074 6865 2072 6573 756c  set to the resul
-00003770: 7420 6f66 2074 6865 206c 6173 7420 696e  t of the last in
-00003780: 7465 7270 7265 7465 720a 2020 2063 6f6d  terpreter.   com
-00003790: 6d61 6e64 2066 726f 6d20 7468 6520 6465  mand from the de
-000037a0: 6661 756c 7420 275f 272e 2043 616e 2062  fault '_'. Can b
-000037b0: 6520 7573 6564 2074 6f20 6176 6f69 6420  e used to avoid 
-000037c0: 636f 6e66 6c69 6374 7320 7769 7468 0a20  conflicts with. 
-000037d0: 2020 7468 6520 5f28 2920 6675 6e63 7469    the _() functi
-000037e0: 6f6e 2075 7365 6420 666f 7220 7465 7874  on used for text
-000037f0: 2074 7261 6e73 6c61 7469 6f6e 2e0a 2020   translation..  
-00003800: 205b 4e4f 5345 5f44 4f43 5445 5354 5f52   [NOSE_DOCTEST_R
-00003810: 4553 554c 545f 5641 525d 0a0a 2d2d 646f  ESULT_VAR]..--do
-00003820: 6374 6573 742d 6669 7874 7572 6573 3d53  ctest-fixtures=S
-00003830: 5546 4649 580a 0a20 2020 4669 6e64 2066  UFFIX..   Find f
-00003840: 6978 7475 7265 7320 666f 7220 6120 646f  ixtures for a do
-00003850: 6374 6573 7420 6669 6c65 2069 6e20 6d6f  ctest file in mo
-00003860: 6475 6c65 2077 6974 6820 7468 6973 206e  dule with this n
-00003870: 616d 6520 6170 7065 6e64 6564 0a20 2020  ame appended.   
-00003880: 746f 2074 6865 2062 6173 6520 6e61 6d65  to the base name
-00003890: 206f 6620 7468 6520 646f 6374 6573 7420   of the doctest 
-000038a0: 6669 6c65 0a0a 2d2d 646f 6374 6573 742d  file..--doctest-
-000038b0: 6f70 7469 6f6e 733d 4f50 5449 4f4e 530a  options=OPTIONS.
-000038c0: 0a20 2020 5370 6563 6966 7920 6f70 7469  .   Specify opti
-000038d0: 6f6e 7320 746f 2070 6173 7320 746f 2064  ons to pass to d
-000038e0: 6f63 7465 7374 2e20 4567 2e0a 2020 2027  octest. Eg..   '
-000038f0: 2b45 4c4c 4950 5349 532c 2b4e 4f52 4d41  +ELLIPSIS,+NORMA
-00003900: 4c49 5a45 5f57 4849 5445 5350 4143 4527  LIZE_WHITESPACE'
-00003910: 0a0a 2d2d 7769 7468 2d69 736f 6c61 7469  ..--with-isolati
-00003920: 6f6e 0a0a 2020 2045 6e61 626c 6520 706c  on..   Enable pl
-00003930: 7567 696e 2049 736f 6c61 7469 6f6e 506c  ugin IsolationPl
-00003940: 7567 696e 3a20 4163 7469 7661 7465 2074  ugin: Activate t
-00003950: 6865 2069 736f 6c61 7469 6f6e 2070 6c75  he isolation plu
-00003960: 6769 6e20 746f 0a20 2020 6973 6f6c 6174  gin to.   isolat
-00003970: 6520 6368 616e 6765 7320 746f 2065 7874  e changes to ext
-00003980: 6572 6e61 6c20 6d6f 6475 6c65 7320 746f  ernal modules to
-00003990: 2061 2073 696e 676c 6520 7465 7374 206d   a single test m
-000039a0: 6f64 756c 6520 6f72 0a20 2020 7061 636b  odule or.   pack
-000039b0: 6167 652e 2054 6865 2069 736f 6c61 7469  age. The isolati
-000039c0: 6f6e 2070 6c75 6769 6e20 7265 7365 7473  on plugin resets
-000039d0: 2074 6865 2063 6f6e 7465 6e74 7320 6f66   the contents of
-000039e0: 2073 7973 2e6d 6f64 756c 6573 0a20 2020   sys.modules.   
-000039f0: 6166 7465 7220 6561 6368 2074 6573 7420  after each test 
-00003a00: 6d6f 6475 6c65 206f 7220 7061 636b 6167  module or packag
-00003a10: 6520 7275 6e73 2074 6f20 6974 7320 7374  e runs to its st
-00003a20: 6174 6520 6265 666f 7265 2074 6865 0a20  ate before the. 
-00003a30: 2020 7465 7374 2e20 504c 4541 5345 204e    test. PLEASE N
-00003a40: 4f54 4520 7468 6174 2074 6869 7320 706c  OTE that this pl
-00003a50: 7567 696e 2073 686f 756c 6420 6e6f 7420  ugin should not 
-00003a60: 6265 2075 7365 6420 7769 7468 2074 6865  be used with the
-00003a70: 0a20 2020 636f 7665 7261 6765 2070 6c75  .   coverage plu
-00003a80: 6769 6e2c 206f 7220 696e 2061 6e79 206f  gin, or in any o
-00003a90: 7468 6572 2063 6173 6520 7768 6572 6520  ther case where 
-00003aa0: 6d6f 6475 6c65 2072 656c 6f61 6469 6e67  module reloading
-00003ab0: 206d 6179 0a20 2020 7072 6f64 7563 6520   may.   produce 
-00003ac0: 756e 6465 7369 7261 626c 6520 7369 6465  undesirable side
-00003ad0: 2d65 6666 6563 7473 2e20 5b4e 4f53 455f  -effects. [NOSE_
-00003ae0: 5749 5448 5f49 534f 4c41 5449 4f4e 5d0a  WITH_ISOLATION].
-00003af0: 0a2d 642c 202d 2d64 6574 6169 6c65 642d  .-d, --detailed-
-00003b00: 6572 726f 7273 2c20 2d2d 6661 696c 7572  errors, --failur
-00003b10: 652d 6465 7461 696c 0a0a 2020 2041 6464  e-detail..   Add
-00003b20: 2064 6574 6169 6c20 746f 2065 7272 6f72   detail to error
-00003b30: 206f 7574 7075 7420 6279 2061 7474 656d   output by attem
-00003b40: 7074 696e 6720 746f 2065 7661 6c75 6174  pting to evaluat
-00003b50: 6520 6661 696c 6564 2061 7373 6572 7473  e failed asserts
-00003b60: 0a20 2020 5b4e 4f53 455f 4445 5441 494c  .   [NOSE_DETAIL
-00003b70: 4544 5f45 5252 4f52 535d 0a0a 2d2d 6e6f  ED_ERRORS]..--no
-00003b80: 2d73 6b69 700a 0a20 2020 4469 7361 626c  -skip..   Disabl
-00003b90: 6520 7370 6563 6961 6c20 6861 6e64 6c69  e special handli
-00003ba0: 6e67 206f 6620 536b 6970 5465 7374 2065  ng of SkipTest e
-00003bb0: 7863 6570 7469 6f6e 732e 0a0a 2d2d 7769  xceptions...--wi
-00003bc0: 7468 2d69 640a 0a20 2020 456e 6162 6c65  th-id..   Enable
-00003bd0: 2070 6c75 6769 6e20 5465 7374 4964 3a20   plugin TestId: 
-00003be0: 4163 7469 7661 7465 2074 6f20 6164 6420  Activate to add 
-00003bf0: 6120 7465 7374 2069 6420 286c 696b 6520  a test id (like 
-00003c00: 2331 2920 746f 2065 6163 680a 2020 2074  #1) to each.   t
-00003c10: 6573 7420 6e61 6d65 206f 7574 7075 742e  est name output.
-00003c20: 2041 6374 6976 6174 6520 7769 7468 202d   Activate with -
-00003c30: 2d66 6169 6c65 6420 746f 2072 6572 756e  -failed to rerun
-00003c40: 2066 6169 6c69 6e67 2074 6573 7473 0a20   failing tests. 
-00003c50: 2020 6f6e 6c79 2e20 5b4e 4f53 455f 5749    only. [NOSE_WI
-00003c60: 5448 5f49 445d 0a0a 2d2d 6964 2d66 696c  TH_ID]..--id-fil
-00003c70: 653d 4649 4c45 0a0a 2020 2053 746f 7265  e=FILE..   Store
-00003c80: 2074 6573 7420 6964 7320 666f 756e 6420   test ids found 
-00003c90: 696e 2074 6573 7420 7275 6e73 2069 6e20  in test runs in 
-00003ca0: 7468 6973 2066 696c 652e 2044 6566 6175  this file. Defau
-00003cb0: 6c74 2069 7320 7468 6520 6669 6c65 0a20  lt is the file. 
-00003cc0: 2020 2e6e 6f73 6569 6473 2069 6e20 7468    .noseids in th
-00003cd0: 6520 776f 726b 696e 6720 6469 7265 6374  e working direct
-00003ce0: 6f72 792e 0a0a 2d2d 6661 696c 6564 0a0a  ory...--failed..
-00003cf0: 2020 2052 756e 2074 6865 2074 6573 7473     Run the tests
-00003d00: 2074 6861 7420 6661 696c 6564 2069 6e20   that failed in 
-00003d10: 7468 6520 6c61 7374 2074 6573 7420 7275  the last test ru
-00003d20: 6e2e 0a0a 2d2d 7072 6f63 6573 7365 733d  n...--processes=
-00003d30: 4e55 4d0a 0a20 2020 5370 7265 6164 2074  NUM..   Spread t
-00003d40: 6573 7420 7275 6e20 616d 6f6e 6720 7468  est run among th
-00003d50: 6973 206d 616e 7920 7072 6f63 6573 7365  is many processe
-00003d60: 732e 2053 6574 2061 206e 756d 6265 7220  s. Set a number 
-00003d70: 6571 7561 6c20 746f 0a20 2020 7468 6520  equal to.   the 
-00003d80: 6e75 6d62 6572 206f 6620 7072 6f63 6573  number of proces
-00003d90: 736f 7273 206f 7220 636f 7265 7320 696e  sors or cores in
-00003da0: 2079 6f75 7220 6d61 6368 696e 6520 666f   your machine fo
-00003db0: 7220 6265 7374 2072 6573 756c 7473 2e0a  r best results..
-00003dc0: 2020 2050 6173 7320 6120 6e65 6761 7469     Pass a negati
-00003dd0: 7665 206e 756d 6265 7220 746f 2068 6176  ve number to hav
-00003de0: 6520 7468 6520 6e75 6d62 6572 206f 6620  e the number of 
-00003df0: 7072 6f63 6573 7365 730a 2020 2061 7574  processes.   aut
-00003e00: 6f6d 6174 6963 616c 6c79 2073 6574 2074  omatically set t
-00003e10: 6f20 7468 6520 6e75 6d62 6572 206f 6620  o the number of 
-00003e20: 636f 7265 732e 2050 6173 7369 6e67 2030  cores. Passing 0
-00003e30: 206d 6561 6e73 2074 6f0a 2020 2064 6973   means to.   dis
-00003e40: 6162 6c65 2070 6172 616c 6c65 6c20 7465  able parallel te
-00003e50: 7374 696e 672e 2044 6566 6175 6c74 2069  sting. Default i
-00003e60: 7320 3020 756e 6c65 7373 204e 4f53 455f  s 0 unless NOSE_
-00003e70: 5052 4f43 4553 5345 5320 6973 0a20 2020  PROCESSES is.   
-00003e80: 7365 742e 205b 4e4f 5345 5f50 524f 4345  set. [NOSE_PROCE
-00003e90: 5353 4553 5d0a 0a2d 2d70 726f 6365 7373  SSES]..--process
-00003ea0: 2d74 696d 656f 7574 3d53 4543 4f4e 4453  -timeout=SECONDS
-00003eb0: 0a0a 2020 2053 6574 2074 696d 656f 7574  ..   Set timeout
-00003ec0: 2066 6f72 2072 6574 7572 6e20 6f66 2072   for return of r
-00003ed0: 6573 756c 7473 2066 726f 6d20 6561 6368  esults from each
-00003ee0: 2074 6573 7420 7275 6e6e 6572 2070 726f   test runner pro
-00003ef0: 6365 7373 2e0a 2020 2044 6566 6175 6c74  cess..   Default
-00003f00: 2069 7320 3130 2e20 5b4e 4f53 455f 5052   is 10. [NOSE_PR
-00003f10: 4f43 4553 535f 5449 4d45 4f55 545d 0a0a  OCESS_TIMEOUT]..
-00003f20: 2d2d 7072 6f63 6573 732d 7265 7374 6172  --process-restar
-00003f30: 7477 6f72 6b65 720a 0a20 2020 4966 2073  tworker..   If s
-00003f40: 6574 2c20 7769 6c6c 2072 6573 7461 7274  et, will restart
-00003f50: 2065 6163 6820 776f 726b 6572 2070 726f   each worker pro
-00003f60: 6365 7373 206f 6e63 6520 7468 6569 7220  cess once their 
-00003f70: 7465 7374 7320 6172 6520 646f 6e65 2c0a  tests are done,.
-00003f80: 2020 2074 6869 7320 6865 6c70 7320 636f     this helps co
-00003f90: 6e74 726f 6c20 6d65 6d6f 7279 206c 6561  ntrol memory lea
-00003fa0: 6b73 2066 726f 6d20 6b69 6c6c 696e 6720  ks from killing 
-00003fb0: 7468 6520 7379 7374 656d 2e0a 2020 205b  the system..   [
-00003fc0: 4e4f 5345 5f50 524f 4345 5353 5f52 4553  NOSE_PROCESS_RES
-00003fd0: 5441 5254 574f 524b 4552 5d0a 0a2d 2d77  TARTWORKER]..--w
-00003fe0: 6974 682d 7875 6e69 740a 0a20 2020 456e  ith-xunit..   En
-00003ff0: 6162 6c65 2070 6c75 6769 6e20 5875 6e69  able plugin Xuni
-00004000: 743a 2054 6869 7320 706c 7567 696e 2070  t: This plugin p
-00004010: 726f 7669 6465 7320 7465 7374 2072 6573  rovides test res
-00004020: 756c 7473 2069 6e20 7468 650a 2020 2073  ults in the.   s
-00004030: 7461 6e64 6172 6420 5855 6e69 7420 584d  tandard XUnit XM
-00004040: 4c20 666f 726d 6174 2e20 5b4e 4f53 455f  L format. [NOSE_
-00004050: 5749 5448 5f58 554e 4954 5d0a 0a2d 2d78  WITH_XUNIT]..--x
-00004060: 756e 6974 2d66 696c 653d 4649 4c45 0a0a  unit-file=FILE..
-00004070: 2020 2050 6174 6820 746f 2078 6d6c 2066     Path to xml f
-00004080: 696c 6520 746f 2073 746f 7265 2074 6865  ile to store the
-00004090: 2078 756e 6974 2072 6570 6f72 7420 696e   xunit report in
-000040a0: 2e20 4465 6661 756c 7420 6973 0a20 2020  . Default is.   
-000040b0: 6e6f 7365 7465 7374 732e 786d 6c20 696e  nosetests.xml in
-000040c0: 2074 6865 2077 6f72 6b69 6e67 2064 6972   the working dir
-000040d0: 6563 746f 7279 205b 4e4f 5345 5f58 554e  ectory [NOSE_XUN
-000040e0: 4954 5f46 494c 455d 0a0a 2d2d 7875 6e69  IT_FILE]..--xuni
-000040f0: 742d 7465 7374 7375 6974 652d 6e61 6d65  t-testsuite-name
-00004100: 3d50 4143 4b41 4745 0a0a 2020 204e 616d  =PACKAGE..   Nam
-00004110: 6520 6f66 2074 6865 2074 6573 7473 7569  e of the testsui
-00004120: 7465 2069 6e20 7468 6520 7875 6e69 7420  te in the xunit 
-00004130: 786d 6c2c 2067 656e 6572 6174 6564 2062  xml, generated b
-00004140: 7920 706c 7567 696e 2e0a 2020 2044 6566  y plugin..   Def
-00004150: 6175 6c74 2074 6573 7420 7375 6974 6520  ault test suite 
-00004160: 6e61 6d65 2069 7320 6e6f 7365 7465 7374  name is nosetest
-00004170: 732e 0a0a 2d2d 616c 6c2d 6d6f 6475 6c65  s...--all-module
-00004180: 730a 0a20 2020 456e 6162 6c65 2070 6c75  s..   Enable plu
-00004190: 6769 6e20 416c 6c4d 6f64 756c 6573 3a20  gin AllModules: 
-000041a0: 436f 6c6c 6563 7420 7465 7374 7320 6672  Collect tests fr
-000041b0: 6f6d 2061 6c6c 2070 7974 686f 6e20 6d6f  om all python mo
-000041c0: 6475 6c65 732e 0a20 2020 5b4e 4f53 455f  dules..   [NOSE_
-000041d0: 414c 4c5f 4d4f 4455 4c45 535d 0a0a 2d2d  ALL_MODULES]..--
-000041e0: 636f 2c20 2d2d 636f 6c6c 6563 742d 6f6e  co, --collect-on
-000041f0: 6c79 0a0a 2020 2045 6e61 626c 6520 636f  ly..   Enable co
-00004200: 6c6c 6563 742d 6f6e 6c79 3a20 436f 6c6c  llect-only: Coll
-00004210: 6563 7420 616e 6420 6f75 7470 7574 2074  ect and output t
-00004220: 6573 7420 6e61 6d65 7320 6f6e 6c79 2c0a  est names only,.
-00004230: 2020 2062 7574 2064 6f20 6e6f 7420 7275     but do not ru
-00004240: 6e20 616e 7920 7465 7374 732e 205b 434f  n any tests. [CO
-00004250: 4c4c 4543 545f 4f4e 4c59 5d0a 6060 600a  LLECT_ONLY].```.
+00000000: 3c68 313e 7079 6e6f 7365 20f0 9f90 8df0  <h1>pynose .....
+00000010: 9f91 8320 3c61 2068 7265 663d 2268 7474  ... <a href="htt
+00000020: 7073 3a2f 2f70 7970 692e 7079 7468 6f6e  ps://pypi.python
+00000030: 2e6f 7267 2f70 7970 692f 7079 6e6f 7365  .org/pypi/pynose
+00000040: 2220 7461 7267 6574 3d22 5f62 6c61 6e6b  " target="_blank
+00000050: 223e 3c69 6d67 2073 7263 3d22 6874 7470  "><img src="http
+00000060: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
+00000070: 696f 2f70 7970 692f 762f 7079 6e6f 7365  io/pypi/v/pynose
+00000080: 2e73 7667 3f63 6f6c 6f72 3d33 3339 3945  .svg?color=3399E
+00000090: 4522 2061 6c74 3d22 5079 5049 2076 6572  E" alt="PyPI ver
+000000a0: 7369 6f6e 2220 2f3e 3c2f 613e 3c2f 6831  sion" /></a></h1
+000000b0: 3e0a 0a23 2323 202a 2a5b 7079 6e6f 7365  >..### **[pynose
+000000c0: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
+000000d0: 2e63 6f6d 2f6d 646d 696e 747a 2f70 796e  .com/mdmintz/pyn
+000000e0: 6f73 6529 2a2a 2066 6978 6573 202a 2a5b  ose)** fixes **[
+000000f0: 6e6f 7365 5d28 6874 7470 733a 2f2f 6e6f  nose](https://no
+00000100: 7365 2e72 6561 6474 6865 646f 6373 2e69  se.readthedocs.i
+00000110: 6f2f 656e 2f6c 6174 6573 742f 292a 2a20  o/en/latest/)** 
+00000120: 746f 2065 7874 656e 6420 5b75 6e69 7474  to extend [unitt
+00000130: 6573 745d 2868 7474 7073 3a2f 2f64 6f63  est](https://doc
+00000140: 732e 7079 7468 6f6e 2e6f 7267 2f33 2f6c  s.python.org/3/l
+00000150: 6962 7261 7279 2f75 6e69 7474 6573 742e  ibrary/unittest.
+00000160: 6874 6d6c 2920 616e 6420 6d61 6b65 2074  html) and make t
+00000170: 6573 7469 6e67 2065 6173 6965 722e 0a0a  esting easier...
+00000180: 2d2d 2d2d 2d2d 2d2d 0a0a 6060 7079 6e6f  --------..``pyno
+00000190: 7365 6060 2069 7320 616e 2075 7064 6174  se`` is an updat
+000001a0: 6564 2076 6572 7369 6f6e 206f 6620 6060  ed version of ``
+000001b0: 6e6f 7365 6060 2c20 6f72 6967 696e 616c  nose``, original
+000001c0: 6c79 206d 6164 6520 6279 204a 6173 6f6e  ly made by Jason
+000001d0: 2050 656c 6c65 7269 6e2e 0a0a 5468 6973   Pellerin...This
+000001e0: 2076 6572 7369 6f6e 206f 6620 6060 6e6f   version of ``no
+000001f0: 7365 6060 2069 7320 636f 6d70 6174 6962  se`` is compatib
+00000200: 6c65 2077 6974 6820 6060 5079 7468 6f6e  le with ``Python
+00000210: 2033 2e36 2b60 6020 2869 6e63 6c75 6469   3.6+`` (includi
+00000220: 6e67 2060 6033 2e31 322b 6060 292e 0a0a  ng ``3.12+``)...
+00000230: 4368 616e 6765 7320 696e 2060 6070 796e  Changes in ``pyn
+00000240: 6f73 6560 6020 6672 6f6d 206c 6567 6163  ose`` from legac
+00000250: 7920 6060 6e6f 7365 6060 2069 6e63 6c75  y ``nose`` inclu
+00000260: 6465 3a0a 2a20 4669 7865 7320 2241 7474  de:.* Fixes "Att
+00000270: 7269 6275 7465 4572 726f 723a 206d 6f64  ributeError: mod
+00000280: 756c 6520 2763 6f6c 6c65 6374 696f 6e73  ule 'collections
+00000290: 2720 6861 7320 6e6f 2061 7474 7269 6275  ' has no attribu
+000002a0: 7465 2027 4361 6c6c 6162 6c65 272e 220a  te 'Callable'.".
+000002b0: 2a20 4669 7865 7320 2241 7474 7269 6275  * Fixes "Attribu
+000002c0: 7465 4572 726f 723a 206d 6f64 756c 6520  teError: module 
+000002d0: 2769 6e73 7065 6374 2720 6861 7320 6e6f  'inspect' has no
+000002e0: 2061 7474 7269 6275 7465 2027 6765 7461   attribute 'geta
+000002f0: 7267 7370 6563 272e 220a 2a20 4669 7865  rgspec'.".* Fixe
+00000300: 7320 2249 6d70 6f72 7445 7272 6f72 3a20  s "ImportError: 
+00000310: 6361 6e6e 6f74 2069 6d70 6f72 7420 6e61  cannot import na
+00000320: 6d65 2027 5f54 6578 7454 6573 7452 6573  me '_TextTestRes
+00000330: 756c 7427 2066 726f 6d20 2775 6e69 7474  ult' from 'unitt
+00000340: 6573 7427 2e22 0a2a 2046 6978 6573 2022  est'.".* Fixes "
+00000350: 5275 6e74 696d 6557 6172 6e69 6e67 3a20  RuntimeWarning: 
+00000360: 5465 7374 5265 7375 6c74 2068 6173 206e  TestResult has n
+00000370: 6f20 6164 6444 7572 6174 696f 6e20 6d65  o addDuration me
+00000380: 7468 6f64 2e22 0a2a 2046 6978 6573 2022  thod.".* Fixes "
+00000390: 4465 7072 6563 6174 696f 6e57 6172 6e69  DeprecationWarni
+000003a0: 6e67 3a20 706b 675f 7265 736f 7572 6365  ng: pkg_resource
+000003b0: 7320 6973 2064 6570 7265 6361 7465 6420  s is deprecated 
+000003c0: 6173 2061 6e20 4150 492e 220a 2a20 4669  as an API.".* Fi
+000003d0: 7865 7320 616c 6c20 6060 666c 616b 6538  xes all ``flake8
+000003e0: 6060 2069 7373 7565 7320 6672 6f6d 2074  `` issues from t
+000003f0: 6865 206f 7269 6769 6e61 6c20 6060 6e6f  he original ``no
+00000400: 7365 6060 2e0a 2a20 5265 706c 6163 6573  se``..* Replaces
+00000410: 2074 6865 2060 6069 6d70 6060 206d 6f64   the ``imp`` mod
+00000420: 756c 6520 7769 7468 2074 6865 206e 6577  ule with the new
+00000430: 6572 2060 6069 6d70 6f72 746c 6962 6060  er ``importlib``
+00000440: 206d 6f64 756c 652e 0a2a 2054 6865 2064   module..* The d
+00000450: 6566 6175 6c74 206c 6f67 6769 6e67 206c  efault logging l
+00000460: 6576 656c 206e 6f77 2068 6964 6573 2022  evel now hides "
+00000470: 6465 6275 6722 206c 6f67 7320 666f 7220  debug" logs for 
+00000480: 6c65 7373 206e 6f69 7365 2e0a 2a20 5468  less noise..* Th
+00000490: 6520 6060 2d73 6060 206f 7074 696f 6e20  e ``-s`` option 
+000004a0: 6973 2061 6c77 6179 7320 6163 7469 7665  is always active
+000004b0: 2074 6f20 7365 6520 7468 6520 6f75 7470   to see the outp
+000004c0: 7574 206f 6620 6060 7072 696e 7428 2960  ut of ``print()`
+000004d0: 602e 0a2a 2041 6464 7320 6060 2d2d 636f  `..* Adds ``--co
+000004e0: 6060 2061 7320 6120 7368 6f72 7463 7574  `` as a shortcut
+000004f0: 2074 6f20 7573 696e 6720 6060 2d2d 636f   to using ``--co
+00000500: 6c6c 6563 742d 6f6e 6c79 6060 2e0a 0a2d  llect-only``...-
+00000510: 2d2d 2d2d 2d2d 2d0a 0a54 6865 206f 7269  -------..The ori
+00000520: 6769 6e61 6c20 6465 7363 7269 7074 696f  ginal descriptio
+00000530: 6e20 6f66 2060 606e 6f73 6560 603a 0a0a  n of ``nose``:..
+00000540: 3e6e 6f73 6520 6578 7465 6e64 7320 7468  >nose extends th
+00000550: 6520 7465 7374 206c 6f61 6469 6e67 2061  e test loading a
+00000560: 6e64 2072 756e 6e69 6e67 2066 6561 7475  nd running featu
+00000570: 7265 7320 6f66 2075 6e69 7474 6573 742c  res of unittest,
+00000580: 206d 616b 696e 670a 6974 2065 6173 6965   making.it easie
+00000590: 7220 746f 2077 7269 7465 2c20 6669 6e64  r to write, find
+000005a0: 2061 6e64 2072 756e 2074 6573 7473 2e0a   and run tests..
+000005b0: 0a3e 4279 2064 6566 6175 6c74 2c20 6e6f  .>By default, no
+000005c0: 7365 2072 756e 7320 7465 7374 7320 696e  se runs tests in
+000005d0: 2066 696c 6573 206f 7220 6469 7265 6374   files or direct
+000005e0: 6f72 6965 7320 756e 6465 7220 7468 6520  ories under the 
+000005f0: 6375 7272 656e 740a 776f 726b 696e 6720  current.working 
+00000600: 6469 7265 6374 6f72 7920 7768 6f73 6520  directory whose 
+00000610: 6e61 6d65 7320 696e 636c 7564 6520 2274  names include "t
+00000620: 6573 7422 206f 7220 2254 6573 7422 2061  est" or "Test" a
+00000630: 7420 6120 776f 7264 0a62 6f75 6e64 6172  t a word.boundar
+00000640: 7920 286c 696b 6520 2274 6573 745f 7468  y (like "test_th
+00000650: 6973 2220 6f72 2022 6675 6e63 7469 6f6e  is" or "function
+00000660: 616c 5f74 6573 7422 206f 7220 2254 6573  al_test" or "Tes
+00000670: 7443 6c61 7373 2220 6275 7420 6e6f 740a  tClass" but not.
+00000680: 226c 6962 7465 7374 2229 2e20 5465 7374  "libtest"). Test
+00000690: 206f 7574 7075 7420 6973 2073 696d 696c   output is simil
+000006a0: 6172 2074 6f20 7468 6174 206f 6620 756e  ar to that of un
+000006b0: 6974 7465 7374 2c20 6275 7420 616c 736f  ittest, but also
+000006c0: 2069 6e63 6c75 6465 730a 6361 7074 7572   includes.captur
+000006d0: 6564 2073 7464 6f75 7420 6f75 7470 7574  ed stdout output
+000006e0: 2066 726f 6d20 6661 696c 696e 6720 7465   from failing te
+000006f0: 7374 732c 2066 6f72 2065 6173 7920 7072  sts, for easy pr
+00000700: 696e 742d 7374 796c 6520 6465 6275 6767  int-style debugg
+00000710: 696e 672e 0a0a 3e54 6865 7365 2066 6561  ing...>These fea
+00000720: 7475 7265 732c 2061 6e64 206d 616e 7920  tures, and many 
+00000730: 6d6f 7265 2c20 6172 6520 6375 7374 6f6d  more, are custom
+00000740: 697a 6162 6c65 2074 6872 6f75 6768 2074  izable through t
+00000750: 6865 2075 7365 206f 660a 706c 7567 696e  he use of.plugin
+00000760: 732e 2050 6c75 6769 6e73 2069 6e63 6c75  s. Plugins inclu
+00000770: 6465 6420 7769 7468 206e 6f73 6520 7072  ded with nose pr
+00000780: 6f76 6964 6520 7375 7070 6f72 7420 666f  ovide support fo
+00000790: 7220 646f 6374 6573 742c 2063 6f64 650a  r doctest, code.
+000007a0: 636f 7665 7261 6765 2061 6e64 2070 726f  coverage and pro
+000007b0: 6669 6c69 6e67 2c20 666c 6578 6962 6c65  filing, flexible
+000007c0: 2061 7474 7269 6275 7465 2d62 6173 6564   attribute-based
+000007d0: 2074 6573 7420 7365 6c65 6374 696f 6e2c   test selection,
+000007e0: 0a6f 7574 7075 7420 6361 7074 7572 6520  .output capture 
+000007f0: 616e 6420 6d6f 7265 2e20 4d6f 7265 2069  and more. More i
+00000800: 6e66 6f72 6d61 7469 6f6e 2061 626f 7574  nformation about
+00000810: 2077 7269 7469 6e67 2070 6c75 6769 6e73   writing plugins
+00000820: 0a6d 6179 2062 6520 666f 756e 6420 6f6e  .may be found on
+00000830: 2069 6e20 7468 6520 6e6f 7365 2041 5049   in the nose API
+00000840: 2064 6f63 756d 656e 7461 7469 6f6e 2c20   documentation, 
+00000850: 6865 7265 3a0a 6874 7470 733a 2f2f 6e6f  here:.https://no
+00000860: 7365 2e72 6561 6474 6865 646f 6373 2e69  se.readthedocs.i
+00000870: 6f2f 656e 2f6c 6174 6573 742f 0a0a 2d2d  o/en/latest/..--
+00000880: 2d2d 2d2d 2d2d 0a0a 6060 6062 6173 680a  ------..```bash.
+00000890: 0a42 6173 6963 2075 7361 6765 0a2a 2a2a  .Basic usage.***
+000008a0: 2a2a 2a2a 2a2a 2a2a 0a0a 5573 6520 2270  ********..Use "p
+000008b0: 796e 6f73 6522 204f 5220 226e 6f73 6574  ynose" OR "noset
+000008c0: 6573 7473 2220 746f 2072 756e 2074 6573  ests" to run tes
+000008d0: 7473 3a0a 0a20 2020 2070 796e 6f73 6520  ts:..    pynose 
+000008e0: 5b6f 7074 696f 6e73 5d20 5b28 6f70 7469  [options] [(opti
+000008f0: 6f6e 616c 2920 7465 7374 2066 696c 6573  onal) test files
+00000900: 206f 7220 6469 7265 6374 6f72 6965 735d   or directories]
+00000910: 0a0a 2020 2020 6e6f 7365 7465 7374 7320  ..    nosetests 
+00000920: 5b6f 7074 696f 6e73 5d20 5b28 6f70 7469  [options] [(opti
+00000930: 6f6e 616c 2920 7465 7374 2066 696c 6573  onal) test files
+00000940: 206f 7220 6469 7265 6374 6f72 6965 735d   or directories]
+00000950: 0a0a 496e 2061 6464 6974 696f 6e20 746f  ..In addition to
+00000960: 2070 6173 7369 6e67 2063 6f6d 6d61 6e64   passing command
+00000970: 2d6c 696e 6520 6f70 7469 6f6e 732c 2079  -line options, y
+00000980: 6f75 206d 6179 2061 6c73 6f20 7075 740a  ou may also put.
+00000990: 636f 6e66 6967 7572 6174 696f 6e20 6f70  configuration op
+000009a0: 7469 6f6e 7320 696e 2061 202e 6e6f 7365  tions in a .nose
+000009b0: 7263 206f 7220 6e6f 7365 2e63 6667 2066  rc or nose.cfg f
+000009c0: 696c 6520 696e 2079 6f75 7220 686f 6d65  ile in your home
+000009d0: 0a64 6972 6563 746f 7279 2e20 5468 6573  .directory. Thes
+000009e0: 6520 6172 6520 7374 616e 6461 7264 202e  e are standard .
+000009f0: 696e 692d 7374 796c 6520 636f 6e66 6967  ini-style config
+00000a00: 2066 696c 6573 2e20 5075 7420 796f 7572   files. Put your
+00000a10: 0a6e 6f73 6574 6573 7473 2063 6f6e 6669  .nosetests confi
+00000a20: 6775 7261 7469 6f6e 2069 6e20 6120 5b6e  guration in a [n
+00000a30: 6f73 6574 6573 7473 5d20 7365 6374 696f  osetests] sectio
+00000a40: 6e2c 2077 6974 6820 7468 6520 2d2d 2070  n, with the -- p
+00000a50: 7265 6669 780a 7265 6d6f 7665 643a 0a0a  refix.removed:..
+00000a60: 2020 205b 6e6f 7365 7465 7374 735d 0a20     [nosetests]. 
+00000a70: 2020 7665 7262 6f73 6974 793d 330a 2020    verbosity=3.  
+00000a80: 2077 6974 682d 646f 6374 6573 743d 310a   with-doctest=1.
+00000a90: 0a54 6865 7265 2069 7320 616c 736f 2070  .There is also p
+00000aa0: 6f73 7369 626c 6974 7920 746f 2064 6973  ossiblity to dis
+00000ab0: 6162 6c65 2063 6f6e 6669 6775 7261 7469  able configurati
+00000ac0: 6f6e 2066 696c 6573 206c 6f61 6469 6e67  on files loading
+00000ad0: 2028 6d69 6768 740a 6265 2075 7365 6675   (might.be usefu
+00000ae0: 6c20 7768 656e 2072 756e 6e69 6720 692e  l when runnig i.
+00000af0: 652e 2074 6f78 2061 6e64 2079 6f75 2064  e. tox and you d
+00000b00: 6f20 6e6f 7420 7761 6e74 2079 6f75 7220  o not want your 
+00000b10: 676c 6f62 616c 206e 6f73 650a 636f 6e66  global nose.conf
+00000b20: 6967 2066 696c 6520 746f 2062 6520 7573  ig file to be us
+00000b30: 6564 2062 7920 746f 7829 2e20 496e 206f  ed by tox). In o
+00000b40: 7264 6572 2074 6f20 6967 6e6f 7265 2074  rder to ignore t
+00000b50: 686f 7365 2063 6f6e 6669 6775 7261 7469  hose configurati
+00000b60: 6f6e 0a66 696c 6573 2073 696d 706c 7920  on.files simply 
+00000b70: 7365 7420 616e 2065 6e76 6972 6f6e 6d65  set an environme
+00000b80: 6e74 2076 6172 6961 626c 6520 224e 4f53  nt variable "NOS
+00000b90: 455f 4947 4e4f 5245 5f43 4f4e 4649 475f  E_IGNORE_CONFIG_
+00000ba0: 4649 4c45 5322 2e0a 0a54 6865 7265 2061  FILES"...There a
+00000bb0: 7265 2073 6576 6572 616c 206f 7468 6572  re several other
+00000bc0: 2077 6179 7320 746f 2075 7365 2074 6865   ways to use the
+00000bd0: 206e 6f73 6520 7465 7374 2072 756e 6e65   nose test runne
+00000be0: 7220 6265 7369 6465 7320 7468 650a 2a6e  r besides the.*n
+00000bf0: 6f73 6574 6573 7473 2a20 7363 7269 7074  osetests* script
+00000c00: 2e20 596f 7520 6d61 7920 7573 6520 6e6f  . You may use no
+00000c10: 7365 2069 6e20 6120 7465 7374 2073 6372  se in a test scr
+00000c20: 6970 743a 0a0a 2020 2069 6d70 6f72 7420  ipt:..   import 
+00000c30: 6e6f 7365 0a20 2020 6e6f 7365 2e6d 6169  nose.   nose.mai
+00000c40: 6e28 290a 0a49 6620 796f 7520 646f 206e  n()..If you do n
+00000c50: 6f74 2077 616e 7420 7468 6520 7465 7374  ot want the test
+00000c60: 2073 6372 6970 7420 746f 2065 7869 7420   script to exit 
+00000c70: 7769 7468 2030 206f 6e20 7375 6363 6573  with 0 on succes
+00000c80: 7320 616e 6420 3120 6f6e 0a66 6169 6c75  s and 1 on.failu
+00000c90: 7265 2028 6c69 6b65 2075 6e69 7474 6573  re (like unittes
+00000ca0: 742e 6d61 696e 292c 2075 7365 206e 6f73  t.main), use nos
+00000cb0: 652e 7275 6e28 2920 696e 7374 6561 643a  e.run() instead:
+00000cc0: 0a0a 2020 2069 6d70 6f72 7420 6e6f 7365  ..   import nose
+00000cd0: 0a20 2020 7265 7375 6c74 203d 206e 6f73  .   result = nos
+00000ce0: 652e 7275 6e28 290a 0a2a 7265 7375 6c74  e.run()..*result
+00000cf0: 2a20 7769 6c6c 2062 6520 7472 7565 2069  * will be true i
+00000d00: 6620 7468 6520 7465 7374 2072 756e 2073  f the test run s
+00000d10: 7563 6365 6564 6564 2c20 6f72 2066 616c  ucceeded, or fal
+00000d20: 7365 2069 6620 616e 7920 7465 7374 0a66  se if any test.f
+00000d30: 6169 6c65 6420 6f72 2072 6169 7365 6420  ailed or raised 
+00000d40: 616e 2075 6e63 6175 6768 7420 6578 6365  an uncaught exce
+00000d50: 7074 696f 6e2e 204c 6173 746c 792c 2079  ption. Lastly, y
+00000d60: 6f75 2063 616e 2072 756e 206e 6f73 652e  ou can run nose.
+00000d70: 636f 7265 0a64 6972 6563 746c 792c 2077  core.directly, w
+00000d80: 6869 6368 2077 696c 6c20 7275 6e20 6e6f  hich will run no
+00000d90: 7365 2e6d 6169 6e28 293a 0a0a 2020 2070  se.main():..   p
+00000da0: 7974 686f 6e20 2f70 6174 682f 746f 2f6e  ython /path/to/n
+00000db0: 6f73 652f 636f 7265 2e70 790a 0a50 6c65  ose/core.py..Ple
+00000dc0: 6173 6520 7365 6520 7468 6520 7573 6167  ase see the usag
+00000dd0: 6520 6d65 7373 6167 6520 666f 7220 7468  e message for th
+00000de0: 6520 6e6f 7365 7465 7374 7320 7363 7269  e nosetests scri
+00000df0: 7074 2066 6f72 2069 6e66 6f72 6d61 7469  pt for informati
+00000e00: 6f6e 0a61 626f 7574 2068 6f77 2074 6f20  on.about how to 
+00000e10: 636f 6e74 726f 6c20 7768 6963 6820 7465  control which te
+00000e20: 7374 7320 6e6f 7365 2072 756e 732c 2077  sts nose runs, w
+00000e30: 6869 6368 2070 6c75 6769 6e73 2061 7265  hich plugins are
+00000e40: 206c 6f61 6465 642c 0a61 6e64 2074 6865   loaded,.and the
+00000e50: 2074 6573 7420 6f75 7470 7574 2e0a 0a0a   test output....
+00000e60: 4578 7465 6e64 6564 2075 7361 6765 0a3d  Extended usage.=
+00000e70: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d0a 0a6e  =============..n
+00000e80: 6f73 6520 636f 6c6c 6563 7473 2074 6573  ose collects tes
+00000e90: 7473 2061 7574 6f6d 6174 6963 616c 6c79  ts automatically
+00000ea0: 2066 726f 6d20 7079 7468 6f6e 2073 6f75   from python sou
+00000eb0: 7263 6520 6669 6c65 732c 0a64 6972 6563  rce files,.direc
+00000ec0: 746f 7269 6573 2061 6e64 2070 6163 6b61  tories and packa
+00000ed0: 6765 7320 666f 756e 6420 696e 2069 7473  ges found in its
+00000ee0: 2077 6f72 6b69 6e67 2064 6972 6563 746f   working directo
+00000ef0: 7279 2028 7768 6963 680a 6465 6661 756c  ry (which.defaul
+00000f00: 7473 2074 6f20 7468 6520 6375 7272 656e  ts to the curren
+00000f10: 7420 776f 726b 696e 6720 6469 7265 6374  t working direct
+00000f20: 6f72 7929 2e20 416e 7920 7079 7468 6f6e  ory). Any python
+00000f30: 2073 6f75 7263 6520 6669 6c65 2c0a 6469   source file,.di
+00000f40: 7265 6374 6f72 7920 6f72 2070 6163 6b61  rectory or packa
+00000f50: 6765 2074 6861 7420 6d61 7463 6865 7320  ge that matches 
+00000f60: 7468 6520 7465 7374 4d61 7463 6820 7265  the testMatch re
+00000f70: 6775 6c61 7220 6578 7072 6573 7369 6f6e  gular expression
+00000f80: 2028 6279 0a64 6566 6175 6c74 3a20 2a28   (by.default: *(
+00000f90: 3f3a 5e7c 5b62 5f2e 2d5d 295b 5474 5d65  ?:^|[b_.-])[Tt]e
+00000fa0: 7374 292a 2077 696c 6c20 6265 2063 6f6c  st)* will be col
+00000fb0: 6c65 6374 6564 2061 7320 6120 7465 7374  lected as a test
+00000fc0: 2028 6f72 2073 6f75 7263 650a 666f 7220   (or source.for 
+00000fd0: 636f 6c6c 6563 7469 6f6e 206f 6620 7465  collection of te
+00000fe0: 7374 7329 2e20 496e 2061 6464 6974 696f  sts). In additio
+00000ff0: 6e2c 2061 6c6c 206f 7468 6572 2070 6163  n, all other pac
+00001000: 6b61 6765 7320 666f 756e 6420 696e 2074  kages found in t
+00001010: 6865 0a77 6f72 6b69 6e67 2064 6972 6563  he.working direc
+00001020: 746f 7279 2077 696c 6c20 6265 2065 7861  tory will be exa
+00001030: 6d69 6e65 6420 666f 7220 7079 7468 6f6e  mined for python
+00001040: 2073 6f75 7263 6520 6669 6c65 7320 6f72   source files or
+00001050: 0a64 6972 6563 746f 7269 6573 2074 6861  .directories tha
+00001060: 7420 6d61 7463 6820 7465 7374 4d61 7463  t match testMatc
+00001070: 682e 2050 6163 6b61 6765 2064 6973 636f  h. Package disco
+00001080: 7665 7279 2064 6573 6365 6e64 7320 616c  very descends al
+00001090: 6c20 7468 650a 7761 7920 646f 776e 2074  l the.way down t
+000010a0: 6865 2074 7265 652c 2073 6f20 7061 636b  he tree, so pack
+000010b0: 6167 652e 7465 7374 7320 616e 6420 7061  age.tests and pa
+000010c0: 636b 6167 652e 7375 622e 7465 7374 7320  ckage.sub.tests 
+000010d0: 616e 640a 7061 636b 6167 652e 7375 622e  and.package.sub.
+000010e0: 7375 6232 2e74 6573 7473 2077 696c 6c20  sub2.tests will 
+000010f0: 616c 6c20 6265 2063 6f6c 6c65 6374 6564  all be collected
+00001100: 2e0a 0a57 6974 6869 6e20 6120 7465 7374  ...Within a test
+00001110: 2064 6972 6563 746f 7279 206f 7220 7061   directory or pa
+00001120: 636b 6167 652c 2061 6e79 2070 7974 686f  ckage, any pytho
+00001130: 6e20 736f 7572 6365 2066 696c 6520 6d61  n source file ma
+00001140: 7463 6869 6e67 0a74 6573 744d 6174 6368  tching.testMatch
+00001150: 2077 696c 6c20 6265 2065 7861 6d69 6e65   will be examine
+00001160: 6420 666f 7220 7465 7374 2063 6173 6573  d for test cases
+00001170: 2e20 5769 7468 696e 2061 2074 6573 7420  . Within a test 
+00001180: 6d6f 6475 6c65 2c0a 6675 6e63 7469 6f6e  module,.function
+00001190: 7320 616e 6420 636c 6173 7365 7320 7768  s and classes wh
+000011a0: 6f73 6520 6e61 6d65 7320 6d61 7463 6820  ose names match 
+000011b0: 7465 7374 4d61 7463 6820 616e 6420 5465  testMatch and Te
+000011c0: 7374 4361 7365 0a73 7562 636c 6173 7365  stCase.subclasse
+000011d0: 7320 7769 7468 2061 6e79 206e 616d 6520  s with any name 
+000011e0: 7769 6c6c 2062 6520 6c6f 6164 6564 2061  will be loaded a
+000011f0: 6e64 2065 7865 6375 7465 6420 6173 2074  nd executed as t
+00001200: 6573 7473 2e20 5465 7374 730a 6d61 7920  ests. Tests.may 
+00001210: 7573 6520 7468 6520 6173 7365 7274 206b  use the assert k
+00001220: 6579 776f 7264 206f 7220 7261 6973 6520  eyword or raise 
+00001230: 4173 7365 7274 696f 6e45 7272 6f72 7320  AssertionErrors 
+00001240: 746f 2069 6e64 6963 6174 6520 7465 7374  to indicate test
+00001250: 0a66 6169 6c75 7265 2e20 5465 7374 4361  .failure. TestCa
+00001260: 7365 2073 7562 636c 6173 7365 7320 6d61  se subclasses ma
+00001270: 7920 646f 2074 6865 2073 616d 6520 6f72  y do the same or
+00001280: 2075 7365 2074 6865 2076 6172 696f 7573   use the various
+00001290: 0a54 6573 7443 6173 6520 6d65 7468 6f64  .TestCase method
+000012a0: 7320 6176 6169 6c61 626c 652e 0a0a 2a2a  s available...**
+000012b0: 4974 2069 7320 696d 706f 7274 616e 7420  It is important 
+000012c0: 746f 206e 6f74 6520 7468 6174 2074 6865  to note that the
+000012d0: 2064 6566 6175 6c74 2062 6568 6176 696f   default behavio
+000012e0: 7220 6f66 206e 6f73 6520 6973 2074 6f20  r of nose is to 
+000012f0: 6e6f 740a 696e 636c 7564 6520 7465 7374  not.include test
+00001300: 7320 6672 6f6d 2066 696c 6573 2077 6869  s from files whi
+00001310: 6368 2061 7265 2065 7865 6375 7461 626c  ch are executabl
+00001320: 652e 2a2a 2020 546f 2069 6e63 6c75 6465  e.**  To include
+00001330: 2074 6573 7473 0a66 726f 6d20 7375 6368   tests.from such
+00001340: 2066 696c 6573 2c20 7265 6d6f 7665 2074   files, remove t
+00001350: 6865 6972 2065 7865 6375 7461 626c 6520  heir executable 
+00001360: 6269 7420 6f72 2075 7365 2074 6865 202d  bit or use the -
+00001370: 2d65 7865 2066 6c61 670a 2873 6565 2027  -exe flag.(see '
+00001380: 4f70 7469 6f6e 7327 2073 6563 7469 6f6e  Options' section
+00001390: 2062 656c 6f77 292e 0a0a 0a53 656c 6563   below)....Selec
+000013a0: 7469 6e67 2054 6573 7473 0a2d 2d2d 2d2d  ting Tests.-----
+000013b0: 2d2d 2d2d 2d2d 2d2d 2d2d 0a0a 546f 2073  ----------..To s
+000013c0: 7065 6369 6679 2077 6869 6368 2074 6573  pecify which tes
+000013d0: 7473 2074 6f20 7275 6e2c 2070 6173 7320  ts to run, pass 
+000013e0: 7465 7374 206e 616d 6573 206f 6e20 7468  test names on th
+000013f0: 6520 636f 6d6d 616e 6420 6c69 6e65 3a0a  e command line:.
+00001400: 0a20 2020 6e6f 7365 7465 7374 7320 6f6e  .   nosetests on
+00001410: 6c79 5f74 6573 745f 7468 6973 2e70 790a  ly_test_this.py.
+00001420: 0a54 6573 7420 6e61 6d65 7320 7370 6563  .Test names spec
+00001430: 6966 6965 6420 6d61 7920 6265 2066 696c  ified may be fil
+00001440: 6520 6f72 206d 6f64 756c 6520 6e61 6d65  e or module name
+00001450: 732c 2061 6e64 206d 6179 206f 7074 696f  s, and may optio
+00001460: 6e61 6c6c 790a 696e 6469 6361 7465 2074  nally.indicate t
+00001470: 6865 2074 6573 7420 6361 7365 2074 6f20  he test case to 
+00001480: 7275 6e20 6279 2073 6570 6172 6174 696e  run by separatin
+00001490: 6720 7468 6520 6d6f 6475 6c65 206f 7220  g the module or 
+000014a0: 6669 6c65 206e 616d 650a 6672 6f6d 2074  file name.from t
+000014b0: 6865 2074 6573 7420 6361 7365 206e 616d  he test case nam
+000014c0: 6520 7769 7468 2061 2063 6f6c 6f6e 2e20  e with a colon. 
+000014d0: 4669 6c65 6e61 6d65 7320 6d61 7920 6265  Filenames may be
+000014e0: 2072 656c 6174 6976 6520 6f72 0a61 6273   relative or.abs
+000014f0: 6f6c 7574 652e 2045 7861 6d70 6c65 733a  olute. Examples:
+00001500: 0a0a 2020 206e 6f73 6574 6573 7473 2074  ..   nosetests t
+00001510: 6573 742e 6d6f 6475 6c65 0a20 2020 6e6f  est.module.   no
+00001520: 7365 7465 7374 7320 616e 6f74 6865 722e  setests another.
+00001530: 7465 7374 3a54 6573 7443 6173 652e 7465  test:TestCase.te
+00001540: 7374 5f6d 6574 686f 640a 2020 206e 6f73  st_method.   nos
+00001550: 6574 6573 7473 2061 2e74 6573 743a 5465  etests a.test:Te
+00001560: 7374 4361 7365 0a20 2020 6e6f 7365 7465  stCase.   nosete
+00001570: 7374 7320 2f70 6174 682f 746f 2f74 6573  sts /path/to/tes
+00001580: 742f 6669 6c65 2e70 793a 7465 7374 5f66  t/file.py:test_f
+00001590: 756e 6374 696f 6e0a 0a59 6f75 206d 6179  unction..You may
+000015a0: 2061 6c73 6f20 6368 616e 6765 2074 6865   also change the
+000015b0: 2077 6f72 6b69 6e67 2064 6972 6563 746f   working directo
+000015c0: 7279 2077 6865 7265 206e 6f73 6520 6c6f  ry where nose lo
+000015d0: 6f6b 7320 666f 7220 7465 7374 730a 6279  oks for tests.by
+000015e0: 2075 7369 6e67 2074 6865 202d 7720 7377   using the -w sw
+000015f0: 6974 6368 3a0a 0a20 2020 6e6f 7365 7465  itch:..   nosete
+00001600: 7374 7320 2d77 202f 7061 7468 2f74 6f2f  sts -w /path/to/
+00001610: 7465 7374 730a 0a4e 6f74 652c 2068 6f77  tests..Note, how
+00001620: 6576 6572 2c20 7468 6174 2073 7570 706f  ever, that suppo
+00001630: 7274 2066 6f72 206d 756c 7469 706c 6520  rt for multiple 
+00001640: 2d77 2061 7267 756d 656e 7473 2069 7320  -w arguments is 
+00001650: 6e6f 770a 6465 7072 6563 6174 6564 2061  now.deprecated a
+00001660: 6e64 2077 696c 6c20 6265 2072 656d 6f76  nd will be remov
+00001670: 6564 2069 6e20 6120 6675 7475 7265 2072  ed in a future r
+00001680: 656c 6561 7365 2e20 4173 206f 6620 6e6f  elease. As of no
+00001690: 7365 2030 2e31 302c 0a79 6f75 2063 616e  se 0.10,.you can
+000016a0: 2067 6574 2074 6865 2073 616d 6520 6265   get the same be
+000016b0: 6861 7669 6f72 2062 7920 7370 6563 6966  havior by specif
+000016c0: 7969 6e67 2074 6865 2074 6172 6765 7420  ying the target 
+000016d0: 6469 7265 6374 6f72 6965 730a 2a77 6974  directories.*wit
+000016e0: 686f 7574 2a20 7468 6520 2d77 2073 7769  hout* the -w swi
+000016f0: 7463 683a 0a0a 2020 206e 6f73 6574 6573  tch:..   nosetes
+00001700: 7473 202f 7061 7468 2f74 6f2f 7465 7374  ts /path/to/test
+00001710: 7320 2f61 6e6f 7468 6572 2f70 6174 682f  s /another/path/
+00001720: 746f 2f74 6573 7473 0a0a 4675 7274 6865  to/tests..Furthe
+00001730: 7220 6375 7374 6f6d 697a 6174 696f 6e20  r customization 
+00001740: 6f66 2074 6573 7420 7365 6c65 6374 696f  of test selectio
+00001750: 6e20 616e 6420 6c6f 6164 696e 6720 6973  n and loading is
+00001760: 2070 6f73 7369 626c 650a 7468 726f 7567   possible.throug
+00001770: 6820 7468 6520 7573 6520 6f66 2070 6c75  h the use of plu
+00001780: 6769 6e73 2e0a 0a54 6573 7420 7265 7375  gins...Test resu
+00001790: 6c74 206f 7574 7075 7420 6973 2069 6465  lt output is ide
+000017a0: 6e74 6963 616c 2074 6f20 7468 6174 206f  ntical to that o
+000017b0: 6620 756e 6974 7465 7374 2c20 6578 6365  f unittest, exce
+000017c0: 7074 2066 6f72 2074 6865 0a61 6464 6974  pt for the.addit
+000017d0: 696f 6e61 6c20 6665 6174 7572 6573 2028  ional features (
+000017e0: 6572 726f 7220 636c 6173 7365 732c 2061  error classes, a
+000017f0: 6e64 2070 6c75 6769 6e2d 7375 7070 6c69  nd plugin-suppli
+00001800: 6564 2066 6561 7475 7265 7320 7375 6368  ed features such
+00001810: 0a61 7320 6f75 7470 7574 2063 6170 7475  .as output captu
+00001820: 7265 2061 6e64 2061 7373 6572 7420 696e  re and assert in
+00001830: 7472 6f73 7065 6374 696f 6e29 2064 6574  trospection) det
+00001840: 6169 6c65 6420 696e 2074 6865 206f 7074  ailed in the opt
+00001850: 696f 6e73 0a62 656c 6f77 2e0a 0a0a 436f  ions.below....Co
+00001860: 6e66 6967 7572 6174 696f 6e0a 2d2d 2d2d  nfiguration.----
+00001870: 2d2d 2d2d 2d2d 2d2d 2d0a 0a49 6e20 6164  ---------..In ad
+00001880: 6469 7469 6f6e 2074 6f20 7061 7373 696e  dition to passin
+00001890: 6720 636f 6d6d 616e 642d 6c69 6e65 206f  g command-line o
+000018a0: 7074 696f 6e73 2c20 796f 7520 6d61 7920  ptions, you may 
+000018b0: 616c 736f 2070 7574 0a63 6f6e 6669 6775  also put.configu
+000018c0: 7261 7469 6f6e 206f 7074 696f 6e73 2069  ration options i
+000018d0: 6e20 796f 7572 2070 726f 6a65 6374 202a  n your project *
+000018e0: 7365 7475 702e 6366 672a 2066 696c 652c  setup.cfg* file,
+000018f0: 206f 7220 6120 2e6e 6f73 6572 630a 6f72   or a .noserc.or
+00001900: 206e 6f73 652e 6366 6720 6669 6c65 2069   nose.cfg file i
+00001910: 6e20 796f 7572 2068 6f6d 6520 6469 7265  n your home dire
+00001920: 6374 6f72 792e 2049 6e20 616e 7920 6f66  ctory. In any of
+00001930: 2074 6865 7365 2073 7461 6e64 6172 6420   these standard 
+00001940: 696e 692d 0a73 7479 6c65 2063 6f6e 6669  ini-.style confi
+00001950: 6720 6669 6c65 732c 2079 6f75 2070 7574  g files, you put
+00001960: 2079 6f75 7220 6e6f 7365 7465 7374 7320   your nosetests 
+00001970: 636f 6e66 6967 7572 6174 696f 6e20 696e  configuration in
+00001980: 2061 0a22 5b6e 6f73 6574 6573 7473 5d22   a."[nosetests]"
+00001990: 2073 6563 7469 6f6e 2e20 4f70 7469 6f6e   section. Option
+000019a0: 7320 6172 6520 7468 6520 7361 6d65 2061  s are the same a
+000019b0: 7320 6f6e 2074 6865 2063 6f6d 6d61 6e64  s on the command
+000019c0: 206c 696e 652c 0a77 6974 6820 7468 6520   line,.with the 
+000019d0: 2d2d 2070 7265 6669 7820 7265 6d6f 7665  -- prefix remove
+000019e0: 642e 2046 6f72 206f 7074 696f 6e73 2074  d. For options t
+000019f0: 6861 7420 6172 6520 7369 6d70 6c65 2073  hat are simple s
+00001a00: 7769 7463 6865 732c 2079 6f75 0a6d 7573  witches, you.mus
+00001a10: 7420 7375 7070 6c79 2061 2076 616c 7565  t supply a value
+00001a20: 3a0a 0a20 2020 5b6e 6f73 6574 6573 7473  :..   [nosetests
+00001a30: 5d0a 2020 2076 6572 626f 7369 7479 3d33  ].   verbosity=3
+00001a40: 0a20 2020 7769 7468 2d64 6f63 7465 7374  .   with-doctest
+00001a50: 3d31 0a0a 416c 6c20 636f 6e66 6967 7572  =1..All configur
+00001a60: 6174 696f 6e20 6669 6c65 7320 7468 6174  ation files that
+00001a70: 2061 7265 2066 6f75 6e64 2077 696c 6c20   are found will 
+00001a80: 6265 206c 6f61 6465 6420 616e 6420 7468  be loaded and th
+00001a90: 6569 720a 6f70 7469 6f6e 7320 636f 6d62  eir.options comb
+00001aa0: 696e 6564 2e20 596f 7520 6361 6e20 6f76  ined. You can ov
+00001ab0: 6572 7269 6465 2074 6865 2073 7461 6e64  erride the stand
+00001ac0: 6172 6420 636f 6e66 6967 2066 696c 6520  ard config file 
+00001ad0: 6c6f 6164 696e 670a 7769 7468 2074 6865  loading.with the
+00001ae0: 2022 2d63 2220 6f70 7469 6f6e 2e0a 0a0a   "-c" option....
+00001af0: 5573 696e 6720 506c 7567 696e 730a 2d2d  Using Plugins.--
+00001b00: 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a 0a54 6865  -----------..The
+00001b10: 7265 2061 7265 206e 756d 6572 6f75 7320  re are numerous 
+00001b20: 6e6f 7365 2070 6c75 6769 6e73 2061 7661  nose plugins ava
+00001b30: 696c 6162 6c65 2076 6961 2065 6173 795f  ilable via easy_
+00001b40: 696e 7374 616c 6c20 616e 640a 656c 7365  install and.else
+00001b50: 7768 6572 652e 2054 6f20 7573 6520 6120  where. To use a 
+00001b60: 706c 7567 696e 2c20 6a75 7374 2069 6e73  plugin, just ins
+00001b70: 7461 6c6c 2069 742e 2054 6865 2070 6c75  tall it. The plu
+00001b80: 6769 6e20 7769 6c6c 2061 6464 0a63 6f6d  gin will add.com
+00001b90: 6d61 6e64 206c 696e 6520 6f70 7469 6f6e  mand line option
+00001ba0: 7320 746f 206e 6f73 6574 6573 7473 2e20  s to nosetests. 
+00001bb0: 546f 2076 6572 6966 7920 7468 6174 2074  To verify that t
+00001bc0: 6865 2070 6c75 6769 6e20 6973 0a69 6e73  he plugin is.ins
+00001bd0: 7461 6c6c 6564 2c20 7275 6e3a 0a0a 2020  talled, run:..  
+00001be0: 206e 6f73 6574 6573 7473 202d 2d70 6c75   nosetests --plu
+00001bf0: 6769 6e73 0a0a 596f 7520 6361 6e20 6164  gins..You can ad
+00001c00: 6420 2d76 206f 7220 2d76 7620 746f 2074  d -v or -vv to t
+00001c10: 6861 7420 636f 6d6d 616e 6420 746f 2073  hat command to s
+00001c20: 686f 7720 6d6f 7265 2069 6e66 6f72 6d61  how more informa
+00001c30: 7469 6f6e 2061 626f 7574 0a65 6163 6820  tion about.each 
+00001c40: 706c 7567 696e 2e0a 0a49 6620 796f 7520  plugin...If you 
+00001c50: 6172 6520 7275 6e6e 696e 6720 6e6f 7365  are running nose
+00001c60: 2e6d 6169 6e28 2920 6f72 206e 6f73 652e  .main() or nose.
+00001c70: 7275 6e28 2920 6672 6f6d 2061 2073 6372  run() from a scr
+00001c80: 6970 742c 2079 6f75 2063 616e 0a73 7065  ipt, you can.spe
+00001c90: 6369 6679 2061 206c 6973 7420 6f66 2070  cify a list of p
+00001ca0: 6c75 6769 6e73 2074 6f20 7573 6520 6279  lugins to use by
+00001cb0: 2070 6173 7369 6e67 2061 206c 6973 7420   passing a list 
+00001cc0: 6f66 2070 6c75 6769 6e73 2077 6974 6820  of plugins with 
+00001cd0: 7468 650a 706c 7567 696e 7320 6b65 7977  the.plugins keyw
+00001ce0: 6f72 6420 6172 6775 6d65 6e74 2e0a 0a0a  ord argument....
+00001cf0: 4f70 7469 6f6e 730a 2d2d 2d2d 2d2d 2d0a  Options.-------.
+00001d00: 0a2d 562c 202d 2d76 6572 7369 6f6e 0a0a  .-V, --version..
+00001d10: 2020 204f 7574 7075 7420 6e6f 7365 2076     Output nose v
+00001d20: 6572 7369 6f6e 2061 6e64 2065 7869 740a  ersion and exit.
+00001d30: 0a2d 702c 202d 2d70 6c75 6769 6e73 0a0a  .-p, --plugins..
+00001d40: 2020 204f 7574 7075 7420 6c69 7374 206f     Output list o
+00001d50: 6620 6176 6169 6c61 626c 6520 706c 7567  f available plug
+00001d60: 696e 7320 616e 6420 6578 6974 2e20 436f  ins and exit. Co
+00001d70: 6d62 696e 6520 7769 7468 2068 6967 6865  mbine with highe
+00001d80: 720a 2020 2076 6572 626f 7369 7479 2066  r.   verbosity f
+00001d90: 6f72 2067 7265 6174 6572 2064 6574 6169  or greater detai
+00001da0: 6c0a 0a2d 763d 4445 4641 554c 542c 202d  l..-v=DEFAULT, -
+00001db0: 2d76 6572 626f 7365 3d44 4546 4155 4c54  -verbose=DEFAULT
+00001dc0: 0a0a 2020 2042 6520 6d6f 7265 2076 6572  ..   Be more ver
+00001dd0: 626f 7365 2e20 5b4e 4f53 455f 5645 5242  bose. [NOSE_VERB
+00001de0: 4f53 455d 0a0a 2d2d 7665 7262 6f73 6974  OSE]..--verbosit
+00001df0: 793d 5645 5242 4f53 4954 590a 0a20 2020  y=VERBOSITY..   
+00001e00: 5365 7420 7665 7262 6f73 6974 793b 202d  Set verbosity; -
+00001e10: 2d76 6572 626f 7369 7479 3d32 2069 7320  -verbosity=2 is 
+00001e20: 7468 6520 7361 6d65 2061 7320 2d76 0a0a  the same as -v..
+00001e30: 2d71 3d44 4546 4155 4c54 2c20 2d2d 7175  -q=DEFAULT, --qu
+00001e40: 6965 743d 4445 4641 554c 540a 0a20 2020  iet=DEFAULT..   
+00001e50: 4265 206c 6573 7320 7665 7262 6f73 650a  Be less verbose.
+00001e60: 0a2d 633d 4649 4c45 532c 202d 2d63 6f6e  .-c=FILES, --con
+00001e70: 6669 673d 4649 4c45 530a 0a20 2020 4c6f  fig=FILES..   Lo
+00001e80: 6164 2063 6f6e 6669 6775 7261 7469 6f6e  ad configuration
+00001e90: 2066 726f 6d20 636f 6e66 6967 2066 696c   from config fil
+00001ea0: 6528 7329 2e20 4d61 7920 6265 2073 7065  e(s). May be spe
+00001eb0: 6369 6669 6564 206d 756c 7469 706c 650a  cified multiple.
+00001ec0: 2020 2074 696d 6573 3b20 696e 2074 6861     times; in tha
+00001ed0: 7420 6361 7365 2c20 616c 6c20 636f 6e66  t case, all conf
+00001ee0: 6967 2066 696c 6573 2077 696c 6c20 6265  ig files will be
+00001ef0: 206c 6f61 6465 6420 616e 6420 636f 6d62   loaded and comb
+00001f00: 696e 6564 0a0a 2d77 3d57 4845 5245 2c20  ined..-w=WHERE, 
+00001f10: 2d2d 7768 6572 653d 5748 4552 450a 0a20  --where=WHERE.. 
+00001f20: 2020 4c6f 6f6b 2066 6f72 2074 6573 7473    Look for tests
+00001f30: 2069 6e20 7468 6973 2064 6972 6563 746f   in this directo
+00001f40: 7279 2e20 4d61 7920 6265 2073 7065 6369  ry. May be speci
+00001f50: 6669 6564 206d 756c 7469 706c 6520 7469  fied multiple ti
+00001f60: 6d65 732e 0a20 2020 5468 6520 6669 7273  mes..   The firs
+00001f70: 7420 6469 7265 6374 6f72 7920 7061 7373  t directory pass
+00001f80: 6564 2077 696c 6c20 6265 2075 7365 6420  ed will be used 
+00001f90: 6173 2074 6865 2077 6f72 6b69 6e67 2064  as the working d
+00001fa0: 6972 6563 746f 7279 2c0a 2020 2069 6e20  irectory,.   in 
+00001fb0: 706c 6163 6520 6f66 2074 6865 2063 7572  place of the cur
+00001fc0: 7265 6e74 2077 6f72 6b69 6e67 2064 6972  rent working dir
+00001fd0: 6563 746f 7279 2c20 7768 6963 6820 6973  ectory, which is
+00001fe0: 2074 6865 2064 6566 6175 6c74 2e0a 2020   the default..  
+00001ff0: 204f 7468 6572 7320 7769 6c6c 2062 6520   Others will be 
+00002000: 6164 6465 6420 746f 2074 6865 206c 6973  added to the lis
+00002010: 7420 6f66 2074 6573 7473 2074 6f20 6578  t of tests to ex
+00002020: 6563 7574 652e 205b 4e4f 5345 5f57 4845  ecute. [NOSE_WHE
+00002030: 5245 5d0a 0a2d 2d70 7933 7768 6572 653d  RE]..--py3where=
+00002040: 5059 3357 4845 5245 0a0a 2020 204c 6f6f  PY3WHERE..   Loo
+00002050: 6b20 666f 7220 7465 7374 7320 696e 2074  k for tests in t
+00002060: 6869 7320 6469 7265 6374 6f72 7920 756e  his directory un
+00002070: 6465 7220 5079 7468 6f6e 2033 2e78 2e20  der Python 3.x. 
+00002080: 4675 6e63 7469 6f6e 7320 7468 650a 2020  Functions the.  
+00002090: 2073 616d 6520 6173 2027 7768 6572 6527   same as 'where'
+000020a0: 2c20 6275 7420 6f6e 6c79 2061 7070 6c69  , but only appli
+000020b0: 6573 2069 6620 7275 6e6e 696e 6720 756e  es if running un
+000020c0: 6465 7220 5079 7468 6f6e 2033 2e78 206f  der Python 3.x o
+000020d0: 720a 2020 2061 626f 7665 2e20 204e 6f74  r.   above.  Not
+000020e0: 6520 7468 6174 2c20 6966 2070 7265 7365  e that, if prese
+000020f0: 6e74 2075 6e64 6572 2033 2e78 2c20 7468  nt under 3.x, th
+00002100: 6973 206f 7074 696f 6e20 636f 6d70 6c65  is option comple
+00002110: 7465 6c79 0a20 2020 7265 706c 6163 6573  tely.   replaces
+00002120: 2061 6e79 2064 6972 6563 746f 7269 6573   any directories
+00002130: 2073 7065 6369 6669 6564 2077 6974 6820   specified with 
+00002140: 2777 6865 7265 272c 2073 6f20 7468 6520  'where', so the 
+00002150: 2777 6865 7265 270a 2020 206f 7074 696f  'where'.   optio
+00002160: 6e20 6265 636f 6d65 7320 696e 6566 6665  n becomes ineffe
+00002170: 6374 6976 652e 205b 4e4f 5345 5f50 5933  ctive. [NOSE_PY3
+00002180: 5748 4552 455d 0a0a 2d6d 3d52 4547 4558  WHERE]..-m=REGEX
+00002190: 2c20 2d2d 6d61 7463 683d 5245 4745 582c  , --match=REGEX,
+000021a0: 202d 2d74 6573 746d 6174 6368 3d52 4547   --testmatch=REG
+000021b0: 4558 0a0a 2020 2046 696c 6573 2c20 6469  EX..   Files, di
+000021c0: 7265 6374 6f72 6965 732c 2066 756e 6374  rectories, funct
+000021d0: 696f 6e20 6e61 6d65 732c 2061 6e64 2063  ion names, and c
+000021e0: 6c61 7373 206e 616d 6573 2074 6861 7420  lass names that 
+000021f0: 6d61 7463 6820 7468 6973 0a20 2020 7265  match this.   re
+00002200: 6775 6c61 7220 6578 7072 6573 7369 6f6e  gular expression
+00002210: 2061 7265 2063 6f6e 7369 6465 7265 6420   are considered 
+00002220: 7465 7374 732e 2020 4465 6661 756c 743a  tests.  Default:
+00002230: 0a20 2020 283f 3a5e 7c5b 625f 2e2f 2d5d  .   (?:^|[b_./-]
+00002240: 295b 5474 5d65 7374 205b 4e4f 5345 5f54  )[Tt]est [NOSE_T
+00002250: 4553 544d 4154 4348 5d0a 0a2d 2d74 6573  ESTMATCH]..--tes
+00002260: 7473 3d4e 414d 4553 0a0a 2020 2052 756e  ts=NAMES..   Run
+00002270: 2074 6865 7365 2074 6573 7473 2028 636f   these tests (co
+00002280: 6d6d 612d 7365 7061 7261 7465 6420 6c69  mma-separated li
+00002290: 7374 292e 2054 6869 7320 6172 6775 6d65  st). This argume
+000022a0: 6e74 2069 7320 7573 6566 756c 0a20 2020  nt is useful.   
+000022b0: 6d61 696e 6c79 2066 726f 6d20 636f 6e66  mainly from conf
+000022c0: 6967 7572 6174 696f 6e20 6669 6c65 733b  iguration files;
+000022d0: 206f 6e20 7468 6520 636f 6d6d 616e 6420   on the command 
+000022e0: 6c69 6e65 2c20 6a75 7374 2070 6173 7320  line, just pass 
+000022f0: 7468 650a 2020 2074 6573 7473 2074 6f20  the.   tests to 
+00002300: 7275 6e20 6173 2061 6464 6974 696f 6e61  run as additiona
+00002310: 6c20 6172 6775 6d65 6e74 7320 7769 7468  l arguments with
+00002320: 206e 6f20 7377 6974 6368 2e0a 0a2d 6c3d   no switch...-l=
+00002330: 4445 4641 554c 542c 202d 2d64 6562 7567  DEFAULT, --debug
+00002340: 3d44 4546 4155 4c54 0a0a 2020 2041 6374  =DEFAULT..   Act
+00002350: 6976 6174 6520 6465 6275 6720 6c6f 6767  ivate debug logg
+00002360: 696e 6720 666f 7220 6f6e 6520 6f72 206d  ing for one or m
+00002370: 6f72 6520 7379 7374 656d 732e 2041 7661  ore systems. Ava
+00002380: 696c 6162 6c65 2064 6562 7567 0a20 2020  ilable debug.   
+00002390: 6c6f 6767 6572 733a 206e 6f73 652c 206e  loggers: nose, n
+000023a0: 6f73 652e 696d 706f 7274 6572 2c20 6e6f  ose.importer, no
+000023b0: 7365 2e69 6e73 7065 6374 6f72 2c20 6e6f  se.inspector, no
+000023c0: 7365 2e70 6c75 6769 6e73 2c0a 2020 206e  se.plugins,.   n
+000023d0: 6f73 652e 7265 7375 6c74 2061 6e64 206e  ose.result and n
+000023e0: 6f73 652e 7365 6c65 6374 6f72 2e20 5365  ose.selector. Se
+000023f0: 7061 7261 7465 206d 756c 7469 706c 6520  parate multiple 
+00002400: 6e61 6d65 7320 7769 7468 2061 0a20 2020  names with a.   
+00002410: 636f 6d6d 612e 0a0a 2d2d 6465 6275 672d  comma...--debug-
+00002420: 6c6f 673d 4649 4c45 0a0a 2020 204c 6f67  log=FILE..   Log
+00002430: 2064 6562 7567 206d 6573 7361 6765 7320   debug messages 
+00002440: 746f 2074 6869 7320 6669 6c65 2028 6465  to this file (de
+00002450: 6661 756c 743a 2073 7973 2e73 7464 6572  fault: sys.stder
+00002460: 7229 0a0a 2d2d 6c6f 6767 696e 672d 636f  r)..--logging-co
+00002470: 6e66 6967 3d46 494c 452c 202d 2d6c 6f67  nfig=FILE, --log
+00002480: 2d63 6f6e 6669 673d 4649 4c45 0a0a 2020  -config=FILE..  
+00002490: 204c 6f61 6420 6c6f 6767 696e 6720 636f   Load logging co
+000024a0: 6e66 6967 2066 726f 6d20 7468 6973 2066  nfig from this f
+000024b0: 696c 6520 2d2d 2062 7970 6173 7365 7320  ile -- bypasses 
+000024c0: 616c 6c20 6f74 6865 7220 6c6f 6767 696e  all other loggin
+000024d0: 670a 2020 2063 6f6e 6669 6720 7365 7474  g.   config sett
+000024e0: 696e 6773 2e0a 0a2d 493d 5245 4745 582c  ings...-I=REGEX,
+000024f0: 202d 2d69 676e 6f72 652d 6669 6c65 733d   --ignore-files=
+00002500: 5245 4745 580a 0a20 2020 436f 6d70 6c65  REGEX..   Comple
+00002510: 7465 6c79 2069 676e 6f72 6520 616e 7920  tely ignore any 
+00002520: 6669 6c65 2074 6861 7420 6d61 7463 6865  file that matche
+00002530: 7320 7468 6973 2072 6567 756c 6172 2065  s this regular e
+00002540: 7870 7265 7373 696f 6e2e 0a20 2020 5461  xpression..   Ta
+00002550: 6b65 7320 7072 6563 6564 656e 6365 206f  kes precedence o
+00002560: 7665 7220 616e 7920 6f74 6865 7220 7365  ver any other se
+00002570: 7474 696e 6773 206f 7220 706c 7567 696e  ttings or plugin
+00002580: 732e 2053 7065 6369 6679 696e 670a 2020  s. Specifying.  
+00002590: 2074 6869 7320 6f70 7469 6f6e 2077 696c   this option wil
+000025a0: 6c20 7265 706c 6163 6520 7468 6520 6465  l replace the de
+000025b0: 6661 756c 7420 7365 7474 696e 672e 2053  fault setting. S
+000025c0: 7065 6369 6679 2074 6869 7320 6f70 7469  pecify this opti
+000025d0: 6f6e 0a20 2020 6d75 6c74 6970 6c65 2074  on.   multiple t
+000025e0: 696d 6573 2074 6f20 6164 6420 6d6f 7265  imes to add more
+000025f0: 2072 6567 756c 6172 2065 7870 7265 7373   regular express
+00002600: 696f 6e73 205b 4e4f 5345 5f49 474e 4f52  ions [NOSE_IGNOR
+00002610: 455f 4649 4c45 535d 0a0a 2d65 3d52 4547  E_FILES]..-e=REG
+00002620: 4558 2c20 2d2d 6578 636c 7564 653d 5245  EX, --exclude=RE
+00002630: 4745 580a 0a20 2020 446f 206e 6f74 2072  GEX..   Do not r
+00002640: 756e 2074 6573 7473 2074 6861 7420 6d61  un tests that ma
+00002650: 7463 6820 7265 6775 6c61 7220 6578 7072  tch regular expr
+00002660: 6573 7369 6f6e 205b 4e4f 5345 5f45 5843  ession [NOSE_EXC
+00002670: 4c55 4445 5d0a 0a2d 693d 5245 4745 582c  LUDE]..-i=REGEX,
+00002680: 202d 2d69 6e63 6c75 6465 3d52 4547 4558   --include=REGEX
+00002690: 0a0a 2020 2054 6869 7320 7265 6775 6c61  ..   This regula
+000026a0: 7220 6578 7072 6573 7369 6f6e 2077 696c  r expression wil
+000026b0: 6c20 6265 2061 7070 6c69 6564 2074 6f20  l be applied to 
+000026c0: 6669 6c65 732c 2064 6972 6563 746f 7269  files, directori
+000026d0: 6573 2c0a 2020 2066 756e 6374 696f 6e20  es,.   function 
+000026e0: 6e61 6d65 732c 2061 6e64 2063 6c61 7373  names, and class
+000026f0: 206e 616d 6573 2066 6f72 2061 2063 6861   names for a cha
+00002700: 6e63 6520 746f 2069 6e63 6c75 6465 2061  nce to include a
+00002710: 6464 6974 696f 6e61 6c0a 2020 2074 6573  dditional.   tes
+00002720: 7473 2074 6861 7420 646f 206e 6f74 206d  ts that do not m
+00002730: 6174 6368 2054 4553 544d 4154 4348 2e20  atch TESTMATCH. 
+00002740: 2053 7065 6369 6679 2074 6869 7320 6f70   Specify this op
+00002750: 7469 6f6e 206d 756c 7469 706c 650a 2020  tion multiple.  
+00002760: 2074 696d 6573 2074 6f20 6164 6420 6d6f   times to add mo
+00002770: 7265 2072 6567 756c 6172 2065 7870 7265  re regular expre
+00002780: 7373 696f 6e73 205b 4e4f 5345 5f49 4e43  ssions [NOSE_INC
+00002790: 4c55 4445 5d0a 0a2d 782c 202d 2d73 746f  LUDE]..-x, --sto
+000027a0: 700a 0a20 2020 5374 6f70 2072 756e 6e69  p..   Stop runni
+000027b0: 6e67 2074 6573 7473 2061 6674 6572 2074  ng tests after t
+000027c0: 6865 2066 6972 7374 2065 7272 6f72 206f  he first error o
+000027d0: 7220 6661 696c 7572 650a 0a2d 502c 202d  r failure..-P, -
+000027e0: 2d6e 6f2d 7061 7468 2d61 646a 7573 746d  -no-path-adjustm
+000027f0: 656e 740a 0a20 2020 446f 206e 6f74 206d  ent..   Do not m
+00002800: 616b 6520 616e 7920 6368 616e 6765 7320  ake any changes 
+00002810: 746f 2073 7973 2e70 6174 6820 7768 656e  to sys.path when
+00002820: 206c 6f61 6469 6e67 2074 6573 7473 205b   loading tests [
+00002830: 4e4f 5345 5f4e 4f50 4154 485d 0a0a 2d2d  NOSE_NOPATH]..--
+00002840: 6578 650a 0a20 2020 4c6f 6f6b 2066 6f72  exe..   Look for
+00002850: 2074 6573 7473 2069 6e20 7079 7468 6f6e   tests in python
+00002860: 206d 6f64 756c 6573 2074 6861 7420 6172   modules that ar
+00002870: 6520 6578 6563 7574 6162 6c65 2e20 4e6f  e executable. No
+00002880: 726d 616c 0a20 2020 6265 6861 7669 6f72  rmal.   behavior
+00002890: 2069 7320 746f 2065 7863 6c75 6465 2065   is to exclude e
+000028a0: 7865 6375 7461 626c 6520 6d6f 6475 6c65  xecutable module
+000028b0: 732c 2073 696e 6365 2074 6865 7920 6d61  s, since they ma
+000028c0: 7920 6e6f 7420 6265 0a20 2020 696d 706f  y not be.   impo
+000028d0: 7274 2d73 6166 6520 5b4e 4f53 455f 494e  rt-safe [NOSE_IN
+000028e0: 434c 5544 455f 4558 455d 0a0a 2d2d 6e6f  CLUDE_EXE]..--no
+000028f0: 6578 650a 0a20 2020 444f 204e 4f54 206c  exe..   DO NOT l
+00002900: 6f6f 6b20 666f 7220 7465 7374 7320 696e  ook for tests in
+00002910: 2070 7974 686f 6e20 6d6f 6475 6c65 7320   python modules 
+00002920: 7468 6174 2061 7265 2065 7865 6375 7461  that are executa
+00002930: 626c 652e 2028 5468 650a 2020 2064 6566  ble. (The.   def
+00002940: 6175 6c74 206f 6e20 7468 6520 7769 6e64  ault on the wind
+00002950: 6f77 7320 706c 6174 666f 726d 2069 7320  ows platform is 
+00002960: 746f 2064 6f20 736f 2e29 0a0a 2d2d 7472  to do so.)..--tr
+00002970: 6176 6572 7365 2d6e 616d 6573 7061 6365  averse-namespace
+00002980: 0a0a 2020 2054 7261 7665 7273 6520 7468  ..   Traverse th
+00002990: 726f 7567 6820 616c 6c20 7061 7468 2065  rough all path e
+000029a0: 6e74 7269 6573 206f 6620 6120 6e61 6d65  ntries of a name
+000029b0: 7370 6163 6520 7061 636b 6167 650a 0a2d  space package..-
+000029c0: 2d66 6972 7374 2d70 6163 6b61 6765 2d77  -first-package-w
+000029d0: 696e 732c 202d 2d66 6972 7374 2d70 6b67  ins, --first-pkg
+000029e0: 2d77 696e 732c 202d 2d31 7374 2d70 6b67  -wins, --1st-pkg
+000029f0: 2d77 696e 730a 0a20 2020 5468 6520 6e6f  -wins..   The no
+00002a00: 7365 2069 6d70 6f72 7465 7220 7769 6c6c  se importer will
+00002a10: 206e 6f72 6d61 6c6c 7920 6576 6963 7420   normally evict 
+00002a20: 6120 7061 636b 6167 6520 6672 6f6d 2073  a package from s
+00002a30: 7973 2e6d 6f64 756c 6573 2069 660a 2020  ys.modules if.  
+00002a40: 2069 7420 7365 6573 2061 2070 6163 6b61   it sees a packa
+00002a50: 6765 2077 6974 6820 7468 6520 7361 6d65  ge with the same
+00002a60: 206e 616d 6520 696e 2061 2064 6966 6665   name in a diffe
+00002a70: 7265 6e74 206c 6f63 6174 696f 6e2e 2053  rent location. S
+00002a80: 6574 0a20 2020 7468 6973 206f 7074 696f  et.   this optio
+00002a90: 6e20 746f 2064 6973 6162 6c65 2074 6861  n to disable tha
+00002aa0: 7420 6265 6861 7669 6f72 2e0a 0a2d 2d6e  t behavior...--n
+00002ab0: 6f2d 6279 7465 2d63 6f6d 7069 6c65 0a0a  o-byte-compile..
+00002ac0: 2020 2050 7265 7665 6e74 206e 6f73 6520     Prevent nose 
+00002ad0: 6672 6f6d 2062 7974 652d 636f 6d70 696c  from byte-compil
+00002ae0: 696e 6720 7468 6520 736f 7572 6365 2069  ing the source i
+00002af0: 6e74 6f20 2e70 7963 2066 696c 6573 2077  nto .pyc files w
+00002b00: 6869 6c65 0a20 2020 6e6f 7365 2069 7320  hile.   nose is 
+00002b10: 7363 616e 6e69 6e67 2066 6f72 2061 6e64  scanning for and
+00002b20: 2072 756e 6e69 6e67 2074 6573 7473 2e0a   running tests..
+00002b30: 0a2d 613d 4154 5452 2c20 2d2d 6174 7472  .-a=ATTR, --attr
+00002b40: 3d41 5454 520a 0a20 2020 5275 6e20 6f6e  =ATTR..   Run on
+00002b50: 6c79 2074 6573 7473 2074 6861 7420 6861  ly tests that ha
+00002b60: 7665 2061 7474 7269 6275 7465 7320 7370  ve attributes sp
+00002b70: 6563 6966 6965 6420 6279 2041 5454 5220  ecified by ATTR 
+00002b80: 5b4e 4f53 455f 4154 5452 5d0a 0a2d 413d  [NOSE_ATTR]..-A=
+00002b90: 4558 5052 2c20 2d2d 6576 616c 2d61 7474  EXPR, --eval-att
+00002ba0: 723d 4558 5052 0a0a 2020 2052 756e 206f  r=EXPR..   Run o
+00002bb0: 6e6c 7920 7465 7374 7320 666f 7220 7768  nly tests for wh
+00002bc0: 6f73 6520 6174 7472 6962 7574 6573 2074  ose attributes t
+00002bd0: 6865 2050 7974 686f 6e20 6578 7072 6573  he Python expres
+00002be0: 7369 6f6e 2045 5850 520a 2020 2065 7661  sion EXPR.   eva
+00002bf0: 6c75 6174 6573 2074 6f20 5472 7565 205b  luates to True [
+00002c00: 4e4f 5345 5f45 5641 4c5f 4154 5452 5d0a  NOSE_EVAL_ATTR].
+00002c10: 0a2d 732c 202d 2d6e 6f63 6170 7475 7265  .-s, --nocapture
+00002c20: 0a0a 2020 2044 6f20 6e6f 7420 6361 7074  ..   Do not capt
+00002c30: 7572 6520 7374 646f 7574 2028 616e 7920  ure stdout (any 
+00002c40: 7374 646f 7574 206f 7574 7075 7420 7769  stdout output wi
+00002c50: 6c6c 2062 6520 7072 696e 7465 640a 2020  ll be printed.  
+00002c60: 2069 6d6d 6564 6961 7465 6c79 2920 5b4e   immediately) [N
+00002c70: 4f53 455f 4e4f 4341 5054 5552 455d 0a0a  OSE_NOCAPTURE]..
+00002c80: 2d2d 6e6f 6c6f 6763 6170 7475 7265 0a0a  --nologcapture..
+00002c90: 2020 2044 6973 6162 6c65 206c 6f67 6769     Disable loggi
+00002ca0: 6e67 2063 6170 7475 7265 2070 6c75 6769  ng capture plugi
+00002cb0: 6e2e 204c 6f67 6769 6e67 2063 6f6e 6669  n. Logging confi
+00002cc0: 6775 7261 7469 6f6e 2077 696c 6c20 6265  guration will be
+00002cd0: 206c 6566 740a 2020 2069 6e74 6163 742e   left.   intact.
+00002ce0: 205b 4e4f 5345 5f4e 4f4c 4f47 4341 5054   [NOSE_NOLOGCAPT
+00002cf0: 5552 455d 0a0a 2d2d 6c6f 6767 696e 672d  URE]..--logging-
+00002d00: 666f 726d 6174 3d46 4f52 4d41 540a 0a20  format=FORMAT.. 
+00002d10: 2020 5370 6563 6966 7920 6375 7374 6f6d    Specify custom
+00002d20: 2066 6f72 6d61 7420 746f 2070 7269 6e74   format to print
+00002d30: 2073 7461 7465 6d65 6e74 732e 2055 7365   statements. Use
+00002d40: 7320 7468 6520 7361 6d65 2066 6f72 6d61  s the same forma
+00002d50: 7420 6173 0a20 2020 7573 6564 2062 7920  t as.   used by 
+00002d60: 7374 616e 6461 7264 206c 6f67 6769 6e67  standard logging
+00002d70: 2068 616e 646c 6572 732e 205b 4e4f 5345   handlers. [NOSE
+00002d80: 5f4c 4f47 464f 524d 4154 5d0a 0a2d 2d6c  _LOGFORMAT]..--l
+00002d90: 6f67 6769 6e67 2d64 6174 6566 6d74 3d46  ogging-datefmt=F
+00002da0: 4f52 4d41 540a 0a20 2020 5370 6563 6966  ORMAT..   Specif
+00002db0: 7920 6375 7374 6f6d 2064 6174 652f 7469  y custom date/ti
+00002dc0: 6d65 2066 6f72 6d61 7420 746f 2070 7269  me format to pri
+00002dd0: 6e74 2073 7461 7465 6d65 6e74 732e 2055  nt statements. U
+00002de0: 7365 7320 7468 6520 7361 6d65 0a20 2020  ses the same.   
+00002df0: 666f 726d 6174 2061 7320 7573 6564 2062  format as used b
+00002e00: 7920 7374 616e 6461 7264 206c 6f67 6769  y standard loggi
+00002e10: 6e67 2068 616e 646c 6572 732e 205b 4e4f  ng handlers. [NO
+00002e20: 5345 5f4c 4f47 4441 5445 464d 545d 0a0a  SE_LOGDATEFMT]..
+00002e30: 2d2d 6c6f 6767 696e 672d 6669 6c74 6572  --logging-filter
+00002e40: 3d46 494c 5445 520a 0a20 2020 5370 6563  =FILTER..   Spec
+00002e50: 6966 7920 7768 6963 6820 7374 6174 656d  ify which statem
+00002e60: 656e 7473 2074 6f20 6669 6c74 6572 2069  ents to filter i
+00002e70: 6e2f 6f75 742e 2042 7920 6465 6661 756c  n/out. By defaul
+00002e80: 742c 2065 7665 7279 7468 696e 670a 2020  t, everything.  
+00002e90: 2069 7320 6361 7074 7572 6564 2e20 4966   is captured. If
+00002ea0: 2074 6865 206f 7574 7075 7420 6973 2074   the output is t
+00002eb0: 6f6f 2076 6572 626f 7365 2c20 7573 6520  oo verbose, use 
+00002ec0: 7468 6973 206f 7074 696f 6e20 746f 0a20  this option to. 
+00002ed0: 2020 6669 6c74 6572 206f 7574 206e 6565    filter out nee
+00002ee0: 646c 6573 7320 6f75 7470 7574 2e20 4578  dless output. Ex
+00002ef0: 616d 706c 653a 2066 696c 7465 723d 666f  ample: filter=fo
+00002f00: 6f20 7769 6c6c 2063 6170 7475 7265 0a20  o will capture. 
+00002f10: 2020 7374 6174 656d 656e 7473 2069 7373    statements iss
+00002f20: 7565 6420 4f4e 4c59 2074 6f20 2066 6f6f  ued ONLY to  foo
+00002f30: 206f 7220 666f 6f2e 7768 6174 2e65 7665   or foo.what.eve
+00002f40: 722e 7375 6220 6275 7420 6e6f 7420 666f  r.sub but not fo
+00002f50: 6f62 6172 0a20 2020 6f72 206f 7468 6572  obar.   or other
+00002f60: 206c 6f67 6765 722e 2053 7065 6369 6679   logger. Specify
+00002f70: 206d 756c 7469 706c 6520 6c6f 6767 6572   multiple logger
+00002f80: 7320 7769 7468 2063 6f6d 6d61 3a0a 2020  s with comma:.  
+00002f90: 2066 696c 7465 723d 666f 6f2c 6261 722c   filter=foo,bar,
+00002fa0: 6261 7a2e 2049 6620 616e 7920 6c6f 6767  baz. If any logg
+00002fb0: 6572 206e 616d 6520 6973 2070 7265 6669  er name is prefi
+00002fc0: 7865 6420 7769 7468 2061 206d 696e 7573  xed with a minus
+00002fd0: 2c20 6567 0a20 2020 6669 6c74 6572 3d2d  , eg.   filter=-
+00002fe0: 666f 6f2c 2069 7420 7769 6c6c 2062 6520  foo, it will be 
+00002ff0: 6578 636c 7564 6564 2072 6174 6865 7220  excluded rather 
+00003000: 7468 616e 2069 6e63 6c75 6465 642e 2044  than included. D
+00003010: 6566 6175 6c74 3a0a 2020 2065 7863 6c75  efault:.   exclu
+00003020: 6465 206c 6f67 6769 6e67 206d 6573 7361  de logging messa
+00003030: 6765 7320 6672 6f6d 206e 6f73 6520 6974  ges from nose it
+00003040: 7365 6c66 2028 2d6e 6f73 6529 2e20 5b4e  self (-nose). [N
+00003050: 4f53 455f 4c4f 4746 494c 5445 525d 0a0a  OSE_LOGFILTER]..
+00003060: 2d2d 6c6f 6767 696e 672d 636c 6561 722d  --logging-clear-
+00003070: 6861 6e64 6c65 7273 0a0a 2020 2043 6c65  handlers..   Cle
+00003080: 6172 2061 6c6c 206f 7468 6572 206c 6f67  ar all other log
+00003090: 6769 6e67 2068 616e 646c 6572 730a 0a2d  ging handlers..-
+000030a0: 2d6c 6f67 6769 6e67 2d6c 6576 656c 3d44  -logging-level=D
+000030b0: 4546 4155 4c54 0a0a 2020 2053 6574 2074  EFAULT..   Set t
+000030c0: 6865 206c 6f67 206c 6576 656c 2074 6f20  he log level to 
+000030d0: 6361 7074 7572 650a 0a2d 2d77 6974 682d  capture..--with-
+000030e0: 636f 7665 7261 6765 0a0a 2020 2045 6e61  coverage..   Ena
+000030f0: 626c 6520 706c 7567 696e 2043 6f76 6572  ble plugin Cover
+00003100: 6167 653a 2041 6374 6976 6174 6520 6120  age: Activate a 
+00003110: 636f 7665 7261 6765 2072 6570 6f72 7420  coverage report 
+00003120: 7573 696e 6720 7468 650a 2020 204e 6564  using the.   Ned
+00003130: 2042 6174 6368 656c 6465 7220 636f 7665   Batchelder cove
+00003140: 7261 6765 206d 6f64 756c 652e 205b 4e4f  rage module. [NO
+00003150: 5345 5f57 4954 485f 434f 5645 5241 4745  SE_WITH_COVERAGE
+00003160: 5d0a 0a2d 2d63 6f76 6572 2d70 6163 6b61  ]..--cover-packa
+00003170: 6765 3d50 4143 4b41 4745 0a0a 2020 2052  ge=PACKAGE..   R
+00003180: 6573 7472 6963 7420 636f 7665 7261 6765  estrict coverage
+00003190: 206f 7574 7075 7420 746f 2073 656c 6563   output to selec
+000031a0: 7465 6420 7061 636b 6167 6573 205b 4e4f  ted packages [NO
+000031b0: 5345 5f43 4f56 4552 5f50 4143 4b41 4745  SE_COVER_PACKAGE
+000031c0: 5d0a 0a2d 2d63 6f76 6572 2d65 7261 7365  ]..--cover-erase
+000031d0: 0a0a 2020 2045 7261 7365 2070 7265 7669  ..   Erase previ
+000031e0: 6f75 736c 7920 636f 6c6c 6563 7465 6420  ously collected 
+000031f0: 636f 7665 7261 6765 2073 7461 7469 7374  coverage statist
+00003200: 6963 7320 6265 666f 7265 2072 756e 0a0a  ics before run..
+00003210: 2d2d 636f 7665 722d 7465 7374 730a 0a20  --cover-tests.. 
+00003220: 2020 496e 636c 7564 6520 7465 7374 206d    Include test m
+00003230: 6f64 756c 6573 2069 6e20 636f 7665 7261  odules in covera
+00003240: 6765 2072 6570 6f72 7420 5b4e 4f53 455f  ge report [NOSE_
+00003250: 434f 5645 525f 5445 5354 535d 0a0a 2d2d  COVER_TESTS]..--
+00003260: 636f 7665 722d 6d69 6e2d 7065 7263 656e  cover-min-percen
+00003270: 7461 6765 3d44 4546 4155 4c54 0a0a 2020  tage=DEFAULT..  
+00003280: 204d 696e 696d 756d 2070 6572 6365 6e74   Minimum percent
+00003290: 6167 6520 6f66 2063 6f76 6572 6167 6520  age of coverage 
+000032a0: 666f 7220 7465 7374 7320 746f 2070 6173  for tests to pas
+000032b0: 730a 2020 205b 4e4f 5345 5f43 4f56 4552  s.   [NOSE_COVER
+000032c0: 5f4d 494e 5f50 4552 4345 4e54 4147 455d  _MIN_PERCENTAGE]
+000032d0: 0a0a 2d2d 636f 7665 722d 696e 636c 7573  ..--cover-inclus
+000032e0: 6976 650a 0a20 2020 496e 636c 7564 6520  ive..   Include 
+000032f0: 616c 6c20 7079 7468 6f6e 2066 696c 6573  all python files
+00003300: 2075 6e64 6572 2077 6f72 6b69 6e67 2064   under working d
+00003310: 6972 6563 746f 7279 2069 6e20 636f 7665  irectory in cove
+00003320: 7261 6765 0a20 2020 7265 706f 7274 2e20  rage.   report. 
+00003330: 2055 7365 6675 6c20 666f 7220 6469 7363   Useful for disc
+00003340: 6f76 6572 696e 6720 686f 6c65 7320 696e  overing holes in
+00003350: 2074 6573 7420 636f 7665 7261 6765 2069   test coverage i
+00003360: 6620 6e6f 7420 616c 6c0a 2020 2066 696c  f not all.   fil
+00003370: 6573 2061 7265 2069 6d70 6f72 7465 6420  es are imported 
+00003380: 6279 2074 6865 2074 6573 7420 7375 6974  by the test suit
+00003390: 652e 205b 4e4f 5345 5f43 4f56 4552 5f49  e. [NOSE_COVER_I
+000033a0: 4e43 4c55 5349 5645 5d0a 0a2d 2d63 6f76  NCLUSIVE]..--cov
+000033b0: 6572 2d68 746d 6c0a 0a20 2020 5072 6f64  er-html..   Prod
+000033c0: 7563 6520 4854 4d4c 2063 6f76 6572 6167  uce HTML coverag
+000033d0: 6520 696e 666f 726d 6174 696f 6e0a 0a2d  e information..-
+000033e0: 2d63 6f76 6572 2d68 746d 6c2d 6469 723d  -cover-html-dir=
+000033f0: 4449 520a 0a20 2020 5072 6f64 7563 6520  DIR..   Produce 
+00003400: 4854 4d4c 2063 6f76 6572 6167 6520 696e  HTML coverage in
+00003410: 666f 726d 6174 696f 6e20 696e 2064 6972  formation in dir
+00003420: 0a0a 2d2d 636f 7665 722d 6272 616e 6368  ..--cover-branch
+00003430: 6573 0a0a 2020 2049 6e63 6c75 6465 2062  es..   Include b
+00003440: 7261 6e63 6820 636f 7665 7261 6765 2069  ranch coverage i
+00003450: 6e20 636f 7665 7261 6765 2072 6570 6f72  n coverage repor
+00003460: 7420 5b4e 4f53 455f 434f 5645 525f 4252  t [NOSE_COVER_BR
+00003470: 414e 4348 4553 5d0a 0a2d 2d63 6f76 6572  ANCHES]..--cover
+00003480: 2d78 6d6c 0a0a 2020 2050 726f 6475 6365  -xml..   Produce
+00003490: 2058 4d4c 2063 6f76 6572 6167 6520 696e   XML coverage in
+000034a0: 666f 726d 6174 696f 6e0a 0a2d 2d63 6f76  formation..--cov
+000034b0: 6572 2d78 6d6c 2d66 696c 653d 4649 4c45  er-xml-file=FILE
+000034c0: 0a0a 2020 2050 726f 6475 6365 2058 4d4c  ..   Produce XML
+000034d0: 2063 6f76 6572 6167 6520 696e 666f 726d   coverage inform
+000034e0: 6174 696f 6e20 696e 2066 696c 650a 0a2d  ation in file..-
+000034f0: 2d70 6462 0a0a 2020 2044 726f 7020 696e  -pdb..   Drop in
+00003500: 746f 2064 6562 7567 6765 7220 6f6e 2066  to debugger on f
+00003510: 6169 6c75 7265 7320 6f72 2065 7272 6f72  ailures or error
+00003520: 730a 0a2d 2d70 6462 2d66 6169 6c75 7265  s..--pdb-failure
+00003530: 730a 0a20 2020 4472 6f70 2069 6e74 6f20  s..   Drop into 
+00003540: 6465 6275 6767 6572 206f 6e20 6661 696c  debugger on fail
+00003550: 7572 6573 0a0a 2d2d 7064 622d 6572 726f  ures..--pdb-erro
+00003560: 7273 0a0a 2020 2044 726f 7020 696e 746f  rs..   Drop into
+00003570: 2064 6562 7567 6765 7220 6f6e 2065 7272   debugger on err
+00003580: 6f72 730a 0a2d 2d6e 6f2d 6465 7072 6563  ors..--no-deprec
+00003590: 6174 6564 0a0a 2020 2044 6973 6162 6c65  ated..   Disable
+000035a0: 2073 7065 6369 616c 2068 616e 646c 696e   special handlin
+000035b0: 6720 6f66 2044 6570 7265 6361 7465 6454  g of DeprecatedT
+000035c0: 6573 7420 6578 6365 7074 696f 6e73 2e0a  est exceptions..
+000035d0: 0a2d 2d77 6974 682d 646f 6374 6573 740a  .--with-doctest.
+000035e0: 0a20 2020 456e 6162 6c65 2070 6c75 6769  .   Enable plugi
+000035f0: 6e20 446f 6374 6573 743a 2041 6374 6976  n Doctest: Activ
+00003600: 6174 6520 646f 6374 6573 7420 706c 7567  ate doctest plug
+00003610: 696e 2074 6f20 6669 6e64 2061 6e64 2072  in to find and r
+00003620: 756e 0a20 2020 646f 6374 6573 7473 2069  un.   doctests i
+00003630: 6e20 6e6f 6e2d 7465 7374 206d 6f64 756c  n non-test modul
+00003640: 6573 2e20 5b4e 4f53 455f 5749 5448 5f44  es. [NOSE_WITH_D
+00003650: 4f43 5445 5354 5d0a 0a2d 2d64 6f63 7465  OCTEST]..--docte
+00003660: 7374 2d74 6573 7473 0a0a 2020 2041 6c73  st-tests..   Als
+00003670: 6f20 6c6f 6f6b 2066 6f72 2064 6f63 7465  o look for docte
+00003680: 7374 7320 696e 2074 6573 7420 6d6f 6475  sts in test modu
+00003690: 6c65 732e 204e 6f74 6520 7468 6174 2063  les. Note that c
+000036a0: 6c61 7373 6573 2c20 6d65 7468 6f64 730a  lasses, methods.
+000036b0: 2020 2061 6e64 2066 756e 6374 696f 6e73     and functions
+000036c0: 2073 686f 756c 6420 6861 7665 2065 6974   should have eit
+000036d0: 6865 7220 646f 6374 6573 7473 206f 7220  her doctests or 
+000036e0: 6e6f 6e2d 646f 6374 6573 7420 7465 7374  non-doctest test
+000036f0: 732c 206e 6f74 0a20 2020 626f 7468 2e20  s, not.   both. 
+00003700: 5b4e 4f53 455f 444f 4354 4553 545f 5445  [NOSE_DOCTEST_TE
+00003710: 5354 535d 0a0a 2d2d 646f 6374 6573 742d  STS]..--doctest-
+00003720: 6578 7465 6e73 696f 6e3d 4558 540a 0a20  extension=EXT.. 
+00003730: 2020 416c 736f 206c 6f6f 6b20 666f 7220    Also look for 
+00003740: 646f 6374 6573 7473 2069 6e20 6669 6c65  doctests in file
+00003750: 7320 7769 7468 2074 6869 7320 6578 7465  s with this exte
+00003760: 6e73 696f 6e0a 2020 205b 4e4f 5345 5f44  nsion.   [NOSE_D
+00003770: 4f43 5445 5354 5f45 5854 454e 5349 4f4e  OCTEST_EXTENSION
+00003780: 5d0a 0a2d 2d64 6f63 7465 7374 2d72 6573  ]..--doctest-res
+00003790: 756c 742d 7661 7269 6162 6c65 3d56 4152  ult-variable=VAR
+000037a0: 0a0a 2020 2043 6861 6e67 6520 7468 6520  ..   Change the 
+000037b0: 7661 7269 6162 6c65 206e 616d 6520 7365  variable name se
+000037c0: 7420 746f 2074 6865 2072 6573 756c 7420  t to the result 
+000037d0: 6f66 2074 6865 206c 6173 7420 696e 7465  of the last inte
+000037e0: 7270 7265 7465 720a 2020 2063 6f6d 6d61  rpreter.   comma
+000037f0: 6e64 2066 726f 6d20 7468 6520 6465 6661  nd from the defa
+00003800: 756c 7420 275f 272e 2043 616e 2062 6520  ult '_'. Can be 
+00003810: 7573 6564 2074 6f20 6176 6f69 6420 636f  used to avoid co
+00003820: 6e66 6c69 6374 7320 7769 7468 0a20 2020  nflicts with.   
+00003830: 7468 6520 5f28 2920 6675 6e63 7469 6f6e  the _() function
+00003840: 2075 7365 6420 666f 7220 7465 7874 2074   used for text t
+00003850: 7261 6e73 6c61 7469 6f6e 2e0a 2020 205b  ranslation..   [
+00003860: 4e4f 5345 5f44 4f43 5445 5354 5f52 4553  NOSE_DOCTEST_RES
+00003870: 554c 545f 5641 525d 0a0a 2d2d 646f 6374  ULT_VAR]..--doct
+00003880: 6573 742d 6669 7874 7572 6573 3d53 5546  est-fixtures=SUF
+00003890: 4649 580a 0a20 2020 4669 6e64 2066 6978  FIX..   Find fix
+000038a0: 7475 7265 7320 666f 7220 6120 646f 6374  tures for a doct
+000038b0: 6573 7420 6669 6c65 2069 6e20 6d6f 6475  est file in modu
+000038c0: 6c65 2077 6974 6820 7468 6973 206e 616d  le with this nam
+000038d0: 6520 6170 7065 6e64 6564 0a20 2020 746f  e appended.   to
+000038e0: 2074 6865 2062 6173 6520 6e61 6d65 206f   the base name o
+000038f0: 6620 7468 6520 646f 6374 6573 7420 6669  f the doctest fi
+00003900: 6c65 0a0a 2d2d 646f 6374 6573 742d 6f70  le..--doctest-op
+00003910: 7469 6f6e 733d 4f50 5449 4f4e 530a 0a20  tions=OPTIONS.. 
+00003920: 2020 5370 6563 6966 7920 6f70 7469 6f6e    Specify option
+00003930: 7320 746f 2070 6173 7320 746f 2064 6f63  s to pass to doc
+00003940: 7465 7374 2e20 4567 2e0a 2020 2027 2b45  test. Eg..   '+E
+00003950: 4c4c 4950 5349 532c 2b4e 4f52 4d41 4c49  LLIPSIS,+NORMALI
+00003960: 5a45 5f57 4849 5445 5350 4143 4527 0a0a  ZE_WHITESPACE'..
+00003970: 2d2d 7769 7468 2d69 736f 6c61 7469 6f6e  --with-isolation
+00003980: 0a0a 2020 2045 6e61 626c 6520 706c 7567  ..   Enable plug
+00003990: 696e 2049 736f 6c61 7469 6f6e 506c 7567  in IsolationPlug
+000039a0: 696e 3a20 4163 7469 7661 7465 2074 6865  in: Activate the
+000039b0: 2069 736f 6c61 7469 6f6e 2070 6c75 6769   isolation plugi
+000039c0: 6e20 746f 0a20 2020 6973 6f6c 6174 6520  n to.   isolate 
+000039d0: 6368 616e 6765 7320 746f 2065 7874 6572  changes to exter
+000039e0: 6e61 6c20 6d6f 6475 6c65 7320 746f 2061  nal modules to a
+000039f0: 2073 696e 676c 6520 7465 7374 206d 6f64   single test mod
+00003a00: 756c 6520 6f72 0a20 2020 7061 636b 6167  ule or.   packag
+00003a10: 652e 2054 6865 2069 736f 6c61 7469 6f6e  e. The isolation
+00003a20: 2070 6c75 6769 6e20 7265 7365 7473 2074   plugin resets t
+00003a30: 6865 2063 6f6e 7465 6e74 7320 6f66 2073  he contents of s
+00003a40: 7973 2e6d 6f64 756c 6573 0a20 2020 6166  ys.modules.   af
+00003a50: 7465 7220 6561 6368 2074 6573 7420 6d6f  ter each test mo
+00003a60: 6475 6c65 206f 7220 7061 636b 6167 6520  dule or package 
+00003a70: 7275 6e73 2074 6f20 6974 7320 7374 6174  runs to its stat
+00003a80: 6520 6265 666f 7265 2074 6865 0a20 2020  e before the.   
+00003a90: 7465 7374 2e20 504c 4541 5345 204e 4f54  test. PLEASE NOT
+00003aa0: 4520 7468 6174 2074 6869 7320 706c 7567  E that this plug
+00003ab0: 696e 2073 686f 756c 6420 6e6f 7420 6265  in should not be
+00003ac0: 2075 7365 6420 7769 7468 2074 6865 0a20   used with the. 
+00003ad0: 2020 636f 7665 7261 6765 2070 6c75 6769    coverage plugi
+00003ae0: 6e2c 206f 7220 696e 2061 6e79 206f 7468  n, or in any oth
+00003af0: 6572 2063 6173 6520 7768 6572 6520 6d6f  er case where mo
+00003b00: 6475 6c65 2072 656c 6f61 6469 6e67 206d  dule reloading m
+00003b10: 6179 0a20 2020 7072 6f64 7563 6520 756e  ay.   produce un
+00003b20: 6465 7369 7261 626c 6520 7369 6465 2d65  desirable side-e
+00003b30: 6666 6563 7473 2e20 5b4e 4f53 455f 5749  ffects. [NOSE_WI
+00003b40: 5448 5f49 534f 4c41 5449 4f4e 5d0a 0a2d  TH_ISOLATION]..-
+00003b50: 642c 202d 2d64 6574 6169 6c65 642d 6572  d, --detailed-er
+00003b60: 726f 7273 2c20 2d2d 6661 696c 7572 652d  rors, --failure-
+00003b70: 6465 7461 696c 0a0a 2020 2041 6464 2064  detail..   Add d
+00003b80: 6574 6169 6c20 746f 2065 7272 6f72 206f  etail to error o
+00003b90: 7574 7075 7420 6279 2061 7474 656d 7074  utput by attempt
+00003ba0: 696e 6720 746f 2065 7661 6c75 6174 6520  ing to evaluate 
+00003bb0: 6661 696c 6564 2061 7373 6572 7473 0a20  failed asserts. 
+00003bc0: 2020 5b4e 4f53 455f 4445 5441 494c 4544    [NOSE_DETAILED
+00003bd0: 5f45 5252 4f52 535d 0a0a 2d2d 6e6f 2d73  _ERRORS]..--no-s
+00003be0: 6b69 700a 0a20 2020 4469 7361 626c 6520  kip..   Disable 
+00003bf0: 7370 6563 6961 6c20 6861 6e64 6c69 6e67  special handling
+00003c00: 206f 6620 536b 6970 5465 7374 2065 7863   of SkipTest exc
+00003c10: 6570 7469 6f6e 732e 0a0a 2d2d 7769 7468  eptions...--with
+00003c20: 2d69 640a 0a20 2020 456e 6162 6c65 2070  -id..   Enable p
+00003c30: 6c75 6769 6e20 5465 7374 4964 3a20 4163  lugin TestId: Ac
+00003c40: 7469 7661 7465 2074 6f20 6164 6420 6120  tivate to add a 
+00003c50: 7465 7374 2069 6420 286c 696b 6520 2331  test id (like #1
+00003c60: 2920 746f 2065 6163 680a 2020 2074 6573  ) to each.   tes
+00003c70: 7420 6e61 6d65 206f 7574 7075 742e 2041  t name output. A
+00003c80: 6374 6976 6174 6520 7769 7468 202d 2d66  ctivate with --f
+00003c90: 6169 6c65 6420 746f 2072 6572 756e 2066  ailed to rerun f
+00003ca0: 6169 6c69 6e67 2074 6573 7473 0a20 2020  ailing tests.   
+00003cb0: 6f6e 6c79 2e20 5b4e 4f53 455f 5749 5448  only. [NOSE_WITH
+00003cc0: 5f49 445d 0a0a 2d2d 6964 2d66 696c 653d  _ID]..--id-file=
+00003cd0: 4649 4c45 0a0a 2020 2053 746f 7265 2074  FILE..   Store t
+00003ce0: 6573 7420 6964 7320 666f 756e 6420 696e  est ids found in
+00003cf0: 2074 6573 7420 7275 6e73 2069 6e20 7468   test runs in th
+00003d00: 6973 2066 696c 652e 2044 6566 6175 6c74  is file. Default
+00003d10: 2069 7320 7468 6520 6669 6c65 0a20 2020   is the file.   
+00003d20: 2e6e 6f73 6569 6473 2069 6e20 7468 6520  .noseids in the 
+00003d30: 776f 726b 696e 6720 6469 7265 6374 6f72  working director
+00003d40: 792e 0a0a 2d2d 6661 696c 6564 0a0a 2020  y...--failed..  
+00003d50: 2052 756e 2074 6865 2074 6573 7473 2074   Run the tests t
+00003d60: 6861 7420 6661 696c 6564 2069 6e20 7468  hat failed in th
+00003d70: 6520 6c61 7374 2074 6573 7420 7275 6e2e  e last test run.
+00003d80: 0a0a 2d2d 7072 6f63 6573 7365 733d 4e55  ..--processes=NU
+00003d90: 4d0a 0a20 2020 5370 7265 6164 2074 6573  M..   Spread tes
+00003da0: 7420 7275 6e20 616d 6f6e 6720 7468 6973  t run among this
+00003db0: 206d 616e 7920 7072 6f63 6573 7365 732e   many processes.
+00003dc0: 2053 6574 2061 206e 756d 6265 7220 6571   Set a number eq
+00003dd0: 7561 6c20 746f 0a20 2020 7468 6520 6e75  ual to.   the nu
+00003de0: 6d62 6572 206f 6620 7072 6f63 6573 736f  mber of processo
+00003df0: 7273 206f 7220 636f 7265 7320 696e 2079  rs or cores in y
+00003e00: 6f75 7220 6d61 6368 696e 6520 666f 7220  our machine for 
+00003e10: 6265 7374 2072 6573 756c 7473 2e0a 2020  best results..  
+00003e20: 2050 6173 7320 6120 6e65 6761 7469 7665   Pass a negative
+00003e30: 206e 756d 6265 7220 746f 2068 6176 6520   number to have 
+00003e40: 7468 6520 6e75 6d62 6572 206f 6620 7072  the number of pr
+00003e50: 6f63 6573 7365 730a 2020 2061 7574 6f6d  ocesses.   autom
+00003e60: 6174 6963 616c 6c79 2073 6574 2074 6f20  atically set to 
+00003e70: 7468 6520 6e75 6d62 6572 206f 6620 636f  the number of co
+00003e80: 7265 732e 2050 6173 7369 6e67 2030 206d  res. Passing 0 m
+00003e90: 6561 6e73 2074 6f0a 2020 2064 6973 6162  eans to.   disab
+00003ea0: 6c65 2070 6172 616c 6c65 6c20 7465 7374  le parallel test
+00003eb0: 696e 672e 2044 6566 6175 6c74 2069 7320  ing. Default is 
+00003ec0: 3020 756e 6c65 7373 204e 4f53 455f 5052  0 unless NOSE_PR
+00003ed0: 4f43 4553 5345 5320 6973 0a20 2020 7365  OCESSES is.   se
+00003ee0: 742e 205b 4e4f 5345 5f50 524f 4345 5353  t. [NOSE_PROCESS
+00003ef0: 4553 5d0a 0a2d 2d70 726f 6365 7373 2d74  ES]..--process-t
+00003f00: 696d 656f 7574 3d53 4543 4f4e 4453 0a0a  imeout=SECONDS..
+00003f10: 2020 2053 6574 2074 696d 656f 7574 2066     Set timeout f
+00003f20: 6f72 2072 6574 7572 6e20 6f66 2072 6573  or return of res
+00003f30: 756c 7473 2066 726f 6d20 6561 6368 2074  ults from each t
+00003f40: 6573 7420 7275 6e6e 6572 2070 726f 6365  est runner proce
+00003f50: 7373 2e0a 2020 2044 6566 6175 6c74 2069  ss..   Default i
+00003f60: 7320 3130 2e20 5b4e 4f53 455f 5052 4f43  s 10. [NOSE_PROC
+00003f70: 4553 535f 5449 4d45 4f55 545d 0a0a 2d2d  ESS_TIMEOUT]..--
+00003f80: 7072 6f63 6573 732d 7265 7374 6172 7477  process-restartw
+00003f90: 6f72 6b65 720a 0a20 2020 4966 2073 6574  orker..   If set
+00003fa0: 2c20 7769 6c6c 2072 6573 7461 7274 2065  , will restart e
+00003fb0: 6163 6820 776f 726b 6572 2070 726f 6365  ach worker proce
+00003fc0: 7373 206f 6e63 6520 7468 6569 7220 7465  ss once their te
+00003fd0: 7374 7320 6172 6520 646f 6e65 2c0a 2020  sts are done,.  
+00003fe0: 2074 6869 7320 6865 6c70 7320 636f 6e74   this helps cont
+00003ff0: 726f 6c20 6d65 6d6f 7279 206c 6561 6b73  rol memory leaks
+00004000: 2066 726f 6d20 6b69 6c6c 696e 6720 7468   from killing th
+00004010: 6520 7379 7374 656d 2e0a 2020 205b 4e4f  e system..   [NO
+00004020: 5345 5f50 524f 4345 5353 5f52 4553 5441  SE_PROCESS_RESTA
+00004030: 5254 574f 524b 4552 5d0a 0a2d 2d77 6974  RTWORKER]..--wit
+00004040: 682d 7875 6e69 740a 0a20 2020 456e 6162  h-xunit..   Enab
+00004050: 6c65 2070 6c75 6769 6e20 5875 6e69 743a  le plugin Xunit:
+00004060: 2054 6869 7320 706c 7567 696e 2070 726f   This plugin pro
+00004070: 7669 6465 7320 7465 7374 2072 6573 756c  vides test resul
+00004080: 7473 2069 6e20 7468 650a 2020 2073 7461  ts in the.   sta
+00004090: 6e64 6172 6420 5855 6e69 7420 584d 4c20  ndard XUnit XML 
+000040a0: 666f 726d 6174 2e20 5b4e 4f53 455f 5749  format. [NOSE_WI
+000040b0: 5448 5f58 554e 4954 5d0a 0a2d 2d78 756e  TH_XUNIT]..--xun
+000040c0: 6974 2d66 696c 653d 4649 4c45 0a0a 2020  it-file=FILE..  
+000040d0: 2050 6174 6820 746f 2078 6d6c 2066 696c   Path to xml fil
+000040e0: 6520 746f 2073 746f 7265 2074 6865 2078  e to store the x
+000040f0: 756e 6974 2072 6570 6f72 7420 696e 2e20  unit report in. 
+00004100: 4465 6661 756c 7420 6973 0a20 2020 6e6f  Default is.   no
+00004110: 7365 7465 7374 732e 786d 6c20 696e 2074  setests.xml in t
+00004120: 6865 2077 6f72 6b69 6e67 2064 6972 6563  he working direc
+00004130: 746f 7279 205b 4e4f 5345 5f58 554e 4954  tory [NOSE_XUNIT
+00004140: 5f46 494c 455d 0a0a 2d2d 7875 6e69 742d  _FILE]..--xunit-
+00004150: 7465 7374 7375 6974 652d 6e61 6d65 3d50  testsuite-name=P
+00004160: 4143 4b41 4745 0a0a 2020 204e 616d 6520  ACKAGE..   Name 
+00004170: 6f66 2074 6865 2074 6573 7473 7569 7465  of the testsuite
+00004180: 2069 6e20 7468 6520 7875 6e69 7420 786d   in the xunit xm
+00004190: 6c2c 2067 656e 6572 6174 6564 2062 7920  l, generated by 
+000041a0: 706c 7567 696e 2e0a 2020 2044 6566 6175  plugin..   Defau
+000041b0: 6c74 2074 6573 7420 7375 6974 6520 6e61  lt test suite na
+000041c0: 6d65 2069 7320 6e6f 7365 7465 7374 732e  me is nosetests.
+000041d0: 0a0a 2d2d 616c 6c2d 6d6f 6475 6c65 730a  ..--all-modules.
+000041e0: 0a20 2020 456e 6162 6c65 2070 6c75 6769  .   Enable plugi
+000041f0: 6e20 416c 6c4d 6f64 756c 6573 3a20 436f  n AllModules: Co
+00004200: 6c6c 6563 7420 7465 7374 7320 6672 6f6d  llect tests from
+00004210: 2061 6c6c 2070 7974 686f 6e20 6d6f 6475   all python modu
+00004220: 6c65 732e 0a20 2020 5b4e 4f53 455f 414c  les..   [NOSE_AL
+00004230: 4c5f 4d4f 4455 4c45 535d 0a0a 2d2d 636f  L_MODULES]..--co
+00004240: 2c20 2d2d 636f 6c6c 6563 742d 6f6e 6c79  , --collect-only
+00004250: 0a0a 2020 2045 6e61 626c 6520 636f 6c6c  ..   Enable coll
+00004260: 6563 742d 6f6e 6c79 3a20 436f 6c6c 6563  ect-only: Collec
+00004270: 7420 616e 6420 6f75 7470 7574 2074 6573  t and output tes
+00004280: 7420 6e61 6d65 7320 6f6e 6c79 2c0a 2020  t names only,.  
+00004290: 2062 7574 2064 6f20 6e6f 7420 7275 6e20   but do not run 
+000042a0: 616e 7920 7465 7374 732e 205b 434f 4c4c  any tests. [COLL
+000042b0: 4543 545f 4f4e 4c59 5d0a 6060 600a       ECT_ONLY].```.
```

### Comparing `pynose-1.4.5/nose/__init__.py` & `pynose-1.4.6/nose/__init__.py`

 * *Files identical despite different names*

### Comparing `pynose-1.4.5/nose/case.py` & `pynose-1.4.6/nose/case.py`

 * *Files identical despite different names*

### Comparing `pynose-1.4.5/nose/commands.py` & `pynose-1.4.6/nose/commands.py`

 * *Files identical despite different names*

### Comparing `pynose-1.4.5/nose/config.py` & `pynose-1.4.6/nose/config.py`

 * *Files identical despite different names*

### Comparing `pynose-1.4.5/nose/core.py` & `pynose-1.4.6/nose/core.py`

 * *Files identical despite different names*

### Comparing `pynose-1.4.5/nose/failure.py` & `pynose-1.4.6/nose/failure.py`

 * *Files identical despite different names*

### Comparing `pynose-1.4.5/nose/importer.py` & `pynose-1.4.6/nose/importer.py`

 * *Files identical despite different names*

### Comparing `pynose-1.4.5/nose/inspector.py` & `pynose-1.4.6/nose/inspector.py`

 * *Files identical despite different names*

### Comparing `pynose-1.4.5/nose/loader.py` & `pynose-1.4.6/nose/loader.py`

 * *Files identical despite different names*

### Comparing `pynose-1.4.5/nose/plugins/__init__.py` & `pynose-1.4.6/nose/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `pynose-1.4.5/nose/plugins/allmodules.py` & `pynose-1.4.6/nose/plugins/allmodules.py`

 * *Files identical despite different names*

### Comparing `pynose-1.4.5/nose/plugins/attrib.py` & `pynose-1.4.6/nose/plugins/attrib.py`

 * *Files identical despite different names*

### Comparing `pynose-1.4.5/nose/plugins/base.py` & `pynose-1.4.6/nose/plugins/base.py`

 * *Files identical despite different names*

### Comparing `pynose-1.4.5/nose/plugins/builtin.py` & `pynose-1.4.6/nose/plugins/builtin.py`

 * *Files identical despite different names*

### Comparing `pynose-1.4.5/nose/plugins/capture.py` & `pynose-1.4.6/nose/plugins/capture.py`

 * *Files identical despite different names*

### Comparing `pynose-1.4.5/nose/plugins/collect.py` & `pynose-1.4.6/nose/plugins/collect.py`

 * *Files identical despite different names*

### Comparing `pynose-1.4.5/nose/plugins/cover.py` & `pynose-1.4.6/nose/plugins/cover.py`

 * *Files identical despite different names*

### Comparing `pynose-1.4.5/nose/plugins/debug.py` & `pynose-1.4.6/nose/plugins/debug.py`

 * *Files identical despite different names*

### Comparing `pynose-1.4.5/nose/plugins/deprecated.py` & `pynose-1.4.6/nose/plugins/deprecated.py`

 * *Files identical despite different names*

### Comparing `pynose-1.4.5/nose/plugins/doctests.py` & `pynose-1.4.6/nose/plugins/doctests.py`

 * *Files identical despite different names*

### Comparing `pynose-1.4.5/nose/plugins/errorclass.py` & `pynose-1.4.6/nose/plugins/errorclass.py`

 * *Files identical despite different names*

### Comparing `pynose-1.4.5/nose/plugins/failuredetail.py` & `pynose-1.4.6/nose/plugins/failuredetail.py`

 * *Files identical despite different names*

### Comparing `pynose-1.4.5/nose/plugins/isolate.py` & `pynose-1.4.6/nose/plugins/isolate.py`

 * *Files identical despite different names*

### Comparing `pynose-1.4.5/nose/plugins/logcapture.py` & `pynose-1.4.6/nose/plugins/logcapture.py`

 * *Files identical despite different names*

### Comparing `pynose-1.4.5/nose/plugins/manager.py` & `pynose-1.4.6/nose/plugins/manager.py`

 * *Files 8% similar despite different names*

```diff
@@ -320,22 +320,42 @@
             return
         return self.plugin.stopTest(test.test)
 
     def __getattr__(self, val):
         return getattr(self.plugin, val)
 
 
+def iter_entry_points(group_name):
+    try:
+        from importlib.metadata import entry_points
+    except (ImportError, Exception):
+        try:
+            from pkg_resources import iter_entry_points
+        except (ImportError, OSError):
+            return []
+        else:
+            return iter_entry_points(group_name)
+    groups = entry_points()
+    if hasattr(groups, 'select'):
+        # New interface in Python 3.10 and newer versions of the
+        # importlib_metadata backport.
+        return groups.select(group=group_name)
+    else:
+        # Older interface, deprecated in Python 3.10 and recent
+        # importlib_metadata, but we need it in Python 3.8 and 3.9.
+        return groups.get(group_name, [])
+
+
 class EntryPointPluginManager(PluginManager):
     """Plugin manager that loads plugins from `nose.plugins` entry points."""
     entry_points = (('nose.plugins.0.10', None),
                     ('nose.plugins', ZeroNinePlugin))
 
     def loadPlugins(self):
         """Load plugins by iterating the `nose.plugins` entry point."""
-        from pkg_resources import iter_entry_points
         loaded = {}
         for entry_point, adapt in self.entry_points:
             for ep in iter_entry_points(entry_point):
                 if ep.name in loaded:
                     continue
                 loaded[ep.name] = True
                 log.debug('%s load plugin %s', self.__class__.__name__, ep)
```

### Comparing `pynose-1.4.5/nose/plugins/multiprocess.py` & `pynose-1.4.6/nose/plugins/multiprocess.py`

 * *Files identical despite different names*

### Comparing `pynose-1.4.5/nose/plugins/plugintest.py` & `pynose-1.4.6/nose/plugins/plugintest.py`

 * *Files identical despite different names*

### Comparing `pynose-1.4.5/nose/plugins/skip.py` & `pynose-1.4.6/nose/plugins/skip.py`

 * *Files identical despite different names*

### Comparing `pynose-1.4.5/nose/plugins/testid.py` & `pynose-1.4.6/nose/plugins/testid.py`

 * *Files identical despite different names*

### Comparing `pynose-1.4.5/nose/plugins/xunit.py` & `pynose-1.4.6/nose/plugins/xunit.py`

 * *Files identical despite different names*

### Comparing `pynose-1.4.5/nose/proxy.py` & `pynose-1.4.6/nose/proxy.py`

 * *Files identical despite different names*

### Comparing `pynose-1.4.5/nose/pyversion.py` & `pynose-1.4.6/nose/pyversion.py`

 * *Files identical despite different names*

### Comparing `pynose-1.4.5/nose/result.py` & `pynose-1.4.6/nose/result.py`

 * *Files identical despite different names*

### Comparing `pynose-1.4.5/nose/selector.py` & `pynose-1.4.6/nose/selector.py`

 * *Files identical despite different names*

### Comparing `pynose-1.4.5/nose/sphinx/pluginopts.py` & `pynose-1.4.6/nose/sphinx/pluginopts.py`

 * *Files identical despite different names*

### Comparing `pynose-1.4.5/nose/suite.py` & `pynose-1.4.6/nose/suite.py`

 * *Files identical despite different names*

### Comparing `pynose-1.4.5/nose/tools/nontrivial.py` & `pynose-1.4.6/nose/tools/nontrivial.py`

 * *Files identical despite different names*

### Comparing `pynose-1.4.5/nose/tools/trivial.py` & `pynose-1.4.6/nose/tools/trivial.py`

 * *Files identical despite different names*

### Comparing `pynose-1.4.5/nose/twistedtools.py` & `pynose-1.4.6/nose/twistedtools.py`

 * *Files identical despite different names*

### Comparing `pynose-1.4.5/nose/usage.txt` & `pynose-1.4.6/nose/usage.txt`

 * *Files identical despite different names*

### Comparing `pynose-1.4.5/nose/util.py` & `pynose-1.4.6/nose/util.py`

 * *Files identical despite different names*

### Comparing `pynose-1.4.5/pynose.egg-info/PKG-INFO` & `pynose-1.4.6/pynose.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 7079 6e6f  : 2.1.Name: pyno
 00000020: 7365 0a56 6572 7369 6f6e 3a20 312e 342e  se.Version: 1.4.
-00000030: 350a 5375 6d6d 6172 793a 2070 796e 6f73  5.Summary: pynos
+00000030: 360a 5375 6d6d 6172 793a 2070 796e 6f73  6.Summary: pynos
 00000040: 6520 6669 7865 7320 6e6f 7365 2074 6f20  e fixes nose to 
 00000050: 6578 7465 6e64 2075 6e69 7474 6573 7420  extend unittest 
 00000060: 616e 6420 6d61 6b65 2074 6573 7469 6e67  and make testing
 00000070: 2065 6173 6965 720a 486f 6d65 2d70 6167   easier.Home-pag
 00000080: 653a 2068 7474 7073 3a2f 2f67 6974 6875  e: https://githu
 00000090: 622e 636f 6d2f 6d64 6d69 6e74 7a2f 7079  b.com/mdmintz/py
 000000a0: 6e6f 7365 0a41 7574 686f 723a 204d 6963  nose.Author: Mic
@@ -85,1070 +85,1075 @@
 00000540: 6172 6520 4465 7665 6c6f 706d 656e 7420  are Development 
 00000550: 3a3a 2054 6573 7469 6e67 0a52 6571 7569  :: Testing.Requi
 00000560: 7265 732d 5079 7468 6f6e 3a20 3e3d 332e  res-Python: >=3.
 00000570: 360a 4465 7363 7269 7074 696f 6e2d 436f  6.Description-Co
 00000580: 6e74 656e 742d 5479 7065 3a20 7465 7874  ntent-Type: text
 00000590: 2f6d 6172 6b64 6f77 6e0a 4c69 6365 6e73  /markdown.Licens
 000005a0: 652d 4669 6c65 3a20 4c49 4345 4e53 450a  e-File: LICENSE.
-000005b0: 0a23 2070 796e 6f73 650a 0a23 2323 2060  .# pynose..### `
-000005c0: 6070 796e 6f73 6560 6020 6669 7865 7320  `pynose`` fixes 
-000005d0: 6060 6e6f 7365 6060 2074 6f20 6578 7465  ``nose`` to exte
-000005e0: 6e64 205b 756e 6974 7465 7374 5d28 6874  nd [unittest](ht
-000005f0: 7470 733a 2f2f 646f 6373 2e70 7974 686f  tps://docs.pytho
-00000600: 6e2e 6f72 672f 332f 6c69 6272 6172 792f  n.org/3/library/
-00000610: 756e 6974 7465 7374 2e68 746d 6c29 2061  unittest.html) a
-00000620: 6e64 206d 616b 6520 7465 7374 696e 6720  nd make testing 
-00000630: 6561 7369 6572 2e0a 0a28 4e4f 5445 3a20  easier...(NOTE: 
-00000640: 4966 2079 6f75 2063 616e 2c20 7573 6520  If you can, use 
-00000650: 2a2a 5b70 7974 6573 745d 2868 7474 7073  **[pytest](https
-00000660: 3a2f 2f64 6f63 732e 7079 7465 7374 2e6f  ://docs.pytest.o
-00000670: 7267 2f29 2a2a 2069 6e73 7465 6164 2e20  rg/)** instead. 
-00000680: 2a2a 5b70 796e 6f73 655d 2868 7474 7073  **[pynose](https
-00000690: 3a2f 2f67 6974 6875 622e 636f 6d2f 6d64  ://github.com/md
-000006a0: 6d69 6e74 7a2f 7079 6e6f 7365 292a 2a20  mintz/pynose)** 
-000006b0: 7761 7320 6275 696c 7420 746f 206d 6169  was built to mai
-000006c0: 6e74 6169 6e20 2a2a 5b6e 6f73 655d 2868  ntain **[nose](h
-000006d0: 7474 7073 3a2f 2f6e 6f73 652e 7265 6164  ttps://nose.read
-000006e0: 7468 6564 6f63 732e 696f 2f65 6e2f 6c61  thedocs.io/en/la
-000006f0: 7465 7374 2f29 2a2a 2066 6f72 2064 6576  test/)** for dev
-00000700: 656c 6f70 6572 7320 7768 6f20 7374 696c  elopers who stil
-00000710: 6c20 7573 6520 6974 2e29 0a0a 2d2d 2d2d  l use it.)..----
-00000720: 2d2d 2d2d 0a0a 6060 7079 6e6f 7365 6060  ----..``pynose``
-00000730: 2069 7320 616e 2075 7064 6174 6564 2076   is an updated v
-00000740: 6572 7369 6f6e 206f 6620 6060 6e6f 7365  ersion of ``nose
-00000750: 6060 2c20 6f72 6967 696e 616c 6c79 206d  ``, originally m
-00000760: 6164 6520 6279 204a 6173 6f6e 2050 656c  ade by Jason Pel
-00000770: 6c65 7269 6e2e 0a0a 5468 6973 2076 6572  lerin...This ver
-00000780: 7369 6f6e 206f 6620 6060 6e6f 7365 6060  sion of ``nose``
-00000790: 2069 7320 636f 6d70 6174 6962 6c65 2077   is compatible w
-000007a0: 6974 6820 5079 7468 6f6e 2033 2e36 2b20  ith Python 3.6+ 
-000007b0: 2869 6e63 6c75 6469 6e67 2033 2e31 3220  (including 3.12 
-000007c0: 2620 7570 292e 0a0a 4368 616e 6765 7320  & up)...Changes 
-000007d0: 696e 2060 6070 796e 6f73 6560 6020 6672  in ``pynose`` fr
-000007e0: 6f6d 206c 6567 6163 7920 6060 6e6f 7365  om legacy ``nose
-000007f0: 6060 2069 6e63 6c75 6465 3a0a 2a20 4669  `` include:.* Fi
-00000800: 7865 7320 2241 7474 7269 6275 7465 4572  xes "AttributeEr
-00000810: 726f 723a 206d 6f64 756c 6520 2763 6f6c  ror: module 'col
-00000820: 6c65 6374 696f 6e73 2720 6861 7320 6e6f  lections' has no
-00000830: 2061 7474 7269 6275 7465 2027 4361 6c6c   attribute 'Call
-00000840: 6162 6c65 272e 220a 2a20 4669 7865 7320  able'.".* Fixes 
-00000850: 2241 7474 7269 6275 7465 4572 726f 723a  "AttributeError:
-00000860: 206d 6f64 756c 6520 2769 6e73 7065 6374   module 'inspect
-00000870: 2720 6861 7320 6e6f 2061 7474 7269 6275  ' has no attribu
-00000880: 7465 2027 6765 7461 7267 7370 6563 272e  te 'getargspec'.
-00000890: 220a 2a20 4669 7865 7320 2249 6d70 6f72  ".* Fixes "Impor
-000008a0: 7445 7272 6f72 3a20 6361 6e6e 6f74 2069  tError: cannot i
-000008b0: 6d70 6f72 7420 6e61 6d65 2027 5f54 6578  mport name '_Tex
-000008c0: 7454 6573 7452 6573 756c 7427 2066 726f  tTestResult' fro
-000008d0: 6d20 2775 6e69 7474 6573 7427 2e22 0a2a  m 'unittest'.".*
-000008e0: 2046 6978 6573 2022 5275 6e74 696d 6557   Fixes "RuntimeW
-000008f0: 6172 6e69 6e67 3a20 5465 7374 5265 7375  arning: TestResu
-00000900: 6c74 2068 6173 206e 6f20 6164 6444 7572  lt has no addDur
-00000910: 6174 696f 6e20 6d65 7468 6f64 2e22 0a2a  ation method.".*
-00000920: 2046 6978 6573 2061 6c6c 2060 6066 6c61   Fixes all ``fla
-00000930: 6b65 3860 6020 6973 7375 6573 2066 726f  ke8`` issues fro
-00000940: 6d20 7468 6520 6f72 6967 696e 616c 2060  m the original `
-00000950: 606e 6f73 6560 602e 0a2a 2052 6570 6c61  `nose``..* Repla
-00000960: 6365 7320 7468 6520 6060 696d 7060 6020  ces the ``imp`` 
-00000970: 6d6f 6475 6c65 2077 6974 6820 7468 6520  module with the 
-00000980: 6e65 7765 7220 6060 696d 706f 7274 6c69  newer ``importli
-00000990: 6260 6020 6d6f 6475 6c65 2e0a 2a20 5468  b`` module..* Th
-000009a0: 6520 6465 6661 756c 7420 6c6f 6767 696e  e default loggin
-000009b0: 6720 6c65 7665 6c20 6e6f 7720 6869 6465  g level now hide
-000009c0: 7320 2264 6562 7567 2220 6c6f 6773 2066  s "debug" logs f
-000009d0: 6f72 206c 6573 7320 6e6f 6973 652e 0a2a  or less noise..*
-000009e0: 2054 6865 2060 602d 7360 6020 6f70 7469   The ``-s`` opti
-000009f0: 6f6e 2069 7320 616c 7761 7973 2061 6374  on is always act
-00000a00: 6976 6520 746f 2073 6565 2074 6865 206f  ive to see the o
-00000a10: 7574 7075 7420 6f66 2060 6070 7269 6e74  utput of ``print
-00000a20: 2829 6060 2e0a 2a20 4164 6473 2060 602d  ()``..* Adds ``-
-00000a30: 2d63 6f60 6020 6173 2061 2073 686f 7274  -co`` as a short
-00000a40: 6375 7420 746f 2075 7369 6e67 2060 602d  cut to using ``-
-00000a50: 2d63 6f6c 6c65 6374 2d6f 6e6c 7960 602e  -collect-only``.
-00000a60: 0a0a 2d2d 2d2d 2d2d 2d2d 0a0a 5468 6520  ..--------..The 
-00000a70: 6f72 6967 696e 616c 2064 6573 6372 6970  original descrip
-00000a80: 7469 6f6e 206f 6620 6060 6e6f 7365 6060  tion of ``nose``
-00000a90: 3a0a 0a3e 6e6f 7365 2065 7874 656e 6473  :..>nose extends
-00000aa0: 2074 6865 2074 6573 7420 6c6f 6164 696e   the test loadin
-00000ab0: 6720 616e 6420 7275 6e6e 696e 6720 6665  g and running fe
-00000ac0: 6174 7572 6573 206f 6620 756e 6974 7465  atures of unitte
-00000ad0: 7374 2c20 6d61 6b69 6e67 0a69 7420 6561  st, making.it ea
-00000ae0: 7369 6572 2074 6f20 7772 6974 652c 2066  sier to write, f
-00000af0: 696e 6420 616e 6420 7275 6e20 7465 7374  ind and run test
-00000b00: 732e 0a0a 3e42 7920 6465 6661 756c 742c  s...>By default,
-00000b10: 206e 6f73 6520 7275 6e73 2074 6573 7473   nose runs tests
-00000b20: 2069 6e20 6669 6c65 7320 6f72 2064 6972   in files or dir
-00000b30: 6563 746f 7269 6573 2075 6e64 6572 2074  ectories under t
-00000b40: 6865 2063 7572 7265 6e74 0a77 6f72 6b69  he current.worki
-00000b50: 6e67 2064 6972 6563 746f 7279 2077 686f  ng directory who
-00000b60: 7365 206e 616d 6573 2069 6e63 6c75 6465  se names include
-00000b70: 2022 7465 7374 2220 6f72 2022 5465 7374   "test" or "Test
-00000b80: 2220 6174 2061 2077 6f72 640a 626f 756e  " at a word.boun
-00000b90: 6461 7279 2028 6c69 6b65 2022 7465 7374  dary (like "test
-00000ba0: 5f74 6869 7322 206f 7220 2266 756e 6374  _this" or "funct
-00000bb0: 696f 6e61 6c5f 7465 7374 2220 6f72 2022  ional_test" or "
-00000bc0: 5465 7374 436c 6173 7322 2062 7574 206e  TestClass" but n
-00000bd0: 6f74 0a22 6c69 6274 6573 7422 292e 2054  ot."libtest"). T
-00000be0: 6573 7420 6f75 7470 7574 2069 7320 7369  est output is si
-00000bf0: 6d69 6c61 7220 746f 2074 6861 7420 6f66  milar to that of
-00000c00: 2075 6e69 7474 6573 742c 2062 7574 2061   unittest, but a
-00000c10: 6c73 6f20 696e 636c 7564 6573 0a63 6170  lso includes.cap
-00000c20: 7475 7265 6420 7374 646f 7574 206f 7574  tured stdout out
-00000c30: 7075 7420 6672 6f6d 2066 6169 6c69 6e67  put from failing
-00000c40: 2074 6573 7473 2c20 666f 7220 6561 7379   tests, for easy
-00000c50: 2070 7269 6e74 2d73 7479 6c65 2064 6562   print-style deb
-00000c60: 7567 6769 6e67 2e0a 0a3e 5468 6573 6520  ugging...>These 
-00000c70: 6665 6174 7572 6573 2c20 616e 6420 6d61  features, and ma
-00000c80: 6e79 206d 6f72 652c 2061 7265 2063 7573  ny more, are cus
-00000c90: 746f 6d69 7a61 626c 6520 7468 726f 7567  tomizable throug
-00000ca0: 6820 7468 6520 7573 6520 6f66 0a70 6c75  h the use of.plu
-00000cb0: 6769 6e73 2e20 506c 7567 696e 7320 696e  gins. Plugins in
-00000cc0: 636c 7564 6564 2077 6974 6820 6e6f 7365  cluded with nose
-00000cd0: 2070 726f 7669 6465 2073 7570 706f 7274   provide support
-00000ce0: 2066 6f72 2064 6f63 7465 7374 2c20 636f   for doctest, co
-00000cf0: 6465 0a63 6f76 6572 6167 6520 616e 6420  de.coverage and 
-00000d00: 7072 6f66 696c 696e 672c 2066 6c65 7869  profiling, flexi
-00000d10: 626c 6520 6174 7472 6962 7574 652d 6261  ble attribute-ba
-00000d20: 7365 6420 7465 7374 2073 656c 6563 7469  sed test selecti
-00000d30: 6f6e 2c0a 6f75 7470 7574 2063 6170 7475  on,.output captu
-00000d40: 7265 2061 6e64 206d 6f72 652e 204d 6f72  re and more. Mor
-00000d50: 6520 696e 666f 726d 6174 696f 6e20 6162  e information ab
-00000d60: 6f75 7420 7772 6974 696e 6720 706c 7567  out writing plug
-00000d70: 696e 730a 6d61 7920 6265 2066 6f75 6e64  ins.may be found
-00000d80: 206f 6e20 696e 2074 6865 206e 6f73 6520   on in the nose 
-00000d90: 4150 4920 646f 6375 6d65 6e74 6174 696f  API documentatio
-00000da0: 6e2c 2068 6572 653a 0a68 7474 7073 3a2f  n, here:.https:/
-00000db0: 2f6e 6f73 652e 7265 6164 7468 6564 6f63  /nose.readthedoc
-00000dc0: 732e 696f 2f65 6e2f 6c61 7465 7374 2f0a  s.io/en/latest/.
-00000dd0: 0a2d 2d2d 2d2d 2d2d 2d0a 0a60 6060 6261  .--------..```ba
-00000de0: 7368 0a0a 4261 7369 6320 7573 6167 650a  sh..Basic usage.
-00000df0: 2a2a 2a2a 2a2a 2a2a 2a2a 2a0a 0a55 7365  ***********..Use
-00000e00: 2022 7079 6e6f 7365 2220 4f52 2022 6e6f   "pynose" OR "no
-00000e10: 7365 7465 7374 7322 2074 6f20 7275 6e20  setests" to run 
-00000e20: 7465 7374 733a 0a0a 2020 2020 7079 6e6f  tests:..    pyno
-00000e30: 7365 205b 6f70 7469 6f6e 735d 205b 286f  se [options] [(o
-00000e40: 7074 696f 6e61 6c29 2074 6573 7420 6669  ptional) test fi
-00000e50: 6c65 7320 6f72 2064 6972 6563 746f 7269  les or directori
-00000e60: 6573 5d0a 0a20 2020 206e 6f73 6574 6573  es]..    nosetes
-00000e70: 7473 205b 6f70 7469 6f6e 735d 205b 286f  ts [options] [(o
-00000e80: 7074 696f 6e61 6c29 2074 6573 7420 6669  ptional) test fi
-00000e90: 6c65 7320 6f72 2064 6972 6563 746f 7269  les or directori
-00000ea0: 6573 5d0a 0a49 6e20 6164 6469 7469 6f6e  es]..In addition
-00000eb0: 2074 6f20 7061 7373 696e 6720 636f 6d6d   to passing comm
-00000ec0: 616e 642d 6c69 6e65 206f 7074 696f 6e73  and-line options
-00000ed0: 2c20 796f 7520 6d61 7920 616c 736f 2070  , you may also p
-00000ee0: 7574 0a63 6f6e 6669 6775 7261 7469 6f6e  ut.configuration
-00000ef0: 206f 7074 696f 6e73 2069 6e20 6120 2e6e   options in a .n
-00000f00: 6f73 6572 6320 6f72 206e 6f73 652e 6366  oserc or nose.cf
-00000f10: 6720 6669 6c65 2069 6e20 796f 7572 2068  g file in your h
-00000f20: 6f6d 650a 6469 7265 6374 6f72 792e 2054  ome.directory. T
-00000f30: 6865 7365 2061 7265 2073 7461 6e64 6172  hese are standar
-00000f40: 6420 2e69 6e69 2d73 7479 6c65 2063 6f6e  d .ini-style con
-00000f50: 6669 6720 6669 6c65 732e 2050 7574 2079  fig files. Put y
-00000f60: 6f75 720a 6e6f 7365 7465 7374 7320 636f  our.nosetests co
-00000f70: 6e66 6967 7572 6174 696f 6e20 696e 2061  nfiguration in a
-00000f80: 205b 6e6f 7365 7465 7374 735d 2073 6563   [nosetests] sec
-00000f90: 7469 6f6e 2c20 7769 7468 2074 6865 202d  tion, with the -
-00000fa0: 2d20 7072 6566 6978 0a72 656d 6f76 6564  - prefix.removed
-00000fb0: 3a0a 0a20 2020 5b6e 6f73 6574 6573 7473  :..   [nosetests
-00000fc0: 5d0a 2020 2076 6572 626f 7369 7479 3d33  ].   verbosity=3
-00000fd0: 0a20 2020 7769 7468 2d64 6f63 7465 7374  .   with-doctest
-00000fe0: 3d31 0a0a 5468 6572 6520 6973 2061 6c73  =1..There is als
-00000ff0: 6f20 706f 7373 6962 6c69 7479 2074 6f20  o possiblity to 
-00001000: 6469 7361 626c 6520 636f 6e66 6967 7572  disable configur
-00001010: 6174 696f 6e20 6669 6c65 7320 6c6f 6164  ation files load
-00001020: 696e 6720 286d 6967 6874 0a62 6520 7573  ing (might.be us
-00001030: 6566 756c 2077 6865 6e20 7275 6e6e 6967  eful when runnig
-00001040: 2069 2e65 2e20 746f 7820 616e 6420 796f   i.e. tox and yo
-00001050: 7520 646f 206e 6f74 2077 616e 7420 796f  u do not want yo
-00001060: 7572 2067 6c6f 6261 6c20 6e6f 7365 0a63  ur global nose.c
-00001070: 6f6e 6669 6720 6669 6c65 2074 6f20 6265  onfig file to be
-00001080: 2075 7365 6420 6279 2074 6f78 292e 2049   used by tox). I
-00001090: 6e20 6f72 6465 7220 746f 2069 676e 6f72  n order to ignor
-000010a0: 6520 7468 6f73 6520 636f 6e66 6967 7572  e those configur
-000010b0: 6174 696f 6e0a 6669 6c65 7320 7369 6d70  ation.files simp
-000010c0: 6c79 2073 6574 2061 6e20 656e 7669 726f  ly set an enviro
-000010d0: 6e6d 656e 7420 7661 7269 6162 6c65 2022  nment variable "
-000010e0: 4e4f 5345 5f49 474e 4f52 455f 434f 4e46  NOSE_IGNORE_CONF
-000010f0: 4947 5f46 494c 4553 222e 0a0a 5468 6572  IG_FILES"...Ther
-00001100: 6520 6172 6520 7365 7665 7261 6c20 6f74  e are several ot
-00001110: 6865 7220 7761 7973 2074 6f20 7573 6520  her ways to use 
-00001120: 7468 6520 6e6f 7365 2074 6573 7420 7275  the nose test ru
-00001130: 6e6e 6572 2062 6573 6964 6573 2074 6865  nner besides the
-00001140: 0a2a 6e6f 7365 7465 7374 732a 2073 6372  .*nosetests* scr
-00001150: 6970 742e 2059 6f75 206d 6179 2075 7365  ipt. You may use
-00001160: 206e 6f73 6520 696e 2061 2074 6573 7420   nose in a test 
-00001170: 7363 7269 7074 3a0a 0a20 2020 696d 706f  script:..   impo
-00001180: 7274 206e 6f73 650a 2020 206e 6f73 652e  rt nose.   nose.
-00001190: 6d61 696e 2829 0a0a 4966 2079 6f75 2064  main()..If you d
-000011a0: 6f20 6e6f 7420 7761 6e74 2074 6865 2074  o not want the t
-000011b0: 6573 7420 7363 7269 7074 2074 6f20 6578  est script to ex
-000011c0: 6974 2077 6974 6820 3020 6f6e 2073 7563  it with 0 on suc
-000011d0: 6365 7373 2061 6e64 2031 206f 6e0a 6661  cess and 1 on.fa
-000011e0: 696c 7572 6520 286c 696b 6520 756e 6974  ilure (like unit
-000011f0: 7465 7374 2e6d 6169 6e29 2c20 7573 6520  test.main), use 
-00001200: 6e6f 7365 2e72 756e 2829 2069 6e73 7465  nose.run() inste
-00001210: 6164 3a0a 0a20 2020 696d 706f 7274 206e  ad:..   import n
-00001220: 6f73 650a 2020 2072 6573 756c 7420 3d20  ose.   result = 
-00001230: 6e6f 7365 2e72 756e 2829 0a0a 2a72 6573  nose.run()..*res
-00001240: 756c 742a 2077 696c 6c20 6265 2074 7275  ult* will be tru
-00001250: 6520 6966 2074 6865 2074 6573 7420 7275  e if the test ru
-00001260: 6e20 7375 6363 6565 6465 642c 206f 7220  n succeeded, or 
-00001270: 6661 6c73 6520 6966 2061 6e79 2074 6573  false if any tes
-00001280: 740a 6661 696c 6564 206f 7220 7261 6973  t.failed or rais
-00001290: 6564 2061 6e20 756e 6361 7567 6874 2065  ed an uncaught e
-000012a0: 7863 6570 7469 6f6e 2e20 4c61 7374 6c79  xception. Lastly
-000012b0: 2c20 796f 7520 6361 6e20 7275 6e20 6e6f  , you can run no
-000012c0: 7365 2e63 6f72 650a 6469 7265 6374 6c79  se.core.directly
-000012d0: 2c20 7768 6963 6820 7769 6c6c 2072 756e  , which will run
-000012e0: 206e 6f73 652e 6d61 696e 2829 3a0a 0a20   nose.main():.. 
-000012f0: 2020 7079 7468 6f6e 202f 7061 7468 2f74    python /path/t
-00001300: 6f2f 6e6f 7365 2f63 6f72 652e 7079 0a0a  o/nose/core.py..
-00001310: 506c 6561 7365 2073 6565 2074 6865 2075  Please see the u
-00001320: 7361 6765 206d 6573 7361 6765 2066 6f72  sage message for
-00001330: 2074 6865 206e 6f73 6574 6573 7473 2073   the nosetests s
-00001340: 6372 6970 7420 666f 7220 696e 666f 726d  cript for inform
-00001350: 6174 696f 6e0a 6162 6f75 7420 686f 7720  ation.about how 
-00001360: 746f 2063 6f6e 7472 6f6c 2077 6869 6368  to control which
-00001370: 2074 6573 7473 206e 6f73 6520 7275 6e73   tests nose runs
-00001380: 2c20 7768 6963 6820 706c 7567 696e 7320  , which plugins 
-00001390: 6172 6520 6c6f 6164 6564 2c0a 616e 6420  are loaded,.and 
-000013a0: 7468 6520 7465 7374 206f 7574 7075 742e  the test output.
-000013b0: 0a0a 0a45 7874 656e 6465 6420 7573 6167  ...Extended usag
-000013c0: 650a 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  e.==============
-000013d0: 0a0a 6e6f 7365 2063 6f6c 6c65 6374 7320  ..nose collects 
-000013e0: 7465 7374 7320 6175 746f 6d61 7469 6361  tests automatica
-000013f0: 6c6c 7920 6672 6f6d 2070 7974 686f 6e20  lly from python 
-00001400: 736f 7572 6365 2066 696c 6573 2c0a 6469  source files,.di
-00001410: 7265 6374 6f72 6965 7320 616e 6420 7061  rectories and pa
-00001420: 636b 6167 6573 2066 6f75 6e64 2069 6e20  ckages found in 
-00001430: 6974 7320 776f 726b 696e 6720 6469 7265  its working dire
-00001440: 6374 6f72 7920 2877 6869 6368 0a64 6566  ctory (which.def
-00001450: 6175 6c74 7320 746f 2074 6865 2063 7572  aults to the cur
-00001460: 7265 6e74 2077 6f72 6b69 6e67 2064 6972  rent working dir
-00001470: 6563 746f 7279 292e 2041 6e79 2070 7974  ectory). Any pyt
-00001480: 686f 6e20 736f 7572 6365 2066 696c 652c  hon source file,
-00001490: 0a64 6972 6563 746f 7279 206f 7220 7061  .directory or pa
-000014a0: 636b 6167 6520 7468 6174 206d 6174 6368  ckage that match
-000014b0: 6573 2074 6865 2074 6573 744d 6174 6368  es the testMatch
-000014c0: 2072 6567 756c 6172 2065 7870 7265 7373   regular express
-000014d0: 696f 6e20 2862 790a 6465 6661 756c 743a  ion (by.default:
-000014e0: 202a 283f 3a5e 7c5b 625f 2e2d 5d29 5b54   *(?:^|[b_.-])[T
-000014f0: 745d 6573 7429 2a20 7769 6c6c 2062 6520  t]est)* will be 
-00001500: 636f 6c6c 6563 7465 6420 6173 2061 2074  collected as a t
-00001510: 6573 7420 286f 7220 736f 7572 6365 0a66  est (or source.f
-00001520: 6f72 2063 6f6c 6c65 6374 696f 6e20 6f66  or collection of
-00001530: 2074 6573 7473 292e 2049 6e20 6164 6469   tests). In addi
-00001540: 7469 6f6e 2c20 616c 6c20 6f74 6865 7220  tion, all other 
-00001550: 7061 636b 6167 6573 2066 6f75 6e64 2069  packages found i
-00001560: 6e20 7468 650a 776f 726b 696e 6720 6469  n the.working di
-00001570: 7265 6374 6f72 7920 7769 6c6c 2062 6520  rectory will be 
-00001580: 6578 616d 696e 6564 2066 6f72 2070 7974  examined for pyt
-00001590: 686f 6e20 736f 7572 6365 2066 696c 6573  hon source files
-000015a0: 206f 720a 6469 7265 6374 6f72 6965 7320   or.directories 
-000015b0: 7468 6174 206d 6174 6368 2074 6573 744d  that match testM
-000015c0: 6174 6368 2e20 5061 636b 6167 6520 6469  atch. Package di
-000015d0: 7363 6f76 6572 7920 6465 7363 656e 6473  scovery descends
-000015e0: 2061 6c6c 2074 6865 0a77 6179 2064 6f77   all the.way dow
-000015f0: 6e20 7468 6520 7472 6565 2c20 736f 2070  n the tree, so p
-00001600: 6163 6b61 6765 2e74 6573 7473 2061 6e64  ackage.tests and
-00001610: 2070 6163 6b61 6765 2e73 7562 2e74 6573   package.sub.tes
-00001620: 7473 2061 6e64 0a70 6163 6b61 6765 2e73  ts and.package.s
-00001630: 7562 2e73 7562 322e 7465 7374 7320 7769  ub.sub2.tests wi
-00001640: 6c6c 2061 6c6c 2062 6520 636f 6c6c 6563  ll all be collec
-00001650: 7465 642e 0a0a 5769 7468 696e 2061 2074  ted...Within a t
-00001660: 6573 7420 6469 7265 6374 6f72 7920 6f72  est directory or
-00001670: 2070 6163 6b61 6765 2c20 616e 7920 7079   package, any py
-00001680: 7468 6f6e 2073 6f75 7263 6520 6669 6c65  thon source file
-00001690: 206d 6174 6368 696e 670a 7465 7374 4d61   matching.testMa
-000016a0: 7463 6820 7769 6c6c 2062 6520 6578 616d  tch will be exam
-000016b0: 696e 6564 2066 6f72 2074 6573 7420 6361  ined for test ca
-000016c0: 7365 732e 2057 6974 6869 6e20 6120 7465  ses. Within a te
-000016d0: 7374 206d 6f64 756c 652c 0a66 756e 6374  st module,.funct
-000016e0: 696f 6e73 2061 6e64 2063 6c61 7373 6573  ions and classes
-000016f0: 2077 686f 7365 206e 616d 6573 206d 6174   whose names mat
-00001700: 6368 2074 6573 744d 6174 6368 2061 6e64  ch testMatch and
-00001710: 2054 6573 7443 6173 650a 7375 6263 6c61   TestCase.subcla
-00001720: 7373 6573 2077 6974 6820 616e 7920 6e61  sses with any na
-00001730: 6d65 2077 696c 6c20 6265 206c 6f61 6465  me will be loade
-00001740: 6420 616e 6420 6578 6563 7574 6564 2061  d and executed a
-00001750: 7320 7465 7374 732e 2054 6573 7473 0a6d  s tests. Tests.m
-00001760: 6179 2075 7365 2074 6865 2061 7373 6572  ay use the asser
-00001770: 7420 6b65 7977 6f72 6420 6f72 2072 6169  t keyword or rai
-00001780: 7365 2041 7373 6572 7469 6f6e 4572 726f  se AssertionErro
-00001790: 7273 2074 6f20 696e 6469 6361 7465 2074  rs to indicate t
-000017a0: 6573 740a 6661 696c 7572 652e 2054 6573  est.failure. Tes
-000017b0: 7443 6173 6520 7375 6263 6c61 7373 6573  tCase subclasses
-000017c0: 206d 6179 2064 6f20 7468 6520 7361 6d65   may do the same
-000017d0: 206f 7220 7573 6520 7468 6520 7661 7269   or use the vari
-000017e0: 6f75 730a 5465 7374 4361 7365 206d 6574  ous.TestCase met
-000017f0: 686f 6473 2061 7661 696c 6162 6c65 2e0a  hods available..
-00001800: 0a2a 2a49 7420 6973 2069 6d70 6f72 7461  .**It is importa
-00001810: 6e74 2074 6f20 6e6f 7465 2074 6861 7420  nt to note that 
-00001820: 7468 6520 6465 6661 756c 7420 6265 6861  the default beha
-00001830: 7669 6f72 206f 6620 6e6f 7365 2069 7320  vior of nose is 
-00001840: 746f 206e 6f74 0a69 6e63 6c75 6465 2074  to not.include t
-00001850: 6573 7473 2066 726f 6d20 6669 6c65 7320  ests from files 
-00001860: 7768 6963 6820 6172 6520 6578 6563 7574  which are execut
-00001870: 6162 6c65 2e2a 2a20 2054 6f20 696e 636c  able.**  To incl
-00001880: 7564 6520 7465 7374 730a 6672 6f6d 2073  ude tests.from s
-00001890: 7563 6820 6669 6c65 732c 2072 656d 6f76  uch files, remov
-000018a0: 6520 7468 6569 7220 6578 6563 7574 6162  e their executab
-000018b0: 6c65 2062 6974 206f 7220 7573 6520 7468  le bit or use th
-000018c0: 6520 2d2d 6578 6520 666c 6167 0a28 7365  e --exe flag.(se
-000018d0: 6520 274f 7074 696f 6e73 2720 7365 6374  e 'Options' sect
-000018e0: 696f 6e20 6265 6c6f 7729 2e0a 0a0a 5365  ion below)....Se
-000018f0: 6c65 6374 696e 6720 5465 7374 730a 2d2d  lecting Tests.--
-00001900: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a 0a54  -------------..T
-00001910: 6f20 7370 6563 6966 7920 7768 6963 6820  o specify which 
-00001920: 7465 7374 7320 746f 2072 756e 2c20 7061  tests to run, pa
-00001930: 7373 2074 6573 7420 6e61 6d65 7320 6f6e  ss test names on
-00001940: 2074 6865 2063 6f6d 6d61 6e64 206c 696e   the command lin
-00001950: 653a 0a0a 2020 206e 6f73 6574 6573 7473  e:..   nosetests
-00001960: 206f 6e6c 795f 7465 7374 5f74 6869 732e   only_test_this.
-00001970: 7079 0a0a 5465 7374 206e 616d 6573 2073  py..Test names s
-00001980: 7065 6369 6669 6564 206d 6179 2062 6520  pecified may be 
-00001990: 6669 6c65 206f 7220 6d6f 6475 6c65 206e  file or module n
-000019a0: 616d 6573 2c20 616e 6420 6d61 7920 6f70  ames, and may op
-000019b0: 7469 6f6e 616c 6c79 0a69 6e64 6963 6174  tionally.indicat
-000019c0: 6520 7468 6520 7465 7374 2063 6173 6520  e the test case 
-000019d0: 746f 2072 756e 2062 7920 7365 7061 7261  to run by separa
-000019e0: 7469 6e67 2074 6865 206d 6f64 756c 6520  ting the module 
-000019f0: 6f72 2066 696c 6520 6e61 6d65 0a66 726f  or file name.fro
-00001a00: 6d20 7468 6520 7465 7374 2063 6173 6520  m the test case 
-00001a10: 6e61 6d65 2077 6974 6820 6120 636f 6c6f  name with a colo
-00001a20: 6e2e 2046 696c 656e 616d 6573 206d 6179  n. Filenames may
-00001a30: 2062 6520 7265 6c61 7469 7665 206f 720a   be relative or.
-00001a40: 6162 736f 6c75 7465 2e20 4578 616d 706c  absolute. Exampl
-00001a50: 6573 3a0a 0a20 2020 6e6f 7365 7465 7374  es:..   nosetest
-00001a60: 7320 7465 7374 2e6d 6f64 756c 650a 2020  s test.module.  
-00001a70: 206e 6f73 6574 6573 7473 2061 6e6f 7468   nosetests anoth
-00001a80: 6572 2e74 6573 743a 5465 7374 4361 7365  er.test:TestCase
-00001a90: 2e74 6573 745f 6d65 7468 6f64 0a20 2020  .test_method.   
-00001aa0: 6e6f 7365 7465 7374 7320 612e 7465 7374  nosetests a.test
-00001ab0: 3a54 6573 7443 6173 650a 2020 206e 6f73  :TestCase.   nos
-00001ac0: 6574 6573 7473 202f 7061 7468 2f74 6f2f  etests /path/to/
-00001ad0: 7465 7374 2f66 696c 652e 7079 3a74 6573  test/file.py:tes
-00001ae0: 745f 6675 6e63 7469 6f6e 0a0a 596f 7520  t_function..You 
-00001af0: 6d61 7920 616c 736f 2063 6861 6e67 6520  may also change 
-00001b00: 7468 6520 776f 726b 696e 6720 6469 7265  the working dire
-00001b10: 6374 6f72 7920 7768 6572 6520 6e6f 7365  ctory where nose
-00001b20: 206c 6f6f 6b73 2066 6f72 2074 6573 7473   looks for tests
-00001b30: 0a62 7920 7573 696e 6720 7468 6520 2d77  .by using the -w
-00001b40: 2073 7769 7463 683a 0a0a 2020 206e 6f73   switch:..   nos
-00001b50: 6574 6573 7473 202d 7720 2f70 6174 682f  etests -w /path/
-00001b60: 746f 2f74 6573 7473 0a0a 4e6f 7465 2c20  to/tests..Note, 
-00001b70: 686f 7765 7665 722c 2074 6861 7420 7375  however, that su
-00001b80: 7070 6f72 7420 666f 7220 6d75 6c74 6970  pport for multip
-00001b90: 6c65 202d 7720 6172 6775 6d65 6e74 7320  le -w arguments 
-00001ba0: 6973 206e 6f77 0a64 6570 7265 6361 7465  is now.deprecate
-00001bb0: 6420 616e 6420 7769 6c6c 2062 6520 7265  d and will be re
-00001bc0: 6d6f 7665 6420 696e 2061 2066 7574 7572  moved in a futur
-00001bd0: 6520 7265 6c65 6173 652e 2041 7320 6f66  e release. As of
-00001be0: 206e 6f73 6520 302e 3130 2c0a 796f 7520   nose 0.10,.you 
-00001bf0: 6361 6e20 6765 7420 7468 6520 7361 6d65  can get the same
-00001c00: 2062 6568 6176 696f 7220 6279 2073 7065   behavior by spe
-00001c10: 6369 6679 696e 6720 7468 6520 7461 7267  cifying the targ
-00001c20: 6574 2064 6972 6563 746f 7269 6573 0a2a  et directories.*
-00001c30: 7769 7468 6f75 742a 2074 6865 202d 7720  without* the -w 
-00001c40: 7377 6974 6368 3a0a 0a20 2020 6e6f 7365  switch:..   nose
-00001c50: 7465 7374 7320 2f70 6174 682f 746f 2f74  tests /path/to/t
-00001c60: 6573 7473 202f 616e 6f74 6865 722f 7061  ests /another/pa
-00001c70: 7468 2f74 6f2f 7465 7374 730a 0a46 7572  th/to/tests..Fur
-00001c80: 7468 6572 2063 7573 746f 6d69 7a61 7469  ther customizati
-00001c90: 6f6e 206f 6620 7465 7374 2073 656c 6563  on of test selec
-00001ca0: 7469 6f6e 2061 6e64 206c 6f61 6469 6e67  tion and loading
-00001cb0: 2069 7320 706f 7373 6962 6c65 0a74 6872   is possible.thr
-00001cc0: 6f75 6768 2074 6865 2075 7365 206f 6620  ough the use of 
-00001cd0: 706c 7567 696e 732e 0a0a 5465 7374 2072  plugins...Test r
-00001ce0: 6573 756c 7420 6f75 7470 7574 2069 7320  esult output is 
-00001cf0: 6964 656e 7469 6361 6c20 746f 2074 6861  identical to tha
-00001d00: 7420 6f66 2075 6e69 7474 6573 742c 2065  t of unittest, e
-00001d10: 7863 6570 7420 666f 7220 7468 650a 6164  xcept for the.ad
-00001d20: 6469 7469 6f6e 616c 2066 6561 7475 7265  ditional feature
-00001d30: 7320 2865 7272 6f72 2063 6c61 7373 6573  s (error classes
-00001d40: 2c20 616e 6420 706c 7567 696e 2d73 7570  , and plugin-sup
-00001d50: 706c 6965 6420 6665 6174 7572 6573 2073  plied features s
-00001d60: 7563 680a 6173 206f 7574 7075 7420 6361  uch.as output ca
-00001d70: 7074 7572 6520 616e 6420 6173 7365 7274  pture and assert
-00001d80: 2069 6e74 726f 7370 6563 7469 6f6e 2920   introspection) 
-00001d90: 6465 7461 696c 6564 2069 6e20 7468 6520  detailed in the 
-00001da0: 6f70 7469 6f6e 730a 6265 6c6f 772e 0a0a  options.below...
-00001db0: 0a43 6f6e 6669 6775 7261 7469 6f6e 0a2d  .Configuration.-
-00001dc0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0a0a 496e  ------------..In
-00001dd0: 2061 6464 6974 696f 6e20 746f 2070 6173   addition to pas
-00001de0: 7369 6e67 2063 6f6d 6d61 6e64 2d6c 696e  sing command-lin
-00001df0: 6520 6f70 7469 6f6e 732c 2079 6f75 206d  e options, you m
-00001e00: 6179 2061 6c73 6f20 7075 740a 636f 6e66  ay also put.conf
-00001e10: 6967 7572 6174 696f 6e20 6f70 7469 6f6e  iguration option
-00001e20: 7320 696e 2079 6f75 7220 7072 6f6a 6563  s in your projec
-00001e30: 7420 2a73 6574 7570 2e63 6667 2a20 6669  t *setup.cfg* fi
-00001e40: 6c65 2c20 6f72 2061 202e 6e6f 7365 7263  le, or a .noserc
-00001e50: 0a6f 7220 6e6f 7365 2e63 6667 2066 696c  .or nose.cfg fil
-00001e60: 6520 696e 2079 6f75 7220 686f 6d65 2064  e in your home d
-00001e70: 6972 6563 746f 7279 2e20 496e 2061 6e79  irectory. In any
-00001e80: 206f 6620 7468 6573 6520 7374 616e 6461   of these standa
-00001e90: 7264 2069 6e69 2d0a 7374 796c 6520 636f  rd ini-.style co
-00001ea0: 6e66 6967 2066 696c 6573 2c20 796f 7520  nfig files, you 
-00001eb0: 7075 7420 796f 7572 206e 6f73 6574 6573  put your nosetes
-00001ec0: 7473 2063 6f6e 6669 6775 7261 7469 6f6e  ts configuration
-00001ed0: 2069 6e20 610a 225b 6e6f 7365 7465 7374   in a."[nosetest
-00001ee0: 735d 2220 7365 6374 696f 6e2e 204f 7074  s]" section. Opt
-00001ef0: 696f 6e73 2061 7265 2074 6865 2073 616d  ions are the sam
-00001f00: 6520 6173 206f 6e20 7468 6520 636f 6d6d  e as on the comm
-00001f10: 616e 6420 6c69 6e65 2c0a 7769 7468 2074  and line,.with t
-00001f20: 6865 202d 2d20 7072 6566 6978 2072 656d  he -- prefix rem
-00001f30: 6f76 6564 2e20 466f 7220 6f70 7469 6f6e  oved. For option
-00001f40: 7320 7468 6174 2061 7265 2073 696d 706c  s that are simpl
-00001f50: 6520 7377 6974 6368 6573 2c20 796f 750a  e switches, you.
-00001f60: 6d75 7374 2073 7570 706c 7920 6120 7661  must supply a va
-00001f70: 6c75 653a 0a0a 2020 205b 6e6f 7365 7465  lue:..   [nosete
-00001f80: 7374 735d 0a20 2020 7665 7262 6f73 6974  sts].   verbosit
-00001f90: 793d 330a 2020 2077 6974 682d 646f 6374  y=3.   with-doct
-00001fa0: 6573 743d 310a 0a41 6c6c 2063 6f6e 6669  est=1..All confi
-00001fb0: 6775 7261 7469 6f6e 2066 696c 6573 2074  guration files t
-00001fc0: 6861 7420 6172 6520 666f 756e 6420 7769  hat are found wi
-00001fd0: 6c6c 2062 6520 6c6f 6164 6564 2061 6e64  ll be loaded and
-00001fe0: 2074 6865 6972 0a6f 7074 696f 6e73 2063   their.options c
-00001ff0: 6f6d 6269 6e65 642e 2059 6f75 2063 616e  ombined. You can
-00002000: 206f 7665 7272 6964 6520 7468 6520 7374   override the st
-00002010: 616e 6461 7264 2063 6f6e 6669 6720 6669  andard config fi
-00002020: 6c65 206c 6f61 6469 6e67 0a77 6974 6820  le loading.with 
-00002030: 7468 6520 222d 6322 206f 7074 696f 6e2e  the "-c" option.
-00002040: 0a0a 0a55 7369 6e67 2050 6c75 6769 6e73  ...Using Plugins
-00002050: 0a2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0a0a  .-------------..
-00002060: 5468 6572 6520 6172 6520 6e75 6d65 726f  There are numero
-00002070: 7573 206e 6f73 6520 706c 7567 696e 7320  us nose plugins 
-00002080: 6176 6169 6c61 626c 6520 7669 6120 6561  available via ea
-00002090: 7379 5f69 6e73 7461 6c6c 2061 6e64 0a65  sy_install and.e
-000020a0: 6c73 6577 6865 7265 2e20 546f 2075 7365  lsewhere. To use
-000020b0: 2061 2070 6c75 6769 6e2c 206a 7573 7420   a plugin, just 
-000020c0: 696e 7374 616c 6c20 6974 2e20 5468 6520  install it. The 
-000020d0: 706c 7567 696e 2077 696c 6c20 6164 640a  plugin will add.
-000020e0: 636f 6d6d 616e 6420 6c69 6e65 206f 7074  command line opt
-000020f0: 696f 6e73 2074 6f20 6e6f 7365 7465 7374  ions to nosetest
-00002100: 732e 2054 6f20 7665 7269 6679 2074 6861  s. To verify tha
-00002110: 7420 7468 6520 706c 7567 696e 2069 730a  t the plugin is.
-00002120: 696e 7374 616c 6c65 642c 2072 756e 3a0a  installed, run:.
-00002130: 0a20 2020 6e6f 7365 7465 7374 7320 2d2d  .   nosetests --
-00002140: 706c 7567 696e 730a 0a59 6f75 2063 616e  plugins..You can
-00002150: 2061 6464 202d 7620 6f72 202d 7676 2074   add -v or -vv t
-00002160: 6f20 7468 6174 2063 6f6d 6d61 6e64 2074  o that command t
-00002170: 6f20 7368 6f77 206d 6f72 6520 696e 666f  o show more info
-00002180: 726d 6174 696f 6e20 6162 6f75 740a 6561  rmation about.ea
-00002190: 6368 2070 6c75 6769 6e2e 0a0a 4966 2079  ch plugin...If y
-000021a0: 6f75 2061 7265 2072 756e 6e69 6e67 206e  ou are running n
-000021b0: 6f73 652e 6d61 696e 2829 206f 7220 6e6f  ose.main() or no
-000021c0: 7365 2e72 756e 2829 2066 726f 6d20 6120  se.run() from a 
-000021d0: 7363 7269 7074 2c20 796f 7520 6361 6e0a  script, you can.
-000021e0: 7370 6563 6966 7920 6120 6c69 7374 206f  specify a list o
-000021f0: 6620 706c 7567 696e 7320 746f 2075 7365  f plugins to use
-00002200: 2062 7920 7061 7373 696e 6720 6120 6c69   by passing a li
-00002210: 7374 206f 6620 706c 7567 696e 7320 7769  st of plugins wi
-00002220: 7468 2074 6865 0a70 6c75 6769 6e73 206b  th the.plugins k
-00002230: 6579 776f 7264 2061 7267 756d 656e 742e  eyword argument.
-00002240: 0a0a 0a4f 7074 696f 6e73 0a2d 2d2d 2d2d  ...Options.-----
-00002250: 2d2d 0a0a 2d56 2c20 2d2d 7665 7273 696f  --..-V, --versio
-00002260: 6e0a 0a20 2020 4f75 7470 7574 206e 6f73  n..   Output nos
-00002270: 6520 7665 7273 696f 6e20 616e 6420 6578  e version and ex
-00002280: 6974 0a0a 2d70 2c20 2d2d 706c 7567 696e  it..-p, --plugin
-00002290: 730a 0a20 2020 4f75 7470 7574 206c 6973  s..   Output lis
-000022a0: 7420 6f66 2061 7661 696c 6162 6c65 2070  t of available p
-000022b0: 6c75 6769 6e73 2061 6e64 2065 7869 742e  lugins and exit.
-000022c0: 2043 6f6d 6269 6e65 2077 6974 6820 6869   Combine with hi
-000022d0: 6768 6572 0a20 2020 7665 7262 6f73 6974  gher.   verbosit
-000022e0: 7920 666f 7220 6772 6561 7465 7220 6465  y for greater de
-000022f0: 7461 696c 0a0a 2d76 3d44 4546 4155 4c54  tail..-v=DEFAULT
-00002300: 2c20 2d2d 7665 7262 6f73 653d 4445 4641  , --verbose=DEFA
-00002310: 554c 540a 0a20 2020 4265 206d 6f72 6520  ULT..   Be more 
-00002320: 7665 7262 6f73 652e 205b 4e4f 5345 5f56  verbose. [NOSE_V
-00002330: 4552 424f 5345 5d0a 0a2d 2d76 6572 626f  ERBOSE]..--verbo
-00002340: 7369 7479 3d56 4552 424f 5349 5459 0a0a  sity=VERBOSITY..
-00002350: 2020 2053 6574 2076 6572 626f 7369 7479     Set verbosity
-00002360: 3b20 2d2d 7665 7262 6f73 6974 793d 3220  ; --verbosity=2 
-00002370: 6973 2074 6865 2073 616d 6520 6173 202d  is the same as -
-00002380: 760a 0a2d 713d 4445 4641 554c 542c 202d  v..-q=DEFAULT, -
-00002390: 2d71 7569 6574 3d44 4546 4155 4c54 0a0a  -quiet=DEFAULT..
-000023a0: 2020 2042 6520 6c65 7373 2076 6572 626f     Be less verbo
-000023b0: 7365 0a0a 2d63 3d46 494c 4553 2c20 2d2d  se..-c=FILES, --
-000023c0: 636f 6e66 6967 3d46 494c 4553 0a0a 2020  config=FILES..  
-000023d0: 204c 6f61 6420 636f 6e66 6967 7572 6174   Load configurat
-000023e0: 696f 6e20 6672 6f6d 2063 6f6e 6669 6720  ion from config 
-000023f0: 6669 6c65 2873 292e 204d 6179 2062 6520  file(s). May be 
-00002400: 7370 6563 6966 6965 6420 6d75 6c74 6970  specified multip
-00002410: 6c65 0a20 2020 7469 6d65 733b 2069 6e20  le.   times; in 
-00002420: 7468 6174 2063 6173 652c 2061 6c6c 2063  that case, all c
-00002430: 6f6e 6669 6720 6669 6c65 7320 7769 6c6c  onfig files will
-00002440: 2062 6520 6c6f 6164 6564 2061 6e64 2063   be loaded and c
-00002450: 6f6d 6269 6e65 640a 0a2d 773d 5748 4552  ombined..-w=WHER
-00002460: 452c 202d 2d77 6865 7265 3d57 4845 5245  E, --where=WHERE
-00002470: 0a0a 2020 204c 6f6f 6b20 666f 7220 7465  ..   Look for te
-00002480: 7374 7320 696e 2074 6869 7320 6469 7265  sts in this dire
-00002490: 6374 6f72 792e 204d 6179 2062 6520 7370  ctory. May be sp
-000024a0: 6563 6966 6965 6420 6d75 6c74 6970 6c65  ecified multiple
-000024b0: 2074 696d 6573 2e0a 2020 2054 6865 2066   times..   The f
-000024c0: 6972 7374 2064 6972 6563 746f 7279 2070  irst directory p
-000024d0: 6173 7365 6420 7769 6c6c 2062 6520 7573  assed will be us
-000024e0: 6564 2061 7320 7468 6520 776f 726b 696e  ed as the workin
-000024f0: 6720 6469 7265 6374 6f72 792c 0a20 2020  g directory,.   
-00002500: 696e 2070 6c61 6365 206f 6620 7468 6520  in place of the 
-00002510: 6375 7272 656e 7420 776f 726b 696e 6720  current working 
-00002520: 6469 7265 6374 6f72 792c 2077 6869 6368  directory, which
-00002530: 2069 7320 7468 6520 6465 6661 756c 742e   is the default.
-00002540: 0a20 2020 4f74 6865 7273 2077 696c 6c20  .   Others will 
-00002550: 6265 2061 6464 6564 2074 6f20 7468 6520  be added to the 
-00002560: 6c69 7374 206f 6620 7465 7374 7320 746f  list of tests to
-00002570: 2065 7865 6375 7465 2e20 5b4e 4f53 455f   execute. [NOSE_
-00002580: 5748 4552 455d 0a0a 2d2d 7079 3377 6865  WHERE]..--py3whe
-00002590: 7265 3d50 5933 5748 4552 450a 0a20 2020  re=PY3WHERE..   
-000025a0: 4c6f 6f6b 2066 6f72 2074 6573 7473 2069  Look for tests i
-000025b0: 6e20 7468 6973 2064 6972 6563 746f 7279  n this directory
-000025c0: 2075 6e64 6572 2050 7974 686f 6e20 332e   under Python 3.
-000025d0: 782e 2046 756e 6374 696f 6e73 2074 6865  x. Functions the
-000025e0: 0a20 2020 7361 6d65 2061 7320 2777 6865  .   same as 'whe
-000025f0: 7265 272c 2062 7574 206f 6e6c 7920 6170  re', but only ap
-00002600: 706c 6965 7320 6966 2072 756e 6e69 6e67  plies if running
-00002610: 2075 6e64 6572 2050 7974 686f 6e20 332e   under Python 3.
-00002620: 7820 6f72 0a20 2020 6162 6f76 652e 2020  x or.   above.  
-00002630: 4e6f 7465 2074 6861 742c 2069 6620 7072  Note that, if pr
-00002640: 6573 656e 7420 756e 6465 7220 332e 782c  esent under 3.x,
-00002650: 2074 6869 7320 6f70 7469 6f6e 2063 6f6d   this option com
-00002660: 706c 6574 656c 790a 2020 2072 6570 6c61  pletely.   repla
-00002670: 6365 7320 616e 7920 6469 7265 6374 6f72  ces any director
-00002680: 6965 7320 7370 6563 6966 6965 6420 7769  ies specified wi
-00002690: 7468 2027 7768 6572 6527 2c20 736f 2074  th 'where', so t
-000026a0: 6865 2027 7768 6572 6527 0a20 2020 6f70  he 'where'.   op
-000026b0: 7469 6f6e 2062 6563 6f6d 6573 2069 6e65  tion becomes ine
-000026c0: 6666 6563 7469 7665 2e20 5b4e 4f53 455f  ffective. [NOSE_
-000026d0: 5059 3357 4845 5245 5d0a 0a2d 6d3d 5245  PY3WHERE]..-m=RE
-000026e0: 4745 582c 202d 2d6d 6174 6368 3d52 4547  GEX, --match=REG
-000026f0: 4558 2c20 2d2d 7465 7374 6d61 7463 683d  EX, --testmatch=
-00002700: 5245 4745 580a 0a20 2020 4669 6c65 732c  REGEX..   Files,
-00002710: 2064 6972 6563 746f 7269 6573 2c20 6675   directories, fu
-00002720: 6e63 7469 6f6e 206e 616d 6573 2c20 616e  nction names, an
-00002730: 6420 636c 6173 7320 6e61 6d65 7320 7468  d class names th
-00002740: 6174 206d 6174 6368 2074 6869 730a 2020  at match this.  
-00002750: 2072 6567 756c 6172 2065 7870 7265 7373   regular express
-00002760: 696f 6e20 6172 6520 636f 6e73 6964 6572  ion are consider
-00002770: 6564 2074 6573 7473 2e20 2044 6566 6175  ed tests.  Defau
-00002780: 6c74 3a0a 2020 2028 3f3a 5e7c 5b62 5f2e  lt:.   (?:^|[b_.
-00002790: 2f2d 5d29 5b54 745d 6573 7420 5b4e 4f53  /-])[Tt]est [NOS
-000027a0: 455f 5445 5354 4d41 5443 485d 0a0a 2d2d  E_TESTMATCH]..--
-000027b0: 7465 7374 733d 4e41 4d45 530a 0a20 2020  tests=NAMES..   
-000027c0: 5275 6e20 7468 6573 6520 7465 7374 7320  Run these tests 
-000027d0: 2863 6f6d 6d61 2d73 6570 6172 6174 6564  (comma-separated
-000027e0: 206c 6973 7429 2e20 5468 6973 2061 7267   list). This arg
-000027f0: 756d 656e 7420 6973 2075 7365 6675 6c0a  ument is useful.
-00002800: 2020 206d 6169 6e6c 7920 6672 6f6d 2063     mainly from c
-00002810: 6f6e 6669 6775 7261 7469 6f6e 2066 696c  onfiguration fil
-00002820: 6573 3b20 6f6e 2074 6865 2063 6f6d 6d61  es; on the comma
-00002830: 6e64 206c 696e 652c 206a 7573 7420 7061  nd line, just pa
-00002840: 7373 2074 6865 0a20 2020 7465 7374 7320  ss the.   tests 
-00002850: 746f 2072 756e 2061 7320 6164 6469 7469  to run as additi
-00002860: 6f6e 616c 2061 7267 756d 656e 7473 2077  onal arguments w
-00002870: 6974 6820 6e6f 2073 7769 7463 682e 0a0a  ith no switch...
-00002880: 2d6c 3d44 4546 4155 4c54 2c20 2d2d 6465  -l=DEFAULT, --de
-00002890: 6275 673d 4445 4641 554c 540a 0a20 2020  bug=DEFAULT..   
-000028a0: 4163 7469 7661 7465 2064 6562 7567 206c  Activate debug l
-000028b0: 6f67 6769 6e67 2066 6f72 206f 6e65 206f  ogging for one o
-000028c0: 7220 6d6f 7265 2073 7973 7465 6d73 2e20  r more systems. 
-000028d0: 4176 6169 6c61 626c 6520 6465 6275 670a  Available debug.
-000028e0: 2020 206c 6f67 6765 7273 3a20 6e6f 7365     loggers: nose
-000028f0: 2c20 6e6f 7365 2e69 6d70 6f72 7465 722c  , nose.importer,
-00002900: 206e 6f73 652e 696e 7370 6563 746f 722c   nose.inspector,
-00002910: 206e 6f73 652e 706c 7567 696e 732c 0a20   nose.plugins,. 
-00002920: 2020 6e6f 7365 2e72 6573 756c 7420 616e    nose.result an
-00002930: 6420 6e6f 7365 2e73 656c 6563 746f 722e  d nose.selector.
-00002940: 2053 6570 6172 6174 6520 6d75 6c74 6970   Separate multip
-00002950: 6c65 206e 616d 6573 2077 6974 6820 610a  le names with a.
-00002960: 2020 2063 6f6d 6d61 2e0a 0a2d 2d64 6562     comma...--deb
-00002970: 7567 2d6c 6f67 3d46 494c 450a 0a20 2020  ug-log=FILE..   
-00002980: 4c6f 6720 6465 6275 6720 6d65 7373 6167  Log debug messag
-00002990: 6573 2074 6f20 7468 6973 2066 696c 6520  es to this file 
-000029a0: 2864 6566 6175 6c74 3a20 7379 732e 7374  (default: sys.st
-000029b0: 6465 7272 290a 0a2d 2d6c 6f67 6769 6e67  derr)..--logging
-000029c0: 2d63 6f6e 6669 673d 4649 4c45 2c20 2d2d  -config=FILE, --
-000029d0: 6c6f 672d 636f 6e66 6967 3d46 494c 450a  log-config=FILE.
-000029e0: 0a20 2020 4c6f 6164 206c 6f67 6769 6e67  .   Load logging
-000029f0: 2063 6f6e 6669 6720 6672 6f6d 2074 6869   config from thi
-00002a00: 7320 6669 6c65 202d 2d20 6279 7061 7373  s file -- bypass
-00002a10: 6573 2061 6c6c 206f 7468 6572 206c 6f67  es all other log
-00002a20: 6769 6e67 0a20 2020 636f 6e66 6967 2073  ging.   config s
-00002a30: 6574 7469 6e67 732e 0a0a 2d49 3d52 4547  ettings...-I=REG
-00002a40: 4558 2c20 2d2d 6967 6e6f 7265 2d66 696c  EX, --ignore-fil
-00002a50: 6573 3d52 4547 4558 0a0a 2020 2043 6f6d  es=REGEX..   Com
-00002a60: 706c 6574 656c 7920 6967 6e6f 7265 2061  pletely ignore a
-00002a70: 6e79 2066 696c 6520 7468 6174 206d 6174  ny file that mat
-00002a80: 6368 6573 2074 6869 7320 7265 6775 6c61  ches this regula
-00002a90: 7220 6578 7072 6573 7369 6f6e 2e0a 2020  r expression..  
-00002aa0: 2054 616b 6573 2070 7265 6365 6465 6e63   Takes precedenc
-00002ab0: 6520 6f76 6572 2061 6e79 206f 7468 6572  e over any other
-00002ac0: 2073 6574 7469 6e67 7320 6f72 2070 6c75   settings or plu
-00002ad0: 6769 6e73 2e20 5370 6563 6966 7969 6e67  gins. Specifying
-00002ae0: 0a20 2020 7468 6973 206f 7074 696f 6e20  .   this option 
-00002af0: 7769 6c6c 2072 6570 6c61 6365 2074 6865  will replace the
-00002b00: 2064 6566 6175 6c74 2073 6574 7469 6e67   default setting
-00002b10: 2e20 5370 6563 6966 7920 7468 6973 206f  . Specify this o
-00002b20: 7074 696f 6e0a 2020 206d 756c 7469 706c  ption.   multipl
-00002b30: 6520 7469 6d65 7320 746f 2061 6464 206d  e times to add m
-00002b40: 6f72 6520 7265 6775 6c61 7220 6578 7072  ore regular expr
-00002b50: 6573 7369 6f6e 7320 5b4e 4f53 455f 4947  essions [NOSE_IG
-00002b60: 4e4f 5245 5f46 494c 4553 5d0a 0a2d 653d  NORE_FILES]..-e=
-00002b70: 5245 4745 582c 202d 2d65 7863 6c75 6465  REGEX, --exclude
-00002b80: 3d52 4547 4558 0a0a 2020 2044 6f20 6e6f  =REGEX..   Do no
-00002b90: 7420 7275 6e20 7465 7374 7320 7468 6174  t run tests that
-00002ba0: 206d 6174 6368 2072 6567 756c 6172 2065   match regular e
-00002bb0: 7870 7265 7373 696f 6e20 5b4e 4f53 455f  xpression [NOSE_
-00002bc0: 4558 434c 5544 455d 0a0a 2d69 3d52 4547  EXCLUDE]..-i=REG
-00002bd0: 4558 2c20 2d2d 696e 636c 7564 653d 5245  EX, --include=RE
-00002be0: 4745 580a 0a20 2020 5468 6973 2072 6567  GEX..   This reg
-00002bf0: 756c 6172 2065 7870 7265 7373 696f 6e20  ular expression 
-00002c00: 7769 6c6c 2062 6520 6170 706c 6965 6420  will be applied 
-00002c10: 746f 2066 696c 6573 2c20 6469 7265 6374  to files, direct
-00002c20: 6f72 6965 732c 0a20 2020 6675 6e63 7469  ories,.   functi
-00002c30: 6f6e 206e 616d 6573 2c20 616e 6420 636c  on names, and cl
-00002c40: 6173 7320 6e61 6d65 7320 666f 7220 6120  ass names for a 
-00002c50: 6368 616e 6365 2074 6f20 696e 636c 7564  chance to includ
-00002c60: 6520 6164 6469 7469 6f6e 616c 0a20 2020  e additional.   
-00002c70: 7465 7374 7320 7468 6174 2064 6f20 6e6f  tests that do no
-00002c80: 7420 6d61 7463 6820 5445 5354 4d41 5443  t match TESTMATC
-00002c90: 482e 2020 5370 6563 6966 7920 7468 6973  H.  Specify this
-00002ca0: 206f 7074 696f 6e20 6d75 6c74 6970 6c65   option multiple
-00002cb0: 0a20 2020 7469 6d65 7320 746f 2061 6464  .   times to add
-00002cc0: 206d 6f72 6520 7265 6775 6c61 7220 6578   more regular ex
-00002cd0: 7072 6573 7369 6f6e 7320 5b4e 4f53 455f  pressions [NOSE_
-00002ce0: 494e 434c 5544 455d 0a0a 2d78 2c20 2d2d  INCLUDE]..-x, --
-00002cf0: 7374 6f70 0a0a 2020 2053 746f 7020 7275  stop..   Stop ru
-00002d00: 6e6e 696e 6720 7465 7374 7320 6166 7465  nning tests afte
-00002d10: 7220 7468 6520 6669 7273 7420 6572 726f  r the first erro
-00002d20: 7220 6f72 2066 6169 6c75 7265 0a0a 2d50  r or failure..-P
-00002d30: 2c20 2d2d 6e6f 2d70 6174 682d 6164 6a75  , --no-path-adju
-00002d40: 7374 6d65 6e74 0a0a 2020 2044 6f20 6e6f  stment..   Do no
-00002d50: 7420 6d61 6b65 2061 6e79 2063 6861 6e67  t make any chang
-00002d60: 6573 2074 6f20 7379 732e 7061 7468 2077  es to sys.path w
-00002d70: 6865 6e20 6c6f 6164 696e 6720 7465 7374  hen loading test
-00002d80: 7320 5b4e 4f53 455f 4e4f 5041 5448 5d0a  s [NOSE_NOPATH].
-00002d90: 0a2d 2d65 7865 0a0a 2020 204c 6f6f 6b20  .--exe..   Look 
-00002da0: 666f 7220 7465 7374 7320 696e 2070 7974  for tests in pyt
-00002db0: 686f 6e20 6d6f 6475 6c65 7320 7468 6174  hon modules that
-00002dc0: 2061 7265 2065 7865 6375 7461 626c 652e   are executable.
-00002dd0: 204e 6f72 6d61 6c0a 2020 2062 6568 6176   Normal.   behav
-00002de0: 696f 7220 6973 2074 6f20 6578 636c 7564  ior is to exclud
-00002df0: 6520 6578 6563 7574 6162 6c65 206d 6f64  e executable mod
-00002e00: 756c 6573 2c20 7369 6e63 6520 7468 6579  ules, since they
-00002e10: 206d 6179 206e 6f74 2062 650a 2020 2069   may not be.   i
-00002e20: 6d70 6f72 742d 7361 6665 205b 4e4f 5345  mport-safe [NOSE
-00002e30: 5f49 4e43 4c55 4445 5f45 5845 5d0a 0a2d  _INCLUDE_EXE]..-
-00002e40: 2d6e 6f65 7865 0a0a 2020 2044 4f20 4e4f  -noexe..   DO NO
-00002e50: 5420 6c6f 6f6b 2066 6f72 2074 6573 7473  T look for tests
-00002e60: 2069 6e20 7079 7468 6f6e 206d 6f64 756c   in python modul
-00002e70: 6573 2074 6861 7420 6172 6520 6578 6563  es that are exec
-00002e80: 7574 6162 6c65 2e20 2854 6865 0a20 2020  utable. (The.   
-00002e90: 6465 6661 756c 7420 6f6e 2074 6865 2077  default on the w
-00002ea0: 696e 646f 7773 2070 6c61 7466 6f72 6d20  indows platform 
-00002eb0: 6973 2074 6f20 646f 2073 6f2e 290a 0a2d  is to do so.)..-
-00002ec0: 2d74 7261 7665 7273 652d 6e61 6d65 7370  -traverse-namesp
-00002ed0: 6163 650a 0a20 2020 5472 6176 6572 7365  ace..   Traverse
-00002ee0: 2074 6872 6f75 6768 2061 6c6c 2070 6174   through all pat
-00002ef0: 6820 656e 7472 6965 7320 6f66 2061 206e  h entries of a n
-00002f00: 616d 6573 7061 6365 2070 6163 6b61 6765  amespace package
-00002f10: 0a0a 2d2d 6669 7273 742d 7061 636b 6167  ..--first-packag
-00002f20: 652d 7769 6e73 2c20 2d2d 6669 7273 742d  e-wins, --first-
-00002f30: 706b 672d 7769 6e73 2c20 2d2d 3173 742d  pkg-wins, --1st-
-00002f40: 706b 672d 7769 6e73 0a0a 2020 2054 6865  pkg-wins..   The
-00002f50: 206e 6f73 6520 696d 706f 7274 6572 2077   nose importer w
-00002f60: 696c 6c20 6e6f 726d 616c 6c79 2065 7669  ill normally evi
-00002f70: 6374 2061 2070 6163 6b61 6765 2066 726f  ct a package fro
-00002f80: 6d20 7379 732e 6d6f 6475 6c65 7320 6966  m sys.modules if
-00002f90: 0a20 2020 6974 2073 6565 7320 6120 7061  .   it sees a pa
-00002fa0: 636b 6167 6520 7769 7468 2074 6865 2073  ckage with the s
-00002fb0: 616d 6520 6e61 6d65 2069 6e20 6120 6469  ame name in a di
-00002fc0: 6666 6572 656e 7420 6c6f 6361 7469 6f6e  fferent location
-00002fd0: 2e20 5365 740a 2020 2074 6869 7320 6f70  . Set.   this op
-00002fe0: 7469 6f6e 2074 6f20 6469 7361 626c 6520  tion to disable 
-00002ff0: 7468 6174 2062 6568 6176 696f 722e 0a0a  that behavior...
-00003000: 2d2d 6e6f 2d62 7974 652d 636f 6d70 696c  --no-byte-compil
-00003010: 650a 0a20 2020 5072 6576 656e 7420 6e6f  e..   Prevent no
-00003020: 7365 2066 726f 6d20 6279 7465 2d63 6f6d  se from byte-com
-00003030: 7069 6c69 6e67 2074 6865 2073 6f75 7263  piling the sourc
-00003040: 6520 696e 746f 202e 7079 6320 6669 6c65  e into .pyc file
-00003050: 7320 7768 696c 650a 2020 206e 6f73 6520  s while.   nose 
-00003060: 6973 2073 6361 6e6e 696e 6720 666f 7220  is scanning for 
-00003070: 616e 6420 7275 6e6e 696e 6720 7465 7374  and running test
-00003080: 732e 0a0a 2d61 3d41 5454 522c 202d 2d61  s...-a=ATTR, --a
-00003090: 7474 723d 4154 5452 0a0a 2020 2052 756e  ttr=ATTR..   Run
-000030a0: 206f 6e6c 7920 7465 7374 7320 7468 6174   only tests that
-000030b0: 2068 6176 6520 6174 7472 6962 7574 6573   have attributes
-000030c0: 2073 7065 6369 6669 6564 2062 7920 4154   specified by AT
-000030d0: 5452 205b 4e4f 5345 5f41 5454 525d 0a0a  TR [NOSE_ATTR]..
-000030e0: 2d41 3d45 5850 522c 202d 2d65 7661 6c2d  -A=EXPR, --eval-
-000030f0: 6174 7472 3d45 5850 520a 0a20 2020 5275  attr=EXPR..   Ru
-00003100: 6e20 6f6e 6c79 2074 6573 7473 2066 6f72  n only tests for
-00003110: 2077 686f 7365 2061 7474 7269 6275 7465   whose attribute
-00003120: 7320 7468 6520 5079 7468 6f6e 2065 7870  s the Python exp
-00003130: 7265 7373 696f 6e20 4558 5052 0a20 2020  ression EXPR.   
-00003140: 6576 616c 7561 7465 7320 746f 2054 7275  evaluates to Tru
-00003150: 6520 5b4e 4f53 455f 4556 414c 5f41 5454  e [NOSE_EVAL_ATT
-00003160: 525d 0a0a 2d73 2c20 2d2d 6e6f 6361 7074  R]..-s, --nocapt
-00003170: 7572 650a 0a20 2020 446f 206e 6f74 2063  ure..   Do not c
-00003180: 6170 7475 7265 2073 7464 6f75 7420 2861  apture stdout (a
-00003190: 6e79 2073 7464 6f75 7420 6f75 7470 7574  ny stdout output
-000031a0: 2077 696c 6c20 6265 2070 7269 6e74 6564   will be printed
-000031b0: 0a20 2020 696d 6d65 6469 6174 656c 7929  .   immediately)
-000031c0: 205b 4e4f 5345 5f4e 4f43 4150 5455 5245   [NOSE_NOCAPTURE
-000031d0: 5d0a 0a2d 2d6e 6f6c 6f67 6361 7074 7572  ]..--nologcaptur
-000031e0: 650a 0a20 2020 4469 7361 626c 6520 6c6f  e..   Disable lo
-000031f0: 6767 696e 6720 6361 7074 7572 6520 706c  gging capture pl
-00003200: 7567 696e 2e20 4c6f 6767 696e 6720 636f  ugin. Logging co
-00003210: 6e66 6967 7572 6174 696f 6e20 7769 6c6c  nfiguration will
-00003220: 2062 6520 6c65 6674 0a20 2020 696e 7461   be left.   inta
-00003230: 6374 2e20 5b4e 4f53 455f 4e4f 4c4f 4743  ct. [NOSE_NOLOGC
-00003240: 4150 5455 5245 5d0a 0a2d 2d6c 6f67 6769  APTURE]..--loggi
-00003250: 6e67 2d66 6f72 6d61 743d 464f 524d 4154  ng-format=FORMAT
-00003260: 0a0a 2020 2053 7065 6369 6679 2063 7573  ..   Specify cus
-00003270: 746f 6d20 666f 726d 6174 2074 6f20 7072  tom format to pr
-00003280: 696e 7420 7374 6174 656d 656e 7473 2e20  int statements. 
-00003290: 5573 6573 2074 6865 2073 616d 6520 666f  Uses the same fo
-000032a0: 726d 6174 2061 730a 2020 2075 7365 6420  rmat as.   used 
-000032b0: 6279 2073 7461 6e64 6172 6420 6c6f 6767  by standard logg
-000032c0: 696e 6720 6861 6e64 6c65 7273 2e20 5b4e  ing handlers. [N
-000032d0: 4f53 455f 4c4f 4746 4f52 4d41 545d 0a0a  OSE_LOGFORMAT]..
-000032e0: 2d2d 6c6f 6767 696e 672d 6461 7465 666d  --logging-datefm
-000032f0: 743d 464f 524d 4154 0a0a 2020 2053 7065  t=FORMAT..   Spe
-00003300: 6369 6679 2063 7573 746f 6d20 6461 7465  cify custom date
-00003310: 2f74 696d 6520 666f 726d 6174 2074 6f20  /time format to 
-00003320: 7072 696e 7420 7374 6174 656d 656e 7473  print statements
-00003330: 2e20 5573 6573 2074 6865 2073 616d 650a  . Uses the same.
-00003340: 2020 2066 6f72 6d61 7420 6173 2075 7365     format as use
-00003350: 6420 6279 2073 7461 6e64 6172 6420 6c6f  d by standard lo
-00003360: 6767 696e 6720 6861 6e64 6c65 7273 2e20  gging handlers. 
-00003370: 5b4e 4f53 455f 4c4f 4744 4154 4546 4d54  [NOSE_LOGDATEFMT
-00003380: 5d0a 0a2d 2d6c 6f67 6769 6e67 2d66 696c  ]..--logging-fil
-00003390: 7465 723d 4649 4c54 4552 0a0a 2020 2053  ter=FILTER..   S
-000033a0: 7065 6369 6679 2077 6869 6368 2073 7461  pecify which sta
-000033b0: 7465 6d65 6e74 7320 746f 2066 696c 7465  tements to filte
-000033c0: 7220 696e 2f6f 7574 2e20 4279 2064 6566  r in/out. By def
-000033d0: 6175 6c74 2c20 6576 6572 7974 6869 6e67  ault, everything
-000033e0: 0a20 2020 6973 2063 6170 7475 7265 642e  .   is captured.
-000033f0: 2049 6620 7468 6520 6f75 7470 7574 2069   If the output i
-00003400: 7320 746f 6f20 7665 7262 6f73 652c 2075  s too verbose, u
-00003410: 7365 2074 6869 7320 6f70 7469 6f6e 2074  se this option t
-00003420: 6f0a 2020 2066 696c 7465 7220 6f75 7420  o.   filter out 
-00003430: 6e65 6564 6c65 7373 206f 7574 7075 742e  needless output.
-00003440: 2045 7861 6d70 6c65 3a20 6669 6c74 6572   Example: filter
-00003450: 3d66 6f6f 2077 696c 6c20 6361 7074 7572  =foo will captur
-00003460: 650a 2020 2073 7461 7465 6d65 6e74 7320  e.   statements 
-00003470: 6973 7375 6564 204f 4e4c 5920 746f 2020  issued ONLY to  
-00003480: 666f 6f20 6f72 2066 6f6f 2e77 6861 742e  foo or foo.what.
-00003490: 6576 6572 2e73 7562 2062 7574 206e 6f74  ever.sub but not
-000034a0: 2066 6f6f 6261 720a 2020 206f 7220 6f74   foobar.   or ot
-000034b0: 6865 7220 6c6f 6767 6572 2e20 5370 6563  her logger. Spec
-000034c0: 6966 7920 6d75 6c74 6970 6c65 206c 6f67  ify multiple log
-000034d0: 6765 7273 2077 6974 6820 636f 6d6d 613a  gers with comma:
-000034e0: 0a20 2020 6669 6c74 6572 3d66 6f6f 2c62  .   filter=foo,b
-000034f0: 6172 2c62 617a 2e20 4966 2061 6e79 206c  ar,baz. If any l
-00003500: 6f67 6765 7220 6e61 6d65 2069 7320 7072  ogger name is pr
-00003510: 6566 6978 6564 2077 6974 6820 6120 6d69  efixed with a mi
-00003520: 6e75 732c 2065 670a 2020 2066 696c 7465  nus, eg.   filte
-00003530: 723d 2d66 6f6f 2c20 6974 2077 696c 6c20  r=-foo, it will 
-00003540: 6265 2065 7863 6c75 6465 6420 7261 7468  be excluded rath
-00003550: 6572 2074 6861 6e20 696e 636c 7564 6564  er than included
-00003560: 2e20 4465 6661 756c 743a 0a20 2020 6578  . Default:.   ex
-00003570: 636c 7564 6520 6c6f 6767 696e 6720 6d65  clude logging me
-00003580: 7373 6167 6573 2066 726f 6d20 6e6f 7365  ssages from nose
-00003590: 2069 7473 656c 6620 282d 6e6f 7365 292e   itself (-nose).
-000035a0: 205b 4e4f 5345 5f4c 4f47 4649 4c54 4552   [NOSE_LOGFILTER
-000035b0: 5d0a 0a2d 2d6c 6f67 6769 6e67 2d63 6c65  ]..--logging-cle
-000035c0: 6172 2d68 616e 646c 6572 730a 0a20 2020  ar-handlers..   
-000035d0: 436c 6561 7220 616c 6c20 6f74 6865 7220  Clear all other 
-000035e0: 6c6f 6767 696e 6720 6861 6e64 6c65 7273  logging handlers
-000035f0: 0a0a 2d2d 6c6f 6767 696e 672d 6c65 7665  ..--logging-leve
-00003600: 6c3d 4445 4641 554c 540a 0a20 2020 5365  l=DEFAULT..   Se
-00003610: 7420 7468 6520 6c6f 6720 6c65 7665 6c20  t the log level 
-00003620: 746f 2063 6170 7475 7265 0a0a 2d2d 7769  to capture..--wi
-00003630: 7468 2d63 6f76 6572 6167 650a 0a20 2020  th-coverage..   
-00003640: 456e 6162 6c65 2070 6c75 6769 6e20 436f  Enable plugin Co
-00003650: 7665 7261 6765 3a20 4163 7469 7661 7465  verage: Activate
-00003660: 2061 2063 6f76 6572 6167 6520 7265 706f   a coverage repo
-00003670: 7274 2075 7369 6e67 2074 6865 0a20 2020  rt using the.   
-00003680: 4e65 6420 4261 7463 6865 6c64 6572 2063  Ned Batchelder c
-00003690: 6f76 6572 6167 6520 6d6f 6475 6c65 2e20  overage module. 
-000036a0: 5b4e 4f53 455f 5749 5448 5f43 4f56 4552  [NOSE_WITH_COVER
-000036b0: 4147 455d 0a0a 2d2d 636f 7665 722d 7061  AGE]..--cover-pa
-000036c0: 636b 6167 653d 5041 434b 4147 450a 0a20  ckage=PACKAGE.. 
-000036d0: 2020 5265 7374 7269 6374 2063 6f76 6572    Restrict cover
-000036e0: 6167 6520 6f75 7470 7574 2074 6f20 7365  age output to se
-000036f0: 6c65 6374 6564 2070 6163 6b61 6765 7320  lected packages 
-00003700: 5b4e 4f53 455f 434f 5645 525f 5041 434b  [NOSE_COVER_PACK
-00003710: 4147 455d 0a0a 2d2d 636f 7665 722d 6572  AGE]..--cover-er
-00003720: 6173 650a 0a20 2020 4572 6173 6520 7072  ase..   Erase pr
-00003730: 6576 696f 7573 6c79 2063 6f6c 6c65 6374  eviously collect
-00003740: 6564 2063 6f76 6572 6167 6520 7374 6174  ed coverage stat
-00003750: 6973 7469 6373 2062 6566 6f72 6520 7275  istics before ru
-00003760: 6e0a 0a2d 2d63 6f76 6572 2d74 6573 7473  n..--cover-tests
-00003770: 0a0a 2020 2049 6e63 6c75 6465 2074 6573  ..   Include tes
-00003780: 7420 6d6f 6475 6c65 7320 696e 2063 6f76  t modules in cov
-00003790: 6572 6167 6520 7265 706f 7274 205b 4e4f  erage report [NO
-000037a0: 5345 5f43 4f56 4552 5f54 4553 5453 5d0a  SE_COVER_TESTS].
-000037b0: 0a2d 2d63 6f76 6572 2d6d 696e 2d70 6572  .--cover-min-per
-000037c0: 6365 6e74 6167 653d 4445 4641 554c 540a  centage=DEFAULT.
-000037d0: 0a20 2020 4d69 6e69 6d75 6d20 7065 7263  .   Minimum perc
-000037e0: 656e 7461 6765 206f 6620 636f 7665 7261  entage of covera
-000037f0: 6765 2066 6f72 2074 6573 7473 2074 6f20  ge for tests to 
-00003800: 7061 7373 0a20 2020 5b4e 4f53 455f 434f  pass.   [NOSE_CO
-00003810: 5645 525f 4d49 4e5f 5045 5243 454e 5441  VER_MIN_PERCENTA
-00003820: 4745 5d0a 0a2d 2d63 6f76 6572 2d69 6e63  GE]..--cover-inc
-00003830: 6c75 7369 7665 0a0a 2020 2049 6e63 6c75  lusive..   Inclu
-00003840: 6465 2061 6c6c 2070 7974 686f 6e20 6669  de all python fi
-00003850: 6c65 7320 756e 6465 7220 776f 726b 696e  les under workin
-00003860: 6720 6469 7265 6374 6f72 7920 696e 2063  g directory in c
-00003870: 6f76 6572 6167 650a 2020 2072 6570 6f72  overage.   repor
-00003880: 742e 2020 5573 6566 756c 2066 6f72 2064  t.  Useful for d
-00003890: 6973 636f 7665 7269 6e67 2068 6f6c 6573  iscovering holes
-000038a0: 2069 6e20 7465 7374 2063 6f76 6572 6167   in test coverag
-000038b0: 6520 6966 206e 6f74 2061 6c6c 0a20 2020  e if not all.   
-000038c0: 6669 6c65 7320 6172 6520 696d 706f 7274  files are import
-000038d0: 6564 2062 7920 7468 6520 7465 7374 2073  ed by the test s
-000038e0: 7569 7465 2e20 5b4e 4f53 455f 434f 5645  uite. [NOSE_COVE
-000038f0: 525f 494e 434c 5553 4956 455d 0a0a 2d2d  R_INCLUSIVE]..--
-00003900: 636f 7665 722d 6874 6d6c 0a0a 2020 2050  cover-html..   P
-00003910: 726f 6475 6365 2048 544d 4c20 636f 7665  roduce HTML cove
-00003920: 7261 6765 2069 6e66 6f72 6d61 7469 6f6e  rage information
-00003930: 0a0a 2d2d 636f 7665 722d 6874 6d6c 2d64  ..--cover-html-d
-00003940: 6972 3d44 4952 0a0a 2020 2050 726f 6475  ir=DIR..   Produ
-00003950: 6365 2048 544d 4c20 636f 7665 7261 6765  ce HTML coverage
-00003960: 2069 6e66 6f72 6d61 7469 6f6e 2069 6e20   information in 
-00003970: 6469 720a 0a2d 2d63 6f76 6572 2d62 7261  dir..--cover-bra
-00003980: 6e63 6865 730a 0a20 2020 496e 636c 7564  nches..   Includ
-00003990: 6520 6272 616e 6368 2063 6f76 6572 6167  e branch coverag
-000039a0: 6520 696e 2063 6f76 6572 6167 6520 7265  e in coverage re
-000039b0: 706f 7274 205b 4e4f 5345 5f43 4f56 4552  port [NOSE_COVER
-000039c0: 5f42 5241 4e43 4845 535d 0a0a 2d2d 636f  _BRANCHES]..--co
-000039d0: 7665 722d 786d 6c0a 0a20 2020 5072 6f64  ver-xml..   Prod
-000039e0: 7563 6520 584d 4c20 636f 7665 7261 6765  uce XML coverage
-000039f0: 2069 6e66 6f72 6d61 7469 6f6e 0a0a 2d2d   information..--
-00003a00: 636f 7665 722d 786d 6c2d 6669 6c65 3d46  cover-xml-file=F
-00003a10: 494c 450a 0a20 2020 5072 6f64 7563 6520  ILE..   Produce 
-00003a20: 584d 4c20 636f 7665 7261 6765 2069 6e66  XML coverage inf
-00003a30: 6f72 6d61 7469 6f6e 2069 6e20 6669 6c65  ormation in file
-00003a40: 0a0a 2d2d 7064 620a 0a20 2020 4472 6f70  ..--pdb..   Drop
-00003a50: 2069 6e74 6f20 6465 6275 6767 6572 206f   into debugger o
-00003a60: 6e20 6661 696c 7572 6573 206f 7220 6572  n failures or er
-00003a70: 726f 7273 0a0a 2d2d 7064 622d 6661 696c  rors..--pdb-fail
-00003a80: 7572 6573 0a0a 2020 2044 726f 7020 696e  ures..   Drop in
-00003a90: 746f 2064 6562 7567 6765 7220 6f6e 2066  to debugger on f
-00003aa0: 6169 6c75 7265 730a 0a2d 2d70 6462 2d65  ailures..--pdb-e
-00003ab0: 7272 6f72 730a 0a20 2020 4472 6f70 2069  rrors..   Drop i
-00003ac0: 6e74 6f20 6465 6275 6767 6572 206f 6e20  nto debugger on 
-00003ad0: 6572 726f 7273 0a0a 2d2d 6e6f 2d64 6570  errors..--no-dep
-00003ae0: 7265 6361 7465 640a 0a20 2020 4469 7361  recated..   Disa
-00003af0: 626c 6520 7370 6563 6961 6c20 6861 6e64  ble special hand
-00003b00: 6c69 6e67 206f 6620 4465 7072 6563 6174  ling of Deprecat
-00003b10: 6564 5465 7374 2065 7863 6570 7469 6f6e  edTest exception
-00003b20: 732e 0a0a 2d2d 7769 7468 2d64 6f63 7465  s...--with-docte
-00003b30: 7374 0a0a 2020 2045 6e61 626c 6520 706c  st..   Enable pl
-00003b40: 7567 696e 2044 6f63 7465 7374 3a20 4163  ugin Doctest: Ac
-00003b50: 7469 7661 7465 2064 6f63 7465 7374 2070  tivate doctest p
-00003b60: 6c75 6769 6e20 746f 2066 696e 6420 616e  lugin to find an
-00003b70: 6420 7275 6e0a 2020 2064 6f63 7465 7374  d run.   doctest
-00003b80: 7320 696e 206e 6f6e 2d74 6573 7420 6d6f  s in non-test mo
-00003b90: 6475 6c65 732e 205b 4e4f 5345 5f57 4954  dules. [NOSE_WIT
-00003ba0: 485f 444f 4354 4553 545d 0a0a 2d2d 646f  H_DOCTEST]..--do
-00003bb0: 6374 6573 742d 7465 7374 730a 0a20 2020  ctest-tests..   
-00003bc0: 416c 736f 206c 6f6f 6b20 666f 7220 646f  Also look for do
-00003bd0: 6374 6573 7473 2069 6e20 7465 7374 206d  ctests in test m
-00003be0: 6f64 756c 6573 2e20 4e6f 7465 2074 6861  odules. Note tha
-00003bf0: 7420 636c 6173 7365 732c 206d 6574 686f  t classes, metho
-00003c00: 6473 0a20 2020 616e 6420 6675 6e63 7469  ds.   and functi
-00003c10: 6f6e 7320 7368 6f75 6c64 2068 6176 6520  ons should have 
-00003c20: 6569 7468 6572 2064 6f63 7465 7374 7320  either doctests 
-00003c30: 6f72 206e 6f6e 2d64 6f63 7465 7374 2074  or non-doctest t
-00003c40: 6573 7473 2c20 6e6f 740a 2020 2062 6f74  ests, not.   bot
-00003c50: 682e 205b 4e4f 5345 5f44 4f43 5445 5354  h. [NOSE_DOCTEST
-00003c60: 5f54 4553 5453 5d0a 0a2d 2d64 6f63 7465  _TESTS]..--docte
-00003c70: 7374 2d65 7874 656e 7369 6f6e 3d45 5854  st-extension=EXT
-00003c80: 0a0a 2020 2041 6c73 6f20 6c6f 6f6b 2066  ..   Also look f
-00003c90: 6f72 2064 6f63 7465 7374 7320 696e 2066  or doctests in f
-00003ca0: 696c 6573 2077 6974 6820 7468 6973 2065  iles with this e
-00003cb0: 7874 656e 7369 6f6e 0a20 2020 5b4e 4f53  xtension.   [NOS
-00003cc0: 455f 444f 4354 4553 545f 4558 5445 4e53  E_DOCTEST_EXTENS
-00003cd0: 494f 4e5d 0a0a 2d2d 646f 6374 6573 742d  ION]..--doctest-
-00003ce0: 7265 7375 6c74 2d76 6172 6961 626c 653d  result-variable=
-00003cf0: 5641 520a 0a20 2020 4368 616e 6765 2074  VAR..   Change t
-00003d00: 6865 2076 6172 6961 626c 6520 6e61 6d65  he variable name
-00003d10: 2073 6574 2074 6f20 7468 6520 7265 7375   set to the resu
-00003d20: 6c74 206f 6620 7468 6520 6c61 7374 2069  lt of the last i
-00003d30: 6e74 6572 7072 6574 6572 0a20 2020 636f  nterpreter.   co
-00003d40: 6d6d 616e 6420 6672 6f6d 2074 6865 2064  mmand from the d
-00003d50: 6566 6175 6c74 2027 5f27 2e20 4361 6e20  efault '_'. Can 
-00003d60: 6265 2075 7365 6420 746f 2061 766f 6964  be used to avoid
-00003d70: 2063 6f6e 666c 6963 7473 2077 6974 680a   conflicts with.
-00003d80: 2020 2074 6865 205f 2829 2066 756e 6374     the _() funct
-00003d90: 696f 6e20 7573 6564 2066 6f72 2074 6578  ion used for tex
-00003da0: 7420 7472 616e 736c 6174 696f 6e2e 0a20  t translation.. 
-00003db0: 2020 5b4e 4f53 455f 444f 4354 4553 545f    [NOSE_DOCTEST_
-00003dc0: 5245 5355 4c54 5f56 4152 5d0a 0a2d 2d64  RESULT_VAR]..--d
-00003dd0: 6f63 7465 7374 2d66 6978 7475 7265 733d  octest-fixtures=
-00003de0: 5355 4646 4958 0a0a 2020 2046 696e 6420  SUFFIX..   Find 
-00003df0: 6669 7874 7572 6573 2066 6f72 2061 2064  fixtures for a d
-00003e00: 6f63 7465 7374 2066 696c 6520 696e 206d  octest file in m
-00003e10: 6f64 756c 6520 7769 7468 2074 6869 7320  odule with this 
-00003e20: 6e61 6d65 2061 7070 656e 6465 640a 2020  name appended.  
-00003e30: 2074 6f20 7468 6520 6261 7365 206e 616d   to the base nam
-00003e40: 6520 6f66 2074 6865 2064 6f63 7465 7374  e of the doctest
-00003e50: 2066 696c 650a 0a2d 2d64 6f63 7465 7374   file..--doctest
-00003e60: 2d6f 7074 696f 6e73 3d4f 5054 494f 4e53  -options=OPTIONS
-00003e70: 0a0a 2020 2053 7065 6369 6679 206f 7074  ..   Specify opt
-00003e80: 696f 6e73 2074 6f20 7061 7373 2074 6f20  ions to pass to 
-00003e90: 646f 6374 6573 742e 2045 672e 0a20 2020  doctest. Eg..   
-00003ea0: 272b 454c 4c49 5053 4953 2c2b 4e4f 524d  '+ELLIPSIS,+NORM
-00003eb0: 414c 495a 455f 5748 4954 4553 5041 4345  ALIZE_WHITESPACE
-00003ec0: 270a 0a2d 2d77 6974 682d 6973 6f6c 6174  '..--with-isolat
-00003ed0: 696f 6e0a 0a20 2020 456e 6162 6c65 2070  ion..   Enable p
-00003ee0: 6c75 6769 6e20 4973 6f6c 6174 696f 6e50  lugin IsolationP
-00003ef0: 6c75 6769 6e3a 2041 6374 6976 6174 6520  lugin: Activate 
-00003f00: 7468 6520 6973 6f6c 6174 696f 6e20 706c  the isolation pl
-00003f10: 7567 696e 2074 6f0a 2020 2069 736f 6c61  ugin to.   isola
-00003f20: 7465 2063 6861 6e67 6573 2074 6f20 6578  te changes to ex
-00003f30: 7465 726e 616c 206d 6f64 756c 6573 2074  ternal modules t
-00003f40: 6f20 6120 7369 6e67 6c65 2074 6573 7420  o a single test 
-00003f50: 6d6f 6475 6c65 206f 720a 2020 2070 6163  module or.   pac
-00003f60: 6b61 6765 2e20 5468 6520 6973 6f6c 6174  kage. The isolat
-00003f70: 696f 6e20 706c 7567 696e 2072 6573 6574  ion plugin reset
-00003f80: 7320 7468 6520 636f 6e74 656e 7473 206f  s the contents o
-00003f90: 6620 7379 732e 6d6f 6475 6c65 730a 2020  f sys.modules.  
-00003fa0: 2061 6674 6572 2065 6163 6820 7465 7374   after each test
-00003fb0: 206d 6f64 756c 6520 6f72 2070 6163 6b61   module or packa
-00003fc0: 6765 2072 756e 7320 746f 2069 7473 2073  ge runs to its s
-00003fd0: 7461 7465 2062 6566 6f72 6520 7468 650a  tate before the.
-00003fe0: 2020 2074 6573 742e 2050 4c45 4153 4520     test. PLEASE 
-00003ff0: 4e4f 5445 2074 6861 7420 7468 6973 2070  NOTE that this p
-00004000: 6c75 6769 6e20 7368 6f75 6c64 206e 6f74  lugin should not
-00004010: 2062 6520 7573 6564 2077 6974 6820 7468   be used with th
-00004020: 650a 2020 2063 6f76 6572 6167 6520 706c  e.   coverage pl
-00004030: 7567 696e 2c20 6f72 2069 6e20 616e 7920  ugin, or in any 
-00004040: 6f74 6865 7220 6361 7365 2077 6865 7265  other case where
-00004050: 206d 6f64 756c 6520 7265 6c6f 6164 696e   module reloadin
-00004060: 6720 6d61 790a 2020 2070 726f 6475 6365  g may.   produce
-00004070: 2075 6e64 6573 6972 6162 6c65 2073 6964   undesirable sid
-00004080: 652d 6566 6665 6374 732e 205b 4e4f 5345  e-effects. [NOSE
-00004090: 5f57 4954 485f 4953 4f4c 4154 494f 4e5d  _WITH_ISOLATION]
-000040a0: 0a0a 2d64 2c20 2d2d 6465 7461 696c 6564  ..-d, --detailed
-000040b0: 2d65 7272 6f72 732c 202d 2d66 6169 6c75  -errors, --failu
-000040c0: 7265 2d64 6574 6169 6c0a 0a20 2020 4164  re-detail..   Ad
-000040d0: 6420 6465 7461 696c 2074 6f20 6572 726f  d detail to erro
-000040e0: 7220 6f75 7470 7574 2062 7920 6174 7465  r output by atte
-000040f0: 6d70 7469 6e67 2074 6f20 6576 616c 7561  mpting to evalua
-00004100: 7465 2066 6169 6c65 6420 6173 7365 7274  te failed assert
-00004110: 730a 2020 205b 4e4f 5345 5f44 4554 4149  s.   [NOSE_DETAI
-00004120: 4c45 445f 4552 524f 5253 5d0a 0a2d 2d6e  LED_ERRORS]..--n
-00004130: 6f2d 736b 6970 0a0a 2020 2044 6973 6162  o-skip..   Disab
-00004140: 6c65 2073 7065 6369 616c 2068 616e 646c  le special handl
-00004150: 696e 6720 6f66 2053 6b69 7054 6573 7420  ing of SkipTest 
-00004160: 6578 6365 7074 696f 6e73 2e0a 0a2d 2d77  exceptions...--w
-00004170: 6974 682d 6964 0a0a 2020 2045 6e61 626c  ith-id..   Enabl
-00004180: 6520 706c 7567 696e 2054 6573 7449 643a  e plugin TestId:
-00004190: 2041 6374 6976 6174 6520 746f 2061 6464   Activate to add
-000041a0: 2061 2074 6573 7420 6964 2028 6c69 6b65   a test id (like
-000041b0: 2023 3129 2074 6f20 6561 6368 0a20 2020   #1) to each.   
-000041c0: 7465 7374 206e 616d 6520 6f75 7470 7574  test name output
-000041d0: 2e20 4163 7469 7661 7465 2077 6974 6820  . Activate with 
-000041e0: 2d2d 6661 696c 6564 2074 6f20 7265 7275  --failed to reru
-000041f0: 6e20 6661 696c 696e 6720 7465 7374 730a  n failing tests.
-00004200: 2020 206f 6e6c 792e 205b 4e4f 5345 5f57     only. [NOSE_W
-00004210: 4954 485f 4944 5d0a 0a2d 2d69 642d 6669  ITH_ID]..--id-fi
-00004220: 6c65 3d46 494c 450a 0a20 2020 5374 6f72  le=FILE..   Stor
-00004230: 6520 7465 7374 2069 6473 2066 6f75 6e64  e test ids found
-00004240: 2069 6e20 7465 7374 2072 756e 7320 696e   in test runs in
-00004250: 2074 6869 7320 6669 6c65 2e20 4465 6661   this file. Defa
-00004260: 756c 7420 6973 2074 6865 2066 696c 650a  ult is the file.
-00004270: 2020 202e 6e6f 7365 6964 7320 696e 2074     .noseids in t
-00004280: 6865 2077 6f72 6b69 6e67 2064 6972 6563  he working direc
-00004290: 746f 7279 2e0a 0a2d 2d66 6169 6c65 640a  tory...--failed.
-000042a0: 0a20 2020 5275 6e20 7468 6520 7465 7374  .   Run the test
-000042b0: 7320 7468 6174 2066 6169 6c65 6420 696e  s that failed in
-000042c0: 2074 6865 206c 6173 7420 7465 7374 2072   the last test r
-000042d0: 756e 2e0a 0a2d 2d70 726f 6365 7373 6573  un...--processes
-000042e0: 3d4e 554d 0a0a 2020 2053 7072 6561 6420  =NUM..   Spread 
-000042f0: 7465 7374 2072 756e 2061 6d6f 6e67 2074  test run among t
-00004300: 6869 7320 6d61 6e79 2070 726f 6365 7373  his many process
-00004310: 6573 2e20 5365 7420 6120 6e75 6d62 6572  es. Set a number
-00004320: 2065 7175 616c 2074 6f0a 2020 2074 6865   equal to.   the
-00004330: 206e 756d 6265 7220 6f66 2070 726f 6365   number of proce
-00004340: 7373 6f72 7320 6f72 2063 6f72 6573 2069  ssors or cores i
-00004350: 6e20 796f 7572 206d 6163 6869 6e65 2066  n your machine f
-00004360: 6f72 2062 6573 7420 7265 7375 6c74 732e  or best results.
-00004370: 0a20 2020 5061 7373 2061 206e 6567 6174  .   Pass a negat
-00004380: 6976 6520 6e75 6d62 6572 2074 6f20 6861  ive number to ha
-00004390: 7665 2074 6865 206e 756d 6265 7220 6f66  ve the number of
-000043a0: 2070 726f 6365 7373 6573 0a20 2020 6175   processes.   au
-000043b0: 746f 6d61 7469 6361 6c6c 7920 7365 7420  tomatically set 
-000043c0: 746f 2074 6865 206e 756d 6265 7220 6f66  to the number of
-000043d0: 2063 6f72 6573 2e20 5061 7373 696e 6720   cores. Passing 
-000043e0: 3020 6d65 616e 7320 746f 0a20 2020 6469  0 means to.   di
-000043f0: 7361 626c 6520 7061 7261 6c6c 656c 2074  sable parallel t
-00004400: 6573 7469 6e67 2e20 4465 6661 756c 7420  esting. Default 
-00004410: 6973 2030 2075 6e6c 6573 7320 4e4f 5345  is 0 unless NOSE
-00004420: 5f50 524f 4345 5353 4553 2069 730a 2020  _PROCESSES is.  
-00004430: 2073 6574 2e20 5b4e 4f53 455f 5052 4f43   set. [NOSE_PROC
-00004440: 4553 5345 535d 0a0a 2d2d 7072 6f63 6573  ESSES]..--proces
-00004450: 732d 7469 6d65 6f75 743d 5345 434f 4e44  s-timeout=SECOND
-00004460: 530a 0a20 2020 5365 7420 7469 6d65 6f75  S..   Set timeou
-00004470: 7420 666f 7220 7265 7475 726e 206f 6620  t for return of 
-00004480: 7265 7375 6c74 7320 6672 6f6d 2065 6163  results from eac
-00004490: 6820 7465 7374 2072 756e 6e65 7220 7072  h test runner pr
-000044a0: 6f63 6573 732e 0a20 2020 4465 6661 756c  ocess..   Defaul
-000044b0: 7420 6973 2031 302e 205b 4e4f 5345 5f50  t is 10. [NOSE_P
-000044c0: 524f 4345 5353 5f54 494d 454f 5554 5d0a  ROCESS_TIMEOUT].
-000044d0: 0a2d 2d70 726f 6365 7373 2d72 6573 7461  .--process-resta
-000044e0: 7274 776f 726b 6572 0a0a 2020 2049 6620  rtworker..   If 
-000044f0: 7365 742c 2077 696c 6c20 7265 7374 6172  set, will restar
-00004500: 7420 6561 6368 2077 6f72 6b65 7220 7072  t each worker pr
-00004510: 6f63 6573 7320 6f6e 6365 2074 6865 6972  ocess once their
-00004520: 2074 6573 7473 2061 7265 2064 6f6e 652c   tests are done,
-00004530: 0a20 2020 7468 6973 2068 656c 7073 2063  .   this helps c
-00004540: 6f6e 7472 6f6c 206d 656d 6f72 7920 6c65  ontrol memory le
-00004550: 616b 7320 6672 6f6d 206b 696c 6c69 6e67  aks from killing
-00004560: 2074 6865 2073 7973 7465 6d2e 0a20 2020   the system..   
-00004570: 5b4e 4f53 455f 5052 4f43 4553 535f 5245  [NOSE_PROCESS_RE
-00004580: 5354 4152 5457 4f52 4b45 525d 0a0a 2d2d  STARTWORKER]..--
-00004590: 7769 7468 2d78 756e 6974 0a0a 2020 2045  with-xunit..   E
-000045a0: 6e61 626c 6520 706c 7567 696e 2058 756e  nable plugin Xun
-000045b0: 6974 3a20 5468 6973 2070 6c75 6769 6e20  it: This plugin 
-000045c0: 7072 6f76 6964 6573 2074 6573 7420 7265  provides test re
-000045d0: 7375 6c74 7320 696e 2074 6865 0a20 2020  sults in the.   
-000045e0: 7374 616e 6461 7264 2058 556e 6974 2058  standard XUnit X
-000045f0: 4d4c 2066 6f72 6d61 742e 205b 4e4f 5345  ML format. [NOSE
-00004600: 5f57 4954 485f 5855 4e49 545d 0a0a 2d2d  _WITH_XUNIT]..--
-00004610: 7875 6e69 742d 6669 6c65 3d46 494c 450a  xunit-file=FILE.
-00004620: 0a20 2020 5061 7468 2074 6f20 786d 6c20  .   Path to xml 
-00004630: 6669 6c65 2074 6f20 7374 6f72 6520 7468  file to store th
-00004640: 6520 7875 6e69 7420 7265 706f 7274 2069  e xunit report i
-00004650: 6e2e 2044 6566 6175 6c74 2069 730a 2020  n. Default is.  
-00004660: 206e 6f73 6574 6573 7473 2e78 6d6c 2069   nosetests.xml i
-00004670: 6e20 7468 6520 776f 726b 696e 6720 6469  n the working di
-00004680: 7265 6374 6f72 7920 5b4e 4f53 455f 5855  rectory [NOSE_XU
-00004690: 4e49 545f 4649 4c45 5d0a 0a2d 2d78 756e  NIT_FILE]..--xun
-000046a0: 6974 2d74 6573 7473 7569 7465 2d6e 616d  it-testsuite-nam
-000046b0: 653d 5041 434b 4147 450a 0a20 2020 4e61  e=PACKAGE..   Na
-000046c0: 6d65 206f 6620 7468 6520 7465 7374 7375  me of the testsu
-000046d0: 6974 6520 696e 2074 6865 2078 756e 6974  ite in the xunit
-000046e0: 2078 6d6c 2c20 6765 6e65 7261 7465 6420   xml, generated 
-000046f0: 6279 2070 6c75 6769 6e2e 0a20 2020 4465  by plugin..   De
-00004700: 6661 756c 7420 7465 7374 2073 7569 7465  fault test suite
-00004710: 206e 616d 6520 6973 206e 6f73 6574 6573   name is nosetes
-00004720: 7473 2e0a 0a2d 2d61 6c6c 2d6d 6f64 756c  ts...--all-modul
-00004730: 6573 0a0a 2020 2045 6e61 626c 6520 706c  es..   Enable pl
-00004740: 7567 696e 2041 6c6c 4d6f 6475 6c65 733a  ugin AllModules:
-00004750: 2043 6f6c 6c65 6374 2074 6573 7473 2066   Collect tests f
-00004760: 726f 6d20 616c 6c20 7079 7468 6f6e 206d  rom all python m
-00004770: 6f64 756c 6573 2e0a 2020 205b 4e4f 5345  odules..   [NOSE
-00004780: 5f41 4c4c 5f4d 4f44 554c 4553 5d0a 0a2d  _ALL_MODULES]..-
-00004790: 2d63 6f2c 202d 2d63 6f6c 6c65 6374 2d6f  -co, --collect-o
-000047a0: 6e6c 790a 0a20 2020 456e 6162 6c65 2063  nly..   Enable c
-000047b0: 6f6c 6c65 6374 2d6f 6e6c 793a 2043 6f6c  ollect-only: Col
-000047c0: 6c65 6374 2061 6e64 206f 7574 7075 7420  lect and output 
-000047d0: 7465 7374 206e 616d 6573 206f 6e6c 792c  test names only,
-000047e0: 0a20 2020 6275 7420 646f 206e 6f74 2072  .   but do not r
-000047f0: 756e 2061 6e79 2074 6573 7473 2e20 5b43  un any tests. [C
-00004800: 4f4c 4c45 4354 5f4f 4e4c 595d 0a60 6060  OLLECT_ONLY].```
-00004810: 0a                                       .
+000005b0: 0a3c 6831 3e70 796e 6f73 6520 f09f 908d  .<h1>pynose ....
+000005c0: f09f 9183 203c 6120 6872 6566 3d22 6874  .... <a href="ht
+000005d0: 7470 733a 2f2f 7079 7069 2e70 7974 686f  tps://pypi.pytho
+000005e0: 6e2e 6f72 672f 7079 7069 2f70 796e 6f73  n.org/pypi/pynos
+000005f0: 6522 2074 6172 6765 743d 225f 626c 616e  e" target="_blan
+00000600: 6b22 3e3c 696d 6720 7372 633d 2268 7474  k"><img src="htt
+00000610: 7073 3a2f 2f69 6d67 2e73 6869 656c 6473  ps://img.shields
+00000620: 2e69 6f2f 7079 7069 2f76 2f70 796e 6f73  .io/pypi/v/pynos
+00000630: 652e 7376 673f 636f 6c6f 723d 3333 3939  e.svg?color=3399
+00000640: 4545 2220 616c 743d 2250 7950 4920 7665  EE" alt="PyPI ve
+00000650: 7273 696f 6e22 202f 3e3c 2f61 3e3c 2f68  rsion" /></a></h
+00000660: 313e 0a0a 2323 2320 2a2a 5b70 796e 6f73  1>..### **[pynos
+00000670: 655d 2868 7474 7073 3a2f 2f67 6974 6875  e](https://githu
+00000680: 622e 636f 6d2f 6d64 6d69 6e74 7a2f 7079  b.com/mdmintz/py
+00000690: 6e6f 7365 292a 2a20 6669 7865 7320 2a2a  nose)** fixes **
+000006a0: 5b6e 6f73 655d 2868 7474 7073 3a2f 2f6e  [nose](https://n
+000006b0: 6f73 652e 7265 6164 7468 6564 6f63 732e  ose.readthedocs.
+000006c0: 696f 2f65 6e2f 6c61 7465 7374 2f29 2a2a  io/en/latest/)**
+000006d0: 2074 6f20 6578 7465 6e64 205b 756e 6974   to extend [unit
+000006e0: 7465 7374 5d28 6874 7470 733a 2f2f 646f  test](https://do
+000006f0: 6373 2e70 7974 686f 6e2e 6f72 672f 332f  cs.python.org/3/
+00000700: 6c69 6272 6172 792f 756e 6974 7465 7374  library/unittest
+00000710: 2e68 746d 6c29 2061 6e64 206d 616b 6520  .html) and make 
+00000720: 7465 7374 696e 6720 6561 7369 6572 2e0a  testing easier..
+00000730: 0a2d 2d2d 2d2d 2d2d 2d0a 0a60 6070 796e  .--------..``pyn
+00000740: 6f73 6560 6020 6973 2061 6e20 7570 6461  ose`` is an upda
+00000750: 7465 6420 7665 7273 696f 6e20 6f66 2060  ted version of `
+00000760: 606e 6f73 6560 602c 206f 7269 6769 6e61  `nose``, origina
+00000770: 6c6c 7920 6d61 6465 2062 7920 4a61 736f  lly made by Jaso
+00000780: 6e20 5065 6c6c 6572 696e 2e0a 0a54 6869  n Pellerin...Thi
+00000790: 7320 7665 7273 696f 6e20 6f66 2060 606e  s version of ``n
+000007a0: 6f73 6560 6020 6973 2063 6f6d 7061 7469  ose`` is compati
+000007b0: 626c 6520 7769 7468 2060 6050 7974 686f  ble with ``Pytho
+000007c0: 6e20 332e 362b 6060 2028 696e 636c 7564  n 3.6+`` (includ
+000007d0: 696e 6720 6060 332e 3132 2b60 6029 2e0a  ing ``3.12+``)..
+000007e0: 0a43 6861 6e67 6573 2069 6e20 6060 7079  .Changes in ``py
+000007f0: 6e6f 7365 6060 2066 726f 6d20 6c65 6761  nose`` from lega
+00000800: 6379 2060 606e 6f73 6560 6020 696e 636c  cy ``nose`` incl
+00000810: 7564 653a 0a2a 2046 6978 6573 2022 4174  ude:.* Fixes "At
+00000820: 7472 6962 7574 6545 7272 6f72 3a20 6d6f  tributeError: mo
+00000830: 6475 6c65 2027 636f 6c6c 6563 7469 6f6e  dule 'collection
+00000840: 7327 2068 6173 206e 6f20 6174 7472 6962  s' has no attrib
+00000850: 7574 6520 2743 616c 6c61 626c 6527 2e22  ute 'Callable'."
+00000860: 0a2a 2046 6978 6573 2022 4174 7472 6962  .* Fixes "Attrib
+00000870: 7574 6545 7272 6f72 3a20 6d6f 6475 6c65  uteError: module
+00000880: 2027 696e 7370 6563 7427 2068 6173 206e   'inspect' has n
+00000890: 6f20 6174 7472 6962 7574 6520 2767 6574  o attribute 'get
+000008a0: 6172 6773 7065 6327 2e22 0a2a 2046 6978  argspec'.".* Fix
+000008b0: 6573 2022 496d 706f 7274 4572 726f 723a  es "ImportError:
+000008c0: 2063 616e 6e6f 7420 696d 706f 7274 206e   cannot import n
+000008d0: 616d 6520 275f 5465 7874 5465 7374 5265  ame '_TextTestRe
+000008e0: 7375 6c74 2720 6672 6f6d 2027 756e 6974  sult' from 'unit
+000008f0: 7465 7374 272e 220a 2a20 4669 7865 7320  test'.".* Fixes 
+00000900: 2252 756e 7469 6d65 5761 726e 696e 673a  "RuntimeWarning:
+00000910: 2054 6573 7452 6573 756c 7420 6861 7320   TestResult has 
+00000920: 6e6f 2061 6464 4475 7261 7469 6f6e 206d  no addDuration m
+00000930: 6574 686f 642e 220a 2a20 4669 7865 7320  ethod.".* Fixes 
+00000940: 2244 6570 7265 6361 7469 6f6e 5761 726e  "DeprecationWarn
+00000950: 696e 673a 2070 6b67 5f72 6573 6f75 7263  ing: pkg_resourc
+00000960: 6573 2069 7320 6465 7072 6563 6174 6564  es is deprecated
+00000970: 2061 7320 616e 2041 5049 2e22 0a2a 2046   as an API.".* F
+00000980: 6978 6573 2061 6c6c 2060 6066 6c61 6b65  ixes all ``flake
+00000990: 3860 6020 6973 7375 6573 2066 726f 6d20  8`` issues from 
+000009a0: 7468 6520 6f72 6967 696e 616c 2060 606e  the original ``n
+000009b0: 6f73 6560 602e 0a2a 2052 6570 6c61 6365  ose``..* Replace
+000009c0: 7320 7468 6520 6060 696d 7060 6020 6d6f  s the ``imp`` mo
+000009d0: 6475 6c65 2077 6974 6820 7468 6520 6e65  dule with the ne
+000009e0: 7765 7220 6060 696d 706f 7274 6c69 6260  wer ``importlib`
+000009f0: 6020 6d6f 6475 6c65 2e0a 2a20 5468 6520  ` module..* The 
+00000a00: 6465 6661 756c 7420 6c6f 6767 696e 6720  default logging 
+00000a10: 6c65 7665 6c20 6e6f 7720 6869 6465 7320  level now hides 
+00000a20: 2264 6562 7567 2220 6c6f 6773 2066 6f72  "debug" logs for
+00000a30: 206c 6573 7320 6e6f 6973 652e 0a2a 2054   less noise..* T
+00000a40: 6865 2060 602d 7360 6020 6f70 7469 6f6e  he ``-s`` option
+00000a50: 2069 7320 616c 7761 7973 2061 6374 6976   is always activ
+00000a60: 6520 746f 2073 6565 2074 6865 206f 7574  e to see the out
+00000a70: 7075 7420 6f66 2060 6070 7269 6e74 2829  put of ``print()
+00000a80: 6060 2e0a 2a20 4164 6473 2060 602d 2d63  ``..* Adds ``--c
+00000a90: 6f60 6020 6173 2061 2073 686f 7274 6375  o`` as a shortcu
+00000aa0: 7420 746f 2075 7369 6e67 2060 602d 2d63  t to using ``--c
+00000ab0: 6f6c 6c65 6374 2d6f 6e6c 7960 602e 0a0a  ollect-only``...
+00000ac0: 2d2d 2d2d 2d2d 2d2d 0a0a 5468 6520 6f72  --------..The or
+00000ad0: 6967 696e 616c 2064 6573 6372 6970 7469  iginal descripti
+00000ae0: 6f6e 206f 6620 6060 6e6f 7365 6060 3a0a  on of ``nose``:.
+00000af0: 0a3e 6e6f 7365 2065 7874 656e 6473 2074  .>nose extends t
+00000b00: 6865 2074 6573 7420 6c6f 6164 696e 6720  he test loading 
+00000b10: 616e 6420 7275 6e6e 696e 6720 6665 6174  and running feat
+00000b20: 7572 6573 206f 6620 756e 6974 7465 7374  ures of unittest
+00000b30: 2c20 6d61 6b69 6e67 0a69 7420 6561 7369  , making.it easi
+00000b40: 6572 2074 6f20 7772 6974 652c 2066 696e  er to write, fin
+00000b50: 6420 616e 6420 7275 6e20 7465 7374 732e  d and run tests.
+00000b60: 0a0a 3e42 7920 6465 6661 756c 742c 206e  ..>By default, n
+00000b70: 6f73 6520 7275 6e73 2074 6573 7473 2069  ose runs tests i
+00000b80: 6e20 6669 6c65 7320 6f72 2064 6972 6563  n files or direc
+00000b90: 746f 7269 6573 2075 6e64 6572 2074 6865  tories under the
+00000ba0: 2063 7572 7265 6e74 0a77 6f72 6b69 6e67   current.working
+00000bb0: 2064 6972 6563 746f 7279 2077 686f 7365   directory whose
+00000bc0: 206e 616d 6573 2069 6e63 6c75 6465 2022   names include "
+00000bd0: 7465 7374 2220 6f72 2022 5465 7374 2220  test" or "Test" 
+00000be0: 6174 2061 2077 6f72 640a 626f 756e 6461  at a word.bounda
+00000bf0: 7279 2028 6c69 6b65 2022 7465 7374 5f74  ry (like "test_t
+00000c00: 6869 7322 206f 7220 2266 756e 6374 696f  his" or "functio
+00000c10: 6e61 6c5f 7465 7374 2220 6f72 2022 5465  nal_test" or "Te
+00000c20: 7374 436c 6173 7322 2062 7574 206e 6f74  stClass" but not
+00000c30: 0a22 6c69 6274 6573 7422 292e 2054 6573  ."libtest"). Tes
+00000c40: 7420 6f75 7470 7574 2069 7320 7369 6d69  t output is simi
+00000c50: 6c61 7220 746f 2074 6861 7420 6f66 2075  lar to that of u
+00000c60: 6e69 7474 6573 742c 2062 7574 2061 6c73  nittest, but als
+00000c70: 6f20 696e 636c 7564 6573 0a63 6170 7475  o includes.captu
+00000c80: 7265 6420 7374 646f 7574 206f 7574 7075  red stdout outpu
+00000c90: 7420 6672 6f6d 2066 6169 6c69 6e67 2074  t from failing t
+00000ca0: 6573 7473 2c20 666f 7220 6561 7379 2070  ests, for easy p
+00000cb0: 7269 6e74 2d73 7479 6c65 2064 6562 7567  rint-style debug
+00000cc0: 6769 6e67 2e0a 0a3e 5468 6573 6520 6665  ging...>These fe
+00000cd0: 6174 7572 6573 2c20 616e 6420 6d61 6e79  atures, and many
+00000ce0: 206d 6f72 652c 2061 7265 2063 7573 746f   more, are custo
+00000cf0: 6d69 7a61 626c 6520 7468 726f 7567 6820  mizable through 
+00000d00: 7468 6520 7573 6520 6f66 0a70 6c75 6769  the use of.plugi
+00000d10: 6e73 2e20 506c 7567 696e 7320 696e 636c  ns. Plugins incl
+00000d20: 7564 6564 2077 6974 6820 6e6f 7365 2070  uded with nose p
+00000d30: 726f 7669 6465 2073 7570 706f 7274 2066  rovide support f
+00000d40: 6f72 2064 6f63 7465 7374 2c20 636f 6465  or doctest, code
+00000d50: 0a63 6f76 6572 6167 6520 616e 6420 7072  .coverage and pr
+00000d60: 6f66 696c 696e 672c 2066 6c65 7869 626c  ofiling, flexibl
+00000d70: 6520 6174 7472 6962 7574 652d 6261 7365  e attribute-base
+00000d80: 6420 7465 7374 2073 656c 6563 7469 6f6e  d test selection
+00000d90: 2c0a 6f75 7470 7574 2063 6170 7475 7265  ,.output capture
+00000da0: 2061 6e64 206d 6f72 652e 204d 6f72 6520   and more. More 
+00000db0: 696e 666f 726d 6174 696f 6e20 6162 6f75  information abou
+00000dc0: 7420 7772 6974 696e 6720 706c 7567 696e  t writing plugin
+00000dd0: 730a 6d61 7920 6265 2066 6f75 6e64 206f  s.may be found o
+00000de0: 6e20 696e 2074 6865 206e 6f73 6520 4150  n in the nose AP
+00000df0: 4920 646f 6375 6d65 6e74 6174 696f 6e2c  I documentation,
+00000e00: 2068 6572 653a 0a68 7474 7073 3a2f 2f6e   here:.https://n
+00000e10: 6f73 652e 7265 6164 7468 6564 6f63 732e  ose.readthedocs.
+00000e20: 696f 2f65 6e2f 6c61 7465 7374 2f0a 0a2d  io/en/latest/..-
+00000e30: 2d2d 2d2d 2d2d 2d0a 0a60 6060 6261 7368  -------..```bash
+00000e40: 0a0a 4261 7369 6320 7573 6167 650a 2a2a  ..Basic usage.**
+00000e50: 2a2a 2a2a 2a2a 2a2a 2a0a 0a55 7365 2022  *********..Use "
+00000e60: 7079 6e6f 7365 2220 4f52 2022 6e6f 7365  pynose" OR "nose
+00000e70: 7465 7374 7322 2074 6f20 7275 6e20 7465  tests" to run te
+00000e80: 7374 733a 0a0a 2020 2020 7079 6e6f 7365  sts:..    pynose
+00000e90: 205b 6f70 7469 6f6e 735d 205b 286f 7074   [options] [(opt
+00000ea0: 696f 6e61 6c29 2074 6573 7420 6669 6c65  ional) test file
+00000eb0: 7320 6f72 2064 6972 6563 746f 7269 6573  s or directories
+00000ec0: 5d0a 0a20 2020 206e 6f73 6574 6573 7473  ]..    nosetests
+00000ed0: 205b 6f70 7469 6f6e 735d 205b 286f 7074   [options] [(opt
+00000ee0: 696f 6e61 6c29 2074 6573 7420 6669 6c65  ional) test file
+00000ef0: 7320 6f72 2064 6972 6563 746f 7269 6573  s or directories
+00000f00: 5d0a 0a49 6e20 6164 6469 7469 6f6e 2074  ]..In addition t
+00000f10: 6f20 7061 7373 696e 6720 636f 6d6d 616e  o passing comman
+00000f20: 642d 6c69 6e65 206f 7074 696f 6e73 2c20  d-line options, 
+00000f30: 796f 7520 6d61 7920 616c 736f 2070 7574  you may also put
+00000f40: 0a63 6f6e 6669 6775 7261 7469 6f6e 206f  .configuration o
+00000f50: 7074 696f 6e73 2069 6e20 6120 2e6e 6f73  ptions in a .nos
+00000f60: 6572 6320 6f72 206e 6f73 652e 6366 6720  erc or nose.cfg 
+00000f70: 6669 6c65 2069 6e20 796f 7572 2068 6f6d  file in your hom
+00000f80: 650a 6469 7265 6374 6f72 792e 2054 6865  e.directory. The
+00000f90: 7365 2061 7265 2073 7461 6e64 6172 6420  se are standard 
+00000fa0: 2e69 6e69 2d73 7479 6c65 2063 6f6e 6669  .ini-style confi
+00000fb0: 6720 6669 6c65 732e 2050 7574 2079 6f75  g files. Put you
+00000fc0: 720a 6e6f 7365 7465 7374 7320 636f 6e66  r.nosetests conf
+00000fd0: 6967 7572 6174 696f 6e20 696e 2061 205b  iguration in a [
+00000fe0: 6e6f 7365 7465 7374 735d 2073 6563 7469  nosetests] secti
+00000ff0: 6f6e 2c20 7769 7468 2074 6865 202d 2d20  on, with the -- 
+00001000: 7072 6566 6978 0a72 656d 6f76 6564 3a0a  prefix.removed:.
+00001010: 0a20 2020 5b6e 6f73 6574 6573 7473 5d0a  .   [nosetests].
+00001020: 2020 2076 6572 626f 7369 7479 3d33 0a20     verbosity=3. 
+00001030: 2020 7769 7468 2d64 6f63 7465 7374 3d31    with-doctest=1
+00001040: 0a0a 5468 6572 6520 6973 2061 6c73 6f20  ..There is also 
+00001050: 706f 7373 6962 6c69 7479 2074 6f20 6469  possiblity to di
+00001060: 7361 626c 6520 636f 6e66 6967 7572 6174  sable configurat
+00001070: 696f 6e20 6669 6c65 7320 6c6f 6164 696e  ion files loadin
+00001080: 6720 286d 6967 6874 0a62 6520 7573 6566  g (might.be usef
+00001090: 756c 2077 6865 6e20 7275 6e6e 6967 2069  ul when runnig i
+000010a0: 2e65 2e20 746f 7820 616e 6420 796f 7520  .e. tox and you 
+000010b0: 646f 206e 6f74 2077 616e 7420 796f 7572  do not want your
+000010c0: 2067 6c6f 6261 6c20 6e6f 7365 0a63 6f6e   global nose.con
+000010d0: 6669 6720 6669 6c65 2074 6f20 6265 2075  fig file to be u
+000010e0: 7365 6420 6279 2074 6f78 292e 2049 6e20  sed by tox). In 
+000010f0: 6f72 6465 7220 746f 2069 676e 6f72 6520  order to ignore 
+00001100: 7468 6f73 6520 636f 6e66 6967 7572 6174  those configurat
+00001110: 696f 6e0a 6669 6c65 7320 7369 6d70 6c79  ion.files simply
+00001120: 2073 6574 2061 6e20 656e 7669 726f 6e6d   set an environm
+00001130: 656e 7420 7661 7269 6162 6c65 2022 4e4f  ent variable "NO
+00001140: 5345 5f49 474e 4f52 455f 434f 4e46 4947  SE_IGNORE_CONFIG
+00001150: 5f46 494c 4553 222e 0a0a 5468 6572 6520  _FILES"...There 
+00001160: 6172 6520 7365 7665 7261 6c20 6f74 6865  are several othe
+00001170: 7220 7761 7973 2074 6f20 7573 6520 7468  r ways to use th
+00001180: 6520 6e6f 7365 2074 6573 7420 7275 6e6e  e nose test runn
+00001190: 6572 2062 6573 6964 6573 2074 6865 0a2a  er besides the.*
+000011a0: 6e6f 7365 7465 7374 732a 2073 6372 6970  nosetests* scrip
+000011b0: 742e 2059 6f75 206d 6179 2075 7365 206e  t. You may use n
+000011c0: 6f73 6520 696e 2061 2074 6573 7420 7363  ose in a test sc
+000011d0: 7269 7074 3a0a 0a20 2020 696d 706f 7274  ript:..   import
+000011e0: 206e 6f73 650a 2020 206e 6f73 652e 6d61   nose.   nose.ma
+000011f0: 696e 2829 0a0a 4966 2079 6f75 2064 6f20  in()..If you do 
+00001200: 6e6f 7420 7761 6e74 2074 6865 2074 6573  not want the tes
+00001210: 7420 7363 7269 7074 2074 6f20 6578 6974  t script to exit
+00001220: 2077 6974 6820 3020 6f6e 2073 7563 6365   with 0 on succe
+00001230: 7373 2061 6e64 2031 206f 6e0a 6661 696c  ss and 1 on.fail
+00001240: 7572 6520 286c 696b 6520 756e 6974 7465  ure (like unitte
+00001250: 7374 2e6d 6169 6e29 2c20 7573 6520 6e6f  st.main), use no
+00001260: 7365 2e72 756e 2829 2069 6e73 7465 6164  se.run() instead
+00001270: 3a0a 0a20 2020 696d 706f 7274 206e 6f73  :..   import nos
+00001280: 650a 2020 2072 6573 756c 7420 3d20 6e6f  e.   result = no
+00001290: 7365 2e72 756e 2829 0a0a 2a72 6573 756c  se.run()..*resul
+000012a0: 742a 2077 696c 6c20 6265 2074 7275 6520  t* will be true 
+000012b0: 6966 2074 6865 2074 6573 7420 7275 6e20  if the test run 
+000012c0: 7375 6363 6565 6465 642c 206f 7220 6661  succeeded, or fa
+000012d0: 6c73 6520 6966 2061 6e79 2074 6573 740a  lse if any test.
+000012e0: 6661 696c 6564 206f 7220 7261 6973 6564  failed or raised
+000012f0: 2061 6e20 756e 6361 7567 6874 2065 7863   an uncaught exc
+00001300: 6570 7469 6f6e 2e20 4c61 7374 6c79 2c20  eption. Lastly, 
+00001310: 796f 7520 6361 6e20 7275 6e20 6e6f 7365  you can run nose
+00001320: 2e63 6f72 650a 6469 7265 6374 6c79 2c20  .core.directly, 
+00001330: 7768 6963 6820 7769 6c6c 2072 756e 206e  which will run n
+00001340: 6f73 652e 6d61 696e 2829 3a0a 0a20 2020  ose.main():..   
+00001350: 7079 7468 6f6e 202f 7061 7468 2f74 6f2f  python /path/to/
+00001360: 6e6f 7365 2f63 6f72 652e 7079 0a0a 506c  nose/core.py..Pl
+00001370: 6561 7365 2073 6565 2074 6865 2075 7361  ease see the usa
+00001380: 6765 206d 6573 7361 6765 2066 6f72 2074  ge message for t
+00001390: 6865 206e 6f73 6574 6573 7473 2073 6372  he nosetests scr
+000013a0: 6970 7420 666f 7220 696e 666f 726d 6174  ipt for informat
+000013b0: 696f 6e0a 6162 6f75 7420 686f 7720 746f  ion.about how to
+000013c0: 2063 6f6e 7472 6f6c 2077 6869 6368 2074   control which t
+000013d0: 6573 7473 206e 6f73 6520 7275 6e73 2c20  ests nose runs, 
+000013e0: 7768 6963 6820 706c 7567 696e 7320 6172  which plugins ar
+000013f0: 6520 6c6f 6164 6564 2c0a 616e 6420 7468  e loaded,.and th
+00001400: 6520 7465 7374 206f 7574 7075 742e 0a0a  e test output...
+00001410: 0a45 7874 656e 6465 6420 7573 6167 650a  .Extended usage.
+00001420: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 0a0a  ==============..
+00001430: 6e6f 7365 2063 6f6c 6c65 6374 7320 7465  nose collects te
+00001440: 7374 7320 6175 746f 6d61 7469 6361 6c6c  sts automaticall
+00001450: 7920 6672 6f6d 2070 7974 686f 6e20 736f  y from python so
+00001460: 7572 6365 2066 696c 6573 2c0a 6469 7265  urce files,.dire
+00001470: 6374 6f72 6965 7320 616e 6420 7061 636b  ctories and pack
+00001480: 6167 6573 2066 6f75 6e64 2069 6e20 6974  ages found in it
+00001490: 7320 776f 726b 696e 6720 6469 7265 6374  s working direct
+000014a0: 6f72 7920 2877 6869 6368 0a64 6566 6175  ory (which.defau
+000014b0: 6c74 7320 746f 2074 6865 2063 7572 7265  lts to the curre
+000014c0: 6e74 2077 6f72 6b69 6e67 2064 6972 6563  nt working direc
+000014d0: 746f 7279 292e 2041 6e79 2070 7974 686f  tory). Any pytho
+000014e0: 6e20 736f 7572 6365 2066 696c 652c 0a64  n source file,.d
+000014f0: 6972 6563 746f 7279 206f 7220 7061 636b  irectory or pack
+00001500: 6167 6520 7468 6174 206d 6174 6368 6573  age that matches
+00001510: 2074 6865 2074 6573 744d 6174 6368 2072   the testMatch r
+00001520: 6567 756c 6172 2065 7870 7265 7373 696f  egular expressio
+00001530: 6e20 2862 790a 6465 6661 756c 743a 202a  n (by.default: *
+00001540: 283f 3a5e 7c5b 625f 2e2d 5d29 5b54 745d  (?:^|[b_.-])[Tt]
+00001550: 6573 7429 2a20 7769 6c6c 2062 6520 636f  est)* will be co
+00001560: 6c6c 6563 7465 6420 6173 2061 2074 6573  llected as a tes
+00001570: 7420 286f 7220 736f 7572 6365 0a66 6f72  t (or source.for
+00001580: 2063 6f6c 6c65 6374 696f 6e20 6f66 2074   collection of t
+00001590: 6573 7473 292e 2049 6e20 6164 6469 7469  ests). In additi
+000015a0: 6f6e 2c20 616c 6c20 6f74 6865 7220 7061  on, all other pa
+000015b0: 636b 6167 6573 2066 6f75 6e64 2069 6e20  ckages found in 
+000015c0: 7468 650a 776f 726b 696e 6720 6469 7265  the.working dire
+000015d0: 6374 6f72 7920 7769 6c6c 2062 6520 6578  ctory will be ex
+000015e0: 616d 696e 6564 2066 6f72 2070 7974 686f  amined for pytho
+000015f0: 6e20 736f 7572 6365 2066 696c 6573 206f  n source files o
+00001600: 720a 6469 7265 6374 6f72 6965 7320 7468  r.directories th
+00001610: 6174 206d 6174 6368 2074 6573 744d 6174  at match testMat
+00001620: 6368 2e20 5061 636b 6167 6520 6469 7363  ch. Package disc
+00001630: 6f76 6572 7920 6465 7363 656e 6473 2061  overy descends a
+00001640: 6c6c 2074 6865 0a77 6179 2064 6f77 6e20  ll the.way down 
+00001650: 7468 6520 7472 6565 2c20 736f 2070 6163  the tree, so pac
+00001660: 6b61 6765 2e74 6573 7473 2061 6e64 2070  kage.tests and p
+00001670: 6163 6b61 6765 2e73 7562 2e74 6573 7473  ackage.sub.tests
+00001680: 2061 6e64 0a70 6163 6b61 6765 2e73 7562   and.package.sub
+00001690: 2e73 7562 322e 7465 7374 7320 7769 6c6c  .sub2.tests will
+000016a0: 2061 6c6c 2062 6520 636f 6c6c 6563 7465   all be collecte
+000016b0: 642e 0a0a 5769 7468 696e 2061 2074 6573  d...Within a tes
+000016c0: 7420 6469 7265 6374 6f72 7920 6f72 2070  t directory or p
+000016d0: 6163 6b61 6765 2c20 616e 7920 7079 7468  ackage, any pyth
+000016e0: 6f6e 2073 6f75 7263 6520 6669 6c65 206d  on source file m
+000016f0: 6174 6368 696e 670a 7465 7374 4d61 7463  atching.testMatc
+00001700: 6820 7769 6c6c 2062 6520 6578 616d 696e  h will be examin
+00001710: 6564 2066 6f72 2074 6573 7420 6361 7365  ed for test case
+00001720: 732e 2057 6974 6869 6e20 6120 7465 7374  s. Within a test
+00001730: 206d 6f64 756c 652c 0a66 756e 6374 696f   module,.functio
+00001740: 6e73 2061 6e64 2063 6c61 7373 6573 2077  ns and classes w
+00001750: 686f 7365 206e 616d 6573 206d 6174 6368  hose names match
+00001760: 2074 6573 744d 6174 6368 2061 6e64 2054   testMatch and T
+00001770: 6573 7443 6173 650a 7375 6263 6c61 7373  estCase.subclass
+00001780: 6573 2077 6974 6820 616e 7920 6e61 6d65  es with any name
+00001790: 2077 696c 6c20 6265 206c 6f61 6465 6420   will be loaded 
+000017a0: 616e 6420 6578 6563 7574 6564 2061 7320  and executed as 
+000017b0: 7465 7374 732e 2054 6573 7473 0a6d 6179  tests. Tests.may
+000017c0: 2075 7365 2074 6865 2061 7373 6572 7420   use the assert 
+000017d0: 6b65 7977 6f72 6420 6f72 2072 6169 7365  keyword or raise
+000017e0: 2041 7373 6572 7469 6f6e 4572 726f 7273   AssertionErrors
+000017f0: 2074 6f20 696e 6469 6361 7465 2074 6573   to indicate tes
+00001800: 740a 6661 696c 7572 652e 2054 6573 7443  t.failure. TestC
+00001810: 6173 6520 7375 6263 6c61 7373 6573 206d  ase subclasses m
+00001820: 6179 2064 6f20 7468 6520 7361 6d65 206f  ay do the same o
+00001830: 7220 7573 6520 7468 6520 7661 7269 6f75  r use the variou
+00001840: 730a 5465 7374 4361 7365 206d 6574 686f  s.TestCase metho
+00001850: 6473 2061 7661 696c 6162 6c65 2e0a 0a2a  ds available...*
+00001860: 2a49 7420 6973 2069 6d70 6f72 7461 6e74  *It is important
+00001870: 2074 6f20 6e6f 7465 2074 6861 7420 7468   to note that th
+00001880: 6520 6465 6661 756c 7420 6265 6861 7669  e default behavi
+00001890: 6f72 206f 6620 6e6f 7365 2069 7320 746f  or of nose is to
+000018a0: 206e 6f74 0a69 6e63 6c75 6465 2074 6573   not.include tes
+000018b0: 7473 2066 726f 6d20 6669 6c65 7320 7768  ts from files wh
+000018c0: 6963 6820 6172 6520 6578 6563 7574 6162  ich are executab
+000018d0: 6c65 2e2a 2a20 2054 6f20 696e 636c 7564  le.**  To includ
+000018e0: 6520 7465 7374 730a 6672 6f6d 2073 7563  e tests.from suc
+000018f0: 6820 6669 6c65 732c 2072 656d 6f76 6520  h files, remove 
+00001900: 7468 6569 7220 6578 6563 7574 6162 6c65  their executable
+00001910: 2062 6974 206f 7220 7573 6520 7468 6520   bit or use the 
+00001920: 2d2d 6578 6520 666c 6167 0a28 7365 6520  --exe flag.(see 
+00001930: 274f 7074 696f 6e73 2720 7365 6374 696f  'Options' sectio
+00001940: 6e20 6265 6c6f 7729 2e0a 0a0a 5365 6c65  n below)....Sele
+00001950: 6374 696e 6720 5465 7374 730a 2d2d 2d2d  cting Tests.----
+00001960: 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a 0a54 6f20  -----------..To 
+00001970: 7370 6563 6966 7920 7768 6963 6820 7465  specify which te
+00001980: 7374 7320 746f 2072 756e 2c20 7061 7373  sts to run, pass
+00001990: 2074 6573 7420 6e61 6d65 7320 6f6e 2074   test names on t
+000019a0: 6865 2063 6f6d 6d61 6e64 206c 696e 653a  he command line:
+000019b0: 0a0a 2020 206e 6f73 6574 6573 7473 206f  ..   nosetests o
+000019c0: 6e6c 795f 7465 7374 5f74 6869 732e 7079  nly_test_this.py
+000019d0: 0a0a 5465 7374 206e 616d 6573 2073 7065  ..Test names spe
+000019e0: 6369 6669 6564 206d 6179 2062 6520 6669  cified may be fi
+000019f0: 6c65 206f 7220 6d6f 6475 6c65 206e 616d  le or module nam
+00001a00: 6573 2c20 616e 6420 6d61 7920 6f70 7469  es, and may opti
+00001a10: 6f6e 616c 6c79 0a69 6e64 6963 6174 6520  onally.indicate 
+00001a20: 7468 6520 7465 7374 2063 6173 6520 746f  the test case to
+00001a30: 2072 756e 2062 7920 7365 7061 7261 7469   run by separati
+00001a40: 6e67 2074 6865 206d 6f64 756c 6520 6f72  ng the module or
+00001a50: 2066 696c 6520 6e61 6d65 0a66 726f 6d20   file name.from 
+00001a60: 7468 6520 7465 7374 2063 6173 6520 6e61  the test case na
+00001a70: 6d65 2077 6974 6820 6120 636f 6c6f 6e2e  me with a colon.
+00001a80: 2046 696c 656e 616d 6573 206d 6179 2062   Filenames may b
+00001a90: 6520 7265 6c61 7469 7665 206f 720a 6162  e relative or.ab
+00001aa0: 736f 6c75 7465 2e20 4578 616d 706c 6573  solute. Examples
+00001ab0: 3a0a 0a20 2020 6e6f 7365 7465 7374 7320  :..   nosetests 
+00001ac0: 7465 7374 2e6d 6f64 756c 650a 2020 206e  test.module.   n
+00001ad0: 6f73 6574 6573 7473 2061 6e6f 7468 6572  osetests another
+00001ae0: 2e74 6573 743a 5465 7374 4361 7365 2e74  .test:TestCase.t
+00001af0: 6573 745f 6d65 7468 6f64 0a20 2020 6e6f  est_method.   no
+00001b00: 7365 7465 7374 7320 612e 7465 7374 3a54  setests a.test:T
+00001b10: 6573 7443 6173 650a 2020 206e 6f73 6574  estCase.   noset
+00001b20: 6573 7473 202f 7061 7468 2f74 6f2f 7465  ests /path/to/te
+00001b30: 7374 2f66 696c 652e 7079 3a74 6573 745f  st/file.py:test_
+00001b40: 6675 6e63 7469 6f6e 0a0a 596f 7520 6d61  function..You ma
+00001b50: 7920 616c 736f 2063 6861 6e67 6520 7468  y also change th
+00001b60: 6520 776f 726b 696e 6720 6469 7265 6374  e working direct
+00001b70: 6f72 7920 7768 6572 6520 6e6f 7365 206c  ory where nose l
+00001b80: 6f6f 6b73 2066 6f72 2074 6573 7473 0a62  ooks for tests.b
+00001b90: 7920 7573 696e 6720 7468 6520 2d77 2073  y using the -w s
+00001ba0: 7769 7463 683a 0a0a 2020 206e 6f73 6574  witch:..   noset
+00001bb0: 6573 7473 202d 7720 2f70 6174 682f 746f  ests -w /path/to
+00001bc0: 2f74 6573 7473 0a0a 4e6f 7465 2c20 686f  /tests..Note, ho
+00001bd0: 7765 7665 722c 2074 6861 7420 7375 7070  wever, that supp
+00001be0: 6f72 7420 666f 7220 6d75 6c74 6970 6c65  ort for multiple
+00001bf0: 202d 7720 6172 6775 6d65 6e74 7320 6973   -w arguments is
+00001c00: 206e 6f77 0a64 6570 7265 6361 7465 6420   now.deprecated 
+00001c10: 616e 6420 7769 6c6c 2062 6520 7265 6d6f  and will be remo
+00001c20: 7665 6420 696e 2061 2066 7574 7572 6520  ved in a future 
+00001c30: 7265 6c65 6173 652e 2041 7320 6f66 206e  release. As of n
+00001c40: 6f73 6520 302e 3130 2c0a 796f 7520 6361  ose 0.10,.you ca
+00001c50: 6e20 6765 7420 7468 6520 7361 6d65 2062  n get the same b
+00001c60: 6568 6176 696f 7220 6279 2073 7065 6369  ehavior by speci
+00001c70: 6679 696e 6720 7468 6520 7461 7267 6574  fying the target
+00001c80: 2064 6972 6563 746f 7269 6573 0a2a 7769   directories.*wi
+00001c90: 7468 6f75 742a 2074 6865 202d 7720 7377  thout* the -w sw
+00001ca0: 6974 6368 3a0a 0a20 2020 6e6f 7365 7465  itch:..   nosete
+00001cb0: 7374 7320 2f70 6174 682f 746f 2f74 6573  sts /path/to/tes
+00001cc0: 7473 202f 616e 6f74 6865 722f 7061 7468  ts /another/path
+00001cd0: 2f74 6f2f 7465 7374 730a 0a46 7572 7468  /to/tests..Furth
+00001ce0: 6572 2063 7573 746f 6d69 7a61 7469 6f6e  er customization
+00001cf0: 206f 6620 7465 7374 2073 656c 6563 7469   of test selecti
+00001d00: 6f6e 2061 6e64 206c 6f61 6469 6e67 2069  on and loading i
+00001d10: 7320 706f 7373 6962 6c65 0a74 6872 6f75  s possible.throu
+00001d20: 6768 2074 6865 2075 7365 206f 6620 706c  gh the use of pl
+00001d30: 7567 696e 732e 0a0a 5465 7374 2072 6573  ugins...Test res
+00001d40: 756c 7420 6f75 7470 7574 2069 7320 6964  ult output is id
+00001d50: 656e 7469 6361 6c20 746f 2074 6861 7420  entical to that 
+00001d60: 6f66 2075 6e69 7474 6573 742c 2065 7863  of unittest, exc
+00001d70: 6570 7420 666f 7220 7468 650a 6164 6469  ept for the.addi
+00001d80: 7469 6f6e 616c 2066 6561 7475 7265 7320  tional features 
+00001d90: 2865 7272 6f72 2063 6c61 7373 6573 2c20  (error classes, 
+00001da0: 616e 6420 706c 7567 696e 2d73 7570 706c  and plugin-suppl
+00001db0: 6965 6420 6665 6174 7572 6573 2073 7563  ied features suc
+00001dc0: 680a 6173 206f 7574 7075 7420 6361 7074  h.as output capt
+00001dd0: 7572 6520 616e 6420 6173 7365 7274 2069  ure and assert i
+00001de0: 6e74 726f 7370 6563 7469 6f6e 2920 6465  ntrospection) de
+00001df0: 7461 696c 6564 2069 6e20 7468 6520 6f70  tailed in the op
+00001e00: 7469 6f6e 730a 6265 6c6f 772e 0a0a 0a43  tions.below....C
+00001e10: 6f6e 6669 6775 7261 7469 6f6e 0a2d 2d2d  onfiguration.---
+00001e20: 2d2d 2d2d 2d2d 2d2d 2d2d 0a0a 496e 2061  ----------..In a
+00001e30: 6464 6974 696f 6e20 746f 2070 6173 7369  ddition to passi
+00001e40: 6e67 2063 6f6d 6d61 6e64 2d6c 696e 6520  ng command-line 
+00001e50: 6f70 7469 6f6e 732c 2079 6f75 206d 6179  options, you may
+00001e60: 2061 6c73 6f20 7075 740a 636f 6e66 6967   also put.config
+00001e70: 7572 6174 696f 6e20 6f70 7469 6f6e 7320  uration options 
+00001e80: 696e 2079 6f75 7220 7072 6f6a 6563 7420  in your project 
+00001e90: 2a73 6574 7570 2e63 6667 2a20 6669 6c65  *setup.cfg* file
+00001ea0: 2c20 6f72 2061 202e 6e6f 7365 7263 0a6f  , or a .noserc.o
+00001eb0: 7220 6e6f 7365 2e63 6667 2066 696c 6520  r nose.cfg file 
+00001ec0: 696e 2079 6f75 7220 686f 6d65 2064 6972  in your home dir
+00001ed0: 6563 746f 7279 2e20 496e 2061 6e79 206f  ectory. In any o
+00001ee0: 6620 7468 6573 6520 7374 616e 6461 7264  f these standard
+00001ef0: 2069 6e69 2d0a 7374 796c 6520 636f 6e66   ini-.style conf
+00001f00: 6967 2066 696c 6573 2c20 796f 7520 7075  ig files, you pu
+00001f10: 7420 796f 7572 206e 6f73 6574 6573 7473  t your nosetests
+00001f20: 2063 6f6e 6669 6775 7261 7469 6f6e 2069   configuration i
+00001f30: 6e20 610a 225b 6e6f 7365 7465 7374 735d  n a."[nosetests]
+00001f40: 2220 7365 6374 696f 6e2e 204f 7074 696f  " section. Optio
+00001f50: 6e73 2061 7265 2074 6865 2073 616d 6520  ns are the same 
+00001f60: 6173 206f 6e20 7468 6520 636f 6d6d 616e  as on the comman
+00001f70: 6420 6c69 6e65 2c0a 7769 7468 2074 6865  d line,.with the
+00001f80: 202d 2d20 7072 6566 6978 2072 656d 6f76   -- prefix remov
+00001f90: 6564 2e20 466f 7220 6f70 7469 6f6e 7320  ed. For options 
+00001fa0: 7468 6174 2061 7265 2073 696d 706c 6520  that are simple 
+00001fb0: 7377 6974 6368 6573 2c20 796f 750a 6d75  switches, you.mu
+00001fc0: 7374 2073 7570 706c 7920 6120 7661 6c75  st supply a valu
+00001fd0: 653a 0a0a 2020 205b 6e6f 7365 7465 7374  e:..   [nosetest
+00001fe0: 735d 0a20 2020 7665 7262 6f73 6974 793d  s].   verbosity=
+00001ff0: 330a 2020 2077 6974 682d 646f 6374 6573  3.   with-doctes
+00002000: 743d 310a 0a41 6c6c 2063 6f6e 6669 6775  t=1..All configu
+00002010: 7261 7469 6f6e 2066 696c 6573 2074 6861  ration files tha
+00002020: 7420 6172 6520 666f 756e 6420 7769 6c6c  t are found will
+00002030: 2062 6520 6c6f 6164 6564 2061 6e64 2074   be loaded and t
+00002040: 6865 6972 0a6f 7074 696f 6e73 2063 6f6d  heir.options com
+00002050: 6269 6e65 642e 2059 6f75 2063 616e 206f  bined. You can o
+00002060: 7665 7272 6964 6520 7468 6520 7374 616e  verride the stan
+00002070: 6461 7264 2063 6f6e 6669 6720 6669 6c65  dard config file
+00002080: 206c 6f61 6469 6e67 0a77 6974 6820 7468   loading.with th
+00002090: 6520 222d 6322 206f 7074 696f 6e2e 0a0a  e "-c" option...
+000020a0: 0a55 7369 6e67 2050 6c75 6769 6e73 0a2d  .Using Plugins.-
+000020b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0a0a 5468  ------------..Th
+000020c0: 6572 6520 6172 6520 6e75 6d65 726f 7573  ere are numerous
+000020d0: 206e 6f73 6520 706c 7567 696e 7320 6176   nose plugins av
+000020e0: 6169 6c61 626c 6520 7669 6120 6561 7379  ailable via easy
+000020f0: 5f69 6e73 7461 6c6c 2061 6e64 0a65 6c73  _install and.els
+00002100: 6577 6865 7265 2e20 546f 2075 7365 2061  ewhere. To use a
+00002110: 2070 6c75 6769 6e2c 206a 7573 7420 696e   plugin, just in
+00002120: 7374 616c 6c20 6974 2e20 5468 6520 706c  stall it. The pl
+00002130: 7567 696e 2077 696c 6c20 6164 640a 636f  ugin will add.co
+00002140: 6d6d 616e 6420 6c69 6e65 206f 7074 696f  mmand line optio
+00002150: 6e73 2074 6f20 6e6f 7365 7465 7374 732e  ns to nosetests.
+00002160: 2054 6f20 7665 7269 6679 2074 6861 7420   To verify that 
+00002170: 7468 6520 706c 7567 696e 2069 730a 696e  the plugin is.in
+00002180: 7374 616c 6c65 642c 2072 756e 3a0a 0a20  stalled, run:.. 
+00002190: 2020 6e6f 7365 7465 7374 7320 2d2d 706c    nosetests --pl
+000021a0: 7567 696e 730a 0a59 6f75 2063 616e 2061  ugins..You can a
+000021b0: 6464 202d 7620 6f72 202d 7676 2074 6f20  dd -v or -vv to 
+000021c0: 7468 6174 2063 6f6d 6d61 6e64 2074 6f20  that command to 
+000021d0: 7368 6f77 206d 6f72 6520 696e 666f 726d  show more inform
+000021e0: 6174 696f 6e20 6162 6f75 740a 6561 6368  ation about.each
+000021f0: 2070 6c75 6769 6e2e 0a0a 4966 2079 6f75   plugin...If you
+00002200: 2061 7265 2072 756e 6e69 6e67 206e 6f73   are running nos
+00002210: 652e 6d61 696e 2829 206f 7220 6e6f 7365  e.main() or nose
+00002220: 2e72 756e 2829 2066 726f 6d20 6120 7363  .run() from a sc
+00002230: 7269 7074 2c20 796f 7520 6361 6e0a 7370  ript, you can.sp
+00002240: 6563 6966 7920 6120 6c69 7374 206f 6620  ecify a list of 
+00002250: 706c 7567 696e 7320 746f 2075 7365 2062  plugins to use b
+00002260: 7920 7061 7373 696e 6720 6120 6c69 7374  y passing a list
+00002270: 206f 6620 706c 7567 696e 7320 7769 7468   of plugins with
+00002280: 2074 6865 0a70 6c75 6769 6e73 206b 6579   the.plugins key
+00002290: 776f 7264 2061 7267 756d 656e 742e 0a0a  word argument...
+000022a0: 0a4f 7074 696f 6e73 0a2d 2d2d 2d2d 2d2d  .Options.-------
+000022b0: 0a0a 2d56 2c20 2d2d 7665 7273 696f 6e0a  ..-V, --version.
+000022c0: 0a20 2020 4f75 7470 7574 206e 6f73 6520  .   Output nose 
+000022d0: 7665 7273 696f 6e20 616e 6420 6578 6974  version and exit
+000022e0: 0a0a 2d70 2c20 2d2d 706c 7567 696e 730a  ..-p, --plugins.
+000022f0: 0a20 2020 4f75 7470 7574 206c 6973 7420  .   Output list 
+00002300: 6f66 2061 7661 696c 6162 6c65 2070 6c75  of available plu
+00002310: 6769 6e73 2061 6e64 2065 7869 742e 2043  gins and exit. C
+00002320: 6f6d 6269 6e65 2077 6974 6820 6869 6768  ombine with high
+00002330: 6572 0a20 2020 7665 7262 6f73 6974 7920  er.   verbosity 
+00002340: 666f 7220 6772 6561 7465 7220 6465 7461  for greater deta
+00002350: 696c 0a0a 2d76 3d44 4546 4155 4c54 2c20  il..-v=DEFAULT, 
+00002360: 2d2d 7665 7262 6f73 653d 4445 4641 554c  --verbose=DEFAUL
+00002370: 540a 0a20 2020 4265 206d 6f72 6520 7665  T..   Be more ve
+00002380: 7262 6f73 652e 205b 4e4f 5345 5f56 4552  rbose. [NOSE_VER
+00002390: 424f 5345 5d0a 0a2d 2d76 6572 626f 7369  BOSE]..--verbosi
+000023a0: 7479 3d56 4552 424f 5349 5459 0a0a 2020  ty=VERBOSITY..  
+000023b0: 2053 6574 2076 6572 626f 7369 7479 3b20   Set verbosity; 
+000023c0: 2d2d 7665 7262 6f73 6974 793d 3220 6973  --verbosity=2 is
+000023d0: 2074 6865 2073 616d 6520 6173 202d 760a   the same as -v.
+000023e0: 0a2d 713d 4445 4641 554c 542c 202d 2d71  .-q=DEFAULT, --q
+000023f0: 7569 6574 3d44 4546 4155 4c54 0a0a 2020  uiet=DEFAULT..  
+00002400: 2042 6520 6c65 7373 2076 6572 626f 7365   Be less verbose
+00002410: 0a0a 2d63 3d46 494c 4553 2c20 2d2d 636f  ..-c=FILES, --co
+00002420: 6e66 6967 3d46 494c 4553 0a0a 2020 204c  nfig=FILES..   L
+00002430: 6f61 6420 636f 6e66 6967 7572 6174 696f  oad configuratio
+00002440: 6e20 6672 6f6d 2063 6f6e 6669 6720 6669  n from config fi
+00002450: 6c65 2873 292e 204d 6179 2062 6520 7370  le(s). May be sp
+00002460: 6563 6966 6965 6420 6d75 6c74 6970 6c65  ecified multiple
+00002470: 0a20 2020 7469 6d65 733b 2069 6e20 7468  .   times; in th
+00002480: 6174 2063 6173 652c 2061 6c6c 2063 6f6e  at case, all con
+00002490: 6669 6720 6669 6c65 7320 7769 6c6c 2062  fig files will b
+000024a0: 6520 6c6f 6164 6564 2061 6e64 2063 6f6d  e loaded and com
+000024b0: 6269 6e65 640a 0a2d 773d 5748 4552 452c  bined..-w=WHERE,
+000024c0: 202d 2d77 6865 7265 3d57 4845 5245 0a0a   --where=WHERE..
+000024d0: 2020 204c 6f6f 6b20 666f 7220 7465 7374     Look for test
+000024e0: 7320 696e 2074 6869 7320 6469 7265 6374  s in this direct
+000024f0: 6f72 792e 204d 6179 2062 6520 7370 6563  ory. May be spec
+00002500: 6966 6965 6420 6d75 6c74 6970 6c65 2074  ified multiple t
+00002510: 696d 6573 2e0a 2020 2054 6865 2066 6972  imes..   The fir
+00002520: 7374 2064 6972 6563 746f 7279 2070 6173  st directory pas
+00002530: 7365 6420 7769 6c6c 2062 6520 7573 6564  sed will be used
+00002540: 2061 7320 7468 6520 776f 726b 696e 6720   as the working 
+00002550: 6469 7265 6374 6f72 792c 0a20 2020 696e  directory,.   in
+00002560: 2070 6c61 6365 206f 6620 7468 6520 6375   place of the cu
+00002570: 7272 656e 7420 776f 726b 696e 6720 6469  rrent working di
+00002580: 7265 6374 6f72 792c 2077 6869 6368 2069  rectory, which i
+00002590: 7320 7468 6520 6465 6661 756c 742e 0a20  s the default.. 
+000025a0: 2020 4f74 6865 7273 2077 696c 6c20 6265    Others will be
+000025b0: 2061 6464 6564 2074 6f20 7468 6520 6c69   added to the li
+000025c0: 7374 206f 6620 7465 7374 7320 746f 2065  st of tests to e
+000025d0: 7865 6375 7465 2e20 5b4e 4f53 455f 5748  xecute. [NOSE_WH
+000025e0: 4552 455d 0a0a 2d2d 7079 3377 6865 7265  ERE]..--py3where
+000025f0: 3d50 5933 5748 4552 450a 0a20 2020 4c6f  =PY3WHERE..   Lo
+00002600: 6f6b 2066 6f72 2074 6573 7473 2069 6e20  ok for tests in 
+00002610: 7468 6973 2064 6972 6563 746f 7279 2075  this directory u
+00002620: 6e64 6572 2050 7974 686f 6e20 332e 782e  nder Python 3.x.
+00002630: 2046 756e 6374 696f 6e73 2074 6865 0a20   Functions the. 
+00002640: 2020 7361 6d65 2061 7320 2777 6865 7265    same as 'where
+00002650: 272c 2062 7574 206f 6e6c 7920 6170 706c  ', but only appl
+00002660: 6965 7320 6966 2072 756e 6e69 6e67 2075  ies if running u
+00002670: 6e64 6572 2050 7974 686f 6e20 332e 7820  nder Python 3.x 
+00002680: 6f72 0a20 2020 6162 6f76 652e 2020 4e6f  or.   above.  No
+00002690: 7465 2074 6861 742c 2069 6620 7072 6573  te that, if pres
+000026a0: 656e 7420 756e 6465 7220 332e 782c 2074  ent under 3.x, t
+000026b0: 6869 7320 6f70 7469 6f6e 2063 6f6d 706c  his option compl
+000026c0: 6574 656c 790a 2020 2072 6570 6c61 6365  etely.   replace
+000026d0: 7320 616e 7920 6469 7265 6374 6f72 6965  s any directorie
+000026e0: 7320 7370 6563 6966 6965 6420 7769 7468  s specified with
+000026f0: 2027 7768 6572 6527 2c20 736f 2074 6865   'where', so the
+00002700: 2027 7768 6572 6527 0a20 2020 6f70 7469   'where'.   opti
+00002710: 6f6e 2062 6563 6f6d 6573 2069 6e65 6666  on becomes ineff
+00002720: 6563 7469 7665 2e20 5b4e 4f53 455f 5059  ective. [NOSE_PY
+00002730: 3357 4845 5245 5d0a 0a2d 6d3d 5245 4745  3WHERE]..-m=REGE
+00002740: 582c 202d 2d6d 6174 6368 3d52 4547 4558  X, --match=REGEX
+00002750: 2c20 2d2d 7465 7374 6d61 7463 683d 5245  , --testmatch=RE
+00002760: 4745 580a 0a20 2020 4669 6c65 732c 2064  GEX..   Files, d
+00002770: 6972 6563 746f 7269 6573 2c20 6675 6e63  irectories, func
+00002780: 7469 6f6e 206e 616d 6573 2c20 616e 6420  tion names, and 
+00002790: 636c 6173 7320 6e61 6d65 7320 7468 6174  class names that
+000027a0: 206d 6174 6368 2074 6869 730a 2020 2072   match this.   r
+000027b0: 6567 756c 6172 2065 7870 7265 7373 696f  egular expressio
+000027c0: 6e20 6172 6520 636f 6e73 6964 6572 6564  n are considered
+000027d0: 2074 6573 7473 2e20 2044 6566 6175 6c74   tests.  Default
+000027e0: 3a0a 2020 2028 3f3a 5e7c 5b62 5f2e 2f2d  :.   (?:^|[b_./-
+000027f0: 5d29 5b54 745d 6573 7420 5b4e 4f53 455f  ])[Tt]est [NOSE_
+00002800: 5445 5354 4d41 5443 485d 0a0a 2d2d 7465  TESTMATCH]..--te
+00002810: 7374 733d 4e41 4d45 530a 0a20 2020 5275  sts=NAMES..   Ru
+00002820: 6e20 7468 6573 6520 7465 7374 7320 2863  n these tests (c
+00002830: 6f6d 6d61 2d73 6570 6172 6174 6564 206c  omma-separated l
+00002840: 6973 7429 2e20 5468 6973 2061 7267 756d  ist). This argum
+00002850: 656e 7420 6973 2075 7365 6675 6c0a 2020  ent is useful.  
+00002860: 206d 6169 6e6c 7920 6672 6f6d 2063 6f6e   mainly from con
+00002870: 6669 6775 7261 7469 6f6e 2066 696c 6573  figuration files
+00002880: 3b20 6f6e 2074 6865 2063 6f6d 6d61 6e64  ; on the command
+00002890: 206c 696e 652c 206a 7573 7420 7061 7373   line, just pass
+000028a0: 2074 6865 0a20 2020 7465 7374 7320 746f   the.   tests to
+000028b0: 2072 756e 2061 7320 6164 6469 7469 6f6e   run as addition
+000028c0: 616c 2061 7267 756d 656e 7473 2077 6974  al arguments wit
+000028d0: 6820 6e6f 2073 7769 7463 682e 0a0a 2d6c  h no switch...-l
+000028e0: 3d44 4546 4155 4c54 2c20 2d2d 6465 6275  =DEFAULT, --debu
+000028f0: 673d 4445 4641 554c 540a 0a20 2020 4163  g=DEFAULT..   Ac
+00002900: 7469 7661 7465 2064 6562 7567 206c 6f67  tivate debug log
+00002910: 6769 6e67 2066 6f72 206f 6e65 206f 7220  ging for one or 
+00002920: 6d6f 7265 2073 7973 7465 6d73 2e20 4176  more systems. Av
+00002930: 6169 6c61 626c 6520 6465 6275 670a 2020  ailable debug.  
+00002940: 206c 6f67 6765 7273 3a20 6e6f 7365 2c20   loggers: nose, 
+00002950: 6e6f 7365 2e69 6d70 6f72 7465 722c 206e  nose.importer, n
+00002960: 6f73 652e 696e 7370 6563 746f 722c 206e  ose.inspector, n
+00002970: 6f73 652e 706c 7567 696e 732c 0a20 2020  ose.plugins,.   
+00002980: 6e6f 7365 2e72 6573 756c 7420 616e 6420  nose.result and 
+00002990: 6e6f 7365 2e73 656c 6563 746f 722e 2053  nose.selector. S
+000029a0: 6570 6172 6174 6520 6d75 6c74 6970 6c65  eparate multiple
+000029b0: 206e 616d 6573 2077 6974 6820 610a 2020   names with a.  
+000029c0: 2063 6f6d 6d61 2e0a 0a2d 2d64 6562 7567   comma...--debug
+000029d0: 2d6c 6f67 3d46 494c 450a 0a20 2020 4c6f  -log=FILE..   Lo
+000029e0: 6720 6465 6275 6720 6d65 7373 6167 6573  g debug messages
+000029f0: 2074 6f20 7468 6973 2066 696c 6520 2864   to this file (d
+00002a00: 6566 6175 6c74 3a20 7379 732e 7374 6465  efault: sys.stde
+00002a10: 7272 290a 0a2d 2d6c 6f67 6769 6e67 2d63  rr)..--logging-c
+00002a20: 6f6e 6669 673d 4649 4c45 2c20 2d2d 6c6f  onfig=FILE, --lo
+00002a30: 672d 636f 6e66 6967 3d46 494c 450a 0a20  g-config=FILE.. 
+00002a40: 2020 4c6f 6164 206c 6f67 6769 6e67 2063    Load logging c
+00002a50: 6f6e 6669 6720 6672 6f6d 2074 6869 7320  onfig from this 
+00002a60: 6669 6c65 202d 2d20 6279 7061 7373 6573  file -- bypasses
+00002a70: 2061 6c6c 206f 7468 6572 206c 6f67 6769   all other loggi
+00002a80: 6e67 0a20 2020 636f 6e66 6967 2073 6574  ng.   config set
+00002a90: 7469 6e67 732e 0a0a 2d49 3d52 4547 4558  tings...-I=REGEX
+00002aa0: 2c20 2d2d 6967 6e6f 7265 2d66 696c 6573  , --ignore-files
+00002ab0: 3d52 4547 4558 0a0a 2020 2043 6f6d 706c  =REGEX..   Compl
+00002ac0: 6574 656c 7920 6967 6e6f 7265 2061 6e79  etely ignore any
+00002ad0: 2066 696c 6520 7468 6174 206d 6174 6368   file that match
+00002ae0: 6573 2074 6869 7320 7265 6775 6c61 7220  es this regular 
+00002af0: 6578 7072 6573 7369 6f6e 2e0a 2020 2054  expression..   T
+00002b00: 616b 6573 2070 7265 6365 6465 6e63 6520  akes precedence 
+00002b10: 6f76 6572 2061 6e79 206f 7468 6572 2073  over any other s
+00002b20: 6574 7469 6e67 7320 6f72 2070 6c75 6769  ettings or plugi
+00002b30: 6e73 2e20 5370 6563 6966 7969 6e67 0a20  ns. Specifying. 
+00002b40: 2020 7468 6973 206f 7074 696f 6e20 7769    this option wi
+00002b50: 6c6c 2072 6570 6c61 6365 2074 6865 2064  ll replace the d
+00002b60: 6566 6175 6c74 2073 6574 7469 6e67 2e20  efault setting. 
+00002b70: 5370 6563 6966 7920 7468 6973 206f 7074  Specify this opt
+00002b80: 696f 6e0a 2020 206d 756c 7469 706c 6520  ion.   multiple 
+00002b90: 7469 6d65 7320 746f 2061 6464 206d 6f72  times to add mor
+00002ba0: 6520 7265 6775 6c61 7220 6578 7072 6573  e regular expres
+00002bb0: 7369 6f6e 7320 5b4e 4f53 455f 4947 4e4f  sions [NOSE_IGNO
+00002bc0: 5245 5f46 494c 4553 5d0a 0a2d 653d 5245  RE_FILES]..-e=RE
+00002bd0: 4745 582c 202d 2d65 7863 6c75 6465 3d52  GEX, --exclude=R
+00002be0: 4547 4558 0a0a 2020 2044 6f20 6e6f 7420  EGEX..   Do not 
+00002bf0: 7275 6e20 7465 7374 7320 7468 6174 206d  run tests that m
+00002c00: 6174 6368 2072 6567 756c 6172 2065 7870  atch regular exp
+00002c10: 7265 7373 696f 6e20 5b4e 4f53 455f 4558  ression [NOSE_EX
+00002c20: 434c 5544 455d 0a0a 2d69 3d52 4547 4558  CLUDE]..-i=REGEX
+00002c30: 2c20 2d2d 696e 636c 7564 653d 5245 4745  , --include=REGE
+00002c40: 580a 0a20 2020 5468 6973 2072 6567 756c  X..   This regul
+00002c50: 6172 2065 7870 7265 7373 696f 6e20 7769  ar expression wi
+00002c60: 6c6c 2062 6520 6170 706c 6965 6420 746f  ll be applied to
+00002c70: 2066 696c 6573 2c20 6469 7265 6374 6f72   files, director
+00002c80: 6965 732c 0a20 2020 6675 6e63 7469 6f6e  ies,.   function
+00002c90: 206e 616d 6573 2c20 616e 6420 636c 6173   names, and clas
+00002ca0: 7320 6e61 6d65 7320 666f 7220 6120 6368  s names for a ch
+00002cb0: 616e 6365 2074 6f20 696e 636c 7564 6520  ance to include 
+00002cc0: 6164 6469 7469 6f6e 616c 0a20 2020 7465  additional.   te
+00002cd0: 7374 7320 7468 6174 2064 6f20 6e6f 7420  sts that do not 
+00002ce0: 6d61 7463 6820 5445 5354 4d41 5443 482e  match TESTMATCH.
+00002cf0: 2020 5370 6563 6966 7920 7468 6973 206f    Specify this o
+00002d00: 7074 696f 6e20 6d75 6c74 6970 6c65 0a20  ption multiple. 
+00002d10: 2020 7469 6d65 7320 746f 2061 6464 206d    times to add m
+00002d20: 6f72 6520 7265 6775 6c61 7220 6578 7072  ore regular expr
+00002d30: 6573 7369 6f6e 7320 5b4e 4f53 455f 494e  essions [NOSE_IN
+00002d40: 434c 5544 455d 0a0a 2d78 2c20 2d2d 7374  CLUDE]..-x, --st
+00002d50: 6f70 0a0a 2020 2053 746f 7020 7275 6e6e  op..   Stop runn
+00002d60: 696e 6720 7465 7374 7320 6166 7465 7220  ing tests after 
+00002d70: 7468 6520 6669 7273 7420 6572 726f 7220  the first error 
+00002d80: 6f72 2066 6169 6c75 7265 0a0a 2d50 2c20  or failure..-P, 
+00002d90: 2d2d 6e6f 2d70 6174 682d 6164 6a75 7374  --no-path-adjust
+00002da0: 6d65 6e74 0a0a 2020 2044 6f20 6e6f 7420  ment..   Do not 
+00002db0: 6d61 6b65 2061 6e79 2063 6861 6e67 6573  make any changes
+00002dc0: 2074 6f20 7379 732e 7061 7468 2077 6865   to sys.path whe
+00002dd0: 6e20 6c6f 6164 696e 6720 7465 7374 7320  n loading tests 
+00002de0: 5b4e 4f53 455f 4e4f 5041 5448 5d0a 0a2d  [NOSE_NOPATH]..-
+00002df0: 2d65 7865 0a0a 2020 204c 6f6f 6b20 666f  -exe..   Look fo
+00002e00: 7220 7465 7374 7320 696e 2070 7974 686f  r tests in pytho
+00002e10: 6e20 6d6f 6475 6c65 7320 7468 6174 2061  n modules that a
+00002e20: 7265 2065 7865 6375 7461 626c 652e 204e  re executable. N
+00002e30: 6f72 6d61 6c0a 2020 2062 6568 6176 696f  ormal.   behavio
+00002e40: 7220 6973 2074 6f20 6578 636c 7564 6520  r is to exclude 
+00002e50: 6578 6563 7574 6162 6c65 206d 6f64 756c  executable modul
+00002e60: 6573 2c20 7369 6e63 6520 7468 6579 206d  es, since they m
+00002e70: 6179 206e 6f74 2062 650a 2020 2069 6d70  ay not be.   imp
+00002e80: 6f72 742d 7361 6665 205b 4e4f 5345 5f49  ort-safe [NOSE_I
+00002e90: 4e43 4c55 4445 5f45 5845 5d0a 0a2d 2d6e  NCLUDE_EXE]..--n
+00002ea0: 6f65 7865 0a0a 2020 2044 4f20 4e4f 5420  oexe..   DO NOT 
+00002eb0: 6c6f 6f6b 2066 6f72 2074 6573 7473 2069  look for tests i
+00002ec0: 6e20 7079 7468 6f6e 206d 6f64 756c 6573  n python modules
+00002ed0: 2074 6861 7420 6172 6520 6578 6563 7574   that are execut
+00002ee0: 6162 6c65 2e20 2854 6865 0a20 2020 6465  able. (The.   de
+00002ef0: 6661 756c 7420 6f6e 2074 6865 2077 696e  fault on the win
+00002f00: 646f 7773 2070 6c61 7466 6f72 6d20 6973  dows platform is
+00002f10: 2074 6f20 646f 2073 6f2e 290a 0a2d 2d74   to do so.)..--t
+00002f20: 7261 7665 7273 652d 6e61 6d65 7370 6163  raverse-namespac
+00002f30: 650a 0a20 2020 5472 6176 6572 7365 2074  e..   Traverse t
+00002f40: 6872 6f75 6768 2061 6c6c 2070 6174 6820  hrough all path 
+00002f50: 656e 7472 6965 7320 6f66 2061 206e 616d  entries of a nam
+00002f60: 6573 7061 6365 2070 6163 6b61 6765 0a0a  espace package..
+00002f70: 2d2d 6669 7273 742d 7061 636b 6167 652d  --first-package-
+00002f80: 7769 6e73 2c20 2d2d 6669 7273 742d 706b  wins, --first-pk
+00002f90: 672d 7769 6e73 2c20 2d2d 3173 742d 706b  g-wins, --1st-pk
+00002fa0: 672d 7769 6e73 0a0a 2020 2054 6865 206e  g-wins..   The n
+00002fb0: 6f73 6520 696d 706f 7274 6572 2077 696c  ose importer wil
+00002fc0: 6c20 6e6f 726d 616c 6c79 2065 7669 6374  l normally evict
+00002fd0: 2061 2070 6163 6b61 6765 2066 726f 6d20   a package from 
+00002fe0: 7379 732e 6d6f 6475 6c65 7320 6966 0a20  sys.modules if. 
+00002ff0: 2020 6974 2073 6565 7320 6120 7061 636b    it sees a pack
+00003000: 6167 6520 7769 7468 2074 6865 2073 616d  age with the sam
+00003010: 6520 6e61 6d65 2069 6e20 6120 6469 6666  e name in a diff
+00003020: 6572 656e 7420 6c6f 6361 7469 6f6e 2e20  erent location. 
+00003030: 5365 740a 2020 2074 6869 7320 6f70 7469  Set.   this opti
+00003040: 6f6e 2074 6f20 6469 7361 626c 6520 7468  on to disable th
+00003050: 6174 2062 6568 6176 696f 722e 0a0a 2d2d  at behavior...--
+00003060: 6e6f 2d62 7974 652d 636f 6d70 696c 650a  no-byte-compile.
+00003070: 0a20 2020 5072 6576 656e 7420 6e6f 7365  .   Prevent nose
+00003080: 2066 726f 6d20 6279 7465 2d63 6f6d 7069   from byte-compi
+00003090: 6c69 6e67 2074 6865 2073 6f75 7263 6520  ling the source 
+000030a0: 696e 746f 202e 7079 6320 6669 6c65 7320  into .pyc files 
+000030b0: 7768 696c 650a 2020 206e 6f73 6520 6973  while.   nose is
+000030c0: 2073 6361 6e6e 696e 6720 666f 7220 616e   scanning for an
+000030d0: 6420 7275 6e6e 696e 6720 7465 7374 732e  d running tests.
+000030e0: 0a0a 2d61 3d41 5454 522c 202d 2d61 7474  ..-a=ATTR, --att
+000030f0: 723d 4154 5452 0a0a 2020 2052 756e 206f  r=ATTR..   Run o
+00003100: 6e6c 7920 7465 7374 7320 7468 6174 2068  nly tests that h
+00003110: 6176 6520 6174 7472 6962 7574 6573 2073  ave attributes s
+00003120: 7065 6369 6669 6564 2062 7920 4154 5452  pecified by ATTR
+00003130: 205b 4e4f 5345 5f41 5454 525d 0a0a 2d41   [NOSE_ATTR]..-A
+00003140: 3d45 5850 522c 202d 2d65 7661 6c2d 6174  =EXPR, --eval-at
+00003150: 7472 3d45 5850 520a 0a20 2020 5275 6e20  tr=EXPR..   Run 
+00003160: 6f6e 6c79 2074 6573 7473 2066 6f72 2077  only tests for w
+00003170: 686f 7365 2061 7474 7269 6275 7465 7320  hose attributes 
+00003180: 7468 6520 5079 7468 6f6e 2065 7870 7265  the Python expre
+00003190: 7373 696f 6e20 4558 5052 0a20 2020 6576  ssion EXPR.   ev
+000031a0: 616c 7561 7465 7320 746f 2054 7275 6520  aluates to True 
+000031b0: 5b4e 4f53 455f 4556 414c 5f41 5454 525d  [NOSE_EVAL_ATTR]
+000031c0: 0a0a 2d73 2c20 2d2d 6e6f 6361 7074 7572  ..-s, --nocaptur
+000031d0: 650a 0a20 2020 446f 206e 6f74 2063 6170  e..   Do not cap
+000031e0: 7475 7265 2073 7464 6f75 7420 2861 6e79  ture stdout (any
+000031f0: 2073 7464 6f75 7420 6f75 7470 7574 2077   stdout output w
+00003200: 696c 6c20 6265 2070 7269 6e74 6564 0a20  ill be printed. 
+00003210: 2020 696d 6d65 6469 6174 656c 7929 205b    immediately) [
+00003220: 4e4f 5345 5f4e 4f43 4150 5455 5245 5d0a  NOSE_NOCAPTURE].
+00003230: 0a2d 2d6e 6f6c 6f67 6361 7074 7572 650a  .--nologcapture.
+00003240: 0a20 2020 4469 7361 626c 6520 6c6f 6767  .   Disable logg
+00003250: 696e 6720 6361 7074 7572 6520 706c 7567  ing capture plug
+00003260: 696e 2e20 4c6f 6767 696e 6720 636f 6e66  in. Logging conf
+00003270: 6967 7572 6174 696f 6e20 7769 6c6c 2062  iguration will b
+00003280: 6520 6c65 6674 0a20 2020 696e 7461 6374  e left.   intact
+00003290: 2e20 5b4e 4f53 455f 4e4f 4c4f 4743 4150  . [NOSE_NOLOGCAP
+000032a0: 5455 5245 5d0a 0a2d 2d6c 6f67 6769 6e67  TURE]..--logging
+000032b0: 2d66 6f72 6d61 743d 464f 524d 4154 0a0a  -format=FORMAT..
+000032c0: 2020 2053 7065 6369 6679 2063 7573 746f     Specify custo
+000032d0: 6d20 666f 726d 6174 2074 6f20 7072 696e  m format to prin
+000032e0: 7420 7374 6174 656d 656e 7473 2e20 5573  t statements. Us
+000032f0: 6573 2074 6865 2073 616d 6520 666f 726d  es the same form
+00003300: 6174 2061 730a 2020 2075 7365 6420 6279  at as.   used by
+00003310: 2073 7461 6e64 6172 6420 6c6f 6767 696e   standard loggin
+00003320: 6720 6861 6e64 6c65 7273 2e20 5b4e 4f53  g handlers. [NOS
+00003330: 455f 4c4f 4746 4f52 4d41 545d 0a0a 2d2d  E_LOGFORMAT]..--
+00003340: 6c6f 6767 696e 672d 6461 7465 666d 743d  logging-datefmt=
+00003350: 464f 524d 4154 0a0a 2020 2053 7065 6369  FORMAT..   Speci
+00003360: 6679 2063 7573 746f 6d20 6461 7465 2f74  fy custom date/t
+00003370: 696d 6520 666f 726d 6174 2074 6f20 7072  ime format to pr
+00003380: 696e 7420 7374 6174 656d 656e 7473 2e20  int statements. 
+00003390: 5573 6573 2074 6865 2073 616d 650a 2020  Uses the same.  
+000033a0: 2066 6f72 6d61 7420 6173 2075 7365 6420   format as used 
+000033b0: 6279 2073 7461 6e64 6172 6420 6c6f 6767  by standard logg
+000033c0: 696e 6720 6861 6e64 6c65 7273 2e20 5b4e  ing handlers. [N
+000033d0: 4f53 455f 4c4f 4744 4154 4546 4d54 5d0a  OSE_LOGDATEFMT].
+000033e0: 0a2d 2d6c 6f67 6769 6e67 2d66 696c 7465  .--logging-filte
+000033f0: 723d 4649 4c54 4552 0a0a 2020 2053 7065  r=FILTER..   Spe
+00003400: 6369 6679 2077 6869 6368 2073 7461 7465  cify which state
+00003410: 6d65 6e74 7320 746f 2066 696c 7465 7220  ments to filter 
+00003420: 696e 2f6f 7574 2e20 4279 2064 6566 6175  in/out. By defau
+00003430: 6c74 2c20 6576 6572 7974 6869 6e67 0a20  lt, everything. 
+00003440: 2020 6973 2063 6170 7475 7265 642e 2049    is captured. I
+00003450: 6620 7468 6520 6f75 7470 7574 2069 7320  f the output is 
+00003460: 746f 6f20 7665 7262 6f73 652c 2075 7365  too verbose, use
+00003470: 2074 6869 7320 6f70 7469 6f6e 2074 6f0a   this option to.
+00003480: 2020 2066 696c 7465 7220 6f75 7420 6e65     filter out ne
+00003490: 6564 6c65 7373 206f 7574 7075 742e 2045  edless output. E
+000034a0: 7861 6d70 6c65 3a20 6669 6c74 6572 3d66  xample: filter=f
+000034b0: 6f6f 2077 696c 6c20 6361 7074 7572 650a  oo will capture.
+000034c0: 2020 2073 7461 7465 6d65 6e74 7320 6973     statements is
+000034d0: 7375 6564 204f 4e4c 5920 746f 2020 666f  sued ONLY to  fo
+000034e0: 6f20 6f72 2066 6f6f 2e77 6861 742e 6576  o or foo.what.ev
+000034f0: 6572 2e73 7562 2062 7574 206e 6f74 2066  er.sub but not f
+00003500: 6f6f 6261 720a 2020 206f 7220 6f74 6865  oobar.   or othe
+00003510: 7220 6c6f 6767 6572 2e20 5370 6563 6966  r logger. Specif
+00003520: 7920 6d75 6c74 6970 6c65 206c 6f67 6765  y multiple logge
+00003530: 7273 2077 6974 6820 636f 6d6d 613a 0a20  rs with comma:. 
+00003540: 2020 6669 6c74 6572 3d66 6f6f 2c62 6172    filter=foo,bar
+00003550: 2c62 617a 2e20 4966 2061 6e79 206c 6f67  ,baz. If any log
+00003560: 6765 7220 6e61 6d65 2069 7320 7072 6566  ger name is pref
+00003570: 6978 6564 2077 6974 6820 6120 6d69 6e75  ixed with a minu
+00003580: 732c 2065 670a 2020 2066 696c 7465 723d  s, eg.   filter=
+00003590: 2d66 6f6f 2c20 6974 2077 696c 6c20 6265  -foo, it will be
+000035a0: 2065 7863 6c75 6465 6420 7261 7468 6572   excluded rather
+000035b0: 2074 6861 6e20 696e 636c 7564 6564 2e20   than included. 
+000035c0: 4465 6661 756c 743a 0a20 2020 6578 636c  Default:.   excl
+000035d0: 7564 6520 6c6f 6767 696e 6720 6d65 7373  ude logging mess
+000035e0: 6167 6573 2066 726f 6d20 6e6f 7365 2069  ages from nose i
+000035f0: 7473 656c 6620 282d 6e6f 7365 292e 205b  tself (-nose). [
+00003600: 4e4f 5345 5f4c 4f47 4649 4c54 4552 5d0a  NOSE_LOGFILTER].
+00003610: 0a2d 2d6c 6f67 6769 6e67 2d63 6c65 6172  .--logging-clear
+00003620: 2d68 616e 646c 6572 730a 0a20 2020 436c  -handlers..   Cl
+00003630: 6561 7220 616c 6c20 6f74 6865 7220 6c6f  ear all other lo
+00003640: 6767 696e 6720 6861 6e64 6c65 7273 0a0a  gging handlers..
+00003650: 2d2d 6c6f 6767 696e 672d 6c65 7665 6c3d  --logging-level=
+00003660: 4445 4641 554c 540a 0a20 2020 5365 7420  DEFAULT..   Set 
+00003670: 7468 6520 6c6f 6720 6c65 7665 6c20 746f  the log level to
+00003680: 2063 6170 7475 7265 0a0a 2d2d 7769 7468   capture..--with
+00003690: 2d63 6f76 6572 6167 650a 0a20 2020 456e  -coverage..   En
+000036a0: 6162 6c65 2070 6c75 6769 6e20 436f 7665  able plugin Cove
+000036b0: 7261 6765 3a20 4163 7469 7661 7465 2061  rage: Activate a
+000036c0: 2063 6f76 6572 6167 6520 7265 706f 7274   coverage report
+000036d0: 2075 7369 6e67 2074 6865 0a20 2020 4e65   using the.   Ne
+000036e0: 6420 4261 7463 6865 6c64 6572 2063 6f76  d Batchelder cov
+000036f0: 6572 6167 6520 6d6f 6475 6c65 2e20 5b4e  erage module. [N
+00003700: 4f53 455f 5749 5448 5f43 4f56 4552 4147  OSE_WITH_COVERAG
+00003710: 455d 0a0a 2d2d 636f 7665 722d 7061 636b  E]..--cover-pack
+00003720: 6167 653d 5041 434b 4147 450a 0a20 2020  age=PACKAGE..   
+00003730: 5265 7374 7269 6374 2063 6f76 6572 6167  Restrict coverag
+00003740: 6520 6f75 7470 7574 2074 6f20 7365 6c65  e output to sele
+00003750: 6374 6564 2070 6163 6b61 6765 7320 5b4e  cted packages [N
+00003760: 4f53 455f 434f 5645 525f 5041 434b 4147  OSE_COVER_PACKAG
+00003770: 455d 0a0a 2d2d 636f 7665 722d 6572 6173  E]..--cover-eras
+00003780: 650a 0a20 2020 4572 6173 6520 7072 6576  e..   Erase prev
+00003790: 696f 7573 6c79 2063 6f6c 6c65 6374 6564  iously collected
+000037a0: 2063 6f76 6572 6167 6520 7374 6174 6973   coverage statis
+000037b0: 7469 6373 2062 6566 6f72 6520 7275 6e0a  tics before run.
+000037c0: 0a2d 2d63 6f76 6572 2d74 6573 7473 0a0a  .--cover-tests..
+000037d0: 2020 2049 6e63 6c75 6465 2074 6573 7420     Include test 
+000037e0: 6d6f 6475 6c65 7320 696e 2063 6f76 6572  modules in cover
+000037f0: 6167 6520 7265 706f 7274 205b 4e4f 5345  age report [NOSE
+00003800: 5f43 4f56 4552 5f54 4553 5453 5d0a 0a2d  _COVER_TESTS]..-
+00003810: 2d63 6f76 6572 2d6d 696e 2d70 6572 6365  -cover-min-perce
+00003820: 6e74 6167 653d 4445 4641 554c 540a 0a20  ntage=DEFAULT.. 
+00003830: 2020 4d69 6e69 6d75 6d20 7065 7263 656e    Minimum percen
+00003840: 7461 6765 206f 6620 636f 7665 7261 6765  tage of coverage
+00003850: 2066 6f72 2074 6573 7473 2074 6f20 7061   for tests to pa
+00003860: 7373 0a20 2020 5b4e 4f53 455f 434f 5645  ss.   [NOSE_COVE
+00003870: 525f 4d49 4e5f 5045 5243 454e 5441 4745  R_MIN_PERCENTAGE
+00003880: 5d0a 0a2d 2d63 6f76 6572 2d69 6e63 6c75  ]..--cover-inclu
+00003890: 7369 7665 0a0a 2020 2049 6e63 6c75 6465  sive..   Include
+000038a0: 2061 6c6c 2070 7974 686f 6e20 6669 6c65   all python file
+000038b0: 7320 756e 6465 7220 776f 726b 696e 6720  s under working 
+000038c0: 6469 7265 6374 6f72 7920 696e 2063 6f76  directory in cov
+000038d0: 6572 6167 650a 2020 2072 6570 6f72 742e  erage.   report.
+000038e0: 2020 5573 6566 756c 2066 6f72 2064 6973    Useful for dis
+000038f0: 636f 7665 7269 6e67 2068 6f6c 6573 2069  covering holes i
+00003900: 6e20 7465 7374 2063 6f76 6572 6167 6520  n test coverage 
+00003910: 6966 206e 6f74 2061 6c6c 0a20 2020 6669  if not all.   fi
+00003920: 6c65 7320 6172 6520 696d 706f 7274 6564  les are imported
+00003930: 2062 7920 7468 6520 7465 7374 2073 7569   by the test sui
+00003940: 7465 2e20 5b4e 4f53 455f 434f 5645 525f  te. [NOSE_COVER_
+00003950: 494e 434c 5553 4956 455d 0a0a 2d2d 636f  INCLUSIVE]..--co
+00003960: 7665 722d 6874 6d6c 0a0a 2020 2050 726f  ver-html..   Pro
+00003970: 6475 6365 2048 544d 4c20 636f 7665 7261  duce HTML covera
+00003980: 6765 2069 6e66 6f72 6d61 7469 6f6e 0a0a  ge information..
+00003990: 2d2d 636f 7665 722d 6874 6d6c 2d64 6972  --cover-html-dir
+000039a0: 3d44 4952 0a0a 2020 2050 726f 6475 6365  =DIR..   Produce
+000039b0: 2048 544d 4c20 636f 7665 7261 6765 2069   HTML coverage i
+000039c0: 6e66 6f72 6d61 7469 6f6e 2069 6e20 6469  nformation in di
+000039d0: 720a 0a2d 2d63 6f76 6572 2d62 7261 6e63  r..--cover-branc
+000039e0: 6865 730a 0a20 2020 496e 636c 7564 6520  hes..   Include 
+000039f0: 6272 616e 6368 2063 6f76 6572 6167 6520  branch coverage 
+00003a00: 696e 2063 6f76 6572 6167 6520 7265 706f  in coverage repo
+00003a10: 7274 205b 4e4f 5345 5f43 4f56 4552 5f42  rt [NOSE_COVER_B
+00003a20: 5241 4e43 4845 535d 0a0a 2d2d 636f 7665  RANCHES]..--cove
+00003a30: 722d 786d 6c0a 0a20 2020 5072 6f64 7563  r-xml..   Produc
+00003a40: 6520 584d 4c20 636f 7665 7261 6765 2069  e XML coverage i
+00003a50: 6e66 6f72 6d61 7469 6f6e 0a0a 2d2d 636f  nformation..--co
+00003a60: 7665 722d 786d 6c2d 6669 6c65 3d46 494c  ver-xml-file=FIL
+00003a70: 450a 0a20 2020 5072 6f64 7563 6520 584d  E..   Produce XM
+00003a80: 4c20 636f 7665 7261 6765 2069 6e66 6f72  L coverage infor
+00003a90: 6d61 7469 6f6e 2069 6e20 6669 6c65 0a0a  mation in file..
+00003aa0: 2d2d 7064 620a 0a20 2020 4472 6f70 2069  --pdb..   Drop i
+00003ab0: 6e74 6f20 6465 6275 6767 6572 206f 6e20  nto debugger on 
+00003ac0: 6661 696c 7572 6573 206f 7220 6572 726f  failures or erro
+00003ad0: 7273 0a0a 2d2d 7064 622d 6661 696c 7572  rs..--pdb-failur
+00003ae0: 6573 0a0a 2020 2044 726f 7020 696e 746f  es..   Drop into
+00003af0: 2064 6562 7567 6765 7220 6f6e 2066 6169   debugger on fai
+00003b00: 6c75 7265 730a 0a2d 2d70 6462 2d65 7272  lures..--pdb-err
+00003b10: 6f72 730a 0a20 2020 4472 6f70 2069 6e74  ors..   Drop int
+00003b20: 6f20 6465 6275 6767 6572 206f 6e20 6572  o debugger on er
+00003b30: 726f 7273 0a0a 2d2d 6e6f 2d64 6570 7265  rors..--no-depre
+00003b40: 6361 7465 640a 0a20 2020 4469 7361 626c  cated..   Disabl
+00003b50: 6520 7370 6563 6961 6c20 6861 6e64 6c69  e special handli
+00003b60: 6e67 206f 6620 4465 7072 6563 6174 6564  ng of Deprecated
+00003b70: 5465 7374 2065 7863 6570 7469 6f6e 732e  Test exceptions.
+00003b80: 0a0a 2d2d 7769 7468 2d64 6f63 7465 7374  ..--with-doctest
+00003b90: 0a0a 2020 2045 6e61 626c 6520 706c 7567  ..   Enable plug
+00003ba0: 696e 2044 6f63 7465 7374 3a20 4163 7469  in Doctest: Acti
+00003bb0: 7661 7465 2064 6f63 7465 7374 2070 6c75  vate doctest plu
+00003bc0: 6769 6e20 746f 2066 696e 6420 616e 6420  gin to find and 
+00003bd0: 7275 6e0a 2020 2064 6f63 7465 7374 7320  run.   doctests 
+00003be0: 696e 206e 6f6e 2d74 6573 7420 6d6f 6475  in non-test modu
+00003bf0: 6c65 732e 205b 4e4f 5345 5f57 4954 485f  les. [NOSE_WITH_
+00003c00: 444f 4354 4553 545d 0a0a 2d2d 646f 6374  DOCTEST]..--doct
+00003c10: 6573 742d 7465 7374 730a 0a20 2020 416c  est-tests..   Al
+00003c20: 736f 206c 6f6f 6b20 666f 7220 646f 6374  so look for doct
+00003c30: 6573 7473 2069 6e20 7465 7374 206d 6f64  ests in test mod
+00003c40: 756c 6573 2e20 4e6f 7465 2074 6861 7420  ules. Note that 
+00003c50: 636c 6173 7365 732c 206d 6574 686f 6473  classes, methods
+00003c60: 0a20 2020 616e 6420 6675 6e63 7469 6f6e  .   and function
+00003c70: 7320 7368 6f75 6c64 2068 6176 6520 6569  s should have ei
+00003c80: 7468 6572 2064 6f63 7465 7374 7320 6f72  ther doctests or
+00003c90: 206e 6f6e 2d64 6f63 7465 7374 2074 6573   non-doctest tes
+00003ca0: 7473 2c20 6e6f 740a 2020 2062 6f74 682e  ts, not.   both.
+00003cb0: 205b 4e4f 5345 5f44 4f43 5445 5354 5f54   [NOSE_DOCTEST_T
+00003cc0: 4553 5453 5d0a 0a2d 2d64 6f63 7465 7374  ESTS]..--doctest
+00003cd0: 2d65 7874 656e 7369 6f6e 3d45 5854 0a0a  -extension=EXT..
+00003ce0: 2020 2041 6c73 6f20 6c6f 6f6b 2066 6f72     Also look for
+00003cf0: 2064 6f63 7465 7374 7320 696e 2066 696c   doctests in fil
+00003d00: 6573 2077 6974 6820 7468 6973 2065 7874  es with this ext
+00003d10: 656e 7369 6f6e 0a20 2020 5b4e 4f53 455f  ension.   [NOSE_
+00003d20: 444f 4354 4553 545f 4558 5445 4e53 494f  DOCTEST_EXTENSIO
+00003d30: 4e5d 0a0a 2d2d 646f 6374 6573 742d 7265  N]..--doctest-re
+00003d40: 7375 6c74 2d76 6172 6961 626c 653d 5641  sult-variable=VA
+00003d50: 520a 0a20 2020 4368 616e 6765 2074 6865  R..   Change the
+00003d60: 2076 6172 6961 626c 6520 6e61 6d65 2073   variable name s
+00003d70: 6574 2074 6f20 7468 6520 7265 7375 6c74  et to the result
+00003d80: 206f 6620 7468 6520 6c61 7374 2069 6e74   of the last int
+00003d90: 6572 7072 6574 6572 0a20 2020 636f 6d6d  erpreter.   comm
+00003da0: 616e 6420 6672 6f6d 2074 6865 2064 6566  and from the def
+00003db0: 6175 6c74 2027 5f27 2e20 4361 6e20 6265  ault '_'. Can be
+00003dc0: 2075 7365 6420 746f 2061 766f 6964 2063   used to avoid c
+00003dd0: 6f6e 666c 6963 7473 2077 6974 680a 2020  onflicts with.  
+00003de0: 2074 6865 205f 2829 2066 756e 6374 696f   the _() functio
+00003df0: 6e20 7573 6564 2066 6f72 2074 6578 7420  n used for text 
+00003e00: 7472 616e 736c 6174 696f 6e2e 0a20 2020  translation..   
+00003e10: 5b4e 4f53 455f 444f 4354 4553 545f 5245  [NOSE_DOCTEST_RE
+00003e20: 5355 4c54 5f56 4152 5d0a 0a2d 2d64 6f63  SULT_VAR]..--doc
+00003e30: 7465 7374 2d66 6978 7475 7265 733d 5355  test-fixtures=SU
+00003e40: 4646 4958 0a0a 2020 2046 696e 6420 6669  FFIX..   Find fi
+00003e50: 7874 7572 6573 2066 6f72 2061 2064 6f63  xtures for a doc
+00003e60: 7465 7374 2066 696c 6520 696e 206d 6f64  test file in mod
+00003e70: 756c 6520 7769 7468 2074 6869 7320 6e61  ule with this na
+00003e80: 6d65 2061 7070 656e 6465 640a 2020 2074  me appended.   t
+00003e90: 6f20 7468 6520 6261 7365 206e 616d 6520  o the base name 
+00003ea0: 6f66 2074 6865 2064 6f63 7465 7374 2066  of the doctest f
+00003eb0: 696c 650a 0a2d 2d64 6f63 7465 7374 2d6f  ile..--doctest-o
+00003ec0: 7074 696f 6e73 3d4f 5054 494f 4e53 0a0a  ptions=OPTIONS..
+00003ed0: 2020 2053 7065 6369 6679 206f 7074 696f     Specify optio
+00003ee0: 6e73 2074 6f20 7061 7373 2074 6f20 646f  ns to pass to do
+00003ef0: 6374 6573 742e 2045 672e 0a20 2020 272b  ctest. Eg..   '+
+00003f00: 454c 4c49 5053 4953 2c2b 4e4f 524d 414c  ELLIPSIS,+NORMAL
+00003f10: 495a 455f 5748 4954 4553 5041 4345 270a  IZE_WHITESPACE'.
+00003f20: 0a2d 2d77 6974 682d 6973 6f6c 6174 696f  .--with-isolatio
+00003f30: 6e0a 0a20 2020 456e 6162 6c65 2070 6c75  n..   Enable plu
+00003f40: 6769 6e20 4973 6f6c 6174 696f 6e50 6c75  gin IsolationPlu
+00003f50: 6769 6e3a 2041 6374 6976 6174 6520 7468  gin: Activate th
+00003f60: 6520 6973 6f6c 6174 696f 6e20 706c 7567  e isolation plug
+00003f70: 696e 2074 6f0a 2020 2069 736f 6c61 7465  in to.   isolate
+00003f80: 2063 6861 6e67 6573 2074 6f20 6578 7465   changes to exte
+00003f90: 726e 616c 206d 6f64 756c 6573 2074 6f20  rnal modules to 
+00003fa0: 6120 7369 6e67 6c65 2074 6573 7420 6d6f  a single test mo
+00003fb0: 6475 6c65 206f 720a 2020 2070 6163 6b61  dule or.   packa
+00003fc0: 6765 2e20 5468 6520 6973 6f6c 6174 696f  ge. The isolatio
+00003fd0: 6e20 706c 7567 696e 2072 6573 6574 7320  n plugin resets 
+00003fe0: 7468 6520 636f 6e74 656e 7473 206f 6620  the contents of 
+00003ff0: 7379 732e 6d6f 6475 6c65 730a 2020 2061  sys.modules.   a
+00004000: 6674 6572 2065 6163 6820 7465 7374 206d  fter each test m
+00004010: 6f64 756c 6520 6f72 2070 6163 6b61 6765  odule or package
+00004020: 2072 756e 7320 746f 2069 7473 2073 7461   runs to its sta
+00004030: 7465 2062 6566 6f72 6520 7468 650a 2020  te before the.  
+00004040: 2074 6573 742e 2050 4c45 4153 4520 4e4f   test. PLEASE NO
+00004050: 5445 2074 6861 7420 7468 6973 2070 6c75  TE that this plu
+00004060: 6769 6e20 7368 6f75 6c64 206e 6f74 2062  gin should not b
+00004070: 6520 7573 6564 2077 6974 6820 7468 650a  e used with the.
+00004080: 2020 2063 6f76 6572 6167 6520 706c 7567     coverage plug
+00004090: 696e 2c20 6f72 2069 6e20 616e 7920 6f74  in, or in any ot
+000040a0: 6865 7220 6361 7365 2077 6865 7265 206d  her case where m
+000040b0: 6f64 756c 6520 7265 6c6f 6164 696e 6720  odule reloading 
+000040c0: 6d61 790a 2020 2070 726f 6475 6365 2075  may.   produce u
+000040d0: 6e64 6573 6972 6162 6c65 2073 6964 652d  ndesirable side-
+000040e0: 6566 6665 6374 732e 205b 4e4f 5345 5f57  effects. [NOSE_W
+000040f0: 4954 485f 4953 4f4c 4154 494f 4e5d 0a0a  ITH_ISOLATION]..
+00004100: 2d64 2c20 2d2d 6465 7461 696c 6564 2d65  -d, --detailed-e
+00004110: 7272 6f72 732c 202d 2d66 6169 6c75 7265  rrors, --failure
+00004120: 2d64 6574 6169 6c0a 0a20 2020 4164 6420  -detail..   Add 
+00004130: 6465 7461 696c 2074 6f20 6572 726f 7220  detail to error 
+00004140: 6f75 7470 7574 2062 7920 6174 7465 6d70  output by attemp
+00004150: 7469 6e67 2074 6f20 6576 616c 7561 7465  ting to evaluate
+00004160: 2066 6169 6c65 6420 6173 7365 7274 730a   failed asserts.
+00004170: 2020 205b 4e4f 5345 5f44 4554 4149 4c45     [NOSE_DETAILE
+00004180: 445f 4552 524f 5253 5d0a 0a2d 2d6e 6f2d  D_ERRORS]..--no-
+00004190: 736b 6970 0a0a 2020 2044 6973 6162 6c65  skip..   Disable
+000041a0: 2073 7065 6369 616c 2068 616e 646c 696e   special handlin
+000041b0: 6720 6f66 2053 6b69 7054 6573 7420 6578  g of SkipTest ex
+000041c0: 6365 7074 696f 6e73 2e0a 0a2d 2d77 6974  ceptions...--wit
+000041d0: 682d 6964 0a0a 2020 2045 6e61 626c 6520  h-id..   Enable 
+000041e0: 706c 7567 696e 2054 6573 7449 643a 2041  plugin TestId: A
+000041f0: 6374 6976 6174 6520 746f 2061 6464 2061  ctivate to add a
+00004200: 2074 6573 7420 6964 2028 6c69 6b65 2023   test id (like #
+00004210: 3129 2074 6f20 6561 6368 0a20 2020 7465  1) to each.   te
+00004220: 7374 206e 616d 6520 6f75 7470 7574 2e20  st name output. 
+00004230: 4163 7469 7661 7465 2077 6974 6820 2d2d  Activate with --
+00004240: 6661 696c 6564 2074 6f20 7265 7275 6e20  failed to rerun 
+00004250: 6661 696c 696e 6720 7465 7374 730a 2020  failing tests.  
+00004260: 206f 6e6c 792e 205b 4e4f 5345 5f57 4954   only. [NOSE_WIT
+00004270: 485f 4944 5d0a 0a2d 2d69 642d 6669 6c65  H_ID]..--id-file
+00004280: 3d46 494c 450a 0a20 2020 5374 6f72 6520  =FILE..   Store 
+00004290: 7465 7374 2069 6473 2066 6f75 6e64 2069  test ids found i
+000042a0: 6e20 7465 7374 2072 756e 7320 696e 2074  n test runs in t
+000042b0: 6869 7320 6669 6c65 2e20 4465 6661 756c  his file. Defaul
+000042c0: 7420 6973 2074 6865 2066 696c 650a 2020  t is the file.  
+000042d0: 202e 6e6f 7365 6964 7320 696e 2074 6865   .noseids in the
+000042e0: 2077 6f72 6b69 6e67 2064 6972 6563 746f   working directo
+000042f0: 7279 2e0a 0a2d 2d66 6169 6c65 640a 0a20  ry...--failed.. 
+00004300: 2020 5275 6e20 7468 6520 7465 7374 7320    Run the tests 
+00004310: 7468 6174 2066 6169 6c65 6420 696e 2074  that failed in t
+00004320: 6865 206c 6173 7420 7465 7374 2072 756e  he last test run
+00004330: 2e0a 0a2d 2d70 726f 6365 7373 6573 3d4e  ...--processes=N
+00004340: 554d 0a0a 2020 2053 7072 6561 6420 7465  UM..   Spread te
+00004350: 7374 2072 756e 2061 6d6f 6e67 2074 6869  st run among thi
+00004360: 7320 6d61 6e79 2070 726f 6365 7373 6573  s many processes
+00004370: 2e20 5365 7420 6120 6e75 6d62 6572 2065  . Set a number e
+00004380: 7175 616c 2074 6f0a 2020 2074 6865 206e  qual to.   the n
+00004390: 756d 6265 7220 6f66 2070 726f 6365 7373  umber of process
+000043a0: 6f72 7320 6f72 2063 6f72 6573 2069 6e20  ors or cores in 
+000043b0: 796f 7572 206d 6163 6869 6e65 2066 6f72  your machine for
+000043c0: 2062 6573 7420 7265 7375 6c74 732e 0a20   best results.. 
+000043d0: 2020 5061 7373 2061 206e 6567 6174 6976    Pass a negativ
+000043e0: 6520 6e75 6d62 6572 2074 6f20 6861 7665  e number to have
+000043f0: 2074 6865 206e 756d 6265 7220 6f66 2070   the number of p
+00004400: 726f 6365 7373 6573 0a20 2020 6175 746f  rocesses.   auto
+00004410: 6d61 7469 6361 6c6c 7920 7365 7420 746f  matically set to
+00004420: 2074 6865 206e 756d 6265 7220 6f66 2063   the number of c
+00004430: 6f72 6573 2e20 5061 7373 696e 6720 3020  ores. Passing 0 
+00004440: 6d65 616e 7320 746f 0a20 2020 6469 7361  means to.   disa
+00004450: 626c 6520 7061 7261 6c6c 656c 2074 6573  ble parallel tes
+00004460: 7469 6e67 2e20 4465 6661 756c 7420 6973  ting. Default is
+00004470: 2030 2075 6e6c 6573 7320 4e4f 5345 5f50   0 unless NOSE_P
+00004480: 524f 4345 5353 4553 2069 730a 2020 2073  ROCESSES is.   s
+00004490: 6574 2e20 5b4e 4f53 455f 5052 4f43 4553  et. [NOSE_PROCES
+000044a0: 5345 535d 0a0a 2d2d 7072 6f63 6573 732d  SES]..--process-
+000044b0: 7469 6d65 6f75 743d 5345 434f 4e44 530a  timeout=SECONDS.
+000044c0: 0a20 2020 5365 7420 7469 6d65 6f75 7420  .   Set timeout 
+000044d0: 666f 7220 7265 7475 726e 206f 6620 7265  for return of re
+000044e0: 7375 6c74 7320 6672 6f6d 2065 6163 6820  sults from each 
+000044f0: 7465 7374 2072 756e 6e65 7220 7072 6f63  test runner proc
+00004500: 6573 732e 0a20 2020 4465 6661 756c 7420  ess..   Default 
+00004510: 6973 2031 302e 205b 4e4f 5345 5f50 524f  is 10. [NOSE_PRO
+00004520: 4345 5353 5f54 494d 454f 5554 5d0a 0a2d  CESS_TIMEOUT]..-
+00004530: 2d70 726f 6365 7373 2d72 6573 7461 7274  -process-restart
+00004540: 776f 726b 6572 0a0a 2020 2049 6620 7365  worker..   If se
+00004550: 742c 2077 696c 6c20 7265 7374 6172 7420  t, will restart 
+00004560: 6561 6368 2077 6f72 6b65 7220 7072 6f63  each worker proc
+00004570: 6573 7320 6f6e 6365 2074 6865 6972 2074  ess once their t
+00004580: 6573 7473 2061 7265 2064 6f6e 652c 0a20  ests are done,. 
+00004590: 2020 7468 6973 2068 656c 7073 2063 6f6e    this helps con
+000045a0: 7472 6f6c 206d 656d 6f72 7920 6c65 616b  trol memory leak
+000045b0: 7320 6672 6f6d 206b 696c 6c69 6e67 2074  s from killing t
+000045c0: 6865 2073 7973 7465 6d2e 0a20 2020 5b4e  he system..   [N
+000045d0: 4f53 455f 5052 4f43 4553 535f 5245 5354  OSE_PROCESS_REST
+000045e0: 4152 5457 4f52 4b45 525d 0a0a 2d2d 7769  ARTWORKER]..--wi
+000045f0: 7468 2d78 756e 6974 0a0a 2020 2045 6e61  th-xunit..   Ena
+00004600: 626c 6520 706c 7567 696e 2058 756e 6974  ble plugin Xunit
+00004610: 3a20 5468 6973 2070 6c75 6769 6e20 7072  : This plugin pr
+00004620: 6f76 6964 6573 2074 6573 7420 7265 7375  ovides test resu
+00004630: 6c74 7320 696e 2074 6865 0a20 2020 7374  lts in the.   st
+00004640: 616e 6461 7264 2058 556e 6974 2058 4d4c  andard XUnit XML
+00004650: 2066 6f72 6d61 742e 205b 4e4f 5345 5f57   format. [NOSE_W
+00004660: 4954 485f 5855 4e49 545d 0a0a 2d2d 7875  ITH_XUNIT]..--xu
+00004670: 6e69 742d 6669 6c65 3d46 494c 450a 0a20  nit-file=FILE.. 
+00004680: 2020 5061 7468 2074 6f20 786d 6c20 6669    Path to xml fi
+00004690: 6c65 2074 6f20 7374 6f72 6520 7468 6520  le to store the 
+000046a0: 7875 6e69 7420 7265 706f 7274 2069 6e2e  xunit report in.
+000046b0: 2044 6566 6175 6c74 2069 730a 2020 206e   Default is.   n
+000046c0: 6f73 6574 6573 7473 2e78 6d6c 2069 6e20  osetests.xml in 
+000046d0: 7468 6520 776f 726b 696e 6720 6469 7265  the working dire
+000046e0: 6374 6f72 7920 5b4e 4f53 455f 5855 4e49  ctory [NOSE_XUNI
+000046f0: 545f 4649 4c45 5d0a 0a2d 2d78 756e 6974  T_FILE]..--xunit
+00004700: 2d74 6573 7473 7569 7465 2d6e 616d 653d  -testsuite-name=
+00004710: 5041 434b 4147 450a 0a20 2020 4e61 6d65  PACKAGE..   Name
+00004720: 206f 6620 7468 6520 7465 7374 7375 6974   of the testsuit
+00004730: 6520 696e 2074 6865 2078 756e 6974 2078  e in the xunit x
+00004740: 6d6c 2c20 6765 6e65 7261 7465 6420 6279  ml, generated by
+00004750: 2070 6c75 6769 6e2e 0a20 2020 4465 6661   plugin..   Defa
+00004760: 756c 7420 7465 7374 2073 7569 7465 206e  ult test suite n
+00004770: 616d 6520 6973 206e 6f73 6574 6573 7473  ame is nosetests
+00004780: 2e0a 0a2d 2d61 6c6c 2d6d 6f64 756c 6573  ...--all-modules
+00004790: 0a0a 2020 2045 6e61 626c 6520 706c 7567  ..   Enable plug
+000047a0: 696e 2041 6c6c 4d6f 6475 6c65 733a 2043  in AllModules: C
+000047b0: 6f6c 6c65 6374 2074 6573 7473 2066 726f  ollect tests fro
+000047c0: 6d20 616c 6c20 7079 7468 6f6e 206d 6f64  m all python mod
+000047d0: 756c 6573 2e0a 2020 205b 4e4f 5345 5f41  ules..   [NOSE_A
+000047e0: 4c4c 5f4d 4f44 554c 4553 5d0a 0a2d 2d63  LL_MODULES]..--c
+000047f0: 6f2c 202d 2d63 6f6c 6c65 6374 2d6f 6e6c  o, --collect-onl
+00004800: 790a 0a20 2020 456e 6162 6c65 2063 6f6c  y..   Enable col
+00004810: 6c65 6374 2d6f 6e6c 793a 2043 6f6c 6c65  lect-only: Colle
+00004820: 6374 2061 6e64 206f 7574 7075 7420 7465  ct and output te
+00004830: 7374 206e 616d 6573 206f 6e6c 792c 0a20  st names only,. 
+00004840: 2020 6275 7420 646f 206e 6f74 2072 756e    but do not run
+00004850: 2061 6e79 2074 6573 7473 2e20 5b43 4f4c   any tests. [COL
+00004860: 4c45 4354 5f4f 4e4c 595d 0a60 6060 0a    LECT_ONLY].```.
```

### Comparing `pynose-1.4.5/pynose.egg-info/SOURCES.txt` & `pynose-1.4.6/pynose.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -53,8 +53,9 @@
 nose/sphinx/pluginopts.py
 nose/tools/__init__.py
 nose/tools/nontrivial.py
 nose/tools/trivial.py
 pynose.egg-info/PKG-INFO
 pynose.egg-info/SOURCES.txt
 pynose.egg-info/dependency_links.txt
+pynose.egg-info/entry_points.txt
 pynose.egg-info/top_level.txt
```

### Comparing `pynose-1.4.5/setup.py` & `pynose-1.4.6/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -26,32 +26,34 @@
 
 if sys.argv[-1] == "publish":
     reply = None
     input_method = input
     confirm_text = ">>> Confirm release PUBLISH to PyPI? (yes/no): "
     reply = str(input_method(confirm_text)).lower().strip()
     if reply == "yes":
+        if sys.version_info < (3, 9):
+            print("\nERROR! Publishing to PyPI requires Python>=3.9")
+            sys.exit()
         print("\n*** Checking code health with flake8:\n")
-        if sys.version_info >= (3, 9):
-            os.system("python -m pip install 'flake8==6.0.0'")
-        else:
-            os.system("python -m pip install 'flake8==5.0.4'")
+        os.system("python -m pip install 'flake8==6.0.0'")
         flake8_status = os.system("flake8 --exclude=recordings,temp")
         if flake8_status != 0:
-            print("\nWARNING! Fix flake8 issues before publishing to PyPI!\n")
+            print("\nERROR! Fix flake8 issues before publishing to PyPI!\n")
             sys.exit()
         else:
             print("*** No flake8 issues detected. Continuing...")
         print("\n*** Removing existing distribution packages: ***\n")
         os.system("rm -f dist/*.egg; rm -f dist/*.tar.gz; rm -f dist/*.whl")
         os.system("rm -rf build/bdist.*; rm -rf build/lib")
         print("\n*** Installing build: *** (Required for PyPI uploads)\n")
         os.system("python -m pip install --upgrade 'build>=0.10.0'")
         print("\n*** Installing pkginfo: *** (Required for PyPI uploads)\n")
         os.system("python -m pip install --upgrade 'pkginfo>=1.9.6'")
+        print("\n*** Installing readme-renderer: *** (For PyPI uploads)\n")
+        os.system("python -m pip install --upgrade 'readme-renderer>=40.0'")
         print("\n*** Installing twine: *** (Required for PyPI uploads)\n")
         os.system("python -m pip install --upgrade 'twine>=4.0.2'")
         print("\n*** Installing tqdm: *** (Required for PyPI uploads)\n")
         os.system("python -m pip install --upgrade tqdm")
         print("\n*** Rebuilding distribution packages: ***\n")
         os.system("python -m build")  # Create new tar/wheel
         print("\n*** Publishing The Release to PyPI: ***\n")
@@ -59,15 +61,20 @@
         print("\n*** The Release was PUBLISHED SUCCESSFULLY to PyPI! :) ***\n")
     else:
         print("\n>>> The Release was NOT PUBLISHED to PyPI! <<<\n")
     sys.exit()
 
 addl_args = dict(
     packages=["nose", "nose.plugins", "nose.sphinx", "nose.tools"],
-    scripts=["bin/nosetests", "bin/pynose"],
+    entry_points={
+        "console_scripts": [
+            "nosetests = nose.core:run_exit",
+            "pynose = nose.core:run_exit",
+        ]
+    },
 )
 
 setup(
     name="pynose",
     version=VERSION,
     author="Michael Mintz",
     author_email="mdmintz@gmail.com",
```

