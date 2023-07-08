# Comparing `tmp/soapcw-0.1.9.tar.gz` & `tmp/soapcw-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "soapcw-0.1.9.tar", last modified: Thu Jul  6 15:47:03 2023, max compression
+gzip compressed data, was "soapcw-0.2.0.tar", last modified: Sat Jul  8 21:02:59 2023, max compression
```

## Comparing `soapcw-0.1.9.tar` & `soapcw-0.2.0.tar`

### file list

```diff
@@ -1,91 +1,96 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 15:47:03.500949 soapcw-0.1.9/
--rw-rw-rw-   0 root         (0) root         (0)      166 2023-07-05 17:01:34.000000 soapcw-0.1.9/AUTHORS.rst
--rw-rw-rw-   0 root         (0) root         (0)     3508 2023-07-05 17:01:34.000000 soapcw-0.1.9/CONTRIBUTING.rst
--rw-rw-rw-   0 root         (0) root         (0)      153 2023-07-05 17:01:34.000000 soapcw-0.1.9/HISTORY.rst
--rw-rw-rw-   0 root         (0) root         (0)     1072 2023-07-05 17:01:34.000000 soapcw-0.1.9/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      361 2023-07-05 17:01:34.000000 soapcw-0.1.9/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2446 2023-07-06 15:47:03.500949 soapcw-0.1.9/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1377 2023-07-06 15:28:59.000000 soapcw-0.1.9/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 15:47:03.487949 soapcw-0.1.9/docs/
--rw-rw-rw-   0 root         (0) root         (0)      605 2023-07-05 17:01:34.000000 soapcw-0.1.9/docs/Makefile
--rw-rw-rw-   0 root         (0) root         (0)       28 2023-07-05 17:01:34.000000 soapcw-0.1.9/docs/authors.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 15:47:03.488949 soapcw-0.1.9/docs/cnn_usage/
--rw-rw-rw-   0 root         (0) root         (0)     5902 2023-07-05 17:01:34.000000 soapcw-0.1.9/docs/cnn_usage/data_generation.rst
--rw-rw-rw-   0 root         (0) root         (0)      243 2023-07-05 17:01:34.000000 soapcw-0.1.9/docs/cnn_usage/index.rst
--rw-rw-rw-   0 root         (0) root         (0)     5625 2023-07-05 17:01:34.000000 soapcw-0.1.9/docs/cnn_usage/train_model.rst
--rwxrwxrwx   0 root         (0) root         (0)     4930 2023-07-05 17:01:34.000000 soapcw-0.1.9/docs/conf.py
--rw-rw-rw-   0 root         (0) root         (0)       33 2023-07-05 17:01:34.000000 soapcw-0.1.9/docs/contributing.rst
--rw-rw-rw-   0 root         (0) root         (0)       28 2023-07-05 17:01:34.000000 soapcw-0.1.9/docs/history.rst
--rw-rw-rw-   0 root         (0) root         (0)     1213 2023-07-05 17:01:34.000000 soapcw-0.1.9/docs/index.rst
--rw-rw-rw-   0 root         (0) root         (0)     1062 2023-07-05 17:01:34.000000 soapcw-0.1.9/docs/installation.rst
--rw-rw-rw-   0 root         (0) root         (0)      766 2023-07-05 17:01:34.000000 soapcw-0.1.9/docs/make.bat
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 15:47:03.488949 soapcw-0.1.9/docs/pipeline_usage/
--rw-rw-rw-   0 root         (0) root         (0)      166 2023-07-05 17:01:34.000000 soapcw-0.1.9/docs/pipeline_usage/index.rst
--rw-rw-rw-   0 root         (0) root         (0)     6633 2023-07-05 17:01:34.000000 soapcw-0.1.9/docs/pipeline_usage/run_pipeline.rst
--rw-rw-rw-   0 root         (0) root         (0)       27 2023-07-05 17:01:34.000000 soapcw-0.1.9/docs/readme.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 15:47:03.488949 soapcw-0.1.9/docs/usage/
--rw-rw-rw-   0 root         (0) root         (0)      280 2023-07-05 17:01:34.000000 soapcw-0.1.9/docs/usage/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 15:47:03.489949 soapcw-0.1.9/pipeline/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-06 15:44:48.000000 soapcw-0.1.9/pipeline/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 15:47:03.489949 soapcw-0.1.9/pipeline/css/
--rw-rw-rw-   0 root         (0) root         (0)     3163 2023-07-05 17:01:34.000000 soapcw-0.1.9/pipeline/css/general.css
--rwxrwxrwx   0 root         (0) root         (0)     7001 2023-07-05 17:01:34.000000 soapcw-0.1.9/pipeline/make_dag_files_astro.py
--rwxrwxrwx   0 root         (0) root         (0)     6963 2023-07-05 17:01:34.000000 soapcw-0.1.9/pipeline/make_dag_files_lines.py
--rw-rw-rw-   0 root         (0) root         (0)    38283 2023-07-05 17:01:34.000000 soapcw-0.1.9/pipeline/make_html_page.py
--rwxrwxrwx   0 root         (0) root         (0)    37058 2023-07-06 15:04:52.000000 soapcw-0.1.9/pipeline/run_full_soap_astro.py
--rwxrwxrwx   0 root         (0) root         (0)    40172 2023-07-05 17:01:34.000000 soapcw-0.1.9/pipeline/run_full_soap_lines.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 15:47:03.489949 soapcw-0.1.9/pipeline/scripts/
--rw-rw-rw-   0 root         (0) root         (0)    18806 2023-07-05 17:01:34.000000 soapcw-0.1.9/pipeline/scripts/table_scripts.js
--rw-rw-rw-   0 root         (0) root         (0)     3367 2023-07-05 17:01:34.000000 soapcw-0.1.9/pipeline/soap_config_parser.py
--rw-rw-rw-   0 root         (0) root         (0)     1004 2023-07-06 15:47:03.501949 soapcw-0.1.9/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     4209 2023-07-05 17:01:34.000000 soapcw-0.1.9/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 15:47:03.492949 soapcw-0.1.9/soapcw/
--rw-rw-rw-   0 root         (0) root         (0)      589 2023-07-06 15:04:52.000000 soapcw-0.1.9/soapcw/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      406 2023-07-05 17:01:34.000000 soapcw-0.1.9/soapcw/cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 15:47:03.494949 soapcw-0.1.9/soapcw/cnn/
--rw-rw-rw-   0 root         (0) root         (0)       26 2023-07-05 17:01:34.000000 soapcw-0.1.9/soapcw/cnn/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4682 2023-07-05 17:01:34.000000 soapcw-0.1.9/soapcw/cnn/cnn_data_dag_gen.py
--rwxrwxrwx   0 root         (0) root         (0)    17948 2023-07-06 15:04:52.000000 soapcw-0.1.9/soapcw/cnn/cnn_data_gen.py
--rw-rw-rw-   0 root         (0) root         (0)    12490 2023-07-05 17:01:34.000000 soapcw-0.1.9/soapcw/cnn/generate_gaussian_train_data.py
--rw-rw-rw-   0 root         (0) root         (0)    11006 2023-07-05 17:01:34.000000 soapcw-0.1.9/soapcw/cnn/generate_test_data.py
--rw-rw-rw-   0 root         (0) root         (0)    20005 2023-07-05 17:01:34.000000 soapcw-0.1.9/soapcw/cnn/generate_train_data.py
--rwxrwxrwx   0 root         (0) root         (0)     5822 2023-07-05 17:01:34.000000 soapcw-0.1.9/soapcw/cnn/narrowband_sfts.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 15:47:03.495949 soapcw-0.1.9/soapcw/cnn/pytorch/
--rw-rw-rw-   0 root         (0) root         (0)       68 2023-07-05 17:01:34.000000 soapcw-0.1.9/soapcw/cnn/pytorch/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4307 2023-07-05 17:01:34.000000 soapcw-0.1.9/soapcw/cnn/pytorch/load_models.py
--rw-rw-rw-   0 root         (0) root         (0)    15950 2023-07-05 17:01:34.000000 soapcw-0.1.9/soapcw/cnn/pytorch/models.py
--rw-rw-rw-   0 root         (0) root         (0)    14625 2023-07-06 15:04:52.000000 soapcw-0.1.9/soapcw/cnn/train_model.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 15:47:03.497949 soapcw-0.1.9/soapcw/cw/
--rw-rw-rw-   0 root         (0) root         (0)      197 2023-07-05 17:01:34.000000 soapcw-0.1.9/soapcw/cw/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    43688 2023-07-06 14:43:01.000000 soapcw-0.1.9/soapcw/cw/generate_data.py
--rw-rw-rw-   0 root         (0) root         (0)    19576 2023-07-05 17:01:34.000000 soapcw-0.1.9/soapcw/cw/load_sfts.py
--rw-rw-rw-   0 root         (0) root         (0)     8660 2023-07-05 17:01:34.000000 soapcw-0.1.9/soapcw/cw/make_sfts.py
--rw-rw-rw-   0 root         (0) root         (0)     9450 2023-07-05 17:01:34.000000 soapcw-0.1.9/soapcw/cw/sft.py
--rw-rw-rw-   0 root         (0) root         (0)     8567 2023-07-05 17:01:34.000000 soapcw-0.1.9/soapcw/cw/timeseries.py
--rw-rw-rw-   0 root         (0) root         (0)     1687 2023-07-05 17:01:34.000000 soapcw-0.1.9/soapcw/cw/tools.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 15:47:03.498949 soapcw-0.1.9/soapcw/line_aware_stat/
--rw-rw-rw-   0 root         (0) root         (0)      123 2023-07-05 17:01:34.000000 soapcw-0.1.9/soapcw/line_aware_stat/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11721 2023-07-05 17:01:34.000000 soapcw-0.1.9/soapcw/line_aware_stat/gen_lookup.pyx
--rw-rw-rw-   0 root         (0) root         (0)    38004 2023-07-05 17:01:34.000000 soapcw-0.1.9/soapcw/line_aware_stat/gen_lookup_python.py
--rwxrwxrwx   0 root         (0) root         (0)     6514 2023-07-05 17:01:34.000000 soapcw-0.1.9/soapcw/line_aware_stat/save_lookup.py
--rw-rw-rw-   0 root         (0) root         (0)     4237 2023-07-05 17:01:34.000000 soapcw-0.1.9/soapcw/soap_config_parser.py
--rw-r--r--   0 root         (0) root         (0)  2271838 2023-07-06 15:47:02.000000 soapcw-0.1.9/soapcw/soapcw.c
--rw-rw-rw-   0 root         (0) root         (0)    65928 2023-07-05 17:01:34.000000 soapcw-0.1.9/soapcw/soapcw.pyx
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 15:47:03.498949 soapcw-0.1.9/soapcw/tools/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-06 15:44:48.000000 soapcw-0.1.9/soapcw/tools/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2885 2023-07-05 17:01:34.000000 soapcw-0.1.9/soapcw/tools/plots.py
--rw-rw-rw-   0 root         (0) root         (0)     9044 2023-07-05 17:01:34.000000 soapcw-0.1.9/soapcw/tools/tools.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 15:47:03.493949 soapcw-0.1.9/soapcw.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2446 2023-07-06 15:47:03.000000 soapcw-0.1.9/soapcw.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1829 2023-07-06 15:47:03.000000 soapcw-0.1.9/soapcw.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-06 15:47:03.000000 soapcw-0.1.9/soapcw.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      484 2023-07-06 15:47:03.000000 soapcw-0.1.9/soapcw.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-06 15:47:03.000000 soapcw-0.1.9/soapcw.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       65 2023-07-06 15:47:03.000000 soapcw-0.1.9/soapcw.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-06 15:47:03.000000 soapcw-0.1.9/soapcw.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 15:47:03.499949 soapcw-0.1.9/tests/
--rw-rw-rw-   0 root         (0) root         (0)   445283 2023-07-05 17:01:34.000000 soapcw-0.1.9/tests/SNR_injections.ipynb
--rw-rw-rw-   0 root         (0) root         (0)       59 2023-07-05 17:01:34.000000 soapcw-0.1.9/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1130 2023-07-05 17:01:34.000000 soapcw-0.1.9/tests/test_cwload.py
--rw-rw-rw-   0 root         (0) root         (0)     3602 2023-07-05 17:01:34.000000 soapcw-0.1.9/tests/test_line_aware_stat.py
--rw-rw-rw-   0 root         (0) root         (0)     4290 2023-07-05 17:01:34.000000 soapcw-0.1.9/tests/test_soap.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-08 21:02:59.685006 soapcw-0.2.0/
+-rw-rw-rw-   0 root         (0) root         (0)      166 2023-07-08 21:01:19.000000 soapcw-0.2.0/AUTHORS.rst
+-rw-rw-rw-   0 root         (0) root         (0)     3508 2023-07-08 21:01:19.000000 soapcw-0.2.0/CONTRIBUTING.rst
+-rw-rw-rw-   0 root         (0) root         (0)      153 2023-07-08 21:01:19.000000 soapcw-0.2.0/HISTORY.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1072 2023-07-08 21:01:19.000000 soapcw-0.2.0/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      361 2023-07-08 21:01:19.000000 soapcw-0.2.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2446 2023-07-08 21:02:59.685006 soapcw-0.2.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1377 2023-07-08 21:01:19.000000 soapcw-0.2.0/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-08 21:02:59.677006 soapcw-0.2.0/docs/
+-rw-rw-rw-   0 root         (0) root         (0)      605 2023-07-08 21:01:19.000000 soapcw-0.2.0/docs/Makefile
+-rw-rw-rw-   0 root         (0) root         (0)       28 2023-07-08 21:01:19.000000 soapcw-0.2.0/docs/authors.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-08 21:02:59.677006 soapcw-0.2.0/docs/cnn_usage/
+-rw-rw-rw-   0 root         (0) root         (0)     5902 2023-07-08 21:01:19.000000 soapcw-0.2.0/docs/cnn_usage/data_generation.rst
+-rw-rw-rw-   0 root         (0) root         (0)      243 2023-07-08 21:01:19.000000 soapcw-0.2.0/docs/cnn_usage/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     5625 2023-07-08 21:01:19.000000 soapcw-0.2.0/docs/cnn_usage/train_model.rst
+-rwxrwxrwx   0 root         (0) root         (0)     4930 2023-07-08 21:01:19.000000 soapcw-0.2.0/docs/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)       33 2023-07-08 21:01:19.000000 soapcw-0.2.0/docs/contributing.rst
+-rw-rw-rw-   0 root         (0) root         (0)       28 2023-07-08 21:01:19.000000 soapcw-0.2.0/docs/history.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1213 2023-07-08 21:01:19.000000 soapcw-0.2.0/docs/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1062 2023-07-08 21:01:19.000000 soapcw-0.2.0/docs/installation.rst
+-rw-rw-rw-   0 root         (0) root         (0)      766 2023-07-08 21:01:19.000000 soapcw-0.2.0/docs/make.bat
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-08 21:02:59.677006 soapcw-0.2.0/docs/pipeline_usage/
+-rw-rw-rw-   0 root         (0) root         (0)      166 2023-07-08 21:01:19.000000 soapcw-0.2.0/docs/pipeline_usage/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     6633 2023-07-08 21:01:19.000000 soapcw-0.2.0/docs/pipeline_usage/run_pipeline.rst
+-rw-rw-rw-   0 root         (0) root         (0)       27 2023-07-08 21:01:19.000000 soapcw-0.2.0/docs/readme.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-08 21:02:59.677006 soapcw-0.2.0/docs/usage/
+-rw-rw-rw-   0 root         (0) root         (0)      280 2023-07-08 21:01:19.000000 soapcw-0.2.0/docs/usage/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-08 21:02:59.678006 soapcw-0.2.0/pipeline/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-08 21:01:19.000000 soapcw-0.2.0/pipeline/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-08 21:02:59.678006 soapcw-0.2.0/pipeline/css/
+-rw-rw-rw-   0 root         (0) root         (0)     3163 2023-07-08 21:01:19.000000 soapcw-0.2.0/pipeline/css/general.css
+-rwxrwxrwx   0 root         (0) root         (0)     7001 2023-07-08 21:01:19.000000 soapcw-0.2.0/pipeline/make_dag_files_astro.py
+-rwxrwxrwx   0 root         (0) root         (0)     6963 2023-07-08 21:01:19.000000 soapcw-0.2.0/pipeline/make_dag_files_lines.py
+-rw-rw-rw-   0 root         (0) root         (0)    38283 2023-07-08 21:01:19.000000 soapcw-0.2.0/pipeline/make_html_page.py
+-rwxrwxrwx   0 root         (0) root         (0)    37058 2023-07-08 21:01:19.000000 soapcw-0.2.0/pipeline/run_full_soap_astro.py
+-rwxrwxrwx   0 root         (0) root         (0)    40172 2023-07-08 21:01:19.000000 soapcw-0.2.0/pipeline/run_full_soap_lines.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-08 21:02:59.678006 soapcw-0.2.0/pipeline/scripts/
+-rw-rw-rw-   0 root         (0) root         (0)    18806 2023-07-08 21:01:19.000000 soapcw-0.2.0/pipeline/scripts/table_scripts.js
+-rw-rw-rw-   0 root         (0) root         (0)     3367 2023-07-08 21:01:19.000000 soapcw-0.2.0/pipeline/soap_config_parser.py
+-rw-rw-rw-   0 root         (0) root         (0)     1004 2023-07-08 21:02:59.686006 soapcw-0.2.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     4209 2023-07-08 21:01:19.000000 soapcw-0.2.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-08 21:02:59.681006 soapcw-0.2.0/soapcw/
+-rw-rw-rw-   0 root         (0) root         (0)      619 2023-07-08 21:01:19.000000 soapcw-0.2.0/soapcw/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      406 2023-07-08 21:01:19.000000 soapcw-0.2.0/soapcw/cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-08 21:02:59.682006 soapcw-0.2.0/soapcw/cnn/
+-rw-rw-rw-   0 root         (0) root         (0)       26 2023-07-08 21:01:19.000000 soapcw-0.2.0/soapcw/cnn/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4682 2023-07-08 21:01:19.000000 soapcw-0.2.0/soapcw/cnn/cnn_data_dag_gen.py
+-rwxrwxrwx   0 root         (0) root         (0)    17948 2023-07-08 21:01:19.000000 soapcw-0.2.0/soapcw/cnn/cnn_data_gen.py
+-rw-rw-rw-   0 root         (0) root         (0)    12490 2023-07-08 21:01:19.000000 soapcw-0.2.0/soapcw/cnn/generate_gaussian_train_data.py
+-rw-rw-rw-   0 root         (0) root         (0)    11006 2023-07-08 21:01:19.000000 soapcw-0.2.0/soapcw/cnn/generate_test_data.py
+-rw-rw-rw-   0 root         (0) root         (0)    20005 2023-07-08 21:01:19.000000 soapcw-0.2.0/soapcw/cnn/generate_train_data.py
+-rwxrwxrwx   0 root         (0) root         (0)     5822 2023-07-08 21:01:19.000000 soapcw-0.2.0/soapcw/cnn/narrowband_sfts.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-08 21:02:59.682006 soapcw-0.2.0/soapcw/cnn/pytorch/
+-rw-rw-rw-   0 root         (0) root         (0)       68 2023-07-08 21:01:19.000000 soapcw-0.2.0/soapcw/cnn/pytorch/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4307 2023-07-08 21:01:19.000000 soapcw-0.2.0/soapcw/cnn/pytorch/load_models.py
+-rw-rw-rw-   0 root         (0) root         (0)    15950 2023-07-08 21:01:19.000000 soapcw-0.2.0/soapcw/cnn/pytorch/models.py
+-rw-rw-rw-   0 root         (0) root         (0)    14625 2023-07-08 21:01:19.000000 soapcw-0.2.0/soapcw/cnn/train_model.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-08 21:02:59.683006 soapcw-0.2.0/soapcw/cw/
+-rw-rw-rw-   0 root         (0) root         (0)      197 2023-07-08 21:01:19.000000 soapcw-0.2.0/soapcw/cw/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    43688 2023-07-08 21:01:19.000000 soapcw-0.2.0/soapcw/cw/generate_data.py
+-rw-rw-rw-   0 root         (0) root         (0)    19576 2023-07-08 21:01:19.000000 soapcw-0.2.0/soapcw/cw/load_sfts.py
+-rw-rw-rw-   0 root         (0) root         (0)     8660 2023-07-08 21:01:19.000000 soapcw-0.2.0/soapcw/cw/make_sfts.py
+-rw-rw-rw-   0 root         (0) root         (0)     9450 2023-07-08 21:01:19.000000 soapcw-0.2.0/soapcw/cw/sft.py
+-rw-rw-rw-   0 root         (0) root         (0)     8567 2023-07-08 21:01:19.000000 soapcw-0.2.0/soapcw/cw/timeseries.py
+-rw-rw-rw-   0 root         (0) root         (0)     1687 2023-07-08 21:01:19.000000 soapcw-0.2.0/soapcw/cw/tools.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-08 21:02:59.683006 soapcw-0.2.0/soapcw/line_aware_stat/
+-rw-rw-rw-   0 root         (0) root         (0)      123 2023-07-08 21:01:19.000000 soapcw-0.2.0/soapcw/line_aware_stat/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11721 2023-07-08 21:01:19.000000 soapcw-0.2.0/soapcw/line_aware_stat/gen_lookup.pyx
+-rw-rw-rw-   0 root         (0) root         (0)    38004 2023-07-08 21:01:19.000000 soapcw-0.2.0/soapcw/line_aware_stat/gen_lookup_python.py
+-rwxrwxrwx   0 root         (0) root         (0)     6514 2023-07-08 21:01:19.000000 soapcw-0.2.0/soapcw/line_aware_stat/save_lookup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-08 21:02:59.684006 soapcw-0.2.0/soapcw/neville/
+-rw-rw-rw-   0 root         (0) root         (0)       85 2023-07-08 21:01:19.000000 soapcw-0.2.0/soapcw/neville/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1898 2023-07-08 21:01:19.000000 soapcw-0.2.0/soapcw/neville/load_models.py
+-rw-rw-rw-   0 root         (0) root         (0)    23724 2023-07-08 21:01:19.000000 soapcw-0.2.0/soapcw/neville/models.py
+-rw-rw-rw-   0 root         (0) root         (0)     4753 2023-07-08 21:01:19.000000 soapcw-0.2.0/soapcw/neville/truncated_gauss.py
+-rw-rw-rw-   0 root         (0) root         (0)     4331 2023-07-08 21:01:19.000000 soapcw-0.2.0/soapcw/soap_config_parser.py
+-rw-r--r--   0 root         (0) root         (0)  2271838 2023-07-08 21:02:59.000000 soapcw-0.2.0/soapcw/soapcw.c
+-rw-rw-rw-   0 root         (0) root         (0)    65928 2023-07-08 21:01:19.000000 soapcw-0.2.0/soapcw/soapcw.pyx
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-08 21:02:59.684006 soapcw-0.2.0/soapcw/tools/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-08 21:01:19.000000 soapcw-0.2.0/soapcw/tools/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2885 2023-07-08 21:01:19.000000 soapcw-0.2.0/soapcw/tools/plots.py
+-rw-rw-rw-   0 root         (0) root         (0)     9044 2023-07-08 21:01:19.000000 soapcw-0.2.0/soapcw/tools/tools.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-08 21:02:59.681006 soapcw-0.2.0/soapcw.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2446 2023-07-08 21:02:59.000000 soapcw-0.2.0/soapcw.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1945 2023-07-08 21:02:59.000000 soapcw-0.2.0/soapcw.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-08 21:02:59.000000 soapcw-0.2.0/soapcw.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      484 2023-07-08 21:02:59.000000 soapcw-0.2.0/soapcw.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-08 21:02:59.000000 soapcw-0.2.0/soapcw.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       65 2023-07-08 21:02:59.000000 soapcw-0.2.0/soapcw.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-08 21:02:59.000000 soapcw-0.2.0/soapcw.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-08 21:02:59.685006 soapcw-0.2.0/tests/
+-rw-rw-rw-   0 root         (0) root         (0)   445283 2023-07-08 21:01:19.000000 soapcw-0.2.0/tests/SNR_injections.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)       59 2023-07-08 21:01:19.000000 soapcw-0.2.0/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1130 2023-07-08 21:01:19.000000 soapcw-0.2.0/tests/test_cwload.py
+-rw-rw-rw-   0 root         (0) root         (0)     3602 2023-07-08 21:01:19.000000 soapcw-0.2.0/tests/test_line_aware_stat.py
+-rw-rw-rw-   0 root         (0) root         (0)     4290 2023-07-08 21:01:19.000000 soapcw-0.2.0/tests/test_soap.py
```

### Comparing `soapcw-0.1.9/CONTRIBUTING.rst` & `soapcw-0.2.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `soapcw-0.1.9/LICENSE` & `soapcw-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `soapcw-0.1.9/PKG-INFO` & `soapcw-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: soapcw
-Version: 0.1.9
+Version: 0.2.0
 Summary: SOAP is a rapid algorithm to search for continuous sources of gravitational waves, with a wider application to long duration narrowband signals.
 Home-page: https://git.ligo.org/joseph.bayley/soapcw
 Author: Joe Bayley
 Author-email: joseph.bayley@glasgow.ac.uk
 License: MIT license
 Download-URL: https://git.ligo.org/joseph.bayley/soapcw/-/archive/0.1.2/soapcw-0.1.2.tar.gz
 Keywords: soapcw,soap,gravitational waves,pulsars,neutron stars,continuous waves
```

### Comparing `soapcw-0.1.9/README.rst` & `soapcw-0.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `soapcw-0.1.9/docs/Makefile` & `soapcw-0.2.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `soapcw-0.1.9/docs/cnn_usage/data_generation.rst` & `soapcw-0.2.0/docs/cnn_usage/data_generation.rst`

 * *Files identical despite different names*

### Comparing `soapcw-0.1.9/docs/cnn_usage/train_model.rst` & `soapcw-0.2.0/docs/cnn_usage/train_model.rst`

 * *Files identical despite different names*

### Comparing `soapcw-0.1.9/docs/conf.py` & `soapcw-0.2.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `soapcw-0.1.9/docs/index.rst` & `soapcw-0.2.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `soapcw-0.1.9/docs/installation.rst` & `soapcw-0.2.0/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `soapcw-0.1.9/docs/make.bat` & `soapcw-0.2.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `soapcw-0.1.9/docs/pipeline_usage/run_pipeline.rst` & `soapcw-0.2.0/docs/pipeline_usage/run_pipeline.rst`

 * *Files identical despite different names*

### Comparing `soapcw-0.1.9/pipeline/css/general.css` & `soapcw-0.2.0/pipeline/css/general.css`

 * *Files identical despite different names*

### Comparing `soapcw-0.1.9/pipeline/make_dag_files_astro.py` & `soapcw-0.2.0/pipeline/make_dag_files_astro.py`

 * *Files identical despite different names*

### Comparing `soapcw-0.1.9/pipeline/make_dag_files_lines.py` & `soapcw-0.2.0/pipeline/make_dag_files_lines.py`

 * *Files identical despite different names*

### Comparing `soapcw-0.1.9/pipeline/make_html_page.py` & `soapcw-0.2.0/pipeline/make_html_page.py`

 * *Files identical despite different names*

### Comparing `soapcw-0.1.9/pipeline/run_full_soap_astro.py` & `soapcw-0.2.0/pipeline/run_full_soap_astro.py`

 * *Files identical despite different names*

### Comparing `soapcw-0.1.9/pipeline/run_full_soap_lines.py` & `soapcw-0.2.0/pipeline/run_full_soap_lines.py`

 * *Files identical despite different names*

### Comparing `soapcw-0.1.9/pipeline/scripts/table_scripts.js` & `soapcw-0.2.0/pipeline/scripts/table_scripts.js`

 * *Files identical despite different names*

### Comparing `soapcw-0.1.9/pipeline/soap_config_parser.py` & `soapcw-0.2.0/pipeline/soap_config_parser.py`

 * *Files identical despite different names*

### Comparing `soapcw-0.1.9/setup.cfg` & `soapcw-0.2.0/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [bumpversion]
-current_version = 0.1.8
-new_version = 0.1.9
+current_version = 0.1.9
+new_version = 0.2.0
 commit = True
 tag = True
 
 [bumpversion:file:setup.py]
 search = version='{current_version}'
 replace = version='{new_version}'
 
@@ -18,15 +18,15 @@
 [flake8]
 exclude = docs
 
 [aliases]
 
 [metadata]
 name = soapcw
-version = 0.1.9
+version = 0.2.0
 
 [options]
 packages = soapcw, pipeline
 
 [options.entry_points]
 console_scripts = 
 	soapcw-make-dag-files-lines = pipeline.make_dag_files_lines:main
```

### Comparing `soapcw-0.1.9/setup.py` & `soapcw-0.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `soapcw-0.1.9/soapcw/__init__.py` & `soapcw-0.2.0/soapcw/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 __author__ = """Joe Bayley"""
 __email__ = 'joseph.bayley@glasgow.ac.uk'
 __version__ = '0.1.9'
 from .soapcw import single_detector, two_detector, three_detector, single_detector_gaps
 from .tools import tools, plots
 from .cnn import __init__
+from .neville import __init__
 from .line_aware_stat import __init__
 from .cw import __init__
 from . import soap_config_parser
 
 #try:
 #    from .lookup_table import gen_lookup_python, save_lookup, gen_lookup
 #except:
```

### Comparing `soapcw-0.1.9/soapcw/cnn/cnn_data_dag_gen.py` & `soapcw-0.2.0/soapcw/cnn/cnn_data_dag_gen.py`

 * *Files identical despite different names*

### Comparing `soapcw-0.1.9/soapcw/cnn/cnn_data_gen.py` & `soapcw-0.2.0/soapcw/cnn/cnn_data_gen.py`

 * *Files identical despite different names*

### Comparing `soapcw-0.1.9/soapcw/cnn/generate_gaussian_train_data.py` & `soapcw-0.2.0/soapcw/cnn/generate_gaussian_train_data.py`

 * *Files identical despite different names*

### Comparing `soapcw-0.1.9/soapcw/cnn/generate_test_data.py` & `soapcw-0.2.0/soapcw/cnn/generate_test_data.py`

 * *Files identical despite different names*

### Comparing `soapcw-0.1.9/soapcw/cnn/generate_train_data.py` & `soapcw-0.2.0/soapcw/cnn/generate_train_data.py`

 * *Files identical despite different names*

### Comparing `soapcw-0.1.9/soapcw/cnn/narrowband_sfts.py` & `soapcw-0.2.0/soapcw/cnn/narrowband_sfts.py`

 * *Files identical despite different names*

### Comparing `soapcw-0.1.9/soapcw/cnn/pytorch/load_models.py` & `soapcw-0.2.0/soapcw/cnn/pytorch/load_models.py`

 * *Files identical despite different names*

### Comparing `soapcw-0.1.9/soapcw/cnn/pytorch/models.py` & `soapcw-0.2.0/soapcw/cnn/pytorch/models.py`

 * *Files identical despite different names*

### Comparing `soapcw-0.1.9/soapcw/cnn/train_model.py` & `soapcw-0.2.0/soapcw/cnn/train_model.py`

 * *Files identical despite different names*

### Comparing `soapcw-0.1.9/soapcw/cw/generate_data.py` & `soapcw-0.2.0/soapcw/cw/generate_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,19 +43,19 @@
             path to earth ephemeris file
         sun_ephem: string
             path to sun ephemeris file
         snr: float
             SNR of signal, overwrites the h0 parameter
         """
         if earth_ephem is None:
-            self.earth_ephem = "earth00-19-DE405.dat.gz"
+            self.earth_ephem = "earth00-40-DE430.dat.gz"
         else:
             self.earth_ephem = earth_ephem
         if sun_ephem is None:
-            self.sun_ephem = "sun00-19-DE405.dat.gz"
+            self.sun_ephem = "sun00-40-DE430.dat.gz"
         else:
             self.sun_ephem = sun_ephem
         
         self.alpha = alpha
         self.delta = delta
         self.psi   = psi
         self.phi0  = phi0
```

### Comparing `soapcw-0.1.9/soapcw/cw/load_sfts.py` & `soapcw-0.2.0/soapcw/cw/load_sfts.py`

 * *Files identical despite different names*

### Comparing `soapcw-0.1.9/soapcw/cw/make_sfts.py` & `soapcw-0.2.0/soapcw/cw/make_sfts.py`

 * *Files identical despite different names*

### Comparing `soapcw-0.1.9/soapcw/cw/sft.py` & `soapcw-0.2.0/soapcw/cw/sft.py`

 * *Files identical despite different names*

### Comparing `soapcw-0.1.9/soapcw/cw/timeseries.py` & `soapcw-0.2.0/soapcw/cw/timeseries.py`

 * *Files identical despite different names*

### Comparing `soapcw-0.1.9/soapcw/cw/tools.py` & `soapcw-0.2.0/soapcw/cw/tools.py`

 * *Files identical despite different names*

### Comparing `soapcw-0.1.9/soapcw/line_aware_stat/gen_lookup.pyx` & `soapcw-0.2.0/soapcw/line_aware_stat/gen_lookup.pyx`

 * *Files identical despite different names*

### Comparing `soapcw-0.1.9/soapcw/line_aware_stat/gen_lookup_python.py` & `soapcw-0.2.0/soapcw/line_aware_stat/gen_lookup_python.py`

 * *Files identical despite different names*

### Comparing `soapcw-0.1.9/soapcw/line_aware_stat/save_lookup.py` & `soapcw-0.2.0/soapcw/line_aware_stat/save_lookup.py`

 * *Files identical despite different names*

### Comparing `soapcw-0.1.9/soapcw/soap_config_parser.py` & `soapcw-0.2.0/soapcw/soap_config_parser.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,21 +16,21 @@
         self.config_file = os.path.abspath(config_file)
         self.float_list = ["band_starts","band_ends","band_widths"]
         self.int_list = ["strides","fc_layers","img_dim", "avg_pool_size"]
         self.string_list = ["load_directory","save_options","type","band_types","sft_dirs"]
         self.tuple_list = ["conv_layers"]
         self.floats = ["band_load_size", "snr_width_line", "snr_width_signal", 
                         "prob_line", "left_right_prob", "det1_prob", "det2_prob",
-                        "snrmin","snrmax","learning_rate","data_load_size","tstart"]
+                        "snrmin","snrmax","learning_rate","data_load_size","tstart","dropout"]
         self.ints = ["memory", "request_disk", "n_jobs", "n_channels","nperband",
                      "n_summed_sfts","n_epochs","save_interval","nsfts", "tstart", "tend",
-                     "n_train_multi_size"]
+                     "n_train_multi_size","fdim","input_dim","par_dim","num_predict_params","latent_dim","stride"]
         self.bools = ["resize_image", "overwrite_files", "gen_noise_only"]
         self.strings = ["save_dir", "narrowband_sft_dir", "accounting_group", "root_dir", 
-                        "run", "type", "lookup_dir", "model_type","search_exec"]
+                        "run", "type", "lookup_dir", "model_type","search_exec","dist_type"]
 
 
         self.config = self.parse_config(cfg)
 
     def __getitem__(self, key):
         return self.config[key]
```

### Comparing `soapcw-0.1.9/soapcw/soapcw.c` & `soapcw-0.2.0/soapcw/soapcw.c`

 * *Files identical despite different names*

### Comparing `soapcw-0.1.9/soapcw/soapcw.pyx` & `soapcw-0.2.0/soapcw/soapcw.pyx`

 * *Files identical despite different names*

### Comparing `soapcw-0.1.9/soapcw/tools/plots.py` & `soapcw-0.2.0/soapcw/tools/plots.py`

 * *Files identical despite different names*

### Comparing `soapcw-0.1.9/soapcw/tools/tools.py` & `soapcw-0.2.0/soapcw/tools/tools.py`

 * *Files identical despite different names*

### Comparing `soapcw-0.1.9/soapcw.egg-info/PKG-INFO` & `soapcw-0.2.0/soapcw.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: soapcw
-Version: 0.1.9
+Version: 0.2.0
 Summary: SOAP is a rapid algorithm to search for continuous sources of gravitational waves, with a wider application to long duration narrowband signals.
 Home-page: https://git.ligo.org/joseph.bayley/soapcw
 Author: Joe Bayley
 Author-email: joseph.bayley@glasgow.ac.uk
 License: MIT license
 Download-URL: https://git.ligo.org/joseph.bayley/soapcw/-/archive/0.1.2/soapcw-0.1.2.tar.gz
 Keywords: soapcw,soap,gravitational waves,pulsars,neutron stars,continuous waves
```

### Comparing `soapcw-0.1.9/soapcw.egg-info/SOURCES.txt` & `soapcw-0.2.0/soapcw.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -60,14 +60,18 @@
 soapcw/cw/sft.py
 soapcw/cw/timeseries.py
 soapcw/cw/tools.py
 soapcw/line_aware_stat/__init__.py
 soapcw/line_aware_stat/gen_lookup.pyx
 soapcw/line_aware_stat/gen_lookup_python.py
 soapcw/line_aware_stat/save_lookup.py
+soapcw/neville/__init__.py
+soapcw/neville/load_models.py
+soapcw/neville/models.py
+soapcw/neville/truncated_gauss.py
 soapcw/tools/__init__.py
 soapcw/tools/plots.py
 soapcw/tools/tools.py
 tests/SNR_injections.ipynb
 tests/__init__.py
 tests/test_cwload.py
 tests/test_line_aware_stat.py
```

### Comparing `soapcw-0.1.9/tests/SNR_injections.ipynb` & `soapcw-0.2.0/tests/SNR_injections.ipynb`

 * *Files identical despite different names*

### Comparing `soapcw-0.1.9/tests/test_cwload.py` & `soapcw-0.2.0/tests/test_cwload.py`

 * *Files identical despite different names*

### Comparing `soapcw-0.1.9/tests/test_line_aware_stat.py` & `soapcw-0.2.0/tests/test_line_aware_stat.py`

 * *Files identical despite different names*

### Comparing `soapcw-0.1.9/tests/test_soap.py` & `soapcw-0.2.0/tests/test_soap.py`

 * *Files identical despite different names*

