# Comparing `tmp/experiment-utilities-0.3.3.tar.gz` & `tmp/experiment-utilities-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/experiment-utilities-0.3.3.tar", last modified: Thu Jan 12 12:25:35 2023, max compression
+gzip compressed data, was "dist/experiment-utilities-0.3.4.tar", last modified: Sat Jul  8 08:39:33 2023, max compression
```

## Comparing `experiment-utilities-0.3.3.tar` & `experiment-utilities-0.3.4.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 creinke  (661016) perception (50060)        0 2023-01-12 12:25:35.000000 experiment-utilities-0.3.3/
-drwxr-xr-x   0 creinke  (661016) perception (50060)        0 2023-01-12 12:25:35.000000 experiment-utilities-0.3.3/exputils/
--rw-r--r--   0 creinke  (661016) perception (50060)     1029 2023-01-12 11:08:42.000000 experiment-utilities-0.3.3/exputils/__init__.py
-drwxr-xr-x   0 creinke  (661016) perception (50060)        0 2023-01-12 12:25:35.000000 experiment-utilities-0.3.3/exputils/manage/
--rw-r--r--   0 creinke  (661016) perception (50060)      666 2023-01-11 12:41:01.000000 experiment-utilities-0.3.3/exputils/manage/__init__.py
--rw-r--r--   0 creinke  (661016) perception (50060)    10821 2023-01-11 12:41:01.000000 experiment-utilities-0.3.3/exputils/manage/experimentstarter.py
--rw-r--r--   0 creinke  (661016) perception (50060)    18311 2023-01-11 12:41:01.000000 experiment-utilities-0.3.3/exputils/manage/experimentgenerator.py
-drwxr-xr-x   0 creinke  (661016) perception (50060)        0 2023-01-12 12:25:35.000000 experiment-utilities-0.3.3/exputils/data/
--rw-r--r--   0 creinke  (661016) perception (50060)      727 2023-01-11 12:41:01.000000 experiment-utilities-0.3.3/exputils/data/utils.py
--rw-r--r--   0 creinke  (661016) perception (50060)      951 2023-01-11 12:41:01.000000 experiment-utilities-0.3.3/exputils/data/__init__.py
--rw-r--r--   0 creinke  (661016) perception (50060)    12904 2023-01-11 12:41:01.000000 experiment-utilities-0.3.3/exputils/data/statistics.py
--rw-r--r--   0 creinke  (661016) perception (50060)    18960 2023-01-11 12:41:01.000000 experiment-utilities-0.3.3/exputils/data/loading.py
--rw-r--r--   0 creinke  (661016) perception (50060)     9183 2023-01-12 10:59:20.000000 experiment-utilities-0.3.3/exputils/data/logging.py
--rw-r--r--   0 creinke  (661016) perception (50060)    11066 2023-01-12 11:04:03.000000 experiment-utilities-0.3.3/exputils/data/logger.py
--rw-r--r--   0 creinke  (661016) perception (50060)    18966 2023-01-11 12:41:01.000000 experiment-utilities-0.3.3/exputils/data/selection.py
-drwxr-xr-x   0 creinke  (661016) perception (50060)        0 2023-01-12 12:25:35.000000 experiment-utilities-0.3.3/exputils/misc/
--rw-r--r--   0 creinke  (661016) perception (50060)     1004 2023-01-11 12:41:01.000000 experiment-utilities-0.3.3/exputils/misc/__init__.py
--rw-r--r--   0 creinke  (661016) perception (50060)    21415 2023-01-11 12:41:01.000000 experiment-utilities-0.3.3/exputils/misc/attrdict.py
--rw-r--r--   0 creinke  (661016) perception (50060)    18731 2023-01-11 12:41:01.000000 experiment-utilities-0.3.3/exputils/misc/misc.py
-drwxr-xr-x   0 creinke  (661016) perception (50060)        0 2023-01-12 12:25:35.000000 experiment-utilities-0.3.3/exputils/gui/
--rw-r--r--   0 creinke  (661016) perception (50060)      231 2023-01-11 12:41:01.000000 experiment-utilities-0.3.3/exputils/gui/__init__.py
--rw-r--r--   0 creinke  (661016) perception (50060)      967 2023-01-11 12:41:01.000000 experiment-utilities-0.3.3/exputils/gui/misc.py
-drwxr-xr-x   0 creinke  (661016) perception (50060)        0 2023-01-12 12:25:35.000000 experiment-utilities-0.3.3/exputils/gui/jupyter/
--rw-r--r--   0 creinke  (661016) perception (50060)    23142 2023-01-11 12:41:01.000000 experiment-utilities-0.3.3/exputils/gui/jupyter/plotly_meanstd_scatter.py
--rw-r--r--   0 creinke  (661016) perception (50060)     2002 2023-01-11 12:41:01.000000 experiment-utilities-0.3.3/exputils/gui/jupyter/__init__.py
--rw-r--r--   0 creinke  (661016) perception (50060)     2094 2023-01-11 12:41:01.000000 experiment-utilities-0.3.3/exputils/gui/jupyter/repetition_ids_selection_widget.py
--rw-r--r--   0 creinke  (661016) perception (50060)    27218 2023-01-11 12:41:01.000000 experiment-utilities-0.3.3/exputils/gui/jupyter/experiment_data_loader_widget.py
--rw-r--r--   0 creinke  (661016) perception (50060)     9246 2023-01-11 12:41:01.000000 experiment-utilities-0.3.3/exputils/gui/jupyter/tabulate_pairwise.py
--rw-r--r--   0 creinke  (661016) perception (50060)    21931 2023-01-11 12:41:01.000000 experiment-utilities-0.3.3/exputils/gui/jupyter/experiment_data_selection_widget.py
--rw-r--r--   0 creinke  (661016) perception (50060)     4378 2023-01-11 12:41:01.000000 experiment-utilities-0.3.3/exputils/gui/jupyter/misc.py
--rw-r--r--   0 creinke  (661016) perception (50060)     3903 2023-01-11 12:41:01.000000 experiment-utilities-0.3.3/exputils/gui/jupyter/experiment_ids_selection_widget.py
--rw-r--r--   0 creinke  (661016) perception (50060)    11084 2023-01-11 12:41:01.000000 experiment-utilities-0.3.3/exputils/gui/jupyter/plotly_box.py
--rw-r--r--   0 creinke  (661016) perception (50060)     4440 2023-01-11 12:41:01.000000 experiment-utilities-0.3.3/exputils/gui/jupyter/text_selection_accordion_widget.py
--rw-r--r--   0 creinke  (661016) perception (50060)    12686 2023-01-11 12:41:01.000000 experiment-utilities-0.3.3/exputils/gui/jupyter/multi_selection_widget.py
--rw-r--r--   0 creinke  (661016) perception (50060)     3654 2023-01-11 12:41:01.000000 experiment-utilities-0.3.3/exputils/gui/jupyter/code_producer_widget.py
--rw-r--r--   0 creinke  (661016) perception (50060)     2884 2023-01-11 12:41:01.000000 experiment-utilities-0.3.3/exputils/gui/jupyter/ipynbname.py
--rw-r--r--   0 creinke  (661016) perception (50060)     2346 2023-01-11 12:41:01.000000 experiment-utilities-0.3.3/exputils/gui/jupyter/base_widget.py
--rw-r--r--   0 creinke  (661016) perception (50060)     7377 2023-01-11 12:41:01.000000 experiment-utilities-0.3.3/exputils/gui/jupyter/tabulate_meanstd.py
--rw-r--r--   0 creinke  (661016) perception (50060)    10229 2023-01-11 12:41:01.000000 experiment-utilities-0.3.3/exputils/gui/jupyter/plotly_meanstd_bar.py
--rw-r--r--   0 creinke  (661016) perception (50060)    19853 2023-01-11 12:41:01.000000 experiment-utilities-0.3.3/exputils/gui/jupyter/experiment_data_plot_selection_widget.py
-drwxr-xr-x   0 creinke  (661016) perception (50060)        0 2023-01-12 12:25:35.000000 experiment-utilities-0.3.3/exputils/io/
--rw-r--r--   0 creinke  (661016) perception (50060)      813 2023-01-11 12:41:01.000000 experiment-utilities-0.3.3/exputils/io/__init__.py
--rw-r--r--   0 creinke  (661016) perception (50060)      233 2023-01-11 12:41:01.000000 experiment-utilities-0.3.3/exputils/io/pytorch.py
--rw-r--r--   0 creinke  (661016) perception (50060)     3897 2023-01-11 12:41:01.000000 experiment-utilities-0.3.3/exputils/io/odsreader.py
--rw-r--r--   0 creinke  (661016) perception (50060)     1258 2023-01-11 12:41:01.000000 experiment-utilities-0.3.3/exputils/io/dill.py
--rw-r--r--   0 creinke  (661016) perception (50060)      697 2023-01-11 12:41:01.000000 experiment-utilities-0.3.3/exputils/io/general.py
--rw-r--r--   0 creinke  (661016) perception (50060)     3467 2023-01-11 12:41:01.000000 experiment-utilities-0.3.3/exputils/io/numpy.py
--rw-r--r--   0 creinke  (661016) perception (50060)     4287 2023-01-11 12:41:01.000000 experiment-utilities-0.3.3/exputils/io/json.py
-drwxr-xr-x   0 creinke  (661016) perception (50060)        0 2023-01-12 12:25:35.000000 experiment-utilities-0.3.3/experiment_utilities.egg-info/
--rw-r--r--   0 creinke  (661016) perception (50060)        9 2023-01-12 12:25:35.000000 experiment-utilities-0.3.3/experiment_utilities.egg-info/top_level.txt
--rw-r--r--   0 creinke  (661016) perception (50060)     1612 2023-01-12 12:25:35.000000 experiment-utilities-0.3.3/experiment_utilities.egg-info/SOURCES.txt
--rw-r--r--   0 creinke  (661016) perception (50060)     5965 2023-01-12 12:25:35.000000 experiment-utilities-0.3.3/experiment_utilities.egg-info/PKG-INFO
--rw-r--r--   0 creinke  (661016) perception (50060)      201 2023-01-12 12:25:35.000000 experiment-utilities-0.3.3/experiment_utilities.egg-info/requires.txt
--rw-r--r--   0 creinke  (661016) perception (50060)        1 2023-01-12 12:25:35.000000 experiment-utilities-0.3.3/experiment_utilities.egg-info/dependency_links.txt
--rw-r--r--   0 creinke  (661016) perception (50060)     5965 2023-01-12 12:25:35.000000 experiment-utilities-0.3.3/PKG-INFO
--rw-r--r--   0 creinke  (661016) perception (50060)    34502 2022-11-06 11:14:59.000000 experiment-utilities-0.3.3/LICENSE
--rw-r--r--   0 creinke  (661016) perception (50060)      217 2023-01-11 12:41:01.000000 experiment-utilities-0.3.3/setup.py
--rw-r--r--   0 creinke  (661016) perception (50060)      743 2023-01-12 12:25:35.000000 experiment-utilities-0.3.3/setup.cfg
--rw-r--r--   0 creinke  (661016) perception (50060)       80 2022-11-06 11:14:59.000000 experiment-utilities-0.3.3/pyproject.toml
+drwxr-xr-x   0 creinke  (661016) perception (50060)        0 2023-07-08 08:39:33.000000 experiment-utilities-0.3.4/
+drwxr-xr-x   0 creinke  (661016) perception (50060)        0 2023-07-08 08:39:33.000000 experiment-utilities-0.3.4/exputils/
+-rw-r--r--   0 creinke  (661016) perception (50060)     1029 2023-03-08 18:50:59.000000 experiment-utilities-0.3.4/exputils/__init__.py
+drwxr-xr-x   0 creinke  (661016) perception (50060)        0 2023-07-08 08:39:33.000000 experiment-utilities-0.3.4/exputils/manage/
+-rw-r--r--   0 creinke  (661016) perception (50060)      666 2023-01-11 12:41:01.000000 experiment-utilities-0.3.4/exputils/manage/__init__.py
+-rw-r--r--   0 creinke  (661016) perception (50060)    10821 2023-01-11 12:41:01.000000 experiment-utilities-0.3.4/exputils/manage/experimentstarter.py
+-rw-r--r--   0 creinke  (661016) perception (50060)    19818 2023-03-08 18:43:09.000000 experiment-utilities-0.3.4/exputils/manage/experimentgenerator.py
+drwxr-xr-x   0 creinke  (661016) perception (50060)        0 2023-07-08 08:39:33.000000 experiment-utilities-0.3.4/exputils/data/
+-rw-r--r--   0 creinke  (661016) perception (50060)      727 2023-01-11 12:41:01.000000 experiment-utilities-0.3.4/exputils/data/utils.py
+-rw-r--r--   0 creinke  (661016) perception (50060)      951 2023-01-11 12:41:01.000000 experiment-utilities-0.3.4/exputils/data/__init__.py
+-rw-r--r--   0 creinke  (661016) perception (50060)    12904 2023-01-11 12:41:01.000000 experiment-utilities-0.3.4/exputils/data/statistics.py
+-rw-r--r--   0 creinke  (661016) perception (50060)    18960 2023-01-11 12:41:01.000000 experiment-utilities-0.3.4/exputils/data/loading.py
+-rw-r--r--   0 creinke  (661016) perception (50060)     9183 2023-01-12 10:59:20.000000 experiment-utilities-0.3.4/exputils/data/logging.py
+-rw-r--r--   0 creinke  (661016) perception (50060)    11066 2023-01-12 11:04:03.000000 experiment-utilities-0.3.4/exputils/data/logger.py
+-rw-r--r--   0 creinke  (661016) perception (50060)    18966 2023-01-11 12:41:01.000000 experiment-utilities-0.3.4/exputils/data/selection.py
+drwxr-xr-x   0 creinke  (661016) perception (50060)        0 2023-07-08 08:39:33.000000 experiment-utilities-0.3.4/exputils/misc/
+-rw-r--r--   0 creinke  (661016) perception (50060)     1004 2023-01-11 12:41:01.000000 experiment-utilities-0.3.4/exputils/misc/__init__.py
+-rw-r--r--   0 creinke  (661016) perception (50060)    21415 2023-01-11 12:41:01.000000 experiment-utilities-0.3.4/exputils/misc/attrdict.py
+-rw-r--r--   0 creinke  (661016) perception (50060)    18731 2023-01-11 12:41:01.000000 experiment-utilities-0.3.4/exputils/misc/misc.py
+drwxr-xr-x   0 creinke  (661016) perception (50060)        0 2023-07-08 08:39:33.000000 experiment-utilities-0.3.4/exputils/gui/
+-rw-r--r--   0 creinke  (661016) perception (50060)      231 2023-01-11 12:41:01.000000 experiment-utilities-0.3.4/exputils/gui/__init__.py
+-rw-r--r--   0 creinke  (661016) perception (50060)      967 2023-01-11 12:41:01.000000 experiment-utilities-0.3.4/exputils/gui/misc.py
+drwxr-xr-x   0 creinke  (661016) perception (50060)        0 2023-07-08 08:39:33.000000 experiment-utilities-0.3.4/exputils/gui/jupyter/
+-rw-r--r--   0 creinke  (661016) perception (50060)    23142 2023-01-11 12:41:01.000000 experiment-utilities-0.3.4/exputils/gui/jupyter/plotly_meanstd_scatter.py
+-rw-r--r--   0 creinke  (661016) perception (50060)     2002 2023-01-11 12:41:01.000000 experiment-utilities-0.3.4/exputils/gui/jupyter/__init__.py
+-rw-r--r--   0 creinke  (661016) perception (50060)     2094 2023-01-11 12:41:01.000000 experiment-utilities-0.3.4/exputils/gui/jupyter/repetition_ids_selection_widget.py
+-rw-r--r--   0 creinke  (661016) perception (50060)    27218 2023-01-11 12:41:01.000000 experiment-utilities-0.3.4/exputils/gui/jupyter/experiment_data_loader_widget.py
+-rw-r--r--   0 creinke  (661016) perception (50060)     9246 2023-01-11 12:41:01.000000 experiment-utilities-0.3.4/exputils/gui/jupyter/tabulate_pairwise.py
+-rw-r--r--   0 creinke  (661016) perception (50060)    21931 2023-01-11 12:41:01.000000 experiment-utilities-0.3.4/exputils/gui/jupyter/experiment_data_selection_widget.py
+-rw-r--r--   0 creinke  (661016) perception (50060)     4378 2023-01-11 12:41:01.000000 experiment-utilities-0.3.4/exputils/gui/jupyter/misc.py
+-rw-r--r--   0 creinke  (661016) perception (50060)     3903 2023-01-11 12:41:01.000000 experiment-utilities-0.3.4/exputils/gui/jupyter/experiment_ids_selection_widget.py
+-rw-r--r--   0 creinke  (661016) perception (50060)    11084 2023-01-11 12:41:01.000000 experiment-utilities-0.3.4/exputils/gui/jupyter/plotly_box.py
+-rw-r--r--   0 creinke  (661016) perception (50060)     4440 2023-01-11 12:41:01.000000 experiment-utilities-0.3.4/exputils/gui/jupyter/text_selection_accordion_widget.py
+-rw-r--r--   0 creinke  (661016) perception (50060)    12686 2023-01-11 12:41:01.000000 experiment-utilities-0.3.4/exputils/gui/jupyter/multi_selection_widget.py
+-rw-r--r--   0 creinke  (661016) perception (50060)     3654 2023-01-11 12:41:01.000000 experiment-utilities-0.3.4/exputils/gui/jupyter/code_producer_widget.py
+-rw-r--r--   0 creinke  (661016) perception (50060)     2884 2023-01-11 12:41:01.000000 experiment-utilities-0.3.4/exputils/gui/jupyter/ipynbname.py
+-rw-r--r--   0 creinke  (661016) perception (50060)     2346 2023-01-11 12:41:01.000000 experiment-utilities-0.3.4/exputils/gui/jupyter/base_widget.py
+-rw-r--r--   0 creinke  (661016) perception (50060)     7377 2023-01-11 12:41:01.000000 experiment-utilities-0.3.4/exputils/gui/jupyter/tabulate_meanstd.py
+-rw-r--r--   0 creinke  (661016) perception (50060)    10229 2023-01-11 12:41:01.000000 experiment-utilities-0.3.4/exputils/gui/jupyter/plotly_meanstd_bar.py
+-rw-r--r--   0 creinke  (661016) perception (50060)    19853 2023-01-11 12:41:01.000000 experiment-utilities-0.3.4/exputils/gui/jupyter/experiment_data_plot_selection_widget.py
+drwxr-xr-x   0 creinke  (661016) perception (50060)        0 2023-07-08 08:39:33.000000 experiment-utilities-0.3.4/exputils/io/
+-rw-r--r--   0 creinke  (661016) perception (50060)      813 2023-01-11 12:41:01.000000 experiment-utilities-0.3.4/exputils/io/__init__.py
+-rw-r--r--   0 creinke  (661016) perception (50060)      233 2023-01-11 12:41:01.000000 experiment-utilities-0.3.4/exputils/io/pytorch.py
+-rw-r--r--   0 creinke  (661016) perception (50060)     3897 2023-01-11 12:41:01.000000 experiment-utilities-0.3.4/exputils/io/odsreader.py
+-rw-r--r--   0 creinke  (661016) perception (50060)     1258 2023-01-11 12:41:01.000000 experiment-utilities-0.3.4/exputils/io/dill.py
+-rw-r--r--   0 creinke  (661016) perception (50060)      697 2023-01-11 12:41:01.000000 experiment-utilities-0.3.4/exputils/io/general.py
+-rw-r--r--   0 creinke  (661016) perception (50060)     3467 2023-01-11 12:41:01.000000 experiment-utilities-0.3.4/exputils/io/numpy.py
+-rw-r--r--   0 creinke  (661016) perception (50060)     4287 2023-01-11 12:41:01.000000 experiment-utilities-0.3.4/exputils/io/json.py
+drwxr-xr-x   0 creinke  (661016) perception (50060)        0 2023-07-08 08:39:33.000000 experiment-utilities-0.3.4/experiment_utilities.egg-info/
+-rw-r--r--   0 creinke  (661016) perception (50060)        9 2023-07-08 08:39:32.000000 experiment-utilities-0.3.4/experiment_utilities.egg-info/top_level.txt
+-rw-r--r--   0 creinke  (661016) perception (50060)     1612 2023-07-08 08:39:32.000000 experiment-utilities-0.3.4/experiment_utilities.egg-info/SOURCES.txt
+-rw-r--r--   0 creinke  (661016) perception (50060)     5965 2023-07-08 08:39:32.000000 experiment-utilities-0.3.4/experiment_utilities.egg-info/PKG-INFO
+-rw-r--r--   0 creinke  (661016) perception (50060)      201 2023-07-08 08:39:32.000000 experiment-utilities-0.3.4/experiment_utilities.egg-info/requires.txt
+-rw-r--r--   0 creinke  (661016) perception (50060)        1 2023-07-08 08:39:32.000000 experiment-utilities-0.3.4/experiment_utilities.egg-info/dependency_links.txt
+-rw-r--r--   0 creinke  (661016) perception (50060)     5965 2023-07-08 08:39:33.000000 experiment-utilities-0.3.4/PKG-INFO
+-rw-r--r--   0 creinke  (661016) perception (50060)    34502 2022-11-06 11:14:59.000000 experiment-utilities-0.3.4/LICENSE
+-rw-r--r--   0 creinke  (661016) perception (50060)      217 2023-01-11 12:41:01.000000 experiment-utilities-0.3.4/setup.py
+-rw-r--r--   0 creinke  (661016) perception (50060)      743 2023-07-08 08:39:33.000000 experiment-utilities-0.3.4/setup.cfg
+-rw-r--r--   0 creinke  (661016) perception (50060)      179 2023-05-16 12:42:25.000000 experiment-utilities-0.3.4/pyproject.toml
```

### Comparing `experiment-utilities-0.3.3/exputils/__init__.py` & `experiment-utilities-0.3.4/exputils/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 from exputils.misc.attrdict import AutoAttrDict
 from exputils.misc.attrdict import DefaultAttrDict
 from exputils.misc.attrdict import DefaultFactoryAttrDict
 from exputils.misc.attrdict import combine_dicts
 
 from exputils.misc import update_status
 
-__version__ = '0.3.3'
+__version__ = '0.3.4'
 
 DEFAULT_ODS_CONFIGURATION_FILE = 'experiment_configurations.ods'
 DEFAULT_EXPERIMENTS_DIRECTORY = 'experiments'
 EXPERIMENT_DIRECTORY_TEMPLATE = 'experiment_{:06d}'
 REPETITION_DIRECTORY_TEMPLATE = 'repetition_{:06d}'
 DEFAULT_DATA_DIRECTORY = 'data'  # name of the data directory under the experiments and repetition folders
```

### Comparing `experiment-utilities-0.3.3/exputils/manage/__init__.py` & `experiment-utilities-0.3.4/exputils/manage/__init__.py`

 * *Files identical despite different names*

### Comparing `experiment-utilities-0.3.3/exputils/manage/experimentstarter.py` & `experiment-utilities-0.3.4/exputils/manage/experimentstarter.py`

 * *Files identical despite different names*

### Comparing `experiment-utilities-0.3.3/exputils/manage/experimentgenerator.py` & `experiment-utilities-0.3.4/exputils/manage/experimentgenerator.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,14 +11,17 @@
 import stat
 import re
 import copy
 import shutil
 import exputils
 from collections import OrderedDict
 
+# TODO: allow default values in the config
+# TODO: allow to delete a line in the config, for example if the value of a param is "#RM"
+
 
 def generate_experiment_files(ods_filepath=None, directory=None, extra_files=None, extra_experiment_files=None, verbose=False, copy_operator='shutil'):
     """
     Generates experiment files and configurations based on entries in a ODS file (LibreOffice Spreadsheet).
 
     The ODS has to be in a specific form.
     Sheets define group of experiment for which an extra subfolder in the output directory will be generated.
@@ -229,15 +232,15 @@
 
                     experiments_data['experiments'][experiment_id]['files'][file_idx]['variables'] = dict()
 
                     for variable_name in variable_names[file_idx]:
 
                         if col_idx > len(sheet_data[row_idx]) - 1:
                             # if there is no content in the final cells, the array that holds the data is shorter
-                            cur_cell_data = ''
+                            cur_cell_data = None
                         else:
                             cur_cell_data = get_cell_data(sheet_data[row_idx][col_idx])
 
                         experiments_data['experiments'][experiment_id]['files'][file_idx]['variables'][variable_name] = cur_cell_data
 
                         col_idx +=1
 
@@ -245,15 +248,15 @@
 
     return config_data
 
 
 def get_cell_data(data):
 
     if data is None:
-        data = ''
+        return None
 
     # replace strange characters that are not used for python strings
     data = data.replace('’', '\'')
     data = data.replace('`', '\'')
 
     return data
 
@@ -351,14 +354,16 @@
                     experiment_id,
                     copy_operator=copy_operator
                 )
 
 
 def generate_source_files(source_files, experiment_files_directory, experiment_config, experiment_id, repetition_id=None, copy_operator='shutil'):
 
+    default_value = ''
+
     if copy_operator.lower() == 'shutil':
         copy_function = _copy_operator_shutil
     elif copy_operator.lower() == 'cp':
         copy_function = _copy_operator_linux_cp
     else:
         raise ValueError('Unknown copy_operator "{}"! Must be either "shutil" or "cp".'.format(copy_operator))
 
@@ -378,33 +383,63 @@
 
         if template_file_path is not None:
 
             # get file permissions
             permissions = os.stat(template_file_path)[stat.ST_MODE]
 
             # Read in the template file
+            file_lines = []
             with open(template_file_path, 'r') as file:
-                file_content = file.read()
-
-            # Replace the variables
-            file_content = file_content.replace('<experiment_id>', str(experiment_id))
-
-            if repetition_id is not None:
-                file_content = file_content.replace('<repetition_id>', str(repetition_id))
+                file_lines = file.readlines()
 
-            for variable_name, variable_value in file_config['variables'].items():
-                file_content = re.sub('<{}>'.format(variable_name),
-                                      variable_value,
-                                      file_content,
-                                      flags=re.IGNORECASE)
+            # lines that should be written
+            write_lines = []
+            for line in file_lines:
+
+                # Replace the variables
+                line = line.replace('<experiment_id>', str(experiment_id))
+
+                if repetition_id is not None:
+                    line = line.replace('<repetition_id>', str(repetition_id))
+
+                is_remove_line = False
+                for variable_name, variable_value in file_config['variables'].items():
+
+                    match = True
+                    while match is not None:
+                        # allow default values that come directly after the varibale_name: "<var_name,'varibale'>"
+                        match = re.search(r"<{}(,[^<]+)?>".format(variable_name), line, flags=re.IGNORECASE)
+
+                        if match is not None:
+                            # value is the variable_value
+                            val = variable_value
+
+                            # if it is None, then use the default value from the file, or the general default value which is ''
+                            if val is None:
+                                # if there is a default value defined in the source file
+                                if match.group(1) is None:
+                                    val = default_value
+                                else:
+                                    val = match.group(1)[1:]  # remove the initial ','
+
+                            # delete the whole line if the varibale value is "%RM"
+                            if val == '%RM':
+                                is_remove_line = True
+                                break
+
+                            line = line.replace(match.group(0), val)
+
+                # delete the whole line if the varibale value is "%RM"
+                if not is_remove_line:
+                    write_lines.append(line)
 
             # Write the final output file
             file_path = os.path.join(experiment_files_directory, file_config['file_name_template'].format(experiment_id))
             with open(file_path, 'w') as file:
-                file.write(file_content)
+                file.writelines(write_lines)
             os.chmod(file_path, permissions)
 
     # copy all other sources, but not the templates if they are in one of the source directories
     template_files = [file_config['template_file_path'] for file_config in experiment_config['files']]
 
     for src in source_files:
         copy_experiment_files(src, experiment_files_directory, template_files, copy_function)
```

### Comparing `experiment-utilities-0.3.3/exputils/data/utils.py` & `experiment-utilities-0.3.4/exputils/data/utils.py`

 * *Files identical despite different names*

### Comparing `experiment-utilities-0.3.3/exputils/data/__init__.py` & `experiment-utilities-0.3.4/exputils/data/__init__.py`

 * *Files identical despite different names*

### Comparing `experiment-utilities-0.3.3/exputils/data/statistics.py` & `experiment-utilities-0.3.4/exputils/data/statistics.py`

 * *Files identical despite different names*

### Comparing `experiment-utilities-0.3.3/exputils/data/loading.py` & `experiment-utilities-0.3.4/exputils/data/loading.py`

 * *Files identical despite different names*

### Comparing `experiment-utilities-0.3.3/exputils/data/logging.py` & `experiment-utilities-0.3.4/exputils/data/logging.py`

 * *Files identical despite different names*

### Comparing `experiment-utilities-0.3.3/exputils/data/logger.py` & `experiment-utilities-0.3.4/exputils/data/logger.py`

 * *Files identical despite different names*

### Comparing `experiment-utilities-0.3.3/exputils/data/selection.py` & `experiment-utilities-0.3.4/exputils/data/selection.py`

 * *Files identical despite different names*

### Comparing `experiment-utilities-0.3.3/exputils/misc/__init__.py` & `experiment-utilities-0.3.4/exputils/misc/__init__.py`

 * *Files identical despite different names*

### Comparing `experiment-utilities-0.3.3/exputils/misc/attrdict.py` & `experiment-utilities-0.3.4/exputils/misc/attrdict.py`

 * *Files identical despite different names*

### Comparing `experiment-utilities-0.3.3/exputils/misc/misc.py` & `experiment-utilities-0.3.4/exputils/misc/misc.py`

 * *Files identical despite different names*

### Comparing `experiment-utilities-0.3.3/exputils/gui/misc.py` & `experiment-utilities-0.3.4/exputils/gui/misc.py`

 * *Files identical despite different names*

### Comparing `experiment-utilities-0.3.3/exputils/gui/jupyter/plotly_meanstd_scatter.py` & `experiment-utilities-0.3.4/exputils/gui/jupyter/plotly_meanstd_scatter.py`

 * *Files identical despite different names*

### Comparing `experiment-utilities-0.3.3/exputils/gui/jupyter/__init__.py` & `experiment-utilities-0.3.4/exputils/gui/jupyter/__init__.py`

 * *Files identical despite different names*

### Comparing `experiment-utilities-0.3.3/exputils/gui/jupyter/repetition_ids_selection_widget.py` & `experiment-utilities-0.3.4/exputils/gui/jupyter/repetition_ids_selection_widget.py`

 * *Files identical despite different names*

### Comparing `experiment-utilities-0.3.3/exputils/gui/jupyter/experiment_data_loader_widget.py` & `experiment-utilities-0.3.4/exputils/gui/jupyter/experiment_data_loader_widget.py`

 * *Files identical despite different names*

### Comparing `experiment-utilities-0.3.3/exputils/gui/jupyter/tabulate_pairwise.py` & `experiment-utilities-0.3.4/exputils/gui/jupyter/tabulate_pairwise.py`

 * *Files identical despite different names*

### Comparing `experiment-utilities-0.3.3/exputils/gui/jupyter/experiment_data_selection_widget.py` & `experiment-utilities-0.3.4/exputils/gui/jupyter/experiment_data_selection_widget.py`

 * *Files identical despite different names*

### Comparing `experiment-utilities-0.3.3/exputils/gui/jupyter/misc.py` & `experiment-utilities-0.3.4/exputils/gui/jupyter/misc.py`

 * *Files identical despite different names*

### Comparing `experiment-utilities-0.3.3/exputils/gui/jupyter/experiment_ids_selection_widget.py` & `experiment-utilities-0.3.4/exputils/gui/jupyter/experiment_ids_selection_widget.py`

 * *Files identical despite different names*

### Comparing `experiment-utilities-0.3.3/exputils/gui/jupyter/plotly_box.py` & `experiment-utilities-0.3.4/exputils/gui/jupyter/plotly_box.py`

 * *Files identical despite different names*

### Comparing `experiment-utilities-0.3.3/exputils/gui/jupyter/text_selection_accordion_widget.py` & `experiment-utilities-0.3.4/exputils/gui/jupyter/text_selection_accordion_widget.py`

 * *Files identical despite different names*

### Comparing `experiment-utilities-0.3.3/exputils/gui/jupyter/multi_selection_widget.py` & `experiment-utilities-0.3.4/exputils/gui/jupyter/multi_selection_widget.py`

 * *Files identical despite different names*

### Comparing `experiment-utilities-0.3.3/exputils/gui/jupyter/code_producer_widget.py` & `experiment-utilities-0.3.4/exputils/gui/jupyter/code_producer_widget.py`

 * *Files identical despite different names*

### Comparing `experiment-utilities-0.3.3/exputils/gui/jupyter/ipynbname.py` & `experiment-utilities-0.3.4/exputils/gui/jupyter/ipynbname.py`

 * *Files identical despite different names*

### Comparing `experiment-utilities-0.3.3/exputils/gui/jupyter/base_widget.py` & `experiment-utilities-0.3.4/exputils/gui/jupyter/base_widget.py`

 * *Files identical despite different names*

### Comparing `experiment-utilities-0.3.3/exputils/gui/jupyter/tabulate_meanstd.py` & `experiment-utilities-0.3.4/exputils/gui/jupyter/tabulate_meanstd.py`

 * *Files identical despite different names*

### Comparing `experiment-utilities-0.3.3/exputils/gui/jupyter/plotly_meanstd_bar.py` & `experiment-utilities-0.3.4/exputils/gui/jupyter/plotly_meanstd_bar.py`

 * *Files identical despite different names*

### Comparing `experiment-utilities-0.3.3/exputils/gui/jupyter/experiment_data_plot_selection_widget.py` & `experiment-utilities-0.3.4/exputils/gui/jupyter/experiment_data_plot_selection_widget.py`

 * *Files identical despite different names*

### Comparing `experiment-utilities-0.3.3/exputils/io/__init__.py` & `experiment-utilities-0.3.4/exputils/io/__init__.py`

 * *Files identical despite different names*

### Comparing `experiment-utilities-0.3.3/exputils/io/odsreader.py` & `experiment-utilities-0.3.4/exputils/io/odsreader.py`

 * *Files identical despite different names*

### Comparing `experiment-utilities-0.3.3/exputils/io/dill.py` & `experiment-utilities-0.3.4/exputils/io/dill.py`

 * *Files identical despite different names*

### Comparing `experiment-utilities-0.3.3/exputils/io/general.py` & `experiment-utilities-0.3.4/exputils/io/general.py`

 * *Files identical despite different names*

### Comparing `experiment-utilities-0.3.3/exputils/io/numpy.py` & `experiment-utilities-0.3.4/exputils/io/numpy.py`

 * *Files identical despite different names*

### Comparing `experiment-utilities-0.3.3/exputils/io/json.py` & `experiment-utilities-0.3.4/exputils/io/json.py`

 * *Files identical despite different names*

### Comparing `experiment-utilities-0.3.3/experiment_utilities.egg-info/SOURCES.txt` & `experiment-utilities-0.3.4/experiment_utilities.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `experiment-utilities-0.3.3/experiment_utilities.egg-info/PKG-INFO` & `experiment-utilities-0.3.4/experiment_utilities.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: experiment-utilities
-Version: 0.3.3
+Version: 0.3.4
 Summary: Toolbox to run and analyse scientific computer experiments.
 Home-page: https://gitlab.inria.fr/creinke/exputils/
 Author: Chris Reinke
 Author-email: chris.reinke@inria.fr
 License: GNU General Public License v3 (GPLv3)
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-Current version: 0.3.3 (12/01/2023)
+Current version: 0.3.4 (08/03/2023)
 
 # Introduction
 
 Experiment Utilities (exputils) contains various tools for the management of scientific experiments and their experimental data.
 It is especially designed to handle experimental repetitions, including to run different repetitions, to effectively store and load data for them, and to visualize their results.  
  
 Main features:
```

### Comparing `experiment-utilities-0.3.3/PKG-INFO` & `experiment-utilities-0.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: experiment-utilities
-Version: 0.3.3
+Version: 0.3.4
 Summary: Toolbox to run and analyse scientific computer experiments.
 Home-page: https://gitlab.inria.fr/creinke/exputils/
 Author: Chris Reinke
 Author-email: chris.reinke@inria.fr
 License: GNU General Public License v3 (GPLv3)
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-Current version: 0.3.3 (12/01/2023)
+Current version: 0.3.4 (08/03/2023)
 
 # Introduction
 
 Experiment Utilities (exputils) contains various tools for the management of scientific experiments and their experimental data.
 It is especially designed to handle experimental repetitions, including to run different repetitions, to effectively store and load data for them, and to visualize their results.  
  
 Main features:
```

### Comparing `experiment-utilities-0.3.3/LICENSE` & `experiment-utilities-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `experiment-utilities-0.3.3/setup.cfg` & `experiment-utilities-0.3.4/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = experiment-utilities
-version = 0.3.3
+version = 0.3.4
 author = Chris Reinke
 author_email = chris.reinke@inria.fr
 url = https://gitlab.inria.fr/creinke/exputils/
 description = Toolbox to run and analyse scientific computer experiments.
 long_description = file: readme.md
 long_description_content_type = text/markdown
 license = GNU General Public License v3 (GPLv3)
```

