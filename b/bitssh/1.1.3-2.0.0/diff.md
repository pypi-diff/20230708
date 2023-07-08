# Comparing `tmp/bitssh-1.1.3.tar.gz` & `tmp/bitssh-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bitssh-1.1.3.tar", last modified: Sat Jul  8 08:40:04 2023, max compression
+gzip compressed data, was "bitssh-2.0.0.tar", last modified: Sat Jul  8 18:58:08 2023, max compression
```

## Comparing `bitssh-1.1.3.tar` & `bitssh-2.0.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 08:40:04.477789 bitssh-1.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-08 08:39:48.000000 bitssh-1.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4920 2023-07-08 08:40:04.477789 bitssh-1.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3068 2023-07-08 08:39:48.000000 bitssh-1.1.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-07-08 08:39:48.000000 bitssh-1.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 08:40:04.477789 bitssh-1.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 08:39:48.000000 bitssh-1.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 08:40:04.473789 bitssh-1.1.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 08:40:04.473789 bitssh-1.1.3/src/bitssh/
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-07-08 08:39:48.000000 bitssh-1.1.3/src/bitssh/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-07-08 08:39:48.000000 bitssh-1.1.3/src/bitssh/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-07-08 08:39:48.000000 bitssh-1.1.3/src/bitssh/core.py
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-07-08 08:39:48.000000 bitssh-1.1.3/src/bitssh/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 08:40:04.477789 bitssh-1.1.3/src/bitssh.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4920 2023-07-08 08:40:04.000000 bitssh-1.1.3/src/bitssh.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-07-08 08:40:04.000000 bitssh-1.1.3/src/bitssh.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 08:40:04.000000 bitssh-1.1.3/src/bitssh.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-08 08:40:04.000000 bitssh-1.1.3/src/bitssh.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-08 08:40:04.000000 bitssh-1.1.3/src/bitssh.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-08 08:40:04.000000 bitssh-1.1.3/src/bitssh.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 08:40:04.477789 bitssh-1.1.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-07-08 08:39:48.000000 bitssh-1.1.3/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 18:58:08.780623 bitssh-2.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-08 18:57:53.000000 bitssh-2.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4920 2023-07-08 18:58:08.780623 bitssh-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3068 2023-07-08 18:57:53.000000 bitssh-2.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-07-08 18:57:53.000000 bitssh-2.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 18:58:08.780623 bitssh-2.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 18:57:53.000000 bitssh-2.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 18:58:08.776623 bitssh-2.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 18:58:08.780623 bitssh-2.0.0/src/bitssh/
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-07-08 18:57:53.000000 bitssh-2.0.0/src/bitssh/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-07-08 18:57:53.000000 bitssh-2.0.0/src/bitssh/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-07-08 18:57:53.000000 bitssh-2.0.0/src/bitssh/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-07-08 18:57:53.000000 bitssh-2.0.0/src/bitssh/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 18:58:08.780623 bitssh-2.0.0/src/bitssh.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4920 2023-07-08 18:58:08.000000 bitssh-2.0.0/src/bitssh.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-07-08 18:58:08.000000 bitssh-2.0.0/src/bitssh.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 18:58:08.000000 bitssh-2.0.0/src/bitssh.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-08 18:58:08.000000 bitssh-2.0.0/src/bitssh.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-08 18:58:08.000000 bitssh-2.0.0/src/bitssh.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-08 18:58:08.000000 bitssh-2.0.0/src/bitssh.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 18:58:08.780623 bitssh-2.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-07-08 18:57:53.000000 bitssh-2.0.0/tests/test_utils.py
```

### Comparing `bitssh-1.1.3/LICENSE` & `bitssh-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bitssh-1.1.3/PKG-INFO` & `bitssh-2.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bitssh
-Version: 1.1.3
+Version: 2.0.0
 Summary: A command-line tool for managing SSH connections
 Author-email: Kanishk Pachauri <itskanishkp.py@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Kanishk Pachauri
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `bitssh-1.1.3/README.md` & `bitssh-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `bitssh-1.1.3/pyproject.toml` & `bitssh-2.0.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "bitssh"
-version = "1.1.3"
+version = "2.0.0"
 description = "A command-line tool for managing SSH connections"
 readme = "README.md"
 authors = [{ name = "Kanishk Pachauri", email = "itskanishkp.py@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
@@ -28,17 +28,17 @@
 Homepage = "https://github.com/Mr-Sunglasses/bitssh"
 Docs = "https://github.com/Mr-Sunglasses/bitssh/blob/master/docs/docs.md"
 
 [project.scripts]
 bitssh = "bitssh.__main__:main"
 
 [tool.bumpver]
-current_version = "1.1.3"
+current_version = "2.0.0"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message  = "Bump version {old_version} -> {new_version}"
 commit          = true
 tag             = true
 push            = false
 
 [tool.bumpver.file_patterns]
 "pyproject.toml" = ['current_version = "{version}"', 'version = "{version}"']
-"src/__init__.py" = ["{version}"]
+"src/bitssh/__init__.py" = ["{version}"]
```

### Comparing `bitssh-1.1.3/src/bitssh/core.py` & `bitssh-2.0.0/src/bitssh/core.py`

 * *Files identical despite different names*

### Comparing `bitssh-1.1.3/src/bitssh/utils.py` & `bitssh-2.0.0/src/bitssh/utils.py`

 * *Files identical despite different names*

### Comparing `bitssh-1.1.3/src/bitssh.egg-info/PKG-INFO` & `bitssh-2.0.0/src/bitssh.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bitssh
-Version: 1.1.3
+Version: 2.0.0
 Summary: A command-line tool for managing SSH connections
 Author-email: Kanishk Pachauri <itskanishkp.py@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Kanishk Pachauri
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `bitssh-1.1.3/tests/test_utils.py` & `bitssh-2.0.0/tests/test_utils.py`

 * *Files identical despite different names*

