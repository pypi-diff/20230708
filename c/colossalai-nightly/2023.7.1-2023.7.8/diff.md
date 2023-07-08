# Comparing `tmp/colossalai-nightly-2023.7.1.tar.gz` & `tmp/colossalai-nightly-2023.7.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "colossalai-nightly-2023.7.1.tar", last modified: Sat Jul  1 00:21:10 2023, max compression
+gzip compressed data, was "colossalai-nightly-2023.7.8.tar", last modified: Sat Jul  8 00:17:20 2023, max compression
```

## Comparing `colossalai-nightly-2023.7.1.tar` & `colossalai-nightly-2023.7.8.tar`

### file list

```diff
@@ -1,907 +1,955 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 00:21:10.800050 colossalai-nightly-2023.7.1/
--rw-r--r--   0 runner    (1001) docker     (123)    22244 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    25399 2023-07-01 00:21:10.800050 colossalai-nightly-2023.7.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    20789 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 00:21:10.732051 colossalai-nightly-2023.7.1/colossalai/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 00:21:10.732051 colossalai-nightly-2023.7.1/colossalai/_C/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/_C/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 00:21:10.732051 colossalai-nightly-2023.7.1/colossalai/_analyzer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/_analyzer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 00:21:10.732051 colossalai-nightly-2023.7.1/colossalai/_analyzer/_subclasses/
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/_analyzer/_subclasses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20609 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/_analyzer/_subclasses/_meta_registration.py
--rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/_analyzer/_subclasses/_monkey_patch.py
--rw-r--r--   0 runner    (1001) docker     (123)    18694 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/_analyzer/_subclasses/flop_tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     7667 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/_analyzer/_subclasses/meta_tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/_analyzer/envs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 00:21:10.732051 colossalai-nightly-2023.7.1/colossalai/_analyzer/fx/
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/_analyzer/fx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18761 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/_analyzer/fx/codegen.py
--rw-r--r--   0 runner    (1001) docker     (123)     9920 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/_analyzer/fx/graph_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     8526 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/_analyzer/fx/node_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 00:21:10.736050 colossalai-nightly-2023.7.1/colossalai/_analyzer/fx/passes/
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/_analyzer/fx/passes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12600 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/_analyzer/fx/passes/graph_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     9892 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/_analyzer/fx/passes/shape_prop.py
--rw-r--r--   0 runner    (1001) docker     (123)      983 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/_analyzer/fx/symbolic_profile.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 00:21:10.736050 colossalai-nightly-2023.7.1/colossalai/_analyzer/fx/tracer/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/_analyzer/fx/tracer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6512 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/_analyzer/fx/tracer/bias_addition.py
--rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/_analyzer/fx/tracer/custom_leaf_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     3651 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/_analyzer/fx/tracer/proxy.py
--rw-r--r--   0 runner    (1001) docker     (123)     6048 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/_analyzer/fx/tracer/symbolic_trace.py
--rw-r--r--   0 runner    (1001) docker     (123)    15758 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/_analyzer/fx/tracer/tracer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 00:21:10.736050 colossalai-nightly-2023.7.1/colossalai/amp/
--rw-r--r--   0 runner    (1001) docker     (123)     2313 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/amp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/amp/amp_type.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 00:21:10.736050 colossalai-nightly-2023.7.1/colossalai/amp/apex_amp/
--rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/amp/apex_amp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/amp/apex_amp/apex_amp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 00:21:10.736050 colossalai-nightly-2023.7.1/colossalai/amp/naive_amp/
--rw-r--r--   0 runner    (1001) docker     (123)     2422 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/amp/naive_amp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13454 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/amp/naive_amp/_fp16_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/amp/naive_amp/_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 00:21:10.736050 colossalai-nightly-2023.7.1/colossalai/amp/naive_amp/grad_scaler/
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/amp/naive_amp/grad_scaler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/amp/naive_amp/grad_scaler/base_grad_scaler.py
--rw-r--r--   0 runner    (1001) docker     (123)      748 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/amp/naive_amp/grad_scaler/constant_grad_scaler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4755 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/amp/naive_amp/grad_scaler/dynamic_grad_scaler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 00:21:10.736050 colossalai-nightly-2023.7.1/colossalai/amp/naive_amp/mixed_precision_mixin/
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/amp/naive_amp/mixed_precision_mixin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2596 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/amp/naive_amp/mixed_precision_mixin/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/amp/naive_amp/mixed_precision_mixin/bf16.py
--rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/amp/naive_amp/mixed_precision_mixin/fp16.py
--rw-r--r--   0 runner    (1001) docker     (123)     6098 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/amp/naive_amp/naive_amp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 00:21:10.736050 colossalai-nightly-2023.7.1/colossalai/amp/torch_amp/
--rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/amp/torch_amp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26520 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/amp/torch_amp/_grad_scaler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3344 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/amp/torch_amp/torch_amp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 00:21:10.736050 colossalai-nightly-2023.7.1/colossalai/auto_parallel/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/auto_parallel/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 00:21:10.736050 colossalai-nightly-2023.7.1/colossalai/auto_parallel/checkpoint/
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/auto_parallel/checkpoint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/auto_parallel/checkpoint/build_c_ext.py
--rw-r--r--   0 runner    (1001) docker     (123)     7716 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/auto_parallel/checkpoint/ckpt_solver_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3469 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/auto_parallel/checkpoint/ckpt_solver_chen.py
--rw-r--r--   0 runner    (1001) docker     (123)    18543 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/auto_parallel/checkpoint/ckpt_solver_rotor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4938 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/auto_parallel/checkpoint/operation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 00:21:10.736050 colossalai-nightly-2023.7.1/colossalai/auto_parallel/meta_profiler/
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/auto_parallel/meta_profiler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/auto_parallel/meta_profiler/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 00:21:10.740050 colossalai-nightly-2023.7.1/colossalai/auto_parallel/meta_profiler/meta_registry/
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/auto_parallel/meta_profiler/meta_registry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4050 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/auto_parallel/meta_profiler/meta_registry/activation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2824 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/auto_parallel/meta_profiler/meta_registry/binary_elementwise_ops.py
--rw-r--r--   0 runner    (1001) docker     (123)     7900 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/auto_parallel/meta_profiler/meta_registry/conv.py
--rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/auto_parallel/meta_profiler/meta_registry/embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)    25633 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/auto_parallel/meta_profiler/meta_registry/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/auto_parallel/meta_profiler/meta_registry/non_spmd.py
--rw-r--r--   0 runner    (1001) docker     (123)     9721 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/auto_parallel/meta_profiler/meta_registry/norm.py
--rw-r--r--   0 runner    (1001) docker     (123)     7399 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/auto_parallel/meta_profiler/meta_registry/pooling.py
--rw-r--r--   0 runner    (1001) docker     (123)     3363 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/auto_parallel/meta_profiler/meta_registry/tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2968 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/auto_parallel/meta_profiler/meta_registry/where.py
--rw-r--r--   0 runner    (1001) docker     (123)      763 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/auto_parallel/meta_profiler/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     4847 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/auto_parallel/meta_profiler/shard_metainfo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 00:21:10.740050 colossalai-nightly-2023.7.1/colossalai/auto_parallel/offload/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/auto_parallel/offload/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7001 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/auto_parallel/offload/amp_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3618 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/auto_parallel/offload/base_offload_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     2127 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/auto_parallel/offload/mem_optimize.py
--rw-r--r--   0 runner    (1001) docker     (123)     5134 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/auto_parallel/offload/region.py
--rw-r--r--   0 runner    (1001) docker     (123)    20381 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/auto_parallel/offload/region_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    10128 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/auto_parallel/offload/runtime.py
--rw-r--r--   0 runner    (1001) docker     (123)    18888 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/auto_parallel/offload/solver.py
--rw-r--r--   0 runner    (1001) docker     (123)    18549 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/auto_parallel/offload/training_simulator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2966 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/auto_parallel/offload/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 00:21:10.740050 colossalai-nightly-2023.7.1/colossalai/auto_parallel/passes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/auto_parallel/passes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5214 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/auto_parallel/passes/comm_metainfo_pass.py
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/auto_parallel/passes/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     6030 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/auto_parallel/passes/meta_info_prop.py
--rw-r--r--   0 runner    (1001) docker     (123)    12067 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/auto_parallel/passes/runtime_apply_pass.py
--rw-r--r--   0 runner    (1001) docker     (123)    22686 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/auto_parallel/passes/runtime_preparation_pass.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 00:21:10.740050 colossalai-nightly-2023.7.1/colossalai/auto_parallel/pipeline_shard/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/auto_parallel/pipeline_shard/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 00:21:10.740050 colossalai-nightly-2023.7.1/colossalai/auto_parallel/tensor_shard/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/auto_parallel/tensor_shard/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2662 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/auto_parallel/tensor_shard/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    18744 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/auto_parallel/tensor_shard/initialize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 00:21:10.744050 colossalai-nightly-2023.7.1/colossalai/auto_parallel/tensor_shard/node_handler/
--rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/auto_parallel/tensor_shard/node_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4187 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/auto_parallel/tensor_shard/node_handler/addmm_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3519 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/auto_parallel/tensor_shard/node_handler/batch_norm_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     5425 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/auto_parallel/tensor_shard/node_handler/binary_elementwise_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     5270 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/auto_parallel/tensor_shard/node_handler/bmm_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6009 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/auto_parallel/tensor_shard/node_handler/conv_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3028 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/auto_parallel/tensor_shard/node_handler/default_reshape_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    12452 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/auto_parallel/tensor_shard/node_handler/embedding_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/auto_parallel/tensor_shard/node_handler/getattr_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/auto_parallel/tensor_shard/node_handler/getitem_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/auto_parallel/tensor_shard/node_handler/layer_norm_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    14746 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/auto_parallel/tensor_shard/node_handler/linear_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    20532 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/auto_parallel/tensor_shard/node_handler/matmul_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    16519 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/auto_parallel/tensor_shard/node_handler/node_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/auto_parallel/tensor_shard/node_handler/normal_pooling_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/auto_parallel/tensor_shard/node_handler/output_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2999 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/auto_parallel/tensor_shard/node_handler/permute_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/auto_parallel/tensor_shard/node_handler/placeholder_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/auto_parallel/tensor_shard/node_handler/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/auto_parallel/tensor_shard/node_handler/softmax_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2237 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/auto_parallel/tensor_shard/node_handler/split_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 00:21:10.744050 colossalai-nightly-2023.7.1/colossalai/auto_parallel/tensor_shard/node_handler/strategy/
--rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/auto_parallel/tensor_shard/node_handler/strategy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14859 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/auto_parallel/tensor_shard/node_handler/strategy/batch_norm_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5258 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/auto_parallel/tensor_shard/node_handler/strategy/binary_elementwise_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)    24314 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/auto_parallel/tensor_shard/node_handler/strategy/conv_strategy_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)    12308 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/auto_parallel/tensor_shard/node_handler/strategy/embedding_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3597 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/auto_parallel/tensor_shard/node_handler/strategy/getattr_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7524 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/auto_parallel/tensor_shard/node_handler/strategy/getitem_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     9295 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/auto_parallel/tensor_shard/node_handler/strategy/layer_norm_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)    43503 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/auto_parallel/tensor_shard/node_handler/strategy/matmul_strategy_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5524 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/auto_parallel/tensor_shard/node_handler/strategy/normal_pooling_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4733 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/auto_parallel/tensor_shard/node_handler/strategy/output_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3727 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/auto_parallel/tensor_shard/node_handler/strategy/placeholder_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)    19134 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/auto_parallel/tensor_shard/node_handler/strategy/reshape_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5041 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/auto_parallel/tensor_shard/node_handler/strategy/softmax_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)    13270 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/auto_parallel/tensor_shard/node_handler/strategy/strategy_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5400 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/auto_parallel/tensor_shard/node_handler/strategy/sum_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2509 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/auto_parallel/tensor_shard/node_handler/strategy/tensor_constructor_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4033 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/auto_parallel/tensor_shard/node_handler/strategy/unary_elementwise_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4201 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/auto_parallel/tensor_shard/node_handler/strategy/where_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/auto_parallel/tensor_shard/node_handler/sum_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/auto_parallel/tensor_shard/node_handler/tensor_constructor_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/auto_parallel/tensor_shard/node_handler/transpose_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/auto_parallel/tensor_shard/node_handler/unary_elementwise_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/auto_parallel/tensor_shard/node_handler/view_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3835 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/auto_parallel/tensor_shard/node_handler/where_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/auto_parallel/tensor_shard/options.py
--rw-r--r--   0 runner    (1001) docker     (123)    10911 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/auto_parallel/tensor_shard/sharding_strategy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 00:21:10.744050 colossalai-nightly-2023.7.1/colossalai/auto_parallel/tensor_shard/solver/
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/auto_parallel/tensor_shard/solver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9989 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/auto_parallel/tensor_shard/solver/cost_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     5784 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/auto_parallel/tensor_shard/solver/graph_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)    20520 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/auto_parallel/tensor_shard/solver/solver.py
--rw-r--r--   0 runner    (1001) docker     (123)     9158 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/auto_parallel/tensor_shard/solver/strategies_constructor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 00:21:10.744050 colossalai-nightly-2023.7.1/colossalai/auto_parallel/tensor_shard/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/auto_parallel/tensor_shard/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6015 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/auto_parallel/tensor_shard/utils/broadcast.py
--rw-r--r--   0 runner    (1001) docker     (123)     8432 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/auto_parallel/tensor_shard/utils/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     3837 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/auto_parallel/tensor_shard/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     9116 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/auto_parallel/tensor_shard/utils/reshape.py
--rw-r--r--   0 runner    (1001) docker     (123)     4530 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/auto_parallel/tensor_shard/utils/sharding.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 00:21:10.744050 colossalai-nightly-2023.7.1/colossalai/booster/
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/booster/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/booster/accelerator.py
--rw-r--r--   0 runner    (1001) docker     (123)    12659 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/booster/booster.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 00:21:10.748051 colossalai-nightly-2023.7.1/colossalai/booster/mixed_precision/
--rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/booster/mixed_precision/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/booster/mixed_precision/bf16.py
--rw-r--r--   0 runner    (1001) docker     (123)     3301 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/booster/mixed_precision/fp16_apex.py
--rw-r--r--   0 runner    (1001) docker     (123)      918 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/booster/mixed_precision/fp16_naive.py
--rw-r--r--   0 runner    (1001) docker     (123)     5083 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/booster/mixed_precision/fp16_torch.py
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/booster/mixed_precision/fp8.py
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/booster/mixed_precision/mixed_precision_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 00:21:10.748051 colossalai-nightly-2023.7.1/colossalai/booster/plugin/
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/booster/plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3177 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/booster/plugin/dp_plugin_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    14223 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/booster/plugin/gemini_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     9752 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/booster/plugin/low_level_zero_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/booster/plugin/plugin_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6820 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/booster/plugin/torch_ddp_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     8877 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/booster/plugin/torch_fsdp_plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 00:21:10.748051 colossalai-nightly-2023.7.1/colossalai/builder/
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/builder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3013 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/builder/builder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 00:21:10.748051 colossalai-nightly-2023.7.1/colossalai/checkpoint_io/
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/checkpoint_io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15019 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/checkpoint_io/checkpoint_io_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     9094 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/checkpoint_io/general_checkpoint_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     5758 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/checkpoint_io/index_file.py
--rw-r--r--   0 runner    (1001) docker     (123)    21396 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/checkpoint_io/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 00:21:10.748051 colossalai-nightly-2023.7.1/colossalai/cli/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 00:21:10.748051 colossalai-nightly-2023.7.1/colossalai/cli/benchmark/
--rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/cli/benchmark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4240 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/cli/benchmark/benchmark.py
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/cli/benchmark/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     4864 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/cli/benchmark/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 00:21:10.748051 colossalai-nightly-2023.7.1/colossalai/cli/check/
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/cli/check/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8495 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/cli/check/check_installation.py
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/cli/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 00:21:10.748051 colossalai-nightly-2023.7.1/colossalai/cli/launcher/
--rw-r--r--   0 runner    (1001) docker     (123)     3764 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/cli/launcher/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3457 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/cli/launcher/hostinfo.py
--rw-r--r--   0 runner    (1001) docker     (123)     4295 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/cli/launcher/multinode_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)    10169 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/cli/launcher/run.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 00:21:10.748051 colossalai-nightly-2023.7.1/colossalai/cluster/
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/cluster/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4207 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/cluster/device_mesh_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     7307 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/cluster/dist_coordinator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/cluster/process_group_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 00:21:10.748051 colossalai-nightly-2023.7.1/colossalai/communication/
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/communication/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11446 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/communication/collective.py
--rw-r--r--   0 runner    (1001) docker     (123)    19462 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/communication/p2p.py
--rw-r--r--   0 runner    (1001) docker     (123)     9013 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/communication/p2p_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/communication/ring.py
--rw-r--r--   0 runner    (1001) docker     (123)     5095 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/communication/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 00:21:10.748051 colossalai-nightly-2023.7.1/colossalai/context/
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/context/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3152 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/context/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4649 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/context/moe_context.py
--rw-r--r--   0 runner    (1001) docker     (123)    23924 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/context/parallel_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/context/parallel_mode.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 00:21:10.752050 colossalai-nightly-2023.7.1/colossalai/context/process_group_initializer/
--rw-r--r--   0 runner    (1001) docker     (123)      730 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/context/process_group_initializer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/context/process_group_initializer/initializer_1d.py
--rw-r--r--   0 runner    (1001) docker     (123)     6239 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/context/process_group_initializer/initializer_2d.py
--rw-r--r--   0 runner    (1001) docker     (123)    12842 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/context/process_group_initializer/initializer_2p5d.py
--rw-r--r--   0 runner    (1001) docker     (123)    13259 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/context/process_group_initializer/initializer_3d.py
--rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/context/process_group_initializer/initializer_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/context/process_group_initializer/initializer_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/context/process_group_initializer/initializer_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     4092 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/context/process_group_initializer/initializer_sequence.py
--rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/context/process_group_initializer/initializer_tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/context/process_group_initializer/process_group_initializer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 00:21:10.752050 colossalai-nightly-2023.7.1/colossalai/context/random/
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/context/random/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5169 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/context/random/_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3372 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/context/random/seed_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/context/singleton_meta.py
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 00:21:10.752050 colossalai-nightly-2023.7.1/colossalai/device/
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/device/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17420 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/device/alpha_beta_profiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     5691 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/device/calc_pipeline_strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)    11473 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/device/device_mesh.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 00:21:10.752050 colossalai-nightly-2023.7.1/colossalai/engine/
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7864 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/engine/_base_engine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 00:21:10.752050 colossalai-nightly-2023.7.1/colossalai/engine/gradient_accumulation/
--rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/engine/gradient_accumulation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10256 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/engine/gradient_accumulation/_gradient_accumulation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 00:21:10.752050 colossalai-nightly-2023.7.1/colossalai/engine/gradient_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/engine/gradient_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      763 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/engine/gradient_handler/_base_gradient_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/engine/gradient_handler/_data_parallel_gradient_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/engine/gradient_handler/_moe_gradient_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2378 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/engine/gradient_handler/_pipeline_parallel_gradient_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/engine/gradient_handler/_sequence_parallel_gradient_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/engine/gradient_handler/_zero_gradient_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/engine/gradient_handler/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 00:21:10.752050 colossalai-nightly-2023.7.1/colossalai/engine/schedule/
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/engine/schedule/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5875 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/engine/schedule/_base_schedule.py
--rw-r--r--   0 runner    (1001) docker     (123)     3876 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/engine/schedule/_non_pipeline_schedule.py
--rw-r--r--   0 runner    (1001) docker     (123)    41258 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/engine/schedule/_pipeline_schedule.py
--rw-r--r--   0 runner    (1001) docker     (123)     7511 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/engine/schedule/_pipeline_schedule_v2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 00:21:10.752050 colossalai-nightly-2023.7.1/colossalai/fx/
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/fx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/fx/_compatibility.py
--rw-r--r--   0 runner    (1001) docker     (123)    19408 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/fx/_meta_regist_12.py
--rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/fx/_meta_regist_13.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 00:21:10.752050 colossalai-nightly-2023.7.1/colossalai/fx/codegen/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/fx/codegen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    44753 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/fx/codegen/activation_checkpoint_codegen.py
--rw-r--r--   0 runner    (1001) docker     (123)     7373 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/fx/graph_module.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 00:21:10.756050 colossalai-nightly-2023.7.1/colossalai/fx/passes/
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/fx/passes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13583 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/fx/passes/adding_split_node_pass.py
--rw-r--r--   0 runner    (1001) docker     (123)    12179 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/fx/passes/concrete_info_prop.py
--rw-r--r--   0 runner    (1001) docker     (123)    13967 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/fx/passes/meta_info_prop.py
--rw-r--r--   0 runner    (1001) docker     (123)    16288 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/fx/passes/passes_for_gpt2_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6821 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/fx/passes/shard_1d_pass.py
--rw-r--r--   0 runner    (1001) docker     (123)    14022 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/fx/passes/split_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     6160 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/fx/passes/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 00:21:10.756050 colossalai-nightly-2023.7.1/colossalai/fx/profiler/
--rw-r--r--   0 runner    (1001) docker     (123)      695 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/fx/profiler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/fx/profiler/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     6315 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/fx/profiler/dataflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 00:21:10.756050 colossalai-nightly-2023.7.1/colossalai/fx/profiler/experimental/
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/fx/profiler/experimental/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/fx/profiler/experimental/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     7047 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/fx/profiler/experimental/profiler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 00:21:10.756050 colossalai-nightly-2023.7.1/colossalai/fx/profiler/experimental/profiler_function/
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/fx/profiler/experimental/profiler_function/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/fx/profiler/experimental/profiler_function/activation_function.py
--rw-r--r--   0 runner    (1001) docker     (123)     3475 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/fx/profiler/experimental/profiler_function/arithmetic.py
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/fx/profiler/experimental/profiler_function/embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/fx/profiler/experimental/profiler_function/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/fx/profiler/experimental/profiler_function/normalization.py
--rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/fx/profiler/experimental/profiler_function/pooling.py
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/fx/profiler/experimental/profiler_function/python_ops.py
--rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/fx/profiler/experimental/profiler_function/torch_ops.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 00:21:10.756050 colossalai-nightly-2023.7.1/colossalai/fx/profiler/experimental/profiler_module/
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/fx/profiler/experimental/profiler_module/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/fx/profiler/experimental/profiler_module/activation_function.py
--rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/fx/profiler/experimental/profiler_module/attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     6632 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/fx/profiler/experimental/profiler_module/convolution.py
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/fx/profiler/experimental/profiler_module/dropout.py
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/fx/profiler/experimental/profiler_module/embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/fx/profiler/experimental/profiler_module/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/fx/profiler/experimental/profiler_module/normalization.py
--rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/fx/profiler/experimental/profiler_module/pooling.py
--rw-r--r--   0 runner    (1001) docker     (123)     3034 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/fx/profiler/experimental/profiler_module/rnn.py
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/fx/profiler/experimental/profiler_module/torch_op.py
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/fx/profiler/experimental/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/fx/profiler/experimental/shard_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/fx/profiler/memory_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    13226 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/fx/profiler/opcount.py
--rw-r--r--   0 runner    (1001) docker     (123)    15387 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/fx/profiler/profiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4235 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/fx/profiler/shard_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5011 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/fx/profiler/tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4041 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/fx/proxy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 00:21:10.760050 colossalai-nightly-2023.7.1/colossalai/fx/tracer/
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/fx/tracer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4825 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/fx/tracer/_meta_trace.py
--rw-r--r--   0 runner    (1001) docker     (123)     2197 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/fx/tracer/_symbolic_trace.py
--rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/fx/tracer/_tracer_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 00:21:10.760050 colossalai-nightly-2023.7.1/colossalai/fx/tracer/bias_addition_patch/
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/fx/tracer/bias_addition_patch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 00:21:10.760050 colossalai-nightly-2023.7.1/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_function/
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_function/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_function/addbmm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_function/addmm.py
--rw-r--r--   0 runner    (1001) docker     (123)     4471 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_function/bias_addition_function.py
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_function/linear.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 00:21:10.760050 colossalai-nightly-2023.7.1/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_module/
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_module/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4421 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_module/bias_addition_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_module/conv.py
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_module/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)    26969 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/fx/tracer/experimental.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 00:21:10.760050 colossalai-nightly-2023.7.1/colossalai/fx/tracer/meta_patch/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/fx/tracer/meta_patch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 00:21:10.760050 colossalai-nightly-2023.7.1/colossalai/fx/tracer/meta_patch/patched_function/
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/fx/tracer/meta_patch/patched_function/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/fx/tracer/meta_patch/patched_function/activation_function.py
--rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/fx/tracer/meta_patch/patched_function/arithmetic.py
--rw-r--r--   0 runner    (1001) docker     (123)     5762 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/fx/tracer/meta_patch/patched_function/convolution.py
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/fx/tracer/meta_patch/patched_function/embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/fx/tracer/meta_patch/patched_function/normalization.py
--rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/fx/tracer/meta_patch/patched_function/python_ops.py
--rw-r--r--   0 runner    (1001) docker     (123)     5753 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/fx/tracer/meta_patch/patched_function/torch_ops.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 00:21:10.760050 colossalai-nightly-2023.7.1/colossalai/fx/tracer/meta_patch/patched_module/
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/fx/tracer/meta_patch/patched_module/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/fx/tracer/meta_patch/patched_module/activation_function.py
--rw-r--r--   0 runner    (1001) docker     (123)     4674 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/fx/tracer/meta_patch/patched_module/convolution.py
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/fx/tracer/meta_patch/patched_module/embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/fx/tracer/meta_patch/patched_module/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/fx/tracer/meta_patch/patched_module/normalization.py
--rw-r--r--   0 runner    (1001) docker     (123)     6769 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/fx/tracer/meta_patch/patched_module/pooling.py
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/fx/tracer/meta_patch/patched_module/rnn.py
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/fx/tracer/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)    24624 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/fx/tracer/tracer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/global_variables.py
--rw-r--r--   0 runner    (1001) docker     (123)    21027 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/initialize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 00:21:10.760050 colossalai-nightly-2023.7.1/colossalai/interface/
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/interface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/interface/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3922 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/interface/optimizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 00:21:10.760050 colossalai-nightly-2023.7.1/colossalai/kernel/
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/kernel/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 00:21:10.760050 colossalai-nightly-2023.7.1/colossalai/kernel/cuda_native/
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/kernel/cuda_native/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 00:21:10.764050 colossalai-nightly-2023.7.1/colossalai/kernel/cuda_native/csrc/
--rw-r--r--   0 runner    (1001) docker     (123)     2606 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/kernel/cuda_native/csrc/colossal_C_frontend.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/kernel/cuda_native/csrc/compat.h
--rw-r--r--   0 runner    (1001) docker     (123)    16815 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/kernel/cuda_native/csrc/cpu_adam.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5187 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/kernel/cuda_native/csrc/cpu_adam.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 00:21:10.764050 colossalai-nightly-2023.7.1/colossalai/kernel/cuda_native/csrc/kernels/
--rw-r--r--   0 runner    (1001) docker     (123)     7526 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/kernel/cuda_native/csrc/kernels/cross_entropy.cu
--rw-r--r--   0 runner    (1001) docker     (123)     3767 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/kernel/cuda_native/csrc/kernels/cublas_wrappers.cu
--rw-r--r--   0 runner    (1001) docker     (123)     5441 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/kernel/cuda_native/csrc/kernels/cuda_util.cu
--rw-r--r--   0 runner    (1001) docker     (123)    37586 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/kernel/cuda_native/csrc/kernels/dropout_kernels.cu
--rw-r--r--   0 runner    (1001) docker     (123)     7653 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/kernel/cuda_native/csrc/kernels/general_kernels.cu
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 00:21:10.764050 colossalai-nightly-2023.7.1/colossalai/kernel/cuda_native/csrc/kernels/include/
--rw-r--r--   0 runner    (1001) docker     (123)     8585 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/kernel/cuda_native/csrc/kernels/include/block_reduce.h
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/kernel/cuda_native/csrc/kernels/include/context.h
--rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/kernel/cuda_native/csrc/kernels/include/cross_entropy_layer.h
--rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/kernel/cuda_native/csrc/kernels/include/cublas_wrappers.h
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/kernel/cuda_native/csrc/kernels/include/cuda_util.h
--rw-r--r--   0 runner    (1001) docker     (123)     3415 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/kernel/cuda_native/csrc/kernels/include/dropout.h
--rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/kernel/cuda_native/csrc/kernels/include/feed_forward.h
--rw-r--r--   0 runner    (1001) docker     (123)     9260 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/kernel/cuda_native/csrc/kernels/include/kernels.h
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/kernel/cuda_native/csrc/kernels/include/ls_cub.cuh
--rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/kernel/cuda_native/csrc/kernels/include/normalize_layer.h
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/kernel/cuda_native/csrc/kernels/include/softmax.h
--rw-r--r--   0 runner    (1001) docker     (123)     3043 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/kernel/cuda_native/csrc/kernels/include/strided_batch_gemm.h
--rw-r--r--   0 runner    (1001) docker     (123)    48403 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/kernel/cuda_native/csrc/kernels/normalize_kernels.cu
--rw-r--r--   0 runner    (1001) docker     (123)    13619 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/kernel/cuda_native/csrc/kernels/softmax_kernels.cu
--rw-r--r--   0 runner    (1001) docker     (123)    10953 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/kernel/cuda_native/csrc/kernels/transform_kernels.cu
--rw-r--r--   0 runner    (1001) docker     (123)     4877 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/kernel/cuda_native/csrc/layer_norm_cuda.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    25828 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/kernel/cuda_native/csrc/layer_norm_cuda_kernel.cu
--rw-r--r--   0 runner    (1001) docker     (123)     4003 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/kernel/cuda_native/csrc/moe_cuda.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    26286 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/kernel/cuda_native/csrc/moe_cuda_kernel.cu
--rw-r--r--   0 runner    (1001) docker     (123)     5046 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/kernel/cuda_native/csrc/multi_tensor_adam.cu
--rw-r--r--   0 runner    (1001) docker     (123)     5200 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/kernel/cuda_native/csrc/multi_tensor_apply.cuh
--rw-r--r--   0 runner    (1001) docker     (123)    13278 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/kernel/cuda_native/csrc/multi_tensor_l2norm_kernel.cu
--rw-r--r--   0 runner    (1001) docker     (123)    13114 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/kernel/cuda_native/csrc/multi_tensor_lamb.cu
--rw-r--r--   0 runner    (1001) docker     (123)     4439 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/kernel/cuda_native/csrc/multi_tensor_scale_kernel.cu
--rw-r--r--   0 runner    (1001) docker     (123)     6478 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/kernel/cuda_native/csrc/multi_tensor_sgd_kernel.cu
--rw-r--r--   0 runner    (1001) docker     (123)    16988 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/kernel/cuda_native/csrc/multihead_attention_1d.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4701 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/kernel/cuda_native/csrc/multihead_attention_1d.h
--rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/kernel/cuda_native/csrc/scaled_masked_softmax.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    21701 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/kernel/cuda_native/csrc/scaled_masked_softmax.h
--rw-r--r--   0 runner    (1001) docker     (123)     3467 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/kernel/cuda_native/csrc/scaled_masked_softmax_cuda.cu
--rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/kernel/cuda_native/csrc/scaled_upper_triang_masked_softmax.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    22850 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/kernel/cuda_native/csrc/scaled_upper_triang_masked_softmax.h
--rw-r--r--   0 runner    (1001) docker     (123)     2818 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/kernel/cuda_native/csrc/scaled_upper_triang_masked_softmax_cuda.cu
--rw-r--r--   0 runner    (1001) docker     (123)    14851 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/kernel/cuda_native/csrc/type_shim.h
--rw-r--r--   0 runner    (1001) docker     (123)    24864 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/kernel/cuda_native/flash_attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/kernel/cuda_native/layer_norm.py
--rw-r--r--   0 runner    (1001) docker     (123)    10754 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/kernel/cuda_native/multihead_attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     6715 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/kernel/cuda_native/scaled_softmax.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 00:21:10.768051 colossalai-nightly-2023.7.1/colossalai/kernel/jit/
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/kernel/jit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/kernel/jit/bias_dropout_add.py
--rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/kernel/jit/bias_gelu.py
--rw-r--r--   0 runner    (1001) docker     (123)     3477 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/kernel/jit/option.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 00:21:10.768051 colossalai-nightly-2023.7.1/colossalai/kernel/op_builder/
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/kernel/op_builder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8943 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/kernel/op_builder/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/kernel/op_builder/cpu_adam.py
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/kernel/op_builder/fused_optim.py
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/kernel/op_builder/layernorm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/kernel/op_builder/moe.py
--rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/kernel/op_builder/multi_head_attn.py
--rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/kernel/op_builder/scaled_masked_softmax.py
--rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/kernel/op_builder/scaled_upper_triangle_masked_softmax.py
--rw-r--r--   0 runner    (1001) docker     (123)     8210 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/kernel/op_builder/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 00:21:10.768051 colossalai-nightly-2023.7.1/colossalai/lazy/
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/lazy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23336 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/lazy/lazy_init.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 00:21:10.768051 colossalai-nightly-2023.7.1/colossalai/logging/
--rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/logging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7511 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/logging/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 00:21:10.768051 colossalai-nightly-2023.7.1/colossalai/nn/
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/nn/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 00:21:10.768051 colossalai-nightly-2023.7.1/colossalai/nn/_ops/
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/nn/_ops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8713 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/nn/_ops/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4153 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/nn/_ops/addmm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/nn/_ops/batch_norm.py
--rw-r--r--   0 runner    (1001) docker     (123)     9289 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/nn/_ops/element_wise.py
--rw-r--r--   0 runner    (1001) docker     (123)     6666 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/nn/_ops/embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)     6607 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/nn/_ops/embedding_bag.py
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/nn/_ops/layernorm.py
--rw-r--r--   0 runner    (1001) docker     (123)     7122 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/nn/_ops/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)     2641 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/nn/_ops/loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     3143 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/nn/_ops/view.py
--rw-r--r--   0 runner    (1001) docker     (123)     9552 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/nn/init.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 00:21:10.768051 colossalai-nightly-2023.7.1/colossalai/nn/layer/
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/nn/layer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2845 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/nn/layer/base_layer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 00:21:10.768051 colossalai-nightly-2023.7.1/colossalai/nn/layer/colossalai_layer/
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/nn/layer/colossalai_layer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/nn/layer/colossalai_layer/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      992 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/nn/layer/colossalai_layer/dropout.py
--rw-r--r--   0 runner    (1001) docker     (123)     6304 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/nn/layer/colossalai_layer/embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)     5375 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/nn/layer/colossalai_layer/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/nn/layer/colossalai_layer/normalization.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 00:21:10.768051 colossalai-nightly-2023.7.1/colossalai/nn/layer/moe/
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/nn/layer/moe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5557 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/nn/layer/moe/_operation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/nn/layer/moe/checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     8241 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/nn/layer/moe/experts.py
--rw-r--r--   0 runner    (1001) docker     (123)     9431 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/nn/layer/moe/layers.py
--rw-r--r--   0 runner    (1001) docker     (123)    10066 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/nn/layer/moe/routers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/nn/layer/moe/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 00:21:10.772050 colossalai-nightly-2023.7.1/colossalai/nn/layer/parallel_1d/
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/nn/layer/parallel_1d/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3796 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/nn/layer/parallel_1d/_operation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5048 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/nn/layer/parallel_1d/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    49753 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/nn/layer/parallel_1d/layers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 00:21:10.772050 colossalai-nightly-2023.7.1/colossalai/nn/layer/parallel_2d/
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/nn/layer/parallel_2d/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    34900 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/nn/layer/parallel_2d/_operation.py
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/nn/layer/parallel_2d/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    50524 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/nn/layer/parallel_2d/layers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 00:21:10.772050 colossalai-nightly-2023.7.1/colossalai/nn/layer/parallel_2p5d/
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/nn/layer/parallel_2p5d/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    37643 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/nn/layer/parallel_2p5d/_operation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/nn/layer/parallel_2p5d/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    50769 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/nn/layer/parallel_2p5d/layers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 00:21:10.772050 colossalai-nightly-2023.7.1/colossalai/nn/layer/parallel_3d/
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/nn/layer/parallel_3d/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    22769 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/nn/layer/parallel_3d/_operation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2967 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/nn/layer/parallel_3d/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    51441 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/nn/layer/parallel_3d/layers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 00:21:10.772050 colossalai-nightly-2023.7.1/colossalai/nn/layer/parallel_sequence/
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/nn/layer/parallel_sequence/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6411 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/nn/layer/parallel_sequence/_operation.py
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/nn/layer/parallel_sequence/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    10754 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/nn/layer/parallel_sequence/layers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 00:21:10.772050 colossalai-nightly-2023.7.1/colossalai/nn/layer/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/nn/layer/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/nn/layer/utils/common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 00:21:10.772050 colossalai-nightly-2023.7.1/colossalai/nn/layer/vanilla/
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/nn/layer/vanilla/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14535 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/nn/layer/vanilla/layers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 00:21:10.772050 colossalai-nightly-2023.7.1/colossalai/nn/layer/wrapper/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/nn/layer/wrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2133 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/nn/layer/wrapper/pipeline_wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 00:21:10.772050 colossalai-nightly-2023.7.1/colossalai/nn/loss/
--rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/nn/loss/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4693 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/nn/loss/loss_1d.py
--rw-r--r--   0 runner    (1001) docker     (123)     5728 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/nn/loss/loss_2d.py
--rw-r--r--   0 runner    (1001) docker     (123)     5536 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/nn/loss/loss_2p5d.py
--rw-r--r--   0 runner    (1001) docker     (123)     6362 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/nn/loss/loss_3d.py
--rw-r--r--   0 runner    (1001) docker     (123)     3249 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/nn/loss/loss_moe.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 00:21:10.772050 colossalai-nightly-2023.7.1/colossalai/nn/lr_scheduler/
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/nn/lr_scheduler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6171 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/nn/lr_scheduler/cosine.py
--rw-r--r--   0 runner    (1001) docker     (123)     7800 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/nn/lr_scheduler/delayed.py
--rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/nn/lr_scheduler/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)     2867 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/nn/lr_scheduler/multistep.py
--rw-r--r--   0 runner    (1001) docker     (123)     5319 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/nn/lr_scheduler/onecycle.py
--rw-r--r--   0 runner    (1001) docker     (123)     2686 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/nn/lr_scheduler/poly.py
--rw-r--r--   0 runner    (1001) docker     (123)     3687 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/nn/lr_scheduler/torch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 00:21:10.776050 colossalai-nightly-2023.7.1/colossalai/nn/metric/
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/nn/metric/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/nn/metric/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/nn/metric/accuracy_2d.py
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/nn/metric/accuracy_2p5d.py
--rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/nn/metric/accuracy_3d.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 00:21:10.776050 colossalai-nightly-2023.7.1/colossalai/nn/optimizer/
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/nn/optimizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/nn/optimizer/colossalai_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     8234 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/nn/optimizer/cpu_adam.py
--rw-r--r--   0 runner    (1001) docker     (123)     6385 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/nn/optimizer/fused_adam.py
--rw-r--r--   0 runner    (1001) docker     (123)     8926 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/nn/optimizer/fused_lamb.py
--rw-r--r--   0 runner    (1001) docker     (123)     6094 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/nn/optimizer/fused_sgd.py
--rw-r--r--   0 runner    (1001) docker     (123)     7338 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/nn/optimizer/hybrid_adam.py
--rw-r--r--   0 runner    (1001) docker     (123)     4495 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/nn/optimizer/lamb.py
--rw-r--r--   0 runner    (1001) docker     (123)     3784 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/nn/optimizer/lars.py
--rw-r--r--   0 runner    (1001) docker     (123)     6778 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/nn/optimizer/nvme_optimizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 00:21:10.776050 colossalai-nightly-2023.7.1/colossalai/nn/parallel/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/nn/parallel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6575 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/nn/parallel/data_parallel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 00:21:10.776050 colossalai-nightly-2023.7.1/colossalai/nn/parallel/layers/
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/nn/parallel/layers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 00:21:10.776050 colossalai-nightly-2023.7.1/colossalai/nn/parallel/layers/cache_embedding/
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/nn/parallel/layers/cache_embedding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/nn/parallel/layers/cache_embedding/base_embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)    28600 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/nn/parallel/layers/cache_embedding/cache_mgr.py
--rw-r--r--   0 runner    (1001) docker     (123)     8828 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/nn/parallel/layers/cache_embedding/cached_embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/nn/parallel/layers/cache_embedding/copyer.py
--rw-r--r--   0 runner    (1001) docker     (123)      855 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/nn/parallel/layers/cache_embedding/embedding_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5922 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/nn/parallel/layers/cache_embedding/parallel_cached_embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)    10057 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/nn/parallel/layers/cache_embedding/parallel_cached_embedding_tablewise.py
--rw-r--r--   0 runner    (1001) docker     (123)     7481 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/nn/parallel/layers/cache_embedding/parallel_cached_embedding_tablewise_split_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/nn/parallel/layers/colo_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/nn/parallel/layers/embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/nn/parallel/layers/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)     4816 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/nn/parallel/layers/module_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3875 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/nn/parallel/reducer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 00:21:10.776050 colossalai-nightly-2023.7.1/colossalai/pipeline/
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/pipeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/pipeline/layer_spec.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 00:21:10.776050 colossalai-nightly-2023.7.1/colossalai/pipeline/middleware/
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/pipeline/middleware/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 00:21:10.776050 colossalai-nightly-2023.7.1/colossalai/pipeline/middleware/adaptor/
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/pipeline/middleware/adaptor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6154 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/pipeline/middleware/adaptor/fx.py
--rw-r--r--   0 runner    (1001) docker     (123)     7051 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/pipeline/middleware/topo.py
--rw-r--r--   0 runner    (1001) docker     (123)    11415 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/pipeline/pipelinable.py
--rw-r--r--   0 runner    (1001) docker     (123)     5857 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/pipeline/pipeline_process_group.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 00:21:10.776050 colossalai-nightly-2023.7.1/colossalai/pipeline/rpc/
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/pipeline/rpc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    59170 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/pipeline/rpc/_pipeline_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    14859 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/pipeline/rpc/_pipeline_schedule.py
--rw-r--r--   0 runner    (1001) docker     (123)     5460 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/pipeline/rpc/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9012 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/pipeline/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 00:21:10.780050 colossalai-nightly-2023.7.1/colossalai/registry/
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/registry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3054 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/registry/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 00:21:10.780050 colossalai-nightly-2023.7.1/colossalai/tensor/
--rw-r--r--   0 runner    (1001) docker     (123)      946 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/tensor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4449 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/tensor/colo_parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)    13185 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/tensor/colo_tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)    22269 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/tensor/comm_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/tensor/compute_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/tensor/const.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 00:21:10.780050 colossalai-nightly-2023.7.1/colossalai/tensor/d_tensor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/tensor/d_tensor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11876 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/tensor/d_tensor/comm_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)     4944 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/tensor/d_tensor/d_tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2863 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/tensor/d_tensor/layout.py
--rw-r--r--   0 runner    (1001) docker     (123)    25229 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/tensor/d_tensor/layout_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/tensor/d_tensor/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     9277 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/tensor/d_tensor/sharding_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)     3268 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/tensor/d_tensor/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8688 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/tensor/dist_spec_mgr.py
--rw-r--r--   0 runner    (1001) docker     (123)     2715 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/tensor/distspec.py
--rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/tensor/op_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     6127 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/tensor/param_op_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)    10365 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/tensor/process_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    36501 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/tensor/shape_consistency.py
--rw-r--r--   0 runner    (1001) docker     (123)    11620 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/tensor/sharding_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/tensor/tensor_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)     8443 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/tensor/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 00:21:10.780050 colossalai-nightly-2023.7.1/colossalai/testing/
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/testing/comparison.py
--rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/testing/pytest_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/testing/random.py
--rw-r--r--   0 runner    (1001) docker     (123)     8629 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/testing/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 00:21:10.780050 colossalai-nightly-2023.7.1/colossalai/trainer/
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/trainer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14776 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/trainer/_trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 00:21:10.780050 colossalai-nightly-2023.7.1/colossalai/trainer/hooks/
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/trainer/hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/trainer/hooks/_base_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     3247 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/trainer/hooks/_checkpoint_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/trainer/hooks/_commons_.py
--rw-r--r--   0 runner    (1001) docker     (123)    13106 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/trainer/hooks/_log_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/trainer/hooks/_lr_scheduler_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)    16131 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/trainer/hooks/_metric_hook.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 00:21:10.784050 colossalai-nightly-2023.7.1/colossalai/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9856 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/utils/activation_checkpoint.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 00:21:10.784050 colossalai-nightly-2023.7.1/colossalai/utils/checkpoint/
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/utils/checkpoint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5521 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/utils/checkpoint/module_checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/utils/checkpoint/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 00:21:10.784050 colossalai-nightly-2023.7.1/colossalai/utils/checkpoint_io/
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/utils/checkpoint_io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/utils/checkpoint_io/backend.py
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/utils/checkpoint_io/constant.py
--rw-r--r--   0 runner    (1001) docker     (123)     9794 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/utils/checkpoint_io/convertor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5971 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/utils/checkpoint_io/distributed.py
--rw-r--r--   0 runner    (1001) docker     (123)     7008 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/utils/checkpoint_io/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/utils/checkpoint_io/meta.py
--rw-r--r--   0 runner    (1001) docker     (123)     4813 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/utils/checkpoint_io/reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     8908 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/utils/checkpoint_io/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3966 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/utils/checkpoint_io/writer.py
--rw-r--r--   0 runner    (1001) docker     (123)    11400 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/utils/checkpointing.py
--rw-r--r--   0 runner    (1001) docker     (123)    17450 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/utils/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/utils/cuda.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 00:21:10.784050 colossalai-nightly-2023.7.1/colossalai/utils/data_sampler/
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/utils/data_sampler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/utils/data_sampler/base_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     7128 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/utils/data_sampler/data_parallel_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6425 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/utils/memory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 00:21:10.784050 colossalai-nightly-2023.7.1/colossalai/utils/model/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/utils/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/utils/model/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/utils/moe.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 00:21:10.784050 colossalai-nightly-2023.7.1/colossalai/utils/multi_tensor_apply/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/utils/multi_tensor_apply/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/utils/multi_tensor_apply/multi_tensor_apply.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 00:21:10.784050 colossalai-nightly-2023.7.1/colossalai/utils/profiler/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/utils/profiler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/utils/profiler/extention.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 00:21:10.784050 colossalai-nightly-2023.7.1/colossalai/utils/profiler/legacy/
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/utils/profiler/legacy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10914 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/utils/profiler/legacy/comm_profiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     5050 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/utils/profiler/legacy/pcie_profiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3896 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/utils/profiler/legacy/prof_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8616 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/utils/profiler/profiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3998 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/utils/profiler/stateful_tensor_mem_extention.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 00:21:10.784050 colossalai-nightly-2023.7.1/colossalai/utils/rank_recorder/
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/utils/rank_recorder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5528 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/utils/rank_recorder/rank_recorder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 00:21:10.784050 colossalai-nightly-2023.7.1/colossalai/utils/tensor_detector/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/utils/tensor_detector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8651 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/utils/tensor_detector/tensor_detector.py
--rw-r--r--   0 runner    (1001) docker     (123)     4279 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/utils/timer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 00:21:10.784050 colossalai-nightly-2023.7.1/colossalai/zero/
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/zero/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 00:21:10.784050 colossalai-nightly-2023.7.1/colossalai/zero/gemini/
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/zero/gemini/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 00:21:10.788051 colossalai-nightly-2023.7.1/colossalai/zero/gemini/chunk/
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/zero/gemini/chunk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22079 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/zero/gemini/chunk/chunk.py
--rw-r--r--   0 runner    (1001) docker     (123)     9531 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/zero/gemini/chunk/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     6714 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/zero/gemini/chunk/search_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/zero/gemini/chunk/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7515 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/zero/gemini/colo_init_context.py
--rw-r--r--   0 runner    (1001) docker     (123)    37822 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/zero/gemini/gemini_ddp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2395 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/zero/gemini/gemini_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     6627 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/zero/gemini/gemini_mgr.py
--rw-r--r--   0 runner    (1001) docker     (123)    14838 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/zero/gemini/gemini_optimizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 00:21:10.788051 colossalai-nightly-2023.7.1/colossalai/zero/gemini/memory_tracer/
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/zero/gemini/memory_tracer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/zero/gemini/memory_tracer/chunk_memstats_collector.py
--rw-r--r--   0 runner    (1001) docker     (123)     3980 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/zero/gemini/memory_tracer/memory_monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4111 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/zero/gemini/memory_tracer/memory_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     3582 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/zero/gemini/memory_tracer/memstats_collector.py
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/zero/gemini/memory_tracer/param_runtime_order.py
--rw-r--r--   0 runner    (1001) docker     (123)     3738 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/zero/gemini/memory_tracer/runtime_mem_tracer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4233 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/zero/gemini/memory_tracer/static_memstats_collector.py
--rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/zero/gemini/memory_tracer/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    10482 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/zero/gemini/placement_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)     4168 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/zero/gemini/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 00:21:10.788051 colossalai-nightly-2023.7.1/colossalai/zero/legacy/
--rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/zero/legacy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 00:21:10.788051 colossalai-nightly-2023.7.1/colossalai/zero/legacy/gemini/
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/zero/legacy/gemini/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/zero/legacy/gemini/gemini_context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 00:21:10.788051 colossalai-nightly-2023.7.1/colossalai/zero/legacy/gemini/ophooks/
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/zero/legacy/gemini/ophooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/zero/legacy/gemini/ophooks/_shard_grad_ophook.py
--rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/zero/legacy/gemini/ophooks/_shard_param_ophook.py
--rw-r--r--   0 runner    (1001) docker     (123)     5161 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/zero/legacy/gemini/ophooks/runtime_mem_tracer_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     4814 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/zero/legacy/gemini/ophooks/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 00:21:10.788051 colossalai-nightly-2023.7.1/colossalai/zero/legacy/gemini/paramhooks/
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/zero/legacy/gemini/paramhooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/zero/legacy/gemini/paramhooks/_param_hookmgr.py
--rw-r--r--   0 runner    (1001) docker     (123)     6927 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/zero/legacy/gemini/stateful_tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4252 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/zero/legacy/gemini/stateful_tensor_mgr.py
--rw-r--r--   0 runner    (1001) docker     (123)     6449 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/zero/legacy/gemini/tensor_placement_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)     3984 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/zero/legacy/gemini/tensor_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 00:21:10.788051 colossalai-nightly-2023.7.1/colossalai/zero/legacy/init_ctx/
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/zero/legacy/init_ctx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11385 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/zero/legacy/init_ctx/init_context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 00:21:10.788051 colossalai-nightly-2023.7.1/colossalai/zero/legacy/shard_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/zero/legacy/shard_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/zero/legacy/shard_utils/base_shard_strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2217 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/zero/legacy/shard_utils/bucket_tensor_shard_strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/zero/legacy/shard_utils/commons.py
--rw-r--r--   0 runner    (1001) docker     (123)     2642 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/zero/legacy/shard_utils/tensor_shard_strategy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 00:21:10.788051 colossalai-nightly-2023.7.1/colossalai/zero/legacy/sharded_model/
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/zero/legacy/sharded_model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/zero/legacy/sharded_model/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8357 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/zero/legacy/sharded_model/reduce_scatter.py
--rw-r--r--   0 runner    (1001) docker     (123)    29261 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/zero/legacy/sharded_model/sharded_model_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/zero/legacy/sharded_model/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4846 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/zero/legacy/sharded_model/zero_hook.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 00:21:10.788051 colossalai-nightly-2023.7.1/colossalai/zero/legacy/sharded_optim/
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/zero/legacy/sharded_optim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19215 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/zero/legacy/sharded_optim/sharded_optim_v2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 00:21:10.788051 colossalai-nightly-2023.7.1/colossalai/zero/legacy/sharded_param/
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/zero/legacy/sharded_param/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3869 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/zero/legacy/sharded_param/sharded_param.py
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/zero/legacy/sharded_param/sharded_tensor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 00:21:10.792050 colossalai-nightly-2023.7.1/colossalai/zero/low_level/
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/zero/low_level/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9957 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/zero/low_level/_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 00:21:10.792050 colossalai-nightly-2023.7.1/colossalai/zero/low_level/bookkeeping/
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/zero/low_level/bookkeeping/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/zero/low_level/bookkeeping/base_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/zero/low_level/bookkeeping/bucket_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     2896 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/zero/low_level/bookkeeping/gradient_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     3353 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/zero/low_level/bookkeeping/parameter_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/zero/low_level/bookkeeping/tensor_bucket.py
--rw-r--r--   0 runner    (1001) docker     (123)    26595 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/zero/low_level/low_level_optim.py
--rw-r--r--   0 runner    (1001) docker     (123)     5176 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/colossalai/zero/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 00:21:10.792050 colossalai-nightly-2023.7.1/colossalai_nightly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    25399 2023-07-01 00:21:10.000000 colossalai-nightly-2023.7.1/colossalai_nightly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    37585 2023-07-01 00:21:10.000000 colossalai-nightly-2023.7.1/colossalai_nightly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 00:21:10.000000 colossalai-nightly-2023.7.1/colossalai_nightly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-01 00:21:10.000000 colossalai-nightly-2023.7.1/colossalai_nightly.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-01 00:21:10.000000 colossalai-nightly-2023.7.1/colossalai_nightly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-01 00:21:10.000000 colossalai-nightly-2023.7.1/colossalai_nightly.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 00:21:10.792050 colossalai-nightly-2023.7.1/op_builder/
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/op_builder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8943 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/op_builder/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/op_builder/cpu_adam.py
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/op_builder/fused_optim.py
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/op_builder/layernorm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/op_builder/moe.py
--rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/op_builder/multi_head_attn.py
--rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/op_builder/scaled_masked_softmax.py
--rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/op_builder/scaled_upper_triangle_masked_softmax.py
--rw-r--r--   0 runner    (1001) docker     (123)     8210 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/op_builder/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 00:21:10.792050 colossalai-nightly-2023.7.1/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/requirements/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/requirements/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-01 00:21:10.800050 colossalai-nightly-2023.7.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     6229 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 00:21:10.732051 colossalai-nightly-2023.7.1/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 00:21:10.792050 colossalai-nightly-2023.7.1/tests/components_to_test/
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/tests/components_to_test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2469 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/tests/components_to_test/albert.py
--rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/tests/components_to_test/beit.py
--rw-r--r--   0 runner    (1001) docker     (123)     3270 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/tests/components_to_test/bert.py
--rw-r--r--   0 runner    (1001) docker     (123)     2857 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/tests/components_to_test/gpt2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/tests/components_to_test/hanging_param_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/tests/components_to_test/inline_op_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/tests/components_to_test/nested_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/tests/components_to_test/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/tests/components_to_test/repeated_computed_layers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/tests/components_to_test/resnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/tests/components_to_test/simple_net.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 00:21:10.792050 colossalai-nightly-2023.7.1/tests/components_to_test/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/tests/components_to_test/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/tests/components_to_test/utils/dummy_data_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/tests/components_to_test/utils/executor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 00:21:10.792050 colossalai-nightly-2023.7.1/tests/kit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/tests/kit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 00:21:10.792050 colossalai-nightly-2023.7.1/tests/kit/model_zoo/
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/tests/kit/model_zoo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 00:21:10.792050 colossalai-nightly-2023.7.1/tests/kit/model_zoo/diffusers/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/tests/kit/model_zoo/diffusers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2825 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/tests/kit/model_zoo/diffusers/diffusers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/tests/kit/model_zoo/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 00:21:10.796050 colossalai-nightly-2023.7.1/tests/kit/model_zoo/timm/
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/tests/kit/model_zoo/timm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7513 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/tests/kit/model_zoo/timm/timm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 00:21:10.796050 colossalai-nightly-2023.7.1/tests/kit/model_zoo/torchaudio/
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/tests/kit/model_zoo/torchaudio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5409 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/tests/kit/model_zoo/torchaudio/torchaudio.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 00:21:10.796050 colossalai-nightly-2023.7.1/tests/kit/model_zoo/torchrec/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/tests/kit/model_zoo/torchrec/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4634 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/tests/kit/model_zoo/torchrec/torchrec.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 00:21:10.796050 colossalai-nightly-2023.7.1/tests/kit/model_zoo/torchvision/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/tests/kit/model_zoo/torchvision/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5931 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/tests/kit/model_zoo/torchvision/torchvision.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 00:21:10.796050 colossalai-nightly-2023.7.1/tests/kit/model_zoo/transformers/
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/tests/kit/model_zoo/transformers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4023 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/tests/kit/model_zoo/transformers/albert.py
--rw-r--r--   0 runner    (1001) docker     (123)     4335 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/tests/kit/model_zoo/transformers/bert.py
--rw-r--r--   0 runner    (1001) docker     (123)     2767 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/tests/kit/model_zoo/transformers/gpt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/tests/kit/model_zoo/transformers/opt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/tests/kit/model_zoo/transformers/t5.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 00:21:10.796050 colossalai-nightly-2023.7.1/tests/test_analyzer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/tests/test_analyzer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 00:21:10.796050 colossalai-nightly-2023.7.1/tests/test_analyzer/test_fx/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/tests/test_analyzer/test_fx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4330 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/tests/test_analyzer/test_fx/test_bias_addition.py
--rw-r--r--   0 runner    (1001) docker     (123)     2735 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/tests/test_analyzer/test_fx/test_mod_dir.py
--rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/tests/test_analyzer/test_fx/test_nested_ckpt.py
--rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/tests/test_analyzer/test_fx/test_shape_prop.py
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/tests/test_analyzer/test_fx/test_symbolic_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/tests/test_analyzer/test_fx/zoo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 00:21:10.796050 colossalai-nightly-2023.7.1/tests/test_analyzer/test_subclasses/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/tests/test_analyzer/test_subclasses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3644 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/tests/test_analyzer/test_subclasses/test_aten.py
--rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/tests/test_analyzer/test_subclasses/test_flop_tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/tests/test_analyzer/test_subclasses/test_meta_mode.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 00:21:10.796050 colossalai-nightly-2023.7.1/tests/test_auto_parallel/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/tests/test_auto_parallel/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 00:21:10.796050 colossalai-nightly-2023.7.1/tests/test_auto_parallel/test_pass/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/tests/test_auto_parallel/test_pass/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/tests/test_auto_parallel/test_pass/test_node_converting_pass.py
--rw-r--r--   0 runner    (1001) docker     (123)     2283 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/tests/test_auto_parallel/test_pass/test_size_value_converting_pass.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 00:21:10.796050 colossalai-nightly-2023.7.1/tests/test_auto_parallel/test_tensor_shard/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/tests/test_auto_parallel/test_tensor_shard/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2842 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/tests/test_auto_parallel/test_tensor_shard/test_bias_addition_forward.py
--rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/tests/test_auto_parallel/test_tensor_shard/test_broadcast.py
--rw-r--r--   0 runner    (1001) docker     (123)     2417 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/tests/test_auto_parallel/test_tensor_shard/test_checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3521 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/tests/test_auto_parallel/test_tensor_shard/test_compatibility_with_ddp.py
--rw-r--r--   0 runner    (1001) docker     (123)     4172 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/tests/test_auto_parallel/test_tensor_shard/test_compatibility_with_gemini.py
--rw-r--r--   0 runner    (1001) docker     (123)     3747 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/tests/test_auto_parallel/test_tensor_shard/test_find_repeat_block.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 00:21:10.796050 colossalai-nightly-2023.7.1/tests/test_auto_parallel/test_tensor_shard/test_gpt/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/tests/test_auto_parallel/test_tensor_shard/test_gpt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11050 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/tests/test_auto_parallel/test_tensor_shard/test_gpt/gpt_modules.py
--rw-r--r--   0 runner    (1001) docker     (123)     7786 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/tests/test_auto_parallel/test_tensor_shard/test_gpt/test_runtime_with_gpt_modules.py
--rw-r--r--   0 runner    (1001) docker     (123)     3932 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/tests/test_auto_parallel/test_tensor_shard/test_gpt/test_solver_with_gpt_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/tests/test_auto_parallel/test_tensor_shard/test_liveness_analysis.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 00:21:10.800050 colossalai-nightly-2023.7.1/tests/test_auto_parallel/test_tensor_shard/test_node_handler/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/tests/test_auto_parallel/test_tensor_shard/test_node_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11552 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_addbmm_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     7693 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_addmm_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4842 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_batch_norm_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6740 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_bias_linear_function_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     6205 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_bias_linear_module_node.py
--rw-r--r--   0 runner    (1001) docker     (123)    10993 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_binary_elementwise_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     9001 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_bmm_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    12886 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_conv_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3734 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_default_reshape_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    11802 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_embedding_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3003 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_getattr_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     8173 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_getitem_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4372 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_layer_norm_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    13108 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_linear_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     8356 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_matmul_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_norm_pooling_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2623 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_output_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    18730 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_permute_and_transpose_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3153 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_placeholder_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4263 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_shard_option.py
--rw-r--r--   0 runner    (1001) docker     (123)     9001 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_softmax_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    12527 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_split_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    12380 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_sum_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_tensor_constructor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3762 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_unary_element_wise_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    14158 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_view_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_where_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     8918 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/tests/test_auto_parallel/test_tensor_shard/test_node_handler/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5325 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/tests/test_auto_parallel/test_tensor_shard/test_solver_with_resnet_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-01 00:20:59.000000 colossalai-nightly-2023.7.1/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:20.026470 colossalai-nightly-2023.7.8/
+-rw-r--r--   0 runner    (1001) docker     (123)    22244 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    25399 2023-07-08 00:17:20.026470 colossalai-nightly-2023.7.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    20789 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.926462 colossalai-nightly-2023.7.8/colossalai/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.926462 colossalai-nightly-2023.7.8/colossalai/_C/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/_C/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.926462 colossalai-nightly-2023.7.8/colossalai/_analyzer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/_analyzer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.926462 colossalai-nightly-2023.7.8/colossalai/_analyzer/_subclasses/
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/_analyzer/_subclasses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20609 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/_analyzer/_subclasses/_meta_registration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/_analyzer/_subclasses/_monkey_patch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18694 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/_analyzer/_subclasses/flop_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7667 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/_analyzer/_subclasses/meta_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/_analyzer/envs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.926462 colossalai-nightly-2023.7.8/colossalai/_analyzer/fx/
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/_analyzer/fx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18761 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/_analyzer/fx/codegen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9920 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/_analyzer/fx/graph_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8526 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/_analyzer/fx/node_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.926462 colossalai-nightly-2023.7.8/colossalai/_analyzer/fx/passes/
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/_analyzer/fx/passes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12600 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/_analyzer/fx/passes/graph_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9892 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/_analyzer/fx/passes/shape_prop.py
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/_analyzer/fx/symbolic_profile.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.926462 colossalai-nightly-2023.7.8/colossalai/_analyzer/fx/tracer/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/_analyzer/fx/tracer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6512 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/_analyzer/fx/tracer/bias_addition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/_analyzer/fx/tracer/custom_leaf_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3651 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/_analyzer/fx/tracer/proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6048 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/_analyzer/fx/tracer/symbolic_trace.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15758 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/_analyzer/fx/tracer/tracer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.926462 colossalai-nightly-2023.7.8/colossalai/amp/
+-rw-r--r--   0 runner    (1001) docker     (123)     2313 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/amp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/amp/amp_type.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.930462 colossalai-nightly-2023.7.8/colossalai/amp/apex_amp/
+-rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/amp/apex_amp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/amp/apex_amp/apex_amp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.930462 colossalai-nightly-2023.7.8/colossalai/amp/naive_amp/
+-rw-r--r--   0 runner    (1001) docker     (123)     2422 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/amp/naive_amp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13454 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/amp/naive_amp/_fp16_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/amp/naive_amp/_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.930462 colossalai-nightly-2023.7.8/colossalai/amp/naive_amp/grad_scaler/
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/amp/naive_amp/grad_scaler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/amp/naive_amp/grad_scaler/base_grad_scaler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/amp/naive_amp/grad_scaler/constant_grad_scaler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4755 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/amp/naive_amp/grad_scaler/dynamic_grad_scaler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.930462 colossalai-nightly-2023.7.8/colossalai/amp/naive_amp/mixed_precision_mixin/
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/amp/naive_amp/mixed_precision_mixin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2596 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/amp/naive_amp/mixed_precision_mixin/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/amp/naive_amp/mixed_precision_mixin/bf16.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/amp/naive_amp/mixed_precision_mixin/fp16.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6098 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/amp/naive_amp/naive_amp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.930462 colossalai-nightly-2023.7.8/colossalai/amp/torch_amp/
+-rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/amp/torch_amp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26520 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/amp/torch_amp/_grad_scaler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3344 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/amp/torch_amp/torch_amp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.930462 colossalai-nightly-2023.7.8/colossalai/auto_parallel/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.930462 colossalai-nightly-2023.7.8/colossalai/auto_parallel/checkpoint/
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/checkpoint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/checkpoint/build_c_ext.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7716 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/checkpoint/ckpt_solver_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3469 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/checkpoint/ckpt_solver_chen.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18543 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/checkpoint/ckpt_solver_rotor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4938 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/checkpoint/operation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.930462 colossalai-nightly-2023.7.8/colossalai/auto_parallel/meta_profiler/
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/meta_profiler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/meta_profiler/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.934462 colossalai-nightly-2023.7.8/colossalai/auto_parallel/meta_profiler/meta_registry/
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/meta_profiler/meta_registry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4050 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/meta_profiler/meta_registry/activation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2824 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/meta_profiler/meta_registry/binary_elementwise_ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7900 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/meta_profiler/meta_registry/conv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/meta_profiler/meta_registry/embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25633 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/meta_profiler/meta_registry/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/meta_profiler/meta_registry/non_spmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9721 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/meta_profiler/meta_registry/norm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7399 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/meta_profiler/meta_registry/pooling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3363 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/meta_profiler/meta_registry/tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2968 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/meta_profiler/meta_registry/where.py
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/meta_profiler/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4847 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/meta_profiler/shard_metainfo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.934462 colossalai-nightly-2023.7.8/colossalai/auto_parallel/offload/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/offload/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7001 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/offload/amp_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3618 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/offload/base_offload_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2127 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/offload/mem_optimize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5134 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/offload/region.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20381 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/offload/region_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10128 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/offload/runtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18888 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/offload/solver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18549 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/offload/training_simulator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2966 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/offload/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.934462 colossalai-nightly-2023.7.8/colossalai/auto_parallel/passes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/passes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5214 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/passes/comm_metainfo_pass.py
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/passes/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6030 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/passes/meta_info_prop.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12067 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/passes/runtime_apply_pass.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22686 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/passes/runtime_preparation_pass.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.934462 colossalai-nightly-2023.7.8/colossalai/auto_parallel/pipeline_shard/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/pipeline_shard/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.934462 colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2662 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18744 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/initialize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.938463 colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4187 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/addmm_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3519 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/batch_norm_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5425 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/binary_elementwise_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5270 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/bmm_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6009 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/conv_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3028 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/default_reshape_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12452 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/embedding_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/getattr_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/getitem_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/layer_norm_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14746 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/linear_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20532 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/matmul_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16514 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/node_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/normal_pooling_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/output_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2999 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/permute_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/placeholder_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/softmax_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2237 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/split_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.942463 colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/strategy/
+-rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/strategy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14859 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/strategy/batch_norm_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5258 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/strategy/binary_elementwise_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24314 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/strategy/conv_strategy_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12308 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/strategy/embedding_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3597 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/strategy/getattr_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7524 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/strategy/getitem_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9295 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/strategy/layer_norm_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43483 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/strategy/matmul_strategy_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5524 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/strategy/normal_pooling_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4733 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/strategy/output_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3727 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/strategy/placeholder_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19134 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/strategy/reshape_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5041 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/strategy/softmax_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13270 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/strategy/strategy_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5400 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/strategy/sum_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2509 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/strategy/tensor_constructor_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4033 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/strategy/unary_elementwise_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4201 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/strategy/where_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/sum_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/tensor_constructor_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/transpose_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/unary_elementwise_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/view_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3835 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/where_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10911 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/sharding_strategy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.942463 colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/solver/
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/solver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9989 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/solver/cost_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5784 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/solver/graph_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20520 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/solver/solver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9158 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/solver/strategies_constructor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.942463 colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6015 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/utils/broadcast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8432 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/utils/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3827 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9116 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/utils/reshape.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4530 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/utils/sharding.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.942463 colossalai-nightly-2023.7.8/colossalai/booster/
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/booster/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/booster/accelerator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12659 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/booster/booster.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.946463 colossalai-nightly-2023.7.8/colossalai/booster/mixed_precision/
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/booster/mixed_precision/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/booster/mixed_precision/bf16.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3301 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/booster/mixed_precision/fp16_apex.py
+-rw-r--r--   0 runner    (1001) docker     (123)      918 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/booster/mixed_precision/fp16_naive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5083 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/booster/mixed_precision/fp16_torch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/booster/mixed_precision/fp8.py
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/booster/mixed_precision/mixed_precision_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.946463 colossalai-nightly-2023.7.8/colossalai/booster/plugin/
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/booster/plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3177 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/booster/plugin/dp_plugin_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15137 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/booster/plugin/gemini_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9752 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/booster/plugin/low_level_zero_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/booster/plugin/plugin_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6820 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/booster/plugin/torch_ddp_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8877 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/booster/plugin/torch_fsdp_plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.946463 colossalai-nightly-2023.7.8/colossalai/builder/
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/builder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3013 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/builder/builder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.946463 colossalai-nightly-2023.7.8/colossalai/checkpoint_io/
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/checkpoint_io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15021 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/checkpoint_io/checkpoint_io_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9263 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/checkpoint_io/general_checkpoint_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5758 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/checkpoint_io/index_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22100 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/checkpoint_io/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.946463 colossalai-nightly-2023.7.8/colossalai/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.946463 colossalai-nightly-2023.7.8/colossalai/cli/benchmark/
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/cli/benchmark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4240 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/cli/benchmark/benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/cli/benchmark/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4864 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/cli/benchmark/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.946463 colossalai-nightly-2023.7.8/colossalai/cli/check/
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/cli/check/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8495 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/cli/check/check_installation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/cli/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.950464 colossalai-nightly-2023.7.8/colossalai/cli/launcher/
+-rw-r--r--   0 runner    (1001) docker     (123)     3764 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/cli/launcher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3457 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/cli/launcher/hostinfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4295 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/cli/launcher/multinode_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10034 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/cli/launcher/run.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.950464 colossalai-nightly-2023.7.8/colossalai/cluster/
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/cluster/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4207 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/cluster/device_mesh_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7307 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/cluster/dist_coordinator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/cluster/process_group_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.950464 colossalai-nightly-2023.7.8/colossalai/communication/
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/communication/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11446 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/communication/collective.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19462 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/communication/p2p.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9013 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/communication/p2p_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/communication/ring.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5095 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/communication/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.950464 colossalai-nightly-2023.7.8/colossalai/context/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/context/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3152 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/context/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4649 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/context/moe_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23924 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/context/parallel_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/context/parallel_mode.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.950464 colossalai-nightly-2023.7.8/colossalai/context/process_group_initializer/
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/context/process_group_initializer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/context/process_group_initializer/initializer_1d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6239 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/context/process_group_initializer/initializer_2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12842 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/context/process_group_initializer/initializer_2p5d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13259 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/context/process_group_initializer/initializer_3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/context/process_group_initializer/initializer_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/context/process_group_initializer/initializer_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/context/process_group_initializer/initializer_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4092 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/context/process_group_initializer/initializer_sequence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/context/process_group_initializer/initializer_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/context/process_group_initializer/process_group_initializer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.954464 colossalai-nightly-2023.7.8/colossalai/context/random/
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/context/random/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5169 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/context/random/_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3372 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/context/random/seed_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/context/singleton_meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.954464 colossalai-nightly-2023.7.8/colossalai/device/
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/device/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17420 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/device/alpha_beta_profiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5691 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/device/calc_pipeline_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23687 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/device/device_mesh.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.954464 colossalai-nightly-2023.7.8/colossalai/engine/
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7864 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/engine/_base_engine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.954464 colossalai-nightly-2023.7.8/colossalai/engine/gradient_accumulation/
+-rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/engine/gradient_accumulation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10256 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/engine/gradient_accumulation/_gradient_accumulation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.954464 colossalai-nightly-2023.7.8/colossalai/engine/gradient_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/engine/gradient_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/engine/gradient_handler/_base_gradient_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/engine/gradient_handler/_data_parallel_gradient_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/engine/gradient_handler/_moe_gradient_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2378 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/engine/gradient_handler/_pipeline_parallel_gradient_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/engine/gradient_handler/_sequence_parallel_gradient_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/engine/gradient_handler/_zero_gradient_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/engine/gradient_handler/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.958464 colossalai-nightly-2023.7.8/colossalai/engine/schedule/
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/engine/schedule/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5875 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/engine/schedule/_base_schedule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3876 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/engine/schedule/_non_pipeline_schedule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41258 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/engine/schedule/_pipeline_schedule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7511 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/engine/schedule/_pipeline_schedule_v2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.958464 colossalai-nightly-2023.7.8/colossalai/fx/
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/_compatibility.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19408 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/_meta_regist_12.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/_meta_regist_13.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.958464 colossalai-nightly-2023.7.8/colossalai/fx/codegen/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/codegen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44753 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/codegen/activation_checkpoint_codegen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7373 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/graph_module.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.958464 colossalai-nightly-2023.7.8/colossalai/fx/passes/
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/passes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13583 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/passes/adding_split_node_pass.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12179 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/passes/concrete_info_prop.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13967 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/passes/meta_info_prop.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16288 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/passes/passes_for_gpt2_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6821 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/passes/shard_1d_pass.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14022 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/passes/split_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6160 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/passes/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.958464 colossalai-nightly-2023.7.8/colossalai/fx/profiler/
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/profiler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/profiler/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6315 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/profiler/dataflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.962465 colossalai-nightly-2023.7.8/colossalai/fx/profiler/experimental/
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/profiler/experimental/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/profiler/experimental/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7047 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/profiler/experimental/profiler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.962465 colossalai-nightly-2023.7.8/colossalai/fx/profiler/experimental/profiler_function/
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/profiler/experimental/profiler_function/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/profiler/experimental/profiler_function/activation_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3475 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/profiler/experimental/profiler_function/arithmetic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/profiler/experimental/profiler_function/embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/profiler/experimental/profiler_function/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/profiler/experimental/profiler_function/normalization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/profiler/experimental/profiler_function/pooling.py
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/profiler/experimental/profiler_function/python_ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/profiler/experimental/profiler_function/torch_ops.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.962465 colossalai-nightly-2023.7.8/colossalai/fx/profiler/experimental/profiler_module/
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/profiler/experimental/profiler_module/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/profiler/experimental/profiler_module/activation_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/profiler/experimental/profiler_module/attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6632 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/profiler/experimental/profiler_module/convolution.py
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/profiler/experimental/profiler_module/dropout.py
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/profiler/experimental/profiler_module/embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/profiler/experimental/profiler_module/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/profiler/experimental/profiler_module/normalization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/profiler/experimental/profiler_module/pooling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3034 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/profiler/experimental/profiler_module/rnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/profiler/experimental/profiler_module/torch_op.py
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/profiler/experimental/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/profiler/experimental/shard_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/profiler/memory_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13226 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/profiler/opcount.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15387 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/profiler/profiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4235 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/profiler/shard_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5011 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/profiler/tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4041 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/proxy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.962465 colossalai-nightly-2023.7.8/colossalai/fx/tracer/
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/tracer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4825 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/tracer/_meta_trace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2197 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/tracer/_symbolic_trace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/tracer/_tracer_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.962465 colossalai-nightly-2023.7.8/colossalai/fx/tracer/bias_addition_patch/
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/tracer/bias_addition_patch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.966465 colossalai-nightly-2023.7.8/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_function/
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_function/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_function/addbmm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_function/addmm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4471 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_function/bias_addition_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_function/linear.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.966465 colossalai-nightly-2023.7.8/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_module/
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_module/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4421 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_module/bias_addition_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_module/conv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_module/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26969 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/tracer/experimental.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.966465 colossalai-nightly-2023.7.8/colossalai/fx/tracer/meta_patch/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/tracer/meta_patch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.966465 colossalai-nightly-2023.7.8/colossalai/fx/tracer/meta_patch/patched_function/
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/tracer/meta_patch/patched_function/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/tracer/meta_patch/patched_function/activation_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/tracer/meta_patch/patched_function/arithmetic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5762 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/tracer/meta_patch/patched_function/convolution.py
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/tracer/meta_patch/patched_function/embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/tracer/meta_patch/patched_function/normalization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/tracer/meta_patch/patched_function/python_ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5753 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/tracer/meta_patch/patched_function/torch_ops.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.966465 colossalai-nightly-2023.7.8/colossalai/fx/tracer/meta_patch/patched_module/
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/tracer/meta_patch/patched_module/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/tracer/meta_patch/patched_module/activation_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4674 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/tracer/meta_patch/patched_module/convolution.py
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/tracer/meta_patch/patched_module/embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/tracer/meta_patch/patched_module/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/tracer/meta_patch/patched_module/normalization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6769 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/tracer/meta_patch/patched_module/pooling.py
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/tracer/meta_patch/patched_module/rnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/tracer/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24624 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/tracer/tracer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/global_variables.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21027 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/initialize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.966465 colossalai-nightly-2023.7.8/colossalai/interface/
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/interface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/interface/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4055 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/interface/optimizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.966465 colossalai-nightly-2023.7.8/colossalai/kernel/
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/kernel/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.966465 colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.970465 colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/
+-rw-r--r--   0 runner    (1001) docker     (123)     2606 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/colossal_C_frontend.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/compat.h
+-rw-r--r--   0 runner    (1001) docker     (123)    16815 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/cpu_adam.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5187 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/cpu_adam.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.970465 colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/kernels/
+-rw-r--r--   0 runner    (1001) docker     (123)     7526 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/kernels/cross_entropy.cu
+-rw-r--r--   0 runner    (1001) docker     (123)     3767 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/kernels/cublas_wrappers.cu
+-rw-r--r--   0 runner    (1001) docker     (123)     5441 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/kernels/cuda_util.cu
+-rw-r--r--   0 runner    (1001) docker     (123)    37586 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/kernels/dropout_kernels.cu
+-rw-r--r--   0 runner    (1001) docker     (123)     7653 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/kernels/general_kernels.cu
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.974466 colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/kernels/include/
+-rw-r--r--   0 runner    (1001) docker     (123)     8585 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/kernels/include/block_reduce.h
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/kernels/include/context.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/kernels/include/cross_entropy_layer.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/kernels/include/cublas_wrappers.h
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/kernels/include/cuda_util.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3415 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/kernels/include/dropout.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/kernels/include/feed_forward.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9260 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/kernels/include/kernels.h
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/kernels/include/ls_cub.cuh
+-rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/kernels/include/normalize_layer.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/kernels/include/softmax.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3043 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/kernels/include/strided_batch_gemm.h
+-rw-r--r--   0 runner    (1001) docker     (123)    48403 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/kernels/normalize_kernels.cu
+-rw-r--r--   0 runner    (1001) docker     (123)    13619 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/kernels/softmax_kernels.cu
+-rw-r--r--   0 runner    (1001) docker     (123)    10953 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/kernels/transform_kernels.cu
+-rw-r--r--   0 runner    (1001) docker     (123)     4877 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/layer_norm_cuda.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    25828 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/layer_norm_cuda_kernel.cu
+-rw-r--r--   0 runner    (1001) docker     (123)     4003 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/moe_cuda.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    26286 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/moe_cuda_kernel.cu
+-rw-r--r--   0 runner    (1001) docker     (123)     5046 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/multi_tensor_adam.cu
+-rw-r--r--   0 runner    (1001) docker     (123)     5200 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/multi_tensor_apply.cuh
+-rw-r--r--   0 runner    (1001) docker     (123)    13278 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/multi_tensor_l2norm_kernel.cu
+-rw-r--r--   0 runner    (1001) docker     (123)    13114 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/multi_tensor_lamb.cu
+-rw-r--r--   0 runner    (1001) docker     (123)     4439 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/multi_tensor_scale_kernel.cu
+-rw-r--r--   0 runner    (1001) docker     (123)     6478 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/multi_tensor_sgd_kernel.cu
+-rw-r--r--   0 runner    (1001) docker     (123)    16988 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/multihead_attention_1d.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4701 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/multihead_attention_1d.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/scaled_masked_softmax.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    21701 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/scaled_masked_softmax.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3467 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/scaled_masked_softmax_cuda.cu
+-rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/scaled_upper_triang_masked_softmax.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    22850 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/scaled_upper_triang_masked_softmax.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2818 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/scaled_upper_triang_masked_softmax_cuda.cu
+-rw-r--r--   0 runner    (1001) docker     (123)    14851 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/type_shim.h
+-rw-r--r--   0 runner    (1001) docker     (123)    24864 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/flash_attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/layer_norm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10754 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/multihead_attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6715 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/scaled_softmax.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.974466 colossalai-nightly-2023.7.8/colossalai/kernel/jit/
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/kernel/jit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      893 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/kernel/jit/bias_dropout_add.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/kernel/jit/bias_gelu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3477 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/kernel/jit/option.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.974466 colossalai-nightly-2023.7.8/colossalai/kernel/op_builder/
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/kernel/op_builder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8943 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/kernel/op_builder/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/kernel/op_builder/cpu_adam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/kernel/op_builder/fused_optim.py
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/kernel/op_builder/layernorm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/kernel/op_builder/moe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/kernel/op_builder/multi_head_attn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/kernel/op_builder/scaled_masked_softmax.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/kernel/op_builder/scaled_upper_triangle_masked_softmax.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8210 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/kernel/op_builder/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.974466 colossalai-nightly-2023.7.8/colossalai/lazy/
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/lazy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23592 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/lazy/lazy_init.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.974466 colossalai-nightly-2023.7.8/colossalai/logging/
+-rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7511 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/logging/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.974466 colossalai-nightly-2023.7.8/colossalai/nn/
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.978466 colossalai-nightly-2023.7.8/colossalai/nn/_ops/
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/_ops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8713 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/_ops/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4153 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/_ops/addmm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/_ops/batch_norm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9289 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/_ops/element_wise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6666 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/_ops/embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6607 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/_ops/embedding_bag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/_ops/layernorm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7122 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/_ops/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2641 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/_ops/loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3143 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/_ops/view.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9552 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/init.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.978466 colossalai-nightly-2023.7.8/colossalai/nn/layer/
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/layer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2846 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/layer/base_layer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.978466 colossalai-nightly-2023.7.8/colossalai/nn/layer/colossalai_layer/
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/layer/colossalai_layer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/layer/colossalai_layer/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/layer/colossalai_layer/dropout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6304 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/layer/colossalai_layer/embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5375 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/layer/colossalai_layer/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/layer/colossalai_layer/normalization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.978466 colossalai-nightly-2023.7.8/colossalai/nn/layer/moe/
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/layer/moe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5557 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/layer/moe/_operation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/layer/moe/checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8241 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/layer/moe/experts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9431 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/layer/moe/layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10066 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/layer/moe/routers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/layer/moe/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.978466 colossalai-nightly-2023.7.8/colossalai/nn/layer/parallel_1d/
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/layer/parallel_1d/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3797 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/layer/parallel_1d/_operation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5048 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/layer/parallel_1d/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49753 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/layer/parallel_1d/layers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.978466 colossalai-nightly-2023.7.8/colossalai/nn/layer/parallel_2d/
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/layer/parallel_2d/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34900 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/layer/parallel_2d/_operation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/layer/parallel_2d/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50524 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/layer/parallel_2d/layers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.978466 colossalai-nightly-2023.7.8/colossalai/nn/layer/parallel_2p5d/
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/layer/parallel_2p5d/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37643 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/layer/parallel_2p5d/_operation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/layer/parallel_2p5d/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50769 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/layer/parallel_2p5d/layers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.982466 colossalai-nightly-2023.7.8/colossalai/nn/layer/parallel_3d/
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/layer/parallel_3d/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    22769 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/layer/parallel_3d/_operation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2967 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/layer/parallel_3d/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51441 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/layer/parallel_3d/layers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.982466 colossalai-nightly-2023.7.8/colossalai/nn/layer/parallel_sequence/
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/layer/parallel_sequence/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6411 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/layer/parallel_sequence/_operation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/layer/parallel_sequence/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10754 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/layer/parallel_sequence/layers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.982466 colossalai-nightly-2023.7.8/colossalai/nn/layer/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/layer/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/layer/utils/common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.982466 colossalai-nightly-2023.7.8/colossalai/nn/layer/vanilla/
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/layer/vanilla/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14535 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/layer/vanilla/layers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.982466 colossalai-nightly-2023.7.8/colossalai/nn/layer/wrapper/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/layer/wrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2133 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/layer/wrapper/pipeline_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.982466 colossalai-nightly-2023.7.8/colossalai/nn/loss/
+-rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/loss/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4693 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/loss/loss_1d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5728 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/loss/loss_2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5536 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/loss/loss_2p5d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6362 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/loss/loss_3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3249 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/loss/loss_moe.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.982466 colossalai-nightly-2023.7.8/colossalai/nn/lr_scheduler/
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/lr_scheduler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6171 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/lr_scheduler/cosine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7800 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/lr_scheduler/delayed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/lr_scheduler/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2867 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/lr_scheduler/multistep.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5319 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/lr_scheduler/onecycle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2686 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/lr_scheduler/poly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3687 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/lr_scheduler/torch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.982466 colossalai-nightly-2023.7.8/colossalai/nn/metric/
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/metric/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/metric/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/metric/accuracy_2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/metric/accuracy_2p5d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/metric/accuracy_3d.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.986467 colossalai-nightly-2023.7.8/colossalai/nn/optimizer/
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/optimizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/optimizer/colossalai_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8234 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/optimizer/cpu_adam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6385 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/optimizer/fused_adam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8926 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/optimizer/fused_lamb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6094 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/optimizer/fused_sgd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7338 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/optimizer/hybrid_adam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4495 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/optimizer/lamb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3784 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/optimizer/lars.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6778 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/optimizer/nvme_optimizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.986467 colossalai-nightly-2023.7.8/colossalai/nn/parallel/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/parallel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6575 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/parallel/data_parallel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.986467 colossalai-nightly-2023.7.8/colossalai/nn/parallel/layers/
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/parallel/layers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.986467 colossalai-nightly-2023.7.8/colossalai/nn/parallel/layers/cache_embedding/
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/parallel/layers/cache_embedding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/parallel/layers/cache_embedding/base_embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28600 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/parallel/layers/cache_embedding/cache_mgr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8828 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/parallel/layers/cache_embedding/cached_embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/parallel/layers/cache_embedding/copyer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/parallel/layers/cache_embedding/embedding_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5922 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/parallel/layers/cache_embedding/parallel_cached_embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10057 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/parallel/layers/cache_embedding/parallel_cached_embedding_tablewise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7481 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/parallel/layers/cache_embedding/parallel_cached_embedding_tablewise_split_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/parallel/layers/colo_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/parallel/layers/embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/parallel/layers/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4816 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/parallel/layers/module_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3875 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/parallel/reducer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.990467 colossalai-nightly-2023.7.8/colossalai/pipeline/
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/pipeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/pipeline/layer_spec.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.990467 colossalai-nightly-2023.7.8/colossalai/pipeline/middleware/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/pipeline/middleware/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.990467 colossalai-nightly-2023.7.8/colossalai/pipeline/middleware/adaptor/
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/pipeline/middleware/adaptor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6154 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/pipeline/middleware/adaptor/fx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7051 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/pipeline/middleware/topo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11415 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/pipeline/pipelinable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5857 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/pipeline/pipeline_process_group.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.990467 colossalai-nightly-2023.7.8/colossalai/pipeline/rpc/
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/pipeline/rpc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59170 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/pipeline/rpc/_pipeline_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14859 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/pipeline/rpc/_pipeline_schedule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5460 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/pipeline/rpc/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9012 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/pipeline/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.990467 colossalai-nightly-2023.7.8/colossalai/registry/
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/registry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3054 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/registry/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.990467 colossalai-nightly-2023.7.8/colossalai/shardformer/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/shardformer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2220 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/shardformer/_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.990467 colossalai-nightly-2023.7.8/colossalai/shardformer/layer/
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/shardformer/layer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9628 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/shardformer/layer/_operation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3544 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/shardformer/layer/dropout.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12750 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/shardformer/layer/embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14617 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/shardformer/layer/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4461 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/shardformer/layer/loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3959 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/shardformer/layer/normalization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8789 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/shardformer/layer/parallel_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20697 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/shardformer/layer/qkv_fused_linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7001 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/shardformer/layer/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.990467 colossalai-nightly-2023.7.8/colossalai/shardformer/modeling/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/shardformer/modeling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3955 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/shardformer/modeling/bloom.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.994467 colossalai-nightly-2023.7.8/colossalai/shardformer/policies/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/shardformer/policies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6168 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/shardformer/policies/autopolicy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6266 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/shardformer/policies/basepolicy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12461 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/shardformer/policies/bert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8385 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/shardformer/policies/bloom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8623 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/shardformer/policies/gpt2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5595 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/shardformer/policies/llama.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6139 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/shardformer/policies/opt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11077 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/shardformer/policies/t5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5183 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/shardformer/policies/vit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.994467 colossalai-nightly-2023.7.8/colossalai/shardformer/shard/
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/shardformer/shard/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/shardformer/shard/shard_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7140 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/shardformer/shard/sharder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/shardformer/shard/shardformer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.994467 colossalai-nightly-2023.7.8/colossalai/tensor/
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/tensor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4449 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/tensor/colo_parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13185 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/tensor/colo_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21790 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/tensor/comm_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/tensor/compute_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/tensor/const.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.994467 colossalai-nightly-2023.7.8/colossalai/tensor/d_tensor/
+-rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/tensor/d_tensor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14992 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/tensor/d_tensor/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11262 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/tensor/d_tensor/comm_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2736 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/tensor/d_tensor/layout.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24565 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/tensor/d_tensor/layout_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/tensor/d_tensor/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9277 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/tensor/d_tensor/sharding_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3263 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/tensor/d_tensor/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8688 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/tensor/dist_spec_mgr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2715 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/tensor/distspec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/tensor/op_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6127 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/tensor/param_op_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10365 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/tensor/process_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36486 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/tensor/shape_consistency.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11605 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/tensor/sharding_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/tensor/tensor_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8443 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/tensor/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.998468 colossalai-nightly-2023.7.8/colossalai/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5605 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/testing/comparison.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/testing/pytest_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/testing/random.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8629 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/testing/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.998468 colossalai-nightly-2023.7.8/colossalai/trainer/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/trainer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14776 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/trainer/_trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.998468 colossalai-nightly-2023.7.8/colossalai/trainer/hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/trainer/hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/trainer/hooks/_base_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3247 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/trainer/hooks/_checkpoint_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/trainer/hooks/_commons_.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13106 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/trainer/hooks/_log_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/trainer/hooks/_lr_scheduler_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16131 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/trainer/hooks/_metric_hook.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.998468 colossalai-nightly-2023.7.8/colossalai/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9856 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/utils/activation_checkpoint.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.998468 colossalai-nightly-2023.7.8/colossalai/utils/checkpoint/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/utils/checkpoint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5521 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/utils/checkpoint/module_checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/utils/checkpoint/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.998468 colossalai-nightly-2023.7.8/colossalai/utils/checkpoint_io/
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/utils/checkpoint_io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/utils/checkpoint_io/backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/utils/checkpoint_io/constant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9794 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/utils/checkpoint_io/convertor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5971 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/utils/checkpoint_io/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7008 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/utils/checkpoint_io/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/utils/checkpoint_io/meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4813 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/utils/checkpoint_io/reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8908 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/utils/checkpoint_io/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3966 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/utils/checkpoint_io/writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11400 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/utils/checkpointing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17450 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/utils/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/utils/cuda.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:20.002468 colossalai-nightly-2023.7.8/colossalai/utils/data_sampler/
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/utils/data_sampler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/utils/data_sampler/base_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7128 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/utils/data_sampler/data_parallel_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6425 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/utils/memory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:20.002468 colossalai-nightly-2023.7.8/colossalai/utils/model/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/utils/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/utils/model/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/utils/moe.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:20.002468 colossalai-nightly-2023.7.8/colossalai/utils/multi_tensor_apply/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/utils/multi_tensor_apply/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/utils/multi_tensor_apply/multi_tensor_apply.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:20.002468 colossalai-nightly-2023.7.8/colossalai/utils/profiler/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/utils/profiler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/utils/profiler/extention.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:20.002468 colossalai-nightly-2023.7.8/colossalai/utils/profiler/legacy/
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/utils/profiler/legacy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10914 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/utils/profiler/legacy/comm_profiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5050 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/utils/profiler/legacy/pcie_profiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3896 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/utils/profiler/legacy/prof_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8616 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/utils/profiler/profiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3998 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/utils/profiler/stateful_tensor_mem_extention.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:20.002468 colossalai-nightly-2023.7.8/colossalai/utils/rank_recorder/
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/utils/rank_recorder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5528 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/utils/rank_recorder/rank_recorder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:20.002468 colossalai-nightly-2023.7.8/colossalai/utils/tensor_detector/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/utils/tensor_detector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8651 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/utils/tensor_detector/tensor_detector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4279 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/utils/timer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:20.002468 colossalai-nightly-2023.7.8/colossalai/zero/
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/zero/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:20.002468 colossalai-nightly-2023.7.8/colossalai/zero/gemini/
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/zero/gemini/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:20.006468 colossalai-nightly-2023.7.8/colossalai/zero/gemini/chunk/
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/zero/gemini/chunk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22079 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/zero/gemini/chunk/chunk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9531 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/zero/gemini/chunk/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6714 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/zero/gemini/chunk/search_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/zero/gemini/chunk/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7515 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/zero/gemini/colo_init_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37822 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/zero/gemini/gemini_ddp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2395 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/zero/gemini/gemini_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6627 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/zero/gemini/gemini_mgr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29879 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/zero/gemini/gemini_optimizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:20.006468 colossalai-nightly-2023.7.8/colossalai/zero/gemini/memory_tracer/
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/zero/gemini/memory_tracer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/zero/gemini/memory_tracer/chunk_memstats_collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3980 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/zero/gemini/memory_tracer/memory_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4111 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/zero/gemini/memory_tracer/memory_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3582 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/zero/gemini/memory_tracer/memstats_collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/zero/gemini/memory_tracer/param_runtime_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3738 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/zero/gemini/memory_tracer/runtime_mem_tracer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4233 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/zero/gemini/memory_tracer/static_memstats_collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/zero/gemini/memory_tracer/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10482 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/zero/gemini/placement_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4168 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/zero/gemini/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:20.006468 colossalai-nightly-2023.7.8/colossalai/zero/legacy/
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/zero/legacy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:20.006468 colossalai-nightly-2023.7.8/colossalai/zero/legacy/gemini/
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/zero/legacy/gemini/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/zero/legacy/gemini/gemini_context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:20.006468 colossalai-nightly-2023.7.8/colossalai/zero/legacy/gemini/ophooks/
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/zero/legacy/gemini/ophooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/zero/legacy/gemini/ophooks/_shard_grad_ophook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/zero/legacy/gemini/ophooks/_shard_param_ophook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5161 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/zero/legacy/gemini/ophooks/runtime_mem_tracer_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4814 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/zero/legacy/gemini/ophooks/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:20.006468 colossalai-nightly-2023.7.8/colossalai/zero/legacy/gemini/paramhooks/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/zero/legacy/gemini/paramhooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/zero/legacy/gemini/paramhooks/_param_hookmgr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6927 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/zero/legacy/gemini/stateful_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4252 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/zero/legacy/gemini/stateful_tensor_mgr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6449 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/zero/legacy/gemini/tensor_placement_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3984 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/zero/legacy/gemini/tensor_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:20.006468 colossalai-nightly-2023.7.8/colossalai/zero/legacy/init_ctx/
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/zero/legacy/init_ctx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11385 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/zero/legacy/init_ctx/init_context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:20.006468 colossalai-nightly-2023.7.8/colossalai/zero/legacy/shard_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/zero/legacy/shard_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/zero/legacy/shard_utils/base_shard_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2217 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/zero/legacy/shard_utils/bucket_tensor_shard_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/zero/legacy/shard_utils/commons.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2642 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/zero/legacy/shard_utils/tensor_shard_strategy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:20.010469 colossalai-nightly-2023.7.8/colossalai/zero/legacy/sharded_model/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/zero/legacy/sharded_model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/zero/legacy/sharded_model/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8357 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/zero/legacy/sharded_model/reduce_scatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29261 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/zero/legacy/sharded_model/sharded_model_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/zero/legacy/sharded_model/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4846 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/zero/legacy/sharded_model/zero_hook.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:20.010469 colossalai-nightly-2023.7.8/colossalai/zero/legacy/sharded_optim/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/zero/legacy/sharded_optim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19215 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/zero/legacy/sharded_optim/sharded_optim_v2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:20.010469 colossalai-nightly-2023.7.8/colossalai/zero/legacy/sharded_param/
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/zero/legacy/sharded_param/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3869 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/zero/legacy/sharded_param/sharded_param.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/zero/legacy/sharded_param/sharded_tensor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:20.010469 colossalai-nightly-2023.7.8/colossalai/zero/low_level/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/zero/low_level/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9957 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/zero/low_level/_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:20.010469 colossalai-nightly-2023.7.8/colossalai/zero/low_level/bookkeeping/
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/zero/low_level/bookkeeping/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/zero/low_level/bookkeeping/base_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/zero/low_level/bookkeeping/bucket_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2896 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/zero/low_level/bookkeeping/gradient_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3353 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/zero/low_level/bookkeeping/parameter_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/zero/low_level/bookkeeping/tensor_bucket.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26595 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/zero/low_level/low_level_optim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5176 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/zero/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:20.010469 colossalai-nightly-2023.7.8/colossalai_nightly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    25399 2023-07-08 00:17:19.000000 colossalai-nightly-2023.7.8/colossalai_nightly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    39364 2023-07-08 00:17:19.000000 colossalai-nightly-2023.7.8/colossalai_nightly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 00:17:19.000000 colossalai-nightly-2023.7.8/colossalai_nightly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-08 00:17:19.000000 colossalai-nightly-2023.7.8/colossalai_nightly.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-08 00:17:19.000000 colossalai-nightly-2023.7.8/colossalai_nightly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-08 00:17:19.000000 colossalai-nightly-2023.7.8/colossalai_nightly.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:20.014469 colossalai-nightly-2023.7.8/op_builder/
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/op_builder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8943 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/op_builder/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/op_builder/cpu_adam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/op_builder/fused_optim.py
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/op_builder/layernorm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/op_builder/moe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/op_builder/multi_head_attn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/op_builder/scaled_masked_softmax.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/op_builder/scaled_upper_triangle_masked_softmax.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8210 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/op_builder/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:20.014469 colossalai-nightly-2023.7.8/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/requirements/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/requirements/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 00:17:20.026470 colossalai-nightly-2023.7.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     6229 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.922461 colossalai-nightly-2023.7.8/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:20.014469 colossalai-nightly-2023.7.8/tests/components_to_test/
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/components_to_test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2469 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/components_to_test/albert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/components_to_test/beit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3270 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/components_to_test/bert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2857 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/components_to_test/gpt2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/components_to_test/hanging_param_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/components_to_test/inline_op_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/components_to_test/nested_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/components_to_test/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/components_to_test/repeated_computed_layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/components_to_test/resnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/components_to_test/simple_net.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:20.014469 colossalai-nightly-2023.7.8/tests/components_to_test/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/components_to_test/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/components_to_test/utils/dummy_data_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/components_to_test/utils/executor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:20.014469 colossalai-nightly-2023.7.8/tests/kit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/kit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:20.014469 colossalai-nightly-2023.7.8/tests/kit/model_zoo/
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/kit/model_zoo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:20.014469 colossalai-nightly-2023.7.8/tests/kit/model_zoo/diffusers/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/kit/model_zoo/diffusers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2825 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/kit/model_zoo/diffusers/diffusers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2604 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/kit/model_zoo/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:20.014469 colossalai-nightly-2023.7.8/tests/kit/model_zoo/timm/
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/kit/model_zoo/timm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7513 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/kit/model_zoo/timm/timm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:20.014469 colossalai-nightly-2023.7.8/tests/kit/model_zoo/torchaudio/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/kit/model_zoo/torchaudio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5409 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/kit/model_zoo/torchaudio/torchaudio.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:20.014469 colossalai-nightly-2023.7.8/tests/kit/model_zoo/torchrec/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/kit/model_zoo/torchrec/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4634 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/kit/model_zoo/torchrec/torchrec.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:20.014469 colossalai-nightly-2023.7.8/tests/kit/model_zoo/torchvision/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/kit/model_zoo/torchvision/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5931 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/kit/model_zoo/torchvision/torchvision.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:20.018469 colossalai-nightly-2023.7.8/tests/kit/model_zoo/transformers/
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/kit/model_zoo/transformers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4023 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/kit/model_zoo/transformers/albert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7419 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/kit/model_zoo/transformers/bert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4659 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/kit/model_zoo/transformers/bloom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3910 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/kit/model_zoo/transformers/gpt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3213 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/kit/model_zoo/transformers/llama.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3114 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/kit/model_zoo/transformers/opt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/kit/model_zoo/transformers/t5.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:20.018469 colossalai-nightly-2023.7.8/tests/test_analyzer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/test_analyzer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:20.018469 colossalai-nightly-2023.7.8/tests/test_analyzer/test_fx/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/test_analyzer/test_fx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4330 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/test_analyzer/test_fx/test_bias_addition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2735 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/test_analyzer/test_fx/test_mod_dir.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/test_analyzer/test_fx/test_nested_ckpt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/test_analyzer/test_fx/test_shape_prop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/test_analyzer/test_fx/test_symbolic_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/test_analyzer/test_fx/zoo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:20.018469 colossalai-nightly-2023.7.8/tests/test_analyzer/test_subclasses/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/test_analyzer/test_subclasses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3644 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/test_analyzer/test_subclasses/test_aten.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/test_analyzer/test_subclasses/test_flop_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/test_analyzer/test_subclasses/test_meta_mode.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:20.018469 colossalai-nightly-2023.7.8/tests/test_auto_parallel/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/test_auto_parallel/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:20.018469 colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_pass/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_pass/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_pass/test_node_converting_pass.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2283 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_pass/test_size_value_converting_pass.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:20.018469 colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2842 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_bias_addition_forward.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_broadcast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2417 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3521 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_compatibility_with_ddp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4172 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_compatibility_with_gemini.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3747 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_find_repeat_block.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:20.022470 colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_gpt/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_gpt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11050 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_gpt/gpt_modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7786 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_gpt/test_runtime_with_gpt_modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3932 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_gpt/test_solver_with_gpt_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_liveness_analysis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:20.022470 colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11552 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_addbmm_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7693 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_addmm_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4842 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_batch_norm_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6740 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_bias_linear_function_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6205 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_bias_linear_module_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10993 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_binary_elementwise_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9001 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_bmm_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12886 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_conv_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3734 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_default_reshape_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11802 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_embedding_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3003 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_getattr_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8173 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_getitem_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4372 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_layer_norm_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13108 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_linear_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8356 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_matmul_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_norm_pooling_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2623 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_output_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18730 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_permute_and_transpose_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3153 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_placeholder_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4263 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_shard_option.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9001 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_softmax_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12527 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_split_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12380 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_sum_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_tensor_constructor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3762 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_unary_element_wise_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14158 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_view_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_where_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8918 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5325 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_solver_with_resnet_v2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:20.026470 colossalai-nightly-2023.7.8/tests/test_shardformer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/test_shardformer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:20.026470 colossalai-nightly-2023.7.8/tests/test_shardformer/test_model/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/test_shardformer/test_model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/test_shardformer/test_model/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3833 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/test_shardformer/test_model/test_shard_bert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3828 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/test_shardformer/test_model/test_shard_bloom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3736 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/test_shardformer/test_model/test_shard_gpt2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3906 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/test_shardformer/test_model/test_shard_llama.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3911 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/test_shardformer/test_model/test_shard_opt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4801 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/test_shardformer/test_model/test_shard_t5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/test_shardformer/test_model/test_shard_vit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/test_shardformer/test_with_torch_ddp.py
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/version.txt
```

### Comparing `colossalai-nightly-2023.7.1/LICENSE` & `colossalai-nightly-2023.7.8/LICENSE`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/PKG-INFO` & `colossalai-nightly-2023.7.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: colossalai-nightly
-Version: 2023.7.1
+Version: 2023.7.8
 Summary: An integrated large-scale model training system with efficient parallelization techniques
 Home-page: https://www.colossalai.org
 License: Apache Software License 2.0
 Project-URL: Forum, https://github.com/hpcaitech/ColossalAI/discussions
 Project-URL: Bug Tracker, https://github.com/hpcaitech/ColossalAI/issues
 Project-URL: Examples, https://github.com/hpcaitech/ColossalAI-Examples
 Project-URL: Documentation, http://colossalai.readthedocs.io
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: colossalai-nightly Version: 2023.7.1 Summary: An
+Metadata-Version: 2.1 Name: colossalai-nightly Version: 2023.7.8 Summary: An
 integrated large-scale model training system with efficient parallelization
 techniques Home-page: https://www.colossalai.org License: Apache Software
 License 2.0 Project-URL: Forum, https://github.com/hpcaitech/ColossalAI/
 discussions Project-URL: Bug Tracker, https://github.com/hpcaitech/ColossalAI/
 issues Project-URL: Examples, https://github.com/hpcaitech/ColossalAI-Examples
 Project-URL: Documentation, http://colossalai.readthedocs.io Project-URL:
 Github, https://github.com/hpcaitech/ColossalAI Description: # Colossal-AI
```

### Comparing `colossalai-nightly-2023.7.1/README.md` & `colossalai-nightly-2023.7.8/README.md`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/__init__.py` & `colossalai-nightly-2023.7.8/colossalai/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/_analyzer/_subclasses/_meta_registration.py` & `colossalai-nightly-2023.7.8/colossalai/_analyzer/_subclasses/_meta_registration.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/_analyzer/_subclasses/_monkey_patch.py` & `colossalai-nightly-2023.7.8/colossalai/_analyzer/_subclasses/_monkey_patch.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/_analyzer/_subclasses/flop_tensor.py` & `colossalai-nightly-2023.7.8/colossalai/_analyzer/_subclasses/flop_tensor.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/_analyzer/_subclasses/meta_tensor.py` & `colossalai-nightly-2023.7.8/colossalai/_analyzer/_subclasses/meta_tensor.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/_analyzer/fx/codegen.py` & `colossalai-nightly-2023.7.8/colossalai/_analyzer/fx/codegen.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/_analyzer/fx/graph_module.py` & `colossalai-nightly-2023.7.8/colossalai/_analyzer/fx/graph_module.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/_analyzer/fx/node_util.py` & `colossalai-nightly-2023.7.8/colossalai/_analyzer/fx/node_util.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/_analyzer/fx/passes/graph_profile.py` & `colossalai-nightly-2023.7.8/colossalai/_analyzer/fx/passes/graph_profile.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/_analyzer/fx/passes/shape_prop.py` & `colossalai-nightly-2023.7.8/colossalai/_analyzer/fx/passes/shape_prop.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/_analyzer/fx/symbolic_profile.py` & `colossalai-nightly-2023.7.8/colossalai/_analyzer/fx/symbolic_profile.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/_analyzer/fx/tracer/bias_addition.py` & `colossalai-nightly-2023.7.8/colossalai/_analyzer/fx/tracer/bias_addition.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/_analyzer/fx/tracer/custom_leaf_module.py` & `colossalai-nightly-2023.7.8/colossalai/_analyzer/fx/tracer/custom_leaf_module.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/_analyzer/fx/tracer/proxy.py` & `colossalai-nightly-2023.7.8/colossalai/_analyzer/fx/tracer/proxy.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/_analyzer/fx/tracer/symbolic_trace.py` & `colossalai-nightly-2023.7.8/colossalai/_analyzer/fx/tracer/symbolic_trace.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/_analyzer/fx/tracer/tracer.py` & `colossalai-nightly-2023.7.8/colossalai/_analyzer/fx/tracer/tracer.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/amp/__init__.py` & `colossalai-nightly-2023.7.8/colossalai/amp/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/amp/apex_amp/__init__.py` & `colossalai-nightly-2023.7.8/colossalai/amp/apex_amp/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/amp/apex_amp/apex_amp.py` & `colossalai-nightly-2023.7.8/colossalai/amp/apex_amp/apex_amp.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/amp/naive_amp/__init__.py` & `colossalai-nightly-2023.7.8/colossalai/amp/naive_amp/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/amp/naive_amp/_fp16_optimizer.py` & `colossalai-nightly-2023.7.8/colossalai/amp/naive_amp/_fp16_optimizer.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/amp/naive_amp/_utils.py` & `colossalai-nightly-2023.7.8/colossalai/amp/naive_amp/_utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/amp/naive_amp/grad_scaler/base_grad_scaler.py` & `colossalai-nightly-2023.7.8/colossalai/amp/naive_amp/grad_scaler/base_grad_scaler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/amp/naive_amp/grad_scaler/constant_grad_scaler.py` & `colossalai-nightly-2023.7.8/colossalai/amp/naive_amp/grad_scaler/constant_grad_scaler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/amp/naive_amp/grad_scaler/dynamic_grad_scaler.py` & `colossalai-nightly-2023.7.8/colossalai/amp/naive_amp/grad_scaler/dynamic_grad_scaler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/amp/naive_amp/mixed_precision_mixin/base.py` & `colossalai-nightly-2023.7.8/colossalai/amp/naive_amp/mixed_precision_mixin/base.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/amp/naive_amp/mixed_precision_mixin/fp16.py` & `colossalai-nightly-2023.7.8/colossalai/amp/naive_amp/mixed_precision_mixin/fp16.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/amp/naive_amp/naive_amp.py` & `colossalai-nightly-2023.7.8/colossalai/amp/naive_amp/naive_amp.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/amp/torch_amp/__init__.py` & `colossalai-nightly-2023.7.8/colossalai/amp/torch_amp/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/amp/torch_amp/_grad_scaler.py` & `colossalai-nightly-2023.7.8/colossalai/amp/torch_amp/_grad_scaler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/amp/torch_amp/torch_amp.py` & `colossalai-nightly-2023.7.8/colossalai/amp/torch_amp/torch_amp.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/auto_parallel/checkpoint/ckpt_solver_base.py` & `colossalai-nightly-2023.7.8/colossalai/auto_parallel/checkpoint/ckpt_solver_base.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/auto_parallel/checkpoint/ckpt_solver_chen.py` & `colossalai-nightly-2023.7.8/colossalai/auto_parallel/checkpoint/ckpt_solver_chen.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/auto_parallel/checkpoint/ckpt_solver_rotor.py` & `colossalai-nightly-2023.7.8/colossalai/auto_parallel/checkpoint/ckpt_solver_rotor.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/auto_parallel/checkpoint/operation.py` & `colossalai-nightly-2023.7.8/colossalai/auto_parallel/checkpoint/operation.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/auto_parallel/meta_profiler/meta_registry/activation.py` & `colossalai-nightly-2023.7.8/colossalai/auto_parallel/meta_profiler/meta_registry/activation.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/auto_parallel/meta_profiler/meta_registry/binary_elementwise_ops.py` & `colossalai-nightly-2023.7.8/colossalai/auto_parallel/meta_profiler/meta_registry/binary_elementwise_ops.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/auto_parallel/meta_profiler/meta_registry/conv.py` & `colossalai-nightly-2023.7.8/colossalai/auto_parallel/meta_profiler/meta_registry/conv.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/auto_parallel/meta_profiler/meta_registry/embedding.py` & `colossalai-nightly-2023.7.8/colossalai/auto_parallel/meta_profiler/meta_registry/embedding.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/auto_parallel/meta_profiler/meta_registry/linear.py` & `colossalai-nightly-2023.7.8/colossalai/auto_parallel/meta_profiler/meta_registry/linear.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/auto_parallel/meta_profiler/meta_registry/non_spmd.py` & `colossalai-nightly-2023.7.8/colossalai/auto_parallel/meta_profiler/meta_registry/non_spmd.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/auto_parallel/meta_profiler/meta_registry/norm.py` & `colossalai-nightly-2023.7.8/colossalai/auto_parallel/meta_profiler/meta_registry/norm.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/auto_parallel/meta_profiler/meta_registry/pooling.py` & `colossalai-nightly-2023.7.8/colossalai/auto_parallel/meta_profiler/meta_registry/pooling.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/auto_parallel/meta_profiler/meta_registry/tensor.py` & `colossalai-nightly-2023.7.8/colossalai/auto_parallel/meta_profiler/meta_registry/tensor.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/auto_parallel/meta_profiler/meta_registry/where.py` & `colossalai-nightly-2023.7.8/colossalai/auto_parallel/meta_profiler/meta_registry/where.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/auto_parallel/meta_profiler/registry.py` & `colossalai-nightly-2023.7.8/colossalai/auto_parallel/meta_profiler/registry.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/auto_parallel/meta_profiler/shard_metainfo.py` & `colossalai-nightly-2023.7.8/colossalai/auto_parallel/meta_profiler/shard_metainfo.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/auto_parallel/offload/amp_optimizer.py` & `colossalai-nightly-2023.7.8/colossalai/auto_parallel/offload/amp_optimizer.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/auto_parallel/offload/base_offload_module.py` & `colossalai-nightly-2023.7.8/colossalai/auto_parallel/offload/base_offload_module.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/auto_parallel/offload/mem_optimize.py` & `colossalai-nightly-2023.7.8/colossalai/auto_parallel/offload/mem_optimize.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/auto_parallel/offload/region.py` & `colossalai-nightly-2023.7.8/colossalai/auto_parallel/offload/region.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/auto_parallel/offload/region_manager.py` & `colossalai-nightly-2023.7.8/colossalai/auto_parallel/offload/region_manager.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/auto_parallel/offload/runtime.py` & `colossalai-nightly-2023.7.8/colossalai/auto_parallel/offload/runtime.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/auto_parallel/offload/solver.py` & `colossalai-nightly-2023.7.8/colossalai/auto_parallel/offload/solver.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/auto_parallel/offload/training_simulator.py` & `colossalai-nightly-2023.7.8/colossalai/auto_parallel/offload/training_simulator.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/auto_parallel/offload/util.py` & `colossalai-nightly-2023.7.8/colossalai/auto_parallel/offload/util.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/auto_parallel/passes/comm_metainfo_pass.py` & `colossalai-nightly-2023.7.8/colossalai/auto_parallel/passes/comm_metainfo_pass.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/auto_parallel/passes/meta_info_prop.py` & `colossalai-nightly-2023.7.8/colossalai/auto_parallel/passes/meta_info_prop.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/auto_parallel/passes/runtime_apply_pass.py` & `colossalai-nightly-2023.7.8/colossalai/auto_parallel/passes/runtime_apply_pass.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/auto_parallel/passes/runtime_preparation_pass.py` & `colossalai-nightly-2023.7.8/colossalai/auto_parallel/passes/runtime_preparation_pass.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/auto_parallel/tensor_shard/constants.py` & `colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/constants.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/auto_parallel/tensor_shard/initialize.py` & `colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/initialize.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/auto_parallel/tensor_shard/node_handler/__init__.py` & `colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/auto_parallel/tensor_shard/node_handler/addmm_handler.py` & `colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/addmm_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/auto_parallel/tensor_shard/node_handler/batch_norm_handler.py` & `colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/batch_norm_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/auto_parallel/tensor_shard/node_handler/binary_elementwise_handler.py` & `colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/binary_elementwise_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/auto_parallel/tensor_shard/node_handler/bmm_handler.py` & `colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/bmm_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/auto_parallel/tensor_shard/node_handler/conv_handler.py` & `colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/conv_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/auto_parallel/tensor_shard/node_handler/default_reshape_handler.py` & `colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/default_reshape_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/auto_parallel/tensor_shard/node_handler/embedding_handler.py` & `colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/embedding_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/auto_parallel/tensor_shard/node_handler/getattr_handler.py` & `colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/getattr_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/auto_parallel/tensor_shard/node_handler/getitem_handler.py` & `colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/getitem_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/auto_parallel/tensor_shard/node_handler/layer_norm_handler.py` & `colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/layer_norm_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/auto_parallel/tensor_shard/node_handler/linear_handler.py` & `colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/linear_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/auto_parallel/tensor_shard/node_handler/matmul_handler.py` & `colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/matmul_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/auto_parallel/tensor_shard/node_handler/node_handler.py` & `colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/node_handler.py`

 * *Files 0% similar despite different names*

```diff
@@ -184,15 +184,15 @@
             for op_data, sharding_spec in strategy.sharding_specs.items():
                 if op_data.data is not None and isinstance(op_data.data, torch.Tensor):
                     check_sharding_spec_validity(sharding_spec, op_data.data)
 
         remove_strategy_list = []
         for strategy in self.strategies_vector:
             shard_axis_list = []
-            last_axis = len(self.device_mesh.mesh_shape) - 1
+            last_axis = len(self.device_mesh.shape) - 1
             for op_data, sharding_spec in strategy.sharding_specs.items():
                 if op_data.data is not None and isinstance(op_data.data, torch.Tensor):
                     for dim, shard_axes in sharding_spec.dim_partition_dict.items():
                         for shard_axis in shard_axes:
                             if shard_axis not in shard_axis_list:
                                 shard_axis_list.append(shard_axis)
```

### Comparing `colossalai-nightly-2023.7.1/colossalai/auto_parallel/tensor_shard/node_handler/normal_pooling_handler.py` & `colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/normal_pooling_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/auto_parallel/tensor_shard/node_handler/output_handler.py` & `colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/output_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/auto_parallel/tensor_shard/node_handler/permute_handler.py` & `colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/permute_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/auto_parallel/tensor_shard/node_handler/placeholder_handler.py` & `colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/placeholder_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/auto_parallel/tensor_shard/node_handler/registry.py` & `colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/registry.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/auto_parallel/tensor_shard/node_handler/softmax_handler.py` & `colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/softmax_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/auto_parallel/tensor_shard/node_handler/split_handler.py` & `colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/split_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/auto_parallel/tensor_shard/node_handler/strategy/__init__.py` & `colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/strategy/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/auto_parallel/tensor_shard/node_handler/strategy/batch_norm_generator.py` & `colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/strategy/batch_norm_generator.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/auto_parallel/tensor_shard/node_handler/strategy/binary_elementwise_generator.py` & `colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/strategy/binary_elementwise_generator.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/auto_parallel/tensor_shard/node_handler/strategy/conv_strategy_generator.py` & `colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/strategy/conv_strategy_generator.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/auto_parallel/tensor_shard/node_handler/strategy/embedding_generator.py` & `colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/strategy/embedding_generator.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/auto_parallel/tensor_shard/node_handler/strategy/getattr_generator.py` & `colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/strategy/getattr_generator.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/auto_parallel/tensor_shard/node_handler/strategy/getitem_generator.py` & `colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/strategy/getitem_generator.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/auto_parallel/tensor_shard/node_handler/strategy/layer_norm_generator.py` & `colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/strategy/layer_norm_generator.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/auto_parallel/tensor_shard/node_handler/strategy/matmul_strategy_generator.py` & `colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/strategy/matmul_strategy_generator.py`

 * *Files 0% similar despite different names*

```diff
@@ -980,26 +980,26 @@
         return self.get_sharding_strategy(name=name,
                                           sharding_spec_mapping=sharding_spec_mapping,
                                           communication_action_mapping=communication_action_mapping)
 
     def collate_strategies(self) -> List[ShardingStrategy]:
         strategy_list = []
         device_mesh_is_1d = True
-        if len(self.device_mesh.mesh_shape) == 2 and 1 not in self.device_mesh.mesh_shape:
+        if len(self.device_mesh.shape) == 2 and 1 not in self.device_mesh.shape:
             device_mesh_is_1d = False
 
         if device_mesh_is_1d:
             # split only the batch dimension
             # Sb = Sb x Sb
             # can be None as it is only for 1D device mesh
             # only for 1D device mesh
-            if len(self.device_mesh.mesh_shape) == 1:
+            if len(self.device_mesh.shape) == 1:
                 mesh_dim = 0
             else:
-                mesh_dim = self.device_mesh.mesh_shape.index(1)
+                mesh_dim = self.device_mesh.shape.index(1)
             strategy_list.append(self.split_one_batch_dim(mesh_dim))
         else:
             # for 2D device mesh
             # split batch dim of two inputs and the i dim of the first tensor
             # SbSi = SbSi x Sb
             strategy_list.append(self.split_batch_dim_lhs_space(0, 1))
             strategy_list.append(self.split_batch_dim_lhs_space(1, 0))
```

### Comparing `colossalai-nightly-2023.7.1/colossalai/auto_parallel/tensor_shard/node_handler/strategy/normal_pooling_generator.py` & `colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/strategy/normal_pooling_generator.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/auto_parallel/tensor_shard/node_handler/strategy/output_generator.py` & `colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/strategy/output_generator.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/auto_parallel/tensor_shard/node_handler/strategy/placeholder_generator.py` & `colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/strategy/placeholder_generator.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/auto_parallel/tensor_shard/node_handler/strategy/reshape_generator.py` & `colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/strategy/reshape_generator.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/auto_parallel/tensor_shard/node_handler/strategy/softmax_generator.py` & `colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/strategy/softmax_generator.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/auto_parallel/tensor_shard/node_handler/strategy/strategy_generator.py` & `colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/strategy/strategy_generator.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/auto_parallel/tensor_shard/node_handler/strategy/sum_generator.py` & `colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/strategy/sum_generator.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/auto_parallel/tensor_shard/node_handler/strategy/tensor_constructor_generator.py` & `colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/strategy/tensor_constructor_generator.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/auto_parallel/tensor_shard/node_handler/strategy/unary_elementwise_generator.py` & `colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/strategy/unary_elementwise_generator.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/auto_parallel/tensor_shard/node_handler/strategy/where_generator.py` & `colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/strategy/where_generator.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/auto_parallel/tensor_shard/node_handler/sum_handler.py` & `colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/sum_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/auto_parallel/tensor_shard/node_handler/tensor_constructor_handler.py` & `colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/tensor_constructor_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/auto_parallel/tensor_shard/node_handler/transpose_handler.py` & `colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/transpose_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/auto_parallel/tensor_shard/node_handler/unary_elementwise_handler.py` & `colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/unary_elementwise_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/auto_parallel/tensor_shard/node_handler/view_handler.py` & `colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/view_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/auto_parallel/tensor_shard/node_handler/where_handler.py` & `colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/where_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/auto_parallel/tensor_shard/options.py` & `colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/options.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/auto_parallel/tensor_shard/sharding_strategy.py` & `colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/sharding_strategy.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/auto_parallel/tensor_shard/solver/cost_graph.py` & `colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/solver/cost_graph.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/auto_parallel/tensor_shard/solver/graph_analysis.py` & `colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/solver/graph_analysis.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/auto_parallel/tensor_shard/solver/solver.py` & `colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/solver/solver.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/auto_parallel/tensor_shard/solver/strategies_constructor.py` & `colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/solver/strategies_constructor.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/auto_parallel/tensor_shard/utils/__init__.py` & `colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/auto_parallel/tensor_shard/utils/broadcast.py` & `colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/utils/broadcast.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/auto_parallel/tensor_shard/utils/factory.py` & `colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/utils/factory.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/auto_parallel/tensor_shard/utils/misc.py` & `colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/utils/misc.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,16 +42,16 @@
         2. the sharding spec for each dimension is divisible by the number of devices.
         3. the sharding spec's entire shape must match the tensor shape
     #
     """
     # make sure all dims are covered in sharding spec
     sharding_len = len(sharding_spec.sharding_sequence)
     tensor_num_dim = tensor.dim()
-    num_devices_in_col = sharding_spec.device_mesh.mesh_shape[0]
-    num_devices_in_row = sharding_spec.device_mesh.mesh_shape[1]
+    num_devices_in_col = sharding_spec.device_mesh.shape[0]
+    num_devices_in_row = sharding_spec.device_mesh.shape[1]
     assert sharding_len == tensor_num_dim, \
         f'The ShardingSpec ({sharding_spec.sharding_sequence}) is created for {sharding_len}-dimension tensor, but the given tensor is {tensor_num_dim}-dimension ({tensor.shape}).'
 
     # make sure the sharding is valid for each dim
     for i in range(tensor_num_dim):
         dim_size = tensor.shape[i]
         dim_spec = sharding_spec.sharding_sequence[i]
```

### Comparing `colossalai-nightly-2023.7.1/colossalai/auto_parallel/tensor_shard/utils/reshape.py` & `colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/utils/reshape.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/auto_parallel/tensor_shard/utils/sharding.py` & `colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/utils/sharding.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/booster/accelerator.py` & `colossalai-nightly-2023.7.8/colossalai/booster/accelerator.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/booster/booster.py` & `colossalai-nightly-2023.7.8/colossalai/booster/booster.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/booster/mixed_precision/__init__.py` & `colossalai-nightly-2023.7.8/colossalai/booster/mixed_precision/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/booster/mixed_precision/fp16_apex.py` & `colossalai-nightly-2023.7.8/colossalai/booster/mixed_precision/fp16_apex.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/booster/mixed_precision/fp16_naive.py` & `colossalai-nightly-2023.7.8/colossalai/booster/mixed_precision/fp16_naive.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/booster/mixed_precision/fp16_torch.py` & `colossalai-nightly-2023.7.8/colossalai/booster/mixed_precision/fp16_torch.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/booster/mixed_precision/mixed_precision_base.py` & `colossalai-nightly-2023.7.8/colossalai/booster/mixed_precision/mixed_precision_base.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/booster/plugin/dp_plugin_base.py` & `colossalai-nightly-2023.7.8/colossalai/booster/plugin/dp_plugin_base.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/booster/plugin/gemini_plugin.py` & `colossalai-nightly-2023.7.8/colossalai/booster/plugin/gemini_plugin.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,63 +29,65 @@
 
 class GeminiCheckpointIO(GeneralCheckpointIO):
 
     def __init__(self) -> None:
         super().__init__()
         self.coordinator = DistCoordinator()
 
-    def load_unsharded_model(self, model: GeminiDDP, checkpoint: str, strict: bool = True):
-        """
-        Load model from checkpoint with automatic unwrapping.
-        """
-        # the model should be unwrapped in self.load_model via ModelWrapper.unwrap
-        return super().load_unsharded_model(model, checkpoint, strict=strict)
-
     def save_unsharded_model(self, model: GeminiDDP, checkpoint: str, gather_dtensor: bool, use_safetensors: bool):
         """
-        Save model to checkpoint but only on master process.
+        Save sharded model to checkpoint but only on master process.
+        The model should be unwrapped in self.load_model via ModelWrapper.unwrap.
+        As there is communication when getting state dict, this must be called on all processes.
         """
-        # the model should be unwrapped in self.load_model via ModelWrapper.unwrap
-        # as there is communication when get state dict, this must be called on all processes
         state_dict = model.state_dict(only_rank_0=True)
         if self.coordinator.is_master():
             save_state_dict(state_dict, checkpoint, use_safetensors)
 
-    def save_unsharded_optimizer(self, optimizer: Optimizer, checkpoint: str, gather_dtensor: bool):
+    def load_unsharded_model(self, model: GeminiDDP, checkpoint: str, strict: bool = True):
         """
-        Save optimizer to checkpoint but only on master process.
+        Load model from checkpoint with automatic unwrapping.
+        The model should be unwrapped in self.load_model via ModelWrapper.unwrap.
         """
-        # TODO(ver217): optimizer state dict is sharded
-        warnings.warn('GeminiPlugin does not support save full optimizer checkpoint now. Save it on every process.')
-        checkpoint = f'{checkpoint}.rank{self.coordinator.rank}'
-        super().save_unsharded_optimizer(optimizer, checkpoint, gather_dtensor)
-
-    def load_optimizer(self, optimizer: Optimizer, checkpoint: str):
-        warnings.warn(
-            'GeminiPlugin can only load optimizer checkpoint saved by itself with the same number of processes.')
-        checkpoint = f'{checkpoint}.rank{self.coordinator.rank}'
-        super().load_optimizer(optimizer, checkpoint)
+        super().load_unsharded_model(model, checkpoint, strict=strict)
 
-    def save_lr_scheduler(self, lr_scheduler: LRScheduler, checkpoint: str):
+    def save_unsharded_optimizer(self, optimizer: Optimizer, checkpoint: str, gather_dtensor: bool):
         """
-        Save model to checkpoint but only on master process.
+        Save unsharded optimizer state dict to checkpoint.
+        After calling optimizer.state_dict(), the complete optimizer states will be collected on master rank.
+        As there is communication when getting state dict, this must be called on all processes.
+        The saving process will only be executed by master rank.
         """
+        state_dict = optimizer.state_dict()
         if self.coordinator.is_master():
-            super().save_lr_scheduler(lr_scheduler, checkpoint)
+            save_state_dict(state_dict, checkpoint, use_safetensors=False)
+
+    def load_unsharded_optimizer(self, optimizer: Optimizer, checkpoint: str):
+        """
+        Loading unsharded optimizer from checkpoint file.
+        For each process, only loading optimizer states of parameters it controls.
+        """
+        super().load_unsharded_optimizer(optimizer, checkpoint)
 
     def save_sharded_model(self,
                            model: GeminiDDP,
                            checkpoint_path: str,
                            gather_dtensor: bool = False,
                            prefix: Optional[str] = None,
                            max_shard_size: int = 1024,
                            use_safetensors: bool = False):
         """
         Save sharded model
         """
+        if os.path.isfile(checkpoint_path):
+            logging.error(f"Provided path ({checkpoint_path}) should be a directory, not a file")
+            return
+
+        Path(checkpoint_path).mkdir(parents=True, exist_ok=True)
+
         state_dict_shard = model.state_dict_shard(max_shard_size=max_shard_size, only_rank_0=True, dtype=torch.float32)
         weights_name, save_index_file = get_model_base_filenames(prefix, use_safetensors)
         total_size = 0
         index_file = CheckpointIndexFile(checkpoint_path)
         for idx, shard_pair in enumerate(state_dict_shard):
             if not self.coordinator.is_master():
                 continue
@@ -113,14 +115,31 @@
                            strict: bool = False,
                            use_safetensors: bool = False):
         """
         load shard model, load model from multiple files
         """
         return super().load_sharded_model(model, checkpoint_index_file, strict, use_safetensors, load_sub_module=False)
 
+    def save_sharded_optimizer(self, optimizer: Optimizer, checkpoint: Path, gather_dtensor: bool, prefix: str,
+                               size_per_shard: int):
+        """
+        Save sharded optimizer state dict to checkpoint folder.
+        As there is communication when getting state dict, this must be called on all processes.
+        """
+        Path(checkpoint).mkdir(parents=True, exist_ok=True)
+        super().save_sharded_optimizer(optimizer, checkpoint, gather_dtensor, prefix, size_per_shard)
+
+    def load_sharded_optimizer(self, optimizer: Optimizer, checkpoint_index_file: Path, prefix: str):
+        """
+        Loading sharded optimizer from checkpoint folder, with index file given.
+        For each process, only loading optimizer states of parameters it controls.
+        """
+        # TODO(Baizhou): To be implemented.
+        pass
+
 
 class GeminiModel(ModelWrapper):
 
     def __init__(self, module: nn.Module, gemini_config: dict, verbose: bool = False) -> None:
         super().__init__(module)
         self.module = zero_model_wrapper(module, zero_stage=3, gemini_config=gemini_config, verbose=verbose)
 
@@ -189,15 +208,15 @@
             If the aggregate size of parameters is still smaller than the minimum chunk size,
             all parameters will be compacted into one small chunk.
         memstats (MemStats, optional) the memory statistics collector by a runtime memory tracer.
         gpu_margin_mem_ratio (float, optional): The ratio of GPU remaining memory (after the first forward-backward)
             which will be used when using hybrid CPU optimizer.
             This argument is meaningless when `placement_policy` of `GeminiManager` is not "auto".
             Defaults to 0.0.
-        initial_scale (float, optional): Initial scale used by DynamicGradScaler. Defaults to 2**32.
+        initial_scale (float, optional): Initial scale used by DynamicGradScaler. Defaults to 2**16.
         min_scale (float, optional): Min scale used by DynamicGradScaler. Defaults to 1.
         growth_factor (float, optional): growth_factor used by DynamicGradScaler. Defaults to 2.
         backoff_factor (float, optional): backoff_factor used by DynamicGradScaler. Defaults to 0.5.
         growth_interval (float, optional): growth_interval used by DynamicGradScaler. Defaults to 1000.
         hysteresis (float, optional): hysteresis used by DynamicGradScaler. Defaults to 2.
         max_scale (int, optional): max_scale used by DynamicGradScaler. Defaults to 2**32.
         max_norm (float, optional): max_norm used for `clip_grad_norm`. You should notice that you shall not do
@@ -215,15 +234,15 @@
         force_outputs_fp32: bool = False,
         strict_ddp_mode: bool = False,
         search_range_m: int = 32,
         hidden_dim: Optional[int] = None,
         min_chunk_size_m: float = 32,
         memstats: Optional[MemStats] = None,
         gpu_margin_mem_ratio: float = 0.0,
-        initial_scale: float = 2**32,
+        initial_scale: float = 2**16,
         min_scale: float = 1,
         growth_factor: float = 2,
         backoff_factor: float = 0.5,
         growth_interval: int = 1000,
         hysteresis: int = 2,
         max_scale: float = 2**32,
         max_norm: float = 0.0,
```

### Comparing `colossalai-nightly-2023.7.1/colossalai/booster/plugin/low_level_zero_plugin.py` & `colossalai-nightly-2023.7.8/colossalai/booster/plugin/low_level_zero_plugin.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/booster/plugin/plugin_base.py` & `colossalai-nightly-2023.7.8/colossalai/booster/plugin/plugin_base.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/booster/plugin/torch_ddp_plugin.py` & `colossalai-nightly-2023.7.8/colossalai/booster/plugin/torch_ddp_plugin.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/booster/plugin/torch_fsdp_plugin.py` & `colossalai-nightly-2023.7.8/colossalai/booster/plugin/torch_fsdp_plugin.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/builder/builder.py` & `colossalai-nightly-2023.7.8/colossalai/builder/builder.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/checkpoint_io/checkpoint_io_base.py` & `colossalai-nightly-2023.7.8/colossalai/checkpoint_io/checkpoint_io_base.py`

 * *Files 0% similar despite different names*

```diff
@@ -148,14 +148,15 @@
         Args:
             optimizer (Optimizer): optimizer to be loaded.
             checkpoint (str): checkpoint path. This value is made compatibility with the model checkpoints in the
             prefix (str, optional): A prefix added to parameter and buffer
                 names to compose the keys in state_dict. Defaults to None.
             size_per_shard (int, optional): Maximum size of checkpoint shard file in MB. This is useful only when ``shard=True``. Defaults to 1024.
         """
+
         index_file_exists, index_file_path = has_index_file(checkpoint)
 
         if Path(checkpoint).is_dir() and not index_file_exists:
             # if the checkpoint is a directory and there is no index file, raise error
             raise ValueError(f'Cannot find index file in {checkpoint}')
 
         if index_file_exists:
@@ -182,14 +183,15 @@
                 3. a path to a folder containing a unique .index.json file for sharded checkpoint
             shard (bool): whether to shard the checkpoint. Default: False. If set to True, the checkpoint will be sharded into
                 multiple files. The optimizer shards will be specified by a `optimizer.index.json` file.
             gather_dtensor (bool): whether to gather the distributed tensor to the first device. Default: True.
             prefix (str): prefix for the optimizer checkpoint when shard = True. Default: None.
             size_per_shard (int): size per shard in MB. Default: 1024. This value is only used when shard is set to True.
         """
+
         if shard:
             self.save_sharded_optimizer(optimizer, checkpoint, gather_dtensor, prefix, size_per_shard)
         else:
             self.save_unsharded_optimizer(optimizer, checkpoint, gather_dtensor)
 
     # ========================================================
     # Abstract methods for model loading/saving implementation
```

### Comparing `colossalai-nightly-2023.7.1/colossalai/checkpoint_io/general_checkpoint_io.py` & `colossalai-nightly-2023.7.8/colossalai/checkpoint_io/general_checkpoint_io.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,14 +24,15 @@
     load_state_dict_into_model,
     load_states_into_optimizer,
     save_param_groups,
     save_state_dict,
     shard_model_checkpoint,
     shard_optimizer_checkpoint,
     sharded_optimizer_loading_epilogue,
+    unwrap_optimizer,
 )
 
 __all__ = ['GeneralCheckpointIO']
 
 
 class GeneralCheckpointIO(CheckpointIO):
     """
@@ -55,15 +56,15 @@
     def load_sharded_optimizer(self, optimizer: Optimizer, index_file_path: str, prefix: str):
         """
         Load sharded optimizer with the given path to index file.
         """
 
         # If optimizer is wrapped, unwrap it.
         if isinstance(optimizer, OptimizerWrapper):
-            optimizer = optimizer.optim
+            optimizer = unwrap_optimizer(optimizer)
 
         # Read checkpoint index file.
         ckpt_index_file = CheckpointIndexFile.from_file(index_file_path)
 
         # Load param_groups
         param_group_path = ckpt_index_file.get_param_group_filename()
         if param_group_path is None:
@@ -92,14 +93,19 @@
         """
         Save sharded optimizer checkpoint under the given checkpointing path.
         The following files will be created under the path:
         - An index file (pytorch_optim.bin.index.json) containing a map between optimizer states and file names
         - A group file (pytorch_optim_group.bin) recording information of param_groups
         - Multiple files (pytorch_optim-000XX.bin) that store state tensors of optimizer in a sharding way
         """
+
+        # If optimizer is wrapped, unwrap it.
+        if isinstance(optimizer, OptimizerWrapper):
+            optimizer = unwrap_optimizer(optimizer)
+
         if os.path.isfile(checkpoint):
             logging.error(f"Provided path ({checkpoint}) should be a directory, not a file")
             return
 
         Path(checkpoint).mkdir(parents=True, exist_ok=True)
 
         # Offload optimizer states. States are broken into shards within max_shard_size.
@@ -117,17 +123,16 @@
 
         # Save shards of optimizer states.
         total_size = 0
         for idx, shard_pair in enumerate(sharded_state):
             shard, current_size = shard_pair
             shard_file = get_shard_filename(states_name, idx)
             total_size = total_size + current_size
-            for param_id in shard.keys():
-                index_file.append_weight_map(str(param_id), shard_file)
-
+            for key in shard.keys():
+                index_file.append_weight_map(key, shard_file)
             checkpoint_file_path = os.path.join(checkpoint, shard_file)
             save_state_dict(shard, checkpoint_file_path, use_safetensors=False)
 
         # Wrap up index file.
         index_file.append_meta_data("total_size", total_size)
         index_file.write_index_file(save_index_file)
         logging.info(f"The optimizer is going to be split to checkpoint shards. "
@@ -173,15 +178,14 @@
         index_file = CheckpointIndexFile(checkpoint_path)
         for idx, shard_pair in enumerate(state_dict_shard):
             shard = shard_pair[0]
             shard_file = get_shard_filename(weights_name, idx)
             total_size = total_size + shard_pair[1]
             for key in shard.keys():
                 index_file.append_weight_map(key, shard_file)
-
             checkpoint_file_path = os.path.join(checkpoint_path, shard_file)
             save_state_dict(shard, checkpoint_file_path, use_safetensors)
 
         index_file.append_meta_data("total_size", total_size)
         index_file.write_index_file(save_index_file)
         logging.info(f"The model is going to be split to checkpoint shards. "
                      f"You can find where each parameters has been saved in the "
```

### Comparing `colossalai-nightly-2023.7.1/colossalai/checkpoint_io/index_file.py` & `colossalai-nightly-2023.7.8/colossalai/checkpoint_io/index_file.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/checkpoint_io/utils.py` & `colossalai-nightly-2023.7.8/colossalai/checkpoint_io/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,17 @@
 from pathlib import Path
 from typing import Iterator, List, Mapping, Optional, OrderedDict, Tuple
 
 import torch
 import torch.nn as nn
 from torch.optim import Optimizer
 
-from colossalai.tensor.d_tensor.d_tensor import DTensor
+from colossalai.interface import OptimizerWrapper
+from colossalai.nn.optimizer import ColossalaiOptimizer
+from colossalai.tensor.d_tensor import is_distributed_tensor
 
 SAFE_WEIGHTS_NAME = "model.safetensors"
 WEIGHTS_NAME = "pytorch_model.bin"
 STATES_NAME = "pytorch_optim.bin"
 SAFE_WEIGHTS_INDEX_NAME = "model.safetensors.index.json"
 WEIGHTS_INDEX_NAME = "pytorch_model.bin.index.json"
 STATES_INDEX_NAME = "pytorch_optim.bin.index.json"
@@ -84,30 +86,43 @@
     else:
         return False
 
 
 # ======================================
 # Helper functions for saving shard file
 # ======================================
+def unwrap_optimizer(optimizer: OptimizerWrapper):
+    '''
+    Unwrap a wrapped optimizer.
+    This method should be used before saving/loading it to/from sharded checkpoints.
+    '''
+
+    # TODO(Baizhou): ColossalaiOptimizer will be replaced with OptimizerWrapper in the future
+    unwrapped_optim = optimizer.optim
+    if isinstance(unwrapped_optim, ColossalaiOptimizer):
+        unwrapped_optim = unwrapped_optim.optim
+    return unwrapped_optim
+
+
 def shard_model_checkpoint(state_dict: torch.Tensor, max_shard_size: int = 1024) -> Iterator[Tuple[OrderedDict, int]]:
     """
     Splits a model state dictionary in sub-checkpoints so that the final size of each sub-checkpoint does not exceed a
     given size.
     """
     current_block = {}
     current_block_size = 0
 
     for key, weight in state_dict.items():
         ret_block = None
         ret_block_size = 0
-        if type(weight) != DTensor:
+        if not is_distributed_tensor(weight):
             weight_size = calculate_tensor_size(weight)
 
             # If this weight is going to tip up over the maximal size, we split.
-            if current_block_size + weight_size > max_shard_size:
+            if current_block_size + weight_size > max_shard_size and current_block_size > 0:
                 ret_block = current_block
                 ret_block_size = current_block_size
                 current_block = {}
                 current_block_size = 0
             current_block[key] = weight
             current_block_size += weight_size
 
@@ -136,27 +151,28 @@
 
         # A state might contain more than one tensors.
         # e.g. each Adam state includes: 'step', 'exp_avg', 'exp_avg_sq'
         state_size = 0
         isDTensor = False
         for state_tensor in state.values():
 
-            # When state_tensor is None (e.g., a SGD optimizer with momentum set to 0),
+            # When state_tensor is not of Tensor class,
+            # e.g., a SGD optimizer with momentum set to 0 can have None as state
             # The calculation of tensor size should be skipped to avoid error.
-            if state_tensor is None:
+            if not isinstance(state_tensor, torch.Tensor):
                 continue
 
             # If the states are stored as DTensors, mark isDTensor as true.
-            if type(state_tensor) == DTensor:
+            if is_distributed_tensor(state_tensor):
                 isDTensor = True
             state_size += calculate_tensor_size(state_tensor)
 
         if not isDTensor:
 
-            if current_block_size + state_size > max_shard_size:
+            if current_block_size + state_size > max_shard_size and current_block_size > 0:
                 ret_block = current_block
                 ret_block_size = current_block_size
                 current_block = {}
                 current_block_size = 0
 
             current_block[param_id] = state
             current_block_size += state_size
```

### Comparing `colossalai-nightly-2023.7.1/colossalai/cli/benchmark/__init__.py` & `colossalai-nightly-2023.7.8/colossalai/cli/benchmark/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/cli/benchmark/benchmark.py` & `colossalai-nightly-2023.7.8/colossalai/cli/benchmark/benchmark.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/cli/benchmark/utils.py` & `colossalai-nightly-2023.7.8/colossalai/cli/benchmark/utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/cli/check/check_installation.py` & `colossalai-nightly-2023.7.8/colossalai/cli/check/check_installation.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/cli/launcher/__init__.py` & `colossalai-nightly-2023.7.8/colossalai/cli/launcher/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/cli/launcher/hostinfo.py` & `colossalai-nightly-2023.7.8/colossalai/cli/launcher/hostinfo.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/cli/launcher/multinode_runner.py` & `colossalai-nightly-2023.7.8/colossalai/cli/launcher/multinode_runner.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/cli/launcher/run.py` & `colossalai-nightly-2023.7.8/colossalai/cli/launcher/run.py`

 * *Files 2% similar despite different names*

```diff
@@ -160,17 +160,15 @@
         cmd = [
             sys.executable, "-m", "torch.distributed.launch", f"--nproc_per_node={nproc_per_node}",
             f"--master_addr={master_addr}", f"--master_port={master_port}", f"--nnodes={num_nodes}",
             f"--node_rank={node_rank}"
         ]
     else:
         # extra launch args for torch distributed launcher with torch >= 1.9
-        default_torchrun_rdzv_args = dict(rdzv_backend="c10d",
-                                          rdzv_endpoint=f"{master_addr}:{master_port}",
-                                          rdzv_id="colossalai-default-job")
+        default_torchrun_rdzv_args = dict(master_addr=master_addr, master_port=master_port)
 
         # update rdzv arguments
         for key in default_torchrun_rdzv_args.keys():
             if key in extra_launch_args:
                 value = extra_launch_args.pop(key)
                 default_torchrun_rdzv_args[key] = value
```

### Comparing `colossalai-nightly-2023.7.1/colossalai/cluster/device_mesh_manager.py` & `colossalai-nightly-2023.7.8/colossalai/cluster/device_mesh_manager.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/cluster/dist_coordinator.py` & `colossalai-nightly-2023.7.8/colossalai/cluster/dist_coordinator.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/cluster/process_group_manager.py` & `colossalai-nightly-2023.7.8/colossalai/cluster/process_group_manager.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/communication/__init__.py` & `colossalai-nightly-2023.7.8/colossalai/communication/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/communication/collective.py` & `colossalai-nightly-2023.7.8/colossalai/communication/collective.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/communication/p2p.py` & `colossalai-nightly-2023.7.8/colossalai/communication/p2p.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/communication/p2p_v2.py` & `colossalai-nightly-2023.7.8/colossalai/communication/p2p_v2.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/communication/ring.py` & `colossalai-nightly-2023.7.8/colossalai/communication/ring.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/communication/utils.py` & `colossalai-nightly-2023.7.8/colossalai/communication/utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/constants.py` & `colossalai-nightly-2023.7.8/colossalai/constants.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/context/config.py` & `colossalai-nightly-2023.7.8/colossalai/context/config.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/context/moe_context.py` & `colossalai-nightly-2023.7.8/colossalai/context/moe_context.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/context/parallel_context.py` & `colossalai-nightly-2023.7.8/colossalai/context/parallel_context.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/context/parallel_mode.py` & `colossalai-nightly-2023.7.8/colossalai/context/parallel_mode.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/context/process_group_initializer/__init__.py` & `colossalai-nightly-2023.7.8/colossalai/context/process_group_initializer/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/context/process_group_initializer/initializer_1d.py` & `colossalai-nightly-2023.7.8/colossalai/context/process_group_initializer/initializer_1d.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/context/process_group_initializer/initializer_2d.py` & `colossalai-nightly-2023.7.8/colossalai/context/process_group_initializer/initializer_2d.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/context/process_group_initializer/initializer_2p5d.py` & `colossalai-nightly-2023.7.8/colossalai/context/process_group_initializer/initializer_2p5d.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/context/process_group_initializer/initializer_3d.py` & `colossalai-nightly-2023.7.8/colossalai/context/process_group_initializer/initializer_3d.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/context/process_group_initializer/initializer_data.py` & `colossalai-nightly-2023.7.8/colossalai/context/process_group_initializer/initializer_data.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/context/process_group_initializer/initializer_model.py` & `colossalai-nightly-2023.7.8/colossalai/context/process_group_initializer/initializer_model.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/context/process_group_initializer/initializer_pipeline.py` & `colossalai-nightly-2023.7.8/colossalai/context/process_group_initializer/initializer_pipeline.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/context/process_group_initializer/initializer_sequence.py` & `colossalai-nightly-2023.7.8/colossalai/context/process_group_initializer/initializer_sequence.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/context/process_group_initializer/initializer_tensor.py` & `colossalai-nightly-2023.7.8/colossalai/context/process_group_initializer/initializer_tensor.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/context/process_group_initializer/process_group_initializer.py` & `colossalai-nightly-2023.7.8/colossalai/context/process_group_initializer/process_group_initializer.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/context/random/_helper.py` & `colossalai-nightly-2023.7.8/colossalai/context/random/_helper.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/context/random/seed_manager.py` & `colossalai-nightly-2023.7.8/colossalai/context/random/seed_manager.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/context/singleton_meta.py` & `colossalai-nightly-2023.7.8/colossalai/context/singleton_meta.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/device/alpha_beta_profiler.py` & `colossalai-nightly-2023.7.8/colossalai/device/alpha_beta_profiler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/device/calc_pipeline_strategy.py` & `colossalai-nightly-2023.7.8/colossalai/device/calc_pipeline_strategy.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/engine/_base_engine.py` & `colossalai-nightly-2023.7.8/colossalai/engine/_base_engine.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/engine/gradient_accumulation/__init__.py` & `colossalai-nightly-2023.7.8/colossalai/engine/gradient_accumulation/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/engine/gradient_accumulation/_gradient_accumulation.py` & `colossalai-nightly-2023.7.8/colossalai/engine/gradient_accumulation/_gradient_accumulation.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/engine/gradient_handler/__init__.py` & `colossalai-nightly-2023.7.8/colossalai/engine/gradient_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/engine/gradient_handler/_base_gradient_handler.py` & `colossalai-nightly-2023.7.8/colossalai/engine/gradient_handler/_base_gradient_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/engine/gradient_handler/_data_parallel_gradient_handler.py` & `colossalai-nightly-2023.7.8/colossalai/engine/gradient_handler/_data_parallel_gradient_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/engine/gradient_handler/_moe_gradient_handler.py` & `colossalai-nightly-2023.7.8/colossalai/engine/gradient_handler/_moe_gradient_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/engine/gradient_handler/_pipeline_parallel_gradient_handler.py` & `colossalai-nightly-2023.7.8/colossalai/engine/gradient_handler/_pipeline_parallel_gradient_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/engine/gradient_handler/_sequence_parallel_gradient_handler.py` & `colossalai-nightly-2023.7.8/colossalai/engine/gradient_handler/_sequence_parallel_gradient_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/engine/gradient_handler/_zero_gradient_handler.py` & `colossalai-nightly-2023.7.8/colossalai/engine/gradient_handler/_zero_gradient_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/engine/gradient_handler/utils.py` & `colossalai-nightly-2023.7.8/colossalai/engine/gradient_handler/utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/engine/schedule/_base_schedule.py` & `colossalai-nightly-2023.7.8/colossalai/engine/schedule/_base_schedule.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/engine/schedule/_non_pipeline_schedule.py` & `colossalai-nightly-2023.7.8/colossalai/engine/schedule/_non_pipeline_schedule.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/engine/schedule/_pipeline_schedule.py` & `colossalai-nightly-2023.7.8/colossalai/engine/schedule/_pipeline_schedule.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/engine/schedule/_pipeline_schedule_v2.py` & `colossalai-nightly-2023.7.8/colossalai/engine/schedule/_pipeline_schedule_v2.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/fx/_compatibility.py` & `colossalai-nightly-2023.7.8/colossalai/fx/_compatibility.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/fx/_meta_regist_12.py` & `colossalai-nightly-2023.7.8/colossalai/fx/_meta_regist_12.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/fx/_meta_regist_13.py` & `colossalai-nightly-2023.7.8/colossalai/fx/_meta_regist_13.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/fx/codegen/activation_checkpoint_codegen.py` & `colossalai-nightly-2023.7.8/colossalai/fx/codegen/activation_checkpoint_codegen.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/fx/graph_module.py` & `colossalai-nightly-2023.7.8/colossalai/fx/graph_module.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/fx/passes/adding_split_node_pass.py` & `colossalai-nightly-2023.7.8/colossalai/fx/passes/adding_split_node_pass.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/fx/passes/concrete_info_prop.py` & `colossalai-nightly-2023.7.8/colossalai/fx/passes/concrete_info_prop.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/fx/passes/meta_info_prop.py` & `colossalai-nightly-2023.7.8/colossalai/fx/passes/meta_info_prop.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/fx/passes/passes_for_gpt2_test.py` & `colossalai-nightly-2023.7.8/colossalai/fx/passes/passes_for_gpt2_test.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/fx/passes/shard_1d_pass.py` & `colossalai-nightly-2023.7.8/colossalai/fx/passes/shard_1d_pass.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/fx/passes/split_module.py` & `colossalai-nightly-2023.7.8/colossalai/fx/passes/split_module.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/fx/passes/utils.py` & `colossalai-nightly-2023.7.8/colossalai/fx/passes/utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/fx/profiler/__init__.py` & `colossalai-nightly-2023.7.8/colossalai/fx/profiler/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/fx/profiler/constants.py` & `colossalai-nightly-2023.7.8/colossalai/fx/profiler/constants.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/fx/profiler/dataflow.py` & `colossalai-nightly-2023.7.8/colossalai/fx/profiler/dataflow.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/fx/profiler/experimental/constants.py` & `colossalai-nightly-2023.7.8/colossalai/fx/profiler/experimental/constants.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/fx/profiler/experimental/profiler.py` & `colossalai-nightly-2023.7.8/colossalai/fx/profiler/experimental/profiler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/fx/profiler/experimental/profiler_function/activation_function.py` & `colossalai-nightly-2023.7.8/colossalai/fx/profiler/experimental/profiler_function/activation_function.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/fx/profiler/experimental/profiler_function/arithmetic.py` & `colossalai-nightly-2023.7.8/colossalai/fx/profiler/experimental/profiler_function/arithmetic.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/fx/profiler/experimental/profiler_function/embedding.py` & `colossalai-nightly-2023.7.8/colossalai/fx/profiler/experimental/profiler_function/embedding.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/fx/profiler/experimental/profiler_function/normalization.py` & `colossalai-nightly-2023.7.8/colossalai/fx/profiler/experimental/profiler_function/normalization.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/fx/profiler/experimental/profiler_function/pooling.py` & `colossalai-nightly-2023.7.8/colossalai/fx/profiler/experimental/profiler_function/pooling.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/fx/profiler/experimental/profiler_function/torch_ops.py` & `colossalai-nightly-2023.7.8/colossalai/fx/profiler/experimental/profiler_function/torch_ops.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/fx/profiler/experimental/profiler_module/activation_function.py` & `colossalai-nightly-2023.7.8/colossalai/fx/profiler/experimental/profiler_module/activation_function.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/fx/profiler/experimental/profiler_module/attention.py` & `colossalai-nightly-2023.7.8/colossalai/fx/profiler/experimental/profiler_module/attention.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/fx/profiler/experimental/profiler_module/convolution.py` & `colossalai-nightly-2023.7.8/colossalai/fx/profiler/experimental/profiler_module/convolution.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/fx/profiler/experimental/profiler_module/normalization.py` & `colossalai-nightly-2023.7.8/colossalai/fx/profiler/experimental/profiler_module/normalization.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/fx/profiler/experimental/profiler_module/pooling.py` & `colossalai-nightly-2023.7.8/colossalai/fx/profiler/experimental/profiler_module/pooling.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/fx/profiler/experimental/profiler_module/rnn.py` & `colossalai-nightly-2023.7.8/colossalai/fx/profiler/experimental/profiler_module/rnn.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/fx/profiler/experimental/registry.py` & `colossalai-nightly-2023.7.8/colossalai/fx/profiler/experimental/registry.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/fx/profiler/experimental/shard_utils.py` & `colossalai-nightly-2023.7.8/colossalai/fx/profiler/experimental/shard_utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/fx/profiler/memory_utils.py` & `colossalai-nightly-2023.7.8/colossalai/fx/profiler/memory_utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/fx/profiler/opcount.py` & `colossalai-nightly-2023.7.8/colossalai/fx/profiler/opcount.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/fx/profiler/profiler.py` & `colossalai-nightly-2023.7.8/colossalai/fx/profiler/profiler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/fx/profiler/shard_utils.py` & `colossalai-nightly-2023.7.8/colossalai/fx/profiler/shard_utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/fx/profiler/tensor.py` & `colossalai-nightly-2023.7.8/colossalai/fx/profiler/tensor.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/fx/proxy.py` & `colossalai-nightly-2023.7.8/colossalai/fx/proxy.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/fx/tracer/_meta_trace.py` & `colossalai-nightly-2023.7.8/colossalai/fx/tracer/_meta_trace.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/fx/tracer/_symbolic_trace.py` & `colossalai-nightly-2023.7.8/colossalai/fx/tracer/_symbolic_trace.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/fx/tracer/_tracer_utils.py` & `colossalai-nightly-2023.7.8/colossalai/fx/tracer/_tracer_utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_function/addbmm.py` & `colossalai-nightly-2023.7.8/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_function/addbmm.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_function/addmm.py` & `colossalai-nightly-2023.7.8/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_function/addmm.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_function/bias_addition_function.py` & `colossalai-nightly-2023.7.8/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_function/bias_addition_function.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_function/linear.py` & `colossalai-nightly-2023.7.8/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_function/linear.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_module/bias_addition_module.py` & `colossalai-nightly-2023.7.8/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_module/bias_addition_module.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_module/conv.py` & `colossalai-nightly-2023.7.8/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_module/conv.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_module/linear.py` & `colossalai-nightly-2023.7.8/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_module/linear.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/fx/tracer/experimental.py` & `colossalai-nightly-2023.7.8/colossalai/fx/tracer/experimental.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/fx/tracer/meta_patch/patched_function/arithmetic.py` & `colossalai-nightly-2023.7.8/colossalai/fx/tracer/meta_patch/patched_function/arithmetic.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/fx/tracer/meta_patch/patched_function/convolution.py` & `colossalai-nightly-2023.7.8/colossalai/fx/tracer/meta_patch/patched_function/convolution.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/fx/tracer/meta_patch/patched_function/embedding.py` & `colossalai-nightly-2023.7.8/colossalai/fx/tracer/meta_patch/patched_function/embedding.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/fx/tracer/meta_patch/patched_function/normalization.py` & `colossalai-nightly-2023.7.8/colossalai/fx/tracer/meta_patch/patched_function/normalization.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/fx/tracer/meta_patch/patched_function/python_ops.py` & `colossalai-nightly-2023.7.8/colossalai/fx/tracer/meta_patch/patched_function/python_ops.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/fx/tracer/meta_patch/patched_function/torch_ops.py` & `colossalai-nightly-2023.7.8/colossalai/fx/tracer/meta_patch/patched_function/torch_ops.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/fx/tracer/meta_patch/patched_module/convolution.py` & `colossalai-nightly-2023.7.8/colossalai/fx/tracer/meta_patch/patched_module/convolution.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/fx/tracer/meta_patch/patched_module/normalization.py` & `colossalai-nightly-2023.7.8/colossalai/fx/tracer/meta_patch/patched_module/normalization.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/fx/tracer/meta_patch/patched_module/pooling.py` & `colossalai-nightly-2023.7.8/colossalai/fx/tracer/meta_patch/patched_module/pooling.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/fx/tracer/meta_patch/patched_module/rnn.py` & `colossalai-nightly-2023.7.8/colossalai/fx/tracer/meta_patch/patched_module/rnn.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/fx/tracer/registry.py` & `colossalai-nightly-2023.7.8/colossalai/fx/tracer/registry.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/fx/tracer/tracer.py` & `colossalai-nightly-2023.7.8/colossalai/fx/tracer/tracer.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/global_variables.py` & `colossalai-nightly-2023.7.8/colossalai/global_variables.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/initialize.py` & `colossalai-nightly-2023.7.8/colossalai/initialize.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/interface/model.py` & `colossalai-nightly-2023.7.8/colossalai/interface/model.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/interface/optimizer.py` & `colossalai-nightly-2023.7.8/colossalai/interface/optimizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -115,7 +115,13 @@
         """
         Unscale the gradients for mixed precision training.
 
         Note: Only available for optimizers with mixed precision training.
         """
         raise NotImplementedError(
             "The method unscale_grad is only available for optimizers with mixed precision training")
+
+    def unwrap(self):
+        """
+        Unwrap the optimizer for checkpoint saving/loading.
+        """
+        return self.optim
```

### Comparing `colossalai-nightly-2023.7.1/colossalai/kernel/cuda_native/csrc/colossal_C_frontend.cpp` & `colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/colossal_C_frontend.cpp`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/kernel/cuda_native/csrc/cpu_adam.cpp` & `colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/cpu_adam.cpp`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/kernel/cuda_native/csrc/cpu_adam.h` & `colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/cpu_adam.h`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/kernel/cuda_native/csrc/kernels/cross_entropy.cu` & `colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/kernels/cross_entropy.cu`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/kernel/cuda_native/csrc/kernels/cublas_wrappers.cu` & `colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/kernels/cublas_wrappers.cu`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/kernel/cuda_native/csrc/kernels/cuda_util.cu` & `colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/kernels/cuda_util.cu`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/kernel/cuda_native/csrc/kernels/dropout_kernels.cu` & `colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/kernels/dropout_kernels.cu`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/kernel/cuda_native/csrc/kernels/general_kernels.cu` & `colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/kernels/general_kernels.cu`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/kernel/cuda_native/csrc/kernels/include/block_reduce.h` & `colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/kernels/include/block_reduce.h`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/kernel/cuda_native/csrc/kernels/include/context.h` & `colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/kernels/include/context.h`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/kernel/cuda_native/csrc/kernels/include/cross_entropy_layer.h` & `colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/kernels/include/cross_entropy_layer.h`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/kernel/cuda_native/csrc/kernels/include/cublas_wrappers.h` & `colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/kernels/include/cublas_wrappers.h`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/kernel/cuda_native/csrc/kernels/include/cuda_util.h` & `colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/kernels/include/cuda_util.h`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/kernel/cuda_native/csrc/kernels/include/dropout.h` & `colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/kernels/include/dropout.h`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/kernel/cuda_native/csrc/kernels/include/feed_forward.h` & `colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/kernels/include/feed_forward.h`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/kernel/cuda_native/csrc/kernels/include/kernels.h` & `colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/kernels/include/kernels.h`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/kernel/cuda_native/csrc/kernels/include/normalize_layer.h` & `colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/kernels/include/normalize_layer.h`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/kernel/cuda_native/csrc/kernels/include/softmax.h` & `colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/kernels/include/softmax.h`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/kernel/cuda_native/csrc/kernels/include/strided_batch_gemm.h` & `colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/kernels/include/strided_batch_gemm.h`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/kernel/cuda_native/csrc/kernels/normalize_kernels.cu` & `colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/kernels/normalize_kernels.cu`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/kernel/cuda_native/csrc/kernels/softmax_kernels.cu` & `colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/kernels/softmax_kernels.cu`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/kernel/cuda_native/csrc/kernels/transform_kernels.cu` & `colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/kernels/transform_kernels.cu`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/kernel/cuda_native/csrc/layer_norm_cuda.cpp` & `colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/layer_norm_cuda.cpp`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/kernel/cuda_native/csrc/layer_norm_cuda_kernel.cu` & `colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/layer_norm_cuda_kernel.cu`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/kernel/cuda_native/csrc/moe_cuda.cpp` & `colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/moe_cuda.cpp`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/kernel/cuda_native/csrc/moe_cuda_kernel.cu` & `colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/moe_cuda_kernel.cu`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/kernel/cuda_native/csrc/multi_tensor_adam.cu` & `colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/multi_tensor_adam.cu`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/kernel/cuda_native/csrc/multi_tensor_apply.cuh` & `colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/multi_tensor_apply.cuh`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/kernel/cuda_native/csrc/multi_tensor_l2norm_kernel.cu` & `colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/multi_tensor_l2norm_kernel.cu`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/kernel/cuda_native/csrc/multi_tensor_lamb.cu` & `colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/multi_tensor_lamb.cu`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/kernel/cuda_native/csrc/multi_tensor_scale_kernel.cu` & `colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/multi_tensor_scale_kernel.cu`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/kernel/cuda_native/csrc/multi_tensor_sgd_kernel.cu` & `colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/multi_tensor_sgd_kernel.cu`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/kernel/cuda_native/csrc/multihead_attention_1d.cpp` & `colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/multihead_attention_1d.cpp`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/kernel/cuda_native/csrc/multihead_attention_1d.h` & `colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/multihead_attention_1d.h`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/kernel/cuda_native/csrc/scaled_masked_softmax.cpp` & `colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/scaled_masked_softmax.cpp`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/kernel/cuda_native/csrc/scaled_masked_softmax.h` & `colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/scaled_masked_softmax.h`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/kernel/cuda_native/csrc/scaled_masked_softmax_cuda.cu` & `colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/scaled_masked_softmax_cuda.cu`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/kernel/cuda_native/csrc/scaled_upper_triang_masked_softmax.cpp` & `colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/scaled_upper_triang_masked_softmax.cpp`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/kernel/cuda_native/csrc/scaled_upper_triang_masked_softmax.h` & `colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/scaled_upper_triang_masked_softmax.h`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/kernel/cuda_native/csrc/scaled_upper_triang_masked_softmax_cuda.cu` & `colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/scaled_upper_triang_masked_softmax_cuda.cu`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/kernel/cuda_native/csrc/type_shim.h` & `colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/type_shim.h`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/kernel/cuda_native/flash_attention.py` & `colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/flash_attention.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/kernel/cuda_native/layer_norm.py` & `colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/layer_norm.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/kernel/cuda_native/multihead_attention.py` & `colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/multihead_attention.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/kernel/cuda_native/scaled_softmax.py` & `colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/scaled_softmax.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/kernel/jit/bias_dropout_add.py` & `colossalai-nightly-2023.7.8/colossalai/kernel/jit/bias_dropout_add.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import torch
+from torch import Tensor
 
 
 def bias_dropout_add(x, bias, residual, prob, training):
     # type: (Tensor, Tensor, Tensor, float, bool) -> Tensor
     out = torch.nn.functional.dropout(x + bias, p=prob, training=training)
     out = residual + out
     return out
```

### Comparing `colossalai-nightly-2023.7.1/colossalai/kernel/jit/bias_gelu.py` & `colossalai-nightly-2023.7.8/colossalai/kernel/jit/bias_gelu.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/kernel/jit/option.py` & `colossalai-nightly-2023.7.8/colossalai/kernel/jit/option.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/kernel/op_builder/__init__.py` & `colossalai-nightly-2023.7.8/colossalai/kernel/op_builder/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/kernel/op_builder/builder.py` & `colossalai-nightly-2023.7.8/colossalai/kernel/op_builder/builder.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/kernel/op_builder/cpu_adam.py` & `colossalai-nightly-2023.7.8/colossalai/kernel/op_builder/cpu_adam.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/kernel/op_builder/fused_optim.py` & `colossalai-nightly-2023.7.8/colossalai/kernel/op_builder/fused_optim.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/kernel/op_builder/layernorm.py` & `colossalai-nightly-2023.7.8/colossalai/kernel/op_builder/layernorm.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/kernel/op_builder/moe.py` & `colossalai-nightly-2023.7.8/colossalai/kernel/op_builder/moe.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/kernel/op_builder/multi_head_attn.py` & `colossalai-nightly-2023.7.8/colossalai/kernel/op_builder/multi_head_attn.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/kernel/op_builder/scaled_masked_softmax.py` & `colossalai-nightly-2023.7.8/colossalai/kernel/op_builder/scaled_masked_softmax.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/kernel/op_builder/scaled_upper_triangle_masked_softmax.py` & `colossalai-nightly-2023.7.8/colossalai/kernel/op_builder/scaled_upper_triangle_masked_softmax.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/kernel/op_builder/utils.py` & `colossalai-nightly-2023.7.8/colossalai/kernel/op_builder/utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/lazy/lazy_init.py` & `colossalai-nightly-2023.7.8/colossalai/lazy/lazy_init.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 from types import MethodType
-from typing import Callable, Optional, Union
+from typing import Callable, Dict, Optional, Union
 
 import torch
 import torch.distributed as dist
 import torch.nn as nn
 from torch import Tensor
 from torch.utils._pytree import tree_map
 
 from colossalai._analyzer._subclasses import MetaTensor
-from colossalai.tensor.d_tensor.d_tensor import DTensor
-from colossalai.tensor.d_tensor.layout import Layout
+from colossalai.device.device_mesh import DeviceMesh
+from colossalai.tensor.d_tensor import distribute_tensor
+from colossalai.tensor.d_tensor.sharding_spec import ShardingSpec
 
 # reference: https://pytorch.org/cppdocs/notes/tensor_creation.html
 _NORMAL_FACTORY = [
     "arange",
     "full",
     "empty",
     "linspace",
@@ -168,26 +169,26 @@
         Returns:
             torch.Tensor: The materialized tensor (self).
         """
         target = self._materialize_data()
         self.clean()
         return _convert_cls(self, target)
 
-    def distribute(self, layout: Layout) -> torch.Tensor:
+    def distribute(self, device_mesh: DeviceMesh, sharding_spec: ShardingSpec) -> torch.Tensor:
         """Distribute the ``LazyTensor`` to ``torch.Tensor`` by modifying __class__ (inplace), according to the layout.
 
         Args:
             layout (Layout): Distribution layout.
 
         Returns:
             torch.Tensor: The distributed tensor (self).
         """
         target = self._materialize_data()
         self.clean()
-        local_tensor = DTensor(target, layout).local_tensor
+        local_tensor = distribute_tensor(target, device_mesh, sharding_spec)
         return _convert_cls(self, local_tensor)
 
     def clean(self) -> None:
         """Clean all stored operations, meta data and materialized data, which prevents memory leaking. This should be called after all tensors are materialized.
         """
         self._factory_method = None
         self._op_buffer = None
@@ -532,25 +533,28 @@
 
         def apply_fn(name: str, p: LazyTensor):
             p.materialize()
 
         return _apply_to_lazy_module(module, apply_fn, verbose)
 
     @staticmethod
-    def distribute(module: nn.Module, layout_dict: dict, verbose: bool = False) -> nn.Module:
+    def distribute(module: nn.Module,
+                   device_mesh: DeviceMesh,
+                   sharding_spec_dict: Dict[str, ShardingSpec],
+                   verbose: bool = False) -> nn.Module:
         """Distribute all ``nn.Parameter`` from ``LazyTensor``. This function will modify the module in-place.
 
         Args:
             module (nn.Module): Target ``nn.Module``
             layout_dict (dict): Dict of layout for each parameter/buffer. The key is the parameter/buffer name, and the value is the layout.
             verbose (bool, optional): Whether to print lazy initialization rate. Defaults to False.
         """
 
         def apply_fn(name: str, p: LazyTensor):
-            p.distribute(layout_dict[name])
+            p.distribute(device_mesh, sharding_spec_dict[name])
 
         return _apply_to_lazy_module(module, apply_fn, verbose)
 
 
 def _apply_to_lazy_module(module: nn.Module,
                           apply_fn: Callable[[str, torch.Tensor], None],
                           verbose: bool = False) -> nn.Module:
```

### Comparing `colossalai-nightly-2023.7.1/colossalai/logging/__init__.py` & `colossalai-nightly-2023.7.8/colossalai/logging/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/logging/logger.py` & `colossalai-nightly-2023.7.8/colossalai/logging/logger.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/nn/_ops/_utils.py` & `colossalai-nightly-2023.7.8/colossalai/nn/_ops/_utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/nn/_ops/addmm.py` & `colossalai-nightly-2023.7.8/colossalai/nn/_ops/addmm.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/nn/_ops/batch_norm.py` & `colossalai-nightly-2023.7.8/colossalai/nn/_ops/batch_norm.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/nn/_ops/element_wise.py` & `colossalai-nightly-2023.7.8/colossalai/nn/_ops/element_wise.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/nn/_ops/embedding.py` & `colossalai-nightly-2023.7.8/colossalai/nn/_ops/embedding.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/nn/_ops/embedding_bag.py` & `colossalai-nightly-2023.7.8/colossalai/nn/_ops/embedding_bag.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/nn/_ops/layernorm.py` & `colossalai-nightly-2023.7.8/colossalai/nn/_ops/layernorm.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/nn/_ops/linear.py` & `colossalai-nightly-2023.7.8/colossalai/nn/_ops/linear.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/nn/_ops/loss.py` & `colossalai-nightly-2023.7.8/colossalai/nn/_ops/loss.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/nn/_ops/view.py` & `colossalai-nightly-2023.7.8/colossalai/nn/_ops/view.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/nn/init.py` & `colossalai-nightly-2023.7.8/colossalai/nn/init.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/nn/layer/base_layer.py` & `colossalai-nightly-2023.7.8/colossalai/nn/layer/base_layer.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 import torch.nn as nn
 
 from colossalai.context import ParallelMode
 from colossalai.core import global_context as gpc
 
 
 class ParallelLayer(nn.Module):
+
     global_state_dict: bool = True
 
     def __init__(self):
         super().__init__()
         self.data_parallel_rank = 0 if not gpc.is_initialized(ParallelMode.DATA) else gpc.get_local_rank(
             ParallelMode.DATA)
         self.data_parallel_size = 1 if not gpc.is_initialized(ParallelMode.DATA) else gpc.get_world_size(
```

### Comparing `colossalai-nightly-2023.7.1/colossalai/nn/layer/colossalai_layer/_utils.py` & `colossalai-nightly-2023.7.8/colossalai/nn/layer/colossalai_layer/_utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/nn/layer/colossalai_layer/dropout.py` & `colossalai-nightly-2023.7.8/colossalai/nn/layer/colossalai_layer/dropout.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/nn/layer/colossalai_layer/embedding.py` & `colossalai-nightly-2023.7.8/colossalai/nn/layer/colossalai_layer/embedding.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/nn/layer/colossalai_layer/linear.py` & `colossalai-nightly-2023.7.8/colossalai/nn/layer/colossalai_layer/linear.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/nn/layer/colossalai_layer/normalization.py` & `colossalai-nightly-2023.7.8/colossalai/nn/layer/colossalai_layer/normalization.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/nn/layer/moe/__init__.py` & `colossalai-nightly-2023.7.8/colossalai/nn/layer/moe/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/nn/layer/moe/_operation.py` & `colossalai-nightly-2023.7.8/colossalai/nn/layer/moe/_operation.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/nn/layer/moe/checkpoint.py` & `colossalai-nightly-2023.7.8/colossalai/nn/layer/moe/checkpoint.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/nn/layer/moe/experts.py` & `colossalai-nightly-2023.7.8/colossalai/nn/layer/moe/experts.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/nn/layer/moe/layers.py` & `colossalai-nightly-2023.7.8/colossalai/nn/layer/moe/layers.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/nn/layer/moe/routers.py` & `colossalai-nightly-2023.7.8/colossalai/nn/layer/moe/routers.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/nn/layer/moe/utils.py` & `colossalai-nightly-2023.7.8/colossalai/nn/layer/moe/utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/nn/layer/parallel_1d/_operation.py` & `colossalai-nightly-2023.7.8/colossalai/nn/layer/parallel_1d/_operation.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import torch
 import torch.distributed as dist
+
 from colossalai.core import global_context as gpc
 
 try:
     import fused_mix_prec_layer_norm_cuda
 except:
     fused_mix_prec_layer_norm_cuda = None
```

### Comparing `colossalai-nightly-2023.7.1/colossalai/nn/layer/parallel_1d/_utils.py` & `colossalai-nightly-2023.7.8/colossalai/nn/layer/parallel_1d/_utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/nn/layer/parallel_1d/layers.py` & `colossalai-nightly-2023.7.8/colossalai/nn/layer/parallel_1d/layers.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/nn/layer/parallel_2d/_operation.py` & `colossalai-nightly-2023.7.8/colossalai/nn/layer/parallel_2d/_operation.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/nn/layer/parallel_2d/_utils.py` & `colossalai-nightly-2023.7.8/colossalai/nn/layer/parallel_2d/_utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/nn/layer/parallel_2d/layers.py` & `colossalai-nightly-2023.7.8/colossalai/nn/layer/parallel_2d/layers.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/nn/layer/parallel_2p5d/_operation.py` & `colossalai-nightly-2023.7.8/colossalai/nn/layer/parallel_2p5d/_operation.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/nn/layer/parallel_2p5d/_utils.py` & `colossalai-nightly-2023.7.8/colossalai/nn/layer/parallel_2p5d/_utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/nn/layer/parallel_2p5d/layers.py` & `colossalai-nightly-2023.7.8/colossalai/nn/layer/parallel_2p5d/layers.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/nn/layer/parallel_3d/_operation.py` & `colossalai-nightly-2023.7.8/colossalai/nn/layer/parallel_3d/_operation.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/nn/layer/parallel_3d/_utils.py` & `colossalai-nightly-2023.7.8/colossalai/nn/layer/parallel_3d/_utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/nn/layer/parallel_3d/layers.py` & `colossalai-nightly-2023.7.8/colossalai/nn/layer/parallel_3d/layers.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/nn/layer/parallel_sequence/_operation.py` & `colossalai-nightly-2023.7.8/colossalai/nn/layer/parallel_sequence/_operation.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/nn/layer/parallel_sequence/layers.py` & `colossalai-nightly-2023.7.8/colossalai/nn/layer/parallel_sequence/layers.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/nn/layer/utils/common.py` & `colossalai-nightly-2023.7.8/colossalai/nn/layer/utils/common.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/nn/layer/vanilla/layers.py` & `colossalai-nightly-2023.7.8/colossalai/nn/layer/vanilla/layers.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/nn/layer/wrapper/pipeline_wrapper.py` & `colossalai-nightly-2023.7.8/colossalai/nn/layer/wrapper/pipeline_wrapper.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/nn/loss/__init__.py` & `colossalai-nightly-2023.7.8/colossalai/nn/loss/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/nn/loss/loss_1d.py` & `colossalai-nightly-2023.7.8/colossalai/nn/loss/loss_1d.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/nn/loss/loss_2d.py` & `colossalai-nightly-2023.7.8/colossalai/nn/loss/loss_2d.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/nn/loss/loss_2p5d.py` & `colossalai-nightly-2023.7.8/colossalai/nn/loss/loss_2p5d.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/nn/loss/loss_3d.py` & `colossalai-nightly-2023.7.8/colossalai/nn/loss/loss_3d.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/nn/loss/loss_moe.py` & `colossalai-nightly-2023.7.8/colossalai/nn/loss/loss_moe.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/nn/lr_scheduler/__init__.py` & `colossalai-nightly-2023.7.8/colossalai/nn/lr_scheduler/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/nn/lr_scheduler/cosine.py` & `colossalai-nightly-2023.7.8/colossalai/nn/lr_scheduler/cosine.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/nn/lr_scheduler/delayed.py` & `colossalai-nightly-2023.7.8/colossalai/nn/lr_scheduler/delayed.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/nn/lr_scheduler/linear.py` & `colossalai-nightly-2023.7.8/colossalai/nn/lr_scheduler/linear.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/nn/lr_scheduler/multistep.py` & `colossalai-nightly-2023.7.8/colossalai/nn/lr_scheduler/multistep.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/nn/lr_scheduler/onecycle.py` & `colossalai-nightly-2023.7.8/colossalai/nn/lr_scheduler/onecycle.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/nn/lr_scheduler/poly.py` & `colossalai-nightly-2023.7.8/colossalai/nn/lr_scheduler/poly.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/nn/lr_scheduler/torch.py` & `colossalai-nightly-2023.7.8/colossalai/nn/lr_scheduler/torch.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/nn/metric/__init__.py` & `colossalai-nightly-2023.7.8/colossalai/nn/metric/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/nn/metric/accuracy_2d.py` & `colossalai-nightly-2023.7.8/colossalai/nn/metric/accuracy_2d.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/nn/metric/accuracy_2p5d.py` & `colossalai-nightly-2023.7.8/colossalai/nn/metric/accuracy_2p5d.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/nn/metric/accuracy_3d.py` & `colossalai-nightly-2023.7.8/colossalai/nn/metric/accuracy_3d.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/nn/optimizer/colossalai_optimizer.py` & `colossalai-nightly-2023.7.8/colossalai/nn/optimizer/colossalai_optimizer.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/nn/optimizer/cpu_adam.py` & `colossalai-nightly-2023.7.8/colossalai/nn/optimizer/cpu_adam.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/nn/optimizer/fused_adam.py` & `colossalai-nightly-2023.7.8/colossalai/nn/optimizer/fused_adam.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/nn/optimizer/fused_lamb.py` & `colossalai-nightly-2023.7.8/colossalai/nn/optimizer/fused_lamb.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/nn/optimizer/fused_sgd.py` & `colossalai-nightly-2023.7.8/colossalai/nn/optimizer/fused_sgd.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/nn/optimizer/hybrid_adam.py` & `colossalai-nightly-2023.7.8/colossalai/nn/optimizer/hybrid_adam.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/nn/optimizer/lamb.py` & `colossalai-nightly-2023.7.8/colossalai/nn/optimizer/lamb.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/nn/optimizer/lars.py` & `colossalai-nightly-2023.7.8/colossalai/nn/optimizer/lars.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/nn/optimizer/nvme_optimizer.py` & `colossalai-nightly-2023.7.8/colossalai/nn/optimizer/nvme_optimizer.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/nn/parallel/data_parallel.py` & `colossalai-nightly-2023.7.8/colossalai/nn/parallel/data_parallel.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/nn/parallel/layers/__init__.py` & `colossalai-nightly-2023.7.8/colossalai/nn/parallel/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/nn/parallel/layers/cache_embedding/__init__.py` & `colossalai-nightly-2023.7.8/colossalai/nn/parallel/layers/cache_embedding/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/nn/parallel/layers/cache_embedding/base_embedding.py` & `colossalai-nightly-2023.7.8/colossalai/nn/parallel/layers/cache_embedding/base_embedding.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/nn/parallel/layers/cache_embedding/cache_mgr.py` & `colossalai-nightly-2023.7.8/colossalai/nn/parallel/layers/cache_embedding/cache_mgr.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/nn/parallel/layers/cache_embedding/cached_embedding.py` & `colossalai-nightly-2023.7.8/colossalai/nn/parallel/layers/cache_embedding/cached_embedding.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/nn/parallel/layers/cache_embedding/copyer.py` & `colossalai-nightly-2023.7.8/colossalai/nn/parallel/layers/cache_embedding/copyer.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/nn/parallel/layers/cache_embedding/embedding_config.py` & `colossalai-nightly-2023.7.8/colossalai/nn/parallel/layers/cache_embedding/embedding_config.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/nn/parallel/layers/cache_embedding/parallel_cached_embedding.py` & `colossalai-nightly-2023.7.8/colossalai/nn/parallel/layers/cache_embedding/parallel_cached_embedding.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/nn/parallel/layers/cache_embedding/parallel_cached_embedding_tablewise.py` & `colossalai-nightly-2023.7.8/colossalai/nn/parallel/layers/cache_embedding/parallel_cached_embedding_tablewise.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/nn/parallel/layers/cache_embedding/parallel_cached_embedding_tablewise_split_cache.py` & `colossalai-nightly-2023.7.8/colossalai/nn/parallel/layers/cache_embedding/parallel_cached_embedding_tablewise_split_cache.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/nn/parallel/layers/colo_module.py` & `colossalai-nightly-2023.7.8/colossalai/nn/parallel/layers/colo_module.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/nn/parallel/layers/embedding.py` & `colossalai-nightly-2023.7.8/colossalai/nn/parallel/layers/embedding.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/nn/parallel/layers/linear.py` & `colossalai-nightly-2023.7.8/colossalai/nn/parallel/layers/linear.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/nn/parallel/layers/module_utils.py` & `colossalai-nightly-2023.7.8/colossalai/nn/parallel/layers/module_utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/nn/parallel/reducer.py` & `colossalai-nightly-2023.7.8/colossalai/nn/parallel/reducer.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/pipeline/layer_spec.py` & `colossalai-nightly-2023.7.8/colossalai/pipeline/layer_spec.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/pipeline/middleware/adaptor/fx.py` & `colossalai-nightly-2023.7.8/colossalai/pipeline/middleware/adaptor/fx.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/pipeline/middleware/topo.py` & `colossalai-nightly-2023.7.8/colossalai/pipeline/middleware/topo.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/pipeline/pipelinable.py` & `colossalai-nightly-2023.7.8/colossalai/pipeline/pipelinable.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/pipeline/pipeline_process_group.py` & `colossalai-nightly-2023.7.8/colossalai/pipeline/pipeline_process_group.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/pipeline/rpc/_pipeline_base.py` & `colossalai-nightly-2023.7.8/colossalai/pipeline/rpc/_pipeline_base.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/pipeline/rpc/_pipeline_schedule.py` & `colossalai-nightly-2023.7.8/colossalai/pipeline/rpc/_pipeline_schedule.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/pipeline/rpc/utils.py` & `colossalai-nightly-2023.7.8/colossalai/pipeline/rpc/utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/pipeline/utils.py` & `colossalai-nightly-2023.7.8/colossalai/pipeline/utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/registry/__init__.py` & `colossalai-nightly-2023.7.8/colossalai/registry/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/registry/registry.py` & `colossalai-nightly-2023.7.8/colossalai/registry/registry.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/tensor/__init__.py` & `colossalai-nightly-2023.7.8/colossalai/tensor/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/tensor/colo_parameter.py` & `colossalai-nightly-2023.7.8/colossalai/tensor/colo_parameter.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/tensor/colo_tensor.py` & `colossalai-nightly-2023.7.8/colossalai/tensor/colo_tensor.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/tensor/comm_spec.py` & `colossalai-nightly-2023.7.8/colossalai/tensor/comm_spec.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,77 +12,74 @@
 ]
 
 
 def _all_gather(tensor, comm_spec):
     '''
     Implement all gather operation on device mesh based on information provided by comm_spec.
     '''
-    process_groups_list = comm_spec.device_mesh.process_groups_dict[comm_spec.logical_process_axis]
-    for rank_list, process_group in process_groups_list:
-        if dist.get_rank() in rank_list:
-            tensor_list = [
-                torch.zeros(tensor.shape, dtype=tensor.dtype, device=tensor.device)
-                for _ in range(comm_spec.device_mesh.mesh_shape[comm_spec.logical_process_axis])
-            ]
-            # without this contiguous operation, the all gather may get some unexpected results.
-            tensor = tensor.contiguous()
-            dist.all_gather(tensor_list, tensor, group=process_group)
-            output = torch.cat(tuple(tensor_list), comm_spec.gather_dim).contiguous()
-            return output
+    process_groups = comm_spec.device_mesh.get_process_group_for_all_axes()
+    process_group = process_groups[comm_spec.logical_process_axis]
+
+    tensor_list = [
+        torch.zeros(tensor.shape, dtype=tensor.dtype, device=tensor.device)
+        for _ in range(comm_spec.device_mesh.shape[comm_spec.logical_process_axis])
+    ]
+    # without this contiguous operation, the all gather may get some unexpected results.
+    tensor = tensor.contiguous()
+    dist.all_gather(tensor_list, tensor, group=process_group)
+    output = torch.cat(tuple(tensor_list), comm_spec.gather_dim).contiguous()
+    return output
 
 
 def _split(tensor, comm_spec):
     '''
     Implement shard operation on device mesh based on information provided by comm_spec.
     '''
-    process_groups_list = comm_spec.device_mesh.process_groups_dict[comm_spec.logical_process_axis]
-    for rank_list, _ in process_groups_list:
-        if dist.get_rank() in rank_list:
-            dim = comm_spec.shard_dim
-            length = tensor.shape[comm_spec.shard_dim] // len(rank_list)
-            start = length * rank_list.index(dist.get_rank())
-            output = torch.narrow(tensor, dim, start, length).contiguous()
-            return output
+    process_groups = comm_spec.device_mesh.get_process_group_for_all_axes()
+    process_group = process_groups[comm_spec.logical_process_axis]
+
+    dim = comm_spec.shard_dim
+    length = tensor.shape[comm_spec.shard_dim] // dist.get_world_size(process_group)
+    start = length * dist.get_rank(process_group)
+    output = torch.narrow(tensor, dim, start, length).contiguous()
+    return output
 
 
 def _all_to_all(tensor, comm_spec):
     '''
     Implement all to all operation on device mesh based on information provided by comm_spec.
     '''
-    process_groups_list = comm_spec.device_mesh.process_groups_dict[comm_spec.logical_process_axis]
-    for rank_list, process_group in process_groups_list:
-        if dist.get_rank() in rank_list:
-            new_shape = list(tensor.shape)
-            new_shape[comm_spec.shard_dim] = new_shape[comm_spec.shard_dim] // len(rank_list)
-            new_shape = torch.Size(new_shape)
-            output_tensor_list = [
-                torch.zeros(new_shape, dtype=tensor.dtype, device=tensor.device) for _ in range(len(rank_list))
-            ]
-            dim = comm_spec.shard_dim
-            length = tensor.shape[comm_spec.shard_dim] // len(rank_list)
-            input_tensor_list = [
-                torch.narrow(tensor, dim, length * i, length).contiguous() for i in range(len(rank_list))
-            ]
-            group = process_group
-            dist.all_to_all(output_tensor_list, input_tensor_list, group)
-            output = torch.cat(tuple(output_tensor_list), comm_spec.gather_dim).contiguous()
-            return output
+    process_groups = comm_spec.device_mesh.get_process_group_for_all_axes()
+    process_group = process_groups[comm_spec.logical_process_axis]
+    world_size = dist.get_world_size(process_group)
+
+    new_shape = list(tensor.shape)
+    new_shape[comm_spec.shard_dim] = new_shape[comm_spec.shard_dim] // world_size
+    new_shape = torch.Size(new_shape)
+    output_tensor_list = [torch.zeros(new_shape, dtype=tensor.dtype, device=tensor.device) for _ in range(world_size)]
+    dim = comm_spec.shard_dim
+    length = tensor.shape[comm_spec.shard_dim] // world_size
+    input_tensor_list = [torch.narrow(tensor, dim, length * i, length).contiguous() for i in range(world_size)]
+    group = process_group
+    dist.all_to_all(output_tensor_list, input_tensor_list, group)
+    output = torch.cat(tuple(output_tensor_list), comm_spec.gather_dim).contiguous()
+    return output
 
 
 def _all_reduce(tensor, comm_spec, async_op=False):
     '''
     Implement all reduce operation on device mesh based on information provided by comm_spec.
     '''
-    process_groups_list = comm_spec.device_mesh.process_groups_dict[comm_spec.logical_process_axis]
-    for rank_list, process_group in process_groups_list:
-        if dist.get_rank() in rank_list:
-            if not tensor.is_contiguous():
-                tensor = tensor.contiguous()
-            dist.all_reduce(tensor, op=ReduceOp.SUM, group=process_group, async_op=async_op)
-            return tensor
+    process_groups = comm_spec.device_mesh.get_process_group_for_all_axes()
+    process_group = process_groups[comm_spec.logical_process_axis]
+
+    if not tensor.is_contiguous():
+        tensor = tensor.contiguous()
+    dist.all_reduce(tensor, op=ReduceOp.SUM, group=process_group, async_op=async_op)
+    return tensor
 
 
 def _mix_gather(tensor, comm_spec):
     '''
     Implement mix gather operation on device mesh based on information provided by comm_spec.
     Mix gather is the all-gather operation on all devices in the device_mesh(FlattenDeviceMesh) of the comm_spec. It is
     different from _all_gather because _mix_gather does all-gather in two dimensions of device mesh, while _all_gather
@@ -124,15 +121,15 @@
     process_group = "[0, 4, 1, 5, 2, 6, 3, 7]"
     tensor_list = [(0,0),(1,0),(2,0),(3,0),(4,0),(5,0),(6,0),(7,0)]
     S01R:
     leading_group_dim = 1
     process_group = "[0, 1, 2, 3, 4, 5, 6, 7]"
     tensor_list = [(0,0),(1,0),(2,0),(3,0),(4,0),(5,0),(6,0),(7,0)]
     '''
-    total_slices = comm_spec.device_mesh.mesh_shape[0]
+    total_slices = comm_spec.device_mesh.shape[0]
     tensor_list = [torch.zeros(tensor.shape, dtype=tensor.dtype, device=tensor.device) for _ in range(total_slices)]
     leading_group_dim = comm_spec.logical_process_axes[0]
     assert len(comm_spec.device_mesh.process_groups_dict) == 1
     _, process_group = comm_spec.device_mesh.process_groups_dict[0][0]
     process_number_list = comm_spec.device_meshes.process_number_dict[leading_group_dim]
 
     # Global all_gather
@@ -145,15 +142,15 @@
     for i in range(total_slices):
         tensor_list_sorted[i] = tensor_list[process_number_list[i]]
     tensor_list = tensor_list_sorted
 
     if comm_spec.logical_process_axes[0] == comm_spec.logical_process_axes[1]:
         output = torch.cat(tuple(tensor_list), comm_spec.gather_dim[0]).contiguous()
     else:
-        mesh_shape = comm_spec.device_meshes.mesh_shape
+        mesh_shape = comm_spec.device_meshes.shape
         cat_slice = [mesh_shape[comm_spec.logical_process_axes[0]], mesh_shape[comm_spec.logical_process_axes[1]]]
         tmp_tensor_shape = list(tensor.shape)
         tmp_tensor_shape[comm_spec.gather_dim[0]] *= cat_slice[0]
         tmp_tensor_shape = torch.Size(tmp_tensor_shape)
         tmp_tensor_list = [
             torch.zeros(tmp_tensor_shape, dtype=tensor.dtype, device=tensor.device) for _ in range(cat_slice[1])
         ]
@@ -177,17 +174,17 @@
     RS01 => [b], (0, 0)
     Example:
     mesh_shape = (2,4)
             # [[0, 1, 2, 3],
             #  [4, 5, 6, 7]]
             # return {0: [0, 4, 1, 5, 2, 6, 3, 7], 1: [0, 1, 2, 3, 4, 5, 6, 7]}
     '''
-    mesh_shape = comm_spec.device_meshes.mesh_shape
+    mesh_shape = comm_spec.device_meshes.shape
     dim = comm_spec.gather_dim
-    total_slices = comm_spec.device_mesh.mesh_shape[0]
+    total_slices = comm_spec.device_mesh.shape[0]
 
     # Get global rank
     rank = dist.get_rank()
 
     leading_group_dim = comm_spec.logical_process_axes[0]
     process_number_list = comm_spec.device_meshes.process_number_dict[leading_group_dim]
     rank = process_number_list.index(rank)
@@ -410,15 +407,15 @@
         self.sharding_spec = sharding_spec
         self.gather_dim = gather_dim
         self.shard_dim = shard_dim
         self.logical_process_axis = logical_process_axis
         self.forward_only = forward_only
         if isinstance(self.logical_process_axis, list):
             if not mix_gather:
-                self.device_mesh = self.sharding_spec.device_mesh.flatten_device_mesh
+                self.device_mesh = self.sharding_spec.device_mesh.flatten()
                 self.logical_process_axis = 0
             else:
                 self.device_meshes = self.sharding_spec.device_mesh.flatten_device_meshes
                 self.device_mesh = self.sharding_spec.device_mesh.flatten_device_mesh
                 # Create a new member `logical_process_axes` to distinguish from original flatten
                 self.logical_process_axes = logical_process_axis
         else:
```

### Comparing `colossalai-nightly-2023.7.1/colossalai/tensor/compute_spec.py` & `colossalai-nightly-2023.7.8/colossalai/tensor/compute_spec.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/tensor/d_tensor/comm_spec.py` & `colossalai-nightly-2023.7.8/colossalai/tensor/d_tensor/comm_spec.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,36 +20,36 @@
     MIXGATHER_FWD_SPLIT_BWD = "mixgather_fwd_split_bwd"
 
 
 class CommSpec:
     '''
     Communication spec is used to record the communication action. It converts the communication spec
     to real action which will be used in runtime. It contains comm_pattern to determine the
-    communication method, process_groups_dict to determine the process groups, gather_dim and shard_dim
+    communication method, process_group_dict to determine the process groups, gather_dim and shard_dim
     to determine the buffer shape, and logical_process_axis
 
     Argument:
-        comm_pattern(CollectiveCommPattern): describe the communication method used in this spec.
-        process_groups_dict(Dict): A dict which contains the process groups used to apply this CommSpec.
+        comm_pattern(CollectiveCommPattern): decribe the communication method used in this spec.
+        process_group_dict(Dict): A dict which contains the process groups used to apply this CommSpec.
         gather_dim(int, Optional): The gather_dim of the tensor will be gathered.
         shard_dim(int, Optional): The shard_dim of the tensor will be sharded.
         logical_process_axis(Union(int, List[int]), Optional): The mesh_dim to implement the communication action.
     '''
 
     def __init__(self,
                  comm_pattern: CollectiveCommPattern,
-                 process_groups_dict: Dict,
+                 process_group_dict: Dict,
                  gather_dim: int = None,
                  shard_dim: int = None,
                  logical_process_axis: int = None):
         self.comm_pattern = comm_pattern
         self.gather_dim = gather_dim
         self.shard_dim = shard_dim
         self.logical_process_axis = logical_process_axis
-        self.process_groups_dict = process_groups_dict
+        self.process_group_dict = process_group_dict
 
     def __repr__(self):
         res_list = ["CommSpec:("]
         if self.comm_pattern == CollectiveCommPattern.GATHER_FWD_SPLIT_BWD:
             res_list.append(f"comm_pattern:GATHER_FWD_SPLIT_BWD, ")
             res_list.append(f"gather_dim:{self.gather_dim}, ")
             res_list.append(f"shard_dim:{self.gather_dim}, ")
@@ -88,76 +88,64 @@
         return tensor
 
 
 def _all_gather(tensor: torch.Tensor, comm_spec: CommSpec):
     '''
     Implement all gather operation on device mesh based on information provided by comm_spec.
     '''
-    process_groups_list = comm_spec.process_groups_dict[comm_spec.logical_process_axis]
-    for rank_list, process_group in process_groups_list:
-        if dist.get_rank() in rank_list:
-            tensor_list = [
-                torch.zeros(tensor.shape, dtype=tensor.dtype, device=tensor.device) for _ in range(len(rank_list))
-            ]
-            # without this contiguous operation, the all gather may get some unexpected results.
-            tensor = tensor.contiguous()
-            dist.all_gather(tensor_list, tensor, group=process_group)
-            output = torch.cat(tuple(tensor_list), comm_spec.gather_dim).contiguous()
-            return output
+    process_group = comm_spec.process_group_dict[comm_spec.logical_process_axis]
+    world_size = dist.get_world_size(process_group)
+    tensor_list = [torch.zeros(tensor.shape, dtype=tensor.dtype, device=tensor.device) for _ in range(world_size)]
+    # without this contiguous operation, the all gather may get some unexpected results.
+    tensor = tensor.contiguous()
+    dist.all_gather(tensor_list, tensor, group=process_group)
+    output = torch.cat(tuple(tensor_list), comm_spec.gather_dim).contiguous()
+    return output
 
 
 def _split(tensor: torch.Tensor, comm_spec: CommSpec):
     '''
     Implement shard operation on device mesh based on information provided by comm_spec.
     '''
-    process_groups_list = comm_spec.process_groups_dict[comm_spec.logical_process_axis]
-    for rank_list, _ in process_groups_list:
-        if dist.get_rank() in rank_list:
-            dim = comm_spec.shard_dim
-            length = tensor.shape[comm_spec.shard_dim] // len(rank_list)
-            start = length * rank_list.index(dist.get_rank())
-            output = torch.narrow(tensor, dim, start, length).contiguous()
-            return output
+    process_group = comm_spec.process_group_dict[comm_spec.logical_process_axis]
+    dim = comm_spec.shard_dim
+    length = tensor.shape[comm_spec.shard_dim] // dist.get_world_size(process_group)
+    start = length * dist.get_rank(process_group)
+    output = torch.narrow(tensor, dim, start, length).contiguous()
+    return output
 
 
 def _all_to_all(tensor: torch.Tensor, comm_spec: CommSpec):
     '''
     Implement all to all operation on device mesh based on information provided by comm_spec.
     '''
-    process_groups_list = comm_spec.process_groups_dict[comm_spec.logical_process_axis]
-    for rank_list, process_group in process_groups_list:
-        if dist.get_rank() in rank_list:
-            new_shape = list(tensor.shape)
-            new_shape[comm_spec.shard_dim] = new_shape[comm_spec.shard_dim] // len(rank_list)
-            new_shape = torch.Size(new_shape)
-            output_tensor_list = [
-                torch.zeros(new_shape, dtype=tensor.dtype, device=tensor.device) for _ in range(len(rank_list))
-            ]
-            dim = comm_spec.shard_dim
-            length = tensor.shape[comm_spec.shard_dim] // len(rank_list)
-            input_tensor_list = [
-                torch.narrow(tensor, dim, length * i, length).contiguous() for i in range(len(rank_list))
-            ]
-            group = process_group
-            dist.all_to_all(output_tensor_list, input_tensor_list, group)
-            output = torch.cat(tuple(output_tensor_list), comm_spec.gather_dim).contiguous()
-            return output
+    process_group = comm_spec.process_group_dict[comm_spec.logical_process_axis]
+    world_size = dist.get_world_size(process_group)
+    new_shape = list(tensor.shape)
+    new_shape[comm_spec.shard_dim] = new_shape[comm_spec.shard_dim] // world_size
+    new_shape = torch.Size(new_shape)
+    output_tensor_list = [torch.zeros(new_shape, dtype=tensor.dtype, device=tensor.device) for _ in range(world_size)]
+    dim = comm_spec.shard_dim
+    length = tensor.shape[comm_spec.shard_dim] // world_size
+    input_tensor_list = [torch.narrow(tensor, dim, length * i, length).contiguous() for i in range(world_size)]
+    group = process_group
+    dist.all_to_all(output_tensor_list, input_tensor_list, group)
+    output = torch.cat(tuple(output_tensor_list), comm_spec.gather_dim).contiguous()
+    return output
 
 
 def _all_reduce(tensor: torch.Tensor, comm_spec: CommSpec, async_op: bool = False):
     '''
     Implement all reduce operation on device mesh based on information provided by comm_spec.
     '''
-    process_groups_list = comm_spec.process_groups_dict[comm_spec.logical_process_axis]
-    for rank_list, process_group in process_groups_list:
-        if dist.get_rank() in rank_list:
-            if not tensor.is_contiguous():
-                tensor = tensor.contiguous()
-            dist.all_reduce(tensor, op=ReduceOp.SUM, group=process_group, async_op=async_op)
-            return tensor
+    process_group = comm_spec.process_group_dict[comm_spec.logical_process_axis]
+    if not tensor.is_contiguous():
+        tensor = tensor.contiguous()
+    dist.all_reduce(tensor, op=ReduceOp.SUM, group=process_group, async_op=async_op)
+    return tensor
 
 
 class _ReduceGrad(torch.autograd.Function):
     """
     A customized communication operation which forward is an identity operation,
     backward is all_reduce operation.
 
@@ -265,15 +253,15 @@
     def symbolic(graph, input_):
         return _all_to_all(input_)
 
     @staticmethod
     def forward(ctx, input_, comm_spec):
         output = _all_to_all(input_, comm_spec)
         comm_spec_for_backward = CommSpec(comm_pattern=comm_spec.comm_pattern,
-                                          process_groups_dict=comm_spec.process_groups_dict,
+                                          process_group_dict=comm_spec.process_group_dict,
                                           gather_dim=comm_spec.shard_dim,
                                           shard_dim=comm_spec.gather_dim,
                                           logical_process_axis=comm_spec.logical_process_axis)
         ctx.comm_spec = comm_spec_for_backward
         return output
 
     @staticmethod
```

### Comparing `colossalai-nightly-2023.7.1/colossalai/tensor/d_tensor/layout.py` & `colossalai-nightly-2023.7.8/colossalai/tensor/d_tensor/layout.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,68 +1,65 @@
 import operator
-from dataclasses import dataclass
 from functools import reduce
 
 import torch
 
 from colossalai.device.device_mesh import DeviceMesh
 
-from .misc import DuplicatedShardingDimensionError, LayoutException, ShardingNotDivisibleError
+from .misc import DuplicatedShardingDimensionError, ShardingNotDivisibleError
 from .sharding_spec import ShardingSpec
 
 
 class Layout:
     """Layout of a tensor.
 
     Attributes:
         device_mesh: the device mesh to store the tensor distributed.
-        device_type: the type of the device mesh, e.g. 'cpu' or 'cuda'.
         sharding_spec: the sharding specification to describe how the tensor is sharded.
-        entire_shape: the entire shape of the global tensor.
+        global_shape: the entire shape of the global tensor.
     """
 
-    def __init__(self, device_mesh: DeviceMesh, device_type: torch.device, sharding_spec: ShardingSpec,
-                 entire_shape: torch.Size):
+    def __init__(self, device_mesh: DeviceMesh, sharding_spec: ShardingSpec, global_shape: torch.Size):
         self.device_mesh = device_mesh
-        self.device_type = device_type
         self.sharding_spec = sharding_spec
-        self.entire_shape = entire_shape
+        self.global_shape = global_shape
         self._sanity_check()
 
     def __hash__(self) -> int:
         return hash(f'{self.sharding_spec}')
 
     def get_sharded_shape_per_device(self):
-        sharded_shape = list(self.entire_shape)
+        sharded_shape = list(self.global_shape)
         for dim, shard_list in self.sharding_spec.dim_partition_dict.items():
-            mesh_list = [self.device_mesh.mesh_shape[mesh_dim] for mesh_dim in shard_list]
+            mesh_list = [self.device_mesh.shape[mesh_dim] for mesh_dim in shard_list]
             shard_partitions = reduce(operator.mul, mesh_list, 1)
             assert sharded_shape[
                 dim] % shard_partitions == 0, f'Cannot shard dimension {dim} into {shard_partitions} partitions.'
             sharded_shape[dim] //= shard_partitions
         return torch.Size(sharded_shape)
 
     def _sanity_check(self):
         sharding_spec = self.sharding_spec
 
         # make sure all axes in logical device mesh only be used once
-        dim_check_list = list(range(self.device_mesh.logical_mesh_id.dim()))
-        for dim, shard_list in sharding_spec.dim_partition_dict.items():
-            for element in shard_list:
-                if element in dim_check_list:
-                    dim_check_list.remove(element)
-                else:
-                    raise DuplicatedShardingDimensionError(
-                        f"find an invalid sharding axis {element} in dim_partition_dict in tensor dimension {dim}.")
+        if self.device_mesh.logical_mesh_id is not None:
+            dim_check_list = list(range(self.device_mesh.logical_mesh_id.dim()))
+            for dim, shard_list in sharding_spec.dim_partition_dict.items():
+                for element in shard_list:
+                    if element in dim_check_list:
+                        dim_check_list.remove(element)
+                    else:
+                        raise DuplicatedShardingDimensionError(
+                            f"find an invalid sharding axis {element} in dim_partition_dict in tensor dimension {dim}.")
 
         # make sure that the sharding for a dimension is divisible by the number of devices
         for dim, shard_list in sharding_spec.dim_partition_dict.items():
-            tensor_dim_size = self.entire_shape[dim]
+            tensor_dim_size = self.global_shape[dim]
             num_devices = 1
 
             for element in shard_list:
-                num_devices *= self.device_mesh.mesh_shape[element]
+                num_devices *= self.device_mesh.shape[element]
 
             if tensor_dim_size % num_devices != 0:
                 raise ShardingNotDivisibleError(
                     f'The size of dimension at index {dim} is {tensor_dim_size}, it cannot be sharded over {num_devices} devices.'
                 )
```

### Comparing `colossalai-nightly-2023.7.1/colossalai/tensor/d_tensor/layout_converter.py` & `colossalai-nightly-2023.7.8/colossalai/tensor/d_tensor/layout_converter.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 import math
 from copy import deepcopy
 from dataclasses import dataclass
 from typing import Dict, List, Tuple
 
-import numpy as np
 import torch
 
-from colossalai.auto_parallel.tensor_shard.sharding_strategy import MemoryCost, TrainCycleItem
 from colossalai.context.singleton_meta import SingletonMeta
 from colossalai.tensor.d_tensor.comm_spec import *
 from colossalai.tensor.d_tensor.layout import Layout
 from colossalai.tensor.d_tensor.misc import LayoutException
 from colossalai.tensor.utils import all_gather_simulator, all_to_all_simulator, shard_simulator
 
 from .sharding_spec import ShardingSpec
@@ -24,35 +22,26 @@
     """
     LayoutConverterOptions is a dataclass which specifies the preferences for layout converting.
     """
     # TODO: layout converter option is not implemented yet
     pass
 
 
-def to_global(distributed_tensor: torch.Tensor, layout: Layout) -> torch.Tensor:
-    layout_converter = LayoutConverter()
-    global_sharding_spec = ShardingSpec(distributed_tensor.dim(), {})
-    global_layout = Layout(device_mesh=layout.device_mesh,
-                           device_type=layout.device_type,
-                           sharding_spec=global_sharding_spec,
-                           entire_shape=layout.entire_shape)
-    with torch.no_grad():
-        global_tensor = layout_converter.apply(distributed_tensor, layout, global_layout)
-    return global_tensor
-
-
 def set_layout_converting_options(options: LayoutConverterOptions):
     """
     Configure the shape consistency manager via function call.
     """
     manager = LayoutConverter()
     manager.options = options
 
 
 class LayoutConverter(metaclass=SingletonMeta):
+    """
+    LayoutConverter is a singleton class which converts the layout of a distributed tensor.
+    """
 
     def __init__(self):
         self._options = None
         self._forward_only = False
         self.cached_solution = {}
 
     @property
@@ -87,36 +76,40 @@
         Example:
             layout_converter = LayoutConverter()
             physical_mesh_id = torch.arange(0, 4)
             mesh_shape = (2, 2)
             # [[0, 1,
             #  [2, 3]]
             device_mesh = DeviceMesh(physical_mesh_id, mesh_shape, init_process_group=True)
-            entire_shape = (4, 4, 4)
+            global_shape = (4, 4, 4)
             dim_partition_dict = {0: [0], 1: [1]}
 
             # [S0,S1,R]
             sharding_spec = ShardingSpec(dim_size=3, dim_partition_dict=dim_partition_dict)
             layout = Layout(device_mesh=device_mesh,
-                            device_type=torch.device('cuda'),
                             sharding_spec=sharding_spec,
-                            entire_shape=entire_shape)
+                            global_shape=global_shape)
 
             rst_dict = layout_converter.all_gather_transform_layouts(layout)
             for layout, comm_spec in rst_dict.items():
                 print(f'{layout.sharding_spec.sharding_sequence}: {comm_spec}')
 
         Output:
             [R, S1, R]: CommSpec:(comm_pattern:GATHER_FWD_SPLIT_BWD, gather_dim:0, shard_dim:0, logical_process_axis:0)
             [S0, R, R]: CommSpec:(comm_pattern:GATHER_FWD_SPLIT_BWD, gather_dim:1, shard_dim:1, logical_process_axis:1)
         '''
         valid_spec_dict = {}
         comm_pattern = CollectiveCommPattern.GATHER_FWD_SPLIT_BWD
         source_spec = source_layout.sharding_spec
-        process_groups_dict = source_layout.device_mesh.process_groups_dict
+
+        # the key of the dict is the axis
+        # the value is the process group
+        current_rank = source_layout.device_mesh._global_rank_of_current_process
+        process_group_dict = source_layout.device_mesh._process_group_dict[current_rank]
+
         for target_pair in source_spec.dim_partition_dict.items():
             shard_list = all_gather_simulator(target_pair)
             index = target_pair[0]
             new_dim_partition_dict = deepcopy(source_spec.dim_partition_dict)
 
             # We won't add empty list into dim_partition_dict
             # The key will be popped if the related shard_list is empty
@@ -126,27 +119,26 @@
                 new_dim_partition_dict.pop(index)
 
             # generate the CommSpec to record the action of source_sharding_spec->new_sharding_spec
             gather_dim = index
             logical_process_axis = target_pair[1][-1]
             comm_spec = CommSpec(
                 comm_pattern,
-                process_groups_dict=process_groups_dict,
+                process_group_dict=process_group_dict,
                 gather_dim=gather_dim,
             # shard_dim will be used during backward
                 shard_dim=gather_dim,
                 logical_process_axis=logical_process_axis)
 
             # generate new sharding spec
             try:
                 new_sharding_spec = ShardingSpec(source_spec.dims, dim_partition_dict=new_dim_partition_dict)
                 new_layout = Layout(device_mesh=source_layout.device_mesh,
                                     sharding_spec=new_sharding_spec,
-                                    device_type=source_layout.device_type,
-                                    entire_shape=source_layout.entire_shape)
+                                    global_shape=source_layout.global_shape)
 
                 valid_spec_dict[new_layout] = comm_spec
             except LayoutException:
                 pass
         return valid_spec_dict
 
     def all_to_all_transform_layout(self, source_layout: Layout) -> Dict[Layout, CommSpec]:
@@ -163,36 +155,40 @@
         Example:
             layout_converter = LayoutConverter()
             physical_mesh_id = torch.arange(0, 4)
             mesh_shape = (2, 2)
             # [[0, 1,
             #  [2, 3]]
             device_mesh = DeviceMesh(physical_mesh_id, mesh_shape, init_process_group=True)
-            entire_shape = (4, 4, 4)
+            global_shape = (4, 4, 4)
             dim_partition_dict = {0: [0], 1: [1]}
 
             # [S0,S1,R]
             sharding_spec = ShardingSpec(dim_size=3, dim_partition_dict=dim_partition_dict)
             layout = Layout(device_mesh=device_mesh,
-                                    device_type=torch.device('cuda'),
                                     sharding_spec=sharding_spec,
-                                    entire_shape=entire_shape)
+                                    global_shape=global_shape)
             rst_dict = layout_converter.all_to_all_transform_layout(layout)
 
             for layout, comm_spec in rst_dict.items():
                 print(f'{layout.sharding_spec.sharding_sequence}: {comm_spec}')
 
         Output:
             [S01, R, R]: CommSpec:(comm_pattern:ALL2ALL_FWD_ALL2ALL_BWD, gather_dim:1, shard_dim:0, logical_process_axis: 1)
             [R, S1, S0]: CommSpec:(comm_pattern:ALL2ALL_FWD_ALL2ALL_BWD, gather_dim:0, shard_dim:2, logical_process_axis: 0)
             [S0, R, S1]: CommSpec:(comm_pattern:ALL2ALL_FWD_ALL2ALL_BWD, gather_dim:1, shard_dim:2, logical_process_axis: 1)
         '''
         valid_spec_dict = {}
         comm_pattern = CollectiveCommPattern.ALL2ALL_FWD_ALL2ALL_BWD
-        process_groups_dict = source_layout.device_mesh.process_groups_dict
+
+        # the key of the dict is the axis
+        # the value is the process group
+        current_rank = source_layout.device_mesh._global_rank_of_current_process
+        process_group_dict = source_layout.device_mesh._process_group_dict[current_rank]
+
         source_spec = source_layout.sharding_spec
         tensor_dims = source_spec.dims
         for f_index in range(tensor_dims - 1):
             for b_index in range(f_index + 1, tensor_dims):
                 # skip (R, R) cases
                 if f_index not in source_spec.dim_partition_dict and b_index not in source_spec.dim_partition_dict:
                     continue
@@ -225,15 +221,15 @@
                     shard_dim = b_index
                     logical_process_axis = f_target_pair[1][-1]
                 else:
                     gather_dim = b_index
                     shard_dim = f_index
                     logical_process_axis = b_target_pair[1][-1]
                 comm_spec = CommSpec(comm_pattern,
-                                     process_groups_dict,
+                                     process_group_dict=process_group_dict,
                                      gather_dim=gather_dim,
                                      shard_dim=shard_dim,
                                      logical_process_axis=logical_process_axis)
 
                 new_dim_partition_dict = deepcopy(source_spec.dim_partition_dict)
 
                 # We won't add empty list into dim_partition_dict
@@ -248,16 +244,15 @@
                     new_dim_partition_dict.pop(b_index)
 
                 # generate new sharding spec
                 try:
                     new_sharding_spec = ShardingSpec(source_spec.dims, dim_partition_dict=new_dim_partition_dict)
                     new_layout = Layout(device_mesh=source_layout.device_mesh,
                                         sharding_spec=new_sharding_spec,
-                                        device_type=source_layout.device_type,
-                                        entire_shape=source_layout.entire_shape)
+                                        global_shape=source_layout.global_shape)
                     valid_spec_dict[new_layout] = comm_spec
                 except LayoutException:
                     pass
 
         return valid_spec_dict
 
     def shard_transform_layout(self, source_layout: Layout) -> Dict[Layout, CommSpec]:
@@ -274,41 +269,44 @@
         Example:
             layout_converter = LayoutConverter()
             physical_mesh_id = torch.arange(0, 4)
             mesh_shape = (2, 2)
             # [[0, 1,
             #  [2, 3]]
             device_mesh = DeviceMesh(physical_mesh_id, mesh_shape, init_process_group=True)
-            entire_shape = (4, 4, 4)
+            global_shape = (4, 4, 4)
 
             dim_partition_dict = {0: [0]}
 
             # [S0,R,R]
             sharding_spec = ShardingSpec(dim_size=3, dim_partition_dict=dim_partition_dict)
             layout = Layout(device_mesh=device_mesh,
-                          device_type=torch.device('cuda'),
                           sharding_spec=sharding_spec,
-                          entire_shape=entire_shape)
+                          global_shape=global_shape)
             rst_dict = layout_converter.shard_transform_layout(layout)
 
             for layout, comm_spec in rst_dict.items():
                 print(f'{layout.sharding_spec.sharding_sequence}: {comm_spec}')
 
         Output:
             [S01, R, R]: CommSpec:(comm_pattern:SPLIT_FWD_GATHER_BWD, gather_dim:0, shard_dim:0, logical_process_axis:1)
             [S0, S1, R]: CommSpec:(comm_pattern:SPLIT_FWD_GATHER_BWD, gather_dim:1, shard_dim:1, logical_process_axis:1)
             [S0, R, S1]: CommSpec:(comm_pattern:SPLIT_FWD_GATHER_BWD, gather_dim:2, shard_dim:2, logical_process_axis:1)
         '''
         valid_spec_dict = {}
         comm_pattern = CollectiveCommPattern.SPLIT_FWD_GATHER_BWD
         source_spec = source_layout.sharding_spec
-        process_groups_dict = source_layout.device_mesh.process_groups_dict
+
+        # the key of the dict is the axis
+        # the value is the process group
+        current_rank = source_layout.device_mesh._global_rank_of_current_process
+        process_group_dict = source_layout.device_mesh._process_group_dict[current_rank]
 
         # legal sharding dims means the mesh_id is still available to use.
-        legal_sharding_dims = [i for i in range(len(source_layout.device_mesh.mesh_shape))]
+        legal_sharding_dims = [i for i in range(len(source_layout.device_mesh.shape))]
         for dim, shard_list in source_spec.dim_partition_dict.items():
             for element in shard_list:
                 legal_sharding_dims.remove(element)
 
         if len(legal_sharding_dims) == 0:
             return valid_spec_dict
 
@@ -325,27 +323,26 @@
                 new_dim_partition_dict = deepcopy(source_spec.dim_partition_dict)
                 new_dim_partition_dict[index] = shard_list
 
                 # generate the CommSpec to record the action of source_sharding_spec->new_sharding_spec
                 shard_dim = index
                 logical_process_axis = shard_list[-1]
                 comm_spec = CommSpec(comm_pattern,
-                                     process_groups_dict,
+                                     process_group_dict=process_group_dict,
                                      gather_dim=shard_dim,
                                      shard_dim=shard_dim,
                                      logical_process_axis=logical_process_axis)
 
                 # generate new sharding spec
                 try:
                     new_sharding_spec = ShardingSpec(dim_size=source_spec.dims,
                                                      dim_partition_dict=new_dim_partition_dict)
                     new_layout = Layout(device_mesh=source_layout.device_mesh,
                                         sharding_spec=new_sharding_spec,
-                                        device_type=source_layout.device_type,
-                                        entire_shape=source_layout.entire_shape)
+                                        global_shape=source_layout.global_shape)
                     valid_spec_dict[new_layout] = comm_spec
                 except LayoutException:
                     pass
         return valid_spec_dict
 
     def get_all_one_step_transform_spec(self, source_layout: Layout) -> Dict[Layout, CommSpec]:
         '''
@@ -395,32 +392,30 @@
 
         Example:
             physical_mesh_id = torch.arange(0, 4)
             mesh_shape = (2, 2)
             # [[0, 1,
             #  [2, 3]]
             device_mesh = DeviceMesh(physical_mesh_id, mesh_shape, init_process_group=True)
-            entire_shape = (4, 4, 4)
+            global_shape = (4, 4, 4)
 
             dim_partition_source = {1: [0, 1]}
             dim_partition_target = {0: [0, 1]}
 
             # [R,S01,R]
             sharding_spec_source = ShardingSpec(dim_size=3, dim_partition_dict=dim_partition_source)
             source_layout = Layout(device_mesh=device_mesh,
-                                device_type=torch.device('cuda'),
                                 sharding_spec=sharding_spec_source,
-                                entire_shape=entire_shape)
+                                global_shape=global_shape)
 
             # [S01,R,R]
             sharding_spec_target = ShardingSpec(dim_size=3, dim_partition_dict=dim_partition_target)
             target_layout = Layout(device_mesh=device_mesh,
-                                device_type=torch.device('cuda'),
                                 sharding_spec=sharding_spec_target,
-                                entire_shape=entire_shape)
+                                global_shape=global_shape)
 
             transform_path, comm_action_sequence = layout_converter.layout_converting(source_layout, target_layout)
             transform_path_str = '->'.join([str(layout.sharding_spec.sharding_sequence) for layout in transform_path])
             print(transform_path_str)
 
         output:
             [R, S01, R]->[R, S0, R]->[S0, R, R]->[S01, R, R]
@@ -501,29 +496,27 @@
             dim_partition_source = {0: [0]}
             dim_partition_target = {1: [0]}
             physical_mesh_id = torch.arange(0, 4)
             mesh_shape = (2, 2)
             # [[0, 1,
             #  [2, 3]]
             device_mesh = DeviceMesh(physical_mesh_id, mesh_shape, init_process_group=True)
-            entire_shape = (4, 4, 4)
+            global_shape = (4, 4, 4)
 
             # [S0,R,R]
             sharding_spec_source = ShardingSpec(dim_size=3, dim_partition_dict=dim_partition_source)
             source_layout = Layout(device_mesh=device_mesh,
-                                device_type=torch.device('cuda'),
                                 sharding_spec=sharding_spec_source,
-                                entire_shape=entire_shape)
+                                global_shape=global_shape)
 
             # [R,S0,R]
             sharding_spec_target = ShardingSpec(dim_size=3, dim_partition_dict=dim_partition_target)
             target_layout = Layout(device_mesh=device_mesh,
-                                device_type=torch.device('cuda'),
                                 sharding_spec=sharding_spec_target,
-                                entire_shape=entire_shape)
+                                global_shape=global_shape)
 
             if rank in (0, 1):
                 sharded_tensor_0 = torch.zeros(2, 1)
                 sharded_tensor_1 = torch.ones(2, 1)
                 # tensor([[0., 1.],
                 #         [0., 1.]])
                 tensor_to_comm = torch.cat((sharded_tensor_0, sharded_tensor_1), 1).cuda()
@@ -549,8 +542,9 @@
                     [1.],
                     [3.],
                     [3.]])
         '''
         _, comm_action_sequence = self.layout_converting(source_layout, target_layout)
         for comm_spec in comm_action_sequence:
             tensor = comm_spec.covert_spec_to_action(tensor)
+        tensor.dist_layout = target_layout
         return tensor
```

### Comparing `colossalai-nightly-2023.7.1/colossalai/tensor/d_tensor/sharding_spec.py` & `colossalai-nightly-2023.7.8/colossalai/tensor/d_tensor/sharding_spec.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/tensor/d_tensor/utils.py` & `colossalai-nightly-2023.7.8/colossalai/tensor/d_tensor/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     logical_process_axis = comm_spec.logical_process_axis
     cost_dict = {}
 
     if comm_pattern == CollectiveCommPattern.GATHER_FWD_SPLIT_BWD:
         # the comm size for all gather is the size of the gathered tensor
         gather_dim = comm_spec.gather_dim
         all_gather_axis = layout.sharding_spec.dim_partition_dict[gather_dim][-1]
-        all_gather_size = device_mesh.mesh_shape[all_gather_axis]
+        all_gather_size = device_mesh.shape[all_gather_axis]
         comm_size_for_all_gather = comm_size * all_gather_size
         forward_communication_cost = device_mesh.all_gather_cost(comm_size_for_all_gather, logical_process_axis)
         # give a tiny cost to shard
         backward_communication_cost = 100
 
     if comm_pattern == CollectiveCommPattern.ALL2ALL_FWD_ALL2ALL_BWD:
         forward_communication_cost = device_mesh.all_to_all_cost(comm_size, logical_process_axis)
```

### Comparing `colossalai-nightly-2023.7.1/colossalai/tensor/dist_spec_mgr.py` & `colossalai-nightly-2023.7.8/colossalai/tensor/dist_spec_mgr.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/tensor/distspec.py` & `colossalai-nightly-2023.7.8/colossalai/tensor/distspec.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/tensor/op_wrapper.py` & `colossalai-nightly-2023.7.8/colossalai/tensor/op_wrapper.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/tensor/param_op_hook.py` & `colossalai-nightly-2023.7.8/colossalai/tensor/param_op_hook.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/tensor/process_group.py` & `colossalai-nightly-2023.7.8/colossalai/tensor/process_group.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/tensor/shape_consistency.py` & `colossalai-nightly-2023.7.8/colossalai/tensor/shape_consistency.py`

 * *Files 0% similar despite different names*

```diff
@@ -281,15 +281,15 @@
             shard_sequence: S0,R,S1
             device_mesh_shape: (4, 4): 0}
         '''
         valid_spec_dict = {}
         comm_pattern = CollectiveCommPattern.SPLIT_FWD_GATHER_BWD
 
         # legal sharding dims means the mesh_id is still available to use.
-        legal_sharding_dims = [i for i in range(len(source_spec.device_mesh.mesh_shape))]
+        legal_sharding_dims = [i for i in range(len(source_spec.device_mesh.shape))]
         for dim, shard_list in source_spec.dim_partition_dict.items():
             for element in shard_list:
                 legal_sharding_dims.remove(element)
         if len(legal_sharding_dims) == 0:
             return valid_spec_dict
 
         tensor_dims = len(source_spec.entire_shape)
@@ -431,15 +431,15 @@
                 comm_spec (CommSpec): input CommSpec
                 discard_input (bool): whether to discard the input tensor
                 alloc_numel (int): current allocated numel
                 peak_numel (int): current peak numel
             """
             input_shape = compute_shape(comm_spec.sharding_spec)
             input_numel = np.prod(input_shape)
-            output_numel = input_numel * comm_spec.device_mesh.mesh_shape[comm_spec.logical_process_axis]
+            output_numel = input_numel * comm_spec.device_mesh.shape[comm_spec.logical_process_axis]
             peak_numel = max(peak_numel, alloc_numel + output_numel * 2)
             alloc_numel += output_numel
             if discard_input:
                 alloc_numel -= input_numel
 
             return alloc_numel, peak_numel
 
@@ -457,15 +457,15 @@
             """
             shard_dim = comm_spec.shard_dim
             if shard_dim != 0:
                 # if we don't shard the tensor on the first dimension, the split action will
                 # generate a new tensor
                 input_shape = compute_shape(comm_spec.sharding_spec)
                 input_numel = np.prod(input_shape)
-                output_numel = input_numel // comm_spec.device_mesh.mesh_shape[comm_spec.logical_process_axis]
+                output_numel = input_numel // comm_spec.device_mesh.shape[comm_spec.logical_process_axis]
                 alloc_numel += output_numel
                 peak_numel = max(peak_numel, alloc_numel)
                 if discard_input:
                     alloc_numel -= input_numel
             else:
                 # if we shard the tensor on the first dimension, the split action will not generate
                 # a new tensor, and as it will preserve a reference to the input tensor, we could
```

### Comparing `colossalai-nightly-2023.7.1/colossalai/tensor/sharding_spec.py` & `colossalai-nightly-2023.7.8/colossalai/tensor/sharding_spec.py`

 * *Files 0% similar despite different names*

```diff
@@ -191,15 +191,15 @@
             assert self.sharding_sequence is not None, f'sharding_sequence should not be None, if dim_partition_dict is NoneType object.'
             self.convert_shard_sequence_to_dict()
         self._sanity_check()
 
     def __repr__(self):
         res_list = ["DistSpec:"]
         res_list.append(f"\n\tshard_sequence: " + ",".join(str(dimspec) for dimspec in self.sharding_sequence))
-        res_list.append(f"\n\tdevice_mesh_shape: {self.device_mesh.mesh_shape}")
+        res_list.append(f"\n\tdevice_mesh_shape: {self.device_mesh.shape}")
         return ' '.join(res_list)
 
     def _sanity_check(self):
         # make sure all axes in logical device mesh only be used once
         dim_check_list = list(range(self.device_mesh.logical_mesh_id.dim()))
         for dim, shard_list in self.dim_partition_dict.items():
             for element in shard_list:
@@ -218,15 +218,15 @@
 
         # make sure that the sharding for a dimension is divisible by the number of devices
         for dim, shard_list in self.dim_partition_dict.items():
             tensor_dim_size = self.entire_shape[dim]
             num_devices = 1
 
             for element in shard_list:
-                num_devices *= self.device_mesh.mesh_shape[element]
+                num_devices *= self.device_mesh.shape[element]
 
             if tensor_dim_size % num_devices != 0:
                 raise ShardingNotDivisibleError(
                     f'The size of dimension at index {dim} is {tensor_dim_size}, it cannot be sharded over {num_devices} devices.'
                 )
 
     def convert_dict_to_shard_sequence(self):
@@ -284,13 +284,13 @@
             difference += orig_dim_spec.difference(other_dim_spec)
         return difference
 
     def get_sharded_shape_per_device(self):
 
         sharded_shape = list(self.entire_shape)
         for dim, shard_list in self.dim_partition_dict.items():
-            mesh_list = [self.device_mesh.mesh_shape[mesh_dim] for mesh_dim in shard_list]
+            mesh_list = [self.device_mesh.shape[mesh_dim] for mesh_dim in shard_list]
             shard_partitions = reduce(operator.mul, mesh_list, 1)
             assert sharded_shape[
                 dim] % shard_partitions == 0, f'Cannot shard dimension {dim} into {shard_partitions} partitions.'
             sharded_shape[dim] //= shard_partitions
         return torch.Size(sharded_shape)
```

### Comparing `colossalai-nightly-2023.7.1/colossalai/tensor/tensor_spec.py` & `colossalai-nightly-2023.7.8/colossalai/tensor/tensor_spec.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/tensor/utils.py` & `colossalai-nightly-2023.7.8/colossalai/tensor/utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/testing/__init__.py` & `colossalai-nightly-2023.7.8/colossalai/testing/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from .comparison import (
     assert_close,
     assert_close_loose,
     assert_equal,
     assert_equal_in_group,
+    assert_hf_output_close,
     assert_not_equal,
     check_state_dict_equal,
 )
 from .pytest_wrapper import run_on_environment_flag
 from .utils import (
     clear_cache_before_run,
     free_port,
@@ -16,9 +17,9 @@
     skip_if_not_enough_gpus,
     spawn,
 )
 
 __all__ = [
     'assert_equal', 'assert_not_equal', 'assert_close', 'assert_close_loose', 'assert_equal_in_group', 'parameterize',
     'rerun_on_exception', 'rerun_if_address_is_in_use', 'skip_if_not_enough_gpus', 'free_port', 'spawn',
-    'clear_cache_before_run', 'run_on_environment_flag', 'check_state_dict_equal'
+    'clear_cache_before_run', 'run_on_environment_flag', 'check_state_dict_equal', 'assert_hf_output_close'
 ]
```

### Comparing `colossalai-nightly-2023.7.1/colossalai/testing/pytest_wrapper.py` & `colossalai-nightly-2023.7.8/colossalai/testing/pytest_wrapper.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/testing/random.py` & `colossalai-nightly-2023.7.8/colossalai/testing/random.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/testing/utils.py` & `colossalai-nightly-2023.7.8/colossalai/testing/utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/trainer/_trainer.py` & `colossalai-nightly-2023.7.8/colossalai/trainer/_trainer.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/trainer/hooks/__init__.py` & `colossalai-nightly-2023.7.8/colossalai/trainer/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/trainer/hooks/_base_hook.py` & `colossalai-nightly-2023.7.8/colossalai/trainer/hooks/_base_hook.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/trainer/hooks/_checkpoint_hook.py` & `colossalai-nightly-2023.7.8/colossalai/trainer/hooks/_checkpoint_hook.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/trainer/hooks/_log_hook.py` & `colossalai-nightly-2023.7.8/colossalai/trainer/hooks/_log_hook.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/trainer/hooks/_lr_scheduler_hook.py` & `colossalai-nightly-2023.7.8/colossalai/trainer/hooks/_lr_scheduler_hook.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/trainer/hooks/_metric_hook.py` & `colossalai-nightly-2023.7.8/colossalai/trainer/hooks/_metric_hook.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/utils/__init__.py` & `colossalai-nightly-2023.7.8/colossalai/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/utils/activation_checkpoint.py` & `colossalai-nightly-2023.7.8/colossalai/utils/activation_checkpoint.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/utils/checkpoint/module_checkpoint.py` & `colossalai-nightly-2023.7.8/colossalai/utils/checkpoint/module_checkpoint.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/utils/checkpoint/utils.py` & `colossalai-nightly-2023.7.8/colossalai/utils/checkpoint/utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/utils/checkpoint_io/backend.py` & `colossalai-nightly-2023.7.8/colossalai/utils/checkpoint_io/backend.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/utils/checkpoint_io/convertor.py` & `colossalai-nightly-2023.7.8/colossalai/utils/checkpoint_io/convertor.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/utils/checkpoint_io/distributed.py` & `colossalai-nightly-2023.7.8/colossalai/utils/checkpoint_io/distributed.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/utils/checkpoint_io/io.py` & `colossalai-nightly-2023.7.8/colossalai/utils/checkpoint_io/io.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/utils/checkpoint_io/meta.py` & `colossalai-nightly-2023.7.8/colossalai/utils/checkpoint_io/meta.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/utils/checkpoint_io/reader.py` & `colossalai-nightly-2023.7.8/colossalai/utils/checkpoint_io/reader.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/utils/checkpoint_io/utils.py` & `colossalai-nightly-2023.7.8/colossalai/utils/checkpoint_io/utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/utils/checkpoint_io/writer.py` & `colossalai-nightly-2023.7.8/colossalai/utils/checkpoint_io/writer.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/utils/checkpointing.py` & `colossalai-nightly-2023.7.8/colossalai/utils/checkpointing.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/utils/common.py` & `colossalai-nightly-2023.7.8/colossalai/utils/common.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/utils/cuda.py` & `colossalai-nightly-2023.7.8/colossalai/utils/cuda.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/utils/data_sampler/data_parallel_sampler.py` & `colossalai-nightly-2023.7.8/colossalai/utils/data_sampler/data_parallel_sampler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/utils/memory.py` & `colossalai-nightly-2023.7.8/colossalai/utils/memory.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/utils/model/utils.py` & `colossalai-nightly-2023.7.8/colossalai/utils/model/utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/utils/moe.py` & `colossalai-nightly-2023.7.8/colossalai/utils/moe.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/utils/multi_tensor_apply/multi_tensor_apply.py` & `colossalai-nightly-2023.7.8/colossalai/utils/multi_tensor_apply/multi_tensor_apply.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/utils/profiler/legacy/comm_profiler.py` & `colossalai-nightly-2023.7.8/colossalai/utils/profiler/legacy/comm_profiler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/utils/profiler/legacy/pcie_profiler.py` & `colossalai-nightly-2023.7.8/colossalai/utils/profiler/legacy/pcie_profiler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/utils/profiler/legacy/prof_utils.py` & `colossalai-nightly-2023.7.8/colossalai/utils/profiler/legacy/prof_utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/utils/profiler/profiler.py` & `colossalai-nightly-2023.7.8/colossalai/utils/profiler/profiler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/utils/profiler/stateful_tensor_mem_extention.py` & `colossalai-nightly-2023.7.8/colossalai/utils/profiler/stateful_tensor_mem_extention.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/utils/rank_recorder/rank_recorder.py` & `colossalai-nightly-2023.7.8/colossalai/utils/rank_recorder/rank_recorder.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/utils/tensor_detector/tensor_detector.py` & `colossalai-nightly-2023.7.8/colossalai/utils/tensor_detector/tensor_detector.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/utils/timer.py` & `colossalai-nightly-2023.7.8/colossalai/utils/timer.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/zero/__init__.py` & `colossalai-nightly-2023.7.8/colossalai/zero/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/zero/gemini/__init__.py` & `colossalai-nightly-2023.7.8/colossalai/zero/gemini/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/zero/gemini/chunk/chunk.py` & `colossalai-nightly-2023.7.8/colossalai/zero/gemini/chunk/chunk.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/zero/gemini/chunk/manager.py` & `colossalai-nightly-2023.7.8/colossalai/zero/gemini/chunk/manager.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/zero/gemini/chunk/search_utils.py` & `colossalai-nightly-2023.7.8/colossalai/zero/gemini/chunk/search_utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/zero/gemini/chunk/utils.py` & `colossalai-nightly-2023.7.8/colossalai/zero/gemini/chunk/utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/zero/gemini/colo_init_context.py` & `colossalai-nightly-2023.7.8/colossalai/zero/gemini/colo_init_context.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/zero/gemini/gemini_ddp.py` & `colossalai-nightly-2023.7.8/colossalai/zero/gemini/gemini_ddp.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/zero/gemini/gemini_hook.py` & `colossalai-nightly-2023.7.8/colossalai/zero/gemini/gemini_hook.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/zero/gemini/gemini_mgr.py` & `colossalai-nightly-2023.7.8/colossalai/zero/gemini/gemini_mgr.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/zero/gemini/memory_tracer/__init__.py` & `colossalai-nightly-2023.7.8/colossalai/zero/gemini/memory_tracer/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/zero/gemini/memory_tracer/chunk_memstats_collector.py` & `colossalai-nightly-2023.7.8/colossalai/zero/gemini/memory_tracer/chunk_memstats_collector.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/zero/gemini/memory_tracer/memory_monitor.py` & `colossalai-nightly-2023.7.8/colossalai/zero/gemini/memory_tracer/memory_monitor.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/zero/gemini/memory_tracer/memory_stats.py` & `colossalai-nightly-2023.7.8/colossalai/zero/gemini/memory_tracer/memory_stats.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/zero/gemini/memory_tracer/memstats_collector.py` & `colossalai-nightly-2023.7.8/colossalai/zero/gemini/memory_tracer/memstats_collector.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/zero/gemini/memory_tracer/param_runtime_order.py` & `colossalai-nightly-2023.7.8/colossalai/zero/gemini/memory_tracer/param_runtime_order.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/zero/gemini/memory_tracer/runtime_mem_tracer.py` & `colossalai-nightly-2023.7.8/colossalai/zero/gemini/memory_tracer/runtime_mem_tracer.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/zero/gemini/memory_tracer/static_memstats_collector.py` & `colossalai-nightly-2023.7.8/colossalai/zero/gemini/memory_tracer/static_memstats_collector.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/zero/gemini/memory_tracer/utils.py` & `colossalai-nightly-2023.7.8/colossalai/zero/gemini/memory_tracer/utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/zero/gemini/placement_policy.py` & `colossalai-nightly-2023.7.8/colossalai/zero/gemini/placement_policy.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/zero/gemini/utils.py` & `colossalai-nightly-2023.7.8/colossalai/zero/gemini/utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/zero/legacy/__init__.py` & `colossalai-nightly-2023.7.8/colossalai/zero/legacy/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/zero/legacy/gemini/gemini_context.py` & `colossalai-nightly-2023.7.8/colossalai/zero/legacy/gemini/gemini_context.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/zero/legacy/gemini/ophooks/_shard_grad_ophook.py` & `colossalai-nightly-2023.7.8/colossalai/zero/legacy/gemini/ophooks/_shard_grad_ophook.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/zero/legacy/gemini/ophooks/_shard_param_ophook.py` & `colossalai-nightly-2023.7.8/colossalai/zero/legacy/gemini/ophooks/_shard_param_ophook.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/zero/legacy/gemini/ophooks/runtime_mem_tracer_hook.py` & `colossalai-nightly-2023.7.8/colossalai/zero/legacy/gemini/ophooks/runtime_mem_tracer_hook.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/zero/legacy/gemini/ophooks/utils.py` & `colossalai-nightly-2023.7.8/colossalai/zero/legacy/gemini/ophooks/utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/zero/legacy/gemini/paramhooks/_param_hookmgr.py` & `colossalai-nightly-2023.7.8/colossalai/zero/legacy/gemini/paramhooks/_param_hookmgr.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/zero/legacy/gemini/stateful_tensor.py` & `colossalai-nightly-2023.7.8/colossalai/zero/legacy/gemini/stateful_tensor.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/zero/legacy/gemini/stateful_tensor_mgr.py` & `colossalai-nightly-2023.7.8/colossalai/zero/legacy/gemini/stateful_tensor_mgr.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/zero/legacy/gemini/tensor_placement_policy.py` & `colossalai-nightly-2023.7.8/colossalai/zero/legacy/gemini/tensor_placement_policy.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/zero/legacy/gemini/tensor_utils.py` & `colossalai-nightly-2023.7.8/colossalai/zero/legacy/gemini/tensor_utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/zero/legacy/init_ctx/init_context.py` & `colossalai-nightly-2023.7.8/colossalai/zero/legacy/init_ctx/init_context.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/zero/legacy/shard_utils/base_shard_strategy.py` & `colossalai-nightly-2023.7.8/colossalai/zero/legacy/shard_utils/base_shard_strategy.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/zero/legacy/shard_utils/bucket_tensor_shard_strategy.py` & `colossalai-nightly-2023.7.8/colossalai/zero/legacy/shard_utils/bucket_tensor_shard_strategy.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/zero/legacy/shard_utils/commons.py` & `colossalai-nightly-2023.7.8/colossalai/zero/legacy/shard_utils/commons.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/zero/legacy/shard_utils/tensor_shard_strategy.py` & `colossalai-nightly-2023.7.8/colossalai/zero/legacy/shard_utils/tensor_shard_strategy.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/zero/legacy/sharded_model/_utils.py` & `colossalai-nightly-2023.7.8/colossalai/zero/legacy/sharded_model/_utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/zero/legacy/sharded_model/reduce_scatter.py` & `colossalai-nightly-2023.7.8/colossalai/zero/legacy/sharded_model/reduce_scatter.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/zero/legacy/sharded_model/sharded_model_v2.py` & `colossalai-nightly-2023.7.8/colossalai/zero/legacy/sharded_model/sharded_model_v2.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/zero/legacy/sharded_model/utils.py` & `colossalai-nightly-2023.7.8/colossalai/zero/legacy/sharded_model/utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/zero/legacy/sharded_model/zero_hook.py` & `colossalai-nightly-2023.7.8/colossalai/zero/legacy/sharded_model/zero_hook.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/zero/legacy/sharded_optim/sharded_optim_v2.py` & `colossalai-nightly-2023.7.8/colossalai/zero/legacy/sharded_optim/sharded_optim_v2.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/zero/legacy/sharded_param/sharded_param.py` & `colossalai-nightly-2023.7.8/colossalai/zero/legacy/sharded_param/sharded_param.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/zero/legacy/sharded_param/sharded_tensor.py` & `colossalai-nightly-2023.7.8/colossalai/zero/legacy/sharded_param/sharded_tensor.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/zero/low_level/_utils.py` & `colossalai-nightly-2023.7.8/colossalai/zero/low_level/_utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/zero/low_level/bookkeeping/bucket_store.py` & `colossalai-nightly-2023.7.8/colossalai/zero/low_level/bookkeeping/bucket_store.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/zero/low_level/bookkeeping/gradient_store.py` & `colossalai-nightly-2023.7.8/colossalai/zero/low_level/bookkeeping/gradient_store.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/zero/low_level/bookkeeping/parameter_store.py` & `colossalai-nightly-2023.7.8/colossalai/zero/low_level/bookkeeping/parameter_store.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/zero/low_level/bookkeeping/tensor_bucket.py` & `colossalai-nightly-2023.7.8/colossalai/zero/low_level/bookkeeping/tensor_bucket.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/zero/low_level/low_level_optim.py` & `colossalai-nightly-2023.7.8/colossalai/zero/low_level/low_level_optim.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai/zero/wrapper.py` & `colossalai-nightly-2023.7.8/colossalai/zero/wrapper.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/colossalai_nightly.egg-info/PKG-INFO` & `colossalai-nightly-2023.7.8/colossalai_nightly.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: colossalai-nightly
-Version: 2023.7.1
+Version: 2023.7.8
 Summary: An integrated large-scale model training system with efficient parallelization techniques
 Home-page: https://www.colossalai.org
 License: Apache Software License 2.0
 Project-URL: Forum, https://github.com/hpcaitech/ColossalAI/discussions
 Project-URL: Bug Tracker, https://github.com/hpcaitech/ColossalAI/issues
 Project-URL: Examples, https://github.com/hpcaitech/ColossalAI-Examples
 Project-URL: Documentation, http://colossalai.readthedocs.io
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: colossalai-nightly Version: 2023.7.1 Summary: An
+Metadata-Version: 2.1 Name: colossalai-nightly Version: 2023.7.8 Summary: An
 integrated large-scale model training system with efficient parallelization
 techniques Home-page: https://www.colossalai.org License: Apache Software
 License 2.0 Project-URL: Forum, https://github.com/hpcaitech/ColossalAI/
 discussions Project-URL: Bug Tracker, https://github.com/hpcaitech/ColossalAI/
 issues Project-URL: Examples, https://github.com/hpcaitech/ColossalAI-Examples
 Project-URL: Documentation, http://colossalai.readthedocs.io Project-URL:
 Github, https://github.com/hpcaitech/ColossalAI Description: # Colossal-AI
```

### Comparing `colossalai-nightly-2023.7.1/colossalai_nightly.egg-info/SOURCES.txt` & `colossalai-nightly-2023.7.8/colossalai_nightly.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -501,14 +501,42 @@
 colossalai/pipeline/middleware/adaptor/fx.py
 colossalai/pipeline/rpc/__init__.py
 colossalai/pipeline/rpc/_pipeline_base.py
 colossalai/pipeline/rpc/_pipeline_schedule.py
 colossalai/pipeline/rpc/utils.py
 colossalai/registry/__init__.py
 colossalai/registry/registry.py
+colossalai/shardformer/__init__.py
+colossalai/shardformer/_utils.py
+colossalai/shardformer/layer/__init__.py
+colossalai/shardformer/layer/_operation.py
+colossalai/shardformer/layer/dropout.py
+colossalai/shardformer/layer/embedding.py
+colossalai/shardformer/layer/linear.py
+colossalai/shardformer/layer/loss.py
+colossalai/shardformer/layer/normalization.py
+colossalai/shardformer/layer/parallel_module.py
+colossalai/shardformer/layer/qkv_fused_linear.py
+colossalai/shardformer/layer/utils.py
+colossalai/shardformer/modeling/__init__.py
+colossalai/shardformer/modeling/bloom.py
+colossalai/shardformer/policies/__init__.py
+colossalai/shardformer/policies/autopolicy.py
+colossalai/shardformer/policies/basepolicy.py
+colossalai/shardformer/policies/bert.py
+colossalai/shardformer/policies/bloom.py
+colossalai/shardformer/policies/gpt2.py
+colossalai/shardformer/policies/llama.py
+colossalai/shardformer/policies/opt.py
+colossalai/shardformer/policies/t5.py
+colossalai/shardformer/policies/vit.py
+colossalai/shardformer/shard/__init__.py
+colossalai/shardformer/shard/shard_config.py
+colossalai/shardformer/shard/sharder.py
+colossalai/shardformer/shard/shardformer.py
 colossalai/tensor/__init__.py
 colossalai/tensor/colo_parameter.py
 colossalai/tensor/colo_tensor.py
 colossalai/tensor/comm_spec.py
 colossalai/tensor/compute_spec.py
 colossalai/tensor/const.py
 colossalai/tensor/dist_spec_mgr.py
@@ -517,16 +545,16 @@
 colossalai/tensor/param_op_hook.py
 colossalai/tensor/process_group.py
 colossalai/tensor/shape_consistency.py
 colossalai/tensor/sharding_spec.py
 colossalai/tensor/tensor_spec.py
 colossalai/tensor/utils.py
 colossalai/tensor/d_tensor/__init__.py
+colossalai/tensor/d_tensor/api.py
 colossalai/tensor/d_tensor/comm_spec.py
-colossalai/tensor/d_tensor/d_tensor.py
 colossalai/tensor/d_tensor/layout.py
 colossalai/tensor/d_tensor/layout_converter.py
 colossalai/tensor/d_tensor/misc.py
 colossalai/tensor/d_tensor/sharding_spec.py
 colossalai/tensor/d_tensor/utils.py
 colossalai/testing/__init__.py
 colossalai/testing/comparison.py
@@ -692,15 +720,17 @@
 tests/kit/model_zoo/torchrec/__init__.py
 tests/kit/model_zoo/torchrec/torchrec.py
 tests/kit/model_zoo/torchvision/__init__.py
 tests/kit/model_zoo/torchvision/torchvision.py
 tests/kit/model_zoo/transformers/__init__.py
 tests/kit/model_zoo/transformers/albert.py
 tests/kit/model_zoo/transformers/bert.py
+tests/kit/model_zoo/transformers/bloom.py
 tests/kit/model_zoo/transformers/gpt.py
+tests/kit/model_zoo/transformers/llama.py
 tests/kit/model_zoo/transformers/opt.py
 tests/kit/model_zoo/transformers/t5.py
 tests/test_analyzer/__init__.py
 tests/test_analyzer/test_fx/__init__.py
 tests/test_analyzer/test_fx/test_bias_addition.py
 tests/test_analyzer/test_fx/test_mod_dir.py
 tests/test_analyzer/test_fx/test_nested_ckpt.py
@@ -752,8 +782,19 @@
 tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_softmax_handler.py
 tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_split_handler.py
 tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_sum_handler.py
 tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_tensor_constructor.py
 tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_unary_element_wise_handler.py
 tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_view_handler.py
 tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_where_handler.py
-tests/test_auto_parallel/test_tensor_shard/test_node_handler/utils.py
+tests/test_auto_parallel/test_tensor_shard/test_node_handler/utils.py
+tests/test_shardformer/__init__.py
+tests/test_shardformer/test_with_torch_ddp.py
+tests/test_shardformer/test_model/__init__.py
+tests/test_shardformer/test_model/_utils.py
+tests/test_shardformer/test_model/test_shard_bert.py
+tests/test_shardformer/test_model/test_shard_bloom.py
+tests/test_shardformer/test_model/test_shard_gpt2.py
+tests/test_shardformer/test_model/test_shard_llama.py
+tests/test_shardformer/test_model/test_shard_opt.py
+tests/test_shardformer/test_model/test_shard_t5.py
+tests/test_shardformer/test_model/test_shard_vit.py
```

### Comparing `colossalai-nightly-2023.7.1/op_builder/__init__.py` & `colossalai-nightly-2023.7.8/op_builder/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/op_builder/builder.py` & `colossalai-nightly-2023.7.8/op_builder/builder.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/op_builder/cpu_adam.py` & `colossalai-nightly-2023.7.8/op_builder/cpu_adam.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/op_builder/fused_optim.py` & `colossalai-nightly-2023.7.8/op_builder/fused_optim.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/op_builder/layernorm.py` & `colossalai-nightly-2023.7.8/op_builder/layernorm.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/op_builder/moe.py` & `colossalai-nightly-2023.7.8/op_builder/moe.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/op_builder/multi_head_attn.py` & `colossalai-nightly-2023.7.8/op_builder/multi_head_attn.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/op_builder/scaled_masked_softmax.py` & `colossalai-nightly-2023.7.8/op_builder/scaled_masked_softmax.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/op_builder/scaled_upper_triangle_masked_softmax.py` & `colossalai-nightly-2023.7.8/op_builder/scaled_upper_triangle_masked_softmax.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/op_builder/utils.py` & `colossalai-nightly-2023.7.8/op_builder/utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/requirements/requirements-test.txt` & `colossalai-nightly-2023.7.8/requirements/requirements-test.txt`

 * *Files 20% similar despite different names*

```diff
@@ -11,7 +11,8 @@
 torchx-nightly==2022.6.29 # torchrec 0.2.0 requires torchx-nightly. This package is updated every day. We fix the version to a specific date to avoid breaking changes.
 torchrec==0.2.0
 contexttimer
 einops
 triton==2.0.0.dev20221202
 git+https://github.com/HazyResearch/flash-attention.git@c422fee3776eb3ea24e011ef641fd5fbeb212623#egg=flash_attn
 requests==2.27.1 # downgrade to avoid huggingface error https://github.com/huggingface/transformers/issues/17611
+SentencePiece
```

### Comparing `colossalai-nightly-2023.7.1/setup.py` & `colossalai-nightly-2023.7.8/setup.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/tests/components_to_test/albert.py` & `colossalai-nightly-2023.7.8/tests/components_to_test/albert.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/tests/components_to_test/beit.py` & `colossalai-nightly-2023.7.8/tests/components_to_test/beit.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/tests/components_to_test/bert.py` & `colossalai-nightly-2023.7.8/tests/components_to_test/bert.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/tests/components_to_test/gpt2.py` & `colossalai-nightly-2023.7.8/tests/components_to_test/gpt2.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/tests/components_to_test/hanging_param_model.py` & `colossalai-nightly-2023.7.8/tests/components_to_test/hanging_param_model.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/tests/components_to_test/inline_op_model.py` & `colossalai-nightly-2023.7.8/tests/components_to_test/inline_op_model.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/tests/components_to_test/nested_model.py` & `colossalai-nightly-2023.7.8/tests/components_to_test/nested_model.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/tests/components_to_test/registry.py` & `colossalai-nightly-2023.7.8/tests/components_to_test/registry.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/tests/components_to_test/repeated_computed_layers.py` & `colossalai-nightly-2023.7.8/tests/components_to_test/repeated_computed_layers.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/tests/components_to_test/resnet.py` & `colossalai-nightly-2023.7.8/tests/components_to_test/resnet.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/tests/components_to_test/simple_net.py` & `colossalai-nightly-2023.7.8/tests/components_to_test/simple_net.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/tests/components_to_test/utils/executor.py` & `colossalai-nightly-2023.7.8/tests/components_to_test/utils/executor.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/tests/kit/model_zoo/diffusers/diffusers.py` & `colossalai-nightly-2023.7.8/tests/kit/model_zoo/diffusers/diffusers.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/tests/kit/model_zoo/registry.py` & `colossalai-nightly-2023.7.8/tests/kit/model_zoo/registry.py`

 * *Files 11% similar despite different names*

```diff
@@ -24,45 +24,55 @@
     """
 
     def register(self,
                  name: str,
                  model_fn: Callable,
                  data_gen_fn: Callable,
                  output_transform_fn: Callable,
+                 loss_fn: Callable = None,
                  model_attribute: ModelAttribute = None):
         """
         Register a model and data generation function.
 
         Examples:
-        >>> # Register
-        >>> model_zoo = ModelZooRegistry()
-        >>> model_zoo.register('resnet18', resnet18, resnet18_data_gen)
-        >>> # Run the model
-        >>> data = resnet18_data_gen() # do not input any argument
-        >>> model = resnet18() # do not input any argument
-        >>> out = model(**data)
+
+        ```python
+        # normal forward workflow
+        model = resnet18()
+        data = resnet18_data_gen()
+        output = model(**data)
+        transformed_output = output_transform_fn(output)
+        loss = loss_fn(transformed_output)
+
+        # Register
+        model_zoo = ModelZooRegistry()
+        model_zoo.register('resnet18', resnet18, resnet18_data_gen, output_transform_fn, loss_fn)
+        ```
 
         Args:
             name (str): Name of the model.
-            model_fn (callable): A function that returns a model. **It must not contain any arguments.**
-            output_transform_fn (callable): A function that transforms the output of the model into Dict.
-            data_gen_fn (callable): A function that returns a data sample in the form of Dict. **It must not contain any arguments.**
+            model_fn (Callable): A function that returns a model. **It must not contain any arguments.**
+            data_gen_fn (Callable): A function that returns a data sample in the form of Dict. **It must not contain any arguments.**
+            output_transform_fn (Callable): A function that transforms the output of the model into Dict.
+            loss_fn (Callable): a function to compute the loss from the given output. Defaults to None
             model_attribute (ModelAttribute): Attributes of the model. Defaults to None.
         """
-        self[name] = (model_fn, data_gen_fn, output_transform_fn, model_attribute)
+        self[name] = (model_fn, data_gen_fn, output_transform_fn, loss_fn, model_attribute)
 
     def get_sub_registry(self, keyword: str):
         """
         Get a sub registry with models that contain the keyword.
 
         Args:
             keyword (str): Keyword to filter models.
         """
         new_dict = dict()
 
         for k, v in self.items():
             if keyword in k:
                 new_dict[k] = v
+
+        assert len(new_dict) > 0, f'No model found with keyword {keyword}'
         return new_dict
 
 
 model_zoo = ModelZooRegistry()
```

### Comparing `colossalai-nightly-2023.7.1/tests/kit/model_zoo/timm/timm.py` & `colossalai-nightly-2023.7.8/tests/kit/model_zoo/timm/timm.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/tests/kit/model_zoo/torchaudio/torchaudio.py` & `colossalai-nightly-2023.7.8/tests/kit/model_zoo/torchaudio/torchaudio.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/tests/kit/model_zoo/torchrec/torchrec.py` & `colossalai-nightly-2023.7.8/tests/kit/model_zoo/torchrec/torchrec.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/tests/kit/model_zoo/torchvision/torchvision.py` & `colossalai-nightly-2023.7.8/tests/kit/model_zoo/torchvision/torchvision.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/tests/kit/model_zoo/transformers/albert.py` & `colossalai-nightly-2023.7.8/tests/kit/model_zoo/transformers/albert.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/tests/kit/model_zoo/transformers/bert.py` & `colossalai-nightly-2023.7.8/tests/kit/model_zoo/transformers/gpt.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,88 +1,94 @@
 import torch
 import transformers
 
 from ..registry import ModelAttribute, model_zoo
 
 # ===============================
-# Register single-sentence BERT
+# Register single-sentence GPT
 # ===============================
-BATCH_SIZE = 2
-SEQ_LENGTH = 16
 
 
-def data_gen_fn():
-    input_ids = torch.zeros((BATCH_SIZE, SEQ_LENGTH), dtype=torch.int64)
-    token_type_ids = torch.zeros((BATCH_SIZE, SEQ_LENGTH), dtype=torch.int64)
-    attention_mask = torch.zeros((BATCH_SIZE, SEQ_LENGTH), dtype=torch.int64)
-    return dict(input_ids=input_ids, token_type_ids=token_type_ids, attention_mask=attention_mask)
+def data_gen():
+    # Generated from following code snippet
+    #
+    # from transformers import GPT2Tokenizer
+    # input = 'Hello, my dog is cute'
+    # tokenized_input = tokenizer(input, return_tensors='pt')
+    # input_ids = tokenized_input['input_ids']
+    # attention_mask = tokenized_input['attention_mask']
+    input_ids = torch.tensor([[15496, 11, 616, 3290, 318, 13779]], dtype=torch.int64)
+    attention_mask = torch.tensor([[1, 1, 1, 1, 1, 1]], dtype=torch.int64)
+    return dict(input_ids=input_ids, attention_mask=attention_mask)
+
+
+def data_gen_for_lm():
+    # LM data gen
+    # the `labels` of LM is the token of the output, cause no padding, use `input_ids` as `labels`
+    data = data_gen()
+    data['labels'] = data['input_ids'].clone()
+    return data
+
+
+def data_gen_for_token_classification():
+    # token classification data gen
+    # `labels` is the type not the token id for token classification, 0 or 1
+    data = data_gen()
+    data['labels'] = torch.tensor([[0, 0, 0, 0, 0, 0]], dtype=torch.int64)
+    return data
+
+
+def data_gen_for_sequence_classification():
+    # sequence classification data gen
+    data = data_gen()
+    data['labels'] = torch.tensor([0], dtype=torch.int64)
+    return data
 
 
+# define output transform function
 output_transform_fn = lambda x: x
 
-config = transformers.BertConfig(hidden_size=128, num_hidden_layers=2, num_attention_heads=4, intermediate_size=256)
+# define loss function
+loss_fn_for_gpt2_model = lambda x: x.last_hidden_state.mean()
+loss_fn = lambda x: x.loss
+
+config = transformers.GPT2Config(n_layer=2,
+                                 n_head=4,
+                                 vocab_size=50258,
+                                 attn_pdrop=0,
+                                 embd_pdrop=0,
+                                 resid_pdrop=0,
+                                 summary_first_dropout=0,
+                                 hidden_dropout=0,
+                                 problem_type="single_label_classification")
 
-# register the BERT variants
-model_zoo.register(name='transformers_bert',
-                   model_fn=lambda: transformers.BertModel(config),
-                   data_gen_fn=data_gen_fn,
-                   output_transform_fn=output_transform_fn,
-                   model_attribute=ModelAttribute(has_control_flow=True))
-model_zoo.register(name='transformers_bert_for_pretraining',
-                   model_fn=lambda: transformers.BertForPreTraining(config),
-                   data_gen_fn=data_gen_fn,
-                   output_transform_fn=output_transform_fn,
-                   model_attribute=ModelAttribute(has_control_flow=True))
-model_zoo.register(name='transformers_bert_lm_head_model',
-                   model_fn=lambda: transformers.BertLMHeadModel(config),
-                   data_gen_fn=data_gen_fn,
-                   output_transform_fn=output_transform_fn,
-                   model_attribute=ModelAttribute(has_control_flow=True))
-model_zoo.register(name='transformers_bert_for_masked_lm',
-                   model_fn=lambda: transformers.BertForMaskedLM(config),
-                   data_gen_fn=data_gen_fn,
+# register the following models
+model_zoo.register(name='transformers_gpt',
+                   model_fn=lambda: transformers.GPT2Model(config),
+                   data_gen_fn=data_gen,
                    output_transform_fn=output_transform_fn,
+                   loss_fn=loss_fn_for_gpt2_model,
                    model_attribute=ModelAttribute(has_control_flow=True))
-model_zoo.register(name='transformers_bert_for_sequence_classification',
-                   model_fn=lambda: transformers.BertForSequenceClassification(config),
-                   data_gen_fn=data_gen_fn,
+model_zoo.register(name='transformers_gpt_lm',
+                   model_fn=lambda: transformers.GPT2LMHeadModel(config),
+                   data_gen_fn=data_gen_for_lm,
                    output_transform_fn=output_transform_fn,
+                   loss_fn=loss_fn,
                    model_attribute=ModelAttribute(has_control_flow=True))
-model_zoo.register(name='transformers_bert_for_token_classification',
-                   model_fn=lambda: transformers.BertForTokenClassification(config),
-                   data_gen_fn=data_gen_fn,
+model_zoo.register(name='transformers_gpt_double_heads',
+                   model_fn=lambda: transformers.GPT2DoubleHeadsModel(config),
+                   data_gen_fn=data_gen_for_lm,
                    output_transform_fn=output_transform_fn,
+                   loss_fn=loss_fn,
                    model_attribute=ModelAttribute(has_control_flow=True))
-
-
-# ===============================
-# Register multi-sentence BERT
-# ===============================
-def data_gen_for_next_sentence():
-    tokenizer = transformers.BertTokenizer.from_pretrained("bert-base-uncased")
-    prompt = "In Italy, pizza served in formal settings, such as at a restaurant, is presented unsliced."
-    next_sentence = "The sky is blue due to the shorter wavelength of blue light."
-    encoding = tokenizer(prompt, next_sentence, return_tensors="pt")
-    return encoding
-
-
-def data_gen_for_mcq():
-    tokenizer = transformers.BertTokenizer.from_pretrained("bert-base-uncased")
-    prompt = "In Italy, pizza served in formal settings, such as at a restaurant, is presented unsliced."
-    choice0 = "It is eaten with a fork and a knife."
-    choice1 = "It is eaten while held in the hand."
-    encoding = tokenizer([prompt, prompt], [choice0, choice1], return_tensors="pt", padding=True)
-    encoding = {k: v.unsqueeze(0) for k, v in encoding.items()}
-    return encoding
-
-
-# register the following models
-model_zoo.register(name='transformers_bert_for_next_sentence',
-                   model_fn=lambda: transformers.BertForNextSentencePrediction(config),
-                   data_gen_fn=data_gen_for_next_sentence,
+model_zoo.register(name='transformers_gpt_for_token_classification',
+                   model_fn=lambda: transformers.GPT2ForTokenClassification(config),
+                   data_gen_fn=data_gen_for_token_classification,
                    output_transform_fn=output_transform_fn,
+                   loss_fn=loss_fn,
                    model_attribute=ModelAttribute(has_control_flow=True))
-model_zoo.register(name='transformers_bert_for_mcq',
-                   model_fn=lambda: transformers.BertForMultipleChoice(config),
-                   data_gen_fn=data_gen_for_mcq,
+model_zoo.register(name='transformers_gpt_for_sequence_classification',
+                   model_fn=lambda: transformers.GPT2ForSequenceClassification(config),
+                   data_gen_fn=data_gen_for_sequence_classification,
                    output_transform_fn=output_transform_fn,
+                   loss_fn=loss_fn,
                    model_attribute=ModelAttribute(has_control_flow=True))
```

### Comparing `colossalai-nightly-2023.7.1/tests/test_analyzer/test_fx/test_bias_addition.py` & `colossalai-nightly-2023.7.8/tests/test_analyzer/test_fx/test_bias_addition.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/tests/test_analyzer/test_fx/test_mod_dir.py` & `colossalai-nightly-2023.7.8/tests/test_analyzer/test_fx/test_mod_dir.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/tests/test_analyzer/test_fx/test_nested_ckpt.py` & `colossalai-nightly-2023.7.8/tests/test_analyzer/test_fx/test_nested_ckpt.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/tests/test_analyzer/test_fx/test_shape_prop.py` & `colossalai-nightly-2023.7.8/tests/test_analyzer/test_fx/test_shape_prop.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/tests/test_analyzer/test_fx/test_symbolic_profile.py` & `colossalai-nightly-2023.7.8/tests/test_analyzer/test_fx/test_symbolic_profile.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/tests/test_analyzer/test_fx/zoo.py` & `colossalai-nightly-2023.7.8/tests/test_analyzer/test_fx/zoo.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/tests/test_analyzer/test_subclasses/test_aten.py` & `colossalai-nightly-2023.7.8/tests/test_analyzer/test_subclasses/test_aten.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/tests/test_analyzer/test_subclasses/test_flop_tensor.py` & `colossalai-nightly-2023.7.8/tests/test_analyzer/test_subclasses/test_flop_tensor.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/tests/test_analyzer/test_subclasses/test_meta_mode.py` & `colossalai-nightly-2023.7.8/tests/test_analyzer/test_subclasses/test_meta_mode.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/tests/test_auto_parallel/test_pass/test_node_converting_pass.py` & `colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_pass/test_node_converting_pass.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/tests/test_auto_parallel/test_pass/test_size_value_converting_pass.py` & `colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_pass/test_size_value_converting_pass.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/tests/test_auto_parallel/test_tensor_shard/test_bias_addition_forward.py` & `colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_bias_addition_forward.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/tests/test_auto_parallel/test_tensor_shard/test_broadcast.py` & `colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_broadcast.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/tests/test_auto_parallel/test_tensor_shard/test_checkpoint.py` & `colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_checkpoint.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/tests/test_auto_parallel/test_tensor_shard/test_compatibility_with_ddp.py` & `colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_compatibility_with_ddp.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/tests/test_auto_parallel/test_tensor_shard/test_compatibility_with_gemini.py` & `colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_compatibility_with_gemini.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/tests/test_auto_parallel/test_tensor_shard/test_find_repeat_block.py` & `colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_find_repeat_block.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/tests/test_auto_parallel/test_tensor_shard/test_gpt/gpt_modules.py` & `colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_gpt/gpt_modules.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/tests/test_auto_parallel/test_tensor_shard/test_gpt/test_runtime_with_gpt_modules.py` & `colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_gpt/test_runtime_with_gpt_modules.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/tests/test_auto_parallel/test_tensor_shard/test_gpt/test_solver_with_gpt_module.py` & `colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_gpt/test_solver_with_gpt_module.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/tests/test_auto_parallel/test_tensor_shard/test_liveness_analysis.py` & `colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_liveness_analysis.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_addbmm_handler.py` & `colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_addbmm_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_addmm_handler.py` & `colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_addmm_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_batch_norm_handler.py` & `colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_batch_norm_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_bias_linear_function_node.py` & `colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_bias_linear_function_node.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_bias_linear_module_node.py` & `colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_bias_linear_module_node.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_binary_elementwise_handler.py` & `colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_binary_elementwise_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_bmm_handler.py` & `colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_bmm_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_conv_handler.py` & `colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_conv_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_default_reshape_handler.py` & `colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_default_reshape_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_embedding_handler.py` & `colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_embedding_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_getattr_handler.py` & `colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_getattr_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_getitem_handler.py` & `colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_getitem_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_layer_norm_handler.py` & `colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_layer_norm_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_linear_handler.py` & `colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_linear_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_matmul_handler.py` & `colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_matmul_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_norm_pooling_handler.py` & `colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_norm_pooling_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_output_handler.py` & `colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_output_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_permute_and_transpose_handler.py` & `colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_permute_and_transpose_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_placeholder_handler.py` & `colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_placeholder_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_shard_option.py` & `colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_shard_option.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_softmax_handler.py` & `colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_softmax_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_split_handler.py` & `colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_split_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_sum_handler.py` & `colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_sum_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_tensor_constructor.py` & `colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_tensor_constructor.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_unary_element_wise_handler.py` & `colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_unary_element_wise_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_view_handler.py` & `colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_view_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_where_handler.py` & `colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_where_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/tests/test_auto_parallel/test_tensor_shard/test_node_handler/utils.py` & `colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.1/tests/test_auto_parallel/test_tensor_shard/test_solver_with_resnet_v2.py` & `colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_solver_with_resnet_v2.py`

 * *Files identical despite different names*

