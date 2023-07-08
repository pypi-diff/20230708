# Comparing `tmp/pbcmd-6.0.tar.gz` & `tmp/pbcmd-7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pbcmd-6.0.tar", last modified: Mon Jun 19 13:43:11 2023, max compression
+gzip compressed data, was "pbcmd-7.1.tar", last modified: Sat Jul  8 18:00:11 2023, max compression
```

## Comparing `pbcmd-6.0.tar` & `pbcmd-7.1.tar`

### file list

```diff
@@ -1,30 +1,31 @@
-drwxr-xr-x   0 parantapa  (1000) parantapa  (1000)        0 2023-06-19 13:43:11.991117 pbcmd-6.0/
--rw-r--r--   0 parantapa  (1000) parantapa  (1000)     2035 2020-12-15 02:52:07.000000 pbcmd-6.0/.gitignore
--rw-r--r--   0 parantapa  (1000) parantapa  (1000)      667 2023-06-19 13:43:11.991117 pbcmd-6.0/PKG-INFO
--rw-r--r--   0 parantapa  (1000) parantapa  (1000)      245 2021-08-03 13:23:21.000000 pbcmd-6.0/README.rst
--rw-r--r--   0 parantapa  (1000) parantapa  (1000)      758 2023-06-19 13:42:46.000000 pbcmd-6.0/pyproject.toml
--rw-r--r--   0 parantapa  (1000) parantapa  (1000)       38 2023-06-19 13:43:11.991117 pbcmd-6.0/setup.cfg
--rw-r--r--   0 parantapa  (1000) parantapa  (1000)       37 2023-06-19 13:37:37.000000 pbcmd-6.0/setup.py
-drwxr-xr-x   0 parantapa  (1000) parantapa  (1000)        0 2023-06-19 13:43:11.987784 pbcmd-6.0/src/
-drwxr-xr-x   0 parantapa  (1000) parantapa  (1000)        0 2023-06-19 13:43:11.991117 pbcmd-6.0/src/pbcmd/
--rw-r--r--   0 parantapa  (1000) parantapa  (1000)        0 2021-07-29 14:48:36.000000 pbcmd-6.0/src/pbcmd/__init__.py
--rw-r--r--   0 parantapa  (1000) parantapa  (1000)      469 2023-06-06 00:18:27.000000 pbcmd-6.0/src/pbcmd/calc.py
--rw-r--r--   0 parantapa  (1000) parantapa  (1000)      814 2023-06-19 13:38:07.000000 pbcmd-6.0/src/pbcmd/cli.py
--rw-r--r--   0 parantapa  (1000) parantapa  (1000)     5710 2023-06-19 13:30:53.000000 pbcmd-6.0/src/pbcmd/cpush.py
--rw-r--r--   0 parantapa  (1000) parantapa  (1000)     3030 2023-05-24 14:27:43.000000 pbcmd-6.0/src/pbcmd/csplit.py
--rw-r--r--   0 parantapa  (1000) parantapa  (1000)     6585 2022-12-06 02:43:49.000000 pbcmd-6.0/src/pbcmd/git.py
--rw-r--r--   0 parantapa  (1000) parantapa  (1000)      208 2021-07-29 15:09:35.000000 pbcmd-6.0/src/pbcmd/hello.py
--rw-r--r--   0 parantapa  (1000) parantapa  (1000)     1783 2022-12-06 02:43:54.000000 pbcmd-6.0/src/pbcmd/mail.py
--rw-r--r--   0 parantapa  (1000) parantapa  (1000)     1773 2022-12-06 02:45:17.000000 pbcmd-6.0/src/pbcmd/obscure.py
--rw-r--r--   0 parantapa  (1000) parantapa  (1000)      416 2023-06-19 13:37:48.000000 pbcmd-6.0/src/pbcmd/pqcat.py
--rw-r--r--   0 parantapa  (1000) parantapa  (1000)     1069 2021-09-07 16:30:06.000000 pbcmd-6.0/src/pbcmd/proxy.py
--rw-r--r--   0 parantapa  (1000) parantapa  (1000)     1688 2022-12-06 02:47:02.000000 pbcmd-6.0/src/pbcmd/pyon2json.py
--rw-r--r--   0 parantapa  (1000) parantapa  (1000)     1891 2021-07-29 15:15:52.000000 pbcmd-6.0/src/pbcmd/rm_timestamped.py
--rw-r--r--   0 parantapa  (1000) parantapa  (1000)      746 2022-12-06 02:47:15.000000 pbcmd-6.0/src/pbcmd/timefmt.py
-drwxr-xr-x   0 parantapa  (1000) parantapa  (1000)        0 2023-06-19 13:43:11.991117 pbcmd-6.0/src/pbcmd.egg-info/
--rw-r--r--   0 parantapa  (1000) parantapa  (1000)      667 2023-06-19 13:43:11.000000 pbcmd-6.0/src/pbcmd.egg-info/PKG-INFO
--rw-r--r--   0 parantapa  (1000) parantapa  (1000)      526 2023-06-19 13:43:11.000000 pbcmd-6.0/src/pbcmd.egg-info/SOURCES.txt
--rw-r--r--   0 parantapa  (1000) parantapa  (1000)        1 2023-06-19 13:43:11.000000 pbcmd-6.0/src/pbcmd.egg-info/dependency_links.txt
--rw-r--r--   0 parantapa  (1000) parantapa  (1000)       37 2023-06-19 13:43:11.000000 pbcmd-6.0/src/pbcmd.egg-info/entry_points.txt
--rw-r--r--   0 parantapa  (1000) parantapa  (1000)       64 2023-06-19 13:43:11.000000 pbcmd-6.0/src/pbcmd.egg-info/requires.txt
--rw-r--r--   0 parantapa  (1000) parantapa  (1000)        6 2023-06-19 13:43:11.000000 pbcmd-6.0/src/pbcmd.egg-info/top_level.txt
+drwxr-xr-x   0 parantapa  (1000) parantapa  (1000)        0 2023-07-08 18:00:11.937866 pbcmd-7.1/
+-rw-r--r--   0 parantapa  (1000) parantapa  (1000)     2035 2020-12-15 02:52:07.000000 pbcmd-7.1/.gitignore
+-rw-r--r--   0 parantapa  (1000) parantapa  (1000)      667 2023-07-08 18:00:11.937866 pbcmd-7.1/PKG-INFO
+-rw-r--r--   0 parantapa  (1000) parantapa  (1000)      245 2021-08-03 13:23:21.000000 pbcmd-7.1/README.rst
+-rw-r--r--   0 parantapa  (1000) parantapa  (1000)      785 2023-07-08 17:55:21.000000 pbcmd-7.1/pyproject.toml
+-rw-r--r--   0 parantapa  (1000) parantapa  (1000)       38 2023-07-08 18:00:11.937866 pbcmd-7.1/setup.cfg
+-rw-r--r--   0 parantapa  (1000) parantapa  (1000)       37 2023-06-19 13:37:37.000000 pbcmd-7.1/setup.py
+drwxr-xr-x   0 parantapa  (1000) parantapa  (1000)        0 2023-07-08 18:00:11.601199 pbcmd-7.1/src/
+drwxr-xr-x   0 parantapa  (1000) parantapa  (1000)        0 2023-07-08 18:00:11.931199 pbcmd-7.1/src/pbcmd/
+-rw-r--r--   0 parantapa  (1000) parantapa  (1000)        0 2021-07-29 14:48:36.000000 pbcmd-7.1/src/pbcmd/__init__.py
+-rw-r--r--   0 parantapa  (1000) parantapa  (1000)      469 2023-06-06 00:18:27.000000 pbcmd-7.1/src/pbcmd/calc.py
+-rw-r--r--   0 parantapa  (1000) parantapa  (1000)      868 2023-07-08 15:58:19.000000 pbcmd-7.1/src/pbcmd/cli.py
+-rw-r--r--   0 parantapa  (1000) parantapa  (1000)     5710 2023-06-19 13:30:53.000000 pbcmd-7.1/src/pbcmd/cpush.py
+-rw-r--r--   0 parantapa  (1000) parantapa  (1000)     3030 2023-05-24 14:27:43.000000 pbcmd-7.1/src/pbcmd/csplit.py
+-rw-r--r--   0 parantapa  (1000) parantapa  (1000)     2733 2023-07-08 17:05:35.000000 pbcmd-7.1/src/pbcmd/csv2tex.py
+-rw-r--r--   0 parantapa  (1000) parantapa  (1000)     6585 2022-12-06 02:43:49.000000 pbcmd-7.1/src/pbcmd/git.py
+-rw-r--r--   0 parantapa  (1000) parantapa  (1000)      208 2021-07-29 15:09:35.000000 pbcmd-7.1/src/pbcmd/hello.py
+-rw-r--r--   0 parantapa  (1000) parantapa  (1000)     1783 2022-12-06 02:43:54.000000 pbcmd-7.1/src/pbcmd/mail.py
+-rw-r--r--   0 parantapa  (1000) parantapa  (1000)     1773 2022-12-06 02:45:17.000000 pbcmd-7.1/src/pbcmd/obscure.py
+-rw-r--r--   0 parantapa  (1000) parantapa  (1000)      416 2023-06-19 13:37:48.000000 pbcmd-7.1/src/pbcmd/pqcat.py
+-rw-r--r--   0 parantapa  (1000) parantapa  (1000)     1069 2021-09-07 16:30:06.000000 pbcmd-7.1/src/pbcmd/proxy.py
+-rw-r--r--   0 parantapa  (1000) parantapa  (1000)     1688 2022-12-06 02:47:02.000000 pbcmd-7.1/src/pbcmd/pyon2json.py
+-rw-r--r--   0 parantapa  (1000) parantapa  (1000)     1891 2021-07-29 15:15:52.000000 pbcmd-7.1/src/pbcmd/rm_timestamped.py
+-rw-r--r--   0 parantapa  (1000) parantapa  (1000)      746 2022-12-06 02:47:15.000000 pbcmd-7.1/src/pbcmd/timefmt.py
+drwxr-xr-x   0 parantapa  (1000) parantapa  (1000)        0 2023-07-08 18:00:11.937866 pbcmd-7.1/src/pbcmd.egg-info/
+-rw-r--r--   0 parantapa  (1000) parantapa  (1000)      667 2023-07-08 18:00:11.000000 pbcmd-7.1/src/pbcmd.egg-info/PKG-INFO
+-rw-r--r--   0 parantapa  (1000) parantapa  (1000)      547 2023-07-08 18:00:11.000000 pbcmd-7.1/src/pbcmd.egg-info/SOURCES.txt
+-rw-r--r--   0 parantapa  (1000) parantapa  (1000)        1 2023-07-08 18:00:11.000000 pbcmd-7.1/src/pbcmd.egg-info/dependency_links.txt
+-rw-r--r--   0 parantapa  (1000) parantapa  (1000)       37 2023-07-08 18:00:11.000000 pbcmd-7.1/src/pbcmd.egg-info/entry_points.txt
+-rw-r--r--   0 parantapa  (1000) parantapa  (1000)       77 2023-07-08 18:00:11.000000 pbcmd-7.1/src/pbcmd.egg-info/requires.txt
+-rw-r--r--   0 parantapa  (1000) parantapa  (1000)        6 2023-07-08 18:00:11.000000 pbcmd-7.1/src/pbcmd.egg-info/top_level.txt
```

### Comparing `pbcmd-6.0/.gitignore` & `pbcmd-7.1/.gitignore`

 * *Files identical despite different names*

### Comparing `pbcmd-6.0/PKG-INFO` & `pbcmd-7.1/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pbcmd
-Version: 6.0
+Version: 7.1
 Summary: PB's miscellaneous command line tools.
 Author-email: Parantapa Bhattacharya <pb+pypi@parantapa.net>
 Project-URL: Homepage, https://github.com/parantapa/pbcmd
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
```

### Comparing `pbcmd-6.0/pyproject.toml` & `pbcmd-7.1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pbcmd"
-version = "6.0"
+version = "7.1"
 authors = [
   { name="Parantapa Bhattacharya", email="pb+pypi@parantapa.net" },
 ]
 description = "PB's miscellaneous command line tools."
 readme = "README.rst"
 requires-python = ">=3.10"
 classifiers = [
@@ -21,15 +21,17 @@
     "click",
     "python-dateutil",
     "wasabi",
     "tqdm",
     "pydantic",
     "json5",
     "pandas",
-    "pyarrow"
+    "pyarrow",
+    "attrs",
+    "cattrs"
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/parantapa/pbcmd"
 
 [tool.setuptools.packages.find]
 where = ["src"]
```

### Comparing `pbcmd-6.0/src/pbcmd/cli.py` & `pbcmd-7.1/src/pbcmd/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from .proxy import proxy
 from .timefmt import timefmt
 from .git import git
 from .pyon2json import pyon2json
 from .csplit import csplit
 from .cpush import cpush
 from .pqcat import pqcat
+from .csv2tex import csv2tex
 
 # from .rm_timestamped import rm_timestamped
 from .obscure import obscure, unobscure
 from .mail import mail
 
 
 @click.group()
@@ -31,10 +32,11 @@
 cli.add_command(csplit)
 cli.add_command(cpush)
 # cli.add_command(rm_timestamped)
 cli.add_command(obscure)
 cli.add_command(unobscure)
 cli.add_command(mail)
 cli.add_command(pqcat)
+cli.add_command(csv2tex)
 
 if __name__ == "__main__":
     cli(prog_name="pb")
```

### Comparing `pbcmd-6.0/src/pbcmd/cpush.py` & `pbcmd-7.1/src/pbcmd/cpush.py`

 * *Files identical despite different names*

### Comparing `pbcmd-6.0/src/pbcmd/csplit.py` & `pbcmd-7.1/src/pbcmd/csplit.py`

 * *Files identical despite different names*

### Comparing `pbcmd-6.0/src/pbcmd/git.py` & `pbcmd-7.1/src/pbcmd/git.py`

 * *Files identical despite different names*

### Comparing `pbcmd-6.0/src/pbcmd/mail.py` & `pbcmd-7.1/src/pbcmd/mail.py`

 * *Files identical despite different names*

### Comparing `pbcmd-6.0/src/pbcmd/obscure.py` & `pbcmd-7.1/src/pbcmd/obscure.py`

 * *Files identical despite different names*

### Comparing `pbcmd-6.0/src/pbcmd/proxy.py` & `pbcmd-7.1/src/pbcmd/proxy.py`

 * *Files identical despite different names*

### Comparing `pbcmd-6.0/src/pbcmd/pyon2json.py` & `pbcmd-7.1/src/pbcmd/pyon2json.py`

 * *Files identical despite different names*

### Comparing `pbcmd-6.0/src/pbcmd/rm_timestamped.py` & `pbcmd-7.1/src/pbcmd/rm_timestamped.py`

 * *Files identical despite different names*

### Comparing `pbcmd-6.0/src/pbcmd/timefmt.py` & `pbcmd-7.1/src/pbcmd/timefmt.py`

 * *Files identical despite different names*

### Comparing `pbcmd-6.0/src/pbcmd.egg-info/PKG-INFO` & `pbcmd-7.1/src/pbcmd.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pbcmd
-Version: 6.0
+Version: 7.1
 Summary: PB's miscellaneous command line tools.
 Author-email: Parantapa Bhattacharya <pb+pypi@parantapa.net>
 Project-URL: Homepage, https://github.com/parantapa/pbcmd
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
```

