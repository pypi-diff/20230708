# Comparing `tmp/samus-logging-0.1.86.tar.gz` & `tmp/samus-logging-0.1.88.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "samus-logging-0.1.86.tar", last modified: Sat Jul  8 10:03:03 2023, max compression
+gzip compressed data, was "samus-logging-0.1.88.tar", last modified: Sat Jul  8 10:13:34 2023, max compression
```

## Comparing `samus-logging-0.1.86.tar` & `samus-logging-0.1.88.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 samu      (1000) samu      (1000)        0 2023-07-08 10:03:03.184050 samus-logging-0.1.86/
--rw-rw-r--   0 samu      (1000) samu      (1000)        0 2023-06-28 14:33:05.000000 samus-logging-0.1.86/LICENSE
--rw-rw-r--   0 samu      (1000) samu      (1000)      787 2023-07-08 10:03:03.184050 samus-logging-0.1.86/PKG-INFO
--rw-rw-r--   0 samu      (1000) samu      (1000)      365 2023-07-08 09:46:06.000000 samus-logging-0.1.86/README.md
-drwxrwxr-x   0 samu      (1000) samu      (1000)        0 2023-07-08 10:03:03.184050 samus-logging-0.1.86/samus_logging/
--rw-rw-r--   0 samu      (1000) samu      (1000)       83 2023-07-08 08:29:30.000000 samus-logging-0.1.86/samus_logging/__init__.py
--rw-rw-r--   0 samu      (1000) samu      (1000)      473 2023-07-08 08:28:01.000000 samus-logging-0.1.86/samus_logging/level_filter.py
--rw-rw-r--   0 samu      (1000) samu      (1000)     4797 2023-07-08 08:29:38.000000 samus-logging-0.1.86/samus_logging/samus_logging.py
-drwxrwxr-x   0 samu      (1000) samu      (1000)        0 2023-07-08 10:03:03.184050 samus-logging-0.1.86/samus_logging.egg-info/
--rw-rw-r--   0 samu      (1000) samu      (1000)      787 2023-07-08 10:03:03.000000 samus-logging-0.1.86/samus_logging.egg-info/PKG-INFO
--rw-rw-r--   0 samu      (1000) samu      (1000)      303 2023-07-08 10:03:03.000000 samus-logging-0.1.86/samus_logging.egg-info/SOURCES.txt
--rw-rw-r--   0 samu      (1000) samu      (1000)        1 2023-07-08 10:03:03.000000 samus-logging-0.1.86/samus_logging.egg-info/dependency_links.txt
--rw-rw-r--   0 samu      (1000) samu      (1000)       20 2023-07-08 10:03:03.000000 samus-logging-0.1.86/samus_logging.egg-info/requires.txt
--rw-rw-r--   0 samu      (1000) samu      (1000)       14 2023-07-08 10:03:03.000000 samus-logging-0.1.86/samus_logging.egg-info/top_level.txt
--rw-rw-r--   0 samu      (1000) samu      (1000)       38 2023-07-08 10:03:03.184050 samus-logging-0.1.86/setup.cfg
--rw-rw-r--   0 samu      (1000) samu      (1000)     1014 2023-07-08 10:02:31.000000 samus-logging-0.1.86/setup.py
+drwxrwxr-x   0 samu      (1000) samu      (1000)        0 2023-07-08 10:13:34.486878 samus-logging-0.1.88/
+-rw-rw-r--   0 samu      (1000) samu      (1000)        0 2023-06-28 14:33:05.000000 samus-logging-0.1.88/LICENSE
+-rw-rw-r--   0 samu      (1000) samu      (1000)     1095 2023-07-08 10:13:34.486878 samus-logging-0.1.88/PKG-INFO
+-rw-rw-r--   0 samu      (1000) samu      (1000)      365 2023-07-08 09:46:06.000000 samus-logging-0.1.88/README.md
+drwxrwxr-x   0 samu      (1000) samu      (1000)        0 2023-07-08 10:13:34.482878 samus-logging-0.1.88/samus_logging/
+-rw-rw-r--   0 samu      (1000) samu      (1000)       83 2023-07-08 08:29:30.000000 samus-logging-0.1.88/samus_logging/__init__.py
+-rw-rw-r--   0 samu      (1000) samu      (1000)      473 2023-07-08 08:28:01.000000 samus-logging-0.1.88/samus_logging/level_filter.py
+-rw-rw-r--   0 samu      (1000) samu      (1000)     4797 2023-07-08 08:29:38.000000 samus-logging-0.1.88/samus_logging/samus_logging.py
+drwxrwxr-x   0 samu      (1000) samu      (1000)        0 2023-07-08 10:13:34.482878 samus-logging-0.1.88/samus_logging.egg-info/
+-rw-rw-r--   0 samu      (1000) samu      (1000)     1095 2023-07-08 10:13:34.000000 samus-logging-0.1.88/samus_logging.egg-info/PKG-INFO
+-rw-rw-r--   0 samu      (1000) samu      (1000)      303 2023-07-08 10:13:34.000000 samus-logging-0.1.88/samus_logging.egg-info/SOURCES.txt
+-rw-rw-r--   0 samu      (1000) samu      (1000)        1 2023-07-08 10:13:34.000000 samus-logging-0.1.88/samus_logging.egg-info/dependency_links.txt
+-rw-rw-r--   0 samu      (1000) samu      (1000)       20 2023-07-08 10:13:34.000000 samus-logging-0.1.88/samus_logging.egg-info/requires.txt
+-rw-rw-r--   0 samu      (1000) samu      (1000)       14 2023-07-08 10:13:34.000000 samus-logging-0.1.88/samus_logging.egg-info/top_level.txt
+-rw-rw-r--   0 samu      (1000) samu      (1000)       38 2023-07-08 10:13:34.486878 samus-logging-0.1.88/setup.cfg
+-rw-rw-r--   0 samu      (1000) samu      (1000)     1290 2023-07-08 10:13:28.000000 samus-logging-0.1.88/setup.py
```

### Comparing `samus-logging-0.1.86/PKG-INFO` & `samus-logging-0.1.88/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,19 +1,24 @@
 Metadata-Version: 2.1
 Name: samus-logging
-Version: 0.1.86
+Version: 0.1.88
 Summary: A minimal Logging-controller.
-Home-page: UNKNOWN
+Home-page: https://github.com/Samus-Modules/Samus-Logging
 Author: Samu Rabin
 Author-email: samu.ca.rabin@gmail.com
 Maintainer: Samu Rabin
 Maintainer-email: samu.ca.rabin@gmail.com
 License: UNKNOWN
+Download-URL: https://github.com/Samus-Modules/Samus-Logging
 Keywords: python,logging,logger,minimal
 Platform: UNKNOWN
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: Programming Language :: Python :: 3
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 A minimal Logger-module for your projects.
```

### Comparing `samus-logging-0.1.86/samus_logging/samus_logging.py` & `samus-logging-0.1.88/samus_logging/samus_logging.py`

 * *Files identical despite different names*

### Comparing `samus-logging-0.1.86/samus_logging.egg-info/PKG-INFO` & `samus-logging-0.1.88/samus_logging.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,19 +1,24 @@
 Metadata-Version: 2.1
 Name: samus-logging
-Version: 0.1.86
+Version: 0.1.88
 Summary: A minimal Logging-controller.
-Home-page: UNKNOWN
+Home-page: https://github.com/Samus-Modules/Samus-Logging
 Author: Samu Rabin
 Author-email: samu.ca.rabin@gmail.com
 Maintainer: Samu Rabin
 Maintainer-email: samu.ca.rabin@gmail.com
 License: UNKNOWN
+Download-URL: https://github.com/Samus-Modules/Samus-Logging
 Keywords: python,logging,logger,minimal
 Platform: UNKNOWN
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: Programming Language :: Python :: 3
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 A minimal Logger-module for your projects.
```

### Comparing `samus-logging-0.1.86/setup.py` & `samus-logging-0.1.88/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -18,22 +18,25 @@
     name='samus-logging',
     version=read_file(f'VERSION'),
     python_requires='>=3.10',
     package_dir={'': '.'},
     packages=find_packages(where='.'),
     install_requires=[],
     extras_require={'dev': ['twine==4.0.2']},
-
-    # license='',
+    license='',  # TODO
     description='A minimal Logging-controller.',
     long_description=read_file('README.md'),
     long_description_content_type='text/markdown',
     author='Samu Rabin',
     author_email='samu.ca.rabin@gmail.com',
     maintainer='Samu Rabin',
     maintainer_email='samu.ca.rabin@gmail.com',
-    url='',
-    # download_url=''
-
+    url='https://github.com/Samus-Modules/Samus-Logging',
+    download_url='https://github.com/Samus-Modules/Samus-Logging',
     keywords=['python', 'logging', 'logger', 'minimal'],
-    # classifiers=setup_config['CLASSIFIERS'],
+    classifiers=[
+        'Development Status :: 4 - Beta',
+        'Intended Audience :: Developers',
+        'Programming Language :: Python :: 3',
+        'Topic :: Software Development :: Libraries :: Python Modules'
+    ],
 )
```

