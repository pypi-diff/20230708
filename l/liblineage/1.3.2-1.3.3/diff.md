# Comparing `tmp/liblineage-1.3.2.tar.gz` & `tmp/liblineage-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "liblineage-1.3.2.tar", max compression
+gzip compressed data, was "liblineage-1.3.3.tar", max compression
```

## Comparing `liblineage-1.3.2.tar` & `liblineage-1.3.3.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0      386 2022-08-26 23:24:36.752356 liblineage-1.3.2/README.md
--rw-r--r--   0        0        0      237 2023-05-01 17:23:47.459149 liblineage-1.3.2/liblineage/__init__.py
--rw-r--r--   0        0        0      198 2022-08-30 13:21:57.046166 liblineage-1.3.2/liblineage/constants/infra.py
--rw-r--r--   0        0        0      657 2023-03-06 00:37:23.199983 liblineage-1.3.2/liblineage/constants/versions.py
--rw-r--r--   0        0        0      746 2023-03-06 15:41:20.302137 liblineage-1.3.2/liblineage/device.py
--rw-r--r--   0        0        0     2277 2023-05-01 17:19:48.153672 liblineage-1.3.2/liblineage/hudson/build_target.py
--rw-r--r--   0        0        0      222 2022-09-10 16:59:53.229174 liblineage-1.3.2/liblineage/hudson/period.py
--rw-r--r--   0        0        0     2360 2023-03-06 15:35:33.081202 liblineage-1.3.2/liblineage/ota/full_update_info.py
--rw-r--r--   0        0        0      219 2023-03-06 13:45:03.612525 liblineage-1.3.2/liblineage/updater/__init__.py
--rw-r--r--   0        0        0      463 2023-03-06 13:57:45.253121 liblineage-1.3.2/liblineage/updater/http_utils.py
--rw-r--r--   0        0        0     2008 2023-03-06 15:15:22.908220 liblineage-1.3.2/liblineage/updater/v1/__init__.py
--rw-r--r--   0        0        0      479 2023-03-06 15:15:13.344857 liblineage-1.3.2/liblineage/updater/v1/_deserializer.py
--rw-r--r--   0        0        0     1249 2023-03-06 15:13:58.101291 liblineage-1.3.2/liblineage/updater/v1/build.py
--rw-r--r--   0        0        0     1726 2023-03-06 15:15:46.388292 liblineage-1.3.2/liblineage/updater/v2/__init__.py
--rw-r--r--   0        0        0      527 2023-03-06 15:16:02.488342 liblineage-1.3.2/liblineage/updater/v2/_deserializer.py
--rw-r--r--   0        0        0      943 2023-03-06 13:43:39.422459 liblineage-1.3.2/liblineage/updater/v2/build.py
--rw-r--r--   0        0        0      971 2023-03-06 00:38:14.543370 liblineage-1.3.2/liblineage/updater/v2/build_file.py
--rw-r--r--   0        0        0     1049 2023-04-11 15:28:06.745781 liblineage-1.3.2/liblineage/updater/v2/device.py
--rw-r--r--   0        0        0      681 2023-03-06 13:30:12.755159 liblineage-1.3.2/liblineage/updater/v2/oem.py
--rw-r--r--   0        0        0      543 2023-03-06 13:30:12.755159 liblineage-1.3.2/liblineage/updater/v2/oem_device.py
--rw-r--r--   0        0        0      879 2023-05-01 15:29:50.890397 liblineage-1.3.2/liblineage/wiki/data_types/architecture_data.py
--rw-r--r--   0        0        0      582 2022-08-27 01:08:57.416656 liblineage-1.3.2/liblineage/wiki/data_types/base_data.py
--rw-r--r--   0        0        0     1279 2023-05-01 17:14:06.456807 liblineage-1.3.2/liblineage/wiki/data_types/battery_data.py
--rw-r--r--   0        0        0      918 2023-05-01 17:14:18.776934 liblineage-1.3.2/liblineage/wiki/data_types/bluetooth_data.py
--rw-r--r--   0        0        0      904 2023-05-01 17:13:44.383245 liblineage-1.3.2/liblineage/wiki/data_types/camera_data.py
--rw-r--r--   0        0        0     1204 2023-05-01 15:29:50.890397 liblineage-1.3.2/liblineage/wiki/data_types/dimension_data.py
--rw-r--r--   0        0        0      819 2023-05-01 15:29:50.890397 liblineage-1.3.2/liblineage/wiki/data_types/peripherals_data.py
--rw-r--r--   0        0        0     1144 2023-05-01 17:15:15.924192 liblineage-1.3.2/liblineage/wiki/data_types/release_data.py
--rw-r--r--   0        0        0     1352 2023-05-01 15:29:50.890397 liblineage-1.3.2/liblineage/wiki/data_types/screen_data.py
--rw-r--r--   0        0        0      897 2023-05-01 17:15:56.411278 liblineage-1.3.2/liblineage/wiki/data_types/sdcard_data.py
--rw-r--r--   0        0        0    11617 2023-05-01 17:17:27.062215 liblineage-1.3.2/liblineage/wiki/device_data.py
--rw-r--r--   0        0        0      520 2023-05-01 17:23:43.362447 liblineage-1.3.2/pyproject.toml
--rw-r--r--   0        0        0     1281 1970-01-01 00:00:00.000000 liblineage-1.3.2/PKG-INFO
+-rw-r--r--   0        0        0      386 2022-08-26 23:24:36.752356 liblineage-1.3.3/README.md
+-rw-r--r--   0        0        0      237 2023-07-07 22:45:02.721415 liblineage-1.3.3/liblineage/__init__.py
+-rw-r--r--   0        0        0      198 2022-08-30 13:21:57.046166 liblineage-1.3.3/liblineage/constants/infra.py
+-rw-r--r--   0        0        0      657 2023-03-06 00:37:23.199983 liblineage-1.3.3/liblineage/constants/versions.py
+-rw-r--r--   0        0        0      746 2023-03-06 15:41:20.302137 liblineage-1.3.3/liblineage/device.py
+-rw-r--r--   0        0        0     2277 2023-05-01 17:19:48.153672 liblineage-1.3.3/liblineage/hudson/build_target.py
+-rw-r--r--   0        0        0      222 2022-09-10 16:59:53.229174 liblineage-1.3.3/liblineage/hudson/period.py
+-rw-r--r--   0        0        0     2360 2023-03-06 15:35:33.081202 liblineage-1.3.3/liblineage/ota/full_update_info.py
+-rw-r--r--   0        0        0      219 2023-03-06 13:45:03.612525 liblineage-1.3.3/liblineage/updater/__init__.py
+-rw-r--r--   0        0        0      463 2023-03-06 13:57:45.253121 liblineage-1.3.3/liblineage/updater/http_utils.py
+-rw-r--r--   0        0        0     2008 2023-03-06 15:15:22.908220 liblineage-1.3.3/liblineage/updater/v1/__init__.py
+-rw-r--r--   0        0        0      479 2023-03-06 15:15:13.344857 liblineage-1.3.3/liblineage/updater/v1/_deserializer.py
+-rw-r--r--   0        0        0     1249 2023-03-06 15:13:58.101291 liblineage-1.3.3/liblineage/updater/v1/build.py
+-rw-r--r--   0        0        0     1726 2023-03-06 15:15:46.388292 liblineage-1.3.3/liblineage/updater/v2/__init__.py
+-rw-r--r--   0        0        0      527 2023-03-06 15:16:02.488342 liblineage-1.3.3/liblineage/updater/v2/_deserializer.py
+-rw-r--r--   0        0        0      943 2023-03-06 13:43:39.422459 liblineage-1.3.3/liblineage/updater/v2/build.py
+-rw-r--r--   0        0        0      971 2023-03-06 00:38:14.543370 liblineage-1.3.3/liblineage/updater/v2/build_file.py
+-rw-r--r--   0        0        0     1049 2023-04-11 15:28:06.745781 liblineage-1.3.3/liblineage/updater/v2/device.py
+-rw-r--r--   0        0        0      681 2023-03-06 13:30:12.755159 liblineage-1.3.3/liblineage/updater/v2/oem.py
+-rw-r--r--   0        0        0      543 2023-03-06 13:30:12.755159 liblineage-1.3.3/liblineage/updater/v2/oem_device.py
+-rw-r--r--   0        0        0      879 2023-05-01 15:29:50.890397 liblineage-1.3.3/liblineage/wiki/data_types/architecture_data.py
+-rw-r--r--   0        0        0      582 2022-08-27 01:08:57.416656 liblineage-1.3.3/liblineage/wiki/data_types/base_data.py
+-rw-r--r--   0        0        0     1279 2023-05-01 17:14:06.456807 liblineage-1.3.3/liblineage/wiki/data_types/battery_data.py
+-rw-r--r--   0        0        0      918 2023-05-01 17:14:18.776934 liblineage-1.3.3/liblineage/wiki/data_types/bluetooth_data.py
+-rw-r--r--   0        0        0      904 2023-05-01 17:13:44.383245 liblineage-1.3.3/liblineage/wiki/data_types/camera_data.py
+-rw-r--r--   0        0        0     1204 2023-05-01 15:29:50.890397 liblineage-1.3.3/liblineage/wiki/data_types/dimension_data.py
+-rw-r--r--   0        0        0      819 2023-05-01 15:29:50.890397 liblineage-1.3.3/liblineage/wiki/data_types/peripherals_data.py
+-rw-r--r--   0        0        0     1144 2023-05-01 17:15:15.924192 liblineage-1.3.3/liblineage/wiki/data_types/release_data.py
+-rw-r--r--   0        0        0     1433 2023-07-07 22:45:02.674747 liblineage-1.3.3/liblineage/wiki/data_types/screen_data.py
+-rw-r--r--   0        0        0      897 2023-05-01 17:15:56.411278 liblineage-1.3.3/liblineage/wiki/data_types/sdcard_data.py
+-rw-r--r--   0        0        0    11617 2023-05-01 17:17:27.062215 liblineage-1.3.3/liblineage/wiki/device_data.py
+-rw-r--r--   0        0        0      520 2023-07-07 22:45:02.721415 liblineage-1.3.3/pyproject.toml
+-rw-r--r--   0        0        0     1281 1970-01-01 00:00:00.000000 liblineage-1.3.3/PKG-INFO
```

### Comparing `liblineage-1.3.2/liblineage/constants/versions.py` & `liblineage-1.3.3/liblineage/constants/versions.py`

 * *Files identical despite different names*

### Comparing `liblineage-1.3.2/liblineage/device.py` & `liblineage-1.3.3/liblineage/device.py`

 * *Files identical despite different names*

### Comparing `liblineage-1.3.2/liblineage/hudson/build_target.py` & `liblineage-1.3.3/liblineage/hudson/build_target.py`

 * *Files identical despite different names*

### Comparing `liblineage-1.3.2/liblineage/ota/full_update_info.py` & `liblineage-1.3.3/liblineage/ota/full_update_info.py`

 * *Files identical despite different names*

### Comparing `liblineage-1.3.2/liblineage/updater/v1/__init__.py` & `liblineage-1.3.3/liblineage/updater/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `liblineage-1.3.2/liblineage/updater/v1/build.py` & `liblineage-1.3.3/liblineage/updater/v1/build.py`

 * *Files identical despite different names*

### Comparing `liblineage-1.3.2/liblineage/updater/v2/__init__.py` & `liblineage-1.3.3/liblineage/updater/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `liblineage-1.3.2/liblineage/updater/v2/_deserializer.py` & `liblineage-1.3.3/liblineage/updater/v2/_deserializer.py`

 * *Files identical despite different names*

### Comparing `liblineage-1.3.2/liblineage/updater/v2/build.py` & `liblineage-1.3.3/liblineage/updater/v2/build.py`

 * *Files identical despite different names*

### Comparing `liblineage-1.3.2/liblineage/updater/v2/build_file.py` & `liblineage-1.3.3/liblineage/updater/v2/build_file.py`

 * *Files identical despite different names*

### Comparing `liblineage-1.3.2/liblineage/updater/v2/device.py` & `liblineage-1.3.3/liblineage/updater/v2/device.py`

 * *Files identical despite different names*

### Comparing `liblineage-1.3.2/liblineage/updater/v2/oem.py` & `liblineage-1.3.3/liblineage/updater/v2/oem.py`

 * *Files identical despite different names*

### Comparing `liblineage-1.3.2/liblineage/updater/v2/oem_device.py` & `liblineage-1.3.3/liblineage/updater/v2/oem_device.py`

 * *Files identical despite different names*

### Comparing `liblineage-1.3.2/liblineage/wiki/data_types/architecture_data.py` & `liblineage-1.3.3/liblineage/wiki/data_types/architecture_data.py`

 * *Files identical despite different names*

### Comparing `liblineage-1.3.2/liblineage/wiki/data_types/base_data.py` & `liblineage-1.3.3/liblineage/wiki/data_types/base_data.py`

 * *Files identical despite different names*

### Comparing `liblineage-1.3.2/liblineage/wiki/data_types/battery_data.py` & `liblineage-1.3.3/liblineage/wiki/data_types/battery_data.py`

 * *Files identical despite different names*

### Comparing `liblineage-1.3.2/liblineage/wiki/data_types/bluetooth_data.py` & `liblineage-1.3.3/liblineage/wiki/data_types/bluetooth_data.py`

 * *Files identical despite different names*

### Comparing `liblineage-1.3.2/liblineage/wiki/data_types/camera_data.py` & `liblineage-1.3.3/liblineage/wiki/data_types/camera_data.py`

 * *Files identical despite different names*

### Comparing `liblineage-1.3.2/liblineage/wiki/data_types/dimension_data.py` & `liblineage-1.3.3/liblineage/wiki/data_types/dimension_data.py`

 * *Files identical despite different names*

### Comparing `liblineage-1.3.2/liblineage/wiki/data_types/peripherals_data.py` & `liblineage-1.3.3/liblineage/wiki/data_types/peripherals_data.py`

 * *Files identical despite different names*

### Comparing `liblineage-1.3.2/liblineage/wiki/data_types/release_data.py` & `liblineage-1.3.3/liblineage/wiki/data_types/release_data.py`

 * *Files identical despite different names*

### Comparing `liblineage-1.3.2/liblineage/wiki/data_types/screen_data.py` & `liblineage-1.3.3/liblineage/wiki/data_types/screen_data.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,39 +1,43 @@
 #
-# Copyright (C) 2022 The LineageOS Project
+# Copyright (C) 2022-2023 The LineageOS Project
 #
 # SPDX-License-Identifier: LGPL-3.0-or-later
 #
 
-from typing import Dict, List, Union
+from typing import Dict, List, Optional, Union
 
 from liblineage.wiki.data_types.base_data import BaseData
 
 class ScreenData(BaseData):
 	"""LineageOS screen information.
 
 	Attributes:
 	- size: The screen size (inches)
 	- density: The screen density (dpi)
 	- resolution: The screen resolution (e.g. 1080x1920)
 	- technology: The screen technology (e.g. LCD)
+	- refresh_rate: Maximum screen refresh rate (Hz)
 	"""
-	def __init__(self,
-	             size: str,
-	             density: int,
-	             resolution: str,
-	             technology: str,
-	            ):
+	def __init__(
+		self,
+		size: str,
+		density: int,
+		resolution: str,
+		technology: str,
+		refresh_rate: Optional[int] = None,
+	):
 		"""Initialize the screen information."""
 		super().__init__()
 
 		self.size = size
 		self.density = density
 		self.resolution = resolution
 		self.technology = technology
+		self.refresh_rate = refresh_rate
 
 	@classmethod
 	def from_data(cls, data: Union[None, Dict, List, str]) -> Union[None, "ScreenData", Dict[str, "ScreenData"], None]:
 		"""Create a screen information object from YAML data."""
 		if data is None:
 			screen = None
 		elif isinstance(data, dict):
```

### Comparing `liblineage-1.3.2/liblineage/wiki/data_types/sdcard_data.py` & `liblineage-1.3.3/liblineage/wiki/data_types/sdcard_data.py`

 * *Files identical despite different names*

### Comparing `liblineage-1.3.2/liblineage/wiki/device_data.py` & `liblineage-1.3.3/liblineage/wiki/device_data.py`

 * *Files identical despite different names*

### Comparing `liblineage-1.3.2/pyproject.toml` & `liblineage-1.3.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "liblineage"
-version = "1.3.2"
+version = "1.3.3"
 description = "LineageOS utils library"
 authors = ["Sebastiano Barezzi <barezzisebastiano@gmail.com>"]
 license = "LGPL-3.0-or-later"
 readme = "README.md"
 repository = "https://github.com/sebaubuntu-python/liblineage"
 
 [tool.poetry.dependencies]
```

### Comparing `liblineage-1.3.2/PKG-INFO` & `liblineage-1.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: liblineage
-Version: 1.3.2
+Version: 1.3.3
 Summary: LineageOS utils library
 Home-page: https://github.com/sebaubuntu-python/liblineage
 License: LGPL-3.0-or-later
 Author: Sebastiano Barezzi
 Author-email: barezzisebastiano@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
```

