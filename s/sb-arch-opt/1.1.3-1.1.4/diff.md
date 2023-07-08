# Comparing `tmp/sb-arch-opt-1.1.3.tar.gz` & `tmp/sb-arch-opt-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sb-arch-opt-1.1.3.tar", last modified: Wed Jun 21 19:06:36 2023, max compression
+gzip compressed data, was "sb-arch-opt-1.1.4.tar", last modified: Sat Jul  8 19:24:10 2023, max compression
```

## Comparing `sb-arch-opt-1.1.3.tar` & `sb-arch-opt-1.1.4.tar`

### file list

```diff
@@ -1,100 +1,101 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:06:36.973551 sb-arch-opt-1.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-06-21 19:06:25.000000 sb-arch-opt-1.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5369 2023-06-21 19:06:36.969551 sb-arch-opt-1.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4802 2023-06-21 19:06:25.000000 sb-arch-opt-1.1.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-21 19:06:25.000000 sb-arch-opt-1.1.3/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:06:36.961551 sb-arch-opt-1.1.3/sb_arch_opt/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-21 19:06:25.000000 sb-arch-opt-1.1.3/sb_arch_opt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:06:36.961551 sb-arch-opt-1.1.3/sb_arch_opt/algo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 19:06:25.000000 sb-arch-opt-1.1.3/sb_arch_opt/algo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:06:36.961551 sb-arch-opt-1.1.3/sb_arch_opt/algo/arch_sbo/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-21 19:06:25.000000 sb-arch-opt-1.1.3/sb_arch_opt/algo/arch_sbo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23630 2023-06-21 19:06:25.000000 sb-arch-opt-1.1.3/sb_arch_opt/algo/arch_sbo/algo.py
--rw-r--r--   0 runner    (1001) docker     (123)     4575 2023-06-21 19:06:25.000000 sb-arch-opt-1.1.3/sb_arch_opt/algo/arch_sbo/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    13383 2023-06-21 19:06:25.000000 sb-arch-opt-1.1.3/sb_arch_opt/algo/arch_sbo/hc_strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)    33800 2023-06-21 19:06:25.000000 sb-arch-opt-1.1.3/sb_arch_opt/algo/arch_sbo/infill.py
--rw-r--r--   0 runner    (1001) docker     (123)     4006 2023-06-21 19:06:25.000000 sb-arch-opt-1.1.3/sb_arch_opt/algo/arch_sbo/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    11777 2023-06-21 19:06:25.000000 sb-arch-opt-1.1.3/sb_arch_opt/algo/arch_sbo/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:06:36.961551 sb-arch-opt-1.1.3/sb_arch_opt/algo/botorch_interface/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-21 19:06:25.000000 sb-arch-opt-1.1.3/sb_arch_opt/algo/botorch_interface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7018 2023-06-21 19:06:25.000000 sb-arch-opt-1.1.3/sb_arch_opt/algo/botorch_interface/algo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-06-21 19:06:25.000000 sb-arch-opt-1.1.3/sb_arch_opt/algo/botorch_interface/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:06:36.965551 sb-arch-opt-1.1.3/sb_arch_opt/algo/hebo_interface/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-21 19:06:25.000000 sb-arch-opt-1.1.3/sb_arch_opt/algo/hebo_interface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5869 2023-06-21 19:06:25.000000 sb-arch-opt-1.1.3/sb_arch_opt/algo/hebo_interface/algo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-06-21 19:06:25.000000 sb-arch-opt-1.1.3/sb_arch_opt/algo/hebo_interface/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:06:36.965551 sb-arch-opt-1.1.3/sb_arch_opt/algo/pymoo_interface/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-21 19:06:25.000000 sb-arch-opt-1.1.3/sb_arch_opt/algo/pymoo_interface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4898 2023-06-21 19:06:25.000000 sb-arch-opt-1.1.3/sb_arch_opt/algo/pymoo_interface/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5482 2023-06-21 19:06:25.000000 sb-arch-opt-1.1.3/sb_arch_opt/algo/pymoo_interface/md_mating.py
--rw-r--r--   0 runner    (1001) docker     (123)     6591 2023-06-21 19:06:25.000000 sb-arch-opt-1.1.3/sb_arch_opt/algo/pymoo_interface/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     2911 2023-06-21 19:06:25.000000 sb-arch-opt-1.1.3/sb_arch_opt/algo/pymoo_interface/random_search.py
--rw-r--r--   0 runner    (1001) docker     (123)    13809 2023-06-21 19:06:25.000000 sb-arch-opt-1.1.3/sb_arch_opt/algo/pymoo_interface/storage_restart.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:06:36.965551 sb-arch-opt-1.1.3/sb_arch_opt/algo/segomoe_interface/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-21 19:06:25.000000 sb-arch-opt-1.1.3/sb_arch_opt/algo/segomoe_interface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14420 2023-06-21 19:06:25.000000 sb-arch-opt-1.1.3/sb_arch_opt/algo/segomoe_interface/algo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-06-21 19:06:25.000000 sb-arch-opt-1.1.3/sb_arch_opt/algo/segomoe_interface/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:06:36.965551 sb-arch-opt-1.1.3/sb_arch_opt/algo/smarty_interface/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-21 19:06:25.000000 sb-arch-opt-1.1.3/sb_arch_opt/algo/smarty_interface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4656 2023-06-21 19:06:25.000000 sb-arch-opt-1.1.3/sb_arch_opt/algo/smarty_interface/algo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-06-21 19:06:25.000000 sb-arch-opt-1.1.3/sb_arch_opt/algo/smarty_interface/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:06:36.965551 sb-arch-opt-1.1.3/sb_arch_opt/algo/tpe_interface/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-21 19:06:25.000000 sb-arch-opt-1.1.3/sb_arch_opt/algo/tpe_interface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8399 2023-06-21 19:06:25.000000 sb-arch-opt-1.1.3/sb_arch_opt/algo/tpe_interface/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:06:36.965551 sb-arch-opt-1.1.3/sb_arch_opt/algo/trieste_interface/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-21 19:06:25.000000 sb-arch-opt-1.1.3/sb_arch_opt/algo/trieste_interface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17309 2023-06-21 19:06:25.000000 sb-arch-opt-1.1.3/sb_arch_opt/algo/trieste_interface/algo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-06-21 19:06:25.000000 sb-arch-opt-1.1.3/sb_arch_opt/algo/trieste_interface/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    24815 2023-06-21 19:06:25.000000 sb-arch-opt-1.1.3/sb_arch_opt/design_space.py
--rw-r--r--   0 runner    (1001) docker     (123)    18656 2023-06-21 19:06:25.000000 sb-arch-opt-1.1.3/sb_arch_opt/design_space_explicit.py
--rw-r--r--   0 runner    (1001) docker     (123)     8637 2023-06-21 19:06:25.000000 sb-arch-opt-1.1.3/sb_arch_opt/pareto_front.py
--rw-r--r--   0 runner    (1001) docker     (123)    17347 2023-06-21 19:06:25.000000 sb-arch-opt-1.1.3/sb_arch_opt/problem.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:06:36.969551 sb-arch-opt-1.1.3/sb_arch_opt/problems/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 19:06:25.000000 sb-arch-opt-1.1.3/sb_arch_opt/problems/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19688 2023-06-21 19:06:25.000000 sb-arch-opt-1.1.3/sb_arch_opt/problems/assignment.py
--rw-r--r--   0 runner    (1001) docker     (123)     6013 2023-06-21 19:06:25.000000 sb-arch-opt-1.1.3/sb_arch_opt/problems/constrained.py
--rw-r--r--   0 runner    (1001) docker     (123)     3348 2023-06-21 19:06:25.000000 sb-arch-opt-1.1.3/sb_arch_opt/problems/continuous.py
--rw-r--r--   0 runner    (1001) docker     (123)     9871 2023-06-21 19:06:25.000000 sb-arch-opt-1.1.3/sb_arch_opt/problems/discrete.py
--rw-r--r--   0 runner    (1001) docker     (123)    20006 2023-06-21 19:06:25.000000 sb-arch-opt-1.1.3/sb_arch_opt/problems/gnc.py
--rw-r--r--   0 runner    (1001) docker     (123)    21192 2023-06-21 19:06:25.000000 sb-arch-opt-1.1.3/sb_arch_opt/problems/hidden_constraints.py
--rw-r--r--   0 runner    (1001) docker     (123)    48482 2023-06-21 19:06:25.000000 sb-arch-opt-1.1.3/sb_arch_opt/problems/hierarchical.py
--rw-r--r--   0 runner    (1001) docker     (123)     6022 2023-06-21 19:06:25.000000 sb-arch-opt-1.1.3/sb_arch_opt/problems/md_mo.py
--rw-r--r--   0 runner    (1001) docker     (123)     8556 2023-06-21 19:06:25.000000 sb-arch-opt-1.1.3/sb_arch_opt/problems/problems_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    17572 2023-06-21 19:06:25.000000 sb-arch-opt-1.1.3/sb_arch_opt/problems/turbofan_arch.py
--rw-r--r--   0 runner    (1001) docker     (123)    22864 2023-06-21 19:06:25.000000 sb-arch-opt-1.1.3/sb_arch_opt/sampling.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:06:36.969551 sb-arch-opt-1.1.3/sb_arch_opt/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 19:06:25.000000 sb-arch-opt-1.1.3/sb_arch_opt/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:06:36.969551 sb-arch-opt-1.1.3/sb_arch_opt/tests/algo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 19:06:25.000000 sb-arch-opt-1.1.3/sb_arch_opt/tests/algo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9346 2023-06-21 19:06:25.000000 sb-arch-opt-1.1.3/sb_arch_opt/tests/algo/test_arch_sbo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-06-21 19:06:25.000000 sb-arch-opt-1.1.3/sb_arch_opt/tests/algo/test_botorch.py
--rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-06-21 19:06:25.000000 sb-arch-opt-1.1.3/sb_arch_opt/tests/algo/test_hebo.py
--rw-r--r--   0 runner    (1001) docker     (123)     9632 2023-06-21 19:06:25.000000 sb-arch-opt-1.1.3/sb_arch_opt/tests/algo/test_pymoo.py
--rw-r--r--   0 runner    (1001) docker     (123)     6421 2023-06-21 19:06:25.000000 sb-arch-opt-1.1.3/sb_arch_opt/tests/algo/test_segomoe.py
--rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-06-21 19:06:25.000000 sb-arch-opt-1.1.3/sb_arch_opt/tests/algo/test_smarty.py
--rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-06-21 19:06:25.000000 sb-arch-opt-1.1.3/sb_arch_opt/tests/algo/test_tpe.py
--rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-06-21 19:06:25.000000 sb-arch-opt-1.1.3/sb_arch_opt/tests/algo/test_trieste.py
--rw-r--r--   0 runner    (1001) docker     (123)     3840 2023-06-21 19:06:25.000000 sb-arch-opt-1.1.3/sb_arch_opt/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:06:36.969551 sb-arch-opt-1.1.3/sb_arch_opt/tests/problems/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 19:06:25.000000 sb-arch-opt-1.1.3/sb_arch_opt/tests/problems/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-06-21 19:06:25.000000 sb-arch-opt-1.1.3/sb_arch_opt/tests/problems/test_assignment.py
--rw-r--r--   0 runner    (1001) docker     (123)      736 2023-06-21 19:06:25.000000 sb-arch-opt-1.1.3/sb_arch_opt/tests/problems/test_constrained.py
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-06-21 19:06:25.000000 sb-arch-opt-1.1.3/sb_arch_opt/tests/problems/test_continuous.py
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-06-21 19:06:25.000000 sb-arch-opt-1.1.3/sb_arch_opt/tests/problems/test_discrete.py
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-06-21 19:06:25.000000 sb-arch-opt-1.1.3/sb_arch_opt/tests/problems/test_gnc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-06-21 19:06:25.000000 sb-arch-opt-1.1.3/sb_arch_opt/tests/problems/test_hidden_constraints.py
--rw-r--r--   0 runner    (1001) docker     (123)     3373 2023-06-21 19:06:25.000000 sb-arch-opt-1.1.3/sb_arch_opt/tests/problems/test_hierarchical.py
--rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-06-21 19:06:25.000000 sb-arch-opt-1.1.3/sb_arch_opt/tests/problems/test_md_mo.py
--rw-r--r--   0 runner    (1001) docker     (123)     3901 2023-06-21 19:06:25.000000 sb-arch-opt-1.1.3/sb_arch_opt/tests/problems/test_turbofan_arch.py
--rw-r--r--   0 runner    (1001) docker     (123)     4939 2023-06-21 19:06:25.000000 sb-arch-opt-1.1.3/sb_arch_opt/tests/test_design_space.py
--rw-r--r--   0 runner    (1001) docker     (123)    12538 2023-06-21 19:06:25.000000 sb-arch-opt-1.1.3/sb_arch_opt/tests/test_design_space_explicit.py
--rw-r--r--   0 runner    (1001) docker     (123)    15326 2023-06-21 19:06:25.000000 sb-arch-opt-1.1.3/sb_arch_opt/tests/test_problem.py
--rw-r--r--   0 runner    (1001) docker     (123)      962 2023-06-21 19:06:25.000000 sb-arch-opt-1.1.3/sb_arch_opt/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:06:36.961551 sb-arch-opt-1.1.3/sb_arch_opt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5369 2023-06-21 19:06:36.000000 sb-arch-opt-1.1.3/sb_arch_opt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3047 2023-06-21 19:06:36.000000 sb-arch-opt-1.1.3/sb_arch_opt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 19:06:36.000000 sb-arch-opt-1.1.3/sb_arch_opt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-06-21 19:06:36.000000 sb-arch-opt-1.1.3/sb_arch_opt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-21 19:06:36.000000 sb-arch-opt-1.1.3/sb_arch_opt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 19:06:36.973551 sb-arch-opt-1.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3670 2023-06-21 19:06:25.000000 sb-arch-opt-1.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 19:24:10.226050 sb-arch-opt-1.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-07-08 19:23:58.000000 sb-arch-opt-1.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4530 2023-07-08 19:24:10.226050 sb-arch-opt-1.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3963 2023-07-08 19:23:58.000000 sb-arch-opt-1.1.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-08 19:23:58.000000 sb-arch-opt-1.1.4/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 19:24:10.214050 sb-arch-opt-1.1.4/sb_arch_opt/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-08 19:23:58.000000 sb-arch-opt-1.1.4/sb_arch_opt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 19:24:10.218050 sb-arch-opt-1.1.4/sb_arch_opt/algo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 19:23:58.000000 sb-arch-opt-1.1.4/sb_arch_opt/algo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 19:24:10.218050 sb-arch-opt-1.1.4/sb_arch_opt/algo/arch_sbo/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-08 19:23:58.000000 sb-arch-opt-1.1.4/sb_arch_opt/algo/arch_sbo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23630 2023-07-08 19:23:58.000000 sb-arch-opt-1.1.4/sb_arch_opt/algo/arch_sbo/algo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4642 2023-07-08 19:23:58.000000 sb-arch-opt-1.1.4/sb_arch_opt/algo/arch_sbo/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13383 2023-07-08 19:23:58.000000 sb-arch-opt-1.1.4/sb_arch_opt/algo/arch_sbo/hc_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33800 2023-07-08 19:23:58.000000 sb-arch-opt-1.1.4/sb_arch_opt/algo/arch_sbo/infill.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4006 2023-07-08 19:23:58.000000 sb-arch-opt-1.1.4/sb_arch_opt/algo/arch_sbo/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12520 2023-07-08 19:23:58.000000 sb-arch-opt-1.1.4/sb_arch_opt/algo/arch_sbo/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 19:24:10.218050 sb-arch-opt-1.1.4/sb_arch_opt/algo/botorch_interface/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-08 19:23:58.000000 sb-arch-opt-1.1.4/sb_arch_opt/algo/botorch_interface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7018 2023-07-08 19:23:58.000000 sb-arch-opt-1.1.4/sb_arch_opt/algo/botorch_interface/algo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-07-08 19:23:58.000000 sb-arch-opt-1.1.4/sb_arch_opt/algo/botorch_interface/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 19:24:10.218050 sb-arch-opt-1.1.4/sb_arch_opt/algo/hebo_interface/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-08 19:23:58.000000 sb-arch-opt-1.1.4/sb_arch_opt/algo/hebo_interface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5869 2023-07-08 19:23:58.000000 sb-arch-opt-1.1.4/sb_arch_opt/algo/hebo_interface/algo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-07-08 19:23:58.000000 sb-arch-opt-1.1.4/sb_arch_opt/algo/hebo_interface/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 19:24:10.218050 sb-arch-opt-1.1.4/sb_arch_opt/algo/pymoo_interface/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-08 19:23:58.000000 sb-arch-opt-1.1.4/sb_arch_opt/algo/pymoo_interface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4898 2023-07-08 19:23:58.000000 sb-arch-opt-1.1.4/sb_arch_opt/algo/pymoo_interface/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5482 2023-07-08 19:23:58.000000 sb-arch-opt-1.1.4/sb_arch_opt/algo/pymoo_interface/md_mating.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6591 2023-07-08 19:23:58.000000 sb-arch-opt-1.1.4/sb_arch_opt/algo/pymoo_interface/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2911 2023-07-08 19:23:58.000000 sb-arch-opt-1.1.4/sb_arch_opt/algo/pymoo_interface/random_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13611 2023-07-08 19:23:58.000000 sb-arch-opt-1.1.4/sb_arch_opt/algo/pymoo_interface/storage_restart.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 19:24:10.218050 sb-arch-opt-1.1.4/sb_arch_opt/algo/segomoe_interface/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-08 19:23:58.000000 sb-arch-opt-1.1.4/sb_arch_opt/algo/segomoe_interface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14420 2023-07-08 19:23:58.000000 sb-arch-opt-1.1.4/sb_arch_opt/algo/segomoe_interface/algo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-07-08 19:23:58.000000 sb-arch-opt-1.1.4/sb_arch_opt/algo/segomoe_interface/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 19:24:10.222050 sb-arch-opt-1.1.4/sb_arch_opt/algo/smarty_interface/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-08 19:23:58.000000 sb-arch-opt-1.1.4/sb_arch_opt/algo/smarty_interface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4656 2023-07-08 19:23:58.000000 sb-arch-opt-1.1.4/sb_arch_opt/algo/smarty_interface/algo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-07-08 19:23:58.000000 sb-arch-opt-1.1.4/sb_arch_opt/algo/smarty_interface/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 19:24:10.222050 sb-arch-opt-1.1.4/sb_arch_opt/algo/tpe_interface/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-08 19:23:58.000000 sb-arch-opt-1.1.4/sb_arch_opt/algo/tpe_interface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8399 2023-07-08 19:23:58.000000 sb-arch-opt-1.1.4/sb_arch_opt/algo/tpe_interface/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 19:24:10.222050 sb-arch-opt-1.1.4/sb_arch_opt/algo/trieste_interface/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-08 19:23:58.000000 sb-arch-opt-1.1.4/sb_arch_opt/algo/trieste_interface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17309 2023-07-08 19:23:58.000000 sb-arch-opt-1.1.4/sb_arch_opt/algo/trieste_interface/algo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-07-08 19:23:58.000000 sb-arch-opt-1.1.4/sb_arch_opt/algo/trieste_interface/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24809 2023-07-08 19:23:58.000000 sb-arch-opt-1.1.4/sb_arch_opt/design_space.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18656 2023-07-08 19:23:58.000000 sb-arch-opt-1.1.4/sb_arch_opt/design_space_explicit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8637 2023-07-08 19:23:58.000000 sb-arch-opt-1.1.4/sb_arch_opt/pareto_front.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17454 2023-07-08 19:23:58.000000 sb-arch-opt-1.1.4/sb_arch_opt/problem.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 19:24:10.222050 sb-arch-opt-1.1.4/sb_arch_opt/problems/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 19:23:58.000000 sb-arch-opt-1.1.4/sb_arch_opt/problems/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19688 2023-07-08 19:23:58.000000 sb-arch-opt-1.1.4/sb_arch_opt/problems/assignment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6013 2023-07-08 19:23:58.000000 sb-arch-opt-1.1.4/sb_arch_opt/problems/constrained.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3348 2023-07-08 19:23:58.000000 sb-arch-opt-1.1.4/sb_arch_opt/problems/continuous.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9871 2023-07-08 19:23:58.000000 sb-arch-opt-1.1.4/sb_arch_opt/problems/discrete.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20006 2023-07-08 19:23:58.000000 sb-arch-opt-1.1.4/sb_arch_opt/problems/gnc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21192 2023-07-08 19:23:58.000000 sb-arch-opt-1.1.4/sb_arch_opt/problems/hidden_constraints.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48482 2023-07-08 19:23:58.000000 sb-arch-opt-1.1.4/sb_arch_opt/problems/hierarchical.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6022 2023-07-08 19:23:58.000000 sb-arch-opt-1.1.4/sb_arch_opt/problems/md_mo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8556 2023-07-08 19:23:58.000000 sb-arch-opt-1.1.4/sb_arch_opt/problems/problems_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17572 2023-07-08 19:23:58.000000 sb-arch-opt-1.1.4/sb_arch_opt/problems/turbofan_arch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23052 2023-07-08 19:23:58.000000 sb-arch-opt-1.1.4/sb_arch_opt/sampling.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 19:24:10.222050 sb-arch-opt-1.1.4/sb_arch_opt/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 19:23:58.000000 sb-arch-opt-1.1.4/sb_arch_opt/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 19:24:10.226050 sb-arch-opt-1.1.4/sb_arch_opt/tests/algo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 19:23:58.000000 sb-arch-opt-1.1.4/sb_arch_opt/tests/algo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13571 2023-07-08 19:23:58.000000 sb-arch-opt-1.1.4/sb_arch_opt/tests/algo/test_arch_sbo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-07-08 19:23:58.000000 sb-arch-opt-1.1.4/sb_arch_opt/tests/algo/test_botorch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-07-08 19:23:58.000000 sb-arch-opt-1.1.4/sb_arch_opt/tests/algo/test_hebo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9632 2023-07-08 19:23:58.000000 sb-arch-opt-1.1.4/sb_arch_opt/tests/algo/test_pymoo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6421 2023-07-08 19:23:58.000000 sb-arch-opt-1.1.4/sb_arch_opt/tests/algo/test_segomoe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-07-08 19:23:58.000000 sb-arch-opt-1.1.4/sb_arch_opt/tests/algo/test_smarty.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-07-08 19:23:58.000000 sb-arch-opt-1.1.4/sb_arch_opt/tests/algo/test_tpe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-07-08 19:23:58.000000 sb-arch-opt-1.1.4/sb_arch_opt/tests/algo/test_trieste.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3840 2023-07-08 19:23:58.000000 sb-arch-opt-1.1.4/sb_arch_opt/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 19:24:10.226050 sb-arch-opt-1.1.4/sb_arch_opt/tests/problems/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 19:23:58.000000 sb-arch-opt-1.1.4/sb_arch_opt/tests/problems/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-07-08 19:23:58.000000 sb-arch-opt-1.1.4/sb_arch_opt/tests/problems/test_assignment.py
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-07-08 19:23:58.000000 sb-arch-opt-1.1.4/sb_arch_opt/tests/problems/test_constrained.py
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-07-08 19:23:58.000000 sb-arch-opt-1.1.4/sb_arch_opt/tests/problems/test_continuous.py
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-07-08 19:23:58.000000 sb-arch-opt-1.1.4/sb_arch_opt/tests/problems/test_discrete.py
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-07-08 19:23:58.000000 sb-arch-opt-1.1.4/sb_arch_opt/tests/problems/test_gnc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-07-08 19:23:58.000000 sb-arch-opt-1.1.4/sb_arch_opt/tests/problems/test_hidden_constraints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3716 2023-07-08 19:23:58.000000 sb-arch-opt-1.1.4/sb_arch_opt/tests/problems/test_hierarchical.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-07-08 19:23:58.000000 sb-arch-opt-1.1.4/sb_arch_opt/tests/problems/test_md_mo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3978 2023-07-08 19:23:58.000000 sb-arch-opt-1.1.4/sb_arch_opt/tests/problems/test_turbofan_arch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4939 2023-07-08 19:23:58.000000 sb-arch-opt-1.1.4/sb_arch_opt/tests/test_design_space.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12538 2023-07-08 19:23:58.000000 sb-arch-opt-1.1.4/sb_arch_opt/tests/test_design_space_explicit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15326 2023-07-08 19:23:58.000000 sb-arch-opt-1.1.4/sb_arch_opt/tests/test_problem.py
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-07-08 19:23:58.000000 sb-arch-opt-1.1.4/sb_arch_opt/tests/test_tutorials.py
+-rw-r--r--   0 runner    (1001) docker     (123)      962 2023-07-08 19:23:58.000000 sb-arch-opt-1.1.4/sb_arch_opt/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 19:24:10.218050 sb-arch-opt-1.1.4/sb_arch_opt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4530 2023-07-08 19:24:10.000000 sb-arch-opt-1.1.4/sb_arch_opt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3083 2023-07-08 19:24:10.000000 sb-arch-opt-1.1.4/sb_arch_opt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 19:24:10.000000 sb-arch-opt-1.1.4/sb_arch_opt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-07-08 19:24:10.000000 sb-arch-opt-1.1.4/sb_arch_opt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-08 19:24:10.000000 sb-arch-opt-1.1.4/sb_arch_opt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 19:24:10.226050 sb-arch-opt-1.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3693 2023-07-08 19:23:58.000000 sb-arch-opt-1.1.4/setup.py
```

### Comparing `sb-arch-opt-1.1.3/LICENSE` & `sb-arch-opt-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `sb-arch-opt-1.1.3/sb_arch_opt/algo/arch_sbo/algo.py` & `sb-arch-opt-1.1.4/sb_arch_opt/algo/arch_sbo/algo.py`

 * *Files identical despite different names*

### Comparing `sb-arch-opt-1.1.3/sb_arch_opt/algo/arch_sbo/api.py` & `sb-arch-opt-1.1.4/sb_arch_opt/algo/arch_sbo/api.py`

 * *Files 7% similar despite different names*

```diff
@@ -32,26 +32,27 @@
 if not HAS_ARCH_SBO:
     get_sbo_termination = lambda *_, **__: None
 
 
 __all__ = ['get_arch_sbo_rbf', 'get_arch_sbo_gp', 'HAS_ARCH_SBO', 'get_sbo_termination', 'get_sbo']
 
 
-def get_arch_sbo_rbf(init_size: int = 100, results_folder=None, **kwargs):
+def get_arch_sbo_rbf(init_size: int = 100, results_folder=None, **kwargs) -> InfillAlgorithm:
     """
     Get a architecture SBO algorithm using an RBF model as its surrogate model.
     """
     model = ModelFactory.get_rbf_model()
     hc_strategy = get_hc_strategy()
     return get_sbo(model, FunctionEstimateInfill(), init_size=init_size, results_folder=results_folder,
                    hc_strategy=hc_strategy, **kwargs)
 
 
 def get_arch_sbo_gp(problem: ArchOptProblemBase, init_size: int = 100, n_parallel=None, min_pof: float = None,
-                    kpls_n_dim: int = 10, g_aggregation: ConstraintAggregation = None, results_folder=None, **kwargs):
+                    kpls_n_dim: int = 10, g_aggregation: ConstraintAggregation = None, results_folder=None, **kwargs) \
+        -> InfillAlgorithm:
     """
     Get an architecture SBO algorithm using a mixed-discrete Gaussian Process (Kriging) model as its surrogate model.
     Appropriate (multi-objective) infills and constraint handling techniques are automatically selected.
 
     For constraint handling, increase min_pof to between 0.50 and 0.75 to be more conservative (i.e. require a higher
     probability of being feasible for infill points) or decrease below 0.50 to be more exploratory. Optionally defined
     an aggregation strategy to reduce the number of models to train.
@@ -73,15 +74,15 @@
 
     return get_sbo(model, infill, infill_size=infill_batch, init_size=init_size, normalization=normalization,
                    results_folder=results_folder, hc_strategy=hc_strategy, **kwargs)
 
 
 def get_sbo(surrogate_model, infill: 'SurrogateInfill', infill_size: int = 1, init_size: int = 100,
             infill_pop_size: int = 100, infill_gens: int = 100, repair=None, normalization=None,
-            hc_strategy: 'HiddenConstraintStrategy' = None, results_folder=None, **kwargs):
+            hc_strategy: 'HiddenConstraintStrategy' = None, results_folder=None, **kwargs) -> InfillAlgorithm:
     """Create the SBO algorithm given some SMT surrogate model and an infill criterion"""
 
     sbo = SBOInfill(surrogate_model, infill, pop_size=infill_pop_size, termination=infill_gens, repair=repair,
                     normalization=normalization, hc_strategy=hc_strategy, verbose=True)\
         .algorithm(infill_size=infill_size, init_size=init_size, **kwargs)
 
     if results_folder is not None:
```

### Comparing `sb-arch-opt-1.1.3/sb_arch_opt/algo/arch_sbo/hc_strategy.py` & `sb-arch-opt-1.1.4/sb_arch_opt/algo/arch_sbo/hc_strategy.py`

 * *Files identical despite different names*

### Comparing `sb-arch-opt-1.1.3/sb_arch_opt/algo/arch_sbo/infill.py` & `sb-arch-opt-1.1.4/sb_arch_opt/algo/arch_sbo/infill.py`

 * *Files identical despite different names*

### Comparing `sb-arch-opt-1.1.3/sb_arch_opt/algo/arch_sbo/metrics.py` & `sb-arch-opt-1.1.4/sb_arch_opt/algo/arch_sbo/metrics.py`

 * *Files identical despite different names*

### Comparing `sb-arch-opt-1.1.3/sb_arch_opt/algo/arch_sbo/models.py` & `sb-arch-opt-1.1.4/sb_arch_opt/algo/arch_sbo/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,34 +18,35 @@
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 """
+import os
 import copy
 import numpy as np
 from typing import *
 from dataclasses import dataclass
 import pymoo.core.variable as var
 from pymoo.core.problem import Problem
 from sb_arch_opt.problem import ArchOptProblemBase
 from sb_arch_opt.design_space import ArchDesignSpace
 from sb_arch_opt.sampling import HierarchicalSampling
 from pymoo.util.normalization import Normalization, SimpleZeroToOneNormalization
 
 try:
+    os.environ['USE_NUMBA_JIT'] = '1'
     from smt.surrogate_models.rbf import RBF
     from smt.surrogate_models.surrogate_model import SurrogateModel
 
     from smt.surrogate_models.krg import KRG, KrgBased
     from smt.surrogate_models.kpls import KPLS
     from smt.surrogate_models.krg_based import MixIntKernelType, MixHrcKernelType
 
-    from smt.applications.mixed_integer import MixedIntegerKrigingModel
     from smt.utils.design_space import BaseDesignSpace
     import smt.utils.design_space as ds
 
     HAS_ARCH_SBO = True
 except ImportError:
     HAS_ARCH_SBO = False
 
@@ -115,18 +116,18 @@
 
     def get_smt_design_space_spec(self) -> SMTDesignSpaceSpec:
         """Get information about the design space as needed by SMT and SEGOMOE"""
         check_dependencies()
         return self.create_smt_design_space_spec(self.problem.design_space)
 
     @staticmethod
-    def create_smt_design_space_spec(arch_design_space: ArchDesignSpace, md_normalize=False):
+    def create_smt_design_space_spec(arch_design_space: ArchDesignSpace, md_normalize=False, cont_relax=False):
         check_dependencies()
 
-        design_space = SBArchOptDesignSpace(arch_design_space, md_normalize=md_normalize)
+        design_space = SBArchOptDesignSpace(arch_design_space, md_normalize=md_normalize, cont_relax=cont_relax)
         is_mixed_discrete = not np.all(arch_design_space.is_cont_mask)
 
         var_defs = [{'name': f'x{i}', 'lb': bounds[0], 'ub': bounds[1]}
                     for i, bounds in enumerate(design_space.get_num_bounds())]
 
         return SMTDesignSpaceSpec(
             var_defs=var_defs,
@@ -155,76 +156,91 @@
         else:
             surrogate = KRG(print_global=False, **kwargs)
 
         if multi:
             surrogate = MultiSurrogateModel(surrogate)
         return surrogate
 
-    def get_md_kriging_model(self, kpls_n_comp: int = None, multi=True, **kwargs) -> Tuple['SurrogateModel', Normalization]:
+    def get_md_kriging_model(self, kpls_n_comp: int = None, multi=True, **kwargs_) -> Tuple['SurrogateModel', Normalization]:
         check_dependencies()
         normalization = self.get_md_normalization()
         norm_ds_spec = self.create_smt_design_space_spec(self.problem.design_space, md_normalize=True)
 
-        kwargs.update(
+        kwargs = dict(
             print_global=False,
             design_space=norm_ds_spec.design_space,
             categorical_kernel=MixIntKernelType.EXP_HOMO_HSPHERE,
             hierarchical_kernel=MixHrcKernelType.ALG_KERNEL,
         )
         if norm_ds_spec.is_mixed_discrete:
             kwargs['n_start'] = kwargs.get('n_start', 5)
+        kwargs.update(kwargs_)
 
         if kpls_n_comp is not None:
+            cr_ds_spec = self.create_smt_design_space_spec(
+                self.problem.design_space, md_normalize=True, cont_relax=True)
+            kwargs['design_space'] = cr_ds_spec.design_space
             surrogate = KPLS(n_comp=kpls_n_comp, **kwargs)
-            if norm_ds_spec.is_mixed_discrete:
-                surrogate = MixedIntegerKrigingModel(surrogate)
         else:
             surrogate = KRG(**kwargs)
 
         if multi:
             surrogate = MultiSurrogateModel(surrogate)
 
         return surrogate, normalization
 
 
 class SBArchOptDesignSpace(BaseDesignSpace):
     """SMT design space implementation using SBArchOpt's design space logic"""
 
-    def __init__(self, arch_design_space: ArchDesignSpace, md_normalize=False):
+    _global_disable_hierarchical_cat_fix = False
+
+    def __init__(self, arch_design_space: ArchDesignSpace, md_normalize=False, cont_relax=False):
         self._ds = arch_design_space
         self.normalize = MixedDiscreteNormalization(arch_design_space) if md_normalize else None
+        self._cont_relax = cont_relax
         super().__init__()
 
     @property
     def arch_design_space(self) -> ArchDesignSpace:
         return self._ds
 
     def _get_design_variables(self) -> List['ds.DesignVariable']:
         """Return the design variables defined in this design space if not provided upon initialization of the class"""
         smt_des_vars = []
         is_conditional = self._ds.is_conditionally_active
         normalize = self.normalize is not None
+        cont_relax = self._cont_relax
         for i, dv in enumerate(self._ds.des_vars):
             if isinstance(dv, var.Real):
                 bounds = (0, 1) if normalize else dv.bounds
                 smt_des_vars.append(ds.FloatVariable(bounds[0], bounds[1]))
 
             elif isinstance(dv, var.Integer):
                 bounds = (0, dv.bounds[1]-dv.bounds[0]) if normalize else dv.bounds
-                smt_des_vars.append(ds.IntegerVariable(bounds[0], bounds[1]))
+                if cont_relax:
+                    smt_des_vars.append(ds.FloatVariable(bounds[0], bounds[1]))
+                else:
+                    smt_des_vars.append(ds.IntegerVariable(bounds[0], bounds[1]))
 
             elif isinstance(dv, var.Binary):
-                smt_des_vars.append(ds.OrdinalVariable(values=[0, 1]))
+                if cont_relax:
+                    smt_des_vars.append(ds.FloatVariable(0, 1))
+                else:
+                    smt_des_vars.append(ds.OrdinalVariable(values=[0, 1]))
 
             elif isinstance(dv, var.Choice):
-                # Conditional categorical variables are currently not supported
-                if is_conditional[i]:
-                    smt_des_vars.append(ds.IntegerVariable(0, len(dv.options)-1))
+                if cont_relax:
+                    smt_des_vars.append(ds.FloatVariable(0, len(dv.options)-1))
                 else:
-                    smt_des_vars.append(ds.CategoricalVariable(values=dv.options))
+                    # Conditional categorical variables are currently not supported
+                    if is_conditional[i] and not self._global_disable_hierarchical_cat_fix:
+                        smt_des_vars.append(ds.IntegerVariable(0, len(dv.options)-1))
+                    else:
+                        smt_des_vars.append(ds.CategoricalVariable(values=dv.options))
 
             else:
                 raise ValueError(f'Unexpected variable type: {dv!r}')
         return smt_des_vars
 
     def _is_conditionally_acting(self) -> np.ndarray:
         return self._ds.is_conditionally_active
```

### Comparing `sb-arch-opt-1.1.3/sb_arch_opt/algo/botorch_interface/algo.py` & `sb-arch-opt-1.1.4/sb_arch_opt/algo/botorch_interface/algo.py`

 * *Files identical despite different names*

### Comparing `sb-arch-opt-1.1.3/sb_arch_opt/algo/botorch_interface/api.py` & `sb-arch-opt-1.1.4/sb_arch_opt/algo/botorch_interface/api.py`

 * *Files identical despite different names*

### Comparing `sb-arch-opt-1.1.3/sb_arch_opt/algo/hebo_interface/algo.py` & `sb-arch-opt-1.1.4/sb_arch_opt/algo/hebo_interface/algo.py`

 * *Files identical despite different names*

### Comparing `sb-arch-opt-1.1.3/sb_arch_opt/algo/hebo_interface/api.py` & `sb-arch-opt-1.1.4/sb_arch_opt/algo/hebo_interface/api.py`

 * *Files identical despite different names*

### Comparing `sb-arch-opt-1.1.3/sb_arch_opt/algo/pymoo_interface/api.py` & `sb-arch-opt-1.1.4/sb_arch_opt/algo/pymoo_interface/api.py`

 * *Files identical despite different names*

### Comparing `sb-arch-opt-1.1.3/sb_arch_opt/algo/pymoo_interface/md_mating.py` & `sb-arch-opt-1.1.4/sb_arch_opt/algo/pymoo_interface/md_mating.py`

 * *Files identical despite different names*

### Comparing `sb-arch-opt-1.1.3/sb_arch_opt/algo/pymoo_interface/metrics.py` & `sb-arch-opt-1.1.4/sb_arch_opt/algo/pymoo_interface/metrics.py`

 * *Files identical despite different names*

### Comparing `sb-arch-opt-1.1.3/sb_arch_opt/algo/pymoo_interface/random_search.py` & `sb-arch-opt-1.1.4/sb_arch_opt/algo/pymoo_interface/random_search.py`

 * *Files identical despite different names*

### Comparing `sb-arch-opt-1.1.3/sb_arch_opt/algo/pymoo_interface/storage_restart.py` & `sb-arch-opt-1.1.4/sb_arch_opt/algo/pymoo_interface/storage_restart.py`

 * *Files 2% similar despite different names*

```diff
@@ -248,29 +248,25 @@
     def _apply_extreme_barrier(pop: Population):
         for key in ['F', 'G', 'H']:
             values = pop.get(key)
             values[np.isnan(values)] = np.inf
             pop.set(key, values)
 
     @staticmethod
-    def _normalize_pop(pop: Population, evaluate_values_of, nan_as_inf=True, evaluated_pop: Population = None) -> Population:
+    def _normalize_pop(pop: Population, evaluate_values_of, evaluated_pop: Population = None) -> Population:
         """Ensure that the matrices in a Population are two-dimensional"""
         pop_data = {}
         for key in (['X']+evaluate_values_of):
-            data = pop.get(key)
+            data = pop.get(key, to_numpy=False)
 
-            if len(data.shape) == 1:
-                partial_data = np.zeros((len(data), len(data[0])))*np.nan
-                for i, row in enumerate(data):
-                    if row is not None and len(row) > 0:
-                        if nan_as_inf:
-                            row = row.copy()
-                            row[np.isnan(row)] = np.inf
-                        partial_data[i, :] = row
-                data = partial_data
+            partial_data = np.zeros((len(data), len(data[0])))*np.nan
+            for i, row in enumerate(data):
+                if row is not None and len(row) > 0:
+                    partial_data[i, :] = row
+            data = partial_data
 
             pop_data[key] = data
 
         normalized_pop = Population.new(**pop_data)
         if evaluated_pop is not None:
             normalized_pop = Population.merge(evaluated_pop, normalized_pop)
         return normalized_pop
```

### Comparing `sb-arch-opt-1.1.3/sb_arch_opt/algo/segomoe_interface/algo.py` & `sb-arch-opt-1.1.4/sb_arch_opt/algo/segomoe_interface/algo.py`

 * *Files identical despite different names*

### Comparing `sb-arch-opt-1.1.3/sb_arch_opt/algo/segomoe_interface/api.py` & `sb-arch-opt-1.1.4/sb_arch_opt/algo/segomoe_interface/api.py`

 * *Files identical despite different names*

### Comparing `sb-arch-opt-1.1.3/sb_arch_opt/algo/smarty_interface/algo.py` & `sb-arch-opt-1.1.4/sb_arch_opt/algo/smarty_interface/algo.py`

 * *Files identical despite different names*

### Comparing `sb-arch-opt-1.1.3/sb_arch_opt/algo/smarty_interface/api.py` & `sb-arch-opt-1.1.4/sb_arch_opt/algo/smarty_interface/api.py`

 * *Files identical despite different names*

### Comparing `sb-arch-opt-1.1.3/sb_arch_opt/algo/tpe_interface/api.py` & `sb-arch-opt-1.1.4/sb_arch_opt/algo/tpe_interface/api.py`

 * *Files identical despite different names*

### Comparing `sb-arch-opt-1.1.3/sb_arch_opt/algo/trieste_interface/algo.py` & `sb-arch-opt-1.1.4/sb_arch_opt/algo/trieste_interface/algo.py`

 * *Files identical despite different names*

### Comparing `sb-arch-opt-1.1.3/sb_arch_opt/algo/trieste_interface/api.py` & `sb-arch-opt-1.1.4/sb_arch_opt/algo/trieste_interface/api.py`

 * *Files identical despite different names*

### Comparing `sb-arch-opt-1.1.3/sb_arch_opt/design_space.py` & `sb-arch-opt-1.1.4/sb_arch_opt/design_space.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,22 +32,24 @@
 __all__ = ['ArchDesignSpace', 'ImplicitArchDesignSpace']
 
 
 class ArchDesignSpace:
     """
     Base class for a hierarchical architecture design space definition. The basic information optimization algorithms
     need from a design space is as follows:
+
     - Design variable definition: types, bounds, options
     - Some way to exhaustively sample all discrete design vectors (aka full factorial; grid)
     - Activeness information: for a given matrix of design vectors, a boolean matrix specifying which vars are active
     - Imputation: correction of design vectors to canonical design vectors, setting inactive variables to some default
       value and correcting invalid variable values
     - Optionally calculate the design of the design space: number of valid discrete design vectors
 
     Design variable terminology:
+
     - Continuous: any value between some lower and upper bound (inclusive)
       --> for example [0, 1]: 0, 0.25, .667, 1
     - Discrete: integer or categorical
     - Integer: integer between 0 and some upper bound (inclusive); ordering and distance matters
       --> for example [0, 2]: 0, 1, 2
     - Categorical: one of n options, encoded as integers; ordering and distance are not defined
       --> for example [red, blue, yellow]: red, blue
@@ -195,15 +197,15 @@
 
         Stretched rounding:
         x = np.linspace(0, 2, 100)
         xs = x*((np.max(x)+.99)/np.max(x))-.5
         np.unique(np.abs(np.round(xs)).astype(int), return_counts=True) --> 34, 33, 33 (evenly distributed)
         """
         is_discrete_mask = self.is_discrete_mask
-        x_discrete = x[:, is_discrete_mask].astype(np.float64)
+        x_discrete = x[:, is_discrete_mask].astype(float)
         xl, xu = self.xl[is_discrete_mask], self.xu[is_discrete_mask]
         diff = xu-xl
 
         for ix in range(x_discrete.shape[1]):
             x_discrete[x_discrete[:, ix] < xl[ix], ix] = xl[ix]
             x_discrete[x_discrete[:, ix] > xu[ix], ix] = xu[ix]
 
@@ -245,15 +247,15 @@
 
         # Get number of discrete options for each discrete design variable
         is_discrete_mask = self.is_discrete_mask
         n_opts_discrete = self.xu[is_discrete_mask]-self.xl[is_discrete_mask]+1
         if len(n_opts_discrete) == 0:
             return 1
 
-        return int(np.prod(n_opts_discrete, dtype=np.float))
+        return int(np.prod(n_opts_discrete, dtype=float))
 
     @cached_property
     def imputation_ratio(self) -> float:
         """
         Returns the problem-level imputation ratio, a measure of how hierarchical the problem is. It is calculated
         from the product of the discrete and continuous imputation ratios.
         """
```

### Comparing `sb-arch-opt-1.1.3/sb_arch_opt/design_space_explicit.py` & `sb-arch-opt-1.1.4/sb_arch_opt/design_space_explicit.py`

 * *Files identical despite different names*

### Comparing `sb-arch-opt-1.1.3/sb_arch_opt/pareto_front.py` & `sb-arch-opt-1.1.4/sb_arch_opt/pareto_front.py`

 * *Files identical despite different names*

### Comparing `sb-arch-opt-1.1.3/sb_arch_opt/problem.py` & `sb-arch-opt-1.1.4/sb_arch_opt/problem.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,20 +33,22 @@
 
 __all__ = ['ArchOptProblemBase', 'ArchOptRepair', 'ArchDesignSpace']
 
 
 class ArchOptProblemBase(Problem):
     """
     Base class for an architecture optimization problem, featuring:
+
     - Mixed-discrete design variable definitions
     - Function for imputing a design vector and requesting the activeness vector (specifying which variables were active
       for the imputed design vector)
     - Interface to get a repair operator to implement design vector imputation
 
     Design variable terminology:
+
     - Continuous: any value between some lower and upper bound (inclusive)
       --> for example [0, 1]: 0, 0.25, .667, 1
     - Discrete: integer or categorical
     - Integer: integer between 0 and some upper bound (inclusive); ordering and distance matters
       --> for example [0, 2]: 0, 1, 2
     - Categorical: one of n options, encoded as integers; ordering and distance are not defined
       --> for example [red, blue, yellow]: red, blue
@@ -106,14 +108,15 @@
     @property
     def is_cont_mask(self):
         """Boolean mask specifying for each design variable whether it is a continues (i.e. not discrete) variable"""
         return self.design_space.is_cont_mask
 
     @property
     def is_conditionally_active(self):
+        """Boolean mask specifying for each design variable whether it is conditionally active or not"""
         return self.design_space.is_conditionally_active
 
     def get_categorical_values(self, x: np.ndarray, i_dv) -> np.ndarray:
         """Gets the associated categorical variable values for some design variable"""
         return self.design_space.get_categorical_values(x, i_dv)
 
     def correct_x(self, x: np.ndarray) -> Tuple[np.ndarray, np.ndarray]:
```

### Comparing `sb-arch-opt-1.1.3/sb_arch_opt/problems/assignment.py` & `sb-arch-opt-1.1.4/sb_arch_opt/problems/assignment.py`

 * *Files identical despite different names*

### Comparing `sb-arch-opt-1.1.3/sb_arch_opt/problems/constrained.py` & `sb-arch-opt-1.1.4/sb_arch_opt/problems/constrained.py`

 * *Files identical despite different names*

### Comparing `sb-arch-opt-1.1.3/sb_arch_opt/problems/continuous.py` & `sb-arch-opt-1.1.4/sb_arch_opt/problems/continuous.py`

 * *Files identical despite different names*

### Comparing `sb-arch-opt-1.1.3/sb_arch_opt/problems/discrete.py` & `sb-arch-opt-1.1.4/sb_arch_opt/problems/discrete.py`

 * *Files identical despite different names*

### Comparing `sb-arch-opt-1.1.3/sb_arch_opt/problems/gnc.py` & `sb-arch-opt-1.1.4/sb_arch_opt/problems/gnc.py`

 * *Files identical despite different names*

### Comparing `sb-arch-opt-1.1.3/sb_arch_opt/problems/hidden_constraints.py` & `sb-arch-opt-1.1.4/sb_arch_opt/problems/hidden_constraints.py`

 * *Files identical despite different names*

### Comparing `sb-arch-opt-1.1.3/sb_arch_opt/problems/hierarchical.py` & `sb-arch-opt-1.1.4/sb_arch_opt/problems/hierarchical.py`

 * *Files identical despite different names*

### Comparing `sb-arch-opt-1.1.3/sb_arch_opt/problems/md_mo.py` & `sb-arch-opt-1.1.4/sb_arch_opt/problems/md_mo.py`

 * *Files identical despite different names*

### Comparing `sb-arch-opt-1.1.3/sb_arch_opt/problems/problems_base.py` & `sb-arch-opt-1.1.4/sb_arch_opt/problems/problems_base.py`

 * *Files identical despite different names*

### Comparing `sb-arch-opt-1.1.3/sb_arch_opt/problems/turbofan_arch.py` & `sb-arch-opt-1.1.4/sb_arch_opt/problems/turbofan_arch.py`

 * *Files identical despite different names*

### Comparing `sb-arch-opt-1.1.3/sb_arch_opt/sampling.py` & `sb-arch-opt-1.1.4/sb_arch_opt/sampling.py`

 * *Files 1% similar despite different names*

```diff
@@ -197,15 +197,19 @@
         self.n_iter = 10
         super().__init__()
 
     def _do(self, problem, n_samples, **kwargs):
         x_sampled, _ = self.sample_get_x(problem, n_samples)
         return x_sampled
 
-    def sample_get_x(self, problem, n_samples):
+    def sample_get_x(self, problem: ArchOptProblemBase, n_samples: int) -> Tuple[np.ndarray, np.ndarray]:
+        """
+        Sample design points using the hierarchical sampling algorithm and return is_active information.
+        """
+
         # Get Cartesian product of all discrete design variables (only available if design space is not too large)
         x, is_active = self.get_hierarchical_cartesian_product(problem, self._repair)
 
         x_sampled, is_active = self.randomly_sample(problem, n_samples, self._repair, x, is_active)
         return x_sampled, is_active
 
     @classmethod
```

### Comparing `sb-arch-opt-1.1.3/sb_arch_opt/tests/algo/test_arch_sbo.py` & `sb-arch-opt-1.1.4/sb_arch_opt/tests/algo/test_pymoo.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,172 +1,192 @@
-import pytest
+import os
+import pickle
 import tempfile
 import numpy as np
-from typing import Tuple
+from typing import Optional
 from sb_arch_opt.problem import *
 from sb_arch_opt.sampling import *
-from pymoo.core.variable import Real, Integer, Choice
-from sb_arch_opt.problems.md_mo import *
-from sb_arch_opt.problems.constrained import *
-from sb_arch_opt.problems.hidden_constraints import *
-from sb_arch_opt.tests.algo.test_pymoo import CrashingProblem
-from sb_arch_opt.algo.pymoo_interface import load_from_previous_results
+from sb_arch_opt.algo.pymoo_interface import *
+from sb_arch_opt.algo.pymoo_interface.random_search import RandomSearchAlgorithm
+
 from pymoo.optimize import minimize
+from pymoo.algorithms.soo.nonconvex.ga import GA
+from pymoo.core.variable import Real, Integer
 from pymoo.core.population import Population
+from pymoo.problems.multi.zdt import ZDT1
 
-from sb_arch_opt.algo.arch_sbo import *
-from sb_arch_opt.algo.arch_sbo.algo import *
-from sb_arch_opt.algo.arch_sbo.infill import *
-from sb_arch_opt.algo.arch_sbo.models import *
-from sb_arch_opt.algo.arch_sbo.hc_strategy import *
-
-check_dependency = lambda: pytest.mark.skipif(not HAS_ARCH_SBO, reason='ArchSBO dependencies not installed')
-
-
-@check_dependency()
-def test_arch_sbo_rbf(problem: ArchOptProblemBase):
-    assert HAS_ARCH_SBO
-
-    sbo = get_arch_sbo_rbf(init_size=10)
-    result = minimize(problem, sbo, termination=('n_eval', 12), verbose=True, progress=True)
-    assert len(result.pop) == 12
-
-
-@check_dependency()
-def test_arch_sbo_rbf_termination(problem: ArchOptProblemBase):
-    assert HAS_ARCH_SBO
-
-    sbo = get_arch_sbo_rbf(init_size=10)
-    termination = get_sbo_termination(n_max_infill=12, tol=1e-3)
-    assert minimize(problem, sbo, termination=termination, verbose=True, progress=True)
-
-
-@check_dependency()
-def test_arch_sbo_rbf_failing(failing_problem: ArchOptProblemBase):
-    assert HAS_ARCH_SBO
-
-    sbo = get_arch_sbo_rbf(init_size=10)
-    result = minimize(failing_problem, sbo, termination=('n_eval', 12), verbose=True, progress=True)
-    assert len(result.pop) == 12
-
-
-@check_dependency()
-def test_arch_sbo_y(problem: ArchOptProblemBase):
-    assert HAS_ARCH_SBO
 
-    model = ModelFactory.get_kriging_model()
-    infill = FunctionEstimateConstrainedInfill()
-    sbo = get_sbo(model, infill, init_size=10)
-    result = minimize(problem, sbo, termination=('n_eval', 12))
-    assert len(result.pop) == 12
+def test_provision():
+    ga = GA()
+    provision_pymoo(ga)
+    assert isinstance(ga.repair, ArchOptRepair)
+    assert isinstance(ga.initialization.sampling, HierarchicalSampling)
 
 
-@check_dependency()
-def test_arch_sbo_ei(problem: ArchOptProblemBase):
-    assert HAS_ARCH_SBO
+def test_nsga2(problem: ArchOptProblemBase):
+    nsga2 = get_nsga2(pop_size=100)
+    result = minimize(problem, nsga2, termination=('n_gen', 10), verbose=True, progress=True)
+    pop = result.pop
 
-    model = ModelFactory.get_kriging_model()
-    infill = ExpectedImprovementInfill()
-    sbo = get_sbo(model, infill, init_size=10)
-    result = minimize(problem, sbo, termination=('n_eval', 12))
-    assert len(result.pop) == 12
+    x_imp, _ = problem.correct_x(pop.get('X'))
+    assert np.all(pop.get('X') == x_imp)
 
 
-@check_dependency()
-def test_arch_sbo_mvpf():
-    model = ModelFactory.get_kriging_model()
-    infill = MinVariancePFInfill()
-    sbo = get_sbo(model, infill, init_size=10)
-    result = minimize(MOHimmelblau(), sbo, termination=('n_eval', 12))
-    assert len(result.pop) == 12
+def test_termination(problem: ArchOptProblemBase):
+    nsga2 = get_nsga2(pop_size=100)
+    assert minimize(problem, nsga2, get_default_termination(problem, tol=1e-4), verbose=True, progress=True)
 
 
-@check_dependency()
-def test_arch_sbo_hc_rf():
-    assert HAS_ARCH_SBO
+def test_failing_evaluations(failing_problem: ArchOptProblemBase):
+    nsga2 = get_nsga2(pop_size=100)
+    assert minimize(failing_problem, nsga2, termination=('n_gen', 10), verbose=True, progress=True)
 
-    hc_strategy = PredictionHCStrategy(RandomForestClassifier())
 
-    problem = Mueller01()
-    model = ModelFactory.get_kriging_model()
-    infill = MinVariancePFInfill()
-    sbo = get_sbo(model, infill, hc_strategy=hc_strategy, init_size=10)
-    result = minimize(problem, sbo, termination=('n_eval', 11))
-    assert len(result.pop) == 11
+class DummyResultSavingProblem(ArchOptProblemBase):
 
+    def __init__(self):
+        self._problem = problem = ZDT1(n_var=5)
+        var_types = [Real(bounds=(0, 1)) if i % 2 == 0 else Integer(bounds=(0, 9)) for i in range(problem.n_var)]
+        super().__init__(var_types, n_obj=problem.n_obj)
+
+        self.n_eval = 0
+        self.n_stored = 0
+        self.last_evaluated = None
+        self.provide_previous_results = True
 
-@check_dependency()
-def test_arch_sbo_hc_md_gp():
-    assert HAS_ARCH_SBO
+    def _arch_evaluate(self, x: np.ndarray, is_active_out: np.ndarray, f_out: np.ndarray, g_out: np.ndarray,
+                       h_out: np.ndarray, *args, **kwargs):
+        self.n_eval += 1
+        self._correct_x(x, is_active_out)
+        x_eval = x.copy()
+        x_eval[:, self.is_discrete_mask] /= 9
+        out = self._problem.evaluate(x_eval, return_as_dictionary=True)
+        f_out[:, :] = out['F']
+        self.last_evaluated = (x.copy(), is_active_out.copy(), f_out.copy())
+
+    def _correct_x(self, x: np.ndarray, is_active: np.ndarray):
+        is_active[:, -1] = x[:, 1] < 5
+        self.impute_x(x, is_active)
+
+    def store_results(self, results_folder):
+        self.n_stored += 1
+
+        assert self.last_evaluated is not None
+        with open(os.path.join(results_folder, 'problem_last_pop.pkl'), 'wb') as fp:
+            pickle.dump(self.last_evaluated, fp)
+
+    def load_previous_results(self, results_folder) -> Optional[Population]:
+        if not self.provide_previous_results:
+            return
+        path = os.path.join(results_folder, 'problem_last_pop.pkl')
+        if not os.path.exists(path):
+            return
+        with open(path, 'rb') as fp:
+            x, is_active, f = pickle.load(fp)
+        return Population.new(X=x, F=f, is_active=is_active)
 
-    hc_strategy = PredictionHCStrategy(MDGPRegressor())
+    def __repr__(self):
+        return f'{self.__class__.__name__}()'
 
-    problem = Mueller01()
-    model = ModelFactory.get_kriging_model()
-    infill = MinVariancePFInfill()
-    sbo = get_sbo(model, infill, hc_strategy=hc_strategy, init_size=10)
-    result = minimize(problem, sbo, termination=('n_eval', 11))
-    assert len(result.pop) == 11
 
+def test_store_results_restart():
+    problem = DummyResultSavingProblem()
 
-@check_dependency()
-def test_arch_sbo_gp(problem: ArchOptProblemBase):
-    assert HAS_ARCH_SBO
+    with tempfile.TemporaryDirectory() as tmp_folder:
+        for i in range(5):
+            nsga2 = get_nsga2(pop_size=100, results_folder=tmp_folder)
+            assert isinstance(nsga2.evaluator, ArchOptEvaluator)
+            nsga2.evaluator.n_batch = 500
+            assert isinstance(nsga2.callback, ResultsStorageCallback)
+
+            if i > 2:
+                problem.provide_previous_results = False
+            assert initialize_from_previous_results(nsga2, problem, tmp_folder) == (i > 0)
+            if i > 0:
+                assert isinstance(nsga2.initialization.sampling, Population)
+                assert len(nsga2.initialization.sampling) - (100+2*100*i) < 20
+
+            minimize(problem, nsga2, termination=('n_gen', 3), copy_algorithm=False)
+            assert os.path.exists(os.path.join(tmp_folder, 'pymoo_results.pkl'))
+            assert os.path.exists(os.path.join(tmp_folder, 'pymoo_population.pkl'))
+            assert os.path.exists(os.path.join(tmp_folder, 'pymoo_population.csv'))
+            assert os.path.exists(os.path.join(tmp_folder, 'pymoo_population_cumulative.pkl'))
+            assert os.path.exists(os.path.join(tmp_folder, 'pymoo_population_cumulative.csv'))
 
-    _, n_batch = get_default_infill(problem)
-    assert n_batch == 1
+            assert problem.n_eval == 3+2*i  # 3 for initial population, 2 for next because the first is a restart
+            assert problem.n_stored == 6+5*i
 
-    sbo = get_arch_sbo_gp(problem, init_size=10)
-    result = minimize(problem, sbo, termination=('n_eval', 12))
-    assert len(result.pop) == 12
+            n_cumulative = load_from_previous_results(problem, tmp_folder)
+            assert abs(len(n_cumulative) - (100+2*100*(i+1))) < 20
 
 
-@check_dependency()
-def test_arch_sbo_gp_failing():
-    assert HAS_ARCH_SBO
+def test_batch_storage_evaluator(problem: ArchOptProblemBase):
+    with tempfile.TemporaryDirectory() as tmp_folder:
+        pop = HierarchicalSampling().do(problem, 110)
+        assert pop.get('F').shape == (110, 0)
 
-    problem = Mueller01()
-    sbo = get_arch_sbo_gp(problem, init_size=10)
-    result = minimize(problem, sbo, termination=('n_eval', 12))
-    assert len(result.pop) == 12
+        evaluator = ArchOptEvaluator(results_folder=tmp_folder, n_batch=20)
+        pop = evaluator.eval(problem, pop)
+        assert len(pop) == 110
+        assert pop.get('F').shape == (110, 2)
 
+        pop_loaded = load_from_previous_results(problem, tmp_folder)
+        assert np.all(pop_loaded.get('X') == pop.get('X'))
+        assert np.all(pop_loaded.get('F') == pop.get('F'))
 
-@check_dependency()
-def test_arch_sbo_gp_batch(problem: ArchOptProblemBase):
-    _, n_batch = get_default_infill(problem, n_parallel=5)
-    assert n_batch == 5
 
-    sbo = get_arch_sbo_gp(problem, init_size=10, n_parallel=5)
-    result = minimize(problem, sbo, termination=('n_gen', 2))
-    assert len(result.pop) == 15
+def test_doe_algo(problem: ArchOptProblemBase):
+    with tempfile.TemporaryDirectory() as tmp_folder:
+        doe_algo = get_doe_algo(doe_size=100)
+        doe_algo.setup(problem)
+        doe_algo.run()
+        pop = doe_algo.pop
+        assert len(pop) == 100
+        assert not os.path.exists(os.path.join(tmp_folder, 'pymoo_population.csv'))
+
+        doe_algo = get_doe_algo(doe_size=100, results_folder=tmp_folder)
+        doe_algo.setup(problem)
+        doe_algo.run()
+        pop = doe_algo.pop
+        assert len(pop) == 100
+        assert os.path.exists(os.path.join(tmp_folder, 'pymoo_population.csv'))
+
+        pop_loaded = load_from_previous_results(problem, tmp_folder)
+        assert pop_loaded.get('X').shape == pop.get('X').shape
+        assert pop_loaded.get('F').shape == pop.get('F').shape
+
+
+class CrashingProblem(DummyResultSavingProblem):
+
+    def __init__(self, failed_evals=True):
+        self.failed_evals = failed_evals
+        super().__init__()
+        self.i_eval = 0
 
+    def _arch_evaluate(self, x: np.ndarray, is_active_out: np.ndarray, f_out: np.ndarray, g_out: np.ndarray,
+                       h_out: np.ndarray, *args, **kwargs):
+        super()._arch_evaluate(x, is_active_out, f_out, g_out, h_out, *args, **kwargs)
 
-@check_dependency()
-def test_arch_sbo_gp_high_dim():
-    assert HAS_ARCH_SBO
+        if self.failed_evals:
+            i_failed = np.arange(0, x.shape[0])[::2]
+            f_out[i_failed, :] = np.nan
+            g_out[i_failed, :] = np.nan
 
-    problem = MOZDT1()
-    sbo = get_arch_sbo_gp(problem, init_size=10, kpls_n_dim=5)
-    result = minimize(problem, sbo, termination=('n_eval', 12))
-    assert len(result.pop) == 12
+        self.i_eval += 1
+        if self.i_eval > 1:
+            raise RuntimeError
 
+    def get_n_batch_evaluate(self) -> Optional[int]:
+        return 10
 
-@check_dependency()
-def test_store_results_restart(problem: ArchOptProblemBase):
-    assert HAS_ARCH_SBO
+    def store_results(self, results_folder):
+        pass
 
-    with tempfile.TemporaryDirectory() as tmp_folder:
-        for i in range(2):
-            sbo = get_arch_sbo_rbf(init_size=10)
-            sbo.store_intermediate_results(tmp_folder)
-            sbo.initialize_from_previous_results(problem, tmp_folder)
-
-            n_eval = 10+(i+1)
-            result = minimize(problem, sbo, termination=('n_eval', n_eval))
-            assert len(result.pop) == 10+(i+1)
+    def load_previous_results(self, results_folder) -> Optional[Population]:
+        pass
 
 
 def test_partial_restart():
     with tempfile.TemporaryDirectory() as tmp_folder:
         for i in range(100):
             try:
                 problem = CrashingProblem()
@@ -182,98 +202,53 @@
                     assert x.shape == (20*((i+1)//2), problem.n_var)
 
                     f = pop.get('F')
                     assert f.shape == (x.shape[0], problem.n_obj)
                     n_empty = np.sum(np.any(np.isnan(f), axis=1))
                     assert n_empty == x.shape[0]-n_evaluated
 
-                sbo = get_arch_sbo_rbf(init_size=20, results_folder=tmp_folder)
-                sbo.infill_size = 20
-
-                sbo.initialize_from_previous_results(problem, result_folder=tmp_folder)
-                assert sbo.evaluator.n_eval == n_evaluated
-                result = minimize(problem, sbo, termination=('n_eval', 40))
+                nsga2 = get_nsga2(pop_size=20, results_folder=tmp_folder)
+                initialize_from_previous_results(nsga2, problem, tmp_folder)
+                assert nsga2.evaluator.n_eval == n_evaluated
+                result = minimize(problem, nsga2, termination=('n_eval', 40))
                 assert len(result.pop) == 40
                 break
 
             except RuntimeError:
                 pass
 
 
-@check_dependency()
-def test_constraint_handling():
-    problem = ArchCarside()
-    assert problem.n_ieq_constr == 10
-
-    for strategy, n_g_infill in [
-        (MeanConstraintPrediction(), {problem.n_ieq_constr}),
-        (MeanConstraintPrediction(aggregation=ConstraintAggregation.ELIMINATE), set(range(1, 5))),
-        (MeanConstraintPrediction(aggregation=ConstraintAggregation.AGGREGATE), {1}),
-        (ProbabilityOfFeasibility(), {problem.n_ieq_constr}),
-        (ProbabilityOfFeasibility(min_pof=.25), {problem.n_ieq_constr}),
-    ]:
-        model = ModelFactory.get_kriging_model()
-        infill = FunctionEstimateConstrainedInfill(constraint_strategy=strategy)
-        sbo = get_sbo(model, infill, init_size=10)
-
-        result = minimize(problem, sbo, termination=('n_eval', 12), copy_algorithm=False)
-        assert infill.constraint_strategy.problem is problem
-        assert infill.get_n_infill_constraints() in n_g_infill
-        assert len(result.pop) == 12
-
-
-class FailedXYRemovingSBO(SBOInfill):
-
-    def _get_xy_train(self, x: np.ndarray, y: np.ndarray) -> Tuple[np.ndarray, np.ndarray]:
-        is_failed = np.any(~np.isfinite(y), axis=1)
-        return x[~is_failed, :], y[~is_failed, :]
-
-
-@check_dependency()
-def test_invalid_training_set(problem: ArchOptProblemBase):
-    from smt.surrogate_models.rbf import RBF
-    sbo = FailedXYRemovingSBO(RBF(print_global=False), FunctionEstimateInfill(), pop_size=100, termination=100,
-                              repair=ArchOptRepair()).algorithm(infill_size=1, init_size=10)
-    sbo.setup(problem)
-
-    for i in range(2):
-        pop = sbo.ask()
-        assert len(pop) == (10 if i == 0 else 1)
-        sbo.evaluator.eval(problem, pop)
-        pop.set('F', pop.get('F')*np.nan)
-        sbo.tell(pop)
-
-    sbo.ask()
-
-
-class MDNormProblem(ArchOptProblemBase):
-
-    def __init__(self):
-        super().__init__(des_vars=[
-            Real(bounds=(-5, 2)),
-            Integer(bounds=[0, 5]),
-            Integer(bounds=[-1, 2]),
-            Integer(bounds=[1, 10]),
-            Choice(options=[1, 2, 3]),
-        ])
+def test_partial_doe_restart():
+    with tempfile.TemporaryDirectory() as tmp_folder:
+        for i in range(100):
+            try:
+                problem = CrashingProblem()
+                pop = load_from_previous_results(problem, tmp_folder)
+                n_empty = 30
+                if i == 0:
+                    assert pop is None
+                else:
+                    assert isinstance(pop, Population)
+                    x = pop.get('X')
+                    assert np.all(np.isfinite(x))
+                    assert x.shape == (30, problem.n_var)
 
-    def _arch_evaluate(self, x: np.ndarray, is_active_out: np.ndarray, f_out: np.ndarray, g_out: np.ndarray,
-                       h_out: np.ndarray, *args, **kwargs):
-        raise RuntimeError
+                    f = pop.get('F')
+                    assert f.shape == (30, problem.n_obj)
+                    n_empty = np.sum(np.any(np.isnan(f), axis=1))
+                    assert n_empty == 30-i*10
 
-    def __repr__(self):
-        return f'{self.__class__.__name__}()'
+                doe_algo = get_doe_algo(doe_size=30, results_folder=tmp_folder)
+                initialize_from_previous_results(doe_algo, problem, tmp_folder)
+                assert doe_algo.evaluator.n_eval == 30-n_empty
+                doe_algo.setup(problem)
+                doe_algo.run()
+                break
 
+            except RuntimeError:
+                pass
 
-def test_md_normalization():
-    problem = MDNormProblem()
-    x = HierarchicalSampling().do(problem, 1000).get('X')
-    assert np.all(np.round(np.min(x, axis=0)) == problem.xl)
-    assert np.all(np.round(np.max(x, axis=0)) == problem.xu)
-
-    md_norm = MixedDiscreteNormalization(problem.design_space)
-    x_norm = md_norm.forward(x)
-    assert np.all(np.round(np.min(x_norm, axis=0)) == [0, 0, 0, 0, 0])
-    assert np.all(np.round(np.max(x_norm, axis=0)) == [1, 5, 3, 9, 2])
 
-    x_abs = md_norm.backward(x_norm)
-    assert np.all(x == x_abs)
+def test_random_search(problem: ArchOptProblemBase):
+    rs = RandomSearchAlgorithm(n_init=10)
+    result = minimize(problem, rs, termination=('n_eval', 100))
+    assert len(result.pop) == 100
```

### Comparing `sb-arch-opt-1.1.3/sb_arch_opt/tests/algo/test_botorch.py` & `sb-arch-opt-1.1.4/sb_arch_opt/tests/algo/test_botorch.py`

 * *Files identical despite different names*

### Comparing `sb-arch-opt-1.1.3/sb_arch_opt/tests/algo/test_hebo.py` & `sb-arch-opt-1.1.4/sb_arch_opt/tests/algo/test_hebo.py`

 * *Files identical despite different names*

### Comparing `sb-arch-opt-1.1.3/sb_arch_opt/tests/algo/test_segomoe.py` & `sb-arch-opt-1.1.4/sb_arch_opt/tests/algo/test_segomoe.py`

 * *Files identical despite different names*

### Comparing `sb-arch-opt-1.1.3/sb_arch_opt/tests/algo/test_smarty.py` & `sb-arch-opt-1.1.4/sb_arch_opt/tests/algo/test_smarty.py`

 * *Files identical despite different names*

### Comparing `sb-arch-opt-1.1.3/sb_arch_opt/tests/algo/test_tpe.py` & `sb-arch-opt-1.1.4/sb_arch_opt/tests/algo/test_tpe.py`

 * *Files identical despite different names*

### Comparing `sb-arch-opt-1.1.3/sb_arch_opt/tests/algo/test_trieste.py` & `sb-arch-opt-1.1.4/sb_arch_opt/tests/algo/test_trieste.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import os
 import pytest
 import tempfile
 from sb_arch_opt.problem import *
 from sb_arch_opt.algo.trieste_interface import *
 from sb_arch_opt.problems.constrained import ArchCantileveredBeam
 from sb_arch_opt.algo.trieste_interface.algo import ArchOptBayesianOptimizer
 
@@ -22,32 +23,35 @@
     assert repr(opt)
     result = opt.run_optimization()
 
     pop = opt.to_population(result.datasets)
     assert len(pop) == 11
 
 
+@pytest.mark.skipif(int(os.getenv('RUN_SLOW_TESTS', 0)) != 1, reason='Set RUN_SLOW_TESTS=1 to run slow tests')
 @check_dependency()
 def test_constrained():
     opt = get_trieste_optimizer(ArchCantileveredBeam(), n_init=10, n_infill=1)
     assert opt.run_optimization()
 
 
+@pytest.mark.skipif(int(os.getenv('RUN_SLOW_TESTS', 0)) != 1, reason='Set RUN_SLOW_TESTS=1 to run slow tests')
 @check_dependency()
 def test_store_results_restart(problem: ArchOptProblemBase):
     with tempfile.TemporaryDirectory() as tmp_folder:
         for i in range(2):
             opt = get_trieste_optimizer(problem, n_init=10, n_infill=1+i)
             opt.initialize_from_previous(tmp_folder)
             result = opt.run_optimization(results_folder=tmp_folder)
 
             pop = opt.to_population(result.datasets)
             assert len(pop) == 11+i
 
 
+@pytest.mark.skipif(int(os.getenv('RUN_SLOW_TESTS', 0)) != 1, reason='Set RUN_SLOW_TESTS=1 to run slow tests')
 @check_dependency()
 def test_simple_failing(failing_problem: ArchOptProblemBase):
     opt = get_trieste_optimizer(failing_problem, n_init=10, n_infill=1)
     result = opt.run_optimization()
 
     pop = opt.to_population(result.datasets)
     assert len(pop) == 5
```

### Comparing `sb-arch-opt-1.1.3/sb_arch_opt/tests/conftest.py` & `sb-arch-opt-1.1.4/sb_arch_opt/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `sb-arch-opt-1.1.3/sb_arch_opt/tests/problems/test_assignment.py` & `sb-arch-opt-1.1.4/sb_arch_opt/tests/problems/test_assignment.py`

 * *Files identical despite different names*

### Comparing `sb-arch-opt-1.1.3/sb_arch_opt/tests/problems/test_constrained.py` & `sb-arch-opt-1.1.4/sb_arch_opt/tests/problems/test_constrained.py`

 * *Files identical despite different names*

### Comparing `sb-arch-opt-1.1.3/sb_arch_opt/tests/problems/test_gnc.py` & `sb-arch-opt-1.1.4/sb_arch_opt/tests/problems/test_gnc.py`

 * *Files identical despite different names*

### Comparing `sb-arch-opt-1.1.3/sb_arch_opt/tests/problems/test_hidden_constraints.py` & `sb-arch-opt-1.1.4/sb_arch_opt/tests/problems/test_hidden_constraints.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import os
+import pytest
 from sb_arch_opt.problems.hidden_constraints import *
 from sb_arch_opt.tests.problems.test_discrete import run_test_no_hierarchy
 from sb_arch_opt.tests.problems.test_hierarchical import run_test_hierarchy
 
 
 def test_mueller_01():
     run_test_no_hierarchy(Mueller01())
@@ -9,23 +11,25 @@
 
 def test_mueller_02():
     run_test_no_hierarchy(Mueller02())
     run_test_no_hierarchy(MDMueller02())
     run_test_hierarchy(HierMueller02(), 5.4)
 
 
+@pytest.mark.skipif(int(os.getenv('RUN_SLOW_TESTS', 0)) != 1, reason='Set RUN_SLOW_TESTS=1 to run slow tests')
 def test_mueller_08():
     run_test_no_hierarchy(Mueller08())
     run_test_no_hierarchy(MOMueller08())
     run_test_no_hierarchy(MDMueller08())
     run_test_no_hierarchy(MDMOMueller08())
     run_test_hierarchy(HierMueller08(), 5.4)
     run_test_hierarchy(MOHierMueller08(), 5.4)
 
 
+@pytest.mark.skipif(int(os.getenv('RUN_SLOW_TESTS', 0)) != 1, reason='Set RUN_SLOW_TESTS=1 to run slow tests')
 def test_alimo():
     run_test_no_hierarchy(Alimo())
     run_test_no_hierarchy(AlimoEdge())
     run_test_hierarchy(HierAlimo(), 5.4)
     run_test_hierarchy(HierAlimoEdge(), 5.4)
```

### Comparing `sb-arch-opt-1.1.3/sb_arch_opt/tests/problems/test_hierarchical.py` & `sb-arch-opt-1.1.4/sb_arch_opt/tests/problems/test_hierarchical.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import os
 import pytest
 import numpy as np
 from sb_arch_opt.sampling import *
 from sb_arch_opt.problems.continuous import *
 from sb_arch_opt.problems.hierarchical import *
 from pymoo.core.evaluator import Evaluator
 
@@ -68,25 +69,28 @@
     run_test_hierarchy(Jenatton(explicit=False), 2)
 
 
 def test_hier_branin():
     run_test_hierarchy(HierBranin(), 3.24, validate_exhaustive=True)
 
 
+@pytest.mark.skipif(int(os.getenv('RUN_SLOW_TESTS', 0)) != 1, reason='Set RUN_SLOW_TESTS=1 to run slow tests')
 def test_hier_zdt1():
     run_test_hierarchy(HierZDT1Small(), 1.8, validate_exhaustive=True)
     run_test_hierarchy(HierZDT1(), 4.86, validate_exhaustive=True)
     run_test_hierarchy(HierZDT1Large(), 8.19)
     run_test_hierarchy(HierDiscreteZDT1(), 4.1)
 
 
+@pytest.mark.skipif(int(os.getenv('RUN_SLOW_TESTS', 0)) != 1, reason='Set RUN_SLOW_TESTS=1 to run slow tests')
 def test_hier_cantilevered_beam():
     run_test_hierarchy(HierCantileveredBeam(), 5.4)
 
 
+@pytest.mark.skipif(int(os.getenv('RUN_SLOW_TESTS', 0)) != 1, reason='Set RUN_SLOW_TESTS=1 to run slow tests')
 def test_hier_carside():
     run_test_hierarchy(HierCarside(), 6.48)
 
 
 def test_hier_nn():
     run_test_hierarchy(NeuralNetwork(), 2.51)
```

### Comparing `sb-arch-opt-1.1.3/sb_arch_opt/tests/problems/test_md_mo.py` & `sb-arch-opt-1.1.4/sb_arch_opt/tests/problems/test_md_mo.py`

 * *Files identical despite different names*

### Comparing `sb-arch-opt-1.1.3/sb_arch_opt/tests/problems/test_turbofan_arch.py` & `sb-arch-opt-1.1.4/sb_arch_opt/tests/problems/test_turbofan_arch.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import os
 import pytest
 import tempfile
 import numpy as np
 from sb_arch_opt.sampling import *
 from sb_arch_opt.problems.turbofan_arch import *
 from sb_arch_opt.algo.pymoo_interface import get_nsga2
 from pymoo.optimize import minimize
@@ -43,15 +44,15 @@
     assert len(x_pf) == 1
     f_pf = problem.pareto_front()
     assert len(f_pf) == 1
 
     assert problem._load_evaluated()
 
 
-# @pytest.mark.skip('Takes about 1 minute')
+@pytest.mark.skipif(int(os.getenv('RUN_SLOW_TESTS', 0)) != 1, reason='Set RUN_SLOW_TESTS=1 to run slow tests')
 @check_dependency()
 def test_simple_problem_eval():
     with tempfile.TemporaryDirectory() as tmp_folder:
         problem = SimpleTurbofanArch(n_parallel=2)
         algo = get_nsga2(pop_size=2, results_folder=tmp_folder)
 
         algo.initialization = Initialization(Population.new(X=np.array([
```

### Comparing `sb-arch-opt-1.1.3/sb_arch_opt/tests/test_design_space.py` & `sb-arch-opt-1.1.4/sb_arch_opt/tests/test_design_space.py`

 * *Files identical despite different names*

### Comparing `sb-arch-opt-1.1.3/sb_arch_opt/tests/test_design_space_explicit.py` & `sb-arch-opt-1.1.4/sb_arch_opt/tests/test_design_space_explicit.py`

 * *Files identical despite different names*

### Comparing `sb-arch-opt-1.1.3/sb_arch_opt/tests/test_problem.py` & `sb-arch-opt-1.1.4/sb_arch_opt/tests/test_problem.py`

 * *Files identical despite different names*

### Comparing `sb-arch-opt-1.1.3/sb_arch_opt/util.py` & `sb-arch-opt-1.1.4/sb_arch_opt/util.py`

 * *Files identical despite different names*

### Comparing `sb-arch-opt-1.1.3/sb_arch_opt.egg-info/SOURCES.txt` & `sb-arch-opt-1.1.4/sb_arch_opt.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -57,14 +57,15 @@
 sb_arch_opt/problems/problems_base.py
 sb_arch_opt/problems/turbofan_arch.py
 sb_arch_opt/tests/__init__.py
 sb_arch_opt/tests/conftest.py
 sb_arch_opt/tests/test_design_space.py
 sb_arch_opt/tests/test_design_space_explicit.py
 sb_arch_opt/tests/test_problem.py
+sb_arch_opt/tests/test_tutorials.py
 sb_arch_opt/tests/algo/__init__.py
 sb_arch_opt/tests/algo/test_arch_sbo.py
 sb_arch_opt/tests/algo/test_botorch.py
 sb_arch_opt/tests/algo/test_hebo.py
 sb_arch_opt/tests/algo/test_pymoo.py
 sb_arch_opt/tests/algo/test_segomoe.py
 sb_arch_opt/tests/algo/test_smarty.py
```

### Comparing `sb-arch-opt-1.1.3/setup.py` & `sb-arch-opt-1.1.4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -58,15 +58,16 @@
             'pandas',
             'cached-property~=1.5',
             'ConfigSpace~=0.6.1',
             'more-itertools~=9.1',
         ],
         extras_require={
             'arch_sbo': [
-                'smt~=2.0b3',
+                'smt~=2.0',
+                'numba',
                 'scikit-learn',
             ],
             # 'ota': [  # pip install -r requirements-ota.txt
             #     'open_turb_arch @ git+https://github.com/jbussemaker/OpenTurbofanArchitecting@pymoo_optional#egg=open_turb_arch',
             # ],
             # 'assignment': [  # pip install -r requirements-assignment.txt
             #     'assign_enc @ git+https://github.com/jbussemaker/AssignmentEncoding#egg=assign_enc',
```

