# Comparing `tmp/mct-nightly-1.9.0.20230706.post446.tar.gz` & `tmp/mct-nightly-1.9.0.20230707.post446.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mct-nightly-1.9.0.20230706.post446.tar", last modified: Thu Jul  6 00:04:47 2023, max compression
+gzip compressed data, was "mct-nightly-1.9.0.20230707.post446.tar", last modified: Fri Jul  7 00:04:47 2023, max compression
```

## Comparing `mct-nightly-1.9.0.20230706.post446.tar` & `mct-nightly-1.9.0.20230707.post446.tar`

### file list

```diff
@@ -1,529 +1,526 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 00:04:47.757074 mct-nightly-1.9.0.20230706.post446/
--rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)    11727 2023-07-06 00:04:47.757074 mct-nightly-1.9.0.20230706.post446/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10054 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 00:04:47.721074 mct-nightly-1.9.0.20230706.post446/mct_nightly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11727 2023-07-06 00:04:47.000000 mct-nightly-1.9.0.20230706.post446/mct_nightly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    32808 2023-07-06 00:04:47.000000 mct-nightly-1.9.0.20230706.post446/mct_nightly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 00:04:47.000000 mct-nightly-1.9.0.20230706.post446/mct_nightly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-07-06 00:04:47.000000 mct-nightly-1.9.0.20230706.post446/mct_nightly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-06 00:04:47.000000 mct-nightly-1.9.0.20230706.post446/mct_nightly.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 00:04:47.721074 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/
--rw-r--r--   0 runner    (1001) docker     (123)     3608 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3949 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 00:04:47.721074 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/
--rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2975 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/analyzer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 00:04:47.725075 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/
--rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 00:04:47.725075 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/back2framework/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/back2framework/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/back2framework/base_model_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/base_substitutions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 00:04:47.725075 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/collectors/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/collectors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2576 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/collectors/base_collector.py
--rw-r--r--   0 runner    (1001) docker     (123)     6864 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/collectors/histogram_collector.py
--rw-r--r--   0 runner    (1001) docker     (123)     3888 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/collectors/mean_collector.py
--rw-r--r--   0 runner    (1001) docker     (123)     5207 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/collectors/min_max_per_channel_collector.py
--rw-r--r--   0 runner    (1001) docker     (123)     7929 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/collectors/statistics_collector.py
--rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/collectors/statistics_collector_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4017 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/data_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2281 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/defaultdict.py
--rw-r--r--   0 runner    (1001) docker     (123)    22391 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/framework_implementation.py
--rw-r--r--   0 runner    (1001) docker     (123)     6424 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/framework_info.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 00:04:47.725075 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/fusion/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/fusion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5479 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/fusion/layer_fusing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 00:04:47.725075 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/graph/
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28860 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/graph/base_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)    20579 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/graph/base_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     3733 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/graph/edge.py
--rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/graph/functional_node.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4732 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/graph/graph_matchers.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5128 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/graph/graph_searches.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 00:04:47.725075 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/graph/memory_graph/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/graph/memory_graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3880 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/graph/memory_graph/bipartite_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     2612 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/graph/memory_graph/compute_graph_max_cut.py
--rw-r--r--   0 runner    (1001) docker     (123)     2470 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/graph/memory_graph/cut.py
--rw-r--r--   0 runner    (1001) docker     (123)    17045 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/graph/memory_graph/max_cut_astar.py
--rw-r--r--   0 runner    (1001) docker     (123)     3961 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/graph/memory_graph/memory_element.py
--rw-r--r--   0 runner    (1001) docker     (123)     7175 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/graph/memory_graph/memory_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     9265 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/graph/virtual_activation_weights_node.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 00:04:47.725075 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/matchers/
--rwxr-xr-x   0 runner    (1001) docker     (123)      697 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/matchers/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3091 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/matchers/base_graph_filter.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2210 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/matchers/base_matcher.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3706 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/matchers/edge_matcher.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1773 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/matchers/function.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2745 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/matchers/node_matcher.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1111 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/matchers/walk_matcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/memory_computation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 00:04:47.725075 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/mixed_precision/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/mixed_precision/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6704 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/mixed_precision/bit_width_setter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/mixed_precision/distance_weighting.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 00:04:47.729075 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/mixed_precision/kpi_tools/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/mixed_precision/kpi_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4297 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/mixed_precision/kpi_tools/kpi.py
--rw-r--r--   0 runner    (1001) docker     (123)     3920 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/mixed_precision/kpi_tools/kpi_aggregation_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)     7046 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/mixed_precision/kpi_tools/kpi_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/mixed_precision/kpi_tools/kpi_functions_mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)    19323 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/mixed_precision/kpi_tools/kpi_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)     8041 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/mixed_precision/mixed_precision_quantization_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6822 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/mixed_precision/mixed_precision_search_facade.py
--rw-r--r--   0 runner    (1001) docker     (123)    34622 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/mixed_precision/mixed_precision_search_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 00:04:47.729075 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/mixed_precision/search_methods/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/mixed_precision/search_methods/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15453 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/mixed_precision/search_methods/linear_programming.py
--rw-r--r--   0 runner    (1001) docker     (123)    25266 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/mixed_precision/sensitivity_evaluation.py
--rw-r--r--   0 runner    (1001) docker     (123)     6326 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/mixed_precision/solution_refinement_procedure.py
--rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/model_builder_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)     5005 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/model_collector.py
--rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/model_validation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 00:04:47.729075 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/network_editors/
--rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/network_editors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17994 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/network_editors/actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/network_editors/edit_network.py
--rw-r--r--   0 runner    (1001) docker     (123)     3149 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/network_editors/node_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/node_prior_info.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 00:04:47.729075 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/quantization/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/quantization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3022 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/quantization/candidate_node_quantization_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/quantization/core_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/quantization/debug_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6137 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/quantization/filter_nodes_candidates.py
--rw-r--r--   0 runner    (1001) docker     (123)    16271 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/quantization/node_quantization_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/quantization/quantization_analyzer.py
--rw-r--r--   0 runner    (1001) docker     (123)     7247 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/quantization/quantization_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/quantization/quantization_fn_selection.py
--rw-r--r--   0 runner    (1001) docker     (123)     4090 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/quantization/quantization_params_fn_selection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 00:04:47.729075 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/quantization/quantization_params_generation/
--rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/quantization/quantization_params_generation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16505 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/quantization/quantization_params_generation/error_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2927 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/quantization/quantization_params_generation/kmeans_params.py
--rw-r--r--   0 runner    (1001) docker     (123)     7292 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/quantization/quantization_params_generation/lut_kmeans_params.py
--rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/quantization/quantization_params_generation/outlier_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     8484 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/quantization/quantization_params_generation/power_of_two_selection.py
--rw-r--r--   0 runner    (1001) docker     (123)     4558 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/quantization/quantization_params_generation/qparams_activations_computation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4315 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/quantization/quantization_params_generation/qparams_computation.py
--rw-r--r--   0 runner    (1001) docker     (123)    41685 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/quantization/quantization_params_generation/qparams_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     5090 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/quantization/quantization_params_generation/qparams_weights_computation.py
--rw-r--r--   0 runner    (1001) docker     (123)     9689 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/quantization/quantization_params_generation/symmetric_selection.py
--rw-r--r--   0 runner    (1001) docker     (123)     7879 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/quantization/quantization_params_generation/uniform_selection.py
--rw-r--r--   0 runner    (1001) docker     (123)     2939 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/quantization/quantize_graph_weights.py
--rw-r--r--   0 runner    (1001) docker     (123)     3614 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/quantization/quantize_node.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 00:04:47.729075 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/quantization/quantizers/
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/quantization/quantizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/quantization/quantizers/kmeans_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2774 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/quantization/quantizers/lut_kmeans_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    14210 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/quantization/quantizers/quantizers_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5486 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/quantization/quantizers/uniform_quantizers.py
--rw-r--r--   0 runner    (1001) docker     (123)    10683 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/quantization/set_node_quantization_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     7450 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/similarity_analyzer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 00:04:47.729075 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/statistics_correction/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/statistics_correction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3434 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/statistics_correction/apply_bias_correction_to_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     5956 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/statistics_correction/apply_second_moment_correction_to_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)    10228 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/statistics_correction/compute_bias_correction_of_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     5584 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/statistics_correction/statistics_correction.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 00:04:47.733075 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/substitutions/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/substitutions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/substitutions/apply_substitutions.py
--rw-r--r--   0 runner    (1001) docker     (123)    12692 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/substitutions/batchnorm_folding.py
--rw-r--r--   0 runner    (1001) docker     (123)     5892 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/substitutions/batchnorm_reconstruction.py
--rw-r--r--   0 runner    (1001) docker     (123)     9962 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/substitutions/batchnorm_refusing.py
--rw-r--r--   0 runner    (1001) docker     (123)     9093 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/substitutions/linear_collapsing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/substitutions/linear_collapsing_substitution.py
--rw-r--r--   0 runner    (1001) docker     (123)     4866 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/substitutions/residual_collapsing.py
--rw-r--r--   0 runner    (1001) docker     (123)    10978 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/substitutions/scale_equalization.py
--rw-r--r--   0 runner    (1001) docker     (123)    26835 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/substitutions/shift_negative_activation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/substitutions/softmax_shift.py
--rw-r--r--   0 runner    (1001) docker     (123)     3400 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/substitutions/virtual_activation_weights_composition.py
--rw-r--r--   0 runner    (1001) docker     (123)     4228 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/substitutions/weights_activation_split.py
--rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/user_info.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 00:04:47.733075 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/visualization/
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/visualization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6371 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/visualization/final_config_visualizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5955 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/visualization/nn_visualizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    20099 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/visualization/tensorboard_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4233 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/exporter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 00:04:47.733075 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/keras/
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/keras/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 00:04:47.733075 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/keras/back2framework/
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/keras/back2framework/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/keras/back2framework/factory_model_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2444 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/keras/back2framework/float_model_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     4508 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/keras/back2framework/instance_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)    16452 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/keras/back2framework/keras_model_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     7150 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/keras/back2framework/mixed_precision_model_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)    15316 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/keras/back2framework/model_gradients.py
--rw-r--r--   0 runner    (1001) docker     (123)     2481 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/keras/back2framework/quantized_model_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2664 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/keras/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     4999 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/keras/default_framework_info.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 00:04:47.733075 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/keras/graph_substitutions/
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/keras/graph_substitutions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 00:04:47.737074 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/keras/graph_substitutions/substitutions/
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/keras/graph_substitutions/substitutions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3940 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/keras/graph_substitutions/substitutions/activation_decomposition.py
--rw-r--r--   0 runner    (1001) docker     (123)     7317 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/keras/graph_substitutions/substitutions/batchnorm_folding.py
--rw-r--r--   0 runner    (1001) docker     (123)     3168 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/keras/graph_substitutions/substitutions/batchnorm_reconstruction.py
--rw-r--r--   0 runner    (1001) docker     (123)     2478 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/keras/graph_substitutions/substitutions/batchnorm_refusing.py
--rw-r--r--   0 runner    (1001) docker     (123)     5598 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/keras/graph_substitutions/substitutions/input_scaling.py
--rw-r--r--   0 runner    (1001) docker     (123)     5925 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/keras/graph_substitutions/substitutions/linear_collapsing.py
--rw-r--r--   0 runner    (1001) docker     (123)    26778 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/keras/graph_substitutions/substitutions/multi_head_attention_decomposition.py
--rw-r--r--   0 runner    (1001) docker     (123)     3872 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/keras/graph_substitutions/substitutions/relu_bound_to_power_of_2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2387 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/keras/graph_substitutions/substitutions/remove_relu_upper_bound.py
--rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/keras/graph_substitutions/substitutions/residual_collapsing.py
--rw-r--r--   0 runner    (1001) docker     (123)     5542 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/keras/graph_substitutions/substitutions/scale_equalization.py
--rw-r--r--   0 runner    (1001) docker     (123)     7714 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/keras/graph_substitutions/substitutions/separableconv_decomposition.py
--rw-r--r--   0 runner    (1001) docker     (123)    10781 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/keras/graph_substitutions/substitutions/shift_negative_activation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/keras/graph_substitutions/substitutions/softmax_shift.py
--rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/keras/graph_substitutions/substitutions/virtual_activation_weights_composition.py
--rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/keras/graph_substitutions/substitutions/weights_activation_split.py
--rw-r--r--   0 runner    (1001) docker     (123)    27295 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/keras/keras_implementation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/keras/keras_model_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3941 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/keras/keras_node_prior_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     8600 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/keras/kpi_data_facade.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 00:04:47.737074 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/keras/mixed_precision/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/keras/mixed_precision/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/keras/mixed_precision/set_layer_to_bitwidth.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 00:04:47.737074 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/keras/quantizer/
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/keras/quantizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/keras/quantizer/base_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6151 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/keras/quantizer/fake_quant_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3120 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/keras/quantizer/input_layer_quantize_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     4507 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/keras/quantizer/lut_fake_quant.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 00:04:47.737074 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/keras/quantizer/mixed_precision/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/keras/quantizer/mixed_precision/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2837 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/keras/quantizer/mixed_precision/quantization_config_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     6854 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/keras/quantizer/mixed_precision/selective_activation_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    10902 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/keras/quantizer/mixed_precision/selective_quantize_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     7621 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/keras/quantizer/mixed_precision/selective_weights_quantizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 00:04:47.737074 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/keras/reader/
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/keras/reader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2627 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/keras/reader/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    11418 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/keras/reader/connectivity_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 00:04:47.737074 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/keras/reader/nested_model/
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/keras/reader/nested_model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7906 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/keras/reader/nested_model/edges_merger.py
--rw-r--r--   0 runner    (1001) docker     (123)     2760 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/keras/reader/nested_model/nested_model_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/keras/reader/nested_model/nodes_merger.py
--rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/keras/reader/nested_model/outputs_merger.py
--rw-r--r--   0 runner    (1001) docker     (123)     5951 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/keras/reader/node_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     8109 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/keras/reader/reader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 00:04:47.737074 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/keras/statistics_correction/
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/keras/statistics_correction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/keras/statistics_correction/apply_second_moment_correction.py
--rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/keras/tf_tensor_numpy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 00:04:47.737074 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/keras/visualization/
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/keras/visualization/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 00:04:47.737074 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/pytorch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 00:04:47.737074 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/pytorch/back2framework/
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/pytorch/back2framework/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2274 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/pytorch/back2framework/factory_model_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3419 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/pytorch/back2framework/float_model_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/pytorch/back2framework/instance_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     4976 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/pytorch/back2framework/mixed_precision_model_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)    18214 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/pytorch/back2framework/model_gradients.py
--rw-r--r--   0 runner    (1001) docker     (123)    16443 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/pytorch/back2framework/pytorch_model_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 00:04:47.737074 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/pytorch/back2framework/quantization_wrapper/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/pytorch/back2framework/quantization_wrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5773 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/pytorch/back2framework/quantization_wrapper/quantized_layer_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/pytorch/back2framework/quantization_wrapper/wrapper_quantize_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3456 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/pytorch/back2framework/quantized_model_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/pytorch/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     4224 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/pytorch/default_framework_info.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 00:04:47.737074 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/pytorch/graph_substitutions/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/pytorch/graph_substitutions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 00:04:47.741074 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6840 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/batchnorm_folding.py
--rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/batchnorm_reconstruction.py
--rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/batchnorm_refusing.py
--rw-r--r--   0 runner    (1001) docker     (123)     4804 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/const_holder_conv.py
--rw-r--r--   0 runner    (1001) docker     (123)     5797 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/linear_collapsing.py
--rw-r--r--   0 runner    (1001) docker     (123)    38353 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/multi_head_attention_decomposition.py
--rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/permute_call_method.py
--rw-r--r--   0 runner    (1001) docker     (123)     5601 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/relu_bound_to_power_of_2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4148 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/reshape_with_static_shapes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2899 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/residual_collapsing.py
--rw-r--r--   0 runner    (1001) docker     (123)     3303 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/scale_equalization.py
--rw-r--r--   0 runner    (1001) docker     (123)     9838 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/shift_negative_activation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/softmax_shift.py
--rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/virtual_activation_weights_composition.py
--rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/weights_activation_split.py
--rw-r--r--   0 runner    (1001) docker     (123)     8482 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/pytorch/kpi_data_facade.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 00:04:47.741074 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/pytorch/mixed_precision/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/pytorch/mixed_precision/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11345 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/pytorch/mixed_precision/mixed_precision_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/pytorch/mixed_precision/set_layer_to_bitwidth.py
--rw-r--r--   0 runner    (1001) docker     (123)    25800 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/pytorch/pytorch_implementation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3250 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/pytorch/pytorch_node_prior_info.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 00:04:47.741074 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/pytorch/quantizer/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/pytorch/quantizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6464 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/pytorch/quantizer/fake_quant_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     4452 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/pytorch/quantizer/lut_fake_quant.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 00:04:47.741074 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/pytorch/reader/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/pytorch/reader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12113 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/pytorch/reader/graph_builders.py
--rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/pytorch/reader/node_holders.py
--rw-r--r--   0 runner    (1001) docker     (123)     5801 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/pytorch/reader/reader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 00:04:47.741074 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/pytorch/statistics_correction/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/pytorch/statistics_correction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3261 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/pytorch/statistics_correction/apply_second_moment_correction.py
--rw-r--r--   0 runner    (1001) docker     (123)     2959 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/pytorch/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    23009 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/runner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 00:04:47.741074 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/exporter/
--rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/exporter/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 00:04:47.741074 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/exporter/model_exporter/
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/exporter/model_exporter/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 00:04:47.741074 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/exporter/model_exporter/fw_agonstic/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/exporter/model_exporter/fw_agonstic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/exporter/model_exporter/fw_agonstic/exporter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 00:04:47.741074 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/exporter/model_exporter/keras/
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/exporter/model_exporter/keras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/exporter/model_exporter/keras/base_keras_exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/exporter/model_exporter/keras/export_serialization_format.py
--rw-r--r--   0 runner    (1001) docker     (123)    11100 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/exporter/model_exporter/keras/fakely_quant_keras_exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3043 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/exporter/model_exporter/keras/fakely_quant_tflite_exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     8048 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/exporter/model_exporter/keras/int8_tflite_exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6016 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/exporter/model_exporter/keras/keras_export_facade.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 00:04:47.741074 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/exporter/model_exporter/pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/exporter/model_exporter/pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4020 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/exporter/model_exporter/pytorch/base_pytorch_exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/exporter/model_exporter/pytorch/export_serialization_format.py
--rw-r--r--   0 runner    (1001) docker     (123)     3298 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/exporter/model_exporter/pytorch/fakely_quant_onnx_pytorch_exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/exporter/model_exporter/pytorch/fakely_quant_torchscript_pytorch_exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5866 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/exporter/model_exporter/pytorch/pytorch_export_facade.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 00:04:47.741074 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/exporter/model_wrapper/
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/exporter/model_wrapper/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 00:04:47.741074 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/exporter/model_wrapper/keras/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/exporter/model_wrapper/keras/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 00:04:47.745075 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/exporter/model_wrapper/keras/builder/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/exporter/model_wrapper/keras/builder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4287 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/exporter/model_wrapper/keras/builder/fully_quantized_model_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     8764 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/exporter/model_wrapper/keras/builder/node_to_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/exporter/model_wrapper/keras/builder/node_to_quantizers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3543 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/exporter/model_wrapper/keras/validate_layer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 00:04:47.745075 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/exporter/model_wrapper/pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/exporter/model_wrapper/pytorch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 00:04:47.745075 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/exporter/model_wrapper/pytorch/builder/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/exporter/model_wrapper/pytorch/builder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3921 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/exporter/model_wrapper/pytorch/builder/fully_quantized_model_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     8656 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/exporter/model_wrapper/pytorch/builder/node_to_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/exporter/model_wrapper/pytorch/builder/node_to_quantizers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3449 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/exporter/model_wrapper/pytorch/validate_layer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 00:04:47.745075 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/gptq/
--rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/gptq/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 00:04:47.745075 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/gptq/common/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/gptq/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9508 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/gptq/common/gptq_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/gptq/common/gptq_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/gptq/common/gptq_framework_implementation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2826 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/gptq/common/gptq_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)    15167 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/gptq/common/gptq_training.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 00:04:47.745075 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/gptq/keras/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/gptq/keras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/gptq/keras/gptq_keras_implementation.py
--rw-r--r--   0 runner    (1001) docker     (123)     6241 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/gptq/keras/gptq_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)    17319 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/gptq/keras/gptq_training.py
--rw-r--r--   0 runner    (1001) docker     (123)     4564 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/gptq/keras/graph_info.py
--rw-r--r--   0 runner    (1001) docker     (123)    14791 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/gptq/keras/quantization_facade.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 00:04:47.745075 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/gptq/keras/quantizer/
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/gptq/keras/quantizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4751 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/gptq/keras/quantizer/base_keras_gptq_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5055 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/gptq/keras/quantizer/quant_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4431 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/gptq/keras/quantizer/quantization_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/gptq/keras/quantizer/regularization_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 00:04:47.745075 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3962 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/soft_quantizer_reg.py
--rw-r--r--   0 runner    (1001) docker     (123)    12163 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/symmetric_soft_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    10381 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/uniform_soft_quantizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 00:04:47.745075 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/gptq/keras/quantizer/ste_rounding/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/gptq/keras/quantizer/ste_rounding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8370 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/gptq/keras/quantizer/ste_rounding/symmetric_ste.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 00:04:47.745075 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/gptq/pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/gptq/pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/gptq/pytorch/gptq_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/gptq/pytorch/gptq_pytorch_implementation.py
--rw-r--r--   0 runner    (1001) docker     (123)    14668 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/gptq/pytorch/gptq_training.py
--rw-r--r--   0 runner    (1001) docker     (123)     3955 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/gptq/pytorch/graph_info.py
--rw-r--r--   0 runner    (1001) docker     (123)    12768 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/gptq/pytorch/quantization_facade.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 00:04:47.745075 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/gptq/pytorch/quantizer/
--rw-r--r--   0 runner    (1001) docker     (123)      968 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/gptq/pytorch/quantizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4171 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/gptq/pytorch/quantizer/base_pytorch_gptq_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3893 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/gptq/pytorch/quantizer/quant_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4291 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/gptq/pytorch/quantizer/quantization_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/gptq/pytorch/quantizer/regularization_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 00:04:47.749075 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4132 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/soft_quantizer_reg.py
--rw-r--r--   0 runner    (1001) docker     (123)    12351 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/symmetric_soft_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     9103 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/uniform_soft_quantizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 00:04:47.749075 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/gptq/pytorch/quantizer/ste_rounding/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/gptq/pytorch/quantizer/ste_rounding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8782 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/gptq/pytorch/quantizer/ste_rounding/symmetric_ste.py
--rw-r--r--   0 runner    (1001) docker     (123)     5534 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/gptq/runner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 00:04:47.749075 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/legacy/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/legacy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18116 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/legacy/keras_quantization_facade.py
--rw-r--r--   0 runner    (1001) docker     (123)    17664 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/legacy/pytorch_quantization_facade.py
--rw-r--r--   0 runner    (1001) docker     (123)     4863 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 00:04:47.749075 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/ptq/
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/ptq/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 00:04:47.749075 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/ptq/keras/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/ptq/keras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9868 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/ptq/keras/quantization_facade.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 00:04:47.749075 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/ptq/pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/ptq/pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8580 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/ptq/pytorch/quantization_facade.py
--rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/ptq/runner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 00:04:47.749075 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/qat/
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/qat/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 00:04:47.749075 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/qat/common/
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/qat/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3295 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/qat/common/qat_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 00:04:47.749075 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/qat/keras/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/qat/keras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16051 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/qat/keras/quantization_facade.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 00:04:47.749075 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/qat/keras/quantizer/
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/qat/keras/quantizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/qat/keras/quantizer/base_keras_qat_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/qat/keras/quantizer/quant_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5635 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/qat/keras/quantizer/quantization_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 00:04:47.749075 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/qat/keras/quantizer/ste_rounding/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/qat/keras/quantizer/ste_rounding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13436 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/qat/keras/quantizer/ste_rounding/symmetric_ste.py
--rw-r--r--   0 runner    (1001) docker     (123)    10708 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/qat/keras/quantizer/ste_rounding/uniform_ste.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 00:04:47.749075 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/qat/pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/qat/pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12461 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/qat/pytorch/quantization_facade.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 00:04:47.749075 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/qat/pytorch/quantizer/
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/qat/pytorch/quantizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/qat/pytorch/quantizer/base_pytorch_qat_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5491 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/qat/pytorch/quantizer/quantization_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     5004 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/qat/pytorch/quantizer/quantizer_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 00:04:47.749075 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/qat/pytorch/quantizer/ste_rounding/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/qat/pytorch/quantizer/ste_rounding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9629 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/qat/pytorch/quantizer/ste_rounding/symmetric_ste.py
--rw-r--r--   0 runner    (1001) docker     (123)     8651 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/qat/pytorch/quantizer/ste_rounding/uniform_ste.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 00:04:47.749075 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/target_platform_capabilities/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/target_platform_capabilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/target_platform_capabilities/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/target_platform_capabilities/immutable.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 00:04:47.749075 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/target_platform_capabilities/target_platform/
--rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/target_platform_capabilities/target_platform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/target_platform_capabilities/target_platform/current_tp_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/target_platform_capabilities/target_platform/fusing.py
--rw-r--r--   0 runner    (1001) docker     (123)     8538 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/target_platform_capabilities/target_platform/op_quantization_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/target_platform_capabilities/target_platform/operators.py
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/target_platform_capabilities/target_platform/quantization_format.py
--rw-r--r--   0 runner    (1001) docker     (123)     9206 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/target_platform_capabilities/target_platform/target_platform_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/target_platform_capabilities/target_platform/target_platform_model_component.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 00:04:47.753075 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/
--rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8759 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/attribute_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/current_tpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4019 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/layer_filter_params.py
--rw-r--r--   0 runner    (1001) docker     (123)     6040 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/operations_to_layers.py
--rw-r--r--   0 runner    (1001) docker     (123)     8713 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/target_platform_capabilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/target_platform_capabilities_component.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 00:04:47.753075 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 00:04:47.753075 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 00:04:47.753075 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/latest/
--rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/latest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4625 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/target_platform_capabilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 00:04:47.753075 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v1/
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6310 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v1/tp_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3845 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v1/tpc_keras.py
--rw-r--r--   0 runner    (1001) docker     (123)     3261 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v1/tpc_pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 00:04:47.753075 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v2/
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6846 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v2/tp_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4321 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v2/tpc_keras.py
--rw-r--r--   0 runner    (1001) docker     (123)     3859 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v2/tpc_pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 00:04:47.753075 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v3/
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8148 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v3/tp_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4618 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v3/tpc_keras.py
--rw-r--r--   0 runner    (1001) docker     (123)     4196 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v3/tpc_pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 00:04:47.753075 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v3_lut/
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v3_lut/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8332 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v3_lut/tp_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4631 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v3_lut/tpc_keras.py
--rw-r--r--   0 runner    (1001) docker     (123)     4209 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v3_lut/tpc_pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 00:04:47.753075 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v4/
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v4/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8148 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v4/tp_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     5372 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v4/tpc_keras.py
--rw-r--r--   0 runner    (1001) docker     (123)     4714 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v4/tpc_pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 00:04:47.753075 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v4_lut/
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v4_lut/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8332 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v4_lut/tp_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     5477 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v4_lut/tpc_keras.py
--rw-r--r--   0 runner    (1001) docker     (123)     4727 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v4_lut/tpc_pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 00:04:47.753075 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v5/
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v5/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8145 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v5/tp_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     5373 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v5/tpc_keras.py
--rw-r--r--   0 runner    (1001) docker     (123)     4714 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v5/tpc_pytorch.py
--rw-r--r--   0 runner    (1001) docker     (123)     3526 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/get_target_platform_capabilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 00:04:47.753075 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 00:04:47.753075 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/latest/
--rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/latest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/target_platform_capabilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 00:04:47.753075 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8140 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/tp_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     5379 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/tpc_keras.py
--rw-r--r--   0 runner    (1001) docker     (123)     4721 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/tpc_pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 00:04:47.753075 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 00:04:47.753075 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/latest/
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/latest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/target_platform_capabilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 00:04:47.757074 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6204 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/tp_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3198 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/tpc_keras.py
--rw-r--r--   0 runner    (1001) docker     (123)     2942 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/tpc_pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 00:04:47.757074 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 00:04:47.757074 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/latest/
--rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/latest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2085 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/target_platform_capabilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 00:04:47.757074 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8048 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/tp_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     6131 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/tpc_keras.py
--rw-r--r--   0 runner    (1001) docker     (123)     5002 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/tpc_pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 00:04:47.757074 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/trainable_infrastructure/
--rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/trainable_infrastructure/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 00:04:47.757074 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/trainable_infrastructure/common/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/trainable_infrastructure/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7564 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/trainable_infrastructure/common/base_trainable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)      875 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/trainable_infrastructure/common/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     6351 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/trainable_infrastructure/common/get_quantizer_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3558 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/trainable_infrastructure/common/get_quantizers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/trainable_infrastructure/common/quant_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4791 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/trainable_infrastructure/common/trainable_quantizer_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 00:04:47.757074 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/trainable_infrastructure/keras/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/trainable_infrastructure/keras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4212 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/trainable_infrastructure/keras/base_keras_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3991 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/trainable_infrastructure/keras/config_serialization.py
--rw-r--r--   0 runner    (1001) docker     (123)     3480 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/trainable_infrastructure/keras/load_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/trainable_infrastructure/keras/quantizer_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 00:04:47.757074 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/trainable_infrastructure/pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/trainable_infrastructure/pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3083 2023-07-06 00:04:03.000000 mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/trainable_infrastructure/pytorch/base_pytorch_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-06 00:04:47.757074 mct-nightly-1.9.0.20230706.post446/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-07-06 00:04:46.000000 mct-nightly-1.9.0.20230706.post446/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 00:04:47.048461 mct-nightly-1.9.0.20230707.post446/
+-rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11612 2023-07-07 00:04:47.052461 mct-nightly-1.9.0.20230707.post446/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9939 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 00:04:46.988461 mct-nightly-1.9.0.20230707.post446/mct_nightly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11612 2023-07-07 00:04:46.000000 mct-nightly-1.9.0.20230707.post446/mct_nightly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    32637 2023-07-07 00:04:46.000000 mct-nightly-1.9.0.20230707.post446/mct_nightly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 00:04:46.000000 mct-nightly-1.9.0.20230707.post446/mct_nightly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-07 00:04:46.000000 mct-nightly-1.9.0.20230707.post446/mct_nightly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-07 00:04:46.000000 mct-nightly-1.9.0.20230707.post446/mct_nightly.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 00:04:46.988461 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/
+-rw-r--r--   0 runner    (1001) docker     (123)     3608 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3890 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 00:04:46.992461 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2975 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/analyzer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 00:04:46.992461 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/
+-rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 00:04:46.992461 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/back2framework/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/back2framework/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/back2framework/base_model_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/base_substitutions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 00:04:46.992461 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/collectors/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/collectors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2576 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/collectors/base_collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6864 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/collectors/histogram_collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3888 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/collectors/mean_collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5207 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/collectors/min_max_per_channel_collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7929 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/collectors/statistics_collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/collectors/statistics_collector_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4017 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/data_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2281 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/defaultdict.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21343 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/framework_implementation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6424 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/framework_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 00:04:46.992461 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/fusion/
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/fusion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5479 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/fusion/layer_fusing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 00:04:46.996461 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/graph/
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28860 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/graph/base_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20579 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/graph/base_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3733 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/graph/edge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/graph/functional_node.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4732 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/graph/graph_matchers.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5128 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/graph/graph_searches.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 00:04:46.996461 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/graph/memory_graph/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/graph/memory_graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3880 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/graph/memory_graph/bipartite_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2612 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/graph/memory_graph/compute_graph_max_cut.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2470 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/graph/memory_graph/cut.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17045 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/graph/memory_graph/max_cut_astar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3961 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/graph/memory_graph/memory_element.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7175 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/graph/memory_graph/memory_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9265 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/graph/virtual_activation_weights_node.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 00:04:46.996461 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/matchers/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      697 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/matchers/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3091 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/matchers/base_graph_filter.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2210 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/matchers/base_matcher.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3706 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/matchers/edge_matcher.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1773 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/matchers/function.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2745 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/matchers/node_matcher.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1111 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/matchers/walk_matcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/memory_computation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 00:04:47.000461 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/mixed_precision/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/mixed_precision/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6704 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/mixed_precision/bit_width_setter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/mixed_precision/configurable_quant_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3871 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/mixed_precision/configurable_quantizer_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/mixed_precision/distance_weighting.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 00:04:47.000461 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/mixed_precision/kpi_tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/mixed_precision/kpi_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4297 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/mixed_precision/kpi_tools/kpi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3920 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/mixed_precision/kpi_tools/kpi_aggregation_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7046 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/mixed_precision/kpi_tools/kpi_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/mixed_precision/kpi_tools/kpi_functions_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19323 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/mixed_precision/kpi_tools/kpi_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8041 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/mixed_precision/mixed_precision_quantization_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6822 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/mixed_precision/mixed_precision_search_facade.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34622 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/mixed_precision/mixed_precision_search_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 00:04:47.000461 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/mixed_precision/search_methods/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/mixed_precision/search_methods/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15453 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/mixed_precision/search_methods/linear_programming.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24909 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/mixed_precision/sensitivity_evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2846 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/mixed_precision/set_layer_to_bitwidth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6326 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/mixed_precision/solution_refinement_procedure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/model_builder_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5005 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/model_collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/model_validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 00:04:47.000461 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/network_editors/
+-rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/network_editors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17994 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/network_editors/actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/network_editors/edit_network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3149 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/network_editors/node_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/node_prior_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 00:04:47.004461 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/quantization/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/quantization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3022 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/quantization/candidate_node_quantization_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/quantization/core_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/quantization/debug_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6137 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/quantization/filter_nodes_candidates.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16271 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/quantization/node_quantization_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/quantization/quantization_analyzer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7247 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/quantization/quantization_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/quantization/quantization_fn_selection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4090 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/quantization/quantization_params_fn_selection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 00:04:47.004461 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/quantization/quantization_params_generation/
+-rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/quantization/quantization_params_generation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16505 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/quantization/quantization_params_generation/error_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2927 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/quantization/quantization_params_generation/kmeans_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7292 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/quantization/quantization_params_generation/lut_kmeans_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/quantization/quantization_params_generation/outlier_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8484 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/quantization/quantization_params_generation/power_of_two_selection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4558 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/quantization/quantization_params_generation/qparams_activations_computation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4315 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/quantization/quantization_params_generation/qparams_computation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41685 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/quantization/quantization_params_generation/qparams_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5090 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/quantization/quantization_params_generation/qparams_weights_computation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9689 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/quantization/quantization_params_generation/symmetric_selection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7879 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/quantization/quantization_params_generation/uniform_selection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2939 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/quantization/quantize_graph_weights.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3614 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/quantization/quantize_node.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 00:04:47.004461 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/quantization/quantizers/
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/quantization/quantizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/quantization/quantizers/kmeans_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2774 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/quantization/quantizers/lut_kmeans_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14210 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/quantization/quantizers/quantizers_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5486 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/quantization/quantizers/uniform_quantizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10683 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/quantization/set_node_quantization_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7450 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/similarity_analyzer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 00:04:47.004461 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/statistics_correction/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/statistics_correction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3434 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/statistics_correction/apply_bias_correction_to_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5956 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/statistics_correction/apply_second_moment_correction_to_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10228 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/statistics_correction/compute_bias_correction_of_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5584 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/statistics_correction/statistics_correction.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 00:04:47.008461 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/substitutions/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/substitutions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/substitutions/apply_substitutions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12692 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/substitutions/batchnorm_folding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5892 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/substitutions/batchnorm_reconstruction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9962 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/substitutions/batchnorm_refusing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9093 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/substitutions/linear_collapsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/substitutions/linear_collapsing_substitution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4866 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/substitutions/residual_collapsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10978 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/substitutions/scale_equalization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26835 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/substitutions/shift_negative_activation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/substitutions/softmax_shift.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3400 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/substitutions/virtual_activation_weights_composition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4228 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/substitutions/weights_activation_split.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/user_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 00:04:47.008461 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/visualization/
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/visualization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6371 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/visualization/final_config_visualizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5955 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/visualization/nn_visualizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20099 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/visualization/tensorboard_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4233 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/exporter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 00:04:47.008461 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/keras/
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/keras/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 00:04:47.012461 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/keras/back2framework/
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/keras/back2framework/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/keras/back2framework/factory_model_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2444 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/keras/back2framework/float_model_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4508 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/keras/back2framework/instance_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16109 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/keras/back2framework/keras_model_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14442 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/keras/back2framework/mixed_precision_model_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15316 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/keras/back2framework/model_gradients.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2481 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/keras/back2framework/quantized_model_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2664 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/keras/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4999 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/keras/default_framework_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 00:04:47.012461 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/keras/graph_substitutions/
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/keras/graph_substitutions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 00:04:47.012461 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/keras/graph_substitutions/substitutions/
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/keras/graph_substitutions/substitutions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3940 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/keras/graph_substitutions/substitutions/activation_decomposition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7317 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/keras/graph_substitutions/substitutions/batchnorm_folding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3168 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/keras/graph_substitutions/substitutions/batchnorm_reconstruction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2478 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/keras/graph_substitutions/substitutions/batchnorm_refusing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5598 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/keras/graph_substitutions/substitutions/input_scaling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5925 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/keras/graph_substitutions/substitutions/linear_collapsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26778 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/keras/graph_substitutions/substitutions/multi_head_attention_decomposition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3872 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/keras/graph_substitutions/substitutions/relu_bound_to_power_of_2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2387 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/keras/graph_substitutions/substitutions/remove_relu_upper_bound.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/keras/graph_substitutions/substitutions/residual_collapsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5542 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/keras/graph_substitutions/substitutions/scale_equalization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7714 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/keras/graph_substitutions/substitutions/separableconv_decomposition.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10781 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/keras/graph_substitutions/substitutions/shift_negative_activation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/keras/graph_substitutions/substitutions/softmax_shift.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/keras/graph_substitutions/substitutions/virtual_activation_weights_composition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/keras/graph_substitutions/substitutions/weights_activation_split.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27296 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/keras/keras_implementation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/keras/keras_model_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3941 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/keras/keras_node_prior_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8600 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/keras/kpi_data_facade.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 00:04:47.012461 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/keras/mixed_precision/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/keras/mixed_precision/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4926 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/keras/mixed_precision/configurable_activation_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6367 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/keras/mixed_precision/configurable_weights_quantizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 00:04:47.016461 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/keras/quantizer/
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/keras/quantizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/keras/quantizer/base_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6151 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/keras/quantizer/fake_quant_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4507 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/keras/quantizer/lut_fake_quant.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 00:04:47.016461 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/keras/reader/
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/keras/reader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2627 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/keras/reader/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11418 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/keras/reader/connectivity_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 00:04:47.016461 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/keras/reader/nested_model/
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/keras/reader/nested_model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7906 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/keras/reader/nested_model/edges_merger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2760 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/keras/reader/nested_model/nested_model_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/keras/reader/nested_model/nodes_merger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/keras/reader/nested_model/outputs_merger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5951 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/keras/reader/node_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8109 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/keras/reader/reader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 00:04:47.016461 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/keras/statistics_correction/
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/keras/statistics_correction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/keras/statistics_correction/apply_second_moment_correction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/keras/tf_tensor_numpy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 00:04:47.016461 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/keras/visualization/
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/keras/visualization/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 00:04:47.016461 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/pytorch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 00:04:47.020461 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/pytorch/back2framework/
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/pytorch/back2framework/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2274 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/pytorch/back2framework/factory_model_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3419 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/pytorch/back2framework/float_model_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/pytorch/back2framework/instance_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14033 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/pytorch/back2framework/mixed_precision_model_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18214 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/pytorch/back2framework/model_gradients.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16443 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/pytorch/back2framework/pytorch_model_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 00:04:47.020461 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/pytorch/back2framework/quantization_wrapper/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/pytorch/back2framework/quantization_wrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5773 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/pytorch/back2framework/quantization_wrapper/quantized_layer_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/pytorch/back2framework/quantization_wrapper/wrapper_quantize_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3456 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/pytorch/back2framework/quantized_model_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/pytorch/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4224 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/pytorch/default_framework_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 00:04:47.020461 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/pytorch/graph_substitutions/
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/pytorch/graph_substitutions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 00:04:47.020461 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6840 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/batchnorm_folding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/batchnorm_reconstruction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/batchnorm_refusing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4804 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/const_holder_conv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5797 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/linear_collapsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38353 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/multi_head_attention_decomposition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/permute_call_method.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5601 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/relu_bound_to_power_of_2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4148 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/reshape_with_static_shapes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2899 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/residual_collapsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3303 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/scale_equalization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9838 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/shift_negative_activation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/softmax_shift.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/virtual_activation_weights_composition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/weights_activation_split.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8482 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/pytorch/kpi_data_facade.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 00:04:47.020461 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/pytorch/mixed_precision/
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/pytorch/mixed_precision/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4660 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/pytorch/mixed_precision/configurable_activation_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5965 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/pytorch/mixed_precision/configurable_weights_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25782 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/pytorch/pytorch_implementation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3250 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/pytorch/pytorch_node_prior_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 00:04:47.024461 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/pytorch/quantizer/
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/pytorch/quantizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6464 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/pytorch/quantizer/fake_quant_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4452 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/pytorch/quantizer/lut_fake_quant.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 00:04:47.024461 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/pytorch/reader/
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/pytorch/reader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12113 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/pytorch/reader/graph_builders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/pytorch/reader/node_holders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5801 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/pytorch/reader/reader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 00:04:47.024461 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/pytorch/statistics_correction/
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/pytorch/statistics_correction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3261 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/pytorch/statistics_correction/apply_second_moment_correction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2959 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/pytorch/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23009 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 00:04:47.024461 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/exporter/
+-rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/exporter/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 00:04:47.024461 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/exporter/model_exporter/
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/exporter/model_exporter/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 00:04:47.024461 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/exporter/model_exporter/fw_agonstic/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/exporter/model_exporter/fw_agonstic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/exporter/model_exporter/fw_agonstic/exporter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 00:04:47.024461 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/exporter/model_exporter/keras/
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/exporter/model_exporter/keras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/exporter/model_exporter/keras/base_keras_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/exporter/model_exporter/keras/export_serialization_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11100 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/exporter/model_exporter/keras/fakely_quant_keras_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3043 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/exporter/model_exporter/keras/fakely_quant_tflite_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8048 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/exporter/model_exporter/keras/int8_tflite_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6016 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/exporter/model_exporter/keras/keras_export_facade.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 00:04:47.024461 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/exporter/model_exporter/pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/exporter/model_exporter/pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4020 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/exporter/model_exporter/pytorch/base_pytorch_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/exporter/model_exporter/pytorch/export_serialization_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3298 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/exporter/model_exporter/pytorch/fakely_quant_onnx_pytorch_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/exporter/model_exporter/pytorch/fakely_quant_torchscript_pytorch_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5866 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/exporter/model_exporter/pytorch/pytorch_export_facade.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 00:04:47.024461 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/exporter/model_wrapper/
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/exporter/model_wrapper/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 00:04:47.028461 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/exporter/model_wrapper/keras/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/exporter/model_wrapper/keras/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 00:04:47.028461 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/exporter/model_wrapper/keras/builder/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/exporter/model_wrapper/keras/builder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4287 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/exporter/model_wrapper/keras/builder/fully_quantized_model_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8764 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/exporter/model_wrapper/keras/builder/node_to_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/exporter/model_wrapper/keras/builder/node_to_quantizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3543 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/exporter/model_wrapper/keras/validate_layer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 00:04:47.028461 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/exporter/model_wrapper/pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/exporter/model_wrapper/pytorch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 00:04:47.028461 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/exporter/model_wrapper/pytorch/builder/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/exporter/model_wrapper/pytorch/builder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3921 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/exporter/model_wrapper/pytorch/builder/fully_quantized_model_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8656 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/exporter/model_wrapper/pytorch/builder/node_to_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/exporter/model_wrapper/pytorch/builder/node_to_quantizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3449 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/exporter/model_wrapper/pytorch/validate_layer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 00:04:47.028461 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/gptq/
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/gptq/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 00:04:47.028461 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/gptq/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/gptq/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9508 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/gptq/common/gptq_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/gptq/common/gptq_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/gptq/common/gptq_framework_implementation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2826 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/gptq/common/gptq_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15167 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/gptq/common/gptq_training.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 00:04:47.028461 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/gptq/keras/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/gptq/keras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/gptq/keras/gptq_keras_implementation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6241 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/gptq/keras/gptq_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17319 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/gptq/keras/gptq_training.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4564 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/gptq/keras/graph_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14791 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/gptq/keras/quantization_facade.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 00:04:47.032461 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/gptq/keras/quantizer/
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/gptq/keras/quantizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4751 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/gptq/keras/quantizer/base_keras_gptq_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5055 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/gptq/keras/quantizer/quant_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4431 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/gptq/keras/quantizer/quantization_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/gptq/keras/quantizer/regularization_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 00:04:47.032461 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3962 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/soft_quantizer_reg.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12163 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/symmetric_soft_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10381 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/uniform_soft_quantizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 00:04:47.032461 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/gptq/keras/quantizer/ste_rounding/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/gptq/keras/quantizer/ste_rounding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8370 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/gptq/keras/quantizer/ste_rounding/symmetric_ste.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 00:04:47.032461 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/gptq/pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/gptq/pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/gptq/pytorch/gptq_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/gptq/pytorch/gptq_pytorch_implementation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14668 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/gptq/pytorch/gptq_training.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3955 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/gptq/pytorch/graph_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12768 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/gptq/pytorch/quantization_facade.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 00:04:47.032461 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/gptq/pytorch/quantizer/
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/gptq/pytorch/quantizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4171 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/gptq/pytorch/quantizer/base_pytorch_gptq_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3893 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/gptq/pytorch/quantizer/quant_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4291 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/gptq/pytorch/quantizer/quantization_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/gptq/pytorch/quantizer/regularization_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 00:04:47.032461 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4132 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/soft_quantizer_reg.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12351 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/symmetric_soft_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9103 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/uniform_soft_quantizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 00:04:47.032461 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/gptq/pytorch/quantizer/ste_rounding/
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/gptq/pytorch/quantizer/ste_rounding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8782 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/gptq/pytorch/quantizer/ste_rounding/symmetric_ste.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5534 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/gptq/runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 00:04:47.032461 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/legacy/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/legacy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18116 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/legacy/keras_quantization_facade.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17664 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/legacy/pytorch_quantization_facade.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4863 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 00:04:47.036461 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/ptq/
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/ptq/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 00:04:47.036461 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/ptq/keras/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/ptq/keras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9868 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/ptq/keras/quantization_facade.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 00:04:47.036461 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/ptq/pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/ptq/pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8580 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/ptq/pytorch/quantization_facade.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/ptq/runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 00:04:47.036461 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/qat/
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/qat/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 00:04:47.036461 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/qat/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/qat/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3295 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/qat/common/qat_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 00:04:47.036461 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/qat/keras/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/qat/keras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16051 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/qat/keras/quantization_facade.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 00:04:47.036461 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/qat/keras/quantizer/
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/qat/keras/quantizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/qat/keras/quantizer/base_keras_qat_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/qat/keras/quantizer/quant_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5635 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/qat/keras/quantizer/quantization_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 00:04:47.036461 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/qat/keras/quantizer/ste_rounding/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/qat/keras/quantizer/ste_rounding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13436 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/qat/keras/quantizer/ste_rounding/symmetric_ste.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10708 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/qat/keras/quantizer/ste_rounding/uniform_ste.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 00:04:47.036461 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/qat/pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/qat/pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12461 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/qat/pytorch/quantization_facade.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 00:04:47.036461 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/qat/pytorch/quantizer/
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/qat/pytorch/quantizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/qat/pytorch/quantizer/base_pytorch_qat_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5491 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/qat/pytorch/quantizer/quantization_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5004 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/qat/pytorch/quantizer/quantizer_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 00:04:47.036461 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/qat/pytorch/quantizer/ste_rounding/
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/qat/pytorch/quantizer/ste_rounding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9629 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/qat/pytorch/quantizer/ste_rounding/symmetric_ste.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8651 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/qat/pytorch/quantizer/ste_rounding/uniform_ste.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 00:04:47.040461 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/target_platform_capabilities/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/target_platform_capabilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/target_platform_capabilities/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/target_platform_capabilities/immutable.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 00:04:47.040461 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/target_platform_capabilities/target_platform/
+-rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/target_platform_capabilities/target_platform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/target_platform_capabilities/target_platform/current_tp_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/target_platform_capabilities/target_platform/fusing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8538 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/target_platform_capabilities/target_platform/op_quantization_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/target_platform_capabilities/target_platform/operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/target_platform_capabilities/target_platform/quantization_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9206 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/target_platform_capabilities/target_platform/target_platform_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/target_platform_capabilities/target_platform/target_platform_model_component.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 00:04:47.040461 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/
+-rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8759 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/attribute_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/current_tpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4019 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/layer_filter_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6040 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/operations_to_layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8713 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/target_platform_capabilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/target_platform_capabilities_component.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 00:04:47.040461 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 00:04:47.040461 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 00:04:47.040461 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/latest/
+-rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/latest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4625 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/target_platform_capabilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 00:04:47.040461 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6310 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v1/tp_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3845 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v1/tpc_keras.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3261 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v1/tpc_pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 00:04:47.044461 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v2/
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6846 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v2/tp_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4321 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v2/tpc_keras.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3859 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v2/tpc_pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 00:04:47.044461 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v3/
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8148 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v3/tp_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4618 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v3/tpc_keras.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4196 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v3/tpc_pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 00:04:47.044461 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v3_lut/
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v3_lut/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8332 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v3_lut/tp_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4631 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v3_lut/tpc_keras.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4209 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v3_lut/tpc_pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 00:04:47.044461 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v4/
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v4/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8148 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v4/tp_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5372 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v4/tpc_keras.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4714 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v4/tpc_pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 00:04:47.044461 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v4_lut/
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v4_lut/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8332 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v4_lut/tp_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5477 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v4_lut/tpc_keras.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4727 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v4_lut/tpc_pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 00:04:47.044461 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v5/
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v5/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8145 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v5/tp_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5373 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v5/tpc_keras.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4714 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v5/tpc_pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3526 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/get_target_platform_capabilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 00:04:47.044461 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 00:04:47.044461 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/latest/
+-rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/latest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/target_platform_capabilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 00:04:47.044461 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8140 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/tp_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5379 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/tpc_keras.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4721 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/tpc_pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 00:04:47.048461 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 00:04:47.048461 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/latest/
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/latest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/target_platform_capabilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 00:04:47.048461 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6204 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/tp_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3198 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/tpc_keras.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2942 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/tpc_pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 00:04:47.048461 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 00:04:47.048461 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/latest/
+-rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/latest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2085 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/target_platform_capabilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 00:04:47.048461 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8048 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/tp_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6131 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/tpc_keras.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5002 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/tpc_pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 00:04:47.048461 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/trainable_infrastructure/
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/trainable_infrastructure/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 00:04:47.048461 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/trainable_infrastructure/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/trainable_infrastructure/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7564 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/trainable_infrastructure/common/base_trainable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/trainable_infrastructure/common/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6351 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/trainable_infrastructure/common/get_quantizer_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3558 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/trainable_infrastructure/common/get_quantizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/trainable_infrastructure/common/quant_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4791 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/trainable_infrastructure/common/trainable_quantizer_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 00:04:47.048461 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/trainable_infrastructure/keras/
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/trainable_infrastructure/keras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4212 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/trainable_infrastructure/keras/base_keras_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3991 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/trainable_infrastructure/keras/config_serialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3480 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/trainable_infrastructure/keras/load_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/trainable_infrastructure/keras/quantizer_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 00:04:47.048461 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/trainable_infrastructure/pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/trainable_infrastructure/pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3083 2023-07-07 00:04:07.000000 mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/trainable_infrastructure/pytorch/base_pytorch_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-07 00:04:47.052461 mct-nightly-1.9.0.20230707.post446/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-07-07 00:04:46.000000 mct-nightly-1.9.0.20230707.post446/setup.py
```

### Comparing `mct-nightly-1.9.0.20230706.post446/LICENSE.md` & `mct-nightly-1.9.0.20230707.post446/LICENSE.md`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/PKG-INFO` & `mct-nightly-1.9.0.20230707.post446/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mct-nightly
-Version: 1.9.0.20230706.post446
+Version: 1.9.0.20230707.post446
 Summary: A Model Compression Toolkit for neural networks
 Home-page: UNKNOWN
 License: UNKNOWN
 Description: # Model Compression Toolkit (MCT)
         
         Model Compression Toolkit (MCT) is an open-source project for neural network model optimization under efficient, constrained hardware.
         
@@ -125,18 +125,18 @@
         For more results, please see [1]
         
         ### Pytorch
         We quantized classification networks from the torchvision library. 
         In the following table we present the ImageNet validation results for these models:
         
         | Network Name              | Float Accuracy  | 8Bit Accuracy   | 
-        | --------------------------| ---------------:| ---------------:| 
-        | MobileNet V2 [3]          | 71.886          | 71.444           |                                      
-        | ResNet-18 [3]             | 69.86           | 69.63           |                                      
-        | SqueezeNet 1.1 [3]        | 58.128          | 57.678          |                                      
+        |---------------------------|-----------------|-----------------| 
+        | MobileNet V2 [3]          | 71.886          | 71.444          |
+        | ResNet-18 [3]             | 69.86           | 69.63           |
+        | SqueezeNet 1.1 [3]        | 58.128          | 57.678          |
         
         For more results, please refer to [quick start](https://github.com/sony/model_optimization/tree/main/tutorials/quick_start).
         
         ## Contributions
         MCT aims at keeping a more up-to-date fork and welcomes contributions from anyone.
         
         *You will find more information about contributions in the [Contribution guide](CONTRIBUTING.md).
```

### Comparing `mct-nightly-1.9.0.20230706.post446/README.md` & `mct-nightly-1.9.0.20230707.post446/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -119,18 +119,18 @@
 For more results, please see [1]
 
 ### Pytorch
 We quantized classification networks from the torchvision library. 
 In the following table we present the ImageNet validation results for these models:
 
 | Network Name              | Float Accuracy  | 8Bit Accuracy   | 
-| --------------------------| ---------------:| ---------------:| 
-| MobileNet V2 [3]          | 71.886          | 71.444           |                                      
-| ResNet-18 [3]             | 69.86           | 69.63           |                                      
-| SqueezeNet 1.1 [3]        | 58.128          | 57.678          |                                      
+|---------------------------|-----------------|-----------------| 
+| MobileNet V2 [3]          | 71.886          | 71.444          |
+| ResNet-18 [3]             | 69.86           | 69.63           |
+| SqueezeNet 1.1 [3]        | 58.128          | 57.678          |
 
 For more results, please refer to [quick start](https://github.com/sony/model_optimization/tree/main/tutorials/quick_start).
 
 ## Contributions
 MCT aims at keeping a more up-to-date fork and welcomes contributions from anyone.
 
 *You will find more information about contributions in the [Contribution guide](CONTRIBUTING.md).
```

### Comparing `mct-nightly-1.9.0.20230706.post446/mct_nightly.egg-info/PKG-INFO` & `mct-nightly-1.9.0.20230707.post446/mct_nightly.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mct-nightly
-Version: 1.9.0.20230706.post446
+Version: 1.9.0.20230707.post446
 Summary: A Model Compression Toolkit for neural networks
 Home-page: UNKNOWN
 License: UNKNOWN
 Description: # Model Compression Toolkit (MCT)
         
         Model Compression Toolkit (MCT) is an open-source project for neural network model optimization under efficient, constrained hardware.
         
@@ -125,18 +125,18 @@
         For more results, please see [1]
         
         ### Pytorch
         We quantized classification networks from the torchvision library. 
         In the following table we present the ImageNet validation results for these models:
         
         | Network Name              | Float Accuracy  | 8Bit Accuracy   | 
-        | --------------------------| ---------------:| ---------------:| 
-        | MobileNet V2 [3]          | 71.886          | 71.444           |                                      
-        | ResNet-18 [3]             | 69.86           | 69.63           |                                      
-        | SqueezeNet 1.1 [3]        | 58.128          | 57.678          |                                      
+        |---------------------------|-----------------|-----------------| 
+        | MobileNet V2 [3]          | 71.886          | 71.444          |
+        | ResNet-18 [3]             | 69.86           | 69.63           |
+        | SqueezeNet 1.1 [3]        | 58.128          | 57.678          |
         
         For more results, please refer to [quick start](https://github.com/sony/model_optimization/tree/main/tutorials/quick_start).
         
         ## Contributions
         MCT aims at keeping a more up-to-date fork and welcomes contributions from anyone.
         
         *You will find more information about contributions in the [Contribution guide](CONTRIBUTING.md).
```

### Comparing `mct-nightly-1.9.0.20230706.post446/mct_nightly.egg-info/SOURCES.txt` & `mct-nightly-1.9.0.20230707.post446/mct_nightly.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -58,19 +58,22 @@
 model_compression_toolkit/core/common/matchers/base_matcher.py
 model_compression_toolkit/core/common/matchers/edge_matcher.py
 model_compression_toolkit/core/common/matchers/function.py
 model_compression_toolkit/core/common/matchers/node_matcher.py
 model_compression_toolkit/core/common/matchers/walk_matcher.py
 model_compression_toolkit/core/common/mixed_precision/__init__.py
 model_compression_toolkit/core/common/mixed_precision/bit_width_setter.py
+model_compression_toolkit/core/common/mixed_precision/configurable_quant_id.py
+model_compression_toolkit/core/common/mixed_precision/configurable_quantizer_utils.py
 model_compression_toolkit/core/common/mixed_precision/distance_weighting.py
 model_compression_toolkit/core/common/mixed_precision/mixed_precision_quantization_config.py
 model_compression_toolkit/core/common/mixed_precision/mixed_precision_search_facade.py
 model_compression_toolkit/core/common/mixed_precision/mixed_precision_search_manager.py
 model_compression_toolkit/core/common/mixed_precision/sensitivity_evaluation.py
+model_compression_toolkit/core/common/mixed_precision/set_layer_to_bitwidth.py
 model_compression_toolkit/core/common/mixed_precision/solution_refinement_procedure.py
 model_compression_toolkit/core/common/mixed_precision/kpi_tools/__init__.py
 model_compression_toolkit/core/common/mixed_precision/kpi_tools/kpi.py
 model_compression_toolkit/core/common/mixed_precision/kpi_tools/kpi_aggregation_methods.py
 model_compression_toolkit/core/common/mixed_precision/kpi_tools/kpi_data.py
 model_compression_toolkit/core/common/mixed_precision/kpi_tools/kpi_functions_mapping.py
 model_compression_toolkit/core/common/mixed_precision/kpi_tools/kpi_methods.py
@@ -163,25 +166,20 @@
 model_compression_toolkit/core/keras/graph_substitutions/substitutions/scale_equalization.py
 model_compression_toolkit/core/keras/graph_substitutions/substitutions/separableconv_decomposition.py
 model_compression_toolkit/core/keras/graph_substitutions/substitutions/shift_negative_activation.py
 model_compression_toolkit/core/keras/graph_substitutions/substitutions/softmax_shift.py
 model_compression_toolkit/core/keras/graph_substitutions/substitutions/virtual_activation_weights_composition.py
 model_compression_toolkit/core/keras/graph_substitutions/substitutions/weights_activation_split.py
 model_compression_toolkit/core/keras/mixed_precision/__init__.py
-model_compression_toolkit/core/keras/mixed_precision/set_layer_to_bitwidth.py
+model_compression_toolkit/core/keras/mixed_precision/configurable_activation_quantizer.py
+model_compression_toolkit/core/keras/mixed_precision/configurable_weights_quantizer.py
 model_compression_toolkit/core/keras/quantizer/__init__.py
 model_compression_toolkit/core/keras/quantizer/base_quantizer.py
 model_compression_toolkit/core/keras/quantizer/fake_quant_builder.py
-model_compression_toolkit/core/keras/quantizer/input_layer_quantize_transform.py
 model_compression_toolkit/core/keras/quantizer/lut_fake_quant.py
-model_compression_toolkit/core/keras/quantizer/mixed_precision/__init__.py
-model_compression_toolkit/core/keras/quantizer/mixed_precision/quantization_config_factory.py
-model_compression_toolkit/core/keras/quantizer/mixed_precision/selective_activation_quantizer.py
-model_compression_toolkit/core/keras/quantizer/mixed_precision/selective_quantize_config.py
-model_compression_toolkit/core/keras/quantizer/mixed_precision/selective_weights_quantizer.py
 model_compression_toolkit/core/keras/reader/__init__.py
 model_compression_toolkit/core/keras/reader/common.py
 model_compression_toolkit/core/keras/reader/connectivity_handler.py
 model_compression_toolkit/core/keras/reader/node_builder.py
 model_compression_toolkit/core/keras/reader/reader.py
 model_compression_toolkit/core/keras/reader/nested_model/__init__.py
 model_compression_toolkit/core/keras/reader/nested_model/edges_merger.py
@@ -223,16 +221,16 @@
 model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/residual_collapsing.py
 model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/scale_equalization.py
 model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/shift_negative_activation.py
 model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/softmax_shift.py
 model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/virtual_activation_weights_composition.py
 model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/weights_activation_split.py
 model_compression_toolkit/core/pytorch/mixed_precision/__init__.py
-model_compression_toolkit/core/pytorch/mixed_precision/mixed_precision_wrapper.py
-model_compression_toolkit/core/pytorch/mixed_precision/set_layer_to_bitwidth.py
+model_compression_toolkit/core/pytorch/mixed_precision/configurable_activation_quantizer.py
+model_compression_toolkit/core/pytorch/mixed_precision/configurable_weights_quantizer.py
 model_compression_toolkit/core/pytorch/quantizer/__init__.py
 model_compression_toolkit/core/pytorch/quantizer/fake_quant_builder.py
 model_compression_toolkit/core/pytorch/quantizer/lut_fake_quant.py
 model_compression_toolkit/core/pytorch/reader/__init__.py
 model_compression_toolkit/core/pytorch/reader/graph_builders.py
 model_compression_toolkit/core/pytorch/reader/node_holders.py
 model_compression_toolkit/core/pytorch/reader/reader.py
```

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/__init__.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/constants.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/constants.py`

 * *Files 3% similar despite different names*

```diff
@@ -113,14 +113,10 @@
 WEIGHTS_QUANT_PARAMS_FN = 'weights_quantization_params_fn'
 WEIGHTS_CHANNELS_AXIS = 'weights_channels_axis'
 
 # Memory graph constants
 DUMMY_NODE = 'dummy_node'
 DUMMY_TENSOR = 'dummy_tensor'
 
-
-# TF Input node base name
-INPUT_BASE_NAME = 'base_input'
-
 # Jacobian-weights constants
 MIN_JACOBIANS_ITER = 10
 JACOBIANS_COMP_TOLERANCE = 1e-3
```

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/__init__.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/analyzer.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/analyzer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/__init__.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/back2framework/__init__.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/back2framework/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/back2framework/base_model_builder.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/back2framework/base_model_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/base_substitutions.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/base_substitutions.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/collectors/__init__.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/collectors/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/collectors/base_collector.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/collectors/base_collector.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/collectors/histogram_collector.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/collectors/histogram_collector.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/collectors/mean_collector.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/collectors/mean_collector.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/collectors/min_max_per_channel_collector.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/collectors/min_max_per_channel_collector.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/collectors/statistics_collector.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/collectors/statistics_collector.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/collectors/statistics_collector_generator.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/collectors/statistics_collector_generator.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/data_loader.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/data_loader.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/defaultdict.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/defaultdict.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/framework_implementation.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/framework_implementation.py`

 * *Files 4% similar despite different names*

```diff
@@ -90,29 +90,29 @@
 
     @abstractmethod
     def model_builder(self,
                       graph: Graph,
                       mode: ModelBuilderMode,
                       append2output: List[Any],
                       fw_info: FrameworkInfo,
-                      return_float_outputs: bool = False) -> Tuple[Any, UserInformation]:
+                      return_float_outputs: bool = False) -> Tuple:
         """
         Build a framework model from a graph.
         The mode determines how the model should be build. append2output is a list of Nodes
         to set as the model outputs.
 
         Args:
             graph: Graph to build the model from it.
             mode: Mode for how to build the model.
             append2output: List of Nodes to set as the model's outputs.
             fw_info: FrameworkInfo object with information about the specific framework's model
             return_float_outputs (bool): whether to return outputs before or after quantization nodes (default)
 
         Returns:
-            A tuple of the model that was built and an UserInformation object.
+            A tuple with the model and additional relevant supporting objects.
         """
         raise NotImplemented(f'{self.__class__.__name__} have to implement the '
                              f'framework\'s model_builder method.')  # pragma: no cover
 
     @abstractmethod
     def run_model_inference(self,
                             model: Any,
@@ -284,15 +284,14 @@
         Returns:
             A list of the framework substitutions used after we apply second moment statistics.
         """
         raise NotImplemented(f'{self.__class__.__name__} have to implement the '
                              f'framework\'s get_substitutions_after_second_moment_correction '
                              f'method.')  # pragma: no cover
 
-
     @abstractmethod
     def get_sensitivity_evaluator(self,
                                   graph: Graph,
                                   quant_config: MixedPrecisionQuantizationConfigV2,
                                   representative_data_gen: Callable,
                                   fw_info: FrameworkInfo,
                                   disable_activation_for_metric: bool = False) -> SensitivityEvaluation:
@@ -359,48 +358,14 @@
         Returns: A distance function between two tensors.
         """
 
         raise NotImplemented(f'{self.__class__.__name__} have to implement the '
                              f'framework\'s get_node_distance_fn method.')  # pragma: no cover
 
     @abstractmethod
-    def get_model_layers_names(self,
-                               model: Any) -> List[str]:
-        """
-        Returns a list of the given model's layers names.
-
-        Args:
-            model: A model.
-
-        Returns: List of layers' names.
-
-        """
-
-        raise NotImplemented(f'{self.__class__.__name__} have to implement the '
-                             f'framework\'s get_model_layers_names method.')  # pragma: no cover
-
-    @abstractmethod
-    def get_model_layer_by_name(self,
-                                model: Any,
-                                layer_name: str) -> Any:
-        """
-        Returns a model's layer by its name.
-
-        Args:
-            model: A model to retrieve a layer from.
-            layer_name: The requested layer's name.
-
-        Returns: A layer object.
-
-        """
-
-        raise NotImplemented(f'{self.__class__.__name__} have to implement the '
-                             f'framework\'s get_model_layer_by_name method.')  # pragma: no cover
-
-    @abstractmethod
     def model_grad(self,
                    graph_float: common.Graph,
                    model_input_tensors: Dict[BaseNode, np.ndarray],
                    interest_points: List[BaseNode],
                    output_list: List[BaseNode],
                    all_outputs_indices: List[int],
                    alpha: float = 0.3,
```

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/framework_info.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/framework_info.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/fusion/__init__.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/fusion/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/fusion/layer_fusing.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/fusion/layer_fusing.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/graph/__init__.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/graph/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/graph/base_graph.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/graph/base_graph.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/graph/base_node.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/graph/base_node.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/graph/edge.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/graph/edge.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/graph/functional_node.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/graph/functional_node.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/graph/graph_matchers.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/graph/graph_matchers.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/graph/graph_searches.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/graph/graph_searches.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/graph/memory_graph/__init__.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/graph/memory_graph/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/graph/memory_graph/bipartite_graph.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/graph/memory_graph/bipartite_graph.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/graph/memory_graph/compute_graph_max_cut.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/graph/memory_graph/compute_graph_max_cut.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/graph/memory_graph/cut.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/graph/memory_graph/cut.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/graph/memory_graph/max_cut_astar.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/graph/memory_graph/max_cut_astar.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/graph/memory_graph/memory_element.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/graph/memory_graph/memory_element.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/graph/memory_graph/memory_graph.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/graph/memory_graph/memory_graph.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/graph/virtual_activation_weights_node.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/graph/virtual_activation_weights_node.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/matchers/__init__.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/matchers/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/matchers/base_graph_filter.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/matchers/base_graph_filter.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/matchers/base_matcher.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/matchers/base_matcher.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/matchers/edge_matcher.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/matchers/edge_matcher.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/matchers/function.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/matchers/function.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/matchers/node_matcher.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/matchers/node_matcher.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/matchers/walk_matcher.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/matchers/walk_matcher.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/memory_computation.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/memory_computation.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/mixed_precision/__init__.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/mixed_precision/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/mixed_precision/bit_width_setter.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/mixed_precision/bit_width_setter.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/mixed_precision/distance_weighting.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/mixed_precision/distance_weighting.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/mixed_precision/kpi_tools/__init__.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/mixed_precision/kpi_tools/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/mixed_precision/kpi_tools/kpi.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/mixed_precision/kpi_tools/kpi.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/mixed_precision/kpi_tools/kpi_aggregation_methods.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/mixed_precision/kpi_tools/kpi_aggregation_methods.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/mixed_precision/kpi_tools/kpi_data.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/mixed_precision/kpi_tools/kpi_data.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/mixed_precision/kpi_tools/kpi_functions_mapping.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/mixed_precision/kpi_tools/kpi_functions_mapping.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/mixed_precision/kpi_tools/kpi_methods.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/mixed_precision/kpi_tools/kpi_methods.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/mixed_precision/mixed_precision_quantization_config.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/mixed_precision/mixed_precision_quantization_config.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/mixed_precision/mixed_precision_search_facade.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/mixed_precision/mixed_precision_search_facade.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/mixed_precision/mixed_precision_search_manager.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/mixed_precision/mixed_precision_search_manager.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/mixed_precision/search_methods/__init__.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/mixed_precision/search_methods/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/mixed_precision/search_methods/linear_programming.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/mixed_precision/search_methods/linear_programming.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/mixed_precision/sensitivity_evaluation.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/mixed_precision/sensitivity_evaluation.py`

 * *Files 6% similar despite different names*

```diff
@@ -32,15 +32,14 @@
     def __init__(self,
                  graph: Graph,
                  quant_config: MixedPrecisionQuantizationConfigV2,
                  representative_data_gen: Callable,
                  fw_info: FrameworkInfo,
                  fw_impl: Any,
                  set_layer_to_bitwidth: Callable,
-                 get_quant_node_name: Callable,
                  disable_activation_for_metric: bool = False):
         """
         Initiates all relevant objects to manage a sensitivity evaluation for MP search.
         Create an object that allows to compute the sensitivity metric of an MP model (the sensitivity
         is computed based on the similarity of the interest points' outputs between the MP model
         and the float model).
         First, we initiate a SensitivityEvaluationManager that handles the components which are necessary for
@@ -54,25 +53,22 @@
             fw_info: FrameworkInfo object about the specific framework
                 (e.g., attributes of different layers' weights to quantize).
             quant_config: MP Quantization configuration for how the graph should be quantized.
             representative_data_gen: Dataset used for getting batches for inference.
             fw_impl: FrameworkImplementation object with a specific framework methods implementation.
             set_layer_to_bitwidth: A fw-dependent function that allows to configure a configurable MP model
                     with a specific bit-width configuration.
-            get_quant_node_name: A fw-dependent function that takes a node's name and outputs the node's name in a
-                quantized model (according to the fw conventions).
             disable_activation_for_metric: Whether to disable activation quantization when computing the MP metric.
         """
         self.graph = graph
         self.quant_config = quant_config
         self.representative_data_gen = representative_data_gen
         self.fw_info = fw_info
         self.fw_impl = fw_impl
         self.set_layer_to_bitwidth = set_layer_to_bitwidth
-        self.get_quant_node_name = get_quant_node_name
         self.disable_activation_for_metric = disable_activation_for_metric
 
         # Get interest points for distance measurement and a list of sorted configurable nodes names
         self.sorted_configurable_nodes_names = graph.get_configurable_sorted_nodes_names()
         self.interest_points = get_mp_interest_points(graph,
                                                       fw_impl.count_node_for_mixed_precision_interest_points,
                                                       quant_config.num_interest_points_factor)
@@ -86,15 +82,17 @@
             # Note that we need to modify the set of interest points before building the models,
             # therefore, it is separated from the part where we compute the actual gradient weights.
             self.outputs_replacement_nodes = get_output_replacement_nodes(graph, fw_impl)
             self.output_nodes_indices = self._update_ips_with_outputs_replacements()
 
         # Build a mixed-precision model which can be configured to use different bitwidth in different layers.
         # And a baseline model.
-        self.baseline_model, self.model_mp = self._build_models()
+        # Also, returns a mapping between a configurable graph's node and its matching layer(s)
+        # in the new built MP model.
+        self.baseline_model, self.model_mp, self.conf_node2layers = self._build_models()
 
         # Build images batches for inference comparison
         self.images_batches = self._get_images_batches(quant_config.num_of_images)
 
         # Get baseline model inference on all samples
         self.baseline_tensors_list = []  # setting from outside scope
 
@@ -131,27 +129,23 @@
                 compute the metric for the given configuration.
 
         Returns:
             The sensitivity metric of the MP model for a given configuration.
         """
 
         # Configure MP model with the given configuration.
-        self._configure_bitwidths_model(self.model_mp,
-                                        self.sorted_configurable_nodes_names,
-                                        mp_model_configuration,
+        self._configure_bitwidths_model(mp_model_configuration,
                                         node_idx)
 
         # Compute the distance matrix
         distance_matrix = self._build_distance_matrix()
 
         # Configure MP model back to the same configuration as the baseline model if baseline provided
         if baseline_mp_configuration is not None:
-            self._configure_bitwidths_model(self.model_mp,
-                                            self.sorted_configurable_nodes_names,
-                                            baseline_mp_configuration,
+            self._configure_bitwidths_model(baseline_mp_configuration,
                                             node_idx)
 
         return self._compute_mp_distance_measure(distance_matrix, self.quant_config.distance_weighting_method)
 
     def _init_baseline_tensors_list(self):
         """
         Evaluates the baseline model on all images and saves the obtained lists of tensors in a list for later use.
@@ -173,25 +167,25 @@
         evaluation_graph = copy.deepcopy(self.graph)
 
         if self.disable_activation_for_metric:
             for n in evaluation_graph.get_topo_sorted_nodes():
                 for c in n.candidates_quantization_cfg:
                     c.activation_quantization_cfg.enable_activation_quantization = False
 
-        model_mp, _ = self.fw_impl.model_builder(evaluation_graph,
-                                                 mode=ModelBuilderMode.MIXEDPRECISION,
-                                                 append2output=self.interest_points,
-                                                 fw_info=self.fw_info)
+        model_mp, _, conf_node2layers = self.fw_impl.model_builder(evaluation_graph,
+                                                                   mode=ModelBuilderMode.MIXEDPRECISION,
+                                                                   append2output=self.interest_points,
+                                                                   fw_info=self.fw_info)
 
         # Build a baseline model.
         baseline_model, _ = self.fw_impl.model_builder(evaluation_graph,
                                                        mode=ModelBuilderMode.FLOAT,
                                                        append2output=self.interest_points)
 
-        return baseline_model, model_mp
+        return baseline_model, model_mp, conf_node2layers
 
     def _compute_gradient_based_weights(self) -> np.ndarray:
         """
         Computes the gradient-based weights using the framework's model_grad method per batch of images.
 
         Returns: A vector of weights, one for each interest point,
         to be used for the distance metric weighted average computation.
@@ -211,54 +205,62 @@
                                                              self.quant_config.output_grad_factor,
                                                              norm_weights=self.quant_config.norm_weights)
                 batch_ip_gradients.append(image_ip_gradients)
             grad_per_batch.append(np.mean(batch_ip_gradients, axis=0))
         return np.mean(grad_per_batch, axis=0)
 
     def _configure_bitwidths_model(self,
-                                   model_mp: Any,
-                                   sorted_configurable_nodes_names: List[str],
                                    mp_model_configuration: List[int],
                                    node_idx: List[int]):
         """
         Configure a dynamic model (namely, model with layers that their weights and activation
         bit-width can be configured) using an MP model configuration mp_model_configuration.
 
         Args:
-            model_mp: Dynamic model to configure.
-            sorted_configurable_nodes_names: List of configurable nodes names sorted topology.
             mp_model_configuration: Configuration of bit-width indices to set to the model.
             node_idx: List of nodes' indices to configure (the rest layers are configured as the baseline model).
         """
 
         # Configure model
         # Note: Not all nodes in the graph are included in the MP model that is returned by the model builder.
         # Thus, the last configurable layer must be included in the interest points for evaluating the metric,
         # otherwise, not all configurable nodes will be considered throughout the MP optimization search (since
         # they will not affect the metric value).
-        model_mp_layers_names = self.fw_impl.get_model_layers_names(model_mp)
         if node_idx is not None:  # configure specific layers in the mp model
             for node_idx_to_configure in node_idx:
-                node_name = self.get_quant_node_name(sorted_configurable_nodes_names[node_idx_to_configure])
-                if node_name in model_mp_layers_names:
-                    current_layer = self.fw_impl.get_model_layer_by_name(model_mp, node_name)
-                    self.set_layer_to_bitwidth(current_layer, mp_model_configuration[node_idx_to_configure])
-                else:
-                    raise Exception("The last configurable node is not included in the list of interest points for"  # pragma: no cover
-                                    "sensitivity evaluation metric for the mixed-precision search.")
-
+                self._configure_node_bitwidth(self.sorted_configurable_nodes_names,
+                                              mp_model_configuration, node_idx_to_configure)
         else:  # use the entire mp_model_configuration to configure the model
             for node_idx_to_configure, bitwidth_idx in enumerate(mp_model_configuration):
-                node_name = self.get_quant_node_name(sorted_configurable_nodes_names[node_idx_to_configure])
-                if node_name in model_mp_layers_names:
-                    current_layer = self.fw_impl.get_model_layer_by_name(model_mp, node_name)
-                    self.set_layer_to_bitwidth(current_layer, mp_model_configuration[node_idx_to_configure])
-                else:
-                    raise Exception("The last configurable node is not included in the list of interest points for"
-                                    "sensitivity evaluation metric for the mixed-precision search.")  # pragma: no cover
+                self._configure_node_bitwidth(self.sorted_configurable_nodes_names,
+                                              mp_model_configuration, node_idx_to_configure)
+
+    def _configure_node_bitwidth(self,
+                                 sorted_configurable_nodes_names: List[str],
+                                 mp_model_configuration: List[int],
+                                 node_idx_to_configure: int):
+        """
+        Configures a node with multiple quantization candidates to the bitwidth candidate in the given index.
+        Args:
+            sorted_configurable_nodes_names: A list of configurable nodes names sorted according to the graph
+                topological sort order.
+            mp_model_configuration: Configuration of bit-width indices to set to the model.
+            node_idx_to_configure: Quantization configuration candidate to configure.
+
+        Returns:
+
+        """
+        node_name = sorted_configurable_nodes_names[node_idx_to_configure]
+        layers_to_config = self.conf_node2layers.get(node_name, None)
+        if layers_to_config is None:
+            Logger.error(
+                f"Couldn't find matching layers in the MP model for node {node_name}.")  # pragma: no cover
+
+        for current_layer in layers_to_config:
+            self.set_layer_to_bitwidth(current_layer, mp_model_configuration[node_idx_to_configure])
 
     def _compute_distance_matrix(self,
                                  baseline_tensors: List[Any],
                                  mp_tensors: List[Any]):
         """
         Compute the distance between the MP model's outputs and the baseline model's outputs
         for each image in the batch that was inferred.
```

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/mixed_precision/solution_refinement_procedure.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/mixed_precision/solution_refinement_procedure.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/model_builder_mode.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/model_builder_mode.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/model_collector.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/model_collector.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/model_validation.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/model_validation.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/network_editors/__init__.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/network_editors/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/network_editors/actions.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/network_editors/actions.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/network_editors/edit_network.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/network_editors/edit_network.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/network_editors/node_filters.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/network_editors/node_filters.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/node_prior_info.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/node_prior_info.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/quantization/__init__.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/quantization/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/quantization/candidate_node_quantization_config.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/quantization/candidate_node_quantization_config.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/quantization/core_config.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/quantization/core_config.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/quantization/debug_config.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/quantization/debug_config.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/quantization/filter_nodes_candidates.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/quantization/filter_nodes_candidates.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/quantization/node_quantization_config.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/quantization/node_quantization_config.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/quantization/quantization_analyzer.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/quantization/quantization_analyzer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/quantization/quantization_config.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/quantization/quantization_config.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/quantization/quantization_fn_selection.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/quantization/quantization_fn_selection.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/quantization/quantization_params_fn_selection.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/quantization/quantization_params_fn_selection.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/quantization/quantization_params_generation/__init__.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/quantization/quantization_params_generation/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/quantization/quantization_params_generation/error_functions.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/quantization/quantization_params_generation/error_functions.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/quantization/quantization_params_generation/kmeans_params.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/quantization/quantization_params_generation/kmeans_params.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/quantization/quantization_params_generation/lut_kmeans_params.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/quantization/quantization_params_generation/lut_kmeans_params.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/quantization/quantization_params_generation/outlier_filter.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/quantization/quantization_params_generation/outlier_filter.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/quantization/quantization_params_generation/power_of_two_selection.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/quantization/quantization_params_generation/power_of_two_selection.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/quantization/quantization_params_generation/qparams_activations_computation.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/quantization/quantization_params_generation/qparams_activations_computation.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/quantization/quantization_params_generation/qparams_computation.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/quantization/quantization_params_generation/qparams_computation.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/quantization/quantization_params_generation/qparams_search.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/quantization/quantization_params_generation/qparams_search.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/quantization/quantization_params_generation/qparams_weights_computation.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/quantization/quantization_params_generation/qparams_weights_computation.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/quantization/quantization_params_generation/symmetric_selection.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/quantization/quantization_params_generation/symmetric_selection.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/quantization/quantization_params_generation/uniform_selection.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/quantization/quantization_params_generation/uniform_selection.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/quantization/quantize_graph_weights.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/quantization/quantize_graph_weights.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/quantization/quantize_node.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/quantization/quantize_node.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/quantization/quantizers/__init__.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/quantization/quantizers/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/quantization/quantizers/kmeans_quantizer.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/quantization/quantizers/kmeans_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/quantization/quantizers/lut_kmeans_quantizer.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/quantization/quantizers/lut_kmeans_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/quantization/quantizers/quantizers_helpers.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/quantization/quantizers/quantizers_helpers.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/quantization/quantizers/uniform_quantizers.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/quantization/quantizers/uniform_quantizers.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/quantization/set_node_quantization_config.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/quantization/set_node_quantization_config.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/similarity_analyzer.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/similarity_analyzer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/statistics_correction/__init__.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/statistics_correction/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/statistics_correction/apply_bias_correction_to_graph.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/statistics_correction/apply_bias_correction_to_graph.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/statistics_correction/apply_second_moment_correction_to_graph.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/statistics_correction/apply_second_moment_correction_to_graph.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/statistics_correction/compute_bias_correction_of_graph.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/statistics_correction/compute_bias_correction_of_graph.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/statistics_correction/statistics_correction.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/statistics_correction/statistics_correction.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/substitutions/__init__.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/substitutions/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/substitutions/apply_substitutions.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/substitutions/apply_substitutions.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/substitutions/batchnorm_folding.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/substitutions/batchnorm_folding.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/substitutions/batchnorm_reconstruction.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/substitutions/batchnorm_reconstruction.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/substitutions/batchnorm_refusing.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/substitutions/batchnorm_refusing.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/substitutions/linear_collapsing.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/substitutions/linear_collapsing.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/substitutions/linear_collapsing_substitution.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/substitutions/linear_collapsing_substitution.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/substitutions/residual_collapsing.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/substitutions/residual_collapsing.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/substitutions/scale_equalization.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/substitutions/scale_equalization.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/substitutions/shift_negative_activation.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/substitutions/shift_negative_activation.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/substitutions/softmax_shift.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/substitutions/softmax_shift.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/substitutions/virtual_activation_weights_composition.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/substitutions/virtual_activation_weights_composition.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/substitutions/weights_activation_split.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/substitutions/weights_activation_split.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/user_info.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/user_info.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/visualization/__init__.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/visualization/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/visualization/final_config_visualizer.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/visualization/final_config_visualizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/visualization/nn_visualizer.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/visualization/nn_visualizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/common/visualization/tensorboard_writer.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/visualization/tensorboard_writer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/exporter.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/exporter.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/keras/__init__.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/keras/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/keras/back2framework/__init__.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/keras/back2framework/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/keras/back2framework/factory_model_builder.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/keras/back2framework/factory_model_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/keras/back2framework/float_model_builder.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/keras/back2framework/float_model_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/keras/back2framework/instance_builder.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/keras/back2framework/instance_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/keras/back2framework/keras_model_builder.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/keras/back2framework/keras_model_builder.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,22 +10,19 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 
 import tensorflow as tf
-from keras.engine.input_layer import InputLayer
-from keras.models import Model, clone_model
+from keras.models import Model
 from packaging import version
 
-from model_compression_toolkit.constants import INPUT_BASE_NAME
 from model_compression_toolkit.core.common.back2framework.base_model_builder import BaseModelBuilder
 from model_compression_toolkit.core.common.user_info import UserInformation
-from mct_quantizers import KerasActivationQuantizationHolder
 
 # As from Tensorflow 2.6, keras is a separate package and some classes should be imported differently.
 if version.parse(tf.__version__) < version.parse("2.6"):
     from tensorflow.keras.layers import Input
     from tensorflow.python.keras.layers.core import TFOpLambda
     from tensorflow.python.keras.engine.base_layer import TensorFlowOpLayer
     from tensorflow.python.keras.layers import Layer
@@ -164,29 +161,26 @@
             output_list = [OutTensor(n, 0) for n in self.append2output]
         else:
             output_list = self.graph.get_outputs()
 
         # Hold a dictionary from an input node to its corresponding input tensor. It is needed for when
         # building the model. Initially input nodes with input tensors are added to the dictionary,
         # as they're not added later.
-        input_nodes_to_input_tensors = {inode: Input(inode.framework_attr[BATCH_INPUT_SHAPE][1:],
-                                                     name=f'{inode.name}_{INPUT_BASE_NAME}')
-                                        for
-                                        inode in self.graph.get_inputs()}
-
+        input_nodes_to_input_tensors = {inode: Input(inode.framework_attr[BATCH_INPUT_SHAPE][1:], name=inode.name)
+                                        for inode in self.graph.get_inputs()}
 
         # Build a list of the model's input tensors. Switching from a dictionary to a list
         # to keep the tensors input order, since inputs in Graph are ordered by their indices.
         inputs_list = []
         for input_node in self.graph.get_inputs():
             inputs_list.append(input_nodes_to_input_tensors.get(input_node))
 
         # Build a dictionary from node to its output tensors, by applying the layers sequentially.
         for n in self.oh.node_sort:
-            op_func = self.oh.get_node_op_function(n) # Get node operation function
+            op_func = self.oh.get_node_op_function(n)  # Get node operation function
 
             input_tensors = self._build_input_tensors_list(n,
                                                            node_to_output_tensors_dict)  # Fetch Node inputs
             out_tensors_of_n, out_tensors_of_n_float = self._run_operation(n,  # Run node operation and fetch outputs
                                                                            input_tensors,
                                                                            op_func,
                                                                            input_nodes_to_input_tensors)
@@ -234,15 +228,14 @@
         List[TFReference]]:
         """
         Given a node, build a list of input tensors the node gets. The list is built
         based on the node's incoming edges and previous nodes' output tensors.
 
         Args:
             node: Node to build its input tensors list.
-            graph: Graph the node is in.
             node_to_output_tensors_dict: A dictionary from a node to its output tensors.
 
         Returns:
             A list of the node's input tensors.
         """
 
         input_tensors = []
```

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/keras/back2framework/model_gradients.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/keras/back2framework/model_gradients.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/keras/back2framework/quantized_model_builder.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/keras/back2framework/quantized_model_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/keras/constants.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/keras/constants.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/keras/default_framework_info.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/keras/default_framework_info.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/keras/graph_substitutions/__init__.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/keras/graph_substitutions/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/keras/graph_substitutions/substitutions/__init__.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/keras/graph_substitutions/substitutions/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/keras/graph_substitutions/substitutions/activation_decomposition.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/keras/graph_substitutions/substitutions/activation_decomposition.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/keras/graph_substitutions/substitutions/batchnorm_folding.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/keras/graph_substitutions/substitutions/batchnorm_folding.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/keras/graph_substitutions/substitutions/batchnorm_reconstruction.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/keras/graph_substitutions/substitutions/batchnorm_reconstruction.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/keras/graph_substitutions/substitutions/batchnorm_refusing.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/keras/graph_substitutions/substitutions/batchnorm_refusing.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/keras/graph_substitutions/substitutions/input_scaling.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/keras/graph_substitutions/substitutions/input_scaling.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/keras/graph_substitutions/substitutions/linear_collapsing.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/keras/graph_substitutions/substitutions/linear_collapsing.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/keras/graph_substitutions/substitutions/multi_head_attention_decomposition.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/keras/graph_substitutions/substitutions/multi_head_attention_decomposition.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/keras/graph_substitutions/substitutions/relu_bound_to_power_of_2.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/keras/graph_substitutions/substitutions/relu_bound_to_power_of_2.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/keras/graph_substitutions/substitutions/remove_relu_upper_bound.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/keras/graph_substitutions/substitutions/remove_relu_upper_bound.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/keras/graph_substitutions/substitutions/residual_collapsing.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/keras/graph_substitutions/substitutions/residual_collapsing.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/keras/graph_substitutions/substitutions/scale_equalization.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/keras/graph_substitutions/substitutions/scale_equalization.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/keras/graph_substitutions/substitutions/separableconv_decomposition.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/keras/graph_substitutions/substitutions/separableconv_decomposition.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/keras/graph_substitutions/substitutions/shift_negative_activation.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/keras/graph_substitutions/substitutions/shift_negative_activation.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/keras/graph_substitutions/substitutions/softmax_shift.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/keras/graph_substitutions/substitutions/softmax_shift.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/keras/graph_substitutions/substitutions/virtual_activation_weights_composition.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/keras/graph_substitutions/substitutions/virtual_activation_weights_composition.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/keras/graph_substitutions/substitutions/weights_activation_split.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/keras/graph_substitutions/substitutions/weights_activation_split.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/keras/keras_implementation.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/keras/keras_implementation.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,33 +8,39 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
+from functools import partial
 from typing import List, Any, Tuple, Callable, Dict
 
 import numpy as np
 import tensorflow as tf
+from mct_quantizers import KerasQuantizationWrapper, KerasActivationQuantizationHolder
 from tensorflow.keras.models import Model
 from tensorflow.python.layers.base import Layer
 
 from model_compression_toolkit.core.common.mixed_precision.sensitivity_evaluation import SensitivityEvaluation
+from model_compression_toolkit.core.common.mixed_precision.set_layer_to_bitwidth import set_layer_to_bitwidth
 from model_compression_toolkit.core.common.similarity_analyzer import compute_kl_divergence, compute_cs, compute_mse
 from model_compression_toolkit.core.keras.back2framework.model_gradients import \
     keras_iterative_approx_jacobian_trace
 from model_compression_toolkit.core.keras.constants import ACTIVATION, SOFTMAX, SIGMOID, ARGMAX, LAYER_NAME
 from model_compression_toolkit.core.keras.graph_substitutions.substitutions.batchnorm_reconstruction import \
     keras_batchnorm_reconstruction
 from model_compression_toolkit.core.keras.graph_substitutions.substitutions.virtual_activation_weights_composition import \
     VirtualActivationWeightsComposition
 from model_compression_toolkit.core.keras.graph_substitutions.substitutions.weights_activation_split import \
     WeightsActivationSplit
-from model_compression_toolkit.core.keras.mixed_precision.set_layer_to_bitwidth import set_layer_to_bitwidth
+from model_compression_toolkit.core.keras.mixed_precision.configurable_activation_quantizer import \
+    ConfigurableActivationQuantizer
+from model_compression_toolkit.core.keras.mixed_precision.configurable_weights_quantizer import \
+    ConfigurableWeightsQuantizer
 from model_compression_toolkit.core.keras.statistics_correction.apply_second_moment_correction import \
     keras_apply_second_moment_correction
 from packaging import version
 
 if version.parse(tf.__version__) < version.parse("2.6"):
     from tensorflow.keras.layers import Dense, Activation, Conv2D, DepthwiseConv2D, Conv2DTranspose, Concatenate, Add
     from tensorflow.python.keras.layers.core import TFOpLambda
@@ -85,15 +91,15 @@
 import model_compression_toolkit.core.keras.constants as keras_constants
 from model_compression_toolkit.core.keras.tf_tensor_numpy import tf_tensor_to_numpy, to_tf_tensor
 from model_compression_toolkit.core.keras.back2framework import get_keras_model_builder
 
 
 class KerasImplementation(FrameworkImplementation):
     """
-    An class with implemented methods to support optimizing Keras models.
+    A class with implemented methods to support optimizing Keras models.
     """
 
     def __init__(self):
         super().__init__()
 
     @property
     def constants(self):
@@ -141,28 +147,28 @@
         return to_tf_tensor(tensor)
 
     def model_builder(self,
                       graph: Graph,
                       mode: ModelBuilderMode,
                       append2output: List[Any] = None,
                       fw_info: FrameworkInfo = DEFAULT_KERAS_INFO,
-                      return_float_outputs: bool = False) -> Tuple[Model, UserInformation]:
+                      return_float_outputs: bool = False) -> Tuple:
         """
         Build a Keras model from a graph.
         The mode determines how the model should be build. append2output is a list of Nodes
         to set as the model outputs.
 
         Args:
             graph: Graph to build the model from it.
             mode: Mode for how to build the model.
             append2output: List of Nodes to set as the model's outputs.
             fw_info: FrameworkInfo object with information about the specific framework's model
             return_float_outputs (bool): whether to return outputs before or after quantization nodes (default)
         Returns:
-            A tuple of the Keras model that was built and an UserInformation object.
+            A tuple with the model and additional relevant supporting objects.
         """
 
         keras_model_builder = get_keras_model_builder(mode)
         return keras_model_builder(graph=graph,
                                    append2output=append2output,
                                    fw_info=fw_info,
                                    return_float_outputs=return_float_outputs).build_model()
@@ -369,16 +375,19 @@
         """
 
         return SensitivityEvaluation(graph=graph,
                                      quant_config=quant_config,
                                      representative_data_gen=representative_data_gen,
                                      fw_info=fw_info,
                                      fw_impl=self,
-                                     set_layer_to_bitwidth=set_layer_to_bitwidth,
-                                     get_quant_node_name=lambda node_name: f'quant_{node_name}',
+                                     set_layer_to_bitwidth=partial(set_layer_to_bitwidth,
+                                                                   weights_quantizer_type=ConfigurableWeightsQuantizer,
+                                                                   activation_quantizer_type=ConfigurableActivationQuantizer,
+                                                                   weights_quant_layer_type=KerasQuantizationWrapper,
+                                                                   activation_quant_layer_type=KerasActivationQuantizationHolder),
                                      disable_activation_for_metric=disable_activation_for_metric)
 
     def get_node_prior_info(self,
                             node: BaseNode,
                             fw_info: FrameworkInfo,
                             graph: Graph) -> NodePriorInfo:
         """
@@ -443,44 +452,14 @@
             return compute_kl_divergence
         elif layer_class == tf.nn.sigmoid:
             return compute_cs
         elif layer_class == Dense:
             return compute_cs
         return compute_mse
 
-    def get_model_layers_names(self,
-                               model: Model) -> List[str]:
-        """
-        Returns a list of the given model's layers names.
-
-        Args:
-            model: A Keras model.
-
-        Returns: List of layers' names.
-
-        """
-
-        return [layer.name for layer in model.layers]
-
-    def get_model_layer_by_name(self,
-                                model: Model,
-                                layer_name: str) -> Layer:
-        """
-        Returns a Keras model's layer by its name.
-
-        Args:
-            model: A Keras model to retrieve a layer from.
-            layer_name: The requested layer's name.
-
-        Returns: A Keras layer object.
-
-        """
-
-        return model.get_layer(name=layer_name)
-
     def model_grad(self,
                    graph_float: common.Graph,
                    model_input_tensors: Dict[BaseNode, np.ndarray],
                    interest_points: List[BaseNode],
                    output_list: List[BaseNode],
                    all_outputs_indices: List[int],
                    alpha: float = 0.3,
```

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/keras/keras_model_validation.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/keras/keras_model_validation.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/keras/keras_node_prior_info.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/keras/keras_node_prior_info.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/keras/kpi_data_facade.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/keras/kpi_data_facade.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/keras/mixed_precision/__init__.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/keras/mixed_precision/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/keras/quantizer/__init__.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/keras/quantizer/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/keras/quantizer/base_quantizer.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/keras/quantizer/base_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/keras/quantizer/fake_quant_builder.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/keras/quantizer/fake_quant_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/keras/quantizer/lut_fake_quant.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/keras/quantizer/lut_fake_quant.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/keras/quantizer/mixed_precision/__init__.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/keras/reader/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,7 +8,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
+
```

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/keras/quantizer/mixed_precision/selective_activation_quantizer.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/keras/mixed_precision/configurable_weights_quantizer.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,162 +1,131 @@
-# Copyright 2022 Sony Semiconductor Israel, Inc. All rights reserved.
+# Copyright 2023 Sony Semiconductor Israel, Inc. All rights reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
+from functools import partial
+from typing import Dict, Any, List
 
-import numpy as np
-import tensorflow as tf
-from tensorflow.python.framework.tensor_shape import TensorShape
-from tensorflow_model_optimization.python.core.quantization.keras.quantize_wrapper import QuantizeWrapper
-from tensorflow_model_optimization.python.core.quantization.keras.quantizers import Quantizer
-from typing import Dict, Any, List, Callable
-
+from model_compression_toolkit.core.common.mixed_precision.configurable_quantizer_utils import \
+    verify_candidates_descending_order, init_quantized_weights
 from model_compression_toolkit.core.common.quantization.candidate_node_quantization_config import \
     CandidateNodeQuantizationConfig
-from model_compression_toolkit.core.common.quantization.node_quantization_config import NodeActivationQuantizationConfig
+from model_compression_toolkit.logger import Logger
+from model_compression_toolkit.target_platform_capabilities.target_platform import QuantizationMethod
+from mct_quantizers import QuantizationTarget
+from mct_quantizers import mark_quantizer
+
+import tensorflow as tf
+from model_compression_toolkit.core.common.mixed_precision.configurable_quant_id import \
+    ConfigurableQuantizerIdentifier
+from mct_quantizers.keras.quantizers import BaseKerasInferableQuantizer
 
 
-class SelectiveActivationQuantizer(Quantizer):
+@mark_quantizer(quantization_target=QuantizationTarget.Weights,
+                quantization_method=[QuantizationMethod.POWER_OF_TWO, QuantizationMethod.SYMMETRIC,
+                                     QuantizationMethod.UNIFORM, QuantizationMethod.LUT_POT_QUANTIZER,
+                                     QuantizationMethod.LUT_SYM_QUANTIZER],
+                quantizer_type=ConfigurableQuantizerIdentifier.CONFIGURABLE_ID)
+class ConfigurableWeightsQuantizer(BaseKerasInferableQuantizer):
     """
-    Quantizer that can use different quantized weights on-the-fly.
+    Configurable weights quantizer for Keras mixed precision search.
+    The quantizer holds a set of quantized layer's weights for each of the given bit-width candidates, provided by the
+    node's quantization config. This allows to use different quantized weights on-the-fly.
+
     The general idea behind this kind of quantizer is that it gets the float tensor to quantize
-    when initialize, it quantizes the float tensor in different bitwidths, and every time it need to return a
+    when initialized, it quantizes the float tensor in different bitwidths, and every time it need to return a
     quantized version of the float weight, it returns only one quantized weight according to an "active"
     index - the index of a candidate weight quantization configuration from a list of candidates that was passed
-    to the SelectiveWeightsQuantizer when it was initialized.
-    The "active" index can be configured as part of the SelectiveWeightsQuantizer's API, so a different quantized
-    weight can be returned in another time.
+    to the quantizer when it was initialized.
     """
 
     def __init__(self,
                  node_q_cfg: List[CandidateNodeQuantizationConfig],
-                 max_candidate_idx: int):
+                 float_weights: tf.Tensor,
+                 max_candidate_idx: int = 0):
         """
-        Init a selective quantizer.
+        Initializes a configurable quantizer.
 
         Args:
-            node_q_cfg: Quantization configuration candidate of the node that generated the layer that will
+            node_q_cfg: Quantization configuration candidates of the node that generated the layer that will
                 use this quantizer.
+            float_weights: Float weights of the layer.
             max_candidate_idx: Index of the node's candidate that has the maximal bitwidth (must exist absolute max).
+
         """
+
+        super(ConfigurableWeightsQuantizer, self).__init__()
+
         self.node_q_cfg = node_q_cfg
-        self.active_quantization_config_index = max_candidate_idx  # initialize with first config as default
-        self.activation_quantizers = []
-        self._store_activation_quantizers()
+        self.float_weights = float_weights
+        self.max_candidate_idx = max_candidate_idx
 
-    def _get_qc_quantizer(self, index: int) -> NodeActivationQuantizationConfig:
-        """
-        Quantize the quantizer float weight using a candidate quantization configuration.
+        verify_candidates_descending_order(self.node_q_cfg)
 
-        Args:
-            index: Index of the candidate to use for the quantization.
+        for qc in self.node_q_cfg:
+            if qc.weights_quantization_cfg.enable_weights_quantization != \
+                    self.node_q_cfg[0].weights_quantization_cfg.enable_weights_quantization:
+                Logger.error("Candidates with different weights enabled properties is currently not supported.")
 
-        Returns:
-            Quantized weight.
-        """
-        qc = self.node_q_cfg[index].activation_quantization_cfg
-        return qc
+        # Initialize quantized weights for each weight that should be quantized.
+        self.quantized_weights = init_quantized_weights(node_q_cfg=self.node_q_cfg,
+                                                        float_weights=self.float_weights,
+                                                        fw_tensor_convert_func=partial(tf.convert_to_tensor,
+                                                                                       dtype=tf.float32))
 
-    def _store_activation_quantizers(self):
-        """
-        Go over all candidates configurations, quantize the quantizer float weight according to each one
-        of them, and store the quantized weights in a list quantized_weights the quantizer holds.
-        """
-        for i in range(len(self.node_q_cfg)):
-            q_activation = self._get_qc_quantizer(i)
-            self.activation_quantizers.append(q_activation.quantize_node_output)
+        self.active_quantization_config_index = self.max_candidate_idx
 
-    def build(self,
-              tensor_shape: TensorShape,
-              name: str,
-              layer: QuantizeWrapper) -> Dict[str, tf.Variable]:
+    def set_weights_bit_width_index(self,
+                                    index: int):
         """
-        The build method has to be implemented as part of the Keras framework,
-        but there is no need to use it here as we do not train any new variable.
-        Hence, it returns an empty dictionary.
+        Change the "active" bitwidth index the configurable quantizer uses, so a different quantized weight
+        will be used.
+
+        Args:
+            index: Quantization configuration candidate index to use.
+
         """
 
-        return {}
+        if index >= len(self.node_q_cfg):
+            Logger.error(f'Quantizer has {len(self.node_q_cfg)} '  # pragma: no cover
+                         f'possible nbits. Can not set index {index}')
+        self.active_quantization_config_index = index
 
     def __call__(self,
-                 inputs: tf.Tensor,
-                 training: bool,
-                 weights: Dict[str, tf.Variable],
-                 **kwargs: Dict[str, Any]) -> np.ndarray:
-        """
-        Method to return the quantized weight. This method is called
-        when the framework needs to quantize a float weight, and is expected to return the quantized
-        weight. Since we already quantized the weight in all possible bitwidths, we do not
-        quantize it again, and simply return the quantized weight according to the current
-        active_quantization_config_index.
+                 inputs: tf.Tensor) -> tf.Tensor:
+        """
+        Method to return the quantized weight. This method is called when the framework needs to quantize a
+        float weight, and is expected to return the quantized weight. Since we already quantized the weight in
+        all possible bitwidths, we do not quantize it again, and simply return the quantized weight according
+        to the current active_quantization_config_index.
+
+        Args:
+            inputs: Input tensor (not relevant since the weights are already quantized).
 
         Returns:
             Quantized weight, that was quantized using number of bits that is in a
             specific quantization configuration candidate (the candidate's index is the
             index that is in active_quantization_config_index the quantizer holds).
         """
-        return self.activation_quantizers[self.active_quantization_config_index](inputs)
 
-    def set_active_quantization_config_index(self, index: int):
-        """
-        Set an index to use for the quantized weight the quantizer returns
-        when requested.
-
-        Args:
-            index: Index of a candidate quantization configuration to use its quantized
-            version of the float weight.
-        """
-        assert index < len(
-            self.node_q_cfg), f'Quantizer has {len(self.node_q_cfg)} ' \
-                                      f'possible nbits. Can not set ' \
-                                      f'index {index}'
-        self.active_quantization_config_index = index
+        return self.quantized_weights[self.active_quantization_config_index]
 
     def get_config(self) -> Dict[str, Any]:  # pragma: no cover
         """
-        Returns: Configuration of TrainableQuantizer.
+        Returns: The ConfigurableWeightsQuantizer configuration.
         """
 
         return {
+            'float_weights': self.float_weights,
             'node_q_cfg': self.node_q_cfg,
-            'active_quantization_config_index': self.active_quantization_config_index,
-            'activation_quantizers': self.activation_quantizers
+            'active_quantization_config_index': self.active_quantization_config_index
         }
-
-    def __eq__(self, other: Any) -> bool:  # pragma: no cover
-        """
-        Check if equals to another object.
-
-        Args:
-            other: Other object to compare.
-
-        Returns:
-            Whether they are equal or not.
-        """
-        if not isinstance(other, SelectiveActivationQuantizer):
-            return False
-
-        return self.node_q_cfg == other.node_q_cfg and \
-               self.active_quantization_config_index == other.node_q_cfg and \
-               self.activation_quantizers == other.activation_quantizers
-
-    def __ne__(self, other: Any) -> bool:  # pragma: no cover
-        """
-        Check if not equals to another object.
-
-        Args:
-            other: Other object to compare.
-
-        Returns:
-            Whether they are differ or not.
-        """
-        return not self.__eq__(other)
```

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/keras/quantizer/mixed_precision/selective_weights_quantizer.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/gptq/keras/quantizer/ste_rounding/symmetric_ste.py`

 * *Files 23% similar despite different names*

```diff
@@ -9,171 +9,173 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 
+from typing import Dict, Any
+
 import numpy as np
 import tensorflow as tf
-from tensorflow.python.framework.tensor_shape import TensorShape
-from tensorflow_model_optimization.python.core.quantization.keras.quantize_wrapper import QuantizeWrapper
-from tensorflow_model_optimization.python.core.quantization.keras.quantizers import Quantizer
-from typing import Dict, Any, List
-
-from model_compression_toolkit.core.common.quantization.candidate_node_quantization_config import \
-    CandidateNodeQuantizationConfig
-
 
-class SelectiveWeightsQuantizer(Quantizer):
-    """
-    Quantizer that can use different quantized weights on-the-fly.
-    The general idea behind this kind of quantizer is that it gets the float tensor to quantize
-    when initialize, it quantizes the float tensor in different bitwidths, and every time it need to return a
-    quantized version of the float weight, it returns only one quantized weight according to an "active"
-    index - the index of a candidate weight quantization configuration from a list of candidates that was passed
-    to the SelectiveWeightsQuantizer when it was initialized.
-    The "active" index can be configured as part of the SelectiveWeightsQuantizer's API, so a different quantized
-    weight can be returned in another time.
+from model_compression_toolkit.gptq import RoundingType
+from model_compression_toolkit.target_platform_capabilities.target_platform import QuantizationMethod
+from mct_quantizers import QuantizationTarget
+from model_compression_toolkit.gptq.common.gptq_constants import AUXVAR, PTQ_THRESHOLD
+from model_compression_toolkit.gptq.keras.quantizer import quant_utils as qutils
+from model_compression_toolkit.constants import THRESHOLD
+from model_compression_toolkit.core.common.defaultdict import DefaultDict
+from model_compression_toolkit.gptq.keras.quantizer.base_keras_gptq_quantizer import BaseKerasGPTQTrainableQuantizer
+from model_compression_toolkit.trainable_infrastructure import TrainableQuantizerWeightsConfig
+from mct_quantizers import mark_quantizer
+from model_compression_toolkit.trainable_infrastructure.common.quant_utils import \
+    get_threshold_reshape_shape
+from model_compression_toolkit.trainable_infrastructure.common.base_trainable_quantizer import VariableGroup
+
+
+def pertubation_symmetric_quantizer(input_tensor: tf.Tensor,
+                                    auxvar_tensor: tf.Variable,
+                                    max_tensor: tf.Tensor,
+                                    num_bits: int,
+                                    signed: bool,
+                                    power_of_two: bool,
+                                    max_lsbs_change: int = 1) -> tf.Tensor:
     """
+    Quantize a tensor symmetrically with maximum LSBs shift.
 
-    def __init__(self,
-                 node_q_cfg: List[CandidateNodeQuantizationConfig],
-                 float_weight: np.ndarray,
-                 max_candidate_idx: int):
-        """
-        Init a selective quantizer.
+    Args:
+        input_tensor: Tensor to quantize. values of this tensor are not changed during gptq.
+        auxvar_tensor: Tensor that manifests the bit shift the weight due to gptq
+        max_tensor: Tensor with max values to compute the threshold.
+        num_bits: Num of bits to use.
+        signed: Signedness of the quantization range.
+        power_of_two: Whether the threshold should be constrained or not.
+        max_lsbs_change: maximum number of LSBs that the auxvar is allowed to change
 
-        Args:
-            node_q_cfg: Quantization configuration candidates of the node that generated the layer that will
-                use this quantizer.
-            float_weight: Float weights of the layer.
-            max_candidate_idx: Index of the node's candidate that has the maximal bitwidth (must exist absolute max).
-        """
-
-        self.node_q_cfg = node_q_cfg
-        self.quantizer_fn_list = [qc.weights_quantization_cfg.weights_quantization_fn for qc in self.node_q_cfg]
-        self.float_weight = float_weight
-        self.quantized_weights = []
-        self.active_quantization_config_index = max_candidate_idx
-        self._store_quantized_weights()
+    Returns:
+        A quantized tensor.
+    """
 
-    def _quantize_by_qc(self, index: int) -> np.ndarray:
-        """
-        Quantize the quantizer float weight using a candidate quantization configuration.
+    if power_of_two:
+        max_tensor = qutils.power_of_two_max(max_tensor)
+    delta = qutils.calculate_delta(max_tensor, num_bits, signed)
+    input_tensor_int = tf.stop_gradient(tf.round(input_tensor / delta))
+    tensor_q = qutils.ste_round(
+        input_tensor_int + qutils.ste_clip(auxvar_tensor, max_val=max_lsbs_change * delta) / delta)
+    min_int = -int(signed) * (2 ** (num_bits - int(signed)))
+    max_int = (2 ** (num_bits - int(signed))) - 1
+    return delta * qutils.ste_clip(tensor_q, max_val=max_int, min_val=min_int)
 
-        Args:
-            index: Index of the candidate to use for the quantization.
 
-        Returns:
-            Quantized weight.
-        """
-        qc = self.node_q_cfg[index].weights_quantization_cfg
-        return self.quantizer_fn_list[index](self.float_weight,
-                                             qc.weights_n_bits,
-                                             True,
-                                             qc.weights_quantization_params,
-                                             qc.weights_per_channel_threshold,
-                                             qc.weights_channels_axis)
+@mark_quantizer(quantization_target=QuantizationTarget.Weights,
+                quantization_method=[QuantizationMethod.POWER_OF_TWO, QuantizationMethod.SYMMETRIC],
+                quantizer_type=RoundingType.STE)
+class STEWeightGPTQQuantizer(BaseKerasGPTQTrainableQuantizer):
+    """
+    Trainable symmetric quantizer to quantize a layer weights.
+    """
 
-    def _store_quantized_weights(self):
+    def __init__(self,
+                 quantization_config: TrainableQuantizerWeightsConfig,
+                 max_lsbs_change_map: dict = DefaultDict({}, lambda: 1)):
         """
+        Initialize a STEWeightGPTQQuantizer object with parameters to use for the quantization.
 
-        Go over all candidates configurations, quantize the quantizer float weight according to each one
-        of them, and store the quantized weights in a list quantized_weights the quantizer holds.
-
+        Args:
+            quantization_config: Trainable weights quantizer config.
+            max_lsbs_change_map: a mapping between number of bits to max lsb change.
         """
-        for i in range(len(self.node_q_cfg)):
-            q_weight = self._quantize_by_qc(i)
-            self.quantized_weights.append(tf.Variable(q_weight,
-                                                      trainable=False,
-                                                      dtype=tf.float32))
-
-    def build(self,
-              tensor_shape: TensorShape,
-              name: str,
-              layer: QuantizeWrapper) -> Dict[str, tf.Variable]:
+        super().__init__(quantization_config)
+        self.num_bits = quantization_config.weights_n_bits
+        self.per_channel = quantization_config.weights_per_channel_threshold
+
+        threshold_values = quantization_config.weights_quantization_params[THRESHOLD]
+        self.threshold_shape = np.asarray(threshold_values).shape
+        self.threshold_values = np.reshape(np.asarray(threshold_values), [-1]) if self.per_channel else float(
+            threshold_values)
+
+        self.quantization_axis = quantization_config.weights_channels_axis
+        self.power_of_two = quantization_config.weights_quantization_method == QuantizationMethod.POWER_OF_TWO
+        self.max_lsbs_change = max_lsbs_change_map.get(self.num_bits)
+
+    def initialize_quantization(self,
+                                tensor_shape: Any,
+                                name: str,
+                                layer: Any):
         """
-        The build method has to be implemented as part of the Keras framework,
-        but there is no need to use it here as we do not train any new variable.
-        Hence, it returns an empty dictionary.
+        Add quantizer parameters to the quantizer parameters dictionary
 
+        Args:
+            tensor_shape: tensor shape of the quantized tensor.
+            name: Tensor name.
+            layer: Layer to quantize.
+        """
+
+        ptq_threshold_tensor = layer.add_weight(
+            f"{name}_{PTQ_THRESHOLD}",
+            shape=len(self.threshold_values) if self.per_channel else (),
+            initializer=tf.keras.initializers.Constant(1.0),
+            trainable=False)
+        ptq_threshold_tensor.assign(self.threshold_values)
+
+        w = getattr(layer.layer, name)
+        auxvar_tensor = layer.add_weight(
+            f"{name}_{AUXVAR}",
+            shape=list(w.shape),
+            initializer=tf.keras.initializers.Constant(0.0),
+            trainable=True)
+
+        # save the quantizer added parameters for later calculations
+        self.add_quantizer_variable(PTQ_THRESHOLD, ptq_threshold_tensor, VariableGroup.QPARAMS)
+        self.add_quantizer_variable(AUXVAR, auxvar_tensor, VariableGroup.WEIGHTS)
+
+    def __call__(self,
+                 inputs: tf.Tensor,
+                 training: bool):
         """
+        Quantize a tensor.
 
-        return {}
-
-    def __call__(self, inputs: tf.Tensor,
-                 training: bool,
-                 weights: Dict[str, tf.Variable],
-                 **kwargs: Dict[str, Any]) -> np.ndarray:
-        """
-        Method to return the quantized weight. This method is called
-        when the framework needs to quantize a float weight, and is expected to return the quantized
-        weight. Since we already quantized the weight in all possible bitwidths, we do not
-        quantize it again, and simply return the quantized weight according to the current
-        active_quantization_config_index.
+        Args:
+            inputs: Input tensor to quantize.
+            training: Whether the graph is in training mode.
 
         Returns:
-            Quantized weight, that was quantized using number of bits that is in a
-            specific quantization configuration candidate (the candidate's index is the
-            index that is in active_quantization_config_index the quantizer holds).
+            The quantized tensor.
         """
 
-        return self.quantized_weights[self.active_quantization_config_index]
-
-    def set_active_quantization_config_index(self, index: int):
-        """
-        Set an index to use for the quantized weight the quantizer returns
-        when requested.
-
-        Args:
-            index: Index of a candidate quantization configuration to use its quantized
-            version of the float weight.
-
-        """
-        assert index < len(
-            self.node_q_cfg), f'Quantizer has {len(self.node_q_cfg)} ' \
-                                      f'possible nbits. Can not set ' \
-                                      f'index {index}'
-        self.active_quantization_config_index = index
+        auxvar = self.get_quantizer_variable(AUXVAR)
+        ptq_threshold_tensor = self.get_quantizer_variable(PTQ_THRESHOLD)
 
-    def get_config(self) -> Dict[str, Any]:  # pragma: no cover
-        """
-        Returns: Configuration of TrainableQuantizer.
-        """
+        if self.per_channel:
+            reshape_shape = get_threshold_reshape_shape(inputs.shape,
+                                                        quant_axis=self.quantization_axis,
+                                                        quant_axis_dim=-1)
+            ptq_threshold_tensor = tf.reshape(ptq_threshold_tensor, reshape_shape)
+            q_tensor = pertubation_symmetric_quantizer(inputs,
+                                                       auxvar,
+                                                       ptq_threshold_tensor,
+                                                       self.num_bits,
+                                                       signed=True,
+                                                       power_of_two=self.power_of_two,
+                                                       max_lsbs_change=self.max_lsbs_change)
+            return q_tensor
+        else:
+            return pertubation_symmetric_quantizer(inputs,
+                                                   auxvar,
+                                                   ptq_threshold_tensor,
+                                                   self.num_bits,
+                                                   signed=True,
+                                                   power_of_two=self.power_of_two)
 
-        return {
-            'node_q_cfg': self.node_q_cfg,
-            'float_weight': self.float_weight,
-            'quantizer_fn_list': self.quantizer_fn_list,
-            'quantized_weights': self.quantized_weights,
-            'active_quantization_config_index': self.active_quantization_config_index
-        }
 
-    def __eq__(self, other: Any) -> bool:  # pragma: no cover
+    def get_quant_config(self) -> Dict[str, np.ndarray]:
         """
-        Check if equals to another object.
-        Args:
-            other: Other object to compare.
+        Returns the config used to edit NodeQuantizationConfig after GPTQ retraining
 
         Returns:
-            Whether they are equal or not.
-        """
-        if not isinstance(other, SelectiveWeightsQuantizer):
-            return False
-
-        return (self.node_q_cfg == other.node_q_cfg and
-                self.float_weight == other.float_weight and
-                self.quantizer_fn_list == other.quantizer_fn_list and
-                self.self.quantized_weights == other.self.quantized_weights and
-                self.active_quantization_config_index == other.active_quantization_config_index)
+            A dictionary of attributes the quantize_config retraining has changed during GPTQ retraining.
+            Keys must match NodeQuantizationConfig attributes
 
-    def __ne__(self, other: Any) -> bool:  # pragma: no cover
-        """
-        Check if not equals to another object.
-        Args:
-            other: Other object to compare.
-
-        Returns:
-            Whether they are differ or not.
         """
-        return not self.__eq__(other)
+        old_threshold = self.get_quantizer_variable(PTQ_THRESHOLD)
+        return {THRESHOLD: old_threshold.numpy().reshape(self.threshold_shape)}
```

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/keras/reader/__init__.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/keras/reader/nested_model/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/keras/reader/common.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/keras/reader/common.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/keras/reader/connectivity_handler.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/keras/reader/connectivity_handler.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/keras/reader/nested_model/__init__.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/keras/visualization/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/keras/reader/nested_model/edges_merger.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/keras/reader/nested_model/edges_merger.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/keras/reader/nested_model/nested_model_handler.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/keras/reader/nested_model/nested_model_handler.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/keras/reader/nested_model/nodes_merger.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/keras/reader/nested_model/nodes_merger.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/keras/reader/nested_model/outputs_merger.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/keras/reader/nested_model/outputs_merger.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/keras/reader/node_builder.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/keras/reader/node_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/keras/reader/reader.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/keras/reader/reader.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/keras/statistics_correction/__init__.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/keras/statistics_correction/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/keras/statistics_correction/apply_second_moment_correction.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/keras/statistics_correction/apply_second_moment_correction.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/keras/tf_tensor_numpy.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/keras/tf_tensor_numpy.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/keras/visualization/__init__.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,14 @@
-# Copyright 2021 Sony Semiconductor Israel, Inc. All rights reserved.
+# Copyright 2023 Sony Semiconductor Israel, Inc. All rights reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
-
```

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/pytorch/__init__.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/pytorch/back2framework/__init__.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/pytorch/back2framework/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/pytorch/back2framework/factory_model_builder.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/pytorch/back2framework/factory_model_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/pytorch/back2framework/float_model_builder.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/pytorch/back2framework/float_model_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/pytorch/back2framework/instance_builder.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/pytorch/back2framework/instance_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/pytorch/back2framework/mixed_precision_model_builder.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/pytorch/back2framework/quantized_model_builder.py`

 * *Files 26% similar despite different names*

```diff
@@ -9,102 +9,68 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 
-from typing import List, Any, Tuple
+from typing import List, Tuple
 
 import torch
 
 from model_compression_toolkit.core import FrameworkInfo
 from model_compression_toolkit.core import common
 from model_compression_toolkit.core.common import BaseNode
-from model_compression_toolkit.core.common.graph.functional_node import FunctionalNode
 from model_compression_toolkit.core.common.user_info import UserInformation
-from model_compression_toolkit.core.pytorch.back2framework.instance_builder import node_builder
 from model_compression_toolkit.core.pytorch.back2framework.pytorch_model_builder import PyTorchModelBuilder, \
     PytorchModel
-
 from model_compression_toolkit.core.pytorch.default_framework_info import DEFAULT_PYTORCH_INFO
-from model_compression_toolkit.core.pytorch.mixed_precision.mixed_precision_wrapper import PytorchMixedPrecisionWrapper
 
 
-class MixedPrecisionPyTorchModel(PytorchModel):
+class QuantizedPyTorchModel(PytorchModel):
+    """
+    Quantized PyTorch model.
+    """
 
     def __init__(self,
                  graph: common.Graph,
                  append2output=None):
         """
 
         Args:
             graph: Graph to build its corresponding Pytorch model.
             append2output: List of nodes or OutTensor objects.
         """
 
         super().__init__(graph,
                          append2output)
 
-
-    def _add_modules(self):
-        configurable_nodes = self.graph.get_configurable_sorted_nodes()
-        for n in self.node_sort:
-            if n in configurable_nodes:
-                self.add_module(n.name, PytorchMixedPrecisionWrapper(n,
-                                                                     DEFAULT_PYTORCH_INFO))
-            else:
-                if not isinstance(n, FunctionalNode):
-                    self.add_module(n.name, node_builder(n))
-
     def _quantize_node_activations(self,
                                    node: BaseNode,
                                    input_tensors: List[torch.Tensor]) -> List[torch.Tensor]:
         """
         Quantize node's activation given input tensors.
 
         Args:
             node: Node to quantize its outputs.
             input_tensors: Input tensors of the node.
 
         Returns:
             Output of the node.
 
         """
-        if node.is_all_activation_candidates_equal():
-            # otherwise, we want to use the float tensor when building the model for MP search
-            input_tensors = node.candidates_quantization_cfg[0].activation_quantization_cfg.quantize_node_output(input_tensors)
+        if node.is_activation_quantization_enabled():
+            if isinstance(input_tensors, list):
+                input_tensors = torch.cat(input_tensors, dim=0)
+            return node.final_activation_quantization_cfg.quantize_node_output(input_tensors)
         return input_tensors
 
 
-    def _get_op_func(self,
-                     node: BaseNode,
-                     configurable_nodes_names: List[str]) -> Any:
-        """
-        Gets the operation function that runs the actual inference of the nodes compatible layer.
-
-        Args:
-            node: The corresponding node of the layer it runs.
-            configurable_nodes_names: A list of names of configurable nodes in the quantized model.
-
-        Returns: Module/functional to apply to the input tensors.
-
-        """
-        if node.name in configurable_nodes_names:
-            return getattr(self, node.name)
-        else:
-            return node.type if isinstance(node, FunctionalNode) else getattr(self, node.name)
-
+class QuantizedPyTorchModelBuilder(PyTorchModelBuilder):
 
-
-
-class MixedPrecisionPyTorchModelBuilder(PyTorchModelBuilder):
-    """
-    Mixed-precision PyTorch model.
-    """
     def __init__(self,
                  graph: common.Graph,
                  append2output=None,
                  fw_info: FrameworkInfo = DEFAULT_PYTORCH_INFO,
                  return_float_outputs: bool = False):
         """
 
@@ -118,13 +84,13 @@
         super().__init__(graph,
                          append2output,
                          fw_info,
                          return_float_outputs)
 
     def build_model(self) -> Tuple[PytorchModel, UserInformation]:
         """
-        Build a PyTorch float model and return it.
-        Returns: Float PyTorch model and user information.
+        Build a PyTorch quantized model and return it.
+        Returns: Quantized PyTorch model and user information.
 
         """
-        return MixedPrecisionPyTorchModel(self.graph,
-                                          self.append2output), self.graph.user_info
+        return QuantizedPyTorchModel(self.graph,
+                                     self.append2output), self.graph.user_info
```

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/pytorch/back2framework/model_gradients.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/pytorch/back2framework/model_gradients.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/pytorch/back2framework/pytorch_model_builder.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/pytorch/back2framework/pytorch_model_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/pytorch/back2framework/quantization_wrapper/__init__.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/pytorch/back2framework/quantization_wrapper/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/pytorch/back2framework/quantization_wrapper/quantized_layer_wrapper.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/pytorch/back2framework/quantization_wrapper/quantized_layer_wrapper.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/pytorch/back2framework/quantization_wrapper/wrapper_quantize_config.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/pytorch/back2framework/quantization_wrapper/wrapper_quantize_config.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/pytorch/constants.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/pytorch/constants.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/pytorch/default_framework_info.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/pytorch/default_framework_info.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/pytorch/graph_substitutions/__init__.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/pytorch/graph_substitutions/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/__init__.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/batchnorm_folding.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/batchnorm_folding.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/batchnorm_reconstruction.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/batchnorm_reconstruction.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/batchnorm_refusing.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/batchnorm_refusing.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/const_holder_conv.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/const_holder_conv.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/linear_collapsing.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/linear_collapsing.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/multi_head_attention_decomposition.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/multi_head_attention_decomposition.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/permute_call_method.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/permute_call_method.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/relu_bound_to_power_of_2.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/relu_bound_to_power_of_2.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/reshape_with_static_shapes.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/reshape_with_static_shapes.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/residual_collapsing.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/residual_collapsing.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/scale_equalization.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/scale_equalization.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/shift_negative_activation.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/shift_negative_activation.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/softmax_shift.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/softmax_shift.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/virtual_activation_weights_composition.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/virtual_activation_weights_composition.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/weights_activation_split.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/weights_activation_split.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/pytorch/kpi_data_facade.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/pytorch/kpi_data_facade.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/pytorch/mixed_precision/__init__.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/pytorch/mixed_precision/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/pytorch/mixed_precision/mixed_precision_wrapper.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/keras/back2framework/mixed_precision_model_builder.py`

 * *Files 22% similar despite different names*

```diff
@@ -8,205 +8,270 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
+from typing import Tuple, Any, Dict, Union, List
 
-from typing import Any, List
+from keras.engine.base_layer import Layer
+from keras.models import Model
+from mct_quantizers import KerasQuantizationWrapper, KerasActivationQuantizationHolder, QuantizationTarget
+from mct_quantizers.common.get_quantizers import get_inferable_quantizer_class
+from mct_quantizers.keras.quantizers import BaseKerasInferableQuantizer
 
-import torch
-import copy
-
-from model_compression_toolkit.core import FrameworkInfo
 from model_compression_toolkit.core.common import BaseNode
-from model_compression_toolkit.core.common.graph.functional_node import FunctionalNode
-from model_compression_toolkit.core.pytorch.utils import set_model, to_torch_tensor
+from model_compression_toolkit.core.common.user_info import UserInformation
+from model_compression_toolkit.core.keras.back2framework.keras_model_builder import KerasModelBuilder
+from model_compression_toolkit.core.keras.mixed_precision.configurable_activation_quantizer import \
+    ConfigurableActivationQuantizer
+from model_compression_toolkit.core.keras.mixed_precision.configurable_weights_quantizer import \
+    ConfigurableWeightsQuantizer
+
+from model_compression_toolkit.exporter.model_wrapper.keras.builder.node_to_quantizer import \
+    get_inferable_quantizer_kwargs
+
+from model_compression_toolkit.logger import Logger
+from model_compression_toolkit.core import common
+from model_compression_toolkit.core.common.framework_info import FrameworkInfo
+from model_compression_toolkit.core.keras.default_framework_info import DEFAULT_KERAS_INFO
 
 
-class PytorchMixedPrecisionWrapper(torch.nn.Module):
+class MixedPrecisionKerasModelBuilder(KerasModelBuilder):
     """
-    Class that wraps a Pytorch layer (nn.Module) to be used for mixed precision quantization.
-    Allows to maintain quantized weights tensors for each of the layer's attributes that we want to quantize,
-    and a list of activation quantizers for each quantization candidate,
-    for each of the candidate bitwidth options specified for the mixed precision model.
-    During MP search, it allows to activate the relevant quantized weights tensor and activation quantizer
-    according to a given configuration, and use it for inference.
+    Builder of mixed-precision Keras models.
     """
+
     def __init__(self,
-                 n: BaseNode,
-                 fw_info: FrameworkInfo):
+                 graph: common.Graph,
+                 append2output=None,
+                 fw_info: FrameworkInfo = DEFAULT_KERAS_INFO,
+                 return_float_outputs: bool = False):
         """
-        Construct a Pytorch model that constitutes as a wrapper for a Pytorch layer, built from a given graph node.
+
         Args:
-            n: Node to build its Pytorch layer.
-            fw_info: Framework information (e.g., mapping from layers to their attributes to quantize).
+            graph: Graph to build the model from.
+            append2output: Nodes to append to model's output.
+            fw_info: Information about the specific framework of the model that is built.
+            return_float_outputs: Whether the model returns float tensors or not.
+        """
+
+        self.graph = graph
+
+        super().__init__(graph,
+                         append2output,
+                         fw_info,
+                         return_float_outputs,
+                         wrapper=self.mixed_precision_wrapper,
+                         get_activation_quantizer_holder_fn=self.mixed_precision_activation_holder)
+
+    def mixed_precision_wrapper(self,
+                                n: common.BaseNode,
+                                layer: Layer) -> Union[KerasQuantizationWrapper, Layer]:
         """
-        super(PytorchMixedPrecisionWrapper, self).__init__()
+        A function which takes a computational graph node and a keras layer and perform the quantization
+        wrapping for mixed precision.
 
-        assert n.candidates_quantization_cfg is not None
-        self.node_q_cfg = n.candidates_quantization_cfg
-        if isinstance(n, FunctionalNode):
-            self.layer = n.type
-        else:
-            framework_attr = copy.copy(n.framework_attr)
-            self.layer = n.type(**framework_attr)
+        Args:
+            n: A node of mct graph.
+            layer: A keras layer
+
+        Returns: Wrapped layer with a configurable quantizer if the layer should quantized in mixed precision,
+        otherwise returns either the layer wrapped with a fixed precision inferable quantizer or the layer as is if it's
+        not supposed to be quantized.
+
+        """
+
+        weights_conf_nodes_names = [n.name for n in self.graph.get_weights_configurable_nodes()]
+
+        if n.is_weights_quantization_enabled():
+            kernel_attributes = self.fw_info.get_kernel_op_attributes(n.type)
+            if n.name in weights_conf_nodes_names:
+                return KerasQuantizationWrapper(layer,
+                                                weights_quantizers={attr: ConfigurableWeightsQuantizer(
+                                                    **self._get_weights_configurable_quantizer_kwargs(n, attr))
+                                                                    for attr in kernel_attributes})
+            else:
+                node_weights_qc = n.get_unique_weights_candidates()
+                if not len(node_weights_qc) == 1:
+                    Logger.error(f"Expecting node {n.name} to have a unique weights configuration "  # pragma: no cover
+                                 f"but {len(node_weights_qc)} different configurations exist.")
+
+                quantier_for_node = get_inferable_quantizer_class(QuantizationTarget.Weights,
+                                                                  node_weights_qc[0].weights_quantization_cfg.weights_quantization_method,
+                                                                  BaseKerasInferableQuantizer)
+                kwargs = get_inferable_quantizer_kwargs(node_weights_qc[0].weights_quantization_cfg,
+                                                        QuantizationTarget.Weights)
+
+                return KerasQuantizationWrapper(layer,
+                                                weights_quantizers={attr: quantier_for_node(**kwargs)
+                                                                    for attr in kernel_attributes})
 
-        for qc in self.node_q_cfg:
-            assert qc.weights_quantization_cfg.enable_weights_quantization == \
-                   self.node_q_cfg[0].weights_quantization_cfg.enable_weights_quantization \
-                   and qc.activation_quantization_cfg.enable_activation_quantization == \
-                   self.node_q_cfg[0].activation_quantization_cfg.enable_activation_quantization, \
-                "Candidates with different weights/activation enabled properties is currently not supported"
-
-        self.enable_weights_quantization = \
-            self.node_q_cfg[0].weights_quantization_cfg.enable_weights_quantization and \
-            not n.is_all_weights_candidates_equal()
-        self.enable_activation_quantization = \
-            self.node_q_cfg[0].activation_quantization_cfg.enable_activation_quantization and \
-            not n.is_all_activation_candidates_equal()
+        return layer
+
+    def _get_weights_configurable_quantizer_kwargs(self, n: BaseNode, attr: str) -> Dict[str, Any]:
+        """
+        Get the quantization parameters for a configurable quantizer.
+
+        Args:
+            n: The node for which the quantizer is being created.
+            attr: The name of the weights attribute to be quantized.
+
+        Returns:
+            The quantization parameters as a dictionary.
+        """
+
+        assert n.candidates_quantization_cfg is not None, f"Node {n.name} candidates_quantization_cfg is None"
+        node_q_cfg_candidates = n.candidates_quantization_cfg
+        # sort by descending bit width so using indices would be easier
+        node_q_cfg_candidates.sort(key=lambda x: (x.weights_quantization_cfg.weights_n_bits,
+                                                  x.activation_quantization_cfg.activation_n_bits), reverse=True)
+
+        float_weights = n.get_weights_by_keys(attr)
 
         max_cfg_candidates = n.find_max_candidates_indices()
-        assert len(max_cfg_candidates) == 1, \
-            f"A maximal config candidate must be defined, but some node have multiple potential maximal candidates"
+        if not len(max_cfg_candidates) == 1:
+            Logger.error(f"A maximal config candidate must be defined, "  # pragma: no cover
+                         f"but some node have multiple potential maximal candidates")
+
         max_candidate_idx = max_cfg_candidates[0]
 
-        if not isinstance(n, FunctionalNode):
-            # loading the weights (if exists) from the graph node (weights of the trained model)
-            self.layer.load_state_dict({k: torch.Tensor(v) for k, v in n.weights.items()}, strict=False)
-            set_model(self.layer)
-
-        # Setting layers' weights
-        if self.enable_weights_quantization:
-            self.weight_attrs = fw_info.get_kernel_op_attributes(n.type)
-            # float_weights is a list of weights for each attribute that we want to quantize.
-            self.float_weights = [n.get_weights_by_keys(attr) for attr in
-                                  self.weight_attrs]
-
-            assert len(self.weight_attrs) == len(self.float_weights)
-            self.weights_quantizer_fn_list = [qc.weights_quantization_cfg.weights_quantization_fn
-                                              for qc in self.node_q_cfg]
-            self.quantized_weights = self._get_quantized_weights()
-            # Setting the model with the initial quantized weights (the highest precision)
-            self.set_active_weights(bitwidth_idx=max_candidate_idx)
-
-        # Setting layer's activation
-        if self.enable_activation_quantization:
-            self.activation_quantizers = self._get_activation_quantizers()
-            self.activation_bitwidth_idx = max_candidate_idx
+        return {'node_q_cfg': node_q_cfg_candidates,
+                'float_weights': float_weights,
+                'max_candidate_idx': max_candidate_idx
+                }
+
+    def mixed_precision_activation_holder(self, n: BaseNode) -> KerasActivationQuantizationHolder:
+        """
+        Retrieve a KerasActivationQuantizationHolder layer to use for activation quantization for a node.
+        The layer should hold either a configurable activation quantizer, if it is quantized with mixed precision,
+        or an inferable quantizer for fixed single bit-width quantization.
 
-    def forward(self, x: Any, *args: Any, **kwargs: Any) -> Any:
-        """
         Args:
-            x: input tensors to layer.
+            n: Node to get KerasActivationQuantizationHolder to attach in its output.
+
         Returns:
-            torch Tensor which is the output of the wrapped layer on the given input.
+            A KerasActivationQuantizationHolder layer for the node activation quantization.
         """
-        outputs = self.layer(x, *args, **kwargs)
 
-        if self.enable_activation_quantization:
-            # add fake quant to quantize activations with the active number of bits
-            if isinstance(outputs, list):
-                # we assume here that it can't be multiple outputs out of a quantized layer.
-                # We are not expecting to get here since we call this wrapper layer op only through the
-                # sensitivity evaluation inference pytorch method which unfolds the input list to separate arguments.
-                # But, in order to prevent possible issues (if someone will use this wrapper otherwise,
-                # we keep this line which handles an input as list, and exclude it from the test coverage report.
-                assert len(outputs) == 1, "Activation quantization for node with multiple outputs is not supported."  # pragma: no cover
-                outputs = torch.cat(outputs, dim=0)  # pragma: no cover
-
-            outputs = self.activation_quantizers[self.activation_bitwidth_idx](outputs)
-
-        return outputs
-
-    def _get_quantized_weights(self):
-        """
-        Calculates the quantized weights' tensors for each of the bitwidth candidates for quantization,
-        to be stored and used during MP search.
-        Returns: a list of quantized weights - for each bitwidth and layer's attribute to be quantized.
-        """
-        quantized_weights = []
-        for index, qc in enumerate(self.node_q_cfg):
-            # for each quantization configuration in mixed precision
-            # get quantized weights for each attribute and for each filter
-            quantized_per_attr = []
-            for float_weight in self.float_weights:
-                # for each attribute
-                quantized_per_attr.append(self.weights_quantizer_fn_list[index](tensor_data=float_weight,
-                                                                                n_bits=qc.weights_quantization_cfg.weights_n_bits,
-                                                                                signed=True,
-                                                                                quantization_params=qc.weights_quantization_cfg.weights_quantization_params,
-                                                                                per_channel=qc.weights_quantization_cfg.weights_per_channel_threshold,
-                                                                                output_channels_axis=qc.weights_quantization_cfg.weights_channels_axis))
-            quantized_weights.append(quantized_per_attr)
+        activation_conf_nodes_names = [n.name for n in self.graph.get_activation_configurable_nodes()]
 
-        return quantized_weights
+        activation_quantizers = []
+        if n.is_activation_quantization_enabled():
+            num_of_outputs = len(n.output_shape) if isinstance(n.output_shape, list) else 1
+            if n.name in activation_conf_nodes_names:
+                assert n.candidates_quantization_cfg is not None, f"Node {n.name} candidates_quantization_cfg is None"
+                node_q_cfg_candidates = n.candidates_quantization_cfg
+                # sort by descending bit width so using indices would be easier
+                node_q_cfg_candidates.sort(key=lambda x: (x.weights_quantization_cfg.weights_n_bits,
+                                                          x.activation_quantization_cfg.activation_n_bits),
+                                           reverse=True)
+
+                max_cfg_candidates = n.find_max_candidates_indices()
+                assert len(max_cfg_candidates) == 1, \
+                    f"A maximal config candidate must be defined, but some node have multiple potential maximal candidates"
+                max_candidate_idx = max_cfg_candidates[0]
+
+                activation_quantizers = [ConfigurableActivationQuantizer(**{'node_q_cfg': node_q_cfg_candidates,
+                                                                            'max_candidate_idx': max_candidate_idx})] \
+                                        * num_of_outputs
+            else:
+                node_act_qc = n.get_unique_activation_candidates()
+                assert len(node_act_qc) == 1, f"Expecting node {n.name} to have a unique activation configuration, " \
+                                              f"but {len(node_act_qc)} different configurations exist."
+                quantizer_for_node = get_inferable_quantizer_class(QuantizationTarget.Activation,
+                                                                   node_act_qc[0].activation_quantization_cfg.activation_quantization_method,
+                                                                   BaseKerasInferableQuantizer)
+                kwargs = get_inferable_quantizer_kwargs(node_act_qc[0].activation_quantization_cfg,
+                                                        QuantizationTarget.Activation)
+
+                activation_quantizers = [quantizer_for_node(**kwargs)] * num_of_outputs
+
+        # Holder by definition uses a single quantizer for the activation quantization
+        # thus we make sure this is the only possible case (unless it's a node with no activation
+        # quantization, which in this case has an empty list).
+        if len(activation_quantizers) == 1:
+            return KerasActivationQuantizationHolder(activation_quantizers[0])
+
+        Logger.error(f'KerasActivationQuantizationHolder supports a single quantizer but '  # pragma: no cover
+                     f'{len(activation_quantizers)} quantizers were found for node {n}')
+
+    def build_model(self) -> Tuple[Model, UserInformation,
+                                   Dict[str, Union[KerasQuantizationWrapper, KerasActivationQuantizationHolder]]]:
+        """
+        Build a Keras mixed-precision model and return it.
+        Used the basic Keras model builder to build the model, and adding a mapping between each configurable node to
+        a list of layers (from the new model) that are matching to the node (either KerasQuantizationWrapper or
+        KerasActivationQuantizationHolder type layers).
+        This mapping is used during mixed precision metric computation to enforce pairs of weights-activation bit-width
+        candidates when configuring a model.
+
+        Returns: Mixed-precision Keras model.
+
+        """
+        model, user_info = super().build_model()
+
+        # creating a mapping between graph nodes and model's layers for mixed precision configurability
+        conf_node2layers = {n.name: self._find_layers_in_model_by_node(n, model.layers)
+                            for n in self.graph.get_configurable_sorted_nodes()}
+
+        return model, user_info, conf_node2layers
 
-    def _get_activation_quantizers(self) -> List[Any]:
+    @staticmethod
+    def _get_weights_quant_layers(n: BaseNode, layers_list: List[Layer]) -> List[KerasQuantizationWrapper]:
         """
-        Builds a list of quantizers for each of the bitwidth candidates for activation quantization,
-        to be stored and used during MP search.
+        Filters KerasQuantizationWrapper layers from an MP model that are matching to the given graph node.
+
+        Args:
+            n: A configurable graph node.
+            layers_list: Mixed precision model layers list.
+
+        Returns: A list of layers that responsible for the node's weights quantization.
 
-        Returns: a list of activation quantizers - for each bitwidth and layer's attribute to be quantized.
         """
-        activation_quantizers = []
-        for index, qc in enumerate(self.node_q_cfg):
-            q_activation = self.node_q_cfg[index].activation_quantization_cfg
-            activation_quantizers.append(q_activation.quantize_node_output)
-
-        return activation_quantizers
-
-    def set_active_weights(self,
-                           bitwidth_idx: int,
-                           attr: str = None):
-        """
-        Set a weights' tensor to use by the layer wrapped by the module.
-        Args:
-            bitwidth_idx: Index of a candidate quantization configuration to use its quantized
-            version of the float weight.
-            attr: Attributes of the layer's weights to quantize
-        """
-        if self.enable_weights_quantization:
-            if attr is None:  # set bit width to all weights of the layer
-                attr_idxs = [attr_idx for attr_idx in range(len(self.quantized_weights[bitwidth_idx]))]
-                self._set_weights_bit_width_index(bitwidth_idx, attr_idxs)
-            else:  # set bit width to a specific attribute
-                attr_idx = self.weight_attrs.index(attr)
-                self._set_weights_bit_width_index(bitwidth_idx, [attr_idx])
-
-    def set_active_activation_quantizer(self,
-                                        bitwidth_idx: int):
-        """
-        Set an activation quantizer to use by the layer wrapped by the module.
-
-        Args:
-            bitwidth_idx: Index of a candidate quantization configuration to use its quantizer
-            for quantizing the activation.
-        """
-        if self.enable_activation_quantization:
-            self.activation_bitwidth_idx = bitwidth_idx
-
-    def _set_weights_bit_width_index(self,
-                                     bitwidth_idx: int,
-                                     attr_idxs: List[int]):
-        """
-        Sets the wrapped layer's weights state with quantized weights, according to the given configuration.
-        Args:
-            bitwidth_idx: Index of a candidate quantization configuration to use its quantized
-            version of the float weight.
-            attr_idxs: Indices list of attributes of the layer's weights to quantize
-        Returns: None (sets the new state of the layer inplace).
-        """
-        assert bitwidth_idx < len(self.quantized_weights), \
-            f"Index {bitwidth_idx} does not exist in current quantization candidates list"
-
-        loaded_weights = {k: torch.as_tensor(v) for k, v in self.layer.state_dict().items()}
-        with torch.no_grad():
-            for attr_idx in attr_idxs:
-                # need to prepare the weights' tensor - extract it from the maintained quantized_weights list
-                # and move it to the relevant device as the wrapped layer's weights.
-                weights_tensor = self.quantized_weights[bitwidth_idx][attr_idx]
-                weights_device = loaded_weights[self.weight_attrs[attr_idx]].device
-                active_weights = torch.nn.Parameter(torch.from_numpy(weights_tensor).to(weights_device))
-                loaded_weights[self.weight_attrs[attr_idx]] = active_weights
-            self.layer.load_state_dict(loaded_weights, strict=True)
+        return [_l for _l in layers_list if isinstance(_l, KerasQuantizationWrapper) and _l.layer.name == n.name]
+
+    @staticmethod
+    def _get_activation_quant_layers(n: BaseNode, layers_list: List[Layer]) -> List[KerasActivationQuantizationHolder]:
+        """
+        Filters KerasActivationQuantizationHolder layers from an MP model that are matching to the given graph node.
+
+        Args:
+            n: A configurable graph node.
+            layers_list: Mixed precision model layers list.
+
+        Returns: A list of layers that responsible for the node's activation quantization.
+
+        """
+        return [_l for _l in layers_list if isinstance(_l, KerasActivationQuantizationHolder)
+                and (_l.inbound_nodes[0].inbound_layers.name == n.name or
+                     (isinstance(_l.inbound_nodes[0].inbound_layers, KerasQuantizationWrapper) and
+                      _l.inbound_nodes[0].inbound_layers.layer.name == n.name))]
+
+    def _find_layers_in_model_by_node(self, n: BaseNode, layers_list: List[Layer]) -> \
+            List[Union[KerasQuantizationWrapper, KerasActivationQuantizationHolder]]:
+        """
+        Retries layers from an MP model that are matching to the given graph node, that is, this are either
+        KerasQuantizationWrapper layers or KerasActivationQuantizationHolder layers that are responsible for the graph
+        configurable model quantization.
+
+        Args:
+            n: A configurable graph node.
+            layers_list: Mixed precision model layers list.
+
+        Returns: A list of layers that responsible for the node's quantization.
+
+        """
+        weights_quant = n.is_weights_quantization_enabled()
+        act_quant = n.is_activation_quantization_enabled()
+
+        if weights_quant and not act_quant:
+            return self._get_weights_quant_layers(n, layers_list)
+        elif not weights_quant and act_quant:
+            return self._get_activation_quant_layers(n, layers_list)
+        elif weights_quant and act_quant:
+            return self._get_weights_quant_layers(n, layers_list) + self._get_activation_quant_layers(n, layers_list)
+        else:
+            Logger.error(f"Expects node {n.name} to have at either weights or activation quantization configured,"  # pragma: no cover
+                         f"but both are disabled.")
+
```

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/pytorch/pytorch_implementation.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/pytorch/pytorch_implementation.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,31 +10,34 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 import operator
 from copy import deepcopy
+from functools import partial
 from typing import List, Any, Tuple, Callable, Type, Dict
 
 import numpy as np
 import torch
+from mct_quantizers import PytorchQuantizationWrapper, PytorchActivationQuantizationHolder
 from torch import sigmoid, softmax, add, cat, argmax
 from torch.nn import Conv2d, ConvTranspose2d, Linear
 from torch.nn import Module, Sigmoid, Softmax
 
 import model_compression_toolkit.core.pytorch.constants as pytorch_constants
 from model_compression_toolkit.core import QuantizationConfig, FrameworkInfo, CoreConfig, MixedPrecisionQuantizationConfigV2
 from model_compression_toolkit.core import common
 from model_compression_toolkit.core.common import Graph, BaseNode
 from model_compression_toolkit.core.common.collectors.statistics_collector import BaseStatsCollector
 from model_compression_toolkit.core.common.collectors.statistics_collector_generator import \
     create_stats_collector_for_node
 from model_compression_toolkit.core.common.framework_implementation import FrameworkImplementation
 from model_compression_toolkit.core.common.mixed_precision.sensitivity_evaluation import SensitivityEvaluation
+from model_compression_toolkit.core.common.mixed_precision.set_layer_to_bitwidth import set_layer_to_bitwidth
 from model_compression_toolkit.core.common.model_builder_mode import ModelBuilderMode
 from model_compression_toolkit.core.common.node_prior_info import NodePriorInfo
 from model_compression_toolkit.core.common.similarity_analyzer import compute_mse, compute_kl_divergence, compute_cs
 from model_compression_toolkit.core.common.user_info import UserInformation
 from model_compression_toolkit.core.pytorch.back2framework import get_pytorch_model_builder
 from model_compression_toolkit.core.pytorch.back2framework.model_gradients import \
     pytorch_iterative_approx_jacobian_trace
@@ -66,25 +69,28 @@
     pytorch_apply_shift_negative_correction
 from model_compression_toolkit.core.pytorch.graph_substitutions.substitutions.softmax_shift import \
     pytorch_softmax_shift
 from model_compression_toolkit.core.pytorch.graph_substitutions.substitutions.virtual_activation_weights_composition import \
     VirtualActivationWeightsComposition
 from model_compression_toolkit.core.pytorch.graph_substitutions.substitutions.weights_activation_split import \
     WeightsActivationSplit
-from model_compression_toolkit.core.pytorch.mixed_precision.set_layer_to_bitwidth import set_layer_to_bitwidth
+from model_compression_toolkit.core.pytorch.mixed_precision.configurable_activation_quantizer import \
+    ConfigurableActivationQuantizer
+from model_compression_toolkit.core.pytorch.mixed_precision.configurable_weights_quantizer import \
+    ConfigurableWeightsQuantizer
 from model_compression_toolkit.core.pytorch.pytorch_node_prior_info import create_node_prior_info
 from model_compression_toolkit.core.pytorch.reader.reader import model_reader
 from model_compression_toolkit.core.pytorch.statistics_correction.apply_second_moment_correction import \
     pytorch_apply_second_moment_correction
 from model_compression_toolkit.core.pytorch.utils import to_torch_tensor, torch_tensor_to_numpy, set_model
 
 
 class PytorchImplementation(FrameworkImplementation):
     """
-    An class with implemented methods to support optimizing Pytorch models.
+    A class with implemented methods to support optimizing Pytorch models.
     """
 
     def __init__(self):
         super().__init__()
 
     @property
     def constants(self):
@@ -130,29 +136,29 @@
         return model_reader(_module, representative_data_gen, self.to_numpy, self.to_tensor)
 
     def model_builder(self,
                       graph: Graph,
                       mode: ModelBuilderMode,
                       append2output: List[Any] = None,
                       fw_info: FrameworkInfo = DEFAULT_PYTORCH_INFO,
-                      return_float_outputs: bool = False) -> Tuple[Module, UserInformation]:
+                      return_float_outputs: bool = False) -> Tuple:
         """
         Build a Pytorch module from a graph.
         The mode determines how the module should be build. append2output is a list of Nodes
         to set as the module outputs.
 
         Args:
             graph: Graph to build the module from it.
             mode: Mode for how to build the module.
             append2output: List of Nodes to set as the module's outputs.
             fw_info: FrameworkInfo object with information about the specific framework's module
             return_float_outputs (bool): whether to return outputs before or after quantization nodes (default)
 
         Returns:
-            A tuple of the Pytorch module that was built and an UserInformation object.
+            A tuple with the model and additional relevant supporting objects.
         """
         pytorch_model_builder = get_pytorch_model_builder(mode)
         return pytorch_model_builder(graph=graph,
                                      append2output=append2output,
                                      fw_info=fw_info,
                                      return_float_outputs=return_float_outputs).build_model()
 
@@ -346,16 +352,19 @@
         """
 
         return SensitivityEvaluation(graph=graph,
                                      quant_config=quant_config,
                                      representative_data_gen=representative_data_gen,
                                      fw_info=fw_info,
                                      fw_impl=self,
-                                     set_layer_to_bitwidth=set_layer_to_bitwidth,
-                                     get_quant_node_name=lambda node_name: f'{node_name}',
+                                     set_layer_to_bitwidth=partial(set_layer_to_bitwidth,
+                                                                   weights_quantizer_type=ConfigurableWeightsQuantizer,
+                                                                   activation_quantizer_type=ConfigurableActivationQuantizer,
+                                                                   weights_quant_layer_type=PytorchQuantizationWrapper,
+                                                                   activation_quant_layer_type=PytorchActivationQuantizationHolder),
                                      disable_activation_for_metric=disable_activation_for_metric)
 
     def get_node_prior_info(self,
                             node: BaseNode,
                             fw_info: FrameworkInfo,
                             graph: Graph) -> NodePriorInfo:
         """
@@ -407,44 +416,14 @@
             return compute_kl_divergence
         elif layer_class in [Sigmoid, sigmoid]:
             return compute_cs
         elif layer_class == Linear:
             return compute_cs
         return compute_mse
 
-    def get_model_layers_names(self,
-                               model: Module) -> List[str]:
-        """
-        Returns a list of the given model's layers names.
-
-        Args:
-            model: A Pytorch model.
-
-        Returns: List of layers' names.
-
-        """
-
-        return [layer[0] for layer in list(model.named_children())]
-
-    def get_model_layer_by_name(self,
-                                model: Module,
-                                layer_name: str) -> Module:
-        """
-        Returns a Pytorch model's layer by its name.
-
-        Args:
-            model: A Pytorch model to retrieve a layer from.
-            layer_name: The requested layer's name.
-
-        Returns: A Pytorch layer object.
-
-        """
-
-        return model.get_submodule(target=layer_name)
-
     def model_grad(self,
                    graph_float: common.Graph,
                    model_input_tensors: Dict[BaseNode, torch.Tensor],
                    interest_points: List[BaseNode],
                    output_list: List[BaseNode],  # dummy - not used in pytorch
                    all_outputs_indices: List[int],
                    alpha: float = 0.3,
```

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/pytorch/pytorch_node_prior_info.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/pytorch/pytorch_node_prior_info.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/pytorch/quantizer/__init__.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/pytorch/quantizer/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/pytorch/quantizer/fake_quant_builder.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/pytorch/quantizer/fake_quant_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/pytorch/quantizer/lut_fake_quant.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/pytorch/quantizer/lut_fake_quant.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/pytorch/reader/__init__.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/pytorch/reader/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/pytorch/reader/graph_builders.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/pytorch/reader/graph_builders.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/pytorch/reader/node_holders.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/pytorch/reader/node_holders.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/pytorch/reader/reader.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/pytorch/reader/reader.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/pytorch/statistics_correction/__init__.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/pytorch/statistics_correction/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/pytorch/statistics_correction/apply_second_moment_correction.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/pytorch/statistics_correction/apply_second_moment_correction.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/pytorch/utils.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/pytorch/utils.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/core/runner.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/runner.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/exporter/__init__.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/exporter/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/exporter/model_exporter/__init__.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/exporter/model_exporter/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/exporter/model_exporter/fw_agonstic/__init__.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/exporter/model_exporter/fw_agonstic/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/exporter/model_exporter/fw_agonstic/exporter.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/exporter/model_exporter/fw_agonstic/exporter.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/exporter/model_exporter/keras/__init__.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/exporter/model_exporter/keras/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/exporter/model_exporter/keras/base_keras_exporter.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/exporter/model_exporter/keras/base_keras_exporter.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/exporter/model_exporter/keras/export_serialization_format.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/exporter/model_exporter/keras/export_serialization_format.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/exporter/model_exporter/keras/fakely_quant_keras_exporter.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/exporter/model_exporter/keras/fakely_quant_keras_exporter.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/exporter/model_exporter/keras/fakely_quant_tflite_exporter.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/exporter/model_exporter/keras/fakely_quant_tflite_exporter.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/exporter/model_exporter/keras/int8_tflite_exporter.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/exporter/model_exporter/keras/int8_tflite_exporter.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/exporter/model_exporter/keras/keras_export_facade.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/exporter/model_exporter/keras/keras_export_facade.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/exporter/model_exporter/pytorch/__init__.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/exporter/model_exporter/pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/exporter/model_exporter/pytorch/base_pytorch_exporter.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/exporter/model_exporter/pytorch/base_pytorch_exporter.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/exporter/model_exporter/pytorch/export_serialization_format.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/exporter/model_exporter/pytorch/export_serialization_format.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/exporter/model_exporter/pytorch/fakely_quant_onnx_pytorch_exporter.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/exporter/model_exporter/pytorch/fakely_quant_onnx_pytorch_exporter.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/exporter/model_exporter/pytorch/fakely_quant_torchscript_pytorch_exporter.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/exporter/model_exporter/pytorch/fakely_quant_torchscript_pytorch_exporter.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/exporter/model_exporter/pytorch/pytorch_export_facade.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/exporter/model_exporter/pytorch/pytorch_export_facade.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/exporter/model_wrapper/__init__.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/exporter/model_wrapper/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/exporter/model_wrapper/keras/__init__.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/exporter/model_wrapper/keras/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/exporter/model_wrapper/keras/builder/__init__.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/exporter/model_wrapper/keras/builder/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/exporter/model_wrapper/keras/builder/fully_quantized_model_builder.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/exporter/model_wrapper/keras/builder/fully_quantized_model_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/exporter/model_wrapper/keras/builder/node_to_quantizer.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/exporter/model_wrapper/keras/builder/node_to_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/exporter/model_wrapper/keras/builder/node_to_quantizers.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/exporter/model_wrapper/keras/builder/node_to_quantizers.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/exporter/model_wrapper/keras/validate_layer.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/exporter/model_wrapper/keras/validate_layer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/exporter/model_wrapper/pytorch/__init__.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/exporter/model_wrapper/pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/exporter/model_wrapper/pytorch/builder/__init__.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/exporter/model_wrapper/pytorch/builder/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/exporter/model_wrapper/pytorch/builder/fully_quantized_model_builder.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/exporter/model_wrapper/pytorch/builder/fully_quantized_model_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/exporter/model_wrapper/pytorch/builder/node_to_quantizer.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/exporter/model_wrapper/pytorch/builder/node_to_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/exporter/model_wrapper/pytorch/builder/node_to_quantizers.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/exporter/model_wrapper/pytorch/builder/node_to_quantizers.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/exporter/model_wrapper/pytorch/validate_layer.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/exporter/model_wrapper/pytorch/validate_layer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/gptq/__init__.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/gptq/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/gptq/common/__init__.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/gptq/common/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/gptq/common/gptq_config.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/gptq/common/gptq_config.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/gptq/common/gptq_constants.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/gptq/common/gptq_constants.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/gptq/common/gptq_framework_implementation.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/gptq/common/gptq_framework_implementation.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/gptq/common/gptq_graph.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/gptq/common/gptq_graph.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/gptq/common/gptq_training.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/gptq/common/gptq_training.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/gptq/keras/__init__.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/gptq/keras/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/gptq/keras/gptq_keras_implementation.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/gptq/keras/gptq_keras_implementation.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/gptq/keras/gptq_loss.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/gptq/keras/gptq_loss.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/gptq/keras/gptq_training.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/gptq/keras/gptq_training.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/gptq/keras/graph_info.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/gptq/keras/graph_info.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/gptq/keras/quantization_facade.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/gptq/keras/quantization_facade.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/gptq/keras/quantizer/__init__.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/gptq/keras/quantizer/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/gptq/keras/quantizer/base_keras_gptq_quantizer.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/gptq/keras/quantizer/base_keras_gptq_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/gptq/keras/quantizer/quant_utils.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/gptq/keras/quantizer/quant_utils.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/gptq/keras/quantizer/quantization_builder.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/gptq/keras/quantizer/quantization_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/gptq/keras/quantizer/regularization_factory.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/gptq/keras/quantizer/regularization_factory.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/__init__.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/soft_quantizer_reg.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/soft_quantizer_reg.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/symmetric_soft_quantizer.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/symmetric_soft_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/uniform_soft_quantizer.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/uniform_soft_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/gptq/keras/quantizer/ste_rounding/__init__.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/gptq/keras/quantizer/ste_rounding/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/gptq/keras/quantizer/ste_rounding/symmetric_ste.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/gptq/pytorch/quantizer/ste_rounding/symmetric_ste.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,49 +1,50 @@
-# Copyright 2021 Sony Semiconductor Israel, Inc. All rights reserved.
+# Copyright 2023 Sony Semiconductor Israel, Inc. All rights reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
-
-from typing import Dict, Any
-
+import torch
+import torch.nn as nn
+from typing import Dict
 import numpy as np
-import tensorflow as tf
+from model_compression_toolkit.core.common.defaultdict import DefaultDict
 
-from model_compression_toolkit.gptq import RoundingType
 from model_compression_toolkit.target_platform_capabilities.target_platform import QuantizationMethod
-from mct_quantizers import QuantizationTarget
-from model_compression_toolkit.gptq.common.gptq_constants import AUXVAR, PTQ_THRESHOLD
-from model_compression_toolkit.gptq.keras.quantizer import quant_utils as qutils
+from mct_quantizers import QuantizationTarget, PytorchQuantizationWrapper
+from model_compression_toolkit.gptq.common.gptq_config import RoundingType
+from model_compression_toolkit.gptq.pytorch.quantizer.base_pytorch_gptq_quantizer import \
+    BasePytorchGPTQTrainableQuantizer
+from model_compression_toolkit.core.pytorch.utils import to_torch_tensor, torch_tensor_to_numpy
+from model_compression_toolkit.gptq.pytorch.quantizer import quant_utils as qutils
+from model_compression_toolkit.gptq.common.gptq_constants import AUXVAR, PTQ_THRESHOLD, MAX_LSB_CHANGE
 from model_compression_toolkit.constants import THRESHOLD
-from model_compression_toolkit.core.common.defaultdict import DefaultDict
-from model_compression_toolkit.gptq.keras.quantizer.base_keras_gptq_quantizer import BaseKerasGPTQTrainableQuantizer
 from model_compression_toolkit.trainable_infrastructure import TrainableQuantizerWeightsConfig
 from mct_quantizers import mark_quantizer
+from model_compression_toolkit.trainable_infrastructure.common.base_trainable_quantizer import VariableGroup
 from model_compression_toolkit.trainable_infrastructure.common.quant_utils import \
     get_threshold_reshape_shape
-from model_compression_toolkit.trainable_infrastructure.common.base_trainable_quantizer import VariableGroup
 
 
-def pertubation_symmetric_quantizer(input_tensor: tf.Tensor,
-                                    auxvar_tensor: tf.Variable,
-                                    max_tensor: tf.Tensor,
+def pertubation_symmetric_quantizer(input_tensor: torch.Tensor,
+                                    auxvar_tensor: nn.Parameter,
+                                    max_tensor: torch.Tensor,
                                     num_bits: int,
                                     signed: bool,
                                     power_of_two: bool,
-                                    max_lsbs_change: int = 1) -> tf.Tensor:
+                                    max_lsbs_change: int = MAX_LSB_CHANGE) -> nn.Parameter:
     """
     Quantize a tensor symmetrically with maximum LSBs shift.
 
     Args:
         input_tensor: Tensor to quantize. values of this tensor are not changed during gptq.
         auxvar_tensor: Tensor that manifests the bit shift the weight due to gptq
         max_tensor: Tensor with max values to compute the threshold.
@@ -55,106 +56,118 @@
     Returns:
         A quantized tensor.
     """
 
     if power_of_two:
         max_tensor = qutils.power_of_two_max(max_tensor)
     delta = qutils.calculate_delta(max_tensor, num_bits, signed)
-    input_tensor_int = tf.stop_gradient(tf.round(input_tensor / delta))
-    tensor_q = qutils.ste_round(
-        input_tensor_int + qutils.ste_clip(auxvar_tensor, max_val=max_lsbs_change * delta) / delta)
+    delta = to_torch_tensor(delta)
+    max_tensor_change = delta * max_lsbs_change
+
     min_int = -int(signed) * (2 ** (num_bits - int(signed)))
     max_int = (2 ** (num_bits - int(signed))) - 1
+
+    tensor_clipped = qutils.ste_clip(auxvar_tensor, min_val=-max_tensor_change, max_val=max_tensor_change) / delta
+    input_tensor_int = torch.round(input_tensor / delta).detach()
+
+    tensor_q = qutils.ste_round(qutils.ste_round(input_tensor_int + tensor_clipped))
+
     return delta * qutils.ste_clip(tensor_q, max_val=max_int, min_val=min_int)
 
 
 @mark_quantizer(quantization_target=QuantizationTarget.Weights,
                 quantization_method=[QuantizationMethod.POWER_OF_TWO, QuantizationMethod.SYMMETRIC],
                 quantizer_type=RoundingType.STE)
-class STEWeightGPTQQuantizer(BaseKerasGPTQTrainableQuantizer):
+class STEWeightGPTQQuantizer(BasePytorchGPTQTrainableQuantizer):
     """
     Trainable symmetric quantizer to quantize a layer weights.
     """
 
     def __init__(self,
                  quantization_config: TrainableQuantizerWeightsConfig,
                  max_lsbs_change_map: dict = DefaultDict({}, lambda: 1)):
         """
-        Initialize a STEWeightGPTQQuantizer object with parameters to use for the quantization.
+        Construct a Pytorch model that utilize a fake weight quantizer of STE (Straight Through Estimator) for symmetric quantizer.
 
         Args:
             quantization_config: Trainable weights quantizer config.
-            max_lsbs_change_map: a mapping between number of bits to max lsb change.
         """
         super().__init__(quantization_config)
         self.num_bits = quantization_config.weights_n_bits
         self.per_channel = quantization_config.weights_per_channel_threshold
 
         threshold_values = quantization_config.weights_quantization_params[THRESHOLD]
         self.threshold_shape = np.asarray(threshold_values).shape
         self.threshold_values = np.reshape(np.asarray(threshold_values), [-1]) if self.per_channel else float(
             threshold_values)
 
         self.quantization_axis = quantization_config.weights_channels_axis
         self.power_of_two = quantization_config.weights_quantization_method == QuantizationMethod.POWER_OF_TWO
         self.max_lsbs_change = max_lsbs_change_map.get(self.num_bits)
 
+
     def initialize_quantization(self,
-                                tensor_shape: Any,
+                                tensor_shape: torch.Size,
                                 name: str,
-                                layer: Any):
+                                layer: PytorchQuantizationWrapper):
         """
         Add quantizer parameters to the quantizer parameters dictionary
 
         Args:
             tensor_shape: tensor shape of the quantized tensor.
             name: Tensor name.
             layer: Layer to quantize.
         """
 
-        ptq_threshold_tensor = layer.add_weight(
-            f"{name}_{PTQ_THRESHOLD}",
-            shape=len(self.threshold_values) if self.per_channel else (),
-            initializer=tf.keras.initializers.Constant(1.0),
-            trainable=False)
-        ptq_threshold_tensor.assign(self.threshold_values)
-
-        w = getattr(layer.layer, name)
-        auxvar_tensor = layer.add_weight(
-            f"{name}_{AUXVAR}",
-            shape=list(w.shape),
-            initializer=tf.keras.initializers.Constant(0.0),
-            trainable=True)
+        layer.register_parameter(f"{name}_{PTQ_THRESHOLD}",
+                                 nn.Parameter(torch.tensor(self.threshold_values, requires_grad=False)
+                                              if not self.per_channel
+                                              else to_torch_tensor(self.threshold_values),requires_grad=False))
+        layer.register_parameter(f"{name}_{AUXVAR}", nn.Parameter(to_torch_tensor(torch.zeros(self.threshold_shape)),
+                                                                  requires_grad=True))
 
         # save the quantizer added parameters for later calculations
-        self.add_quantizer_variable(PTQ_THRESHOLD, ptq_threshold_tensor, VariableGroup.QPARAMS)
-        self.add_quantizer_variable(AUXVAR, auxvar_tensor, VariableGroup.WEIGHTS)
+        self.add_quantizer_variable(PTQ_THRESHOLD, layer.get_parameter(f"{name}_{PTQ_THRESHOLD}"), VariableGroup.QPARAMS)
+        self.add_quantizer_variable(AUXVAR, layer.get_parameter(f"{name}_{AUXVAR}"), VariableGroup.WEIGHTS)
+
+
+    def get_quant_config(self) -> Dict[str, np.ndarray]:
+        """
+        Returns the config used to edit NodeQuantizationConfig after GPTQ retraining
+
+        Returns:
+            A dictionary of attributes the quantize_config retraining has changed during GPTQ retraining.
+            Keys must match NodeQuantizationConfig attributes
+
+        """
+        old_threshold = self.get_quantizer_variable(PTQ_THRESHOLD)
+        return {THRESHOLD: torch_tensor_to_numpy(old_threshold).reshape(self.threshold_shape)}
 
     def __call__(self,
-                 inputs: tf.Tensor,
-                 training: bool):
+                 inputs: nn.Parameter,
+                 training: bool) -> nn.Parameter:
         """
         Quantize a tensor.
 
         Args:
             inputs: Input tensor to quantize.
-            training: Whether the graph is in training mode.
+            training: whether in training mode or not
 
         Returns:
-            The quantized tensor.
+            quantized tensor
         """
-
         auxvar = self.get_quantizer_variable(AUXVAR)
         ptq_threshold_tensor = self.get_quantizer_variable(PTQ_THRESHOLD)
 
         if self.per_channel:
             reshape_shape = get_threshold_reshape_shape(inputs.shape,
                                                         quant_axis=self.quantization_axis,
                                                         quant_axis_dim=-1)
-            ptq_threshold_tensor = tf.reshape(ptq_threshold_tensor, reshape_shape)
+            ptq_threshold_tensor = torch.reshape(ptq_threshold_tensor, reshape_shape)
+
             q_tensor = pertubation_symmetric_quantizer(inputs,
                                                        auxvar,
                                                        ptq_threshold_tensor,
                                                        self.num_bits,
                                                        signed=True,
                                                        power_of_two=self.power_of_two,
                                                        max_lsbs_change=self.max_lsbs_change)
@@ -162,20 +175,7 @@
         else:
             return pertubation_symmetric_quantizer(inputs,
                                                    auxvar,
                                                    ptq_threshold_tensor,
                                                    self.num_bits,
                                                    signed=True,
                                                    power_of_two=self.power_of_two)
-
-
-    def get_quant_config(self) -> Dict[str, np.ndarray]:
-        """
-        Returns the config used to edit NodeQuantizationConfig after GPTQ retraining
-
-        Returns:
-            A dictionary of attributes the quantize_config retraining has changed during GPTQ retraining.
-            Keys must match NodeQuantizationConfig attributes
-
-        """
-        old_threshold = self.get_quantizer_variable(PTQ_THRESHOLD)
-        return {THRESHOLD: old_threshold.numpy().reshape(self.threshold_shape)}
```

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/gptq/pytorch/__init__.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/gptq/pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/gptq/pytorch/gptq_loss.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/gptq/pytorch/gptq_loss.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/gptq/pytorch/gptq_pytorch_implementation.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/gptq/pytorch/gptq_pytorch_implementation.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/gptq/pytorch/gptq_training.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/gptq/pytorch/gptq_training.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/gptq/pytorch/graph_info.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/gptq/pytorch/graph_info.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/gptq/pytorch/quantization_facade.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/gptq/pytorch/quantization_facade.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/gptq/pytorch/quantizer/__init__.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/gptq/pytorch/quantizer/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/gptq/pytorch/quantizer/base_pytorch_gptq_quantizer.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/gptq/pytorch/quantizer/base_pytorch_gptq_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/gptq/pytorch/quantizer/quant_utils.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/gptq/pytorch/quantizer/quant_utils.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/gptq/pytorch/quantizer/quantization_builder.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/gptq/pytorch/quantizer/quantization_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/gptq/pytorch/quantizer/regularization_factory.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/gptq/pytorch/quantizer/regularization_factory.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/__init__.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/legacy/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/soft_quantizer_reg.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/soft_quantizer_reg.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/symmetric_soft_quantizer.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/symmetric_soft_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/uniform_soft_quantizer.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/uniform_soft_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/gptq/pytorch/quantizer/ste_rounding/__init__.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/gptq/pytorch/quantizer/ste_rounding/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/gptq/runner.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/gptq/runner.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/legacy/__init__.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/legacy/keras_quantization_facade.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/legacy/keras_quantization_facade.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/legacy/pytorch_quantization_facade.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/legacy/pytorch_quantization_facade.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/logger.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/logger.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/ptq/__init__.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/ptq/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/ptq/keras/__init__.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/ptq/keras/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/ptq/keras/quantization_facade.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/ptq/keras/quantization_facade.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/ptq/pytorch/__init__.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/ptq/pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/ptq/pytorch/quantization_facade.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/ptq/pytorch/quantization_facade.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/ptq/runner.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/ptq/runner.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/qat/__init__.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/qat/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/qat/common/__init__.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/qat/common/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/qat/common/qat_config.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/qat/common/qat_config.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/qat/keras/__init__.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/qat/keras/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/qat/keras/quantization_facade.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/qat/keras/quantization_facade.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/qat/keras/quantizer/__init__.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/qat/keras/quantizer/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/qat/keras/quantizer/base_keras_qat_quantizer.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/qat/keras/quantizer/base_keras_qat_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/qat/keras/quantizer/quant_utils.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/qat/keras/quantizer/quant_utils.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/qat/keras/quantizer/quantization_builder.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/qat/keras/quantizer/quantization_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/qat/keras/quantizer/ste_rounding/__init__.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/qat/keras/quantizer/ste_rounding/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/qat/keras/quantizer/ste_rounding/symmetric_ste.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/qat/keras/quantizer/ste_rounding/symmetric_ste.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/qat/keras/quantizer/ste_rounding/uniform_ste.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/qat/keras/quantizer/ste_rounding/uniform_ste.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/qat/pytorch/__init__.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/qat/pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/qat/pytorch/quantization_facade.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/qat/pytorch/quantization_facade.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/qat/pytorch/quantizer/__init__.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/qat/pytorch/quantizer/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/qat/pytorch/quantizer/base_pytorch_qat_quantizer.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/qat/pytorch/quantizer/base_pytorch_qat_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/qat/pytorch/quantizer/quantization_builder.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/qat/pytorch/quantizer/quantization_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/qat/pytorch/quantizer/quantizer_utils.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/qat/pytorch/quantizer/quantizer_utils.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/qat/pytorch/quantizer/ste_rounding/__init__.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/qat/pytorch/quantizer/ste_rounding/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/qat/pytorch/quantizer/ste_rounding/symmetric_ste.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/qat/pytorch/quantizer/ste_rounding/symmetric_ste.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/qat/pytorch/quantizer/ste_rounding/uniform_ste.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/qat/pytorch/quantizer/ste_rounding/uniform_ste.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/target_platform_capabilities/__init__.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/target_platform_capabilities/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/target_platform_capabilities/constants.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/target_platform_capabilities/constants.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/target_platform_capabilities/immutable.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/target_platform_capabilities/immutable.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/target_platform_capabilities/target_platform/__init__.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/target_platform_capabilities/target_platform/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/target_platform_capabilities/target_platform/current_tp_model.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/target_platform_capabilities/target_platform/current_tp_model.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/target_platform_capabilities/target_platform/fusing.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/target_platform_capabilities/target_platform/fusing.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/target_platform_capabilities/target_platform/op_quantization_config.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/target_platform_capabilities/target_platform/op_quantization_config.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/target_platform_capabilities/target_platform/operators.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/target_platform_capabilities/target_platform/operators.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/target_platform_capabilities/target_platform/quantization_format.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/target_platform_capabilities/target_platform/quantization_format.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/target_platform_capabilities/target_platform/target_platform_model.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/target_platform_capabilities/target_platform/target_platform_model.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/target_platform_capabilities/target_platform/target_platform_model_component.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/target_platform_capabilities/target_platform/target_platform_model_component.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/__init__.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/attribute_filter.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/attribute_filter.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/current_tpc.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/current_tpc.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/layer_filter_params.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/layer_filter_params.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/operations_to_layers.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/operations_to_layers.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/target_platform_capabilities.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/target_platform_capabilities.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/target_platform_capabilities_component.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/target_platform_capabilities_component.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/__init__.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/latest/__init__.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/latest/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/target_platform_capabilities.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/target_platform_capabilities.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v1/__init__.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v1/tp_model.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v1/tp_model.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v1/tpc_keras.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v1/tpc_keras.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v1/tpc_pytorch.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v1/tpc_pytorch.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v2/__init__.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v2/tp_model.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v2/tp_model.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v2/tpc_keras.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v2/tpc_keras.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v2/tpc_pytorch.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v2/tpc_pytorch.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v3/__init__.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v3/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v3/tp_model.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v3/tp_model.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v3/tpc_keras.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v3/tpc_keras.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v3/tpc_pytorch.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v3/tpc_pytorch.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v3_lut/__init__.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v3_lut/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v3_lut/tp_model.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v3_lut/tp_model.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v3_lut/tpc_keras.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v3_lut/tpc_keras.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v3_lut/tpc_pytorch.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v3_lut/tpc_pytorch.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v4/__init__.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v4/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v4/tp_model.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v4/tp_model.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v4/tpc_keras.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v4/tpc_keras.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v4/tpc_pytorch.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v4/tpc_pytorch.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v4_lut/__init__.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v4_lut/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v4_lut/tp_model.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v4_lut/tp_model.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v4_lut/tpc_keras.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v4_lut/tpc_keras.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v4_lut/tpc_pytorch.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v4_lut/tpc_pytorch.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v5/__init__.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v5/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v5/tp_model.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v5/tp_model.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v5/tpc_keras.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v5/tpc_keras.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v5/tpc_pytorch.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v5/tpc_pytorch.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/get_target_platform_capabilities.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/get_target_platform_capabilities.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/__init__.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/trainable_infrastructure/common/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-# ==============================================================================
+# ==============================================================================
```

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/latest/__init__.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/latest/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/target_platform_capabilities.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/target_platform_capabilities.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/__init__.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/tp_model.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/tp_model.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/tpc_keras.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/tpc_keras.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/tpc_pytorch.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/tpc_pytorch.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/__init__.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/latest/__init__.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/latest/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/target_platform_capabilities.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/target_platform_capabilities.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/__init__.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/tp_model.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/tp_model.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/tpc_keras.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/tpc_keras.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/tpc_pytorch.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/tpc_pytorch.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/__init__.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/latest/__init__.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/latest/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/target_platform_capabilities.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/target_platform_capabilities.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/__init__.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/tp_model.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/tp_model.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/tpc_keras.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/tpc_keras.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/tpc_pytorch.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/tpc_pytorch.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/trainable_infrastructure/__init__.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/trainable_infrastructure/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/trainable_infrastructure/common/__init__.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/trainable_infrastructure/keras/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/trainable_infrastructure/common/base_trainable_quantizer.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/trainable_infrastructure/common/base_trainable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/trainable_infrastructure/common/constants.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/trainable_infrastructure/common/constants.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/trainable_infrastructure/common/get_quantizer_config.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/trainable_infrastructure/common/get_quantizer_config.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/trainable_infrastructure/common/get_quantizers.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/trainable_infrastructure/common/get_quantizers.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/trainable_infrastructure/common/quant_utils.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/trainable_infrastructure/common/quant_utils.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/trainable_infrastructure/common/trainable_quantizer_config.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/trainable_infrastructure/common/trainable_quantizer_config.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/trainable_infrastructure/keras/__init__.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/trainable_infrastructure/pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/trainable_infrastructure/keras/base_keras_quantizer.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/trainable_infrastructure/keras/base_keras_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/trainable_infrastructure/keras/config_serialization.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/trainable_infrastructure/keras/config_serialization.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/trainable_infrastructure/keras/load_model.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/trainable_infrastructure/keras/load_model.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/trainable_infrastructure/keras/quantizer_utils.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/trainable_infrastructure/keras/quantizer_utils.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/trainable_infrastructure/pytorch/__init__.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/core/common/mixed_precision/configurable_quant_id.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,8 +7,17 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-# ==============================================================================
+# ==============================================================================
+from enum import Enum
+
+
+class ConfigurableQuantizerIdentifier(Enum):
+    """
+    A unique idetifier for configurable quantizers.
+    """
+
+    CONFIGURABLE_ID = "Configurable_Quantizer"
```

### Comparing `mct-nightly-1.9.0.20230706.post446/model_compression_toolkit/trainable_infrastructure/pytorch/base_pytorch_quantizer.py` & `mct-nightly-1.9.0.20230707.post446/model_compression_toolkit/trainable_infrastructure/pytorch/base_pytorch_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230706.post446/setup.py` & `mct-nightly-1.9.0.20230707.post446/setup.py`

 * *Files identical despite different names*

