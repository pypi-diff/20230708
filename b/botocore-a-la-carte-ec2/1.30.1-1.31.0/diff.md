# Comparing `tmp/botocore-a-la-carte-ec2-1.30.1.tar.gz` & `tmp/botocore-a-la-carte-ec2-1.31.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botocore-a-la-carte-ec2-1.30.1.tar", last modified: Thu Jul  6 01:45:02 2023, max compression
+gzip compressed data, was "botocore-a-la-carte-ec2-1.31.0.tar", last modified: Fri Jul  7 01:43:52 2023, max compression
```

## Comparing `botocore-a-la-carte-ec2-1.30.1.tar` & `botocore-a-la-carte-ec2-1.31.0.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 01:45:02.258756 botocore-a-la-carte-ec2-1.30.1/
--rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-07-06 01:45:02.000000 botocore-a-la-carte-ec2-1.30.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-07-06 01:45:02.258756 botocore-a-la-carte-ec2-1.30.1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 01:45:02.242756 botocore-a-la-carte-ec2-1.30.1/botocore/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 01:45:02.242756 botocore-a-la-carte-ec2-1.30.1/botocore/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 01:45:02.242756 botocore-a-la-carte-ec2-1.30.1/botocore/data/ec2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 01:45:02.246756 botocore-a-la-carte-ec2-1.30.1/botocore/data/ec2/2014-09-01/
--rw-r--r--   0 runner    (1001) docker     (123)    14695 2023-07-06 01:44:40.000000 botocore-a-la-carte-ec2-1.30.1/botocore/data/ec2/2014-09-01/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-07-06 01:44:40.000000 botocore-a-la-carte-ec2-1.30.1/botocore/data/ec2/2014-09-01/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (123)   539923 2023-07-06 01:44:40.000000 botocore-a-la-carte-ec2-1.30.1/botocore/data/ec2/2014-09-01/service-2.json
--rw-r--r--   0 runner    (1001) docker     (123)     8548 2023-07-06 01:44:40.000000 botocore-a-la-carte-ec2-1.30.1/botocore/data/ec2/2014-09-01/waiters-2.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 01:45:02.246756 botocore-a-la-carte-ec2-1.30.1/botocore/data/ec2/2014-10-01/
--rw-r--r--   0 runner    (1001) docker     (123)    14695 2023-07-06 01:44:40.000000 botocore-a-la-carte-ec2-1.30.1/botocore/data/ec2/2014-10-01/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-07-06 01:44:40.000000 botocore-a-la-carte-ec2-1.30.1/botocore/data/ec2/2014-10-01/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (123)   566499 2023-07-06 01:44:40.000000 botocore-a-la-carte-ec2-1.30.1/botocore/data/ec2/2014-10-01/service-2.json
--rw-r--r--   0 runner    (1001) docker     (123)    11040 2023-07-06 01:44:40.000000 botocore-a-la-carte-ec2-1.30.1/botocore/data/ec2/2014-10-01/waiters-2.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 01:45:02.246756 botocore-a-la-carte-ec2-1.30.1/botocore/data/ec2/2015-03-01/
--rw-r--r--   0 runner    (1001) docker     (123)    14695 2023-07-06 01:44:40.000000 botocore-a-la-carte-ec2-1.30.1/botocore/data/ec2/2015-03-01/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-07-06 01:44:40.000000 botocore-a-la-carte-ec2-1.30.1/botocore/data/ec2/2015-03-01/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (123)   588390 2023-07-06 01:44:40.000000 botocore-a-la-carte-ec2-1.30.1/botocore/data/ec2/2015-03-01/service-2.json
--rw-r--r--   0 runner    (1001) docker     (123)    11040 2023-07-06 01:44:40.000000 botocore-a-la-carte-ec2-1.30.1/botocore/data/ec2/2015-03-01/waiters-2.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 01:45:02.246756 botocore-a-la-carte-ec2-1.30.1/botocore/data/ec2/2015-04-15/
--rw-r--r--   0 runner    (1001) docker     (123)    14695 2023-07-06 01:44:40.000000 botocore-a-la-carte-ec2-1.30.1/botocore/data/ec2/2015-04-15/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-07-06 01:44:40.000000 botocore-a-la-carte-ec2-1.30.1/botocore/data/ec2/2015-04-15/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (123)   715324 2023-07-06 01:44:40.000000 botocore-a-la-carte-ec2-1.30.1/botocore/data/ec2/2015-04-15/service-2.json
--rw-r--r--   0 runner    (1001) docker     (123)    11546 2023-07-06 01:44:40.000000 botocore-a-la-carte-ec2-1.30.1/botocore/data/ec2/2015-04-15/waiters-2.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 01:45:02.250756 botocore-a-la-carte-ec2-1.30.1/botocore/data/ec2/2015-10-01/
--rw-r--r--   0 runner    (1001) docker     (123)    14695 2023-07-06 01:44:40.000000 botocore-a-la-carte-ec2-1.30.1/botocore/data/ec2/2015-10-01/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-06 01:44:40.000000 botocore-a-la-carte-ec2-1.30.1/botocore/data/ec2/2015-10-01/examples-1.json
--rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-07-06 01:44:40.000000 botocore-a-la-carte-ec2-1.30.1/botocore/data/ec2/2015-10-01/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (123)   847080 2023-07-06 01:44:40.000000 botocore-a-la-carte-ec2-1.30.1/botocore/data/ec2/2015-10-01/service-2.json
--rw-r--r--   0 runner    (1001) docker     (123)    14823 2023-07-06 01:44:40.000000 botocore-a-la-carte-ec2-1.30.1/botocore/data/ec2/2015-10-01/waiters-2.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 01:45:02.250756 botocore-a-la-carte-ec2-1.30.1/botocore/data/ec2/2016-04-01/
--rw-r--r--   0 runner    (1001) docker     (123)    14695 2023-07-06 01:44:40.000000 botocore-a-la-carte-ec2-1.30.1/botocore/data/ec2/2016-04-01/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (123)   109914 2023-07-06 01:44:40.000000 botocore-a-la-carte-ec2-1.30.1/botocore/data/ec2/2016-04-01/examples-1.json
--rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-07-06 01:44:40.000000 botocore-a-la-carte-ec2-1.30.1/botocore/data/ec2/2016-04-01/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (123)   878250 2023-07-06 01:44:40.000000 botocore-a-la-carte-ec2-1.30.1/botocore/data/ec2/2016-04-01/service-2.json
--rw-r--r--   0 runner    (1001) docker     (123)    15259 2023-07-06 01:44:40.000000 botocore-a-la-carte-ec2-1.30.1/botocore/data/ec2/2016-04-01/waiters-2.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 01:45:02.254756 botocore-a-la-carte-ec2-1.30.1/botocore/data/ec2/2016-09-15/
--rw-r--r--   0 runner    (1001) docker     (123)    14695 2023-07-06 01:44:40.000000 botocore-a-la-carte-ec2-1.30.1/botocore/data/ec2/2016-09-15/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (123)   110174 2023-07-06 01:44:40.000000 botocore-a-la-carte-ec2-1.30.1/botocore/data/ec2/2016-09-15/examples-1.json
--rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-07-06 01:44:40.000000 botocore-a-la-carte-ec2-1.30.1/botocore/data/ec2/2016-09-15/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (123)   891280 2023-07-06 01:44:40.000000 botocore-a-la-carte-ec2-1.30.1/botocore/data/ec2/2016-09-15/service-2.json
--rw-r--r--   0 runner    (1001) docker     (123)    14875 2023-07-06 01:44:40.000000 botocore-a-la-carte-ec2-1.30.1/botocore/data/ec2/2016-09-15/waiters-2.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 01:45:02.258756 botocore-a-la-carte-ec2-1.30.1/botocore/data/ec2/2016-11-15/
--rw-r--r--   0 runner    (1001) docker     (123)    19575 2023-07-06 01:44:40.000000 botocore-a-la-carte-ec2-1.30.1/botocore/data/ec2/2016-11-15/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (123)   147949 2023-07-06 01:44:40.000000 botocore-a-la-carte-ec2-1.30.1/botocore/data/ec2/2016-11-15/examples-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    26102 2023-07-06 01:44:40.000000 botocore-a-la-carte-ec2-1.30.1/botocore/data/ec2/2016-11-15/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-07-06 01:44:40.000000 botocore-a-la-carte-ec2-1.30.1/botocore/data/ec2/2016-11-15/paginators-1.sdk-extras.json
--rw-r--r--   0 runner    (1001) docker     (123)  2879126 2023-07-06 01:44:40.000000 botocore-a-la-carte-ec2-1.30.1/botocore/data/ec2/2016-11-15/service-2.json
--rw-r--r--   0 runner    (1001) docker     (123)    17748 2023-07-06 01:44:40.000000 botocore-a-la-carte-ec2-1.30.1/botocore/data/ec2/2016-11-15/waiters-2.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 01:45:02.258756 botocore-a-la-carte-ec2-1.30.1/botocore_a_la_carte_ec2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-07-06 01:45:02.000000 botocore-a-la-carte-ec2-1.30.1/botocore_a_la_carte_ec2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-07-06 01:45:02.000000 botocore-a-la-carte-ec2-1.30.1/botocore_a_la_carte_ec2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 01:45:02.000000 botocore-a-la-carte-ec2-1.30.1/botocore_a_la_carte_ec2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-06 01:45:02.000000 botocore-a-la-carte-ec2-1.30.1/botocore_a_la_carte_ec2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 01:45:02.258756 botocore-a-la-carte-ec2-1.30.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-07-06 01:45:02.000000 botocore-a-la-carte-ec2-1.30.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 01:43:52.819285 botocore-a-la-carte-ec2-1.31.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-07-07 01:43:52.000000 botocore-a-la-carte-ec2-1.31.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-07-07 01:43:52.819285 botocore-a-la-carte-ec2-1.31.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 01:43:52.803285 botocore-a-la-carte-ec2-1.31.0/botocore/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 01:43:52.803285 botocore-a-la-carte-ec2-1.31.0/botocore/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 01:43:52.803285 botocore-a-la-carte-ec2-1.31.0/botocore/data/ec2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 01:43:52.807285 botocore-a-la-carte-ec2-1.31.0/botocore/data/ec2/2014-09-01/
+-rw-r--r--   0 runner    (1001) docker     (123)    14695 2023-07-07 01:43:28.000000 botocore-a-la-carte-ec2-1.31.0/botocore/data/ec2/2014-09-01/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-07-07 01:43:28.000000 botocore-a-la-carte-ec2-1.31.0/botocore/data/ec2/2014-09-01/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)   539923 2023-07-07 01:43:28.000000 botocore-a-la-carte-ec2-1.31.0/botocore/data/ec2/2014-09-01/service-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8548 2023-07-07 01:43:28.000000 botocore-a-la-carte-ec2-1.31.0/botocore/data/ec2/2014-09-01/waiters-2.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 01:43:52.807285 botocore-a-la-carte-ec2-1.31.0/botocore/data/ec2/2014-10-01/
+-rw-r--r--   0 runner    (1001) docker     (123)    14695 2023-07-07 01:43:28.000000 botocore-a-la-carte-ec2-1.31.0/botocore/data/ec2/2014-10-01/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-07-07 01:43:28.000000 botocore-a-la-carte-ec2-1.31.0/botocore/data/ec2/2014-10-01/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)   566499 2023-07-07 01:43:28.000000 botocore-a-la-carte-ec2-1.31.0/botocore/data/ec2/2014-10-01/service-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11040 2023-07-07 01:43:28.000000 botocore-a-la-carte-ec2-1.31.0/botocore/data/ec2/2014-10-01/waiters-2.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 01:43:52.807285 botocore-a-la-carte-ec2-1.31.0/botocore/data/ec2/2015-03-01/
+-rw-r--r--   0 runner    (1001) docker     (123)    14695 2023-07-07 01:43:28.000000 botocore-a-la-carte-ec2-1.31.0/botocore/data/ec2/2015-03-01/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-07-07 01:43:28.000000 botocore-a-la-carte-ec2-1.31.0/botocore/data/ec2/2015-03-01/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)   588390 2023-07-07 01:43:28.000000 botocore-a-la-carte-ec2-1.31.0/botocore/data/ec2/2015-03-01/service-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11040 2023-07-07 01:43:28.000000 botocore-a-la-carte-ec2-1.31.0/botocore/data/ec2/2015-03-01/waiters-2.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 01:43:52.811285 botocore-a-la-carte-ec2-1.31.0/botocore/data/ec2/2015-04-15/
+-rw-r--r--   0 runner    (1001) docker     (123)    14695 2023-07-07 01:43:28.000000 botocore-a-la-carte-ec2-1.31.0/botocore/data/ec2/2015-04-15/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-07-07 01:43:28.000000 botocore-a-la-carte-ec2-1.31.0/botocore/data/ec2/2015-04-15/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)   715324 2023-07-07 01:43:28.000000 botocore-a-la-carte-ec2-1.31.0/botocore/data/ec2/2015-04-15/service-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11546 2023-07-07 01:43:28.000000 botocore-a-la-carte-ec2-1.31.0/botocore/data/ec2/2015-04-15/waiters-2.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 01:43:52.811285 botocore-a-la-carte-ec2-1.31.0/botocore/data/ec2/2015-10-01/
+-rw-r--r--   0 runner    (1001) docker     (123)    14695 2023-07-07 01:43:28.000000 botocore-a-la-carte-ec2-1.31.0/botocore/data/ec2/2015-10-01/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-07 01:43:28.000000 botocore-a-la-carte-ec2-1.31.0/botocore/data/ec2/2015-10-01/examples-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-07-07 01:43:28.000000 botocore-a-la-carte-ec2-1.31.0/botocore/data/ec2/2015-10-01/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)   847080 2023-07-07 01:43:28.000000 botocore-a-la-carte-ec2-1.31.0/botocore/data/ec2/2015-10-01/service-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)    14823 2023-07-07 01:43:28.000000 botocore-a-la-carte-ec2-1.31.0/botocore/data/ec2/2015-10-01/waiters-2.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 01:43:52.811285 botocore-a-la-carte-ec2-1.31.0/botocore/data/ec2/2016-04-01/
+-rw-r--r--   0 runner    (1001) docker     (123)    14695 2023-07-07 01:43:28.000000 botocore-a-la-carte-ec2-1.31.0/botocore/data/ec2/2016-04-01/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)   109914 2023-07-07 01:43:28.000000 botocore-a-la-carte-ec2-1.31.0/botocore/data/ec2/2016-04-01/examples-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-07-07 01:43:28.000000 botocore-a-la-carte-ec2-1.31.0/botocore/data/ec2/2016-04-01/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)   878250 2023-07-07 01:43:28.000000 botocore-a-la-carte-ec2-1.31.0/botocore/data/ec2/2016-04-01/service-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)    15259 2023-07-07 01:43:28.000000 botocore-a-la-carte-ec2-1.31.0/botocore/data/ec2/2016-04-01/waiters-2.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 01:43:52.815286 botocore-a-la-carte-ec2-1.31.0/botocore/data/ec2/2016-09-15/
+-rw-r--r--   0 runner    (1001) docker     (123)    14695 2023-07-07 01:43:28.000000 botocore-a-la-carte-ec2-1.31.0/botocore/data/ec2/2016-09-15/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)   110174 2023-07-07 01:43:28.000000 botocore-a-la-carte-ec2-1.31.0/botocore/data/ec2/2016-09-15/examples-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-07-07 01:43:28.000000 botocore-a-la-carte-ec2-1.31.0/botocore/data/ec2/2016-09-15/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)   891280 2023-07-07 01:43:28.000000 botocore-a-la-carte-ec2-1.31.0/botocore/data/ec2/2016-09-15/service-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)    14875 2023-07-07 01:43:28.000000 botocore-a-la-carte-ec2-1.31.0/botocore/data/ec2/2016-09-15/waiters-2.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 01:43:52.819285 botocore-a-la-carte-ec2-1.31.0/botocore/data/ec2/2016-11-15/
+-rw-r--r--   0 runner    (1001) docker     (123)    19575 2023-07-07 01:43:28.000000 botocore-a-la-carte-ec2-1.31.0/botocore/data/ec2/2016-11-15/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)   147949 2023-07-07 01:43:28.000000 botocore-a-la-carte-ec2-1.31.0/botocore/data/ec2/2016-11-15/examples-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    26102 2023-07-07 01:43:28.000000 botocore-a-la-carte-ec2-1.31.0/botocore/data/ec2/2016-11-15/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-07-07 01:43:28.000000 botocore-a-la-carte-ec2-1.31.0/botocore/data/ec2/2016-11-15/paginators-1.sdk-extras.json
+-rw-r--r--   0 runner    (1001) docker     (123)  2879536 2023-07-07 01:43:28.000000 botocore-a-la-carte-ec2-1.31.0/botocore/data/ec2/2016-11-15/service-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)    17748 2023-07-07 01:43:28.000000 botocore-a-la-carte-ec2-1.31.0/botocore/data/ec2/2016-11-15/waiters-2.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 01:43:52.819285 botocore-a-la-carte-ec2-1.31.0/botocore_a_la_carte_ec2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-07-07 01:43:52.000000 botocore-a-la-carte-ec2-1.31.0/botocore_a_la_carte_ec2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-07-07 01:43:52.000000 botocore-a-la-carte-ec2-1.31.0/botocore_a_la_carte_ec2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 01:43:52.000000 botocore-a-la-carte-ec2-1.31.0/botocore_a_la_carte_ec2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-07 01:43:52.000000 botocore-a-la-carte-ec2-1.31.0/botocore_a_la_carte_ec2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 01:43:52.819285 botocore-a-la-carte-ec2-1.31.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-07-07 01:43:52.000000 botocore-a-la-carte-ec2-1.31.0/setup.py
```

### Comparing `botocore-a-la-carte-ec2-1.30.1/LICENSE.txt` & `botocore-a-la-carte-ec2-1.31.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-ec2-1.30.1/PKG-INFO` & `botocore-a-la-carte-ec2-1.31.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-ec2
-Version: 1.30.1
+Version: 1.31.0
 Summary: ec2 data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-ec2-1.30.1/botocore/data/ec2/2014-09-01/endpoint-rule-set-1.json` & `botocore-a-la-carte-ec2-1.31.0/botocore/data/ec2/2014-09-01/endpoint-rule-set-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-ec2-1.30.1/botocore/data/ec2/2014-09-01/paginators-1.json` & `botocore-a-la-carte-ec2-1.31.0/botocore/data/ec2/2014-09-01/paginators-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-ec2-1.30.1/botocore/data/ec2/2014-09-01/service-2.json` & `botocore-a-la-carte-ec2-1.31.0/botocore/data/ec2/2014-09-01/service-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-ec2-1.30.1/botocore/data/ec2/2014-09-01/waiters-2.json` & `botocore-a-la-carte-ec2-1.31.0/botocore/data/ec2/2014-09-01/waiters-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-ec2-1.30.1/botocore/data/ec2/2014-10-01/endpoint-rule-set-1.json` & `botocore-a-la-carte-ec2-1.31.0/botocore/data/ec2/2014-10-01/endpoint-rule-set-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-ec2-1.30.1/botocore/data/ec2/2014-10-01/paginators-1.json` & `botocore-a-la-carte-ec2-1.31.0/botocore/data/ec2/2014-10-01/paginators-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-ec2-1.30.1/botocore/data/ec2/2014-10-01/service-2.json` & `botocore-a-la-carte-ec2-1.31.0/botocore/data/ec2/2014-10-01/service-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-ec2-1.30.1/botocore/data/ec2/2014-10-01/waiters-2.json` & `botocore-a-la-carte-ec2-1.31.0/botocore/data/ec2/2014-10-01/waiters-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-ec2-1.30.1/botocore/data/ec2/2015-03-01/endpoint-rule-set-1.json` & `botocore-a-la-carte-ec2-1.31.0/botocore/data/ec2/2015-03-01/endpoint-rule-set-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-ec2-1.30.1/botocore/data/ec2/2015-03-01/paginators-1.json` & `botocore-a-la-carte-ec2-1.31.0/botocore/data/ec2/2015-03-01/paginators-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-ec2-1.30.1/botocore/data/ec2/2015-03-01/service-2.json` & `botocore-a-la-carte-ec2-1.31.0/botocore/data/ec2/2015-03-01/service-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-ec2-1.30.1/botocore/data/ec2/2015-03-01/waiters-2.json` & `botocore-a-la-carte-ec2-1.31.0/botocore/data/ec2/2015-03-01/waiters-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-ec2-1.30.1/botocore/data/ec2/2015-04-15/endpoint-rule-set-1.json` & `botocore-a-la-carte-ec2-1.31.0/botocore/data/ec2/2015-04-15/endpoint-rule-set-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-ec2-1.30.1/botocore/data/ec2/2015-04-15/paginators-1.json` & `botocore-a-la-carte-ec2-1.31.0/botocore/data/ec2/2015-04-15/paginators-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-ec2-1.30.1/botocore/data/ec2/2015-04-15/service-2.json` & `botocore-a-la-carte-ec2-1.31.0/botocore/data/ec2/2015-04-15/service-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-ec2-1.30.1/botocore/data/ec2/2015-04-15/waiters-2.json` & `botocore-a-la-carte-ec2-1.31.0/botocore/data/ec2/2015-04-15/waiters-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-ec2-1.30.1/botocore/data/ec2/2015-10-01/endpoint-rule-set-1.json` & `botocore-a-la-carte-ec2-1.31.0/botocore/data/ec2/2015-10-01/endpoint-rule-set-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-ec2-1.30.1/botocore/data/ec2/2015-10-01/paginators-1.json` & `botocore-a-la-carte-ec2-1.31.0/botocore/data/ec2/2015-10-01/paginators-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-ec2-1.30.1/botocore/data/ec2/2015-10-01/service-2.json` & `botocore-a-la-carte-ec2-1.31.0/botocore/data/ec2/2015-10-01/service-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-ec2-1.30.1/botocore/data/ec2/2015-10-01/waiters-2.json` & `botocore-a-la-carte-ec2-1.31.0/botocore/data/ec2/2015-10-01/waiters-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-ec2-1.30.1/botocore/data/ec2/2016-04-01/endpoint-rule-set-1.json` & `botocore-a-la-carte-ec2-1.31.0/botocore/data/ec2/2016-04-01/endpoint-rule-set-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-ec2-1.30.1/botocore/data/ec2/2016-04-01/examples-1.json` & `botocore-a-la-carte-ec2-1.31.0/botocore/data/ec2/2016-04-01/examples-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-ec2-1.30.1/botocore/data/ec2/2016-04-01/paginators-1.json` & `botocore-a-la-carte-ec2-1.31.0/botocore/data/ec2/2016-04-01/paginators-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-ec2-1.30.1/botocore/data/ec2/2016-04-01/service-2.json` & `botocore-a-la-carte-ec2-1.31.0/botocore/data/ec2/2016-04-01/service-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-ec2-1.30.1/botocore/data/ec2/2016-04-01/waiters-2.json` & `botocore-a-la-carte-ec2-1.31.0/botocore/data/ec2/2016-04-01/waiters-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-ec2-1.30.1/botocore/data/ec2/2016-09-15/endpoint-rule-set-1.json` & `botocore-a-la-carte-ec2-1.31.0/botocore/data/ec2/2016-09-15/endpoint-rule-set-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-ec2-1.30.1/botocore/data/ec2/2016-09-15/examples-1.json` & `botocore-a-la-carte-ec2-1.31.0/botocore/data/ec2/2016-09-15/examples-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-ec2-1.30.1/botocore/data/ec2/2016-09-15/paginators-1.json` & `botocore-a-la-carte-ec2-1.31.0/botocore/data/ec2/2016-09-15/paginators-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-ec2-1.30.1/botocore/data/ec2/2016-09-15/service-2.json` & `botocore-a-la-carte-ec2-1.31.0/botocore/data/ec2/2016-09-15/service-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-ec2-1.30.1/botocore/data/ec2/2016-09-15/waiters-2.json` & `botocore-a-la-carte-ec2-1.31.0/botocore/data/ec2/2016-09-15/waiters-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-ec2-1.30.1/botocore/data/ec2/2016-11-15/endpoint-rule-set-1.json` & `botocore-a-la-carte-ec2-1.31.0/botocore/data/ec2/2016-11-15/endpoint-rule-set-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-ec2-1.30.1/botocore/data/ec2/2016-11-15/examples-1.json` & `botocore-a-la-carte-ec2-1.31.0/botocore/data/ec2/2016-11-15/examples-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-ec2-1.30.1/botocore/data/ec2/2016-11-15/paginators-1.json` & `botocore-a-la-carte-ec2-1.31.0/botocore/data/ec2/2016-11-15/paginators-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-ec2-1.30.1/botocore/data/ec2/2016-11-15/service-2.json` & `botocore-a-la-carte-ec2-1.31.0/botocore/data/ec2/2016-11-15/service-2.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999479366352085%*

 * *Differences: {"'operations'": "{'StopInstances': {'documentation': '<p>Stops an Amazon EBS-backed instance. For "*

 * *                 'more information, see <a '*

 * *                 'href="https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/Stop_Start.html">Stop '*

 * *                 'and start your instance</a> in the <i>Amazon EC2 User Guide</i>.</p> <p>You can '*

 * *                 'use the Stop action to hibernate an instance if the instance is <a '*

 * *                 'href="https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/ena […]*

```diff
@@ -8020,15 +8020,15 @@
             },
             "name": "StartVpcEndpointServicePrivateDnsVerification",
             "output": {
                 "shape": "StartVpcEndpointServicePrivateDnsVerificationResult"
             }
         },
         "StopInstances": {
-            "documentation": "<p>Stops an Amazon EBS-backed instance. For more information, see <a href=\"https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/Stop_Start.html\">Stop and start your instance</a> in the <i>Amazon EC2 User Guide</i>.</p> <p>You can use the Stop action to hibernate an instance if the instance is <a href=\"https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/Hibernate.html#enabling-hibernation\">enabled for hibernation</a> and it meets the <a href=\"https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/Hibernate.html#hibernating-prerequisites\">hibernation prerequisites</a>. For more information, see <a href=\"https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/Hibernate.html\">Hibernate your instance</a> in the <i>Amazon EC2 User Guide</i>.</p> <p>We don't charge usage for a stopped instance, or data transfer fees; however, your root partition Amazon EBS volume remains and continues to persist your data, and you are charged for Amazon EBS volume usage. Every time you start your instance, Amazon EC2 charges a one-minute minimum for instance usage, and thereafter charges per second for instance usage.</p> <p>You can't stop or hibernate instance store-backed instances. You can't use the Stop action to hibernate Spot Instances, but you can specify that Amazon EC2 should hibernate Spot Instances when they are interrupted. For more information, see <a href=\"https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/spot-interruptions.html#hibernate-spot-instances\">Hibernating interrupted Spot Instances</a> in the <i>Amazon EC2 User Guide</i>.</p> <p>When you stop or hibernate an instance, we shut it down. You can restart your instance at any time. Before stopping or hibernating an instance, make sure it is in a state from which it can be restarted. Stopping an instance does not preserve data stored in RAM, but hibernating an instance does preserve data stored in RAM. If an instance cannot hibernate successfully, a normal shutdown occurs.</p> <p>Stopping and hibernating an instance is different to rebooting or terminating it. For example, when you stop or hibernate an instance, the root device and any other devices attached to the instance persist. When you terminate an instance, the root device and any other devices attached during the instance launch are automatically deleted. For more information about the differences between rebooting, stopping, hibernating, and terminating instances, see <a href=\"https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/ec2-instance-lifecycle.html\">Instance lifecycle</a> in the <i>Amazon EC2 User Guide</i>.</p> <p>When you stop an instance, we attempt to shut it down forcibly after a short while. If your instance appears stuck in the stopping state after a period of time, there may be an issue with the underlying host computer. For more information, see <a href=\"https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/TroubleshootingInstancesStopping.html\">Troubleshoot stopping your instance</a> in the <i>Amazon EC2 User Guide</i>.</p>",
+            "documentation": "<p>Stops an Amazon EBS-backed instance. For more information, see <a href=\"https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/Stop_Start.html\">Stop and start your instance</a> in the <i>Amazon EC2 User Guide</i>.</p> <p>You can use the Stop action to hibernate an instance if the instance is <a href=\"https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/enabling-hibernation.html\">enabled for hibernation</a> and it meets the <a href=\"https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/hibernating-prerequisites.html\">hibernation prerequisites</a>. For more information, see <a href=\"https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/Hibernate.html\">Hibernate your instance</a> in the <i>Amazon EC2 User Guide</i>.</p> <p>We don't charge usage for a stopped instance, or data transfer fees; however, your root partition Amazon EBS volume remains and continues to persist your data, and you are charged for Amazon EBS volume usage. Every time you start your instance, Amazon EC2 charges a one-minute minimum for instance usage, and thereafter charges per second for instance usage.</p> <p>You can't stop or hibernate instance store-backed instances. You can't use the Stop action to hibernate Spot Instances, but you can specify that Amazon EC2 should hibernate Spot Instances when they are interrupted. For more information, see <a href=\"https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/spot-interruptions.html#hibernate-spot-instances\">Hibernating interrupted Spot Instances</a> in the <i>Amazon EC2 User Guide</i>.</p> <p>When you stop or hibernate an instance, we shut it down. You can restart your instance at any time. Before stopping or hibernating an instance, make sure it is in a state from which it can be restarted. Stopping an instance does not preserve data stored in RAM, but hibernating an instance does preserve data stored in RAM. If an instance cannot hibernate successfully, a normal shutdown occurs.</p> <p>Stopping and hibernating an instance is different to rebooting or terminating it. For example, when you stop or hibernate an instance, the root device and any other devices attached to the instance persist. When you terminate an instance, the root device and any other devices attached during the instance launch are automatically deleted. For more information about the differences between rebooting, stopping, hibernating, and terminating instances, see <a href=\"https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/ec2-instance-lifecycle.html\">Instance lifecycle</a> in the <i>Amazon EC2 User Guide</i>.</p> <p>When you stop an instance, we attempt to shut it down forcibly after a short while. If your instance appears stuck in the stopping state after a period of time, there may be an issue with the underlying host computer. For more information, see <a href=\"https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/TroubleshootingInstancesStopping.html\">Troubleshoot stopping your instance</a> in the <i>Amazon EC2 User Guide</i>.</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/"
             },
             "input": {
                 "shape": "StopInstancesRequest"
             },
@@ -33726,29 +33726,29 @@
             },
             "type": "list"
         },
         "HibernationFlag": {
             "type": "boolean"
         },
         "HibernationOptions": {
-            "documentation": "<p>Indicates whether your instance is configured for hibernation. This parameter is valid only if the instance meets the <a href=\"https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/Hibernate.html#hibernating-prerequisites\">hibernation prerequisites</a>. For more information, see <a href=\"https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/Hibernate.html\">Hibernate your instance</a> in the <i>Amazon EC2 User Guide</i>.</p>",
+            "documentation": "<p>Indicates whether your instance is configured for hibernation. This parameter is valid only if the instance meets the <a href=\"https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/hibernating-prerequisites.html\">hibernation prerequisites</a>. For more information, see <a href=\"https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/Hibernate.html\">Hibernate your instance</a> in the <i>Amazon EC2 User Guide</i>.</p>",
             "members": {
                 "Configured": {
-                    "documentation": "<p>If this parameter is set to <code>true</code>, your instance is enabled for hibernation; otherwise, it is not enabled for hibernation.</p>",
+                    "documentation": "<p>If <code>true</code>, your instance is enabled for hibernation; otherwise, it is not enabled for hibernation.</p>",
                     "locationName": "configured",
                     "shape": "Boolean"
                 }
             },
             "type": "structure"
         },
         "HibernationOptionsRequest": {
-            "documentation": "<p>Indicates whether your instance is configured for hibernation. This parameter is valid only if the instance meets the <a href=\"https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/Hibernate.html#hibernating-prerequisites\">hibernation prerequisites</a>. For more information, see <a href=\"https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/Hibernate.html\">Hibernate your instance</a> in the <i>Amazon EC2 User Guide</i>.</p>",
+            "documentation": "<p>Indicates whether your instance is configured for hibernation. This parameter is valid only if the instance meets the <a href=\"https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/hibernating-prerequisites.html\">hibernation prerequisites</a>. For more information, see <a href=\"https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/Hibernate.html\">Hibernate your instance</a> in the <i>Amazon EC2 User Guide</i>.</p>",
             "members": {
                 "Configured": {
-                    "documentation": "<p>If you set this parameter to <code>true</code>, your instance is enabled for hibernation.</p> <p>Default: <code>false</code> </p>",
+                    "documentation": "<p>Set to <code>true</code> to enable your instance for hibernation.</p> <p>Default: <code>false</code> </p>",
                     "shape": "Boolean"
                 }
             },
             "type": "structure"
         },
         "HistoryRecord": {
             "documentation": "<p>Describes an event in the history of the Spot Fleet request.</p>",
@@ -38230,14 +38230,19 @@
                     "shape": "MemoryInfo"
                 },
                 "NetworkInfo": {
                     "documentation": "<p>Describes the network settings for the instance type.</p>",
                     "locationName": "networkInfo",
                     "shape": "NetworkInfo"
                 },
+                "NitroEnclavesSupport": {
+                    "documentation": "<p>Indicates whether Nitro Enclaves is supported.</p>",
+                    "locationName": "nitroEnclavesSupport",
+                    "shape": "NitroEnclavesSupport"
+                },
                 "PlacementGroupInfo": {
                     "documentation": "<p>Describes the placement group settings for the instance type.</p>",
                     "locationName": "placementGroupInfo",
                     "shape": "PlacementGroupInfo"
                 },
                 "ProcessorInfo": {
                     "documentation": "<p>Describes the processor.</p>",
@@ -46721,14 +46726,21 @@
                 "shape": "NewDhcpConfiguration"
             },
             "type": "list"
         },
         "NextToken": {
             "type": "string"
         },
+        "NitroEnclavesSupport": {
+            "enum": [
+                "unsupported",
+                "supported"
+            ],
+            "type": "string"
+        },
         "OccurrenceDayRequestSet": {
             "member": {
                 "locationName": "OccurenceDay",
                 "shape": "Integer"
             },
             "type": "list"
         },
@@ -47626,15 +47638,15 @@
                     "locationName": "tagSet",
                     "shape": "TagList"
                 }
             },
             "type": "structure"
         },
         "PlacementGroupArn": {
-            "pattern": "^arn:aws([a-z-]+)?:ec2:[a-z\\d-]+:\\d{12}:placement-group/([^\\s].+[^\\s]){1,255}$",
+            "pattern": "^arn:aws([a-z-]+)?:ec2:[a-z\\d-]+:\\d{12}:placement-group/^.{1,255}$",
             "type": "string"
         },
         "PlacementGroupId": {
             "type": "string"
         },
         "PlacementGroupIdStringList": {
             "member": {
@@ -52214,19 +52226,19 @@
                 },
                 "ElasticInferenceAccelerators": {
                     "documentation": "<p>An elastic inference accelerator to associate with the instance. Elastic inference accelerators are a resource you can attach to your Amazon EC2 instances to accelerate your Deep Learning (DL) inference workloads.</p> <p>You cannot specify accelerators from different generations in the same request.</p> <note> <p>Starting April 15, 2023, Amazon Web Services will not onboard new customers to Amazon Elastic Inference (EI), and will help current customers migrate their workloads to options that offer better price and performance. After April 15, 2023, new customers will not be able to launch instances with Amazon EI accelerators in Amazon SageMaker, Amazon ECS, or Amazon EC2. However, customers who have used Amazon EI at least once during the past 30-day period are considered current customers and will be able to continue using the service.</p> </note>",
                     "locationName": "ElasticInferenceAccelerator",
                     "shape": "ElasticInferenceAccelerators"
                 },
                 "EnclaveOptions": {
-                    "documentation": "<p>Indicates whether the instance is enabled for Amazon Web Services Nitro Enclaves. For more information, see <a href=\"https://docs.aws.amazon.com/enclaves/latest/user/nitro-enclave.html\"> What is Amazon Web Services Nitro Enclaves?</a> in the <i>Amazon Web Services Nitro Enclaves User Guide</i>.</p> <p>You can't enable Amazon Web Services Nitro Enclaves and hibernation on the same instance.</p>",
+                    "documentation": "<p>Indicates whether the instance is enabled for Amazon Web Services Nitro Enclaves. For more information, see <a href=\"https://docs.aws.amazon.com/enclaves/latest/user/nitro-enclave.html\">What is Amazon Web Services Nitro Enclaves?</a> in the <i>Amazon Web Services Nitro Enclaves User Guide</i>.</p> <p>You can't enable Amazon Web Services Nitro Enclaves and hibernation on the same instance.</p>",
                     "shape": "EnclaveOptionsRequest"
                 },
                 "HibernationOptions": {
-                    "documentation": "<p>Indicates whether an instance is enabled for hibernation. For more information, see <a href=\"https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/Hibernate.html\">Hibernate your instance</a> in the <i>Amazon EC2 User Guide</i>.</p> <p>You can't enable hibernation and Amazon Web Services Nitro Enclaves on the same instance.</p>",
+                    "documentation": "<p>Indicates whether an instance is enabled for hibernation. This parameter is valid only if the instance meets the <a href=\"https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/hibernating-prerequisites.html\">hibernation prerequisites</a>. For more information, see <a href=\"https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/Hibernate.html\">Hibernate your instance</a> in the <i>Amazon EC2 User Guide</i>.</p> <p>You can't enable hibernation and Amazon Web Services Nitro Enclaves on the same instance.</p>",
                     "shape": "HibernationOptionsRequest"
                 },
                 "IamInstanceProfile": {
                     "documentation": "<p>The name or Amazon Resource Name (ARN) of an IAM instance profile.</p>",
                     "locationName": "iamInstanceProfile",
                     "shape": "IamInstanceProfileSpecification"
                 },
@@ -56023,15 +56035,15 @@
             "members": {
                 "ClientVpnEndpointId": {
                     "documentation": "<p>The ID of the Client VPN endpoint to which the client is connected.</p>",
                     "shape": "ClientVpnEndpointId"
                 },
                 "ConnectionId": {
                     "documentation": "<p>The ID of the client connection to be terminated.</p>",
-                    "shape": "VpnConnectionId"
+                    "shape": "String"
                 },
                 "DryRun": {
                     "documentation": "<p>Checks whether you have the required permissions for the action, without actually making the request, and provides an error response. If you have the required permissions, the error response is <code>DryRunOperation</code>. Otherwise, it is <code>UnauthorizedOperation</code>.</p>",
                     "shape": "Boolean"
                 },
                 "Username": {
                     "documentation": "<p>The name of the user who initiated the connection. Use this option to terminate all active connections for the specified user. This option can only be used if the user has established up to five connections.</p>",
```

### Comparing `botocore-a-la-carte-ec2-1.30.1/botocore/data/ec2/2016-11-15/waiters-2.json` & `botocore-a-la-carte-ec2-1.31.0/botocore/data/ec2/2016-11-15/waiters-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-ec2-1.30.1/botocore_a_la_carte_ec2.egg-info/PKG-INFO` & `botocore-a-la-carte-ec2-1.31.0/botocore_a_la_carte_ec2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-ec2
-Version: 1.30.1
+Version: 1.31.0
 Summary: ec2 data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-ec2-1.30.1/botocore_a_la_carte_ec2.egg-info/SOURCES.txt` & `botocore-a-la-carte-ec2-1.31.0/botocore_a_la_carte_ec2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-ec2-1.30.1/setup.py` & `botocore-a-la-carte-ec2-1.31.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import setup
 
 setup(
     name='botocore-a-la-carte-ec2',
-    version="1.30.1",
+    version="1.31.0",
     description='ec2 data for botocore. See the `botocore-a-la-carte` package for more info.',
     author='Amazon Web Services',
     url='https://github.com/thejcannon/botocore-a-la-carte',
     scripts=[],
     packages=["botocore"],
     package_data={
         'botocore': ['data/ec2/*/*.json'],
```

