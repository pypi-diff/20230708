# Comparing `tmp/torchtnt-nightly-2023.7.6.tar.gz` & `tmp/torchtnt-nightly-2023.7.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torchtnt-nightly-2023.7.6.tar", last modified: Thu Jul  6 11:24:17 2023, max compression
+gzip compressed data, was "torchtnt-nightly-2023.7.7.tar", last modified: Fri Jul  7 11:24:15 2023, max compression
```

## Comparing `torchtnt-nightly-2023.7.6.tar` & `torchtnt-nightly-2023.7.7.tar`

### file list

```diff
@@ -1,75 +1,75 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:24:17.659711 torchtnt-nightly-2023.7.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-07-06 11:22:46.000000 torchtnt-nightly-2023.7.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-07-06 11:24:17.659711 torchtnt-nightly-2023.7.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-07-06 11:22:46.000000 torchtnt-nightly-2023.7.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-06 11:22:46.000000 torchtnt-nightly-2023.7.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 11:24:17.659711 torchtnt-nightly-2023.7.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2948 2023-07-06 11:22:46.000000 torchtnt-nightly-2023.7.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:24:17.655711 torchtnt-nightly-2023.7.6/torchtnt/
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-07-06 11:22:46.000000 torchtnt-nightly-2023.7.6/torchtnt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:24:17.655711 torchtnt-nightly-2023.7.6/torchtnt/framework/
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-07-06 11:22:46.000000 torchtnt-nightly-2023.7.6/torchtnt/framework/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4046 2023-07-06 11:22:46.000000 torchtnt-nightly-2023.7.6/torchtnt/framework/_test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    35861 2023-07-06 11:22:46.000000 torchtnt-nightly-2023.7.6/torchtnt/framework/auto_unit.py
--rw-r--r--   0 runner    (1001) docker     (123)     5188 2023-07-06 11:22:46.000000 torchtnt-nightly-2023.7.6/torchtnt/framework/callback.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:24:17.655711 torchtnt-nightly-2023.7.6/torchtnt/framework/callbacks/
--rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-07-06 11:22:46.000000 torchtnt-nightly-2023.7.6/torchtnt/framework/callbacks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3358 2023-07-06 11:22:46.000000 torchtnt-nightly-2023.7.6/torchtnt/framework/callbacks/base_csv_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4148 2023-07-06 11:22:46.000000 torchtnt-nightly-2023.7.6/torchtnt/framework/callbacks/garbage_collector.py
--rw-r--r--   0 runner    (1001) docker     (123)     4452 2023-07-06 11:22:46.000000 torchtnt-nightly-2023.7.6/torchtnt/framework/callbacks/lambda_callback.py
--rw-r--r--   0 runner    (1001) docker     (123)     3582 2023-07-06 11:22:46.000000 torchtnt-nightly-2023.7.6/torchtnt/framework/callbacks/learning_rate_monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3628 2023-07-06 11:22:46.000000 torchtnt-nightly-2023.7.6/torchtnt/framework/callbacks/module_summary.py
--rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-07-06 11:22:46.000000 torchtnt-nightly-2023.7.6/torchtnt/framework/callbacks/pytorch_profiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3532 2023-07-06 11:22:46.000000 torchtnt-nightly-2023.7.6/torchtnt/framework/callbacks/system_resources_monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-07-06 11:22:46.000000 torchtnt-nightly-2023.7.6/torchtnt/framework/callbacks/tensorboard_parameter_monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)    12926 2023-07-06 11:22:46.000000 torchtnt-nightly-2023.7.6/torchtnt/framework/callbacks/torchsnapshot_saver.py
--rw-r--r--   0 runner    (1001) docker     (123)     5260 2023-07-06 11:22:46.000000 torchtnt-nightly-2023.7.6/torchtnt/framework/callbacks/tqdm_progress_bar.py
--rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-07-06 11:22:46.000000 torchtnt-nightly-2023.7.6/torchtnt/framework/callbacks/train_progress_monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)     8868 2023-07-06 11:22:46.000000 torchtnt-nightly-2023.7.6/torchtnt/framework/evaluate.py
--rw-r--r--   0 runner    (1001) docker     (123)     8500 2023-07-06 11:22:46.000000 torchtnt-nightly-2023.7.6/torchtnt/framework/fit.py
--rw-r--r--   0 runner    (1001) docker     (123)     9232 2023-07-06 11:22:46.000000 torchtnt-nightly-2023.7.6/torchtnt/framework/predict.py
--rw-r--r--   0 runner    (1001) docker     (123)     7154 2023-07-06 11:22:46.000000 torchtnt-nightly-2023.7.6/torchtnt/framework/state.py
--rw-r--r--   0 runner    (1001) docker     (123)    11789 2023-07-06 11:22:46.000000 torchtnt-nightly-2023.7.6/torchtnt/framework/train.py
--rw-r--r--   0 runner    (1001) docker     (123)    15355 2023-07-06 11:22:46.000000 torchtnt-nightly-2023.7.6/torchtnt/framework/unit.py
--rw-r--r--   0 runner    (1001) docker     (123)     9965 2023-07-06 11:22:46.000000 torchtnt-nightly-2023.7.6/torchtnt/framework/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 11:22:46.000000 torchtnt-nightly-2023.7.6/torchtnt/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:24:17.659711 torchtnt-nightly-2023.7.6/torchtnt/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     3405 2023-07-06 11:22:46.000000 torchtnt-nightly-2023.7.6/torchtnt/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:24:17.659711 torchtnt-nightly-2023.7.6/torchtnt/utils/data/
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-07-06 11:22:46.000000 torchtnt-nightly-2023.7.6/torchtnt/utils/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3836 2023-07-06 11:22:46.000000 torchtnt-nightly-2023.7.6/torchtnt/utils/data/data_prefetcher.py
--rw-r--r--   0 runner    (1001) docker     (123)    20345 2023-07-06 11:22:46.000000 torchtnt-nightly-2023.7.6/torchtnt/utils/data/iterators.py
--rw-r--r--   0 runner    (1001) docker     (123)     3386 2023-07-06 11:22:46.000000 torchtnt-nightly-2023.7.6/torchtnt/utils/data/multi_dataloader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2302 2023-07-06 11:22:46.000000 torchtnt-nightly-2023.7.6/torchtnt/utils/data/profile_dataloader.py
--rw-r--r--   0 runner    (1001) docker     (123)    11235 2023-07-06 11:22:46.000000 torchtnt-nightly-2023.7.6/torchtnt/utils/device.py
--rw-r--r--   0 runner    (1001) docker     (123)    19265 2023-07-06 11:22:46.000000 torchtnt-nightly-2023.7.6/torchtnt/utils/distributed.py
--rw-r--r--   0 runner    (1001) docker     (123)     9897 2023-07-06 11:22:46.000000 torchtnt-nightly-2023.7.6/torchtnt/utils/early_stop_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)     6211 2023-07-06 11:22:46.000000 torchtnt-nightly-2023.7.6/torchtnt/utils/env.py
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-07-06 11:22:46.000000 torchtnt-nightly-2023.7.6/torchtnt/utils/fsspec.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:24:17.659711 torchtnt-nightly-2023.7.6/torchtnt/utils/loggers/
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-07-06 11:22:46.000000 torchtnt-nightly-2023.7.6/torchtnt/utils/loggers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-07-06 11:22:46.000000 torchtnt-nightly-2023.7.6/torchtnt/utils/loggers/csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     2881 2023-07-06 11:22:46.000000 torchtnt-nightly-2023.7.6/torchtnt/utils/loggers/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-07-06 11:22:46.000000 torchtnt-nightly-2023.7.6/torchtnt/utils/loggers/in_memory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-07-06 11:22:46.000000 torchtnt-nightly-2023.7.6/torchtnt/utils/loggers/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-07-06 11:22:46.000000 torchtnt-nightly-2023.7.6/torchtnt/utils/loggers/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     5786 2023-07-06 11:22:46.000000 torchtnt-nightly-2023.7.6/torchtnt/utils/loggers/tensorboard.py
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-07-06 11:22:46.000000 torchtnt-nightly-2023.7.6/torchtnt/utils/loggers/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-07-06 11:22:46.000000 torchtnt-nightly-2023.7.6/torchtnt/utils/lr_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4760 2023-07-06 11:22:46.000000 torchtnt-nightly-2023.7.6/torchtnt/utils/memory.py
--rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-07-06 11:22:46.000000 torchtnt-nightly-2023.7.6/torchtnt/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4804 2023-07-06 11:22:46.000000 torchtnt-nightly-2023.7.6/torchtnt/utils/oom.py
--rw-r--r--   0 runner    (1001) docker     (123)     6639 2023-07-06 11:22:46.000000 torchtnt-nightly-2023.7.6/torchtnt/utils/prepare_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3219 2023-07-06 11:22:46.000000 torchtnt-nightly-2023.7.6/torchtnt/utils/progress.py
--rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-07-06 11:22:46.000000 torchtnt-nightly-2023.7.6/torchtnt/utils/rank_zero_log.py
--rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-07-06 11:22:46.000000 torchtnt-nightly-2023.7.6/torchtnt/utils/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    13242 2023-07-06 11:22:46.000000 torchtnt-nightly-2023.7.6/torchtnt/utils/timer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-07-06 11:22:46.000000 torchtnt-nightly-2023.7.6/torchtnt/utils/tqdm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-07-06 11:22:46.000000 torchtnt-nightly-2023.7.6/torchtnt/utils/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:24:17.659711 torchtnt-nightly-2023.7.6/torchtnt_nightly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-07-06 11:24:17.000000 torchtnt-nightly-2023.7.6/torchtnt_nightly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-07-06 11:24:17.000000 torchtnt-nightly-2023.7.6/torchtnt_nightly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 11:24:17.000000 torchtnt-nightly-2023.7.6/torchtnt_nightly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-06 11:24:17.000000 torchtnt-nightly-2023.7.6/torchtnt_nightly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-06 11:24:17.000000 torchtnt-nightly-2023.7.6/torchtnt_nightly.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 11:24:17.000000 torchtnt-nightly-2023.7.6/torchtnt_nightly.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 11:24:15.988702 torchtnt-nightly-2023.7.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-07-07 11:22:36.000000 torchtnt-nightly-2023.7.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-07-07 11:24:15.988702 torchtnt-nightly-2023.7.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-07-07 11:22:36.000000 torchtnt-nightly-2023.7.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-07 11:22:37.000000 torchtnt-nightly-2023.7.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 11:24:15.988702 torchtnt-nightly-2023.7.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2948 2023-07-07 11:22:37.000000 torchtnt-nightly-2023.7.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 11:24:15.976702 torchtnt-nightly-2023.7.7/torchtnt/
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-07-07 11:22:37.000000 torchtnt-nightly-2023.7.7/torchtnt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 11:24:15.980702 torchtnt-nightly-2023.7.7/torchtnt/framework/
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-07-07 11:22:37.000000 torchtnt-nightly-2023.7.7/torchtnt/framework/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4046 2023-07-07 11:22:37.000000 torchtnt-nightly-2023.7.7/torchtnt/framework/_test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36790 2023-07-07 11:22:37.000000 torchtnt-nightly-2023.7.7/torchtnt/framework/auto_unit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5188 2023-07-07 11:22:37.000000 torchtnt-nightly-2023.7.7/torchtnt/framework/callback.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 11:24:15.980702 torchtnt-nightly-2023.7.7/torchtnt/framework/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-07-07 11:22:37.000000 torchtnt-nightly-2023.7.7/torchtnt/framework/callbacks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3358 2023-07-07 11:22:37.000000 torchtnt-nightly-2023.7.7/torchtnt/framework/callbacks/base_csv_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4148 2023-07-07 11:22:37.000000 torchtnt-nightly-2023.7.7/torchtnt/framework/callbacks/garbage_collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4452 2023-07-07 11:22:37.000000 torchtnt-nightly-2023.7.7/torchtnt/framework/callbacks/lambda_callback.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3582 2023-07-07 11:22:37.000000 torchtnt-nightly-2023.7.7/torchtnt/framework/callbacks/learning_rate_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3628 2023-07-07 11:22:37.000000 torchtnt-nightly-2023.7.7/torchtnt/framework/callbacks/module_summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-07-07 11:22:37.000000 torchtnt-nightly-2023.7.7/torchtnt/framework/callbacks/pytorch_profiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3532 2023-07-07 11:22:37.000000 torchtnt-nightly-2023.7.7/torchtnt/framework/callbacks/system_resources_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-07-07 11:22:37.000000 torchtnt-nightly-2023.7.7/torchtnt/framework/callbacks/tensorboard_parameter_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12579 2023-07-07 11:22:37.000000 torchtnt-nightly-2023.7.7/torchtnt/framework/callbacks/torchsnapshot_saver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5260 2023-07-07 11:22:37.000000 torchtnt-nightly-2023.7.7/torchtnt/framework/callbacks/tqdm_progress_bar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-07-07 11:22:37.000000 torchtnt-nightly-2023.7.7/torchtnt/framework/callbacks/train_progress_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8868 2023-07-07 11:22:37.000000 torchtnt-nightly-2023.7.7/torchtnt/framework/evaluate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8500 2023-07-07 11:22:37.000000 torchtnt-nightly-2023.7.7/torchtnt/framework/fit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9232 2023-07-07 11:22:37.000000 torchtnt-nightly-2023.7.7/torchtnt/framework/predict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7154 2023-07-07 11:22:37.000000 torchtnt-nightly-2023.7.7/torchtnt/framework/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11789 2023-07-07 11:22:37.000000 torchtnt-nightly-2023.7.7/torchtnt/framework/train.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15355 2023-07-07 11:22:37.000000 torchtnt-nightly-2023.7.7/torchtnt/framework/unit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9965 2023-07-07 11:22:37.000000 torchtnt-nightly-2023.7.7/torchtnt/framework/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 11:22:37.000000 torchtnt-nightly-2023.7.7/torchtnt/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 11:24:15.984702 torchtnt-nightly-2023.7.7/torchtnt/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     3405 2023-07-07 11:22:37.000000 torchtnt-nightly-2023.7.7/torchtnt/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 11:24:15.984702 torchtnt-nightly-2023.7.7/torchtnt/utils/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-07-07 11:22:37.000000 torchtnt-nightly-2023.7.7/torchtnt/utils/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3836 2023-07-07 11:22:37.000000 torchtnt-nightly-2023.7.7/torchtnt/utils/data/data_prefetcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20345 2023-07-07 11:22:37.000000 torchtnt-nightly-2023.7.7/torchtnt/utils/data/iterators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3386 2023-07-07 11:22:37.000000 torchtnt-nightly-2023.7.7/torchtnt/utils/data/multi_dataloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2302 2023-07-07 11:22:37.000000 torchtnt-nightly-2023.7.7/torchtnt/utils/data/profile_dataloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11235 2023-07-07 11:22:37.000000 torchtnt-nightly-2023.7.7/torchtnt/utils/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19191 2023-07-07 11:22:37.000000 torchtnt-nightly-2023.7.7/torchtnt/utils/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9897 2023-07-07 11:22:37.000000 torchtnt-nightly-2023.7.7/torchtnt/utils/early_stop_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6211 2023-07-07 11:22:37.000000 torchtnt-nightly-2023.7.7/torchtnt/utils/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-07-07 11:22:37.000000 torchtnt-nightly-2023.7.7/torchtnt/utils/fsspec.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 11:24:15.988702 torchtnt-nightly-2023.7.7/torchtnt/utils/loggers/
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-07-07 11:22:37.000000 torchtnt-nightly-2023.7.7/torchtnt/utils/loggers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-07-07 11:22:37.000000 torchtnt-nightly-2023.7.7/torchtnt/utils/loggers/csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2881 2023-07-07 11:22:37.000000 torchtnt-nightly-2023.7.7/torchtnt/utils/loggers/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-07-07 11:22:37.000000 torchtnt-nightly-2023.7.7/torchtnt/utils/loggers/in_memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-07-07 11:22:37.000000 torchtnt-nightly-2023.7.7/torchtnt/utils/loggers/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-07-07 11:22:37.000000 torchtnt-nightly-2023.7.7/torchtnt/utils/loggers/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6171 2023-07-07 11:22:37.000000 torchtnt-nightly-2023.7.7/torchtnt/utils/loggers/tensorboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-07-07 11:22:37.000000 torchtnt-nightly-2023.7.7/torchtnt/utils/loggers/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-07-07 11:22:37.000000 torchtnt-nightly-2023.7.7/torchtnt/utils/lr_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4760 2023-07-07 11:22:37.000000 torchtnt-nightly-2023.7.7/torchtnt/utils/memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-07-07 11:22:37.000000 torchtnt-nightly-2023.7.7/torchtnt/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4804 2023-07-07 11:22:37.000000 torchtnt-nightly-2023.7.7/torchtnt/utils/oom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6639 2023-07-07 11:22:37.000000 torchtnt-nightly-2023.7.7/torchtnt/utils/prepare_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3219 2023-07-07 11:22:37.000000 torchtnt-nightly-2023.7.7/torchtnt/utils/progress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-07-07 11:22:37.000000 torchtnt-nightly-2023.7.7/torchtnt/utils/rank_zero_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-07-07 11:22:37.000000 torchtnt-nightly-2023.7.7/torchtnt/utils/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13242 2023-07-07 11:22:37.000000 torchtnt-nightly-2023.7.7/torchtnt/utils/timer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-07-07 11:22:37.000000 torchtnt-nightly-2023.7.7/torchtnt/utils/tqdm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-07-07 11:22:37.000000 torchtnt-nightly-2023.7.7/torchtnt/utils/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 11:24:15.988702 torchtnt-nightly-2023.7.7/torchtnt_nightly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-07-07 11:24:15.000000 torchtnt-nightly-2023.7.7/torchtnt_nightly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-07-07 11:24:15.000000 torchtnt-nightly-2023.7.7/torchtnt_nightly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 11:24:15.000000 torchtnt-nightly-2023.7.7/torchtnt_nightly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-07 11:24:15.000000 torchtnt-nightly-2023.7.7/torchtnt_nightly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-07 11:24:15.000000 torchtnt-nightly-2023.7.7/torchtnt_nightly.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 11:24:15.000000 torchtnt-nightly-2023.7.7/torchtnt_nightly.egg-info/zip-safe
```

### Comparing `torchtnt-nightly-2023.7.6/LICENSE` & `torchtnt-nightly-2023.7.7/LICENSE`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.7.6/PKG-INFO` & `torchtnt-nightly-2023.7.7/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torchtnt-nightly
-Version: 2023.7.6
+Version: 2023.7.7
 Summary: A lightweight library for PyTorch training tools and utilities
 Home-page: https://github.com/pytorch/tnt
 Author: PyTorch
 Author-email: daniellepintz@fb.com
 License: BSD-3
 Keywords: pytorch,torch,training,tools,utilities
 Classifier: Development Status :: 2 - Pre-Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: torchtnt-nightly Version: 2023.7.6 Summary: A
+Metadata-Version: 2.1 Name: torchtnt-nightly Version: 2023.7.7 Summary: A
 lightweight library for PyTorch training tools and utilities Home-page: https:/
 /github.com/pytorch/tnt Author: PyTorch Author-email: daniellepintz@fb.com
 License: BSD-3 Keywords: pytorch,torch,training,tools,utilities Classifier:
 Development Status :: 2 - Pre-Alpha Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research Classifier: License :: OSI
 Approved :: BSD License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7 Classifier: Topic ::
```

### Comparing `torchtnt-nightly-2023.7.6/README.md` & `torchtnt-nightly-2023.7.7/README.md`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.7.6/setup.py` & `torchtnt-nightly-2023.7.7/setup.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.7.6/torchtnt/framework/__init__.py` & `torchtnt-nightly-2023.7.7/torchtnt/framework/__init__.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.7.6/torchtnt/framework/_test_utils.py` & `torchtnt-nightly-2023.7.7/torchtnt/framework/_test_utils.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.7.6/torchtnt/framework/auto_unit.py` & `torchtnt-nightly-2023.7.7/torchtnt/framework/auto_unit.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,17 +6,17 @@
 
 # ignore errors due to `Any` type
 # pyre-ignore-all-errors[2]
 # pyre-ignore-all-errors[3]
 
 import contextlib
 from abc import ABCMeta, abstractmethod
-from dataclasses import dataclass
+from dataclasses import asdict, dataclass
 from functools import partial
-from typing import Any, Callable, Iterator, Optional, Tuple, TypeVar, Union
+from typing import Any, Callable, Dict, Iterator, Optional, Tuple, TypeVar, Union
 
 import torch
 from pyre_extensions import none_throws
 from torch.cuda.amp import GradScaler
 from torch.distributed.algorithms._checkpoint.checkpoint_wrapper import (
     apply_activation_checkpointing,
     checkpoint_wrapper,
@@ -70,23 +70,26 @@
     anneal_epochs: int
     anneal_strategy: str = "linear"
     lr: float = 0.05
     avg_fn: Optional[TSWA_avg_fn] = None
 
 
 @dataclass
-class TorchDynamoParams:
+class TorchCompileParams:
     """
-    Dataclass to store parameters for torchdynamo.
-
-    Args:
-        backend: a string backend name in `torch._dynamo.list_backends()`
+    Dataclass to store parameters for torch compile. See https://pytorch.org/docs/stable/generated/torch.compile.html for details.
     """
 
-    backend: str
+    fullgraph: bool = False
+    dynamic: bool = False
+    # pyre-ignore: Invalid type parameters [24]
+    backend: Union[str, Callable] = "inductor"
+    mode: Union[str, None] = None
+    options: Optional[Dict[str, Union[str, int, bool]]] = None
+    disable: bool = False
 
 
 @dataclass
 class ActivationCheckpointParams:
     """
     Dataclass to store parameters for activation checkpointing.
 
@@ -141,15 +144,15 @@
     def __init__(
         self,
         *,
         module: torch.nn.Module,
         device: Optional[torch.device] = None,
         strategy: Optional[Union[Strategy, str]] = None,
         precision: Optional[Union[str, torch.dtype]] = None,
-        torchdynamo_params: Optional[TorchDynamoParams] = None,
+        torch_compile_params: Optional[TorchCompileParams] = None,
     ) -> None:
         """
         AutoPredictUnit is a convenience for users who are running inference and would like to have certain features handled for them, such as:
         - Moving data to the correct device.
         - Running inference under a mixed precision context.
         - Handling data parallel replication, especially if the module cannot fit on a single device using FullyShardedDataParallel.
         - Profiling the data transfer to device and forward pass.
@@ -162,21 +165,21 @@
         For more advanced customization, directly use the :class:`~torchtnt.framework.unit.PredictUnit` interface.
 
         Args:
             module: module to be used during prediction.
             device: the device to be used.
             precision: the precision to use in training, as either a string or a torch.dtype.
             strategy: the data parallelization strategy to be used. if a string, must be one of ``ddp`` or ``fsdp``.
-            torchdynamo_params: params for TorchDynamo https://pytorch.org/docs/stable/dynamo/index.html
+            torch_compile_params: params for Torch compile https://pytorch.org/docs/stable/generated/torch.compile.html
 
         Note:
-            TorchDynamo support is only available in PyTorch 2.0 or higher.
+            Torch compile support is only available in PyTorch 2.0 or higher.
         """
-        if torchdynamo_params:
-            _validate_torchdynamo_available()
+        if torch_compile_params:
+            _validate_torch_compile_available()
 
         super().__init__()
 
         self.device: torch.device = device or init_from_env()
         self.precision: Optional[torch.dtype]
         if isinstance(precision, str):
             self.precision = _convert_precision_str_to_dtype(precision)
@@ -189,32 +192,37 @@
             dtype=self.precision,
             enabled=self.precision is not None,
         )
         if strategy:
             if isinstance(strategy, str):
                 strategy = _convert_str_to_strategy(strategy)
             if isinstance(strategy, DDPStrategy):
-                if torchdynamo_params:
-                    # TODO: Add support for dynamo and DDP
-                    rank_zero_warn(
-                        "Torchdynamo params has been set with DDP - Note that performance will likely be slower and we recommend using only one."
+                if torch_compile_params and strategy.static_graph is True:
+                    # https://dev-discuss.pytorch.org/t/torchdynamo-update-9-making-ddp-work-with-torchdynamo/860
+                    raise RuntimeError(
+                        "Torch compile requires DDPStrategy's static_graph to be False"
                     )
                 module = prepare_ddp(module, self.device, strategy)
             elif isinstance(strategy, FSDPStrategy):
+                if torch_compile_params and strategy.use_orig_params is False:
+                    # as stated here https://pytorch.org/get-started/pytorch-2.0/
+                    rank_zero_warn(
+                        "We recommend setting FSDPStrategy's use_orig_params to True when using torch compile."
+                    )
                 module = prepare_fsdp(
                     module,
                     self.device,
                     strategy,
                     self.precision,
                 )
         else:
             module = module.to(self.device)
-        if torchdynamo_params:
+        if torch_compile_params:
             # use in-place compile to avoid altering the state_dict keys
-            module.compile(backend=torchdynamo_params.backend)
+            module.compile(**asdict(torch_compile_params))
         self.module: torch.nn.Module = module
 
         # cuda stream to use for moving data to device
         self._prefetch_stream: Optional[torch.cuda.streams.Stream] = (
             torch.cuda.Stream() if self.device.type == "cuda" else None
         )
         # the next batch which has been prefetched and is ready to be used
@@ -363,23 +371,23 @@
         step_lr_interval: whether to step lr_scheduler every step or every epoch. Defaults to every epoch.
         precision: the precision to use in training/evaluation, as either a string or a torch.dtype.
         gradient_accumulation_steps: how many batches to accumulate gradients over.
         detect_anomaly: whether to enable anomaly detection for the autograd engine https://pytorch.org/docs/stable/autograd.html#anomaly-detection
         clip_grad_norm: max norm of the gradients for clipping https://pytorch.org/docs/stable/generated/torch.nn.utils.clip_grad_norm_.html
         clip_grad_value: max value of the gradients for clipping https://pytorch.org/docs/stable/generated/torch.nn.utils.clip_grad_value_.html
         swa_params: params for stochastic weight averaging https://pytorch.org/docs/stable/optim.html#stochastic-weight-averaging
-        torchdynamo_params: params for TorchDynamo https://pytorch.org/docs/stable/dynamo/index.html
+        torch_compile_params: params for Torch compile https://pytorch.org/docs/stable/generated/torch.compile.html
         activation_checkpoint_params: params for enabling activation checkpointing
         training: if True, the optimizer and optionally LR scheduler will be created after the class is initialized.
 
     Note:
         Stochastic Weight Averaging is currently not supported with the FSDP strategy.
 
     Note:
-        TorchDynamo support is only available in PyTorch 2.0 or higher.
+        Torch compile support is only available in PyTorch 2.0 or higher.
 
     """
 
     def __init__(
         self,
         *,
         module: torch.nn.Module,
@@ -388,49 +396,53 @@
         step_lr_interval: Literal["step", "epoch"] = "epoch",
         precision: Optional[Union[str, torch.dtype]] = None,
         gradient_accumulation_steps: int = 1,
         detect_anomaly: Optional[bool] = None,
         clip_grad_norm: Optional[float] = None,
         clip_grad_value: Optional[float] = None,
         swa_params: Optional[SWAParams] = None,
-        torchdynamo_params: Optional[TorchDynamoParams] = None,
+        torch_compile_params: Optional[TorchCompileParams] = None,
         activation_checkpoint_params: Optional[ActivationCheckpointParams] = None,
         training: bool = True,
     ) -> None:
         super().__init__()
 
         if not gradient_accumulation_steps > 0:
             raise ValueError(
                 f"gradient_accumulation_steps must be > 0. Got {gradient_accumulation_steps}"
             )
-        if torchdynamo_params:
-            _validate_torchdynamo_available()
+        if torch_compile_params:
+            _validate_torch_compile_available()
 
         self.device: torch.device = device or init_from_env()
         self.precision: Optional[torch.dtype]
         if isinstance(precision, str):
             self.precision = _convert_precision_str_to_dtype(precision)
         else:
             self.precision = precision
 
         if strategy:
             if isinstance(strategy, str):
                 strategy = _convert_str_to_strategy(strategy)
             if isinstance(strategy, DDPStrategy):
-                if torchdynamo_params:
-                    # TODO: Add support for dynamo and DDP
-                    rank_zero_warn(
-                        "Torchdynamo params has been set with DDP - Note that performance will likely be slower and we recommend using only one."
+                if torch_compile_params and strategy.static_graph is True:
+                    # https://dev-discuss.pytorch.org/t/torchdynamo-update-9-making-ddp-work-with-torchdynamo/860
+                    raise RuntimeError(
+                        "Torch compile requires DDPStrategy's static_graph to be False"
                     )
                 module = prepare_ddp(module, self.device, strategy)
             elif isinstance(strategy, FSDPStrategy):
                 if swa_params:
                     raise RuntimeError(
                         "Stochastic Weight Averaging is currently not supported with the FSDP strategy"
                     )
+                # as stated here https://pytorch.org/get-started/pytorch-2.0/
+                rank_zero_warn(
+                    "We recommend setting FSDPStrategy's use_original_params to True when using torch compile."
+                )
                 module = prepare_fsdp(module, self.device, strategy, self.precision)
         else:
             module = module.to(self.device)
 
         if activation_checkpoint_params:
             checkpoint_impl = activation_checkpoint_params.checkpoint_impl
             check_fn = activation_checkpoint_params.check_fn
@@ -447,21 +459,22 @@
         self.grad_scaler: Optional[GradScaler] = None
         if self.precision:
             self.grad_scaler = _get_grad_scaler_from_precision(
                 self.precision,
                 module,
             )
 
-        if torchdynamo_params:
+        if torch_compile_params:
             # pyre-ignore
             self.compute_loss = torch.compile(
-                self.compute_loss, backend=torchdynamo_params.backend
+                self.compute_loss,
+                **asdict(torch_compile_params),
             )
             # use in-place compile to avoid altering the state_dict keys
-            module.compile(backend=torchdynamo_params.backend)
+            module.compile(**asdict(torch_compile_params))
 
         self.module: torch.nn.Module = module
 
         self.step_lr_interval = step_lr_interval
 
         self.gradient_accumulation_steps = gradient_accumulation_steps
 
@@ -653,15 +666,14 @@
                     scaled_loss.backward()
             else:
                 with _get_timing_context(state, f"{self.__class__.__name__}.backward"):
                     loss.backward()
 
         if should_update_weights:
             # Run gradient clipping, optimizer step, and zero_grad
-            # TODO try to use dynamo here
             clip_grad_norm = self.clip_grad_norm
             clip_grad_value = self.clip_grad_value
             if grad_scaler and (clip_grad_norm or clip_grad_value):
                 # unscale the gradients of optimizer's assigned params in-place in preparation for gradient clipping
                 with _get_timing_context(
                     state, f"{self.__class__.__name__}.grad_unscale"
                 ):
@@ -823,18 +835,18 @@
             step: how many steps have been completed (``train_step``s when running fit and ``eval_step``s when running evaluation)
             loss: the loss computed in the ``compute_loss`` function
             outputs: the outputs of the model forward pass
         """
         pass
 
 
-def _validate_torchdynamo_available() -> None:
+def _validate_torch_compile_available() -> None:
     if not is_torch_version_ge_1_13_1():
         raise RuntimeError(
-            "TorchDynamo support is available only in PyTorch 2.0 or higher. "
+            "Torch compile support is available only in PyTorch 2.0 or higher. "
             "Please install PyTorch 2.0 or higher to continue: https://pytorch.org/get-started/locally/"
         )
 
 
 def _convert_precision_str_to_dtype(precision: str) -> Optional[torch.dtype]:
     """
     Converts precision as a string to a torch.dtype
```

### Comparing `torchtnt-nightly-2023.7.6/torchtnt/framework/callback.py` & `torchtnt-nightly-2023.7.7/torchtnt/framework/callback.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.7.6/torchtnt/framework/callbacks/__init__.py` & `torchtnt-nightly-2023.7.7/torchtnt/framework/callbacks/__init__.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.7.6/torchtnt/framework/callbacks/base_csv_writer.py` & `torchtnt-nightly-2023.7.7/torchtnt/framework/callbacks/base_csv_writer.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.7.6/torchtnt/framework/callbacks/garbage_collector.py` & `torchtnt-nightly-2023.7.7/torchtnt/framework/callbacks/garbage_collector.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.7.6/torchtnt/framework/callbacks/lambda_callback.py` & `torchtnt-nightly-2023.7.7/torchtnt/framework/callbacks/lambda_callback.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.7.6/torchtnt/framework/callbacks/learning_rate_monitor.py` & `torchtnt-nightly-2023.7.7/torchtnt/framework/callbacks/learning_rate_monitor.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.7.6/torchtnt/framework/callbacks/module_summary.py` & `torchtnt-nightly-2023.7.7/torchtnt/framework/callbacks/module_summary.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.7.6/torchtnt/framework/callbacks/pytorch_profiler.py` & `torchtnt-nightly-2023.7.7/torchtnt/framework/callbacks/pytorch_profiler.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.7.6/torchtnt/framework/callbacks/system_resources_monitor.py` & `torchtnt-nightly-2023.7.7/torchtnt/framework/callbacks/system_resources_monitor.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.7.6/torchtnt/framework/callbacks/tensorboard_parameter_monitor.py` & `torchtnt-nightly-2023.7.7/torchtnt/framework/callbacks/tensorboard_parameter_monitor.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.7.6/torchtnt/framework/callbacks/torchsnapshot_saver.py` & `torchtnt-nightly-2023.7.7/torchtnt/framework/callbacks/torchsnapshot_saver.py`

 * *Files 4% similar despite different names*

```diff
@@ -71,21 +71,21 @@
         dirpath: str,
         *,
         save_every_n_train_steps: Optional[int] = None,
         save_every_n_epochs: Optional[int] = None,
         replicated: Optional[List[str]] = None,
     ) -> None:
         _validate_snapshot_available()
-        if save_every_n_train_steps is not None and save_every_n_train_steps < 0:
+        if save_every_n_train_steps is not None and save_every_n_train_steps <= 0:
             raise ValueError(
-                f"Invalid value passed for save_every_n_train_steps. Expected to receive either None or non-negative number, but received {save_every_n_train_steps}"
+                f"Invalid value passed for save_every_n_train_steps. Expected to receive either None or positive number, but received {save_every_n_train_steps}"
             )
-        if save_every_n_epochs is not None and save_every_n_epochs < 0:
+        if save_every_n_epochs is not None and save_every_n_epochs <= 0:
             raise ValueError(
-                f"Invalid value passed for save_every_n_epochs. Expected to receive either None or non-negative number, but received {save_every_n_epochs}"
+                f"Invalid value passed for save_every_n_epochs. Expected to receive either None or positive number, but received {save_every_n_epochs}"
             )
         self._save_every_n_epochs = save_every_n_epochs
         self._save_every_n_train_steps = save_every_n_train_steps
         self._sync_dirpath_to_all_ranks(dirpath)
         self._replicated: Set[str] = set(replicated or [])
 
         self._prev_snapshot: Optional[PendingSnapshot] = None
@@ -111,69 +111,55 @@
 
     def on_train_start(self, state: State, unit: TTrainUnit) -> None:
         """Validate there's no key collision for the app state."""
         app_state = _app_state(unit)
         _check_app_state_collision(app_state)
 
     def on_train_step_end(self, state: State, unit: TTrainUnit) -> None:
-        train_state = none_throws(state.train_state)
+        train_progress = none_throws(state.train_state).progress
 
-        num_steps_completed = train_state.progress.num_steps_completed
+        num_steps_completed = train_progress.num_steps_completed
         save_every_n_train_steps = self._save_every_n_train_steps
         if (
             save_every_n_train_steps is None
             or num_steps_completed % save_every_n_train_steps != 0
         ):
             return
 
         app_state = _get_app_state(state, unit, self._replicated, intra_epoch=True)
-
-        # save snapshot to predetermined path
-        # TODO: discuss whether this path should be customized
-        epoch = train_state.progress.num_epochs_completed
+        epoch = train_progress.num_epochs_completed
         snapshot_path = _get_snapshot_save_path(
             self._dirpath, epoch, num_steps_completed
         )
         self._async_snapshot(snapshot_path, app_state, wait=False)
 
     def on_train_epoch_end(self, state: State, unit: TTrainUnit) -> None:
-        train_state = none_throws(state.train_state)
+        train_progress = none_throws(state.train_state).progress
 
-        train_progress = train_state.progress
         epoch = train_progress.num_epochs_completed
         save_every_n_epochs = self._save_every_n_epochs
         if save_every_n_epochs is None or epoch % save_every_n_epochs != 0:
             return
 
-        app_state = _get_app_state(
-            state, unit, replicated=self._replicated, intra_epoch=False
-        )
-
-        # save snapshot to predetermined path
-        # TODO: discuss whether this path should be customized
+        app_state = _get_app_state(state, unit, self._replicated, intra_epoch=False)
         num_steps_completed = train_progress.num_steps_completed
         snapshot_path = _get_snapshot_save_path(
             self._dirpath, epoch, num_steps_completed
         )
         self._async_snapshot(snapshot_path, app_state, wait=True)
 
     def on_train_end(self, state: State, unit: TTrainUnit) -> None:
-        train_state = none_throws(state.train_state)
-        num_steps_completed = train_state.progress.num_steps_completed
-
         app_state = _get_app_state(state, unit, self._replicated, intra_epoch=False)
-
-        # save snapshot to predetermined path
-        # TODO: discuss whether this path should be customized
-        epoch = train_state.progress.num_epochs_completed
+        train_progress = none_throws(state.train_state).progress
+        num_steps_completed = train_progress.num_steps_completed
+        epoch = train_progress.num_epochs_completed
         snapshot_path = _get_snapshot_save_path(
             self._dirpath, epoch, num_steps_completed
         )
-        self._async_snapshot(snapshot_path, app_state, wait=False)
-
+        self._async_snapshot(snapshot_path, app_state, wait=True)
         self._wait()
 
     def on_exception(
         self,
         state: State,
         unit: Union[TTrainUnit, TEvalUnit, TPredictUnit],
         exc: BaseException,
@@ -265,14 +251,15 @@
             "TorchSnapshotSaver support requires torchsnapshot. "
             "Please make sure ``torchsnapshot`` is installed. "
             "Installation: https://github.com/pytorch/torchsnapshot#install"
         )
 
 
 def _get_snapshot_save_path(dirpath: str, epoch: int, step: int) -> str:
+    # TODO: discuss whether this path should be customized
     return os.path.join(dirpath, f"epoch_{epoch}_step_{step}")
 
 
 def _app_state(unit: AppStateMixin) -> Dict[str, Any]:
     """Join together all of the tracked stateful entities to simplify registration of snapshottable states, deals with FSDP case"""
     app_state = unit.app_state()
     tracked_optimizers = _construct_tracked_optimizers(unit)  # handles fsdp
```

### Comparing `torchtnt-nightly-2023.7.6/torchtnt/framework/callbacks/tqdm_progress_bar.py` & `torchtnt-nightly-2023.7.7/torchtnt/framework/callbacks/tqdm_progress_bar.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.7.6/torchtnt/framework/callbacks/train_progress_monitor.py` & `torchtnt-nightly-2023.7.7/torchtnt/framework/callbacks/train_progress_monitor.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.7.6/torchtnt/framework/evaluate.py` & `torchtnt-nightly-2023.7.7/torchtnt/framework/evaluate.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.7.6/torchtnt/framework/fit.py` & `torchtnt-nightly-2023.7.7/torchtnt/framework/fit.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.7.6/torchtnt/framework/predict.py` & `torchtnt-nightly-2023.7.7/torchtnt/framework/predict.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.7.6/torchtnt/framework/state.py` & `torchtnt-nightly-2023.7.7/torchtnt/framework/state.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.7.6/torchtnt/framework/train.py` & `torchtnt-nightly-2023.7.7/torchtnt/framework/train.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.7.6/torchtnt/framework/unit.py` & `torchtnt-nightly-2023.7.7/torchtnt/framework/unit.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.7.6/torchtnt/framework/utils.py` & `torchtnt-nightly-2023.7.7/torchtnt/framework/utils.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.7.6/torchtnt/utils/__init__.py` & `torchtnt-nightly-2023.7.7/torchtnt/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.7.6/torchtnt/utils/data/__init__.py` & `torchtnt-nightly-2023.7.7/torchtnt/utils/data/__init__.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.7.6/torchtnt/utils/data/data_prefetcher.py` & `torchtnt-nightly-2023.7.7/torchtnt/utils/data/data_prefetcher.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.7.6/torchtnt/utils/data/iterators.py` & `torchtnt-nightly-2023.7.7/torchtnt/utils/data/iterators.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.7.6/torchtnt/utils/data/multi_dataloader.py` & `torchtnt-nightly-2023.7.7/torchtnt/utils/data/multi_dataloader.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.7.6/torchtnt/utils/data/profile_dataloader.py` & `torchtnt-nightly-2023.7.7/torchtnt/utils/data/profile_dataloader.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.7.6/torchtnt/utils/device.py` & `torchtnt-nightly-2023.7.7/torchtnt/utils/device.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.7.6/torchtnt/utils/distributed.py` & `torchtnt-nightly-2023.7.7/torchtnt/utils/distributed.py`

 * *Files 1% similar despite different names*

```diff
@@ -411,15 +411,14 @@
             with torch.no_grad():
                 module_output.weight = module.weight
                 module_output.bias = module.bias
         module_output.running_mean = module.running_mean
         module_output.running_var = module.running_var
         module_output.num_batches_tracked = module.num_batches_tracked
         if hasattr(module, "qconfig"):
-            # pyre-ignore[16]: `_BatchNormXd` has no attribute `qconfig`.
             module_output.qconfig = module.qconfig
     for name, child in module.named_children():
         module_output.add_module(name, revert_sync_batchnorm(child, device))
     del module
     return module_output
```

### Comparing `torchtnt-nightly-2023.7.6/torchtnt/utils/early_stop_checker.py` & `torchtnt-nightly-2023.7.7/torchtnt/utils/early_stop_checker.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.7.6/torchtnt/utils/env.py` & `torchtnt-nightly-2023.7.7/torchtnt/utils/env.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.7.6/torchtnt/utils/fsspec.py` & `torchtnt-nightly-2023.7.7/torchtnt/utils/fsspec.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.7.6/torchtnt/utils/loggers/__init__.py` & `torchtnt-nightly-2023.7.7/torchtnt/utils/loggers/__init__.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.7.6/torchtnt/utils/loggers/csv.py` & `torchtnt-nightly-2023.7.7/torchtnt/utils/loggers/csv.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.7.6/torchtnt/utils/loggers/file.py` & `torchtnt-nightly-2023.7.7/torchtnt/utils/loggers/file.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.7.6/torchtnt/utils/loggers/in_memory.py` & `torchtnt-nightly-2023.7.7/torchtnt/utils/loggers/in_memory.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.7.6/torchtnt/utils/loggers/json.py` & `torchtnt-nightly-2023.7.7/torchtnt/utils/loggers/json.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.7.6/torchtnt/utils/loggers/logger.py` & `torchtnt-nightly-2023.7.7/torchtnt/utils/loggers/logger.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.7.6/torchtnt/utils/loggers/tensorboard.py` & `torchtnt-nightly-2023.7.7/torchtnt/utils/loggers/tensorboard.py`

 * *Files 3% similar despite different names*

```diff
@@ -156,14 +156,25 @@
             *args (Any): Positional arguments passed to SummaryWriter.add_images
             **kwargs(Any): Keyword arguments passed to SummaryWriter.add_images
         """
         writer = self._writer
         if writer:
             writer.add_images(*args, **kwargs)
 
+    def log_audio(self, *args: Any, **kwargs: Any) -> None:
+        """Add audio data to TensorBoard.
+
+        Args:
+            *args (Any): Positional arguments passed to SummaryWriter.add_audio
+            **kwargs (Any): Keyword arguments passed to SummaryWriter.add_audio
+        """
+        writer = self._writer
+        if writer:
+            writer.add_audio(*args, **kwargs)
+
     def flush(self) -> None:
         """Writes pending logs to disk."""
 
         if self._writer:
             self._writer.flush()
 
     def close(self) -> None:
```

### Comparing `torchtnt-nightly-2023.7.6/torchtnt/utils/loggers/utils.py` & `torchtnt-nightly-2023.7.7/torchtnt/utils/loggers/utils.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.7.6/torchtnt/utils/memory.py` & `torchtnt-nightly-2023.7.7/torchtnt/utils/memory.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.7.6/torchtnt/utils/misc.py` & `torchtnt-nightly-2023.7.7/torchtnt/utils/misc.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.7.6/torchtnt/utils/oom.py` & `torchtnt-nightly-2023.7.7/torchtnt/utils/oom.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.7.6/torchtnt/utils/prepare_model.py` & `torchtnt-nightly-2023.7.7/torchtnt/utils/prepare_model.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.7.6/torchtnt/utils/progress.py` & `torchtnt-nightly-2023.7.7/torchtnt/utils/progress.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.7.6/torchtnt/utils/rank_zero_log.py` & `torchtnt-nightly-2023.7.7/torchtnt/utils/rank_zero_log.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.7.6/torchtnt/utils/test_utils.py` & `torchtnt-nightly-2023.7.7/torchtnt/utils/test_utils.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.7.6/torchtnt/utils/timer.py` & `torchtnt-nightly-2023.7.7/torchtnt/utils/timer.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.7.6/torchtnt/utils/tqdm.py` & `torchtnt-nightly-2023.7.7/torchtnt/utils/tqdm.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.7.6/torchtnt/utils/version.py` & `torchtnt-nightly-2023.7.7/torchtnt/utils/version.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.7.6/torchtnt_nightly.egg-info/PKG-INFO` & `torchtnt-nightly-2023.7.7/torchtnt_nightly.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torchtnt-nightly
-Version: 2023.7.6
+Version: 2023.7.7
 Summary: A lightweight library for PyTorch training tools and utilities
 Home-page: https://github.com/pytorch/tnt
 Author: PyTorch
 Author-email: daniellepintz@fb.com
 License: BSD-3
 Keywords: pytorch,torch,training,tools,utilities
 Classifier: Development Status :: 2 - Pre-Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: torchtnt-nightly Version: 2023.7.6 Summary: A
+Metadata-Version: 2.1 Name: torchtnt-nightly Version: 2023.7.7 Summary: A
 lightweight library for PyTorch training tools and utilities Home-page: https:/
 /github.com/pytorch/tnt Author: PyTorch Author-email: daniellepintz@fb.com
 License: BSD-3 Keywords: pytorch,torch,training,tools,utilities Classifier:
 Development Status :: 2 - Pre-Alpha Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research Classifier: License :: OSI
 Approved :: BSD License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7 Classifier: Topic ::
```

### Comparing `torchtnt-nightly-2023.7.6/torchtnt_nightly.egg-info/SOURCES.txt` & `torchtnt-nightly-2023.7.7/torchtnt_nightly.egg-info/SOURCES.txt`

 * *Files identical despite different names*

