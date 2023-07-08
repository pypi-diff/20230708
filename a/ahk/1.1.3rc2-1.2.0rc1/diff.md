# Comparing `tmp/ahk-1.1.3rc2.tar.gz` & `tmp/ahk-1.2.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ahk-1.1.3rc2.tar", last modified: Wed May 17 19:28:58 2023, max compression
+gzip compressed data, was "ahk-1.2.0rc1.tar", last modified: Sat Jul  8 06:57:43 2023, max compression
```

## Comparing `ahk-1.1.3rc2.tar` & `ahk-1.2.0rc1.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:28:58.251110 ahk-1.1.3rc2/
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-17 19:28:43.000000 ahk-1.1.3rc2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    18814 2023-05-17 19:28:58.251110 ahk-1.1.3rc2/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:28:58.247110 ahk-1.1.3rc2/ahk/
--rw-r--r--   0 runner    (1001) docker     (123)      956 2023-05-17 19:28:43.000000 ahk-1.1.3rc2/ahk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:28:58.247110 ahk-1.1.3rc2/ahk/_async/
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-17 19:28:43.000000 ahk-1.1.3rc2/ahk/_async/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   179999 2023-05-17 19:28:43.000000 ahk-1.1.3rc2/ahk/_async/engine.py
--rw-r--r--   0 runner    (1001) docker     (123)    43479 2023-05-17 19:28:43.000000 ahk-1.1.3rc2/ahk/_async/transport.py
--rw-r--r--   0 runner    (1001) docker     (123)    29128 2023-05-17 19:28:43.000000 ahk-1.1.3rc2/ahk/_async/window.py
--rw-r--r--   0 runner    (1001) docker     (123)    83686 2023-05-17 19:28:43.000000 ahk-1.1.3rc2/ahk/_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    14354 2023-05-17 19:28:43.000000 ahk-1.1.3rc2/ahk/_hotkey.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:28:58.247110 ahk-1.1.3rc2/ahk/_sync/
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-17 19:28:43.000000 ahk-1.1.3rc2/ahk/_sync/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   174245 2023-05-17 19:28:43.000000 ahk-1.1.3rc2/ahk/_sync/engine.py
--rw-r--r--   0 runner    (1001) docker     (123)    39283 2023-05-17 19:28:43.000000 ahk-1.1.3rc2/ahk/_sync/transport.py
--rw-r--r--   0 runner    (1001) docker     (123)    26344 2023-05-17 19:28:43.000000 ahk-1.1.3rc2/ahk/_sync/window.py
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-05-17 19:28:43.000000 ahk-1.1.3rc2/ahk/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3496 2023-05-17 19:28:43.000000 ahk-1.1.3rc2/ahk/directives.py
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-17 19:28:43.000000 ahk-1.1.3rc2/ahk/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7506 2023-05-17 19:28:43.000000 ahk-1.1.3rc2/ahk/keys.py
--rw-r--r--   0 runner    (1001) docker     (123)    11435 2023-05-17 19:28:43.000000 ahk-1.1.3rc2/ahk/message.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 19:28:43.000000 ahk-1.1.3rc2/ahk/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:28:58.247110 ahk-1.1.3rc2/ahk/templates/
--rw-r--r--   0 runner    (1001) docker     (123)    79035 2023-05-17 19:28:43.000000 ahk-1.1.3rc2/ahk/templates/daemon.ahk
--rw-r--r--   0 runner    (1001) docker     (123)     4508 2023-05-17 19:28:43.000000 ahk-1.1.3rc2/ahk/templates/hotkeys.ahk
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:28:58.247110 ahk-1.1.3rc2/ahk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18814 2023-05-17 19:28:58.000000 ahk-1.1.3rc2/ahk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-05-17 19:28:58.000000 ahk-1.1.3rc2/ahk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 19:28:58.000000 ahk-1.1.3rc2/ahk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-17 19:28:58.000000 ahk-1.1.3rc2/ahk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-17 19:28:58.000000 ahk-1.1.3rc2/ahk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      875 2023-05-17 19:28:43.000000 ahk-1.1.3rc2/buildunasync.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:28:58.251110 ahk-1.1.3rc2/docs/
--rw-r--r--   0 runner    (1001) docker     (123)    17928 2023-05-17 19:28:43.000000 ahk-1.1.3rc2/docs/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-17 19:28:43.000000 ahk-1.1.3rc2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-05-17 19:28:58.251110 ahk-1.1.3rc2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 19:28:43.000000 ahk-1.1.3rc2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 06:57:43.213669 ahk-1.2.0rc1/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-08 06:57:30.000000 ahk-1.2.0rc1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    19167 2023-07-08 06:57:43.213669 ahk-1.2.0rc1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 06:57:43.213669 ahk-1.2.0rc1/ahk/
+-rw-r--r--   0 runner    (1001) docker     (123)      956 2023-07-08 06:57:30.000000 ahk-1.2.0rc1/ahk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 06:57:43.213669 ahk-1.2.0rc1/ahk/_async/
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-07-08 06:57:30.000000 ahk-1.2.0rc1/ahk/_async/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   180681 2023-07-08 06:57:30.000000 ahk-1.2.0rc1/ahk/_async/engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44668 2023-07-08 06:57:30.000000 ahk-1.2.0rc1/ahk/_async/transport.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29128 2023-07-08 06:57:30.000000 ahk-1.2.0rc1/ahk/_async/window.py
+-rw-r--r--   0 runner    (1001) docker     (123)    83686 2023-07-08 06:57:30.000000 ahk-1.2.0rc1/ahk/_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15818 2023-07-08 06:57:30.000000 ahk-1.2.0rc1/ahk/_hotkey.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 06:57:43.213669 ahk-1.2.0rc1/ahk/_sync/
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-08 06:57:30.000000 ahk-1.2.0rc1/ahk/_sync/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   174928 2023-07-08 06:57:30.000000 ahk-1.2.0rc1/ahk/_sync/engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40339 2023-07-08 06:57:30.000000 ahk-1.2.0rc1/ahk/_sync/transport.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26344 2023-07-08 06:57:30.000000 ahk-1.2.0rc1/ahk/_sync/window.py
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-07-08 06:57:30.000000 ahk-1.2.0rc1/ahk/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3496 2023-07-08 06:57:30.000000 ahk-1.2.0rc1/ahk/directives.py
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-08 06:57:30.000000 ahk-1.2.0rc1/ahk/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7506 2023-07-08 06:57:30.000000 ahk-1.2.0rc1/ahk/keys.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11435 2023-07-08 06:57:30.000000 ahk-1.2.0rc1/ahk/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 06:57:30.000000 ahk-1.2.0rc1/ahk/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 06:57:43.213669 ahk-1.2.0rc1/ahk/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)    79035 2023-07-08 06:57:30.000000 ahk-1.2.0rc1/ahk/templates/daemon.ahk
+-rw-r--r--   0 runner    (1001) docker     (123)     4508 2023-07-08 06:57:30.000000 ahk-1.2.0rc1/ahk/templates/hotkeys.ahk
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 06:57:43.213669 ahk-1.2.0rc1/ahk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19167 2023-07-08 06:57:43.000000 ahk-1.2.0rc1/ahk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-07-08 06:57:43.000000 ahk-1.2.0rc1/ahk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 06:57:43.000000 ahk-1.2.0rc1/ahk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-08 06:57:43.000000 ahk-1.2.0rc1/ahk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-08 06:57:43.000000 ahk-1.2.0rc1/ahk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-07-08 06:57:30.000000 ahk-1.2.0rc1/buildunasync.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 06:57:43.213669 ahk-1.2.0rc1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)    18281 2023-07-08 06:57:30.000000 ahk-1.2.0rc1/docs/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-07-08 06:57:30.000000 ahk-1.2.0rc1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-07-08 06:57:43.213669 ahk-1.2.0rc1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 06:57:30.000000 ahk-1.2.0rc1/setup.py
```

### Comparing `ahk-1.1.3rc2/PKG-INFO` & `ahk-1.2.0rc1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ahk
-Version: 1.1.3rc2
+Version: 1.2.0rc1
 Summary: A Python wrapper for AHK
 Home-page: https://github.com/spyoungtech/ahk
 Author: Spencer Young
 Author-email: spencer.young@spyoung.com
 Keywords: ahk,autohotkey,windows,mouse,keyboard,automation,pyautogui
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Desktop Environment
@@ -91,20 +91,28 @@
 
 def my_ex_handler(hotkey: str, exception: Exception):
     print('exception with callback for hotkey', hotkey, 'Here was the error:', exception)
 
 ahk.add_hotkey('#n', callback=go_boom, ex_handler=my_ex_handler)
 ```
 
+There are also methods for removing hotkeys:
+
+```python
+# ...
+ahk.remove_hotkey('#n') # remove a hotkey by its keyname
+ahk.clear_hotkeys()  # remove all hotkeys
+```
+
 Note that:
 
 - Hotkeys run in a separate process that must be started manually (with `ahk.start_hotkeys()`)
 - Hotkeys can be stopped with `ahk.stop_hotkeys()` (will not stop actively running callbacks)
 - Hotstrings (discussed below) share the same process with hotkeys and are started/stopped in the same manner
-- If hotkeys or hotstrings are added while the process is running, the underlying AHK process is restarted automatically
+- If hotkeys or hotstrings are added or removed while the process is running, the underlying AHK process is restarted automatically
 
 
 See also the [relevant AHK documentation](https://www.autohotkey.com/docs/Hotkeys.htm)
 
 ## Hotstrings
 
 
@@ -119,14 +127,21 @@
 def my_callback():
     print('hello callback!')
 
 ahk.add_hotstring('btw', 'by the way')  # string replacements
 ahk.add_hotstring('btw', my_callback) # call python function in response to the hotstring
 ```
 
+You can also remove hotstrings:
+
+```python
+ahk.remove_hotstring('btw')  # remove hotkey by the trigger sequence
+ahk.clear_hotstrings()  # remove all registered hotstrings
+```
+
 ## Mouse
 
 ```python
 from ahk import AHK
 
 ahk = AHK()
```

### Comparing `ahk-1.1.3rc2/ahk/__init__.py` & `ahk-1.2.0rc1/ahk/__init__.py`

 * *Files identical despite different names*

### Comparing `ahk-1.1.3rc2/ahk/_async/engine.py` & `ahk-1.2.0rc1/ahk/_async/engine.py`

 * *Files 0% similar despite different names*

```diff
@@ -185,14 +185,35 @@
         with warnings.catch_warnings(record=True) as caught_warnings:
             self._transport.add_hotstring(hotstring=hotstring)
         if caught_warnings:
             for warning in caught_warnings:
                 warnings.warn(warning.message, warning.category, stacklevel=2)
         return None
 
+    def remove_hotkey(self, keyname: str) -> None:
+        def _() -> None:
+            return None
+
+        h = Hotkey(keyname=keyname, callback=_)  # XXX: this can probably be avoided
+        self._transport.remove_hotkey(hotkey=h)
+        return None
+
+    def clear_hotkeys(self) -> None:
+        self._transport.clear_hotkeys()
+        return None
+
+    def remove_hotstring(self, trigger: str) -> None:
+        hs = Hotstring(trigger=trigger, replacement_or_callback='')  # XXX: this can probably be avoided
+        self._transport.remove_hotstring(hs)
+        return None
+
+    def clear_hotstrings(self) -> None:
+        self._transport.clear_hotstrings()
+        return None
+
     async def set_title_match_mode(self, title_match_mode: TitleMatchMode, /) -> None:
         """
         Sets the default title match mode
 
         Does not affect methods called with ``blocking=True`` (because these run in a separate AHK process)
 
         Reference: https://www.autohotkey.com/docs/commands/SetTitleMatchMode.htm
```

### Comparing `ahk-1.1.3rc2/ahk/_async/transport.py` & `ahk-1.2.0rc1/ahk/_async/transport.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 import asyncio.subprocess
 import atexit
 import os
 import subprocess
 import sys
 import tempfile
+import threading
 import warnings
 from abc import ABC
 from abc import abstractmethod
 from io import BytesIO
 from shutil import which
 from typing import Any
 from typing import Callable
@@ -357,14 +358,30 @@
         with warnings.catch_warnings(record=True) as caught_warnings:
             self._hotkey_transport.add_hotstring(hotstring=hotstring)
         if caught_warnings:
             for warning in caught_warnings:
                 warnings.warn(warning.message, warning.category, stacklevel=2)
         return None
 
+    def remove_hotkey(self, hotkey: Hotkey) -> None:
+        self._hotkey_transport.remove_hotkey(hotkey)
+        return None
+
+    def clear_hotkeys(self) -> None:
+        self._hotkey_transport.clear_hotkeys()
+        return None
+
+    def remove_hotstring(self, hotstring: Hotstring) -> None:
+        self._hotkey_transport.remove_hotstring(hotstring)
+        return None
+
+    def clear_hotstrings(self) -> None:
+        self._hotkey_transport.clear_hotstrings()
+        return None
+
     def start_hotkeys(self) -> None:
         return self._hotkey_transport.start()
 
     def stop_hotkeys(self) -> None:
         return self._hotkey_transport.stop()
 
     async def init(self) -> None:
@@ -627,14 +644,16 @@
         template: Optional[jinja2.Template] = None,
     ):
         self._proc: Optional[AsyncAHKProcess]
         self._proc = None
         self._temp_script: Optional[str] = None
         self.__template: jinja2.Template
         self._jinja_env: jinja2.Environment
+        self._execution_lock = threading.Lock()
+        self._a_execution_lock = asyncio.Lock()  # unasync: remove
         if jinja_loader is None:
             try:
                 loader: jinja2.BaseLoader
                 loader = jinja2.PackageLoader('ahk', 'templates')
             except ValueError:
                 # see: https://github.com/spyoungtech/ahk/issues/201
                 warnings.warn(
@@ -663,26 +682,32 @@
         await self.start()
         await super().init()
         return None
 
     async def start(self) -> None:
         assert self._proc is None, 'cannot start a process twice'
         with warnings.catch_warnings(record=True) as caught_warnings:
-            self._proc = await self._create_process()
+            async with self.lock:
+                self._proc = await self._create_process()
         if caught_warnings:
             for warning in caught_warnings:
                 warnings.warn(warning.message, warning.category, stacklevel=2)
 
     def _render_script(self, template: Optional[jinja2.Template] = None, **kwargs: Any) -> str:
         if template is None:
             template = self._template
         kwargs['daemon'] = self.__template
         message_types = {str(tom, 'utf-8'): c.__name__.upper() for tom, c in _message_registry.items()}
         return template.render(directives=self._directives, message_types=message_types, **kwargs)
 
+    @property
+    def lock(self) -> Any:
+        return self._a_execution_lock  # unasync: remove
+        return self._execution_lock
+
     async def _create_process(
         self, template: Optional[jinja2.Template] = None, **template_kwargs: Any
     ) -> AsyncAHKProcess:
         if template is None:
             if template_kwargs:
                 raise ValueError('template kwargs were specified, but no template was provided')
             if self._temp_script is None or not os.path.exists(self._temp_script):
@@ -716,15 +741,21 @@
             proc.write(msg)
             await proc.adrain_stdin()
             tom = await proc.readline()
             num_lines = await proc.readline()
             content_buffer = BytesIO()
             content_buffer.write(tom)
             content_buffer.write(num_lines)
-            for _ in range(int(num_lines) + 1):
+            try:
+                lines_to_read = int(num_lines) + 1
+            except ValueError as e:
+                raise AHKProtocolError(
+                    'Unexpected data received. This is usually the result of an unhandled error in the AHK process.'
+                ) from e
+            for _ in range(lines_to_read):
                 part = await proc.readline()
                 content_buffer.write(part)
             content = content_buffer.getvalue()[:-1]
         finally:
             try:
                 proc.kill()
             except:  # noqa
@@ -754,33 +785,34 @@
         return FutureResult(fut)
 
     async def send(
         self, request: RequestMessage, engine: Optional[AsyncAHK] = None
     ) -> Union[None, Tuple[int, int], int, str, bool, AsyncWindow, List[AsyncWindow], List[AsyncControl]]:
         msg = request.format()
         assert self._proc is not None
-        self._proc.write(msg)
-        await self._proc.adrain_stdin()
-        tom = await self._proc.readline()
-        num_lines = await self._proc.readline()
-        content_buffer = BytesIO()
-        content_buffer.write(tom)
-        content_buffer.write(num_lines)
-        try:
-            lines_to_read = int(num_lines) + 1
-        except ValueError:
-            raise AHKProtocolError(
-                'Unexpected data received. This is usually the result of an unhandled error in the AHK process.'
-            )
-        for _ in range(lines_to_read):
-            part = await self._proc.readline()
-            content_buffer.write(part)
-        content = content_buffer.getvalue()[:-1]
-        response = ResponseMessage.from_bytes(content, engine=engine)
-        return response.unpack()  # type: ignore
+        async with self.lock:
+            self._proc.write(msg)
+            await self._proc.adrain_stdin()
+            tom = await self._proc.readline()
+            num_lines = await self._proc.readline()
+            content_buffer = BytesIO()
+            content_buffer.write(tom)
+            content_buffer.write(num_lines)
+            try:
+                lines_to_read = int(num_lines) + 1
+            except ValueError as e:
+                raise AHKProtocolError(
+                    'Unexpected data received. This is usually the result of an unhandled error in the AHK process.'
+                ) from e
+            for _ in range(lines_to_read):
+                part = await self._proc.readline()
+                content_buffer.write(part)
+            content = content_buffer.getvalue()[:-1]
+            response = ResponseMessage.from_bytes(content, engine=engine)
+            return response.unpack()  # type: ignore
 
     async def _async_run_nonblocking(  # unasync: remove
         self, proc: Communicable, script_bytes: Optional[bytes], timeout: Optional[int] = None
     ) -> AsyncFutureResult[str]:
         loop = asyncio.get_running_loop()
 
         async def f() -> str:
```

### Comparing `ahk-1.1.3rc2/ahk/_async/window.py` & `ahk-1.2.0rc1/ahk/_async/window.py`

 * *Files identical despite different names*

### Comparing `ahk-1.1.3rc2/ahk/_constants.py` & `ahk-1.2.0rc1/ahk/_constants.py`

 * *Files identical despite different names*

### Comparing `ahk-1.1.3rc2/ahk/_hotkey.py` & `ahk-1.2.0rc1/ahk/_hotkey.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import atexit
 import functools
 import os
 import re
 import subprocess
 import sys
 import threading
+import time
 import warnings
 from abc import ABC
 from abc import abstractmethod
 from base64 import b64encode
 from typing import Any
 from typing import Callable
 from typing import Dict
@@ -98,14 +99,46 @@
         self._hotstrings[hotstring._id] = hotstring
         self._get_callback_registry.cache_clear()
         if self._running:
             self.restart()
         # TODO: add support for adding IfWinActive/IfWinExist
         return None
 
+    def remove_hotkey(self, hotkey: Hotkey) -> None:
+        if hotkey._id not in self._callback_registry:
+            raise ValueError(f'Hotkey {hotkey.keyname!r} is not registered')
+        del self._hotkeys[hotkey._id]
+        self._get_callback_registry.cache_clear()
+        if self._running:
+            self.restart()
+        return None
+
+    def clear_hotkeys(self) -> None:
+        self._hotkeys.clear()
+        self._get_callback_registry.cache_clear()
+        if self._running:
+            self.restart()
+        return None
+
+    def remove_hotstring(self, hotstring: Hotstring) -> None:
+        if hotstring._id not in self._callback_registry:
+            raise ValueError(f'Hostring {hotstring.trigger!r} is not registered')
+        del self._hotstrings[hotstring._id]
+        self._get_callback_registry.cache_clear()
+        if self._running:
+            self.restart()
+        return None
+
+    def clear_hotstrings(self) -> None:
+        self._hotstrings.clear()
+        self._get_callback_registry.cache_clear()
+        if self._running:
+            self.restart()
+        return None
+
     def on_clipboard_change(
         self, callback: Callable[[int], Any], ex_handler: Optional[Callable[[int, Exception], Any]] = None
     ) -> None:
         self._clipboard_callback = callback
         if ex_handler is not None:
             self._clipboard_ex_handler = ex_handler
         if self._running:
@@ -166,14 +199,21 @@
         self._listener_thread = listener_thread
         listener_thread.start()
         dispatcher_thread = threading.Thread(target=self.dispatcher, daemon=True)
         self._dispatcher_thread = dispatcher_thread
         dispatcher_thread.start()
 
     def stop(self) -> None:
+        assert self._running is True, 'Not running! Must be started first!'
+        assert self._dispatcher_thread is not None
+        for i in range(1, 6):
+            if self._proc is not None:
+                break
+            logging.debug(f'stop called before dispatched has started proc. Waiting for proc ({i}/5)')
+            time.sleep(0.2)
         assert self._proc is not None
         self._running = False
 
         self._callback_queue.empty()
         self._callback_queue.put_nowait(STOP)
         logging.debug('Waiting for stop...')
         if self._dispatcher_thread is not None:
```

### Comparing `ahk-1.1.3rc2/ahk/_sync/engine.py` & `ahk-1.2.0rc1/ahk/_sync/engine.py`

 * *Files 0% similar despite different names*

```diff
@@ -181,14 +181,35 @@
         with warnings.catch_warnings(record=True) as caught_warnings:
             self._transport.add_hotstring(hotstring=hotstring)
         if caught_warnings:
             for warning in caught_warnings:
                 warnings.warn(warning.message, warning.category, stacklevel=2)
         return None
 
+    def remove_hotkey(self, keyname: str) -> None:
+        def _() -> None:
+            return None
+        h = Hotkey(keyname=keyname, callback=_)  # XXX: this can probably be avoided
+        self._transport.remove_hotkey(hotkey=h)
+        return None
+
+    def clear_hotkeys(self) -> None:
+        self._transport.clear_hotkeys()
+        return None
+
+    def remove_hotstring(self, trigger: str) -> None:
+        hs = Hotstring(trigger=trigger, replacement_or_callback='')  # XXX: this can probably be avoided
+        self._transport.remove_hotstring(hs)
+        return None
+
+    def clear_hotstrings(self) -> None:
+        self._transport.clear_hotstrings()
+        return None
+
+
     def set_title_match_mode(self, title_match_mode: TitleMatchMode, /) -> None:
         """
         Sets the default title match mode
 
         Does not affect methods called with ``blocking=True`` (because these run in a separate AHK process)
 
         Reference: https://www.autohotkey.com/docs/commands/SetTitleMatchMode.htm
@@ -2689,14 +2710,15 @@
             opts = ' '.join(f'*{opt}' for opt in options)
             args.append(opts + f' {image_path}')
         else:
             args.append(image_path)
 
         if coord_mode is not None:
             args.append(coord_mode)
+
         resp = self._transport.function_call('AHKImageSearch', args, blocking=blocking)
         return resp
 
     def mouse_drag(
         self,
         x: int,
         y: int,
```

### Comparing `ahk-1.1.3rc2/ahk/_sync/transport.py` & `ahk-1.2.0rc1/ahk/_sync/transport.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 import asyncio.subprocess
 import atexit
 import os
 import subprocess
 import sys
 import tempfile
+import threading
 import warnings
 from abc import ABC
 from abc import abstractmethod
 from io import BytesIO
 from shutil import which
 from typing import Any
 from typing import Callable
@@ -338,14 +339,33 @@
         with warnings.catch_warnings(record=True) as caught_warnings:
             self._hotkey_transport.add_hotstring(hotstring=hotstring)
         if caught_warnings:
             for warning in caught_warnings:
                 warnings.warn(warning.message, warning.category, stacklevel=2)
         return None
 
+    def remove_hotkey(self, hotkey: Hotkey) -> None:
+        self._hotkey_transport.remove_hotkey(hotkey)
+        return None
+
+    def clear_hotkeys(self) -> None:
+        self._hotkey_transport.clear_hotkeys()
+        return None
+
+    def remove_hotstring(self, hotstring: Hotstring) -> None:
+        self._hotkey_transport.remove_hotstring(hotstring)
+        return None
+
+    def clear_hotstrings(self) -> None:
+        self._hotkey_transport.clear_hotstrings()
+        return None
+
+
+
+
     def start_hotkeys(self) -> None:
         return self._hotkey_transport.start()
 
     def stop_hotkeys(self) -> None:
         return self._hotkey_transport.stop()
 
     def init(self) -> None:
@@ -601,14 +621,15 @@
         template: Optional[jinja2.Template] = None,
     ):
         self._proc: Optional[SyncAHKProcess]
         self._proc = None
         self._temp_script: Optional[str] = None
         self.__template: jinja2.Template
         self._jinja_env: jinja2.Environment
+        self._execution_lock = threading.Lock()
         if jinja_loader is None:
             try:
                 loader: jinja2.BaseLoader
                 loader = jinja2.PackageLoader('ahk', 'templates')
             except ValueError:
                 # see: https://github.com/spyoungtech/ahk/issues/201
                 warnings.warn(
@@ -637,26 +658,31 @@
         self.start()
         super().init()
         return None
 
     def start(self) -> None:
         assert self._proc is None, 'cannot start a process twice'
         with warnings.catch_warnings(record=True) as caught_warnings:
-            self._proc = self._create_process()
+            with self.lock:
+                self._proc = self._create_process()
         if caught_warnings:
             for warning in caught_warnings:
                 warnings.warn(warning.message, warning.category, stacklevel=2)
 
     def _render_script(self, template: Optional[jinja2.Template] = None, **kwargs: Any) -> str:
         if template is None:
             template = self._template
         kwargs['daemon'] = self.__template
         message_types = {str(tom, 'utf-8'): c.__name__.upper() for tom, c in _message_registry.items()}
         return template.render(directives=self._directives, message_types=message_types, **kwargs)
 
+    @property
+    def lock(self) -> Any:
+        return self._execution_lock
+
     def _create_process(
         self, template: Optional[jinja2.Template] = None, **template_kwargs: Any
     ) -> SyncAHKProcess:
         if template is None:
             if template_kwargs:
                 raise ValueError('template kwargs were specified, but no template was provided')
             if self._temp_script is None or not os.path.exists(self._temp_script):
@@ -690,15 +716,21 @@
             proc.write(msg)
             proc.drain_stdin()
             tom = proc.readline()
             num_lines = proc.readline()
             content_buffer = BytesIO()
             content_buffer.write(tom)
             content_buffer.write(num_lines)
-            for _ in range(int(num_lines) + 1):
+            try:
+                lines_to_read = int(num_lines) + 1
+            except ValueError as e:
+                raise AHKProtocolError(
+                    'Unexpected data received. This is usually the result of an unhandled error in the AHK process.'
+                ) from e
+            for _ in range(lines_to_read):
                 part = proc.readline()
                 content_buffer.write(part)
             content = content_buffer.getvalue()[:-1]
         finally:
             try:
                 proc.kill()
             except:  # noqa
@@ -720,33 +752,34 @@
         return FutureResult(fut)
 
     def send(
         self, request: RequestMessage, engine: Optional[AHK] = None
     ) -> Union[None, Tuple[int, int], int, str, bool, Window, List[Window], List[Control]]:
         msg = request.format()
         assert self._proc is not None
-        self._proc.write(msg)
-        self._proc.drain_stdin()
-        tom = self._proc.readline()
-        num_lines = self._proc.readline()
-        content_buffer = BytesIO()
-        content_buffer.write(tom)
-        content_buffer.write(num_lines)
-        try:
-            lines_to_read = int(num_lines) + 1
-        except ValueError:
-            raise AHKProtocolError(
-                'Unexpected data received. This is usually the result of an unhandled error in the AHK process.'
-            )
-        for _ in range(lines_to_read):
-            part = self._proc.readline()
-            content_buffer.write(part)
-        content = content_buffer.getvalue()[:-1]
-        response = ResponseMessage.from_bytes(content, engine=engine)
-        return response.unpack()  # type: ignore
+        with self.lock:
+            self._proc.write(msg)
+            self._proc.drain_stdin()
+            tom = self._proc.readline()
+            num_lines = self._proc.readline()
+            content_buffer = BytesIO()
+            content_buffer.write(tom)
+            content_buffer.write(num_lines)
+            try:
+                lines_to_read = int(num_lines) + 1
+            except ValueError as e:
+                raise AHKProtocolError(
+                    'Unexpected data received. This is usually the result of an unhandled error in the AHK process.'
+                ) from e
+            for _ in range(lines_to_read):
+                part = self._proc.readline()
+                content_buffer.write(part)
+            content = content_buffer.getvalue()[:-1]
+            response = ResponseMessage.from_bytes(content, engine=engine)
+            return response.unpack()  # type: ignore
 
 
     def _sync_run_nonblocking(
         self,
         proc: Communicable,
         script_bytes: Optional[bytes],
         timeout: Optional[int] = None,
```

### Comparing `ahk-1.1.3rc2/ahk/_sync/window.py` & `ahk-1.2.0rc1/ahk/_sync/window.py`

 * *Files identical despite different names*

### Comparing `ahk-1.1.3rc2/ahk/_utils.py` & `ahk-1.2.0rc1/ahk/_utils.py`

 * *Files identical despite different names*

### Comparing `ahk-1.1.3rc2/ahk/directives.py` & `ahk-1.2.0rc1/ahk/directives.py`

 * *Files identical despite different names*

### Comparing `ahk-1.1.3rc2/ahk/keys.py` & `ahk-1.2.0rc1/ahk/keys.py`

 * *Files identical despite different names*

### Comparing `ahk-1.1.3rc2/ahk/message.py` & `ahk-1.2.0rc1/ahk/message.py`

 * *Files identical despite different names*

### Comparing `ahk-1.1.3rc2/ahk/templates/daemon.ahk` & `ahk-1.2.0rc1/ahk/templates/daemon.ahk`

 * *Files identical despite different names*

### Comparing `ahk-1.1.3rc2/ahk/templates/hotkeys.ahk` & `ahk-1.2.0rc1/ahk/templates/hotkeys.ahk`

 * *Files identical despite different names*

### Comparing `ahk-1.1.3rc2/ahk.egg-info/PKG-INFO` & `ahk-1.2.0rc1/ahk.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ahk
-Version: 1.1.3rc2
+Version: 1.2.0rc1
 Summary: A Python wrapper for AHK
 Home-page: https://github.com/spyoungtech/ahk
 Author: Spencer Young
 Author-email: spencer.young@spyoung.com
 Keywords: ahk,autohotkey,windows,mouse,keyboard,automation,pyautogui
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Desktop Environment
@@ -91,20 +91,28 @@
 
 def my_ex_handler(hotkey: str, exception: Exception):
     print('exception with callback for hotkey', hotkey, 'Here was the error:', exception)
 
 ahk.add_hotkey('#n', callback=go_boom, ex_handler=my_ex_handler)
 ```
 
+There are also methods for removing hotkeys:
+
+```python
+# ...
+ahk.remove_hotkey('#n') # remove a hotkey by its keyname
+ahk.clear_hotkeys()  # remove all hotkeys
+```
+
 Note that:
 
 - Hotkeys run in a separate process that must be started manually (with `ahk.start_hotkeys()`)
 - Hotkeys can be stopped with `ahk.stop_hotkeys()` (will not stop actively running callbacks)
 - Hotstrings (discussed below) share the same process with hotkeys and are started/stopped in the same manner
-- If hotkeys or hotstrings are added while the process is running, the underlying AHK process is restarted automatically
+- If hotkeys or hotstrings are added or removed while the process is running, the underlying AHK process is restarted automatically
 
 
 See also the [relevant AHK documentation](https://www.autohotkey.com/docs/Hotkeys.htm)
 
 ## Hotstrings
 
 
@@ -119,14 +127,21 @@
 def my_callback():
     print('hello callback!')
 
 ahk.add_hotstring('btw', 'by the way')  # string replacements
 ahk.add_hotstring('btw', my_callback) # call python function in response to the hotstring
 ```
 
+You can also remove hotstrings:
+
+```python
+ahk.remove_hotstring('btw')  # remove hotkey by the trigger sequence
+ahk.clear_hotstrings()  # remove all registered hotstrings
+```
+
 ## Mouse
 
 ```python
 from ahk import AHK
 
 ahk = AHK()
```

### Comparing `ahk-1.1.3rc2/ahk.egg-info/SOURCES.txt` & `ahk-1.2.0rc1/ahk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ahk-1.1.3rc2/buildunasync.py` & `ahk-1.2.0rc1/buildunasync.py`

 * *Files identical despite different names*

### Comparing `ahk-1.1.3rc2/docs/README.md` & `ahk-1.2.0rc1/docs/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -68,20 +68,28 @@
 
 def my_ex_handler(hotkey: str, exception: Exception):
     print('exception with callback for hotkey', hotkey, 'Here was the error:', exception)
 
 ahk.add_hotkey('#n', callback=go_boom, ex_handler=my_ex_handler)
 ```
 
+There are also methods for removing hotkeys:
+
+```python
+# ...
+ahk.remove_hotkey('#n') # remove a hotkey by its keyname
+ahk.clear_hotkeys()  # remove all hotkeys
+```
+
 Note that:
 
 - Hotkeys run in a separate process that must be started manually (with `ahk.start_hotkeys()`)
 - Hotkeys can be stopped with `ahk.stop_hotkeys()` (will not stop actively running callbacks)
 - Hotstrings (discussed below) share the same process with hotkeys and are started/stopped in the same manner
-- If hotkeys or hotstrings are added while the process is running, the underlying AHK process is restarted automatically
+- If hotkeys or hotstrings are added or removed while the process is running, the underlying AHK process is restarted automatically
 
 
 See also the [relevant AHK documentation](https://www.autohotkey.com/docs/Hotkeys.htm)
 
 ## Hotstrings
 
 
@@ -96,14 +104,21 @@
 def my_callback():
     print('hello callback!')
 
 ahk.add_hotstring('btw', 'by the way')  # string replacements
 ahk.add_hotstring('btw', my_callback) # call python function in response to the hotstring
 ```
 
+You can also remove hotstrings:
+
+```python
+ahk.remove_hotstring('btw')  # remove hotkey by the trigger sequence
+ahk.clear_hotstrings()  # remove all registered hotstrings
+```
+
 ## Mouse
 
 ```python
 from ahk import AHK
 
 ahk = AHK()
```

### Comparing `ahk-1.1.3rc2/setup.cfg` & `ahk-1.2.0rc1/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ahk
-version = 1.1.3rc2
+version = 1.2.0rc1
 author_email = spencer.young@spyoung.com
 author = Spencer Young
 description = A Python wrapper for AHK
 long_description = file: docs/README.md
 long_description_content_type = text/markdown
 url = https://github.com/spyoungtech/ahk
 keywords =
```

