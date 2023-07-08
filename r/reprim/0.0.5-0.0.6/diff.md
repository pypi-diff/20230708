# Comparing `tmp/reprim-0.0.5.tar.gz` & `tmp/reprim-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reprim-0.0.5.tar", last modified: Sat Jul  8 17:26:13 2023, max compression
+gzip compressed data, was "reprim-0.0.6.tar", last modified: Sat Jul  8 17:33:44 2023, max compression
```

## Comparing `reprim-0.0.5.tar` & `reprim-0.0.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-07-08 17:26:13.336638 reprim-0.0.5/
--rw-rw-rw-   0        0        0      683 2023-07-08 17:26:13.336638 reprim-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0      303 2023-07-06 00:02:04.000000 reprim-0.0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-07-08 17:26:13.298810 reprim-0.0.5/RePrIm/
--rw-rw-rw-   0        0        0       22 2023-07-06 00:02:04.000000 reprim-0.0.5/RePrIm/__init__.py
--rw-rw-rw-   0        0        0    20167 2023-07-08 17:16:21.000000 reprim-0.0.5/RePrIm/reprim.py
-drwxrwxrwx   0        0        0        0 2023-07-08 17:26:13.323534 reprim-0.0.5/RePrIm/util/
--rw-rw-rw-   0        0        0     1960 2023-07-08 17:25:54.000000 reprim-0.0.5/RePrIm/util/hardware_monitor.py
--rw-rw-rw-   0        0        0   311808 2023-07-06 00:02:04.000000 reprim-0.0.5/RePrIm/util/lib.py
--rw-rw-rw-   0        0        0     2258 2023-07-06 00:02:04.000000 reprim-0.0.5/RePrIm/util/process.py
--rw-rw-rw-   0        0        0     2099 2023-07-08 17:16:36.000000 reprim-0.0.5/RePrIm/util/tools.py
-drwxrwxrwx   0        0        0        0 2023-07-08 17:26:13.335639 reprim-0.0.5/reprim.egg-info/
--rw-rw-rw-   0        0        0      683 2023-07-08 17:26:13.000000 reprim-0.0.5/reprim.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      393 2023-07-08 17:26:13.000000 reprim-0.0.5/reprim.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-08 17:26:13.000000 reprim-0.0.5/reprim.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       27 2023-07-08 17:26:13.000000 reprim-0.0.5/reprim.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-07-08 17:26:13.000000 reprim-0.0.5/reprim.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-08 17:26:13.337635 reprim-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0      709 2023-07-08 17:25:54.000000 reprim-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-08 17:33:44.596362 reprim-0.0.6/
+-rw-rw-rw-   0        0        0      683 2023-07-08 17:33:44.596362 reprim-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0      303 2023-07-06 00:02:04.000000 reprim-0.0.6/README.md
+drwxrwxrwx   0        0        0        0 2023-07-08 17:33:44.578771 reprim-0.0.6/RePrIm/
+-rw-rw-rw-   0        0        0       22 2023-07-06 00:02:04.000000 reprim-0.0.6/RePrIm/__init__.py
+-rw-rw-rw-   0        0        0    20167 2023-07-08 17:16:21.000000 reprim-0.0.6/RePrIm/reprim.py
+drwxrwxrwx   0        0        0        0 2023-07-08 17:33:44.582399 reprim-0.0.6/RePrIm/util/
+-rw-rw-rw-   0        0        0     1960 2023-07-08 17:25:54.000000 reprim-0.0.6/RePrIm/util/hardware_monitor.py
+-rw-rw-rw-   0        0        0   311808 2023-07-06 00:02:04.000000 reprim-0.0.6/RePrIm/util/lib.py
+-rw-rw-rw-   0        0        0     2258 2023-07-06 00:02:04.000000 reprim-0.0.6/RePrIm/util/process.py
+-rw-rw-rw-   0        0        0     2268 2023-07-08 17:33:17.000000 reprim-0.0.6/RePrIm/util/tools.py
+drwxrwxrwx   0        0        0        0 2023-07-08 17:33:44.595366 reprim-0.0.6/reprim.egg-info/
+-rw-rw-rw-   0        0        0      683 2023-07-08 17:33:44.000000 reprim-0.0.6/reprim.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      393 2023-07-08 17:33:44.000000 reprim-0.0.6/reprim.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-08 17:33:44.000000 reprim-0.0.6/reprim.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       27 2023-07-08 17:33:44.000000 reprim-0.0.6/reprim.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-07-08 17:33:44.000000 reprim-0.0.6/reprim.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-08 17:33:44.596362 reprim-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      709 2023-07-08 17:33:17.000000 reprim-0.0.6/setup.py
```

### Comparing `reprim-0.0.5/PKG-INFO` & `reprim-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reprim
-Version: 0.0.5
+Version: 0.0.6
 Summary: for questions write me in Telegram (@IDieLast)
 Home-page: https://github.com/GGergy/RePrIm/
 Author: GGergy
 Author-email: gergy2k07@gmail.com
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Description-Content-Type: text/markdown
```

### Comparing `reprim-0.0.5/RePrIm/reprim.py` & `reprim-0.0.6/RePrIm/reprim.py`

 * *Files identical despite different names*

### Comparing `reprim-0.0.5/RePrIm/util/hardware_monitor.py` & `reprim-0.0.6/RePrIm/util/hardware_monitor.py`

 * *Files identical despite different names*

### Comparing `reprim-0.0.5/RePrIm/util/lib.py` & `reprim-0.0.6/RePrIm/util/lib.py`

 * *Files identical despite different names*

### Comparing `reprim-0.0.5/RePrIm/util/process.py` & `reprim-0.0.6/RePrIm/util/process.py`

 * *Files identical despite different names*

### Comparing `reprim-0.0.5/RePrIm/util/tools.py` & `reprim-0.0.6/RePrIm/util/tools.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,17 @@
 import json
 import telebot
 import os
 from functools import lru_cache
-from .hardware_monitor import fetch_stats
+
+try:
+    from .hardware_monitor import fetch_stats
+    hm_supported = True
+except:
+    hm_supported = False
 
 
 def init():
     if not os.path.isfile('reprim.rpc'):
         with open('reprim.rpc', mode='w') as wf:
             wf.write('{"lexemas": {}}')
         return {"lexemas": {}}
@@ -75,8 +80,11 @@
 
 @lru_cache
 def unlex(arg):
     return '/'.join([data['lexemas'][item] if item != '.' else item for item in arg.split('/')])
 
 
 def get_sensors():
-    return "\n".join(fetch_stats())
+    if hm_supported:
+        return "\n".join(fetch_stats())
+    else:
+        return "your pc is not supported hardware monitor"
```

### Comparing `reprim-0.0.5/reprim.egg-info/PKG-INFO` & `reprim-0.0.6/reprim.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reprim
-Version: 0.0.5
+Version: 0.0.6
 Summary: for questions write me in Telegram (@IDieLast)
 Home-page: https://github.com/GGergy/RePrIm/
 Author: GGergy
 Author-email: gergy2k07@gmail.com
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Description-Content-Type: text/markdown
```

### Comparing `reprim-0.0.5/setup.py` & `reprim-0.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     readme = readme_file.read()
 
 requirements = ["pytelegrambotapi", "pythonnet"]
 
 
 setup(
     name="reprim",
-    version="0.0.5",
+    version="0.0.6",
     author="GGergy",
     author_email="gergy2k07@gmail.com",
     description="for questions write me in Telegram (@IDieLast)",
     long_description=readme,
     long_description_content_type="text/markdown",
     url="https://github.com/GGergy/RePrIm/",
     packages=['RePrIm', 'RePrIm/util'],
```

