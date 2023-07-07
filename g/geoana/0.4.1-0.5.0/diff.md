# Comparing `tmp/geoana-0.4.1.tar.gz` & `tmp/geoana-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geoana-0.4.1.tar", last modified: Thu Jul  6 18:53:41 2023, max compression
+gzip compressed data, was "geoana-0.5.0.tar", last modified: Fri Jul  7 22:49:16 2023, max compression
```

## Comparing `geoana-0.4.1.tar` & `geoana-0.5.0.tar`

### file list

```diff
@@ -1,78 +1,61 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:53:41.747113 geoana-0.4.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-06 18:51:22.000000 geoana-0.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-06 18:51:22.000000 geoana-0.4.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3585 2023-07-06 18:53:41.747113 geoana-0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2550 2023-07-06 18:51:22.000000 geoana-0.4.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:53:41.739113 geoana-0.4.1/geoana/
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-07-06 18:51:22.000000 geoana-0.4.1/geoana/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:53:41.739113 geoana-0.4.1/geoana/earthquake/
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-07-06 18:51:22.000000 geoana-0.4.1/geoana/earthquake/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    43873 2023-07-06 18:51:22.000000 geoana-0.4.1/geoana/earthquake/oksar.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:53:41.739113 geoana-0.4.1/geoana/em/
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-07-06 18:51:22.000000 geoana-0.4.1/geoana/em/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14000 2023-07-06 18:51:22.000000 geoana-0.4.1/geoana/em/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:53:41.743113 geoana-0.4.1/geoana/em/fdem/
--rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-07-06 18:51:22.000000 geoana-0.4.1/geoana/em/fdem/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10864 2023-07-06 18:51:22.000000 geoana-0.4.1/geoana/em/fdem/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4952 2023-07-06 18:51:22.000000 geoana-0.4.1/geoana/em/fdem/halfspace.py
--rw-r--r--   0 runner    (1001) docker     (123)    18894 2023-07-06 18:51:22.000000 geoana-0.4.1/geoana/em/fdem/layered.py
--rw-r--r--   0 runner    (1001) docker     (123)     5064 2023-07-06 18:51:22.000000 geoana-0.4.1/geoana/em/fdem/simple_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    48584 2023-07-06 18:51:22.000000 geoana-0.4.1/geoana/em/fdem/wholespace.py
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-07-06 18:51:22.000000 geoana-0.4.1/geoana/em/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:53:41.743113 geoana-0.4.1/geoana/em/static/
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-07-06 18:51:22.000000 geoana-0.4.1/geoana/em/static/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13137 2023-07-06 18:51:22.000000 geoana-0.4.1/geoana/em/static/freespace.py
--rw-r--r--   0 runner    (1001) docker     (123)    24482 2023-07-06 18:51:22.000000 geoana-0.4.1/geoana/em/static/halfspace.py
--rw-r--r--   0 runner    (1001) docker     (123)    31922 2023-07-06 18:51:22.000000 geoana-0.4.1/geoana/em/static/sphere.py
--rw-r--r--   0 runner    (1001) docker     (123)    38382 2023-07-06 18:51:22.000000 geoana-0.4.1/geoana/em/static/wholespace.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:53:41.743113 geoana-0.4.1/geoana/em/tdem/
--rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-07-06 18:51:22.000000 geoana-0.4.1/geoana/em/tdem/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8543 2023-07-06 18:51:22.000000 geoana-0.4.1/geoana/em/tdem/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2929 2023-07-06 18:51:22.000000 geoana-0.4.1/geoana/em/tdem/halfspace.py
--rw-r--r--   0 runner    (1001) docker     (123)    15326 2023-07-06 18:51:22.000000 geoana-0.4.1/geoana/em/tdem/simple_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    36451 2023-07-06 18:51:22.000000 geoana-0.4.1/geoana/em/tdem/wholespace.py
--rw-r--r--   0 runner    (1001) docker     (123)    20996 2023-07-06 18:51:22.000000 geoana-0.4.1/geoana/gravity.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:53:41.743113 geoana-0.4.1/geoana/kernels/
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-07-06 18:51:22.000000 geoana-0.4.1/geoana/kernels/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:53:41.743113 geoana-0.4.1/geoana/kernels/_extensions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 18:51:22.000000 geoana-0.4.1/geoana/kernels/_extensions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5192 2023-07-06 18:51:22.000000 geoana-0.4.1/geoana/kernels/_extensions/_rTE.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-07-06 18:51:22.000000 geoana-0.4.1/geoana/kernels/_extensions/_rTE.h
--rw-r--r--   0 runner    (1001) docker     (123)    17198 2023-07-06 18:51:22.000000 geoana-0.4.1/geoana/kernels/_extensions/potential_field_prism.c
--rw-r--r--   0 runner    (1001) docker     (123)   973806 2023-07-06 18:53:41.000000 geoana-0.4.1/geoana/kernels/_extensions/rTE.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     7325 2023-07-06 18:51:22.000000 geoana-0.4.1/geoana/kernels/_extensions/rTE.pyx
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-07-06 18:51:22.000000 geoana-0.4.1/geoana/kernels/_extensions/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     7012 2023-07-06 18:51:22.000000 geoana-0.4.1/geoana/kernels/potential_field_prism.py
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-07-06 18:51:22.000000 geoana-0.4.1/geoana/kernels/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     4886 2023-07-06 18:51:22.000000 geoana-0.4.1/geoana/kernels/tranverse_electric_reflections.py
--rw-r--r--   0 runner    (1001) docker     (123)     8704 2023-07-06 18:51:22.000000 geoana-0.4.1/geoana/plotting_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-07-06 18:51:22.000000 geoana-0.4.1/geoana/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     3895 2023-07-06 18:51:22.000000 geoana-0.4.1/geoana/shapes.py
--rw-r--r--   0 runner    (1001) docker     (123)    21783 2023-07-06 18:51:22.000000 geoana-0.4.1/geoana/spatial.py
--rw-r--r--   0 runner    (1001) docker     (123)     5032 2023-07-06 18:51:22.000000 geoana-0.4.1/geoana/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:53:41.739113 geoana-0.4.1/geoana.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3585 2023-07-06 18:53:41.000000 geoana-0.4.1/geoana.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-07-06 18:53:41.000000 geoana-0.4.1/geoana.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 18:53:41.000000 geoana-0.4.1/geoana.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-06 18:53:41.000000 geoana-0.4.1/geoana.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-06 18:53:41.000000 geoana-0.4.1/geoana.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 18:53:41.747113 geoana-0.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2768 2023-07-06 18:51:22.000000 geoana-0.4.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:53:41.747113 geoana-0.4.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-06 18:51:22.000000 geoana-0.4.1/tests/test_docs.py
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-07-06 18:51:22.000000 geoana-0.4.1/tests/test_earthquake_oksar.py
--rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-07-06 18:51:22.000000 geoana-0.4.1/tests/test_em_fdem_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    11324 2023-07-06 18:51:22.000000 geoana-0.4.1/tests/test_em_fdem_electric_dipole.py
--rw-r--r--   0 runner    (1001) docker     (123)    14839 2023-07-06 18:51:22.000000 geoana-0.4.1/tests/test_em_fdem_layered.py
--rw-r--r--   0 runner    (1001) docker     (123)    14730 2023-07-06 18:51:22.000000 geoana-0.4.1/tests/test_em_fdem_magnetic_dipole.py
--rw-r--r--   0 runner    (1001) docker     (123)     5312 2023-07-06 18:51:22.000000 geoana-0.4.1/tests/test_em_fdem_planewave.py
--rw-r--r--   0 runner    (1001) docker     (123)     4002 2023-07-06 18:51:22.000000 geoana-0.4.1/tests/test_em_simple.py
--rw-r--r--   0 runner    (1001) docker     (123)    54251 2023-07-06 18:51:22.000000 geoana-0.4.1/tests/test_em_static.py
--rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-07-06 18:51:22.000000 geoana-0.4.1/tests/test_em_tdem_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4476 2023-07-06 18:51:22.000000 geoana-0.4.1/tests/test_em_tdem_halfspace.py
--rw-r--r--   0 runner    (1001) docker     (123)     5408 2023-07-06 18:51:22.000000 geoana-0.4.1/tests/test_em_tdem_planewave.py
--rw-r--r--   0 runner    (1001) docker     (123)     7199 2023-07-06 18:51:22.000000 geoana-0.4.1/tests/test_gravity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-07-06 18:51:22.000000 geoana-0.4.1/tests/test_plotting_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9389 2023-07-06 18:51:22.000000 geoana-0.4.1/tests/test_potential_prism.py
--rw-r--r--   0 runner    (1001) docker     (123)     4382 2023-07-06 18:51:22.000000 geoana-0.4.1/tests/test_spatial.py
--rw-r--r--   0 runner    (1001) docker     (123)     2962 2023-07-06 18:51:22.000000 geoana-0.4.1/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 22:49:16.735088 geoana-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-07 22:47:03.000000 geoana-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3585 2023-07-07 22:49:16.735088 geoana-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2550 2023-07-07 22:47:03.000000 geoana-0.5.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 22:49:16.727088 geoana-0.5.0/geoana/
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-07-07 22:47:03.000000 geoana-0.5.0/geoana/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 22:49:16.731088 geoana-0.5.0/geoana/earthquake/
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-07-07 22:47:03.000000 geoana-0.5.0/geoana/earthquake/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-07-07 22:47:03.000000 geoana-0.5.0/geoana/earthquake/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44179 2023-07-07 22:47:03.000000 geoana-0.5.0/geoana/earthquake/oksar.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 22:49:16.731088 geoana-0.5.0/geoana/em/
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-07-07 22:47:03.000000 geoana-0.5.0/geoana/em/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14000 2023-07-07 22:47:03.000000 geoana-0.5.0/geoana/em/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 22:49:16.731088 geoana-0.5.0/geoana/em/fdem/
+-rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-07-07 22:47:03.000000 geoana-0.5.0/geoana/em/fdem/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10864 2023-07-07 22:47:03.000000 geoana-0.5.0/geoana/em/fdem/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4952 2023-07-07 22:47:03.000000 geoana-0.5.0/geoana/em/fdem/halfspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18637 2023-07-07 22:47:03.000000 geoana-0.5.0/geoana/em/fdem/layered.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5064 2023-07-07 22:47:03.000000 geoana-0.5.0/geoana/em/fdem/simple_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48584 2023-07-07 22:47:03.000000 geoana-0.5.0/geoana/em/fdem/wholespace.py
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-07-07 22:47:03.000000 geoana-0.5.0/geoana/em/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 22:49:16.731088 geoana-0.5.0/geoana/em/static/
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-07-07 22:47:03.000000 geoana-0.5.0/geoana/em/static/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13137 2023-07-07 22:47:03.000000 geoana-0.5.0/geoana/em/static/freespace.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24482 2023-07-07 22:47:03.000000 geoana-0.5.0/geoana/em/static/halfspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31922 2023-07-07 22:47:03.000000 geoana-0.5.0/geoana/em/static/sphere.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38382 2023-07-07 22:47:03.000000 geoana-0.5.0/geoana/em/static/wholespace.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 22:49:16.731088 geoana-0.5.0/geoana/em/tdem/
+-rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-07-07 22:47:03.000000 geoana-0.5.0/geoana/em/tdem/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8543 2023-07-07 22:47:03.000000 geoana-0.5.0/geoana/em/tdem/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2929 2023-07-07 22:47:03.000000 geoana-0.5.0/geoana/em/tdem/halfspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15326 2023-07-07 22:47:03.000000 geoana-0.5.0/geoana/em/tdem/simple_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36451 2023-07-07 22:47:03.000000 geoana-0.5.0/geoana/em/tdem/wholespace.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20996 2023-07-07 22:47:03.000000 geoana-0.5.0/geoana/gravity.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 22:49:16.731088 geoana-0.5.0/geoana/kernels/
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-07-07 22:47:03.000000 geoana-0.5.0/geoana/kernels/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 22:49:16.735088 geoana-0.5.0/geoana/kernels/_extensions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 22:47:03.000000 geoana-0.5.0/geoana/kernels/_extensions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5192 2023-07-07 22:47:03.000000 geoana-0.5.0/geoana/kernels/_extensions/_rTE.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-07-07 22:47:03.000000 geoana-0.5.0/geoana/kernels/_extensions/_rTE.h
+-rw-r--r--   0 runner    (1001) docker     (123)    17198 2023-07-07 22:47:03.000000 geoana-0.5.0/geoana/kernels/_extensions/potential_field_prism.c
+-rw-r--r--   0 runner    (1001) docker     (123)   974929 2023-07-07 22:49:16.000000 geoana-0.5.0/geoana/kernels/_extensions/rTE.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     7325 2023-07-07 22:47:03.000000 geoana-0.5.0/geoana/kernels/_extensions/rTE.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-07-07 22:47:03.000000 geoana-0.5.0/geoana/kernels/_extensions/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7012 2023-07-07 22:47:03.000000 geoana-0.5.0/geoana/kernels/potential_field_prism.py
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-07-07 22:47:03.000000 geoana-0.5.0/geoana/kernels/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4886 2023-07-07 22:47:03.000000 geoana-0.5.0/geoana/kernels/tranverse_electric_reflections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8832 2023-07-07 22:47:03.000000 geoana-0.5.0/geoana/plotting_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-07-07 22:47:03.000000 geoana-0.5.0/geoana/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3895 2023-07-07 22:47:03.000000 geoana-0.5.0/geoana/shapes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21783 2023-07-07 22:47:03.000000 geoana-0.5.0/geoana/spatial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6235 2023-07-07 22:47:03.000000 geoana-0.5.0/geoana/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-07 22:49:16.000000 geoana-0.5.0/geoana/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 22:49:16.731088 geoana-0.5.0/geoana.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3585 2023-07-07 22:49:16.000000 geoana-0.5.0/geoana.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-07-07 22:49:16.000000 geoana-0.5.0/geoana.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 22:49:16.000000 geoana-0.5.0/geoana.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-07 22:49:16.000000 geoana-0.5.0/geoana.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-07 22:49:16.000000 geoana-0.5.0/geoana.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 22:49:16.735088 geoana-0.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2753 2023-07-07 22:47:03.000000 geoana-0.5.0/setup.py
```

### Comparing `geoana-0.4.1/LICENSE` & `geoana-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `geoana-0.4.1/PKG-INFO` & `geoana-0.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geoana
-Version: 0.4.1
+Version: 0.5.0
 Summary: Analytic expressions for geophysical responses
 Home-page: https://www.simpeg.xyz
 Download-URL: https://github.com/simpeg/geoana
 Author: SimPEG developers
 Author-email: lindseyheagy@gmail.com
 License: MIT License
 Keywords: geophysics,electromagnetics
@@ -22,15 +22,15 @@
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS
 Classifier: Natural Language :: English
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 License-File: LICENSE
 
 | `getting_started`_ | `connecting`_ | `installing`_ | `license`_ | `documentation <https://geoana.simpeg.xyz/>`_ |
 
 geoana
 ======
```

### Comparing `geoana-0.4.1/README.rst` & `geoana-0.5.0/README.rst`

 * *Files identical despite different names*

### Comparing `geoana-0.4.1/geoana/earthquake/oksar.py` & `geoana-0.5.0/geoana/earthquake/oksar.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,17 +11,25 @@
     - oksar3:       added new line of sight calculator tjw feb 2003
     - Modified into Python by RowanCockett, 3point Science Aug 2014
 
 
 """
 
 import numpy as np
-import utm
-import matplotlib.pyplot as plt
+try:
+    import utm
+except ImportError:
+    utm = False
+try:
+    import matplotlib.pyplot as plt
+    matplotlib = True
+except ImportError:
+    matplotlib = False
 from datetime import datetime
+from geoana.utils import requires
 
 def _date_time_from_json(value):
     if len(value) == 10:
         return datetime.strptime(value.replace('-', '/'),'%Y/%m/%d')
     return datetime.strptime(value, '%Y-%m-%dT%H:%M:%SZ')
 
 
@@ -667,14 +675,15 @@
         data = self.data.copy()
         data = np.flipud(data.reshape(self.shape, order='F').T)
         data[data == 0] = np.nan
         data *= self.scaling
 
         return vectorNx, vectorNy, data
 
+    @requires({"matplotlib": matplotlib})
     def plot_interferogram(self, wrap=True, ax=None):
         """Plot interferogram
 
         Parameters
         ----------
         wrap: bool
             If ``True``, wrap the function
@@ -720,14 +729,15 @@
         ax.set_ylabel('Northing, m')
 
         cb = plt.colorbar(out, ax=ax)
         cb.set_label('Displacement, m')
 
         return out
 
+    @requires({"matplotlib": matplotlib})
     def plot_mask(self, ax=None, opacity=0.2):
         """Plot masked interferogram
 
         Parameters
         ----------
         ax: matplotlib.ax.Axes
             An axes object
@@ -762,14 +772,15 @@
         ax.set_xlabel('Easting, m (UTM Zone {})'.format(
             self.location_UTM_zone
         ))
         ax.set_ylabel('Northing, m')
 
         return out
 
+    @requires({"utm":utm})
     def get_LOS_vector(self, locations):
         """calculate beta - the angle at earth center between reference point
         and satellite nadir
 
         Parameters
         ----------
         locations: list
@@ -1510,14 +1521,15 @@
                 du = np.array([dux, duy, duz])
                 if((j+k) != 3):
                     u = + du + u
                 else:
                     u = - du + u
         return u
 
+    @requires({"matplotlib": matplotlib})
     def plot_displacement(self, eq=None, ax=None, wrap=True, mask_opacity=0.2):
         """Plot displacement/
 
         Parameters
         ----------
         eq: EarthquakeInterferogram
             Instance of ``EarthquakeInterferogram``
```

### Comparing `geoana-0.4.1/geoana/em/__init__.py` & `geoana-0.5.0/geoana/em/__init__.py`

 * *Files identical despite different names*

### Comparing `geoana-0.4.1/geoana/em/base.py` & `geoana-0.5.0/geoana/em/base.py`

 * *Files identical despite different names*

### Comparing `geoana-0.4.1/geoana/em/fdem/__init__.py` & `geoana-0.5.0/geoana/em/fdem/__init__.py`

 * *Files identical despite different names*

### Comparing `geoana-0.4.1/geoana/em/fdem/base.py` & `geoana-0.5.0/geoana/em/fdem/base.py`

 * *Files identical despite different names*

### Comparing `geoana-0.4.1/geoana/em/fdem/halfspace.py` & `geoana-0.5.0/geoana/em/fdem/halfspace.py`

 * *Files identical despite different names*

### Comparing `geoana-0.4.1/geoana/em/fdem/layered.py` & `geoana-0.5.0/geoana/em/fdem/layered.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import numpy as np
 from geoana.em.base import BaseMagneticDipole
 from geoana.em.fdem.base import BaseFDEM, sigma_hat
 from scipy.constants import mu_0, epsilon_0
-from empymod.utils import check_hankel
-from empymod.transform import get_dlf_points
 from geoana.kernels.tranverse_electric_reflections import rTE_forward
+import libdlf
 
 
 class MagneticDipoleLayeredHalfSpace(BaseFDEM, BaseMagneticDipole):
     """Simulation class for a harmonic magnetic dipole over a layered halfspace.
 
     This class is used to simulate the fields produced by a harmonic magnetic dipole
     source over a layered halfspace.
@@ -397,25 +396,21 @@
 
         if (xyz[:, 2] < 0.0).any():
             raise ValueError("Cannot compute fields below the surface")
         h = self.location[2]
         dxyz = xyz - self.location
         offsets = np.linalg.norm(dxyz[:, :-1], axis=-1)
 
-        # Comput transform operations
-        # -1 gives lagged convolution in dlf
-        ht, htarg = check_hankel('dlf', {'dlf': 'key_101_2009', 'pts_per_dec': 0}, 1)
-        fhtfilt = htarg['dlf']
-        pts_per_dec = htarg['pts_per_dec']
+        # Compute transform operations
+        filt_base, filt_j0, filt_j1 = libdlf.hankel.key_101_2009()
+        lambd = filt_base/offsets[:, None]
 
         f = self.frequency
         n_frequency = len(f)
 
-        lambd, int_points = get_dlf_points(fhtfilt, offsets, pts_per_dec)
-
         thick = self.thickness
         n_layer = len(thick) + 1
 
         thick, sigma, epsilon, mu = self._get_valid_properties_array()
 
         # sigh = sigma_hat(
         #     self.frequency[:, None], sigma, epsilon,
@@ -460,17 +455,17 @@
             C1x += (src_z*dxyz[:, 0]/offsets)[:, None]*lambd**2
             # C0y += 0.0
             C1y += (src_z*dxyz[:, 1]/offsets)[:, None]*lambd**2
             C0z += src_z*lambd**2
             # C1z += 0.0
 
         # Do the hankel transform on each component
-        em_x = ((C0x*rTE)@fhtfilt.j0 + (C1x*rTE)@fhtfilt.j1)/offsets
-        em_y = ((C0y*rTE)@fhtfilt.j0 + (C1y*rTE)@fhtfilt.j1)/offsets
-        em_z = ((C0z*rTE)@fhtfilt.j0 + (C1z*rTE)@fhtfilt.j1)/offsets
+        em_x = ((C0x*rTE)@filt_j0 + (C1x*rTE)@filt_j1)/offsets
+        em_y = ((C0y*rTE)@filt_j0 + (C1y*rTE)@filt_j1)/offsets
+        em_z = ((C0z*rTE)@filt_j0 + (C1z*rTE)@filt_j1)/offsets
 
         if field == "total":
             # add in the primary field
             r = np.linalg.norm(dxyz, axis=-1)
             mdotr = src_x*dxyz[:, 0] + src_y*dxyz[:, 1] + src_z*dxyz[:, 2]
 
             em_x += 3*dxyz[:, 0]*mdotr/r**5 - src_x/r**3
```

### Comparing `geoana-0.4.1/geoana/em/fdem/simple_functions.py` & `geoana-0.5.0/geoana/em/fdem/simple_functions.py`

 * *Files identical despite different names*

### Comparing `geoana-0.4.1/geoana/em/fdem/wholespace.py` & `geoana-0.5.0/geoana/em/fdem/wholespace.py`

 * *Files identical despite different names*

### Comparing `geoana-0.4.1/geoana/em/static/__init__.py` & `geoana-0.5.0/geoana/em/static/__init__.py`

 * *Files identical despite different names*

### Comparing `geoana-0.4.1/geoana/em/static/freespace.py` & `geoana-0.5.0/geoana/em/static/freespace.py`

 * *Files identical despite different names*

### Comparing `geoana-0.4.1/geoana/em/static/halfspace.py` & `geoana-0.5.0/geoana/em/static/halfspace.py`

 * *Files identical despite different names*

### Comparing `geoana-0.4.1/geoana/em/static/sphere.py` & `geoana-0.5.0/geoana/em/static/sphere.py`

 * *Files identical despite different names*

### Comparing `geoana-0.4.1/geoana/em/static/wholespace.py` & `geoana-0.5.0/geoana/em/static/wholespace.py`

 * *Files identical despite different names*

### Comparing `geoana-0.4.1/geoana/em/tdem/__init__.py` & `geoana-0.5.0/geoana/em/tdem/__init__.py`

 * *Files identical despite different names*

### Comparing `geoana-0.4.1/geoana/em/tdem/base.py` & `geoana-0.5.0/geoana/em/tdem/base.py`

 * *Files identical despite different names*

### Comparing `geoana-0.4.1/geoana/em/tdem/halfspace.py` & `geoana-0.5.0/geoana/em/tdem/halfspace.py`

 * *Files identical despite different names*

### Comparing `geoana-0.4.1/geoana/em/tdem/simple_functions.py` & `geoana-0.5.0/geoana/em/tdem/simple_functions.py`

 * *Files identical despite different names*

### Comparing `geoana-0.4.1/geoana/em/tdem/wholespace.py` & `geoana-0.5.0/geoana/em/tdem/wholespace.py`

 * *Files identical despite different names*

### Comparing `geoana-0.4.1/geoana/gravity.py` & `geoana-0.5.0/geoana/gravity.py`

 * *Files identical despite different names*

### Comparing `geoana-0.4.1/geoana/kernels/_extensions/_rTE.cpp` & `geoana-0.5.0/geoana/kernels/_extensions/_rTE.cpp`

 * *Files identical despite different names*

### Comparing `geoana-0.4.1/geoana/kernels/_extensions/_rTE.h` & `geoana-0.5.0/geoana/kernels/_extensions/_rTE.h`

 * *Files identical despite different names*

### Comparing `geoana-0.4.1/geoana/kernels/_extensions/potential_field_prism.c` & `geoana-0.5.0/geoana/kernels/_extensions/potential_field_prism.c`

 * *Files identical despite different names*

### Comparing `geoana-0.4.1/geoana/kernels/_extensions/rTE.cpp` & `geoana-0.5.0/geoana/kernels/_extensions/rTE.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -1136,195 +1136,177 @@
   char enc_type;
   char new_packmode;
   char enc_packmode;
   char is_valid_array;
 } __Pyx_BufFmt_Context;
 
 
-/* "../../../../../usr/share/miniconda/envs/geoana-test/lib/python3.8/site-packages/numpy/__init__.pxd":689
+/* "../../../../../usr/share/miniconda/envs/geoana-test/lib/python3.10/site-packages/numpy/__init__.pxd":688
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "../../../../../usr/share/miniconda/envs/geoana-test/lib/python3.8/site-packages/numpy/__init__.pxd":690
+/* "../../../../../usr/share/miniconda/envs/geoana-test/lib/python3.10/site-packages/numpy/__init__.pxd":689
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "../../../../../usr/share/miniconda/envs/geoana-test/lib/python3.8/site-packages/numpy/__init__.pxd":691
+/* "../../../../../usr/share/miniconda/envs/geoana-test/lib/python3.10/site-packages/numpy/__init__.pxd":690
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "../../../../../usr/share/miniconda/envs/geoana-test/lib/python3.8/site-packages/numpy/__init__.pxd":692
+/* "../../../../../usr/share/miniconda/envs/geoana-test/lib/python3.10/site-packages/numpy/__init__.pxd":691
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "../../../../../usr/share/miniconda/envs/geoana-test/lib/python3.8/site-packages/numpy/__init__.pxd":696
+/* "../../../../../usr/share/miniconda/envs/geoana-test/lib/python3.10/site-packages/numpy/__init__.pxd":695
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "../../../../../usr/share/miniconda/envs/geoana-test/lib/python3.8/site-packages/numpy/__init__.pxd":697
+/* "../../../../../usr/share/miniconda/envs/geoana-test/lib/python3.10/site-packages/numpy/__init__.pxd":696
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "../../../../../usr/share/miniconda/envs/geoana-test/lib/python3.8/site-packages/numpy/__init__.pxd":698
+/* "../../../../../usr/share/miniconda/envs/geoana-test/lib/python3.10/site-packages/numpy/__init__.pxd":697
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "../../../../../usr/share/miniconda/envs/geoana-test/lib/python3.8/site-packages/numpy/__init__.pxd":699
+/* "../../../../../usr/share/miniconda/envs/geoana-test/lib/python3.10/site-packages/numpy/__init__.pxd":698
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "../../../../../usr/share/miniconda/envs/geoana-test/lib/python3.8/site-packages/numpy/__init__.pxd":703
+/* "../../../../../usr/share/miniconda/envs/geoana-test/lib/python3.10/site-packages/numpy/__init__.pxd":702
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "../../../../../usr/share/miniconda/envs/geoana-test/lib/python3.8/site-packages/numpy/__init__.pxd":704
+/* "../../../../../usr/share/miniconda/envs/geoana-test/lib/python3.10/site-packages/numpy/__init__.pxd":703
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "../../../../../usr/share/miniconda/envs/geoana-test/lib/python3.8/site-packages/numpy/__init__.pxd":713
+/* "../../../../../usr/share/miniconda/envs/geoana-test/lib/python3.10/site-packages/numpy/__init__.pxd":712
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
- * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t
+ * 
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "../../../../../usr/share/miniconda/envs/geoana-test/lib/python3.8/site-packages/numpy/__init__.pxd":714
+/* "../../../../../usr/share/miniconda/envs/geoana-test/lib/python3.10/site-packages/numpy/__init__.pxd":713
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
- * ctypedef npy_longlong   long_t             # <<<<<<<<<<<<<<
- * ctypedef npy_longlong   longlong_t
- * 
- */
-typedef npy_longlong __pyx_t_5numpy_long_t;
-
-/* "../../../../../usr/share/miniconda/envs/geoana-test/lib/python3.8/site-packages/numpy/__init__.pxd":715
- * ctypedef npy_long       int_t
- * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "../../../../../usr/share/miniconda/envs/geoana-test/lib/python3.8/site-packages/numpy/__init__.pxd":717
+/* "../../../../../usr/share/miniconda/envs/geoana-test/lib/python3.10/site-packages/numpy/__init__.pxd":715
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
- * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t
+ * 
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "../../../../../usr/share/miniconda/envs/geoana-test/lib/python3.8/site-packages/numpy/__init__.pxd":718
+/* "../../../../../usr/share/miniconda/envs/geoana-test/lib/python3.10/site-packages/numpy/__init__.pxd":716
  * 
  * ctypedef npy_ulong      uint_t
- * ctypedef npy_ulonglong  ulong_t             # <<<<<<<<<<<<<<
- * ctypedef npy_ulonglong  ulonglong_t
- * 
- */
-typedef npy_ulonglong __pyx_t_5numpy_ulong_t;
-
-/* "../../../../../usr/share/miniconda/envs/geoana-test/lib/python3.8/site-packages/numpy/__init__.pxd":719
- * ctypedef npy_ulong      uint_t
- * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "../../../../../usr/share/miniconda/envs/geoana-test/lib/python3.8/site-packages/numpy/__init__.pxd":721
+/* "../../../../../usr/share/miniconda/envs/geoana-test/lib/python3.10/site-packages/numpy/__init__.pxd":718
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "../../../../../usr/share/miniconda/envs/geoana-test/lib/python3.8/site-packages/numpy/__init__.pxd":722
+/* "../../../../../usr/share/miniconda/envs/geoana-test/lib/python3.10/site-packages/numpy/__init__.pxd":719
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "../../../../../usr/share/miniconda/envs/geoana-test/lib/python3.8/site-packages/numpy/__init__.pxd":724
+/* "../../../../../usr/share/miniconda/envs/geoana-test/lib/python3.10/site-packages/numpy/__init__.pxd":721
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "../../../../../usr/share/miniconda/envs/geoana-test/lib/python3.8/site-packages/numpy/__init__.pxd":725
+/* "../../../../../usr/share/miniconda/envs/geoana-test/lib/python3.10/site-packages/numpy/__init__.pxd":722
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "../../../../../usr/share/miniconda/envs/geoana-test/lib/python3.8/site-packages/numpy/__init__.pxd":726
+/* "../../../../../usr/share/miniconda/envs/geoana-test/lib/python3.10/site-packages/numpy/__init__.pxd":723
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -1373,42 +1355,42 @@
 
 /*--- Type declarations ---*/
 struct __pyx_array_obj;
 struct __pyx_MemviewEnum_obj;
 struct __pyx_memoryview_obj;
 struct __pyx_memoryviewslice_obj;
 
-/* "../../../../../usr/share/miniconda/envs/geoana-test/lib/python3.8/site-packages/numpy/__init__.pxd":728
+/* "../../../../../usr/share/miniconda/envs/geoana-test/lib/python3.10/site-packages/numpy/__init__.pxd":725
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "../../../../../usr/share/miniconda/envs/geoana-test/lib/python3.8/site-packages/numpy/__init__.pxd":729
+/* "../../../../../usr/share/miniconda/envs/geoana-test/lib/python3.10/site-packages/numpy/__init__.pxd":726
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "../../../../../usr/share/miniconda/envs/geoana-test/lib/python3.8/site-packages/numpy/__init__.pxd":730
+/* "../../../../../usr/share/miniconda/envs/geoana-test/lib/python3.10/site-packages/numpy/__init__.pxd":727
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "../../../../../usr/share/miniconda/envs/geoana-test/lib/python3.8/site-packages/numpy/__init__.pxd":732
+/* "../../../../../usr/share/miniconda/envs/geoana-test/lib/python3.10/site-packages/numpy/__init__.pxd":729
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
@@ -1859,14 +1841,19 @@
 #define __pyx_get_slice_count_pointer(memview) (memview->acquisition_count_aligned_p)
 #define __pyx_get_slice_count(memview) (*__pyx_get_slice_count_pointer(memview))
 #define __PYX_INC_MEMVIEW(slice, have_gil) __Pyx_INC_MEMVIEW(slice, have_gil, __LINE__)
 #define __PYX_XDEC_MEMVIEW(slice, have_gil) __Pyx_XDEC_MEMVIEW(slice, have_gil, __LINE__)
 static CYTHON_INLINE void __Pyx_INC_MEMVIEW(__Pyx_memviewslice *, int, int);
 static CYTHON_INLINE void __Pyx_XDEC_MEMVIEW(__Pyx_memviewslice *, int, int);
 
+/* WriteUnraisableException.proto */
+static void __Pyx_WriteUnraisable(const char *name, int clineno,
+                                  int lineno, const char *filename,
+                                  int full_traceback, int nogil);
+
 /* GetTopmostException.proto */
 #if CYTHON_USE_EXC_INFO_STACK
 static _PyErr_StackItem * __Pyx_PyErr_GetTopmostException(PyThreadState *tstate);
 #endif
 
 /* SaveResetException.proto */
 #if CYTHON_FAST_THREAD_STATE
@@ -4978,15 +4965,15 @@
   __Pyx_XDECREF(__pyx_v_mu);
   __Pyx_XDECREF(__pyx_v_thicknesses);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../usr/share/miniconda/envs/geoana-test/lib/python3.8/site-packages/numpy/__init__.pxd":734
+/* "../../../../../usr/share/miniconda/envs/geoana-test/lib/python3.10/site-packages/numpy/__init__.pxd":731
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -4995,29 +4982,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 0);
 
-  /* "../../../../../usr/share/miniconda/envs/geoana-test/lib/python3.8/site-packages/numpy/__init__.pxd":735
+  /* "../../../../../usr/share/miniconda/envs/geoana-test/lib/python3.10/site-packages/numpy/__init__.pxd":732
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 735, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 732, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../usr/share/miniconda/envs/geoana-test/lib/python3.8/site-packages/numpy/__init__.pxd":734
+  /* "../../../../../usr/share/miniconda/envs/geoana-test/lib/python3.10/site-packages/numpy/__init__.pxd":731
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -5028,15 +5015,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../usr/share/miniconda/envs/geoana-test/lib/python3.8/site-packages/numpy/__init__.pxd":737
+/* "../../../../../usr/share/miniconda/envs/geoana-test/lib/python3.10/site-packages/numpy/__init__.pxd":734
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -5045,29 +5032,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 0);
 
-  /* "../../../../../usr/share/miniconda/envs/geoana-test/lib/python3.8/site-packages/numpy/__init__.pxd":738
+  /* "../../../../../usr/share/miniconda/envs/geoana-test/lib/python3.10/site-packages/numpy/__init__.pxd":735
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 738, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 735, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../usr/share/miniconda/envs/geoana-test/lib/python3.8/site-packages/numpy/__init__.pxd":737
+  /* "../../../../../usr/share/miniconda/envs/geoana-test/lib/python3.10/site-packages/numpy/__init__.pxd":734
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -5078,15 +5065,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../usr/share/miniconda/envs/geoana-test/lib/python3.8/site-packages/numpy/__init__.pxd":740
+/* "../../../../../usr/share/miniconda/envs/geoana-test/lib/python3.10/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -5095,29 +5082,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 0);
 
-  /* "../../../../../usr/share/miniconda/envs/geoana-test/lib/python3.8/site-packages/numpy/__init__.pxd":741
+  /* "../../../../../usr/share/miniconda/envs/geoana-test/lib/python3.10/site-packages/numpy/__init__.pxd":738
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 741, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 738, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../usr/share/miniconda/envs/geoana-test/lib/python3.8/site-packages/numpy/__init__.pxd":740
+  /* "../../../../../usr/share/miniconda/envs/geoana-test/lib/python3.10/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -5128,15 +5115,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../usr/share/miniconda/envs/geoana-test/lib/python3.8/site-packages/numpy/__init__.pxd":743
+/* "../../../../../usr/share/miniconda/envs/geoana-test/lib/python3.10/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -5145,29 +5132,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 0);
 
-  /* "../../../../../usr/share/miniconda/envs/geoana-test/lib/python3.8/site-packages/numpy/__init__.pxd":744
+  /* "../../../../../usr/share/miniconda/envs/geoana-test/lib/python3.10/site-packages/numpy/__init__.pxd":741
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 744, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 741, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../usr/share/miniconda/envs/geoana-test/lib/python3.8/site-packages/numpy/__init__.pxd":743
+  /* "../../../../../usr/share/miniconda/envs/geoana-test/lib/python3.10/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -5178,15 +5165,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../usr/share/miniconda/envs/geoana-test/lib/python3.8/site-packages/numpy/__init__.pxd":746
+/* "../../../../../usr/share/miniconda/envs/geoana-test/lib/python3.10/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -5195,29 +5182,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 0);
 
-  /* "../../../../../usr/share/miniconda/envs/geoana-test/lib/python3.8/site-packages/numpy/__init__.pxd":747
+  /* "../../../../../usr/share/miniconda/envs/geoana-test/lib/python3.10/site-packages/numpy/__init__.pxd":744
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 747, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 744, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../usr/share/miniconda/envs/geoana-test/lib/python3.8/site-packages/numpy/__init__.pxd":746
+  /* "../../../../../usr/share/miniconda/envs/geoana-test/lib/python3.10/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -5228,212 +5215,220 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../usr/share/miniconda/envs/geoana-test/lib/python3.8/site-packages/numpy/__init__.pxd":749
+/* "../../../../../usr/share/miniconda/envs/geoana-test/lib/python3.10/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 0);
 
-  /* "../../../../../usr/share/miniconda/envs/geoana-test/lib/python3.8/site-packages/numpy/__init__.pxd":750
+  /* "../../../../../usr/share/miniconda/envs/geoana-test/lib/python3.10/site-packages/numpy/__init__.pxd":747
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = (PyDataType_HASSUBARRAY(__pyx_v_d) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../../../usr/share/miniconda/envs/geoana-test/lib/python3.8/site-packages/numpy/__init__.pxd":751
+    /* "../../../../../usr/share/miniconda/envs/geoana-test/lib/python3.10/site-packages/numpy/__init__.pxd":748
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "../../../../../usr/share/miniconda/envs/geoana-test/lib/python3.8/site-packages/numpy/__init__.pxd":750
+    /* "../../../../../usr/share/miniconda/envs/geoana-test/lib/python3.10/site-packages/numpy/__init__.pxd":747
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "../../../../../usr/share/miniconda/envs/geoana-test/lib/python3.8/site-packages/numpy/__init__.pxd":753
+  /* "../../../../../usr/share/miniconda/envs/geoana-test/lib/python3.10/site-packages/numpy/__init__.pxd":750
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "../../../../../usr/share/miniconda/envs/geoana-test/lib/python3.8/site-packages/numpy/__init__.pxd":749
+  /* "../../../../../usr/share/miniconda/envs/geoana-test/lib/python3.10/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../usr/share/miniconda/envs/geoana-test/lib/python3.8/site-packages/numpy/__init__.pxd":928
+/* "../../../../../usr/share/miniconda/envs/geoana-test/lib/python3.10/site-packages/numpy/__init__.pxd":925
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
 static CYTHON_INLINE void __pyx_f_5numpy_set_array_base(PyArrayObject *__pyx_v_arr, PyObject *__pyx_v_base) {
   __Pyx_RefNannyDeclarations
+  int __pyx_t_1;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("set_array_base", 0);
 
-  /* "../../../../../usr/share/miniconda/envs/geoana-test/lib/python3.8/site-packages/numpy/__init__.pxd":929
+  /* "../../../../../usr/share/miniconda/envs/geoana-test/lib/python3.10/site-packages/numpy/__init__.pxd":926
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "../../../../../usr/share/miniconda/envs/geoana-test/lib/python3.8/site-packages/numpy/__init__.pxd":930
+  /* "../../../../../usr/share/miniconda/envs/geoana-test/lib/python3.10/site-packages/numpy/__init__.pxd":927
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
-  (void)(PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base));
+  __pyx_t_1 = PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base); if (unlikely(__pyx_t_1 == ((int)-1))) __PYX_ERR(1, 927, __pyx_L1_error)
 
-  /* "../../../../../usr/share/miniconda/envs/geoana-test/lib/python3.8/site-packages/numpy/__init__.pxd":928
+  /* "../../../../../usr/share/miniconda/envs/geoana-test/lib/python3.10/site-packages/numpy/__init__.pxd":925
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
   /* function exit code */
+  goto __pyx_L0;
+  __pyx_L1_error:;
+  __Pyx_WriteUnraisable("numpy.set_array_base", __pyx_clineno, __pyx_lineno, __pyx_filename, 1, 0);
+  __pyx_L0:;
   __Pyx_RefNannyFinishContext();
 }
 
-/* "../../../../../usr/share/miniconda/envs/geoana-test/lib/python3.8/site-packages/numpy/__init__.pxd":932
+/* "../../../../../usr/share/miniconda/envs/geoana-test/lib/python3.10/site-packages/numpy/__init__.pxd":929
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("get_array_base", 0);
 
-  /* "../../../../../usr/share/miniconda/envs/geoana-test/lib/python3.8/site-packages/numpy/__init__.pxd":933
+  /* "../../../../../usr/share/miniconda/envs/geoana-test/lib/python3.10/site-packages/numpy/__init__.pxd":930
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "../../../../../usr/share/miniconda/envs/geoana-test/lib/python3.8/site-packages/numpy/__init__.pxd":934
+  /* "../../../../../usr/share/miniconda/envs/geoana-test/lib/python3.10/site-packages/numpy/__init__.pxd":931
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = ((__pyx_v_base == NULL) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../../../usr/share/miniconda/envs/geoana-test/lib/python3.8/site-packages/numpy/__init__.pxd":935
+    /* "../../../../../usr/share/miniconda/envs/geoana-test/lib/python3.10/site-packages/numpy/__init__.pxd":932
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "../../../../../usr/share/miniconda/envs/geoana-test/lib/python3.8/site-packages/numpy/__init__.pxd":934
+    /* "../../../../../usr/share/miniconda/envs/geoana-test/lib/python3.10/site-packages/numpy/__init__.pxd":931
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "../../../../../usr/share/miniconda/envs/geoana-test/lib/python3.8/site-packages/numpy/__init__.pxd":936
+  /* "../../../../../usr/share/miniconda/envs/geoana-test/lib/python3.10/site-packages/numpy/__init__.pxd":933
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "../../../../../usr/share/miniconda/envs/geoana-test/lib/python3.8/site-packages/numpy/__init__.pxd":932
+  /* "../../../../../usr/share/miniconda/envs/geoana-test/lib/python3.10/site-packages/numpy/__init__.pxd":929
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../usr/share/miniconda/envs/geoana-test/lib/python3.8/site-packages/numpy/__init__.pxd":940
+/* "../../../../../usr/share/miniconda/envs/geoana-test/lib/python3.10/site-packages/numpy/__init__.pxd":937
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -5449,15 +5444,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 0);
 
-  /* "../../../../../usr/share/miniconda/envs/geoana-test/lib/python3.8/site-packages/numpy/__init__.pxd":941
+  /* "../../../../../usr/share/miniconda/envs/geoana-test/lib/python3.10/site-packages/numpy/__init__.pxd":938
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
   {
@@ -5465,84 +5460,84 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../usr/share/miniconda/envs/geoana-test/lib/python3.8/site-packages/numpy/__init__.pxd":942
+      /* "../../../../../usr/share/miniconda/envs/geoana-test/lib/python3.10/site-packages/numpy/__init__.pxd":939
  * cdef inline int import_array() except -1:
  *     try:
  *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
-      __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 942, __pyx_L3_error)
+      __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 939, __pyx_L3_error)
 
-      /* "../../../../../usr/share/miniconda/envs/geoana-test/lib/python3.8/site-packages/numpy/__init__.pxd":941
+      /* "../../../../../usr/share/miniconda/envs/geoana-test/lib/python3.10/site-packages/numpy/__init__.pxd":938
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../usr/share/miniconda/envs/geoana-test/lib/python3.8/site-packages/numpy/__init__.pxd":943
+    /* "../../../../../usr/share/miniconda/envs/geoana-test/lib/python3.10/site-packages/numpy/__init__.pxd":940
  *     try:
  *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 943, __pyx_L5_except_error)
+      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 940, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../usr/share/miniconda/envs/geoana-test/lib/python3.8/site-packages/numpy/__init__.pxd":944
+      /* "../../../../../usr/share/miniconda/envs/geoana-test/lib/python3.10/site-packages/numpy/__init__.pxd":941
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple_, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 944, __pyx_L5_except_error)
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple_, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 941, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __PYX_ERR(1, 944, __pyx_L5_except_error)
+      __PYX_ERR(1, 941, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../usr/share/miniconda/envs/geoana-test/lib/python3.8/site-packages/numpy/__init__.pxd":941
+    /* "../../../../../usr/share/miniconda/envs/geoana-test/lib/python3.10/site-packages/numpy/__init__.pxd":938
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../usr/share/miniconda/envs/geoana-test/lib/python3.8/site-packages/numpy/__init__.pxd":940
+  /* "../../../../../usr/share/miniconda/envs/geoana-test/lib/python3.10/site-packages/numpy/__init__.pxd":937
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -5557,15 +5552,15 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../usr/share/miniconda/envs/geoana-test/lib/python3.8/site-packages/numpy/__init__.pxd":946
+/* "../../../../../usr/share/miniconda/envs/geoana-test/lib/python3.10/site-packages/numpy/__init__.pxd":943
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -5581,15 +5576,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 0);
 
-  /* "../../../../../usr/share/miniconda/envs/geoana-test/lib/python3.8/site-packages/numpy/__init__.pxd":947
+  /* "../../../../../usr/share/miniconda/envs/geoana-test/lib/python3.10/site-packages/numpy/__init__.pxd":944
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -5597,84 +5592,84 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../usr/share/miniconda/envs/geoana-test/lib/python3.8/site-packages/numpy/__init__.pxd":948
+      /* "../../../../../usr/share/miniconda/envs/geoana-test/lib/python3.10/site-packages/numpy/__init__.pxd":945
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
-      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 948, __pyx_L3_error)
+      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 945, __pyx_L3_error)
 
-      /* "../../../../../usr/share/miniconda/envs/geoana-test/lib/python3.8/site-packages/numpy/__init__.pxd":947
+      /* "../../../../../usr/share/miniconda/envs/geoana-test/lib/python3.10/site-packages/numpy/__init__.pxd":944
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../usr/share/miniconda/envs/geoana-test/lib/python3.8/site-packages/numpy/__init__.pxd":949
+    /* "../../../../../usr/share/miniconda/envs/geoana-test/lib/python3.10/site-packages/numpy/__init__.pxd":946
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 949, __pyx_L5_except_error)
+      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 946, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../usr/share/miniconda/envs/geoana-test/lib/python3.8/site-packages/numpy/__init__.pxd":950
+      /* "../../../../../usr/share/miniconda/envs/geoana-test/lib/python3.10/site-packages/numpy/__init__.pxd":947
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 950, __pyx_L5_except_error)
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 947, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __PYX_ERR(1, 950, __pyx_L5_except_error)
+      __PYX_ERR(1, 947, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../usr/share/miniconda/envs/geoana-test/lib/python3.8/site-packages/numpy/__init__.pxd":947
+    /* "../../../../../usr/share/miniconda/envs/geoana-test/lib/python3.10/site-packages/numpy/__init__.pxd":944
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../usr/share/miniconda/envs/geoana-test/lib/python3.8/site-packages/numpy/__init__.pxd":946
+  /* "../../../../../usr/share/miniconda/envs/geoana-test/lib/python3.10/site-packages/numpy/__init__.pxd":943
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -5689,15 +5684,15 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../usr/share/miniconda/envs/geoana-test/lib/python3.8/site-packages/numpy/__init__.pxd":952
+/* "../../../../../usr/share/miniconda/envs/geoana-test/lib/python3.10/site-packages/numpy/__init__.pxd":949
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -5713,15 +5708,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 0);
 
-  /* "../../../../../usr/share/miniconda/envs/geoana-test/lib/python3.8/site-packages/numpy/__init__.pxd":953
+  /* "../../../../../usr/share/miniconda/envs/geoana-test/lib/python3.10/site-packages/numpy/__init__.pxd":950
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -5729,84 +5724,84 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../usr/share/miniconda/envs/geoana-test/lib/python3.8/site-packages/numpy/__init__.pxd":954
+      /* "../../../../../usr/share/miniconda/envs/geoana-test/lib/python3.10/site-packages/numpy/__init__.pxd":951
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
-      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 954, __pyx_L3_error)
+      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 951, __pyx_L3_error)
 
-      /* "../../../../../usr/share/miniconda/envs/geoana-test/lib/python3.8/site-packages/numpy/__init__.pxd":953
+      /* "../../../../../usr/share/miniconda/envs/geoana-test/lib/python3.10/site-packages/numpy/__init__.pxd":950
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../usr/share/miniconda/envs/geoana-test/lib/python3.8/site-packages/numpy/__init__.pxd":955
+    /* "../../../../../usr/share/miniconda/envs/geoana-test/lib/python3.10/site-packages/numpy/__init__.pxd":952
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 955, __pyx_L5_except_error)
+      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 952, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../usr/share/miniconda/envs/geoana-test/lib/python3.8/site-packages/numpy/__init__.pxd":956
+      /* "../../../../../usr/share/miniconda/envs/geoana-test/lib/python3.10/site-packages/numpy/__init__.pxd":953
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef extern from *:
  */
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 956, __pyx_L5_except_error)
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 953, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __PYX_ERR(1, 956, __pyx_L5_except_error)
+      __PYX_ERR(1, 953, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../usr/share/miniconda/envs/geoana-test/lib/python3.8/site-packages/numpy/__init__.pxd":953
+    /* "../../../../../usr/share/miniconda/envs/geoana-test/lib/python3.10/site-packages/numpy/__init__.pxd":950
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../usr/share/miniconda/envs/geoana-test/lib/python3.8/site-packages/numpy/__init__.pxd":952
+  /* "../../../../../usr/share/miniconda/envs/geoana-test/lib/python3.10/site-packages/numpy/__init__.pxd":949
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -5821,176 +5816,176 @@
   __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../usr/share/miniconda/envs/geoana-test/lib/python3.8/site-packages/numpy/__init__.pxd":966
+/* "../../../../../usr/share/miniconda/envs/geoana-test/lib/python3.10/site-packages/numpy/__init__.pxd":963
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_timedelta64_object", 0);
 
-  /* "../../../../../usr/share/miniconda/envs/geoana-test/lib/python3.8/site-packages/numpy/__init__.pxd":978
+  /* "../../../../../usr/share/miniconda/envs/geoana-test/lib/python3.10/site-packages/numpy/__init__.pxd":975
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../usr/share/miniconda/envs/geoana-test/lib/python3.8/site-packages/numpy/__init__.pxd":966
+  /* "../../../../../usr/share/miniconda/envs/geoana-test/lib/python3.10/site-packages/numpy/__init__.pxd":963
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../usr/share/miniconda/envs/geoana-test/lib/python3.8/site-packages/numpy/__init__.pxd":981
+/* "../../../../../usr/share/miniconda/envs/geoana-test/lib/python3.10/site-packages/numpy/__init__.pxd":978
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_datetime64_object", 0);
 
-  /* "../../../../../usr/share/miniconda/envs/geoana-test/lib/python3.8/site-packages/numpy/__init__.pxd":993
+  /* "../../../../../usr/share/miniconda/envs/geoana-test/lib/python3.10/site-packages/numpy/__init__.pxd":990
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../usr/share/miniconda/envs/geoana-test/lib/python3.8/site-packages/numpy/__init__.pxd":981
+  /* "../../../../../usr/share/miniconda/envs/geoana-test/lib/python3.10/site-packages/numpy/__init__.pxd":978
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../usr/share/miniconda/envs/geoana-test/lib/python3.8/site-packages/numpy/__init__.pxd":996
+/* "../../../../../usr/share/miniconda/envs/geoana-test/lib/python3.10/site-packages/numpy/__init__.pxd":993
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
 static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
   npy_datetime __pyx_r;
 
-  /* "../../../../../usr/share/miniconda/envs/geoana-test/lib/python3.8/site-packages/numpy/__init__.pxd":1003
+  /* "../../../../../usr/share/miniconda/envs/geoana-test/lib/python3.10/site-packages/numpy/__init__.pxd":1000
  *     also needed.  That can be found using `get_datetime64_unit`.
  *     """
  *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../usr/share/miniconda/envs/geoana-test/lib/python3.8/site-packages/numpy/__init__.pxd":996
+  /* "../../../../../usr/share/miniconda/envs/geoana-test/lib/python3.10/site-packages/numpy/__init__.pxd":993
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../usr/share/miniconda/envs/geoana-test/lib/python3.8/site-packages/numpy/__init__.pxd":1006
+/* "../../../../../usr/share/miniconda/envs/geoana-test/lib/python3.10/site-packages/numpy/__init__.pxd":1003
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
 static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
   npy_timedelta __pyx_r;
 
-  /* "../../../../../usr/share/miniconda/envs/geoana-test/lib/python3.8/site-packages/numpy/__init__.pxd":1010
+  /* "../../../../../usr/share/miniconda/envs/geoana-test/lib/python3.10/site-packages/numpy/__init__.pxd":1007
  *     returns the int64 value underlying scalar numpy timedelta64 object
  *     """
  *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../usr/share/miniconda/envs/geoana-test/lib/python3.8/site-packages/numpy/__init__.pxd":1006
+  /* "../../../../../usr/share/miniconda/envs/geoana-test/lib/python3.10/site-packages/numpy/__init__.pxd":1003
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../usr/share/miniconda/envs/geoana-test/lib/python3.8/site-packages/numpy/__init__.pxd":1013
+/* "../../../../../usr/share/miniconda/envs/geoana-test/lib/python3.10/site-packages/numpy/__init__.pxd":1010
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
 static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
   NPY_DATETIMEUNIT __pyx_r;
 
-  /* "../../../../../usr/share/miniconda/envs/geoana-test/lib/python3.8/site-packages/numpy/__init__.pxd":1017
+  /* "../../../../../usr/share/miniconda/envs/geoana-test/lib/python3.10/site-packages/numpy/__init__.pxd":1014
  *     returns the unit part of the dtype for a numpy datetime64 object.
  *     """
  *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
  */
   __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
   goto __pyx_L0;
 
-  /* "../../../../../usr/share/miniconda/envs/geoana-test/lib/python3.8/site-packages/numpy/__init__.pxd":1013
+  /* "../../../../../usr/share/miniconda/envs/geoana-test/lib/python3.10/site-packages/numpy/__init__.pxd":1010
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -19945,15 +19940,15 @@
   {&__pyx_kp_s_unable_to_allocate_shape_and_str, __pyx_k_unable_to_allocate_shape_and_str, sizeof(__pyx_k_unable_to_allocate_shape_and_str), 0, 0, 1, 0},
   {&__pyx_n_s_unpack, __pyx_k_unpack, sizeof(__pyx_k_unpack), 0, 0, 1, 1},
   {&__pyx_n_s_update, __pyx_k_update, sizeof(__pyx_k_update), 0, 0, 1, 1},
   {0, 0, 0, 0, 0, 0, 0}
 };
 static CYTHON_SMALL_CODE int __Pyx_InitCachedBuiltins(void) {
   __pyx_builtin_ValueError = __Pyx_GetBuiltinName(__pyx_n_s_ValueError); if (!__pyx_builtin_ValueError) __PYX_ERR(0, 77, __pyx_L1_error)
-  __pyx_builtin_ImportError = __Pyx_GetBuiltinName(__pyx_n_s_ImportError); if (!__pyx_builtin_ImportError) __PYX_ERR(1, 944, __pyx_L1_error)
+  __pyx_builtin_ImportError = __Pyx_GetBuiltinName(__pyx_n_s_ImportError); if (!__pyx_builtin_ImportError) __PYX_ERR(1, 941, __pyx_L1_error)
   __pyx_builtin_MemoryError = __Pyx_GetBuiltinName(__pyx_n_s_MemoryError); if (!__pyx_builtin_MemoryError) __PYX_ERR(2, 149, __pyx_L1_error)
   __pyx_builtin_enumerate = __Pyx_GetBuiltinName(__pyx_n_s_enumerate); if (!__pyx_builtin_enumerate) __PYX_ERR(2, 152, __pyx_L1_error)
   __pyx_builtin_range = __Pyx_GetBuiltinName(__pyx_n_s_range); if (!__pyx_builtin_range) __PYX_ERR(2, 181, __pyx_L1_error)
   __pyx_builtin_TypeError = __Pyx_GetBuiltinName(__pyx_n_s_TypeError); if (!__pyx_builtin_TypeError) __PYX_ERR(2, 2, __pyx_L1_error)
   __pyx_builtin_Ellipsis = __Pyx_GetBuiltinName(__pyx_n_s_Ellipsis); if (!__pyx_builtin_Ellipsis) __PYX_ERR(2, 406, __pyx_L1_error)
   __pyx_builtin_id = __Pyx_GetBuiltinName(__pyx_n_s_id); if (!__pyx_builtin_id) __PYX_ERR(2, 615, __pyx_L1_error)
   __pyx_builtin_IndexError = __Pyx_GetBuiltinName(__pyx_n_s_IndexError); if (!__pyx_builtin_IndexError) __PYX_ERR(2, 834, __pyx_L1_error)
@@ -19962,33 +19957,33 @@
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__Pyx_InitCachedConstants", 0);
 
-  /* "../../../../../usr/share/miniconda/envs/geoana-test/lib/python3.8/site-packages/numpy/__init__.pxd":944
+  /* "../../../../../usr/share/miniconda/envs/geoana-test/lib/python3.10/site-packages/numpy/__init__.pxd":941
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
-  __pyx_tuple_ = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple_)) __PYX_ERR(1, 944, __pyx_L1_error)
+  __pyx_tuple_ = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple_)) __PYX_ERR(1, 941, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple_);
   __Pyx_GIVEREF(__pyx_tuple_);
 
-  /* "../../../../../usr/share/miniconda/envs/geoana-test/lib/python3.8/site-packages/numpy/__init__.pxd":950
+  /* "../../../../../usr/share/miniconda/envs/geoana-test/lib/python3.10/site-packages/numpy/__init__.pxd":947
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
-  __pyx_tuple__2 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(1, 950, __pyx_L1_error)
+  __pyx_tuple__2 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(1, 947, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__2);
   __Pyx_GIVEREF(__pyx_tuple__2);
 
   /* "View.MemoryView":134
  * 
  *         if not self.ndim:
  *             raise ValueError("Empty shape tuple for cython.array")             # <<<<<<<<<<<<<<
@@ -20418,25 +20413,25 @@
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("numpy"); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 199, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_ptype_5numpy_dtype = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyArray_Descr),__Pyx_ImportType_CheckSize_Ignore_0_29_36); if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(1, 199, __pyx_L1_error)
   __pyx_ptype_5numpy_flatiter = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyArrayIterObject),__Pyx_ImportType_CheckSize_Ignore_0_29_36); if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(1, 222, __pyx_L1_error)
   __pyx_ptype_5numpy_broadcast = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyArrayMultiIterObject),__Pyx_ImportType_CheckSize_Ignore_0_29_36); if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(1, 226, __pyx_L1_error)
   __pyx_ptype_5numpy_ndarray = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyArrayObject),__Pyx_ImportType_CheckSize_Ignore_0_29_36); if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(1, 238, __pyx_L1_error)
-  __pyx_ptype_5numpy_generic = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_generic) __PYX_ERR(1, 770, __pyx_L1_error)
-  __pyx_ptype_5numpy_number = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "number", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_number) __PYX_ERR(1, 772, __pyx_L1_error)
-  __pyx_ptype_5numpy_integer = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_integer) __PYX_ERR(1, 774, __pyx_L1_error)
-  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_signedinteger) __PYX_ERR(1, 776, __pyx_L1_error)
-  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_unsignedinteger) __PYX_ERR(1, 778, __pyx_L1_error)
-  __pyx_ptype_5numpy_inexact = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_inexact) __PYX_ERR(1, 780, __pyx_L1_error)
-  __pyx_ptype_5numpy_floating = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_floating) __PYX_ERR(1, 782, __pyx_L1_error)
-  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_complexfloating) __PYX_ERR(1, 784, __pyx_L1_error)
-  __pyx_ptype_5numpy_flexible = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_flexible) __PYX_ERR(1, 786, __pyx_L1_error)
-  __pyx_ptype_5numpy_character = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "character", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_character) __PYX_ERR(1, 788, __pyx_L1_error)
-  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyUFuncObject),__Pyx_ImportType_CheckSize_Ignore_0_29_36); if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(1, 826, __pyx_L1_error)
+  __pyx_ptype_5numpy_generic = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_generic) __PYX_ERR(1, 767, __pyx_L1_error)
+  __pyx_ptype_5numpy_number = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "number", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_number) __PYX_ERR(1, 769, __pyx_L1_error)
+  __pyx_ptype_5numpy_integer = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_integer) __PYX_ERR(1, 771, __pyx_L1_error)
+  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_signedinteger) __PYX_ERR(1, 773, __pyx_L1_error)
+  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_unsignedinteger) __PYX_ERR(1, 775, __pyx_L1_error)
+  __pyx_ptype_5numpy_inexact = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_inexact) __PYX_ERR(1, 777, __pyx_L1_error)
+  __pyx_ptype_5numpy_floating = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_floating) __PYX_ERR(1, 779, __pyx_L1_error)
+  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_complexfloating) __PYX_ERR(1, 781, __pyx_L1_error)
+  __pyx_ptype_5numpy_flexible = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_flexible) __PYX_ERR(1, 783, __pyx_L1_error)
+  __pyx_ptype_5numpy_character = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "character", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_character) __PYX_ERR(1, 785, __pyx_L1_error)
+  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyUFuncObject),__Pyx_ImportType_CheckSize_Ignore_0_29_36); if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(1, 823, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
   return -1;
@@ -21972,14 +21967,54 @@
             PyGILState_Release(_gilstate);
         }
     } else {
         memslice->memview = NULL;
     }
 }
 
+/* WriteUnraisableException */
+static void __Pyx_WriteUnraisable(const char *name, CYTHON_UNUSED int clineno,
+                                  CYTHON_UNUSED int lineno, CYTHON_UNUSED const char *filename,
+                                  int full_traceback, CYTHON_UNUSED int nogil) {
+    PyObject *old_exc, *old_val, *old_tb;
+    PyObject *ctx;
+    __Pyx_PyThreadState_declare
+#ifdef WITH_THREAD
+    PyGILState_STATE state;
+    if (nogil)
+        state = PyGILState_Ensure();
+    else state = (PyGILState_STATE)0;
+#endif
+    __Pyx_PyThreadState_assign
+    __Pyx_ErrFetch(&old_exc, &old_val, &old_tb);
+    if (full_traceback) {
+        Py_XINCREF(old_exc);
+        Py_XINCREF(old_val);
+        Py_XINCREF(old_tb);
+        __Pyx_ErrRestore(old_exc, old_val, old_tb);
+        PyErr_PrintEx(1);
+    }
+    #if PY_MAJOR_VERSION < 3
+    ctx = PyString_FromString(name);
+    #else
+    ctx = PyUnicode_FromString(name);
+    #endif
+    __Pyx_ErrRestore(old_exc, old_val, old_tb);
+    if (!ctx) {
+        PyErr_WriteUnraisable(Py_None);
+    } else {
+        PyErr_WriteUnraisable(ctx);
+        Py_DECREF(ctx);
+    }
+#ifdef WITH_THREAD
+    if (nogil)
+        PyGILState_Release(state);
+#endif
+}
+
 /* GetTopmostException */
 #if CYTHON_USE_EXC_INFO_STACK
 static _PyErr_StackItem *
 __Pyx_PyErr_GetTopmostException(PyThreadState *tstate)
 {
     _PyErr_StackItem *exc_info = tstate->exc_info;
     while ((exc_info->exc_type == NULL || exc_info->exc_type == Py_None) &&
```

### Comparing `geoana-0.4.1/geoana/kernels/_extensions/rTE.pyx` & `geoana-0.5.0/geoana/kernels/_extensions/rTE.pyx`

 * *Files identical despite different names*

### Comparing `geoana-0.4.1/geoana/kernels/_extensions/setup.py` & `geoana-0.5.0/geoana/kernels/_extensions/setup.py`

 * *Files identical despite different names*

### Comparing `geoana-0.4.1/geoana/kernels/potential_field_prism.py` & `geoana-0.5.0/geoana/kernels/potential_field_prism.py`

 * *Files identical despite different names*

### Comparing `geoana-0.4.1/geoana/kernels/tranverse_electric_reflections.py` & `geoana-0.5.0/geoana/kernels/tranverse_electric_reflections.py`

 * *Files identical despite different names*

### Comparing `geoana-0.4.1/geoana/plotting_utils.py` & `geoana-0.5.0/geoana/plotting_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,19 +12,24 @@
 
   plot2Ddata
 
 """
 
 import numpy as np
 from scipy.interpolate import LinearNDInterpolator, NearestNDInterpolator
-import matplotlib.pyplot as plt
-from matplotlib import colors
-import warnings
+from .utils import requires
+try:
+    import matplotlib.pyplot as plt
+    from matplotlib import colors
+    matplotlib = True
+except ImportError:
+    matplotlib = False
 
 
+@requires({"matplotlib": matplotlib})
 def plot2Ddata(
     xyz,
     data,
     vec=False,
     nx=100,
     ny=100,
     ax=None,
```

### Comparing `geoana-0.4.1/geoana/shapes.py` & `geoana-0.5.0/geoana/shapes.py`

 * *Files identical despite different names*

### Comparing `geoana-0.4.1/geoana/spatial.py` & `geoana-0.5.0/geoana/spatial.py`

 * *Files identical despite different names*

### Comparing `geoana-0.4.1/geoana.egg-info/PKG-INFO` & `geoana-0.5.0/geoana.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geoana
-Version: 0.4.1
+Version: 0.5.0
 Summary: Analytic expressions for geophysical responses
 Home-page: https://www.simpeg.xyz
 Download-URL: https://github.com/simpeg/geoana
 Author: SimPEG developers
 Author-email: lindseyheagy@gmail.com
 License: MIT License
 Keywords: geophysics,electromagnetics
@@ -22,15 +22,15 @@
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS
 Classifier: Natural Language :: English
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 License-File: LICENSE
 
 | `getting_started`_ | `connecting`_ | `installing`_ | `license`_ | `documentation <https://geoana.simpeg.xyz/>`_ |
 
 geoana
 ======
```

### Comparing `geoana-0.4.1/geoana.egg-info/SOURCES.txt` & `geoana-0.5.0/geoana.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 LICENSE
-MANIFEST.in
 README.rst
 setup.py
 geoana/__init__.py
 geoana/gravity.py
 geoana/plotting_utils.py
 geoana/setup.py
 geoana/shapes.py
 geoana/spatial.py
 geoana/utils.py
+geoana/version.py
 geoana.egg-info/PKG-INFO
 geoana.egg-info/SOURCES.txt
 geoana.egg-info/dependency_links.txt
 geoana.egg-info/requires.txt
 geoana.egg-info/top_level.txt
+geoana/earthquake/README.md
 geoana/earthquake/__init__.py
 geoana/earthquake/oksar.py
 geoana/em/__init__.py
 geoana/em/base.py
 geoana/em/setup.py
 geoana/em/fdem/__init__.py
 geoana/em/fdem/base.py
@@ -41,25 +42,8 @@
 geoana/kernels/tranverse_electric_reflections.py
 geoana/kernels/_extensions/__init__.py
 geoana/kernels/_extensions/_rTE.cpp
 geoana/kernels/_extensions/_rTE.h
 geoana/kernels/_extensions/potential_field_prism.c
 geoana/kernels/_extensions/rTE.cpp
 geoana/kernels/_extensions/rTE.pyx
-geoana/kernels/_extensions/setup.py
-tests/test_docs.py
-tests/test_earthquake_oksar.py
-tests/test_em_fdem_base.py
-tests/test_em_fdem_electric_dipole.py
-tests/test_em_fdem_layered.py
-tests/test_em_fdem_magnetic_dipole.py
-tests/test_em_fdem_planewave.py
-tests/test_em_simple.py
-tests/test_em_static.py
-tests/test_em_tdem_base.py
-tests/test_em_tdem_halfspace.py
-tests/test_em_tdem_planewave.py
-tests/test_gravity.py
-tests/test_plotting_utils.py
-tests/test_potential_prism.py
-tests/test_spatial.py
-tests/test_utils.py
+geoana/kernels/_extensions/setup.py
```

### Comparing `geoana-0.4.1/setup.py` & `geoana-0.5.0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 #!/usr/bin/env python
 """
 geoana
 
 Interactive geoscience (mostly) analytic functions.
 """
 
-from distutils.core import setup
 import sys
+import os
+from setuptools import setup
 
 CLASSIFIERS = [
     'Development Status :: 4 - Beta',
     'Intended Audience :: Education',
     'Intended Audience :: Science/Research',
     'License :: OSI Approved :: MIT License',
     'Programming Language :: Python',
@@ -39,60 +40,56 @@
 
     return config
 
 with open('README.rst') as f:
     LONG_DESCRIPTION = ''.join(f.readlines())
 
 metadata = dict(
-    name = 'geoana',
-    version = '0.4.1',
-    python_requires=">=3.6",
+    name='geoana',
+    python_requires=">=3.8",
     setup_requires=[
-        "numpy>=1.8",
-        "cython>=0.2",
+        "numpy>=1.20",
+        "cython>=0.29",
+        "setuptools_scm",
     ],
     install_requires = [
-        'numpy>=1.8',
-        'scipy>=0.13',
-        'matplotlib',
-        'utm',
-        'empymod'
+        "numpy>=1.20",
+        "scipy>=1.8",
+        'libdlf',
     ],
     author = 'SimPEG developers',
     author_email = 'lindseyheagy@gmail.com',
     description = 'Analytic expressions for geophysical responses',
     long_description = LONG_DESCRIPTION,
     keywords = 'geophysics, electromagnetics',
     url = 'https://www.simpeg.xyz',
     download_url = 'https://github.com/simpeg/geoana',
     classifiers=CLASSIFIERS,
     platforms = ['Windows', 'Linux', 'Solaris', 'Mac OS-X', 'Unix'],
-    license='MIT License'
+    license='MIT License',
+    use_scm_version={
+        "write_to": os.path.join("geoana", "version.py"),
+    },
 )
 
 if len(sys.argv) >= 2 and (
     "--help" in sys.argv[1:]
-    or sys.argv[1] in ("--help-commands", "egg_info", "--version", "clean")
+    or sys.argv[1] in ("--help-commands", "egg_info", "install_egg_info", "--version", "clean")
 ):
     # For these actions, NumPy is not required.
     #
     # They are required to succeed without Numpy, for example when
-    # pip is used to install discretize when Numpy is not yet present in
+    # pip is used to install geoana when Numpy is not yet present in
     # the system.
-    try:
-        from setuptools import setup
-    except ImportError:
-        from distutils.core import setup
-else:
-    if (len(sys.argv) >= 2 and sys.argv[1] in ("bdist_wheel", "bdist_egg")) or (
-        "develop" in sys.argv
-    ):
-        # bdist_wheel/bdist_egg needs setuptools
-        import setuptools
 
+    setup_requires = metadata['setup_requires']
+    install_requires = metadata['install_requires']
+    install_requires = setup_requires + install_requires[1:]
+    metadata['install_requires'] = install_requires
+else:
     from numpy.distutils.core import setup
 
     # Add the configuration to the setup dict when building
     # after numpy is installed
     metadata["configuration"] = configuration
```

