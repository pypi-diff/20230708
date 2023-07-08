# Comparing `tmp/goxlr-1.2.0.tar.gz` & `tmp/goxlr-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "goxlr-1.2.0.tar", last modified: Thu Jul  6 18:58:09 2023, max compression
+gzip compressed data, was "goxlr-1.3.0.tar", last modified: Sat Jul  8 12:49:31 2023, max compression
```

## Comparing `goxlr-1.2.0.tar` & `goxlr-1.3.0.tar`

### file list

```diff
@@ -1,25 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-07-06 18:58:09.090412 goxlr-1.2.0/
--rw-rw-rw-   0        0        0     1134 2023-07-04 22:58:41.000000 goxlr-1.2.0/LICENSE-3RD-PARTY.txt
--rw-rw-rw-   0        0        0     1089 2023-07-04 22:53:25.000000 goxlr-1.2.0/LICENSE.txt
--rw-rw-rw-   0        0        0     2503 2023-07-06 18:58:09.090914 goxlr-1.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     2147 2023-07-05 12:48:27.000000 goxlr-1.2.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-06 18:58:09.079412 goxlr-1.2.0/goxlr/
--rw-rw-rw-   0        0        0       62 2023-07-05 11:07:26.000000 goxlr-1.2.0/goxlr/__init__.py
--rw-rw-rw-   0        0        0       23 2023-07-06 18:57:22.000000 goxlr-1.2.0/goxlr/_version.py
-drwxrwxrwx   0        0        0        0 2023-07-06 18:58:09.089412 goxlr-1.2.0/goxlr/commands/
--rw-rw-rw-   0        0        0      108 2023-07-05 11:52:15.000000 goxlr-1.2.0/goxlr/commands/__init__.py
--rw-rw-rw-   0        0        0     1376 2023-07-05 12:17:31.000000 goxlr-1.2.0/goxlr/commands/daemon.py
--rw-rw-rw-   0        0        0      237 2023-07-05 11:08:41.000000 goxlr-1.2.0/goxlr/commands/general.py
--rw-rw-rw-   0        0        0    26136 2023-07-05 12:17:07.000000 goxlr-1.2.0/goxlr/commands/goxlr.py
--rw-rw-rw-   0        0        0       41 2023-07-03 22:14:52.000000 goxlr-1.2.0/goxlr/error.py
--rw-rw-rw-   0        0        0     5101 2023-07-06 18:56:24.000000 goxlr-1.2.0/goxlr/socket.py
--rw-rw-rw-   0        0        0    11533 2023-07-05 12:17:58.000000 goxlr-1.2.0/goxlr/types.py
-drwxrwxrwx   0        0        0        0 2023-07-06 18:58:09.084913 goxlr-1.2.0/goxlr.egg-info/
--rw-rw-rw-   0        0        0     2503 2023-07-06 18:58:09.000000 goxlr-1.2.0/goxlr.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      405 2023-07-06 18:58:09.000000 goxlr-1.2.0/goxlr.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-06 18:58:09.000000 goxlr-1.2.0/goxlr.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2023-07-06 18:58:09.000000 goxlr-1.2.0/goxlr.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-07-06 18:58:09.000000 goxlr-1.2.0/goxlr.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       91 2023-07-04 15:57:33.000000 goxlr-1.2.0/pyproject.toml
--rw-rw-rw-   0        0        0       86 2023-07-06 18:58:09.091911 goxlr-1.2.0/setup.cfg
--rw-rw-rw-   0        0        0      859 2023-07-04 23:15:06.000000 goxlr-1.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-08 12:49:31.335472 goxlr-1.3.0/
+-rw-rw-rw-   0        0        0     1134 2023-07-04 22:58:41.000000 goxlr-1.3.0/LICENSE-3RD-PARTY.txt
+-rw-rw-rw-   0        0        0     1089 2023-07-04 22:53:25.000000 goxlr-1.3.0/LICENSE.txt
+-rw-rw-rw-   0        0        0     2504 2023-07-08 12:49:31.335972 goxlr-1.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2147 2023-07-05 12:48:27.000000 goxlr-1.3.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-08 12:49:31.321973 goxlr-1.3.0/goxlr/
+-rw-rw-rw-   0        0        0       62 2023-07-05 11:07:26.000000 goxlr-1.3.0/goxlr/__init__.py
+-rw-rw-rw-   0        0        0       23 2023-07-08 12:49:08.000000 goxlr-1.3.0/goxlr/_version.py
+drwxrwxrwx   0        0        0        0 2023-07-08 12:49:31.331471 goxlr-1.3.0/goxlr/commands/
+-rw-rw-rw-   0        0        0      106 2023-07-07 18:35:48.000000 goxlr-1.3.0/goxlr/commands/__init__.py
+-rw-rw-rw-   0        0        0     1376 2023-07-07 18:15:11.000000 goxlr-1.3.0/goxlr/commands/daemon.py
+-rw-rw-rw-   0        0        0    26315 2023-07-08 12:48:03.000000 goxlr-1.3.0/goxlr/commands/goxlr.py
+-rw-rw-rw-   0        0        0     4685 2023-07-08 12:39:50.000000 goxlr-1.3.0/goxlr/commands/status.py
+-rw-rw-rw-   0        0        0       93 2023-07-07 19:20:53.000000 goxlr-1.3.0/goxlr/error.py
+-rw-rw-rw-   0        0        0     7764 2023-07-08 12:42:53.000000 goxlr-1.3.0/goxlr/socket.py
+drwxrwxrwx   0        0        0        0 2023-07-08 12:49:31.334473 goxlr-1.3.0/goxlr/types/
+-rw-rw-rw-   0        0        0       45 2023-07-08 11:41:47.000000 goxlr-1.3.0/goxlr/types/__init__.py
+-rw-rw-rw-   0        0        0    11552 2023-07-08 10:59:03.000000 goxlr-1.3.0/goxlr/types/enums.py
+-rw-rw-rw-   0        0        0    22457 2023-07-08 12:28:22.000000 goxlr-1.3.0/goxlr/types/models.py
+drwxrwxrwx   0        0        0        0 2023-07-08 12:49:31.326971 goxlr-1.3.0/goxlr.egg-info/
+-rw-rw-rw-   0        0        0     2504 2023-07-08 12:49:31.000000 goxlr-1.3.0/goxlr.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      456 2023-07-08 12:49:31.000000 goxlr-1.3.0/goxlr.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-08 12:49:31.000000 goxlr-1.3.0/goxlr.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2023-07-08 12:49:31.000000 goxlr-1.3.0/goxlr.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-07-08 12:49:31.000000 goxlr-1.3.0/goxlr.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       91 2023-07-04 15:57:33.000000 goxlr-1.3.0/pyproject.toml
+-rw-rw-rw-   0        0        0       86 2023-07-08 12:49:31.336977 goxlr-1.3.0/setup.cfg
+-rw-rw-rw-   0        0        0      860 2023-07-08 12:29:52.000000 goxlr-1.3.0/setup.py
```

### Comparing `goxlr-1.2.0/LICENSE-3RD-PARTY.txt` & `goxlr-1.3.0/LICENSE-3RD-PARTY.txt`

 * *Files identical despite different names*

### Comparing `goxlr-1.2.0/LICENSE.txt` & `goxlr-1.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `goxlr-1.2.0/PKG-INFO` & `goxlr-1.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: goxlr
-Version: 1.2.0
+Version: 1.3.0
 Summary: A Python wrapper for the GoXLR Utility API.
 Home-page: https://github.com/samcarsonx/goxlr
 Author: Sam Carson
 Author-email: sam@samcarson.co.uk
 License: MIT
-Requires-Python: >=3.6
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE-3RD-PARTY.txt
 License-File: LICENSE.txt
 
 # GoXLR Utility API Python Wrapper
 
  [![License](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT) [![PyPI version](https://badge.fury.io/py/goxlr.svg)](https://badge.fury.io/py/goxlr) ![PyPI - Downloads](https://img.shields.io/pypi/dm/goxlr) ![GitHub issues](https://img.shields.io/github/issues/samcarsonx/goxlr) [![Documentation Status](https://readthedocs.org/projects/goxlr/badge/?version=latest)](https://goxlr.readthedocs.io/en/latest/?badge=latest)
```

### Comparing `goxlr-1.2.0/README.md` & `goxlr-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `goxlr-1.2.0/goxlr/commands/daemon.py` & `goxlr-1.3.0/goxlr/commands/daemon.py`

 * *Files identical despite different names*

### Comparing `goxlr-1.2.0/goxlr/commands/goxlr.py` & `goxlr-1.3.0/goxlr/commands/goxlr.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 import ctypes
-from ..types import *
+from ..types.enums import *
 
 
 class GoXLRCommands:
     # GoXLR commands
 
     async def __send_command(self, payload, serial=None):
         payload = {"Command": [serial or self.serial, payload]}
         return await self.send(payload)
 
-    async def set_shutdown_commands(self, *methods):
+    async def set_shutdown_commands(self, *methods) -> dict | str:
         """
         Set the commands to be executed when the GoXLR is shutting down.
         Commands are accepted as a list of lists, where the first item is
         the method name and the remaining items are the arguments for that
         method.
 
         :param methods: A list of methods to be executed when the GoXLR is shutting down.
         :type methods: list
         :return: The response from the GoXLR.
-        :rtype: dict or str
 
         :Example:
 
         >>> await xlr.set_shutdown_commands(
-        ...     ["SetFader", FaderName.A, ChannelName.Headphones]
+        ...     ["SetFader", Fader.A, Channel.Headphones],
+        ...     ["SetFader", Fader.B, Channel.Chat]
         ... )
         """
 
         # Initialize the command dictionary
         command = {"SetShutdownCommands": []}
 
         # Iterate over the provided methods
@@ -167,15 +167,21 @@
 
     # DeEss
     async def set_deeser(self, deesser: ctypes.c_uint8):
         return await self.__send_command({"SetDeesser": deesser})
 
     # Colour Related Settings
     async def set_animation_mode(self, animation_mode: AnimationMode):
-        return await self.__send_command({"SetAnimationMode": animation_mode.name})
+        return await self.__send_command(
+            {
+                "SetAnimationMode": "None"
+                if animation_mode is AnimationMode.NONE
+                else animation_mode.name
+            }
+        )
 
     async def set_animation_mod1(self, animation_mod1: ctypes.c_uint8):
         return await self.__send_command({"SetAnimationMod1": animation_mod1})
 
     async def set_animation_mod2(self, animation_mod2: ctypes.c_uint8):
         return await self.__send_command({"SetAnimationMod2": animation_mod2})
```

### Comparing `goxlr-1.2.0/goxlr/types.py` & `goxlr-1.3.0/goxlr/types/enums.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 from enum import Enum
 
+# Enumerators used by the GoXLR Utility Daemon. (with slight name changes)
+
 
 class PathType(Enum):
     Profiles = 1
     MicProfiles = 2
     Presets = 3
     Samples = 4
     Icons = 5
@@ -571,14 +573,14 @@
 
 class AnimationMode(Enum):
     RetroRainbow = 1
     RainbowDark = 2
     RainbowBright = 3
     Simple = 4
     Ripple = 5
-    NoMode = 6  # Should be 'None' but that's a reserved word in Python
+    NONE = 6
 
 
 class WaterfallDirection(Enum):
     Down = 1
     Up = 2
     Off = 3
```

### Comparing `goxlr-1.2.0/goxlr.egg-info/PKG-INFO` & `goxlr-1.3.0/goxlr.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: goxlr
-Version: 1.2.0
+Version: 1.3.0
 Summary: A Python wrapper for the GoXLR Utility API.
 Home-page: https://github.com/samcarsonx/goxlr
 Author: Sam Carson
 Author-email: sam@samcarson.co.uk
 License: MIT
-Requires-Python: >=3.6
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE-3RD-PARTY.txt
 License-File: LICENSE.txt
 
 # GoXLR Utility API Python Wrapper
 
  [![License](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT) [![PyPI version](https://badge.fury.io/py/goxlr.svg)](https://badge.fury.io/py/goxlr) ![PyPI - Downloads](https://img.shields.io/pypi/dm/goxlr) ![GitHub issues](https://img.shields.io/github/issues/samcarsonx/goxlr) [![Documentation Status](https://readthedocs.org/projects/goxlr/badge/?version=latest)](https://goxlr.readthedocs.io/en/latest/?badge=latest)
```

### Comparing `goxlr-1.2.0/setup.py` & `goxlr-1.3.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -18,11 +18,11 @@
     description="A Python wrapper for the GoXLR Utility API.",
     url="https://github.com/samcarsonx/goxlr",
     author="Sam Carson",
     author_email="sam@samcarson.co.uk",
     license="MIT",
     packages=find_packages(),
     install_requires=["asyncio", "websockets"],
-    python_requires=">=3.6",
+    python_requires=">=3.10",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
 )
```

