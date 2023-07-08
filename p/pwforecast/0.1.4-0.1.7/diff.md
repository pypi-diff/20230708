# Comparing `tmp/pwforecast-0.1.4.tar.gz` & `tmp/pwforecast-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pwforecast-0.1.4.tar", last modified: Sat Jul  8 07:35:55 2023, max compression
+gzip compressed data, was "pwforecast-0.1.7.tar", last modified: Sat Jul  8 09:32:45 2023, max compression
```

## Comparing `pwforecast-0.1.4.tar` & `pwforecast-0.1.7.tar`

### file list

```diff
@@ -1,11 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 07:35:55.591199 pwforecast-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-08 07:35:43.000000 pwforecast-0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2932 2023-07-08 07:35:55.591199 pwforecast-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2639 2023-07-08 07:35:43.000000 pwforecast-0.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 07:35:55.591199 pwforecast-0.1.4/pwforecast.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2932 2023-07-08 07:35:55.000000 pwforecast-0.1.4/pwforecast.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-08 07:35:55.000000 pwforecast-0.1.4/pwforecast.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 07:35:55.000000 pwforecast-0.1.4/pwforecast.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 07:35:55.000000 pwforecast-0.1.4/pwforecast.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 07:35:55.591199 pwforecast-0.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-07-08 07:35:43.000000 pwforecast-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 09:32:45.183333 pwforecast-0.1.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-08 09:32:33.000000 pwforecast-0.1.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2932 2023-07-08 09:32:45.183333 pwforecast-0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2639 2023-07-08 09:32:33.000000 pwforecast-0.1.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 09:32:45.183333 pwforecast-0.1.7/pwforecast/
+-rw-r--r--   0 runner    (1001) docker     (123)    15901 2023-07-08 09:32:33.000000 pwforecast-0.1.7/pwforecast/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 09:32:45.183333 pwforecast-0.1.7/pwforecast.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2932 2023-07-08 09:32:45.000000 pwforecast-0.1.7/pwforecast.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-07-08 09:32:45.000000 pwforecast-0.1.7/pwforecast.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 09:32:45.000000 pwforecast-0.1.7/pwforecast.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-08 09:32:45.000000 pwforecast-0.1.7/pwforecast.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 09:32:45.183333 pwforecast-0.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-07-08 09:32:33.000000 pwforecast-0.1.7/setup.py
```

### Comparing `pwforecast-0.1.4/LICENSE` & `pwforecast-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pwforecast-0.1.4/PKG-INFO` & `pwforecast-0.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pwforecast
-Version: 0.1.4
+Version: 0.1.7
 Summary: A Python module to charge/discharge Powerwall based on solar forecast and peak/off peak tariffs.
 Home-page: https://github.com/timhawker/pwforecast
 Author: Tim Hawker
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ## PwForecast
```

### Comparing `pwforecast-0.1.4/README.md` & `pwforecast-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `pwforecast-0.1.4/pwforecast.egg-info/PKG-INFO` & `pwforecast-0.1.7/pwforecast.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pwforecast
-Version: 0.1.4
+Version: 0.1.7
 Summary: A Python module to charge/discharge Powerwall based on solar forecast and peak/off peak tariffs.
 Home-page: https://github.com/timhawker/pwforecast
 Author: Tim Hawker
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ## PwForecast
```

### Comparing `pwforecast-0.1.4/setup.py` & `pwforecast-0.1.7/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 # read the contents of your README file
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setuptools.setup(
     name='pwforecast',
-    version='0.1.4',
+    version='0.1.7',
     author='Tim Hawker',
     description='A Python module to charge/discharge Powerwall based on solar forecast and peak/off peak tariffs.',
     url='https://github.com/timhawker/pwforecast',
     long_description_content_type='text/markdown',
-    long_description=long_description
+    long_description=long_description,
+    packages=['pwforecast']
 )
```

