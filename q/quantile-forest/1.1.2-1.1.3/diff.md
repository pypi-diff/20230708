# Comparing `tmp/quantile-forest-1.1.2.tar.gz` & `tmp/quantile-forest-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quantile-forest-1.1.2.tar", last modified: Thu Mar 23 08:26:15 2023, max compression
+gzip compressed data, was "quantile-forest-1.1.3.tar", last modified: Sat Jul  8 11:46:41 2023, max compression
```

## Comparing `quantile-forest-1.1.2.tar` & `quantile-forest-1.1.3.tar`

### file list

```diff
@@ -1,54 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 08:26:15.718992 quantile-forest-1.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11341 2023-03-23 08:25:45.000000 quantile-forest-1.1.2/LICENSE
--rwxr-xr-x   0 runner    (1001) docker     (123)      146 2023-03-23 08:25:45.000000 quantile-forest-1.1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3489 2023-03-23 08:26:15.718992 quantile-forest-1.1.2/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)     2556 2023-03-23 08:25:45.000000 quantile-forest-1.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 08:26:15.714992 quantile-forest-1.1.2/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-03-23 08:25:45.000000 quantile-forest-1.1.2/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 08:26:15.710992 quantile-forest-1.1.2/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 08:26:15.714992 quantile-forest-1.1.2/docs/_static/css/
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-03-23 08:25:45.000000 quantile-forest-1.1.2/docs/_static/css/quantile-forest.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 08:26:15.714992 quantile-forest-1.1.2/docs/_static/js/
--rw-r--r--   0 runner    (1001) docker     (123)     2803 2023-03-23 08:25:45.000000 quantile-forest-1.1.2/docs/_static/js/copybutton.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 08:26:15.714992 quantile-forest-1.1.2/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-03-23 08:25:45.000000 quantile-forest-1.1.2/docs/_templates/breadcrumbs.html
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-03-23 08:25:45.000000 quantile-forest-1.1.2/docs/_templates/class.rst
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-03-23 08:25:45.000000 quantile-forest-1.1.2/docs/_templates/function.rst
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-03-23 08:25:45.000000 quantile-forest-1.1.2/docs/_templates/numpydoc_docstring.rst
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-03-23 08:25:45.000000 quantile-forest-1.1.2/docs/_templates/sidebar-search-bs.html
--rwxr-xr-x   0 runner    (1001) docker     (123)      314 2023-03-23 08:25:45.000000 quantile-forest-1.1.2/docs/api.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)     7000 2023-03-23 08:25:45.000000 quantile-forest-1.1.2/docs/conf.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      922 2023-03-23 08:25:45.000000 quantile-forest-1.1.2/docs/index.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)      912 2023-03-23 08:25:45.000000 quantile-forest-1.1.2/docs/install.rst
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-03-23 08:25:45.000000 quantile-forest-1.1.2/docs/make.bat
--rwxr-xr-x   0 runner    (1001) docker     (123)      268 2023-03-23 08:25:45.000000 quantile-forest-1.1.2/docs/refs.bib
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-03-23 08:25:45.000000 quantile-forest-1.1.2/docs/sphinx_requirements.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)    12126 2023-03-23 08:25:45.000000 quantile-forest-1.1.2/docs/user_guide.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 08:26:15.718992 quantile-forest-1.1.2/examples/
--rwxr-xr-x   0 runner    (1001) docker     (123)      101 2023-03-23 08:25:45.000000 quantile-forest-1.1.2/examples/README.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)     2878 2023-03-23 08:25:45.000000 quantile-forest-1.1.2/examples/plot_quantile_extrapolation_problem.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1865 2023-03-23 08:25:45.000000 quantile-forest-1.1.2/examples/plot_quantile_interpolation.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3961 2023-03-23 08:25:45.000000 quantile-forest-1.1.2/examples/plot_quantile_regression_intervals.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1784 2023-03-23 08:25:45.000000 quantile-forest-1.1.2/examples/plot_quantile_toy_example.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1578 2023-03-23 08:25:45.000000 quantile-forest-1.1.2/examples/plot_quantile_vs_standard_forest.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3270 2023-03-23 08:25:45.000000 quantile-forest-1.1.2/examples/plot_quantile_weighted_vs_unweighted.py
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-03-23 08:25:45.000000 quantile-forest-1.1.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 08:26:15.718992 quantile-forest-1.1.2/quantile_forest/
--rwxr-xr-x   0 runner    (1001) docker     (123)      956 2023-03-23 08:25:45.000000 quantile-forest-1.1.2/quantile_forest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-03-23 08:25:45.000000 quantile-forest-1.1.2/quantile_forest/_min_dependencies.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    51906 2023-03-23 08:25:45.000000 quantile-forest-1.1.2/quantile_forest/_quantile_forest.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1347 2023-03-23 08:25:45.000000 quantile-forest-1.1.2/quantile_forest/_quantile_forest_fast.pxd
--rwxr-xr-x   0 runner    (1001) docker     (123)    37885 2023-03-23 08:25:45.000000 quantile-forest-1.1.2/quantile_forest/_quantile_forest_fast.pyx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 08:26:15.718992 quantile-forest-1.1.2/quantile_forest/tests/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 08:25:45.000000 quantile-forest-1.1.2/quantile_forest/tests/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    43958 2023-03-23 08:25:45.000000 quantile-forest-1.1.2/quantile_forest/tests/test_quantile_forest.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-03-23 08:26:15.000000 quantile-forest-1.1.2/quantile_forest/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 08:26:15.718992 quantile-forest-1.1.2/quantile_forest.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3489 2023-03-23 08:26:15.000000 quantile-forest-1.1.2/quantile_forest.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-03-23 08:26:15.000000 quantile-forest-1.1.2/quantile_forest.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-23 08:26:15.000000 quantile-forest-1.1.2/quantile_forest.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-23 08:26:15.000000 quantile-forest-1.1.2/quantile_forest.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-03-23 08:26:15.000000 quantile-forest-1.1.2/quantile_forest.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-03-23 08:26:15.000000 quantile-forest-1.1.2/quantile_forest.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-03-23 08:26:15.722992 quantile-forest-1.1.2/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     3130 2023-03-23 08:25:45.000000 quantile-forest-1.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 11:46:41.462120 quantile-forest-1.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11341 2023-07-08 11:46:11.000000 quantile-forest-1.1.3/LICENSE
+-rwxr-xr-x   0 runner    (1001) docker     (123)      182 2023-07-08 11:46:11.000000 quantile-forest-1.1.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3566 2023-07-08 11:46:41.462120 quantile-forest-1.1.3/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2633 2023-07-08 11:46:11.000000 quantile-forest-1.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 11:46:41.454120 quantile-forest-1.1.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-07-08 11:46:11.000000 quantile-forest-1.1.3/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 11:46:41.450119 quantile-forest-1.1.3/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 11:46:41.454120 quantile-forest-1.1.3/docs/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-07-08 11:46:11.000000 quantile-forest-1.1.3/docs/_static/css/quantile-forest.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 11:46:41.454120 quantile-forest-1.1.3/docs/_static/js/
+-rw-r--r--   0 runner    (1001) docker     (123)     2803 2023-07-08 11:46:11.000000 quantile-forest-1.1.3/docs/_static/js/copybutton.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 11:46:41.458120 quantile-forest-1.1.3/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-08 11:46:11.000000 quantile-forest-1.1.3/docs/_templates/breadcrumbs.html
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-07-08 11:46:11.000000 quantile-forest-1.1.3/docs/_templates/class.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-07-08 11:46:11.000000 quantile-forest-1.1.3/docs/_templates/function.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-07-08 11:46:11.000000 quantile-forest-1.1.3/docs/_templates/numpydoc_docstring.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-07-08 11:46:11.000000 quantile-forest-1.1.3/docs/_templates/sidebar-search-bs.html
+-rwxr-xr-x   0 runner    (1001) docker     (123)      314 2023-07-08 11:46:11.000000 quantile-forest-1.1.3/docs/api.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7000 2023-07-08 11:46:11.000000 quantile-forest-1.1.3/docs/conf.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      922 2023-07-08 11:46:11.000000 quantile-forest-1.1.3/docs/index.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)      912 2023-07-08 11:46:11.000000 quantile-forest-1.1.3/docs/install.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-07-08 11:46:11.000000 quantile-forest-1.1.3/docs/make.bat
+-rwxr-xr-x   0 runner    (1001) docker     (123)      268 2023-07-08 11:46:11.000000 quantile-forest-1.1.3/docs/refs.bib
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-08 11:46:11.000000 quantile-forest-1.1.3/docs/sphinx_requirements.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12126 2023-07-08 11:46:11.000000 quantile-forest-1.1.3/docs/user_guide.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 11:46:41.458120 quantile-forest-1.1.3/examples/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      101 2023-07-08 11:46:11.000000 quantile-forest-1.1.3/examples/README.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2878 2023-07-08 11:46:11.000000 quantile-forest-1.1.3/examples/plot_quantile_extrapolation_problem.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1865 2023-07-08 11:46:11.000000 quantile-forest-1.1.3/examples/plot_quantile_interpolation.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3961 2023-07-08 11:46:11.000000 quantile-forest-1.1.3/examples/plot_quantile_regression_intervals.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1784 2023-07-08 11:46:11.000000 quantile-forest-1.1.3/examples/plot_quantile_toy_example.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1578 2023-07-08 11:46:11.000000 quantile-forest-1.1.3/examples/plot_quantile_vs_standard_forest.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3270 2023-07-08 11:46:11.000000 quantile-forest-1.1.3/examples/plot_quantile_weighted_vs_unweighted.py
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-07-08 11:46:11.000000 quantile-forest-1.1.3/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 11:46:41.458120 quantile-forest-1.1.3/quantile_forest/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      956 2023-07-08 11:46:11.000000 quantile-forest-1.1.3/quantile_forest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-07-08 11:46:11.000000 quantile-forest-1.1.3/quantile_forest/_min_dependencies.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    51906 2023-07-08 11:46:11.000000 quantile-forest-1.1.3/quantile_forest/_quantile_forest.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1347 2023-07-08 11:46:11.000000 quantile-forest-1.1.3/quantile_forest/_quantile_forest_fast.pxd
+-rwxr-xr-x   0 runner    (1001) docker     (123)    37885 2023-07-08 11:46:11.000000 quantile-forest-1.1.3/quantile_forest/_quantile_forest_fast.pyx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 11:46:41.462120 quantile-forest-1.1.3/quantile_forest/tests/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 11:46:11.000000 quantile-forest-1.1.3/quantile_forest/tests/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    43958 2023-07-08 11:46:11.000000 quantile-forest-1.1.3/quantile_forest/tests/test_quantile_forest.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-08 11:46:41.000000 quantile-forest-1.1.3/quantile_forest/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-08 11:46:11.000000 quantile-forest-1.1.3/quantile_forest/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 11:46:41.462120 quantile-forest-1.1.3/quantile_forest.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3566 2023-07-08 11:46:41.000000 quantile-forest-1.1.3/quantile_forest.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-07-08 11:46:41.000000 quantile-forest-1.1.3/quantile_forest.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 11:46:41.000000 quantile-forest-1.1.3/quantile_forest.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 11:46:41.000000 quantile-forest-1.1.3/quantile_forest.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-08 11:46:41.000000 quantile-forest-1.1.3/quantile_forest.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-08 11:46:41.000000 quantile-forest-1.1.3/quantile_forest.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-07-08 11:46:41.462120 quantile-forest-1.1.3/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3130 2023-07-08 11:46:11.000000 quantile-forest-1.1.3/setup.py
```

### Comparing `quantile-forest-1.1.2/LICENSE` & `quantile-forest-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `quantile-forest-1.1.2/PKG-INFO` & `quantile-forest-1.1.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quantile-forest
-Version: 1.1.2
+Version: 1.1.3
 Summary: scikit-learn compatible quantile forests.
 Maintainer: Zillow Group AI Team
 License: Apache License 2.0
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved
 Classifier: Programming Language :: Python
@@ -29,15 +29,15 @@
 [![GitHub Actions](https://github.com/zillow/quantile-forest/actions/workflows/build.yml/badge.svg)](https://github.com/zillow/quantile-forest/actions/workflows/build.yml)
 [![Codecov](https://codecov.io/gh/zillow/quantile-forest/branch/main/graph/badge.svg?token=STRT8T67YP)](https://codecov.io/gh/zillow/quantile-forest)
 [![Code Style black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/quantile-forest)](https://pypi.org/project/quantile-forest)
 
 **quantile-forest** offers a Python implementation of quantile regression forests compatible with scikit-learn.
 
-Quantile regression forests are a non-parametric, tree-based ensemble method for estimating conditional quantiles, with application to high-dimensional data and uncertainty estimation [[1]](#1). The estimators in this package extend the forest estimators available in scikit-learn to estimate conditional quantiles. They are compatible with and can serve as drop-in replacements for the scikit-learn variants.
+Quantile regression forests are a non-parametric, tree-based ensemble method for estimating conditional quantiles, with application to high-dimensional data and uncertainty estimation [[1]](#1). The estimators in this package extend the forest estimators available in scikit-learn to estimate conditional quantiles; they can estimate arbitrary quantiles at prediction time without retraining. They are compatible with and can serve as drop-in replacements for the scikit-learn variants.
 
 #### Example of fitted model predictions and prediction intervals on California housing data ([code](https://zillow.github.io/quantile-forest/auto_examples/plot_quantile_regression_intervals.html#sphx-glr-auto-examples-plot-quantile-regression-intervals-py))
 <img src="https://zillow.github.io/quantile-forest/_images/sphx_glr_plot_quantile_regression_intervals_001.png" height="300" />
 
 Quick Start
 -----------
```

### Comparing `quantile-forest-1.1.2/README.md` & `quantile-forest-1.1.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 [![GitHub Actions](https://github.com/zillow/quantile-forest/actions/workflows/build.yml/badge.svg)](https://github.com/zillow/quantile-forest/actions/workflows/build.yml)
 [![Codecov](https://codecov.io/gh/zillow/quantile-forest/branch/main/graph/badge.svg?token=STRT8T67YP)](https://codecov.io/gh/zillow/quantile-forest)
 [![Code Style black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/quantile-forest)](https://pypi.org/project/quantile-forest)
 
 **quantile-forest** offers a Python implementation of quantile regression forests compatible with scikit-learn.
 
-Quantile regression forests are a non-parametric, tree-based ensemble method for estimating conditional quantiles, with application to high-dimensional data and uncertainty estimation [[1]](#1). The estimators in this package extend the forest estimators available in scikit-learn to estimate conditional quantiles. They are compatible with and can serve as drop-in replacements for the scikit-learn variants.
+Quantile regression forests are a non-parametric, tree-based ensemble method for estimating conditional quantiles, with application to high-dimensional data and uncertainty estimation [[1]](#1). The estimators in this package extend the forest estimators available in scikit-learn to estimate conditional quantiles; they can estimate arbitrary quantiles at prediction time without retraining. They are compatible with and can serve as drop-in replacements for the scikit-learn variants.
 
 #### Example of fitted model predictions and prediction intervals on California housing data ([code](https://zillow.github.io/quantile-forest/auto_examples/plot_quantile_regression_intervals.html#sphx-glr-auto-examples-plot-quantile-regression-intervals-py))
 <img src="https://zillow.github.io/quantile-forest/_images/sphx_glr_plot_quantile_regression_intervals_001.png" height="300" />
 
 Quick Start
 -----------
```

### Comparing `quantile-forest-1.1.2/docs/Makefile` & `quantile-forest-1.1.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `quantile-forest-1.1.2/docs/_static/css/quantile-forest.css` & `quantile-forest-1.1.3/docs/_static/css/quantile-forest.css`

 * *Files identical despite different names*

### Comparing `quantile-forest-1.1.2/docs/_static/js/copybutton.js` & `quantile-forest-1.1.3/docs/_static/js/copybutton.js`

 * *Files identical despite different names*

### Comparing `quantile-forest-1.1.2/docs/conf.py` & `quantile-forest-1.1.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `quantile-forest-1.1.2/docs/index.rst` & `quantile-forest-1.1.3/docs/index.rst`

 * *Files identical despite different names*

### Comparing `quantile-forest-1.1.2/docs/install.rst` & `quantile-forest-1.1.3/docs/install.rst`

 * *Files identical despite different names*

### Comparing `quantile-forest-1.1.2/docs/make.bat` & `quantile-forest-1.1.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `quantile-forest-1.1.2/docs/user_guide.rst` & `quantile-forest-1.1.3/docs/user_guide.rst`

 * *Files identical despite different names*

### Comparing `quantile-forest-1.1.2/examples/plot_quantile_extrapolation_problem.py` & `quantile-forest-1.1.3/examples/plot_quantile_extrapolation_problem.py`

 * *Files identical despite different names*

### Comparing `quantile-forest-1.1.2/examples/plot_quantile_interpolation.py` & `quantile-forest-1.1.3/examples/plot_quantile_interpolation.py`

 * *Files identical despite different names*

### Comparing `quantile-forest-1.1.2/examples/plot_quantile_regression_intervals.py` & `quantile-forest-1.1.3/examples/plot_quantile_regression_intervals.py`

 * *Files identical despite different names*

### Comparing `quantile-forest-1.1.2/examples/plot_quantile_toy_example.py` & `quantile-forest-1.1.3/examples/plot_quantile_toy_example.py`

 * *Files identical despite different names*

### Comparing `quantile-forest-1.1.2/examples/plot_quantile_vs_standard_forest.py` & `quantile-forest-1.1.3/examples/plot_quantile_vs_standard_forest.py`

 * *Files identical despite different names*

### Comparing `quantile-forest-1.1.2/examples/plot_quantile_weighted_vs_unweighted.py` & `quantile-forest-1.1.3/examples/plot_quantile_weighted_vs_unweighted.py`

 * *Files identical despite different names*

### Comparing `quantile-forest-1.1.2/pyproject.toml` & `quantile-forest-1.1.3/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     "numpy>=1.23",
     "scipy>=1.4",
     "scikit-learn>=1.0",
 ]
 
 [tool.black]
 line-length = 100
-target_version = ['py38', 'py39', 'py310']
+target_version = ['py38', 'py39', 'py310', 'py311']
 preview = true
 exclude = '''
 /(
     \.eggs         # exclude a few common directories in the
   | \.git          # root of the project
   | \.mypy_cache
   | \.vscode
```

### Comparing `quantile-forest-1.1.2/quantile_forest/__init__.py` & `quantile-forest-1.1.3/quantile_forest/__init__.py`

 * *Files identical despite different names*

### Comparing `quantile-forest-1.1.2/quantile_forest/_min_dependencies.py` & `quantile-forest-1.1.3/quantile_forest/_min_dependencies.py`

 * *Files identical despite different names*

### Comparing `quantile-forest-1.1.2/quantile_forest/_quantile_forest.py` & `quantile-forest-1.1.3/quantile_forest/_quantile_forest.py`

 * *Files 0% similar despite different names*

```diff
@@ -928,15 +928,15 @@
     >>> from sklearn.datasets import make_regression
     >>> X, y = make_regression(
     ...     n_features=4, n_informative=2, random_state=0, shuffle=False)
     >>> regr = RandomForestQuantileRegressor(max_depth=2, random_state=0)
     >>> regr.fit(X, y)
     RandomForestQuantileRegressor(...)
     >>> print(regr.predict([[0, 0, 0, 0]], quantiles=0.5))
-    [-4.68693299]
+    [-3.04264873]
     """
 
     def __init__(
         self,
         n_estimators=100,
         *,
         criterion="squared_error",
```

### Comparing `quantile-forest-1.1.2/quantile_forest/_quantile_forest_fast.pxd` & `quantile-forest-1.1.3/quantile_forest/_quantile_forest_fast.pxd`

 * *Files identical despite different names*

### Comparing `quantile-forest-1.1.2/quantile_forest/_quantile_forest_fast.pyx` & `quantile-forest-1.1.3/quantile_forest/_quantile_forest_fast.pyx`

 * *Files identical despite different names*

### Comparing `quantile-forest-1.1.2/quantile_forest/tests/test_quantile_forest.py` & `quantile-forest-1.1.3/quantile_forest/tests/test_quantile_forest.py`

 * *Files identical despite different names*

### Comparing `quantile-forest-1.1.2/quantile_forest.egg-info/PKG-INFO` & `quantile-forest-1.1.3/quantile_forest.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quantile-forest
-Version: 1.1.2
+Version: 1.1.3
 Summary: scikit-learn compatible quantile forests.
 Maintainer: Zillow Group AI Team
 License: Apache License 2.0
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved
 Classifier: Programming Language :: Python
@@ -29,15 +29,15 @@
 [![GitHub Actions](https://github.com/zillow/quantile-forest/actions/workflows/build.yml/badge.svg)](https://github.com/zillow/quantile-forest/actions/workflows/build.yml)
 [![Codecov](https://codecov.io/gh/zillow/quantile-forest/branch/main/graph/badge.svg?token=STRT8T67YP)](https://codecov.io/gh/zillow/quantile-forest)
 [![Code Style black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/quantile-forest)](https://pypi.org/project/quantile-forest)
 
 **quantile-forest** offers a Python implementation of quantile regression forests compatible with scikit-learn.
 
-Quantile regression forests are a non-parametric, tree-based ensemble method for estimating conditional quantiles, with application to high-dimensional data and uncertainty estimation [[1]](#1). The estimators in this package extend the forest estimators available in scikit-learn to estimate conditional quantiles. They are compatible with and can serve as drop-in replacements for the scikit-learn variants.
+Quantile regression forests are a non-parametric, tree-based ensemble method for estimating conditional quantiles, with application to high-dimensional data and uncertainty estimation [[1]](#1). The estimators in this package extend the forest estimators available in scikit-learn to estimate conditional quantiles; they can estimate arbitrary quantiles at prediction time without retraining. They are compatible with and can serve as drop-in replacements for the scikit-learn variants.
 
 #### Example of fitted model predictions and prediction intervals on California housing data ([code](https://zillow.github.io/quantile-forest/auto_examples/plot_quantile_regression_intervals.html#sphx-glr-auto-examples-plot-quantile-regression-intervals-py))
 <img src="https://zillow.github.io/quantile-forest/_images/sphx_glr_plot_quantile_regression_intervals_001.png" height="300" />
 
 Quick Start
 -----------
```

### Comparing `quantile-forest-1.1.2/quantile_forest.egg-info/SOURCES.txt` & `quantile-forest-1.1.3/quantile_forest.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -29,14 +29,15 @@
 examples/plot_quantile_weighted_vs_unweighted.py
 quantile_forest/__init__.py
 quantile_forest/_min_dependencies.py
 quantile_forest/_quantile_forest.py
 quantile_forest/_quantile_forest_fast.pxd
 quantile_forest/_quantile_forest_fast.pyx
 quantile_forest/version.py
+quantile_forest/version.txt
 quantile_forest.egg-info/PKG-INFO
 quantile_forest.egg-info/SOURCES.txt
 quantile_forest.egg-info/dependency_links.txt
 quantile_forest.egg-info/not-zip-safe
 quantile_forest.egg-info/requires.txt
 quantile_forest.egg-info/top_level.txt
 quantile_forest/tests/__init__.py
```

### Comparing `quantile-forest-1.1.2/setup.cfg` & `quantile-forest-1.1.3/setup.cfg`

 * *Files 20% similar despite different names*

```diff
@@ -21,16 +21,16 @@
 select = B,C,E,F,W,T4,B9
 exclude = 
 	.git,
 	build,
 	__pycache__
 
 [metadata]
-description-file = README.md
-license_file = LICENSE
+description_file = README.md
+license_files = LICENSE
 
 [check-manifest]
 ignore = 
 	quantile_forest/_quantile_forest_fast.pyx
 	quantile_forest/_quantile_forest_fast.pyd
 
 [egg_info]
```

### Comparing `quantile-forest-1.1.2/setup.py` & `quantile-forest-1.1.3/setup.py`

 * *Files identical despite different names*

