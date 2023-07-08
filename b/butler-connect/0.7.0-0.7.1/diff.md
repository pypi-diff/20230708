# Comparing `tmp/butler-connect-0.7.0.tar.gz` & `tmp/butler-connect-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "butler-connect-0.7.0.tar", last modified: Fri Jul  7 08:25:31 2023, max compression
+gzip compressed data, was "butler-connect-0.7.1.tar", last modified: Sat Jul  8 09:44:14 2023, max compression
```

## Comparing `butler-connect-0.7.0.tar` & `butler-connect-0.7.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-07-07 08:25:31.945533 butler-connect-0.7.0/
--rw-rw-rw-   0        0        0     1091 2022-12-30 14:19:14.000000 butler-connect-0.7.0/LICENSE
--rw-rw-rw-   0        0        0     2520 2023-07-07 08:25:31.944543 butler-connect-0.7.0/PKG-INFO
--rw-rw-rw-   0        0        0      748 2023-07-07 08:25:07.000000 butler-connect-0.7.0/README.md
--rw-rw-rw-   0        0        0      738 2023-07-07 08:25:15.000000 butler-connect-0.7.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-07 08:25:31.945533 butler-connect-0.7.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-07 08:25:31.914020 butler-connect-0.7.0/src/
-drwxrwxrwx   0        0        0        0 2023-07-07 08:25:31.918021 butler-connect-0.7.0/src/butlerConnect/
--rw-rw-rw-   0        0        0      123 2023-05-18 09:03:28.000000 butler-connect-0.7.0/src/butlerConnect/__init__.py
--rw-rw-rw-   0        0        0    18719 2023-05-20 09:13:29.000000 butler-connect-0.7.0/src/butlerConnect/pikaButler.py
-drwxrwxrwx   0        0        0        0 2023-07-07 08:25:31.926020 butler-connect-0.7.0/src/butlerDescription/
--rw-rw-rw-   0        0        0      208 2023-05-18 09:13:48.000000 butler-connect-0.7.0/src/butlerDescription/__init__.py
--rw-rw-rw-   0        0        0      180 2023-04-11 15:45:51.000000 butler-connect-0.7.0/src/butlerDescription/component.py
--rw-rw-rw-   0        0        0     1525 2022-12-30 14:09:45.000000 butler-connect-0.7.0/src/butlerDescription/control.py
--rw-rw-rw-   0        0        0      209 2023-05-12 19:37:37.000000 butler-connect-0.7.0/src/butlerDescription/group.py
--rw-rw-rw-   0        0        0     2024 2023-07-07 08:23:39.000000 butler-connect-0.7.0/src/butlerDescription/signal.py
-drwxrwxrwx   0        0        0        0 2023-07-07 08:25:31.944543 butler-connect-0.7.0/src/butler_connect.egg-info/
--rw-rw-rw-   0        0        0     2520 2023-07-07 08:25:31.000000 butler-connect-0.7.0/src/butler_connect.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      468 2023-07-07 08:25:31.000000 butler-connect-0.7.0/src/butler_connect.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-07 08:25:31.000000 butler-connect-0.7.0/src/butler_connect.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       80 2023-07-07 08:25:31.000000 butler-connect-0.7.0/src/butler_connect.egg-info/requires.txt
--rw-rw-rw-   0        0        0       32 2023-07-07 08:25:31.000000 butler-connect-0.7.0/src/butler_connect.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-08 09:44:14.232107 butler-connect-0.7.1/
+-rw-rw-rw-   0        0        0     1091 2022-12-30 14:19:14.000000 butler-connect-0.7.1/LICENSE
+-rw-rw-rw-   0        0        0     2584 2023-07-08 09:44:14.231117 butler-connect-0.7.1/PKG-INFO
+-rw-rw-rw-   0        0        0      809 2023-07-08 09:42:59.000000 butler-connect-0.7.1/README.md
+-rw-rw-rw-   0        0        0      738 2023-07-08 09:42:21.000000 butler-connect-0.7.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-08 09:44:14.232107 butler-connect-0.7.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-08 09:44:14.200104 butler-connect-0.7.1/src/
+drwxrwxrwx   0        0        0        0 2023-07-08 09:44:14.203167 butler-connect-0.7.1/src/butlerConnect/
+-rw-rw-rw-   0        0        0      123 2023-05-18 09:03:28.000000 butler-connect-0.7.1/src/butlerConnect/__init__.py
+-rw-rw-rw-   0        0        0    18719 2023-05-20 09:13:29.000000 butler-connect-0.7.1/src/butlerConnect/pikaButler.py
+drwxrwxrwx   0        0        0        0 2023-07-08 09:44:14.213095 butler-connect-0.7.1/src/butlerDescription/
+-rw-rw-rw-   0        0        0      208 2023-05-18 09:13:48.000000 butler-connect-0.7.1/src/butlerDescription/__init__.py
+-rw-rw-rw-   0        0        0      180 2023-04-11 15:45:51.000000 butler-connect-0.7.1/src/butlerDescription/component.py
+-rw-rw-rw-   0        0        0     1525 2022-12-30 14:09:45.000000 butler-connect-0.7.1/src/butlerDescription/control.py
+-rw-rw-rw-   0        0        0      209 2023-05-12 19:37:37.000000 butler-connect-0.7.1/src/butlerDescription/group.py
+-rw-rw-rw-   0        0        0     2034 2023-07-08 09:43:40.000000 butler-connect-0.7.1/src/butlerDescription/signal.py
+drwxrwxrwx   0        0        0        0 2023-07-08 09:44:14.231117 butler-connect-0.7.1/src/butler_connect.egg-info/
+-rw-rw-rw-   0        0        0     2584 2023-07-08 09:44:14.000000 butler-connect-0.7.1/src/butler_connect.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      468 2023-07-08 09:44:14.000000 butler-connect-0.7.1/src/butler_connect.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-08 09:44:14.000000 butler-connect-0.7.1/src/butler_connect.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       80 2023-07-08 09:44:14.000000 butler-connect-0.7.1/src/butler_connect.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       32 2023-07-08 09:44:14.000000 butler-connect-0.7.1/src/butler_connect.egg-info/top_level.txt
```

### Comparing `butler-connect-0.7.0/LICENSE` & `butler-connect-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `butler-connect-0.7.0/PKG-INFO` & `butler-connect-0.7.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: butler-connect
-Version: 0.7.0
+Version: 0.7.1
 Summary: Access libraries (with pika) and data definitions for the Buttler project.
 Author-email: Oliver Birkholz <info@aibutler.de>
 License: MIT License
         
         Copyright (c) 2023 Oliver Birkholz
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -54,7 +54,10 @@
 - Solving Problems with createConsumer with same topic an different routing_keys
 
 ### 0.6.0
 - add new signal  types f.ex. system_state or set_temperature.heater
 
 ### 0.7.0
 - change signal Description and add ext. !!! No backwards compatibility! if Using Schmema for parsing
+
+### 0.7.1
+- Bugifx in Signal().__init__(.. ext was missing)
```

### Comparing `butler-connect-0.7.0/README.md` & `butler-connect-0.7.1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -18,8 +18,11 @@
 ### 0.5.5
 - Solving Problems with createConsumer with same topic an different routing_keys
 
 ### 0.6.0
 - add new signal  types f.ex. system_state or set_temperature.heater
 
 ### 0.7.0
-- change signal Description and add ext. !!! No backwards compatibility! if Using Schmema for parsing
+- change signal Description and add ext. !!! No backwards compatibility! if Using Schmema for parsing
+
+### 0.7.1
+- Bugifx in Signal().__init__(.. ext was missing)
```

### Comparing `butler-connect-0.7.0/pyproject.toml` & `butler-connect-0.7.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "butler-connect"
-version = "0.7.0"
+version = "0.7.1"
 description = "Access libraries (with pika) and data definitions for the Buttler project."
 readme = "README.md"
 authors = [{ name = "Oliver Birkholz", email = "info@aibutler.de" }]
 license = { file = "LICENSE" }
 requires-python = ">=3.7"
 classifiers = [
     "License :: OSI Approved :: MIT License",
```

### Comparing `butler-connect-0.7.0/src/butlerConnect/pikaButler.py` & `butler-connect-0.7.1/src/butlerConnect/pikaButler.py`

 * *Files identical despite different names*

### Comparing `butler-connect-0.7.0/src/butlerDescription/control.py` & `butler-connect-0.7.1/src/butlerDescription/control.py`

 * *Files identical despite different names*

### Comparing `butler-connect-0.7.0/src/butlerDescription/signal.py` & `butler-connect-0.7.1/src/butlerDescription/signal.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,24 +25,24 @@
 class SignalOptionType():
     unDef = 'undef'
     forwardingMQTT = 'forwarding_mqtt'
     
 
 
 class Signal():
-    def __init__(self,type,component=0,group=0,ioDevice="",ioSignal="",parameter={},timestamp=datetime.now(),value = 0.0,valueStr = ""):
+    def __init__(self,type,component=0,group=0,ioDevice="",ioSignal="",parameter={},timestamp=datetime.now(),value = 0.0,valueStr = "",ext={}):
         self.timestamp  = timestamp
         self.component  = int(component)
         self.group      = int(group)
         self.ioDevice   = ioDevice
         self.ioSignal   = ioSignal
         self.type       = type
         self.value      = float(value)
         self.valueStr   = str(valueStr)
-        self.ext        = dict()
+        self.ext        = dict(ext)
         
     def __repr__(self):
         return "<User(name={self.name!r})>".format(self=self)
     def __str__(self) -> str:
         return f'component={self.component}, group={self.group}, ioDevice={self.ioDevice}, ioSignal={self.ioSignal}, type={self.type}, value={self.value}, valueStr={self.valueStr}, timestmap={self.timestamp}, ext={self.ext}'        
 
 class SignalSchmea(Schema):
```

### Comparing `butler-connect-0.7.0/src/butler_connect.egg-info/PKG-INFO` & `butler-connect-0.7.1/src/butler_connect.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: butler-connect
-Version: 0.7.0
+Version: 0.7.1
 Summary: Access libraries (with pika) and data definitions for the Buttler project.
 Author-email: Oliver Birkholz <info@aibutler.de>
 License: MIT License
         
         Copyright (c) 2023 Oliver Birkholz
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -54,7 +54,10 @@
 - Solving Problems with createConsumer with same topic an different routing_keys
 
 ### 0.6.0
 - add new signal  types f.ex. system_state or set_temperature.heater
 
 ### 0.7.0
 - change signal Description and add ext. !!! No backwards compatibility! if Using Schmema for parsing
+
+### 0.7.1
+- Bugifx in Signal().__init__(.. ext was missing)
```

