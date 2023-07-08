# Comparing `tmp/pyezviz-0.2.2.0.tar.gz` & `tmp/pyezviz-0.2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyezviz-0.2.2.0.tar", last modified: Tue Jul  4 05:42:08 2023, max compression
+gzip compressed data, was "pyezviz-0.2.2.1.tar", last modified: Sat Jul  8 19:55:13 2023, max compression
```

## Comparing `pyezviz-0.2.2.0.tar` & `pyezviz-0.2.2.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 05:42:08.004020 pyezviz-0.2.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-04 05:41:57.000000 pyezviz-0.2.2.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-04 05:41:57.000000 pyezviz-0.2.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-07-04 05:42:08.004020 pyezviz-0.2.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4352 2023-07-04 05:41:57.000000 pyezviz-0.2.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 05:42:08.004020 pyezviz-0.2.2.0/pyezviz/
--rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-07-04 05:41:57.000000 pyezviz-0.2.2.0/pyezviz/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12269 2023-07-04 05:41:57.000000 pyezviz-0.2.2.0/pyezviz/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2188 2023-07-04 05:41:57.000000 pyezviz-0.2.2.0/pyezviz/api_endpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)    10613 2023-07-04 05:41:57.000000 pyezviz-0.2.2.0/pyezviz/camera.py
--rw-r--r--   0 runner    (1001) docker     (123)     5626 2023-07-04 05:41:57.000000 pyezviz-0.2.2.0/pyezviz/cas.py
--rw-r--r--   0 runner    (1001) docker     (123)    62664 2023-07-04 05:41:57.000000 pyezviz-0.2.2.0/pyezviz/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    10065 2023-07-04 05:41:57.000000 pyezviz-0.2.2.0/pyezviz/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-07-04 05:41:57.000000 pyezviz-0.2.2.0/pyezviz/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7866 2023-07-04 05:41:57.000000 pyezviz-0.2.2.0/pyezviz/mqtt.py
--rw-r--r--   0 runner    (1001) docker     (123)     4902 2023-07-04 05:41:57.000000 pyezviz-0.2.2.0/pyezviz/test_cam_rtsp.py
--rw-r--r--   0 runner    (1001) docker     (123)     3342 2023-07-04 05:41:57.000000 pyezviz-0.2.2.0/pyezviz/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 05:42:08.004020 pyezviz-0.2.2.0/pyezviz.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-07-04 05:42:07.000000 pyezviz-0.2.2.0/pyezviz.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-07-04 05:42:07.000000 pyezviz-0.2.2.0/pyezviz.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 05:42:07.000000 pyezviz-0.2.2.0/pyezviz.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-04 05:42:07.000000 pyezviz-0.2.2.0/pyezviz.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-04 05:42:07.000000 pyezviz-0.2.2.0/pyezviz.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-04 05:42:07.000000 pyezviz-0.2.2.0/pyezviz.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 05:42:08.004020 pyezviz-0.2.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      809 2023-07-04 05:41:57.000000 pyezviz-0.2.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 19:55:13.469589 pyezviz-0.2.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-08 19:55:05.000000 pyezviz-0.2.2.1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-08 19:55:05.000000 pyezviz-0.2.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-07-08 19:55:13.469589 pyezviz-0.2.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4352 2023-07-08 19:55:05.000000 pyezviz-0.2.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 19:55:13.469589 pyezviz-0.2.2.1/pyezviz/
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-07-08 19:55:05.000000 pyezviz-0.2.2.1/pyezviz/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12269 2023-07-08 19:55:05.000000 pyezviz-0.2.2.1/pyezviz/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2188 2023-07-08 19:55:05.000000 pyezviz-0.2.2.1/pyezviz/api_endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10752 2023-07-08 19:55:05.000000 pyezviz-0.2.2.1/pyezviz/camera.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5626 2023-07-08 19:55:05.000000 pyezviz-0.2.2.1/pyezviz/cas.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62740 2023-07-08 19:55:05.000000 pyezviz-0.2.2.1/pyezviz/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10065 2023-07-08 19:55:05.000000 pyezviz-0.2.2.1/pyezviz/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-07-08 19:55:05.000000 pyezviz-0.2.2.1/pyezviz/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7866 2023-07-08 19:55:05.000000 pyezviz-0.2.2.1/pyezviz/mqtt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4902 2023-07-08 19:55:05.000000 pyezviz-0.2.2.1/pyezviz/test_cam_rtsp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3342 2023-07-08 19:55:05.000000 pyezviz-0.2.2.1/pyezviz/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 19:55:13.469589 pyezviz-0.2.2.1/pyezviz.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-07-08 19:55:13.000000 pyezviz-0.2.2.1/pyezviz.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-07-08 19:55:13.000000 pyezviz-0.2.2.1/pyezviz.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 19:55:13.000000 pyezviz-0.2.2.1/pyezviz.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-08 19:55:13.000000 pyezviz-0.2.2.1/pyezviz.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-08 19:55:13.000000 pyezviz-0.2.2.1/pyezviz.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-08 19:55:13.000000 pyezviz-0.2.2.1/pyezviz.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 19:55:13.469589 pyezviz-0.2.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-07-08 19:55:05.000000 pyezviz-0.2.2.1/setup.py
```

### Comparing `pyezviz-0.2.2.0/LICENSE.md` & `pyezviz-0.2.2.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pyezviz-0.2.2.0/README.md` & `pyezviz-0.2.2.1/README.md`

 * *Files identical despite different names*

### Comparing `pyezviz-0.2.2.0/pyezviz/__init__.py` & `pyezviz-0.2.2.1/pyezviz/__init__.py`

 * *Files identical despite different names*

### Comparing `pyezviz-0.2.2.0/pyezviz/__main__.py` & `pyezviz-0.2.2.1/pyezviz/__main__.py`

 * *Files identical despite different names*

### Comparing `pyezviz-0.2.2.0/pyezviz/api_endpoints.py` & `pyezviz-0.2.2.1/pyezviz/api_endpoints.py`

 * *Files identical despite different names*

### Comparing `pyezviz-0.2.2.0/pyezviz/camera.py` & `pyezviz-0.2.2.1/pyezviz/camera.py`

 * *Files 1% similar despite different names*

```diff
@@ -156,14 +156,17 @@
             ),
             "NightVision_Model": self.fetch_key(
                 ["STATUS", "optionals", "NightVision_Model"]
             ),
             "batteryCameraWorkMode": self.fetch_key(
                 ["STATUS", "optionals", "workMode"]
             ),
+            "Alarm_AdvancedDetect": self.fetch_key(
+                ["STATUS", "optionals", "Alarm_AdvancedDetect", "type"]
+            ),
             "wifiInfos": self._device["WIFI"],
             "switches": self._switch,
             "optionals": self.fetch_key(["STATUS", "optionals"]),
             "supportExt": self._device["deviceInfos"]["supportExt"],
             "ezDeviceCapability": self.fetch_key(["deviceInfos", "ezDeviceCapability"]),
         }
```

### Comparing `pyezviz-0.2.2.0/pyezviz/cas.py` & `pyezviz-0.2.2.1/pyezviz/cas.py`

 * *Files identical despite different names*

### Comparing `pyezviz-0.2.2.0/pyezviz/client.py` & `pyezviz-0.2.2.1/pyezviz/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1174,15 +1174,15 @@
         _LOGGER.debug("PTZ Control: %s", json_output)
 
         return True
 
     def get_cam_key(
         self, serial: str, smscode: int | None = None, max_retries: int = 0
     ) -> Any:
-        """Get Camera encryption key."""
+        """Get Camera encryption key. The key that is set after the camera is added to the account."""
 
         if max_retries > MAX_RETRIES:
             raise PyEzvizError("Can't gather proper data. Max retries exceeded.")
 
         try:
             req = self._session.post(
                 "https://" + self._token["api_url"] + API_ENDPOINT_CAM_ENCRYPTKEY,
@@ -1230,15 +1230,15 @@
                     max_retries,
                 )
                 return self.get_cam_key(serial, smscode, max_retries + 1)
             raise PyEzvizError(
                 f"Could not get camera encryption key: Got {json_output})"
             )
 
-        return json_output
+        return json_output["encryptkey"]
 
     def create_panoramic(self, serial: str, max_retries: int = 0) -> Any:
         """Create panoramic image."""
 
         if max_retries > MAX_RETRIES:
             raise PyEzvizError("Can't gather proper data. Max retries exceeded.")
```

### Comparing `pyezviz-0.2.2.0/pyezviz/constants.py` & `pyezviz-0.2.2.1/pyezviz/constants.py`

 * *Files identical despite different names*

### Comparing `pyezviz-0.2.2.0/pyezviz/exceptions.py` & `pyezviz-0.2.2.1/pyezviz/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyezviz-0.2.2.0/pyezviz/mqtt.py` & `pyezviz-0.2.2.1/pyezviz/mqtt.py`

 * *Files identical despite different names*

### Comparing `pyezviz-0.2.2.0/pyezviz/test_cam_rtsp.py` & `pyezviz-0.2.2.1/pyezviz/test_cam_rtsp.py`

 * *Files identical despite different names*

### Comparing `pyezviz-0.2.2.0/pyezviz/utils.py` & `pyezviz-0.2.2.1/pyezviz/utils.py`

 * *Files identical despite different names*

### Comparing `pyezviz-0.2.2.0/setup.py` & `pyezviz-0.2.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='pyezviz',
-    version="0.2.2.0",
+    version="0.2.2.1",
     license='Apache Software License 2.0',
     author='Pierre Ourdouille',
     author_email='baqs@users.github.com',
     description='Pilot your Ezviz cameras',
     long_description="Pilot your Ezviz cameras with this module. Please view readme on github",
     url='http://github.com/baqs/pyEzviz/',
     packages=setuptools.find_packages(),
```

