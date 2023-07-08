# Comparing `tmp/edp_redy_py-0.1.1.tar.gz` & `tmp/edp_redy_py-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edp_redy_py-0.1.1.tar", last modified: Sat Jul  8 17:34:54 2023, max compression
+gzip compressed data, was "edp_redy_py-0.1.3.tar", last modified: Sat Jul  8 17:42:48 2023, max compression
```

## Comparing `edp_redy_py-0.1.1.tar` & `edp_redy_py-0.1.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-07-08 17:34:54.654149 edp_redy_py-0.1.1/
--rw-rw-rw-   0        0        0    11556 2023-07-08 16:56:32.000000 edp_redy_py-0.1.1/LICENSE
--rw-rw-rw-   0        0        0      283 2023-07-08 17:34:54.654149 edp_redy_py-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0       22 2023-07-08 17:07:46.000000 edp_redy_py-0.1.1/README.md
--rw-rw-rw-   0        0        0      111 2023-07-08 17:34:54.655611 edp_redy_py-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      375 2023-07-08 17:34:51.000000 edp_redy_py-0.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-08 17:34:54.615697 edp_redy_py-0.1.1/src/
-drwxrwxrwx   0        0        0        0 2023-07-08 17:34:54.640292 edp_redy_py-0.1.1/src/edp_redy/
--rw-rw-rw-   0        0        0        0 2023-07-08 15:14:43.000000 edp_redy_py-0.1.1/src/edp_redy/__init__.py
--rw-rw-rw-   0        0        0     1941 2023-07-08 17:33:35.000000 edp_redy_py-0.1.1/src/edp_redy/authenticate.py
--rw-rw-rw-   0        0        0      204 2023-07-08 16:51:43.000000 edp_redy_py-0.1.1/src/edp_redy/consts.py
--rw-rw-rw-   0        0        0     2570 2023-07-08 17:15:29.000000 edp_redy_py-0.1.1/src/edp_redy/edp_mqtt.py
-drwxrwxrwx   0        0        0        0 2023-07-08 17:34:54.641339 edp_redy_py-0.1.1/src/edp_redy/equipment/
--rw-rw-rw-   0        0        0        0 2023-07-08 16:25:40.000000 edp_redy_py-0.1.1/src/edp_redy/equipment/__init__.py
--rw-rw-rw-   0        0        0     7618 2023-07-08 17:33:47.000000 edp_redy_py-0.1.1/src/edp_redy/equipment/equipment.py
--rw-rw-rw-   0        0        0     1003 2023-07-08 16:51:43.000000 edp_redy_py-0.1.1/src/edp_redy/helpers.py
--rw-rw-rw-   0        0        0      594 2023-07-08 17:33:28.000000 edp_redy_py-0.1.1/src/edp_redy/redy.py
-drwxrwxrwx   0        0        0        0 2023-07-08 17:34:54.642922 edp_redy_py-0.1.1/src/edp_redy/usermanagement/
--rw-rw-rw-   0        0        0        0 2023-07-08 15:24:38.000000 edp_redy_py-0.1.1/src/edp_redy/usermanagement/__init__.py
--rw-rw-rw-   0        0        0     2296 2023-07-08 17:33:51.000000 edp_redy_py-0.1.1/src/edp_redy/usermanagement/usermanagement.py
-drwxrwxrwx   0        0        0        0 2023-07-08 17:34:54.653101 edp_redy_py-0.1.1/src/edp_redy_py.egg-info/
--rw-rw-rw-   0        0        0      283 2023-07-08 17:34:54.000000 edp_redy_py-0.1.1/src/edp_redy_py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      496 2023-07-08 17:34:54.000000 edp_redy_py-0.1.1/src/edp_redy_py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-08 17:34:54.000000 edp_redy_py-0.1.1/src/edp_redy_py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-07-08 17:34:54.000000 edp_redy_py-0.1.1/src/edp_redy_py.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-08 17:42:48.066316 edp_redy_py-0.1.3/
+-rw-rw-rw-   0        0        0    11556 2023-07-08 16:56:32.000000 edp_redy_py-0.1.3/LICENSE
+-rw-rw-rw-   0        0        0      283 2023-07-08 17:42:48.066316 edp_redy_py-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0       22 2023-07-08 17:07:46.000000 edp_redy_py-0.1.3/README.md
+-rw-rw-rw-   0        0        0      111 2023-07-08 17:42:48.067890 edp_redy_py-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      375 2023-07-08 17:42:44.000000 edp_redy_py-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-08 17:42:48.016451 edp_redy_py-0.1.3/src/
+drwxrwxrwx   0        0        0        0 2023-07-08 17:42:48.028855 edp_redy_py-0.1.3/src/edp_redy/
+-rw-rw-rw-   0        0        0        0 2023-07-08 15:14:43.000000 edp_redy_py-0.1.3/src/edp_redy/__init__.py
+-rw-rw-rw-   0        0        0     1941 2023-07-08 17:33:35.000000 edp_redy_py-0.1.3/src/edp_redy/authenticate.py
+-rw-rw-rw-   0        0        0      204 2023-07-08 16:51:43.000000 edp_redy_py-0.1.3/src/edp_redy/consts.py
+-rw-rw-rw-   0        0        0     2570 2023-07-08 17:15:29.000000 edp_redy_py-0.1.3/src/edp_redy/edp_mqtt.py
+drwxrwxrwx   0        0        0        0 2023-07-08 17:42:48.051325 edp_redy_py-0.1.3/src/edp_redy/equipment/
+-rw-rw-rw-   0        0        0        0 2023-07-08 16:25:40.000000 edp_redy_py-0.1.3/src/edp_redy/equipment/__init__.py
+-rw-rw-rw-   0        0        0     7618 2023-07-08 17:33:47.000000 edp_redy_py-0.1.3/src/edp_redy/equipment/equipment.py
+-rw-rw-rw-   0        0        0     1003 2023-07-08 16:51:43.000000 edp_redy_py-0.1.3/src/edp_redy/helpers.py
+-rw-rw-rw-   0        0        0      721 2023-07-08 17:37:45.000000 edp_redy_py-0.1.3/src/edp_redy/redy.py
+drwxrwxrwx   0        0        0        0 2023-07-08 17:42:48.053449 edp_redy_py-0.1.3/src/edp_redy/usermanagement/
+-rw-rw-rw-   0        0        0        0 2023-07-08 15:24:38.000000 edp_redy_py-0.1.3/src/edp_redy/usermanagement/__init__.py
+-rw-rw-rw-   0        0        0     2296 2023-07-08 17:33:51.000000 edp_redy_py-0.1.3/src/edp_redy/usermanagement/usermanagement.py
+drwxrwxrwx   0        0        0        0 2023-07-08 17:42:48.064729 edp_redy_py-0.1.3/src/edp_redy_py.egg-info/
+-rw-rw-rw-   0        0        0      283 2023-07-08 17:42:47.000000 edp_redy_py-0.1.3/src/edp_redy_py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      496 2023-07-08 17:42:47.000000 edp_redy_py-0.1.3/src/edp_redy_py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-08 17:42:47.000000 edp_redy_py-0.1.3/src/edp_redy_py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-07-08 17:42:47.000000 edp_redy_py-0.1.3/src/edp_redy_py.egg-info/top_level.txt
```

### Comparing `edp_redy_py-0.1.1/LICENSE` & `edp_redy_py-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `edp_redy_py-0.1.1/src/edp_redy/authenticate.py` & `edp_redy_py-0.1.3/src/edp_redy/authenticate.py`

 * *Files identical despite different names*

### Comparing `edp_redy_py-0.1.1/src/edp_redy/edp_mqtt.py` & `edp_redy_py-0.1.3/src/edp_redy/edp_mqtt.py`

 * *Files identical despite different names*

### Comparing `edp_redy_py-0.1.1/src/edp_redy/equipment/equipment.py` & `edp_redy_py-0.1.3/src/edp_redy/equipment/equipment.py`

 * *Files identical despite different names*

### Comparing `edp_redy_py-0.1.1/src/edp_redy/helpers.py` & `edp_redy_py-0.1.3/src/edp_redy/helpers.py`

 * *Files identical despite different names*

### Comparing `edp_redy_py-0.1.1/src/edp_redy/usermanagement/usermanagement.py` & `edp_redy_py-0.1.3/src/edp_redy/usermanagement/usermanagement.py`

 * *Files identical despite different names*

