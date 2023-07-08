# Comparing `tmp/dreimac-0.2.0.tar.gz` & `tmp/dreimac-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dreimac-0.2.0.tar", last modified: Mon May  8 16:30:17 2023, max compression
+gzip compressed data, was "dreimac-0.2.2.tar", last modified: Sat Jul  8 21:26:48 2023, max compression
```

## Comparing `dreimac-0.2.0.tar` & `dreimac-0.2.2.tar`

### file list

```diff
@@ -1,27 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:30:17.384883 dreimac-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11376 2023-05-08 16:28:38.000000 dreimac-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6460 2023-05-08 16:30:17.384883 dreimac-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4688 2023-05-08 16:28:38.000000 dreimac-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:30:17.384883 dreimac-0.2.0/dreimac/
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-05-08 16:28:38.000000 dreimac-0.2.0/dreimac/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-08 16:28:38.000000 dreimac-0.2.0/dreimac/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-05-08 16:28:38.000000 dreimac-0.2.0/dreimac/circularcoords.py
--rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-05-08 16:28:38.000000 dreimac-0.2.0/dreimac/combinatorial.py
--rw-r--r--   0 runner    (1001) docker     (123)     6231 2023-05-08 16:28:38.000000 dreimac-0.2.0/dreimac/emcoords.py
--rw-r--r--   0 runner    (1001) docker     (123)     8020 2023-05-08 16:28:38.000000 dreimac-0.2.0/dreimac/plotting_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5330 2023-05-08 16:28:38.000000 dreimac-0.2.0/dreimac/projectivecoords.py
--rw-r--r--   0 runner    (1001) docker     (123)    14987 2023-05-08 16:28:38.000000 dreimac-0.2.0/dreimac/toroidalcoords.py
--rw-r--r--   0 runner    (1001) docker     (123)    36173 2023-05-08 16:28:38.000000 dreimac-0.2.0/dreimac/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:30:17.384883 dreimac-0.2.0/dreimac.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6460 2023-05-08 16:30:17.000000 dreimac-0.2.0/dreimac.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-05-08 16:30:17.000000 dreimac-0.2.0/dreimac.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 16:30:17.000000 dreimac-0.2.0/dreimac.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-08 16:30:17.000000 dreimac-0.2.0/dreimac.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-08 16:30:17.000000 dreimac-0.2.0/dreimac.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 16:30:17.384883 dreimac-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-05-08 16:28:38.000000 dreimac-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:30:17.384883 dreimac-0.2.0/test/
--rw-r--r--   0 runner    (1001) docker     (123)     4549 2023-05-08 16:28:38.000000 dreimac-0.2.0/test/test_circular.py
--rw-r--r--   0 runner    (1001) docker     (123)      858 2023-05-08 16:28:38.000000 dreimac-0.2.0/test/test_combinatorial_number_system.py
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-08 16:28:38.000000 dreimac-0.2.0/test/test_library.py
--rw-r--r--   0 runner    (1001) docker     (123)     3042 2023-05-08 16:28:38.000000 dreimac-0.2.0/test/test_projective.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 21:26:48.284497 dreimac-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11376 2023-07-08 21:24:56.000000 dreimac-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5857 2023-07-08 21:26:48.284497 dreimac-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4880 2023-07-08 21:24:56.000000 dreimac-0.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 21:26:48.284497 dreimac-0.2.2/dreimac/
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-07-08 21:24:56.000000 dreimac-0.2.2/dreimac/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-08 21:24:56.000000 dreimac-0.2.2/dreimac/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-07-08 21:24:56.000000 dreimac-0.2.2/dreimac/circularcoords.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-07-08 21:24:56.000000 dreimac-0.2.2/dreimac/combinatorial.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12239 2023-07-08 21:24:56.000000 dreimac-0.2.2/dreimac/complexprojectivecoords.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7327 2023-07-08 21:24:56.000000 dreimac-0.2.2/dreimac/emcoords.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3710 2023-07-08 21:24:56.000000 dreimac-0.2.2/dreimac/lenscoords.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11253 2023-07-08 21:24:56.000000 dreimac-0.2.2/dreimac/plotting_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3658 2023-07-08 21:24:56.000000 dreimac-0.2.2/dreimac/projectivecoords.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14991 2023-07-08 21:24:56.000000 dreimac-0.2.2/dreimac/toroidalcoords.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54214 2023-07-08 21:24:56.000000 dreimac-0.2.2/dreimac/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 21:26:48.284497 dreimac-0.2.2/dreimac.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5857 2023-07-08 21:26:48.000000 dreimac-0.2.2/dreimac.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-07-08 21:26:48.000000 dreimac-0.2.2/dreimac.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 21:26:48.000000 dreimac-0.2.2/dreimac.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-08 21:26:48.000000 dreimac-0.2.2/dreimac.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-08 21:26:48.000000 dreimac-0.2.2/dreimac.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 21:26:48.284497 dreimac-0.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-07-08 21:24:56.000000 dreimac-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 21:26:48.284497 dreimac-0.2.2/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     4662 2023-07-08 21:24:56.000000 dreimac-0.2.2/test/test_circular.py
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-07-08 21:24:56.000000 dreimac-0.2.2/test/test_combinatorial_number_system.py
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-07-08 21:24:56.000000 dreimac-0.2.2/test/test_library.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3916 2023-07-08 21:24:56.000000 dreimac-0.2.2/test/test_projective.py
```

### Comparing `dreimac-0.2.0/LICENSE` & `dreimac-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dreimac-0.2.0/PKG-INFO` & `dreimac-0.2.2/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,132 +1,142 @@
 Metadata-Version: 2.1
 Name: dreimac
-Version: 0.2.0
-Summary: DREiMac: Dimension reduction with Eilenberg-MacLane coordinates
-Home-page: UNKNOWN
+Version: 0.2.2
+Summary: DREiMac: Dimensionality reduction with Eilenberg-MacLane coordinates
 Author: Jose A. Perea, Luis Scoccola, Chris Tralie
 Author-email: ctralie@alumni.princeton.edu
 License: Apache2
-Description: [![PyPI version](https://badge.fury.io/py/dreimac.svg)](https://badge.fury.io/py/dreimac)
-        [![Downloads](https://static.pepy.tech/badge/dreimac)](https://pepy.tech/project/dreimac)
-        [![codecov](https://codecov.io/gh/scikit-tda/dreimac/branch/master/graph/badge.svg)](https://codecov.io/gh/scikit-tda/dreimac)
-        [![License](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
-        
-        # DREiMac: Dimension Reduction with Eilenberg-MacLane Coordinates
-        
-        DREiMac is a library for topological data coordinatization, visualization, and dimensionality reduction.
-        Currently, DREiMac is able to find topology-preserving representations of point clouds taking values in the circle, in higher dimensional tori, and in the real projective space.
-        
-        In a few words, DREiMac takes as input a point cloud together with a topological feature of the point cloud (in the form of a persistent cohomology class), and returns a map from the point cloud to a well-understood topological space (a circle, a product of circles, or a projective space), which preserves the given topological feature in a precise sense.
-        For more information, please check the theory and examples in the [documentation](https://scikit-tda.org/DREiMac/index.html).
-        
-        ## Basic usage
-        
-        Here is a simple example; please check the Jupyter notebooks in the `notebooks` directory for further examples.
-        
-        ```python
-        # basic imports
-        from dreimac import CircularCoords
-        from persim import plot_diagrams
-        import matplotlib.pyplot as plt
-        import numpy as np
-        
-        # prepare plot with 4 subplots
-        f, (a0, a1, a2, a3) = plt.subplots(1, 4, width_ratios=[1, 1, 1, 0.2], figsize=(14,3))
-        
-        # 200 samples from a noisy circle
-        n_samples = 200
-        np.random.seed(0)
-        Z = np.random.random((n_samples, 2)) - 0.5
-        X = Z / np.linalg.norm(Z, axis=1).reshape((n_samples, 1)) + (np.random.random((n_samples, 2)) - 0.5) * 0.2
-        
-        # plot point cloud
-        a0.scatter(X[:,0], X[:,1], s=10)
-        a0.set_title("Input point cloud") ; a0.axis("off") ; a0.set_aspect("equal")
-        
-        # plot the persistence diagram, showing a single prominent class
-        cc = CircularCoords(X, n_landmarks=200)
-        plot_diagrams(cc.dgms_, title="Persistence diagram", ax=a1)
-        
-        # plot the data colored by the circle-valued map constructed by DREiMac
-        circular_coordinates = cc.get_coordinates()
-        a2.scatter(X[:,0], X[:,1], c=circular_coordinates, s=10, cmap="viridis")
-        a2.set_title("Input colored by circular coordinate") ; a2.axis("off") ; a2.set_aspect("equal")
-        
-        # plot colorbar
-        img = a3.imshow([[0,1]], cmap="viridis"); a3.set_visible(False)
-        cb = plt.colorbar(mappable=img,ticks=[0,0.5,1]) ; _ = cb.ax.set_yticklabels(["0","$\pi$","2$\pi$"])
-        ```
-        
-        ![output](https://user-images.githubusercontent.com/1679929/232109124-bf2653e5-6f91-409d-b972-7104b96b3430.png)
-        
-        ## More examples
-        
-        For Jupyter notebooks with more examples, please check the [documentation](https://scikit-tda.org/DREiMac/index.html) or this repository's [docs/notebooks](https://github.com/scikit-tda/DREiMac/tree/master/docs/notebooks) directory.
-        
-        ## Installing
-        
-        Make sure you are using Python 3.8 or 3.9.
-        DREiMac depends on the following python packages, which will be installed automatically when you install with pip:
-        `matplotlib`,
-        `numba`,
-        `numpy`,
-        `persim`,
-        `ripser`, and
-        `scipy`.
-        
-        ~~~~~ bash
-        pip install dreimac
-        ~~~~~
-        
-        ## Documentation and support
-        
-        You can find the documentation [here](https://scikit-tda.org/DREiMac/index.html), including the [API reference](https://scikit-tda.org/DREiMac/api.html).
-        If you have further questions, please [open an issue](https://github.com/scikit-tda/DREiMac/issues/new) and we will do our best to help you.
-        Please include as much information as possible, including your system's information, warnings, logs, screenshots, and anything else you think may be of use.
-        
-        ## Running the tests
-        
-        If you want to check that your machine is running DREiMac properly, you may run the tests by running the following commands from the root directory of a clone of this repository.
-        
-        ```bash
-        pip install pytest
-        pip install -r requirements.txt
-        pytest .
-        ```
-        
-        ## Contributing
-        
-        To contribute, you can fork the project, make your changes, and submit a pull request.
-        If you're looking for a way to contribute, you could consider:
-        * adding documentation to existing functionality;
-        * adding missing tests to improve coverage;
-        * adding a Jupyter notebook with a tutorial or demo;
-        * adding functionality and the corresponding documentation and tests;
-        * responding to a bug or feature request in the Github issues.
-        
-        ## Authors
-        
-        Jose A. Perea, Luis Scoccola, Chris Tralie
-        
-        ## Acknowledgements
-        
-        We thank Tom Mease for contributions and discussions.
-        
-        ## License
-        
-        This software is published under Apache License Version 2.0.
-        
-Keywords: topological data analysis,dimension reduction
-Platform: UNKNOWN
+Keywords: topological data analysis,dimensionality reduction
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: Intended Audience :: Healthcare Industry
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Requires-Python: >=3.8, <3.10
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: testing
 Provides-Extra: examples
+License-File: LICENSE
+
+[![PyPI version](https://badge.fury.io/py/dreimac.svg)](https://badge.fury.io/py/dreimac)
+[![Downloads](https://static.pepy.tech/badge/dreimac)](https://pepy.tech/project/dreimac)
+[![codecov](https://codecov.io/gh/scikit-tda/dreimac/branch/master/graph/badge.svg)](https://codecov.io/gh/scikit-tda/dreimac)
+[![License](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
+
+# DREiMac: Dimensionality Reduction with Eilenberg-MacLane Coordinates
+
+DREiMac is a library for topological data coordinatization, visualization, and dimensionality reduction.
+Currently, DREiMac is able to find topology-preserving representations of point clouds taking values in the circle, in higher dimensional tori, in the real and complex projective space, and in lens spaces.
+
+In a few words, DREiMac takes as input a point cloud together with a topological feature of the point cloud (in the form of a persistent cohomology class), and returns a map from the point cloud to a well-understood topological space (a circle, a product of circles, a projective space, or a lens space), which preserves the given topological feature in a precise sense.
+For more information, please check the theory and examples in the [documentation](https://scikit-tda.org/DREiMac/index.html).
+
+
+## Basic usage
+
+Here is a simple example; please check the Jupyter notebooks in the `notebooks` directory for further examples.
+
+```python
+# basic imports
+from dreimac import CircularCoords
+from persim import plot_diagrams
+import matplotlib.pyplot as plt
+import numpy as np
+
+# prepare plot with 4 subplots
+f, (a0, a1, a2, a3) = plt.subplots(1, 4, width_ratios=[1, 1, 1, 0.2], figsize=(14,3))
+
+# 200 samples from a noisy circle
+n_samples = 200
+np.random.seed(0)
+Z = np.random.random((n_samples, 2)) - 0.5
+X = Z / np.linalg.norm(Z, axis=1).reshape((n_samples, 1)) + (np.random.random((n_samples, 2)) - 0.5) * 0.2
+
+# plot point cloud
+a0.scatter(X[:,0], X[:,1], s=10)
+a0.set_title("Input point cloud") ; a0.axis("off") ; a0.set_aspect("equal")
+
+# plot the persistence diagram, showing a single prominent class
+cc = CircularCoords(X, n_landmarks=200)
+plot_diagrams(cc.dgms_, title="Persistence diagram", ax=a1)
+
+# plot the data colored by the circle-valued map constructed by DREiMac
+circular_coordinates = cc.get_coordinates()
+a2.scatter(X[:,0], X[:,1], c=circular_coordinates, s=10, cmap="viridis")
+a2.set_title("Input colored by circular coordinate") ; a2.axis("off") ; a2.set_aspect("equal")
+
+# plot colorbar
+img = a3.imshow([[0,1]], cmap="viridis"); a3.set_visible(False)
+cb = plt.colorbar(mappable=img,ticks=[0,0.5,1]) ; _ = cb.ax.set_yticklabels(["0","$\pi$","2$\pi$"])
+```
+
+![output](https://user-images.githubusercontent.com/1679929/232109124-bf2653e5-6f91-409d-b972-7104b96b3430.png)
+
+## More examples
+
+For Jupyter notebooks with more examples, please check the [documentation](https://scikit-tda.org/DREiMac/index.html) or this repository's [docs/notebooks](https://github.com/scikit-tda/DREiMac/tree/master/docs/notebooks) directory.
+
+## Installing
+
+Make sure you are using Python 3.8 or newer.
+DREiMac depends on the following python packages, which will be installed automatically when you install with pip:
+`matplotlib`,
+`numba`,
+`numpy`,
+`persim`,
+`ripser`, and
+`scipy`.
+
+To install the latest release:
+
+~~~~~ bash
+pip install dreimac
+~~~~~
+
+To install directly from GitHub:
+
+~~~~~ bash
+pip install git+https://github.com/scikit-tda/DREiMac.git
+~~~~~
+
+## Documentation and support
+
+You can find the documentation [here](https://scikit-tda.org/DREiMac/index.html), including the [API reference](https://scikit-tda.org/DREiMac/api.html).
+If you have further questions, please [open an issue](https://github.com/scikit-tda/DREiMac/issues/new) and we will do our best to help you.
+Please include as much information as possible, including your system's information, warnings, logs, screenshots, and anything else you think may be of use.
+
+## Running the tests
+
+If you want to check that your machine is running DREiMac properly, you may run the tests by running the following commands from the root directory of a clone of this repository.
+
+```bash
+pip install pytest
+pip install -r requirements.txt
+pytest .
+```
+
+## Contributing
+
+To contribute, you can fork the project, make your changes, and submit a pull request.
+If you're looking for a way to contribute, you could consider:
+* adding documentation to existing functionality;
+* adding missing tests to improve coverage;
+* adding a Jupyter notebook with a tutorial or demo;
+* adding functionality and the corresponding documentation and tests;
+* responding to a bug or feature request in the Github issues.
+
+## Authors
+
+Jose A. Perea, Luis Scoccola, Chris Tralie
+
+## Acknowledgements
+
+We thank Tom Mease for contributions and discussions.
+
+## License
+
+This software is published under Apache License Version 2.0.
```

### Comparing `dreimac-0.2.0/README.md` & `dreimac-0.2.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 [![PyPI version](https://badge.fury.io/py/dreimac.svg)](https://badge.fury.io/py/dreimac)
 [![Downloads](https://static.pepy.tech/badge/dreimac)](https://pepy.tech/project/dreimac)
 [![codecov](https://codecov.io/gh/scikit-tda/dreimac/branch/master/graph/badge.svg)](https://codecov.io/gh/scikit-tda/dreimac)
 [![License](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 
-# DREiMac: Dimension Reduction with Eilenberg-MacLane Coordinates
+# DREiMac: Dimensionality Reduction with Eilenberg-MacLane Coordinates
 
 DREiMac is a library for topological data coordinatization, visualization, and dimensionality reduction.
-Currently, DREiMac is able to find topology-preserving representations of point clouds taking values in the circle, in higher dimensional tori, and in the real projective space.
+Currently, DREiMac is able to find topology-preserving representations of point clouds taking values in the circle, in higher dimensional tori, in the real and complex projective space, and in lens spaces.
 
-In a few words, DREiMac takes as input a point cloud together with a topological feature of the point cloud (in the form of a persistent cohomology class), and returns a map from the point cloud to a well-understood topological space (a circle, a product of circles, or a projective space), which preserves the given topological feature in a precise sense.
+In a few words, DREiMac takes as input a point cloud together with a topological feature of the point cloud (in the form of a persistent cohomology class), and returns a map from the point cloud to a well-understood topological space (a circle, a product of circles, a projective space, or a lens space), which preserves the given topological feature in a precise sense.
 For more information, please check the theory and examples in the [documentation](https://scikit-tda.org/DREiMac/index.html).
 
+
 ## Basic usage
 
 Here is a simple example; please check the Jupyter notebooks in the `notebooks` directory for further examples.
 
 ```python
 # basic imports
 from dreimac import CircularCoords
@@ -53,27 +54,35 @@
 
 ## More examples
 
 For Jupyter notebooks with more examples, please check the [documentation](https://scikit-tda.org/DREiMac/index.html) or this repository's [docs/notebooks](https://github.com/scikit-tda/DREiMac/tree/master/docs/notebooks) directory.
 
 ## Installing
 
-Make sure you are using Python 3.8 or 3.9.
+Make sure you are using Python 3.8 or newer.
 DREiMac depends on the following python packages, which will be installed automatically when you install with pip:
 `matplotlib`,
 `numba`,
 `numpy`,
 `persim`,
 `ripser`, and
 `scipy`.
 
+To install the latest release:
+
 ~~~~~ bash
 pip install dreimac
 ~~~~~
 
+To install directly from GitHub:
+
+~~~~~ bash
+pip install git+https://github.com/scikit-tda/DREiMac.git
+~~~~~
+
 ## Documentation and support
 
 You can find the documentation [here](https://scikit-tda.org/DREiMac/index.html), including the [API reference](https://scikit-tda.org/DREiMac/api.html).
 If you have further questions, please [open an issue](https://github.com/scikit-tda/DREiMac/issues/new) and we will do our best to help you.
 Please include as much information as possible, including your system's information, warnings, logs, screenshots, and anything else you think may be of use.
 
 ## Running the tests
```

### Comparing `dreimac-0.2.0/dreimac/circularcoords.py` & `dreimac-0.2.2/dreimac/circularcoords.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,11 @@
 from .utils import PartUnity
 from .toroidalcoords import ToroidalCoords
 
 
-"""#########################################
-        Main Circular Coordinates Class
-#########################################"""
-
-
 class CircularCoords(ToroidalCoords):
     """
     Object that performs circular coordinates via persistent cohomology of
     sparse filtrations (Jose Perea 2020).
 
     Parameters
     ----------
```

### Comparing `dreimac-0.2.0/dreimac/combinatorial.py` & `dreimac-0.2.2/dreimac/combinatorial.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,28 +13,28 @@
             lookup_table[i, l] = comb(i, l, exact=True)
 
     return lookup_table
     
 def number_of_simplices_of_dimension(dimension, n_vertices, lookup_table):
     return lookup_table[n_vertices,dimension+1]
 
-@jit
+@jit(nopython=True)
 def combinatorial_number_system_forward(
     oriented_simplex: np.ndarray, lookup_table: np.ndarray
 ):
     dimension = len(oriented_simplex) - 1
     res = 0
     for l in range(dimension + 1):
         res += lookup_table[oriented_simplex[l], l + 1]
     return res
 
 
-@jit
+@jit(nopython=True)
 def combinatorial_number_system_d1_forward(v0: int, v1: int, lookup_table: np.ndarray):
     return lookup_table[v0, 1] + lookup_table[v1, 2]
 
 
-@jit
+@jit(nopython=True)
 def combinatorial_number_system_d2_forward(
     v0: int, v1: int, v2: int, lookup_table: np.ndarray
 ):
     return lookup_table[v0, 1] + lookup_table[v1, 2] + lookup_table[v2, 3]
```

### Comparing `dreimac-0.2.0/dreimac/emcoords.py` & `dreimac-0.2.2/dreimac/emcoords.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,57 +15,77 @@
         Perform persistent homology on the landmarks, store distance
         from the landmarks to themselves and to the rest of the points,
         and sort persistence diagrams and cocycles in decreasing order of persistence
 
         Parameters
         ----------
         X: ndarray(N, d)
-            A point cloud with N points in d dimensions
+            A point cloud with N points in d dimensions, or a matrix of distances from N points to d points.
+            See distance_matrix, below, for a description of the second scenario.
         n_landmarks: int
             Number of landmarks to use
         distance_matrix: boolean
-            If true, treat X as a distance matrix instead of a point cloud
+            If true, treat X as a distance matrix instead of a point cloud.
+            If X is square, then the i-th row should represent the same point as the i-th column, meaning
+            that the matrix should be symmetric.
+            If X is not square, then it should have more columns than rows (i.e., N > d).
+            Moreover, if i < N, the i-th row should represent the same point as the i-th column.
+            When X is not square, the rows of X are interpreted as a subsample and the columns as all available points; thus
+            X represents the distance from the points in the subsample to all available points.
         prime : int
             Field coefficient with which to compute rips on landmarks
         maxdim : int
-            Maximum dimension of homology.  Only dimension 1 is needed for circular coordinates,
-            but it may be of interest to see other dimensions (e.g. for a torus)
+            Maximum dimension of homology. 
+
         """
         assert maxdim >= 1
         self.verbose = verbose
         self.X_ = X
         if verbose:
             tic = time.time()
             print("Doing TDA...")
+        if distance_matrix is False:
+            ripser_metric_input = X 
+        elif X.shape[0] == X.shape[1]:
+            ripser_metric_input = X 
+        else:
+            ripser_metric_input = X[:,:X.shape[0]]
         res = ripser(
-            X,
+            ripser_metric_input,
             distance_matrix=distance_matrix,
             coeff=prime,
             maxdim=maxdim,
             n_perm=n_landmarks,
             do_cocycles=True,
         )
         if verbose:
             print("Elapsed time persistence: %.3g seconds" % (time.time() - tic))
         self.prime_ = prime
         self.dgms_ = res["dgms"]
-        self.dist_land_data_ = res["dperm2all"]
-        self.coverage_ = np.max(np.min(self.dist_land_data_, 1))
         self.idx_land_ = res["idx_perm"]
+        self.n_landmarks_ = len(self.idx_land_)
+        #self.dist_land_data_ = res["dperm2all"]
+        if distance_matrix is False:
+            self.dist_land_data_ = res["dperm2all"]
+        elif X.shape[0] == X.shape[1]:
+            self.dist_land_data_ = res["dperm2all"]
+        else:
+            self.dist_land_data_ = X[self.idx_land_,:]
+        self.coverage_ = np.max(np.min(self.dist_land_data_, 1))
         self.dist_land_land_ = self.dist_land_data_[:, self.idx_land_]
         self.cocycles_ = res["cocycles"]
         # Sort persistence diagrams in descending order of persistence
-        idxs = np.argsort(self.dgms_[1][:, 0] - self.dgms_[1][:, 1])
-        self.dgms_[1] = self.dgms_[1][idxs, :]
-        self.dgm1_lifetime = np.array(self.dgms_[1])
-        self.dgm1_lifetime[:, 1] -= self.dgm1_lifetime[:, 0]
-        self.cocycles_[1] = [self.cocycles_[1][idx] for idx in idxs]
+        for i in range(1, maxdim+1):
+            idxs = np.argsort(self.dgms_[i][:, 0] - self.dgms_[i][:, 1])
+            self.dgms_[i] = self.dgms_[i][idxs, :]
+            dgm_lifetime = np.array(self.dgms_[i])
+            dgm_lifetime[:, 1] -= dgm_lifetime[:, 0]
+            self.cocycles_[i] = [self.cocycles_[i][idx] for idx in idxs]
         CohomologyUtils.reindex_cocycles(self.cocycles_, self.idx_land_, X.shape[0])
 
-        self.n_landmarks_ = n_landmarks
         self.type_ = "emcoords"
 
     def get_representative_cocycle(self, cohomology_class, homological_dimension):
         """
         Compute the representative cocycle, given a list of cohomology classes
 
         Parameters
```

### Comparing `dreimac-0.2.0/dreimac/plotting_utils.py` & `dreimac-0.2.2/dreimac/plotting_utils.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import warnings
 import numpy as np
 import matplotlib.pyplot as plt
 from matplotlib.offsetbox import OffsetImage, AnnotationBbox
 
+
 class PlotUtils:
     """
     Plotting utilities for DREiMac's output.
 
     """
 
     @staticmethod
@@ -26,18 +27,21 @@
             If given, plot on those axes, otherwise plot
             on current axes by calling gca()
 
         """
         # https://stackoverflow.com/questions/22566284/matplotlib-how-to-plot-images-instead-of-points
 
         ax = ax or plt.gca()
+        min_color = np.min(P)
+        max_color = np.max(P)
         for i in range(P.shape[0]):
             patch = np.reshape(P[i, :], (dim, dim))
             x, y = X[i, :]
             im = OffsetImage(patch, zoom=zoom, cmap="gray")
+            im.get_children()[0].set_clim(vmin=min_color, vmax=max_color)
             ab = AnnotationBbox(im, (x, y), xycoords="data", frameon=False)
             ax.add_artist(ab)
         ax.update_datalim(X)
         ax.autoscale()
         ax.set_xticks([])
         ax.set_yticks([])
         return ax
@@ -95,26 +99,156 @@
             ec="c",
             width=0,
         )
         ax.set_facecolor((0.35, 0.35, 0.35))
         return ax
 
     @staticmethod
+    def plot_2sphere_boundary(ax=None):
+        """
+        Plot the boundary of two sphere hemispheres
+
+        Parameters
+        ----------
+        ax : matplotlib axes, optional
+            If given, plot on those axes, otherwise plot
+            on current axes by calling gca()
+
+        """
+
+        second_circle_offset = 2.5
+        ax = ax or plt.gca()
+        t = np.linspace(0, 2 * np.pi, 200)
+        ax.plot(np.cos(t), np.sin(t), "c")
+        ax.plot(np.cos(t) + second_circle_offset, np.sin(t), "c")
+        ax.axis("equal")
+
+        ax.arrow(
+            0, 0.9, 0, 0.001, head_width=0.15, head_length=0.2, fc="c", ec="c", width=0
+        )
+        ax.arrow(
+            second_circle_offset,
+            1.1,
+            0,
+            -0.001,
+            head_width=0.15,
+            head_length=0.2,
+            fc="c",
+            ec="c",
+            width=0,
+        )
+
+        ax.arrow(
+            0,
+            -0.9,
+            0,
+            -0.001,
+            head_width=0.15,
+            head_length=0.2,
+            fc="c",
+            ec="c",
+            width=0,
+        )
+        ax.arrow(
+            second_circle_offset,
+            -1.1,
+            0,
+            0.001,
+            head_width=0.15,
+            head_length=0.2,
+            fc="c",
+            ec="c",
+            width=0,
+        )
+
+        ax.arrow(
+            0.9, 0, 0.001, 0, head_width=0.15, head_length=0.2, fc="c", ec="c", width=0
+        )
+        ax.arrow(
+            second_circle_offset + 1.1,
+            0,
+            -0.001,
+            0,
+            head_width=0.15,
+            head_length=0.2,
+            fc="c",
+            ec="c",
+            width=0,
+        )
+
+        ax.arrow(
+            -0.9,
+            0,
+            -0.001,
+            0,
+            head_width=0.15,
+            head_length=0.2,
+            fc="c",
+            ec="c",
+            width=0,
+        )
+        ax.arrow(
+            second_circle_offset - 1.1,
+            0,
+            0.001,
+            0,
+            head_width=0.15,
+            head_length=0.2,
+            fc="c",
+            ec="c",
+            width=0,
+        )
+
+        ax.set_facecolor((0.35, 0.35, 0.35))
+
+        return ax
+
+    @staticmethod
+    def plot_3sphere_mesh(n_parallels = 10, n_meridians = 20, alpha=0.1, ax=None):
+        """
+        Draw a spherical mesh in 3D around the unit sphere.
+
+        Parameters
+        ----------
+        n_parallels : int
+            How many parallels to draw.
+
+        n_meridians : int
+            How many meridians to draw.
+
+        alpha : float
+            Opacity of the mesh. Must be between 0 and 1.
+
+        ax : matplotlib axes, optional
+            If given, plot on those axes, otherwise plot
+            on current axes by calling gca()
+
+        """
+
+        ax = ax or plt.gca()
+        u, v = np.mgrid[0 : 2 * np.pi : n_meridians * 1j, 0 : np.pi : n_parallels * 1j]
+        x = np.cos(u) * np.sin(v)
+        y = np.sin(u) * np.sin(v)
+        z = np.cos(v)
+        ax.plot_wireframe(x, y, z, color="black", alpha=alpha)
+        return ax
+
+    @staticmethod
     def set_axes_equal(ax):
-        # taken from https://stackoverflow.com/a/31364297/2171328
         """
         Make axes of 3D plot have equal scale so that spheres appear as spheres,
         cubes as cubes, etc..  This is one possible solution to Matplotlib's
         ax.set_aspect('equal') and ax.axis('equal') not working for 3D.
 
         Parameters
         ----------
-          ax: a matplotlib axis, e.g., as output from plt.gca().
+        ax : a matplotlib axis, e.g., as output from plt.gca().
 
         """
+        # taken from https://stackoverflow.com/a/31364297/2171328
 
         x_limits = ax.get_xlim3d()
         y_limits = ax.get_ylim3d()
         z_limits = ax.get_zlim3d()
 
         x_range = abs(x_limits[1] - x_limits[0])
         x_middle = np.mean(x_limits)
@@ -141,14 +275,15 @@
         ----------
         S : ndarray (N, 2)
             An Nx2 array of N points to plot on RP2
         f : ndarray (N) or ndarray (N, 3)
             A function with which to color the points, or a list of colors
 
         """
+
         def _plot_rp2_circle(
             ax, arrowcolor="c", facecolor=(0.15, 0.15, 0.15), do_arrows=True, pad=1.1
         ):
             """
             Plot a circle with arrows showing the identifications for RP2.
             Set an equal aspect ratio and get rid of the axis ticks, since
             they are clear from the circle
@@ -243,8 +378,7 @@
         if draw_sphere:
             u, v = np.mgrid[0 : 2 * np.pi : 20j, 0 : np.pi : 20j]
             ax.set_aspect("equal")
             x = np.cos(u) * np.sin(v)
             y = np.sin(u) * np.sin(v)
             z = np.cos(v)
             ax.plot_wireframe(x, y, z, color="k")
-
```

### Comparing `dreimac-0.2.0/dreimac/toroidalcoords.py` & `dreimac-0.2.2/dreimac/toroidalcoords.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import numpy as np
 import scipy
 from numba import jit
 import scipy.sparse as sparse
 from scipy.sparse.linalg import lsqr
-from scipy.optimize import LinearConstraint, milp, linprog
+from scipy.optimize import LinearConstraint, milp
 from .utils import PartUnity, CircleMapUtils, CohomologyUtils
 from .emcoords import EMCoords
 from .combinatorial import (
     combinatorial_number_system_table,
     combinatorial_number_system_d1_forward,
 )
 
@@ -124,15 +124,15 @@
         ]
 
         if check_cocycle_condition:
             delta1 = None
             fixed_cocycles = []
 
             for class_idx, cocycle_as_vector in enumerate(integer_cocycles_as_vectors):
-                is_cocycle, _ = _is_cocycle(
+                is_cocycle, _ = _is_one_cocycle(
                     cocycle_as_vector,
                     dist_land_land,
                     rips_threshold,
                     self.cns_lookup_table_,
                 )
                 if is_cocycle:
                     fixed_cocycles.append(cocycle_as_vector)
@@ -140,22 +140,24 @@
                     delta1 = (
                         delta1
                         if delta1
                         else CohomologyUtils.make_delta1_compact(
                             dist_land_land, rips_threshold, self.cns_lookup_table_
                         )
                     )
+
                     d1cocycle = delta1 @ cocycle_as_vector.T
 
                     y = d1cocycle // self.prime_
 
-                    constraints = LinearConstraint(delta1, y, y, keep_feasible=True)
+                    constraints = LinearConstraint(delta1, y, y)
                     n_edges = delta1.shape[1]
-                    objective = np.zeros((n_edges), dtype=int)
-                    integrality = np.ones((n_edges), dtype=int)
+                    objective = np.zeros((n_edges))
+                    integrality = np.ones((n_edges))
+
                     optimizer_solution = milp(
                         objective,
                         integrality=integrality,
                         constraints=constraints,
                     )
 
                     if not optimizer_solution["success"]:
@@ -234,15 +236,15 @@
     n_edges = (n_points * (n_points - 1)) // 2
 
     max_n_entries = n_edges
     rows = np.empty((max_n_entries,), dtype=int)
     columns = np.empty((max_n_entries,), dtype=int)
     values = np.empty((max_n_entries,), dtype=float)
 
-    @jit(fastmath=True)
+    @jit(fastmath=True, nopython=True)
     def _make_inner_product_get_row_columns_values(
         dist_mat: np.ndarray,
         threshold: float,
         lookup_table: np.ndarray,
         n_points: int,
         rows: np.ndarray,
         columns: np.ndarray,
@@ -283,15 +285,15 @@
     dist_mat,
     threshold,
     lookup_table,
 ):
     n_points = integral.shape[0]
     theta_matrix = np.zeros((n_points, n_points))
 
-    @jit(fastmath=True)
+    @jit(fastmath=True, nopython=True)
     def _cocycle_to_matrix(
         dist_mat: np.ndarray,
         threshold: float,
         lookup_table: np.ndarray,
         n_points: int,
         theta_matrix: np.ndarray,
     ):
@@ -305,16 +307,16 @@
 
     class_map = integral[membership_function].copy()
     for i in range(class_map.shape[0]):
         class_map[i] += theta_matrix[membership_function[i], :].dot(part_unity[:, i])
     return np.mod(2 * np.pi * class_map, 2 * np.pi)
 
 
-@jit(fastmath=True)
-def _is_cocycle(
+@jit(fastmath=True, nopython=True)
+def _is_one_cocycle(
     cochain: np.ndarray,
     dist_mat: np.ndarray,
     threshold: float,
     lookup_table: np.ndarray,
 ):
     is_cocycle = True
     first_failure = np.inf
```

### Comparing `dreimac-0.2.0/dreimac/utils.py` & `dreimac-0.2.2/dreimac/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,20 @@
 """
 Programmer: Chris Tralie (ctralie@alumni.princeton.edu) and Luis Scoccola
 Purpose: To provide a number of utility functions, including
 - Quickly computing all pairs self-similarity and cross-similarity matrices
 - Doing "greedy permutations" 
 - Some relevant geometric examples for tests
 """
+import time
 import numpy as np
 import scipy.sparse as sparse
+from scipy.spatial import KDTree
+from scipy.sparse import csr_matrix
+from scipy.sparse.csgraph import shortest_path
 from numba import jit
 from .combinatorial import (
     combinatorial_number_system_forward,
     combinatorial_number_system_d1_forward,
     combinatorial_number_system_d2_forward,
     number_of_simplices_of_dimension,
 )
@@ -149,14 +153,81 @@
             idx = np.argmax(ds)
             perm[i] = idx
             lambdas[i] = ds[idx]
             ds = np.minimum(ds, D[idx, :])
         DLandmarks = D[perm, :]
         return {"perm": perm, "lambdas": lambdas, "DLandmarks": DLandmarks}
 
+    @staticmethod
+    def landmark_geodesic_distance(X, n_landmarks, n_neighbors):
+        """
+        Get a minmax sample of Euclidean point cloud using an approximation of the geodesic distance.
+        Return the geodesic distance from the sample (landmarks) to the rest of the points.
+
+        Parameters
+        ----------
+        X : ndarray(n,d)
+            Point cloud of n points in d-dimensional Euclidean space.
+        n_landmarks : int
+            How many landmarks to sample.
+        n_neighbors : int
+            How many neighbors to use to compute the nearest neighbors graph used to approximate
+            the geodesic distance.
+
+        Return
+        ------
+        dist_landmarks_points : ndarray(n_landmarks,n)
+            Geodesic distance from landmarks to the rest of the points.
+            The first n_landmarks columns represent the landmarks, and are in the same order as landmarks.
+            The rest of the columns represent the rest of the data points.
+            The permutation that reorders the rows of X to correspond to the columns of dist_landmarks_points is
+            given by perm_all_points.
+
+        perm_all_points : ndarray(n)
+            Permutation of [0, ..., n-1] which makes the rows of X correspond to the columns of dist_landmarks_points.
+
+        """
+        assert n_landmarks <= X.shape[0]
+        assert n_neighbors <= X.shape[0]
+
+        spatial_tree = KDTree(X)
+        distances_nn, indices_nn = spatial_tree.query(X, k=n_neighbors)
+        # https://github.com/scikit-learn/scikit-learn/blob/364c77e047ca08a95862becf40a04fe9d4cd2c98/sklearn/neighbors/_base.py#L997
+        n_queries = X.shape[0]
+        n_nonzero = n_queries * n_neighbors
+        indptr = np.arange(0, n_nonzero + 1, n_neighbors)
+        kneighbors_graph = csr_matrix(
+            (distances_nn.ravel(), indices_nn.ravel(), indptr),
+            shape=(n_queries, n_queries),
+        )
+
+        # furthest point sampling
+        n_points = X.shape[0]
+        perm = np.zeros(n_landmarks, dtype=np.int64)
+        lambdas = np.zeros(n_landmarks)
+        ds = shortest_path(kneighbors_graph, indices=0, directed=False)
+        D = np.zeros((n_landmarks, n_points))
+        D[0, :] = ds
+        for i in range(1, n_landmarks):
+            idx = np.argmax(ds)
+            perm[i] = idx
+            lambdas[i] = ds[idx]
+            thisds = shortest_path(kneighbors_graph, indices=idx, directed=False)
+            D[i, :] = thisds
+            ds = np.minimum(ds, thisds)
+
+        perm_rest_points = np.setdiff1d(
+            np.arange(0, n_points, dtype=int), perm, assume_unique=True
+        )
+        perm_all_points = np.concatenate((perm, perm_rest_points))
+
+        dist_landmarks_points = D[:, perm_all_points]
+
+        return dist_landmarks_points, perm_all_points
+
 
 class CohomologyUtils:
     @staticmethod
     def lift_to_integer_cocycle(cocycle, prime):
         """
         Lift the given cocycle with values in a prime field to a cocycle with integer coefficients.
 
@@ -243,19 +314,19 @@
 
     @staticmethod
     def make_delta0(dist_mat: np.ndarray, threshold: float, lookup_table: np.ndarray):
         n_points = dist_mat.shape[0]
         n_edges = (n_points * (n_points - 1)) // 2
 
         max_n_entries = 2 * n_edges
-        rows = np.empty((max_n_entries,), dtype=int)
-        columns = np.empty((max_n_entries,), dtype=int)
+        rows = np.empty((max_n_entries,), dtype=np.int32)
+        columns = np.empty((max_n_entries,), dtype=np.int32)
         values = np.empty((max_n_entries,), dtype=float)
 
-        @jit(fastmath=True)
+        @jit(fastmath=True, nopython=True)
         def _delta0_get_row_columns_values(
             dist_mat: np.ndarray,
             threshold: float,
             lookup_table: np.ndarray,
             n_points: int,
             rows: np.ndarray,
             columns: np.ndarray,
@@ -291,19 +362,19 @@
     @staticmethod
     def make_delta1(dist_mat: np.ndarray, threshold: float, lookup_table: np.ndarray):
         n_points = dist_mat.shape[0]
         n_edges = (n_points * (n_points - 1)) // 2
         n_faces = number_of_simplices_of_dimension(2, n_points, lookup_table)
 
         max_n_entries = 3 * n_faces
-        rows = np.empty((max_n_entries,), dtype=int)
-        columns = np.empty((max_n_entries,), dtype=int)
+        rows = np.empty((max_n_entries,), dtype=np.int32)
+        columns = np.empty((max_n_entries,), dtype=np.int32)
         values = np.empty((max_n_entries,), dtype=float)
 
-        @jit(fastmath=True)
+        @jit(fastmath=True, nopython=True)
         def _delta1_get_row_columns_values(
             dist_mat: np.ndarray,
             threshold: float,
             lookup_table: np.ndarray,
             n_points: int,
             rows: np.ndarray,
             columns: np.ndarray,
@@ -378,19 +449,19 @@
         fewer rows.
         """
         n_points = dist_mat.shape[0]
         n_edges = (n_points * (n_points - 1)) // 2
         n_faces = number_of_simplices_of_dimension(2, n_points, lookup_table)
 
         max_n_entries = 3 * n_faces
-        rows = np.empty((max_n_entries,), dtype=int)
-        columns = np.empty((max_n_entries,), dtype=int)
+        rows = np.empty((max_n_entries,), dtype=np.int32)
+        columns = np.empty((max_n_entries,), dtype=np.int32)
         values = np.empty((max_n_entries,), dtype=float)
 
-        @jit(fastmath=True)
+        @jit(fastmath=True, nopython=True)
         def _delta1_get_row_columns_values(
             dist_mat: np.ndarray,
             threshold: float,
             lookup_table: np.ndarray,
             n_points: int,
             rows: np.ndarray,
             columns: np.ndarray,
@@ -452,14 +523,115 @@
         # print(max_n_entries)
 
         return sparse.csr_array(
             (values[:n_entries], (rows[:n_entries], columns[:n_entries])),
             shape=(n_actual_faces, n_edges),
         )
 
+    @staticmethod
+    def make_delta2_compact(
+        dist_mat: np.ndarray, threshold: float, lookup_table: np.ndarray
+    ):
+        """
+        Like [make_delta1_compact] but for delta2.
+        """
+        n_points = dist_mat.shape[0]
+        n_faces = number_of_simplices_of_dimension(2, n_points, lookup_table)
+        n_three_simplices = number_of_simplices_of_dimension(3, n_points, lookup_table)
+
+        max_n_entries = 4 * n_three_simplices
+        rows = np.empty((max_n_entries,), dtype=np.int32)
+        columns = np.empty((max_n_entries,), dtype=np.int32)
+        values = np.empty((max_n_entries,), dtype=float)
+
+        @jit(fastmath=True, nopython=True)
+        def _delta2_get_row_columns_values(
+            dist_mat: np.ndarray,
+            threshold: float,
+            lookup_table: np.ndarray,
+            n_points: int,
+            rows: np.ndarray,
+            columns: np.ndarray,
+            values: np.ndarray,
+        ):
+            n_entries = 0
+            n_actual_three_simplices = 0
+            for i in range(n_points):
+                for j in range(i + 1, n_points):
+                    if dist_mat[i, j] < threshold:
+                        for k in range(j + 1, n_points):
+                            if (
+                                dist_mat[i, k] < threshold
+                                and dist_mat[j, k] < threshold
+                            ):
+                                for l in range(k + 1, n_points):
+                                    if (
+                                        dist_mat[i, l] < threshold
+                                        and dist_mat[j, l] < threshold
+                                        and dist_mat[k, l] < threshold
+                                    ):
+                                        row_index = n_actual_three_simplices
+
+                                        column_index_ijk = (
+                                            combinatorial_number_system_d2_forward(
+                                                i, j, k, lookup_table
+                                            )
+                                        )
+                                        column_index_ijl = (
+                                            combinatorial_number_system_d2_forward(
+                                                i, j, l, lookup_table
+                                            )
+                                        )
+                                        column_index_ikl = (
+                                            combinatorial_number_system_d2_forward(
+                                                i, k, l, lookup_table
+                                            )
+                                        )
+                                        column_index_jkl = (
+                                            combinatorial_number_system_d2_forward(
+                                                j, k, l, lookup_table
+                                            )
+                                        )
+
+                                        rows[n_entries] = row_index
+                                        columns[n_entries] = column_index_ijk
+                                        values[n_entries] = 1
+                                        n_entries += 1
+
+                                        rows[n_entries] = row_index
+                                        columns[n_entries] = column_index_ijl
+                                        values[n_entries] = -1
+                                        n_entries += 1
+
+                                        rows[n_entries] = row_index
+                                        columns[n_entries] = column_index_ikl
+                                        values[n_entries] = 1
+                                        n_entries += 1
+
+                                        rows[n_entries] = row_index
+                                        columns[n_entries] = column_index_jkl
+                                        values[n_entries] = -1
+                                        n_entries += 1
+
+                                        n_actual_three_simplices += 1
+            return n_entries, n_actual_three_simplices
+
+        n_entries, n_actual_three_simplices = _delta2_get_row_columns_values(
+            dist_mat, threshold, lookup_table, n_points, rows, columns, values
+        )
+
+        # print("delta 1")
+        # print(n_entries)
+        # print(max_n_entries)
+
+        return sparse.csr_array(
+            (values[:n_entries], (rows[:n_entries], columns[:n_entries])),
+            shape=(n_actual_three_simplices, n_faces),
+        )
+
 
 class PartUnity:
     """
     Partitions of unity subordinate to open ball covers using
     standard bump functions.
 
     """
@@ -524,20 +696,118 @@
         varphi: ndarray(n)
             The bump function
 
         """
         return np.exp(r_cover**2 / (ds**2 - r_cover**2))
 
 
+class EquivariantPCA:
+    @staticmethod
+    def ppca(class_map, proj_dim, projective_dim_red_mode="one-by-one", verbose=False):
+        """
+        Principal Projective Component Analysis (Jose Perea 2017)
+
+        Parameters
+        ----------
+        class_map : ndarray (N, d)
+            For all N points of the dataset, membership weights to
+            d different classes are the coordinates
+        proj_dim : integer
+            The dimension of the projective space onto which to project
+        projective_dim_red_mode : string
+            Either "one-by-one", "exponential", or "direct". How to perform equivariant
+            dimensionality reduction. "exponential" usually works best, being fast
+            without compromising quality.
+        verbose : boolean
+            Whether to print information during iterations
+
+        Returns
+        -------
+        {'variance': ndarray(N-1)
+            The variance captured by each dimension
+        'X': ndarray(N, proj_dim+1)
+            The projective coordinates
+        }
+
+        """
+        if verbose:
+            print(
+                "Doing ppca on %i points in %i dimensions down to %i dimensions"
+                % (class_map.shape[0], class_map.shape[1], proj_dim)
+            )
+
+        assert projective_dim_red_mode in ["direct", "exponential", "one-by-one"]
+
+        X = class_map.T
+        variance = np.zeros(X.shape[0] - 1)
+        n_dim = class_map.shape[1]
+
+        def _one_step_linear_reduction(X, dims_to_keep):
+            try:
+                _, U = np.linalg.eigh(X.dot(np.conjugate(X).T))
+                U = np.fliplr(U)
+            except:
+                U = np.eye(X.shape[0])
+            Y = (np.conjugate(U).T).dot(X)
+            Y = Y[:dims_to_keep, :]
+            X = Y / np.linalg.norm(Y, axis=0)[None, :]
+            return X
+
+        total_dims_to_keep = proj_dim + 1
+
+        mode = projective_dim_red_mode
+        if mode == "direct":
+            XRet = _one_step_linear_reduction(X, total_dims_to_keep)
+        elif mode == "exponential":
+            to_keep_this_iter = (n_dim - total_dims_to_keep) // 2
+            while to_keep_this_iter > 0:
+                X = _one_step_linear_reduction(
+                    X, total_dims_to_keep + to_keep_this_iter
+                )
+                to_keep_this_iter = to_keep_this_iter // 2
+            if X.shape[0] > total_dims_to_keep:
+                X = _one_step_linear_reduction(X, total_dims_to_keep)
+            XRet = X
+
+        elif mode == "one-by-one":
+            tic = time.time()
+            # Projective dimensionality reduction : Main Loop
+            XRet = None
+            for i in range(n_dim - 1):
+                if i == n_dim - proj_dim - 1:
+                    XRet = X
+                try:
+                    _, U = np.linalg.eigh(X.dot(np.conjugate(X).T))
+                    U = np.fliplr(U)
+                    # U, _, _ = np.linalg.svd(X)
+                except:
+                    U = np.eye(X.shape[0])
+                variance[-i - 1] = np.mean(
+                    (np.pi / 2 - np.real(np.arccos(np.abs(U[:, -1][None, :].dot(X)))))
+                    ** 2
+                )
+                Y = (np.conjugate(U).T).dot(X)
+                # y = np.array(Y[-1, :])
+                Y = Y[0:-1, :]
+                # X = Y / np.sqrt(1 - np.abs(y) ** 2)[None, :]
+                X = Y / np.linalg.norm(Y, axis=0)[None, :]
+            if verbose:
+                print("Elapsed time ppca: %.3g" % (time.time() - tic))
+
+        # Return the variance and the projective coordinates
+        return {"variance": variance, "X": XRet.T}
+
+
 class GeometryExamples:
     """
     Finite samples from topologically nontrivial spaces.
 
     """
-    # TODO: These probably belong in tdasets, but I'll keep them here for now
+
+    # TODO: These could belong to tdasets, but we'll keep them here for now
 
     @staticmethod
     def line_patches(dim, n_angles, n_offsets, sigma):
         """
         Sample a set of line segments, as witnessed by square patches
 
         Parameters
@@ -571,14 +841,57 @@
                 patch = X * c + Y * s + ps[j]
                 patch = np.exp(-(patch**2) / sigma**2)
                 P[idx, :] = patch.flatten()
                 idx += 1
         return P
 
     @staticmethod
+    def moving_dot(sqrt_num_images, sigma=3, dim=10):
+        """
+        Sample a set of (smoothened) dots on the plane, as witnessed by square patches
+
+        Parameters
+        ----------
+        sqrt_num_images : int
+            The output will consist of sqrt_num_images**2 patches.
+
+        sigma : float
+            The blur parameter. Higher sigma is more blur. Default is 3.
+
+        dim : int
+            Patches will be dim x dim. Default is 10.
+
+        Returns
+        -------
+        ndarray(sqrt_num_images*sqrt_num_images, dim*dim)
+            An array of all of the patches raveled into dim*dim dimensional Euclidean space
+
+        """
+
+        def _gkern(l=5, mu=0, sig=1.0):
+            ax = np.linspace(-(l - 1) / 2.0, (l - 1) / 2.0, l)
+            gauss_x = np.exp(-0.5 * np.square(ax - mu[0]) / np.square(sig))
+            gauss_y = np.exp(-0.5 * np.square(ax - mu[1]) / np.square(sig))
+            kernel = np.outer(gauss_x, gauss_y)
+            return kernel
+
+        dim = 10
+        P = np.zeros((sqrt_num_images**2, dim * dim))
+        bound = 15
+        xs = bound * np.power(np.linspace(-1, 1, sqrt_num_images), 3)
+        # xs = bound * np.linspace(-1,1,sqrt_num_images)
+        ys = -xs
+        i = 0
+        for x in xs:
+            for y in ys:
+                P[i] = _gkern(l=dim, mu=np.array([x, y]), sig=sigma).flatten()
+                i += 1
+        return P
+
+    @staticmethod
     def rp2_metric(n_samples, seed=None):
         """
         Return a distance matrix of points on the projective plane
         obtained by identifying antipodal Gaussian random samples
         of a sphere
 
         Parameters
@@ -825,31 +1138,101 @@
 
         """
         np.random.seed(0)
         data = 2 * np.random.random_sample((n_samples, 3)) - 1
         return data / np.linalg.norm(data, axis=1)[:, np.newaxis]
 
     @staticmethod
-    def noisy_circle(n_samples, seed=0):
+    def noisy_circle(n_samples, noise_size=0.2, seed=0):
         """
         Samples on a circle in 2D.
 
+        Parameters
+        ----------
+        n_samples : int
+            Number of points on the circle to sample.
+
+        noise_size : float
+            Maximum perturbation per sample. Must be between 0 and 1.
+        
+        seed : float
+            Seed for random number generator.
+
         Returns
         -------
         X: ndarray(n_samples, 2)
             2D circle samples
 
         """
         np.random.seed(seed)
         X = np.random.random((n_samples, 2)) - 0.5
         return (
             X / np.linalg.norm(X, axis=1).reshape((n_samples, 1))
-            + (np.random.random((n_samples, 2)) - 0.5) * 0.2
+            + (np.random.random((n_samples, 2)) - 0.5) * noise_size
         )
 
+    @staticmethod
+    def moore_space_distance_matrix(rough_n_points=2000, prime=3):
+        """
+        Distance matrix of a sample of the Moore space M(1,Z/prime).
+
+        Parameters
+        ----------
+        rough_n_samples : int
+            The function returns a distance matrix with approximately n = rough_n_points * (pi/4) points.
+
+        prime : int
+            The prime associated with the Moore space.
+
+        Returns
+        -------
+        ndarray(n, n)
+            Distance matrix of points on the Moore space M(1,Z/prime).
+
+        """
+        np.random.seed(0)
+        X = (np.random.random((rough_n_points, 2)) - 0.5) * 2
+        X = X[np.linalg.norm(X, axis=1) <= 1]
+        q = prime
+
+        def _rot_mat(theta):
+            c, s = np.cos(theta), np.sin(theta)
+            return np.array(((c, -s), (s, c)))
+
+        R = _rot_mat((2 * np.pi) / q)
+
+        n_points = X.shape[0]
+        dist_mat = np.zeros((n_points, n_points))
+
+        @jit(fastmath=True, nopython=True)
+        def _fill_dist_mat(X, dist_mat, rot_mat, prime):
+            for i, x in enumerate(X):
+                for j, y in enumerate(X):
+                    proj_x_to_boundary = x / np.linalg.norm(x)
+
+                    dist_mat[i, j] = min(
+                        # stay inside disk
+                        np.linalg.norm(x - y),
+                        # go to boundary and then to y
+                        np.linalg.norm(x - proj_x_to_boundary)
+                        + min(
+                            [
+                                np.linalg.norm(
+                                    np.linalg.matrix_power(rot_mat, i)
+                                    @ proj_x_to_boundary
+                                    - y
+                                )
+                                for i in range(prime)
+                            ]
+                        ),
+                    )
+
+        _fill_dist_mat(X, dist_mat, R, prime)
+        return dist_mat, X
+
 
 class CircleMapUtils:
     """
 
     Utilities for adding, rotating, and plotting circle-valued maps.
 
     """
@@ -868,17 +1251,17 @@
 
         Returns
         -------
         ndarray
             A numpy array of floats to be used as color in a matplotlib scatterplot.
 
         """
-        h = np.mod(circle_map/(2*np.pi) + 0.5, 1)
-        f = lambda x : np.sin(np.pi * x)**2
-        return np.stack([f(3/6-h), f(5/6-h), f(7/6-h)], -1)
+        h = np.mod(circle_map / (2 * np.pi) + 0.5, 1)
+        f = lambda x: np.sin(np.pi * x) ** 2
+        return np.stack([f(3 / 6 - h), f(5 / 6 - h), f(7 / 6 - h)], -1)
 
     @staticmethod
     def center(circle_map):
         """
         Rotationally offset a circle-valued map so that most
         of the points map to the center of the circle (i.e., pi).
 
@@ -1032,72 +1415,27 @@
 
         Returns
         -------
         S: ndarray(N, d-1)
             The stereographically projected coordinates
 
         """
-        def _rotmat(a, b=np.array([])):
-            """
-            Construct a d x d rotation matrix that rotates
-            a vector a so that it coincides with a vector b
-
-            Parameters
-            ----------
-            a : ndarray (d)
-                A d-dimensional vector that should be rotated to b
-            b : ndarray(d)
-                A d-dimensional vector that shoudl end up residing at
-                the north pole (0,0,...,0,1)
-
-            """
-            if (len(a.shape) > 1 and np.min(a.shape) > 1) or (
-                len(b.shape) > 1 and np.min(b.shape) > 1
-            ):
-                print("Error: a and b need to be 1D vectors")
-                return None
-            a = a.flatten()
-            a = a / np.sqrt(np.sum(a**2))
-            d = a.size
-
-            if b.size == 0:
-                b = np.zeros(d)
-                b[-1] = 1
-            b = b / np.sqrt(np.sum(b**2))
-
-            c = a - np.sum(b * a) * b
-            # If a numerically coincides with b, don't rotate at all
-            if np.sqrt(np.sum(c**2)) < 1e-15:
-                return np.eye(d)
-
-            # Otherwise, compute rotation matrix
-            c = c / np.sqrt(np.sum(c**2))
-            lam = np.sum(b * a)
-            beta = np.sqrt(1 - np.abs(lam) ** 2)
-            rot = (
-                np.eye(d)
-                - (1 - lam) * (c[:, None].dot(c[None, :]))
-                - (1 - lam) * (b[:, None].dot(b[None, :]))
-                + beta * (b[:, None].dot(c[None, :]) - c[:, None].dot(b[None, :]))
-            )
-            return rot
 
         X = pX.T
         # Put points all on the same hemisphere
         if u.size == 0:
             _, U = np.linalg.eigh(X.dot(X.T))
             u = U[:, 0]
-        XX = _rotmat(u).dot(X)
+        XX = ProjectiveMapUtils.rotmat(u).dot(X)
         ind = XX[-1, :] < 0
         XX[:, ind] *= -1
         # Do stereographic projection
         S = XX[0:-1, :] / (1 + XX[-1, :])[None, :]
         return S.T
 
-
     @staticmethod
     def circle_to_3dnorthpole(x):
         """
         Convert a point selected on the circle to a 3D
         unit vector on the upper hemisphere
 
         Parameters
@@ -1117,7 +1455,163 @@
         if magSqr > 1:
             x /= np.sqrt(magSqr)
             magSqr = 1
         u = np.zeros(3)
         u[0:2] = x
         u[2] = np.sqrt(1 - magSqr)
         return x, u
+
+    @staticmethod
+    def hopf_map(X):
+        """
+        Use the Hopf map to project points on the unit sphere in C^2 representing points in CP^1 to points on the unit sphere in R^3.
+
+        Parameters
+        ----------
+        X : complex ndarray(n,2)
+            Points on the unit sphere in C^2.
+
+        Returns
+        -------
+        real ndarray(n,3)
+            Points on the unit sphere in R^3.
+
+        """
+        Y = np.zeros((2 * X.shape[1], X.shape[0]))
+        Y[::2, :] = np.real(X).T
+        Y[1::2, :] = np.imag(X).T
+        return np.array(
+            [
+                2 * (np.prod(Y[[0, 2], :], axis=0) + np.prod(Y[[1, 3], :], axis=0)),
+                2 * (np.prod(Y[[1, 2], :], axis=0) - np.prod(Y[[0, 3], :], axis=0)),
+                np.sum(Y[[0, 1], :] ** 2, axis=0) - np.sum(Y[[2, 3], :] ** 2, axis=0),
+            ]
+        ).T
+
+    @staticmethod
+    def stereographic_projection_hemispheres(X, center_vector=None):
+        """
+        Project points on the unit sphere in 3D to two disks in 2D corresponding to each hemisphere.
+
+        Parameters
+        ----------
+        X : ndarray(n,3)
+            Points on the unit sphere in 3D
+
+        Returns
+        -------
+        ndarray(n,2)
+
+        """
+
+        def _stereo(v):
+            return v[:, :-1] / (1 - v[:, -1])[:, None]
+
+        n = X.shape[1]
+        if center_vector is None:
+            center_vector = np.zeros((n))
+            center_vector[-1] = 1
+        centering_rotation = ProjectiveMapUtils.rotmat(center_vector)
+        X_ = X @ centering_rotation.T
+        e1 = np.zeros((n - 1))
+        e1[0] = 1
+        res = np.zeros((X_.shape[0], n - 1))
+        res[X_[:, -1] < 0, :] = _stereo(X_[X_[:, -1] < 0, :])
+        Y = X_[X_[:, -1] >= 0, :]
+        Y[:, -1] *= -1
+        res[X_[:, -1] >= 0, :] = _stereo(Y) + 2.5 * e1
+        return res
+
+    @staticmethod
+    def rotmat(a, b=np.array([])):
+        """
+        Construct a d x d rotation matrix that rotates
+        a vector a so that it coincides with a vector b
+
+        Parameters
+        ----------
+        a : ndarray (d)
+            A d-dimensional vector that should be rotated to b
+        b : ndarray(d)
+            A d-dimensional vector that should end up residing at
+            the north pole (0,0,...,0,1)
+
+        """
+        if (len(a.shape) > 1 and np.min(a.shape) > 1) or (
+            len(b.shape) > 1 and np.min(b.shape) > 1
+        ):
+            print("Error: a and b need to be 1D vectors")
+            return None
+        a = a.flatten()
+        a = a / np.sqrt(np.sum(a**2))
+        d = a.size
+
+        if b.size == 0:
+            b = np.zeros(d)
+            b[-1] = 1
+        b = b / np.sqrt(np.sum(b**2))
+
+        c = a - np.sum(b * a) * b
+        # If a numerically coincides with b, don't rotate at all
+        if np.sqrt(np.sum(c**2)) < 1e-15:
+            return np.eye(d)
+
+        # Otherwise, compute rotation matrix
+        c = c / np.sqrt(np.sum(c**2))
+        lam = np.sum(b * a)
+        beta = np.sqrt(1 - np.abs(lam) ** 2)
+        rot = (
+            np.eye(d)
+            - (1 - lam) * (c[:, None].dot(c[None, :]))
+            - (1 - lam) * (b[:, None].dot(b[None, :]))
+            + beta * (b[:, None].dot(c[None, :]) - c[:, None].dot(b[None, :]))
+        )
+        return rot
+
+
+class LensMapUtils:
+    """
+    Utilities for manipulating lens space-valued maps.
+
+    """
+
+    @staticmethod
+    def lens_3D_to_disk_3D(X, q):
+        """
+        Project points on the unit sphere in C^2 representing points in the 3-dimensional
+        lens space corresponding to the prime q to points on the unit disk in R^3.
+
+        Parameters
+        ----------
+        X : complex ndarray(n,2)
+            Points on the unit sphere in C^2.
+
+        q : int
+            Prime number such that X represents points in the 3-dimensional lens space
+            corresponding to this prime.
+
+        Returns
+        -------
+        real ndarray(n,3)
+            Points on the unit disk in R^3.
+
+        """
+
+        def _point_lens_to_sphere(p, q):
+            p1 = p[0]
+            p2 = p[1]
+            arg_z = np.mod(np.angle(p1), 2 * np.pi)
+            theta = np.mod(arg_z, 2 * np.pi / q)
+
+            k = np.floor((arg_z - theta) / (2 * np.pi / q))
+
+            phi = np.mod(np.angle(p2), 2 * np.pi) - 2 * k * np.pi / q
+
+            r = np.abs(p2)
+            x, y, z = (
+                r * np.cos(phi),
+                r * np.sin(phi),
+                (q / np.pi) * (theta - np.pi / q) * np.sqrt(1 - r**2),
+            )
+            return [x, y, z]
+
+        return np.array([_point_lens_to_sphere(p, q) for p in X])
```

### Comparing `dreimac-0.2.0/dreimac.egg-info/PKG-INFO` & `dreimac-0.2.2/dreimac.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,132 +1,142 @@
 Metadata-Version: 2.1
 Name: dreimac
-Version: 0.2.0
-Summary: DREiMac: Dimension reduction with Eilenberg-MacLane coordinates
-Home-page: UNKNOWN
+Version: 0.2.2
+Summary: DREiMac: Dimensionality reduction with Eilenberg-MacLane coordinates
 Author: Jose A. Perea, Luis Scoccola, Chris Tralie
 Author-email: ctralie@alumni.princeton.edu
 License: Apache2
-Description: [![PyPI version](https://badge.fury.io/py/dreimac.svg)](https://badge.fury.io/py/dreimac)
-        [![Downloads](https://static.pepy.tech/badge/dreimac)](https://pepy.tech/project/dreimac)
-        [![codecov](https://codecov.io/gh/scikit-tda/dreimac/branch/master/graph/badge.svg)](https://codecov.io/gh/scikit-tda/dreimac)
-        [![License](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
-        
-        # DREiMac: Dimension Reduction with Eilenberg-MacLane Coordinates
-        
-        DREiMac is a library for topological data coordinatization, visualization, and dimensionality reduction.
-        Currently, DREiMac is able to find topology-preserving representations of point clouds taking values in the circle, in higher dimensional tori, and in the real projective space.
-        
-        In a few words, DREiMac takes as input a point cloud together with a topological feature of the point cloud (in the form of a persistent cohomology class), and returns a map from the point cloud to a well-understood topological space (a circle, a product of circles, or a projective space), which preserves the given topological feature in a precise sense.
-        For more information, please check the theory and examples in the [documentation](https://scikit-tda.org/DREiMac/index.html).
-        
-        ## Basic usage
-        
-        Here is a simple example; please check the Jupyter notebooks in the `notebooks` directory for further examples.
-        
-        ```python
-        # basic imports
-        from dreimac import CircularCoords
-        from persim import plot_diagrams
-        import matplotlib.pyplot as plt
-        import numpy as np
-        
-        # prepare plot with 4 subplots
-        f, (a0, a1, a2, a3) = plt.subplots(1, 4, width_ratios=[1, 1, 1, 0.2], figsize=(14,3))
-        
-        # 200 samples from a noisy circle
-        n_samples = 200
-        np.random.seed(0)
-        Z = np.random.random((n_samples, 2)) - 0.5
-        X = Z / np.linalg.norm(Z, axis=1).reshape((n_samples, 1)) + (np.random.random((n_samples, 2)) - 0.5) * 0.2
-        
-        # plot point cloud
-        a0.scatter(X[:,0], X[:,1], s=10)
-        a0.set_title("Input point cloud") ; a0.axis("off") ; a0.set_aspect("equal")
-        
-        # plot the persistence diagram, showing a single prominent class
-        cc = CircularCoords(X, n_landmarks=200)
-        plot_diagrams(cc.dgms_, title="Persistence diagram", ax=a1)
-        
-        # plot the data colored by the circle-valued map constructed by DREiMac
-        circular_coordinates = cc.get_coordinates()
-        a2.scatter(X[:,0], X[:,1], c=circular_coordinates, s=10, cmap="viridis")
-        a2.set_title("Input colored by circular coordinate") ; a2.axis("off") ; a2.set_aspect("equal")
-        
-        # plot colorbar
-        img = a3.imshow([[0,1]], cmap="viridis"); a3.set_visible(False)
-        cb = plt.colorbar(mappable=img,ticks=[0,0.5,1]) ; _ = cb.ax.set_yticklabels(["0","$\pi$","2$\pi$"])
-        ```
-        
-        ![output](https://user-images.githubusercontent.com/1679929/232109124-bf2653e5-6f91-409d-b972-7104b96b3430.png)
-        
-        ## More examples
-        
-        For Jupyter notebooks with more examples, please check the [documentation](https://scikit-tda.org/DREiMac/index.html) or this repository's [docs/notebooks](https://github.com/scikit-tda/DREiMac/tree/master/docs/notebooks) directory.
-        
-        ## Installing
-        
-        Make sure you are using Python 3.8 or 3.9.
-        DREiMac depends on the following python packages, which will be installed automatically when you install with pip:
-        `matplotlib`,
-        `numba`,
-        `numpy`,
-        `persim`,
-        `ripser`, and
-        `scipy`.
-        
-        ~~~~~ bash
-        pip install dreimac
-        ~~~~~
-        
-        ## Documentation and support
-        
-        You can find the documentation [here](https://scikit-tda.org/DREiMac/index.html), including the [API reference](https://scikit-tda.org/DREiMac/api.html).
-        If you have further questions, please [open an issue](https://github.com/scikit-tda/DREiMac/issues/new) and we will do our best to help you.
-        Please include as much information as possible, including your system's information, warnings, logs, screenshots, and anything else you think may be of use.
-        
-        ## Running the tests
-        
-        If you want to check that your machine is running DREiMac properly, you may run the tests by running the following commands from the root directory of a clone of this repository.
-        
-        ```bash
-        pip install pytest
-        pip install -r requirements.txt
-        pytest .
-        ```
-        
-        ## Contributing
-        
-        To contribute, you can fork the project, make your changes, and submit a pull request.
-        If you're looking for a way to contribute, you could consider:
-        * adding documentation to existing functionality;
-        * adding missing tests to improve coverage;
-        * adding a Jupyter notebook with a tutorial or demo;
-        * adding functionality and the corresponding documentation and tests;
-        * responding to a bug or feature request in the Github issues.
-        
-        ## Authors
-        
-        Jose A. Perea, Luis Scoccola, Chris Tralie
-        
-        ## Acknowledgements
-        
-        We thank Tom Mease for contributions and discussions.
-        
-        ## License
-        
-        This software is published under Apache License Version 2.0.
-        
-Keywords: topological data analysis,dimension reduction
-Platform: UNKNOWN
+Keywords: topological data analysis,dimensionality reduction
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: Intended Audience :: Healthcare Industry
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Requires-Python: >=3.8, <3.10
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: testing
 Provides-Extra: examples
+License-File: LICENSE
+
+[![PyPI version](https://badge.fury.io/py/dreimac.svg)](https://badge.fury.io/py/dreimac)
+[![Downloads](https://static.pepy.tech/badge/dreimac)](https://pepy.tech/project/dreimac)
+[![codecov](https://codecov.io/gh/scikit-tda/dreimac/branch/master/graph/badge.svg)](https://codecov.io/gh/scikit-tda/dreimac)
+[![License](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
+
+# DREiMac: Dimensionality Reduction with Eilenberg-MacLane Coordinates
+
+DREiMac is a library for topological data coordinatization, visualization, and dimensionality reduction.
+Currently, DREiMac is able to find topology-preserving representations of point clouds taking values in the circle, in higher dimensional tori, in the real and complex projective space, and in lens spaces.
+
+In a few words, DREiMac takes as input a point cloud together with a topological feature of the point cloud (in the form of a persistent cohomology class), and returns a map from the point cloud to a well-understood topological space (a circle, a product of circles, a projective space, or a lens space), which preserves the given topological feature in a precise sense.
+For more information, please check the theory and examples in the [documentation](https://scikit-tda.org/DREiMac/index.html).
+
+
+## Basic usage
+
+Here is a simple example; please check the Jupyter notebooks in the `notebooks` directory for further examples.
+
+```python
+# basic imports
+from dreimac import CircularCoords
+from persim import plot_diagrams
+import matplotlib.pyplot as plt
+import numpy as np
+
+# prepare plot with 4 subplots
+f, (a0, a1, a2, a3) = plt.subplots(1, 4, width_ratios=[1, 1, 1, 0.2], figsize=(14,3))
+
+# 200 samples from a noisy circle
+n_samples = 200
+np.random.seed(0)
+Z = np.random.random((n_samples, 2)) - 0.5
+X = Z / np.linalg.norm(Z, axis=1).reshape((n_samples, 1)) + (np.random.random((n_samples, 2)) - 0.5) * 0.2
+
+# plot point cloud
+a0.scatter(X[:,0], X[:,1], s=10)
+a0.set_title("Input point cloud") ; a0.axis("off") ; a0.set_aspect("equal")
+
+# plot the persistence diagram, showing a single prominent class
+cc = CircularCoords(X, n_landmarks=200)
+plot_diagrams(cc.dgms_, title="Persistence diagram", ax=a1)
+
+# plot the data colored by the circle-valued map constructed by DREiMac
+circular_coordinates = cc.get_coordinates()
+a2.scatter(X[:,0], X[:,1], c=circular_coordinates, s=10, cmap="viridis")
+a2.set_title("Input colored by circular coordinate") ; a2.axis("off") ; a2.set_aspect("equal")
+
+# plot colorbar
+img = a3.imshow([[0,1]], cmap="viridis"); a3.set_visible(False)
+cb = plt.colorbar(mappable=img,ticks=[0,0.5,1]) ; _ = cb.ax.set_yticklabels(["0","$\pi$","2$\pi$"])
+```
+
+![output](https://user-images.githubusercontent.com/1679929/232109124-bf2653e5-6f91-409d-b972-7104b96b3430.png)
+
+## More examples
+
+For Jupyter notebooks with more examples, please check the [documentation](https://scikit-tda.org/DREiMac/index.html) or this repository's [docs/notebooks](https://github.com/scikit-tda/DREiMac/tree/master/docs/notebooks) directory.
+
+## Installing
+
+Make sure you are using Python 3.8 or newer.
+DREiMac depends on the following python packages, which will be installed automatically when you install with pip:
+`matplotlib`,
+`numba`,
+`numpy`,
+`persim`,
+`ripser`, and
+`scipy`.
+
+To install the latest release:
+
+~~~~~ bash
+pip install dreimac
+~~~~~
+
+To install directly from GitHub:
+
+~~~~~ bash
+pip install git+https://github.com/scikit-tda/DREiMac.git
+~~~~~
+
+## Documentation and support
+
+You can find the documentation [here](https://scikit-tda.org/DREiMac/index.html), including the [API reference](https://scikit-tda.org/DREiMac/api.html).
+If you have further questions, please [open an issue](https://github.com/scikit-tda/DREiMac/issues/new) and we will do our best to help you.
+Please include as much information as possible, including your system's information, warnings, logs, screenshots, and anything else you think may be of use.
+
+## Running the tests
+
+If you want to check that your machine is running DREiMac properly, you may run the tests by running the following commands from the root directory of a clone of this repository.
+
+```bash
+pip install pytest
+pip install -r requirements.txt
+pytest .
+```
+
+## Contributing
+
+To contribute, you can fork the project, make your changes, and submit a pull request.
+If you're looking for a way to contribute, you could consider:
+* adding documentation to existing functionality;
+* adding missing tests to improve coverage;
+* adding a Jupyter notebook with a tutorial or demo;
+* adding functionality and the corresponding documentation and tests;
+* responding to a bug or feature request in the Github issues.
+
+## Authors
+
+Jose A. Perea, Luis Scoccola, Chris Tralie
+
+## Acknowledgements
+
+We thank Tom Mease for contributions and discussions.
+
+## License
+
+This software is published under Apache License Version 2.0.
```

### Comparing `dreimac-0.2.0/setup.py` & `dreimac-0.2.2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,32 +22,34 @@
     with open("requirements.txt") as f:
         return [line.strip() for line in f if line.strip()]
 
 
 setup(
     name="dreimac",
     version=verstr,
-    description="DREiMac: Dimension reduction with Eilenberg-MacLane coordinates",
+    description="DREiMac: Dimensionality reduction with Eilenberg-MacLane coordinates",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Jose A. Perea, Luis Scoccola, Chris Tralie",
     author_email="ctralie@alumni.princeton.edu",
     license="Apache2",
     packages=["dreimac"],
     install_requires=requirements(),
     extras_require={
         "testing": ["pytest"],
         "examples": [],
     },
-    python_requires=">=3.8, <3.10",
+    python_requires=">=3.8",
     classifiers=[
         "Intended Audience :: Science/Research",
         "Intended Audience :: Education",
         "Intended Audience :: Financial and Insurance Industry",
         "Intended Audience :: Healthcare Industry",
         "Topic :: Scientific/Engineering :: Information Analysis",
         "Topic :: Scientific/Engineering :: Mathematics",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
     ],
-    keywords="topological data analysis, dimension reduction",
+    keywords="topological data analysis, dimensionality reduction",
 )
```

### Comparing `dreimac-0.2.0/test/test_circular.py` & `dreimac-0.2.2/test/test_circular.py`

 * *Files 5% similar despite different names*

```diff
@@ -98,34 +98,35 @@
         )
 
 
     def test_trefoil(self):
         """Check that circular coordinates returns a continuous map, even when the lifted
         cochain may fail to be a cocycle and fix the cocycle using the integer linear system
         """
-        X = GeometryExamples.trefoil(n_samples=2500, horizontal_width=10)
+        for noisy in [True, False]:
+            X = GeometryExamples.trefoil(n_samples=2500, horizontal_width=10, noisy=noisy)
 
-        prime = 3
-        large_perc = 0.8
-        cc = CircularCoords(X, 300, prime=prime)
-        coords = cc.get_coordinates(
-            perc=large_perc,
-            cocycle_idx=0,
-            check_cocycle_condition=True,
-        )
-        assert len(coords) == len(X)
-
-        tree = KDTree(X)
-        k = 5
-        _, nns = tree.query(X, k=k)
+            prime = 3
+            large_perc = 0.8
+            cc = CircularCoords(X, 300, prime=prime)
+            coords = cc.get_coordinates(
+                perc=large_perc,
+                cocycle_idx=0,
+                check_cocycle_condition=True,
+            )
+            assert len(coords) == len(X)
+
+            tree = KDTree(X)
+            k = 5
+            _, nns = tree.query(X, k=k)
 
-        tolerance = 5 / 100 * (2 * np.pi)  # 5% of the full circle
+            tolerance = 5 / 100 * (2 * np.pi)  # 5% of the full circle
 
-        for i in range(X.shape[0]):
-            assert _maximum_circle_distance(coords[nns[i]]) <= tolerance
+            for i in range(X.shape[0]):
+                assert _maximum_circle_distance(coords[nns[i]]) <= tolerance
 
 
 def _circle_distance(x, y):
     return np.minimum(
         np.minimum(np.abs(x - y), np.abs((x - 2 * np.pi) - y)),
         np.abs(x - (y - 2 * np.pi)),
     )
```

### Comparing `dreimac-0.2.0/test/test_combinatorial_number_system.py` & `dreimac-0.2.2/test/test_combinatorial_number_system.py`

 * *Files identical despite different names*

