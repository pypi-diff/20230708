# Comparing `tmp/scikit-rmt-0.6.0.tar.gz` & `tmp/scikit-rmt-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/scikit-rmt-0.6.0.tar", last modified: Wed Jun 21 15:28:57 2023, max compression
+gzip compressed data, was "dist/scikit-rmt-0.6.1.tar", last modified: Sat Jul  8 21:07:00 2023, max compression
```

## Comparing `scikit-rmt-0.6.0.tar` & `scikit-rmt-0.6.1.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxr-xr-x   0 santorum   (501) staff       (20)        0 2023-06-21 15:28:57.597631 scikit-rmt-0.6.0/
--rw-r--r--   0 santorum   (501) staff       (20)      337 2021-05-02 17:28:24.000000 scikit-rmt-0.6.0/.coveragerc
--rw-r--r--   0 santorum   (501) staff       (20)      278 2023-03-09 19:40:44.000000 scikit-rmt-0.6.0/.travis.yml
--rw-r--r--   0 santorum   (501) staff       (20)      382 2023-01-27 19:58:20.000000 scikit-rmt-0.6.0/CITATION.cff
--rw-r--r--   0 santorum   (501) staff       (20)     1563 2021-04-26 20:56:17.000000 scikit-rmt-0.6.0/LICENSE
--rw-r--r--   0 santorum   (501) staff       (20)      346 2023-01-27 19:52:49.000000 scikit-rmt-0.6.0/MANIFEST.in
--rw-r--r--   0 santorum   (501) staff       (20)     2569 2021-05-05 17:08:35.000000 scikit-rmt-0.6.0/Makefile
--rw-r--r--   0 santorum   (501) staff       (20)    23760 2023-06-21 15:28:57.598713 scikit-rmt-0.6.0/PKG-INFO
--rw-r--r--   0 santorum   (501) staff       (20)    19268 2023-06-21 14:56:22.000000 scikit-rmt-0.6.0/README.md
--rw-r--r--   0 santorum   (501) staff       (20)     3189 2023-01-27 19:40:29.000000 scikit-rmt-0.6.0/conf.py
-drwxr-xr-x   0 santorum   (501) staff       (20)        0 2023-06-21 15:28:57.545699 scikit-rmt-0.6.0/docs/
--rw-r--r--   0 santorum   (501) staff       (20)       52 2022-10-04 14:32:13.000000 scikit-rmt-0.6.0/docs/modules.rst
--rw-r--r--   0 santorum   (501) staff       (20)       54 2021-05-08 23:10:40.000000 scikit-rmt-0.6.0/docs/readthedocs-requirements.txt
--rw-r--r--   0 santorum   (501) staff       (20)      522 2022-10-04 14:32:13.000000 scikit-rmt-0.6.0/docs/skrmt.covariance.rst
--rw-r--r--   0 santorum   (501) staff       (20)     1114 2023-06-21 14:56:22.000000 scikit-rmt-0.6.0/docs/skrmt.ensemble.rst
--rw-r--r--   0 santorum   (501) staff       (20)      232 2022-10-04 14:32:13.000000 scikit-rmt-0.6.0/docs/skrmt.rst
-drwxr-xr-x   0 santorum   (501) staff       (20)        0 2023-06-21 15:28:57.558401 scikit-rmt-0.6.0/examples/
--rw-r--r--   0 santorum   (501) staff       (20)       70 2021-05-08 16:13:31.000000 scikit-rmt-0.6.0/examples/README.txt
--rw-r--r--   0 santorum   (501) staff       (20)     2155 2021-05-10 19:43:36.000000 scikit-rmt-0.6.0/examples/plot_boosting_density_representation.py
--rw-r--r--   0 santorum   (501) staff       (20)     2559 2021-05-10 19:22:01.000000 scikit-rmt-0.6.0/examples/plot_circular_ensemble.py
--rw-r--r--   0 santorum   (501) staff       (20)     1385 2022-10-04 14:35:07.000000 scikit-rmt-0.6.0/examples/plot_complex_histograms.py
--rw-r--r--   0 santorum   (501) staff       (20)     2651 2021-05-10 18:16:25.000000 scikit-rmt-0.6.0/examples/plot_gaussian_ensemble.py
--rw-r--r--   0 santorum   (501) staff       (20)     3200 2021-05-10 19:13:42.000000 scikit-rmt-0.6.0/examples/plot_manova_ensemble.py
--rw-r--r--   0 santorum   (501) staff       (20)     2417 2021-05-10 19:07:13.000000 scikit-rmt-0.6.0/examples/plot_wishart_ensemble.py
--rw-r--r--   0 santorum   (501) staff       (20)     2293 2021-05-14 20:07:04.000000 scikit-rmt-0.6.0/index.rst
--rw-r--r--   0 santorum   (501) staff       (20)      506 2023-05-06 11:49:55.000000 scikit-rmt-0.6.0/readthedocs.yml
--rw-r--r--   0 santorum   (501) staff       (20)       66 2023-06-21 14:56:22.000000 scikit-rmt-0.6.0/requirements.txt
-drwxr-xr-x   0 santorum   (501) staff       (20)        0 2023-06-21 15:28:57.566671 scikit-rmt-0.6.0/scikit_rmt.egg-info/
--rw-r--r--   0 santorum   (501) staff       (20)    23760 2023-06-21 15:28:57.000000 scikit-rmt-0.6.0/scikit_rmt.egg-info/PKG-INFO
--rw-r--r--   0 santorum   (501) staff       (20)     1718 2023-06-21 15:28:57.000000 scikit-rmt-0.6.0/scikit_rmt.egg-info/SOURCES.txt
--rw-r--r--   0 santorum   (501) staff       (20)        1 2023-06-21 15:28:57.000000 scikit-rmt-0.6.0/scikit_rmt.egg-info/dependency_links.txt
--rw-r--r--   0 santorum   (501) staff       (20)       67 2023-06-21 15:28:57.000000 scikit-rmt-0.6.0/scikit_rmt.egg-info/requires.txt
--rw-r--r--   0 santorum   (501) staff       (20)        6 2023-06-21 15:28:57.000000 scikit-rmt-0.6.0/scikit_rmt.egg-info/top_level.txt
--rw-r--r--   0 santorum   (501) staff       (20)       38 2023-06-21 15:28:57.602252 scikit-rmt-0.6.0/setup.cfg
--rw-r--r--   0 santorum   (501) staff       (20)     2239 2023-05-06 11:35:01.000000 scikit-rmt-0.6.0/setup.py
-drwxr-xr-x   0 santorum   (501) staff       (20)        0 2023-06-21 15:28:57.569092 scikit-rmt-0.6.0/skrmt/
--rw-r--r--   0 santorum   (501) staff       (20)       95 2023-01-27 19:00:33.000000 scikit-rmt-0.6.0/skrmt/__init__.py
--rw-r--r--   0 santorum   (501) staff       (20)       49 2023-06-21 14:56:22.000000 scikit-rmt-0.6.0/skrmt/_version.py
-drwxr-xr-x   0 santorum   (501) staff       (20)        0 2023-06-21 15:28:57.572410 scikit-rmt-0.6.0/skrmt/covariance/
--rw-r--r--   0 santorum   (501) staff       (20)      734 2021-04-28 22:17:52.000000 scikit-rmt-0.6.0/skrmt/covariance/__init__.py
--rw-r--r--   0 santorum   (501) staff       (20)    10347 2021-05-04 14:06:35.000000 scikit-rmt-0.6.0/skrmt/covariance/estimator.py
--rw-r--r--   0 santorum   (501) staff       (20)     3144 2021-04-28 17:36:36.000000 scikit-rmt-0.6.0/skrmt/covariance/metrics.py
-drwxr-xr-x   0 santorum   (501) staff       (20)        0 2023-06-21 15:28:57.574926 scikit-rmt-0.6.0/skrmt/covariance/tests/
--rw-r--r--   0 santorum   (501) staff       (20)        0 2021-04-13 20:20:47.000000 scikit-rmt-0.6.0/skrmt/covariance/tests/__init__.py
--rw-r--r--   0 santorum   (501) staff       (20)     6356 2021-04-28 22:13:28.000000 scikit-rmt-0.6.0/skrmt/covariance/tests/test_estimator.py
--rw-r--r--   0 santorum   (501) staff       (20)     3823 2021-05-02 17:01:05.000000 scikit-rmt-0.6.0/skrmt/covariance/tests/test_metrics.py
-drwxr-xr-x   0 santorum   (501) staff       (20)        0 2023-06-21 15:28:57.585824 scikit-rmt-0.6.0/skrmt/ensemble/
--rw-r--r--   0 santorum   (501) staff       (20)     1021 2023-06-21 14:56:22.000000 scikit-rmt-0.6.0/skrmt/ensemble/__init__.py
--rw-r--r--   0 santorum   (501) staff       (20)     9337 2023-06-21 14:56:22.000000 scikit-rmt-0.6.0/skrmt/ensemble/_base_ensemble.py
--rw-r--r--   0 santorum   (501) staff       (20)    13146 2023-06-21 14:56:22.000000 scikit-rmt-0.6.0/skrmt/ensemble/circular_ensemble.py
--rw-r--r--   0 santorum   (501) staff       (20)    14462 2023-06-21 14:56:22.000000 scikit-rmt-0.6.0/skrmt/ensemble/gaussian_ensemble.py
--rw-r--r--   0 santorum   (501) staff       (20)    13462 2023-06-21 14:56:22.000000 scikit-rmt-0.6.0/skrmt/ensemble/manova_ensemble.py
--rw-r--r--   0 santorum   (501) staff       (20)    57283 2023-06-21 14:56:22.000000 scikit-rmt-0.6.0/skrmt/ensemble/spectral_law.py
-drwxr-xr-x   0 santorum   (501) staff       (20)        0 2023-06-21 15:28:57.592524 scikit-rmt-0.6.0/skrmt/ensemble/tests/
--rw-r--r--   0 santorum   (501) staff       (20)        0 2021-03-30 20:39:25.000000 scikit-rmt-0.6.0/skrmt/ensemble/tests/__init__.py
--rw-r--r--   0 santorum   (501) staff       (20)      287 2023-06-21 14:56:22.000000 scikit-rmt-0.6.0/skrmt/ensemble/tests/test_base_ens.py
--rw-r--r--   0 santorum   (501) staff       (20)     5714 2023-06-21 14:56:22.000000 scikit-rmt-0.6.0/skrmt/ensemble/tests/test_circular_ens.py
--rw-r--r--   0 santorum   (501) staff       (20)    11926 2023-06-21 14:56:22.000000 scikit-rmt-0.6.0/skrmt/ensemble/tests/test_gaussian_ens.py
--rw-r--r--   0 santorum   (501) staff       (20)     5058 2023-06-21 14:56:22.000000 scikit-rmt-0.6.0/skrmt/ensemble/tests/test_manova_ens.py
--rw-r--r--   0 santorum   (501) staff       (20)    42495 2023-06-21 14:56:22.000000 scikit-rmt-0.6.0/skrmt/ensemble/tests/test_spectral_law.py
--rw-r--r--   0 santorum   (501) staff       (20)     1611 2023-01-05 15:04:32.000000 scikit-rmt-0.6.0/skrmt/ensemble/tests/test_tracy_widom_approx.py
--rw-r--r--   0 santorum   (501) staff       (20)     1200 2021-05-04 14:00:53.000000 scikit-rmt-0.6.0/skrmt/ensemble/tests/test_tridiagonalization.py
--rw-r--r--   0 santorum   (501) staff       (20)    14668 2023-06-21 14:56:22.000000 scikit-rmt-0.6.0/skrmt/ensemble/tests/test_wishart_ens.py
--rw-r--r--   0 santorum   (501) staff       (20)    33083 2023-05-06 11:35:01.000000 scikit-rmt-0.6.0/skrmt/ensemble/tracy_widom_approximator.py
--rw-r--r--   0 santorum   (501) staff       (20)     6028 2023-05-06 11:35:01.000000 scikit-rmt-0.6.0/skrmt/ensemble/tridiagonal_utils.py
--rw-r--r--   0 santorum   (501) staff       (20)    16015 2023-06-21 14:56:22.000000 scikit-rmt-0.6.0/skrmt/ensemble/wishart_ensemble.py
-drwxr-xr-x   0 santorum   (501) staff       (20)        0 2023-06-21 15:28:57.596444 scikit-rmt-0.6.0/tutorial/
--rw-r--r--   0 santorum   (501) staff       (20)       64 2021-05-09 15:49:23.000000 scikit-rmt-0.6.0/tutorial/README.txt
--rw-r--r--   0 santorum   (501) staff       (20)     2706 2023-06-21 14:56:22.000000 scikit-rmt-0.6.0/tutorial/plot_0_introduction.py
--rw-r--r--   0 santorum   (501) staff       (20)    10272 2023-06-21 14:56:22.000000 scikit-rmt-0.6.0/tutorial/plot_1_spectral_laws.py
--rw-r--r--   0 santorum   (501) staff       (20)     9176 2023-06-21 15:09:01.000000 scikit-rmt-0.6.0/tutorial/plot_2_plot_spectral_laws.py
+drwxr-xr-x   0 santorum   (501) staff       (20)        0 2023-07-08 21:07:00.387165 scikit-rmt-0.6.1/
+-rw-r--r--   0 santorum   (501) staff       (20)      337 2021-05-02 17:28:24.000000 scikit-rmt-0.6.1/.coveragerc
+-rw-r--r--   0 santorum   (501) staff       (20)      278 2023-03-09 19:40:44.000000 scikit-rmt-0.6.1/.travis.yml
+-rw-r--r--   0 santorum   (501) staff       (20)      382 2023-01-27 19:58:20.000000 scikit-rmt-0.6.1/CITATION.cff
+-rw-r--r--   0 santorum   (501) staff       (20)     1563 2021-04-26 20:56:17.000000 scikit-rmt-0.6.1/LICENSE
+-rw-r--r--   0 santorum   (501) staff       (20)      346 2023-01-27 19:52:49.000000 scikit-rmt-0.6.1/MANIFEST.in
+-rw-r--r--   0 santorum   (501) staff       (20)     2569 2021-05-05 17:08:35.000000 scikit-rmt-0.6.1/Makefile
+-rw-r--r--   0 santorum   (501) staff       (20)    23760 2023-07-08 21:07:00.387626 scikit-rmt-0.6.1/PKG-INFO
+-rw-r--r--   0 santorum   (501) staff       (20)    19268 2023-06-21 14:56:22.000000 scikit-rmt-0.6.1/README.md
+-rw-r--r--   0 santorum   (501) staff       (20)     3189 2023-01-27 19:40:29.000000 scikit-rmt-0.6.1/conf.py
+drwxr-xr-x   0 santorum   (501) staff       (20)        0 2023-07-08 21:07:00.340109 scikit-rmt-0.6.1/docs/
+-rw-r--r--   0 santorum   (501) staff       (20)       52 2022-10-04 14:32:13.000000 scikit-rmt-0.6.1/docs/modules.rst
+-rw-r--r--   0 santorum   (501) staff       (20)       54 2021-05-08 23:10:40.000000 scikit-rmt-0.6.1/docs/readthedocs-requirements.txt
+-rw-r--r--   0 santorum   (501) staff       (20)      522 2022-10-04 14:32:13.000000 scikit-rmt-0.6.1/docs/skrmt.covariance.rst
+-rw-r--r--   0 santorum   (501) staff       (20)     1114 2023-06-21 14:56:22.000000 scikit-rmt-0.6.1/docs/skrmt.ensemble.rst
+-rw-r--r--   0 santorum   (501) staff       (20)      232 2022-10-04 14:32:13.000000 scikit-rmt-0.6.1/docs/skrmt.rst
+drwxr-xr-x   0 santorum   (501) staff       (20)        0 2023-07-08 21:07:00.345620 scikit-rmt-0.6.1/examples/
+-rw-r--r--   0 santorum   (501) staff       (20)       70 2021-05-08 16:13:31.000000 scikit-rmt-0.6.1/examples/README.txt
+-rw-r--r--   0 santorum   (501) staff       (20)     2155 2023-07-08 20:47:44.000000 scikit-rmt-0.6.1/examples/plot_boosting_density_representation.py
+-rw-r--r--   0 santorum   (501) staff       (20)     2559 2021-05-10 19:22:01.000000 scikit-rmt-0.6.1/examples/plot_circular_ensemble.py
+-rw-r--r--   0 santorum   (501) staff       (20)     1385 2022-10-04 14:35:07.000000 scikit-rmt-0.6.1/examples/plot_complex_histograms.py
+-rw-r--r--   0 santorum   (501) staff       (20)     2651 2021-05-10 18:16:25.000000 scikit-rmt-0.6.1/examples/plot_gaussian_ensemble.py
+-rw-r--r--   0 santorum   (501) staff       (20)     3200 2021-05-10 19:13:42.000000 scikit-rmt-0.6.1/examples/plot_manova_ensemble.py
+-rw-r--r--   0 santorum   (501) staff       (20)     2417 2021-05-10 19:07:13.000000 scikit-rmt-0.6.1/examples/plot_wishart_ensemble.py
+-rw-r--r--   0 santorum   (501) staff       (20)     2293 2021-05-14 20:07:04.000000 scikit-rmt-0.6.1/index.rst
+-rw-r--r--   0 santorum   (501) staff       (20)      506 2023-05-06 11:49:55.000000 scikit-rmt-0.6.1/readthedocs.yml
+-rw-r--r--   0 santorum   (501) staff       (20)       66 2023-06-21 14:56:22.000000 scikit-rmt-0.6.1/requirements.txt
+drwxr-xr-x   0 santorum   (501) staff       (20)        0 2023-07-08 21:07:00.350303 scikit-rmt-0.6.1/scikit_rmt.egg-info/
+-rw-r--r--   0 santorum   (501) staff       (20)    23760 2023-07-08 21:07:00.000000 scikit-rmt-0.6.1/scikit_rmt.egg-info/PKG-INFO
+-rw-r--r--   0 santorum   (501) staff       (20)     1718 2023-07-08 21:07:00.000000 scikit-rmt-0.6.1/scikit_rmt.egg-info/SOURCES.txt
+-rw-r--r--   0 santorum   (501) staff       (20)        1 2023-07-08 21:07:00.000000 scikit-rmt-0.6.1/scikit_rmt.egg-info/dependency_links.txt
+-rw-r--r--   0 santorum   (501) staff       (20)       67 2023-07-08 21:07:00.000000 scikit-rmt-0.6.1/scikit_rmt.egg-info/requires.txt
+-rw-r--r--   0 santorum   (501) staff       (20)        6 2023-07-08 21:07:00.000000 scikit-rmt-0.6.1/scikit_rmt.egg-info/top_level.txt
+-rw-r--r--   0 santorum   (501) staff       (20)       38 2023-07-08 21:07:00.388242 scikit-rmt-0.6.1/setup.cfg
+-rw-r--r--   0 santorum   (501) staff       (20)     2239 2023-05-06 11:35:01.000000 scikit-rmt-0.6.1/setup.py
+drwxr-xr-x   0 santorum   (501) staff       (20)        0 2023-07-08 21:07:00.351812 scikit-rmt-0.6.1/skrmt/
+-rw-r--r--   0 santorum   (501) staff       (20)       95 2023-01-27 19:00:33.000000 scikit-rmt-0.6.1/skrmt/__init__.py
+-rw-r--r--   0 santorum   (501) staff       (20)       49 2023-07-06 19:32:53.000000 scikit-rmt-0.6.1/skrmt/_version.py
+drwxr-xr-x   0 santorum   (501) staff       (20)        0 2023-07-08 21:07:00.354789 scikit-rmt-0.6.1/skrmt/covariance/
+-rw-r--r--   0 santorum   (501) staff       (20)      734 2021-04-28 22:17:52.000000 scikit-rmt-0.6.1/skrmt/covariance/__init__.py
+-rw-r--r--   0 santorum   (501) staff       (20)    10347 2021-05-04 14:06:35.000000 scikit-rmt-0.6.1/skrmt/covariance/estimator.py
+-rw-r--r--   0 santorum   (501) staff       (20)     3144 2021-04-28 17:36:36.000000 scikit-rmt-0.6.1/skrmt/covariance/metrics.py
+drwxr-xr-x   0 santorum   (501) staff       (20)        0 2023-07-08 21:07:00.357234 scikit-rmt-0.6.1/skrmt/covariance/tests/
+-rw-r--r--   0 santorum   (501) staff       (20)        0 2021-04-13 20:20:47.000000 scikit-rmt-0.6.1/skrmt/covariance/tests/__init__.py
+-rw-r--r--   0 santorum   (501) staff       (20)     6356 2021-04-28 22:13:28.000000 scikit-rmt-0.6.1/skrmt/covariance/tests/test_estimator.py
+-rw-r--r--   0 santorum   (501) staff       (20)     3823 2021-05-02 17:01:05.000000 scikit-rmt-0.6.1/skrmt/covariance/tests/test_metrics.py
+drwxr-xr-x   0 santorum   (501) staff       (20)        0 2023-07-08 21:07:00.368282 scikit-rmt-0.6.1/skrmt/ensemble/
+-rw-r--r--   0 santorum   (501) staff       (20)     1021 2023-06-21 14:56:22.000000 scikit-rmt-0.6.1/skrmt/ensemble/__init__.py
+-rw-r--r--   0 santorum   (501) staff       (20)     9693 2023-07-08 21:05:42.000000 scikit-rmt-0.6.1/skrmt/ensemble/_base_ensemble.py
+-rw-r--r--   0 santorum   (501) staff       (20)    13737 2023-07-08 21:05:42.000000 scikit-rmt-0.6.1/skrmt/ensemble/circular_ensemble.py
+-rw-r--r--   0 santorum   (501) staff       (20)    14984 2023-07-08 21:05:42.000000 scikit-rmt-0.6.1/skrmt/ensemble/gaussian_ensemble.py
+-rw-r--r--   0 santorum   (501) staff       (20)    13881 2023-07-08 21:05:42.000000 scikit-rmt-0.6.1/skrmt/ensemble/manova_ensemble.py
+-rw-r--r--   0 santorum   (501) staff       (20)    56082 2023-07-08 21:05:42.000000 scikit-rmt-0.6.1/skrmt/ensemble/spectral_law.py
+drwxr-xr-x   0 santorum   (501) staff       (20)        0 2023-07-08 21:07:00.383580 scikit-rmt-0.6.1/skrmt/ensemble/tests/
+-rw-r--r--   0 santorum   (501) staff       (20)        0 2021-03-30 20:39:25.000000 scikit-rmt-0.6.1/skrmt/ensemble/tests/__init__.py
+-rw-r--r--   0 santorum   (501) staff       (20)      287 2023-07-08 21:05:42.000000 scikit-rmt-0.6.1/skrmt/ensemble/tests/test_base_ens.py
+-rw-r--r--   0 santorum   (501) staff       (20)     5714 2023-06-21 14:56:22.000000 scikit-rmt-0.6.1/skrmt/ensemble/tests/test_circular_ens.py
+-rw-r--r--   0 santorum   (501) staff       (20)    11926 2023-07-08 21:05:42.000000 scikit-rmt-0.6.1/skrmt/ensemble/tests/test_gaussian_ens.py
+-rw-r--r--   0 santorum   (501) staff       (20)     5058 2023-06-21 14:56:22.000000 scikit-rmt-0.6.1/skrmt/ensemble/tests/test_manova_ens.py
+-rw-r--r--   0 santorum   (501) staff       (20)    42454 2023-07-06 19:27:12.000000 scikit-rmt-0.6.1/skrmt/ensemble/tests/test_spectral_law.py
+-rw-r--r--   0 santorum   (501) staff       (20)     1611 2023-01-05 15:04:32.000000 scikit-rmt-0.6.1/skrmt/ensemble/tests/test_tracy_widom_approx.py
+-rw-r--r--   0 santorum   (501) staff       (20)     1200 2021-05-04 14:00:53.000000 scikit-rmt-0.6.1/skrmt/ensemble/tests/test_tridiagonalization.py
+-rw-r--r--   0 santorum   (501) staff       (20)    14668 2023-07-08 21:05:42.000000 scikit-rmt-0.6.1/skrmt/ensemble/tests/test_wishart_ens.py
+-rw-r--r--   0 santorum   (501) staff       (20)    33083 2023-05-06 11:35:01.000000 scikit-rmt-0.6.1/skrmt/ensemble/tracy_widom_approximator.py
+-rw-r--r--   0 santorum   (501) staff       (20)     6028 2023-05-06 11:35:01.000000 scikit-rmt-0.6.1/skrmt/ensemble/tridiagonal_utils.py
+-rw-r--r--   0 santorum   (501) staff       (20)    16537 2023-07-08 21:05:42.000000 scikit-rmt-0.6.1/skrmt/ensemble/wishart_ensemble.py
+drwxr-xr-x   0 santorum   (501) staff       (20)        0 2023-07-08 21:07:00.386580 scikit-rmt-0.6.1/tutorial/
+-rw-r--r--   0 santorum   (501) staff       (20)       64 2021-05-09 15:49:23.000000 scikit-rmt-0.6.1/tutorial/README.txt
+-rw-r--r--   0 santorum   (501) staff       (20)     2706 2023-07-08 21:05:42.000000 scikit-rmt-0.6.1/tutorial/plot_0_introduction.py
+-rw-r--r--   0 santorum   (501) staff       (20)    10272 2023-06-21 14:56:22.000000 scikit-rmt-0.6.1/tutorial/plot_1_spectral_laws.py
+-rw-r--r--   0 santorum   (501) staff       (20)     9176 2023-07-08 21:05:42.000000 scikit-rmt-0.6.1/tutorial/plot_2_plot_spectral_laws.py
```

### Comparing `scikit-rmt-0.6.0/LICENSE` & `scikit-rmt-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `scikit-rmt-0.6.0/Makefile` & `scikit-rmt-0.6.1/Makefile`

 * *Files identical despite different names*

### Comparing `scikit-rmt-0.6.0/PKG-INFO` & `scikit-rmt-0.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: scikit-rmt
-Version: 0.6.0
+Version: 0.6.1
 Summary: Random Matrix Theory Python package
 Home-page: https://github.com/AlejandroSantorum/scikit-rmt
 Author: Alejandro Santorum Varela
 Author-email: alejandro.santorum@gmail.com
 License: BSD
-Download-URL: https://github.com/AlejandroSantorum/scikit-rmt/archive/refs/tags/v0.6.0.tar.gz
+Download-URL: https://github.com/AlejandroSantorum/scikit-rmt/archive/refs/tags/v0.6.1.tar.gz
 Description: ![scikit-rmt logo](https://raw.githubusercontent.com/AlejandroSantorum/scikit-rmt/main/imgs/scikit-rmt_logo_bigger.png)
         
         
         [![PyPI](https://img.shields.io/pypi/v/scikit-rmt?color=g)](https://pypi.org/project/scikit-rmt/)
         [![Documentation Status](https://readthedocs.org/projects/scikit-rmt/badge/?version=latest)](https://scikit-rmt.readthedocs.io/en/latest/?badge=latest)
         [![Build Status](https://travis-ci.com/AlejandroSantorum/scikit-rmt.svg?branch=main)](https://travis-ci.com/AlejandroSantorum/scikit-rmt)
         [![codecov](https://codecov.io/gh/AlejandroSantorum/scikit-rmt/branch/main/graph/badge.svg?token=56TNEASPJK)](https://codecov.io/gh/AlejandroSantorum/scikit-rmt)
```

### Comparing `scikit-rmt-0.6.0/README.md` & `scikit-rmt-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `scikit-rmt-0.6.0/conf.py` & `scikit-rmt-0.6.1/conf.py`

 * *Files identical despite different names*

### Comparing `scikit-rmt-0.6.0/docs/skrmt.covariance.rst` & `scikit-rmt-0.6.1/docs/skrmt.covariance.rst`

 * *Files identical despite different names*

### Comparing `scikit-rmt-0.6.0/docs/skrmt.ensemble.rst` & `scikit-rmt-0.6.1/docs/skrmt.ensemble.rst`

 * *Files identical despite different names*

### Comparing `scikit-rmt-0.6.0/examples/plot_boosting_density_representation.py` & `scikit-rmt-0.6.1/examples/plot_boosting_density_representation.py`

 * *Files identical despite different names*

### Comparing `scikit-rmt-0.6.0/examples/plot_circular_ensemble.py` & `scikit-rmt-0.6.1/examples/plot_circular_ensemble.py`

 * *Files identical despite different names*

### Comparing `scikit-rmt-0.6.0/examples/plot_complex_histograms.py` & `scikit-rmt-0.6.1/examples/plot_complex_histograms.py`

 * *Files identical despite different names*

### Comparing `scikit-rmt-0.6.0/examples/plot_gaussian_ensemble.py` & `scikit-rmt-0.6.1/examples/plot_gaussian_ensemble.py`

 * *Files identical despite different names*

### Comparing `scikit-rmt-0.6.0/examples/plot_manova_ensemble.py` & `scikit-rmt-0.6.1/examples/plot_manova_ensemble.py`

 * *Files identical despite different names*

### Comparing `scikit-rmt-0.6.0/examples/plot_wishart_ensemble.py` & `scikit-rmt-0.6.1/examples/plot_wishart_ensemble.py`

 * *Files identical despite different names*

### Comparing `scikit-rmt-0.6.0/index.rst` & `scikit-rmt-0.6.1/index.rst`

 * *Files identical despite different names*

### Comparing `scikit-rmt-0.6.0/scikit_rmt.egg-info/PKG-INFO` & `scikit-rmt-0.6.1/scikit_rmt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: scikit-rmt
-Version: 0.6.0
+Version: 0.6.1
 Summary: Random Matrix Theory Python package
 Home-page: https://github.com/AlejandroSantorum/scikit-rmt
 Author: Alejandro Santorum Varela
 Author-email: alejandro.santorum@gmail.com
 License: BSD
-Download-URL: https://github.com/AlejandroSantorum/scikit-rmt/archive/refs/tags/v0.6.0.tar.gz
+Download-URL: https://github.com/AlejandroSantorum/scikit-rmt/archive/refs/tags/v0.6.1.tar.gz
 Description: ![scikit-rmt logo](https://raw.githubusercontent.com/AlejandroSantorum/scikit-rmt/main/imgs/scikit-rmt_logo_bigger.png)
         
         
         [![PyPI](https://img.shields.io/pypi/v/scikit-rmt?color=g)](https://pypi.org/project/scikit-rmt/)
         [![Documentation Status](https://readthedocs.org/projects/scikit-rmt/badge/?version=latest)](https://scikit-rmt.readthedocs.io/en/latest/?badge=latest)
         [![Build Status](https://travis-ci.com/AlejandroSantorum/scikit-rmt.svg?branch=main)](https://travis-ci.com/AlejandroSantorum/scikit-rmt)
         [![codecov](https://codecov.io/gh/AlejandroSantorum/scikit-rmt/branch/main/graph/badge.svg?token=56TNEASPJK)](https://codecov.io/gh/AlejandroSantorum/scikit-rmt)
```

### Comparing `scikit-rmt-0.6.0/scikit_rmt.egg-info/SOURCES.txt` & `scikit-rmt-0.6.1/scikit_rmt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scikit-rmt-0.6.0/setup.py` & `scikit-rmt-0.6.1/setup.py`

 * *Files identical despite different names*

### Comparing `scikit-rmt-0.6.0/skrmt/covariance/__init__.py` & `scikit-rmt-0.6.1/skrmt/covariance/__init__.py`

 * *Files identical despite different names*

### Comparing `scikit-rmt-0.6.0/skrmt/covariance/estimator.py` & `scikit-rmt-0.6.1/skrmt/covariance/estimator.py`

 * *Files identical despite different names*

### Comparing `scikit-rmt-0.6.0/skrmt/covariance/metrics.py` & `scikit-rmt-0.6.1/skrmt/covariance/metrics.py`

 * *Files identical despite different names*

### Comparing `scikit-rmt-0.6.0/skrmt/covariance/tests/test_estimator.py` & `scikit-rmt-0.6.1/skrmt/covariance/tests/test_estimator.py`

 * *Files identical despite different names*

### Comparing `scikit-rmt-0.6.0/skrmt/covariance/tests/test_metrics.py` & `scikit-rmt-0.6.1/skrmt/covariance/tests/test_metrics.py`

 * *Files identical despite different names*

### Comparing `scikit-rmt-0.6.0/skrmt/ensemble/__init__.py` & `scikit-rmt-0.6.1/skrmt/ensemble/__init__.py`

 * *Files identical despite different names*

### Comparing `scikit-rmt-0.6.0/skrmt/ensemble/_base_ensemble.py` & `scikit-rmt-0.6.1/skrmt/ensemble/_base_ensemble.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,20 +22,25 @@
     This class contains common attributes and methods for all the
     ensembles. It also defines the basic interface to be
     supported by inherited classes.
 
     Attributes:
         matrix (numpy array): instance of the random matrix ensemble
             of size n times n.
-
+        _eigvals (numpy array): array of computed eigenvalues. This array
+            is None until the method `eigvals` is called. The computed
+            eigenvalues are cached in the attribute _eigvals to avoid
+            re-computing them. The eigenvalues are re-calculated again
+            if the matrix sample changes.
     """
 
     @abstractmethod
     def __init__(self):
         self.matrix = None
+        self._eigvals = None
 
     @abstractmethod
     def sample(self):
         """Samples new random matrix.
 
         The sampling algorithm depends on the inherited classes, so it should be
         specified by them.
```

### Comparing `scikit-rmt-0.6.0/skrmt/ensemble/circular_ensemble.py` & `scikit-rmt-0.6.1/skrmt/ensemble/circular_ensemble.py`

 * *Files 5% similar despite different names*

```diff
@@ -139,31 +139,37 @@
             return self._sample_cse()
 
     def _sample_coe(self):
         # sampling unitary Haar-distributed matrix
         u_mtx = _sample_haar_mtx(self.n)
         # mapping to Circular Orthogonal Ensemble
         self.matrix = np.matmul(u_mtx.transpose(), u_mtx)
+        # setting array of eigenvalues to None to force re-computing them
+        self._eigvals = None
         return self.matrix
 
     def _sample_cue(self):
         # sampling unitary Haar-distributed matrix
         self.matrix = _sample_haar_mtx(self.n)
+        # setting array of eigenvalues to None to force re-computing them
+        self._eigvals = None
         return self.matrix
 
     def _sample_cse(self):
         # sampling unitary Haar-distributed matrix of size 2n
         u_mtx = _sample_haar_mtx(2*self.n)
         # mapping to Circular Symplectic Ensemble
         j_mtx = self._build_j_mtx()
         # U_R = J * U^T * J^T
         u_r_aux = np.matmul(j_mtx, u_mtx.transpose())
         u_r_mtx = np.matmul(u_r_aux, j_mtx.transpose())
         # A = U^R * U
         self.matrix = np.matmul(u_r_mtx, u_mtx)
+        # setting array of eigenvalues to None to force re-computing them
+        self._eigvals = None
         return self.matrix
 
     def _build_j_mtx(self):
         """Creates an useful matrix to sample CSE matrices.
 
         Creates matrix J of zeros but with the upper-diagonal
         set to -1 and the lower-diagonal set to 1. This matrix
@@ -199,17 +205,25 @@
         Calculates the random matrix eigenvalues using numpy standard procedure.
         If the matrix ensemble is symmetric, a faster algorithm is used.
 
         Returns:
             numpy array with the calculated eigenvalues.
 
         """
+        if self._eigvals is not None:
+            return self._eigvals
+
         if self.beta == 1:
-            return np.linalg.eigvalsh(self.matrix)
-        return np.linalg.eigvals(self.matrix)
+            # using eigvalsh because it's known all eigenvalues are real
+            self._eigvals = np.linalg.eigvalsh(self.matrix)
+        else:
+            # using eigvals since some eigenvalues could be imaginary
+            self._eigvals = np.linalg.eigvals(self.matrix)
+
+        return self._eigvals
 
     def plot_eigval_hist(self, bins, interval=None, density=False, norm_const=None, fig_path=None):
         """Computes and plots the histogram of the matrix eigenvalues.
 
         Calculates and plots the histogram of the current sampled matrix eigenvalues.
         It is important to underline that this function works with real and complex
         eigenvalues: if the matrix eigenvalues are complex, they are plotted in the
```

### Comparing `scikit-rmt-0.6.0/skrmt/ensemble/gaussian_ensemble.py` & `scikit-rmt-0.6.1/skrmt/ensemble/gaussian_ensemble.py`

 * *Files 6% similar despite different names*

```diff
@@ -136,22 +136,26 @@
             return self._sample_gse()
 
     def _sample_goe(self):
         # n by n matrix of random Gaussians
         mtx = np.random.randn(self.n,self.n) * self.sigma
         # symmetrize matrix
         self.matrix = (mtx + mtx.transpose())/np.sqrt(2)
+        # setting array of eigenvalues to None to force re-computing them
+        self._eigvals = None
         return self.matrix
 
     def _sample_gue(self):
         size = self.n
         # n by n random complex matrix
         mtx = np.random.randn(size,size)*self.sigma + 1j*np.random.randn(size,size)*self.sigma
         # hermitian matrix
         self.matrix = (mtx + mtx.transpose().conj())/np.sqrt(2)
+        # setting array of eigenvalues to None to force re-computing them
+        self._eigvals = None
         return self.matrix
 
     def _sample_gse(self):
         size = self.n
         # n by n random complex matrix
         x_mtx = np.random.randn(size,size)*self.sigma + 1j*np.random.randn(size,size)*self.sigma
         # another n by n random complex matrix
@@ -159,14 +163,16 @@
         # [X Y; -conj(Y) conj(X)]
         mtx = np.block([
                        [x_mtx               , y_mtx],
                        [-np.conjugate(y_mtx), np.conjugate(x_mtx)]
                         ])
         # hermitian matrix
         self.matrix = (mtx + mtx.transpose().conj())/np.sqrt(2)
+        # setting array of eigenvalues to None to force re-computing them
+        self._eigvals = None
         return self.matrix
 
     def sample_tridiagonal(self):
         '''Samples a Gaussian Ensemble random matrix in its tridiagonal form.
 
         Samples a random matrix of the specified Gaussian Ensemble (remember,
         beta=1 is GOE, beta=2 is GUE and beta=4 is GSE) in its tridiagonal
@@ -196,27 +202,33 @@
         chisqs = (1/np.sqrt(2)) * \
                  np.array([np.sqrt(np.random.chisquare(df*self.beta)) for df in dfs])
         # inserting diagonals
         diagonals = [chisqs, normals, chisqs]
         mtx = sparse.diags(diagonals, [-1, 0, 1])
         # converting to numpy array
         self.matrix = mtx.toarray()
+        # setting array of eigenvalues to None to force re-computing them
+        self._eigvals = None
         return self.matrix
 
     def eigvals(self):
         """Computes the random matrix eigenvalues.
 
         Calculates the random matrix eigenvalues using numpy standard procedure.
         If the matrix ensemble is symmetric, a faster algorithm is used.
 
         Returns:
             numpy array with the calculated eigenvalues.
 
         """
-        return np.linalg.eigvalsh(self.matrix)
+        if self._eigvals is not None:
+            return self._eigvals
+
+        self._eigvals = np.linalg.eigvalsh(self.matrix)
+        return self._eigvals
 
     def eigval_hist(self, bins, interval=None, density=False, norm_const=None, avoid_img=False):
         if self.use_tridiagonal:
             if norm_const:
                 return tridiag_eigval_hist(self.matrix*norm_const, bins=bins,
                                            interval=interval, density=density)
             return tridiag_eigval_hist(self.matrix, bins=bins, interval=interval, density=density)
```

### Comparing `scikit-rmt-0.6.0/skrmt/ensemble/manova_ensemble.py` & `scikit-rmt-0.6.1/skrmt/ensemble/manova_ensemble.py`

 * *Files 2% similar despite different names*

```diff
@@ -148,14 +148,16 @@
         y_mtx = np.random.randn(m_size,n2_size)
         # A1 = X * X'
         a1_mtx = np.matmul(x_mtx, x_mtx.transpose())
         # A2 = X * X' + Y * Y'
         a2_mtx = a1_mtx + np.matmul(y_mtx, y_mtx.transpose())
         # A = (X * X') / (X * X' + Y * Y') = (X * X') * (X * X' + Y * Y')^(-1)
         self.matrix = np.matmul(a1_mtx, np.linalg.inv(a2_mtx))
+        # setting array of eigenvalues to None to force re-computing them
+        self._eigvals = None
         return self.matrix
 
     def _sample_mce(self):
         m_size = self.m
         n1_size = self.n1
         n2_size = self.n2
         # m by n1 random complex matrix of random Gaussians
@@ -164,14 +166,16 @@
         y_mtx = np.random.randn(m_size,n2_size) + (0+1j)*np.random.randn(m_size,n2_size)
         # A1 = X * X'
         a1_mtx = np.matmul(x_mtx, x_mtx.transpose().conj())
         # A2 = X * X' + Y * Y'
         a2_mtx = a1_mtx + np.matmul(y_mtx, y_mtx.transpose().conj())
         # A = (X * X') / (X * X' + Y * Y') = (X * X') * (X * X' + Y * Y')^(-1)
         self.matrix = np.matmul(a1_mtx, np.linalg.inv(a2_mtx))
+        # setting array of eigenvalues to None to force re-computing them
+        self._eigvals = None
         return self.matrix
 
     def _sample_mqe(self):
         m_size = self.m
         n1_size = self.n1
         n2_size = self.n2
         # m by n1 random complex matrix of random Gaussians
@@ -194,27 +198,33 @@
                         ])
         # A1 = X * X'
         a1_mtx = np.matmul(x_mtx, x_mtx.transpose().conj())
         # A2 = X * X' + Y * Y'
         a2_mtx = a1_mtx + np.matmul(y_mtx, y_mtx.transpose().conj())
         # A = (X * X') / (X * X' + Y * Y') = (X * X') * (X * X' + Y * Y')^(-1)
         self.matrix = np.matmul(a1_mtx, np.linalg.inv(a2_mtx))
+        # setting array of eigenvalues to None to force re-computing them
+        self._eigvals = None
         return self.matrix
 
     def eigvals(self):
         """Computes the random matrix eigenvalues.
 
         Calculates the random matrix eigenvalues using numpy standard procedure.
         If the matrix ensemble is symmetric, a faster algorithm is used.
 
         Returns:
             numpy array with the calculated eigenvalues.
 
         """
-        return np.linalg.eigvals(self.matrix)
+        if self._eigvals is not None:
+            return self._eigvals
+
+        self._eigvals = np.linalg.eigvals(self.matrix)
+        return self._eigvals
 
     def plot_eigval_hist(self, bins, interval=(0,1), density=False, norm_const=None, fig_path=None):
         """Computes and plots the histogram of the matrix eigenvalues
 
         Calculates and plots the histogram of the current sampled matrix eigenvalues.
 
         Args:
```

### Comparing `scikit-rmt-0.6.0/skrmt/ensemble/spectral_law.py` & `scikit-rmt-0.6.1/skrmt/ensemble/spectral_law.py`

 * *Files 1% similar despite different names*

```diff
@@ -184,37 +184,31 @@
         if beta not in [1,2,4]:
             raise ValueError(f"Error: invalid beta. It has to be 1,2 or 4. Provided beta = {beta}.")
 
         self.beta = beta
         self.center = center
         self.sigma = sigma
         self.radius = 2.0 * np.sqrt(self.beta) * self.sigma
-        self._gaussian_ens = None
     
     def rvs(self, size):
         """Samples ranfom variates following this distribution.
+        This uses the relationship between Wigner Semicircle law and Beta distribution.
 
         Args:
             size (int): sample size.
         
         Returns:
             numpy array with the generated samples.
         """
         if size <= 0:
             raise ValueError(f"Error: invalid sample size. It has to be positive. Provided size = {size}.")
-        
-        if not self._gaussian_ens:
-            self._gaussian_ens = GaussianEnsemble(beta=self.beta, n=size, use_tridiagonal=False, sigma=self.sigma)
-        else:
-            self._gaussian_ens.set_size(size, resample_mtx=True)
-        
-        _eigval_norm_const = 1/np.sqrt(size)
-        if self.beta == 4:
-            return _eigval_norm_const * self._gaussian_ens.eigvals()[::2]
-        return _eigval_norm_const * self._gaussian_ens.eigvals()
+
+        # Use relationship with beta distribution
+        beta_samples = np.random.beta(1.5, 1.5, size=size)
+        return self.center + 2*self.radius*beta_samples - self.radius
 
     def pdf(self, x):
         """Computes PDF of the Wigner Semicircle Law.
 
         Args:
             x (float or ndarray): value or (numpy) array of values in which compute the PDF.
         
@@ -281,23 +275,24 @@
             interval, func=self.cdf, bins=bins, 
             plot_ylabel="cumulative distribution", savefig_path=savefig_path
         )
     
 
     def plot_empirical_pdf(self, n_size=1000, bins=100, interval=None, density=False,
                            plot_law_pdf=False, savefig_path=None):
-        """Computes and plots Wigner's semicircle empirical law using Gaussian Ensemble.
+        """Computes and plots Wigner's semicircle empirical law.
 
-        Calculates and plots Wigner's semicircle empirical law using Gaussian Ensemble
-        random matrices. Gaussian (Hermite) ensemble has improved routines (using
-        tridiagonal forms and Sturm sequences) to avoid calculating the eigenvalues,
-        so the histogram is built using certain techniques to boost efficiency.
+        Calculates and plots Wigner's semicircle empirical law using random samples generated
+        using the relationship between the Wigner Semicircle law and the Beta distribution:
+        the Wigner's Semicircle distribution it is a scaled Beta distribution with parameters
+        :math:`\alpha = \beta = 3/2`.
 
         Args:
-            n_size (int, default=1000): random matrix size n times n. This is the sample size.
+            n_size (int, default=1000): number of random samples that can be interpreted as
+                random eigenvalues of a Wigner matrix. This is the sample size.
             bins (int or sequence, default=100): If bins is an integer, it defines the number
                 of equal-width bins in the range. If bins is a sequence, it defines the
                 bin edges, including the left edge of the first bin and the right
                 edge of the last bin; in this case, bins may be unequally spaced.
             interval (tuple, default=None): Delimiters (xmin, xmax) of the histogram.
                 The lower and upper range of the bins. Lower and upper outliers are ignored.
             density (bool, default=False): If True, draw and return a probability
@@ -320,50 +315,29 @@
                 Journal of Mathematical Physics. 43.11 (2002): 5830-5847.
 
         """
         # pylint: disable=too-many-arguments
         if n_size<1:
             raise ValueError("matrix size must be positive")
 
-        if self.center != 0.0:
-            print(f"Warning: The given center is not 0.0 (center = {self.center}).\n"
-                  "\t It is only available the centered empirical Wigner's semicircle law.")
-        
-        use_tridiag = (self.sigma == 1.0)
-        if not use_tridiag:
-            print(f"Warning: The given scale is not the standard (sigma = {self.sigma}).\n"
-                "\t Tridiagonal histogramming is deactivated.\n"
-                "\t It is adviced to set sigma=1.0 to optimize and boost histogramming.")
-
-        ens = GaussianEnsemble(beta=self.beta, n=n_size, sigma=self.sigma, use_tridiagonal=use_tridiag)
-
-        # default plotting interval in case it's not provided
-        if interval is None:
-            interval = (-self.radius, self.radius)
-
-        # Wigner eigenvalue normalization constant
-        if use_tridiag:
-            norm_const = 1/np.sqrt(n_size) if self.beta==4 else 1/np.sqrt(n_size/2)
-        else:
-            norm_const = 1/np.sqrt(n_size)
+        random_samples = self.rvs(size=n_size)
+        observed, bins = np.histogram(random_samples, bins=bins, range=interval, density=density)
 
-        observed, bins = ens.eigval_hist(bins=bins, interval=interval,
-                                        density=density, norm_const=norm_const)
         width = bins[1]-bins[0]
         plt.bar(bins[:-1], observed, width=width, align='edge')
 
         # Plotting Wigner Semicircle Law pdf
         if plot_law_pdf and density:
             centers = np.asarray(_get_bins_centers_and_contour(bins))
             pdf = self.pdf(centers)
             plt.plot(centers, pdf, color='red', linewidth=2)
         elif plot_law_pdf and not density:
             print("Warning: Wigner's Semicircle Law PDF is only plotted when density is True.")
 
-        plt.title("Wigner Semicircle Law - Empirical density histogram", fontweight="bold")
+        plt.title("Wigner Semicircle Law - Eigenvalue histogram", fontweight="bold")
         plt.xlabel("x")
         plt.ylabel("probability density")
 
         # Saving plot or showing it
         if savefig_path:
             plt.savefig(savefig_path, dpi=1200)
         else:
```

### Comparing `scikit-rmt-0.6.0/skrmt/ensemble/tests/test_circular_ens.py` & `scikit-rmt-0.6.1/skrmt/ensemble/tests/test_circular_ens.py`

 * *Files identical despite different names*

### Comparing `scikit-rmt-0.6.0/skrmt/ensemble/tests/test_gaussian_ens.py` & `scikit-rmt-0.6.1/skrmt/ensemble/tests/test_gaussian_ens.py`

 * *Files identical despite different names*

### Comparing `scikit-rmt-0.6.0/skrmt/ensemble/tests/test_manova_ens.py` & `scikit-rmt-0.6.1/skrmt/ensemble/tests/test_manova_ens.py`

 * *Files identical despite different names*

### Comparing `scikit-rmt-0.6.0/skrmt/ensemble/tests/test_spectral_law.py` & `scikit-rmt-0.6.1/skrmt/ensemble/tests/test_spectral_law.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,15 +54,14 @@
 
         wsd = WignerSemicircleDistribution(beta=beta, sigma=sigma)
 
         assert wsd.beta == beta
         assert wsd.center == 0.0
         assert wsd.sigma == sigma
         assert wsd.radius == 2.0 * np.sqrt(beta) * sigma
-        assert wsd._gaussian_ens is None
     
     def test_wsd_init_raise(self):
         '''Testing WignerSemicircleDistribution init raising exception
         '''
         with pytest.raises(ValueError):
             _ = WignerSemicircleDistribution(beta=3)
```

### Comparing `scikit-rmt-0.6.0/skrmt/ensemble/tests/test_tracy_widom_approx.py` & `scikit-rmt-0.6.1/skrmt/ensemble/tests/test_tracy_widom_approx.py`

 * *Files identical despite different names*

### Comparing `scikit-rmt-0.6.0/skrmt/ensemble/tests/test_tridiagonalization.py` & `scikit-rmt-0.6.1/skrmt/ensemble/tests/test_tridiagonalization.py`

 * *Files identical despite different names*

### Comparing `scikit-rmt-0.6.0/skrmt/ensemble/tests/test_wishart_ens.py` & `scikit-rmt-0.6.1/skrmt/ensemble/tests/test_wishart_ens.py`

 * *Files identical despite different names*

### Comparing `scikit-rmt-0.6.0/skrmt/ensemble/tracy_widom_approximator.py` & `scikit-rmt-0.6.1/skrmt/ensemble/tracy_widom_approximator.py`

 * *Files identical despite different names*

### Comparing `scikit-rmt-0.6.0/skrmt/ensemble/tridiagonal_utils.py` & `scikit-rmt-0.6.1/skrmt/ensemble/tridiagonal_utils.py`

 * *Files identical despite different names*

### Comparing `scikit-rmt-0.6.0/skrmt/ensemble/wishart_ensemble.py` & `scikit-rmt-0.6.1/skrmt/ensemble/wishart_ensemble.py`

 * *Files 3% similar despite different names*

```diff
@@ -159,23 +159,27 @@
     def _sample_wre(self):
         p_size = self.p
         n_size = self.n
         # p by n matrix of random Gaussians
         mtx = np.random.randn(p_size,n_size) * self.sigma
         # symmetrize matrix
         self.matrix = np.matmul(mtx, mtx.transpose())
+        # setting array of eigenvalues to None to force re-computing them
+        self._eigvals = None
         return self.matrix
 
     def _sample_wce(self):
         p_size = self.p
         n_size = self.n
         # p by n random complex matrix of random Gaussians
         mtx = np.random.randn(p_size,n_size)*self.sigma + 1j*np.random.randn(p_size,n_size)*self.sigma
         # hermitian matrix
         self.matrix = np.matmul(mtx, mtx.transpose().conj())
+        # setting array of eigenvalues to None to force re-computing them
+        self._eigvals = None
         return self.matrix
 
     def _sample_wqe(self):
         p_size = self.p
         n_size = self.n
         # p by n random complex matrix of random Gaussians
         x_mtx = np.random.randn(p_size,n_size)*self.sigma + 1j*np.random.randn(p_size,n_size)*self.sigma
@@ -184,14 +188,16 @@
         # [X Y; -conj(Y) conj(X)]
         mtx = np.block([
                         [x_mtx              , y_mtx],
                         [-np.conjugate(y_mtx), np.conjugate(x_mtx)]
                     ])
         # hermitian matrix
         self.matrix = np.matmul(mtx, mtx.transpose().conj())
+        # setting array of eigenvalues to None to force re-computing them
+        self._eigvals = None
         return self.matrix
 
     def sample_tridiagonal(self):
         '''Samples a Wishart Ensemble random matrix in its tridiagonal form.
 
         Samples a random matrix of the specified Wishart Ensemble (remember,
         beta=1 is Real, beta=2 is Complex and beta=4 is Quaternion) in its
@@ -219,28 +225,34 @@
                          chisqs_offdiag[i]**2 for i in range(self.p-1)])
         offdiag = np.multiply(chisqs_offdiag, chisqs_diag[:-1])
         # inserting diagonals
         diagonals = [offdiag, diag, offdiag]
         mtx = sparse.diags(diagonals, [-1, 0, 1])
         # converting to numpy array
         self.matrix = mtx.toarray()
+        # setting array of eigenvalues to None to force re-computing them
+        self._eigvals = None
         return self.matrix
 
 
     def eigvals(self):
         """Computes the random matrix eigenvalues.
 
         Calculates the random matrix eigenvalues using numpy standard procedure.
         If the matrix ensemble is symmetric, a faster algorithm is used.
 
         Returns:
             numpy array with the calculated eigenvalues.
 
         """
-        return np.linalg.eigvalsh(self.matrix)
+        if self._eigvals is not None:
+            return self._eigvals
+
+        self._eigvals = np.linalg.eigvalsh(self.matrix)
+        return self._eigvals
 
     def eigval_hist(self, bins, interval=None, density=False, norm_const=None, avoid_img=False):
         if self.use_tridiagonal:
             if norm_const:
                 return tridiag_eigval_hist(self.matrix*norm_const, bins=bins,
                                            interval=interval, density=density)
             return tridiag_eigval_hist(self.matrix, bins=bins, interval=interval, density=density)
```

### Comparing `scikit-rmt-0.6.0/tutorial/plot_0_introduction.py` & `scikit-rmt-0.6.1/tutorial/plot_0_introduction.py`

 * *Files identical despite different names*

### Comparing `scikit-rmt-0.6.0/tutorial/plot_1_spectral_laws.py` & `scikit-rmt-0.6.1/tutorial/plot_1_spectral_laws.py`

 * *Files identical despite different names*

### Comparing `scikit-rmt-0.6.0/tutorial/plot_2_plot_spectral_laws.py` & `scikit-rmt-0.6.1/tutorial/plot_2_plot_spectral_laws.py`

 * *Files identical despite different names*

