# Comparing `tmp/bitssh-1.1.1.tar.gz` & `tmp/bitssh-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bitssh-1.1.1.tar", last modified: Fri Jul  7 21:31:14 2023, max compression
+gzip compressed data, was "bitssh-1.1.2.tar", last modified: Fri Jul  7 22:19:22 2023, max compression
```

## Comparing `bitssh-1.1.1.tar` & `bitssh-1.1.2.tar`

### file list

```diff
@@ -1,19 +1,22 @@
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-07-07 21:31:14.859950 bitssh-1.1.1/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1073 2023-06-25 12:55:13.000000 bitssh-1.1.1/LICENSE
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4836 2023-07-07 21:31:14.859950 bitssh-1.1.1/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3068 2023-07-07 21:29:25.000000 bitssh-1.1.1/README.md
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1176 2023-07-07 21:29:26.000000 bitssh-1.1.1/pyproject.toml
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2023-07-07 21:31:14.859950 bitssh-1.1.1/setup.cfg
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2023-07-07 21:29:26.000000 bitssh-1.1.1/setup.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-07-07 21:31:14.851951 bitssh-1.1.1/src/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       50 2023-07-07 21:29:26.000000 bitssh-1.1.1/src/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      453 2023-07-07 21:29:26.000000 bitssh-1.1.1/src/__main__.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-07-07 21:31:14.859950 bitssh-1.1.1/src/bitssh.egg-info/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4836 2023-07-07 21:31:14.000000 bitssh-1.1.1/src/bitssh.egg-info/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      304 2023-07-07 21:31:14.000000 bitssh-1.1.1/src/bitssh.egg-info/SOURCES.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-07-07 21:31:14.000000 bitssh-1.1.1/src/bitssh.egg-info/dependency_links.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       45 2023-07-07 21:31:14.000000 bitssh-1.1.1/src/bitssh.egg-info/entry_points.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       58 2023-07-07 21:31:14.000000 bitssh-1.1.1/src/bitssh.egg-info/requires.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       40 2023-07-07 21:31:14.000000 bitssh-1.1.1/src/bitssh.egg-info/top_level.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      995 2023-07-07 21:29:26.000000 bitssh-1.1.1/src/core.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      782 2023-07-07 21:29:26.000000 bitssh-1.1.1/src/utils.py
+drwxr-xr-x   0 itskanishkp  (1000) itskanishkp  (1000)        0 2023-07-07 22:19:22.960448 bitssh-1.1.2/
+-rw-r--r--   0 itskanishkp  (1000) itskanishkp  (1000)     1073 2023-07-03 17:33:19.000000 bitssh-1.1.2/LICENSE
+-rw-r--r--   0 itskanishkp  (1000) itskanishkp  (1000)     4836 2023-07-07 22:19:22.960448 bitssh-1.1.2/PKG-INFO
+-rw-r--r--   0 itskanishkp  (1000) itskanishkp  (1000)     3068 2023-07-07 20:38:00.000000 bitssh-1.1.2/README.md
+-rw-r--r--   0 itskanishkp  (1000) itskanishkp  (1000)     1179 2023-07-07 22:16:40.000000 bitssh-1.1.2/pyproject.toml
+-rw-r--r--   0 itskanishkp  (1000) itskanishkp  (1000)       38 2023-07-07 22:19:22.961448 bitssh-1.1.2/setup.cfg
+-rw-r--r--   0 itskanishkp  (1000) itskanishkp  (1000)       38 2023-07-07 20:09:24.000000 bitssh-1.1.2/setup.py
+drwxr-xr-x   0 itskanishkp  (1000) itskanishkp  (1000)        0 2023-07-07 22:19:22.957448 bitssh-1.1.2/src/
+drwxr-xr-x   0 itskanishkp  (1000) itskanishkp  (1000)        0 2023-07-07 22:19:22.959448 bitssh-1.1.2/src/bitssh/
+-rw-r--r--   0 itskanishkp  (1000) itskanishkp  (1000)      163 2023-07-07 22:16:17.000000 bitssh-1.1.2/src/bitssh/__init__.py
+-rw-r--r--   0 itskanishkp  (1000) itskanishkp  (1000)      453 2023-07-07 18:52:59.000000 bitssh-1.1.2/src/bitssh/__main__.py
+-rw-r--r--   0 itskanishkp  (1000) itskanishkp  (1000)     1056 2023-07-07 22:16:07.000000 bitssh-1.1.2/src/bitssh/core.py
+-rw-r--r--   0 itskanishkp  (1000) itskanishkp  (1000)      782 2023-07-07 18:30:45.000000 bitssh-1.1.2/src/bitssh/utils.py
+drwxr-xr-x   0 itskanishkp  (1000) itskanishkp  (1000)        0 2023-07-07 22:19:22.960448 bitssh-1.1.2/src/bitssh.egg-info/
+-rw-r--r--   0 itskanishkp  (1000) itskanishkp  (1000)     4836 2023-07-07 22:19:22.000000 bitssh-1.1.2/src/bitssh.egg-info/PKG-INFO
+-rw-r--r--   0 itskanishkp  (1000) itskanishkp  (1000)      352 2023-07-07 22:19:22.000000 bitssh-1.1.2/src/bitssh.egg-info/SOURCES.txt
+-rw-r--r--   0 itskanishkp  (1000) itskanishkp  (1000)        1 2023-07-07 22:19:22.000000 bitssh-1.1.2/src/bitssh.egg-info/dependency_links.txt
+-rw-r--r--   0 itskanishkp  (1000) itskanishkp  (1000)       48 2023-07-07 22:19:22.000000 bitssh-1.1.2/src/bitssh.egg-info/entry_points.txt
+-rw-r--r--   0 itskanishkp  (1000) itskanishkp  (1000)       58 2023-07-07 22:19:22.000000 bitssh-1.1.2/src/bitssh.egg-info/requires.txt
+-rw-r--r--   0 itskanishkp  (1000) itskanishkp  (1000)        7 2023-07-07 22:19:22.000000 bitssh-1.1.2/src/bitssh.egg-info/top_level.txt
+drwxr-xr-x   0 itskanishkp  (1000) itskanishkp  (1000)        0 2023-07-07 22:19:22.960448 bitssh-1.1.2/tests/
+-rw-r--r--   0 itskanishkp  (1000) itskanishkp  (1000)     1004 2023-07-07 22:13:44.000000 bitssh-1.1.2/tests/test_utils.py
```

### Comparing `bitssh-1.1.1/LICENSE` & `bitssh-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `bitssh-1.1.1/PKG-INFO` & `bitssh-1.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bitssh
-Version: 1.1.1
+Version: 1.1.2
 Summary: A command-line tool for managing SSH connections
 Author-email: Kanishk Pachauri <itskanishkp.py@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Kanishk Pachauri
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `bitssh-1.1.1/README.md` & `bitssh-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `bitssh-1.1.1/pyproject.toml` & `bitssh-1.1.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "bitssh"
-version = "1.1.1"
+version = "1.1.2"
 description = "A command-line tool for managing SSH connections"
 readme = "README.md"
 authors = [{ name = "Kanishk Pachauri", email = "itskanishkp.py@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
@@ -24,18 +24,18 @@
 [project.optional-dependencies]
 dev = ["black", "bumpver", "isort", "pip-tools", "pytest"]
 
 [project.urls]
 Homepage = "https://github.com/Mr-Sunglasses/bitssh"
 
 [project.scripts]
-bitssh = "src.__main__:main"
+bitssh = "bitssh.__main__:main"
 
 [tool.bumpver]
-current_version = "1.1.1"
+current_version = "1.1.2"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message  = "Bump version {old_version} -> {new_version}"
 commit          = true
 tag             = true
 push            = false
 
 [tool.bumpver.file_patterns]
```

### Comparing `bitssh-1.1.1/src/bitssh.egg-info/PKG-INFO` & `bitssh-1.1.2/src/bitssh.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bitssh
-Version: 1.1.1
+Version: 1.1.2
 Summary: A command-line tool for managing SSH connections
 Author-email: Kanishk Pachauri <itskanishkp.py@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Kanishk Pachauri
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `bitssh-1.1.1/src/core.py` & `bitssh-1.1.2/src/bitssh/core.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 from rich.console import Console
 from rich.table import Table
 import inquirer
 from . import utils
 try:
     content = utils.get_config_content(config_file=utils.get_config_path())
 except FileNotFoundError:
-    print("Config file is not Found in ~/.ssh/config")
+    raise Exception(
+        "Config file is not Found in ~/.ssh/config Please See the Docs of bitssh.")
 ROWS = []
 
 for host, attributes in content.items():
-    row = (attributes["Hostname"], host, attributes["port"], attributes["User"])
+    row = (attributes["Hostname"], host,
+           attributes["port"], attributes["User"])
     ROWS.append(row)
 
 
 table = Table(title="SSH Servers in Config File")
 
 table.add_column("Hostname", justify="left", style="cyan", no_wrap=True)
 table.add_column("Host", style="magenta")
```

### Comparing `bitssh-1.1.1/src/utils.py` & `bitssh-1.1.2/src/bitssh/utils.py`

 * *Files identical despite different names*

