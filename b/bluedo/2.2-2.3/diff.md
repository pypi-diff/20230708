# Comparing `tmp/bluedo-2.2.tar.gz` & `tmp/bluedo-2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bluedo-2.2.tar", last modified: Tue Feb 21 19:06:22 2023, max compression
+gzip compressed data, was "bluedo-2.3.tar", last modified: Fri Jul  7 23:45:37 2023, max compression
```

## Comparing `bluedo-2.2.tar` & `bluedo-2.3.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxr-x   0 lars      (1000) lars      (1000)        0 2023-02-21 19:06:22.792077 bluedo-2.2/
--rw-rw-r--   0 lars      (1000) lars      (1000)    35149 2022-11-05 18:15:30.000000 bluedo-2.2/LICENSE
--rw-rw-r--   0 lars      (1000) lars      (1000)      487 2022-11-05 18:15:30.000000 bluedo-2.2/MANIFEST.in
--rw-rw-r--   0 lars      (1000) lars      (1000)     3985 2023-02-21 19:06:22.792077 bluedo-2.2/PKG-INFO
--rw-rw-r--   0 lars      (1000) lars      (1000)     3116 2023-02-21 18:55:47.000000 bluedo-2.2/README.md
-drwxrwxr-x   0 lars      (1000) lars      (1000)        0 2023-02-21 19:06:22.788077 bluedo-2.2/applications/
--rw-rw-r--   0 lars      (1000) lars      (1000)      251 2022-11-05 18:15:30.000000 bluedo-2.2/applications/bluedo.desktop
-drwxrwxr-x   0 lars      (1000) lars      (1000)        0 2023-02-21 19:06:22.792077 bluedo-2.2/bluedo/
--rwxrwxr-x   0 lars      (1000) lars      (1000)      252 2022-11-04 22:23:57.000000 bluedo-2.2/bluedo/__init__.py
--rw-rw-r--   0 lars      (1000) lars      (1000)   106494 2022-11-04 22:23:57.000000 bluedo-2.2/bluedo/bluedo.png
--rw-rw-r--   0 lars      (1000) lars      (1000)    27134 2023-02-21 19:03:10.000000 bluedo-2.2/bluedo/bluedoapp.py
--rw-rw-r--   0 lars      (1000) lars      (1000)    79675 2022-11-04 22:23:57.000000 bluedo-2.2/bluedo/lock_animation.gif
--rw-rw-r--   0 lars      (1000) lars      (1000)     8631 2022-11-04 22:23:57.000000 bluedo-2.2/bluedo/unlocked.png
--rw-rw-r--   0 lars      (1000) lars      (1000)    21441 2022-11-06 19:28:59.000000 bluedo-2.2/bluedo/window.glade
-drwxrwxr-x   0 lars      (1000) lars      (1000)        0 2023-02-21 19:06:22.792077 bluedo-2.2/bluedo.egg-info/
--rw-r--r--   0 lars      (1000) lars      (1000)     3985 2023-02-21 19:06:22.000000 bluedo-2.2/bluedo.egg-info/PKG-INFO
--rw-r--r--   0 lars      (1000) lars      (1000)      415 2023-02-21 19:06:22.000000 bluedo-2.2/bluedo.egg-info/SOURCES.txt
--rw-r--r--   0 lars      (1000) lars      (1000)        1 2023-02-21 19:06:22.000000 bluedo-2.2/bluedo.egg-info/dependency_links.txt
--rw-r--r--   0 lars      (1000) lars      (1000)       40 2023-02-21 19:06:22.000000 bluedo-2.2/bluedo.egg-info/entry_points.txt
--rw-r--r--   0 lars      (1000) lars      (1000)       48 2023-02-21 19:06:22.000000 bluedo-2.2/bluedo.egg-info/requires.txt
--rw-r--r--   0 lars      (1000) lars      (1000)        7 2023-02-21 19:06:22.000000 bluedo-2.2/bluedo.egg-info/top_level.txt
--rw-rw-r--   0 lars      (1000) lars      (1000)       38 2023-02-21 19:06:22.792077 bluedo-2.2/setup.cfg
--rw-rw-r--   0 lars      (1000) lars      (1000)     2263 2022-11-05 20:49:19.000000 bluedo-2.2/setup.py
-drwxrwxr-x   0 lars      (1000) lars      (1000)        0 2023-02-21 19:06:22.788077 bluedo-2.2/share/
-drwxrwxr-x   0 lars      (1000) lars      (1000)        0 2023-02-21 19:06:22.788077 bluedo-2.2/share/icons/
-drwxrwxr-x   0 lars      (1000) lars      (1000)        0 2023-02-21 19:06:22.788077 bluedo-2.2/share/icons/hicolor/
-drwxrwxr-x   0 lars      (1000) lars      (1000)        0 2023-02-21 19:06:22.788077 bluedo-2.2/share/icons/hicolor/256x256/
-drwxrwxr-x   0 lars      (1000) lars      (1000)        0 2023-02-21 19:06:22.792077 bluedo-2.2/share/icons/hicolor/256x256/apps/
--rw-rw-r--   0 lars      (1000) lars      (1000)   106494 2022-11-05 18:15:30.000000 bluedo-2.2/share/icons/hicolor/256x256/apps/bluedo.png
+drwxrwxr-x   0 lars      (1000) lars      (1000)        0 2023-07-07 23:45:37.787989 bluedo-2.3/
+-rw-rw-r--   0 lars      (1000) lars      (1000)    35149 2022-11-05 18:15:30.000000 bluedo-2.3/LICENSE
+-rw-rw-r--   0 lars      (1000) lars      (1000)      487 2022-11-05 18:15:30.000000 bluedo-2.3/MANIFEST.in
+-rw-rw-r--   0 lars      (1000) lars      (1000)     4050 2023-07-07 23:45:37.787989 bluedo-2.3/PKG-INFO
+-rw-rw-r--   0 lars      (1000) lars      (1000)     3181 2023-07-07 23:40:24.000000 bluedo-2.3/README.md
+drwxrwxr-x   0 lars      (1000) lars      (1000)        0 2023-07-07 23:45:37.783989 bluedo-2.3/applications/
+-rw-rw-r--   0 lars      (1000) lars      (1000)      251 2022-11-05 18:15:30.000000 bluedo-2.3/applications/bluedo.desktop
+drwxrwxr-x   0 lars      (1000) lars      (1000)        0 2023-07-07 23:45:37.787989 bluedo-2.3/bluedo/
+-rwxrwxr-x   0 lars      (1000) lars      (1000)      252 2022-11-04 22:23:57.000000 bluedo-2.3/bluedo/__init__.py
+-rw-rw-r--   0 lars      (1000) lars      (1000)   106494 2022-11-04 22:23:57.000000 bluedo-2.3/bluedo/bluedo.png
+-rw-rw-r--   0 lars      (1000) lars      (1000)    27134 2023-07-07 23:43:01.000000 bluedo-2.3/bluedo/bluedoapp.py
+-rw-rw-r--   0 lars      (1000) lars      (1000)    79675 2022-11-04 22:23:57.000000 bluedo-2.3/bluedo/lock_animation.gif
+-rw-rw-r--   0 lars      (1000) lars      (1000)     8631 2022-11-04 22:23:57.000000 bluedo-2.3/bluedo/unlocked.png
+-rw-rw-r--   0 lars      (1000) lars      (1000)    21441 2023-07-07 23:38:29.000000 bluedo-2.3/bluedo/window.glade
+drwxrwxr-x   0 lars      (1000) lars      (1000)        0 2023-07-07 23:45:37.787989 bluedo-2.3/bluedo.egg-info/
+-rw-r--r--   0 lars      (1000) lars      (1000)     4050 2023-07-07 23:45:37.000000 bluedo-2.3/bluedo.egg-info/PKG-INFO
+-rw-r--r--   0 lars      (1000) lars      (1000)      415 2023-07-07 23:45:37.000000 bluedo-2.3/bluedo.egg-info/SOURCES.txt
+-rw-r--r--   0 lars      (1000) lars      (1000)        1 2023-07-07 23:45:37.000000 bluedo-2.3/bluedo.egg-info/dependency_links.txt
+-rw-r--r--   0 lars      (1000) lars      (1000)       40 2023-07-07 23:45:37.000000 bluedo-2.3/bluedo.egg-info/entry_points.txt
+-rw-r--r--   0 lars      (1000) lars      (1000)       48 2023-07-07 23:45:37.000000 bluedo-2.3/bluedo.egg-info/requires.txt
+-rw-r--r--   0 lars      (1000) lars      (1000)        7 2023-07-07 23:45:37.000000 bluedo-2.3/bluedo.egg-info/top_level.txt
+-rw-rw-r--   0 lars      (1000) lars      (1000)       38 2023-07-07 23:45:37.787989 bluedo-2.3/setup.cfg
+-rw-rw-r--   0 lars      (1000) lars      (1000)     2263 2023-07-07 23:38:29.000000 bluedo-2.3/setup.py
+drwxrwxr-x   0 lars      (1000) lars      (1000)        0 2023-07-07 23:45:37.783989 bluedo-2.3/share/
+drwxrwxr-x   0 lars      (1000) lars      (1000)        0 2023-07-07 23:45:37.783989 bluedo-2.3/share/icons/
+drwxrwxr-x   0 lars      (1000) lars      (1000)        0 2023-07-07 23:45:37.783989 bluedo-2.3/share/icons/hicolor/
+drwxrwxr-x   0 lars      (1000) lars      (1000)        0 2023-07-07 23:45:37.783989 bluedo-2.3/share/icons/hicolor/256x256/
+drwxrwxr-x   0 lars      (1000) lars      (1000)        0 2023-07-07 23:45:37.787989 bluedo-2.3/share/icons/hicolor/256x256/apps/
+-rw-rw-r--   0 lars      (1000) lars      (1000)   106494 2022-11-05 18:15:30.000000 bluedo-2.3/share/icons/hicolor/256x256/apps/bluedo.png
```

### Comparing `bluedo-2.2/LICENSE` & `bluedo-2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `bluedo-2.2/PKG-INFO` & `bluedo-2.3/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bluedo
-Version: 2.2
+Version: 2.3
 Summary: Bluetooth proximity automation
 Home-page: https://github.com/ways/BlueDo/
 Author: Lars Falk-Petersen
 Author-email: dev@falkp.no
 License: GPLv3+
 Keywords: bluetooth
 Platform: UNKNOWN
@@ -29,18 +29,20 @@
 
 ![Logo](https://raw.githubusercontent.com/ways/BlueDo/master/images/bluedo.png)
 
 Lock your desktop, mute music or run any other command when leaving your PC. There are dozens of apps like this. This one just aims to make it beautiful, modern and easy.
 
 Not all bluetooth devices works for this. Some devices randomizes the bluetooth address as a privacy feature, some disconnects to save power. If you have trouble using your phone, try a headset, watch, etc.
 
+Only Bluetooth is supported, not Bluetooth Low-Energy (BLE).
+
 # Maturity
 
-2.1 is in beta
-1 is deprecated
+* 2 is in beta
+* 1 is deprecated
 
 # Installation
 
 ## From pip
 
     sudo apt install python3-pip gir1.2-appindicator3-0.1
     pip3 install --upgrade bluedo
@@ -57,14 +59,15 @@
 * hcitool
 * loginctl
 * gsettings
 * amixer (if using mute)
 * playerctl (if using pause)
 
 Version > 2.0 is only tested on Ubuntu 22.04 with GNOME.
+
 Version < 2.0 is only tested on Ubuntu 20.04-21.04 with GNOME.
 
 # Command line options
 
 * -e / --enable to start service on app start.
 * -m / --minimize to start minimized
```

### Comparing `bluedo-2.2/README.md` & `bluedo-2.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -4,18 +4,20 @@
 
 ![Logo](https://raw.githubusercontent.com/ways/BlueDo/master/images/bluedo.png)
 
 Lock your desktop, mute music or run any other command when leaving your PC. There are dozens of apps like this. This one just aims to make it beautiful, modern and easy.
 
 Not all bluetooth devices works for this. Some devices randomizes the bluetooth address as a privacy feature, some disconnects to save power. If you have trouble using your phone, try a headset, watch, etc.
 
+Only Bluetooth is supported, not Bluetooth Low-Energy (BLE).
+
 # Maturity
 
-2.1 is in beta
-1 is deprecated
+* 2 is in beta
+* 1 is deprecated
 
 # Installation
 
 ## From pip
 
     sudo apt install python3-pip gir1.2-appindicator3-0.1
     pip3 install --upgrade bluedo
@@ -32,14 +34,15 @@
 * hcitool
 * loginctl
 * gsettings
 * amixer (if using mute)
 * playerctl (if using pause)
 
 Version > 2.0 is only tested on Ubuntu 22.04 with GNOME.
+
 Version < 2.0 is only tested on Ubuntu 20.04-21.04 with GNOME.
 
 # Command line options
 
 * -e / --enable to start service on app start.
 * -m / --minimize to start minimized
```

### Comparing `bluedo-2.2/bluedo/bluedo.png` & `bluedo-2.3/bluedo/bluedo.png`

 * *Files identical despite different names*

### Comparing `bluedo-2.2/bluedo/bluedoapp.py` & `bluedo-2.3/bluedo/bluedoapp.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 import syslog
 import appdirs
 import configparser
 
 
 class BlueDo(Gtk.Application):
     project_name = 'bluedo'
-    project_version = 2.2
+    project_version = 2.3
     config_path = appdirs.user_config_dir(project_name) + '/' + project_name + '.ini'
     config_section = 'CONFIG'
     run_path = os.path.dirname(os.path.realpath(__file__)) + '/'
     autostart_dir = os.getenv("HOME") + '/.config/autostart/'
 
     builder = None
     enabled = False
```

### Comparing `bluedo-2.2/bluedo/lock_animation.gif` & `bluedo-2.3/bluedo/lock_animation.gif`

 * *Files identical despite different names*

### Comparing `bluedo-2.2/bluedo/unlocked.png` & `bluedo-2.3/bluedo/unlocked.png`

 * *Files identical despite different names*

### Comparing `bluedo-2.2/bluedo/window.glade` & `bluedo-2.3/bluedo/window.glade`

 * *Files identical despite different names*

### Comparing `bluedo-2.2/bluedo.egg-info/PKG-INFO` & `bluedo-2.3/bluedo.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bluedo
-Version: 2.2
+Version: 2.3
 Summary: Bluetooth proximity automation
 Home-page: https://github.com/ways/BlueDo/
 Author: Lars Falk-Petersen
 Author-email: dev@falkp.no
 License: GPLv3+
 Keywords: bluetooth
 Platform: UNKNOWN
@@ -29,18 +29,20 @@
 
 ![Logo](https://raw.githubusercontent.com/ways/BlueDo/master/images/bluedo.png)
 
 Lock your desktop, mute music or run any other command when leaving your PC. There are dozens of apps like this. This one just aims to make it beautiful, modern and easy.
 
 Not all bluetooth devices works for this. Some devices randomizes the bluetooth address as a privacy feature, some disconnects to save power. If you have trouble using your phone, try a headset, watch, etc.
 
+Only Bluetooth is supported, not Bluetooth Low-Energy (BLE).
+
 # Maturity
 
-2.1 is in beta
-1 is deprecated
+* 2 is in beta
+* 1 is deprecated
 
 # Installation
 
 ## From pip
 
     sudo apt install python3-pip gir1.2-appindicator3-0.1
     pip3 install --upgrade bluedo
@@ -57,14 +59,15 @@
 * hcitool
 * loginctl
 * gsettings
 * amixer (if using mute)
 * playerctl (if using pause)
 
 Version > 2.0 is only tested on Ubuntu 22.04 with GNOME.
+
 Version < 2.0 is only tested on Ubuntu 20.04-21.04 with GNOME.
 
 # Command line options
 
 * -e / --enable to start service on app start.
 * -m / --minimize to start minimized
```

### Comparing `bluedo-2.2/setup.py` & `bluedo-2.3/setup.py`

 * *Files identical despite different names*

### Comparing `bluedo-2.2/share/icons/hicolor/256x256/apps/bluedo.png` & `bluedo-2.3/share/icons/hicolor/256x256/apps/bluedo.png`

 * *Files identical despite different names*

