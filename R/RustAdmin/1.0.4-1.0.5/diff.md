# Comparing `tmp/RustAdmin-1.0.4.tar.gz` & `tmp/RustAdmin-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RustAdmin-1.0.4.tar", last modified: Sat Jul  8 20:07:49 2023, max compression
+gzip compressed data, was "RustAdmin-1.0.5.tar", last modified: Sat Jul  8 20:13:58 2023, max compression
```

## Comparing `RustAdmin-1.0.4.tar` & `RustAdmin-1.0.5.tar`

### file list

```diff
@@ -1,10 +1,13 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-08 20:07:49.789938 RustAdmin-1.0.4/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      512 2023-07-08 20:07:49.789938 RustAdmin-1.0.4/PKG-INFO
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-08 20:07:49.789938 RustAdmin-1.0.4/RustAdmin.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      512 2023-07-08 20:07:49.000000 RustAdmin-1.0.4/RustAdmin.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      176 2023-07-08 20:07:49.000000 RustAdmin-1.0.4/RustAdmin.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-07-08 20:07:49.000000 RustAdmin-1.0.4/RustAdmin.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       48 2023-07-08 20:07:49.000000 RustAdmin-1.0.4/RustAdmin.egg-info/entry_points.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-07-08 20:07:49.000000 RustAdmin-1.0.4/RustAdmin.egg-info/top_level.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-07-08 20:07:49.789938 RustAdmin-1.0.4/setup.cfg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      695 2023-07-08 20:07:25.000000 RustAdmin-1.0.4/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-08 20:13:58.739782 RustAdmin-1.0.5/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      512 2023-07-08 20:13:58.739782 RustAdmin-1.0.5/PKG-INFO
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-08 20:13:58.739782 RustAdmin-1.0.5/RustAdmin.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      512 2023-07-08 20:13:58.000000 RustAdmin-1.0.5/RustAdmin.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      208 2023-07-08 20:13:58.000000 RustAdmin-1.0.5/RustAdmin.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-07-08 20:13:58.000000 RustAdmin-1.0.5/RustAdmin.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       48 2023-07-08 20:13:58.000000 RustAdmin-1.0.5/RustAdmin.egg-info/entry_points.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       16 2023-07-08 20:13:58.000000 RustAdmin-1.0.5/RustAdmin.egg-info/top_level.txt
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-08 20:13:58.739782 RustAdmin-1.0.5/admin/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-08 20:11:09.000000 RustAdmin-1.0.5/admin/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    14449 2023-07-08 19:55:04.000000 RustAdmin-1.0.5/admin/main.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-07-08 20:13:58.739782 RustAdmin-1.0.5/setup.cfg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      725 2023-07-08 20:13:47.000000 RustAdmin-1.0.5/setup.py
```

### Comparing `RustAdmin-1.0.4/PKG-INFO` & `RustAdmin-1.0.5/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RustAdmin
-Version: 1.0.4
+Version: 1.0.5
 Summary: UNKNOWN
 Home-page: https://github.com/yourusername/rustadmin
 Author: Pawan kumar
 Author-email: control@vvfin.in
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `RustAdmin-1.0.4/RustAdmin.egg-info/PKG-INFO` & `RustAdmin-1.0.5/RustAdmin.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RustAdmin
-Version: 1.0.4
+Version: 1.0.5
 Summary: UNKNOWN
 Home-page: https://github.com/yourusername/rustadmin
 Author: Pawan kumar
 Author-email: control@vvfin.in
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `RustAdmin-1.0.4/setup.py` & `RustAdmin-1.0.5/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 from setuptools import setup, find_packages
 
 setup(
     name='RustAdmin',
-    version='1.0.4',
+    version='1.0.5',
     author='Pawan kumar',
     author_email='control@vvfin.in',
     url='https://github.com/yourusername/rustadmin',
+    py_modules=['rustadmin'],
     packages=find_packages(),
     classifiers=[
         'Development Status :: 3 - Alpha',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
     ],
     install_requires=[
     ],
     entry_points={
         'console_scripts': [
-            'rust-admin = Admin.main:main',
+            'rust-admin = admin.main:main',
         ],
     },
 )
```

