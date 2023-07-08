# Comparing `tmp/hat_stc-0.6.3-cp38.cp39.cp310-none-any.whl.zip` & `tmp/hat_stc-0.6.4-cp310.cp311-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 10464 bytes, number of entries: 7
--rw-r--r--  2.0 unx    15943 b- defN 21-Nov-23 15:41 hat/stc.py
--rw-r--r--  2.0 unx    11358 b- defN 23-Feb-23 20:45 hat_stc-0.6.3.dist-info/LICENSE
--rw-r--r--  2.0 unx     1837 b- defN 23-Feb-23 20:45 hat_stc-0.6.3.dist-info/METADATA
--rw-r--r--  2.0 unx      132 b- defN 23-Feb-23 20:45 hat_stc-0.6.3.dist-info/WHEEL
--rw-r--r--  2.0 unx        4 b- defN 23-Feb-23 20:45 hat_stc-0.6.3.dist-info/top_level.txt
--rw-r--r--  2.0 unx        1 b- defN 23-Feb-23 20:45 hat_stc-0.6.3.dist-info/zip-safe
-?rw-rw-r--  2.0 unx      541 b- defN 23-Feb-23 20:45 hat_stc-0.6.3.dist-info/RECORD
-7 files, 29816 bytes uncompressed, 9508 bytes compressed:  68.1%
+Zip file size: 10558 bytes, number of entries: 7
+-rw-r--r--  2.0 unx    15720 b- defN 23-Jul-08 10:22 hat/stc.py
+-rw-r--r--  2.0 unx    11358 b- defN 23-Jul-08 10:23 hat_stc-0.6.4.dist-info/LICENSE
+-rw-r--r--  2.0 unx     2223 b- defN 23-Jul-08 10:23 hat_stc-0.6.4.dist-info/METADATA
+-rw-r--r--  2.0 unx      114 b- defN 23-Jul-08 10:23 hat_stc-0.6.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx        4 b- defN 23-Jul-08 10:23 hat_stc-0.6.4.dist-info/top_level.txt
+-rw-r--r--  2.0 unx        1 b- defN 23-Jul-08 10:23 hat_stc-0.6.4.dist-info/zip-safe
+-rw-rw-r--  2.0 unx      541 b- defN 23-Jul-08 10:23 hat_stc-0.6.4.dist-info/RECORD
+7 files, 29961 bytes uncompressed, 9602 bytes compressed:  68.0%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: hat/stc.py
 Comment: 
 
-Filename: hat_stc-0.6.3.dist-info/LICENSE
+Filename: hat_stc-0.6.4.dist-info/LICENSE
 Comment: 
 
-Filename: hat_stc-0.6.3.dist-info/METADATA
+Filename: hat_stc-0.6.4.dist-info/METADATA
 Comment: 
 
-Filename: hat_stc-0.6.3.dist-info/WHEEL
+Filename: hat_stc-0.6.4.dist-info/WHEEL
 Comment: 
 
-Filename: hat_stc-0.6.3.dist-info/top_level.txt
+Filename: hat_stc-0.6.4.dist-info/top_level.txt
 Comment: 
 
-Filename: hat_stc-0.6.3.dist-info/zip-safe
+Filename: hat_stc-0.6.4.dist-info/zip-safe
 Comment: 
 
-Filename: hat_stc-0.6.3.dist-info/RECORD
+Filename: hat_stc-0.6.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## hat/stc.py

```diff
@@ -3,32 +3,27 @@
 import collections
 import itertools
 import pathlib
 import typing
 import xml.etree.ElementTree
 
 from hat import aio
-from hat import util
 
 
-EventName = str
+EventName: typing.TypeAlias = str
 """Event name"""
-util.register_type_alias('EventName')
 
-StateName = str
+StateName: typing.TypeAlias = str
 """State name"""
-util.register_type_alias('StateName')
 
-ActionName = str
+ActionName: typing.TypeAlias = str
 """Action name"""
-util.register_type_alias('ActionName')
 
-ConditionName = str
+ConditionName: typing.TypeAlias = str
 """Condition name"""
-util.register_type_alias('ConditionName')
 
 
 class Event(typing.NamedTuple):
     """Event instance"""
     name: EventName
     """Event name"""
     payload: typing.Any = None
@@ -36,21 +31,21 @@
 
 
 class Transition(typing.NamedTuple):
     """Transition definition"""
     event: EventName
     """Event identifier. Occurrence of event with this exact identifier can
     trigger state transition."""
-    target: typing.Optional[StateName]
+    target: StateName | None
     """Destination state identifier. If destination state is not defined,
     local transition is assumed - state is not changed and transition
     actions are triggered."""
-    actions: typing.List[ActionName] = []
+    actions: list[ActionName] = []
     """Actions executed on transition."""
-    conditions: typing.List[ConditionName] = []
+    conditions: list[ConditionName] = []
     """List of conditions. Transition is triggered only if all provided
     conditions are met."""
     internal: bool = False
     """Internal transition modifier. Determines whether the source state is
     exited in transitions whose target state is a descendant of the source
     state."""
 
@@ -58,44 +53,43 @@
 class State(typing.NamedTuple):
     """State definition"""
     name: StateName
     """Unique state identifier."""
     children: typing.List['State'] = []
     """Optional child states. If state has children, first child is
     considered as its initial state."""
-    transitions: typing.List[Transition] = []
+    transitions: list[Transition] = []
     """Possible transitions to other states."""
-    entries: typing.List[ActionName] = []
+    entries: list[ActionName] = []
     """Actions executed when state is entered."""
-    exits: typing.List[ActionName] = []
+    exits: list[ActionName] = []
     """Actions executed when state is exited."""
     final: bool = False
     """Is state final."""
 
 
-Action = typing.Callable[['Statechart', typing.Optional[Event]], None]
+Action: typing.TypeAlias = typing.Callable[['Statechart', Event | None], None]
 """Action function
 
 Action implementation which can be executed as part of entering/exiting
 state or transition execution. It is called with statechart instance and
 `Event` which triggered transition. In case of initial actions, run during
 transition to initial state, it is called with ``None``.
 
 """
-util.register_type_alias('Action')
 
-Condition = typing.Callable[['Statechart', typing.Optional[Event]], bool]
+Condition: typing.TypeAlias = typing.Callable[['Statechart', Event | None],
+                                              bool]
 """Condition function
 
 Condition implementation used as transition guard. It is called with statechart
 instance and `Event` which triggered transition. Return value ``True`` is
 interpreted as satisfied condition.
 
 """
-util.register_type_alias('Condition')
 
 
 class Statechart:
     """Statechart engine
 
     Each instance is initialized with state definitions (first state is
     considered initial) and action and condition definitions.
@@ -123,16 +117,16 @@
         actions: mapping of action names to their implementation
         conditions: mapping of conditions names to their implementation
 
     """
 
     def __init__(self,
                  states: typing.Iterable[State],
-                 actions: typing.Dict[str, Action],
-                 conditions: typing.Dict[str, Condition] = {}):
+                 actions: dict[str, Action],
+                 conditions: dict[str, Condition] = {}):
         states = collections.deque(states)
         initial = states[0].name if states else None
 
         self._actions = actions
         self._conditions = conditions
         self._states = {}
         self._parents = {}
@@ -145,15 +139,15 @@
             self._states[state.name] = state
             self._parents.update({i.name: state.name for i in state.children})
 
         if initial:
             self._walk_down(initial, None)
 
     @property
-    def state(self) -> typing.Optional[StateName]:
+    def state(self) -> StateName | None:
         """Current state"""
         return self._stack[-1] if self._stack else None
 
     @property
     def finished(self) -> bool:
         """Is statechart in final state"""
         state = self.state
@@ -248,16 +242,15 @@
 
     def _exec_actions(self, names, event):
         for name in names:
             action = self._actions[name]
             action(self, event)
 
 
-def parse_scxml(scxml: typing.Union[typing.TextIO, pathlib.Path]
-                ) -> typing.List[State]:
+def parse_scxml(scxml: typing.TextIO | pathlib.Path) -> list[State]:
     """Parse SCXML into list of state definitions"""
     if isinstance(scxml, pathlib.Path):
         with open(scxml, encoding='utf-8') as f:
             root_el = _read_xml(f)
     else:
         root_el = _read_xml(scxml)
     return _parse_scxml_states(root_el)
```

## Comparing `hat_stc-0.6.3.dist-info/LICENSE` & `hat_stc-0.6.4.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `hat_stc-0.6.3.dist-info/METADATA` & `hat_stc-0.6.4.dist-info/METADATA`

 * *Files 18% similar despite different names*

```diff
@@ -1,56 +1,86 @@
 Metadata-Version: 2.1
 Name: hat-stc
-Version: 0.6.3
+Version: 0.6.4
 Summary: Hat statechart engine
 Home-page: https://github.com/hat-open/hat-stc
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
-Requires-Python: >=3.8
+Requires-Python: >=3.10
 Description-Content-Type: text/x-rst
 License-File: LICENSE
-Requires-Dist: hat-aio (~=0.7.4)
-Requires-Dist: hat-util (~=0.6.7)
+Requires-Dist: hat-aio (~=0.7.8)
 
-hat-stc - Statechart library
-============================
+.. _online documentation: https://hat-stc.hat-open.com
+.. _git repository: https://github.com/hat-open/hat-stc.git
+.. _PyPI project: https://pypi.org/project/hat-stc
+.. _pydoit: https://pydoit.org
+.. _Hat Open: https://hat-open.com
+.. _Končar Digital: https://www.koncar.hr/en
 
-This library is part of Hat Open project - open-source framework of tools and
-libraries for developing applications used for remote monitoring, control and
-management of intelligent electronic devices such as IoT devices, PLCs,
-industrial automation or home automation systems.
 
-Development of Hat Open and associated repositories is sponsored by
-`Končar Digital <https://www.koncar.hr>`_.
+hat-stc - Statechart library
+============================
 
 For more information see:
 
-    * hat-stc documentation - `<https://hat-stc.hat-open.com>`_
-    * hat-stc git repository - `<https://github.com/hat-open/hat-stc.git>`_
-    * Hat Open homepage - `<https://hat-open.com>`_
+* `online documentation`_
+* `git repository`_
 
-.. warning::
 
-    This project is currently in state of active development. Features,
-    functionality and API are unstable.
+Runtime requirements
+--------------------
+
+* python >=3.10
 
 
 Install
 -------
 
-::
+`hat-stc` is available as `PyPI project`_::
 
     $ pip install hat-stc
 
 
+Build
+-----
+
+Build tool used for `hat-stc` is `pydoit`_. It can be installed together
+with other python dependencies by running::
+
+    $ pip install -r requirements.pip.dev.txt
+
+For listing available doit tasks, use::
+
+    $ doit list
+
+Default task::
+
+    $ doit
+
+creates wheel package inside `build` directory.
+
+
+Hat Open
+--------
+
+`hat-stc` is part of `Hat Open`_ project - open-source framework of tools
+and libraries for developing applications used for remote monitoring, control
+and management of intelligent electronic devices such as IoT devices, PLCs,
+industrial automation or home automation systems.
+
+Development of Hat Open and associated repositories is sponsored by
+`Končar Digital`_.
+
+
 License
 -------
 
-Copyright 2020-2022 Hat Open AUTHORS
+Copyright 2020-2023 Hat Open AUTHORS
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

