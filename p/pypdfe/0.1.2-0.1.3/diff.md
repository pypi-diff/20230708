# Comparing `tmp/pypdfe-0.1.2.tar.gz` & `tmp/pypdfe-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypdfe-0.1.2.tar", last modified: Sat Jul  8 18:38:19 2023, max compression
+gzip compressed data, was "pypdfe-0.1.3.tar", last modified: Sat Jul  8 18:52:02 2023, max compression
```

## Comparing `pypdfe-0.1.2.tar` & `pypdfe-0.1.3.tar`

### file list

```diff
@@ -1,15 +1,43 @@
-drwxr-xr-x   0 nate       (501) staff       (20)        0 2023-07-08 18:38:19.847067 pypdfe-0.1.2/
--rw-r--r--   0 nate       (501) staff       (20)    35148 2023-07-08 07:31:18.000000 pypdfe-0.1.2/LICENSE
--rw-r--r--   0 nate       (501) staff       (20)      297 2023-07-08 18:38:19.846976 pypdfe-0.1.2/PKG-INFO
-drwxr-xr-x   0 nate       (501) staff       (20)        0 2023-07-08 18:38:19.846098 pypdfe-0.1.2/pypdfe/
--rw-r--r--   0 nate       (501) staff       (20)     1025 2023-07-08 07:18:43.000000 pypdfe-0.1.2/pypdfe/__init__.py
-drwxr-xr-x   0 nate       (501) staff       (20)        0 2023-07-08 18:38:19.846818 pypdfe-0.1.2/pypdfe.egg-info/
--rw-r--r--   0 nate       (501) staff       (20)      297 2023-07-08 18:38:19.000000 pypdfe-0.1.2/pypdfe.egg-info/PKG-INFO
--rw-r--r--   0 nate       (501) staff       (20)     1532 2023-07-08 18:38:19.000000 pypdfe-0.1.2/pypdfe.egg-info/SOURCES.txt
--rw-r--r--   0 nate       (501) staff       (20)        1 2023-07-08 18:38:19.000000 pypdfe-0.1.2/pypdfe.egg-info/dependency_links.txt
--rw-r--r--   0 nate       (501) staff       (20)        1 2023-07-08 18:38:19.000000 pypdfe-0.1.2/pypdfe.egg-info/not-zip-safe
--rw-r--r--   0 nate       (501) staff       (20)       26 2023-07-08 18:38:19.000000 pypdfe-0.1.2/pypdfe.egg-info/requires.txt
--rw-r--r--   0 nate       (501) staff       (20)        7 2023-07-08 18:38:19.000000 pypdfe-0.1.2/pypdfe.egg-info/top_level.txt
--rw-r--r--   0 nate       (501) staff       (20)      143 2023-07-08 18:37:36.000000 pypdfe-0.1.2/pyproject.toml
--rw-r--r--   0 nate       (501) staff       (20)       38 2023-07-08 18:38:19.847100 pypdfe-0.1.2/setup.cfg
--rw-r--r--   0 nate       (501) staff       (20)     1642 2023-07-08 18:37:36.000000 pypdfe-0.1.2/setup.py
+drwxr-xr-x   0 nate       (501) staff       (20)        0 2023-07-08 18:52:02.896220 pypdfe-0.1.3/
+-rw-r--r--   0 nate       (501) staff       (20)    35148 2023-07-08 07:31:18.000000 pypdfe-0.1.3/LICENSE
+-rw-r--r--   0 nate       (501) staff       (20)      297 2023-07-08 18:52:02.896106 pypdfe-0.1.3/PKG-INFO
+drwxr-xr-x   0 nate       (501) staff       (20)        0 2023-07-08 18:52:02.891801 pypdfe-0.1.3/pypdfe/
+-rw-r--r--   0 nate       (501) staff       (20)     1025 2023-07-08 07:18:43.000000 pypdfe-0.1.3/pypdfe/__init__.py
+drwxr-xr-x   0 nate       (501) staff       (20)        0 2023-07-08 18:52:02.892489 pypdfe-0.1.3/pypdfe.egg-info/
+-rw-r--r--   0 nate       (501) staff       (20)      297 2023-07-08 18:52:02.000000 pypdfe-0.1.3/pypdfe.egg-info/PKG-INFO
+-rw-r--r--   0 nate       (501) staff       (20)     2604 2023-07-08 18:52:02.000000 pypdfe-0.1.3/pypdfe.egg-info/SOURCES.txt
+-rw-r--r--   0 nate       (501) staff       (20)        1 2023-07-08 18:52:02.000000 pypdfe-0.1.3/pypdfe.egg-info/dependency_links.txt
+-rw-r--r--   0 nate       (501) staff       (20)        1 2023-07-08 18:52:02.000000 pypdfe-0.1.3/pypdfe.egg-info/not-zip-safe
+-rw-r--r--   0 nate       (501) staff       (20)       26 2023-07-08 18:52:02.000000 pypdfe-0.1.3/pypdfe.egg-info/requires.txt
+-rw-r--r--   0 nate       (501) staff       (20)        7 2023-07-08 18:52:02.000000 pypdfe-0.1.3/pypdfe.egg-info/top_level.txt
+-rw-r--r--   0 nate       (501) staff       (20)      143 2023-07-08 18:51:54.000000 pypdfe-0.1.3/pyproject.toml
+-rw-r--r--   0 nate       (501) staff       (20)       38 2023-07-08 18:52:02.896265 pypdfe-0.1.3/setup.cfg
+-rw-r--r--   0 nate       (501) staff       (20)     1765 2023-07-08 18:51:54.000000 pypdfe-0.1.3/setup.py
+drwxr-xr-x   0 nate       (501) staff       (20)        0 2023-07-08 18:52:02.892610 pypdfe-0.1.3/src/
+drwxr-xr-x   0 nate       (501) staff       (20)        0 2023-07-08 18:52:02.895940 pypdfe-0.1.3/src/PDF-Estimator/
+-rw-r--r--   0 nate       (501) staff       (20)     2947 2023-06-21 20:32:32.000000 pypdfe-0.1.3/src/PDF-Estimator/ChebyShev.cpp
+-rw-r--r--   0 nate       (501) staff       (20)     1542 2023-06-21 20:32:32.000000 pypdfe-0.1.3/src/PDF-Estimator/ChebyShev.h
+-rw-r--r--   0 nate       (501) staff       (20)     9785 2023-06-21 20:32:32.000000 pypdfe-0.1.3/src/PDF-Estimator/InputData.cpp
+-rw-r--r--   0 nate       (501) staff       (20)     2214 2023-06-21 20:32:32.000000 pypdfe-0.1.3/src/PDF-Estimator/InputData.h
+-rw-r--r--   0 nate       (501) staff       (20)     8394 2023-06-21 20:32:32.000000 pypdfe-0.1.3/src/PDF-Estimator/InputParameters.cpp
+-rw-r--r--   0 nate       (501) staff       (20)     2470 2023-06-21 20:32:32.000000 pypdfe-0.1.3/src/PDF-Estimator/InputParameters.h
+-rw-r--r--   0 nate       (501) staff       (20)     4922 2023-06-21 20:32:32.000000 pypdfe-0.1.3/src/PDF-Estimator/JointProbability.cpp
+-rw-r--r--   0 nate       (501) staff       (20)     1711 2023-06-21 20:32:32.000000 pypdfe-0.1.3/src/PDF-Estimator/JointProbability.h
+-rw-r--r--   0 nate       (501) staff       (20)    35149 2023-06-21 20:32:32.000000 pypdfe-0.1.3/src/PDF-Estimator/LICENSE
+-rw-r--r--   0 nate       (501) staff       (20)    17168 2023-06-21 20:32:32.000000 pypdfe-0.1.3/src/PDF-Estimator/MinimizeScore.cpp
+-rw-r--r--   0 nate       (501) staff       (20)     2839 2023-06-21 20:32:32.000000 pypdfe-0.1.3/src/PDF-Estimator/MinimizeScore.h
+-rw-r--r--   0 nate       (501) staff       (20)     4372 2023-06-21 20:32:32.000000 pypdfe-0.1.3/src/PDF-Estimator/OutputControl.cpp
+-rw-r--r--   0 nate       (501) staff       (20)     2028 2023-06-21 20:32:32.000000 pypdfe-0.1.3/src/PDF-Estimator/OutputControl.h
+-rw-r--r--   0 nate       (501) staff       (20)      773 2023-06-21 20:32:32.000000 pypdfe-0.1.3/src/PDF-Estimator/README.txt
+-rw-r--r--   0 nate       (501) staff       (20)     1959 2023-06-21 20:32:32.000000 pypdfe-0.1.3/src/PDF-Estimator/Score.cpp
+-rw-r--r--   0 nate       (501) staff       (20)     1857 2023-06-21 20:32:32.000000 pypdfe-0.1.3/src/PDF-Estimator/Score.h
+-rw-r--r--   0 nate       (501) staff       (20)    16156 2023-06-21 20:32:32.000000 pypdfe-0.1.3/src/PDF-Estimator/ScoreQZ.cpp
+-rw-r--r--   0 nate       (501) staff       (20)     1410 2023-06-21 20:32:32.000000 pypdfe-0.1.3/src/PDF-Estimator/ScoreQZ.h
+-rw-r--r--   0 nate       (501) staff       (20)     5467 2023-06-21 20:32:32.000000 pypdfe-0.1.3/src/PDF-Estimator/Variable.cpp
+-rw-r--r--   0 nate       (501) staff       (20)     1995 2023-06-21 20:32:32.000000 pypdfe-0.1.3/src/PDF-Estimator/Variable.h
+-rw-r--r--   0 nate       (501) staff       (20)    11691 2023-06-21 20:32:32.000000 pypdfe-0.1.3/src/PDF-Estimator/WriteResults.cpp
+-rw-r--r--   0 nate       (501) staff       (20)     2352 2023-06-21 20:32:32.000000 pypdfe-0.1.3/src/PDF-Estimator/WriteResults.h
+-rw-r--r--   0 nate       (501) staff       (20)     2407 2023-06-21 20:32:32.000000 pypdfe-0.1.3/src/PDF-Estimator/callPDF.cpp
+-rw-r--r--   0 nate       (501) staff       (20)     1007 2023-06-21 20:32:32.000000 pypdfe-0.1.3/src/PDF-Estimator/callPDF.h
+-rw-r--r--   0 nate       (501) staff       (20)     1669 2023-06-21 20:32:32.000000 pypdfe-0.1.3/src/PDF-Estimator/mvPDFMain.cpp
+-rw-r--r--   0 nate       (501) staff       (20)     1149 2023-07-08 18:51:54.000000 pypdfe-0.1.3/src/main.cpp
```

### Comparing `pypdfe-0.1.2/LICENSE` & `pypdfe-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pypdfe-0.1.2/pypdfe/__init__.py` & `pypdfe-0.1.3/pypdfe/__init__.py`

 * *Files identical despite different names*

### Comparing `pypdfe-0.1.2/pypdfe.egg-info/SOURCES.txt` & `pypdfe-0.1.3/pypdfe.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -15,8 +15,34 @@
 /Users/nate/Desktop/Research/pyPDFe_dev/setuptools_for_self_replacing/pypdfe/src/PDF-Estimator/callPDF.cpp
 pypdfe/__init__.py
 pypdfe.egg-info/PKG-INFO
 pypdfe.egg-info/SOURCES.txt
 pypdfe.egg-info/dependency_links.txt
 pypdfe.egg-info/not-zip-safe
 pypdfe.egg-info/requires.txt
-pypdfe.egg-info/top_level.txt
+pypdfe.egg-info/top_level.txt
+pypdfe/../src/main.cpp
+pypdfe/../src/PDF-Estimator/ChebyShev.cpp
+pypdfe/../src/PDF-Estimator/ChebyShev.h
+pypdfe/../src/PDF-Estimator/InputData.cpp
+pypdfe/../src/PDF-Estimator/InputData.h
+pypdfe/../src/PDF-Estimator/InputParameters.cpp
+pypdfe/../src/PDF-Estimator/InputParameters.h
+pypdfe/../src/PDF-Estimator/JointProbability.cpp
+pypdfe/../src/PDF-Estimator/JointProbability.h
+pypdfe/../src/PDF-Estimator/LICENSE
+pypdfe/../src/PDF-Estimator/MinimizeScore.cpp
+pypdfe/../src/PDF-Estimator/MinimizeScore.h
+pypdfe/../src/PDF-Estimator/OutputControl.cpp
+pypdfe/../src/PDF-Estimator/OutputControl.h
+pypdfe/../src/PDF-Estimator/README.txt
+pypdfe/../src/PDF-Estimator/Score.cpp
+pypdfe/../src/PDF-Estimator/Score.h
+pypdfe/../src/PDF-Estimator/ScoreQZ.cpp
+pypdfe/../src/PDF-Estimator/ScoreQZ.h
+pypdfe/../src/PDF-Estimator/Variable.cpp
+pypdfe/../src/PDF-Estimator/Variable.h
+pypdfe/../src/PDF-Estimator/WriteResults.cpp
+pypdfe/../src/PDF-Estimator/WriteResults.h
+pypdfe/../src/PDF-Estimator/callPDF.cpp
+pypdfe/../src/PDF-Estimator/callPDF.h
+pypdfe/../src/PDF-Estimator/mvPDFMain.cpp
```

### Comparing `pypdfe-0.1.2/setup.py` & `pypdfe-0.1.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Available at setup time due to pyproject.toml
 from pybind11.setup_helpers import Pybind11Extension, build_ext
 from setuptools import setup
 from glob import glob
 import os
 
-__version__ = "0.1.2"
+__version__ = "0.1.3"
 
 # The main interface is through Pybind11Extension.
 # * You can add cxx_std=11/14/17, and then build_ext can be removed.
 # * You can set include_pybind11=false to add the include directory yourself,
 #   say from a submodule.
 #
 # Note:
@@ -22,25 +22,27 @@
 ext_modules = [
     Pybind11Extension("pypdfe._pypdfe",
                       sources=sources,
                       depends=depends,
                       )
     ]
 
+src_files = sorted(glob(f'{os.path.dirname(os.path.realpath(__file__))}{os.sep}src{os.sep}**', recursive=True))
+
 setup(
     name="pypdfe",
     version=__version__,
     author="Nate Mauney",
     author_email="nmauney4@uncc.edu",
     url="https://github.com/CHANGE_ME",
     description="A Python package for PDF estimation using Dr. Jennifer Farmer's PDFe and multivariate PDF libraries.",
     long_description="",
     ext_modules=ext_modules,
     packages=['pypdfe'],
-    package_data={'pypdfe': ['_pypdfe.*']},
+    package_data={'pypdfe': ['_pypdfe.*']+src_files},
     cmdclass={"build_ext": build_ext},
     zip_safe=False,
     python_requires=">=3.8",
     install_requires=[
         'setuptools',
         'pybind11',
         'numpy',
```

