# Comparing `tmp/pandas_flavor-0.5.0.tar.gz` & `tmp/pandas_flavor-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pandas_flavor-0.5.0.tar", last modified: Fri Feb  3 16:36:14 2023, max compression
+gzip compressed data, was "pandas_flavor-0.6.0.tar", last modified: Sat Jul  8 19:14:53 2023, max compression
```

## Comparing `pandas_flavor-0.5.0.tar` & `pandas_flavor-0.6.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 16:36:14.552210 pandas_flavor-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-02-03 16:36:08.000000 pandas_flavor-0.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-02-03 16:36:08.000000 pandas_flavor-0.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5802 2023-02-03 16:36:14.548210 pandas_flavor-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4923 2023-02-03 16:36:08.000000 pandas_flavor-0.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 16:36:14.548210 pandas_flavor-0.5.0/pandas_flavor/
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-02-03 16:36:08.000000 pandas_flavor-0.5.0/pandas_flavor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-02-03 16:36:13.000000 pandas_flavor-0.5.0/pandas_flavor/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6823 2023-02-03 16:36:08.000000 pandas_flavor-0.5.0/pandas_flavor/register.py
--rw-r--r--   0 runner    (1001) docker     (123)     1927 2023-02-03 16:36:08.000000 pandas_flavor-0.5.0/pandas_flavor/xarray.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 16:36:14.548210 pandas_flavor-0.5.0/pandas_flavor.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5802 2023-02-03 16:36:14.000000 pandas_flavor-0.5.0/pandas_flavor.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-02-03 16:36:14.000000 pandas_flavor-0.5.0/pandas_flavor.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-03 16:36:14.000000 pandas_flavor-0.5.0/pandas_flavor.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-02-03 16:36:14.000000 pandas_flavor-0.5.0/pandas_flavor.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-02-03 16:36:14.000000 pandas_flavor-0.5.0/pandas_flavor.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-02-03 16:36:08.000000 pandas_flavor-0.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-03 16:36:14.552210 pandas_flavor-0.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3371 2023-02-03 16:36:08.000000 pandas_flavor-0.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 19:14:53.411992 pandas_flavor-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-07-08 19:14:47.000000 pandas_flavor-0.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-08 19:14:47.000000 pandas_flavor-0.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6267 2023-07-08 19:14:53.411992 pandas_flavor-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5388 2023-07-08 19:14:47.000000 pandas_flavor-0.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 19:14:53.411992 pandas_flavor-0.6.0/pandas_flavor/
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-07-08 19:14:47.000000 pandas_flavor-0.6.0/pandas_flavor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-08 19:14:51.000000 pandas_flavor-0.6.0/pandas_flavor/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7219 2023-07-08 19:14:47.000000 pandas_flavor-0.6.0/pandas_flavor/register.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1927 2023-07-08 19:14:47.000000 pandas_flavor-0.6.0/pandas_flavor/xarray.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 19:14:53.411992 pandas_flavor-0.6.0/pandas_flavor.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6267 2023-07-08 19:14:53.000000 pandas_flavor-0.6.0/pandas_flavor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-07-08 19:14:53.000000 pandas_flavor-0.6.0/pandas_flavor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 19:14:53.000000 pandas_flavor-0.6.0/pandas_flavor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-08 19:14:53.000000 pandas_flavor-0.6.0/pandas_flavor.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-08 19:14:53.000000 pandas_flavor-0.6.0/pandas_flavor.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-07-08 19:14:47.000000 pandas_flavor-0.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 19:14:53.411992 pandas_flavor-0.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3344 2023-07-08 19:14:47.000000 pandas_flavor-0.6.0/setup.py
```

### Comparing `pandas_flavor-0.5.0/LICENSE` & `pandas_flavor-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pandas_flavor-0.5.0/PKG-INFO` & `pandas_flavor-0.6.0/pandas_flavor.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: pandas_flavor
-Version: 0.5.0
+Name: pandas-flavor
+Version: 0.6.0
 Summary: The easy way to write your own Pandas flavor.
 Home-page: https://github.com/Zsailer/pandas_flavor
 Author: Zach Sailer
 Author-email: zachsailer@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -140,14 +140,20 @@
 df.row_by_value('x', 10)
 
 # x    10
 # y     0
 # Name: 0, dtype: int64
 ```
 
+## Registered methods tracing
+
+The pandas_flavor 0.5.0 release introduced [tracing of the registered method calls](/docs/tracing_ext.md). Now it is possible to add additional run-time logic around registered method execution which can be used for some support tasks. This extension was introduced
+to allow visualization of [pyjanitor](https://github.com/pyjanitor-devs/pyjanitor) method chains as implemented in [pyjviz](https://github.com/pyjanitor-devs/pyjviz)
+
+
 ## Available Methods
 
 - **register_dataframe_method**: register a method directly with a pandas DataFrame.
 - **register_dataframe_accessor**: register an accessor (and it's methods) with a pandas DataFrame.
 - **register_series_method**: register a methods directly with a pandas Series.
 - **register_series_accessor**: register an accessor (and it's methods) with a pandas Series.
```

### Comparing `pandas_flavor-0.5.0/README.md` & `pandas_flavor-0.6.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -117,14 +117,20 @@
 df.row_by_value('x', 10)
 
 # x    10
 # y     0
 # Name: 0, dtype: int64
 ```
 
+## Registered methods tracing
+
+The pandas_flavor 0.5.0 release introduced [tracing of the registered method calls](/docs/tracing_ext.md). Now it is possible to add additional run-time logic around registered method execution which can be used for some support tasks. This extension was introduced
+to allow visualization of [pyjanitor](https://github.com/pyjanitor-devs/pyjanitor) method chains as implemented in [pyjviz](https://github.com/pyjanitor-devs/pyjviz)
+
+
 ## Available Methods
 
 - **register_dataframe_method**: register a method directly with a pandas DataFrame.
 - **register_dataframe_accessor**: register an accessor (and it's methods) with a pandas DataFrame.
 - **register_series_method**: register a methods directly with a pandas Series.
 - **register_series_accessor**: register an accessor (and it's methods) with a pandas Series.
```

### Comparing `pandas_flavor-0.5.0/pandas_flavor/register.py` & `pandas_flavor-0.6.0/pandas_flavor/register.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+"""Register functions as methods of Pandas DataFrame and Series."""
 from functools import wraps
 from pandas.api.extensions import (
     register_series_accessor,
     register_dataframe_accessor,
 )
 import inspect
 
@@ -75,15 +76,18 @@
     with method_call_ctx_factory(
         method.__name__, args, kwargs
     ) as method_call_ctx:
         if method_call_ctx is None:  # nullcontext __enter__ returns None
             ret = method(obj, *args, **kwargs)
         else:
             all_args = tuple([obj] + list(args))
-            (new_args, new_kwargs,) = method_call_ctx.handle_start_method_call(
+            (
+                new_args,
+                new_kwargs,
+            ) = method_call_ctx.handle_start_method_call(
                 method.__name__, method_signature, all_args, kwargs
             )
             args = new_args[1:]
             kwargs = new_kwargs
 
             ret = method(obj, *args, **kwargs)
 
@@ -172,14 +176,24 @@
     Returns:
         callable: The original method.
     """
 
     method_signature = inspect.signature(method)
 
     def inner(*args, **kwargs):
+        """Inner function to register the method.
+
+        Args:
+            *args: The arguments to pass to the registered method.
+            **kwargs: The keyword arguments to pass to the registered method.
+
+        Returns:
+            method: The original method.
+        """
+
         class AccessorMethod(object):
             """Series Accessor method class."""
 
             __doc__ = method.__doc__
 
             def __init__(self, pandas_obj):
                 """Initialize the accessor method class.
```

### Comparing `pandas_flavor-0.5.0/pandas_flavor/xarray.py` & `pandas_flavor-0.6.0/pandas_flavor/xarray.py`

 * *Files identical despite different names*

### Comparing `pandas_flavor-0.5.0/pandas_flavor.egg-info/PKG-INFO` & `pandas_flavor-0.6.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: pandas-flavor
-Version: 0.5.0
+Name: pandas_flavor
+Version: 0.6.0
 Summary: The easy way to write your own Pandas flavor.
 Home-page: https://github.com/Zsailer/pandas_flavor
 Author: Zach Sailer
 Author-email: zachsailer@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -140,14 +140,20 @@
 df.row_by_value('x', 10)
 
 # x    10
 # y     0
 # Name: 0, dtype: int64
 ```
 
+## Registered methods tracing
+
+The pandas_flavor 0.5.0 release introduced [tracing of the registered method calls](/docs/tracing_ext.md). Now it is possible to add additional run-time logic around registered method execution which can be used for some support tasks. This extension was introduced
+to allow visualization of [pyjanitor](https://github.com/pyjanitor-devs/pyjanitor) method chains as implemented in [pyjviz](https://github.com/pyjanitor-devs/pyjviz)
+
+
 ## Available Methods
 
 - **register_dataframe_method**: register a method directly with a pandas DataFrame.
 - **register_dataframe_accessor**: register an accessor (and it's methods) with a pandas DataFrame.
 - **register_series_method**: register a methods directly with a pandas Series.
 - **register_series_accessor**: register an accessor (and it's methods) with a pandas Series.
```

### Comparing `pandas_flavor-0.5.0/setup.py` & `pandas_flavor-0.6.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,8 @@
-#!/usr/bin/env python
-# -*- coding: utf-8 -*-
-
-# Note: To use the 'upload' functionality of this file, you must:
-#   $ pip install twine
-
+"""Setup script."""
 import io
 import os
 import sys
 from shutil import rmtree
 
 from setuptools import find_packages, setup, Command
 
@@ -15,15 +10,15 @@
 NAME = "pandas_flavor"
 DESCRIPTION = "The easy way to write your own Pandas flavor."
 URL = "https://github.com/Zsailer/pandas_flavor"
 EMAIL = "zachsailer@gmail.com"
 AUTHOR = "Zach Sailer"
 
 # What packages are required for this module to be executed?
-REQUIRED = ["pandas>=0.23", "xarray", "lazy-loader>=0.1"]
+REQUIRED = ["pandas>=0.23", "xarray"]
 
 # The rest you shouldn't have to touch too much :)
 # ------------------------------------------------
 # Except, perhaps the License and Trove Classifiers!
 # If you do change the License,
 # remember to change the Trove Classifier for that!
 
@@ -54,20 +49,23 @@
         Args:
             s: The string to print.
 
         """
         print("\033[1m{0}\033[0m".format(s))
 
     def initialize_options(self):
+        """Initialize options."""
         pass
 
     def finalize_options(self):
+        """Finalize options."""
         pass
 
     def run(self):
+        """Build and publish the package."""
         try:
             self.status("Removing previous builds…")
             rmtree(os.path.join(here, "dist"))
         except OSError:
             pass
 
         self.status("Building Source and Wheel (universal) distribution…")
```

