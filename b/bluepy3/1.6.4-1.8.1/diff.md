# Comparing `tmp/bluepy3-1.6.4.tar.gz` & `tmp/bluepy3-1.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bluepy3-1.6.4.tar", last modified: Tue Jun  6 06:52:01 2023, max compression
+gzip compressed data, was "bluepy3-1.8.1.tar", last modified: Sat Jul  8 10:09:38 2023, max compression
```

## Comparing `bluepy3-1.6.4.tar` & `bluepy3-1.8.1.tar`

### file list

```diff
@@ -1,29 +1,30 @@
-drwxr-xr-x   0 maurice    (501) staff       (20)        0 2023-06-06 06:52:01.678108 bluepy3-1.6.4/
--rw-r--r--   0 maurice    (501) staff       (20)     1084 2023-04-29 09:30:37.000000 bluepy3-1.6.4/LICENSE
--rw-r--r--   0 maurice    (501) staff       (20)     5536 2023-06-06 06:52:01.678196 bluepy3-1.6.4/PKG-INFO
--rw-r--r--   0 maurice    (501) staff       (20)     3650 2023-06-04 07:33:33.000000 bluepy3-1.6.4/README.md
-drwxr-xr-x   0 maurice    (501) staff       (20)        0 2023-06-06 06:52:01.677207 bluepy3-1.6.4/bluepy3/
--rw-r--r--   0 maurice    (501) staff       (20)     1571 2023-04-29 09:30:37.000000 bluepy3-1.6.4/bluepy3/Makefile
--rwxr-xr-x   0 maurice    (501) staff       (20)      135 2023-04-29 09:30:37.000000 bluepy3-1.6.4/bluepy3/__init__.py
--rwxr-xr-x   0 maurice    (501) staff       (20)     4732 2023-06-04 08:43:19.000000 bluepy3-1.6.4/bluepy3/blescan.py
--rw-r--r--   0 maurice    (501) staff       (20)    58458 2023-04-29 09:30:37.000000 bluepy3-1.6.4/bluepy3/bluepy3-helper.c
--rwxr-xr-x   0 maurice    (501) staff       (20)    36910 2023-06-04 08:43:37.000000 bluepy3-1.6.4/bluepy3/btle.py
--rw-r--r--   0 maurice    (501) staff       (20)     4167 2023-04-29 09:30:37.000000 bluepy3-1.6.4/bluepy3/config.5.47.h
--rw-r--r--   0 maurice    (501) staff       (20)     4317 2023-04-29 09:30:37.000000 bluepy3-1.6.4/bluepy3/config.5.50.h
--rw-r--r--   0 maurice    (501) staff       (20)     4317 2023-04-29 09:30:37.000000 bluepy3-1.6.4/bluepy3/config.5.60.h
--rw-r--r--   0 maurice    (501) staff       (20)     4317 2023-04-29 09:30:37.000000 bluepy3-1.6.4/bluepy3/config.5.66.h
--rwxr-xr-x   0 maurice    (501) staff       (20)     9749 2023-06-04 08:43:19.000000 bluepy3-1.6.4/bluepy3/get_services.py
--rwxr-xr-x   0 maurice    (501) staff       (20)      690 2023-04-29 09:30:37.000000 bluepy3-1.6.4/bluepy3/scan_fuzz.py
--rwxr-xr-x   0 maurice    (501) staff       (20)      454 2023-04-29 09:30:37.000000 bluepy3-1.6.4/bluepy3/scanner.py
--rwxr-xr-x   0 maurice    (501) staff       (20)    16627 2023-06-04 08:43:19.000000 bluepy3-1.6.4/bluepy3/sensortag.py
--rwxr-xr-x   0 maurice    (501) staff       (20)    34902 2023-06-04 08:43:19.000000 bluepy3-1.6.4/bluepy3/thingy52.py
--rw-r--r--   0 maurice    (501) staff       (20)    37880 2023-04-29 09:30:37.000000 bluepy3-1.6.4/bluepy3/uuids.json
--rw-r--r--   0 maurice    (501) staff       (20)      125 2023-04-29 09:30:37.000000 bluepy3-1.6.4/bluepy3/version.h
-drwxr-xr-x   0 maurice    (501) staff       (20)        0 2023-06-06 06:52:01.677888 bluepy3-1.6.4/bluepy3.egg-info/
--rw-r--r--   0 maurice    (501) staff       (20)     5536 2023-06-06 06:52:01.000000 bluepy3-1.6.4/bluepy3.egg-info/PKG-INFO
--rw-r--r--   0 maurice    (501) staff       (20)      521 2023-06-06 06:52:01.000000 bluepy3-1.6.4/bluepy3.egg-info/SOURCES.txt
--rw-r--r--   0 maurice    (501) staff       (20)        1 2023-06-06 06:52:01.000000 bluepy3-1.6.4/bluepy3.egg-info/dependency_links.txt
--rw-r--r--   0 maurice    (501) staff       (20)      117 2023-06-06 06:52:01.000000 bluepy3-1.6.4/bluepy3.egg-info/entry_points.txt
--rw-r--r--   0 maurice    (501) staff       (20)        8 2023-06-06 06:52:01.000000 bluepy3-1.6.4/bluepy3.egg-info/top_level.txt
--rw-r--r--   0 maurice    (501) staff       (20)       94 2023-06-06 06:52:01.678428 bluepy3-1.6.4/setup.cfg
--rw-r--r--   0 maurice    (501) staff       (20)     3467 2023-06-06 06:51:38.000000 bluepy3-1.6.4/setup.py
+drwxr-xr-x   0 maurice    (501) staff       (20)        0 2023-07-08 10:09:38.659618 bluepy3-1.8.1/
+-rw-r--r--   0 maurice    (501) staff       (20)     1084 2023-04-29 09:30:37.000000 bluepy3-1.8.1/LICENSE
+-rw-r--r--   0 maurice    (501) staff       (20)     5536 2023-07-08 10:09:38.659698 bluepy3-1.8.1/PKG-INFO
+-rw-r--r--   0 maurice    (501) staff       (20)     3650 2023-06-04 07:33:33.000000 bluepy3-1.8.1/README.md
+drwxr-xr-x   0 maurice    (501) staff       (20)        0 2023-07-08 10:09:38.658877 bluepy3-1.8.1/bluepy3/
+-rw-r--r--   0 maurice    (501) staff       (20)     1723 2023-07-08 09:22:49.000000 bluepy3-1.8.1/bluepy3/Makefile
+-rwxr-xr-x   0 maurice    (501) staff       (20)      135 2023-04-29 09:30:37.000000 bluepy3-1.8.1/bluepy3/__init__.py
+-rwxr-xr-x   0 maurice    (501) staff       (20)     4732 2023-06-04 08:43:19.000000 bluepy3-1.8.1/bluepy3/blescan.py
+-rw-r--r--   0 maurice    (501) staff       (20)    58458 2023-04-29 09:30:37.000000 bluepy3-1.8.1/bluepy3/bluepy3-helper.c
+-rwxr-xr-x   0 maurice    (501) staff       (20)    36910 2023-06-04 08:43:37.000000 bluepy3-1.8.1/bluepy3/btle.py
+-rw-r--r--   0 maurice    (501) staff       (20)     4167 2023-04-29 09:30:37.000000 bluepy3-1.8.1/bluepy3/config.5.47.h
+-rw-r--r--   0 maurice    (501) staff       (20)     4317 2023-04-29 09:30:37.000000 bluepy3-1.8.1/bluepy3/config.5.50.h
+-rw-r--r--   0 maurice    (501) staff       (20)     4317 2023-04-29 09:30:37.000000 bluepy3-1.8.1/bluepy3/config.5.60.h
+-rw-r--r--   0 maurice    (501) staff       (20)     4317 2023-04-29 09:30:37.000000 bluepy3-1.8.1/bluepy3/config.5.66.h
+-rw-r--r--   0 maurice    (501) staff       (20)     4317 2023-07-08 08:43:06.000000 bluepy3-1.8.1/bluepy3/config.5.68.h
+-rwxr-xr-x   0 maurice    (501) staff       (20)     9749 2023-06-04 08:43:19.000000 bluepy3-1.8.1/bluepy3/get_services.py
+-rwxr-xr-x   0 maurice    (501) staff       (20)      690 2023-04-29 09:30:37.000000 bluepy3-1.8.1/bluepy3/scan_fuzz.py
+-rwxr-xr-x   0 maurice    (501) staff       (20)      454 2023-04-29 09:30:37.000000 bluepy3-1.8.1/bluepy3/scanner.py
+-rwxr-xr-x   0 maurice    (501) staff       (20)    16627 2023-06-04 08:43:19.000000 bluepy3-1.8.1/bluepy3/sensortag.py
+-rwxr-xr-x   0 maurice    (501) staff       (20)    34902 2023-06-04 08:43:19.000000 bluepy3-1.8.1/bluepy3/thingy52.py
+-rw-r--r--   0 maurice    (501) staff       (20)    37880 2023-04-29 09:30:37.000000 bluepy3-1.8.1/bluepy3/uuids.json
+-rw-r--r--   0 maurice    (501) staff       (20)      125 2023-04-29 09:30:37.000000 bluepy3-1.8.1/bluepy3/version.h
+drwxr-xr-x   0 maurice    (501) staff       (20)        0 2023-07-08 10:09:38.659515 bluepy3-1.8.1/bluepy3.egg-info/
+-rw-r--r--   0 maurice    (501) staff       (20)     5536 2023-07-08 10:09:38.000000 bluepy3-1.8.1/bluepy3.egg-info/PKG-INFO
+-rw-r--r--   0 maurice    (501) staff       (20)      543 2023-07-08 10:09:38.000000 bluepy3-1.8.1/bluepy3.egg-info/SOURCES.txt
+-rw-r--r--   0 maurice    (501) staff       (20)        1 2023-07-08 10:09:38.000000 bluepy3-1.8.1/bluepy3.egg-info/dependency_links.txt
+-rw-r--r--   0 maurice    (501) staff       (20)      117 2023-07-08 10:09:38.000000 bluepy3-1.8.1/bluepy3.egg-info/entry_points.txt
+-rw-r--r--   0 maurice    (501) staff       (20)        8 2023-07-08 10:09:38.000000 bluepy3-1.8.1/bluepy3.egg-info/top_level.txt
+-rw-r--r--   0 maurice    (501) staff       (20)       94 2023-07-08 10:09:38.659925 bluepy3-1.8.1/setup.cfg
+-rw-r--r--   0 maurice    (501) staff       (20)     3548 2023-07-08 10:09:14.000000 bluepy3-1.8.1/setup.py
```

### Comparing `bluepy3-1.6.4/LICENSE` & `bluepy3-1.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bluepy3-1.6.4/PKG-INFO` & `bluepy3-1.8.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bluepy3
-Version: 1.6.4
+Version: 1.8.1
 Summary: Python module for interfacing with BLE devices through Bluez
 Home-page: https://github.com/Mausy5043/bluepy3
 Download-URL: https://github.com/Mausy5043/bluepy3
 Author: mausy5043
 Keywords: Bluetooth,Bluetooth Smart,BLE,Bluetooth Low Energy,Raspberry Pi
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `bluepy3-1.6.4/README.md` & `bluepy3-1.8.1/README.md`

 * *Files identical despite different names*

### Comparing `bluepy3-1.6.4/bluepy3/Makefile` & `bluepy3-1.8.1/bluepy3/Makefile`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,20 @@
-BLUEZ_VERSION=5.66
+BLUEZ_VERSION=5.68
 
 BLUEZ_PATH=/tmp/bluez-$(BLUEZ_VERSION)
 
 BLUEZ_SRCS  = lib/bluetooth.c lib/hci.c lib/sdp.c lib/uuid.c
 BLUEZ_SRCS += attrib/att.c attrib/gatt.c attrib/gattrib.c attrib/utils.c
 BLUEZ_SRCS += btio/btio.c src/log.c src/shared/mgmt.c
 BLUEZ_SRCS += src/shared/crypto.c src/shared/att.c src/shared/queue.c src/shared/util.c
 BLUEZ_SRCS += src/shared/io-glib.c src/shared/timeout-glib.c
 # compiling against bluez 5.50+ requires these additional sources
 BLUEZ_SRCS += src/shared/log.c
+# compiling against bluez 5.58+ requires these additional sources
+BLUEZ_SRCS += src/shared/gatt-client.c src/shared/gatt-db.c src/shared/gatt-helpers.c
 
 IMPORT_SRCS = $(addprefix $(BLUEZ_PATH)/, $(BLUEZ_SRCS))
 LOCAL_SRCS  = bluepy3-helper.c
 
 CC ?= gcc
 CFLAGS += -g -Wall # -Werror
```

### Comparing `bluepy3-1.6.4/bluepy3/blescan.py` & `bluepy3-1.8.1/bluepy3/blescan.py`

 * *Files identical despite different names*

### Comparing `bluepy3-1.6.4/bluepy3/bluepy3-helper.c` & `bluepy3-1.8.1/bluepy3/bluepy3-helper.c`

 * *Files identical despite different names*

### Comparing `bluepy3-1.6.4/bluepy3/btle.py` & `bluepy3-1.8.1/bluepy3/btle.py`

 * *Files identical despite different names*

### Comparing `bluepy3-1.6.4/bluepy3/config.5.47.h` & `bluepy3-1.8.1/bluepy3/config.5.47.h`

 * *Files identical despite different names*

### Comparing `bluepy3-1.6.4/bluepy3/config.5.50.h` & `bluepy3-1.8.1/bluepy3/config.5.50.h`

 * *Files identical despite different names*

### Comparing `bluepy3-1.6.4/bluepy3/config.5.60.h` & `bluepy3-1.8.1/bluepy3/config.5.60.h`

 * *Files identical despite different names*

### Comparing `bluepy3-1.6.4/bluepy3/config.5.66.h` & `bluepy3-1.8.1/bluepy3/config.5.66.h`

 * *Files identical despite different names*

### Comparing `bluepy3-1.6.4/bluepy3/get_services.py` & `bluepy3-1.8.1/bluepy3/get_services.py`

 * *Files identical despite different names*

### Comparing `bluepy3-1.6.4/bluepy3/scan_fuzz.py` & `bluepy3-1.8.1/bluepy3/scan_fuzz.py`

 * *Files identical despite different names*

### Comparing `bluepy3-1.6.4/bluepy3/sensortag.py` & `bluepy3-1.8.1/bluepy3/sensortag.py`

 * *Files identical despite different names*

### Comparing `bluepy3-1.6.4/bluepy3/thingy52.py` & `bluepy3-1.8.1/bluepy3/thingy52.py`

 * *Files identical despite different names*

### Comparing `bluepy3-1.6.4/bluepy3/uuids.json` & `bluepy3-1.8.1/bluepy3/uuids.json`

 * *Files identical despite different names*

### Comparing `bluepy3-1.6.4/bluepy3.egg-info/PKG-INFO` & `bluepy3-1.8.1/bluepy3.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bluepy3
-Version: 1.6.4
+Version: 1.8.1
 Summary: Python module for interfacing with BLE devices through Bluez
 Home-page: https://github.com/Mausy5043/bluepy3
 Download-URL: https://github.com/Mausy5043/bluepy3
 Author: mausy5043
 Keywords: Bluetooth,Bluetooth Smart,BLE,Bluetooth Low Energy,Raspberry Pi
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `bluepy3-1.6.4/bluepy3.egg-info/SOURCES.txt` & `bluepy3-1.8.1/bluepy3.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 bluepy3/blescan.py
 bluepy3/bluepy3-helper.c
 bluepy3/btle.py
 bluepy3/config.5.47.h
 bluepy3/config.5.50.h
 bluepy3/config.5.60.h
 bluepy3/config.5.66.h
+bluepy3/config.5.68.h
 bluepy3/get_services.py
 bluepy3/scan_fuzz.py
 bluepy3/scanner.py
 bluepy3/sensortag.py
 bluepy3/thingy52.py
 bluepy3/uuids.json
 bluepy3/version.h
```

### Comparing `bluepy3-1.6.4/setup.py` & `bluepy3-1.8.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 import shlex
 import subprocess
 import sys
 
 from setuptools import setup
 from setuptools.command.build_py import build_py
 
-# VERSION = "1.7.1"  # latest version for testing
-VERSION = "1.6.4"  # latest version for production
+# VERSION = "1.7.8"  # latest version for testing
+VERSION = "1.8.1"  # latest version for production
 MAKEFILE = "bluepy3/Makefile"
 VERSION_FILE = "bluepy3/version.h"
 BLUEZ_VERSION = "(unknown)"
 
 
 def pre_install():
     """Do the custom compiling of the bluepy3-helper executable from the makefile"""
@@ -30,18 +30,19 @@
         with open(VERSION_FILE, "w", encoding="utf-8") as verfile:
             verfile.write(f'#define VERSION_STRING "{VERSION}-{BLUEZ_VERSION}"\n')
         for cmd in ["make -dC bluepy3 clean", "make -dC bluepy3 -j1"]:
             print(f"\nexecute {cmd}")
             msgs = subprocess.check_output(shlex.split(cmd), stderr=subprocess.STDOUT)  # noqa
         print("\n\n*** Finished pre-install ***\n\n")
     except subprocess.CalledProcessError as e:
-        print("Failed to compile bluepy3-helper. Exiting install.")
         print(f"Command was {repr(cmd)} in {os.getcwd()}")
         print(f"Return code was {e.returncode}")
-        print(f"Output was:\n{e.output}")
+        err_out = e.output
+        print(f"Output was:\n{err_out.decode('utf-8')}")
+        print(f"\nFailed to compile bluepy3-helper version {VERSION}-{BLUEZ_VERSION}. Exiting install.\n")
         sys.exit(1)
 
 
 class MyBuildPy(build_py):
     def run(self):
         pre_install()
         build_py.run(self)
```

