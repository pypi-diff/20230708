# Comparing `tmp/bitssh-1.1.2.tar.gz` & `tmp/bitssh-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bitssh-1.1.2.tar", last modified: Fri Jul  7 22:19:22 2023, max compression
+gzip compressed data, was "bitssh-1.1.3.tar", last modified: Sat Jul  8 08:40:04 2023, max compression
```

## Comparing `bitssh-1.1.2.tar` & `bitssh-1.1.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 itskanishkp  (1000) itskanishkp  (1000)        0 2023-07-07 22:19:22.960448 bitssh-1.1.2/
--rw-r--r--   0 itskanishkp  (1000) itskanishkp  (1000)     1073 2023-07-03 17:33:19.000000 bitssh-1.1.2/LICENSE
--rw-r--r--   0 itskanishkp  (1000) itskanishkp  (1000)     4836 2023-07-07 22:19:22.960448 bitssh-1.1.2/PKG-INFO
--rw-r--r--   0 itskanishkp  (1000) itskanishkp  (1000)     3068 2023-07-07 20:38:00.000000 bitssh-1.1.2/README.md
--rw-r--r--   0 itskanishkp  (1000) itskanishkp  (1000)     1179 2023-07-07 22:16:40.000000 bitssh-1.1.2/pyproject.toml
--rw-r--r--   0 itskanishkp  (1000) itskanishkp  (1000)       38 2023-07-07 22:19:22.961448 bitssh-1.1.2/setup.cfg
--rw-r--r--   0 itskanishkp  (1000) itskanishkp  (1000)       38 2023-07-07 20:09:24.000000 bitssh-1.1.2/setup.py
-drwxr-xr-x   0 itskanishkp  (1000) itskanishkp  (1000)        0 2023-07-07 22:19:22.957448 bitssh-1.1.2/src/
-drwxr-xr-x   0 itskanishkp  (1000) itskanishkp  (1000)        0 2023-07-07 22:19:22.959448 bitssh-1.1.2/src/bitssh/
--rw-r--r--   0 itskanishkp  (1000) itskanishkp  (1000)      163 2023-07-07 22:16:17.000000 bitssh-1.1.2/src/bitssh/__init__.py
--rw-r--r--   0 itskanishkp  (1000) itskanishkp  (1000)      453 2023-07-07 18:52:59.000000 bitssh-1.1.2/src/bitssh/__main__.py
--rw-r--r--   0 itskanishkp  (1000) itskanishkp  (1000)     1056 2023-07-07 22:16:07.000000 bitssh-1.1.2/src/bitssh/core.py
--rw-r--r--   0 itskanishkp  (1000) itskanishkp  (1000)      782 2023-07-07 18:30:45.000000 bitssh-1.1.2/src/bitssh/utils.py
-drwxr-xr-x   0 itskanishkp  (1000) itskanishkp  (1000)        0 2023-07-07 22:19:22.960448 bitssh-1.1.2/src/bitssh.egg-info/
--rw-r--r--   0 itskanishkp  (1000) itskanishkp  (1000)     4836 2023-07-07 22:19:22.000000 bitssh-1.1.2/src/bitssh.egg-info/PKG-INFO
--rw-r--r--   0 itskanishkp  (1000) itskanishkp  (1000)      352 2023-07-07 22:19:22.000000 bitssh-1.1.2/src/bitssh.egg-info/SOURCES.txt
--rw-r--r--   0 itskanishkp  (1000) itskanishkp  (1000)        1 2023-07-07 22:19:22.000000 bitssh-1.1.2/src/bitssh.egg-info/dependency_links.txt
--rw-r--r--   0 itskanishkp  (1000) itskanishkp  (1000)       48 2023-07-07 22:19:22.000000 bitssh-1.1.2/src/bitssh.egg-info/entry_points.txt
--rw-r--r--   0 itskanishkp  (1000) itskanishkp  (1000)       58 2023-07-07 22:19:22.000000 bitssh-1.1.2/src/bitssh.egg-info/requires.txt
--rw-r--r--   0 itskanishkp  (1000) itskanishkp  (1000)        7 2023-07-07 22:19:22.000000 bitssh-1.1.2/src/bitssh.egg-info/top_level.txt
-drwxr-xr-x   0 itskanishkp  (1000) itskanishkp  (1000)        0 2023-07-07 22:19:22.960448 bitssh-1.1.2/tests/
--rw-r--r--   0 itskanishkp  (1000) itskanishkp  (1000)     1004 2023-07-07 22:13:44.000000 bitssh-1.1.2/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 08:40:04.477789 bitssh-1.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-08 08:39:48.000000 bitssh-1.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4920 2023-07-08 08:40:04.477789 bitssh-1.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3068 2023-07-08 08:39:48.000000 bitssh-1.1.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-07-08 08:39:48.000000 bitssh-1.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 08:40:04.477789 bitssh-1.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 08:39:48.000000 bitssh-1.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 08:40:04.473789 bitssh-1.1.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 08:40:04.473789 bitssh-1.1.3/src/bitssh/
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-07-08 08:39:48.000000 bitssh-1.1.3/src/bitssh/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-07-08 08:39:48.000000 bitssh-1.1.3/src/bitssh/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-07-08 08:39:48.000000 bitssh-1.1.3/src/bitssh/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-07-08 08:39:48.000000 bitssh-1.1.3/src/bitssh/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 08:40:04.477789 bitssh-1.1.3/src/bitssh.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4920 2023-07-08 08:40:04.000000 bitssh-1.1.3/src/bitssh.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-07-08 08:40:04.000000 bitssh-1.1.3/src/bitssh.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 08:40:04.000000 bitssh-1.1.3/src/bitssh.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-08 08:40:04.000000 bitssh-1.1.3/src/bitssh.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-08 08:40:04.000000 bitssh-1.1.3/src/bitssh.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-08 08:40:04.000000 bitssh-1.1.3/src/bitssh.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 08:40:04.477789 bitssh-1.1.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-07-08 08:39:48.000000 bitssh-1.1.3/tests/test_utils.py
```

### Comparing `bitssh-1.1.2/LICENSE` & `bitssh-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `bitssh-1.1.2/PKG-INFO` & `bitssh-1.1.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bitssh
-Version: 1.1.2
+Version: 1.1.3
 Summary: A command-line tool for managing SSH connections
 Author-email: Kanishk Pachauri <itskanishkp.py@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Kanishk Pachauri
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -22,14 +22,15 @@
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Project-URL: Homepage, https://github.com/Mr-Sunglasses/bitssh
+Project-URL: Docs, https://github.com/Mr-Sunglasses/bitssh/blob/master/docs/docs.md
 Keywords: bitssh,sshmanager,commandline
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

### Comparing `bitssh-1.1.2/README.md` & `bitssh-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `bitssh-1.1.2/pyproject.toml` & `bitssh-1.1.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "bitssh"
-version = "1.1.2"
+version = "1.1.3"
 description = "A command-line tool for managing SSH connections"
 readme = "README.md"
 authors = [{ name = "Kanishk Pachauri", email = "itskanishkp.py@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
@@ -22,20 +22,21 @@
 requires-python = ">=3.9"
 
 [project.optional-dependencies]
 dev = ["black", "bumpver", "isort", "pip-tools", "pytest"]
 
 [project.urls]
 Homepage = "https://github.com/Mr-Sunglasses/bitssh"
+Docs = "https://github.com/Mr-Sunglasses/bitssh/blob/master/docs/docs.md"
 
 [project.scripts]
 bitssh = "bitssh.__main__:main"
 
 [tool.bumpver]
-current_version = "1.1.2"
+current_version = "1.1.3"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message  = "Bump version {old_version} -> {new_version}"
 commit          = true
 tag             = true
 push            = false
 
 [tool.bumpver.file_patterns]
```

### Comparing `bitssh-1.1.2/src/bitssh/core.py` & `bitssh-1.1.3/src/bitssh/core.py`

 * *Files identical despite different names*

### Comparing `bitssh-1.1.2/src/bitssh/utils.py` & `bitssh-1.1.3/src/bitssh/utils.py`

 * *Files identical despite different names*

### Comparing `bitssh-1.1.2/src/bitssh.egg-info/PKG-INFO` & `bitssh-1.1.3/src/bitssh.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bitssh
-Version: 1.1.2
+Version: 1.1.3
 Summary: A command-line tool for managing SSH connections
 Author-email: Kanishk Pachauri <itskanishkp.py@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Kanishk Pachauri
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -22,14 +22,15 @@
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Project-URL: Homepage, https://github.com/Mr-Sunglasses/bitssh
+Project-URL: Docs, https://github.com/Mr-Sunglasses/bitssh/blob/master/docs/docs.md
 Keywords: bitssh,sshmanager,commandline
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

### Comparing `bitssh-1.1.2/tests/test_utils.py` & `bitssh-1.1.3/tests/test_utils.py`

 * *Files identical despite different names*

