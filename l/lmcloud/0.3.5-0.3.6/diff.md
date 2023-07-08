# Comparing `tmp/lmcloud-0.3.5.tar.gz` & `tmp/lmcloud-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lmcloud-0.3.5.tar", last modified: Thu Jul  6 10:51:41 2023, max compression
+gzip compressed data, was "lmcloud-0.3.6.tar", last modified: Sat Jul  8 12:25:18 2023, max compression
```

## Comparing `lmcloud-0.3.5.tar` & `lmcloud-0.3.6.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:51:41.232125 lmcloud-0.3.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-07-06 10:51:27.000000 lmcloud-0.3.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5994 2023-07-06 10:51:41.232125 lmcloud-0.3.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5342 2023-07-06 10:51:27.000000 lmcloud-0.3.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:51:41.232125 lmcloud-0.3.5/lmcloud/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-06 10:51:27.000000 lmcloud-0.3.5/lmcloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-06 10:51:27.000000 lmcloud-0.3.5/lmcloud/const.py
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-07-06 10:51:27.000000 lmcloud-0.3.5/lmcloud/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-07-06 10:51:27.000000 lmcloud-0.3.5/lmcloud/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4814 2023-07-06 10:51:27.000000 lmcloud-0.3.5/lmcloud/lmbluetooth.py
--rw-r--r--   0 runner    (1001) docker     (123)    22263 2023-07-06 10:51:27.000000 lmcloud-0.3.5/lmcloud/lmcloud.py
--rw-r--r--   0 runner    (1001) docker     (123)     3927 2023-07-06 10:51:27.000000 lmcloud-0.3.5/lmcloud/lmlocalapi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:51:41.232125 lmcloud-0.3.5/lmcloud.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5994 2023-07-06 10:51:41.000000 lmcloud-0.3.5/lmcloud.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-07-06 10:51:41.000000 lmcloud-0.3.5/lmcloud.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 10:51:41.000000 lmcloud-0.3.5/lmcloud.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-06 10:51:41.000000 lmcloud-0.3.5/lmcloud.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-06 10:51:41.000000 lmcloud-0.3.5/lmcloud.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 10:51:41.232125 lmcloud-0.3.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-07-06 10:51:27.000000 lmcloud-0.3.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 12:25:18.830167 lmcloud-0.3.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-07-08 12:25:02.000000 lmcloud-0.3.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5994 2023-07-08 12:25:18.830167 lmcloud-0.3.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5342 2023-07-08 12:25:02.000000 lmcloud-0.3.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 12:25:18.830167 lmcloud-0.3.6/lmcloud/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-08 12:25:02.000000 lmcloud-0.3.6/lmcloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-08 12:25:02.000000 lmcloud-0.3.6/lmcloud/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-07-08 12:25:02.000000 lmcloud-0.3.6/lmcloud/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-07-08 12:25:02.000000 lmcloud-0.3.6/lmcloud/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4814 2023-07-08 12:25:02.000000 lmcloud-0.3.6/lmcloud/lmbluetooth.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22549 2023-07-08 12:25:02.000000 lmcloud-0.3.6/lmcloud/lmcloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4025 2023-07-08 12:25:02.000000 lmcloud-0.3.6/lmcloud/lmlocalapi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 12:25:18.830167 lmcloud-0.3.6/lmcloud.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5994 2023-07-08 12:25:18.000000 lmcloud-0.3.6/lmcloud.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-07-08 12:25:18.000000 lmcloud-0.3.6/lmcloud.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 12:25:18.000000 lmcloud-0.3.6/lmcloud.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-08 12:25:18.000000 lmcloud-0.3.6/lmcloud.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-08 12:25:18.000000 lmcloud-0.3.6/lmcloud.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 12:25:18.830167 lmcloud-0.3.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-07-08 12:25:02.000000 lmcloud-0.3.6/setup.py
```

### Comparing `lmcloud-0.3.5/LICENSE` & `lmcloud-0.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `lmcloud-0.3.5/PKG-INFO` & `lmcloud-0.3.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lmcloud
-Version: 0.3.5
+Version: 0.3.6
 Summary: A Python implementation of the new La Marzocco API
 Home-page: https://github.com/zweckj/lmcloud
 Author: Josef Zweck
 Author-email: 24647999+zweckj@users.noreply.github.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `lmcloud-0.3.5/README.md` & `lmcloud-0.3.6/README.md`

 * *Files identical despite different names*

### Comparing `lmcloud-0.3.5/lmcloud/const.py` & `lmcloud-0.3.6/lmcloud/const.py`

 * *Files identical despite different names*

### Comparing `lmcloud-0.3.5/lmcloud/helpers.py` & `lmcloud-0.3.6/lmcloud/helpers.py`

 * *Files identical despite different names*

### Comparing `lmcloud-0.3.5/lmcloud/lmbluetooth.py` & `lmcloud-0.3.6/lmcloud/lmbluetooth.py`

 * *Files identical despite different names*

### Comparing `lmcloud-0.3.5/lmcloud/lmcloud.py` & `lmcloud-0.3.6/lmcloud/lmcloud.py`

 * *Files 1% similar despite different names*

```diff
@@ -132,31 +132,37 @@
 
 
     @classmethod
     async def create(cls, credentials):
         '''
         Initialize a cloud only client
         '''
-
         self = cls()
         self.client = await self._connect(credentials)
         self._machine_info = await self._get_machine_info()
         self._gw_url_with_serial = GW_MACHINE_BASE_URL + "/" + self.machine_info[SERIAL_NUMBER]
         self._firmware = await self.get_firmware()
         await self.update_local_machine_status()
         return self
 
 
     @classmethod
     async def create_with_local_api(cls, credentials, ip, port=8081, use_websocket=False, use_bluetooth=False, bluetooth_scanner=None):
         '''
         Also initialize a local API client
         '''
-
         self = cls()
+        self.init_with_local_api(credentials, ip, port, use_websocket, use_bluetooth, bluetooth_scanner)
+
+        await self.update_local_machine_status(in_init=True)
+        return self
+    
+
+    async def init_with_local_api(self, credentials, ip, port=8081, use_websocket=False, use_bluetooth=False, bluetooth_scanner=None):
+        ''' init where data is loaded '''
         self.client = await self._connect(credentials)
         self._machine_info = await self._get_machine_info()
         self._lm_local_api = LMLocalAPI(local_ip=ip, local_port=port, local_bearer=self.machine_info[KEY])
         self._gw_url_with_serial = GW_MACHINE_BASE_URL + "/" + self.machine_info[SERIAL_NUMBER]
         self._firmware = await self.get_firmware()
 
         # init websockets if set
@@ -174,17 +180,14 @@
             except BluetoothDeviceNotFound as e:
                 _logger.warn(f"Could not find bluetooth device. Bluetooth commands will not be available and commands will all be sent through cloud.")
                 _logger.debug(f"Full error: {e}")
             except BleakError as e:
                 _logger.warn(f"Bleak encountered an error while trying to connect to bluetooth device. \
                              Maybe no bluetooth adapter is available? Bluetooth commands will not be available and commands will all be sent through cloud.")
                 _logger.debug(f"Full error: {e}")
-
-        await self.update_local_machine_status(in_init=True)
-        return self
         
 
     async def _connect(self, credentials):
         '''
         Establish connection by building the OAuth client and requesting the token
         '''
```

### Comparing `lmcloud-0.3.5/lmcloud/lmlocalapi.py` & `lmcloud-0.3.6/lmcloud/lmlocalapi.py`

 * *Files 7% similar despite different names*

```diff
@@ -52,46 +52,48 @@
     async def local_get_config(self):
         headers = {"Authorization": f"Bearer {self._local_bearer}"}
         async with aiohttp.ClientSession(headers=headers) as session:
             async with session.get(f"http://{self._local_ip}:{self._local_port}/api/v1/config") as response:
                 if response.status == 200:
                     return await response.json()
                 
-    async def websocket_connect(self):
+    async def websocket_connect(self, callback = None):
         headers = {"Authorization": f"Bearer {self._local_bearer}"}
         async for websocket in websockets.connect(f"ws://{self._local_ip}:{self._local_port}/api/v1/streaming", extra_headers=headers):
             try:
                 # Close the connection when receiving SIGTERM.
                 loop = asyncio.get_running_loop()
                 loop.add_signal_handler(
                     signal.SIGTERM, loop.create_task, websocket.close())
 
                 # Process messages received on the connection.
                 async for message in websocket:
                     await self.handle_websocket_message(message)
+                    if callback:
+                        callback(self._status)
             except websockets.ConnectionClosed:
                 await asyncio.sleep(20) # wait 20 seconds before trying to reconnect
                 continue
             except Exception as e:
                 _logger.error(f"Error during websocket connection: {e}")
                 await asyncio.sleep(20)
                 continue
 
     async def handle_websocket_message(self, message):
         try:
             self._timestamp_last_websocket_msg = datetime.now()
             message = json.loads(message)
-            # if type(message) is dict:
-            #     if message["name"] == "SteamBoilerUpdateTemperature":
-            #         self._status[STEAM_TEMP] = message["value"]
-            #     elif message["name"] == "CoffeeBoiler1UpdateTemperature":
-            #         self._status[COFFEE_TEMP] = message["value"]
-            #     elif message["name"] == "MachineConfiguration":
-            #         self._full_config = message["value"]
-            #         self._status[TANK_LEVEL] = message["value"]
+            if type(message) is dict:
+                if message["name"] == "SteamBoilerUpdateTemperature":
+                    self._status["SteamTemperature"] = message["value"]
+                elif message["name"] == "CoffeeBoiler1UpdateTemperature":
+                    self._status["CoffeeTemperature"] = message["value"]
+                elif message["name"] == "MachineConfiguration":
+                    self._full_config = message["value"]
+                    self._status["TankLevel"] = message["value"]
             if type(message) is list:
                 if message[0]["name"] == "BrewingUpdateGroup1Time":
                     self._status[ACTIVE_BREW_DURATION] = message[0]["value"]
                 elif message[0]["name"] in ["BrewingStartedGroup1StopType", "BrewingStartedGroup1DoseIndex"]:
                     # started active brew
                     self._status[ACTIVE_BREW] = True
                 elif message[0]["name"] in ["BrewingSnapshotGroup1", "FlushStoppedGroup1DoseIndex", "FlushStoppedGroup1Time"]:
```

### Comparing `lmcloud-0.3.5/lmcloud.egg-info/PKG-INFO` & `lmcloud-0.3.6/lmcloud.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lmcloud
-Version: 0.3.5
+Version: 0.3.6
 Summary: A Python implementation of the new La Marzocco API
 Home-page: https://github.com/zweckj/lmcloud
 Author: Josef Zweck
 Author-email: 24647999+zweckj@users.noreply.github.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `lmcloud-0.3.5/setup.py` & `lmcloud-0.3.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as f:
     readme = f.read()
 
 setuptools.setup(
     name="lmcloud",
-    version="0.3.5",
+    version="0.3.6",
     description="A Python implementation of the new La Marzocco API",
     long_description=readme,
     long_description_content_type="text/markdown",
     url="https://github.com/zweckj/lmcloud",
     author="Josef Zweck",
     author_email="24647999+zweckj@users.noreply.github.com",
     license="MIT",
```

