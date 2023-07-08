# Comparing `tmp/preliz-0.3.0.tar.gz` & `tmp/preliz-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "preliz-0.3.0.tar", last modified: Wed Apr 19 00:58:29 2023, max compression
+gzip compressed data, was "preliz-0.3.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `preliz-0.3.0.tar` & `preliz-0.3.1.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0     2802 2023-04-19 00:58:22.162966 preliz-0.3.0/README.md
--rw-r--r--   0        0        0      649 2023-04-19 00:58:22.334967 preliz-0.3.0/preliz/__init__.py
--rw-r--r--   0        0        0     1016 2023-04-19 00:58:22.334967 preliz-0.3.0/preliz/distributions/__init__.py
--rw-r--r--   0        0        0    89157 2023-04-19 00:58:22.334967 preliz-0.3.0/preliz/distributions/continuous.py
--rw-r--r--   0        0        0    14095 2023-04-19 00:58:22.334967 preliz-0.3.0/preliz/distributions/continuous_multivariate.py
--rw-r--r--   0        0        0    39411 2023-04-19 00:58:22.334967 preliz-0.3.0/preliz/distributions/discrete.py
--rw-r--r--   0        0        0    18095 2023-04-19 00:58:22.334967 preliz-0.3.0/preliz/distributions/distributions.py
--rw-r--r--   0        0        0     6516 2023-04-19 00:58:22.334967 preliz-0.3.0/preliz/distributions/distributions_multivariate.py
--rw-r--r--   0        0        0       64 2023-04-19 00:58:22.334967 preliz-0.3.0/preliz/internal/__init__.py
--rw-r--r--   0        0        0     4611 2023-04-19 00:58:22.334967 preliz-0.3.0/preliz/internal/distribution_helper.py
--rw-r--r--   0        0        0     7289 2023-04-19 00:58:22.334967 preliz-0.3.0/preliz/internal/optimization.py
--rw-r--r--   0        0        0     3043 2023-04-19 00:58:22.334967 preliz-0.3.0/preliz/internal/parser.py
--rw-r--r--   0        0        0    14995 2023-04-19 00:58:22.334967 preliz-0.3.0/preliz/internal/plot_helper.py
--rw-r--r--   0        0        0     8168 2023-04-19 00:58:22.334967 preliz-0.3.0/preliz/internal/plot_helper_multivariate.py
--rw-r--r--   0        0        0      114 2023-04-19 00:58:22.334967 preliz-0.3.0/preliz/predictive/__init__.py
--rw-r--r--   0        0        0    14107 2023-04-19 00:58:22.334967 preliz-0.3.0/preliz/predictive/ppa.py
--rw-r--r--   0        0        0     1345 2023-04-19 00:58:22.334967 preliz-0.3.0/preliz/predictive/predictive_sliders.py
--rw-r--r--   0        0        0     1946 2023-04-19 00:58:22.334967 preliz-0.3.0/preliz/tests/check_inside_notebook.ipynb
--rw-r--r--   0        0        0     1799 2023-04-19 00:58:22.334967 preliz-0.3.0/preliz/tests/plot_interactive.ipynb
--rw-r--r--   0        0        0     2244 2023-04-19 00:58:22.334967 preliz-0.3.0/preliz/tests/predictive_sliders.ipynb
--rw-r--r--   0        0        0     1472 2023-04-19 00:58:22.334967 preliz-0.3.0/preliz/tests/roulette.ipynb
--rw-r--r--   0        0        0     7310 2023-04-19 00:58:22.334967 preliz-0.3.0/preliz/tests/test_distributions.py
--rw-r--r--   0        0        0      626 2023-04-19 00:58:22.334967 preliz-0.3.0/preliz/tests/test_helper.py
--rw-r--r--   0        0        0      338 2023-04-19 00:58:22.334967 preliz-0.3.0/preliz/tests/test_internals.py
--rw-r--r--   0        0        0     6488 2023-04-19 00:58:22.334967 preliz-0.3.0/preliz/tests/test_maxent.py
--rw-r--r--   0        0        0     2859 2023-04-19 00:58:22.334967 preliz-0.3.0/preliz/tests/test_mle.py
--rw-r--r--   0        0        0     2789 2023-04-19 00:58:22.334967 preliz-0.3.0/preliz/tests/test_plots.py
--rw-r--r--   0        0        0      115 2023-04-19 00:58:22.334967 preliz-0.3.0/preliz/tests/test_predictive_sliders.py
--rw-r--r--   0        0        0     3455 2023-04-19 00:58:22.334967 preliz-0.3.0/preliz/tests/test_quartile.py
--rw-r--r--   0        0        0      906 2023-04-19 00:58:22.334967 preliz-0.3.0/preliz/tests/test_roulette.py
--rw-r--r--   0        0        0      164 2023-04-19 00:58:22.334967 preliz-0.3.0/preliz/unidimensional/__init__.py
--rw-r--r--   0        0        0     3898 2023-04-19 00:58:22.334967 preliz-0.3.0/preliz/unidimensional/maxent.py
--rw-r--r--   0        0        0     1681 2023-04-19 00:58:22.334967 preliz-0.3.0/preliz/unidimensional/mle.py
--rw-r--r--   0        0        0     3263 2023-04-19 00:58:22.334967 preliz-0.3.0/preliz/unidimensional/quartile.py
--rw-r--r--   0        0        0     9633 2023-04-19 00:58:22.338967 preliz-0.3.0/preliz/unidimensional/roulette.py
--rw-r--r--   0        0        0     1298 2023-04-19 00:58:22.338967 preliz-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     3801 1970-01-01 00:00:00.000000 preliz-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     3712 2023-07-08 12:03:31.873032 preliz-0.3.1/README.md
+-rw-r--r--   0        0        0      649 2023-07-08 12:03:32.033036 preliz-0.3.1/preliz/__init__.py
+-rw-r--r--   0        0        0     1037 2023-07-08 12:03:32.033036 preliz-0.3.1/preliz/distributions/__init__.py
+-rw-r--r--   0        0        0    89186 2023-07-08 12:03:32.037036 preliz-0.3.1/preliz/distributions/continuous.py
+-rw-r--r--   0        0        0    14095 2023-07-08 12:03:32.037036 preliz-0.3.1/preliz/distributions/continuous_multivariate.py
+-rw-r--r--   0        0        0    43519 2023-07-08 12:03:32.037036 preliz-0.3.1/preliz/distributions/discrete.py
+-rw-r--r--   0        0        0    19949 2023-07-08 12:03:32.037036 preliz-0.3.1/preliz/distributions/distributions.py
+-rw-r--r--   0        0        0     6516 2023-07-08 12:03:32.037036 preliz-0.3.1/preliz/distributions/distributions_multivariate.py
+-rw-r--r--   0        0        0       64 2023-07-08 12:03:32.037036 preliz-0.3.1/preliz/internal/__init__.py
+-rw-r--r--   0        0        0     4659 2023-07-08 12:03:32.037036 preliz-0.3.1/preliz/internal/distribution_helper.py
+-rw-r--r--   0        0        0     8770 2023-07-08 12:03:32.037036 preliz-0.3.1/preliz/internal/optimization.py
+-rw-r--r--   0        0        0     3043 2023-07-08 12:03:32.037036 preliz-0.3.1/preliz/internal/parser.py
+-rw-r--r--   0        0        0    15583 2023-07-08 12:03:32.037036 preliz-0.3.1/preliz/internal/plot_helper.py
+-rw-r--r--   0        0        0     8168 2023-07-08 12:03:32.037036 preliz-0.3.1/preliz/internal/plot_helper_multivariate.py
+-rw-r--r--   0        0        0      114 2023-07-08 12:03:32.037036 preliz-0.3.1/preliz/predictive/__init__.py
+-rw-r--r--   0        0        0    14107 2023-07-08 12:03:32.037036 preliz-0.3.1/preliz/predictive/ppa.py
+-rw-r--r--   0        0        0     1345 2023-07-08 12:03:32.037036 preliz-0.3.1/preliz/predictive/predictive_sliders.py
+-rw-r--r--   0        0        0     1946 2023-07-08 12:03:32.037036 preliz-0.3.1/preliz/tests/check_inside_notebook.ipynb
+-rw-r--r--   0        0        0     1799 2023-07-08 12:03:32.037036 preliz-0.3.1/preliz/tests/plot_interactive.ipynb
+-rw-r--r--   0        0        0     2244 2023-07-08 12:03:32.037036 preliz-0.3.1/preliz/tests/predictive_sliders.ipynb
+-rw-r--r--   0        0        0     1472 2023-07-08 12:03:32.037036 preliz-0.3.1/preliz/tests/roulette.ipynb
+-rw-r--r--   0        0        0     7434 2023-07-08 12:03:32.037036 preliz-0.3.1/preliz/tests/test_distributions.py
+-rw-r--r--   0        0        0      626 2023-07-08 12:03:32.037036 preliz-0.3.1/preliz/tests/test_helper.py
+-rw-r--r--   0        0        0      338 2023-07-08 12:03:32.037036 preliz-0.3.1/preliz/tests/test_internals.py
+-rw-r--r--   0        0        0     6634 2023-07-08 12:03:32.037036 preliz-0.3.1/preliz/tests/test_maxent.py
+-rw-r--r--   0        0        0     2919 2023-07-08 12:03:32.037036 preliz-0.3.1/preliz/tests/test_mle.py
+-rw-r--r--   0        0        0     2828 2023-07-08 12:03:32.037036 preliz-0.3.1/preliz/tests/test_plots.py
+-rw-r--r--   0        0        0      115 2023-07-08 12:03:32.037036 preliz-0.3.1/preliz/tests/test_predictive_sliders.py
+-rw-r--r--   0        0        0     3483 2023-07-08 12:03:32.037036 preliz-0.3.1/preliz/tests/test_quartile.py
+-rw-r--r--   0        0        0      906 2023-07-08 12:03:32.037036 preliz-0.3.1/preliz/tests/test_roulette.py
+-rw-r--r--   0        0        0      164 2023-07-08 12:03:32.037036 preliz-0.3.1/preliz/unidimensional/__init__.py
+-rw-r--r--   0        0        0     3898 2023-07-08 12:03:32.037036 preliz-0.3.1/preliz/unidimensional/maxent.py
+-rw-r--r--   0        0        0     1681 2023-07-08 12:03:32.037036 preliz-0.3.1/preliz/unidimensional/mle.py
+-rw-r--r--   0        0        0     3214 2023-07-08 12:03:32.037036 preliz-0.3.1/preliz/unidimensional/quartile.py
+-rw-r--r--   0        0        0     9633 2023-07-08 12:03:32.037036 preliz-0.3.1/preliz/unidimensional/roulette.py
+-rw-r--r--   0        0        0     1393 2023-07-08 12:03:32.037036 preliz-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     4928 1970-01-01 00:00:00.000000 preliz-0.3.1/PKG-INFO
```

### Comparing `preliz-0.3.0/README.md` & `preliz-0.3.1/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -5,29 +5,42 @@
 
 [![PyPi version](https://badge.fury.io/py/preliz.svg)](https://badge.fury.io/py/preliz)
 [![Build Status](https://github.com/arviz-devs/preliz/actions/workflows/test.yml/badge.svg)](https://github.com/arviz-devs/preliz/actions/workflows/test.yml)
 [![codecov](https://codecov.io/gh/arviz-devs/preliz/branch/master/graph/badge.svg?token=SLJIK2O4C5 )](https://codecov.io/gh/arviz-devs/preliz/)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black)
 
 
-
+Prior elicitation refers to the process of transforming the knowledge of a particular domain into well-defined probability distributions. Specifying useful priors is a central aspect of Bayesian statistics. PreliZ is a Python package aimed at helping practitioners choose prior distributions by offering a set of tools for the various facets of prior elicitation. It covers a range of methods, from unidimensional prior elicitation on the parameter space to predictive elicitation on the observed space. The goal is to be compatible with probabilistic programming languages (PPL) in the Python ecosystem like PyMC and PyStan, while remaining agnostic of any specific PPL.
 
 ## Documentation
 
 The PreliZ documentation can be found in the [official docs](https://preliz.readthedocs.io/en/latest/).
 
 ## Installation
 
 ### Last release
 PreliZ is available for installation from [PyPI](https://pypi.org/project/preliz/).
-The latest  version can be installed using pip:
+The latest version (base set of dependencies) can be installed using pip:
 
 ```
 pip install preliz
 ```
+To make use of the interactive features, you can install the optional dependencies:
+
+* For JupyterLab:
+
+```
+pip install "preliz[full,lab]"
+```
+
+* For Jupyter Notebook:
+
+```
+pip install "preliz[full,notebook]"
+```
 
 ### Development
 The latest development version can be installed from the main branch using pip:
 
 ```
 pip install git+git://github.com/arviz-devs/preliz.git
 ```
```

### Comparing `preliz-0.3.0/preliz/__init__.py` & `preliz-0.3.1/preliz/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from .distributions import *
 from .predictive import *
 from .unidimensional import *
 
 
 __all__ = ["maxent", "mle", "ppa", "roulette", "quartile"]
 
-__version__ = "0.3.0"
+__version__ = "0.3.1"
 
 _log = logging.getLogger("preliz")
 
 if not logging.root.handlers:
     _log.setLevel(logging.INFO)
     if len(_log.handlers) == 0:
         handler = logging.StreamHandler()
```

### Comparing `preliz-0.3.0/preliz/distributions/__init__.py` & `preliz-0.3.1/preliz/distributions/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -36,14 +36,15 @@
 ]
 all_discrete = [
     Bernoulli,
     BetaBinomial,
     Binomial,
     Categorical,
     DiscreteUniform,
+    DiscreteWeibull,
     Geometric,
     HyperGeometric,
     NegativeBinomial,
     Poisson,
     ZeroInflatedBinomial,
     ZeroInflatedNegativeBinomial,
     ZeroInflatedPoisson,
```

### Comparing `preliz-0.3.0/preliz/distributions/continuous.py` & `preliz-0.3.1/preliz/distributions/continuous.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 import numpy as np
 from scipy import stats
 from scipy.special import gamma as gammaf
 from scipy.special import beta as betaf  # pylint: disable=no-name-in-module
 from scipy.special import logit, expit  # pylint: disable=no-name-in-module
 
-from ..internal.optimization import optimize_ml, optimize_moments
+from ..internal.optimization import optimize_ml, optimize_moments, optimize_moments_rice
 from ..internal.distribution_helper import garcia_approximation, all_not_none, any_not_none
 from .distributions import Continuous
 
 eps = np.finfo(float).eps
 
 
 def from_precision(precision):
@@ -2206,16 +2206,16 @@
             self.params = (self.nu, self.sigma)
         elif self.param_names[0] == "b":
             self.params = (self.b, self.sigma)
 
         self._update_rv_frozen()
 
     def _fit_moments(self, mean, sigma):
-        params = mean, sigma
-        optimize_moments(self, mean, sigma, params)
+        nu, sigma = optimize_moments_rice(mean, sigma)
+        self._update(nu, sigma)
 
     def _fit_mle(self, sample, **kwargs):
         b, _, sigma = self.dist.fit(sample, **kwargs)
         nu = self._from_b(b, sigma)
         self._update(nu, sigma)
```

### Comparing `preliz-0.3.0/preliz/distributions/continuous_multivariate.py` & `preliz-0.3.1/preliz/distributions/continuous_multivariate.py`

 * *Files identical despite different names*

### Comparing `preliz-0.3.0/preliz/distributions/discrete.py` & `preliz-0.3.1/preliz/distributions/discrete.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 """
 from copy import copy
 import logging
 from math import ceil
 
 import numpy as np
 from scipy import stats
-from scipy.special import logit, expit  # pylint: disable=no-name-in-module
+from scipy.special import logit, expit, gamma  # pylint: disable=no-name-in-module
 
 
 from .distributions import Discrete
 from ..internal.optimization import optimize_ml, optimize_moments
 from ..internal.distribution_helper import all_not_none, any_not_none
 
 
@@ -466,14 +466,140 @@
 
     def _fit_mle(self, sample):
         lower = np.min(sample)
         upper = np.max(sample)
         self._update(lower, upper)
 
 
+class DiscreteWeibull(Discrete):
+    R"""
+    Discrete Weibull distribution.
+
+    The pmf of this distribution is
+
+    .. math::
+
+        f(x \mid q, \beta) = q^{x^{\beta}} - q^{(x+1)^{\beta}}
+
+    .. plot::
+        :context: close-figs
+
+        import arviz as az
+        from preliz import DiscreteWeibull
+        az.style.use('arviz-white')
+        qs = [0.1, 0.9, 0.9]
+        betas = [0.3, 1.3, 3]
+        for q, b in zip(qs, betas):
+            DiscreteWeibull(q, b).plot_pdf(support=(0,10))
+
+    ========  ===============================================
+    Support   :math:`x \in \mathbb{N}_0`
+    Mean      :math:`\mu = \sum_{x = 1}^{\infty} q^{x^{\beta}}`
+    Variance  :math:`2 \sum_{x = 1}^{\infty} x q^{x^{\beta}} - \mu - \mu^2`
+    ========  ===============================================
+
+    Parameters
+    ----------
+    q: float
+        Shape parameter (0 < q < 1).
+    beta: float
+        Shape parameter (beta > 0).
+    """
+
+    def __init__(self, q=None, beta=None):
+        super().__init__()
+        self.dist = _DiscreteWeibull
+        self.support = (0, np.inf)
+        self._parametrization(q, beta)
+
+    def _parametrization(self, q=None, beta=None):
+        self.q = q
+        self.beta = beta
+        self.params = (self.q, self.beta)
+        self.param_names = ("q", "beta")
+        self.params_support = ((eps, 1 - eps), (eps, np.inf))
+        if all_not_none(q, beta):
+            self._update(q, beta)
+
+    def _get_frozen(self):
+        frozen = None
+        if all_not_none(self.params):
+            frozen = self.dist(self.q, self.beta)
+        return frozen
+
+    def _update(self, q, beta):
+        self.q = np.float64(q)
+        self.beta = np.float64(beta)
+        self.support = (0, np.inf)
+        self.params = (self.q, self.beta)
+        self._update_rv_frozen()
+
+    def _fit_moments(self, mean, sigma):
+        optimize_moments(self, mean, sigma)
+
+    def _fit_mle(self, sample):
+        optimize_ml(self, sample)
+
+
+class _DiscreteWeibull(stats.rv_continuous):
+    def __init__(self, q=None, beta=None):
+        super().__init__()
+        self.q = q
+        self.beta = beta
+
+    def support(self, *args, **kwds):  # pylint: disable=unused-argument
+        return (0, np.inf)
+
+    def cdf(self, x, *args, **kwds):  # pylint: disable=unused-argument
+        x = np.asarray(x)
+        return 1 - self.q ** ((x + 1) ** self.beta)
+
+    def pmf(self, x, *args, **kwds):  # pylint: disable=unused-argument
+        x = np.asarray(x)
+        return self.q ** (x**self.beta) - self.q ** ((x + 1) ** self.beta)
+
+    def logpmf(self, x, *args, **kwds):  # pylint: disable=unused-argument
+        return np.log(self.pmf(x, *args, **kwds))
+
+    def ppf(self, p, *args, **kwds):  # pylint: disable=arguments-differ unused-argument
+        p = np.asarray(p)
+        p[p == 1] = 0.999999
+        ppf = np.ceil((np.log(1 - p) / np.log(self.q)) ** (1 / self.beta) - 1)
+        return ppf
+
+    def _stats(self, *args, **kwds):  # pylint: disable=unused-argument
+        x_max = np.nan_to_num(self._ppf(0.999), nan=1)
+        if x_max < 10000:
+            x_range = np.arange(1, x_max + 1, dtype=int)
+            mean = np.sum(self.q ** (x_range**self.beta))
+            var = 2 * np.sum(x_range * self.q ** (x_range**self.beta)) - mean - mean**2
+        else:
+            lam = (-1 / np.log(self.q)) ** (1 / self.beta)
+            kappa = gamma(1 + 1 / self.beta)
+            mean = lam * kappa - 0.5
+            var = lam**2 * (gamma(1 + 2 / self.beta) - (kappa**2)) - 1
+        return (mean, var, np.nan, np.nan)
+
+    def entropy(self):  # pylint: disable=arguments-differ
+        entropy = 0.0
+        x = 0
+        while True:
+            p_x = self.q ** (x**self.beta) - self.q ** ((x + 1) ** self.beta)
+            if p_x < 1e-6:
+                break
+            entropy -= p_x * np.log(p_x)
+            x += 1
+        return entropy
+
+        # return self.q / np.log(self.beta)
+
+    def rvs(self, size=1, random_state=None):  # pylint: disable=arguments-differ
+        return self.ppf(np.random.uniform(size=size), random_state=random_state)
+
+
 class Geometric(Discrete):
     R"""
     Geometric distribution.
 
     The probability that the first success in a sequence of Bernoulli trials
     occurs on the x'th trial.
     The pmf of this distribution is
@@ -1100,15 +1226,15 @@
     def _update(self, psi, mu):
         self.psi = np.float64(psi)
         self.mu = np.float64(mu)
         self.params = (self.psi, self.mu)
         self._update_rv_frozen()
 
     def _fit_moments(self, mean, sigma):
-        psi = mean**2 / (mean**2 - mean + sigma**2)
+        psi = min(0.99, max(0.01, mean**2 / (mean**2 - mean + sigma**2)))
         mean = mean / psi
         self._update(psi, mean)
 
     def _fit_mle(self, sample):
         optimize_ml(self, sample)
```

### Comparing `preliz-0.3.0/preliz/distributions/distributions.py` & `preliz-0.3.1/preliz/distributions/distributions.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 Parent classes for all families.
 """
 # pylint: disable=no-member
+import warnings
 from collections import namedtuple
 
 from ipywidgets import interactive
 import numpy as np
 
 from ..internal.plot_helper import (
     plot_pdfpmf,
@@ -221,14 +222,16 @@
         self,
         moments=None,
         pointinterval=False,
         interval="hdi",
         levels=None,
         support="full",
         legend="legend",
+        color=None,
+        alpha=1,
         figsize=None,
         ax=None,
     ):
         """
         Plot the  pdf (continuous) or pmf (discrete).
 
         Parameters
@@ -249,34 +252,51 @@
             (in this last case nothing will be plotted).
         support : str:
             If ``full`` use the finite end-points to set the limits of the plot. For unbounded
             end-points or if ``restricted`` use the 0.001 and 0.999 quantiles to set the limits.
         legend : str
             Whether to include a string with the distribution and its parameter as a ``"legend"`` a
             ``"title"`` or not include them ``None``.
+        color : str
+            Valid matplotlib color. Defaults to None, colors will be selected from the active
+            color cycle.
+        alpha : float
+            Transparency of the line. Defaults to 1 (no transparency).
         figsize : tuple
             Size of the figure
         ax : matplotlib axes
         """
 
         if valid_scalar_params(self):
             return plot_pdfpmf(
-                self, moments, pointinterval, interval, levels, support, legend, figsize, ax
+                self,
+                moments,
+                pointinterval,
+                interval,
+                levels,
+                support,
+                legend,
+                color,
+                alpha,
+                figsize,
+                ax,
             )
         else:
             return None
 
     def plot_cdf(
         self,
         moments=None,
         pointinterval=False,
         interval="hdi",
         levels=None,
         support="full",
         legend="legend",
+        color=None,
+        alpha=1,
         figsize=None,
         ax=None,
     ):
         """
         Plot the cumulative distribution function.
 
         Parameters
@@ -294,35 +314,52 @@
         levels : list
             Mass of the intervals. For hdi or eti the number of elements should be 2 or 1.
             For quantiles the number of elements should be 5, 3, 1 or 0
             (in this last case nothing will be plotted).
         support : str:
             If ``full`` use the finite end-points to set the limits of the plot. For unbounded
             end-points or if ``restricted`` use the 0.001 and 0.999 quantiles to set the limits.
+        color : str
+            Valid matplotlib color. Defaults to None, colors will be selected from the active
+            color cycle.
+        alpha : float
+            Transparency of the line. Defaults to 1 (no transparency).
         legend : str
             Whether to include a string with the distribution and its parameter as a ``"legend"`` a
             ``"title"`` or not include them ``None``.
         figsize : tuple
             Size of the figure
         ax : matplotlib axes
         """
         if valid_scalar_params(self):
             return plot_cdf(
-                self, moments, pointinterval, interval, levels, support, legend, figsize, ax
+                self,
+                moments,
+                pointinterval,
+                interval,
+                levels,
+                support,
+                legend,
+                color,
+                alpha,
+                figsize,
+                ax,
             )
         else:
             return None
 
     def plot_ppf(
         self,
         moments=None,
         pointinterval=False,
         interval="hdi",
         levels=None,
         legend="legend",
+        color=None,
+        alpha=1,
         figsize=None,
         ax=None,
     ):
         """
         Plot the quantile function.
 
         Parameters
@@ -340,71 +377,94 @@
         levels : list
             Mass of the intervals. For hdi or eti the number of elements should be 2 or 1.
             For quantiles the number of elements should be 5, 3, 1 or 0
             (in this last case nothing will be plotted).
         legend : str
             Whether to include a string with the distribution and its parameter as a ``"legend"`` a
             ``"title"`` or not include them ``None``.
+        color : str
+            Valid matplotlib color. Defaults to None, colors will be selected from the active
+            color cycle.
+        alpha : float
+            Transparency of the line. Defaults to 1 (no transparency).
         figsize : tuple
             Size of the figure
         ax : matplotlib axes
         """
         if valid_scalar_params(self):
-            return plot_ppf(self, moments, pointinterval, interval, levels, legend, figsize, ax)
+            return plot_ppf(
+                self, moments, pointinterval, interval, levels, legend, color, alpha, figsize, ax
+            )
         else:
             return None
 
     def plot_interactive(
-        self, kind="pdf", fixed_lim="both", pointinterval=True, interval="hdi", levels=None
+        self,
+        kind="pdf",
+        xy_lim="both",
+        pointinterval=True,
+        interval="hdi",
+        levels=None,
+        figsize=None,
+        fixed_lim=None,
     ):
         """
         Interactive exploration of distributions parameters
 
         Parameters
         ----------
         kind : str:
             Type of plot. Available options are `pdf`, `cdf` and `ppf`.
-        fixed_lim : str or tuple
+        xy_lim : str or tuple
             Set the limits of the x-axis and/or y-axis.
             Defaults to `"both"`, the limits of both axis are fixed.
             Use `"auto"` for automatic rescaling of x-axis and y-axis.
             Or set them manually by passing a tuple of 4 elements,
-            the first two fox x-axis, the last two for x-axis. The tuple can have `None`.
+            the first two for x-axis, the last two for x-axis. The tuple can have `None`.
         pointinterval : bool
             Whether to include a plot of the quantiles. Defaults to False. If True the default is to
             plot the median and two interquantiles ranges.
         interval : str
             Type of interval. Available options are highest density interval `"hdi"` (default),
         equal tailed interval `"eti"` or intervals defined by arbitrary `"quantiles"`.
         levels : list
             Mass of the intervals. For hdi or eti the number of elements should be 2 or 1.
             For quantiles the number of elements should be 5, 3, 1 or 0
             (in this last case nothing will be plotted).
+        figsize : tuple
+            Size of the figure
         """
         check_inside_notebook()
 
         if valid_scalar_params(self, check_frozen=False):
             args = dict(zip(self.param_names, self.params))
         else:
             args = init_vals[self.__class__.__name__]
 
         self.__init__(**args)
 
-        if fixed_lim == "both":
+        if fixed_lim is not None:
+            warnings.warn(
+                "The 'fixed_lim' parameter will be deprecated. Use 'xy_lim' instead.",
+                FutureWarning,
+            )
+            xy_lim = fixed_lim
+
+        if xy_lim == "both":
             xlim = self._finite_endpoints("full")
             xvals = self.xvals("restricted")
             if kind == "pdf":
                 max_pdf = np.max(self.pdf(xvals))
                 ylim = (-max_pdf * 0.075, max_pdf * 1.5)
             elif kind == "ppf":
                 max_ppf = self.ppf(0.999)
                 ylim = (-max_ppf * 0.075, max_ppf * 1.5)
-        elif isinstance(fixed_lim, tuple):
-            xlim = fixed_lim[:2]
-            ylim = fixed_lim[2:]
+        elif isinstance(xy_lim, tuple):
+            xlim = xy_lim[:2]
+            ylim = xy_lim[2:]
 
         sliders = {}
         if self.__class__.__name__ == "Categorical":
             pointinterval = False
             name = self.param_names[0]
             params = self.params[0]
             names = [f"{name}_{i}" for i in range(len(params))]
@@ -421,27 +481,39 @@
                 values = list(args.values())
                 args = {list(args.keys())[0].split("_")[0]: values}
                 if np.sum(values) > 1:
                     return None
             self.__init__(**args)
             if kind == "pdf":
                 ax = self.plot_pdf(
-                    legend=False, pointinterval=pointinterval, interval=interval, levels=levels
+                    legend=False,
+                    pointinterval=pointinterval,
+                    interval=interval,
+                    levels=levels,
+                    figsize=figsize,
                 )
             elif kind == "cdf":
                 ax = self.plot_cdf(
-                    legend=False, pointinterval=pointinterval, interval=interval, levels=levels
+                    legend=False,
+                    pointinterval=pointinterval,
+                    interval=interval,
+                    levels=levels,
+                    figsize=figsize,
                 )
             elif kind == "ppf":
                 ax = self.plot_ppf(
-                    legend=False, pointinterval=pointinterval, interval=interval, levels=levels
+                    legend=False,
+                    pointinterval=pointinterval,
+                    interval=interval,
+                    levels=levels,
+                    figsize=figsize,
                 )
-            if fixed_lim != "auto" and kind != "ppf":
+            if xy_lim != "auto" and kind != "ppf":
                 ax.set_xlim(*xlim)
-            if fixed_lim != "auto" and kind != "cdf":
+            if xy_lim != "auto" and kind != "cdf":
                 ax.set_ylim(*ylim)
 
         return interactive(plot, **sliders)
 
 
 class Continuous(Distribution):
     """Base class for continuous distributions."""
```

### Comparing `preliz-0.3.0/preliz/distributions/distributions_multivariate.py` & `preliz-0.3.1/preliz/distributions/distributions_multivariate.py`

 * *Files identical despite different names*

### Comparing `preliz-0.3.0/preliz/internal/distribution_helper.py` & `preliz-0.3.1/preliz/internal/distribution_helper.py`

 * *Files 2% similar despite different names*

```diff
@@ -124,14 +124,15 @@
     "Wald": {"mu": 1, "lam": 3.0},
     "Weibull": {"alpha": 5.0, "beta": 2.0},
     "Bernoulli": {"p": 0.5},
     "BetaBinomial": {"alpha": 2, "beta": 2, "n": 10},
     "Binomial": {"n": 5, "p": 0.5},
     "Categorical": {"p": [0.5, 0.1, 0.4]},
     "DiscreteUniform": {"lower": -2.0, "upper": 2.0},
+    "DiscreteWeibull": {"q": 0.9, "beta": 1.3},
     "Geometric": {"p": 0.5},
     "HyperGeometric": {"N": 50, "k": 10, "n": 20},
     "NegativeBinomial": {"mu": 5.0, "alpha": 2.0},
     "Poisson": {"mu": 4.5},
     "ZeroInflatedBinomial": {"psi": 0.7, "n": 10, "p": 0.5},
     "ZeroInflatedNegativeBinomial": {"psi": 0.7, "mu": 5, "alpha": 8},
     "ZeroInflatedPoisson": {"psi": 0.8, "mu": 4.5},
```

### Comparing `preliz-0.3.0/preliz/internal/optimization.py` & `preliz-0.3.1/preliz/internal/optimization.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """
 Optimization routines and utilities
 """
 from sys import modules
 import numpy as np
 from scipy.optimize import minimize, least_squares
+from scipy.special import i0, i1  # pylint: disable=no-name-in-module
 from .distribution_helper import init_vals as default_vals
 
 
 def optimize_max_ent(dist, lower, upper, mass, none_idx, fixed):
     def prob_bound(params, dist, lower, upper, mass):
         params = get_params(dist, params, none_idx, fixed)
         dist._parametrization(**params)
@@ -60,15 +61,14 @@
         dist._parametrization(**params)
         loss = dist.cdf(x_vals) - [0.25, 0.5, 0.75]
         return loss
 
     init_vals = np.array(dist.params)[none_idx]
     bounds = np.array(dist.params_support)[none_idx]
     bounds = list(zip(*bounds))
-
     opt = least_squares(func, x0=init_vals, args=(dist, x_vals), bounds=bounds)
     params = get_params(dist, opt["x"], none_idx, fixed)
     dist._parametrization(**params)
     return opt
 
 
 def optimize_cdf(dist, x_vals, ecdf, none_idx, fixed):
@@ -98,24 +98,70 @@
     if params is not None:
         dist._update(*params)
     else:
         dist._update(**default_vals[dist.__class__.__name__])
 
     init_vals = np.array(dist.params)[none_idx]
 
-    if dist == "HyperGeometric":
-        opt = minimize(func, x0=init_vals, args=(dist, mean, sigma), method="Powell")
-    else:
+    if dist.__class__.__name__ in ["HyperGeometric", "BetaBinomial"]:
         opt = least_squares(func, x0=init_vals, args=(dist, mean, sigma))
+    else:
+        bounds = np.array(dist.params_support)[none_idx]
+        bounds = list(zip(*bounds))
+        if dist.__class__.__name__ in ["DiscreteWeibull"]:
+            opt = least_squares(
+                func, x0=init_vals, args=(dist, mean, sigma), bounds=bounds, loss="soft_l1"
+            )
+        else:
+            opt = least_squares(func, x0=init_vals, args=(dist, mean, sigma), bounds=bounds)
 
     params = get_params(dist, opt["x"], none_idx, fixed)
     dist._parametrization(**params)
     return opt
 
 
+def optimize_moments_rice(mean, std_dev):
+    """
+    Moment matching for the Rice distribution
+
+    This function uses the Koay inversion technique, see: https://doi.org/10.1016/j.jmr.2006.01.016
+    and https://en.wikipedia.org/wiki/Rice_distribution
+    """
+
+    ratio = mean / std_dev
+
+    if ratio < 1.913:  # Rayleigh distribution
+        nu = np.finfo(float).eps
+        sigma = 0.655 * std_dev
+    else:
+
+        def xi(theta):
+            return (
+                2
+                + theta**2
+                - np.pi
+                / 8
+                * np.exp(-(theta**2) / 2)
+                * ((2 + theta**2) * i0(theta**2 / 4) + theta**2 * i1(theta**2 / 4)) ** 2
+            )
+
+        def fpf(theta):
+            return (xi(theta) * (1 + ratio**2) - 2) ** 0.5
+
+        def func(theta):
+            return np.abs(fpf(theta) - theta)
+
+        theta = minimize(func, x0=fpf(1), bounds=[(0, None)]).x
+        xi_theta = xi(theta)
+        sigma = std_dev / xi_theta**0.5
+        nu = (mean**2 + (xi_theta - 2) * sigma**2) ** 0.5
+
+    return nu, sigma
+
+
 def optimize_ml(dist, sample):
     def negll(params, dist, sample):
         dist._update(*params)
         if dist.kind == "continuous":
             neg = -dist.rv_frozen.logpdf(sample).sum()
         else:
             neg = -dist.rv_frozen.logpmf(sample).sum()
```

### Comparing `preliz-0.3.0/preliz/internal/parser.py` & `preliz-0.3.1/preliz/internal/parser.py`

 * *Files identical despite different names*

### Comparing `preliz-0.3.0/preliz/internal/plot_helper.py` & `preliz-0.3.1/preliz/internal/plot_helper.py`

 * *Files 4% similar despite different names*

```diff
@@ -96,17 +96,20 @@
 
 
 def eti(distribution, mass):
     lower = (1 - mass) / 2
     return np.quantile(distribution, (lower, mass + lower))
 
 
-def plot_pdfpmf(dist, moments, pointinterval, interval, levels, support, legend, figsize, ax):
+def plot_pdfpmf(
+    dist, moments, pointinterval, interval, levels, support, legend, color, alpha, figsize, ax
+):
     ax = get_ax(ax, figsize)
-    color = next(ax._get_lines.prop_cycler)["color"]
+    if color is None:
+        color = next(ax._get_lines.prop_cycler)["color"]
     if legend is not None:
         label = repr_to_matplotlib(dist)
 
         if moments is not None:
             label += get_moments(dist, moments)
 
         if legend == "title":
@@ -115,44 +118,47 @@
     else:
         label = None
 
     x = dist.xvals(support)
     if dist.kind == "continuous":
         density = dist.pdf(x)
         ax.axhline(0, color="0.8", ls="--", zorder=0)
-        ax.plot(x, density, label=label, color=color)
+        ax.plot(x, density, label=label, color=color, alpha=alpha)
         ax.set_yticks([])
     else:
         mass = dist.pdf(x)
         eps = np.clip(dist._finite_endpoints(support), *dist.support)
         x_c = np.linspace(*eps, 1000)
 
         if len(x) > 2:
             interp = PchipInterpolator(x, mass)
         else:
             interp = interp1d(x, mass)
 
         mass_c = np.clip(interp(x_c), np.min(mass), np.max(mass))
 
         ax.axhline(0, color="0.8", ls="--", zorder=0)
-        ax.plot(x_c, mass_c, ls="dotted", color=color)
-        ax.plot(x, mass, "o", label=label, color=color)
+        ax.plot(x_c, mass_c, ls="dotted", color=color, alpha=alpha)
+        ax.plot(x, mass, "o", label=label, color=color, alpha=alpha)
 
     if pointinterval:
         plot_pointinterval(dist, interval, levels, ax=ax)
 
     if legend == "legend":
         side_legend(ax)
 
     return ax
 
 
-def plot_cdf(dist, moments, pointinterval, interval, levels, support, legend, figsize, ax):
+def plot_cdf(
+    dist, moments, pointinterval, interval, levels, support, legend, color, alpha, figsize, ax
+):
     ax = get_ax(ax, figsize)
-    color = next(ax._get_lines.prop_cycler)["color"]
+    if color is None:
+        color = next(ax._get_lines.prop_cycler)["color"]
     if legend is not None:
         label = repr_to_matplotlib(dist)
 
         if moments is not None:
             label += get_moments(dist, moments)
 
         if legend == "title":
@@ -167,45 +173,46 @@
     if dist.kind == "discrete":
         lower = x[0]
         upper = x[-1]
         x = np.insert(x, [0, len(x)], (lower - 1, upper + 1))
         cdf = dist.cdf(x)
         ax.set_xlim(lower - 0.1, upper + 0.1)
         ax.xaxis.set_major_locator(MaxNLocator(integer=True))
-        ax.step(x, cdf, where="post", label=label, color=color)
+        ax.step(x, cdf, where="post", label=label, color=color, alpha=alpha)
     else:
         cdf = dist.cdf(x)
-        ax.plot(x, cdf, label=label, color=color)
+        ax.plot(x, cdf, label=label, color=color, alpha=alpha)
 
     if pointinterval:
         plot_pointinterval(dist, interval, levels, ax=ax)
 
     if legend == "legend":
         side_legend(ax)
     return ax
 
 
-def plot_ppf(dist, moments, pointinterval, interval, levels, legend, figsize, ax):
+def plot_ppf(dist, moments, pointinterval, interval, levels, legend, color, alpha, figsize, ax):
     ax = get_ax(ax, figsize)
-    color = next(ax._get_lines.prop_cycler)["color"]
+    if color is None:
+        color = next(ax._get_lines.prop_cycler)["color"]
 
     if legend is not None:
         label = repr_to_matplotlib(dist)
 
         if moments is not None:
             label += get_moments(dist, moments)
 
         if legend == "title":
             ax.set_title(label)
             label = None
     else:
         label = None
 
     x = np.linspace(0, 1, 1000)
-    ax.plot(x, dist.ppf(x), label=label, color=color)
+    ax.plot(x, dist.ppf(x), label=label, color=color, alpha=alpha)
     if dist.kind == "discrete":
         ax.yaxis.set_major_locator(MaxNLocator(integer=True))
 
     if pointinterval:
         plot_pointinterval(dist, interval, levels, rotated=True, ax=ax)
 
     if legend == "legend":
@@ -257,26 +264,19 @@
 
         seen.append(moment)
 
     return "\n" + ", ".join(str_m)
 
 
 def get_slider(name, value, lower, upper, continuous_update=True):
-    if np.isfinite(lower):
-        min_v = lower
-    else:
-        min_v = value - 10
-    if np.isfinite(upper):
-        max_v = upper
-    else:
-        max_v = value + 10
+
+    min_v, max_v, step = generate_range(value, lower, upper)
 
     if isinstance(value, float):
         slider_type = FloatSlider
-        step = (max_v - min_v) / 100
     else:
         slider_type = IntSlider
         step = 1
 
     slider = slider_type(
         min=min_v,
         max=max_v,
@@ -286,14 +286,32 @@
         style={"description_width": "initial"},
         continuous_update=continuous_update,
     )
 
     return slider
 
 
+def generate_range(value, lower, upper):
+    if value == 0:
+        return -10, 10, 0.1
+
+    power = np.floor(np.log10(abs(value)))
+    order_of_magnitude = 10**power
+    decimal_places = int(-power)
+    std = order_of_magnitude * 10 - order_of_magnitude / 10
+    min_v = round(value - std, decimal_places)
+    max_v = round(value + std, decimal_places)
+
+    min_v = lower if np.isfinite(lower) else min_v
+    max_v = upper if np.isfinite(upper) else max_v
+
+    step = order_of_magnitude / 10
+    return min_v, max_v, step
+
+
 def get_sliders(signature, model):
     sliders = {}
     for name, param in signature.parameters.items():
         if isinstance(param.default, (int, float)):
             value = float(param.default)
         else:
             value = None
```

### Comparing `preliz-0.3.0/preliz/internal/plot_helper_multivariate.py` & `preliz-0.3.1/preliz/internal/plot_helper_multivariate.py`

 * *Files identical despite different names*

### Comparing `preliz-0.3.0/preliz/predictive/ppa.py` & `preliz-0.3.1/preliz/predictive/ppa.py`

 * *Files identical despite different names*

### Comparing `preliz-0.3.0/preliz/predictive/predictive_sliders.py` & `preliz-0.3.1/preliz/predictive/predictive_sliders.py`

 * *Files identical despite different names*

### Comparing `preliz-0.3.0/preliz/tests/check_inside_notebook.ipynb` & `preliz-0.3.1/preliz/tests/check_inside_notebook.ipynb`

 * *Files identical despite different names*

### Comparing `preliz-0.3.0/preliz/tests/plot_interactive.ipynb` & `preliz-0.3.1/preliz/tests/plot_interactive.ipynb`

 * *Files identical despite different names*

### Comparing `preliz-0.3.0/preliz/tests/predictive_sliders.ipynb` & `preliz-0.3.1/preliz/tests/predictive_sliders.ipynb`

 * *Files identical despite different names*

### Comparing `preliz-0.3.0/preliz/tests/roulette.ipynb` & `preliz-0.3.1/preliz/tests/roulette.ipynb`

 * *Files identical despite different names*

### Comparing `preliz-0.3.0/preliz/tests/test_distributions.py` & `preliz-0.3.1/preliz/tests/test_distributions.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,14 +35,15 @@
     VonMises,
     Wald,
     Weibull,
     Bernoulli,
     BetaBinomial,
     Binomial,
     DiscreteUniform,
+    DiscreteWeibull,
     Geometric,
     NegativeBinomial,
     Poisson,
     ZeroInflatedNegativeBinomial,
     ZeroInflatedPoisson,
     Dirichlet,
     MvNormal,
@@ -90,14 +91,15 @@
         (Wald, (1, 1)),
         (Weibull, (2, 1)),
         (Bernoulli, (0.8,)),
         (BetaBinomial, (1, 1, 10)),
         (Binomial, (2, 0.5)),
         (Binomial, (2, 0.1)),
         (DiscreteUniform, (0, 1)),
+        (DiscreteWeibull, (0.5, 3)),
         (Geometric, (0.75,)),
         (NegativeBinomial, (8, 4)),
         (Poisson, (4.5,)),
         (
             ZeroInflatedPoisson,
             (
                 0.8,
@@ -112,14 +114,15 @@
 
     dist_._fit_moments(dist.rv_frozen.mean(), dist.rv_frozen.std())
 
     tol = 5
     if dist.__class__.__name__ in [
         "BetaBinomial",
         "Binomial",
+        "DiscreteWeibull",
         "Kumaraswamy",
         "LogitNormal",
         "Rice",
         "StudentT",
     ]:
         tol = 0
     assert_almost_equal(dist.rv_frozen.mean(), dist_.rv_frozen.mean(), tol)
@@ -162,14 +165,15 @@
         (Wald, (1, 1)),
         (Weibull, (2, 1)),
         (Bernoulli, (0.4,)),
         (BetaBinomial, (2, 2, 10)),
         (Binomial, (2, 0.5)),
         (Binomial, (2, 0.1)),
         (DiscreteUniform, (0, 1)),
+        (DiscreteWeibull, (0.1, 1.5)),
         (Geometric, (0.5,)),
         (NegativeBinomial, (8, 4)),
         (Poisson, (4.5,)),
         (ZeroInflatedNegativeBinomial, (0.7, 8, 4)),
         (
             ZeroInflatedPoisson,
             (
```

### Comparing `preliz-0.3.0/preliz/tests/test_helper.py` & `preliz-0.3.1/preliz/tests/test_helper.py`

 * *Files identical despite different names*

### Comparing `preliz-0.3.0/preliz/tests/test_maxent.py` & `preliz-0.3.1/preliz/tests/test_maxent.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,14 +36,15 @@
     VonMises,
     Wald,
     Weibull,
     # Bernoulli, maxent is not useful for Bernoulli distribution as we only have two states
     BetaBinomial,
     Binomial,
     DiscreteUniform,
+    DiscreteWeibull,
     Geometric,
     HyperGeometric,
     NegativeBinomial,
     Poisson,
     ZeroInflatedBinomial,
     ZeroInflatedNegativeBinomial,
     ZeroInflatedPoisson,
@@ -82,30 +83,31 @@
         (Gumbel(), 0, 10, 0.9, (-np.inf, np.inf), (3.557, 2.598)),
         (Gumbel(mu=9), 0, 10, 0.9, (-np.inf, np.inf), (0.444)),
         (HalfCauchy(), 0, 10, 0.7, (0, np.inf), (5.095)),
         (HalfNormal(), 0, 10, 0.7, (0, np.inf), (9.648)),
         (HalfStudentT(), 1, 10, 0.7, (0, np.inf), (99.997, 7.697)),
         (HalfStudentT(nu=7), 1, 10, 0.7, (0, np.inf), (2.541)),
         (InverseGamma(), 0, 1, 0.99, (0, np.inf), (8.889, 3.439)),
-        (Kumaraswamy(), 0.1, 0.6, 0.9, (0, 1), (2.246, 7.426)),
+        (Kumaraswamy(), 0.1, 0.6, 0.9, (0, 1), (2.246, 7.427)),
         (Laplace(), -1, 1, 0.9, (-np.inf, np.inf), (0, 0.435)),
         (Laplace(mu=0.5), -1, 1, 0.9, (-np.inf, np.inf), (0.303)),
         (Logistic(), -1, 1, 0.5, (-np.inf, np.inf), (0, 0.91)),
         (LogNormal(), 1, 4, 0.5, (0, np.inf), (1.216, 0.859)),
         (LogNormal(mu=1), 1, 4, 0.5, (0, np.inf), (0.978)),
         (LogitNormal(), 0.3, 0.8, 0.9, (0, 1), (0.226, 0.677)),
         (LogitNormal(mu=0.7), 0.3, 0.8, 0.9, (0, 1), (0.531)),
         (Moyal(), 0, 10, 0.9, (-np.inf, np.inf), (2.935, 1.6)),
         (Moyal(mu=4), 0, 10, 0.9, (-np.inf, np.inf), (1.445)),
         (Normal(), -1, 1, 0.683, (-np.inf, np.inf), (0, 1)),
         (Normal(), 10, 12, 0.99, (-np.inf, np.inf), (11, 0.388)),
         (Normal(mu=0.5), -1, 1, 0.8, (-np.inf, np.inf), (0.581)),
         (Pareto(), 1, 4, 0.9, (1, np.inf), (1.660, 1)),
         (Pareto(m=2), 1, 4, 0.9, (2, np.inf), (3.321)),
-        (Rice(), 0, 4, 0.7, (0, np.inf), (0.0139, 2.577)),
+        (Rice(), 0, 4, 0.7, (0, np.inf), (0, 2.577)),
+        (Rice(), 1, 10, 0.9, (0, np.inf), (3.453, 3.735)),
         (Rice(nu=4), 0, 6, 0.9, (0, np.inf), (1.402)),
         (SkewNormal(), -2, 10, 0.9, (-np.inf, np.inf), (3.999, 3.647, 0)),
         (SkewNormal(mu=-1), -2, 10, 0.9, (-np.inf, np.inf), (6.2924, 4.905)),
         (StudentT(), -1, 1, 0.683, (-np.inf, np.inf), (99.999, 0, 0.994)),
         (StudentT(nu=7), -1, 1, 0.683, (-np.inf, np.inf), (0, 0.928)),
         (
             Triangular(),
@@ -137,18 +139,19 @@
         (VonMises(mu=0.5), -1, 1, 0.9, (-np.pi, np.pi), (6.997)),
         (Wald(), 0, 10, 0.9, (0, np.inf), (5.061, 7.937)),
         (Wald(mu=5), 0, 10, 0.9, (0, np.inf), (7.348)),
         (Weibull(), 0, 10, 0.9, (0, np.inf), (1.411, 5.537)),
         (Weibull(alpha=2), 0, 10, 0.9, (0, np.inf), (6.590)),
         (BetaBinomial(), 2, 8, 0.9, (0, 8), (1.951, 1.345, 8)),
         (BetaBinomial(n=10), 2, 6, 0.6, (0, 10), (1.837, 2.181)),
-        # results for binomial are close to the correct result, but still off
+        # # results for binomial are close to the correct result, but still off
         (Binomial(), 3, 9, 0.9, (0, 9), (9, 0.490)),
         (Binomial(n=12), 3, 9, 0.9, (0, 12), (0.612)),
         (DiscreteUniform(), -2, 10, 0.9, (-3, 11), (-2, 10)),
+        (DiscreteWeibull(), 1, 6, 0.7, (0, np.inf), (0.938, 1.604)),
         (Geometric(), 1, 4, 0.99, (0, np.inf), (0.6837)),
         (HyperGeometric(), 2, 14, 0.9, (0, 21), (56, 21, 21)),
         (NegativeBinomial(), 0, 15, 0.9, (0, np.inf), (7.546, 2.041)),
         (NegativeBinomial(p=0.2), 0, 15, 0.9, (0, np.inf), (1.847)),
         (Poisson(), 0, 3, 0.7, (0, np.inf), (2.763)),
         (ZeroInflatedBinomial(), 1, 10, 0.9, (0, np.inf), (0.901, 10, 0.493)),
         (ZeroInflatedBinomial(psi=0.7), 1, 10, 0.7, (0, np.inf), (11, 0.5)),
```

### Comparing `preliz-0.3.0/preliz/tests/test_mle.py` & `preliz-0.3.1/preliz/tests/test_mle.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,14 +35,15 @@
     VonMises,
     Wald,
     Weibull,
     Bernoulli,
     BetaBinomial,
     Binomial,
     DiscreteUniform,
+    DiscreteWeibull,
     Geometric,
     HyperGeometric,
     NegativeBinomial,
     Poisson,
     ZeroInflatedBinomial,
     ZeroInflatedNegativeBinomial,
     ZeroInflatedPoisson,
@@ -83,14 +84,15 @@
         (VonMises, (1, 2)),
         (Wald, (2, 1)),
         (Weibull, (2, 1)),
         (Bernoulli, (0.5,)),
         (BetaBinomial, (1, 2, 10)),
         (Binomial, (5, 0.5)),
         (DiscreteUniform, (-2, 2)),
+        (DiscreteWeibull, (0.9, 1.3)),
         (Geometric, (0.75,)),
         (HyperGeometric, (50, 20, 10)),
         (NegativeBinomial, (10, 0.5)),
         (Poisson, (4.2,)),
         (ZeroInflatedBinomial, (0.5, 10, 0.8)),
         (ZeroInflatedNegativeBinomial, (0.7, 8, 4)),
         (
```

### Comparing `preliz-0.3.0/preliz/tests/test_plots.py` & `preliz-0.3.1/preliz/tests/test_plots.py`

 * *Files 7% similar despite different names*

```diff
@@ -20,14 +20,15 @@
         {"moments": "mdsk", "legend": "title"},
         {"pointinterval": True},
         {"pointinterval": True, "levels": [0.1, 0.9]},
         {"pointinterval": True, "interval": "eti", "levels": [0.9]},
         {"pointinterval": True, "interval": "quantiles"},
         {"pointinterval": True, "interval": "quantiles", "levels": [0.1, 0.5, 0.9]},
         {"support": "restricted"},
+        {"color": "C1", "alpha": 0.1},
         {"figsize": (4, 4)},
         {"ax": plt.subplots()[1]},
     ],
 )
 def test_continuous_plot_pdf_cdf_ppf(two_dist, kwargs):
     for a_dist in two_dist:
         a_dist.plot_pdf(**kwargs)
```

### Comparing `preliz-0.3.0/preliz/tests/test_quartile.py` & `preliz-0.3.1/preliz/tests/test_quartile.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,15 +31,16 @@
     TruncatedNormal,
     Uniform,
     VonMises,
     Wald,
     Weibull,
     # Bernoulli, quartile is not useful for Bernoulli distribution as we only have two states
     BetaBinomial,
-    # DiscreteUniform,
+    DiscreteUniform,
+    DiscreteWeibull,
     Geometric,
     HyperGeometric,
     NegativeBinomial,
     Poisson,
     ZeroInflatedBinomial,
     ZeroInflatedNegativeBinomial,
     ZeroInflatedPoisson,
@@ -66,15 +67,15 @@
         (Laplace(), -1, 0, 1, (0, 1.442)),
         (Logistic(), -1, 0, 1, (0, 0.910)),
         (LogNormal(), 0.5, 1, 2, (0, 1.027)),
         (LogitNormal(), 0.3, 0.45, 0.6, (-0.212, 0.929)),
         (Moyal(), 0.5, 1, 2, (0.620, 0.567)),
         (Normal(), -1, 0, 1, (0, 1.482)),
         (Pareto(), 0.5, 1, 4, (0.541, 0.289)),
-        (Rice(), 2, 4, 6, (0.03566, 3.395)),
+        (Rice(), 2, 4, 6, (0, 3.395)),
         pytest.param(
             StudentT(),
             -1,
             0,
             1,
             (84576.43, 0, 1.482),
             marks=pytest.mark.skipif(
@@ -84,22 +85,23 @@
         (StudentT(nu=4), -1, 0, 1, (0, 1.350)),
         (Triangular(), 0, 1, 2, (-2.414, 1.0, 4.414)),
         (TruncatedNormal(), -1, 0, 1, (0, 1.482)),
         (Uniform(), -1, 0, 1, (-2, 2)),
         (VonMises(), -1, 0, 1, (0, 0.656)),
         (Wald(), 0.5, 1, 2, (1.698, 1.109)),
         (Weibull(), 0.5, 1, 2, (1.109, 1.456)),
-        (BetaBinomial(), 2, 5, 8, (1.59, 4.49, 23)),
-        # (DiscreteUniform(), -1, 0, 1, (-5, 5)), # the mass is 0.27 instead of 0.5
+        (BetaBinomial(), 2, 5, 8, (1.182, 1.53, 13.0)),
+        (DiscreteUniform(), -2, 0, 2, (-5, 5)),
+        (DiscreteWeibull(), 2, 6, 7, (0.951, 1.487)),
         (Geometric(), 2, 4, 6, (0.17)),
-        (HyperGeometric(), 2, 3, 4, (75, 15, 15)),
+        (HyperGeometric(), 2, 3, 4, (26, 8, 8)),
         (NegativeBinomial(), 3, 5, 10, (7.283, 2.167)),
         (Poisson(), 4, 5, 6, (5.641)),
-        (ZeroInflatedBinomial(), 3, 4, 7, (0.726, 17.001, 0.375)),
-        (ZeroInflatedBinomial(psi=0.7), 2, 4, 6, (16, 0.362)),
+        (ZeroInflatedBinomial(), 1, 4, 7, (0.683, 12, 0.540)),
+        (ZeroInflatedBinomial(psi=0.7), 2, 4, 6, (9, 0.6322)),
         (ZeroInflatedNegativeBinomial(), 2, 4, 6, (0.87, 5.24, 17.49)),
         (ZeroInflatedNegativeBinomial(psi=0.9), 2, 4, 6, (5.16, 11.32)),
         (ZeroInflatedPoisson(), 4, 5, 6, (1, 5.641)),
         (ZeroInflatedPoisson(psi=0.8), 2, 4, 6, (5.475)),
     ],
 )
 def test_quartile(distribution, q1, q2, q3, result):
```

### Comparing `preliz-0.3.0/preliz/tests/test_roulette.py` & `preliz-0.3.1/preliz/tests/test_roulette.py`

 * *Files identical despite different names*

### Comparing `preliz-0.3.0/preliz/unidimensional/maxent.py` & `preliz-0.3.1/preliz/unidimensional/maxent.py`

 * *Files identical despite different names*

### Comparing `preliz-0.3.0/preliz/unidimensional/mle.py` & `preliz-0.3.1/preliz/unidimensional/mle.py`

 * *Files identical despite different names*

### Comparing `preliz-0.3.0/preliz/unidimensional/quartile.py` & `preliz-0.3.1/preliz/unidimensional/quartile.py`

 * *Files 3% similar despite different names*

```diff
@@ -86,27 +86,24 @@
 
     # Find which parameters has been fixed
     none_idx, fixed = get_fixed_params(distribution)
 
     # Heuristic to provide an initial guess for the optimization step
     # We obtain those guesses by first approximating the mean and standard deviation
     # from the quartiles and then use those values for moment matching
-    distribution._fit_moments(mean=q2, sigma=(q3 - q1) * 1.5)  # pylint:disable=protected-access
+    distribution._fit_moments(mean=q2, sigma=(q3 - q1) / 1.35)  # pylint:disable=protected-access
 
     opt = optimize_quartile(distribution, (q1, q2, q3), none_idx, fixed)
 
-    r_error, computed_mass = relative_error(distribution, q1, q3, 0.5)
+    r_error, _ = relative_error(distribution, q1, q3, 0.5)
 
     if r_error > 0.01:
         _log.info(
-            "The requested mass in the interval (q1=%.2g - q3=%.2g) is 0.5, "
-            "but the computed one is %.2g",
-            q1,
-            q3,
-            computed_mass,
+            "The expected masses are 0.25, 0.5, 0.75\n" "The computed ones are: %.2g, %.2g, %.2g",
+            *distribution.cdf([q1, q2, q3])
         )
 
     if plot:
         ax = distribution.plot_pdf(**plot_kwargs)
         if plot_kwargs.get("pointinterval"):
             cid = -4
         else:
```

### Comparing `preliz-0.3.0/preliz/unidimensional/roulette.py` & `preliz-0.3.1/preliz/unidimensional/roulette.py`

 * *Files identical despite different names*

### Comparing `preliz-0.3.0/pyproject.toml` & `preliz-0.3.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -20,30 +20,34 @@
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
 ]
 dynamic = ["version"]
 description = "The place for all your prior elicitation needs."
 dependencies = [
   "arviz",
-  "numpy>=1.22",
-  "scipy>=1.9.1",
   "matplotlib>=3.5",
-  "nbclient<0.6,>=0.2",
-  "ipywidgets",
-  "ipympl",
+  "numpy>=1.22",
+  "scipy>=1.9.1,<1.11.0",
 ]
 
 [tool.flit.module]
 name = "preliz"
 
 [project.urls]
 source = "https://github.com/arviz-devs/preliz"
 tracker = "https://github.com/arviz-devs/preliz/issues"
 
-
+[project.optional-dependencies]
+full = [
+  "nbclient<0.6,>=0.2",
+  "ipywidgets",
+  "ipympl",
+]
+lab = ["jupyterlab"]
+notebook = ["notebook"]
 
 [tool.black]
 line-length = 100
 
 [tool.isort]
 profile = "black"
 include_trailing_comma = true
```

### Comparing `preliz-0.3.0/PKG-INFO` & `preliz-0.3.1/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,59 +1,77 @@
 Metadata-Version: 2.1
 Name: preliz
-Version: 0.3.0
+Version: 0.3.1
 Summary: The place for all your prior elicitation needs.
 Author-email: ArviZ team <arviz.devs@gmail.com>
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Education
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: arviz
-Requires-Dist: numpy>=1.22
-Requires-Dist: scipy>=1.9.1
 Requires-Dist: matplotlib>=3.5
-Requires-Dist: nbclient<0.6,>=0.2
-Requires-Dist: ipywidgets
-Requires-Dist: ipympl
+Requires-Dist: numpy>=1.22
+Requires-Dist: scipy>=1.9.1,<1.11.0
+Requires-Dist: nbclient<0.6,>=0.2 ; extra == "full"
+Requires-Dist: ipywidgets ; extra == "full"
+Requires-Dist: ipympl ; extra == "full"
+Requires-Dist: jupyterlab ; extra == "lab"
+Requires-Dist: notebook ; extra == "notebook"
 Project-URL: source, https://github.com/arviz-devs/preliz
 Project-URL: tracker, https://github.com/arviz-devs/preliz/issues
+Provides-Extra: full
+Provides-Extra: lab
+Provides-Extra: notebook
 
 <img src="https://raw.githubusercontent.com/arviz-devs/preliz/main/docs/logos/PreliZ.png#gh-light-mode-only" width=200></img>
 <img src="https://raw.githubusercontent.com/arviz-devs/preliz/main/docs/logos/PreliZ_white.png#gh-dark-mode-only" width=200></img>
 
 A tool-box for prior elicitation.
 
 [![PyPi version](https://badge.fury.io/py/preliz.svg)](https://badge.fury.io/py/preliz)
 [![Build Status](https://github.com/arviz-devs/preliz/actions/workflows/test.yml/badge.svg)](https://github.com/arviz-devs/preliz/actions/workflows/test.yml)
 [![codecov](https://codecov.io/gh/arviz-devs/preliz/branch/master/graph/badge.svg?token=SLJIK2O4C5 )](https://codecov.io/gh/arviz-devs/preliz/)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black)
 
 
-
+Prior elicitation refers to the process of transforming the knowledge of a particular domain into well-defined probability distributions. Specifying useful priors is a central aspect of Bayesian statistics. PreliZ is a Python package aimed at helping practitioners choose prior distributions by offering a set of tools for the various facets of prior elicitation. It covers a range of methods, from unidimensional prior elicitation on the parameter space to predictive elicitation on the observed space. The goal is to be compatible with probabilistic programming languages (PPL) in the Python ecosystem like PyMC and PyStan, while remaining agnostic of any specific PPL.
 
 ## Documentation
 
 The PreliZ documentation can be found in the [official docs](https://preliz.readthedocs.io/en/latest/).
 
 ## Installation
 
 ### Last release
 PreliZ is available for installation from [PyPI](https://pypi.org/project/preliz/).
-The latest  version can be installed using pip:
+The latest version (base set of dependencies) can be installed using pip:
 
 ```
 pip install preliz
 ```
+To make use of the interactive features, you can install the optional dependencies:
+
+* For JupyterLab:
+
+```
+pip install "preliz[full,lab]"
+```
+
+* For Jupyter Notebook:
+
+```
+pip install "preliz[full,notebook]"
+```
 
 ### Development
 The latest development version can be installed from the main branch using pip:
 
 ```
 pip install git+git://github.com/arviz-devs/preliz.git
 ```
```

