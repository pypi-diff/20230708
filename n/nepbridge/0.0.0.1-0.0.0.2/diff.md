# Comparing `tmp/nepbridge-0.0.0.1.tar.gz` & `tmp/nepbridge-0.0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\nepbridge-0.0.0.1.tar", last modified: Sat Jul  8 20:50:31 2023, max compression
+gzip compressed data, was "dist\nepbridge-0.0.0.2.tar", last modified: Sat Jul  8 20:59:00 2023, max compression
```

## Comparing `nepbridge-0.0.0.1.tar` & `nepbridge-0.0.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-07-08 20:50:31.000000 nepbridge-0.0.0.1/
--rw-rw-rw-   0        0        0     1094 2023-06-30 01:37:20.000000 nepbridge-0.0.0.1/LICENSE
--rw-rw-rw-   0        0        0     1109 2023-07-08 20:50:31.000000 nepbridge-0.0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       89 2023-07-08 03:40:38.000000 nepbridge-0.0.0.1/README.md
--rw-rw-rw-   0        0        0       42 2023-07-08 20:50:31.000000 nepbridge-0.0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1283 2023-07-08 20:50:24.000000 nepbridge-0.0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-08 20:50:31.000000 nepbridge-0.0.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-07-08 20:50:31.000000 nepbridge-0.0.0.1/src/nepbridge/
--rw-rw-rw-   0        0        0    13688 2023-07-08 03:40:38.000000 nepbridge-0.0.0.1/src/nepbridge/JSON2ROS.py
--rw-rw-rw-   0        0        0     8585 2023-07-08 03:40:38.000000 nepbridge-0.0.0.1/src/nepbridge/ROS2JSON.py
--rw-rw-rw-   0        0        0      199 2023-07-08 03:40:38.000000 nepbridge-0.0.0.1/src/nepbridge/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-08 20:50:31.000000 nepbridge-0.0.0.1/src/nepbridge.egg-info/
--rw-rw-rw-   0        0        0     1109 2023-07-08 20:50:31.000000 nepbridge-0.0.0.1/src/nepbridge.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      288 2023-07-08 20:50:31.000000 nepbridge-0.0.0.1/src/nepbridge.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-08 20:50:31.000000 nepbridge-0.0.0.1/src/nepbridge.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        4 2023-07-08 20:50:31.000000 nepbridge-0.0.0.1/src/nepbridge.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-07-08 20:50:31.000000 nepbridge-0.0.0.1/src/nepbridge.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-08 20:59:00.000000 nepbridge-0.0.0.2/
+-rw-rw-rw-   0        0        0     1094 2023-06-30 01:37:20.000000 nepbridge-0.0.0.2/LICENSE
+-rw-rw-rw-   0        0        0     1109 2023-07-08 20:59:00.000000 nepbridge-0.0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       89 2023-07-08 03:40:38.000000 nepbridge-0.0.0.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-08 20:59:00.000000 nepbridge-0.0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1283 2023-07-08 20:58:49.000000 nepbridge-0.0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-08 20:59:00.000000 nepbridge-0.0.0.2/src/
+drwxrwxrwx   0        0        0        0 2023-07-08 20:59:00.000000 nepbridge-0.0.0.2/src/nepbridge/
+-rw-rw-rw-   0        0        0    13688 2023-07-08 20:57:48.000000 nepbridge-0.0.0.2/src/nepbridge/JSON2ROS.py
+-rw-rw-rw-   0        0        0     8585 2023-07-08 03:40:38.000000 nepbridge-0.0.0.2/src/nepbridge/ROS2JSON.py
+-rw-rw-rw-   0        0        0      199 2023-07-08 03:40:38.000000 nepbridge-0.0.0.2/src/nepbridge/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-08 20:59:00.000000 nepbridge-0.0.0.2/src/nepbridge.egg-info/
+-rw-rw-rw-   0        0        0     1109 2023-07-08 20:59:00.000000 nepbridge-0.0.0.2/src/nepbridge.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      288 2023-07-08 20:59:00.000000 nepbridge-0.0.0.2/src/nepbridge.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-08 20:59:00.000000 nepbridge-0.0.0.2/src/nepbridge.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        4 2023-07-08 20:59:00.000000 nepbridge-0.0.0.2/src/nepbridge.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-08 20:59:00.000000 nepbridge-0.0.0.2/src/nepbridge.egg-info/top_level.txt
```

### Comparing `nepbridge-0.0.0.1/LICENSE` & `nepbridge-0.0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nepbridge-0.0.0.1/PKG-INFO` & `nepbridge-0.0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nepbridge
-Version: 0.0.0.1
+Version: 0.0.0.2
 Summary: Enrique Coronado
 Home-page: http://enriquecoronadozu.github.io
 Author: Enrique Coronado
 Author-email: enriquecoronadozu@gmail.com
 Keywords: Technology
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 2.7
```

### Comparing `nepbridge-0.0.0.1/setup.py` & `nepbridge-0.0.0.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup
 
 setup(
 
     name = 'nepbridge', 
-    version='0.0.0.1',
+    version='0.0.0.2',
     description = 'Enrique Coronado',
     packages=["nepbridge"],
     package_dir = {'':'src'},
     author='Enrique Coronado',
     author_email='enriquecoronadozu@gmail.com',
     url='http://enriquecoronadozu.github.io',
     include_package_data=True,
```

### Comparing `nepbridge-0.0.0.1/src/nepbridge/JSON2ROS.py` & `nepbridge-0.0.0.2/src/nepbridge/JSON2ROS.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import json
-from geometry_msgs.msg import Accel, Point, Pose, Quaternion, Transform, Twist, Vector3, Wrench, Point32, ChannelFloat32
-from sensor_msgs.msg import CameraInfo, JointState, Imu, Temperature, PointCloud
+from geometry_msgs.msg import Accel, Point, Pose, Quaternion, Transform, Twist, Vector3, Wrench, Point32
+from sensor_msgs.msg import CameraInfo, JointState, Imu, Temperature, PointCloud, ChannelFloat32
 from std_msgs.msg import String, Float32, ColorRGBA, Bool, Int32
 
 
 def create_ros_message(data, handle_missing_msg_type=False):
 
     if "msg_type" in data:
         msg_type = data["msg_type"]
```

### Comparing `nepbridge-0.0.0.1/src/nepbridge/ROS2JSON.py` & `nepbridge-0.0.0.2/src/nepbridge/ROS2JSON.py`

 * *Files identical despite different names*

### Comparing `nepbridge-0.0.0.1/src/nepbridge.egg-info/PKG-INFO` & `nepbridge-0.0.0.2/src/nepbridge.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nepbridge
-Version: 0.0.0.1
+Version: 0.0.0.2
 Summary: Enrique Coronado
 Home-page: http://enriquecoronadozu.github.io
 Author: Enrique Coronado
 Author-email: enriquecoronadozu@gmail.com
 Keywords: Technology
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 2.7
```

