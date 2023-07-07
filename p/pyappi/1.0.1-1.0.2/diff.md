# Comparing `tmp/pyappi-1.0.1.tar.gz` & `tmp/pyappi-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyappi-1.0.1.tar", last modified: Mon May 22 20:19:06 2023, max compression
+gzip compressed data, was "pyappi-1.0.2.tar", last modified: Fri Jul  7 23:18:40 2023, max compression
```

## Comparing `pyappi-1.0.1.tar` & `pyappi-1.0.2.tar`

### file list

```diff
@@ -1,18 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-05-22 20:19:06.854685 pyappi-1.0.1/
--rw-rw-rw-   0        0        0       20 2023-05-22 20:01:33.000000 pyappi-1.0.1/LICENSE
--rw-rw-rw-   0        0        0      208 2023-05-22 20:19:06.854685 pyappi-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-05-22 15:41:28.000000 pyappi-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-22 20:19:06.844644 pyappi-1.0.1/pyappi/
--rw-rw-rw-   0        0        0        0 2023-05-22 15:40:49.000000 pyappi-1.0.1/pyappi/__init__.py
--rw-rw-rw-   0        0        0     1650 2023-05-22 18:08:49.000000 pyappi-1.0.1/pyappi/core.py
--rw-rw-rw-   0        0        0      381 2023-05-22 17:16:18.000000 pyappi-1.0.1/pyappi/main.py
-drwxrwxrwx   0        0        0        0 2023-05-22 20:19:06.850681 pyappi-1.0.1/pyappi.egg-info/
--rw-rw-rw-   0        0        0      208 2023-05-22 20:19:06.000000 pyappi-1.0.1/pyappi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      232 2023-05-22 20:19:06.000000 pyappi-1.0.1/pyappi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-22 20:19:06.000000 pyappi-1.0.1/pyappi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-05-22 20:19:06.000000 pyappi-1.0.1/pyappi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-22 20:19:06.855941 pyappi-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      354 2023-05-22 20:17:28.000000 pyappi-1.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-22 20:19:06.852685 pyappi-1.0.1/tests/
--rw-rw-rw-   0        0        0        0 2023-05-22 15:40:49.000000 pyappi-1.0.1/tests/__init__.py
--rw-rw-rw-   0        0        0        0 2023-05-22 19:43:33.000000 pyappi-1.0.1/tests/test_core.py
+drwxrwxrwx   0        0        0        0 2023-07-07 23:18:40.157883 pyappi-1.0.2/
+-rw-rw-rw-   0        0        0       20 2023-05-22 20:01:33.000000 pyappi-1.0.2/LICENSE
+-rw-rw-rw-   0        0        0      324 2023-07-07 23:18:40.156883 pyappi-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      112 2023-05-22 21:24:09.000000 pyappi-1.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-07 23:18:40.131600 pyappi-1.0.2/pyappi/
+-rw-rw-rw-   0        0        0        0 2023-06-30 22:18:56.000000 pyappi-1.0.2/pyappi/__init__.py
+-rw-rw-rw-   0        0        0      509 2023-07-03 23:24:25.000000 pyappi-1.0.2/pyappi/api_base.py
+-rw-rw-rw-   0        0        0      393 2023-07-07 20:33:20.000000 pyappi-1.0.2/pyappi/endpoints.py
+-rw-rw-rw-   0        0        0      265 2023-07-03 23:19:17.000000 pyappi-1.0.2/pyappi/main.py
+drwxrwxrwx   0        0        0        0 2023-07-07 23:18:40.150372 pyappi-1.0.2/pyappi.egg-info/
+-rw-rw-rw-   0        0        0      324 2023-07-07 23:18:40.000000 pyappi-1.0.2/pyappi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      274 2023-07-07 23:18:40.000000 pyappi-1.0.2/pyappi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-07 23:18:40.000000 pyappi-1.0.2/pyappi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-07-07 23:18:40.000000 pyappi-1.0.2/pyappi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-07 23:18:40.157883 pyappi-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      354 2023-07-07 23:13:16.000000 pyappi-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-07 23:18:40.154548 pyappi-1.0.2/tests/
+-rw-rw-rw-   0        0        0        0 2023-05-22 15:40:49.000000 pyappi-1.0.2/tests/__init__.py
+-rw-rw-rw-   0        0        0     1506 2023-06-13 18:44:20.000000 pyappi-1.0.2/tests/test_core.py
+-rw-rw-rw-   0        0        0     1051 2023-06-13 18:55:48.000000 pyappi-1.0.2/tests/test_log.py
```

