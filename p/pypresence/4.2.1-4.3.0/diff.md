# Comparing `tmp/pypresence-4.2.1.tar.gz` & `tmp/pypresence-4.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypresence-4.2.1.tar", last modified: Sat Nov 13 21:09:53 2021, max compression
+gzip compressed data, was "pypresence-4.3.0.tar", last modified: Sat Jul  8 00:33:51 2023, max compression
```

## Comparing `pypresence-4.2.1.tar` & `pypresence-4.3.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-13 21:09:53.458886 pypresence-4.2.1/
--rw-r--r--   0 runner    (1001) docker     (121)     1458 2021-11-13 21:09:44.000000 pypresence-4.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     3954 2021-11-13 21:09:53.458886 pypresence-4.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2728 2021-11-13 21:09:44.000000 pypresence-4.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-13 21:09:53.458886 pypresence-4.2.1/pypresence/
--rw-r--r--   0 runner    (1001) docker     (121)      385 2021-11-13 21:09:44.000000 pypresence-4.2.1/pypresence/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4520 2021-11-13 21:09:44.000000 pypresence-4.2.1/pypresence/baseclient.py
--rw-r--r--   0 runner    (1001) docker     (121)    15461 2021-11-13 21:09:44.000000 pypresence-4.2.1/pypresence/client.py
--rw-r--r--   0 runner    (1001) docker     (121)     1717 2021-11-13 21:09:44.000000 pypresence-4.2.1/pypresence/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)     8560 2021-11-13 21:09:44.000000 pypresence-4.2.1/pypresence/payloads.py
--rw-r--r--   0 runner    (1001) docker     (121)     3629 2021-11-13 21:09:44.000000 pypresence-4.2.1/pypresence/presence.py
--rw-r--r--   0 runner    (1001) docker     (121)     2056 2021-11-13 21:09:44.000000 pypresence-4.2.1/pypresence/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-13 21:09:53.458886 pypresence-4.2.1/pypresence.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3954 2021-11-13 21:09:53.000000 pypresence-4.2.1/pypresence.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      361 2021-11-13 21:09:53.000000 pypresence-4.2.1/pypresence.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-11-13 21:09:53.000000 pypresence-4.2.1/pypresence.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       11 2021-11-13 21:09:53.000000 pypresence-4.2.1/pypresence.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-11-13 21:09:53.000000 pypresence-4.2.1/pypresence.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      147 2021-11-13 21:09:53.458886 pypresence-4.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2026 2021-11-13 21:09:44.000000 pypresence-4.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:33:51.207905 pypresence-4.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-08 00:33:41.000000 pypresence-4.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3950 2023-07-08 00:33:51.207905 pypresence-4.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2675 2023-07-08 00:33:41.000000 pypresence-4.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:33:51.207905 pypresence-4.3.0/pypresence/
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-07-08 00:33:41.000000 pypresence-4.3.0/pypresence/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5056 2023-07-08 00:33:41.000000 pypresence-4.3.0/pypresence/baseclient.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15461 2023-07-08 00:33:41.000000 pypresence-4.3.0/pypresence/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-07-08 00:33:41.000000 pypresence-4.3.0/pypresence/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8560 2023-07-08 00:33:41.000000 pypresence-4.3.0/pypresence/payloads.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3642 2023-07-08 00:33:41.000000 pypresence-4.3.0/pypresence/presence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-07-08 00:33:41.000000 pypresence-4.3.0/pypresence/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:33:51.207905 pypresence-4.3.0/pypresence.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3950 2023-07-08 00:33:51.000000 pypresence-4.3.0/pypresence.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-07-08 00:33:51.000000 pypresence-4.3.0/pypresence.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 00:33:51.000000 pypresence-4.3.0/pypresence.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-08 00:33:51.000000 pypresence-4.3.0/pypresence.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 00:33:51.000000 pypresence-4.3.0/pypresence.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-07-08 00:33:51.207905 pypresence-4.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-07-08 00:33:41.000000 pypresence-4.3.0/setup.py
```

### Comparing `pypresence-4.2.1/PKG-INFO` & `pypresence-4.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypresence
-Version: 4.2.1
+Version: 4.3.0
 Summary: Discord RPC client written in Python
 Home-page: https://github.com/qwertyquerty/pypresence
 Author: qwertyquerty
 License: MIT
 Keywords: discord rich presence pypresence rpc api wrapper gamers chat irc
 Platform: Windows
 Platform: Linux
@@ -14,40 +14,32 @@
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Communications :: Chat
 Classifier: Framework :: AsyncIO
-Requires-Python: >=3.5
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 > A Discord Rich Presence Client in Python? Looks like you've come to the right place.
 
-Written by: [qwertyquerty](https://github.com/qwertyquerty)
-
-Notable Contributors: [GiovanniMCMXCIX](https://github.com/GiovanniMCMXCIX), [GhostofGoes](https://github.com/GhostofGoes)
-
 [![GitHub stars](https://img.shields.io/github/stars/qwertyquerty/pypresence.svg?style=for-the-badge&label=Stars)](https://github.com/qwertyquerty/pypresence) [![license](https://img.shields.io/github/license/qwertyquerty/pypresence.svg?style=for-the-badge)](https://github.com/qwertyquerty/pypresence/blob/master/LICENSE) ![GitHub last commit](https://img.shields.io/github/last-commit/qwertyquerty/pypresence.svg?style=for-the-badge) ![GitHub top language](https://img.shields.io/github/languages/top/qwertyquerty/pypresence.svg?style=for-the-badge) ![PyPI](https://img.shields.io/pypi/v/pypresence.svg?style=for-the-badge)
 
-
 ## NOTE: Only Python versions 3.8 and above are supported.
 
-
-## NOTICE: Activity() class has been removed in 4.0.0
-
-
 ### [Documentation](https://qwertyquerty.github.io/pypresence/html/index.html), [Discord Server](https://discord.gg/JF3kg77), [Patreon](https://www.patreon.com/qwertyquerty)
 
 ----------
 
 **Use this badge in your project's Readme to show you're using pypresence! The markdown code is below.**
 
 [![pypresence](https://img.shields.io/badge/using-pypresence-00bb88.svg?style=for-the-badge&logo=discord&logoWidth=20)](https://github.com/qwertyquerty/pypresence)
@@ -75,19 +67,22 @@
 
 
 # Documentation
 
 > **NOTE**: You need an **authorized app** to do anything besides rich presence!
 
 ####  [pypresence Documentation](https://qwertyquerty.github.io/pypresence/html/index.html)
-####  [Discord Rich Presence Documentation](https://discordapp.com/developers/docs/rich-presence/how-to)
-####  [Discord RPC Documentation](https://discordapp.com/developers/docs/topics/rpc)
+####  [Discord Rich Presence Documentation](https://discord.com/developers/docs/rich-presence/how-to)
+####  [Discord RPC Documentation](https://discord.com/developers/docs/topics/rpc)
 ####  [pyresence Discord Support Server](https://discord.gg/JF3kg77)
 ####  [Discord API Support Server](https://discord.gg/discord-api)
 
 ----------
 
 # Examples
 
 Examples can be found in the [examples](https://github.com/qwertyquerty/pypresence/tree/master/examples) directory, and you can contribute your own examples if you wish, just read [examples.md](https://github.com/qwertyquerty/pypresence/blob/master/examples/examples.md)!
 
+----------
+Written by: [qwertyquerty](https://github.com/qwertyquerty)
 
+Notable Contributors: [GiovanniMCMXCIX](https://github.com/GiovanniMCMXCIX), [GhostofGoes](https://github.com/GhostofGoes)
```

### Comparing `pypresence-4.2.1/README.md` & `pypresence-4.3.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,13 @@
 > A Discord Rich Presence Client in Python? Looks like you've come to the right place.
 
-Written by: [qwertyquerty](https://github.com/qwertyquerty)
-
-Notable Contributors: [GiovanniMCMXCIX](https://github.com/GiovanniMCMXCIX), [GhostofGoes](https://github.com/GhostofGoes)
-
 [![GitHub stars](https://img.shields.io/github/stars/qwertyquerty/pypresence.svg?style=for-the-badge&label=Stars)](https://github.com/qwertyquerty/pypresence) [![license](https://img.shields.io/github/license/qwertyquerty/pypresence.svg?style=for-the-badge)](https://github.com/qwertyquerty/pypresence/blob/master/LICENSE) ![GitHub last commit](https://img.shields.io/github/last-commit/qwertyquerty/pypresence.svg?style=for-the-badge) ![GitHub top language](https://img.shields.io/github/languages/top/qwertyquerty/pypresence.svg?style=for-the-badge) ![PyPI](https://img.shields.io/pypi/v/pypresence.svg?style=for-the-badge)
 
-
 ## NOTE: Only Python versions 3.8 and above are supported.
 
-
-## NOTICE: Activity() class has been removed in 4.0.0
-
-
 ### [Documentation](https://qwertyquerty.github.io/pypresence/html/index.html), [Discord Server](https://discord.gg/JF3kg77), [Patreon](https://www.patreon.com/qwertyquerty)
 
 ----------
 
 **Use this badge in your project's Readme to show you're using pypresence! The markdown code is below.**
 
 [![pypresence](https://img.shields.io/badge/using-pypresence-00bb88.svg?style=for-the-badge&logo=discord&logoWidth=20)](https://github.com/qwertyquerty/pypresence)
@@ -44,17 +35,22 @@
 
 
 # Documentation
 
 > **NOTE**: You need an **authorized app** to do anything besides rich presence!
 
 ####  [pypresence Documentation](https://qwertyquerty.github.io/pypresence/html/index.html)
-####  [Discord Rich Presence Documentation](https://discordapp.com/developers/docs/rich-presence/how-to)
-####  [Discord RPC Documentation](https://discordapp.com/developers/docs/topics/rpc)
+####  [Discord Rich Presence Documentation](https://discord.com/developers/docs/rich-presence/how-to)
+####  [Discord RPC Documentation](https://discord.com/developers/docs/topics/rpc)
 ####  [pyresence Discord Support Server](https://discord.gg/JF3kg77)
 ####  [Discord API Support Server](https://discord.gg/discord-api)
 
 ----------
 
 # Examples
 
 Examples can be found in the [examples](https://github.com/qwertyquerty/pypresence/tree/master/examples) directory, and you can contribute your own examples if you wish, just read [examples.md](https://github.com/qwertyquerty/pypresence/blob/master/examples/examples.md)!
+
+----------
+Written by: [qwertyquerty](https://github.com/qwertyquerty)
+
+Notable Contributors: [GiovanniMCMXCIX](https://github.com/GiovanniMCMXCIX), [GhostofGoes](https://github.com/GhostofGoes)
```

### Comparing `pypresence-4.2.1/pypresence/baseclient.py` & `pypresence-4.3.0/pypresence/baseclient.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,24 +12,22 @@
 from .payloads import Payload
 from .utils import get_ipc_path, get_event_loop
 
 
 class BaseClient:
 
     def __init__(self, client_id: str, **kwargs):
-        pipe = kwargs.get('pipe', None)
         loop = kwargs.get('loop', None)
         handler = kwargs.get('handler', None)
+        self.pipe = kwargs.get('pipe', None)
         self.isasync = kwargs.get('isasync', False)
+        self.connection_timeout = kwargs.get('connection_timeout', 30)
+        self.response_timeout = kwargs.get('response_timeout', 10)
 
         client_id = str(client_id)
-        self.ipc_path = get_ipc_path(pipe)
-
-        if not self.ipc_path:
-            raise DiscordNotFound
 
         if loop is not None:
             self.update_event_loop(loop)
         else:
             self.update_event_loop(get_event_loop())
 
         self.sock_reader: Optional[asyncio.StreamReader] = None
@@ -74,19 +72,21 @@
 
     # noinspection PyUnusedLocal
     async def _async_err_handle(self, loop, context: dict):
         await self.handler(context['exception'], context['future'])
 
     async def read_output(self):
         try:
-            preamble = await self.sock_reader.read(8)
+            preamble = await asyncio.wait_for(self.sock_reader.read(8), self.response_timeout)
             status_code, length = struct.unpack('<II', preamble[:8])
-            data = await self.sock_reader.read(length)
-        except BrokenPipeError:
-            raise InvalidID
+            data = await asyncio.wait_for(self.sock_reader.read(length), self.response_timeout)
+        except (BrokenPipeError, struct.error):
+            raise PipeClosed
+        except asyncio.TimeoutError:
+            raise ResponseTimeout
         payload = json.loads(data.decode('utf-8'))
         if payload["evt"] == "ERROR":
             raise ServerError(payload["data"]["message"])
         return payload
 
     def send_data(self, op: int, payload: Union[dict, Payload]):
         if isinstance(payload, Payload):
@@ -99,25 +99,33 @@
             struct.pack(
                 '<II',
                 op,
                 len(payload)) +
             payload.encode('utf-8'))
 
     async def handshake(self):
-        if sys.platform == 'linux' or sys.platform == 'darwin':
-            self.sock_reader, self.sock_writer = await asyncio.open_unix_connection(self.ipc_path)
-        elif sys.platform == 'win32' or sys.platform == 'win64':
-            self.sock_reader = asyncio.StreamReader(loop=self.loop)
-            reader_protocol = asyncio.StreamReaderProtocol(
-                self.sock_reader, loop=self.loop)
-            try:
-                self.sock_writer, _ = await self.loop.create_pipe_connection(lambda: reader_protocol, self.ipc_path)
-            except FileNotFoundError:
-                raise InvalidPipe
+        ipc_path = get_ipc_path(self.pipe)
+        if not ipc_path:
+            raise DiscordNotFound
+
+        try:
+            if sys.platform == 'linux' or sys.platform == 'darwin':
+                self.sock_reader, self.sock_writer = await asyncio.wait_for(asyncio.open_unix_connection(ipc_path), self.connection_timeout)
+            elif sys.platform == 'win32' or sys.platform == 'win64':
+                self.sock_reader = asyncio.StreamReader(loop=self.loop)
+                reader_protocol = asyncio.StreamReaderProtocol(self.sock_reader, loop=self.loop)
+                self.sock_writer, _ = await asyncio.wait_for(self.loop.create_pipe_connection(lambda: reader_protocol, ipc_path), self.connection_timeout)
+        except FileNotFoundError:
+            raise InvalidPipe
+        except asyncio.TimeoutError:
+            raise ConnectionTimeout
+
         self.send_data(0, {'v': 1, 'client_id': self.client_id})
         preamble = await self.sock_reader.read(8)
         code, length = struct.unpack('<ii', preamble)
         data = json.loads(await self.sock_reader.read(length))
         if 'code' in data:
+            if data['message'] == 'Invalid Client ID':
+                raise InvalidID
             raise DiscordError(data['code'], data['message'])
         if self._events_on:
             self.sock_reader.feed_data = self.on_event
```

### Comparing `pypresence-4.2.1/pypresence/client.py` & `pypresence-4.3.0/pypresence/client.py`

 * *Files identical despite different names*

### Comparing `pypresence-4.2.1/pypresence/exceptions.py` & `pypresence-4.3.0/pypresence/exceptions.py`

 * *Files 22% similar despite different names*

```diff
@@ -6,19 +6,14 @@
 
 
 class DiscordNotFound(PyPresenceException):
     def __init__(self):
         super().__init__('Could not find Discord installed and running on this machine.')
 
 
-class InvalidID(PyPresenceException):
-    def __init__(self):
-        super().__init__('Client ID is Invalid')
-
-
 class InvalidPipe(PyPresenceException):
     def __init__(self):
         super().__init__('Pipe Not Found - Is Discord Running?')
 
 
 class InvalidArgument(PyPresenceException):
     def __init__(self, expected, received, description: str = None):
@@ -30,21 +25,41 @@
 
 class ServerError(PyPresenceException):
     def __init__(self, message: str):
         super().__init__(message.replace(']', '').replace('[', '').capitalize())
 
 
 class DiscordError(PyPresenceException):
-    def __init__(self, code: int, message: str):
+    def __init__(self, code: int, message: str, override=False):
         self.code = code
         self.message = message
-        super().__init__('Error Code: {0} Message: {1}'.format(code, message))
+        super().__init__('Error Code: {0} Message: {1}'.format(code, message) if not override else message)
+
+
+class InvalidID(DiscordError):
+    def __init__(self):
+        super().__init__(4000, 'Client ID is Invalid')
 
 
 class ArgumentError(PyPresenceException):
     def __init__(self):
         super().__init__('Supplied function must have one argument.')
 
 
 class EventNotFound(PyPresenceException):
     def __init__(self, event):
         super().__init__('No event with name {0} exists.'.format(event))
+
+
+class PipeClosed(PyPresenceException):
+    def __init__(self):
+        super().__init__('The pipe was closed. Catch this exception and re-connect your instance.')
+
+
+class ResponseTimeout(PyPresenceException):
+    def __init__(self):
+        super().__init__('No response was received from the pipe in time')
+
+
+class ConnectionTimeout(PyPresenceException):
+    def __init__(self):
+        super().__init__('Unable to create a connection to the pipe in time')
```

### Comparing `pypresence-4.2.1/pypresence/payloads.py` & `pypresence-4.3.0/pypresence/payloads.py`

 * *Files identical despite different names*

### Comparing `pypresence-4.2.1/pypresence/presence.py` & `pypresence-4.3.0/pypresence/presence.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,26 +16,24 @@
                state: str = None, details: str = None,
                start: int = None, end: int = None,
                large_image: str = None, large_text: str = None,
                small_image: str = None, small_text: str = None,
                party_id: str = None, party_size: list = None,
                join: str = None, spectate: str = None,
                match: str = None, buttons: list = None,
-               instance: bool = True,
-               _donotuse=True):
+               instance: bool = True, payload_override: dict = None):
 
-        if _donotuse is True:
+        if payload_override is None:
             payload = Payload.set_activity(pid=pid, state=state, details=details, start=start, end=end,
                                            large_image=large_image, large_text=large_text,
                                            small_image=small_image, small_text=small_text, party_id=party_id,
                                            party_size=party_size, join=join, spectate=spectate,
                                            match=match, buttons=buttons, instance=instance, activity=True)
-
         else:
-            payload = _donotuse
+            payload = payload_override
         self.send_data(1, payload)
         return self.loop.run_until_complete(self.read_output())
 
     def clear(self, pid: int = os.getpid()):
         payload = Payload.set_activity(pid, activity=None)
         self.send_data(1, payload)
         return self.loop.run_until_complete(self.read_output())
```

### Comparing `pypresence-4.2.1/pypresence.egg-info/PKG-INFO` & `pypresence-4.3.0/pypresence.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypresence
-Version: 4.2.1
+Version: 4.3.0
 Summary: Discord RPC client written in Python
 Home-page: https://github.com/qwertyquerty/pypresence
 Author: qwertyquerty
 License: MIT
 Keywords: discord rich presence pypresence rpc api wrapper gamers chat irc
 Platform: Windows
 Platform: Linux
@@ -14,40 +14,32 @@
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Communications :: Chat
 Classifier: Framework :: AsyncIO
-Requires-Python: >=3.5
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 > A Discord Rich Presence Client in Python? Looks like you've come to the right place.
 
-Written by: [qwertyquerty](https://github.com/qwertyquerty)
-
-Notable Contributors: [GiovanniMCMXCIX](https://github.com/GiovanniMCMXCIX), [GhostofGoes](https://github.com/GhostofGoes)
-
 [![GitHub stars](https://img.shields.io/github/stars/qwertyquerty/pypresence.svg?style=for-the-badge&label=Stars)](https://github.com/qwertyquerty/pypresence) [![license](https://img.shields.io/github/license/qwertyquerty/pypresence.svg?style=for-the-badge)](https://github.com/qwertyquerty/pypresence/blob/master/LICENSE) ![GitHub last commit](https://img.shields.io/github/last-commit/qwertyquerty/pypresence.svg?style=for-the-badge) ![GitHub top language](https://img.shields.io/github/languages/top/qwertyquerty/pypresence.svg?style=for-the-badge) ![PyPI](https://img.shields.io/pypi/v/pypresence.svg?style=for-the-badge)
 
-
 ## NOTE: Only Python versions 3.8 and above are supported.
 
-
-## NOTICE: Activity() class has been removed in 4.0.0
-
-
 ### [Documentation](https://qwertyquerty.github.io/pypresence/html/index.html), [Discord Server](https://discord.gg/JF3kg77), [Patreon](https://www.patreon.com/qwertyquerty)
 
 ----------
 
 **Use this badge in your project's Readme to show you're using pypresence! The markdown code is below.**
 
 [![pypresence](https://img.shields.io/badge/using-pypresence-00bb88.svg?style=for-the-badge&logo=discord&logoWidth=20)](https://github.com/qwertyquerty/pypresence)
@@ -75,19 +67,22 @@
 
 
 # Documentation
 
 > **NOTE**: You need an **authorized app** to do anything besides rich presence!
 
 ####  [pypresence Documentation](https://qwertyquerty.github.io/pypresence/html/index.html)
-####  [Discord Rich Presence Documentation](https://discordapp.com/developers/docs/rich-presence/how-to)
-####  [Discord RPC Documentation](https://discordapp.com/developers/docs/topics/rpc)
+####  [Discord Rich Presence Documentation](https://discord.com/developers/docs/rich-presence/how-to)
+####  [Discord RPC Documentation](https://discord.com/developers/docs/topics/rpc)
 ####  [pyresence Discord Support Server](https://discord.gg/JF3kg77)
 ####  [Discord API Support Server](https://discord.gg/discord-api)
 
 ----------
 
 # Examples
 
 Examples can be found in the [examples](https://github.com/qwertyquerty/pypresence/tree/master/examples) directory, and you can contribute your own examples if you wish, just read [examples.md](https://github.com/qwertyquerty/pypresence/blob/master/examples/examples.md)!
 
+----------
+Written by: [qwertyquerty](https://github.com/qwertyquerty)
 
+Notable Contributors: [GiovanniMCMXCIX](https://github.com/GiovanniMCMXCIX), [GhostofGoes](https://github.com/GhostofGoes)
```

### Comparing `pypresence-4.2.1/setup.py` & `pypresence-4.3.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 # https://setuptools.readthedocs.io/en/latest/setuptools.html
 setup(name='pypresence',
       author='qwertyquerty',
       url='https://github.com/qwertyquerty/pypresence',
       version=pypresence.__version__,
       packages=['pypresence'],
-      python_requires='>=3.5',
+      python_requires='>=3.8',
       platforms=['Windows', 'Linux', 'OSX'],
       zip_safe=True,
       license='MIT',
       description='Discord RPC client written in Python',
       long_description=long_description,
       # PEP 566, PyPI Warehouse, setuptools>=38.6.0 make markdown possible
       long_description_content_type='text/markdown',
@@ -31,14 +31,15 @@
             'Operating System :: POSIX :: Linux',
             'Operating System :: MacOS :: MacOS X',
 
             'Programming Language :: Python',
             'Programming Language :: Python :: 3.8',
             'Programming Language :: Python :: 3.9',
             'Programming Language :: Python :: 3.10',
+            'Programming Language :: Python :: 3.11',
 
             'Programming Language :: Python :: 3 :: Only',
             'Programming Language :: Python :: Implementation :: CPython',
 
             'Intended Audience :: Developers',
             'Topic :: Software Development :: Libraries :: Python Modules',
             'Topic :: Software Development :: Libraries',
```

