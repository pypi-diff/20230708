# Comparing `tmp/ligo.skymap-1.1.0.tar.gz` & `tmp/ligo.skymap-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ligo.skymap-1.1.0.tar", last modified: Fri Jul  7 17:47:37 2023, max compression
+gzip compressed data, was "ligo.skymap-1.1.1.tar", last modified: Sat Jul  8 17:33:18 2023, max compression
```

## Comparing `ligo.skymap-1.1.0.tar` & `ligo.skymap-1.1.1.tar`

### file list

```diff
@@ -1,294 +1,294 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 17:47:37.555839 ligo.skymap-1.1.0/
--rw-rw-rw-   0 root         (0) root         (0)      602 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/.gitignore
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 17:47:37.516839 ligo.skymap-1.1.0/.gitlab/
--rwxrwxrwx   0 root         (0) root         (0)     2033 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/.gitlab/combine-coverage.py
--rw-rw-rw-   0 root         (0) root         (0)    12513 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)    42221 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/CHANGES.rst
--rw-rw-rw-   0 root         (0) root         (0)      677 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/CONTRIBUTING.rst
--rw-rw-rw-   0 root         (0) root         (0)      286 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     4216 2023-07-07 17:47:37.556839 ligo.skymap-1.1.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2777 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 17:47:37.509839 ligo.skymap-1.1.0/cextern/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 17:47:37.516839 ligo.skymap-1.1.0/cextern/chealpix/
--rw-rw-rw-   0 root         (0) root         (0)    30207 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/cextern/chealpix/chealpix.c
--rw-rw-rw-   0 root         (0) root         (0)     7407 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/cextern/chealpix/chealpix.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 17:47:37.518839 ligo.skymap-1.1.0/docs/
--rw-rw-rw-   0 root         (0) root         (0)     4581 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/docs/Makefile
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 17:47:37.519839 ligo.skymap-1.1.0/docs/_static/
--rw-rw-rw-   0 root         (0) root         (0)    39163 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/docs/_static/benchmark.svg
--rw-rw-rw-   0 root         (0) root         (0)   567737 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/docs/_static/coinc.xml
--rw-rw-rw-   0 root         (0) root         (0)   260305 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/docs/_static/localization.svg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 17:47:37.509839 ligo.skymap-1.1.0/docs/_templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 17:47:37.520839 ligo.skymap-1.1.0/docs/_templates/autosummary/
--rw-rw-rw-   0 root         (0) root         (0)      250 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/docs/_templates/autosummary/base.rst
--rw-rw-rw-   0 root         (0) root         (0)      251 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/docs/_templates/autosummary/class.rst
--rw-rw-rw-   0 root         (0) root         (0)      252 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/docs/_templates/autosummary/module.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 17:47:37.520839 ligo.skymap-1.1.0/docs/bayestar/
--rw-rw-rw-   0 root         (0) root         (0)    56171 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/docs/bayestar/eggbox.png
--rw-rw-rw-   0 root         (0) root         (0)      212 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/docs/bayestar/ez_emcee.rst
--rw-rw-rw-   0 root         (0) root         (0)      182 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/docs/bayestar/filter.rst
--rw-rw-rw-   0 root         (0) root         (0)      309 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/docs/bayestar/index.rst
--rw-rw-rw-   0 root         (0) root         (0)      225 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/docs/bayestar/interpolation.rst
--rw-rw-rw-   0 root         (0) root         (0)    42221 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/docs/changes.rst
--rw-rw-rw-   0 root         (0) root         (0)     8638 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/docs/conf.py
--rw-rw-rw-   0 root         (0) root         (0)      677 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/docs/contributing.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 17:47:37.521839 ligo.skymap-1.1.0/docs/coordinates/
--rw-rw-rw-   0 root         (0) root         (0)      191 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/docs/coordinates/detector.rst
--rw-rw-rw-   0 root         (0) root         (0)      189 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/docs/coordinates/eigenframe.rst
--rw-rw-rw-   0 root         (0) root         (0)     2304 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/docs/develop.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 17:47:37.521839 ligo.skymap-1.1.0/docs/distance/
--rw-rw-rw-   0 root         (0) root         (0)     1243 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/docs/distance/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 17:47:37.521839 ligo.skymap-1.1.0/docs/healpix_tree/
--rw-rw-rw-   0 root         (0) root         (0)      165 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/docs/healpix_tree/index.rst
--rw-rw-rw-   0 root         (0) root         (0)      595 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/docs/help.rst
--rw-rw-rw-   0 root         (0) root         (0)     4574 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/docs/index.rst
--rw-rw-rw-   0 root         (0) root         (0)    15650 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/docs/interface.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 17:47:37.521839 ligo.skymap-1.1.0/docs/io/
--rw-rw-rw-   0 root         (0) root         (0)     3691 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/docs/io/events.rst
--rw-rw-rw-   0 root         (0) root         (0)      146 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/docs/io/fits.rst
--rw-rw-rw-   0 root         (0) root         (0)      166 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/docs/io/hdf5.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 17:47:37.522839 ligo.skymap-1.1.0/docs/kde/
--rw-rw-rw-   0 root         (0) root         (0)      162 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/docs/kde/index.rst
--rw-rw-rw-   0 root         (0) root         (0)     4549 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/docs/make.bat
--rw-rw-rw-   0 root         (0) root         (0)       13 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/docs/matplotlibrc
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 17:47:37.522839 ligo.skymap-1.1.0/docs/moc/
--rw-rw-rw-   0 root         (0) root         (0)      267 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/docs/moc/index.rst
--rw-rw-rw-   0 root         (0) root         (0)     1282 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/docs/performance.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 17:47:37.523839 ligo.skymap-1.1.0/docs/plot/
--rw-rw-rw-   0 root         (0) root         (0)      186 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/docs/plot/allsky.rst
--rw-rw-rw-   0 root         (0) root         (0)      198 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/docs/plot/backdrop.rst
--rw-rw-rw-   0 root         (0) root         (0)      206 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/docs/plot/bayes_factor.rst
--rw-rw-rw-   0 root         (0) root         (0)      205 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/docs/plot/marker.rst
--rw-rw-rw-   0 root         (0) root         (0)      166 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/docs/plot/poly.rst
--rw-rw-rw-   0 root         (0) root         (0)      182 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/docs/plot/pp.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 17:47:37.524839 ligo.skymap-1.1.0/docs/postprocess/
--rw-rw-rw-   0 root         (0) root         (0)      180 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/docs/postprocess/contour.rst
--rw-rw-rw-   0 root         (0) root         (0)      184 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/docs/postprocess/cosmology.rst
--rw-rw-rw-   0 root         (0) root         (0)      253 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/docs/postprocess/crossmatch.rst
--rw-rw-rw-   0 root         (0) root         (0)      200 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/docs/postprocess/ellipse.rst
--rw-rw-rw-   0 root         (0) root         (0)      195 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/docs/postprocess/util.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 17:47:37.524839 ligo.skymap-1.1.0/docs/quickstart/
--rw-rw-rw-   0 root         (0) root         (0)     6351 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/docs/quickstart/bayestar-injections.rst
--rw-rw-rw-   0 root         (0) root         (0)     4156 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/docs/quickstart/install.rst
--rw-rw-rw-   0 root         (0) root         (0)     1595 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/docs/testing.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 17:47:37.527839 ligo.skymap-1.1.0/docs/tool/
--rw-rw-rw-   0 root         (0) root         (0)      314 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/docs/tool/bayestar_inject.rst
--rw-rw-rw-   0 root         (0) root         (0)      188 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/docs/tool/bayestar_localize_coincs.rst
--rw-rw-rw-   0 root         (0) root         (0)      204 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/docs/tool/bayestar_localize_lvalert.rst
--rw-rw-rw-   0 root         (0) root         (0)      189 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/docs/tool/bayestar_mcmc.rst
--rw-rw-rw-   0 root         (0) root         (0)      179 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/docs/tool/bayestar_realize_coincs.rst
--rw-rw-rw-   0 root         (0) root         (0)      175 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/docs/tool/bayestar_sample_model_psd.rst
--rw-rw-rw-   0 root         (0) root         (0)      175 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/docs/tool/index.rst
--rw-rw-rw-   0 root         (0) root         (0)     1400 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/docs/tool/ligo_skymap_combine.rst
--rw-rw-rw-   0 root         (0) root         (0)     3709 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/docs/tool/ligo_skymap_constellations.rst
--rw-rw-rw-   0 root         (0) root         (0)      165 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/docs/tool/ligo_skymap_contour.rst
--rw-rw-rw-   0 root         (0) root         (0)      215 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/docs/tool/ligo_skymap_contour_moc.rst
--rw-rw-rw-   0 root         (0) root         (0)      199 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/docs/tool/ligo_skymap_flatten.rst
--rw-rw-rw-   0 root         (0) root         (0)     1387 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/docs/tool/ligo_skymap_from_samples.rst
--rw-rw-rw-   0 root         (0) root         (0)      747 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/docs/tool/ligo_skymap_plot.rst
--rw-rw-rw-   0 root         (0) root         (0)      795 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/docs/tool/ligo_skymap_plot_airmass.rst
--rw-rw-rw-   0 root         (0) root         (0)      779 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/docs/tool/ligo_skymap_plot_coherence.rst
--rw-rw-rw-   0 root         (0) root         (0)     1121 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/docs/tool/ligo_skymap_plot_observability.rst
--rw-rw-rw-   0 root         (0) root         (0)      188 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/docs/tool/ligo_skymap_plot_stats.rst
--rw-rw-rw-   0 root         (0) root         (0)      700 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/docs/tool/ligo_skymap_plot_volume.rst
--rw-rw-rw-   0 root         (0) root         (0)      177 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/docs/tool/ligo_skymap_stats.rst
--rw-rw-rw-   0 root         (0) root         (0)      209 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/docs/tool/ligo_skymap_unflatten.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 17:47:37.528839 ligo.skymap-1.1.0/docs/util/
--rw-rw-rw-   0 root         (0) root         (0)      158 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/docs/util/file.rst
--rw-rw-rw-   0 root         (0) root         (0)      172 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/docs/util/ilwd.rst
--rw-rw-rw-   0 root         (0) root         (0)      163 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/docs/util/numpy.rst
--rw-rw-rw-   0 root         (0) root         (0)      168 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/docs/util/sqlite.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 17:47:37.529839 ligo.skymap-1.1.0/licenses/
--rw-rw-rw-   0 root         (0) root         (0)     6360 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/licenses/CHEALPIX_LICENSE.rst
--rw-rw-rw-   0 root         (0) root         (0)    37565 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/licenses/LICENSE.rst
--rw-rw-rw-   0 root         (0) root         (0)     1792 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/licenses/NUMPY_LICENSE.rst
--rw-rw-rw-   0 root         (0) root         (0)      372 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/licenses/README.rst
--rw-rw-rw-   0 root         (0) root         (0)     1659 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/licenses/TEMPLATE_LICENCE.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 17:47:37.511839 ligo.skymap-1.1.0/ligo/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 17:47:37.531839 ligo.skymap-1.1.0/ligo/skymap/
--rw-rw-rw-   0 root         (0) root         (0)     1012 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      698 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/_astropy_init.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 17:47:37.532839 ligo.skymap-1.1.0/ligo/skymap/bayestar/
--rw-rw-rw-   0 root         (0) root         (0)    20852 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/bayestar/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5864 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/bayestar/ez_emcee.py
--rw-rw-rw-   0 root         (0) root         (0)    19685 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/bayestar/filter.py
--rw-rw-rw-   0 root         (0) root         (0)    10348 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/bayestar/interpolation.py
--rw-rw-rw-   0 root         (0) root         (0)     2176 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/bayestar/ptemcee.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 17:47:37.532839 ligo.skymap-1.1.0/ligo/skymap/bayestar/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/bayestar/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1545 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/bayestar/tests/test_bayestar.py
--rw-rw-rw-   0 root         (0) root         (0)     4573 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/bayestar/tests/test_interpolation.py
--rw-rw-rw-   0 root         (0) root         (0)     4287 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/bayestar/tests/test_signal_amplitude_model.py
--rw-rw-rw-   0 root         (0) root         (0)     2321 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/conftest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 17:47:37.533839 ligo.skymap-1.1.0/ligo/skymap/coordinates/
--rw-rw-rw-   0 root         (0) root         (0)      382 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/coordinates/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3645 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/coordinates/detector.py
--rw-rw-rw-   0 root         (0) root         (0)     4132 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/coordinates/eigenframe.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 17:47:37.533839 ligo.skymap-1.1.0/ligo/skymap/coordinates/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/coordinates/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      996 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/coordinates/tests/test_detector.py
--rw-rw-rw-   0 root         (0) root         (0)    20879 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/distance.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 17:47:37.533839 ligo.skymap-1.1.0/ligo/skymap/extern/
--rw-rw-rw-   0 root         (0) root         (0)      460 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/extern/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 17:47:37.534839 ligo.skymap-1.1.0/ligo/skymap/extern/numpy/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/extern/numpy/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    13938 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/extern/numpy/quantile.py
--rw-rw-rw-   0 root         (0) root         (0)    15264 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/healpix_tree.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 17:47:37.534839 ligo.skymap-1.1.0/ligo/skymap/io/
--rw-rw-rw-   0 root         (0) root         (0)      382 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/io/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 17:47:37.536839 ligo.skymap-1.1.0/ligo/skymap/io/events/
--rw-rw-rw-   0 root         (0) root         (0)      382 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/io/events/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3832 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/io/events/base.py
--rw-rw-rw-   0 root         (0) root         (0)     2664 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/io/events/detector_disabled.py
--rw-rw-rw-   0 root         (0) root         (0)     2274 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/io/events/gracedb.py
--rw-rw-rw-   0 root         (0) root         (0)     7809 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/io/events/hdf.py
--rw-rw-rw-   0 root         (0) root         (0)    11345 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/io/events/ligolw.py
--rw-rw-rw-   0 root         (0) root         (0)     2563 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/io/events/magic.py
--rw-rw-rw-   0 root         (0) root         (0)     1700 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/io/events/sqlite.py
--rwxrwxrwx   0 root         (0) root         (0)    19227 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/io/fits.py
--rwxrwxrwx   0 root         (0) root         (0)    10598 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/io/hdf5.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 17:47:37.536839 ligo.skymap-1.1.0/ligo/skymap/io/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/io/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 17:47:37.537839 ligo.skymap-1.1.0/ligo/skymap/io/tests/data/
--rw-rw-rw-   0 root         (0) root         (0)   492938 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/io/tests/data/2016_subset.xml.gz
--rw-rw-rw-   0 root         (0) root         (0)     1699 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/io/tests/data/G197392_coinc.xml.gz
--rw-rw-rw-   0 root         (0) root         (0)      675 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/io/tests/data/G197392_psd.xml.gz
--rw-rw-rw-   0 root         (0) root         (0)     2470 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/io/tests/data/G211117_coinc.xml.gz
--rw-rw-rw-   0 root         (0) root         (0)     2355 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/io/tests/data/G211117_psd.xml.gz
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/io/tests/data/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 17:47:37.538839 ligo.skymap-1.1.0/ligo/skymap/io/tests/data/gstlal_reference_psd/
--rw-rw-rw-   0 root         (0) root         (0)      717 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/io/tests/data/gstlal_reference_psd/H1L1V1-REFERENCE_PSD-967234210-29963.xml.gz
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/io/tests/data/gstlal_reference_psd/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9120 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/io/tests/data/test.hdf5
--rw-rw-rw-   0 root         (0) root         (0)    12598 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/io/tests/test_io_events.py
--rw-rw-rw-   0 root         (0) root         (0)    17043 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/kde.py
--rw-rw-rw-   0 root         (0) root         (0)     7533 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/moc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 17:47:37.540839 ligo.skymap-1.1.0/ligo/skymap/plot/
--rw-rw-rw-   0 root         (0) root         (0)      382 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/plot/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    29184 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/plot/allsky.py
--rw-rw-rw-   0 root         (0) root         (0)     1415 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/plot/angle.py
--rw-rw-rw-   0 root         (0) root         (0)     7291 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/plot/backdrop.py
--rw-rw-rw-   0 root         (0) root         (0)     3910 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/plot/bayes_factor.py
--rw-rw-rw-   0 root         (0) root         (0)     1522 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/plot/cmap.py
--rw-rw-rw-   0 root         (0) root         (0)     8714 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/plot/cylon.csv
--rw-rw-rw-   0 root         (0) root         (0)     2125 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/plot/cylon.py
--rw-rw-rw-   0 root         (0) root         (0)     2933 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/plot/marker.py
--rw-rw-rw-   0 root         (0) root         (0)    63275 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/plot/ne_simplified_coastline.json
--rw-rw-rw-   0 root         (0) root         (0)     7394 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/plot/poly.py
--rw-rw-rw-   0 root         (0) root         (0)     9445 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/plot/pp.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 17:47:37.540839 ligo.skymap-1.1.0/ligo/skymap/plot/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/plot/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 17:47:37.544839 ligo.skymap-1.1.0/ligo/skymap/plot/tests/baseline/
--rw-rw-rw-   0 root         (0) root         (0)    67690 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/plot/tests/baseline/test_allsky_axes_astro-degrees-aitoff.png
--rw-rw-rw-   0 root         (0) root         (0)    65830 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/plot/tests/baseline/test_allsky_axes_astro-degrees-mollweide.png
--rw-rw-rw-   0 root         (0) root         (0)    65829 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/plot/tests/baseline/test_allsky_axes_astro-hours-aitoff.png
--rw-rw-rw-   0 root         (0) root         (0)    63879 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/plot/tests/baseline/test_allsky_axes_astro-hours-mollweide.png
--rw-rw-rw-   0 root         (0) root         (0)    71762 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/plot/tests/baseline/test_allsky_axes_galactic-degrees-aitoff.png
--rw-rw-rw-   0 root         (0) root         (0)    71509 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/plot/tests/baseline/test_allsky_axes_galactic-degrees-mollweide.png
--rw-rw-rw-   0 root         (0) root         (0)    70497 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/plot/tests/baseline/test_allsky_axes_galactic-hours-aitoff.png
--rw-rw-rw-   0 root         (0) root         (0)    69334 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/plot/tests/baseline/test_allsky_axes_galactic-hours-mollweide.png
--rw-rw-rw-   0 root         (0) root         (0)    64896 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/plot/tests/baseline/test_allsky_axes_geo-degrees-aitoff.png
--rw-rw-rw-   0 root         (0) root         (0)    63732 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/plot/tests/baseline/test_allsky_axes_geo-degrees-mollweide.png
--rw-rw-rw-   0 root         (0) root         (0)    63470 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/plot/tests/baseline/test_allsky_axes_geo-hours-aitoff.png
--rw-rw-rw-   0 root         (0) root         (0)    61561 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/plot/tests/baseline/test_allsky_axes_geo-hours-mollweide.png
--rw-rw-rw-   0 root         (0) root         (0)    33964 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/plot/tests/baseline/test_allsky_obstime.png
--rw-rw-rw-   0 root         (0) root         (0)    20330 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/plot/tests/baseline/test_globe_axes.png
--rw-rw-rw-   0 root         (0) root         (0)    19092 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/plot/tests/baseline/test_pp_plot_default.png
--rw-rw-rw-   0 root         (0) root         (0)    39991 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/plot/tests/baseline/test_pp_plot_lines.png
--rw-rw-rw-   0 root         (0) root         (0)    19092 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/plot/tests/baseline/test_pp_plot_steps.png
--rw-rw-rw-   0 root         (0) root         (0)     8866 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/plot/tests/baseline/test_reticle.png
--rw-rw-rw-   0 root         (0) root         (0)    19815 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/plot/tests/baseline/test_zoom_axes.png
--rw-rw-rw-   0 root         (0) root         (0)     5202 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/plot/tests/test_plot.py
--rw-rw-rw-   0 root         (0) root         (0)     2400 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/plot/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 17:47:37.545839 ligo.skymap-1.1.0/ligo/skymap/postprocess/
--rw-rw-rw-   0 root         (0) root         (0)      382 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/postprocess/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6348 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/postprocess/contour.py
--rw-rw-rw-   0 root         (0) root         (0)     2407 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/postprocess/cosmology.py
--rw-rw-rw-   0 root         (0) root         (0)    18664 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/postprocess/crossmatch.py
--rw-rw-rw-   0 root         (0) root         (0)    15257 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/postprocess/ellipse.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 17:47:37.546839 ligo.skymap-1.1.0/ligo/skymap/postprocess/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/postprocess/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      899 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/postprocess/tests/test_cosmology.py
--rw-rw-rw-   0 root         (0) root         (0)     4373 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/postprocess/tests/test_crossmatch.py
--rw-rw-rw-   0 root         (0) root         (0)     3219 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/postprocess/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 17:47:37.546839 ligo.skymap-1.1.0/ligo/skymap/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 17:47:37.546839 ligo.skymap-1.1.0/ligo/skymap/tests/plugins/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/tests/plugins/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      578 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/tests/plugins/omp.py
--rw-rw-rw-   0 root         (0) root         (0)     4831 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/tests/test_moc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 17:47:37.550839 ligo.skymap-1.1.0/ligo/skymap/tool/
--rw-rw-rw-   0 root         (0) root         (0)    15669 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/tool/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    21608 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/tool/bayestar_inject.py
--rw-rw-rw-   0 root         (0) root         (0)     7538 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/tool/bayestar_localize_coincs.py
--rwxrwxrwx   0 root         (0) root         (0)     6821 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/tool/bayestar_localize_lvalert.py
--rw-rw-rw-   0 root         (0) root         (0)     8137 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/tool/bayestar_mcmc.py
--rw-rw-rw-   0 root         (0) root         (0)    18761 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/tool/bayestar_realize_coincs.py
--rw-rw-rw-   0 root         (0) root         (0)     4600 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/tool/bayestar_sample_model_psd.py
--rw-rw-rw-   0 root         (0) root         (0)     5841 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/tool/ligo_skymap_combine.py
--rw-rw-rw-   0 root         (0) root         (0)     2011 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/tool/ligo_skymap_constellations.py
--rw-rw-rw-   0 root         (0) root         (0)     3341 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/tool/ligo_skymap_contour.py
--rw-rw-rw-   0 root         (0) root         (0)     2519 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/tool/ligo_skymap_contour_moc.py
--rw-rw-rw-   0 root         (0) root         (0)     2288 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/tool/ligo_skymap_flatten.py
--rw-rw-rw-   0 root         (0) root         (0)     7662 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/tool/ligo_skymap_from_samples.py
--rw-rw-rw-   0 root         (0) root         (0)     6732 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/tool/ligo_skymap_plot.py
--rw-rw-rw-   0 root         (0) root         (0)     8353 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/tool/ligo_skymap_plot_airmass.py
--rw-rw-rw-   0 root         (0) root         (0)     1713 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/tool/ligo_skymap_plot_coherence.py
--rw-rw-rw-   0 root         (0) root         (0)     5711 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/tool/ligo_skymap_plot_observability.py
--rw-rw-rw-   0 root         (0) root         (0)     5158 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/tool/ligo_skymap_plot_pp_samples.py
--rw-rw-rw-   0 root         (0) root         (0)     8048 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/tool/ligo_skymap_plot_stats.py
--rwxrwxrwx   0 root         (0) root         (0)     9404 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/tool/ligo_skymap_plot_volume.py
--rw-rw-rw-   0 root         (0) root         (0)    11830 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/tool/ligo_skymap_stats.py
--rw-rw-rw-   0 root         (0) root         (0)     1739 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/tool/ligo_skymap_unflatten.py
--rw-rw-rw-   0 root         (0) root         (0)     4508 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/tool/matplotlib.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 17:47:37.551839 ligo.skymap-1.1.0/ligo/skymap/tool/tests/
--rw-rw-rw-   0 root         (0) root         (0)     3064 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/tool/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5271 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/tool/tests/test_bayestar.py
--rw-rw-rw-   0 root         (0) root         (0)     4494 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/tool/tests/test_bayestar_inject.py
--rw-rw-rw-   0 root         (0) root         (0)     2400 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/tool/tests/test_combine.py
--rw-rw-rw-   0 root         (0) root         (0)     4015 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/tool/tests/test_flatten.py
--rw-rw-rw-   0 root         (0) root         (0)     2631 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/tool/tests/test_from_samples.py
--rw-rw-rw-   0 root         (0) root         (0)      529 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/tool/tests/test_help.py
--rw-rw-rw-   0 root         (0) root         (0)     1826 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/tool/tests/test_plot.py
--rw-rw-rw-   0 root         (0) root         (0)     2065 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/tool/tests/test_plot_stats.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 17:47:37.552839 ligo.skymap-1.1.0/ligo/skymap/util/
--rw-rw-rw-   0 root         (0) root         (0)      382 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/util/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1794 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/util/file.py
--rw-rw-rw-   0 root         (0) root         (0)     5163 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/util/ilwd.py
--rw-rw-rw-   0 root         (0) root         (0)     1680 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/util/numpy.py
--rw-rw-rw-   0 root         (0) root         (0)     2854 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/util/progress.py
--rw-rw-rw-   0 root         (0) root         (0)     4451 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/util/sqlite.py
--rw-rw-rw-   0 root         (0) root         (0)     2694 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/util/stopwatch.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 17:47:37.553839 ligo.skymap-1.1.0/ligo/skymap/util/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/util/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      363 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/util/tests/test_progress.py
--rw-r--r--   0 root         (0) root         (0)      337 2023-07-07 17:47:37.000000 ligo.skymap-1.1.0/ligo/skymap/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 17:47:37.530839 ligo.skymap-1.1.0/ligo.skymap.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4216 2023-07-07 17:47:37.000000 ligo.skymap-1.1.0/ligo.skymap.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     8311 2023-07-07 17:47:37.000000 ligo.skymap-1.1.0/ligo.skymap.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-07 17:47:37.000000 ligo.skymap-1.1.0/ligo.skymap.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)     1550 2023-07-07 17:47:37.000000 ligo.skymap-1.1.0/ligo.skymap.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-07 17:47:37.000000 ligo.skymap-1.1.0/ligo.skymap.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      432 2023-07-07 17:47:37.000000 ligo.skymap-1.1.0/ligo.skymap.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2023-07-07 17:47:37.000000 ligo.skymap-1.1.0/ligo.skymap.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      355 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)     6429 2023-07-07 17:47:37.557839 ligo.skymap-1.1.0/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     3574 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 17:47:37.555839 ligo.skymap-1.1.0/src/
--rw-rw-rw-   0 root         (0) root         (0)    37062 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/src/bayestar_cosmology.h
--rw-rw-rw-   0 root         (0) root         (0)     4078 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/src/bayestar_cosmology.py
--rw-rw-rw-   0 root         (0) root         (0)    15859 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/src/bayestar_distance.c
--rw-rw-rw-   0 root         (0) root         (0)     2067 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/src/bayestar_distance.h
--rw-rw-rw-   0 root         (0) root         (0)     4025 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/src/bayestar_moc.c
--rw-rw-rw-   0 root         (0) root         (0)     1492 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/src/bayestar_moc.h
--rw-rw-rw-   0 root         (0) root         (0)    53672 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/src/bayestar_sky_map.c
--rw-rw-rw-   0 root         (0) root         (0)     7887 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/src/bayestar_sky_map.h
--rw-rw-rw-   0 root         (0) root         (0)      218 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/src/branch_prediction.h
--rw-rw-rw-   0 root         (0) root         (0)    39503 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/src/core.c
--rw-rw-rw-   0 root         (0) root         (0)     5818 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/src/cubic_interp.c
--rw-rw-rw-   0 root         (0) root         (0)     2069 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/src/cubic_interp.h
--rw-rw-rw-   0 root         (0) root         (0)    13016 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/src/cubic_interp_test.c
--rw-rw-rw-   0 root         (0) root         (0)     6370 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/src/omp_interruptible.h
--rw-rw-rw-   0 root         (0) root         (0)     2377 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/src/vmath.h
--rw-rw-rw-   0 root         (0) root         (0)     1869 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/src/warnings.h
--rw-rw-rw-   0 root         (0) root         (0)     2595 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/tox.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-08 17:33:18.762179 ligo.skymap-1.1.1/
+-rw-rw-rw-   0 root         (0) root         (0)      602 2023-07-06 20:38:49.000000 ligo.skymap-1.1.1/.gitignore
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-08 17:33:18.668176 ligo.skymap-1.1.1/.gitlab/
+-rwxrwxrwx   0 root         (0) root         (0)     2033 2023-07-06 20:38:49.000000 ligo.skymap-1.1.1/.gitlab/combine-coverage.py
+-rw-rw-rw-   0 root         (0) root         (0)    12513 2023-07-06 20:38:49.000000 ligo.skymap-1.1.1/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)    42428 2023-07-08 17:32:59.000000 ligo.skymap-1.1.1/CHANGES.rst
+-rw-rw-rw-   0 root         (0) root         (0)      677 2023-07-06 20:38:49.000000 ligo.skymap-1.1.1/CONTRIBUTING.rst
+-rw-rw-rw-   0 root         (0) root         (0)      286 2023-07-06 20:38:49.000000 ligo.skymap-1.1.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     4239 2023-07-08 17:33:18.762179 ligo.skymap-1.1.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2777 2023-07-06 20:38:49.000000 ligo.skymap-1.1.1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-08 17:33:18.661176 ligo.skymap-1.1.1/cextern/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-08 17:33:18.669176 ligo.skymap-1.1.1/cextern/chealpix/
+-rw-rw-rw-   0 root         (0) root         (0)    30207 2023-07-06 20:38:49.000000 ligo.skymap-1.1.1/cextern/chealpix/chealpix.c
+-rw-rw-rw-   0 root         (0) root         (0)     7407 2023-07-06 20:38:49.000000 ligo.skymap-1.1.1/cextern/chealpix/chealpix.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-08 17:33:18.673176 ligo.skymap-1.1.1/docs/
+-rw-rw-rw-   0 root         (0) root         (0)     4581 2023-07-06 20:38:49.000000 ligo.skymap-1.1.1/docs/Makefile
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-08 17:33:18.677177 ligo.skymap-1.1.1/docs/_static/
+-rw-rw-rw-   0 root         (0) root         (0)    34751 2023-07-08 12:53:24.000000 ligo.skymap-1.1.1/docs/_static/benchmark.svg
+-rw-rw-rw-   0 root         (0) root         (0)   567737 2023-07-06 20:38:49.000000 ligo.skymap-1.1.1/docs/_static/coinc.xml
+-rw-rw-rw-   0 root         (0) root         (0)   260305 2023-07-06 20:38:49.000000 ligo.skymap-1.1.1/docs/_static/localization.svg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-08 17:33:18.661176 ligo.skymap-1.1.1/docs/_templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-08 17:33:18.680177 ligo.skymap-1.1.1/docs/_templates/autosummary/
+-rw-rw-rw-   0 root         (0) root         (0)      250 2023-07-06 20:38:49.000000 ligo.skymap-1.1.1/docs/_templates/autosummary/base.rst
+-rw-rw-rw-   0 root         (0) root         (0)      251 2023-07-06 20:38:49.000000 ligo.skymap-1.1.1/docs/_templates/autosummary/class.rst
+-rw-rw-rw-   0 root         (0) root         (0)      252 2023-07-06 20:38:49.000000 ligo.skymap-1.1.1/docs/_templates/autosummary/module.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-08 17:33:18.683177 ligo.skymap-1.1.1/docs/bayestar/
+-rw-rw-rw-   0 root         (0) root         (0)    56171 2023-07-06 20:38:49.000000 ligo.skymap-1.1.1/docs/bayestar/eggbox.png
+-rw-rw-rw-   0 root         (0) root         (0)      212 2023-07-06 20:38:49.000000 ligo.skymap-1.1.1/docs/bayestar/ez_emcee.rst
+-rw-rw-rw-   0 root         (0) root         (0)      182 2023-07-06 20:38:49.000000 ligo.skymap-1.1.1/docs/bayestar/filter.rst
+-rw-rw-rw-   0 root         (0) root         (0)      309 2023-07-06 20:38:49.000000 ligo.skymap-1.1.1/docs/bayestar/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)      225 2023-07-06 20:38:49.000000 ligo.skymap-1.1.1/docs/bayestar/interpolation.rst
+-rw-rw-rw-   0 root         (0) root         (0)    42428 2023-07-08 17:32:59.000000 ligo.skymap-1.1.1/docs/changes.rst
+-rw-rw-rw-   0 root         (0) root         (0)     8638 2023-07-06 20:38:49.000000 ligo.skymap-1.1.1/docs/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)      677 2023-07-06 20:38:49.000000 ligo.skymap-1.1.1/docs/contributing.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-08 17:33:18.683177 ligo.skymap-1.1.1/docs/coordinates/
+-rw-rw-rw-   0 root         (0) root         (0)      191 2023-07-06 20:38:49.000000 ligo.skymap-1.1.1/docs/coordinates/detector.rst
+-rw-rw-rw-   0 root         (0) root         (0)      189 2023-07-06 20:38:49.000000 ligo.skymap-1.1.1/docs/coordinates/eigenframe.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2304 2023-07-06 20:38:49.000000 ligo.skymap-1.1.1/docs/develop.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-08 17:33:18.683177 ligo.skymap-1.1.1/docs/distance/
+-rw-rw-rw-   0 root         (0) root         (0)     1243 2023-07-06 20:38:49.000000 ligo.skymap-1.1.1/docs/distance/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-08 17:33:18.684177 ligo.skymap-1.1.1/docs/healpix_tree/
+-rw-rw-rw-   0 root         (0) root         (0)      165 2023-07-06 20:38:49.000000 ligo.skymap-1.1.1/docs/healpix_tree/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)      595 2023-07-06 20:38:49.000000 ligo.skymap-1.1.1/docs/help.rst
+-rw-rw-rw-   0 root         (0) root         (0)     4574 2023-07-07 17:42:23.000000 ligo.skymap-1.1.1/docs/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)    15650 2023-07-06 20:38:49.000000 ligo.skymap-1.1.1/docs/interface.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-08 17:33:18.685177 ligo.skymap-1.1.1/docs/io/
+-rw-rw-rw-   0 root         (0) root         (0)     3691 2023-07-06 20:38:49.000000 ligo.skymap-1.1.1/docs/io/events.rst
+-rw-rw-rw-   0 root         (0) root         (0)      146 2023-07-06 20:38:49.000000 ligo.skymap-1.1.1/docs/io/fits.rst
+-rw-rw-rw-   0 root         (0) root         (0)      166 2023-07-06 20:38:49.000000 ligo.skymap-1.1.1/docs/io/hdf5.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-08 17:33:18.685177 ligo.skymap-1.1.1/docs/kde/
+-rw-rw-rw-   0 root         (0) root         (0)      162 2023-07-06 20:38:49.000000 ligo.skymap-1.1.1/docs/kde/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     4549 2023-07-06 20:38:49.000000 ligo.skymap-1.1.1/docs/make.bat
+-rw-rw-rw-   0 root         (0) root         (0)       13 2023-07-06 20:38:49.000000 ligo.skymap-1.1.1/docs/matplotlibrc
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-08 17:33:18.685177 ligo.skymap-1.1.1/docs/moc/
+-rw-rw-rw-   0 root         (0) root         (0)      267 2023-07-06 20:38:49.000000 ligo.skymap-1.1.1/docs/moc/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1282 2023-07-06 20:38:49.000000 ligo.skymap-1.1.1/docs/performance.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-08 17:33:18.688177 ligo.skymap-1.1.1/docs/plot/
+-rw-rw-rw-   0 root         (0) root         (0)      186 2023-07-06 20:38:49.000000 ligo.skymap-1.1.1/docs/plot/allsky.rst
+-rw-rw-rw-   0 root         (0) root         (0)      198 2023-07-06 20:38:49.000000 ligo.skymap-1.1.1/docs/plot/backdrop.rst
+-rw-rw-rw-   0 root         (0) root         (0)      206 2023-07-07 17:42:23.000000 ligo.skymap-1.1.1/docs/plot/bayes_factor.rst
+-rw-rw-rw-   0 root         (0) root         (0)      205 2023-07-06 20:38:49.000000 ligo.skymap-1.1.1/docs/plot/marker.rst
+-rw-rw-rw-   0 root         (0) root         (0)      166 2023-07-06 20:38:49.000000 ligo.skymap-1.1.1/docs/plot/poly.rst
+-rw-rw-rw-   0 root         (0) root         (0)      182 2023-07-06 20:38:49.000000 ligo.skymap-1.1.1/docs/plot/pp.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-08 17:33:18.689177 ligo.skymap-1.1.1/docs/postprocess/
+-rw-rw-rw-   0 root         (0) root         (0)      180 2023-07-06 20:38:49.000000 ligo.skymap-1.1.1/docs/postprocess/contour.rst
+-rw-rw-rw-   0 root         (0) root         (0)      184 2023-07-06 20:38:49.000000 ligo.skymap-1.1.1/docs/postprocess/cosmology.rst
+-rw-rw-rw-   0 root         (0) root         (0)      253 2023-07-06 20:38:49.000000 ligo.skymap-1.1.1/docs/postprocess/crossmatch.rst
+-rw-rw-rw-   0 root         (0) root         (0)      200 2023-07-06 20:38:49.000000 ligo.skymap-1.1.1/docs/postprocess/ellipse.rst
+-rw-rw-rw-   0 root         (0) root         (0)      195 2023-07-06 20:38:49.000000 ligo.skymap-1.1.1/docs/postprocess/util.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-08 17:33:18.690177 ligo.skymap-1.1.1/docs/quickstart/
+-rw-rw-rw-   0 root         (0) root         (0)     6351 2023-07-06 20:38:49.000000 ligo.skymap-1.1.1/docs/quickstart/bayestar-injections.rst
+-rw-rw-rw-   0 root         (0) root         (0)     4156 2023-07-06 20:38:49.000000 ligo.skymap-1.1.1/docs/quickstart/install.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1595 2023-07-06 20:38:49.000000 ligo.skymap-1.1.1/docs/testing.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-08 17:33:18.697177 ligo.skymap-1.1.1/docs/tool/
+-rw-rw-rw-   0 root         (0) root         (0)      314 2023-07-06 20:38:49.000000 ligo.skymap-1.1.1/docs/tool/bayestar_inject.rst
+-rw-rw-rw-   0 root         (0) root         (0)      188 2023-07-06 20:38:49.000000 ligo.skymap-1.1.1/docs/tool/bayestar_localize_coincs.rst
+-rw-rw-rw-   0 root         (0) root         (0)      204 2023-07-06 20:38:49.000000 ligo.skymap-1.1.1/docs/tool/bayestar_localize_lvalert.rst
+-rw-rw-rw-   0 root         (0) root         (0)      189 2023-07-06 20:38:49.000000 ligo.skymap-1.1.1/docs/tool/bayestar_mcmc.rst
+-rw-rw-rw-   0 root         (0) root         (0)      179 2023-07-06 20:38:49.000000 ligo.skymap-1.1.1/docs/tool/bayestar_realize_coincs.rst
+-rw-rw-rw-   0 root         (0) root         (0)      175 2023-07-06 20:38:49.000000 ligo.skymap-1.1.1/docs/tool/bayestar_sample_model_psd.rst
+-rw-rw-rw-   0 root         (0) root         (0)      175 2023-07-06 20:38:49.000000 ligo.skymap-1.1.1/docs/tool/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1400 2023-07-06 20:38:49.000000 ligo.skymap-1.1.1/docs/tool/ligo_skymap_combine.rst
+-rw-rw-rw-   0 root         (0) root         (0)     3709 2023-07-06 20:38:49.000000 ligo.skymap-1.1.1/docs/tool/ligo_skymap_constellations.rst
+-rw-rw-rw-   0 root         (0) root         (0)      165 2023-07-06 20:38:49.000000 ligo.skymap-1.1.1/docs/tool/ligo_skymap_contour.rst
+-rw-rw-rw-   0 root         (0) root         (0)      215 2023-07-06 20:38:49.000000 ligo.skymap-1.1.1/docs/tool/ligo_skymap_contour_moc.rst
+-rw-rw-rw-   0 root         (0) root         (0)      199 2023-07-06 20:38:49.000000 ligo.skymap-1.1.1/docs/tool/ligo_skymap_flatten.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1387 2023-07-06 20:38:49.000000 ligo.skymap-1.1.1/docs/tool/ligo_skymap_from_samples.rst
+-rw-rw-rw-   0 root         (0) root         (0)      747 2023-07-06 20:38:49.000000 ligo.skymap-1.1.1/docs/tool/ligo_skymap_plot.rst
+-rw-rw-rw-   0 root         (0) root         (0)      795 2023-07-06 20:38:49.000000 ligo.skymap-1.1.1/docs/tool/ligo_skymap_plot_airmass.rst
+-rw-rw-rw-   0 root         (0) root         (0)      779 2023-07-07 17:42:23.000000 ligo.skymap-1.1.1/docs/tool/ligo_skymap_plot_coherence.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1121 2023-07-06 20:38:49.000000 ligo.skymap-1.1.1/docs/tool/ligo_skymap_plot_observability.rst
+-rw-rw-rw-   0 root         (0) root         (0)      188 2023-07-06 20:38:49.000000 ligo.skymap-1.1.1/docs/tool/ligo_skymap_plot_stats.rst
+-rw-rw-rw-   0 root         (0) root         (0)      700 2023-07-06 20:38:49.000000 ligo.skymap-1.1.1/docs/tool/ligo_skymap_plot_volume.rst
+-rw-rw-rw-   0 root         (0) root         (0)      177 2023-07-06 20:38:49.000000 ligo.skymap-1.1.1/docs/tool/ligo_skymap_stats.rst
+-rw-rw-rw-   0 root         (0) root         (0)      209 2023-07-06 20:38:49.000000 ligo.skymap-1.1.1/docs/tool/ligo_skymap_unflatten.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-08 17:33:18.698177 ligo.skymap-1.1.1/docs/util/
+-rw-rw-rw-   0 root         (0) root         (0)      158 2023-07-06 20:38:49.000000 ligo.skymap-1.1.1/docs/util/file.rst
+-rw-rw-rw-   0 root         (0) root         (0)      172 2023-07-06 20:38:49.000000 ligo.skymap-1.1.1/docs/util/ilwd.rst
+-rw-rw-rw-   0 root         (0) root         (0)      163 2023-07-06 20:38:49.000000 ligo.skymap-1.1.1/docs/util/numpy.rst
+-rw-rw-rw-   0 root         (0) root         (0)      168 2023-07-06 20:38:49.000000 ligo.skymap-1.1.1/docs/util/sqlite.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-08 17:33:18.700177 ligo.skymap-1.1.1/licenses/
+-rw-rw-rw-   0 root         (0) root         (0)     6360 2023-07-06 20:38:49.000000 ligo.skymap-1.1.1/licenses/CHEALPIX_LICENSE.rst
+-rw-rw-rw-   0 root         (0) root         (0)    37565 2023-07-06 20:38:49.000000 ligo.skymap-1.1.1/licenses/LICENSE.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1792 2023-07-06 20:38:49.000000 ligo.skymap-1.1.1/licenses/NUMPY_LICENSE.rst
+-rw-rw-rw-   0 root         (0) root         (0)      372 2023-07-06 20:38:49.000000 ligo.skymap-1.1.1/licenses/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1659 2023-07-06 20:38:49.000000 ligo.skymap-1.1.1/licenses/TEMPLATE_LICENCE.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-08 17:33:18.663176 ligo.skymap-1.1.1/ligo/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-08 17:33:18.704177 ligo.skymap-1.1.1/ligo/skymap/
+-rw-rw-rw-   0 root         (0) root         (0)     1012 2023-07-06 20:38:49.000000 ligo.skymap-1.1.1/ligo/skymap/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      698 2023-07-06 20:38:49.000000 ligo.skymap-1.1.1/ligo/skymap/_astropy_init.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-08 17:33:18.706178 ligo.skymap-1.1.1/ligo/skymap/bayestar/
+-rw-rw-rw-   0 root         (0) root         (0)    20852 2023-07-06 20:38:49.000000 ligo.skymap-1.1.1/ligo/skymap/bayestar/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5864 2023-07-06 20:38:49.000000 ligo.skymap-1.1.1/ligo/skymap/bayestar/ez_emcee.py
+-rw-rw-rw-   0 root         (0) root         (0)    19685 2023-07-06 20:38:49.000000 ligo.skymap-1.1.1/ligo/skymap/bayestar/filter.py
+-rw-rw-rw-   0 root         (0) root         (0)    10348 2023-07-06 20:38:49.000000 ligo.skymap-1.1.1/ligo/skymap/bayestar/interpolation.py
+-rw-rw-rw-   0 root         (0) root         (0)     2176 2023-07-06 20:38:49.000000 ligo.skymap-1.1.1/ligo/skymap/bayestar/ptemcee.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-08 17:33:18.707177 ligo.skymap-1.1.1/ligo/skymap/bayestar/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-08 17:32:59.000000 ligo.skymap-1.1.1/ligo/skymap/bayestar/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1545 2023-07-06 20:38:49.000000 ligo.skymap-1.1.1/ligo/skymap/bayestar/tests/test_bayestar.py
+-rw-rw-rw-   0 root         (0) root         (0)     4573 2023-07-06 20:38:49.000000 ligo.skymap-1.1.1/ligo/skymap/bayestar/tests/test_interpolation.py
+-rw-rw-rw-   0 root         (0) root         (0)     4287 2023-07-06 20:38:49.000000 ligo.skymap-1.1.1/ligo/skymap/bayestar/tests/test_signal_amplitude_model.py
+-rw-rw-rw-   0 root         (0) root         (0)     2321 2023-07-06 20:38:49.000000 ligo.skymap-1.1.1/ligo/skymap/conftest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-08 17:33:18.708178 ligo.skymap-1.1.1/ligo/skymap/coordinates/
+-rw-rw-rw-   0 root         (0) root         (0)      382 2023-07-06 20:38:49.000000 ligo.skymap-1.1.1/ligo/skymap/coordinates/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3645 2023-07-06 20:38:49.000000 ligo.skymap-1.1.1/ligo/skymap/coordinates/detector.py
+-rw-rw-rw-   0 root         (0) root         (0)     4132 2023-07-06 20:38:49.000000 ligo.skymap-1.1.1/ligo/skymap/coordinates/eigenframe.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-08 17:33:18.708178 ligo.skymap-1.1.1/ligo/skymap/coordinates/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-08 17:32:59.000000 ligo.skymap-1.1.1/ligo/skymap/coordinates/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      996 2023-07-06 20:38:49.000000 ligo.skymap-1.1.1/ligo/skymap/coordinates/tests/test_detector.py
+-rw-rw-rw-   0 root         (0) root         (0)    20879 2023-07-06 20:38:49.000000 ligo.skymap-1.1.1/ligo/skymap/distance.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-08 17:33:18.709178 ligo.skymap-1.1.1/ligo/skymap/extern/
+-rw-rw-rw-   0 root         (0) root         (0)      460 2023-07-06 20:38:49.000000 ligo.skymap-1.1.1/ligo/skymap/extern/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-08 17:33:18.709178 ligo.skymap-1.1.1/ligo/skymap/extern/numpy/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-08 17:32:59.000000 ligo.skymap-1.1.1/ligo/skymap/extern/numpy/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    13938 2023-07-06 20:38:49.000000 ligo.skymap-1.1.1/ligo/skymap/extern/numpy/quantile.py
+-rw-rw-rw-   0 root         (0) root         (0)    15264 2023-07-06 20:38:49.000000 ligo.skymap-1.1.1/ligo/skymap/healpix_tree.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-08 17:33:18.710178 ligo.skymap-1.1.1/ligo/skymap/io/
+-rw-rw-rw-   0 root         (0) root         (0)      382 2023-07-06 20:38:49.000000 ligo.skymap-1.1.1/ligo/skymap/io/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-08 17:33:18.712178 ligo.skymap-1.1.1/ligo/skymap/io/events/
+-rw-rw-rw-   0 root         (0) root         (0)      382 2023-07-06 20:38:49.000000 ligo.skymap-1.1.1/ligo/skymap/io/events/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3832 2023-07-06 20:38:49.000000 ligo.skymap-1.1.1/ligo/skymap/io/events/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     2664 2023-07-06 20:38:49.000000 ligo.skymap-1.1.1/ligo/skymap/io/events/detector_disabled.py
+-rw-rw-rw-   0 root         (0) root         (0)     2274 2023-07-06 20:38:49.000000 ligo.skymap-1.1.1/ligo/skymap/io/events/gracedb.py
+-rw-rw-rw-   0 root         (0) root         (0)     7809 2023-07-06 20:38:49.000000 ligo.skymap-1.1.1/ligo/skymap/io/events/hdf.py
+-rw-rw-rw-   0 root         (0) root         (0)    11345 2023-07-06 20:38:49.000000 ligo.skymap-1.1.1/ligo/skymap/io/events/ligolw.py
+-rw-rw-rw-   0 root         (0) root         (0)     2563 2023-07-06 20:38:49.000000 ligo.skymap-1.1.1/ligo/skymap/io/events/magic.py
+-rw-rw-rw-   0 root         (0) root         (0)     1700 2023-07-06 20:38:49.000000 ligo.skymap-1.1.1/ligo/skymap/io/events/sqlite.py
+-rwxrwxrwx   0 root         (0) root         (0)    19227 2023-07-06 20:38:49.000000 ligo.skymap-1.1.1/ligo/skymap/io/fits.py
+-rwxrwxrwx   0 root         (0) root         (0)    10598 2023-07-06 20:38:49.000000 ligo.skymap-1.1.1/ligo/skymap/io/hdf5.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-08 17:33:18.712178 ligo.skymap-1.1.1/ligo/skymap/io/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-08 17:32:59.000000 ligo.skymap-1.1.1/ligo/skymap/io/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-08 17:33:18.717178 ligo.skymap-1.1.1/ligo/skymap/io/tests/data/
+-rw-rw-rw-   0 root         (0) root         (0)   492938 2023-07-06 20:38:49.000000 ligo.skymap-1.1.1/ligo/skymap/io/tests/data/2016_subset.xml.gz
+-rw-rw-rw-   0 root         (0) root         (0)     1699 2023-07-06 20:38:49.000000 ligo.skymap-1.1.1/ligo/skymap/io/tests/data/G197392_coinc.xml.gz
+-rw-rw-rw-   0 root         (0) root         (0)      675 2023-07-06 20:38:49.000000 ligo.skymap-1.1.1/ligo/skymap/io/tests/data/G197392_psd.xml.gz
+-rw-rw-rw-   0 root         (0) root         (0)     2470 2023-07-06 20:38:49.000000 ligo.skymap-1.1.1/ligo/skymap/io/tests/data/G211117_coinc.xml.gz
+-rw-rw-rw-   0 root         (0) root         (0)     2355 2023-07-06 20:38:49.000000 ligo.skymap-1.1.1/ligo/skymap/io/tests/data/G211117_psd.xml.gz
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-08 17:32:59.000000 ligo.skymap-1.1.1/ligo/skymap/io/tests/data/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-08 17:33:18.718178 ligo.skymap-1.1.1/ligo/skymap/io/tests/data/gstlal_reference_psd/
+-rw-rw-rw-   0 root         (0) root         (0)      717 2023-07-06 20:38:49.000000 ligo.skymap-1.1.1/ligo/skymap/io/tests/data/gstlal_reference_psd/H1L1V1-REFERENCE_PSD-967234210-29963.xml.gz
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-08 17:32:59.000000 ligo.skymap-1.1.1/ligo/skymap/io/tests/data/gstlal_reference_psd/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9120 2023-07-06 20:38:49.000000 ligo.skymap-1.1.1/ligo/skymap/io/tests/data/test.hdf5
+-rw-rw-rw-   0 root         (0) root         (0)    12598 2023-07-06 20:38:49.000000 ligo.skymap-1.1.1/ligo/skymap/io/tests/test_io_events.py
+-rw-rw-rw-   0 root         (0) root         (0)    17043 2023-07-06 20:38:49.000000 ligo.skymap-1.1.1/ligo/skymap/kde.py
+-rw-rw-rw-   0 root         (0) root         (0)     7533 2023-07-07 17:20:00.000000 ligo.skymap-1.1.1/ligo/skymap/moc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-08 17:33:18.723178 ligo.skymap-1.1.1/ligo/skymap/plot/
+-rw-rw-rw-   0 root         (0) root         (0)      382 2023-07-06 20:38:49.000000 ligo.skymap-1.1.1/ligo/skymap/plot/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    29184 2023-07-06 20:38:49.000000 ligo.skymap-1.1.1/ligo/skymap/plot/allsky.py
+-rw-rw-rw-   0 root         (0) root         (0)     1415 2023-07-06 20:38:49.000000 ligo.skymap-1.1.1/ligo/skymap/plot/angle.py
+-rw-rw-rw-   0 root         (0) root         (0)     7291 2023-07-06 20:38:49.000000 ligo.skymap-1.1.1/ligo/skymap/plot/backdrop.py
+-rw-rw-rw-   0 root         (0) root         (0)     3910 2023-07-07 17:42:23.000000 ligo.skymap-1.1.1/ligo/skymap/plot/bayes_factor.py
+-rw-rw-rw-   0 root         (0) root         (0)     1522 2023-07-06 20:38:49.000000 ligo.skymap-1.1.1/ligo/skymap/plot/cmap.py
+-rw-rw-rw-   0 root         (0) root         (0)     8714 2023-07-06 20:38:49.000000 ligo.skymap-1.1.1/ligo/skymap/plot/cylon.csv
+-rw-rw-rw-   0 root         (0) root         (0)     2125 2023-07-06 20:38:49.000000 ligo.skymap-1.1.1/ligo/skymap/plot/cylon.py
+-rw-rw-rw-   0 root         (0) root         (0)     2933 2023-07-06 20:38:49.000000 ligo.skymap-1.1.1/ligo/skymap/plot/marker.py
+-rw-rw-rw-   0 root         (0) root         (0)    63275 2023-07-06 20:38:49.000000 ligo.skymap-1.1.1/ligo/skymap/plot/ne_simplified_coastline.json
+-rw-rw-rw-   0 root         (0) root         (0)     7394 2023-07-06 20:38:49.000000 ligo.skymap-1.1.1/ligo/skymap/plot/poly.py
+-rw-rw-rw-   0 root         (0) root         (0)     9445 2023-07-06 20:38:49.000000 ligo.skymap-1.1.1/ligo/skymap/plot/pp.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-08 17:33:18.723178 ligo.skymap-1.1.1/ligo/skymap/plot/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-08 17:32:59.000000 ligo.skymap-1.1.1/ligo/skymap/plot/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-08 17:33:18.738179 ligo.skymap-1.1.1/ligo/skymap/plot/tests/baseline/
+-rw-rw-rw-   0 root         (0) root         (0)    67690 2023-07-06 20:38:49.000000 ligo.skymap-1.1.1/ligo/skymap/plot/tests/baseline/test_allsky_axes_astro-degrees-aitoff.png
+-rw-rw-rw-   0 root         (0) root         (0)    65830 2023-07-06 20:38:49.000000 ligo.skymap-1.1.1/ligo/skymap/plot/tests/baseline/test_allsky_axes_astro-degrees-mollweide.png
+-rw-rw-rw-   0 root         (0) root         (0)    65829 2023-07-06 20:38:49.000000 ligo.skymap-1.1.1/ligo/skymap/plot/tests/baseline/test_allsky_axes_astro-hours-aitoff.png
+-rw-rw-rw-   0 root         (0) root         (0)    63879 2023-07-06 20:38:49.000000 ligo.skymap-1.1.1/ligo/skymap/plot/tests/baseline/test_allsky_axes_astro-hours-mollweide.png
+-rw-rw-rw-   0 root         (0) root         (0)    71762 2023-07-06 20:38:49.000000 ligo.skymap-1.1.1/ligo/skymap/plot/tests/baseline/test_allsky_axes_galactic-degrees-aitoff.png
+-rw-rw-rw-   0 root         (0) root         (0)    71509 2023-07-06 20:38:49.000000 ligo.skymap-1.1.1/ligo/skymap/plot/tests/baseline/test_allsky_axes_galactic-degrees-mollweide.png
+-rw-rw-rw-   0 root         (0) root         (0)    70497 2023-07-06 20:38:49.000000 ligo.skymap-1.1.1/ligo/skymap/plot/tests/baseline/test_allsky_axes_galactic-hours-aitoff.png
+-rw-rw-rw-   0 root         (0) root         (0)    69334 2023-07-06 20:38:49.000000 ligo.skymap-1.1.1/ligo/skymap/plot/tests/baseline/test_allsky_axes_galactic-hours-mollweide.png
+-rw-rw-rw-   0 root         (0) root         (0)    64896 2023-07-06 20:38:49.000000 ligo.skymap-1.1.1/ligo/skymap/plot/tests/baseline/test_allsky_axes_geo-degrees-aitoff.png
+-rw-rw-rw-   0 root         (0) root         (0)    63732 2023-07-06 20:38:49.000000 ligo.skymap-1.1.1/ligo/skymap/plot/tests/baseline/test_allsky_axes_geo-degrees-mollweide.png
+-rw-rw-rw-   0 root         (0) root         (0)    63470 2023-07-06 20:38:49.000000 ligo.skymap-1.1.1/ligo/skymap/plot/tests/baseline/test_allsky_axes_geo-hours-aitoff.png
+-rw-rw-rw-   0 root         (0) root         (0)    61561 2023-07-06 20:38:49.000000 ligo.skymap-1.1.1/ligo/skymap/plot/tests/baseline/test_allsky_axes_geo-hours-mollweide.png
+-rw-rw-rw-   0 root         (0) root         (0)    33964 2023-07-06 20:38:49.000000 ligo.skymap-1.1.1/ligo/skymap/plot/tests/baseline/test_allsky_obstime.png
+-rw-rw-rw-   0 root         (0) root         (0)    20330 2023-07-06 20:38:49.000000 ligo.skymap-1.1.1/ligo/skymap/plot/tests/baseline/test_globe_axes.png
+-rw-rw-rw-   0 root         (0) root         (0)    19092 2023-07-06 20:38:49.000000 ligo.skymap-1.1.1/ligo/skymap/plot/tests/baseline/test_pp_plot_default.png
+-rw-rw-rw-   0 root         (0) root         (0)    39991 2023-07-06 20:38:49.000000 ligo.skymap-1.1.1/ligo/skymap/plot/tests/baseline/test_pp_plot_lines.png
+-rw-rw-rw-   0 root         (0) root         (0)    19092 2023-07-06 20:38:49.000000 ligo.skymap-1.1.1/ligo/skymap/plot/tests/baseline/test_pp_plot_steps.png
+-rw-rw-rw-   0 root         (0) root         (0)     8866 2023-07-06 20:38:49.000000 ligo.skymap-1.1.1/ligo/skymap/plot/tests/baseline/test_reticle.png
+-rw-rw-rw-   0 root         (0) root         (0)    19815 2023-07-06 20:38:49.000000 ligo.skymap-1.1.1/ligo/skymap/plot/tests/baseline/test_zoom_axes.png
+-rw-rw-rw-   0 root         (0) root         (0)     5202 2023-07-06 20:38:49.000000 ligo.skymap-1.1.1/ligo/skymap/plot/tests/test_plot.py
+-rw-rw-rw-   0 root         (0) root         (0)     2400 2023-07-06 20:38:49.000000 ligo.skymap-1.1.1/ligo/skymap/plot/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-08 17:33:18.740179 ligo.skymap-1.1.1/ligo/skymap/postprocess/
+-rw-rw-rw-   0 root         (0) root         (0)      382 2023-07-06 20:38:49.000000 ligo.skymap-1.1.1/ligo/skymap/postprocess/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6348 2023-07-06 20:38:49.000000 ligo.skymap-1.1.1/ligo/skymap/postprocess/contour.py
+-rw-rw-rw-   0 root         (0) root         (0)     2407 2023-07-06 20:38:49.000000 ligo.skymap-1.1.1/ligo/skymap/postprocess/cosmology.py
+-rw-rw-rw-   0 root         (0) root         (0)    18664 2023-07-06 20:38:49.000000 ligo.skymap-1.1.1/ligo/skymap/postprocess/crossmatch.py
+-rw-rw-rw-   0 root         (0) root         (0)    15257 2023-07-06 20:38:49.000000 ligo.skymap-1.1.1/ligo/skymap/postprocess/ellipse.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-08 17:33:18.740179 ligo.skymap-1.1.1/ligo/skymap/postprocess/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-08 17:32:59.000000 ligo.skymap-1.1.1/ligo/skymap/postprocess/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      899 2023-07-06 20:38:49.000000 ligo.skymap-1.1.1/ligo/skymap/postprocess/tests/test_cosmology.py
+-rw-rw-rw-   0 root         (0) root         (0)     4373 2023-07-06 20:38:49.000000 ligo.skymap-1.1.1/ligo/skymap/postprocess/tests/test_crossmatch.py
+-rw-rw-rw-   0 root         (0) root         (0)     3219 2023-07-06 20:38:49.000000 ligo.skymap-1.1.1/ligo/skymap/postprocess/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-08 17:33:18.741179 ligo.skymap-1.1.1/ligo/skymap/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-08 17:32:59.000000 ligo.skymap-1.1.1/ligo/skymap/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-08 17:33:18.741179 ligo.skymap-1.1.1/ligo/skymap/tests/plugins/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-08 17:32:59.000000 ligo.skymap-1.1.1/ligo/skymap/tests/plugins/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      578 2023-07-06 20:38:49.000000 ligo.skymap-1.1.1/ligo/skymap/tests/plugins/omp.py
+-rw-rw-rw-   0 root         (0) root         (0)     4831 2023-07-06 20:38:49.000000 ligo.skymap-1.1.1/ligo/skymap/tests/test_moc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-08 17:33:18.751179 ligo.skymap-1.1.1/ligo/skymap/tool/
+-rw-rw-rw-   0 root         (0) root         (0)    15669 2023-07-07 17:20:00.000000 ligo.skymap-1.1.1/ligo/skymap/tool/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    21608 2023-07-07 17:20:00.000000 ligo.skymap-1.1.1/ligo/skymap/tool/bayestar_inject.py
+-rw-rw-rw-   0 root         (0) root         (0)     7538 2023-07-07 17:20:00.000000 ligo.skymap-1.1.1/ligo/skymap/tool/bayestar_localize_coincs.py
+-rwxrwxrwx   0 root         (0) root         (0)     6821 2023-07-07 17:20:00.000000 ligo.skymap-1.1.1/ligo/skymap/tool/bayestar_localize_lvalert.py
+-rw-rw-rw-   0 root         (0) root         (0)     8137 2023-07-07 17:20:00.000000 ligo.skymap-1.1.1/ligo/skymap/tool/bayestar_mcmc.py
+-rw-rw-rw-   0 root         (0) root         (0)    18761 2023-07-07 17:20:00.000000 ligo.skymap-1.1.1/ligo/skymap/tool/bayestar_realize_coincs.py
+-rw-rw-rw-   0 root         (0) root         (0)     4600 2023-07-06 20:38:49.000000 ligo.skymap-1.1.1/ligo/skymap/tool/bayestar_sample_model_psd.py
+-rw-rw-rw-   0 root         (0) root         (0)     5841 2023-07-06 20:38:49.000000 ligo.skymap-1.1.1/ligo/skymap/tool/ligo_skymap_combine.py
+-rw-rw-rw-   0 root         (0) root         (0)     2011 2023-07-06 20:38:49.000000 ligo.skymap-1.1.1/ligo/skymap/tool/ligo_skymap_constellations.py
+-rw-rw-rw-   0 root         (0) root         (0)     3341 2023-07-06 20:38:49.000000 ligo.skymap-1.1.1/ligo/skymap/tool/ligo_skymap_contour.py
+-rw-rw-rw-   0 root         (0) root         (0)     2519 2023-07-06 20:38:49.000000 ligo.skymap-1.1.1/ligo/skymap/tool/ligo_skymap_contour_moc.py
+-rw-rw-rw-   0 root         (0) root         (0)     2288 2023-07-06 20:38:49.000000 ligo.skymap-1.1.1/ligo/skymap/tool/ligo_skymap_flatten.py
+-rw-rw-rw-   0 root         (0) root         (0)     7662 2023-07-07 17:20:00.000000 ligo.skymap-1.1.1/ligo/skymap/tool/ligo_skymap_from_samples.py
+-rw-rw-rw-   0 root         (0) root         (0)     6732 2023-07-07 17:20:00.000000 ligo.skymap-1.1.1/ligo/skymap/tool/ligo_skymap_plot.py
+-rw-rw-rw-   0 root         (0) root         (0)     8353 2023-07-07 17:20:00.000000 ligo.skymap-1.1.1/ligo/skymap/tool/ligo_skymap_plot_airmass.py
+-rw-rw-rw-   0 root         (0) root         (0)     1713 2023-07-07 17:42:23.000000 ligo.skymap-1.1.1/ligo/skymap/tool/ligo_skymap_plot_coherence.py
+-rw-rw-rw-   0 root         (0) root         (0)     5711 2023-07-07 17:20:00.000000 ligo.skymap-1.1.1/ligo/skymap/tool/ligo_skymap_plot_observability.py
+-rw-rw-rw-   0 root         (0) root         (0)     5158 2023-07-07 17:20:00.000000 ligo.skymap-1.1.1/ligo/skymap/tool/ligo_skymap_plot_pp_samples.py
+-rw-rw-rw-   0 root         (0) root         (0)     8048 2023-07-06 20:38:49.000000 ligo.skymap-1.1.1/ligo/skymap/tool/ligo_skymap_plot_stats.py
+-rwxrwxrwx   0 root         (0) root         (0)     9404 2023-07-07 17:20:00.000000 ligo.skymap-1.1.1/ligo/skymap/tool/ligo_skymap_plot_volume.py
+-rw-rw-rw-   0 root         (0) root         (0)    11830 2023-07-06 20:38:49.000000 ligo.skymap-1.1.1/ligo/skymap/tool/ligo_skymap_stats.py
+-rw-rw-rw-   0 root         (0) root         (0)     1739 2023-07-06 20:38:49.000000 ligo.skymap-1.1.1/ligo/skymap/tool/ligo_skymap_unflatten.py
+-rw-rw-rw-   0 root         (0) root         (0)     4508 2023-07-07 17:20:00.000000 ligo.skymap-1.1.1/ligo/skymap/tool/matplotlib.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-08 17:33:18.754179 ligo.skymap-1.1.1/ligo/skymap/tool/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     3064 2023-07-06 20:38:49.000000 ligo.skymap-1.1.1/ligo/skymap/tool/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5271 2023-07-06 20:38:49.000000 ligo.skymap-1.1.1/ligo/skymap/tool/tests/test_bayestar.py
+-rw-rw-rw-   0 root         (0) root         (0)     4494 2023-07-06 20:38:49.000000 ligo.skymap-1.1.1/ligo/skymap/tool/tests/test_bayestar_inject.py
+-rw-rw-rw-   0 root         (0) root         (0)     2400 2023-07-06 20:38:49.000000 ligo.skymap-1.1.1/ligo/skymap/tool/tests/test_combine.py
+-rw-rw-rw-   0 root         (0) root         (0)     4015 2023-07-06 20:38:49.000000 ligo.skymap-1.1.1/ligo/skymap/tool/tests/test_flatten.py
+-rw-rw-rw-   0 root         (0) root         (0)     2631 2023-07-06 20:38:49.000000 ligo.skymap-1.1.1/ligo/skymap/tool/tests/test_from_samples.py
+-rw-rw-rw-   0 root         (0) root         (0)      529 2023-07-06 20:38:49.000000 ligo.skymap-1.1.1/ligo/skymap/tool/tests/test_help.py
+-rw-rw-rw-   0 root         (0) root         (0)     1826 2023-07-06 20:38:49.000000 ligo.skymap-1.1.1/ligo/skymap/tool/tests/test_plot.py
+-rw-rw-rw-   0 root         (0) root         (0)     2065 2023-07-06 20:38:49.000000 ligo.skymap-1.1.1/ligo/skymap/tool/tests/test_plot_stats.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-08 17:33:18.756179 ligo.skymap-1.1.1/ligo/skymap/util/
+-rw-rw-rw-   0 root         (0) root         (0)      382 2023-07-06 20:38:49.000000 ligo.skymap-1.1.1/ligo/skymap/util/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1794 2023-07-06 20:38:49.000000 ligo.skymap-1.1.1/ligo/skymap/util/file.py
+-rw-rw-rw-   0 root         (0) root         (0)     5163 2023-07-06 20:38:49.000000 ligo.skymap-1.1.1/ligo/skymap/util/ilwd.py
+-rw-rw-rw-   0 root         (0) root         (0)     1680 2023-07-06 20:38:49.000000 ligo.skymap-1.1.1/ligo/skymap/util/numpy.py
+-rw-rw-rw-   0 root         (0) root         (0)     2854 2023-07-06 20:38:49.000000 ligo.skymap-1.1.1/ligo/skymap/util/progress.py
+-rw-rw-rw-   0 root         (0) root         (0)     4451 2023-07-06 20:38:49.000000 ligo.skymap-1.1.1/ligo/skymap/util/sqlite.py
+-rw-rw-rw-   0 root         (0) root         (0)     2694 2023-07-06 20:38:49.000000 ligo.skymap-1.1.1/ligo/skymap/util/stopwatch.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-08 17:33:18.757179 ligo.skymap-1.1.1/ligo/skymap/util/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-08 17:32:59.000000 ligo.skymap-1.1.1/ligo/skymap/util/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      363 2023-07-06 20:38:49.000000 ligo.skymap-1.1.1/ligo/skymap/util/tests/test_progress.py
+-rw-r--r--   0 root         (0) root         (0)      337 2023-07-08 17:33:18.000000 ligo.skymap-1.1.1/ligo/skymap/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-08 17:33:18.701177 ligo.skymap-1.1.1/ligo.skymap.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4239 2023-07-08 17:33:18.000000 ligo.skymap-1.1.1/ligo.skymap.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     8311 2023-07-08 17:33:18.000000 ligo.skymap-1.1.1/ligo.skymap.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-08 17:33:18.000000 ligo.skymap-1.1.1/ligo.skymap.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)     1550 2023-07-08 17:33:18.000000 ligo.skymap-1.1.1/ligo.skymap.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-08 17:33:18.000000 ligo.skymap-1.1.1/ligo.skymap.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      432 2023-07-08 17:33:18.000000 ligo.skymap-1.1.1/ligo.skymap.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2023-07-08 17:33:18.000000 ligo.skymap-1.1.1/ligo.skymap.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      355 2023-07-06 20:38:49.000000 ligo.skymap-1.1.1/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)     6430 2023-07-08 17:33:18.763179 ligo.skymap-1.1.1/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     3574 2023-07-06 20:38:49.000000 ligo.skymap-1.1.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-08 17:33:18.761179 ligo.skymap-1.1.1/src/
+-rw-rw-rw-   0 root         (0) root         (0)    37062 2023-07-06 20:38:49.000000 ligo.skymap-1.1.1/src/bayestar_cosmology.h
+-rw-rw-rw-   0 root         (0) root         (0)     4078 2023-07-06 20:38:49.000000 ligo.skymap-1.1.1/src/bayestar_cosmology.py
+-rw-rw-rw-   0 root         (0) root         (0)    15859 2023-07-06 20:38:49.000000 ligo.skymap-1.1.1/src/bayestar_distance.c
+-rw-rw-rw-   0 root         (0) root         (0)     2067 2023-07-06 20:38:49.000000 ligo.skymap-1.1.1/src/bayestar_distance.h
+-rw-rw-rw-   0 root         (0) root         (0)     4025 2023-07-06 20:38:49.000000 ligo.skymap-1.1.1/src/bayestar_moc.c
+-rw-rw-rw-   0 root         (0) root         (0)     1492 2023-07-06 20:38:49.000000 ligo.skymap-1.1.1/src/bayestar_moc.h
+-rw-rw-rw-   0 root         (0) root         (0)    53672 2023-07-06 20:38:49.000000 ligo.skymap-1.1.1/src/bayestar_sky_map.c
+-rw-rw-rw-   0 root         (0) root         (0)     7887 2023-07-06 20:38:49.000000 ligo.skymap-1.1.1/src/bayestar_sky_map.h
+-rw-rw-rw-   0 root         (0) root         (0)      218 2023-07-06 20:38:49.000000 ligo.skymap-1.1.1/src/branch_prediction.h
+-rw-rw-rw-   0 root         (0) root         (0)    39503 2023-07-06 20:38:49.000000 ligo.skymap-1.1.1/src/core.c
+-rw-rw-rw-   0 root         (0) root         (0)     5818 2023-07-06 20:38:49.000000 ligo.skymap-1.1.1/src/cubic_interp.c
+-rw-rw-rw-   0 root         (0) root         (0)     2069 2023-07-06 20:38:49.000000 ligo.skymap-1.1.1/src/cubic_interp.h
+-rw-rw-rw-   0 root         (0) root         (0)    13016 2023-07-06 20:38:49.000000 ligo.skymap-1.1.1/src/cubic_interp_test.c
+-rw-rw-rw-   0 root         (0) root         (0)     6370 2023-07-06 20:38:49.000000 ligo.skymap-1.1.1/src/omp_interruptible.h
+-rw-rw-rw-   0 root         (0) root         (0)     2377 2023-07-06 20:38:49.000000 ligo.skymap-1.1.1/src/vmath.h
+-rw-rw-rw-   0 root         (0) root         (0)     1869 2023-07-06 20:38:49.000000 ligo.skymap-1.1.1/src/warnings.h
+-rw-rw-rw-   0 root         (0) root         (0)     2595 2023-07-06 20:38:49.000000 ligo.skymap-1.1.1/tox.ini
```

### Comparing `ligo.skymap-1.1.0/.gitignore` & `ligo.skymap-1.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.1.0/.gitlab/combine-coverage.py` & `ligo.skymap-1.1.1/.gitlab/combine-coverage.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.1.0/.gitlab-ci.yml` & `ligo.skymap-1.1.1/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.1.0/CHANGES.rst` & `ligo.skymap-1.1.1/CHANGES.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,18 @@
 #########
 Changelog
 #########
 
+1.1.1 (2023-07-08)
+==================
+
+- Fix a typo in the ``setup.cfg`` file that prevented correct interpretation of
+  the minimum Python version. Contributed by
+  `@ahnitz <https://github.com/ahnitz>`_.
+
 1.1.0 (2023-07-07)
 ==================
 
 - Add ``max_depth`` keyword argument to the call to
   ``MOC.from_valued_healpix_cells`` in ``ligo-skymap-contour-moc``.
   Contributed by `@parkma99 <https://github.com/parkma99>`_.
```

### Comparing `ligo.skymap-1.1.0/CONTRIBUTING.rst` & `ligo.skymap-1.1.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.1.0/PKG-INFO` & `ligo.skymap-1.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ligo.skymap
-Version: 1.1.0
+Version: 1.1.1
 Summary: Tools for reading, writing, manipulating, and making LIGO and Virgo sky maps
 Home-page: https://lscsoft.docs.ligo.org/ligo.skymap/
 Author: Leo Singer
 Author-email: leo.singer@ligo.org
 License: GNU GPL v3+
 Project-URL: Bug Tracker, https://git.ligo.org/lscsoft/ligo.skymap/issues
 Project-URL: Change Log, https://lscsoft.docs.ligo.org/ligo.skymap/changes.html
@@ -21,14 +21,15 @@
 Classifier: Programming Language :: C
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Classifier: Topic :: Scientific/Engineering :: Physics
+Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 Provides-Extra: test
 Provides-Extra: docs
 License-File: licenses/LICENSE.rst
 
 ###########
 ligo.skymap
```

### Comparing `ligo.skymap-1.1.0/README.rst` & `ligo.skymap-1.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.1.0/cextern/chealpix/chealpix.c` & `ligo.skymap-1.1.1/cextern/chealpix/chealpix.c`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.1.0/cextern/chealpix/chealpix.h` & `ligo.skymap-1.1.1/cextern/chealpix/chealpix.h`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.1.0/docs/Makefile` & `ligo.skymap-1.1.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.1.0/docs/_static/coinc.xml` & `ligo.skymap-1.1.1/docs/_static/coinc.xml`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.1.0/docs/_static/localization.svg` & `ligo.skymap-1.1.1/docs/_static/localization.svg`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.1.0/docs/bayestar/eggbox.png` & `ligo.skymap-1.1.1/docs/bayestar/eggbox.png`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.1.0/docs/changes.rst` & `ligo.skymap-1.1.1/docs/changes.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,18 @@
 #########
 Changelog
 #########
 
+1.1.1 (2023-07-08)
+==================
+
+- Fix a typo in the ``setup.cfg`` file that prevented correct interpretation of
+  the minimum Python version. Contributed by
+  `@ahnitz <https://github.com/ahnitz>`_.
+
 1.1.0 (2023-07-07)
 ==================
 
 - Add ``max_depth`` keyword argument to the call to
   ``MOC.from_valued_healpix_cells`` in ``ligo-skymap-contour-moc``.
   Contributed by `@parkma99 <https://github.com/parkma99>`_.
```

### Comparing `ligo.skymap-1.1.0/docs/conf.py` & `ligo.skymap-1.1.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.1.0/docs/contributing.rst` & `ligo.skymap-1.1.1/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.1.0/docs/develop.rst` & `ligo.skymap-1.1.1/docs/develop.rst`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.1.0/docs/distance/index.rst` & `ligo.skymap-1.1.1/docs/distance/index.rst`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.1.0/docs/help.rst` & `ligo.skymap-1.1.1/docs/help.rst`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.1.0/docs/index.rst` & `ligo.skymap-1.1.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.1.0/docs/interface.rst` & `ligo.skymap-1.1.1/docs/interface.rst`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.1.0/docs/io/events.rst` & `ligo.skymap-1.1.1/docs/io/events.rst`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.1.0/docs/make.bat` & `ligo.skymap-1.1.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.1.0/docs/performance.rst` & `ligo.skymap-1.1.1/docs/performance.rst`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.1.0/docs/quickstart/bayestar-injections.rst` & `ligo.skymap-1.1.1/docs/quickstart/bayestar-injections.rst`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.1.0/docs/quickstart/install.rst` & `ligo.skymap-1.1.1/docs/quickstart/install.rst`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.1.0/docs/testing.rst` & `ligo.skymap-1.1.1/docs/testing.rst`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.1.0/docs/tool/ligo_skymap_combine.rst` & `ligo.skymap-1.1.1/docs/tool/ligo_skymap_combine.rst`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.1.0/docs/tool/ligo_skymap_constellations.rst` & `ligo.skymap-1.1.1/docs/tool/ligo_skymap_constellations.rst`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.1.0/docs/tool/ligo_skymap_from_samples.rst` & `ligo.skymap-1.1.1/docs/tool/ligo_skymap_from_samples.rst`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.1.0/docs/tool/ligo_skymap_plot.rst` & `ligo.skymap-1.1.1/docs/tool/ligo_skymap_plot.rst`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.1.0/docs/tool/ligo_skymap_plot_airmass.rst` & `ligo.skymap-1.1.1/docs/tool/ligo_skymap_plot_airmass.rst`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.1.0/docs/tool/ligo_skymap_plot_coherence.rst` & `ligo.skymap-1.1.1/docs/tool/ligo_skymap_plot_coherence.rst`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.1.0/docs/tool/ligo_skymap_plot_observability.rst` & `ligo.skymap-1.1.1/docs/tool/ligo_skymap_plot_observability.rst`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.1.0/docs/tool/ligo_skymap_plot_volume.rst` & `ligo.skymap-1.1.1/docs/tool/ligo_skymap_plot_volume.rst`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.1.0/licenses/CHEALPIX_LICENSE.rst` & `ligo.skymap-1.1.1/licenses/CHEALPIX_LICENSE.rst`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.1.0/licenses/LICENSE.rst` & `ligo.skymap-1.1.1/licenses/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.1.0/licenses/NUMPY_LICENSE.rst` & `ligo.skymap-1.1.1/licenses/NUMPY_LICENSE.rst`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.1.0/licenses/TEMPLATE_LICENCE.rst` & `ligo.skymap-1.1.1/licenses/TEMPLATE_LICENCE.rst`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.1.0/ligo/skymap/__init__.py` & `ligo.skymap-1.1.1/ligo/skymap/__init__.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.1.0/ligo/skymap/_astropy_init.py` & `ligo.skymap-1.1.1/ligo/skymap/_astropy_init.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.1.0/ligo/skymap/bayestar/__init__.py` & `ligo.skymap-1.1.1/ligo/skymap/bayestar/__init__.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.1.0/ligo/skymap/bayestar/ez_emcee.py` & `ligo.skymap-1.1.1/ligo/skymap/bayestar/ez_emcee.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.1.0/ligo/skymap/bayestar/filter.py` & `ligo.skymap-1.1.1/ligo/skymap/bayestar/filter.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.1.0/ligo/skymap/bayestar/interpolation.py` & `ligo.skymap-1.1.1/ligo/skymap/bayestar/interpolation.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.1.0/ligo/skymap/bayestar/ptemcee.py` & `ligo.skymap-1.1.1/ligo/skymap/bayestar/ptemcee.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.1.0/ligo/skymap/bayestar/tests/test_bayestar.py` & `ligo.skymap-1.1.1/ligo/skymap/bayestar/tests/test_bayestar.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.1.0/ligo/skymap/bayestar/tests/test_interpolation.py` & `ligo.skymap-1.1.1/ligo/skymap/bayestar/tests/test_interpolation.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.1.0/ligo/skymap/bayestar/tests/test_signal_amplitude_model.py` & `ligo.skymap-1.1.1/ligo/skymap/bayestar/tests/test_signal_amplitude_model.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.1.0/ligo/skymap/conftest.py` & `ligo.skymap-1.1.1/ligo/skymap/conftest.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.1.0/ligo/skymap/coordinates/detector.py` & `ligo.skymap-1.1.1/ligo/skymap/coordinates/detector.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.1.0/ligo/skymap/coordinates/eigenframe.py` & `ligo.skymap-1.1.1/ligo/skymap/coordinates/eigenframe.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.1.0/ligo/skymap/coordinates/tests/test_detector.py` & `ligo.skymap-1.1.1/ligo/skymap/coordinates/tests/test_detector.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.1.0/ligo/skymap/distance.py` & `ligo.skymap-1.1.1/ligo/skymap/distance.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.1.0/ligo/skymap/extern/numpy/quantile.py` & `ligo.skymap-1.1.1/ligo/skymap/extern/numpy/quantile.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.1.0/ligo/skymap/healpix_tree.py` & `ligo.skymap-1.1.1/ligo/skymap/healpix_tree.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.1.0/ligo/skymap/io/events/base.py` & `ligo.skymap-1.1.1/ligo/skymap/io/events/base.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.1.0/ligo/skymap/io/events/detector_disabled.py` & `ligo.skymap-1.1.1/ligo/skymap/io/events/detector_disabled.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.1.0/ligo/skymap/io/events/gracedb.py` & `ligo.skymap-1.1.1/ligo/skymap/io/events/gracedb.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.1.0/ligo/skymap/io/events/hdf.py` & `ligo.skymap-1.1.1/ligo/skymap/io/events/hdf.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.1.0/ligo/skymap/io/events/ligolw.py` & `ligo.skymap-1.1.1/ligo/skymap/io/events/ligolw.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.1.0/ligo/skymap/io/events/magic.py` & `ligo.skymap-1.1.1/ligo/skymap/io/events/magic.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.1.0/ligo/skymap/io/events/sqlite.py` & `ligo.skymap-1.1.1/ligo/skymap/io/events/sqlite.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.1.0/ligo/skymap/io/fits.py` & `ligo.skymap-1.1.1/ligo/skymap/io/fits.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.1.0/ligo/skymap/io/hdf5.py` & `ligo.skymap-1.1.1/ligo/skymap/io/hdf5.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.1.0/ligo/skymap/io/tests/data/2016_subset.xml.gz` & `ligo.skymap-1.1.1/ligo/skymap/io/tests/data/2016_subset.xml.gz`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.1.0/ligo/skymap/io/tests/data/G197392_coinc.xml.gz` & `ligo.skymap-1.1.1/ligo/skymap/io/tests/data/G197392_coinc.xml.gz`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.1.0/ligo/skymap/io/tests/data/G197392_psd.xml.gz` & `ligo.skymap-1.1.1/ligo/skymap/io/tests/data/G197392_psd.xml.gz`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.1.0/ligo/skymap/io/tests/data/G211117_coinc.xml.gz` & `ligo.skymap-1.1.1/ligo/skymap/io/tests/data/G211117_coinc.xml.gz`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.1.0/ligo/skymap/io/tests/data/G211117_psd.xml.gz` & `ligo.skymap-1.1.1/ligo/skymap/io/tests/data/G211117_psd.xml.gz`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.1.0/ligo/skymap/io/tests/data/gstlal_reference_psd/H1L1V1-REFERENCE_PSD-967234210-29963.xml.gz` & `ligo.skymap-1.1.1/ligo/skymap/io/tests/data/gstlal_reference_psd/H1L1V1-REFERENCE_PSD-967234210-29963.xml.gz`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.1.0/ligo/skymap/io/tests/data/test.hdf5` & `ligo.skymap-1.1.1/ligo/skymap/io/tests/data/test.hdf5`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.1.0/ligo/skymap/io/tests/test_io_events.py` & `ligo.skymap-1.1.1/ligo/skymap/io/tests/test_io_events.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.1.0/ligo/skymap/kde.py` & `ligo.skymap-1.1.1/ligo/skymap/kde.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.1.0/ligo/skymap/moc.py` & `ligo.skymap-1.1.1/ligo/skymap/moc.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.1.0/ligo/skymap/plot/allsky.py` & `ligo.skymap-1.1.1/ligo/skymap/plot/allsky.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.1.0/ligo/skymap/plot/angle.py` & `ligo.skymap-1.1.1/ligo/skymap/plot/angle.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.1.0/ligo/skymap/plot/backdrop.py` & `ligo.skymap-1.1.1/ligo/skymap/plot/backdrop.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.1.0/ligo/skymap/plot/bayes_factor.py` & `ligo.skymap-1.1.1/ligo/skymap/plot/bayes_factor.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.1.0/ligo/skymap/plot/cmap.py` & `ligo.skymap-1.1.1/ligo/skymap/plot/cmap.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.1.0/ligo/skymap/plot/cylon.csv` & `ligo.skymap-1.1.1/ligo/skymap/plot/cylon.csv`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.1.0/ligo/skymap/plot/cylon.py` & `ligo.skymap-1.1.1/ligo/skymap/plot/cylon.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.1.0/ligo/skymap/plot/marker.py` & `ligo.skymap-1.1.1/ligo/skymap/plot/marker.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.1.0/ligo/skymap/plot/ne_simplified_coastline.json` & `ligo.skymap-1.1.1/ligo/skymap/plot/ne_simplified_coastline.json`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.1.0/ligo/skymap/plot/poly.py` & `ligo.skymap-1.1.1/ligo/skymap/plot/poly.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.1.0/ligo/skymap/plot/pp.py` & `ligo.skymap-1.1.1/ligo/skymap/plot/pp.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.1.0/ligo/skymap/plot/tests/baseline/test_allsky_axes_astro-degrees-aitoff.png` & `ligo.skymap-1.1.1/ligo/skymap/plot/tests/baseline/test_allsky_axes_astro-degrees-aitoff.png`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.1.0/ligo/skymap/plot/tests/baseline/test_allsky_axes_astro-degrees-mollweide.png` & `ligo.skymap-1.1.1/ligo/skymap/plot/tests/baseline/test_allsky_axes_astro-degrees-mollweide.png`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.1.0/ligo/skymap/plot/tests/baseline/test_allsky_axes_astro-hours-aitoff.png` & `ligo.skymap-1.1.1/ligo/skymap/plot/tests/baseline/test_allsky_axes_astro-hours-aitoff.png`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.1.0/ligo/skymap/plot/tests/baseline/test_allsky_axes_astro-hours-mollweide.png` & `ligo.skymap-1.1.1/ligo/skymap/plot/tests/baseline/test_allsky_axes_astro-hours-mollweide.png`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.1.0/ligo/skymap/plot/tests/baseline/test_allsky_axes_galactic-degrees-aitoff.png` & `ligo.skymap-1.1.1/ligo/skymap/plot/tests/baseline/test_allsky_axes_galactic-degrees-aitoff.png`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.1.0/ligo/skymap/plot/tests/baseline/test_allsky_axes_galactic-degrees-mollweide.png` & `ligo.skymap-1.1.1/ligo/skymap/plot/tests/baseline/test_allsky_axes_galactic-degrees-mollweide.png`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.1.0/ligo/skymap/plot/tests/baseline/test_allsky_axes_galactic-hours-aitoff.png` & `ligo.skymap-1.1.1/ligo/skymap/plot/tests/baseline/test_allsky_axes_galactic-hours-aitoff.png`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.1.0/ligo/skymap/plot/tests/baseline/test_allsky_axes_galactic-hours-mollweide.png` & `ligo.skymap-1.1.1/ligo/skymap/plot/tests/baseline/test_allsky_axes_galactic-hours-mollweide.png`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.1.0/ligo/skymap/plot/tests/baseline/test_allsky_axes_geo-degrees-aitoff.png` & `ligo.skymap-1.1.1/ligo/skymap/plot/tests/baseline/test_allsky_axes_geo-degrees-aitoff.png`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.1.0/ligo/skymap/plot/tests/baseline/test_allsky_axes_geo-degrees-mollweide.png` & `ligo.skymap-1.1.1/ligo/skymap/plot/tests/baseline/test_allsky_axes_geo-degrees-mollweide.png`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.1.0/ligo/skymap/plot/tests/baseline/test_allsky_axes_geo-hours-aitoff.png` & `ligo.skymap-1.1.1/ligo/skymap/plot/tests/baseline/test_allsky_axes_geo-hours-aitoff.png`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.1.0/ligo/skymap/plot/tests/baseline/test_allsky_axes_geo-hours-mollweide.png` & `ligo.skymap-1.1.1/ligo/skymap/plot/tests/baseline/test_allsky_axes_geo-hours-mollweide.png`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.1.0/ligo/skymap/plot/tests/baseline/test_allsky_obstime.png` & `ligo.skymap-1.1.1/ligo/skymap/plot/tests/baseline/test_allsky_obstime.png`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.1.0/ligo/skymap/plot/tests/baseline/test_globe_axes.png` & `ligo.skymap-1.1.1/ligo/skymap/plot/tests/baseline/test_globe_axes.png`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.1.0/ligo/skymap/plot/tests/baseline/test_pp_plot_default.png` & `ligo.skymap-1.1.1/ligo/skymap/plot/tests/baseline/test_pp_plot_default.png`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.1.0/ligo/skymap/plot/tests/baseline/test_pp_plot_lines.png` & `ligo.skymap-1.1.1/ligo/skymap/plot/tests/baseline/test_pp_plot_lines.png`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.1.0/ligo/skymap/plot/tests/baseline/test_pp_plot_steps.png` & `ligo.skymap-1.1.1/ligo/skymap/plot/tests/baseline/test_pp_plot_steps.png`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.1.0/ligo/skymap/plot/tests/baseline/test_reticle.png` & `ligo.skymap-1.1.1/ligo/skymap/plot/tests/baseline/test_reticle.png`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.1.0/ligo/skymap/plot/tests/baseline/test_zoom_axes.png` & `ligo.skymap-1.1.1/ligo/skymap/plot/tests/baseline/test_zoom_axes.png`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.1.0/ligo/skymap/plot/tests/test_plot.py` & `ligo.skymap-1.1.1/ligo/skymap/plot/tests/test_plot.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.1.0/ligo/skymap/plot/util.py` & `ligo.skymap-1.1.1/ligo/skymap/plot/util.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.1.0/ligo/skymap/postprocess/contour.py` & `ligo.skymap-1.1.1/ligo/skymap/postprocess/contour.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.1.0/ligo/skymap/postprocess/cosmology.py` & `ligo.skymap-1.1.1/ligo/skymap/postprocess/cosmology.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.1.0/ligo/skymap/postprocess/crossmatch.py` & `ligo.skymap-1.1.1/ligo/skymap/postprocess/crossmatch.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.1.0/ligo/skymap/postprocess/ellipse.py` & `ligo.skymap-1.1.1/ligo/skymap/postprocess/ellipse.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.1.0/ligo/skymap/postprocess/tests/test_cosmology.py` & `ligo.skymap-1.1.1/ligo/skymap/postprocess/tests/test_cosmology.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.1.0/ligo/skymap/postprocess/tests/test_crossmatch.py` & `ligo.skymap-1.1.1/ligo/skymap/postprocess/tests/test_crossmatch.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.1.0/ligo/skymap/postprocess/util.py` & `ligo.skymap-1.1.1/ligo/skymap/postprocess/util.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.1.0/ligo/skymap/tests/plugins/omp.py` & `ligo.skymap-1.1.1/ligo/skymap/tests/plugins/omp.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.1.0/ligo/skymap/tests/test_moc.py` & `ligo.skymap-1.1.1/ligo/skymap/tests/test_moc.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.1.0/ligo/skymap/tool/__init__.py` & `ligo.skymap-1.1.1/ligo/skymap/tool/__init__.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.1.0/ligo/skymap/tool/bayestar_inject.py` & `ligo.skymap-1.1.1/ligo/skymap/tool/bayestar_inject.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.1.0/ligo/skymap/tool/bayestar_localize_coincs.py` & `ligo.skymap-1.1.1/ligo/skymap/tool/bayestar_localize_coincs.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.1.0/ligo/skymap/tool/bayestar_localize_lvalert.py` & `ligo.skymap-1.1.1/ligo/skymap/tool/bayestar_localize_lvalert.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.1.0/ligo/skymap/tool/bayestar_mcmc.py` & `ligo.skymap-1.1.1/ligo/skymap/tool/bayestar_mcmc.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.1.0/ligo/skymap/tool/bayestar_realize_coincs.py` & `ligo.skymap-1.1.1/ligo/skymap/tool/bayestar_realize_coincs.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.1.0/ligo/skymap/tool/bayestar_sample_model_psd.py` & `ligo.skymap-1.1.1/ligo/skymap/tool/bayestar_sample_model_psd.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.1.0/ligo/skymap/tool/ligo_skymap_combine.py` & `ligo.skymap-1.1.1/ligo/skymap/tool/ligo_skymap_combine.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.1.0/ligo/skymap/tool/ligo_skymap_constellations.py` & `ligo.skymap-1.1.1/ligo/skymap/tool/ligo_skymap_constellations.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.1.0/ligo/skymap/tool/ligo_skymap_contour.py` & `ligo.skymap-1.1.1/ligo/skymap/tool/ligo_skymap_contour.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.1.0/ligo/skymap/tool/ligo_skymap_contour_moc.py` & `ligo.skymap-1.1.1/ligo/skymap/tool/ligo_skymap_contour_moc.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.1.0/ligo/skymap/tool/ligo_skymap_flatten.py` & `ligo.skymap-1.1.1/ligo/skymap/tool/ligo_skymap_flatten.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.1.0/ligo/skymap/tool/ligo_skymap_from_samples.py` & `ligo.skymap-1.1.1/ligo/skymap/tool/ligo_skymap_from_samples.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.1.0/ligo/skymap/tool/ligo_skymap_plot.py` & `ligo.skymap-1.1.1/ligo/skymap/tool/ligo_skymap_plot.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.1.0/ligo/skymap/tool/ligo_skymap_plot_airmass.py` & `ligo.skymap-1.1.1/ligo/skymap/tool/ligo_skymap_plot_airmass.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.1.0/ligo/skymap/tool/ligo_skymap_plot_coherence.py` & `ligo.skymap-1.1.1/ligo/skymap/tool/ligo_skymap_plot_coherence.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.1.0/ligo/skymap/tool/ligo_skymap_plot_observability.py` & `ligo.skymap-1.1.1/ligo/skymap/tool/ligo_skymap_plot_observability.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.1.0/ligo/skymap/tool/ligo_skymap_plot_pp_samples.py` & `ligo.skymap-1.1.1/ligo/skymap/tool/ligo_skymap_plot_pp_samples.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.1.0/ligo/skymap/tool/ligo_skymap_plot_stats.py` & `ligo.skymap-1.1.1/ligo/skymap/tool/ligo_skymap_plot_stats.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.1.0/ligo/skymap/tool/ligo_skymap_plot_volume.py` & `ligo.skymap-1.1.1/ligo/skymap/tool/ligo_skymap_plot_volume.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.1.0/ligo/skymap/tool/ligo_skymap_stats.py` & `ligo.skymap-1.1.1/ligo/skymap/tool/ligo_skymap_stats.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.1.0/ligo/skymap/tool/ligo_skymap_unflatten.py` & `ligo.skymap-1.1.1/ligo/skymap/tool/ligo_skymap_unflatten.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.1.0/ligo/skymap/tool/matplotlib.py` & `ligo.skymap-1.1.1/ligo/skymap/tool/matplotlib.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.1.0/ligo/skymap/tool/tests/__init__.py` & `ligo.skymap-1.1.1/ligo/skymap/tool/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.1.0/ligo/skymap/tool/tests/test_bayestar.py` & `ligo.skymap-1.1.1/ligo/skymap/tool/tests/test_bayestar.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.1.0/ligo/skymap/tool/tests/test_bayestar_inject.py` & `ligo.skymap-1.1.1/ligo/skymap/tool/tests/test_bayestar_inject.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.1.0/ligo/skymap/tool/tests/test_combine.py` & `ligo.skymap-1.1.1/ligo/skymap/tool/tests/test_combine.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.1.0/ligo/skymap/tool/tests/test_flatten.py` & `ligo.skymap-1.1.1/ligo/skymap/tool/tests/test_flatten.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.1.0/ligo/skymap/tool/tests/test_from_samples.py` & `ligo.skymap-1.1.1/ligo/skymap/tool/tests/test_from_samples.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.1.0/ligo/skymap/tool/tests/test_help.py` & `ligo.skymap-1.1.1/ligo/skymap/tool/tests/test_help.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.1.0/ligo/skymap/tool/tests/test_plot.py` & `ligo.skymap-1.1.1/ligo/skymap/tool/tests/test_plot.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.1.0/ligo/skymap/tool/tests/test_plot_stats.py` & `ligo.skymap-1.1.1/ligo/skymap/tool/tests/test_plot_stats.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.1.0/ligo/skymap/util/file.py` & `ligo.skymap-1.1.1/ligo/skymap/util/file.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.1.0/ligo/skymap/util/ilwd.py` & `ligo.skymap-1.1.1/ligo/skymap/util/ilwd.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.1.0/ligo/skymap/util/numpy.py` & `ligo.skymap-1.1.1/ligo/skymap/util/numpy.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.1.0/ligo/skymap/util/progress.py` & `ligo.skymap-1.1.1/ligo/skymap/util/progress.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.1.0/ligo/skymap/util/sqlite.py` & `ligo.skymap-1.1.1/ligo/skymap/util/sqlite.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.1.0/ligo/skymap/util/stopwatch.py` & `ligo.skymap-1.1.1/ligo/skymap/util/stopwatch.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.1.0/ligo.skymap.egg-info/PKG-INFO` & `ligo.skymap-1.1.1/ligo.skymap.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ligo.skymap
-Version: 1.1.0
+Version: 1.1.1
 Summary: Tools for reading, writing, manipulating, and making LIGO and Virgo sky maps
 Home-page: https://lscsoft.docs.ligo.org/ligo.skymap/
 Author: Leo Singer
 Author-email: leo.singer@ligo.org
 License: GNU GPL v3+
 Project-URL: Bug Tracker, https://git.ligo.org/lscsoft/ligo.skymap/issues
 Project-URL: Change Log, https://lscsoft.docs.ligo.org/ligo.skymap/changes.html
@@ -21,14 +21,15 @@
 Classifier: Programming Language :: C
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Classifier: Topic :: Scientific/Engineering :: Physics
+Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 Provides-Extra: test
 Provides-Extra: docs
 License-File: licenses/LICENSE.rst
 
 ###########
 ligo.skymap
```

### Comparing `ligo.skymap-1.1.0/ligo.skymap.egg-info/SOURCES.txt` & `ligo.skymap-1.1.1/ligo.skymap.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.1.0/ligo.skymap.egg-info/entry_points.txt` & `ligo.skymap-1.1.1/ligo.skymap.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.1.0/setup.cfg` & `ligo.skymap-1.1.1/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 	Documentation = https://lscsoft.docs.ligo.org/ligo.skymap
 	GitHub = https://github.com/lpsinger/ligo.skymap
 	Source Code = https://git.ligo.org/lscsoft/ligo.skymap
 
 [options]
 zip_safe = False
 packages = find_namespace:
-python_version = >=3.9
+python_requires = >=3.9
 setup_requires = setuptools_scm
 install_requires = 
 	astroplan>=0.7  # https://github.com/astropy/astroplan/issues/479
 	astropy>=5.0  # https://github.com/astropy/astropy/pull/12176
 	astropy-healpix>=0.3  # https://github.com/astropy/astropy-healpix/pull/106
 	healpy
 	h5py
```

### Comparing `ligo.skymap-1.1.0/setup.py` & `ligo.skymap-1.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.1.0/src/bayestar_cosmology.h` & `ligo.skymap-1.1.1/src/bayestar_cosmology.h`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.1.0/src/bayestar_cosmology.py` & `ligo.skymap-1.1.1/src/bayestar_cosmology.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.1.0/src/bayestar_distance.c` & `ligo.skymap-1.1.1/src/bayestar_distance.c`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.1.0/src/bayestar_distance.h` & `ligo.skymap-1.1.1/src/bayestar_distance.h`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.1.0/src/bayestar_moc.c` & `ligo.skymap-1.1.1/src/bayestar_moc.c`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.1.0/src/bayestar_moc.h` & `ligo.skymap-1.1.1/src/bayestar_moc.h`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.1.0/src/bayestar_sky_map.c` & `ligo.skymap-1.1.1/src/bayestar_sky_map.c`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.1.0/src/bayestar_sky_map.h` & `ligo.skymap-1.1.1/src/bayestar_sky_map.h`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.1.0/src/core.c` & `ligo.skymap-1.1.1/src/core.c`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.1.0/src/cubic_interp.c` & `ligo.skymap-1.1.1/src/cubic_interp.c`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.1.0/src/cubic_interp.h` & `ligo.skymap-1.1.1/src/cubic_interp.h`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.1.0/src/cubic_interp_test.c` & `ligo.skymap-1.1.1/src/cubic_interp_test.c`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.1.0/src/omp_interruptible.h` & `ligo.skymap-1.1.1/src/omp_interruptible.h`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.1.0/src/vmath.h` & `ligo.skymap-1.1.1/src/vmath.h`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.1.0/src/warnings.h` & `ligo.skymap-1.1.1/src/warnings.h`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.1.0/tox.ini` & `ligo.skymap-1.1.1/tox.ini`

 * *Files identical despite different names*

