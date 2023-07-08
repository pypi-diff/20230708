# Comparing `tmp/edp_redy_py-0.1.4.tar.gz` & `tmp/edp_redy_py-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edp_redy_py-0.1.4.tar", last modified: Sat Jul  8 17:49:55 2023, max compression
+gzip compressed data, was "edp_redy_py-0.1.5.tar", last modified: Sat Jul  8 17:55:23 2023, max compression
```

## Comparing `edp_redy_py-0.1.4.tar` & `edp_redy_py-0.1.5.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-07-08 17:49:55.205275 edp_redy_py-0.1.4/
--rw-rw-rw-   0        0        0    11556 2023-07-08 16:56:32.000000 edp_redy_py-0.1.4/LICENSE
--rw-rw-rw-   0        0        0      283 2023-07-08 17:49:55.205803 edp_redy_py-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0       22 2023-07-08 17:07:46.000000 edp_redy_py-0.1.4/README.md
--rw-rw-rw-   0        0        0      111 2023-07-08 17:49:55.207641 edp_redy_py-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0      375 2023-07-08 17:49:25.000000 edp_redy_py-0.1.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-08 17:49:55.177699 edp_redy_py-0.1.4/src/
-drwxrwxrwx   0        0        0        0 2023-07-08 17:49:55.188800 edp_redy_py-0.1.4/src/edp_redy/
--rw-rw-rw-   0        0        0        0 2023-07-08 15:14:43.000000 edp_redy_py-0.1.4/src/edp_redy/__init__.py
--rw-rw-rw-   0        0        0     1941 2023-07-08 17:33:35.000000 edp_redy_py-0.1.4/src/edp_redy/authenticate.py
--rw-rw-rw-   0        0        0      204 2023-07-08 16:51:43.000000 edp_redy_py-0.1.4/src/edp_redy/consts.py
--rw-rw-rw-   0        0        0     2573 2023-07-08 17:49:03.000000 edp_redy_py-0.1.4/src/edp_redy/edp_mqtt.py
-drwxrwxrwx   0        0        0        0 2023-07-08 17:49:55.190921 edp_redy_py-0.1.4/src/edp_redy/equipment/
--rw-rw-rw-   0        0        0        0 2023-07-08 16:25:40.000000 edp_redy_py-0.1.4/src/edp_redy/equipment/__init__.py
--rw-rw-rw-   0        0        0     7618 2023-07-08 17:33:47.000000 edp_redy_py-0.1.4/src/edp_redy/equipment/equipment.py
--rw-rw-rw-   0        0        0     1003 2023-07-08 16:51:43.000000 edp_redy_py-0.1.4/src/edp_redy/helpers.py
--rw-rw-rw-   0        0        0      721 2023-07-08 17:37:45.000000 edp_redy_py-0.1.4/src/edp_redy/redy.py
-drwxrwxrwx   0        0        0        0 2023-07-08 17:49:55.193166 edp_redy_py-0.1.4/src/edp_redy/usermanagement/
--rw-rw-rw-   0        0        0        0 2023-07-08 15:24:38.000000 edp_redy_py-0.1.4/src/edp_redy/usermanagement/__init__.py
--rw-rw-rw-   0        0        0     2296 2023-07-08 17:33:51.000000 edp_redy_py-0.1.4/src/edp_redy/usermanagement/usermanagement.py
-drwxrwxrwx   0        0        0        0 2023-07-08 17:49:55.204749 edp_redy_py-0.1.4/src/edp_redy_py.egg-info/
--rw-rw-rw-   0        0        0      283 2023-07-08 17:49:55.000000 edp_redy_py-0.1.4/src/edp_redy_py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      496 2023-07-08 17:49:55.000000 edp_redy_py-0.1.4/src/edp_redy_py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-08 17:49:55.000000 edp_redy_py-0.1.4/src/edp_redy_py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-07-08 17:49:55.000000 edp_redy_py-0.1.4/src/edp_redy_py.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-08 17:55:23.132063 edp_redy_py-0.1.5/
+-rw-rw-rw-   0        0        0    11556 2023-07-08 16:56:32.000000 edp_redy_py-0.1.5/LICENSE
+-rw-rw-rw-   0        0        0      283 2023-07-08 17:55:23.132603 edp_redy_py-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0       22 2023-07-08 17:07:46.000000 edp_redy_py-0.1.5/README.md
+-rw-rw-rw-   0        0        0      111 2023-07-08 17:55:23.134177 edp_redy_py-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0      375 2023-07-08 17:54:21.000000 edp_redy_py-0.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-08 17:55:23.109630 edp_redy_py-0.1.5/src/
+drwxrwxrwx   0        0        0        0 2023-07-08 17:55:23.118243 edp_redy_py-0.1.5/src/edp_redy/
+-rw-rw-rw-   0        0        0        0 2023-07-08 15:14:43.000000 edp_redy_py-0.1.5/src/edp_redy/__init__.py
+-rw-rw-rw-   0        0        0     1953 2023-07-08 17:53:36.000000 edp_redy_py-0.1.5/src/edp_redy/authenticate.py
+-rw-rw-rw-   0        0        0      204 2023-07-08 16:51:43.000000 edp_redy_py-0.1.5/src/edp_redy/consts.py
+-rw-rw-rw-   0        0        0     2573 2023-07-08 17:49:03.000000 edp_redy_py-0.1.5/src/edp_redy/edp_mqtt.py
+drwxrwxrwx   0        0        0        0 2023-07-08 17:55:23.119826 edp_redy_py-0.1.5/src/edp_redy/equipment/
+-rw-rw-rw-   0        0        0        0 2023-07-08 16:25:40.000000 edp_redy_py-0.1.5/src/edp_redy/equipment/__init__.py
+-rw-rw-rw-   0        0        0     7618 2023-07-08 17:33:47.000000 edp_redy_py-0.1.5/src/edp_redy/equipment/equipment.py
+-rw-rw-rw-   0        0        0     1003 2023-07-08 16:51:43.000000 edp_redy_py-0.1.5/src/edp_redy/helpers.py
+-rw-rw-rw-   0        0        0      721 2023-07-08 17:37:45.000000 edp_redy_py-0.1.5/src/edp_redy/redy.py
+drwxrwxrwx   0        0        0        0 2023-07-08 17:55:23.121411 edp_redy_py-0.1.5/src/edp_redy/usermanagement/
+-rw-rw-rw-   0        0        0        0 2023-07-08 15:24:38.000000 edp_redy_py-0.1.5/src/edp_redy/usermanagement/__init__.py
+-rw-rw-rw-   0        0        0     2296 2023-07-08 17:33:51.000000 edp_redy_py-0.1.5/src/edp_redy/usermanagement/usermanagement.py
+drwxrwxrwx   0        0        0        0 2023-07-08 17:55:23.130896 edp_redy_py-0.1.5/src/edp_redy_py.egg-info/
+-rw-rw-rw-   0        0        0      283 2023-07-08 17:55:23.000000 edp_redy_py-0.1.5/src/edp_redy_py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      496 2023-07-08 17:55:23.000000 edp_redy_py-0.1.5/src/edp_redy_py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-08 17:55:23.000000 edp_redy_py-0.1.5/src/edp_redy_py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-07-08 17:55:23.000000 edp_redy_py-0.1.5/src/edp_redy_py.egg-info/top_level.txt
```

### Comparing `edp_redy_py-0.1.4/LICENSE` & `edp_redy_py-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `edp_redy_py-0.1.4/src/edp_redy/authenticate.py` & `edp_redy_py-0.1.5/src/edp_redy/authenticate.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from .consts import POOL_ID, CLIENT_ID, POOL_REGION
 
 io.init_logging(io.LogLevel.Error, 'stderr')
 
 
 def authenticate(USERNAME, PASSWORD):
     aws = AWSSRP(username=USERNAME, password=PASSWORD, pool_id=POOL_ID, client_id=CLIENT_ID, pool_region=POOL_REGION)
-    authentication = AuthenticationResult.from_dict(json.loads(aws.authenticate_user()))
+    authentication = AuthenticationResult.from_dict(aws.authenticate_user()["AuthenticationResult"])
     return authentication
 
 
 @dataclass
 class NewDeviceMetadata:
     DeviceKey: str
     DeviceGroupKey: str
```

### Comparing `edp_redy_py-0.1.4/src/edp_redy/edp_mqtt.py` & `edp_redy_py-0.1.5/src/edp_redy/edp_mqtt.py`

 * *Files identical despite different names*

### Comparing `edp_redy_py-0.1.4/src/edp_redy/equipment/equipment.py` & `edp_redy_py-0.1.5/src/edp_redy/equipment/equipment.py`

 * *Files identical despite different names*

### Comparing `edp_redy_py-0.1.4/src/edp_redy/helpers.py` & `edp_redy_py-0.1.5/src/edp_redy/helpers.py`

 * *Files identical despite different names*

### Comparing `edp_redy_py-0.1.4/src/edp_redy/redy.py` & `edp_redy_py-0.1.5/src/edp_redy/redy.py`

 * *Files identical despite different names*

### Comparing `edp_redy_py-0.1.4/src/edp_redy/usermanagement/usermanagement.py` & `edp_redy_py-0.1.5/src/edp_redy/usermanagement/usermanagement.py`

 * *Files identical despite different names*

