# Comparing `tmp/dantro-0.19.0b1.tar.gz` & `tmp/dantro-0.19.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dantro-0.19.0b1.tar", last modified: Wed Dec  7 15:32:57 2022, max compression
+gzip compressed data, was "dantro-0.19.0b2.tar", last modified: Fri Dec  9 16:49:32 2022, max compression
```

## Comparing `dantro-0.19.0b1.tar` & `dantro-0.19.0b2.tar`

### file list

```diff
@@ -1,109 +1,109 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-07 15:32:57.474126 dantro-0.19.0b1/
--rw-rw-rw-   0 root         (0) root         (0)    35149 2022-12-07 15:32:45.000000 dantro-0.19.0b1/COPYING
--rw-rw-rw-   0 root         (0) root         (0)     7633 2022-12-07 15:32:45.000000 dantro-0.19.0b1/COPYING.LESSER
--rw-r--r--   0 root         (0) root         (0)     3220 2022-12-07 15:32:57.474126 dantro-0.19.0b1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)    15686 2022-12-07 15:32:45.000000 dantro-0.19.0b1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-07 15:32:57.451245 dantro-0.19.0b1/dantro/
--rw-rw-rw-   0 root         (0) root         (0)     1007 2022-12-07 15:32:45.000000 dantro-0.19.0b1/dantro/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      889 2022-12-07 15:32:45.000000 dantro-0.19.0b1/dantro/_copy.py
--rw-rw-rw-   0 root         (0) root         (0)    30886 2022-12-07 15:32:45.000000 dantro-0.19.0b1/dantro/_dag_utils.py
--rw-rw-rw-   0 root         (0) root         (0)      922 2022-12-07 15:32:45.000000 dantro-0.19.0b1/dantro/_hash.py
--rw-rw-rw-   0 root         (0) root         (0)    14740 2022-12-07 15:32:45.000000 dantro-0.19.0b1/dantro/_import_tools.py
--rw-rw-rw-   0 root         (0) root         (0)     7267 2022-12-07 15:32:45.000000 dantro-0.19.0b1/dantro/_registry.py
--rw-rw-rw-   0 root         (0) root         (0)     9390 2022-12-07 15:32:45.000000 dantro-0.19.0b1/dantro/_yaml.py
--rw-rw-rw-   0 root         (0) root         (0)    15796 2022-12-07 15:32:45.000000 dantro-0.19.0b1/dantro/abc.py
--rw-rw-rw-   0 root         (0) root         (0)    44192 2022-12-07 15:32:45.000000 dantro-0.19.0b1/dantro/base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-07 15:32:57.453075 dantro-0.19.0b1/dantro/cfg/
--rw-rw-rw-   0 root         (0) root         (0)    22021 2022-12-07 15:32:45.000000 dantro-0.19.0b1/dantro/cfg/base_plots.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-07 15:32:57.454906 dantro-0.19.0b1/dantro/containers/
--rw-rw-rw-   0 root         (0) root         (0)      545 2022-12-07 15:32:45.000000 dantro-0.19.0b1/dantro/containers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3675 2022-12-07 15:32:45.000000 dantro-0.19.0b1/dantro/containers/_registry.py
--rw-rw-rw-   0 root         (0) root         (0)     3223 2022-12-07 15:32:45.000000 dantro-0.19.0b1/dantro/containers/general.py
--rw-rw-rw-   0 root         (0) root         (0)     1302 2022-12-07 15:32:45.000000 dantro-0.19.0b1/dantro/containers/link.py
--rw-rw-rw-   0 root         (0) root         (0)     3409 2022-12-07 15:32:45.000000 dantro-0.19.0b1/dantro/containers/numeric.py
--rw-rw-rw-   0 root         (0) root         (0)     3489 2022-12-07 15:32:45.000000 dantro-0.19.0b1/dantro/containers/path.py
--rw-rw-rw-   0 root         (0) root         (0)    13561 2022-12-07 15:32:45.000000 dantro-0.19.0b1/dantro/containers/xr.py
--rw-rw-rw-   0 root         (0) root         (0)   130454 2022-12-07 15:32:45.000000 dantro-0.19.0b1/dantro/dag.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-07 15:32:57.457651 dantro-0.19.0b1/dantro/data_loaders/
--rw-rw-rw-   0 root         (0) root         (0)     2963 2022-12-07 15:32:45.000000 dantro-0.19.0b1/dantro/data_loaders/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6739 2022-12-07 15:32:45.000000 dantro-0.19.0b1/dantro/data_loaders/_registry.py
--rw-rw-rw-   0 root         (0) root         (0)     3786 2022-12-07 15:32:45.000000 dantro-0.19.0b1/dantro/data_loaders/fspath.py
--rw-rw-rw-   0 root         (0) root         (0)    19584 2022-12-07 15:32:45.000000 dantro-0.19.0b1/dantro/data_loaders/hdf5.py
--rw-rw-rw-   0 root         (0) root         (0)     2009 2022-12-07 15:32:45.000000 dantro-0.19.0b1/dantro/data_loaders/numpy.py
--rw-rw-rw-   0 root         (0) root         (0)     4230 2022-12-07 15:32:45.000000 dantro-0.19.0b1/dantro/data_loaders/pandas.py
--rw-rw-rw-   0 root         (0) root         (0)     1180 2022-12-07 15:32:45.000000 dantro-0.19.0b1/dantro/data_loaders/pickle.py
--rw-rw-rw-   0 root         (0) root         (0)      993 2022-12-07 15:32:45.000000 dantro-0.19.0b1/dantro/data_loaders/text.py
--rw-rw-rw-   0 root         (0) root         (0)     3442 2022-12-07 15:32:45.000000 dantro-0.19.0b1/dantro/data_loaders/xarray.py
--rw-rw-rw-   0 root         (0) root         (0)     2165 2022-12-07 15:32:45.000000 dantro-0.19.0b1/dantro/data_loaders/yaml.py
--rw-rw-rw-   0 root         (0) root         (0)    64943 2022-12-07 15:32:45.000000 dantro-0.19.0b1/dantro/data_mngr.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-07 15:32:57.461313 dantro-0.19.0b1/dantro/data_ops/
--rw-rw-rw-   0 root         (0) root         (0)      454 2022-12-07 15:32:45.000000 dantro-0.19.0b1/dantro/data_ops/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      979 2022-12-07 15:32:45.000000 dantro-0.19.0b1/dantro/data_ops/_base_ops.py
--rw-rw-rw-   0 root         (0) root         (0)     2807 2022-12-07 15:32:45.000000 dantro-0.19.0b1/dantro/data_ops/apply.py
--rw-rw-rw-   0 root         (0) root         (0)    28398 2022-12-07 15:32:45.000000 dantro-0.19.0b1/dantro/data_ops/arr_ops.py
--rw-rw-rw-   0 root         (0) root         (0)     2716 2022-12-07 15:32:45.000000 dantro-0.19.0b1/dantro/data_ops/ctrl_ops.py
--rw-rw-rw-   0 root         (0) root         (0)    16685 2022-12-07 15:32:45.000000 dantro-0.19.0b1/dantro/data_ops/db.py
--rw-rw-rw-   0 root         (0) root         (0)     8250 2022-12-07 15:32:45.000000 dantro-0.19.0b1/dantro/data_ops/db_tools.py
--rw-rw-rw-   0 root         (0) root         (0)     9010 2022-12-07 15:32:45.000000 dantro-0.19.0b1/dantro/data_ops/expr_ops.py
--rw-rw-rw-   0 root         (0) root         (0)     3947 2022-12-07 15:32:45.000000 dantro-0.19.0b1/dantro/data_ops/hooks.py
--rw-rw-rw-   0 root         (0) root         (0)    12931 2022-12-07 15:32:45.000000 dantro-0.19.0b1/dantro/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-07 15:32:57.464058 dantro-0.19.0b1/dantro/groups/
--rw-rw-rw-   0 root         (0) root         (0)      601 2022-12-07 15:32:45.000000 dantro-0.19.0b1/dantro/groups/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3497 2022-12-07 15:32:45.000000 dantro-0.19.0b1/dantro/groups/_registry.py
--rw-rw-rw-   0 root         (0) root         (0)     2787 2022-12-07 15:32:45.000000 dantro-0.19.0b1/dantro/groups/dirpath.py
--rw-rw-rw-   0 root         (0) root         (0)    38203 2022-12-07 15:32:45.000000 dantro-0.19.0b1/dantro/groups/graph.py
--rw-rw-rw-   0 root         (0) root         (0)    46441 2022-12-07 15:32:45.000000 dantro-0.19.0b1/dantro/groups/labelled.py
--rw-rw-rw-   0 root         (0) root         (0)     5143 2022-12-07 15:32:45.000000 dantro-0.19.0b1/dantro/groups/ordered.py
--rw-rw-rw-   0 root         (0) root         (0)    25069 2022-12-07 15:32:45.000000 dantro-0.19.0b1/dantro/groups/psp.py
--rw-rw-rw-   0 root         (0) root         (0)     2500 2022-12-07 15:32:45.000000 dantro-0.19.0b1/dantro/groups/time_series.py
--rw-rw-rw-   0 root         (0) root         (0)     1899 2022-12-07 15:32:45.000000 dantro-0.19.0b1/dantro/logging.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-07 15:32:57.465889 dantro-0.19.0b1/dantro/mixins/
--rw-rw-rw-   0 root         (0) root         (0)      613 2022-12-07 15:32:45.000000 dantro-0.19.0b1/dantro/mixins/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    13225 2022-12-07 15:32:45.000000 dantro-0.19.0b1/dantro/mixins/base.py
--rw-rw-rw-   0 root         (0) root         (0)     3054 2022-12-07 15:32:45.000000 dantro-0.19.0b1/dantro/mixins/general.py
--rw-rw-rw-   0 root         (0) root         (0)     6696 2022-12-07 15:32:45.000000 dantro-0.19.0b1/dantro/mixins/indexing.py
--rw-rw-rw-   0 root         (0) root         (0)     7862 2022-12-07 15:32:45.000000 dantro-0.19.0b1/dantro/mixins/numeric.py
--rw-rw-rw-   0 root         (0) root         (0)     7694 2022-12-07 15:32:45.000000 dantro-0.19.0b1/dantro/mixins/proxy_support.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-07 15:32:57.466804 dantro-0.19.0b1/dantro/plot/
--rw-rw-rw-   0 root         (0) root         (0)      295 2022-12-07 15:32:45.000000 dantro-0.19.0b1/dantro/plot/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    10615 2022-12-07 15:32:45.000000 dantro-0.19.0b1/dantro/plot/_cfg.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-07 15:32:57.467719 dantro-0.19.0b1/dantro/plot/creators/
--rw-rw-rw-   0 root         (0) root         (0)      556 2022-12-07 15:32:45.000000 dantro-0.19.0b1/dantro/plot/creators/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    45845 2022-12-07 15:32:45.000000 dantro-0.19.0b1/dantro/plot/creators/base.py
--rw-rw-rw-   0 root         (0) root         (0)    37576 2022-12-07 15:32:45.000000 dantro-0.19.0b1/dantro/plot/creators/psp.py
--rw-rw-rw-   0 root         (0) root         (0)    24018 2022-12-07 15:32:45.000000 dantro-0.19.0b1/dantro/plot/creators/pyplot.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-07 15:32:57.470465 dantro-0.19.0b1/dantro/plot/funcs/
--rw-rw-rw-   0 root         (0) root         (0)      248 2022-12-07 15:32:45.000000 dantro-0.19.0b1/dantro/plot/funcs/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    10598 2022-12-07 15:32:45.000000 dantro-0.19.0b1/dantro/plot/funcs/_multiplot.py
--rw-rw-rw-   0 root         (0) root         (0)     2886 2022-12-07 15:32:45.000000 dantro-0.19.0b1/dantro/plot/funcs/_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     1445 2022-12-07 15:32:45.000000 dantro-0.19.0b1/dantro/plot/funcs/basic.py
--rw-rw-rw-   0 root         (0) root         (0)    53862 2022-12-07 15:32:45.000000 dantro-0.19.0b1/dantro/plot/funcs/generic.py
--rw-rw-rw-   0 root         (0) root         (0)     9313 2022-12-07 15:32:45.000000 dantro-0.19.0b1/dantro/plot/funcs/graph.py
--rw-rw-rw-   0 root         (0) root         (0)     6939 2022-12-07 15:32:45.000000 dantro-0.19.0b1/dantro/plot/funcs/multiplot.py
--rw-rw-rw-   0 root         (0) root         (0)    90282 2022-12-07 15:32:45.000000 dantro-0.19.0b1/dantro/plot/plot_helper.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-07 15:32:57.472296 dantro-0.19.0b1/dantro/plot/utils/
--rw-rw-rw-   0 root         (0) root         (0)      220 2022-12-07 15:32:45.000000 dantro-0.19.0b1/dantro/plot/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3870 2022-12-07 15:32:45.000000 dantro-0.19.0b1/dantro/plot/utils/_file_writer.py
--rw-rw-rw-   0 root         (0) root         (0)    41637 2022-12-07 15:32:45.000000 dantro-0.19.0b1/dantro/plot/utils/color_mngr.py
--rw-rw-rw-   0 root         (0) root         (0)    11757 2022-12-07 15:32:45.000000 dantro-0.19.0b1/dantro/plot/utils/mpl.py
--rw-rw-rw-   0 root         (0) root         (0)    13223 2022-12-07 15:32:45.000000 dantro-0.19.0b1/dantro/plot/utils/plot_func.py
--rw-rw-rw-   0 root         (0) root         (0)    58440 2022-12-07 15:32:45.000000 dantro-0.19.0b1/dantro/plot_mngr.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-07 15:32:57.473211 dantro-0.19.0b1/dantro/proxy/
--rw-rw-rw-   0 root         (0) root         (0)      142 2022-12-07 15:32:45.000000 dantro-0.19.0b1/dantro/proxy/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6545 2022-12-07 15:32:45.000000 dantro-0.19.0b1/dantro/proxy/hdf5.py
--rw-rw-rw-   0 root         (0) root         (0)    23632 2022-12-07 15:32:45.000000 dantro-0.19.0b1/dantro/tools.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-07 15:32:57.474126 dantro-0.19.0b1/dantro/utils/
--rw-rw-rw-   0 root         (0) root         (0)      315 2022-12-07 15:32:45.000000 dantro-0.19.0b1/dantro/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    21012 2022-12-07 15:32:45.000000 dantro-0.19.0b1/dantro/utils/coords.py
--rw-rw-rw-   0 root         (0) root         (0)     7146 2022-12-07 15:32:45.000000 dantro-0.19.0b1/dantro/utils/link.py
--rw-rw-rw-   0 root         (0) root         (0)    15838 2022-12-07 15:32:45.000000 dantro-0.19.0b1/dantro/utils/nx.py
--rw-rw-rw-   0 root         (0) root         (0)    16382 2022-12-07 15:32:45.000000 dantro-0.19.0b1/dantro/utils/ordereddict.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-07 15:32:57.453075 dantro-0.19.0b1/dantro.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3220 2022-12-07 15:32:57.000000 dantro-0.19.0b1/dantro.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2301 2022-12-07 15:32:57.000000 dantro-0.19.0b1/dantro.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-12-07 15:32:57.000000 dantro-0.19.0b1/dantro.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      371 2022-12-07 15:32:57.000000 dantro-0.19.0b1/dantro.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2022-12-07 15:32:57.000000 dantro-0.19.0b1/dantro.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)     1723 2022-12-07 15:32:45.000000 dantro-0.19.0b1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2022-12-07 15:32:57.474126 dantro-0.19.0b1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     6012 2022-12-07 15:32:45.000000 dantro-0.19.0b1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-09 16:49:32.579645 dantro-0.19.0b2/
+-rw-rw-rw-   0 root         (0) root         (0)    35149 2022-12-09 16:49:20.000000 dantro-0.19.0b2/COPYING
+-rw-rw-rw-   0 root         (0) root         (0)     7633 2022-12-09 16:49:20.000000 dantro-0.19.0b2/COPYING.LESSER
+-rw-r--r--   0 root         (0) root         (0)     3220 2022-12-09 16:49:32.579645 dantro-0.19.0b2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)    15686 2022-12-09 16:49:20.000000 dantro-0.19.0b2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-09 16:49:32.555643 dantro-0.19.0b2/dantro/
+-rw-rw-rw-   0 root         (0) root         (0)     1007 2022-12-09 16:49:20.000000 dantro-0.19.0b2/dantro/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      889 2022-12-09 16:49:20.000000 dantro-0.19.0b2/dantro/_copy.py
+-rw-rw-rw-   0 root         (0) root         (0)    30886 2022-12-09 16:49:20.000000 dantro-0.19.0b2/dantro/_dag_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)      922 2022-12-09 16:49:20.000000 dantro-0.19.0b2/dantro/_hash.py
+-rw-rw-rw-   0 root         (0) root         (0)    14740 2022-12-09 16:49:20.000000 dantro-0.19.0b2/dantro/_import_tools.py
+-rw-rw-rw-   0 root         (0) root         (0)     7267 2022-12-09 16:49:20.000000 dantro-0.19.0b2/dantro/_registry.py
+-rw-rw-rw-   0 root         (0) root         (0)     9390 2022-12-09 16:49:20.000000 dantro-0.19.0b2/dantro/_yaml.py
+-rw-rw-rw-   0 root         (0) root         (0)    15796 2022-12-09 16:49:20.000000 dantro-0.19.0b2/dantro/abc.py
+-rw-rw-rw-   0 root         (0) root         (0)    44192 2022-12-09 16:49:20.000000 dantro-0.19.0b2/dantro/base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-09 16:49:32.557643 dantro-0.19.0b2/dantro/cfg/
+-rw-rw-rw-   0 root         (0) root         (0)    22021 2022-12-09 16:49:20.000000 dantro-0.19.0b2/dantro/cfg/base_plots.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-09 16:49:32.559643 dantro-0.19.0b2/dantro/containers/
+-rw-rw-rw-   0 root         (0) root         (0)      545 2022-12-09 16:49:20.000000 dantro-0.19.0b2/dantro/containers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3675 2022-12-09 16:49:20.000000 dantro-0.19.0b2/dantro/containers/_registry.py
+-rw-rw-rw-   0 root         (0) root         (0)     3223 2022-12-09 16:49:20.000000 dantro-0.19.0b2/dantro/containers/general.py
+-rw-rw-rw-   0 root         (0) root         (0)     1302 2022-12-09 16:49:20.000000 dantro-0.19.0b2/dantro/containers/link.py
+-rw-rw-rw-   0 root         (0) root         (0)     3409 2022-12-09 16:49:20.000000 dantro-0.19.0b2/dantro/containers/numeric.py
+-rw-rw-rw-   0 root         (0) root         (0)     3489 2022-12-09 16:49:20.000000 dantro-0.19.0b2/dantro/containers/path.py
+-rw-rw-rw-   0 root         (0) root         (0)    13561 2022-12-09 16:49:20.000000 dantro-0.19.0b2/dantro/containers/xr.py
+-rw-rw-rw-   0 root         (0) root         (0)   131976 2022-12-09 16:49:20.000000 dantro-0.19.0b2/dantro/dag.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-09 16:49:32.562644 dantro-0.19.0b2/dantro/data_loaders/
+-rw-rw-rw-   0 root         (0) root         (0)     2963 2022-12-09 16:49:20.000000 dantro-0.19.0b2/dantro/data_loaders/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6739 2022-12-09 16:49:20.000000 dantro-0.19.0b2/dantro/data_loaders/_registry.py
+-rw-rw-rw-   0 root         (0) root         (0)     3786 2022-12-09 16:49:20.000000 dantro-0.19.0b2/dantro/data_loaders/fspath.py
+-rw-rw-rw-   0 root         (0) root         (0)    19584 2022-12-09 16:49:20.000000 dantro-0.19.0b2/dantro/data_loaders/hdf5.py
+-rw-rw-rw-   0 root         (0) root         (0)     2009 2022-12-09 16:49:20.000000 dantro-0.19.0b2/dantro/data_loaders/numpy.py
+-rw-rw-rw-   0 root         (0) root         (0)     4230 2022-12-09 16:49:20.000000 dantro-0.19.0b2/dantro/data_loaders/pandas.py
+-rw-rw-rw-   0 root         (0) root         (0)     1180 2022-12-09 16:49:20.000000 dantro-0.19.0b2/dantro/data_loaders/pickle.py
+-rw-rw-rw-   0 root         (0) root         (0)      993 2022-12-09 16:49:20.000000 dantro-0.19.0b2/dantro/data_loaders/text.py
+-rw-rw-rw-   0 root         (0) root         (0)     3442 2022-12-09 16:49:20.000000 dantro-0.19.0b2/dantro/data_loaders/xarray.py
+-rw-rw-rw-   0 root         (0) root         (0)     2165 2022-12-09 16:49:20.000000 dantro-0.19.0b2/dantro/data_loaders/yaml.py
+-rw-rw-rw-   0 root         (0) root         (0)    64943 2022-12-09 16:49:20.000000 dantro-0.19.0b2/dantro/data_mngr.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-09 16:49:32.565644 dantro-0.19.0b2/dantro/data_ops/
+-rw-rw-rw-   0 root         (0) root         (0)      454 2022-12-09 16:49:20.000000 dantro-0.19.0b2/dantro/data_ops/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      979 2022-12-09 16:49:20.000000 dantro-0.19.0b2/dantro/data_ops/_base_ops.py
+-rw-rw-rw-   0 root         (0) root         (0)     2807 2022-12-09 16:49:20.000000 dantro-0.19.0b2/dantro/data_ops/apply.py
+-rw-rw-rw-   0 root         (0) root         (0)    28398 2022-12-09 16:49:20.000000 dantro-0.19.0b2/dantro/data_ops/arr_ops.py
+-rw-rw-rw-   0 root         (0) root         (0)     2716 2022-12-09 16:49:20.000000 dantro-0.19.0b2/dantro/data_ops/ctrl_ops.py
+-rw-rw-rw-   0 root         (0) root         (0)    16685 2022-12-09 16:49:20.000000 dantro-0.19.0b2/dantro/data_ops/db.py
+-rw-rw-rw-   0 root         (0) root         (0)     8250 2022-12-09 16:49:20.000000 dantro-0.19.0b2/dantro/data_ops/db_tools.py
+-rw-rw-rw-   0 root         (0) root         (0)     9010 2022-12-09 16:49:20.000000 dantro-0.19.0b2/dantro/data_ops/expr_ops.py
+-rw-rw-rw-   0 root         (0) root         (0)     3947 2022-12-09 16:49:20.000000 dantro-0.19.0b2/dantro/data_ops/hooks.py
+-rw-rw-rw-   0 root         (0) root         (0)    12931 2022-12-09 16:49:20.000000 dantro-0.19.0b2/dantro/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-09 16:49:32.568644 dantro-0.19.0b2/dantro/groups/
+-rw-rw-rw-   0 root         (0) root         (0)      601 2022-12-09 16:49:20.000000 dantro-0.19.0b2/dantro/groups/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3497 2022-12-09 16:49:20.000000 dantro-0.19.0b2/dantro/groups/_registry.py
+-rw-rw-rw-   0 root         (0) root         (0)     2787 2022-12-09 16:49:20.000000 dantro-0.19.0b2/dantro/groups/dirpath.py
+-rw-rw-rw-   0 root         (0) root         (0)    38203 2022-12-09 16:49:20.000000 dantro-0.19.0b2/dantro/groups/graph.py
+-rw-rw-rw-   0 root         (0) root         (0)    46441 2022-12-09 16:49:20.000000 dantro-0.19.0b2/dantro/groups/labelled.py
+-rw-rw-rw-   0 root         (0) root         (0)     5143 2022-12-09 16:49:20.000000 dantro-0.19.0b2/dantro/groups/ordered.py
+-rw-rw-rw-   0 root         (0) root         (0)    25069 2022-12-09 16:49:20.000000 dantro-0.19.0b2/dantro/groups/psp.py
+-rw-rw-rw-   0 root         (0) root         (0)     2500 2022-12-09 16:49:20.000000 dantro-0.19.0b2/dantro/groups/time_series.py
+-rw-rw-rw-   0 root         (0) root         (0)     1899 2022-12-09 16:49:20.000000 dantro-0.19.0b2/dantro/logging.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-09 16:49:32.570644 dantro-0.19.0b2/dantro/mixins/
+-rw-rw-rw-   0 root         (0) root         (0)      613 2022-12-09 16:49:20.000000 dantro-0.19.0b2/dantro/mixins/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    13225 2022-12-09 16:49:20.000000 dantro-0.19.0b2/dantro/mixins/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     3054 2022-12-09 16:49:20.000000 dantro-0.19.0b2/dantro/mixins/general.py
+-rw-rw-rw-   0 root         (0) root         (0)     6696 2022-12-09 16:49:20.000000 dantro-0.19.0b2/dantro/mixins/indexing.py
+-rw-rw-rw-   0 root         (0) root         (0)     7862 2022-12-09 16:49:20.000000 dantro-0.19.0b2/dantro/mixins/numeric.py
+-rw-rw-rw-   0 root         (0) root         (0)     7694 2022-12-09 16:49:20.000000 dantro-0.19.0b2/dantro/mixins/proxy_support.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-09 16:49:32.571644 dantro-0.19.0b2/dantro/plot/
+-rw-rw-rw-   0 root         (0) root         (0)      295 2022-12-09 16:49:20.000000 dantro-0.19.0b2/dantro/plot/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    10615 2022-12-09 16:49:20.000000 dantro-0.19.0b2/dantro/plot/_cfg.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-09 16:49:32.572644 dantro-0.19.0b2/dantro/plot/creators/
+-rw-rw-rw-   0 root         (0) root         (0)      556 2022-12-09 16:49:20.000000 dantro-0.19.0b2/dantro/plot/creators/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    45845 2022-12-09 16:49:20.000000 dantro-0.19.0b2/dantro/plot/creators/base.py
+-rw-rw-rw-   0 root         (0) root         (0)    37576 2022-12-09 16:49:20.000000 dantro-0.19.0b2/dantro/plot/creators/psp.py
+-rw-rw-rw-   0 root         (0) root         (0)    24018 2022-12-09 16:49:20.000000 dantro-0.19.0b2/dantro/plot/creators/pyplot.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-09 16:49:32.575645 dantro-0.19.0b2/dantro/plot/funcs/
+-rw-rw-rw-   0 root         (0) root         (0)      248 2022-12-09 16:49:20.000000 dantro-0.19.0b2/dantro/plot/funcs/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    10598 2022-12-09 16:49:20.000000 dantro-0.19.0b2/dantro/plot/funcs/_multiplot.py
+-rw-rw-rw-   0 root         (0) root         (0)     2886 2022-12-09 16:49:20.000000 dantro-0.19.0b2/dantro/plot/funcs/_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     1445 2022-12-09 16:49:20.000000 dantro-0.19.0b2/dantro/plot/funcs/basic.py
+-rw-rw-rw-   0 root         (0) root         (0)    53862 2022-12-09 16:49:20.000000 dantro-0.19.0b2/dantro/plot/funcs/generic.py
+-rw-rw-rw-   0 root         (0) root         (0)     9313 2022-12-09 16:49:20.000000 dantro-0.19.0b2/dantro/plot/funcs/graph.py
+-rw-rw-rw-   0 root         (0) root         (0)     6939 2022-12-09 16:49:20.000000 dantro-0.19.0b2/dantro/plot/funcs/multiplot.py
+-rw-rw-rw-   0 root         (0) root         (0)    90282 2022-12-09 16:49:20.000000 dantro-0.19.0b2/dantro/plot/plot_helper.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-09 16:49:32.576645 dantro-0.19.0b2/dantro/plot/utils/
+-rw-rw-rw-   0 root         (0) root         (0)      220 2022-12-09 16:49:20.000000 dantro-0.19.0b2/dantro/plot/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3870 2022-12-09 16:49:20.000000 dantro-0.19.0b2/dantro/plot/utils/_file_writer.py
+-rw-rw-rw-   0 root         (0) root         (0)    41637 2022-12-09 16:49:20.000000 dantro-0.19.0b2/dantro/plot/utils/color_mngr.py
+-rw-rw-rw-   0 root         (0) root         (0)    11757 2022-12-09 16:49:20.000000 dantro-0.19.0b2/dantro/plot/utils/mpl.py
+-rw-rw-rw-   0 root         (0) root         (0)    13223 2022-12-09 16:49:20.000000 dantro-0.19.0b2/dantro/plot/utils/plot_func.py
+-rw-rw-rw-   0 root         (0) root         (0)    58440 2022-12-09 16:49:20.000000 dantro-0.19.0b2/dantro/plot_mngr.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-09 16:49:32.577645 dantro-0.19.0b2/dantro/proxy/
+-rw-rw-rw-   0 root         (0) root         (0)      142 2022-12-09 16:49:20.000000 dantro-0.19.0b2/dantro/proxy/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6545 2022-12-09 16:49:20.000000 dantro-0.19.0b2/dantro/proxy/hdf5.py
+-rw-rw-rw-   0 root         (0) root         (0)    23632 2022-12-09 16:49:20.000000 dantro-0.19.0b2/dantro/tools.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-09 16:49:32.579645 dantro-0.19.0b2/dantro/utils/
+-rw-rw-rw-   0 root         (0) root         (0)      315 2022-12-09 16:49:20.000000 dantro-0.19.0b2/dantro/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    21012 2022-12-09 16:49:20.000000 dantro-0.19.0b2/dantro/utils/coords.py
+-rw-rw-rw-   0 root         (0) root         (0)     7146 2022-12-09 16:49:20.000000 dantro-0.19.0b2/dantro/utils/link.py
+-rw-rw-rw-   0 root         (0) root         (0)    15838 2022-12-09 16:49:20.000000 dantro-0.19.0b2/dantro/utils/nx.py
+-rw-rw-rw-   0 root         (0) root         (0)    16382 2022-12-09 16:49:20.000000 dantro-0.19.0b2/dantro/utils/ordereddict.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-09 16:49:32.556643 dantro-0.19.0b2/dantro.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3220 2022-12-09 16:49:32.000000 dantro-0.19.0b2/dantro.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2301 2022-12-09 16:49:32.000000 dantro-0.19.0b2/dantro.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-12-09 16:49:32.000000 dantro-0.19.0b2/dantro.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      371 2022-12-09 16:49:32.000000 dantro-0.19.0b2/dantro.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2022-12-09 16:49:32.000000 dantro-0.19.0b2/dantro.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1723 2022-12-09 16:49:20.000000 dantro-0.19.0b2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2022-12-09 16:49:32.579645 dantro-0.19.0b2/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     6012 2022-12-09 16:49:20.000000 dantro-0.19.0b2/setup.py
```

### Comparing `dantro-0.19.0b1/COPYING` & `dantro-0.19.0b2/COPYING`

 * *Files identical despite different names*

### Comparing `dantro-0.19.0b1/COPYING.LESSER` & `dantro-0.19.0b2/COPYING.LESSER`

 * *Files identical despite different names*

### Comparing `dantro-0.19.0b1/PKG-INFO` & `dantro-0.19.0b2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dantro
-Version: 0.19.0b1
+Version: 0.19.0b2
 Summary: Handle, transform, and visualize hierarchically structured data
 Home-page: https://gitlab.com/utopia-project/dantro
 Author: dantro developers
 Author-email: dantro-dev@iup.uni.heidelberg.de
 License: LGPL-3.0-or-later
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `dantro-0.19.0b1/README.md` & `dantro-0.19.0b2/README.md`

 * *Files identical despite different names*

### Comparing `dantro-0.19.0b1/dantro/__init__.py` & `dantro-0.19.0b2/dantro/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 Together, these stages constitute a **data processing pipeline**:
 an automated sequence of predefined, configurable operations.
 
 See :ref:`the user manual <welcome>` for more information.
 """
 
-__version__ = "0.19.0b1"
+__version__ = "0.19.0b2"
 """Package version"""
 
 # Set up the root logger such that the logging configuration is applied
 from .logging import getLogger as _getLogger
 
 _log = _getLogger(__name__)
```

### Comparing `dantro-0.19.0b1/dantro/_copy.py` & `dantro-0.19.0b2/dantro/_copy.py`

 * *Files identical despite different names*

### Comparing `dantro-0.19.0b1/dantro/_dag_utils.py` & `dantro-0.19.0b2/dantro/_dag_utils.py`

 * *Files identical despite different names*

### Comparing `dantro-0.19.0b1/dantro/_hash.py` & `dantro-0.19.0b2/dantro/_hash.py`

 * *Files identical despite different names*

### Comparing `dantro-0.19.0b1/dantro/_import_tools.py` & `dantro-0.19.0b2/dantro/_import_tools.py`

 * *Files identical despite different names*

### Comparing `dantro-0.19.0b1/dantro/_registry.py` & `dantro-0.19.0b2/dantro/_registry.py`

 * *Files identical despite different names*

### Comparing `dantro-0.19.0b1/dantro/_yaml.py` & `dantro-0.19.0b2/dantro/_yaml.py`

 * *Files identical despite different names*

### Comparing `dantro-0.19.0b1/dantro/abc.py` & `dantro-0.19.0b2/dantro/abc.py`

 * *Files identical despite different names*

### Comparing `dantro-0.19.0b1/dantro/base.py` & `dantro-0.19.0b2/dantro/base.py`

 * *Files identical despite different names*

### Comparing `dantro-0.19.0b1/dantro/cfg/base_plots.yml` & `dantro-0.19.0b2/dantro/cfg/base_plots.yml`

 * *Files identical despite different names*

### Comparing `dantro-0.19.0b1/dantro/containers/__init__.py` & `dantro-0.19.0b2/dantro/containers/__init__.py`

 * *Files identical despite different names*

### Comparing `dantro-0.19.0b1/dantro/containers/_registry.py` & `dantro-0.19.0b2/dantro/containers/_registry.py`

 * *Files identical despite different names*

### Comparing `dantro-0.19.0b1/dantro/containers/general.py` & `dantro-0.19.0b2/dantro/containers/general.py`

 * *Files identical despite different names*

### Comparing `dantro-0.19.0b1/dantro/containers/link.py` & `dantro-0.19.0b2/dantro/containers/link.py`

 * *Files identical despite different names*

### Comparing `dantro-0.19.0b1/dantro/containers/numeric.py` & `dantro-0.19.0b2/dantro/containers/numeric.py`

 * *Files identical despite different names*

### Comparing `dantro-0.19.0b1/dantro/containers/path.py` & `dantro-0.19.0b2/dantro/containers/path.py`

 * *Files identical despite different names*

### Comparing `dantro-0.19.0b1/dantro/containers/xr.py` & `dantro-0.19.0b2/dantro/containers/xr.py`

 * *Files identical despite different names*

### Comparing `dantro-0.19.0b1/dantro/dag.py` & `dantro-0.19.0b2/dantro/dag.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,25 @@
 import os
 import pickle as _pickle
 import sys
 import time
 import warnings
 from collections import defaultdict as _defaultdict
 from itertools import chain
-from typing import Any, Callable, Dict, List, Sequence, Set, Tuple, Union
+from typing import (
+    Any,
+    Callable,
+    Dict,
+    List,
+    Optional,
+    Sequence,
+    Set,
+    Tuple,
+    Union,
+)
 
 import numpy as np
 from paramspace.tools import recursive_collect, recursive_replace
 
 from ._copy import _deepcopy, _shallowcopy
 from ._dag_utils import DAGMetaOperationTag as _MOpTag
 from ._dag_utils import DAGNode, DAGObjects, DAGReference, DAGTag
@@ -809,21 +819,23 @@
 
         .. note::
 
             Unlike the more general :py:meth:`._lookup_result`, this one does
             not check whether reading from cache is enabled or disabled.
         """
         read_opts = self._fc_opts.get("read", {})
+        always_from_file = read_opts.get("always", False)
         load_opts = read_opts.get("load_options", {})
+
         t0 = time.time()
 
         # Let the DAG check if there is a file cache, i.e. if a file with
         # this Transformation's hash exists in the DAG's cache directory.
         success, res = self.dag._retrieve_from_cache_file(
-            self.hashstr, **load_opts
+            self.hashstr, always_from_file=always_from_file, **load_opts
         )
 
         # Store the result in the memory cache
         if success:
             self.status = "looked_up"
 
         self._update_profile(cache_lookup=(time.time() - t0))
@@ -844,15 +856,18 @@
             storage_options: dict = None,
         ) -> bool:
             """A helper function to evaluate _whether_ the file cache is to be
             written or not.
 
             Args:
                 enabled (bool): Whether writing is enabled at all
-                always (bool, optional): If given, will always write.
+                always (bool, optional): If given, will not evaluate other
+                    conditions but always write, *unless* a cache file already
+                    exists. Set ``allow_overwrite`` to always overwrite an
+                    existing cache file.
                 allow_overwrite (bool, optional): If False, will not write a
                     cache file if one already exists. If True, a cache file
                     _might_ be written, although one already exists. This is
                     still conditional on the evaluation of the other arguments.
                 min_size (int, optional): The minimum size of the result object
                     that allows writing the cache.
                 max_size (int, optional): The maximum size of the result object
@@ -872,16 +887,24 @@
             Returns:
                 bool: Whether to write the file cache or not.
             """
             if not enabled:
                 # ... nothing else to check
                 return False
 
-            # With always: always write, don't look at other arguments.
+            # Some evaluations depend on whether a cache file already exists
+            file_exists = self.hashstr in self.dag.cache_files
+
+            # With always: always write (skip other conditions), but do not
+            # _overwrite_ a potentially existing file.
             if always:
+                if file_exists and not allow_overwrite:
+                    return False
+
+                # "always overwrite" --> no further checks needed
                 return True
             # All checks below are formulated such that they return False.
 
             # If overwriting is _disabled_ and a cache file already exists, it
             # is already clear that a new one should _not_ be written
             if not allow_overwrite and self.hashstr in self.dag.cache_files:
                 return False
@@ -2947,37 +2970,53 @@
 
     # .........................................................................
     # Cache writing and reading
     # NOTE This is done here rather than in Transformation because this is the
     #      more central entity and it is a bit easier ...
 
     def _retrieve_from_cache_file(
-        self, trf_hash: str, **load_kwargs
+        self,
+        trf_hash: str,
+        *,
+        always_from_file: bool = False,
+        unpack: Optional[bool] = None,
+        **load_kwargs,
     ) -> Tuple[bool, Any]:
         """Retrieves a transformation's result from a cache file and stores it
         in the data manager's cache group.
 
         .. note::
 
             If a file was already loaded from the cache, it will not be loaded
             again. Thus, the DataManager acts as a persistent storage for
             loaded cache files. Consequently, these are shared among all
             TransformationDAG objects.
+
+        Args:
+            trf_hash (str): The hash to use for lookup
+            always_from_file (bool, optional): If set, will always load from
+                file instead of using a potentially existing already loaded
+                object in the data manager.
+            unpack (Optional[bool], optional): Whether to unpack the data from
+                the container. If None, will only do so for certain types, see
+                :py:data:`.DAG_CACHE_CONTAINER_TYPES_TO_UNPACK`.
+            **load_kwargs: Passed on to load function of associated DataManager
         """
         success, res = False, None
 
         # Check if the file was already loaded; only go through the trouble of
         # checking all the hash files and invoking the load method if the
         # desired cache file was really not loaded
-        try:
-            res = self.dm[DAG_CACHE_DM_PATH][trf_hash]
-        except ItemAccessError:
-            pass
-        else:
-            success = True
+        if not always_from_file:
+            try:
+                res = self.dm[DAG_CACHE_DM_PATH][trf_hash]
+            except ItemAccessError:
+                pass
+            else:
+                success = True
 
         if not success:
             cache_files = self.cache_files
 
             if trf_hash not in cache_files.keys():
                 # Bad luck, no cache file
                 log.trace("No cache file found for %s.", trf_hash)
@@ -3002,16 +3041,19 @@
                     **load_kwargs,
                 )
 
             # Can now retrieve the loaded data
             res = self.dm[DAG_CACHE_DM_PATH][trf_hash]
             success = True
 
-        # Have to unpack some container types
-        if isinstance(res, DAG_CACHE_CONTAINER_TYPES_TO_UNPACK):
+        # Have to / may want to unpack some container types
+        if unpack is True or (
+            unpack is None
+            and isinstance(res, DAG_CACHE_CONTAINER_TYPES_TO_UNPACK)
+        ):
             res = res.data
 
         # Done.
         return success, res
 
     def _write_to_cache_file(
         self,
```

### Comparing `dantro-0.19.0b1/dantro/data_loaders/__init__.py` & `dantro-0.19.0b2/dantro/data_loaders/__init__.py`

 * *Files identical despite different names*

### Comparing `dantro-0.19.0b1/dantro/data_loaders/_registry.py` & `dantro-0.19.0b2/dantro/data_loaders/_registry.py`

 * *Files identical despite different names*

### Comparing `dantro-0.19.0b1/dantro/data_loaders/fspath.py` & `dantro-0.19.0b2/dantro/data_loaders/fspath.py`

 * *Files identical despite different names*

### Comparing `dantro-0.19.0b1/dantro/data_loaders/hdf5.py` & `dantro-0.19.0b2/dantro/data_loaders/hdf5.py`

 * *Files identical despite different names*

### Comparing `dantro-0.19.0b1/dantro/data_loaders/numpy.py` & `dantro-0.19.0b2/dantro/data_loaders/numpy.py`

 * *Files identical despite different names*

### Comparing `dantro-0.19.0b1/dantro/data_loaders/pandas.py` & `dantro-0.19.0b2/dantro/data_loaders/pandas.py`

 * *Files identical despite different names*

### Comparing `dantro-0.19.0b1/dantro/data_loaders/pickle.py` & `dantro-0.19.0b2/dantro/data_loaders/pickle.py`

 * *Files identical despite different names*

### Comparing `dantro-0.19.0b1/dantro/data_loaders/text.py` & `dantro-0.19.0b2/dantro/data_loaders/text.py`

 * *Files identical despite different names*

### Comparing `dantro-0.19.0b1/dantro/data_loaders/xarray.py` & `dantro-0.19.0b2/dantro/data_loaders/xarray.py`

 * *Files identical despite different names*

### Comparing `dantro-0.19.0b1/dantro/data_loaders/yaml.py` & `dantro-0.19.0b2/dantro/data_loaders/yaml.py`

 * *Files identical despite different names*

### Comparing `dantro-0.19.0b1/dantro/data_mngr.py` & `dantro-0.19.0b2/dantro/data_mngr.py`

 * *Files identical despite different names*

### Comparing `dantro-0.19.0b1/dantro/data_ops/_base_ops.py` & `dantro-0.19.0b2/dantro/data_ops/_base_ops.py`

 * *Files identical despite different names*

### Comparing `dantro-0.19.0b1/dantro/data_ops/apply.py` & `dantro-0.19.0b2/dantro/data_ops/apply.py`

 * *Files identical despite different names*

### Comparing `dantro-0.19.0b1/dantro/data_ops/arr_ops.py` & `dantro-0.19.0b2/dantro/data_ops/arr_ops.py`

 * *Files identical despite different names*

### Comparing `dantro-0.19.0b1/dantro/data_ops/ctrl_ops.py` & `dantro-0.19.0b2/dantro/data_ops/ctrl_ops.py`

 * *Files identical despite different names*

### Comparing `dantro-0.19.0b1/dantro/data_ops/db.py` & `dantro-0.19.0b2/dantro/data_ops/db.py`

 * *Files identical despite different names*

### Comparing `dantro-0.19.0b1/dantro/data_ops/db_tools.py` & `dantro-0.19.0b2/dantro/data_ops/db_tools.py`

 * *Files identical despite different names*

### Comparing `dantro-0.19.0b1/dantro/data_ops/expr_ops.py` & `dantro-0.19.0b2/dantro/data_ops/expr_ops.py`

 * *Files identical despite different names*

### Comparing `dantro-0.19.0b1/dantro/data_ops/hooks.py` & `dantro-0.19.0b2/dantro/data_ops/hooks.py`

 * *Files identical despite different names*

### Comparing `dantro-0.19.0b1/dantro/exceptions.py` & `dantro-0.19.0b2/dantro/exceptions.py`

 * *Files identical despite different names*

### Comparing `dantro-0.19.0b1/dantro/groups/__init__.py` & `dantro-0.19.0b2/dantro/groups/__init__.py`

 * *Files identical despite different names*

### Comparing `dantro-0.19.0b1/dantro/groups/_registry.py` & `dantro-0.19.0b2/dantro/groups/_registry.py`

 * *Files identical despite different names*

### Comparing `dantro-0.19.0b1/dantro/groups/dirpath.py` & `dantro-0.19.0b2/dantro/groups/dirpath.py`

 * *Files identical despite different names*

### Comparing `dantro-0.19.0b1/dantro/groups/graph.py` & `dantro-0.19.0b2/dantro/groups/graph.py`

 * *Files identical despite different names*

### Comparing `dantro-0.19.0b1/dantro/groups/labelled.py` & `dantro-0.19.0b2/dantro/groups/labelled.py`

 * *Files identical despite different names*

### Comparing `dantro-0.19.0b1/dantro/groups/ordered.py` & `dantro-0.19.0b2/dantro/groups/ordered.py`

 * *Files identical despite different names*

### Comparing `dantro-0.19.0b1/dantro/groups/psp.py` & `dantro-0.19.0b2/dantro/groups/psp.py`

 * *Files identical despite different names*

### Comparing `dantro-0.19.0b1/dantro/groups/time_series.py` & `dantro-0.19.0b2/dantro/groups/time_series.py`

 * *Files identical despite different names*

### Comparing `dantro-0.19.0b1/dantro/logging.py` & `dantro-0.19.0b2/dantro/logging.py`

 * *Files identical despite different names*

### Comparing `dantro-0.19.0b1/dantro/mixins/__init__.py` & `dantro-0.19.0b2/dantro/mixins/__init__.py`

 * *Files identical despite different names*

### Comparing `dantro-0.19.0b1/dantro/mixins/base.py` & `dantro-0.19.0b2/dantro/mixins/base.py`

 * *Files identical despite different names*

### Comparing `dantro-0.19.0b1/dantro/mixins/general.py` & `dantro-0.19.0b2/dantro/mixins/general.py`

 * *Files identical despite different names*

### Comparing `dantro-0.19.0b1/dantro/mixins/indexing.py` & `dantro-0.19.0b2/dantro/mixins/indexing.py`

 * *Files identical despite different names*

### Comparing `dantro-0.19.0b1/dantro/mixins/numeric.py` & `dantro-0.19.0b2/dantro/mixins/numeric.py`

 * *Files identical despite different names*

### Comparing `dantro-0.19.0b1/dantro/mixins/proxy_support.py` & `dantro-0.19.0b2/dantro/mixins/proxy_support.py`

 * *Files identical despite different names*

### Comparing `dantro-0.19.0b1/dantro/plot/_cfg.py` & `dantro-0.19.0b2/dantro/plot/_cfg.py`

 * *Files identical despite different names*

### Comparing `dantro-0.19.0b1/dantro/plot/creators/__init__.py` & `dantro-0.19.0b2/dantro/plot/creators/__init__.py`

 * *Files identical despite different names*

### Comparing `dantro-0.19.0b1/dantro/plot/creators/base.py` & `dantro-0.19.0b2/dantro/plot/creators/base.py`

 * *Files identical despite different names*

### Comparing `dantro-0.19.0b1/dantro/plot/creators/psp.py` & `dantro-0.19.0b2/dantro/plot/creators/psp.py`

 * *Files identical despite different names*

### Comparing `dantro-0.19.0b1/dantro/plot/creators/pyplot.py` & `dantro-0.19.0b2/dantro/plot/creators/pyplot.py`

 * *Files identical despite different names*

### Comparing `dantro-0.19.0b1/dantro/plot/funcs/_multiplot.py` & `dantro-0.19.0b2/dantro/plot/funcs/_multiplot.py`

 * *Files identical despite different names*

### Comparing `dantro-0.19.0b1/dantro/plot/funcs/_utils.py` & `dantro-0.19.0b2/dantro/plot/funcs/_utils.py`

 * *Files identical despite different names*

### Comparing `dantro-0.19.0b1/dantro/plot/funcs/basic.py` & `dantro-0.19.0b2/dantro/plot/funcs/basic.py`

 * *Files identical despite different names*

### Comparing `dantro-0.19.0b1/dantro/plot/funcs/generic.py` & `dantro-0.19.0b2/dantro/plot/funcs/generic.py`

 * *Files identical despite different names*

### Comparing `dantro-0.19.0b1/dantro/plot/funcs/graph.py` & `dantro-0.19.0b2/dantro/plot/funcs/graph.py`

 * *Files identical despite different names*

### Comparing `dantro-0.19.0b1/dantro/plot/funcs/multiplot.py` & `dantro-0.19.0b2/dantro/plot/funcs/multiplot.py`

 * *Files identical despite different names*

### Comparing `dantro-0.19.0b1/dantro/plot/plot_helper.py` & `dantro-0.19.0b2/dantro/plot/plot_helper.py`

 * *Files identical despite different names*

### Comparing `dantro-0.19.0b1/dantro/plot/utils/_file_writer.py` & `dantro-0.19.0b2/dantro/plot/utils/_file_writer.py`

 * *Files identical despite different names*

### Comparing `dantro-0.19.0b1/dantro/plot/utils/color_mngr.py` & `dantro-0.19.0b2/dantro/plot/utils/color_mngr.py`

 * *Files identical despite different names*

### Comparing `dantro-0.19.0b1/dantro/plot/utils/mpl.py` & `dantro-0.19.0b2/dantro/plot/utils/mpl.py`

 * *Files identical despite different names*

### Comparing `dantro-0.19.0b1/dantro/plot/utils/plot_func.py` & `dantro-0.19.0b2/dantro/plot/utils/plot_func.py`

 * *Files identical despite different names*

### Comparing `dantro-0.19.0b1/dantro/plot_mngr.py` & `dantro-0.19.0b2/dantro/plot_mngr.py`

 * *Files identical despite different names*

### Comparing `dantro-0.19.0b1/dantro/proxy/hdf5.py` & `dantro-0.19.0b2/dantro/proxy/hdf5.py`

 * *Files identical despite different names*

### Comparing `dantro-0.19.0b1/dantro/tools.py` & `dantro-0.19.0b2/dantro/tools.py`

 * *Files identical despite different names*

### Comparing `dantro-0.19.0b1/dantro/utils/coords.py` & `dantro-0.19.0b2/dantro/utils/coords.py`

 * *Files identical despite different names*

### Comparing `dantro-0.19.0b1/dantro/utils/link.py` & `dantro-0.19.0b2/dantro/utils/link.py`

 * *Files identical despite different names*

### Comparing `dantro-0.19.0b1/dantro/utils/nx.py` & `dantro-0.19.0b2/dantro/utils/nx.py`

 * *Files identical despite different names*

### Comparing `dantro-0.19.0b1/dantro/utils/ordereddict.py` & `dantro-0.19.0b2/dantro/utils/ordereddict.py`

 * *Files identical despite different names*

### Comparing `dantro-0.19.0b1/dantro.egg-info/PKG-INFO` & `dantro-0.19.0b2/dantro.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dantro
-Version: 0.19.0b1
+Version: 0.19.0b2
 Summary: Handle, transform, and visualize hierarchically structured data
 Home-page: https://gitlab.com/utopia-project/dantro
 Author: dantro developers
 Author-email: dantro-dev@iup.uni.heidelberg.de
 License: LGPL-3.0-or-later
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `dantro-0.19.0b1/dantro.egg-info/SOURCES.txt` & `dantro-0.19.0b2/dantro.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dantro-0.19.0b1/pyproject.toml` & `dantro-0.19.0b2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dantro-0.19.0b1/setup.py` & `dantro-0.19.0b2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     "pooch",
     "cftime",
 ]
 
 # Dependencies for building the dantro documentation
 doc_deps = [
     "sphinx==4.*",
-    "sphinx-book-theme>=0.3.*",
+    "sphinx-book-theme==0.3.*",
     "sphinx-togglebutton",
     "ipython",
 ]
 
 # .............................................................................
 
 DESCRIPTION = "Handle, transform, and visualize hierarchically structured data"
```

