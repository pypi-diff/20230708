# Comparing `tmp/hyfi-1.0.5.tar.gz` & `tmp/hyfi-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyfi-1.0.5.tar", max compression
+gzip compressed data, was "hyfi-1.1.0.tar", max compression
```

## Comparing `hyfi-1.0.5.tar` & `hyfi-1.1.0.tar`

### file list

```diff
@@ -1,109 +1,110 @@
--rw-r--r--   0        0        0     1071 2023-07-05 23:58:53.756217 hyfi-1.0.5/LICENSE
--rw-r--r--   0        0        0     1881 2023-07-05 23:58:53.756217 hyfi-1.0.5/README.md
--rw-r--r--   0        0        0     4863 2023-07-05 23:59:18.488518 hyfi-1.0.5/pyproject.toml
--rw-r--r--   0        0        0     4267 2023-07-05 23:58:53.760217 hyfi-1.0.5/src/hyfi/__cli__.py
--rw-r--r--   0        0        0     2550 2023-07-05 23:58:53.760217 hyfi-1.0.5/src/hyfi/__click__.py
--rw-r--r--   0        0        0      788 2023-07-05 23:58:53.760217 hyfi-1.0.5/src/hyfi/__global__/__init__.py
--rw-r--r--   0        0        0     9245 2023-07-05 23:58:53.760217 hyfi-1.0.5/src/hyfi/__global__/config.py
--rw-r--r--   0        0        0      733 2023-07-05 23:58:53.760217 hyfi-1.0.5/src/hyfi/__init__.py
--rw-r--r--   0        0        0       22 2023-07-05 23:59:18.412517 hyfi-1.0.5/src/hyfi/_version.py
--rw-r--r--   0        0        0     1890 2023-07-05 23:58:53.760217 hyfi-1.0.5/src/hyfi/about/__init__.py
--rw-r--r--   0        0        0     7229 2023-07-05 23:58:53.760217 hyfi-1.0.5/src/hyfi/batch/__init__.py
--rw-r--r--   0        0        0     1206 2023-07-05 23:58:53.760217 hyfi-1.0.5/src/hyfi/cached_path/__init__.py
--rw-r--r--   0        0        0    14373 2023-07-05 23:58:53.760217 hyfi-1.0.5/src/hyfi/cached_path/_cached_path.py
--rw-r--r--   0        0        0     1619 2023-07-05 23:58:53.760217 hyfi-1.0.5/src/hyfi/cached_path/cache_file.py
--rw-r--r--   0        0        0     1100 2023-07-05 23:58:53.760217 hyfi-1.0.5/src/hyfi/cached_path/common.py
--rw-r--r--   0        0        0     1921 2023-07-05 23:58:53.760217 hyfi-1.0.5/src/hyfi/cached_path/file_lock.py
--rw-r--r--   0        0        0     3441 2023-07-05 23:58:53.760217 hyfi-1.0.5/src/hyfi/cached_path/meta.py
--rw-r--r--   0        0        0     3247 2023-07-05 23:58:53.760217 hyfi-1.0.5/src/hyfi/cached_path/progress.py
--rw-r--r--   0        0        0     1437 2023-07-05 23:58:53.760217 hyfi-1.0.5/src/hyfi/cached_path/schemes/__init__.py
--rw-r--r--   0        0        0     1815 2023-07-05 23:58:53.760217 hyfi-1.0.5/src/hyfi/cached_path/schemes/beaker.py
--rw-r--r--   0        0        0     2862 2023-07-05 23:58:53.760217 hyfi-1.0.5/src/hyfi/cached_path/schemes/hf.py
--rw-r--r--   0        0        0     2942 2023-07-05 23:58:53.760217 hyfi-1.0.5/src/hyfi/cached_path/schemes/http.py
--rw-r--r--   0        0        0     3645 2023-07-05 23:58:53.760217 hyfi-1.0.5/src/hyfi/cached_path/schemes/scheme_client.py
--rw-r--r--   0        0        0     1222 2023-07-05 23:58:53.760217 hyfi-1.0.5/src/hyfi/cached_path/testing.py
--rw-r--r--   0        0        0     4799 2023-07-05 23:58:53.760217 hyfi-1.0.5/src/hyfi/cached_path/util.py
--rw-r--r--   0        0        0      464 2023-07-05 23:58:53.760217 hyfi-1.0.5/src/hyfi/cached_path/version.py
--rw-r--r--   0        0        0    32964 2023-07-05 23:58:53.760217 hyfi-1.0.5/src/hyfi/composer/__init__.py
--rw-r--r--   0        0        0     7421 2023-07-05 23:58:53.760217 hyfi-1.0.5/src/hyfi/composer/extended.py
--rw-r--r--   0        0        0        0 2023-07-05 23:58:53.760217 hyfi-1.0.5/src/hyfi/conf/__init__.py
--rw-r--r--   0        0        0      233 2023-07-05 23:59:18.412517 hyfi-1.0.5/src/hyfi/conf/about/__init__.yaml
--rw-r--r--   0        0        0      553 2023-07-05 23:58:53.760217 hyfi-1.0.5/src/hyfi/conf/batch/__init__.yaml
--rw-r--r--   0        0        0        0 2023-07-05 23:58:53.760217 hyfi-1.0.5/src/hyfi/conf/cmd/__init__.yaml
--rw-r--r--   0        0        0       49 2023-07-05 23:58:53.760217 hyfi-1.0.5/src/hyfi/conf/cmd/about.yaml
--rw-r--r--   0        0        0      155 2023-07-05 23:58:53.760217 hyfi-1.0.5/src/hyfi/conf/cmd/copy_conf.yaml
--rw-r--r--   0        0        0       83 2023-07-05 23:58:53.760217 hyfi-1.0.5/src/hyfi/conf/cmd/run_task.yaml
--rw-r--r--   0        0        0       91 2023-07-05 23:58:53.760217 hyfi-1.0.5/src/hyfi/conf/cmd/run_workflow.yaml
--rw-r--r--   0        0        0      320 2023-07-05 23:58:53.760217 hyfi-1.0.5/src/hyfi/conf/config.yaml
--rw-r--r--   0        0        0      569 2023-07-05 23:58:53.760217 hyfi-1.0.5/src/hyfi/conf/copier/conf.yaml
--rw-r--r--   0        0        0      709 2023-07-05 23:58:53.760217 hyfi-1.0.5/src/hyfi/conf/dotenv/__init__.yaml
--rw-r--r--   0        0        0      319 2023-07-05 23:58:53.760217 hyfi-1.0.5/src/hyfi/conf/hconf.yaml
--rw-r--r--   0        0        0     1128 2023-07-05 23:58:53.760217 hyfi-1.0.5/src/hyfi/conf/hydra/help/help.yaml
--rw-r--r--   0        0        0      264 2023-07-05 23:58:53.760217 hyfi-1.0.5/src/hyfi/conf/hydra/job_logging/custom.yaml
--rw-r--r--   0        0        0      137 2023-07-05 23:58:53.760217 hyfi-1.0.5/src/hyfi/conf/joblib/__init__.yaml
--rw-r--r--   0        0        0      217 2023-07-05 23:58:53.760217 hyfi-1.0.5/src/hyfi/conf/mode/__debug__.yaml
--rw-r--r--   0        0        0      921 2023-07-05 23:58:53.760217 hyfi-1.0.5/src/hyfi/conf/mode/__init__.yaml
--rw-r--r--   0        0        0       61 2023-07-05 23:58:53.760217 hyfi-1.0.5/src/hyfi/conf/module/__init__.yaml
--rw-r--r--   0        0        0       73 2023-07-05 23:58:53.760217 hyfi-1.0.5/src/hyfi/conf/path/__batch__.yaml
--rw-r--r--   0        0        0      880 2023-07-05 23:58:53.760217 hyfi-1.0.5/src/hyfi/conf/path/__init__.yaml
--rw-r--r--   0        0        0      133 2023-07-05 23:58:53.760217 hyfi-1.0.5/src/hyfi/conf/path/__task__.yaml
--rw-r--r--   0        0        0      291 2023-07-05 23:58:53.760217 hyfi-1.0.5/src/hyfi/conf/path/dirnames/__init__.yaml
--rw-r--r--   0        0        0       76 2023-07-05 23:58:53.760217 hyfi-1.0.5/src/hyfi/conf/pipe/__dataframe__.yaml
--rw-r--r--   0        0        0       77 2023-07-05 23:58:53.760217 hyfi-1.0.5/src/hyfi/conf/pipe/__dataframe_external_funcs__.yaml
--rw-r--r--   0        0        0       79 2023-07-05 23:58:53.760217 hyfi-1.0.5/src/hyfi/conf/pipe/__dataframe_instance_methods__.yaml
--rw-r--r--   0        0        0       70 2023-07-05 23:58:53.760217 hyfi-1.0.5/src/hyfi/conf/pipe/__general_external_funcs__.yaml
--rw-r--r--   0        0        0       72 2023-07-05 23:58:53.760217 hyfi-1.0.5/src/hyfi/conf/pipe/__general_instance_methods__.yaml
--rw-r--r--   0        0        0      128 2023-07-05 23:58:53.760217 hyfi-1.0.5/src/hyfi/conf/pipe/__init__.yaml
--rw-r--r--   0        0        0      236 2023-07-05 23:58:53.760217 hyfi-1.0.5/src/hyfi/conf/pipe/load_dataframes.yaml
--rw-r--r--   0        0        0      241 2023-07-05 23:58:53.760217 hyfi-1.0.5/src/hyfi/conf/pipe/save_dataframes.yaml
--rw-r--r--   0        0        0       90 2023-07-05 23:58:53.760217 hyfi-1.0.5/src/hyfi/conf/pipe/test_preprocessing.yaml
--rw-r--r--   0        0        0       69 2023-07-05 23:58:53.760217 hyfi-1.0.5/src/hyfi/conf/pipeline/__init__.yaml
--rw-r--r--   0        0        0      388 2023-07-05 23:58:53.760217 hyfi-1.0.5/src/hyfi/conf/pipeline/__test_dataframe__.yaml
--rw-r--r--   0        0        0      268 2023-07-05 23:58:53.760217 hyfi-1.0.5/src/hyfi/conf/pipeline/__test_general__.yaml
--rw-r--r--   0        0        0      744 2023-07-05 23:58:53.760217 hyfi-1.0.5/src/hyfi/conf/project/__init__.yaml
--rw-r--r--   0        0        0      170 2023-07-05 23:58:53.760217 hyfi-1.0.5/src/hyfi/conf/project/__test__.yaml
--rw-r--r--   0        0        0       38 2023-07-05 23:58:53.760217 hyfi-1.0.5/src/hyfi/conf/running/__init__.yaml
--rw-r--r--   0        0        0      161 2023-07-05 23:58:53.760217 hyfi-1.0.5/src/hyfi/conf/task/__batch__.yaml
--rw-r--r--   0        0        0      359 2023-07-05 23:58:53.760217 hyfi-1.0.5/src/hyfi/conf/task/__init__.yaml
--rw-r--r--   0        0        0      378 2023-07-05 23:58:53.760217 hyfi-1.0.5/src/hyfi/conf/task/__test__.yaml
--rw-r--r--   0        0        0       99 2023-07-05 23:58:53.760217 hyfi-1.0.5/src/hyfi/conf/workflow/__init__.yaml
--rw-r--r--   0        0        0       99 2023-07-05 23:58:53.760217 hyfi-1.0.5/src/hyfi/conf/workflow/__test__.yaml
--rw-r--r--   0        0        0     6548 2023-07-05 23:58:53.760217 hyfi-1.0.5/src/hyfi/copier/__init__.py
--rw-r--r--   0        0        0     5915 2023-07-05 23:58:53.760217 hyfi-1.0.5/src/hyfi/dotenv/__init__.py
--rw-r--r--   0        0        0        0 2023-07-05 23:58:53.760217 hyfi-1.0.5/src/hyfi/graphics/__init__.py
--rw-r--r--   0        0        0     8470 2023-07-05 23:58:53.760217 hyfi-1.0.5/src/hyfi/graphics/collage.py
--rw-r--r--   0        0        0     4538 2023-07-05 23:58:53.760217 hyfi-1.0.5/src/hyfi/graphics/motion.py
--rw-r--r--   0        0        0     7020 2023-07-05 23:58:53.760217 hyfi-1.0.5/src/hyfi/graphics/utils.py
--rw-r--r--   0        0        0     4228 2023-07-05 23:58:53.760217 hyfi-1.0.5/src/hyfi/joblib/__init__.py
--rw-r--r--   0        0        0      111 2023-07-05 23:58:53.760217 hyfi-1.0.5/src/hyfi/joblib/batch/__init__.py
--rw-r--r--   0        0        0     6312 2023-07-05 23:58:53.760217 hyfi-1.0.5/src/hyfi/joblib/batch/apply.py
--rw-r--r--   0        0        0     4779 2023-07-05 23:58:53.760217 hyfi-1.0.5/src/hyfi/joblib/batch/apply_batch.py
--rw-r--r--   0        0        0    13823 2023-07-05 23:58:53.760217 hyfi-1.0.5/src/hyfi/joblib/batch/batcher.py
--rw-r--r--   0        0        0    50188 2023-07-05 23:58:53.764217 hyfi-1.0.5/src/hyfi/main/__init__.py
--rw-r--r--   0        0        0      280 2023-07-05 23:58:53.764217 hyfi-1.0.5/src/hyfi/module/__init__.py
--rw-r--r--   0        0        0     4915 2023-07-05 23:58:53.764217 hyfi-1.0.5/src/hyfi/path/__init__.py
--rw-r--r--   0        0        0     4183 2023-07-05 23:58:53.764217 hyfi-1.0.5/src/hyfi/path/base.py
--rw-r--r--   0        0        0      782 2023-07-05 23:58:53.764217 hyfi-1.0.5/src/hyfi/path/batch.py
--rw-r--r--   0        0        0      599 2023-07-05 23:58:53.764217 hyfi-1.0.5/src/hyfi/path/dirnames.py
--rw-r--r--   0        0        0     1609 2023-07-05 23:58:53.764217 hyfi-1.0.5/src/hyfi/path/task.py
--rw-r--r--   0        0        0     5030 2023-07-05 23:58:53.764217 hyfi-1.0.5/src/hyfi/pipe/__init__.py
--rw-r--r--   0        0        0     1455 2023-07-05 23:58:53.764217 hyfi-1.0.5/src/hyfi/pipe/test.py
--rw-r--r--   0        0        0     8085 2023-07-05 23:58:53.764217 hyfi-1.0.5/src/hyfi/pipeline/__init__.py
--rw-r--r--   0        0        0     2900 2023-07-05 23:58:53.764217 hyfi-1.0.5/src/hyfi/pipeline/configs.py
--rw-r--r--   0        0        0     5618 2023-07-05 23:58:53.764217 hyfi-1.0.5/src/hyfi/project/__init__.py
--rw-r--r--   0        0        0        0 2023-07-05 23:58:53.764217 hyfi-1.0.5/src/hyfi/py.typed
--rw-r--r--   0        0        0     4268 2023-07-05 23:58:53.764217 hyfi-1.0.5/src/hyfi/task/__init__.py
--rw-r--r--   0        0        0     7014 2023-07-05 23:58:53.764217 hyfi-1.0.5/src/hyfi/task/batch.py
--rw-r--r--   0        0        0        0 2023-07-05 23:58:53.764217 hyfi-1.0.5/src/hyfi/utils/__init__.py
--rw-r--r--   0        0        0     1314 2023-07-05 23:58:53.764217 hyfi-1.0.5/src/hyfi/utils/contexts.py
--rw-r--r--   0        0        0    30058 2023-07-05 23:58:53.764217 hyfi-1.0.5/src/hyfi/utils/datasets.py
--rw-r--r--   0        0        0     6568 2023-07-05 23:58:53.764217 hyfi-1.0.5/src/hyfi/utils/envs.py
--rw-r--r--   0        0        0    10857 2023-07-05 23:58:53.764217 hyfi-1.0.5/src/hyfi/utils/funcs.py
--rw-r--r--   0        0        0     3769 2023-07-05 23:58:53.764217 hyfi-1.0.5/src/hyfi/utils/gpumon.py
--rw-r--r--   0        0        0    20157 2023-07-05 23:58:53.764217 hyfi-1.0.5/src/hyfi/utils/iolibs.py
--rw-r--r--   0        0        0     2259 2023-07-05 23:58:53.764217 hyfi-1.0.5/src/hyfi/utils/logging.py
--rw-r--r--   0        0        0    12820 2023-07-05 23:58:53.764217 hyfi-1.0.5/src/hyfi/utils/notebooks.py
--rw-r--r--   0        0        0     6955 2023-07-05 23:58:53.764217 hyfi-1.0.5/src/hyfi/utils/packages.py
--rw-r--r--   0        0        0      382 2023-07-05 23:58:53.764217 hyfi-1.0.5/src/hyfi/utils/types.py
--rw-r--r--   0        0        0      753 2023-07-05 23:58:53.764217 hyfi-1.0.5/src/hyfi/workflow/__init__.py
--rw-r--r--   0        0        0     3393 1970-01-01 00:00:00.000000 hyfi-1.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-07-08 12:48:12.957773 hyfi-1.1.0/LICENSE
+-rw-r--r--   0        0        0     1881 2023-07-08 12:48:12.957773 hyfi-1.1.0/README.md
+-rw-r--r--   0        0        0     4863 2023-07-08 12:48:40.322071 hyfi-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     4206 2023-07-08 12:48:12.957773 hyfi-1.1.0/src/hyfi/__cli__.py
+-rw-r--r--   0        0        0     2550 2023-07-08 12:48:12.957773 hyfi-1.1.0/src/hyfi/__click__.py
+-rw-r--r--   0        0        0      788 2023-07-08 12:48:12.961773 hyfi-1.1.0/src/hyfi/__global__/__init__.py
+-rw-r--r--   0        0        0     9332 2023-07-08 12:48:12.961773 hyfi-1.1.0/src/hyfi/__global__/config.py
+-rw-r--r--   0        0        0      733 2023-07-08 12:48:12.961773 hyfi-1.1.0/src/hyfi/__init__.py
+-rw-r--r--   0        0        0       22 2023-07-08 12:48:40.246070 hyfi-1.1.0/src/hyfi/_version.py
+-rw-r--r--   0        0        0     2376 2023-07-08 12:48:12.961773 hyfi-1.1.0/src/hyfi/about/__init__.py
+-rw-r--r--   0        0        0     7229 2023-07-08 12:48:12.961773 hyfi-1.1.0/src/hyfi/batch/__init__.py
+-rw-r--r--   0        0        0     1206 2023-07-08 12:48:12.961773 hyfi-1.1.0/src/hyfi/cached_path/__init__.py
+-rw-r--r--   0        0        0    14373 2023-07-08 12:48:12.961773 hyfi-1.1.0/src/hyfi/cached_path/_cached_path.py
+-rw-r--r--   0        0        0     1619 2023-07-08 12:48:12.961773 hyfi-1.1.0/src/hyfi/cached_path/cache_file.py
+-rw-r--r--   0        0        0     1100 2023-07-08 12:48:12.961773 hyfi-1.1.0/src/hyfi/cached_path/common.py
+-rw-r--r--   0        0        0     1921 2023-07-08 12:48:12.961773 hyfi-1.1.0/src/hyfi/cached_path/file_lock.py
+-rw-r--r--   0        0        0     3441 2023-07-08 12:48:12.961773 hyfi-1.1.0/src/hyfi/cached_path/meta.py
+-rw-r--r--   0        0        0     3247 2023-07-08 12:48:12.961773 hyfi-1.1.0/src/hyfi/cached_path/progress.py
+-rw-r--r--   0        0        0     1437 2023-07-08 12:48:12.961773 hyfi-1.1.0/src/hyfi/cached_path/schemes/__init__.py
+-rw-r--r--   0        0        0     1815 2023-07-08 12:48:12.961773 hyfi-1.1.0/src/hyfi/cached_path/schemes/beaker.py
+-rw-r--r--   0        0        0     2862 2023-07-08 12:48:12.961773 hyfi-1.1.0/src/hyfi/cached_path/schemes/hf.py
+-rw-r--r--   0        0        0     2942 2023-07-08 12:48:12.961773 hyfi-1.1.0/src/hyfi/cached_path/schemes/http.py
+-rw-r--r--   0        0        0     3645 2023-07-08 12:48:12.961773 hyfi-1.1.0/src/hyfi/cached_path/schemes/scheme_client.py
+-rw-r--r--   0        0        0     1222 2023-07-08 12:48:12.961773 hyfi-1.1.0/src/hyfi/cached_path/testing.py
+-rw-r--r--   0        0        0     4799 2023-07-08 12:48:12.961773 hyfi-1.1.0/src/hyfi/cached_path/util.py
+-rw-r--r--   0        0        0      464 2023-07-08 12:48:12.961773 hyfi-1.1.0/src/hyfi/cached_path/version.py
+-rw-r--r--   0        0        0    32964 2023-07-08 12:48:12.961773 hyfi-1.1.0/src/hyfi/composer/__init__.py
+-rw-r--r--   0        0        0     7426 2023-07-08 12:48:12.961773 hyfi-1.1.0/src/hyfi/composer/extended.py
+-rw-r--r--   0        0        0     1933 2023-07-08 12:48:12.961773 hyfi-1.1.0/src/hyfi/composer/pydantic.py
+-rw-r--r--   0        0        0        0 2023-07-08 12:48:12.961773 hyfi-1.1.0/src/hyfi/conf/__init__.py
+-rw-r--r--   0        0        0      233 2023-07-08 12:48:40.246070 hyfi-1.1.0/src/hyfi/conf/about/__init__.yaml
+-rw-r--r--   0        0        0      553 2023-07-08 12:48:12.961773 hyfi-1.1.0/src/hyfi/conf/batch/__init__.yaml
+-rw-r--r--   0        0        0        0 2023-07-08 12:48:12.961773 hyfi-1.1.0/src/hyfi/conf/cmd/__init__.yaml
+-rw-r--r--   0        0        0       49 2023-07-08 12:48:12.961773 hyfi-1.1.0/src/hyfi/conf/cmd/about.yaml
+-rw-r--r--   0        0        0      155 2023-07-08 12:48:12.961773 hyfi-1.1.0/src/hyfi/conf/cmd/copy_conf.yaml
+-rw-r--r--   0        0        0       83 2023-07-08 12:48:12.961773 hyfi-1.1.0/src/hyfi/conf/cmd/run_task.yaml
+-rw-r--r--   0        0        0       91 2023-07-08 12:48:12.961773 hyfi-1.1.0/src/hyfi/conf/cmd/run_workflow.yaml
+-rw-r--r--   0        0        0      320 2023-07-08 12:48:12.961773 hyfi-1.1.0/src/hyfi/conf/config.yaml
+-rw-r--r--   0        0        0      569 2023-07-08 12:48:12.961773 hyfi-1.1.0/src/hyfi/conf/copier/conf.yaml
+-rw-r--r--   0        0        0      709 2023-07-08 12:48:12.961773 hyfi-1.1.0/src/hyfi/conf/dotenv/__init__.yaml
+-rw-r--r--   0        0        0      319 2023-07-08 12:48:12.961773 hyfi-1.1.0/src/hyfi/conf/hconf.yaml
+-rw-r--r--   0        0        0     1128 2023-07-08 12:48:12.961773 hyfi-1.1.0/src/hyfi/conf/hydra/help/help.yaml
+-rw-r--r--   0        0        0      264 2023-07-08 12:48:12.961773 hyfi-1.1.0/src/hyfi/conf/hydra/job_logging/custom.yaml
+-rw-r--r--   0        0        0      137 2023-07-08 12:48:12.961773 hyfi-1.1.0/src/hyfi/conf/joblib/__init__.yaml
+-rw-r--r--   0        0        0      217 2023-07-08 12:48:12.961773 hyfi-1.1.0/src/hyfi/conf/mode/__debug__.yaml
+-rw-r--r--   0        0        0      921 2023-07-08 12:48:12.961773 hyfi-1.1.0/src/hyfi/conf/mode/__init__.yaml
+-rw-r--r--   0        0        0       61 2023-07-08 12:48:12.961773 hyfi-1.1.0/src/hyfi/conf/module/__init__.yaml
+-rw-r--r--   0        0        0       73 2023-07-08 12:48:12.961773 hyfi-1.1.0/src/hyfi/conf/path/__batch__.yaml
+-rw-r--r--   0        0        0      880 2023-07-08 12:48:12.961773 hyfi-1.1.0/src/hyfi/conf/path/__init__.yaml
+-rw-r--r--   0        0        0      133 2023-07-08 12:48:12.961773 hyfi-1.1.0/src/hyfi/conf/path/__task__.yaml
+-rw-r--r--   0        0        0      291 2023-07-08 12:48:12.961773 hyfi-1.1.0/src/hyfi/conf/path/dirnames/__init__.yaml
+-rw-r--r--   0        0        0       76 2023-07-08 12:48:12.961773 hyfi-1.1.0/src/hyfi/conf/pipe/__dataframe__.yaml
+-rw-r--r--   0        0        0       77 2023-07-08 12:48:12.961773 hyfi-1.1.0/src/hyfi/conf/pipe/__dataframe_external_funcs__.yaml
+-rw-r--r--   0        0        0       79 2023-07-08 12:48:12.961773 hyfi-1.1.0/src/hyfi/conf/pipe/__dataframe_instance_methods__.yaml
+-rw-r--r--   0        0        0       70 2023-07-08 12:48:12.961773 hyfi-1.1.0/src/hyfi/conf/pipe/__general_external_funcs__.yaml
+-rw-r--r--   0        0        0       72 2023-07-08 12:48:12.961773 hyfi-1.1.0/src/hyfi/conf/pipe/__general_instance_methods__.yaml
+-rw-r--r--   0        0        0      128 2023-07-08 12:48:12.961773 hyfi-1.1.0/src/hyfi/conf/pipe/__init__.yaml
+-rw-r--r--   0        0        0      236 2023-07-08 12:48:12.961773 hyfi-1.1.0/src/hyfi/conf/pipe/load_dataframes.yaml
+-rw-r--r--   0        0        0      241 2023-07-08 12:48:12.961773 hyfi-1.1.0/src/hyfi/conf/pipe/save_dataframes.yaml
+-rw-r--r--   0        0        0       90 2023-07-08 12:48:12.961773 hyfi-1.1.0/src/hyfi/conf/pipe/test_preprocessing.yaml
+-rw-r--r--   0        0        0       69 2023-07-08 12:48:12.961773 hyfi-1.1.0/src/hyfi/conf/pipeline/__init__.yaml
+-rw-r--r--   0        0        0      388 2023-07-08 12:48:12.961773 hyfi-1.1.0/src/hyfi/conf/pipeline/__test_dataframe__.yaml
+-rw-r--r--   0        0        0      268 2023-07-08 12:48:12.961773 hyfi-1.1.0/src/hyfi/conf/pipeline/__test_general__.yaml
+-rw-r--r--   0        0        0      744 2023-07-08 12:48:12.961773 hyfi-1.1.0/src/hyfi/conf/project/__init__.yaml
+-rw-r--r--   0        0        0      170 2023-07-08 12:48:12.961773 hyfi-1.1.0/src/hyfi/conf/project/__test__.yaml
+-rw-r--r--   0        0        0       38 2023-07-08 12:48:12.961773 hyfi-1.1.0/src/hyfi/conf/running/__init__.yaml
+-rw-r--r--   0        0        0      161 2023-07-08 12:48:12.961773 hyfi-1.1.0/src/hyfi/conf/task/__batch__.yaml
+-rw-r--r--   0        0        0      359 2023-07-08 12:48:12.961773 hyfi-1.1.0/src/hyfi/conf/task/__init__.yaml
+-rw-r--r--   0        0        0      378 2023-07-08 12:48:12.961773 hyfi-1.1.0/src/hyfi/conf/task/__test__.yaml
+-rw-r--r--   0        0        0       99 2023-07-08 12:48:12.961773 hyfi-1.1.0/src/hyfi/conf/workflow/__init__.yaml
+-rw-r--r--   0        0        0       99 2023-07-08 12:48:12.961773 hyfi-1.1.0/src/hyfi/conf/workflow/__test__.yaml
+-rw-r--r--   0        0        0     6548 2023-07-08 12:48:12.961773 hyfi-1.1.0/src/hyfi/copier/__init__.py
+-rw-r--r--   0        0        0     5915 2023-07-08 12:48:12.961773 hyfi-1.1.0/src/hyfi/dotenv/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-08 12:48:12.961773 hyfi-1.1.0/src/hyfi/graphics/__init__.py
+-rw-r--r--   0        0        0     8470 2023-07-08 12:48:12.961773 hyfi-1.1.0/src/hyfi/graphics/collage.py
+-rw-r--r--   0        0        0     4538 2023-07-08 12:48:12.961773 hyfi-1.1.0/src/hyfi/graphics/motion.py
+-rw-r--r--   0        0        0     7020 2023-07-08 12:48:12.961773 hyfi-1.1.0/src/hyfi/graphics/utils.py
+-rw-r--r--   0        0        0     4228 2023-07-08 12:48:12.961773 hyfi-1.1.0/src/hyfi/joblib/__init__.py
+-rw-r--r--   0        0        0      111 2023-07-08 12:48:12.961773 hyfi-1.1.0/src/hyfi/joblib/batch/__init__.py
+-rw-r--r--   0        0        0     6312 2023-07-08 12:48:12.961773 hyfi-1.1.0/src/hyfi/joblib/batch/apply.py
+-rw-r--r--   0        0        0     4779 2023-07-08 12:48:12.961773 hyfi-1.1.0/src/hyfi/joblib/batch/apply_batch.py
+-rw-r--r--   0        0        0    13823 2023-07-08 12:48:12.961773 hyfi-1.1.0/src/hyfi/joblib/batch/batcher.py
+-rw-r--r--   0        0        0    50273 2023-07-08 12:48:12.961773 hyfi-1.1.0/src/hyfi/main/__init__.py
+-rw-r--r--   0        0        0      280 2023-07-08 12:48:12.961773 hyfi-1.1.0/src/hyfi/module/__init__.py
+-rw-r--r--   0        0        0     4915 2023-07-08 12:48:12.965773 hyfi-1.1.0/src/hyfi/path/__init__.py
+-rw-r--r--   0        0        0     4183 2023-07-08 12:48:12.965773 hyfi-1.1.0/src/hyfi/path/base.py
+-rw-r--r--   0        0        0      782 2023-07-08 12:48:12.965773 hyfi-1.1.0/src/hyfi/path/batch.py
+-rw-r--r--   0        0        0      599 2023-07-08 12:48:12.965773 hyfi-1.1.0/src/hyfi/path/dirnames.py
+-rw-r--r--   0        0        0     1609 2023-07-08 12:48:12.965773 hyfi-1.1.0/src/hyfi/path/task.py
+-rw-r--r--   0        0        0     5030 2023-07-08 12:48:12.965773 hyfi-1.1.0/src/hyfi/pipe/__init__.py
+-rw-r--r--   0        0        0     1455 2023-07-08 12:48:12.965773 hyfi-1.1.0/src/hyfi/pipe/test.py
+-rw-r--r--   0        0        0     8085 2023-07-08 12:48:12.965773 hyfi-1.1.0/src/hyfi/pipeline/__init__.py
+-rw-r--r--   0        0        0     2900 2023-07-08 12:48:12.965773 hyfi-1.1.0/src/hyfi/pipeline/configs.py
+-rw-r--r--   0        0        0     5618 2023-07-08 12:48:12.965773 hyfi-1.1.0/src/hyfi/project/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-08 12:48:12.965773 hyfi-1.1.0/src/hyfi/py.typed
+-rw-r--r--   0        0        0     4268 2023-07-08 12:48:12.965773 hyfi-1.1.0/src/hyfi/task/__init__.py
+-rw-r--r--   0        0        0     7014 2023-07-08 12:48:12.965773 hyfi-1.1.0/src/hyfi/task/batch.py
+-rw-r--r--   0        0        0        0 2023-07-08 12:48:12.965773 hyfi-1.1.0/src/hyfi/utils/__init__.py
+-rw-r--r--   0        0        0     1314 2023-07-08 12:48:12.965773 hyfi-1.1.0/src/hyfi/utils/contexts.py
+-rw-r--r--   0        0        0    30058 2023-07-08 12:48:12.965773 hyfi-1.1.0/src/hyfi/utils/datasets.py
+-rw-r--r--   0        0        0     6568 2023-07-08 12:48:12.965773 hyfi-1.1.0/src/hyfi/utils/envs.py
+-rw-r--r--   0        0        0    10857 2023-07-08 12:48:12.965773 hyfi-1.1.0/src/hyfi/utils/funcs.py
+-rw-r--r--   0        0        0     3769 2023-07-08 12:48:12.965773 hyfi-1.1.0/src/hyfi/utils/gpumon.py
+-rw-r--r--   0        0        0    20157 2023-07-08 12:48:12.965773 hyfi-1.1.0/src/hyfi/utils/iolibs.py
+-rw-r--r--   0        0        0     2259 2023-07-08 12:48:12.965773 hyfi-1.1.0/src/hyfi/utils/logging.py
+-rw-r--r--   0        0        0    12820 2023-07-08 12:48:12.965773 hyfi-1.1.0/src/hyfi/utils/notebooks.py
+-rw-r--r--   0        0        0     6955 2023-07-08 12:48:12.965773 hyfi-1.1.0/src/hyfi/utils/packages.py
+-rw-r--r--   0        0        0      382 2023-07-08 12:48:12.965773 hyfi-1.1.0/src/hyfi/utils/types.py
+-rw-r--r--   0        0        0      753 2023-07-08 12:48:12.965773 hyfi-1.1.0/src/hyfi/workflow/__init__.py
+-rw-r--r--   0        0        0     3393 1970-01-01 00:00:00.000000 hyfi-1.1.0/PKG-INFO
```

### Comparing `hyfi-1.0.5/LICENSE` & `hyfi-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.5/README.md` & `hyfi-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.5/pyproject.toml` & `hyfi-1.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hyfi"
-version = "1.0.5"
+version = "1.1.0"
 description = "Hydra Fast Interface (Hydra and Pydantic based interface framework)"
 authors = ["Young Joon Lee <entelecheia@hotmail.com>"]
 license = "MIT"
 homepage = "https://hyfi.entelecheia.ai"
 repository = "https://github.com/entelecheia/hyfi"
 readme = "README.md"
 packages = [{ include = "hyfi", from = "src" }]
```

### Comparing `hyfi-1.0.5/src/hyfi/__cli__.py` & `hyfi-1.1.0/src/hyfi/__cli__.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,16 +73,17 @@
         cfg: Configuration dictionary to be used for instantiation
 
     Returns:
         None if everything went fine otherwise an error is raised
         to indicate the reason for the failure
     """
     hyfi = HyfiConfig(**cfg)  # type: ignore
+    hyfi.initialize()
     verbose = hyfi.verbose
-    app_name = hyfi.about.name
+    app_name = hyfi.app_name
     print_config = hyfi.print_config
     resolve = hyfi.resolve
 
     # Print out the command line interface for the application.
     if verbose:
         print(f"## Command Line Interface for {app_name} ##")
     HyFI.initialize()
@@ -120,19 +121,14 @@
                         Relative paths are interpreted relative to the declaring python
                         file. Alternatively, you can use the prefix `pkg://` to specify
                         a python package to add to the searchpath.
                         If config_path is None no directory is added to the Config search path.
         config_name: The name of the config (usually the file name without the .yaml extension)
     """
     # Returns the path to the config file.
-    if config_path is None:
-        config_path = __about__.config_path
+    # if config_path is None:
+    config_path = __about__.config_path
     hydra.main(
         config_path=config_path,
         config_name=config_name,
         version_base=__hydra_version_base__,
     )(cli_main)()
-
-
-# Run the command line interface
-if __name__ == "__main__":
-    hydra_main()
```

### Comparing `hyfi-1.0.5/src/hyfi/__click__.py` & `hyfi-1.1.0/src/hyfi/__click__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.5/src/hyfi/__global__/__init__.py` & `hyfi-1.1.0/src/hyfi/__global__/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.5/src/hyfi/__global__/config.py` & `hyfi-1.1.0/src/hyfi/__global__/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,38 +11,25 @@
     FieldValidationInfo,
     PrivateAttr,
     field_validator,
     model_validator,
 )
 
 from hyfi.__global__ import __about__, __hydra_config__
-from hyfi.about import AboutConfig
+from hyfi.about import AboutConfig, __app_name__, __version__
 from hyfi.dotenv import DotEnvConfig
 from hyfi.project import ProjectConfig
 from hyfi.task import TaskConfig
 from hyfi.utils.envs import ENVs
 from hyfi.utils.logging import LOGGING
 from hyfi.utils.notebooks import NBs
 
 logger = LOGGING.getLogger(__name__)
 
 
-def __version__():
-    """
-    Returns the version of Hyfi. It is used to determine the version of Hyfi.
-
-
-    Returns:
-        string containing the version of
-    """
-    from hyfi._version import __version__
-
-    return __version__
-
-
 class HyfiConfig(BaseModel):
     """HyFI root config class.  This class is used to store the configuration"""
 
     hyfi_config_path: str = __about__.config_path
     hyfi_config_module: str = __about__.config_module
     hyfi_user_config_path: str = ""
 
@@ -50,15 +37,15 @@
     print_config: bool = False
     resolve: bool = False
     verbose: bool = False
     logging_level: str = "WARNING"
 
     hydra: Optional[DictConfig] = None
 
-    about: AboutConfig = AboutConfig()
+    about: Optional[AboutConfig] = None
     copier: Optional[DictConfig] = None
     project: Optional[ProjectConfig] = None
     task: Optional[TaskConfig] = None
 
     _version_: str = PrivateAttr(__version__())
     _initilized_: bool = PrivateAttr(False)
 
@@ -95,19 +82,19 @@
 
     @field_validator("hyfi_user_config_path")
     def _validate_hyfi_user_config_path(cls, v):
         """
         Validate and set hyfi_user_config_path.
 
         Args:
-                cls: Class to use for validation.
-                v: Value to set if valid.
+            cls: Class to use for validation.
+            v: Value to set if valid.
 
         Returns:
-                True if valid False otherwise
+            True if valid False otherwise
         """
         return ENVs.check_and_set_osenv_var("hyfi_user_config_path", v)
 
     @field_validator("logging_level")
     def _validate_logging_level(cls, v, info: FieldValidationInfo):
         """
         Validate and set the logging level
@@ -144,25 +131,25 @@
         verbose: Union[bool, int] = False,
         **kwargs,
     ):
         """
         Initialize and start hyfi.
 
         Args:
-                project_name: Name of the project to use.
-                project_description: Description of the project that will be used.
-                project_root: Root directory of the project.
-                project_workspace_name: Name of the project's workspace directory.
-                global_hyfi_root: Root directory of the global hyfi.
-                global_workspace_name: Name of the global hierachical workspace directory.
-                num_workers: Number of workers to run.
-                log_level: Log level for the log.
-                autotime: Whether to automatically set time and / or keep track of run times.
-                retina: Whether to use retina or not.
-                verbose: Enables or disables logging
+            project_name: Name of the project to use.
+            project_description: Description of the project that will be used.
+            project_root: Root directory of the project.
+            project_workspace_name: Name of the project's workspace directory.
+            global_hyfi_root: Root directory of the global hyfi.
+            global_workspace_name: Name of the global hierachical workspace directory.
+            num_workers: Number of workers to run.
+            log_level: Log level for the log.
+            autotime: Whether to automatically set time and / or keep track of run times.
+            retina: Whether to use retina or not.
+            verbose: Enables or disables logging
         """
         envs = DotEnvConfig(HYFI_VERBOSE=verbose)  # type: ignore
         # Set the project name environment variable HYFI_PROJECT_NAME environment variable if project_name is not set.
         if project_name:
             envs.HYFI_PROJECT_NAME = ENVs.expand_posix_vars(project_name)
         # Set the project description environment variable HYFI_PROJECT_DESC environment variable.
         if project_description:
@@ -207,14 +194,16 @@
 
         Returns:
             A boolean indicating whether initialization was successful
         """
         # Returns the current value of the _initilized_ attribute.
         if self._initilized_ and not force:
             return
+        if self.about is None:
+            self.about = AboutConfig()
         __hydra_config__.hyfi_config_module = __about__.config_module
         __hydra_config__.hyfi_config_path = __about__.config_path
         __hydra_config__.hyfi_user_config_path = self.hyfi_user_config_path
         logger.debug(
             "HyFiConfig initialized with hyfi_config_module=%s, hyfi_config_path=%s, hyfi_user_config_path=%s",
             __hydra_config__.hyfi_config_module,
             __hydra_config__.hyfi_config_path,
@@ -239,15 +228,15 @@
         self._initilized_ = False
 
     def __repr__(self):
         """
         Returns a string representation of HyFIConfig.
 
         Returns:
-                The string representation of HyFI
+            The string representation of HyFI
         """
         return f"HyFIConfig(project={self.project})"
 
     def __str__(self):
         """
         Returns a string representation of the object.
 
@@ -259,27 +248,38 @@
     @property
     def app_version(self):
         """
         Get the version of the application.
 
 
         Returns:
-                The version of the application
+            The version of the application
+        """
+        return self.about.version if self.about else __version__()
+
+    @property
+    def app_name(self):
+        """
+        Get the name of the application.
+
+        Returns:
+            The name of the application
         """
-        return self.about.version
+        return self.about.name if self.about else __app_name__
 
     @property
     def dotenv(self):
         return DotEnvConfig()  # type: ignore
 
     @property
     def osenv(self):
         return os.environ
 
 
 __global_config__ = HyfiConfig()
-__global_config__.about.version = __version__()
+if __global_config__.about:
+    __global_config__.about.version = __version__()
 
 
 def __search_package_path__():
     """Global HyFI config path for the package to search for."""
     return __global_config__.hyfi_config_path
```

### Comparing `hyfi-1.0.5/src/hyfi/__init__.py` & `hyfi-1.1.0/src/hyfi/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.5/src/hyfi/about/__init__.py` & `hyfi-1.1.0/src/hyfi/about/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -7,14 +7,36 @@
 """
 from pydantic import BaseModel, ConfigDict
 
 from hyfi.utils.logging import LOGGING
 
 logger = LOGGING.getLogger(__name__)
 
+__package_name__: str = "hyfi"
+__app_name__: str = "HyFI"
+__authors__: str = "Young Joon Lee <entelecheia@hotmail.com>"
+__description__: str = (
+    "Hydra Fast Interface (Hydra and Pydantic based interface framework)"
+)
+__homepage__: str = "https://hyfi.entelecheia.ai"
+__license__: str = "MIT"
+
+
+def __version__() -> str:
+    """
+    Returns the version of Hyfi. It is used to determine the version of Hyfi.
+
+
+    Returns:
+        string containing the version of
+    """
+    from hyfi._version import __version__
+
+    return __version__
+
 
 class AboutConfig(BaseModel):
     """A Pydantic BaseModel that contains metadata about the package.
 
     Attributes:
         __package_name__ (str): The name of the package.
         name (str): The display name of the package.
@@ -23,23 +45,23 @@
         homepage (str): The URL of the package's homepage.
         license (str): The license under which the package is distributed.
         version (str): The version number of the package.
         model_config (ConfigDict): A ConfigDict that allows extra configuration
             options to be added to the AboutConfig instance.
     """
 
-    __package_name__: str = "hyfi"
-    name: str = "HyFI"
-    authors: str = "Young Joon Lee <entelecheia@hotmail.com>"
-    description: str = (
-        "Hydra Fast Interface (Hydra and Pydantic based interface framework)"
-    )
-    homepage: str = "https://hyfi.entelecheia.ai"
-    license: str = "MIT"
-    version: str = "0.0.0"
+    _config_group_: str = "about"
+    __package_name__: str = __package_name__
+
+    name: str = __app_name__
+    authors: str = __authors__
+    description: str = __description__
+    homepage: str = __homepage__
+    license: str = __license__
+    version: str = __version__()
 
     model_config = ConfigDict(extra="allow")  # type: ignore
 
     @property
     def config_module(self) -> str:
         """Returns the name of the configuration module."""
         return f"{self.__package_name__}.conf"
```

### Comparing `hyfi-1.0.5/src/hyfi/batch/__init__.py` & `hyfi-1.1.0/src/hyfi/batch/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.5/src/hyfi/cached_path/__init__.py` & `hyfi-1.1.0/src/hyfi/cached_path/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.5/src/hyfi/cached_path/_cached_path.py` & `hyfi-1.1.0/src/hyfi/cached_path/_cached_path.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.5/src/hyfi/cached_path/cache_file.py` & `hyfi-1.1.0/src/hyfi/cached_path/cache_file.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.5/src/hyfi/cached_path/common.py` & `hyfi-1.1.0/src/hyfi/cached_path/common.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.5/src/hyfi/cached_path/file_lock.py` & `hyfi-1.1.0/src/hyfi/cached_path/file_lock.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.5/src/hyfi/cached_path/meta.py` & `hyfi-1.1.0/src/hyfi/cached_path/meta.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.5/src/hyfi/cached_path/progress.py` & `hyfi-1.1.0/src/hyfi/cached_path/progress.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.5/src/hyfi/cached_path/schemes/__init__.py` & `hyfi-1.1.0/src/hyfi/cached_path/schemes/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.5/src/hyfi/cached_path/schemes/beaker.py` & `hyfi-1.1.0/src/hyfi/cached_path/schemes/beaker.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.5/src/hyfi/cached_path/schemes/hf.py` & `hyfi-1.1.0/src/hyfi/cached_path/schemes/hf.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.5/src/hyfi/cached_path/schemes/http.py` & `hyfi-1.1.0/src/hyfi/cached_path/schemes/http.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.5/src/hyfi/cached_path/schemes/scheme_client.py` & `hyfi-1.1.0/src/hyfi/cached_path/schemes/scheme_client.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.5/src/hyfi/cached_path/testing.py` & `hyfi-1.1.0/src/hyfi/cached_path/testing.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.5/src/hyfi/cached_path/util.py` & `hyfi-1.1.0/src/hyfi/cached_path/util.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.5/src/hyfi/composer/__init__.py` & `hyfi-1.1.0/src/hyfi/composer/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.5/src/hyfi/composer/extended.py` & `hyfi-1.1.0/src/hyfi/composer/extended.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,19 +2,16 @@
 import random
 from typing import Any, Callable, Dict, Union
 
 import hydra
 from omegaconf import OmegaConf
 
 from hyfi.__global__ import __home_path__, __hyfi_path__
-from hyfi.__global__.config import (
-    __global_config__,
-    __search_package_path__,
-    __version__,
-)
+from hyfi.__global__.config import __global_config__, __search_package_path__
+from hyfi.about import __version__
 from hyfi.cached_path import cached_path
 from hyfi.composer import Composer, SpecialKeys
 from hyfi.utils.envs import ENVs
 from hyfi.utils.funcs import FUNCs
 from hyfi.utils.iolibs import IOLIBs
 from hyfi.utils.logging import LOGGING
 from hyfi.utils.packages import PKGs
```

### Comparing `hyfi-1.0.5/src/hyfi/conf/batch/__init__.yaml` & `hyfi-1.1.0/src/hyfi/conf/batch/__init__.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.5/src/hyfi/conf/copier/conf.yaml` & `hyfi-1.1.0/src/hyfi/conf/copier/conf.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.5/src/hyfi/conf/dotenv/__init__.yaml` & `hyfi-1.1.0/src/hyfi/conf/dotenv/__init__.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.5/src/hyfi/conf/hydra/help/help.yaml` & `hyfi-1.1.0/src/hyfi/conf/hydra/help/help.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.5/src/hyfi/conf/mode/__init__.yaml` & `hyfi-1.1.0/src/hyfi/conf/mode/__init__.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.5/src/hyfi/conf/path/__init__.yaml` & `hyfi-1.1.0/src/hyfi/conf/path/__init__.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.5/src/hyfi/conf/project/__init__.yaml` & `hyfi-1.1.0/src/hyfi/conf/project/__init__.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.5/src/hyfi/copier/__init__.py` & `hyfi-1.1.0/src/hyfi/copier/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.5/src/hyfi/dotenv/__init__.py` & `hyfi-1.1.0/src/hyfi/dotenv/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.5/src/hyfi/graphics/collage.py` & `hyfi-1.1.0/src/hyfi/graphics/collage.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.5/src/hyfi/graphics/motion.py` & `hyfi-1.1.0/src/hyfi/graphics/motion.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.5/src/hyfi/graphics/utils.py` & `hyfi-1.1.0/src/hyfi/graphics/utils.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.5/src/hyfi/joblib/__init__.py` & `hyfi-1.1.0/src/hyfi/joblib/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.5/src/hyfi/joblib/batch/apply.py` & `hyfi-1.1.0/src/hyfi/joblib/batch/apply.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.5/src/hyfi/joblib/batch/apply_batch.py` & `hyfi-1.1.0/src/hyfi/joblib/batch/apply_batch.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.5/src/hyfi/joblib/batch/batcher.py` & `hyfi-1.1.0/src/hyfi/joblib/batch/batcher.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.5/src/hyfi/main/__init__.py` & `hyfi-1.1.0/src/hyfi/main/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 )
 
 import pandas as pd
 from omegaconf import DictConfig, ListConfig, SCMode
 
 from hyfi.__global__ import __home_path__, __hyfi_path__
 from hyfi.__global__.config import __global_config__
+from hyfi.about import AboutConfig
 from hyfi.composer import Composer, DictKeyType, SpecialKeys
 from hyfi.composer.extended import XC
 from hyfi.dotenv import DotEnvConfig
 from hyfi.joblib import BATCHER, JobLibConfig
 from hyfi.pipeline import PipelineConfig, PIPELINEs
 from hyfi.pipeline.configs import PipeConfig
 from hyfi.project import ProjectConfig
@@ -41,18 +42,19 @@
 from hyfi.utils.types import PathLikeType
 from hyfi.workflow import WorkflowConfig
 
 logger = LOGGING.getLogger(__name__)
 
 
 def _about(cfg):
-    pkg_name = cfg.about.__package_name__
-    name = cfg.about.name
+    about = AboutConfig() if cfg.about is None else cfg.about
+    pkg_name = about.__package_name__
+    name = about.name
     print()
-    for k, v in cfg.about.model_dump().items():
+    for k, v in about.model_dump().items():
         if k.startswith("_"):
             continue
         print(f"{k:11} : {v}")
     if pkg_name:
         print(f"\nExecute `{pkg_name} --help` to see what you can do with {name}")
```

### Comparing `hyfi-1.0.5/src/hyfi/path/__init__.py` & `hyfi-1.1.0/src/hyfi/path/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.5/src/hyfi/path/base.py` & `hyfi-1.1.0/src/hyfi/path/base.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.5/src/hyfi/path/batch.py` & `hyfi-1.1.0/src/hyfi/path/batch.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.5/src/hyfi/path/dirnames.py` & `hyfi-1.1.0/src/hyfi/path/dirnames.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.5/src/hyfi/path/task.py` & `hyfi-1.1.0/src/hyfi/path/task.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.5/src/hyfi/pipe/__init__.py` & `hyfi-1.1.0/src/hyfi/pipe/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.5/src/hyfi/pipe/test.py` & `hyfi-1.1.0/src/hyfi/pipe/test.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.5/src/hyfi/pipeline/__init__.py` & `hyfi-1.1.0/src/hyfi/pipeline/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.5/src/hyfi/pipeline/configs.py` & `hyfi-1.1.0/src/hyfi/pipeline/configs.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.5/src/hyfi/project/__init__.py` & `hyfi-1.1.0/src/hyfi/project/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.5/src/hyfi/task/__init__.py` & `hyfi-1.1.0/src/hyfi/task/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.5/src/hyfi/task/batch.py` & `hyfi-1.1.0/src/hyfi/task/batch.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.5/src/hyfi/utils/contexts.py` & `hyfi-1.1.0/src/hyfi/utils/contexts.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.5/src/hyfi/utils/datasets.py` & `hyfi-1.1.0/src/hyfi/utils/datasets.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.5/src/hyfi/utils/envs.py` & `hyfi-1.1.0/src/hyfi/utils/envs.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.5/src/hyfi/utils/funcs.py` & `hyfi-1.1.0/src/hyfi/utils/funcs.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.5/src/hyfi/utils/gpumon.py` & `hyfi-1.1.0/src/hyfi/utils/gpumon.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.5/src/hyfi/utils/iolibs.py` & `hyfi-1.1.0/src/hyfi/utils/iolibs.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.5/src/hyfi/utils/logging.py` & `hyfi-1.1.0/src/hyfi/utils/logging.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.5/src/hyfi/utils/notebooks.py` & `hyfi-1.1.0/src/hyfi/utils/notebooks.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.5/src/hyfi/utils/packages.py` & `hyfi-1.1.0/src/hyfi/utils/packages.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.5/src/hyfi/workflow/__init__.py` & `hyfi-1.1.0/src/hyfi/workflow/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.5/PKG-INFO` & `hyfi-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyfi
-Version: 1.0.5
+Version: 1.1.0
 Summary: Hydra Fast Interface (Hydra and Pydantic based interface framework)
 Home-page: https://hyfi.entelecheia.ai
 License: MIT
 Author: Young Joon Lee
 Author-email: entelecheia@hotmail.com
 Requires-Python: >=3.8.1,<3.12
 Classifier: License :: OSI Approved :: MIT License
```

