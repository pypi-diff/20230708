# Comparing `tmp/SuperSuit-3.8.0.tar.gz` & `tmp/SuperSuit-3.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SuperSuit-3.8.0.tar", last modified: Mon May 15 21:03:05 2023, max compression
+gzip compressed data, was "SuperSuit-3.8.1.tar", last modified: Fri Jul  7 23:49:42 2023, max compression
```

## Comparing `SuperSuit-3.8.0.tar` & `SuperSuit-3.8.1.tar`

### file list

```diff
@@ -1,101 +1,101 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:03:05.038030 SuperSuit-3.8.0/
--rw-r--r--   0 runner    (1001) docker     (123)    12201 2023-05-15 21:03:02.000000 SuperSuit-3.8.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2321 2023-05-15 21:03:05.038030 SuperSuit-3.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-05-15 21:03:02.000000 SuperSuit-3.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:03:05.030030 SuperSuit-3.8.0/SuperSuit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2321 2023-05-15 21:03:05.000000 SuperSuit-3.8.0/SuperSuit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3030 2023-05-15 21:03:05.000000 SuperSuit-3.8.0/SuperSuit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 21:03:05.000000 SuperSuit-3.8.0/SuperSuit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-15 21:03:05.000000 SuperSuit-3.8.0/SuperSuit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-15 21:03:05.000000 SuperSuit-3.8.0/SuperSuit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 21:03:05.038030 SuperSuit-3.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-05-15 21:03:02.000000 SuperSuit-3.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:03:05.030030 SuperSuit-3.8.0/supersuit/
--rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-05-15 21:03:02.000000 SuperSuit-3.8.0/supersuit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:03:05.030030 SuperSuit-3.8.0/supersuit/aec_vector/
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-15 21:03:02.000000 SuperSuit-3.8.0/supersuit/aec_vector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18256 2023-05-15 21:03:02.000000 SuperSuit-3.8.0/supersuit/aec_vector/async_vector_env.py
--rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-05-15 21:03:02.000000 SuperSuit-3.8.0/supersuit/aec_vector/base_aec_vec_env.py
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-05-15 21:03:02.000000 SuperSuit-3.8.0/supersuit/aec_vector/create.py
--rw-r--r--   0 runner    (1001) docker     (123)     5787 2023-05-15 21:03:02.000000 SuperSuit-3.8.0/supersuit/aec_vector/vector_env.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:03:05.034030 SuperSuit-3.8.0/supersuit/generic_wrappers/
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-05-15 21:03:02.000000 SuperSuit-3.8.0/supersuit/generic_wrappers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-05-15 21:03:02.000000 SuperSuit-3.8.0/supersuit/generic_wrappers/basic_wrappers.py
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-05-15 21:03:02.000000 SuperSuit-3.8.0/supersuit/generic_wrappers/delay_observations.py
--rw-r--r--   0 runner    (1001) docker     (123)     7962 2023-05-15 21:03:02.000000 SuperSuit-3.8.0/supersuit/generic_wrappers/frame_skip.py
--rw-r--r--   0 runner    (1001) docker     (123)     3351 2023-05-15 21:03:02.000000 SuperSuit-3.8.0/supersuit/generic_wrappers/frame_stack.py
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-05-15 21:03:02.000000 SuperSuit-3.8.0/supersuit/generic_wrappers/max_observation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-05-15 21:03:02.000000 SuperSuit-3.8.0/supersuit/generic_wrappers/nan_wrappers.py
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-05-15 21:03:02.000000 SuperSuit-3.8.0/supersuit/generic_wrappers/sticky_actions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:03:05.034030 SuperSuit-3.8.0/supersuit/generic_wrappers/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 21:03:02.000000 SuperSuit-3.8.0/supersuit/generic_wrappers/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-05-15 21:03:02.000000 SuperSuit-3.8.0/supersuit/generic_wrappers/utils/base_modifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     5709 2023-05-15 21:03:02.000000 SuperSuit-3.8.0/supersuit/generic_wrappers/utils/shared_wrapper_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:03:05.034030 SuperSuit-3.8.0/supersuit/lambda_wrappers/
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-05-15 21:03:02.000000 SuperSuit-3.8.0/supersuit/lambda_wrappers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-05-15 21:03:02.000000 SuperSuit-3.8.0/supersuit/lambda_wrappers/action_lambda.py
--rw-r--r--   0 runner    (1001) docker     (123)     5161 2023-05-15 21:03:02.000000 SuperSuit-3.8.0/supersuit/lambda_wrappers/observation_lambda.py
--rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-05-15 21:03:02.000000 SuperSuit-3.8.0/supersuit/lambda_wrappers/reward_lambda.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:03:05.034030 SuperSuit-3.8.0/supersuit/multiagent_wrappers/
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-05-15 21:03:02.000000 SuperSuit-3.8.0/supersuit/multiagent_wrappers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-05-15 21:03:02.000000 SuperSuit-3.8.0/supersuit/multiagent_wrappers/agent_indication.py
--rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-05-15 21:03:02.000000 SuperSuit-3.8.0/supersuit/multiagent_wrappers/black_death.py
--rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-05-15 21:03:02.000000 SuperSuit-3.8.0/supersuit/multiagent_wrappers/padding_wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:03:05.034030 SuperSuit-3.8.0/supersuit/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 21:03:02.000000 SuperSuit-3.8.0/supersuit/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-05-15 21:03:02.000000 SuperSuit-3.8.0/supersuit/utils/accumulator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:03:05.034030 SuperSuit-3.8.0/supersuit/utils/action_transforms/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 21:03:02.000000 SuperSuit-3.8.0/supersuit/utils/action_transforms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3473 2023-05-15 21:03:02.000000 SuperSuit-3.8.0/supersuit/utils/action_transforms/homogenize_ops.py
--rw-r--r--   0 runner    (1001) docker     (123)     3533 2023-05-15 21:03:02.000000 SuperSuit-3.8.0/supersuit/utils/agent_indicator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-05-15 21:03:02.000000 SuperSuit-3.8.0/supersuit/utils/base_aec_wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:03:05.034030 SuperSuit-3.8.0/supersuit/utils/basic_transforms/
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-05-15 21:03:02.000000 SuperSuit-3.8.0/supersuit/utils/basic_transforms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-05-15 21:03:02.000000 SuperSuit-3.8.0/supersuit/utils/basic_transforms/color_reduction.py
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-05-15 21:03:02.000000 SuperSuit-3.8.0/supersuit/utils/basic_transforms/dtype.py
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-05-15 21:03:02.000000 SuperSuit-3.8.0/supersuit/utils/basic_transforms/flatten.py
--rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-05-15 21:03:02.000000 SuperSuit-3.8.0/supersuit/utils/basic_transforms/normalize_obs.py
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-05-15 21:03:02.000000 SuperSuit-3.8.0/supersuit/utils/basic_transforms/reshape.py
--rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-05-15 21:03:02.000000 SuperSuit-3.8.0/supersuit/utils/basic_transforms/resize.py
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-05-15 21:03:02.000000 SuperSuit-3.8.0/supersuit/utils/convert_box.py
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-05-15 21:03:02.000000 SuperSuit-3.8.0/supersuit/utils/frame_skip.py
--rw-r--r--   0 runner    (1001) docker     (123)     3837 2023-05-15 21:03:02.000000 SuperSuit-3.8.0/supersuit/utils/frame_stack.py
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-05-15 21:03:02.000000 SuperSuit-3.8.0/supersuit/utils/make_defaultdict.py
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-05-15 21:03:02.000000 SuperSuit-3.8.0/supersuit/utils/obs_delay.py
--rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-05-15 21:03:02.000000 SuperSuit-3.8.0/supersuit/utils/wrapper_chooser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:03:05.038030 SuperSuit-3.8.0/supersuit/vector/
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-05-15 21:03:02.000000 SuperSuit-3.8.0/supersuit/vector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3788 2023-05-15 21:03:02.000000 SuperSuit-3.8.0/supersuit/vector/concat_vec_env.py
--rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-05-15 21:03:02.000000 SuperSuit-3.8.0/supersuit/vector/constructors.py
--rw-r--r--   0 runner    (1001) docker     (123)     4844 2023-05-15 21:03:02.000000 SuperSuit-3.8.0/supersuit/vector/markov_vector_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     8726 2023-05-15 21:03:02.000000 SuperSuit-3.8.0/supersuit/vector/multiproc_vec.py
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-05-15 21:03:02.000000 SuperSuit-3.8.0/supersuit/vector/sb3_vector_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-05-15 21:03:02.000000 SuperSuit-3.8.0/supersuit/vector/sb_vector_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-05-15 21:03:02.000000 SuperSuit-3.8.0/supersuit/vector/single_vec_env.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:03:05.038030 SuperSuit-3.8.0/supersuit/vector/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 21:03:02.000000 SuperSuit-3.8.0/supersuit/vector/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-05-15 21:03:02.000000 SuperSuit-3.8.0/supersuit/vector/utils/shared_array.py
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-05-15 21:03:02.000000 SuperSuit-3.8.0/supersuit/vector/utils/space_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3031 2023-05-15 21:03:02.000000 SuperSuit-3.8.0/supersuit/vector/vector_constructors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:03:05.038030 SuperSuit-3.8.0/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 21:03:02.000000 SuperSuit-3.8.0/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13699 2023-05-15 21:03:02.000000 SuperSuit-3.8.0/test/aec_mock_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4758 2023-05-15 21:03:02.000000 SuperSuit-3.8.0/test/aec_unwrapped_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-05-15 21:03:02.000000 SuperSuit-3.8.0/test/dummy_aec_env.py
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-05-15 21:03:02.000000 SuperSuit-3.8.0/test/dummy_gym_env.py
--rw-r--r--   0 runner    (1001) docker     (123)     5318 2023-05-15 21:03:02.000000 SuperSuit-3.8.0/test/generated_agents_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4264 2023-05-15 21:03:02.000000 SuperSuit-3.8.0/test/gym_mock_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2575 2023-05-15 21:03:02.000000 SuperSuit-3.8.0/test/gym_unwrapped_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-05-15 21:03:02.000000 SuperSuit-3.8.0/test/parallel_env_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4213 2023-05-15 21:03:02.000000 SuperSuit-3.8.0/test/pettingzoo_api_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-05-15 21:03:02.000000 SuperSuit-3.8.0/test/test_autodep.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:03:05.038030 SuperSuit-3.8.0/test/test_vector/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 21:03:02.000000 SuperSuit-3.8.0/test/test_vector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-05-15 21:03:02.000000 SuperSuit-3.8.0/test/test_vector/test_aec_vector_identity_env.py
--rw-r--r--   0 runner    (1001) docker     (123)     2792 2023-05-15 21:03:02.000000 SuperSuit-3.8.0/test/test_vector/test_aec_vector_values.py
--rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-05-15 21:03:02.000000 SuperSuit-3.8.0/test/test_vector/test_env_is_wrapped.py
--rw-r--r--   0 runner    (1001) docker     (123)     4517 2023-05-15 21:03:02.000000 SuperSuit-3.8.0/test/test_vector/test_gym_vector.py
--rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-05-15 21:03:02.000000 SuperSuit-3.8.0/test/test_vector/test_pettingzoo_to_vec.py
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-05-15 21:03:02.000000 SuperSuit-3.8.0/test/test_vector/test_render.py
--rw-r--r--   0 runner    (1001) docker     (123)     2959 2023-05-15 21:03:02.000000 SuperSuit-3.8.0/test/test_vector/test_vector_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-05-15 21:03:02.000000 SuperSuit-3.8.0/test/vec_env_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 23:49:42.639312 SuperSuit-3.8.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    12201 2023-07-07 23:49:36.000000 SuperSuit-3.8.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2321 2023-07-07 23:49:42.639312 SuperSuit-3.8.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-07-07 23:49:36.000000 SuperSuit-3.8.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 23:49:42.627312 SuperSuit-3.8.1/SuperSuit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2321 2023-07-07 23:49:42.000000 SuperSuit-3.8.1/SuperSuit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3030 2023-07-07 23:49:42.000000 SuperSuit-3.8.1/SuperSuit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 23:49:42.000000 SuperSuit-3.8.1/SuperSuit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-07 23:49:42.000000 SuperSuit-3.8.1/SuperSuit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-07 23:49:42.000000 SuperSuit-3.8.1/SuperSuit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 23:49:42.639312 SuperSuit-3.8.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-07-07 23:49:36.000000 SuperSuit-3.8.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 23:49:42.627312 SuperSuit-3.8.1/supersuit/
+-rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-07-07 23:49:36.000000 SuperSuit-3.8.1/supersuit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 23:49:42.627312 SuperSuit-3.8.1/supersuit/aec_vector/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-07 23:49:36.000000 SuperSuit-3.8.1/supersuit/aec_vector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18256 2023-07-07 23:49:36.000000 SuperSuit-3.8.1/supersuit/aec_vector/async_vector_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-07-07 23:49:36.000000 SuperSuit-3.8.1/supersuit/aec_vector/base_aec_vec_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-07-07 23:49:36.000000 SuperSuit-3.8.1/supersuit/aec_vector/create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5787 2023-07-07 23:49:36.000000 SuperSuit-3.8.1/supersuit/aec_vector/vector_env.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 23:49:42.631312 SuperSuit-3.8.1/supersuit/generic_wrappers/
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-07-07 23:49:36.000000 SuperSuit-3.8.1/supersuit/generic_wrappers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-07-07 23:49:36.000000 SuperSuit-3.8.1/supersuit/generic_wrappers/basic_wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-07-07 23:49:36.000000 SuperSuit-3.8.1/supersuit/generic_wrappers/delay_observations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7962 2023-07-07 23:49:36.000000 SuperSuit-3.8.1/supersuit/generic_wrappers/frame_skip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3351 2023-07-07 23:49:36.000000 SuperSuit-3.8.1/supersuit/generic_wrappers/frame_stack.py
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-07-07 23:49:36.000000 SuperSuit-3.8.1/supersuit/generic_wrappers/max_observation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-07-07 23:49:36.000000 SuperSuit-3.8.1/supersuit/generic_wrappers/nan_wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-07-07 23:49:36.000000 SuperSuit-3.8.1/supersuit/generic_wrappers/sticky_actions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 23:49:42.631312 SuperSuit-3.8.1/supersuit/generic_wrappers/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 23:49:36.000000 SuperSuit-3.8.1/supersuit/generic_wrappers/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-07-07 23:49:36.000000 SuperSuit-3.8.1/supersuit/generic_wrappers/utils/base_modifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5709 2023-07-07 23:49:36.000000 SuperSuit-3.8.1/supersuit/generic_wrappers/utils/shared_wrapper_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 23:49:42.631312 SuperSuit-3.8.1/supersuit/lambda_wrappers/
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-07 23:49:36.000000 SuperSuit-3.8.1/supersuit/lambda_wrappers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-07-07 23:49:36.000000 SuperSuit-3.8.1/supersuit/lambda_wrappers/action_lambda.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5161 2023-07-07 23:49:36.000000 SuperSuit-3.8.1/supersuit/lambda_wrappers/observation_lambda.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-07-07 23:49:36.000000 SuperSuit-3.8.1/supersuit/lambda_wrappers/reward_lambda.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 23:49:42.631312 SuperSuit-3.8.1/supersuit/multiagent_wrappers/
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-07-07 23:49:36.000000 SuperSuit-3.8.1/supersuit/multiagent_wrappers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-07-07 23:49:36.000000 SuperSuit-3.8.1/supersuit/multiagent_wrappers/agent_indication.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-07-07 23:49:36.000000 SuperSuit-3.8.1/supersuit/multiagent_wrappers/black_death.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-07-07 23:49:36.000000 SuperSuit-3.8.1/supersuit/multiagent_wrappers/padding_wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 23:49:42.631312 SuperSuit-3.8.1/supersuit/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 23:49:36.000000 SuperSuit-3.8.1/supersuit/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-07-07 23:49:36.000000 SuperSuit-3.8.1/supersuit/utils/accumulator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 23:49:42.631312 SuperSuit-3.8.1/supersuit/utils/action_transforms/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 23:49:36.000000 SuperSuit-3.8.1/supersuit/utils/action_transforms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3473 2023-07-07 23:49:36.000000 SuperSuit-3.8.1/supersuit/utils/action_transforms/homogenize_ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3533 2023-07-07 23:49:36.000000 SuperSuit-3.8.1/supersuit/utils/agent_indicator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-07-07 23:49:36.000000 SuperSuit-3.8.1/supersuit/utils/base_aec_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 23:49:42.631312 SuperSuit-3.8.1/supersuit/utils/basic_transforms/
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-07-07 23:49:36.000000 SuperSuit-3.8.1/supersuit/utils/basic_transforms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-07-07 23:49:36.000000 SuperSuit-3.8.1/supersuit/utils/basic_transforms/color_reduction.py
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-07-07 23:49:36.000000 SuperSuit-3.8.1/supersuit/utils/basic_transforms/dtype.py
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-07-07 23:49:36.000000 SuperSuit-3.8.1/supersuit/utils/basic_transforms/flatten.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-07-07 23:49:36.000000 SuperSuit-3.8.1/supersuit/utils/basic_transforms/normalize_obs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-07-07 23:49:36.000000 SuperSuit-3.8.1/supersuit/utils/basic_transforms/reshape.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-07-07 23:49:36.000000 SuperSuit-3.8.1/supersuit/utils/basic_transforms/resize.py
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-07-07 23:49:36.000000 SuperSuit-3.8.1/supersuit/utils/convert_box.py
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-07-07 23:49:36.000000 SuperSuit-3.8.1/supersuit/utils/frame_skip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3837 2023-07-07 23:49:36.000000 SuperSuit-3.8.1/supersuit/utils/frame_stack.py
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-07-07 23:49:36.000000 SuperSuit-3.8.1/supersuit/utils/make_defaultdict.py
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-07-07 23:49:36.000000 SuperSuit-3.8.1/supersuit/utils/obs_delay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-07-07 23:49:36.000000 SuperSuit-3.8.1/supersuit/utils/wrapper_chooser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 23:49:42.635312 SuperSuit-3.8.1/supersuit/vector/
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-07-07 23:49:36.000000 SuperSuit-3.8.1/supersuit/vector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3788 2023-07-07 23:49:36.000000 SuperSuit-3.8.1/supersuit/vector/concat_vec_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-07-07 23:49:36.000000 SuperSuit-3.8.1/supersuit/vector/constructors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4844 2023-07-07 23:49:36.000000 SuperSuit-3.8.1/supersuit/vector/markov_vector_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8684 2023-07-07 23:49:36.000000 SuperSuit-3.8.1/supersuit/vector/multiproc_vec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-07-07 23:49:36.000000 SuperSuit-3.8.1/supersuit/vector/sb3_vector_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-07-07 23:49:36.000000 SuperSuit-3.8.1/supersuit/vector/sb_vector_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-07-07 23:49:36.000000 SuperSuit-3.8.1/supersuit/vector/single_vec_env.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 23:49:42.635312 SuperSuit-3.8.1/supersuit/vector/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 23:49:36.000000 SuperSuit-3.8.1/supersuit/vector/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-07 23:49:36.000000 SuperSuit-3.8.1/supersuit/vector/utils/shared_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-07-07 23:49:36.000000 SuperSuit-3.8.1/supersuit/vector/utils/space_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3031 2023-07-07 23:49:36.000000 SuperSuit-3.8.1/supersuit/vector/vector_constructors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 23:49:42.635312 SuperSuit-3.8.1/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 23:49:36.000000 SuperSuit-3.8.1/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13699 2023-07-07 23:49:36.000000 SuperSuit-3.8.1/test/aec_mock_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4758 2023-07-07 23:49:36.000000 SuperSuit-3.8.1/test/aec_unwrapped_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-07-07 23:49:36.000000 SuperSuit-3.8.1/test/dummy_aec_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-07-07 23:49:36.000000 SuperSuit-3.8.1/test/dummy_gym_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5318 2023-07-07 23:49:36.000000 SuperSuit-3.8.1/test/generated_agents_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4264 2023-07-07 23:49:36.000000 SuperSuit-3.8.1/test/gym_mock_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2575 2023-07-07 23:49:36.000000 SuperSuit-3.8.1/test/gym_unwrapped_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-07-07 23:49:36.000000 SuperSuit-3.8.1/test/parallel_env_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4213 2023-07-07 23:49:36.000000 SuperSuit-3.8.1/test/pettingzoo_api_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-07-07 23:49:36.000000 SuperSuit-3.8.1/test/test_autodep.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 23:49:42.639312 SuperSuit-3.8.1/test/test_vector/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 23:49:36.000000 SuperSuit-3.8.1/test/test_vector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-07-07 23:49:36.000000 SuperSuit-3.8.1/test/test_vector/test_aec_vector_identity_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2792 2023-07-07 23:49:36.000000 SuperSuit-3.8.1/test/test_vector/test_aec_vector_values.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-07-07 23:49:36.000000 SuperSuit-3.8.1/test/test_vector/test_env_is_wrapped.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4517 2023-07-07 23:49:36.000000 SuperSuit-3.8.1/test/test_vector/test_gym_vector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-07-07 23:49:36.000000 SuperSuit-3.8.1/test/test_vector/test_pettingzoo_to_vec.py
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-07-07 23:49:36.000000 SuperSuit-3.8.1/test/test_vector/test_render.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2959 2023-07-07 23:49:36.000000 SuperSuit-3.8.1/test/test_vector/test_vector_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-07-07 23:49:36.000000 SuperSuit-3.8.1/test/vec_env_test.py
```

### Comparing `SuperSuit-3.8.0/LICENSE.txt` & `SuperSuit-3.8.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `SuperSuit-3.8.0/PKG-INFO` & `SuperSuit-3.8.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SuperSuit
-Version: 3.8.0
+Version: 3.8.1
 Summary: Wrappers for Gymnasium and PettingZoo
 Home-page: https://github.com/Farama-Foundation/SuperSuit
 Author: Farama Foundation
 Author-email: contact@farama.org
 Keywords: Reinforcement Learning,game,RL,AI,gymnasium
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `SuperSuit-3.8.0/README.md` & `SuperSuit-3.8.1/README.md`

 * *Files identical despite different names*

### Comparing `SuperSuit-3.8.0/SuperSuit.egg-info/PKG-INFO` & `SuperSuit-3.8.1/SuperSuit.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SuperSuit
-Version: 3.8.0
+Version: 3.8.1
 Summary: Wrappers for Gymnasium and PettingZoo
 Home-page: https://github.com/Farama-Foundation/SuperSuit
 Author: Farama Foundation
 Author-email: contact@farama.org
 Keywords: Reinforcement Learning,game,RL,AI,gymnasium
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `SuperSuit-3.8.0/SuperSuit.egg-info/SOURCES.txt` & `SuperSuit-3.8.1/SuperSuit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `SuperSuit-3.8.0/setup.py` & `SuperSuit-3.8.1/setup.py`

 * *Files identical despite different names*

### Comparing `SuperSuit-3.8.0/supersuit/__init__.py` & `SuperSuit-3.8.1/supersuit/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -61,8 +61,8 @@
                     raise DeprecatedWrapper(
                         f"{base}{version_num} is now deprecated, use {base}{act_version_num} instead"
                     )
 
     raise ImportError(f"cannot import name '{wrapper_name}' from 'supersuit'")
 
 
-__version__ = "3.8.0"
+__version__ = "3.8.1"
```

### Comparing `SuperSuit-3.8.0/supersuit/aec_vector/async_vector_env.py` & `SuperSuit-3.8.1/supersuit/aec_vector/async_vector_env.py`

 * *Files identical despite different names*

### Comparing `SuperSuit-3.8.0/supersuit/aec_vector/base_aec_vec_env.py` & `SuperSuit-3.8.1/supersuit/aec_vector/base_aec_vec_env.py`

 * *Files identical despite different names*

### Comparing `SuperSuit-3.8.0/supersuit/aec_vector/create.py` & `SuperSuit-3.8.1/supersuit/aec_vector/create.py`

 * *Files identical despite different names*

### Comparing `SuperSuit-3.8.0/supersuit/aec_vector/vector_env.py` & `SuperSuit-3.8.1/supersuit/aec_vector/vector_env.py`

 * *Files identical despite different names*

### Comparing `SuperSuit-3.8.0/supersuit/generic_wrappers/__init__.py` & `SuperSuit-3.8.1/supersuit/generic_wrappers/__init__.py`

 * *Files identical despite different names*

### Comparing `SuperSuit-3.8.0/supersuit/generic_wrappers/basic_wrappers.py` & `SuperSuit-3.8.1/supersuit/generic_wrappers/basic_wrappers.py`

 * *Files identical despite different names*

### Comparing `SuperSuit-3.8.0/supersuit/generic_wrappers/delay_observations.py` & `SuperSuit-3.8.1/supersuit/generic_wrappers/delay_observations.py`

 * *Files identical despite different names*

### Comparing `SuperSuit-3.8.0/supersuit/generic_wrappers/frame_skip.py` & `SuperSuit-3.8.1/supersuit/generic_wrappers/frame_skip.py`

 * *Files identical despite different names*

### Comparing `SuperSuit-3.8.0/supersuit/generic_wrappers/frame_stack.py` & `SuperSuit-3.8.1/supersuit/generic_wrappers/frame_stack.py`

 * *Files identical despite different names*

### Comparing `SuperSuit-3.8.0/supersuit/generic_wrappers/max_observation.py` & `SuperSuit-3.8.1/supersuit/generic_wrappers/max_observation.py`

 * *Files identical despite different names*

### Comparing `SuperSuit-3.8.0/supersuit/generic_wrappers/nan_wrappers.py` & `SuperSuit-3.8.1/supersuit/generic_wrappers/nan_wrappers.py`

 * *Files identical despite different names*

### Comparing `SuperSuit-3.8.0/supersuit/generic_wrappers/sticky_actions.py` & `SuperSuit-3.8.1/supersuit/generic_wrappers/sticky_actions.py`

 * *Files identical despite different names*

### Comparing `SuperSuit-3.8.0/supersuit/generic_wrappers/utils/base_modifier.py` & `SuperSuit-3.8.1/supersuit/generic_wrappers/utils/base_modifier.py`

 * *Files identical despite different names*

### Comparing `SuperSuit-3.8.0/supersuit/generic_wrappers/utils/shared_wrapper_util.py` & `SuperSuit-3.8.1/supersuit/generic_wrappers/utils/shared_wrapper_util.py`

 * *Files identical despite different names*

### Comparing `SuperSuit-3.8.0/supersuit/lambda_wrappers/action_lambda.py` & `SuperSuit-3.8.1/supersuit/lambda_wrappers/action_lambda.py`

 * *Files identical despite different names*

### Comparing `SuperSuit-3.8.0/supersuit/lambda_wrappers/observation_lambda.py` & `SuperSuit-3.8.1/supersuit/lambda_wrappers/observation_lambda.py`

 * *Files identical despite different names*

### Comparing `SuperSuit-3.8.0/supersuit/lambda_wrappers/reward_lambda.py` & `SuperSuit-3.8.1/supersuit/lambda_wrappers/reward_lambda.py`

 * *Files identical despite different names*

### Comparing `SuperSuit-3.8.0/supersuit/multiagent_wrappers/agent_indication.py` & `SuperSuit-3.8.1/supersuit/multiagent_wrappers/agent_indication.py`

 * *Files identical despite different names*

### Comparing `SuperSuit-3.8.0/supersuit/multiagent_wrappers/black_death.py` & `SuperSuit-3.8.1/supersuit/multiagent_wrappers/black_death.py`

 * *Files identical despite different names*

### Comparing `SuperSuit-3.8.0/supersuit/multiagent_wrappers/padding_wrappers.py` & `SuperSuit-3.8.1/supersuit/multiagent_wrappers/padding_wrappers.py`

 * *Files identical despite different names*

### Comparing `SuperSuit-3.8.0/supersuit/utils/accumulator.py` & `SuperSuit-3.8.1/supersuit/utils/accumulator.py`

 * *Files identical despite different names*

### Comparing `SuperSuit-3.8.0/supersuit/utils/action_transforms/homogenize_ops.py` & `SuperSuit-3.8.1/supersuit/utils/action_transforms/homogenize_ops.py`

 * *Files identical despite different names*

### Comparing `SuperSuit-3.8.0/supersuit/utils/agent_indicator.py` & `SuperSuit-3.8.1/supersuit/utils/agent_indicator.py`

 * *Files identical despite different names*

### Comparing `SuperSuit-3.8.0/supersuit/utils/base_aec_wrapper.py` & `SuperSuit-3.8.1/supersuit/utils/base_aec_wrapper.py`

 * *Files identical despite different names*

### Comparing `SuperSuit-3.8.0/supersuit/utils/basic_transforms/color_reduction.py` & `SuperSuit-3.8.1/supersuit/utils/basic_transforms/color_reduction.py`

 * *Files identical despite different names*

### Comparing `SuperSuit-3.8.0/supersuit/utils/basic_transforms/normalize_obs.py` & `SuperSuit-3.8.1/supersuit/utils/basic_transforms/normalize_obs.py`

 * *Files identical despite different names*

### Comparing `SuperSuit-3.8.0/supersuit/utils/basic_transforms/reshape.py` & `SuperSuit-3.8.1/supersuit/utils/basic_transforms/reshape.py`

 * *Files identical despite different names*

### Comparing `SuperSuit-3.8.0/supersuit/utils/basic_transforms/resize.py` & `SuperSuit-3.8.1/supersuit/utils/basic_transforms/resize.py`

 * *Files identical despite different names*

### Comparing `SuperSuit-3.8.0/supersuit/utils/frame_skip.py` & `SuperSuit-3.8.1/supersuit/utils/frame_skip.py`

 * *Files identical despite different names*

### Comparing `SuperSuit-3.8.0/supersuit/utils/frame_stack.py` & `SuperSuit-3.8.1/supersuit/utils/frame_stack.py`

 * *Files identical despite different names*

### Comparing `SuperSuit-3.8.0/supersuit/utils/wrapper_chooser.py` & `SuperSuit-3.8.1/supersuit/utils/wrapper_chooser.py`

 * *Files identical despite different names*

### Comparing `SuperSuit-3.8.0/supersuit/vector/concat_vec_env.py` & `SuperSuit-3.8.1/supersuit/vector/concat_vec_env.py`

 * *Files identical despite different names*

### Comparing `SuperSuit-3.8.0/supersuit/vector/constructors.py` & `SuperSuit-3.8.1/supersuit/vector/constructors.py`

 * *Files identical despite different names*

### Comparing `SuperSuit-3.8.0/supersuit/vector/markov_vector_wrapper.py` & `SuperSuit-3.8.1/supersuit/vector/markov_vector_wrapper.py`

 * *Files identical despite different names*

### Comparing `SuperSuit-3.8.0/supersuit/vector/multiproc_vec.py` & `SuperSuit-3.8.1/supersuit/vector/multiproc_vec.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import copy
 import multiprocessing as mp
+import time
 import traceback
 
 import gymnasium.vector
 import numpy as np
 from gymnasium.vector.utils import (
     concatenate,
     create_empty_array,
@@ -114,18 +115,14 @@
         pipe.send((e, tb))
 
 
 class ProcConcatVec(gymnasium.vector.VectorEnv):
     def __init__(
         self, vec_env_constrs, observation_space, action_space, tot_num_envs, metadata
     ):
-        raise NotImplementedError(
-            "The wrapper ProcConcatVec is temporarily depreciated whilst it is being debugged. "
-            "Please refer to https://github.com/Farama-Foundation/SuperSuit/pull/165 for more information, or to contact the devs in regard to this."
-        )
         self.observation_space = observation_space
         self.action_space = action_space
         self.num_envs = num_envs = tot_num_envs
         self.metadata = metadata
 
         self.shared_obs = create_shared_memory(self.observation_space, n=self.num_envs)
         self.shared_act = create_shared_memory(self.action_space, n=self.num_envs)
@@ -133,14 +130,16 @@
         self.shared_terms = SharedArray((num_envs,), dtype=np.uint8)
         self.shared_truncs = SharedArray((num_envs,), dtype=np.uint8)
 
         self.observations_buffers = read_from_shared_memory(
             self.observation_space, self.shared_obs, n=self.num_envs
         )
 
+        self.graceful_shutdown_timeout = 10
+
         pipes = []
         procs = []
         for constr in vec_env_constrs:
             inpt, outpt = mp.Pipe()
             constr = gymnasium.vector.async_vector_env.CloudpickleWrapper(constr)
             proc = mp.Process(
                 target=async_loop,
@@ -219,45 +218,49 @@
         )
 
     def step(self, actions):
         self.step_async(actions)
         return self.step_wait()
 
     def __del__(self):
-        for pipe in self.pipes:
-            try:
-                pipe.send("terminate")
-            except ConnectionError:
-                pass
-        for proc in self.procs:
-            proc.join()
+        self.close()
 
     def render(self):
         self.pipes[0].send("render")
         render_result = self.pipes[0].recv()
 
         if isinstance(render_result, tuple):
             e, tb = render_result
             print(tb)
             raise e
 
         return render_result
 
     def close(self):
-        for pipe in self.pipes:
-            pipe.send("close")
-        for pipe in self.pipes:
-            try:
-                pipe.recv()
-            except EOFError:
-                raise RuntimeError(
-                    "only one multiproccessing vector environment can open a window over the duration of a process"
-                )
-            except ConnectionError:
-                pass
+        try:
+            for pipe, proc in zip(self.pipes, self.procs):
+                if proc.is_alive():
+                    pipe.send("close")
+        except OSError:
+            pass
+        else:
+            deadline = (
+                None
+                if self.graceful_shutdown_timeout is None
+                else time.monotonic() + self.graceful_shutdown_timeout
+            )
+            for proc in self.procs:
+                timeout = None if deadline is None else deadline - time.monotonic()
+                if timeout is not None and timeout <= 0:
+                    break
+                proc.join(timeout)
+        for pipe, proc in zip(self.pipes, self.procs):
+            if proc.is_alive():
+                proc.kill()
+            pipe.close()
 
     def env_is_wrapped(self, wrapper_class, indices=None):
         for i, pipe in enumerate(self.pipes):
             pipe.send(("env_is_wrapped", wrapper_class))
 
         results = self._receive_info()
         return sum(results, [])
```

### Comparing `SuperSuit-3.8.0/supersuit/vector/sb3_vector_wrapper.py` & `SuperSuit-3.8.1/supersuit/vector/sb_vector_wrapper.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,27 +1,39 @@
-from stable_baselines3.common.vec_env import VecEnvWrapper
+from stable_baselines.common.vec_env.base_vec_env import VecEnv
 
 
-class SB3VecEnvWrapper(VecEnvWrapper):
+class SBVecEnvWrapper(VecEnv):
     def __init__(self, venv):
         self.venv = venv
         self.num_envs = venv.num_envs
         self.observation_space = venv.observation_space
         self.action_space = venv.action_space
 
     def reset(self, seed=None, options=None):
         if seed is not None:
             self.seed(seed=seed)
+
         return self.venv.reset()
 
+    def step_async(self, actions):
+        self.venv.step_async(actions)
+
     def step_wait(self):
         return self.venv.step_wait()
 
-    def env_is_wrapped(self, wrapper_class, indices=None):
-        # ignores indices
-        return self.venv.env_is_wrapped(wrapper_class)
+    def step(self, actions):
+        return self.venv.step(actions)
+
+    def close(self):
+        del self.venv
+
+    def seed(self, seed=None):
+        self.venv.seed(seed)
+
+    def get_attr(self, attr_name, indices=None):
+        raise NotImplementedError()
 
-    def getattr_recursive(self, name):
-        raise AttributeError(name)
+    def set_attr(self, attr_name, value, indices=None):
+        raise NotImplementedError()
 
-    def getattr_depth_check(self, name, already_found):
-        return None
+    def env_method(self, method_name, *method_args, indices=None, **method_kwargs):
+        raise NotImplementedError()
```

### Comparing `SuperSuit-3.8.0/supersuit/vector/single_vec_env.py` & `SuperSuit-3.8.1/supersuit/vector/single_vec_env.py`

 * *Files identical despite different names*

### Comparing `SuperSuit-3.8.0/supersuit/vector/utils/shared_array.py` & `SuperSuit-3.8.1/supersuit/vector/utils/shared_array.py`

 * *Files identical despite different names*

### Comparing `SuperSuit-3.8.0/supersuit/vector/vector_constructors.py` & `SuperSuit-3.8.1/supersuit/vector/vector_constructors.py`

 * *Files identical despite different names*

### Comparing `SuperSuit-3.8.0/test/aec_mock_test.py` & `SuperSuit-3.8.1/test/aec_mock_test.py`

 * *Files identical despite different names*

### Comparing `SuperSuit-3.8.0/test/aec_unwrapped_test.py` & `SuperSuit-3.8.1/test/aec_unwrapped_test.py`

 * *Files identical despite different names*

### Comparing `SuperSuit-3.8.0/test/dummy_aec_env.py` & `SuperSuit-3.8.1/test/dummy_aec_env.py`

 * *Files identical despite different names*

### Comparing `SuperSuit-3.8.0/test/generated_agents_test.py` & `SuperSuit-3.8.1/test/generated_agents_test.py`

 * *Files identical despite different names*

### Comparing `SuperSuit-3.8.0/test/gym_mock_test.py` & `SuperSuit-3.8.1/test/gym_mock_test.py`

 * *Files identical despite different names*

### Comparing `SuperSuit-3.8.0/test/gym_unwrapped_test.py` & `SuperSuit-3.8.1/test/gym_unwrapped_test.py`

 * *Files identical despite different names*

### Comparing `SuperSuit-3.8.0/test/parallel_env_test.py` & `SuperSuit-3.8.1/test/parallel_env_test.py`

 * *Files identical despite different names*

### Comparing `SuperSuit-3.8.0/test/pettingzoo_api_test.py` & `SuperSuit-3.8.1/test/pettingzoo_api_test.py`

 * *Files identical despite different names*

### Comparing `SuperSuit-3.8.0/test/test_vector/test_aec_vector_identity_env.py` & `SuperSuit-3.8.1/test/test_vector/test_aec_vector_identity_env.py`

 * *Files identical despite different names*

### Comparing `SuperSuit-3.8.0/test/test_vector/test_aec_vector_values.py` & `SuperSuit-3.8.1/test/test_vector/test_aec_vector_values.py`

 * *Files identical despite different names*

### Comparing `SuperSuit-3.8.0/test/test_vector/test_env_is_wrapped.py` & `SuperSuit-3.8.1/test/test_vector/test_env_is_wrapped.py`

 * *Files identical despite different names*

### Comparing `SuperSuit-3.8.0/test/test_vector/test_gym_vector.py` & `SuperSuit-3.8.1/test/test_vector/test_gym_vector.py`

 * *Files identical despite different names*

### Comparing `SuperSuit-3.8.0/test/test_vector/test_pettingzoo_to_vec.py` & `SuperSuit-3.8.1/test/test_vector/test_pettingzoo_to_vec.py`

 * *Files identical despite different names*

### Comparing `SuperSuit-3.8.0/test/test_vector/test_render.py` & `SuperSuit-3.8.1/test/test_vector/test_render.py`

 * *Files identical despite different names*

### Comparing `SuperSuit-3.8.0/test/test_vector/test_vector_dict.py` & `SuperSuit-3.8.1/test/test_vector/test_vector_dict.py`

 * *Files identical despite different names*

### Comparing `SuperSuit-3.8.0/test/vec_env_test.py` & `SuperSuit-3.8.1/test/vec_env_test.py`

 * *Files identical despite different names*

