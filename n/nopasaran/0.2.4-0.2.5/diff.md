# Comparing `tmp/nopasaran-0.2.4.tar.gz` & `tmp/nopasaran-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nopasaran-0.2.4.tar", last modified: Thu Jul  6 03:58:49 2023, max compression
+gzip compressed data, was "nopasaran-0.2.5.tar", last modified: Sat Jul  8 10:11:09 2023, max compression
```

## Comparing `nopasaran-0.2.4.tar` & `nopasaran-0.2.5.tar`

### file list

```diff
@@ -1,56 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 03:58:49.582018 nopasaran-0.2.4/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-06 03:58:41.000000 nopasaran-0.2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7502 2023-07-06 03:58:49.582018 nopasaran-0.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5560 2023-07-06 03:58:41.000000 nopasaran-0.2.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 03:58:49.578018 nopasaran-0.2.4/nopasaran/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 03:58:41.000000 nopasaran-0.2.4/nopasaran/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3836 2023-07-06 03:58:41.000000 nopasaran-0.2.4/nopasaran/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 03:58:49.578018 nopasaran-0.2.4/nopasaran/controllers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 03:58:41.000000 nopasaran-0.2.4/nopasaran/controllers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6478 2023-07-06 03:58:41.000000 nopasaran-0.2.4/nopasaran/controllers/controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-07-06 03:58:41.000000 nopasaran-0.2.4/nopasaran/controllers/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     4463 2023-07-06 03:58:41.000000 nopasaran-0.2.4/nopasaran/controllers/protocol.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2583 2023-07-06 03:58:41.000000 nopasaran-0.2.4/nopasaran/decorators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 03:58:49.578018 nopasaran-0.2.4/nopasaran/definitions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 03:58:41.000000 nopasaran-0.2.4/nopasaran/definitions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-07-06 03:58:41.000000 nopasaran-0.2.4/nopasaran/definitions/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-07-06 03:58:41.000000 nopasaran-0.2.4/nopasaran/definitions/control_channel.py
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-06 03:58:41.000000 nopasaran-0.2.4/nopasaran/definitions/events.py
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-07-06 03:58:41.000000 nopasaran-0.2.4/nopasaran/definitions/transitions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 03:58:49.578018 nopasaran-0.2.4/nopasaran/interpreters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 03:58:41.000000 nopasaran-0.2.4/nopasaran/interpreters/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      756 2023-07-06 03:58:41.000000 nopasaran-0.2.4/nopasaran/interpreters/action_interpreter.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      787 2023-07-06 03:58:41.000000 nopasaran-0.2.4/nopasaran/interpreters/condition_interpreter.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2131 2023-07-06 03:58:41.000000 nopasaran-0.2.4/nopasaran/interpreters/interpreter.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      817 2023-07-06 03:58:41.000000 nopasaran-0.2.4/nopasaran/interpreters/transition_interpreter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 03:58:49.578018 nopasaran-0.2.4/nopasaran/ipsec_tunnels/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 03:58:41.000000 nopasaran-0.2.4/nopasaran/ipsec_tunnels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4635 2023-07-06 03:58:41.000000 nopasaran-0.2.4/nopasaran/ipsec_tunnels/ipsec_conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 03:58:49.582018 nopasaran-0.2.4/nopasaran/machines/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 03:58:41.000000 nopasaran-0.2.4/nopasaran/machines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2899 2023-07-06 03:58:41.000000 nopasaran-0.2.4/nopasaran/machines/action_queue.py
--rw-r--r--   0 runner    (1001) docker     (123)     9036 2023-07-06 03:58:41.000000 nopasaran-0.2.4/nopasaran/machines/state_machine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 03:58:49.582018 nopasaran-0.2.4/nopasaran/parsers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 03:58:41.000000 nopasaran-0.2.4/nopasaran/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4271 2023-07-06 03:58:41.000000 nopasaran-0.2.4/nopasaran/parsers/interpreter_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     4610 2023-07-06 03:58:41.000000 nopasaran-0.2.4/nopasaran/parsers/state_machine_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 03:58:49.582018 nopasaran-0.2.4/nopasaran/primitives/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 03:58:41.000000 nopasaran-0.2.4/nopasaran/primitives/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    14684 2023-07-06 03:58:41.000000 nopasaran-0.2.4/nopasaran/primitives/action_primitives.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1025 2023-07-06 03:58:41.000000 nopasaran-0.2.4/nopasaran/primitives/condition_primitives.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      406 2023-07-06 03:58:41.000000 nopasaran-0.2.4/nopasaran/primitives/transition_primitives.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 03:58:49.582018 nopasaran-0.2.4/nopasaran/sniffers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 03:58:41.000000 nopasaran-0.2.4/nopasaran/sniffers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2664 2023-07-06 03:58:41.000000 nopasaran-0.2.4/nopasaran/sniffers/sniffer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3592 2023-07-06 03:58:41.000000 nopasaran-0.2.4/nopasaran/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 03:58:49.578018 nopasaran-0.2.4/nopasaran.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7502 2023-07-06 03:58:49.000000 nopasaran-0.2.4/nopasaran.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-07-06 03:58:49.000000 nopasaran-0.2.4/nopasaran.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 03:58:49.000000 nopasaran-0.2.4/nopasaran.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-06 03:58:49.000000 nopasaran-0.2.4/nopasaran.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 03:58:49.000000 nopasaran-0.2.4/nopasaran.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-06 03:58:49.000000 nopasaran-0.2.4/nopasaran.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 03:58:49.582018 nopasaran-0.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-07-06 03:58:49.000000 nopasaran-0.2.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 03:58:49.582018 nopasaran-0.2.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 03:58:41.000000 nopasaran-0.2.4/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 10:11:09.851551 nopasaran-0.2.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-08 10:10:57.000000 nopasaran-0.2.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7502 2023-07-08 10:11:09.851551 nopasaran-0.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5560 2023-07-08 10:10:57.000000 nopasaran-0.2.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 10:11:09.839551 nopasaran-0.2.5/nopasaran/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 10:10:57.000000 nopasaran-0.2.5/nopasaran/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3836 2023-07-08 10:10:57.000000 nopasaran-0.2.5/nopasaran/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 10:11:09.843551 nopasaran-0.2.5/nopasaran/controllers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 10:10:57.000000 nopasaran-0.2.5/nopasaran/controllers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6478 2023-07-08 10:10:57.000000 nopasaran-0.2.5/nopasaran/controllers/controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-07-08 10:10:57.000000 nopasaran-0.2.5/nopasaran/controllers/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4463 2023-07-08 10:10:57.000000 nopasaran-0.2.5/nopasaran/controllers/protocol.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2633 2023-07-08 10:10:57.000000 nopasaran-0.2.5/nopasaran/decorators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 10:11:09.843551 nopasaran-0.2.5/nopasaran/definitions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 10:10:57.000000 nopasaran-0.2.5/nopasaran/definitions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-07-08 10:10:57.000000 nopasaran-0.2.5/nopasaran/definitions/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-07-08 10:10:57.000000 nopasaran-0.2.5/nopasaran/definitions/control_channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-08 10:10:57.000000 nopasaran-0.2.5/nopasaran/definitions/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-07-08 10:10:57.000000 nopasaran-0.2.5/nopasaran/definitions/transitions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 10:11:09.847551 nopasaran-0.2.5/nopasaran/interpreters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 10:10:57.000000 nopasaran-0.2.5/nopasaran/interpreters/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      822 2023-07-08 10:10:57.000000 nopasaran-0.2.5/nopasaran/interpreters/action_interpreter.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      862 2023-07-08 10:10:57.000000 nopasaran-0.2.5/nopasaran/interpreters/condition_interpreter.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2130 2023-07-08 10:10:57.000000 nopasaran-0.2.5/nopasaran/interpreters/interpreter.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      895 2023-07-08 10:10:57.000000 nopasaran-0.2.5/nopasaran/interpreters/transition_interpreter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 10:11:09.847551 nopasaran-0.2.5/nopasaran/ipsec_tunnels/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 10:10:57.000000 nopasaran-0.2.5/nopasaran/ipsec_tunnels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4635 2023-07-08 10:10:57.000000 nopasaran-0.2.5/nopasaran/ipsec_tunnels/ipsec_conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 10:11:09.847551 nopasaran-0.2.5/nopasaran/machines/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 10:10:57.000000 nopasaran-0.2.5/nopasaran/machines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2899 2023-07-08 10:10:57.000000 nopasaran-0.2.5/nopasaran/machines/action_queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9036 2023-07-08 10:10:57.000000 nopasaran-0.2.5/nopasaran/machines/state_machine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 10:11:09.847551 nopasaran-0.2.5/nopasaran/parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 10:10:57.000000 nopasaran-0.2.5/nopasaran/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4271 2023-07-08 10:10:57.000000 nopasaran-0.2.5/nopasaran/parsers/interpreter_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4610 2023-07-08 10:10:57.000000 nopasaran-0.2.5/nopasaran/parsers/state_machine_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 10:11:09.847551 nopasaran-0.2.5/nopasaran/primitives/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 10:10:57.000000 nopasaran-0.2.5/nopasaran/primitives/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 10:11:09.851551 nopasaran-0.2.5/nopasaran/primitives/action_primitives/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 10:10:57.000000 nopasaran-0.2.5/nopasaran/primitives/action_primitives/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      925 2023-07-08 10:10:57.000000 nopasaran-0.2.5/nopasaran/primitives/action_primitives/action_primitives.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10481 2023-07-08 10:10:57.000000 nopasaran-0.2.5/nopasaran/primitives/action_primitives/control_channel_primitives.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3051 2023-07-08 10:10:57.000000 nopasaran-0.2.5/nopasaran/primitives/action_primitives/data_manipulation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3306 2023-07-08 10:10:57.000000 nopasaran-0.2.5/nopasaran/primitives/action_primitives/ip_primitives.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4571 2023-07-08 10:10:57.000000 nopasaran-0.2.5/nopasaran/primitives/action_primitives/nested_machine_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11862 2023-07-08 10:10:57.000000 nopasaran-0.2.5/nopasaran/primitives/action_primitives/tcp_primitives.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9859 2023-07-08 10:10:57.000000 nopasaran-0.2.5/nopasaran/primitives/action_primitives/tmp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3208 2023-07-08 10:10:57.000000 nopasaran-0.2.5/nopasaran/primitives/action_primitives/udp_primitives.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 10:11:09.851551 nopasaran-0.2.5/nopasaran/primitives/condition_primitives/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 10:10:57.000000 nopasaran-0.2.5/nopasaran/primitives/condition_primitives/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      307 2023-07-08 10:10:57.000000 nopasaran-0.2.5/nopasaran/primitives/condition_primitives/condition_primitives.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4727 2023-07-08 10:10:57.000000 nopasaran-0.2.5/nopasaran/primitives/condition_primitives/variable_comparisons.py
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-07-08 10:10:57.000000 nopasaran-0.2.5/nopasaran/primitives/primitives.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 10:11:09.851551 nopasaran-0.2.5/nopasaran/primitives/transition_primitives/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 10:10:57.000000 nopasaran-0.2.5/nopasaran/primitives/transition_primitives/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-07-08 10:10:57.000000 nopasaran-0.2.5/nopasaran/primitives/transition_primitives/assignment_transitions.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      332 2023-07-08 10:10:57.000000 nopasaran-0.2.5/nopasaran/primitives/transition_primitives/transition_primitives.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 10:11:09.851551 nopasaran-0.2.5/nopasaran/sniffers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 10:10:57.000000 nopasaran-0.2.5/nopasaran/sniffers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2664 2023-07-08 10:10:57.000000 nopasaran-0.2.5/nopasaran/sniffers/sniffer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3592 2023-07-08 10:10:57.000000 nopasaran-0.2.5/nopasaran/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 10:11:09.843551 nopasaran-0.2.5/nopasaran.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7502 2023-07-08 10:11:09.000000 nopasaran-0.2.5/nopasaran.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-07-08 10:11:09.000000 nopasaran-0.2.5/nopasaran.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 10:11:09.000000 nopasaran-0.2.5/nopasaran.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-08 10:11:09.000000 nopasaran-0.2.5/nopasaran.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 10:11:09.000000 nopasaran-0.2.5/nopasaran.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-08 10:11:09.000000 nopasaran-0.2.5/nopasaran.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 10:11:09.851551 nopasaran-0.2.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-07-08 10:11:08.000000 nopasaran-0.2.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 10:11:09.851551 nopasaran-0.2.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 10:10:57.000000 nopasaran-0.2.5/tests/__init__.py
```

### Comparing `nopasaran-0.2.4/LICENSE` & `nopasaran-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `nopasaran-0.2.4/PKG-INFO` & `nopasaran-0.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nopasaran
-Version: 0.2.4
+Version: 0.2.5
 Summary: NoPASARAN is an advanced network tool designed to detect, fingerprint, and locate network middleboxes in a unified framework.
 Home-page: https://github.com/BenIlies/NoPASARAN
 Author: Ilies Benhabbour
 Author-email: ilies.benhabbour@kaust.edu.sa
 License: UNKNOWN
 Description: # NoPASARAN
```

### Comparing `nopasaran-0.2.4/README.md` & `nopasaran-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `nopasaran-0.2.4/nopasaran/__main__.py` & `nopasaran-0.2.5/nopasaran/__main__.py`

 * *Files identical despite different names*

### Comparing `nopasaran-0.2.4/nopasaran/controllers/controller.py` & `nopasaran-0.2.5/nopasaran/controllers/controller.py`

 * *Files identical despite different names*

### Comparing `nopasaran-0.2.4/nopasaran/controllers/factory.py` & `nopasaran-0.2.5/nopasaran/controllers/factory.py`

 * *Files identical despite different names*

### Comparing `nopasaran-0.2.4/nopasaran/controllers/protocol.py` & `nopasaran-0.2.5/nopasaran/controllers/protocol.py`

 * *Files identical despite different names*

### Comparing `nopasaran-0.2.4/nopasaran/decorators.py` & `nopasaran-0.2.5/nopasaran/decorators.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 import logging
 
+from functools import wraps
+
 from nopasaran.parsers.interpreter_parser import Parser
 
 
 def parsing_decorator(input_args, output_args, optional_inputs=False, optional_outputs=False):
     """
     Decorator for parsing inputs and outputs of a function.
     
@@ -18,14 +20,15 @@
     Returns:
         function: The decorated function.
     
     Raises:
         RuntimeError: If an error occurs while parsing or executing the function.
     """
     def decorator(func):
+        @wraps(func)
         def wrapper(line, variable_dict):
             """
             Wrapper function for the decorator.
             
             This function parses the inputs and outputs, logs the details, and calls the decorated function.
             
             Args:
```

### Comparing `nopasaran-0.2.4/nopasaran/definitions/control_channel.py` & `nopasaran-0.2.5/nopasaran/definitions/control_channel.py`

 * *Files identical despite different names*

### Comparing `nopasaran-0.2.4/nopasaran/interpreters/action_interpreter.py` & `nopasaran-0.2.5/nopasaran/interpreters/condition_interpreter.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 from nopasaran.interpreters.interpreter import Interpreter
-from nopasaran.primitives.action_primitives import ActionPrimitives
+from nopasaran.primitives.condition_primitives.condition_primitives import ConditionPrimitives
 
 
-class ActionInterpreter(Interpreter):
+class ConditionInterpreter(Interpreter):
     """
-    A custom ActionInterpreter class that inherits from Interpreter.
-    This class interprets actions in the context of a command-line interface.
+    A custom ConditionInterpreter class that inherits from Interpreter.
+    This class interprets conditions in the context of a command-line interface.
     """
 
     @classmethod
     def evaluate(cls, line, state_variables):
         """
-        Evaluate the action line using the provided state variables.
+        Evaluate the condition line using the provided state variables.
 
         Args:
-            line (str): The action line to evaluate.
+            line (str): The condition line to evaluate.
             state_variables: The state variables to use during evaluation.
 
         Returns:
             The result of the evaluation.
         """
-        super().evaluate(line, state_variables, ActionPrimitives)
+        condition_primitives = ConditionPrimitives()
+        return super().evaluate(line, state_variables, condition_primitives)
```

### Comparing `nopasaran-0.2.4/nopasaran/interpreters/interpreter.py` & `nopasaran-0.2.5/nopasaran/interpreters/interpreter.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     def evaluate(cls, line, variable, *function_classes):
         """
         Evaluate the input line using the provided variable and function classes.
 
         Args:
             line (str): The input line to evaluate.
             variable: The variable to use during evaluation.
-            *function_classes: Variable-length argument list of function classes.
+            function_classes: Variable-length argument list of function classes.
 
         Returns:
             The result of the evaluation.
         """
         instance = cls()
         instance.function_classes = function_classes
         return instance.onecmd(line, variable)
```

### Comparing `nopasaran-0.2.4/nopasaran/interpreters/transition_interpreter.py` & `nopasaran-0.2.5/nopasaran/interpreters/transition_interpreter.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from nopasaran.interpreters.interpreter import Interpreter
-from nopasaran.primitives.transition_primitives import TransitionPrimitives
+from nopasaran.primitives.transition_primitives.transition_primitives import TransitionPrimitives
 
 
 class TransitionInterpreter(Interpreter):
     """
     A custom TransitionInterpreter class that inherits from Interpreter.
     This class interprets transitions in the context of a command-line interface.
     """
@@ -16,8 +16,9 @@
         Args:
             line (str): The transition line to evaluate.
             trans_tmp_dict: The transition temporary dictionary to use during evaluation.
 
         Returns:
             The result of the evaluation.
         """
-        super().evaluate(line, trans_tmp_dict, TransitionPrimitives)
+        transition_primitives = TransitionPrimitives()
+        super().evaluate(line, trans_tmp_dict, transition_primitives)
```

### Comparing `nopasaran-0.2.4/nopasaran/ipsec_tunnels/ipsec_conf.py` & `nopasaran-0.2.5/nopasaran/ipsec_tunnels/ipsec_conf.py`

 * *Files identical despite different names*

### Comparing `nopasaran-0.2.4/nopasaran/machines/action_queue.py` & `nopasaran-0.2.5/nopasaran/machines/action_queue.py`

 * *Files identical despite different names*

### Comparing `nopasaran-0.2.4/nopasaran/machines/state_machine.py` & `nopasaran-0.2.5/nopasaran/machines/state_machine.py`

 * *Files identical despite different names*

### Comparing `nopasaran-0.2.4/nopasaran/parsers/interpreter_parser.py` & `nopasaran-0.2.5/nopasaran/parsers/interpreter_parser.py`

 * *Files identical despite different names*

### Comparing `nopasaran-0.2.4/nopasaran/parsers/state_machine_parser.py` & `nopasaran-0.2.5/nopasaran/parsers/state_machine_parser.py`

 * *Files identical despite different names*

### Comparing `nopasaran-0.2.4/nopasaran/sniffers/sniffer.py` & `nopasaran-0.2.5/nopasaran/sniffers/sniffer.py`

 * *Files identical despite different names*

### Comparing `nopasaran-0.2.4/nopasaran/utils.py` & `nopasaran-0.2.5/nopasaran/utils.py`

 * *Files identical despite different names*

### Comparing `nopasaran-0.2.4/nopasaran.egg-info/PKG-INFO` & `nopasaran-0.2.5/nopasaran.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nopasaran
-Version: 0.2.4
+Version: 0.2.5
 Summary: NoPASARAN is an advanced network tool designed to detect, fingerprint, and locate network middleboxes in a unified framework.
 Home-page: https://github.com/BenIlies/NoPASARAN
 Author: Ilies Benhabbour
 Author-email: ilies.benhabbour@kaust.edu.sa
 License: UNKNOWN
 Description: # NoPASARAN
```

### Comparing `nopasaran-0.2.4/setup.py` & `nopasaran-0.2.5/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 requirements_file = os.path.join(os.path.dirname(__file__), "requirements.txt")
 with open(requirements_file, "r") as f:
     requirements = [str(req) for req in parse_requirements(f)]
 
 # Version will automatically be updated when pushed on the main branch
 setup(
     name="nopasaran",
-    version='0.2.4',
+    version='0.2.5',
     author="Ilies Benhabbour",
     author_email="ilies.benhabbour@kaust.edu.sa",
     description="NoPASARAN is an advanced network tool designed to detect, fingerprint, and locate network middleboxes in a unified framework.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/BenIlies/NoPASARAN",
     packages=find_packages(),
```

