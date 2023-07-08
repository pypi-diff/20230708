# Comparing `tmp/vban_cmd-2.1.2.tar.gz` & `tmp/vban_cmd-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vban_cmd-2.1.2.tar", max compression
+gzip compressed data, was "vban_cmd-2.2.0.tar", max compression
```

## Comparing `vban_cmd-2.1.2.tar` & `vban_cmd-2.2.0.tar`

### file list

```diff
@@ -1,20 +1,22 @@
--rw-r--r--   0        0        0     1091 2022-03-24 12:30:28.474287 vban_cmd-2.1.2/LICENSE
--rw-r--r--   0        0        0      951 2023-07-05 17:15:05.999987 vban_cmd-2.1.2/pyproject.toml
--rw-r--r--   0        0        0    11605 2023-07-05 13:04:56.374532 vban_cmd-2.1.2/README.md
--rw-r--r--   0        0        0       70 2022-07-12 16:30:51.963399 vban_cmd-2.1.2/vban_cmd/__init__.py
--rw-r--r--   0        0        0     5276 2023-06-25 10:36:16.654167 vban_cmd-2.1.2/vban_cmd/bus.py
--rw-r--r--   0        0        0     1127 2023-06-25 10:36:19.263212 vban_cmd-2.1.2/vban_cmd/command.py
--rw-r--r--   0        0        0     5855 2023-06-25 10:36:21.413563 vban_cmd-2.1.2/vban_cmd/config.py
--rw-r--r--   0        0        0      197 2023-06-25 10:36:23.500662 vban_cmd-2.1.2/vban_cmd/error.py
--rw-r--r--   0        0        0     1621 2023-06-22 09:26:30.424951 vban_cmd-2.1.2/vban_cmd/event.py
--rw-r--r--   0        0        0     6133 2023-07-05 13:04:18.891728 vban_cmd-2.1.2/vban_cmd/factory.py
--rw-r--r--   0        0        0     4115 2023-07-05 18:08:51.113607 vban_cmd-2.1.2/vban_cmd/iremote.py
--rw-r--r--   0        0        0     2184 2023-06-22 02:29:18.843450 vban_cmd-2.1.2/vban_cmd/kinds.py
--rw-r--r--   0        0        0     2992 2023-06-25 10:36:33.230612 vban_cmd-2.1.2/vban_cmd/meta.py
--rw-r--r--   0        0        0     9644 2023-06-25 14:59:01.896621 vban_cmd-2.1.2/vban_cmd/packet.py
--rw-r--r--   0        0        0    10137 2023-06-25 12:32:36.307607 vban_cmd-2.1.2/vban_cmd/strip.py
--rw-r--r--   0        0        0     2277 2023-06-25 10:36:40.287522 vban_cmd-2.1.2/vban_cmd/subject.py
--rw-r--r--   0        0        0     2060 2023-06-25 10:36:42.302165 vban_cmd-2.1.2/vban_cmd/util.py
--rw-r--r--   0        0        0     6666 2023-07-05 18:08:31.368177 vban_cmd-2.1.2/vban_cmd/vbancmd.py
--rw-r--r--   0        0        0     6905 2023-06-25 14:54:55.684238 vban_cmd-2.1.2/vban_cmd/worker.py
--rw-r--r--   0        0        0    11763 1970-01-01 00:00:00.000000 vban_cmd-2.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1091 2022-03-24 12:30:28.474287 vban_cmd-2.2.0/LICENSE
+-rw-r--r--   0        0        0      951 2023-07-08 06:34:03.457702 vban_cmd-2.2.0/pyproject.toml
+-rw-r--r--   0        0        0    11605 2023-07-05 13:04:56.374532 vban_cmd-2.2.0/README.md
+-rw-r--r--   0        0        0       70 2022-07-12 16:30:51.963399 vban_cmd-2.2.0/vban_cmd/__init__.py
+-rw-r--r--   0        0        0     5276 2023-06-25 10:36:16.654167 vban_cmd-2.2.0/vban_cmd/bus.py
+-rw-r--r--   0        0        0     1127 2023-06-25 10:36:19.263212 vban_cmd-2.2.0/vban_cmd/command.py
+-rw-r--r--   0        0        0     5855 2023-06-25 10:36:21.413563 vban_cmd-2.2.0/vban_cmd/config.py
+-rw-r--r--   0        0        0      197 2023-06-25 10:36:23.500662 vban_cmd-2.2.0/vban_cmd/error.py
+-rw-r--r--   0        0        0     1621 2023-06-22 09:26:30.424951 vban_cmd-2.2.0/vban_cmd/event.py
+-rw-r--r--   0        0        0     6902 2023-07-08 06:42:16.984039 vban_cmd-2.2.0/vban_cmd/factory.py
+-rw-r--r--   0        0        0     4115 2023-07-05 18:08:51.113607 vban_cmd-2.2.0/vban_cmd/iremote.py
+-rw-r--r--   0        0        0     2184 2023-06-22 02:29:18.843450 vban_cmd-2.2.0/vban_cmd/kinds.py
+-rw-r--r--   0        0        0     1150 2023-07-08 06:13:52.713834 vban_cmd-2.2.0/vban_cmd/macrobutton.py
+-rw-r--r--   0        0        0     2992 2023-06-25 10:36:33.230612 vban_cmd-2.2.0/vban_cmd/meta.py
+-rw-r--r--   0        0        0     9644 2023-06-25 14:59:01.896621 vban_cmd-2.2.0/vban_cmd/packet.py
+-rw-r--r--   0        0        0    10137 2023-06-25 12:32:36.307607 vban_cmd-2.2.0/vban_cmd/strip.py
+-rw-r--r--   0        0        0     2277 2023-06-25 10:36:40.287522 vban_cmd-2.2.0/vban_cmd/subject.py
+-rw-r--r--   0        0        0     2060 2023-06-25 10:36:42.302165 vban_cmd-2.2.0/vban_cmd/util.py
+-rw-r--r--   0        0        0     4320 2023-07-08 06:27:12.206963 vban_cmd-2.2.0/vban_cmd/vban.py
+-rw-r--r--   0        0        0     6915 2023-07-08 07:08:39.810087 vban_cmd-2.2.0/vban_cmd/vbancmd.py
+-rw-r--r--   0        0        0     6905 2023-06-25 14:54:55.684238 vban_cmd-2.2.0/vban_cmd/worker.py
+-rw-r--r--   0        0        0    11763 1970-01-01 00:00:00.000000 vban_cmd-2.2.0/PKG-INFO
```

### Comparing `vban_cmd-2.1.2/LICENSE` & `vban_cmd-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vban_cmd-2.1.2/pyproject.toml` & `vban_cmd-2.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "vban-cmd"
-version = "2.1.2"
+version = "2.2.0"
 description = "Python interface for the VBAN RT Packet Service (Sendtext)"
 authors = ["onyx-and-iris <code@onyxandiris.online>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/onyx-and-iris/vban-cmd-python"
 
 [tool.poetry.dependencies]
```

### Comparing `vban_cmd-2.1.2/README.md` & `vban_cmd-2.2.0/README.md`

 * *Files identical despite different names*

### Comparing `vban_cmd-2.1.2/vban_cmd/bus.py` & `vban_cmd-2.2.0/vban_cmd/bus.py`

 * *Files identical despite different names*

### Comparing `vban_cmd-2.1.2/vban_cmd/command.py` & `vban_cmd-2.2.0/vban_cmd/command.py`

 * *Files identical despite different names*

### Comparing `vban_cmd-2.1.2/vban_cmd/config.py` & `vban_cmd-2.2.0/vban_cmd/config.py`

 * *Files identical despite different names*

### Comparing `vban_cmd-2.1.2/vban_cmd/event.py` & `vban_cmd-2.2.0/vban_cmd/event.py`

 * *Files identical despite different names*

### Comparing `vban_cmd-2.1.2/vban_cmd/factory.py` & `vban_cmd-2.2.0/vban_cmd/factory.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,36 +6,42 @@
 
 from .bus import request_bus_obj as bus
 from .command import Command
 from .config import request_config as configs
 from .error import VBANCMDError
 from .kinds import KindMapClass
 from .kinds import request_kind_map as kindmap
+from .macrobutton import MacroButton
 from .strip import request_strip_obj as strip
+from .vban import request_vban_obj as vban
 from .vbancmd import VbanCmd
 
 logger = logging.getLogger(__name__)
 
 
 class FactoryBuilder:
     """
     Builder class for factories.
 
     Separates construction from representation.
     """
 
-    BuilderProgress = IntEnum("BuilderProgress", "strip bus command", start=0)
+    BuilderProgress = IntEnum(
+        "BuilderProgress", "strip bus command macrobutton vban", start=0
+    )
 
     def __init__(self, factory, kind: KindMapClass):
         self._factory = factory
         self.kind = kind
         self._info = (
             f"Finished building strips for {self._factory}",
             f"Finished building buses for {self._factory}",
             f"Finished building commands for {self._factory}",
+            f"Finished building macrobuttons for {self._factory}",
+            f"Finished building vban in/out streams for {self._factory}",
         )
         self.logger = logger.getChild(self.__class__.__name__)
 
     def _pinfo(self, name: str) -> NoReturn:
         """prints progress status for each step"""
         name = name.split("_")[1]
         self.logger.info(self._info[int(getattr(self.BuilderProgress, name))])
@@ -54,14 +60,22 @@
         )
         return self
 
     def make_command(self):
         self._factory.command = Command.make(self._factory)
         return self
 
+    def make_macrobutton(self):
+        self._factory.button = tuple(MacroButton(self._factory, i) for i in range(80))
+        return self
+
+    def make_vban(self):
+        self._factory.vban = vban(self._factory)
+        return self
+
 
 class FactoryBase(VbanCmd):
     """Base class for factories, subclasses VbanCmd."""
 
     def __init__(self, kind_id: str, **kwargs):
         defaultkwargs = {
             "ip": None,
@@ -82,20 +96,28 @@
         self.kind = kindmap(kind_id)
         super().__init__(**kwargs)
         self.builder = FactoryBuilder(self, self.kind)
         self._steps = (
             self.builder.make_strip,
             self.builder.make_bus,
             self.builder.make_command,
+            self.builder.make_macrobutton,
+            self.builder.make_vban,
         )
         self._configs = None
 
     def __str__(self) -> str:
         return f"Voicemeeter {self.kind}"
 
+    def __repr__(self):
+        return (
+            type(self).__name__
+            + f"({self.kind}, ip='{self.ip}', port={self.port}, streamname='{self.streamname}')"
+        )
+
     @property
     @abstractmethod
     def steps(self):
         pass
 
     @cached_property
     def configs(self):
```

### Comparing `vban_cmd-2.1.2/vban_cmd/iremote.py` & `vban_cmd-2.2.0/vban_cmd/iremote.py`

 * *Files identical despite different names*

### Comparing `vban_cmd-2.1.2/vban_cmd/kinds.py` & `vban_cmd-2.2.0/vban_cmd/kinds.py`

 * *Files identical despite different names*

### Comparing `vban_cmd-2.1.2/vban_cmd/meta.py` & `vban_cmd-2.2.0/vban_cmd/meta.py`

 * *Files identical despite different names*

### Comparing `vban_cmd-2.1.2/vban_cmd/packet.py` & `vban_cmd-2.2.0/vban_cmd/packet.py`

 * *Files identical despite different names*

### Comparing `vban_cmd-2.1.2/vban_cmd/strip.py` & `vban_cmd-2.2.0/vban_cmd/strip.py`

 * *Files identical despite different names*

### Comparing `vban_cmd-2.1.2/vban_cmd/subject.py` & `vban_cmd-2.2.0/vban_cmd/subject.py`

 * *Files identical despite different names*

### Comparing `vban_cmd-2.1.2/vban_cmd/util.py` & `vban_cmd-2.2.0/vban_cmd/util.py`

 * *Files identical despite different names*

### Comparing `vban_cmd-2.1.2/vban_cmd/vbancmd.py` & `vban_cmd-2.2.0/vban_cmd/vbancmd.py`

 * *Files 4% similar despite different names*

```diff
@@ -96,15 +96,19 @@
 
             queue = Queue()
             self.updater = Updater(self, queue)
             self.updater.start()
             self.producer = Producer(self, queue)
             self.producer.start()
 
-        self.logger.info(f"{type(self).__name__}: Successfully logged into {self}")
+        self.logger.info(
+            "Successfully logged into {kind} with ip='{ip}', port={port}, streamname='{streamname}'".format(
+                **self.__dict__
+            )
+        )
 
     def _set_rt(self, cmd: str, val: Union[str, float]):
         """Sends a string request command over a network."""
         self.socks[Socket.request].sendto(
             self.packet_request.header + f"{cmd}={val};".encode(),
             (socket.gethostbyname(self.ip), self.port),
         )
@@ -119,15 +123,15 @@
         self.socks[Socket.request].sendto(
             self.packet_request.header + script.encode(),
             (socket.gethostbyname(self.ip), self.port),
         )
         self.packet_request.framecounter = (
             int.from_bytes(self.packet_request.framecounter, "little") + 1
         ).to_bytes(4, "little")
-        self.logger.debug(f"sendtext: [{self.ip}:{self.port}] {script}")
+        self.logger.debug(f"sendtext: {script}")
         time.sleep(self.DELAY)
 
     @property
     def type(self) -> str:
         """Returns the type of Voicemeeter installation."""
         return self.public_packet.voicemeetertype
 
@@ -171,32 +175,34 @@
 
         minor delay between each recursion
         """
 
         def param(key):
             obj, m2, *rem = key.split("-")
             index = int(m2) if m2.isnumeric() else int(*rem)
-            if obj in ("strip", "bus"):
+            if obj in ("strip", "bus", "button"):
                 return getattr(self, obj)[index]
-            else:
-                raise ValueError(obj)
+            elif obj == "vban":
+                return getattr(getattr(self, obj), f"{m2}stream")[index]
+            raise ValueError(obj)
 
         [param(key).apply(datum).then_wait() for key, datum in data.items()]
 
     def apply_config(self, name):
         """applies a config from memory"""
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
+            raise VBANCMDError(("\n").join(error_msg)) from e
 
     def logout(self):
         self.running = False
         time.sleep(0.2)
         [sock.close() for sock in self.socks]
         self.logger.info(f"{type(self).__name__}: Successfully logged out of {self}")
```

### Comparing `vban_cmd-2.1.2/vban_cmd/worker.py` & `vban_cmd-2.2.0/vban_cmd/worker.py`

 * *Files identical despite different names*

### Comparing `vban_cmd-2.1.2/PKG-INFO` & `vban_cmd-2.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vban-cmd
-Version: 2.1.2
+Version: 2.2.0
 Summary: Python interface for the VBAN RT Packet Service (Sendtext)
 Home-page: https://github.com/onyx-and-iris/vban-cmd-python
 License: MIT
 Author: onyx-and-iris
 Author-email: code@onyxandiris.online
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

