# Comparing `tmp/clarifai-grpc-9.5.0.tar.gz` & `tmp/clarifai-grpc-9.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clarifai-grpc-9.5.0.tar", last modified: Thu Jun  1 20:39:40 2023, max compression
+gzip compressed data, was "clarifai-grpc-9.6.0.tar", last modified: Sat Jul  8 06:39:51 2023, max compression
```

## Comparing `clarifai-grpc-9.5.0.tar` & `clarifai-grpc-9.6.0.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:39:40.296612 clarifai-grpc-9.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-06-01 20:39:26.000000 clarifai-grpc-9.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3940 2023-06-01 20:39:40.296612 clarifai-grpc-9.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3402 2023-06-01 20:39:26.000000 clarifai-grpc-9.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:39:40.292612 clarifai-grpc-9.5.0/clarifai_grpc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 20:39:26.000000 clarifai-grpc-9.5.0/clarifai_grpc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:39:40.292612 clarifai-grpc-9.5.0/clarifai_grpc/channel/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 20:39:26.000000 clarifai-grpc-9.5.0/clarifai_grpc/channel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-06-01 20:39:26.000000 clarifai-grpc-9.5.0/clarifai_grpc/channel/clarifai_channel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:39:40.292612 clarifai-grpc-9.5.0/clarifai_grpc/channel/custom_converters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 20:39:26.000000 clarifai-grpc-9.5.0/clarifai_grpc/channel/custom_converters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-06-01 20:39:26.000000 clarifai-grpc-9.5.0/clarifai_grpc/channel/custom_converters/custom_dict_to_message.py
--rw-r--r--   0 runner    (1001) docker     (123)     3601 2023-06-01 20:39:26.000000 clarifai-grpc-9.5.0/clarifai_grpc/channel/custom_converters/custom_message_to_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-01 20:39:26.000000 clarifai-grpc-9.5.0/clarifai_grpc/channel/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-01 20:39:26.000000 clarifai-grpc-9.5.0/clarifai_grpc/channel/exceptions.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    12533 2023-06-01 20:39:26.000000 clarifai-grpc-9.5.0/clarifai_grpc/channel/grpc_json_channel.py
--rw-r--r--   0 runner    (1001) docker     (123)     5530 2023-06-01 20:39:26.000000 clarifai-grpc-9.5.0/clarifai_grpc/channel/http_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:39:40.292612 clarifai-grpc-9.5.0/clarifai_grpc/grpc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 20:39:26.000000 clarifai-grpc-9.5.0/clarifai_grpc/grpc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:39:40.292612 clarifai-grpc-9.5.0/clarifai_grpc/grpc/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 20:39:26.000000 clarifai-grpc-9.5.0/clarifai_grpc/grpc/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    97700 2023-06-01 20:39:26.000000 clarifai-grpc-9.5.0/clarifai_grpc/grpc/api/resources_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)   381233 2023-06-01 20:39:26.000000 clarifai-grpc-9.5.0/clarifai_grpc/grpc/api/resources_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-01 20:39:26.000000 clarifai-grpc-9.5.0/clarifai_grpc/grpc/api/resources_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)   234025 2023-06-01 20:39:26.000000 clarifai-grpc-9.5.0/clarifai_grpc/grpc/api/service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)   384781 2023-06-01 20:39:26.000000 clarifai-grpc-9.5.0/clarifai_grpc/grpc/api/service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)   371517 2023-06-01 20:39:26.000000 clarifai-grpc-9.5.0/clarifai_grpc/grpc/api/service_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:39:40.296612 clarifai-grpc-9.5.0/clarifai_grpc/grpc/api/status/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 20:39:26.000000 clarifai-grpc-9.5.0/clarifai_grpc/grpc/api/status/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20688 2023-06-01 20:39:26.000000 clarifai-grpc-9.5.0/clarifai_grpc/grpc/api/status/status_code_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    52203 2023-06-01 20:39:26.000000 clarifai-grpc-9.5.0/clarifai_grpc/grpc/api/status/status_code_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-01 20:39:26.000000 clarifai-grpc-9.5.0/clarifai_grpc/grpc/api/status/status_code_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2978 2023-06-01 20:39:26.000000 clarifai-grpc-9.5.0/clarifai_grpc/grpc/api/status/status_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4791 2023-06-01 20:39:26.000000 clarifai-grpc-9.5.0/clarifai_grpc/grpc/api/status/status_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-01 20:39:26.000000 clarifai-grpc-9.5.0/clarifai_grpc/grpc/api/status/status_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:39:40.296612 clarifai-grpc-9.5.0/clarifai_grpc/grpc/api/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 20:39:26.000000 clarifai-grpc-9.5.0/clarifai_grpc/grpc/api/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-06-01 20:39:26.000000 clarifai-grpc-9.5.0/clarifai_grpc/grpc/api/utils/extensions_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-06-01 20:39:26.000000 clarifai-grpc-9.5.0/clarifai_grpc/grpc/api/utils/extensions_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-01 20:39:26.000000 clarifai-grpc-9.5.0/clarifai_grpc/grpc/api/utils/extensions_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-06-01 20:39:26.000000 clarifai-grpc-9.5.0/clarifai_grpc/grpc/api/utils/matrix_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-06-01 20:39:26.000000 clarifai-grpc-9.5.0/clarifai_grpc/grpc/api/utils/matrix_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-01 20:39:26.000000 clarifai-grpc-9.5.0/clarifai_grpc/grpc/api/utils/matrix_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2362 2023-06-01 20:39:26.000000 clarifai-grpc-9.5.0/clarifai_grpc/grpc/api/utils/test_proto_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2573 2023-06-01 20:39:26.000000 clarifai-grpc-9.5.0/clarifai_grpc/grpc/api/utils/test_proto_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-01 20:39:26.000000 clarifai-grpc-9.5.0/clarifai_grpc/grpc/api/utils/test_proto_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:39:40.296612 clarifai-grpc-9.5.0/clarifai_grpc/grpc/auth/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 20:39:26.000000 clarifai-grpc-9.5.0/clarifai_grpc/grpc/auth/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:39:40.296612 clarifai-grpc-9.5.0/clarifai_grpc/grpc/auth/scope/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 20:39:26.000000 clarifai-grpc-9.5.0/clarifai_grpc/grpc/auth/scope/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19845 2023-06-01 20:39:26.000000 clarifai-grpc-9.5.0/clarifai_grpc/grpc/auth/scope/scope_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    17727 2023-06-01 20:39:26.000000 clarifai-grpc-9.5.0/clarifai_grpc/grpc/auth/scope/scope_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-01 20:39:26.000000 clarifai-grpc-9.5.0/clarifai_grpc/grpc/auth/scope/scope_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:39:40.296612 clarifai-grpc-9.5.0/clarifai_grpc/grpc/auth/types/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 20:39:26.000000 clarifai-grpc-9.5.0/clarifai_grpc/grpc/auth/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-06-01 20:39:26.000000 clarifai-grpc-9.5.0/clarifai_grpc/grpc/auth/types/types_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-06-01 20:39:26.000000 clarifai-grpc-9.5.0/clarifai_grpc/grpc/auth/types/types_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-01 20:39:26.000000 clarifai-grpc-9.5.0/clarifai_grpc/grpc/auth/types/types_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:39:40.296612 clarifai-grpc-9.5.0/clarifai_grpc/grpc/auth/util/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 20:39:26.000000 clarifai-grpc-9.5.0/clarifai_grpc/grpc/auth/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2612 2023-06-01 20:39:26.000000 clarifai-grpc-9.5.0/clarifai_grpc/grpc/auth/util/extension_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3232 2023-06-01 20:39:26.000000 clarifai-grpc-9.5.0/clarifai_grpc/grpc/auth/util/extension_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-01 20:39:26.000000 clarifai-grpc-9.5.0/clarifai_grpc/grpc/auth/util/extension_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:39:40.292612 clarifai-grpc-9.5.0/clarifai_grpc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3940 2023-06-01 20:39:40.000000 clarifai-grpc-9.5.0/clarifai_grpc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-06-01 20:39:40.000000 clarifai-grpc-9.5.0/clarifai_grpc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 20:39:40.000000 clarifai-grpc-9.5.0/clarifai_grpc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-01 20:39:40.000000 clarifai-grpc-9.5.0/clarifai_grpc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-01 20:39:40.000000 clarifai-grpc-9.5.0/clarifai_grpc.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 20:39:40.296612 clarifai-grpc-9.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-06-01 20:39:26.000000 clarifai-grpc-9.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 06:39:51.684214 clarifai-grpc-9.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-07-08 06:39:42.000000 clarifai-grpc-9.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3940 2023-07-08 06:39:51.684214 clarifai-grpc-9.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3402 2023-07-08 06:39:42.000000 clarifai-grpc-9.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 06:39:51.676214 clarifai-grpc-9.6.0/clarifai_grpc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 06:39:42.000000 clarifai-grpc-9.6.0/clarifai_grpc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 06:39:51.680214 clarifai-grpc-9.6.0/clarifai_grpc/channel/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 06:39:42.000000 clarifai-grpc-9.6.0/clarifai_grpc/channel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-07-08 06:39:42.000000 clarifai-grpc-9.6.0/clarifai_grpc/channel/clarifai_channel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 06:39:51.680214 clarifai-grpc-9.6.0/clarifai_grpc/channel/custom_converters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 06:39:42.000000 clarifai-grpc-9.6.0/clarifai_grpc/channel/custom_converters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-07-08 06:39:42.000000 clarifai-grpc-9.6.0/clarifai_grpc/channel/custom_converters/custom_dict_to_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3601 2023-07-08 06:39:42.000000 clarifai-grpc-9.6.0/clarifai_grpc/channel/custom_converters/custom_message_to_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-08 06:39:42.000000 clarifai-grpc-9.6.0/clarifai_grpc/channel/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-08 06:39:42.000000 clarifai-grpc-9.6.0/clarifai_grpc/channel/exceptions.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12533 2023-07-08 06:39:42.000000 clarifai-grpc-9.6.0/clarifai_grpc/channel/grpc_json_channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5526 2023-07-08 06:39:42.000000 clarifai-grpc-9.6.0/clarifai_grpc/channel/http_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 06:39:51.680214 clarifai-grpc-9.6.0/clarifai_grpc/grpc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 06:39:42.000000 clarifai-grpc-9.6.0/clarifai_grpc/grpc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 06:39:51.680214 clarifai-grpc-9.6.0/clarifai_grpc/grpc/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 06:39:42.000000 clarifai-grpc-9.6.0/clarifai_grpc/grpc/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    98821 2023-07-08 06:39:42.000000 clarifai-grpc-9.6.0/clarifai_grpc/grpc/api/resources_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)   386723 2023-07-08 06:39:42.000000 clarifai-grpc-9.6.0/clarifai_grpc/grpc/api/resources_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-08 06:39:42.000000 clarifai-grpc-9.6.0/clarifai_grpc/grpc/api/resources_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)   242782 2023-07-08 06:39:42.000000 clarifai-grpc-9.6.0/clarifai_grpc/grpc/api/service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)   391049 2023-07-08 06:39:42.000000 clarifai-grpc-9.6.0/clarifai_grpc/grpc/api/service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)   378749 2023-07-08 06:39:42.000000 clarifai-grpc-9.6.0/clarifai_grpc/grpc/api/service_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 06:39:51.680214 clarifai-grpc-9.6.0/clarifai_grpc/grpc/api/status/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 06:39:42.000000 clarifai-grpc-9.6.0/clarifai_grpc/grpc/api/status/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21161 2023-07-08 06:39:42.000000 clarifai-grpc-9.6.0/clarifai_grpc/grpc/api/status/status_code_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53274 2023-07-08 06:39:42.000000 clarifai-grpc-9.6.0/clarifai_grpc/grpc/api/status/status_code_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-08 06:39:42.000000 clarifai-grpc-9.6.0/clarifai_grpc/grpc/api/status/status_code_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2978 2023-07-08 06:39:42.000000 clarifai-grpc-9.6.0/clarifai_grpc/grpc/api/status/status_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4791 2023-07-08 06:39:42.000000 clarifai-grpc-9.6.0/clarifai_grpc/grpc/api/status/status_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-08 06:39:42.000000 clarifai-grpc-9.6.0/clarifai_grpc/grpc/api/status/status_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 06:39:51.680214 clarifai-grpc-9.6.0/clarifai_grpc/grpc/api/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 06:39:42.000000 clarifai-grpc-9.6.0/clarifai_grpc/grpc/api/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-07-08 06:39:42.000000 clarifai-grpc-9.6.0/clarifai_grpc/grpc/api/utils/extensions_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-07-08 06:39:42.000000 clarifai-grpc-9.6.0/clarifai_grpc/grpc/api/utils/extensions_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-08 06:39:42.000000 clarifai-grpc-9.6.0/clarifai_grpc/grpc/api/utils/extensions_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-07-08 06:39:42.000000 clarifai-grpc-9.6.0/clarifai_grpc/grpc/api/utils/matrix_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-07-08 06:39:42.000000 clarifai-grpc-9.6.0/clarifai_grpc/grpc/api/utils/matrix_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-08 06:39:42.000000 clarifai-grpc-9.6.0/clarifai_grpc/grpc/api/utils/matrix_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2362 2023-07-08 06:39:42.000000 clarifai-grpc-9.6.0/clarifai_grpc/grpc/api/utils/test_proto_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2573 2023-07-08 06:39:42.000000 clarifai-grpc-9.6.0/clarifai_grpc/grpc/api/utils/test_proto_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-08 06:39:42.000000 clarifai-grpc-9.6.0/clarifai_grpc/grpc/api/utils/test_proto_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 06:39:51.680214 clarifai-grpc-9.6.0/clarifai_grpc/grpc/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 06:39:42.000000 clarifai-grpc-9.6.0/clarifai_grpc/grpc/auth/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 06:39:51.684214 clarifai-grpc-9.6.0/clarifai_grpc/grpc/auth/scope/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 06:39:42.000000 clarifai-grpc-9.6.0/clarifai_grpc/grpc/auth/scope/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19845 2023-07-08 06:39:42.000000 clarifai-grpc-9.6.0/clarifai_grpc/grpc/auth/scope/scope_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17727 2023-07-08 06:39:42.000000 clarifai-grpc-9.6.0/clarifai_grpc/grpc/auth/scope/scope_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-08 06:39:42.000000 clarifai-grpc-9.6.0/clarifai_grpc/grpc/auth/scope/scope_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 06:39:51.684214 clarifai-grpc-9.6.0/clarifai_grpc/grpc/auth/types/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 06:39:42.000000 clarifai-grpc-9.6.0/clarifai_grpc/grpc/auth/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-07-08 06:39:42.000000 clarifai-grpc-9.6.0/clarifai_grpc/grpc/auth/types/types_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-07-08 06:39:42.000000 clarifai-grpc-9.6.0/clarifai_grpc/grpc/auth/types/types_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-08 06:39:42.000000 clarifai-grpc-9.6.0/clarifai_grpc/grpc/auth/types/types_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 06:39:51.684214 clarifai-grpc-9.6.0/clarifai_grpc/grpc/auth/util/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 06:39:42.000000 clarifai-grpc-9.6.0/clarifai_grpc/grpc/auth/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2612 2023-07-08 06:39:42.000000 clarifai-grpc-9.6.0/clarifai_grpc/grpc/auth/util/extension_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3232 2023-07-08 06:39:42.000000 clarifai-grpc-9.6.0/clarifai_grpc/grpc/auth/util/extension_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-08 06:39:42.000000 clarifai-grpc-9.6.0/clarifai_grpc/grpc/auth/util/extension_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 06:39:51.676214 clarifai-grpc-9.6.0/clarifai_grpc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3940 2023-07-08 06:39:51.000000 clarifai-grpc-9.6.0/clarifai_grpc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-07-08 06:39:51.000000 clarifai-grpc-9.6.0/clarifai_grpc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 06:39:51.000000 clarifai-grpc-9.6.0/clarifai_grpc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-08 06:39:51.000000 clarifai-grpc-9.6.0/clarifai_grpc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-08 06:39:51.000000 clarifai-grpc-9.6.0/clarifai_grpc.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 06:39:51.684214 clarifai-grpc-9.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-07-08 06:39:42.000000 clarifai-grpc-9.6.0/setup.py
```

### Comparing `clarifai-grpc-9.5.0/LICENSE` & `clarifai-grpc-9.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `clarifai-grpc-9.5.0/PKG-INFO` & `clarifai-grpc-9.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clarifai-grpc
-Version: 9.5.0
+Version: 9.6.0
 Summary: Clarifai gRPC API Client
 Home-page: https://github.com/Clarifai/clarifai-python-grpc
 Author: Clarifai
 Author-email: support@clarifai.com
 License: Apache 2.0
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Programming Language :: Python :: 3
```

### Comparing `clarifai-grpc-9.5.0/README.md` & `clarifai-grpc-9.6.0/README.md`

 * *Files identical despite different names*

### Comparing `clarifai-grpc-9.5.0/clarifai_grpc/channel/clarifai_channel.py` & `clarifai-grpc-9.6.0/clarifai_grpc/channel/clarifai_channel.py`

 * *Files identical despite different names*

### Comparing `clarifai-grpc-9.5.0/clarifai_grpc/channel/custom_converters/custom_dict_to_message.py` & `clarifai-grpc-9.6.0/clarifai_grpc/channel/custom_converters/custom_dict_to_message.py`

 * *Files identical despite different names*

### Comparing `clarifai-grpc-9.5.0/clarifai_grpc/channel/custom_converters/custom_message_to_dict.py` & `clarifai-grpc-9.6.0/clarifai_grpc/channel/custom_converters/custom_message_to_dict.py`

 * *Files identical despite different names*

### Comparing `clarifai-grpc-9.5.0/clarifai_grpc/channel/grpc_json_channel.py` & `clarifai-grpc-9.6.0/clarifai_grpc/channel/grpc_json_channel.py`

 * *Files identical despite different names*

### Comparing `clarifai-grpc-9.5.0/clarifai_grpc/channel/http_client.py` & `clarifai-grpc-9.6.0/clarifai_grpc/channel/http_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import os
 import typing  # noqa
 
 import requests
 
 from clarifai_grpc.channel.errors import ApiError
 
-CLIENT_VERSION = "6.8.1"
+CLIENT_VERSION = "9.6.0"
 OS_VER = os.sys.platform
 PYTHON_VERSION = ".".join(
     map(
         str,
         [
             os.sys.version_info.major,
             os.sys.version_info.minor,
@@ -121,23 +121,23 @@
             return original_base64
 
     def _encode_get_params(self, params):
         """
         Encodes message params into format for use in GET args
         """
         encoded_params = {}
-        for (k, v) in params.items():
+        for k, v in params.items():
             if isinstance(v, str):
                 encoded_params[k] = v
             elif isinstance(v, bytes):
                 encoded_params[k] = v.decode("utf-8")
             elif isinstance(v, (int, float, bool)):
                 encoded_params[k] = str(v)
             elif isinstance(v, dict):
-                for (subk, subv) in self._encode_get_params(v).items():
+                for subk, subv in self._encode_get_params(v).items():
                     encoded_params[k + "." + subk] = subv
             elif isinstance(v, list):
                 if v:
                     encoded_params[k] = v
             else:
                 raise TypeError("Cannot convert type for get params: %s" % type(v))
         return encoded_params
```

### Comparing `clarifai-grpc-9.5.0/clarifai_grpc/grpc/api/resources_pb2.py` & `clarifai-grpc-9.6.0/clarifai_grpc/grpc/api/resources_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 from clarifai_grpc.grpc.api.utils import matrix_pb2 as proto_dot_clarifai_dot_api_dot_utils_dot_matrix__pb2
 from clarifai_grpc.grpc.auth.util import extension_pb2 as proto_dot_clarifai_dot_auth_dot_util_dot_extension__pb2
 from google.protobuf import struct_pb2 as google_dot_protobuf_dot_struct__pb2
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 from google.protobuf import wrappers_pb2 as google_dot_protobuf_dot_wrappers__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\"proto/clarifai/api/resources.proto\x12\x0c\x63larifai.api\x1a&proto/clarifai/api/status/status.proto\x1a+proto/clarifai/api/status/status_code.proto\x1a)proto/clarifai/api/utils/extensions.proto\x1a%proto/clarifai/api/utils/matrix.proto\x1a(proto/clarifai/auth/util/extension.proto\x1a\x1cgoogle/protobuf/struct.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x1egoogle/protobuf/wrappers.proto\"\xe5\x03\n\nAnnotation\x12\n\n\x02id\x18\x01 \x01(\t\x12\x10\n\x08input_id\x18\x02 \x01(\t\x12 \n\x04\x64\x61ta\x18\x03 \x01(\x0b\x32\x12.clarifai.api.Data\x12\x30\n\x0f\x61nnotation_info\x18\r \x01(\x0b\x32\x17.google.protobuf.Struct\x12\x0f\n\x07user_id\x18\x0f \x01(\t\x12\x18\n\x10model_version_id\x18\x10 \x01(\t\x12\"\n\x16\x65mbed_model_version_id\x18\x0e \x01(\tB\x02\x18\x01\x12+\n\x06status\x18\x07 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12.\n\ncreated_at\x18\x08 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12/\n\x0bmodified_at\x18\t \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x13\n\x07trusted\x18\n \x01(\x08\x42\x02\x18\x01\x12\x13\n\x0binput_level\x18\x11 \x01(\x08\x12/\n\x0e\x63onsensus_info\x18\x12 \x01(\x0b\x32\x17.google.protobuf.Struct\x12\x0f\n\x07task_id\x18\x13 \x01(\tJ\x04\x08\x04\x10\x05J\x04\x08\x05\x10\x06J\x04\x08\x06\x10\x07J\x04\x08\x0b\x10\x0cJ\x04\x08\x0c\x10\r\"\x9c\x04\n\x03\x41pp\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x18\n\x10\x64\x65\x66\x61ult_language\x18\x03 \x01(\t\x12\x1b\n\x13\x64\x65\x66\x61ult_workflow_id\x18\x04 \x01(\t\x12\x30\n\x10\x64\x65\x66\x61ult_workflow\x18\x17 \x01(\x0b\x32\x16.clarifai.api.Workflow\x12\x0f\n\x07user_id\x18\x05 \x01(\t\x12.\n\ncreated_at\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12/\n\x0bmodified_at\x18\x11 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x1c\n\x14legal_consent_status\x18\x07 \x01(\r\x12)\n\x08metadata\x18\r \x01(\x0b\x32\x17.google.protobuf.Struct\x12\x13\n\x0b\x64\x65scription\x18\x0e \x01(\t\x12\x11\n\tsample_ms\x18\x0f \x01(\r\x12,\n\nvisibility\x18\x10 \x01(\x0b\x32\x18.clarifai.api.Visibility\x12\x14\n\x0c\x64\x61ta_tier_id\x18\x12 \x01(\t\x12\x12\n\nis_starred\x18\x13 \x01(\x08\x12\x12\n\nstar_count\x18\x14 \x01(\x05\x12\r\n\x05notes\x18\x15 \x01(\t\x12\"\n\x05image\x18\x16 \x01(\x0b\x32\x13.clarifai.api.ImageJ\x04\x08\n\x10\x0bJ\x04\x08\x0b\x10\x0cJ\x04\x08\x0c\x10\r\"\x18\n\x08\x41ppQuery\x12\x0c\n\x04name\x18\x01 \x01(\t\"\x90\x02\n\x0c\x43ollaborator\x12\n\n\x02id\x18\x01 \x01(\t\x12\x1e\n\x03\x61pp\x18\x02 \x01(\x0b\x32\x11.clarifai.api.App\x12 \n\x04user\x18\x03 \x01(\x0b\x32\x12.clarifai.api.User\x12\x0e\n\x06scopes\x18\x04 \x03(\t\x12\x11\n\tendpoints\x18\x05 \x03(\t\x12.\n\ncreated_at\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12/\n\x0bmodified_at\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12.\n\ndeleted_at\x18\x08 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"\xa9\x01\n\rCollaboration\x12\x1e\n\x03\x61pp\x18\x01 \x01(\x0b\x32\x11.clarifai.api.App\x12%\n\tapp_owner\x18\x02 \x01(\x0b\x32\x12.clarifai.api.User\x12\x0e\n\x06scopes\x18\x03 \x03(\t\x12\x11\n\tendpoints\x18\x04 \x03(\t\x12.\n\ncreated_at\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"\x97\x01\n\x05\x41udio\x12\x0b\n\x03url\x18\x01 \x01(\t\x12\x0e\n\x06\x62\x61se64\x18\x02 \x01(\x0c\x12\x1b\n\x13\x61llow_duplicate_url\x18\x04 \x01(\x08\x12\'\n\x06hosted\x18\x05 \x01(\x0b\x32\x17.clarifai.api.HostedURL\x12+\n\naudio_info\x18\x06 \x01(\x0b\x32\x17.clarifai.api.AudioInfo\"b\n\tAudioInfo\x12\x14\n\x0c\x61udio_format\x18\x01 \x01(\t\x12\x13\n\x0bsample_rate\x18\x02 \x01(\x05\x12\x18\n\x10\x64uration_seconds\x18\x03 \x01(\x02\x12\x10\n\x08\x62it_rate\x18\x04 \x01(\x05\"w\n\x05Track\x12\n\n\x02id\x18\x01 \x01(\t\x12 \n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x12.clarifai.api.Data\x12)\n\ttime_info\x18\x04 \x01(\x0b\x32\x16.clarifai.api.TimeInfo\x12\x0f\n\x07quality\x18\x05 \x01(\x02J\x04\x08\x03\x10\x04\"h\n\x07\x43luster\x12\n\n\x02id\x18\x01 \x01(\t\x12\r\n\x05\x63ount\x18\x02 \x01(\r\x12\r\n\x05score\x18\x03 \x01(\x02\x12\x1f\n\x04hits\x18\x04 \x03(\x0b\x32\x11.clarifai.api.Hit\x12\x12\n\nprojection\x18\x05 \x03(\x02\"M\n\x05\x43olor\x12\x0f\n\x07raw_hex\x18\x01 \x01(\t\x12\x1e\n\x03w3c\x18\x02 \x01(\x0b\x32\x11.clarifai.api.W3C\x12\x13\n\x05value\x18\x03 \x01(\x02\x42\x04\x80\xb5\x18\x01\" \n\x03W3C\x12\x0b\n\x03hex\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\"/\n\x0cUserAppIDSet\x12\x0f\n\x07user_id\x18\x01 \x01(\t\x12\x0e\n\x06\x61pp_id\x18\x02 \x01(\t\"J\n\x0bPatchAction\x12\n\n\x02op\x18\x01 \x01(\t\x12!\n\x19merge_conflict_resolution\x18\x02 \x01(\t\x12\x0c\n\x04path\x18\x03 \x01(\t\"\xa9\x02\n\x07\x43oncept\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x1a\n\x05value\x18\x03 \x01(\x02\x42\x0b\xd5\xb5\x18\x00\x00\x80?\x80\xb5\x18\x01\x12.\n\ncreated_at\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x10\n\x08language\x18\x05 \x01(\t\x12\x0e\n\x06\x61pp_id\x18\x06 \x01(\t\x12\x12\n\ndefinition\x18\x07 \x01(\t\x12\x10\n\x08vocab_id\x18\x08 \x01(\t\x12,\n\nvisibility\x18\t \x01(\x0b\x32\x18.clarifai.api.Visibility\x12\x0f\n\x07user_id\x18\n \x01(\t\x12\x31\n\rkeypoint_info\x18\x0b \x01(\x0b\x32\x1a.clarifai.api.KeypointInfo\"T\n\x0cKeypointInfo\x12\x16\n\x0ekeypoint_names\x18\x01 \x03(\t\x12,\n\x08skeleton\x18\x02 \x03(\x0b\x32\x1a.clarifai.api.KeypointEdge\"&\n\x0cKeypointEdge\x12\n\n\x02k1\x18\x01 \x01(\r\x12\n\n\x02k2\x18\x02 \x01(\r\"\xa4\x01\n\x0c\x43onceptCount\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12:\n\x12\x63oncept_type_count\x18\x03 \x01(\x0b\x32\x1e.clarifai.api.ConceptTypeCount\x12>\n\x14\x64\x65tail_concept_count\x18\x04 \x01(\x0b\x32 .clarifai.api.DetailConceptCount\"B\n\x10\x43onceptTypeCount\x12\x16\n\x08positive\x18\x01 \x01(\rB\x04\x80\xb5\x18\x01\x12\x16\n\x08negative\x18\x02 \x01(\rB\x04\x80\xb5\x18\x01\"\xdf\x01\n\x12\x44\x65tailConceptCount\x12\x31\n\tprocessed\x18\x01 \x01(\x0b\x32\x1e.clarifai.api.ConceptTypeCount\x12\x32\n\nto_process\x18\x02 \x01(\x0b\x32\x1e.clarifai.api.ConceptTypeCount\x12.\n\x06\x65rrors\x18\x03 \x01(\x0b\x32\x1e.clarifai.api.ConceptTypeCount\x12\x32\n\nprocessing\x18\x04 \x01(\x0b\x32\x1e.clarifai.api.ConceptTypeCount\"C\n\x0c\x43onceptQuery\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x10\n\x08language\x18\x02 \x01(\t\x12\x13\n\x0bworkflow_id\x18\x03 \x01(\t\"\xd9\x01\n\x0f\x43onceptRelation\x12\n\n\x02id\x18\x01 \x01(\t\x12.\n\x0fsubject_concept\x18\x02 \x01(\x0b\x32\x15.clarifai.api.Concept\x12-\n\x0eobject_concept\x18\x03 \x01(\x0b\x32\x15.clarifai.api.Concept\x12\x11\n\tpredicate\x18\x04 \x01(\t\x12\x1a\n\x12knowledge_graph_id\x18\x05 \x01(\t\x12,\n\nvisibility\x18\x06 \x01(\x0b\x32\x18.clarifai.api.Visibility\"y\n\x0eKnowledgeGraph\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x03 \x01(\t\x12\x17\n\x0f\x65xamples_app_id\x18\x04 \x01(\t\x12\x1f\n\x17sampled_examples_app_id\x18\x05 \x01(\t\"D\n\x11\x43onceptMappingJob\x12\x1a\n\x12knowledge_graph_id\x18\x01 \x01(\t\x12\x13\n\x0b\x63oncept_ids\x18\x02 \x03(\t\"?\n\x0f\x43onceptLanguage\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x12\n\ndefinition\x18\x03 \x01(\t\"\xfa\x04\n\x04\x44\x61ta\x12\"\n\x05image\x18\x01 \x01(\x0b\x32\x13.clarifai.api.Image\x12\"\n\x05video\x18\x02 \x01(\x0b\x32\x13.clarifai.api.Video\x12\'\n\x08\x63oncepts\x18\x03 \x03(\x0b\x32\x15.clarifai.api.Concept\x12)\n\x08metadata\x18\x05 \x01(\x0b\x32\x17.google.protobuf.Struct\x12\x1e\n\x03geo\x18\x06 \x01(\x0b\x32\x11.clarifai.api.Geo\x12#\n\x06\x63olors\x18\x07 \x03(\x0b\x32\x13.clarifai.api.Color\x12\'\n\x08\x63lusters\x18\x08 \x03(\x0b\x32\x15.clarifai.api.Cluster\x12+\n\nembeddings\x18\t \x03(\x0b\x32\x17.clarifai.api.Embedding\x12%\n\x07regions\x18\x0b \x03(\x0b\x32\x14.clarifai.api.Region\x12#\n\x06\x66rames\x18\x0c \x03(\x0b\x32\x13.clarifai.api.Frame\x12 \n\x04text\x18\r \x01(\x0b\x32\x12.clarifai.api.Text\x12\"\n\x05\x61udio\x18\x0e \x01(\x0b\x32\x13.clarifai.api.Audio\x12#\n\x06tracks\x18\x0f \x03(\x0b\x32\x13.clarifai.api.Track\x12\x30\n\rtime_segments\x18\x10 \x03(\x0b\x32\x19.clarifai.api.TimeSegment\x12\x1f\n\x04hits\x18\x11 \x03(\x0b\x32\x11.clarifai.api.Hit\x12%\n\x08heatmaps\x18\x12 \x03(\x0b\x32\x13.clarifai.api.ImageJ\x04\x08\x04\x10\x05J\x04\x08\n\x10\x0b\"\x86\x01\n\x06Region\x12\n\n\x02id\x18\x01 \x01(\t\x12-\n\x0bregion_info\x18\x02 \x01(\x0b\x32\x18.clarifai.api.RegionInfo\x12 \n\x04\x64\x61ta\x18\x03 \x01(\x0b\x32\x12.clarifai.api.Data\x12\r\n\x05value\x18\x04 \x01(\x02\x12\x10\n\x08track_id\x18\x05 \x01(\t\"\xae\x02\n\nRegionInfo\x12/\n\x0c\x62ounding_box\x18\x01 \x01(\x0b\x32\x19.clarifai.api.BoundingBox\x12 \n\x04mask\x18\x04 \x01(\x0b\x32\x12.clarifai.api.Mask\x12&\n\x07polygon\x18\x05 \x01(\x0b\x32\x15.clarifai.api.Polygon\x12\"\n\x05point\x18\x06 \x01(\x0b\x32\x13.clarifai.api.Point\x12 \n\x04span\x18\x07 \x01(\x0b\x32\x12.clarifai.api.Span\x12\"\n\x05token\x18\x08 \x01(\x0b\x32\x13.clarifai.api.Token\x12/\n\x12keypoint_locations\x18\t \x03(\x0b\x32\x13.clarifai.api.PointJ\x04\x08\x02\x10\x03J\x04\x08\x03\x10\x04\"o\n\x0b\x42oundingBox\x12\x15\n\x07top_row\x18\x01 \x01(\x02\x42\x04\x80\xb5\x18\x01\x12\x16\n\x08left_col\x18\x02 \x01(\x02\x42\x04\x80\xb5\x18\x01\x12\x18\n\nbottom_row\x18\x03 \x01(\x02\x42\x04\x80\xb5\x18\x01\x12\x17\n\tright_col\x18\x04 \x01(\x02\x42\x04\x80\xb5\x18\x01\"4\n\tFrameInfo\x12\x13\n\x05index\x18\x01 \x01(\rB\x04\x80\xb5\x18\x01\x12\x12\n\x04time\x18\x02 \x01(\rB\x04\x80\xb5\x18\x01\"b\n\x05\x46rame\x12+\n\nframe_info\x18\x01 \x01(\x0b\x32\x17.clarifai.api.FrameInfo\x12 \n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x12.clarifai.api.Data\x12\n\n\x02id\x18\x03 \x01(\t\"0\n\x04Mask\x12\"\n\x05image\x18\x02 \x01(\x0b\x32\x13.clarifai.api.ImageJ\x04\x08\x01\x10\x02\".\n\x07Polygon\x12#\n\x06points\x18\x01 \x03(\x0b\x32\x13.clarifai.api.Point\"\xb6\x01\n\x05Point\x12\x11\n\x03row\x18\x01 \x01(\x02\x42\x04\x80\xb5\x18\x01\x12\x11\n\x03\x63ol\x18\x02 \x01(\x02\x42\x04\x80\xb5\x18\x01\x12\t\n\x01z\x18\x03 \x01(\x02\x12\x32\n\nvisibility\x18\x04 \x01(\x0e\x32\x1e.clarifai.api.Point.Visibility\"H\n\nVisibility\x12\x0b\n\x07NOT_SET\x10\x00\x12\x0b\n\x07VISIBLE\x10\x01\x12\x0f\n\x0bNOT_VISIBLE\x10\x02\x12\x0f\n\x0bNOT_PRESENT\x10\x03\"J\n\x04Span\x12\x18\n\nchar_start\x18\x01 \x01(\rB\x04\x80\xb5\x18\x01\x12\x16\n\x08\x63har_end\x18\x02 \x01(\rB\x04\x80\xb5\x18\x01\x12\x10\n\x08raw_text\x18\x03 \x01(\t\"K\n\x05Token\x12\x18\n\nchar_start\x18\x01 \x01(\rB\x04\x80\xb5\x18\x01\x12\x16\n\x08\x63har_end\x18\x02 \x01(\rB\x04\x80\xb5\x18\x01\x12\x10\n\x08raw_text\x18\x03 \x01(\t\"7\n\tEmbedding\x12\x12\n\x06vector\x18\x01 \x03(\x02\x42\x02\x10\x01\x12\x16\n\x0enum_dimensions\x18\x02 \x01(\r\";\n\x08GeoPoint\x12\x17\n\tlongitude\x18\x01 \x01(\x02\x42\x04\x80\xb5\x18\x01\x12\x16\n\x08latitude\x18\x02 \x01(\x02\x42\x04\x80\xb5\x18\x01\"-\n\x08GeoLimit\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x13\n\x05value\x18\x02 \x01(\x02\x42\x04\x80\xb5\x18\x01\":\n\rGeoBoxedPoint\x12)\n\tgeo_point\x18\x01 \x01(\x0b\x32\x16.clarifai.api.GeoPoint\"\x89\x01\n\x03Geo\x12)\n\tgeo_point\x18\x01 \x01(\x0b\x32\x16.clarifai.api.GeoPoint\x12)\n\tgeo_limit\x18\x02 \x01(\x0b\x32\x16.clarifai.api.GeoLimit\x12,\n\x07geo_box\x18\x03 \x03(\x0b\x32\x1b.clarifai.api.GeoBoxedPoint\"\x9d\x01\n\x05Image\x12\x0b\n\x03url\x18\x01 \x01(\t\x12\x0e\n\x06\x62\x61se64\x18\x02 \x01(\x0c\x12\x1b\n\x13\x61llow_duplicate_url\x18\x04 \x01(\x08\x12\'\n\x06hosted\x18\x05 \x01(\x0b\x32\x17.clarifai.api.HostedURL\x12+\n\nimage_info\x18\x06 \x01(\x0b\x32\x17.clarifai.api.ImageInfoJ\x04\x08\x03\x10\x04\"N\n\tImageInfo\x12\r\n\x05width\x18\x01 \x01(\x05\x12\x0e\n\x06height\x18\x02 \x01(\x05\x12\x0e\n\x06\x66ormat\x18\x03 \x01(\t\x12\x12\n\ncolor_mode\x18\x04 \x01(\t\"O\n\tHostedURL\x12\x0e\n\x06prefix\x18\x01 \x01(\t\x12\x0e\n\x06suffix\x18\x02 \x01(\t\x12\r\n\x05sizes\x18\x03 \x03(\t\x12\x13\n\x0b\x63rossorigin\x18\x04 \x01(\t\"\xde\x01\n\x05Input\x12\n\n\x02id\x18\x01 \x01(\t\x12 \n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x12.clarifai.api.Data\x12.\n\ncreated_at\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12/\n\x0bmodified_at\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12+\n\x06status\x18\x06 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x13\n\x0b\x64\x61taset_ids\x18\x07 \x03(\tJ\x04\x08\x03\x10\x04\"1\n\nInputBatch\x12#\n\x06inputs\x18\x01 \x03(\x0b\x32\x13.clarifai.api.Input\"\xda\x01\n\nInputCount\x12\x17\n\tprocessed\x18\x01 \x01(\rB\x04\x80\xb5\x18\x01\x12\x18\n\nto_process\x18\x02 \x01(\rB\x04\x80\xb5\x18\x01\x12\x14\n\x06\x65rrors\x18\x03 \x01(\rB\x04\x80\xb5\x18\x01\x12\x18\n\nprocessing\x18\x04 \x01(\rB\x04\x80\xb5\x18\x01\x12\x17\n\treindexed\x18\x05 \x01(\rB\x04\x80\xb5\x18\x01\x12\x18\n\nto_reindex\x18\x06 \x01(\rB\x04\x80\xb5\x18\x01\x12\x1c\n\x0ereindex_errors\x18\x07 \x01(\rB\x04\x80\xb5\x18\x01\x12\x18\n\nreindexing\x18\x08 \x01(\rB\x04\x80\xb5\x18\x01\"\xba\x03\n\x07\x44\x61taset\x12\n\n\x02id\x18\x01 \x01(\t\x12.\n\ncreated_at\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12/\n\x0bmodified_at\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x0e\n\x06\x61pp_id\x18\x04 \x01(\t\x12\x0f\n\x07user_id\x18\x05 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x07 \x01(\t\x12)\n\x08metadata\x18\x08 \x01(\x0b\x32\x17.google.protobuf.Struct\x12,\n\nvisibility\x18\t \x01(\x0b\x32\x18.clarifai.api.Visibility\x12\x41\n\x19\x64\x65\x66\x61ult_annotation_filter\x18\x0c \x01(\x0b\x32\x1e.clarifai.api.AnnotationFilter\x12\r\n\x05notes\x18\x0b \x01(\t\x12-\n\x07version\x18\r \x01(\x0b\x32\x1c.clarifai.api.DatasetVersion\x12\x12\n\nis_starred\x18\x0e \x01(\x08\x12\x12\n\nstar_count\x18\x0f \x01(\x05J\x04\x08\x06\x10\x07J\x04\x08\n\x10\x0b\"\xd8\x01\n\x10\x41nnotationFilter\x12\n\n\x02id\x18\x01 \x01(\t\x12.\n\ncreated_at\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12/\n\x0bmodified_at\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x0f\n\x07user_id\x18\x04 \x01(\t\x12\x0e\n\x06\x61pp_id\x18\x05 \x01(\t\x12*\n\x0csaved_search\x18\x08 \x01(\x0b\x32\x14.clarifai.api.SearchJ\x04\x08\x06\x10\x07J\x04\x08\x07\x10\x08\"b\n\x0c\x44\x61tasetInput\x12.\n\ncreated_at\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\"\n\x05input\x18\x02 \x01(\x0b\x32\x13.clarifai.api.Input\"\xe9\x05\n\x0e\x44\x61tasetVersion\x12\n\n\x02id\x18\x01 \x01(\t\x12.\n\ncreated_at\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12/\n\x0bmodified_at\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x0e\n\x06\x61pp_id\x18\x04 \x01(\t\x12\x0f\n\x07user_id\x18\x05 \x01(\t\x12\x12\n\ndataset_id\x18\x06 \x01(\t\x12H\n\x18\x61nnotation_filter_config\x18\x0f \x01(\x0b\x32$.clarifai.api.AnnotationFilterConfigH\x00\x12@\n\x14model_predict_config\x18\x12 \x01(\x0b\x32 .clarifai.api.ModelPredictConfigH\x00\x12+\n\x06status\x18\x08 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x13\n\x0b\x64\x65scription\x18\n \x01(\t\x12:\n\x07metrics\x18\x10 \x03(\x0b\x32).clarifai.api.DatasetVersion.MetricsEntry\x12;\n\x0b\x65xport_info\x18\x11 \x01(\x0b\x32&.clarifai.api.DatasetVersionExportInfo\x12)\n\x08metadata\x18\x0c \x01(\x0b\x32\x17.google.protobuf.Struct\x12,\n\nvisibility\x18\r \x01(\x0b\x32\x18.clarifai.api.Visibility\x12\x1f\n\x17\x65mbed_model_version_ids\x18\x0e \x03(\t\x1aS\n\x0cMetricsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x32\n\x05value\x18\x02 \x01(\x0b\x32#.clarifai.api.DatasetVersionMetrics:\x02\x38\x01\x42\r\n\x0b\x64\x61ta_configJ\x04\x08\x07\x10\x08J\x04\x08\t\x10\nJ\x04\x08\x0b\x10\x0c\"p\n\x16\x41nnotationFilterConfig\x12\x39\n\x11\x61nnotation_filter\x18\x01 \x01(\x0b\x32\x1e.clarifai.api.AnnotationFilter\x12\x1b\n\x13ignore_empty_inputs\x18\x02 \x01(\x08\"8\n\x12ModelPredictConfig\x12\"\n\x05model\x18\x01 \x01(\x0b\x32\x13.clarifai.api.Model\"\xc3\x08\n\x15\x44\x61tasetVersionMetrics\x12\x32\n\x0cinputs_count\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.UInt64Value\x12<\n\x16unlabeled_inputs_count\x18\x06 \x01(\x0b\x32\x1c.google.protobuf.UInt64Value\x12@\n\x1ainputs_with_metadata_count\x18\x08 \x01(\x0b\x32\x1c.google.protobuf.UInt64Value\x12;\n\x15inputs_with_geo_count\x18\t \x01(\x0b\x32\x1c.google.protobuf.UInt64Value\x12\x33\n\rregions_count\x18\x14 \x01(\x0b\x32\x1c.google.protobuf.UInt64Value\x12-\n\x16region_location_matrix\x18\x15 \x01(\x0b\x32\r.MatrixUint64\x12:\n\x14\x62ounding_boxes_count\x18\x16 \x01(\x0b\x32\x1c.google.protobuf.UInt64Value\x12\x34\n\x0epolygons_count\x18\x17 \x01(\x0b\x32\x1c.google.protobuf.UInt64Value\x12\x32\n\x0cpoints_count\x18\x18 \x01(\x0b\x32\x1c.google.protobuf.UInt64Value\x12\x31\n\x0bmasks_count\x18\x19 \x01(\x0b\x32\x1c.google.protobuf.UInt64Value\x12\x39\n\x13region_inputs_count\x18< \x01(\x0b\x32\x1c.google.protobuf.UInt64Value\x12\x39\n\x13region_frames_count\x18= \x01(\x0b\x32\x1c.google.protobuf.UInt64Value\x12\x32\n\x0c\x66rames_count\x18\x1e \x01(\x0b\x32\x1c.google.protobuf.UInt64Value\x12\x38\n\x12\x66rame_inputs_count\x18\x46 \x01(\x0b\x32\x1c.google.protobuf.UInt64Value\x12\x36\n\x10\x65mbeddings_count\x18( \x01(\x0b\x32\x1c.google.protobuf.UInt64Value\x12?\n\x19positive_input_tags_count\x18\x32 \x01(\x0b\x32\x1c.google.protobuf.UInt64Value\x12@\n\x1apositive_region_tags_count\x18\x33 \x01(\x0b\x32\x1c.google.protobuf.UInt64Value\x12?\n\x19positive_frame_tags_count\x18\x34 \x01(\x0b\x32\x1c.google.protobuf.UInt64ValueJ\x04\x08\x02\x10\x03J\x04\x08\x03\x10\x04J\x04\x08\x04\x10\x05J\x04\x08\x05\x10\x06J\x04\x08\x07\x10\x08\"\xca\x01\n\x1a\x44\x61tasetVersionMetricsGroup\x12\x13\n\x0bparent_path\x18\x01 \x01(\t\x12:\n\x04type\x18\x02 \x01(\x0e\x32,.clarifai.api.DatasetVersionMetricsGroupType\x12%\n\x05value\x18\x03 \x01(\x0b\x32\x16.google.protobuf.Value\x12\x34\n\x07metrics\x18\x04 \x01(\x0b\x32#.clarifai.api.DatasetVersionMetrics\"\xd0\x01\n\x18\x44\x61tasetVersionExportInfo\x12\x42\n\x16\x63larifai_data_protobuf\x18\x01 \x01(\x0b\x32\".clarifai.api.DatasetVersionExport\x12>\n\x12\x63larifai_data_json\x18\x03 \x01(\x0b\x32\".clarifai.api.DatasetVersionExport\x12\x30\n\x04\x63oco\x18\x02 \x01(\x0b\x32\".clarifai.api.DatasetVersionExport\"\xb4\x01\n\x14\x44\x61tasetVersionExport\x12\x38\n\x06\x66ormat\x18\x01 \x01(\x0e\x32(.clarifai.api.DatasetVersionExportFormat\x12+\n\x06status\x18\x02 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x0b\n\x03url\x18\x03 \x01(\t\x12\x0c\n\x04size\x18\x04 \x01(\x04\x12\x1a\n\x12include_embeddings\x18\x05 \x01(\x08\"n\n\x19WorkflowResultsSimilarity\x12(\n\x0bprobe_input\x18\x01 \x01(\x0b\x32\x13.clarifai.api.Input\x12\'\n\x0cpool_results\x18\x02 \x03(\x0b\x32\x11.clarifai.api.Hit\"\xf4\x01\n\x03Key\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x04type\x18\x08 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\x0e\n\x06scopes\x18\x03 \x03(\t\x12\x11\n\tendpoints\x18\x07 \x03(\t\x12\x1f\n\x04\x61pps\x18\x04 \x03(\x0b\x32\x11.clarifai.api.App\x12.\n\ncreated_at\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12.\n\nexpires_at\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x1a\n\x12\x61uthorized_idp_ids\x18\t \x03(\t\"\xd8\x07\n\x05Model\x12\n\n\x02id\x18\x01 \x01(\t\x12\x10\n\x04name\x18\x02 \x01(\tB\x02\x18\x01\x12.\n\ncreated_at\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12/\n\x0bmodified_at\x18\x13 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x14\n\x06\x61pp_id\x18\x04 \x01(\tB\x04\x80\xb5\x18\x01\x12\x31\n\x0boutput_info\x18\x05 \x01(\x0b\x32\x18.clarifai.api.OutputInfoB\x02\x18\x01\x12\x31\n\rmodel_version\x18\x06 \x01(\x0b\x32\x1a.clarifai.api.ModelVersion\x12\x18\n\x0c\x64isplay_name\x18\x07 \x01(\tB\x02\x18\x01\x12\x0f\n\x07user_id\x18\t \x01(\t\x12/\n\ninput_info\x18\x0c \x01(\x0b\x32\x17.clarifai.api.InputInfoB\x02\x18\x01\x12/\n\ntrain_info\x18\r \x01(\x0b\x32\x17.clarifai.api.TrainInfoB\x02\x18\x01\x12\x31\n\x11\x64\x65\x66\x61ult_eval_info\x18\x1e \x01(\x0b\x32\x16.clarifai.api.EvalInfo\x12\x15\n\rmodel_type_id\x18\x0e \x01(\t\x12\x0c\n\x04task\x18\x1a \x01(\t\x12,\n\nvisibility\x18\x0f \x01(\x0b\x32\x18.clarifai.api.Visibility\x12\x13\n\x0b\x64\x65scription\x18\x10 \x01(\t\x12)\n\x08metadata\x18\x11 \x01(\x0b\x32\x17.google.protobuf.Struct\x12(\n\x07presets\x18\x1b \x01(\x0b\x32\x17.google.protobuf.Struct\x12\r\n\x05notes\x18\x12 \x01(\t\x12\x16\n\x08toolkits\x18\x14 \x03(\tB\x04\x80\xb5\x18\x01\x12\x17\n\tuse_cases\x18\x15 \x03(\tB\x04\x80\xb5\x18\x01\x12\x17\n\tlanguages\x18\x19 \x03(\tB\x04\x80\xb5\x18\x01\x12\x33\n\x0elanguages_full\x18\x1f \x03(\x0b\x32\x15.clarifai.api.FullTagB\x04\x80\xb5\x18\x01\x12\x1c\n\x0e\x63heck_consents\x18  \x03(\tB\x04\x80\xb5\x18\x01\x12\x12\n\nis_starred\x18\x16 \x01(\x08\x12\x12\n\nstar_count\x18\x17 \x01(\x05\x12\x31\n\x0bimport_info\x18\x18 \x01(\x0b\x32\x18.clarifai.api.ImportInfoB\x02\x18\x01\x12\x38\n\x14workflow_recommended\x18\x1d \x01(\x0b\x32\x1a.google.protobuf.BoolValueJ\x04\x08\x08\x10\tJ\x04\x08\n\x10\x0bJ\x04\x08\x0b\x10\x0cJ\x04\x08\x1c\x10\x1d\"t\n\x0eModelReference\x12\n\n\x02id\x18\x01 \x01(\t\x12\x10\n\x08model_id\x18\x02 \x01(\t\x12\x0b\n\x03url\x18\x03 \x01(\t\x12\x0c\n\x04name\x18\x04 \x01(\t\x12)\n\x08metadata\x18\x05 \x01(\x0b\x32\x17.google.protobuf.Struct\"\x97\x01\n\x18ModelVersionInputExample\x12\n\n\x02id\x18\x01 \x01(\t\x12\x10\n\x08model_id\x18\x02 \x01(\t\x12\x18\n\x10model_version_id\x18\x03 \x01(\t\x12 \n\x04\x64\x61ta\x18\x04 \x01(\x0b\x32\x12.clarifai.api.Data\x12\x0c\n\x04name\x18\x05 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x06 \x01(\t\"\xd4\x01\n\nOutputInfo\x12 \n\x04\x64\x61ta\x18\x01 \x01(\x0b\x32\x12.clarifai.api.Data\x12\x31\n\routput_config\x18\x02 \x01(\x0b\x32\x1a.clarifai.api.OutputConfig\x12\x0f\n\x07message\x18\x03 \x01(\t\x12+\n\nfields_map\x18\x06 \x01(\x0b\x32\x17.google.protobuf.Struct\x12\'\n\x06params\x18\x07 \x01(\x0b\x32\x17.google.protobuf.StructJ\x04\x08\x04\x10\x05J\x04\x08\x05\x10\x06\"a\n\tInputInfo\x12+\n\nfields_map\x18\x01 \x01(\x0b\x32\x17.google.protobuf.Struct\x12\'\n\x06params\x18\x02 \x01(\x0b\x32\x17.google.protobuf.Struct\"4\n\tTrainInfo\x12\'\n\x06params\x18\x01 \x01(\x0b\x32\x17.google.protobuf.Struct\"3\n\x08\x45valInfo\x12\'\n\x06params\x18\x01 \x01(\x0b\x32\x17.google.protobuf.Struct\"5\n\nImportInfo\x12\'\n\x06params\x18\x01 \x01(\x0b\x32\x17.google.protobuf.Struct\"\x81\x04\n\x0cOutputConfig\x12\'\n\x1b\x63oncepts_mutually_exclusive\x18\x01 \x01(\x08\x42\x02\x18\x01\x12 \n\x12\x63losed_environment\x18\x02 \x01(\x08\x42\x04\x80\xb5\x18\x01\x12\x1d\n\x11\x65xisting_model_id\x18\x03 \x01(\tB\x02\x18\x01\x12\x10\n\x08language\x18\x04 \x01(\t\x12\x1c\n\x10hyper_parameters\x18\x05 \x01(\tB\x02\x18\x01\x12\x1a\n\x0cmax_concepts\x18\x06 \x01(\rB\x04\x80\xb5\x18\x01\x12\x17\n\tmin_value\x18\x07 \x01(\x02\x42\x04\x80\xb5\x18\x01\x12.\n\x0fselect_concepts\x18\x08 \x03(\x0b\x32\x15.clarifai.api.Concept\x12\x18\n\x10training_timeout\x18\t \x01(\r\x12\x11\n\tsample_ms\x18\n \x01(\r\x12-\n\x0chyper_params\x18\r \x01(\x0b\x32\x17.google.protobuf.Struct\x12\x1e\n\x16\x65mbed_model_version_id\x18\x0e \x01(\t\x12)\n!fail_on_missing_positive_examples\x18\x0f \x01(\x08\x12\x33\n\x0emodel_metadata\x18\x11 \x01(\x0b\x32\x17.google.protobuf.StructB\x02\x18\x01J\x04\x08\x0b\x10\x0cJ\x04\x08\x0c\x10\rJ\x04\x08\x10\x10\x11J\x04\x08\x12\x10\x13\"\xd2\x03\n\tModelType\x12\n\n\x02id\x18\x01 \x01(\t\x12\r\n\x05title\x18\x02 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x03 \x01(\t\x12\x14\n\x0cinput_fields\x18\x05 \x03(\t\x12\x15\n\routput_fields\x18\x06 \x03(\t\x12\x11\n\ttrainable\x18\x08 \x01(\x08\x12\x11\n\tcreatable\x18\t \x01(\x08\x12\x15\n\rinternal_only\x18\n \x01(\x08\x12\x37\n\x11model_type_fields\x18\x0b \x03(\x0b\x32\x1c.clarifai.api.ModelTypeField\x12\"\n\x1arequires_sequential_frames\x18\x0c \x01(\x08\x12;\n\x15\x65xpected_input_layers\x18\x10 \x03(\x0b\x32\x1c.clarifai.api.ModelLayerInfo\x12<\n\x16\x65xpected_output_layers\x18\x11 \x03(\x0b\x32\x1c.clarifai.api.ModelLayerInfo\x12\x35\n\x0f\x65valuation_type\x18\x12 \x01(\x0e\x32\x1c.clarifai.api.EvaluationTypeJ\x04\x08\x07\x10\x08J\x04\x08\x04\x10\x05J\x04\x08\r\x10\x0eJ\x04\x08\x0e\x10\x0fJ\x04\x08\x0f\x10\x10\"\x89\x01\n\x0eModelLayerInfo\x12\x17\n\x0f\x64\x61ta_field_name\x18\x01 \x01(\t\x12(\n\x06shapes\x18\x02 \x03(\x0b\x32\x18.clarifai.api.LayerShape\x12\x13\n\x0b\x64\x65scription\x18\x03 \x01(\t\x12\x1f\n\x17requires_label_filename\x18\x04 \x01(\x08\"D\n\x12TritonCondaEnvInfo\x12\x16\n\x0e\x63onda_pack_url\x18\x01 \x01(\t\x12\x16\n\x0e\x63onda_yaml_url\x18\x02 \x01(\t\"l\n\nLayerShape\x12\x0c\n\x04\x64ims\x18\x01 \x03(\x05\x12\x10\n\x08max_dims\x18\x02 \x03(\x05\x12)\n\tdata_type\x18\x03 \x01(\x0e\x32\x16.clarifai.api.DataType\x12\x13\n\x0b\x64\x65scription\x18\x04 \x01(\t\"\xd2\x05\n\x0eModelTypeField\x12\x0c\n\x04path\x18\x01 \x01(\t\x12\x43\n\nfield_type\x18\x02 \x01(\x0e\x32/.clarifai.api.ModelTypeField.ModelTypeFieldType\x12-\n\rdefault_value\x18\x03 \x01(\x0b\x32\x16.google.protobuf.Value\x12\x13\n\x0b\x64\x65scription\x18\x04 \x01(\t\x12\x13\n\x0bplaceholder\x18\x05 \x01(\t\x12\x42\n\x17model_type_enum_options\x18\x06 \x03(\x0b\x32!.clarifai.api.ModelTypeEnumOption\x12\x15\n\rinternal_only\x18\x07 \x01(\x08\x12\x10\n\x08required\x18\x08 \x01(\x08\x12?\n\x15model_type_range_info\x18\t \x01(\x0b\x32 .clarifai.api.ModelTypeRangeInfo\"\xe5\x02\n\x12ModelTypeFieldType\x12!\n\x1dINVALID_MODEL_TYPE_FIELD_TYPE\x10\x00\x12\x0b\n\x07\x42OOLEAN\x10\x01\x12\n\n\x06STRING\x10\x02\x12\n\n\x06NUMBER\x10\x03\x12\x15\n\x11\x41RRAY_OF_CONCEPTS\x10\x04\x12$\n ARRAY_OF_CONCEPTS_WITH_THRESHOLD\x10\x05\x12\t\n\x05RANGE\x10\x07\x12\x08\n\x04\x45NUM\x10\x08\x12\x11\n\rCOLLABORATORS\x10\t\x12\x08\n\x04JSON\x10\n\x12\x14\n\x10\x41RRAY_OF_NUMBERS\x10\x0b\x12\x19\n\x15WORKFLOW_EMBED_MODELS\x10\x0c\x12\x14\n\x10\x41RRAY_OF_STRINGS\x10\r\x12\x12\n\x0eRECURSIVE_ENUM\x10\x0e\x12\x0f\n\x0bPYTHON_CODE\x10\x0f\x12\x0e\n\nDATASET_ID\x10\x10\x12\x16\n\x12\x44\x41TASET_VERSION_ID\x10\x11\"\x04\x08\x06\x10\x06\"<\n\x12ModelTypeRangeInfo\x12\x0b\n\x03min\x18\x01 \x01(\x02\x12\x0b\n\x03max\x18\x02 \x01(\x02\x12\x0c\n\x04step\x18\x03 \x01(\x02\"\xd4\x01\n\x13ModelTypeEnumOption\x12\n\n\x02id\x18\x01 \x01(\t\x12\x37\n\x07\x61liases\x18\x05 \x03(\x0b\x32&.clarifai.api.ModelTypeEnumOptionAlias\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\x37\n\x11model_type_fields\x18\x03 \x03(\x0b\x32\x1c.clarifai.api.ModelTypeField\x12\x15\n\rinternal_only\x18\x04 \x01(\x08\x12\x13\n\x0brecommended\x18\x06 \x01(\x08\"C\n\x18ModelTypeEnumOptionAlias\x12\x0e\n\x06id_int\x18\x01 \x01(\x03\x12\x17\n\x0fwildcard_string\x18\x02 \x01(\t\"7\n\nModelQuery\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x15\n\rmodel_type_id\x18\x03 \x01(\tJ\x04\x08\x02\x10\x03\"\xfc\x05\n\x0cModelVersion\x12\n\n\x02id\x18\x01 \x01(\t\x12.\n\ncreated_at\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12+\n\x06status\x18\x03 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x1c\n\x14\x61\x63tive_concept_count\x18\x04 \x01(\r\x12*\n\x07metrics\x18\x05 \x01(\x0b\x32\x19.clarifai.api.EvalMetrics\x12\x19\n\x11total_input_count\x18\x06 \x01(\r\x12\x44\n\x17pretrained_model_config\x18\x07 \x01(\x0b\x32#.clarifai.api.PretrainedModelConfig\x12\x30\n\x0c\x63ompleted_at\x18\n \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x13\n\x0b\x64\x65scription\x18\x0b \x01(\t\x12,\n\nvisibility\x18\x0c \x01(\x0b\x32\x18.clarifai.api.Visibility\x12\x0e\n\x06\x61pp_id\x18\r \x01(\t\x12\x0f\n\x07user_id\x18\x0e \x01(\t\x12/\n\x0bmodified_at\x18\x0f \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12)\n\x08metadata\x18\x10 \x01(\x0b\x32\x17.google.protobuf.Struct\x12\x0f\n\x07license\x18\x11 \x01(\t\x12-\n\x0boutput_info\x18\x13 \x01(\x0b\x32\x18.clarifai.api.OutputInfo\x12+\n\ninput_info\x18\x14 \x01(\x0b\x32\x17.clarifai.api.InputInfo\x12+\n\ntrain_info\x18\x15 \x01(\x0b\x32\x17.clarifai.api.TrainInfo\x12-\n\x0bimport_info\x18\x16 \x01(\x0b\x32\x18.clarifai.api.ImportInfo\x12\x11\n\ttrain_log\x18\x17 \x01(\tJ\x04\x08\t\x10\nJ\x04\x08\x12\x10\x13\"\xa1\x01\n\x15PretrainedModelConfig\x12\x31\n\x10input_fields_map\x18\x03 \x01(\x0b\x32\x17.google.protobuf.Struct\x12\x32\n\x11output_fields_map\x18\x04 \x01(\x0b\x32\x17.google.protobuf.Struct\x12\x15\n\rmodel_zip_url\x18\x06 \x01(\tJ\x04\x08\x02\x10\x03J\x04\x08\x05\x10\x06\">\n\nTrainStats\x12\x30\n\nloss_curve\x18\x01 \x03(\x0b\x32\x1c.clarifai.api.LossCurveEntry\"B\n\x0eLossCurveEntry\x12\r\n\x05\x65poch\x18\x01 \x01(\r\x12\x13\n\x0bglobal_step\x18\x02 \x01(\r\x12\x0c\n\x04\x63ost\x18\x03 \x01(\x02\"1\n\nLabelCount\x12\x14\n\x0c\x63oncept_name\x18\x01 \x01(\t\x12\r\n\x05\x63ount\x18\x02 \x01(\r\"L\n\x11LabelDistribution\x12\x37\n\x15positive_label_counts\x18\x01 \x03(\x0b\x32\x18.clarifai.api.LabelCount\"B\n\x17\x43ooccurrenceMatrixEntry\x12\x0b\n\x03row\x18\x01 \x01(\t\x12\x0b\n\x03\x63ol\x18\x02 \x01(\t\x12\r\n\x05\x63ount\x18\x03 \x01(\r\"`\n\x12\x43ooccurrenceMatrix\x12\x35\n\x06matrix\x18\x01 \x03(\x0b\x32%.clarifai.api.CooccurrenceMatrixEntry\x12\x13\n\x0b\x63oncept_ids\x18\x02 \x03(\t\"N\n\x14\x43onfusionMatrixEntry\x12\x11\n\tpredicted\x18\x01 \x01(\t\x12\x0e\n\x06\x61\x63tual\x18\x02 \x01(\t\x12\x13\n\x05value\x18\x04 \x01(\x02\x42\x04\x80\xb5\x18\x01\"Z\n\x0f\x43onfusionMatrix\x12\x32\n\x06matrix\x18\x01 \x03(\x0b\x32\".clarifai.api.ConfusionMatrixEntry\x12\x13\n\x0b\x63oncept_ids\x18\x02 \x03(\t\"t\n\x03ROC\x12\x11\n\x03\x66pr\x18\x01 \x03(\x02\x42\x04\x80\xb5\x18\x01\x12\x11\n\x03tpr\x18\x02 \x03(\x02\x42\x04\x80\xb5\x18\x01\x12\x18\n\nthresholds\x18\x03 \x03(\x02\x42\x04\x80\xb5\x18\x01\x12\x15\n\rfpr_per_image\x18\x04 \x03(\x02\x12\x16\n\x0e\x66pr_per_object\x18\x05 \x03(\x02\"_\n\x14PrecisionRecallCurve\x12\x14\n\x06recall\x18\x01 \x03(\x02\x42\x04\x80\xb5\x18\x01\x12\x17\n\tprecision\x18\x02 \x03(\x02\x42\x04\x80\xb5\x18\x01\x12\x18\n\nthresholds\x18\x03 \x03(\x02\x42\x04\x80\xb5\x18\x01\"\xea\x02\n\rBinaryMetrics\x12\x15\n\x07num_pos\x18\x01 \x01(\rB\x04\x80\xb5\x18\x01\x12\x15\n\x07num_neg\x18\x02 \x01(\rB\x04\x80\xb5\x18\x01\x12\x15\n\x07num_tot\x18\x03 \x01(\rB\x04\x80\xb5\x18\x01\x12\x15\n\x07roc_auc\x18\x04 \x01(\x02\x42\x04\x80\xb5\x18\x01\x12\x10\n\x02\x66\x31\x18\x05 \x01(\x02\x42\x04\x80\xb5\x18\x01\x12&\n\x07\x63oncept\x18\x06 \x01(\x0b\x32\x15.clarifai.api.Concept\x12$\n\troc_curve\x18\x07 \x01(\x0b\x32\x11.clarifai.api.ROC\x12\x42\n\x16precision_recall_curve\x18\x08 \x01(\x0b\x32\".clarifai.api.PrecisionRecallCurve\x12\x15\n\ravg_precision\x18\t \x01(\x02\x12\x11\n\tarea_name\x18\n \x01(\t\x12\x10\n\x08\x61rea_min\x18\x0b \x01(\x01\x12\x10\n\x08\x61rea_max\x18\x0c \x01(\x01\x12\x0b\n\x03iou\x18\r \x01(\x02\"\x91\x01\n\x0eTrackerMetrics\x12\x10\n\x08mot_mota\x18\x01 \x01(\x02\x12\x18\n\x10mot_num_switches\x18\x02 \x01(\x05\x12\x12\n\nmorse_frag\x18\x03 \x01(\x02\x12\x15\n\ravg_precision\x18\x04 \x01(\x02\x12\x0c\n\x04\x61iid\x18\x05 \x01(\t\x12\x1a\n\x12unique_switch_rate\x18\x06 \x01(\x02\"\xd9\x01\n\x10\x45valTestSetEntry\x12\"\n\x05input\x18\x06 \x01(\x0b\x32\x13.clarifai.api.Input\x12\x31\n\x12predicted_concepts\x18\x03 \x03(\x0b\x32\x15.clarifai.api.Concept\x12\x34\n\x15ground_truth_concepts\x18\x04 \x03(\x0b\x32\x15.clarifai.api.Concept\x12,\n\nannotation\x18\x05 \x01(\x0b\x32\x18.clarifai.api.AnnotationJ\x04\x08\x01\x10\x02J\x04\x08\x02\x10\x03\"\xcd\x01\n\x0eLOPQEvalResult\x12\t\n\x01k\x18\x01 \x01(\x05\x12#\n\x15recall_vs_brute_force\x18\x02 \x01(\x02\x42\x04\x80\xb5\x18\x01\x12(\n\x1akendall_tau_vs_brute_force\x18\x03 \x01(\x02\x42\x04\x80\xb5\x18\x01\x12(\n\x1amost_frequent_code_percent\x18\x04 \x01(\x02\x42\x04\x80\xb5\x18\x01\x12\x17\n\tlopq_ndcg\x18\x05 \x01(\x02\x42\x04\x80\xb5\x18\x01\x12\x1e\n\x10\x62rute_force_ndcg\x18\x06 \x01(\x02\x42\x04\x80\xb5\x18\x01\"\x8c\x03\n\x0eMetricsSummary\x12\x19\n\rtop1_accuracy\x18\x01 \x01(\x02\x42\x02\x18\x01\x12\x19\n\rtop5_accuracy\x18\x02 \x01(\x02\x42\x02\x18\x01\x12\x1f\n\x11macro_avg_roc_auc\x18\x03 \x01(\x02\x42\x04\x80\xb5\x18\x01\x12\x1f\n\x11macro_std_roc_auc\x18\x04 \x01(\x02\x42\x04\x80\xb5\x18\x01\x12 \n\x12macro_avg_f1_score\x18\x05 \x01(\x02\x42\x04\x80\xb5\x18\x01\x12 \n\x12macro_std_f1_score\x18\x06 \x01(\x02\x42\x04\x80\xb5\x18\x01\x12!\n\x13macro_avg_precision\x18\x07 \x01(\x02\x42\x04\x80\xb5\x18\x01\x12\x1e\n\x10macro_avg_recall\x18\x08 \x01(\x02\x42\x04\x80\xb5\x18\x01\x12!\n\x19mean_avg_precision_iou_50\x18\n \x01(\x02\x12$\n\x1cmean_avg_precision_iou_range\x18\x0b \x01(\x02\x12\x32\n\x0clopq_metrics\x18\t \x03(\x0b\x32\x1c.clarifai.api.LOPQEvalResult\"\xda\x04\n\x0b\x45valMetrics\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\n\n\x02id\x18\n \x01(\t\x12-\n\x07summary\x18\x02 \x01(\x0b\x32\x1c.clarifai.api.MetricsSummary\x12\x37\n\x10\x63onfusion_matrix\x18\x03 \x01(\x0b\x32\x1d.clarifai.api.ConfusionMatrix\x12=\n\x13\x63ooccurrence_matrix\x18\x04 \x01(\x0b\x32 .clarifai.api.CooccurrenceMatrix\x12\x35\n\x0clabel_counts\x18\x05 \x01(\x0b\x32\x1f.clarifai.api.LabelDistribution\x12\x33\n\x0e\x62inary_metrics\x18\x06 \x03(\x0b\x32\x1b.clarifai.api.BinaryMetrics\x12\x30\n\x08test_set\x18\x07 \x03(\x0b\x32\x1e.clarifai.api.EvalTestSetEntry\x12\x34\n\x0fmetrics_by_area\x18\x08 \x03(\x0b\x32\x1b.clarifai.api.BinaryMetrics\x12\x35\n\x10metrics_by_class\x18\t \x03(\x0b\x32\x1b.clarifai.api.BinaryMetrics\x12\x35\n\x0ftracker_metrics\x18\x0b \x03(\x0b\x32\x1c.clarifai.api.TrackerMetrics\x12)\n\teval_info\x18\x0c \x01(\x0b\x32\x16.clarifai.api.EvalInfo\"\xb7\x01\n\x0b\x46ieldsValue\x12\x18\n\x10\x63onfusion_matrix\x18\x01 \x01(\x08\x12\x1b\n\x13\x63ooccurrence_matrix\x18\x02 \x01(\x08\x12\x14\n\x0clabel_counts\x18\x03 \x01(\x08\x12\x16\n\x0e\x62inary_metrics\x18\x04 \x01(\x08\x12\x10\n\x08test_set\x18\x05 \x01(\x08\x12\x17\n\x0fmetrics_by_area\x18\x06 \x01(\x08\x12\x18\n\x10metrics_by_class\x18\x07 \x01(\x08\"\xdb\x01\n\x06Output\x12\n\n\x02id\x18\x01 \x01(\t\x12+\n\x06status\x18\x02 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12.\n\ncreated_at\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\"\n\x05model\x18\x04 \x01(\x0b\x32\x13.clarifai.api.Model\x12\"\n\x05input\x18\x05 \x01(\x0b\x32\x13.clarifai.api.Input\x12 \n\x04\x64\x61ta\x18\x06 \x01(\x0b\x32\x12.clarifai.api.Data\"4\n\tScopeDeps\x12\r\n\x05scope\x18\x01 \x01(\t\x12\x18\n\x10\x64\x65pending_scopes\x18\x02 \x03(\t\":\n\x0c\x45ndpointDeps\x12\x10\n\x08\x65ndpoint\x18\x01 \x01(\t\x12\x18\n\x10\x64\x65pending_scopes\x18\x02 \x03(\t\"\x8d\x01\n\x03Hit\x12\x13\n\x05score\x18\x01 \x01(\x02\x42\x04\x80\xb5\x18\x01\x12\"\n\x05input\x18\x02 \x01(\x0b\x32\x13.clarifai.api.Input\x12,\n\nannotation\x18\x03 \x01(\x0b\x32\x18.clarifai.api.Annotation\x12\x0f\n\x07user_id\x18\x04 \x01(\t\x12\x0e\n\x06\x61pp_id\x18\x05 \x01(\t\"#\n\x08HitCount\x12\x17\n\x0f\x65stimated_total\x18\x01 \x01(\x04\"\x8d\x01\n\x03\x41nd\x12\"\n\x05input\x18\x01 \x01(\x0b\x32\x13.clarifai.api.Input\x12$\n\x06output\x18\x02 \x01(\x0b\x32\x14.clarifai.api.Output\x12\x0e\n\x06negate\x18\x03 \x01(\x08\x12,\n\nannotation\x18\x04 \x01(\x0b\x32\x18.clarifai.api.Annotation\"\x88\x01\n\x05Query\x12#\n\x04\x61nds\x18\x01 \x03(\x0b\x32\x11.clarifai.api.AndB\x02\x18\x01\x12\x10\n\x08language\x18\x02 \x01(\t\x12%\n\x07\x66ilters\x18\x03 \x03(\x0b\x32\x14.clarifai.api.Filter\x12!\n\x05ranks\x18\x04 \x03(\x0b\x32\x12.clarifai.api.Rank\"\xd6\x03\n\x06Search\x12\"\n\x05query\x18\x01 \x01(\x0b\x32\x13.clarifai.api.Query\x12\n\n\x02id\x18\x02 \x01(\t\x12\x16\n\x0e\x61pplication_id\x18\x03 \x01(\t\x12\x0c\n\x04name\x18\x04 \x01(\t\x12)\n\x05\x61s_of\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x10\n\x08git_hash\x18\x06 \x01(\t\x12.\n\ncreated_at\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12/\n\x0bmodified_at\x18\x08 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x11\n\talgorithm\x18\t \x01(\t\x12\x0c\n\x04save\x18\n \x01(\x08\x12\x11\n\tmin_value\x18\x0b \x01(\x02\x12,\n\nvisibility\x18\x0c \x01(\x0b\x32\x18.clarifai.api.Visibility\x12+\n\x06metric\x18\r \x01(\x0e\x32\x1b.clarifai.api.Search.Metric\"I\n\x06Metric\x12\x12\n\x0eMETRIC_NOT_SET\x10\x00\x12\x16\n\x12\x45UCLIDEAN_DISTANCE\x10\x01\x12\x13\n\x0f\x43OSINE_DISTANCE\x10\x02\"\xa4\x01\n\x06\x46ilter\x12\x0e\n\x06negate\x18\x03 \x01(\x08\x12,\n\nannotation\x18\x04 \x01(\x0b\x32\x18.clarifai.api.Annotation\x12\"\n\x05input\x18\x05 \x01(\x0b\x32\x13.clarifai.api.Input\x12\x38\n\x17last_updated_time_range\x18\x06 \x01(\x0b\x32\x17.clarifai.api.TimeRange\"i\n\tTimeRange\x12.\n\nstart_time\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12,\n\x08\x65nd_time\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"D\n\x04Rank\x12\x0e\n\x06negate\x18\x03 \x01(\x08\x12,\n\nannotation\x18\x04 \x01(\x0b\x32\x18.clarifai.api.Annotation\"\x8d\x02\n\x17\x41nnotationSearchMetrics\x12*\n\x0cground_truth\x18\x01 \x01(\x0b\x32\x14.clarifai.api.Search\x12,\n\x0esearch_to_eval\x18\x02 \x01(\x0b\x32\x14.clarifai.api.Search\x12*\n\x07metrics\x18\x03 \x01(\x0b\x32\x19.clarifai.api.EvalMetrics\x12 \n\x04\x64\x61ta\x18\x04 \x01(\x0b\x32\x12.clarifai.api.Data\x12\x1c\n\x14\x61\x63tive_concept_count\x18\x05 \x01(\r\x12,\n\nvisibility\x18\x06 \x01(\x0b\x32\x18.clarifai.api.Visibility\"\x91\x01\n\x04Text\x12\x0b\n\x03raw\x18\x01 \x01(\t\x12\x0b\n\x03url\x18\x02 \x01(\t\x12\x1b\n\x13\x61llow_duplicate_url\x18\x03 \x01(\x08\x12\'\n\x06hosted\x18\x04 \x01(\x0b\x32\x17.clarifai.api.HostedURL\x12)\n\ttext_info\x18\x05 \x01(\x0b\x32\x16.clarifai.api.TextInfo\"0\n\x08TextInfo\x12\x12\n\nchar_count\x18\x01 \x01(\x05\x12\x10\n\x08\x65ncoding\x18\x02 \x01(\t\"\xfc\x05\n\x04User\x12\n\n\x02id\x18\x01 \x01(\t\x12\x19\n\rprimary_email\x18\x02 \x01(\tB\x02\x18\x01\x12\x12\n\nfirst_name\x18\x03 \x01(\t\x12\x11\n\tlast_name\x18\x04 \x01(\t\x12\x14\n\x0c\x63ompany_name\x18\x05 \x01(\t\x12\x11\n\tjob_title\x18\x13 \x01(\t\x12\x10\n\x08job_role\x18\x14 \x01(\t\x12\x15\n\tbill_type\x18\x07 \x01(\tB\x02\x18\x01\x12.\n\ncreated_at\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x39\n\x11\x64\x61te_gdpr_consent\x18\x08 \x01(\x0b\x32\x1a.google.protobuf.TimestampB\x02\x18\x01\x12\x38\n\x10\x64\x61te_tos_consent\x18\t \x01(\x0b\x32\x1a.google.protobuf.TimestampB\x02\x18\x01\x12>\n\x16\x64\x61te_marketing_consent\x18\n \x01(\x0b\x32\x1a.google.protobuf.TimestampB\x02\x18\x01\x12\x38\n\x10\x64\x61te_pii_consent\x18\x17 \x01(\x0b\x32\x1a.google.protobuf.TimestampB\x02\x18\x01\x12-\n\x08metadata\x18\x0b \x01(\x0b\x32\x17.google.protobuf.StructB\x02\x18\x01\x12\x37\n\x0f\x65mail_addresses\x18\x0c \x03(\x0b\x32\x1a.clarifai.api.EmailAddressB\x02\x18\x01\x12#\n\x17two_factor_auth_enabled\x18\x0f \x01(\x08\x42\x02\x18\x01\x12\x17\n\x0bteams_count\x18\x10 \x01(\rB\x02\x18\x01\x12\x12\n\nis_starred\x18\x15 \x01(\x08\x12\x12\n\nstar_count\x18\x16 \x01(\x05\x12,\n\nvisibility\x18\x11 \x01(\x0b\x32\x18.clarifai.api.Visibility\x12-\n\x0buser_detail\x18\x12 \x01(\x0b\x32\x18.clarifai.api.UserDetailJ\x04\x08\r\x10\x0eJ\x04\x08\x0e\x10\x0f\"\xd1\x03\n\nUserDetail\x12\x15\n\rprimary_email\x18\x01 \x01(\t\x12\x11\n\tbill_type\x18\x02 \x01(\t\x12\x35\n\x11\x64\x61te_gdpr_consent\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x34\n\x10\x64\x61te_tos_consent\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12:\n\x16\x64\x61te_marketing_consent\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x34\n\x10\x64\x61te_pii_consent\x18\r \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12)\n\x08metadata\x18\x06 \x01(\x0b\x32\x17.google.protobuf.Struct\x12\x33\n\x0f\x65mail_addresses\x18\x07 \x03(\x0b\x32\x1a.clarifai.api.EmailAddress\x12\x1f\n\x17two_factor_auth_enabled\x18\t \x01(\x08\x12\x13\n\x0bteams_count\x18\n \x01(\r\x12\x0f\n\x07\x63ountry\x18\x0b \x01(\t\x12\r\n\x05state\x18\x0c \x01(\tJ\x04\x08\x08\x10\t\"R\n\x0c\x45mailAddress\x12\x13\n\x05\x65mail\x18\x01 \x01(\tB\x04\x80\xb5\x18\x01\x12\x15\n\x07primary\x18\x02 \x01(\x08\x42\x04\x80\xb5\x18\x01\x12\x16\n\x08verified\x18\x03 \x01(\x08\x42\x04\x80\xb5\x18\x01\"\x1d\n\x08Password\x12\x11\n\tplaintext\x18\x01 \x01(\t\"\x86\x03\n\x12PasswordViolations\x12\x16\n\x0eminimum_length\x18\x01 \x01(\x08\x12\x16\n\x0emaximum_length\x18\x02 \x01(\x08\x12\x19\n\x11upper_case_needed\x18\x03 \x01(\x08\x12\x19\n\x11lower_case_needed\x18\x04 \x01(\x08\x12\x16\n\x0enumeric_needed\x18\x05 \x01(\x08\x12\x1f\n\x17non_alphanumeric_needed\x18\x06 \x01(\x08\x12\x16\n\x0epassword_reuse\x18\x07 \x01(\x08\x12\x15\n\rexclude_names\x18\x08 \x01(\x08\x12\x15\n\rexclude_email\x18\t \x01(\x08\x12\x1c\n\x14no_confusing_letters\x18\n \x01(\x08\x12\x1b\n\x13no_simple_passwords\x18\x0b \x01(\x08\x12\x18\n\x10no_common_vocabs\x18\x0c \x01(\x08\x12\x1b\n\x13no_overlap_with_old\x18\r \x01(\x08\x12\x19\n\x11password_lifespan\x18\x0e \x01(\x08\"\xae\x01\n\x05Video\x12\x0b\n\x03url\x18\x01 \x01(\t\x12\x0e\n\x06\x62\x61se64\x18\x02 \x01(\x0c\x12\x1b\n\x13\x61llow_duplicate_url\x18\x04 \x01(\x08\x12\x15\n\rthumbnail_url\x18\x05 \x01(\t\x12\'\n\x06hosted\x18\x06 \x01(\x0b\x32\x17.clarifai.api.HostedURL\x12+\n\nvideo_info\x18\x07 \x01(\x0b\x32\x17.clarifai.api.VideoInfo\"\x8e\x01\n\tVideoInfo\x12\r\n\x05width\x18\x01 \x01(\x05\x12\x0e\n\x06height\x18\x02 \x01(\x05\x12\x0b\n\x03\x66ps\x18\x03 \x01(\x02\x12\x14\n\x0cvideo_format\x18\x04 \x01(\t\x12\x10\n\x08\x62it_rate\x18\x05 \x01(\x05\x12\x13\n\x0b\x66rame_count\x18\x06 \x01(\x05\x12\x18\n\x10\x64uration_seconds\x18\x07 \x01(\x02\"\xcf\x03\n\x08Workflow\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0e\n\x06\x61pp_id\x18\x02 \x01(\t\x12.\n\ncreated_at\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12)\n\x05nodes\x18\x04 \x03(\x0b\x32\x1a.clarifai.api.WorkflowNode\x12)\n\x08metadata\x18\x05 \x01(\x0b\x32\x17.google.protobuf.Struct\x12,\n\nvisibility\x18\x06 \x01(\x0b\x32\x18.clarifai.api.Visibility\x12\x0f\n\x07user_id\x18\x07 \x01(\t\x12/\n\x0bmodified_at\x18\x08 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12.\n\x07version\x18\t \x01(\x0b\x32\x1d.clarifai.api.WorkflowVersion\x12\x12\n\nis_starred\x18\n \x01(\x08\x12\x12\n\nstar_count\x18\x0b \x01(\x05\x12\x13\n\x0b\x64\x65scription\x18\x0c \x01(\t\x12\r\n\x05notes\x18\r \x01(\t\x12\x17\n\tuse_cases\x18\x0e \x03(\tB\x04\x80\xb5\x18\x01\x12\x1c\n\x0e\x63heck_consents\x18\x0f \x03(\tB\x04\x80\xb5\x18\x01\"\xde\x02\n\x0fWorkflowVersion\x12\n\n\x02id\x18\x01 \x01(\t\x12\x13\n\x0bworkflow_id\x18\x02 \x01(\t\x12.\n\ncreated_at\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12/\n\x0bmodified_at\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12,\n\nvisibility\x18\x05 \x01(\x0b\x32\x18.clarifai.api.Visibility\x12)\n\x05nodes\x18\x06 \x03(\x0b\x32\x1a.clarifai.api.WorkflowNode\x12)\n\x08metadata\x18\x07 \x01(\x0b\x32\x17.google.protobuf.Struct\x12\x0e\n\x06\x61pp_id\x18\x08 \x01(\t\x12\x0f\n\x07user_id\x18\t \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\n \x01(\t\x12\x0f\n\x07license\x18\x0b \x01(\t\"\xbd\x01\n\x0cWorkflowNode\x12\n\n\x02id\x18\x01 \x01(\t\x12\"\n\x05model\x18\x02 \x01(\x0b\x32\x13.clarifai.api.Model\x12,\n\x0bnode_inputs\x18\x03 \x03(\x0b\x32\x17.clarifai.api.NodeInput\x12\x17\n\x0fsuppress_output\x18\x04 \x01(\x08\x12\x36\n\x14output_info_override\x18\x05 \x01(\x0b\x32\x18.clarifai.api.OutputInfo\"\x1c\n\tNodeInput\x12\x0f\n\x07node_id\x18\x01 \x01(\t\"\x81\x02\n\x0eWorkflowResult\x12\n\n\x02id\x18\x01 \x01(\t\x12+\n\x06status\x18\x02 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12.\n\ncreated_at\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\"\n\x05model\x18\x04 \x01(\x0b\x32\x13.clarifai.api.Model\x12\"\n\x05input\x18\x05 \x01(\x0b\x32\x13.clarifai.api.Input\x12%\n\x07outputs\x18\x06 \x03(\x0b\x32\x14.clarifai.api.Output\x12\x17\n\x0fsuppress_output\x18\x07 \x01(\x08\"\x1b\n\rWorkflowState\x12\n\n\x02id\x18\x01 \x01(\t\"\xd8\x02\n\x0e\x41ppDuplication\x12\n\n\x02id\x18\x01 \x01(\t\x12\x12\n\nnew_app_id\x18\x02 \x01(\t\x12\x14\n\x0cnew_app_name\x18\x03 \x01(\t\x12+\n\x06status\x18\x04 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12.\n\ncreated_at\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x34\n\x10last_modified_at\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x33\n\x06\x66ilter\x18\x07 \x01(\x0b\x32#.clarifai.api.AppDuplicationFilters\x12\x17\n\x0f\x65xisting_app_id\x18\x08 \x01(\t\x12/\n\x08progress\x18\t \x03(\x0b\x32\x1d.clarifai.api.AppCopyProgress\"/\n\x0f\x41ppCopyProgress\x12\r\n\x05\x66ield\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x05\"\x8a\x01\n\x15\x41ppDuplicationFilters\x12\x13\n\x0b\x63opy_inputs\x18\x01 \x01(\x08\x12\x15\n\rcopy_concepts\x18\x02 \x01(\x08\x12\x18\n\x10\x63opy_annotations\x18\x03 \x01(\x08\x12\x13\n\x0b\x63opy_models\x18\x04 \x01(\x08\x12\x16\n\x0e\x63opy_workflows\x18\x05 \x01(\x08\"\xfa\x02\n\nLabelOrder\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12+\n\x06status\x18\x03 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x14\n\x0c\x61uto_release\x18\x04 \x01(\x08\x12\x17\n\x0f\x61llow_empty_tag\x18\x05 \x01(\x08\x12\x38\n\x14\x64\x65sired_fulfill_time\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x39\n\x15\x65stimate_fulfill_time\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12 \n\x04task\x18\x08 \x01(\x0b\x32\x12.clarifai.api.Task\x12.\n\ncreated_at\x18\t \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12/\n\x0bmodified_at\x18\n \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"\xb7\x06\n\x04Task\x12\n\n\x02id\x18\x01 \x01(\t\x12.\n\ncreated_at\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12/\n\x0bmodified_at\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12)\n\x04type\x18\x04 \x01(\x0e\x32\x1b.clarifai.api.Task.TaskType\x12\x13\n\x0b\x64\x65scription\x18\x05 \x01(\t\x12(\n\x06worker\x18\x06 \x01(\x0b\x32\x18.clarifai.api.TaskWorker\x12\x13\n\x0b\x63oncept_ids\x18\x07 \x03(\t\x12\x33\n\x0cinput_source\x18\x08 \x01(\x0b\x32\x1d.clarifai.api.TaskInputSource\x12\x11\n\tsample_ms\x18\t \x01(\r\x12\x33\n\x0c\x61i_assistant\x18\n \x01(\x0b\x32\x1d.clarifai.api.TaskAIAssistant\x12(\n\x06review\x18\x0b \x01(\x0b\x32\x18.clarifai.api.TaskReview\x12+\n\x06status\x18\x0c \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x0c\n\x04name\x18\r \x01(\t\x12:\n\x10\x61i_assist_params\x18\x0e \x01(\x0b\x32 .clarifai.api.AiAssistParameters\x12,\n\nvisibility\x18\x0f \x01(\x0b\x32\x18.clarifai.api.Visibility\x12\x0e\n\x06\x61pp_id\x18\x10 \x01(\t\x12\x0f\n\x07user_id\x18\x11 \x01(\t\x12\x16\n\x0elabel_order_id\x18\x12 \x01(\t\x12+\n\x08\x63oncepts\x18\x13 \x03(\x0b\x32\x19.clarifai.api.TaskConcept\x12#\n\x1b\x64\x65lete_previous_annotations\x18\x14 \x01(\x08\"l\n\x08TaskType\x12\x10\n\x0cTYPE_NOT_SET\x10\x00\x12\x1b\n\x17\x43ONCEPTS_CLASSIFICATION\x10\x01\x12\x1a\n\x16\x42OUNDING_BOX_DETECTION\x10\x02\x12\x15\n\x11POLYGON_DETECTION\x10\x03\"`\n\x12\x41iAssistParameters\x12\x15\n\rmin_threshold\x18\x01 \x01(\x02\x12\x15\n\rmax_threshold\x18\x02 \x01(\x02\x12\x1c\n\x14\x63oncept_relation_ids\x18\x03 \x03(\t\"\x8f\x03\n\nTaskWorker\x12=\n\x08strategy\x18\x01 \x01(\x0e\x32+.clarifai.api.TaskWorker.TaskWorkerStrategy\x12\x14\n\x08user_ids\x18\x02 \x03(\tB\x02\x18\x01\x12!\n\x05users\x18\x04 \x03(\x0b\x32\x12.clarifai.api.User\x12#\n\x06models\x18\x05 \x03(\x0b\x32\x13.clarifai.api.Model\x12)\n\tworkflows\x18\x06 \x03(\x0b\x32\x16.clarifai.api.Workflow\x12T\n\x19partitioned_strategy_info\x18\x03 \x01(\x0b\x32/.clarifai.api.TaskWorkerPartitionedStrategyInfoH\x00\"R\n\x12TaskWorkerStrategy\x12\x1b\n\x17WORKER_STRATEGY_NOT_SET\x10\x00\x12\x0f\n\x0bPARTITIONED\x10\x02\x12\x08\n\x04\x46ULL\x10\x03\"\x04\x08\x01\x10\x01\x42\x0f\n\rstrategy_info\"\xa9\x02\n!TaskWorkerPartitionedStrategyInfo\x12[\n\x04type\x18\x01 \x01(\x0e\x32M.clarifai.api.TaskWorkerPartitionedStrategyInfo.TaskWorkerPartitionedStrategy\x12\x19\n\x11workers_per_input\x18\x02 \x01(\x05\x12(\n\x07weights\x18\x03 \x01(\x0b\x32\x17.google.protobuf.Struct\"b\n\x1dTaskWorkerPartitionedStrategy\x12\'\n#PARTITIONED_WORKER_STRATEGY_NOT_SET\x10\x00\x12\n\n\x06\x45VENLY\x10\x01\x12\x0c\n\x08WEIGHTED\x10\x02\"\xc3\x01\n\x0fTaskInputSource\x12?\n\x04type\x18\x01 \x01(\x0e\x32\x31.clarifai.api.TaskInputSource.TaskInputSourceType\x12\n\n\x02id\x18\x02 \x01(\t\"c\n\x13TaskInputSourceType\x12\x1d\n\x19INPUT_SOURCE_TYPE_NOT_SET\x10\x00\x12\x0e\n\nALL_INPUTS\x10\x01\x12\x10\n\x0cSAVED_SEARCH\x10\x02\x12\x0b\n\x07\x44\x41TASET\x10\x03\"\x90\x03\n\nTaskReview\x12=\n\x08strategy\x18\x01 \x01(\x0e\x32+.clarifai.api.TaskReview.TaskReviewStrategy\x12\x14\n\x08user_ids\x18\x02 \x03(\tB\x02\x18\x01\x12!\n\x05users\x18\x05 \x03(\x0b\x32\x12.clarifai.api.User\x12J\n\x14manual_strategy_info\x18\x03 \x01(\x0b\x32*.clarifai.api.TaskReviewManualStrategyInfoH\x00\x12P\n\x17\x63onsensus_strategy_info\x18\x04 \x01(\x0b\x32-.clarifai.api.TaskReviewConsensusStrategyInfoH\x00\"[\n\x12TaskReviewStrategy\x12 \n\x1cTASK_REVIEW_STRATEGY_NOT_SET\x10\x00\x12\x08\n\x04NONE\x10\x01\x12\n\n\x06MANUAL\x10\x02\x12\r\n\tCONSENSUS\x10\x03\x42\x0f\n\rstrategy_info\"9\n\x1cTaskReviewManualStrategyInfo\x12\x19\n\x11sample_percentage\x18\x01 \x01(\x02\"C\n\x1fTaskReviewConsensusStrategyInfo\x12\x1a\n\x12\x61pproval_threshold\x18\x02 \x01(\rJ\x04\x08\x01\x10\x02\"&\n\x0fTaskAIAssistant\x12\x13\n\x0bworkflow_id\x18\x01 \x01(\t\"\xbc\x01\n\x16TaskStatusCountPerUser\x12\x0f\n\x07user_id\x18\x01 \x01(\t\x12\x15\n\x07pending\x18\x02 \x01(\rB\x04\x80\xb5\x18\x01\x12\x1d\n\x0f\x61waiting_review\x18\x03 \x01(\rB\x04\x80\xb5\x18\x01\x12\x15\n\x07success\x18\x04 \x01(\rB\x04\x80\xb5\x18\x01\x12\x1b\n\rreview_denied\x18\x05 \x01(\rB\x04\x80\xb5\x18\x01\x12\'\n\x19\x61waiting_consensus_review\x18\x06 \x01(\rB\x04\x80\xb5\x18\x01\"f\n\x0eThresholdRange\x12\x1a\n\x12is_lower_inclusive\x18\x01 \x01(\x08\x12\x1a\n\x12is_upper_inclusive\x18\x02 \x01(\x08\x12\r\n\x05lower\x18\x03 \x01(\x02\x12\r\n\x05upper\x18\x04 \x01(\x02\"\xad\x01\n\x1fTaskConceptAutoAnnotationConfig\x12\x1d\n\x15\x61nnotation_data_types\x18\x01 \x01(\r\x12\x35\n\x0fthreshold_range\x18\x02 \x01(\x0b\x32\x1c.clarifai.api.ThresholdRange\x12\x34\n\x0bstatus_code\x18\x03 \x01(\x0e\x32\x1f.clarifai.api.status.StatusCode\"\x84\x01\n\x0bTaskConcept\x12&\n\x07\x63oncept\x18\x01 \x01(\x0b\x32\x15.clarifai.api.Concept\x12M\n\x16\x61uto_annotation_config\x18\x02 \x01(\x0b\x32-.clarifai.api.TaskConceptAutoAnnotationConfig\"\x81\x02\n\tCollector\x12\n\n\x02id\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12.\n\ncreated_at\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x1d\n\x15pre_queue_workflow_id\x18\x04 \x01(\t\x12\x1e\n\x16post_queue_workflow_id\x18\x05 \x01(\t\x12\x37\n\x10\x63ollector_source\x18\x06 \x01(\x0b\x32\x1d.clarifai.api.CollectorSource\x12+\n\x06status\x18\x07 \x01(\x0b\x32\x1b.clarifai.api.status.Status\"t\n\x0f\x43ollectorSource\x12\x61\n\'api_post_model_outputs_collector_source\x18\x02 \x01(\x0b\x32\x30.clarifai.api.APIPostModelOutputsCollectorSource\"\x99\x01\n\"APIPostModelOutputsCollectorSource\x12\x15\n\rmodel_user_id\x18\x01 \x01(\t\x12\x14\n\x0cmodel_app_id\x18\x02 \x01(\t\x12\x10\n\x08model_id\x18\x03 \x01(\t\x12\x18\n\x10model_version_id\x18\x04 \x01(\t\x12\x1a\n\x12post_inputs_key_id\x18\x05 \x01(\t\"R\n\tStatValue\x12(\n\x04time\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\r\n\x05value\x18\x02 \x01(\x02\x12\x0c\n\x04tags\x18\x03 \x03(\t\"\xa6\x01\n\x18StatValueAggregateResult\x12?\n\x15stat_value_aggregates\x18\x01 \x03(\x0b\x32 .clarifai.api.StatValueAggregate\x12I\n\x1astat_value_aggregate_query\x18\x02 \x01(\x0b\x32%.clarifai.api.StatValueAggregateQuery\"t\n\x12StatValueAggregate\x12(\n\x04time\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x17\n\x0f\x61ggregate_value\x18\x02 \x01(\x02\x12\r\n\x05\x63ount\x18\x03 \x01(\x04\x12\x0c\n\x04tags\x18\x04 \x03(\t\"\x91\x02\n\x17StatValueAggregateQuery\x12\x0c\n\x04tags\x18\x01 \x03(\t\x12\x12\n\ntag_groups\x18\x02 \x03(\t\x12;\n\x13stat_value_agg_type\x18\x03 \x01(\x0e\x32\x1e.clarifai.api.StatValueAggType\x12\x39\n\x12stat_time_agg_type\x18\x04 \x01(\x0e\x32\x1d.clarifai.api.StatTimeAggType\x12.\n\nstart_time\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12,\n\x08\x65nd_time\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"\xef\x01\n\x19\x44\x61tasetInputsSearchAddJob\x12\n\n\x02id\x18\x01 \x01(\t\x12.\n\ncreated_at\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12/\n\x0bmodified_at\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12+\n\x06status\x18\x04 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x12\n\ndataset_id\x18\x05 \x01(\t\x12$\n\x06search\x18\x06 \x01(\x0b\x32\x14.clarifai.api.Search\"O\n\x17PCAProjectionComparator\x12\x1a\n\x12\x64istance_threshold\x18\x01 \x01(\x02\x12\x18\n\x10model_version_id\x18\x02 \x01(\t\"K\n\x1b\x44uplicateAnnotationsResults\x12\x16\n\x0e\x64uplicate_cfid\x18\x01 \x03(\t\x12\x14\n\x0cunique_count\x18\x02 \x01(\x05\"\x87\x01\n\nVisibility\x12\x33\n\x08gettable\x18\x01 \x01(\x0e\x32!.clarifai.api.Visibility.Gettable\"D\n\x08Gettable\x12\x16\n\x12UNKNOWN_VISIBILITY\x10\x00\x12\x0b\n\x07PRIVATE\x10\n\x12\x07\n\x03ORG\x10\x1e\x12\n\n\x06PUBLIC\x10\x32\"X\n\x0eTrendingMetric\x12\x0f\n\x07user_id\x18\x01 \x01(\t\x12\x0e\n\x06\x61pp_id\x18\x02 \x01(\t\x12\x11\n\tobject_id\x18\x03 \x01(\t\x12\x12\n\nview_count\x18\x04 \x01(\x04\"#\n\x07\x46ullTag\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\n\n\x02id\x18\x02 \x01(\t\"f\n\x0bTimeSegment\x12\n\n\x02id\x18\x01 \x01(\t\x12 \n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x12.clarifai.api.Data\x12)\n\ttime_info\x18\x03 \x01(\x0b\x32\x16.clarifai.api.TimeInfo\"D\n\x08TimeInfo\x12\x12\n\nnum_frames\x18\x01 \x01(\r\x12\x12\n\nbegin_time\x18\x02 \x01(\r\x12\x10\n\x08\x65nd_time\x18\x03 \x01(\r\"!\n\x0b\x44\x61tasetStar\x12\x12\n\ndataset_id\x18\x01 \x01(\t\"\x1f\n\nModuleStar\x12\x11\n\tmodule_id\x18\x01 \x01(\t\"\xe7\x02\n\x06Module\x12\n\n\x02id\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x03 \x01(\t\x12.\n\ncreated_at\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12/\n\x0bmodified_at\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12,\n\nvisibility\x18\x07 \x01(\x0b\x32\x18.clarifai.api.Visibility\x12)\n\x08metadata\x18\x08 \x01(\x0b\x32\x17.google.protobuf.Struct\x12\x0f\n\x07user_id\x18\t \x01(\t\x12\x0e\n\x06\x61pp_id\x18\n \x01(\t\x12\x33\n\x0emodule_version\x18\x0b \x01(\x0b\x32\x1b.clarifai.api.ModuleVersion\x12\x12\n\nis_starred\x18\x0c \x01(\x08\x12\x12\n\nstar_count\x18\r \x01(\x05J\x04\x08\x02\x10\x03\"\xbe\x04\n\rModuleVersion\x12\n\n\x02id\x18\x01 \x01(\t\x12\x11\n\tmodule_id\x18\x02 \x01(\t\x12\x0e\n\x06\x61pp_id\x18\x03 \x01(\t\x12\x0f\n\x07user_id\x18\x04 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x06 \x01(\t\x12\r\n\x05notes\x18\x07 \x01(\t\x12.\n\ncreated_at\x18\x08 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12/\n\x0bmodified_at\x18\t \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x16\n\x0egit_commit_url\x18\n \x01(\t\x12\x39\n\nmodule_nav\x18\x0b \x01(\x0b\x32%.clarifai.api.ModuleVersion.ModuleNav\x12\x10\n\x08\x61pproved\x18\x0c \x01(\x08\x12,\n\nvisibility\x18\r \x01(\x0b\x32\x18.clarifai.api.Visibility\x12)\n\x08metadata\x18\x0e \x01(\x0b\x32\x17.google.protobuf.Struct\x1a\x45\n\x0cModuleSubNav\x12\r\n\x05title\x18\x01 \x01(\t\x12\x11\n\tquery_key\x18\x02 \x01(\t\x12\x13\n\x0bquery_value\x18\x03 \x01(\t\x1a]\n\tModuleNav\x12\r\n\x05title\x18\x01 \x01(\t\x12\x41\n\x0fmodule_sub_navs\x18\x02 \x03(\x0b\x32(.clarifai.api.ModuleVersion.ModuleSubNavJ\x04\x08\x05\x10\x06\"\xad\x02\n\x16InstalledModuleVersion\x12\n\n\x02id\x18\x01 \x01(\t\x12\x33\n\x0emodule_version\x18\x02 \x01(\x0b\x32\x1b.clarifai.api.ModuleVersion\x12\x0e\n\x06\x61pp_id\x18\x03 \x01(\t\x12\x0f\n\x07user_id\x18\x04 \x01(\t\x12.\n\ncreated_at\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12/\n\x0bmodified_at\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x12\n\ndeploy_url\x18\x07 \x01(\t\x12,\n\nvisibility\x18\x08 \x01(\x0b\x32\x18.clarifai.api.Visibility\x12\x0e\n\x06key_id\x18\t \x01(\t\"\xb7\x03\n\rBulkOperation\x12\n\n\x02id\x18\x01 \x01(\t\x12+\n\tinput_ids\x18\x02 \x01(\x0b\x32\x16.clarifai.api.InputIDsH\x00\x12&\n\x06search\x18\n \x01(\x0b\x32\x14.clarifai.api.SearchH\x00\x12(\n\x07\x64\x61taset\x18\x0b \x01(\x0b\x32\x15.clarifai.api.DatasetH\x00\x12*\n\toperation\x18\x03 \x01(\x0b\x32\x17.clarifai.api.Operation\x12\x0e\n\x06\x61pp_id\x18\x04 \x01(\t\x12+\n\x06status\x18\x05 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12(\n\x08progress\x18\x06 \x01(\x0b\x32\x16.clarifai.api.Progress\x12\x12\n\ncreated_by\x18\x07 \x01(\t\x12.\n\ncreated_at\x18\x08 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x34\n\x10last_modified_at\x18\t \x01(\x0b\x32\x1a.google.protobuf.TimestampB\x0e\n\x0cinput_source\"\x1d\n\x08InputIDs\x12\x11\n\tinput_ids\x18\x01 \x03(\t\"8\n\x08Progress\x12\x11\n\tprocessed\x18\x01 \x01(\r\x12\x19\n\x11last_processed_id\x18\x02 \x01(\t\"\x8a\x04\n\tOperation\x12\x31\n\x0c\x61\x64\x64_concepts\x18\x01 \x01(\x0b\x32\x19.clarifai.api.AddConceptsH\x00\x12\x37\n\x0f\x64\x65lete_concepts\x18\x02 \x01(\x0b\x32\x1c.clarifai.api.DeleteConceptsH\x00\x12\x31\n\x0c\x61\x64\x64_metadata\x18\x03 \x01(\x0b\x32\x19.clarifai.api.AddMetadataH\x00\x12\x37\n\x0f\x64\x65lete_metadata\x18\x04 \x01(\x0b\x32\x1c.clarifai.api.DeleteMetadataH\x00\x12\x33\n\roverwrite_geo\x18\x05 \x01(\x0b\x32\x1a.clarifai.api.OverwriteGeoH\x00\x12-\n\ndelete_geo\x18\x06 \x01(\x0b\x32\x17.clarifai.api.DeleteGeoH\x00\x12>\n\x13\x64\x65lete_from_dataset\x18\x07 \x01(\x0b\x32\x1f.clarifai.api.DeleteFromDatasetH\x00\x12\x34\n\x0e\x61\x64\x64_to_dataset\x18\x08 \x01(\x0b\x32\x1a.clarifai.api.AddToDatasetH\x00\x12>\n\x13split_into_datasets\x18\t \x01(\x0b\x32\x1f.clarifai.api.SplitIntoDatasetsH\x00\x42\x0b\n\toperation\"6\n\x0b\x41\x64\x64\x43oncepts\x12\'\n\x08\x63oncepts\x18\x01 \x03(\x0b\x32\x15.clarifai.api.Concept\"K\n\x0e\x44\x65leteConcepts\x12\'\n\x08\x63oncepts\x18\x01 \x03(\x0b\x32\x15.clarifai.api.Concept\x12\x10\n\x08user_ids\x18\x02 \x03(\t\"8\n\x0b\x41\x64\x64Metadata\x12)\n\x08metadata\x18\x01 \x01(\x0b\x32\x17.google.protobuf.Struct\";\n\x0e\x44\x65leteMetadata\x12)\n\x08metadata\x18\x01 \x01(\x0b\x32\x17.google.protobuf.Struct\".\n\x0cOverwriteGeo\x12\x1e\n\x03geo\x18\x01 \x01(\x0b\x32\x11.clarifai.api.Geo\"\x0b\n\tDeleteGeo\"\"\n\x0c\x41\x64\x64ToDataset\x12\x12\n\ndataset_id\x18\x01 \x01(\t\"\'\n\x11\x44\x65leteFromDataset\x12\x12\n\ndataset_id\x18\x01 \x01(\t\"\xcb\x01\n\x11SplitIntoDatasets\x12\x32\n\x0e\x64\x61taset_splits\x18\x01 \x03(\x0b\x32\x1a.clarifai.api.DatasetSplit\x12\x42\n\x06method\x18\x02 \x01(\x0e\x32\x32.clarifai.api.SplitIntoDatasets.DatasetSplitMethod\">\n\x12\x44\x61tasetSplitMethod\x12\x0b\n\x07NOT_SET\x10\x00\x12\x1b\n\x17RANDOM_PERCENTAGE_SPLIT\x10\x01\"[\n\x0c\x44\x61tasetSplit\x12&\n\x07\x64\x61taset\x18\x01 \x01(\x0b\x32\x15.clarifai.api.Dataset\x12\x14\n\npercentage\x18\x02 \x01(\rH\x00\x42\r\n\x0bmethod_info\"\xce\x02\n\x0cInputsAddJob\x12\n\n\x02id\x18\x01 \x01(\t\x12\x15\n\rcall_back_url\x18\x03 \x01(\t\x12\x0f\n\x07\x61pp_pat\x18\x04 \x01(\t\x12\x34\n\x08progress\x18\x07 \x01(\x0b\x32\".clarifai.api.InputsAddJobProgress\x12.\n\ncreated_at\x18\x08 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12/\n\x0bmodified_at\x18\t \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12:\n\x0f\x65xtraction_jobs\x18\n \x03(\x0b\x32!.clarifai.api.InputsExtractionJob\x12%\n\x07uploads\x18\x0b \x03(\x0b\x32\x14.clarifai.api.UploadJ\x04\x08\x02\x10\x03J\x04\x08\x05\x10\x06J\x04\x08\x06\x10\x07\"u\n\x14InputsAddJobProgress\x12\x15\n\rpending_count\x18\x01 \x01(\x04\x12\x19\n\x11in_progress_count\x18\x02 \x01(\x04\x12\x15\n\rsuccess_count\x18\x03 \x01(\x04\x12\x14\n\x0c\x66\x61iled_count\x18\x04 \x01(\x04\"\x95\x02\n\x06Upload\x12\n\n\x02id\x18\x01 \x01(\t\x12.\n\ncreated_at\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12/\n\x0bmodified_at\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12.\n\nexpires_at\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12+\n\x06status\x18\x05 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x14\n\x0c\x63ontent_name\x18\x08 \x01(\t\x12\x16\n\x0e\x63ontent_length\x18\x06 \x01(\x04\x12\x13\n\x0b\x63ontent_url\x18\x07 \x01(\t\"K\n\x11UploadContentPart\x12\x13\n\x0brange_start\x18\x01 \x01(\x04\x12\x13\n\x0bpart_number\x18\x02 \x01(\x03\x12\x0c\n\x04\x64\x61ta\x18\x03 \x01(\x0c\"l\n\x19\x43ustomCodeOperatorRequest\x12#\n\x06inputs\x18\x01 \x03(\x0b\x32\x13.clarifai.api.Input\x12*\n\x08metadata\x18\xea\x07 \x01(\x0b\x32\x17.google.protobuf.Struct\"\xf9\x01\n\x13InputsExtractionJob\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\n\n\x02id\x18\x02 \x01(\t\x12\x0b\n\x03url\x18\x03 \x01(\t\x12;\n\x08progress\x18\x04 \x01(\x0b\x32).clarifai.api.InputsExtractionJobProgress\x12.\n\ncreated_at\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12/\n\x0bmodified_at\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"\xad\x02\n\x1bInputsExtractionJobProgress\x12\x1a\n\x12read_objects_count\x18\x01 \x01(\x04\x12\x1a\n\x12\x61udio_inputs_count\x18\x02 \x01(\x04\x12\x1a\n\x12image_inputs_count\x18\x03 \x01(\x04\x12\x1a\n\x12video_inputs_count\x18\x04 \x01(\x04\x12\x19\n\x11text_inputs_count\x18\x05 \x01(\x04\x12\x1e\n\x16pending_archives_count\x18\x06 \x01(\x04\x12\"\n\x1ain_progress_archives_count\x18\x07 \x01(\x04\x12 \n\x18\x63ompleted_archives_count\x18\x08 \x01(\x04\x12\x1d\n\x15\x66\x61iled_archives_count\x18\t \x01(\x04\"W\n\x10InputsDataSource\x12\x19\n\x11inputs_add_job_id\x18\x01 \x01(\t\x12(\n\x03url\x18\x02 \x01(\x0b\x32\x1b.clarifai.api.DataSourceURL\"V\n\rDataSourceURL\x12\x0b\n\x03url\x18\x01 \x01(\t\x12\x38\n\x0b\x63redentials\x18\x02 \x01(\x0b\x32#.clarifai.api.DataSourceCredentials\"\xa7\x01\n\x15\x44\x61taSourceCredentials\x12*\n\x08s3_creds\x18\x01 \x01(\x0b\x32\x16.clarifai.api.AWSCredsH\x00\x12\x13\n\tgcp_creds\x18\x02 \x01(\x0cH\x00\x12\x38\n\x10\x61zure_blob_creds\x18\x04 \x01(\x0b\x32\x1c.clarifai.api.AzureBlobCredsH\x00\x42\r\n\x0b\x63redentialsJ\x04\x08\x03\x10\x04\"K\n\x08\x41WSCreds\x12\x0e\n\x06region\x18\x02 \x01(\t\x12\n\n\x02id\x18\x03 \x01(\t\x12\x0e\n\x06secret\x18\x04 \x01(\t\x12\r\n\x05token\x18\x05 \x01(\tJ\x04\x08\x01\x10\x02\";\n\x0e\x41zureBlobCreds\x12\x14\n\x0c\x61\x63\x63ount_name\x18\x01 \x01(\t\x12\x13\n\x0b\x61\x63\x63ount_key\x18\x02 \x01(\t\"`\n\x0cInputsUpload\x12\x19\n\x11inputs_add_job_id\x18\x01 \x01(\t\x12\x0f\n\x07\x61pp_pat\x18\x02 \x01(\t\x12$\n\x06upload\x18\x03 \x01(\x0b\x32\x14.clarifai.api.Upload*\xf9\x01\n\x1e\x44\x61tasetVersionMetricsGroupType\x12.\n*DATASET_VERSION_METRICS_GROUP_TYPE_NOT_SET\x10\x00\x12\x0e\n\nINPUT_TYPE\x10\x02\x12\x0e\n\nCONCEPT_ID\x10\n\x12\x12\n\x0e\x43ONCEPTS_COUNT\x10\x0b\x12\x18\n\x14\x42OUNDING_BOXES_COUNT\x10\x14\x12\x12\n\x0ePOLYGONS_COUNT\x10\x15\x12\x10\n\x0cPOINTS_COUNT\x10\x16\x12\x0f\n\x0bMASKS_COUNT\x10\x17\x12\x10\n\x0cPIXELS_COUNT\x10\x1e\x12\x10\n\x0c\x41SPECT_RATIO\x10\x1f*\x85\x01\n\x1a\x44\x61tasetVersionExportFormat\x12)\n%DATASET_VERSION_EXPORT_FORMAT_NOT_SET\x10\x00\x12\x1a\n\x16\x43LARIFAI_DATA_PROTOBUF\x10\x01\x12\x16\n\x12\x43LARIFAI_DATA_JSON\x10\x03\x12\x08\n\x04\x43OCO\x10\x02*H\n\x10\x45xpirationAction\x12\x1d\n\x19\x45XPIRATION_ACTION_NOT_SET\x10\x00\x12\t\n\x05\x44\x45LAY\x10\x01\x12\n\n\x06\x45XPIRY\x10\x02*M\n\x0cLicenseScope\x12\x19\n\x15LICENSE_SCOPE_NOT_SET\x10\x00\x12\x0b\n\x07PREDICT\x10\x01\x12\t\n\x05TRAIN\x10\x02\x12\n\n\x06SEARCH\x10\x03*P\n\x08\x44\x61taType\x12\r\n\tUNDEFINED\x10\x00\x12\n\n\x06STRING\x10\x01\x12\t\n\x05UINT8\x10\x02\x12\t\n\x05INT32\x10\x03\x12\t\n\x05INT64\x10\x04\x12\x08\n\x04\x46P32\x10\x05*\x8f\x01\n\x0fValueComparator\x12\x1d\n\x19\x43ONCEPT_THRESHOLD_NOT_SET\x10\x00\x12\x10\n\x0cGREATER_THAN\x10\x01\x12\x19\n\x15GREATER_THAN_OR_EQUAL\x10\x02\x12\r\n\tLESS_THAN\x10\x03\x12\x16\n\x12LESS_THAN_OR_EQUAL\x10\x04\x12\t\n\x05\x45QUAL\x10\x05*q\n\x0e\x45valuationType\x12\r\n\tUndefined\x10\x00\x12\x12\n\x0e\x43lassification\x10\x01\x12\r\n\tDetection\x10\x02\x12\x10\n\x0cSegmentation\x10\x03\x12\x0e\n\nClustering\x10\x04\x12\x0b\n\x07Tracker\x10\x05*f\n\x0c\x41PIEventType\x12\x1a\n\x16\x41PI_EVENT_TYPE_NOT_SET\x10\x00\x12\x13\n\x0fON_PREM_PREDICT\x10\x01\x12\x11\n\rON_PREM_TRAIN\x10\x02\x12\x12\n\x0eON_PREM_SEARCH\x10\x03*<\n\x11UsageIntervalType\x12\t\n\x05undef\x10\x00\x12\x07\n\x03\x64\x61y\x10\x01\x12\t\n\x05month\x10\x02\x12\x08\n\x04year\x10\x03*t\n\x12\x41nnotationDataType\x12 \n\x1c\x41NNOTATION_DATA_TYPE_NOT_SET\x10\x00\x12\x10\n\x0c\x42OUNDING_BOX\x10\x01\x12\x0b\n\x07POLYGON\x10\x02\x12\t\n\x05POINT\x10\x04\x12\x08\n\x04SPAN\x10\x08\x12\x08\n\x04MASK\x10\x10*\x1d\n\x08RoleType\x12\x08\n\x04TEAM\x10\x00\x12\x07\n\x03ORG\x10\x01*$\n\x10StatValueAggType\x12\x07\n\x03SUM\x10\x00\x12\x07\n\x03\x41VG\x10\x01*`\n\x0fStatTimeAggType\x12\x0f\n\x0bNO_TIME_AGG\x10\x00\x12\x08\n\x04YEAR\x10\x01\x12\t\n\x05MONTH\x10\x02\x12\x08\n\x04WEEK\x10\x03\x12\x07\n\x03\x44\x41Y\x10\x04\x12\x08\n\x04HOUR\x10\x05\x12\n\n\x06MINUTE\x10\x06*b\n\x13ValidationErrorType\x12!\n\x1dVALIDATION_ERROR_TYPE_NOT_SET\x10\x00\x12\x0e\n\nRESTRICTED\x10\x01\x12\x0c\n\x08\x44\x41TABASE\x10\x02\x12\n\n\x06\x46ORMAT\x10\x03\x42Y\n\x15\x63om.clarifai.grpc.apiP\x01Z7github.com/Clarifai/clarifai-go-grpc/proto/clarifai/api\xa2\x02\x04\x43\x41IPb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\"proto/clarifai/api/resources.proto\x12\x0c\x63larifai.api\x1a&proto/clarifai/api/status/status.proto\x1a+proto/clarifai/api/status/status_code.proto\x1a)proto/clarifai/api/utils/extensions.proto\x1a%proto/clarifai/api/utils/matrix.proto\x1a(proto/clarifai/auth/util/extension.proto\x1a\x1cgoogle/protobuf/struct.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x1egoogle/protobuf/wrappers.proto\"\xe5\x03\n\nAnnotation\x12\n\n\x02id\x18\x01 \x01(\t\x12\x10\n\x08input_id\x18\x02 \x01(\t\x12 \n\x04\x64\x61ta\x18\x03 \x01(\x0b\x32\x12.clarifai.api.Data\x12\x30\n\x0f\x61nnotation_info\x18\r \x01(\x0b\x32\x17.google.protobuf.Struct\x12\x0f\n\x07user_id\x18\x0f \x01(\t\x12\x18\n\x10model_version_id\x18\x10 \x01(\t\x12\"\n\x16\x65mbed_model_version_id\x18\x0e \x01(\tB\x02\x18\x01\x12+\n\x06status\x18\x07 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12.\n\ncreated_at\x18\x08 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12/\n\x0bmodified_at\x18\t \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x13\n\x07trusted\x18\n \x01(\x08\x42\x02\x18\x01\x12\x13\n\x0binput_level\x18\x11 \x01(\x08\x12/\n\x0e\x63onsensus_info\x18\x12 \x01(\x0b\x32\x17.google.protobuf.Struct\x12\x0f\n\x07task_id\x18\x13 \x01(\tJ\x04\x08\x04\x10\x05J\x04\x08\x05\x10\x06J\x04\x08\x06\x10\x07J\x04\x08\x0b\x10\x0cJ\x04\x08\x0c\x10\r\"\x9c\x04\n\x03\x41pp\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x18\n\x10\x64\x65\x66\x61ult_language\x18\x03 \x01(\t\x12\x1b\n\x13\x64\x65\x66\x61ult_workflow_id\x18\x04 \x01(\t\x12\x30\n\x10\x64\x65\x66\x61ult_workflow\x18\x17 \x01(\x0b\x32\x16.clarifai.api.Workflow\x12\x0f\n\x07user_id\x18\x05 \x01(\t\x12.\n\ncreated_at\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12/\n\x0bmodified_at\x18\x11 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x1c\n\x14legal_consent_status\x18\x07 \x01(\r\x12)\n\x08metadata\x18\r \x01(\x0b\x32\x17.google.protobuf.Struct\x12\x13\n\x0b\x64\x65scription\x18\x0e \x01(\t\x12\x11\n\tsample_ms\x18\x0f \x01(\r\x12,\n\nvisibility\x18\x10 \x01(\x0b\x32\x18.clarifai.api.Visibility\x12\x14\n\x0c\x64\x61ta_tier_id\x18\x12 \x01(\t\x12\x12\n\nis_starred\x18\x13 \x01(\x08\x12\x12\n\nstar_count\x18\x14 \x01(\x05\x12\r\n\x05notes\x18\x15 \x01(\t\x12\"\n\x05image\x18\x16 \x01(\x0b\x32\x13.clarifai.api.ImageJ\x04\x08\n\x10\x0bJ\x04\x08\x0b\x10\x0cJ\x04\x08\x0c\x10\r\"\x18\n\x08\x41ppQuery\x12\x0c\n\x04name\x18\x01 \x01(\t\"\x90\x02\n\x0c\x43ollaborator\x12\n\n\x02id\x18\x01 \x01(\t\x12\x1e\n\x03\x61pp\x18\x02 \x01(\x0b\x32\x11.clarifai.api.App\x12 \n\x04user\x18\x03 \x01(\x0b\x32\x12.clarifai.api.User\x12\x0e\n\x06scopes\x18\x04 \x03(\t\x12\x11\n\tendpoints\x18\x05 \x03(\t\x12.\n\ncreated_at\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12/\n\x0bmodified_at\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12.\n\ndeleted_at\x18\x08 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"\xa9\x01\n\rCollaboration\x12\x1e\n\x03\x61pp\x18\x01 \x01(\x0b\x32\x11.clarifai.api.App\x12%\n\tapp_owner\x18\x02 \x01(\x0b\x32\x12.clarifai.api.User\x12\x0e\n\x06scopes\x18\x03 \x03(\t\x12\x11\n\tendpoints\x18\x04 \x03(\t\x12.\n\ncreated_at\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"\x97\x01\n\x05\x41udio\x12\x0b\n\x03url\x18\x01 \x01(\t\x12\x0e\n\x06\x62\x61se64\x18\x02 \x01(\x0c\x12\x1b\n\x13\x61llow_duplicate_url\x18\x04 \x01(\x08\x12\'\n\x06hosted\x18\x05 \x01(\x0b\x32\x17.clarifai.api.HostedURL\x12+\n\naudio_info\x18\x06 \x01(\x0b\x32\x17.clarifai.api.AudioInfo\"b\n\tAudioInfo\x12\x14\n\x0c\x61udio_format\x18\x01 \x01(\t\x12\x13\n\x0bsample_rate\x18\x02 \x01(\x05\x12\x18\n\x10\x64uration_seconds\x18\x03 \x01(\x02\x12\x10\n\x08\x62it_rate\x18\x04 \x01(\x05\"w\n\x05Track\x12\n\n\x02id\x18\x01 \x01(\t\x12 \n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x12.clarifai.api.Data\x12)\n\ttime_info\x18\x04 \x01(\x0b\x32\x16.clarifai.api.TimeInfo\x12\x0f\n\x07quality\x18\x05 \x01(\x02J\x04\x08\x03\x10\x04\"h\n\x07\x43luster\x12\n\n\x02id\x18\x01 \x01(\t\x12\r\n\x05\x63ount\x18\x02 \x01(\r\x12\r\n\x05score\x18\x03 \x01(\x02\x12\x1f\n\x04hits\x18\x04 \x03(\x0b\x32\x11.clarifai.api.Hit\x12\x12\n\nprojection\x18\x05 \x03(\x02\"M\n\x05\x43olor\x12\x0f\n\x07raw_hex\x18\x01 \x01(\t\x12\x1e\n\x03w3c\x18\x02 \x01(\x0b\x32\x11.clarifai.api.W3C\x12\x13\n\x05value\x18\x03 \x01(\x02\x42\x04\x80\xb5\x18\x01\" \n\x03W3C\x12\x0b\n\x03hex\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\"/\n\x0cUserAppIDSet\x12\x0f\n\x07user_id\x18\x01 \x01(\t\x12\x0e\n\x06\x61pp_id\x18\x02 \x01(\t\"J\n\x0bPatchAction\x12\n\n\x02op\x18\x01 \x01(\t\x12!\n\x19merge_conflict_resolution\x18\x02 \x01(\t\x12\x0c\n\x04path\x18\x03 \x01(\t\"\xa9\x02\n\x07\x43oncept\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x1a\n\x05value\x18\x03 \x01(\x02\x42\x0b\xd5\xb5\x18\x00\x00\x80?\x80\xb5\x18\x01\x12.\n\ncreated_at\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x10\n\x08language\x18\x05 \x01(\t\x12\x0e\n\x06\x61pp_id\x18\x06 \x01(\t\x12\x12\n\ndefinition\x18\x07 \x01(\t\x12\x10\n\x08vocab_id\x18\x08 \x01(\t\x12,\n\nvisibility\x18\t \x01(\x0b\x32\x18.clarifai.api.Visibility\x12\x0f\n\x07user_id\x18\n \x01(\t\x12\x31\n\rkeypoint_info\x18\x0b \x01(\x0b\x32\x1a.clarifai.api.KeypointInfo\"T\n\x0cKeypointInfo\x12\x16\n\x0ekeypoint_names\x18\x01 \x03(\t\x12,\n\x08skeleton\x18\x02 \x03(\x0b\x32\x1a.clarifai.api.KeypointEdge\"&\n\x0cKeypointEdge\x12\n\n\x02k1\x18\x01 \x01(\r\x12\n\n\x02k2\x18\x02 \x01(\r\"\xa4\x01\n\x0c\x43onceptCount\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12:\n\x12\x63oncept_type_count\x18\x03 \x01(\x0b\x32\x1e.clarifai.api.ConceptTypeCount\x12>\n\x14\x64\x65tail_concept_count\x18\x04 \x01(\x0b\x32 .clarifai.api.DetailConceptCount\"B\n\x10\x43onceptTypeCount\x12\x16\n\x08positive\x18\x01 \x01(\rB\x04\x80\xb5\x18\x01\x12\x16\n\x08negative\x18\x02 \x01(\rB\x04\x80\xb5\x18\x01\"\xdf\x01\n\x12\x44\x65tailConceptCount\x12\x31\n\tprocessed\x18\x01 \x01(\x0b\x32\x1e.clarifai.api.ConceptTypeCount\x12\x32\n\nto_process\x18\x02 \x01(\x0b\x32\x1e.clarifai.api.ConceptTypeCount\x12.\n\x06\x65rrors\x18\x03 \x01(\x0b\x32\x1e.clarifai.api.ConceptTypeCount\x12\x32\n\nprocessing\x18\x04 \x01(\x0b\x32\x1e.clarifai.api.ConceptTypeCount\"C\n\x0c\x43onceptQuery\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x10\n\x08language\x18\x02 \x01(\t\x12\x13\n\x0bworkflow_id\x18\x03 \x01(\t\"\xd9\x01\n\x0f\x43onceptRelation\x12\n\n\x02id\x18\x01 \x01(\t\x12.\n\x0fsubject_concept\x18\x02 \x01(\x0b\x32\x15.clarifai.api.Concept\x12-\n\x0eobject_concept\x18\x03 \x01(\x0b\x32\x15.clarifai.api.Concept\x12\x11\n\tpredicate\x18\x04 \x01(\t\x12\x1a\n\x12knowledge_graph_id\x18\x05 \x01(\t\x12,\n\nvisibility\x18\x06 \x01(\x0b\x32\x18.clarifai.api.Visibility\"y\n\x0eKnowledgeGraph\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x03 \x01(\t\x12\x17\n\x0f\x65xamples_app_id\x18\x04 \x01(\t\x12\x1f\n\x17sampled_examples_app_id\x18\x05 \x01(\t\"D\n\x11\x43onceptMappingJob\x12\x1a\n\x12knowledge_graph_id\x18\x01 \x01(\t\x12\x13\n\x0b\x63oncept_ids\x18\x02 \x03(\t\"?\n\x0f\x43onceptLanguage\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x12\n\ndefinition\x18\x03 \x01(\t\"\xfa\x04\n\x04\x44\x61ta\x12\"\n\x05image\x18\x01 \x01(\x0b\x32\x13.clarifai.api.Image\x12\"\n\x05video\x18\x02 \x01(\x0b\x32\x13.clarifai.api.Video\x12\'\n\x08\x63oncepts\x18\x03 \x03(\x0b\x32\x15.clarifai.api.Concept\x12)\n\x08metadata\x18\x05 \x01(\x0b\x32\x17.google.protobuf.Struct\x12\x1e\n\x03geo\x18\x06 \x01(\x0b\x32\x11.clarifai.api.Geo\x12#\n\x06\x63olors\x18\x07 \x03(\x0b\x32\x13.clarifai.api.Color\x12\'\n\x08\x63lusters\x18\x08 \x03(\x0b\x32\x15.clarifai.api.Cluster\x12+\n\nembeddings\x18\t \x03(\x0b\x32\x17.clarifai.api.Embedding\x12%\n\x07regions\x18\x0b \x03(\x0b\x32\x14.clarifai.api.Region\x12#\n\x06\x66rames\x18\x0c \x03(\x0b\x32\x13.clarifai.api.Frame\x12 \n\x04text\x18\r \x01(\x0b\x32\x12.clarifai.api.Text\x12\"\n\x05\x61udio\x18\x0e \x01(\x0b\x32\x13.clarifai.api.Audio\x12#\n\x06tracks\x18\x0f \x03(\x0b\x32\x13.clarifai.api.Track\x12\x30\n\rtime_segments\x18\x10 \x03(\x0b\x32\x19.clarifai.api.TimeSegment\x12\x1f\n\x04hits\x18\x11 \x03(\x0b\x32\x11.clarifai.api.Hit\x12%\n\x08heatmaps\x18\x12 \x03(\x0b\x32\x13.clarifai.api.ImageJ\x04\x08\x04\x10\x05J\x04\x08\n\x10\x0b\"\x86\x01\n\x06Region\x12\n\n\x02id\x18\x01 \x01(\t\x12-\n\x0bregion_info\x18\x02 \x01(\x0b\x32\x18.clarifai.api.RegionInfo\x12 \n\x04\x64\x61ta\x18\x03 \x01(\x0b\x32\x12.clarifai.api.Data\x12\r\n\x05value\x18\x04 \x01(\x02\x12\x10\n\x08track_id\x18\x05 \x01(\t\"\xae\x02\n\nRegionInfo\x12/\n\x0c\x62ounding_box\x18\x01 \x01(\x0b\x32\x19.clarifai.api.BoundingBox\x12 \n\x04mask\x18\x04 \x01(\x0b\x32\x12.clarifai.api.Mask\x12&\n\x07polygon\x18\x05 \x01(\x0b\x32\x15.clarifai.api.Polygon\x12\"\n\x05point\x18\x06 \x01(\x0b\x32\x13.clarifai.api.Point\x12 \n\x04span\x18\x07 \x01(\x0b\x32\x12.clarifai.api.Span\x12\"\n\x05token\x18\x08 \x01(\x0b\x32\x13.clarifai.api.Token\x12/\n\x12keypoint_locations\x18\t \x03(\x0b\x32\x13.clarifai.api.PointJ\x04\x08\x02\x10\x03J\x04\x08\x03\x10\x04\"o\n\x0b\x42oundingBox\x12\x15\n\x07top_row\x18\x01 \x01(\x02\x42\x04\x80\xb5\x18\x01\x12\x16\n\x08left_col\x18\x02 \x01(\x02\x42\x04\x80\xb5\x18\x01\x12\x18\n\nbottom_row\x18\x03 \x01(\x02\x42\x04\x80\xb5\x18\x01\x12\x17\n\tright_col\x18\x04 \x01(\x02\x42\x04\x80\xb5\x18\x01\"4\n\tFrameInfo\x12\x13\n\x05index\x18\x01 \x01(\rB\x04\x80\xb5\x18\x01\x12\x12\n\x04time\x18\x02 \x01(\rB\x04\x80\xb5\x18\x01\"b\n\x05\x46rame\x12+\n\nframe_info\x18\x01 \x01(\x0b\x32\x17.clarifai.api.FrameInfo\x12 \n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x12.clarifai.api.Data\x12\n\n\x02id\x18\x03 \x01(\t\"0\n\x04Mask\x12\"\n\x05image\x18\x02 \x01(\x0b\x32\x13.clarifai.api.ImageJ\x04\x08\x01\x10\x02\".\n\x07Polygon\x12#\n\x06points\x18\x01 \x03(\x0b\x32\x13.clarifai.api.Point\"\xb6\x01\n\x05Point\x12\x11\n\x03row\x18\x01 \x01(\x02\x42\x04\x80\xb5\x18\x01\x12\x11\n\x03\x63ol\x18\x02 \x01(\x02\x42\x04\x80\xb5\x18\x01\x12\t\n\x01z\x18\x03 \x01(\x02\x12\x32\n\nvisibility\x18\x04 \x01(\x0e\x32\x1e.clarifai.api.Point.Visibility\"H\n\nVisibility\x12\x0b\n\x07NOT_SET\x10\x00\x12\x0b\n\x07VISIBLE\x10\x01\x12\x0f\n\x0bNOT_VISIBLE\x10\x02\x12\x0f\n\x0bNOT_PRESENT\x10\x03\"J\n\x04Span\x12\x18\n\nchar_start\x18\x01 \x01(\rB\x04\x80\xb5\x18\x01\x12\x16\n\x08\x63har_end\x18\x02 \x01(\rB\x04\x80\xb5\x18\x01\x12\x10\n\x08raw_text\x18\x03 \x01(\t\"K\n\x05Token\x12\x18\n\nchar_start\x18\x01 \x01(\rB\x04\x80\xb5\x18\x01\x12\x16\n\x08\x63har_end\x18\x02 \x01(\rB\x04\x80\xb5\x18\x01\x12\x10\n\x08raw_text\x18\x03 \x01(\t\"7\n\tEmbedding\x12\x12\n\x06vector\x18\x01 \x03(\x02\x42\x02\x10\x01\x12\x16\n\x0enum_dimensions\x18\x02 \x01(\r\";\n\x08GeoPoint\x12\x17\n\tlongitude\x18\x01 \x01(\x02\x42\x04\x80\xb5\x18\x01\x12\x16\n\x08latitude\x18\x02 \x01(\x02\x42\x04\x80\xb5\x18\x01\"-\n\x08GeoLimit\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x13\n\x05value\x18\x02 \x01(\x02\x42\x04\x80\xb5\x18\x01\":\n\rGeoBoxedPoint\x12)\n\tgeo_point\x18\x01 \x01(\x0b\x32\x16.clarifai.api.GeoPoint\"\x89\x01\n\x03Geo\x12)\n\tgeo_point\x18\x01 \x01(\x0b\x32\x16.clarifai.api.GeoPoint\x12)\n\tgeo_limit\x18\x02 \x01(\x0b\x32\x16.clarifai.api.GeoLimit\x12,\n\x07geo_box\x18\x03 \x03(\x0b\x32\x1b.clarifai.api.GeoBoxedPoint\"\x9d\x01\n\x05Image\x12\x0b\n\x03url\x18\x01 \x01(\t\x12\x0e\n\x06\x62\x61se64\x18\x02 \x01(\x0c\x12\x1b\n\x13\x61llow_duplicate_url\x18\x04 \x01(\x08\x12\'\n\x06hosted\x18\x05 \x01(\x0b\x32\x17.clarifai.api.HostedURL\x12+\n\nimage_info\x18\x06 \x01(\x0b\x32\x17.clarifai.api.ImageInfoJ\x04\x08\x03\x10\x04\"N\n\tImageInfo\x12\r\n\x05width\x18\x01 \x01(\x05\x12\x0e\n\x06height\x18\x02 \x01(\x05\x12\x0e\n\x06\x66ormat\x18\x03 \x01(\t\x12\x12\n\ncolor_mode\x18\x04 \x01(\t\"O\n\tHostedURL\x12\x0e\n\x06prefix\x18\x01 \x01(\t\x12\x0e\n\x06suffix\x18\x02 \x01(\t\x12\r\n\x05sizes\x18\x03 \x03(\t\x12\x13\n\x0b\x63rossorigin\x18\x04 \x01(\t\"\xde\x01\n\x05Input\x12\n\n\x02id\x18\x01 \x01(\t\x12 \n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x12.clarifai.api.Data\x12.\n\ncreated_at\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12/\n\x0bmodified_at\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12+\n\x06status\x18\x06 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x13\n\x0b\x64\x61taset_ids\x18\x07 \x03(\tJ\x04\x08\x03\x10\x04\"1\n\nInputBatch\x12#\n\x06inputs\x18\x01 \x03(\x0b\x32\x13.clarifai.api.Input\"\xda\x01\n\nInputCount\x12\x17\n\tprocessed\x18\x01 \x01(\rB\x04\x80\xb5\x18\x01\x12\x18\n\nto_process\x18\x02 \x01(\rB\x04\x80\xb5\x18\x01\x12\x14\n\x06\x65rrors\x18\x03 \x01(\rB\x04\x80\xb5\x18\x01\x12\x18\n\nprocessing\x18\x04 \x01(\rB\x04\x80\xb5\x18\x01\x12\x17\n\treindexed\x18\x05 \x01(\rB\x04\x80\xb5\x18\x01\x12\x18\n\nto_reindex\x18\x06 \x01(\rB\x04\x80\xb5\x18\x01\x12\x1c\n\x0ereindex_errors\x18\x07 \x01(\rB\x04\x80\xb5\x18\x01\x12\x18\n\nreindexing\x18\x08 \x01(\rB\x04\x80\xb5\x18\x01\"\xba\x03\n\x07\x44\x61taset\x12\n\n\x02id\x18\x01 \x01(\t\x12.\n\ncreated_at\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12/\n\x0bmodified_at\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x0e\n\x06\x61pp_id\x18\x04 \x01(\t\x12\x0f\n\x07user_id\x18\x05 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x07 \x01(\t\x12)\n\x08metadata\x18\x08 \x01(\x0b\x32\x17.google.protobuf.Struct\x12,\n\nvisibility\x18\t \x01(\x0b\x32\x18.clarifai.api.Visibility\x12\x41\n\x19\x64\x65\x66\x61ult_annotation_filter\x18\x0c \x01(\x0b\x32\x1e.clarifai.api.AnnotationFilter\x12\r\n\x05notes\x18\x0b \x01(\t\x12-\n\x07version\x18\r \x01(\x0b\x32\x1c.clarifai.api.DatasetVersion\x12\x12\n\nis_starred\x18\x0e \x01(\x08\x12\x12\n\nstar_count\x18\x0f \x01(\x05J\x04\x08\x06\x10\x07J\x04\x08\n\x10\x0b\"\xd8\x01\n\x10\x41nnotationFilter\x12\n\n\x02id\x18\x01 \x01(\t\x12.\n\ncreated_at\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12/\n\x0bmodified_at\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x0f\n\x07user_id\x18\x04 \x01(\t\x12\x0e\n\x06\x61pp_id\x18\x05 \x01(\t\x12*\n\x0csaved_search\x18\x08 \x01(\x0b\x32\x14.clarifai.api.SearchJ\x04\x08\x06\x10\x07J\x04\x08\x07\x10\x08\"b\n\x0c\x44\x61tasetInput\x12.\n\ncreated_at\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\"\n\x05input\x18\x02 \x01(\x0b\x32\x13.clarifai.api.Input\"\xae\x06\n\x0e\x44\x61tasetVersion\x12\n\n\x02id\x18\x01 \x01(\t\x12.\n\ncreated_at\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12/\n\x0bmodified_at\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x0e\n\x06\x61pp_id\x18\x04 \x01(\t\x12\x0f\n\x07user_id\x18\x05 \x01(\t\x12\x12\n\ndataset_id\x18\x06 \x01(\t\x12H\n\x18\x61nnotation_filter_config\x18\x0f \x01(\x0b\x32$.clarifai.api.AnnotationFilterConfigH\x00\x12@\n\x14model_predict_config\x18\x12 \x01(\x0b\x32 .clarifai.api.ModelPredictConfigH\x00\x12+\n\x06status\x18\x08 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x13\n\x0b\x64\x65scription\x18\n \x01(\t\x12\x43\n\x0fprocessing_info\x18\x13 \x01(\x0b\x32*.clarifai.api.DatasetVersionProcessingInfo\x12:\n\x07metrics\x18\x10 \x03(\x0b\x32).clarifai.api.DatasetVersion.MetricsEntry\x12;\n\x0b\x65xport_info\x18\x11 \x01(\x0b\x32&.clarifai.api.DatasetVersionExportInfo\x12)\n\x08metadata\x18\x0c \x01(\x0b\x32\x17.google.protobuf.Struct\x12,\n\nvisibility\x18\r \x01(\x0b\x32\x18.clarifai.api.Visibility\x12\x1f\n\x17\x65mbed_model_version_ids\x18\x0e \x03(\t\x1aS\n\x0cMetricsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x32\n\x05value\x18\x02 \x01(\x0b\x32#.clarifai.api.DatasetVersionMetrics:\x02\x38\x01\x42\r\n\x0b\x64\x61ta_configJ\x04\x08\x07\x10\x08J\x04\x08\t\x10\nJ\x04\x08\x0b\x10\x0c\"p\n\x16\x41nnotationFilterConfig\x12\x39\n\x11\x61nnotation_filter\x18\x01 \x01(\x0b\x32\x1e.clarifai.api.AnnotationFilter\x12\x1b\n\x13ignore_empty_inputs\x18\x02 \x01(\x08\"8\n\x12ModelPredictConfig\x12\"\n\x05model\x18\x01 \x01(\x0b\x32\x13.clarifai.api.Model\"\xc3\x08\n\x15\x44\x61tasetVersionMetrics\x12\x32\n\x0cinputs_count\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.UInt64Value\x12<\n\x16unlabeled_inputs_count\x18\x06 \x01(\x0b\x32\x1c.google.protobuf.UInt64Value\x12@\n\x1ainputs_with_metadata_count\x18\x08 \x01(\x0b\x32\x1c.google.protobuf.UInt64Value\x12;\n\x15inputs_with_geo_count\x18\t \x01(\x0b\x32\x1c.google.protobuf.UInt64Value\x12\x33\n\rregions_count\x18\x14 \x01(\x0b\x32\x1c.google.protobuf.UInt64Value\x12-\n\x16region_location_matrix\x18\x15 \x01(\x0b\x32\r.MatrixUint64\x12:\n\x14\x62ounding_boxes_count\x18\x16 \x01(\x0b\x32\x1c.google.protobuf.UInt64Value\x12\x34\n\x0epolygons_count\x18\x17 \x01(\x0b\x32\x1c.google.protobuf.UInt64Value\x12\x32\n\x0cpoints_count\x18\x18 \x01(\x0b\x32\x1c.google.protobuf.UInt64Value\x12\x31\n\x0bmasks_count\x18\x19 \x01(\x0b\x32\x1c.google.protobuf.UInt64Value\x12\x39\n\x13region_inputs_count\x18< \x01(\x0b\x32\x1c.google.protobuf.UInt64Value\x12\x39\n\x13region_frames_count\x18= \x01(\x0b\x32\x1c.google.protobuf.UInt64Value\x12\x32\n\x0c\x66rames_count\x18\x1e \x01(\x0b\x32\x1c.google.protobuf.UInt64Value\x12\x38\n\x12\x66rame_inputs_count\x18\x46 \x01(\x0b\x32\x1c.google.protobuf.UInt64Value\x12\x36\n\x10\x65mbeddings_count\x18( \x01(\x0b\x32\x1c.google.protobuf.UInt64Value\x12?\n\x19positive_input_tags_count\x18\x32 \x01(\x0b\x32\x1c.google.protobuf.UInt64Value\x12@\n\x1apositive_region_tags_count\x18\x33 \x01(\x0b\x32\x1c.google.protobuf.UInt64Value\x12?\n\x19positive_frame_tags_count\x18\x34 \x01(\x0b\x32\x1c.google.protobuf.UInt64ValueJ\x04\x08\x02\x10\x03J\x04\x08\x03\x10\x04J\x04\x08\x04\x10\x05J\x04\x08\x05\x10\x06J\x04\x08\x07\x10\x08\"\xca\x01\n\x1a\x44\x61tasetVersionMetricsGroup\x12\x13\n\x0bparent_path\x18\x01 \x01(\t\x12:\n\x04type\x18\x02 \x01(\x0e\x32,.clarifai.api.DatasetVersionMetricsGroupType\x12%\n\x05value\x18\x03 \x01(\x0b\x32\x16.google.protobuf.Value\x12\x34\n\x07metrics\x18\x04 \x01(\x0b\x32#.clarifai.api.DatasetVersionMetrics\"\xd0\x01\n\x18\x44\x61tasetVersionExportInfo\x12\x42\n\x16\x63larifai_data_protobuf\x18\x01 \x01(\x0b\x32\".clarifai.api.DatasetVersionExport\x12>\n\x12\x63larifai_data_json\x18\x03 \x01(\x0b\x32\".clarifai.api.DatasetVersionExport\x12\x30\n\x04\x63oco\x18\x02 \x01(\x0b\x32\".clarifai.api.DatasetVersionExport\"\xb4\x01\n\x14\x44\x61tasetVersionExport\x12\x38\n\x06\x66ormat\x18\x01 \x01(\x0e\x32(.clarifai.api.DatasetVersionExportFormat\x12+\n\x06status\x18\x02 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x0b\n\x03url\x18\x03 \x01(\t\x12\x0c\n\x04size\x18\x04 \x01(\x04\x12\x1a\n\x12include_embeddings\x18\x05 \x01(\x08\"f\n\x1c\x44\x61tasetVersionProcessingInfo\x12\x46\n\x18\x66rame_interpolation_info\x18\x01 \x01(\x0b\x32$.clarifai.api.FrameInterpolationInfo\"+\n\x16\x46rameInterpolationInfo\x12\x11\n\tsample_ms\x18\x01 \x01(\r\"n\n\x19WorkflowResultsSimilarity\x12(\n\x0bprobe_input\x18\x01 \x01(\x0b\x32\x13.clarifai.api.Input\x12\'\n\x0cpool_results\x18\x02 \x03(\x0b\x32\x11.clarifai.api.Hit\"\xf4\x01\n\x03Key\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x04type\x18\x08 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\x0e\n\x06scopes\x18\x03 \x03(\t\x12\x11\n\tendpoints\x18\x07 \x03(\t\x12\x1f\n\x04\x61pps\x18\x04 \x03(\x0b\x32\x11.clarifai.api.App\x12.\n\ncreated_at\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12.\n\nexpires_at\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x1a\n\x12\x61uthorized_idp_ids\x18\t \x03(\t\"\xd8\x07\n\x05Model\x12\n\n\x02id\x18\x01 \x01(\t\x12\x10\n\x04name\x18\x02 \x01(\tB\x02\x18\x01\x12.\n\ncreated_at\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12/\n\x0bmodified_at\x18\x13 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x14\n\x06\x61pp_id\x18\x04 \x01(\tB\x04\x80\xb5\x18\x01\x12\x31\n\x0boutput_info\x18\x05 \x01(\x0b\x32\x18.clarifai.api.OutputInfoB\x02\x18\x01\x12\x31\n\rmodel_version\x18\x06 \x01(\x0b\x32\x1a.clarifai.api.ModelVersion\x12\x18\n\x0c\x64isplay_name\x18\x07 \x01(\tB\x02\x18\x01\x12\x0f\n\x07user_id\x18\t \x01(\t\x12/\n\ninput_info\x18\x0c \x01(\x0b\x32\x17.clarifai.api.InputInfoB\x02\x18\x01\x12/\n\ntrain_info\x18\r \x01(\x0b\x32\x17.clarifai.api.TrainInfoB\x02\x18\x01\x12\x31\n\x11\x64\x65\x66\x61ult_eval_info\x18\x1e \x01(\x0b\x32\x16.clarifai.api.EvalInfo\x12\x15\n\rmodel_type_id\x18\x0e \x01(\t\x12\x0c\n\x04task\x18\x1a \x01(\t\x12,\n\nvisibility\x18\x0f \x01(\x0b\x32\x18.clarifai.api.Visibility\x12\x13\n\x0b\x64\x65scription\x18\x10 \x01(\t\x12)\n\x08metadata\x18\x11 \x01(\x0b\x32\x17.google.protobuf.Struct\x12(\n\x07presets\x18\x1b \x01(\x0b\x32\x17.google.protobuf.Struct\x12\r\n\x05notes\x18\x12 \x01(\t\x12\x16\n\x08toolkits\x18\x14 \x03(\tB\x04\x80\xb5\x18\x01\x12\x17\n\tuse_cases\x18\x15 \x03(\tB\x04\x80\xb5\x18\x01\x12\x17\n\tlanguages\x18\x19 \x03(\tB\x04\x80\xb5\x18\x01\x12\x33\n\x0elanguages_full\x18\x1f \x03(\x0b\x32\x15.clarifai.api.FullTagB\x04\x80\xb5\x18\x01\x12\x1c\n\x0e\x63heck_consents\x18  \x03(\tB\x04\x80\xb5\x18\x01\x12\x12\n\nis_starred\x18\x16 \x01(\x08\x12\x12\n\nstar_count\x18\x17 \x01(\x05\x12\x31\n\x0bimport_info\x18\x18 \x01(\x0b\x32\x18.clarifai.api.ImportInfoB\x02\x18\x01\x12\x38\n\x14workflow_recommended\x18\x1d \x01(\x0b\x32\x1a.google.protobuf.BoolValueJ\x04\x08\x08\x10\tJ\x04\x08\n\x10\x0bJ\x04\x08\x0b\x10\x0cJ\x04\x08\x1c\x10\x1d\"t\n\x0eModelReference\x12\n\n\x02id\x18\x01 \x01(\t\x12\x10\n\x08model_id\x18\x02 \x01(\t\x12\x0b\n\x03url\x18\x03 \x01(\t\x12\x0c\n\x04name\x18\x04 \x01(\t\x12)\n\x08metadata\x18\x05 \x01(\x0b\x32\x17.google.protobuf.Struct\"\x97\x01\n\x18ModelVersionInputExample\x12\n\n\x02id\x18\x01 \x01(\t\x12\x10\n\x08model_id\x18\x02 \x01(\t\x12\x18\n\x10model_version_id\x18\x03 \x01(\t\x12 \n\x04\x64\x61ta\x18\x04 \x01(\x0b\x32\x12.clarifai.api.Data\x12\x0c\n\x04name\x18\x05 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x06 \x01(\t\"\xd4\x01\n\nOutputInfo\x12 \n\x04\x64\x61ta\x18\x01 \x01(\x0b\x32\x12.clarifai.api.Data\x12\x31\n\routput_config\x18\x02 \x01(\x0b\x32\x1a.clarifai.api.OutputConfig\x12\x0f\n\x07message\x18\x03 \x01(\t\x12+\n\nfields_map\x18\x06 \x01(\x0b\x32\x17.google.protobuf.Struct\x12\'\n\x06params\x18\x07 \x01(\x0b\x32\x17.google.protobuf.StructJ\x04\x08\x04\x10\x05J\x04\x08\x05\x10\x06\"a\n\tInputInfo\x12+\n\nfields_map\x18\x01 \x01(\x0b\x32\x17.google.protobuf.Struct\x12\'\n\x06params\x18\x02 \x01(\x0b\x32\x17.google.protobuf.Struct\"4\n\tTrainInfo\x12\'\n\x06params\x18\x01 \x01(\x0b\x32\x17.google.protobuf.Struct\"3\n\x08\x45valInfo\x12\'\n\x06params\x18\x01 \x01(\x0b\x32\x17.google.protobuf.Struct\"5\n\nImportInfo\x12\'\n\x06params\x18\x01 \x01(\x0b\x32\x17.google.protobuf.Struct\"\xdf\x03\n\x0cOutputConfig\x12\'\n\x1b\x63oncepts_mutually_exclusive\x18\x01 \x01(\x08\x42\x02\x18\x01\x12\x1d\n\x11\x65xisting_model_id\x18\x03 \x01(\tB\x02\x18\x01\x12\x10\n\x08language\x18\x04 \x01(\t\x12\x1c\n\x10hyper_parameters\x18\x05 \x01(\tB\x02\x18\x01\x12\x1a\n\x0cmax_concepts\x18\x06 \x01(\rB\x04\x80\xb5\x18\x01\x12\x17\n\tmin_value\x18\x07 \x01(\x02\x42\x04\x80\xb5\x18\x01\x12.\n\x0fselect_concepts\x18\x08 \x03(\x0b\x32\x15.clarifai.api.Concept\x12\x18\n\x10training_timeout\x18\t \x01(\r\x12\x11\n\tsample_ms\x18\n \x01(\r\x12-\n\x0chyper_params\x18\r \x01(\x0b\x32\x17.google.protobuf.Struct\x12\x1e\n\x16\x65mbed_model_version_id\x18\x0e \x01(\t\x12)\n!fail_on_missing_positive_examples\x18\x0f \x01(\x08\x12\x33\n\x0emodel_metadata\x18\x11 \x01(\x0b\x32\x17.google.protobuf.StructB\x02\x18\x01J\x04\x08\x0b\x10\x0cJ\x04\x08\x0c\x10\rJ\x04\x08\x10\x10\x11J\x04\x08\x12\x10\x13\"\xd2\x03\n\tModelType\x12\n\n\x02id\x18\x01 \x01(\t\x12\r\n\x05title\x18\x02 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x03 \x01(\t\x12\x14\n\x0cinput_fields\x18\x05 \x03(\t\x12\x15\n\routput_fields\x18\x06 \x03(\t\x12\x11\n\ttrainable\x18\x08 \x01(\x08\x12\x11\n\tcreatable\x18\t \x01(\x08\x12\x15\n\rinternal_only\x18\n \x01(\x08\x12\x37\n\x11model_type_fields\x18\x0b \x03(\x0b\x32\x1c.clarifai.api.ModelTypeField\x12\"\n\x1arequires_sequential_frames\x18\x0c \x01(\x08\x12;\n\x15\x65xpected_input_layers\x18\x10 \x03(\x0b\x32\x1c.clarifai.api.ModelLayerInfo\x12<\n\x16\x65xpected_output_layers\x18\x11 \x03(\x0b\x32\x1c.clarifai.api.ModelLayerInfo\x12\x35\n\x0f\x65valuation_type\x18\x12 \x01(\x0e\x32\x1c.clarifai.api.EvaluationTypeJ\x04\x08\x07\x10\x08J\x04\x08\x04\x10\x05J\x04\x08\r\x10\x0eJ\x04\x08\x0e\x10\x0fJ\x04\x08\x0f\x10\x10\"\x89\x01\n\x0eModelLayerInfo\x12\x17\n\x0f\x64\x61ta_field_name\x18\x01 \x01(\t\x12(\n\x06shapes\x18\x02 \x03(\x0b\x32\x18.clarifai.api.LayerShape\x12\x13\n\x0b\x64\x65scription\x18\x03 \x01(\t\x12\x1f\n\x17requires_label_filename\x18\x04 \x01(\x08\"D\n\x12TritonCondaEnvInfo\x12\x16\n\x0e\x63onda_pack_url\x18\x01 \x01(\t\x12\x16\n\x0e\x63onda_yaml_url\x18\x02 \x01(\t\"l\n\nLayerShape\x12\x0c\n\x04\x64ims\x18\x01 \x03(\x05\x12\x10\n\x08max_dims\x18\x02 \x03(\x05\x12)\n\tdata_type\x18\x03 \x01(\x0e\x32\x16.clarifai.api.DataType\x12\x13\n\x0b\x64\x65scription\x18\x04 \x01(\t\"\xd2\x05\n\x0eModelTypeField\x12\x0c\n\x04path\x18\x01 \x01(\t\x12\x43\n\nfield_type\x18\x02 \x01(\x0e\x32/.clarifai.api.ModelTypeField.ModelTypeFieldType\x12-\n\rdefault_value\x18\x03 \x01(\x0b\x32\x16.google.protobuf.Value\x12\x13\n\x0b\x64\x65scription\x18\x04 \x01(\t\x12\x13\n\x0bplaceholder\x18\x05 \x01(\t\x12\x42\n\x17model_type_enum_options\x18\x06 \x03(\x0b\x32!.clarifai.api.ModelTypeEnumOption\x12\x15\n\rinternal_only\x18\x07 \x01(\x08\x12\x10\n\x08required\x18\x08 \x01(\x08\x12?\n\x15model_type_range_info\x18\t \x01(\x0b\x32 .clarifai.api.ModelTypeRangeInfo\"\xe5\x02\n\x12ModelTypeFieldType\x12!\n\x1dINVALID_MODEL_TYPE_FIELD_TYPE\x10\x00\x12\x0b\n\x07\x42OOLEAN\x10\x01\x12\n\n\x06STRING\x10\x02\x12\n\n\x06NUMBER\x10\x03\x12\x15\n\x11\x41RRAY_OF_CONCEPTS\x10\x04\x12$\n ARRAY_OF_CONCEPTS_WITH_THRESHOLD\x10\x05\x12\t\n\x05RANGE\x10\x07\x12\x08\n\x04\x45NUM\x10\x08\x12\x11\n\rCOLLABORATORS\x10\t\x12\x08\n\x04JSON\x10\n\x12\x14\n\x10\x41RRAY_OF_NUMBERS\x10\x0b\x12\x19\n\x15WORKFLOW_EMBED_MODELS\x10\x0c\x12\x14\n\x10\x41RRAY_OF_STRINGS\x10\r\x12\x12\n\x0eRECURSIVE_ENUM\x10\x0e\x12\x0f\n\x0bPYTHON_CODE\x10\x0f\x12\x0e\n\nDATASET_ID\x10\x10\x12\x16\n\x12\x44\x41TASET_VERSION_ID\x10\x11\"\x04\x08\x06\x10\x06\"<\n\x12ModelTypeRangeInfo\x12\x0b\n\x03min\x18\x01 \x01(\x02\x12\x0b\n\x03max\x18\x02 \x01(\x02\x12\x0c\n\x04step\x18\x03 \x01(\x02\"\xd4\x01\n\x13ModelTypeEnumOption\x12\n\n\x02id\x18\x01 \x01(\t\x12\x37\n\x07\x61liases\x18\x05 \x03(\x0b\x32&.clarifai.api.ModelTypeEnumOptionAlias\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\x37\n\x11model_type_fields\x18\x03 \x03(\x0b\x32\x1c.clarifai.api.ModelTypeField\x12\x15\n\rinternal_only\x18\x04 \x01(\x08\x12\x13\n\x0brecommended\x18\x06 \x01(\x08\"C\n\x18ModelTypeEnumOptionAlias\x12\x0e\n\x06id_int\x18\x01 \x01(\x03\x12\x17\n\x0fwildcard_string\x18\x02 \x01(\t\"7\n\nModelQuery\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x15\n\rmodel_type_id\x18\x03 \x01(\tJ\x04\x08\x02\x10\x03\"\xfc\x05\n\x0cModelVersion\x12\n\n\x02id\x18\x01 \x01(\t\x12.\n\ncreated_at\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12+\n\x06status\x18\x03 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x1c\n\x14\x61\x63tive_concept_count\x18\x04 \x01(\r\x12*\n\x07metrics\x18\x05 \x01(\x0b\x32\x19.clarifai.api.EvalMetrics\x12\x19\n\x11total_input_count\x18\x06 \x01(\r\x12\x44\n\x17pretrained_model_config\x18\x07 \x01(\x0b\x32#.clarifai.api.PretrainedModelConfig\x12\x30\n\x0c\x63ompleted_at\x18\n \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x13\n\x0b\x64\x65scription\x18\x0b \x01(\t\x12,\n\nvisibility\x18\x0c \x01(\x0b\x32\x18.clarifai.api.Visibility\x12\x0e\n\x06\x61pp_id\x18\r \x01(\t\x12\x0f\n\x07user_id\x18\x0e \x01(\t\x12/\n\x0bmodified_at\x18\x0f \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12)\n\x08metadata\x18\x10 \x01(\x0b\x32\x17.google.protobuf.Struct\x12\x0f\n\x07license\x18\x11 \x01(\t\x12-\n\x0boutput_info\x18\x13 \x01(\x0b\x32\x18.clarifai.api.OutputInfo\x12+\n\ninput_info\x18\x14 \x01(\x0b\x32\x17.clarifai.api.InputInfo\x12+\n\ntrain_info\x18\x15 \x01(\x0b\x32\x17.clarifai.api.TrainInfo\x12-\n\x0bimport_info\x18\x16 \x01(\x0b\x32\x18.clarifai.api.ImportInfo\x12\x11\n\ttrain_log\x18\x17 \x01(\tJ\x04\x08\t\x10\nJ\x04\x08\x12\x10\x13\"\xa1\x01\n\x15PretrainedModelConfig\x12\x31\n\x10input_fields_map\x18\x03 \x01(\x0b\x32\x17.google.protobuf.Struct\x12\x32\n\x11output_fields_map\x18\x04 \x01(\x0b\x32\x17.google.protobuf.Struct\x12\x15\n\rmodel_zip_url\x18\x06 \x01(\tJ\x04\x08\x02\x10\x03J\x04\x08\x05\x10\x06\">\n\nTrainStats\x12\x30\n\nloss_curve\x18\x01 \x03(\x0b\x32\x1c.clarifai.api.LossCurveEntry\"B\n\x0eLossCurveEntry\x12\r\n\x05\x65poch\x18\x01 \x01(\r\x12\x13\n\x0bglobal_step\x18\x02 \x01(\r\x12\x0c\n\x04\x63ost\x18\x03 \x01(\x02\"1\n\nLabelCount\x12\x14\n\x0c\x63oncept_name\x18\x01 \x01(\t\x12\r\n\x05\x63ount\x18\x02 \x01(\r\"L\n\x11LabelDistribution\x12\x37\n\x15positive_label_counts\x18\x01 \x03(\x0b\x32\x18.clarifai.api.LabelCount\"B\n\x17\x43ooccurrenceMatrixEntry\x12\x0b\n\x03row\x18\x01 \x01(\t\x12\x0b\n\x03\x63ol\x18\x02 \x01(\t\x12\r\n\x05\x63ount\x18\x03 \x01(\r\"`\n\x12\x43ooccurrenceMatrix\x12\x35\n\x06matrix\x18\x01 \x03(\x0b\x32%.clarifai.api.CooccurrenceMatrixEntry\x12\x13\n\x0b\x63oncept_ids\x18\x02 \x03(\t\"N\n\x14\x43onfusionMatrixEntry\x12\x11\n\tpredicted\x18\x01 \x01(\t\x12\x0e\n\x06\x61\x63tual\x18\x02 \x01(\t\x12\x13\n\x05value\x18\x04 \x01(\x02\x42\x04\x80\xb5\x18\x01\"Z\n\x0f\x43onfusionMatrix\x12\x32\n\x06matrix\x18\x01 \x03(\x0b\x32\".clarifai.api.ConfusionMatrixEntry\x12\x13\n\x0b\x63oncept_ids\x18\x02 \x03(\t\"t\n\x03ROC\x12\x11\n\x03\x66pr\x18\x01 \x03(\x02\x42\x04\x80\xb5\x18\x01\x12\x11\n\x03tpr\x18\x02 \x03(\x02\x42\x04\x80\xb5\x18\x01\x12\x18\n\nthresholds\x18\x03 \x03(\x02\x42\x04\x80\xb5\x18\x01\x12\x15\n\rfpr_per_image\x18\x04 \x03(\x02\x12\x16\n\x0e\x66pr_per_object\x18\x05 \x03(\x02\"_\n\x14PrecisionRecallCurve\x12\x14\n\x06recall\x18\x01 \x03(\x02\x42\x04\x80\xb5\x18\x01\x12\x17\n\tprecision\x18\x02 \x03(\x02\x42\x04\x80\xb5\x18\x01\x12\x18\n\nthresholds\x18\x03 \x03(\x02\x42\x04\x80\xb5\x18\x01\"\xea\x02\n\rBinaryMetrics\x12\x15\n\x07num_pos\x18\x01 \x01(\rB\x04\x80\xb5\x18\x01\x12\x15\n\x07num_neg\x18\x02 \x01(\rB\x04\x80\xb5\x18\x01\x12\x15\n\x07num_tot\x18\x03 \x01(\rB\x04\x80\xb5\x18\x01\x12\x15\n\x07roc_auc\x18\x04 \x01(\x02\x42\x04\x80\xb5\x18\x01\x12\x10\n\x02\x66\x31\x18\x05 \x01(\x02\x42\x04\x80\xb5\x18\x01\x12&\n\x07\x63oncept\x18\x06 \x01(\x0b\x32\x15.clarifai.api.Concept\x12$\n\troc_curve\x18\x07 \x01(\x0b\x32\x11.clarifai.api.ROC\x12\x42\n\x16precision_recall_curve\x18\x08 \x01(\x0b\x32\".clarifai.api.PrecisionRecallCurve\x12\x15\n\ravg_precision\x18\t \x01(\x02\x12\x11\n\tarea_name\x18\n \x01(\t\x12\x10\n\x08\x61rea_min\x18\x0b \x01(\x01\x12\x10\n\x08\x61rea_max\x18\x0c \x01(\x01\x12\x0b\n\x03iou\x18\r \x01(\x02\"\x91\x01\n\x0eTrackerMetrics\x12\x10\n\x08mot_mota\x18\x01 \x01(\x02\x12\x18\n\x10mot_num_switches\x18\x02 \x01(\x05\x12\x12\n\nmorse_frag\x18\x03 \x01(\x02\x12\x15\n\ravg_precision\x18\x04 \x01(\x02\x12\x0c\n\x04\x61iid\x18\x05 \x01(\t\x12\x1a\n\x12unique_switch_rate\x18\x06 \x01(\x02\"\xd9\x01\n\x10\x45valTestSetEntry\x12\"\n\x05input\x18\x06 \x01(\x0b\x32\x13.clarifai.api.Input\x12\x31\n\x12predicted_concepts\x18\x03 \x03(\x0b\x32\x15.clarifai.api.Concept\x12\x34\n\x15ground_truth_concepts\x18\x04 \x03(\x0b\x32\x15.clarifai.api.Concept\x12,\n\nannotation\x18\x05 \x01(\x0b\x32\x18.clarifai.api.AnnotationJ\x04\x08\x01\x10\x02J\x04\x08\x02\x10\x03\"\xcd\x01\n\x0eLOPQEvalResult\x12\t\n\x01k\x18\x01 \x01(\x05\x12#\n\x15recall_vs_brute_force\x18\x02 \x01(\x02\x42\x04\x80\xb5\x18\x01\x12(\n\x1akendall_tau_vs_brute_force\x18\x03 \x01(\x02\x42\x04\x80\xb5\x18\x01\x12(\n\x1amost_frequent_code_percent\x18\x04 \x01(\x02\x42\x04\x80\xb5\x18\x01\x12\x17\n\tlopq_ndcg\x18\x05 \x01(\x02\x42\x04\x80\xb5\x18\x01\x12\x1e\n\x10\x62rute_force_ndcg\x18\x06 \x01(\x02\x42\x04\x80\xb5\x18\x01\"\x8c\x03\n\x0eMetricsSummary\x12\x19\n\rtop1_accuracy\x18\x01 \x01(\x02\x42\x02\x18\x01\x12\x19\n\rtop5_accuracy\x18\x02 \x01(\x02\x42\x02\x18\x01\x12\x1f\n\x11macro_avg_roc_auc\x18\x03 \x01(\x02\x42\x04\x80\xb5\x18\x01\x12\x1f\n\x11macro_std_roc_auc\x18\x04 \x01(\x02\x42\x04\x80\xb5\x18\x01\x12 \n\x12macro_avg_f1_score\x18\x05 \x01(\x02\x42\x04\x80\xb5\x18\x01\x12 \n\x12macro_std_f1_score\x18\x06 \x01(\x02\x42\x04\x80\xb5\x18\x01\x12!\n\x13macro_avg_precision\x18\x07 \x01(\x02\x42\x04\x80\xb5\x18\x01\x12\x1e\n\x10macro_avg_recall\x18\x08 \x01(\x02\x42\x04\x80\xb5\x18\x01\x12!\n\x19mean_avg_precision_iou_50\x18\n \x01(\x02\x12$\n\x1cmean_avg_precision_iou_range\x18\x0b \x01(\x02\x12\x32\n\x0clopq_metrics\x18\t \x03(\x0b\x32\x1c.clarifai.api.LOPQEvalResult\"\xd4\x05\n\x0b\x45valMetrics\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x0f\n\x07user_id\x18\x0f \x01(\t\x12\x0e\n\x06\x61pp_id\x18\x10 \x01(\t\x12\n\n\x02id\x18\n \x01(\t\x12\"\n\x05model\x18\r \x01(\x0b\x32\x13.clarifai.api.Model\x12\x33\n\x14ground_truth_dataset\x18\x0e \x01(\x0b\x32\x15.clarifai.api.Dataset\x12-\n\x07summary\x18\x02 \x01(\x0b\x32\x1c.clarifai.api.MetricsSummary\x12\x37\n\x10\x63onfusion_matrix\x18\x03 \x01(\x0b\x32\x1d.clarifai.api.ConfusionMatrix\x12=\n\x13\x63ooccurrence_matrix\x18\x04 \x01(\x0b\x32 .clarifai.api.CooccurrenceMatrix\x12\x35\n\x0clabel_counts\x18\x05 \x01(\x0b\x32\x1f.clarifai.api.LabelDistribution\x12\x33\n\x0e\x62inary_metrics\x18\x06 \x03(\x0b\x32\x1b.clarifai.api.BinaryMetrics\x12\x30\n\x08test_set\x18\x07 \x03(\x0b\x32\x1e.clarifai.api.EvalTestSetEntry\x12\x34\n\x0fmetrics_by_area\x18\x08 \x03(\x0b\x32\x1b.clarifai.api.BinaryMetrics\x12\x35\n\x10metrics_by_class\x18\t \x03(\x0b\x32\x1b.clarifai.api.BinaryMetrics\x12\x35\n\x0ftracker_metrics\x18\x0b \x03(\x0b\x32\x1c.clarifai.api.TrackerMetrics\x12)\n\teval_info\x18\x0c \x01(\x0b\x32\x16.clarifai.api.EvalInfo\"\xb7\x01\n\x0b\x46ieldsValue\x12\x18\n\x10\x63onfusion_matrix\x18\x01 \x01(\x08\x12\x1b\n\x13\x63ooccurrence_matrix\x18\x02 \x01(\x08\x12\x14\n\x0clabel_counts\x18\x03 \x01(\x08\x12\x16\n\x0e\x62inary_metrics\x18\x04 \x01(\x08\x12\x10\n\x08test_set\x18\x05 \x01(\x08\x12\x17\n\x0fmetrics_by_area\x18\x06 \x01(\x08\x12\x18\n\x10metrics_by_class\x18\x07 \x01(\x08\"\xdb\x01\n\x06Output\x12\n\n\x02id\x18\x01 \x01(\t\x12+\n\x06status\x18\x02 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12.\n\ncreated_at\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\"\n\x05model\x18\x04 \x01(\x0b\x32\x13.clarifai.api.Model\x12\"\n\x05input\x18\x05 \x01(\x0b\x32\x13.clarifai.api.Input\x12 \n\x04\x64\x61ta\x18\x06 \x01(\x0b\x32\x12.clarifai.api.Data\"4\n\tScopeDeps\x12\r\n\x05scope\x18\x01 \x01(\t\x12\x18\n\x10\x64\x65pending_scopes\x18\x02 \x03(\t\":\n\x0c\x45ndpointDeps\x12\x10\n\x08\x65ndpoint\x18\x01 \x01(\t\x12\x18\n\x10\x64\x65pending_scopes\x18\x02 \x03(\t\"\x8d\x01\n\x03Hit\x12\x13\n\x05score\x18\x01 \x01(\x02\x42\x04\x80\xb5\x18\x01\x12\"\n\x05input\x18\x02 \x01(\x0b\x32\x13.clarifai.api.Input\x12,\n\nannotation\x18\x03 \x01(\x0b\x32\x18.clarifai.api.Annotation\x12\x0f\n\x07user_id\x18\x04 \x01(\t\x12\x0e\n\x06\x61pp_id\x18\x05 \x01(\t\"#\n\x08HitCount\x12\x17\n\x0f\x65stimated_total\x18\x01 \x01(\x04\"\x8d\x01\n\x03\x41nd\x12\"\n\x05input\x18\x01 \x01(\x0b\x32\x13.clarifai.api.Input\x12$\n\x06output\x18\x02 \x01(\x0b\x32\x14.clarifai.api.Output\x12\x0e\n\x06negate\x18\x03 \x01(\x08\x12,\n\nannotation\x18\x04 \x01(\x0b\x32\x18.clarifai.api.Annotation\"\x88\x01\n\x05Query\x12#\n\x04\x61nds\x18\x01 \x03(\x0b\x32\x11.clarifai.api.AndB\x02\x18\x01\x12\x10\n\x08language\x18\x02 \x01(\t\x12%\n\x07\x66ilters\x18\x03 \x03(\x0b\x32\x14.clarifai.api.Filter\x12!\n\x05ranks\x18\x04 \x03(\x0b\x32\x12.clarifai.api.Rank\"\xd6\x03\n\x06Search\x12\"\n\x05query\x18\x01 \x01(\x0b\x32\x13.clarifai.api.Query\x12\n\n\x02id\x18\x02 \x01(\t\x12\x16\n\x0e\x61pplication_id\x18\x03 \x01(\t\x12\x0c\n\x04name\x18\x04 \x01(\t\x12)\n\x05\x61s_of\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x10\n\x08git_hash\x18\x06 \x01(\t\x12.\n\ncreated_at\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12/\n\x0bmodified_at\x18\x08 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x11\n\talgorithm\x18\t \x01(\t\x12\x0c\n\x04save\x18\n \x01(\x08\x12\x11\n\tmin_value\x18\x0b \x01(\x02\x12,\n\nvisibility\x18\x0c \x01(\x0b\x32\x18.clarifai.api.Visibility\x12+\n\x06metric\x18\r \x01(\x0e\x32\x1b.clarifai.api.Search.Metric\"I\n\x06Metric\x12\x12\n\x0eMETRIC_NOT_SET\x10\x00\x12\x16\n\x12\x45UCLIDEAN_DISTANCE\x10\x01\x12\x13\n\x0f\x43OSINE_DISTANCE\x10\x02\"\xa4\x01\n\x06\x46ilter\x12\x0e\n\x06negate\x18\x03 \x01(\x08\x12,\n\nannotation\x18\x04 \x01(\x0b\x32\x18.clarifai.api.Annotation\x12\"\n\x05input\x18\x05 \x01(\x0b\x32\x13.clarifai.api.Input\x12\x38\n\x17last_updated_time_range\x18\x06 \x01(\x0b\x32\x17.clarifai.api.TimeRange\"i\n\tTimeRange\x12.\n\nstart_time\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12,\n\x08\x65nd_time\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"D\n\x04Rank\x12\x0e\n\x06negate\x18\x03 \x01(\x08\x12,\n\nannotation\x18\x04 \x01(\x0b\x32\x18.clarifai.api.Annotation\"\x8d\x02\n\x17\x41nnotationSearchMetrics\x12*\n\x0cground_truth\x18\x01 \x01(\x0b\x32\x14.clarifai.api.Search\x12,\n\x0esearch_to_eval\x18\x02 \x01(\x0b\x32\x14.clarifai.api.Search\x12*\n\x07metrics\x18\x03 \x01(\x0b\x32\x19.clarifai.api.EvalMetrics\x12 \n\x04\x64\x61ta\x18\x04 \x01(\x0b\x32\x12.clarifai.api.Data\x12\x1c\n\x14\x61\x63tive_concept_count\x18\x05 \x01(\r\x12,\n\nvisibility\x18\x06 \x01(\x0b\x32\x18.clarifai.api.Visibility\"\x91\x01\n\x04Text\x12\x0b\n\x03raw\x18\x01 \x01(\t\x12\x0b\n\x03url\x18\x02 \x01(\t\x12\x1b\n\x13\x61llow_duplicate_url\x18\x03 \x01(\x08\x12\'\n\x06hosted\x18\x04 \x01(\x0b\x32\x17.clarifai.api.HostedURL\x12)\n\ttext_info\x18\x05 \x01(\x0b\x32\x16.clarifai.api.TextInfo\"0\n\x08TextInfo\x12\x12\n\nchar_count\x18\x01 \x01(\x05\x12\x10\n\x08\x65ncoding\x18\x02 \x01(\t\"\xfc\x05\n\x04User\x12\n\n\x02id\x18\x01 \x01(\t\x12\x19\n\rprimary_email\x18\x02 \x01(\tB\x02\x18\x01\x12\x12\n\nfirst_name\x18\x03 \x01(\t\x12\x11\n\tlast_name\x18\x04 \x01(\t\x12\x14\n\x0c\x63ompany_name\x18\x05 \x01(\t\x12\x11\n\tjob_title\x18\x13 \x01(\t\x12\x10\n\x08job_role\x18\x14 \x01(\t\x12\x15\n\tbill_type\x18\x07 \x01(\tB\x02\x18\x01\x12.\n\ncreated_at\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x39\n\x11\x64\x61te_gdpr_consent\x18\x08 \x01(\x0b\x32\x1a.google.protobuf.TimestampB\x02\x18\x01\x12\x38\n\x10\x64\x61te_tos_consent\x18\t \x01(\x0b\x32\x1a.google.protobuf.TimestampB\x02\x18\x01\x12>\n\x16\x64\x61te_marketing_consent\x18\n \x01(\x0b\x32\x1a.google.protobuf.TimestampB\x02\x18\x01\x12\x38\n\x10\x64\x61te_pii_consent\x18\x17 \x01(\x0b\x32\x1a.google.protobuf.TimestampB\x02\x18\x01\x12-\n\x08metadata\x18\x0b \x01(\x0b\x32\x17.google.protobuf.StructB\x02\x18\x01\x12\x37\n\x0f\x65mail_addresses\x18\x0c \x03(\x0b\x32\x1a.clarifai.api.EmailAddressB\x02\x18\x01\x12#\n\x17two_factor_auth_enabled\x18\x0f \x01(\x08\x42\x02\x18\x01\x12\x17\n\x0bteams_count\x18\x10 \x01(\rB\x02\x18\x01\x12\x12\n\nis_starred\x18\x15 \x01(\x08\x12\x12\n\nstar_count\x18\x16 \x01(\x05\x12,\n\nvisibility\x18\x11 \x01(\x0b\x32\x18.clarifai.api.Visibility\x12-\n\x0buser_detail\x18\x12 \x01(\x0b\x32\x18.clarifai.api.UserDetailJ\x04\x08\r\x10\x0eJ\x04\x08\x0e\x10\x0f\"\xd1\x03\n\nUserDetail\x12\x15\n\rprimary_email\x18\x01 \x01(\t\x12\x11\n\tbill_type\x18\x02 \x01(\t\x12\x35\n\x11\x64\x61te_gdpr_consent\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x34\n\x10\x64\x61te_tos_consent\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12:\n\x16\x64\x61te_marketing_consent\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x34\n\x10\x64\x61te_pii_consent\x18\r \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12)\n\x08metadata\x18\x06 \x01(\x0b\x32\x17.google.protobuf.Struct\x12\x33\n\x0f\x65mail_addresses\x18\x07 \x03(\x0b\x32\x1a.clarifai.api.EmailAddress\x12\x1f\n\x17two_factor_auth_enabled\x18\t \x01(\x08\x12\x13\n\x0bteams_count\x18\n \x01(\r\x12\x0f\n\x07\x63ountry\x18\x0b \x01(\t\x12\r\n\x05state\x18\x0c \x01(\tJ\x04\x08\x08\x10\t\"R\n\x0c\x45mailAddress\x12\x13\n\x05\x65mail\x18\x01 \x01(\tB\x04\x80\xb5\x18\x01\x12\x15\n\x07primary\x18\x02 \x01(\x08\x42\x04\x80\xb5\x18\x01\x12\x16\n\x08verified\x18\x03 \x01(\x08\x42\x04\x80\xb5\x18\x01\"\x1d\n\x08Password\x12\x11\n\tplaintext\x18\x01 \x01(\t\"\x86\x03\n\x12PasswordViolations\x12\x16\n\x0eminimum_length\x18\x01 \x01(\x08\x12\x16\n\x0emaximum_length\x18\x02 \x01(\x08\x12\x19\n\x11upper_case_needed\x18\x03 \x01(\x08\x12\x19\n\x11lower_case_needed\x18\x04 \x01(\x08\x12\x16\n\x0enumeric_needed\x18\x05 \x01(\x08\x12\x1f\n\x17non_alphanumeric_needed\x18\x06 \x01(\x08\x12\x16\n\x0epassword_reuse\x18\x07 \x01(\x08\x12\x15\n\rexclude_names\x18\x08 \x01(\x08\x12\x15\n\rexclude_email\x18\t \x01(\x08\x12\x1c\n\x14no_confusing_letters\x18\n \x01(\x08\x12\x1b\n\x13no_simple_passwords\x18\x0b \x01(\x08\x12\x18\n\x10no_common_vocabs\x18\x0c \x01(\x08\x12\x1b\n\x13no_overlap_with_old\x18\r \x01(\x08\x12\x19\n\x11password_lifespan\x18\x0e \x01(\x08\"\xae\x01\n\x05Video\x12\x0b\n\x03url\x18\x01 \x01(\t\x12\x0e\n\x06\x62\x61se64\x18\x02 \x01(\x0c\x12\x1b\n\x13\x61llow_duplicate_url\x18\x04 \x01(\x08\x12\x15\n\rthumbnail_url\x18\x05 \x01(\t\x12\'\n\x06hosted\x18\x06 \x01(\x0b\x32\x17.clarifai.api.HostedURL\x12+\n\nvideo_info\x18\x07 \x01(\x0b\x32\x17.clarifai.api.VideoInfo\"\x8e\x01\n\tVideoInfo\x12\r\n\x05width\x18\x01 \x01(\x05\x12\x0e\n\x06height\x18\x02 \x01(\x05\x12\x0b\n\x03\x66ps\x18\x03 \x01(\x02\x12\x14\n\x0cvideo_format\x18\x04 \x01(\t\x12\x10\n\x08\x62it_rate\x18\x05 \x01(\x05\x12\x13\n\x0b\x66rame_count\x18\x06 \x01(\x05\x12\x18\n\x10\x64uration_seconds\x18\x07 \x01(\x02\"\xcf\x03\n\x08Workflow\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0e\n\x06\x61pp_id\x18\x02 \x01(\t\x12.\n\ncreated_at\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12)\n\x05nodes\x18\x04 \x03(\x0b\x32\x1a.clarifai.api.WorkflowNode\x12)\n\x08metadata\x18\x05 \x01(\x0b\x32\x17.google.protobuf.Struct\x12,\n\nvisibility\x18\x06 \x01(\x0b\x32\x18.clarifai.api.Visibility\x12\x0f\n\x07user_id\x18\x07 \x01(\t\x12/\n\x0bmodified_at\x18\x08 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12.\n\x07version\x18\t \x01(\x0b\x32\x1d.clarifai.api.WorkflowVersion\x12\x12\n\nis_starred\x18\n \x01(\x08\x12\x12\n\nstar_count\x18\x0b \x01(\x05\x12\x13\n\x0b\x64\x65scription\x18\x0c \x01(\t\x12\r\n\x05notes\x18\r \x01(\t\x12\x17\n\tuse_cases\x18\x0e \x03(\tB\x04\x80\xb5\x18\x01\x12\x1c\n\x0e\x63heck_consents\x18\x0f \x03(\tB\x04\x80\xb5\x18\x01\"\xde\x02\n\x0fWorkflowVersion\x12\n\n\x02id\x18\x01 \x01(\t\x12\x13\n\x0bworkflow_id\x18\x02 \x01(\t\x12.\n\ncreated_at\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12/\n\x0bmodified_at\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12,\n\nvisibility\x18\x05 \x01(\x0b\x32\x18.clarifai.api.Visibility\x12)\n\x05nodes\x18\x06 \x03(\x0b\x32\x1a.clarifai.api.WorkflowNode\x12)\n\x08metadata\x18\x07 \x01(\x0b\x32\x17.google.protobuf.Struct\x12\x0e\n\x06\x61pp_id\x18\x08 \x01(\t\x12\x0f\n\x07user_id\x18\t \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\n \x01(\t\x12\x0f\n\x07license\x18\x0b \x01(\t\"\xbd\x01\n\x0cWorkflowNode\x12\n\n\x02id\x18\x01 \x01(\t\x12\"\n\x05model\x18\x02 \x01(\x0b\x32\x13.clarifai.api.Model\x12,\n\x0bnode_inputs\x18\x03 \x03(\x0b\x32\x17.clarifai.api.NodeInput\x12\x17\n\x0fsuppress_output\x18\x04 \x01(\x08\x12\x36\n\x14output_info_override\x18\x05 \x01(\x0b\x32\x18.clarifai.api.OutputInfo\"\x1c\n\tNodeInput\x12\x0f\n\x07node_id\x18\x01 \x01(\t\"\x81\x02\n\x0eWorkflowResult\x12\n\n\x02id\x18\x01 \x01(\t\x12+\n\x06status\x18\x02 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12.\n\ncreated_at\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\"\n\x05model\x18\x04 \x01(\x0b\x32\x13.clarifai.api.Model\x12\"\n\x05input\x18\x05 \x01(\x0b\x32\x13.clarifai.api.Input\x12%\n\x07outputs\x18\x06 \x03(\x0b\x32\x14.clarifai.api.Output\x12\x17\n\x0fsuppress_output\x18\x07 \x01(\x08\"\x1b\n\rWorkflowState\x12\n\n\x02id\x18\x01 \x01(\t\"\xd8\x02\n\x0e\x41ppDuplication\x12\n\n\x02id\x18\x01 \x01(\t\x12\x12\n\nnew_app_id\x18\x02 \x01(\t\x12\x14\n\x0cnew_app_name\x18\x03 \x01(\t\x12+\n\x06status\x18\x04 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12.\n\ncreated_at\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x34\n\x10last_modified_at\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x33\n\x06\x66ilter\x18\x07 \x01(\x0b\x32#.clarifai.api.AppDuplicationFilters\x12\x17\n\x0f\x65xisting_app_id\x18\x08 \x01(\t\x12/\n\x08progress\x18\t \x03(\x0b\x32\x1d.clarifai.api.AppCopyProgress\"/\n\x0f\x41ppCopyProgress\x12\r\n\x05\x66ield\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x05\"\x8a\x01\n\x15\x41ppDuplicationFilters\x12\x13\n\x0b\x63opy_inputs\x18\x01 \x01(\x08\x12\x15\n\rcopy_concepts\x18\x02 \x01(\x08\x12\x18\n\x10\x63opy_annotations\x18\x03 \x01(\x08\x12\x13\n\x0b\x63opy_models\x18\x04 \x01(\x08\x12\x16\n\x0e\x63opy_workflows\x18\x05 \x01(\x08\"\xfa\x02\n\nLabelOrder\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12+\n\x06status\x18\x03 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x14\n\x0c\x61uto_release\x18\x04 \x01(\x08\x12\x17\n\x0f\x61llow_empty_tag\x18\x05 \x01(\x08\x12\x38\n\x14\x64\x65sired_fulfill_time\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x39\n\x15\x65stimate_fulfill_time\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12 \n\x04task\x18\x08 \x01(\x0b\x32\x12.clarifai.api.Task\x12.\n\ncreated_at\x18\t \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12/\n\x0bmodified_at\x18\n \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"\xb7\x06\n\x04Task\x12\n\n\x02id\x18\x01 \x01(\t\x12.\n\ncreated_at\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12/\n\x0bmodified_at\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12)\n\x04type\x18\x04 \x01(\x0e\x32\x1b.clarifai.api.Task.TaskType\x12\x13\n\x0b\x64\x65scription\x18\x05 \x01(\t\x12(\n\x06worker\x18\x06 \x01(\x0b\x32\x18.clarifai.api.TaskWorker\x12\x13\n\x0b\x63oncept_ids\x18\x07 \x03(\t\x12\x33\n\x0cinput_source\x18\x08 \x01(\x0b\x32\x1d.clarifai.api.TaskInputSource\x12\x11\n\tsample_ms\x18\t \x01(\r\x12\x33\n\x0c\x61i_assistant\x18\n \x01(\x0b\x32\x1d.clarifai.api.TaskAIAssistant\x12(\n\x06review\x18\x0b \x01(\x0b\x32\x18.clarifai.api.TaskReview\x12+\n\x06status\x18\x0c \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x0c\n\x04name\x18\r \x01(\t\x12:\n\x10\x61i_assist_params\x18\x0e \x01(\x0b\x32 .clarifai.api.AiAssistParameters\x12,\n\nvisibility\x18\x0f \x01(\x0b\x32\x18.clarifai.api.Visibility\x12\x0e\n\x06\x61pp_id\x18\x10 \x01(\t\x12\x0f\n\x07user_id\x18\x11 \x01(\t\x12\x16\n\x0elabel_order_id\x18\x12 \x01(\t\x12+\n\x08\x63oncepts\x18\x13 \x03(\x0b\x32\x19.clarifai.api.TaskConcept\x12#\n\x1b\x64\x65lete_previous_annotations\x18\x14 \x01(\x08\"l\n\x08TaskType\x12\x10\n\x0cTYPE_NOT_SET\x10\x00\x12\x1b\n\x17\x43ONCEPTS_CLASSIFICATION\x10\x01\x12\x1a\n\x16\x42OUNDING_BOX_DETECTION\x10\x02\x12\x15\n\x11POLYGON_DETECTION\x10\x03\"`\n\x12\x41iAssistParameters\x12\x15\n\rmin_threshold\x18\x01 \x01(\x02\x12\x15\n\rmax_threshold\x18\x02 \x01(\x02\x12\x1c\n\x14\x63oncept_relation_ids\x18\x03 \x03(\t\"\x8f\x03\n\nTaskWorker\x12=\n\x08strategy\x18\x01 \x01(\x0e\x32+.clarifai.api.TaskWorker.TaskWorkerStrategy\x12\x14\n\x08user_ids\x18\x02 \x03(\tB\x02\x18\x01\x12!\n\x05users\x18\x04 \x03(\x0b\x32\x12.clarifai.api.User\x12#\n\x06models\x18\x05 \x03(\x0b\x32\x13.clarifai.api.Model\x12)\n\tworkflows\x18\x06 \x03(\x0b\x32\x16.clarifai.api.Workflow\x12T\n\x19partitioned_strategy_info\x18\x03 \x01(\x0b\x32/.clarifai.api.TaskWorkerPartitionedStrategyInfoH\x00\"R\n\x12TaskWorkerStrategy\x12\x1b\n\x17WORKER_STRATEGY_NOT_SET\x10\x00\x12\x0f\n\x0bPARTITIONED\x10\x02\x12\x08\n\x04\x46ULL\x10\x03\"\x04\x08\x01\x10\x01\x42\x0f\n\rstrategy_info\"\xa9\x02\n!TaskWorkerPartitionedStrategyInfo\x12[\n\x04type\x18\x01 \x01(\x0e\x32M.clarifai.api.TaskWorkerPartitionedStrategyInfo.TaskWorkerPartitionedStrategy\x12\x19\n\x11workers_per_input\x18\x02 \x01(\x05\x12(\n\x07weights\x18\x03 \x01(\x0b\x32\x17.google.protobuf.Struct\"b\n\x1dTaskWorkerPartitionedStrategy\x12\'\n#PARTITIONED_WORKER_STRATEGY_NOT_SET\x10\x00\x12\n\n\x06\x45VENLY\x10\x01\x12\x0c\n\x08WEIGHTED\x10\x02\"\xc3\x01\n\x0fTaskInputSource\x12?\n\x04type\x18\x01 \x01(\x0e\x32\x31.clarifai.api.TaskInputSource.TaskInputSourceType\x12\n\n\x02id\x18\x02 \x01(\t\"c\n\x13TaskInputSourceType\x12\x1d\n\x19INPUT_SOURCE_TYPE_NOT_SET\x10\x00\x12\x0e\n\nALL_INPUTS\x10\x01\x12\x10\n\x0cSAVED_SEARCH\x10\x02\x12\x0b\n\x07\x44\x41TASET\x10\x03\"\x90\x03\n\nTaskReview\x12=\n\x08strategy\x18\x01 \x01(\x0e\x32+.clarifai.api.TaskReview.TaskReviewStrategy\x12\x14\n\x08user_ids\x18\x02 \x03(\tB\x02\x18\x01\x12!\n\x05users\x18\x05 \x03(\x0b\x32\x12.clarifai.api.User\x12J\n\x14manual_strategy_info\x18\x03 \x01(\x0b\x32*.clarifai.api.TaskReviewManualStrategyInfoH\x00\x12P\n\x17\x63onsensus_strategy_info\x18\x04 \x01(\x0b\x32-.clarifai.api.TaskReviewConsensusStrategyInfoH\x00\"[\n\x12TaskReviewStrategy\x12 \n\x1cTASK_REVIEW_STRATEGY_NOT_SET\x10\x00\x12\x08\n\x04NONE\x10\x01\x12\n\n\x06MANUAL\x10\x02\x12\r\n\tCONSENSUS\x10\x03\x42\x0f\n\rstrategy_info\"9\n\x1cTaskReviewManualStrategyInfo\x12\x19\n\x11sample_percentage\x18\x01 \x01(\x02\"C\n\x1fTaskReviewConsensusStrategyInfo\x12\x1a\n\x12\x61pproval_threshold\x18\x02 \x01(\rJ\x04\x08\x01\x10\x02\"&\n\x0fTaskAIAssistant\x12\x13\n\x0bworkflow_id\x18\x01 \x01(\t\"\xbc\x01\n\x16TaskStatusCountPerUser\x12\x0f\n\x07user_id\x18\x01 \x01(\t\x12\x15\n\x07pending\x18\x02 \x01(\rB\x04\x80\xb5\x18\x01\x12\x1d\n\x0f\x61waiting_review\x18\x03 \x01(\rB\x04\x80\xb5\x18\x01\x12\x15\n\x07success\x18\x04 \x01(\rB\x04\x80\xb5\x18\x01\x12\x1b\n\rreview_denied\x18\x05 \x01(\rB\x04\x80\xb5\x18\x01\x12\'\n\x19\x61waiting_consensus_review\x18\x06 \x01(\rB\x04\x80\xb5\x18\x01\"f\n\x0eThresholdRange\x12\x1a\n\x12is_lower_inclusive\x18\x01 \x01(\x08\x12\x1a\n\x12is_upper_inclusive\x18\x02 \x01(\x08\x12\r\n\x05lower\x18\x03 \x01(\x02\x12\r\n\x05upper\x18\x04 \x01(\x02\"\xad\x01\n\x1fTaskConceptAutoAnnotationConfig\x12\x1d\n\x15\x61nnotation_data_types\x18\x01 \x01(\r\x12\x35\n\x0fthreshold_range\x18\x02 \x01(\x0b\x32\x1c.clarifai.api.ThresholdRange\x12\x34\n\x0bstatus_code\x18\x03 \x01(\x0e\x32\x1f.clarifai.api.status.StatusCode\"\x84\x01\n\x0bTaskConcept\x12&\n\x07\x63oncept\x18\x01 \x01(\x0b\x32\x15.clarifai.api.Concept\x12M\n\x16\x61uto_annotation_config\x18\x02 \x01(\x0b\x32-.clarifai.api.TaskConceptAutoAnnotationConfig\"\x81\x02\n\tCollector\x12\n\n\x02id\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12.\n\ncreated_at\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x1d\n\x15pre_queue_workflow_id\x18\x04 \x01(\t\x12\x1e\n\x16post_queue_workflow_id\x18\x05 \x01(\t\x12\x37\n\x10\x63ollector_source\x18\x06 \x01(\x0b\x32\x1d.clarifai.api.CollectorSource\x12+\n\x06status\x18\x07 \x01(\x0b\x32\x1b.clarifai.api.status.Status\"t\n\x0f\x43ollectorSource\x12\x61\n\'api_post_model_outputs_collector_source\x18\x02 \x01(\x0b\x32\x30.clarifai.api.APIPostModelOutputsCollectorSource\"\x99\x01\n\"APIPostModelOutputsCollectorSource\x12\x15\n\rmodel_user_id\x18\x01 \x01(\t\x12\x14\n\x0cmodel_app_id\x18\x02 \x01(\t\x12\x10\n\x08model_id\x18\x03 \x01(\t\x12\x18\n\x10model_version_id\x18\x04 \x01(\t\x12\x1a\n\x12post_inputs_key_id\x18\x05 \x01(\t\"R\n\tStatValue\x12(\n\x04time\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\r\n\x05value\x18\x02 \x01(\x02\x12\x0c\n\x04tags\x18\x03 \x03(\t\"\xa6\x01\n\x18StatValueAggregateResult\x12?\n\x15stat_value_aggregates\x18\x01 \x03(\x0b\x32 .clarifai.api.StatValueAggregate\x12I\n\x1astat_value_aggregate_query\x18\x02 \x01(\x0b\x32%.clarifai.api.StatValueAggregateQuery\"t\n\x12StatValueAggregate\x12(\n\x04time\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x17\n\x0f\x61ggregate_value\x18\x02 \x01(\x02\x12\r\n\x05\x63ount\x18\x03 \x01(\x04\x12\x0c\n\x04tags\x18\x04 \x03(\t\"\x91\x02\n\x17StatValueAggregateQuery\x12\x0c\n\x04tags\x18\x01 \x03(\t\x12\x12\n\ntag_groups\x18\x02 \x03(\t\x12;\n\x13stat_value_agg_type\x18\x03 \x01(\x0e\x32\x1e.clarifai.api.StatValueAggType\x12\x39\n\x12stat_time_agg_type\x18\x04 \x01(\x0e\x32\x1d.clarifai.api.StatTimeAggType\x12.\n\nstart_time\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12,\n\x08\x65nd_time\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"\xef\x01\n\x19\x44\x61tasetInputsSearchAddJob\x12\n\n\x02id\x18\x01 \x01(\t\x12.\n\ncreated_at\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12/\n\x0bmodified_at\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12+\n\x06status\x18\x04 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x12\n\ndataset_id\x18\x05 \x01(\t\x12$\n\x06search\x18\x06 \x01(\x0b\x32\x14.clarifai.api.Search\"O\n\x17PCAProjectionComparator\x12\x1a\n\x12\x64istance_threshold\x18\x01 \x01(\x02\x12\x18\n\x10model_version_id\x18\x02 \x01(\t\"K\n\x1b\x44uplicateAnnotationsResults\x12\x16\n\x0e\x64uplicate_cfid\x18\x01 \x03(\t\x12\x14\n\x0cunique_count\x18\x02 \x01(\x05\"\x87\x01\n\nVisibility\x12\x33\n\x08gettable\x18\x01 \x01(\x0e\x32!.clarifai.api.Visibility.Gettable\"D\n\x08Gettable\x12\x16\n\x12UNKNOWN_VISIBILITY\x10\x00\x12\x0b\n\x07PRIVATE\x10\n\x12\x07\n\x03ORG\x10\x1e\x12\n\n\x06PUBLIC\x10\x32\"X\n\x0eTrendingMetric\x12\x0f\n\x07user_id\x18\x01 \x01(\t\x12\x0e\n\x06\x61pp_id\x18\x02 \x01(\t\x12\x11\n\tobject_id\x18\x03 \x01(\t\x12\x12\n\nview_count\x18\x04 \x01(\x04\"#\n\x07\x46ullTag\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\n\n\x02id\x18\x02 \x01(\t\"f\n\x0bTimeSegment\x12\n\n\x02id\x18\x01 \x01(\t\x12 \n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x12.clarifai.api.Data\x12)\n\ttime_info\x18\x03 \x01(\x0b\x32\x16.clarifai.api.TimeInfo\"D\n\x08TimeInfo\x12\x12\n\nnum_frames\x18\x01 \x01(\r\x12\x12\n\nbegin_time\x18\x02 \x01(\r\x12\x10\n\x08\x65nd_time\x18\x03 \x01(\r\"!\n\x0b\x44\x61tasetStar\x12\x12\n\ndataset_id\x18\x01 \x01(\t\"\x1f\n\nModuleStar\x12\x11\n\tmodule_id\x18\x01 \x01(\t\"\xe7\x02\n\x06Module\x12\n\n\x02id\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x03 \x01(\t\x12.\n\ncreated_at\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12/\n\x0bmodified_at\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12,\n\nvisibility\x18\x07 \x01(\x0b\x32\x18.clarifai.api.Visibility\x12)\n\x08metadata\x18\x08 \x01(\x0b\x32\x17.google.protobuf.Struct\x12\x0f\n\x07user_id\x18\t \x01(\t\x12\x0e\n\x06\x61pp_id\x18\n \x01(\t\x12\x33\n\x0emodule_version\x18\x0b \x01(\x0b\x32\x1b.clarifai.api.ModuleVersion\x12\x12\n\nis_starred\x18\x0c \x01(\x08\x12\x12\n\nstar_count\x18\r \x01(\x05J\x04\x08\x02\x10\x03\"\xbe\x04\n\rModuleVersion\x12\n\n\x02id\x18\x01 \x01(\t\x12\x11\n\tmodule_id\x18\x02 \x01(\t\x12\x0e\n\x06\x61pp_id\x18\x03 \x01(\t\x12\x0f\n\x07user_id\x18\x04 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x06 \x01(\t\x12\r\n\x05notes\x18\x07 \x01(\t\x12.\n\ncreated_at\x18\x08 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12/\n\x0bmodified_at\x18\t \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x16\n\x0egit_commit_url\x18\n \x01(\t\x12\x39\n\nmodule_nav\x18\x0b \x01(\x0b\x32%.clarifai.api.ModuleVersion.ModuleNav\x12\x10\n\x08\x61pproved\x18\x0c \x01(\x08\x12,\n\nvisibility\x18\r \x01(\x0b\x32\x18.clarifai.api.Visibility\x12)\n\x08metadata\x18\x0e \x01(\x0b\x32\x17.google.protobuf.Struct\x1a\x45\n\x0cModuleSubNav\x12\r\n\x05title\x18\x01 \x01(\t\x12\x11\n\tquery_key\x18\x02 \x01(\t\x12\x13\n\x0bquery_value\x18\x03 \x01(\t\x1a]\n\tModuleNav\x12\r\n\x05title\x18\x01 \x01(\t\x12\x41\n\x0fmodule_sub_navs\x18\x02 \x03(\x0b\x32(.clarifai.api.ModuleVersion.ModuleSubNavJ\x04\x08\x05\x10\x06\"\xad\x02\n\x16InstalledModuleVersion\x12\n\n\x02id\x18\x01 \x01(\t\x12\x33\n\x0emodule_version\x18\x02 \x01(\x0b\x32\x1b.clarifai.api.ModuleVersion\x12\x0e\n\x06\x61pp_id\x18\x03 \x01(\t\x12\x0f\n\x07user_id\x18\x04 \x01(\t\x12.\n\ncreated_at\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12/\n\x0bmodified_at\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x12\n\ndeploy_url\x18\x07 \x01(\t\x12,\n\nvisibility\x18\x08 \x01(\x0b\x32\x18.clarifai.api.Visibility\x12\x0e\n\x06key_id\x18\t \x01(\t\"\xb7\x03\n\rBulkOperation\x12\n\n\x02id\x18\x01 \x01(\t\x12+\n\tinput_ids\x18\x02 \x01(\x0b\x32\x16.clarifai.api.InputIDsH\x00\x12&\n\x06search\x18\n \x01(\x0b\x32\x14.clarifai.api.SearchH\x00\x12(\n\x07\x64\x61taset\x18\x0b \x01(\x0b\x32\x15.clarifai.api.DatasetH\x00\x12*\n\toperation\x18\x03 \x01(\x0b\x32\x17.clarifai.api.Operation\x12\x0e\n\x06\x61pp_id\x18\x04 \x01(\t\x12+\n\x06status\x18\x05 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12(\n\x08progress\x18\x06 \x01(\x0b\x32\x16.clarifai.api.Progress\x12\x12\n\ncreated_by\x18\x07 \x01(\t\x12.\n\ncreated_at\x18\x08 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x34\n\x10last_modified_at\x18\t \x01(\x0b\x32\x1a.google.protobuf.TimestampB\x0e\n\x0cinput_source\"\x1d\n\x08InputIDs\x12\x11\n\tinput_ids\x18\x01 \x03(\t\"8\n\x08Progress\x12\x11\n\tprocessed\x18\x01 \x01(\r\x12\x19\n\x11last_processed_id\x18\x02 \x01(\t\"\x8a\x04\n\tOperation\x12\x31\n\x0c\x61\x64\x64_concepts\x18\x01 \x01(\x0b\x32\x19.clarifai.api.AddConceptsH\x00\x12\x37\n\x0f\x64\x65lete_concepts\x18\x02 \x01(\x0b\x32\x1c.clarifai.api.DeleteConceptsH\x00\x12\x31\n\x0c\x61\x64\x64_metadata\x18\x03 \x01(\x0b\x32\x19.clarifai.api.AddMetadataH\x00\x12\x37\n\x0f\x64\x65lete_metadata\x18\x04 \x01(\x0b\x32\x1c.clarifai.api.DeleteMetadataH\x00\x12\x33\n\roverwrite_geo\x18\x05 \x01(\x0b\x32\x1a.clarifai.api.OverwriteGeoH\x00\x12-\n\ndelete_geo\x18\x06 \x01(\x0b\x32\x17.clarifai.api.DeleteGeoH\x00\x12>\n\x13\x64\x65lete_from_dataset\x18\x07 \x01(\x0b\x32\x1f.clarifai.api.DeleteFromDatasetH\x00\x12\x34\n\x0e\x61\x64\x64_to_dataset\x18\x08 \x01(\x0b\x32\x1a.clarifai.api.AddToDatasetH\x00\x12>\n\x13split_into_datasets\x18\t \x01(\x0b\x32\x1f.clarifai.api.SplitIntoDatasetsH\x00\x42\x0b\n\toperation\"6\n\x0b\x41\x64\x64\x43oncepts\x12\'\n\x08\x63oncepts\x18\x01 \x03(\x0b\x32\x15.clarifai.api.Concept\"K\n\x0e\x44\x65leteConcepts\x12\'\n\x08\x63oncepts\x18\x01 \x03(\x0b\x32\x15.clarifai.api.Concept\x12\x10\n\x08user_ids\x18\x02 \x03(\t\"8\n\x0b\x41\x64\x64Metadata\x12)\n\x08metadata\x18\x01 \x01(\x0b\x32\x17.google.protobuf.Struct\";\n\x0e\x44\x65leteMetadata\x12)\n\x08metadata\x18\x01 \x01(\x0b\x32\x17.google.protobuf.Struct\".\n\x0cOverwriteGeo\x12\x1e\n\x03geo\x18\x01 \x01(\x0b\x32\x11.clarifai.api.Geo\"\x0b\n\tDeleteGeo\"\"\n\x0c\x41\x64\x64ToDataset\x12\x12\n\ndataset_id\x18\x01 \x01(\t\"\'\n\x11\x44\x65leteFromDataset\x12\x12\n\ndataset_id\x18\x01 \x01(\t\"\xcb\x01\n\x11SplitIntoDatasets\x12\x32\n\x0e\x64\x61taset_splits\x18\x01 \x03(\x0b\x32\x1a.clarifai.api.DatasetSplit\x12\x42\n\x06method\x18\x02 \x01(\x0e\x32\x32.clarifai.api.SplitIntoDatasets.DatasetSplitMethod\">\n\x12\x44\x61tasetSplitMethod\x12\x0b\n\x07NOT_SET\x10\x00\x12\x1b\n\x17RANDOM_PERCENTAGE_SPLIT\x10\x01\"[\n\x0c\x44\x61tasetSplit\x12&\n\x07\x64\x61taset\x18\x01 \x01(\x0b\x32\x15.clarifai.api.Dataset\x12\x14\n\npercentage\x18\x02 \x01(\rH\x00\x42\r\n\x0bmethod_info\"\xfb\x02\n\x0cInputsAddJob\x12\n\n\x02id\x18\x01 \x01(\t\x12\x15\n\rcall_back_url\x18\x03 \x01(\t\x12\x0f\n\x07\x61pp_pat\x18\x04 \x01(\t\x12\x34\n\x08progress\x18\x07 \x01(\x0b\x32\".clarifai.api.InputsAddJobProgress\x12.\n\ncreated_at\x18\x08 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12/\n\x0bmodified_at\x18\t \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12:\n\x0f\x65xtraction_jobs\x18\n \x03(\x0b\x32!.clarifai.api.InputsExtractionJob\x12%\n\x07uploads\x18\x0b \x03(\x0b\x32\x14.clarifai.api.Upload\x12+\n\x06status\x18\x0c \x01(\x0b\x32\x1b.clarifai.api.status.StatusJ\x04\x08\x02\x10\x03J\x04\x08\x05\x10\x06J\x04\x08\x06\x10\x07\"u\n\x14InputsAddJobProgress\x12\x15\n\rpending_count\x18\x01 \x01(\x04\x12\x19\n\x11in_progress_count\x18\x02 \x01(\x04\x12\x15\n\rsuccess_count\x18\x03 \x01(\x04\x12\x14\n\x0c\x66\x61iled_count\x18\x04 \x01(\x04\"\x95\x02\n\x06Upload\x12\n\n\x02id\x18\x01 \x01(\t\x12.\n\ncreated_at\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12/\n\x0bmodified_at\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12.\n\nexpires_at\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12+\n\x06status\x18\x05 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x14\n\x0c\x63ontent_name\x18\x08 \x01(\t\x12\x16\n\x0e\x63ontent_length\x18\x06 \x01(\x04\x12\x13\n\x0b\x63ontent_url\x18\x07 \x01(\t\"K\n\x11UploadContentPart\x12\x13\n\x0brange_start\x18\x01 \x01(\x04\x12\x13\n\x0bpart_number\x18\x02 \x01(\x03\x12\x0c\n\x04\x64\x61ta\x18\x03 \x01(\x0c\"l\n\x19\x43ustomCodeOperatorRequest\x12#\n\x06inputs\x18\x01 \x03(\x0b\x32\x13.clarifai.api.Input\x12*\n\x08metadata\x18\xea\x07 \x01(\x0b\x32\x17.google.protobuf.Struct\"\xc8\x02\n\x13InputsExtractionJob\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\n\n\x02id\x18\x02 \x01(\t\x12\x0b\n\x03url\x18\x03 \x01(\t\x12;\n\x08progress\x18\x04 \x01(\x0b\x32).clarifai.api.InputsExtractionJobProgress\x12.\n\ncreated_at\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12/\n\x0bmodified_at\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12M\n\x1cinput_id_conflict_resolution\x18\x07 \x01(\x0e\x32\'.clarifai.api.InputIDConflictResolution\"\x97\x02\n\x1bInputsExtractionJobProgress\x12\x1a\n\x12\x61udio_inputs_count\x18\x02 \x01(\x04\x12\x1a\n\x12image_inputs_count\x18\x03 \x01(\x04\x12\x1a\n\x12video_inputs_count\x18\x04 \x01(\x04\x12\x19\n\x11text_inputs_count\x18\x05 \x01(\x04\x12\x1e\n\x16pending_archives_count\x18\x06 \x01(\x04\x12\"\n\x1ain_progress_archives_count\x18\x07 \x01(\x04\x12 \n\x18\x63ompleted_archives_count\x18\x08 \x01(\x04\x12\x1d\n\x15\x66\x61iled_archives_count\x18\t \x01(\x04J\x04\x08\x01\x10\x02\"\xa6\x01\n\x10InputsDataSource\x12\x19\n\x11inputs_add_job_id\x18\x01 \x01(\t\x12(\n\x03url\x18\x02 \x01(\x0b\x32\x1b.clarifai.api.DataSourceURL\x12M\n\x1cinput_id_conflict_resolution\x18\x03 \x01(\x0e\x32\'.clarifai.api.InputIDConflictResolution\"V\n\rDataSourceURL\x12\x0b\n\x03url\x18\x01 \x01(\t\x12\x38\n\x0b\x63redentials\x18\x02 \x01(\x0b\x32#.clarifai.api.DataSourceCredentials\"\xa7\x01\n\x15\x44\x61taSourceCredentials\x12*\n\x08s3_creds\x18\x01 \x01(\x0b\x32\x16.clarifai.api.AWSCredsH\x00\x12\x13\n\tgcp_creds\x18\x02 \x01(\x0cH\x00\x12\x38\n\x10\x61zure_blob_creds\x18\x04 \x01(\x0b\x32\x1c.clarifai.api.AzureBlobCredsH\x00\x42\r\n\x0b\x63redentialsJ\x04\x08\x03\x10\x04\"K\n\x08\x41WSCreds\x12\x0e\n\x06region\x18\x02 \x01(\t\x12\n\n\x02id\x18\x03 \x01(\t\x12\x0e\n\x06secret\x18\x04 \x01(\t\x12\r\n\x05token\x18\x05 \x01(\tJ\x04\x08\x01\x10\x02\";\n\x0e\x41zureBlobCreds\x12\x14\n\x0c\x61\x63\x63ount_name\x18\x01 \x01(\t\x12\x13\n\x0b\x61\x63\x63ount_key\x18\x02 \x01(\t\"\xaf\x01\n\x0cInputsUpload\x12\x19\n\x11inputs_add_job_id\x18\x01 \x01(\t\x12\x0f\n\x07\x61pp_pat\x18\x02 \x01(\t\x12$\n\x06upload\x18\x03 \x01(\x0b\x32\x14.clarifai.api.Upload\x12M\n\x1cinput_id_conflict_resolution\x18\x04 \x01(\x0e\x32\'.clarifai.api.InputIDConflictResolution*\xf9\x01\n\x1e\x44\x61tasetVersionMetricsGroupType\x12.\n*DATASET_VERSION_METRICS_GROUP_TYPE_NOT_SET\x10\x00\x12\x0e\n\nINPUT_TYPE\x10\x02\x12\x0e\n\nCONCEPT_ID\x10\n\x12\x12\n\x0e\x43ONCEPTS_COUNT\x10\x0b\x12\x18\n\x14\x42OUNDING_BOXES_COUNT\x10\x14\x12\x12\n\x0ePOLYGONS_COUNT\x10\x15\x12\x10\n\x0cPOINTS_COUNT\x10\x16\x12\x0f\n\x0bMASKS_COUNT\x10\x17\x12\x10\n\x0cPIXELS_COUNT\x10\x1e\x12\x10\n\x0c\x41SPECT_RATIO\x10\x1f*\x85\x01\n\x1a\x44\x61tasetVersionExportFormat\x12)\n%DATASET_VERSION_EXPORT_FORMAT_NOT_SET\x10\x00\x12\x1a\n\x16\x43LARIFAI_DATA_PROTOBUF\x10\x01\x12\x16\n\x12\x43LARIFAI_DATA_JSON\x10\x03\x12\x08\n\x04\x43OCO\x10\x02*H\n\x10\x45xpirationAction\x12\x1d\n\x19\x45XPIRATION_ACTION_NOT_SET\x10\x00\x12\t\n\x05\x44\x45LAY\x10\x01\x12\n\n\x06\x45XPIRY\x10\x02*M\n\x0cLicenseScope\x12\x19\n\x15LICENSE_SCOPE_NOT_SET\x10\x00\x12\x0b\n\x07PREDICT\x10\x01\x12\t\n\x05TRAIN\x10\x02\x12\n\n\x06SEARCH\x10\x03*P\n\x08\x44\x61taType\x12\r\n\tUNDEFINED\x10\x00\x12\n\n\x06STRING\x10\x01\x12\t\n\x05UINT8\x10\x02\x12\t\n\x05INT32\x10\x03\x12\t\n\x05INT64\x10\x04\x12\x08\n\x04\x46P32\x10\x05*\x8f\x01\n\x0fValueComparator\x12\x1d\n\x19\x43ONCEPT_THRESHOLD_NOT_SET\x10\x00\x12\x10\n\x0cGREATER_THAN\x10\x01\x12\x19\n\x15GREATER_THAN_OR_EQUAL\x10\x02\x12\r\n\tLESS_THAN\x10\x03\x12\x16\n\x12LESS_THAN_OR_EQUAL\x10\x04\x12\t\n\x05\x45QUAL\x10\x05*q\n\x0e\x45valuationType\x12\r\n\tUndefined\x10\x00\x12\x12\n\x0e\x43lassification\x10\x01\x12\r\n\tDetection\x10\x02\x12\x10\n\x0cSegmentation\x10\x03\x12\x0e\n\nClustering\x10\x04\x12\x0b\n\x07Tracker\x10\x05*f\n\x0c\x41PIEventType\x12\x1a\n\x16\x41PI_EVENT_TYPE_NOT_SET\x10\x00\x12\x13\n\x0fON_PREM_PREDICT\x10\x01\x12\x11\n\rON_PREM_TRAIN\x10\x02\x12\x12\n\x0eON_PREM_SEARCH\x10\x03*<\n\x11UsageIntervalType\x12\t\n\x05undef\x10\x00\x12\x07\n\x03\x64\x61y\x10\x01\x12\t\n\x05month\x10\x02\x12\x08\n\x04year\x10\x03*}\n\x12\x41nnotationDataType\x12 \n\x1c\x41NNOTATION_DATA_TYPE_NOT_SET\x10\x00\x12\x07\n\x03TAG\x10\x01\x12\x10\n\x0c\x42OUNDING_BOX\x10\x02\x12\x0b\n\x07POLYGON\x10\x04\x12\t\n\x05POINT\x10\x08\x12\x08\n\x04SPAN\x10\x10\x12\x08\n\x04MASK\x10 *\x1d\n\x08RoleType\x12\x08\n\x04TEAM\x10\x00\x12\x07\n\x03ORG\x10\x01*$\n\x10StatValueAggType\x12\x07\n\x03SUM\x10\x00\x12\x07\n\x03\x41VG\x10\x01*`\n\x0fStatTimeAggType\x12\x0f\n\x0bNO_TIME_AGG\x10\x00\x12\x08\n\x04YEAR\x10\x01\x12\t\n\x05MONTH\x10\x02\x12\x08\n\x04WEEK\x10\x03\x12\x07\n\x03\x44\x41Y\x10\x04\x12\x08\n\x04HOUR\x10\x05\x12\n\n\x06MINUTE\x10\x06*b\n\x13ValidationErrorType\x12!\n\x1dVALIDATION_ERROR_TYPE_NOT_SET\x10\x00\x12\x0e\n\nRESTRICTED\x10\x01\x12\x0c\n\x08\x44\x41TABASE\x10\x02\x12\n\n\x06\x46ORMAT\x10\x03*[\n\x19InputIDConflictResolution\x12(\n$INPUT_ID_CONFLICT_RESOLUTION_NOT_SET\x10\x00\x12\x08\n\x04SKIP\x10\x01\x12\n\n\x06SUFFIX\x10\x02\x42Y\n\x15\x63om.clarifai.grpc.apiP\x01Z7github.com/Clarifai/clarifai-go-grpc/proto/clarifai/api\xa2\x02\x04\x43\x41IPb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'proto.clarifai.api.resources_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\025com.clarifai.grpc.apiP\001Z7github.com/Clarifai/clarifai-go-grpc/proto/clarifai/api\242\002\004CAIP'
@@ -113,16 +113,14 @@
   _MODEL.fields_by_name['languages_full']._serialized_options = b'\200\265\030\001'
   _MODEL.fields_by_name['check_consents']._options = None
   _MODEL.fields_by_name['check_consents']._serialized_options = b'\200\265\030\001'
   _MODEL.fields_by_name['import_info']._options = None
   _MODEL.fields_by_name['import_info']._serialized_options = b'\030\001'
   _OUTPUTCONFIG.fields_by_name['concepts_mutually_exclusive']._options = None
   _OUTPUTCONFIG.fields_by_name['concepts_mutually_exclusive']._serialized_options = b'\030\001'
-  _OUTPUTCONFIG.fields_by_name['closed_environment']._options = None
-  _OUTPUTCONFIG.fields_by_name['closed_environment']._serialized_options = b'\200\265\030\001'
   _OUTPUTCONFIG.fields_by_name['existing_model_id']._options = None
   _OUTPUTCONFIG.fields_by_name['existing_model_id']._serialized_options = b'\030\001'
   _OUTPUTCONFIG.fields_by_name['hyper_parameters']._options = None
   _OUTPUTCONFIG.fields_by_name['hyper_parameters']._serialized_options = b'\030\001'
   _OUTPUTCONFIG.fields_by_name['max_concepts']._options = None
   _OUTPUTCONFIG.fields_by_name['max_concepts']._serialized_options = b'\200\265\030\001'
   _OUTPUTCONFIG.fields_by_name['min_value']._options = None
@@ -223,42 +221,44 @@
   _TASKSTATUSCOUNTPERUSER.fields_by_name['awaiting_review']._serialized_options = b'\200\265\030\001'
   _TASKSTATUSCOUNTPERUSER.fields_by_name['success']._options = None
   _TASKSTATUSCOUNTPERUSER.fields_by_name['success']._serialized_options = b'\200\265\030\001'
   _TASKSTATUSCOUNTPERUSER.fields_by_name['review_denied']._options = None
   _TASKSTATUSCOUNTPERUSER.fields_by_name['review_denied']._serialized_options = b'\200\265\030\001'
   _TASKSTATUSCOUNTPERUSER.fields_by_name['awaiting_consensus_review']._options = None
   _TASKSTATUSCOUNTPERUSER.fields_by_name['awaiting_consensus_review']._serialized_options = b'\200\265\030\001'
-  _DATASETVERSIONMETRICSGROUPTYPE._serialized_start=35298
-  _DATASETVERSIONMETRICSGROUPTYPE._serialized_end=35547
-  _DATASETVERSIONEXPORTFORMAT._serialized_start=35550
-  _DATASETVERSIONEXPORTFORMAT._serialized_end=35683
-  _EXPIRATIONACTION._serialized_start=35685
-  _EXPIRATIONACTION._serialized_end=35757
-  _LICENSESCOPE._serialized_start=35759
-  _LICENSESCOPE._serialized_end=35836
-  _DATATYPE._serialized_start=35838
-  _DATATYPE._serialized_end=35918
-  _VALUECOMPARATOR._serialized_start=35921
-  _VALUECOMPARATOR._serialized_end=36064
-  _EVALUATIONTYPE._serialized_start=36066
-  _EVALUATIONTYPE._serialized_end=36179
-  _APIEVENTTYPE._serialized_start=36181
-  _APIEVENTTYPE._serialized_end=36283
-  _USAGEINTERVALTYPE._serialized_start=36285
-  _USAGEINTERVALTYPE._serialized_end=36345
-  _ANNOTATIONDATATYPE._serialized_start=36347
-  _ANNOTATIONDATATYPE._serialized_end=36463
-  _ROLETYPE._serialized_start=36465
-  _ROLETYPE._serialized_end=36494
-  _STATVALUEAGGTYPE._serialized_start=36496
-  _STATVALUEAGGTYPE._serialized_end=36532
-  _STATTIMEAGGTYPE._serialized_start=36534
-  _STATTIMEAGGTYPE._serialized_end=36630
-  _VALIDATIONERRORTYPE._serialized_start=36632
-  _VALIDATIONERRORTYPE._serialized_end=36730
+  _DATASETVERSIONMETRICSGROUPTYPE._serialized_start=35866
+  _DATASETVERSIONMETRICSGROUPTYPE._serialized_end=36115
+  _DATASETVERSIONEXPORTFORMAT._serialized_start=36118
+  _DATASETVERSIONEXPORTFORMAT._serialized_end=36251
+  _EXPIRATIONACTION._serialized_start=36253
+  _EXPIRATIONACTION._serialized_end=36325
+  _LICENSESCOPE._serialized_start=36327
+  _LICENSESCOPE._serialized_end=36404
+  _DATATYPE._serialized_start=36406
+  _DATATYPE._serialized_end=36486
+  _VALUECOMPARATOR._serialized_start=36489
+  _VALUECOMPARATOR._serialized_end=36632
+  _EVALUATIONTYPE._serialized_start=36634
+  _EVALUATIONTYPE._serialized_end=36747
+  _APIEVENTTYPE._serialized_start=36749
+  _APIEVENTTYPE._serialized_end=36851
+  _USAGEINTERVALTYPE._serialized_start=36853
+  _USAGEINTERVALTYPE._serialized_end=36913
+  _ANNOTATIONDATATYPE._serialized_start=36915
+  _ANNOTATIONDATATYPE._serialized_end=37040
+  _ROLETYPE._serialized_start=37042
+  _ROLETYPE._serialized_end=37071
+  _STATVALUEAGGTYPE._serialized_start=37073
+  _STATVALUEAGGTYPE._serialized_end=37109
+  _STATTIMEAGGTYPE._serialized_start=37111
+  _STATTIMEAGGTYPE._serialized_end=37207
+  _VALIDATIONERRORTYPE._serialized_start=37209
+  _VALIDATIONERRORTYPE._serialized_end=37307
+  _INPUTIDCONFLICTRESOLUTION._serialized_start=37309
+  _INPUTIDCONFLICTRESOLUTION._serialized_end=37400
   _ANNOTATION._serialized_start=357
   _ANNOTATION._serialized_end=842
   _APP._serialized_start=845
   _APP._serialized_end=1385
   _APPQUERY._serialized_start=1387
   _APPQUERY._serialized_end=1411
   _COLLABORATOR._serialized_start=1414
@@ -352,305 +352,309 @@
   _DATASET._serialized_start=6979
   _DATASET._serialized_end=7421
   _ANNOTATIONFILTER._serialized_start=7424
   _ANNOTATIONFILTER._serialized_end=7640
   _DATASETINPUT._serialized_start=7642
   _DATASETINPUT._serialized_end=7740
   _DATASETVERSION._serialized_start=7743
-  _DATASETVERSION._serialized_end=8488
-  _DATASETVERSION_METRICSENTRY._serialized_start=8372
-  _DATASETVERSION_METRICSENTRY._serialized_end=8455
-  _ANNOTATIONFILTERCONFIG._serialized_start=8490
-  _ANNOTATIONFILTERCONFIG._serialized_end=8602
-  _MODELPREDICTCONFIG._serialized_start=8604
-  _MODELPREDICTCONFIG._serialized_end=8660
-  _DATASETVERSIONMETRICS._serialized_start=8663
-  _DATASETVERSIONMETRICS._serialized_end=9754
-  _DATASETVERSIONMETRICSGROUP._serialized_start=9757
-  _DATASETVERSIONMETRICSGROUP._serialized_end=9959
-  _DATASETVERSIONEXPORTINFO._serialized_start=9962
-  _DATASETVERSIONEXPORTINFO._serialized_end=10170
-  _DATASETVERSIONEXPORT._serialized_start=10173
-  _DATASETVERSIONEXPORT._serialized_end=10353
-  _WORKFLOWRESULTSSIMILARITY._serialized_start=10355
-  _WORKFLOWRESULTSSIMILARITY._serialized_end=10465
-  _KEY._serialized_start=10468
-  _KEY._serialized_end=10712
-  _MODEL._serialized_start=10715
-  _MODEL._serialized_end=11699
-  _MODELREFERENCE._serialized_start=11701
-  _MODELREFERENCE._serialized_end=11817
-  _MODELVERSIONINPUTEXAMPLE._serialized_start=11820
-  _MODELVERSIONINPUTEXAMPLE._serialized_end=11971
-  _OUTPUTINFO._serialized_start=11974
-  _OUTPUTINFO._serialized_end=12186
-  _INPUTINFO._serialized_start=12188
-  _INPUTINFO._serialized_end=12285
-  _TRAININFO._serialized_start=12287
-  _TRAININFO._serialized_end=12339
-  _EVALINFO._serialized_start=12341
-  _EVALINFO._serialized_end=12392
-  _IMPORTINFO._serialized_start=12394
-  _IMPORTINFO._serialized_end=12447
-  _OUTPUTCONFIG._serialized_start=12450
-  _OUTPUTCONFIG._serialized_end=12963
-  _MODELTYPE._serialized_start=12966
-  _MODELTYPE._serialized_end=13432
-  _MODELLAYERINFO._serialized_start=13435
-  _MODELLAYERINFO._serialized_end=13572
-  _TRITONCONDAENVINFO._serialized_start=13574
-  _TRITONCONDAENVINFO._serialized_end=13642
-  _LAYERSHAPE._serialized_start=13644
-  _LAYERSHAPE._serialized_end=13752
-  _MODELTYPEFIELD._serialized_start=13755
-  _MODELTYPEFIELD._serialized_end=14477
-  _MODELTYPEFIELD_MODELTYPEFIELDTYPE._serialized_start=14120
-  _MODELTYPEFIELD_MODELTYPEFIELDTYPE._serialized_end=14477
-  _MODELTYPERANGEINFO._serialized_start=14479
-  _MODELTYPERANGEINFO._serialized_end=14539
-  _MODELTYPEENUMOPTION._serialized_start=14542
-  _MODELTYPEENUMOPTION._serialized_end=14754
-  _MODELTYPEENUMOPTIONALIAS._serialized_start=14756
-  _MODELTYPEENUMOPTIONALIAS._serialized_end=14823
-  _MODELQUERY._serialized_start=14825
-  _MODELQUERY._serialized_end=14880
-  _MODELVERSION._serialized_start=14883
-  _MODELVERSION._serialized_end=15647
-  _PRETRAINEDMODELCONFIG._serialized_start=15650
-  _PRETRAINEDMODELCONFIG._serialized_end=15811
-  _TRAINSTATS._serialized_start=15813
-  _TRAINSTATS._serialized_end=15875
-  _LOSSCURVEENTRY._serialized_start=15877
-  _LOSSCURVEENTRY._serialized_end=15943
-  _LABELCOUNT._serialized_start=15945
-  _LABELCOUNT._serialized_end=15994
-  _LABELDISTRIBUTION._serialized_start=15996
-  _LABELDISTRIBUTION._serialized_end=16072
-  _COOCCURRENCEMATRIXENTRY._serialized_start=16074
-  _COOCCURRENCEMATRIXENTRY._serialized_end=16140
-  _COOCCURRENCEMATRIX._serialized_start=16142
-  _COOCCURRENCEMATRIX._serialized_end=16238
-  _CONFUSIONMATRIXENTRY._serialized_start=16240
-  _CONFUSIONMATRIXENTRY._serialized_end=16318
-  _CONFUSIONMATRIX._serialized_start=16320
-  _CONFUSIONMATRIX._serialized_end=16410
-  _ROC._serialized_start=16412
-  _ROC._serialized_end=16528
-  _PRECISIONRECALLCURVE._serialized_start=16530
-  _PRECISIONRECALLCURVE._serialized_end=16625
-  _BINARYMETRICS._serialized_start=16628
-  _BINARYMETRICS._serialized_end=16990
-  _TRACKERMETRICS._serialized_start=16993
-  _TRACKERMETRICS._serialized_end=17138
-  _EVALTESTSETENTRY._serialized_start=17141
-  _EVALTESTSETENTRY._serialized_end=17358
-  _LOPQEVALRESULT._serialized_start=17361
-  _LOPQEVALRESULT._serialized_end=17566
-  _METRICSSUMMARY._serialized_start=17569
-  _METRICSSUMMARY._serialized_end=17965
-  _EVALMETRICS._serialized_start=17968
-  _EVALMETRICS._serialized_end=18570
-  _FIELDSVALUE._serialized_start=18573
-  _FIELDSVALUE._serialized_end=18756
-  _OUTPUT._serialized_start=18759
-  _OUTPUT._serialized_end=18978
-  _SCOPEDEPS._serialized_start=18980
-  _SCOPEDEPS._serialized_end=19032
-  _ENDPOINTDEPS._serialized_start=19034
-  _ENDPOINTDEPS._serialized_end=19092
-  _HIT._serialized_start=19095
-  _HIT._serialized_end=19236
-  _HITCOUNT._serialized_start=19238
-  _HITCOUNT._serialized_end=19273
-  _AND._serialized_start=19276
-  _AND._serialized_end=19417
-  _QUERY._serialized_start=19420
-  _QUERY._serialized_end=19556
-  _SEARCH._serialized_start=19559
-  _SEARCH._serialized_end=20029
-  _SEARCH_METRIC._serialized_start=19956
-  _SEARCH_METRIC._serialized_end=20029
-  _FILTER._serialized_start=20032
-  _FILTER._serialized_end=20196
-  _TIMERANGE._serialized_start=20198
-  _TIMERANGE._serialized_end=20303
-  _RANK._serialized_start=20305
-  _RANK._serialized_end=20373
-  _ANNOTATIONSEARCHMETRICS._serialized_start=20376
-  _ANNOTATIONSEARCHMETRICS._serialized_end=20645
-  _TEXT._serialized_start=20648
-  _TEXT._serialized_end=20793
-  _TEXTINFO._serialized_start=20795
-  _TEXTINFO._serialized_end=20843
-  _USER._serialized_start=20846
-  _USER._serialized_end=21610
-  _USERDETAIL._serialized_start=21613
-  _USERDETAIL._serialized_end=22078
-  _EMAILADDRESS._serialized_start=22080
-  _EMAILADDRESS._serialized_end=22162
-  _PASSWORD._serialized_start=22164
-  _PASSWORD._serialized_end=22193
-  _PASSWORDVIOLATIONS._serialized_start=22196
-  _PASSWORDVIOLATIONS._serialized_end=22586
-  _VIDEO._serialized_start=22589
-  _VIDEO._serialized_end=22763
-  _VIDEOINFO._serialized_start=22766
-  _VIDEOINFO._serialized_end=22908
-  _WORKFLOW._serialized_start=22911
-  _WORKFLOW._serialized_end=23374
-  _WORKFLOWVERSION._serialized_start=23377
-  _WORKFLOWVERSION._serialized_end=23727
-  _WORKFLOWNODE._serialized_start=23730
-  _WORKFLOWNODE._serialized_end=23919
-  _NODEINPUT._serialized_start=23921
-  _NODEINPUT._serialized_end=23949
-  _WORKFLOWRESULT._serialized_start=23952
-  _WORKFLOWRESULT._serialized_end=24209
-  _WORKFLOWSTATE._serialized_start=24211
-  _WORKFLOWSTATE._serialized_end=24238
-  _APPDUPLICATION._serialized_start=24241
-  _APPDUPLICATION._serialized_end=24585
-  _APPCOPYPROGRESS._serialized_start=24587
-  _APPCOPYPROGRESS._serialized_end=24634
-  _APPDUPLICATIONFILTERS._serialized_start=24637
-  _APPDUPLICATIONFILTERS._serialized_end=24775
-  _LABELORDER._serialized_start=24778
-  _LABELORDER._serialized_end=25156
-  _TASK._serialized_start=25159
-  _TASK._serialized_end=25982
-  _TASK_TASKTYPE._serialized_start=25874
-  _TASK_TASKTYPE._serialized_end=25982
-  _AIASSISTPARAMETERS._serialized_start=25984
-  _AIASSISTPARAMETERS._serialized_end=26080
-  _TASKWORKER._serialized_start=26083
-  _TASKWORKER._serialized_end=26482
-  _TASKWORKER_TASKWORKERSTRATEGY._serialized_start=26383
-  _TASKWORKER_TASKWORKERSTRATEGY._serialized_end=26465
-  _TASKWORKERPARTITIONEDSTRATEGYINFO._serialized_start=26485
-  _TASKWORKERPARTITIONEDSTRATEGYINFO._serialized_end=26782
-  _TASKWORKERPARTITIONEDSTRATEGYINFO_TASKWORKERPARTITIONEDSTRATEGY._serialized_start=26684
-  _TASKWORKERPARTITIONEDSTRATEGYINFO_TASKWORKERPARTITIONEDSTRATEGY._serialized_end=26782
-  _TASKINPUTSOURCE._serialized_start=26785
-  _TASKINPUTSOURCE._serialized_end=26980
-  _TASKINPUTSOURCE_TASKINPUTSOURCETYPE._serialized_start=26881
-  _TASKINPUTSOURCE_TASKINPUTSOURCETYPE._serialized_end=26980
-  _TASKREVIEW._serialized_start=26983
-  _TASKREVIEW._serialized_end=27383
-  _TASKREVIEW_TASKREVIEWSTRATEGY._serialized_start=27275
-  _TASKREVIEW_TASKREVIEWSTRATEGY._serialized_end=27366
-  _TASKREVIEWMANUALSTRATEGYINFO._serialized_start=27385
-  _TASKREVIEWMANUALSTRATEGYINFO._serialized_end=27442
-  _TASKREVIEWCONSENSUSSTRATEGYINFO._serialized_start=27444
-  _TASKREVIEWCONSENSUSSTRATEGYINFO._serialized_end=27511
-  _TASKAIASSISTANT._serialized_start=27513
-  _TASKAIASSISTANT._serialized_end=27551
-  _TASKSTATUSCOUNTPERUSER._serialized_start=27554
-  _TASKSTATUSCOUNTPERUSER._serialized_end=27742
-  _THRESHOLDRANGE._serialized_start=27744
-  _THRESHOLDRANGE._serialized_end=27846
-  _TASKCONCEPTAUTOANNOTATIONCONFIG._serialized_start=27849
-  _TASKCONCEPTAUTOANNOTATIONCONFIG._serialized_end=28022
-  _TASKCONCEPT._serialized_start=28025
-  _TASKCONCEPT._serialized_end=28157
-  _COLLECTOR._serialized_start=28160
-  _COLLECTOR._serialized_end=28417
-  _COLLECTORSOURCE._serialized_start=28419
-  _COLLECTORSOURCE._serialized_end=28535
-  _APIPOSTMODELOUTPUTSCOLLECTORSOURCE._serialized_start=28538
-  _APIPOSTMODELOUTPUTSCOLLECTORSOURCE._serialized_end=28691
-  _STATVALUE._serialized_start=28693
-  _STATVALUE._serialized_end=28775
-  _STATVALUEAGGREGATERESULT._serialized_start=28778
-  _STATVALUEAGGREGATERESULT._serialized_end=28944
-  _STATVALUEAGGREGATE._serialized_start=28946
-  _STATVALUEAGGREGATE._serialized_end=29062
-  _STATVALUEAGGREGATEQUERY._serialized_start=29065
-  _STATVALUEAGGREGATEQUERY._serialized_end=29338
-  _DATASETINPUTSSEARCHADDJOB._serialized_start=29341
-  _DATASETINPUTSSEARCHADDJOB._serialized_end=29580
-  _PCAPROJECTIONCOMPARATOR._serialized_start=29582
-  _PCAPROJECTIONCOMPARATOR._serialized_end=29661
-  _DUPLICATEANNOTATIONSRESULTS._serialized_start=29663
-  _DUPLICATEANNOTATIONSRESULTS._serialized_end=29738
-  _VISIBILITY._serialized_start=29741
-  _VISIBILITY._serialized_end=29876
-  _VISIBILITY_GETTABLE._serialized_start=29808
-  _VISIBILITY_GETTABLE._serialized_end=29876
-  _TRENDINGMETRIC._serialized_start=29878
-  _TRENDINGMETRIC._serialized_end=29966
-  _FULLTAG._serialized_start=29968
-  _FULLTAG._serialized_end=30003
-  _TIMESEGMENT._serialized_start=30005
-  _TIMESEGMENT._serialized_end=30107
-  _TIMEINFO._serialized_start=30109
-  _TIMEINFO._serialized_end=30177
-  _DATASETSTAR._serialized_start=30179
-  _DATASETSTAR._serialized_end=30212
-  _MODULESTAR._serialized_start=30214
-  _MODULESTAR._serialized_end=30245
-  _MODULE._serialized_start=30248
-  _MODULE._serialized_end=30607
-  _MODULEVERSION._serialized_start=30610
-  _MODULEVERSION._serialized_end=31184
-  _MODULEVERSION_MODULESUBNAV._serialized_start=31014
-  _MODULEVERSION_MODULESUBNAV._serialized_end=31083
-  _MODULEVERSION_MODULENAV._serialized_start=31085
-  _MODULEVERSION_MODULENAV._serialized_end=31178
-  _INSTALLEDMODULEVERSION._serialized_start=31187
-  _INSTALLEDMODULEVERSION._serialized_end=31488
-  _BULKOPERATION._serialized_start=31491
-  _BULKOPERATION._serialized_end=31930
-  _INPUTIDS._serialized_start=31932
-  _INPUTIDS._serialized_end=31961
-  _PROGRESS._serialized_start=31963
-  _PROGRESS._serialized_end=32019
-  _OPERATION._serialized_start=32022
-  _OPERATION._serialized_end=32544
-  _ADDCONCEPTS._serialized_start=32546
-  _ADDCONCEPTS._serialized_end=32600
-  _DELETECONCEPTS._serialized_start=32602
-  _DELETECONCEPTS._serialized_end=32677
-  _ADDMETADATA._serialized_start=32679
-  _ADDMETADATA._serialized_end=32735
-  _DELETEMETADATA._serialized_start=32737
-  _DELETEMETADATA._serialized_end=32796
-  _OVERWRITEGEO._serialized_start=32798
-  _OVERWRITEGEO._serialized_end=32844
-  _DELETEGEO._serialized_start=32846
-  _DELETEGEO._serialized_end=32857
-  _ADDTODATASET._serialized_start=32859
-  _ADDTODATASET._serialized_end=32893
-  _DELETEFROMDATASET._serialized_start=32895
-  _DELETEFROMDATASET._serialized_end=32934
-  _SPLITINTODATASETS._serialized_start=32937
-  _SPLITINTODATASETS._serialized_end=33140
-  _SPLITINTODATASETS_DATASETSPLITMETHOD._serialized_start=33078
-  _SPLITINTODATASETS_DATASETSPLITMETHOD._serialized_end=33140
-  _DATASETSPLIT._serialized_start=33142
-  _DATASETSPLIT._serialized_end=33233
-  _INPUTSADDJOB._serialized_start=33236
-  _INPUTSADDJOB._serialized_end=33570
-  _INPUTSADDJOBPROGRESS._serialized_start=33572
-  _INPUTSADDJOBPROGRESS._serialized_end=33689
-  _UPLOAD._serialized_start=33692
-  _UPLOAD._serialized_end=33969
-  _UPLOADCONTENTPART._serialized_start=33971
-  _UPLOADCONTENTPART._serialized_end=34046
-  _CUSTOMCODEOPERATORREQUEST._serialized_start=34048
-  _CUSTOMCODEOPERATORREQUEST._serialized_end=34156
-  _INPUTSEXTRACTIONJOB._serialized_start=34159
-  _INPUTSEXTRACTIONJOB._serialized_end=34408
-  _INPUTSEXTRACTIONJOBPROGRESS._serialized_start=34411
-  _INPUTSEXTRACTIONJOBPROGRESS._serialized_end=34712
-  _INPUTSDATASOURCE._serialized_start=34714
-  _INPUTSDATASOURCE._serialized_end=34801
-  _DATASOURCEURL._serialized_start=34803
-  _DATASOURCEURL._serialized_end=34889
-  _DATASOURCECREDENTIALS._serialized_start=34892
-  _DATASOURCECREDENTIALS._serialized_end=35059
-  _AWSCREDS._serialized_start=35061
-  _AWSCREDS._serialized_end=35136
-  _AZUREBLOBCREDS._serialized_start=35138
-  _AZUREBLOBCREDS._serialized_end=35197
-  _INPUTSUPLOAD._serialized_start=35199
-  _INPUTSUPLOAD._serialized_end=35295
+  _DATASETVERSION._serialized_end=8557
+  _DATASETVERSION_METRICSENTRY._serialized_start=8441
+  _DATASETVERSION_METRICSENTRY._serialized_end=8524
+  _ANNOTATIONFILTERCONFIG._serialized_start=8559
+  _ANNOTATIONFILTERCONFIG._serialized_end=8671
+  _MODELPREDICTCONFIG._serialized_start=8673
+  _MODELPREDICTCONFIG._serialized_end=8729
+  _DATASETVERSIONMETRICS._serialized_start=8732
+  _DATASETVERSIONMETRICS._serialized_end=9823
+  _DATASETVERSIONMETRICSGROUP._serialized_start=9826
+  _DATASETVERSIONMETRICSGROUP._serialized_end=10028
+  _DATASETVERSIONEXPORTINFO._serialized_start=10031
+  _DATASETVERSIONEXPORTINFO._serialized_end=10239
+  _DATASETVERSIONEXPORT._serialized_start=10242
+  _DATASETVERSIONEXPORT._serialized_end=10422
+  _DATASETVERSIONPROCESSINGINFO._serialized_start=10424
+  _DATASETVERSIONPROCESSINGINFO._serialized_end=10526
+  _FRAMEINTERPOLATIONINFO._serialized_start=10528
+  _FRAMEINTERPOLATIONINFO._serialized_end=10571
+  _WORKFLOWRESULTSSIMILARITY._serialized_start=10573
+  _WORKFLOWRESULTSSIMILARITY._serialized_end=10683
+  _KEY._serialized_start=10686
+  _KEY._serialized_end=10930
+  _MODEL._serialized_start=10933
+  _MODEL._serialized_end=11917
+  _MODELREFERENCE._serialized_start=11919
+  _MODELREFERENCE._serialized_end=12035
+  _MODELVERSIONINPUTEXAMPLE._serialized_start=12038
+  _MODELVERSIONINPUTEXAMPLE._serialized_end=12189
+  _OUTPUTINFO._serialized_start=12192
+  _OUTPUTINFO._serialized_end=12404
+  _INPUTINFO._serialized_start=12406
+  _INPUTINFO._serialized_end=12503
+  _TRAININFO._serialized_start=12505
+  _TRAININFO._serialized_end=12557
+  _EVALINFO._serialized_start=12559
+  _EVALINFO._serialized_end=12610
+  _IMPORTINFO._serialized_start=12612
+  _IMPORTINFO._serialized_end=12665
+  _OUTPUTCONFIG._serialized_start=12668
+  _OUTPUTCONFIG._serialized_end=13147
+  _MODELTYPE._serialized_start=13150
+  _MODELTYPE._serialized_end=13616
+  _MODELLAYERINFO._serialized_start=13619
+  _MODELLAYERINFO._serialized_end=13756
+  _TRITONCONDAENVINFO._serialized_start=13758
+  _TRITONCONDAENVINFO._serialized_end=13826
+  _LAYERSHAPE._serialized_start=13828
+  _LAYERSHAPE._serialized_end=13936
+  _MODELTYPEFIELD._serialized_start=13939
+  _MODELTYPEFIELD._serialized_end=14661
+  _MODELTYPEFIELD_MODELTYPEFIELDTYPE._serialized_start=14304
+  _MODELTYPEFIELD_MODELTYPEFIELDTYPE._serialized_end=14661
+  _MODELTYPERANGEINFO._serialized_start=14663
+  _MODELTYPERANGEINFO._serialized_end=14723
+  _MODELTYPEENUMOPTION._serialized_start=14726
+  _MODELTYPEENUMOPTION._serialized_end=14938
+  _MODELTYPEENUMOPTIONALIAS._serialized_start=14940
+  _MODELTYPEENUMOPTIONALIAS._serialized_end=15007
+  _MODELQUERY._serialized_start=15009
+  _MODELQUERY._serialized_end=15064
+  _MODELVERSION._serialized_start=15067
+  _MODELVERSION._serialized_end=15831
+  _PRETRAINEDMODELCONFIG._serialized_start=15834
+  _PRETRAINEDMODELCONFIG._serialized_end=15995
+  _TRAINSTATS._serialized_start=15997
+  _TRAINSTATS._serialized_end=16059
+  _LOSSCURVEENTRY._serialized_start=16061
+  _LOSSCURVEENTRY._serialized_end=16127
+  _LABELCOUNT._serialized_start=16129
+  _LABELCOUNT._serialized_end=16178
+  _LABELDISTRIBUTION._serialized_start=16180
+  _LABELDISTRIBUTION._serialized_end=16256
+  _COOCCURRENCEMATRIXENTRY._serialized_start=16258
+  _COOCCURRENCEMATRIXENTRY._serialized_end=16324
+  _COOCCURRENCEMATRIX._serialized_start=16326
+  _COOCCURRENCEMATRIX._serialized_end=16422
+  _CONFUSIONMATRIXENTRY._serialized_start=16424
+  _CONFUSIONMATRIXENTRY._serialized_end=16502
+  _CONFUSIONMATRIX._serialized_start=16504
+  _CONFUSIONMATRIX._serialized_end=16594
+  _ROC._serialized_start=16596
+  _ROC._serialized_end=16712
+  _PRECISIONRECALLCURVE._serialized_start=16714
+  _PRECISIONRECALLCURVE._serialized_end=16809
+  _BINARYMETRICS._serialized_start=16812
+  _BINARYMETRICS._serialized_end=17174
+  _TRACKERMETRICS._serialized_start=17177
+  _TRACKERMETRICS._serialized_end=17322
+  _EVALTESTSETENTRY._serialized_start=17325
+  _EVALTESTSETENTRY._serialized_end=17542
+  _LOPQEVALRESULT._serialized_start=17545
+  _LOPQEVALRESULT._serialized_end=17750
+  _METRICSSUMMARY._serialized_start=17753
+  _METRICSSUMMARY._serialized_end=18149
+  _EVALMETRICS._serialized_start=18152
+  _EVALMETRICS._serialized_end=18876
+  _FIELDSVALUE._serialized_start=18879
+  _FIELDSVALUE._serialized_end=19062
+  _OUTPUT._serialized_start=19065
+  _OUTPUT._serialized_end=19284
+  _SCOPEDEPS._serialized_start=19286
+  _SCOPEDEPS._serialized_end=19338
+  _ENDPOINTDEPS._serialized_start=19340
+  _ENDPOINTDEPS._serialized_end=19398
+  _HIT._serialized_start=19401
+  _HIT._serialized_end=19542
+  _HITCOUNT._serialized_start=19544
+  _HITCOUNT._serialized_end=19579
+  _AND._serialized_start=19582
+  _AND._serialized_end=19723
+  _QUERY._serialized_start=19726
+  _QUERY._serialized_end=19862
+  _SEARCH._serialized_start=19865
+  _SEARCH._serialized_end=20335
+  _SEARCH_METRIC._serialized_start=20262
+  _SEARCH_METRIC._serialized_end=20335
+  _FILTER._serialized_start=20338
+  _FILTER._serialized_end=20502
+  _TIMERANGE._serialized_start=20504
+  _TIMERANGE._serialized_end=20609
+  _RANK._serialized_start=20611
+  _RANK._serialized_end=20679
+  _ANNOTATIONSEARCHMETRICS._serialized_start=20682
+  _ANNOTATIONSEARCHMETRICS._serialized_end=20951
+  _TEXT._serialized_start=20954
+  _TEXT._serialized_end=21099
+  _TEXTINFO._serialized_start=21101
+  _TEXTINFO._serialized_end=21149
+  _USER._serialized_start=21152
+  _USER._serialized_end=21916
+  _USERDETAIL._serialized_start=21919
+  _USERDETAIL._serialized_end=22384
+  _EMAILADDRESS._serialized_start=22386
+  _EMAILADDRESS._serialized_end=22468
+  _PASSWORD._serialized_start=22470
+  _PASSWORD._serialized_end=22499
+  _PASSWORDVIOLATIONS._serialized_start=22502
+  _PASSWORDVIOLATIONS._serialized_end=22892
+  _VIDEO._serialized_start=22895
+  _VIDEO._serialized_end=23069
+  _VIDEOINFO._serialized_start=23072
+  _VIDEOINFO._serialized_end=23214
+  _WORKFLOW._serialized_start=23217
+  _WORKFLOW._serialized_end=23680
+  _WORKFLOWVERSION._serialized_start=23683
+  _WORKFLOWVERSION._serialized_end=24033
+  _WORKFLOWNODE._serialized_start=24036
+  _WORKFLOWNODE._serialized_end=24225
+  _NODEINPUT._serialized_start=24227
+  _NODEINPUT._serialized_end=24255
+  _WORKFLOWRESULT._serialized_start=24258
+  _WORKFLOWRESULT._serialized_end=24515
+  _WORKFLOWSTATE._serialized_start=24517
+  _WORKFLOWSTATE._serialized_end=24544
+  _APPDUPLICATION._serialized_start=24547
+  _APPDUPLICATION._serialized_end=24891
+  _APPCOPYPROGRESS._serialized_start=24893
+  _APPCOPYPROGRESS._serialized_end=24940
+  _APPDUPLICATIONFILTERS._serialized_start=24943
+  _APPDUPLICATIONFILTERS._serialized_end=25081
+  _LABELORDER._serialized_start=25084
+  _LABELORDER._serialized_end=25462
+  _TASK._serialized_start=25465
+  _TASK._serialized_end=26288
+  _TASK_TASKTYPE._serialized_start=26180
+  _TASK_TASKTYPE._serialized_end=26288
+  _AIASSISTPARAMETERS._serialized_start=26290
+  _AIASSISTPARAMETERS._serialized_end=26386
+  _TASKWORKER._serialized_start=26389
+  _TASKWORKER._serialized_end=26788
+  _TASKWORKER_TASKWORKERSTRATEGY._serialized_start=26689
+  _TASKWORKER_TASKWORKERSTRATEGY._serialized_end=26771
+  _TASKWORKERPARTITIONEDSTRATEGYINFO._serialized_start=26791
+  _TASKWORKERPARTITIONEDSTRATEGYINFO._serialized_end=27088
+  _TASKWORKERPARTITIONEDSTRATEGYINFO_TASKWORKERPARTITIONEDSTRATEGY._serialized_start=26990
+  _TASKWORKERPARTITIONEDSTRATEGYINFO_TASKWORKERPARTITIONEDSTRATEGY._serialized_end=27088
+  _TASKINPUTSOURCE._serialized_start=27091
+  _TASKINPUTSOURCE._serialized_end=27286
+  _TASKINPUTSOURCE_TASKINPUTSOURCETYPE._serialized_start=27187
+  _TASKINPUTSOURCE_TASKINPUTSOURCETYPE._serialized_end=27286
+  _TASKREVIEW._serialized_start=27289
+  _TASKREVIEW._serialized_end=27689
+  _TASKREVIEW_TASKREVIEWSTRATEGY._serialized_start=27581
+  _TASKREVIEW_TASKREVIEWSTRATEGY._serialized_end=27672
+  _TASKREVIEWMANUALSTRATEGYINFO._serialized_start=27691
+  _TASKREVIEWMANUALSTRATEGYINFO._serialized_end=27748
+  _TASKREVIEWCONSENSUSSTRATEGYINFO._serialized_start=27750
+  _TASKREVIEWCONSENSUSSTRATEGYINFO._serialized_end=27817
+  _TASKAIASSISTANT._serialized_start=27819
+  _TASKAIASSISTANT._serialized_end=27857
+  _TASKSTATUSCOUNTPERUSER._serialized_start=27860
+  _TASKSTATUSCOUNTPERUSER._serialized_end=28048
+  _THRESHOLDRANGE._serialized_start=28050
+  _THRESHOLDRANGE._serialized_end=28152
+  _TASKCONCEPTAUTOANNOTATIONCONFIG._serialized_start=28155
+  _TASKCONCEPTAUTOANNOTATIONCONFIG._serialized_end=28328
+  _TASKCONCEPT._serialized_start=28331
+  _TASKCONCEPT._serialized_end=28463
+  _COLLECTOR._serialized_start=28466
+  _COLLECTOR._serialized_end=28723
+  _COLLECTORSOURCE._serialized_start=28725
+  _COLLECTORSOURCE._serialized_end=28841
+  _APIPOSTMODELOUTPUTSCOLLECTORSOURCE._serialized_start=28844
+  _APIPOSTMODELOUTPUTSCOLLECTORSOURCE._serialized_end=28997
+  _STATVALUE._serialized_start=28999
+  _STATVALUE._serialized_end=29081
+  _STATVALUEAGGREGATERESULT._serialized_start=29084
+  _STATVALUEAGGREGATERESULT._serialized_end=29250
+  _STATVALUEAGGREGATE._serialized_start=29252
+  _STATVALUEAGGREGATE._serialized_end=29368
+  _STATVALUEAGGREGATEQUERY._serialized_start=29371
+  _STATVALUEAGGREGATEQUERY._serialized_end=29644
+  _DATASETINPUTSSEARCHADDJOB._serialized_start=29647
+  _DATASETINPUTSSEARCHADDJOB._serialized_end=29886
+  _PCAPROJECTIONCOMPARATOR._serialized_start=29888
+  _PCAPROJECTIONCOMPARATOR._serialized_end=29967
+  _DUPLICATEANNOTATIONSRESULTS._serialized_start=29969
+  _DUPLICATEANNOTATIONSRESULTS._serialized_end=30044
+  _VISIBILITY._serialized_start=30047
+  _VISIBILITY._serialized_end=30182
+  _VISIBILITY_GETTABLE._serialized_start=30114
+  _VISIBILITY_GETTABLE._serialized_end=30182
+  _TRENDINGMETRIC._serialized_start=30184
+  _TRENDINGMETRIC._serialized_end=30272
+  _FULLTAG._serialized_start=30274
+  _FULLTAG._serialized_end=30309
+  _TIMESEGMENT._serialized_start=30311
+  _TIMESEGMENT._serialized_end=30413
+  _TIMEINFO._serialized_start=30415
+  _TIMEINFO._serialized_end=30483
+  _DATASETSTAR._serialized_start=30485
+  _DATASETSTAR._serialized_end=30518
+  _MODULESTAR._serialized_start=30520
+  _MODULESTAR._serialized_end=30551
+  _MODULE._serialized_start=30554
+  _MODULE._serialized_end=30913
+  _MODULEVERSION._serialized_start=30916
+  _MODULEVERSION._serialized_end=31490
+  _MODULEVERSION_MODULESUBNAV._serialized_start=31320
+  _MODULEVERSION_MODULESUBNAV._serialized_end=31389
+  _MODULEVERSION_MODULENAV._serialized_start=31391
+  _MODULEVERSION_MODULENAV._serialized_end=31484
+  _INSTALLEDMODULEVERSION._serialized_start=31493
+  _INSTALLEDMODULEVERSION._serialized_end=31794
+  _BULKOPERATION._serialized_start=31797
+  _BULKOPERATION._serialized_end=32236
+  _INPUTIDS._serialized_start=32238
+  _INPUTIDS._serialized_end=32267
+  _PROGRESS._serialized_start=32269
+  _PROGRESS._serialized_end=32325
+  _OPERATION._serialized_start=32328
+  _OPERATION._serialized_end=32850
+  _ADDCONCEPTS._serialized_start=32852
+  _ADDCONCEPTS._serialized_end=32906
+  _DELETECONCEPTS._serialized_start=32908
+  _DELETECONCEPTS._serialized_end=32983
+  _ADDMETADATA._serialized_start=32985
+  _ADDMETADATA._serialized_end=33041
+  _DELETEMETADATA._serialized_start=33043
+  _DELETEMETADATA._serialized_end=33102
+  _OVERWRITEGEO._serialized_start=33104
+  _OVERWRITEGEO._serialized_end=33150
+  _DELETEGEO._serialized_start=33152
+  _DELETEGEO._serialized_end=33163
+  _ADDTODATASET._serialized_start=33165
+  _ADDTODATASET._serialized_end=33199
+  _DELETEFROMDATASET._serialized_start=33201
+  _DELETEFROMDATASET._serialized_end=33240
+  _SPLITINTODATASETS._serialized_start=33243
+  _SPLITINTODATASETS._serialized_end=33446
+  _SPLITINTODATASETS_DATASETSPLITMETHOD._serialized_start=33384
+  _SPLITINTODATASETS_DATASETSPLITMETHOD._serialized_end=33446
+  _DATASETSPLIT._serialized_start=33448
+  _DATASETSPLIT._serialized_end=33539
+  _INPUTSADDJOB._serialized_start=33542
+  _INPUTSADDJOB._serialized_end=33921
+  _INPUTSADDJOBPROGRESS._serialized_start=33923
+  _INPUTSADDJOBPROGRESS._serialized_end=34040
+  _UPLOAD._serialized_start=34043
+  _UPLOAD._serialized_end=34320
+  _UPLOADCONTENTPART._serialized_start=34322
+  _UPLOADCONTENTPART._serialized_end=34397
+  _CUSTOMCODEOPERATORREQUEST._serialized_start=34399
+  _CUSTOMCODEOPERATORREQUEST._serialized_end=34507
+  _INPUTSEXTRACTIONJOB._serialized_start=34510
+  _INPUTSEXTRACTIONJOB._serialized_end=34838
+  _INPUTSEXTRACTIONJOBPROGRESS._serialized_start=34841
+  _INPUTSEXTRACTIONJOBPROGRESS._serialized_end=35120
+  _INPUTSDATASOURCE._serialized_start=35123
+  _INPUTSDATASOURCE._serialized_end=35289
+  _DATASOURCEURL._serialized_start=35291
+  _DATASOURCEURL._serialized_end=35377
+  _DATASOURCECREDENTIALS._serialized_start=35380
+  _DATASOURCECREDENTIALS._serialized_end=35547
+  _AWSCREDS._serialized_start=35549
+  _AWSCREDS._serialized_end=35624
+  _AZUREBLOBCREDS._serialized_start=35626
+  _AZUREBLOBCREDS._serialized_end=35685
+  _INPUTSUPLOAD._serialized_start=35688
+  _INPUTSUPLOAD._serialized_end=35863
 # @@protoc_insertion_point(module_scope)
```

### Comparing `clarifai-grpc-9.5.0/clarifai_grpc/grpc/api/resources_pb2.pyi` & `clarifai-grpc-9.6.0/clarifai_grpc/grpc/api/resources_pb2.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -328,28 +328,30 @@
 class _AnnotationDataType:
     ValueType = typing.NewType("ValueType", builtins.int)
     V: typing_extensions.TypeAlias = ValueType
 
 class _AnnotationDataTypeEnumTypeWrapper(google.protobuf.internal.enum_type_wrapper._EnumTypeWrapper[_AnnotationDataType.ValueType], builtins.type):
     DESCRIPTOR: google.protobuf.descriptor.EnumDescriptor
     ANNOTATION_DATA_TYPE_NOT_SET: _AnnotationDataType.ValueType  # 0
-    BOUNDING_BOX: _AnnotationDataType.ValueType  # 1
-    POLYGON: _AnnotationDataType.ValueType  # 2
-    POINT: _AnnotationDataType.ValueType  # 4
-    SPAN: _AnnotationDataType.ValueType  # 8
-    MASK: _AnnotationDataType.ValueType  # 16
+    TAG: _AnnotationDataType.ValueType  # 1
+    BOUNDING_BOX: _AnnotationDataType.ValueType  # 2
+    POLYGON: _AnnotationDataType.ValueType  # 4
+    POINT: _AnnotationDataType.ValueType  # 8
+    SPAN: _AnnotationDataType.ValueType  # 16
+    MASK: _AnnotationDataType.ValueType  # 32
 
 class AnnotationDataType(_AnnotationDataType, metaclass=_AnnotationDataTypeEnumTypeWrapper): ...
 
 ANNOTATION_DATA_TYPE_NOT_SET: AnnotationDataType.ValueType  # 0
-BOUNDING_BOX: AnnotationDataType.ValueType  # 1
-POLYGON: AnnotationDataType.ValueType  # 2
-POINT: AnnotationDataType.ValueType  # 4
-SPAN: AnnotationDataType.ValueType  # 8
-MASK: AnnotationDataType.ValueType  # 16
+TAG: AnnotationDataType.ValueType  # 1
+BOUNDING_BOX: AnnotationDataType.ValueType  # 2
+POLYGON: AnnotationDataType.ValueType  # 4
+POINT: AnnotationDataType.ValueType  # 8
+SPAN: AnnotationDataType.ValueType  # 16
+MASK: AnnotationDataType.ValueType  # 32
 global___AnnotationDataType = AnnotationDataType
 
 class _RoleType:
     ValueType = typing.NewType("ValueType", builtins.int)
     V: typing_extensions.TypeAlias = ValueType
 
 class _RoleTypeEnumTypeWrapper(google.protobuf.internal.enum_type_wrapper._EnumTypeWrapper[_RoleType.ValueType], builtins.type):
@@ -418,14 +420,37 @@
 
 VALIDATION_ERROR_TYPE_NOT_SET: ValidationErrorType.ValueType  # 0
 RESTRICTED: ValidationErrorType.ValueType  # 1
 DATABASE: ValidationErrorType.ValueType  # 2
 FORMAT: ValidationErrorType.ValueType  # 3
 global___ValidationErrorType = ValidationErrorType
 
+class _InputIDConflictResolution:
+    ValueType = typing.NewType("ValueType", builtins.int)
+    V: typing_extensions.TypeAlias = ValueType
+
+class _InputIDConflictResolutionEnumTypeWrapper(google.protobuf.internal.enum_type_wrapper._EnumTypeWrapper[_InputIDConflictResolution.ValueType], builtins.type):
+    DESCRIPTOR: google.protobuf.descriptor.EnumDescriptor
+    INPUT_ID_CONFLICT_RESOLUTION_NOT_SET: _InputIDConflictResolution.ValueType  # 0
+    """Defaults to SKIP"""
+    SKIP: _InputIDConflictResolution.ValueType  # 1
+    """Mark duplicate inputs as error and skip processing them."""
+    SUFFIX: _InputIDConflictResolution.ValueType  # 2
+    """Add a suffix to inputs with conflicting IDs. Attempts numeric suffixes "-1" to "-9" and then a randomized suffix. Identical ID's in the same request are still treated as errors."""
+
+class InputIDConflictResolution(_InputIDConflictResolution, metaclass=_InputIDConflictResolutionEnumTypeWrapper): ...
+
+INPUT_ID_CONFLICT_RESOLUTION_NOT_SET: InputIDConflictResolution.ValueType  # 0
+"""Defaults to SKIP"""
+SKIP: InputIDConflictResolution.ValueType  # 1
+"""Mark duplicate inputs as error and skip processing them."""
+SUFFIX: InputIDConflictResolution.ValueType  # 2
+"""Add a suffix to inputs with conflicting IDs. Attempts numeric suffixes "-1" to "-9" and then a randomized suffix. Identical ID's in the same request are still treated as errors."""
+global___InputIDConflictResolution = InputIDConflictResolution
+
 @typing_extensions.final
 class Annotation(google.protobuf.message.Message):
     """Annotation of an asset with metadata"""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     ID_FIELD_NUMBER: builtins.int
@@ -2384,14 +2409,15 @@
     APP_ID_FIELD_NUMBER: builtins.int
     USER_ID_FIELD_NUMBER: builtins.int
     DATASET_ID_FIELD_NUMBER: builtins.int
     ANNOTATION_FILTER_CONFIG_FIELD_NUMBER: builtins.int
     MODEL_PREDICT_CONFIG_FIELD_NUMBER: builtins.int
     STATUS_FIELD_NUMBER: builtins.int
     DESCRIPTION_FIELD_NUMBER: builtins.int
+    PROCESSING_INFO_FIELD_NUMBER: builtins.int
     METRICS_FIELD_NUMBER: builtins.int
     EXPORT_INFO_FIELD_NUMBER: builtins.int
     METADATA_FIELD_NUMBER: builtins.int
     VISIBILITY_FIELD_NUMBER: builtins.int
     EMBED_MODEL_VERSION_IDS_FIELD_NUMBER: builtins.int
     id: builtins.str
     """The ID for the dataset version"""
@@ -2421,14 +2447,17 @@
         """The dataset version will be generated based on model version inferences."""
     @property
     def status(self) -> proto.clarifai.api.status.status_pb2.Status:
         """Status for this dataset version."""
     description: builtins.str
     """Description of the dataset version"""
     @property
+    def processing_info(self) -> global___DatasetVersionProcessingInfo:
+        """Dataset version processing"""
+    @property
     def metrics(self) -> google.protobuf.internal.containers.MessageMap[builtins.str, global___DatasetVersionMetrics]:
         """Dataset version metrics"""
     @property
     def export_info(self) -> global___DatasetVersionExportInfo:
         """Dataset version exports"""
     @property
     def metadata(self) -> google.protobuf.struct_pb2.Struct:
@@ -2453,22 +2482,23 @@
         app_id: builtins.str = ...,
         user_id: builtins.str = ...,
         dataset_id: builtins.str = ...,
         annotation_filter_config: global___AnnotationFilterConfig | None = ...,
         model_predict_config: global___ModelPredictConfig | None = ...,
         status: proto.clarifai.api.status.status_pb2.Status | None = ...,
         description: builtins.str = ...,
+        processing_info: global___DatasetVersionProcessingInfo | None = ...,
         metrics: collections.abc.Mapping[builtins.str, global___DatasetVersionMetrics] | None = ...,
         export_info: global___DatasetVersionExportInfo | None = ...,
         metadata: google.protobuf.struct_pb2.Struct | None = ...,
         visibility: global___Visibility | None = ...,
         embed_model_version_ids: collections.abc.Iterable[builtins.str] | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["annotation_filter_config", b"annotation_filter_config", "created_at", b"created_at", "data_config", b"data_config", "export_info", b"export_info", "metadata", b"metadata", "model_predict_config", b"model_predict_config", "modified_at", b"modified_at", "status", b"status", "visibility", b"visibility"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["annotation_filter_config", b"annotation_filter_config", "app_id", b"app_id", "created_at", b"created_at", "data_config", b"data_config", "dataset_id", b"dataset_id", "description", b"description", "embed_model_version_ids", b"embed_model_version_ids", "export_info", b"export_info", "id", b"id", "metadata", b"metadata", "metrics", b"metrics", "model_predict_config", b"model_predict_config", "modified_at", b"modified_at", "status", b"status", "user_id", b"user_id", "visibility", b"visibility"]) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["annotation_filter_config", b"annotation_filter_config", "created_at", b"created_at", "data_config", b"data_config", "export_info", b"export_info", "metadata", b"metadata", "model_predict_config", b"model_predict_config", "modified_at", b"modified_at", "processing_info", b"processing_info", "status", b"status", "visibility", b"visibility"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["annotation_filter_config", b"annotation_filter_config", "app_id", b"app_id", "created_at", b"created_at", "data_config", b"data_config", "dataset_id", b"dataset_id", "description", b"description", "embed_model_version_ids", b"embed_model_version_ids", "export_info", b"export_info", "id", b"id", "metadata", b"metadata", "metrics", b"metrics", "model_predict_config", b"model_predict_config", "modified_at", b"modified_at", "processing_info", b"processing_info", "status", b"status", "user_id", b"user_id", "visibility", b"visibility"]) -> None: ...
     def WhichOneof(self, oneof_group: typing_extensions.Literal["data_config", b"data_config"]) -> typing_extensions.Literal["annotation_filter_config", "model_predict_config"] | None: ...
 
 global___DatasetVersion = DatasetVersion
 
 @typing_extensions.final
 class AnnotationFilterConfig(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
@@ -2719,14 +2749,61 @@
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["status", b"status"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["format", b"format", "include_embeddings", b"include_embeddings", "size", b"size", "status", b"status", "url", b"url"]) -> None: ...
 
 global___DatasetVersionExport = DatasetVersionExport
 
 @typing_extensions.final
+class DatasetVersionProcessingInfo(google.protobuf.message.Message):
+    """DatasetVersionProcessingInfo contains information about processing applied
+    to a dataset version.
+    """
+
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+    FRAME_INTERPOLATION_INFO_FIELD_NUMBER: builtins.int
+    @property
+    def frame_interpolation_info(self) -> global___FrameInterpolationInfo:
+        """If frame_interpolation_info is set, then these settings are used to
+        interpolate new frame annotation from other video annotations.
+        """
+    def __init__(
+        self,
+        *,
+        frame_interpolation_info: global___FrameInterpolationInfo | None = ...,
+    ) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["frame_interpolation_info", b"frame_interpolation_info"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["frame_interpolation_info", b"frame_interpolation_info"]) -> None: ...
+
+global___DatasetVersionProcessingInfo = DatasetVersionProcessingInfo
+
+@typing_extensions.final
+class FrameInterpolationInfo(google.protobuf.message.Message):
+    """FrameInterpolationInfo contains information about frame annotations
+    interpolated from other video annotations, such as image object-detection
+    regions generated from video object-tracking regions.
+    """
+
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+    SAMPLE_MS_FIELD_NUMBER: builtins.int
+    sample_ms: builtins.int
+    """sample_ms is the sampling rate at which frame annotations are interpolated.
+    If zero, then the input frame prediction sampling rate is used.
+    """
+    def __init__(
+        self,
+        *,
+        sample_ms: builtins.int = ...,
+    ) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["sample_ms", b"sample_ms"]) -> None: ...
+
+global___FrameInterpolationInfo = FrameInterpolationInfo
+
+@typing_extensions.final
 class WorkflowResultsSimilarity(google.protobuf.message.Message):
     """WorkflowResultsSimilarity"""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     PROBE_INPUT_FIELD_NUMBER: builtins.int
     POOL_RESULTS_FIELD_NUMBER: builtins.int
@@ -3218,34 +3295,28 @@
     the given Model. This message will be deprecated over time in favor or infer_params and
     train_params in OutputInfo which are cleaner and more extensible for many ModelTypes.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     CONCEPTS_MUTUALLY_EXCLUSIVE_FIELD_NUMBER: builtins.int
-    CLOSED_ENVIRONMENT_FIELD_NUMBER: builtins.int
     EXISTING_MODEL_ID_FIELD_NUMBER: builtins.int
     LANGUAGE_FIELD_NUMBER: builtins.int
     HYPER_PARAMETERS_FIELD_NUMBER: builtins.int
     MAX_CONCEPTS_FIELD_NUMBER: builtins.int
     MIN_VALUE_FIELD_NUMBER: builtins.int
     SELECT_CONCEPTS_FIELD_NUMBER: builtins.int
     TRAINING_TIMEOUT_FIELD_NUMBER: builtins.int
     SAMPLE_MS_FIELD_NUMBER: builtins.int
     HYPER_PARAMS_FIELD_NUMBER: builtins.int
     EMBED_MODEL_VERSION_ID_FIELD_NUMBER: builtins.int
     FAIL_ON_MISSING_POSITIVE_EXAMPLES_FIELD_NUMBER: builtins.int
     MODEL_METADATA_FIELD_NUMBER: builtins.int
     concepts_mutually_exclusive: builtins.bool
     """For custom concept model training: whether the concept predictions must sum to 1."""
-    closed_environment: builtins.bool
-    """For custom concept model training: Whether negatives should only be sampled from within the app during
-    training, for custom models.
-    Deprecated field. Use train_info.params.enrich_dataset for the model types that support it.
-    """
     existing_model_id: builtins.str
     """DEPRECATED: For custom models, this is the base model to use for image embeddings.
     Default is general model.
     """
     language: builtins.str
     """For concept model predictions: Overrides the default_language for the app in a predict call."""
     hyper_parameters: builtins.str
@@ -3289,30 +3360,29 @@
         details on what fields are supported for which models.
         TODO(zeiler): remove this field after Portal is updated.
         """
     def __init__(
         self,
         *,
         concepts_mutually_exclusive: builtins.bool = ...,
-        closed_environment: builtins.bool = ...,
         existing_model_id: builtins.str = ...,
         language: builtins.str = ...,
         hyper_parameters: builtins.str = ...,
         max_concepts: builtins.int = ...,
         min_value: builtins.float = ...,
         select_concepts: collections.abc.Iterable[global___Concept] | None = ...,
         training_timeout: builtins.int = ...,
         sample_ms: builtins.int = ...,
         hyper_params: google.protobuf.struct_pb2.Struct | None = ...,
         embed_model_version_id: builtins.str = ...,
         fail_on_missing_positive_examples: builtins.bool = ...,
         model_metadata: google.protobuf.struct_pb2.Struct | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["hyper_params", b"hyper_params", "model_metadata", b"model_metadata"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["closed_environment", b"closed_environment", "concepts_mutually_exclusive", b"concepts_mutually_exclusive", "embed_model_version_id", b"embed_model_version_id", "existing_model_id", b"existing_model_id", "fail_on_missing_positive_examples", b"fail_on_missing_positive_examples", "hyper_parameters", b"hyper_parameters", "hyper_params", b"hyper_params", "language", b"language", "max_concepts", b"max_concepts", "min_value", b"min_value", "model_metadata", b"model_metadata", "sample_ms", b"sample_ms", "select_concepts", b"select_concepts", "training_timeout", b"training_timeout"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["concepts_mutually_exclusive", b"concepts_mutually_exclusive", "embed_model_version_id", b"embed_model_version_id", "existing_model_id", b"existing_model_id", "fail_on_missing_positive_examples", b"fail_on_missing_positive_examples", "hyper_parameters", b"hyper_parameters", "hyper_params", b"hyper_params", "language", b"language", "max_concepts", b"max_concepts", "min_value", b"min_value", "model_metadata", b"model_metadata", "sample_ms", b"sample_ms", "select_concepts", b"select_concepts", "training_timeout", b"training_timeout"]) -> None: ...
 
 global___OutputConfig = OutputConfig
 
 @typing_extensions.final
 class ModelType(google.protobuf.message.Message):
     """ModelSpec is a definition of a Model type. This is used in model mode of portal
     to list out the possible models that can be created and can be used to understand more about
@@ -4378,28 +4448,43 @@
 @typing_extensions.final
 class EvalMetrics(google.protobuf.message.Message):
     """EvalMetrics"""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     STATUS_FIELD_NUMBER: builtins.int
+    USER_ID_FIELD_NUMBER: builtins.int
+    APP_ID_FIELD_NUMBER: builtins.int
     ID_FIELD_NUMBER: builtins.int
+    MODEL_FIELD_NUMBER: builtins.int
+    GROUND_TRUTH_DATASET_FIELD_NUMBER: builtins.int
     SUMMARY_FIELD_NUMBER: builtins.int
     CONFUSION_MATRIX_FIELD_NUMBER: builtins.int
     COOCCURRENCE_MATRIX_FIELD_NUMBER: builtins.int
     LABEL_COUNTS_FIELD_NUMBER: builtins.int
     BINARY_METRICS_FIELD_NUMBER: builtins.int
     TEST_SET_FIELD_NUMBER: builtins.int
     METRICS_BY_AREA_FIELD_NUMBER: builtins.int
     METRICS_BY_CLASS_FIELD_NUMBER: builtins.int
     TRACKER_METRICS_FIELD_NUMBER: builtins.int
     EVAL_INFO_FIELD_NUMBER: builtins.int
     @property
     def status(self) -> proto.clarifai.api.status.status_pb2.Status: ...
+    user_id: builtins.str
+    """user id that owns this evaluation"""
+    app_id: builtins.str
+    """app id that owns this evaluation"""
     id: builtins.str
+    """Id of this evaluation"""
+    @property
+    def model(self) -> global___Model:
+        """Model to evaluate"""
+    @property
+    def ground_truth_dataset(self) -> global___Dataset:
+        """The ground truth dataset"""
     @property
     def summary(self) -> global___MetricsSummary: ...
     @property
     def confusion_matrix(self) -> global___ConfusionMatrix: ...
     @property
     def cooccurrence_matrix(self) -> global___CooccurrenceMatrix: ...
     @property
@@ -4411,33 +4496,40 @@
     @property
     def metrics_by_area(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___BinaryMetrics]: ...
     @property
     def metrics_by_class(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___BinaryMetrics]: ...
     @property
     def tracker_metrics(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___TrackerMetrics]: ...
     @property
-    def eval_info(self) -> global___EvalInfo: ...
+    def eval_info(self) -> global___EvalInfo:
+        """Evaluation parameters to pass. Expected to match what
+        is defined in the model type for the respective model.
+        """
     def __init__(
         self,
         *,
         status: proto.clarifai.api.status.status_pb2.Status | None = ...,
+        user_id: builtins.str = ...,
+        app_id: builtins.str = ...,
         id: builtins.str = ...,
+        model: global___Model | None = ...,
+        ground_truth_dataset: global___Dataset | None = ...,
         summary: global___MetricsSummary | None = ...,
         confusion_matrix: global___ConfusionMatrix | None = ...,
         cooccurrence_matrix: global___CooccurrenceMatrix | None = ...,
         label_counts: global___LabelDistribution | None = ...,
         binary_metrics: collections.abc.Iterable[global___BinaryMetrics] | None = ...,
         test_set: collections.abc.Iterable[global___EvalTestSetEntry] | None = ...,
         metrics_by_area: collections.abc.Iterable[global___BinaryMetrics] | None = ...,
         metrics_by_class: collections.abc.Iterable[global___BinaryMetrics] | None = ...,
         tracker_metrics: collections.abc.Iterable[global___TrackerMetrics] | None = ...,
         eval_info: global___EvalInfo | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["confusion_matrix", b"confusion_matrix", "cooccurrence_matrix", b"cooccurrence_matrix", "eval_info", b"eval_info", "label_counts", b"label_counts", "status", b"status", "summary", b"summary"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["binary_metrics", b"binary_metrics", "confusion_matrix", b"confusion_matrix", "cooccurrence_matrix", b"cooccurrence_matrix", "eval_info", b"eval_info", "id", b"id", "label_counts", b"label_counts", "metrics_by_area", b"metrics_by_area", "metrics_by_class", b"metrics_by_class", "status", b"status", "summary", b"summary", "test_set", b"test_set", "tracker_metrics", b"tracker_metrics"]) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["confusion_matrix", b"confusion_matrix", "cooccurrence_matrix", b"cooccurrence_matrix", "eval_info", b"eval_info", "ground_truth_dataset", b"ground_truth_dataset", "label_counts", b"label_counts", "model", b"model", "status", b"status", "summary", b"summary"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["app_id", b"app_id", "binary_metrics", b"binary_metrics", "confusion_matrix", b"confusion_matrix", "cooccurrence_matrix", b"cooccurrence_matrix", "eval_info", b"eval_info", "ground_truth_dataset", b"ground_truth_dataset", "id", b"id", "label_counts", b"label_counts", "metrics_by_area", b"metrics_by_area", "metrics_by_class", b"metrics_by_class", "model", b"model", "status", b"status", "summary", b"summary", "test_set", b"test_set", "tracker_metrics", b"tracker_metrics", "user_id", b"user_id"]) -> None: ...
 
 global___EvalMetrics = EvalMetrics
 
 @typing_extensions.final
 class FieldsValue(google.protobuf.message.Message):
     """FieldsValue"""
 
@@ -7867,14 +7959,15 @@
     CALL_BACK_URL_FIELD_NUMBER: builtins.int
     APP_PAT_FIELD_NUMBER: builtins.int
     PROGRESS_FIELD_NUMBER: builtins.int
     CREATED_AT_FIELD_NUMBER: builtins.int
     MODIFIED_AT_FIELD_NUMBER: builtins.int
     EXTRACTION_JOBS_FIELD_NUMBER: builtins.int
     UPLOADS_FIELD_NUMBER: builtins.int
+    STATUS_FIELD_NUMBER: builtins.int
     id: builtins.str
     """id of the job"""
     call_back_url: builtins.str
     """If call back url is set, we will send a Post request to this endpoint with job status."""
     app_pat: builtins.str
     """Personal Access Token to the application to which inputs are added"""
     @property
@@ -7894,28 +7987,32 @@
         """
     @property
     def extraction_jobs(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___InputsExtractionJob]:
         """Sub-jobs that extract inputs from the cloud and/or archives"""
     @property
     def uploads(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___Upload]:
         """Archive uploads"""
+    @property
+    def status(self) -> proto.clarifai.api.status.status_pb2.Status:
+        """Status of the job"""
     def __init__(
         self,
         *,
         id: builtins.str = ...,
         call_back_url: builtins.str = ...,
         app_pat: builtins.str = ...,
         progress: global___InputsAddJobProgress | None = ...,
         created_at: google.protobuf.timestamp_pb2.Timestamp | None = ...,
         modified_at: google.protobuf.timestamp_pb2.Timestamp | None = ...,
         extraction_jobs: collections.abc.Iterable[global___InputsExtractionJob] | None = ...,
         uploads: collections.abc.Iterable[global___Upload] | None = ...,
+        status: proto.clarifai.api.status.status_pb2.Status | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["created_at", b"created_at", "modified_at", b"modified_at", "progress", b"progress"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["app_pat", b"app_pat", "call_back_url", b"call_back_url", "created_at", b"created_at", "extraction_jobs", b"extraction_jobs", "id", b"id", "modified_at", b"modified_at", "progress", b"progress", "uploads", b"uploads"]) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["created_at", b"created_at", "modified_at", b"modified_at", "progress", b"progress", "status", b"status"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["app_pat", b"app_pat", "call_back_url", b"call_back_url", "created_at", b"created_at", "extraction_jobs", b"extraction_jobs", "id", b"id", "modified_at", b"modified_at", "progress", b"progress", "status", b"status", "uploads", b"uploads"]) -> None: ...
 
 global___InputsAddJob = InputsAddJob
 
 @typing_extensions.final
 class InputsAddJobProgress(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -8051,14 +8148,15 @@
 
     STATUS_FIELD_NUMBER: builtins.int
     ID_FIELD_NUMBER: builtins.int
     URL_FIELD_NUMBER: builtins.int
     PROGRESS_FIELD_NUMBER: builtins.int
     CREATED_AT_FIELD_NUMBER: builtins.int
     MODIFIED_AT_FIELD_NUMBER: builtins.int
+    INPUT_ID_CONFLICT_RESOLUTION_FIELD_NUMBER: builtins.int
     @property
     def status(self) -> proto.clarifai.api.status.status_pb2.Status: ...
     id: builtins.str
     """ID of extraction job"""
     url: builtins.str
     """Url of archive or bucket"""
     @property
@@ -8072,90 +8170,94 @@
         """
     @property
     def modified_at(self) -> google.protobuf.timestamp_pb2.Timestamp:
         """Most recent time when the extraction job was updated.
         The format is https://www.ietf.org/rfc/rfc3339.txt.
         Example: "2006-01-02T15:04:05.999999Z".
         """
+    input_id_conflict_resolution: global___InputIDConflictResolution.ValueType
+    """How to handle input ID conflicts."""
     def __init__(
         self,
         *,
         status: proto.clarifai.api.status.status_pb2.Status | None = ...,
         id: builtins.str = ...,
         url: builtins.str = ...,
         progress: global___InputsExtractionJobProgress | None = ...,
         created_at: google.protobuf.timestamp_pb2.Timestamp | None = ...,
         modified_at: google.protobuf.timestamp_pb2.Timestamp | None = ...,
+        input_id_conflict_resolution: global___InputIDConflictResolution.ValueType = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["created_at", b"created_at", "modified_at", b"modified_at", "progress", b"progress", "status", b"status"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["created_at", b"created_at", "id", b"id", "modified_at", b"modified_at", "progress", b"progress", "status", b"status", "url", b"url"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["created_at", b"created_at", "id", b"id", "input_id_conflict_resolution", b"input_id_conflict_resolution", "modified_at", b"modified_at", "progress", b"progress", "status", b"status", "url", b"url"]) -> None: ...
 
 global___InputsExtractionJob = InputsExtractionJob
 
 @typing_extensions.final
 class InputsExtractionJobProgress(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    READ_OBJECTS_COUNT_FIELD_NUMBER: builtins.int
     AUDIO_INPUTS_COUNT_FIELD_NUMBER: builtins.int
     IMAGE_INPUTS_COUNT_FIELD_NUMBER: builtins.int
     VIDEO_INPUTS_COUNT_FIELD_NUMBER: builtins.int
     TEXT_INPUTS_COUNT_FIELD_NUMBER: builtins.int
     PENDING_ARCHIVES_COUNT_FIELD_NUMBER: builtins.int
     IN_PROGRESS_ARCHIVES_COUNT_FIELD_NUMBER: builtins.int
     COMPLETED_ARCHIVES_COUNT_FIELD_NUMBER: builtins.int
     FAILED_ARCHIVES_COUNT_FIELD_NUMBER: builtins.int
-    read_objects_count: builtins.int
     audio_inputs_count: builtins.int
     image_inputs_count: builtins.int
     video_inputs_count: builtins.int
     text_inputs_count: builtins.int
     pending_archives_count: builtins.int
     in_progress_archives_count: builtins.int
     completed_archives_count: builtins.int
     failed_archives_count: builtins.int
     def __init__(
         self,
         *,
-        read_objects_count: builtins.int = ...,
         audio_inputs_count: builtins.int = ...,
         image_inputs_count: builtins.int = ...,
         video_inputs_count: builtins.int = ...,
         text_inputs_count: builtins.int = ...,
         pending_archives_count: builtins.int = ...,
         in_progress_archives_count: builtins.int = ...,
         completed_archives_count: builtins.int = ...,
         failed_archives_count: builtins.int = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["audio_inputs_count", b"audio_inputs_count", "completed_archives_count", b"completed_archives_count", "failed_archives_count", b"failed_archives_count", "image_inputs_count", b"image_inputs_count", "in_progress_archives_count", b"in_progress_archives_count", "pending_archives_count", b"pending_archives_count", "read_objects_count", b"read_objects_count", "text_inputs_count", b"text_inputs_count", "video_inputs_count", b"video_inputs_count"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["audio_inputs_count", b"audio_inputs_count", "completed_archives_count", b"completed_archives_count", "failed_archives_count", b"failed_archives_count", "image_inputs_count", b"image_inputs_count", "in_progress_archives_count", b"in_progress_archives_count", "pending_archives_count", b"pending_archives_count", "text_inputs_count", b"text_inputs_count", "video_inputs_count", b"video_inputs_count"]) -> None: ...
 
 global___InputsExtractionJobProgress = InputsExtractionJobProgress
 
 @typing_extensions.final
 class InputsDataSource(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     INPUTS_ADD_JOB_ID_FIELD_NUMBER: builtins.int
     URL_FIELD_NUMBER: builtins.int
+    INPUT_ID_CONFLICT_RESOLUTION_FIELD_NUMBER: builtins.int
     inputs_add_job_id: builtins.str
     """Collect statistics about created inputs in job with given ID.
     On Post call:
     * If job ID is empty, then job is automatically created with random ID.
     * If job ID is non-empty, then a new job will be created with given ID.
     """
     @property
     def url(self) -> global___DataSourceURL: ...
+    input_id_conflict_resolution: global___InputIDConflictResolution.ValueType
+    """How to handle input ID conflicts."""
     def __init__(
         self,
         *,
         inputs_add_job_id: builtins.str = ...,
         url: global___DataSourceURL | None = ...,
+        input_id_conflict_resolution: global___InputIDConflictResolution.ValueType = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["url", b"url"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["inputs_add_job_id", b"inputs_add_job_id", "url", b"url"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["input_id_conflict_resolution", b"input_id_conflict_resolution", "inputs_add_job_id", b"inputs_add_job_id", "url", b"url"]) -> None: ...
 
 global___InputsDataSource = InputsDataSource
 
 @typing_extensions.final
 class DataSourceURL(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -8254,27 +8356,31 @@
 @typing_extensions.final
 class InputsUpload(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     INPUTS_ADD_JOB_ID_FIELD_NUMBER: builtins.int
     APP_PAT_FIELD_NUMBER: builtins.int
     UPLOAD_FIELD_NUMBER: builtins.int
+    INPUT_ID_CONFLICT_RESOLUTION_FIELD_NUMBER: builtins.int
     inputs_add_job_id: builtins.str
     """Collect statistics about created inputs in job with given ID.
     * If job ID is empty, then job is automatically created with random ID.
     * If job ID is non-empty, then a new job will be created with given ID.
     """
     app_pat: builtins.str
     """Personal Access Token to the application to which inputs are added"""
     @property
     def upload(self) -> global___Upload: ...
+    input_id_conflict_resolution: global___InputIDConflictResolution.ValueType
+    """How to handle input ID conflicts."""
     def __init__(
         self,
         *,
         inputs_add_job_id: builtins.str = ...,
         app_pat: builtins.str = ...,
         upload: global___Upload | None = ...,
+        input_id_conflict_resolution: global___InputIDConflictResolution.ValueType = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["upload", b"upload"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["app_pat", b"app_pat", "inputs_add_job_id", b"inputs_add_job_id", "upload", b"upload"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["app_pat", b"app_pat", "input_id_conflict_resolution", b"input_id_conflict_resolution", "inputs_add_job_id", b"inputs_add_job_id", "upload", b"upload"]) -> None: ...
 
 global___InputsUpload = InputsUpload
```

### Comparing `clarifai-grpc-9.5.0/clarifai_grpc/grpc/api/service_pb2.py` & `clarifai-grpc-9.6.0/clarifai_grpc/grpc/api/service_pb2.py`

 * *Files 9% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 from clarifai_grpc.grpc.api.status import status_code_pb2 as proto_dot_clarifai_dot_api_dot_status_dot_status__code__pb2
 from google.api import annotations_pb2 as google_dot_api_dot_annotations__pb2
 from google.protobuf import duration_pb2 as google_dot_protobuf_dot_duration__pb2
 from google.protobuf import struct_pb2 as google_dot_protobuf_dot_struct__pb2
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n proto/clarifai/api/service.proto\x12\x0c\x63larifai.api\x1a\"proto/clarifai/api/resources.proto\x1a&proto/clarifai/api/status/status.proto\x1a)proto/clarifai/api/utils/extensions.proto\x1a%proto/clarifai/auth/scope/scope.proto\x1a(proto/clarifai/auth/util/extension.proto\x1a+proto/clarifai/api/status/status_code.proto\x1a\x1cgoogle/api/annotations.proto\x1a\x1egoogle/protobuf/duration.proto\x1a\x1cgoogle/protobuf/struct.proto\x1a\x1fgoogle/protobuf/timestamp.proto\",\n\nPagination\x12\x0c\n\x04page\x18\x01 \x01(\r\x12\x10\n\x08per_page\x18\x02 \x01(\r\"p\n\x14GetAnnotationRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x15\n\rannotation_id\x18\x02 \x01(\t\x12\x10\n\x08input_id\x18\x03 \x01(\t\"\xb7\x02\n\x16ListAnnotationsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0b\n\x03ids\x18\x02 \x03(\t\x12\x11\n\tinput_ids\x18\x03 \x03(\t\x12\x10\n\x08user_ids\x18\t \x03(\t\x12\x19\n\x11model_version_ids\x18\n \x03(\t\x12-\n\x08statuses\x18\x05 \x03(\x0b\x32\x1b.clarifai.api.status.Status\x12\x1c\n\x14list_all_annotations\x18\x06 \x01(\x08\x12\x1b\n\x13return_model_output\x18\x0c \x01(\x08\x12\x0c\n\x04page\x18\x07 \x01(\r\x12\x10\n\x08per_page\x18\x08 \x01(\r\x12\x0f\n\x07task_id\x18\x0b \x01(\tJ\x04\x08\x04\x10\x05\"x\n\x16PostAnnotationsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12-\n\x0b\x61nnotations\x18\x02 \x03(\x0b\x32\x18.clarifai.api.Annotation\"\x89\x01\n\x17PatchAnnotationsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12-\n\x0b\x61nnotations\x18\x02 \x03(\x0b\x32\x18.clarifai.api.Annotation\x12\x0e\n\x06\x61\x63tion\x18\x03 \x01(\t\"\xb9\x01\n\x1dPatchAnnotationsStatusRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x34\n\x0bstatus_code\x18\x02 \x01(\x0e\x32\x1f.clarifai.api.status.StatusCode\x12\x10\n\x08user_ids\x18\x03 \x03(\t\x12\x0f\n\x07task_id\x18\x04 \x01(\t\x12\x0e\n\x06\x61\x63tion\x18\x05 \x01(\t\"v\n\x1ePatchAnnotationsStatusResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x10\n\x08user_ids\x18\x02 \x03(\t\x12\x15\n\rupdated_count\x18\x03 \x01(\r\"s\n\x17\x44\x65leteAnnotationRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x10\n\x08input_id\x18\x02 \x01(\t\x12\x15\n\rannotation_id\x18\x03 \x01(\t\"k\n\x18\x44\x65leteAnnotationsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0b\n\x03ids\x18\x02 \x03(\t\x12\x11\n\tinput_ids\x18\x03 \x03(\t\"u\n\x18SingleAnnotationResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12,\n\nannotation\x18\x02 \x01(\x0b\x32\x18.clarifai.api.Annotation\"{\n\x17MultiAnnotationResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x33\n\x0b\x61nnotations\x18\x02 \x03(\x0b\x32\x18.clarifai.api.AnnotationB\x04\x80\xb5\x18\x01\"[\n\rGetAppRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x19\n\x11\x61\x64\x64itional_fields\x18\x02 \x03(\t\"\xa5\x02\n\x0fListAppsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0c\n\x04page\x18\x02 \x01(\r\x12\x10\n\x08per_page\x18\x03 \x01(\r\x12\x16\n\x0esort_ascending\x18\x05 \x01(\x08\x12\x16\n\x0csort_by_name\x18\x06 \x01(\x08H\x00\x12\x1d\n\x13sort_by_modified_at\x18\x07 \x01(\x08H\x00\x12\r\n\x05query\x18\x08 \x01(\t\x12\x10\n\x04name\x18\x04 \x01(\tB\x02\x18\x01\x12\x15\n\rfeatured_only\x18\t \x01(\x08\x12\x14\n\x0cstarred_only\x18\x0b \x01(\x08\x12\x19\n\x11\x61\x64\x64itional_fields\x18\n \x03(\tB\t\n\x07sort_by\"c\n\x0fPostAppsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x1f\n\x04\x61pps\x18\x02 \x03(\x0b\x32\x11.clarifai.api.App\"C\n\x10\x44\x65leteAppRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\"\xb9\x01\n\x10PatchAppsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x1f\n\x04\x61pps\x18\x02 \x03(\x0b\x32\x11.clarifai.api.App\x12\x0e\n\x06\x61\x63tion\x18\x03 \x01(\t\x12\x32\n\x0fmetadata_action\x18\x04 \x01(\x0b\x32\x19.clarifai.api.PatchAction\x12\x0f\n\x07reindex\x18\x05 \x01(\x08\"\xb7\x01\n\x0fPatchAppRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x1e\n\x03\x61pp\x18\x02 \x01(\x0b\x32\x11.clarifai.api.App\x12\x0e\n\x06\x61\x63tion\x18\x03 \x01(\t\x12\x32\n\x0fmetadata_action\x18\x04 \x01(\x0b\x32\x19.clarifai.api.PatchAction\x12\x0f\n\x07reindex\x18\x05 \x01(\x08\"\x81\x01\n\x13PatchAppsIdsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12)\n\x03ids\x18\x03 \x03(\x0b\x32\x1c.clarifai.api.IdUpdateSource\x12\x0e\n\x06\x61\x63tion\x18\x04 \x01(\t\"\xa3\x01\n\x17PostAppsSearchesRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12)\n\tapp_query\x18\x02 \x01(\x0b\x32\x16.clarifai.api.AppQuery\x12,\n\npagination\x18\x03 \x01(\x0b\x32\x18.clarifai.api.Pagination\"`\n\x11SingleAppResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x1e\n\x03\x61pp\x18\x02 \x01(\x0b\x32\x11.clarifai.api.App\"f\n\x10MultiAppResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12%\n\x04\x61pps\x18\x02 \x03(\x0b\x32\x11.clarifai.api.AppB\x04\x80\xb5\x18\x01\"\x8b\x01\n\x18ListCollaboratorsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x1e\n\x16list_all_collaborators\x18\x02 \x01(\x08\x12\x0c\n\x04page\x18\x03 \x01(\r\x12\x10\n\x08per_page\x18\x04 \x01(\r\"~\n\x18PostCollaboratorsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x31\n\rcollaborators\x18\x02 \x03(\x0b\x32\x1a.clarifai.api.Collaborator\"\x8f\x01\n\x19PatchCollaboratorsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x31\n\rcollaborators\x18\x02 \x03(\x0b\x32\x1a.clarifai.api.Collaborator\x12\x0e\n\x06\x61\x63tion\x18\x03 \x01(\t\"|\n\x1a\x44\x65leteCollaboratorsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x18\n\x10\x63ollaborator_ids\x18\x02 \x03(\t\x12\x13\n\x0buser_emails\x18\x03 \x03(\t\"\x82\x01\n\x1aMultiCollaboratorsResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x37\n\rcollaborators\x18\x02 \x03(\x0b\x32\x1a.clarifai.api.CollaboratorB\x04\x80\xb5\x18\x01\"l\n\x19ListCollaborationsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0c\n\x04page\x18\x02 \x01(\r\x12\x10\n\x08per_page\x18\x03 \x01(\r\"\x85\x01\n\x1bMultiCollaborationsResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x39\n\x0e\x63ollaborations\x18\x02 \x03(\x0b\x32\x1b.clarifai.api.CollaborationB\x04\x80\xb5\x18\x01\".\n\x14GetStatusCodeRequest\x12\x16\n\x0estatus_code_id\x18\x01 \x01(\t\"\x18\n\x16ListStatusCodesRequest\"G\n\x18SingleStatusCodeResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\"u\n\x17MultiStatusCodeResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12-\n\x08statuses\x18\x02 \x03(\x0b\x32\x1b.clarifai.api.status.Status\"X\n\x11GetConceptRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x12\n\nconcept_id\x18\x02 \x01(\t\"f\n\x13ListConceptsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0c\n\x04page\x18\x02 \x01(\r\x12\x10\n\x08per_page\x18\x03 \x01(\r\"\x91\x01\n\x18ListModelConceptsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x10\n\x08model_id\x18\x02 \x01(\t\x12\x12\n\nversion_id\x18\x03 \x01(\t\x12\x0c\n\x04page\x18\x04 \x01(\r\x12\x10\n\x08per_page\x18\x05 \x01(\r\"\xaf\x01\n\x1bPostConceptsSearchesRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x31\n\rconcept_query\x18\x02 \x01(\x0b\x32\x1a.clarifai.api.ConceptQuery\x12,\n\npagination\x18\x03 \x01(\x0b\x32\x18.clarifai.api.Pagination\"o\n\x13PostConceptsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\'\n\x08\x63oncepts\x18\x02 \x03(\x0b\x32\x15.clarifai.api.Concept\"\x80\x01\n\x14PatchConceptsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\'\n\x08\x63oncepts\x18\x02 \x03(\x0b\x32\x15.clarifai.api.Concept\x12\x0e\n\x06\x61\x63tion\x18\x03 \x01(\t\"j\n\x17GetConceptCountsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0c\n\x04page\x18\x02 \x01(\r\x12\x10\n\x08per_page\x18\x03 \x01(\r\"l\n\x15SingleConceptResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12&\n\x07\x63oncept\x18\x02 \x01(\x0b\x32\x15.clarifai.api.Concept\"r\n\x14MultiConceptResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12-\n\x08\x63oncepts\x18\x02 \x03(\x0b\x32\x15.clarifai.api.ConceptB\x04\x80\xb5\x18\x01\"\x82\x01\n\x19MultiConceptCountResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x38\n\x0e\x63oncept_counts\x18\x02 \x03(\x0b\x32\x1a.clarifai.api.ConceptCountB\x04\x80\xb5\x18\x01\"\xb1\x01\n\x1bListConceptRelationsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x12\n\nconcept_id\x18\x02 \x01(\t\x12\x11\n\tpredicate\x18\x03 \x01(\t\x12\x1a\n\x12knowledge_graph_id\x18\x04 \x01(\t\x12\x0c\n\x04page\x18\x05 \x01(\r\x12\x10\n\x08per_page\x18\x06 \x01(\r\"\x9c\x01\n\x1bPostConceptRelationsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x12\n\nconcept_id\x18\x02 \x01(\t\x12\x38\n\x11\x63oncept_relations\x18\x03 \x03(\x0b\x32\x1d.clarifai.api.ConceptRelation\"q\n\x1d\x44\x65leteConceptRelationsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x12\n\nconcept_id\x18\x02 \x01(\t\x12\x0b\n\x03ids\x18\x03 \x03(\t\"M\n\x1aListKnowledgeGraphsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\"\x85\x01\n\x1aPostKnowledgeGraphsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x36\n\x10knowledge_graphs\x18\x02 \x03(\x0b\x32\x1c.clarifai.api.KnowledgeGraph\"\x8f\x01\n\x1dPostConceptMappingJobsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12=\n\x14\x63oncept_mapping_jobs\x18\x02 \x03(\x0b\x32\x1f.clarifai.api.ConceptMappingJob\"\x8b\x01\n\x1cMultiConceptRelationResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12>\n\x11\x63oncept_relations\x18\x02 \x03(\x0b\x32\x1d.clarifai.api.ConceptRelationB\x04\x80\xb5\x18\x01\"\x88\x01\n\x1bMultiKnowledgeGraphResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12<\n\x10knowledge_graphs\x18\x02 \x03(\x0b\x32\x1c.clarifai.api.KnowledgeGraphB\x04\x80\xb5\x18\x01\"Z\n\x1eMultiConceptMappingJobResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x0b\n\x03ids\x18\x02 \x03(\t\"r\n\x19GetConceptLanguageRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x12\n\nconcept_id\x18\x02 \x01(\t\x12\x10\n\x08language\x18\x03 \x01(\t\"\x82\x01\n\x1bListConceptLanguagesRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x12\n\nconcept_id\x18\x02 \x01(\t\x12\x0c\n\x04page\x18\x03 \x01(\r\x12\x10\n\x08per_page\x18\x04 \x01(\r\"\xad\x01\n\x1cPatchConceptLanguagesRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x12\n\nconcept_id\x18\x02 \x01(\t\x12\x38\n\x11\x63oncept_languages\x18\x03 \x03(\x0b\x32\x1d.clarifai.api.ConceptLanguage\x12\x0e\n\x06\x61\x63tion\x18\x04 \x01(\t\"\x9c\x01\n\x1bPostConceptLanguagesRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x12\n\nconcept_id\x18\x02 \x01(\t\x12\x38\n\x11\x63oncept_languages\x18\x03 \x03(\x0b\x32\x1d.clarifai.api.ConceptLanguage\"\x85\x01\n\x1dSingleConceptLanguageResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x37\n\x10\x63oncept_language\x18\x02 \x01(\x0b\x32\x1d.clarifai.api.ConceptLanguage\"\x8b\x01\n\x1cMultiConceptLanguageResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12>\n\x11\x63oncept_languages\x18\x02 \x03(\x0b\x32\x1d.clarifai.api.ConceptLanguageB\x04\x80\xb5\x18\x01\"T\n\x0fGetInputRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x10\n\x08input_id\x18\x02 \x01(\t\"\\\n\x17GetVideoManifestRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x10\n\x08input_id\x18\x02 \x01(\t\"l\n\x16GetInputSamplesRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0f\n\x07task_id\x18\x02 \x01(\t\x12\x10\n\x08user_ids\x18\x03 \x03(\t\"\x9e\x01\n\x11ListInputsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0c\n\x04page\x18\x02 \x01(\r\x12\x10\n\x08per_page\x18\x03 \x01(\r\x12+\n\x06status\x18\x05 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x0b\n\x03ids\x18\x04 \x03(\t\"\x92\x01\n\x13StreamInputsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x10\n\x08per_page\x18\x02 \x01(\r\x12\x0f\n\x07last_id\x18\x03 \x01(\t\x12\x13\n\x0border_by_id\x18\x05 \x01(\x08\x12\x12\n\ndescending\x18\x04 \x01(\x08\"\x84\x01\n\x11PostInputsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12#\n\x06inputs\x18\x02 \x03(\x0b\x32\x13.clarifai.api.Input\x12\x19\n\x11inputs_add_job_id\x18\x03 \x01(\t\"z\n\x12PatchInputsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12#\n\x06inputs\x18\x02 \x03(\x0b\x32\x13.clarifai.api.Input\x12\x0e\n\x06\x61\x63tion\x18\x03 \x01(\t\"W\n\x12\x44\x65leteInputRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x10\n\x08input_id\x18\x02 \x01(\t\"Y\n\x13\x44\x65leteInputsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0b\n\x03ids\x18\x02 \x03(\tJ\x04\x08\x03\x10\x04\"f\n\x13SingleInputResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\"\n\x05input\x18\x02 \x01(\x0b\x32\x13.clarifai.api.Input\"]\n\x18GetVideoManifestResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x14\n\x0cmanifest_url\x18\x02 \x01(\t\"\xa0\x01\n\x12MultiInputResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12)\n\x06inputs\x18\x02 \x03(\x0b\x32\x13.clarifai.api.InputB\x04\x80\xb5\x18\x01\x12\x32\n\x0einputs_add_job\x18\x03 \x01(\x0b\x32\x1a.clarifai.api.InputsAddJob\"r\n\x1cMultiInputAnnotationResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12%\n\x04hits\x18\x03 \x03(\x0b\x32\x11.clarifai.api.HitB\x04\x80\xb5\x18\x01\"q\n\x18SingleInputCountResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12(\n\x06\x63ounts\x18\x02 \x01(\x0b\x32\x18.clarifai.api.InputCount\"G\n\x14GetInputCountRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\"\x97\x01\n\x13ListDatasetsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0c\n\x04page\x18\x02 \x01(\r\x12\x10\n\x08per_page\x18\x03 \x01(\r\x12\x14\n\x0cstarred_only\x18\x04 \x01(\x08\x12\x19\n\x11\x61\x64\x64itional_fields\x18\x05 \x03(\t\"s\n\x11GetDatasetRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x12\n\ndataset_id\x18\x02 \x01(\t\x12\x19\n\x11\x61\x64\x64itional_fields\x18\x03 \x03(\t\"o\n\x13PostDatasetsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\'\n\x08\x64\x61tasets\x18\x02 \x03(\x0b\x32\x15.clarifai.api.Dataset\"\x80\x01\n\x14PatchDatasetsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\'\n\x08\x64\x61tasets\x18\x02 \x03(\x0b\x32\x15.clarifai.api.Dataset\x12\x0e\n\x06\x61\x63tion\x18\x03 \x01(\t\"\x84\x01\n\x16PatchDatasetIdsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12)\n\x03ids\x18\x03 \x03(\x0b\x32\x1c.clarifai.api.IdUpdateSource\x12\x0e\n\x06\x61\x63tion\x18\x04 \x01(\t\"]\n\x15\x44\x65leteDatasetsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x13\n\x0b\x64\x61taset_ids\x18\x02 \x03(\t\"r\n\x14MultiDatasetResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12-\n\x08\x64\x61tasets\x18\x02 \x03(\x0b\x32\x15.clarifai.api.DatasetB\x04\x80\xb5\x18\x01\"l\n\x15SingleDatasetResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12&\n\x07\x64\x61taset\x18\x02 \x01(\x0b\x32\x15.clarifai.api.Dataset\"\x7f\n\x18ListDatasetInputsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x12\n\ndataset_id\x18\x02 \x01(\t\x12\x0c\n\x04page\x18\x03 \x01(\r\x12\x10\n\x08per_page\x18\x04 \x01(\r\"o\n\x16GetDatasetInputRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x12\n\ndataset_id\x18\x02 \x01(\t\x12\x10\n\x08input_id\x18\x03 \x01(\t\"\xb9\x01\n\x18PostDatasetInputsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x12\n\ndataset_id\x18\x02 \x01(\t\x12\x32\n\x0e\x64\x61taset_inputs\x18\x03 \x03(\x0b\x32\x1a.clarifai.api.DatasetInput\x12$\n\x06search\x18\x04 \x01(\x0b\x32\x14.clarifai.api.Search\"t\n\x1a\x44\x65leteDatasetInputsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x12\n\ndataset_id\x18\x02 \x01(\t\x12\x11\n\tinput_ids\x18\x03 \x03(\t\"\xd2\x01\n\x19MultiDatasetInputResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x38\n\x0e\x64\x61taset_inputs\x18\x02 \x03(\x0b\x32\x1a.clarifai.api.DatasetInputB\x04\x80\xb5\x18\x01\x12N\n\x1d\x64\x61taset_inputs_search_add_job\x18\x03 \x01(\x0b\x32\'.clarifai.api.DatasetInputsSearchAddJob\"|\n\x1aSingleDatasetInputResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x31\n\rdataset_input\x18\x02 \x01(\x0b\x32\x1a.clarifai.api.DatasetInput\"\x81\x01\n\x1aListDatasetVersionsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x12\n\ndataset_id\x18\x02 \x01(\t\x12\x0c\n\x04page\x18\x03 \x01(\r\x12\x10\n\x08per_page\x18\x04 \x01(\r\"{\n\x18GetDatasetVersionRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x12\n\ndataset_id\x18\x02 \x01(\t\x12\x1a\n\x12\x64\x61taset_version_id\x18\x03 \x01(\t\"\xa4\x02\n&ListDatasetVersionMetricsGroupsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x12\n\ndataset_id\x18\x02 \x01(\t\x12\x1a\n\x12\x64\x61taset_version_id\x18\x03 \x01(\t\x12\x0c\n\x04page\x18\x04 \x01(\r\x12\x10\n\x08per_page\x18\x05 \x01(\r\x12\x14\n\x0cparent_paths\x18\x06 \x03(\t\x12;\n\x05types\x18\x07 \x03(\x0e\x32,.clarifai.api.DatasetVersionMetricsGroupType\x12&\n\x06values\x18\x08 \x03(\x0b\x32\x16.google.protobuf.Value\"\x99\x01\n\x1aPostDatasetVersionsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x12\n\ndataset_id\x18\x02 \x01(\t\x12\x36\n\x10\x64\x61taset_versions\x18\x03 \x03(\x0b\x32\x1c.clarifai.api.DatasetVersion\"\xaa\x01\n\x1bPatchDatasetVersionsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x12\n\ndataset_id\x18\x02 \x01(\t\x12\x36\n\x10\x64\x61taset_versions\x18\x03 \x03(\x0b\x32\x1c.clarifai.api.DatasetVersion\x12\x0e\n\x06\x61\x63tion\x18\x04 \x01(\t\"\x80\x01\n\x1c\x44\x65leteDatasetVersionsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x12\n\ndataset_id\x18\x02 \x01(\t\x12\x1b\n\x13\x64\x61taset_version_ids\x18\x03 \x03(\t\"\xb7\x01\n\x1fPutDatasetVersionExportsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x12\n\ndataset_id\x18\x02 \x01(\t\x12\x1a\n\x12\x64\x61taset_version_id\x18\x03 \x01(\t\x12\x33\n\x07\x65xports\x18\x04 \x03(\x0b\x32\".clarifai.api.DatasetVersionExport\"\x88\x01\n\x1bMultiDatasetVersionResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12<\n\x10\x64\x61taset_versions\x18\x02 \x03(\x0b\x32\x1c.clarifai.api.DatasetVersionB\x04\x80\xb5\x18\x01\"\x8b\x01\n!MultiDatasetVersionExportResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x39\n\x07\x65xports\x18\x02 \x03(\x0b\x32\".clarifai.api.DatasetVersionExportB\x04\x80\xb5\x18\x01\"\xae\x01\n\'MultiDatasetVersionMetricsGroupResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12V\n\x1e\x64\x61taset_version_metrics_groups\x18\x02 \x03(\x0b\x32(.clarifai.api.DatasetVersionMetricsGroupB\x04\x80\xb5\x18\x01\"\x82\x01\n\x1cSingleDatasetVersionResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x35\n\x0f\x64\x61taset_version\x18\x02 \x01(\x0b\x32\x1c.clarifai.api.DatasetVersion\"f\n#GetDatasetInputsSearchAddJobRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0e\n\x06job_id\x18\x02 \x01(\t\"\x8c\x01\n\'SingleDatasetInputsSearchAddJobResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x34\n\x03job\x18\x02 \x01(\x0b\x32\'.clarifai.api.DatasetInputsSearchAddJob\"\xb9\x01\n\x17PostModelOutputsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x10\n\x08model_id\x18\x02 \x01(\t\x12\x12\n\nversion_id\x18\x03 \x01(\t\x12#\n\x06inputs\x18\x04 \x03(\x0b\x32\x13.clarifai.api.Input\x12\"\n\x05model\x18\x05 \x01(\x0b\x32\x13.clarifai.api.Model\"\x8f\x01\n\x16ListModelInputsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x10\n\x08model_id\x18\x02 \x01(\t\x12\x12\n\nversion_id\x18\x03 \x01(\t\x12\x0c\n\x04page\x18\x04 \x01(\r\x12\x10\n\x08per_page\x18\x05 \x01(\r\"P\n\rGetKeyRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0e\n\x06key_id\x18\x02 \x01(\t\"\x9a\x01\n\x0fListKeysRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0c\n\x04page\x18\x02 \x01(\r\x12\x10\n\x08per_page\x18\x03 \x01(\r\x12\x13\n\x0bnot_expired\x18\x04 \x01(\x08\x12\x0e\n\x06scopes\x18\x05 \x03(\t\x12\x11\n\tendpoints\x18\x06 \x03(\t\"e\n\x12ListAppKeysRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0c\n\x04page\x18\x02 \x01(\r\x12\x10\n\x08per_page\x18\x03 \x01(\r\"c\n\x0fPostKeysRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x1f\n\x04keys\x18\x02 \x03(\x0b\x32\x11.clarifai.api.Key\"S\n\x10\x44\x65leteKeyRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0e\n\x06key_id\x18\x02 \x01(\t\"t\n\x10PatchKeysRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x1f\n\x04keys\x18\x02 \x03(\x0b\x32\x11.clarifai.api.Key\x12\x0e\n\x06\x61\x63tion\x18\x03 \x01(\t\"`\n\x11SingleKeyResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x1e\n\x03key\x18\x02 \x01(\x0b\x32\x11.clarifai.api.Key\"f\n\x10MultiKeyResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12%\n\x04keys\x18\x02 \x03(\x0b\x32\x11.clarifai.api.KeyB\x04\x80\xb5\x18\x01\"\xad\x01\n\x0fGetModelRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x10\n\x08model_id\x18\x02 \x01(\t\x12\x12\n\nversion_id\x18\x03 \x01(\t\x12\x10\n\x08language\x18\x04 \x01(\t\x12\x16\n\x0etrained_before\x18\x05 \x01(\x08\x12\x19\n\x11\x61\x64\x64itional_fields\x18\x13 \x03(\t\"\xa3\x04\n\x11ListModelsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0c\n\x04page\x18\x02 \x01(\r\x12\x10\n\x08per_page\x18\x03 \x01(\r\x12\x16\n\x0esort_ascending\x18\n \x01(\x08\x12\x16\n\x0csort_by_name\x18\x0b \x01(\x08H\x00\x12\x1c\n\x12sort_by_num_inputs\x18\x0c \x01(\x08H\x00\x12\x1d\n\x13sort_by_modified_at\x18\r \x01(\x08H\x00\x12\r\n\x05query\x18\x0e \x01(\t\x12\x0c\n\x04name\x18\x05 \x01(\t\x12\x19\n\x11\x66ilter_by_user_id\x18\x16 \x01(\x08\x12\x15\n\rmodel_type_id\x18\x06 \x01(\t\x12\x14\n\x0ctrained_only\x18\x07 \x01(\x08\x12\x14\n\x0cinput_fields\x18\x08 \x03(\t\x12\x15\n\routput_fields\x18\t \x03(\t\x12\x0f\n\x07license\x18\x0f \x01(\t\x12\x15\n\rfeatured_only\x18\x10 \x01(\x08\x12\x14\n\x0cstarred_only\x18\x14 \x01(\x08\x12\x10\n\x08toolkits\x18\x11 \x03(\t\x12\x11\n\tuse_cases\x18\x12 \x03(\t\x12\x11\n\tlanguages\x18\x15 \x03(\t\x12\x19\n\x11\x61\x64\x64itional_fields\x18\x13 \x03(\t\x12\x1c\n\x14\x64ont_fetch_from_main\x18\x17 \x01(\x08\x42\t\n\x07sort_byJ\x04\x08\x04\x10\x05\"\x80\x01\n\x19PatchModelToolkitsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x10\n\x08model_id\x18\x02 \x01(\t\x12\x10\n\x08toolkits\x18\x03 \x03(\t\x12\x0e\n\x06\x61\x63tion\x18\x04 \x01(\t\"\x8b\x01\n\x1ePatchModelCheckConsentsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x10\n\x08model_id\x18\x02 \x01(\t\x12\x16\n\x0e\x63heck_consents\x18\x03 \x03(\t\x12\x0e\n\x06\x61\x63tion\x18\x04 \x01(\t\"\x80\x01\n\x19PatchModelUseCasesRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x10\n\x08model_id\x18\x02 \x01(\t\x12\x10\n\x08usecases\x18\x03 \x03(\t\x12\x0e\n\x06\x61\x63tion\x18\x04 \x01(\t\"\x82\x01\n\x1aPatchModelLanguagesRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x10\n\x08model_id\x18\x02 \x01(\t\x12\x11\n\tlanguages\x18\x03 \x03(\t\x12\x0e\n\x06\x61\x63tion\x18\x04 \x01(\t\"Z\n\x19MultiModelToolkitResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x10\n\x08toolkits\x18\x02 \x03(\t\"e\n\x1eMultiModelCheckConsentResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x16\n\x0e\x63heck_consents\x18\x02 \x03(\t\"Z\n\x19MultiModelUseCaseResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x10\n\x08usecases\x18\x02 \x03(\t\"\\\n\x1aMultiModelLanguageResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x11\n\tlanguages\x18\x02 \x03(\t\"\x91\x01\n\x11PostModelsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12&\n\x05model\x18\x02 \x01(\x0b\x32\x13.clarifai.api.ModelB\x02\x18\x01\x12#\n\x06models\x18\x03 \x03(\x0b\x32\x13.clarifai.api.Model\"z\n\x12PatchModelsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12#\n\x06models\x18\x02 \x03(\x0b\x32\x13.clarifai.api.Model\x12\x0e\n\x06\x61\x63tion\x18\x03 \x01(\t\",\n\x0eIdUpdateSource\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0e\n\x06new_id\x18\x02 \x01(\t\"\x82\x01\n\x14PatchModelIdsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12)\n\x03ids\x18\x03 \x03(\x0b\x32\x1c.clarifai.api.IdUpdateSource\x12\x0e\n\x06\x61\x63tion\x18\x04 \x01(\t\"W\n\x12\x44\x65leteModelRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x10\n\x08model_id\x18\x02 \x01(\t\"g\n\x13\x44\x65leteModelsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0b\n\x03ids\x18\x02 \x03(\t\x12\x12\n\ndelete_all\x18\x03 \x01(\x08\"\xa9\x01\n\x19PostModelsSearchesRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12-\n\x0bmodel_query\x18\x02 \x01(\x0b\x32\x18.clarifai.api.ModelQuery\x12,\n\npagination\x18\x03 \x01(\x0b\x32\x18.clarifai.api.Pagination\"f\n\x13SingleModelResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\"\n\x05model\x18\x02 \x01(\x0b\x32\x13.clarifai.api.Model\"l\n\x12MultiModelResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12)\n\x06models\x18\x02 \x03(\x0b\x32\x13.clarifai.api.ModelB\x04\x80\xb5\x18\x01\"\xa2\x01\n\x19PatchModelVersionsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x10\n\x08model_id\x18\x02 \x01(\t\x12\x32\n\x0emodel_versions\x18\x03 \x03(\x0b\x32\x1a.clarifai.api.ModelVersion\x12\x0e\n\x06\x61\x63tion\x18\x04 \x01(\t\"o\n\x16GetModelVersionRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x10\n\x08model_id\x18\x02 \x01(\t\x12\x12\n\nversion_id\x18\x03 \x01(\t\"\xc5\x02\n\x18ListModelVersionsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x10\n\x08model_id\x18\x02 \x01(\t\x12\x0c\n\x04page\x18\x03 \x01(\r\x12\x10\n\x08per_page\x18\x04 \x01(\r\x12\x13\n\x0b\x63oncept_ids\x18\x05 \x03(\t\x12\x14\n\x0ctrained_only\x18\x06 \x01(\x08\x12\x16\n\x0esort_ascending\x18\x07 \x01(\x08\x12\x1d\n\x13sort_by_status_code\x18\x08 \x01(\x08H\x00\x12\x1c\n\x12sort_by_num_inputs\x18\t \x01(\x08H\x00\x12\x1d\n\x13sort_by_description\x18\n \x01(\x08H\x00\x12\x1c\n\x12sort_by_created_at\x18\x0b \x01(\x08H\x00\x42\t\n\x07sort_by\"r\n\x19\x44\x65leteModelVersionRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x10\n\x08model_id\x18\x03 \x01(\t\x12\x12\n\nversion_id\x18\x04 \x01(\t\"|\n\x1aSingleModelVersionResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x31\n\rmodel_version\x18\x02 \x01(\x0b\x32\x1a.clarifai.api.ModelVersion\"\x82\x01\n\x19MultiModelVersionResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x38\n\x0emodel_versions\x18\x02 \x03(\x0b\x32\x1a.clarifai.api.ModelVersionB\x04\x80\xb5\x18\x01\"\xef\x01\n\x18PostModelVersionsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x10\n\x08model_id\x18\x02 \x01(\t\x12\x32\n\x0emodel_versions\x18\x03 \x03(\x0b\x32\x1a.clarifai.api.ModelVersion\x12\x13\n\x0b\x64\x65scription\x18\x08 \x01(\t\x12)\n\teval_info\x18\n \x01(\x0b\x32\x16.clarifai.api.EvalInfoJ\x04\x08\x04\x10\x05J\x04\x08\x05\x10\x06J\x04\x08\x06\x10\x07J\x04\x08\x07\x10\x08J\x04\x08\t\x10\n\"\xb1\x01\n$PostWorkflowVersionsUnPublishRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x13\n\x0bworkflow_id\x18\x02 \x01(\t\x12\x43\n\x0cpublications\x18\x03 \x03(\x0b\x32-.clarifai.api.WorkflowVersionUnPublishRequest\"\xad\x01\n\"PostWorkflowVersionsPublishRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x13\n\x0bworkflow_id\x18\x02 \x01(\t\x12\x41\n\x0cpublications\x18\x03 \x03(\x0b\x32+.clarifai.api.WorkflowVersionPublishRequest\"3\n\x1dWorkflowVersionPublishRequest\x12\x12\n\nversion_id\x18\x01 \x01(\t\"5\n\x1fWorkflowVersionUnPublishRequest\x12\x12\n\nversion_id\x18\x01 \x01(\t\"0\n\x1aModelVersionPublishRequest\x12\x12\n\nversion_id\x18\x01 \x01(\t\"\xa4\x01\n\x1fPostModelVersionsPublishRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x10\n\x08model_id\x18\x02 \x01(\t\x12>\n\x0cpublications\x18\x03 \x03(\x0b\x32(.clarifai.api.ModelVersionPublishRequest\"2\n\x1cModelVersionUnpublishRequest\x12\x12\n\nversion_id\x18\x01 \x01(\t\"\xa8\x01\n!PostModelVersionsUnPublishRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x10\n\x08model_id\x18\x02 \x01(\t\x12@\n\x0cpublications\x18\x03 \x03(\x0b\x32*.clarifai.api.ModelVersionUnpublishRequest\"\xb2\x01\n\"PostModelVersionEvaluationsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x10\n\x08model_id\x18\x02 \x01(\t\x12\x18\n\x10model_version_id\x18\x03 \x01(\t\x12/\n\x0c\x65val_metrics\x18\x04 \x03(\x0b\x32\x19.clarifai.api.EvalMetrics\"\xa1\x01\n\"ListModelVersionEvaluationsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x10\n\x08model_id\x18\x02 \x01(\t\x12\x18\n\x10model_version_id\x18\x03 \x01(\t\x12\x0c\n\x04page\x18\x04 \x01(\r\x12\x10\n\x08per_page\x18\x05 \x01(\r\"\xc1\x01\n GetModelVersionEvaluationRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x10\n\x08model_id\x18\x02 \x01(\t\x12\x18\n\x10model_version_id\x18\x03 \x01(\t\x12\x15\n\revaluation_id\x18\x04 \x01(\t\x12)\n\x06\x66ields\x18\x05 \x01(\x0b\x32\x19.clarifai.api.FieldsValue\"y\n\x19SingleEvalMetricsResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12/\n\x0c\x65val_metrics\x18\x02 \x01(\x0b\x32\x19.clarifai.api.EvalMetrics\"x\n\x18MultiEvalMetricsResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12/\n\x0c\x65val_metrics\x18\x02 \x03(\x0b\x32\x19.clarifai.api.EvalMetrics\"\xd3\x01\n\x1ePostModelVersionMetricsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x10\n\x08model_id\x18\x02 \x01(\t\x12\x12\n\nversion_id\x18\x03 \x01(\t\x12)\n\x0btest_search\x18\x05 \x01(\x0b\x32\x14.clarifai.api.Search\x12)\n\teval_info\x18\n \x01(\x0b\x32\x16.clarifai.api.EvalInfoJ\x04\x08\x04\x10\x05\"\xa1\x01\n\x1dGetModelVersionMetricsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x10\n\x08model_id\x18\x02 \x01(\t\x12\x12\n\nversion_id\x18\x03 \x01(\t\x12)\n\x06\x66ields\x18\x04 \x01(\x0b\x32\x19.clarifai.api.FieldsValue\"]\n\x13GetModelTypeRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x15\n\rmodel_type_id\x18\x02 \x01(\t\"h\n\x15ListModelTypesRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0c\n\x04page\x18\x02 \x01(\r\x12\x10\n\x08per_page\x18\x03 \x01(\r\"\x1f\n\x1dListOpenSourceLicensesRequest\"_\n\x1eListOpenSourceLicensesResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x10\n\x08licenses\x18\x02 \x03(\t\"y\n\x17SingleModelTypeResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x31\n\nmodel_type\x18\x02 \x01(\x0b\x32\x17.clarifai.api.ModelTypeB\x04\x80\xb5\x18\x01\"\xf2\x01\n\x16MultiModelTypeResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x32\n\x0bmodel_types\x18\x02 \x03(\x0b\x32\x17.clarifai.api.ModelTypeB\x04\x80\xb5\x18\x01\x12\x35\n\x0fmodel_importers\x18\x03 \x01(\x0b\x32\x1c.clarifai.api.ModelTypeField\x12@\n\x16triton_conda_envs_info\x18\x04 \x03(\x0b\x32 .clarifai.api.TritonCondaEnvInfo\"\x95\x01\n\"GetModelVersionInputExampleRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x10\n\x08model_id\x18\x02 \x01(\t\x12\x18\n\x10model_version_id\x18\x03 \x01(\t\x12\x12\n\nexample_id\x18\x04 \x01(\t\"\xa3\x01\n$ListModelVersionInputExamplesRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x10\n\x08model_id\x18\x02 \x01(\t\x12\x18\n\x10model_version_id\x18\x03 \x01(\t\x12\x0c\n\x04page\x18\x04 \x01(\r\x12\x10\n\x08per_page\x18\x05 \x01(\r\"\xa2\x01\n&SingleModelVersionInputExampleResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12K\n\x1bmodel_version_input_example\x18\x02 \x01(\x0b\x32&.clarifai.api.ModelVersionInputExample\"\xa2\x01\n%MultiModelVersionInputExampleResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12L\n\x1cmodel_version_input_examples\x18\x02 \x03(\x0b\x32&.clarifai.api.ModelVersionInputExample\"\x7f\n\x1aListModelReferencesRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x10\n\x08model_id\x18\x02 \x01(\t\x12\x0c\n\x04page\x18\x03 \x01(\r\x12\x10\n\x08per_page\x18\x04 \x01(\r\"\x82\x01\n\x1bMultiModelReferenceResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x36\n\x10model_references\x18\x02 \x03(\x0b\x32\x1c.clarifai.api.ModelReference\"o\n\x13MultiOutputResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12+\n\x07outputs\x18\x02 \x03(\x0b\x32\x14.clarifai.api.OutputB\x04\x80\xb5\x18\x01\"V\n\x11ListScopesRequest\x12\x10\n\x08key_type\x18\x01 \x01(\t\x12/\n\x0buser_app_id\x18\x02 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\"B\n\x0fMyScopesRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\"F\n\x13MyScopesUserRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\"\x15\n\x13MyScopesRootRequest\"\xa5\x01\n\x16MultiScopeDepsResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12+\n\nscope_deps\x18\x02 \x03(\x0b\x32\x17.clarifai.api.ScopeDeps\x12\x31\n\rendpoint_deps\x18\x03 \x03(\x0b\x32\x1a.clarifai.api.EndpointDeps\"\xa0\x01\n\x12MultiScopeResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x0e\n\x06scopes\x18\x02 \x03(\t\x12\x1e\n\x03\x61pp\x18\x03 \x01(\x0b\x32\x11.clarifai.api.App\x12\x11\n\tendpoints\x18\x04 \x03(\t\x12\x1a\n\x12user_feature_flags\x18\x05 \x01(\t\"\x84\x01\n\x16MultiScopeUserResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x0e\n\x06scopes\x18\x02 \x03(\t\x12\x11\n\tendpoints\x18\x04 \x03(\t\x12\x1a\n\x12user_feature_flags\x18\x05 \x01(\t\"\x84\x01\n\x16MultiScopeRootResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x0e\n\x06scopes\x18\x02 \x03(\t\x12\x11\n\tendpoints\x18\x04 \x03(\t\x12\x1a\n\x12user_feature_flags\x18\x05 \x01(\t\"O\n\x10GetSearchRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\n\n\x02id\x18\x02 \x01(\t\"f\n\x13ListSearchesRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0c\n\x04page\x18\x02 \x01(\r\x12\x10\n\x08per_page\x18\x03 \x01(\r\"\xc4\x01\n\x13PostSearchesRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12&\n\x05query\x18\x02 \x01(\x0b\x32\x13.clarifai.api.QueryB\x02\x18\x01\x12&\n\x08searches\x18\x03 \x03(\x0b\x32\x14.clarifai.api.Search\x12,\n\npagination\x18\x04 \x01(\x0b\x32\x18.clarifai.api.Pagination\"\x85\x01\n\x1aPatchInputsSearchesRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12&\n\x08searches\x18\x02 \x03(\x0b\x32\x14.clarifai.api.Search\x12\x0e\n\x06\x61\x63tion\x18\x03 \x01(\t\"\x8a\x01\n\x1fPatchAnnotationsSearchesRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12&\n\x08searches\x18\x02 \x03(\x0b\x32\x14.clarifai.api.Search\x12\x0e\n\x06\x61\x63tion\x18\x03 \x01(\t\"\x7f\n\x14PatchSearchesRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12&\n\x08searches\x18\x02 \x03(\x0b\x32\x14.clarifai.api.Search\x12\x0e\n\x06\x61\x63tion\x18\x03 \x01(\t\"\x84\x01\n\x17PostSearchesByIDRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\n\n\x02id\x18\x02 \x01(\t\x12,\n\npagination\x18\x03 \x01(\x0b\x32\x18.clarifai.api.Pagination\"R\n\x13\x44\x65leteSearchRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\n\n\x02id\x18\x02 \x01(\t\"\xa7\x01\n\x1ePostAnnotationsSearchesRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12&\n\x08searches\x18\x02 \x03(\x0b\x32\x14.clarifai.api.Search\x12,\n\npagination\x18\x03 \x01(\x0b\x32\x18.clarifai.api.Pagination\"c\n$DeleteAnnotationSearchMetricsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\n\n\x02id\x18\x02 \x01(\t\"\xb6\x01\n\x19PostInputsSearchesRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12&\n\x08searches\x18\x02 \x03(\x0b\x32\x14.clarifai.api.Search\x12,\n\npagination\x18\x03 \x01(\x0b\x32\x18.clarifai.api.Pagination\x12\x12\n\nonly_count\x18\x04 \x01(\x08\"i\n\x14SingleSearchResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12$\n\x06search\x18\x05 \x01(\x0b\x32\x14.clarifai.api.Search\"\xed\x01\n\x13MultiSearchResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\n\n\x02id\x18\x02 \x01(\t\x12%\n\x04hits\x18\x03 \x03(\x0b\x32\x11.clarifai.api.HitB\x04\x80\xb5\x18\x01\x12\"\n\x05query\x18\x04 \x01(\x0b\x32\x13.clarifai.api.Query\x12&\n\x08searches\x18\x05 \x03(\x0b\x32\x14.clarifai.api.Search\x12*\n\nhit_counts\x18\x06 \x03(\x0b\x32\x16.clarifai.api.HitCount\"\x94\x02\n\"PostAnnotationSearchMetricsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\n\n\x02id\x18\x02 \x01(\t\x12*\n\x0cground_truth\x18\x03 \x01(\x0b\x32\x14.clarifai.api.Search\x12,\n\x0esearch_to_eval\x18\x04 \x01(\x0b\x32\x14.clarifai.api.Search\x12 \n\x04\x64\x61ta\x18\x05 \x01(\x0b\x32\x12.clarifai.api.Data\x12\x35\n\x0f\x65valuation_type\x18\x06 \x01(\x0e\x32\x1c.clarifai.api.EvaluationType\"`\n!GetAnnotationSearchMetricsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\n\n\x02id\x18\x02 \x01(\t\"U\n\"ListAnnotationSearchMetricsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\"\x9d\x01\n$MultiAnnotationSearchMetricsResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12H\n\x19\x61nnotation_search_metrics\x18\x02 \x03(\x0b\x32%.clarifai.api.AnnotationSearchMetrics\"o\n\x1cListAnnotationFiltersRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0c\n\x04page\x18\x02 \x01(\r\x12\x10\n\x08per_page\x18\x03 \x01(\r\"k\n\x1aGetAnnotationFilterRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x1c\n\x14\x61nnotation_filter_id\x18\x02 \x01(\t\"\x8b\x01\n\x1cPostAnnotationFiltersRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12:\n\x12\x61nnotation_filters\x18\x02 \x03(\x0b\x32\x1e.clarifai.api.AnnotationFilter\"\x9c\x01\n\x1dPatchAnnotationFiltersRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12:\n\x12\x61nnotation_filters\x18\x02 \x03(\x0b\x32\x1e.clarifai.api.AnnotationFilter\x12\x0e\n\x06\x61\x63tion\x18\x03 \x01(\t\"p\n\x1e\x44\x65leteAnnotationFiltersRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x1d\n\x15\x61nnotation_filter_ids\x18\x02 \x03(\t\"\x8e\x01\n\x1dMultiAnnotationFilterResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12@\n\x12\x61nnotation_filters\x18\x02 \x03(\x0b\x32\x1e.clarifai.api.AnnotationFilterB\x04\x80\xb5\x18\x01\"\x88\x01\n\x1eSingleAnnotationFilterResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x39\n\x11\x61nnotation_filter\x18\x02 \x01(\x0b\x32\x1e.clarifai.api.AnnotationFilter\"\\\n\x0eGetUserRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x19\n\x11\x61\x64\x64itional_fields\x18\x02 \x03(\t\"c\n\x12SingleUserResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12 \n\x04user\x18\x02 \x01(\x0b\x32\x12.clarifai.api.User\"x\n\x1bPostValidatePasswordRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12(\n\x08password\x18\x02 \x01(\x0b\x32\x16.clarifai.api.Password\"\x8e\x01\n SinglePasswordValidationResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12=\n\x13password_violations\x18\x02 \x01(\x0b\x32 .clarifai.api.PasswordViolations\"\xbb\x01\n\x12GetWorkflowRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x13\n\x0bworkflow_id\x18\x02 \x01(\t\x12 \n\x18\x66\x61vor_clarifai_workflows\x18\x03 \x01(\x08\x12\x19\n\x11\x61\x64\x64itional_fields\x18\x04 \x03(\t\x12\"\n\x1a\x65xclude_clarifai_workflows\x18\x05 \x01(\x08\"\xbb\x02\n\x14ListWorkflowsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0c\n\x04page\x18\x02 \x01(\r\x12\x10\n\x08per_page\x18\x03 \x01(\r\x12\x16\n\x0esort_ascending\x18\x05 \x01(\x08\x12\x14\n\nsort_by_id\x18\x06 \x01(\x08H\x00\x12\x1d\n\x13sort_by_modified_at\x18\x07 \x01(\x08H\x00\x12\r\n\x05query\x18\x08 \x01(\t\x12\x0e\n\x02id\x18\x04 \x01(\tB\x02\x18\x01\x12\x15\n\rfeatured_only\x18\t \x01(\x08\x12\x14\n\x0cstarred_only\x18\x0b \x01(\x08\x12\x19\n\x11\x61\x64\x64itional_fields\x18\n \x03(\t\x12\x13\n\x0bsearch_term\x18\x0c \x01(\tB\t\n\x07sort_by\"r\n\x14PostWorkflowsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12)\n\tworkflows\x18\x02 \x03(\x0b\x32\x16.clarifai.api.Workflow\"\x83\x01\n\x15PatchWorkflowsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12)\n\tworkflows\x18\x02 \x03(\x0b\x32\x16.clarifai.api.Workflow\x12\x0e\n\x06\x61\x63tion\x18\x03 \x01(\t\"\x85\x01\n\x17PatchWorkflowIdsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12)\n\x03ids\x18\x03 \x03(\x0b\x32\x1c.clarifai.api.IdUpdateSource\x12\x0e\n\x06\x61\x63tion\x18\x04 \x01(\t\"]\n\x15\x44\x65leteWorkflowRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x13\n\x0bworkflow_id\x18\x02 \x01(\t\"j\n\x16\x44\x65leteWorkflowsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0b\n\x03ids\x18\x02 \x03(\t\x12\x12\n\ndelete_all\x18\x03 \x01(\x08\"o\n\x16SingleWorkflowResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12(\n\x08workflow\x18\x02 \x01(\x0b\x32\x16.clarifai.api.Workflow\"u\n\x15MultiWorkflowResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12/\n\tworkflows\x18\x02 \x03(\x0b\x32\x16.clarifai.api.WorkflowB\x04\x80\xb5\x18\x01\"\xa5\x02\n\x1aPostWorkflowResultsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x13\n\x0bworkflow_id\x18\x02 \x01(\t\x12\x12\n\nversion_id\x18\x07 \x01(\t\x12#\n\x06inputs\x18\x03 \x03(\x0b\x32\x13.clarifai.api.Input\x12\x31\n\routput_config\x18\x04 \x01(\x0b\x32\x1a.clarifai.api.OutputConfig\x12 \n\x18\x66\x61vor_clarifai_workflows\x18\x05 \x01(\x08\x12\x33\n\x0eworkflow_state\x18\x06 \x01(\x0b\x32\x1b.clarifai.api.WorkflowState\"\xd8\x01\n\x1bPostWorkflowResultsResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12(\n\x08workflow\x18\x02 \x01(\x0b\x32\x16.clarifai.api.Workflow\x12-\n\x07results\x18\x03 \x03(\x0b\x32\x1c.clarifai.api.WorkflowResult\x12\x33\n\x0eworkflow_state\x18\x04 \x01(\x0b\x32\x1b.clarifai.api.WorkflowState\"\x91\x02\n$PostWorkflowResultsSimilarityRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x13\n\x0bworkflow_id\x18\x02 \x01(\t\x12\x12\n\nversion_id\x18\x07 \x01(\t\x12\x18\n\x10model_version_id\x18\x03 \x01(\t\x12)\n\x0cprobe_inputs\x18\x04 \x03(\x0b\x32\x13.clarifai.api.Input\x12(\n\x0bpool_inputs\x18\x05 \x03(\x0b\x32\x13.clarifai.api.Input\x12 \n\x18\x66\x61vor_clarifai_workflows\x18\x06 \x01(\x08\"\x8e\x01\n%PostWorkflowResultsSimilarityResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x38\n\x07results\x18\x02 \x03(\x0b\x32\'.clarifai.api.WorkflowResultsSimilarity\"\x83\x01\n\x1bListWorkflowVersionsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x13\n\x0bworkflow_id\x18\x02 \x01(\t\x12\x0c\n\x04page\x18\x03 \x01(\r\x12\x10\n\x08per_page\x18\x04 \x01(\r\"~\n\x19GetWorkflowVersionRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x13\n\x0bworkflow_id\x18\x02 \x01(\t\x12\x1b\n\x13workflow_version_id\x18\x03 \x01(\t\"\x83\x01\n\x1d\x44\x65leteWorkflowVersionsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x13\n\x0bworkflow_id\x18\x02 \x01(\t\x12\x1c\n\x14workflow_version_ids\x18\x03 \x03(\t\"\xae\x01\n\x1cPatchWorkflowVersionsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x13\n\x0bworkflow_id\x18\x02 \x01(\t\x12\x38\n\x11workflow_versions\x18\x03 \x03(\x0b\x32\x1d.clarifai.api.WorkflowVersion\x12\x0e\n\x06\x61\x63tion\x18\x04 \x01(\t\"\x8b\x01\n\x1cMultiWorkflowVersionResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12>\n\x11workflow_versions\x18\x02 \x03(\x0b\x32\x1d.clarifai.api.WorkflowVersionB\x04\x80\xb5\x18\x01\"\x85\x01\n\x1dSingleWorkflowVersionResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x37\n\x10workflow_version\x18\x02 \x01(\x0b\x32\x1d.clarifai.api.WorkflowVersion\"\x85\x01\n\x1aPostAppDuplicationsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x36\n\x10\x61pp_duplications\x18\x02 \x03(\x0b\x32\x1c.clarifai.api.AppDuplication\"g\n\x18GetAppDuplicationRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x1a\n\x12\x61pp_duplication_id\x18\x02 \x01(\t\"m\n\x1aListAppDuplicationsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0c\n\x04page\x18\x02 \x01(\r\x12\x10\n\x08per_page\x18\x03 \x01(\r\"\x83\x01\n\x1cMultiAppDuplicationsResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x36\n\x10\x61pp_duplications\x18\x02 \x03(\x0b\x32\x1c.clarifai.api.AppDuplication\"\x82\x01\n\x1cSingleAppDuplicationResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x35\n\x0f\x61pp_duplication\x18\x02 \x01(\x0b\x32\x1c.clarifai.api.AppDuplication\"f\n\x10PostTasksRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12!\n\x05tasks\x18\x02 \x03(\x0b\x32\x12.clarifai.api.Task\"m\n\x0eGetTaskRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0f\n\x07task_id\x18\x02 \x01(\t\x12\x19\n\x11\x61\x64\x64itional_fields\x18\x03 \x03(\t\"\xee\x01\n\x10ListTasksRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0c\n\x04page\x18\x02 \x01(\r\x12\x10\n\x08per_page\x18\x03 \x01(\r\x12\x17\n\x0fworker_user_ids\x18\x04 \x03(\t\x12\x17\n\x0freview_user_ids\x18\x05 \x03(\t\x12\x17\n\x0flabel_order_ids\x18\x08 \x03(\t\x12#\n\x1bincluding_label_order_tasks\x18\x06 \x01(\x08\x12\x19\n\x11\x61\x64\x64itional_fields\x18\x07 \x03(\t\"w\n\x11PatchTasksRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12!\n\x05tasks\x18\x02 \x03(\x0b\x32\x12.clarifai.api.Task\x12\x0e\n\x06\x61\x63tion\x18\x03 \x01(\t\"R\n\x12\x44\x65leteTasksRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0b\n\x03ids\x18\x02 \x03(\t\"i\n\x11MultiTaskResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\'\n\x05tasks\x18\x02 \x03(\x0b\x32\x12.clarifai.api.TaskB\x04\x80\xb5\x18\x01\"c\n\x12SingleTaskResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12 \n\x04task\x18\x02 \x01(\x0b\x32\x12.clarifai.api.Task\"i\n\x13GetTaskCountRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0f\n\x07task_id\x18\x02 \x01(\t\x12\x10\n\x08user_ids\x18\x03 \x03(\t\"\x9d\x01\n\x17SingleTaskCountResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x0e\n\x06\x61pp_id\x18\x02 \x01(\t\x12\x0f\n\x07task_id\x18\x03 \x01(\t\x12\x34\n\x06\x63ounts\x18\x04 \x03(\x0b\x32$.clarifai.api.TaskStatusCountPerUser\"y\n\x16PostLabelOrdersRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12.\n\x0clabel_orders\x18\x02 \x03(\x0b\x32\x18.clarifai.api.LabelOrder\"_\n\x14GetLabelOrderRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x16\n\x0elabel_order_id\x18\x02 \x01(\t\"i\n\x16ListLabelOrdersRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0c\n\x04page\x18\x02 \x01(\r\x12\x10\n\x08per_page\x18\x03 \x01(\r\"\x8a\x01\n\x17PatchLabelOrdersRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12.\n\x0clabel_orders\x18\x02 \x03(\x0b\x32\x18.clarifai.api.LabelOrder\x12\x0e\n\x06\x61\x63tion\x18\x03 \x01(\t\"X\n\x18\x44\x65leteLabelOrdersRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0b\n\x03ids\x18\x02 \x03(\t\"|\n\x17MultiLabelOrderResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x34\n\x0clabel_orders\x18\x02 \x03(\x0b\x32\x18.clarifai.api.LabelOrderB\x04\x80\xb5\x18\x01\"v\n\x18SingleLabelOrderResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12-\n\x0blabel_order\x18\x02 \x01(\x0b\x32\x18.clarifai.api.LabelOrder\"u\n\x15PostCollectorsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12+\n\ncollectors\x18\x02 \x03(\x0b\x32\x17.clarifai.api.Collector\"\x86\x01\n\x16PatchCollectorsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12+\n\ncollectors\x18\x02 \x03(\x0b\x32\x17.clarifai.api.Collector\x12\x0e\n\x06\x61\x63tion\x18\x03 \x01(\t\"k\n\x17\x44\x65leteCollectorsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0b\n\x03ids\x18\x02 \x03(\t\x12\x12\n\ndelete_all\x18\x03 \x01(\x08\"\\\n\x13GetCollectorRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x14\n\x0c\x63ollector_id\x18\x02 \x01(\t\"h\n\x15ListCollectorsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0c\n\x04page\x18\x02 \x01(\r\x12\x10\n\x08per_page\x18\x03 \x01(\r\"r\n\x16MultiCollectorResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12+\n\ncollectors\x18\x02 \x03(\x0b\x32\x17.clarifai.api.Collector\"r\n\x17SingleCollectorResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12*\n\tcollector\x18\x02 \x01(\x0b\x32\x17.clarifai.api.Collector\"v\n\x15PostStatValuesRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12,\n\x0bstat_values\x18\x02 \x03(\x0b\x32\x17.clarifai.api.StatValue\"y\n\x16MultiStatValueResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x32\n\x0bstat_values\x18\x02 \x03(\x0b\x32\x17.clarifai.api.StatValueB\x04\x80\xb5\x18\x01\"\x9e\x01\n\x1ePostStatValuesAggregateRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12K\n\x1cstat_value_aggregate_queries\x18\x02 \x03(\x0b\x32%.clarifai.api.StatValueAggregateQuery\"\x9c\x01\n\x1fMultiStatValueAggregateResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12L\n\x1cstat_value_aggregate_results\x18\x02 \x03(\x0b\x32&.clarifai.api.StatValueAggregateResult\"w\n\x1ePostTrendingMetricsViewRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x11\n\tview_type\x18\x02 \x01(\t\x12\x11\n\tobject_id\x18\x03 \x01(\t\"\x85\x01\n\x1fListTrendingMetricsViewsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x11\n\tview_type\x18\x02 \x01(\t\x12\x0c\n\x04page\x18\x03 \x01(\r\x12\x10\n\x08per_page\x18\x04 \x01(\r\"~\n MultiTrendingMetricsViewResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12-\n\x07metrics\x18\x02 \x03(\x0b\x32\x1c.clarifai.api.TrendingMetric\"q\n\x10GetModuleRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x11\n\tmodule_id\x18\x02 \x01(\t\x12\x19\n\x11\x61\x64\x64itional_fields\x18\x03 \x03(\t\"\x96\x01\n\x12ListModulesRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0c\n\x04page\x18\x02 \x01(\r\x12\x10\n\x08per_page\x18\x03 \x01(\r\x12\x14\n\x0cstarred_only\x18\x04 \x01(\x08\x12\x19\n\x11\x61\x64\x64itional_fields\x18\x05 \x03(\t\"l\n\x12PostModulesRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12%\n\x07modules\x18\x03 \x03(\x0b\x32\x14.clarifai.api.Module\"}\n\x13PatchModulesRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12%\n\x07modules\x18\x02 \x03(\x0b\x32\x14.clarifai.api.Module\x12\x0e\n\x06\x61\x63tion\x18\x03 \x01(\t\"T\n\x14\x44\x65leteModulesRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0b\n\x03ids\x18\x02 \x03(\t\"i\n\x14SingleModuleResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12$\n\x06module\x18\x02 \x01(\x0b\x32\x14.clarifai.api.Module\"o\n\x13MultiModuleResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12+\n\x07modules\x18\x02 \x03(\x0b\x32\x14.clarifai.api.ModuleB\x04\x80\xb5\x18\x01\"x\n\x17GetModuleVersionRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x11\n\tmodule_id\x18\x02 \x01(\t\x12\x19\n\x11module_version_id\x18\x03 \x01(\t\"\x7f\n\x19ListModuleVersionsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x11\n\tmodule_id\x18\x02 \x01(\t\x12\x0c\n\x04page\x18\x03 \x01(\r\x12\x10\n\x08per_page\x18\x04 \x01(\r\"\x95\x01\n\x19PostModuleVersionsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x11\n\tmodule_id\x18\x02 \x01(\t\x12\x34\n\x0fmodule_versions\x18\x03 \x03(\x0b\x32\x1b.clarifai.api.ModuleVersion\"n\n\x1b\x44\x65leteModuleVersionsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x11\n\tmodule_id\x18\x02 \x01(\t\x12\x0b\n\x03ids\x18\x03 \x03(\t\"\x7f\n\x1bSingleModuleVersionResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x33\n\x0emodule_version\x18\x02 \x01(\x0b\x32\x1b.clarifai.api.ModuleVersion\"\x85\x01\n\x1aMultiModuleVersionResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12:\n\x0fmodule_versions\x18\x02 \x03(\x0b\x32\x1b.clarifai.api.ModuleVersionB\x04\x80\xb5\x18\x01\"x\n GetInstalledModuleVersionRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12#\n\x1binstalled_module_version_id\x18\x02 \x01(\t\"u\n\"ListInstalledModuleVersionsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0c\n\x04page\x18\x02 \x01(\r\x12\x10\n\x08per_page\x18\x03 \x01(\r\"\x9e\x01\n\"PostInstalledModuleVersionsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12G\n\x19installed_module_versions\x18\x02 \x03(\x0b\x32$.clarifai.api.InstalledModuleVersion\"}\n%PostInstalledModuleVersionsKeyRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12#\n\x1binstalled_module_version_id\x18\x02 \x01(\t\"d\n$DeleteInstalledModuleVersionsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0b\n\x03ids\x18\x02 \x03(\t\"\x9b\x01\n$SingleInstalledModuleVersionResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x46\n\x18installed_module_version\x18\x02 \x01(\x0b\x32$.clarifai.api.InstalledModuleVersion\"\xa1\x01\n#MultiInstalledModuleVersionResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12M\n\x19installed_module_versions\x18\x02 \x03(\x0b\x32$.clarifai.api.InstalledModuleVersionB\x04\x80\xb5\x18\x01\"b\n\x1eListNextTaskAssignmentsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0f\n\x07task_id\x18\x02 \x01(\t\"\x82\x01\n\x19PostBulkOperationsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x34\n\x0f\x62ulk_operations\x18\x02 \x03(\x0b\x32\x1b.clarifai.api.BulkOperation\"l\n\x19ListBulkOperationsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0c\n\x04page\x18\x02 \x01(\r\x12\x10\n\x08per_page\x18\x03 \x01(\r\"V\n\x17GetBulkOperationRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\n\n\x02id\x18\x02 \x01(\t\"Z\n\x1a\x43\x61ncelBulkOperationRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0b\n\x03ids\x18\x02 \x03(\t\"Z\n\x1a\x44\x65leteBulkOperationRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0b\n\x03ids\x18\x02 \x03(\t\"\x80\x01\n\x1cSingleBulkOperationsResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x33\n\x0e\x62ulk_operation\x18\x02 \x01(\x0b\x32\x1b.clarifai.api.BulkOperation\"\x7f\n\x1bMultiBulkOperationsResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x33\n\x0e\x62ulk_operation\x18\x02 \x03(\x0b\x32\x1b.clarifai.api.BulkOperation\"o\n\x19PutTaskAssignmentsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0f\n\x07task_id\x18\x02 \x01(\t\x12\x10\n\x08input_id\x18\x03 \x01(\t\"k\n\x18ListInputsAddJobsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0c\n\x04page\x18\x02 \x01(\r\x12\x10\n\x08per_page\x18\x03 \x01(\r\"U\n\x16GetInputsAddJobRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\n\n\x02id\x18\x02 \x01(\t\"\x83\x01\n\x19MultiInputsAddJobResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x39\n\x0finputs_add_jobs\x18\x02 \x03(\x0b\x32\x1a.clarifai.api.InputsAddJobB\x04\x80\xb5\x18\x01\"}\n\x1aSingleInputsAddJobResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x32\n\x0einputs_add_job\x18\x02 \x01(\x0b\x32\x1a.clarifai.api.InputsAddJob\"l\n\x12PostUploadsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12%\n\x07uploads\x18\x02 \x03(\x0b\x32\x14.clarifai.api.Upload\"T\n\x14\x44\x65leteUploadsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0b\n\x03ids\x18\x02 \x03(\t\"e\n\x12ListUploadsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0c\n\x04page\x18\x02 \x01(\r\x12\x10\n\x08per_page\x18\x03 \x01(\r\"V\n\x10GetUploadRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x11\n\tupload_id\x18\x02 \x01(\t\"i\n\x14SingleUploadResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12$\n\x06upload\x18\x02 \x01(\x0b\x32\x14.clarifai.api.Upload\"i\n\x13MultiUploadResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12%\n\x07uploads\x18\x02 \x03(\x0b\x32\x14.clarifai.api.Upload\"\x9a\x01\n\x1cPutUploadContentPartsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x11\n\tupload_id\x18\x02 \x01(\t\x12\x36\n\rcontent_parts\x18\x03 \x03(\x0b\x32\x1f.clarifai.api.UploadContentPart\"\xad\x01\n\x1cPostInputsDataSourcesRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x34\n\x0c\x64\x61ta_sources\x18\x02 \x03(\x0b\x32\x1e.clarifai.api.InputsDataSource\x12\x15\n\rcall_back_url\x18\x03 \x01(\t\x12\x0f\n\x07\x61pp_pat\x18\x04 \x01(\t\"r\n\x1dGetInputsExtractionJobRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12 \n\x18inputs_extraction_job_id\x18\x02 \x01(\t\"r\n\x1fListInputsExtractionJobsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0c\n\x04page\x18\x02 \x01(\r\x12\x10\n\x08per_page\x18\x03 \x01(\r\"\x92\x01\n!SingleInputsExtractionJobResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12@\n\x15inputs_extraction_job\x18\x02 \x01(\x0b\x32!.clarifai.api.InputsExtractionJob\"\x92\x01\n MultiInputsExtractionJobResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x41\n\x16inputs_extraction_jobs\x18\x02 \x03(\x0b\x32!.clarifai.api.InputsExtractionJob\"a\n!CancelInputsExtractionJobsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0b\n\x03ids\x18\x02 \x03(\t\"\x7f\n\x18PostInputsUploadsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x32\n\x0einputs_uploads\x18\x02 \x03(\x0b\x32\x1a.clarifai.api.InputsUpload*p\n\x1cOrganizationInvitationStatus\x12\x0b\n\x07NOT_SET\x10\x00\x12\x0b\n\x07PENDING\x10\x01\x12\x0c\n\x08\x41\x43\x43\x45PTED\x10\x02\x12\r\n\tCANCELLED\x10\x03\x12\x0c\n\x08\x44\x45\x43LINED\x10\x04\x12\x0b\n\x07\x45XPIRED\x10\x05\x32\x96\xf5\x02\n\x02V2\x12\xaa\x02\n\x14ListConceptRelations\x12).clarifai.api.ListConceptRelationsRequest\x1a*.clarifai.api.MultiConceptRelationResponse\"\xba\x01\x82\xd3\xe4\x93\x02\xab\x01\x12Y/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/concepts/{concept_id}/relationsZN\x12L/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/concepts/relations\x98\x9c\'\x05\x90\x9c\'\x0b\x12\xdf\x01\n\x14PostConceptRelations\x12).clarifai.api.PostConceptRelationsRequest\x1a*.clarifai.api.MultiConceptRelationResponse\"p\x82\xd3\xe4\x93\x02^\"Y/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/concepts/{concept_id}/relations:\x01*\x98\x9c\'\x05\x90\x9c\'\n\x90\x9c\'\x0b\x12\xde\x01\n\x16\x44\x65leteConceptRelations\x12+.clarifai.api.DeleteConceptRelationsRequest\x1a!.clarifai.api.status.BaseResponse\"t\x82\xd3\xe4\x93\x02^*Y/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/concepts/{concept_id}/relations:\x01*\x98\x9c\'\x05\x90\x9c\'\r\x90\x9c\'\n\x90\x9c\'\x0b\x12\xdc\x01\n\x10GetConceptCounts\x12%.clarifai.api.GetConceptCountsRequest\x1a\'.clarifai.api.MultiConceptCountResponse\"x\x82\xd3\xe4\x93\x02\x62\x12I/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/concepts/statusZ\x15\x12\x13/v2/concepts/status\x98\x9c\'\x02\x90\x9c\'&\x90\x9c\'\x0b\x90\x9c\'\x05\x12\xd0\x01\n\nGetConcept\x12\x1f.clarifai.api.GetConceptRequest\x1a#.clarifai.api.SingleConceptResponse\"|\x82\xd3\xe4\x93\x02n\x12O/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/concepts/{concept_id}Z\x1b\x12\x19/v2/concepts/{concept_id}\x98\x9c\'\x02\x90\x9c\'\x0b\x12\xb9\x01\n\x0cListConcepts\x12!.clarifai.api.ListConceptsRequest\x1a\".clarifai.api.MultiConceptResponse\"b\x82\xd3\xe4\x93\x02T\x12\x42/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/conceptsZ\x0e\x12\x0c/v2/concepts\x98\x9c\'\x02\x90\x9c\'\x0b\x12\xb9\x02\n\x11ListModelConcepts\x12&.clarifai.api.ListModelConceptsRequest\x1a\".clarifai.api.MultiConceptResponse\"\xd7\x01\x82\xd3\xe4\x93\x02\xc4\x01\x12T/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}/conceptsZl\x12j/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}/versions/{version_id}/concepts\x98\x9c\'\x02\x90\x9c\'\x0b\x90\x9c\'\x0f\x12\xea\x01\n\x14PostConceptsSearches\x12).clarifai.api.PostConceptsSearchesRequest\x1a\".clarifai.api.MultiConceptResponse\"\x82\x01\x82\xd3\xe4\x93\x02l\"K/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/concepts/searches:\x01*Z\x1a\"\x15/v2/concepts/searches:\x01*\x98\x9c\'\x02\x90\x9c\'\x0b\x90\x9c\'\x0f\x90\x9c\'\x13\x12\xc3\x01\n\x0cPostConcepts\x12!.clarifai.api.PostConceptsRequest\x1a\".clarifai.api.MultiConceptResponse\"l\x82\xd3\xe4\x93\x02Z\"B/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/concepts:\x01*Z\x11\"\x0c/v2/concepts:\x01*\x98\x9c\'\x02\x90\x9c\'\n\x90\x9c\'\x0b\x12\xc5\x01\n\rPatchConcepts\x12\".clarifai.api.PatchConceptsRequest\x1a\".clarifai.api.MultiConceptResponse\"l\x82\xd3\xe4\x93\x02Z2B/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/concepts:\x01*Z\x11\x32\x0c/v2/concepts:\x01*\x98\x9c\'\x02\x90\x9c\'\n\x90\x9c\'\x0b\x12\x94\x02\n\x12GetConceptLanguage\x12\'.clarifai.api.GetConceptLanguageRequest\x1a+.clarifai.api.SingleConceptLanguageResponse\"\xa7\x01\x82\xd3\xe4\x93\x02\x98\x01\x12\x64/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/concepts/{concept_id}/languages/{language}Z0\x12./v2/concepts/{concept_id}/languages/{language}\x98\x9c\'\x02\x90\x9c\'\x0b\x12\x81\x02\n\x14ListConceptLanguages\x12).clarifai.api.ListConceptLanguagesRequest\x1a*.clarifai.api.MultiConceptLanguageResponse\"\x91\x01\x82\xd3\xe4\x93\x02\x82\x01\x12Y/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/concepts/{concept_id}/languagesZ%\x12#/v2/concepts/{concept_id}/languages\x98\x9c\'\x02\x90\x9c\'\x0b\x12\x8b\x02\n\x14PostConceptLanguages\x12).clarifai.api.PostConceptLanguagesRequest\x1a*.clarifai.api.MultiConceptLanguageResponse\"\x9b\x01\x82\xd3\xe4\x93\x02\x88\x01\"Y/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/concepts/{concept_id}/languages:\x01*Z(\"#/v2/concepts/{concept_id}/languages:\x01*\x98\x9c\'\x02\x90\x9c\'\n\x90\x9c\'\x0b\x12\x8d\x02\n\x15PatchConceptLanguages\x12*.clarifai.api.PatchConceptLanguagesRequest\x1a*.clarifai.api.MultiConceptLanguageResponse\"\x9b\x01\x82\xd3\xe4\x93\x02\x88\x01\x32Y/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/concepts/{concept_id}/languages:\x01*Z(2#/v2/concepts/{concept_id}/languages:\x01*\x98\x9c\'\x02\x90\x9c\'\n\x90\x9c\'\x0b\x12\xf1\x01\n\x13ListKnowledgeGraphs\x12(.clarifai.api.ListKnowledgeGraphsRequest\x1a).clarifai.api.MultiKnowledgeGraphResponse\"\x84\x01\x82\xd3\xe4\x93\x02v\x12S/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/concepts/knowledge_graphsZ\x1f\x12\x1d/v2/concepts/knowledge_graphs\x98\x9c\'\x02\x90\x9c\'\x0b\x12\xfb\x01\n\x13PostKnowledgeGraphs\x12(.clarifai.api.PostKnowledgeGraphsRequest\x1a).clarifai.api.MultiKnowledgeGraphResponse\"\x8e\x01\x82\xd3\xe4\x93\x02|\"S/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/concepts/knowledge_graphs:\x01*Z\"\"\x1d/v2/concepts/knowledge_graphs:\x01*\x98\x9c\'\x02\x90\x9c\'\n\x90\x9c\'\x0b\x12\xfe\x01\n\x16PostConceptMappingJobs\x12+.clarifai.api.PostConceptMappingJobsRequest\x1a,.clarifai.api.MultiConceptMappingJobResponse\"\x88\x01\x82\xd3\xe4\x93\x02v\"P/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/concepts/mappings/jobs:\x01*Z\x1f\"\x1a/v2/concepts/mappings/jobs:\x01*\x98\x9c\'\x02\x90\x9c\'\n\x90\x9c\'\x0b\x12\x93\x02\n\rGetAnnotation\x12\".clarifai.api.GetAnnotationRequest\x1a&.clarifai.api.SingleAnnotationResponse\"\xb5\x01\x82\xd3\xe4\x93\x02\x9e\x01\x12g/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/inputs/{input_id}/annotations/{annotation_id}Z3\x12\x31/v2/inputs/{input_id}/annotations/{annotation_id}\x98\x9c\'\x02\x90\x9c\'&\x90\x9c\'\x0b\x90\x9c\'\x0f\x12\xd0\x01\n\x0fListAnnotations\x12$.clarifai.api.ListAnnotationsRequest\x1a%.clarifai.api.MultiAnnotationResponse\"p\x82\xd3\xe4\x93\x02Z\x12\x45/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/annotationsZ\x11\x12\x0f/v2/annotations\x98\x9c\'\x02\x90\x9c\'&\x90\x9c\'\x0b\x90\x9c\'\x0f\x12\xe3\x01\n\x0fPostAnnotations\x12$.clarifai.api.PostAnnotationsRequest\x1a%.clarifai.api.MultiAnnotationResponse\"\x82\x01\x82\xd3\xe4\x93\x02`\"E/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/annotations:\x01*Z\x14\"\x0f/v2/annotations:\x01*\x98\x9c\'\x02\x90\x9c\'\x05\x90\x9c\'%\x90\x9c\'&\x90\x9c\'\x0b\x90\x9c\'\x0f\x90\x9c\'\x13\x12\xe5\x01\n\x10PatchAnnotations\x12%.clarifai.api.PatchAnnotationsRequest\x1a%.clarifai.api.MultiAnnotationResponse\"\x82\x01\x82\xd3\xe4\x93\x02`2E/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/annotations:\x01*Z\x14\x32\x0f/v2/annotations:\x01*\x98\x9c\'\x02\x90\x9c\'\x05\x90\x9c\'%\x90\x9c\'&\x90\x9c\'\x0b\x90\x9c\'\x13\x90\x9c\'\x0f\x12\xf3\x01\n\x16PatchAnnotationsStatus\x12+.clarifai.api.PatchAnnotationsStatusRequest\x1a,.clarifai.api.PatchAnnotationsStatusResponse\"~\x82\xd3\xe4\x93\x02`2[/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/task/{task_id}/annotations/status:\x01*\x98\x9c\'\x02\x90\x9c\'%\x90\x9c\'&\x90\x9c\'\x0b\x90\x9c\'\x13\x90\x9c\'\x0f\x12\x9c\x02\n\x10\x44\x65leteAnnotation\x12%.clarifai.api.DeleteAnnotationRequest\x1a!.clarifai.api.status.BaseResponse\"\xbd\x01\x82\xd3\xe4\x93\x02\x9e\x01*g/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/inputs/{input_id}/annotations/{annotation_id}Z3*1/v2/inputs/{input_id}/annotations/{annotation_id}\x98\x9c\'\x02\x90\x9c\'%\x90\x9c\'(\x90\x9c\'&\x90\x9c\'\x13\x90\x9c\'\x0f\x12\xd0\x02\n\x11\x44\x65leteAnnotations\x12&.clarifai.api.DeleteAnnotationsRequest\x1a!.clarifai.api.status.BaseResponse\"\xef\x01\x82\xd3\xe4\x93\x02\xd0\x01*L/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/inputs/annotations:\x01*Z\x1b*\x16/v2/inputs/annotations:\x01*ZJ*E/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/annotations:\x01*Z\x14*\x0f/v2/annotations:\x01*\x98\x9c\'\x02\x90\x9c\'%\x90\x9c\'(\x90\x9c\'&\x90\x9c\'\x13\x90\x9c\'\x0f\x12\xf3\x01\n\x18PatchAnnotationsSearches\x12-.clarifai.api.PatchAnnotationsSearchesRequest\x1a!.clarifai.api.MultiSearchResponse\"\x84\x01\x82\xd3\xe4\x93\x02r2N/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/annotations/searches:\x01*Z\x1d\x32\x18/v2/annotations/searches:\x01*\x98\x9c\'\x02\x90\x9c\'s\x90\x9c\'r\x12\x81\x02\n\x17PostAnnotationsSearches\x12,.clarifai.api.PostAnnotationsSearchesRequest\x1a!.clarifai.api.MultiSearchResponse\"\x94\x01\x82\xd3\xe4\x93\x02r\"N/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/annotations/searches:\x01*Z\x1d\"\x18/v2/annotations/searches:\x01*\x98\x9c\'\x02\x90\x9c\'&\x90\x9c\'\x0b\x90\x9c\'\x05\x90\x9c\'\x0f\x90\x9c\'\x03\x90\x9c\'\x13\x12\xd1\x01\n\rGetInputCount\x12\".clarifai.api.GetInputCountRequest\x1a&.clarifai.api.SingleInputCountResponse\"t\x82\xd3\xe4\x93\x02^\x12G/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/inputs/statusZ\x13\x12\x11/v2/inputs/status\x98\x9c\'\x02\x90\x9c\'&\x90\x9c\'\x0b\x90\x9c\'\x05\x12\xc9\x01\n\x0cStreamInputs\x12!.clarifai.api.StreamInputsRequest\x1a .clarifai.api.MultiInputResponse\"t\x82\xd3\xe4\x93\x02^\x12G/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/inputs/streamZ\x13\x12\x11/v2/inputs/stream\x98\x9c\'\x02\x90\x9c\'&\x90\x9c\'\x0b\x90\x9c\'\x05\x12\xfd\x01\n\x0fGetInputSamples\x12$.clarifai.api.GetInputSamplesRequest\x1a*.clarifai.api.MultiInputAnnotationResponse\"\x97\x01\x82\xd3\xe4\x93\x02\x80\x01\x12X/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/tasks/{task_id}/inputs/samplesZ$\x12\"/v2/tasks/{task_id}/inputs/samples\x98\x9c\'\x02\x90\x9c\'&\x90\x9c\'\x0b\x90\x9c\'\x05\x12\xca\x01\n\x08GetInput\x12\x1d.clarifai.api.GetInputRequest\x1a!.clarifai.api.SingleInputResponse\"|\x82\xd3\xe4\x93\x02\x66\x12K/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/inputs/{input_id}Z\x17\x12\x15/v2/inputs/{input_id}\x98\x9c\'\x02\x90\x9c\'&\x90\x9c\'\x0b\x90\x9c\'\x05\x12\xfc\x01\n\x15GetInputVideoManifest\x12%.clarifai.api.GetVideoManifestRequest\x1a&.clarifai.api.GetVideoManifestResponse\"\x93\x01\x82\xd3\xe4\x93\x02\x84\x01\x12Z/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/inputs/{input_id}/video_manifestZ&\x12$/v2/inputs/{input_id}/video_manifest\x98\x9c\'\x02\x90\x9c\'\x05\x12\xb7\x01\n\nListInputs\x12\x1f.clarifai.api.ListInputsRequest\x1a .clarifai.api.MultiInputResponse\"f\x82\xd3\xe4\x93\x02P\x12@/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/inputsZ\x0c\x12\n/v2/inputs\x98\x9c\'\x02\x90\x9c\'&\x90\x9c\'\x0b\x90\x9c\'\x05\x12\xd2\x01\n\nPostInputs\x12\x1f.clarifai.api.PostInputsRequest\x1a .clarifai.api.MultiInputResponse\"\x80\x01\x82\xd3\xe4\x93\x02V\"@/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/inputs:\x01*Z\x0f\"\n/v2/inputs:\x01*\x98\x9c\'\x02\x90\x9c\'%\x90\x9c\'&\x90\x9c\'\x0b\x90\x9c\'\x04\x90\x9c\'\x05\x90\x9c\'\x0f\x90\x9c\'\x02\x90\x9c\'\x13\x12\xcb\x01\n\x0bPatchInputs\x12 .clarifai.api.PatchInputsRequest\x1a .clarifai.api.MultiInputResponse\"x\x82\xd3\xe4\x93\x02V2@/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/inputs:\x01*Z\x0f\x32\n/v2/inputs:\x01*\x98\x9c\'\x02\x90\x9c\'%\x90\x9c\'&\x90\x9c\'\x0b\x90\x9c\'\x04\x90\x9c\'\x05\x90\x9c\'\x0f\x12\xe5\x01\n\x0b\x44\x65leteInput\x12 .clarifai.api.DeleteInputRequest\x1a!.clarifai.api.status.BaseResponse\"\x90\x01\x82\xd3\xe4\x93\x02\x66*K/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/inputs/{input_id}Z\x17*\x15/v2/inputs/{input_id}\x98\x9c\'\x02\x90\x9c\'%\x90\x9c\'(\x90\x9c\'&\x90\x9c\'\x04\x90\x9c\'\x08\x90\x9c\'\x05\x90\x9c\'\x0f\x90\x9c\'\x13\x12\xd7\x01\n\x0c\x44\x65leteInputs\x12!.clarifai.api.DeleteInputsRequest\x1a!.clarifai.api.status.BaseResponse\"\x80\x01\x82\xd3\xe4\x93\x02V*@/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/inputs:\x01*Z\x0f*\n/v2/inputs:\x01*\x98\x9c\'\x02\x90\x9c\'%\x90\x9c\'(\x90\x9c\'&\x90\x9c\'\x04\x90\x9c\'\x08\x90\x9c\'\x05\x90\x9c\'\x0f\x90\x9c\'\x13\x12\xde\x01\n\x13PatchInputsSearches\x12(.clarifai.api.PatchInputsSearchesRequest\x1a!.clarifai.api.MultiSearchResponse\"z\x82\xd3\xe4\x93\x02h2I/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/inputs/searches:\x01*Z\x18\x32\x13/v2/inputs/searches:\x01*\x98\x9c\'\x02\x90\x9c\'s\x90\x9c\'r\x12\xed\x01\n\x12PostInputsSearches\x12\'.clarifai.api.PostInputsSearchesRequest\x1a!.clarifai.api.MultiSearchResponse\"\x8a\x01\x82\xd3\xe4\x93\x02h\"I/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/inputs/searches:\x01*Z\x18\"\x13/v2/inputs/searches:\x01*\x98\x9c\'\x02\x90\x9c\'&\x90\x9c\'\x0b\x90\x9c\'\x05\x90\x9c\'\x0f\x90\x9c\'\x03\x90\x9c\'\x13\x12\x9c\x03\n\x10PostModelOutputs\x12%.clarifai.api.PostModelOutputsRequest\x1a!.clarifai.api.MultiOutputResponse\"\xbd\x02\x82\xd3\xe4\x93\x02\xa6\x02\"i/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}/versions/{version_id}/outputs:\x01*Z8\"3/v2/models/{model_id}/versions/{version_id}/outputs:\x01*ZX\"S/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}/outputs:\x01*Z\"\"\x1d/v2/models/{model_id}/outputs:\x01*\x98\x9c\'\x02\x90\x9c\'\x0b\x90\x9c\'\x0f\x90\x9c\'\x02\x12\xbd\x01\n\x0cListDatasets\x12!.clarifai.api.ListDatasetsRequest\x1a\".clarifai.api.MultiDatasetResponse\"f\x82\xd3\xe4\x93\x02T\x12\x42/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/datasetsZ\x0e\x12\x0c/v2/datasets\x98\x9c\'\x02\x90\x9c\'i\x90\x9c\'r\x12\xd5\x01\n\nGetDataset\x12\x1f.clarifai.api.GetDatasetRequest\x1a#.clarifai.api.SingleDatasetResponse\"\x80\x01\x82\xd3\xe4\x93\x02n\x12O/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/datasets/{dataset_id}Z\x1b\x12\x19/v2/datasets/{dataset_id}\x98\x9c\'\x02\x90\x9c\'i\x90\x9c\'r\x12\xc7\x01\n\x0cPostDatasets\x12!.clarifai.api.PostDatasetsRequest\x1a\".clarifai.api.MultiDatasetResponse\"p\x82\xd3\xe4\x93\x02Z\"B/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/datasets:\x01*Z\x11\"\x0c/v2/datasets:\x01*\x98\x9c\'\x02\x90\x9c\'i\x90\x9c\'j\x90\x9c\'r\x12\xc9\x01\n\rPatchDatasets\x12\".clarifai.api.PatchDatasetsRequest\x1a\".clarifai.api.MultiDatasetResponse\"p\x82\xd3\xe4\x93\x02Z2B/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/datasets:\x01*Z\x11\x32\x0c/v2/datasets:\x01*\x98\x9c\'\x02\x90\x9c\'i\x90\x9c\'j\x90\x9c\'r\x12\xba\x01\n\x0fPatchDatasetIds\x12$.clarifai.api.PatchDatasetIdsRequest\x1a\".clarifai.api.MultiDatasetResponse\"]\x82\xd3\xe4\x93\x02K2F/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/datasets/ids:\x01*\x98\x9c\'\x02\x90\x9c\'i\x90\x9c\'j\x12\xca\x01\n\x0e\x44\x65leteDatasets\x12#.clarifai.api.DeleteDatasetsRequest\x1a!.clarifai.api.status.BaseResponse\"p\x82\xd3\xe4\x93\x02Z*B/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/datasets:\x01*Z\x11*\x0c/v2/datasets:\x01*\x98\x9c\'\x02\x90\x9c\'i\x90\x9c\'j\x90\x9c\'k\x12\xfd\x01\n\x11ListDatasetInputs\x12&.clarifai.api.ListDatasetInputsRequest\x1a\'.clarifai.api.MultiDatasetInputResponse\"\x96\x01\x82\xd3\xe4\x93\x02|\x12V/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/datasets/{dataset_id}/inputsZ\"\x12 /v2/datasets/{dataset_id}/inputs\x98\x9c\'\x02\x90\x9c\'i\x90\x9c\'\x05\x90\x9c\'&\x90\x9c\'\x0b\x12\x91\x02\n\x0fGetDatasetInput\x12$.clarifai.api.GetDatasetInputRequest\x1a(.clarifai.api.SingleDatasetInputResponse\"\xad\x01\x82\xd3\xe4\x93\x02\x92\x01\x12\x61/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/datasets/{dataset_id}/inputs/{input_id}Z-\x12+/v2/datasets/{dataset_id}/inputs/{input_id}\x98\x9c\'\x02\x90\x9c\'i\x90\x9c\'\x05\x90\x9c\'&\x90\x9c\'\x0b\x12\x88\x02\n\x11PostDatasetInputs\x12&.clarifai.api.PostDatasetInputsRequest\x1a\'.clarifai.api.MultiDatasetInputResponse\"\xa1\x01\x82\xd3\xe4\x93\x02\x82\x01\"V/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/datasets/{dataset_id}/inputs:\x01*Z%\" /v2/datasets/{dataset_id}/inputs:\x01*\x98\x9c\'\x02\x90\x9c\'i\x90\x9c\'j\x90\x9c\'\x05\x90\x9c\'&\x90\x9c\'\x0b\x12\x82\x02\n\x13\x44\x65leteDatasetInputs\x12(.clarifai.api.DeleteDatasetInputsRequest\x1a!.clarifai.api.status.BaseResponse\"\x9d\x01\x82\xd3\xe4\x93\x02\x82\x01*V/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/datasets/{dataset_id}/inputs:\x01*Z%* /v2/datasets/{dataset_id}/inputs:\x01*\x98\x9c\'\x02\x90\x9c\'i\x90\x9c\'j\x90\x9c\'k\x90\x9c\'\x05\x12\x80\x02\n\x13ListDatasetVersions\x12(.clarifai.api.ListDatasetVersionsRequest\x1a).clarifai.api.MultiDatasetVersionResponse\"\x93\x01\x82\xd3\xe4\x93\x02\x80\x01\x12X/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/datasets/{dataset_id}/versionsZ$\x12\"/v2/datasets/{dataset_id}/versions\x98\x9c\'\x02\x90\x9c\'i\x90\x9c\'r\x12\xa7\x02\n\x11GetDatasetVersion\x12&.clarifai.api.GetDatasetVersionRequest\x1a*.clarifai.api.SingleDatasetVersionResponse\"\xbd\x01\x82\xd3\xe4\x93\x02\xaa\x01\x12m/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/datasets/{dataset_id}/versions/{dataset_version_id}Z9\x12\x37/v2/datasets/{dataset_id}/versions/{dataset_version_id}\x98\x9c\'\x02\x90\x9c\'i\x90\x9c\'r\x12\xe6\x02\n\x1fListDatasetVersionMetricsGroups\x12\x34.clarifai.api.ListDatasetVersionMetricsGroupsRequest\x1a\x35.clarifai.api.MultiDatasetVersionMetricsGroupResponse\"\xd5\x01\x82\xd3\xe4\x93\x02\xba\x01\x12u/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/datasets/{dataset_id}/versions/{dataset_version_id}/metricsZA\x12?/v2/datasets/{dataset_id}/versions/{dataset_version_id}/metrics\x98\x9c\'\x02\x90\x9c\'i\x90\x9c\'&\x90\x9c\'\x0b\x90\x9c\'\x05\x12\x8e\x02\n\x13PostDatasetVersions\x12(.clarifai.api.PostDatasetVersionsRequest\x1a).clarifai.api.MultiDatasetVersionResponse\"\xa1\x01\x82\xd3\xe4\x93\x02\x86\x01\"X/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/datasets/{dataset_id}/versions:\x01*Z\'\"\"/v2/datasets/{dataset_id}/versions:\x01*\x98\x9c\'\x02\x90\x9c\'i\x90\x9c\'j\x90\x9c\'\x0f\x90\x9c\'\x13\x12\x88\x02\n\x14PatchDatasetVersions\x12).clarifai.api.PatchDatasetVersionsRequest\x1a).clarifai.api.MultiDatasetVersionResponse\"\x99\x01\x82\xd3\xe4\x93\x02\x86\x01\x32X/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/datasets/{dataset_id}/versions:\x01*Z\'2\"/v2/datasets/{dataset_id}/versions:\x01*\x98\x9c\'\x02\x90\x9c\'i\x90\x9c\'j\x12\x86\x02\n\x15\x44\x65leteDatasetVersions\x12*.clarifai.api.DeleteDatasetVersionsRequest\x1a!.clarifai.api.status.BaseResponse\"\x9d\x01\x82\xd3\xe4\x93\x02\x86\x01*X/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/datasets/{dataset_id}/versions:\x01*Z\'*\"/v2/datasets/{dataset_id}/versions:\x01*\x98\x9c\'\x02\x90\x9c\'i\x90\x9c\'j\x90\x9c\'k\x12\xd0\x02\n\x18PutDatasetVersionExports\x12-.clarifai.api.PutDatasetVersionExportsRequest\x1a/.clarifai.api.MultiDatasetVersionExportResponse\"\xd3\x01\x82\xd3\xe4\x93\x02\xc0\x01\x1au/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/datasets/{dataset_id}/versions/{dataset_version_id}/exports:\x01*ZD\x1a?/v2/datasets/{dataset_id}/versions/{dataset_version_id}/exports:\x01*\x98\x9c\'\x02\x90\x9c\'i\x90\x9c\'j\x12\xe5\x01\n\x0cGetModelType\x12!.clarifai.api.GetModelTypeRequest\x1a%.clarifai.api.SingleModelTypeResponse\"\x8a\x01\x82\xd3\xe4\x93\x02|\x12V/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/types/{model_type_id}Z\"\x12 /v2/models/types/{model_type_id}\x98\x9c\'\x02\x90\x9c\'\x0f\x12\x99\x01\n\x16ListOpenSourceLicenses\x12+.clarifai.api.ListOpenSourceLicensesRequest\x1a,.clarifai.api.ListOpenSourceLicensesResponse\"$\x82\xd3\xe4\x93\x02\x1a\x12\x18/v2/open_source_licenses\x98\x9c\'\x01\x12\xc7\x01\n\x0eListModelTypes\x12#.clarifai.api.ListModelTypesRequest\x1a$.clarifai.api.MultiModelTypeResponse\"j\x82\xd3\xe4\x93\x02\\\x12\x46/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/typesZ\x12\x12\x10/v2/models/types\x98\x9c\'\x02\x90\x9c\'\x0f\x12\xc6\x01\n\x08GetModel\x12\x1d.clarifai.api.GetModelRequest\x1a!.clarifai.api.SingleModelResponse\"x\x82\xd3\xe4\x93\x02\x66\x12K/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}Z\x17\x12\x15/v2/models/{model_id}\x98\x9c\'\x02\x90\x9c\'\x0b\x90\x9c\'\x0f\x12\x96\x03\n\x12GetModelOutputInfo\x12\x1d.clarifai.api.GetModelRequest\x1a!.clarifai.api.SingleModelResponse\"\xbd\x02\x82\xd3\xe4\x93\x02\xaa\x02\x12W/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}/output_infoZ#\x12!/v2/models/{model_id}/output_infoZo\x12m/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}/versions/{version_id}/output_infoZ9\x12\x37/v2/models/{model_id}/versions/{version_id}/output_info\x98\x9c\'\x02\x90\x9c\'\x0b\x90\x9c\'\x0f\x12\xde\x01\n\nListModels\x12\x1f.clarifai.api.ListModelsRequest\x1a .clarifai.api.MultiModelResponse\"\x8c\x01\x82\xd3\xe4\x93\x02z\x12@/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/modelsZ(\x12&/v2/users/{user_app_id.user_id}/modelsZ\x0c\x12\n/v2/models\x98\x9c\'\x02\x90\x9c\'\x0b\x90\x9c\'\x0f\x12\xdb\x01\n\x12PostModelsSearches\x12\'.clarifai.api.PostModelsSearchesRequest\x1a .clarifai.api.MultiModelResponse\"z\x82\xd3\xe4\x93\x02h\"I/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/searches:\x01*Z\x18\"\x13/v2/models/searches:\x01*\x98\x9c\'\x02\x90\x9c\'\x0b\x90\x9c\'\x0f\x12\xc6\x01\n\nPostModels\x12\x1f.clarifai.api.PostModelsRequest\x1a!.clarifai.api.SingleModelResponse\"t\x82\xd3\xe4\x93\x02V\"@/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models:\x01*Z\x0f\"\n/v2/models:\x01*\x98\x9c\'\x02\x90\x9c\'\x0b\x90\x9c\'\x0e\x90\x9c\'\x0f\x90\x9c\'\x1a\x90\x9c\'\x13\x12\xc3\x01\n\x0bPatchModels\x12 .clarifai.api.PatchModelsRequest\x1a .clarifai.api.MultiModelResponse\"p\x82\xd3\xe4\x93\x02V2@/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models:\x01*Z\x0f\x32\n/v2/models:\x01*\x98\x9c\'\x02\x90\x9c\'\x0b\x90\x9c\'\x0e\x90\x9c\'\x0f\x90\x9c\'\x1a\x12\xb2\x01\n\rPatchModelIds\x12\".clarifai.api.PatchModelIdsRequest\x1a .clarifai.api.MultiModelResponse\"[\x82\xd3\xe4\x93\x02I2D/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/ids:\x01*\x98\x9c\'\x02\x90\x9c\'\x0e\x90\x9c\'\x0f\x12\xd9\x01\n\x0b\x44\x65leteModel\x12 .clarifai.api.DeleteModelRequest\x1a!.clarifai.api.status.BaseResponse\"\x84\x01\x82\xd3\xe4\x93\x02\x66*K/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}Z\x17*\x15/v2/models/{model_id}\x98\x9c\'\x02\x90\x9c\'\x0b\x90\x9c\'\x0e\x90\x9c\'\x11\x90\x9c\'\x0f\x90\x9c\'\x13\x12\xca\x01\n\x0c\x44\x65leteModels\x12!.clarifai.api.DeleteModelsRequest\x1a!.clarifai.api.status.BaseResponse\"t\x82\xd3\xe4\x93\x02V*@/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models:\x01*Z\x0f*\n/v2/models:\x01*\x98\x9c\'\x02\x90\x9c\'\x0b\x90\x9c\'\x0e\x90\x9c\'\x11\x90\x9c\'\x0f\x90\x9c\'\x13\x12\x91\x02\n\x17PatchModelCheckConsents\x12,.clarifai.api.PatchModelCheckConsentsRequest\x1a,.clarifai.api.MultiModelCheckConsentResponse\"\x99\x01\x82\xd3\xe4\x93\x02\x8a\x01\x32Z/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}/check_consents:\x01*Z)2$/v2/models/{model_id}/check_consents:\x01*\x98\x9c\'\x02\x90\x9c\'\x0f\x12\xf5\x01\n\x12PatchModelToolkits\x12\'.clarifai.api.PatchModelToolkitsRequest\x1a\'.clarifai.api.MultiModelToolkitResponse\"\x8c\x01\x82\xd3\xe4\x93\x02~2T/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}/toolkits:\x01*Z#2\x1e/v2/models/{model_id}/toolkits:\x01*\x98\x9c\'\x02\x90\x9c\'\x0f\x12\xf5\x01\n\x12PatchModelUseCases\x12\'.clarifai.api.PatchModelUseCasesRequest\x1a\'.clarifai.api.MultiModelUseCaseResponse\"\x8c\x01\x82\xd3\xe4\x93\x02~2T/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}/usecases:\x01*Z#2\x1e/v2/models/{model_id}/usecases:\x01*\x98\x9c\'\x02\x90\x9c\'\x0f\x12\xfb\x01\n\x13PatchModelLanguages\x12(.clarifai.api.PatchModelLanguagesRequest\x1a(.clarifai.api.MultiModelLanguageResponse\"\x8f\x01\x82\xd3\xe4\x93\x02\x80\x01\x32U/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}/languages:\x01*Z$2\x1f/v2/models/{model_id}/languages:\x01*\x98\x9c\'\x02\x90\x9c\'\x0f\x12\x8d\x03\n\x0fListModelInputs\x12$.clarifai.api.ListModelInputsRequest\x1a .clarifai.api.MultiInputResponse\"\xb1\x02\x82\xd3\xe4\x93\x02\x96\x02\x12R/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}/inputsZ\x1e\x12\x1c/v2/models/{model_id}/inputsZj\x12h/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}/versions/{version_id}/inputsZ4\x12\x32/v2/models/{model_id}/versions/{version_id}/inputs\x98\x9c\'\x02\x90\x9c\'&\x90\x9c\'\x0b\x90\x9c\'\x05\x90\x9c\'\x0f\x12\x89\x02\n\x0fGetModelVersion\x12$.clarifai.api.GetModelVersionRequest\x1a(.clarifai.api.SingleModelVersionResponse\"\xa5\x01\x82\xd3\xe4\x93\x02\x92\x01\x12\x61/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}/versions/{version_id}Z-\x12+/v2/models/{model_id}/versions/{version_id}\x98\x9c\'\x02\x90\x9c\'\x0b\x90\x9c\'\x0f\x12\xf1\x01\n\x11ListModelVersions\x12&.clarifai.api.ListModelVersionsRequest\x1a\'.clarifai.api.MultiModelVersionResponse\"\x8a\x01\x82\xd3\xe4\x93\x02x\x12T/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}/versionsZ \x12\x1e/v2/models/{model_id}/versions\x98\x9c\'\x02\x90\x9c\'\x0b\x90\x9c\'\x0f\x12\xb8\x02\n\x1dPostWorkflowVersionsUnPublish\x12\x32.clarifai.api.PostWorkflowVersionsUnPublishRequest\x1a!.clarifai.api.status.BaseResponse\"\xbf\x01\x82\xd3\xe4\x93\x02\x8c\x01\"[/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/workflows/{workflow_id}/unpublish:\x01*Z*\"%/v2/workflows/{workflow_id}/unpublish:\x01*\x98\x9c\'\x02\x90\x9c\'x\x90\x9c\'&\x90\x9c\'\x0b\x90\x9c\'\x05\x90\x9c\'\x0e\x90\x9c\'\x0f\x90\x9c\'\x1a\x90\x9c\'\x13\x90\x9c\'5\x90\x9c\'6\x12\xb0\x02\n\x1bPostWorkflowVersionsPublish\x12\x30.clarifai.api.PostWorkflowVersionsPublishRequest\x1a!.clarifai.api.status.BaseResponse\"\xbb\x01\x82\xd3\xe4\x93\x02\x88\x01\"Y/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/workflows/{workflow_id}/publish:\x01*Z(\"#/v2/workflows/{workflow_id}/publish:\x01*\x98\x9c\'\x02\x90\x9c\'w\x90\x9c\'&\x90\x9c\'\x0b\x90\x9c\'\x05\x90\x9c\'\x0e\x90\x9c\'\x0f\x90\x9c\'\x1a\x90\x9c\'\x13\x90\x9c\'5\x90\x9c\'6\x12\x9d\x02\n\x18PostModelVersionsPublish\x12-.clarifai.api.PostModelVersionsPublishRequest\x1a!.clarifai.api.status.BaseResponse\"\xae\x01\x82\xd3\xe4\x93\x02|\"S/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}/publish:\x01*Z\"\"\x1d/v2/models/{model_id}/publish:\x01*\x98\x9c\'\x02\x90\x9c\'u\x90\x9c\'&\x90\x9c\'\x0b\x90\x9c\'\x05\x90\x9c\'\x0e\x90\x9c\'\x0f\x90\x9c\'\x1a\x90\x9c\'\x13\x90\x9c\'5\x90\x9c\'6\x12\xa6\x02\n\x1aPostModelVersionsUnPublish\x12/.clarifai.api.PostModelVersionsUnPublishRequest\x1a!.clarifai.api.status.BaseResponse\"\xb3\x01\x82\xd3\xe4\x93\x02\x80\x01\"U/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}/unpublish:\x01*Z$\"\x1f/v2/models/{model_id}/unpublish:\x01*\x98\x9c\'\x02\x90\x9c\'v\x90\x9c\'&\x90\x9c\'\x0b\x90\x9c\'\x05\x90\x9c\'\x0e\x90\x9c\'\x0f\x90\x9c\'\x1a\x90\x9c\'\x13\x90\x9c\'5\x90\x9c\'6\x12\x8d\x02\n\x11PostModelVersions\x12&.clarifai.api.PostModelVersionsRequest\x1a!.clarifai.api.SingleModelResponse\"\xac\x01\x82\xd3\xe4\x93\x02~\"T/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}/versions:\x01*Z#\"\x1e/v2/models/{model_id}/versions:\x01*\x98\x9c\'\x02\x90\x9c\'&\x90\x9c\'\x0b\x90\x9c\'\x05\x90\x9c\'\x0e\x90\x9c\'\x0f\x90\x9c\'\x1a\x90\x9c\'\x13\x90\x9c\'5\x90\x9c\'6\x12\xdb\x01\n\x12PatchModelVersions\x12\'.clarifai.api.PatchModelVersionsRequest\x1a\'.clarifai.api.MultiModelVersionResponse\"s\x82\xd3\xe4\x93\x02Y2T/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}/versions:\x01*\x98\x9c\'\x02\x90\x9c\'\x0b\x90\x9c\'\x0f\x90\x9c\'\x0e\x90\x9c\'\x1a\x12\x94\x02\n\x12\x44\x65leteModelVersion\x12\'.clarifai.api.DeleteModelVersionRequest\x1a!.clarifai.api.status.BaseResponse\"\xb1\x01\x82\xd3\xe4\x93\x02\x92\x01*a/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}/versions/{version_id}Z-*+/v2/models/{model_id}/versions/{version_id}\x98\x9c\'\x02\x90\x9c\'\x0b\x90\x9c\'\x0e\x90\x9c\'\x11\x90\x9c\'\x0f\x90\x9c\'\x13\x12\xb3\x02\n\x16GetModelVersionMetrics\x12+.clarifai.api.GetModelVersionMetricsRequest\x1a(.clarifai.api.SingleModelVersionResponse\"\xc1\x01\x82\xd3\xe4\x93\x02\xa2\x01\x12i/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}/versions/{version_id}/metricsZ5\x12\x33/v2/models/{model_id}/versions/{version_id}/metrics\x98\x9c\'\x02\x90\x9c\'&\x90\x9c\'\x0b\x90\x9c\'\x0f\x90\x9c\'\x05\x90\x9c\'5\x12\xcf\x02\n\x17PostModelVersionMetrics\x12,.clarifai.api.PostModelVersionMetricsRequest\x1a(.clarifai.api.SingleModelVersionResponse\"\xdb\x01\x82\xd3\xe4\x93\x02\xa8\x01\"i/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}/versions/{version_id}/metrics:\x01*Z8\"3/v2/models/{model_id}/versions/{version_id}/metrics:\x01*\x98\x9c\'\x02\x90\x9c\'&\x90\x9c\'\x0b\x90\x9c\'\x05\x90\x9c\'\x0e\x90\x9c\'\x0f\x90\x9c\'\x1a\x90\x9c\'\x02\x90\x9c\'\x13\x90\x9c\'5\x90\x9c\'6\x12\xe9\x02\n\x1bPostModelVersionEvaluations\x12\x30.clarifai.api.PostModelVersionEvaluationsRequest\x1a&.clarifai.api.MultiEvalMetricsResponse\"\xef\x01\x82\xd3\xe4\x93\x02\xbc\x01\"s/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}/versions/{model_version_id}/evaluations:\x01*ZB\"=/v2/models/{model_id}/versions/{model_version_id}/evaluations:\x01*\x98\x9c\'\x02\x90\x9c\'&\x90\x9c\'\x0b\x90\x9c\'\x05\x90\x9c\'\x0e\x90\x9c\'\x0f\x90\x9c\'\x1a\x90\x9c\'\x02\x90\x9c\'\x13\x90\x9c\'5\x90\x9c\'6\x12\xcf\x02\n\x1bListModelVersionEvaluations\x12\x30.clarifai.api.ListModelVersionEvaluationsRequest\x1a&.clarifai.api.MultiEvalMetricsResponse\"\xd5\x01\x82\xd3\xe4\x93\x02\xb6\x01\x12s/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}/versions/{model_version_id}/evaluationsZ?\x12=/v2/models/{model_id}/versions/{model_version_id}/evaluations\x98\x9c\'\x02\x90\x9c\'&\x90\x9c\'\x0b\x90\x9c\'\x0f\x90\x9c\'\x05\x90\x9c\'5\x12\xed\x02\n\x19GetModelVersionEvaluation\x12..clarifai.api.GetModelVersionEvaluationRequest\x1a\'.clarifai.api.SingleEvalMetricsResponse\"\xf6\x01\x82\xd3\xe4\x93\x02\xd7\x01\x12\x83\x01/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}/versions/{model_version_id}/evaluations/{evaluation_id}ZO\x12M/v2/models/{model_id}/versions/{model_version_id}/evaluations/{evaluation_id}\x98\x9c\'\x02\x90\x9c\'&\x90\x9c\'\x0b\x90\x9c\'\x0f\x90\x9c\'\x05\x90\x9c\'5\x12\xf7\x01\n\x13ListModelReferences\x12(.clarifai.api.ListModelReferencesRequest\x1a).clarifai.api.MultiModelReferenceResponse\"\x8a\x01\x82\xd3\xe4\x93\x02|\x12V/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}/referencesZ\"\x12 /v2/models/{model_id}/references\x98\x9c\'\x02\x90\x9c\'\x0f\x12\xee\x02\n\x1bGetModelVersionInputExample\x12\x30.clarifai.api.GetModelVersionInputExampleRequest\x1a\x34.clarifai.api.SingleModelVersionInputExampleResponse\"\xe6\x01\x82\xd3\xe4\x93\x02\xd7\x01\x12\x83\x01/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}/versions/{model_version_id}/input_examples/{example_id}ZO\x12M/v2/models/{model_id}/versions/{model_version_id}/input_examples/{example_id}\x98\x9c\'\x02\x90\x9c\'\x0f\x12\xd6\x02\n\x1dListModelVersionInputExamples\x12\x32.clarifai.api.ListModelVersionInputExamplesRequest\x1a\x33.clarifai.api.MultiModelVersionInputExampleResponse\"\xcb\x01\x82\xd3\xe4\x93\x02\xbc\x01\x12v/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}/versions/{model_version_id}/input_examplesZB\x12@/v2/models/{model_id}/versions/{model_version_id}/input_examples\x98\x9c\'\x02\x90\x9c\'\x0f\x12\xdc\x01\n\x0bGetWorkflow\x12 .clarifai.api.GetWorkflowRequest\x1a$.clarifai.api.SingleWorkflowResponse\"\x84\x01\x82\xd3\xe4\x93\x02r\x12Q/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/workflows/{workflow_id}Z\x1d\x12\x1b/v2/workflows/{workflow_id}\x98\x9c\'\x02\x90\x9c\'\x0f\x90\x9c\'\x13\x12\xf1\x01\n\rListWorkflows\x12\".clarifai.api.ListWorkflowsRequest\x1a#.clarifai.api.MultiWorkflowResponse\"\x96\x01\x82\xd3\xe4\x93\x02\x83\x01\x12\x43/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/workflowsZ+\x12)/v2/users/{user_app_id.user_id}/workflowsZ\x0f\x12\r/v2/workflows\x98\x9c\'\x02\x90\x9c\'\x0f\x90\x9c\'\x13\x12\xcc\x01\n\rPostWorkflows\x12\".clarifai.api.PostWorkflowsRequest\x1a#.clarifai.api.MultiWorkflowResponse\"r\x82\xd3\xe4\x93\x02\\\"C/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/workflows:\x01*Z\x12\"\r/v2/workflows:\x01*\x98\x9c\'\x02\x90\x9c\'\x0f\x90\x9c\'\x12\x90\x9c\'\x13\x12\xce\x01\n\x0ePatchWorkflows\x12#.clarifai.api.PatchWorkflowsRequest\x1a#.clarifai.api.MultiWorkflowResponse\"r\x82\xd3\xe4\x93\x02\\2C/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/workflows:\x01*Z\x12\x32\r/v2/workflows:\x01*\x98\x9c\'\x02\x90\x9c\'\x0f\x90\x9c\'\x12\x90\x9c\'\x13\x12\xbe\x01\n\x10PatchWorkflowIds\x12%.clarifai.api.PatchWorkflowIdsRequest\x1a#.clarifai.api.MultiWorkflowResponse\"^\x82\xd3\xe4\x93\x02L2G/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/workflows/ids:\x01*\x98\x9c\'\x02\x90\x9c\'\x12\x90\x9c\'\x13\x12\xe3\x01\n\x0e\x44\x65leteWorkflow\x12#.clarifai.api.DeleteWorkflowRequest\x1a!.clarifai.api.status.BaseResponse\"\x88\x01\x82\xd3\xe4\x93\x02r*Q/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/workflows/{workflow_id}Z\x1d*\x1b/v2/workflows/{workflow_id}\x98\x9c\'\x02\x90\x9c\'\x12\x90\x9c\'\x15\x90\x9c\'\x13\x12\xce\x01\n\x0f\x44\x65leteWorkflows\x12$.clarifai.api.DeleteWorkflowsRequest\x1a!.clarifai.api.status.BaseResponse\"r\x82\xd3\xe4\x93\x02\\*C/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/workflows:\x01*Z\x12*\r/v2/workflows:\x01*\x98\x9c\'\x02\x90\x9c\'\x12\x90\x9c\'\x15\x90\x9c\'\x13\x12\x86\x03\n\x13PostWorkflowResults\x12(.clarifai.api.PostWorkflowResultsRequest\x1a).clarifai.api.PostWorkflowResultsResponse\"\x99\x02\x82\xd3\xe4\x93\x02\xfe\x01\"o/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/workflows/{workflow_id}/versions/{version_id}/results:\x01*Z^\"Y/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/workflows/{workflow_id}/results:\x01*Z(\"#/v2/workflows/{workflow_id}/results:\x01*\x98\x9c\'\x02\x90\x9c\'\x0f\x90\x9c\'\x0b\x90\x9c\'\x02\x90\x9c\'\x13\x12\xc5\x03\n\x1dPostWorkflowResultsSimilarity\x12\x32.clarifai.api.PostWorkflowResultsSimilarityRequest\x1a\x33.clarifai.api.PostWorkflowResultsSimilarityResponse\"\xba\x02\x82\xd3\xe4\x93\x02\x9f\x02\"z/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/workflows/{workflow_id}/versions/{version_id}/results/similarity:\x01*Zi\"d/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/workflows/{workflow_id}/results/similarity:\x01*Z3\"./v2/workflows/{workflow_id}/results/similarity:\x01*\x98\x9c\'\x02\x90\x9c\'\x0f\x90\x9c\'\x0b\x90\x9c\'\x02\x90\x9c\'\x13\x12\x87\x02\n\x14ListWorkflowVersions\x12).clarifai.api.ListWorkflowVersionsRequest\x1a*.clarifai.api.MultiWorkflowVersionResponse\"\x97\x01\x82\xd3\xe4\x93\x02\x84\x01\x12Z/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/workflows/{workflow_id}/versionsZ&\x12$/v2/workflows/{workflow_id}/versions\x98\x9c\'\x02\x90\x9c\'\x0f\x90\x9c\'\x13\x12\xb0\x02\n\x12GetWorkflowVersion\x12\'.clarifai.api.GetWorkflowVersionRequest\x1a+.clarifai.api.SingleWorkflowVersionResponse\"\xc3\x01\x82\xd3\xe4\x93\x02\xb0\x01\x12p/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/workflows/{workflow_id}/versions/{workflow_version_id}Z<\x12:/v2/workflows/{workflow_id}/versions/{workflow_version_id}\x98\x9c\'\x02\x90\x9c\'\x0f\x90\x9c\'\x13\x12\x8c\x02\n\x16\x44\x65leteWorkflowVersions\x12+.clarifai.api.DeleteWorkflowVersionsRequest\x1a!.clarifai.api.status.BaseResponse\"\xa1\x01\x82\xd3\xe4\x93\x02\x8a\x01*Z/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/workflows/{workflow_id}/versions:\x01*Z)*$/v2/workflows/{workflow_id}/versions:\x01*\x98\x9c\'\x02\x90\x9c\'\x13\x90\x9c\'\x12\x90\x9c\'\x15\x12\x93\x02\n\x15PatchWorkflowVersions\x12*.clarifai.api.PatchWorkflowVersionsRequest\x1a*.clarifai.api.MultiWorkflowVersionResponse\"\xa1\x01\x82\xd3\xe4\x93\x02\x8a\x01\x32Z/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/workflows/{workflow_id}/versions:\x01*Z)2$/v2/workflows/{workflow_id}/versions:\x01*\x98\x9c\'\x02\x90\x9c\'\x0f\x90\x9c\'\x13\x90\x9c\'\x12\x12\x85\x01\n\x06GetKey\x12\x1b.clarifai.api.GetKeyRequest\x1a\x1f.clarifai.api.SingleKeyResponse\"=\x82\xd3\xe4\x93\x02/\x12-/v2/users/{user_app_id.user_id}/keys/{key_id}\x98\x9c\'\x05\x90\x9c\'0\x12\x7f\n\x08ListKeys\x12\x1d.clarifai.api.ListKeysRequest\x1a\x1e.clarifai.api.MultiKeyResponse\"4\x82\xd3\xe4\x93\x02&\x12$/v2/users/{user_app_id.user_id}/keys\x98\x9c\'\x05\x90\x9c\'0\x12\x9f\x01\n\x0bListAppKeys\x12 .clarifai.api.ListAppKeysRequest\x1a\x1e.clarifai.api.MultiKeyResponse\"N\x82\xd3\xe4\x93\x02@\x12>/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/keys\x98\x9c\'\x05\x90\x9c\'0\x12\x95\x01\n\tDeleteKey\x12\x1e.clarifai.api.DeleteKeyRequest\x1a!.clarifai.api.status.BaseResponse\"E\x82\xd3\xe4\x93\x02/*-/v2/users/{user_app_id.user_id}/keys/{key_id}\x98\x9c\'\x05\x90\x9c\'/\x90\x9c\'1\x90\x9c\'0\x12\x8a\x01\n\x08PostKeys\x12\x1d.clarifai.api.PostKeysRequest\x1a\x1e.clarifai.api.MultiKeyResponse\"?\x82\xd3\xe4\x93\x02)\"$/v2/users/{user_app_id.user_id}/keys:\x01*\x98\x9c\'\x05\x90\x9c\'-\x90\x9c\'/\x90\x9c\'0\x12\x88\x01\n\tPatchKeys\x12\x1e.clarifai.api.PatchKeysRequest\x1a\x1e.clarifai.api.MultiKeyResponse\";\x82\xd3\xe4\x93\x02)2$/v2/users/{user_app_id.user_id}/keys:\x01*\x98\x9c\'\x05\x90\x9c\'/\x90\x9c\'0\x12\xbc\x01\n\x08MyScopes\x12\x1d.clarifai.api.MyScopesRequest\x1a .clarifai.api.MultiScopeResponse\"o\x82\xd3\xe4\x93\x02\x65\x12\x42/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/myscopesZ\x0e\x12\x0c/v2/myscopesZ\x0f\x12\r/v2/my_scopes\x98\x9c\'\x02\x12\x8d\x01\n\x0cMyScopesUser\x12!.clarifai.api.MyScopesUserRequest\x1a$.clarifai.api.MultiScopeUserResponse\"4\x82\xd3\xe4\x93\x02*\x12(/v2/users/{user_app_id.user_id}/myscopes\x98\x9c\'\x05\x12u\n\x0cMyScopesRoot\x12!.clarifai.api.MyScopesRootRequest\x1a$.clarifai.api.MultiScopeRootResponse\"\x1c\x82\xd3\xe4\x93\x02\x12\x12\x10/v2/myscopesroot\x98\x9c\'\x05\x12\x87\x01\n\nListScopes\x12\x1f.clarifai.api.ListScopesRequest\x1a$.clarifai.api.MultiScopeDepsResponse\"2\x82\xd3\xe4\x93\x02(\x12&/v2/users/{user_app_id.user_id}/scopes\x98\x9c\'\x03\x12\x95\x01\n\x06GetApp\x12\x1b.clarifai.api.GetAppRequest\x1a\x1f.clarifai.api.SingleAppResponse\"M\x82\xd3\xe4\x93\x02;\x12\x39/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}\x98\x9c\'\x05\x90\x9c\'-\x90\x9c\'\x13\x12\x8f\x01\n\x08ListApps\x12\x1d.clarifai.api.ListAppsRequest\x1a\x1e.clarifai.api.MultiAppResponse\"D\x82\xd3\xe4\x93\x02\x32\x12$/v2/users/{user_app_id.user_id}/appsZ\n\x12\x08/v2/apps\x98\x9c\'\x05\x90\x9c\'-\x90\x9c\'\x13\x12\xa5\x01\n\tDeleteApp\x12\x1e.clarifai.api.DeleteAppRequest\x1a!.clarifai.api.status.BaseResponse\"U\x82\xd3\xe4\x93\x02;*9/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}\x98\x9c\'\x05\x90\x9c\',\x90\x9c\'.\x90\x9c\'-\x90\x9c\'\x13\x12\x92\x01\n\x08PostApps\x12\x1d.clarifai.api.PostAppsRequest\x1a\x1e.clarifai.api.MultiAppResponse\"G\x82\xd3\xe4\x93\x02)\"$/v2/users/{user_app_id.user_id}/apps:\x01*\x98\x9c\'\x05\x90\x9c\',\x90\x9c\'-\x90\x9c\'\x0f\x90\x9c\'\x13\x90\x9c\'\x12\x12\x88\x01\n\tPatchApps\x12\x1e.clarifai.api.PatchAppsRequest\x1a\x1e.clarifai.api.MultiAppResponse\";\x82\xd3\xe4\x93\x02)2$/v2/users/{user_app_id.user_id}/apps:\x01*\x98\x9c\'\x05\x90\x9c\',\x90\x9c\'-\x12\x92\x01\n\x0cPatchAppsIds\x12!.clarifai.api.PatchAppsIdsRequest\x1a\x1e.clarifai.api.MultiAppResponse\"?\x82\xd3\xe4\x93\x02-2(/v2/users/{user_app_id.user_id}/apps/ids:\x01*\x98\x9c\'\x05\x90\x9c\',\x90\x9c\'-\x12\x9c\x01\n\x08PatchApp\x12\x1d.clarifai.api.PatchAppRequest\x1a\x1f.clarifai.api.SingleAppResponse\"P\x82\xd3\xe4\x93\x02>29/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}:\x01*\x98\x9c\'\x05\x90\x9c\',\x90\x9c\'-\x12\x9f\x01\n\x10PostAppsSearches\x12%.clarifai.api.PostAppsSearchesRequest\x1a\x1e.clarifai.api.MultiAppResponse\"D\x82\xd3\xe4\x93\x02\x32\"-/v2/users/{user_app_id.user_id}/apps/searches:\x01*\x98\x9c\'\x05\x90\x9c\'-\x90\x9c\'\x13\x12v\n\x07GetUser\x12\x1c.clarifai.api.GetUserRequest\x1a .clarifai.api.SingleUserResponse\"+\x82\xd3\xe4\x93\x02!\x12\x1f/v2/users/{user_app_id.user_id}\x98\x9c\'\x05\x12\xcf\x01\n\x14PostValidatePassword\x12).clarifai.api.PostValidatePasswordRequest\x1a..clarifai.api.SinglePasswordValidationResponse\"\\\x82\xd3\xe4\x93\x02R\"1/v2/users/{user_app_id.user_id}/validate_password:\x01*Z\x1a\"\x15/v2/validate_password:\x01*\x98\x9c\'\x03\x12\xbd\x01\n\tGetSearch\x12\x1e.clarifai.api.GetSearchRequest\x1a\".clarifai.api.SingleSearchResponse\"l\x82\xd3\xe4\x93\x02^\x12G/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/searches/{id}Z\x13\x12\x11/v2/searches/{id}\x98\x9c\'\x02\x90\x9c\'r\x12\xb8\x01\n\x0cListSearches\x12!.clarifai.api.ListSearchesRequest\x1a!.clarifai.api.MultiSearchResponse\"b\x82\xd3\xe4\x93\x02T\x12\x42/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/searchesZ\x0e\x12\x0c/v2/searches\x98\x9c\'\x02\x90\x9c\'r\x12\xc4\x01\n\rPatchSearches\x12\".clarifai.api.PatchSearchesRequest\x1a!.clarifai.api.MultiSearchResponse\"l\x82\xd3\xe4\x93\x02Z2B/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/searches:\x01*Z\x11\x32\x0c/v2/searches:\x01*\x98\x9c\'\x02\x90\x9c\'s\x90\x9c\'r\x12\xd5\x01\n\x0cPostSearches\x12!.clarifai.api.PostSearchesRequest\x1a!.clarifai.api.MultiSearchResponse\"\x7f\x88\x02\x01\x82\xd3\xe4\x93\x02Z\"B/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/searches:\x01*Z\x11\"\x0c/v2/searches:\x01*\x98\x9c\'\x02\x90\x9c\'&\x90\x9c\'\x0b\x90\x9c\'\x05\x90\x9c\'\x0f\x90\x9c\'\x03\x90\x9c\'\x13\x12\xd4\x01\n\x10PostSearchesByID\x12%.clarifai.api.PostSearchesByIDRequest\x1a!.clarifai.api.MultiSearchResponse\"v\x82\xd3\xe4\x93\x02\x64\"G/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/searches/{id}:\x01*Z\x16\"\x11/v2/searches/{id}:\x01*\x98\x9c\'\x02\x90\x9c\'r\x90\x9c\'\x03\x12\xaf\x02\n\x1bPostAnnotationSearchMetrics\x12\x30.clarifai.api.PostAnnotationSearchMetricsRequest\x1a\x32.clarifai.api.MultiAnnotationSearchMetricsResponse\"\xa9\x01\x82\xd3\xe4\x93\x02\x82\x01\"V/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/annotations/searches/metrics:\x01*Z%\" /v2/annotations/searches/metrics:\x01*\x98\x9c\'\x02\x90\x9c\'&\x90\x9c\'\x0b\x90\x9c\'\x05\x90\x9c\'5\x90\x9c\'6\x90\x9c\'\x0f\x90\x9c\'\x13\x12\xa5\x02\n\x1aGetAnnotationSearchMetrics\x12/.clarifai.api.GetAnnotationSearchMetricsRequest\x1a\x32.clarifai.api.MultiAnnotationSearchMetricsResponse\"\xa1\x01\x82\xd3\xe4\x93\x02\x86\x01\x12[/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/annotations/searches/metrics/{id}Z\'\x12%/v2/annotations/searches/metrics/{id}\x98\x9c\'\x02\x90\x9c\'&\x90\x9c\'\x0b\x90\x9c\'\x05\x90\x9c\'5\x12\x9c\x02\n\x1bListAnnotationSearchMetrics\x12\x30.clarifai.api.ListAnnotationSearchMetricsRequest\x1a\x32.clarifai.api.MultiAnnotationSearchMetricsResponse\"\x96\x01\x82\xd3\xe4\x93\x02|\x12V/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/annotations/searches/metricsZ\"\x12 /v2/annotations/searches/metrics\x98\x9c\'\x02\x90\x9c\'&\x90\x9c\'\x0b\x90\x9c\'\x05\x90\x9c\'5\x12\x96\x02\n\x1d\x44\x65leteAnnotationSearchMetrics\x12\x32.clarifai.api.DeleteAnnotationSearchMetricsRequest\x1a!.clarifai.api.status.BaseResponse\"\x9d\x01\x82\xd3\xe4\x93\x02\x86\x01*[/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/annotations/searches/metrics/{id}Z\'*%/v2/annotations/searches/metrics/{id}\x98\x9c\'\x02\x90\x9c\'5\x90\x9c\'6\x90\x9c\'?\x12\xca\x01\n\x0c\x44\x65leteSearch\x12!.clarifai.api.DeleteSearchRequest\x1a!.clarifai.api.status.BaseResponse\"t\x82\xd3\xe4\x93\x02^*G/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/searches/{id}Z\x13*\x11/v2/searches/{id}\x98\x9c\'\x02\x90\x9c\'r\x90\x9c\'s\x90\x9c\'t\x12\xe8\x01\n\x15ListAnnotationFilters\x12*.clarifai.api.ListAnnotationFiltersRequest\x1a+.clarifai.api.MultiAnnotationFilterResponse\"v\x82\xd3\xe4\x93\x02h\x12L/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/annotation_filtersZ\x18\x12\x16/v2/annotation_filters\x98\x9c\'\x02\x90\x9c\'r\x12\x95\x02\n\x13GetAnnotationFilter\x12(.clarifai.api.GetAnnotationFilterRequest\x1a,.clarifai.api.SingleAnnotationFilterResponse\"\xa5\x01\x82\xd3\xe4\x93\x02\x96\x01\x12\x63/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/annotation_filters/{annotation_filter_id}Z/\x12-/v2/annotation_filters/{annotation_filter_id}\x98\x9c\'\x02\x90\x9c\'r\x12\xf3\x01\n\x15PostAnnotationFilters\x12*.clarifai.api.PostAnnotationFiltersRequest\x1a+.clarifai.api.MultiAnnotationFilterResponse\"\x80\x01\x82\xd3\xe4\x93\x02n\"L/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/annotation_filters:\x01*Z\x1b\"\x16/v2/annotation_filters:\x01*\x98\x9c\'\x02\x90\x9c\'r\x90\x9c\'s\x12\xf5\x01\n\x16PatchAnnotationFilters\x12+.clarifai.api.PatchAnnotationFiltersRequest\x1a+.clarifai.api.MultiAnnotationFilterResponse\"\x80\x01\x82\xd3\xe4\x93\x02n2L/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/annotation_filters:\x01*Z\x1b\x32\x16/v2/annotation_filters:\x01*\x98\x9c\'\x02\x90\x9c\'r\x90\x9c\'s\x12\xed\x01\n\x17\x44\x65leteAnnotationFilters\x12,.clarifai.api.DeleteAnnotationFiltersRequest\x1a!.clarifai.api.status.BaseResponse\"\x80\x01\x82\xd3\xe4\x93\x02n*L/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/annotation_filters:\x01*Z\x1b*\x16/v2/annotation_filters:\x01*\x98\x9c\'\x02\x90\x9c\'r\x90\x9c\'s\x12|\n\x0fListStatusCodes\x12$.clarifai.api.ListStatusCodesRequest\x1a%.clarifai.api.MultiStatusCodeResponse\"\x1c\x82\xd3\xe4\x93\x02\x12\x12\x10/v2/status_codes\x98\x9c\'\x01\x12\x8a\x01\n\rGetStatusCode\x12\".clarifai.api.GetStatusCodeRequest\x1a&.clarifai.api.SingleStatusCodeResponse\"-\x82\xd3\xe4\x93\x02#\x12!/v2/status_codes/{status_code_id}\x98\x9c\'\x01\x12\xbe\x01\n\x11ListCollaborators\x12&.clarifai.api.ListCollaboratorsRequest\x1a(.clarifai.api.MultiCollaboratorsResponse\"W\x82\xd3\xe4\x93\x02I\x12G/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/collaborators\x98\x9c\'\x02\x90\x9c\'2\x12\xc5\x01\n\x11PostCollaborators\x12&.clarifai.api.PostCollaboratorsRequest\x1a(.clarifai.api.MultiCollaboratorsResponse\"^\x82\xd3\xe4\x93\x02L\"G/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/collaborators:\x01*\x98\x9c\'\x02\x90\x9c\'3\x90\x9c\'2\x12\xcb\x01\n\x12PatchCollaborators\x12\'.clarifai.api.PatchCollaboratorsRequest\x1a(.clarifai.api.MultiCollaboratorsResponse\"b\x82\xd3\xe4\x93\x02L2G/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/collaborators:\x01*\x98\x9c\'\x02\x90\x9c\'3\x90\x9c\'2\x90\x9c\'4\x12\xce\x01\n\x13\x44\x65leteCollaborators\x12(.clarifai.api.DeleteCollaboratorsRequest\x1a!.clarifai.api.status.BaseResponse\"j\x82\xd3\xe4\x93\x02L*G/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/collaborators:\x01*\x98\x9c\'\x02\x90\x9c\'3\x90\x9c\'2\x90\x9c\'4\x90\x9c\'7\x90\x9c\'8\x12\xa4\x01\n\x12ListCollaborations\x12\'.clarifai.api.ListCollaborationsRequest\x1a).clarifai.api.MultiCollaborationsResponse\":\x82\xd3\xe4\x93\x02\x30\x12./v2/users/{user_app_id.user_id}/collaborations\x98\x9c\'\x03\x12\xef\x01\n\x13PostAppDuplications\x12(.clarifai.api.PostAppDuplicationsRequest\x1a*.clarifai.api.MultiAppDuplicationsResponse\"\x81\x01\x82\xd3\xe4\x93\x02K\"F/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/duplications:\x01*\x98\x9c\'\x02\x90\x9c\'\x0e\x90\x9c\'\x0f\x90\x9c\'\x1a\x90\x9c\'\n\x90\x9c\'\x0b\x90\x9c\'\x04\x90\x9c\'\x05\x90\x9c\'%\x90\x9c\'&\x90\x9c\'\x12\x90\x9c\'\x13\x12\xa5\x01\n\x13ListAppDuplications\x12(.clarifai.api.ListAppDuplicationsRequest\x1a*.clarifai.api.MultiAppDuplicationsResponse\"8\x82\xd3\xe4\x93\x02.\x12,/v2/users/{user_app_id.user_id}/duplications\x98\x9c\'\x05\x12\xb6\x01\n\x11GetAppDuplication\x12&.clarifai.api.GetAppDuplicationRequest\x1a*.clarifai.api.SingleAppDuplicationResponse\"M\x82\xd3\xe4\x93\x02\x43\x12\x41/v2/users/{user_app_id.user_id}/duplications/{app_duplication_id}\x98\x9c\'\x05\x12\xd5\x01\n\tPostTasks\x12\x1e.clarifai.api.PostTasksRequest\x1a\x1f.clarifai.api.MultiTaskResponse\"\x86\x01\x82\xd3\xe4\x93\x02T\"?/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/tasks:\x01*Z\x0e\"\t/v2/tasks:\x01*\x98\x9c\'\x02\x90\x9c\'7\x90\x9c\'8\x90\x9c\'\x05\x90\x9c\'\x03\x90\x9c\'r\x90\x9c\'\x0b\x90\x9c\'\x13\x90\x9c\'\x0f\x90\x9c\'%\x90\x9c\'&\x12\xfa\x01\n\x16GetTaskAnnotationCount\x12!.clarifai.api.GetTaskCountRequest\x1a%.clarifai.api.SingleTaskCountResponse\"\x95\x01\x82\xd3\xe4\x93\x02\x86\x01\x12[/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/tasks/{task_id}/annotations/countZ\'\x12%/v2/tasks/{task_id}/annotations/count\x98\x9c\'\x02\x90\x9c\'8\x12\xea\x01\n\x11GetTaskInputCount\x12!.clarifai.api.GetTaskCountRequest\x1a%.clarifai.api.SingleTaskCountResponse\"\x8a\x01\x82\xd3\xe4\x93\x02|\x12V/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/tasks/{task_id}/inputs/countZ\"\x12 /v2/tasks/{task_id}/inputs/count\x98\x9c\'\x02\x90\x9c\'8\x12\xcc\x01\n\x07GetTask\x12\x1c.clarifai.api.GetTaskRequest\x1a .clarifai.api.SingleTaskResponse\"\x80\x01\x82\xd3\xe4\x93\x02\x62\x12I/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/tasks/{task_id}Z\x15\x12\x13/v2/tasks/{task_id}\x98\x9c\'\x02\x90\x9c\'8\x90\x9c\'r\x90\x9c\'\x0b\x90\x9c\'\x13\x90\x9c\'\x0f\x12\xba\x01\n\tListTasks\x12\x1e.clarifai.api.ListTasksRequest\x1a\x1f.clarifai.api.MultiTaskResponse\"l\x82\xd3\xe4\x93\x02N\x12?/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/tasksZ\x0b\x12\t/v2/tasks\x98\x9c\'\x02\x90\x9c\'8\x90\x9c\'r\x90\x9c\'\x0b\x90\x9c\'\x13\x90\x9c\'\x0f\x12\xd3\x01\n\nPatchTasks\x12\x1f.clarifai.api.PatchTasksRequest\x1a\x1f.clarifai.api.MultiTaskResponse\"\x82\x01\x82\xd3\xe4\x93\x02T2?/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/tasks:\x01*Z\x0e\x32\t/v2/tasks:\x01*\x98\x9c\'\x02\x90\x9c\'7\x90\x9c\'8\x90\x9c\'\x05\x90\x9c\'r\x90\x9c\'\x0b\x90\x9c\'\x13\x90\x9c\'\x0f\x90\x9c\'%\x90\x9c\'&\x12\xbe\x01\n\x0b\x44\x65leteTasks\x12 .clarifai.api.DeleteTasksRequest\x1a!.clarifai.api.status.BaseResponse\"j\x82\xd3\xe4\x93\x02T*?/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/tasks:\x01*Z\x0e*\t/v2/tasks:\x01*\x98\x9c\'\x02\x90\x9c\'7\x90\x9c\'8\x90\x9c\'F\x12\xf1\x01\n\x0fPostLabelOrders\x12$.clarifai.api.PostLabelOrdersRequest\x1a%.clarifai.api.MultiLabelOrderResponse\"\x90\x01\x82\xd3\xe4\x93\x02\x62\"F/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/label_orders:\x01*Z\x15\"\x10/v2/label_orders:\x01*\x98\x9c\'\x02\x90\x9c\'C\x90\x9c\'D\x90\x9c\'7\x90\x9c\'8\x90\x9c\'\x05\x90\x9c\'r\x90\x9c\'\x0b\x90\x9c\'\x13\x90\x9c\'\x0f\x12\xf2\x01\n\rGetLabelOrder\x12\".clarifai.api.GetLabelOrderRequest\x1a&.clarifai.api.SingleLabelOrderResponse\"\x94\x01\x82\xd3\xe4\x93\x02~\x12W/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/label_orders/{label_order_id}Z#\x12!/v2/label_orders/{label_order_id}\x98\x9c\'\x02\x90\x9c\'C\x90\x9c\'\x0b\x90\x9c\'8\x12\xd2\x01\n\x0fListLabelOrders\x12$.clarifai.api.ListLabelOrdersRequest\x1a%.clarifai.api.MultiLabelOrderResponse\"r\x82\xd3\xe4\x93\x02\\\x12\x46/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/label_ordersZ\x12\x12\x10/v2/label_orders\x98\x9c\'\x02\x90\x9c\'C\x90\x9c\'\x0b\x90\x9c\'8\x12\xe7\x01\n\x10PatchLabelOrders\x12%.clarifai.api.PatchLabelOrdersRequest\x1a%.clarifai.api.MultiLabelOrderResponse\"\x84\x01\x82\xd3\xe4\x93\x02\x62\x32\x46/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/label_orders:\x01*Z\x15\x32\x10/v2/label_orders:\x01*\x98\x9c\'\x02\x90\x9c\'C\x90\x9c\'D\x90\x9c\'\x0b\x90\x9c\'7\x90\x9c\'8\x90\x9c\'F\x12\xe1\x01\n\x11\x44\x65leteLabelOrders\x12&.clarifai.api.DeleteLabelOrdersRequest\x1a!.clarifai.api.status.BaseResponse\"\x80\x01\x82\xd3\xe4\x93\x02\x62*F/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/label_orders:\x01*Z\x15*\x10/v2/label_orders:\x01*\x98\x9c\'\x02\x90\x9c\'E\x90\x9c\'C\x90\x9c\'D\x90\x9c\'7\x90\x9c\'8\x12\xee\x01\n\x0ePostCollectors\x12#.clarifai.api.PostCollectorsRequest\x1a$.clarifai.api.MultiCollectorResponse\"\x90\x01\x82\xd3\xe4\x93\x02^\"D/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/collectors:\x01*Z\x13\"\x0e/v2/collectors:\x01*\x98\x9c\'\x02\x90\x9c\'\x04\x90\x9c\'%\x90\x9c\'&\x90\x9c\')\x90\x9c\'\x0b\x90\x9c\'\x04\x90\x9c\'\x05\x90\x9c\'\x0f\x90\x9c\'\x02\x90\x9c\'\x13\x12\xdf\x01\n\x0cGetCollector\x12!.clarifai.api.GetCollectorRequest\x1a%.clarifai.api.SingleCollectorResponse\"\x84\x01\x82\xd3\xe4\x93\x02v\x12S/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/collectors/{collector_id}Z\x1f\x12\x1d/v2/collectors/{collector_id}\x98\x9c\'\x02\x90\x9c\'*\x12\xc3\x01\n\x0eListCollectors\x12#.clarifai.api.ListCollectorsRequest\x1a$.clarifai.api.MultiCollectorResponse\"f\x82\xd3\xe4\x93\x02X\x12\x44/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/collectorsZ\x10\x12\x0e/v2/collectors\x98\x9c\'\x02\x90\x9c\'*\x12\xcf\x01\n\x0fPatchCollectors\x12$.clarifai.api.PatchCollectorsRequest\x1a$.clarifai.api.MultiCollectorResponse\"p\x82\xd3\xe4\x93\x02^2D/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/collectors:\x01*Z\x13\x32\x0e/v2/collectors:\x01*\x98\x9c\'\x02\x90\x9c\')\x90\x9c\'*\x12\xd2\x01\n\x10\x44\x65leteCollectors\x12%.clarifai.api.DeleteCollectorsRequest\x1a!.clarifai.api.status.BaseResponse\"t\x82\xd3\xe4\x93\x02^*D/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/collectors:\x01*Z\x13*\x0e/v2/collectors:\x01*\x98\x9c\'\x02\x90\x9c\')\x90\x9c\'+\x90\x9c\'*\x12\xc9\x01\n\x0ePostStatValues\x12#.clarifai.api.PostStatValuesRequest\x1a$.clarifai.api.MultiStatValueResponse\"l\x82\xd3\xe4\x93\x02\x62\"F/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/stats/values:\x01*Z\x15\"\x10/v2/stats/values:\x01*\x98\x9c\'\x02\x12\xf9\x01\n\x17PostStatValuesAggregate\x12,.clarifai.api.PostStatValuesAggregateRequest\x1a-.clarifai.api.MultiStatValueAggregateResponse\"\x80\x01\x82\xd3\xe4\x93\x02v\"P/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/stats/values/aggregate:\x01*Z\x1f\"\x1a/v2/stats/values/aggregate:\x01*\x98\x9c\'\x02\x12\xe3\x01\n\x17PostTrendingMetricsView\x12,.clarifai.api.PostTrendingMetricsViewRequest\x1a!.clarifai.api.status.BaseResponse\"w\x82\xd3\xe4\x93\x02m\"h/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/trending_metrics/views/{view_type}/{object_id}:\x01*\x98\x9c\'\x02\x12\x8f\x02\n\x18ListTrendingMetricsViews\x12-.clarifai.api.ListTrendingMetricsViewsRequest\x1a..clarifai.api.MultiTrendingMetricsViewResponse\"\x93\x01\x82\xd3\xe4\x93\x02\x88\x01\x12\\/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/trending_metrics/views/{view_type}Z(\x12&/v2/trending_metrics/views/{view_type}\x98\x9c\'\x02\x12\xae\x01\n\tGetModule\x12\x1e.clarifai.api.GetModuleRequest\x1a\".clarifai.api.SingleModuleResponse\"]\x82\xd3\xe4\x93\x02O\x12M/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/modules/{module_id}\x98\x9c\'\x02\x90\x9c\'m\x12\xe0\x01\n\x0bListModules\x12 .clarifai.api.ListModulesRequest\x1a!.clarifai.api.MultiModuleResponse\"\x8b\x01\x82\xd3\xe4\x93\x02}\x12\x41/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/modulesZ)\x12\'/v2/users/{user_app_id.user_id}/modulesZ\r\x12\x0b/v2/modules\x98\x9c\'\x02\x90\x9c\'m\x12\xac\x01\n\x0bPostModules\x12 .clarifai.api.PostModulesRequest\x1a!.clarifai.api.MultiModuleResponse\"X\x82\xd3\xe4\x93\x02\x46\"A/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/modules:\x01*\x98\x9c\'\x02\x90\x9c\'l\x90\x9c\'m\x12\xae\x01\n\x0cPatchModules\x12!.clarifai.api.PatchModulesRequest\x1a!.clarifai.api.MultiModuleResponse\"X\x82\xd3\xe4\x93\x02\x46\x32\x41/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/modules:\x01*\x98\x9c\'\x02\x90\x9c\'l\x90\x9c\'m\x12\xb4\x01\n\rDeleteModules\x12\".clarifai.api.DeleteModulesRequest\x1a!.clarifai.api.status.BaseResponse\"\\\x82\xd3\xe4\x93\x02\x46*A/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/modules:\x01*\x98\x9c\'\x02\x90\x9c\'l\x90\x9c\'n\x90\x9c\'m\x12\xe8\x01\n\x10GetModuleVersion\x12%.clarifai.api.GetModuleVersionRequest\x1a).clarifai.api.SingleModuleVersionResponse\"\x81\x01\x82\xd3\xe4\x93\x02s\x12q/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/modules/{module_id}/module_versions/{module_version_id}\x98\x9c\'\x02\x90\x9c\'m\x12\xd6\x01\n\x12ListModuleVersions\x12\'.clarifai.api.ListModuleVersionsRequest\x1a(.clarifai.api.MultiModuleVersionResponse\"m\x82\xd3\xe4\x93\x02_\x12]/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/modules/{module_id}/module_versions\x98\x9c\'\x02\x90\x9c\'m\x12\xdd\x01\n\x12PostModuleVersions\x12\'.clarifai.api.PostModuleVersionsRequest\x1a(.clarifai.api.MultiModuleVersionResponse\"t\x82\xd3\xe4\x93\x02\x62\"]/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/modules/{module_id}/module_versions:\x01*\x98\x9c\'\x02\x90\x9c\'l\x90\x9c\'m\x12\xde\x01\n\x14\x44\x65leteModuleVersions\x12).clarifai.api.DeleteModuleVersionsRequest\x1a!.clarifai.api.status.BaseResponse\"x\x82\xd3\xe4\x93\x02\x62*]/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/modules/{module_id}/module_versions:\x01*\x98\x9c\'\x02\x90\x9c\'l\x90\x9c\'n\x90\x9c\'m\x12\x8b\x02\n\x19GetInstalledModuleVersion\x12..clarifai.api.GetInstalledModuleVersionRequest\x1a\x32.clarifai.api.SingleInstalledModuleVersionResponse\"\x89\x01\x82\xd3\xe4\x93\x02s\x12q/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/installed_module_versions/{installed_module_version_id}\x98\x9c\'\x05\x90\x9c\'p\x90\x9c\'m\x90\x9c\'0\x12\xef\x01\n\x1bListInstalledModuleVersions\x12\x30.clarifai.api.ListInstalledModuleVersionsRequest\x1a\x31.clarifai.api.MultiInstalledModuleVersionResponse\"k\x82\xd3\xe4\x93\x02U\x12S/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/installed_module_versions\x98\x9c\'\x05\x90\x9c\'p\x90\x9c\'m\x90\x9c\'0\x12\xf6\x01\n\x1bPostInstalledModuleVersions\x12\x30.clarifai.api.PostInstalledModuleVersionsRequest\x1a\x31.clarifai.api.MultiInstalledModuleVersionResponse\"r\x82\xd3\xe4\x93\x02X\"S/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/installed_module_versions:\x01*\x98\x9c\'\x05\x90\x9c\'o\x90\x9c\'p\x90\x9c\'m\x90\x9c\'-\x12\xf6\x01\n\x1d\x44\x65leteInstalledModuleVersions\x12\x32.clarifai.api.DeleteInstalledModuleVersionsRequest\x1a!.clarifai.api.status.BaseResponse\"~\x82\xd3\xe4\x93\x02X*S/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/installed_module_versions:\x01*\x98\x9c\'\x05\x90\x9c\'o\x90\x9c\'p\x90\x9c\'q\x90\x9c\'m\x90\x9c\'1\x90\x9c\'/\x90\x9c\'0\x12\x95\x02\n\x1ePostInstalledModuleVersionsKey\x12\x33.clarifai.api.PostInstalledModuleVersionsKeyRequest\x1a\x1f.clarifai.api.SingleKeyResponse\"\x9c\x01\x82\xd3\xe4\x93\x02z\"u/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/installed_module_versions/{installed_module_version_id}/key:\x01*\x98\x9c\'\x05\x90\x9c\'o\x90\x9c\'p\x90\x9c\'m\x90\x9c\'-\x90\x9c\'/\x90\x9c\'0\x12\xf1\x01\n\x12PostBulkOperations\x12\'.clarifai.api.PostBulkOperationsRequest\x1a).clarifai.api.MultiBulkOperationsResponse\"\x86\x01\x82\xd3\xe4\x93\x02h\"I/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/bulk_operations:\x01*Z\x18\"\x13/v2/bulk_operations:\x01*\x98\x9c\'\x02\x90\x9c\'z\x90\x9c\'y\x90\x9c\'%\x90\x9c\'&\x90\x9c\'(\x12\xda\x01\n\x12ListBulkOperations\x12\'.clarifai.api.ListBulkOperationsRequest\x1a).clarifai.api.MultiBulkOperationsResponse\"p\x82\xd3\xe4\x93\x02\x62\x12I/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/bulk_operationsZ\x15\x12\x13/v2/bulk_operations\x98\x9c\'\x02\x90\x9c\'z\x12\xe1\x01\n\x10GetBulkOperation\x12%.clarifai.api.GetBulkOperationRequest\x1a*.clarifai.api.SingleBulkOperationsResponse\"z\x82\xd3\xe4\x93\x02l\x12N/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/bulk_operations/{id}Z\x1a\x12\x18/v2/bulk_operations/{id}\x98\x9c\'\x02\x90\x9c\'z\x12\xe7\x01\n\x14\x43\x61ncelBulkOperations\x12(.clarifai.api.CancelBulkOperationRequest\x1a).clarifai.api.MultiBulkOperationsResponse\"z\x82\xd3\xe4\x93\x02h2I/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/bulk_operations:\x01*Z\x18\x32\x13/v2/bulk_operations:\x01*\x98\x9c\'\x02\x90\x9c\'y\x90\x9c\'z\x12\xf0\x01\n\x14\x44\x65leteBulkOperations\x12(.clarifai.api.DeleteBulkOperationRequest\x1a!.clarifai.api.status.BaseResponse\"\x8a\x01\x82\xd3\xe4\x93\x02h*I/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/bulk_operations:\x01*Z\x18*\x13/v2/bulk_operations:\x01*\x98\x9c\'\x02\x90\x9c\'&\x90\x9c\'%\x90\x9c\'(\x90\x9c\'y\x90\x9c\'z\x90\x9c\'{\x12\xae\x02\n\x1cGetDatasetInputsSearchAddJob\x12\x31.clarifai.api.GetDatasetInputsSearchAddJobRequest\x1a\x35.clarifai.api.SingleDatasetInputsSearchAddJobResponse\"\xa3\x01\x82\xd3\xe4\x93\x02\x94\x01\x12\x62/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/datasets/inputs/search_add/jobs/{job_id}Z.\x12,/v2/datasets/inputs/search_add/jobs/{job_id}\x98\x9c\'\x02\x90\x9c\'i\x12\x84\x02\n\x17ListNextTaskAssignments\x12,.clarifai.api.ListNextTaskAssignmentsRequest\x1a .clarifai.api.MultiInputResponse\"\x98\x01\x82\xd3\xe4\x93\x02z\x12U/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/tasks/{task_id}/assignmentsZ!\x12\x1f/v2/tasks/{task_id}/assignments\x98\x9c\'\x02\x90\x9c\'&\x90\x9c\'\x0b\x90\x9c\'\x05\x90\x9c\'8\x90\x9c\'i\x12\xde\x01\n\x12PutTaskAssignments\x12\'.clarifai.api.PutTaskAssignmentsRequest\x1a!.clarifai.api.status.BaseResponse\"|\x82\xd3\xe4\x93\x02Z\x1aU/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/tasks/{task_id}/assignments:\x01*\x98\x9c\'\x02\x90\x9c\'%\x90\x9c\'&\x90\x9c\'\x0b\x90\x9c\'\x05\x90\x9c\'8\x90\x9c\'i\x12\xd6\x01\n\x11ListInputsAddJobs\x12&.clarifai.api.ListInputsAddJobsRequest\x1a\'.clarifai.api.MultiInputsAddJobResponse\"p\x82\xd3\xe4\x93\x02\x62\x12I/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/inputs/jobs/addZ\x15\x12\x13/v2/inputs/jobs/add\x98\x9c\'\x02\x90\x9c\'\x05\x12\xdd\x01\n\x0fGetInputsAddJob\x12$.clarifai.api.GetInputsAddJobRequest\x1a(.clarifai.api.SingleInputsAddJobResponse\"z\x82\xd3\xe4\x93\x02l\x12N/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/inputs/jobs/add/{id}Z\x1a\x12\x18/v2/inputs/jobs/add/{id}\x98\x9c\'\x02\x90\x9c\'\x05\x12\xc0\x01\n\x0bPostUploads\x12 .clarifai.api.PostUploadsRequest\x1a!.clarifai.api.MultiUploadResponse\"l\x82\xd3\xe4\x93\x02X\"A/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/uploads:\x01*Z\x10\"\x0b/v2/uploads:\x01*\x98\x9c\'\x02\x90\x9c\'\x81\x01\x90\x9c\'\x80\x01\x12\x88\x02\n\x15PutUploadContentParts\x12*.clarifai.api.PutUploadContentPartsRequest\x1a\".clarifai.api.SingleUploadResponse\"\x9e\x01\x82\xd3\xe4\x93\x02\x89\x01\x1a[/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/uploads/{upload_id}/content_parts:\x01*Z\'\x1a%/v2/uploads/{upload_id}/content_parts\x98\x9c\'\x02\x90\x9c\'\x81\x01\x90\x9c\'\x80\x01\x12\xca\x01\n\tGetUpload\x12\x1e.clarifai.api.GetUploadRequest\x1a\".clarifai.api.SingleUploadResponse\"y\x82\xd3\xe4\x93\x02j\x12M/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/uploads/{upload_id}Z\x19\x12\x17/v2/uploads/{upload_id}\x98\x9c\'\x02\x90\x9c\'\x80\x01\x12\xb5\x01\n\x0bListUploads\x12 .clarifai.api.ListUploadsRequest\x1a!.clarifai.api.MultiUploadResponse\"a\x82\xd3\xe4\x93\x02R\x12\x41/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/uploadsZ\r\x12\x0b/v2/uploads\x98\x9c\'\x02\x90\x9c\'\x80\x01\x12\xc9\x01\n\rDeleteUploads\x12\".clarifai.api.DeleteUploadsRequest\x1a!.clarifai.api.status.BaseResponse\"q\x82\xd3\xe4\x93\x02X*A/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/uploads:\x01*Z\x10*\x0b/v2/uploads:\x01*\x98\x9c\'\x02\x90\x9c\'\x80\x01\x90\x9c\'\x81\x01\x90\x9c\'\x82\x01\x12\x89\x02\n\x15PostInputsDataSources\x12*.clarifai.api.PostInputsDataSourcesRequest\x1a\'.clarifai.api.MultiInputsAddJobResponse\"\x9a\x01\x82\xd3\xe4\x93\x02p\"M/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/inputs/data_sources:\x01*Z\x1c\"\x17/v2/inputs/data_sources:\x01*\x98\x9c\'\x02\x90\x9c\'%\x90\x9c\'&\x90\x9c\'\x0b\x90\x9c\'\x04\x90\x9c\'\x05\x90\x9c\'\x0f\x90\x9c\'\x02\x90\x9c\'\x13\x12\xae\x02\n\x16GetInputsExtractionJob\x12+.clarifai.api.GetInputsExtractionJobRequest\x1a/.clarifai.api.SingleInputsExtractionJobResponse\"\xb5\x01\x82\xd3\xe4\x93\x02\xa6\x01\x12k/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/inputs/jobs/extraction/{inputs_extraction_job_id}Z7\x12\x35/v2/inputs/jobs/extraction/{inputs_extraction_job_id}\x98\x9c\'\x02\x90\x9c\'\x05\x12\xf9\x01\n\x18ListInputsExtractionJobs\x12-.clarifai.api.ListInputsExtractionJobsRequest\x1a..clarifai.api.MultiInputsExtractionJobResponse\"~\x82\xd3\xe4\x93\x02p\x12P/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/inputs/jobs/extractionZ\x1c\x12\x1a/v2/inputs/jobs/extraction\x98\x9c\'\x02\x90\x9c\'\x05\x12\x88\x02\n\x1a\x43\x61ncelInputsExtractionJobs\x12/.clarifai.api.CancelInputsExtractionJobsRequest\x1a..clarifai.api.MultiInputsExtractionJobResponse\"\x88\x01\x82\xd3\xe4\x93\x02v2P/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/inputs/jobs/extraction:\x01*Z\x1f\x32\x1a/v2/inputs/jobs/extraction:\x01*\x98\x9c\'\x02\x90\x9c\'\x04\x90\x9c\'\x05\x12\x81\x02\n\x11PostInputsUploads\x12&.clarifai.api.PostInputsUploadsRequest\x1a\'.clarifai.api.MultiInputsAddJobResponse\"\x9a\x01\x82\xd3\xe4\x93\x02\x66\"H/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/inputs/uploads:\x01*Z\x17\"\x12/v2/inputs/uploads:\x01*\x98\x9c\'\x02\x90\x9c\'%\x90\x9c\'&\x90\x9c\'\x0b\x90\x9c\'\x04\x90\x9c\'\x05\x90\x9c\'\x0f\x90\x9c\'\x02\x90\x9c\'\x13\x90\x9c\'\x81\x01\x90\x9c\'\x80\x01\x42Y\n\x15\x63om.clarifai.grpc.apiP\x01Z7github.com/Clarifai/clarifai-go-grpc/proto/clarifai/api\xa2\x02\x04\x43\x41IPb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n proto/clarifai/api/service.proto\x12\x0c\x63larifai.api\x1a\"proto/clarifai/api/resources.proto\x1a&proto/clarifai/api/status/status.proto\x1a)proto/clarifai/api/utils/extensions.proto\x1a%proto/clarifai/auth/scope/scope.proto\x1a(proto/clarifai/auth/util/extension.proto\x1a+proto/clarifai/api/status/status_code.proto\x1a\x1cgoogle/api/annotations.proto\x1a\x1egoogle/protobuf/duration.proto\x1a\x1cgoogle/protobuf/struct.proto\x1a\x1fgoogle/protobuf/timestamp.proto\",\n\nPagination\x12\x0c\n\x04page\x18\x01 \x01(\r\x12\x10\n\x08per_page\x18\x02 \x01(\r\"p\n\x14GetAnnotationRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x15\n\rannotation_id\x18\x02 \x01(\t\x12\x10\n\x08input_id\x18\x03 \x01(\t\"\xb7\x02\n\x16ListAnnotationsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0b\n\x03ids\x18\x02 \x03(\t\x12\x11\n\tinput_ids\x18\x03 \x03(\t\x12\x10\n\x08user_ids\x18\t \x03(\t\x12\x19\n\x11model_version_ids\x18\n \x03(\t\x12-\n\x08statuses\x18\x05 \x03(\x0b\x32\x1b.clarifai.api.status.Status\x12\x1c\n\x14list_all_annotations\x18\x06 \x01(\x08\x12\x1b\n\x13return_model_output\x18\x0c \x01(\x08\x12\x0c\n\x04page\x18\x07 \x01(\r\x12\x10\n\x08per_page\x18\x08 \x01(\r\x12\x0f\n\x07task_id\x18\x0b \x01(\tJ\x04\x08\x04\x10\x05\"x\n\x16PostAnnotationsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12-\n\x0b\x61nnotations\x18\x02 \x03(\x0b\x32\x18.clarifai.api.Annotation\"\xa7\x01\n\x17PatchAnnotationsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12-\n\x0b\x61nnotations\x18\x02 \x03(\x0b\x32\x18.clarifai.api.Annotation\x12\x0e\n\x06\x61\x63tion\x18\x03 \x01(\t\x12\x1c\n\x14\x64\x65lete_if_empty_data\x18\x04 \x01(\x08\"\xb9\x01\n\x1dPatchAnnotationsStatusRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x34\n\x0bstatus_code\x18\x02 \x01(\x0e\x32\x1f.clarifai.api.status.StatusCode\x12\x10\n\x08user_ids\x18\x03 \x03(\t\x12\x0f\n\x07task_id\x18\x04 \x01(\t\x12\x0e\n\x06\x61\x63tion\x18\x05 \x01(\t\"v\n\x1ePatchAnnotationsStatusResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x10\n\x08user_ids\x18\x02 \x03(\t\x12\x15\n\rupdated_count\x18\x03 \x01(\r\"s\n\x17\x44\x65leteAnnotationRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x10\n\x08input_id\x18\x02 \x01(\t\x12\x15\n\rannotation_id\x18\x03 \x01(\t\"k\n\x18\x44\x65leteAnnotationsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0b\n\x03ids\x18\x02 \x03(\t\x12\x11\n\tinput_ids\x18\x03 \x03(\t\"u\n\x18SingleAnnotationResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12,\n\nannotation\x18\x02 \x01(\x0b\x32\x18.clarifai.api.Annotation\"{\n\x17MultiAnnotationResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x33\n\x0b\x61nnotations\x18\x02 \x03(\x0b\x32\x18.clarifai.api.AnnotationB\x04\x80\xb5\x18\x01\"[\n\rGetAppRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x19\n\x11\x61\x64\x64itional_fields\x18\x02 \x03(\t\"\xa5\x02\n\x0fListAppsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0c\n\x04page\x18\x02 \x01(\r\x12\x10\n\x08per_page\x18\x03 \x01(\r\x12\x16\n\x0esort_ascending\x18\x05 \x01(\x08\x12\x16\n\x0csort_by_name\x18\x06 \x01(\x08H\x00\x12\x1d\n\x13sort_by_modified_at\x18\x07 \x01(\x08H\x00\x12\r\n\x05query\x18\x08 \x01(\t\x12\x10\n\x04name\x18\x04 \x01(\tB\x02\x18\x01\x12\x15\n\rfeatured_only\x18\t \x01(\x08\x12\x14\n\x0cstarred_only\x18\x0b \x01(\x08\x12\x19\n\x11\x61\x64\x64itional_fields\x18\n \x03(\tB\t\n\x07sort_by\"c\n\x0fPostAppsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x1f\n\x04\x61pps\x18\x02 \x03(\x0b\x32\x11.clarifai.api.App\"C\n\x10\x44\x65leteAppRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\"\xb9\x01\n\x10PatchAppsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x1f\n\x04\x61pps\x18\x02 \x03(\x0b\x32\x11.clarifai.api.App\x12\x0e\n\x06\x61\x63tion\x18\x03 \x01(\t\x12\x32\n\x0fmetadata_action\x18\x04 \x01(\x0b\x32\x19.clarifai.api.PatchAction\x12\x0f\n\x07reindex\x18\x05 \x01(\x08\"\xb7\x01\n\x0fPatchAppRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x1e\n\x03\x61pp\x18\x02 \x01(\x0b\x32\x11.clarifai.api.App\x12\x0e\n\x06\x61\x63tion\x18\x03 \x01(\t\x12\x32\n\x0fmetadata_action\x18\x04 \x01(\x0b\x32\x19.clarifai.api.PatchAction\x12\x0f\n\x07reindex\x18\x05 \x01(\x08\"\x81\x01\n\x13PatchAppsIdsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12)\n\x03ids\x18\x03 \x03(\x0b\x32\x1c.clarifai.api.IdUpdateSource\x12\x0e\n\x06\x61\x63tion\x18\x04 \x01(\t\"\xa3\x01\n\x17PostAppsSearchesRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12)\n\tapp_query\x18\x02 \x01(\x0b\x32\x16.clarifai.api.AppQuery\x12,\n\npagination\x18\x03 \x01(\x0b\x32\x18.clarifai.api.Pagination\"`\n\x11SingleAppResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x1e\n\x03\x61pp\x18\x02 \x01(\x0b\x32\x11.clarifai.api.App\"f\n\x10MultiAppResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12%\n\x04\x61pps\x18\x02 \x03(\x0b\x32\x11.clarifai.api.AppB\x04\x80\xb5\x18\x01\"\x8b\x01\n\x18ListCollaboratorsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x1e\n\x16list_all_collaborators\x18\x02 \x01(\x08\x12\x0c\n\x04page\x18\x03 \x01(\r\x12\x10\n\x08per_page\x18\x04 \x01(\r\"~\n\x18PostCollaboratorsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x31\n\rcollaborators\x18\x02 \x03(\x0b\x32\x1a.clarifai.api.Collaborator\"\x8f\x01\n\x19PatchCollaboratorsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x31\n\rcollaborators\x18\x02 \x03(\x0b\x32\x1a.clarifai.api.Collaborator\x12\x0e\n\x06\x61\x63tion\x18\x03 \x01(\t\"|\n\x1a\x44\x65leteCollaboratorsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x18\n\x10\x63ollaborator_ids\x18\x02 \x03(\t\x12\x13\n\x0buser_emails\x18\x03 \x03(\t\"\x82\x01\n\x1aMultiCollaboratorsResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x37\n\rcollaborators\x18\x02 \x03(\x0b\x32\x1a.clarifai.api.CollaboratorB\x04\x80\xb5\x18\x01\"l\n\x19ListCollaborationsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0c\n\x04page\x18\x02 \x01(\r\x12\x10\n\x08per_page\x18\x03 \x01(\r\"\x85\x01\n\x1bMultiCollaborationsResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x39\n\x0e\x63ollaborations\x18\x02 \x03(\x0b\x32\x1b.clarifai.api.CollaborationB\x04\x80\xb5\x18\x01\".\n\x14GetStatusCodeRequest\x12\x16\n\x0estatus_code_id\x18\x01 \x01(\t\"\x18\n\x16ListStatusCodesRequest\"G\n\x18SingleStatusCodeResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\"u\n\x17MultiStatusCodeResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12-\n\x08statuses\x18\x02 \x03(\x0b\x32\x1b.clarifai.api.status.Status\"X\n\x11GetConceptRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x12\n\nconcept_id\x18\x02 \x01(\t\"f\n\x13ListConceptsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0c\n\x04page\x18\x02 \x01(\r\x12\x10\n\x08per_page\x18\x03 \x01(\r\"\x91\x01\n\x18ListModelConceptsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x10\n\x08model_id\x18\x02 \x01(\t\x12\x12\n\nversion_id\x18\x03 \x01(\t\x12\x0c\n\x04page\x18\x04 \x01(\r\x12\x10\n\x08per_page\x18\x05 \x01(\r\"\xaf\x01\n\x1bPostConceptsSearchesRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x31\n\rconcept_query\x18\x02 \x01(\x0b\x32\x1a.clarifai.api.ConceptQuery\x12,\n\npagination\x18\x03 \x01(\x0b\x32\x18.clarifai.api.Pagination\"o\n\x13PostConceptsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\'\n\x08\x63oncepts\x18\x02 \x03(\x0b\x32\x15.clarifai.api.Concept\"\x80\x01\n\x14PatchConceptsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\'\n\x08\x63oncepts\x18\x02 \x03(\x0b\x32\x15.clarifai.api.Concept\x12\x0e\n\x06\x61\x63tion\x18\x03 \x01(\t\"j\n\x17GetConceptCountsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0c\n\x04page\x18\x02 \x01(\r\x12\x10\n\x08per_page\x18\x03 \x01(\r\"l\n\x15SingleConceptResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12&\n\x07\x63oncept\x18\x02 \x01(\x0b\x32\x15.clarifai.api.Concept\"r\n\x14MultiConceptResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12-\n\x08\x63oncepts\x18\x02 \x03(\x0b\x32\x15.clarifai.api.ConceptB\x04\x80\xb5\x18\x01\"\x82\x01\n\x19MultiConceptCountResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x38\n\x0e\x63oncept_counts\x18\x02 \x03(\x0b\x32\x1a.clarifai.api.ConceptCountB\x04\x80\xb5\x18\x01\"\xb1\x01\n\x1bListConceptRelationsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x12\n\nconcept_id\x18\x02 \x01(\t\x12\x11\n\tpredicate\x18\x03 \x01(\t\x12\x1a\n\x12knowledge_graph_id\x18\x04 \x01(\t\x12\x0c\n\x04page\x18\x05 \x01(\r\x12\x10\n\x08per_page\x18\x06 \x01(\r\"\x9c\x01\n\x1bPostConceptRelationsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x12\n\nconcept_id\x18\x02 \x01(\t\x12\x38\n\x11\x63oncept_relations\x18\x03 \x03(\x0b\x32\x1d.clarifai.api.ConceptRelation\"q\n\x1d\x44\x65leteConceptRelationsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x12\n\nconcept_id\x18\x02 \x01(\t\x12\x0b\n\x03ids\x18\x03 \x03(\t\"M\n\x1aListKnowledgeGraphsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\"\x85\x01\n\x1aPostKnowledgeGraphsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x36\n\x10knowledge_graphs\x18\x02 \x03(\x0b\x32\x1c.clarifai.api.KnowledgeGraph\"\x8f\x01\n\x1dPostConceptMappingJobsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12=\n\x14\x63oncept_mapping_jobs\x18\x02 \x03(\x0b\x32\x1f.clarifai.api.ConceptMappingJob\"\x8b\x01\n\x1cMultiConceptRelationResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12>\n\x11\x63oncept_relations\x18\x02 \x03(\x0b\x32\x1d.clarifai.api.ConceptRelationB\x04\x80\xb5\x18\x01\"\x88\x01\n\x1bMultiKnowledgeGraphResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12<\n\x10knowledge_graphs\x18\x02 \x03(\x0b\x32\x1c.clarifai.api.KnowledgeGraphB\x04\x80\xb5\x18\x01\"Z\n\x1eMultiConceptMappingJobResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x0b\n\x03ids\x18\x02 \x03(\t\"r\n\x19GetConceptLanguageRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x12\n\nconcept_id\x18\x02 \x01(\t\x12\x10\n\x08language\x18\x03 \x01(\t\"\x82\x01\n\x1bListConceptLanguagesRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x12\n\nconcept_id\x18\x02 \x01(\t\x12\x0c\n\x04page\x18\x03 \x01(\r\x12\x10\n\x08per_page\x18\x04 \x01(\r\"\xad\x01\n\x1cPatchConceptLanguagesRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x12\n\nconcept_id\x18\x02 \x01(\t\x12\x38\n\x11\x63oncept_languages\x18\x03 \x03(\x0b\x32\x1d.clarifai.api.ConceptLanguage\x12\x0e\n\x06\x61\x63tion\x18\x04 \x01(\t\"\x9c\x01\n\x1bPostConceptLanguagesRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x12\n\nconcept_id\x18\x02 \x01(\t\x12\x38\n\x11\x63oncept_languages\x18\x03 \x03(\x0b\x32\x1d.clarifai.api.ConceptLanguage\"\x85\x01\n\x1dSingleConceptLanguageResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x37\n\x10\x63oncept_language\x18\x02 \x01(\x0b\x32\x1d.clarifai.api.ConceptLanguage\"\x8b\x01\n\x1cMultiConceptLanguageResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12>\n\x11\x63oncept_languages\x18\x02 \x03(\x0b\x32\x1d.clarifai.api.ConceptLanguageB\x04\x80\xb5\x18\x01\"T\n\x0fGetInputRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x10\n\x08input_id\x18\x02 \x01(\t\"\\\n\x17GetVideoManifestRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x10\n\x08input_id\x18\x02 \x01(\t\"l\n\x16GetInputSamplesRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0f\n\x07task_id\x18\x02 \x01(\t\x12\x10\n\x08user_ids\x18\x03 \x03(\t\"\x9e\x01\n\x11ListInputsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0c\n\x04page\x18\x02 \x01(\r\x12\x10\n\x08per_page\x18\x03 \x01(\r\x12+\n\x06status\x18\x05 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x0b\n\x03ids\x18\x04 \x03(\t\"\x92\x01\n\x13StreamInputsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x10\n\x08per_page\x18\x02 \x01(\r\x12\x0f\n\x07last_id\x18\x03 \x01(\t\x12\x13\n\x0border_by_id\x18\x05 \x01(\x08\x12\x12\n\ndescending\x18\x04 \x01(\x08\"\xd3\x01\n\x11PostInputsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12#\n\x06inputs\x18\x02 \x03(\x0b\x32\x13.clarifai.api.Input\x12\x19\n\x11inputs_add_job_id\x18\x03 \x01(\t\x12M\n\x1cinput_id_conflict_resolution\x18\x04 \x01(\x0e\x32\'.clarifai.api.InputIDConflictResolution\"z\n\x12PatchInputsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12#\n\x06inputs\x18\x02 \x03(\x0b\x32\x13.clarifai.api.Input\x12\x0e\n\x06\x61\x63tion\x18\x03 \x01(\t\"W\n\x12\x44\x65leteInputRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x10\n\x08input_id\x18\x02 \x01(\t\"Y\n\x13\x44\x65leteInputsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0b\n\x03ids\x18\x02 \x03(\tJ\x04\x08\x03\x10\x04\"f\n\x13SingleInputResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\"\n\x05input\x18\x02 \x01(\x0b\x32\x13.clarifai.api.Input\"]\n\x18GetVideoManifestResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x14\n\x0cmanifest_url\x18\x02 \x01(\t\"\xa0\x01\n\x12MultiInputResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12)\n\x06inputs\x18\x02 \x03(\x0b\x32\x13.clarifai.api.InputB\x04\x80\xb5\x18\x01\x12\x32\n\x0einputs_add_job\x18\x03 \x01(\x0b\x32\x1a.clarifai.api.InputsAddJob\"r\n\x1cMultiInputAnnotationResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12%\n\x04hits\x18\x03 \x03(\x0b\x32\x11.clarifai.api.HitB\x04\x80\xb5\x18\x01\"q\n\x18SingleInputCountResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12(\n\x06\x63ounts\x18\x02 \x01(\x0b\x32\x18.clarifai.api.InputCount\"G\n\x14GetInputCountRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\"\x97\x01\n\x13ListDatasetsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0c\n\x04page\x18\x02 \x01(\r\x12\x10\n\x08per_page\x18\x03 \x01(\r\x12\x14\n\x0cstarred_only\x18\x04 \x01(\x08\x12\x19\n\x11\x61\x64\x64itional_fields\x18\x05 \x03(\t\"s\n\x11GetDatasetRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x12\n\ndataset_id\x18\x02 \x01(\t\x12\x19\n\x11\x61\x64\x64itional_fields\x18\x03 \x03(\t\"o\n\x13PostDatasetsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\'\n\x08\x64\x61tasets\x18\x02 \x03(\x0b\x32\x15.clarifai.api.Dataset\"\x80\x01\n\x14PatchDatasetsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\'\n\x08\x64\x61tasets\x18\x02 \x03(\x0b\x32\x15.clarifai.api.Dataset\x12\x0e\n\x06\x61\x63tion\x18\x03 \x01(\t\"]\n\x15\x44\x65leteDatasetsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x13\n\x0b\x64\x61taset_ids\x18\x02 \x03(\t\"r\n\x14MultiDatasetResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12-\n\x08\x64\x61tasets\x18\x02 \x03(\x0b\x32\x15.clarifai.api.DatasetB\x04\x80\xb5\x18\x01\"l\n\x15SingleDatasetResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12&\n\x07\x64\x61taset\x18\x02 \x01(\x0b\x32\x15.clarifai.api.Dataset\"\x7f\n\x18ListDatasetInputsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x12\n\ndataset_id\x18\x02 \x01(\t\x12\x0c\n\x04page\x18\x03 \x01(\r\x12\x10\n\x08per_page\x18\x04 \x01(\r\"o\n\x16GetDatasetInputRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x12\n\ndataset_id\x18\x02 \x01(\t\x12\x10\n\x08input_id\x18\x03 \x01(\t\"\xb9\x01\n\x18PostDatasetInputsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x12\n\ndataset_id\x18\x02 \x01(\t\x12\x32\n\x0e\x64\x61taset_inputs\x18\x03 \x03(\x0b\x32\x1a.clarifai.api.DatasetInput\x12$\n\x06search\x18\x04 \x01(\x0b\x32\x14.clarifai.api.Search\"t\n\x1a\x44\x65leteDatasetInputsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x12\n\ndataset_id\x18\x02 \x01(\t\x12\x11\n\tinput_ids\x18\x03 \x03(\t\"\xd2\x01\n\x19MultiDatasetInputResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x38\n\x0e\x64\x61taset_inputs\x18\x02 \x03(\x0b\x32\x1a.clarifai.api.DatasetInputB\x04\x80\xb5\x18\x01\x12N\n\x1d\x64\x61taset_inputs_search_add_job\x18\x03 \x01(\x0b\x32\'.clarifai.api.DatasetInputsSearchAddJob\"|\n\x1aSingleDatasetInputResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x31\n\rdataset_input\x18\x02 \x01(\x0b\x32\x1a.clarifai.api.DatasetInput\"\x81\x01\n\x1aListDatasetVersionsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x12\n\ndataset_id\x18\x02 \x01(\t\x12\x0c\n\x04page\x18\x03 \x01(\r\x12\x10\n\x08per_page\x18\x04 \x01(\r\"{\n\x18GetDatasetVersionRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x12\n\ndataset_id\x18\x02 \x01(\t\x12\x1a\n\x12\x64\x61taset_version_id\x18\x03 \x01(\t\"\xa4\x02\n&ListDatasetVersionMetricsGroupsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x12\n\ndataset_id\x18\x02 \x01(\t\x12\x1a\n\x12\x64\x61taset_version_id\x18\x03 \x01(\t\x12\x0c\n\x04page\x18\x04 \x01(\r\x12\x10\n\x08per_page\x18\x05 \x01(\r\x12\x14\n\x0cparent_paths\x18\x06 \x03(\t\x12;\n\x05types\x18\x07 \x03(\x0e\x32,.clarifai.api.DatasetVersionMetricsGroupType\x12&\n\x06values\x18\x08 \x03(\x0b\x32\x16.google.protobuf.Value\"\x99\x01\n\x1aPostDatasetVersionsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x12\n\ndataset_id\x18\x02 \x01(\t\x12\x36\n\x10\x64\x61taset_versions\x18\x03 \x03(\x0b\x32\x1c.clarifai.api.DatasetVersion\"\xaa\x01\n\x1bPatchDatasetVersionsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x12\n\ndataset_id\x18\x02 \x01(\t\x12\x36\n\x10\x64\x61taset_versions\x18\x03 \x03(\x0b\x32\x1c.clarifai.api.DatasetVersion\x12\x0e\n\x06\x61\x63tion\x18\x04 \x01(\t\"\x80\x01\n\x1c\x44\x65leteDatasetVersionsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x12\n\ndataset_id\x18\x02 \x01(\t\x12\x1b\n\x13\x64\x61taset_version_ids\x18\x03 \x03(\t\"\xb7\x01\n\x1fPutDatasetVersionExportsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x12\n\ndataset_id\x18\x02 \x01(\t\x12\x1a\n\x12\x64\x61taset_version_id\x18\x03 \x01(\t\x12\x33\n\x07\x65xports\x18\x04 \x03(\x0b\x32\".clarifai.api.DatasetVersionExport\"\x88\x01\n\x1bMultiDatasetVersionResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12<\n\x10\x64\x61taset_versions\x18\x02 \x03(\x0b\x32\x1c.clarifai.api.DatasetVersionB\x04\x80\xb5\x18\x01\"\x8b\x01\n!MultiDatasetVersionExportResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x39\n\x07\x65xports\x18\x02 \x03(\x0b\x32\".clarifai.api.DatasetVersionExportB\x04\x80\xb5\x18\x01\"\xae\x01\n\'MultiDatasetVersionMetricsGroupResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12V\n\x1e\x64\x61taset_version_metrics_groups\x18\x02 \x03(\x0b\x32(.clarifai.api.DatasetVersionMetricsGroupB\x04\x80\xb5\x18\x01\"\x82\x01\n\x1cSingleDatasetVersionResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x35\n\x0f\x64\x61taset_version\x18\x02 \x01(\x0b\x32\x1c.clarifai.api.DatasetVersion\"f\n#GetDatasetInputsSearchAddJobRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0e\n\x06job_id\x18\x02 \x01(\t\"\x8c\x01\n\'SingleDatasetInputsSearchAddJobResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x34\n\x03job\x18\x02 \x01(\x0b\x32\'.clarifai.api.DatasetInputsSearchAddJob\"\xb9\x01\n\x17PostModelOutputsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x10\n\x08model_id\x18\x02 \x01(\t\x12\x12\n\nversion_id\x18\x03 \x01(\t\x12#\n\x06inputs\x18\x04 \x03(\x0b\x32\x13.clarifai.api.Input\x12\"\n\x05model\x18\x05 \x01(\x0b\x32\x13.clarifai.api.Model\"\x8f\x01\n\x16ListModelInputsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x10\n\x08model_id\x18\x02 \x01(\t\x12\x12\n\nversion_id\x18\x03 \x01(\t\x12\x0c\n\x04page\x18\x04 \x01(\r\x12\x10\n\x08per_page\x18\x05 \x01(\r\"P\n\rGetKeyRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0e\n\x06key_id\x18\x02 \x01(\t\"\x9a\x01\n\x0fListKeysRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0c\n\x04page\x18\x02 \x01(\r\x12\x10\n\x08per_page\x18\x03 \x01(\r\x12\x13\n\x0bnot_expired\x18\x04 \x01(\x08\x12\x0e\n\x06scopes\x18\x05 \x03(\t\x12\x11\n\tendpoints\x18\x06 \x03(\t\"e\n\x12ListAppKeysRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0c\n\x04page\x18\x02 \x01(\r\x12\x10\n\x08per_page\x18\x03 \x01(\r\"c\n\x0fPostKeysRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x1f\n\x04keys\x18\x02 \x03(\x0b\x32\x11.clarifai.api.Key\"S\n\x10\x44\x65leteKeyRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0e\n\x06key_id\x18\x02 \x01(\t\"t\n\x10PatchKeysRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x1f\n\x04keys\x18\x02 \x03(\x0b\x32\x11.clarifai.api.Key\x12\x0e\n\x06\x61\x63tion\x18\x03 \x01(\t\"`\n\x11SingleKeyResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x1e\n\x03key\x18\x02 \x01(\x0b\x32\x11.clarifai.api.Key\"f\n\x10MultiKeyResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12%\n\x04keys\x18\x02 \x03(\x0b\x32\x11.clarifai.api.KeyB\x04\x80\xb5\x18\x01\"\xad\x01\n\x0fGetModelRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x10\n\x08model_id\x18\x02 \x01(\t\x12\x12\n\nversion_id\x18\x03 \x01(\t\x12\x10\n\x08language\x18\x04 \x01(\t\x12\x16\n\x0etrained_before\x18\x05 \x01(\x08\x12\x19\n\x11\x61\x64\x64itional_fields\x18\x13 \x03(\t\"\xa3\x04\n\x11ListModelsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0c\n\x04page\x18\x02 \x01(\r\x12\x10\n\x08per_page\x18\x03 \x01(\r\x12\x16\n\x0esort_ascending\x18\n \x01(\x08\x12\x16\n\x0csort_by_name\x18\x0b \x01(\x08H\x00\x12\x1c\n\x12sort_by_num_inputs\x18\x0c \x01(\x08H\x00\x12\x1d\n\x13sort_by_modified_at\x18\r \x01(\x08H\x00\x12\r\n\x05query\x18\x0e \x01(\t\x12\x0c\n\x04name\x18\x05 \x01(\t\x12\x19\n\x11\x66ilter_by_user_id\x18\x16 \x01(\x08\x12\x15\n\rmodel_type_id\x18\x06 \x01(\t\x12\x14\n\x0ctrained_only\x18\x07 \x01(\x08\x12\x14\n\x0cinput_fields\x18\x08 \x03(\t\x12\x15\n\routput_fields\x18\t \x03(\t\x12\x0f\n\x07license\x18\x0f \x01(\t\x12\x15\n\rfeatured_only\x18\x10 \x01(\x08\x12\x14\n\x0cstarred_only\x18\x14 \x01(\x08\x12\x10\n\x08toolkits\x18\x11 \x03(\t\x12\x11\n\tuse_cases\x18\x12 \x03(\t\x12\x11\n\tlanguages\x18\x15 \x03(\t\x12\x19\n\x11\x61\x64\x64itional_fields\x18\x13 \x03(\t\x12\x1c\n\x14\x64ont_fetch_from_main\x18\x17 \x01(\x08\x42\t\n\x07sort_byJ\x04\x08\x04\x10\x05\"K\n\x18GetResourceCountsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\"\x8e\x01\n\x19GetResourceCountsResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x10\n\x08\x64\x61tasets\x18\x02 \x01(\x03\x12\x0e\n\x06models\x18\x03 \x01(\x03\x12\x11\n\tworkflows\x18\x04 \x01(\x03\x12\x0f\n\x07modules\x18\x05 \x01(\x03\"\x80\x01\n\x19PatchModelToolkitsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x10\n\x08model_id\x18\x02 \x01(\t\x12\x10\n\x08toolkits\x18\x03 \x03(\t\x12\x0e\n\x06\x61\x63tion\x18\x04 \x01(\t\"\x8b\x01\n\x1ePatchModelCheckConsentsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x10\n\x08model_id\x18\x02 \x01(\t\x12\x16\n\x0e\x63heck_consents\x18\x03 \x03(\t\x12\x0e\n\x06\x61\x63tion\x18\x04 \x01(\t\"\x80\x01\n\x19PatchModelUseCasesRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x10\n\x08model_id\x18\x02 \x01(\t\x12\x10\n\x08usecases\x18\x03 \x03(\t\x12\x0e\n\x06\x61\x63tion\x18\x04 \x01(\t\"\x82\x01\n\x1aPatchModelLanguagesRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x10\n\x08model_id\x18\x02 \x01(\t\x12\x11\n\tlanguages\x18\x03 \x03(\t\x12\x0e\n\x06\x61\x63tion\x18\x04 \x01(\t\"Z\n\x19MultiModelToolkitResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x10\n\x08toolkits\x18\x02 \x03(\t\"e\n\x1eMultiModelCheckConsentResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x16\n\x0e\x63heck_consents\x18\x02 \x03(\t\"Z\n\x19MultiModelUseCaseResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x10\n\x08usecases\x18\x02 \x03(\t\"\\\n\x1aMultiModelLanguageResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x11\n\tlanguages\x18\x02 \x03(\t\"\x91\x01\n\x11PostModelsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12&\n\x05model\x18\x02 \x01(\x0b\x32\x13.clarifai.api.ModelB\x02\x18\x01\x12#\n\x06models\x18\x03 \x03(\x0b\x32\x13.clarifai.api.Model\"z\n\x12PatchModelsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12#\n\x06models\x18\x02 \x03(\x0b\x32\x13.clarifai.api.Model\x12\x0e\n\x06\x61\x63tion\x18\x03 \x01(\t\",\n\x0eIdUpdateSource\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0e\n\x06new_id\x18\x02 \x01(\t\"\x82\x01\n\x14PatchModelIdsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12)\n\x03ids\x18\x03 \x03(\x0b\x32\x1c.clarifai.api.IdUpdateSource\x12\x0e\n\x06\x61\x63tion\x18\x04 \x01(\t\"W\n\x12\x44\x65leteModelRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x10\n\x08model_id\x18\x02 \x01(\t\"g\n\x13\x44\x65leteModelsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0b\n\x03ids\x18\x02 \x03(\t\x12\x12\n\ndelete_all\x18\x03 \x01(\x08\"\xa9\x01\n\x19PostModelsSearchesRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12-\n\x0bmodel_query\x18\x02 \x01(\x0b\x32\x18.clarifai.api.ModelQuery\x12,\n\npagination\x18\x03 \x01(\x0b\x32\x18.clarifai.api.Pagination\"f\n\x13SingleModelResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\"\n\x05model\x18\x02 \x01(\x0b\x32\x13.clarifai.api.Model\"l\n\x12MultiModelResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12)\n\x06models\x18\x02 \x03(\x0b\x32\x13.clarifai.api.ModelB\x04\x80\xb5\x18\x01\"\xa2\x01\n\x19PatchModelVersionsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x10\n\x08model_id\x18\x02 \x01(\t\x12\x32\n\x0emodel_versions\x18\x03 \x03(\x0b\x32\x1a.clarifai.api.ModelVersion\x12\x0e\n\x06\x61\x63tion\x18\x04 \x01(\t\"o\n\x16GetModelVersionRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x10\n\x08model_id\x18\x02 \x01(\t\x12\x12\n\nversion_id\x18\x03 \x01(\t\"\xc5\x02\n\x18ListModelVersionsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x10\n\x08model_id\x18\x02 \x01(\t\x12\x0c\n\x04page\x18\x03 \x01(\r\x12\x10\n\x08per_page\x18\x04 \x01(\r\x12\x13\n\x0b\x63oncept_ids\x18\x05 \x03(\t\x12\x14\n\x0ctrained_only\x18\x06 \x01(\x08\x12\x16\n\x0esort_ascending\x18\x07 \x01(\x08\x12\x1d\n\x13sort_by_status_code\x18\x08 \x01(\x08H\x00\x12\x1c\n\x12sort_by_num_inputs\x18\t \x01(\x08H\x00\x12\x1d\n\x13sort_by_description\x18\n \x01(\x08H\x00\x12\x1c\n\x12sort_by_created_at\x18\x0b \x01(\x08H\x00\x42\t\n\x07sort_by\"r\n\x19\x44\x65leteModelVersionRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x10\n\x08model_id\x18\x03 \x01(\t\x12\x12\n\nversion_id\x18\x04 \x01(\t\"|\n\x1aSingleModelVersionResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x31\n\rmodel_version\x18\x02 \x01(\x0b\x32\x1a.clarifai.api.ModelVersion\"\x82\x01\n\x19MultiModelVersionResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x38\n\x0emodel_versions\x18\x02 \x03(\x0b\x32\x1a.clarifai.api.ModelVersionB\x04\x80\xb5\x18\x01\"\xef\x01\n\x18PostModelVersionsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x10\n\x08model_id\x18\x02 \x01(\t\x12\x32\n\x0emodel_versions\x18\x03 \x03(\x0b\x32\x1a.clarifai.api.ModelVersion\x12\x13\n\x0b\x64\x65scription\x18\x08 \x01(\t\x12)\n\teval_info\x18\n \x01(\x0b\x32\x16.clarifai.api.EvalInfoJ\x04\x08\x04\x10\x05J\x04\x08\x05\x10\x06J\x04\x08\x06\x10\x07J\x04\x08\x07\x10\x08J\x04\x08\t\x10\n\"\xb1\x01\n$PostWorkflowVersionsUnPublishRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x13\n\x0bworkflow_id\x18\x02 \x01(\t\x12\x43\n\x0cpublications\x18\x03 \x03(\x0b\x32-.clarifai.api.WorkflowVersionUnPublishRequest\"\xad\x01\n\"PostWorkflowVersionsPublishRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x13\n\x0bworkflow_id\x18\x02 \x01(\t\x12\x41\n\x0cpublications\x18\x03 \x03(\x0b\x32+.clarifai.api.WorkflowVersionPublishRequest\"3\n\x1dWorkflowVersionPublishRequest\x12\x12\n\nversion_id\x18\x01 \x01(\t\"5\n\x1fWorkflowVersionUnPublishRequest\x12\x12\n\nversion_id\x18\x01 \x01(\t\"0\n\x1aModelVersionPublishRequest\x12\x12\n\nversion_id\x18\x01 \x01(\t\"\xa4\x01\n\x1fPostModelVersionsPublishRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x10\n\x08model_id\x18\x02 \x01(\t\x12>\n\x0cpublications\x18\x03 \x03(\x0b\x32(.clarifai.api.ModelVersionPublishRequest\"2\n\x1cModelVersionUnpublishRequest\x12\x12\n\nversion_id\x18\x01 \x01(\t\"\xa8\x01\n!PostModelVersionsUnPublishRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x10\n\x08model_id\x18\x02 \x01(\t\x12@\n\x0cpublications\x18\x03 \x03(\x0b\x32*.clarifai.api.ModelVersionUnpublishRequest\"z\n\x16PostEvaluationsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12/\n\x0c\x65val_metrics\x18\x02 \x03(\x0b\x32\x19.clarifai.api.EvalMetrics\"i\n\x16ListEvaluationsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0c\n\x04page\x18\x02 \x01(\r\x12\x10\n\x08per_page\x18\x03 \x01(\r\"\x89\x01\n\x14GetEvaluationRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x15\n\revaluation_id\x18\x02 \x01(\t\x12)\n\x06\x66ields\x18\x03 \x01(\x0b\x32\x19.clarifai.api.FieldsValue\"\xb2\x01\n\"PostModelVersionEvaluationsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x10\n\x08model_id\x18\x02 \x01(\t\x12\x18\n\x10model_version_id\x18\x03 \x01(\t\x12/\n\x0c\x65val_metrics\x18\x04 \x03(\x0b\x32\x19.clarifai.api.EvalMetrics\"\xa1\x01\n\"ListModelVersionEvaluationsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x10\n\x08model_id\x18\x02 \x01(\t\x12\x18\n\x10model_version_id\x18\x03 \x01(\t\x12\x0c\n\x04page\x18\x04 \x01(\r\x12\x10\n\x08per_page\x18\x05 \x01(\r\"\xc1\x01\n GetModelVersionEvaluationRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x10\n\x08model_id\x18\x02 \x01(\t\x12\x18\n\x10model_version_id\x18\x03 \x01(\t\x12\x15\n\revaluation_id\x18\x04 \x01(\t\x12)\n\x06\x66ields\x18\x05 \x01(\x0b\x32\x19.clarifai.api.FieldsValue\"y\n\x19SingleEvalMetricsResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12/\n\x0c\x65val_metrics\x18\x02 \x01(\x0b\x32\x19.clarifai.api.EvalMetrics\"x\n\x18MultiEvalMetricsResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12/\n\x0c\x65val_metrics\x18\x02 \x03(\x0b\x32\x19.clarifai.api.EvalMetrics\"\xd3\x01\n\x1ePostModelVersionMetricsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x10\n\x08model_id\x18\x02 \x01(\t\x12\x12\n\nversion_id\x18\x03 \x01(\t\x12)\n\x0btest_search\x18\x05 \x01(\x0b\x32\x14.clarifai.api.Search\x12)\n\teval_info\x18\n \x01(\x0b\x32\x16.clarifai.api.EvalInfoJ\x04\x08\x04\x10\x05\"\xa1\x01\n\x1dGetModelVersionMetricsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x10\n\x08model_id\x18\x02 \x01(\t\x12\x12\n\nversion_id\x18\x03 \x01(\t\x12)\n\x06\x66ields\x18\x04 \x01(\x0b\x32\x19.clarifai.api.FieldsValue\"]\n\x13GetModelTypeRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x15\n\rmodel_type_id\x18\x02 \x01(\t\"h\n\x15ListModelTypesRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0c\n\x04page\x18\x02 \x01(\r\x12\x10\n\x08per_page\x18\x03 \x01(\r\"\x1f\n\x1dListOpenSourceLicensesRequest\"_\n\x1eListOpenSourceLicensesResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x10\n\x08licenses\x18\x02 \x03(\t\"y\n\x17SingleModelTypeResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x31\n\nmodel_type\x18\x02 \x01(\x0b\x32\x17.clarifai.api.ModelTypeB\x04\x80\xb5\x18\x01\"\xf2\x01\n\x16MultiModelTypeResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x32\n\x0bmodel_types\x18\x02 \x03(\x0b\x32\x17.clarifai.api.ModelTypeB\x04\x80\xb5\x18\x01\x12\x35\n\x0fmodel_importers\x18\x03 \x01(\x0b\x32\x1c.clarifai.api.ModelTypeField\x12@\n\x16triton_conda_envs_info\x18\x04 \x03(\x0b\x32 .clarifai.api.TritonCondaEnvInfo\"\x95\x01\n\"GetModelVersionInputExampleRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x10\n\x08model_id\x18\x02 \x01(\t\x12\x18\n\x10model_version_id\x18\x03 \x01(\t\x12\x12\n\nexample_id\x18\x04 \x01(\t\"\xa3\x01\n$ListModelVersionInputExamplesRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x10\n\x08model_id\x18\x02 \x01(\t\x12\x18\n\x10model_version_id\x18\x03 \x01(\t\x12\x0c\n\x04page\x18\x04 \x01(\r\x12\x10\n\x08per_page\x18\x05 \x01(\r\"\xa2\x01\n&SingleModelVersionInputExampleResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12K\n\x1bmodel_version_input_example\x18\x02 \x01(\x0b\x32&.clarifai.api.ModelVersionInputExample\"\xa2\x01\n%MultiModelVersionInputExampleResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12L\n\x1cmodel_version_input_examples\x18\x02 \x03(\x0b\x32&.clarifai.api.ModelVersionInputExample\"\x7f\n\x1aListModelReferencesRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x10\n\x08model_id\x18\x02 \x01(\t\x12\x0c\n\x04page\x18\x03 \x01(\r\x12\x10\n\x08per_page\x18\x04 \x01(\r\"\x82\x01\n\x1bMultiModelReferenceResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x36\n\x10model_references\x18\x02 \x03(\x0b\x32\x1c.clarifai.api.ModelReference\"o\n\x13MultiOutputResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12+\n\x07outputs\x18\x02 \x03(\x0b\x32\x14.clarifai.api.OutputB\x04\x80\xb5\x18\x01\"V\n\x11ListScopesRequest\x12\x10\n\x08key_type\x18\x01 \x01(\t\x12/\n\x0buser_app_id\x18\x02 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\"B\n\x0fMyScopesRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\"F\n\x13MyScopesUserRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\"\x15\n\x13MyScopesRootRequest\"\xa5\x01\n\x16MultiScopeDepsResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12+\n\nscope_deps\x18\x02 \x03(\x0b\x32\x17.clarifai.api.ScopeDeps\x12\x31\n\rendpoint_deps\x18\x03 \x03(\x0b\x32\x1a.clarifai.api.EndpointDeps\"\xa0\x01\n\x12MultiScopeResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x0e\n\x06scopes\x18\x02 \x03(\t\x12\x1e\n\x03\x61pp\x18\x03 \x01(\x0b\x32\x11.clarifai.api.App\x12\x11\n\tendpoints\x18\x04 \x03(\t\x12\x1a\n\x12user_feature_flags\x18\x05 \x01(\t\"\x84\x01\n\x16MultiScopeUserResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x0e\n\x06scopes\x18\x02 \x03(\t\x12\x11\n\tendpoints\x18\x04 \x03(\t\x12\x1a\n\x12user_feature_flags\x18\x05 \x01(\t\"\x84\x01\n\x16MultiScopeRootResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x0e\n\x06scopes\x18\x02 \x03(\t\x12\x11\n\tendpoints\x18\x04 \x03(\t\x12\x1a\n\x12user_feature_flags\x18\x05 \x01(\t\"O\n\x10GetSearchRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\n\n\x02id\x18\x02 \x01(\t\"f\n\x13ListSearchesRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0c\n\x04page\x18\x02 \x01(\r\x12\x10\n\x08per_page\x18\x03 \x01(\r\"\xc4\x01\n\x13PostSearchesRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12&\n\x05query\x18\x02 \x01(\x0b\x32\x13.clarifai.api.QueryB\x02\x18\x01\x12&\n\x08searches\x18\x03 \x03(\x0b\x32\x14.clarifai.api.Search\x12,\n\npagination\x18\x04 \x01(\x0b\x32\x18.clarifai.api.Pagination\"\x85\x01\n\x1aPatchInputsSearchesRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12&\n\x08searches\x18\x02 \x03(\x0b\x32\x14.clarifai.api.Search\x12\x0e\n\x06\x61\x63tion\x18\x03 \x01(\t\"\x8a\x01\n\x1fPatchAnnotationsSearchesRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12&\n\x08searches\x18\x02 \x03(\x0b\x32\x14.clarifai.api.Search\x12\x0e\n\x06\x61\x63tion\x18\x03 \x01(\t\"\x7f\n\x14PatchSearchesRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12&\n\x08searches\x18\x02 \x03(\x0b\x32\x14.clarifai.api.Search\x12\x0e\n\x06\x61\x63tion\x18\x03 \x01(\t\"\x84\x01\n\x17PostSearchesByIDRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\n\n\x02id\x18\x02 \x01(\t\x12,\n\npagination\x18\x03 \x01(\x0b\x32\x18.clarifai.api.Pagination\"R\n\x13\x44\x65leteSearchRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\n\n\x02id\x18\x02 \x01(\t\"\xa7\x01\n\x1ePostAnnotationsSearchesRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12&\n\x08searches\x18\x02 \x03(\x0b\x32\x14.clarifai.api.Search\x12,\n\npagination\x18\x03 \x01(\x0b\x32\x18.clarifai.api.Pagination\"c\n$DeleteAnnotationSearchMetricsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\n\n\x02id\x18\x02 \x01(\t\"\xb6\x01\n\x19PostInputsSearchesRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12&\n\x08searches\x18\x02 \x03(\x0b\x32\x14.clarifai.api.Search\x12,\n\npagination\x18\x03 \x01(\x0b\x32\x18.clarifai.api.Pagination\x12\x12\n\nonly_count\x18\x04 \x01(\x08\"i\n\x14SingleSearchResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12$\n\x06search\x18\x05 \x01(\x0b\x32\x14.clarifai.api.Search\"\xed\x01\n\x13MultiSearchResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\n\n\x02id\x18\x02 \x01(\t\x12%\n\x04hits\x18\x03 \x03(\x0b\x32\x11.clarifai.api.HitB\x04\x80\xb5\x18\x01\x12\"\n\x05query\x18\x04 \x01(\x0b\x32\x13.clarifai.api.Query\x12&\n\x08searches\x18\x05 \x03(\x0b\x32\x14.clarifai.api.Search\x12*\n\nhit_counts\x18\x06 \x03(\x0b\x32\x16.clarifai.api.HitCount\"\x94\x02\n\"PostAnnotationSearchMetricsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\n\n\x02id\x18\x02 \x01(\t\x12*\n\x0cground_truth\x18\x03 \x01(\x0b\x32\x14.clarifai.api.Search\x12,\n\x0esearch_to_eval\x18\x04 \x01(\x0b\x32\x14.clarifai.api.Search\x12 \n\x04\x64\x61ta\x18\x05 \x01(\x0b\x32\x12.clarifai.api.Data\x12\x35\n\x0f\x65valuation_type\x18\x06 \x01(\x0e\x32\x1c.clarifai.api.EvaluationType\"`\n!GetAnnotationSearchMetricsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\n\n\x02id\x18\x02 \x01(\t\"U\n\"ListAnnotationSearchMetricsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\"\x9d\x01\n$MultiAnnotationSearchMetricsResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12H\n\x19\x61nnotation_search_metrics\x18\x02 \x03(\x0b\x32%.clarifai.api.AnnotationSearchMetrics\"o\n\x1cListAnnotationFiltersRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0c\n\x04page\x18\x02 \x01(\r\x12\x10\n\x08per_page\x18\x03 \x01(\r\"k\n\x1aGetAnnotationFilterRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x1c\n\x14\x61nnotation_filter_id\x18\x02 \x01(\t\"\x8b\x01\n\x1cPostAnnotationFiltersRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12:\n\x12\x61nnotation_filters\x18\x02 \x03(\x0b\x32\x1e.clarifai.api.AnnotationFilter\"\x9c\x01\n\x1dPatchAnnotationFiltersRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12:\n\x12\x61nnotation_filters\x18\x02 \x03(\x0b\x32\x1e.clarifai.api.AnnotationFilter\x12\x0e\n\x06\x61\x63tion\x18\x03 \x01(\t\"p\n\x1e\x44\x65leteAnnotationFiltersRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x1d\n\x15\x61nnotation_filter_ids\x18\x02 \x03(\t\"\x8e\x01\n\x1dMultiAnnotationFilterResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12@\n\x12\x61nnotation_filters\x18\x02 \x03(\x0b\x32\x1e.clarifai.api.AnnotationFilterB\x04\x80\xb5\x18\x01\"\x88\x01\n\x1eSingleAnnotationFilterResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x39\n\x11\x61nnotation_filter\x18\x02 \x01(\x0b\x32\x1e.clarifai.api.AnnotationFilter\"\\\n\x0eGetUserRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x19\n\x11\x61\x64\x64itional_fields\x18\x02 \x03(\t\"c\n\x12SingleUserResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12 \n\x04user\x18\x02 \x01(\x0b\x32\x12.clarifai.api.User\"x\n\x1bPostValidatePasswordRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12(\n\x08password\x18\x02 \x01(\x0b\x32\x16.clarifai.api.Password\"\x8e\x01\n SinglePasswordValidationResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12=\n\x13password_violations\x18\x02 \x01(\x0b\x32 .clarifai.api.PasswordViolations\"\xbb\x01\n\x12GetWorkflowRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x13\n\x0bworkflow_id\x18\x02 \x01(\t\x12 \n\x18\x66\x61vor_clarifai_workflows\x18\x03 \x01(\x08\x12\x19\n\x11\x61\x64\x64itional_fields\x18\x04 \x03(\t\x12\"\n\x1a\x65xclude_clarifai_workflows\x18\x05 \x01(\x08\"\xbb\x02\n\x14ListWorkflowsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0c\n\x04page\x18\x02 \x01(\r\x12\x10\n\x08per_page\x18\x03 \x01(\r\x12\x16\n\x0esort_ascending\x18\x05 \x01(\x08\x12\x14\n\nsort_by_id\x18\x06 \x01(\x08H\x00\x12\x1d\n\x13sort_by_modified_at\x18\x07 \x01(\x08H\x00\x12\r\n\x05query\x18\x08 \x01(\t\x12\x0e\n\x02id\x18\x04 \x01(\tB\x02\x18\x01\x12\x15\n\rfeatured_only\x18\t \x01(\x08\x12\x14\n\x0cstarred_only\x18\x0b \x01(\x08\x12\x19\n\x11\x61\x64\x64itional_fields\x18\n \x03(\t\x12\x13\n\x0bsearch_term\x18\x0c \x01(\tB\t\n\x07sort_by\"r\n\x14PostWorkflowsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12)\n\tworkflows\x18\x02 \x03(\x0b\x32\x16.clarifai.api.Workflow\"\x83\x01\n\x15PatchWorkflowsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12)\n\tworkflows\x18\x02 \x03(\x0b\x32\x16.clarifai.api.Workflow\x12\x0e\n\x06\x61\x63tion\x18\x03 \x01(\t\"\x85\x01\n\x17PatchWorkflowIdsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12)\n\x03ids\x18\x03 \x03(\x0b\x32\x1c.clarifai.api.IdUpdateSource\x12\x0e\n\x06\x61\x63tion\x18\x04 \x01(\t\"]\n\x15\x44\x65leteWorkflowRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x13\n\x0bworkflow_id\x18\x02 \x01(\t\"j\n\x16\x44\x65leteWorkflowsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0b\n\x03ids\x18\x02 \x03(\t\x12\x12\n\ndelete_all\x18\x03 \x01(\x08\"o\n\x16SingleWorkflowResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12(\n\x08workflow\x18\x02 \x01(\x0b\x32\x16.clarifai.api.Workflow\"u\n\x15MultiWorkflowResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12/\n\tworkflows\x18\x02 \x03(\x0b\x32\x16.clarifai.api.WorkflowB\x04\x80\xb5\x18\x01\"\xa5\x02\n\x1aPostWorkflowResultsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x13\n\x0bworkflow_id\x18\x02 \x01(\t\x12\x12\n\nversion_id\x18\x07 \x01(\t\x12#\n\x06inputs\x18\x03 \x03(\x0b\x32\x13.clarifai.api.Input\x12\x31\n\routput_config\x18\x04 \x01(\x0b\x32\x1a.clarifai.api.OutputConfig\x12 \n\x18\x66\x61vor_clarifai_workflows\x18\x05 \x01(\x08\x12\x33\n\x0eworkflow_state\x18\x06 \x01(\x0b\x32\x1b.clarifai.api.WorkflowState\"\xd8\x01\n\x1bPostWorkflowResultsResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12(\n\x08workflow\x18\x02 \x01(\x0b\x32\x16.clarifai.api.Workflow\x12-\n\x07results\x18\x03 \x03(\x0b\x32\x1c.clarifai.api.WorkflowResult\x12\x33\n\x0eworkflow_state\x18\x04 \x01(\x0b\x32\x1b.clarifai.api.WorkflowState\"\x91\x02\n$PostWorkflowResultsSimilarityRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x13\n\x0bworkflow_id\x18\x02 \x01(\t\x12\x12\n\nversion_id\x18\x07 \x01(\t\x12\x18\n\x10model_version_id\x18\x03 \x01(\t\x12)\n\x0cprobe_inputs\x18\x04 \x03(\x0b\x32\x13.clarifai.api.Input\x12(\n\x0bpool_inputs\x18\x05 \x03(\x0b\x32\x13.clarifai.api.Input\x12 \n\x18\x66\x61vor_clarifai_workflows\x18\x06 \x01(\x08\"\x8e\x01\n%PostWorkflowResultsSimilarityResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x38\n\x07results\x18\x02 \x03(\x0b\x32\'.clarifai.api.WorkflowResultsSimilarity\"\x83\x01\n\x1bListWorkflowVersionsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x13\n\x0bworkflow_id\x18\x02 \x01(\t\x12\x0c\n\x04page\x18\x03 \x01(\r\x12\x10\n\x08per_page\x18\x04 \x01(\r\"~\n\x19GetWorkflowVersionRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x13\n\x0bworkflow_id\x18\x02 \x01(\t\x12\x1b\n\x13workflow_version_id\x18\x03 \x01(\t\"\x83\x01\n\x1d\x44\x65leteWorkflowVersionsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x13\n\x0bworkflow_id\x18\x02 \x01(\t\x12\x1c\n\x14workflow_version_ids\x18\x03 \x03(\t\"\xae\x01\n\x1cPatchWorkflowVersionsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x13\n\x0bworkflow_id\x18\x02 \x01(\t\x12\x38\n\x11workflow_versions\x18\x03 \x03(\x0b\x32\x1d.clarifai.api.WorkflowVersion\x12\x0e\n\x06\x61\x63tion\x18\x04 \x01(\t\"\x8b\x01\n\x1cMultiWorkflowVersionResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12>\n\x11workflow_versions\x18\x02 \x03(\x0b\x32\x1d.clarifai.api.WorkflowVersionB\x04\x80\xb5\x18\x01\"\x85\x01\n\x1dSingleWorkflowVersionResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x37\n\x10workflow_version\x18\x02 \x01(\x0b\x32\x1d.clarifai.api.WorkflowVersion\"\x85\x01\n\x1aPostAppDuplicationsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x36\n\x10\x61pp_duplications\x18\x02 \x03(\x0b\x32\x1c.clarifai.api.AppDuplication\"g\n\x18GetAppDuplicationRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x1a\n\x12\x61pp_duplication_id\x18\x02 \x01(\t\"m\n\x1aListAppDuplicationsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0c\n\x04page\x18\x02 \x01(\r\x12\x10\n\x08per_page\x18\x03 \x01(\r\"\x83\x01\n\x1cMultiAppDuplicationsResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x36\n\x10\x61pp_duplications\x18\x02 \x03(\x0b\x32\x1c.clarifai.api.AppDuplication\"\x82\x01\n\x1cSingleAppDuplicationResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x35\n\x0f\x61pp_duplication\x18\x02 \x01(\x0b\x32\x1c.clarifai.api.AppDuplication\"f\n\x10PostTasksRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12!\n\x05tasks\x18\x02 \x03(\x0b\x32\x12.clarifai.api.Task\"m\n\x0eGetTaskRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0f\n\x07task_id\x18\x02 \x01(\t\x12\x19\n\x11\x61\x64\x64itional_fields\x18\x03 \x03(\t\"\xee\x01\n\x10ListTasksRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0c\n\x04page\x18\x02 \x01(\r\x12\x10\n\x08per_page\x18\x03 \x01(\r\x12\x17\n\x0fworker_user_ids\x18\x04 \x03(\t\x12\x17\n\x0freview_user_ids\x18\x05 \x03(\t\x12\x17\n\x0flabel_order_ids\x18\x08 \x03(\t\x12#\n\x1bincluding_label_order_tasks\x18\x06 \x01(\x08\x12\x19\n\x11\x61\x64\x64itional_fields\x18\x07 \x03(\t\"w\n\x11PatchTasksRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12!\n\x05tasks\x18\x02 \x03(\x0b\x32\x12.clarifai.api.Task\x12\x0e\n\x06\x61\x63tion\x18\x03 \x01(\t\"R\n\x12\x44\x65leteTasksRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0b\n\x03ids\x18\x02 \x03(\t\"i\n\x11MultiTaskResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\'\n\x05tasks\x18\x02 \x03(\x0b\x32\x12.clarifai.api.TaskB\x04\x80\xb5\x18\x01\"c\n\x12SingleTaskResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12 \n\x04task\x18\x02 \x01(\x0b\x32\x12.clarifai.api.Task\"i\n\x13GetTaskCountRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0f\n\x07task_id\x18\x02 \x01(\t\x12\x10\n\x08user_ids\x18\x03 \x03(\t\"\x9d\x01\n\x17SingleTaskCountResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x0e\n\x06\x61pp_id\x18\x02 \x01(\t\x12\x0f\n\x07task_id\x18\x03 \x01(\t\x12\x34\n\x06\x63ounts\x18\x04 \x03(\x0b\x32$.clarifai.api.TaskStatusCountPerUser\"y\n\x16PostLabelOrdersRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12.\n\x0clabel_orders\x18\x02 \x03(\x0b\x32\x18.clarifai.api.LabelOrder\"_\n\x14GetLabelOrderRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x16\n\x0elabel_order_id\x18\x02 \x01(\t\"i\n\x16ListLabelOrdersRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0c\n\x04page\x18\x02 \x01(\r\x12\x10\n\x08per_page\x18\x03 \x01(\r\"\x8a\x01\n\x17PatchLabelOrdersRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12.\n\x0clabel_orders\x18\x02 \x03(\x0b\x32\x18.clarifai.api.LabelOrder\x12\x0e\n\x06\x61\x63tion\x18\x03 \x01(\t\"X\n\x18\x44\x65leteLabelOrdersRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0b\n\x03ids\x18\x02 \x03(\t\"|\n\x17MultiLabelOrderResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x34\n\x0clabel_orders\x18\x02 \x03(\x0b\x32\x18.clarifai.api.LabelOrderB\x04\x80\xb5\x18\x01\"v\n\x18SingleLabelOrderResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12-\n\x0blabel_order\x18\x02 \x01(\x0b\x32\x18.clarifai.api.LabelOrder\"u\n\x15PostCollectorsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12+\n\ncollectors\x18\x02 \x03(\x0b\x32\x17.clarifai.api.Collector\"\x86\x01\n\x16PatchCollectorsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12+\n\ncollectors\x18\x02 \x03(\x0b\x32\x17.clarifai.api.Collector\x12\x0e\n\x06\x61\x63tion\x18\x03 \x01(\t\"k\n\x17\x44\x65leteCollectorsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0b\n\x03ids\x18\x02 \x03(\t\x12\x12\n\ndelete_all\x18\x03 \x01(\x08\"\\\n\x13GetCollectorRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x14\n\x0c\x63ollector_id\x18\x02 \x01(\t\"h\n\x15ListCollectorsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0c\n\x04page\x18\x02 \x01(\r\x12\x10\n\x08per_page\x18\x03 \x01(\r\"r\n\x16MultiCollectorResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12+\n\ncollectors\x18\x02 \x03(\x0b\x32\x17.clarifai.api.Collector\"r\n\x17SingleCollectorResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12*\n\tcollector\x18\x02 \x01(\x0b\x32\x17.clarifai.api.Collector\"v\n\x15PostStatValuesRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12,\n\x0bstat_values\x18\x02 \x03(\x0b\x32\x17.clarifai.api.StatValue\"y\n\x16MultiStatValueResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x32\n\x0bstat_values\x18\x02 \x03(\x0b\x32\x17.clarifai.api.StatValueB\x04\x80\xb5\x18\x01\"\x9e\x01\n\x1ePostStatValuesAggregateRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12K\n\x1cstat_value_aggregate_queries\x18\x02 \x03(\x0b\x32%.clarifai.api.StatValueAggregateQuery\"\x9c\x01\n\x1fMultiStatValueAggregateResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12L\n\x1cstat_value_aggregate_results\x18\x02 \x03(\x0b\x32&.clarifai.api.StatValueAggregateResult\"w\n\x1ePostTrendingMetricsViewRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x11\n\tview_type\x18\x02 \x01(\t\x12\x11\n\tobject_id\x18\x03 \x01(\t\"\x85\x01\n\x1fListTrendingMetricsViewsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x11\n\tview_type\x18\x02 \x01(\t\x12\x0c\n\x04page\x18\x03 \x01(\r\x12\x10\n\x08per_page\x18\x04 \x01(\r\"~\n MultiTrendingMetricsViewResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12-\n\x07metrics\x18\x02 \x03(\x0b\x32\x1c.clarifai.api.TrendingMetric\"q\n\x10GetModuleRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x11\n\tmodule_id\x18\x02 \x01(\t\x12\x19\n\x11\x61\x64\x64itional_fields\x18\x03 \x03(\t\"\x96\x01\n\x12ListModulesRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0c\n\x04page\x18\x02 \x01(\r\x12\x10\n\x08per_page\x18\x03 \x01(\r\x12\x14\n\x0cstarred_only\x18\x04 \x01(\x08\x12\x19\n\x11\x61\x64\x64itional_fields\x18\x05 \x03(\t\"l\n\x12PostModulesRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12%\n\x07modules\x18\x03 \x03(\x0b\x32\x14.clarifai.api.Module\"}\n\x13PatchModulesRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12%\n\x07modules\x18\x02 \x03(\x0b\x32\x14.clarifai.api.Module\x12\x0e\n\x06\x61\x63tion\x18\x03 \x01(\t\"T\n\x14\x44\x65leteModulesRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0b\n\x03ids\x18\x02 \x03(\t\"i\n\x14SingleModuleResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12$\n\x06module\x18\x02 \x01(\x0b\x32\x14.clarifai.api.Module\"o\n\x13MultiModuleResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12+\n\x07modules\x18\x02 \x03(\x0b\x32\x14.clarifai.api.ModuleB\x04\x80\xb5\x18\x01\"x\n\x17GetModuleVersionRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x11\n\tmodule_id\x18\x02 \x01(\t\x12\x19\n\x11module_version_id\x18\x03 \x01(\t\"\x7f\n\x19ListModuleVersionsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x11\n\tmodule_id\x18\x02 \x01(\t\x12\x0c\n\x04page\x18\x03 \x01(\r\x12\x10\n\x08per_page\x18\x04 \x01(\r\"\x95\x01\n\x19PostModuleVersionsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x11\n\tmodule_id\x18\x02 \x01(\t\x12\x34\n\x0fmodule_versions\x18\x03 \x03(\x0b\x32\x1b.clarifai.api.ModuleVersion\"n\n\x1b\x44\x65leteModuleVersionsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x11\n\tmodule_id\x18\x02 \x01(\t\x12\x0b\n\x03ids\x18\x03 \x03(\t\"\x7f\n\x1bSingleModuleVersionResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x33\n\x0emodule_version\x18\x02 \x01(\x0b\x32\x1b.clarifai.api.ModuleVersion\"\x85\x01\n\x1aMultiModuleVersionResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12:\n\x0fmodule_versions\x18\x02 \x03(\x0b\x32\x1b.clarifai.api.ModuleVersionB\x04\x80\xb5\x18\x01\"x\n GetInstalledModuleVersionRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12#\n\x1binstalled_module_version_id\x18\x02 \x01(\t\"u\n\"ListInstalledModuleVersionsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0c\n\x04page\x18\x02 \x01(\r\x12\x10\n\x08per_page\x18\x03 \x01(\r\"\x9e\x01\n\"PostInstalledModuleVersionsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12G\n\x19installed_module_versions\x18\x02 \x03(\x0b\x32$.clarifai.api.InstalledModuleVersion\"}\n%PostInstalledModuleVersionsKeyRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12#\n\x1binstalled_module_version_id\x18\x02 \x01(\t\"d\n$DeleteInstalledModuleVersionsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0b\n\x03ids\x18\x02 \x03(\t\"\x9b\x01\n$SingleInstalledModuleVersionResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x46\n\x18installed_module_version\x18\x02 \x01(\x0b\x32$.clarifai.api.InstalledModuleVersion\"\xa1\x01\n#MultiInstalledModuleVersionResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12M\n\x19installed_module_versions\x18\x02 \x03(\x0b\x32$.clarifai.api.InstalledModuleVersionB\x04\x80\xb5\x18\x01\"b\n\x1eListNextTaskAssignmentsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0f\n\x07task_id\x18\x02 \x01(\t\"\x82\x01\n\x19PostBulkOperationsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x34\n\x0f\x62ulk_operations\x18\x02 \x03(\x0b\x32\x1b.clarifai.api.BulkOperation\"l\n\x19ListBulkOperationsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0c\n\x04page\x18\x02 \x01(\r\x12\x10\n\x08per_page\x18\x03 \x01(\r\"V\n\x17GetBulkOperationRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\n\n\x02id\x18\x02 \x01(\t\"Z\n\x1a\x43\x61ncelBulkOperationRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0b\n\x03ids\x18\x02 \x03(\t\"Z\n\x1a\x44\x65leteBulkOperationRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0b\n\x03ids\x18\x02 \x03(\t\"\x80\x01\n\x1cSingleBulkOperationsResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x33\n\x0e\x62ulk_operation\x18\x02 \x01(\x0b\x32\x1b.clarifai.api.BulkOperation\"\x7f\n\x1bMultiBulkOperationsResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x33\n\x0e\x62ulk_operation\x18\x02 \x03(\x0b\x32\x1b.clarifai.api.BulkOperation\"o\n\x19PutTaskAssignmentsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0f\n\x07task_id\x18\x02 \x01(\t\x12\x10\n\x08input_id\x18\x03 \x01(\t\"k\n\x18ListInputsAddJobsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0c\n\x04page\x18\x02 \x01(\r\x12\x10\n\x08per_page\x18\x03 \x01(\r\"U\n\x16GetInputsAddJobRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\n\n\x02id\x18\x02 \x01(\t\"X\n\x19\x43\x61ncelInputsAddJobRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\n\n\x02id\x18\x02 \x01(\t\"\x83\x01\n\x19MultiInputsAddJobResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x39\n\x0finputs_add_jobs\x18\x02 \x03(\x0b\x32\x1a.clarifai.api.InputsAddJobB\x04\x80\xb5\x18\x01\"}\n\x1aSingleInputsAddJobResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x32\n\x0einputs_add_job\x18\x02 \x01(\x0b\x32\x1a.clarifai.api.InputsAddJob\"l\n\x12PostUploadsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12%\n\x07uploads\x18\x02 \x03(\x0b\x32\x14.clarifai.api.Upload\"T\n\x14\x44\x65leteUploadsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0b\n\x03ids\x18\x02 \x03(\t\"e\n\x12ListUploadsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0c\n\x04page\x18\x02 \x01(\r\x12\x10\n\x08per_page\x18\x03 \x01(\r\"V\n\x10GetUploadRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x11\n\tupload_id\x18\x02 \x01(\t\"i\n\x14SingleUploadResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12$\n\x06upload\x18\x02 \x01(\x0b\x32\x14.clarifai.api.Upload\"i\n\x13MultiUploadResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12%\n\x07uploads\x18\x02 \x03(\x0b\x32\x14.clarifai.api.Upload\"\x9a\x01\n\x1cPutUploadContentPartsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x11\n\tupload_id\x18\x02 \x01(\t\x12\x36\n\rcontent_parts\x18\x03 \x03(\x0b\x32\x1f.clarifai.api.UploadContentPart\"\xad\x01\n\x1cPostInputsDataSourcesRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x34\n\x0c\x64\x61ta_sources\x18\x02 \x03(\x0b\x32\x1e.clarifai.api.InputsDataSource\x12\x15\n\rcall_back_url\x18\x03 \x01(\t\x12\x0f\n\x07\x61pp_pat\x18\x04 \x01(\t\"r\n\x1dGetInputsExtractionJobRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12 \n\x18inputs_extraction_job_id\x18\x02 \x01(\t\"r\n\x1fListInputsExtractionJobsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0c\n\x04page\x18\x02 \x01(\r\x12\x10\n\x08per_page\x18\x03 \x01(\r\"\x92\x01\n!SingleInputsExtractionJobResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12@\n\x15inputs_extraction_job\x18\x02 \x01(\x0b\x32!.clarifai.api.InputsExtractionJob\"\x92\x01\n MultiInputsExtractionJobResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x41\n\x16inputs_extraction_jobs\x18\x02 \x03(\x0b\x32!.clarifai.api.InputsExtractionJob\"a\n!CancelInputsExtractionJobsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0b\n\x03ids\x18\x02 \x03(\t\"\x7f\n\x18PostInputsUploadsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x32\n\x0einputs_uploads\x18\x02 \x03(\x0b\x32\x1a.clarifai.api.InputsUpload*p\n\x1cOrganizationInvitationStatus\x12\x0b\n\x07NOT_SET\x10\x00\x12\x0b\n\x07PENDING\x10\x01\x12\x0c\n\x08\x41\x43\x43\x45PTED\x10\x02\x12\r\n\tCANCELLED\x10\x03\x12\x0c\n\x08\x44\x45\x43LINED\x10\x04\x12\x0b\n\x07\x45XPIRED\x10\x05\x32\x8a\x83\x03\n\x02V2\x12\xae\x02\n\x14ListConceptRelations\x12).clarifai.api.ListConceptRelationsRequest\x1a*.clarifai.api.MultiConceptRelationResponse\"\xbe\x01\x82\xd3\xe4\x93\x02\xab\x01\x12Y/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/concepts/{concept_id}/relationsZN\x12L/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/concepts/relations\x98\x9c\'\x05\x90\x9c\'-\x90\x9c\'\x0b\x12\xe3\x01\n\x14PostConceptRelations\x12).clarifai.api.PostConceptRelationsRequest\x1a*.clarifai.api.MultiConceptRelationResponse\"t\x82\xd3\xe4\x93\x02^\"Y/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/concepts/{concept_id}/relations:\x01*\x98\x9c\'\x05\x90\x9c\'-\x90\x9c\'\n\x90\x9c\'\x0b\x12\xe2\x01\n\x16\x44\x65leteConceptRelations\x12+.clarifai.api.DeleteConceptRelationsRequest\x1a!.clarifai.api.status.BaseResponse\"x\x82\xd3\xe4\x93\x02^*Y/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/concepts/{concept_id}/relations:\x01*\x98\x9c\'\x05\x90\x9c\'-\x90\x9c\'\r\x90\x9c\'\n\x90\x9c\'\x0b\x12\xe0\x01\n\x10GetConceptCounts\x12%.clarifai.api.GetConceptCountsRequest\x1a\'.clarifai.api.MultiConceptCountResponse\"|\x82\xd3\xe4\x93\x02\x62\x12I/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/concepts/statusZ\x15\x12\x13/v2/concepts/status\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'&\x90\x9c\'\x0b\x90\x9c\'\x05\x12\xd5\x01\n\nGetConcept\x12\x1f.clarifai.api.GetConceptRequest\x1a#.clarifai.api.SingleConceptResponse\"\x80\x01\x82\xd3\xe4\x93\x02n\x12O/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/concepts/{concept_id}Z\x1b\x12\x19/v2/concepts/{concept_id}\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'\x0b\x12\xbd\x01\n\x0cListConcepts\x12!.clarifai.api.ListConceptsRequest\x1a\".clarifai.api.MultiConceptResponse\"f\x82\xd3\xe4\x93\x02T\x12\x42/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/conceptsZ\x0e\x12\x0c/v2/concepts\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'\x0b\x12\xbd\x02\n\x11ListModelConcepts\x12&.clarifai.api.ListModelConceptsRequest\x1a\".clarifai.api.MultiConceptResponse\"\xdb\x01\x82\xd3\xe4\x93\x02\xc4\x01\x12T/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}/conceptsZl\x12j/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}/versions/{version_id}/concepts\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'\x0b\x90\x9c\'\x0f\x12\xee\x01\n\x14PostConceptsSearches\x12).clarifai.api.PostConceptsSearchesRequest\x1a\".clarifai.api.MultiConceptResponse\"\x86\x01\x82\xd3\xe4\x93\x02l\"K/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/concepts/searches:\x01*Z\x1a\"\x15/v2/concepts/searches:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'\x0b\x90\x9c\'\x0f\x90\x9c\'\x13\x12\xc7\x01\n\x0cPostConcepts\x12!.clarifai.api.PostConceptsRequest\x1a\".clarifai.api.MultiConceptResponse\"p\x82\xd3\xe4\x93\x02Z\"B/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/concepts:\x01*Z\x11\"\x0c/v2/concepts:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'\n\x90\x9c\'\x0b\x12\xc9\x01\n\rPatchConcepts\x12\".clarifai.api.PatchConceptsRequest\x1a\".clarifai.api.MultiConceptResponse\"p\x82\xd3\xe4\x93\x02Z2B/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/concepts:\x01*Z\x11\x32\x0c/v2/concepts:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'\n\x90\x9c\'\x0b\x12\x98\x02\n\x12GetConceptLanguage\x12\'.clarifai.api.GetConceptLanguageRequest\x1a+.clarifai.api.SingleConceptLanguageResponse\"\xab\x01\x82\xd3\xe4\x93\x02\x98\x01\x12\x64/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/concepts/{concept_id}/languages/{language}Z0\x12./v2/concepts/{concept_id}/languages/{language}\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'\x0b\x12\x85\x02\n\x14ListConceptLanguages\x12).clarifai.api.ListConceptLanguagesRequest\x1a*.clarifai.api.MultiConceptLanguageResponse\"\x95\x01\x82\xd3\xe4\x93\x02\x82\x01\x12Y/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/concepts/{concept_id}/languagesZ%\x12#/v2/concepts/{concept_id}/languages\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'\x0b\x12\x8f\x02\n\x14PostConceptLanguages\x12).clarifai.api.PostConceptLanguagesRequest\x1a*.clarifai.api.MultiConceptLanguageResponse\"\x9f\x01\x82\xd3\xe4\x93\x02\x88\x01\"Y/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/concepts/{concept_id}/languages:\x01*Z(\"#/v2/concepts/{concept_id}/languages:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'\n\x90\x9c\'\x0b\x12\x91\x02\n\x15PatchConceptLanguages\x12*.clarifai.api.PatchConceptLanguagesRequest\x1a*.clarifai.api.MultiConceptLanguageResponse\"\x9f\x01\x82\xd3\xe4\x93\x02\x88\x01\x32Y/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/concepts/{concept_id}/languages:\x01*Z(2#/v2/concepts/{concept_id}/languages:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'\n\x90\x9c\'\x0b\x12\xf5\x01\n\x13ListKnowledgeGraphs\x12(.clarifai.api.ListKnowledgeGraphsRequest\x1a).clarifai.api.MultiKnowledgeGraphResponse\"\x88\x01\x82\xd3\xe4\x93\x02v\x12S/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/concepts/knowledge_graphsZ\x1f\x12\x1d/v2/concepts/knowledge_graphs\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'\x0b\x12\xff\x01\n\x13PostKnowledgeGraphs\x12(.clarifai.api.PostKnowledgeGraphsRequest\x1a).clarifai.api.MultiKnowledgeGraphResponse\"\x92\x01\x82\xd3\xe4\x93\x02|\"S/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/concepts/knowledge_graphs:\x01*Z\"\"\x1d/v2/concepts/knowledge_graphs:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'\n\x90\x9c\'\x0b\x12\x82\x02\n\x16PostConceptMappingJobs\x12+.clarifai.api.PostConceptMappingJobsRequest\x1a,.clarifai.api.MultiConceptMappingJobResponse\"\x8c\x01\x82\xd3\xe4\x93\x02v\"P/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/concepts/mappings/jobs:\x01*Z\x1f\"\x1a/v2/concepts/mappings/jobs:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'\n\x90\x9c\'\x0b\x12\x97\x02\n\rGetAnnotation\x12\".clarifai.api.GetAnnotationRequest\x1a&.clarifai.api.SingleAnnotationResponse\"\xb9\x01\x82\xd3\xe4\x93\x02\x9e\x01\x12g/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/inputs/{input_id}/annotations/{annotation_id}Z3\x12\x31/v2/inputs/{input_id}/annotations/{annotation_id}\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'&\x90\x9c\'\x0b\x90\x9c\'\x0f\x12\xd4\x01\n\x0fListAnnotations\x12$.clarifai.api.ListAnnotationsRequest\x1a%.clarifai.api.MultiAnnotationResponse\"t\x82\xd3\xe4\x93\x02Z\x12\x45/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/annotationsZ\x11\x12\x0f/v2/annotations\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'&\x90\x9c\'\x0b\x90\x9c\'\x0f\x12\xe7\x01\n\x0fPostAnnotations\x12$.clarifai.api.PostAnnotationsRequest\x1a%.clarifai.api.MultiAnnotationResponse\"\x86\x01\x82\xd3\xe4\x93\x02`\"E/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/annotations:\x01*Z\x14\"\x0f/v2/annotations:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'\x05\x90\x9c\'%\x90\x9c\'&\x90\x9c\'\x0b\x90\x9c\'\x0f\x90\x9c\'\x13\x12\xe9\x01\n\x10PatchAnnotations\x12%.clarifai.api.PatchAnnotationsRequest\x1a%.clarifai.api.MultiAnnotationResponse\"\x86\x01\x82\xd3\xe4\x93\x02`2E/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/annotations:\x01*Z\x14\x32\x0f/v2/annotations:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'\x05\x90\x9c\'%\x90\x9c\'&\x90\x9c\'\x0b\x90\x9c\'\x13\x90\x9c\'\x0f\x12\xf8\x01\n\x16PatchAnnotationsStatus\x12+.clarifai.api.PatchAnnotationsStatusRequest\x1a,.clarifai.api.PatchAnnotationsStatusResponse\"\x82\x01\x82\xd3\xe4\x93\x02`2[/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/task/{task_id}/annotations/status:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'%\x90\x9c\'&\x90\x9c\'\x0b\x90\x9c\'\x13\x90\x9c\'\x0f\x12\xa0\x02\n\x10\x44\x65leteAnnotation\x12%.clarifai.api.DeleteAnnotationRequest\x1a!.clarifai.api.status.BaseResponse\"\xc1\x01\x82\xd3\xe4\x93\x02\x9e\x01*g/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/inputs/{input_id}/annotations/{annotation_id}Z3*1/v2/inputs/{input_id}/annotations/{annotation_id}\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'%\x90\x9c\'(\x90\x9c\'&\x90\x9c\'\x13\x90\x9c\'\x0f\x12\xd4\x02\n\x11\x44\x65leteAnnotations\x12&.clarifai.api.DeleteAnnotationsRequest\x1a!.clarifai.api.status.BaseResponse\"\xf3\x01\x82\xd3\xe4\x93\x02\xd0\x01*L/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/inputs/annotations:\x01*Z\x1b*\x16/v2/inputs/annotations:\x01*ZJ*E/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/annotations:\x01*Z\x14*\x0f/v2/annotations:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'%\x90\x9c\'(\x90\x9c\'&\x90\x9c\'\x13\x90\x9c\'\x0f\x12\xf7\x01\n\x18PatchAnnotationsSearches\x12-.clarifai.api.PatchAnnotationsSearchesRequest\x1a!.clarifai.api.MultiSearchResponse\"\x88\x01\x82\xd3\xe4\x93\x02r2N/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/annotations/searches:\x01*Z\x1d\x32\x18/v2/annotations/searches:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'s\x90\x9c\'r\x12\x85\x02\n\x17PostAnnotationsSearches\x12,.clarifai.api.PostAnnotationsSearchesRequest\x1a!.clarifai.api.MultiSearchResponse\"\x98\x01\x82\xd3\xe4\x93\x02r\"N/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/annotations/searches:\x01*Z\x1d\"\x18/v2/annotations/searches:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'&\x90\x9c\'\x0b\x90\x9c\'\x05\x90\x9c\'\x0f\x90\x9c\'\x03\x90\x9c\'\x13\x12\xd5\x01\n\rGetInputCount\x12\".clarifai.api.GetInputCountRequest\x1a&.clarifai.api.SingleInputCountResponse\"x\x82\xd3\xe4\x93\x02^\x12G/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/inputs/statusZ\x13\x12\x11/v2/inputs/status\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'&\x90\x9c\'\x0b\x90\x9c\'\x05\x12\xcd\x01\n\x0cStreamInputs\x12!.clarifai.api.StreamInputsRequest\x1a .clarifai.api.MultiInputResponse\"x\x82\xd3\xe4\x93\x02^\x12G/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/inputs/streamZ\x13\x12\x11/v2/inputs/stream\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'&\x90\x9c\'\x0b\x90\x9c\'\x05\x12\x81\x02\n\x0fGetInputSamples\x12$.clarifai.api.GetInputSamplesRequest\x1a*.clarifai.api.MultiInputAnnotationResponse\"\x9b\x01\x82\xd3\xe4\x93\x02\x80\x01\x12X/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/tasks/{task_id}/inputs/samplesZ$\x12\"/v2/tasks/{task_id}/inputs/samples\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'&\x90\x9c\'\x0b\x90\x9c\'\x05\x12\xcf\x01\n\x08GetInput\x12\x1d.clarifai.api.GetInputRequest\x1a!.clarifai.api.SingleInputResponse\"\x80\x01\x82\xd3\xe4\x93\x02\x66\x12K/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/inputs/{input_id}Z\x17\x12\x15/v2/inputs/{input_id}\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'&\x90\x9c\'\x0b\x90\x9c\'\x05\x12\x80\x02\n\x15GetInputVideoManifest\x12%.clarifai.api.GetVideoManifestRequest\x1a&.clarifai.api.GetVideoManifestResponse\"\x97\x01\x82\xd3\xe4\x93\x02\x84\x01\x12Z/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/inputs/{input_id}/video_manifestZ&\x12$/v2/inputs/{input_id}/video_manifest\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'\x05\x12\xbb\x01\n\nListInputs\x12\x1f.clarifai.api.ListInputsRequest\x1a .clarifai.api.MultiInputResponse\"j\x82\xd3\xe4\x93\x02P\x12@/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/inputsZ\x0c\x12\n/v2/inputs\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'&\x90\x9c\'\x0b\x90\x9c\'\x05\x12\xd6\x01\n\nPostInputs\x12\x1f.clarifai.api.PostInputsRequest\x1a .clarifai.api.MultiInputResponse\"\x84\x01\x82\xd3\xe4\x93\x02V\"@/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/inputs:\x01*Z\x0f\"\n/v2/inputs:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'%\x90\x9c\'&\x90\x9c\'\x0b\x90\x9c\'\x04\x90\x9c\'\x05\x90\x9c\'\x0f\x90\x9c\'\x02\x90\x9c\'\x13\x12\xcf\x01\n\x0bPatchInputs\x12 .clarifai.api.PatchInputsRequest\x1a .clarifai.api.MultiInputResponse\"|\x82\xd3\xe4\x93\x02V2@/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/inputs:\x01*Z\x0f\x32\n/v2/inputs:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'%\x90\x9c\'&\x90\x9c\'\x0b\x90\x9c\'\x04\x90\x9c\'\x05\x90\x9c\'\x0f\x12\xe9\x01\n\x0b\x44\x65leteInput\x12 .clarifai.api.DeleteInputRequest\x1a!.clarifai.api.status.BaseResponse\"\x94\x01\x82\xd3\xe4\x93\x02\x66*K/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/inputs/{input_id}Z\x17*\x15/v2/inputs/{input_id}\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'%\x90\x9c\'(\x90\x9c\'&\x90\x9c\'\x04\x90\x9c\'\x08\x90\x9c\'\x05\x90\x9c\'\x0f\x90\x9c\'\x13\x12\xdb\x01\n\x0c\x44\x65leteInputs\x12!.clarifai.api.DeleteInputsRequest\x1a!.clarifai.api.status.BaseResponse\"\x84\x01\x82\xd3\xe4\x93\x02V*@/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/inputs:\x01*Z\x0f*\n/v2/inputs:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'%\x90\x9c\'(\x90\x9c\'&\x90\x9c\'\x04\x90\x9c\'\x08\x90\x9c\'\x05\x90\x9c\'\x0f\x90\x9c\'\x13\x12\xe2\x01\n\x13PatchInputsSearches\x12(.clarifai.api.PatchInputsSearchesRequest\x1a!.clarifai.api.MultiSearchResponse\"~\x82\xd3\xe4\x93\x02h2I/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/inputs/searches:\x01*Z\x18\x32\x13/v2/inputs/searches:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'s\x90\x9c\'r\x12\xf1\x01\n\x12PostInputsSearches\x12\'.clarifai.api.PostInputsSearchesRequest\x1a!.clarifai.api.MultiSearchResponse\"\x8e\x01\x82\xd3\xe4\x93\x02h\"I/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/inputs/searches:\x01*Z\x18\"\x13/v2/inputs/searches:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'&\x90\x9c\'\x0b\x90\x9c\'\x05\x90\x9c\'\x0f\x90\x9c\'\x03\x90\x9c\'\x13\x12\xa0\x03\n\x10PostModelOutputs\x12%.clarifai.api.PostModelOutputsRequest\x1a!.clarifai.api.MultiOutputResponse\"\xc1\x02\x82\xd3\xe4\x93\x02\xa6\x02\"i/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}/versions/{version_id}/outputs:\x01*Z8\"3/v2/models/{model_id}/versions/{version_id}/outputs:\x01*ZX\"S/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}/outputs:\x01*Z\"\"\x1d/v2/models/{model_id}/outputs:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'\x0b\x90\x9c\'\x0f\x90\x9c\'\x02\x12\xef\x01\n\x0cListDatasets\x12!.clarifai.api.ListDatasetsRequest\x1a\".clarifai.api.MultiDatasetResponse\"\x97\x01\x82\xd3\xe4\x93\x02\x80\x01\x12\x42/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/datasetsZ*\x12(/v2/users/{user_app_id.user_id}/datasetsZ\x0e\x12\x0c/v2/datasets\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'i\x90\x9c\'r\x12\xd9\x01\n\nGetDataset\x12\x1f.clarifai.api.GetDatasetRequest\x1a#.clarifai.api.SingleDatasetResponse\"\x84\x01\x82\xd3\xe4\x93\x02n\x12O/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/datasets/{dataset_id}Z\x1b\x12\x19/v2/datasets/{dataset_id}\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'i\x90\x9c\'r\x12\xcb\x01\n\x0cPostDatasets\x12!.clarifai.api.PostDatasetsRequest\x1a\".clarifai.api.MultiDatasetResponse\"t\x82\xd3\xe4\x93\x02Z\"B/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/datasets:\x01*Z\x11\"\x0c/v2/datasets:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'i\x90\x9c\'j\x90\x9c\'r\x12\xcd\x01\n\rPatchDatasets\x12\".clarifai.api.PatchDatasetsRequest\x1a\".clarifai.api.MultiDatasetResponse\"t\x82\xd3\xe4\x93\x02Z2B/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/datasets:\x01*Z\x11\x32\x0c/v2/datasets:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'i\x90\x9c\'j\x90\x9c\'r\x12\xce\x01\n\x0e\x44\x65leteDatasets\x12#.clarifai.api.DeleteDatasetsRequest\x1a!.clarifai.api.status.BaseResponse\"t\x82\xd3\xe4\x93\x02Z*B/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/datasets:\x01*Z\x11*\x0c/v2/datasets:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'i\x90\x9c\'j\x90\x9c\'k\x12\x81\x02\n\x11ListDatasetInputs\x12&.clarifai.api.ListDatasetInputsRequest\x1a\'.clarifai.api.MultiDatasetInputResponse\"\x9a\x01\x82\xd3\xe4\x93\x02|\x12V/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/datasets/{dataset_id}/inputsZ\"\x12 /v2/datasets/{dataset_id}/inputs\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'i\x90\x9c\'\x05\x90\x9c\'&\x90\x9c\'\x0b\x12\x95\x02\n\x0fGetDatasetInput\x12$.clarifai.api.GetDatasetInputRequest\x1a(.clarifai.api.SingleDatasetInputResponse\"\xb1\x01\x82\xd3\xe4\x93\x02\x92\x01\x12\x61/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/datasets/{dataset_id}/inputs/{input_id}Z-\x12+/v2/datasets/{dataset_id}/inputs/{input_id}\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'i\x90\x9c\'\x05\x90\x9c\'&\x90\x9c\'\x0b\x12\x8c\x02\n\x11PostDatasetInputs\x12&.clarifai.api.PostDatasetInputsRequest\x1a\'.clarifai.api.MultiDatasetInputResponse\"\xa5\x01\x82\xd3\xe4\x93\x02\x82\x01\"V/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/datasets/{dataset_id}/inputs:\x01*Z%\" /v2/datasets/{dataset_id}/inputs:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'i\x90\x9c\'j\x90\x9c\'\x05\x90\x9c\'&\x90\x9c\'\x0b\x12\x86\x02\n\x13\x44\x65leteDatasetInputs\x12(.clarifai.api.DeleteDatasetInputsRequest\x1a!.clarifai.api.status.BaseResponse\"\xa1\x01\x82\xd3\xe4\x93\x02\x82\x01*V/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/datasets/{dataset_id}/inputs:\x01*Z%* /v2/datasets/{dataset_id}/inputs:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'i\x90\x9c\'j\x90\x9c\'k\x90\x9c\'\x05\x12\x84\x02\n\x13ListDatasetVersions\x12(.clarifai.api.ListDatasetVersionsRequest\x1a).clarifai.api.MultiDatasetVersionResponse\"\x97\x01\x82\xd3\xe4\x93\x02\x80\x01\x12X/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/datasets/{dataset_id}/versionsZ$\x12\"/v2/datasets/{dataset_id}/versions\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'i\x90\x9c\'r\x12\xab\x02\n\x11GetDatasetVersion\x12&.clarifai.api.GetDatasetVersionRequest\x1a*.clarifai.api.SingleDatasetVersionResponse\"\xc1\x01\x82\xd3\xe4\x93\x02\xaa\x01\x12m/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/datasets/{dataset_id}/versions/{dataset_version_id}Z9\x12\x37/v2/datasets/{dataset_id}/versions/{dataset_version_id}\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'i\x90\x9c\'r\x12\xea\x02\n\x1fListDatasetVersionMetricsGroups\x12\x34.clarifai.api.ListDatasetVersionMetricsGroupsRequest\x1a\x35.clarifai.api.MultiDatasetVersionMetricsGroupResponse\"\xd9\x01\x82\xd3\xe4\x93\x02\xba\x01\x12u/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/datasets/{dataset_id}/versions/{dataset_version_id}/metricsZA\x12?/v2/datasets/{dataset_id}/versions/{dataset_version_id}/metrics\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'i\x90\x9c\'&\x90\x9c\'\x0b\x90\x9c\'\x05\x12\x92\x02\n\x13PostDatasetVersions\x12(.clarifai.api.PostDatasetVersionsRequest\x1a).clarifai.api.MultiDatasetVersionResponse\"\xa5\x01\x82\xd3\xe4\x93\x02\x86\x01\"X/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/datasets/{dataset_id}/versions:\x01*Z\'\"\"/v2/datasets/{dataset_id}/versions:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'i\x90\x9c\'j\x90\x9c\'\x0f\x90\x9c\'\x13\x12\x8c\x02\n\x14PatchDatasetVersions\x12).clarifai.api.PatchDatasetVersionsRequest\x1a).clarifai.api.MultiDatasetVersionResponse\"\x9d\x01\x82\xd3\xe4\x93\x02\x86\x01\x32X/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/datasets/{dataset_id}/versions:\x01*Z\'2\"/v2/datasets/{dataset_id}/versions:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'i\x90\x9c\'j\x12\x8a\x02\n\x15\x44\x65leteDatasetVersions\x12*.clarifai.api.DeleteDatasetVersionsRequest\x1a!.clarifai.api.status.BaseResponse\"\xa1\x01\x82\xd3\xe4\x93\x02\x86\x01*X/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/datasets/{dataset_id}/versions:\x01*Z\'*\"/v2/datasets/{dataset_id}/versions:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'i\x90\x9c\'j\x90\x9c\'k\x12\xd4\x02\n\x18PutDatasetVersionExports\x12-.clarifai.api.PutDatasetVersionExportsRequest\x1a/.clarifai.api.MultiDatasetVersionExportResponse\"\xd7\x01\x82\xd3\xe4\x93\x02\xc0\x01\x1au/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/datasets/{dataset_id}/versions/{dataset_version_id}/exports:\x01*ZD\x1a?/v2/datasets/{dataset_id}/versions/{dataset_version_id}/exports:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'i\x90\x9c\'j\x12\xe9\x01\n\x0cGetModelType\x12!.clarifai.api.GetModelTypeRequest\x1a%.clarifai.api.SingleModelTypeResponse\"\x8e\x01\x82\xd3\xe4\x93\x02|\x12V/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/types/{model_type_id}Z\"\x12 /v2/models/types/{model_type_id}\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'\x0f\x12\x99\x01\n\x16ListOpenSourceLicenses\x12+.clarifai.api.ListOpenSourceLicensesRequest\x1a,.clarifai.api.ListOpenSourceLicensesResponse\"$\x82\xd3\xe4\x93\x02\x1a\x12\x18/v2/open_source_licenses\x98\x9c\'\x01\x12\xcb\x01\n\x0eListModelTypes\x12#.clarifai.api.ListModelTypesRequest\x1a$.clarifai.api.MultiModelTypeResponse\"n\x82\xd3\xe4\x93\x02\\\x12\x46/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/typesZ\x12\x12\x10/v2/models/types\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'\x0f\x12\xca\x01\n\x08GetModel\x12\x1d.clarifai.api.GetModelRequest\x1a!.clarifai.api.SingleModelResponse\"|\x82\xd3\xe4\x93\x02\x66\x12K/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}Z\x17\x12\x15/v2/models/{model_id}\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'\x0b\x90\x9c\'\x0f\x12\x9a\x03\n\x12GetModelOutputInfo\x12\x1d.clarifai.api.GetModelRequest\x1a!.clarifai.api.SingleModelResponse\"\xc1\x02\x82\xd3\xe4\x93\x02\xaa\x02\x12W/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}/output_infoZ#\x12!/v2/models/{model_id}/output_infoZo\x12m/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}/versions/{version_id}/output_infoZ9\x12\x37/v2/models/{model_id}/versions/{version_id}/output_info\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'\x0b\x90\x9c\'\x0f\x12\xe2\x01\n\nListModels\x12\x1f.clarifai.api.ListModelsRequest\x1a .clarifai.api.MultiModelResponse\"\x90\x01\x82\xd3\xe4\x93\x02z\x12@/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/modelsZ(\x12&/v2/users/{user_app_id.user_id}/modelsZ\x0c\x12\n/v2/models\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'\x0b\x90\x9c\'\x0f\x12\xe7\x01\n\x11GetResourceCounts\x12&.clarifai.api.GetResourceCountsRequest\x1a\'.clarifai.api.GetResourceCountsResponse\"\x80\x01\x82\xd3\xe4\x93\x02\x62\x12I/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/resource_countsZ\x15\x12\x13/v2/resource_counts\x98\x9c\'\x02\x90\x9c\'i\x90\x9c\'\x0f\x90\x9c\'\x13\x90\x9c\'m\x90\x9c\'-\x12\xdf\x01\n\x12PostModelsSearches\x12\'.clarifai.api.PostModelsSearchesRequest\x1a .clarifai.api.MultiModelResponse\"~\x82\xd3\xe4\x93\x02h\"I/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/searches:\x01*Z\x18\"\x13/v2/models/searches:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'\x0b\x90\x9c\'\x0f\x12\xca\x01\n\nPostModels\x12\x1f.clarifai.api.PostModelsRequest\x1a!.clarifai.api.SingleModelResponse\"x\x82\xd3\xe4\x93\x02V\"@/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models:\x01*Z\x0f\"\n/v2/models:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'\x0b\x90\x9c\'\x0e\x90\x9c\'\x0f\x90\x9c\'\x1a\x90\x9c\'\x13\x12\xc7\x01\n\x0bPatchModels\x12 .clarifai.api.PatchModelsRequest\x1a .clarifai.api.MultiModelResponse\"t\x82\xd3\xe4\x93\x02V2@/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models:\x01*Z\x0f\x32\n/v2/models:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'\x0b\x90\x9c\'\x0e\x90\x9c\'\x0f\x90\x9c\'\x1a\x12\xb6\x01\n\rPatchModelIds\x12\".clarifai.api.PatchModelIdsRequest\x1a .clarifai.api.MultiModelResponse\"_\x82\xd3\xe4\x93\x02I2D/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/ids:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'\x0e\x90\x9c\'\x0f\x12\xdd\x01\n\x0b\x44\x65leteModel\x12 .clarifai.api.DeleteModelRequest\x1a!.clarifai.api.status.BaseResponse\"\x88\x01\x82\xd3\xe4\x93\x02\x66*K/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}Z\x17*\x15/v2/models/{model_id}\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'\x0b\x90\x9c\'\x0e\x90\x9c\'\x11\x90\x9c\'\x0f\x90\x9c\'\x13\x12\xce\x01\n\x0c\x44\x65leteModels\x12!.clarifai.api.DeleteModelsRequest\x1a!.clarifai.api.status.BaseResponse\"x\x82\xd3\xe4\x93\x02V*@/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models:\x01*Z\x0f*\n/v2/models:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'\x0b\x90\x9c\'\x0e\x90\x9c\'\x11\x90\x9c\'\x0f\x90\x9c\'\x13\x12\x95\x02\n\x17PatchModelCheckConsents\x12,.clarifai.api.PatchModelCheckConsentsRequest\x1a,.clarifai.api.MultiModelCheckConsentResponse\"\x9d\x01\x82\xd3\xe4\x93\x02\x8a\x01\x32Z/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}/check_consents:\x01*Z)2$/v2/models/{model_id}/check_consents:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'\x0f\x12\xf9\x01\n\x12PatchModelToolkits\x12\'.clarifai.api.PatchModelToolkitsRequest\x1a\'.clarifai.api.MultiModelToolkitResponse\"\x90\x01\x82\xd3\xe4\x93\x02~2T/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}/toolkits:\x01*Z#2\x1e/v2/models/{model_id}/toolkits:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'\x0f\x12\xf9\x01\n\x12PatchModelUseCases\x12\'.clarifai.api.PatchModelUseCasesRequest\x1a\'.clarifai.api.MultiModelUseCaseResponse\"\x90\x01\x82\xd3\xe4\x93\x02~2T/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}/usecases:\x01*Z#2\x1e/v2/models/{model_id}/usecases:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'\x0f\x12\xff\x01\n\x13PatchModelLanguages\x12(.clarifai.api.PatchModelLanguagesRequest\x1a(.clarifai.api.MultiModelLanguageResponse\"\x93\x01\x82\xd3\xe4\x93\x02\x80\x01\x32U/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}/languages:\x01*Z$2\x1f/v2/models/{model_id}/languages:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'\x0f\x12\x91\x03\n\x0fListModelInputs\x12$.clarifai.api.ListModelInputsRequest\x1a .clarifai.api.MultiInputResponse\"\xb5\x02\x82\xd3\xe4\x93\x02\x96\x02\x12R/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}/inputsZ\x1e\x12\x1c/v2/models/{model_id}/inputsZj\x12h/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}/versions/{version_id}/inputsZ4\x12\x32/v2/models/{model_id}/versions/{version_id}/inputs\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'&\x90\x9c\'\x0b\x90\x9c\'\x05\x90\x9c\'\x0f\x12\x8d\x02\n\x0fGetModelVersion\x12$.clarifai.api.GetModelVersionRequest\x1a(.clarifai.api.SingleModelVersionResponse\"\xa9\x01\x82\xd3\xe4\x93\x02\x92\x01\x12\x61/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}/versions/{version_id}Z-\x12+/v2/models/{model_id}/versions/{version_id}\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'\x0b\x90\x9c\'\x0f\x12\xf5\x01\n\x11ListModelVersions\x12&.clarifai.api.ListModelVersionsRequest\x1a\'.clarifai.api.MultiModelVersionResponse\"\x8e\x01\x82\xd3\xe4\x93\x02x\x12T/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}/versionsZ \x12\x1e/v2/models/{model_id}/versions\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'\x0b\x90\x9c\'\x0f\x12\xbc\x02\n\x1dPostWorkflowVersionsUnPublish\x12\x32.clarifai.api.PostWorkflowVersionsUnPublishRequest\x1a!.clarifai.api.status.BaseResponse\"\xc3\x01\x82\xd3\xe4\x93\x02\x8c\x01\"[/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/workflows/{workflow_id}/unpublish:\x01*Z*\"%/v2/workflows/{workflow_id}/unpublish:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'x\x90\x9c\'&\x90\x9c\'\x0b\x90\x9c\'\x05\x90\x9c\'\x0e\x90\x9c\'\x0f\x90\x9c\'\x1a\x90\x9c\'\x13\x90\x9c\'5\x90\x9c\'6\x12\xb4\x02\n\x1bPostWorkflowVersionsPublish\x12\x30.clarifai.api.PostWorkflowVersionsPublishRequest\x1a!.clarifai.api.status.BaseResponse\"\xbf\x01\x82\xd3\xe4\x93\x02\x88\x01\"Y/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/workflows/{workflow_id}/publish:\x01*Z(\"#/v2/workflows/{workflow_id}/publish:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'w\x90\x9c\'&\x90\x9c\'\x0b\x90\x9c\'\x05\x90\x9c\'\x0e\x90\x9c\'\x0f\x90\x9c\'\x1a\x90\x9c\'\x13\x90\x9c\'5\x90\x9c\'6\x12\xa1\x02\n\x18PostModelVersionsPublish\x12-.clarifai.api.PostModelVersionsPublishRequest\x1a!.clarifai.api.status.BaseResponse\"\xb2\x01\x82\xd3\xe4\x93\x02|\"S/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}/publish:\x01*Z\"\"\x1d/v2/models/{model_id}/publish:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'u\x90\x9c\'&\x90\x9c\'\x0b\x90\x9c\'\x05\x90\x9c\'\x0e\x90\x9c\'\x0f\x90\x9c\'\x1a\x90\x9c\'\x13\x90\x9c\'5\x90\x9c\'6\x12\xaa\x02\n\x1aPostModelVersionsUnPublish\x12/.clarifai.api.PostModelVersionsUnPublishRequest\x1a!.clarifai.api.status.BaseResponse\"\xb7\x01\x82\xd3\xe4\x93\x02\x80\x01\"U/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}/unpublish:\x01*Z$\"\x1f/v2/models/{model_id}/unpublish:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'v\x90\x9c\'&\x90\x9c\'\x0b\x90\x9c\'\x05\x90\x9c\'\x0e\x90\x9c\'\x0f\x90\x9c\'\x1a\x90\x9c\'\x13\x90\x9c\'5\x90\x9c\'6\x12\x91\x02\n\x11PostModelVersions\x12&.clarifai.api.PostModelVersionsRequest\x1a!.clarifai.api.SingleModelResponse\"\xb0\x01\x82\xd3\xe4\x93\x02~\"T/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}/versions:\x01*Z#\"\x1e/v2/models/{model_id}/versions:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'&\x90\x9c\'\x0b\x90\x9c\'\x05\x90\x9c\'\x0e\x90\x9c\'\x0f\x90\x9c\'\x1a\x90\x9c\'\x13\x90\x9c\'5\x90\x9c\'6\x12\xdf\x01\n\x12PatchModelVersions\x12\'.clarifai.api.PatchModelVersionsRequest\x1a\'.clarifai.api.MultiModelVersionResponse\"w\x82\xd3\xe4\x93\x02Y2T/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}/versions:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'\x0b\x90\x9c\'\x0f\x90\x9c\'\x0e\x90\x9c\'\x1a\x12\x98\x02\n\x12\x44\x65leteModelVersion\x12\'.clarifai.api.DeleteModelVersionRequest\x1a!.clarifai.api.status.BaseResponse\"\xb5\x01\x82\xd3\xe4\x93\x02\x92\x01*a/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}/versions/{version_id}Z-*+/v2/models/{model_id}/versions/{version_id}\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'\x0b\x90\x9c\'\x0e\x90\x9c\'\x11\x90\x9c\'\x0f\x90\x9c\'\x13\x12\xb7\x02\n\x16GetModelVersionMetrics\x12+.clarifai.api.GetModelVersionMetricsRequest\x1a(.clarifai.api.SingleModelVersionResponse\"\xc5\x01\x82\xd3\xe4\x93\x02\xa2\x01\x12i/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}/versions/{version_id}/metricsZ5\x12\x33/v2/models/{model_id}/versions/{version_id}/metrics\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'&\x90\x9c\'\x0b\x90\x9c\'\x0f\x90\x9c\'\x05\x90\x9c\'5\x12\xd3\x02\n\x17PostModelVersionMetrics\x12,.clarifai.api.PostModelVersionMetricsRequest\x1a(.clarifai.api.SingleModelVersionResponse\"\xdf\x01\x82\xd3\xe4\x93\x02\xa8\x01\"i/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}/versions/{version_id}/metrics:\x01*Z8\"3/v2/models/{model_id}/versions/{version_id}/metrics:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'&\x90\x9c\'\x0b\x90\x9c\'\x05\x90\x9c\'\x0e\x90\x9c\'\x0f\x90\x9c\'\x1a\x90\x9c\'\x02\x90\x9c\'\x13\x90\x9c\'5\x90\x9c\'6\x12\xed\x02\n\x1bPostModelVersionEvaluations\x12\x30.clarifai.api.PostModelVersionEvaluationsRequest\x1a&.clarifai.api.MultiEvalMetricsResponse\"\xf3\x01\x82\xd3\xe4\x93\x02\xbc\x01\"s/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}/versions/{model_version_id}/evaluations:\x01*ZB\"=/v2/models/{model_id}/versions/{model_version_id}/evaluations:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'&\x90\x9c\'\x0b\x90\x9c\'\x05\x90\x9c\'\x0e\x90\x9c\'\x0f\x90\x9c\'\x1a\x90\x9c\'\x02\x90\x9c\'\x13\x90\x9c\'5\x90\x9c\'6\x12\xd3\x02\n\x1bListModelVersionEvaluations\x12\x30.clarifai.api.ListModelVersionEvaluationsRequest\x1a&.clarifai.api.MultiEvalMetricsResponse\"\xd9\x01\x82\xd3\xe4\x93\x02\xb6\x01\x12s/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}/versions/{model_version_id}/evaluationsZ?\x12=/v2/models/{model_id}/versions/{model_version_id}/evaluations\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'&\x90\x9c\'\x0b\x90\x9c\'\x0f\x90\x9c\'\x05\x90\x9c\'5\x12\xf1\x02\n\x19GetModelVersionEvaluation\x12..clarifai.api.GetModelVersionEvaluationRequest\x1a\'.clarifai.api.SingleEvalMetricsResponse\"\xfa\x01\x82\xd3\xe4\x93\x02\xd7\x01\x12\x83\x01/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}/versions/{model_version_id}/evaluations/{evaluation_id}ZO\x12M/v2/models/{model_id}/versions/{model_version_id}/evaluations/{evaluation_id}\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'&\x90\x9c\'\x0b\x90\x9c\'\x0f\x90\x9c\'\x05\x90\x9c\'5\x12\xf8\x01\n\x0fPostEvaluations\x12$.clarifai.api.PostEvaluationsRequest\x1a&.clarifai.api.MultiEvalMetricsResponse\"\x96\x01\x82\xd3\xe4\x93\x02`\"E/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/evaluations:\x01*Z\x14\"\x0f/v2/evaluations:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'&\x90\x9c\'\x0b\x90\x9c\'\x05\x90\x9c\'\x0e\x90\x9c\'\x0f\x90\x9c\'\x1a\x90\x9c\'\x02\x90\x9c\'\x13\x90\x9c\'5\x90\x9c\'6\x12\xdd\x01\n\x0fListEvaluations\x12$.clarifai.api.ListEvaluationsRequest\x1a&.clarifai.api.MultiEvalMetricsResponse\"|\x82\xd3\xe4\x93\x02Z\x12\x45/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/evaluationsZ\x11\x12\x0f/v2/evaluations\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'&\x90\x9c\'\x0b\x90\x9c\'\x0f\x90\x9c\'\x05\x90\x9c\'5\x12\xfb\x01\n\rGetEvaluation\x12\".clarifai.api.GetEvaluationRequest\x1a\'.clarifai.api.SingleEvalMetricsResponse\"\x9c\x01\x82\xd3\xe4\x93\x02z\x12U/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/evaluations/{evaluation_id}Z!\x12\x1f/v2/evaluations/{evaluation_id}\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'&\x90\x9c\'\x0b\x90\x9c\'\x0f\x90\x9c\'\x05\x90\x9c\'5\x12\xfb\x01\n\x13ListModelReferences\x12(.clarifai.api.ListModelReferencesRequest\x1a).clarifai.api.MultiModelReferenceResponse\"\x8e\x01\x82\xd3\xe4\x93\x02|\x12V/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}/referencesZ\"\x12 /v2/models/{model_id}/references\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'\x0f\x12\xf2\x02\n\x1bGetModelVersionInputExample\x12\x30.clarifai.api.GetModelVersionInputExampleRequest\x1a\x34.clarifai.api.SingleModelVersionInputExampleResponse\"\xea\x01\x82\xd3\xe4\x93\x02\xd7\x01\x12\x83\x01/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}/versions/{model_version_id}/input_examples/{example_id}ZO\x12M/v2/models/{model_id}/versions/{model_version_id}/input_examples/{example_id}\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'\x0f\x12\xda\x02\n\x1dListModelVersionInputExamples\x12\x32.clarifai.api.ListModelVersionInputExamplesRequest\x1a\x33.clarifai.api.MultiModelVersionInputExampleResponse\"\xcf\x01\x82\xd3\xe4\x93\x02\xbc\x01\x12v/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}/versions/{model_version_id}/input_examplesZB\x12@/v2/models/{model_id}/versions/{model_version_id}/input_examples\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'\x0f\x12\xe0\x01\n\x0bGetWorkflow\x12 .clarifai.api.GetWorkflowRequest\x1a$.clarifai.api.SingleWorkflowResponse\"\x88\x01\x82\xd3\xe4\x93\x02r\x12Q/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/workflows/{workflow_id}Z\x1d\x12\x1b/v2/workflows/{workflow_id}\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'\x0f\x90\x9c\'\x13\x12\xf5\x01\n\rListWorkflows\x12\".clarifai.api.ListWorkflowsRequest\x1a#.clarifai.api.MultiWorkflowResponse\"\x9a\x01\x82\xd3\xe4\x93\x02\x83\x01\x12\x43/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/workflowsZ+\x12)/v2/users/{user_app_id.user_id}/workflowsZ\x0f\x12\r/v2/workflows\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'\x0f\x90\x9c\'\x13\x12\xd0\x01\n\rPostWorkflows\x12\".clarifai.api.PostWorkflowsRequest\x1a#.clarifai.api.MultiWorkflowResponse\"v\x82\xd3\xe4\x93\x02\\\"C/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/workflows:\x01*Z\x12\"\r/v2/workflows:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'\x0f\x90\x9c\'\x12\x90\x9c\'\x13\x12\xd2\x01\n\x0ePatchWorkflows\x12#.clarifai.api.PatchWorkflowsRequest\x1a#.clarifai.api.MultiWorkflowResponse\"v\x82\xd3\xe4\x93\x02\\2C/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/workflows:\x01*Z\x12\x32\r/v2/workflows:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'\x0f\x90\x9c\'\x12\x90\x9c\'\x13\x12\xc2\x01\n\x10PatchWorkflowIds\x12%.clarifai.api.PatchWorkflowIdsRequest\x1a#.clarifai.api.MultiWorkflowResponse\"b\x82\xd3\xe4\x93\x02L2G/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/workflows/ids:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'\x12\x90\x9c\'\x13\x12\xe7\x01\n\x0e\x44\x65leteWorkflow\x12#.clarifai.api.DeleteWorkflowRequest\x1a!.clarifai.api.status.BaseResponse\"\x8c\x01\x82\xd3\xe4\x93\x02r*Q/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/workflows/{workflow_id}Z\x1d*\x1b/v2/workflows/{workflow_id}\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'\x12\x90\x9c\'\x15\x90\x9c\'\x13\x12\xd2\x01\n\x0f\x44\x65leteWorkflows\x12$.clarifai.api.DeleteWorkflowsRequest\x1a!.clarifai.api.status.BaseResponse\"v\x82\xd3\xe4\x93\x02\\*C/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/workflows:\x01*Z\x12*\r/v2/workflows:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'\x12\x90\x9c\'\x15\x90\x9c\'\x13\x12\x8a\x03\n\x13PostWorkflowResults\x12(.clarifai.api.PostWorkflowResultsRequest\x1a).clarifai.api.PostWorkflowResultsResponse\"\x9d\x02\x82\xd3\xe4\x93\x02\xfe\x01\"o/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/workflows/{workflow_id}/versions/{version_id}/results:\x01*Z^\"Y/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/workflows/{workflow_id}/results:\x01*Z(\"#/v2/workflows/{workflow_id}/results:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'\x0f\x90\x9c\'\x0b\x90\x9c\'\x02\x90\x9c\'\x13\x12\xc9\x03\n\x1dPostWorkflowResultsSimilarity\x12\x32.clarifai.api.PostWorkflowResultsSimilarityRequest\x1a\x33.clarifai.api.PostWorkflowResultsSimilarityResponse\"\xbe\x02\x82\xd3\xe4\x93\x02\x9f\x02\"z/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/workflows/{workflow_id}/versions/{version_id}/results/similarity:\x01*Zi\"d/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/workflows/{workflow_id}/results/similarity:\x01*Z3\"./v2/workflows/{workflow_id}/results/similarity:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'\x0f\x90\x9c\'\x0b\x90\x9c\'\x02\x90\x9c\'\x13\x12\x8b\x02\n\x14ListWorkflowVersions\x12).clarifai.api.ListWorkflowVersionsRequest\x1a*.clarifai.api.MultiWorkflowVersionResponse\"\x9b\x01\x82\xd3\xe4\x93\x02\x84\x01\x12Z/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/workflows/{workflow_id}/versionsZ&\x12$/v2/workflows/{workflow_id}/versions\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'\x0f\x90\x9c\'\x13\x12\xb4\x02\n\x12GetWorkflowVersion\x12\'.clarifai.api.GetWorkflowVersionRequest\x1a+.clarifai.api.SingleWorkflowVersionResponse\"\xc7\x01\x82\xd3\xe4\x93\x02\xb0\x01\x12p/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/workflows/{workflow_id}/versions/{workflow_version_id}Z<\x12:/v2/workflows/{workflow_id}/versions/{workflow_version_id}\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'\x0f\x90\x9c\'\x13\x12\x90\x02\n\x16\x44\x65leteWorkflowVersions\x12+.clarifai.api.DeleteWorkflowVersionsRequest\x1a!.clarifai.api.status.BaseResponse\"\xa5\x01\x82\xd3\xe4\x93\x02\x8a\x01*Z/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/workflows/{workflow_id}/versions:\x01*Z)*$/v2/workflows/{workflow_id}/versions:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'\x13\x90\x9c\'\x12\x90\x9c\'\x15\x12\x97\x02\n\x15PatchWorkflowVersions\x12*.clarifai.api.PatchWorkflowVersionsRequest\x1a*.clarifai.api.MultiWorkflowVersionResponse\"\xa5\x01\x82\xd3\xe4\x93\x02\x8a\x01\x32Z/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/workflows/{workflow_id}/versions:\x01*Z)2$/v2/workflows/{workflow_id}/versions:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'\x0f\x90\x9c\'\x13\x90\x9c\'\x12\x12\x85\x01\n\x06GetKey\x12\x1b.clarifai.api.GetKeyRequest\x1a\x1f.clarifai.api.SingleKeyResponse\"=\x82\xd3\xe4\x93\x02/\x12-/v2/users/{user_app_id.user_id}/keys/{key_id}\x98\x9c\'\x05\x90\x9c\'0\x12\x7f\n\x08ListKeys\x12\x1d.clarifai.api.ListKeysRequest\x1a\x1e.clarifai.api.MultiKeyResponse\"4\x82\xd3\xe4\x93\x02&\x12$/v2/users/{user_app_id.user_id}/keys\x98\x9c\'\x05\x90\x9c\'0\x12\xa3\x01\n\x0bListAppKeys\x12 .clarifai.api.ListAppKeysRequest\x1a\x1e.clarifai.api.MultiKeyResponse\"R\x82\xd3\xe4\x93\x02@\x12>/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/keys\x98\x9c\'\x05\x90\x9c\'-\x90\x9c\'0\x12\x95\x01\n\tDeleteKey\x12\x1e.clarifai.api.DeleteKeyRequest\x1a!.clarifai.api.status.BaseResponse\"E\x82\xd3\xe4\x93\x02/*-/v2/users/{user_app_id.user_id}/keys/{key_id}\x98\x9c\'\x05\x90\x9c\'/\x90\x9c\'1\x90\x9c\'0\x12\x8a\x01\n\x08PostKeys\x12\x1d.clarifai.api.PostKeysRequest\x1a\x1e.clarifai.api.MultiKeyResponse\"?\x82\xd3\xe4\x93\x02)\"$/v2/users/{user_app_id.user_id}/keys:\x01*\x98\x9c\'\x05\x90\x9c\'-\x90\x9c\'/\x90\x9c\'0\x12\x88\x01\n\tPatchKeys\x12\x1e.clarifai.api.PatchKeysRequest\x1a\x1e.clarifai.api.MultiKeyResponse\";\x82\xd3\xe4\x93\x02)2$/v2/users/{user_app_id.user_id}/keys:\x01*\x98\x9c\'\x05\x90\x9c\'/\x90\x9c\'0\x12\xbc\x01\n\x08MyScopes\x12\x1d.clarifai.api.MyScopesRequest\x1a .clarifai.api.MultiScopeResponse\"o\x82\xd3\xe4\x93\x02\x65\x12\x42/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/myscopesZ\x0e\x12\x0c/v2/myscopesZ\x0f\x12\r/v2/my_scopes\x98\x9c\'\x02\x12\x8d\x01\n\x0cMyScopesUser\x12!.clarifai.api.MyScopesUserRequest\x1a$.clarifai.api.MultiScopeUserResponse\"4\x82\xd3\xe4\x93\x02*\x12(/v2/users/{user_app_id.user_id}/myscopes\x98\x9c\'\x05\x12u\n\x0cMyScopesRoot\x12!.clarifai.api.MyScopesRootRequest\x1a$.clarifai.api.MultiScopeRootResponse\"\x1c\x82\xd3\xe4\x93\x02\x12\x12\x10/v2/myscopesroot\x98\x9c\'\x05\x12\x87\x01\n\nListScopes\x12\x1f.clarifai.api.ListScopesRequest\x1a$.clarifai.api.MultiScopeDepsResponse\"2\x82\xd3\xe4\x93\x02(\x12&/v2/users/{user_app_id.user_id}/scopes\x98\x9c\'\x03\x12\x95\x01\n\x06GetApp\x12\x1b.clarifai.api.GetAppRequest\x1a\x1f.clarifai.api.SingleAppResponse\"M\x82\xd3\xe4\x93\x02;\x12\x39/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}\x98\x9c\'\x05\x90\x9c\'-\x90\x9c\'\x13\x12\x8f\x01\n\x08ListApps\x12\x1d.clarifai.api.ListAppsRequest\x1a\x1e.clarifai.api.MultiAppResponse\"D\x82\xd3\xe4\x93\x02\x32\x12$/v2/users/{user_app_id.user_id}/appsZ\n\x12\x08/v2/apps\x98\x9c\'\x05\x90\x9c\'-\x90\x9c\'\x13\x12\xa5\x01\n\tDeleteApp\x12\x1e.clarifai.api.DeleteAppRequest\x1a!.clarifai.api.status.BaseResponse\"U\x82\xd3\xe4\x93\x02;*9/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}\x98\x9c\'\x05\x90\x9c\',\x90\x9c\'.\x90\x9c\'-\x90\x9c\'\x13\x12\x92\x01\n\x08PostApps\x12\x1d.clarifai.api.PostAppsRequest\x1a\x1e.clarifai.api.MultiAppResponse\"G\x82\xd3\xe4\x93\x02)\"$/v2/users/{user_app_id.user_id}/apps:\x01*\x98\x9c\'\x05\x90\x9c\',\x90\x9c\'-\x90\x9c\'\x0f\x90\x9c\'\x13\x90\x9c\'\x12\x12\x88\x01\n\tPatchApps\x12\x1e.clarifai.api.PatchAppsRequest\x1a\x1e.clarifai.api.MultiAppResponse\";\x82\xd3\xe4\x93\x02)2$/v2/users/{user_app_id.user_id}/apps:\x01*\x98\x9c\'\x05\x90\x9c\',\x90\x9c\'-\x12\x92\x01\n\x0cPatchAppsIds\x12!.clarifai.api.PatchAppsIdsRequest\x1a\x1e.clarifai.api.MultiAppResponse\"?\x82\xd3\xe4\x93\x02-2(/v2/users/{user_app_id.user_id}/apps/ids:\x01*\x98\x9c\'\x05\x90\x9c\',\x90\x9c\'-\x12\x9c\x01\n\x08PatchApp\x12\x1d.clarifai.api.PatchAppRequest\x1a\x1f.clarifai.api.SingleAppResponse\"P\x82\xd3\xe4\x93\x02>29/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}:\x01*\x98\x9c\'\x05\x90\x9c\',\x90\x9c\'-\x12\x9f\x01\n\x10PostAppsSearches\x12%.clarifai.api.PostAppsSearchesRequest\x1a\x1e.clarifai.api.MultiAppResponse\"D\x82\xd3\xe4\x93\x02\x32\"-/v2/users/{user_app_id.user_id}/apps/searches:\x01*\x98\x9c\'\x05\x90\x9c\'-\x90\x9c\'\x13\x12v\n\x07GetUser\x12\x1c.clarifai.api.GetUserRequest\x1a .clarifai.api.SingleUserResponse\"+\x82\xd3\xe4\x93\x02!\x12\x1f/v2/users/{user_app_id.user_id}\x98\x9c\'\x05\x12\xcf\x01\n\x14PostValidatePassword\x12).clarifai.api.PostValidatePasswordRequest\x1a..clarifai.api.SinglePasswordValidationResponse\"\\\x82\xd3\xe4\x93\x02R\"1/v2/users/{user_app_id.user_id}/validate_password:\x01*Z\x1a\"\x15/v2/validate_password:\x01*\x98\x9c\'\x03\x12\xc1\x01\n\tGetSearch\x12\x1e.clarifai.api.GetSearchRequest\x1a\".clarifai.api.SingleSearchResponse\"p\x82\xd3\xe4\x93\x02^\x12G/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/searches/{id}Z\x13\x12\x11/v2/searches/{id}\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'r\x12\xbc\x01\n\x0cListSearches\x12!.clarifai.api.ListSearchesRequest\x1a!.clarifai.api.MultiSearchResponse\"f\x82\xd3\xe4\x93\x02T\x12\x42/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/searchesZ\x0e\x12\x0c/v2/searches\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'r\x12\xc8\x01\n\rPatchSearches\x12\".clarifai.api.PatchSearchesRequest\x1a!.clarifai.api.MultiSearchResponse\"p\x82\xd3\xe4\x93\x02Z2B/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/searches:\x01*Z\x11\x32\x0c/v2/searches:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'s\x90\x9c\'r\x12\xda\x01\n\x0cPostSearches\x12!.clarifai.api.PostSearchesRequest\x1a!.clarifai.api.MultiSearchResponse\"\x83\x01\x88\x02\x01\x82\xd3\xe4\x93\x02Z\"B/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/searches:\x01*Z\x11\"\x0c/v2/searches:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'&\x90\x9c\'\x0b\x90\x9c\'\x05\x90\x9c\'\x0f\x90\x9c\'\x03\x90\x9c\'\x13\x12\xd8\x01\n\x10PostSearchesByID\x12%.clarifai.api.PostSearchesByIDRequest\x1a!.clarifai.api.MultiSearchResponse\"z\x82\xd3\xe4\x93\x02\x64\"G/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/searches/{id}:\x01*Z\x16\"\x11/v2/searches/{id}:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'r\x90\x9c\'\x03\x12\xb3\x02\n\x1bPostAnnotationSearchMetrics\x12\x30.clarifai.api.PostAnnotationSearchMetricsRequest\x1a\x32.clarifai.api.MultiAnnotationSearchMetricsResponse\"\xad\x01\x82\xd3\xe4\x93\x02\x82\x01\"V/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/annotations/searches/metrics:\x01*Z%\" /v2/annotations/searches/metrics:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'&\x90\x9c\'\x0b\x90\x9c\'\x05\x90\x9c\'5\x90\x9c\'6\x90\x9c\'\x0f\x90\x9c\'\x13\x12\xa9\x02\n\x1aGetAnnotationSearchMetrics\x12/.clarifai.api.GetAnnotationSearchMetricsRequest\x1a\x32.clarifai.api.MultiAnnotationSearchMetricsResponse\"\xa5\x01\x82\xd3\xe4\x93\x02\x86\x01\x12[/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/annotations/searches/metrics/{id}Z\'\x12%/v2/annotations/searches/metrics/{id}\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'&\x90\x9c\'\x0b\x90\x9c\'\x05\x90\x9c\'5\x12\xa0\x02\n\x1bListAnnotationSearchMetrics\x12\x30.clarifai.api.ListAnnotationSearchMetricsRequest\x1a\x32.clarifai.api.MultiAnnotationSearchMetricsResponse\"\x9a\x01\x82\xd3\xe4\x93\x02|\x12V/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/annotations/searches/metricsZ\"\x12 /v2/annotations/searches/metrics\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'&\x90\x9c\'\x0b\x90\x9c\'\x05\x90\x9c\'5\x12\x9a\x02\n\x1d\x44\x65leteAnnotationSearchMetrics\x12\x32.clarifai.api.DeleteAnnotationSearchMetricsRequest\x1a!.clarifai.api.status.BaseResponse\"\xa1\x01\x82\xd3\xe4\x93\x02\x86\x01*[/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/annotations/searches/metrics/{id}Z\'*%/v2/annotations/searches/metrics/{id}\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'5\x90\x9c\'6\x90\x9c\'?\x12\xce\x01\n\x0c\x44\x65leteSearch\x12!.clarifai.api.DeleteSearchRequest\x1a!.clarifai.api.status.BaseResponse\"x\x82\xd3\xe4\x93\x02^*G/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/searches/{id}Z\x13*\x11/v2/searches/{id}\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'r\x90\x9c\'s\x90\x9c\'t\x12\xec\x01\n\x15ListAnnotationFilters\x12*.clarifai.api.ListAnnotationFiltersRequest\x1a+.clarifai.api.MultiAnnotationFilterResponse\"z\x82\xd3\xe4\x93\x02h\x12L/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/annotation_filtersZ\x18\x12\x16/v2/annotation_filters\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'r\x12\x99\x02\n\x13GetAnnotationFilter\x12(.clarifai.api.GetAnnotationFilterRequest\x1a,.clarifai.api.SingleAnnotationFilterResponse\"\xa9\x01\x82\xd3\xe4\x93\x02\x96\x01\x12\x63/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/annotation_filters/{annotation_filter_id}Z/\x12-/v2/annotation_filters/{annotation_filter_id}\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'r\x12\xf7\x01\n\x15PostAnnotationFilters\x12*.clarifai.api.PostAnnotationFiltersRequest\x1a+.clarifai.api.MultiAnnotationFilterResponse\"\x84\x01\x82\xd3\xe4\x93\x02n\"L/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/annotation_filters:\x01*Z\x1b\"\x16/v2/annotation_filters:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'r\x90\x9c\'s\x12\xf9\x01\n\x16PatchAnnotationFilters\x12+.clarifai.api.PatchAnnotationFiltersRequest\x1a+.clarifai.api.MultiAnnotationFilterResponse\"\x84\x01\x82\xd3\xe4\x93\x02n2L/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/annotation_filters:\x01*Z\x1b\x32\x16/v2/annotation_filters:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'r\x90\x9c\'s\x12\xf1\x01\n\x17\x44\x65leteAnnotationFilters\x12,.clarifai.api.DeleteAnnotationFiltersRequest\x1a!.clarifai.api.status.BaseResponse\"\x84\x01\x82\xd3\xe4\x93\x02n*L/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/annotation_filters:\x01*Z\x1b*\x16/v2/annotation_filters:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'r\x90\x9c\'s\x12|\n\x0fListStatusCodes\x12$.clarifai.api.ListStatusCodesRequest\x1a%.clarifai.api.MultiStatusCodeResponse\"\x1c\x82\xd3\xe4\x93\x02\x12\x12\x10/v2/status_codes\x98\x9c\'\x01\x12\x8a\x01\n\rGetStatusCode\x12\".clarifai.api.GetStatusCodeRequest\x1a&.clarifai.api.SingleStatusCodeResponse\"-\x82\xd3\xe4\x93\x02#\x12!/v2/status_codes/{status_code_id}\x98\x9c\'\x01\x12\xc2\x01\n\x11ListCollaborators\x12&.clarifai.api.ListCollaboratorsRequest\x1a(.clarifai.api.MultiCollaboratorsResponse\"[\x82\xd3\xe4\x93\x02I\x12G/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/collaborators\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'2\x12\xc9\x01\n\x11PostCollaborators\x12&.clarifai.api.PostCollaboratorsRequest\x1a(.clarifai.api.MultiCollaboratorsResponse\"b\x82\xd3\xe4\x93\x02L\"G/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/collaborators:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'3\x90\x9c\'2\x12\xcf\x01\n\x12PatchCollaborators\x12\'.clarifai.api.PatchCollaboratorsRequest\x1a(.clarifai.api.MultiCollaboratorsResponse\"f\x82\xd3\xe4\x93\x02L2G/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/collaborators:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'3\x90\x9c\'2\x90\x9c\'4\x12\xd2\x01\n\x13\x44\x65leteCollaborators\x12(.clarifai.api.DeleteCollaboratorsRequest\x1a!.clarifai.api.status.BaseResponse\"n\x82\xd3\xe4\x93\x02L*G/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/collaborators:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'3\x90\x9c\'2\x90\x9c\'4\x90\x9c\'7\x90\x9c\'8\x12\xa4\x01\n\x12ListCollaborations\x12\'.clarifai.api.ListCollaborationsRequest\x1a).clarifai.api.MultiCollaborationsResponse\":\x82\xd3\xe4\x93\x02\x30\x12./v2/users/{user_app_id.user_id}/collaborations\x98\x9c\'\x03\x12\xf3\x01\n\x13PostAppDuplications\x12(.clarifai.api.PostAppDuplicationsRequest\x1a*.clarifai.api.MultiAppDuplicationsResponse\"\x85\x01\x82\xd3\xe4\x93\x02K\"F/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/duplications:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'\x0e\x90\x9c\'\x0f\x90\x9c\'\x1a\x90\x9c\'\n\x90\x9c\'\x0b\x90\x9c\'\x04\x90\x9c\'\x05\x90\x9c\'%\x90\x9c\'&\x90\x9c\'\x12\x90\x9c\'\x13\x12\xa5\x01\n\x13ListAppDuplications\x12(.clarifai.api.ListAppDuplicationsRequest\x1a*.clarifai.api.MultiAppDuplicationsResponse\"8\x82\xd3\xe4\x93\x02.\x12,/v2/users/{user_app_id.user_id}/duplications\x98\x9c\'\x05\x12\xb6\x01\n\x11GetAppDuplication\x12&.clarifai.api.GetAppDuplicationRequest\x1a*.clarifai.api.SingleAppDuplicationResponse\"M\x82\xd3\xe4\x93\x02\x43\x12\x41/v2/users/{user_app_id.user_id}/duplications/{app_duplication_id}\x98\x9c\'\x05\x12\xd9\x01\n\tPostTasks\x12\x1e.clarifai.api.PostTasksRequest\x1a\x1f.clarifai.api.MultiTaskResponse\"\x8a\x01\x82\xd3\xe4\x93\x02T\"?/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/tasks:\x01*Z\x0e\"\t/v2/tasks:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'7\x90\x9c\'8\x90\x9c\'\x05\x90\x9c\'\x03\x90\x9c\'r\x90\x9c\'\x0b\x90\x9c\'\x13\x90\x9c\'\x0f\x90\x9c\'%\x90\x9c\'&\x12\xfe\x01\n\x16GetTaskAnnotationCount\x12!.clarifai.api.GetTaskCountRequest\x1a%.clarifai.api.SingleTaskCountResponse\"\x99\x01\x82\xd3\xe4\x93\x02\x86\x01\x12[/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/tasks/{task_id}/annotations/countZ\'\x12%/v2/tasks/{task_id}/annotations/count\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'8\x12\xee\x01\n\x11GetTaskInputCount\x12!.clarifai.api.GetTaskCountRequest\x1a%.clarifai.api.SingleTaskCountResponse\"\x8e\x01\x82\xd3\xe4\x93\x02|\x12V/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/tasks/{task_id}/inputs/countZ\"\x12 /v2/tasks/{task_id}/inputs/count\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'8\x12\xd0\x01\n\x07GetTask\x12\x1c.clarifai.api.GetTaskRequest\x1a .clarifai.api.SingleTaskResponse\"\x84\x01\x82\xd3\xe4\x93\x02\x62\x12I/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/tasks/{task_id}Z\x15\x12\x13/v2/tasks/{task_id}\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'8\x90\x9c\'r\x90\x9c\'\x0b\x90\x9c\'\x13\x90\x9c\'\x0f\x12\xbe\x01\n\tListTasks\x12\x1e.clarifai.api.ListTasksRequest\x1a\x1f.clarifai.api.MultiTaskResponse\"p\x82\xd3\xe4\x93\x02N\x12?/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/tasksZ\x0b\x12\t/v2/tasks\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'8\x90\x9c\'r\x90\x9c\'\x0b\x90\x9c\'\x13\x90\x9c\'\x0f\x12\xd7\x01\n\nPatchTasks\x12\x1f.clarifai.api.PatchTasksRequest\x1a\x1f.clarifai.api.MultiTaskResponse\"\x86\x01\x82\xd3\xe4\x93\x02T2?/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/tasks:\x01*Z\x0e\x32\t/v2/tasks:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'7\x90\x9c\'8\x90\x9c\'\x05\x90\x9c\'r\x90\x9c\'\x0b\x90\x9c\'\x13\x90\x9c\'\x0f\x90\x9c\'%\x90\x9c\'&\x12\xc2\x01\n\x0b\x44\x65leteTasks\x12 .clarifai.api.DeleteTasksRequest\x1a!.clarifai.api.status.BaseResponse\"n\x82\xd3\xe4\x93\x02T*?/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/tasks:\x01*Z\x0e*\t/v2/tasks:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'7\x90\x9c\'8\x90\x9c\'F\x12\xf5\x01\n\x0fPostLabelOrders\x12$.clarifai.api.PostLabelOrdersRequest\x1a%.clarifai.api.MultiLabelOrderResponse\"\x94\x01\x82\xd3\xe4\x93\x02\x62\"F/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/label_orders:\x01*Z\x15\"\x10/v2/label_orders:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'C\x90\x9c\'D\x90\x9c\'7\x90\x9c\'8\x90\x9c\'\x05\x90\x9c\'r\x90\x9c\'\x0b\x90\x9c\'\x13\x90\x9c\'\x0f\x12\xf6\x01\n\rGetLabelOrder\x12\".clarifai.api.GetLabelOrderRequest\x1a&.clarifai.api.SingleLabelOrderResponse\"\x98\x01\x82\xd3\xe4\x93\x02~\x12W/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/label_orders/{label_order_id}Z#\x12!/v2/label_orders/{label_order_id}\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'C\x90\x9c\'\x0b\x90\x9c\'8\x12\xd6\x01\n\x0fListLabelOrders\x12$.clarifai.api.ListLabelOrdersRequest\x1a%.clarifai.api.MultiLabelOrderResponse\"v\x82\xd3\xe4\x93\x02\\\x12\x46/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/label_ordersZ\x12\x12\x10/v2/label_orders\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'C\x90\x9c\'\x0b\x90\x9c\'8\x12\xeb\x01\n\x10PatchLabelOrders\x12%.clarifai.api.PatchLabelOrdersRequest\x1a%.clarifai.api.MultiLabelOrderResponse\"\x88\x01\x82\xd3\xe4\x93\x02\x62\x32\x46/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/label_orders:\x01*Z\x15\x32\x10/v2/label_orders:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'C\x90\x9c\'D\x90\x9c\'\x0b\x90\x9c\'7\x90\x9c\'8\x90\x9c\'F\x12\xe5\x01\n\x11\x44\x65leteLabelOrders\x12&.clarifai.api.DeleteLabelOrdersRequest\x1a!.clarifai.api.status.BaseResponse\"\x84\x01\x82\xd3\xe4\x93\x02\x62*F/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/label_orders:\x01*Z\x15*\x10/v2/label_orders:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'E\x90\x9c\'C\x90\x9c\'D\x90\x9c\'7\x90\x9c\'8\x12\xf2\x01\n\x0ePostCollectors\x12#.clarifai.api.PostCollectorsRequest\x1a$.clarifai.api.MultiCollectorResponse\"\x94\x01\x82\xd3\xe4\x93\x02^\"D/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/collectors:\x01*Z\x13\"\x0e/v2/collectors:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'\x04\x90\x9c\'%\x90\x9c\'&\x90\x9c\')\x90\x9c\'\x0b\x90\x9c\'\x04\x90\x9c\'\x05\x90\x9c\'\x0f\x90\x9c\'\x02\x90\x9c\'\x13\x12\xe3\x01\n\x0cGetCollector\x12!.clarifai.api.GetCollectorRequest\x1a%.clarifai.api.SingleCollectorResponse\"\x88\x01\x82\xd3\xe4\x93\x02v\x12S/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/collectors/{collector_id}Z\x1f\x12\x1d/v2/collectors/{collector_id}\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'*\x12\xc7\x01\n\x0eListCollectors\x12#.clarifai.api.ListCollectorsRequest\x1a$.clarifai.api.MultiCollectorResponse\"j\x82\xd3\xe4\x93\x02X\x12\x44/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/collectorsZ\x10\x12\x0e/v2/collectors\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'*\x12\xd3\x01\n\x0fPatchCollectors\x12$.clarifai.api.PatchCollectorsRequest\x1a$.clarifai.api.MultiCollectorResponse\"t\x82\xd3\xe4\x93\x02^2D/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/collectors:\x01*Z\x13\x32\x0e/v2/collectors:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\')\x90\x9c\'*\x12\xd6\x01\n\x10\x44\x65leteCollectors\x12%.clarifai.api.DeleteCollectorsRequest\x1a!.clarifai.api.status.BaseResponse\"x\x82\xd3\xe4\x93\x02^*D/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/collectors:\x01*Z\x13*\x0e/v2/collectors:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\')\x90\x9c\'+\x90\x9c\'*\x12\xc9\x01\n\x0ePostStatValues\x12#.clarifai.api.PostStatValuesRequest\x1a$.clarifai.api.MultiStatValueResponse\"l\x82\xd3\xe4\x93\x02\x62\"F/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/stats/values:\x01*Z\x15\"\x10/v2/stats/values:\x01*\x98\x9c\'\x02\x12\xfd\x01\n\x17PostStatValuesAggregate\x12,.clarifai.api.PostStatValuesAggregateRequest\x1a-.clarifai.api.MultiStatValueAggregateResponse\"\x84\x01\x82\xd3\xe4\x93\x02v\"P/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/stats/values/aggregate:\x01*Z\x1f\"\x1a/v2/stats/values/aggregate:\x01*\x98\x9c\'\x02\x90\x9c\'-\x12\xe3\x01\n\x17PostTrendingMetricsView\x12,.clarifai.api.PostTrendingMetricsViewRequest\x1a!.clarifai.api.status.BaseResponse\"w\x82\xd3\xe4\x93\x02m\"h/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/trending_metrics/views/{view_type}/{object_id}:\x01*\x98\x9c\'\x02\x12\x8f\x02\n\x18ListTrendingMetricsViews\x12-.clarifai.api.ListTrendingMetricsViewsRequest\x1a..clarifai.api.MultiTrendingMetricsViewResponse\"\x93\x01\x82\xd3\xe4\x93\x02\x88\x01\x12\\/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/trending_metrics/views/{view_type}Z(\x12&/v2/trending_metrics/views/{view_type}\x98\x9c\'\x02\x12\xb2\x01\n\tGetModule\x12\x1e.clarifai.api.GetModuleRequest\x1a\".clarifai.api.SingleModuleResponse\"a\x82\xd3\xe4\x93\x02O\x12M/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/modules/{module_id}\x98\x9c\'\x05\x90\x9c\'-\x90\x9c\'m\x12\xe4\x01\n\x0bListModules\x12 .clarifai.api.ListModulesRequest\x1a!.clarifai.api.MultiModuleResponse\"\x8f\x01\x82\xd3\xe4\x93\x02}\x12\x41/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/modulesZ)\x12\'/v2/users/{user_app_id.user_id}/modulesZ\r\x12\x0b/v2/modules\x98\x9c\'\x05\x90\x9c\'-\x90\x9c\'m\x12\xb0\x01\n\x0bPostModules\x12 .clarifai.api.PostModulesRequest\x1a!.clarifai.api.MultiModuleResponse\"\\\x82\xd3\xe4\x93\x02\x46\"A/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/modules:\x01*\x98\x9c\'\x05\x90\x9c\'-\x90\x9c\'l\x90\x9c\'m\x12\xb2\x01\n\x0cPatchModules\x12!.clarifai.api.PatchModulesRequest\x1a!.clarifai.api.MultiModuleResponse\"\\\x82\xd3\xe4\x93\x02\x46\x32\x41/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/modules:\x01*\x98\x9c\'\x05\x90\x9c\'-\x90\x9c\'l\x90\x9c\'m\x12\xd0\x01\n\rDeleteModules\x12\".clarifai.api.DeleteModulesRequest\x1a!.clarifai.api.status.BaseResponse\"x\x82\xd3\xe4\x93\x02\x46*A/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/modules:\x01*\x98\x9c\'\x05\x90\x9c\'-\x90\x9c\'l\x90\x9c\'n\x90\x9c\'m\x90\x9c\'p\x90\x9c\'o\x90\x9c\'q\x90\x9c\'1\x90\x9c\'0\x90\x9c\'/\x12\xe4\x01\n\x10GetModuleVersion\x12%.clarifai.api.GetModuleVersionRequest\x1a).clarifai.api.SingleModuleVersionResponse\"~\x82\xd3\xe4\x93\x02l\x12j/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/modules/{module_id}/versions/{module_version_id}\x98\x9c\'\x05\x90\x9c\'-\x90\x9c\'m\x12\xd3\x01\n\x12ListModuleVersions\x12\'.clarifai.api.ListModuleVersionsRequest\x1a(.clarifai.api.MultiModuleVersionResponse\"j\x82\xd3\xe4\x93\x02X\x12V/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/modules/{module_id}/versions\x98\x9c\'\x05\x90\x9c\'-\x90\x9c\'m\x12\xda\x01\n\x12PostModuleVersions\x12\'.clarifai.api.PostModuleVersionsRequest\x1a(.clarifai.api.MultiModuleVersionResponse\"q\x82\xd3\xe4\x93\x02[\"V/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/modules/{module_id}/versions:\x01*\x98\x9c\'\x05\x90\x9c\'-\x90\x9c\'l\x90\x9c\'m\x12\xf4\x01\n\x14\x44\x65leteModuleVersions\x12).clarifai.api.DeleteModuleVersionsRequest\x1a!.clarifai.api.status.BaseResponse\"\x8d\x01\x82\xd3\xe4\x93\x02[*V/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/modules/{module_id}/versions:\x01*\x98\x9c\'\x05\x90\x9c\'-\x90\x9c\'l\x90\x9c\'n\x90\x9c\'m\x90\x9c\'p\x90\x9c\'o\x90\x9c\'q\x90\x9c\'1\x90\x9c\'0\x90\x9c\'/\x12\x8f\x02\n\x19GetInstalledModuleVersion\x12..clarifai.api.GetInstalledModuleVersionRequest\x1a\x32.clarifai.api.SingleInstalledModuleVersionResponse\"\x8d\x01\x82\xd3\xe4\x93\x02s\x12q/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/installed_module_versions/{installed_module_version_id}\x98\x9c\'\x05\x90\x9c\'-\x90\x9c\'p\x90\x9c\'m\x90\x9c\'0\x12\xf3\x01\n\x1bListInstalledModuleVersions\x12\x30.clarifai.api.ListInstalledModuleVersionsRequest\x1a\x31.clarifai.api.MultiInstalledModuleVersionResponse\"o\x82\xd3\xe4\x93\x02U\x12S/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/installed_module_versions\x98\x9c\'\x05\x90\x9c\'-\x90\x9c\'p\x90\x9c\'m\x90\x9c\'0\x12\xf6\x01\n\x1bPostInstalledModuleVersions\x12\x30.clarifai.api.PostInstalledModuleVersionsRequest\x1a\x31.clarifai.api.MultiInstalledModuleVersionResponse\"r\x82\xd3\xe4\x93\x02X\"S/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/installed_module_versions:\x01*\x98\x9c\'\x05\x90\x9c\'o\x90\x9c\'p\x90\x9c\'m\x90\x9c\'-\x12\xfb\x01\n\x1d\x44\x65leteInstalledModuleVersions\x12\x32.clarifai.api.DeleteInstalledModuleVersionsRequest\x1a!.clarifai.api.status.BaseResponse\"\x82\x01\x82\xd3\xe4\x93\x02X*S/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/installed_module_versions:\x01*\x98\x9c\'\x05\x90\x9c\'-\x90\x9c\'m\x90\x9c\'o\x90\x9c\'p\x90\x9c\'q\x90\x9c\'1\x90\x9c\'/\x90\x9c\'0\x12\x95\x02\n\x1ePostInstalledModuleVersionsKey\x12\x33.clarifai.api.PostInstalledModuleVersionsKeyRequest\x1a\x1f.clarifai.api.SingleKeyResponse\"\x9c\x01\x82\xd3\xe4\x93\x02z\"u/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/installed_module_versions/{installed_module_version_id}/key:\x01*\x98\x9c\'\x05\x90\x9c\'o\x90\x9c\'p\x90\x9c\'m\x90\x9c\'-\x90\x9c\'/\x90\x9c\'0\x12\xf5\x01\n\x12PostBulkOperations\x12\'.clarifai.api.PostBulkOperationsRequest\x1a).clarifai.api.MultiBulkOperationsResponse\"\x8a\x01\x82\xd3\xe4\x93\x02h\"I/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/bulk_operations:\x01*Z\x18\"\x13/v2/bulk_operations:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'z\x90\x9c\'y\x90\x9c\'%\x90\x9c\'&\x90\x9c\'(\x12\xde\x01\n\x12ListBulkOperations\x12\'.clarifai.api.ListBulkOperationsRequest\x1a).clarifai.api.MultiBulkOperationsResponse\"t\x82\xd3\xe4\x93\x02\x62\x12I/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/bulk_operationsZ\x15\x12\x13/v2/bulk_operations\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'z\x12\xe5\x01\n\x10GetBulkOperation\x12%.clarifai.api.GetBulkOperationRequest\x1a*.clarifai.api.SingleBulkOperationsResponse\"~\x82\xd3\xe4\x93\x02l\x12N/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/bulk_operations/{id}Z\x1a\x12\x18/v2/bulk_operations/{id}\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'z\x12\xeb\x01\n\x14\x43\x61ncelBulkOperations\x12(.clarifai.api.CancelBulkOperationRequest\x1a).clarifai.api.MultiBulkOperationsResponse\"~\x82\xd3\xe4\x93\x02h2I/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/bulk_operations:\x01*Z\x18\x32\x13/v2/bulk_operations:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'y\x90\x9c\'z\x12\xf4\x01\n\x14\x44\x65leteBulkOperations\x12(.clarifai.api.DeleteBulkOperationRequest\x1a!.clarifai.api.status.BaseResponse\"\x8e\x01\x82\xd3\xe4\x93\x02h*I/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/bulk_operations:\x01*Z\x18*\x13/v2/bulk_operations:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'&\x90\x9c\'%\x90\x9c\'(\x90\x9c\'y\x90\x9c\'z\x90\x9c\'{\x12\xb2\x02\n\x1cGetDatasetInputsSearchAddJob\x12\x31.clarifai.api.GetDatasetInputsSearchAddJobRequest\x1a\x35.clarifai.api.SingleDatasetInputsSearchAddJobResponse\"\xa7\x01\x82\xd3\xe4\x93\x02\x94\x01\x12\x62/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/datasets/inputs/search_add/jobs/{job_id}Z.\x12,/v2/datasets/inputs/search_add/jobs/{job_id}\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'i\x12\x88\x02\n\x17ListNextTaskAssignments\x12,.clarifai.api.ListNextTaskAssignmentsRequest\x1a .clarifai.api.MultiInputResponse\"\x9c\x01\x82\xd3\xe4\x93\x02z\x12U/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/tasks/{task_id}/assignmentsZ!\x12\x1f/v2/tasks/{task_id}/assignments\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'&\x90\x9c\'\x0b\x90\x9c\'\x05\x90\x9c\'8\x90\x9c\'i\x12\xe3\x01\n\x12PutTaskAssignments\x12\'.clarifai.api.PutTaskAssignmentsRequest\x1a!.clarifai.api.status.BaseResponse\"\x80\x01\x82\xd3\xe4\x93\x02Z\x1aU/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/tasks/{task_id}/assignments:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'%\x90\x9c\'&\x90\x9c\'\x0b\x90\x9c\'\x05\x90\x9c\'8\x90\x9c\'i\x12\xda\x01\n\x11ListInputsAddJobs\x12&.clarifai.api.ListInputsAddJobsRequest\x1a\'.clarifai.api.MultiInputsAddJobResponse\"t\x82\xd3\xe4\x93\x02\x62\x12I/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/inputs/jobs/addZ\x15\x12\x13/v2/inputs/jobs/add\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'\x05\x12\xe1\x01\n\x0fGetInputsAddJob\x12$.clarifai.api.GetInputsAddJobRequest\x1a(.clarifai.api.SingleInputsAddJobResponse\"~\x82\xd3\xe4\x93\x02l\x12N/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/inputs/jobs/add/{id}Z\x1a\x12\x18/v2/inputs/jobs/add/{id}\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'\x05\x12\xf2\x01\n\x12\x43\x61ncelInputsAddJob\x12\'.clarifai.api.CancelInputsAddJobRequest\x1a(.clarifai.api.SingleInputsAddJobResponse\"\x88\x01\x82\xd3\xe4\x93\x02r2N/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/inputs/jobs/add/{id}:\x01*Z\x1d\x32\x18/v2/inputs/jobs/add/{id}:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'\x04\x90\x9c\'\x05\x12\xc4\x01\n\x0bPostUploads\x12 .clarifai.api.PostUploadsRequest\x1a!.clarifai.api.MultiUploadResponse\"p\x82\xd3\xe4\x93\x02X\"A/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/uploads:\x01*Z\x10\"\x0b/v2/uploads:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'\x81\x01\x90\x9c\'\x80\x01\x12\x8c\x02\n\x15PutUploadContentParts\x12*.clarifai.api.PutUploadContentPartsRequest\x1a\".clarifai.api.SingleUploadResponse\"\xa2\x01\x82\xd3\xe4\x93\x02\x89\x01\x1a[/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/uploads/{upload_id}/content_parts:\x01*Z\'\x1a%/v2/uploads/{upload_id}/content_parts\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'\x81\x01\x90\x9c\'\x80\x01\x12\xce\x01\n\tGetUpload\x12\x1e.clarifai.api.GetUploadRequest\x1a\".clarifai.api.SingleUploadResponse\"}\x82\xd3\xe4\x93\x02j\x12M/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/uploads/{upload_id}Z\x19\x12\x17/v2/uploads/{upload_id}\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'\x80\x01\x12\xb9\x01\n\x0bListUploads\x12 .clarifai.api.ListUploadsRequest\x1a!.clarifai.api.MultiUploadResponse\"e\x82\xd3\xe4\x93\x02R\x12\x41/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/uploadsZ\r\x12\x0b/v2/uploads\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'\x80\x01\x12\xcd\x01\n\rDeleteUploads\x12\".clarifai.api.DeleteUploadsRequest\x1a!.clarifai.api.status.BaseResponse\"u\x82\xd3\xe4\x93\x02X*A/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/uploads:\x01*Z\x10*\x0b/v2/uploads:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'\x80\x01\x90\x9c\'\x81\x01\x90\x9c\'\x82\x01\x12\x8d\x02\n\x15PostInputsDataSources\x12*.clarifai.api.PostInputsDataSourcesRequest\x1a\'.clarifai.api.MultiInputsAddJobResponse\"\x9e\x01\x82\xd3\xe4\x93\x02p\"M/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/inputs/data_sources:\x01*Z\x1c\"\x17/v2/inputs/data_sources:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'%\x90\x9c\'&\x90\x9c\'\x0b\x90\x9c\'\x04\x90\x9c\'\x05\x90\x9c\'\x0f\x90\x9c\'\x02\x90\x9c\'\x13\x12\xb2\x02\n\x16GetInputsExtractionJob\x12+.clarifai.api.GetInputsExtractionJobRequest\x1a/.clarifai.api.SingleInputsExtractionJobResponse\"\xb9\x01\x82\xd3\xe4\x93\x02\xa6\x01\x12k/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/inputs/jobs/extraction/{inputs_extraction_job_id}Z7\x12\x35/v2/inputs/jobs/extraction/{inputs_extraction_job_id}\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'\x05\x12\xfe\x01\n\x18ListInputsExtractionJobs\x12-.clarifai.api.ListInputsExtractionJobsRequest\x1a..clarifai.api.MultiInputsExtractionJobResponse\"\x82\x01\x82\xd3\xe4\x93\x02p\x12P/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/inputs/jobs/extractionZ\x1c\x12\x1a/v2/inputs/jobs/extraction\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'\x05\x12\x8c\x02\n\x1a\x43\x61ncelInputsExtractionJobs\x12/.clarifai.api.CancelInputsExtractionJobsRequest\x1a..clarifai.api.MultiInputsExtractionJobResponse\"\x8c\x01\x82\xd3\xe4\x93\x02v2P/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/inputs/jobs/extraction:\x01*Z\x1f\x32\x1a/v2/inputs/jobs/extraction:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'\x04\x90\x9c\'\x05\x12\x85\x02\n\x11PostInputsUploads\x12&.clarifai.api.PostInputsUploadsRequest\x1a\'.clarifai.api.MultiInputsAddJobResponse\"\x9e\x01\x82\xd3\xe4\x93\x02\x66\"H/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/inputs/uploads:\x01*Z\x17\"\x12/v2/inputs/uploads:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'%\x90\x9c\'&\x90\x9c\'\x0b\x90\x9c\'\x04\x90\x9c\'\x05\x90\x9c\'\x0f\x90\x9c\'\x02\x90\x9c\'\x13\x90\x9c\'\x81\x01\x90\x9c\'\x80\x01\x42Y\n\x15\x63om.clarifai.grpc.apiP\x01Z7github.com/Clarifai/clarifai-go-grpc/proto/clarifai/api\xa2\x02\x04\x43\x41IPb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'proto.clarifai.api.service_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\025com.clarifai.grpc.apiP\001Z7github.com/Clarifai/clarifai-go-grpc/proto/clarifai/api\242\002\004CAIP'
@@ -102,225 +102,231 @@
   _MULTIMODULEVERSIONRESPONSE.fields_by_name['module_versions']._options = None
   _MULTIMODULEVERSIONRESPONSE.fields_by_name['module_versions']._serialized_options = b'\200\265\030\001'
   _MULTIINSTALLEDMODULEVERSIONRESPONSE.fields_by_name['installed_module_versions']._options = None
   _MULTIINSTALLEDMODULEVERSIONRESPONSE.fields_by_name['installed_module_versions']._serialized_options = b'\200\265\030\001'
   _MULTIINPUTSADDJOBRESPONSE.fields_by_name['inputs_add_jobs']._options = None
   _MULTIINPUTSADDJOBRESPONSE.fields_by_name['inputs_add_jobs']._serialized_options = b'\200\265\030\001'
   _V2.methods_by_name['ListConceptRelations']._options = None
-  _V2.methods_by_name['ListConceptRelations']._serialized_options = b'\202\323\344\223\002\253\001\022Y/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/concepts/{concept_id}/relationsZN\022L/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/concepts/relations\230\234\'\005\220\234\'\013'
+  _V2.methods_by_name['ListConceptRelations']._serialized_options = b'\202\323\344\223\002\253\001\022Y/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/concepts/{concept_id}/relationsZN\022L/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/concepts/relations\230\234\'\005\220\234\'-\220\234\'\013'
   _V2.methods_by_name['PostConceptRelations']._options = None
-  _V2.methods_by_name['PostConceptRelations']._serialized_options = b'\202\323\344\223\002^\"Y/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/concepts/{concept_id}/relations:\001*\230\234\'\005\220\234\'\n\220\234\'\013'
+  _V2.methods_by_name['PostConceptRelations']._serialized_options = b'\202\323\344\223\002^\"Y/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/concepts/{concept_id}/relations:\001*\230\234\'\005\220\234\'-\220\234\'\n\220\234\'\013'
   _V2.methods_by_name['DeleteConceptRelations']._options = None
-  _V2.methods_by_name['DeleteConceptRelations']._serialized_options = b'\202\323\344\223\002^*Y/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/concepts/{concept_id}/relations:\001*\230\234\'\005\220\234\'\r\220\234\'\n\220\234\'\013'
+  _V2.methods_by_name['DeleteConceptRelations']._serialized_options = b'\202\323\344\223\002^*Y/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/concepts/{concept_id}/relations:\001*\230\234\'\005\220\234\'-\220\234\'\r\220\234\'\n\220\234\'\013'
   _V2.methods_by_name['GetConceptCounts']._options = None
-  _V2.methods_by_name['GetConceptCounts']._serialized_options = b'\202\323\344\223\002b\022I/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/concepts/statusZ\025\022\023/v2/concepts/status\230\234\'\002\220\234\'&\220\234\'\013\220\234\'\005'
+  _V2.methods_by_name['GetConceptCounts']._serialized_options = b'\202\323\344\223\002b\022I/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/concepts/statusZ\025\022\023/v2/concepts/status\230\234\'\002\220\234\'-\220\234\'&\220\234\'\013\220\234\'\005'
   _V2.methods_by_name['GetConcept']._options = None
-  _V2.methods_by_name['GetConcept']._serialized_options = b'\202\323\344\223\002n\022O/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/concepts/{concept_id}Z\033\022\031/v2/concepts/{concept_id}\230\234\'\002\220\234\'\013'
+  _V2.methods_by_name['GetConcept']._serialized_options = b'\202\323\344\223\002n\022O/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/concepts/{concept_id}Z\033\022\031/v2/concepts/{concept_id}\230\234\'\002\220\234\'-\220\234\'\013'
   _V2.methods_by_name['ListConcepts']._options = None
-  _V2.methods_by_name['ListConcepts']._serialized_options = b'\202\323\344\223\002T\022B/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/conceptsZ\016\022\014/v2/concepts\230\234\'\002\220\234\'\013'
+  _V2.methods_by_name['ListConcepts']._serialized_options = b'\202\323\344\223\002T\022B/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/conceptsZ\016\022\014/v2/concepts\230\234\'\002\220\234\'-\220\234\'\013'
   _V2.methods_by_name['ListModelConcepts']._options = None
-  _V2.methods_by_name['ListModelConcepts']._serialized_options = b'\202\323\344\223\002\304\001\022T/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}/conceptsZl\022j/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}/versions/{version_id}/concepts\230\234\'\002\220\234\'\013\220\234\'\017'
+  _V2.methods_by_name['ListModelConcepts']._serialized_options = b'\202\323\344\223\002\304\001\022T/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}/conceptsZl\022j/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}/versions/{version_id}/concepts\230\234\'\002\220\234\'-\220\234\'\013\220\234\'\017'
   _V2.methods_by_name['PostConceptsSearches']._options = None
-  _V2.methods_by_name['PostConceptsSearches']._serialized_options = b'\202\323\344\223\002l\"K/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/concepts/searches:\001*Z\032\"\025/v2/concepts/searches:\001*\230\234\'\002\220\234\'\013\220\234\'\017\220\234\'\023'
+  _V2.methods_by_name['PostConceptsSearches']._serialized_options = b'\202\323\344\223\002l\"K/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/concepts/searches:\001*Z\032\"\025/v2/concepts/searches:\001*\230\234\'\002\220\234\'-\220\234\'\013\220\234\'\017\220\234\'\023'
   _V2.methods_by_name['PostConcepts']._options = None
-  _V2.methods_by_name['PostConcepts']._serialized_options = b'\202\323\344\223\002Z\"B/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/concepts:\001*Z\021\"\014/v2/concepts:\001*\230\234\'\002\220\234\'\n\220\234\'\013'
+  _V2.methods_by_name['PostConcepts']._serialized_options = b'\202\323\344\223\002Z\"B/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/concepts:\001*Z\021\"\014/v2/concepts:\001*\230\234\'\002\220\234\'-\220\234\'\n\220\234\'\013'
   _V2.methods_by_name['PatchConcepts']._options = None
-  _V2.methods_by_name['PatchConcepts']._serialized_options = b'\202\323\344\223\002Z2B/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/concepts:\001*Z\0212\014/v2/concepts:\001*\230\234\'\002\220\234\'\n\220\234\'\013'
+  _V2.methods_by_name['PatchConcepts']._serialized_options = b'\202\323\344\223\002Z2B/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/concepts:\001*Z\0212\014/v2/concepts:\001*\230\234\'\002\220\234\'-\220\234\'\n\220\234\'\013'
   _V2.methods_by_name['GetConceptLanguage']._options = None
-  _V2.methods_by_name['GetConceptLanguage']._serialized_options = b'\202\323\344\223\002\230\001\022d/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/concepts/{concept_id}/languages/{language}Z0\022./v2/concepts/{concept_id}/languages/{language}\230\234\'\002\220\234\'\013'
+  _V2.methods_by_name['GetConceptLanguage']._serialized_options = b'\202\323\344\223\002\230\001\022d/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/concepts/{concept_id}/languages/{language}Z0\022./v2/concepts/{concept_id}/languages/{language}\230\234\'\002\220\234\'-\220\234\'\013'
   _V2.methods_by_name['ListConceptLanguages']._options = None
-  _V2.methods_by_name['ListConceptLanguages']._serialized_options = b'\202\323\344\223\002\202\001\022Y/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/concepts/{concept_id}/languagesZ%\022#/v2/concepts/{concept_id}/languages\230\234\'\002\220\234\'\013'
+  _V2.methods_by_name['ListConceptLanguages']._serialized_options = b'\202\323\344\223\002\202\001\022Y/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/concepts/{concept_id}/languagesZ%\022#/v2/concepts/{concept_id}/languages\230\234\'\002\220\234\'-\220\234\'\013'
   _V2.methods_by_name['PostConceptLanguages']._options = None
-  _V2.methods_by_name['PostConceptLanguages']._serialized_options = b'\202\323\344\223\002\210\001\"Y/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/concepts/{concept_id}/languages:\001*Z(\"#/v2/concepts/{concept_id}/languages:\001*\230\234\'\002\220\234\'\n\220\234\'\013'
+  _V2.methods_by_name['PostConceptLanguages']._serialized_options = b'\202\323\344\223\002\210\001\"Y/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/concepts/{concept_id}/languages:\001*Z(\"#/v2/concepts/{concept_id}/languages:\001*\230\234\'\002\220\234\'-\220\234\'\n\220\234\'\013'
   _V2.methods_by_name['PatchConceptLanguages']._options = None
-  _V2.methods_by_name['PatchConceptLanguages']._serialized_options = b'\202\323\344\223\002\210\0012Y/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/concepts/{concept_id}/languages:\001*Z(2#/v2/concepts/{concept_id}/languages:\001*\230\234\'\002\220\234\'\n\220\234\'\013'
+  _V2.methods_by_name['PatchConceptLanguages']._serialized_options = b'\202\323\344\223\002\210\0012Y/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/concepts/{concept_id}/languages:\001*Z(2#/v2/concepts/{concept_id}/languages:\001*\230\234\'\002\220\234\'-\220\234\'\n\220\234\'\013'
   _V2.methods_by_name['ListKnowledgeGraphs']._options = None
-  _V2.methods_by_name['ListKnowledgeGraphs']._serialized_options = b'\202\323\344\223\002v\022S/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/concepts/knowledge_graphsZ\037\022\035/v2/concepts/knowledge_graphs\230\234\'\002\220\234\'\013'
+  _V2.methods_by_name['ListKnowledgeGraphs']._serialized_options = b'\202\323\344\223\002v\022S/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/concepts/knowledge_graphsZ\037\022\035/v2/concepts/knowledge_graphs\230\234\'\002\220\234\'-\220\234\'\013'
   _V2.methods_by_name['PostKnowledgeGraphs']._options = None
-  _V2.methods_by_name['PostKnowledgeGraphs']._serialized_options = b'\202\323\344\223\002|\"S/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/concepts/knowledge_graphs:\001*Z\"\"\035/v2/concepts/knowledge_graphs:\001*\230\234\'\002\220\234\'\n\220\234\'\013'
+  _V2.methods_by_name['PostKnowledgeGraphs']._serialized_options = b'\202\323\344\223\002|\"S/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/concepts/knowledge_graphs:\001*Z\"\"\035/v2/concepts/knowledge_graphs:\001*\230\234\'\002\220\234\'-\220\234\'\n\220\234\'\013'
   _V2.methods_by_name['PostConceptMappingJobs']._options = None
-  _V2.methods_by_name['PostConceptMappingJobs']._serialized_options = b'\202\323\344\223\002v\"P/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/concepts/mappings/jobs:\001*Z\037\"\032/v2/concepts/mappings/jobs:\001*\230\234\'\002\220\234\'\n\220\234\'\013'
+  _V2.methods_by_name['PostConceptMappingJobs']._serialized_options = b'\202\323\344\223\002v\"P/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/concepts/mappings/jobs:\001*Z\037\"\032/v2/concepts/mappings/jobs:\001*\230\234\'\002\220\234\'-\220\234\'\n\220\234\'\013'
   _V2.methods_by_name['GetAnnotation']._options = None
-  _V2.methods_by_name['GetAnnotation']._serialized_options = b'\202\323\344\223\002\236\001\022g/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/inputs/{input_id}/annotations/{annotation_id}Z3\0221/v2/inputs/{input_id}/annotations/{annotation_id}\230\234\'\002\220\234\'&\220\234\'\013\220\234\'\017'
+  _V2.methods_by_name['GetAnnotation']._serialized_options = b'\202\323\344\223\002\236\001\022g/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/inputs/{input_id}/annotations/{annotation_id}Z3\0221/v2/inputs/{input_id}/annotations/{annotation_id}\230\234\'\002\220\234\'-\220\234\'&\220\234\'\013\220\234\'\017'
   _V2.methods_by_name['ListAnnotations']._options = None
-  _V2.methods_by_name['ListAnnotations']._serialized_options = b'\202\323\344\223\002Z\022E/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/annotationsZ\021\022\017/v2/annotations\230\234\'\002\220\234\'&\220\234\'\013\220\234\'\017'
+  _V2.methods_by_name['ListAnnotations']._serialized_options = b'\202\323\344\223\002Z\022E/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/annotationsZ\021\022\017/v2/annotations\230\234\'\002\220\234\'-\220\234\'&\220\234\'\013\220\234\'\017'
   _V2.methods_by_name['PostAnnotations']._options = None
-  _V2.methods_by_name['PostAnnotations']._serialized_options = b'\202\323\344\223\002`\"E/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/annotations:\001*Z\024\"\017/v2/annotations:\001*\230\234\'\002\220\234\'\005\220\234\'%\220\234\'&\220\234\'\013\220\234\'\017\220\234\'\023'
+  _V2.methods_by_name['PostAnnotations']._serialized_options = b'\202\323\344\223\002`\"E/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/annotations:\001*Z\024\"\017/v2/annotations:\001*\230\234\'\002\220\234\'-\220\234\'\005\220\234\'%\220\234\'&\220\234\'\013\220\234\'\017\220\234\'\023'
   _V2.methods_by_name['PatchAnnotations']._options = None
-  _V2.methods_by_name['PatchAnnotations']._serialized_options = b'\202\323\344\223\002`2E/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/annotations:\001*Z\0242\017/v2/annotations:\001*\230\234\'\002\220\234\'\005\220\234\'%\220\234\'&\220\234\'\013\220\234\'\023\220\234\'\017'
+  _V2.methods_by_name['PatchAnnotations']._serialized_options = b'\202\323\344\223\002`2E/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/annotations:\001*Z\0242\017/v2/annotations:\001*\230\234\'\002\220\234\'-\220\234\'\005\220\234\'%\220\234\'&\220\234\'\013\220\234\'\023\220\234\'\017'
   _V2.methods_by_name['PatchAnnotationsStatus']._options = None
-  _V2.methods_by_name['PatchAnnotationsStatus']._serialized_options = b'\202\323\344\223\002`2[/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/task/{task_id}/annotations/status:\001*\230\234\'\002\220\234\'%\220\234\'&\220\234\'\013\220\234\'\023\220\234\'\017'
+  _V2.methods_by_name['PatchAnnotationsStatus']._serialized_options = b'\202\323\344\223\002`2[/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/task/{task_id}/annotations/status:\001*\230\234\'\002\220\234\'-\220\234\'%\220\234\'&\220\234\'\013\220\234\'\023\220\234\'\017'
   _V2.methods_by_name['DeleteAnnotation']._options = None
-  _V2.methods_by_name['DeleteAnnotation']._serialized_options = b'\202\323\344\223\002\236\001*g/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/inputs/{input_id}/annotations/{annotation_id}Z3*1/v2/inputs/{input_id}/annotations/{annotation_id}\230\234\'\002\220\234\'%\220\234\'(\220\234\'&\220\234\'\023\220\234\'\017'
+  _V2.methods_by_name['DeleteAnnotation']._serialized_options = b'\202\323\344\223\002\236\001*g/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/inputs/{input_id}/annotations/{annotation_id}Z3*1/v2/inputs/{input_id}/annotations/{annotation_id}\230\234\'\002\220\234\'-\220\234\'%\220\234\'(\220\234\'&\220\234\'\023\220\234\'\017'
   _V2.methods_by_name['DeleteAnnotations']._options = None
-  _V2.methods_by_name['DeleteAnnotations']._serialized_options = b'\202\323\344\223\002\320\001*L/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/inputs/annotations:\001*Z\033*\026/v2/inputs/annotations:\001*ZJ*E/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/annotations:\001*Z\024*\017/v2/annotations:\001*\230\234\'\002\220\234\'%\220\234\'(\220\234\'&\220\234\'\023\220\234\'\017'
+  _V2.methods_by_name['DeleteAnnotations']._serialized_options = b'\202\323\344\223\002\320\001*L/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/inputs/annotations:\001*Z\033*\026/v2/inputs/annotations:\001*ZJ*E/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/annotations:\001*Z\024*\017/v2/annotations:\001*\230\234\'\002\220\234\'-\220\234\'%\220\234\'(\220\234\'&\220\234\'\023\220\234\'\017'
   _V2.methods_by_name['PatchAnnotationsSearches']._options = None
-  _V2.methods_by_name['PatchAnnotationsSearches']._serialized_options = b'\202\323\344\223\002r2N/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/annotations/searches:\001*Z\0352\030/v2/annotations/searches:\001*\230\234\'\002\220\234\'s\220\234\'r'
+  _V2.methods_by_name['PatchAnnotationsSearches']._serialized_options = b'\202\323\344\223\002r2N/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/annotations/searches:\001*Z\0352\030/v2/annotations/searches:\001*\230\234\'\002\220\234\'-\220\234\'s\220\234\'r'
   _V2.methods_by_name['PostAnnotationsSearches']._options = None
-  _V2.methods_by_name['PostAnnotationsSearches']._serialized_options = b'\202\323\344\223\002r\"N/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/annotations/searches:\001*Z\035\"\030/v2/annotations/searches:\001*\230\234\'\002\220\234\'&\220\234\'\013\220\234\'\005\220\234\'\017\220\234\'\003\220\234\'\023'
+  _V2.methods_by_name['PostAnnotationsSearches']._serialized_options = b'\202\323\344\223\002r\"N/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/annotations/searches:\001*Z\035\"\030/v2/annotations/searches:\001*\230\234\'\002\220\234\'-\220\234\'&\220\234\'\013\220\234\'\005\220\234\'\017\220\234\'\003\220\234\'\023'
   _V2.methods_by_name['GetInputCount']._options = None
-  _V2.methods_by_name['GetInputCount']._serialized_options = b'\202\323\344\223\002^\022G/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/inputs/statusZ\023\022\021/v2/inputs/status\230\234\'\002\220\234\'&\220\234\'\013\220\234\'\005'
+  _V2.methods_by_name['GetInputCount']._serialized_options = b'\202\323\344\223\002^\022G/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/inputs/statusZ\023\022\021/v2/inputs/status\230\234\'\002\220\234\'-\220\234\'&\220\234\'\013\220\234\'\005'
   _V2.methods_by_name['StreamInputs']._options = None
-  _V2.methods_by_name['StreamInputs']._serialized_options = b'\202\323\344\223\002^\022G/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/inputs/streamZ\023\022\021/v2/inputs/stream\230\234\'\002\220\234\'&\220\234\'\013\220\234\'\005'
+  _V2.methods_by_name['StreamInputs']._serialized_options = b'\202\323\344\223\002^\022G/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/inputs/streamZ\023\022\021/v2/inputs/stream\230\234\'\002\220\234\'-\220\234\'&\220\234\'\013\220\234\'\005'
   _V2.methods_by_name['GetInputSamples']._options = None
-  _V2.methods_by_name['GetInputSamples']._serialized_options = b'\202\323\344\223\002\200\001\022X/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/tasks/{task_id}/inputs/samplesZ$\022\"/v2/tasks/{task_id}/inputs/samples\230\234\'\002\220\234\'&\220\234\'\013\220\234\'\005'
+  _V2.methods_by_name['GetInputSamples']._serialized_options = b'\202\323\344\223\002\200\001\022X/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/tasks/{task_id}/inputs/samplesZ$\022\"/v2/tasks/{task_id}/inputs/samples\230\234\'\002\220\234\'-\220\234\'&\220\234\'\013\220\234\'\005'
   _V2.methods_by_name['GetInput']._options = None
-  _V2.methods_by_name['GetInput']._serialized_options = b'\202\323\344\223\002f\022K/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/inputs/{input_id}Z\027\022\025/v2/inputs/{input_id}\230\234\'\002\220\234\'&\220\234\'\013\220\234\'\005'
+  _V2.methods_by_name['GetInput']._serialized_options = b'\202\323\344\223\002f\022K/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/inputs/{input_id}Z\027\022\025/v2/inputs/{input_id}\230\234\'\002\220\234\'-\220\234\'&\220\234\'\013\220\234\'\005'
   _V2.methods_by_name['GetInputVideoManifest']._options = None
-  _V2.methods_by_name['GetInputVideoManifest']._serialized_options = b'\202\323\344\223\002\204\001\022Z/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/inputs/{input_id}/video_manifestZ&\022$/v2/inputs/{input_id}/video_manifest\230\234\'\002\220\234\'\005'
+  _V2.methods_by_name['GetInputVideoManifest']._serialized_options = b'\202\323\344\223\002\204\001\022Z/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/inputs/{input_id}/video_manifestZ&\022$/v2/inputs/{input_id}/video_manifest\230\234\'\002\220\234\'-\220\234\'\005'
   _V2.methods_by_name['ListInputs']._options = None
-  _V2.methods_by_name['ListInputs']._serialized_options = b'\202\323\344\223\002P\022@/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/inputsZ\014\022\n/v2/inputs\230\234\'\002\220\234\'&\220\234\'\013\220\234\'\005'
+  _V2.methods_by_name['ListInputs']._serialized_options = b'\202\323\344\223\002P\022@/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/inputsZ\014\022\n/v2/inputs\230\234\'\002\220\234\'-\220\234\'&\220\234\'\013\220\234\'\005'
   _V2.methods_by_name['PostInputs']._options = None
-  _V2.methods_by_name['PostInputs']._serialized_options = b'\202\323\344\223\002V\"@/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/inputs:\001*Z\017\"\n/v2/inputs:\001*\230\234\'\002\220\234\'%\220\234\'&\220\234\'\013\220\234\'\004\220\234\'\005\220\234\'\017\220\234\'\002\220\234\'\023'
+  _V2.methods_by_name['PostInputs']._serialized_options = b'\202\323\344\223\002V\"@/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/inputs:\001*Z\017\"\n/v2/inputs:\001*\230\234\'\002\220\234\'-\220\234\'%\220\234\'&\220\234\'\013\220\234\'\004\220\234\'\005\220\234\'\017\220\234\'\002\220\234\'\023'
   _V2.methods_by_name['PatchInputs']._options = None
-  _V2.methods_by_name['PatchInputs']._serialized_options = b'\202\323\344\223\002V2@/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/inputs:\001*Z\0172\n/v2/inputs:\001*\230\234\'\002\220\234\'%\220\234\'&\220\234\'\013\220\234\'\004\220\234\'\005\220\234\'\017'
+  _V2.methods_by_name['PatchInputs']._serialized_options = b'\202\323\344\223\002V2@/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/inputs:\001*Z\0172\n/v2/inputs:\001*\230\234\'\002\220\234\'-\220\234\'%\220\234\'&\220\234\'\013\220\234\'\004\220\234\'\005\220\234\'\017'
   _V2.methods_by_name['DeleteInput']._options = None
-  _V2.methods_by_name['DeleteInput']._serialized_options = b'\202\323\344\223\002f*K/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/inputs/{input_id}Z\027*\025/v2/inputs/{input_id}\230\234\'\002\220\234\'%\220\234\'(\220\234\'&\220\234\'\004\220\234\'\010\220\234\'\005\220\234\'\017\220\234\'\023'
+  _V2.methods_by_name['DeleteInput']._serialized_options = b'\202\323\344\223\002f*K/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/inputs/{input_id}Z\027*\025/v2/inputs/{input_id}\230\234\'\002\220\234\'-\220\234\'%\220\234\'(\220\234\'&\220\234\'\004\220\234\'\010\220\234\'\005\220\234\'\017\220\234\'\023'
   _V2.methods_by_name['DeleteInputs']._options = None
-  _V2.methods_by_name['DeleteInputs']._serialized_options = b'\202\323\344\223\002V*@/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/inputs:\001*Z\017*\n/v2/inputs:\001*\230\234\'\002\220\234\'%\220\234\'(\220\234\'&\220\234\'\004\220\234\'\010\220\234\'\005\220\234\'\017\220\234\'\023'
+  _V2.methods_by_name['DeleteInputs']._serialized_options = b'\202\323\344\223\002V*@/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/inputs:\001*Z\017*\n/v2/inputs:\001*\230\234\'\002\220\234\'-\220\234\'%\220\234\'(\220\234\'&\220\234\'\004\220\234\'\010\220\234\'\005\220\234\'\017\220\234\'\023'
   _V2.methods_by_name['PatchInputsSearches']._options = None
-  _V2.methods_by_name['PatchInputsSearches']._serialized_options = b'\202\323\344\223\002h2I/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/inputs/searches:\001*Z\0302\023/v2/inputs/searches:\001*\230\234\'\002\220\234\'s\220\234\'r'
+  _V2.methods_by_name['PatchInputsSearches']._serialized_options = b'\202\323\344\223\002h2I/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/inputs/searches:\001*Z\0302\023/v2/inputs/searches:\001*\230\234\'\002\220\234\'-\220\234\'s\220\234\'r'
   _V2.methods_by_name['PostInputsSearches']._options = None
-  _V2.methods_by_name['PostInputsSearches']._serialized_options = b'\202\323\344\223\002h\"I/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/inputs/searches:\001*Z\030\"\023/v2/inputs/searches:\001*\230\234\'\002\220\234\'&\220\234\'\013\220\234\'\005\220\234\'\017\220\234\'\003\220\234\'\023'
+  _V2.methods_by_name['PostInputsSearches']._serialized_options = b'\202\323\344\223\002h\"I/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/inputs/searches:\001*Z\030\"\023/v2/inputs/searches:\001*\230\234\'\002\220\234\'-\220\234\'&\220\234\'\013\220\234\'\005\220\234\'\017\220\234\'\003\220\234\'\023'
   _V2.methods_by_name['PostModelOutputs']._options = None
-  _V2.methods_by_name['PostModelOutputs']._serialized_options = b'\202\323\344\223\002\246\002\"i/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}/versions/{version_id}/outputs:\001*Z8\"3/v2/models/{model_id}/versions/{version_id}/outputs:\001*ZX\"S/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}/outputs:\001*Z\"\"\035/v2/models/{model_id}/outputs:\001*\230\234\'\002\220\234\'\013\220\234\'\017\220\234\'\002'
+  _V2.methods_by_name['PostModelOutputs']._serialized_options = b'\202\323\344\223\002\246\002\"i/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}/versions/{version_id}/outputs:\001*Z8\"3/v2/models/{model_id}/versions/{version_id}/outputs:\001*ZX\"S/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}/outputs:\001*Z\"\"\035/v2/models/{model_id}/outputs:\001*\230\234\'\002\220\234\'-\220\234\'\013\220\234\'\017\220\234\'\002'
   _V2.methods_by_name['ListDatasets']._options = None
-  _V2.methods_by_name['ListDatasets']._serialized_options = b'\202\323\344\223\002T\022B/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/datasetsZ\016\022\014/v2/datasets\230\234\'\002\220\234\'i\220\234\'r'
+  _V2.methods_by_name['ListDatasets']._serialized_options = b'\202\323\344\223\002\200\001\022B/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/datasetsZ*\022(/v2/users/{user_app_id.user_id}/datasetsZ\016\022\014/v2/datasets\230\234\'\002\220\234\'-\220\234\'i\220\234\'r'
   _V2.methods_by_name['GetDataset']._options = None
-  _V2.methods_by_name['GetDataset']._serialized_options = b'\202\323\344\223\002n\022O/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/datasets/{dataset_id}Z\033\022\031/v2/datasets/{dataset_id}\230\234\'\002\220\234\'i\220\234\'r'
+  _V2.methods_by_name['GetDataset']._serialized_options = b'\202\323\344\223\002n\022O/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/datasets/{dataset_id}Z\033\022\031/v2/datasets/{dataset_id}\230\234\'\002\220\234\'-\220\234\'i\220\234\'r'
   _V2.methods_by_name['PostDatasets']._options = None
-  _V2.methods_by_name['PostDatasets']._serialized_options = b'\202\323\344\223\002Z\"B/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/datasets:\001*Z\021\"\014/v2/datasets:\001*\230\234\'\002\220\234\'i\220\234\'j\220\234\'r'
+  _V2.methods_by_name['PostDatasets']._serialized_options = b'\202\323\344\223\002Z\"B/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/datasets:\001*Z\021\"\014/v2/datasets:\001*\230\234\'\002\220\234\'-\220\234\'i\220\234\'j\220\234\'r'
   _V2.methods_by_name['PatchDatasets']._options = None
-  _V2.methods_by_name['PatchDatasets']._serialized_options = b'\202\323\344\223\002Z2B/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/datasets:\001*Z\0212\014/v2/datasets:\001*\230\234\'\002\220\234\'i\220\234\'j\220\234\'r'
-  _V2.methods_by_name['PatchDatasetIds']._options = None
-  _V2.methods_by_name['PatchDatasetIds']._serialized_options = b'\202\323\344\223\002K2F/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/datasets/ids:\001*\230\234\'\002\220\234\'i\220\234\'j'
+  _V2.methods_by_name['PatchDatasets']._serialized_options = b'\202\323\344\223\002Z2B/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/datasets:\001*Z\0212\014/v2/datasets:\001*\230\234\'\002\220\234\'-\220\234\'i\220\234\'j\220\234\'r'
   _V2.methods_by_name['DeleteDatasets']._options = None
-  _V2.methods_by_name['DeleteDatasets']._serialized_options = b'\202\323\344\223\002Z*B/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/datasets:\001*Z\021*\014/v2/datasets:\001*\230\234\'\002\220\234\'i\220\234\'j\220\234\'k'
+  _V2.methods_by_name['DeleteDatasets']._serialized_options = b'\202\323\344\223\002Z*B/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/datasets:\001*Z\021*\014/v2/datasets:\001*\230\234\'\002\220\234\'-\220\234\'i\220\234\'j\220\234\'k'
   _V2.methods_by_name['ListDatasetInputs']._options = None
-  _V2.methods_by_name['ListDatasetInputs']._serialized_options = b'\202\323\344\223\002|\022V/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/datasets/{dataset_id}/inputsZ\"\022 /v2/datasets/{dataset_id}/inputs\230\234\'\002\220\234\'i\220\234\'\005\220\234\'&\220\234\'\013'
+  _V2.methods_by_name['ListDatasetInputs']._serialized_options = b'\202\323\344\223\002|\022V/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/datasets/{dataset_id}/inputsZ\"\022 /v2/datasets/{dataset_id}/inputs\230\234\'\002\220\234\'-\220\234\'i\220\234\'\005\220\234\'&\220\234\'\013'
   _V2.methods_by_name['GetDatasetInput']._options = None
-  _V2.methods_by_name['GetDatasetInput']._serialized_options = b'\202\323\344\223\002\222\001\022a/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/datasets/{dataset_id}/inputs/{input_id}Z-\022+/v2/datasets/{dataset_id}/inputs/{input_id}\230\234\'\002\220\234\'i\220\234\'\005\220\234\'&\220\234\'\013'
+  _V2.methods_by_name['GetDatasetInput']._serialized_options = b'\202\323\344\223\002\222\001\022a/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/datasets/{dataset_id}/inputs/{input_id}Z-\022+/v2/datasets/{dataset_id}/inputs/{input_id}\230\234\'\002\220\234\'-\220\234\'i\220\234\'\005\220\234\'&\220\234\'\013'
   _V2.methods_by_name['PostDatasetInputs']._options = None
-  _V2.methods_by_name['PostDatasetInputs']._serialized_options = b'\202\323\344\223\002\202\001\"V/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/datasets/{dataset_id}/inputs:\001*Z%\" /v2/datasets/{dataset_id}/inputs:\001*\230\234\'\002\220\234\'i\220\234\'j\220\234\'\005\220\234\'&\220\234\'\013'
+  _V2.methods_by_name['PostDatasetInputs']._serialized_options = b'\202\323\344\223\002\202\001\"V/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/datasets/{dataset_id}/inputs:\001*Z%\" /v2/datasets/{dataset_id}/inputs:\001*\230\234\'\002\220\234\'-\220\234\'i\220\234\'j\220\234\'\005\220\234\'&\220\234\'\013'
   _V2.methods_by_name['DeleteDatasetInputs']._options = None
-  _V2.methods_by_name['DeleteDatasetInputs']._serialized_options = b'\202\323\344\223\002\202\001*V/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/datasets/{dataset_id}/inputs:\001*Z%* /v2/datasets/{dataset_id}/inputs:\001*\230\234\'\002\220\234\'i\220\234\'j\220\234\'k\220\234\'\005'
+  _V2.methods_by_name['DeleteDatasetInputs']._serialized_options = b'\202\323\344\223\002\202\001*V/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/datasets/{dataset_id}/inputs:\001*Z%* /v2/datasets/{dataset_id}/inputs:\001*\230\234\'\002\220\234\'-\220\234\'i\220\234\'j\220\234\'k\220\234\'\005'
   _V2.methods_by_name['ListDatasetVersions']._options = None
-  _V2.methods_by_name['ListDatasetVersions']._serialized_options = b'\202\323\344\223\002\200\001\022X/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/datasets/{dataset_id}/versionsZ$\022\"/v2/datasets/{dataset_id}/versions\230\234\'\002\220\234\'i\220\234\'r'
+  _V2.methods_by_name['ListDatasetVersions']._serialized_options = b'\202\323\344\223\002\200\001\022X/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/datasets/{dataset_id}/versionsZ$\022\"/v2/datasets/{dataset_id}/versions\230\234\'\002\220\234\'-\220\234\'i\220\234\'r'
   _V2.methods_by_name['GetDatasetVersion']._options = None
-  _V2.methods_by_name['GetDatasetVersion']._serialized_options = b'\202\323\344\223\002\252\001\022m/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/datasets/{dataset_id}/versions/{dataset_version_id}Z9\0227/v2/datasets/{dataset_id}/versions/{dataset_version_id}\230\234\'\002\220\234\'i\220\234\'r'
+  _V2.methods_by_name['GetDatasetVersion']._serialized_options = b'\202\323\344\223\002\252\001\022m/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/datasets/{dataset_id}/versions/{dataset_version_id}Z9\0227/v2/datasets/{dataset_id}/versions/{dataset_version_id}\230\234\'\002\220\234\'-\220\234\'i\220\234\'r'
   _V2.methods_by_name['ListDatasetVersionMetricsGroups']._options = None
-  _V2.methods_by_name['ListDatasetVersionMetricsGroups']._serialized_options = b'\202\323\344\223\002\272\001\022u/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/datasets/{dataset_id}/versions/{dataset_version_id}/metricsZA\022?/v2/datasets/{dataset_id}/versions/{dataset_version_id}/metrics\230\234\'\002\220\234\'i\220\234\'&\220\234\'\013\220\234\'\005'
+  _V2.methods_by_name['ListDatasetVersionMetricsGroups']._serialized_options = b'\202\323\344\223\002\272\001\022u/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/datasets/{dataset_id}/versions/{dataset_version_id}/metricsZA\022?/v2/datasets/{dataset_id}/versions/{dataset_version_id}/metrics\230\234\'\002\220\234\'-\220\234\'i\220\234\'&\220\234\'\013\220\234\'\005'
   _V2.methods_by_name['PostDatasetVersions']._options = None
-  _V2.methods_by_name['PostDatasetVersions']._serialized_options = b'\202\323\344\223\002\206\001\"X/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/datasets/{dataset_id}/versions:\001*Z\'\"\"/v2/datasets/{dataset_id}/versions:\001*\230\234\'\002\220\234\'i\220\234\'j\220\234\'\017\220\234\'\023'
+  _V2.methods_by_name['PostDatasetVersions']._serialized_options = b'\202\323\344\223\002\206\001\"X/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/datasets/{dataset_id}/versions:\001*Z\'\"\"/v2/datasets/{dataset_id}/versions:\001*\230\234\'\002\220\234\'-\220\234\'i\220\234\'j\220\234\'\017\220\234\'\023'
   _V2.methods_by_name['PatchDatasetVersions']._options = None
-  _V2.methods_by_name['PatchDatasetVersions']._serialized_options = b'\202\323\344\223\002\206\0012X/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/datasets/{dataset_id}/versions:\001*Z\'2\"/v2/datasets/{dataset_id}/versions:\001*\230\234\'\002\220\234\'i\220\234\'j'
+  _V2.methods_by_name['PatchDatasetVersions']._serialized_options = b'\202\323\344\223\002\206\0012X/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/datasets/{dataset_id}/versions:\001*Z\'2\"/v2/datasets/{dataset_id}/versions:\001*\230\234\'\002\220\234\'-\220\234\'i\220\234\'j'
   _V2.methods_by_name['DeleteDatasetVersions']._options = None
-  _V2.methods_by_name['DeleteDatasetVersions']._serialized_options = b'\202\323\344\223\002\206\001*X/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/datasets/{dataset_id}/versions:\001*Z\'*\"/v2/datasets/{dataset_id}/versions:\001*\230\234\'\002\220\234\'i\220\234\'j\220\234\'k'
+  _V2.methods_by_name['DeleteDatasetVersions']._serialized_options = b'\202\323\344\223\002\206\001*X/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/datasets/{dataset_id}/versions:\001*Z\'*\"/v2/datasets/{dataset_id}/versions:\001*\230\234\'\002\220\234\'-\220\234\'i\220\234\'j\220\234\'k'
   _V2.methods_by_name['PutDatasetVersionExports']._options = None
-  _V2.methods_by_name['PutDatasetVersionExports']._serialized_options = b'\202\323\344\223\002\300\001\032u/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/datasets/{dataset_id}/versions/{dataset_version_id}/exports:\001*ZD\032?/v2/datasets/{dataset_id}/versions/{dataset_version_id}/exports:\001*\230\234\'\002\220\234\'i\220\234\'j'
+  _V2.methods_by_name['PutDatasetVersionExports']._serialized_options = b'\202\323\344\223\002\300\001\032u/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/datasets/{dataset_id}/versions/{dataset_version_id}/exports:\001*ZD\032?/v2/datasets/{dataset_id}/versions/{dataset_version_id}/exports:\001*\230\234\'\002\220\234\'-\220\234\'i\220\234\'j'
   _V2.methods_by_name['GetModelType']._options = None
-  _V2.methods_by_name['GetModelType']._serialized_options = b'\202\323\344\223\002|\022V/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/types/{model_type_id}Z\"\022 /v2/models/types/{model_type_id}\230\234\'\002\220\234\'\017'
+  _V2.methods_by_name['GetModelType']._serialized_options = b'\202\323\344\223\002|\022V/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/types/{model_type_id}Z\"\022 /v2/models/types/{model_type_id}\230\234\'\002\220\234\'-\220\234\'\017'
   _V2.methods_by_name['ListOpenSourceLicenses']._options = None
   _V2.methods_by_name['ListOpenSourceLicenses']._serialized_options = b'\202\323\344\223\002\032\022\030/v2/open_source_licenses\230\234\'\001'
   _V2.methods_by_name['ListModelTypes']._options = None
-  _V2.methods_by_name['ListModelTypes']._serialized_options = b'\202\323\344\223\002\\\022F/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/typesZ\022\022\020/v2/models/types\230\234\'\002\220\234\'\017'
+  _V2.methods_by_name['ListModelTypes']._serialized_options = b'\202\323\344\223\002\\\022F/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/typesZ\022\022\020/v2/models/types\230\234\'\002\220\234\'-\220\234\'\017'
   _V2.methods_by_name['GetModel']._options = None
-  _V2.methods_by_name['GetModel']._serialized_options = b'\202\323\344\223\002f\022K/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}Z\027\022\025/v2/models/{model_id}\230\234\'\002\220\234\'\013\220\234\'\017'
+  _V2.methods_by_name['GetModel']._serialized_options = b'\202\323\344\223\002f\022K/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}Z\027\022\025/v2/models/{model_id}\230\234\'\002\220\234\'-\220\234\'\013\220\234\'\017'
   _V2.methods_by_name['GetModelOutputInfo']._options = None
-  _V2.methods_by_name['GetModelOutputInfo']._serialized_options = b'\202\323\344\223\002\252\002\022W/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}/output_infoZ#\022!/v2/models/{model_id}/output_infoZo\022m/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}/versions/{version_id}/output_infoZ9\0227/v2/models/{model_id}/versions/{version_id}/output_info\230\234\'\002\220\234\'\013\220\234\'\017'
+  _V2.methods_by_name['GetModelOutputInfo']._serialized_options = b'\202\323\344\223\002\252\002\022W/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}/output_infoZ#\022!/v2/models/{model_id}/output_infoZo\022m/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}/versions/{version_id}/output_infoZ9\0227/v2/models/{model_id}/versions/{version_id}/output_info\230\234\'\002\220\234\'-\220\234\'\013\220\234\'\017'
   _V2.methods_by_name['ListModels']._options = None
-  _V2.methods_by_name['ListModels']._serialized_options = b'\202\323\344\223\002z\022@/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/modelsZ(\022&/v2/users/{user_app_id.user_id}/modelsZ\014\022\n/v2/models\230\234\'\002\220\234\'\013\220\234\'\017'
+  _V2.methods_by_name['ListModels']._serialized_options = b'\202\323\344\223\002z\022@/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/modelsZ(\022&/v2/users/{user_app_id.user_id}/modelsZ\014\022\n/v2/models\230\234\'\002\220\234\'-\220\234\'\013\220\234\'\017'
+  _V2.methods_by_name['GetResourceCounts']._options = None
+  _V2.methods_by_name['GetResourceCounts']._serialized_options = b'\202\323\344\223\002b\022I/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/resource_countsZ\025\022\023/v2/resource_counts\230\234\'\002\220\234\'i\220\234\'\017\220\234\'\023\220\234\'m\220\234\'-'
   _V2.methods_by_name['PostModelsSearches']._options = None
-  _V2.methods_by_name['PostModelsSearches']._serialized_options = b'\202\323\344\223\002h\"I/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/searches:\001*Z\030\"\023/v2/models/searches:\001*\230\234\'\002\220\234\'\013\220\234\'\017'
+  _V2.methods_by_name['PostModelsSearches']._serialized_options = b'\202\323\344\223\002h\"I/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/searches:\001*Z\030\"\023/v2/models/searches:\001*\230\234\'\002\220\234\'-\220\234\'\013\220\234\'\017'
   _V2.methods_by_name['PostModels']._options = None
-  _V2.methods_by_name['PostModels']._serialized_options = b'\202\323\344\223\002V\"@/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models:\001*Z\017\"\n/v2/models:\001*\230\234\'\002\220\234\'\013\220\234\'\016\220\234\'\017\220\234\'\032\220\234\'\023'
+  _V2.methods_by_name['PostModels']._serialized_options = b'\202\323\344\223\002V\"@/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models:\001*Z\017\"\n/v2/models:\001*\230\234\'\002\220\234\'-\220\234\'\013\220\234\'\016\220\234\'\017\220\234\'\032\220\234\'\023'
   _V2.methods_by_name['PatchModels']._options = None
-  _V2.methods_by_name['PatchModels']._serialized_options = b'\202\323\344\223\002V2@/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models:\001*Z\0172\n/v2/models:\001*\230\234\'\002\220\234\'\013\220\234\'\016\220\234\'\017\220\234\'\032'
+  _V2.methods_by_name['PatchModels']._serialized_options = b'\202\323\344\223\002V2@/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models:\001*Z\0172\n/v2/models:\001*\230\234\'\002\220\234\'-\220\234\'\013\220\234\'\016\220\234\'\017\220\234\'\032'
   _V2.methods_by_name['PatchModelIds']._options = None
-  _V2.methods_by_name['PatchModelIds']._serialized_options = b'\202\323\344\223\002I2D/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/ids:\001*\230\234\'\002\220\234\'\016\220\234\'\017'
+  _V2.methods_by_name['PatchModelIds']._serialized_options = b'\202\323\344\223\002I2D/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/ids:\001*\230\234\'\002\220\234\'-\220\234\'\016\220\234\'\017'
   _V2.methods_by_name['DeleteModel']._options = None
-  _V2.methods_by_name['DeleteModel']._serialized_options = b'\202\323\344\223\002f*K/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}Z\027*\025/v2/models/{model_id}\230\234\'\002\220\234\'\013\220\234\'\016\220\234\'\021\220\234\'\017\220\234\'\023'
+  _V2.methods_by_name['DeleteModel']._serialized_options = b'\202\323\344\223\002f*K/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}Z\027*\025/v2/models/{model_id}\230\234\'\002\220\234\'-\220\234\'\013\220\234\'\016\220\234\'\021\220\234\'\017\220\234\'\023'
   _V2.methods_by_name['DeleteModels']._options = None
-  _V2.methods_by_name['DeleteModels']._serialized_options = b'\202\323\344\223\002V*@/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models:\001*Z\017*\n/v2/models:\001*\230\234\'\002\220\234\'\013\220\234\'\016\220\234\'\021\220\234\'\017\220\234\'\023'
+  _V2.methods_by_name['DeleteModels']._serialized_options = b'\202\323\344\223\002V*@/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models:\001*Z\017*\n/v2/models:\001*\230\234\'\002\220\234\'-\220\234\'\013\220\234\'\016\220\234\'\021\220\234\'\017\220\234\'\023'
   _V2.methods_by_name['PatchModelCheckConsents']._options = None
-  _V2.methods_by_name['PatchModelCheckConsents']._serialized_options = b'\202\323\344\223\002\212\0012Z/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}/check_consents:\001*Z)2$/v2/models/{model_id}/check_consents:\001*\230\234\'\002\220\234\'\017'
+  _V2.methods_by_name['PatchModelCheckConsents']._serialized_options = b'\202\323\344\223\002\212\0012Z/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}/check_consents:\001*Z)2$/v2/models/{model_id}/check_consents:\001*\230\234\'\002\220\234\'-\220\234\'\017'
   _V2.methods_by_name['PatchModelToolkits']._options = None
-  _V2.methods_by_name['PatchModelToolkits']._serialized_options = b'\202\323\344\223\002~2T/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}/toolkits:\001*Z#2\036/v2/models/{model_id}/toolkits:\001*\230\234\'\002\220\234\'\017'
+  _V2.methods_by_name['PatchModelToolkits']._serialized_options = b'\202\323\344\223\002~2T/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}/toolkits:\001*Z#2\036/v2/models/{model_id}/toolkits:\001*\230\234\'\002\220\234\'-\220\234\'\017'
   _V2.methods_by_name['PatchModelUseCases']._options = None
-  _V2.methods_by_name['PatchModelUseCases']._serialized_options = b'\202\323\344\223\002~2T/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}/usecases:\001*Z#2\036/v2/models/{model_id}/usecases:\001*\230\234\'\002\220\234\'\017'
+  _V2.methods_by_name['PatchModelUseCases']._serialized_options = b'\202\323\344\223\002~2T/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}/usecases:\001*Z#2\036/v2/models/{model_id}/usecases:\001*\230\234\'\002\220\234\'-\220\234\'\017'
   _V2.methods_by_name['PatchModelLanguages']._options = None
-  _V2.methods_by_name['PatchModelLanguages']._serialized_options = b'\202\323\344\223\002\200\0012U/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}/languages:\001*Z$2\037/v2/models/{model_id}/languages:\001*\230\234\'\002\220\234\'\017'
+  _V2.methods_by_name['PatchModelLanguages']._serialized_options = b'\202\323\344\223\002\200\0012U/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}/languages:\001*Z$2\037/v2/models/{model_id}/languages:\001*\230\234\'\002\220\234\'-\220\234\'\017'
   _V2.methods_by_name['ListModelInputs']._options = None
-  _V2.methods_by_name['ListModelInputs']._serialized_options = b'\202\323\344\223\002\226\002\022R/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}/inputsZ\036\022\034/v2/models/{model_id}/inputsZj\022h/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}/versions/{version_id}/inputsZ4\0222/v2/models/{model_id}/versions/{version_id}/inputs\230\234\'\002\220\234\'&\220\234\'\013\220\234\'\005\220\234\'\017'
+  _V2.methods_by_name['ListModelInputs']._serialized_options = b'\202\323\344\223\002\226\002\022R/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}/inputsZ\036\022\034/v2/models/{model_id}/inputsZj\022h/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}/versions/{version_id}/inputsZ4\0222/v2/models/{model_id}/versions/{version_id}/inputs\230\234\'\002\220\234\'-\220\234\'&\220\234\'\013\220\234\'\005\220\234\'\017'
   _V2.methods_by_name['GetModelVersion']._options = None
-  _V2.methods_by_name['GetModelVersion']._serialized_options = b'\202\323\344\223\002\222\001\022a/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}/versions/{version_id}Z-\022+/v2/models/{model_id}/versions/{version_id}\230\234\'\002\220\234\'\013\220\234\'\017'
+  _V2.methods_by_name['GetModelVersion']._serialized_options = b'\202\323\344\223\002\222\001\022a/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}/versions/{version_id}Z-\022+/v2/models/{model_id}/versions/{version_id}\230\234\'\002\220\234\'-\220\234\'\013\220\234\'\017'
   _V2.methods_by_name['ListModelVersions']._options = None
-  _V2.methods_by_name['ListModelVersions']._serialized_options = b'\202\323\344\223\002x\022T/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}/versionsZ \022\036/v2/models/{model_id}/versions\230\234\'\002\220\234\'\013\220\234\'\017'
+  _V2.methods_by_name['ListModelVersions']._serialized_options = b'\202\323\344\223\002x\022T/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}/versionsZ \022\036/v2/models/{model_id}/versions\230\234\'\002\220\234\'-\220\234\'\013\220\234\'\017'
   _V2.methods_by_name['PostWorkflowVersionsUnPublish']._options = None
-  _V2.methods_by_name['PostWorkflowVersionsUnPublish']._serialized_options = b'\202\323\344\223\002\214\001\"[/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/workflows/{workflow_id}/unpublish:\001*Z*\"%/v2/workflows/{workflow_id}/unpublish:\001*\230\234\'\002\220\234\'x\220\234\'&\220\234\'\013\220\234\'\005\220\234\'\016\220\234\'\017\220\234\'\032\220\234\'\023\220\234\'5\220\234\'6'
+  _V2.methods_by_name['PostWorkflowVersionsUnPublish']._serialized_options = b'\202\323\344\223\002\214\001\"[/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/workflows/{workflow_id}/unpublish:\001*Z*\"%/v2/workflows/{workflow_id}/unpublish:\001*\230\234\'\002\220\234\'-\220\234\'x\220\234\'&\220\234\'\013\220\234\'\005\220\234\'\016\220\234\'\017\220\234\'\032\220\234\'\023\220\234\'5\220\234\'6'
   _V2.methods_by_name['PostWorkflowVersionsPublish']._options = None
-  _V2.methods_by_name['PostWorkflowVersionsPublish']._serialized_options = b'\202\323\344\223\002\210\001\"Y/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/workflows/{workflow_id}/publish:\001*Z(\"#/v2/workflows/{workflow_id}/publish:\001*\230\234\'\002\220\234\'w\220\234\'&\220\234\'\013\220\234\'\005\220\234\'\016\220\234\'\017\220\234\'\032\220\234\'\023\220\234\'5\220\234\'6'
+  _V2.methods_by_name['PostWorkflowVersionsPublish']._serialized_options = b'\202\323\344\223\002\210\001\"Y/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/workflows/{workflow_id}/publish:\001*Z(\"#/v2/workflows/{workflow_id}/publish:\001*\230\234\'\002\220\234\'-\220\234\'w\220\234\'&\220\234\'\013\220\234\'\005\220\234\'\016\220\234\'\017\220\234\'\032\220\234\'\023\220\234\'5\220\234\'6'
   _V2.methods_by_name['PostModelVersionsPublish']._options = None
-  _V2.methods_by_name['PostModelVersionsPublish']._serialized_options = b'\202\323\344\223\002|\"S/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}/publish:\001*Z\"\"\035/v2/models/{model_id}/publish:\001*\230\234\'\002\220\234\'u\220\234\'&\220\234\'\013\220\234\'\005\220\234\'\016\220\234\'\017\220\234\'\032\220\234\'\023\220\234\'5\220\234\'6'
+  _V2.methods_by_name['PostModelVersionsPublish']._serialized_options = b'\202\323\344\223\002|\"S/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}/publish:\001*Z\"\"\035/v2/models/{model_id}/publish:\001*\230\234\'\002\220\234\'-\220\234\'u\220\234\'&\220\234\'\013\220\234\'\005\220\234\'\016\220\234\'\017\220\234\'\032\220\234\'\023\220\234\'5\220\234\'6'
   _V2.methods_by_name['PostModelVersionsUnPublish']._options = None
-  _V2.methods_by_name['PostModelVersionsUnPublish']._serialized_options = b'\202\323\344\223\002\200\001\"U/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}/unpublish:\001*Z$\"\037/v2/models/{model_id}/unpublish:\001*\230\234\'\002\220\234\'v\220\234\'&\220\234\'\013\220\234\'\005\220\234\'\016\220\234\'\017\220\234\'\032\220\234\'\023\220\234\'5\220\234\'6'
+  _V2.methods_by_name['PostModelVersionsUnPublish']._serialized_options = b'\202\323\344\223\002\200\001\"U/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}/unpublish:\001*Z$\"\037/v2/models/{model_id}/unpublish:\001*\230\234\'\002\220\234\'-\220\234\'v\220\234\'&\220\234\'\013\220\234\'\005\220\234\'\016\220\234\'\017\220\234\'\032\220\234\'\023\220\234\'5\220\234\'6'
   _V2.methods_by_name['PostModelVersions']._options = None
-  _V2.methods_by_name['PostModelVersions']._serialized_options = b'\202\323\344\223\002~\"T/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}/versions:\001*Z#\"\036/v2/models/{model_id}/versions:\001*\230\234\'\002\220\234\'&\220\234\'\013\220\234\'\005\220\234\'\016\220\234\'\017\220\234\'\032\220\234\'\023\220\234\'5\220\234\'6'
+  _V2.methods_by_name['PostModelVersions']._serialized_options = b'\202\323\344\223\002~\"T/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}/versions:\001*Z#\"\036/v2/models/{model_id}/versions:\001*\230\234\'\002\220\234\'-\220\234\'&\220\234\'\013\220\234\'\005\220\234\'\016\220\234\'\017\220\234\'\032\220\234\'\023\220\234\'5\220\234\'6'
   _V2.methods_by_name['PatchModelVersions']._options = None
-  _V2.methods_by_name['PatchModelVersions']._serialized_options = b'\202\323\344\223\002Y2T/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}/versions:\001*\230\234\'\002\220\234\'\013\220\234\'\017\220\234\'\016\220\234\'\032'
+  _V2.methods_by_name['PatchModelVersions']._serialized_options = b'\202\323\344\223\002Y2T/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}/versions:\001*\230\234\'\002\220\234\'-\220\234\'\013\220\234\'\017\220\234\'\016\220\234\'\032'
   _V2.methods_by_name['DeleteModelVersion']._options = None
-  _V2.methods_by_name['DeleteModelVersion']._serialized_options = b'\202\323\344\223\002\222\001*a/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}/versions/{version_id}Z-*+/v2/models/{model_id}/versions/{version_id}\230\234\'\002\220\234\'\013\220\234\'\016\220\234\'\021\220\234\'\017\220\234\'\023'
+  _V2.methods_by_name['DeleteModelVersion']._serialized_options = b'\202\323\344\223\002\222\001*a/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}/versions/{version_id}Z-*+/v2/models/{model_id}/versions/{version_id}\230\234\'\002\220\234\'-\220\234\'\013\220\234\'\016\220\234\'\021\220\234\'\017\220\234\'\023'
   _V2.methods_by_name['GetModelVersionMetrics']._options = None
-  _V2.methods_by_name['GetModelVersionMetrics']._serialized_options = b'\202\323\344\223\002\242\001\022i/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}/versions/{version_id}/metricsZ5\0223/v2/models/{model_id}/versions/{version_id}/metrics\230\234\'\002\220\234\'&\220\234\'\013\220\234\'\017\220\234\'\005\220\234\'5'
+  _V2.methods_by_name['GetModelVersionMetrics']._serialized_options = b'\202\323\344\223\002\242\001\022i/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}/versions/{version_id}/metricsZ5\0223/v2/models/{model_id}/versions/{version_id}/metrics\230\234\'\002\220\234\'-\220\234\'&\220\234\'\013\220\234\'\017\220\234\'\005\220\234\'5'
   _V2.methods_by_name['PostModelVersionMetrics']._options = None
-  _V2.methods_by_name['PostModelVersionMetrics']._serialized_options = b'\202\323\344\223\002\250\001\"i/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}/versions/{version_id}/metrics:\001*Z8\"3/v2/models/{model_id}/versions/{version_id}/metrics:\001*\230\234\'\002\220\234\'&\220\234\'\013\220\234\'\005\220\234\'\016\220\234\'\017\220\234\'\032\220\234\'\002\220\234\'\023\220\234\'5\220\234\'6'
+  _V2.methods_by_name['PostModelVersionMetrics']._serialized_options = b'\202\323\344\223\002\250\001\"i/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}/versions/{version_id}/metrics:\001*Z8\"3/v2/models/{model_id}/versions/{version_id}/metrics:\001*\230\234\'\002\220\234\'-\220\234\'&\220\234\'\013\220\234\'\005\220\234\'\016\220\234\'\017\220\234\'\032\220\234\'\002\220\234\'\023\220\234\'5\220\234\'6'
   _V2.methods_by_name['PostModelVersionEvaluations']._options = None
-  _V2.methods_by_name['PostModelVersionEvaluations']._serialized_options = b'\202\323\344\223\002\274\001\"s/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}/versions/{model_version_id}/evaluations:\001*ZB\"=/v2/models/{model_id}/versions/{model_version_id}/evaluations:\001*\230\234\'\002\220\234\'&\220\234\'\013\220\234\'\005\220\234\'\016\220\234\'\017\220\234\'\032\220\234\'\002\220\234\'\023\220\234\'5\220\234\'6'
+  _V2.methods_by_name['PostModelVersionEvaluations']._serialized_options = b'\202\323\344\223\002\274\001\"s/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}/versions/{model_version_id}/evaluations:\001*ZB\"=/v2/models/{model_id}/versions/{model_version_id}/evaluations:\001*\230\234\'\002\220\234\'-\220\234\'&\220\234\'\013\220\234\'\005\220\234\'\016\220\234\'\017\220\234\'\032\220\234\'\002\220\234\'\023\220\234\'5\220\234\'6'
   _V2.methods_by_name['ListModelVersionEvaluations']._options = None
-  _V2.methods_by_name['ListModelVersionEvaluations']._serialized_options = b'\202\323\344\223\002\266\001\022s/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}/versions/{model_version_id}/evaluationsZ?\022=/v2/models/{model_id}/versions/{model_version_id}/evaluations\230\234\'\002\220\234\'&\220\234\'\013\220\234\'\017\220\234\'\005\220\234\'5'
+  _V2.methods_by_name['ListModelVersionEvaluations']._serialized_options = b'\202\323\344\223\002\266\001\022s/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}/versions/{model_version_id}/evaluationsZ?\022=/v2/models/{model_id}/versions/{model_version_id}/evaluations\230\234\'\002\220\234\'-\220\234\'&\220\234\'\013\220\234\'\017\220\234\'\005\220\234\'5'
   _V2.methods_by_name['GetModelVersionEvaluation']._options = None
-  _V2.methods_by_name['GetModelVersionEvaluation']._serialized_options = b'\202\323\344\223\002\327\001\022\203\001/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}/versions/{model_version_id}/evaluations/{evaluation_id}ZO\022M/v2/models/{model_id}/versions/{model_version_id}/evaluations/{evaluation_id}\230\234\'\002\220\234\'&\220\234\'\013\220\234\'\017\220\234\'\005\220\234\'5'
+  _V2.methods_by_name['GetModelVersionEvaluation']._serialized_options = b'\202\323\344\223\002\327\001\022\203\001/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}/versions/{model_version_id}/evaluations/{evaluation_id}ZO\022M/v2/models/{model_id}/versions/{model_version_id}/evaluations/{evaluation_id}\230\234\'\002\220\234\'-\220\234\'&\220\234\'\013\220\234\'\017\220\234\'\005\220\234\'5'
+  _V2.methods_by_name['PostEvaluations']._options = None
+  _V2.methods_by_name['PostEvaluations']._serialized_options = b'\202\323\344\223\002`\"E/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/evaluations:\001*Z\024\"\017/v2/evaluations:\001*\230\234\'\002\220\234\'-\220\234\'&\220\234\'\013\220\234\'\005\220\234\'\016\220\234\'\017\220\234\'\032\220\234\'\002\220\234\'\023\220\234\'5\220\234\'6'
+  _V2.methods_by_name['ListEvaluations']._options = None
+  _V2.methods_by_name['ListEvaluations']._serialized_options = b'\202\323\344\223\002Z\022E/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/evaluationsZ\021\022\017/v2/evaluations\230\234\'\002\220\234\'-\220\234\'&\220\234\'\013\220\234\'\017\220\234\'\005\220\234\'5'
+  _V2.methods_by_name['GetEvaluation']._options = None
+  _V2.methods_by_name['GetEvaluation']._serialized_options = b'\202\323\344\223\002z\022U/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/evaluations/{evaluation_id}Z!\022\037/v2/evaluations/{evaluation_id}\230\234\'\002\220\234\'-\220\234\'&\220\234\'\013\220\234\'\017\220\234\'\005\220\234\'5'
   _V2.methods_by_name['ListModelReferences']._options = None
-  _V2.methods_by_name['ListModelReferences']._serialized_options = b'\202\323\344\223\002|\022V/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}/referencesZ\"\022 /v2/models/{model_id}/references\230\234\'\002\220\234\'\017'
+  _V2.methods_by_name['ListModelReferences']._serialized_options = b'\202\323\344\223\002|\022V/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}/referencesZ\"\022 /v2/models/{model_id}/references\230\234\'\002\220\234\'-\220\234\'\017'
   _V2.methods_by_name['GetModelVersionInputExample']._options = None
-  _V2.methods_by_name['GetModelVersionInputExample']._serialized_options = b'\202\323\344\223\002\327\001\022\203\001/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}/versions/{model_version_id}/input_examples/{example_id}ZO\022M/v2/models/{model_id}/versions/{model_version_id}/input_examples/{example_id}\230\234\'\002\220\234\'\017'
+  _V2.methods_by_name['GetModelVersionInputExample']._serialized_options = b'\202\323\344\223\002\327\001\022\203\001/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}/versions/{model_version_id}/input_examples/{example_id}ZO\022M/v2/models/{model_id}/versions/{model_version_id}/input_examples/{example_id}\230\234\'\002\220\234\'-\220\234\'\017'
   _V2.methods_by_name['ListModelVersionInputExamples']._options = None
-  _V2.methods_by_name['ListModelVersionInputExamples']._serialized_options = b'\202\323\344\223\002\274\001\022v/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}/versions/{model_version_id}/input_examplesZB\022@/v2/models/{model_id}/versions/{model_version_id}/input_examples\230\234\'\002\220\234\'\017'
+  _V2.methods_by_name['ListModelVersionInputExamples']._serialized_options = b'\202\323\344\223\002\274\001\022v/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}/versions/{model_version_id}/input_examplesZB\022@/v2/models/{model_id}/versions/{model_version_id}/input_examples\230\234\'\002\220\234\'-\220\234\'\017'
   _V2.methods_by_name['GetWorkflow']._options = None
-  _V2.methods_by_name['GetWorkflow']._serialized_options = b'\202\323\344\223\002r\022Q/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/workflows/{workflow_id}Z\035\022\033/v2/workflows/{workflow_id}\230\234\'\002\220\234\'\017\220\234\'\023'
+  _V2.methods_by_name['GetWorkflow']._serialized_options = b'\202\323\344\223\002r\022Q/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/workflows/{workflow_id}Z\035\022\033/v2/workflows/{workflow_id}\230\234\'\002\220\234\'-\220\234\'\017\220\234\'\023'
   _V2.methods_by_name['ListWorkflows']._options = None
-  _V2.methods_by_name['ListWorkflows']._serialized_options = b'\202\323\344\223\002\203\001\022C/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/workflowsZ+\022)/v2/users/{user_app_id.user_id}/workflowsZ\017\022\r/v2/workflows\230\234\'\002\220\234\'\017\220\234\'\023'
+  _V2.methods_by_name['ListWorkflows']._serialized_options = b'\202\323\344\223\002\203\001\022C/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/workflowsZ+\022)/v2/users/{user_app_id.user_id}/workflowsZ\017\022\r/v2/workflows\230\234\'\002\220\234\'-\220\234\'\017\220\234\'\023'
   _V2.methods_by_name['PostWorkflows']._options = None
-  _V2.methods_by_name['PostWorkflows']._serialized_options = b'\202\323\344\223\002\\\"C/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/workflows:\001*Z\022\"\r/v2/workflows:\001*\230\234\'\002\220\234\'\017\220\234\'\022\220\234\'\023'
+  _V2.methods_by_name['PostWorkflows']._serialized_options = b'\202\323\344\223\002\\\"C/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/workflows:\001*Z\022\"\r/v2/workflows:\001*\230\234\'\002\220\234\'-\220\234\'\017\220\234\'\022\220\234\'\023'
   _V2.methods_by_name['PatchWorkflows']._options = None
-  _V2.methods_by_name['PatchWorkflows']._serialized_options = b'\202\323\344\223\002\\2C/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/workflows:\001*Z\0222\r/v2/workflows:\001*\230\234\'\002\220\234\'\017\220\234\'\022\220\234\'\023'
+  _V2.methods_by_name['PatchWorkflows']._serialized_options = b'\202\323\344\223\002\\2C/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/workflows:\001*Z\0222\r/v2/workflows:\001*\230\234\'\002\220\234\'-\220\234\'\017\220\234\'\022\220\234\'\023'
   _V2.methods_by_name['PatchWorkflowIds']._options = None
-  _V2.methods_by_name['PatchWorkflowIds']._serialized_options = b'\202\323\344\223\002L2G/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/workflows/ids:\001*\230\234\'\002\220\234\'\022\220\234\'\023'
+  _V2.methods_by_name['PatchWorkflowIds']._serialized_options = b'\202\323\344\223\002L2G/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/workflows/ids:\001*\230\234\'\002\220\234\'-\220\234\'\022\220\234\'\023'
   _V2.methods_by_name['DeleteWorkflow']._options = None
-  _V2.methods_by_name['DeleteWorkflow']._serialized_options = b'\202\323\344\223\002r*Q/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/workflows/{workflow_id}Z\035*\033/v2/workflows/{workflow_id}\230\234\'\002\220\234\'\022\220\234\'\025\220\234\'\023'
+  _V2.methods_by_name['DeleteWorkflow']._serialized_options = b'\202\323\344\223\002r*Q/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/workflows/{workflow_id}Z\035*\033/v2/workflows/{workflow_id}\230\234\'\002\220\234\'-\220\234\'\022\220\234\'\025\220\234\'\023'
   _V2.methods_by_name['DeleteWorkflows']._options = None
-  _V2.methods_by_name['DeleteWorkflows']._serialized_options = b'\202\323\344\223\002\\*C/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/workflows:\001*Z\022*\r/v2/workflows:\001*\230\234\'\002\220\234\'\022\220\234\'\025\220\234\'\023'
+  _V2.methods_by_name['DeleteWorkflows']._serialized_options = b'\202\323\344\223\002\\*C/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/workflows:\001*Z\022*\r/v2/workflows:\001*\230\234\'\002\220\234\'-\220\234\'\022\220\234\'\025\220\234\'\023'
   _V2.methods_by_name['PostWorkflowResults']._options = None
-  _V2.methods_by_name['PostWorkflowResults']._serialized_options = b'\202\323\344\223\002\376\001\"o/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/workflows/{workflow_id}/versions/{version_id}/results:\001*Z^\"Y/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/workflows/{workflow_id}/results:\001*Z(\"#/v2/workflows/{workflow_id}/results:\001*\230\234\'\002\220\234\'\017\220\234\'\013\220\234\'\002\220\234\'\023'
+  _V2.methods_by_name['PostWorkflowResults']._serialized_options = b'\202\323\344\223\002\376\001\"o/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/workflows/{workflow_id}/versions/{version_id}/results:\001*Z^\"Y/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/workflows/{workflow_id}/results:\001*Z(\"#/v2/workflows/{workflow_id}/results:\001*\230\234\'\002\220\234\'-\220\234\'\017\220\234\'\013\220\234\'\002\220\234\'\023'
   _V2.methods_by_name['PostWorkflowResultsSimilarity']._options = None
-  _V2.methods_by_name['PostWorkflowResultsSimilarity']._serialized_options = b'\202\323\344\223\002\237\002\"z/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/workflows/{workflow_id}/versions/{version_id}/results/similarity:\001*Zi\"d/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/workflows/{workflow_id}/results/similarity:\001*Z3\"./v2/workflows/{workflow_id}/results/similarity:\001*\230\234\'\002\220\234\'\017\220\234\'\013\220\234\'\002\220\234\'\023'
+  _V2.methods_by_name['PostWorkflowResultsSimilarity']._serialized_options = b'\202\323\344\223\002\237\002\"z/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/workflows/{workflow_id}/versions/{version_id}/results/similarity:\001*Zi\"d/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/workflows/{workflow_id}/results/similarity:\001*Z3\"./v2/workflows/{workflow_id}/results/similarity:\001*\230\234\'\002\220\234\'-\220\234\'\017\220\234\'\013\220\234\'\002\220\234\'\023'
   _V2.methods_by_name['ListWorkflowVersions']._options = None
-  _V2.methods_by_name['ListWorkflowVersions']._serialized_options = b'\202\323\344\223\002\204\001\022Z/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/workflows/{workflow_id}/versionsZ&\022$/v2/workflows/{workflow_id}/versions\230\234\'\002\220\234\'\017\220\234\'\023'
+  _V2.methods_by_name['ListWorkflowVersions']._serialized_options = b'\202\323\344\223\002\204\001\022Z/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/workflows/{workflow_id}/versionsZ&\022$/v2/workflows/{workflow_id}/versions\230\234\'\002\220\234\'-\220\234\'\017\220\234\'\023'
   _V2.methods_by_name['GetWorkflowVersion']._options = None
-  _V2.methods_by_name['GetWorkflowVersion']._serialized_options = b'\202\323\344\223\002\260\001\022p/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/workflows/{workflow_id}/versions/{workflow_version_id}Z<\022:/v2/workflows/{workflow_id}/versions/{workflow_version_id}\230\234\'\002\220\234\'\017\220\234\'\023'
+  _V2.methods_by_name['GetWorkflowVersion']._serialized_options = b'\202\323\344\223\002\260\001\022p/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/workflows/{workflow_id}/versions/{workflow_version_id}Z<\022:/v2/workflows/{workflow_id}/versions/{workflow_version_id}\230\234\'\002\220\234\'-\220\234\'\017\220\234\'\023'
   _V2.methods_by_name['DeleteWorkflowVersions']._options = None
-  _V2.methods_by_name['DeleteWorkflowVersions']._serialized_options = b'\202\323\344\223\002\212\001*Z/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/workflows/{workflow_id}/versions:\001*Z)*$/v2/workflows/{workflow_id}/versions:\001*\230\234\'\002\220\234\'\023\220\234\'\022\220\234\'\025'
+  _V2.methods_by_name['DeleteWorkflowVersions']._serialized_options = b'\202\323\344\223\002\212\001*Z/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/workflows/{workflow_id}/versions:\001*Z)*$/v2/workflows/{workflow_id}/versions:\001*\230\234\'\002\220\234\'-\220\234\'\023\220\234\'\022\220\234\'\025'
   _V2.methods_by_name['PatchWorkflowVersions']._options = None
-  _V2.methods_by_name['PatchWorkflowVersions']._serialized_options = b'\202\323\344\223\002\212\0012Z/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/workflows/{workflow_id}/versions:\001*Z)2$/v2/workflows/{workflow_id}/versions:\001*\230\234\'\002\220\234\'\017\220\234\'\023\220\234\'\022'
+  _V2.methods_by_name['PatchWorkflowVersions']._serialized_options = b'\202\323\344\223\002\212\0012Z/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/workflows/{workflow_id}/versions:\001*Z)2$/v2/workflows/{workflow_id}/versions:\001*\230\234\'\002\220\234\'-\220\234\'\017\220\234\'\023\220\234\'\022'
   _V2.methods_by_name['GetKey']._options = None
   _V2.methods_by_name['GetKey']._serialized_options = b'\202\323\344\223\002/\022-/v2/users/{user_app_id.user_id}/keys/{key_id}\230\234\'\005\220\234\'0'
   _V2.methods_by_name['ListKeys']._options = None
   _V2.methods_by_name['ListKeys']._serialized_options = b'\202\323\344\223\002&\022$/v2/users/{user_app_id.user_id}/keys\230\234\'\005\220\234\'0'
   _V2.methods_by_name['ListAppKeys']._options = None
-  _V2.methods_by_name['ListAppKeys']._serialized_options = b'\202\323\344\223\002@\022>/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/keys\230\234\'\005\220\234\'0'
+  _V2.methods_by_name['ListAppKeys']._serialized_options = b'\202\323\344\223\002@\022>/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/keys\230\234\'\005\220\234\'-\220\234\'0'
   _V2.methods_by_name['DeleteKey']._options = None
   _V2.methods_by_name['DeleteKey']._serialized_options = b'\202\323\344\223\002/*-/v2/users/{user_app_id.user_id}/keys/{key_id}\230\234\'\005\220\234\'/\220\234\'1\220\234\'0'
   _V2.methods_by_name['PostKeys']._options = None
   _V2.methods_by_name['PostKeys']._serialized_options = b'\202\323\344\223\002)\"$/v2/users/{user_app_id.user_id}/keys:\001*\230\234\'\005\220\234\'-\220\234\'/\220\234\'0'
   _V2.methods_by_name['PatchKeys']._options = None
   _V2.methods_by_name['PatchKeys']._serialized_options = b'\202\323\344\223\002)2$/v2/users/{user_app_id.user_id}/keys:\001*\230\234\'\005\220\234\'/\220\234\'0'
   _V2.methods_by_name['MyScopes']._options = None
@@ -348,771 +354,783 @@
   _V2.methods_by_name['PostAppsSearches']._options = None
   _V2.methods_by_name['PostAppsSearches']._serialized_options = b'\202\323\344\223\0022\"-/v2/users/{user_app_id.user_id}/apps/searches:\001*\230\234\'\005\220\234\'-\220\234\'\023'
   _V2.methods_by_name['GetUser']._options = None
   _V2.methods_by_name['GetUser']._serialized_options = b'\202\323\344\223\002!\022\037/v2/users/{user_app_id.user_id}\230\234\'\005'
   _V2.methods_by_name['PostValidatePassword']._options = None
   _V2.methods_by_name['PostValidatePassword']._serialized_options = b'\202\323\344\223\002R\"1/v2/users/{user_app_id.user_id}/validate_password:\001*Z\032\"\025/v2/validate_password:\001*\230\234\'\003'
   _V2.methods_by_name['GetSearch']._options = None
-  _V2.methods_by_name['GetSearch']._serialized_options = b'\202\323\344\223\002^\022G/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/searches/{id}Z\023\022\021/v2/searches/{id}\230\234\'\002\220\234\'r'
+  _V2.methods_by_name['GetSearch']._serialized_options = b'\202\323\344\223\002^\022G/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/searches/{id}Z\023\022\021/v2/searches/{id}\230\234\'\002\220\234\'-\220\234\'r'
   _V2.methods_by_name['ListSearches']._options = None
-  _V2.methods_by_name['ListSearches']._serialized_options = b'\202\323\344\223\002T\022B/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/searchesZ\016\022\014/v2/searches\230\234\'\002\220\234\'r'
+  _V2.methods_by_name['ListSearches']._serialized_options = b'\202\323\344\223\002T\022B/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/searchesZ\016\022\014/v2/searches\230\234\'\002\220\234\'-\220\234\'r'
   _V2.methods_by_name['PatchSearches']._options = None
-  _V2.methods_by_name['PatchSearches']._serialized_options = b'\202\323\344\223\002Z2B/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/searches:\001*Z\0212\014/v2/searches:\001*\230\234\'\002\220\234\'s\220\234\'r'
+  _V2.methods_by_name['PatchSearches']._serialized_options = b'\202\323\344\223\002Z2B/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/searches:\001*Z\0212\014/v2/searches:\001*\230\234\'\002\220\234\'-\220\234\'s\220\234\'r'
   _V2.methods_by_name['PostSearches']._options = None
-  _V2.methods_by_name['PostSearches']._serialized_options = b'\210\002\001\202\323\344\223\002Z\"B/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/searches:\001*Z\021\"\014/v2/searches:\001*\230\234\'\002\220\234\'&\220\234\'\013\220\234\'\005\220\234\'\017\220\234\'\003\220\234\'\023'
+  _V2.methods_by_name['PostSearches']._serialized_options = b'\210\002\001\202\323\344\223\002Z\"B/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/searches:\001*Z\021\"\014/v2/searches:\001*\230\234\'\002\220\234\'-\220\234\'&\220\234\'\013\220\234\'\005\220\234\'\017\220\234\'\003\220\234\'\023'
   _V2.methods_by_name['PostSearchesByID']._options = None
-  _V2.methods_by_name['PostSearchesByID']._serialized_options = b'\202\323\344\223\002d\"G/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/searches/{id}:\001*Z\026\"\021/v2/searches/{id}:\001*\230\234\'\002\220\234\'r\220\234\'\003'
+  _V2.methods_by_name['PostSearchesByID']._serialized_options = b'\202\323\344\223\002d\"G/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/searches/{id}:\001*Z\026\"\021/v2/searches/{id}:\001*\230\234\'\002\220\234\'-\220\234\'r\220\234\'\003'
   _V2.methods_by_name['PostAnnotationSearchMetrics']._options = None
-  _V2.methods_by_name['PostAnnotationSearchMetrics']._serialized_options = b'\202\323\344\223\002\202\001\"V/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/annotations/searches/metrics:\001*Z%\" /v2/annotations/searches/metrics:\001*\230\234\'\002\220\234\'&\220\234\'\013\220\234\'\005\220\234\'5\220\234\'6\220\234\'\017\220\234\'\023'
+  _V2.methods_by_name['PostAnnotationSearchMetrics']._serialized_options = b'\202\323\344\223\002\202\001\"V/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/annotations/searches/metrics:\001*Z%\" /v2/annotations/searches/metrics:\001*\230\234\'\002\220\234\'-\220\234\'&\220\234\'\013\220\234\'\005\220\234\'5\220\234\'6\220\234\'\017\220\234\'\023'
   _V2.methods_by_name['GetAnnotationSearchMetrics']._options = None
-  _V2.methods_by_name['GetAnnotationSearchMetrics']._serialized_options = b'\202\323\344\223\002\206\001\022[/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/annotations/searches/metrics/{id}Z\'\022%/v2/annotations/searches/metrics/{id}\230\234\'\002\220\234\'&\220\234\'\013\220\234\'\005\220\234\'5'
+  _V2.methods_by_name['GetAnnotationSearchMetrics']._serialized_options = b'\202\323\344\223\002\206\001\022[/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/annotations/searches/metrics/{id}Z\'\022%/v2/annotations/searches/metrics/{id}\230\234\'\002\220\234\'-\220\234\'&\220\234\'\013\220\234\'\005\220\234\'5'
   _V2.methods_by_name['ListAnnotationSearchMetrics']._options = None
-  _V2.methods_by_name['ListAnnotationSearchMetrics']._serialized_options = b'\202\323\344\223\002|\022V/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/annotations/searches/metricsZ\"\022 /v2/annotations/searches/metrics\230\234\'\002\220\234\'&\220\234\'\013\220\234\'\005\220\234\'5'
+  _V2.methods_by_name['ListAnnotationSearchMetrics']._serialized_options = b'\202\323\344\223\002|\022V/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/annotations/searches/metricsZ\"\022 /v2/annotations/searches/metrics\230\234\'\002\220\234\'-\220\234\'&\220\234\'\013\220\234\'\005\220\234\'5'
   _V2.methods_by_name['DeleteAnnotationSearchMetrics']._options = None
-  _V2.methods_by_name['DeleteAnnotationSearchMetrics']._serialized_options = b'\202\323\344\223\002\206\001*[/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/annotations/searches/metrics/{id}Z\'*%/v2/annotations/searches/metrics/{id}\230\234\'\002\220\234\'5\220\234\'6\220\234\'?'
+  _V2.methods_by_name['DeleteAnnotationSearchMetrics']._serialized_options = b'\202\323\344\223\002\206\001*[/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/annotations/searches/metrics/{id}Z\'*%/v2/annotations/searches/metrics/{id}\230\234\'\002\220\234\'-\220\234\'5\220\234\'6\220\234\'?'
   _V2.methods_by_name['DeleteSearch']._options = None
-  _V2.methods_by_name['DeleteSearch']._serialized_options = b'\202\323\344\223\002^*G/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/searches/{id}Z\023*\021/v2/searches/{id}\230\234\'\002\220\234\'r\220\234\'s\220\234\'t'
+  _V2.methods_by_name['DeleteSearch']._serialized_options = b'\202\323\344\223\002^*G/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/searches/{id}Z\023*\021/v2/searches/{id}\230\234\'\002\220\234\'-\220\234\'r\220\234\'s\220\234\'t'
   _V2.methods_by_name['ListAnnotationFilters']._options = None
-  _V2.methods_by_name['ListAnnotationFilters']._serialized_options = b'\202\323\344\223\002h\022L/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/annotation_filtersZ\030\022\026/v2/annotation_filters\230\234\'\002\220\234\'r'
+  _V2.methods_by_name['ListAnnotationFilters']._serialized_options = b'\202\323\344\223\002h\022L/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/annotation_filtersZ\030\022\026/v2/annotation_filters\230\234\'\002\220\234\'-\220\234\'r'
   _V2.methods_by_name['GetAnnotationFilter']._options = None
-  _V2.methods_by_name['GetAnnotationFilter']._serialized_options = b'\202\323\344\223\002\226\001\022c/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/annotation_filters/{annotation_filter_id}Z/\022-/v2/annotation_filters/{annotation_filter_id}\230\234\'\002\220\234\'r'
+  _V2.methods_by_name['GetAnnotationFilter']._serialized_options = b'\202\323\344\223\002\226\001\022c/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/annotation_filters/{annotation_filter_id}Z/\022-/v2/annotation_filters/{annotation_filter_id}\230\234\'\002\220\234\'-\220\234\'r'
   _V2.methods_by_name['PostAnnotationFilters']._options = None
-  _V2.methods_by_name['PostAnnotationFilters']._serialized_options = b'\202\323\344\223\002n\"L/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/annotation_filters:\001*Z\033\"\026/v2/annotation_filters:\001*\230\234\'\002\220\234\'r\220\234\'s'
+  _V2.methods_by_name['PostAnnotationFilters']._serialized_options = b'\202\323\344\223\002n\"L/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/annotation_filters:\001*Z\033\"\026/v2/annotation_filters:\001*\230\234\'\002\220\234\'-\220\234\'r\220\234\'s'
   _V2.methods_by_name['PatchAnnotationFilters']._options = None
-  _V2.methods_by_name['PatchAnnotationFilters']._serialized_options = b'\202\323\344\223\002n2L/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/annotation_filters:\001*Z\0332\026/v2/annotation_filters:\001*\230\234\'\002\220\234\'r\220\234\'s'
+  _V2.methods_by_name['PatchAnnotationFilters']._serialized_options = b'\202\323\344\223\002n2L/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/annotation_filters:\001*Z\0332\026/v2/annotation_filters:\001*\230\234\'\002\220\234\'-\220\234\'r\220\234\'s'
   _V2.methods_by_name['DeleteAnnotationFilters']._options = None
-  _V2.methods_by_name['DeleteAnnotationFilters']._serialized_options = b'\202\323\344\223\002n*L/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/annotation_filters:\001*Z\033*\026/v2/annotation_filters:\001*\230\234\'\002\220\234\'r\220\234\'s'
+  _V2.methods_by_name['DeleteAnnotationFilters']._serialized_options = b'\202\323\344\223\002n*L/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/annotation_filters:\001*Z\033*\026/v2/annotation_filters:\001*\230\234\'\002\220\234\'-\220\234\'r\220\234\'s'
   _V2.methods_by_name['ListStatusCodes']._options = None
   _V2.methods_by_name['ListStatusCodes']._serialized_options = b'\202\323\344\223\002\022\022\020/v2/status_codes\230\234\'\001'
   _V2.methods_by_name['GetStatusCode']._options = None
   _V2.methods_by_name['GetStatusCode']._serialized_options = b'\202\323\344\223\002#\022!/v2/status_codes/{status_code_id}\230\234\'\001'
   _V2.methods_by_name['ListCollaborators']._options = None
-  _V2.methods_by_name['ListCollaborators']._serialized_options = b'\202\323\344\223\002I\022G/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/collaborators\230\234\'\002\220\234\'2'
+  _V2.methods_by_name['ListCollaborators']._serialized_options = b'\202\323\344\223\002I\022G/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/collaborators\230\234\'\002\220\234\'-\220\234\'2'
   _V2.methods_by_name['PostCollaborators']._options = None
-  _V2.methods_by_name['PostCollaborators']._serialized_options = b'\202\323\344\223\002L\"G/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/collaborators:\001*\230\234\'\002\220\234\'3\220\234\'2'
+  _V2.methods_by_name['PostCollaborators']._serialized_options = b'\202\323\344\223\002L\"G/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/collaborators:\001*\230\234\'\002\220\234\'-\220\234\'3\220\234\'2'
   _V2.methods_by_name['PatchCollaborators']._options = None
-  _V2.methods_by_name['PatchCollaborators']._serialized_options = b'\202\323\344\223\002L2G/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/collaborators:\001*\230\234\'\002\220\234\'3\220\234\'2\220\234\'4'
+  _V2.methods_by_name['PatchCollaborators']._serialized_options = b'\202\323\344\223\002L2G/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/collaborators:\001*\230\234\'\002\220\234\'-\220\234\'3\220\234\'2\220\234\'4'
   _V2.methods_by_name['DeleteCollaborators']._options = None
-  _V2.methods_by_name['DeleteCollaborators']._serialized_options = b'\202\323\344\223\002L*G/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/collaborators:\001*\230\234\'\002\220\234\'3\220\234\'2\220\234\'4\220\234\'7\220\234\'8'
+  _V2.methods_by_name['DeleteCollaborators']._serialized_options = b'\202\323\344\223\002L*G/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/collaborators:\001*\230\234\'\002\220\234\'-\220\234\'3\220\234\'2\220\234\'4\220\234\'7\220\234\'8'
   _V2.methods_by_name['ListCollaborations']._options = None
   _V2.methods_by_name['ListCollaborations']._serialized_options = b'\202\323\344\223\0020\022./v2/users/{user_app_id.user_id}/collaborations\230\234\'\003'
   _V2.methods_by_name['PostAppDuplications']._options = None
-  _V2.methods_by_name['PostAppDuplications']._serialized_options = b'\202\323\344\223\002K\"F/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/duplications:\001*\230\234\'\002\220\234\'\016\220\234\'\017\220\234\'\032\220\234\'\n\220\234\'\013\220\234\'\004\220\234\'\005\220\234\'%\220\234\'&\220\234\'\022\220\234\'\023'
+  _V2.methods_by_name['PostAppDuplications']._serialized_options = b'\202\323\344\223\002K\"F/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/duplications:\001*\230\234\'\002\220\234\'-\220\234\'\016\220\234\'\017\220\234\'\032\220\234\'\n\220\234\'\013\220\234\'\004\220\234\'\005\220\234\'%\220\234\'&\220\234\'\022\220\234\'\023'
   _V2.methods_by_name['ListAppDuplications']._options = None
   _V2.methods_by_name['ListAppDuplications']._serialized_options = b'\202\323\344\223\002.\022,/v2/users/{user_app_id.user_id}/duplications\230\234\'\005'
   _V2.methods_by_name['GetAppDuplication']._options = None
   _V2.methods_by_name['GetAppDuplication']._serialized_options = b'\202\323\344\223\002C\022A/v2/users/{user_app_id.user_id}/duplications/{app_duplication_id}\230\234\'\005'
   _V2.methods_by_name['PostTasks']._options = None
-  _V2.methods_by_name['PostTasks']._serialized_options = b'\202\323\344\223\002T\"?/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/tasks:\001*Z\016\"\t/v2/tasks:\001*\230\234\'\002\220\234\'7\220\234\'8\220\234\'\005\220\234\'\003\220\234\'r\220\234\'\013\220\234\'\023\220\234\'\017\220\234\'%\220\234\'&'
+  _V2.methods_by_name['PostTasks']._serialized_options = b'\202\323\344\223\002T\"?/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/tasks:\001*Z\016\"\t/v2/tasks:\001*\230\234\'\002\220\234\'-\220\234\'7\220\234\'8\220\234\'\005\220\234\'\003\220\234\'r\220\234\'\013\220\234\'\023\220\234\'\017\220\234\'%\220\234\'&'
   _V2.methods_by_name['GetTaskAnnotationCount']._options = None
-  _V2.methods_by_name['GetTaskAnnotationCount']._serialized_options = b'\202\323\344\223\002\206\001\022[/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/tasks/{task_id}/annotations/countZ\'\022%/v2/tasks/{task_id}/annotations/count\230\234\'\002\220\234\'8'
+  _V2.methods_by_name['GetTaskAnnotationCount']._serialized_options = b'\202\323\344\223\002\206\001\022[/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/tasks/{task_id}/annotations/countZ\'\022%/v2/tasks/{task_id}/annotations/count\230\234\'\002\220\234\'-\220\234\'8'
   _V2.methods_by_name['GetTaskInputCount']._options = None
-  _V2.methods_by_name['GetTaskInputCount']._serialized_options = b'\202\323\344\223\002|\022V/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/tasks/{task_id}/inputs/countZ\"\022 /v2/tasks/{task_id}/inputs/count\230\234\'\002\220\234\'8'
+  _V2.methods_by_name['GetTaskInputCount']._serialized_options = b'\202\323\344\223\002|\022V/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/tasks/{task_id}/inputs/countZ\"\022 /v2/tasks/{task_id}/inputs/count\230\234\'\002\220\234\'-\220\234\'8'
   _V2.methods_by_name['GetTask']._options = None
-  _V2.methods_by_name['GetTask']._serialized_options = b'\202\323\344\223\002b\022I/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/tasks/{task_id}Z\025\022\023/v2/tasks/{task_id}\230\234\'\002\220\234\'8\220\234\'r\220\234\'\013\220\234\'\023\220\234\'\017'
+  _V2.methods_by_name['GetTask']._serialized_options = b'\202\323\344\223\002b\022I/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/tasks/{task_id}Z\025\022\023/v2/tasks/{task_id}\230\234\'\002\220\234\'-\220\234\'8\220\234\'r\220\234\'\013\220\234\'\023\220\234\'\017'
   _V2.methods_by_name['ListTasks']._options = None
-  _V2.methods_by_name['ListTasks']._serialized_options = b'\202\323\344\223\002N\022?/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/tasksZ\013\022\t/v2/tasks\230\234\'\002\220\234\'8\220\234\'r\220\234\'\013\220\234\'\023\220\234\'\017'
+  _V2.methods_by_name['ListTasks']._serialized_options = b'\202\323\344\223\002N\022?/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/tasksZ\013\022\t/v2/tasks\230\234\'\002\220\234\'-\220\234\'8\220\234\'r\220\234\'\013\220\234\'\023\220\234\'\017'
   _V2.methods_by_name['PatchTasks']._options = None
-  _V2.methods_by_name['PatchTasks']._serialized_options = b'\202\323\344\223\002T2?/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/tasks:\001*Z\0162\t/v2/tasks:\001*\230\234\'\002\220\234\'7\220\234\'8\220\234\'\005\220\234\'r\220\234\'\013\220\234\'\023\220\234\'\017\220\234\'%\220\234\'&'
+  _V2.methods_by_name['PatchTasks']._serialized_options = b'\202\323\344\223\002T2?/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/tasks:\001*Z\0162\t/v2/tasks:\001*\230\234\'\002\220\234\'-\220\234\'7\220\234\'8\220\234\'\005\220\234\'r\220\234\'\013\220\234\'\023\220\234\'\017\220\234\'%\220\234\'&'
   _V2.methods_by_name['DeleteTasks']._options = None
-  _V2.methods_by_name['DeleteTasks']._serialized_options = b'\202\323\344\223\002T*?/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/tasks:\001*Z\016*\t/v2/tasks:\001*\230\234\'\002\220\234\'7\220\234\'8\220\234\'F'
+  _V2.methods_by_name['DeleteTasks']._serialized_options = b'\202\323\344\223\002T*?/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/tasks:\001*Z\016*\t/v2/tasks:\001*\230\234\'\002\220\234\'-\220\234\'7\220\234\'8\220\234\'F'
   _V2.methods_by_name['PostLabelOrders']._options = None
-  _V2.methods_by_name['PostLabelOrders']._serialized_options = b'\202\323\344\223\002b\"F/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/label_orders:\001*Z\025\"\020/v2/label_orders:\001*\230\234\'\002\220\234\'C\220\234\'D\220\234\'7\220\234\'8\220\234\'\005\220\234\'r\220\234\'\013\220\234\'\023\220\234\'\017'
+  _V2.methods_by_name['PostLabelOrders']._serialized_options = b'\202\323\344\223\002b\"F/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/label_orders:\001*Z\025\"\020/v2/label_orders:\001*\230\234\'\002\220\234\'-\220\234\'C\220\234\'D\220\234\'7\220\234\'8\220\234\'\005\220\234\'r\220\234\'\013\220\234\'\023\220\234\'\017'
   _V2.methods_by_name['GetLabelOrder']._options = None
-  _V2.methods_by_name['GetLabelOrder']._serialized_options = b'\202\323\344\223\002~\022W/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/label_orders/{label_order_id}Z#\022!/v2/label_orders/{label_order_id}\230\234\'\002\220\234\'C\220\234\'\013\220\234\'8'
+  _V2.methods_by_name['GetLabelOrder']._serialized_options = b'\202\323\344\223\002~\022W/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/label_orders/{label_order_id}Z#\022!/v2/label_orders/{label_order_id}\230\234\'\002\220\234\'-\220\234\'C\220\234\'\013\220\234\'8'
   _V2.methods_by_name['ListLabelOrders']._options = None
-  _V2.methods_by_name['ListLabelOrders']._serialized_options = b'\202\323\344\223\002\\\022F/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/label_ordersZ\022\022\020/v2/label_orders\230\234\'\002\220\234\'C\220\234\'\013\220\234\'8'
+  _V2.methods_by_name['ListLabelOrders']._serialized_options = b'\202\323\344\223\002\\\022F/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/label_ordersZ\022\022\020/v2/label_orders\230\234\'\002\220\234\'-\220\234\'C\220\234\'\013\220\234\'8'
   _V2.methods_by_name['PatchLabelOrders']._options = None
-  _V2.methods_by_name['PatchLabelOrders']._serialized_options = b'\202\323\344\223\002b2F/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/label_orders:\001*Z\0252\020/v2/label_orders:\001*\230\234\'\002\220\234\'C\220\234\'D\220\234\'\013\220\234\'7\220\234\'8\220\234\'F'
+  _V2.methods_by_name['PatchLabelOrders']._serialized_options = b'\202\323\344\223\002b2F/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/label_orders:\001*Z\0252\020/v2/label_orders:\001*\230\234\'\002\220\234\'-\220\234\'C\220\234\'D\220\234\'\013\220\234\'7\220\234\'8\220\234\'F'
   _V2.methods_by_name['DeleteLabelOrders']._options = None
-  _V2.methods_by_name['DeleteLabelOrders']._serialized_options = b'\202\323\344\223\002b*F/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/label_orders:\001*Z\025*\020/v2/label_orders:\001*\230\234\'\002\220\234\'E\220\234\'C\220\234\'D\220\234\'7\220\234\'8'
+  _V2.methods_by_name['DeleteLabelOrders']._serialized_options = b'\202\323\344\223\002b*F/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/label_orders:\001*Z\025*\020/v2/label_orders:\001*\230\234\'\002\220\234\'-\220\234\'E\220\234\'C\220\234\'D\220\234\'7\220\234\'8'
   _V2.methods_by_name['PostCollectors']._options = None
-  _V2.methods_by_name['PostCollectors']._serialized_options = b'\202\323\344\223\002^\"D/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/collectors:\001*Z\023\"\016/v2/collectors:\001*\230\234\'\002\220\234\'\004\220\234\'%\220\234\'&\220\234\')\220\234\'\013\220\234\'\004\220\234\'\005\220\234\'\017\220\234\'\002\220\234\'\023'
+  _V2.methods_by_name['PostCollectors']._serialized_options = b'\202\323\344\223\002^\"D/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/collectors:\001*Z\023\"\016/v2/collectors:\001*\230\234\'\002\220\234\'-\220\234\'\004\220\234\'%\220\234\'&\220\234\')\220\234\'\013\220\234\'\004\220\234\'\005\220\234\'\017\220\234\'\002\220\234\'\023'
   _V2.methods_by_name['GetCollector']._options = None
-  _V2.methods_by_name['GetCollector']._serialized_options = b'\202\323\344\223\002v\022S/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/collectors/{collector_id}Z\037\022\035/v2/collectors/{collector_id}\230\234\'\002\220\234\'*'
+  _V2.methods_by_name['GetCollector']._serialized_options = b'\202\323\344\223\002v\022S/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/collectors/{collector_id}Z\037\022\035/v2/collectors/{collector_id}\230\234\'\002\220\234\'-\220\234\'*'
   _V2.methods_by_name['ListCollectors']._options = None
-  _V2.methods_by_name['ListCollectors']._serialized_options = b'\202\323\344\223\002X\022D/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/collectorsZ\020\022\016/v2/collectors\230\234\'\002\220\234\'*'
+  _V2.methods_by_name['ListCollectors']._serialized_options = b'\202\323\344\223\002X\022D/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/collectorsZ\020\022\016/v2/collectors\230\234\'\002\220\234\'-\220\234\'*'
   _V2.methods_by_name['PatchCollectors']._options = None
-  _V2.methods_by_name['PatchCollectors']._serialized_options = b'\202\323\344\223\002^2D/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/collectors:\001*Z\0232\016/v2/collectors:\001*\230\234\'\002\220\234\')\220\234\'*'
+  _V2.methods_by_name['PatchCollectors']._serialized_options = b'\202\323\344\223\002^2D/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/collectors:\001*Z\0232\016/v2/collectors:\001*\230\234\'\002\220\234\'-\220\234\')\220\234\'*'
   _V2.methods_by_name['DeleteCollectors']._options = None
-  _V2.methods_by_name['DeleteCollectors']._serialized_options = b'\202\323\344\223\002^*D/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/collectors:\001*Z\023*\016/v2/collectors:\001*\230\234\'\002\220\234\')\220\234\'+\220\234\'*'
+  _V2.methods_by_name['DeleteCollectors']._serialized_options = b'\202\323\344\223\002^*D/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/collectors:\001*Z\023*\016/v2/collectors:\001*\230\234\'\002\220\234\'-\220\234\')\220\234\'+\220\234\'*'
   _V2.methods_by_name['PostStatValues']._options = None
   _V2.methods_by_name['PostStatValues']._serialized_options = b'\202\323\344\223\002b\"F/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/stats/values:\001*Z\025\"\020/v2/stats/values:\001*\230\234\'\002'
   _V2.methods_by_name['PostStatValuesAggregate']._options = None
-  _V2.methods_by_name['PostStatValuesAggregate']._serialized_options = b'\202\323\344\223\002v\"P/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/stats/values/aggregate:\001*Z\037\"\032/v2/stats/values/aggregate:\001*\230\234\'\002'
+  _V2.methods_by_name['PostStatValuesAggregate']._serialized_options = b'\202\323\344\223\002v\"P/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/stats/values/aggregate:\001*Z\037\"\032/v2/stats/values/aggregate:\001*\230\234\'\002\220\234\'-'
   _V2.methods_by_name['PostTrendingMetricsView']._options = None
   _V2.methods_by_name['PostTrendingMetricsView']._serialized_options = b'\202\323\344\223\002m\"h/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/trending_metrics/views/{view_type}/{object_id}:\001*\230\234\'\002'
   _V2.methods_by_name['ListTrendingMetricsViews']._options = None
   _V2.methods_by_name['ListTrendingMetricsViews']._serialized_options = b'\202\323\344\223\002\210\001\022\\/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/trending_metrics/views/{view_type}Z(\022&/v2/trending_metrics/views/{view_type}\230\234\'\002'
   _V2.methods_by_name['GetModule']._options = None
-  _V2.methods_by_name['GetModule']._serialized_options = b'\202\323\344\223\002O\022M/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/modules/{module_id}\230\234\'\002\220\234\'m'
+  _V2.methods_by_name['GetModule']._serialized_options = b'\202\323\344\223\002O\022M/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/modules/{module_id}\230\234\'\005\220\234\'-\220\234\'m'
   _V2.methods_by_name['ListModules']._options = None
-  _V2.methods_by_name['ListModules']._serialized_options = b'\202\323\344\223\002}\022A/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/modulesZ)\022\'/v2/users/{user_app_id.user_id}/modulesZ\r\022\013/v2/modules\230\234\'\002\220\234\'m'
+  _V2.methods_by_name['ListModules']._serialized_options = b'\202\323\344\223\002}\022A/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/modulesZ)\022\'/v2/users/{user_app_id.user_id}/modulesZ\r\022\013/v2/modules\230\234\'\005\220\234\'-\220\234\'m'
   _V2.methods_by_name['PostModules']._options = None
-  _V2.methods_by_name['PostModules']._serialized_options = b'\202\323\344\223\002F\"A/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/modules:\001*\230\234\'\002\220\234\'l\220\234\'m'
+  _V2.methods_by_name['PostModules']._serialized_options = b'\202\323\344\223\002F\"A/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/modules:\001*\230\234\'\005\220\234\'-\220\234\'l\220\234\'m'
   _V2.methods_by_name['PatchModules']._options = None
-  _V2.methods_by_name['PatchModules']._serialized_options = b'\202\323\344\223\002F2A/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/modules:\001*\230\234\'\002\220\234\'l\220\234\'m'
+  _V2.methods_by_name['PatchModules']._serialized_options = b'\202\323\344\223\002F2A/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/modules:\001*\230\234\'\005\220\234\'-\220\234\'l\220\234\'m'
   _V2.methods_by_name['DeleteModules']._options = None
-  _V2.methods_by_name['DeleteModules']._serialized_options = b'\202\323\344\223\002F*A/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/modules:\001*\230\234\'\002\220\234\'l\220\234\'n\220\234\'m'
+  _V2.methods_by_name['DeleteModules']._serialized_options = b'\202\323\344\223\002F*A/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/modules:\001*\230\234\'\005\220\234\'-\220\234\'l\220\234\'n\220\234\'m\220\234\'p\220\234\'o\220\234\'q\220\234\'1\220\234\'0\220\234\'/'
   _V2.methods_by_name['GetModuleVersion']._options = None
-  _V2.methods_by_name['GetModuleVersion']._serialized_options = b'\202\323\344\223\002s\022q/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/modules/{module_id}/module_versions/{module_version_id}\230\234\'\002\220\234\'m'
+  _V2.methods_by_name['GetModuleVersion']._serialized_options = b'\202\323\344\223\002l\022j/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/modules/{module_id}/versions/{module_version_id}\230\234\'\005\220\234\'-\220\234\'m'
   _V2.methods_by_name['ListModuleVersions']._options = None
-  _V2.methods_by_name['ListModuleVersions']._serialized_options = b'\202\323\344\223\002_\022]/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/modules/{module_id}/module_versions\230\234\'\002\220\234\'m'
+  _V2.methods_by_name['ListModuleVersions']._serialized_options = b'\202\323\344\223\002X\022V/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/modules/{module_id}/versions\230\234\'\005\220\234\'-\220\234\'m'
   _V2.methods_by_name['PostModuleVersions']._options = None
-  _V2.methods_by_name['PostModuleVersions']._serialized_options = b'\202\323\344\223\002b\"]/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/modules/{module_id}/module_versions:\001*\230\234\'\002\220\234\'l\220\234\'m'
+  _V2.methods_by_name['PostModuleVersions']._serialized_options = b'\202\323\344\223\002[\"V/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/modules/{module_id}/versions:\001*\230\234\'\005\220\234\'-\220\234\'l\220\234\'m'
   _V2.methods_by_name['DeleteModuleVersions']._options = None
-  _V2.methods_by_name['DeleteModuleVersions']._serialized_options = b'\202\323\344\223\002b*]/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/modules/{module_id}/module_versions:\001*\230\234\'\002\220\234\'l\220\234\'n\220\234\'m'
+  _V2.methods_by_name['DeleteModuleVersions']._serialized_options = b'\202\323\344\223\002[*V/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/modules/{module_id}/versions:\001*\230\234\'\005\220\234\'-\220\234\'l\220\234\'n\220\234\'m\220\234\'p\220\234\'o\220\234\'q\220\234\'1\220\234\'0\220\234\'/'
   _V2.methods_by_name['GetInstalledModuleVersion']._options = None
-  _V2.methods_by_name['GetInstalledModuleVersion']._serialized_options = b'\202\323\344\223\002s\022q/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/installed_module_versions/{installed_module_version_id}\230\234\'\005\220\234\'p\220\234\'m\220\234\'0'
+  _V2.methods_by_name['GetInstalledModuleVersion']._serialized_options = b'\202\323\344\223\002s\022q/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/installed_module_versions/{installed_module_version_id}\230\234\'\005\220\234\'-\220\234\'p\220\234\'m\220\234\'0'
   _V2.methods_by_name['ListInstalledModuleVersions']._options = None
-  _V2.methods_by_name['ListInstalledModuleVersions']._serialized_options = b'\202\323\344\223\002U\022S/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/installed_module_versions\230\234\'\005\220\234\'p\220\234\'m\220\234\'0'
+  _V2.methods_by_name['ListInstalledModuleVersions']._serialized_options = b'\202\323\344\223\002U\022S/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/installed_module_versions\230\234\'\005\220\234\'-\220\234\'p\220\234\'m\220\234\'0'
   _V2.methods_by_name['PostInstalledModuleVersions']._options = None
   _V2.methods_by_name['PostInstalledModuleVersions']._serialized_options = b'\202\323\344\223\002X\"S/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/installed_module_versions:\001*\230\234\'\005\220\234\'o\220\234\'p\220\234\'m\220\234\'-'
   _V2.methods_by_name['DeleteInstalledModuleVersions']._options = None
-  _V2.methods_by_name['DeleteInstalledModuleVersions']._serialized_options = b'\202\323\344\223\002X*S/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/installed_module_versions:\001*\230\234\'\005\220\234\'o\220\234\'p\220\234\'q\220\234\'m\220\234\'1\220\234\'/\220\234\'0'
+  _V2.methods_by_name['DeleteInstalledModuleVersions']._serialized_options = b'\202\323\344\223\002X*S/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/installed_module_versions:\001*\230\234\'\005\220\234\'-\220\234\'m\220\234\'o\220\234\'p\220\234\'q\220\234\'1\220\234\'/\220\234\'0'
   _V2.methods_by_name['PostInstalledModuleVersionsKey']._options = None
   _V2.methods_by_name['PostInstalledModuleVersionsKey']._serialized_options = b'\202\323\344\223\002z\"u/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/installed_module_versions/{installed_module_version_id}/key:\001*\230\234\'\005\220\234\'o\220\234\'p\220\234\'m\220\234\'-\220\234\'/\220\234\'0'
   _V2.methods_by_name['PostBulkOperations']._options = None
-  _V2.methods_by_name['PostBulkOperations']._serialized_options = b'\202\323\344\223\002h\"I/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/bulk_operations:\001*Z\030\"\023/v2/bulk_operations:\001*\230\234\'\002\220\234\'z\220\234\'y\220\234\'%\220\234\'&\220\234\'('
+  _V2.methods_by_name['PostBulkOperations']._serialized_options = b'\202\323\344\223\002h\"I/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/bulk_operations:\001*Z\030\"\023/v2/bulk_operations:\001*\230\234\'\002\220\234\'-\220\234\'z\220\234\'y\220\234\'%\220\234\'&\220\234\'('
   _V2.methods_by_name['ListBulkOperations']._options = None
-  _V2.methods_by_name['ListBulkOperations']._serialized_options = b'\202\323\344\223\002b\022I/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/bulk_operationsZ\025\022\023/v2/bulk_operations\230\234\'\002\220\234\'z'
+  _V2.methods_by_name['ListBulkOperations']._serialized_options = b'\202\323\344\223\002b\022I/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/bulk_operationsZ\025\022\023/v2/bulk_operations\230\234\'\002\220\234\'-\220\234\'z'
   _V2.methods_by_name['GetBulkOperation']._options = None
-  _V2.methods_by_name['GetBulkOperation']._serialized_options = b'\202\323\344\223\002l\022N/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/bulk_operations/{id}Z\032\022\030/v2/bulk_operations/{id}\230\234\'\002\220\234\'z'
+  _V2.methods_by_name['GetBulkOperation']._serialized_options = b'\202\323\344\223\002l\022N/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/bulk_operations/{id}Z\032\022\030/v2/bulk_operations/{id}\230\234\'\002\220\234\'-\220\234\'z'
   _V2.methods_by_name['CancelBulkOperations']._options = None
-  _V2.methods_by_name['CancelBulkOperations']._serialized_options = b'\202\323\344\223\002h2I/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/bulk_operations:\001*Z\0302\023/v2/bulk_operations:\001*\230\234\'\002\220\234\'y\220\234\'z'
+  _V2.methods_by_name['CancelBulkOperations']._serialized_options = b'\202\323\344\223\002h2I/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/bulk_operations:\001*Z\0302\023/v2/bulk_operations:\001*\230\234\'\002\220\234\'-\220\234\'y\220\234\'z'
   _V2.methods_by_name['DeleteBulkOperations']._options = None
-  _V2.methods_by_name['DeleteBulkOperations']._serialized_options = b'\202\323\344\223\002h*I/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/bulk_operations:\001*Z\030*\023/v2/bulk_operations:\001*\230\234\'\002\220\234\'&\220\234\'%\220\234\'(\220\234\'y\220\234\'z\220\234\'{'
+  _V2.methods_by_name['DeleteBulkOperations']._serialized_options = b'\202\323\344\223\002h*I/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/bulk_operations:\001*Z\030*\023/v2/bulk_operations:\001*\230\234\'\002\220\234\'-\220\234\'&\220\234\'%\220\234\'(\220\234\'y\220\234\'z\220\234\'{'
   _V2.methods_by_name['GetDatasetInputsSearchAddJob']._options = None
-  _V2.methods_by_name['GetDatasetInputsSearchAddJob']._serialized_options = b'\202\323\344\223\002\224\001\022b/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/datasets/inputs/search_add/jobs/{job_id}Z.\022,/v2/datasets/inputs/search_add/jobs/{job_id}\230\234\'\002\220\234\'i'
+  _V2.methods_by_name['GetDatasetInputsSearchAddJob']._serialized_options = b'\202\323\344\223\002\224\001\022b/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/datasets/inputs/search_add/jobs/{job_id}Z.\022,/v2/datasets/inputs/search_add/jobs/{job_id}\230\234\'\002\220\234\'-\220\234\'i'
   _V2.methods_by_name['ListNextTaskAssignments']._options = None
-  _V2.methods_by_name['ListNextTaskAssignments']._serialized_options = b'\202\323\344\223\002z\022U/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/tasks/{task_id}/assignmentsZ!\022\037/v2/tasks/{task_id}/assignments\230\234\'\002\220\234\'&\220\234\'\013\220\234\'\005\220\234\'8\220\234\'i'
+  _V2.methods_by_name['ListNextTaskAssignments']._serialized_options = b'\202\323\344\223\002z\022U/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/tasks/{task_id}/assignmentsZ!\022\037/v2/tasks/{task_id}/assignments\230\234\'\002\220\234\'-\220\234\'&\220\234\'\013\220\234\'\005\220\234\'8\220\234\'i'
   _V2.methods_by_name['PutTaskAssignments']._options = None
-  _V2.methods_by_name['PutTaskAssignments']._serialized_options = b'\202\323\344\223\002Z\032U/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/tasks/{task_id}/assignments:\001*\230\234\'\002\220\234\'%\220\234\'&\220\234\'\013\220\234\'\005\220\234\'8\220\234\'i'
+  _V2.methods_by_name['PutTaskAssignments']._serialized_options = b'\202\323\344\223\002Z\032U/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/tasks/{task_id}/assignments:\001*\230\234\'\002\220\234\'-\220\234\'%\220\234\'&\220\234\'\013\220\234\'\005\220\234\'8\220\234\'i'
   _V2.methods_by_name['ListInputsAddJobs']._options = None
-  _V2.methods_by_name['ListInputsAddJobs']._serialized_options = b'\202\323\344\223\002b\022I/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/inputs/jobs/addZ\025\022\023/v2/inputs/jobs/add\230\234\'\002\220\234\'\005'
+  _V2.methods_by_name['ListInputsAddJobs']._serialized_options = b'\202\323\344\223\002b\022I/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/inputs/jobs/addZ\025\022\023/v2/inputs/jobs/add\230\234\'\002\220\234\'-\220\234\'\005'
   _V2.methods_by_name['GetInputsAddJob']._options = None
-  _V2.methods_by_name['GetInputsAddJob']._serialized_options = b'\202\323\344\223\002l\022N/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/inputs/jobs/add/{id}Z\032\022\030/v2/inputs/jobs/add/{id}\230\234\'\002\220\234\'\005'
+  _V2.methods_by_name['GetInputsAddJob']._serialized_options = b'\202\323\344\223\002l\022N/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/inputs/jobs/add/{id}Z\032\022\030/v2/inputs/jobs/add/{id}\230\234\'\002\220\234\'-\220\234\'\005'
+  _V2.methods_by_name['CancelInputsAddJob']._options = None
+  _V2.methods_by_name['CancelInputsAddJob']._serialized_options = b'\202\323\344\223\002r2N/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/inputs/jobs/add/{id}:\001*Z\0352\030/v2/inputs/jobs/add/{id}:\001*\230\234\'\002\220\234\'-\220\234\'\004\220\234\'\005'
   _V2.methods_by_name['PostUploads']._options = None
-  _V2.methods_by_name['PostUploads']._serialized_options = b'\202\323\344\223\002X\"A/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/uploads:\001*Z\020\"\013/v2/uploads:\001*\230\234\'\002\220\234\'\201\001\220\234\'\200\001'
+  _V2.methods_by_name['PostUploads']._serialized_options = b'\202\323\344\223\002X\"A/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/uploads:\001*Z\020\"\013/v2/uploads:\001*\230\234\'\002\220\234\'-\220\234\'\201\001\220\234\'\200\001'
   _V2.methods_by_name['PutUploadContentParts']._options = None
-  _V2.methods_by_name['PutUploadContentParts']._serialized_options = b'\202\323\344\223\002\211\001\032[/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/uploads/{upload_id}/content_parts:\001*Z\'\032%/v2/uploads/{upload_id}/content_parts\230\234\'\002\220\234\'\201\001\220\234\'\200\001'
+  _V2.methods_by_name['PutUploadContentParts']._serialized_options = b'\202\323\344\223\002\211\001\032[/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/uploads/{upload_id}/content_parts:\001*Z\'\032%/v2/uploads/{upload_id}/content_parts\230\234\'\002\220\234\'-\220\234\'\201\001\220\234\'\200\001'
   _V2.methods_by_name['GetUpload']._options = None
-  _V2.methods_by_name['GetUpload']._serialized_options = b'\202\323\344\223\002j\022M/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/uploads/{upload_id}Z\031\022\027/v2/uploads/{upload_id}\230\234\'\002\220\234\'\200\001'
+  _V2.methods_by_name['GetUpload']._serialized_options = b'\202\323\344\223\002j\022M/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/uploads/{upload_id}Z\031\022\027/v2/uploads/{upload_id}\230\234\'\002\220\234\'-\220\234\'\200\001'
   _V2.methods_by_name['ListUploads']._options = None
-  _V2.methods_by_name['ListUploads']._serialized_options = b'\202\323\344\223\002R\022A/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/uploadsZ\r\022\013/v2/uploads\230\234\'\002\220\234\'\200\001'
+  _V2.methods_by_name['ListUploads']._serialized_options = b'\202\323\344\223\002R\022A/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/uploadsZ\r\022\013/v2/uploads\230\234\'\002\220\234\'-\220\234\'\200\001'
   _V2.methods_by_name['DeleteUploads']._options = None
-  _V2.methods_by_name['DeleteUploads']._serialized_options = b'\202\323\344\223\002X*A/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/uploads:\001*Z\020*\013/v2/uploads:\001*\230\234\'\002\220\234\'\200\001\220\234\'\201\001\220\234\'\202\001'
+  _V2.methods_by_name['DeleteUploads']._serialized_options = b'\202\323\344\223\002X*A/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/uploads:\001*Z\020*\013/v2/uploads:\001*\230\234\'\002\220\234\'-\220\234\'\200\001\220\234\'\201\001\220\234\'\202\001'
   _V2.methods_by_name['PostInputsDataSources']._options = None
-  _V2.methods_by_name['PostInputsDataSources']._serialized_options = b'\202\323\344\223\002p\"M/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/inputs/data_sources:\001*Z\034\"\027/v2/inputs/data_sources:\001*\230\234\'\002\220\234\'%\220\234\'&\220\234\'\013\220\234\'\004\220\234\'\005\220\234\'\017\220\234\'\002\220\234\'\023'
+  _V2.methods_by_name['PostInputsDataSources']._serialized_options = b'\202\323\344\223\002p\"M/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/inputs/data_sources:\001*Z\034\"\027/v2/inputs/data_sources:\001*\230\234\'\002\220\234\'-\220\234\'%\220\234\'&\220\234\'\013\220\234\'\004\220\234\'\005\220\234\'\017\220\234\'\002\220\234\'\023'
   _V2.methods_by_name['GetInputsExtractionJob']._options = None
-  _V2.methods_by_name['GetInputsExtractionJob']._serialized_options = b'\202\323\344\223\002\246\001\022k/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/inputs/jobs/extraction/{inputs_extraction_job_id}Z7\0225/v2/inputs/jobs/extraction/{inputs_extraction_job_id}\230\234\'\002\220\234\'\005'
+  _V2.methods_by_name['GetInputsExtractionJob']._serialized_options = b'\202\323\344\223\002\246\001\022k/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/inputs/jobs/extraction/{inputs_extraction_job_id}Z7\0225/v2/inputs/jobs/extraction/{inputs_extraction_job_id}\230\234\'\002\220\234\'-\220\234\'\005'
   _V2.methods_by_name['ListInputsExtractionJobs']._options = None
-  _V2.methods_by_name['ListInputsExtractionJobs']._serialized_options = b'\202\323\344\223\002p\022P/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/inputs/jobs/extractionZ\034\022\032/v2/inputs/jobs/extraction\230\234\'\002\220\234\'\005'
+  _V2.methods_by_name['ListInputsExtractionJobs']._serialized_options = b'\202\323\344\223\002p\022P/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/inputs/jobs/extractionZ\034\022\032/v2/inputs/jobs/extraction\230\234\'\002\220\234\'-\220\234\'\005'
   _V2.methods_by_name['CancelInputsExtractionJobs']._options = None
-  _V2.methods_by_name['CancelInputsExtractionJobs']._serialized_options = b'\202\323\344\223\002v2P/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/inputs/jobs/extraction:\001*Z\0372\032/v2/inputs/jobs/extraction:\001*\230\234\'\002\220\234\'\004\220\234\'\005'
+  _V2.methods_by_name['CancelInputsExtractionJobs']._serialized_options = b'\202\323\344\223\002v2P/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/inputs/jobs/extraction:\001*Z\0372\032/v2/inputs/jobs/extraction:\001*\230\234\'\002\220\234\'-\220\234\'\004\220\234\'\005'
   _V2.methods_by_name['PostInputsUploads']._options = None
-  _V2.methods_by_name['PostInputsUploads']._serialized_options = b'\202\323\344\223\002f\"H/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/inputs/uploads:\001*Z\027\"\022/v2/inputs/uploads:\001*\230\234\'\002\220\234\'%\220\234\'&\220\234\'\013\220\234\'\004\220\234\'\005\220\234\'\017\220\234\'\002\220\234\'\023\220\234\'\201\001\220\234\'\200\001'
-  _ORGANIZATIONINVITATIONSTATUS._serialized_start=40076
-  _ORGANIZATIONINVITATIONSTATUS._serialized_end=40188
+  _V2.methods_by_name['PostInputsUploads']._serialized_options = b'\202\323\344\223\002f\"H/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/inputs/uploads:\001*Z\027\"\022/v2/inputs/uploads:\001*\230\234\'\002\220\234\'-\220\234\'%\220\234\'&\220\234\'\013\220\234\'\004\220\234\'\005\220\234\'\017\220\234\'\002\220\234\'\023\220\234\'\201\001\220\234\'\200\001'
+  _ORGANIZATIONINVITATIONSTATUS._serialized_start=40733
+  _ORGANIZATIONINVITATIONSTATUS._serialized_end=40845
   _PAGINATION._serialized_start=420
   _PAGINATION._serialized_end=464
   _GETANNOTATIONREQUEST._serialized_start=466
   _GETANNOTATIONREQUEST._serialized_end=578
   _LISTANNOTATIONSREQUEST._serialized_start=581
   _LISTANNOTATIONSREQUEST._serialized_end=892
   _POSTANNOTATIONSREQUEST._serialized_start=894
   _POSTANNOTATIONSREQUEST._serialized_end=1014
   _PATCHANNOTATIONSREQUEST._serialized_start=1017
-  _PATCHANNOTATIONSREQUEST._serialized_end=1154
-  _PATCHANNOTATIONSSTATUSREQUEST._serialized_start=1157
-  _PATCHANNOTATIONSSTATUSREQUEST._serialized_end=1342
-  _PATCHANNOTATIONSSTATUSRESPONSE._serialized_start=1344
-  _PATCHANNOTATIONSSTATUSRESPONSE._serialized_end=1462
-  _DELETEANNOTATIONREQUEST._serialized_start=1464
-  _DELETEANNOTATIONREQUEST._serialized_end=1579
-  _DELETEANNOTATIONSREQUEST._serialized_start=1581
-  _DELETEANNOTATIONSREQUEST._serialized_end=1688
-  _SINGLEANNOTATIONRESPONSE._serialized_start=1690
-  _SINGLEANNOTATIONRESPONSE._serialized_end=1807
-  _MULTIANNOTATIONRESPONSE._serialized_start=1809
-  _MULTIANNOTATIONRESPONSE._serialized_end=1932
-  _GETAPPREQUEST._serialized_start=1934
-  _GETAPPREQUEST._serialized_end=2025
-  _LISTAPPSREQUEST._serialized_start=2028
-  _LISTAPPSREQUEST._serialized_end=2321
-  _POSTAPPSREQUEST._serialized_start=2323
-  _POSTAPPSREQUEST._serialized_end=2422
-  _DELETEAPPREQUEST._serialized_start=2424
-  _DELETEAPPREQUEST._serialized_end=2491
-  _PATCHAPPSREQUEST._serialized_start=2494
-  _PATCHAPPSREQUEST._serialized_end=2679
-  _PATCHAPPREQUEST._serialized_start=2682
-  _PATCHAPPREQUEST._serialized_end=2865
-  _PATCHAPPSIDSREQUEST._serialized_start=2868
-  _PATCHAPPSIDSREQUEST._serialized_end=2997
-  _POSTAPPSSEARCHESREQUEST._serialized_start=3000
-  _POSTAPPSSEARCHESREQUEST._serialized_end=3163
-  _SINGLEAPPRESPONSE._serialized_start=3165
-  _SINGLEAPPRESPONSE._serialized_end=3261
-  _MULTIAPPRESPONSE._serialized_start=3263
-  _MULTIAPPRESPONSE._serialized_end=3365
-  _LISTCOLLABORATORSREQUEST._serialized_start=3368
-  _LISTCOLLABORATORSREQUEST._serialized_end=3507
-  _POSTCOLLABORATORSREQUEST._serialized_start=3509
-  _POSTCOLLABORATORSREQUEST._serialized_end=3635
-  _PATCHCOLLABORATORSREQUEST._serialized_start=3638
-  _PATCHCOLLABORATORSREQUEST._serialized_end=3781
-  _DELETECOLLABORATORSREQUEST._serialized_start=3783
-  _DELETECOLLABORATORSREQUEST._serialized_end=3907
-  _MULTICOLLABORATORSRESPONSE._serialized_start=3910
-  _MULTICOLLABORATORSRESPONSE._serialized_end=4040
-  _LISTCOLLABORATIONSREQUEST._serialized_start=4042
-  _LISTCOLLABORATIONSREQUEST._serialized_end=4150
-  _MULTICOLLABORATIONSRESPONSE._serialized_start=4153
-  _MULTICOLLABORATIONSRESPONSE._serialized_end=4286
-  _GETSTATUSCODEREQUEST._serialized_start=4288
-  _GETSTATUSCODEREQUEST._serialized_end=4334
-  _LISTSTATUSCODESREQUEST._serialized_start=4336
-  _LISTSTATUSCODESREQUEST._serialized_end=4360
-  _SINGLESTATUSCODERESPONSE._serialized_start=4362
-  _SINGLESTATUSCODERESPONSE._serialized_end=4433
-  _MULTISTATUSCODERESPONSE._serialized_start=4435
-  _MULTISTATUSCODERESPONSE._serialized_end=4552
-  _GETCONCEPTREQUEST._serialized_start=4554
-  _GETCONCEPTREQUEST._serialized_end=4642
-  _LISTCONCEPTSREQUEST._serialized_start=4644
-  _LISTCONCEPTSREQUEST._serialized_end=4746
-  _LISTMODELCONCEPTSREQUEST._serialized_start=4749
-  _LISTMODELCONCEPTSREQUEST._serialized_end=4894
-  _POSTCONCEPTSSEARCHESREQUEST._serialized_start=4897
-  _POSTCONCEPTSSEARCHESREQUEST._serialized_end=5072
-  _POSTCONCEPTSREQUEST._serialized_start=5074
-  _POSTCONCEPTSREQUEST._serialized_end=5185
-  _PATCHCONCEPTSREQUEST._serialized_start=5188
-  _PATCHCONCEPTSREQUEST._serialized_end=5316
-  _GETCONCEPTCOUNTSREQUEST._serialized_start=5318
-  _GETCONCEPTCOUNTSREQUEST._serialized_end=5424
-  _SINGLECONCEPTRESPONSE._serialized_start=5426
-  _SINGLECONCEPTRESPONSE._serialized_end=5534
-  _MULTICONCEPTRESPONSE._serialized_start=5536
-  _MULTICONCEPTRESPONSE._serialized_end=5650
-  _MULTICONCEPTCOUNTRESPONSE._serialized_start=5653
-  _MULTICONCEPTCOUNTRESPONSE._serialized_end=5783
-  _LISTCONCEPTRELATIONSREQUEST._serialized_start=5786
-  _LISTCONCEPTRELATIONSREQUEST._serialized_end=5963
-  _POSTCONCEPTRELATIONSREQUEST._serialized_start=5966
-  _POSTCONCEPTRELATIONSREQUEST._serialized_end=6122
-  _DELETECONCEPTRELATIONSREQUEST._serialized_start=6124
-  _DELETECONCEPTRELATIONSREQUEST._serialized_end=6237
-  _LISTKNOWLEDGEGRAPHSREQUEST._serialized_start=6239
-  _LISTKNOWLEDGEGRAPHSREQUEST._serialized_end=6316
-  _POSTKNOWLEDGEGRAPHSREQUEST._serialized_start=6319
-  _POSTKNOWLEDGEGRAPHSREQUEST._serialized_end=6452
-  _POSTCONCEPTMAPPINGJOBSREQUEST._serialized_start=6455
-  _POSTCONCEPTMAPPINGJOBSREQUEST._serialized_end=6598
-  _MULTICONCEPTRELATIONRESPONSE._serialized_start=6601
-  _MULTICONCEPTRELATIONRESPONSE._serialized_end=6740
-  _MULTIKNOWLEDGEGRAPHRESPONSE._serialized_start=6743
-  _MULTIKNOWLEDGEGRAPHRESPONSE._serialized_end=6879
-  _MULTICONCEPTMAPPINGJOBRESPONSE._serialized_start=6881
-  _MULTICONCEPTMAPPINGJOBRESPONSE._serialized_end=6971
-  _GETCONCEPTLANGUAGEREQUEST._serialized_start=6973
-  _GETCONCEPTLANGUAGEREQUEST._serialized_end=7087
-  _LISTCONCEPTLANGUAGESREQUEST._serialized_start=7090
-  _LISTCONCEPTLANGUAGESREQUEST._serialized_end=7220
-  _PATCHCONCEPTLANGUAGESREQUEST._serialized_start=7223
-  _PATCHCONCEPTLANGUAGESREQUEST._serialized_end=7396
-  _POSTCONCEPTLANGUAGESREQUEST._serialized_start=7399
-  _POSTCONCEPTLANGUAGESREQUEST._serialized_end=7555
-  _SINGLECONCEPTLANGUAGERESPONSE._serialized_start=7558
-  _SINGLECONCEPTLANGUAGERESPONSE._serialized_end=7691
-  _MULTICONCEPTLANGUAGERESPONSE._serialized_start=7694
-  _MULTICONCEPTLANGUAGERESPONSE._serialized_end=7833
-  _GETINPUTREQUEST._serialized_start=7835
-  _GETINPUTREQUEST._serialized_end=7919
-  _GETVIDEOMANIFESTREQUEST._serialized_start=7921
-  _GETVIDEOMANIFESTREQUEST._serialized_end=8013
-  _GETINPUTSAMPLESREQUEST._serialized_start=8015
-  _GETINPUTSAMPLESREQUEST._serialized_end=8123
-  _LISTINPUTSREQUEST._serialized_start=8126
-  _LISTINPUTSREQUEST._serialized_end=8284
-  _STREAMINPUTSREQUEST._serialized_start=8287
-  _STREAMINPUTSREQUEST._serialized_end=8433
-  _POSTINPUTSREQUEST._serialized_start=8436
-  _POSTINPUTSREQUEST._serialized_end=8568
-  _PATCHINPUTSREQUEST._serialized_start=8570
-  _PATCHINPUTSREQUEST._serialized_end=8692
-  _DELETEINPUTREQUEST._serialized_start=8694
-  _DELETEINPUTREQUEST._serialized_end=8781
-  _DELETEINPUTSREQUEST._serialized_start=8783
-  _DELETEINPUTSREQUEST._serialized_end=8872
-  _SINGLEINPUTRESPONSE._serialized_start=8874
-  _SINGLEINPUTRESPONSE._serialized_end=8976
-  _GETVIDEOMANIFESTRESPONSE._serialized_start=8978
-  _GETVIDEOMANIFESTRESPONSE._serialized_end=9071
-  _MULTIINPUTRESPONSE._serialized_start=9074
-  _MULTIINPUTRESPONSE._serialized_end=9234
-  _MULTIINPUTANNOTATIONRESPONSE._serialized_start=9236
-  _MULTIINPUTANNOTATIONRESPONSE._serialized_end=9350
-  _SINGLEINPUTCOUNTRESPONSE._serialized_start=9352
-  _SINGLEINPUTCOUNTRESPONSE._serialized_end=9465
-  _GETINPUTCOUNTREQUEST._serialized_start=9467
-  _GETINPUTCOUNTREQUEST._serialized_end=9538
-  _LISTDATASETSREQUEST._serialized_start=9541
-  _LISTDATASETSREQUEST._serialized_end=9692
-  _GETDATASETREQUEST._serialized_start=9694
-  _GETDATASETREQUEST._serialized_end=9809
-  _POSTDATASETSREQUEST._serialized_start=9811
-  _POSTDATASETSREQUEST._serialized_end=9922
-  _PATCHDATASETSREQUEST._serialized_start=9925
-  _PATCHDATASETSREQUEST._serialized_end=10053
-  _PATCHDATASETIDSREQUEST._serialized_start=10056
-  _PATCHDATASETIDSREQUEST._serialized_end=10188
-  _DELETEDATASETSREQUEST._serialized_start=10190
-  _DELETEDATASETSREQUEST._serialized_end=10283
-  _MULTIDATASETRESPONSE._serialized_start=10285
-  _MULTIDATASETRESPONSE._serialized_end=10399
-  _SINGLEDATASETRESPONSE._serialized_start=10401
-  _SINGLEDATASETRESPONSE._serialized_end=10509
-  _LISTDATASETINPUTSREQUEST._serialized_start=10511
-  _LISTDATASETINPUTSREQUEST._serialized_end=10638
-  _GETDATASETINPUTREQUEST._serialized_start=10640
-  _GETDATASETINPUTREQUEST._serialized_end=10751
-  _POSTDATASETINPUTSREQUEST._serialized_start=10754
-  _POSTDATASETINPUTSREQUEST._serialized_end=10939
-  _DELETEDATASETINPUTSREQUEST._serialized_start=10941
-  _DELETEDATASETINPUTSREQUEST._serialized_end=11057
-  _MULTIDATASETINPUTRESPONSE._serialized_start=11060
-  _MULTIDATASETINPUTRESPONSE._serialized_end=11270
-  _SINGLEDATASETINPUTRESPONSE._serialized_start=11272
-  _SINGLEDATASETINPUTRESPONSE._serialized_end=11396
-  _LISTDATASETVERSIONSREQUEST._serialized_start=11399
-  _LISTDATASETVERSIONSREQUEST._serialized_end=11528
-  _GETDATASETVERSIONREQUEST._serialized_start=11530
-  _GETDATASETVERSIONREQUEST._serialized_end=11653
-  _LISTDATASETVERSIONMETRICSGROUPSREQUEST._serialized_start=11656
-  _LISTDATASETVERSIONMETRICSGROUPSREQUEST._serialized_end=11948
-  _POSTDATASETVERSIONSREQUEST._serialized_start=11951
-  _POSTDATASETVERSIONSREQUEST._serialized_end=12104
-  _PATCHDATASETVERSIONSREQUEST._serialized_start=12107
-  _PATCHDATASETVERSIONSREQUEST._serialized_end=12277
-  _DELETEDATASETVERSIONSREQUEST._serialized_start=12280
-  _DELETEDATASETVERSIONSREQUEST._serialized_end=12408
-  _PUTDATASETVERSIONEXPORTSREQUEST._serialized_start=12411
-  _PUTDATASETVERSIONEXPORTSREQUEST._serialized_end=12594
-  _MULTIDATASETVERSIONRESPONSE._serialized_start=12597
-  _MULTIDATASETVERSIONRESPONSE._serialized_end=12733
-  _MULTIDATASETVERSIONEXPORTRESPONSE._serialized_start=12736
-  _MULTIDATASETVERSIONEXPORTRESPONSE._serialized_end=12875
-  _MULTIDATASETVERSIONMETRICSGROUPRESPONSE._serialized_start=12878
-  _MULTIDATASETVERSIONMETRICSGROUPRESPONSE._serialized_end=13052
-  _SINGLEDATASETVERSIONRESPONSE._serialized_start=13055
-  _SINGLEDATASETVERSIONRESPONSE._serialized_end=13185
-  _GETDATASETINPUTSSEARCHADDJOBREQUEST._serialized_start=13187
-  _GETDATASETINPUTSSEARCHADDJOBREQUEST._serialized_end=13289
-  _SINGLEDATASETINPUTSSEARCHADDJOBRESPONSE._serialized_start=13292
-  _SINGLEDATASETINPUTSSEARCHADDJOBRESPONSE._serialized_end=13432
-  _POSTMODELOUTPUTSREQUEST._serialized_start=13435
-  _POSTMODELOUTPUTSREQUEST._serialized_end=13620
-  _LISTMODELINPUTSREQUEST._serialized_start=13623
-  _LISTMODELINPUTSREQUEST._serialized_end=13766
-  _GETKEYREQUEST._serialized_start=13768
-  _GETKEYREQUEST._serialized_end=13848
-  _LISTKEYSREQUEST._serialized_start=13851
-  _LISTKEYSREQUEST._serialized_end=14005
-  _LISTAPPKEYSREQUEST._serialized_start=14007
-  _LISTAPPKEYSREQUEST._serialized_end=14108
-  _POSTKEYSREQUEST._serialized_start=14110
-  _POSTKEYSREQUEST._serialized_end=14209
-  _DELETEKEYREQUEST._serialized_start=14211
-  _DELETEKEYREQUEST._serialized_end=14294
-  _PATCHKEYSREQUEST._serialized_start=14296
-  _PATCHKEYSREQUEST._serialized_end=14412
-  _SINGLEKEYRESPONSE._serialized_start=14414
-  _SINGLEKEYRESPONSE._serialized_end=14510
-  _MULTIKEYRESPONSE._serialized_start=14512
-  _MULTIKEYRESPONSE._serialized_end=14614
-  _GETMODELREQUEST._serialized_start=14617
-  _GETMODELREQUEST._serialized_end=14790
-  _LISTMODELSREQUEST._serialized_start=14793
-  _LISTMODELSREQUEST._serialized_end=15340
-  _PATCHMODELTOOLKITSREQUEST._serialized_start=15343
-  _PATCHMODELTOOLKITSREQUEST._serialized_end=15471
-  _PATCHMODELCHECKCONSENTSREQUEST._serialized_start=15474
-  _PATCHMODELCHECKCONSENTSREQUEST._serialized_end=15613
-  _PATCHMODELUSECASESREQUEST._serialized_start=15616
-  _PATCHMODELUSECASESREQUEST._serialized_end=15744
-  _PATCHMODELLANGUAGESREQUEST._serialized_start=15747
-  _PATCHMODELLANGUAGESREQUEST._serialized_end=15877
-  _MULTIMODELTOOLKITRESPONSE._serialized_start=15879
-  _MULTIMODELTOOLKITRESPONSE._serialized_end=15969
-  _MULTIMODELCHECKCONSENTRESPONSE._serialized_start=15971
-  _MULTIMODELCHECKCONSENTRESPONSE._serialized_end=16072
-  _MULTIMODELUSECASERESPONSE._serialized_start=16074
-  _MULTIMODELUSECASERESPONSE._serialized_end=16164
-  _MULTIMODELLANGUAGERESPONSE._serialized_start=16166
-  _MULTIMODELLANGUAGERESPONSE._serialized_end=16258
-  _POSTMODELSREQUEST._serialized_start=16261
-  _POSTMODELSREQUEST._serialized_end=16406
-  _PATCHMODELSREQUEST._serialized_start=16408
-  _PATCHMODELSREQUEST._serialized_end=16530
-  _IDUPDATESOURCE._serialized_start=16532
-  _IDUPDATESOURCE._serialized_end=16576
-  _PATCHMODELIDSREQUEST._serialized_start=16579
-  _PATCHMODELIDSREQUEST._serialized_end=16709
-  _DELETEMODELREQUEST._serialized_start=16711
-  _DELETEMODELREQUEST._serialized_end=16798
-  _DELETEMODELSREQUEST._serialized_start=16800
-  _DELETEMODELSREQUEST._serialized_end=16903
-  _POSTMODELSSEARCHESREQUEST._serialized_start=16906
-  _POSTMODELSSEARCHESREQUEST._serialized_end=17075
-  _SINGLEMODELRESPONSE._serialized_start=17077
-  _SINGLEMODELRESPONSE._serialized_end=17179
-  _MULTIMODELRESPONSE._serialized_start=17181
-  _MULTIMODELRESPONSE._serialized_end=17289
-  _PATCHMODELVERSIONSREQUEST._serialized_start=17292
-  _PATCHMODELVERSIONSREQUEST._serialized_end=17454
-  _GETMODELVERSIONREQUEST._serialized_start=17456
-  _GETMODELVERSIONREQUEST._serialized_end=17567
-  _LISTMODELVERSIONSREQUEST._serialized_start=17570
-  _LISTMODELVERSIONSREQUEST._serialized_end=17895
-  _DELETEMODELVERSIONREQUEST._serialized_start=17897
-  _DELETEMODELVERSIONREQUEST._serialized_end=18011
-  _SINGLEMODELVERSIONRESPONSE._serialized_start=18013
-  _SINGLEMODELVERSIONRESPONSE._serialized_end=18137
-  _MULTIMODELVERSIONRESPONSE._serialized_start=18140
-  _MULTIMODELVERSIONRESPONSE._serialized_end=18270
-  _POSTMODELVERSIONSREQUEST._serialized_start=18273
-  _POSTMODELVERSIONSREQUEST._serialized_end=18512
-  _POSTWORKFLOWVERSIONSUNPUBLISHREQUEST._serialized_start=18515
-  _POSTWORKFLOWVERSIONSUNPUBLISHREQUEST._serialized_end=18692
-  _POSTWORKFLOWVERSIONSPUBLISHREQUEST._serialized_start=18695
-  _POSTWORKFLOWVERSIONSPUBLISHREQUEST._serialized_end=18868
-  _WORKFLOWVERSIONPUBLISHREQUEST._serialized_start=18870
-  _WORKFLOWVERSIONPUBLISHREQUEST._serialized_end=18921
-  _WORKFLOWVERSIONUNPUBLISHREQUEST._serialized_start=18923
-  _WORKFLOWVERSIONUNPUBLISHREQUEST._serialized_end=18976
-  _MODELVERSIONPUBLISHREQUEST._serialized_start=18978
-  _MODELVERSIONPUBLISHREQUEST._serialized_end=19026
-  _POSTMODELVERSIONSPUBLISHREQUEST._serialized_start=19029
-  _POSTMODELVERSIONSPUBLISHREQUEST._serialized_end=19193
-  _MODELVERSIONUNPUBLISHREQUEST._serialized_start=19195
-  _MODELVERSIONUNPUBLISHREQUEST._serialized_end=19245
-  _POSTMODELVERSIONSUNPUBLISHREQUEST._serialized_start=19248
-  _POSTMODELVERSIONSUNPUBLISHREQUEST._serialized_end=19416
-  _POSTMODELVERSIONEVALUATIONSREQUEST._serialized_start=19419
-  _POSTMODELVERSIONEVALUATIONSREQUEST._serialized_end=19597
-  _LISTMODELVERSIONEVALUATIONSREQUEST._serialized_start=19600
-  _LISTMODELVERSIONEVALUATIONSREQUEST._serialized_end=19761
-  _GETMODELVERSIONEVALUATIONREQUEST._serialized_start=19764
-  _GETMODELVERSIONEVALUATIONREQUEST._serialized_end=19957
-  _SINGLEEVALMETRICSRESPONSE._serialized_start=19959
-  _SINGLEEVALMETRICSRESPONSE._serialized_end=20080
-  _MULTIEVALMETRICSRESPONSE._serialized_start=20082
-  _MULTIEVALMETRICSRESPONSE._serialized_end=20202
-  _POSTMODELVERSIONMETRICSREQUEST._serialized_start=20205
-  _POSTMODELVERSIONMETRICSREQUEST._serialized_end=20416
-  _GETMODELVERSIONMETRICSREQUEST._serialized_start=20419
-  _GETMODELVERSIONMETRICSREQUEST._serialized_end=20580
-  _GETMODELTYPEREQUEST._serialized_start=20582
-  _GETMODELTYPEREQUEST._serialized_end=20675
-  _LISTMODELTYPESREQUEST._serialized_start=20677
-  _LISTMODELTYPESREQUEST._serialized_end=20781
-  _LISTOPENSOURCELICENSESREQUEST._serialized_start=20783
-  _LISTOPENSOURCELICENSESREQUEST._serialized_end=20814
-  _LISTOPENSOURCELICENSESRESPONSE._serialized_start=20816
-  _LISTOPENSOURCELICENSESRESPONSE._serialized_end=20911
-  _SINGLEMODELTYPERESPONSE._serialized_start=20913
-  _SINGLEMODELTYPERESPONSE._serialized_end=21034
-  _MULTIMODELTYPERESPONSE._serialized_start=21037
-  _MULTIMODELTYPERESPONSE._serialized_end=21279
-  _GETMODELVERSIONINPUTEXAMPLEREQUEST._serialized_start=21282
-  _GETMODELVERSIONINPUTEXAMPLEREQUEST._serialized_end=21431
-  _LISTMODELVERSIONINPUTEXAMPLESREQUEST._serialized_start=21434
-  _LISTMODELVERSIONINPUTEXAMPLESREQUEST._serialized_end=21597
-  _SINGLEMODELVERSIONINPUTEXAMPLERESPONSE._serialized_start=21600
-  _SINGLEMODELVERSIONINPUTEXAMPLERESPONSE._serialized_end=21762
-  _MULTIMODELVERSIONINPUTEXAMPLERESPONSE._serialized_start=21765
-  _MULTIMODELVERSIONINPUTEXAMPLERESPONSE._serialized_end=21927
-  _LISTMODELREFERENCESREQUEST._serialized_start=21929
-  _LISTMODELREFERENCESREQUEST._serialized_end=22056
-  _MULTIMODELREFERENCERESPONSE._serialized_start=22059
-  _MULTIMODELREFERENCERESPONSE._serialized_end=22189
-  _MULTIOUTPUTRESPONSE._serialized_start=22191
-  _MULTIOUTPUTRESPONSE._serialized_end=22302
-  _LISTSCOPESREQUEST._serialized_start=22304
-  _LISTSCOPESREQUEST._serialized_end=22390
-  _MYSCOPESREQUEST._serialized_start=22392
-  _MYSCOPESREQUEST._serialized_end=22458
-  _MYSCOPESUSERREQUEST._serialized_start=22460
-  _MYSCOPESUSERREQUEST._serialized_end=22530
-  _MYSCOPESROOTREQUEST._serialized_start=22532
-  _MYSCOPESROOTREQUEST._serialized_end=22553
-  _MULTISCOPEDEPSRESPONSE._serialized_start=22556
-  _MULTISCOPEDEPSRESPONSE._serialized_end=22721
-  _MULTISCOPERESPONSE._serialized_start=22724
-  _MULTISCOPERESPONSE._serialized_end=22884
-  _MULTISCOPEUSERRESPONSE._serialized_start=22887
-  _MULTISCOPEUSERRESPONSE._serialized_end=23019
-  _MULTISCOPEROOTRESPONSE._serialized_start=23022
-  _MULTISCOPEROOTRESPONSE._serialized_end=23154
-  _GETSEARCHREQUEST._serialized_start=23156
-  _GETSEARCHREQUEST._serialized_end=23235
-  _LISTSEARCHESREQUEST._serialized_start=23237
-  _LISTSEARCHESREQUEST._serialized_end=23339
-  _POSTSEARCHESREQUEST._serialized_start=23342
-  _POSTSEARCHESREQUEST._serialized_end=23538
-  _PATCHINPUTSSEARCHESREQUEST._serialized_start=23541
-  _PATCHINPUTSSEARCHESREQUEST._serialized_end=23674
-  _PATCHANNOTATIONSSEARCHESREQUEST._serialized_start=23677
-  _PATCHANNOTATIONSSEARCHESREQUEST._serialized_end=23815
-  _PATCHSEARCHESREQUEST._serialized_start=23817
-  _PATCHSEARCHESREQUEST._serialized_end=23944
-  _POSTSEARCHESBYIDREQUEST._serialized_start=23947
-  _POSTSEARCHESBYIDREQUEST._serialized_end=24079
-  _DELETESEARCHREQUEST._serialized_start=24081
-  _DELETESEARCHREQUEST._serialized_end=24163
-  _POSTANNOTATIONSSEARCHESREQUEST._serialized_start=24166
-  _POSTANNOTATIONSSEARCHESREQUEST._serialized_end=24333
-  _DELETEANNOTATIONSEARCHMETRICSREQUEST._serialized_start=24335
-  _DELETEANNOTATIONSEARCHMETRICSREQUEST._serialized_end=24434
-  _POSTINPUTSSEARCHESREQUEST._serialized_start=24437
-  _POSTINPUTSSEARCHESREQUEST._serialized_end=24619
-  _SINGLESEARCHRESPONSE._serialized_start=24621
-  _SINGLESEARCHRESPONSE._serialized_end=24726
-  _MULTISEARCHRESPONSE._serialized_start=24729
-  _MULTISEARCHRESPONSE._serialized_end=24966
-  _POSTANNOTATIONSEARCHMETRICSREQUEST._serialized_start=24969
-  _POSTANNOTATIONSEARCHMETRICSREQUEST._serialized_end=25245
-  _GETANNOTATIONSEARCHMETRICSREQUEST._serialized_start=25247
-  _GETANNOTATIONSEARCHMETRICSREQUEST._serialized_end=25343
-  _LISTANNOTATIONSEARCHMETRICSREQUEST._serialized_start=25345
-  _LISTANNOTATIONSEARCHMETRICSREQUEST._serialized_end=25430
-  _MULTIANNOTATIONSEARCHMETRICSRESPONSE._serialized_start=25433
-  _MULTIANNOTATIONSEARCHMETRICSRESPONSE._serialized_end=25590
-  _LISTANNOTATIONFILTERSREQUEST._serialized_start=25592
-  _LISTANNOTATIONFILTERSREQUEST._serialized_end=25703
-  _GETANNOTATIONFILTERREQUEST._serialized_start=25705
-  _GETANNOTATIONFILTERREQUEST._serialized_end=25812
-  _POSTANNOTATIONFILTERSREQUEST._serialized_start=25815
-  _POSTANNOTATIONFILTERSREQUEST._serialized_end=25954
-  _PATCHANNOTATIONFILTERSREQUEST._serialized_start=25957
-  _PATCHANNOTATIONFILTERSREQUEST._serialized_end=26113
-  _DELETEANNOTATIONFILTERSREQUEST._serialized_start=26115
-  _DELETEANNOTATIONFILTERSREQUEST._serialized_end=26227
-  _MULTIANNOTATIONFILTERRESPONSE._serialized_start=26230
-  _MULTIANNOTATIONFILTERRESPONSE._serialized_end=26372
-  _SINGLEANNOTATIONFILTERRESPONSE._serialized_start=26375
-  _SINGLEANNOTATIONFILTERRESPONSE._serialized_end=26511
-  _GETUSERREQUEST._serialized_start=26513
-  _GETUSERREQUEST._serialized_end=26605
-  _SINGLEUSERRESPONSE._serialized_start=26607
-  _SINGLEUSERRESPONSE._serialized_end=26706
-  _POSTVALIDATEPASSWORDREQUEST._serialized_start=26708
-  _POSTVALIDATEPASSWORDREQUEST._serialized_end=26828
-  _SINGLEPASSWORDVALIDATIONRESPONSE._serialized_start=26831
-  _SINGLEPASSWORDVALIDATIONRESPONSE._serialized_end=26973
-  _GETWORKFLOWREQUEST._serialized_start=26976
-  _GETWORKFLOWREQUEST._serialized_end=27163
-  _LISTWORKFLOWSREQUEST._serialized_start=27166
-  _LISTWORKFLOWSREQUEST._serialized_end=27481
-  _POSTWORKFLOWSREQUEST._serialized_start=27483
-  _POSTWORKFLOWSREQUEST._serialized_end=27597
-  _PATCHWORKFLOWSREQUEST._serialized_start=27600
-  _PATCHWORKFLOWSREQUEST._serialized_end=27731
-  _PATCHWORKFLOWIDSREQUEST._serialized_start=27734
-  _PATCHWORKFLOWIDSREQUEST._serialized_end=27867
-  _DELETEWORKFLOWREQUEST._serialized_start=27869
-  _DELETEWORKFLOWREQUEST._serialized_end=27962
-  _DELETEWORKFLOWSREQUEST._serialized_start=27964
-  _DELETEWORKFLOWSREQUEST._serialized_end=28070
-  _SINGLEWORKFLOWRESPONSE._serialized_start=28072
-  _SINGLEWORKFLOWRESPONSE._serialized_end=28183
-  _MULTIWORKFLOWRESPONSE._serialized_start=28185
-  _MULTIWORKFLOWRESPONSE._serialized_end=28302
-  _POSTWORKFLOWRESULTSREQUEST._serialized_start=28305
-  _POSTWORKFLOWRESULTSREQUEST._serialized_end=28598
-  _POSTWORKFLOWRESULTSRESPONSE._serialized_start=28601
-  _POSTWORKFLOWRESULTSRESPONSE._serialized_end=28817
-  _POSTWORKFLOWRESULTSSIMILARITYREQUEST._serialized_start=28820
-  _POSTWORKFLOWRESULTSSIMILARITYREQUEST._serialized_end=29093
-  _POSTWORKFLOWRESULTSSIMILARITYRESPONSE._serialized_start=29096
-  _POSTWORKFLOWRESULTSSIMILARITYRESPONSE._serialized_end=29238
-  _LISTWORKFLOWVERSIONSREQUEST._serialized_start=29241
-  _LISTWORKFLOWVERSIONSREQUEST._serialized_end=29372
-  _GETWORKFLOWVERSIONREQUEST._serialized_start=29374
-  _GETWORKFLOWVERSIONREQUEST._serialized_end=29500
-  _DELETEWORKFLOWVERSIONSREQUEST._serialized_start=29503
-  _DELETEWORKFLOWVERSIONSREQUEST._serialized_end=29634
-  _PATCHWORKFLOWVERSIONSREQUEST._serialized_start=29637
-  _PATCHWORKFLOWVERSIONSREQUEST._serialized_end=29811
-  _MULTIWORKFLOWVERSIONRESPONSE._serialized_start=29814
-  _MULTIWORKFLOWVERSIONRESPONSE._serialized_end=29953
-  _SINGLEWORKFLOWVERSIONRESPONSE._serialized_start=29956
-  _SINGLEWORKFLOWVERSIONRESPONSE._serialized_end=30089
-  _POSTAPPDUPLICATIONSREQUEST._serialized_start=30092
-  _POSTAPPDUPLICATIONSREQUEST._serialized_end=30225
-  _GETAPPDUPLICATIONREQUEST._serialized_start=30227
-  _GETAPPDUPLICATIONREQUEST._serialized_end=30330
-  _LISTAPPDUPLICATIONSREQUEST._serialized_start=30332
-  _LISTAPPDUPLICATIONSREQUEST._serialized_end=30441
-  _MULTIAPPDUPLICATIONSRESPONSE._serialized_start=30444
-  _MULTIAPPDUPLICATIONSRESPONSE._serialized_end=30575
-  _SINGLEAPPDUPLICATIONRESPONSE._serialized_start=30578
-  _SINGLEAPPDUPLICATIONRESPONSE._serialized_end=30708
-  _POSTTASKSREQUEST._serialized_start=30710
-  _POSTTASKSREQUEST._serialized_end=30812
-  _GETTASKREQUEST._serialized_start=30814
-  _GETTASKREQUEST._serialized_end=30923
-  _LISTTASKSREQUEST._serialized_start=30926
-  _LISTTASKSREQUEST._serialized_end=31164
-  _PATCHTASKSREQUEST._serialized_start=31166
-  _PATCHTASKSREQUEST._serialized_end=31285
-  _DELETETASKSREQUEST._serialized_start=31287
-  _DELETETASKSREQUEST._serialized_end=31369
-  _MULTITASKRESPONSE._serialized_start=31371
-  _MULTITASKRESPONSE._serialized_end=31476
-  _SINGLETASKRESPONSE._serialized_start=31478
-  _SINGLETASKRESPONSE._serialized_end=31577
-  _GETTASKCOUNTREQUEST._serialized_start=31579
-  _GETTASKCOUNTREQUEST._serialized_end=31684
-  _SINGLETASKCOUNTRESPONSE._serialized_start=31687
-  _SINGLETASKCOUNTRESPONSE._serialized_end=31844
-  _POSTLABELORDERSREQUEST._serialized_start=31846
-  _POSTLABELORDERSREQUEST._serialized_end=31967
-  _GETLABELORDERREQUEST._serialized_start=31969
-  _GETLABELORDERREQUEST._serialized_end=32064
-  _LISTLABELORDERSREQUEST._serialized_start=32066
-  _LISTLABELORDERSREQUEST._serialized_end=32171
-  _PATCHLABELORDERSREQUEST._serialized_start=32174
-  _PATCHLABELORDERSREQUEST._serialized_end=32312
-  _DELETELABELORDERSREQUEST._serialized_start=32314
-  _DELETELABELORDERSREQUEST._serialized_end=32402
-  _MULTILABELORDERRESPONSE._serialized_start=32404
-  _MULTILABELORDERRESPONSE._serialized_end=32528
-  _SINGLELABELORDERRESPONSE._serialized_start=32530
-  _SINGLELABELORDERRESPONSE._serialized_end=32648
-  _POSTCOLLECTORSREQUEST._serialized_start=32650
-  _POSTCOLLECTORSREQUEST._serialized_end=32767
-  _PATCHCOLLECTORSREQUEST._serialized_start=32770
-  _PATCHCOLLECTORSREQUEST._serialized_end=32904
-  _DELETECOLLECTORSREQUEST._serialized_start=32906
-  _DELETECOLLECTORSREQUEST._serialized_end=33013
-  _GETCOLLECTORREQUEST._serialized_start=33015
-  _GETCOLLECTORREQUEST._serialized_end=33107
-  _LISTCOLLECTORSREQUEST._serialized_start=33109
-  _LISTCOLLECTORSREQUEST._serialized_end=33213
-  _MULTICOLLECTORRESPONSE._serialized_start=33215
-  _MULTICOLLECTORRESPONSE._serialized_end=33329
-  _SINGLECOLLECTORRESPONSE._serialized_start=33331
-  _SINGLECOLLECTORRESPONSE._serialized_end=33445
-  _POSTSTATVALUESREQUEST._serialized_start=33447
-  _POSTSTATVALUESREQUEST._serialized_end=33565
-  _MULTISTATVALUERESPONSE._serialized_start=33567
-  _MULTISTATVALUERESPONSE._serialized_end=33688
-  _POSTSTATVALUESAGGREGATEREQUEST._serialized_start=33691
-  _POSTSTATVALUESAGGREGATEREQUEST._serialized_end=33849
-  _MULTISTATVALUEAGGREGATERESPONSE._serialized_start=33852
-  _MULTISTATVALUEAGGREGATERESPONSE._serialized_end=34008
-  _POSTTRENDINGMETRICSVIEWREQUEST._serialized_start=34010
-  _POSTTRENDINGMETRICSVIEWREQUEST._serialized_end=34129
-  _LISTTRENDINGMETRICSVIEWSREQUEST._serialized_start=34132
-  _LISTTRENDINGMETRICSVIEWSREQUEST._serialized_end=34265
-  _MULTITRENDINGMETRICSVIEWRESPONSE._serialized_start=34267
-  _MULTITRENDINGMETRICSVIEWRESPONSE._serialized_end=34393
-  _GETMODULEREQUEST._serialized_start=34395
-  _GETMODULEREQUEST._serialized_end=34508
-  _LISTMODULESREQUEST._serialized_start=34511
-  _LISTMODULESREQUEST._serialized_end=34661
-  _POSTMODULESREQUEST._serialized_start=34663
-  _POSTMODULESREQUEST._serialized_end=34771
-  _PATCHMODULESREQUEST._serialized_start=34773
-  _PATCHMODULESREQUEST._serialized_end=34898
-  _DELETEMODULESREQUEST._serialized_start=34900
-  _DELETEMODULESREQUEST._serialized_end=34984
-  _SINGLEMODULERESPONSE._serialized_start=34986
-  _SINGLEMODULERESPONSE._serialized_end=35091
-  _MULTIMODULERESPONSE._serialized_start=35093
-  _MULTIMODULERESPONSE._serialized_end=35204
-  _GETMODULEVERSIONREQUEST._serialized_start=35206
-  _GETMODULEVERSIONREQUEST._serialized_end=35326
-  _LISTMODULEVERSIONSREQUEST._serialized_start=35328
-  _LISTMODULEVERSIONSREQUEST._serialized_end=35455
-  _POSTMODULEVERSIONSREQUEST._serialized_start=35458
-  _POSTMODULEVERSIONSREQUEST._serialized_end=35607
-  _DELETEMODULEVERSIONSREQUEST._serialized_start=35609
-  _DELETEMODULEVERSIONSREQUEST._serialized_end=35719
-  _SINGLEMODULEVERSIONRESPONSE._serialized_start=35721
-  _SINGLEMODULEVERSIONRESPONSE._serialized_end=35848
-  _MULTIMODULEVERSIONRESPONSE._serialized_start=35851
-  _MULTIMODULEVERSIONRESPONSE._serialized_end=35984
-  _GETINSTALLEDMODULEVERSIONREQUEST._serialized_start=35986
-  _GETINSTALLEDMODULEVERSIONREQUEST._serialized_end=36106
-  _LISTINSTALLEDMODULEVERSIONSREQUEST._serialized_start=36108
-  _LISTINSTALLEDMODULEVERSIONSREQUEST._serialized_end=36225
-  _POSTINSTALLEDMODULEVERSIONSREQUEST._serialized_start=36228
-  _POSTINSTALLEDMODULEVERSIONSREQUEST._serialized_end=36386
-  _POSTINSTALLEDMODULEVERSIONSKEYREQUEST._serialized_start=36388
-  _POSTINSTALLEDMODULEVERSIONSKEYREQUEST._serialized_end=36513
-  _DELETEINSTALLEDMODULEVERSIONSREQUEST._serialized_start=36515
-  _DELETEINSTALLEDMODULEVERSIONSREQUEST._serialized_end=36615
-  _SINGLEINSTALLEDMODULEVERSIONRESPONSE._serialized_start=36618
-  _SINGLEINSTALLEDMODULEVERSIONRESPONSE._serialized_end=36773
-  _MULTIINSTALLEDMODULEVERSIONRESPONSE._serialized_start=36776
-  _MULTIINSTALLEDMODULEVERSIONRESPONSE._serialized_end=36937
-  _LISTNEXTTASKASSIGNMENTSREQUEST._serialized_start=36939
-  _LISTNEXTTASKASSIGNMENTSREQUEST._serialized_end=37037
-  _POSTBULKOPERATIONSREQUEST._serialized_start=37040
-  _POSTBULKOPERATIONSREQUEST._serialized_end=37170
-  _LISTBULKOPERATIONSREQUEST._serialized_start=37172
-  _LISTBULKOPERATIONSREQUEST._serialized_end=37280
-  _GETBULKOPERATIONREQUEST._serialized_start=37282
-  _GETBULKOPERATIONREQUEST._serialized_end=37368
-  _CANCELBULKOPERATIONREQUEST._serialized_start=37370
-  _CANCELBULKOPERATIONREQUEST._serialized_end=37460
-  _DELETEBULKOPERATIONREQUEST._serialized_start=37462
-  _DELETEBULKOPERATIONREQUEST._serialized_end=37552
-  _SINGLEBULKOPERATIONSRESPONSE._serialized_start=37555
-  _SINGLEBULKOPERATIONSRESPONSE._serialized_end=37683
-  _MULTIBULKOPERATIONSRESPONSE._serialized_start=37685
-  _MULTIBULKOPERATIONSRESPONSE._serialized_end=37812
-  _PUTTASKASSIGNMENTSREQUEST._serialized_start=37814
-  _PUTTASKASSIGNMENTSREQUEST._serialized_end=37925
-  _LISTINPUTSADDJOBSREQUEST._serialized_start=37927
-  _LISTINPUTSADDJOBSREQUEST._serialized_end=38034
-  _GETINPUTSADDJOBREQUEST._serialized_start=38036
-  _GETINPUTSADDJOBREQUEST._serialized_end=38121
-  _MULTIINPUTSADDJOBRESPONSE._serialized_start=38124
-  _MULTIINPUTSADDJOBRESPONSE._serialized_end=38255
-  _SINGLEINPUTSADDJOBRESPONSE._serialized_start=38257
-  _SINGLEINPUTSADDJOBRESPONSE._serialized_end=38382
-  _POSTUPLOADSREQUEST._serialized_start=38384
-  _POSTUPLOADSREQUEST._serialized_end=38492
-  _DELETEUPLOADSREQUEST._serialized_start=38494
-  _DELETEUPLOADSREQUEST._serialized_end=38578
-  _LISTUPLOADSREQUEST._serialized_start=38580
-  _LISTUPLOADSREQUEST._serialized_end=38681
-  _GETUPLOADREQUEST._serialized_start=38683
-  _GETUPLOADREQUEST._serialized_end=38769
-  _SINGLEUPLOADRESPONSE._serialized_start=38771
-  _SINGLEUPLOADRESPONSE._serialized_end=38876
-  _MULTIUPLOADRESPONSE._serialized_start=38878
-  _MULTIUPLOADRESPONSE._serialized_end=38983
-  _PUTUPLOADCONTENTPARTSREQUEST._serialized_start=38986
-  _PUTUPLOADCONTENTPARTSREQUEST._serialized_end=39140
-  _POSTINPUTSDATASOURCESREQUEST._serialized_start=39143
-  _POSTINPUTSDATASOURCESREQUEST._serialized_end=39316
-  _GETINPUTSEXTRACTIONJOBREQUEST._serialized_start=39318
-  _GETINPUTSEXTRACTIONJOBREQUEST._serialized_end=39432
-  _LISTINPUTSEXTRACTIONJOBSREQUEST._serialized_start=39434
-  _LISTINPUTSEXTRACTIONJOBSREQUEST._serialized_end=39548
-  _SINGLEINPUTSEXTRACTIONJOBRESPONSE._serialized_start=39551
-  _SINGLEINPUTSEXTRACTIONJOBRESPONSE._serialized_end=39697
-  _MULTIINPUTSEXTRACTIONJOBRESPONSE._serialized_start=39700
-  _MULTIINPUTSEXTRACTIONJOBRESPONSE._serialized_end=39846
-  _CANCELINPUTSEXTRACTIONJOBSREQUEST._serialized_start=39848
-  _CANCELINPUTSEXTRACTIONJOBSREQUEST._serialized_end=39945
-  _POSTINPUTSUPLOADSREQUEST._serialized_start=39947
-  _POSTINPUTSUPLOADSREQUEST._serialized_end=40074
-  _V2._serialized_start=40192
-  _V2._serialized_end=87958
+  _PATCHANNOTATIONSREQUEST._serialized_end=1184
+  _PATCHANNOTATIONSSTATUSREQUEST._serialized_start=1187
+  _PATCHANNOTATIONSSTATUSREQUEST._serialized_end=1372
+  _PATCHANNOTATIONSSTATUSRESPONSE._serialized_start=1374
+  _PATCHANNOTATIONSSTATUSRESPONSE._serialized_end=1492
+  _DELETEANNOTATIONREQUEST._serialized_start=1494
+  _DELETEANNOTATIONREQUEST._serialized_end=1609
+  _DELETEANNOTATIONSREQUEST._serialized_start=1611
+  _DELETEANNOTATIONSREQUEST._serialized_end=1718
+  _SINGLEANNOTATIONRESPONSE._serialized_start=1720
+  _SINGLEANNOTATIONRESPONSE._serialized_end=1837
+  _MULTIANNOTATIONRESPONSE._serialized_start=1839
+  _MULTIANNOTATIONRESPONSE._serialized_end=1962
+  _GETAPPREQUEST._serialized_start=1964
+  _GETAPPREQUEST._serialized_end=2055
+  _LISTAPPSREQUEST._serialized_start=2058
+  _LISTAPPSREQUEST._serialized_end=2351
+  _POSTAPPSREQUEST._serialized_start=2353
+  _POSTAPPSREQUEST._serialized_end=2452
+  _DELETEAPPREQUEST._serialized_start=2454
+  _DELETEAPPREQUEST._serialized_end=2521
+  _PATCHAPPSREQUEST._serialized_start=2524
+  _PATCHAPPSREQUEST._serialized_end=2709
+  _PATCHAPPREQUEST._serialized_start=2712
+  _PATCHAPPREQUEST._serialized_end=2895
+  _PATCHAPPSIDSREQUEST._serialized_start=2898
+  _PATCHAPPSIDSREQUEST._serialized_end=3027
+  _POSTAPPSSEARCHESREQUEST._serialized_start=3030
+  _POSTAPPSSEARCHESREQUEST._serialized_end=3193
+  _SINGLEAPPRESPONSE._serialized_start=3195
+  _SINGLEAPPRESPONSE._serialized_end=3291
+  _MULTIAPPRESPONSE._serialized_start=3293
+  _MULTIAPPRESPONSE._serialized_end=3395
+  _LISTCOLLABORATORSREQUEST._serialized_start=3398
+  _LISTCOLLABORATORSREQUEST._serialized_end=3537
+  _POSTCOLLABORATORSREQUEST._serialized_start=3539
+  _POSTCOLLABORATORSREQUEST._serialized_end=3665
+  _PATCHCOLLABORATORSREQUEST._serialized_start=3668
+  _PATCHCOLLABORATORSREQUEST._serialized_end=3811
+  _DELETECOLLABORATORSREQUEST._serialized_start=3813
+  _DELETECOLLABORATORSREQUEST._serialized_end=3937
+  _MULTICOLLABORATORSRESPONSE._serialized_start=3940
+  _MULTICOLLABORATORSRESPONSE._serialized_end=4070
+  _LISTCOLLABORATIONSREQUEST._serialized_start=4072
+  _LISTCOLLABORATIONSREQUEST._serialized_end=4180
+  _MULTICOLLABORATIONSRESPONSE._serialized_start=4183
+  _MULTICOLLABORATIONSRESPONSE._serialized_end=4316
+  _GETSTATUSCODEREQUEST._serialized_start=4318
+  _GETSTATUSCODEREQUEST._serialized_end=4364
+  _LISTSTATUSCODESREQUEST._serialized_start=4366
+  _LISTSTATUSCODESREQUEST._serialized_end=4390
+  _SINGLESTATUSCODERESPONSE._serialized_start=4392
+  _SINGLESTATUSCODERESPONSE._serialized_end=4463
+  _MULTISTATUSCODERESPONSE._serialized_start=4465
+  _MULTISTATUSCODERESPONSE._serialized_end=4582
+  _GETCONCEPTREQUEST._serialized_start=4584
+  _GETCONCEPTREQUEST._serialized_end=4672
+  _LISTCONCEPTSREQUEST._serialized_start=4674
+  _LISTCONCEPTSREQUEST._serialized_end=4776
+  _LISTMODELCONCEPTSREQUEST._serialized_start=4779
+  _LISTMODELCONCEPTSREQUEST._serialized_end=4924
+  _POSTCONCEPTSSEARCHESREQUEST._serialized_start=4927
+  _POSTCONCEPTSSEARCHESREQUEST._serialized_end=5102
+  _POSTCONCEPTSREQUEST._serialized_start=5104
+  _POSTCONCEPTSREQUEST._serialized_end=5215
+  _PATCHCONCEPTSREQUEST._serialized_start=5218
+  _PATCHCONCEPTSREQUEST._serialized_end=5346
+  _GETCONCEPTCOUNTSREQUEST._serialized_start=5348
+  _GETCONCEPTCOUNTSREQUEST._serialized_end=5454
+  _SINGLECONCEPTRESPONSE._serialized_start=5456
+  _SINGLECONCEPTRESPONSE._serialized_end=5564
+  _MULTICONCEPTRESPONSE._serialized_start=5566
+  _MULTICONCEPTRESPONSE._serialized_end=5680
+  _MULTICONCEPTCOUNTRESPONSE._serialized_start=5683
+  _MULTICONCEPTCOUNTRESPONSE._serialized_end=5813
+  _LISTCONCEPTRELATIONSREQUEST._serialized_start=5816
+  _LISTCONCEPTRELATIONSREQUEST._serialized_end=5993
+  _POSTCONCEPTRELATIONSREQUEST._serialized_start=5996
+  _POSTCONCEPTRELATIONSREQUEST._serialized_end=6152
+  _DELETECONCEPTRELATIONSREQUEST._serialized_start=6154
+  _DELETECONCEPTRELATIONSREQUEST._serialized_end=6267
+  _LISTKNOWLEDGEGRAPHSREQUEST._serialized_start=6269
+  _LISTKNOWLEDGEGRAPHSREQUEST._serialized_end=6346
+  _POSTKNOWLEDGEGRAPHSREQUEST._serialized_start=6349
+  _POSTKNOWLEDGEGRAPHSREQUEST._serialized_end=6482
+  _POSTCONCEPTMAPPINGJOBSREQUEST._serialized_start=6485
+  _POSTCONCEPTMAPPINGJOBSREQUEST._serialized_end=6628
+  _MULTICONCEPTRELATIONRESPONSE._serialized_start=6631
+  _MULTICONCEPTRELATIONRESPONSE._serialized_end=6770
+  _MULTIKNOWLEDGEGRAPHRESPONSE._serialized_start=6773
+  _MULTIKNOWLEDGEGRAPHRESPONSE._serialized_end=6909
+  _MULTICONCEPTMAPPINGJOBRESPONSE._serialized_start=6911
+  _MULTICONCEPTMAPPINGJOBRESPONSE._serialized_end=7001
+  _GETCONCEPTLANGUAGEREQUEST._serialized_start=7003
+  _GETCONCEPTLANGUAGEREQUEST._serialized_end=7117
+  _LISTCONCEPTLANGUAGESREQUEST._serialized_start=7120
+  _LISTCONCEPTLANGUAGESREQUEST._serialized_end=7250
+  _PATCHCONCEPTLANGUAGESREQUEST._serialized_start=7253
+  _PATCHCONCEPTLANGUAGESREQUEST._serialized_end=7426
+  _POSTCONCEPTLANGUAGESREQUEST._serialized_start=7429
+  _POSTCONCEPTLANGUAGESREQUEST._serialized_end=7585
+  _SINGLECONCEPTLANGUAGERESPONSE._serialized_start=7588
+  _SINGLECONCEPTLANGUAGERESPONSE._serialized_end=7721
+  _MULTICONCEPTLANGUAGERESPONSE._serialized_start=7724
+  _MULTICONCEPTLANGUAGERESPONSE._serialized_end=7863
+  _GETINPUTREQUEST._serialized_start=7865
+  _GETINPUTREQUEST._serialized_end=7949
+  _GETVIDEOMANIFESTREQUEST._serialized_start=7951
+  _GETVIDEOMANIFESTREQUEST._serialized_end=8043
+  _GETINPUTSAMPLESREQUEST._serialized_start=8045
+  _GETINPUTSAMPLESREQUEST._serialized_end=8153
+  _LISTINPUTSREQUEST._serialized_start=8156
+  _LISTINPUTSREQUEST._serialized_end=8314
+  _STREAMINPUTSREQUEST._serialized_start=8317
+  _STREAMINPUTSREQUEST._serialized_end=8463
+  _POSTINPUTSREQUEST._serialized_start=8466
+  _POSTINPUTSREQUEST._serialized_end=8677
+  _PATCHINPUTSREQUEST._serialized_start=8679
+  _PATCHINPUTSREQUEST._serialized_end=8801
+  _DELETEINPUTREQUEST._serialized_start=8803
+  _DELETEINPUTREQUEST._serialized_end=8890
+  _DELETEINPUTSREQUEST._serialized_start=8892
+  _DELETEINPUTSREQUEST._serialized_end=8981
+  _SINGLEINPUTRESPONSE._serialized_start=8983
+  _SINGLEINPUTRESPONSE._serialized_end=9085
+  _GETVIDEOMANIFESTRESPONSE._serialized_start=9087
+  _GETVIDEOMANIFESTRESPONSE._serialized_end=9180
+  _MULTIINPUTRESPONSE._serialized_start=9183
+  _MULTIINPUTRESPONSE._serialized_end=9343
+  _MULTIINPUTANNOTATIONRESPONSE._serialized_start=9345
+  _MULTIINPUTANNOTATIONRESPONSE._serialized_end=9459
+  _SINGLEINPUTCOUNTRESPONSE._serialized_start=9461
+  _SINGLEINPUTCOUNTRESPONSE._serialized_end=9574
+  _GETINPUTCOUNTREQUEST._serialized_start=9576
+  _GETINPUTCOUNTREQUEST._serialized_end=9647
+  _LISTDATASETSREQUEST._serialized_start=9650
+  _LISTDATASETSREQUEST._serialized_end=9801
+  _GETDATASETREQUEST._serialized_start=9803
+  _GETDATASETREQUEST._serialized_end=9918
+  _POSTDATASETSREQUEST._serialized_start=9920
+  _POSTDATASETSREQUEST._serialized_end=10031
+  _PATCHDATASETSREQUEST._serialized_start=10034
+  _PATCHDATASETSREQUEST._serialized_end=10162
+  _DELETEDATASETSREQUEST._serialized_start=10164
+  _DELETEDATASETSREQUEST._serialized_end=10257
+  _MULTIDATASETRESPONSE._serialized_start=10259
+  _MULTIDATASETRESPONSE._serialized_end=10373
+  _SINGLEDATASETRESPONSE._serialized_start=10375
+  _SINGLEDATASETRESPONSE._serialized_end=10483
+  _LISTDATASETINPUTSREQUEST._serialized_start=10485
+  _LISTDATASETINPUTSREQUEST._serialized_end=10612
+  _GETDATASETINPUTREQUEST._serialized_start=10614
+  _GETDATASETINPUTREQUEST._serialized_end=10725
+  _POSTDATASETINPUTSREQUEST._serialized_start=10728
+  _POSTDATASETINPUTSREQUEST._serialized_end=10913
+  _DELETEDATASETINPUTSREQUEST._serialized_start=10915
+  _DELETEDATASETINPUTSREQUEST._serialized_end=11031
+  _MULTIDATASETINPUTRESPONSE._serialized_start=11034
+  _MULTIDATASETINPUTRESPONSE._serialized_end=11244
+  _SINGLEDATASETINPUTRESPONSE._serialized_start=11246
+  _SINGLEDATASETINPUTRESPONSE._serialized_end=11370
+  _LISTDATASETVERSIONSREQUEST._serialized_start=11373
+  _LISTDATASETVERSIONSREQUEST._serialized_end=11502
+  _GETDATASETVERSIONREQUEST._serialized_start=11504
+  _GETDATASETVERSIONREQUEST._serialized_end=11627
+  _LISTDATASETVERSIONMETRICSGROUPSREQUEST._serialized_start=11630
+  _LISTDATASETVERSIONMETRICSGROUPSREQUEST._serialized_end=11922
+  _POSTDATASETVERSIONSREQUEST._serialized_start=11925
+  _POSTDATASETVERSIONSREQUEST._serialized_end=12078
+  _PATCHDATASETVERSIONSREQUEST._serialized_start=12081
+  _PATCHDATASETVERSIONSREQUEST._serialized_end=12251
+  _DELETEDATASETVERSIONSREQUEST._serialized_start=12254
+  _DELETEDATASETVERSIONSREQUEST._serialized_end=12382
+  _PUTDATASETVERSIONEXPORTSREQUEST._serialized_start=12385
+  _PUTDATASETVERSIONEXPORTSREQUEST._serialized_end=12568
+  _MULTIDATASETVERSIONRESPONSE._serialized_start=12571
+  _MULTIDATASETVERSIONRESPONSE._serialized_end=12707
+  _MULTIDATASETVERSIONEXPORTRESPONSE._serialized_start=12710
+  _MULTIDATASETVERSIONEXPORTRESPONSE._serialized_end=12849
+  _MULTIDATASETVERSIONMETRICSGROUPRESPONSE._serialized_start=12852
+  _MULTIDATASETVERSIONMETRICSGROUPRESPONSE._serialized_end=13026
+  _SINGLEDATASETVERSIONRESPONSE._serialized_start=13029
+  _SINGLEDATASETVERSIONRESPONSE._serialized_end=13159
+  _GETDATASETINPUTSSEARCHADDJOBREQUEST._serialized_start=13161
+  _GETDATASETINPUTSSEARCHADDJOBREQUEST._serialized_end=13263
+  _SINGLEDATASETINPUTSSEARCHADDJOBRESPONSE._serialized_start=13266
+  _SINGLEDATASETINPUTSSEARCHADDJOBRESPONSE._serialized_end=13406
+  _POSTMODELOUTPUTSREQUEST._serialized_start=13409
+  _POSTMODELOUTPUTSREQUEST._serialized_end=13594
+  _LISTMODELINPUTSREQUEST._serialized_start=13597
+  _LISTMODELINPUTSREQUEST._serialized_end=13740
+  _GETKEYREQUEST._serialized_start=13742
+  _GETKEYREQUEST._serialized_end=13822
+  _LISTKEYSREQUEST._serialized_start=13825
+  _LISTKEYSREQUEST._serialized_end=13979
+  _LISTAPPKEYSREQUEST._serialized_start=13981
+  _LISTAPPKEYSREQUEST._serialized_end=14082
+  _POSTKEYSREQUEST._serialized_start=14084
+  _POSTKEYSREQUEST._serialized_end=14183
+  _DELETEKEYREQUEST._serialized_start=14185
+  _DELETEKEYREQUEST._serialized_end=14268
+  _PATCHKEYSREQUEST._serialized_start=14270
+  _PATCHKEYSREQUEST._serialized_end=14386
+  _SINGLEKEYRESPONSE._serialized_start=14388
+  _SINGLEKEYRESPONSE._serialized_end=14484
+  _MULTIKEYRESPONSE._serialized_start=14486
+  _MULTIKEYRESPONSE._serialized_end=14588
+  _GETMODELREQUEST._serialized_start=14591
+  _GETMODELREQUEST._serialized_end=14764
+  _LISTMODELSREQUEST._serialized_start=14767
+  _LISTMODELSREQUEST._serialized_end=15314
+  _GETRESOURCECOUNTSREQUEST._serialized_start=15316
+  _GETRESOURCECOUNTSREQUEST._serialized_end=15391
+  _GETRESOURCECOUNTSRESPONSE._serialized_start=15394
+  _GETRESOURCECOUNTSRESPONSE._serialized_end=15536
+  _PATCHMODELTOOLKITSREQUEST._serialized_start=15539
+  _PATCHMODELTOOLKITSREQUEST._serialized_end=15667
+  _PATCHMODELCHECKCONSENTSREQUEST._serialized_start=15670
+  _PATCHMODELCHECKCONSENTSREQUEST._serialized_end=15809
+  _PATCHMODELUSECASESREQUEST._serialized_start=15812
+  _PATCHMODELUSECASESREQUEST._serialized_end=15940
+  _PATCHMODELLANGUAGESREQUEST._serialized_start=15943
+  _PATCHMODELLANGUAGESREQUEST._serialized_end=16073
+  _MULTIMODELTOOLKITRESPONSE._serialized_start=16075
+  _MULTIMODELTOOLKITRESPONSE._serialized_end=16165
+  _MULTIMODELCHECKCONSENTRESPONSE._serialized_start=16167
+  _MULTIMODELCHECKCONSENTRESPONSE._serialized_end=16268
+  _MULTIMODELUSECASERESPONSE._serialized_start=16270
+  _MULTIMODELUSECASERESPONSE._serialized_end=16360
+  _MULTIMODELLANGUAGERESPONSE._serialized_start=16362
+  _MULTIMODELLANGUAGERESPONSE._serialized_end=16454
+  _POSTMODELSREQUEST._serialized_start=16457
+  _POSTMODELSREQUEST._serialized_end=16602
+  _PATCHMODELSREQUEST._serialized_start=16604
+  _PATCHMODELSREQUEST._serialized_end=16726
+  _IDUPDATESOURCE._serialized_start=16728
+  _IDUPDATESOURCE._serialized_end=16772
+  _PATCHMODELIDSREQUEST._serialized_start=16775
+  _PATCHMODELIDSREQUEST._serialized_end=16905
+  _DELETEMODELREQUEST._serialized_start=16907
+  _DELETEMODELREQUEST._serialized_end=16994
+  _DELETEMODELSREQUEST._serialized_start=16996
+  _DELETEMODELSREQUEST._serialized_end=17099
+  _POSTMODELSSEARCHESREQUEST._serialized_start=17102
+  _POSTMODELSSEARCHESREQUEST._serialized_end=17271
+  _SINGLEMODELRESPONSE._serialized_start=17273
+  _SINGLEMODELRESPONSE._serialized_end=17375
+  _MULTIMODELRESPONSE._serialized_start=17377
+  _MULTIMODELRESPONSE._serialized_end=17485
+  _PATCHMODELVERSIONSREQUEST._serialized_start=17488
+  _PATCHMODELVERSIONSREQUEST._serialized_end=17650
+  _GETMODELVERSIONREQUEST._serialized_start=17652
+  _GETMODELVERSIONREQUEST._serialized_end=17763
+  _LISTMODELVERSIONSREQUEST._serialized_start=17766
+  _LISTMODELVERSIONSREQUEST._serialized_end=18091
+  _DELETEMODELVERSIONREQUEST._serialized_start=18093
+  _DELETEMODELVERSIONREQUEST._serialized_end=18207
+  _SINGLEMODELVERSIONRESPONSE._serialized_start=18209
+  _SINGLEMODELVERSIONRESPONSE._serialized_end=18333
+  _MULTIMODELVERSIONRESPONSE._serialized_start=18336
+  _MULTIMODELVERSIONRESPONSE._serialized_end=18466
+  _POSTMODELVERSIONSREQUEST._serialized_start=18469
+  _POSTMODELVERSIONSREQUEST._serialized_end=18708
+  _POSTWORKFLOWVERSIONSUNPUBLISHREQUEST._serialized_start=18711
+  _POSTWORKFLOWVERSIONSUNPUBLISHREQUEST._serialized_end=18888
+  _POSTWORKFLOWVERSIONSPUBLISHREQUEST._serialized_start=18891
+  _POSTWORKFLOWVERSIONSPUBLISHREQUEST._serialized_end=19064
+  _WORKFLOWVERSIONPUBLISHREQUEST._serialized_start=19066
+  _WORKFLOWVERSIONPUBLISHREQUEST._serialized_end=19117
+  _WORKFLOWVERSIONUNPUBLISHREQUEST._serialized_start=19119
+  _WORKFLOWVERSIONUNPUBLISHREQUEST._serialized_end=19172
+  _MODELVERSIONPUBLISHREQUEST._serialized_start=19174
+  _MODELVERSIONPUBLISHREQUEST._serialized_end=19222
+  _POSTMODELVERSIONSPUBLISHREQUEST._serialized_start=19225
+  _POSTMODELVERSIONSPUBLISHREQUEST._serialized_end=19389
+  _MODELVERSIONUNPUBLISHREQUEST._serialized_start=19391
+  _MODELVERSIONUNPUBLISHREQUEST._serialized_end=19441
+  _POSTMODELVERSIONSUNPUBLISHREQUEST._serialized_start=19444
+  _POSTMODELVERSIONSUNPUBLISHREQUEST._serialized_end=19612
+  _POSTEVALUATIONSREQUEST._serialized_start=19614
+  _POSTEVALUATIONSREQUEST._serialized_end=19736
+  _LISTEVALUATIONSREQUEST._serialized_start=19738
+  _LISTEVALUATIONSREQUEST._serialized_end=19843
+  _GETEVALUATIONREQUEST._serialized_start=19846
+  _GETEVALUATIONREQUEST._serialized_end=19983
+  _POSTMODELVERSIONEVALUATIONSREQUEST._serialized_start=19986
+  _POSTMODELVERSIONEVALUATIONSREQUEST._serialized_end=20164
+  _LISTMODELVERSIONEVALUATIONSREQUEST._serialized_start=20167
+  _LISTMODELVERSIONEVALUATIONSREQUEST._serialized_end=20328
+  _GETMODELVERSIONEVALUATIONREQUEST._serialized_start=20331
+  _GETMODELVERSIONEVALUATIONREQUEST._serialized_end=20524
+  _SINGLEEVALMETRICSRESPONSE._serialized_start=20526
+  _SINGLEEVALMETRICSRESPONSE._serialized_end=20647
+  _MULTIEVALMETRICSRESPONSE._serialized_start=20649
+  _MULTIEVALMETRICSRESPONSE._serialized_end=20769
+  _POSTMODELVERSIONMETRICSREQUEST._serialized_start=20772
+  _POSTMODELVERSIONMETRICSREQUEST._serialized_end=20983
+  _GETMODELVERSIONMETRICSREQUEST._serialized_start=20986
+  _GETMODELVERSIONMETRICSREQUEST._serialized_end=21147
+  _GETMODELTYPEREQUEST._serialized_start=21149
+  _GETMODELTYPEREQUEST._serialized_end=21242
+  _LISTMODELTYPESREQUEST._serialized_start=21244
+  _LISTMODELTYPESREQUEST._serialized_end=21348
+  _LISTOPENSOURCELICENSESREQUEST._serialized_start=21350
+  _LISTOPENSOURCELICENSESREQUEST._serialized_end=21381
+  _LISTOPENSOURCELICENSESRESPONSE._serialized_start=21383
+  _LISTOPENSOURCELICENSESRESPONSE._serialized_end=21478
+  _SINGLEMODELTYPERESPONSE._serialized_start=21480
+  _SINGLEMODELTYPERESPONSE._serialized_end=21601
+  _MULTIMODELTYPERESPONSE._serialized_start=21604
+  _MULTIMODELTYPERESPONSE._serialized_end=21846
+  _GETMODELVERSIONINPUTEXAMPLEREQUEST._serialized_start=21849
+  _GETMODELVERSIONINPUTEXAMPLEREQUEST._serialized_end=21998
+  _LISTMODELVERSIONINPUTEXAMPLESREQUEST._serialized_start=22001
+  _LISTMODELVERSIONINPUTEXAMPLESREQUEST._serialized_end=22164
+  _SINGLEMODELVERSIONINPUTEXAMPLERESPONSE._serialized_start=22167
+  _SINGLEMODELVERSIONINPUTEXAMPLERESPONSE._serialized_end=22329
+  _MULTIMODELVERSIONINPUTEXAMPLERESPONSE._serialized_start=22332
+  _MULTIMODELVERSIONINPUTEXAMPLERESPONSE._serialized_end=22494
+  _LISTMODELREFERENCESREQUEST._serialized_start=22496
+  _LISTMODELREFERENCESREQUEST._serialized_end=22623
+  _MULTIMODELREFERENCERESPONSE._serialized_start=22626
+  _MULTIMODELREFERENCERESPONSE._serialized_end=22756
+  _MULTIOUTPUTRESPONSE._serialized_start=22758
+  _MULTIOUTPUTRESPONSE._serialized_end=22869
+  _LISTSCOPESREQUEST._serialized_start=22871
+  _LISTSCOPESREQUEST._serialized_end=22957
+  _MYSCOPESREQUEST._serialized_start=22959
+  _MYSCOPESREQUEST._serialized_end=23025
+  _MYSCOPESUSERREQUEST._serialized_start=23027
+  _MYSCOPESUSERREQUEST._serialized_end=23097
+  _MYSCOPESROOTREQUEST._serialized_start=23099
+  _MYSCOPESROOTREQUEST._serialized_end=23120
+  _MULTISCOPEDEPSRESPONSE._serialized_start=23123
+  _MULTISCOPEDEPSRESPONSE._serialized_end=23288
+  _MULTISCOPERESPONSE._serialized_start=23291
+  _MULTISCOPERESPONSE._serialized_end=23451
+  _MULTISCOPEUSERRESPONSE._serialized_start=23454
+  _MULTISCOPEUSERRESPONSE._serialized_end=23586
+  _MULTISCOPEROOTRESPONSE._serialized_start=23589
+  _MULTISCOPEROOTRESPONSE._serialized_end=23721
+  _GETSEARCHREQUEST._serialized_start=23723
+  _GETSEARCHREQUEST._serialized_end=23802
+  _LISTSEARCHESREQUEST._serialized_start=23804
+  _LISTSEARCHESREQUEST._serialized_end=23906
+  _POSTSEARCHESREQUEST._serialized_start=23909
+  _POSTSEARCHESREQUEST._serialized_end=24105
+  _PATCHINPUTSSEARCHESREQUEST._serialized_start=24108
+  _PATCHINPUTSSEARCHESREQUEST._serialized_end=24241
+  _PATCHANNOTATIONSSEARCHESREQUEST._serialized_start=24244
+  _PATCHANNOTATIONSSEARCHESREQUEST._serialized_end=24382
+  _PATCHSEARCHESREQUEST._serialized_start=24384
+  _PATCHSEARCHESREQUEST._serialized_end=24511
+  _POSTSEARCHESBYIDREQUEST._serialized_start=24514
+  _POSTSEARCHESBYIDREQUEST._serialized_end=24646
+  _DELETESEARCHREQUEST._serialized_start=24648
+  _DELETESEARCHREQUEST._serialized_end=24730
+  _POSTANNOTATIONSSEARCHESREQUEST._serialized_start=24733
+  _POSTANNOTATIONSSEARCHESREQUEST._serialized_end=24900
+  _DELETEANNOTATIONSEARCHMETRICSREQUEST._serialized_start=24902
+  _DELETEANNOTATIONSEARCHMETRICSREQUEST._serialized_end=25001
+  _POSTINPUTSSEARCHESREQUEST._serialized_start=25004
+  _POSTINPUTSSEARCHESREQUEST._serialized_end=25186
+  _SINGLESEARCHRESPONSE._serialized_start=25188
+  _SINGLESEARCHRESPONSE._serialized_end=25293
+  _MULTISEARCHRESPONSE._serialized_start=25296
+  _MULTISEARCHRESPONSE._serialized_end=25533
+  _POSTANNOTATIONSEARCHMETRICSREQUEST._serialized_start=25536
+  _POSTANNOTATIONSEARCHMETRICSREQUEST._serialized_end=25812
+  _GETANNOTATIONSEARCHMETRICSREQUEST._serialized_start=25814
+  _GETANNOTATIONSEARCHMETRICSREQUEST._serialized_end=25910
+  _LISTANNOTATIONSEARCHMETRICSREQUEST._serialized_start=25912
+  _LISTANNOTATIONSEARCHMETRICSREQUEST._serialized_end=25997
+  _MULTIANNOTATIONSEARCHMETRICSRESPONSE._serialized_start=26000
+  _MULTIANNOTATIONSEARCHMETRICSRESPONSE._serialized_end=26157
+  _LISTANNOTATIONFILTERSREQUEST._serialized_start=26159
+  _LISTANNOTATIONFILTERSREQUEST._serialized_end=26270
+  _GETANNOTATIONFILTERREQUEST._serialized_start=26272
+  _GETANNOTATIONFILTERREQUEST._serialized_end=26379
+  _POSTANNOTATIONFILTERSREQUEST._serialized_start=26382
+  _POSTANNOTATIONFILTERSREQUEST._serialized_end=26521
+  _PATCHANNOTATIONFILTERSREQUEST._serialized_start=26524
+  _PATCHANNOTATIONFILTERSREQUEST._serialized_end=26680
+  _DELETEANNOTATIONFILTERSREQUEST._serialized_start=26682
+  _DELETEANNOTATIONFILTERSREQUEST._serialized_end=26794
+  _MULTIANNOTATIONFILTERRESPONSE._serialized_start=26797
+  _MULTIANNOTATIONFILTERRESPONSE._serialized_end=26939
+  _SINGLEANNOTATIONFILTERRESPONSE._serialized_start=26942
+  _SINGLEANNOTATIONFILTERRESPONSE._serialized_end=27078
+  _GETUSERREQUEST._serialized_start=27080
+  _GETUSERREQUEST._serialized_end=27172
+  _SINGLEUSERRESPONSE._serialized_start=27174
+  _SINGLEUSERRESPONSE._serialized_end=27273
+  _POSTVALIDATEPASSWORDREQUEST._serialized_start=27275
+  _POSTVALIDATEPASSWORDREQUEST._serialized_end=27395
+  _SINGLEPASSWORDVALIDATIONRESPONSE._serialized_start=27398
+  _SINGLEPASSWORDVALIDATIONRESPONSE._serialized_end=27540
+  _GETWORKFLOWREQUEST._serialized_start=27543
+  _GETWORKFLOWREQUEST._serialized_end=27730
+  _LISTWORKFLOWSREQUEST._serialized_start=27733
+  _LISTWORKFLOWSREQUEST._serialized_end=28048
+  _POSTWORKFLOWSREQUEST._serialized_start=28050
+  _POSTWORKFLOWSREQUEST._serialized_end=28164
+  _PATCHWORKFLOWSREQUEST._serialized_start=28167
+  _PATCHWORKFLOWSREQUEST._serialized_end=28298
+  _PATCHWORKFLOWIDSREQUEST._serialized_start=28301
+  _PATCHWORKFLOWIDSREQUEST._serialized_end=28434
+  _DELETEWORKFLOWREQUEST._serialized_start=28436
+  _DELETEWORKFLOWREQUEST._serialized_end=28529
+  _DELETEWORKFLOWSREQUEST._serialized_start=28531
+  _DELETEWORKFLOWSREQUEST._serialized_end=28637
+  _SINGLEWORKFLOWRESPONSE._serialized_start=28639
+  _SINGLEWORKFLOWRESPONSE._serialized_end=28750
+  _MULTIWORKFLOWRESPONSE._serialized_start=28752
+  _MULTIWORKFLOWRESPONSE._serialized_end=28869
+  _POSTWORKFLOWRESULTSREQUEST._serialized_start=28872
+  _POSTWORKFLOWRESULTSREQUEST._serialized_end=29165
+  _POSTWORKFLOWRESULTSRESPONSE._serialized_start=29168
+  _POSTWORKFLOWRESULTSRESPONSE._serialized_end=29384
+  _POSTWORKFLOWRESULTSSIMILARITYREQUEST._serialized_start=29387
+  _POSTWORKFLOWRESULTSSIMILARITYREQUEST._serialized_end=29660
+  _POSTWORKFLOWRESULTSSIMILARITYRESPONSE._serialized_start=29663
+  _POSTWORKFLOWRESULTSSIMILARITYRESPONSE._serialized_end=29805
+  _LISTWORKFLOWVERSIONSREQUEST._serialized_start=29808
+  _LISTWORKFLOWVERSIONSREQUEST._serialized_end=29939
+  _GETWORKFLOWVERSIONREQUEST._serialized_start=29941
+  _GETWORKFLOWVERSIONREQUEST._serialized_end=30067
+  _DELETEWORKFLOWVERSIONSREQUEST._serialized_start=30070
+  _DELETEWORKFLOWVERSIONSREQUEST._serialized_end=30201
+  _PATCHWORKFLOWVERSIONSREQUEST._serialized_start=30204
+  _PATCHWORKFLOWVERSIONSREQUEST._serialized_end=30378
+  _MULTIWORKFLOWVERSIONRESPONSE._serialized_start=30381
+  _MULTIWORKFLOWVERSIONRESPONSE._serialized_end=30520
+  _SINGLEWORKFLOWVERSIONRESPONSE._serialized_start=30523
+  _SINGLEWORKFLOWVERSIONRESPONSE._serialized_end=30656
+  _POSTAPPDUPLICATIONSREQUEST._serialized_start=30659
+  _POSTAPPDUPLICATIONSREQUEST._serialized_end=30792
+  _GETAPPDUPLICATIONREQUEST._serialized_start=30794
+  _GETAPPDUPLICATIONREQUEST._serialized_end=30897
+  _LISTAPPDUPLICATIONSREQUEST._serialized_start=30899
+  _LISTAPPDUPLICATIONSREQUEST._serialized_end=31008
+  _MULTIAPPDUPLICATIONSRESPONSE._serialized_start=31011
+  _MULTIAPPDUPLICATIONSRESPONSE._serialized_end=31142
+  _SINGLEAPPDUPLICATIONRESPONSE._serialized_start=31145
+  _SINGLEAPPDUPLICATIONRESPONSE._serialized_end=31275
+  _POSTTASKSREQUEST._serialized_start=31277
+  _POSTTASKSREQUEST._serialized_end=31379
+  _GETTASKREQUEST._serialized_start=31381
+  _GETTASKREQUEST._serialized_end=31490
+  _LISTTASKSREQUEST._serialized_start=31493
+  _LISTTASKSREQUEST._serialized_end=31731
+  _PATCHTASKSREQUEST._serialized_start=31733
+  _PATCHTASKSREQUEST._serialized_end=31852
+  _DELETETASKSREQUEST._serialized_start=31854
+  _DELETETASKSREQUEST._serialized_end=31936
+  _MULTITASKRESPONSE._serialized_start=31938
+  _MULTITASKRESPONSE._serialized_end=32043
+  _SINGLETASKRESPONSE._serialized_start=32045
+  _SINGLETASKRESPONSE._serialized_end=32144
+  _GETTASKCOUNTREQUEST._serialized_start=32146
+  _GETTASKCOUNTREQUEST._serialized_end=32251
+  _SINGLETASKCOUNTRESPONSE._serialized_start=32254
+  _SINGLETASKCOUNTRESPONSE._serialized_end=32411
+  _POSTLABELORDERSREQUEST._serialized_start=32413
+  _POSTLABELORDERSREQUEST._serialized_end=32534
+  _GETLABELORDERREQUEST._serialized_start=32536
+  _GETLABELORDERREQUEST._serialized_end=32631
+  _LISTLABELORDERSREQUEST._serialized_start=32633
+  _LISTLABELORDERSREQUEST._serialized_end=32738
+  _PATCHLABELORDERSREQUEST._serialized_start=32741
+  _PATCHLABELORDERSREQUEST._serialized_end=32879
+  _DELETELABELORDERSREQUEST._serialized_start=32881
+  _DELETELABELORDERSREQUEST._serialized_end=32969
+  _MULTILABELORDERRESPONSE._serialized_start=32971
+  _MULTILABELORDERRESPONSE._serialized_end=33095
+  _SINGLELABELORDERRESPONSE._serialized_start=33097
+  _SINGLELABELORDERRESPONSE._serialized_end=33215
+  _POSTCOLLECTORSREQUEST._serialized_start=33217
+  _POSTCOLLECTORSREQUEST._serialized_end=33334
+  _PATCHCOLLECTORSREQUEST._serialized_start=33337
+  _PATCHCOLLECTORSREQUEST._serialized_end=33471
+  _DELETECOLLECTORSREQUEST._serialized_start=33473
+  _DELETECOLLECTORSREQUEST._serialized_end=33580
+  _GETCOLLECTORREQUEST._serialized_start=33582
+  _GETCOLLECTORREQUEST._serialized_end=33674
+  _LISTCOLLECTORSREQUEST._serialized_start=33676
+  _LISTCOLLECTORSREQUEST._serialized_end=33780
+  _MULTICOLLECTORRESPONSE._serialized_start=33782
+  _MULTICOLLECTORRESPONSE._serialized_end=33896
+  _SINGLECOLLECTORRESPONSE._serialized_start=33898
+  _SINGLECOLLECTORRESPONSE._serialized_end=34012
+  _POSTSTATVALUESREQUEST._serialized_start=34014
+  _POSTSTATVALUESREQUEST._serialized_end=34132
+  _MULTISTATVALUERESPONSE._serialized_start=34134
+  _MULTISTATVALUERESPONSE._serialized_end=34255
+  _POSTSTATVALUESAGGREGATEREQUEST._serialized_start=34258
+  _POSTSTATVALUESAGGREGATEREQUEST._serialized_end=34416
+  _MULTISTATVALUEAGGREGATERESPONSE._serialized_start=34419
+  _MULTISTATVALUEAGGREGATERESPONSE._serialized_end=34575
+  _POSTTRENDINGMETRICSVIEWREQUEST._serialized_start=34577
+  _POSTTRENDINGMETRICSVIEWREQUEST._serialized_end=34696
+  _LISTTRENDINGMETRICSVIEWSREQUEST._serialized_start=34699
+  _LISTTRENDINGMETRICSVIEWSREQUEST._serialized_end=34832
+  _MULTITRENDINGMETRICSVIEWRESPONSE._serialized_start=34834
+  _MULTITRENDINGMETRICSVIEWRESPONSE._serialized_end=34960
+  _GETMODULEREQUEST._serialized_start=34962
+  _GETMODULEREQUEST._serialized_end=35075
+  _LISTMODULESREQUEST._serialized_start=35078
+  _LISTMODULESREQUEST._serialized_end=35228
+  _POSTMODULESREQUEST._serialized_start=35230
+  _POSTMODULESREQUEST._serialized_end=35338
+  _PATCHMODULESREQUEST._serialized_start=35340
+  _PATCHMODULESREQUEST._serialized_end=35465
+  _DELETEMODULESREQUEST._serialized_start=35467
+  _DELETEMODULESREQUEST._serialized_end=35551
+  _SINGLEMODULERESPONSE._serialized_start=35553
+  _SINGLEMODULERESPONSE._serialized_end=35658
+  _MULTIMODULERESPONSE._serialized_start=35660
+  _MULTIMODULERESPONSE._serialized_end=35771
+  _GETMODULEVERSIONREQUEST._serialized_start=35773
+  _GETMODULEVERSIONREQUEST._serialized_end=35893
+  _LISTMODULEVERSIONSREQUEST._serialized_start=35895
+  _LISTMODULEVERSIONSREQUEST._serialized_end=36022
+  _POSTMODULEVERSIONSREQUEST._serialized_start=36025
+  _POSTMODULEVERSIONSREQUEST._serialized_end=36174
+  _DELETEMODULEVERSIONSREQUEST._serialized_start=36176
+  _DELETEMODULEVERSIONSREQUEST._serialized_end=36286
+  _SINGLEMODULEVERSIONRESPONSE._serialized_start=36288
+  _SINGLEMODULEVERSIONRESPONSE._serialized_end=36415
+  _MULTIMODULEVERSIONRESPONSE._serialized_start=36418
+  _MULTIMODULEVERSIONRESPONSE._serialized_end=36551
+  _GETINSTALLEDMODULEVERSIONREQUEST._serialized_start=36553
+  _GETINSTALLEDMODULEVERSIONREQUEST._serialized_end=36673
+  _LISTINSTALLEDMODULEVERSIONSREQUEST._serialized_start=36675
+  _LISTINSTALLEDMODULEVERSIONSREQUEST._serialized_end=36792
+  _POSTINSTALLEDMODULEVERSIONSREQUEST._serialized_start=36795
+  _POSTINSTALLEDMODULEVERSIONSREQUEST._serialized_end=36953
+  _POSTINSTALLEDMODULEVERSIONSKEYREQUEST._serialized_start=36955
+  _POSTINSTALLEDMODULEVERSIONSKEYREQUEST._serialized_end=37080
+  _DELETEINSTALLEDMODULEVERSIONSREQUEST._serialized_start=37082
+  _DELETEINSTALLEDMODULEVERSIONSREQUEST._serialized_end=37182
+  _SINGLEINSTALLEDMODULEVERSIONRESPONSE._serialized_start=37185
+  _SINGLEINSTALLEDMODULEVERSIONRESPONSE._serialized_end=37340
+  _MULTIINSTALLEDMODULEVERSIONRESPONSE._serialized_start=37343
+  _MULTIINSTALLEDMODULEVERSIONRESPONSE._serialized_end=37504
+  _LISTNEXTTASKASSIGNMENTSREQUEST._serialized_start=37506
+  _LISTNEXTTASKASSIGNMENTSREQUEST._serialized_end=37604
+  _POSTBULKOPERATIONSREQUEST._serialized_start=37607
+  _POSTBULKOPERATIONSREQUEST._serialized_end=37737
+  _LISTBULKOPERATIONSREQUEST._serialized_start=37739
+  _LISTBULKOPERATIONSREQUEST._serialized_end=37847
+  _GETBULKOPERATIONREQUEST._serialized_start=37849
+  _GETBULKOPERATIONREQUEST._serialized_end=37935
+  _CANCELBULKOPERATIONREQUEST._serialized_start=37937
+  _CANCELBULKOPERATIONREQUEST._serialized_end=38027
+  _DELETEBULKOPERATIONREQUEST._serialized_start=38029
+  _DELETEBULKOPERATIONREQUEST._serialized_end=38119
+  _SINGLEBULKOPERATIONSRESPONSE._serialized_start=38122
+  _SINGLEBULKOPERATIONSRESPONSE._serialized_end=38250
+  _MULTIBULKOPERATIONSRESPONSE._serialized_start=38252
+  _MULTIBULKOPERATIONSRESPONSE._serialized_end=38379
+  _PUTTASKASSIGNMENTSREQUEST._serialized_start=38381
+  _PUTTASKASSIGNMENTSREQUEST._serialized_end=38492
+  _LISTINPUTSADDJOBSREQUEST._serialized_start=38494
+  _LISTINPUTSADDJOBSREQUEST._serialized_end=38601
+  _GETINPUTSADDJOBREQUEST._serialized_start=38603
+  _GETINPUTSADDJOBREQUEST._serialized_end=38688
+  _CANCELINPUTSADDJOBREQUEST._serialized_start=38690
+  _CANCELINPUTSADDJOBREQUEST._serialized_end=38778
+  _MULTIINPUTSADDJOBRESPONSE._serialized_start=38781
+  _MULTIINPUTSADDJOBRESPONSE._serialized_end=38912
+  _SINGLEINPUTSADDJOBRESPONSE._serialized_start=38914
+  _SINGLEINPUTSADDJOBRESPONSE._serialized_end=39039
+  _POSTUPLOADSREQUEST._serialized_start=39041
+  _POSTUPLOADSREQUEST._serialized_end=39149
+  _DELETEUPLOADSREQUEST._serialized_start=39151
+  _DELETEUPLOADSREQUEST._serialized_end=39235
+  _LISTUPLOADSREQUEST._serialized_start=39237
+  _LISTUPLOADSREQUEST._serialized_end=39338
+  _GETUPLOADREQUEST._serialized_start=39340
+  _GETUPLOADREQUEST._serialized_end=39426
+  _SINGLEUPLOADRESPONSE._serialized_start=39428
+  _SINGLEUPLOADRESPONSE._serialized_end=39533
+  _MULTIUPLOADRESPONSE._serialized_start=39535
+  _MULTIUPLOADRESPONSE._serialized_end=39640
+  _PUTUPLOADCONTENTPARTSREQUEST._serialized_start=39643
+  _PUTUPLOADCONTENTPARTSREQUEST._serialized_end=39797
+  _POSTINPUTSDATASOURCESREQUEST._serialized_start=39800
+  _POSTINPUTSDATASOURCESREQUEST._serialized_end=39973
+  _GETINPUTSEXTRACTIONJOBREQUEST._serialized_start=39975
+  _GETINPUTSEXTRACTIONJOBREQUEST._serialized_end=40089
+  _LISTINPUTSEXTRACTIONJOBSREQUEST._serialized_start=40091
+  _LISTINPUTSEXTRACTIONJOBSREQUEST._serialized_end=40205
+  _SINGLEINPUTSEXTRACTIONJOBRESPONSE._serialized_start=40208
+  _SINGLEINPUTSEXTRACTIONJOBRESPONSE._serialized_end=40354
+  _MULTIINPUTSEXTRACTIONJOBRESPONSE._serialized_start=40357
+  _MULTIINPUTSEXTRACTIONJOBRESPONSE._serialized_end=40503
+  _CANCELINPUTSEXTRACTIONJOBSREQUEST._serialized_start=40505
+  _CANCELINPUTSEXTRACTIONJOBSREQUEST._serialized_end=40602
+  _POSTINPUTSUPLOADSREQUEST._serialized_start=40604
+  _POSTINPUTSUPLOADSREQUEST._serialized_end=40731
+  _V2._serialized_start=40849
+  _V2._serialized_end=90395
 # @@protoc_insertion_point(module_scope)
```

### Comparing `clarifai-grpc-9.5.0/clarifai_grpc/grpc/api/service_pb2.pyi` & `clarifai-grpc-9.6.0/clarifai_grpc/grpc/api/service_pb2.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -209,31 +209,38 @@
     """PatchAnnotationsRequest"""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     USER_APP_ID_FIELD_NUMBER: builtins.int
     ANNOTATIONS_FIELD_NUMBER: builtins.int
     ACTION_FIELD_NUMBER: builtins.int
+    DELETE_IF_EMPTY_DATA_FIELD_NUMBER: builtins.int
     @property
     def user_app_id(self) -> proto.clarifai.api.resources_pb2.UserAppIDSet: ...
     @property
     def annotations(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[proto.clarifai.api.resources_pb2.Annotation]: ...
     action: builtins.str
     """The action to perform on the patched objects
     For now actions 'merge', 'overwrite', and 'remove' are supported
     """
+    delete_if_empty_data: builtins.bool
+    """If the request is a "remove" action and the annotation is left with empty data,
+    then setting delete_if_empty_data to true will delete the annotation,
+    if possible (for example, will not delete an input-level annotation).
+    """
     def __init__(
         self,
         *,
         user_app_id: proto.clarifai.api.resources_pb2.UserAppIDSet | None = ...,
         annotations: collections.abc.Iterable[proto.clarifai.api.resources_pb2.Annotation] | None = ...,
         action: builtins.str = ...,
+        delete_if_empty_data: builtins.bool = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["user_app_id", b"user_app_id"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["action", b"action", "annotations", b"annotations", "user_app_id", b"user_app_id"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["action", b"action", "annotations", b"annotations", "delete_if_empty_data", b"delete_if_empty_data", "user_app_id", b"user_app_id"]) -> None: ...
 
 global___PatchAnnotationsRequest = PatchAnnotationsRequest
 
 @typing_extensions.final
 class PatchAnnotationsStatusRequest(google.protobuf.message.Message):
     """PatchAnnotationsStatusRequest"""
 
@@ -1862,14 +1869,15 @@
     """PostInputsRequest"""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     USER_APP_ID_FIELD_NUMBER: builtins.int
     INPUTS_FIELD_NUMBER: builtins.int
     INPUTS_ADD_JOB_ID_FIELD_NUMBER: builtins.int
+    INPUT_ID_CONFLICT_RESOLUTION_FIELD_NUMBER: builtins.int
     @property
     def user_app_id(self) -> proto.clarifai.api.resources_pb2.UserAppIDSet: ...
     @property
     def inputs(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[proto.clarifai.api.resources_pb2.Input]:
         """List of inputs to post.
         For each input, the following fields are used:
         * id
@@ -1878,23 +1886,26 @@
         """
     inputs_add_job_id: builtins.str
     """Collect statistics about created inputs in job with given ID.
     * If job ID is empty, then job is not created.
     * If job ID is non-empty and doesn't already exist, then a new job will be created with given ID.
     * If job ID does already exist, then new inputs statistics are merged with previous inputs statistics.
     """
+    input_id_conflict_resolution: proto.clarifai.api.resources_pb2.InputIDConflictResolution.ValueType
+    """How to handle input ID conflicts."""
     def __init__(
         self,
         *,
         user_app_id: proto.clarifai.api.resources_pb2.UserAppIDSet | None = ...,
         inputs: collections.abc.Iterable[proto.clarifai.api.resources_pb2.Input] | None = ...,
         inputs_add_job_id: builtins.str = ...,
+        input_id_conflict_resolution: proto.clarifai.api.resources_pb2.InputIDConflictResolution.ValueType = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["user_app_id", b"user_app_id"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["inputs", b"inputs", "inputs_add_job_id", b"inputs_add_job_id", "user_app_id", b"user_app_id"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["input_id_conflict_resolution", b"input_id_conflict_resolution", "inputs", b"inputs", "inputs_add_job_id", b"inputs_add_job_id", "user_app_id", b"user_app_id"]) -> None: ...
 
 global___PostInputsRequest = PostInputsRequest
 
 @typing_extensions.final
 class PatchInputsRequest(google.protobuf.message.Message):
     """PatchInputsRequest"""
 
@@ -2001,14 +2012,18 @@
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     STATUS_FIELD_NUMBER: builtins.int
     MANIFEST_URL_FIELD_NUMBER: builtins.int
     @property
     def status(self) -> proto.clarifai.api.status.status_pb2.Status: ...
     manifest_url: builtins.str
+    """MPEG-dash manifest as data-URI, base64-encoded
+    Can be empty if status is FAILED
+    Can be fallback manifest if status is MIXED_STATUS
+    """
     def __init__(
         self,
         *,
         status: proto.clarifai.api.status.status_pb2.Status | None = ...,
         manifest_url: builtins.str = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["status", b"status"]) -> builtins.bool: ...
@@ -2224,44 +2239,14 @@
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["user_app_id", b"user_app_id"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["action", b"action", "datasets", b"datasets", "user_app_id", b"user_app_id"]) -> None: ...
 
 global___PatchDatasetsRequest = PatchDatasetsRequest
 
 @typing_extensions.final
-class PatchDatasetIdsRequest(google.protobuf.message.Message):
-    """PatchDatasetIdsRequest"""
-
-    DESCRIPTOR: google.protobuf.descriptor.Descriptor
-
-    USER_APP_ID_FIELD_NUMBER: builtins.int
-    IDS_FIELD_NUMBER: builtins.int
-    ACTION_FIELD_NUMBER: builtins.int
-    @property
-    def user_app_id(self) -> proto.clarifai.api.resources_pb2.UserAppIDSet: ...
-    @property
-    def ids(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___IdUpdateSource]:
-        """Array containing 1 entry"""
-    action: builtins.str
-    """The action to perform on the patched objects
-    Only 'overwrite' is supported
-    """
-    def __init__(
-        self,
-        *,
-        user_app_id: proto.clarifai.api.resources_pb2.UserAppIDSet | None = ...,
-        ids: collections.abc.Iterable[global___IdUpdateSource] | None = ...,
-        action: builtins.str = ...,
-    ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["user_app_id", b"user_app_id"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["action", b"action", "ids", b"ids", "user_app_id", b"user_app_id"]) -> None: ...
-
-global___PatchDatasetIdsRequest = PatchDatasetIdsRequest
-
-@typing_extensions.final
 class DeleteDatasetsRequest(google.protobuf.message.Message):
     """Request to delete several datasets by list of ids."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     USER_APP_ID_FIELD_NUMBER: builtins.int
     DATASET_IDS_FIELD_NUMBER: builtins.int
@@ -3321,14 +3306,64 @@
     def HasField(self, field_name: typing_extensions.Literal["sort_by", b"sort_by", "sort_by_modified_at", b"sort_by_modified_at", "sort_by_name", b"sort_by_name", "sort_by_num_inputs", b"sort_by_num_inputs", "user_app_id", b"user_app_id"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["additional_fields", b"additional_fields", "dont_fetch_from_main", b"dont_fetch_from_main", "featured_only", b"featured_only", "filter_by_user_id", b"filter_by_user_id", "input_fields", b"input_fields", "languages", b"languages", "license", b"license", "model_type_id", b"model_type_id", "name", b"name", "output_fields", b"output_fields", "page", b"page", "per_page", b"per_page", "query", b"query", "sort_ascending", b"sort_ascending", "sort_by", b"sort_by", "sort_by_modified_at", b"sort_by_modified_at", "sort_by_name", b"sort_by_name", "sort_by_num_inputs", b"sort_by_num_inputs", "starred_only", b"starred_only", "toolkits", b"toolkits", "trained_only", b"trained_only", "use_cases", b"use_cases", "user_app_id", b"user_app_id"]) -> None: ...
     def WhichOneof(self, oneof_group: typing_extensions.Literal["sort_by", b"sort_by"]) -> typing_extensions.Literal["sort_by_name", "sort_by_num_inputs", "sort_by_modified_at"] | None: ...
 
 global___ListModelsRequest = ListModelsRequest
 
 @typing_extensions.final
+class GetResourceCountsRequest(google.protobuf.message.Message):
+    """ResourceCountRequest"""
+
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+    USER_APP_ID_FIELD_NUMBER: builtins.int
+    @property
+    def user_app_id(self) -> proto.clarifai.api.resources_pb2.UserAppIDSet: ...
+    def __init__(
+        self,
+        *,
+        user_app_id: proto.clarifai.api.resources_pb2.UserAppIDSet | None = ...,
+    ) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["user_app_id", b"user_app_id"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["user_app_id", b"user_app_id"]) -> None: ...
+
+global___GetResourceCountsRequest = GetResourceCountsRequest
+
+@typing_extensions.final
+class GetResourceCountsResponse(google.protobuf.message.Message):
+    """ResourceCountResponse"""
+
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+    STATUS_FIELD_NUMBER: builtins.int
+    DATASETS_FIELD_NUMBER: builtins.int
+    MODELS_FIELD_NUMBER: builtins.int
+    WORKFLOWS_FIELD_NUMBER: builtins.int
+    MODULES_FIELD_NUMBER: builtins.int
+    @property
+    def status(self) -> proto.clarifai.api.status.status_pb2.Status: ...
+    datasets: builtins.int
+    models: builtins.int
+    workflows: builtins.int
+    modules: builtins.int
+    def __init__(
+        self,
+        *,
+        status: proto.clarifai.api.status.status_pb2.Status | None = ...,
+        datasets: builtins.int = ...,
+        models: builtins.int = ...,
+        workflows: builtins.int = ...,
+        modules: builtins.int = ...,
+    ) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["status", b"status"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["datasets", b"datasets", "models", b"models", "modules", b"modules", "status", b"status", "workflows", b"workflows"]) -> None: ...
+
+global___GetResourceCountsResponse = GetResourceCountsResponse
+
+@typing_extensions.final
 class PatchModelToolkitsRequest(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     USER_APP_ID_FIELD_NUMBER: builtins.int
     MODEL_ID_FIELD_NUMBER: builtins.int
     TOOLKITS_FIELD_NUMBER: builtins.int
     ACTION_FIELD_NUMBER: builtins.int
@@ -4158,14 +4193,96 @@
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["user_app_id", b"user_app_id"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["model_id", b"model_id", "publications", b"publications", "user_app_id", b"user_app_id"]) -> None: ...
 
 global___PostModelVersionsUnPublishRequest = PostModelVersionsUnPublishRequest
 
 @typing_extensions.final
+class PostEvaluationsRequest(google.protobuf.message.Message):
+    """Evaluate this model vesion"""
+
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+    USER_APP_ID_FIELD_NUMBER: builtins.int
+    EVAL_METRICS_FIELD_NUMBER: builtins.int
+    @property
+    def user_app_id(self) -> proto.clarifai.api.resources_pb2.UserAppIDSet: ...
+    @property
+    def eval_metrics(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[proto.clarifai.api.resources_pb2.EvalMetrics]:
+        """eval_info, id, model, and ground_truth_dataset will be used when creating the evaluation
+        If no dataset is provided, all app data that is annotated with concepts from the model will be used.
+        """
+    def __init__(
+        self,
+        *,
+        user_app_id: proto.clarifai.api.resources_pb2.UserAppIDSet | None = ...,
+        eval_metrics: collections.abc.Iterable[proto.clarifai.api.resources_pb2.EvalMetrics] | None = ...,
+    ) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["user_app_id", b"user_app_id"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["eval_metrics", b"eval_metrics", "user_app_id", b"user_app_id"]) -> None: ...
+
+global___PostEvaluationsRequest = PostEvaluationsRequest
+
+@typing_extensions.final
+class ListEvaluationsRequest(google.protobuf.message.Message):
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+    USER_APP_ID_FIELD_NUMBER: builtins.int
+    PAGE_FIELD_NUMBER: builtins.int
+    PER_PAGE_FIELD_NUMBER: builtins.int
+    @property
+    def user_app_id(self) -> proto.clarifai.api.resources_pb2.UserAppIDSet: ...
+    page: builtins.int
+    """(optional URL parameter) The page number. Pagination is used to split the results into chunks.
+    Defaults to 1.
+    """
+    per_page: builtins.int
+    """(optional URL parameter) The number of results that will be contained in each page. Defaults
+    to 128.
+    """
+    def __init__(
+        self,
+        *,
+        user_app_id: proto.clarifai.api.resources_pb2.UserAppIDSet | None = ...,
+        page: builtins.int = ...,
+        per_page: builtins.int = ...,
+    ) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["user_app_id", b"user_app_id"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["page", b"page", "per_page", b"per_page", "user_app_id", b"user_app_id"]) -> None: ...
+
+global___ListEvaluationsRequest = ListEvaluationsRequest
+
+@typing_extensions.final
+class GetEvaluationRequest(google.protobuf.message.Message):
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+    USER_APP_ID_FIELD_NUMBER: builtins.int
+    EVALUATION_ID_FIELD_NUMBER: builtins.int
+    FIELDS_FIELD_NUMBER: builtins.int
+    @property
+    def user_app_id(self) -> proto.clarifai.api.resources_pb2.UserAppIDSet: ...
+    evaluation_id: builtins.str
+    @property
+    def fields(self) -> proto.clarifai.api.resources_pb2.FieldsValue:
+        """Any of the fields you wish to return in the metrics
+        By default, only the summary is returned.
+        """
+    def __init__(
+        self,
+        *,
+        user_app_id: proto.clarifai.api.resources_pb2.UserAppIDSet | None = ...,
+        evaluation_id: builtins.str = ...,
+        fields: proto.clarifai.api.resources_pb2.FieldsValue | None = ...,
+    ) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["fields", b"fields", "user_app_id", b"user_app_id"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["evaluation_id", b"evaluation_id", "fields", b"fields", "user_app_id", b"user_app_id"]) -> None: ...
+
+global___GetEvaluationRequest = GetEvaluationRequest
+
+@typing_extensions.final
 class PostModelVersionEvaluationsRequest(google.protobuf.message.Message):
     """Evaluate this model vesion"""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     USER_APP_ID_FIELD_NUMBER: builtins.int
     MODEL_ID_FIELD_NUMBER: builtins.int
@@ -8068,14 +8185,35 @@
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["user_app_id", b"user_app_id"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["id", b"id", "user_app_id", b"user_app_id"]) -> None: ...
 
 global___GetInputsAddJobRequest = GetInputsAddJobRequest
 
 @typing_extensions.final
+class CancelInputsAddJobRequest(google.protobuf.message.Message):
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+    USER_APP_ID_FIELD_NUMBER: builtins.int
+    ID_FIELD_NUMBER: builtins.int
+    @property
+    def user_app_id(self) -> proto.clarifai.api.resources_pb2.UserAppIDSet: ...
+    id: builtins.str
+    """id of add inputs job to be cancelled"""
+    def __init__(
+        self,
+        *,
+        user_app_id: proto.clarifai.api.resources_pb2.UserAppIDSet | None = ...,
+        id: builtins.str = ...,
+    ) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["user_app_id", b"user_app_id"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["id", b"id", "user_app_id", b"user_app_id"]) -> None: ...
+
+global___CancelInputsAddJobRequest = CancelInputsAddJobRequest
+
+@typing_extensions.final
 class MultiInputsAddJobResponse(google.protobuf.message.Message):
     """MultiInputsAddJobResponse"""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     STATUS_FIELD_NUMBER: builtins.int
     INPUTS_ADD_JOBS_FIELD_NUMBER: builtins.int
```

### Comparing `clarifai-grpc-9.5.0/clarifai_grpc/grpc/api/service_pb2_grpc.py` & `clarifai-grpc-9.6.0/clarifai_grpc/grpc/api/service_pb2_grpc.py`

 * *Files 1% similar despite different names*

```diff
@@ -245,19 +245,14 @@
                 response_deserializer=wrap_response_deserializer(proto_dot_clarifai_dot_api_dot_service__pb2.MultiDatasetResponse),
                 )
         self.PatchDatasets = channel.unary_unary(
                 '/clarifai.api.V2/PatchDatasets',
                 request_serializer=proto_dot_clarifai_dot_api_dot_service__pb2.PatchDatasetsRequest.SerializeToString,
                 response_deserializer=wrap_response_deserializer(proto_dot_clarifai_dot_api_dot_service__pb2.MultiDatasetResponse),
                 )
-        self.PatchDatasetIds = channel.unary_unary(
-                '/clarifai.api.V2/PatchDatasetIds',
-                request_serializer=proto_dot_clarifai_dot_api_dot_service__pb2.PatchDatasetIdsRequest.SerializeToString,
-                response_deserializer=wrap_response_deserializer(proto_dot_clarifai_dot_api_dot_service__pb2.MultiDatasetResponse),
-                )
         self.DeleteDatasets = channel.unary_unary(
                 '/clarifai.api.V2/DeleteDatasets',
                 request_serializer=proto_dot_clarifai_dot_api_dot_service__pb2.DeleteDatasetsRequest.SerializeToString,
                 response_deserializer=wrap_response_deserializer(proto_dot_clarifai_dot_api_dot_status_dot_status__pb2.BaseResponse),
                 )
         self.ListDatasetInputs = channel.unary_unary(
                 '/clarifai.api.V2/ListDatasetInputs',
@@ -340,14 +335,19 @@
                 response_deserializer=wrap_response_deserializer(proto_dot_clarifai_dot_api_dot_service__pb2.SingleModelResponse),
                 )
         self.ListModels = channel.unary_unary(
                 '/clarifai.api.V2/ListModels',
                 request_serializer=proto_dot_clarifai_dot_api_dot_service__pb2.ListModelsRequest.SerializeToString,
                 response_deserializer=wrap_response_deserializer(proto_dot_clarifai_dot_api_dot_service__pb2.MultiModelResponse),
                 )
+        self.GetResourceCounts = channel.unary_unary(
+                '/clarifai.api.V2/GetResourceCounts',
+                request_serializer=proto_dot_clarifai_dot_api_dot_service__pb2.GetResourceCountsRequest.SerializeToString,
+                response_deserializer=wrap_response_deserializer(proto_dot_clarifai_dot_api_dot_service__pb2.GetResourceCountsResponse),
+                )
         self.PostModelsSearches = channel.unary_unary(
                 '/clarifai.api.V2/PostModelsSearches',
                 request_serializer=proto_dot_clarifai_dot_api_dot_service__pb2.PostModelsSearchesRequest.SerializeToString,
                 response_deserializer=wrap_response_deserializer(proto_dot_clarifai_dot_api_dot_service__pb2.MultiModelResponse),
                 )
         self.PostModels = channel.unary_unary(
                 '/clarifai.api.V2/PostModels',
@@ -465,14 +465,29 @@
                 response_deserializer=wrap_response_deserializer(proto_dot_clarifai_dot_api_dot_service__pb2.MultiEvalMetricsResponse),
                 )
         self.GetModelVersionEvaluation = channel.unary_unary(
                 '/clarifai.api.V2/GetModelVersionEvaluation',
                 request_serializer=proto_dot_clarifai_dot_api_dot_service__pb2.GetModelVersionEvaluationRequest.SerializeToString,
                 response_deserializer=wrap_response_deserializer(proto_dot_clarifai_dot_api_dot_service__pb2.SingleEvalMetricsResponse),
                 )
+        self.PostEvaluations = channel.unary_unary(
+                '/clarifai.api.V2/PostEvaluations',
+                request_serializer=proto_dot_clarifai_dot_api_dot_service__pb2.PostEvaluationsRequest.SerializeToString,
+                response_deserializer=wrap_response_deserializer(proto_dot_clarifai_dot_api_dot_service__pb2.MultiEvalMetricsResponse),
+                )
+        self.ListEvaluations = channel.unary_unary(
+                '/clarifai.api.V2/ListEvaluations',
+                request_serializer=proto_dot_clarifai_dot_api_dot_service__pb2.ListEvaluationsRequest.SerializeToString,
+                response_deserializer=wrap_response_deserializer(proto_dot_clarifai_dot_api_dot_service__pb2.MultiEvalMetricsResponse),
+                )
+        self.GetEvaluation = channel.unary_unary(
+                '/clarifai.api.V2/GetEvaluation',
+                request_serializer=proto_dot_clarifai_dot_api_dot_service__pb2.GetEvaluationRequest.SerializeToString,
+                response_deserializer=wrap_response_deserializer(proto_dot_clarifai_dot_api_dot_service__pb2.SingleEvalMetricsResponse),
+                )
         self.ListModelReferences = channel.unary_unary(
                 '/clarifai.api.V2/ListModelReferences',
                 request_serializer=proto_dot_clarifai_dot_api_dot_service__pb2.ListModelReferencesRequest.SerializeToString,
                 response_deserializer=wrap_response_deserializer(proto_dot_clarifai_dot_api_dot_service__pb2.MultiModelReferenceResponse),
                 )
         self.GetModelVersionInputExample = channel.unary_unary(
                 '/clarifai.api.V2/GetModelVersionInputExample',
@@ -995,14 +1010,19 @@
                 response_deserializer=wrap_response_deserializer(proto_dot_clarifai_dot_api_dot_service__pb2.MultiInputsAddJobResponse),
                 )
         self.GetInputsAddJob = channel.unary_unary(
                 '/clarifai.api.V2/GetInputsAddJob',
                 request_serializer=proto_dot_clarifai_dot_api_dot_service__pb2.GetInputsAddJobRequest.SerializeToString,
                 response_deserializer=wrap_response_deserializer(proto_dot_clarifai_dot_api_dot_service__pb2.SingleInputsAddJobResponse),
                 )
+        self.CancelInputsAddJob = channel.unary_unary(
+                '/clarifai.api.V2/CancelInputsAddJob',
+                request_serializer=proto_dot_clarifai_dot_api_dot_service__pb2.CancelInputsAddJobRequest.SerializeToString,
+                response_deserializer=wrap_response_deserializer(proto_dot_clarifai_dot_api_dot_service__pb2.SingleInputsAddJobResponse),
+                )
         self.PostUploads = channel.unary_unary(
                 '/clarifai.api.V2/PostUploads',
                 request_serializer=proto_dot_clarifai_dot_api_dot_service__pb2.PostUploadsRequest.SerializeToString,
                 response_deserializer=wrap_response_deserializer(proto_dot_clarifai_dot_api_dot_service__pb2.MultiUploadResponse),
                 )
         self.PutUploadContentParts = channel.unary_unary(
                 '/clarifai.api.V2/PutUploadContentParts',
@@ -1382,21 +1402,14 @@
         If there is an error for one dataset,
         the process will stop, revert the transaction and return the error.
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def PatchDatasetIds(self, request, context):
-        """Patch one or more dataset ids.
-        """
-        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details('Method not implemented!')
-        raise NotImplementedError('Method not implemented!')
-
     def DeleteDatasets(self, request, context):
         """Delete one or more datasets in a single request.
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
@@ -1527,14 +1540,21 @@
     def ListModels(self, request, context):
         """List all the models.
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
+    def GetResourceCounts(self, request, context):
+        """List the resource counts for the app.
+        """
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
     def PostModelsSearches(self, request, context):
         """Search over the models to find one or more you're looking for.
         This leverage the "body" parameter because we also have page and
         per_page as url query param variables in this request.
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
@@ -1670,49 +1690,70 @@
         """Delete a single model.
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def GetModelVersionMetrics(self, request, context):
-        """Deprecated: Use GetModelVersionEvaluation instead
+        """Deprecated: Use GetEvaluation instead
         Get the evaluation metrics for a model version.
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def PostModelVersionMetrics(self, request, context):
-        """Deprecated, use PostModelVersionEvaluations instead
+        """Deprecated, use PostEvaluations instead
         Run the evaluation metrics for a model version.
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def PostModelVersionEvaluations(self, request, context):
-        """Missing associated documentation comment in .proto file."""
+        """Deprecated, use PostEvaluations instead
+        """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def ListModelVersionEvaluations(self, request, context):
-        """List the evaluation metrics for a model version.
+        """Deprecated, use GetEvaluation instead
+        List the evaluation metrics for a model version.
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def GetModelVersionEvaluation(self, request, context):
-        """Get an evaluation metrics for a model version.
+        """Deprecated, use GetEvaluation instead
+        Get an evaluation metrics for a model version.
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
+    def PostEvaluations(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+    def ListEvaluations(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+    def GetEvaluation(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
     def ListModelReferences(self, request, context):
         """Lists model references tied to a particular model id.
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
@@ -2478,14 +2519,21 @@
     def GetInputsAddJob(self, request, context):
         """Get the input add job details by ID
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
+    def CancelInputsAddJob(self, request, context):
+        """cancel the input add job by ID
+        """
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
     def PostUploads(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def PutUploadContentParts(self, request, context):
@@ -2778,19 +2826,14 @@
                     response_serializer=proto_dot_clarifai_dot_api_dot_service__pb2.MultiDatasetResponse.SerializeToString,
             ),
             'PatchDatasets': grpc.unary_unary_rpc_method_handler(
                     servicer.PatchDatasets,
                     request_deserializer=proto_dot_clarifai_dot_api_dot_service__pb2.PatchDatasetsRequest.FromString,
                     response_serializer=proto_dot_clarifai_dot_api_dot_service__pb2.MultiDatasetResponse.SerializeToString,
             ),
-            'PatchDatasetIds': grpc.unary_unary_rpc_method_handler(
-                    servicer.PatchDatasetIds,
-                    request_deserializer=proto_dot_clarifai_dot_api_dot_service__pb2.PatchDatasetIdsRequest.FromString,
-                    response_serializer=proto_dot_clarifai_dot_api_dot_service__pb2.MultiDatasetResponse.SerializeToString,
-            ),
             'DeleteDatasets': grpc.unary_unary_rpc_method_handler(
                     servicer.DeleteDatasets,
                     request_deserializer=proto_dot_clarifai_dot_api_dot_service__pb2.DeleteDatasetsRequest.FromString,
                     response_serializer=proto_dot_clarifai_dot_api_dot_status_dot_status__pb2.BaseResponse.SerializeToString,
             ),
             'ListDatasetInputs': grpc.unary_unary_rpc_method_handler(
                     servicer.ListDatasetInputs,
@@ -2873,14 +2916,19 @@
                     response_serializer=proto_dot_clarifai_dot_api_dot_service__pb2.SingleModelResponse.SerializeToString,
             ),
             'ListModels': grpc.unary_unary_rpc_method_handler(
                     servicer.ListModels,
                     request_deserializer=proto_dot_clarifai_dot_api_dot_service__pb2.ListModelsRequest.FromString,
                     response_serializer=proto_dot_clarifai_dot_api_dot_service__pb2.MultiModelResponse.SerializeToString,
             ),
+            'GetResourceCounts': grpc.unary_unary_rpc_method_handler(
+                    servicer.GetResourceCounts,
+                    request_deserializer=proto_dot_clarifai_dot_api_dot_service__pb2.GetResourceCountsRequest.FromString,
+                    response_serializer=proto_dot_clarifai_dot_api_dot_service__pb2.GetResourceCountsResponse.SerializeToString,
+            ),
             'PostModelsSearches': grpc.unary_unary_rpc_method_handler(
                     servicer.PostModelsSearches,
                     request_deserializer=proto_dot_clarifai_dot_api_dot_service__pb2.PostModelsSearchesRequest.FromString,
                     response_serializer=proto_dot_clarifai_dot_api_dot_service__pb2.MultiModelResponse.SerializeToString,
             ),
             'PostModels': grpc.unary_unary_rpc_method_handler(
                     servicer.PostModels,
@@ -2998,14 +3046,29 @@
                     response_serializer=proto_dot_clarifai_dot_api_dot_service__pb2.MultiEvalMetricsResponse.SerializeToString,
             ),
             'GetModelVersionEvaluation': grpc.unary_unary_rpc_method_handler(
                     servicer.GetModelVersionEvaluation,
                     request_deserializer=proto_dot_clarifai_dot_api_dot_service__pb2.GetModelVersionEvaluationRequest.FromString,
                     response_serializer=proto_dot_clarifai_dot_api_dot_service__pb2.SingleEvalMetricsResponse.SerializeToString,
             ),
+            'PostEvaluations': grpc.unary_unary_rpc_method_handler(
+                    servicer.PostEvaluations,
+                    request_deserializer=proto_dot_clarifai_dot_api_dot_service__pb2.PostEvaluationsRequest.FromString,
+                    response_serializer=proto_dot_clarifai_dot_api_dot_service__pb2.MultiEvalMetricsResponse.SerializeToString,
+            ),
+            'ListEvaluations': grpc.unary_unary_rpc_method_handler(
+                    servicer.ListEvaluations,
+                    request_deserializer=proto_dot_clarifai_dot_api_dot_service__pb2.ListEvaluationsRequest.FromString,
+                    response_serializer=proto_dot_clarifai_dot_api_dot_service__pb2.MultiEvalMetricsResponse.SerializeToString,
+            ),
+            'GetEvaluation': grpc.unary_unary_rpc_method_handler(
+                    servicer.GetEvaluation,
+                    request_deserializer=proto_dot_clarifai_dot_api_dot_service__pb2.GetEvaluationRequest.FromString,
+                    response_serializer=proto_dot_clarifai_dot_api_dot_service__pb2.SingleEvalMetricsResponse.SerializeToString,
+            ),
             'ListModelReferences': grpc.unary_unary_rpc_method_handler(
                     servicer.ListModelReferences,
                     request_deserializer=proto_dot_clarifai_dot_api_dot_service__pb2.ListModelReferencesRequest.FromString,
                     response_serializer=proto_dot_clarifai_dot_api_dot_service__pb2.MultiModelReferenceResponse.SerializeToString,
             ),
             'GetModelVersionInputExample': grpc.unary_unary_rpc_method_handler(
                     servicer.GetModelVersionInputExample,
@@ -3528,14 +3591,19 @@
                     response_serializer=proto_dot_clarifai_dot_api_dot_service__pb2.MultiInputsAddJobResponse.SerializeToString,
             ),
             'GetInputsAddJob': grpc.unary_unary_rpc_method_handler(
                     servicer.GetInputsAddJob,
                     request_deserializer=proto_dot_clarifai_dot_api_dot_service__pb2.GetInputsAddJobRequest.FromString,
                     response_serializer=proto_dot_clarifai_dot_api_dot_service__pb2.SingleInputsAddJobResponse.SerializeToString,
             ),
+            'CancelInputsAddJob': grpc.unary_unary_rpc_method_handler(
+                    servicer.CancelInputsAddJob,
+                    request_deserializer=proto_dot_clarifai_dot_api_dot_service__pb2.CancelInputsAddJobRequest.FromString,
+                    response_serializer=proto_dot_clarifai_dot_api_dot_service__pb2.SingleInputsAddJobResponse.SerializeToString,
+            ),
             'PostUploads': grpc.unary_unary_rpc_method_handler(
                     servicer.PostUploads,
                     request_deserializer=proto_dot_clarifai_dot_api_dot_service__pb2.PostUploadsRequest.FromString,
                     response_serializer=proto_dot_clarifai_dot_api_dot_service__pb2.MultiUploadResponse.SerializeToString,
             ),
             'PutUploadContentParts': grpc.unary_unary_rpc_method_handler(
                     servicer.PutUploadContentParts,
@@ -4338,31 +4406,14 @@
         return grpc.experimental.unary_unary(request, target, '/clarifai.api.V2/PatchDatasets',
             proto_dot_clarifai_dot_api_dot_service__pb2.PatchDatasetsRequest.SerializeToString,
             proto_dot_clarifai_dot_api_dot_service__pb2.MultiDatasetResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def PatchDatasetIds(request,
-            target,
-            options=(),
-            channel_credentials=None,
-            call_credentials=None,
-            insecure=False,
-            compression=None,
-            wait_for_ready=None,
-            timeout=None,
-            metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/clarifai.api.V2/PatchDatasetIds',
-            proto_dot_clarifai_dot_api_dot_service__pb2.PatchDatasetIdsRequest.SerializeToString,
-            proto_dot_clarifai_dot_api_dot_service__pb2.MultiDatasetResponse.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
-
-    @staticmethod
     def DeleteDatasets(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
@@ -4661,14 +4712,31 @@
         return grpc.experimental.unary_unary(request, target, '/clarifai.api.V2/ListModels',
             proto_dot_clarifai_dot_api_dot_service__pb2.ListModelsRequest.SerializeToString,
             proto_dot_clarifai_dot_api_dot_service__pb2.MultiModelResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
+    def GetResourceCounts(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/clarifai.api.V2/GetResourceCounts',
+            proto_dot_clarifai_dot_api_dot_service__pb2.GetResourceCountsRequest.SerializeToString,
+            proto_dot_clarifai_dot_api_dot_service__pb2.GetResourceCountsResponse.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
     def PostModelsSearches(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
@@ -5086,14 +5154,65 @@
         return grpc.experimental.unary_unary(request, target, '/clarifai.api.V2/GetModelVersionEvaluation',
             proto_dot_clarifai_dot_api_dot_service__pb2.GetModelVersionEvaluationRequest.SerializeToString,
             proto_dot_clarifai_dot_api_dot_service__pb2.SingleEvalMetricsResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
+    def PostEvaluations(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/clarifai.api.V2/PostEvaluations',
+            proto_dot_clarifai_dot_api_dot_service__pb2.PostEvaluationsRequest.SerializeToString,
+            proto_dot_clarifai_dot_api_dot_service__pb2.MultiEvalMetricsResponse.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def ListEvaluations(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/clarifai.api.V2/ListEvaluations',
+            proto_dot_clarifai_dot_api_dot_service__pb2.ListEvaluationsRequest.SerializeToString,
+            proto_dot_clarifai_dot_api_dot_service__pb2.MultiEvalMetricsResponse.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def GetEvaluation(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/clarifai.api.V2/GetEvaluation',
+            proto_dot_clarifai_dot_api_dot_service__pb2.GetEvaluationRequest.SerializeToString,
+            proto_dot_clarifai_dot_api_dot_service__pb2.SingleEvalMetricsResponse.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
     def ListModelReferences(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
@@ -6888,14 +7007,31 @@
         return grpc.experimental.unary_unary(request, target, '/clarifai.api.V2/GetInputsAddJob',
             proto_dot_clarifai_dot_api_dot_service__pb2.GetInputsAddJobRequest.SerializeToString,
             proto_dot_clarifai_dot_api_dot_service__pb2.SingleInputsAddJobResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
+    def CancelInputsAddJob(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/clarifai.api.V2/CancelInputsAddJob',
+            proto_dot_clarifai_dot_api_dot_service__pb2.CancelInputsAddJobRequest.SerializeToString,
+            proto_dot_clarifai_dot_api_dot_service__pb2.SingleInputsAddJobResponse.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
     def PostUploads(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
```

### Comparing `clarifai-grpc-9.5.0/clarifai_grpc/grpc/api/status/status_code_pb2.py` & `clarifai-grpc-9.6.0/clarifai_grpc/grpc/api/status/status_code_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n+proto/clarifai/api/status/status_code.proto\x12\x13\x63larifai.api.status*\xa3Q\n\nStatusCode\x12\x08\n\x04ZERO\x10\x00\x12\x0c\n\x07SUCCESS\x10\x90N\x12\x11\n\x0cMIXED_STATUS\x10\x9aN\x12\x0c\n\x07\x46\x41ILURE\x10\xa4N\x12\x0e\n\tTRY_AGAIN\x10\xaeN\x12\x14\n\x0fNOT_IMPLEMENTED\x10\xb8N\x12\n\n\x05MOVED\x10\xc2N\x12\x18\n\x13\x43ONN_ACCOUNT_ISSUES\x10\xf8U\x12\x1b\n\x12\x43ONN_TOKEN_INVALID\x10\xf9U\x1a\x02\x08\x01\x12\x1d\n\x18\x43ONN_CREDENTIALS_INVALID\x10\xfaU\x12\x1d\n\x18\x43ONN_EXCEED_HOURLY_LIMIT\x10\xfbU\x12\x1e\n\x19\x43ONN_EXCEED_MONTHLY_LIMIT\x10\xfcU\x12\x13\n\x0e\x43ONN_THROTTLED\x10\xfdU\x12\x18\n\x13\x43ONN_EXCEEDS_LIMITS\x10\xfeU\x12\x1d\n\x18\x43ONN_INSUFFICIENT_SCOPES\x10\xffU\x12\x15\n\x10\x43ONN_KEY_INVALID\x10\x80V\x12\x17\n\x12\x43ONN_KEY_NOT_FOUND\x10\x81V\x12\x1c\n\x17\x43ONN_BAD_REQUEST_FORMAT\x10\xdcV\x12\x18\n\x13\x43ONN_DOES_NOT_EXIST\x10\xddV\x12\x19\n\x14\x43ONN_INVALID_REQUEST\x10\xdeV\x12\x1c\n\x17\x43ONN_METHOD_NOT_ALLOWED\x10\xdfV\x12\x19\n\x14\x43ONN_NO_GDPR_CONSENT\x10\xe0V\x12\x1e\n\x19\x43ONN_AUTH_METHOD_DISABLED\x10\xc0W\x12\x13\n\rMODEL_TRAINED\x10\xec\xa4\x01\x12\x14\n\x0eMODEL_TRAINING\x10\xed\xa4\x01\x12\x15\n\x0fMODEL_UNTRAINED\x10\xee\xa4\x01\x12\x1f\n\x19MODEL_QUEUED_FOR_TRAINING\x10\xef\xa4\x01\x12\x15\n\x0fMODEL_UPLOADING\x10\xf0\xa4\x01\x12\x1c\n\x16MODEL_UPLOADING_FAILED\x10\xf1\xa4\x01\x12\x1b\n\x15MODEL_TRAINING_FAILED\x10\xf2\xa4\x01\x12\x1c\n\x16MODEL_TRAINING_NO_DATA\x10\xf6\xa4\x01\x12!\n\x1bMODEL_TRAINING_NO_POSITIVES\x10\xf7\xa4\x01\x12*\n$MODEL_TRAINING_ONE_VS_N_SINGLE_CLASS\x10\xf8\xa4\x01\x12\x1e\n\x18MODEL_TRAINING_TIMED_OUT\x10\xf9\xa4\x01\x12\"\n\x1cMODEL_TRAINING_WAITING_ERROR\x10\xfa\xa4\x01\x12\"\n\x1cMODEL_TRAINING_UNKNOWN_ERROR\x10\xfb\xa4\x01\x12&\n\x1cMODEL_TRAINING_MSG_REDELIVER\x10\xfc\xa4\x01\x1a\x02\x08\x01\x12&\n MODEL_TRAINING_INSUFFICIENT_DATA\x10\xfd\xa4\x01\x12#\n\x1dMODEL_TRAINING_INVALID_PARAMS\x10\xfe\xa4\x01\x12\x34\n.MODEL_TRAINING_INVALID_DATA_TOLERANCE_EXCEEDED\x10\xff\xa4\x01\x12\x1a\n\x14MODEL_MODIFY_SUCCESS\x10\x9e\xa5\x01\x12\x1a\n\x14MODEL_MODIFY_PENDING\x10\x9f\xa5\x01\x12\x19\n\x13MODEL_MODIFY_FAILED\x10\xa0\xa5\x01\x12\x1a\n\x14MODEL_DOES_NOT_EXIST\x10\xd0\xa5\x01\x12\x1d\n\x17MODEL_PERMISSION_DENIED\x10\xd1\xa5\x01\x12\x1c\n\x16MODEL_INVALID_ARGUMENT\x10\xd2\xa5\x01\x12\x1b\n\x15MODEL_INVALID_REQUEST\x10\xd3\xa5\x01\x12\x15\n\x0fMODEL_EVALUATED\x10\xb4\xa6\x01\x12\x16\n\x10MODEL_EVALUATING\x10\xb5\xa6\x01\x12\x19\n\x13MODEL_NOT_EVALUATED\x10\xb6\xa6\x01\x12!\n\x1bMODEL_QUEUED_FOR_EVALUATION\x10\xb7\xa6\x01\x12 \n\x1aMODEL_EVALUATION_TIMED_OUT\x10\xbe\xa6\x01\x12$\n\x1eMODEL_EVALUATION_WAITING_ERROR\x10\xbf\xa6\x01\x12$\n\x1eMODEL_EVALUATION_UNKNOWN_ERROR\x10\xc0\xa6\x01\x12\x1d\n\x17MODEL_PREDICTION_FAILED\x10\xc1\xa6\x01\x12(\n\x1eMODEL_EVALUATION_MSG_REDELIVER\x10\xc2\xa6\x01\x1a\x02\x08\x01\x12\"\n\x1cMODEL_EVALUATION_NEED_LABELS\x10\xc3\xa6\x01\x12\"\n\x1cMODEL_EVALUATION_NEED_INPUTS\x10\xc4\xa6\x01\x12\x1d\n\x17MODEL_EVALUATION_FAILED\x10\xc5\xa6\x01\x12\x1d\n\x17MODEL_DEPLOYMENT_FAILED\x10\xe6\xa6\x01\x12\x15\n\x0fMODEL_DEPLOYING\x10\xe7\xa6\x01\x12!\n\x1bMODEL_QUEUED_FOR_DEPLOYMENT\x10\xe8\xa6\x01\x12\x18\n\x12MODEL_NOT_DEPLOYED\x10\xe9\xa6\x01\x12&\n MODEL_REFERENCE_INVALID_ARGUMENT\x10\x98\xa7\x01\x12*\n$MODEL_EXAMPLE_INPUT_INVALID_ARGUMENT\x10\xac\xa7\x01\x12 \n\x1aWORKFLOW_NO_MATCHING_INPUT\x10\xf1\xab\x01\x12$\n\x1eWORKFLOW_REQUIRE_TRAINED_MODEL\x10\xf2\xab\x01\x12\x18\n\x12WORKFLOW_DUPLICATE\x10\xd4\xac\x01\x12!\n\x1bWORKFLOW_UNSUPPORTED_FORMAT\x10\xd5\xac\x01\x12\x1d\n\x17WORKFLOW_DOES_NOT_EXIST\x10\xd6\xac\x01\x12 \n\x1aWORKFLOW_PERMISSION_DENIED\x10\xd7\xac\x01\x12\x1f\n\x19WORKFLOW_INVALID_ARGUMENT\x10\xd8\xac\x01\x12\x1d\n\x17WORKFLOW_INVALID_RECIPE\x10\xd9\xac\x01\x12\x1f\n\x19WORKFLOW_INVALID_TEMPLATE\x10\xda\xac\x01\x12\x1c\n\x16WORKFLOW_INVALID_GRAPH\x10\xdb\xac\x01\x12\x1f\n\x19WORKFLOW_INTERNAL_FAILURE\x10\xdc\xac\x01\x12\x1e\n\x18WORKFLOW_INVALID_REQUEST\x10\xd7\xb3\x01\x12\x1d\n\x17WORKFLOW_MODIFY_SUCCESS\x10\x86\xad\x01\x12\x1d\n\x17WORKFLOW_MODIFY_PENDING\x10\x87\xad\x01\x12\x1c\n\x16WORKFLOW_MODIFY_FAILED\x10\x88\xad\x01\x12\x1d\n\x17WORKFLOW_REINDEX_FAILED\x10\x89\xad\x01\x12\x1c\n\x16\x43ONCEPT_MODIFY_SUCCESS\x10\xee\xb4\x01\x12\x1c\n\x16\x43ONCEPT_MODIFY_PENDING\x10\xef\xb4\x01\x12\x1b\n\x15\x43ONCEPT_MODIFY_FAILED\x10\xf0\xb4\x01\x12\x18\n\x12\x41NNOTATION_SUCCESS\x10\xd6\xbc\x01\x12\x18\n\x12\x41NNOTATION_PENDING\x10\xd7\xbc\x01\x12\x17\n\x11\x41NNOTATION_FAILED\x10\xd8\xbc\x01\x12\x1f\n\x19\x41NNOTATION_UNKNOWN_STATUS\x10\xda\xbc\x01\x12!\n\x1b\x41NNOTATION_INVALID_ARGUMENT\x10\xdb\xbc\x01\x12\"\n\x1c\x41NNOTATION_PERMISSION_DENIED\x10\xdc\xbc\x01\x12 \n\x1a\x41NNOTATION_AWAITING_REVIEW\x10\xdd\xbc\x01\x12*\n$ANNOTATION_AWAITING_CONSENSUS_REVIEW\x10\xdf\xbc\x01\x12\x1e\n\x18\x41NNOTATION_REVIEW_DENIED\x10\xde\xbc\x01\x12\x1f\n\x19\x41NNOTATION_MODIFY_SUCCESS\x10\xba\xbd\x01\x12\x1f\n\x19\x41NNOTATION_MODIFY_PENDING\x10\xbb\xbd\x01\x12\x1e\n\x18\x41NNOTATION_MODIFY_FAILED\x10\xbc\xbd\x01\x12&\n METADATA_INVALID_PATCH_ARGUMENTS\x10\xc4\xc2\x01\x12\x1c\n\x16METADATA_PARSING_ISSUE\x10\xc5\xc2\x01\x12!\n\x1bMETADATA_MANIPULATION_ISSUE\x10\xc6\xc2\x01\x12\x1c\n\x16TRAINER_JOB_STATE_NONE\x10\xa8\xc3\x01\x12\x1e\n\x18TRAINER_JOB_STATE_QUEUED\x10\xa9\xc3\x01\x12\x1f\n\x19TRAINER_JOB_STATE_RUNNING\x10\xaa\xc3\x01\x12 \n\x1aTRAINER_JOB_STATE_COMPLETE\x10\xab\xc3\x01\x12\x1d\n\x17TRAINER_JOB_STATE_ERROR\x10\xac\xc3\x01\x12\x17\n\x11\x44\x41TA_DUMP_SUCCESS\x10\xbe\xc4\x01\x12\x17\n\x11\x44\x41TA_DUMP_PENDING\x10\xbf\xc4\x01\x12\x16\n\x10\x44\x41TA_DUMP_FAILED\x10\xc0\xc4\x01\x12\x1b\n\x15\x44\x41TA_DUMP_IN_PROGRESS\x10\xc1\xc4\x01\x12\x1b\n\x11\x44\x41TA_DUMP_NO_DATA\x10\xc2\xc4\x01\x1a\x02\x08\x01\x12 \n\x1a\x44\x41TA_DUMP_UNEXPECTED_ERROR\x10\xc3\xc4\x01\x12\x1e\n\x18\x44\x41TA_DUMP_EXPORT_SUCCESS\x10\xd2\xc4\x01\x12\x1e\n\x18\x44\x41TA_DUMP_EXPORT_PENDING\x10\xd3\xc4\x01\x12\x1d\n\x17\x44\x41TA_DUMP_EXPORT_FAILED\x10\xd4\xc4\x01\x12\"\n\x1c\x44\x41TA_DUMP_EXPORT_IN_PROGRESS\x10\xd5\xc4\x01\x12\'\n!DATA_DUMP_EXPORT_UNEXPECTED_ERROR\x10\xd6\xc4\x01\x12\x1d\n\x17\x41PP_DUPLICATION_SUCCESS\x10\xf0\xc4\x01\x12\x1c\n\x16\x41PP_DUPLICATION_FAILED\x10\xf1\xc4\x01\x12\x1d\n\x17\x41PP_DUPLICATION_PENDING\x10\xf2\xc4\x01\x12!\n\x1b\x41PP_DUPLICATION_IN_PROGRESS\x10\xf3\xc4\x01\x12%\n\x1f\x41PP_DUPLICATION_INVALID_REQUEST\x10\xf4\xc4\x01\x12\x1b\n\x15MODULE_DOES_NOT_EXIST\x10\xd4\xc5\x01\x12\x1e\n\x18MODULE_PERMISSION_DENIED\x10\xd5\xc5\x01\x12\x1d\n\x17MODULE_INVALID_ARGUMENT\x10\xd6\xc5\x01\x12\x1c\n\x16MODULE_INVALID_REQUEST\x10\xd7\xc5\x01\x12\x1c\n\x16\x42ULK_OPERATION_SUCCESS\x10\xb8\xc6\x01\x12\x1b\n\x15\x42ULK_OPERATION_FAILED\x10\xb9\xc6\x01\x12\x1c\n\x16\x42ULK_OPERATION_PENDING\x10\xba\xc6\x01\x12 \n\x1a\x42ULK_OPERATION_IN_PROGRESS\x10\xbb\xc6\x01\x12$\n\x1e\x42ULK_OPERATION_INVALID_REQUEST\x10\xbc\xc6\x01\x12\x1e\n\x18\x42ULK_OPERATION_CANCELLED\x10\xbd\xc6\x01\x12%\n\x1f\x42ULK_OPERATION_UNEXPECTED_ERROR\x10\xbe\xc6\x01\x12\x1c\n\x16INPUT_DOWNLOAD_SUCCESS\x10\xb0\xea\x01\x12\x1c\n\x16INPUT_DOWNLOAD_PENDING\x10\xb1\xea\x01\x12\x1b\n\x15INPUT_DOWNLOAD_FAILED\x10\xb2\xea\x01\x12 \n\x1aINPUT_DOWNLOAD_IN_PROGRESS\x10\xb3\xea\x01\x12 \n\x1aINPUT_STATUS_UPDATE_FAILED\x10\xb4\xea\x01\x12\x19\n\x13INPUT_DELETE_FAILED\x10\xb5\xea\x01\x12\x15\n\x0fINPUT_DUPLICATE\x10\x94\xeb\x01\x12\x1e\n\x18INPUT_UNSUPPORTED_FORMAT\x10\x95\xeb\x01\x12\x1a\n\x14INPUT_DOES_NOT_EXIST\x10\x96\xeb\x01\x12\x1d\n\x17INPUT_PERMISSION_DENIED\x10\x97\xeb\x01\x12\x1c\n\x16INPUT_INVALID_ARGUMENT\x10\x98\xeb\x01\x12\x16\n\x10INPUT_OVER_LIMIT\x10\x99\xeb\x01\x12\x17\n\x11INPUT_INVALID_URL\x10\x9a\xeb\x01\x12\x1a\n\x14INPUT_MODIFY_SUCCESS\x10\xf8\xeb\x01\x12\x1a\n\x14INPUT_MODIFY_PENDING\x10\xf9\xeb\x01\x12\x19\n\x13INPUT_MODIFY_FAILED\x10\xfb\xeb\x01\x12\x1f\n\x19INPUT_STORAGE_HOST_FAILED\x10\x82\xec\x01\x12\x1d\n\x17\x41LL_INPUT_INVALID_BYTES\x10\xdc\xec\x01\x12\x1b\n\x15INPUT_CLUSTER_SUCCESS\x10\xc0\xed\x01\x12\x1b\n\x15INPUT_CLUSTER_PENDING\x10\xc1\xed\x01\x12\x1a\n\x14INPUT_CLUSTER_FAILED\x10\xc2\xed\x01\x12\x1f\n\x19INPUT_CLUSTER_IN_PROGRESS\x10\xc3\xed\x01\x12\x1b\n\x15INPUT_REINDEX_SUCCESS\x10\xa4\xee\x01\x12\x1b\n\x15INPUT_REINDEX_PENDING\x10\xa5\xee\x01\x12\x1a\n\x14INPUT_REINDEX_FAILED\x10\xa6\xee\x01\x12\x1f\n\x19INPUT_REINDEX_IN_PROGRESS\x10\xa7\xee\x01\x12\"\n\x1cINPUT_VIDEO_DOWNLOAD_SUCCESS\x10\x98\xf2\x01\x12\"\n\x1cINPUT_VIDEO_DOWNLOAD_PENDING\x10\x99\xf2\x01\x12!\n\x1bINPUT_VIDEO_DOWNLOAD_FAILED\x10\x9a\xf2\x01\x12\x1b\n\x15INPUT_VIDEO_DUPLICATE\x10\xfc\xf2\x01\x12$\n\x1eINPUT_VIDEO_UNSUPPORTED_FORMAT\x10\xfd\xf2\x01\x12 \n\x1aINPUT_VIDEO_DOES_NOT_EXIST\x10\xfe\xf2\x01\x12#\n\x1dINPUT_VIDEO_PERMISSION_DENIED\x10\xff\xf2\x01\x12\"\n\x1cINPUT_VIDEO_INVALID_ARGUMENT\x10\x80\xf3\x01\x12\x1c\n\x16INPUT_VIDEO_OVER_LIMIT\x10\x81\xf3\x01\x12\x1d\n\x17INPUT_VIDEO_INVALID_URL\x10\x82\xf3\x01\x12 \n\x1aINPUT_VIDEO_MODIFY_SUCCESS\x10\xe0\xf3\x01\x12 \n\x1aINPUT_VIDEO_MODIFY_PENDING\x10\xe1\xf3\x01\x12\x1f\n\x19INPUT_VIDEO_MODIFY_FAILED\x10\xe3\xf3\x01\x12%\n\x1fINPUT_VIDEO_STORAGE_HOST_FAILED\x10\xea\xf3\x01\x12$\n\x1e\x41LL_INPUT_VIDEOS_INVALID_BYTES\x10\xc4\xf4\x01\x12\x1d\n\x17INPUT_CONNECTION_FAILED\x10\xbc\xb8\x02\x12&\n REQUEST_DISABLED_FOR_MAINTENANCE\x10\xbd\xb8\x02\x12/\n%INPUT_WRITES_DISABLED_FOR_MAINTENANCE\x10\xbe\xb8\x02\x1a\x02\x08\x01\x12\x1b\n\x15INPUT_INVALID_REQUEST\x10\xbf\xb8\x02\x12\x1d\n\x17PREDICT_INVALID_REQUEST\x10\xc1\xb8\x02\x12\x1c\n\x16SEARCH_INVALID_REQUEST\x10\xc2\xb8\x02\x12\x1e\n\x18\x43ONCEPTS_INVALID_REQUEST\x10\xc3\xb8\x02\x12\x1b\n\x15STATS_INVALID_REQUEST\x10\xc4\xb8\x02\x12\x1c\n\x16\x44\x41TABASE_DUPLICATE_KEY\x10\xca\xb8\x02\x12 \n\x1a\x44\x41TABASE_STATEMENT_TIMEOUT\x10\xcb\xb8\x02\x12$\n\x1e\x44\x41TABASE_INVALID_ROWS_AFFECTED\x10\xcc\xb8\x02\x12 \n\x1a\x44\x41TABASE_DEADLOCK_DETECTED\x10\xcd\xb8\x02\x12\x18\n\x12\x44\x41TABASE_FAIL_TASK\x10\xce\xb8\x02\x12&\n DATABASE_FAIL_TO_GET_CONNECTIONS\x10\xcf\xb8\x02\x12\x1f\n\x19\x44\x41TABASE_TOO_MANY_CLIENTS\x10\xd0\xb8\x02\x12\"\n\x1c\x44\x41TABASE_CONSTRAINT_VIOLATED\x10\xd1\xb8\x02\x12\x17\n\x11\x44\x41TABASE_CANCELED\x10\xd5\xb8\x02\x12\x1f\n\x19\x41SYNC_WORKER_MULTI_ERRORS\x10\xd4\xb8\x02\x12\x1c\n\x16RPC_REQUEST_QUEUE_FULL\x10\xde\xb8\x02\x12\x1c\n\x16RPC_SERVER_UNAVAILABLE\x10\xdf\xb8\x02\x12\x19\n\x13RPC_REQUEST_TIMEOUT\x10\xe0\xb8\x02\x12#\n\x1dRPC_MAX_MESSAGE_SIZE_EXCEEDED\x10\xe1\xb8\x02\x12\x12\n\x0cRPC_CANCELED\x10\xe3\xb8\x02\x12\x18\n\x12RPC_UNKNOWN_METHOD\x10\xe4\xb8\x02\x12\x1e\n\x18REQUEST_CANCELED_BY_USER\x10\xe5\xb8\x02\x12\x1e\n\x18\x43LUSTER_INTERNAL_FAILURE\x10\xa0\xd0\x02\x12\x1f\n\x19\x45XTERNAL_CONNECTION_ERROR\x10\xe2\xb8\x02\x12\x1a\n\x14QUERY_INVALID_SYNTAX\x10\xf2\xb8\x02\x12\x16\n\x10QUEUE_CONN_ERROR\x10\xa8\xc0\x02\x12!\n\x1bQUEUE_CLOSE_REQUEST_TIMEOUT\x10\xaa\xc0\x02\x12\x17\n\x11QUEUE_CONN_CLOSED\x10\xab\xc0\x02\x12\x1f\n\x19QUEUE_PUBLISH_ACK_TIMEOUT\x10\xac\xc0\x02\x12\x19\n\x13QUEUE_PUBLISH_ERROR\x10\xad\xc0\x02\x12 \n\x1aQUEUE_SUBSCRIPTION_TIMEOUT\x10\xae\xc0\x02\x12\x1e\n\x18QUEUE_SUBSCRIPTION_ERROR\x10\xaf\xc0\x02\x12\x1e\n\x18QUEUE_MARSHALLING_FAILED\x10\xb0\xc0\x02\x12 \n\x1aQUEUE_UNMARSHALLING_FAILED\x10\xb1\xc0\x02\x12\'\n!QUEUE_MAX_MSG_REDELIVERY_EXCEEDED\x10\xb2\xc0\x02\x12\x17\n\x11QUEUE_ACK_FAILURE\x10\xb3\xc0\x02\x12\x13\n\rSQS_OVERLIMIT\x10\x8c\xc1\x02\x12 \n\x1aSQS_INVALID_RECEIPT_HANDLE\x10\x8d\xc1\x02\x12\x11\n\x0bSQS_UNKNOWN\x10\x8e\xc1\x02\x12\x1d\n\x17SEARCH_INTERNAL_FAILURE\x10\xf9\xcf\x02\x12\x1f\n\x19SEARCH_PROJECTION_FAILURE\x10\xfa\xcf\x02\x12\x1f\n\x19SEARCH_PREDICTION_FAILURE\x10\xfb\xcf\x02\x12\'\n!SEARCH_BY_NOT_FULLY_INDEXED_INPUT\x10\xfc\xcf\x02\x12 \n\x1aSAVED_SEARCH_MODIFY_FAILED\x10\xfd\xcf\x02\x12\x1f\n\x19SEARCH_COUNTS_UNAVAILABLE\x10\xfe\xcf\x02\x12\x17\n\x11\x45VALUATION_QUEUED\x10\xdc\xd0\x02\x12\x1c\n\x16\x45VALUATION_IN_PROGRESS\x10\xdd\xd0\x02\x12\x18\n\x12\x45VALUATION_SUCCESS\x10\xde\xd0\x02\x12(\n\"EVALUATION_FAILED_TO_RETRIEVE_DATA\x10\xdf\xd0\x02\x12!\n\x1b\x45VALUATION_INVALID_ARGUMENT\x10\xe0\xd0\x02\x12\x17\n\x11\x45VALUATION_FAILED\x10\xe1\xd0\x02\x12\x18\n\x12\x45VALUATION_PENDING\x10\xe2\xd0\x02\x12\x1a\n\x14\x45VALUATION_TIMED_OUT\x10\xe3\xd0\x02\x12!\n\x1b\x45VALUATION_UNEXPECTED_ERROR\x10\xe4\xd0\x02\x12\x16\n\x10\x45VALUATION_MIXED\x10\xe5\xd0\x02\x12\x18\n\x12STRIPE_EVENT_ERROR\x10\xe1\xd7\x02\x12\x10\n\nCACHE_MISS\x10\xc9\xdf\x02\x12&\n REDIS_SCRIPT_EXITED_WITH_FAILURE\x10\xca\xdf\x02\x12\x16\n\x10REDIS_STREAM_ERR\x10\xcb\xdf\x02\x12\x18\n\x12REDIS_NO_CONSUMERS\x10\xcc\xdf\x02\x12\x1a\n\x14REDIS_STREAM_BACKOFF\x10\xcd\xdf\x02\x12\x18\n\x12SIGNUP_EVENT_ERROR\x10\xb1\xe7\x02\x12\x14\n\x0eSIGNUP_FLAGGED\x10\xb2\xe7\x02\x12\x1a\n\x14\x46ILETYPE_UNSUPPORTED\x10\xb3\xe7\x02\x12\x1f\n\x19\x41PP_COUNT_INVALID_MESSAGE\x10\x99\xef\x02\x12\'\n!APP_COUNT_UPDATE_INCREMENT_FAILED\x10\x9a\xef\x02\x12\x1e\n\x18\x41PP_COUNT_REBUILD_FAILED\x10\x9b\xef\x02\x12 \n\x1a\x41PP_COUNT_INTERNAL_FAILURE\x10\x9c\xef\x02\x12\x17\n\x11MP_DOWNLOAD_ERROR\x10\xfd\xef\x02\x12\x1a\n\x14MP_RESOLVE_DNS_ERROR\x10\xfe\xef\x02\x12)\n#MP_DOWNLOAD_MAX_SIZE_EXCEEDED_ERROR\x10\xff\xef\x02\x12\x1b\n\x15MP_IMAGE_DECODE_ERROR\x10\x80\xf0\x02\x12\x19\n\x13MP_INVALID_ARGUMENT\x10\x81\xf0\x02\x12\x1f\n\x19MP_IMAGE_PROCESSING_ERROR\x10\x82\xf0\x02\x12\x19\n\x13\x44\x41TATIER_CONN_ERROR\x10\xe1\xf0\x02\x12\x17\n\x11USER_CONSENT_FACE\x10\xd1\x86\x03\x12\x14\n\x0eWORKER_MISSING\x10\xb8\x8e\x03\x12\x13\n\rWORKER_ACTIVE\x10\xb9\x8e\x03\x12\x15\n\x0fWORKER_INACTIVE\x10\xba\x8e\x03\x12\x17\n\x11\x43OLLECTOR_MISSING\x10\xa0\x96\x03\x12\x16\n\x10\x43OLLECTOR_ACTIVE\x10\xa1\x96\x03\x12\x18\n\x12\x43OLLECTOR_INACTIVE\x10\xa2\x96\x03\x12!\n\x1b\x43OLLECTOR_POST_INPUT_FAILED\x10\xa3\x96\x03\x12*\n$SSO_IDENTITY_PROVIDER_DOES_NOT_EXIST\x10\x89\x9e\x03\x12\x16\n\x10TASK_IN_PROGRESS\x10\xf1\xa5\x03\x12\x0f\n\tTASK_DONE\x10\xf2\xa5\x03\x12\x12\n\x0cTASK_WONT_DO\x10\xf3\xa5\x03\x12\"\n\x1cTASK_ADD_ANNOTATIONS_FAILURE\x10\xf5\xa5\x03\x12\x13\n\rTASK_CONFLICT\x10\xd4\xa6\x03\x12\x1a\n\x14TASK_NOT_IMPLEMENTED\x10\xd5\xa6\x03\x12\x12\n\x0cTASK_MISSING\x10\xd6\xa6\x03\x12\x19\n\x13LABEL_ORDER_PENDING\x10\xd9\xad\x03\x12\x1d\n\x17LABEL_ORDER_IN_PROGRESS\x10\xda\xad\x03\x12\x19\n\x13LABEL_ORDER_SUCCESS\x10\xdb\xad\x03\x12\x1a\n\x14LABEL_ORDER_CANCELED\x10\xdc\xad\x03\x12\x14\n\x0eLICENSE_ACTIVE\x10\xe0\xd4\x03\x12\x1c\n\x16LICENSE_DOES_NOT_EXIST\x10\xe1\xd4\x03\x12\x19\n\x13LICENSE_NEED_UPDATE\x10\xe2\xd4\x03\x12\x15\n\x0fLICENSE_EXPIRED\x10\xe3\xd4\x03\x12\x15\n\x0fLICENSE_REVOKED\x10\xe4\xd4\x03\x12\x15\n\x0fLICENSE_DELETED\x10\xe5\xd4\x03\x12\x1d\n\x17LICENSE_VOLUME_EXCEEDED\x10\xe6\xd4\x03\x12!\n\x1bPASSWORD_VALIDATION_SUCCESS\x10\xc8\xdc\x03\x12 \n\x1aPASSWORD_VALIDATION_FAILED\x10\xc9\xdc\x03\x12%\n\x1fPASSWORDPOLICY_INVALID_ARGUMENT\x10\xca\xdc\x03\x12\"\n\x1c\x46\x45\x41TUREFLAG_CONFIG_NOT_FOUND\x10\xb0\xe4\x03\x12\"\n\x1c\x46\x45\x41TUREFLAG_INVALID_ARGUMENT\x10\xb1\xe4\x03\x12\x19\n\x13\x46\x45\x41TUREFLAG_BLOCKED\x10\xb2\xe4\x03\x12\x19\n\x13MAINTENANCE_SUCCESS\x10\x98\xec\x03\x12\x18\n\x12MAINTENANCE_FAILED\x10\x99\xec\x03\x12\x1d\n\x17\x44\x41TASET_VERSION_PENDING\x10\x85\xf4\x03\x12!\n\x1b\x44\x41TASET_VERSION_IN_PROGRESS\x10\x8a\xf4\x03\x12\x1b\n\x15\x44\x41TASET_VERSION_READY\x10\x8f\xf4\x03\x12\x1d\n\x17\x44\x41TASET_VERSION_FAILURE\x10\x94\xf4\x03\x12&\n DATASET_VERSION_UNEXPECTED_ERROR\x10\x99\xf4\x03\x12\x1e\n\x18\x44\x41TASET_VERSION_CONFLICT\x10\x9e\xf4\x03\x12\x1b\n\x15\x44\x41TASET_INPUT_SUCCESS\x10\xe4\xf4\x03\x12\x1d\n\x17\x44\x41TASET_INPUT_DUPLICATE\x10\xe5\xf4\x03\x12$\n\x1e\x44\x41TASET_VERSION_EXPORT_SUCCESS\x10\xc8\xf5\x03\x12$\n\x1e\x44\x41TASET_VERSION_EXPORT_PENDING\x10\xc9\xf5\x03\x12#\n\x1d\x44\x41TASET_VERSION_EXPORT_FAILED\x10\xca\xf5\x03\x12(\n\"DATASET_VERSION_EXPORT_IN_PROGRESS\x10\xcb\xf5\x03\x12-\n\'DATASET_VERSION_EXPORT_UNEXPECTED_ERROR\x10\xcc\xf5\x03\x12\x10\n\nJOB_QUEUED\x10\x80\xf4\x03\x12\x11\n\x0bJOB_RUNNING\x10\x81\xf4\x03\x12\x13\n\rJOB_COMPLETED\x10\x82\xf4\x03\x12\x10\n\nJOB_FAILED\x10\x83\xf4\x03\x12\x13\n\rJOB_CANCELLED\x10\x84\xf4\x03\x12\x1a\n\x14JOB_UNEXPECTED_ERROR\x10\x86\xf4\x03\x12\x1c\n\x16\x41UTH_MISSING_IDP_ASSOC\x10\xe8\xfb\x03\x12\x19\n\x13LIST_OBJECTS_FAILED\x10\xd0\x83\x04\x12\x1c\n\x16\x41RCHIVE_EXTRACT_FAILED\x10\xb8\x8b\x04\x12\x18\n\x12UPLOAD_IN_PROGRESS\x10\xa0\x93\x04\x12\x11\n\x0bUPLOAD_DONE\x10\xa1\x93\x04\x12\x13\n\rUPLOAD_FAILED\x10\xa2\x93\x04\x12\x1d\n\x17UPLOAD_UNEXPECTED_ERROR\x10\xa3\x93\x04\x12\x14\n\x0eUPLOAD_EXPIRED\x10\xa4\x93\x04\x12\x1a\n\x14\x42ILLING_INVALID_INFO\x10\x88\x9b\x04\x12\x1b\n\x15INTERNAL_SERVER_ISSUE\x10\xd4\xfd\x05\x12\x1d\n\x17INTERNAL_FETCHING_ISSUE\x10\xd5\xfd\x05\x12\x1d\n\x17INTERNAL_DATABASE_ISSUE\x10\xd6\xfd\x05\x12!\n\x1bINTERNAL_UNEXPECTED_TIMEOUT\x10\xd9\xfd\x05\x12\x1c\n\x16INTERNAL_UNEXPECTED_V1\x10\xda\xfd\x05\x12\x1f\n\x19INTERNAL_UNEXPECTED_PANIC\x10\xdb\xfd\x05\x12\x1f\n\x19INTERNAL_UNEXPECTED_SPIRE\x10\xdc\xfd\x05\x12 \n\x1aINTERNAL_REDIS_UNAVAILABLE\x10\xdd\xfd\x05\x12!\n\x1bINTERNAL_RESOURCE_EXHAUSTED\x10\xde\xfd\x05\x12\"\n\x1cINTERNAL_REDIS_UNCATEGORIZED\x10\xdf\xfd\x05\x12 \n\x1aINTERNAL_AWS_UNCATEGORIZED\x10\xe0\xfd\x05\x12\"\n\x1cINTERNAL_AZURE_UNCATEGORIZED\x10\xe1\xfd\x05\x12\x18\n\x12\x43ONN_UNCATEGORIZED\x10\xb9\x85\x06\x12\x19\n\x13MODEL_UNCATEGORIZED\x10\xba\x85\x06\x12\x19\n\x13INPUT_UNCATEGORIZED\x10\xbb\x85\x06\x12\x1e\n\x18\x41NNOTATION_UNCATEGORIZED\x10\xbc\x85\x06\x12\x1b\n\x15\x42ILLING_UNCATEGORIZED\x10\xbd\x85\x06\x12\x1c\n\x16INTERNAL_UNCATEGORIZED\x10\xc1\x85\x06\x12\x11\n\x0b\x42\x41\x44_REQUEST\x10\xa0\xc2\x05\x12\x12\n\x0cSERVER_ERROR\x10\x84\xc3\x05\"\x08\x08\xbf\xc6\x01\x10\xbf\xc6\x01\"\x08\x08\xe8\x81\x02\x10\xe8\x81\x02\"\x08\x08\xe9\x81\x02\x10\xe9\x81\x02\"\x08\x08\xea\x81\x02\x10\xea\x81\x02\"\x08\x08\xcc\x82\x02\x10\xcc\x82\x02\"\x08\x08\xcd\x82\x02\x10\xcd\x82\x02\"\x08\x08\xce\x82\x02\x10\xce\x82\x02\"\x08\x08\xcf\x82\x02\x10\xcf\x82\x02\"\x08\x08\xd0\x82\x02\x10\xd0\x82\x02\"\x08\x08\xd1\x82\x02\x10\xd1\x82\x02\"\x08\x08\xd2\x82\x02\x10\xd2\x82\x02\"\x08\x08\xb0\x83\x02\x10\xb0\x83\x02\"\x08\x08\xb1\x83\x02\x10\xb1\x83\x02\"\x08\x08\xb3\x83\x02\x10\xb3\x83\x02\"\x08\x08\xba\x83\x02\x10\xba\x83\x02\"\x08\x08\xbb\xb8\x02\x10\xbb\xb8\x02\"\x08\x08\xd2\xb8\x02\x10\xd2\xb8\x02\"\x08\x08\xd3\xb8\x02\x10\xd3\xb8\x02\"\x08\x08\xf0\xc1\x02\x10\xf0\xc1\x02\"\x08\x08\xf1\xc1\x02\x10\xf1\xc1\x02\"\x08\x08\xf2\xc1\x02\x10\xf2\xc1\x02\"\x08\x08\xf3\xc1\x02\x10\xf3\xc1\x02\"\x08\x08\xf4\xc1\x02\x10\xf4\xc1\x02\"\x08\x08\x9c\xc7\x01\x10\x9c\xc7\x01\"\x08\x08\x9d\xc7\x01\x10\x9d\xc7\x01\"\x08\x08\x9e\xc7\x01\x10\x9e\xc7\x01\"\x08\x08\x9f\xc7\x01\x10\x9f\xc7\x01\"\x08\x08\xa1\xc7\x01\x10\xa1\xc7\x01\"\x08\x08\xa2\xc7\x01\x10\xa2\xc7\x01\x42g\n\x1c\x63om.clarifai.grpc.api.statusP\x01Z>github.com/Clarifai/clarifai-go-grpc/proto/clarifai/api/status\xa2\x02\x04\x43\x41IPb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n+proto/clarifai/api/status/status_code.proto\x12\x13\x63larifai.api.status*\xccS\n\nStatusCode\x12\x08\n\x04ZERO\x10\x00\x12\x0c\n\x07SUCCESS\x10\x90N\x12\x11\n\x0cMIXED_STATUS\x10\x9aN\x12\x0c\n\x07\x46\x41ILURE\x10\xa4N\x12\x0e\n\tTRY_AGAIN\x10\xaeN\x12\x14\n\x0fNOT_IMPLEMENTED\x10\xb8N\x12\n\n\x05MOVED\x10\xc2N\x12\x18\n\x13\x43ONN_ACCOUNT_ISSUES\x10\xf8U\x12\x1b\n\x12\x43ONN_TOKEN_INVALID\x10\xf9U\x1a\x02\x08\x01\x12\x1d\n\x18\x43ONN_CREDENTIALS_INVALID\x10\xfaU\x12\x1d\n\x18\x43ONN_EXCEED_HOURLY_LIMIT\x10\xfbU\x12\x1e\n\x19\x43ONN_EXCEED_MONTHLY_LIMIT\x10\xfcU\x12\x13\n\x0e\x43ONN_THROTTLED\x10\xfdU\x12\x18\n\x13\x43ONN_EXCEEDS_LIMITS\x10\xfeU\x12\x1d\n\x18\x43ONN_INSUFFICIENT_SCOPES\x10\xffU\x12\x15\n\x10\x43ONN_KEY_INVALID\x10\x80V\x12\x17\n\x12\x43ONN_KEY_NOT_FOUND\x10\x81V\x12\x1c\n\x17\x43ONN_BAD_REQUEST_FORMAT\x10\xdcV\x12\x18\n\x13\x43ONN_DOES_NOT_EXIST\x10\xddV\x12\x19\n\x14\x43ONN_INVALID_REQUEST\x10\xdeV\x12\x1c\n\x17\x43ONN_METHOD_NOT_ALLOWED\x10\xdfV\x12\x19\n\x14\x43ONN_NO_GDPR_CONSENT\x10\xe0V\x12\x1e\n\x19\x43ONN_AUTH_METHOD_DISABLED\x10\xc0W\x12\x13\n\rMODEL_TRAINED\x10\xec\xa4\x01\x12\x14\n\x0eMODEL_TRAINING\x10\xed\xa4\x01\x12\x15\n\x0fMODEL_UNTRAINED\x10\xee\xa4\x01\x12\x1f\n\x19MODEL_QUEUED_FOR_TRAINING\x10\xef\xa4\x01\x12\x15\n\x0fMODEL_UPLOADING\x10\xf0\xa4\x01\x12\x1c\n\x16MODEL_UPLOADING_FAILED\x10\xf1\xa4\x01\x12\x1b\n\x15MODEL_TRAINING_FAILED\x10\xf2\xa4\x01\x12\x1c\n\x16MODEL_TRAINING_NO_DATA\x10\xf6\xa4\x01\x12!\n\x1bMODEL_TRAINING_NO_POSITIVES\x10\xf7\xa4\x01\x12*\n$MODEL_TRAINING_ONE_VS_N_SINGLE_CLASS\x10\xf8\xa4\x01\x12\x1e\n\x18MODEL_TRAINING_TIMED_OUT\x10\xf9\xa4\x01\x12\"\n\x1cMODEL_TRAINING_WAITING_ERROR\x10\xfa\xa4\x01\x12\"\n\x1cMODEL_TRAINING_UNKNOWN_ERROR\x10\xfb\xa4\x01\x12&\n\x1cMODEL_TRAINING_MSG_REDELIVER\x10\xfc\xa4\x01\x1a\x02\x08\x01\x12&\n MODEL_TRAINING_INSUFFICIENT_DATA\x10\xfd\xa4\x01\x12#\n\x1dMODEL_TRAINING_INVALID_PARAMS\x10\xfe\xa4\x01\x12\x34\n.MODEL_TRAINING_INVALID_DATA_TOLERANCE_EXCEEDED\x10\xff\xa4\x01\x12\x1a\n\x14MODEL_MODIFY_SUCCESS\x10\x9e\xa5\x01\x12\x1a\n\x14MODEL_MODIFY_PENDING\x10\x9f\xa5\x01\x12\x19\n\x13MODEL_MODIFY_FAILED\x10\xa0\xa5\x01\x12\x1a\n\x14MODEL_DOES_NOT_EXIST\x10\xd0\xa5\x01\x12\x1d\n\x17MODEL_PERMISSION_DENIED\x10\xd1\xa5\x01\x12\x1c\n\x16MODEL_INVALID_ARGUMENT\x10\xd2\xa5\x01\x12\x1b\n\x15MODEL_INVALID_REQUEST\x10\xd3\xa5\x01\x12\x15\n\x0fMODEL_EVALUATED\x10\xb4\xa6\x01\x12\x16\n\x10MODEL_EVALUATING\x10\xb5\xa6\x01\x12\x19\n\x13MODEL_NOT_EVALUATED\x10\xb6\xa6\x01\x12!\n\x1bMODEL_QUEUED_FOR_EVALUATION\x10\xb7\xa6\x01\x12 \n\x1aMODEL_EVALUATION_TIMED_OUT\x10\xbe\xa6\x01\x12$\n\x1eMODEL_EVALUATION_WAITING_ERROR\x10\xbf\xa6\x01\x12$\n\x1eMODEL_EVALUATION_UNKNOWN_ERROR\x10\xc0\xa6\x01\x12\x1d\n\x17MODEL_PREDICTION_FAILED\x10\xc1\xa6\x01\x12(\n\x1eMODEL_EVALUATION_MSG_REDELIVER\x10\xc2\xa6\x01\x1a\x02\x08\x01\x12\"\n\x1cMODEL_EVALUATION_NEED_LABELS\x10\xc3\xa6\x01\x12\"\n\x1cMODEL_EVALUATION_NEED_INPUTS\x10\xc4\xa6\x01\x12\x1d\n\x17MODEL_EVALUATION_FAILED\x10\xc5\xa6\x01\x12\x1d\n\x17MODEL_DEPLOYMENT_FAILED\x10\xe6\xa6\x01\x12\x15\n\x0fMODEL_DEPLOYING\x10\xe7\xa6\x01\x12!\n\x1bMODEL_QUEUED_FOR_DEPLOYMENT\x10\xe8\xa6\x01\x12\x18\n\x12MODEL_NOT_DEPLOYED\x10\xe9\xa6\x01\x12&\n MODEL_REFERENCE_INVALID_ARGUMENT\x10\x98\xa7\x01\x12*\n$MODEL_EXAMPLE_INPUT_INVALID_ARGUMENT\x10\xac\xa7\x01\x12 \n\x1aWORKFLOW_NO_MATCHING_INPUT\x10\xf1\xab\x01\x12$\n\x1eWORKFLOW_REQUIRE_TRAINED_MODEL\x10\xf2\xab\x01\x12\x18\n\x12WORKFLOW_DUPLICATE\x10\xd4\xac\x01\x12!\n\x1bWORKFLOW_UNSUPPORTED_FORMAT\x10\xd5\xac\x01\x12\x1d\n\x17WORKFLOW_DOES_NOT_EXIST\x10\xd6\xac\x01\x12 \n\x1aWORKFLOW_PERMISSION_DENIED\x10\xd7\xac\x01\x12\x1f\n\x19WORKFLOW_INVALID_ARGUMENT\x10\xd8\xac\x01\x12\x1d\n\x17WORKFLOW_INVALID_RECIPE\x10\xd9\xac\x01\x12\x1f\n\x19WORKFLOW_INVALID_TEMPLATE\x10\xda\xac\x01\x12\x1c\n\x16WORKFLOW_INVALID_GRAPH\x10\xdb\xac\x01\x12\x1f\n\x19WORKFLOW_INTERNAL_FAILURE\x10\xdc\xac\x01\x12\x1e\n\x18WORKFLOW_INVALID_REQUEST\x10\xd7\xb3\x01\x12\x1d\n\x17WORKFLOW_MODIFY_SUCCESS\x10\x86\xad\x01\x12\x1d\n\x17WORKFLOW_MODIFY_PENDING\x10\x87\xad\x01\x12\x1c\n\x16WORKFLOW_MODIFY_FAILED\x10\x88\xad\x01\x12\x1d\n\x17WORKFLOW_REINDEX_FAILED\x10\x89\xad\x01\x12\x1c\n\x16\x43ONCEPT_MODIFY_SUCCESS\x10\xee\xb4\x01\x12\x1c\n\x16\x43ONCEPT_MODIFY_PENDING\x10\xef\xb4\x01\x12\x1b\n\x15\x43ONCEPT_MODIFY_FAILED\x10\xf0\xb4\x01\x12\x18\n\x12\x41NNOTATION_SUCCESS\x10\xd6\xbc\x01\x12\x18\n\x12\x41NNOTATION_PENDING\x10\xd7\xbc\x01\x12\x17\n\x11\x41NNOTATION_FAILED\x10\xd8\xbc\x01\x12\x1f\n\x19\x41NNOTATION_UNKNOWN_STATUS\x10\xda\xbc\x01\x12!\n\x1b\x41NNOTATION_INVALID_ARGUMENT\x10\xdb\xbc\x01\x12\"\n\x1c\x41NNOTATION_PERMISSION_DENIED\x10\xdc\xbc\x01\x12 \n\x1a\x41NNOTATION_AWAITING_REVIEW\x10\xdd\xbc\x01\x12*\n$ANNOTATION_AWAITING_CONSENSUS_REVIEW\x10\xdf\xbc\x01\x12\x1e\n\x18\x41NNOTATION_REVIEW_DENIED\x10\xde\xbc\x01\x12\x1f\n\x19\x41NNOTATION_MODIFY_SUCCESS\x10\xba\xbd\x01\x12\x1f\n\x19\x41NNOTATION_MODIFY_PENDING\x10\xbb\xbd\x01\x12\x1e\n\x18\x41NNOTATION_MODIFY_FAILED\x10\xbc\xbd\x01\x12&\n METADATA_INVALID_PATCH_ARGUMENTS\x10\xc4\xc2\x01\x12\x1c\n\x16METADATA_PARSING_ISSUE\x10\xc5\xc2\x01\x12!\n\x1bMETADATA_MANIPULATION_ISSUE\x10\xc6\xc2\x01\x12\x1c\n\x16TRAINER_JOB_STATE_NONE\x10\xa8\xc3\x01\x12\x1e\n\x18TRAINER_JOB_STATE_QUEUED\x10\xa9\xc3\x01\x12\x1f\n\x19TRAINER_JOB_STATE_RUNNING\x10\xaa\xc3\x01\x12 \n\x1aTRAINER_JOB_STATE_COMPLETE\x10\xab\xc3\x01\x12\x1d\n\x17TRAINER_JOB_STATE_ERROR\x10\xac\xc3\x01\x12\x17\n\x11\x44\x41TA_DUMP_SUCCESS\x10\xbe\xc4\x01\x12\x17\n\x11\x44\x41TA_DUMP_PENDING\x10\xbf\xc4\x01\x12\x16\n\x10\x44\x41TA_DUMP_FAILED\x10\xc0\xc4\x01\x12\x1b\n\x15\x44\x41TA_DUMP_IN_PROGRESS\x10\xc1\xc4\x01\x12\x1b\n\x11\x44\x41TA_DUMP_NO_DATA\x10\xc2\xc4\x01\x1a\x02\x08\x01\x12 \n\x1a\x44\x41TA_DUMP_UNEXPECTED_ERROR\x10\xc3\xc4\x01\x12\x1e\n\x18\x44\x41TA_DUMP_EXPORT_SUCCESS\x10\xd2\xc4\x01\x12\x1e\n\x18\x44\x41TA_DUMP_EXPORT_PENDING\x10\xd3\xc4\x01\x12\x1d\n\x17\x44\x41TA_DUMP_EXPORT_FAILED\x10\xd4\xc4\x01\x12\"\n\x1c\x44\x41TA_DUMP_EXPORT_IN_PROGRESS\x10\xd5\xc4\x01\x12\'\n!DATA_DUMP_EXPORT_UNEXPECTED_ERROR\x10\xd6\xc4\x01\x12\x1d\n\x17\x41PP_DUPLICATION_SUCCESS\x10\xf0\xc4\x01\x12\x1c\n\x16\x41PP_DUPLICATION_FAILED\x10\xf1\xc4\x01\x12\x1d\n\x17\x41PP_DUPLICATION_PENDING\x10\xf2\xc4\x01\x12!\n\x1b\x41PP_DUPLICATION_IN_PROGRESS\x10\xf3\xc4\x01\x12%\n\x1f\x41PP_DUPLICATION_INVALID_REQUEST\x10\xf4\xc4\x01\x12\x1b\n\x15MODULE_DOES_NOT_EXIST\x10\xd4\xc5\x01\x12\x1e\n\x18MODULE_PERMISSION_DENIED\x10\xd5\xc5\x01\x12\x1d\n\x17MODULE_INVALID_ARGUMENT\x10\xd6\xc5\x01\x12\x1c\n\x16MODULE_INVALID_REQUEST\x10\xd7\xc5\x01\x12\x1c\n\x16\x42ULK_OPERATION_SUCCESS\x10\xb8\xc6\x01\x12\x1b\n\x15\x42ULK_OPERATION_FAILED\x10\xb9\xc6\x01\x12\x1c\n\x16\x42ULK_OPERATION_PENDING\x10\xba\xc6\x01\x12 \n\x1a\x42ULK_OPERATION_IN_PROGRESS\x10\xbb\xc6\x01\x12$\n\x1e\x42ULK_OPERATION_INVALID_REQUEST\x10\xbc\xc6\x01\x12\x1e\n\x18\x42ULK_OPERATION_CANCELLED\x10\xbd\xc6\x01\x12%\n\x1f\x42ULK_OPERATION_UNEXPECTED_ERROR\x10\xbe\xc6\x01\x12\x1c\n\x16INPUT_DOWNLOAD_SUCCESS\x10\xb0\xea\x01\x12\x1c\n\x16INPUT_DOWNLOAD_PENDING\x10\xb1\xea\x01\x12\x1b\n\x15INPUT_DOWNLOAD_FAILED\x10\xb2\xea\x01\x12 \n\x1aINPUT_DOWNLOAD_IN_PROGRESS\x10\xb3\xea\x01\x12 \n\x1aINPUT_STATUS_UPDATE_FAILED\x10\xb4\xea\x01\x12\x19\n\x13INPUT_DELETE_FAILED\x10\xb5\xea\x01\x12\x15\n\x0fINPUT_DUPLICATE\x10\x94\xeb\x01\x12\x1e\n\x18INPUT_UNSUPPORTED_FORMAT\x10\x95\xeb\x01\x12\x1a\n\x14INPUT_DOES_NOT_EXIST\x10\x96\xeb\x01\x12\x1d\n\x17INPUT_PERMISSION_DENIED\x10\x97\xeb\x01\x12\x1c\n\x16INPUT_INVALID_ARGUMENT\x10\x98\xeb\x01\x12\x16\n\x10INPUT_OVER_LIMIT\x10\x99\xeb\x01\x12\x17\n\x11INPUT_INVALID_URL\x10\x9a\xeb\x01\x12\x1a\n\x14INPUT_MODIFY_SUCCESS\x10\xf8\xeb\x01\x12\x1a\n\x14INPUT_MODIFY_PENDING\x10\xf9\xeb\x01\x12\x19\n\x13INPUT_MODIFY_FAILED\x10\xfb\xeb\x01\x12\x1f\n\x19INPUT_STORAGE_HOST_FAILED\x10\x82\xec\x01\x12\x1d\n\x17\x41LL_INPUT_INVALID_BYTES\x10\xdc\xec\x01\x12\x1b\n\x15INPUT_CLUSTER_SUCCESS\x10\xc0\xed\x01\x12\x1b\n\x15INPUT_CLUSTER_PENDING\x10\xc1\xed\x01\x12\x1a\n\x14INPUT_CLUSTER_FAILED\x10\xc2\xed\x01\x12\x1f\n\x19INPUT_CLUSTER_IN_PROGRESS\x10\xc3\xed\x01\x12\x1b\n\x15INPUT_REINDEX_SUCCESS\x10\xa4\xee\x01\x12\x1b\n\x15INPUT_REINDEX_PENDING\x10\xa5\xee\x01\x12\x1a\n\x14INPUT_REINDEX_FAILED\x10\xa6\xee\x01\x12\x1f\n\x19INPUT_REINDEX_IN_PROGRESS\x10\xa7\xee\x01\x12\"\n\x1cINPUT_VIDEO_DOWNLOAD_SUCCESS\x10\x98\xf2\x01\x12\"\n\x1cINPUT_VIDEO_DOWNLOAD_PENDING\x10\x99\xf2\x01\x12!\n\x1bINPUT_VIDEO_DOWNLOAD_FAILED\x10\x9a\xf2\x01\x12\x1b\n\x15INPUT_VIDEO_DUPLICATE\x10\xfc\xf2\x01\x12$\n\x1eINPUT_VIDEO_UNSUPPORTED_FORMAT\x10\xfd\xf2\x01\x12 \n\x1aINPUT_VIDEO_DOES_NOT_EXIST\x10\xfe\xf2\x01\x12#\n\x1dINPUT_VIDEO_PERMISSION_DENIED\x10\xff\xf2\x01\x12\"\n\x1cINPUT_VIDEO_INVALID_ARGUMENT\x10\x80\xf3\x01\x12\x1c\n\x16INPUT_VIDEO_OVER_LIMIT\x10\x81\xf3\x01\x12\x1d\n\x17INPUT_VIDEO_INVALID_URL\x10\x82\xf3\x01\x12 \n\x1aINPUT_VIDEO_MODIFY_SUCCESS\x10\xe0\xf3\x01\x12 \n\x1aINPUT_VIDEO_MODIFY_PENDING\x10\xe1\xf3\x01\x12\x1f\n\x19INPUT_VIDEO_MODIFY_FAILED\x10\xe3\xf3\x01\x12%\n\x1fINPUT_VIDEO_STORAGE_HOST_FAILED\x10\xea\xf3\x01\x12$\n\x1e\x41LL_INPUT_VIDEOS_INVALID_BYTES\x10\xc4\xf4\x01\x12$\n\x1eINPUT_VIDEO_PROCESSING_SUCCESS\x10\xa8\xf5\x01\x12$\n\x1eINPUT_VIDEO_PROCESSING_PENDING\x10\xb2\xf5\x01\x12#\n\x1dINPUT_VIDEO_PROCESSING_FAILED\x10\xbc\xf5\x01\x12\'\n!INPUT_VIDEO_STORAGE_INCONSISTENCY\x10\xc6\xf5\x01\x12!\n\x1bINPUT_VIDEO_STORAGE_FAILURE\x10\xd0\xf5\x01\x12(\n\"INPUT_VIDEO_URL_GENERATION_FAILURE\x10\xda\xf5\x01\x12\x1d\n\x17INPUT_CONNECTION_FAILED\x10\xbc\xb8\x02\x12&\n REQUEST_DISABLED_FOR_MAINTENANCE\x10\xbd\xb8\x02\x12/\n%INPUT_WRITES_DISABLED_FOR_MAINTENANCE\x10\xbe\xb8\x02\x1a\x02\x08\x01\x12\x1b\n\x15INPUT_INVALID_REQUEST\x10\xbf\xb8\x02\x12\x1d\n\x17PREDICT_INVALID_REQUEST\x10\xc1\xb8\x02\x12\x1c\n\x16SEARCH_INVALID_REQUEST\x10\xc2\xb8\x02\x12\x1e\n\x18\x43ONCEPTS_INVALID_REQUEST\x10\xc3\xb8\x02\x12\x1b\n\x15STATS_INVALID_REQUEST\x10\xc4\xb8\x02\x12\x1c\n\x16\x44\x41TABASE_DUPLICATE_KEY\x10\xca\xb8\x02\x12 \n\x1a\x44\x41TABASE_STATEMENT_TIMEOUT\x10\xcb\xb8\x02\x12$\n\x1e\x44\x41TABASE_INVALID_ROWS_AFFECTED\x10\xcc\xb8\x02\x12 \n\x1a\x44\x41TABASE_DEADLOCK_DETECTED\x10\xcd\xb8\x02\x12\x18\n\x12\x44\x41TABASE_FAIL_TASK\x10\xce\xb8\x02\x12&\n DATABASE_FAIL_TO_GET_CONNECTIONS\x10\xcf\xb8\x02\x12\x1f\n\x19\x44\x41TABASE_TOO_MANY_CLIENTS\x10\xd0\xb8\x02\x12\"\n\x1c\x44\x41TABASE_CONSTRAINT_VIOLATED\x10\xd1\xb8\x02\x12\x17\n\x11\x44\x41TABASE_CANCELED\x10\xd5\xb8\x02\x12\x1f\n\x19\x41SYNC_WORKER_MULTI_ERRORS\x10\xd4\xb8\x02\x12\x1c\n\x16RPC_REQUEST_QUEUE_FULL\x10\xde\xb8\x02\x12\x1c\n\x16RPC_SERVER_UNAVAILABLE\x10\xdf\xb8\x02\x12\x19\n\x13RPC_REQUEST_TIMEOUT\x10\xe0\xb8\x02\x12#\n\x1dRPC_MAX_MESSAGE_SIZE_EXCEEDED\x10\xe1\xb8\x02\x12\x12\n\x0cRPC_CANCELED\x10\xe3\xb8\x02\x12\x18\n\x12RPC_UNKNOWN_METHOD\x10\xe4\xb8\x02\x12\x1e\n\x18REQUEST_CANCELED_BY_USER\x10\xe5\xb8\x02\x12\x1e\n\x18\x43LUSTER_INTERNAL_FAILURE\x10\xa0\xd0\x02\x12\x1f\n\x19\x45XTERNAL_CONNECTION_ERROR\x10\xe2\xb8\x02\x12\x1a\n\x14QUERY_INVALID_SYNTAX\x10\xf2\xb8\x02\x12\x16\n\x10QUEUE_CONN_ERROR\x10\xa8\xc0\x02\x12!\n\x1bQUEUE_CLOSE_REQUEST_TIMEOUT\x10\xaa\xc0\x02\x12\x17\n\x11QUEUE_CONN_CLOSED\x10\xab\xc0\x02\x12\x1f\n\x19QUEUE_PUBLISH_ACK_TIMEOUT\x10\xac\xc0\x02\x12\x19\n\x13QUEUE_PUBLISH_ERROR\x10\xad\xc0\x02\x12 \n\x1aQUEUE_SUBSCRIPTION_TIMEOUT\x10\xae\xc0\x02\x12\x1e\n\x18QUEUE_SUBSCRIPTION_ERROR\x10\xaf\xc0\x02\x12\x1e\n\x18QUEUE_MARSHALLING_FAILED\x10\xb0\xc0\x02\x12 \n\x1aQUEUE_UNMARSHALLING_FAILED\x10\xb1\xc0\x02\x12\'\n!QUEUE_MAX_MSG_REDELIVERY_EXCEEDED\x10\xb2\xc0\x02\x12\x17\n\x11QUEUE_ACK_FAILURE\x10\xb3\xc0\x02\x12\x13\n\rSQS_OVERLIMIT\x10\x8c\xc1\x02\x12 \n\x1aSQS_INVALID_RECEIPT_HANDLE\x10\x8d\xc1\x02\x12\x11\n\x0bSQS_UNKNOWN\x10\x8e\xc1\x02\x12\x1d\n\x17SEARCH_INTERNAL_FAILURE\x10\xf9\xcf\x02\x12\x1f\n\x19SEARCH_PROJECTION_FAILURE\x10\xfa\xcf\x02\x12\x1f\n\x19SEARCH_PREDICTION_FAILURE\x10\xfb\xcf\x02\x12\'\n!SEARCH_BY_NOT_FULLY_INDEXED_INPUT\x10\xfc\xcf\x02\x12 \n\x1aSAVED_SEARCH_MODIFY_FAILED\x10\xfd\xcf\x02\x12\x1f\n\x19SEARCH_COUNTS_UNAVAILABLE\x10\xfe\xcf\x02\x12\x17\n\x11\x45VALUATION_QUEUED\x10\xdc\xd0\x02\x12\x1c\n\x16\x45VALUATION_IN_PROGRESS\x10\xdd\xd0\x02\x12\x18\n\x12\x45VALUATION_SUCCESS\x10\xde\xd0\x02\x12(\n\"EVALUATION_FAILED_TO_RETRIEVE_DATA\x10\xdf\xd0\x02\x12!\n\x1b\x45VALUATION_INVALID_ARGUMENT\x10\xe0\xd0\x02\x12\x17\n\x11\x45VALUATION_FAILED\x10\xe1\xd0\x02\x12\x18\n\x12\x45VALUATION_PENDING\x10\xe2\xd0\x02\x12\x1a\n\x14\x45VALUATION_TIMED_OUT\x10\xe3\xd0\x02\x12!\n\x1b\x45VALUATION_UNEXPECTED_ERROR\x10\xe4\xd0\x02\x12\x16\n\x10\x45VALUATION_MIXED\x10\xe5\xd0\x02\x12\x18\n\x12STRIPE_EVENT_ERROR\x10\xe1\xd7\x02\x12\x10\n\nCACHE_MISS\x10\xc9\xdf\x02\x12&\n REDIS_SCRIPT_EXITED_WITH_FAILURE\x10\xca\xdf\x02\x12\x16\n\x10REDIS_STREAM_ERR\x10\xcb\xdf\x02\x12\x18\n\x12REDIS_NO_CONSUMERS\x10\xcc\xdf\x02\x12\x1a\n\x14REDIS_STREAM_BACKOFF\x10\xcd\xdf\x02\x12\x18\n\x12SIGNUP_EVENT_ERROR\x10\xb1\xe7\x02\x12\x14\n\x0eSIGNUP_FLAGGED\x10\xb2\xe7\x02\x12\x1a\n\x14\x46ILETYPE_UNSUPPORTED\x10\xb3\xe7\x02\x12\x1f\n\x19\x41PP_COUNT_INVALID_MESSAGE\x10\x99\xef\x02\x12\'\n!APP_COUNT_UPDATE_INCREMENT_FAILED\x10\x9a\xef\x02\x12\x1e\n\x18\x41PP_COUNT_REBUILD_FAILED\x10\x9b\xef\x02\x12 \n\x1a\x41PP_COUNT_INTERNAL_FAILURE\x10\x9c\xef\x02\x12\x17\n\x11MP_DOWNLOAD_ERROR\x10\xfd\xef\x02\x12\x1a\n\x14MP_RESOLVE_DNS_ERROR\x10\xfe\xef\x02\x12)\n#MP_DOWNLOAD_MAX_SIZE_EXCEEDED_ERROR\x10\xff\xef\x02\x12\x1b\n\x15MP_IMAGE_DECODE_ERROR\x10\x80\xf0\x02\x12\x19\n\x13MP_INVALID_ARGUMENT\x10\x81\xf0\x02\x12\x1f\n\x19MP_IMAGE_PROCESSING_ERROR\x10\x82\xf0\x02\x12\x19\n\x13\x44\x41TATIER_CONN_ERROR\x10\xe1\xf0\x02\x12\x17\n\x11USER_CONSENT_FACE\x10\xd1\x86\x03\x12\x14\n\x0eWORKER_MISSING\x10\xb8\x8e\x03\x12\x13\n\rWORKER_ACTIVE\x10\xb9\x8e\x03\x12\x15\n\x0fWORKER_INACTIVE\x10\xba\x8e\x03\x12\x17\n\x11\x43OLLECTOR_MISSING\x10\xa0\x96\x03\x12\x16\n\x10\x43OLLECTOR_ACTIVE\x10\xa1\x96\x03\x12\x18\n\x12\x43OLLECTOR_INACTIVE\x10\xa2\x96\x03\x12!\n\x1b\x43OLLECTOR_POST_INPUT_FAILED\x10\xa3\x96\x03\x12*\n$SSO_IDENTITY_PROVIDER_DOES_NOT_EXIST\x10\x89\x9e\x03\x12\x16\n\x10TASK_IN_PROGRESS\x10\xf1\xa5\x03\x12\x0f\n\tTASK_DONE\x10\xf2\xa5\x03\x12\x12\n\x0cTASK_WONT_DO\x10\xf3\xa5\x03\x12\"\n\x1cTASK_ADD_ANNOTATIONS_FAILURE\x10\xf5\xa5\x03\x12\x13\n\rTASK_CONFLICT\x10\xd4\xa6\x03\x12\x1a\n\x14TASK_NOT_IMPLEMENTED\x10\xd5\xa6\x03\x12\x12\n\x0cTASK_MISSING\x10\xd6\xa6\x03\x12\x19\n\x13LABEL_ORDER_PENDING\x10\xd9\xad\x03\x12\x1d\n\x17LABEL_ORDER_IN_PROGRESS\x10\xda\xad\x03\x12\x19\n\x13LABEL_ORDER_SUCCESS\x10\xdb\xad\x03\x12\x1a\n\x14LABEL_ORDER_CANCELED\x10\xdc\xad\x03\x12\x14\n\x0eLICENSE_ACTIVE\x10\xe0\xd4\x03\x12\x1c\n\x16LICENSE_DOES_NOT_EXIST\x10\xe1\xd4\x03\x12\x19\n\x13LICENSE_NEED_UPDATE\x10\xe2\xd4\x03\x12\x15\n\x0fLICENSE_EXPIRED\x10\xe3\xd4\x03\x12\x15\n\x0fLICENSE_REVOKED\x10\xe4\xd4\x03\x12\x15\n\x0fLICENSE_DELETED\x10\xe5\xd4\x03\x12\x1d\n\x17LICENSE_VOLUME_EXCEEDED\x10\xe6\xd4\x03\x12!\n\x1bPASSWORD_VALIDATION_SUCCESS\x10\xc8\xdc\x03\x12 \n\x1aPASSWORD_VALIDATION_FAILED\x10\xc9\xdc\x03\x12%\n\x1fPASSWORDPOLICY_INVALID_ARGUMENT\x10\xca\xdc\x03\x12\"\n\x1c\x46\x45\x41TUREFLAG_CONFIG_NOT_FOUND\x10\xb0\xe4\x03\x12\"\n\x1c\x46\x45\x41TUREFLAG_INVALID_ARGUMENT\x10\xb1\xe4\x03\x12\x19\n\x13\x46\x45\x41TUREFLAG_BLOCKED\x10\xb2\xe4\x03\x12\x19\n\x13MAINTENANCE_SUCCESS\x10\x98\xec\x03\x12\x18\n\x12MAINTENANCE_FAILED\x10\x99\xec\x03\x12\x1d\n\x17\x44\x41TASET_VERSION_PENDING\x10\x85\xf4\x03\x12!\n\x1b\x44\x41TASET_VERSION_IN_PROGRESS\x10\x8a\xf4\x03\x12\x1b\n\x15\x44\x41TASET_VERSION_READY\x10\x8f\xf4\x03\x12\x1d\n\x17\x44\x41TASET_VERSION_FAILURE\x10\x94\xf4\x03\x12&\n DATASET_VERSION_UNEXPECTED_ERROR\x10\x99\xf4\x03\x12\x1e\n\x18\x44\x41TASET_VERSION_CONFLICT\x10\x9e\xf4\x03\x12\x1b\n\x15\x44\x41TASET_INPUT_SUCCESS\x10\xe4\xf4\x03\x12\x1d\n\x17\x44\x41TASET_INPUT_DUPLICATE\x10\xe5\xf4\x03\x12$\n\x1e\x44\x41TASET_VERSION_EXPORT_SUCCESS\x10\xc8\xf5\x03\x12$\n\x1e\x44\x41TASET_VERSION_EXPORT_PENDING\x10\xc9\xf5\x03\x12#\n\x1d\x44\x41TASET_VERSION_EXPORT_FAILED\x10\xca\xf5\x03\x12(\n\"DATASET_VERSION_EXPORT_IN_PROGRESS\x10\xcb\xf5\x03\x12-\n\'DATASET_VERSION_EXPORT_UNEXPECTED_ERROR\x10\xcc\xf5\x03\x12\x10\n\nJOB_QUEUED\x10\x80\xf4\x03\x12\x11\n\x0bJOB_RUNNING\x10\x81\xf4\x03\x12\x13\n\rJOB_COMPLETED\x10\x82\xf4\x03\x12\x10\n\nJOB_FAILED\x10\x83\xf4\x03\x12\x13\n\rJOB_CANCELLED\x10\x84\xf4\x03\x12\x1a\n\x14JOB_UNEXPECTED_ERROR\x10\x86\xf4\x03\x12\x12\n\x0cJOB_CONFLICT\x10\x87\xf4\x03\x12\x1c\n\x16\x41UTH_MISSING_IDP_ASSOC\x10\xe8\xfb\x03\x12\x19\n\x13LIST_OBJECTS_FAILED\x10\xd0\x83\x04\x12\x1c\n\x16\x41RCHIVE_EXTRACT_FAILED\x10\xb8\x8b\x04\x12\x18\n\x12UPLOAD_IN_PROGRESS\x10\xa0\x93\x04\x12\x11\n\x0bUPLOAD_DONE\x10\xa1\x93\x04\x12\x13\n\rUPLOAD_FAILED\x10\xa2\x93\x04\x12\x1d\n\x17UPLOAD_UNEXPECTED_ERROR\x10\xa3\x93\x04\x12\x14\n\x0eUPLOAD_EXPIRED\x10\xa4\x93\x04\x12\x15\n\x0fUPLOAD_CANCELED\x10\xa5\x93\x04\x12\x15\n\x0fUPLOAD_CONFLICT\x10\xa6\x93\x04\x12\x1a\n\x14\x42ILLING_INVALID_INFO\x10\x88\x9b\x04\x12\x1b\n\x15INTERNAL_SERVER_ISSUE\x10\xd4\xfd\x05\x12\x1d\n\x17INTERNAL_FETCHING_ISSUE\x10\xd5\xfd\x05\x12\x1d\n\x17INTERNAL_DATABASE_ISSUE\x10\xd6\xfd\x05\x12!\n\x1bINTERNAL_UNEXPECTED_TIMEOUT\x10\xd9\xfd\x05\x12\x1c\n\x16INTERNAL_UNEXPECTED_V1\x10\xda\xfd\x05\x12\x1f\n\x19INTERNAL_UNEXPECTED_PANIC\x10\xdb\xfd\x05\x12\x1f\n\x19INTERNAL_UNEXPECTED_SPIRE\x10\xdc\xfd\x05\x12 \n\x1aINTERNAL_REDIS_UNAVAILABLE\x10\xdd\xfd\x05\x12!\n\x1bINTERNAL_RESOURCE_EXHAUSTED\x10\xde\xfd\x05\x12\"\n\x1cINTERNAL_REDIS_UNCATEGORIZED\x10\xdf\xfd\x05\x12 \n\x1aINTERNAL_AWS_UNCATEGORIZED\x10\xe0\xfd\x05\x12\"\n\x1cINTERNAL_AZURE_UNCATEGORIZED\x10\xe1\xfd\x05\x12\x18\n\x12\x43ONN_UNCATEGORIZED\x10\xb9\x85\x06\x12\x19\n\x13MODEL_UNCATEGORIZED\x10\xba\x85\x06\x12\x19\n\x13INPUT_UNCATEGORIZED\x10\xbb\x85\x06\x12\x1e\n\x18\x41NNOTATION_UNCATEGORIZED\x10\xbc\x85\x06\x12\x1b\n\x15\x42ILLING_UNCATEGORIZED\x10\xbd\x85\x06\x12\x1c\n\x16INTERNAL_UNCATEGORIZED\x10\xc1\x85\x06\x12\x11\n\x0b\x42\x41\x44_REQUEST\x10\xa0\xc2\x05\x12\x12\n\x0cSERVER_ERROR\x10\x84\xc3\x05\"\x08\x08\xbf\xc6\x01\x10\xbf\xc6\x01\"\x08\x08\xe8\x81\x02\x10\xe8\x81\x02\"\x08\x08\xe9\x81\x02\x10\xe9\x81\x02\"\x08\x08\xea\x81\x02\x10\xea\x81\x02\"\x08\x08\xcc\x82\x02\x10\xcc\x82\x02\"\x08\x08\xcd\x82\x02\x10\xcd\x82\x02\"\x08\x08\xce\x82\x02\x10\xce\x82\x02\"\x08\x08\xcf\x82\x02\x10\xcf\x82\x02\"\x08\x08\xd0\x82\x02\x10\xd0\x82\x02\"\x08\x08\xd1\x82\x02\x10\xd1\x82\x02\"\x08\x08\xd2\x82\x02\x10\xd2\x82\x02\"\x08\x08\xb0\x83\x02\x10\xb0\x83\x02\"\x08\x08\xb1\x83\x02\x10\xb1\x83\x02\"\x08\x08\xb3\x83\x02\x10\xb3\x83\x02\"\x08\x08\xba\x83\x02\x10\xba\x83\x02\"\x08\x08\xbb\xb8\x02\x10\xbb\xb8\x02\"\x08\x08\xd2\xb8\x02\x10\xd2\xb8\x02\"\x08\x08\xd3\xb8\x02\x10\xd3\xb8\x02\"\x08\x08\xf0\xc1\x02\x10\xf0\xc1\x02\"\x08\x08\xf1\xc1\x02\x10\xf1\xc1\x02\"\x08\x08\xf2\xc1\x02\x10\xf2\xc1\x02\"\x08\x08\xf3\xc1\x02\x10\xf3\xc1\x02\"\x08\x08\xf4\xc1\x02\x10\xf4\xc1\x02\"\x08\x08\x9c\xc7\x01\x10\x9c\xc7\x01\"\x08\x08\x9d\xc7\x01\x10\x9d\xc7\x01\"\x08\x08\x9e\xc7\x01\x10\x9e\xc7\x01\"\x08\x08\x9f\xc7\x01\x10\x9f\xc7\x01\"\x08\x08\xa1\xc7\x01\x10\xa1\xc7\x01\"\x08\x08\xa2\xc7\x01\x10\xa2\xc7\x01\x42g\n\x1c\x63om.clarifai.grpc.api.statusP\x01Z>github.com/Clarifai/clarifai-go-grpc/proto/clarifai/api/status\xa2\x02\x04\x43\x41IPb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'proto.clarifai.api.status.status_code_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\034com.clarifai.grpc.api.statusP\001Z>github.com/Clarifai/clarifai-go-grpc/proto/clarifai/api/status\242\002\004CAIP'
@@ -28,9 +28,9 @@
   _STATUSCODE.values_by_name["MODEL_EVALUATION_MSG_REDELIVER"]._options = None
   _STATUSCODE.values_by_name["MODEL_EVALUATION_MSG_REDELIVER"]._serialized_options = b'\010\001'
   _STATUSCODE.values_by_name["DATA_DUMP_NO_DATA"]._options = None
   _STATUSCODE.values_by_name["DATA_DUMP_NO_DATA"]._serialized_options = b'\010\001'
   _STATUSCODE.values_by_name["INPUT_WRITES_DISABLED_FOR_MAINTENANCE"]._options = None
   _STATUSCODE.values_by_name["INPUT_WRITES_DISABLED_FOR_MAINTENANCE"]._serialized_options = b'\010\001'
   _STATUSCODE._serialized_start=69
-  _STATUSCODE._serialized_end=10472
+  _STATUSCODE._serialized_end=10769
 # @@protoc_insertion_point(module_scope)
```

### Comparing `clarifai-grpc-9.5.0/clarifai_grpc/grpc/api/status/status_code_pb2.pyi` & `clarifai-grpc-9.6.0/clarifai_grpc/grpc/api/status/status_code_pb2.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -267,14 +267,20 @@
     INPUT_VIDEO_OVER_LIMIT: _StatusCode.ValueType  # 31105
     INPUT_VIDEO_INVALID_URL: _StatusCode.ValueType  # 31106
     INPUT_VIDEO_MODIFY_SUCCESS: _StatusCode.ValueType  # 31200
     INPUT_VIDEO_MODIFY_PENDING: _StatusCode.ValueType  # 31201
     INPUT_VIDEO_MODIFY_FAILED: _StatusCode.ValueType  # 31203
     INPUT_VIDEO_STORAGE_HOST_FAILED: _StatusCode.ValueType  # 31210
     ALL_INPUT_VIDEOS_INVALID_BYTES: _StatusCode.ValueType  # 31300
+    INPUT_VIDEO_PROCESSING_SUCCESS: _StatusCode.ValueType  # 31400
+    INPUT_VIDEO_PROCESSING_PENDING: _StatusCode.ValueType  # 31410
+    INPUT_VIDEO_PROCESSING_FAILED: _StatusCode.ValueType  # 31420
+    INPUT_VIDEO_STORAGE_INCONSISTENCY: _StatusCode.ValueType  # 31430
+    INPUT_VIDEO_STORAGE_FAILURE: _StatusCode.ValueType  # 31440
+    INPUT_VIDEO_URL_GENERATION_FAILURE: _StatusCode.ValueType  # 31450
     INPUT_CONNECTION_FAILED: _StatusCode.ValueType  # 39996
     REQUEST_DISABLED_FOR_MAINTENANCE: _StatusCode.ValueType  # 39997
     INPUT_WRITES_DISABLED_FOR_MAINTENANCE: _StatusCode.ValueType  # 39998
     """deprecate this one. Use REQUEST_DISABLED_FOR_MAINTENANCE"""
     INPUT_INVALID_REQUEST: _StatusCode.ValueType  # 39999
     PREDICT_INVALID_REQUEST: _StatusCode.ValueType  # 40001
     """API formatting issues 4000x"""
@@ -450,26 +456,29 @@
     JOB_QUEUED: _StatusCode.ValueType  # 64000
     """Generic Job status codes"""
     JOB_RUNNING: _StatusCode.ValueType  # 64001
     JOB_COMPLETED: _StatusCode.ValueType  # 64002
     JOB_FAILED: _StatusCode.ValueType  # 64003
     JOB_CANCELLED: _StatusCode.ValueType  # 64004
     JOB_UNEXPECTED_ERROR: _StatusCode.ValueType  # 64006
+    JOB_CONFLICT: _StatusCode.ValueType  # 64007
     AUTH_MISSING_IDP_ASSOC: _StatusCode.ValueType  # 65000
     """auth issues
     TODO: Knowledge graph related 80xxx
     """
     LIST_OBJECTS_FAILED: _StatusCode.ValueType  # 66000
     ARCHIVE_EXTRACT_FAILED: _StatusCode.ValueType  # 67000
     UPLOAD_IN_PROGRESS: _StatusCode.ValueType  # 68000
     """Multipart uploading status codes"""
     UPLOAD_DONE: _StatusCode.ValueType  # 68001
     UPLOAD_FAILED: _StatusCode.ValueType  # 68002
     UPLOAD_UNEXPECTED_ERROR: _StatusCode.ValueType  # 68003
     UPLOAD_EXPIRED: _StatusCode.ValueType  # 68004
+    UPLOAD_CANCELED: _StatusCode.ValueType  # 68005
+    UPLOAD_CONFLICT: _StatusCode.ValueType  # 68006
     BILLING_INVALID_INFO: _StatusCode.ValueType  # 69000
     """Billing related issues: 69xxx"""
     INTERNAL_SERVER_ISSUE: _StatusCode.ValueType  # 98004
     """Internal issues: 98xxx"""
     INTERNAL_FETCHING_ISSUE: _StatusCode.ValueType  # 98005
     INTERNAL_DATABASE_ISSUE: _StatusCode.ValueType  # 98006
     INTERNAL_UNEXPECTED_TIMEOUT: _StatusCode.ValueType  # 98009
@@ -741,14 +750,20 @@
 INPUT_VIDEO_OVER_LIMIT: StatusCode.ValueType  # 31105
 INPUT_VIDEO_INVALID_URL: StatusCode.ValueType  # 31106
 INPUT_VIDEO_MODIFY_SUCCESS: StatusCode.ValueType  # 31200
 INPUT_VIDEO_MODIFY_PENDING: StatusCode.ValueType  # 31201
 INPUT_VIDEO_MODIFY_FAILED: StatusCode.ValueType  # 31203
 INPUT_VIDEO_STORAGE_HOST_FAILED: StatusCode.ValueType  # 31210
 ALL_INPUT_VIDEOS_INVALID_BYTES: StatusCode.ValueType  # 31300
+INPUT_VIDEO_PROCESSING_SUCCESS: StatusCode.ValueType  # 31400
+INPUT_VIDEO_PROCESSING_PENDING: StatusCode.ValueType  # 31410
+INPUT_VIDEO_PROCESSING_FAILED: StatusCode.ValueType  # 31420
+INPUT_VIDEO_STORAGE_INCONSISTENCY: StatusCode.ValueType  # 31430
+INPUT_VIDEO_STORAGE_FAILURE: StatusCode.ValueType  # 31440
+INPUT_VIDEO_URL_GENERATION_FAILURE: StatusCode.ValueType  # 31450
 INPUT_CONNECTION_FAILED: StatusCode.ValueType  # 39996
 REQUEST_DISABLED_FOR_MAINTENANCE: StatusCode.ValueType  # 39997
 INPUT_WRITES_DISABLED_FOR_MAINTENANCE: StatusCode.ValueType  # 39998
 """deprecate this one. Use REQUEST_DISABLED_FOR_MAINTENANCE"""
 INPUT_INVALID_REQUEST: StatusCode.ValueType  # 39999
 PREDICT_INVALID_REQUEST: StatusCode.ValueType  # 40001
 """API formatting issues 4000x"""
@@ -924,26 +939,29 @@
 JOB_QUEUED: StatusCode.ValueType  # 64000
 """Generic Job status codes"""
 JOB_RUNNING: StatusCode.ValueType  # 64001
 JOB_COMPLETED: StatusCode.ValueType  # 64002
 JOB_FAILED: StatusCode.ValueType  # 64003
 JOB_CANCELLED: StatusCode.ValueType  # 64004
 JOB_UNEXPECTED_ERROR: StatusCode.ValueType  # 64006
+JOB_CONFLICT: StatusCode.ValueType  # 64007
 AUTH_MISSING_IDP_ASSOC: StatusCode.ValueType  # 65000
 """auth issues
 TODO: Knowledge graph related 80xxx
 """
 LIST_OBJECTS_FAILED: StatusCode.ValueType  # 66000
 ARCHIVE_EXTRACT_FAILED: StatusCode.ValueType  # 67000
 UPLOAD_IN_PROGRESS: StatusCode.ValueType  # 68000
 """Multipart uploading status codes"""
 UPLOAD_DONE: StatusCode.ValueType  # 68001
 UPLOAD_FAILED: StatusCode.ValueType  # 68002
 UPLOAD_UNEXPECTED_ERROR: StatusCode.ValueType  # 68003
 UPLOAD_EXPIRED: StatusCode.ValueType  # 68004
+UPLOAD_CANCELED: StatusCode.ValueType  # 68005
+UPLOAD_CONFLICT: StatusCode.ValueType  # 68006
 BILLING_INVALID_INFO: StatusCode.ValueType  # 69000
 """Billing related issues: 69xxx"""
 INTERNAL_SERVER_ISSUE: StatusCode.ValueType  # 98004
 """Internal issues: 98xxx"""
 INTERNAL_FETCHING_ISSUE: StatusCode.ValueType  # 98005
 INTERNAL_DATABASE_ISSUE: StatusCode.ValueType  # 98006
 INTERNAL_UNEXPECTED_TIMEOUT: StatusCode.ValueType  # 98009
```

### Comparing `clarifai-grpc-9.5.0/clarifai_grpc/grpc/api/status/status_pb2.py` & `clarifai-grpc-9.6.0/clarifai_grpc/grpc/api/status/status_pb2.py`

 * *Files identical despite different names*

### Comparing `clarifai-grpc-9.5.0/clarifai_grpc/grpc/api/status/status_pb2.pyi` & `clarifai-grpc-9.6.0/clarifai_grpc/grpc/api/status/status_pb2.pyi`

 * *Files identical despite different names*

### Comparing `clarifai-grpc-9.5.0/clarifai_grpc/grpc/api/utils/extensions_pb2.py` & `clarifai-grpc-9.6.0/clarifai_grpc/grpc/api/utils/extensions_pb2.py`

 * *Files identical despite different names*

### Comparing `clarifai-grpc-9.5.0/clarifai_grpc/grpc/api/utils/extensions_pb2.pyi` & `clarifai-grpc-9.6.0/clarifai_grpc/grpc/api/utils/extensions_pb2.pyi`

 * *Files identical despite different names*

### Comparing `clarifai-grpc-9.5.0/clarifai_grpc/grpc/api/utils/matrix_pb2.py` & `clarifai-grpc-9.6.0/clarifai_grpc/grpc/api/utils/matrix_pb2.py`

 * *Files identical despite different names*

### Comparing `clarifai-grpc-9.5.0/clarifai_grpc/grpc/api/utils/matrix_pb2.pyi` & `clarifai-grpc-9.6.0/clarifai_grpc/grpc/api/utils/matrix_pb2.pyi`

 * *Files identical despite different names*

### Comparing `clarifai-grpc-9.5.0/clarifai_grpc/grpc/api/utils/test_proto_pb2.py` & `clarifai-grpc-9.6.0/clarifai_grpc/grpc/api/utils/test_proto_pb2.py`

 * *Files identical despite different names*

### Comparing `clarifai-grpc-9.5.0/clarifai_grpc/grpc/api/utils/test_proto_pb2.pyi` & `clarifai-grpc-9.6.0/clarifai_grpc/grpc/api/utils/test_proto_pb2.pyi`

 * *Files identical despite different names*

### Comparing `clarifai-grpc-9.5.0/clarifai_grpc/grpc/auth/scope/scope_pb2.py` & `clarifai-grpc-9.6.0/clarifai_grpc/grpc/auth/scope/scope_pb2.py`

 * *Files identical despite different names*

### Comparing `clarifai-grpc-9.5.0/clarifai_grpc/grpc/auth/scope/scope_pb2.pyi` & `clarifai-grpc-9.6.0/clarifai_grpc/grpc/auth/scope/scope_pb2.pyi`

 * *Files identical despite different names*

### Comparing `clarifai-grpc-9.5.0/clarifai_grpc/grpc/auth/types/types_pb2.py` & `clarifai-grpc-9.6.0/clarifai_grpc/grpc/auth/types/types_pb2.py`

 * *Files identical despite different names*

### Comparing `clarifai-grpc-9.5.0/clarifai_grpc/grpc/auth/types/types_pb2.pyi` & `clarifai-grpc-9.6.0/clarifai_grpc/grpc/auth/types/types_pb2.pyi`

 * *Files identical despite different names*

### Comparing `clarifai-grpc-9.5.0/clarifai_grpc/grpc/auth/util/extension_pb2.py` & `clarifai-grpc-9.6.0/clarifai_grpc/grpc/auth/util/extension_pb2.py`

 * *Files identical despite different names*

### Comparing `clarifai-grpc-9.5.0/clarifai_grpc/grpc/auth/util/extension_pb2.pyi` & `clarifai-grpc-9.6.0/clarifai_grpc/grpc/auth/util/extension_pb2.pyi`

 * *Files identical despite different names*

### Comparing `clarifai-grpc-9.5.0/clarifai_grpc.egg-info/PKG-INFO` & `clarifai-grpc-9.6.0/clarifai_grpc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clarifai-grpc
-Version: 9.5.0
+Version: 9.6.0
 Summary: Clarifai gRPC API Client
 Home-page: https://github.com/Clarifai/clarifai-python-grpc
 Author: Clarifai
 Author-email: support@clarifai.com
 License: Apache 2.0
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Programming Language :: Python :: 3
```

### Comparing `clarifai-grpc-9.5.0/clarifai_grpc.egg-info/SOURCES.txt` & `clarifai-grpc-9.6.0/clarifai_grpc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `clarifai-grpc-9.5.0/setup.py` & `clarifai-grpc-9.6.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 with open("README.md", "r") as fh:
   long_description = fh.read()
 
 packages = setuptools.find_packages(include=["clarifai_grpc*"])
 
 setuptools.setup(
     name="clarifai-grpc",
-    version="9.5.0",
+    version="9.6.0",
     author="Clarifai",
     author_email="support@clarifai.com",
     description="Clarifai gRPC API Client",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Clarifai/clarifai-python-grpc",
     packages=packages,
```

