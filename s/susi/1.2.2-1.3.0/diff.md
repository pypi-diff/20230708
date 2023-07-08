# Comparing `tmp/susi-1.2.2.zip` & `tmp/susi-1.3.0.zip`

## zipinfo {}

```diff
@@ -1,24 +1,25 @@
-Zip file size: 36183 bytes, number of entries: 22
-drwxr-xr-x  2.0 unx        0 b- stor 21-Dec-11 15:10 susi-1.2.2/
-drwxr-xr-x  2.0 unx        0 b- stor 21-Dec-11 15:10 susi-1.2.2/susi/
-drwxr-xr-x  2.0 unx        0 b- stor 21-Dec-11 15:10 susi-1.2.2/susi.egg-info/
--rw-r--r--  2.0 unx    14091 b- defN 21-Dec-11 15:10 susi-1.2.2/PKG-INFO
--rw-r--r--  2.0 unx     1519 b- defN 21-Mar-29 08:55 susi-1.2.2/LICENSE
--rw-r--r--  2.0 unx       57 b- defN 21-Feb-12 10:07 susi-1.2.2/MANIFEST.in
--rw-r--r--  2.0 unx     2093 b- defN 21-Dec-11 15:10 susi-1.2.2/setup.py
--rw-r--r--  2.0 unx       38 b- defN 21-Dec-11 15:10 susi-1.2.2/setup.cfg
--rw-r--r--  2.0 unx     6255 b- defN 21-Sep-14 16:24 susi-1.2.2/README.rst
--rw-r--r--  2.0 unx     4098 b- defN 21-Dec-11 11:52 susi-1.2.2/CHANGELOG.rst
--rw-r--r--  2.0 unx    17616 b- defN 21-Mar-29 08:55 susi-1.2.2/susi/SOMClassifier.py
--rw-r--r--  2.0 unx    30807 b- defN 21-Oct-05 12:53 susi-1.2.2/susi/SOMClustering.py
--rw-r--r--  2.0 unx     3552 b- defN 21-Mar-29 08:55 susi-1.2.2/susi/SOMUtils.py
--rw-r--r--  2.0 unx     6439 b- defN 21-Mar-29 08:55 susi-1.2.2/susi/SOMPlots.py
--rw-r--r--  2.0 unx      370 b- defN 21-Dec-11 11:52 susi-1.2.2/susi/__init__.py
--rw-r--r--  2.0 unx     5504 b- defN 21-Mar-29 08:55 susi-1.2.2/susi/SOMRegressor.py
--rw-r--r--  2.0 unx    17410 b- defN 21-Mar-29 08:55 susi-1.2.2/susi/SOMEstimator.py
--rw-r--r--  2.0 unx    14091 b- defN 21-Dec-11 15:10 susi-1.2.2/susi.egg-info/PKG-INFO
--rw-r--r--  2.0 unx      329 b- defN 21-Dec-11 15:10 susi-1.2.2/susi.egg-info/SOURCES.txt
--rw-r--r--  2.0 unx      212 b- defN 21-Dec-11 15:10 susi-1.2.2/susi.egg-info/requires.txt
--rw-r--r--  2.0 unx        5 b- defN 21-Dec-11 15:10 susi-1.2.2/susi.egg-info/top_level.txt
--rw-r--r--  2.0 unx        1 b- defN 21-Dec-11 15:10 susi-1.2.2/susi.egg-info/dependency_links.txt
-22 files, 124487 bytes uncompressed, 33307 bytes compressed:  73.2%
+Zip file size: 36327 bytes, number of entries: 23
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-08 16:42 susi-1.3.0/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-08 16:42 susi-1.3.0/susi/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-08 16:42 susi-1.3.0/susi.egg-info/
+-rw-r--r--  2.0 unx    12077 b- defN 23-Jul-08 16:42 susi-1.3.0/PKG-INFO
+-rw-r--r--  2.0 unx     1519 b- defN 23-Jul-08 16:42 susi-1.3.0/LICENSE
+-rw-r--r--  2.0 unx      412 b- defN 23-Jul-08 16:29 susi-1.3.0/pyproject.toml
+-rw-r--r--  2.0 unx       57 b- defN 19-Mar-26 15:15 susi-1.3.0/MANIFEST.in
+-rw-r--r--  2.0 unx     2027 b- defN 23-Jul-08 16:42 susi-1.3.0/setup.py
+-rw-r--r--  2.0 unx       38 b- defN 23-Jul-08 16:42 susi-1.3.0/setup.cfg
+-rw-r--r--  2.0 unx     6406 b- defN 22-May-08 12:56 susi-1.3.0/README.rst
+-rw-r--r--  2.0 unx     4357 b- defN 23-Jul-08 16:42 susi-1.3.0/CHANGELOG.rst
+-rw-r--r--  2.0 unx    17554 b- defN 22-Nov-19 21:14 susi-1.3.0/susi/SOMClassifier.py
+-rw-r--r--  2.0 unx    31325 b- defN 23-Jul-08 16:29 susi-1.3.0/susi/SOMClustering.py
+-rw-r--r--  2.0 unx     3492 b- defN 22-Nov-19 21:14 susi-1.3.0/susi/SOMUtils.py
+-rw-r--r--  2.0 unx     6387 b- defN 23-Jul-08 16:29 susi-1.3.0/susi/SOMPlots.py
+-rw-r--r--  2.0 unx      370 b- defN 23-Jul-08 16:42 susi-1.3.0/susi/__init__.py
+-rw-r--r--  2.0 unx     5440 b- defN 22-Nov-19 21:14 susi-1.3.0/susi/SOMRegressor.py
+-rw-r--r--  2.0 unx    17309 b- defN 22-Nov-19 21:14 susi-1.3.0/susi/SOMEstimator.py
+-rw-r--r--  2.0 unx    12077 b- defN 23-Jul-08 16:42 susi-1.3.0/susi.egg-info/PKG-INFO
+-rw-r--r--  2.0 unx      344 b- defN 23-Jul-08 16:42 susi-1.3.0/susi.egg-info/SOURCES.txt
+-rw-r--r--  2.0 unx      212 b- defN 23-Jul-08 16:42 susi-1.3.0/susi.egg-info/requires.txt
+-rw-r--r--  2.0 unx        5 b- defN 23-Jul-08 16:42 susi-1.3.0/susi.egg-info/top_level.txt
+-rw-r--r--  2.0 unx        1 b- defN 23-Jul-08 16:42 susi-1.3.0/susi.egg-info/dependency_links.txt
+23 files, 121409 bytes uncompressed, 33325 bytes compressed:  72.6%
```

## zipnote {}

```diff
@@ -1,67 +1,70 @@
-Filename: susi-1.2.2/
+Filename: susi-1.3.0/
 Comment: 
 
-Filename: susi-1.2.2/susi/
+Filename: susi-1.3.0/susi/
 Comment: 
 
-Filename: susi-1.2.2/susi.egg-info/
+Filename: susi-1.3.0/susi.egg-info/
 Comment: 
 
-Filename: susi-1.2.2/PKG-INFO
+Filename: susi-1.3.0/PKG-INFO
 Comment: 
 
-Filename: susi-1.2.2/LICENSE
+Filename: susi-1.3.0/LICENSE
 Comment: 
 
-Filename: susi-1.2.2/MANIFEST.in
+Filename: susi-1.3.0/pyproject.toml
 Comment: 
 
-Filename: susi-1.2.2/setup.py
+Filename: susi-1.3.0/MANIFEST.in
 Comment: 
 
-Filename: susi-1.2.2/setup.cfg
+Filename: susi-1.3.0/setup.py
 Comment: 
 
-Filename: susi-1.2.2/README.rst
+Filename: susi-1.3.0/setup.cfg
 Comment: 
 
-Filename: susi-1.2.2/CHANGELOG.rst
+Filename: susi-1.3.0/README.rst
 Comment: 
 
-Filename: susi-1.2.2/susi/SOMClassifier.py
+Filename: susi-1.3.0/CHANGELOG.rst
 Comment: 
 
-Filename: susi-1.2.2/susi/SOMClustering.py
+Filename: susi-1.3.0/susi/SOMClassifier.py
 Comment: 
 
-Filename: susi-1.2.2/susi/SOMUtils.py
+Filename: susi-1.3.0/susi/SOMClustering.py
 Comment: 
 
-Filename: susi-1.2.2/susi/SOMPlots.py
+Filename: susi-1.3.0/susi/SOMUtils.py
 Comment: 
 
-Filename: susi-1.2.2/susi/__init__.py
+Filename: susi-1.3.0/susi/SOMPlots.py
 Comment: 
 
-Filename: susi-1.2.2/susi/SOMRegressor.py
+Filename: susi-1.3.0/susi/__init__.py
 Comment: 
 
-Filename: susi-1.2.2/susi/SOMEstimator.py
+Filename: susi-1.3.0/susi/SOMRegressor.py
 Comment: 
 
-Filename: susi-1.2.2/susi.egg-info/PKG-INFO
+Filename: susi-1.3.0/susi/SOMEstimator.py
 Comment: 
 
-Filename: susi-1.2.2/susi.egg-info/SOURCES.txt
+Filename: susi-1.3.0/susi.egg-info/PKG-INFO
 Comment: 
 
-Filename: susi-1.2.2/susi.egg-info/requires.txt
+Filename: susi-1.3.0/susi.egg-info/SOURCES.txt
 Comment: 
 
-Filename: susi-1.2.2/susi.egg-info/top_level.txt
+Filename: susi-1.3.0/susi.egg-info/requires.txt
 Comment: 
 
-Filename: susi-1.2.2/susi.egg-info/dependency_links.txt
+Filename: susi-1.3.0/susi.egg-info/top_level.txt
+Comment: 
+
+Filename: susi-1.3.0/susi.egg-info/dependency_links.txt
 Comment: 
 
 Zip file comment:
```

## Comparing `susi-1.2.2/PKG-INFO` & `susi-1.3.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,335 +1,346 @@
 Metadata-Version: 2.1
 Name: susi
-Version: 1.2.2
+Version: 1.3.0
 Summary: Python package for unsupervised, supervised and semi-supervised self-organizing maps (SOM)
 Home-page: https://github.com/felixriese/susi
 Author: Felix M. Riese
 Author-email: github@felixriese.de
 License: BSD-3-Clause
-Project-URL: Source, https://github.com/felixriese/susi
 Project-URL: Documentation, https://susi.readthedocs.io/en/latest/?badge=latest
+Project-URL: Source, https://github.com/felixriese/susi
 Project-URL: Tracker, https://github.com/felixriese/susi/issues
-Description: .. image:: https://badge.fury.io/py/susi.svg
-            :target: https://pypi.org/project/susi/
-            :alt: PyPi - Code Version
-        
-        .. image:: https://img.shields.io/pypi/pyversions/susi.svg
-            :target: https://pypi.org/project/susi/
-            :alt: PyPI - Python Version
-        
-        .. image:: https://travis-ci.com/felixriese/susi.svg?branch=master
-            :target: https://travis-ci.com/felixriese/susi
-            :alt: Travis.CI Status
-        
-        .. image:: https://readthedocs.org/projects/susi/badge/?version=latest
-            :target: https://susi.readthedocs.io/en/latest/?badge=latest
-            :alt: Documentation Status
-        
-        .. image:: https://codecov.io/gh/felixriese/susi/branch/master/graph/badge.svg
-            :target: https://codecov.io/gh/felixriese/susi
-            :alt: Codecov
-        
-        .. image:: https://api.codacy.com/project/badge/Grade/d304689a7364437db1ef998cf7765f5a
-        	:target: https://app.codacy.com/app/felixriese/susi
-        	:alt: Codacy Badge
-        
-        .. image:: https://anaconda.org/conda-forge/susi/badges/version.svg
-            :target: https://anaconda.org/conda-forge/susi
-            :alt: Conda-forge
-            
-        .. image:: https://requires.io/github/felixriese/susi/requirements.svg?branch=main
-             :target: https://requires.io/github/felixriese/susi/requirements/?branch=main
-             :alt: Requirements Status
-        
-        |
-        
-        .. image:: https://raw.githubusercontent.com/felixriese/susi/master/docs/_static/susi_logo_small.png
-            :target: https://github.com/felixriese/susi
-            :align: right
-            :alt: SuSi logo
-        
-        SuSi: Supervised Self-organizing maps in Python
-        ===============================================
-        
-        Python package for unsupervised, supervised and semi-supervised self-organizing maps (SOM)
-        
-        Description
-        -----------
-        
-        We present the SuSi package for Python.
-        It includes a fully functional SOM for unsupervised, supervised and semi-supervised tasks:
-        
-        - SOMClustering: Unsupervised SOM for clustering
-        - SOMRegressor: (Semi-)Supervised Regression SOM
-        - SOMClassifier: (Semi-)Supervised Classification SOM
-        
-        :License:
-            `3-Clause BSD license <LICENSE>`_
-        
-        :Author:
-            `Felix M. Riese <mailto:github@felixriese.de>`_
-        
-        :Citation:
-            see `Citation`_ and in the `bibtex <https://github.com/felixriese/susi/blob/main/bibliography.bib>`_ file
-        
-        :Documentation:
-            `Documentation <https://susi.readthedocs.io/en/latest/index.html>`_
-        
-        :Installation:
-            `Installation guidelines <https://susi.readthedocs.io/en/latest/install.html>`_
-        
-        :Paper:
-            `F. M. Riese, S. Keller and S. Hinz in Remote Sensing, 2020 <https://www.mdpi.com/2072-4292/12/1/7>`_
-        
-        
-        Installation
-        ------------
-        
-        Pip
-        ~~~
-        
-        .. code:: bash
-        
-            pip3 install susi
-        
-        Conda
-        ~~~~~
-        
-        .. code:: bash
-        
-            conda install -c conda-forge susi
-        
-        More information can be found in the `installation guidelines <https://susi.readthedocs.io/en/latest/install.html>`_.
-        
-        .. image:: https://static.pepy.tech/personalized-badge/susi?period=total&units=international_system&left_color=black&right_color=blue&left_text=Downloads
-        	:target: https://pepy.tech/project/susi
-        	:alt: Downloads
-        
-        Examples
-        --------
-        
-        A collection of code examples can be found in `the documentation <https://susi.readthedocs.io/en/latest/examples.html>`_.
-        Code examples as Jupyter Notebooks can be found here:
-        
-        * `examples/SOMClustering <https://github.com/felixriese/susi/blob/main/examples/SOMClustering.ipynb>`_
-        * `examples/SOMRegressor <https://github.com/felixriese/susi/blob/main/examples/SOMRegressor.ipynb>`_
-        * `examples/SOMRegressor_semisupervised <https://github.com/felixriese/susi/blob/main/examples/SOMRegressor_semisupervised.ipynb>`_
-        * `examples/SOMRegressor_multioutput <https://github.com/felixriese/susi/blob/main/examples/SOMRegressor_multioutput.ipynb>`_
-        * `examples/SOMClassifier <https://github.com/felixriese/susi/blob/main/examples/SOMClassifier.ipynb>`_
-        * `examples/SOMClassifier_semisupervised <https://github.com/felixriese/susi/blob/main/examples/SOMClassifier_semisupervised.ipynb>`_
-        
-        FAQs
-        -----
-        
-        - **How should I set the initial hyperparameters of a SOM?** For more details
-          on the hyperparameters, see in `documentation/hyperparameters
-          <https://susi.readthedocs.io/en/latest/hyperparameters.html>`_.
-        - **How can I optimize the hyperparameters?** The SuSi hyperparameters
-          can be optimized, for example, with `scikit-learn.model_selection.GridSearchCV
-          <https://scikit-learn.org/stable/modules/generated/sklearn.model_selection.GridSearchCV.html>`_,
-          since the SuSi package is developed according to several scikit-learn
-          guidelines.
-        
-        
-        ------------
-        
-        
-        Citation
-        --------
-        
-        The bibtex file including both references is available in `bibliography.bib
-        <https://github.com/felixriese/susi/blob/main/bibliography.bib>`_.
-        
-        **Paper:**
-        
-        F. M. Riese, S. Keller and S. Hinz, "Supervised and Semi-Supervised Self-Organizing
-        Maps for Regression and Classification Focusing on Hyperspectral Data",
-        *Remote Sensing*, vol. 12, no. 1, 2020. `DOI:10.3390/rs12010007
-        <https://doi.org/10.3390/rs12010007>`_
-        
-        .. code:: bibtex
-        
-            @article{riese2020supervised,
-                author = {Riese, Felix~M. and Keller, Sina and Hinz, Stefan},
-                title = {{Supervised and Semi-Supervised Self-Organizing Maps for
-                          Regression and Classification Focusing on Hyperspectral Data}},
-                journal = {Remote Sensing},
-                year = {2020},
-                volume = {12},
-                number = {1},
-                article-number = {7},
-                URL = {https://www.mdpi.com/2072-4292/12/1/7},
-                ISSN = {2072-4292},
-                DOI = {10.3390/rs12010007}
-            }
-        
-        **Code:**
-        
-        Felix M. Riese, "SuSi: SUpervised Self-organIzing maps in Python",
-        Zenodo, 2019. `DOI:10.5281/zenodo.2609130
-        <https://doi.org/10.5281/zenodo.2609130>`_
-        
-        .. image:: https://zenodo.org/badge/DOI/10.5281/zenodo.2609130.svg
-           :target: https://doi.org/10.5281/zenodo.2609130
-        
-        .. code:: bibtex
-        
-            @misc{riese2019susicode,
-                author = {Riese, Felix~M.},
-                title = {{SuSi: Supervised Self-Organizing Maps in Python}},
-                year = {2019},
-                DOI = {10.5281/zenodo.2609130},
-                publisher = {Zenodo},
-                howpublished = {\href{https://doi.org/10.5281/zenodo.2609130}{doi.org/10.5281/zenodo.2609130}}
-            }
-        
-        -------------
-        
-        License
-        -------
-        
-        This project is published under the `3-Clause BSD <LICENSE>`_ license.
-        
-        .. image:: https://img.shields.io/pypi/l/susi.svg
-            :target: https://github.com/felixriese/susi/blob/main/LICENSE
-            :alt: PyPI - License
-        
-        
-        Change Log
-        ==========
-        
-        [1.2.2] - 2021-12-11
-        --------------------
-        - [ADDED] Official support for Python 3.10.
-        - [REMOVED] Official support for Python 3.6 (will be deprecated end of 2021
-          anyways). It might still work, but will not be maintained on this version.
-        
-        [1.2.1] - 2021-10-19
-        --------------------
-        - [ADDED] Quantization error `get_quantization_error()`
-        
-        [1.2] - 2021-04-04
-        ------------------
-        - [ADDED] Landing page with vuepress.
-        - [ADDED] Conda-forge recipe.
-        - [ADDED] Function `SOMClassifier.predict_proba()`
-        - [ADDED] Example notebook for multi-output regression
-        - [CHANGED] Code formatting to black.
-        - [CHANGED] CI from travis to GitHub actions.
-        - [FIXED] Requirements in setup.py
-        
-        [1.1.2] - 2021-02-18
-        --------------------
-        - [ADDED] Python 3.9 support. Python 3.6 support will be removed soon.
-        - [CHANGED] Function names for private use now start with an underscore.
-        
-        [1.1.1] - 2020-11-18
-        --------------------
-        - [ADDED] New distance metric "spectralangle".
-        - [ADDED] FAQs.
-        - [ADDED] Separate between positional and keyword parameters.
-        - [ADDED] Plot script for neighborhood distance weight matrix.
-        - [FIXED] Added inherited members to code documentation.
-        
-        [1.1.0] - 2020-08-31
-        --------------------
-        - [ADDED] Logo.
-        - [ADDED] SOMPlots documentation.
-        - [REMOVED] Python 3.5 support. Now, only 3.6-3.8 are supported.
-        - [FIXED] Scikit-learn warnings regarding validation of positional arguments.
-        - [FIXED] Sphinx documentation warnings.
-        
-        [1.0.10] - 2020-04-21
-        ------------------------------------
-        - [ADDED] Support for Python 3.8.x.
-        - [ADDED] Test coverage and MultiOutput test.
-        - [CHANGED] Function `setPlaceholder` to `_set_placeholder`.
-        - [FIXED] Documentation links
-        
-        [1.0.9] - 2020-04-07
-        ------------------------
-        - [ADDED] Documentation of the hyperparameters.
-        - [ADDED] Plot scripts.
-        - [CHANGED] Structure of the module files.
-        
-        [1.0.8] - 2020-01-20
-        ------------------------
-        - [FIXED] Replaced scikit-learn `sklearn.utils.fixes.parallel_helper`, see #12.
-        
-        [1.0.7] - 2019-11-28
-        ------------------------
-        - [ADDED] Optional tqdm visualization of the SOM training
-        - [ADDED] New `init_mode_supervised` called `random_minmax`.
-        - [CHANGED] Official name of package changes from `SUSI` to `SuSi`.
-        - [CHANGED] Docstrings for functions are now according to guidelines.
-        - [FIXED] Semi-supervised classification handling, sample weights
-        - [FIXED] Supervised classification SOM initalization of `n_iter_supervised`
-        - [FIXED] Code refactored according to prospector
-        - [FIXED] Resolved bug in `get_datapoints_from_node()` for unsupervised SOM.
-        
-        [1.0.6] - 2019-09-11
-        ------------------------
-        - [ADDED] Semi-supervised abilities for classifier and regressor
-        - [ADDED] Example notebooks for semi-supervised applications
-        - [ADDED] Tests for example notebooks
-        - [CHANGED] Requirements for the SuSi package
-        - [REMOVED] Support for Python 3.4
-        - [FIXED] Code looks better in documentation with sphinx.ext.napoleon
-        
-        [1.0.5] - 2019-04-23
-        ------------------------
-        - [ADDED] PCA initialization of the SOM weights with 2 principal components
-        - [ADDED] Variable variance
-        - [CHANGED] Moved installation guidelines and examples to documentation
-        
-        [1.0.4] - 2019-04-21
-        ------------------------
-        - [ADDED] Batch algorithm for unsupervised and supervised SOM
-        - [ADDED] Calculation of the unified distance matrix (u-matrix)
-        - [FIXED] Added estimator_check of scikit-learn and fixed recognized issues
-        
-        [1.0.3] - 2019-04-09
-        ------------------------
-        - [ADDED] Link to arXiv paper
-        - [ADDED] Mexican-hat neighborhood distance weight
-        - [ADDED] Possibility for different initialization modes
-        - [CHANGED] Simplified initialization of estimators
-        - [FIXED] URLs and styles in documentation
-        - [FIXED] Colormap in Salinas example
-        
-        [1.0.2] - 2019-03-27
-        ------------------------
-        - [ADDED] Codecov, Codacy
-        - [CHANGED] Moved decreasing_rate() out of SOM classes
-        - [FIXED] Removed duplicate constructor for SOMRegressor, fixed fit() params
-        
-        [1.0.1] - 2019-03-26
-        ------------------------
-        - [ADDED] Config file for Travis
-        - [ADDED] Requirements for read-the-docs documentation
-        
-        [1.0.0] - 2019-03-26
-        ------------------------
-        - Initial release
-        
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 Provides-Extra: docs
+Provides-Extra: examples
 Provides-Extra: tests
 Provides-Extra: formatting
-Provides-Extra: examples
+License-File: LICENSE
+
+.. image:: https://badge.fury.io/py/susi.svg
+    :target: https://pypi.org/project/susi/
+    :alt: PyPi - Code Version
+
+.. image:: https://img.shields.io/pypi/pyversions/susi.svg
+    :target: https://pypi.org/project/susi/
+    :alt: PyPI - Python Version
+
+.. image:: https://travis-ci.com/felixriese/susi.svg?branch=master
+    :target: https://travis-ci.com/felixriese/susi
+    :alt: Travis.CI Status
+
+.. image:: https://readthedocs.org/projects/susi/badge/?version=latest
+    :target: https://susi.readthedocs.io/en/latest/?badge=latest
+    :alt: Documentation Status
+
+.. image:: https://codecov.io/gh/felixriese/susi/branch/master/graph/badge.svg
+    :target: https://codecov.io/gh/felixriese/susi
+    :alt: Codecov
+
+.. image:: https://api.codacy.com/project/badge/Grade/d304689a7364437db1ef998cf7765f5a
+	:target: https://app.codacy.com/app/felixriese/susi
+	:alt: Codacy Badge
+
+.. image:: https://anaconda.org/conda-forge/susi/badges/version.svg
+    :target: https://anaconda.org/conda-forge/susi
+    :alt: Conda-forge
+    
+.. image:: https://requires.io/github/felixriese/susi/requirements.svg?branch=main
+     :target: https://requires.io/github/felixriese/susi/requirements/?branch=main
+     :alt: Requirements Status
+
+|
+
+.. image:: https://raw.githubusercontent.com/felixriese/susi/master/docs/_static/susi_logo_small.png
+    :target: https://github.com/felixriese/susi
+    :align: right
+    :alt: SuSi logo
+
+SuSi: Supervised Self-organizing maps in Python
+===============================================
+
+Python package for unsupervised, supervised and semi-supervised self-organizing maps (SOM)
+
+Description
+-----------
+
+We present the SuSi package for Python.
+It includes a fully functional SOM for unsupervised, supervised and semi-supervised tasks:
+
+- SOMClustering: Unsupervised SOM for clustering
+- SOMRegressor: (Semi-)Supervised Regression SOM
+- SOMClassifier: (Semi-)Supervised Classification SOM
+
+:License:
+    `3-Clause BSD license <LICENSE>`_
+
+:Author:
+    `Felix M. Riese <mailto:github@felixriese.de>`_
+
+:Citation:
+    see `Citation`_ and in the `bibtex <https://github.com/felixriese/susi/blob/main/bibliography.bib>`_ file
+
+:Documentation:
+    `Documentation <https://susi.readthedocs.io/en/latest/index.html>`_
+
+:Installation:
+    `Installation guidelines <https://susi.readthedocs.io/en/latest/install.html>`_
+
+:Paper:
+    `F. M. Riese, S. Keller and S. Hinz in Remote Sensing, 2020 <https://www.mdpi.com/2072-4292/12/1/7>`_
+
+
+Installation
+------------
+
+Pip
+~~~
+
+.. code:: bash
+
+    pip3 install susi
+    
+.. image:: https://static.pepy.tech/personalized-badge/susi?period=total&units=international_system&left_color=black&right_color=blue&left_text=Downloads
+	:target: https://pepy.tech/project/susi
+	:alt: PyPi Downloads
+
+Conda
+~~~~~
+
+.. code:: bash
+
+    conda install -c conda-forge susi
+
+More information can be found in the `installation guidelines <https://susi.readthedocs.io/en/latest/install.html>`_.
+
+.. image:: https://img.shields.io/conda/dn/conda-forge/susi.svg
+	:target: https://anaconda.org/conda-forge/susi
+	:alt: Conda-Forge Downloads
+
+Examples
+--------
+
+A collection of code examples can be found in `the documentation <https://susi.readthedocs.io/en/latest/examples.html>`_.
+Code examples as Jupyter Notebooks can be found here:
+
+* `examples/SOMClustering <https://github.com/felixriese/susi/blob/main/examples/SOMClustering.ipynb>`_
+* `examples/SOMRegressor <https://github.com/felixriese/susi/blob/main/examples/SOMRegressor.ipynb>`_
+* `examples/SOMRegressor_semisupervised <https://github.com/felixriese/susi/blob/main/examples/SOMRegressor_semisupervised.ipynb>`_
+* `examples/SOMRegressor_multioutput <https://github.com/felixriese/susi/blob/main/examples/SOMRegressor_multioutput.ipynb>`_
+* `examples/SOMClassifier <https://github.com/felixriese/susi/blob/main/examples/SOMClassifier.ipynb>`_
+* `examples/SOMClassifier_semisupervised <https://github.com/felixriese/susi/blob/main/examples/SOMClassifier_semisupervised.ipynb>`_
+
+FAQs
+-----
+
+- **How should I set the initial hyperparameters of a SOM?** For more details
+  on the hyperparameters, see in `documentation/hyperparameters
+  <https://susi.readthedocs.io/en/latest/hyperparameters.html>`_.
+- **How can I optimize the hyperparameters?** The SuSi hyperparameters
+  can be optimized, for example, with `scikit-learn.model_selection.GridSearchCV
+  <https://scikit-learn.org/stable/modules/generated/sklearn.model_selection.GridSearchCV.html>`_,
+  since the SuSi package is developed according to several scikit-learn
+  guidelines.
+
+
+------------
+
+
+Citation
+--------
+
+The bibtex file including both references is available in `bibliography.bib
+<https://github.com/felixriese/susi/blob/main/bibliography.bib>`_.
+
+**Paper:**
+
+F. M. Riese, S. Keller and S. Hinz, "Supervised and Semi-Supervised Self-Organizing
+Maps for Regression and Classification Focusing on Hyperspectral Data",
+*Remote Sensing*, vol. 12, no. 1, 2020. `DOI:10.3390/rs12010007
+<https://doi.org/10.3390/rs12010007>`_
+
+.. code:: bibtex
+
+    @article{riese2020supervised,
+        author = {Riese, Felix~M. and Keller, Sina and Hinz, Stefan},
+        title = {{Supervised and Semi-Supervised Self-Organizing Maps for
+                  Regression and Classification Focusing on Hyperspectral Data}},
+        journal = {Remote Sensing},
+        year = {2020},
+        volume = {12},
+        number = {1},
+        article-number = {7},
+        URL = {https://www.mdpi.com/2072-4292/12/1/7},
+        ISSN = {2072-4292},
+        DOI = {10.3390/rs12010007}
+    }
+
+**Code:**
+
+Felix M. Riese, "SuSi: SUpervised Self-organIzing maps in Python",
+Zenodo, 2019. `DOI:10.5281/zenodo.2609130
+<https://doi.org/10.5281/zenodo.2609130>`_
+
+.. image:: https://zenodo.org/badge/DOI/10.5281/zenodo.2609130.svg
+   :target: https://doi.org/10.5281/zenodo.2609130
+
+.. code:: bibtex
+
+    @misc{riese2019susicode,
+        author = {Riese, Felix~M.},
+        title = {{SuSi: Supervised Self-Organizing Maps in Python}},
+        year = {2019},
+        DOI = {10.5281/zenodo.2609130},
+        publisher = {Zenodo},
+        howpublished = {\href{https://doi.org/10.5281/zenodo.2609130}{doi.org/10.5281/zenodo.2609130}}
+    }
+
+-------------
+
+License
+-------
+
+This project is published under the `3-Clause BSD <LICENSE>`_ license.
+
+.. image:: https://img.shields.io/pypi/l/susi.svg
+    :target: https://github.com/felixriese/susi/blob/main/LICENSE
+    :alt: PyPI - License
+
+
+Change Log
+==========
+
+[1.3.0] - 2023-07-08
+--------------------
+- [ADDED] Official support for Python 3.11.
+- [FIXED] Quantization error axis bug.
+- [REMOVED] Official support for Python 3.7 (deprecated in 2023). It might
+  still work, but will not be maintained on this version.
+
+[1.2.2] - 2021-12-11
+--------------------
+- [ADDED] Official support for Python 3.10.
+- [REMOVED] Official support for Python 3.6 (will be deprecated end of 2021
+  anyways). It might still work, but will not be maintained on this version.
+
+[1.2.1] - 2021-10-19
+--------------------
+- [ADDED] Quantization error `get_quantization_error()`
+
+[1.2] - 2021-04-04
+------------------
+- [ADDED] Landing page with vuepress.
+- [ADDED] Conda-forge recipe.
+- [ADDED] Function `SOMClassifier.predict_proba()`
+- [ADDED] Example notebook for multi-output regression
+- [CHANGED] Code formatting to black.
+- [CHANGED] CI from travis to GitHub actions.
+- [FIXED] Requirements in setup.py
+
+[1.1.2] - 2021-02-18
+--------------------
+- [ADDED] Python 3.9 support. Python 3.6 support will be removed soon.
+- [CHANGED] Function names for private use now start with an underscore.
+
+[1.1.1] - 2020-11-18
+--------------------
+- [ADDED] New distance metric "spectralangle".
+- [ADDED] FAQs.
+- [ADDED] Separate between positional and keyword parameters.
+- [ADDED] Plot script for neighborhood distance weight matrix.
+- [FIXED] Added inherited members to code documentation.
+
+[1.1.0] - 2020-08-31
+--------------------
+- [ADDED] Logo.
+- [ADDED] SOMPlots documentation.
+- [REMOVED] Python 3.5 support. Now, only 3.6-3.8 are supported.
+- [FIXED] Scikit-learn warnings regarding validation of positional arguments.
+- [FIXED] Sphinx documentation warnings.
+
+[1.0.10] - 2020-04-21
+------------------------------------
+- [ADDED] Support for Python 3.8.x.
+- [ADDED] Test coverage and MultiOutput test.
+- [CHANGED] Function `setPlaceholder` to `_set_placeholder`.
+- [FIXED] Documentation links
+
+[1.0.9] - 2020-04-07
+------------------------
+- [ADDED] Documentation of the hyperparameters.
+- [ADDED] Plot scripts.
+- [CHANGED] Structure of the module files.
+
+[1.0.8] - 2020-01-20
+------------------------
+- [FIXED] Replaced scikit-learn `sklearn.utils.fixes.parallel_helper`, see #12.
+
+[1.0.7] - 2019-11-28
+------------------------
+- [ADDED] Optional tqdm visualization of the SOM training
+- [ADDED] New `init_mode_supervised` called `random_minmax`.
+- [CHANGED] Official name of package changes from `SUSI` to `SuSi`.
+- [CHANGED] Docstrings for functions are now according to guidelines.
+- [FIXED] Semi-supervised classification handling, sample weights
+- [FIXED] Supervised classification SOM initalization of `n_iter_supervised`
+- [FIXED] Code refactored according to prospector
+- [FIXED] Resolved bug in `get_datapoints_from_node()` for unsupervised SOM.
+
+[1.0.6] - 2019-09-11
+------------------------
+- [ADDED] Semi-supervised abilities for classifier and regressor
+- [ADDED] Example notebooks for semi-supervised applications
+- [ADDED] Tests for example notebooks
+- [CHANGED] Requirements for the SuSi package
+- [REMOVED] Support for Python 3.4
+- [FIXED] Code looks better in documentation with sphinx.ext.napoleon
+
+[1.0.5] - 2019-04-23
+------------------------
+- [ADDED] PCA initialization of the SOM weights with 2 principal components
+- [ADDED] Variable variance
+- [CHANGED] Moved installation guidelines and examples to documentation
+
+[1.0.4] - 2019-04-21
+------------------------
+- [ADDED] Batch algorithm for unsupervised and supervised SOM
+- [ADDED] Calculation of the unified distance matrix (u-matrix)
+- [FIXED] Added estimator_check of scikit-learn and fixed recognized issues
+
+[1.0.3] - 2019-04-09
+------------------------
+- [ADDED] Link to arXiv paper
+- [ADDED] Mexican-hat neighborhood distance weight
+- [ADDED] Possibility for different initialization modes
+- [CHANGED] Simplified initialization of estimators
+- [FIXED] URLs and styles in documentation
+- [FIXED] Colormap in Salinas example
+
+[1.0.2] - 2019-03-27
+------------------------
+- [ADDED] Codecov, Codacy
+- [CHANGED] Moved decreasing_rate() out of SOM classes
+- [FIXED] Removed duplicate constructor for SOMRegressor, fixed fit() params
+
+[1.0.1] - 2019-03-26
+------------------------
+- [ADDED] Config file for Travis
+- [ADDED] Requirements for read-the-docs documentation
+
+[1.0.0] - 2019-03-26
+------------------------
+- Initial release
```

## Comparing `susi-1.2.2/LICENSE` & `susi-1.3.0/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 BSD 3-Clause License
 
-Copyright (c) 2019-2021 Felix M. Riese.
+Copyright (c) 2019-2023 Felix M. Riese.
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
 
 * Redistributions of source code must retain the above copyright notice, this
   list of conditions and the following disclaimer.
```

## Comparing `susi-1.2.2/setup.py` & `susi-1.3.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 # -*- coding: utf-8 -*-
 
-# Copyright (c) 2019-2021 by Felix M. Riese. All rights reserved.
-
 import setuptools
 
 with open("README.rst", "r") as f:
     readme = f.read()
 
 with open("CHANGELOG.rst", "r") as f:
     changelog = f.read()
 
 long_description = "\n\n".join((readme, changelog))
 
 setuptools.setup(
     name="susi",
-    version="1.2.2",
+    version="1.3.0",
     author="Felix M. Riese",
     author_email="github@felixriese.de",
     description=(
         "Python package for unsupervised, supervised and "
         "semi-supervised self-organizing maps (SOM)"
     ),
     long_description=long_description,
@@ -38,18 +36,18 @@
         "examples": ["notebook", "seaborn", "pandas"],
         "tests": ["pytest", "pytest-cov", "codecov", "nbval", "coverage"],
         "formatting": ["black"],
     },
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Environment :: Console",
         "Intended Audience :: Developers",
         "Intended Audience :: Education",
         "Intended Audience :: Information Technology",
         "Intended Audience :: Science/Research",
         "License :: OSI Approved :: BSD License",
         "Natural Language :: English",
```

## Comparing `susi-1.2.2/README.rst` & `susi-1.3.0/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -76,27 +76,31 @@
 
 Pip
 ~~~
 
 .. code:: bash
 
     pip3 install susi
+    
+.. image:: https://static.pepy.tech/personalized-badge/susi?period=total&units=international_system&left_color=black&right_color=blue&left_text=Downloads
+	:target: https://pepy.tech/project/susi
+	:alt: PyPi Downloads
 
 Conda
 ~~~~~
 
 .. code:: bash
 
     conda install -c conda-forge susi
 
 More information can be found in the `installation guidelines <https://susi.readthedocs.io/en/latest/install.html>`_.
 
-.. image:: https://static.pepy.tech/personalized-badge/susi?period=total&units=international_system&left_color=black&right_color=blue&left_text=Downloads
-	:target: https://pepy.tech/project/susi
-	:alt: Downloads
+.. image:: https://img.shields.io/conda/dn/conda-forge/susi.svg
+	:target: https://anaconda.org/conda-forge/susi
+	:alt: Conda-Forge Downloads
 
 Examples
 --------
 
 A collection of code examples can be found in `the documentation <https://susi.readthedocs.io/en/latest/examples.html>`_.
 Code examples as Jupyter Notebooks can be found here:
```

## Comparing `susi-1.2.2/CHANGELOG.rst` & `susi-1.3.0/CHANGELOG.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,17 @@
 Change Log
 ==========
 
+[1.3.0] - 2023-07-08
+--------------------
+- [ADDED] Official support for Python 3.11.
+- [FIXED] Quantization error axis bug.
+- [REMOVED] Official support for Python 3.7 (deprecated in 2023). It might
+  still work, but will not be maintained on this version.
+
 [1.2.2] - 2021-12-11
 --------------------
 - [ADDED] Official support for Python 3.10.
 - [REMOVED] Official support for Python 3.6 (will be deprecated end of 2021
   anyways). It might still work, but will not be maintained on this version.
 
 [1.2.1] - 2021-10-19
```

## Comparing `susi-1.2.2/susi/SOMClassifier.py` & `susi-1.3.0/susi/SOMClassifier.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,8 @@
-"""SOMClassifier class.
-
-Copyright (c) 2019-2021 Felix M. Riese.
-All rights reserved.
-
-"""
+"""SOMClassifier class."""
 from typing import Optional, Sequence, Tuple, Union
 
 import numpy as np
 from scipy.special import softmax
 from sklearn.base import ClassifierMixin
 from sklearn.preprocessing import LabelBinarizer
 from sklearn.utils.validation import check_array, check_is_fitted
@@ -351,15 +346,15 @@
 
         # transform to numpy array
         return np.array(proba_list)
 
     def _modify_weight_matrix_supervised(
         self,
         dist_weight_matrix: np.ndarray,
-        true_vector: Optional[np.array] = None,
+        true_vector: Optional[np.ndarray] = None,
         learning_rate: Optional[float] = None,
     ) -> np.ndarray:
         """Modify weight matrix of the SOM.
 
         Parameters
         ----------
         dist_weight_matrix : np.ndarray of float
```

## Comparing `susi-1.2.2/susi/SOMClustering.py` & `susi-1.3.0/susi/SOMClustering.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,8 @@
-"""SOMClustering class.
-
-Copyright (c) 2019-2021 Felix M. Riese.
-All rights reserved.
-
-"""
+"""SOMClustering class."""
 
 import itertools
 from typing import List, Optional, Sequence, Tuple
 
 import numpy as np
 import scipy.spatial.distance as dist
 from joblib import Parallel, delayed, effective_n_jobs
@@ -189,15 +184,16 @@
                 som[node[0], node[1], :] = np.add(
                     np.multiply(a_row[node[0]], pca_comp[0]),
                     np.multiply(a_col[node[1]], pca_comp[1]),
                 )
 
         else:
             raise ValueError(
-                f"Invalid init_mode_unsupervised: {self.init_mode_unsupervised}."
+                f"Invalid init_mode_unsupervised: "
+                f"{self.init_mode_unsupervised}."
             )
 
         self.unsuper_som_ = som
 
     def fit(self, X: Sequence, y: Optional[Sequence] = None):
         """Fit unsupervised SOM to input data.
 
@@ -368,15 +364,15 @@
         a = self._get_node_distance_matrix(
             datapoint.astype(np.float64), som_array
         )
 
         return np.argwhere(a == np.min(a))[0]
 
     def get_bmus(
-        self, X: np.ndarray, som_array: Optional[np.array] = None
+        self, X: np.ndarray, som_array: Optional[np.ndarray] = None
     ) -> Optional[List[Tuple[int, int]]]:
         """Get Best Matching Units for big datalist.
 
         Parameters
         ----------
         X : np.ndarray
             List of datapoints
@@ -444,15 +440,15 @@
 
         n_datapoints_per_job[: n_datapoints % n_jobs] += 1
         starts = np.cumsum(n_datapoints_per_job)
 
         return n_jobs, n_datapoints_per_job.tolist(), [0] + starts.tolist()
 
     def _set_bmus(
-        self, X: np.ndarray, som_array: Optional[np.array] = None
+        self, X: np.ndarray, som_array: Optional[np.ndarray] = None
     ) -> None:
         """Set BMUs in the current SOM object.
 
         Parameters
         ----------
         X : array-like matrix of shape = [n_samples, n_features]
             The input samples.
@@ -513,26 +509,27 @@
             for node in self.node_list_:
                 som_node = som_array[node[0], node[1]]
                 distmat[node] = dist.rogerstanimoto(
                     binarize(
                         datapoint.reshape(1, -1),
                         threshold=threshold,
                         copy=True,
-                    ),
+                    ).ravel(),
                     binarize(
                         som_node.reshape(1, -1), threshold=threshold, copy=True
-                    ),
+                    ).ravel(),
                 )
 
         elif self.distance_metric == "spectralangle":
             for node in self.node_list_:
                 distmat[node] = np.arccos(
                     np.divide(
                         np.dot(som_array[node[0], node[1]], datapoint),
                         np.multiply(
+                            # TODO check if an axis needs to be set here
                             np.linalg.norm(som_array),
                             np.linalg.norm(datapoint),
                         ),
                     )
                 )
 
         return distmat
@@ -927,14 +924,32 @@
         )
         column_range = range(
             max(node[1] - radius, 0),
             min(node[1] + radius, self.n_columns - 1) + 1,
         )
         return list(itertools.product(row_range, column_range))
 
+    def _get_weights_per_datapoint(self, datapoints: Sequence) -> list:
+        """Get SOM weights per datapoint.
+
+        Parameters
+        ----------
+        datapoints : array-like matrix, optional (default=True)
+            Samples of shape = [n_samples, n_features].
+
+        Returns
+        -------
+        float
+            Mean quantization error over all datapoints.
+        """
+        return [
+            self.unsuper_som_[bmu[0], bmu[1]]
+            for bmu in self.get_bmus(datapoints)
+        ]
+
     def get_quantization_error(self, X: Optional[Sequence] = None) -> float:
         """Get quantization error for `X` (or the training data).
 
         Parameters
         ----------
         X : array-like matrix, optional (default=True)
             Samples of shape = [n_samples, n_features]. If `None`, the training
@@ -953,16 +968,14 @@
         """
         if not self.fitted_:
             raise RuntimeError("SOM is not fitted!")
 
         if X is None:
             X = self.X_
 
-        weights_per_datapoint = [
-            self.unsuper_som_[bmu[0], bmu[1]] for bmu in self.get_bmus(X)
-        ]
+        weights_per_datapoint = self._get_weights_per_datapoint(X)
 
         quantization_errors = np.linalg.norm(
-            np.subtract(weights_per_datapoint, X)
+            np.subtract(weights_per_datapoint, X), axis=1
         )
 
         return np.mean(quantization_errors)
```

## Comparing `susi-1.2.2/susi/SOMUtils.py` & `susi-1.3.0/susi/SOMUtils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,8 @@
-"""SOMUtils functions.
-
-Copyright (c) 2019-2021 Felix M. Riese.
-All rights reserved.
-
-"""
+"""SOMUtils functions."""
 from typing import Sequence, Tuple
 
 import numpy as np
 from sklearn.utils.multiclass import check_classification_targets
 from sklearn.utils.validation import check_array, check_X_y
 
 
@@ -68,15 +63,15 @@
     # rate = max(rate, a_2)
 
     return rate
 
 
 def check_estimation_input(
     X: Sequence, y: Sequence, *, is_classification: bool = False
-) -> Tuple[np.array, np.array]:
+) -> Tuple[np.ndarray, np.ndarray]:
     """Check input arrays.
 
     This function is adapted from sklearn.utils.validation.
 
     Parameters
     ----------
     X : nd-array or list
```

## Comparing `susi-1.2.2/susi/SOMPlots.py` & `susi-1.3.0/susi/SOMPlots.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,13 @@
-"""SOMPlots functions.
-
-Copyright (c) 2019-2021 Felix M. Riese.
-All rights reserved.
-
-"""
+"""SOMPlots functions."""
 
 from typing import List, Tuple
 
-import matplotlib.pyplot as plt
 import matplotlib
+import matplotlib.pyplot as plt
 import numpy as np
 
 
 def plot_estimation_map(
     estimation_map: np.ndarray,
     cbar_label: str = "Variable in unit",
     cmap: str = "viridis",
@@ -48,15 +43,15 @@
     # colorbar
     cbar = plt.colorbar(img, ax=ax)
     cbar.ax.tick_params(labelsize=fontsize)
     cbar.ax.set_ylabel(cbar_label, fontsize=fontsize, labelpad=10)
     for label in cbar.ax.xaxis.get_ticklabels()[::2]:
         label.set_visible(False)
 
-    plt.grid(b=False)
+    plt.grid(visible=False)
 
     return ax
 
 
 def plot_som_histogram(
     bmu_list: List[Tuple[int, int]],
     n_rows: int,
@@ -131,15 +126,15 @@
         tick.label.set_fontsize(fontsize)
     for tick in ax.yaxis.get_major_ticks():
         tick.label.set_fontsize(fontsize)
 
     # to be compatible with plt.imshow:
     ax.invert_yaxis()
 
-    plt.grid(b=False)
+    plt.grid(visible=False)
 
     return ax
 
 
 def plot_umatrix(
     u_matrix: np.ndarray,
     n_rows: int,
```

## Comparing `susi-1.2.2/susi/SOMRegressor.py` & `susi-1.3.0/susi/SOMRegressor.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,8 @@
-"""SOMRegressor class.
-
-Copyright (c) 2019-2021 Felix M. Riese.
-All rights reserved.
-
-"""
+"""SOMRegressor class."""
 
 import numpy as np
 from sklearn.base import RegressorMixin
 
 from .SOMEstimator import SOMEstimator
```

## Comparing `susi-1.2.2/susi/SOMEstimator.py` & `susi-1.3.0/susi/SOMEstimator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,11 @@
-"""SOMEstimator class.
-
-Copyright (c) 2019-2021 Felix M. Riese.
-All rights reserved.
-
-"""
+"""SOMEstimator class."""
 
 from abc import ABC, abstractmethod
-from typing import List, Optional, Sequence, Tuple, Union
+from typing import Optional, Sequence, Tuple, Union
 
 import numpy as np
 from sklearn.base import BaseEstimator
 from sklearn.utils.validation import check_array, check_is_fitted
 from tqdm import tqdm
 
 from .SOMClustering import SOMClustering
@@ -248,17 +243,15 @@
         self._train_unsupervised_som()
         self._train_supervised_som()
 
         self.fitted_ = True
 
         return self
 
-    def predict(
-        self, X: Sequence, y: Optional[Sequence] = None
-    ) -> List[float]:
+    def predict(self, X: Sequence, y: Optional[Sequence] = None) -> np.ndarray:
         """Predict output of data X.
 
         Parameters
         ----------
         X : array-like matrix of shape = [n_samples, n_features]
             The prediction input samples.
         y : None, optional
@@ -342,15 +335,15 @@
 
         """
         return np.array([1.0])
 
     def _modify_weight_matrix_supervised(
         self,
         dist_weight_matrix: np.ndarray,
-        true_vector: Optional[np.array] = None,
+        true_vector: Optional[np.ndarray] = None,
         learning_rate: Optional[float] = None,
     ) -> np.ndarray:
         """Modify weights of the supervised SOM, either online or batch.
 
         Parameters
         ----------
         dist_weight_matrix : np.ndarray of float
@@ -402,16 +395,16 @@
             for it in tqdm(
                 range(self.n_iter_supervised),
                 desc="super",
                 **self.tqdm_params_,
             ):
 
                 # select one input vector & calculate best matching unit (BMU)
-                dp = self._get_random_datapoint()
-                bmu_pos = self.bmus_[dp]
+                dp_index = self._get_random_datapoint_index()
+                bmu_pos = self.bmus_[dp_index]
 
                 # calculate learning rate and neighborhood function
                 learning_rate = self._calc_learning_rate(
                     curr_it=it, mode=self.learn_mode_supervised
                 )
                 nbh_func = self._calc_neighborhood_func(
                     curr_it=it, mode=self.neighborhood_mode_supervised
@@ -419,15 +412,15 @@
 
                 # calculate distance weight matrix and update weights
                 dist_weight_matrix = self._get_nbh_distance_weight_matrix(
                     nbh_func, bmu_pos
                 )
                 self.super_som_ = self._modify_weight_matrix_supervised(
                     dist_weight_matrix=dist_weight_matrix,
-                    true_vector=self.y_[self.labeled_indices_][dp],
+                    true_vector=self.y_[self.labeled_indices_][dp_index],
                     learning_rate=learning_rate,
                 )
 
         elif self.train_mode_supervised == "batch":
             for it in tqdm(
                 range(self.n_iter_supervised),
                 desc="super",
@@ -500,26 +493,25 @@
         >>> som.fit(X, y)
         >>> estimation_map = som.get_estimation_map()
         >>> plt.imshow(np.squeeze(estimation_map,) cmap="viridis_r")
 
         """
         return self.super_som_
 
-    def _get_random_datapoint(self) -> np.ndarray:
-        """Find and return random datapoint from labeled dataset.
+    def _get_random_datapoint_index(self) -> int:
+        """Find and return random datapoint index from labeled dataset.
 
         Returns
         -------
-        random_datapoint : np.ndarray
-            Random datapoint from labeled dataset
+        int
+            Random datapoint index from labeled dataset
 
         """
-        random_datapoint = None
         if self.missing_label_placeholder is not None:
-            random_datapoint = np.random.choice(
+            random_datapoint: int = np.random.choice(
                 len(self.y_[self.labeled_indices_])
             )
         else:
             random_datapoint = np.random.randint(low=0, high=len(self.y_))
         return random_datapoint
 
     def _more_tags(self) -> dict:
```

## Comparing `susi-1.2.2/susi.egg-info/PKG-INFO` & `susi-1.3.0/susi.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,335 +1,346 @@
 Metadata-Version: 2.1
 Name: susi
-Version: 1.2.2
+Version: 1.3.0
 Summary: Python package for unsupervised, supervised and semi-supervised self-organizing maps (SOM)
 Home-page: https://github.com/felixriese/susi
 Author: Felix M. Riese
 Author-email: github@felixriese.de
 License: BSD-3-Clause
-Project-URL: Source, https://github.com/felixriese/susi
 Project-URL: Documentation, https://susi.readthedocs.io/en/latest/?badge=latest
+Project-URL: Source, https://github.com/felixriese/susi
 Project-URL: Tracker, https://github.com/felixriese/susi/issues
-Description: .. image:: https://badge.fury.io/py/susi.svg
-            :target: https://pypi.org/project/susi/
-            :alt: PyPi - Code Version
-        
-        .. image:: https://img.shields.io/pypi/pyversions/susi.svg
-            :target: https://pypi.org/project/susi/
-            :alt: PyPI - Python Version
-        
-        .. image:: https://travis-ci.com/felixriese/susi.svg?branch=master
-            :target: https://travis-ci.com/felixriese/susi
-            :alt: Travis.CI Status
-        
-        .. image:: https://readthedocs.org/projects/susi/badge/?version=latest
-            :target: https://susi.readthedocs.io/en/latest/?badge=latest
-            :alt: Documentation Status
-        
-        .. image:: https://codecov.io/gh/felixriese/susi/branch/master/graph/badge.svg
-            :target: https://codecov.io/gh/felixriese/susi
-            :alt: Codecov
-        
-        .. image:: https://api.codacy.com/project/badge/Grade/d304689a7364437db1ef998cf7765f5a
-        	:target: https://app.codacy.com/app/felixriese/susi
-        	:alt: Codacy Badge
-        
-        .. image:: https://anaconda.org/conda-forge/susi/badges/version.svg
-            :target: https://anaconda.org/conda-forge/susi
-            :alt: Conda-forge
-            
-        .. image:: https://requires.io/github/felixriese/susi/requirements.svg?branch=main
-             :target: https://requires.io/github/felixriese/susi/requirements/?branch=main
-             :alt: Requirements Status
-        
-        |
-        
-        .. image:: https://raw.githubusercontent.com/felixriese/susi/master/docs/_static/susi_logo_small.png
-            :target: https://github.com/felixriese/susi
-            :align: right
-            :alt: SuSi logo
-        
-        SuSi: Supervised Self-organizing maps in Python
-        ===============================================
-        
-        Python package for unsupervised, supervised and semi-supervised self-organizing maps (SOM)
-        
-        Description
-        -----------
-        
-        We present the SuSi package for Python.
-        It includes a fully functional SOM for unsupervised, supervised and semi-supervised tasks:
-        
-        - SOMClustering: Unsupervised SOM for clustering
-        - SOMRegressor: (Semi-)Supervised Regression SOM
-        - SOMClassifier: (Semi-)Supervised Classification SOM
-        
-        :License:
-            `3-Clause BSD license <LICENSE>`_
-        
-        :Author:
-            `Felix M. Riese <mailto:github@felixriese.de>`_
-        
-        :Citation:
-            see `Citation`_ and in the `bibtex <https://github.com/felixriese/susi/blob/main/bibliography.bib>`_ file
-        
-        :Documentation:
-            `Documentation <https://susi.readthedocs.io/en/latest/index.html>`_
-        
-        :Installation:
-            `Installation guidelines <https://susi.readthedocs.io/en/latest/install.html>`_
-        
-        :Paper:
-            `F. M. Riese, S. Keller and S. Hinz in Remote Sensing, 2020 <https://www.mdpi.com/2072-4292/12/1/7>`_
-        
-        
-        Installation
-        ------------
-        
-        Pip
-        ~~~
-        
-        .. code:: bash
-        
-            pip3 install susi
-        
-        Conda
-        ~~~~~
-        
-        .. code:: bash
-        
-            conda install -c conda-forge susi
-        
-        More information can be found in the `installation guidelines <https://susi.readthedocs.io/en/latest/install.html>`_.
-        
-        .. image:: https://static.pepy.tech/personalized-badge/susi?period=total&units=international_system&left_color=black&right_color=blue&left_text=Downloads
-        	:target: https://pepy.tech/project/susi
-        	:alt: Downloads
-        
-        Examples
-        --------
-        
-        A collection of code examples can be found in `the documentation <https://susi.readthedocs.io/en/latest/examples.html>`_.
-        Code examples as Jupyter Notebooks can be found here:
-        
-        * `examples/SOMClustering <https://github.com/felixriese/susi/blob/main/examples/SOMClustering.ipynb>`_
-        * `examples/SOMRegressor <https://github.com/felixriese/susi/blob/main/examples/SOMRegressor.ipynb>`_
-        * `examples/SOMRegressor_semisupervised <https://github.com/felixriese/susi/blob/main/examples/SOMRegressor_semisupervised.ipynb>`_
-        * `examples/SOMRegressor_multioutput <https://github.com/felixriese/susi/blob/main/examples/SOMRegressor_multioutput.ipynb>`_
-        * `examples/SOMClassifier <https://github.com/felixriese/susi/blob/main/examples/SOMClassifier.ipynb>`_
-        * `examples/SOMClassifier_semisupervised <https://github.com/felixriese/susi/blob/main/examples/SOMClassifier_semisupervised.ipynb>`_
-        
-        FAQs
-        -----
-        
-        - **How should I set the initial hyperparameters of a SOM?** For more details
-          on the hyperparameters, see in `documentation/hyperparameters
-          <https://susi.readthedocs.io/en/latest/hyperparameters.html>`_.
-        - **How can I optimize the hyperparameters?** The SuSi hyperparameters
-          can be optimized, for example, with `scikit-learn.model_selection.GridSearchCV
-          <https://scikit-learn.org/stable/modules/generated/sklearn.model_selection.GridSearchCV.html>`_,
-          since the SuSi package is developed according to several scikit-learn
-          guidelines.
-        
-        
-        ------------
-        
-        
-        Citation
-        --------
-        
-        The bibtex file including both references is available in `bibliography.bib
-        <https://github.com/felixriese/susi/blob/main/bibliography.bib>`_.
-        
-        **Paper:**
-        
-        F. M. Riese, S. Keller and S. Hinz, "Supervised and Semi-Supervised Self-Organizing
-        Maps for Regression and Classification Focusing on Hyperspectral Data",
-        *Remote Sensing*, vol. 12, no. 1, 2020. `DOI:10.3390/rs12010007
-        <https://doi.org/10.3390/rs12010007>`_
-        
-        .. code:: bibtex
-        
-            @article{riese2020supervised,
-                author = {Riese, Felix~M. and Keller, Sina and Hinz, Stefan},
-                title = {{Supervised and Semi-Supervised Self-Organizing Maps for
-                          Regression and Classification Focusing on Hyperspectral Data}},
-                journal = {Remote Sensing},
-                year = {2020},
-                volume = {12},
-                number = {1},
-                article-number = {7},
-                URL = {https://www.mdpi.com/2072-4292/12/1/7},
-                ISSN = {2072-4292},
-                DOI = {10.3390/rs12010007}
-            }
-        
-        **Code:**
-        
-        Felix M. Riese, "SuSi: SUpervised Self-organIzing maps in Python",
-        Zenodo, 2019. `DOI:10.5281/zenodo.2609130
-        <https://doi.org/10.5281/zenodo.2609130>`_
-        
-        .. image:: https://zenodo.org/badge/DOI/10.5281/zenodo.2609130.svg
-           :target: https://doi.org/10.5281/zenodo.2609130
-        
-        .. code:: bibtex
-        
-            @misc{riese2019susicode,
-                author = {Riese, Felix~M.},
-                title = {{SuSi: Supervised Self-Organizing Maps in Python}},
-                year = {2019},
-                DOI = {10.5281/zenodo.2609130},
-                publisher = {Zenodo},
-                howpublished = {\href{https://doi.org/10.5281/zenodo.2609130}{doi.org/10.5281/zenodo.2609130}}
-            }
-        
-        -------------
-        
-        License
-        -------
-        
-        This project is published under the `3-Clause BSD <LICENSE>`_ license.
-        
-        .. image:: https://img.shields.io/pypi/l/susi.svg
-            :target: https://github.com/felixriese/susi/blob/main/LICENSE
-            :alt: PyPI - License
-        
-        
-        Change Log
-        ==========
-        
-        [1.2.2] - 2021-12-11
-        --------------------
-        - [ADDED] Official support for Python 3.10.
-        - [REMOVED] Official support for Python 3.6 (will be deprecated end of 2021
-          anyways). It might still work, but will not be maintained on this version.
-        
-        [1.2.1] - 2021-10-19
-        --------------------
-        - [ADDED] Quantization error `get_quantization_error()`
-        
-        [1.2] - 2021-04-04
-        ------------------
-        - [ADDED] Landing page with vuepress.
-        - [ADDED] Conda-forge recipe.
-        - [ADDED] Function `SOMClassifier.predict_proba()`
-        - [ADDED] Example notebook for multi-output regression
-        - [CHANGED] Code formatting to black.
-        - [CHANGED] CI from travis to GitHub actions.
-        - [FIXED] Requirements in setup.py
-        
-        [1.1.2] - 2021-02-18
-        --------------------
-        - [ADDED] Python 3.9 support. Python 3.6 support will be removed soon.
-        - [CHANGED] Function names for private use now start with an underscore.
-        
-        [1.1.1] - 2020-11-18
-        --------------------
-        - [ADDED] New distance metric "spectralangle".
-        - [ADDED] FAQs.
-        - [ADDED] Separate between positional and keyword parameters.
-        - [ADDED] Plot script for neighborhood distance weight matrix.
-        - [FIXED] Added inherited members to code documentation.
-        
-        [1.1.0] - 2020-08-31
-        --------------------
-        - [ADDED] Logo.
-        - [ADDED] SOMPlots documentation.
-        - [REMOVED] Python 3.5 support. Now, only 3.6-3.8 are supported.
-        - [FIXED] Scikit-learn warnings regarding validation of positional arguments.
-        - [FIXED] Sphinx documentation warnings.
-        
-        [1.0.10] - 2020-04-21
-        ------------------------------------
-        - [ADDED] Support for Python 3.8.x.
-        - [ADDED] Test coverage and MultiOutput test.
-        - [CHANGED] Function `setPlaceholder` to `_set_placeholder`.
-        - [FIXED] Documentation links
-        
-        [1.0.9] - 2020-04-07
-        ------------------------
-        - [ADDED] Documentation of the hyperparameters.
-        - [ADDED] Plot scripts.
-        - [CHANGED] Structure of the module files.
-        
-        [1.0.8] - 2020-01-20
-        ------------------------
-        - [FIXED] Replaced scikit-learn `sklearn.utils.fixes.parallel_helper`, see #12.
-        
-        [1.0.7] - 2019-11-28
-        ------------------------
-        - [ADDED] Optional tqdm visualization of the SOM training
-        - [ADDED] New `init_mode_supervised` called `random_minmax`.
-        - [CHANGED] Official name of package changes from `SUSI` to `SuSi`.
-        - [CHANGED] Docstrings for functions are now according to guidelines.
-        - [FIXED] Semi-supervised classification handling, sample weights
-        - [FIXED] Supervised classification SOM initalization of `n_iter_supervised`
-        - [FIXED] Code refactored according to prospector
-        - [FIXED] Resolved bug in `get_datapoints_from_node()` for unsupervised SOM.
-        
-        [1.0.6] - 2019-09-11
-        ------------------------
-        - [ADDED] Semi-supervised abilities for classifier and regressor
-        - [ADDED] Example notebooks for semi-supervised applications
-        - [ADDED] Tests for example notebooks
-        - [CHANGED] Requirements for the SuSi package
-        - [REMOVED] Support for Python 3.4
-        - [FIXED] Code looks better in documentation with sphinx.ext.napoleon
-        
-        [1.0.5] - 2019-04-23
-        ------------------------
-        - [ADDED] PCA initialization of the SOM weights with 2 principal components
-        - [ADDED] Variable variance
-        - [CHANGED] Moved installation guidelines and examples to documentation
-        
-        [1.0.4] - 2019-04-21
-        ------------------------
-        - [ADDED] Batch algorithm for unsupervised and supervised SOM
-        - [ADDED] Calculation of the unified distance matrix (u-matrix)
-        - [FIXED] Added estimator_check of scikit-learn and fixed recognized issues
-        
-        [1.0.3] - 2019-04-09
-        ------------------------
-        - [ADDED] Link to arXiv paper
-        - [ADDED] Mexican-hat neighborhood distance weight
-        - [ADDED] Possibility for different initialization modes
-        - [CHANGED] Simplified initialization of estimators
-        - [FIXED] URLs and styles in documentation
-        - [FIXED] Colormap in Salinas example
-        
-        [1.0.2] - 2019-03-27
-        ------------------------
-        - [ADDED] Codecov, Codacy
-        - [CHANGED] Moved decreasing_rate() out of SOM classes
-        - [FIXED] Removed duplicate constructor for SOMRegressor, fixed fit() params
-        
-        [1.0.1] - 2019-03-26
-        ------------------------
-        - [ADDED] Config file for Travis
-        - [ADDED] Requirements for read-the-docs documentation
-        
-        [1.0.0] - 2019-03-26
-        ------------------------
-        - Initial release
-        
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 Provides-Extra: docs
+Provides-Extra: examples
 Provides-Extra: tests
 Provides-Extra: formatting
-Provides-Extra: examples
+License-File: LICENSE
+
+.. image:: https://badge.fury.io/py/susi.svg
+    :target: https://pypi.org/project/susi/
+    :alt: PyPi - Code Version
+
+.. image:: https://img.shields.io/pypi/pyversions/susi.svg
+    :target: https://pypi.org/project/susi/
+    :alt: PyPI - Python Version
+
+.. image:: https://travis-ci.com/felixriese/susi.svg?branch=master
+    :target: https://travis-ci.com/felixriese/susi
+    :alt: Travis.CI Status
+
+.. image:: https://readthedocs.org/projects/susi/badge/?version=latest
+    :target: https://susi.readthedocs.io/en/latest/?badge=latest
+    :alt: Documentation Status
+
+.. image:: https://codecov.io/gh/felixriese/susi/branch/master/graph/badge.svg
+    :target: https://codecov.io/gh/felixriese/susi
+    :alt: Codecov
+
+.. image:: https://api.codacy.com/project/badge/Grade/d304689a7364437db1ef998cf7765f5a
+	:target: https://app.codacy.com/app/felixriese/susi
+	:alt: Codacy Badge
+
+.. image:: https://anaconda.org/conda-forge/susi/badges/version.svg
+    :target: https://anaconda.org/conda-forge/susi
+    :alt: Conda-forge
+    
+.. image:: https://requires.io/github/felixriese/susi/requirements.svg?branch=main
+     :target: https://requires.io/github/felixriese/susi/requirements/?branch=main
+     :alt: Requirements Status
+
+|
+
+.. image:: https://raw.githubusercontent.com/felixriese/susi/master/docs/_static/susi_logo_small.png
+    :target: https://github.com/felixriese/susi
+    :align: right
+    :alt: SuSi logo
+
+SuSi: Supervised Self-organizing maps in Python
+===============================================
+
+Python package for unsupervised, supervised and semi-supervised self-organizing maps (SOM)
+
+Description
+-----------
+
+We present the SuSi package for Python.
+It includes a fully functional SOM for unsupervised, supervised and semi-supervised tasks:
+
+- SOMClustering: Unsupervised SOM for clustering
+- SOMRegressor: (Semi-)Supervised Regression SOM
+- SOMClassifier: (Semi-)Supervised Classification SOM
+
+:License:
+    `3-Clause BSD license <LICENSE>`_
+
+:Author:
+    `Felix M. Riese <mailto:github@felixriese.de>`_
+
+:Citation:
+    see `Citation`_ and in the `bibtex <https://github.com/felixriese/susi/blob/main/bibliography.bib>`_ file
+
+:Documentation:
+    `Documentation <https://susi.readthedocs.io/en/latest/index.html>`_
+
+:Installation:
+    `Installation guidelines <https://susi.readthedocs.io/en/latest/install.html>`_
+
+:Paper:
+    `F. M. Riese, S. Keller and S. Hinz in Remote Sensing, 2020 <https://www.mdpi.com/2072-4292/12/1/7>`_
+
+
+Installation
+------------
+
+Pip
+~~~
+
+.. code:: bash
+
+    pip3 install susi
+    
+.. image:: https://static.pepy.tech/personalized-badge/susi?period=total&units=international_system&left_color=black&right_color=blue&left_text=Downloads
+	:target: https://pepy.tech/project/susi
+	:alt: PyPi Downloads
+
+Conda
+~~~~~
+
+.. code:: bash
+
+    conda install -c conda-forge susi
+
+More information can be found in the `installation guidelines <https://susi.readthedocs.io/en/latest/install.html>`_.
+
+.. image:: https://img.shields.io/conda/dn/conda-forge/susi.svg
+	:target: https://anaconda.org/conda-forge/susi
+	:alt: Conda-Forge Downloads
+
+Examples
+--------
+
+A collection of code examples can be found in `the documentation <https://susi.readthedocs.io/en/latest/examples.html>`_.
+Code examples as Jupyter Notebooks can be found here:
+
+* `examples/SOMClustering <https://github.com/felixriese/susi/blob/main/examples/SOMClustering.ipynb>`_
+* `examples/SOMRegressor <https://github.com/felixriese/susi/blob/main/examples/SOMRegressor.ipynb>`_
+* `examples/SOMRegressor_semisupervised <https://github.com/felixriese/susi/blob/main/examples/SOMRegressor_semisupervised.ipynb>`_
+* `examples/SOMRegressor_multioutput <https://github.com/felixriese/susi/blob/main/examples/SOMRegressor_multioutput.ipynb>`_
+* `examples/SOMClassifier <https://github.com/felixriese/susi/blob/main/examples/SOMClassifier.ipynb>`_
+* `examples/SOMClassifier_semisupervised <https://github.com/felixriese/susi/blob/main/examples/SOMClassifier_semisupervised.ipynb>`_
+
+FAQs
+-----
+
+- **How should I set the initial hyperparameters of a SOM?** For more details
+  on the hyperparameters, see in `documentation/hyperparameters
+  <https://susi.readthedocs.io/en/latest/hyperparameters.html>`_.
+- **How can I optimize the hyperparameters?** The SuSi hyperparameters
+  can be optimized, for example, with `scikit-learn.model_selection.GridSearchCV
+  <https://scikit-learn.org/stable/modules/generated/sklearn.model_selection.GridSearchCV.html>`_,
+  since the SuSi package is developed according to several scikit-learn
+  guidelines.
+
+
+------------
+
+
+Citation
+--------
+
+The bibtex file including both references is available in `bibliography.bib
+<https://github.com/felixriese/susi/blob/main/bibliography.bib>`_.
+
+**Paper:**
+
+F. M. Riese, S. Keller and S. Hinz, "Supervised and Semi-Supervised Self-Organizing
+Maps for Regression and Classification Focusing on Hyperspectral Data",
+*Remote Sensing*, vol. 12, no. 1, 2020. `DOI:10.3390/rs12010007
+<https://doi.org/10.3390/rs12010007>`_
+
+.. code:: bibtex
+
+    @article{riese2020supervised,
+        author = {Riese, Felix~M. and Keller, Sina and Hinz, Stefan},
+        title = {{Supervised and Semi-Supervised Self-Organizing Maps for
+                  Regression and Classification Focusing on Hyperspectral Data}},
+        journal = {Remote Sensing},
+        year = {2020},
+        volume = {12},
+        number = {1},
+        article-number = {7},
+        URL = {https://www.mdpi.com/2072-4292/12/1/7},
+        ISSN = {2072-4292},
+        DOI = {10.3390/rs12010007}
+    }
+
+**Code:**
+
+Felix M. Riese, "SuSi: SUpervised Self-organIzing maps in Python",
+Zenodo, 2019. `DOI:10.5281/zenodo.2609130
+<https://doi.org/10.5281/zenodo.2609130>`_
+
+.. image:: https://zenodo.org/badge/DOI/10.5281/zenodo.2609130.svg
+   :target: https://doi.org/10.5281/zenodo.2609130
+
+.. code:: bibtex
+
+    @misc{riese2019susicode,
+        author = {Riese, Felix~M.},
+        title = {{SuSi: Supervised Self-Organizing Maps in Python}},
+        year = {2019},
+        DOI = {10.5281/zenodo.2609130},
+        publisher = {Zenodo},
+        howpublished = {\href{https://doi.org/10.5281/zenodo.2609130}{doi.org/10.5281/zenodo.2609130}}
+    }
+
+-------------
+
+License
+-------
+
+This project is published under the `3-Clause BSD <LICENSE>`_ license.
+
+.. image:: https://img.shields.io/pypi/l/susi.svg
+    :target: https://github.com/felixriese/susi/blob/main/LICENSE
+    :alt: PyPI - License
+
+
+Change Log
+==========
+
+[1.3.0] - 2023-07-08
+--------------------
+- [ADDED] Official support for Python 3.11.
+- [FIXED] Quantization error axis bug.
+- [REMOVED] Official support for Python 3.7 (deprecated in 2023). It might
+  still work, but will not be maintained on this version.
+
+[1.2.2] - 2021-12-11
+--------------------
+- [ADDED] Official support for Python 3.10.
+- [REMOVED] Official support for Python 3.6 (will be deprecated end of 2021
+  anyways). It might still work, but will not be maintained on this version.
+
+[1.2.1] - 2021-10-19
+--------------------
+- [ADDED] Quantization error `get_quantization_error()`
+
+[1.2] - 2021-04-04
+------------------
+- [ADDED] Landing page with vuepress.
+- [ADDED] Conda-forge recipe.
+- [ADDED] Function `SOMClassifier.predict_proba()`
+- [ADDED] Example notebook for multi-output regression
+- [CHANGED] Code formatting to black.
+- [CHANGED] CI from travis to GitHub actions.
+- [FIXED] Requirements in setup.py
+
+[1.1.2] - 2021-02-18
+--------------------
+- [ADDED] Python 3.9 support. Python 3.6 support will be removed soon.
+- [CHANGED] Function names for private use now start with an underscore.
+
+[1.1.1] - 2020-11-18
+--------------------
+- [ADDED] New distance metric "spectralangle".
+- [ADDED] FAQs.
+- [ADDED] Separate between positional and keyword parameters.
+- [ADDED] Plot script for neighborhood distance weight matrix.
+- [FIXED] Added inherited members to code documentation.
+
+[1.1.0] - 2020-08-31
+--------------------
+- [ADDED] Logo.
+- [ADDED] SOMPlots documentation.
+- [REMOVED] Python 3.5 support. Now, only 3.6-3.8 are supported.
+- [FIXED] Scikit-learn warnings regarding validation of positional arguments.
+- [FIXED] Sphinx documentation warnings.
+
+[1.0.10] - 2020-04-21
+------------------------------------
+- [ADDED] Support for Python 3.8.x.
+- [ADDED] Test coverage and MultiOutput test.
+- [CHANGED] Function `setPlaceholder` to `_set_placeholder`.
+- [FIXED] Documentation links
+
+[1.0.9] - 2020-04-07
+------------------------
+- [ADDED] Documentation of the hyperparameters.
+- [ADDED] Plot scripts.
+- [CHANGED] Structure of the module files.
+
+[1.0.8] - 2020-01-20
+------------------------
+- [FIXED] Replaced scikit-learn `sklearn.utils.fixes.parallel_helper`, see #12.
+
+[1.0.7] - 2019-11-28
+------------------------
+- [ADDED] Optional tqdm visualization of the SOM training
+- [ADDED] New `init_mode_supervised` called `random_minmax`.
+- [CHANGED] Official name of package changes from `SUSI` to `SuSi`.
+- [CHANGED] Docstrings for functions are now according to guidelines.
+- [FIXED] Semi-supervised classification handling, sample weights
+- [FIXED] Supervised classification SOM initalization of `n_iter_supervised`
+- [FIXED] Code refactored according to prospector
+- [FIXED] Resolved bug in `get_datapoints_from_node()` for unsupervised SOM.
+
+[1.0.6] - 2019-09-11
+------------------------
+- [ADDED] Semi-supervised abilities for classifier and regressor
+- [ADDED] Example notebooks for semi-supervised applications
+- [ADDED] Tests for example notebooks
+- [CHANGED] Requirements for the SuSi package
+- [REMOVED] Support for Python 3.4
+- [FIXED] Code looks better in documentation with sphinx.ext.napoleon
+
+[1.0.5] - 2019-04-23
+------------------------
+- [ADDED] PCA initialization of the SOM weights with 2 principal components
+- [ADDED] Variable variance
+- [CHANGED] Moved installation guidelines and examples to documentation
+
+[1.0.4] - 2019-04-21
+------------------------
+- [ADDED] Batch algorithm for unsupervised and supervised SOM
+- [ADDED] Calculation of the unified distance matrix (u-matrix)
+- [FIXED] Added estimator_check of scikit-learn and fixed recognized issues
+
+[1.0.3] - 2019-04-09
+------------------------
+- [ADDED] Link to arXiv paper
+- [ADDED] Mexican-hat neighborhood distance weight
+- [ADDED] Possibility for different initialization modes
+- [CHANGED] Simplified initialization of estimators
+- [FIXED] URLs and styles in documentation
+- [FIXED] Colormap in Salinas example
+
+[1.0.2] - 2019-03-27
+------------------------
+- [ADDED] Codecov, Codacy
+- [CHANGED] Moved decreasing_rate() out of SOM classes
+- [FIXED] Removed duplicate constructor for SOMRegressor, fixed fit() params
+
+[1.0.1] - 2019-03-26
+------------------------
+- [ADDED] Config file for Travis
+- [ADDED] Requirements for read-the-docs documentation
+
+[1.0.0] - 2019-03-26
+------------------------
+- Initial release
```

