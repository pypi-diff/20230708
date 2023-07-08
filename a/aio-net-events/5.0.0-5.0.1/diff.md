# Comparing `tmp/aio_net_events-5.0.0.tar.gz` & `tmp/aio_net_events-5.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aio_net_events-5.0.0.tar", max compression
+gzip compressed data, was "aio_net_events-5.0.1.tar", max compression
```

## Comparing `aio_net_events-5.0.0.tar` & `aio_net_events-5.0.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1070 2019-11-19 19:09:21.000000 aio_net_events-5.0.0/LICENSE
--rw-r--r--   0        0        0      905 2021-06-02 08:35:57.000000 aio_net_events-5.0.0/README.md
--rw-r--r--   0        0        0     1164 2023-07-08 11:56:57.504103 aio_net_events-5.0.0/pyproject.toml
--rw-r--r--   0        0        0      205 2020-01-22 20:19:10.000000 aio_net_events-5.0.0/src/aio_net_events/__init__.py
--rw-r--r--   0        0        0      241 2020-01-23 11:42:16.000000 aio_net_events-5.0.0/src/aio_net_events/__main__.py
--rw-r--r--   0        0        0       58 2020-01-16 08:06:34.000000 aio_net_events-5.0.0/src/aio_net_events/backends/__init__.py
--rw-r--r--   0        0        0      878 2020-09-30 14:08:09.000000 aio_net_events-5.0.0/src/aio_net_events/backends/autodetect.py
--rw-r--r--   0        0        0     2815 2021-10-08 19:57:24.000000 aio_net_events-5.0.0/src/aio_net_events/backends/base.py
--rw-r--r--   0        0        0     3520 2021-10-08 19:57:31.000000 aio_net_events-5.0.0/src/aio_net_events/backends/macos.py
--rw-r--r--   0        0        0     1663 2021-10-08 17:38:48.000000 aio_net_events-5.0.0/src/aio_net_events/backends/netlink.py
--rw-r--r--   0        0        0     1072 2023-07-08 11:52:34.629853 aio_net_events-5.0.0/src/aio_net_events/backends/portable.py
--rw-r--r--   0        0        0        0 2019-11-19 10:23:12.000000 aio_net_events-5.0.0/src/aio_net_events/py.typed
--rw-r--r--   0        0        0    12739 2021-10-08 20:30:05.000000 aio_net_events-5.0.0/src/aio_net_events/task.py
--rw-r--r--   0        0        0       95 2023-07-08 11:56:57.504479 aio_net_events-5.0.0/src/aio_net_events/version.py
--rw-r--r--   0        0        0     1981 1970-01-01 00:00:00.000000 aio_net_events-5.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2019-11-19 19:09:21.000000 aio_net_events-5.0.1/LICENSE
+-rw-r--r--   0        0        0      905 2021-06-02 08:35:57.000000 aio_net_events-5.0.1/README.md
+-rw-r--r--   0        0        0     1165 2023-07-08 12:12:58.961932 aio_net_events-5.0.1/pyproject.toml
+-rw-r--r--   0        0        0      205 2020-01-22 20:19:10.000000 aio_net_events-5.0.1/src/aio_net_events/__init__.py
+-rw-r--r--   0        0        0      241 2020-01-23 11:42:16.000000 aio_net_events-5.0.1/src/aio_net_events/__main__.py
+-rw-r--r--   0        0        0       58 2020-01-16 08:06:34.000000 aio_net_events-5.0.1/src/aio_net_events/backends/__init__.py
+-rw-r--r--   0        0        0      878 2020-09-30 14:08:09.000000 aio_net_events-5.0.1/src/aio_net_events/backends/autodetect.py
+-rw-r--r--   0        0        0     2815 2021-10-08 19:57:24.000000 aio_net_events-5.0.1/src/aio_net_events/backends/base.py
+-rw-r--r--   0        0        0     3520 2021-10-08 19:57:31.000000 aio_net_events-5.0.1/src/aio_net_events/backends/macos.py
+-rw-r--r--   0        0        0     1663 2021-10-08 17:38:48.000000 aio_net_events-5.0.1/src/aio_net_events/backends/netlink.py
+-rw-r--r--   0        0        0     1072 2023-07-08 11:52:34.629853 aio_net_events-5.0.1/src/aio_net_events/backends/portable.py
+-rw-r--r--   0        0        0        0 2019-11-19 10:23:12.000000 aio_net_events-5.0.1/src/aio_net_events/py.typed
+-rw-r--r--   0        0        0    12739 2021-10-08 20:30:05.000000 aio_net_events-5.0.1/src/aio_net_events/task.py
+-rw-r--r--   0        0        0       95 2023-07-08 12:12:58.962364 aio_net_events-5.0.1/src/aio_net_events/version.py
+-rw-r--r--   0        0        0     1973 1970-01-01 00:00:00.000000 aio_net_events-5.0.1/PKG-INFO
```

### Comparing `aio_net_events-5.0.0/LICENSE` & `aio_net_events-5.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aio_net_events-5.0.0/README.md` & `aio_net_events-5.0.1/README.md`

 * *Files identical despite different names*

### Comparing `aio_net_events-5.0.0/pyproject.toml` & `aio_net_events-5.0.1/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [tool.poetry]
 name = "aio-net-events"
-version = "5.0.0"
+version = "5.0.1"
 description = "Asynchronous network configuration event detector for Python 3.7 and above"
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/ntamas/aio-net-events/"
 repository = "https://github.com/ntamas/aio-net-events/"
 authors = ["Tamas Nepusz <tamas@collmot.com>"]
 packages = [
     { include = "aio_net_events", from = "src" }
 ]
 
 [tool.poetry.dependencies]
 python = "^3.7"
 anyio = "^3.7.1"
-netifaces-plus = "^0.12.0"
+netifaces-plus = ">=0.12.0"
 pyobjc-core = { version = "^9.2", platform = "darwin" }
 pyobjc-framework-Cocoa = { version = "^9.2", platform = "darwin" }
 pyobjc-framework-SystemConfiguration = { version = "^9.2", platform = "darwin" }
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.4.0"
 coverage = {extras = ["toml"], version = "^7.2.7"}
```

### Comparing `aio_net_events-5.0.0/src/aio_net_events/backends/autodetect.py` & `aio_net_events-5.0.1/src/aio_net_events/backends/autodetect.py`

 * *Files identical despite different names*

### Comparing `aio_net_events-5.0.0/src/aio_net_events/backends/base.py` & `aio_net_events-5.0.1/src/aio_net_events/backends/base.py`

 * *Files identical despite different names*

### Comparing `aio_net_events-5.0.0/src/aio_net_events/backends/macos.py` & `aio_net_events-5.0.1/src/aio_net_events/backends/macos.py`

 * *Files identical despite different names*

### Comparing `aio_net_events-5.0.0/src/aio_net_events/backends/netlink.py` & `aio_net_events-5.0.1/src/aio_net_events/backends/netlink.py`

 * *Files identical despite different names*

### Comparing `aio_net_events-5.0.0/src/aio_net_events/backends/portable.py` & `aio_net_events-5.0.1/src/aio_net_events/backends/portable.py`

 * *Files identical despite different names*

### Comparing `aio_net_events-5.0.0/src/aio_net_events/task.py` & `aio_net_events-5.0.1/src/aio_net_events/task.py`

 * *Files identical despite different names*

### Comparing `aio_net_events-5.0.0/PKG-INFO` & `aio_net_events-5.0.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: aio-net-events
-Version: 5.0.0
+Version: 5.0.1
 Summary: Asynchronous network configuration event detector for Python 3.7 and above
 Home-page: https://github.com/ntamas/aio-net-events/
 License: MIT
 Author: Tamas Nepusz
 Author-email: tamas@collmot.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: anyio (>=3.7.1,<4.0.0)
-Requires-Dist: netifaces-plus (>=0.12.0,<0.13.0)
+Requires-Dist: netifaces-plus (>=0.12.0)
 Requires-Dist: pyobjc-core (>=9.2,<10.0) ; sys_platform == "darwin"
 Requires-Dist: pyobjc-framework-Cocoa (>=9.2,<10.0) ; sys_platform == "darwin"
 Requires-Dist: pyobjc-framework-SystemConfiguration (>=9.2,<10.0) ; sys_platform == "darwin"
 Project-URL: Repository, https://github.com/ntamas/aio-net-events/
 Description-Content-Type: text/markdown
 
 # aio-net-events
```

