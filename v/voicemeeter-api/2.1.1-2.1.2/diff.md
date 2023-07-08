# Comparing `tmp/voicemeeter_api-2.1.1.tar.gz` & `tmp/voicemeeter_api-2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "voicemeeter_api-2.1.1.tar", max compression
+gzip compressed data, was "voicemeeter_api-2.1.2.tar", max compression
```

## Comparing `voicemeeter_api-2.1.1.tar` & `voicemeeter_api-2.1.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0     1091 2022-06-16 12:51:04.818279 voicemeeter_api-2.1.1/LICENSE
--rw-r--r--   0        0        0     1111 2023-07-01 18:51:25.724767 voicemeeter_api-2.1.1/pyproject.toml
--rw-r--r--   0        0        0    17394 2023-07-01 18:51:25.723761 voicemeeter_api-2.1.1/README.md
--rw-r--r--   0        0        0       69 2022-07-31 06:38:44.483821 voicemeeter_api-2.1.1/voicemeeterlib/__init__.py
--rw-r--r--   0        0        0     8226 2023-06-23 19:51:19.906407 voicemeeter_api-2.1.1/voicemeeterlib/bus.py
--rw-r--r--   0        0        0     4239 2023-06-22 23:20:33.622570 voicemeeter_api-2.1.1/voicemeeterlib/cbindings.py
--rw-r--r--   0        0        0     1194 2023-06-22 23:31:24.097081 voicemeeter_api-2.1.1/voicemeeterlib/command.py
--rw-r--r--   0        0        0     5819 2023-06-22 09:43:14.446510 voicemeeter_api-2.1.1/voicemeeterlib/config.py
--rw-r--r--   0        0        0     1748 2022-07-07 14:44:58.387087 voicemeeter_api-2.1.1/voicemeeterlib/device.py
--rw-r--r--   0        0        0      273 2023-06-23 00:41:14.485078 voicemeeter_api-2.1.1/voicemeeterlib/error.py
--rw-r--r--   0        0        0     2099 2023-06-22 08:38:58.271443 voicemeeter_api-2.1.1/voicemeeterlib/event.py
--rw-r--r--   0        0        0     7792 2023-06-29 15:52:06.128626 voicemeeter_api-2.1.1/voicemeeterlib/factory.py
--rw-r--r--   0        0        0     1091 2023-06-22 23:31:40.238138 voicemeeter_api-2.1.1/voicemeeterlib/inst.py
--rw-r--r--   0        0        0     1800 2023-06-23 20:52:02.185334 voicemeeter_api-2.1.1/voicemeeterlib/iremote.py
--rw-r--r--   0        0        0     2352 2023-06-22 02:21:02.337418 voicemeeter_api-2.1.1/voicemeeterlib/kinds.py
--rw-r--r--   0        0        0     1063 2023-06-22 23:31:57.569332 voicemeeter_api-2.1.1/voicemeeterlib/macrobutton.py
--rw-r--r--   0        0        0     1130 2023-06-21 12:24:03.433043 voicemeeter_api-2.1.1/voicemeeterlib/meta.py
--rw-r--r--   0        0        0     6485 2023-07-01 18:51:25.725768 voicemeeter_api-2.1.1/voicemeeterlib/misc.py
--rw-r--r--   0        0        0     6739 2023-07-01 18:30:01.004734 voicemeeter_api-2.1.1/voicemeeterlib/recorder.py
--rw-r--r--   0        0        0    11082 2023-06-29 17:03:12.450592 voicemeeter_api-2.1.1/voicemeeterlib/remote.py
--rw-r--r--   0        0        0    15325 2023-06-23 19:51:13.562428 voicemeeter_api-2.1.1/voicemeeterlib/strip.py
--rw-r--r--   0        0        0     2277 2023-06-23 16:22:05.659320 voicemeeter_api-2.1.1/voicemeeterlib/subject.py
--rw-r--r--   0        0        0     2978 2023-06-25 02:33:59.383974 voicemeeter_api-2.1.1/voicemeeterlib/updater.py
--rw-r--r--   0        0        0     1971 2023-06-30 17:58:26.046029 voicemeeter_api-2.1.1/voicemeeterlib/util.py
--rw-r--r--   0        0        0     4650 2023-07-01 18:51:25.726767 voicemeeter_api-2.1.1/voicemeeterlib/vban.py
--rw-r--r--   0        0        0    17226 1970-01-01 00:00:00.000000 voicemeeter_api-2.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1091 2022-06-16 12:51:04.818279 voicemeeter_api-2.1.2/LICENSE
+-rw-r--r--   0        0        0     1111 2023-07-08 06:49:33.599926 voicemeeter_api-2.1.2/pyproject.toml
+-rw-r--r--   0        0        0    17394 2023-07-01 19:24:29.927689 voicemeeter_api-2.1.2/README.md
+-rw-r--r--   0        0        0       69 2022-07-31 06:38:44.483821 voicemeeter_api-2.1.2/voicemeeterlib/__init__.py
+-rw-r--r--   0        0        0     8226 2023-06-23 19:51:19.906407 voicemeeter_api-2.1.2/voicemeeterlib/bus.py
+-rw-r--r--   0        0        0     4239 2023-06-22 23:20:33.622570 voicemeeter_api-2.1.2/voicemeeterlib/cbindings.py
+-rw-r--r--   0        0        0     1194 2023-06-22 23:31:24.097081 voicemeeter_api-2.1.2/voicemeeterlib/command.py
+-rw-r--r--   0        0        0     5819 2023-06-22 09:43:14.446510 voicemeeter_api-2.1.2/voicemeeterlib/config.py
+-rw-r--r--   0        0        0     1748 2022-07-07 14:44:58.387087 voicemeeter_api-2.1.2/voicemeeterlib/device.py
+-rw-r--r--   0        0        0      273 2023-06-23 00:41:14.485078 voicemeeter_api-2.1.2/voicemeeterlib/error.py
+-rw-r--r--   0        0        0     2099 2023-06-22 08:38:58.271443 voicemeeter_api-2.1.2/voicemeeterlib/event.py
+-rw-r--r--   0        0        0     7792 2023-06-29 15:52:06.128626 voicemeeter_api-2.1.2/voicemeeterlib/factory.py
+-rw-r--r--   0        0        0     1091 2023-06-22 23:31:40.238138 voicemeeter_api-2.1.2/voicemeeterlib/inst.py
+-rw-r--r--   0        0        0     1800 2023-06-23 20:52:02.185334 voicemeeter_api-2.1.2/voicemeeterlib/iremote.py
+-rw-r--r--   0        0        0     2352 2023-06-22 02:21:02.337418 voicemeeter_api-2.1.2/voicemeeterlib/kinds.py
+-rw-r--r--   0        0        0     1063 2023-06-22 23:31:57.569332 voicemeeter_api-2.1.2/voicemeeterlib/macrobutton.py
+-rw-r--r--   0        0        0     1130 2023-06-21 12:24:03.433043 voicemeeter_api-2.1.2/voicemeeterlib/meta.py
+-rw-r--r--   0        0        0     6485 2023-07-01 18:51:25.725768 voicemeeter_api-2.1.2/voicemeeterlib/misc.py
+-rw-r--r--   0        0        0     6739 2023-07-01 18:30:01.004734 voicemeeter_api-2.1.2/voicemeeterlib/recorder.py
+-rw-r--r--   0        0        0    11145 2023-07-08 06:48:45.639873 voicemeeter_api-2.1.2/voicemeeterlib/remote.py
+-rw-r--r--   0        0        0    15325 2023-06-23 19:51:13.562428 voicemeeter_api-2.1.2/voicemeeterlib/strip.py
+-rw-r--r--   0        0        0     2277 2023-06-23 16:22:05.659320 voicemeeter_api-2.1.2/voicemeeterlib/subject.py
+-rw-r--r--   0        0        0     2978 2023-06-25 02:33:59.383974 voicemeeter_api-2.1.2/voicemeeterlib/updater.py
+-rw-r--r--   0        0        0     1971 2023-06-30 17:58:26.046029 voicemeeter_api-2.1.2/voicemeeterlib/util.py
+-rw-r--r--   0        0        0     4650 2023-07-01 18:51:25.726767 voicemeeter_api-2.1.2/voicemeeterlib/vban.py
+-rw-r--r--   0        0        0    17226 1970-01-01 00:00:00.000000 voicemeeter_api-2.1.2/PKG-INFO
```

### Comparing `voicemeeter_api-2.1.1/LICENSE` & `voicemeeter_api-2.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `voicemeeter_api-2.1.1/pyproject.toml` & `voicemeeter_api-2.1.2/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "voicemeeter-api"
-version = "2.1.1"
+version = "2.1.2"
 description = "A Python wrapper for the Voiceemeter API"
 authors = ["onyx-and-iris <code@onyxandiris.online>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/onyx-and-iris/voicemeeter-api-python"
 
 packages = [
```

### Comparing `voicemeeter_api-2.1.1/README.md` & `voicemeeter_api-2.1.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -401,15 +401,15 @@
 -   `load(filepath)`: raw string
 -   `goto(time_string)`: time string in format `hh:mm:ss`
 -   `filetype(filetype)`: string, ("wav", "aiff", "bwf", "mp3")
 
 The following properties are available
 
 -   `A1 - A5`: boolean
--   `B1 - A3`: boolean
+-   `B1 - B3`: boolean
 -   `samplerate`: int, (22050, 24000, 32000, 44100, 48000, 88200, 96000, 176400, 192000)
 -   `bitresolution`: int, (8, 16, 24, 32)
 -   `channel`: int, from 1 to 8
 -   `kbps`: int, (32, 40, 48, 56, 64, 80, 96, 112, 128, 160, 192, 224, 256, 320)
 -   `gain`: float, from -60.0 to 12.0
 
 example:
```

### Comparing `voicemeeter_api-2.1.1/voicemeeterlib/bus.py` & `voicemeeter_api-2.1.2/voicemeeterlib/bus.py`

 * *Files identical despite different names*

### Comparing `voicemeeter_api-2.1.1/voicemeeterlib/cbindings.py` & `voicemeeter_api-2.1.2/voicemeeterlib/cbindings.py`

 * *Files identical despite different names*

### Comparing `voicemeeter_api-2.1.1/voicemeeterlib/command.py` & `voicemeeter_api-2.1.2/voicemeeterlib/command.py`

 * *Files identical despite different names*

### Comparing `voicemeeter_api-2.1.1/voicemeeterlib/config.py` & `voicemeeter_api-2.1.2/voicemeeterlib/config.py`

 * *Files identical despite different names*

### Comparing `voicemeeter_api-2.1.1/voicemeeterlib/device.py` & `voicemeeter_api-2.1.2/voicemeeterlib/device.py`

 * *Files identical despite different names*

### Comparing `voicemeeter_api-2.1.1/voicemeeterlib/event.py` & `voicemeeter_api-2.1.2/voicemeeterlib/event.py`

 * *Files identical despite different names*

### Comparing `voicemeeter_api-2.1.1/voicemeeterlib/factory.py` & `voicemeeter_api-2.1.2/voicemeeterlib/factory.py`

 * *Files identical despite different names*

### Comparing `voicemeeter_api-2.1.1/voicemeeterlib/inst.py` & `voicemeeter_api-2.1.2/voicemeeterlib/inst.py`

 * *Files identical despite different names*

### Comparing `voicemeeter_api-2.1.1/voicemeeterlib/iremote.py` & `voicemeeter_api-2.1.2/voicemeeterlib/iremote.py`

 * *Files identical despite different names*

### Comparing `voicemeeter_api-2.1.1/voicemeeterlib/kinds.py` & `voicemeeter_api-2.1.2/voicemeeterlib/kinds.py`

 * *Files identical despite different names*

### Comparing `voicemeeter_api-2.1.1/voicemeeterlib/macrobutton.py` & `voicemeeter_api-2.1.2/voicemeeterlib/macrobutton.py`

 * *Files identical despite different names*

### Comparing `voicemeeter_api-2.1.1/voicemeeterlib/meta.py` & `voicemeeter_api-2.1.2/voicemeeterlib/meta.py`

 * *Files identical despite different names*

### Comparing `voicemeeter_api-2.1.1/voicemeeterlib/misc.py` & `voicemeeter_api-2.1.2/voicemeeterlib/misc.py`

 * *Files identical despite different names*

### Comparing `voicemeeter_api-2.1.1/voicemeeterlib/recorder.py` & `voicemeeter_api-2.1.2/voicemeeterlib/recorder.py`

 * *Files identical despite different names*

### Comparing `voicemeeter_api-2.1.1/voicemeeterlib/remote.py` & `voicemeeter_api-2.1.2/voicemeeterlib/remote.py`

 * *Files 4% similar despite different names*

```diff
@@ -282,16 +282,17 @@
         error_msg = (
             f"No config with name '{name}' is loaded into memory",
             f"Known configs: {list(self.configs.keys())}",
         )
         try:
             self.apply(self.configs[name])
             self.logger.info(f"Profile '{name}' applied!")
-        except KeyError:
+        except KeyError as e:
             self.logger.error(("\n").join(error_msg))
+            raise VMError(("\n").join(error_msg)) from e
 
     def logout(self) -> NoReturn:
         """Wait for dirty parameters to clear, then logout of the API"""
         self.clear_dirty()
         time.sleep(0.1)
         self.call(self.vm_logout)
         self.logger.info(f"{type(self).__name__}: Successfully logged out of {self}")
```

### Comparing `voicemeeter_api-2.1.1/voicemeeterlib/strip.py` & `voicemeeter_api-2.1.2/voicemeeterlib/strip.py`

 * *Files identical despite different names*

### Comparing `voicemeeter_api-2.1.1/voicemeeterlib/subject.py` & `voicemeeter_api-2.1.2/voicemeeterlib/subject.py`

 * *Files identical despite different names*

### Comparing `voicemeeter_api-2.1.1/voicemeeterlib/updater.py` & `voicemeeter_api-2.1.2/voicemeeterlib/updater.py`

 * *Files identical despite different names*

### Comparing `voicemeeter_api-2.1.1/voicemeeterlib/util.py` & `voicemeeter_api-2.1.2/voicemeeterlib/util.py`

 * *Files identical despite different names*

### Comparing `voicemeeter_api-2.1.1/voicemeeterlib/vban.py` & `voicemeeter_api-2.1.2/voicemeeterlib/vban.py`

 * *Files identical despite different names*

### Comparing `voicemeeter_api-2.1.1/PKG-INFO` & `voicemeeter_api-2.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: voicemeeter-api
-Version: 2.1.1
+Version: 2.1.2
 Summary: A Python wrapper for the Voiceemeter API
 Home-page: https://github.com/onyx-and-iris/voicemeeter-api-python
 License: MIT
 Author: onyx-and-iris
 Author-email: code@onyxandiris.online
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -418,15 +418,15 @@
 -   `load(filepath)`: raw string
 -   `goto(time_string)`: time string in format `hh:mm:ss`
 -   `filetype(filetype)`: string, ("wav", "aiff", "bwf", "mp3")
 
 The following properties are available
 
 -   `A1 - A5`: boolean
--   `B1 - A3`: boolean
+-   `B1 - B3`: boolean
 -   `samplerate`: int, (22050, 24000, 32000, 44100, 48000, 88200, 96000, 176400, 192000)
 -   `bitresolution`: int, (8, 16, 24, 32)
 -   `channel`: int, from 1 to 8
 -   `kbps`: int, (32, 40, 48, 56, 64, 80, 96, 112, 128, 160, 192, 224, 256, 320)
 -   `gain`: float, from -60.0 to 12.0
 
 example:
```

