# Comparing `tmp/ex4nicegui-0.1.0.tar.gz` & `tmp/ex4nicegui-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ex4nicegui-0.1.0.tar", last modified: Wed Jul  5 06:12:10 2023, max compression
+gzip compressed data, was "ex4nicegui-0.1.1.tar", last modified: Sat Jul  8 17:56:04 2023, max compression
```

## Comparing `ex4nicegui-0.1.0.tar` & `ex4nicegui-0.1.1.tar`

### file list

```diff
@@ -1,39 +1,45 @@
-drwxrwxrwx   0        0        0        0 2023-07-05 06:12:10.744091 ex4nicegui-0.1.0/
--rw-rw-rw-   0        0        0     1094 2023-06-30 08:17:10.000000 ex4nicegui-0.1.0/LICENSE
--rw-rw-rw-   0        0        0      481 2023-07-05 06:12:10.743094 ex4nicegui-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0       12 2023-07-05 06:11:55.000000 ex4nicegui-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-05 06:12:10.644719 ex4nicegui-0.1.0/ex4nicegui/
--rw-rw-rw-   0        0        0      240 2023-07-05 06:10:00.000000 ex4nicegui-0.1.0/ex4nicegui/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-05 06:12:10.664640 ex4nicegui-0.1.0/ex4nicegui/layout/
--rw-rw-rw-   0        0        0       31 2023-07-05 06:10:00.000000 ex4nicegui-0.1.0/ex4nicegui/layout/__init__.py
--rw-rw-rw-   0        0        0     2378 2023-07-05 06:10:00.000000 ex4nicegui-0.1.0/ex4nicegui/layout/gridbox.py
-drwxrwxrwx   0        0        0        0 2023-07-05 06:12:10.678618 ex4nicegui-0.1.0/ex4nicegui/reactive/
--rw-rw-rw-   0        0        0      457 2023-07-05 06:10:00.000000 ex4nicegui-0.1.0/ex4nicegui/reactive/__index.py
--rw-rw-rw-   0        0        0       24 2023-07-05 06:10:00.000000 ex4nicegui-0.1.0/ex4nicegui/reactive/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-05 06:12:10.684588 ex4nicegui-0.1.0/ex4nicegui/reactive/draggable/
--rw-rw-rw-   0        0        0     4851 2023-07-05 06:10:00.000000 ex4nicegui-0.1.0/ex4nicegui/reactive/draggable/UseDraggable.js
--rw-rw-rw-   0        0        0     2667 2023-07-05 06:10:00.000000 ex4nicegui-0.1.0/ex4nicegui/reactive/draggable/UseDraggable.py
--rw-rw-rw-   0        0        0        0 2023-07-05 06:10:00.000000 ex4nicegui-0.1.0/ex4nicegui/reactive/draggable/__init__.py
--rw-rw-rw-   0        0        0     1320 2023-07-05 06:10:00.000000 ex4nicegui-0.1.0/ex4nicegui/reactive/drawer.py
-drwxrwxrwx   0        0        0        0 2023-07-05 06:12:10.693092 ex4nicegui-0.1.0/ex4nicegui/reactive/echarts/
--rw-rw-rw-   0        0        0  1581614 2023-07-05 06:10:00.000000 ex4nicegui-0.1.0/ex4nicegui/reactive/echarts/ECharts.js
--rw-rw-rw-   0        0        0     2709 2023-07-05 06:10:00.000000 ex4nicegui-0.1.0/ex4nicegui/reactive/echarts/ECharts.py
--rw-rw-rw-   0        0        0        0 2023-07-05 06:10:00.000000 ex4nicegui-0.1.0/ex4nicegui/reactive/echarts/__init__.py
--rw-rw-rw-   0        0        0     5959 2023-07-05 06:10:00.000000 ex4nicegui-0.1.0/ex4nicegui/reactive/local_file_picker.py
--rw-rw-rw-   0        0        0     4787 2023-07-05 06:10:00.000000 ex4nicegui-0.1.0/ex4nicegui/reactive/official.py
--rw-rw-rw-   0        0        0     6761 2023-07-05 06:10:00.000000 ex4nicegui-0.1.0/ex4nicegui/reactive/ref.py
--rw-rw-rw-   0        0        0      803 2023-07-05 06:10:00.000000 ex4nicegui-0.1.0/ex4nicegui/reactive/signature.py
-drwxrwxrwx   0        0        0        0 2023-07-05 06:12:10.741099 ex4nicegui-0.1.0/ex4nicegui/utils/
--rw-rw-rw-   0        0        0        0 2023-07-05 06:10:00.000000 ex4nicegui-0.1.0/ex4nicegui/utils/__init__.py
--rw-rw-rw-   0        0        0      136 2023-07-05 06:10:00.000000 ex4nicegui-0.1.0/ex4nicegui/utils/common.py
--rw-rw-rw-   0        0        0     1977 2023-07-05 06:10:00.000000 ex4nicegui-0.1.0/ex4nicegui/utils/signals.py
--rw-rw-rw-   0        0        0      910 2023-07-05 06:10:00.000000 ex4nicegui-0.1.0/ex4nicegui/utils/types.py
-drwxrwxrwx   0        0        0        0 2023-07-05 06:12:10.661037 ex4nicegui-0.1.0/ex4nicegui.egg-info/
--rw-rw-rw-   0        0        0      481 2023-07-05 06:12:10.000000 ex4nicegui-0.1.0/ex4nicegui.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      898 2023-07-05 06:12:10.000000 ex4nicegui-0.1.0/ex4nicegui.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-05 06:12:10.000000 ex4nicegui-0.1.0/ex4nicegui.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-07-05 06:12:10.000000 ex4nicegui-0.1.0/ex4nicegui.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       32 2023-07-05 06:12:10.000000 ex4nicegui-0.1.0/ex4nicegui.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-07-05 06:12:10.000000 ex4nicegui-0.1.0/ex4nicegui.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-05 06:12:10.744091 ex4nicegui-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1533 2023-07-05 06:10:00.000000 ex4nicegui-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-08 17:56:04.549298 ex4nicegui-0.1.1/
+-rw-rw-rw-   0        0        0     1094 2023-06-30 08:17:10.000000 ex4nicegui-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0      481 2023-07-08 17:56:04.535102 ex4nicegui-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0       12 2023-07-05 06:11:55.000000 ex4nicegui-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-08 17:56:04.447999 ex4nicegui-0.1.1/ex4nicegui/
+-rw-rw-rw-   0        0        0      366 2023-07-08 17:55:31.000000 ex4nicegui-0.1.1/ex4nicegui/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-08 17:56:04.462315 ex4nicegui-0.1.1/ex4nicegui/layout/
+-rw-rw-rw-   0        0        0       31 2023-07-05 06:10:00.000000 ex4nicegui-0.1.1/ex4nicegui/layout/__init__.py
+-rw-rw-rw-   0        0        0     2378 2023-07-05 06:10:00.000000 ex4nicegui-0.1.1/ex4nicegui/layout/gridbox.py
+drwxrwxrwx   0        0        0        0 2023-07-08 17:56:04.474210 ex4nicegui-0.1.1/ex4nicegui/reactive/
+-rw-rw-rw-   0        0        0      829 2023-07-08 17:55:18.000000 ex4nicegui-0.1.1/ex4nicegui/reactive/__index.py
+-rw-rw-rw-   0        0        0       24 2023-07-05 06:10:00.000000 ex4nicegui-0.1.1/ex4nicegui/reactive/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-08 17:56:04.478167 ex4nicegui-0.1.1/ex4nicegui/reactive/draggable/
+-rw-rw-rw-   0        0        0     4851 2023-07-05 09:28:02.000000 ex4nicegui-0.1.1/ex4nicegui/reactive/draggable/UseDraggable.js
+-rw-rw-rw-   0        0        0     3041 2023-07-08 17:55:18.000000 ex4nicegui-0.1.1/ex4nicegui/reactive/draggable/UseDraggable.py
+-rw-rw-rw-   0        0        0        0 2023-07-05 06:10:00.000000 ex4nicegui-0.1.1/ex4nicegui/reactive/draggable/__init__.py
+-rw-rw-rw-   0        0        0     1320 2023-07-05 06:10:00.000000 ex4nicegui-0.1.1/ex4nicegui/reactive/drawer.py
+drwxrwxrwx   0        0        0        0 2023-07-08 17:56:04.521402 ex4nicegui-0.1.1/ex4nicegui/reactive/echarts/
+-rw-rw-rw-   0        0        0  1581614 2023-07-05 06:10:00.000000 ex4nicegui-0.1.1/ex4nicegui/reactive/echarts/ECharts.js
+-rw-rw-rw-   0        0        0     2709 2023-07-05 06:10:00.000000 ex4nicegui-0.1.1/ex4nicegui/reactive/echarts/ECharts.py
+-rw-rw-rw-   0        0        0        0 2023-07-05 06:10:00.000000 ex4nicegui-0.1.1/ex4nicegui/reactive/echarts/__init__.py
+-rw-rw-rw-   0        0        0     6100 2023-07-08 17:55:18.000000 ex4nicegui-0.1.1/ex4nicegui/reactive/local_file_picker.py
+-rw-rw-rw-   0        0        0     1041 2023-07-08 17:55:18.000000 ex4nicegui-0.1.1/ex4nicegui/reactive/official.py
+-rw-rw-rw-   0        0        0    25676 2023-07-08 17:55:18.000000 ex4nicegui-0.1.1/ex4nicegui/reactive/ref.py
+-rw-rw-rw-   0        0        0      803 2023-07-05 06:10:00.000000 ex4nicegui-0.1.1/ex4nicegui/reactive/signature.py
+drwxrwxrwx   0        0        0        0 2023-07-08 17:56:04.524100 ex4nicegui-0.1.1/ex4nicegui/reactive/useMouse/
+-rw-rw-rw-   0        0        0     2244 2023-07-08 17:55:18.000000 ex4nicegui-0.1.1/ex4nicegui/reactive/useMouse/UseMouse.py
+-rw-rw-rw-   0        0        0        0 2023-07-08 17:55:18.000000 ex4nicegui-0.1.1/ex4nicegui/reactive/useMouse/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-08 17:56:04.527096 ex4nicegui-0.1.1/ex4nicegui/tools/
+-rw-rw-rw-   0        0        0       40 2023-07-08 17:55:18.000000 ex4nicegui-0.1.1/ex4nicegui/tools/__init__.py
+-rw-rw-rw-   0        0        0     5024 2023-07-08 17:55:18.000000 ex4nicegui-0.1.1/ex4nicegui/tools/debug.py
+drwxrwxrwx   0        0        0        0 2023-07-08 17:56:04.533080 ex4nicegui-0.1.1/ex4nicegui/utils/
+-rw-rw-rw-   0        0        0        0 2023-07-05 06:10:00.000000 ex4nicegui-0.1.1/ex4nicegui/utils/__init__.py
+-rw-rw-rw-   0        0        0      430 2023-07-08 17:55:18.000000 ex4nicegui-0.1.1/ex4nicegui/utils/common.py
+-rw-rw-rw-   0        0        0     4404 2023-07-08 17:55:18.000000 ex4nicegui-0.1.1/ex4nicegui/utils/signals.py
+-rw-rw-rw-   0        0        0      910 2023-07-05 06:10:00.000000 ex4nicegui-0.1.1/ex4nicegui/utils/types.py
+drwxrwxrwx   0        0        0        0 2023-07-08 17:56:04.459321 ex4nicegui-0.1.1/ex4nicegui.egg-info/
+-rw-rw-rw-   0        0        0      481 2023-07-08 17:56:04.000000 ex4nicegui-0.1.1/ex4nicegui.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1035 2023-07-08 17:56:04.000000 ex4nicegui-0.1.1/ex4nicegui.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-08 17:56:04.000000 ex4nicegui-0.1.1/ex4nicegui.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-08 17:56:04.000000 ex4nicegui-0.1.1/ex4nicegui.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       32 2023-07-08 17:56:04.000000 ex4nicegui-0.1.1/ex4nicegui.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-07-08 17:56:04.000000 ex4nicegui-0.1.1/ex4nicegui.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-08 17:56:04.549298 ex4nicegui-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1533 2023-07-05 06:10:00.000000 ex4nicegui-0.1.1/setup.py
```

### Comparing `ex4nicegui-0.1.0/LICENSE` & `ex4nicegui-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.1.0/ex4nicegui/layout/gridbox.py` & `ex4nicegui-0.1.1/ex4nicegui/layout/gridbox.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.1.0/ex4nicegui/reactive/draggable/UseDraggable.js` & `ex4nicegui-0.1.1/ex4nicegui/reactive/draggable/UseDraggable.js`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.1.0/ex4nicegui/reactive/draggable/UseDraggable.py` & `ex4nicegui-0.1.1/ex4nicegui/reactive/draggable/UseDraggable.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from typing import Any, Callable, Optional
 from dataclasses import dataclass
+from nicegui import ui
 from nicegui.helpers import KWONLY_SLOTS
 from nicegui.events import handle_event, EventArguments
 from nicegui.dependencies import register_component
 from nicegui.element import Element
-from signe import createSignal, effect
-
+from signe import createSignal, effect, batch
+from ex4nicegui.utils.signals import ref_from_signal
 
 register_component("UseDraggable", __file__, "UseDraggable.js")
 
 _Update_Args = [
     "x",
     "y",
     "style",
@@ -19,61 +20,64 @@
 @dataclass(**KWONLY_SLOTS)
 class UseDraggableUpdateEventArguments(EventArguments):
     x: float
     y: float
     style: str
 
 
-def use_draggable(element: Element, auto_bind_style=True):
-    ud = UseDraggable(element)
+def use_draggable(element: Element, init_x=0.0, init_y=0.0, auto_bind_style=True):
+    ud = UseDraggable(element, init_x, init_y)
     if auto_bind_style:
-        element.style(replace="position:fixed")
+        element.style(add=f"position:fixed;left:{init_x}px;top:{init_y}px")
         ud.bind_style(element)
 
     return ud
 
 
 class UseDraggable(Element):
-    def __init__(self, element: Element) -> None:
+    def __init__(self, element: Element, init_x=0.0, init_y=0.0) -> None:
         super().__init__("UseDraggable")
         self._props["elementId"] = str(element.id)
+        self._props["options"] = {"initialValue": {"x": init_x, "y": init_y}}
 
         self.__style_getter, self.__style_setter = createSignal("")
-        self.__x_getter, self.__x_setter = createSignal(0.0)
-        self.__y_getter, self.__y_setter = createSignal(0.0)
+        self.__x_getter, self.__x_setter = createSignal(init_x)
+        self.__y_getter, self.__y_setter = createSignal(init_y)
         self.__isDragging_getter, self.__isDragging_setter = createSignal(False)
 
         def update(args: UseDraggableUpdateEventArguments):
-            self.__style_setter(args.style)
-            self.__x_setter(args.x)
-            self.__y_setter(args.y)
+            @batch
+            def _():
+                self.__style_setter(args.style)
+                self.__x_setter(args.x)
+                self.__y_setter(args.y)
 
         self.on_update(update)
 
         def on_isDraggingUpdate(args):
             self.__isDragging_setter(args["args"]["isDragging"])
             # print(args['args']['isDragging'])
 
         self.on("isDraggingUpdate", on_isDraggingUpdate)
 
     @property
     def x(self):
-        return self.__x_getter()
+        return ref_from_signal(self.__x_getter)
 
     @property
     def y(self):
-        return self.__y_getter()
+        return ref_from_signal(self.__y_getter)
 
     @property
     def style(self):
-        return self.__style_getter()
+        return ref_from_signal(self.__style_getter)
 
     @property
     def is_dragging(self):
-        return self.__isDragging_getter()
+        return ref_from_signal(self.__isDragging_getter)
 
     def bind_style(self, element: Element):
         @effect
         def _():
             element.style(self.__style_getter())
             element.update()
```

### Comparing `ex4nicegui-0.1.0/ex4nicegui/reactive/drawer.py` & `ex4nicegui-0.1.1/ex4nicegui/reactive/drawer.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.1.0/ex4nicegui/reactive/echarts/ECharts.js` & `ex4nicegui-0.1.1/ex4nicegui/reactive/echarts/ECharts.js`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.1.0/ex4nicegui/reactive/echarts/ECharts.py` & `ex4nicegui-0.1.1/ex4nicegui/reactive/echarts/ECharts.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.1.0/ex4nicegui/reactive/local_file_picker.py` & `ex4nicegui-0.1.1/ex4nicegui/reactive/local_file_picker.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,35 @@
 from typing import Any, Callable, Optional, cast
 from typing_extensions import Literal
 from signe import createSignal, effect, computed
 from nicegui import ui, Tailwind
 from pathlib import Path
 
 from signe.types import TGetter
-from ex4nicegui.utils.signals import effect_refreshable, ReadonlyRef
+from ex4nicegui.utils.signals import Ref, effect_refreshable, ReadonlyRef
 
 
 SelectMode = Literal["dir", "file"]
 
 
 class LocalFilePickerResult(ReadonlyRef[str]):
     def __init__(self, getter: Callable[[], str], open_fn: Callable[..., None]) -> None:
         super().__init__(getter)
         self.__open_fn = open_fn
 
     def open(self):
         self.__open_fn()
 
+    def bind_ref(self, ref: Ref[str]):
+        @effect
+        def _():
+            ref.value = self.value
+
+        return self
+
 
 def local_file_picker(
     title: Optional[str] = None,
     dir: Optional[str] = None,
     mode: SelectMode = "file",
     ext: Optional[list[str]] = None,
 ):
```

### Comparing `ex4nicegui-0.1.0/ex4nicegui/reactive/signature.py` & `ex4nicegui-0.1.1/ex4nicegui/reactive/signature.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.1.0/ex4nicegui/utils/types.py` & `ex4nicegui-0.1.1/ex4nicegui/utils/types.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.1.0/setup.py` & `ex4nicegui-0.1.1/setup.py`

 * *Files identical despite different names*

