# Comparing `tmp/signe-0.1.5.tar.gz` & `tmp/signe-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "signe-0.1.5.tar", last modified: Fri Jul  7 13:35:33 2023, max compression
+gzip compressed data, was "signe-0.1.6.tar", last modified: Sat Jul  8 17:46:47 2023, max compression
```

## Comparing `signe-0.1.5.tar` & `signe-0.1.6.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-07-07 13:35:33.173878 signe-0.1.5/
--rw-rw-rw-   0        0        0     1088 2023-06-22 09:11:57.000000 signe-0.1.5/LICENSE
--rw-rw-rw-   0        0        0      469 2023-07-07 13:35:33.171883 signe-0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0      977 2023-06-25 14:01:29.000000 signe-0.1.5/README.md
--rw-rw-rw-   0        0        0       42 2023-07-07 13:35:33.173878 signe-0.1.5/setup.cfg
--rw-rw-rw-   0        0        0     1173 2023-06-25 12:31:47.000000 signe-0.1.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-07 13:35:33.146950 signe-0.1.5/signe/
--rw-rw-rw-   0        0        0      164 2023-07-07 13:35:16.000000 signe-0.1.5/signe/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-07 13:35:33.166896 signe-0.1.5/signe/core/
--rw-rw-rw-   0        0        0        0 2023-06-25 12:24:57.000000 signe-0.1.5/signe/core/__init__.py
--rw-rw-rw-   0        0        0      604 2023-07-06 05:25:51.000000 signe-0.1.5/signe/core/collections.py
--rw-rw-rw-   0        0        0      290 2023-06-25 12:24:57.000000 signe-0.1.5/signe/core/consts.py
--rw-rw-rw-   0        0        0     5778 2023-07-07 13:26:40.000000 signe-0.1.5/signe/core/effect.py
--rw-rw-rw-   0        0        0     2493 2023-06-25 12:24:57.000000 signe-0.1.5/signe/core/runtime.py
--rw-rw-rw-   0        0        0     2737 2023-06-25 12:24:57.000000 signe-0.1.5/signe/core/signal.py
-drwxrwxrwx   0        0        0        0 2023-07-07 13:35:33.170885 signe-0.1.5/signe/reactive/
--rw-rw-rw-   0        0        0        0 2023-06-27 15:43:57.000000 signe-0.1.5/signe/reactive/__init__.py
--rw-rw-rw-   0        0        0     7480 2023-06-25 12:24:57.000000 signe-0.1.5/signe/reactive/proxy.py
--rw-rw-rw-   0        0        0       97 2023-06-25 12:24:57.000000 signe-0.1.5/signe/types.py
--rw-rw-rw-   0        0        0     3355 2023-07-07 13:26:40.000000 signe-0.1.5/signe/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-07 13:35:33.156924 signe-0.1.5/signe.egg-info/
--rw-rw-rw-   0        0        0      469 2023-07-07 13:35:33.000000 signe-0.1.5/signe.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      403 2023-07-07 13:35:33.000000 signe-0.1.5/signe.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-07 13:35:33.000000 signe-0.1.5/signe.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-07-07 13:35:33.000000 signe-0.1.5/signe.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        6 2023-07-07 13:35:33.000000 signe-0.1.5/signe.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-08 17:46:47.984504 signe-0.1.6/
+-rw-rw-rw-   0        0        0     1088 2023-06-22 09:11:57.000000 signe-0.1.6/LICENSE
+-rw-rw-rw-   0        0        0      469 2023-07-08 17:46:47.982508 signe-0.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0      977 2023-06-25 14:01:29.000000 signe-0.1.6/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-08 17:46:47.984504 signe-0.1.6/setup.cfg
+-rw-rw-rw-   0        0        0     1173 2023-06-25 12:31:47.000000 signe-0.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-08 17:46:47.943071 signe-0.1.6/signe/
+-rw-rw-rw-   0        0        0      223 2023-07-08 17:46:37.000000 signe-0.1.6/signe/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-08 17:46:47.966704 signe-0.1.6/signe/core/
+-rw-rw-rw-   0        0        0        0 2023-06-25 12:24:57.000000 signe-0.1.6/signe/core/__init__.py
+-rw-rw-rw-   0        0        0      604 2023-07-06 05:25:51.000000 signe-0.1.6/signe/core/collections.py
+-rw-rw-rw-   0        0        0      290 2023-06-25 12:24:57.000000 signe-0.1.6/signe/core/consts.py
+-rw-rw-rw-   0        0        0     5939 2023-07-08 17:46:06.000000 signe-0.1.6/signe/core/effect.py
+-rw-rw-rw-   0        0        0     2840 2023-07-08 17:46:06.000000 signe-0.1.6/signe/core/runtime.py
+-rw-rw-rw-   0        0        0     2818 2023-07-08 17:46:06.000000 signe-0.1.6/signe/core/signal.py
+drwxrwxrwx   0        0        0        0 2023-07-08 17:46:47.970692 signe-0.1.6/signe/reactive/
+-rw-rw-rw-   0        0        0        0 2023-06-27 15:43:57.000000 signe-0.1.6/signe/reactive/__init__.py
+-rw-rw-rw-   0        0        0     7480 2023-06-25 12:24:57.000000 signe-0.1.6/signe/reactive/proxy.py
+-rw-rw-rw-   0        0        0       97 2023-06-25 12:24:57.000000 signe-0.1.6/signe/types.py
+-rw-rw-rw-   0        0        0     3637 2023-07-08 17:46:06.000000 signe-0.1.6/signe/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-08 17:46:47.953043 signe-0.1.6/signe.egg-info/
+-rw-rw-rw-   0        0        0      469 2023-07-08 17:46:47.000000 signe-0.1.6/signe.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      403 2023-07-08 17:46:47.000000 signe-0.1.6/signe.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-08 17:46:47.000000 signe-0.1.6/signe.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-08 17:46:47.000000 signe-0.1.6/signe.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        6 2023-07-08 17:46:47.000000 signe-0.1.6/signe.egg-info/top_level.txt
```

### Comparing `signe-0.1.5/LICENSE` & `signe-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `signe-0.1.5/README.md` & `signe-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `signe-0.1.5/setup.py` & `signe-0.1.6/setup.py`

 * *Files identical despite different names*

### Comparing `signe-0.1.5/signe/core/collections.py` & `signe-0.1.6/signe/core/collections.py`

 * *Files identical despite different names*

### Comparing `signe-0.1.5/signe/core/effect.py` & `signe-0.1.6/signe/core/effect.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,23 +19,25 @@
     _g_id = 0
 
     def __init__(
         self,
         executor: Executor,
         fn: Callable[[], T],
         debug_trigger: Optional[Callable] = None,
+        priority_level=1,
     ) -> None:
         Effect._g_id += 1
         self.id = Effect._g_id
         self.__executor = executor
         self.value: Optional[T] = None
         self.fn = fn
         self._age = 0
         self._state = EffectState.CURRENT
         self.__dep_signals: Set[Signal] = set()
+        self.__priority_level = priority_level
 
         """
         When one effect is triggered by another effect, 
         the former belongs to a pre dependency 
         and the latter belongs to a next dependency.
 
         @effect
@@ -67,14 +69,18 @@
             + len(self.__next_dep_effects)
             + len(self.__dep_signals)
         ) <= 0
 
     def __get_all_dep_effects(self):
         return chain(self.__pre_dep_effects, self.__next_dep_effects)
 
+    @property
+    def priority_level(self):
+        return self.__priority_level
+
     def _get_pre_dep_effects(self):
         return list(self.__pre_dep_effects)
 
     def _get_next_dep_effects(self):
         return list(self.__next_dep_effects)
 
     def _add_sub_effect(self, effect: Effect):
```

### Comparing `signe-0.1.5/signe/core/runtime.py` & `signe-0.1.6/signe/core/runtime.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from __future__ import annotations
-from typing import TYPE_CHECKING, Set, List, Dict
-from abc import abstractmethod
+from typing import TYPE_CHECKING, Set, Dict
 from .collections import Stack
 
 from .effect import Effect
 
 if TYPE_CHECKING:
     from .signal import Signal
 
@@ -19,20 +18,28 @@
     @property
     def current_execution_scheduler(self):
         return (
             self.execution_scheduler_stack.get_current()
             or self.__defalut_executionScheduler
         )
 
+    @property
+    def is_running(self):
+        return (
+            self.current_execution_scheduler.is_running
+            or len(self.effect_running_stack) > 0
+        )
+
 
 class ExecutionScheduler:
     def __init__(self) -> None:
         self.__tick = 0
         self.__signal_updates: Dict[Signal, None] = {}
         self.__effect_updates: Dict[Effect, None] = {}
+        self.__running = False
 
     @property
     def tick(self):
         return self.__tick
 
     def add_signal(self, signal: Signal):
         self.__signal_updates[signal] = None
@@ -42,28 +49,34 @@
         self.__effect_updates[effect] = None
         return self
 
     def next_tick(self):
         self.__tick += 1
         return self
 
+    @property
+    def is_running(self):
+        return self.__running
+
     def run(self):
         self.__effect_updates.clear()
         self.next_tick()
         count = 0
+        self.__running = True
 
         while len(self.__signal_updates) > 0 or len(self.__effect_updates) > 0:
             self._run_signal_updates()
             self._run_effect_updates()
 
             count += 1
             if count >= 10000:
                 raise Exception("exceeded the maximum number of execution rounds.")
 
         self.__tick = 0
+        self.__running = False
 
     def cleanup_signal_updates(self):
         self.__signal_updates.clear()
 
     def cleanup_effect_updates(self):
         self.__effect_updates.clear()
 
@@ -71,15 +84,15 @@
         signals = list(self.__signal_updates.keys())
         for s in signals:
             s.update()
 
         self.cleanup_signal_updates()
 
     def _run_effect_updates(self):
-        effects = list(self.__effect_updates.keys())
+        effects = sorted(self.__effect_updates.keys(), key=lambda x: x.priority_level)
         for s in effects:
             s.update()
             s._reset_age()
 
         self.cleanup_effect_updates()
```

### Comparing `signe-0.1.5/signe/core/signal.py` & `signe-0.1.6/signe/core/signal.py`

 * *Files 4% similar despite different names*

```diff
@@ -69,15 +69,18 @@
             return self.value  # type: ignore
 
         if len(self.__dep_effects) <= 0:
             self.value = value
             return self.value
 
         self._pending = value
-        self.__executor.current_execution_scheduler.add_signal(self).run()
+        scheduler = self.__executor.current_execution_scheduler.add_signal(self)
+
+        if not self.__executor.is_running:
+            scheduler.run()
 
         return value  # type: ignore
 
     def update(self):
         self.value = self._pending
         self._pending = NOT_PENDING
         for sub in self.__dep_effects:
```

### Comparing `signe-0.1.5/signe/reactive/proxy.py` & `signe-0.1.6/signe/reactive/proxy.py`

 * *Files identical despite different names*

### Comparing `signe-0.1.5/signe/utils.py` & `signe-0.1.6/signe/utils.py`

 * *Files 17% similar despite different names*

```diff
@@ -27,39 +27,49 @@
 
 def createSignal(value: T, comp: TSignalOptionInitComp[T] = None):
     s = Signal(exec, value, SignalOption(comp))
 
     return s.getValue, s.setValue
 
 
-def effect(fn: Callable[[], T]):
+def effect(fn: Callable[..., None], *, priority_level=1):
     return Effect(exec, fn)
 
 
+def effect_with_opts(priority_level: int):
+    def wrap(fn: Callable[..., None]):
+        return effect(fn, priority_level=priority_level)
+
+    return wrap
+
+
 class computed(Generic[T]):
     def __init__(
-        self, fn: Callable[[], T], debug_trigger: Optional[Callable] = None
+        self,
+        fn: Callable[[], T],
+        debug_trigger: Optional[Callable] = None,
+        priority_level=1,
     ) -> None:
         self.fn = fn
 
         def getter():
-            effect = Effect(exec, fn, debug_trigger)
+            effect = Effect(exec, fn, debug_trigger, priority_level)
             self.getter = effect
             return effect.getValue()
 
         self.getter = getter
 
     @staticmethod
-    def debug_trigger(debug_trigger: Optional[Callable] = None):
-        def warp(
+    def with_opts(priority_level=1, debug_trigger: Optional[Callable] = None):
+        def wrap(
             fn: Callable[[], T],
         ):
-            return computed(fn, debug_trigger)
+            return computed(fn, debug_trigger, priority_level)
 
-        return warp
+        return wrap
 
     def __call__(self, *args: Any, **kwds: Any) -> T:
         return self.getter()  # type: ignore
 
 
 def batch(fn: Callable[[], None]):
     if isinstance(exec.current_execution_scheduler, BatchExecutionScheduler):
```

