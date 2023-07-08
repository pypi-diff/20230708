# Comparing `tmp/unifi_protect_backup-0.9.2.tar.gz` & `tmp/unifi_protect_backup-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unifi_protect_backup-0.9.2.tar", max compression
+gzip compressed data, was "unifi_protect_backup-0.9.3.tar", max compression
```

## Comparing `unifi_protect_backup-0.9.2.tar` & `unifi_protect_backup-0.9.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1074 2023-05-23 23:45:52.955222 unifi_protect_backup-0.9.2/LICENSE
--rw-r--r--   0        0        0    17222 2023-05-23 23:45:52.955222 unifi_protect_backup-0.9.2/README.md
--rw-r--r--   0        0        0     2110 2023-05-23 23:45:52.959222 unifi_protect_backup-0.9.2/pyproject.toml
--rw-r--r--   0        0        0       50 2023-05-23 23:45:52.959222 unifi_protect_backup-0.9.2/tests/__init__.py
--rw-r--r--   0        0        0     1031 2023-05-23 23:45:52.959222 unifi_protect_backup-0.9.2/tests/test_unifi_protect_backup.py
--rw-r--r--   0        0        0      359 2023-05-23 23:45:52.959222 unifi_protect_backup-0.9.2/unifi_protect_backup/__init__.py
--rw-r--r--   0        0        0     6416 2023-05-23 23:45:52.959222 unifi_protect_backup-0.9.2/unifi_protect_backup/cli.py
--rw-r--r--   0        0        0     8972 2023-05-23 23:45:52.959222 unifi_protect_backup-0.9.2/unifi_protect_backup/downloader.py
--rw-r--r--   0        0        0     5277 2023-05-23 23:45:52.959222 unifi_protect_backup-0.9.2/unifi_protect_backup/event_listener.py
--rw-r--r--   0        0        0     6589 2023-05-23 23:45:52.959222 unifi_protect_backup-0.9.2/unifi_protect_backup/missing_event_checker.py
--rw-r--r--   0        0        0      540 2023-05-23 23:45:52.959222 unifi_protect_backup-0.9.2/unifi_protect_backup/notifications.py
--rw-r--r--   0        0        0     3682 2023-05-23 23:45:52.959222 unifi_protect_backup-0.9.2/unifi_protect_backup/purge.py
--rw-r--r--   0        0        0    12499 2023-05-23 23:45:52.959222 unifi_protect_backup-0.9.2/unifi_protect_backup/unifi_protect_backup_core.py
--rw-r--r--   0        0        0     6365 2023-05-23 23:45:52.959222 unifi_protect_backup-0.9.2/unifi_protect_backup/uploader.py
--rw-r--r--   0        0        0    16583 2023-05-23 23:45:52.959222 unifi_protect_backup-0.9.2/unifi_protect_backup/utils.py
--rw-r--r--   0        0        0    18258 1970-01-01 00:00:00.000000 unifi_protect_backup-0.9.2/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-07-08 16:39:29.001762 unifi_protect_backup-0.9.3/LICENSE
+-rw-r--r--   0        0        0    17222 2023-07-08 16:39:29.001762 unifi_protect_backup-0.9.3/README.md
+-rw-r--r--   0        0        0     2131 2023-07-08 16:39:29.001762 unifi_protect_backup-0.9.3/pyproject.toml
+-rw-r--r--   0        0        0       50 2023-07-08 16:39:29.001762 unifi_protect_backup-0.9.3/tests/__init__.py
+-rw-r--r--   0        0        0     1031 2023-07-08 16:39:29.001762 unifi_protect_backup-0.9.3/tests/test_unifi_protect_backup.py
+-rw-r--r--   0        0        0      359 2023-07-08 16:39:29.001762 unifi_protect_backup-0.9.3/unifi_protect_backup/__init__.py
+-rw-r--r--   0        0        0     6416 2023-07-08 16:39:29.001762 unifi_protect_backup-0.9.3/unifi_protect_backup/cli.py
+-rw-r--r--   0        0        0     9087 2023-07-08 16:39:29.001762 unifi_protect_backup-0.9.3/unifi_protect_backup/downloader.py
+-rw-r--r--   0        0        0     5371 2023-07-08 16:39:29.001762 unifi_protect_backup-0.9.3/unifi_protect_backup/event_listener.py
+-rw-r--r--   0        0        0     6704 2023-07-08 16:39:29.001762 unifi_protect_backup-0.9.3/unifi_protect_backup/missing_event_checker.py
+-rw-r--r--   0        0        0      540 2023-07-08 16:39:29.001762 unifi_protect_backup-0.9.3/unifi_protect_backup/notifications.py
+-rw-r--r--   0        0        0     3682 2023-07-08 16:39:29.001762 unifi_protect_backup-0.9.3/unifi_protect_backup/purge.py
+-rw-r--r--   0        0        0    12747 2023-07-08 16:39:29.005762 unifi_protect_backup-0.9.3/unifi_protect_backup/unifi_protect_backup_core.py
+-rw-r--r--   0        0        0     6365 2023-07-08 16:39:29.005762 unifi_protect_backup-0.9.3/unifi_protect_backup/uploader.py
+-rw-r--r--   0        0        0    16858 2023-07-08 16:39:29.005762 unifi_protect_backup-0.9.3/unifi_protect_backup/utils.py
+-rw-r--r--   0        0        0    18300 1970-01-01 00:00:00.000000 unifi_protect_backup-0.9.3/PKG-INFO
```

### Comparing `unifi_protect_backup-0.9.2/LICENSE` & `unifi_protect_backup-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `unifi_protect_backup-0.9.2/README.md` & `unifi_protect_backup-0.9.3/README.md`

 * *Files identical despite different names*

### Comparing `unifi_protect_backup-0.9.2/pyproject.toml` & `unifi_protect_backup-0.9.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool]
 [tool.poetry]
 name = "unifi_protect_backup"
-version = "0.9.2"
+version = "0.9.3"
 homepage = "https://github.com/ep1cman/unifi-protect-backup"
 description = "Python tool to backup unifi event clips in realtime."
 authors = ["sebastian.goscik <sebastian@goscik.com>"]
 readme = "README.md"
 license =  "MIT"
 classifiers=[
     'Development Status :: 5 - Production/Stable',
@@ -25,14 +25,15 @@
 click = "8.0.1"
 pyunifiprotect = "^4.0.11"
 aiorun = "^2022.11.1"
 aiosqlite = "^0.17.0"
 python-dateutil = "^2.8.2"
 apprise = "^1.3.0"
 expiring-dict = "^1.1.0"
+async-lru = "^2.0.3"
 
 [tool.poetry.group.dev]
 optional = true
 
 [tool.poetry.group.dev.dependencies]
 black  = "^22.10.0"
 isort  = "^5.8.0"
```

### Comparing `unifi_protect_backup-0.9.2/tests/test_unifi_protect_backup.py` & `unifi_protect_backup-0.9.3/tests/test_unifi_protect_backup.py`

 * *Files identical despite different names*

### Comparing `unifi_protect_backup-0.9.2/unifi_protect_backup/cli.py` & `unifi_protect_backup-0.9.3/unifi_protect_backup/cli.py`

 * *Files identical despite different names*

### Comparing `unifi_protect_backup-0.9.2/unifi_protect_backup/downloader.py` & `unifi_protect_backup-0.9.3/unifi_protect_backup/downloader.py`

 * *Files 2% similar despite different names*

```diff
@@ -78,14 +78,17 @@
             self._has_ffprobe = False
 
     async def start(self):
         """Main loop."""
         self.logger.info("Starting Downloader")
         while True:
             try:
+                # Wait for unifi protect to be connected
+                await self._protect.connect_event.wait()
+
                 event = await self.download_queue.get()
                 self.current_event = event
                 self.logger = logging.LoggerAdapter(self.base_logger, {'event': f' [{event.id}]'})
 
                 # Fix timezones since pyunifiprotect sets all timestamps to UTC. Instead localize them to
                 # the timezone of the unifi protect NVR.
                 event.start = event.start.replace(tzinfo=pytz.utc).astimezone(self._protect.bootstrap.nvr.timezone)
```

### Comparing `unifi_protect_backup-0.9.2/unifi_protect_backup/event_listener.py` & `unifi_protect_backup-0.9.3/unifi_protect_backup/event_listener.py`

 * *Files 8% similar despite different names*

```diff
@@ -96,14 +96,15 @@
 
     async def _check_websocket_and_reconnect(self):
         """Checks for websocket disconnect and triggers a reconnect."""
         logger.extra_debug("Checking the status of the websocket...")
         if self._protect.check_ws():
             logger.extra_debug("Websocket is connected.")
         else:
+            self._protect.connect_event.clear()
             logger.warning("Lost connection to Unifi Protect.")
 
             # Unsubscribe, close the session.
             self._unsub()
             await self._protect.close_session()
 
             while True:
@@ -121,8 +122,9 @@
                         logger.error("Unable to establish connection to Unifi Protect")
                 except Exception as e:
                     logger.error("Unexpected exception occurred while trying to reconnect:", exc_info=e)
 
                 # Back off for a little while
                 await asyncio.sleep(10)
 
+            self._protect.connect_event.set()
             logger.info("Re-established connection to Unifi Protect and to the websocket.")
```

### Comparing `unifi_protect_backup-0.9.2/unifi_protect_backup/missing_event_checker.py` & `unifi_protect_backup-0.9.3/unifi_protect_backup/missing_event_checker.py`

 * *Files 2% similar despite different names*

```diff
@@ -119,14 +119,17 @@
         await self._db.commit()
 
     async def start(self):
         """Main loop."""
         logger.info("Starting Missing Event Checker")
         while True:
             try:
+                # Wait for unifi protect to be connected
+                await self._protect.connect_event.wait()
+
                 logger.extra_debug("Running check for missing events...")
 
                 wanted_events = await self._get_missing_events()
 
                 logger.debug(f" Undownloaded events of wanted types: {len(wanted_events)}")
 
                 if len(wanted_events) > 20:
```

### Comparing `unifi_protect_backup-0.9.2/unifi_protect_backup/notifications.py` & `unifi_protect_backup-0.9.3/unifi_protect_backup/notifications.py`

 * *Files identical despite different names*

### Comparing `unifi_protect_backup-0.9.2/unifi_protect_backup/purge.py` & `unifi_protect_backup-0.9.3/unifi_protect_backup/purge.py`

 * *Files identical despite different names*

### Comparing `unifi_protect_backup-0.9.2/unifi_protect_backup/unifi_protect_backup_core.py` & `unifi_protect_backup-0.9.3/unifi_protect_backup/unifi_protect_backup_core.py`

 * *Files 2% similar despite different names*

```diff
@@ -189,14 +189,19 @@
                     break
                 except Exception as e:
                     logger.warning(f"Failed to connect to UniFi Protect, retrying in {attempts}s...", exc_info=e)
                     await asyncio.sleep(attempts)
             else:
                 raise ConnectionError("Failed to connect to UniFi Protect after 10 attempts")
 
+            # Add a lock to the protect client that can be used to prevent code accessing the client when it has
+            # lost connection
+            self._protect.connect_event = asyncio.Event()
+            self._protect.connect_event.set()
+
             # Get a mapping of camera ids -> names
             logger.info("Found cameras:")
             for camera in self._protect.bootstrap.cameras.values():
                 logger.info(f" - {camera.id}: {camera.name}")
 
             # Print timezone info for debugging
             logger.debug(f'NVR TZ: {self._protect.bootstrap.nvr.timezone}')
```

### Comparing `unifi_protect_backup-0.9.2/unifi_protect_backup/uploader.py` & `unifi_protect_backup-0.9.3/unifi_protect_backup/uploader.py`

 * *Files identical despite different names*

### Comparing `unifi_protect_backup-0.9.2/unifi_protect_backup/utils.py` & `unifi_protect_backup-0.9.3/unifi_protect_backup/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from datetime import datetime
 from typing import List, Optional
 
 from apprise import NotifyType
 from dateutil.relativedelta import relativedelta
 from pyunifiprotect import ProtectApiClient
 from pyunifiprotect.data.nvr import Event
+from async_lru import alru_cache
 
 from unifi_protect_backup import notifications
 
 logger = logging.getLogger(__name__)
 
 
 def add_logging_level(levelName: str, levelNum: int, methodName: Optional[str] = None) -> None:
@@ -273,19 +274,25 @@
 
     value = float(result[1])
     suffix = result[2]
     multiplier = 1024 ** _suffixes.index(suffix)
     return value * multiplier
 
 
+# Cached so that actions like uploads can continue when the connection to the api is lost
+# No max size, and a 6 hour ttl
+@alru_cache(None, ttl=60 * 60 * 6)
 async def get_camera_name(protect: ProtectApiClient, id: str):
     """Returns the name for the camera with the given ID.
 
     If the camera ID is not know, it tries refreshing the cached data
     """
+    # Wait for unifi protect to be connected
+    await protect.connect_event.wait()
+
     try:
         return protect.bootstrap.cameras[id].name
     except KeyError:
         # Refresh cameras
         logger.debug(f"Unknown camera id: '{id}', checking API")
 
         await protect.update(force=True)
```

### Comparing `unifi_protect_backup-0.9.2/PKG-INFO` & `unifi_protect_backup-0.9.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unifi-protect-backup
-Version: 0.9.2
+Version: 0.9.3
 Summary: Python tool to backup unifi event clips in realtime.
 Home-page: https://github.com/ep1cman/unifi-protect-backup
 License: MIT
 Author: sebastian.goscik
 Author-email: sebastian@goscik.com
 Requires-Python: >=3.9.0,<4.0
 Classifier: Development Status :: 5 - Production/Stable
@@ -14,14 +14,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aiorun (>=2022.11.1,<2023.0.0)
 Requires-Dist: aiosqlite (>=0.17.0,<0.18.0)
 Requires-Dist: apprise (>=1.3.0,<2.0.0)
+Requires-Dist: async-lru (>=2.0.3,<3.0.0)
 Requires-Dist: click (==8.0.1)
 Requires-Dist: expiring-dict (>=1.1.0,<2.0.0)
 Requires-Dist: python-dateutil (>=2.8.2,<3.0.0)
 Requires-Dist: pyunifiprotect (>=4.0.11,<5.0.0)
 Description-Content-Type: text/markdown
 
 # Unifi Protect Backup
```

