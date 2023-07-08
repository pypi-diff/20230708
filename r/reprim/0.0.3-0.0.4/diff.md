# Comparing `tmp/reprim-0.0.3.tar.gz` & `tmp/reprim-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reprim-0.0.3.tar", last modified: Sat Jul  8 16:46:20 2023, max compression
+gzip compressed data, was "reprim-0.0.4.tar", last modified: Sat Jul  8 17:18:31 2023, max compression
```

## Comparing `reprim-0.0.3.tar` & `reprim-0.0.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-07-08 16:46:20.785658 reprim-0.0.3/
--rw-rw-rw-   0        0        0      683 2023-07-08 16:46:20.784660 reprim-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0      303 2023-07-06 00:02:04.000000 reprim-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-07-08 16:46:20.752039 reprim-0.0.3/RePrIm/
--rw-rw-rw-   0        0        0       22 2023-07-06 00:02:04.000000 reprim-0.0.3/RePrIm/__init__.py
--rw-rw-rw-   0        0        0    20167 2023-07-08 16:13:08.000000 reprim-0.0.3/RePrIm/reprim.py
-drwxrwxrwx   0        0        0        0 2023-07-08 16:46:20.773422 reprim-0.0.3/RePrIm/util/
--rw-rw-rw-   0        0        0     1900 2023-07-08 16:45:38.000000 reprim-0.0.3/RePrIm/util/hardware_monitor.py
--rw-rw-rw-   0        0        0   311808 2023-07-06 00:02:04.000000 reprim-0.0.3/RePrIm/util/lib.py
--rw-rw-rw-   0        0        0     2258 2023-07-06 00:02:04.000000 reprim-0.0.3/RePrIm/util/process.py
--rw-rw-rw-   0        0        0     2098 2023-07-08 15:06:48.000000 reprim-0.0.3/RePrIm/util/tools.py
-drwxrwxrwx   0        0        0        0 2023-07-08 16:46:20.784660 reprim-0.0.3/reprim.egg-info/
--rw-rw-rw-   0        0        0      683 2023-07-08 16:46:20.000000 reprim-0.0.3/reprim.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      374 2023-07-08 16:46:20.000000 reprim-0.0.3/reprim.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-08 16:46:20.000000 reprim-0.0.3/reprim.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       27 2023-07-08 16:46:20.000000 reprim-0.0.3/reprim.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-07-08 16:46:20.000000 reprim-0.0.3/reprim.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-08 16:46:20.785658 reprim-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      709 2023-07-08 16:44:08.000000 reprim-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-08 17:18:31.064654 reprim-0.0.4/
+-rw-rw-rw-   0        0        0      683 2023-07-08 17:18:31.063656 reprim-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0      303 2023-07-06 00:02:04.000000 reprim-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-07-08 17:18:31.048698 reprim-0.0.4/RePrIm/
+-rw-rw-rw-   0        0        0       22 2023-07-06 00:02:04.000000 reprim-0.0.4/RePrIm/__init__.py
+-rw-rw-rw-   0        0        0    20167 2023-07-08 17:16:21.000000 reprim-0.0.4/RePrIm/reprim.py
+drwxrwxrwx   0        0        0        0 2023-07-08 17:18:31.052687 reprim-0.0.4/RePrIm/util/
+-rw-rw-rw-   0        0        0     1936 2023-07-08 17:16:36.000000 reprim-0.0.4/RePrIm/util/hardware_monitor.py
+-rw-rw-rw-   0        0        0   311808 2023-07-06 00:02:04.000000 reprim-0.0.4/RePrIm/util/lib.py
+-rw-rw-rw-   0        0        0     2258 2023-07-06 00:02:04.000000 reprim-0.0.4/RePrIm/util/process.py
+-rw-rw-rw-   0        0        0     2099 2023-07-08 17:16:36.000000 reprim-0.0.4/RePrIm/util/tools.py
+drwxrwxrwx   0        0        0        0 2023-07-08 17:18:31.063656 reprim-0.0.4/reprim.egg-info/
+-rw-rw-rw-   0        0        0      683 2023-07-08 17:18:30.000000 reprim-0.0.4/reprim.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      393 2023-07-08 17:18:31.000000 reprim-0.0.4/reprim.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-08 17:18:30.000000 reprim-0.0.4/reprim.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       27 2023-07-08 17:18:30.000000 reprim-0.0.4/reprim.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-07-08 17:18:30.000000 reprim-0.0.4/reprim.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-08 17:18:31.064654 reprim-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      709 2023-07-08 17:18:18.000000 reprim-0.0.4/setup.py
```

### Comparing `reprim-0.0.3/PKG-INFO` & `reprim-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reprim
-Version: 0.0.3
+Version: 0.0.4
 Summary: for questions write me in Telegram (@IDieLast)
 Home-page: https://github.com/GGergy/RePrIm/
 Author: GGergy
 Author-email: gergy2k07@gmail.com
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Description-Content-Type: text/markdown
```

### Comparing `reprim-0.0.3/RePrIm/reprim.py` & `reprim-0.0.4/RePrIm/reprim.py`

 * *Files identical despite different names*

### Comparing `reprim-0.0.3/RePrIm/util/hardware_monitor.py` & `reprim-0.0.4/RePrIm/util/hardware_monitor.py`

 * *Files 8% similar despite different names*

```diff
@@ -51,11 +51,13 @@
                 ans = parse_sensor(subsensor)
                 if ans:
                     answer.append(ans)
     return answer
 
 
 def parse_sensor(sensor):
+    if not sensor:
+        return
     if str(sensor.SensorType) not in degrees.keys():
         return
     ref = "HDD " if str(sensor.Name) == 'Used Space' else ""
     return f"{ref}{sensor.Name} {sensor.SensorType} - {round(sensor.Value, 2)} {degrees[str(sensor.SensorType)]}"
```

### Comparing `reprim-0.0.3/RePrIm/util/lib.py` & `reprim-0.0.4/RePrIm/util/lib.py`

 * *Files identical despite different names*

### Comparing `reprim-0.0.3/RePrIm/util/process.py` & `reprim-0.0.4/RePrIm/util/process.py`

 * *Files identical despite different names*

### Comparing `reprim-0.0.3/RePrIm/util/tools.py` & `reprim-0.0.4/RePrIm/util/tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 from functools import lru_cache
 from .hardware_monitor import fetch_stats
 
 
 def init():
     if not os.path.isfile('reprim.rpc'):
-        with open('pyrpc.cfg', mode='w') as wf:
+        with open('reprim.rpc', mode='w') as wf:
             wf.write('{"lexemas": {}}')
         return {"lexemas": {}}
     with open('reprim.rpc') as rf:
         dat = json.load(rf)
         return dat
```

### Comparing `reprim-0.0.3/reprim.egg-info/PKG-INFO` & `reprim-0.0.4/reprim.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reprim
-Version: 0.0.3
+Version: 0.0.4
 Summary: for questions write me in Telegram (@IDieLast)
 Home-page: https://github.com/GGergy/RePrIm/
 Author: GGergy
 Author-email: gergy2k07@gmail.com
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Description-Content-Type: text/markdown
```

### Comparing `reprim-0.0.3/setup.py` & `reprim-0.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     readme = readme_file.read()
 
 requirements = ["pytelegrambotapi", "pythonnet"]
 
 
 setup(
     name="reprim",
-    version="0.0.3",
+    version="0.0.4",
     author="GGergy",
     author_email="gergy2k07@gmail.com",
     description="for questions write me in Telegram (@IDieLast)",
     long_description=readme,
     long_description_content_type="text/markdown",
     url="https://github.com/GGergy/RePrIm/",
     packages=['RePrIm', 'RePrIm/util'],
```

