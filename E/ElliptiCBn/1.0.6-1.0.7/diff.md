# Comparing `tmp/ElliptiCBn-1.0.6.tar.gz` & `tmp/ElliptiCBn-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ElliptiCBn-1.0.6.tar", last modified: Fri Jul  7 23:19:48 2023, max compression
+gzip compressed data, was "ElliptiCBn-1.0.7.tar", last modified: Fri Jul  7 23:30:46 2023, max compression
```

## Comparing `ElliptiCBn-1.0.6.tar` & `ElliptiCBn-1.0.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-07-07 23:19:48.483373 ElliptiCBn-1.0.6/
-drwxrwxrwx   0        0        0        0 2023-07-07 23:19:48.463778 ElliptiCBn-1.0.6/ElliptiC/
--rw-rw-rw-   0        0        0    27466 2023-06-28 19:43:33.000000 ElliptiCBn-1.0.6/ElliptiC/ElliptiC.py
--rw-rw-rw-   0        0        0       30 2023-06-28 19:22:14.000000 ElliptiCBn-1.0.6/ElliptiC/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-07 23:19:48.481438 ElliptiCBn-1.0.6/ElliptiCBn.egg-info/
--rw-rw-rw-   0        0        0     4719 2023-07-07 23:19:48.000000 ElliptiCBn-1.0.6/ElliptiCBn.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      265 2023-07-07 23:19:48.000000 ElliptiCBn-1.0.6/ElliptiCBn.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-07 23:19:48.000000 ElliptiCBn-1.0.6/ElliptiCBn.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       82 2023-07-07 23:19:48.000000 ElliptiCBn-1.0.6/ElliptiCBn.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-07-07 23:19:48.000000 ElliptiCBn-1.0.6/ElliptiCBn.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1108 2023-06-23 18:27:33.000000 ElliptiCBn-1.0.6/LICENSE
--rw-rw-rw-   0        0        0     4719 2023-07-07 23:19:48.483373 ElliptiCBn-1.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     3947 2023-07-07 22:24:48.000000 ElliptiCBn-1.0.6/README.md
-drwxrwxrwx   0        0        0        0 2023-07-07 23:19:48.482373 ElliptiCBn-1.0.6/bin/
--rw-rw-rw-   0        0        0      899 2023-07-07 18:41:14.000000 ElliptiCBn-1.0.6/bin/ElliptiC
--rw-rw-rw-   0        0        0      905 2023-07-07 23:19:04.000000 ElliptiCBn-1.0.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-07 23:19:48.483373 ElliptiCBn-1.0.6/setup.cfg
--rw-rw-rw-   0        0        0     1340 2023-07-07 23:19:18.000000 ElliptiCBn-1.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-07 23:30:46.489584 ElliptiCBn-1.0.7/
+drwxrwxrwx   0        0        0        0 2023-07-07 23:30:46.467394 ElliptiCBn-1.0.7/ElliptiC/
+-rw-rw-rw-   0        0        0    27466 2023-06-28 19:43:33.000000 ElliptiCBn-1.0.7/ElliptiC/ElliptiC.py
+-rw-rw-rw-   0        0        0       30 2023-06-28 19:22:14.000000 ElliptiCBn-1.0.7/ElliptiC/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-07 23:30:46.486993 ElliptiCBn-1.0.7/ElliptiCBn.egg-info/
+-rw-rw-rw-   0        0        0     4741 2023-07-07 23:30:46.000000 ElliptiCBn-1.0.7/ElliptiCBn.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      265 2023-07-07 23:30:46.000000 ElliptiCBn-1.0.7/ElliptiCBn.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-07 23:30:46.000000 ElliptiCBn-1.0.7/ElliptiCBn.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       99 2023-07-07 23:30:46.000000 ElliptiCBn-1.0.7/ElliptiCBn.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-07 23:30:46.000000 ElliptiCBn-1.0.7/ElliptiCBn.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1108 2023-06-23 18:27:33.000000 ElliptiCBn-1.0.7/LICENSE
+-rw-rw-rw-   0        0        0     4741 2023-07-07 23:30:46.488575 ElliptiCBn-1.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     3947 2023-07-07 22:24:48.000000 ElliptiCBn-1.0.7/README.md
+drwxrwxrwx   0        0        0        0 2023-07-07 23:30:46.488020 ElliptiCBn-1.0.7/bin/
+-rw-rw-rw-   0        0        0      899 2023-07-07 18:41:14.000000 ElliptiCBn-1.0.7/bin/ElliptiC
+-rw-rw-rw-   0        0        0      960 2023-07-07 23:29:50.000000 ElliptiCBn-1.0.7/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-07 23:30:46.489584 ElliptiCBn-1.0.7/setup.cfg
+-rw-rw-rw-   0        0        0     1340 2023-07-07 23:30:01.000000 ElliptiCBn-1.0.7/setup.py
```

### Comparing `ElliptiCBn-1.0.6/ElliptiC/ElliptiC.py` & `ElliptiCBn-1.0.7/ElliptiC/ElliptiC.py`

 * *Files identical despite different names*

### Comparing `ElliptiCBn-1.0.6/ElliptiCBn.egg-info/PKG-INFO` & `ElliptiCBn-1.0.7/ElliptiCBn.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ElliptiCBn
-Version: 1.0.6
+Version: 1.0.7
 Summary: Python package for analyzing Cucurbituril crystal structures automatically
 Home-page: https://github.com/harmslab/ElliptiC
 Author: Michael Shavlik
 Author-email: Michael Shavlik <mshavlik@uoregon.edu>
 License: MIT
 Project-URL: Homepage, https://github.com/harmslab/ElliptiC
 Keywords: CBn; Crystal structure
@@ -12,14 +12,15 @@
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
+Provides-Extra: test
 License-File: LICENSE
 
 # ElliptiC - an automated command line tool for visualizing and measuring ellipticity of cucurbituril host/guest structures
 
 <br />
```

### Comparing `ElliptiCBn-1.0.6/LICENSE` & `ElliptiCBn-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `ElliptiCBn-1.0.6/PKG-INFO` & `ElliptiCBn-1.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ElliptiCBn
-Version: 1.0.6
+Version: 1.0.7
 Summary: Python package for analyzing Cucurbituril crystal structures automatically
 Home-page: https://github.com/harmslab/ElliptiC
 Author: Michael Shavlik
 Author-email: Michael Shavlik <mshavlik@uoregon.edu>
 License: MIT
 Project-URL: Homepage, https://github.com/harmslab/ElliptiC
 Keywords: CBn; Crystal structure
@@ -12,14 +12,15 @@
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
+Provides-Extra: test
 License-File: LICENSE
 
 # ElliptiC - an automated command line tool for visualizing and measuring ellipticity of cucurbituril host/guest structures
 
 <br />
```

### Comparing `ElliptiCBn-1.0.6/README.md` & `ElliptiCBn-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `ElliptiCBn-1.0.6/bin/ElliptiC` & `ElliptiCBn-1.0.7/bin/ElliptiC`

 * *Files identical despite different names*

### Comparing `ElliptiCBn-1.0.6/pyproject.toml` & `ElliptiCBn-1.0.7/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "ElliptiCBn"
-version = "1.0.6"
+version = "1.0.7"
 authors = [{name="Michael Shavlik", email="mshavlik@uoregon.edu"}]
 description = "Python package for analyzing Cucurbituril crystal structures automatically"
 readme = "README.md"
 requires-python = ">=3.7.0"
 classifiers = [
                   "Development Status :: 3 - Alpha",
                   "Intended Audience :: Science/Research",
@@ -25,10 +25,14 @@
 "scikit-learn",
 "plotly",
 "pandas",
 "matplotlib",
 "xlsxwriter",
 ]
 
+[project.optional-dependencies]
+test = ["openpyxl",
+]
+
 [project.urls]
 "Homepage" = "https://github.com/harmslab/ElliptiC"
```

### Comparing `ElliptiCBn-1.0.6/setup.py` & `ElliptiCBn-1.0.7/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,27 +12,27 @@
 #Package meta-data
 DESCRIPTION= \
 """ Python package for analyzing CBn crystal structures automatically. """
 URL = "https://github.com/harmslab/ElliptiC"  # temp URL
 EMAIL = "mshavlik@uoregon.edu"
 AUTHOR = "Michael Shavlik"
 REQUIRES_PYTHON = ">=3.7.0"
-VERSION = "1.0.6"
+VERSION = "1.0.7"
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 # Import README for description
 with io.open(os.path.join(here,'README.md'),encoding='utf-8') as f:
     full_description = '\n' + f.read()
 
     
 # Now the part where we do setup
 setup(
     name='ElliptiCBn',
-    version='1.0.6',
+    version='1.0.7',
     author=AUTHOR,
     author_email=EMAIL,
     description=DESCRIPTION,
     long_description=full_description,
     url=URL,
     license='MIT',
     packages=['ElliptiC'],
```

