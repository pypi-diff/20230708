# Comparing `tmp/FiveMCipherFinder-1.6.0.tar.gz` & `tmp/FiveMCipherFinder-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FiveMCipherFinder-1.6.0.tar", last modified: Sun Oct  2 12:03:48 2022, max compression
+gzip compressed data, was "FiveMCipherFinder-2.0.0.tar", last modified: Sat Jul  8 12:18:22 2023, max compression
```

## Comparing `FiveMCipherFinder-1.6.0.tar` & `FiveMCipherFinder-2.0.0.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-02 12:03:48.245931 FiveMCipherFinder-1.6.0/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-02 12:03:48.245931 FiveMCipherFinder-1.6.0/FiveMCipherFinder.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1794 2022-10-02 12:03:48.000000 FiveMCipherFinder-1.6.0/FiveMCipherFinder.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      307 2022-10-02 12:03:48.000000 FiveMCipherFinder-1.6.0/FiveMCipherFinder.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-02 12:03:48.000000 FiveMCipherFinder-1.6.0/FiveMCipherFinder.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       50 2022-10-02 12:03:48.000000 FiveMCipherFinder-1.6.0/FiveMCipherFinder.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       13 2022-10-02 12:03:48.000000 FiveMCipherFinder-1.6.0/FiveMCipherFinder.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1078 2022-10-02 12:03:35.000000 FiveMCipherFinder-1.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     1794 2022-10-02 12:03:48.245931 FiveMCipherFinder-1.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1168 2022-10-02 12:03:35.000000 FiveMCipherFinder-1.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-02 12:03:48.245931 FiveMCipherFinder-1.6.0/cipherFinder/
--rw-r--r--   0 runner    (1001) docker     (121)       64 2022-10-02 12:03:35.000000 FiveMCipherFinder-1.6.0/cipherFinder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4242 2022-10-02 12:03:35.000000 FiveMCipherFinder-1.6.0/cipherFinder/finder.py
--rw-r--r--   0 runner    (1001) docker     (121)      107 2022-10-02 12:03:35.000000 FiveMCipherFinder-1.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      737 2022-10-02 12:03:48.245931 FiveMCipherFinder-1.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)       37 2022-10-02 12:03:35.000000 FiveMCipherFinder-1.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 12:18:22.530048 FiveMCipherFinder-2.0.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 12:18:22.530048 FiveMCipherFinder-2.0.0/FiveMCipherFinder.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-07-08 12:18:22.000000 FiveMCipherFinder-2.0.0/FiveMCipherFinder.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-07-08 12:18:22.000000 FiveMCipherFinder-2.0.0/FiveMCipherFinder.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 12:18:22.000000 FiveMCipherFinder-2.0.0/FiveMCipherFinder.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-08 12:18:22.000000 FiveMCipherFinder-2.0.0/FiveMCipherFinder.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-08 12:18:22.000000 FiveMCipherFinder-2.0.0/FiveMCipherFinder.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-08 12:18:22.000000 FiveMCipherFinder-2.0.0/FiveMCipherFinder.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-07-08 12:18:10.000000 FiveMCipherFinder-2.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-07-08 12:18:22.530048 FiveMCipherFinder-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-07-08 12:18:10.000000 FiveMCipherFinder-2.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 12:18:22.530048 FiveMCipherFinder-2.0.0/cipherFinder/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-08 12:18:10.000000 FiveMCipherFinder-2.0.0/cipherFinder/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6840 2023-07-08 12:18:10.000000 FiveMCipherFinder-2.0.0/cipherFinder/finder.py
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-08 12:18:10.000000 FiveMCipherFinder-2.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-07-08 12:18:22.530048 FiveMCipherFinder-2.0.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)       37 2023-07-08 12:18:10.000000 FiveMCipherFinder-2.0.0/setup.py
```

### Comparing `FiveMCipherFinder-1.6.0/LICENSE` & `FiveMCipherFinder-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `FiveMCipherFinder-1.6.0/setup.cfg` & `FiveMCipherFinder-2.0.0/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = FiveMCipherFinder
-version = 1.6.0
+version = 2.0.0
 description = Finds Cipher in lua scripts.
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = MIT
 author = exersalza
 url = https://github.com/exersalza/FivemCipherFinder
 project_urls = 
@@ -14,14 +14,16 @@
 	Intended Audience :: Developers
 	License :: OSI Approved :: MIT License
 	Operating System :: OS Independent
 	Programming Language :: Python :: 3
 	Topic :: Software Development
 
 [options]
+install_requires = 
+	gibberish_detector
 packages = cipherFinder
 
 [options.entry_points]
 console_scripts = 
 	find-cipher = cipherFinder:main
 
 [egg_info]
```

