# Comparing `tmp/ColabGeek-1.2.1.tar.gz` & `tmp/ColabGeek-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ColabGeek-1.2.1.tar", last modified: Sat May 27 12:39:37 2023, max compression
+gzip compressed data, was "ColabGeek-1.2.2.tar", last modified: Sat Jul  8 03:52:19 2023, max compression
```

## Comparing `ColabGeek-1.2.1.tar` & `ColabGeek-1.2.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-27 12:39:37.282796 ColabGeek-1.2.1/
--rw-rw-r--   0 root         (0) root         (0)     1067 2023-05-27 12:10:14.000000 ColabGeek-1.2.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     7171 2023-05-27 12:39:37.281796 ColabGeek-1.2.1/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)     6434 2023-05-27 12:28:30.000000 ColabGeek-1.2.1/README.md
--rw-rw-r--   0 root         (0) root         (0)      939 2023-05-27 12:28:30.000000 ColabGeek-1.2.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-27 12:39:37.282796 ColabGeek-1.2.1/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-27 12:39:37.278796 ColabGeek-1.2.1/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-27 12:39:37.280796 ColabGeek-1.2.1/src/ColabGeek/
--rw-rw-r--   0 root         (0) root         (0)    11496 2023-05-27 12:28:30.000000 ColabGeek-1.2.1/src/ColabGeek/ColabGeek.py
--rw-rw-r--   0 root         (0) root         (0)       24 2023-05-27 12:10:14.000000 ColabGeek-1.2.1/src/ColabGeek/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-27 12:39:37.281796 ColabGeek-1.2.1/src/ColabGeek/shell_scripts/
--rw-rw-r--   0 root         (0) root         (0)      816 2023-05-27 12:28:30.000000 ColabGeek-1.2.1/src/ColabGeek/shell_scripts/Install_Homebrew.exp
--rw-rw-r--   0 root         (0) root         (0)      324 2023-05-27 12:28:30.000000 ColabGeek-1.2.1/src/ColabGeek/shell_scripts/Install_Jekyll.exp
--rw-rw-r--   0 root         (0) root         (0)      485 2023-05-27 12:28:30.000000 ColabGeek-1.2.1/src/ColabGeek/shell_scripts/Install_Ruby.exp
--rw-rw-r--   0 root         (0) root         (0)      442 2023-05-27 12:28:30.000000 ColabGeek-1.2.1/src/ColabGeek/shell_scripts/Install_rbenv.exp
--rw-rw-r--   0 root         (0) root         (0)      382 2023-05-27 12:10:14.000000 ColabGeek-1.2.1/src/ColabGeek/shell_scripts/Run_Rstudio_server.sh
--rw-rw-r--   0 root         (0) root         (0)     1192 2023-05-27 12:10:14.000000 ColabGeek-1.2.1/src/ColabGeek/shell_scripts/Run_code_server.exp
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-27 12:39:37.280796 ColabGeek-1.2.1/src/ColabGeek.egg-info/
--rw-r--r--   0 root         (0) root         (0)     7171 2023-05-27 12:39:37.000000 ColabGeek-1.2.1/src/ColabGeek.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      518 2023-05-27 12:39:37.000000 ColabGeek-1.2.1/src/ColabGeek.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-27 12:39:37.000000 ColabGeek-1.2.1/src/ColabGeek.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-05-27 12:39:37.000000 ColabGeek-1.2.1/src/ColabGeek.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-08 03:52:19.181100 ColabGeek-1.2.2/
+-rw-rw-r--   0 root         (0) root         (0)     1067 2023-07-08 03:33:26.000000 ColabGeek-1.2.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     7171 2023-07-08 03:52:19.181100 ColabGeek-1.2.2/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)     6434 2023-07-08 03:33:26.000000 ColabGeek-1.2.2/README.md
+-rw-rw-r--   0 root         (0) root         (0)      939 2023-07-08 03:43:44.000000 ColabGeek-1.2.2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-08 03:52:19.181100 ColabGeek-1.2.2/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-08 03:52:19.178100 ColabGeek-1.2.2/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-08 03:52:19.179100 ColabGeek-1.2.2/src/ColabGeek/
+-rw-rw-r--   0 root         (0) root         (0)    11496 2023-07-08 03:33:26.000000 ColabGeek-1.2.2/src/ColabGeek/ColabGeek.py
+-rw-rw-r--   0 root         (0) root         (0)       24 2023-07-08 03:33:26.000000 ColabGeek-1.2.2/src/ColabGeek/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-08 03:52:19.181100 ColabGeek-1.2.2/src/ColabGeek/shell_scripts/
+-rw-rw-r--   0 root         (0) root         (0)      816 2023-07-08 03:33:26.000000 ColabGeek-1.2.2/src/ColabGeek/shell_scripts/Install_Homebrew.exp
+-rw-rw-r--   0 root         (0) root         (0)      324 2023-07-08 03:33:26.000000 ColabGeek-1.2.2/src/ColabGeek/shell_scripts/Install_Jekyll.exp
+-rw-rw-r--   0 root         (0) root         (0)      485 2023-07-08 03:33:26.000000 ColabGeek-1.2.2/src/ColabGeek/shell_scripts/Install_Ruby.exp
+-rw-rw-r--   0 root         (0) root         (0)      442 2023-07-08 03:33:26.000000 ColabGeek-1.2.2/src/ColabGeek/shell_scripts/Install_rbenv.exp
+-rw-rw-r--   0 root         (0) root         (0)      381 2023-07-08 03:43:44.000000 ColabGeek-1.2.2/src/ColabGeek/shell_scripts/Run_Rstudio_server.sh
+-rw-rw-r--   0 root         (0) root         (0)     1192 2023-07-08 03:33:26.000000 ColabGeek-1.2.2/src/ColabGeek/shell_scripts/Run_code_server.exp
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-08 03:52:19.180101 ColabGeek-1.2.2/src/ColabGeek.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     7171 2023-07-08 03:52:19.000000 ColabGeek-1.2.2/src/ColabGeek.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      518 2023-07-08 03:52:19.000000 ColabGeek-1.2.2/src/ColabGeek.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-08 03:52:19.000000 ColabGeek-1.2.2/src/ColabGeek.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-07-08 03:52:19.000000 ColabGeek-1.2.2/src/ColabGeek.egg-info/top_level.txt
```

### Comparing `ColabGeek-1.2.1/LICENSE` & `ColabGeek-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ColabGeek-1.2.1/PKG-INFO` & `ColabGeek-1.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ColabGeek
-Version: 1.2.1
+Version: 1.2.2
 Summary: ColabGeek is designed to help run useful tools on Google Colab, including port forwarding, web IDE and so on. It is worth noting that this package is also compatible with other Ubuntu operating system servers, so try on other platforms as well.
 Author-email: Yiming Sun <yiming.sun12138@gmail.com>
 Project-URL: Homepage, https://github.com/yimingsun12138/ColabGeek
 Project-URL: Bug Tracker, https://github.com/yimingsun12138/ColabGeek/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `ColabGeek-1.2.1/README.md` & `ColabGeek-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `ColabGeek-1.2.1/pyproject.toml` & `ColabGeek-1.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 where = ["src"]
 
 [tool.setuptools.package-data]
 "ColabGeek.shell_scripts" = ["*"]
 
 [project]
 name = "ColabGeek"
-version = "1.2.1"
+version = "1.2.2"
 authors = [
     {name = "Yiming Sun",email = "yiming.sun12138@gmail.com"},
 ]
 description = "ColabGeek is designed to help run useful tools on Google Colab, including port forwarding, web IDE and so on. It is worth noting that this package is also compatible with other Ubuntu operating system servers, so try on other platforms as well."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `ColabGeek-1.2.1/src/ColabGeek/ColabGeek.py` & `ColabGeek-1.2.2/src/ColabGeek/ColabGeek.py`

 * *Files identical despite different names*

### Comparing `ColabGeek-1.2.1/src/ColabGeek/shell_scripts/Install_Homebrew.exp` & `ColabGeek-1.2.2/src/ColabGeek/shell_scripts/Install_Homebrew.exp`

 * *Files identical despite different names*

### Comparing `ColabGeek-1.2.1/src/ColabGeek/shell_scripts/Run_code_server.exp` & `ColabGeek-1.2.2/src/ColabGeek/shell_scripts/Run_code_server.exp`

 * *Files identical despite different names*

### Comparing `ColabGeek-1.2.1/src/ColabGeek.egg-info/PKG-INFO` & `ColabGeek-1.2.2/src/ColabGeek.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ColabGeek
-Version: 1.2.1
+Version: 1.2.2
 Summary: ColabGeek is designed to help run useful tools on Google Colab, including port forwarding, web IDE and so on. It is worth noting that this package is also compatible with other Ubuntu operating system servers, so try on other platforms as well.
 Author-email: Yiming Sun <yiming.sun12138@gmail.com>
 Project-URL: Homepage, https://github.com/yimingsun12138/ColabGeek
 Project-URL: Bug Tracker, https://github.com/yimingsun12138/ColabGeek/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `ColabGeek-1.2.1/src/ColabGeek.egg-info/SOURCES.txt` & `ColabGeek-1.2.2/src/ColabGeek.egg-info/SOURCES.txt`

 * *Files identical despite different names*

