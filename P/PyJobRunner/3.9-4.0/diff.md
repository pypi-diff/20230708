# Comparing `tmp/PyJobRunner-3.9.tar.gz` & `tmp/PyJobRunner-4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyJobRunner-3.9.tar", last modified: Thu Feb 16 16:48:55 2023, max compression
+gzip compressed data, was "PyJobRunner-4.0.tar", last modified: Thu Feb 16 23:47:06 2023, max compression
```

## Comparing `PyJobRunner-3.9.tar` & `PyJobRunner-4.0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxr-x   0 akash     (1001) akash     (1001)        0 2023-02-16 16:48:55.311907 PyJobRunner-3.9/
--rw-rw-r--   0 akash     (1001) akash     (1001)     1068 2022-10-04 16:17:57.000000 PyJobRunner-3.9/LICENSE
--rw-rw-r--   0 akash     (1001) akash     (1001)       51 2022-10-19 20:21:58.000000 PyJobRunner-3.9/MANIFEST.in
--rw-rw-r--   0 akash     (1001) akash     (1001)     9151 2023-02-16 16:48:55.311907 PyJobRunner-3.9/PKG-INFO
-drwxrwxr-x   0 akash     (1001) akash     (1001)        0 2023-02-16 16:48:55.311907 PyJobRunner-3.9/PyJobRunner.egg-info/
--rw-rw-r--   0 akash     (1001) akash     (1001)     9151 2023-02-16 16:48:55.000000 PyJobRunner-3.9/PyJobRunner.egg-info/PKG-INFO
--rw-rw-r--   0 akash     (1001) akash     (1001)      603 2023-02-16 16:48:55.000000 PyJobRunner-3.9/PyJobRunner.egg-info/SOURCES.txt
--rw-rw-r--   0 akash     (1001) akash     (1001)        1 2023-02-16 16:48:55.000000 PyJobRunner-3.9/PyJobRunner.egg-info/dependency_links.txt
--rw-rw-r--   0 akash     (1001) akash     (1001)        5 2023-02-16 16:48:55.000000 PyJobRunner-3.9/PyJobRunner.egg-info/requires.txt
--rw-rw-r--   0 akash     (1001) akash     (1001)       10 2023-02-16 16:48:55.000000 PyJobRunner-3.9/PyJobRunner.egg-info/top_level.txt
--rw-rw-r--   0 akash     (1001) akash     (1001)     8878 2022-10-27 20:37:05.000000 PyJobRunner-3.9/README.rst
-drwxrwxr-x   0 akash     (1001) akash     (1001)        0 2023-02-16 16:48:55.311907 PyJobRunner-3.9/jobrunner/
--rw-rw-r--   0 akash     (1001) akash     (1001)       36 2022-10-01 15:38:33.000000 PyJobRunner-3.9/jobrunner/__init__.py
--rw-rw-r--   0 akash     (1001) akash     (1001)      271 2023-02-16 16:48:50.000000 PyJobRunner-3.9/jobrunner/__meta__.py
-drwxrwxr-x   0 akash     (1001) akash     (1001)        0 2023-02-16 16:48:55.311907 PyJobRunner-3.9/jobrunner/cli/
--rw-rw-r--   0 akash     (1001) akash     (1001)       59 2022-10-02 02:38:44.000000 PyJobRunner-3.9/jobrunner/cli/__init__.py
--rw-rw-r--   0 akash     (1001) akash     (1001)     6987 2022-12-03 07:03:43.000000 PyJobRunner-3.9/jobrunner/cli/_commands.py
--rw-rw-r--   0 akash     (1001) akash     (1001)      650 2022-11-15 18:55:48.000000 PyJobRunner-3.9/jobrunner/cli/_jobrunner.py
-drwxrwxr-x   0 akash     (1001) akash     (1001)        0 2023-02-16 16:48:55.311907 PyJobRunner-3.9/jobrunner/lib/
--rw-rw-r--   0 akash     (1001) akash     (1001)       82 2022-10-08 03:30:26.000000 PyJobRunner-3.9/jobrunner/lib/__init__.py
--rw-rw-r--   0 akash     (1001) akash     (1001)     2358 2022-10-28 15:00:25.000000 PyJobRunner-3.9/jobrunner/lib/_archivetools.py
--rw-rw-r--   0 akash     (1001) akash     (1001)     7309 2022-10-28 15:00:59.000000 PyJobRunner-3.9/jobrunner/lib/_filetools.py
--rw-rw-r--   0 akash     (1001) akash     (1001)     6459 2022-10-28 03:53:15.000000 PyJobRunner-3.9/jobrunner/lib/_parsetools.py
-drwxrwxr-x   0 akash     (1001) akash     (1001)        0 2023-02-16 16:48:55.311907 PyJobRunner-3.9/jobrunner/scripts/
--rwxr-xr-x   0 akash     (1001) akash     (1001)      591 2022-10-13 18:41:29.000000 PyJobRunner-3.9/jobrunner/scripts/catlog
--rwxr-xr-x   0 akash     (1001) akash     (1001)      387 2022-10-13 18:43:33.000000 PyJobRunner-3.9/jobrunner/scripts/catloglast
--rwxrwxr-x   0 akash     (1001) akash     (1001)      143 2022-10-27 20:50:46.000000 PyJobRunner-3.9/jobrunner/scripts/jobrunner
--rwxr-xr-x   0 akash     (1001) akash     (1001)     1101 2022-10-27 20:51:52.000000 PyJobRunner-3.9/jobrunner/scripts/logdiff
-drwxrwxr-x   0 akash     (1001) akash     (1001)        0 2023-02-16 16:48:55.311907 PyJobRunner-3.9/media/
--rw-r--r--   0 akash     (1001) akash     (1001)     2312 2022-10-14 05:48:54.000000 PyJobRunner-3.9/media/icon.svg
--rw-rw-r--   0 akash     (1001) akash     (1001)       38 2023-02-16 16:48:55.311907 PyJobRunner-3.9/setup.cfg
--rw-rw-r--   0 akash     (1001) akash     (1001)     1377 2022-10-15 02:46:24.000000 PyJobRunner-3.9/setup.py
+drwxrwxr-x   0 akash     (1001) akash     (1001)        0 2023-02-16 23:47:06.895737 PyJobRunner-4.0/
+-rw-rw-r--   0 akash     (1001) akash     (1001)     1068 2022-10-04 16:17:57.000000 PyJobRunner-4.0/LICENSE
+-rw-rw-r--   0 akash     (1001) akash     (1001)       51 2022-10-19 20:21:58.000000 PyJobRunner-4.0/MANIFEST.in
+-rw-rw-r--   0 akash     (1001) akash     (1001)     9151 2023-02-16 23:47:06.895737 PyJobRunner-4.0/PKG-INFO
+drwxrwxr-x   0 akash     (1001) akash     (1001)        0 2023-02-16 23:47:06.895737 PyJobRunner-4.0/PyJobRunner.egg-info/
+-rw-rw-r--   0 akash     (1001) akash     (1001)     9151 2023-02-16 23:47:06.000000 PyJobRunner-4.0/PyJobRunner.egg-info/PKG-INFO
+-rw-rw-r--   0 akash     (1001) akash     (1001)      603 2023-02-16 23:47:06.000000 PyJobRunner-4.0/PyJobRunner.egg-info/SOURCES.txt
+-rw-rw-r--   0 akash     (1001) akash     (1001)        1 2023-02-16 23:47:06.000000 PyJobRunner-4.0/PyJobRunner.egg-info/dependency_links.txt
+-rw-rw-r--   0 akash     (1001) akash     (1001)       12 2023-02-16 23:47:06.000000 PyJobRunner-4.0/PyJobRunner.egg-info/requires.txt
+-rw-rw-r--   0 akash     (1001) akash     (1001)       10 2023-02-16 23:47:06.000000 PyJobRunner-4.0/PyJobRunner.egg-info/top_level.txt
+-rw-rw-r--   0 akash     (1001) akash     (1001)     8878 2022-10-27 20:37:05.000000 PyJobRunner-4.0/README.rst
+drwxrwxr-x   0 akash     (1001) akash     (1001)        0 2023-02-16 23:47:06.895737 PyJobRunner-4.0/jobrunner/
+-rw-rw-r--   0 akash     (1001) akash     (1001)       36 2022-10-01 15:38:33.000000 PyJobRunner-4.0/jobrunner/__init__.py
+-rw-rw-r--   0 akash     (1001) akash     (1001)      271 2023-02-16 23:46:59.000000 PyJobRunner-4.0/jobrunner/__meta__.py
+drwxrwxr-x   0 akash     (1001) akash     (1001)        0 2023-02-16 23:47:06.895737 PyJobRunner-4.0/jobrunner/cli/
+-rw-rw-r--   0 akash     (1001) akash     (1001)       59 2022-10-02 02:38:44.000000 PyJobRunner-4.0/jobrunner/cli/__init__.py
+-rw-rw-r--   0 akash     (1001) akash     (1001)     6987 2022-12-03 07:03:43.000000 PyJobRunner-4.0/jobrunner/cli/_commands.py
+-rw-rw-r--   0 akash     (1001) akash     (1001)      650 2022-11-15 18:55:48.000000 PyJobRunner-4.0/jobrunner/cli/_jobrunner.py
+drwxrwxr-x   0 akash     (1001) akash     (1001)        0 2023-02-16 23:47:06.895737 PyJobRunner-4.0/jobrunner/lib/
+-rw-rw-r--   0 akash     (1001) akash     (1001)       82 2022-10-08 03:30:26.000000 PyJobRunner-4.0/jobrunner/lib/__init__.py
+-rw-rw-r--   0 akash     (1001) akash     (1001)     2358 2022-10-28 15:00:25.000000 PyJobRunner-4.0/jobrunner/lib/_archivetools.py
+-rw-rw-r--   0 akash     (1001) akash     (1001)     7309 2022-10-28 15:00:59.000000 PyJobRunner-4.0/jobrunner/lib/_filetools.py
+-rw-rw-r--   0 akash     (1001) akash     (1001)     7558 2023-02-16 17:44:49.000000 PyJobRunner-4.0/jobrunner/lib/_parsetools.py
+drwxrwxr-x   0 akash     (1001) akash     (1001)        0 2023-02-16 23:47:06.895737 PyJobRunner-4.0/jobrunner/scripts/
+-rwxr-xr-x   0 akash     (1001) akash     (1001)      591 2022-10-13 18:41:29.000000 PyJobRunner-4.0/jobrunner/scripts/catlog
+-rwxr-xr-x   0 akash     (1001) akash     (1001)      387 2022-10-13 18:43:33.000000 PyJobRunner-4.0/jobrunner/scripts/catloglast
+-rwxrwxr-x   0 akash     (1001) akash     (1001)      143 2022-10-27 20:50:46.000000 PyJobRunner-4.0/jobrunner/scripts/jobrunner
+-rwxr-xr-x   0 akash     (1001) akash     (1001)     1101 2022-10-27 20:51:52.000000 PyJobRunner-4.0/jobrunner/scripts/logdiff
+drwxrwxr-x   0 akash     (1001) akash     (1001)        0 2023-02-16 23:47:06.895737 PyJobRunner-4.0/media/
+-rw-r--r--   0 akash     (1001) akash     (1001)     2312 2022-10-14 05:48:54.000000 PyJobRunner-4.0/media/icon.svg
+-rw-rw-r--   0 akash     (1001) akash     (1001)       38 2023-02-16 23:47:06.895737 PyJobRunner-4.0/setup.cfg
+-rw-rw-r--   0 akash     (1001) akash     (1001)     1387 2023-02-16 17:42:17.000000 PyJobRunner-4.0/setup.py
```

### Comparing `PyJobRunner-3.9/LICENSE` & `PyJobRunner-4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `PyJobRunner-3.9/PKG-INFO` & `PyJobRunner-4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyJobRunner
-Version: 3.9
+Version: 4.0
 Summary: Job runner for scientific computing workloads
 Author: Akash Dhruv
 License: MIT License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: MIT License
 License-File: LICENSE
```

### Comparing `PyJobRunner-3.9/PyJobRunner.egg-info/PKG-INFO` & `PyJobRunner-4.0/PyJobRunner.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyJobRunner
-Version: 3.9
+Version: 4.0
 Summary: Job runner for scientific computing workloads
 Author: Akash Dhruv
 License: MIT License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: MIT License
 License-File: LICENSE
```

### Comparing `PyJobRunner-3.9/PyJobRunner.egg-info/SOURCES.txt` & `PyJobRunner-4.0/PyJobRunner.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PyJobRunner-3.9/README.rst` & `PyJobRunner-4.0/README.rst`

 * *Files identical despite different names*

### Comparing `PyJobRunner-3.9/jobrunner/cli/_commands.py` & `PyJobRunner-4.0/jobrunner/cli/_commands.py`

 * *Files identical despite different names*

### Comparing `PyJobRunner-3.9/jobrunner/cli/_jobrunner.py` & `PyJobRunner-4.0/jobrunner/cli/_jobrunner.py`

 * *Files identical despite different names*

### Comparing `PyJobRunner-3.9/jobrunner/lib/_archivetools.py` & `PyJobRunner-4.0/jobrunner/lib/_archivetools.py`

 * *Files identical despite different names*

### Comparing `PyJobRunner-3.9/jobrunner/lib/_filetools.py` & `PyJobRunner-4.0/jobrunner/lib/_filetools.py`

 * *Files identical despite different names*

### Comparing `PyJobRunner-3.9/jobrunner/lib/_parsetools.py` & `PyJobRunner-4.0/jobrunner/lib/_parsetools.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,13 +1,40 @@
 # Standard libraries
 import os
 import glob
 
 # Feature libraries
 import toml
+import yaml
+
+
+class __YamlLoader(yaml.SafeLoader):
+    """
+    Class YamlLoader for YAML
+    """
+
+    def __init__(self, stream):
+        """
+        Constructor
+        """
+        super().__init__(stream)
+        self._stream = stream
+
+    def construct_mapping(self, node, deep=False):
+        """
+        Mapping function
+        """
+        mapping = set()
+        for key_node, value_node in node.value:
+            key = self.construct_object(key_node, deep=deep)
+            if key in mapping:
+                print(f"ERROR:   Duplicate {key!r} key found in {self._stream.name!r}.")
+                raise ValueError()
+            mapping.add(key)
+        return super().construct_mapping(node, deep)
 
 
 def ParseJobConfig(basedir, workdir):
     """
     basedir : base directory
     workdir : work directory
     """
@@ -37,16 +64,29 @@
             "workdir": workdir,
         },
     }
 
     # loop over individual files
     for jobfile in jobfile_list:
 
-        # load the toml file
-        work_dict = toml.load(jobfile)
+        # load the job configuration
+        # both toml and yaml formats
+        # supported
+        #
+        # try toml load
+        try:
+            work_dict = toml.load(jobfile)
+        #
+        # if error try yaml load
+        except:
+            with open(jobfile, "r") as stream:
+                try:
+                    work_dict = yaml.load(stream, Loader=__YamlLoader)
+                except yaml.YAMLError as exc:
+                    print(exc)
 
         # loop over keys in work_dict, parse
         # configuration and handle exceptions
         for key in work_dict:
 
             # loop over subkey and values
             for subkey, work_obj in work_dict[key].items():
```

### Comparing `PyJobRunner-3.9/jobrunner/scripts/catlog` & `PyJobRunner-4.0/jobrunner/scripts/catlog`

 * *Files identical despite different names*

### Comparing `PyJobRunner-3.9/jobrunner/scripts/logdiff` & `PyJobRunner-4.0/jobrunner/scripts/logdiff`

 * *Files identical despite different names*

### Comparing `PyJobRunner-3.9/media/icon.svg` & `PyJobRunner-4.0/media/icon.svg`

 * *Files identical despite different names*

### Comparing `PyJobRunner-3.9/setup.py` & `PyJobRunner-4.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
             "__authors__",
             "__license__",
             "__description__",
         ]
     }
 
 # core dependancies
-DEPENDENCIES = ["toml"]
+DEPENDENCIES = ["toml", "pyyaml"]
 
 setup(
     name=metadata["__pkgname__"],
     version=metadata["__version__"],
     author=metadata["__authors__"],
     description=metadata["__description__"],
     license=metadata["__license__"],
```

