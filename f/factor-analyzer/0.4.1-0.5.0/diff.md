# Comparing `tmp/factor_analyzer-0.4.1.tar.gz` & `tmp/factor_analyzer-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "factor_analyzer-0.4.1.tar", last modified: Tue Sep 13 22:06:03 2022, max compression
+gzip compressed data, was "factor_analyzer-0.5.0.tar", last modified: Fri Jul  7 23:37:05 2023, max compression
```

## Comparing `factor_analyzer-0.4.1.tar` & `factor_analyzer-0.5.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 nmadnani   (501) staff       (20)        0 2022-09-13 22:06:03.545439 factor_analyzer-0.4.1/
--rw-r--r--   0 nmadnani   (501) staff       (20)    18092 2021-10-27 17:25:17.000000 factor_analyzer-0.4.1/LICENSE
--rw-r--r--   0 nmadnani   (501) staff       (20)       70 2022-09-08 02:02:29.000000 factor_analyzer-0.4.1/MANIFEST.in
--rw-r--r--   0 nmadnani   (501) staff       (20)     9233 2022-09-13 22:06:03.545519 factor_analyzer-0.4.1/PKG-INFO
--rw-r--r--   0 nmadnani   (501) staff       (20)     8336 2022-09-13 22:04:37.000000 factor_analyzer-0.4.1/README.rst
-drwxr-xr-x   0 nmadnani   (501) staff       (20)        0 2022-09-13 22:06:03.544411 factor_analyzer-0.4.1/factor_analyzer/
--rw-r--r--   0 nmadnani   (501) staff       (20)      817 2022-09-08 02:02:29.000000 factor_analyzer-0.4.1/factor_analyzer/__init__.py
--rw-r--r--   0 nmadnani   (501) staff       (20)    43062 2022-09-08 15:51:44.000000 factor_analyzer-0.4.1/factor_analyzer/confirmatory_factor_analyzer.py
--rw-r--r--   0 nmadnani   (501) staff       (20)    33920 2022-09-09 00:40:36.000000 factor_analyzer-0.4.1/factor_analyzer/factor_analyzer.py
--rw-r--r--   0 nmadnani   (501) staff       (20)    22595 2022-09-08 15:51:44.000000 factor_analyzer-0.4.1/factor_analyzer/rotator.py
--rw-r--r--   0 nmadnani   (501) staff       (20)    12671 2022-09-08 02:02:29.000000 factor_analyzer-0.4.1/factor_analyzer/test_utils.py
--rw-r--r--   0 nmadnani   (501) staff       (20)    14241 2022-09-08 15:51:44.000000 factor_analyzer-0.4.1/factor_analyzer/utils.py
-drwxr-xr-x   0 nmadnani   (501) staff       (20)        0 2022-09-13 22:06:03.545318 factor_analyzer-0.4.1/factor_analyzer.egg-info/
--rw-r--r--   0 nmadnani   (501) staff       (20)     9233 2022-09-13 22:06:03.000000 factor_analyzer-0.4.1/factor_analyzer.egg-info/PKG-INFO
--rw-r--r--   0 nmadnani   (501) staff       (20)      502 2022-09-13 22:06:03.000000 factor_analyzer-0.4.1/factor_analyzer.egg-info/SOURCES.txt
--rw-r--r--   0 nmadnani   (501) staff       (20)        1 2022-09-13 22:06:03.000000 factor_analyzer-0.4.1/factor_analyzer.egg-info/dependency_links.txt
--rw-r--r--   0 nmadnani   (501) staff       (20)       43 2022-09-13 22:06:03.000000 factor_analyzer-0.4.1/factor_analyzer.egg-info/requires.txt
--rw-r--r--   0 nmadnani   (501) staff       (20)       16 2022-09-13 22:06:03.000000 factor_analyzer-0.4.1/factor_analyzer.egg-info/top_level.txt
--rw-r--r--   0 nmadnani   (501) staff       (20)        1 2022-09-03 14:42:03.000000 factor_analyzer-0.4.1/factor_analyzer.egg-info/zip-safe
--rw-r--r--   0 nmadnani   (501) staff       (20)       67 2022-09-08 02:02:29.000000 factor_analyzer-0.4.1/pyproject.toml
--rw-r--r--   0 nmadnani   (501) staff       (20)       43 2022-09-08 02:02:29.000000 factor_analyzer-0.4.1/requirements.txt
--rw-r--r--   0 nmadnani   (501) staff       (20)      133 2022-09-13 22:06:03.545816 factor_analyzer-0.4.1/setup.cfg
--rw-r--r--   0 nmadnani   (501) staff       (20)     1410 2022-09-13 22:04:37.000000 factor_analyzer-0.4.1/setup.py
+drwxr-xr-x   0 nmadnani   (501) staff       (20)        0 2023-07-07 23:37:05.979895 factor_analyzer-0.5.0/
+-rw-r--r--   0 nmadnani   (501) staff       (20)    18092 2021-10-27 17:25:17.000000 factor_analyzer-0.5.0/LICENSE
+-rw-r--r--   0 nmadnani   (501) staff       (20)       82 2023-07-07 23:34:43.000000 factor_analyzer-0.5.0/MANIFEST.in
+-rw-r--r--   0 nmadnani   (501) staff       (20)     9410 2023-07-07 23:37:05.979981 factor_analyzer-0.5.0/PKG-INFO
+-rw-r--r--   0 nmadnani   (501) staff       (20)     8462 2023-07-07 23:08:01.000000 factor_analyzer-0.5.0/README.rst
+drwxr-xr-x   0 nmadnani   (501) staff       (20)        0 2023-07-07 23:37:05.978596 factor_analyzer-0.5.0/factor_analyzer/
+-rw-r--r--   0 nmadnani   (501) staff       (20)      817 2022-09-08 02:02:29.000000 factor_analyzer-0.5.0/factor_analyzer/__init__.py
+-rw-r--r--   0 nmadnani   (501) staff       (20)    43072 2023-07-07 20:02:06.000000 factor_analyzer-0.5.0/factor_analyzer/confirmatory_factor_analyzer.py
+-rw-r--r--   0 nmadnani   (501) staff       (20)    35601 2023-07-07 15:03:26.000000 factor_analyzer-0.5.0/factor_analyzer/factor_analyzer.py
+-rw-r--r--   0 nmadnani   (501) staff       (20)    22595 2022-09-08 15:51:44.000000 factor_analyzer-0.5.0/factor_analyzer/rotator.py
+-rw-r--r--   0 nmadnani   (501) staff       (20)    12671 2022-09-08 02:02:29.000000 factor_analyzer-0.5.0/factor_analyzer/test_utils.py
+-rw-r--r--   0 nmadnani   (501) staff       (20)    14241 2022-09-08 15:51:44.000000 factor_analyzer-0.5.0/factor_analyzer/utils.py
+drwxr-xr-x   0 nmadnani   (501) staff       (20)        0 2023-07-07 23:37:05.979742 factor_analyzer-0.5.0/factor_analyzer.egg-info/
+-rw-r--r--   0 nmadnani   (501) staff       (20)     9410 2023-07-07 23:37:05.000000 factor_analyzer-0.5.0/factor_analyzer.egg-info/PKG-INFO
+-rw-r--r--   0 nmadnani   (501) staff       (20)      502 2023-07-07 23:37:05.000000 factor_analyzer-0.5.0/factor_analyzer.egg-info/SOURCES.txt
+-rw-r--r--   0 nmadnani   (501) staff       (20)        1 2023-07-07 23:37:05.000000 factor_analyzer-0.5.0/factor_analyzer.egg-info/dependency_links.txt
+-rw-r--r--   0 nmadnani   (501) staff       (20)       43 2023-07-07 23:37:05.000000 factor_analyzer-0.5.0/factor_analyzer.egg-info/requires.txt
+-rw-r--r--   0 nmadnani   (501) staff       (20)       16 2023-07-07 23:37:05.000000 factor_analyzer-0.5.0/factor_analyzer.egg-info/top_level.txt
+-rw-r--r--   0 nmadnani   (501) staff       (20)        1 2022-09-03 14:42:03.000000 factor_analyzer-0.5.0/factor_analyzer.egg-info/zip-safe
+-rw-r--r--   0 nmadnani   (501) staff       (20)       67 2022-09-08 02:02:29.000000 factor_analyzer-0.5.0/pyproject.toml
+-rw-r--r--   0 nmadnani   (501) staff       (20)       43 2022-09-08 02:02:29.000000 factor_analyzer-0.5.0/requirements.txt
+-rw-r--r--   0 nmadnani   (501) staff       (20)      133 2023-07-07 23:37:05.980288 factor_analyzer-0.5.0/setup.cfg
+-rw-r--r--   0 nmadnani   (501) staff       (20)     1460 2023-07-07 23:08:57.000000 factor_analyzer-0.5.0/setup.py
```

### Comparing `factor_analyzer-0.4.1/LICENSE` & `factor_analyzer-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `factor_analyzer-0.4.1/PKG-INFO` & `factor_analyzer-0.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: factor_analyzer
-Version: 0.4.1
+Version: 0.5.0
 Summary: A Factor Analysis tool written in Python
 Home-page: https://github.com/EducationalTestingService/factor_analyzer
 Author: Jeremy Biggs
 Author-email: jeremy.m.biggs@gmail.com
 Maintainer: Nitin Madnani
 Maintainer-email: nmadnani@ets.org
 Keywords: factor analysis
@@ -16,31 +16,36 @@
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 License-File: LICENSE
 
 FactorAnalyzer
 --------------
 
 .. image:: https://gitlab.com/EducationalTestingService/factor_analyzer/badges/main/pipeline.svg
    :target: https://gitlab.com/EducationalTestingService/factor_analyzer/-/pipelines
    :alt: Build status
 
 .. image:: https://codecov.io/gh/EducationalTestingService/factor_analyzer/branch/main/graph/badge.svg
    :target: https://codecov.io/gh/EducationalTestingService/factor_analyzer
    :alt: Code coverage
 
-.. image:: https://anaconda.org/ets/factor_analyzer/badges/installer/conda.svg
+.. image:: https://anaconda.org/ets/factor_analyzer/badges/version.svg
    :target: https://anaconda.org/ets/factor_analyzer/
    :alt: Conda version
 
+.. image:: https://img.shields.io/pypi/v/factor_analyzer
+   :target: https://pypi.org/project/factor-analyzer/
+   :alt: PyPI version
+
 .. image:: https://img.shields.io/readthedocs/factor_analyzer/latest.svg
    :target: https://factor-analyzer.readthedocs.io/
    :alt: Docs
 
 .. image:: https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white
    :target: https://github.com/pre-commit/pre-commit
    :alt: Pre-commit checks
```

### Comparing `factor_analyzer-0.4.1/README.rst` & `factor_analyzer-0.5.0/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -5,18 +5,22 @@
    :target: https://gitlab.com/EducationalTestingService/factor_analyzer/-/pipelines
    :alt: Build status
 
 .. image:: https://codecov.io/gh/EducationalTestingService/factor_analyzer/branch/main/graph/badge.svg
    :target: https://codecov.io/gh/EducationalTestingService/factor_analyzer
    :alt: Code coverage
 
-.. image:: https://anaconda.org/ets/factor_analyzer/badges/installer/conda.svg
+.. image:: https://anaconda.org/ets/factor_analyzer/badges/version.svg
    :target: https://anaconda.org/ets/factor_analyzer/
    :alt: Conda version
 
+.. image:: https://img.shields.io/pypi/v/factor_analyzer
+   :target: https://pypi.org/project/factor-analyzer/
+   :alt: PyPI version
+
 .. image:: https://img.shields.io/readthedocs/factor_analyzer/latest.svg
    :target: https://factor-analyzer.readthedocs.io/
    :alt: Docs
 
 .. image:: https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white
    :target: https://github.com/pre-commit/pre-commit
    :alt: Pre-commit checks
```

### Comparing `factor_analyzer-0.4.1/factor_analyzer/__init__.py` & `factor_analyzer-0.5.0/factor_analyzer/__init__.py`

 * *Files identical despite different names*

### Comparing `factor_analyzer-0.4.1/factor_analyzer/confirmatory_factor_analyzer.py` & `factor_analyzer-0.5.0/factor_analyzer/confirmatory_factor_analyzer.py`

 * *Files 0% similar despite different names*

```diff
@@ -737,15 +737,15 @@
             assert len(self.bounds) == len(x0), error_msg
 
         # fit the actual model using L-BFGS algorithm;
         # the constraints are set inside the objective function,
         # so that we can avoid using linear programming methods (e.g. SLSQP)
         res = minimize(
             self._objective,
-            x0,
+            x0.flatten(),
             method="L-BFGS-B",
             options={"maxiter": self.max_iter, "disp": self.disp},
             bounds=self.bounds,
             args=(cov_mtx, self.model.loadings),
         )
 
         # if the optimizer failed to converge, print the message
```

### Comparing `factor_analyzer-0.4.1/factor_analyzer/factor_analyzer.py` & `factor_analyzer-0.5.0/factor_analyzer/factor_analyzer.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 :author: Jeremy Biggs (jeremy.m.biggs@gmail.com)
 :author: Nitin Madnani (nmadnani@ets.org)
 :organization: Educational Testing Service
 :date: 2022-09-05
 """
 
 import warnings
+from typing import Tuple
 
 import numpy as np
 import pandas as pd
 import scipy as sp
 from scipy.optimize import minimize
 from scipy.stats import chi2, pearsonr
 from sklearn.base import BaseEstimator, TransformerMixin
@@ -965,7 +966,55 @@
          array([0.35101885, 0.12837102, 0.07373951]),
          array([0.35101885, 0.47938987, 0.55312938]))
         """
         # meets all of our expected criteria
         check_is_fitted(self, "loadings_")
         loadings = self.loadings_.copy()
         return self._get_factor_variance(loadings)
+
+    def sufficiency(self, num_observations: int) -> Tuple[float, int, float]:
+        """
+        Perform the sufficiency test.
+
+        The test calculates statistics under the null hypothesis that
+        the selected number of factors is sufficient.
+
+        Parameters
+        ----------
+        num_observations: int
+            The number of observations in the input data that this factor
+            analyzer was fit using.
+
+        Returns
+        -------
+        statistic: float
+            The test statistic
+        degrees: int
+            The degrees of freedom
+        pvalue: float
+            The p-value of the test
+
+        References
+        ----------
+        [1] Lawley, D. N. and Maxwell, A. E. (1971). Factor Analysis as a Statistical Method. Second edition.
+        Butterworths. P. 36.
+
+        Examples
+        --------
+        >>> import pandas as pd
+        >>> from factor_analyzer import FactorAnalyzer
+        >>> df_features = pd.read_csv('tests/data/test01.csv')
+        >>> fa = FactorAnalyzer(n_factors=3, rotation=None, method="ml")
+        >>> fa.fit(df_features)
+        >>> fa.sufficiency(df_features.shape[0])
+        (1475.8755629859675, 663, 8.804286459822274e-64)
+        """
+        nvar = self.corr_.shape[0]
+        degrees = ((nvar - self.n_factors) ** 2 - nvar - self.n_factors) // 2
+        obj = self._fit_ml_objective(
+            self.get_uniquenesses(), self.corr_, self.n_factors
+        )
+        statistic = (
+            num_observations - 1 - (2 * nvar + 5) / 6 - (2 * self.n_factors) / 3
+        ) * obj
+        pvalue = chi2.sf(statistic, df=degrees)
+        return statistic, degrees, pvalue
```

### Comparing `factor_analyzer-0.4.1/factor_analyzer/rotator.py` & `factor_analyzer-0.5.0/factor_analyzer/rotator.py`

 * *Files identical despite different names*

### Comparing `factor_analyzer-0.4.1/factor_analyzer/test_utils.py` & `factor_analyzer-0.5.0/factor_analyzer/test_utils.py`

 * *Files identical despite different names*

### Comparing `factor_analyzer-0.4.1/factor_analyzer/utils.py` & `factor_analyzer-0.5.0/factor_analyzer/utils.py`

 * *Files identical despite different names*

### Comparing `factor_analyzer-0.4.1/factor_analyzer.egg-info/PKG-INFO` & `factor_analyzer-0.5.0/factor_analyzer.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: factor-analyzer
-Version: 0.4.1
+Version: 0.5.0
 Summary: A Factor Analysis tool written in Python
 Home-page: https://github.com/EducationalTestingService/factor_analyzer
 Author: Jeremy Biggs
 Author-email: jeremy.m.biggs@gmail.com
 Maintainer: Nitin Madnani
 Maintainer-email: nmadnani@ets.org
 Keywords: factor analysis
@@ -16,31 +16,36 @@
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 License-File: LICENSE
 
 FactorAnalyzer
 --------------
 
 .. image:: https://gitlab.com/EducationalTestingService/factor_analyzer/badges/main/pipeline.svg
    :target: https://gitlab.com/EducationalTestingService/factor_analyzer/-/pipelines
    :alt: Build status
 
 .. image:: https://codecov.io/gh/EducationalTestingService/factor_analyzer/branch/main/graph/badge.svg
    :target: https://codecov.io/gh/EducationalTestingService/factor_analyzer
    :alt: Code coverage
 
-.. image:: https://anaconda.org/ets/factor_analyzer/badges/installer/conda.svg
+.. image:: https://anaconda.org/ets/factor_analyzer/badges/version.svg
    :target: https://anaconda.org/ets/factor_analyzer/
    :alt: Conda version
 
+.. image:: https://img.shields.io/pypi/v/factor_analyzer
+   :target: https://pypi.org/project/factor-analyzer/
+   :alt: PyPI version
+
 .. image:: https://img.shields.io/readthedocs/factor_analyzer/latest.svg
    :target: https://factor-analyzer.readthedocs.io/
    :alt: Docs
 
 .. image:: https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white
    :target: https://github.com/pre-commit/pre-commit
    :alt: Pre-commit checks
```

### Comparing `factor_analyzer-0.4.1/setup.py` & `factor_analyzer-0.5.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     with open(req_path) as f:
         reqs = f.read().splitlines()
     return reqs
 
 
 setup(
     name="factor_analyzer",
-    version="0.4.1",
+    version="0.5.0",
     description="A Factor Analysis tool written in Python",
     long_description=readme(),
     keywords="factor analysis",
     packages=find_packages(),
     author="Jeremy Biggs",
     author_email="jeremy.m.biggs@gmail.com",
     maintainer="Nitin Madnani",
@@ -39,10 +39,11 @@
         "Operating System :: POSIX",
         "Operating System :: Unix",
         "Operating System :: MacOS",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
     ],
     zip_safe=True,
 )
```

