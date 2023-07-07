# Comparing `tmp/fusion-engine-client-1.20.0rc3.tar.gz` & `tmp/fusion-engine-client-1.20.0rc4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fusion-engine-client-1.20.0rc3.tar", last modified: Fri Jun 23 03:46:41 2023, max compression
+gzip compressed data, was "fusion-engine-client-1.20.0rc4.tar", last modified: Fri Jul  7 23:25:15 2023, max compression
```

## Comparing `fusion-engine-client-1.20.0rc3.tar` & `fusion-engine-client-1.20.0rc4.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 03:46:41.055105 fusion-engine-client-1.20.0rc3/
--rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-06-23 03:46:41.055105 fusion-engine-client-1.20.0rc3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12660 2023-06-23 03:45:50.000000 fusion-engine-client-1.20.0rc3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 03:46:41.043105 fusion-engine-client-1.20.0rc3/bin/
--rwxr-xr-x   0 runner    (1001) docker     (123)      472 2023-06-23 03:45:50.000000 fusion-engine-client-1.20.0rc3/bin/p1_display
--rwxr-xr-x   0 runner    (1001) docker     (123)     4679 2023-06-23 03:45:50.000000 fusion-engine-client-1.20.0rc3/bin/p1_extract
--rwxr-xr-x   0 runner    (1001) docker     (123)    13937 2023-06-23 03:45:50.000000 fusion-engine-client-1.20.0rc3/bin/p1_print
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 03:46:41.043105 fusion-engine-client-1.20.0rc3/fusion_engine_client/
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-23 03:45:50.000000 fusion-engine-client-1.20.0rc3/fusion_engine_client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 03:46:41.047104 fusion-engine-client-1.20.0rc3/fusion_engine_client/analysis/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 03:45:50.000000 fusion-engine-client-1.20.0rc3/fusion_engine_client/analysis/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)   113032 2023-06-23 03:45:50.000000 fusion-engine-client-1.20.0rc3/fusion_engine_client/analysis/analyzer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-06-23 03:45:50.000000 fusion-engine-client-1.20.0rc3/fusion_engine_client/analysis/attitude.py
--rw-r--r--   0 runner    (1001) docker     (123)    41758 2023-06-23 03:45:50.000000 fusion-engine-client-1.20.0rc3/fusion_engine_client/analysis/data_loader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 03:46:41.051104 fusion-engine-client-1.20.0rc3/fusion_engine_client/messages/
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-06-23 03:45:50.000000 fusion-engine-client-1.20.0rc3/fusion_engine_client/messages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    56695 2023-06-23 03:45:50.000000 fusion-engine-client-1.20.0rc3/fusion_engine_client/messages/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)    24157 2023-06-23 03:45:50.000000 fusion-engine-client-1.20.0rc3/fusion_engine_client/messages/control.py
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-06-23 03:45:50.000000 fusion-engine-client-1.20.0rc3/fusion_engine_client/messages/core.py
--rw-r--r--   0 runner    (1001) docker     (123)    26227 2023-06-23 03:45:50.000000 fusion-engine-client-1.20.0rc3/fusion_engine_client/messages/defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-06-23 03:45:50.000000 fusion-engine-client-1.20.0rc3/fusion_engine_client/messages/device.py
--rw-r--r--   0 runner    (1001) docker     (123)     6166 2023-06-23 03:45:50.000000 fusion-engine-client-1.20.0rc3/fusion_engine_client/messages/fault_control.py
--rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-06-23 03:45:50.000000 fusion-engine-client-1.20.0rc3/fusion_engine_client/messages/gnss_corrections.py
--rw-r--r--   0 runner    (1001) docker     (123)     5287 2023-06-23 03:45:50.000000 fusion-engine-client-1.20.0rc3/fusion_engine_client/messages/measurement_details.py
--rw-r--r--   0 runner    (1001) docker     (123)    39947 2023-06-23 03:45:50.000000 fusion-engine-client-1.20.0rc3/fusion_engine_client/messages/measurements.py
--rw-r--r--   0 runner    (1001) docker     (123)    15258 2023-06-23 03:45:50.000000 fusion-engine-client-1.20.0rc3/fusion_engine_client/messages/ros.py
--rw-r--r--   0 runner    (1001) docker     (123)    12050 2023-06-23 03:45:50.000000 fusion-engine-client-1.20.0rc3/fusion_engine_client/messages/signal_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    35636 2023-06-23 03:45:50.000000 fusion-engine-client-1.20.0rc3/fusion_engine_client/messages/solution.py
--rw-r--r--   0 runner    (1001) docker     (123)     6433 2023-06-23 03:45:50.000000 fusion-engine-client-1.20.0rc3/fusion_engine_client/messages/timestamp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 03:46:41.051104 fusion-engine-client-1.20.0rc3/fusion_engine_client/parsers/
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-06-23 03:45:50.000000 fusion-engine-client-1.20.0rc3/fusion_engine_client/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15944 2023-06-23 03:45:50.000000 fusion-engine-client-1.20.0rc3/fusion_engine_client/parsers/decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-06-23 03:45:50.000000 fusion-engine-client-1.20.0rc3/fusion_engine_client/parsers/encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)    22997 2023-06-23 03:45:50.000000 fusion-engine-client-1.20.0rc3/fusion_engine_client/parsers/file_index.py
--rw-r--r--   0 runner    (1001) docker     (123)    31146 2023-06-23 03:45:50.000000 fusion-engine-client-1.20.0rc3/fusion_engine_client/parsers/mixed_log_reader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 03:46:41.051104 fusion-engine-client-1.20.0rc3/fusion_engine_client/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 03:45:50.000000 fusion-engine-client-1.20.0rc3/fusion_engine_client/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16397 2023-06-23 03:45:50.000000 fusion-engine-client-1.20.0rc3/fusion_engine_client/utils/argument_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-06-23 03:45:50.000000 fusion-engine-client-1.20.0rc3/fusion_engine_client/utils/bin_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9043 2023-06-23 03:45:50.000000 fusion-engine-client-1.20.0rc3/fusion_engine_client/utils/construct_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3341 2023-06-23 03:45:50.000000 fusion-engine-client-1.20.0rc3/fusion_engine_client/utils/enum_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    24860 2023-06-23 03:45:50.000000 fusion-engine-client-1.20.0rc3/fusion_engine_client/utils/log.py
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-06-23 03:45:50.000000 fusion-engine-client-1.20.0rc3/fusion_engine_client/utils/numpy_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    16857 2023-06-23 03:45:50.000000 fusion-engine-client-1.20.0rc3/fusion_engine_client/utils/time_range.py
--rw-r--r--   0 runner    (1001) docker     (123)     7803 2023-06-23 03:45:50.000000 fusion-engine-client-1.20.0rc3/fusion_engine_client/utils/trace.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 03:46:41.047104 fusion-engine-client-1.20.0rc3/fusion_engine_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-06-23 03:46:41.000000 fusion-engine-client-1.20.0rc3/fusion_engine_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-06-23 03:46:41.000000 fusion-engine-client-1.20.0rc3/fusion_engine_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 03:46:41.000000 fusion-engine-client-1.20.0rc3/fusion_engine_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-06-23 03:46:41.000000 fusion-engine-client-1.20.0rc3/fusion_engine_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-23 03:46:41.000000 fusion-engine-client-1.20.0rc3/fusion_engine_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 03:46:41.055105 fusion-engine-client-1.20.0rc3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2855 2023-06-23 03:45:50.000000 fusion-engine-client-1.20.0rc3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 03:46:41.055105 fusion-engine-client-1.20.0rc3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    10899 2023-06-23 03:45:50.000000 fusion-engine-client-1.20.0rc3/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3339 2023-06-23 03:45:50.000000 fusion-engine-client-1.20.0rc3/tests/test_construct_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    20962 2023-06-23 03:45:50.000000 fusion-engine-client-1.20.0rc3/tests/test_data_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     6129 2023-06-23 03:45:50.000000 fusion-engine-client-1.20.0rc3/tests/test_decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2869 2023-06-23 03:45:50.000000 fusion-engine-client-1.20.0rc3/tests/test_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-06-23 03:45:50.000000 fusion-engine-client-1.20.0rc3/tests/test_enum_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9665 2023-06-23 03:45:50.000000 fusion-engine-client-1.20.0rc3/tests/test_file_index.py
--rw-r--r--   0 runner    (1001) docker     (123)     4820 2023-06-23 03:45:50.000000 fusion-engine-client-1.20.0rc3/tests/test_message_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    17239 2023-06-23 03:45:50.000000 fusion-engine-client-1.20.0rc3/tests/test_mixed_log_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)    13200 2023-06-23 03:45:50.000000 fusion-engine-client-1.20.0rc3/tests/test_time_range.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 23:25:15.148193 fusion-engine-client-1.20.0rc4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-07-07 23:25:15.148193 fusion-engine-client-1.20.0rc4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12660 2023-07-07 23:24:37.000000 fusion-engine-client-1.20.0rc4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 23:25:15.144193 fusion-engine-client-1.20.0rc4/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      472 2023-07-07 23:24:37.000000 fusion-engine-client-1.20.0rc4/bin/p1_display
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4679 2023-07-07 23:24:37.000000 fusion-engine-client-1.20.0rc4/bin/p1_extract
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13937 2023-07-07 23:24:37.000000 fusion-engine-client-1.20.0rc4/bin/p1_print
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 23:25:15.144193 fusion-engine-client-1.20.0rc4/fusion_engine_client/
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-07 23:24:37.000000 fusion-engine-client-1.20.0rc4/fusion_engine_client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 23:25:15.144193 fusion-engine-client-1.20.0rc4/fusion_engine_client/analysis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 23:24:37.000000 fusion-engine-client-1.20.0rc4/fusion_engine_client/analysis/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)   114646 2023-07-07 23:24:37.000000 fusion-engine-client-1.20.0rc4/fusion_engine_client/analysis/analyzer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-07-07 23:24:37.000000 fusion-engine-client-1.20.0rc4/fusion_engine_client/analysis/attitude.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41758 2023-07-07 23:24:37.000000 fusion-engine-client-1.20.0rc4/fusion_engine_client/analysis/data_loader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 23:25:15.144193 fusion-engine-client-1.20.0rc4/fusion_engine_client/messages/
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-07-07 23:24:37.000000 fusion-engine-client-1.20.0rc4/fusion_engine_client/messages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56721 2023-07-07 23:24:37.000000 fusion-engine-client-1.20.0rc4/fusion_engine_client/messages/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24157 2023-07-07 23:24:37.000000 fusion-engine-client-1.20.0rc4/fusion_engine_client/messages/control.py
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-07-07 23:24:37.000000 fusion-engine-client-1.20.0rc4/fusion_engine_client/messages/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26203 2023-07-07 23:24:37.000000 fusion-engine-client-1.20.0rc4/fusion_engine_client/messages/defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-07-07 23:24:37.000000 fusion-engine-client-1.20.0rc4/fusion_engine_client/messages/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6166 2023-07-07 23:24:37.000000 fusion-engine-client-1.20.0rc4/fusion_engine_client/messages/fault_control.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-07-07 23:24:37.000000 fusion-engine-client-1.20.0rc4/fusion_engine_client/messages/gnss_corrections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5287 2023-07-07 23:24:37.000000 fusion-engine-client-1.20.0rc4/fusion_engine_client/messages/measurement_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39947 2023-07-07 23:24:37.000000 fusion-engine-client-1.20.0rc4/fusion_engine_client/messages/measurements.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15258 2023-07-07 23:24:37.000000 fusion-engine-client-1.20.0rc4/fusion_engine_client/messages/ros.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12050 2023-07-07 23:24:37.000000 fusion-engine-client-1.20.0rc4/fusion_engine_client/messages/signal_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35596 2023-07-07 23:24:37.000000 fusion-engine-client-1.20.0rc4/fusion_engine_client/messages/solution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6433 2023-07-07 23:24:37.000000 fusion-engine-client-1.20.0rc4/fusion_engine_client/messages/timestamp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 23:25:15.144193 fusion-engine-client-1.20.0rc4/fusion_engine_client/parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-07-07 23:24:37.000000 fusion-engine-client-1.20.0rc4/fusion_engine_client/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15944 2023-07-07 23:24:37.000000 fusion-engine-client-1.20.0rc4/fusion_engine_client/parsers/decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-07-07 23:24:37.000000 fusion-engine-client-1.20.0rc4/fusion_engine_client/parsers/encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22963 2023-07-07 23:24:37.000000 fusion-engine-client-1.20.0rc4/fusion_engine_client/parsers/file_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31146 2023-07-07 23:24:37.000000 fusion-engine-client-1.20.0rc4/fusion_engine_client/parsers/mixed_log_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 23:25:15.148193 fusion-engine-client-1.20.0rc4/fusion_engine_client/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 23:24:37.000000 fusion-engine-client-1.20.0rc4/fusion_engine_client/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16397 2023-07-07 23:24:37.000000 fusion-engine-client-1.20.0rc4/fusion_engine_client/utils/argument_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-07-07 23:24:37.000000 fusion-engine-client-1.20.0rc4/fusion_engine_client/utils/bin_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9043 2023-07-07 23:24:37.000000 fusion-engine-client-1.20.0rc4/fusion_engine_client/utils/construct_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3341 2023-07-07 23:24:37.000000 fusion-engine-client-1.20.0rc4/fusion_engine_client/utils/enum_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24860 2023-07-07 23:24:37.000000 fusion-engine-client-1.20.0rc4/fusion_engine_client/utils/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-07-07 23:24:37.000000 fusion-engine-client-1.20.0rc4/fusion_engine_client/utils/numpy_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16827 2023-07-07 23:24:37.000000 fusion-engine-client-1.20.0rc4/fusion_engine_client/utils/time_range.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7803 2023-07-07 23:24:37.000000 fusion-engine-client-1.20.0rc4/fusion_engine_client/utils/trace.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 23:25:15.144193 fusion-engine-client-1.20.0rc4/fusion_engine_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-07-07 23:25:15.000000 fusion-engine-client-1.20.0rc4/fusion_engine_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-07-07 23:25:15.000000 fusion-engine-client-1.20.0rc4/fusion_engine_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 23:25:15.000000 fusion-engine-client-1.20.0rc4/fusion_engine_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-07-07 23:25:15.000000 fusion-engine-client-1.20.0rc4/fusion_engine_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-07 23:25:15.000000 fusion-engine-client-1.20.0rc4/fusion_engine_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 23:25:15.148193 fusion-engine-client-1.20.0rc4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2954 2023-07-07 23:24:37.000000 fusion-engine-client-1.20.0rc4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 23:25:15.148193 fusion-engine-client-1.20.0rc4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    10899 2023-07-07 23:24:37.000000 fusion-engine-client-1.20.0rc4/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3339 2023-07-07 23:24:37.000000 fusion-engine-client-1.20.0rc4/tests/test_construct_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20962 2023-07-07 23:24:37.000000 fusion-engine-client-1.20.0rc4/tests/test_data_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6129 2023-07-07 23:24:37.000000 fusion-engine-client-1.20.0rc4/tests/test_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2869 2023-07-07 23:24:37.000000 fusion-engine-client-1.20.0rc4/tests/test_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-07-07 23:24:37.000000 fusion-engine-client-1.20.0rc4/tests/test_enum_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9665 2023-07-07 23:24:37.000000 fusion-engine-client-1.20.0rc4/tests/test_file_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4820 2023-07-07 23:24:37.000000 fusion-engine-client-1.20.0rc4/tests/test_message_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17239 2023-07-07 23:24:37.000000 fusion-engine-client-1.20.0rc4/tests/test_mixed_log_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13200 2023-07-07 23:24:37.000000 fusion-engine-client-1.20.0rc4/tests/test_time_range.py
```

### Comparing `fusion-engine-client-1.20.0rc3/PKG-INFO` & `fusion-engine-client-1.20.0rc4/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fusion-engine-client
-Version: 1.20.0rc3
+Version: 1.20.0rc4
 Summary: Point One FusionEngine Library
 Home-page: https://github.com/PointOneNav/fusion-engine-client
 Author: Point One Navigation
 Author-email: support@pointonenav.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -12,21 +12,23 @@
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >3.7
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: all
 Provides-Extra: dev
 Provides-Extra: display
 Provides-Extra: tools
 
 Point One FusionEngine protocol support for real-time interaction and control, plus post-processing data analysis tools.
```

### Comparing `fusion-engine-client-1.20.0rc3/README.md` & `fusion-engine-client-1.20.0rc4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 * [Requirements](#requirements)
 * [Directory Structure](#directory-structure)
 * [Usage Instructions](#usage-instructions)
 * [Examples](#examples)
 * [Using A Python Virtual Environment](#using-a-python-virtual-environment)
 
 ### Requirements
-- Python 3.8 or later
+- Python 3.6 or later
 
 ### Directory Structure
   - `python/` - Python source files
     - `bin/` - Analysis and processing tools
       - [p1_display](bin/p1_display) - Generate HTML plots of vehicle trajectory, etc. (see also
         `analyzer.py` below)
       - [p1_extract](bin/p1_extract) - Extract FusionEngine message contents from a binary file containing mixed data
@@ -70,29 +70,29 @@
           connected device
       - `utils` - Various utility functions used by the other files (e.g., log search support)
     
 ### Usage Instructions
 
 #### Install From PyPI
 
-1. Install Python 3.8 (or later) and pip.
+1. Install Python (3.6 or later) and pip.
 2. Install the `fusione-engine-client` module, including all analysis and data processing tools:
    ```bash
    python3 -m pip install fusion-engine-client[all]
    ```
    - Note: If you wish to only install data parsing support, and do not want to install plotting and other requirements
      used by the analysis tools in `bin/`, you may omit `[all]` and run `python3 -m pip install fusion-engine-client`
 3. Run any of the applications in `bin/`. For example, to plot results from a `*.p1log` file from a Point One device:
    ```bash
    p1_display /path/to/log/file_or_directory
    ```
 
 #### Install From Source (Use In Another Python Project)
 
-1. Install Python 3.8 (or later) and pip.
+1. Install Python (3.6 or later) and pip.
 2. Clone a copy of this repository:
    ```bash
    git clone https://github.com/PointOneNav/fusion-engine-client.git
    ```
 3. Install the `fusione-engine-client` module, including all analysis and data processing tools:
    ```bash
    python3 -m pip install -e /path/to/fusion-engine-client[all]
@@ -103,15 +103,15 @@
 4. Run any of the applications in `bin/`. For example, to plot results from a `*.p1log` file from a Point One device:
    ```bash
    p1_display /path/to/log/file_or_directory
    ```
 
 #### Install From Source (Development)
 
-1. Install Python 3.8 (or later) and pip.
+1. Install Python (3.6 or later) and pip.
 2. Clone a copy of this repository:
    ```bash
    git clone https://github.com/PointOneNav/fusion-engine-client.git
    ```
 3. Install the Python requirements:
    ```bash
    python3 -m pip install -r requirements.txt
```

### Comparing `fusion-engine-client-1.20.0rc3/bin/p1_extract` & `fusion-engine-client-1.20.0rc4/bin/p1_extract`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.20.0rc3/bin/p1_print` & `fusion-engine-client-1.20.0rc4/bin/p1_print`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.20.0rc3/fusion_engine_client/analysis/analyzer.py` & `fusion-engine-client-1.20.0rc4/fusion_engine_client/analysis/analyzer.py`

 * *Files 1% similar despite different names*

```diff
@@ -103,27 +103,31 @@
     LONG_LOG_DURATION_SEC = 2 * 3600.0
     HIGH_MEASUREMENT_RATE_HZ = 40.0
 
     def __init__(self,
                  file: Union[DataLoader, str], ignore_index: bool = False,
                  output_dir: str = None, prefix: str = '',
                  time_range: TimeRange = None, max_messages: int = None,
+                 time_axis: str = 'relative',
                  truncate_long_logs: bool = True):
         """!
         @brief Create an analyzer for the specified log.
 
         @param file A @ref DataLoader instance, or the path to a file to be loaded.
         @param ignore_index If `True`, do not use the `.p1i` index file if present, and instead regenerate it from the
                `.p1log` data file.
         @param output_dir The directory where output will be stored.
         @param prefix An optional prefix to be appended to the generated filenames.
         @param time_range An optional @ref TimeRange object specifying desired start and end time bounds of the data to
                be read. See @ref TimeRange for more details.
         @param max_messages If set, read up to the specified maximum number of messages. Applies across all message
                types.
+        @param time_axis Specify the way in which time will be plotted:
+               - `absolute`, `abs` - Absolute P1 or system timestamps
+               - `relative`, `rel` - Elapsed time since the start of the log
         @param truncate_long_logs If `True`, reduce or skip certain plots if the log extremely long (as defined by
                @ref LONG_LOG_DURATION_SEC).
         """
         if isinstance(file, str):
             self.reader = DataLoader(file, ignore_index=ignore_index)
         else:
             self.reader = file
@@ -134,21 +138,34 @@
         self.params = {
             'time_range': time_range,
             'max_messages': max_messages,
             'show_progress': True,
             'return_numpy': True
         }
 
-        self.t0 = self.reader.t0
-        if self.t0 is None:
-            self.t0 = Timestamp()
-
-        self.system_t0 = self.reader.get_system_t0()
-        if self.system_t0 is None:
-            self.system_t0 = np.nan
+        if time_axis in ('relative', 'rel'):
+            self.time_axis = 'relative'
+            self.t0 = self.reader.t0
+            if self.t0 is None:
+                self.t0 = Timestamp()
+
+            self.system_t0 = self.reader.get_system_t0()
+            if self.system_t0 is None:
+                self.system_t0 = np.nan
+
+            self.p1_time_label = 'Relative Time (sec)'
+            self.system_time_label = 'Relative Time (sec)'
+        elif time_axis in ('absolute', 'abs'):
+            self.time_axis = 'absolute'
+            self.t0 = Timestamp(0.0)
+            self.system_t0 = 0.0
+            self.p1_time_label = 'P1 Time (sec)'
+            self.system_time_label = 'System Time (sec)'
+        else:
+            raise ValueError(f"Unsupported time axis specifier '{time_axis}'.")
 
         self.plots = {}
         self.summary = ''
 
         self._mapbox_token_missing = False
 
         if self.output_dir is not None:
@@ -177,21 +194,23 @@
                                 (processing_duration_sec / 3600.0, self.LONG_LOG_DURATION_SEC / 3600.0))
 
     def plot_time_scale(self):
         if self.output_dir is None:
             return
 
         # Setup the figure.
+        time_axis_str = 'Relative Time' if self.time_axis == 'relative' else 'P1/System Time'
+        p1_time_axis_str = 'Relative Time' if self.time_axis == 'relative' else 'P1 Time'
         figure = make_subplots(rows=2, cols=1, print_grid=False, shared_xaxes=True,
-                               subplot_titles=['Device Time vs. Relative Time',
-                                               'Pose Message Interval vs. Relative Time'])
+                               subplot_titles=[f'Device Time vs. {time_axis_str}',
+                                               f'Pose Message Interval vs. {p1_time_axis_str}'])
 
         figure['layout'].update(showlegend=True, modebar_add=['v1hovermode'])
-        for i in range(2):
-            figure['layout']['xaxis%d' % (i + 1)].update(title="Relative Time (sec)", showticklabels=True)
+        figure['layout']['xaxis1'].update(title=f"{time_axis_str} (sec)", showticklabels=True)
+        figure['layout']['xaxis2'].update(title=f"{p1_time_axis_str} (sec)", showticklabels=True)
         figure['layout']['yaxis1'].update(title="Absolute Time",
                                           ticktext=['P1/GPS Time', 'System Time'],
                                           tickvals=[1, 2])
         figure['layout']['yaxis2'].update(title="Interval (sec)", rangemode="tozero")
 
         # Read the pose data to get P1 and GPS timestamps.
         result = self.reader.read(message_types=[PoseMessage], **self.params)
@@ -299,15 +318,15 @@
         # Setup the figure.
         figure = make_subplots(rows=2, cols=3, print_grid=False, shared_xaxes=True,
                                subplot_titles=['Attitude (YPR)', 'ENU Displacement', 'Body Velocity',
                                                'Attitude Std', 'ENU Position Std', 'Velocity Std'])
 
         figure['layout'].update(showlegend=True, modebar_add=['v1hovermode'])
         for i in range(6):
-            figure['layout']['xaxis%d' % (i + 1)].update(title="Time (sec)", showticklabels=True, matches='x')
+            figure['layout']['xaxis%d' % (i + 1)].update(title=self.p1_time_label, showticklabels=True, matches='x')
         figure['layout']['yaxis1'].update(title="Degrees")
         figure['layout']['yaxis2'].update(title="Meters")
         figure['layout']['yaxis3'].update(title="Meters/Second")
         figure['layout']['yaxis4'].update(title="Degrees")
         figure['layout']['yaxis5'].update(title="Meters")
         figure['layout']['yaxis6'].update(title="Meters/Second")
 
@@ -406,15 +425,15 @@
         figure = make_subplots(rows=4, cols=1, print_grid=False, shared_xaxes=True,
                                subplot_titles=['<- Percent Complete // Stage ->', 'Mounting Angles',
                                                'Mounting Angle Standard Deviation', 'Travel Distance'],
                                specs=[[{"secondary_y": True}], [{}], [{}], [{}]])
 
         figure['layout'].update(showlegend=True, modebar_add=['v1hovermode'])
         for i in range(4):
-            figure['layout']['xaxis%d' % (i + 1)].update(title="Time (sec)", showticklabels=True)
+            figure['layout']['xaxis%d' % (i + 1)].update(title=self.p1_time_label, showticklabels=True)
         figure['layout']['yaxis1'].update(title="Percent Complete", range=[0, 100])
         figure['layout']['yaxis2'].update(ticktext=['%s' % e.name for e in CalibrationStage],
                                           tickvals=list(range(len(stage_map))))
         figure['layout']['yaxis3'].update(title="Degrees")
         figure['layout']['yaxis4'].update(title="Degrees")
         figure['layout']['yaxis5'].update(title="Meters")
 
@@ -496,15 +515,15 @@
         if len(pose_data.p1_time) == 0:
             self.logger.info('No pose data available. Skipping solution type plot.')
             return
 
         # Setup the figure.
         figure = make_subplots(rows=1, cols=1, print_grid=False, shared_xaxes=True, subplot_titles=['Solution Type'])
 
-        figure['layout']['xaxis'].update(title="Time (sec)")
+        figure['layout']['xaxis'].update(title=self.p1_time_label)
         figure['layout']['yaxis1'].update(title="Solution Type",
                                           ticktext=['%s (%d)' % (e.name, e.value) for e in SolutionType],
                                           tickvals=[e.value for e in SolutionType])
 
         time = pose_data.p1_time - float(self.t0)
 
         text = ["Time: %.3f sec (%.3f sec)" % (t, t + float(self.t0)) for t in time]
@@ -526,15 +545,15 @@
         topo_figure['layout']['xaxis1'].update(title="East (m)")
         topo_figure['layout']['yaxis1'].update(title="North (m)")
 
         time_figure = make_subplots(rows=4, cols=1, print_grid=False, shared_xaxes=True,
                                     subplot_titles=['3D', 'East', 'North', 'Up'])
         time_figure['layout'].update(showlegend=True, modebar_add=['v1hovermode'])
         for i in range(4):
-            time_figure['layout']['xaxis%d' % (i + 1)].update(title="Time (sec)", showticklabels=True)
+            time_figure['layout']['xaxis%d' % (i + 1)].update(title=self.p1_time_label, showticklabels=True)
         time_figure['layout']['yaxis1'].update(title="Displacement (m)")
         time_figure['layout']['yaxis2'].update(title="Displacement (m)")
         time_figure['layout']['yaxis3'].update(title="Displacement (m)")
         time_figure['layout']['yaxis4'].update(title="Displacement (m)")
 
         # Remove invalid solutions.
         valid_idx = np.logical_and(~np.isnan(time), solution_type != SolutionType.Invalid)
@@ -864,15 +883,15 @@
 
         # Setup the figure.
         figure = make_subplots(
             rows=1, cols=1,  print_grid=False, shared_xaxes=True,
             subplot_titles=['C/N0 (L1 Only)'])
 
         figure['layout'].update(showlegend=True, modebar_add=['v1hovermode'])
-        figure['layout']['xaxis1'].update(title="Time (sec)", showticklabels=True)
+        figure['layout']['xaxis1'].update(title=self.p1_time_label, showticklabels=True)
         figure['layout']['yaxis1'].update(title="C/N0 (dB-Hz)")
 
         # Assign colors to each satellite.
         data_by_sv = GNSSSatelliteMessage.group_by_sv(data)
         svs = sorted(list(data_by_sv.keys()))
         color_by_sv = self._assign_colors(svs)
 
@@ -960,15 +979,15 @@
                             'Satellite Count'],
             specs=[[{'rowspan': 4}],
                    [None],
                    [None],
                    [None],
                    [{}]])
         figure['layout'].update(showlegend=False, modebar_add=['v1hovermode'])
-        figure['layout']['xaxis1'].update(title="Time (sec)")
+        figure['layout']['xaxis1'].update(title=self.p1_time_label)
         figure['layout']['yaxis1'].update(title=entry_type)
         figure['layout']['yaxis2'].update(title=f"# {entry_type}s", rangemode='tozero')
 
         # Plot the signal counts.
         time = data.p1_time - float(self.t0)
         text = ["P1: %.3f sec" % (t + float(self.t0)) for t in time]
         figure.add_trace(go.Scattergl(x=time, y=data.num_svs, text=text,
@@ -1058,15 +1077,15 @@
             subplot_titles=['Distance To Station', 'Corrections Age'],
             specs=[[{'rowspan': 3}],
                    [None],
                    [None],
                    [{}]])
         figure['layout'].update(showlegend=True, modebar_add=['v1hovermode'])
         for i in range(2):
-            figure['layout']['xaxis%d' % (i + 1)].update(title="Time (sec)", showticklabels=True, matches='x')
+            figure['layout']['xaxis%d' % (i + 1)].update(title=self.p1_time_label, showticklabels=True, matches='x')
         figure['layout']['yaxis1'].update(title="Baseline Distance (km)")
         figure['layout']['yaxis2'].update(title="Age (sec)")
 
         # Find all base stations present in the data and assign a color to each.
         station_ids = np.unique([s for s in data.reference_station_id
                                  if s != GNSSInfoMessage.INVALID_REFERENCE_STATION])
         if len(station_ids) == 0:
@@ -1216,16 +1235,15 @@
            titles[0] += f'{vehicle_measurement_type.__name__}'
         if raw_vehicle_data is not None and vehicle_measurement_type != raw_vehicle_measurement_type:
             titles[0] += f', {raw_vehicle_measurement_type.__name__}'
 
         figure = make_subplots(rows=len(titles), cols=1, print_grid=False, shared_xaxes=True, subplot_titles=titles)
 
         figure['layout'].update(showlegend=True, modebar_add=['v1hovermode'])
-        for i in range(len(titles)):
-            figure['layout']['xaxis%d' % (i + 1)].update(title="Time (sec)", showticklabels=True)
+        # Note: X-axis title set below after determining time source.
 
         if type == 'tick':
             figure['layout']['yaxis1'].update(title="Tick Count")
             figure['layout']['yaxis2'].update(title="Tick Rate (ticks/s)")
         else:
             figure['layout']['yaxis1'].update(title="Speed (m/s)")
 
@@ -1273,21 +1291,29 @@
             else:
                 self.logger.warning('Both wheel and vehicle %s data present, but timestamped with different '
                                     'sources. Plotted data may not align in time.')
                 same_time_source = False
                 common_time_source = None
 
         if same_time_source:
-            figure['layout']['annotations'][0]['text'] += \
-                '<br>Time Source: %s' % self._time_source_to_display_name(common_time_source)
-        else:
-            figure['layout']['annotations'][0]['text'] += \
-                '<br>Time Source: %s (Wheel), %s (Vehicle)' % \
-                                                          (self._time_source_to_display_name(wheel_time_source),
-                                                           self._time_source_to_display_name(vehicle_time_source))
+            time_name = self._time_source_to_display_name(common_time_source)
+            figure['layout']['annotations'][0]['text'] += '<br>Time Source: %s' % time_name
+
+            time_label = f'{time_name} Time (sec)'
+            for i in range(len(titles)):
+                figure['layout']['xaxis%d' % (i + 1)].update(title=time_label, showticklabels=True)
+        else:
+            wheel_time_name = self._time_source_to_display_name(wheel_time_source)
+            vehicle_time_name = self._time_source_to_display_name(vehicle_time_source)
+            figure['layout']['annotations'][0]['text'] += '<br>Time Source: %s (Wheel), %s (Vehicle)' % \
+                                                          (wheel_time_name, vehicle_time_name)
+
+            time_label = f'{wheel_time_name}/{vehicle_time_name} Time (sec)'
+            for i in range(len(titles)):
+                figure['layout']['xaxis%d' % (i + 1)].update(title=time_label, showticklabels=True)
 
         p1_time_present = (wheel_time_source == SystemTimeSource.P1_TIME or
                            vehicle_time_source == SystemTimeSource.P1_TIME)
 
         # If plotting speed data, try to plot the navigation engine's speed estimate for reference.
         #
         # Note: Pose data is not read when plotting ticks (ticks do not plot in meters/second). If the wheel data is not
@@ -1492,16 +1518,16 @@
             titles = [t + ' (Uncorrected)' for t in titles]
         else:
             titles = [t + ' (Corrected)' for t in titles]
 
         figure = make_subplots(rows=2, cols=1, print_grid=False, shared_xaxes=True, subplot_titles=titles)
 
         figure['layout'].update(showlegend=True, modebar_add=['v1hovermode'])
-        figure['layout']['xaxis1'].update(title="Time (sec)", showticklabels=True)
-        figure['layout']['xaxis2'].update(title="Time (sec)", showticklabels=True)
+        figure['layout']['xaxis1'].update(title=self.p1_time_label, showticklabels=True)
+        figure['layout']['xaxis2'].update(title=self.p1_time_label, showticklabels=True)
         figure['layout']['yaxis1'].update(title="Acceleration (m/s^2)")
         figure['layout']['yaxis2'].update(title="Rotation Rate (rad/s)")
 
         figure.add_trace(go.Scattergl(x=time, y=data.accel_mps2[0, :], name='X', legendgroup='x',
                                       mode='lines', line={'color': 'red'}),
                          1, 1)
         figure.add_trace(go.Scattergl(x=time, y=data.accel_mps2[1, :], name='Y', legendgroup='y',
@@ -1783,15 +1809,15 @@
 
         # Setup the figure.
         figure = make_subplots(rows=1, cols=1, print_grid=False, shared_xaxes=True,
                                subplot_titles=['GNSS Temperature'])
 
         figure['layout'].update(showlegend=True, modebar_add=['v1hovermode'])
         for i in range(1):
-            figure['layout']['xaxis%d' % (i + 1)].update(title="Time (sec)", showticklabels=True)
+            figure['layout']['xaxis%d' % (i + 1)].update(title=self.p1_time_label, showticklabels=True)
         figure['layout']['yaxis1'].update(title="Temp (deg C)")
 
         # Plot the data.
         time = data.p1_time - float(self.t0)
         figure.add_trace(go.Scattergl(x=time, y=data.gnss_temperature_degc, customdata=data.p1_time,
                                       name='GNSS Temperature',
                                       hovertemplate='Time: %{x:.3f} sec (%{customdata:.3f} sec)',
@@ -2003,27 +2029,21 @@
             '',
             'Processed Duration',
         ]
         times = [
             # Log summary.
             str(self.reader.t0),
             system_time_to_str(self.reader.get_system_t0(), is_seconds=True).replace(' time', ':'),
-            # Note: Temporarily replacing <br> so it doesn't get stripped by _data_to_table().
-            self._gps_sec_to_string(t0_gps) \
-                .replace('<br>', (' (approximated)' if t0_is_approx else '') + '<brbak>') \
-                .replace('<brbak>', '<br>'),
+            self._gps_sec_to_string(t0_gps, is_approx=t0_is_approx),
             log_duration_sec,
             '',
             # Processed data summary.
             str(processed_t0),
             system_time_to_str(processed_system_t0, is_seconds=True).replace(' time', ':'),
-            # Note: Temporarily replacing <br> so it doesn't get stripped by _data_to_table().
-            self._gps_sec_to_string(t0_gps) \
-                .replace('<br>', (' (approximated)' if t0_is_approx else '') + '<brbak>') \
-                .replace('<brbak>', '<br>'),
+            self._gps_sec_to_string(t0_gps, is_approx=t0_is_approx),
             '%.1f seconds' % processing_duration_sec,
         ]
         time_table = _data_to_table(['Description', 'Time'], [descriptions, times])
 
         # Create a table with the types and counts of each FusionEngine message type in the log.
         message_types, message_counts = np.unique(reduced_index['type'], return_counts=True)
         message_types = [MessageType.get_type_string(t) for t in message_types]
@@ -2160,27 +2180,29 @@
             data = result[message_type]
             if len(data.p1_time) > 0:
                 selected_type = message_type_to_class[message_type]
                 break
         return selected_type
 
     @classmethod
-    def _gps_sec_to_string(cls, gps_time_sec):
+    def _gps_sec_to_string(cls, gps_time_sec, is_approx: bool = False):
         if isinstance(gps_time_sec, Timestamp):
             gps_time_sec = float(gps_time_sec)
 
         if np.isnan(gps_time_sec):
             return "GPS: N/A<br>UTC: N/A"
         else:
             SECS_PER_WEEK = 7 * 24 * 3600.0
             week = int(gps_time_sec / SECS_PER_WEEK)
             tow_sec = gps_time_sec - week * SECS_PER_WEEK
             utc_time = gpstime.fromgps(gps_time_sec)
-            return "GPS: %d:%.3f (%.3f sec)<br>UTC: %s" %\
-                   (week, tow_sec, gps_time_sec, datetime_to_string(utc_time, decimals=3))
+            approx_str = ' (approximated)' if is_approx else ''
+            return "GPS: %d:%.3f (%.3f sec)%s<br>UTC: %s%s" %\
+                   (week, tow_sec, gps_time_sec, approx_str,
+                    datetime_to_string(utc_time, decimals=3), approx_str)
 
     @classmethod
     def _get_measurement_time(cls, data, time_source: SystemTimeSource) -> np.ndarray:
         if time_source == SystemTimeSource.P1_TIME:
             return data.p1_time
         else:
             return data.measurement_time
@@ -2224,14 +2246,19 @@
         help="A Mapbox token to use for satellite imagery when generating a map. If unspecified, the token will be "
              "read from the MAPBOX_ACCESS_TOKEN or MapboxAccessToken environment variables if set. If no token is "
              "available, a default map will be displayed using Open Street Maps data.")
     plot_group.add_argument(
         '-m', '--measurements', action=ExtendedBooleanAction,
         help="Plot incoming measurement data (slow). Ignored if --plot is specified.")
     plot_group.add_argument(
+        '--time-axis', choices=('absolute', 'abs', 'relative', 'rel'), default='relative',
+        help="Specify the way in which time will be plotted:"
+             "\n- absolute, abs - Absolute P1 or system timestamps"
+             "\n- relative, rel - Elapsed time since the start of the log")
+    plot_group.add_argument(
         '--truncate', '--trunc', action=ExtendedBooleanAction, default=True,
         help="When processing a very long log (>%.1f hours), reduce or skip some plots that may be very slow to "
              "generate or display. This includes:"
              "\n- GNSS signal status display"
              "\n- High-rate (>%d Hz) measurement data"
              "\n"
              "\nTruncation is disabled if --plot is specified." %
@@ -2328,15 +2355,15 @@
             output_dir = os.path.join(output_dir, 'plot_fusion_engine')
     else:
         output_dir = options.output
 
     # Read pose data from the file.
     analyzer = Analyzer(file=input_path, output_dir=output_dir, ignore_index=options.ignore_index,
                         prefix=options.prefix + '.' if options.prefix is not None else '',
-                        time_range=time_range,
+                        time_range=time_range, time_axis=options.time_axis,
                         truncate_long_logs=options.truncate and options.plot is None)
 
     if options.plot is None:
         analyzer.plot_events()
         analyzer.plot_time_scale()
 
         analyzer.plot_solution_type()
```

### Comparing `fusion-engine-client-1.20.0rc3/fusion_engine_client/analysis/attitude.py` & `fusion-engine-client-1.20.0rc4/fusion_engine_client/analysis/attitude.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.20.0rc3/fusion_engine_client/analysis/data_loader.py` & `fusion-engine-client-1.20.0rc4/fusion_engine_client/analysis/data_loader.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.20.0rc3/fusion_engine_client/messages/configuration.py` & `fusion-engine-client-1.20.0rc4/fusion_engine_client/messages/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -146,14 +146,15 @@
     INVALID = 0,
     SERIAL = 1,
     FILE = 2,
     TCP_CLIENT = 3,
     TCP_SERVER = 4,
     UDP_CLIENT = 5,
     UDP_SERVER = 6,
+    WEBSOCKET_SERVER = 7,
     ## Set/get the configuration for the interface on which the command was received.
     CURRENT = 254,
     ## Set/get the configuration for the all I/O interfaces.
     ALL = 255,
 
 
 class UpdateAction(IntEnum):
```

### Comparing `fusion-engine-client-1.20.0rc3/fusion_engine_client/messages/control.py` & `fusion-engine-client-1.20.0rc4/fusion_engine_client/messages/control.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.20.0rc3/fusion_engine_client/messages/defs.py` & `fusion-engine-client-1.20.0rc4/fusion_engine_client/messages/defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-from __future__ import annotations
-
 import inspect
 import re
 import struct
 import sys
 from typing import Dict, List, Optional, Set, Type, Union
 from zlib import crc32
 
@@ -378,31 +376,31 @@
 class MessagePayload:
     """!
     @brief Message payload API.
     """
 
     _UNSPECIFIED_VERSION = 0x100
 
-    message_type_to_class: Dict[MessageType, Type[MessagePayload]] = {}
+    message_type_to_class: Dict[MessageType, Type['MessagePayload']] = {}
     message_type_by_name: Dict[str, MessageType] = {}
 
     def __init__(self):
         pass
 
     def __init_subclass__(cls, **kwargs):
         MessagePayload.message_type_to_class[cls.get_type()] = cls
         MessagePayload.message_type_by_name[cls.__name__] = cls.get_type()
 
     @classmethod
-    def get_message_class(cls, message_type: MessageType) -> Type[MessagePayload]:
+    def get_message_class(cls, message_type: MessageType) -> Type['MessagePayload']:
         return MessagePayload.message_type_to_class.get(message_type, None)
 
     @classmethod
     def find_matching_message_types(cls, pattern: Union[str, List[str]], return_class: bool = False) -> \
-        Union[Set[MessageType], Set[MessagePayload]]:
+        Union[Set[MessageType], Set['MessagePayload']]:
         """!
         @brief Find one or more @ref MessageType%s that match the specified pattern(s).
 
         Examples:
         ```py
         find_matching_message_types('pose')  # {MessageType.POSE}
         find_matching_message_types('posemessage')  # {MessageType.POSE}
@@ -539,15 +537,15 @@
         else:
             return getattr(self, 'p1_time', None)
 
     def get_system_time_ns(self) -> float:
         measurement_details = getattr(self, 'details', None)
         if isinstance(measurement_details, MeasurementDetails):
             if measurement_details.measurement_time_source == SystemTimeSource.TIMESTAMPED_ON_RECEPTION:
-                return float(measurement_details.measurement_time)
+                return float(measurement_details.measurement_time) * 1e9
             else:
                 return np.nan
         else:
             return getattr(self, 'system_time_ns', None)
 
     def get_system_time_sec(self) -> float:
         system_time_ns = self.get_system_time_ns()
```

### Comparing `fusion-engine-client-1.20.0rc3/fusion_engine_client/messages/device.py` & `fusion-engine-client-1.20.0rc4/fusion_engine_client/messages/device.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.20.0rc3/fusion_engine_client/messages/fault_control.py` & `fusion-engine-client-1.20.0rc4/fusion_engine_client/messages/fault_control.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.20.0rc3/fusion_engine_client/messages/gnss_corrections.py` & `fusion-engine-client-1.20.0rc4/fusion_engine_client/messages/gnss_corrections.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.20.0rc3/fusion_engine_client/messages/measurement_details.py` & `fusion-engine-client-1.20.0rc4/fusion_engine_client/messages/measurement_details.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.20.0rc3/fusion_engine_client/messages/measurements.py` & `fusion-engine-client-1.20.0rc4/fusion_engine_client/messages/measurements.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.20.0rc3/fusion_engine_client/messages/ros.py` & `fusion-engine-client-1.20.0rc4/fusion_engine_client/messages/ros.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.20.0rc3/fusion_engine_client/messages/signal_defs.py` & `fusion-engine-client-1.20.0rc4/fusion_engine_client/messages/signal_defs.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.20.0rc3/fusion_engine_client/messages/solution.py` & `fusion-engine-client-1.20.0rc4/fusion_engine_client/messages/solution.py`

 * *Files 0% similar despite different names*

```diff
@@ -351,21 +351,19 @@
                   f'age={self.corrections_age_sec:.1f} sec, baseline={self.baseline_distance_m * 1e-3:.1f} km]'
         return result
 
     def __str__(self):
         string = 'GNSS Info Message @ %s\n' % str(self.p1_time)
         if self.gps_time:
             gps_str = f'{str(self.gps_time).replace("GPS: ", "")}'
-        else:
-            gps_str = 'None'
-        string += '  GPS time: %s\n' % gps_str
-        if self.utc_time:
             utc_str = f'{datetime_to_string(self.gps_time.as_utc())}'
         else:
+            gps_str = 'None'
             utc_str = 'None'
+        string += '  GPS time: %s\n' % gps_str
         string += '  UTC time: %s\n' % utc_str
         string += '  UTC leap second: %s\n' % \
                   (self.leap_second if self.leap_second != GNSSInfoMessage.INVALID_LEAP_SECOND else 'unknown')
         string += '  # SVs used: %d\n' % self.num_svs
         string += ('  Reference station: %s\n' %
                    (str(self.reference_station_id)
                     if self.reference_station_id != GNSSInfoMessage.INVALID_REFERENCE_STATION
```

### Comparing `fusion-engine-client-1.20.0rc3/fusion_engine_client/messages/timestamp.py` & `fusion-engine-client-1.20.0rc4/fusion_engine_client/messages/timestamp.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.20.0rc3/fusion_engine_client/parsers/decoder.py` & `fusion-engine-client-1.20.0rc4/fusion_engine_client/parsers/decoder.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.20.0rc3/fusion_engine_client/parsers/encoder.py` & `fusion-engine-client-1.20.0rc4/fusion_engine_client/parsers/encoder.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.20.0rc3/fusion_engine_client/parsers/file_index.py` & `fusion-engine-client-1.20.0rc4/fusion_engine_client/parsers/file_index.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-from __future__ import annotations
-
 from typing import Union
 
 from collections import namedtuple
 import copy
 import io
 import os
 
@@ -276,15 +274,15 @@
             raw_data = FileIndex._to_raw(data)
 
             if os.path.exists(index_path):
                 os.remove(index_path)
             raw_data.tofile(index_path)
 
     def get_time_range(self, start: Union[Timestamp, float] = None, stop: Union[Timestamp, float] = None,
-                       hint: str = None, time_range: TimeRange = None) -> FileIndex:
+                       hint: str = None, time_range: TimeRange = None) -> 'FileIndex':
         """!
         @brief Get a subset of the contents for a specified time range.
 
         @param start The P1 time at the start of the desired time range (inclusive).
         @param stop The P1 time at the end of the desired time range (exclusive).
         @param hint A hint indicating how to handle entries that do not have P1 time (`nan` timestamps):
                - `all_nans` - Return _all_ elements with nan timestamps in addition to entries within the time range,
```

### Comparing `fusion-engine-client-1.20.0rc3/fusion_engine_client/parsers/mixed_log_reader.py` & `fusion-engine-client-1.20.0rc4/fusion_engine_client/parsers/mixed_log_reader.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.20.0rc3/fusion_engine_client/utils/argument_parser.py` & `fusion-engine-client-1.20.0rc4/fusion_engine_client/utils/argument_parser.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.20.0rc3/fusion_engine_client/utils/bin_utils.py` & `fusion-engine-client-1.20.0rc4/fusion_engine_client/utils/bin_utils.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.20.0rc3/fusion_engine_client/utils/construct_utils.py` & `fusion-engine-client-1.20.0rc4/fusion_engine_client/utils/construct_utils.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.20.0rc3/fusion_engine_client/utils/enum_utils.py` & `fusion-engine-client-1.20.0rc4/fusion_engine_client/utils/enum_utils.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.20.0rc3/fusion_engine_client/utils/log.py` & `fusion-engine-client-1.20.0rc4/fusion_engine_client/utils/log.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.20.0rc3/fusion_engine_client/utils/numpy_utils.py` & `fusion-engine-client-1.20.0rc4/fusion_engine_client/utils/numpy_utils.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.20.0rc3/fusion_engine_client/utils/time_range.py` & `fusion-engine-client-1.20.0rc4/fusion_engine_client/utils/time_range.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-from __future__ import annotations
-
 import copy
 import math
 from typing import Optional, Tuple, Union
 
 from ..messages.defs import Timestamp
 from ..messages.defs import MessagePayload
 
@@ -137,15 +135,15 @@
         self._in_range_started = False
         self._in_range_ended = False
 
     def restart(self):
         self._in_range_started = False
         self._in_range_ended = False
 
-    def make_absolute(self, p1_t0: Timestamp = None, in_place: bool = True) -> TimeRange:
+    def make_absolute(self, p1_t0: Timestamp = None, in_place: bool = True) -> 'TimeRange':
         if not in_place:
             return copy.deepcopy(self).make_absolute(p1_t0=p1_t0)
 
         if p1_t0 and not self.p1_t0:
             self.p1_t0 = p1_t0
 
         if not self.absolute:
@@ -155,15 +153,15 @@
             if self.start is not None:
                 self.start += float(self.p1_t0)
             if self.end is not None:
                 self.end += float(self.p1_t0)
 
         return self
 
-    def intersect(self, other: TimeRange, in_place: bool = True) -> TimeRange:
+    def intersect(self, other: 'TimeRange', in_place: bool = True) -> 'TimeRange':
         if not in_place:
             return copy.copy(self).intersect(other)
 
         # If either range is absolute, enforce that both ranges are absolute before intersecting.
         if self.absolute and not other.absolute:
             other = other.make_absolute(self.p1_t0, in_place=False)
         elif not self.absolute and other.absolute:
```

### Comparing `fusion-engine-client-1.20.0rc3/fusion_engine_client/utils/trace.py` & `fusion-engine-client-1.20.0rc4/fusion_engine_client/utils/trace.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.20.0rc3/fusion_engine_client.egg-info/PKG-INFO` & `fusion-engine-client-1.20.0rc4/fusion_engine_client.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fusion-engine-client
-Version: 1.20.0rc3
+Version: 1.20.0rc4
 Summary: Point One FusionEngine Library
 Home-page: https://github.com/PointOneNav/fusion-engine-client
 Author: Point One Navigation
 Author-email: support@pointonenav.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -12,21 +12,23 @@
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >3.7
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: all
 Provides-Extra: dev
 Provides-Extra: display
 Provides-Extra: tools
 
 Point One FusionEngine protocol support for real-time interaction and control, plus post-processing data analysis tools.
```

### Comparing `fusion-engine-client-1.20.0rc3/fusion_engine_client.egg-info/SOURCES.txt` & `fusion-engine-client-1.20.0rc4/fusion_engine_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.20.0rc3/setup.py` & `fusion-engine-client-1.20.0rc4/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,26 +13,26 @@
     raise RuntimeError("Unable to find version string.")
 
 
 version = find_version('fusion_engine_client', '__init__.py')
 
 tools_requirements = set([
     'argparse-formatter>=1.4',
-    'scipy>=1.6.0',
+    'scipy>=1.5.0',
 ])
 
 display_requirements = set([
     'colorama>=0.4.4',
     'palettable>=3.3.0',
     'plotly>=4.0.0',
     'pymap3d>=2.4.3',
 ]) | tools_requirements
 
 dev_requirements = set([
-    'packaging>=23.0.0',
+    'packaging>=21.0.0',
 ]) | tools_requirements
 
 all_requirements = tools_requirements | display_requirements | dev_requirements
 
 setup(
     name='fusion-engine-client',
     version=version,
@@ -54,29 +54,31 @@
         'Intended Audience :: Science/Research',
         'License :: OSI Approved :: MIT License',
         'Operating System :: MacOS :: MacOS X',
         'Operating System :: Microsoft :: Windows',
         'Operating System :: POSIX',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
+        'Programming Language :: Python :: 3.6',
+        'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
         'Topic :: Software Development :: Libraries',
         'Topic :: Software Development :: Libraries :: Python Modules',
     ],
     url='https://github.com/PointOneNav/fusion-engine-client',
     packages=find_packages(where='.'),
     scripts=[
         'bin/p1_display',
         'bin/p1_extract',
         'bin/p1_print',
     ],
-    python_requires='>3.7',
+    python_requires='>=3.6',
     setup_requires=[
         'wheel>=0.36.2',
     ],
     install_requires=[
         'aenum>=3.1.1',
         'gpstime>=0.6.2',
         'numpy>=1.16.0',
```

### Comparing `fusion-engine-client-1.20.0rc3/tests/test_config.py` & `fusion-engine-client-1.20.0rc4/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.20.0rc3/tests/test_construct_utils.py` & `fusion-engine-client-1.20.0rc4/tests/test_construct_utils.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.20.0rc3/tests/test_data_loader.py` & `fusion-engine-client-1.20.0rc4/tests/test_data_loader.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.20.0rc3/tests/test_decoder.py` & `fusion-engine-client-1.20.0rc4/tests/test_decoder.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.20.0rc3/tests/test_encoder.py` & `fusion-engine-client-1.20.0rc4/tests/test_encoder.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.20.0rc3/tests/test_enum_utils.py` & `fusion-engine-client-1.20.0rc4/tests/test_enum_utils.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.20.0rc3/tests/test_file_index.py` & `fusion-engine-client-1.20.0rc4/tests/test_file_index.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.20.0rc3/tests/test_message_defs.py` & `fusion-engine-client-1.20.0rc4/tests/test_message_defs.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.20.0rc3/tests/test_mixed_log_reader.py` & `fusion-engine-client-1.20.0rc4/tests/test_mixed_log_reader.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.20.0rc3/tests/test_time_range.py` & `fusion-engine-client-1.20.0rc4/tests/test_time_range.py`

 * *Files identical despite different names*

