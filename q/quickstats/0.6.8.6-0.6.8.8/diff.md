# Comparing `tmp/quickstats-0.6.8.6.tar.gz` & `tmp/quickstats-0.6.8.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quickstats-0.6.8.6.tar", last modified: Mon Jun 12 09:05:55 2023, max compression
+gzip compressed data, was "quickstats-0.6.8.8.tar", last modified: Sat Jul  8 17:04:23 2023, max compression
```

## Comparing `quickstats-0.6.8.6.tar` & `quickstats-0.6.8.8.tar`

### file list

```diff
@@ -1,241 +1,242 @@
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-06-12 09:05:55.000000 quickstats-0.6.8.6/
--rw-r--r--   0 chlcheng (124202) zp        (1307)     4011 2023-06-12 09:05:55.000000 quickstats-0.6.8.6/PKG-INFO
--rw-r--r--   0 chlcheng (124202) zp        (1307)     3567 2023-01-04 09:02:54.000000 quickstats-0.6.8.6/README.md
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-06-12 09:05:53.000000 quickstats-0.6.8.6/bin/
--rwxr-xr-x   0 chlcheng (124202) zp        (1307)     1651 2023-05-11 20:22:22.000000 quickstats-0.6.8.6/bin/quickstats
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-06-12 09:05:53.000000 quickstats-0.6.8.6/quickstats/
--rw-r--r--   0 chlcheng (124202) zp        (1307)      626 2023-05-31 15:23:38.000000 quickstats-0.6.8.6/quickstats/__init__.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)       24 2023-06-12 08:48:07.000000 quickstats-0.6.8.6/quickstats/_version.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-06-12 09:05:53.000000 quickstats-0.6.8.6/quickstats/analysis/
--rw-r--r--   0 chlcheng (124202) zp        (1307)      428 2023-02-08 03:42:01.000000 quickstats-0.6.8.6/quickstats/analysis/__init__.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    10275 2023-02-08 08:27:54.000000 quickstats-0.6.8.6/quickstats/analysis/analysis_base.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     4191 2023-02-08 05:24:19.000000 quickstats-0.6.8.6/quickstats/analysis/analysis_path_manager.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    22807 2023-03-14 14:12:10.000000 quickstats-0.6.8.6/quickstats/analysis/config_format_templates.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    41649 2023-05-20 03:33:19.000000 quickstats-0.6.8.6/quickstats/analysis/data_loading.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1303 2023-01-04 09:02:54.000000 quickstats-0.6.8.6/quickstats/analysis/data_preprocessing.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    85935 2023-05-20 03:34:59.000000 quickstats-0.6.8.6/quickstats/analysis/event_categorization.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     8060 2023-01-04 09:02:54.000000 quickstats-0.6.8.6/quickstats/analysis/multi_class_boundary_tree.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     9286 2023-05-20 03:35:21.000000 quickstats-0.6.8.6/quickstats/analysis/ntuple_conversion_tool.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    32052 2023-06-03 14:05:32.000000 quickstats-0.6.8.6/quickstats/analysis/ntuple_process_tool.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     8897 2023-06-07 14:20:37.000000 quickstats-0.6.8.6/quickstats/analysis/sample_poly_param_tool.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-06-12 09:05:53.000000 quickstats-0.6.8.6/quickstats/analysis/systematics/
--rw-r--r--   0 chlcheng (124202) zp        (1307)      241 2023-03-07 22:17:53.000000 quickstats-0.6.8.6/quickstats/analysis/systematics/__init__.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    29550 2023-05-20 03:37:08.000000 quickstats-0.6.8.6/quickstats/analysis/systematics/base_systematics.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     9774 2023-04-03 12:27:59.000000 quickstats-0.6.8.6/quickstats/analysis/systematics/gaussian_shape_systematics.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     6796 2023-03-14 18:47:57.000000 quickstats-0.6.8.6/quickstats/analysis/systematics/normalization_systematics.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    11815 2023-05-20 03:31:54.000000 quickstats-0.6.8.6/quickstats/analysis/systematics/systematics_evaluation_tool.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-06-12 09:05:53.000000 quickstats-0.6.8.6/quickstats/clis/
--rw-r--r--   0 chlcheng (124202) zp        (1307)        0 2021-05-17 11:53:22.000000 quickstats-0.6.8.6/quickstats/clis/__init__.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    35406 2023-06-08 10:16:18.000000 quickstats-0.6.8.6/quickstats/clis/core.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     2174 2023-02-14 22:30:46.000000 quickstats-0.6.8.6/quickstats/clis/inspect_rfile.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     2573 2023-02-14 22:27:47.000000 quickstats-0.6.8.6/quickstats/clis/inspect_ws.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    16785 2023-06-05 09:37:42.000000 quickstats-0.6.8.6/quickstats/clis/likelihood_fit.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     7818 2023-01-04 09:02:54.000000 quickstats-0.6.8.6/quickstats/clis/likelihood_scan.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     8575 2023-01-04 09:02:54.000000 quickstats-0.6.8.6/quickstats/clis/limit_setting.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1327 2023-02-14 22:29:19.000000 quickstats-0.6.8.6/quickstats/clis/processor_cli.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    15178 2023-05-11 20:21:35.000000 quickstats-0.6.8.6/quickstats/clis/workspace_tools.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-06-12 09:05:53.000000 quickstats-0.6.8.6/quickstats/components/
--rw-r--r--   0 chlcheng (124202) zp        (1307)      849 2023-05-30 19:49:31.000000 quickstats-0.6.8.6/quickstats/components/__init__.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     3152 2023-05-27 07:22:07.000000 quickstats-0.6.8.6/quickstats/components/analysis_base.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    13357 2023-06-09 12:55:20.000000 quickstats-0.6.8.6/quickstats/components/analysis_object.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     7333 2023-06-08 10:12:47.000000 quickstats-0.6.8.6/quickstats/components/asimov_generator.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    30804 2023-05-20 02:55:29.000000 quickstats-0.6.8.6/quickstats/components/asymptotic_cls.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     2464 2023-01-04 09:02:54.000000 quickstats-0.6.8.6/quickstats/components/basics.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    31916 2023-06-07 11:32:50.000000 quickstats-0.6.8.6/quickstats/components/extended_minimizer.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)   102368 2023-06-10 22:20:54.000000 quickstats-0.6.8.6/quickstats/components/extended_model.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     5539 2023-05-20 03:03:29.000000 quickstats-0.6.8.6/quickstats/components/extended_rfile.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    14934 2023-06-07 13:15:59.000000 quickstats-0.6.8.6/quickstats/components/likelihood.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-06-12 09:05:53.000000 quickstats-0.6.8.6/quickstats/components/modelling/
--rw-r--r--   0 chlcheng (124202) zp        (1307)      207 2022-09-18 16:06:32.000000 quickstats-0.6.8.6/quickstats/components/modelling/__init__.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     2520 2022-09-18 05:43:28.000000 quickstats-0.6.8.6/quickstats/components/modelling/component_source.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    20157 2023-05-20 03:06:27.000000 quickstats-0.6.8.6/quickstats/components/modelling/data_modelling.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      767 2022-09-18 12:07:18.000000 quickstats-0.6.8.6/quickstats/components/modelling/model_source.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     4562 2022-09-18 16:32:35.000000 quickstats-0.6.8.6/quickstats/components/modelling/parameter_templates.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     5578 2023-05-20 03:07:18.000000 quickstats-0.6.8.6/quickstats/components/modelling/pdf_fit_tool.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     3532 2023-05-20 03:07:28.000000 quickstats-0.6.8.6/quickstats/components/modelling/tree_data_source.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    10839 2022-04-07 03:18:15.000000 quickstats-0.6.8.6/quickstats/components/nuisance_parameter_harmonizer.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    17291 2023-05-31 18:05:59.000000 quickstats-0.6.8.6/quickstats/components/nuisance_parameter_pull.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    12390 2023-05-31 15:55:13.000000 quickstats-0.6.8.6/quickstats/components/nuisance_parameter_ranking.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-06-12 09:05:53.000000 quickstats-0.6.8.6/quickstats/components/processors/
--rw-r--r--   0 chlcheng (124202) zp        (1307)      205 2022-07-19 21:07:01.000000 quickstats-0.6.8.6/quickstats/components/processors/__init__.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-06-12 09:05:54.000000 quickstats-0.6.8.6/quickstats/components/processors/actions/
--rw-r--r--   0 chlcheng (124202) zp        (1307)     2066 2023-05-19 15:52:58.000000 quickstats-0.6.8.6/quickstats/components/processors/actions/__init__.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      111 2022-07-21 18:27:25.000000 quickstats-0.6.8.6/quickstats/components/processors/actions/auxiliary.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1072 2023-03-05 12:07:49.000000 quickstats-0.6.8.6/quickstats/components/processors/actions/rooproc_alias.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1082 2022-07-19 21:51:30.000000 quickstats-0.6.8.6/quickstats/components/processors/actions/rooproc_as_numpy.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     2660 2023-05-21 22:51:18.000000 quickstats-0.6.8.6/quickstats/components/processors/actions/rooproc_base_action.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      784 2023-05-21 22:53:11.000000 quickstats-0.6.8.6/quickstats/components/processors/actions/rooproc_declare.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      870 2023-05-23 18:53:54.000000 quickstats-0.6.8.6/quickstats/components/processors/actions/rooproc_define.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1154 2023-06-03 14:06:41.000000 quickstats-0.6.8.6/quickstats/components/processors/actions/rooproc_export.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1164 2022-07-21 15:20:21.000000 quickstats-0.6.8.6/quickstats/components/processors/actions/rooproc_filter.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1076 2022-08-29 06:56:49.000000 quickstats-0.6.8.6/quickstats/components/processors/actions/rooproc_global_variables.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      506 2022-07-19 21:00:22.000000 quickstats-0.6.8.6/quickstats/components/processors/actions/rooproc_helper_action.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      586 2022-07-19 21:52:08.000000 quickstats-0.6.8.6/quickstats/components/processors/actions/rooproc_hybrid_action.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      697 2022-07-21 18:29:41.000000 quickstats-0.6.8.6/quickstats/components/processors/actions/rooproc_if_defined.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      704 2022-07-21 18:48:13.000000 quickstats-0.6.8.6/quickstats/components/processors/actions/rooproc_if_not_defined.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      636 2022-07-19 21:50:41.000000 quickstats-0.6.8.6/quickstats/components/processors/actions/rooproc_load_frame.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1121 2023-05-21 22:55:55.000000 quickstats-0.6.8.6/quickstats/components/processors/actions/rooproc_load_macro.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      140 2022-07-19 20:40:20.000000 quickstats-0.6.8.6/quickstats/components/processors/actions/rooproc_max.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      142 2022-07-19 20:41:10.000000 quickstats-0.6.8.6/quickstats/components/processors/actions/rooproc_mean.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      140 2022-07-19 20:40:51.000000 quickstats-0.6.8.6/quickstats/components/processors/actions/rooproc_min.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      636 2022-07-21 18:30:05.000000 quickstats-0.6.8.6/quickstats/components/processors/actions/rooproc_nested_action.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      462 2022-07-19 20:22:13.000000 quickstats-0.6.8.6/quickstats/components/processors/actions/rooproc_rdf_action.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      398 2022-07-19 20:28:28.000000 quickstats-0.6.8.6/quickstats/components/processors/actions/rooproc_redefine.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1677 2023-05-22 21:51:19.000000 quickstats-0.6.8.6/quickstats/components/processors/actions/rooproc_report.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1382 2023-03-05 12:11:04.000000 quickstats-0.6.8.6/quickstats/components/processors/actions/rooproc_safe_alias.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      454 2022-07-19 20:28:24.000000 quickstats-0.6.8.6/quickstats/components/processors/actions/rooproc_safe_define.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     2129 2023-06-03 16:04:25.000000 quickstats-0.6.8.6/quickstats/components/processors/actions/rooproc_save.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      645 2023-06-03 14:13:00.000000 quickstats-0.6.8.6/quickstats/components/processors/actions/rooproc_save_frame.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1194 2022-07-19 21:50:00.000000 quickstats-0.6.8.6/quickstats/components/processors/actions/rooproc_stat.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      140 2022-07-19 20:39:49.000000 quickstats-0.6.8.6/quickstats/components/processors/actions/rooproc_sum.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      523 2022-07-19 21:54:23.000000 quickstats-0.6.8.6/quickstats/components/processors/actions/rooproc_treename.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     9969 2023-06-05 23:09:50.000000 quickstats-0.6.8.6/quickstats/components/processors/builtin_methods.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     6504 2023-05-21 22:51:45.000000 quickstats-0.6.8.6/quickstats/components/processors/roo_config_parser.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     6772 2023-06-03 19:25:34.000000 quickstats-0.6.8.6/quickstats/components/processors/roo_processor.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     5397 2021-09-16 21:06:55.000000 quickstats-0.6.8.6/quickstats/components/pvalue_toys.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     3519 2023-05-20 03:04:57.000000 quickstats-0.6.8.6/quickstats/components/roo_inspector.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     3083 2023-05-20 03:04:47.000000 quickstats-0.6.8.6/quickstats/components/root_object.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    21336 2023-05-20 03:06:10.000000 quickstats-0.6.8.6/quickstats/components/toy_limit_calculator.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-06-12 09:05:54.000000 quickstats-0.6.8.6/quickstats/components/workspaces/
--rw-r--r--   0 chlcheng (124202) zp        (1307)      591 2023-05-11 12:58:08.000000 quickstats-0.6.8.6/quickstats/components/workspaces/__init__.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     9877 2023-05-20 03:10:01.000000 quickstats-0.6.8.6/quickstats/components/workspaces/asimov_handler.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1727 2023-05-20 03:10:09.000000 quickstats-0.6.8.6/quickstats/components/workspaces/core_argument_sets.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1997 2023-01-09 17:03:21.000000 quickstats-0.6.8.6/quickstats/components/workspaces/sample.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1991 2023-03-11 17:09:50.000000 quickstats-0.6.8.6/quickstats/components/workspaces/settings.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     8295 2023-05-20 03:10:27.000000 quickstats-0.6.8.6/quickstats/components/workspaces/systematic.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     2303 2023-01-08 18:43:45.000000 quickstats-0.6.8.6/quickstats/components/workspaces/systematics_domain.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    53162 2023-06-06 14:20:25.000000 quickstats-0.6.8.6/quickstats/components/workspaces/ws_comparer.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     8837 2023-05-20 03:11:35.000000 quickstats-0.6.8.6/quickstats/components/workspaces/ws_decomposer.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1756 2022-04-20 13:20:42.000000 quickstats-0.6.8.6/quickstats/components/workspaces/ws_modifier_config.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    10859 2023-05-20 03:12:06.000000 quickstats-0.6.8.6/quickstats/components/workspaces/xml_ws_base.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    87030 2023-05-20 03:16:06.000000 quickstats-0.6.8.6/quickstats/components/workspaces/xml_ws_builder_v1.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    76213 2023-05-20 03:19:36.000000 quickstats-0.6.8.6/quickstats/components/workspaces/xml_ws_builder_v2.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    45866 2023-05-20 03:21:08.000000 quickstats-0.6.8.6/quickstats/components/workspaces/xml_ws_combiner.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    48960 2023-05-20 03:23:15.000000 quickstats-0.6.8.6/quickstats/components/workspaces/xml_ws_modifier.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-06-12 09:05:54.000000 quickstats-0.6.8.6/quickstats/concurrent/
--rw-r--r--   0 chlcheng (124202) zp        (1307)      306 2023-05-31 15:27:50.000000 quickstats-0.6.8.6/quickstats/concurrent/__init__.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     3064 2023-05-31 15:10:38.000000 quickstats-0.6.8.6/quickstats/concurrent/abstract_runner.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      627 2022-05-16 01:31:37.000000 quickstats-0.6.8.6/quickstats/concurrent/logging.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     5239 2023-05-31 16:02:49.000000 quickstats-0.6.8.6/quickstats/concurrent/nuisance_parameter_ranking_runner.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     5891 2023-06-10 22:16:28.000000 quickstats-0.6.8.6/quickstats/concurrent/parameterised_asymptotic_cls.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    10275 2023-05-31 15:28:38.000000 quickstats-0.6.8.6/quickstats/concurrent/parameterised_likelihood.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     3963 2023-05-31 15:27:15.000000 quickstats-0.6.8.6/quickstats/concurrent/parameterised_runner.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-06-12 09:05:54.000000 quickstats-0.6.8.6/quickstats/core/
--rw-r--r--   0 chlcheng (124202) zp        (1307)      398 2023-01-04 09:02:55.000000 quickstats-0.6.8.6/quickstats/core/__init__.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      811 2023-01-04 09:02:55.000000 quickstats-0.6.8.6/quickstats/core/abstract_object.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    20587 2023-05-20 03:28:17.000000 quickstats-0.6.8.6/quickstats/core/configs.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     2198 2023-01-04 09:02:55.000000 quickstats-0.6.8.6/quickstats/core/configurable_object.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      541 2023-01-04 09:02:55.000000 quickstats-0.6.8.6/quickstats/core/dataclass_object.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      971 2023-05-20 03:27:42.000000 quickstats-0.6.8.6/quickstats/core/decorators.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     2296 2023-05-23 21:10:32.000000 quickstats-0.6.8.6/quickstats/core/enums.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     6651 2023-02-14 22:36:19.000000 quickstats-0.6.8.6/quickstats/core/methods.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     9057 2023-02-08 05:24:13.000000 quickstats-0.6.8.6/quickstats/core/path_manager.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     2952 2022-07-21 15:05:33.000000 quickstats-0.6.8.6/quickstats/core/virtual_trees.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-06-12 09:05:54.000000 quickstats-0.6.8.6/quickstats/interface/
--rw-r--r--   0 chlcheng (124202) zp        (1307)       66 2023-05-31 15:27:05.000000 quickstats-0.6.8.6/quickstats/interface/__init__.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-06-12 09:05:54.000000 quickstats-0.6.8.6/quickstats/interface/cppyy/
--rw-r--r--   0 chlcheng (124202) zp        (1307)      130 2023-05-31 20:08:24.000000 quickstats-0.6.8.6/quickstats/interface/cppyy/__init__.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      513 2022-01-31 03:37:54.000000 quickstats-0.6.8.6/quickstats/interface/cppyy/core.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    12546 2023-05-28 20:56:33.000000 quickstats-0.6.8.6/quickstats/interface/cppyy/macros.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     4433 2023-01-04 09:02:55.000000 quickstats-0.6.8.6/quickstats/interface/cppyy/vectorize.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-06-12 09:05:54.000000 quickstats-0.6.8.6/quickstats/interface/root/
--rw-r--r--   0 chlcheng (124202) zp        (1307)      621 2022-09-16 14:23:50.000000 quickstats-0.6.8.6/quickstats/interface/root/RooAbsData.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     9855 2023-05-20 12:12:25.000000 quickstats-0.6.8.6/quickstats/interface/root/RooAbsPdf.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      420 2022-08-23 02:59:13.000000 quickstats-0.6.8.6/quickstats/interface/root/RooArgSet.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1182 2023-03-12 16:17:52.000000 quickstats-0.6.8.6/quickstats/interface/root/RooCategory.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    44679 2023-05-20 12:08:58.000000 quickstats-0.6.8.6/quickstats/interface/root/RooDataSet.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      588 2022-08-23 03:02:49.000000 quickstats-0.6.8.6/quickstats/interface/root/RooMsgService.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     5451 2023-05-11 15:17:32.000000 quickstats-0.6.8.6/quickstats/interface/root/RooRealVar.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      130 2022-01-25 17:28:15.000000 quickstats-0.6.8.6/quickstats/interface/root/TArrayData.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      983 2023-01-04 09:02:55.000000 quickstats-0.6.8.6/quickstats/interface/root/TF1.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1995 2023-02-28 09:57:47.000000 quickstats-0.6.8.6/quickstats/interface/root/TFile.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    13146 2023-05-20 12:06:46.000000 quickstats-0.6.8.6/quickstats/interface/root/TH1.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     5707 2023-05-03 13:36:36.000000 quickstats-0.6.8.6/quickstats/interface/root/TH2.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      571 2022-08-23 03:14:20.000000 quickstats-0.6.8.6/quickstats/interface/root/TObject.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      856 2023-03-12 13:27:02.000000 quickstats-0.6.8.6/quickstats/interface/root/__init__.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1069 2022-08-23 02:53:43.000000 quickstats-0.6.8.6/quickstats/interface/root/helper.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     4530 2022-03-24 19:40:20.000000 quickstats-0.6.8.6/quickstats/interface/root/inspection.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      235 2022-08-23 02:57:43.000000 quickstats-0.6.8.6/quickstats/interface/root/io.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    19576 2023-05-11 13:39:17.000000 quickstats-0.6.8.6/quickstats/interface/root/macros.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     5637 2023-05-27 06:13:47.000000 quickstats-0.6.8.6/quickstats/interface/root/roofit_extension.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-06-12 09:05:53.000000 quickstats-0.6.8.6/quickstats/macros/
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-06-12 09:05:54.000000 quickstats-0.6.8.6/quickstats/macros/AsymptoticCLsTool/
--rw-r--r--   0 chlcheng (124202) zp        (1307)     7083 2021-08-19 17:39:48.000000 quickstats-0.6.8.6/quickstats/macros/AsymptoticCLsTool/AsymptoticCLsTool.cxx
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1511 2021-06-11 19:36:10.000000 quickstats-0.6.8.6/quickstats/macros/AsymptoticCLsTool/AsymptoticCLsTool.h
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-06-12 09:05:54.000000 quickstats-0.6.8.6/quickstats/macros/FlexibleInterpVarMkII/
--rw-r--r--   0 chlcheng (124202) zp        (1307)    12372 2022-03-27 23:04:56.000000 quickstats-0.6.8.6/quickstats/macros/FlexibleInterpVarMkII/FlexibleInterpVarMkII.cxx
--rw-r--r--   0 chlcheng (124202) zp        (1307)     2498 2022-03-27 22:34:26.000000 quickstats-0.6.8.6/quickstats/macros/FlexibleInterpVarMkII/FlexibleInterpVarMkII.h
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-06-12 09:05:54.000000 quickstats-0.6.8.6/quickstats/macros/QuickStatsCore/
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1231 2022-05-07 02:55:05.000000 quickstats-0.6.8.6/quickstats/macros/QuickStatsCore/QuickStatsCore.cxx
--rw-r--r--   0 chlcheng (124202) zp        (1307)    10322 2022-05-11 00:00:32.000000 quickstats-0.6.8.6/quickstats/macros/QuickStatsCore/RooFitExt.cxx
--rw-r--r--   0 chlcheng (124202) zp        (1307)     3429 2022-05-10 23:59:25.000000 quickstats-0.6.8.6/quickstats/macros/QuickStatsCore/RooFitExt.h
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-06-12 09:05:54.000000 quickstats-0.6.8.6/quickstats/macros/ResponseFunction/
--rw-r--r--   0 chlcheng (124202) zp        (1307)    13755 2023-04-25 19:09:18.000000 quickstats-0.6.8.6/quickstats/macros/ResponseFunction/ResponseFunction.cxx
--rw-r--r--   0 chlcheng (124202) zp        (1307)     2982 2023-04-25 19:07:54.000000 quickstats-0.6.8.6/quickstats/macros/ResponseFunction/ResponseFunction.h
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-06-12 09:05:54.000000 quickstats-0.6.8.6/quickstats/macros/RooTwoSidedCBShape/
--rw-r--r--   0 chlcheng (124202) zp        (1307)     3689 2022-03-24 20:47:13.000000 quickstats-0.6.8.6/quickstats/macros/RooTwoSidedCBShape/RooTwoSidedCBShape.cxx
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1358 2021-03-16 05:44:03.000000 quickstats-0.6.8.6/quickstats/macros/RooTwoSidedCBShape/RooTwoSidedCBShape.h
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-06-12 09:05:54.000000 quickstats-0.6.8.6/quickstats/maths/
--rw-r--r--   0 chlcheng (124202) zp        (1307)        0 2022-02-07 21:49:51.000000 quickstats-0.6.8.6/quickstats/maths/__init__.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1785 2023-06-10 18:00:53.000000 quickstats-0.6.8.6/quickstats/maths/interpolation.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     5548 2023-03-30 08:30:53.000000 quickstats-0.6.8.6/quickstats/maths/numerics.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    25719 2023-06-05 15:09:16.000000 quickstats-0.6.8.6/quickstats/maths/statistics.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     3506 2023-05-15 01:04:06.000000 quickstats-0.6.8.6/quickstats/maths/statistics_jitted.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      613 2022-09-23 13:42:24.000000 quickstats-0.6.8.6/quickstats/maths/symbolics.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-06-12 09:05:54.000000 quickstats-0.6.8.6/quickstats/parsers/
--rw-r--r--   0 chlcheng (124202) zp        (1307)      113 2022-04-20 10:58:59.000000 quickstats-0.6.8.6/quickstats/parsers/__init__.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      337 2022-04-20 10:57:08.000000 quickstats-0.6.8.6/quickstats/parsers/config_parser.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    15883 2023-05-31 15:27:08.000000 quickstats-0.6.8.6/quickstats/parsers/param_parser.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-06-12 09:05:55.000000 quickstats-0.6.8.6/quickstats/plots/
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1441 2023-03-29 12:38:13.000000 quickstats-0.6.8.6/quickstats/plots/__init__.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    12868 2023-06-10 17:38:08.000000 quickstats-0.6.8.6/quickstats/plots/abstract_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    14145 2023-03-29 14:21:34.000000 quickstats-0.6.8.6/quickstats/plots/bidirectional_bar_chart.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1634 2022-09-07 04:28:06.000000 quickstats-0.6.8.6/quickstats/plots/collective_data_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     2750 2023-04-01 10:15:48.000000 quickstats-0.6.8.6/quickstats/plots/color_schemes.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     5180 2023-05-17 15:59:58.000000 quickstats-0.6.8.6/quickstats/plots/core.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     4007 2023-05-17 16:00:48.000000 quickstats-0.6.8.6/quickstats/plots/correlation_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     5968 2023-03-22 14:09:34.000000 quickstats-0.6.8.6/quickstats/plots/general_1D_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    22775 2022-09-07 07:18:02.000000 quickstats-0.6.8.6/quickstats/plots/general_distribution_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     3731 2022-09-09 08:30:51.000000 quickstats-0.6.8.6/quickstats/plots/histo_1D_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     6100 2023-03-21 16:34:42.000000 quickstats-0.6.8.6/quickstats/plots/hypotest_inverter_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     8153 2023-06-10 15:01:45.000000 quickstats-0.6.8.6/quickstats/plots/likelihood_1D_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    11993 2023-06-10 17:40:53.000000 quickstats-0.6.8.6/quickstats/plots/likelihood_2D_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      219 2021-04-19 13:56:55.000000 quickstats-0.6.8.6/quickstats/plots/likelihood_scan_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    29009 2023-05-31 19:45:49.000000 quickstats-0.6.8.6/quickstats/plots/np_ranking_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    25696 2023-04-18 01:26:39.000000 quickstats-0.6.8.6/quickstats/plots/pdf_distribution_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     5059 2023-02-06 09:15:46.000000 quickstats-0.6.8.6/quickstats/plots/sample_purity_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    10293 2023-03-27 13:06:51.000000 quickstats-0.6.8.6/quickstats/plots/score_distribution_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     4123 2023-01-04 09:02:56.000000 quickstats-0.6.8.6/quickstats/plots/stat_plot_config.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    18642 2023-04-02 13:33:12.000000 quickstats-0.6.8.6/quickstats/plots/template.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    13688 2022-07-29 18:50:11.000000 quickstats-0.6.8.6/quickstats/plots/test_statistic_distribution_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    11061 2023-01-04 09:02:56.000000 quickstats-0.6.8.6/quickstats/plots/upper_limit_1D_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    12201 2023-04-14 12:19:16.000000 quickstats-0.6.8.6/quickstats/plots/upper_limit_2D_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    13186 2022-08-18 13:35:04.000000 quickstats-0.6.8.6/quickstats/plots/upper_limit_3D_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     5069 2022-08-24 13:05:29.000000 quickstats-0.6.8.6/quickstats/plots/upper_limit_benchmark_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    29805 2023-06-05 15:07:31.000000 quickstats-0.6.8.6/quickstats/plots/variable_distribution_plot.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-06-12 09:05:55.000000 quickstats-0.6.8.6/quickstats/resources/
--rw-r--r--   0 chlcheng (124202) zp        (1307)       90 2023-03-20 15:25:27.000000 quickstats-0.6.8.6/quickstats/resources/default_workspace_extensions.json
--rw-r--r--   0 chlcheng (124202) zp        (1307)     4530 2022-04-08 03:20:04.000000 quickstats-0.6.8.6/quickstats/root_checker.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-06-12 09:05:55.000000 quickstats-0.6.8.6/quickstats/stylesheets/
--rw-r--r--   0 chlcheng (124202) zp        (1307)      379 2021-10-20 08:52:20.000000 quickstats-0.6.8.6/quickstats/stylesheets/quick_default.mplstyle
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-06-12 09:05:55.000000 quickstats-0.6.8.6/quickstats/utils/
--rw-r--r--   0 chlcheng (124202) zp        (1307)        0 2021-11-16 06:49:21.000000 quickstats-0.6.8.6/quickstats/utils/__init__.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    10988 2023-06-03 14:56:07.000000 quickstats-0.6.8.6/quickstats/utils/common_utils.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)        0 2021-09-21 13:14:14.000000 quickstats-0.6.8.6/quickstats/utils/condor_tasks.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    17089 2023-06-04 03:39:00.000000 quickstats-0.6.8.6/quickstats/utils/data_conversion.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1187 2022-08-27 16:49:16.000000 quickstats-0.6.8.6/quickstats/utils/hep_utils.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     6812 2023-05-31 13:27:25.000000 quickstats-0.6.8.6/quickstats/utils/io.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      335 2021-05-17 13:11:29.000000 quickstats-0.6.8.6/quickstats/utils/process_tools.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    26262 2023-06-07 15:13:35.000000 quickstats-0.6.8.6/quickstats/utils/roofit_utils.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     9267 2021-11-23 21:10:48.000000 quickstats-0.6.8.6/quickstats/utils/roostats_utils.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    12379 2023-05-20 03:26:53.000000 quickstats-0.6.8.6/quickstats/utils/root_utils.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1347 2023-05-21 21:45:53.000000 quickstats-0.6.8.6/quickstats/utils/string_utils.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    15011 2023-06-07 03:21:08.000000 quickstats-0.6.8.6/quickstats/utils/xml_tools.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-06-12 09:05:53.000000 quickstats-0.6.8.6/quickstats.egg-info/
--rw-r--r--   0 chlcheng (124202) zp        (1307)     4011 2023-06-12 09:05:52.000000 quickstats-0.6.8.6/quickstats.egg-info/PKG-INFO
--rw-r--r--   0 chlcheng (124202) zp        (1307)     9079 2023-06-12 09:05:52.000000 quickstats-0.6.8.6/quickstats.egg-info/SOURCES.txt
--rw-r--r--   0 chlcheng (124202) zp        (1307)        1 2023-06-12 09:05:52.000000 quickstats-0.6.8.6/quickstats.egg-info/dependency_links.txt
--rw-r--r--   0 chlcheng (124202) zp        (1307)       39 2023-06-12 09:05:52.000000 quickstats-0.6.8.6/quickstats.egg-info/requires.txt
--rw-r--r--   0 chlcheng (124202) zp        (1307)       11 2023-06-12 09:05:52.000000 quickstats-0.6.8.6/quickstats.egg-info/top_level.txt
--rw-r--r--   0 chlcheng (124202) zp        (1307)       38 2023-06-12 09:05:55.000000 quickstats-0.6.8.6/setup.cfg
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1687 2023-01-04 09:02:56.000000 quickstats-0.6.8.6/setup.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-07-08 17:04:23.000000 quickstats-0.6.8.8/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     4011 2023-07-08 17:04:23.000000 quickstats-0.6.8.8/PKG-INFO
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     3567 2023-01-04 09:02:54.000000 quickstats-0.6.8.8/README.md
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-07-08 17:04:22.000000 quickstats-0.6.8.8/bin/
+-rwxr-xr-x   0 chlcheng (124202) zp        (1307)     1651 2023-05-11 20:22:22.000000 quickstats-0.6.8.8/bin/quickstats
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-07-08 17:04:22.000000 quickstats-0.6.8.8/quickstats/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      626 2023-05-31 15:23:38.000000 quickstats-0.6.8.8/quickstats/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)       24 2023-07-08 04:42:44.000000 quickstats-0.6.8.8/quickstats/_version.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-07-08 17:04:22.000000 quickstats-0.6.8.8/quickstats/analysis/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      428 2023-02-08 03:42:01.000000 quickstats-0.6.8.8/quickstats/analysis/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    10275 2023-02-08 08:27:54.000000 quickstats-0.6.8.8/quickstats/analysis/analysis_base.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     4191 2023-02-08 05:24:19.000000 quickstats-0.6.8.8/quickstats/analysis/analysis_path_manager.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    22807 2023-03-14 14:12:10.000000 quickstats-0.6.8.8/quickstats/analysis/config_format_templates.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    41649 2023-05-20 03:33:19.000000 quickstats-0.6.8.8/quickstats/analysis/data_loading.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1303 2023-01-04 09:02:54.000000 quickstats-0.6.8.8/quickstats/analysis/data_preprocessing.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    85935 2023-05-20 03:34:59.000000 quickstats-0.6.8.8/quickstats/analysis/event_categorization.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     8060 2023-01-04 09:02:54.000000 quickstats-0.6.8.8/quickstats/analysis/multi_class_boundary_tree.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     9286 2023-05-20 03:35:21.000000 quickstats-0.6.8.8/quickstats/analysis/ntuple_conversion_tool.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    32121 2023-07-07 22:03:31.000000 quickstats-0.6.8.8/quickstats/analysis/ntuple_process_tool.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     8897 2023-06-07 14:20:37.000000 quickstats-0.6.8.8/quickstats/analysis/sample_poly_param_tool.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-07-08 17:04:22.000000 quickstats-0.6.8.8/quickstats/analysis/systematics/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      241 2023-03-07 22:17:53.000000 quickstats-0.6.8.8/quickstats/analysis/systematics/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    29560 2023-07-07 22:04:35.000000 quickstats-0.6.8.8/quickstats/analysis/systematics/base_systematics.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     9774 2023-04-03 12:27:59.000000 quickstats-0.6.8.8/quickstats/analysis/systematics/gaussian_shape_systematics.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     6796 2023-03-14 18:47:57.000000 quickstats-0.6.8.8/quickstats/analysis/systematics/normalization_systematics.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    11869 2023-07-07 22:04:22.000000 quickstats-0.6.8.8/quickstats/analysis/systematics/systematics_evaluation_tool.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-07-08 17:04:23.000000 quickstats-0.6.8.8/quickstats/clis/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)        0 2021-05-17 11:53:22.000000 quickstats-0.6.8.8/quickstats/clis/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    35406 2023-06-08 10:16:18.000000 quickstats-0.6.8.8/quickstats/clis/core.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     2174 2023-02-14 22:30:46.000000 quickstats-0.6.8.8/quickstats/clis/inspect_rfile.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     2573 2023-02-14 22:27:47.000000 quickstats-0.6.8.8/quickstats/clis/inspect_ws.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    16785 2023-06-05 09:37:42.000000 quickstats-0.6.8.8/quickstats/clis/likelihood_fit.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     7980 2023-06-26 09:38:29.000000 quickstats-0.6.8.8/quickstats/clis/likelihood_scan.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     8575 2023-01-04 09:02:54.000000 quickstats-0.6.8.8/quickstats/clis/limit_setting.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1512 2023-06-13 21:11:53.000000 quickstats-0.6.8.8/quickstats/clis/processor_cli.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    15259 2023-06-13 03:13:49.000000 quickstats-0.6.8.8/quickstats/clis/workspace_tools.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-07-08 17:04:23.000000 quickstats-0.6.8.8/quickstats/components/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      849 2023-05-30 19:49:31.000000 quickstats-0.6.8.8/quickstats/components/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     3152 2023-05-27 07:22:07.000000 quickstats-0.6.8.8/quickstats/components/analysis_base.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    13357 2023-07-07 21:51:04.000000 quickstats-0.6.8.8/quickstats/components/analysis_object.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     7333 2023-06-08 10:12:47.000000 quickstats-0.6.8.8/quickstats/components/asimov_generator.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    30804 2023-05-20 02:55:29.000000 quickstats-0.6.8.8/quickstats/components/asymptotic_cls.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     2464 2023-01-04 09:02:54.000000 quickstats-0.6.8.8/quickstats/components/basics.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    31916 2023-06-07 11:32:50.000000 quickstats-0.6.8.8/quickstats/components/extended_minimizer.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)   102824 2023-07-08 04:44:50.000000 quickstats-0.6.8.8/quickstats/components/extended_model.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     5542 2023-07-07 21:58:36.000000 quickstats-0.6.8.8/quickstats/components/extended_rfile.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    14934 2023-07-04 00:19:59.000000 quickstats-0.6.8.8/quickstats/components/likelihood.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-07-08 17:04:23.000000 quickstats-0.6.8.8/quickstats/components/modelling/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      207 2022-09-18 16:06:32.000000 quickstats-0.6.8.8/quickstats/components/modelling/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     2520 2022-09-18 05:43:28.000000 quickstats-0.6.8.8/quickstats/components/modelling/component_source.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    20157 2023-05-20 03:06:27.000000 quickstats-0.6.8.8/quickstats/components/modelling/data_modelling.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      767 2022-09-18 12:07:18.000000 quickstats-0.6.8.8/quickstats/components/modelling/model_source.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     4562 2022-09-18 16:32:35.000000 quickstats-0.6.8.8/quickstats/components/modelling/parameter_templates.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     5578 2023-05-20 03:07:18.000000 quickstats-0.6.8.8/quickstats/components/modelling/pdf_fit_tool.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     3532 2023-05-20 03:07:28.000000 quickstats-0.6.8.8/quickstats/components/modelling/tree_data_source.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    10888 2023-07-03 21:42:51.000000 quickstats-0.6.8.8/quickstats/components/nuisance_parameter_harmonizer.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    17463 2023-07-07 22:11:31.000000 quickstats-0.6.8.8/quickstats/components/nuisance_parameter_pull.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    12396 2023-07-07 22:07:20.000000 quickstats-0.6.8.8/quickstats/components/nuisance_parameter_ranking.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-07-08 17:04:23.000000 quickstats-0.6.8.8/quickstats/components/processors/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      205 2022-07-19 21:07:01.000000 quickstats-0.6.8.8/quickstats/components/processors/__init__.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-07-08 17:04:23.000000 quickstats-0.6.8.8/quickstats/components/processors/actions/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     2066 2023-05-19 15:52:58.000000 quickstats-0.6.8.8/quickstats/components/processors/actions/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      111 2022-07-21 18:27:25.000000 quickstats-0.6.8.8/quickstats/components/processors/actions/auxiliary.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1072 2023-03-05 12:07:49.000000 quickstats-0.6.8.8/quickstats/components/processors/actions/rooproc_alias.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1082 2022-07-19 21:51:30.000000 quickstats-0.6.8.8/quickstats/components/processors/actions/rooproc_as_numpy.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     2666 2023-07-07 21:51:37.000000 quickstats-0.6.8.8/quickstats/components/processors/actions/rooproc_base_action.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      784 2023-05-21 22:53:11.000000 quickstats-0.6.8.8/quickstats/components/processors/actions/rooproc_declare.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      870 2023-05-23 18:53:54.000000 quickstats-0.6.8.8/quickstats/components/processors/actions/rooproc_define.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1154 2023-06-03 14:06:41.000000 quickstats-0.6.8.8/quickstats/components/processors/actions/rooproc_export.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1164 2022-07-21 15:20:21.000000 quickstats-0.6.8.8/quickstats/components/processors/actions/rooproc_filter.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1250 2023-06-13 21:07:45.000000 quickstats-0.6.8.8/quickstats/components/processors/actions/rooproc_global_variables.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      506 2022-07-19 21:00:22.000000 quickstats-0.6.8.8/quickstats/components/processors/actions/rooproc_helper_action.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      586 2022-07-19 21:52:08.000000 quickstats-0.6.8.8/quickstats/components/processors/actions/rooproc_hybrid_action.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      697 2022-07-21 18:29:41.000000 quickstats-0.6.8.8/quickstats/components/processors/actions/rooproc_if_defined.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      704 2022-07-21 18:48:13.000000 quickstats-0.6.8.8/quickstats/components/processors/actions/rooproc_if_not_defined.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      636 2022-07-19 21:50:41.000000 quickstats-0.6.8.8/quickstats/components/processors/actions/rooproc_load_frame.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1121 2023-05-21 22:55:55.000000 quickstats-0.6.8.8/quickstats/components/processors/actions/rooproc_load_macro.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      140 2022-07-19 20:40:20.000000 quickstats-0.6.8.8/quickstats/components/processors/actions/rooproc_max.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      142 2022-07-19 20:41:10.000000 quickstats-0.6.8.8/quickstats/components/processors/actions/rooproc_mean.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      140 2022-07-19 20:40:51.000000 quickstats-0.6.8.8/quickstats/components/processors/actions/rooproc_min.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      636 2022-07-21 18:30:05.000000 quickstats-0.6.8.8/quickstats/components/processors/actions/rooproc_nested_action.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      462 2022-07-19 20:22:13.000000 quickstats-0.6.8.8/quickstats/components/processors/actions/rooproc_rdf_action.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      398 2022-07-19 20:28:28.000000 quickstats-0.6.8.8/quickstats/components/processors/actions/rooproc_redefine.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1677 2023-05-22 21:51:19.000000 quickstats-0.6.8.8/quickstats/components/processors/actions/rooproc_report.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1382 2023-03-05 12:11:04.000000 quickstats-0.6.8.8/quickstats/components/processors/actions/rooproc_safe_alias.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      454 2022-07-19 20:28:24.000000 quickstats-0.6.8.8/quickstats/components/processors/actions/rooproc_safe_define.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     2129 2023-06-03 16:04:25.000000 quickstats-0.6.8.8/quickstats/components/processors/actions/rooproc_save.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      645 2023-06-03 14:13:00.000000 quickstats-0.6.8.8/quickstats/components/processors/actions/rooproc_save_frame.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1194 2022-07-19 21:50:00.000000 quickstats-0.6.8.8/quickstats/components/processors/actions/rooproc_stat.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      140 2022-07-19 20:39:49.000000 quickstats-0.6.8.8/quickstats/components/processors/actions/rooproc_sum.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      523 2022-07-19 21:54:23.000000 quickstats-0.6.8.8/quickstats/components/processors/actions/rooproc_treename.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     9969 2023-06-05 23:09:50.000000 quickstats-0.6.8.8/quickstats/components/processors/builtin_methods.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     6504 2023-05-21 22:51:45.000000 quickstats-0.6.8.8/quickstats/components/processors/roo_config_parser.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     6788 2023-07-07 21:53:01.000000 quickstats-0.6.8.8/quickstats/components/processors/roo_processor.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     5397 2021-09-16 21:06:55.000000 quickstats-0.6.8.8/quickstats/components/pvalue_toys.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     3551 2023-07-07 21:53:49.000000 quickstats-0.6.8.8/quickstats/components/roo_inspector.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     3083 2023-05-20 03:04:47.000000 quickstats-0.6.8.8/quickstats/components/root_object.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    21336 2023-05-20 03:06:10.000000 quickstats-0.6.8.8/quickstats/components/toy_limit_calculator.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-07-08 17:04:23.000000 quickstats-0.6.8.8/quickstats/components/workspaces/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      591 2023-05-11 12:58:08.000000 quickstats-0.6.8.8/quickstats/components/workspaces/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     9877 2023-05-20 03:10:01.000000 quickstats-0.6.8.8/quickstats/components/workspaces/asimov_handler.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1727 2023-05-20 03:10:09.000000 quickstats-0.6.8.8/quickstats/components/workspaces/core_argument_sets.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1997 2023-01-09 17:03:21.000000 quickstats-0.6.8.8/quickstats/components/workspaces/sample.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1991 2023-03-11 17:09:50.000000 quickstats-0.6.8.8/quickstats/components/workspaces/settings.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     8295 2023-05-20 03:10:27.000000 quickstats-0.6.8.8/quickstats/components/workspaces/systematic.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     2303 2023-01-08 18:43:45.000000 quickstats-0.6.8.8/quickstats/components/workspaces/systematics_domain.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    53162 2023-06-06 14:20:25.000000 quickstats-0.6.8.8/quickstats/components/workspaces/ws_comparer.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     8837 2023-05-20 03:11:35.000000 quickstats-0.6.8.8/quickstats/components/workspaces/ws_decomposer.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1756 2022-04-20 13:20:42.000000 quickstats-0.6.8.8/quickstats/components/workspaces/ws_modifier_config.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    10859 2023-05-20 03:12:06.000000 quickstats-0.6.8.8/quickstats/components/workspaces/xml_ws_base.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    87030 2023-05-20 03:16:06.000000 quickstats-0.6.8.8/quickstats/components/workspaces/xml_ws_builder_v1.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    76213 2023-05-20 03:19:36.000000 quickstats-0.6.8.8/quickstats/components/workspaces/xml_ws_builder_v2.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    45869 2023-07-07 21:58:59.000000 quickstats-0.6.8.8/quickstats/components/workspaces/xml_ws_combiner.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    49268 2023-07-08 04:44:49.000000 quickstats-0.6.8.8/quickstats/components/workspaces/xml_ws_modifier.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-07-08 17:04:23.000000 quickstats-0.6.8.8/quickstats/concurrent/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      306 2023-05-31 15:27:50.000000 quickstats-0.6.8.8/quickstats/concurrent/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     3379 2023-06-26 09:41:33.000000 quickstats-0.6.8.8/quickstats/concurrent/abstract_runner.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      627 2022-05-16 01:31:37.000000 quickstats-0.6.8.8/quickstats/concurrent/logging.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     5239 2023-05-31 16:02:49.000000 quickstats-0.6.8.8/quickstats/concurrent/nuisance_parameter_ranking_runner.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     5891 2023-06-10 22:16:28.000000 quickstats-0.6.8.8/quickstats/concurrent/parameterised_asymptotic_cls.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    10758 2023-06-28 16:38:35.000000 quickstats-0.6.8.8/quickstats/concurrent/parameterised_likelihood.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     3963 2023-05-31 15:27:15.000000 quickstats-0.6.8.8/quickstats/concurrent/parameterised_runner.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-07-08 17:04:23.000000 quickstats-0.6.8.8/quickstats/core/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      398 2023-01-04 09:02:55.000000 quickstats-0.6.8.8/quickstats/core/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      811 2023-01-04 09:02:55.000000 quickstats-0.6.8.8/quickstats/core/abstract_object.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    20587 2023-05-20 03:28:17.000000 quickstats-0.6.8.8/quickstats/core/configs.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     2198 2023-01-04 09:02:55.000000 quickstats-0.6.8.8/quickstats/core/configurable_object.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      541 2023-01-04 09:02:55.000000 quickstats-0.6.8.8/quickstats/core/dataclass_object.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      971 2023-05-20 03:27:42.000000 quickstats-0.6.8.8/quickstats/core/decorators.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     2296 2023-05-23 21:10:32.000000 quickstats-0.6.8.8/quickstats/core/enums.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     6651 2023-02-14 22:36:19.000000 quickstats-0.6.8.8/quickstats/core/methods.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     9057 2023-02-08 05:24:13.000000 quickstats-0.6.8.8/quickstats/core/path_manager.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     2952 2022-07-21 15:05:33.000000 quickstats-0.6.8.8/quickstats/core/virtual_trees.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-07-08 17:04:23.000000 quickstats-0.6.8.8/quickstats/interface/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)       66 2023-05-31 15:27:05.000000 quickstats-0.6.8.8/quickstats/interface/__init__.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-07-08 17:04:23.000000 quickstats-0.6.8.8/quickstats/interface/cppyy/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      130 2023-05-31 20:08:24.000000 quickstats-0.6.8.8/quickstats/interface/cppyy/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      513 2022-01-31 03:37:54.000000 quickstats-0.6.8.8/quickstats/interface/cppyy/core.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    12546 2023-05-28 20:56:33.000000 quickstats-0.6.8.8/quickstats/interface/cppyy/macros.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     4433 2023-01-04 09:02:55.000000 quickstats-0.6.8.8/quickstats/interface/cppyy/vectorize.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-07-08 17:04:23.000000 quickstats-0.6.8.8/quickstats/interface/root/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      621 2022-09-16 14:23:50.000000 quickstats-0.6.8.8/quickstats/interface/root/RooAbsData.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     9855 2023-05-20 12:12:25.000000 quickstats-0.6.8.8/quickstats/interface/root/RooAbsPdf.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      420 2022-08-23 02:59:13.000000 quickstats-0.6.8.8/quickstats/interface/root/RooArgSet.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1182 2023-03-12 16:17:52.000000 quickstats-0.6.8.8/quickstats/interface/root/RooCategory.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    44679 2023-05-20 12:08:58.000000 quickstats-0.6.8.8/quickstats/interface/root/RooDataSet.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      588 2022-08-23 03:02:49.000000 quickstats-0.6.8.8/quickstats/interface/root/RooMsgService.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     5451 2023-05-11 15:17:32.000000 quickstats-0.6.8.8/quickstats/interface/root/RooRealVar.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      130 2022-01-25 17:28:15.000000 quickstats-0.6.8.8/quickstats/interface/root/TArrayData.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      983 2023-01-04 09:02:55.000000 quickstats-0.6.8.8/quickstats/interface/root/TF1.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1995 2023-02-28 09:57:47.000000 quickstats-0.6.8.8/quickstats/interface/root/TFile.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    13146 2023-05-20 12:06:46.000000 quickstats-0.6.8.8/quickstats/interface/root/TH1.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     5707 2023-05-03 13:36:36.000000 quickstats-0.6.8.8/quickstats/interface/root/TH2.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      571 2022-08-23 03:14:20.000000 quickstats-0.6.8.8/quickstats/interface/root/TObject.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      856 2023-03-12 13:27:02.000000 quickstats-0.6.8.8/quickstats/interface/root/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1069 2022-08-23 02:53:43.000000 quickstats-0.6.8.8/quickstats/interface/root/helper.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     4530 2022-03-24 19:40:20.000000 quickstats-0.6.8.8/quickstats/interface/root/inspection.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      235 2022-08-23 02:57:43.000000 quickstats-0.6.8.8/quickstats/interface/root/io.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    19576 2023-05-11 13:39:17.000000 quickstats-0.6.8.8/quickstats/interface/root/macros.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     5637 2023-05-27 06:13:47.000000 quickstats-0.6.8.8/quickstats/interface/root/roofit_extension.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-07-08 17:04:22.000000 quickstats-0.6.8.8/quickstats/macros/
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-07-08 17:04:23.000000 quickstats-0.6.8.8/quickstats/macros/AsymptoticCLsTool/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     7083 2021-08-19 17:39:48.000000 quickstats-0.6.8.8/quickstats/macros/AsymptoticCLsTool/AsymptoticCLsTool.cxx
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1511 2021-06-11 19:36:10.000000 quickstats-0.6.8.8/quickstats/macros/AsymptoticCLsTool/AsymptoticCLsTool.h
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-07-08 17:04:23.000000 quickstats-0.6.8.8/quickstats/macros/FlexibleInterpVarMkII/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    12372 2022-03-27 23:04:56.000000 quickstats-0.6.8.8/quickstats/macros/FlexibleInterpVarMkII/FlexibleInterpVarMkII.cxx
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     2498 2022-03-27 22:34:26.000000 quickstats-0.6.8.8/quickstats/macros/FlexibleInterpVarMkII/FlexibleInterpVarMkII.h
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-07-08 17:04:23.000000 quickstats-0.6.8.8/quickstats/macros/QuickStatsCore/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1231 2022-05-07 02:55:05.000000 quickstats-0.6.8.8/quickstats/macros/QuickStatsCore/QuickStatsCore.cxx
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    10322 2022-05-11 00:00:32.000000 quickstats-0.6.8.8/quickstats/macros/QuickStatsCore/RooFitExt.cxx
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     3429 2022-05-10 23:59:25.000000 quickstats-0.6.8.8/quickstats/macros/QuickStatsCore/RooFitExt.h
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-07-08 17:04:23.000000 quickstats-0.6.8.8/quickstats/macros/ResponseFunction/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    13755 2023-04-25 19:09:18.000000 quickstats-0.6.8.8/quickstats/macros/ResponseFunction/ResponseFunction.cxx
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     2982 2023-04-25 19:07:54.000000 quickstats-0.6.8.8/quickstats/macros/ResponseFunction/ResponseFunction.h
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-07-08 17:04:23.000000 quickstats-0.6.8.8/quickstats/macros/RooTwoSidedCBShape/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     3689 2022-03-24 20:47:13.000000 quickstats-0.6.8.8/quickstats/macros/RooTwoSidedCBShape/RooTwoSidedCBShape.cxx
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1358 2021-03-16 05:44:03.000000 quickstats-0.6.8.8/quickstats/macros/RooTwoSidedCBShape/RooTwoSidedCBShape.h
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-07-08 17:04:23.000000 quickstats-0.6.8.8/quickstats/maths/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)        0 2022-02-07 21:49:51.000000 quickstats-0.6.8.8/quickstats/maths/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     2093 2023-06-21 12:10:05.000000 quickstats-0.6.8.8/quickstats/maths/interpolation.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     5548 2023-03-30 08:30:53.000000 quickstats-0.6.8.8/quickstats/maths/numerics.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    28267 2023-07-08 04:40:34.000000 quickstats-0.6.8.8/quickstats/maths/statistics.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     3506 2023-05-15 01:04:06.000000 quickstats-0.6.8.8/quickstats/maths/statistics_jitted.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      613 2022-09-23 13:42:24.000000 quickstats-0.6.8.8/quickstats/maths/symbolics.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-07-08 17:04:23.000000 quickstats-0.6.8.8/quickstats/parsers/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      113 2022-04-20 10:58:59.000000 quickstats-0.6.8.8/quickstats/parsers/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      337 2022-04-20 10:57:08.000000 quickstats-0.6.8.8/quickstats/parsers/config_parser.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    15916 2023-07-07 22:02:29.000000 quickstats-0.6.8.8/quickstats/parsers/param_parser.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-07-08 17:04:23.000000 quickstats-0.6.8.8/quickstats/plots/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1441 2023-03-29 12:38:13.000000 quickstats-0.6.8.8/quickstats/plots/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    14389 2023-06-21 01:49:40.000000 quickstats-0.6.8.8/quickstats/plots/abstract_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    14145 2023-03-29 14:21:34.000000 quickstats-0.6.8.8/quickstats/plots/bidirectional_bar_chart.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1634 2022-09-07 04:28:06.000000 quickstats-0.6.8.8/quickstats/plots/collective_data_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     2750 2023-04-01 10:15:48.000000 quickstats-0.6.8.8/quickstats/plots/color_schemes.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     5180 2023-05-17 15:59:58.000000 quickstats-0.6.8.8/quickstats/plots/core.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     4007 2023-05-17 16:00:48.000000 quickstats-0.6.8.8/quickstats/plots/correlation_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     6018 2023-07-03 18:31:57.000000 quickstats-0.6.8.8/quickstats/plots/general_1D_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    22775 2022-09-07 07:18:02.000000 quickstats-0.6.8.8/quickstats/plots/general_distribution_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     3731 2022-09-09 08:30:51.000000 quickstats-0.6.8.8/quickstats/plots/histo_1D_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     6100 2023-03-21 16:34:42.000000 quickstats-0.6.8.8/quickstats/plots/hypotest_inverter_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     8917 2023-07-04 13:41:54.000000 quickstats-0.6.8.8/quickstats/plots/likelihood_1D_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    14929 2023-07-08 03:46:17.000000 quickstats-0.6.8.8/quickstats/plots/likelihood_2D_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      219 2021-04-19 13:56:55.000000 quickstats-0.6.8.8/quickstats/plots/likelihood_scan_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    29009 2023-05-31 19:45:49.000000 quickstats-0.6.8.8/quickstats/plots/np_ranking_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    25696 2023-04-18 01:26:39.000000 quickstats-0.6.8.8/quickstats/plots/pdf_distribution_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     5059 2023-02-06 09:15:46.000000 quickstats-0.6.8.8/quickstats/plots/sample_purity_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    10293 2023-03-27 13:06:51.000000 quickstats-0.6.8.8/quickstats/plots/score_distribution_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     4123 2023-01-04 09:02:56.000000 quickstats-0.6.8.8/quickstats/plots/stat_plot_config.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    18642 2023-04-02 13:33:12.000000 quickstats-0.6.8.8/quickstats/plots/template.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    13688 2022-07-29 18:50:11.000000 quickstats-0.6.8.8/quickstats/plots/test_statistic_distribution_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    11061 2023-01-04 09:02:56.000000 quickstats-0.6.8.8/quickstats/plots/upper_limit_1D_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    17787 2023-06-21 01:00:28.000000 quickstats-0.6.8.8/quickstats/plots/upper_limit_2D_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    12201 2023-06-19 12:52:28.000000 quickstats-0.6.8.8/quickstats/plots/upper_limit_2D_plot_deprecated.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    13186 2022-08-18 13:35:04.000000 quickstats-0.6.8.8/quickstats/plots/upper_limit_3D_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    16450 2023-06-21 14:06:12.000000 quickstats-0.6.8.8/quickstats/plots/upper_limit_benchmark_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    29707 2023-06-27 09:55:20.000000 quickstats-0.6.8.8/quickstats/plots/variable_distribution_plot.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-07-08 17:04:23.000000 quickstats-0.6.8.8/quickstats/resources/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)       90 2023-03-20 15:25:27.000000 quickstats-0.6.8.8/quickstats/resources/default_workspace_extensions.json
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     4530 2022-04-08 03:20:04.000000 quickstats-0.6.8.8/quickstats/root_checker.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-07-08 17:04:23.000000 quickstats-0.6.8.8/quickstats/stylesheets/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      379 2021-10-20 08:52:20.000000 quickstats-0.6.8.8/quickstats/stylesheets/quick_default.mplstyle
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-07-08 17:04:23.000000 quickstats-0.6.8.8/quickstats/utils/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)        0 2021-11-16 06:49:21.000000 quickstats-0.6.8.8/quickstats/utils/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    11009 2023-07-07 22:00:44.000000 quickstats-0.6.8.8/quickstats/utils/common_utils.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)        0 2021-09-21 13:14:14.000000 quickstats-0.6.8.8/quickstats/utils/condor_tasks.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    17089 2023-06-04 03:39:00.000000 quickstats-0.6.8.8/quickstats/utils/data_conversion.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1187 2022-08-27 16:49:16.000000 quickstats-0.6.8.8/quickstats/utils/hep_utils.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     6812 2023-05-31 13:27:25.000000 quickstats-0.6.8.8/quickstats/utils/io.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      335 2021-05-17 13:11:29.000000 quickstats-0.6.8.8/quickstats/utils/process_tools.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    26262 2023-06-07 15:13:35.000000 quickstats-0.6.8.8/quickstats/utils/roofit_utils.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     9267 2021-11-23 21:10:48.000000 quickstats-0.6.8.8/quickstats/utils/roostats_utils.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    12379 2023-07-07 22:00:16.000000 quickstats-0.6.8.8/quickstats/utils/root_utils.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1448 2023-07-08 03:51:23.000000 quickstats-0.6.8.8/quickstats/utils/string_utils.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    15023 2023-07-07 22:01:35.000000 quickstats-0.6.8.8/quickstats/utils/xml_tools.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-07-08 17:04:22.000000 quickstats-0.6.8.8/quickstats.egg-info/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     4011 2023-07-08 17:04:22.000000 quickstats-0.6.8.8/quickstats.egg-info/PKG-INFO
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     9130 2023-07-08 17:04:22.000000 quickstats-0.6.8.8/quickstats.egg-info/SOURCES.txt
+-rw-r--r--   0 chlcheng (124202) zp        (1307)        1 2023-07-08 17:04:22.000000 quickstats-0.6.8.8/quickstats.egg-info/dependency_links.txt
+-rw-r--r--   0 chlcheng (124202) zp        (1307)       39 2023-07-08 17:04:22.000000 quickstats-0.6.8.8/quickstats.egg-info/requires.txt
+-rw-r--r--   0 chlcheng (124202) zp        (1307)       11 2023-07-08 17:04:22.000000 quickstats-0.6.8.8/quickstats.egg-info/top_level.txt
+-rw-r--r--   0 chlcheng (124202) zp        (1307)       38 2023-07-08 17:04:23.000000 quickstats-0.6.8.8/setup.cfg
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1687 2023-01-04 09:02:56.000000 quickstats-0.6.8.8/setup.py
```

### Comparing `quickstats-0.6.8.6/PKG-INFO` & `quickstats-0.6.8.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quickstats
-Version: 0.6.8.6
+Version: 0.6.8.8
 Summary: A tool for quick statistical analysis for HEP experiments
 Author: Alkaid Cheng
 Author-email: chi.lung.cheng@cern.ch
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `quickstats-0.6.8.6/README.md` & `quickstats-0.6.8.8/README.md`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.6/bin/quickstats` & `quickstats-0.6.8.8/bin/quickstats`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.6/quickstats/__init__.py` & `quickstats-0.6.8.8/quickstats/__init__.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.6/quickstats/analysis/analysis_base.py` & `quickstats-0.6.8.8/quickstats/analysis/analysis_base.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.6/quickstats/analysis/analysis_path_manager.py` & `quickstats-0.6.8.8/quickstats/analysis/analysis_path_manager.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.6/quickstats/analysis/config_format_templates.py` & `quickstats-0.6.8.8/quickstats/analysis/config_format_templates.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.6/quickstats/analysis/data_loading.py` & `quickstats-0.6.8.8/quickstats/analysis/data_loading.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.6/quickstats/analysis/data_preprocessing.py` & `quickstats-0.6.8.8/quickstats/analysis/data_preprocessing.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.6/quickstats/analysis/event_categorization.py` & `quickstats-0.6.8.8/quickstats/analysis/event_categorization.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.6/quickstats/analysis/multi_class_boundary_tree.py` & `quickstats-0.6.8.8/quickstats/analysis/multi_class_boundary_tree.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.6/quickstats/analysis/ntuple_conversion_tool.py` & `quickstats-0.6.8.8/quickstats/analysis/ntuple_conversion_tool.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.6/quickstats/analysis/ntuple_process_tool.py` & `quickstats-0.6.8.8/quickstats/analysis/ntuple_process_tool.py`

 * *Files 2% similar despite different names*

```diff
@@ -473,19 +473,19 @@
                            self._merge_samples_with_hadd,
                            outdir=outdir,
                            samples=samples,
                            syst_themes=syst_themes,
                            syst_names=syst_names,
                            subdirs=subdirs)
     
-    def _merge_samples_with_hadd(self, fnames:List[str], outname:str):
-        for fname in fnames:
-            if not os.path.exists(fname):
-                raise FileNotFoundError(f'missing ntuple file "{fname}"')
-        hadd_cmd = "hadd -f {} {}".format(outname, " ".join(fnames))
+    def _merge_samples_with_hadd(self, filenames:List[str], outname:str):
+        for filename in filenames:
+            if not os.path.exists(filename):
+                raise FileNotFoundError(f'missing ntuple file "{filename}"')
+        hadd_cmd = "hadd -f {} {}".format(outname, " ".join(filenames))
         os.system(hadd_cmd)
             
     def merge_cutflows(self, samples:Optional[List[str]]=None, subdirs:Optional[List[str]]=None):
         outdir = self.path_manager.get_directory("cutflow")
         self.merge_outputs(self.get_cutflow_outpath,
                            self.get_merged_cutflow_outpath,
                            self._merge_cutflow_data,
@@ -538,42 +538,42 @@
                 continue
             last_idx = np.where(this_pass_values == prev_pass_value)
             if len(last_idx[0]) == 0:
                 raise RuntimeError("failed to calculate efficiency")
             efficiency.append(100 * (weight_values[i] / weight_values[last_idx][0]))
         return efficiency, cumul_efficiency
     
-    def _merge_cutflow_data(self, fnames:List[str], outname:str):
+    def _merge_cutflow_data(self, filenames:List[str], outname:str):
         import pandas as pd
         merged_df = None
-        for fname in fnames:
-            if isinstance(fname, (list, tuple)):
+        for filename in filenames:
+            if isinstance(filename, (list, tuple)):
                 # first file contains cutflow information
                 # second file contains weight information                
-                assert len(fname) == 2
-                cutflow_fname = fname[0]
-                weight_fname = fname[1]
+                assert len(filename) == 2
+                cutflow_filename = filename[0]
+                weight_filename = filename[1]
             else:
-                cutflow_fname = fname
-                weight_fname = None
-            if not os.path.exists(cutflow_fname):
-                raise FileNotFoundError(f'missing cutflow file "{cutflow_fname}"')
-            cutflow_df = pd.read_csv(cutflow_fname)
-            cutflow_df, yield_values = self._process_exported_data(cutflow_df, weight_fname)
+                cutflow_filename = filename
+                weight_filename = None
+            if not os.path.exists(cutflow_filename):
+                raise FileNotFoundError(f'missing cutflow file "{cutflow_filename}"')
+            cutflow_df = pd.read_csv(cutflow_filename)
+            cutflow_df, yield_values = self._process_exported_data(cutflow_df, weight_filename)
             if merged_df is None:
                 merged_df = cutflow_df.copy()
                 if yield_values is not None:
                     merged_df['yield'] = yield_values
             else:
                 merged_df['all']  += cutflow_df['all']
                 merged_df['pass'] += cutflow_df['pass']
                 if 'yield' in merged_df:
                     if yield_values is None:
                         raise RuntimeError(f'missing weight file that is in association with the '
-                                           f'cutflow file "{cutflow_fname}"')
+                                           f'cutflow file "{cutflow_filename}"')
                     merged_df['yield'] += yield_values
         efficiency, cumul_efficiency = self._get_efficiency_values(merged_df, 'pass')
         merged_df['efficiency'] = efficiency
         merged_df['cumulative_efficiency'] = cumul_efficiency
         if 'yield' in merged_df:
             yield_efficiency, yield_cumul_efficiency = self._get_efficiency_values(merged_df, 'yield')
             merged_df['yield_efficiency'] = yield_efficiency
```

### Comparing `quickstats-0.6.8.6/quickstats/analysis/sample_poly_param_tool.py` & `quickstats-0.6.8.8/quickstats/analysis/sample_poly_param_tool.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.6/quickstats/analysis/systematics/base_systematics.py` & `quickstats-0.6.8.8/quickstats/analysis/systematics/base_systematics.py`

 * *Files 0% similar despite different names*

```diff
@@ -566,17 +566,17 @@
     def get_valid_dataframe(self, syst_type):
         if self.dataframe is None:
             return
         if (syst_type, "prune_status") in self.dataframe:
             return self.dataframe[self.dataframe[(syst_type, 'prune_status')] == 0]
         return self.dataframe
     
-    def save_simplified_data(self, fname):
+    def save_simplified_data(self, filename:str):
         data = self.get_simplified_data()
-        with open(fname, 'w') as f:
+        with open(filename, 'w') as f:
             json.dump(data, f, indent=2)
     
     @staticmethod
     def _discard(df, **expressions):
         new_df = df.copy()
         mask = pd.Series(True, index=df.index)
         for index in expressions:
```

### Comparing `quickstats-0.6.8.6/quickstats/analysis/systematics/gaussian_shape_systematics.py` & `quickstats-0.6.8.8/quickstats/analysis/systematics/gaussian_shape_systematics.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.6/quickstats/analysis/systematics/normalization_systematics.py` & `quickstats-0.6.8.8/quickstats/analysis/systematics/normalization_systematics.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.6/quickstats/analysis/systematics/systematics_evaluation_tool.py` & `quickstats-0.6.8.8/quickstats/analysis/systematics/systematics_evaluation_tool.py`

 * *Files 2% similar despite different names*

```diff
@@ -128,38 +128,38 @@
                                    syst_themes:Optional[List[str]]=None):
         input_paths = self.get_selected_paths(samples=samples, syst_themes=syst_themes)
         executor = self.norm_syst_module.get_systematics_from_root_file
         for process in tree_paths:
             categories = self.get_categories(process)
             for syst_theme in tree_paths[process]:
                 syst_list = self.systematics_by_theme[syst_theme]
-                fname = tree_paths[process][syst_theme]
-                executor(fname, categories, syst_list, process, append=True)
+                filename = tree_paths[process][syst_theme]
+                executor(filename, categories, syst_list, process, append=True)
                 
     def create_bootstrap_trees(self, cache:Optional[bool]=None):
         if cache is None:
             cache = self.cache
         tree_paths = self.get_input_tree_paths()
         cache = self.config['cache']
         parallel = self.config['parallel']
         executor = partial(self.shape_syst_module.create_bootstrap_trees_from_root_file, cache=cache)
-        args_fnames = []
+        args_filenames = []
         args_categories = []
         args_syst_list = []
         args_processes = []
         for process in tree_paths:
             categories = self.get_categories(process)
             for syst_theme in tree_paths[process]:
                 syst_list = self.systematics_by_theme[syst_theme]
-                fname = tree_paths[process][syst_theme]
-                args_fnames.append(fname)
+                filename = tree_paths[process][syst_theme]
+                args_filenames.append(filename)
                 args_categories.append(categories)
                 args_syst_list.append(syst_list)
                 args_processes.append(process)
-        task_args = (args_fnames, args_categories, args_syst_list, args_processes)
+        task_args = (args_filenames, args_categories, args_syst_list, args_processes)
         execute_multi_tasks(executor, *task_args, parallel=parallel)
                 
     def evaluate_shape_systematics(self):
         parallel = self.config['parallel']
         save_toys = self.config['save_toys']
         cache = self.config['cache']
         executor = partial(self.shape_syst_module.get_bootstrap_systematics,
@@ -195,37 +195,37 @@
             dirname = os.path.join(self.base_path, "results")
             if mode == "detailed":
                 basename = self.FILE_NAMES['individual_detailed'].format(syst_type=syst_type)
             elif mode == "processed":
                 basename = self.FILE_NAMES['individual_processed'].format(syst_type=syst_type)
             else:
                 raise ValueError("unknown mode: {}".format(mode))
-            fname = os.path.join(dirname, basename)
-            if os.path.exists(fname):
-                modules[syst_type].load(fname)
-                self.stdout.info("Loaded results for {} systematics from `{}`".format(syst_type, fname))
+            filename = os.path.join(dirname, basename)
+            if os.path.exists(filename):
+                modules[syst_type].load(filename)
+                self.stdout.info("Loaded results for {} systematics from `{}`".format(syst_type, filename))
                 modules[syst_type].processed = (mode == "processed")
             else:
-                self.stdout.error("No saved results found for {} systematics (in `{}`)".format(syst_type, fname))
+                self.stdout.error("No saved results found for {} systematics (in `{}`)".format(syst_type, filename))
                 
     def save_result(self, syst_types=None):
         modules = {"yield": self.yield_syst_module, "shape": self.shape_syst_module}
         if syst_types is None:
             syst_types = self.syst_types
         for syst_type in syst_types:
             dirname = os.path.join(self.base_path, "results")
             if modules[syst_type].processed:
                 basename = self.FILE_NAMES['individual_processed'].format(syst_type=syst_type)
             else:
                 basename = self.FILE_NAMES['individual_detailed'].format(syst_type=syst_type)
-            fname = os.path.join(dirname, basename)
+            filename = os.path.join(dirname, basename)
             if not os.path.exists(dirname):
                 os.makedirs(dirname)
-            modules[syst_type].save(fname)
-            self.stdout.info("Saved results for {} systematics in `{}`".format(syst_type, fname))
+            modules[syst_type].save(filename)
+            self.stdout.info("Saved results for {} systematics in `{}`".format(syst_type, filename))
             
     def get_combined_summary(self):
         modules = {"yield": self.yield_syst_module, "shape": self.shape_syst_module}
         combined_result = {}
         for syst_type in self.syst_types:
             if modules[syst_type].dataframe is None:
                 continue
@@ -235,18 +235,18 @@
     
     def save_combined_summary(self):
         combined_result = self.get_combined_summary()
         dirname = os.path.join(self.base_path, "results")
         basename = self.FILE_NAMES['combined_summary']
         if not os.path.exists(dirname):
             os.makedirs(dirname)
-        fname = os.path.join(dirname, basename)
-        with open(fname, 'w') as f:
+        filename = os.path.join(dirname, basename)
+        with open(filename, 'w') as f:
             json.dump(combined_result, f, indent=2)
-        self.stdout.info("Saved combined summary in `{}`".format(fname))
+        self.stdout.info("Saved combined summary in `{}`".format(filename))
             
     def get_dataframe(self, syst_type, simplified=True):
         if syst_type == "yield":
             df = self.yield_syst_module.get_valid_dataframe("yield")
         elif syst_type == "shape":
             df = self.shape_syst_module.dataframe
         elif syst_type == "position_shape":
```

### Comparing `quickstats-0.6.8.6/quickstats/clis/core.py` & `quickstats-0.6.8.8/quickstats/clis/core.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.6/quickstats/clis/inspect_rfile.py` & `quickstats-0.6.8.8/quickstats/clis/inspect_rfile.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.6/quickstats/clis/inspect_ws.py` & `quickstats-0.6.8.8/quickstats/clis/inspect_ws.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.6/quickstats/clis/likelihood_fit.py` & `quickstats-0.6.8.8/quickstats/clis/likelihood_fit.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.6/quickstats/clis/likelihood_scan.py` & `quickstats-0.6.8.8/quickstats/clis/likelihood_scan.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,28 +79,31 @@
               help='Optimize constant terms.')
 @click.option('--improve', type=int, default=0, show_default=True,
               help='Execute improve after each minimization')
 @click.option('--minimizer_offset', type=int, default=1, show_default=True,
               help='Enable minimizer offsetting')
 @click.option('--offset/--no-offset', default=True, show_default=True,
               help='Offset likelihood.')
+@click.option('--allow-nan/--not-allow-nan', default=True, show_default=True,
+              help='Allow cached nll to be nan.')
 @click.option('-v', '--verbosity', default='INFO', show_default=True,
               type=click.Choice(["DEBUG", "INFO", "WARNING", "ERROR"], case_sensitive=False),
               help='Verbosity level.')
 @click.option('--parallel', type=int, default=-1, show_default=True,
               help='\b\n Parallelize job across the N workers.'
                    '\b\n Case  0: Jobs are run sequentially (for debugging).'
                    '\b\n Case -1: Jobs are run across N_CPU workers.')
 def likelihood_scan(**kwargs):
     """
     Evaluate a set of parmeterised likelihood values
     """
     _kwargs = {}
     for arg_name in ["input_file", "param_expr", "data_name", "outdir", "filter_expr", "uncond_snapshot",
-                     "exclude_expr", "outname", "cache", "cachedir", "save_log", "parallel", "verbosity"]:
+                     "exclude_expr", "outname", "cache", "cachedir", "save_log", "parallel", "verbosity",
+                     "allow_nan"]:
         _kwargs[arg_name] = kwargs.pop(arg_name)
     _kwargs['config'] = kwargs
     
     # for backward compatibility
     _deprecated_kwargs = {}
     for arg_name in ["poi_min", "poi_max", "poi_step", "poi_name"]:
         _deprecated_kwargs[arg_name] = kwargs.pop(arg_name)
```

### Comparing `quickstats-0.6.8.6/quickstats/clis/limit_setting.py` & `quickstats-0.6.8.8/quickstats/clis/limit_setting.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.6/quickstats/clis/processor_cli.py` & `quickstats-0.6.8.8/quickstats/clis/processor_cli.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,26 +4,28 @@
 @click.command(name='process_rfile')
 @click.option('-i', '--input_file', 'filename', required=True, 
               help='Input ROOT file to process.')
 @click.option('-c', '--config', 'config_path', required=True,
               help='Path to the processor card.')
 @click.option('--multithread/--no-multirhread', default=True, show_default=True,
               help='Enable implicit multi-threading.')
-@click.option('-t', '--tag', default=None,
-              help='Include `tag` as a global variable.')
+@click.option('-g', '--global', 'glob', default=None,
+              help='Include global variables in the form "<name>=<value>,..."')
 @click.option('-f', '--flag', default=None,
               help='Flags to set (separated by commas).')
 @click.option('-v', '--verbosity',  default="INFO", show_default=True,
               help='verbosity level ("DEBUG", "INFO", "WARNING", "ERROR")')
-def process_rfile(filename, config_path, multithread, tag, flag, verbosity):
+def process_rfile(filename, config_path, multithread, glob, flag, verbosity):
     """
     Process a ROOT file based on RDataFrame routines.
     """
     from quickstats.components.processors import RooProcessor
+    from quickstats.components.processors.actions import RooProcGlobalVariables
     from quickstats.utils.string_utils import split_str
     if flag is not None:
         flags = split_str(flag, sep=',', remove_empty=True)
     else:
         flags = []
     rprocessor = RooProcessor(config_path, multithread=multithread, flags=flags, verbosity=verbosity)
-    rprocessor.global_variables['tag'] = tag
+    global_variables = RooProcGlobalVariables._parse(glob)
+    rprocessor.global_variables.update(global_variables)
     rprocessor.run(filename)
```

### Comparing `quickstats-0.6.8.6/quickstats/clis/workspace_tools.py` & `quickstats-0.6.8.8/quickstats/clis/workspace_tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -135,19 +135,20 @@
               default=kDefaultItems, show_default=True,
               help='Items to include in the comparison (seperated by commas).')
 @click.option('--indent', default="   ", show_default=True,
               help='Indentation for each row.')
 @click.option('--visibility', default=kDefaultVisibility, show_default=True,
               help='\b\n Set visibility of the items included in the comparison:'
                    '\b\n boolean mask for showing definitions of certain objects'
-                   '\b\n 0b00001 = show definitions for unique objects'
-                   '\b\n 0b00010 = show definitions for redefined objects'
-                   '\b\n 0b00100 = show definitions for reconstituted objects'
-                   '\b\n 0b01000 = show definitions for renamed/remapped objects'
-                   '\b\n 0b10000 = show definitions for identical objects')
+                   '\b\n 0b000001 = show definitions for unique objects'
+                   '\b\n 0b000010 = show definitions for redefined objects'
+                   '\b\n 0b000100 = show definitions for reconstituted objects'
+                   '\b\n 0b001000 = show definitions for renamed/remapped objects'
+                   '\b\n 0b010000 = show definitions for identical objects'
+                   '\b\n 0b100000 = show definitions for regrouped objects')
 @click.option('--save_text', default=None,
               help='Save summary print out as a text file.')
 @click.option('--save_json_data', default=None,
               help='Save comparison data as a json file.')
 @click.option('--save_excel_data', default=None,
               help='Save comparison data as an excel file.')
 @click.option('-v', '--verbosity',  default="INFO", show_default=True,
```

### Comparing `quickstats-0.6.8.6/quickstats/components/__init__.py` & `quickstats-0.6.8.8/quickstats/components/__init__.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.6/quickstats/components/analysis_base.py` & `quickstats-0.6.8.8/quickstats/components/analysis_base.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.6/quickstats/components/analysis_object.py` & `quickstats-0.6.8.8/quickstats/components/analysis_object.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
         self._use_blind_range = False
         if minimizer_cls is None:
             self.minimizer_cls = ExtendedMinimizer
         else:
             self.minimizer_cls = minimizer_cls
         if filename is not None:
             model_options = {
-                "fname"             : filename,
+                "filename"          : filename,
                 "ws_name"           : ws_name,
                 "mc_name"           : mc_name,
                 "data_name"         : data_name,
                 "snapshot_name"     : snapshot_name,
                 "binned_likelihood" : binned_likelihood,
                 "fix_cache"         : fix_cache,
                 "fix_multi"         : fix_multi
```

### Comparing `quickstats-0.6.8.6/quickstats/components/asimov_generator.py` & `quickstats-0.6.8.8/quickstats/components/asimov_generator.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.6/quickstats/components/asymptotic_cls.py` & `quickstats-0.6.8.8/quickstats/components/asymptotic_cls.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.6/quickstats/components/basics.py` & `quickstats-0.6.8.8/quickstats/components/basics.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.6/quickstats/components/extended_minimizer.py` & `quickstats-0.6.8.8/quickstats/components/extended_minimizer.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.6/quickstats/components/extended_model.py` & `quickstats-0.6.8.8/quickstats/components/extended_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,21 +54,21 @@
     }
     
     _DEFAULT_CONTENT_ = {
         WSArgument.PDF: kClassName|kName|kArgs,
         WSArgument.FUNCTION: kClassName|kName|kArgs
     }
     
-    def __init__(self, fname:str, ws_name:Optional[str]=None, mc_name:Optional[str]=None,
+    def __init__(self, filename:str, ws_name:Optional[str]=None, mc_name:Optional[str]=None,
                  data_name:Optional[str]="combData", snapshot_name:Optional[Union[List[str], str]]=None,
                  binned_likelihood:bool=True, tag_as_measurement:Optional[str]=None,
                  fix_cache:bool=True, fix_multi:bool=True, interpolation_code:int=-1,
                  load_extension:bool=True, minimizer_cls=None, verbosity:Optional[Union[int, str]]="INFO"):
         super().__init__(verbosity=verbosity)
-        self.fname = fname
+        self.filename = filename
         self.ws_name = ws_name
         self.mc_name = mc_name
         self.data_name = data_name
         self.initial_snapshots = snapshot_name
         self.binned_likelihood = binned_likelihood
         self.tag_as_measurement = tag_as_measurement
         self.fix_cache = fix_cache
@@ -194,35 +194,35 @@
             if self.workspace.getSnapshot(snapshot_name):
                 self.workspace.loadSnapshot(snapshot_name)
                 self.stdout.info(f'Loaded snapshot "{snapshot_name}"')
             else:
                 self.stdout.warning(f'Failed to load snapshot "{snapshot_name}"')
             
     def initialize(self):
-        if isinstance(self.fname, str):
-            if not os.path.exists(self.fname):
-                raise FileNotFoundError(f'workspace file "{self.fname}" does not exist')
-            self.stdout.info(f'Opening file "{self.fname}"')
-            file = ROOT.TFile(self.fname) 
+        if isinstance(self.filename, str):
+            if not os.path.exists(self.filename):
+                raise FileNotFoundError(f'workspace file "{self.filename}" does not exist')
+            self.stdout.info(f'Opening file "{self.filename}"')
+            file = ROOT.TFile(self.filename) 
             if (not file):
-                raise RuntimeError(f"Something went wrong while loading the root file: {self.fname}")
+                raise RuntimeError(f"Something went wrong while loading the root file: {self.filename}")
             # load workspace
             if self.ws_name is None:
                 ws_names = [i.GetName() for i in file.GetListOfKeys() if i.GetClassName() == 'RooWorkspace']
                 if not ws_names:
-                    raise RuntimeError(f"No workspaces found in the root file: {self.fname}")
+                    raise RuntimeError(f"No workspaces found in the root file: {self.filename}")
                 if len(ws_names) > 1:
                     self.stdout.warning("Found multiple workspace instances from the root file: "
-                                        f"{self.fname}. Available workspaces are \"{','.join(ws_names)}\". "
+                                        f"{self.filename}. Available workspaces are \"{','.join(ws_names)}\". "
                                         f"Will choose the first one by default")
                 self.ws_name = ws_names[0]
             ws = file.Get(self.ws_name)
-        elif isinstance(self.fname, ROOT.RooWorkspace):
+        elif isinstance(self.filename, ROOT.RooWorkspace):
             file = None
-            ws = self.fname
+            ws = self.filename
         if not ws:
             raise RuntimeError(f'failed to load workspace "{self.ws_name}"')
         self.ws_name = ws.GetName()
         self.stdout.info(f'Loaded workspace "{self.ws_name}"')
         
         # load model config
         if self.mc_name is None:
@@ -354,14 +354,17 @@
         
     def fix_parameters(self, param_setup_expr:Optional[str]=None, source:Optional["ROOT.RooArgSet"]=None):
         return self.set_parameters_with_expression(param_setup_expr, source, mode=SetValueMode.FIX)
     
     def profile_parameters(self, param_setup_expr:Optional[str]=None, source:Optional["ROOT.RooArgSet"]=None):
         return self.set_parameters_with_expression(param_setup_expr, source, mode=SetValueMode.FREE)
     
+    def reset_parameters(self, param_setup_expr:Optional[str]=None, source:Optional["ROOT.RooArgSet"]=None):
+        return self.set_parameters_with_expression(param_setup_expr, source, mode=SetValueMode.UNCHANGED)
+    
     @semistaticmethod
     def _parse_param_setup(self, source:"ROOT.RooArgSet",
                            param_setup:Optional[Union[float, Dict, Sequence]]=None,
                            fill_missing:bool=False,
                            strict_match:bool=True):
         if isinstance(source, ROOT.RooRealVar):
             source = ROOT.RooArgSet(source)
@@ -478,14 +481,18 @@
         elif (setup['vmax'] is not None):
             if (setup['value'] > setup['vmax']):
                 setup['value'] = setup['vmax']
              # upper bound is zero, if original value is positive, will flip to negative value
             if (setup['vmax'] == 0) and (old_value > 0):
                 setup['value'] = -abs(old_value)
             param.setMax(setup['vmax'])
+        if (setup['value'] < param.getMin()):
+            param.setMin(setup['value'])
+        elif (setup['value'] > param.getMax()):
+            param.setMax(setup['value'])
         # set parameter value
         if setup['value'] != old_value:
             param.setVal(setup['value'])
         # set error value
         if setup['error'] is not None:
             param.setError(setup['error'])
             error_str = f'+/- {param.getError()} '
@@ -1320,28 +1327,28 @@
             modifier.create_modified_workspace(self.workspace, filename,
                                                import_class_code=False,
                                                recreate=recreate)
         else:
             self.workspace.writeToFile(filename, recreate)
     
     @semistaticmethod
-    def load_ws(self, fname:str, ws_name:Optional[str]=None, mc_name:Optional[str]=None):
-        if not os.path.exists(fname):
-            raise FileNotFoundError(f'workspace file {fname} does not exist')
-        file = ROOT.TFile(fname)
+    def load_ws(self, filename:str, ws_name:Optional[str]=None, mc_name:Optional[str]=None):
+        if not os.path.exists(filename):
+            raise FileNotFoundError(f'workspace file {filename} does not exist')
+        file = ROOT.TFile(filename)
         if (not file):
-            raise RuntimeError(f"Something went wrong while loading the root file: {fname}")        
+            raise RuntimeError(f"Something went wrong while loading the root file: {filename}")        
         # load workspace
         if ws_name is None:
             ws_names = [i.GetName() for i in file.GetListOfKeys() if i.GetClassName() == 'RooWorkspace']
             if not ws_names:
-                raise RuntimeError(f"No workspaces found in the root file: {fname}")
+                raise RuntimeError(f"No workspaces found in the root file: {filename}")
             if len(ws_names) > 1:
                 self.stdout.warning("Found multiple workspace instances from the root file: {}. Available workspaces"
-                      " are \"{}\". Will choose the first one by default".format(fname, ','.join(ws_names)))
+                      " are \"{}\". Will choose the first one by default".format(filename, ','.join(ws_names)))
             ws_name = ws_names[0]
         ws = file.Get(ws_name)
         if not ws:
             raise RuntimeError('Failed to load workspace: "{}"'.format(ws_name))
         # load model config
         if mc_name is None:
             mc_names = [i.GetName() for i in ws.allGenericObjects() if 'ModelConfig' in i.ClassName()]
```

### Comparing `quickstats-0.6.8.6/quickstats/components/extended_rfile.py` & `quickstats-0.6.8.8/quickstats/components/extended_rfile.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,27 +64,27 @@
         self._cache  = []
         self._components = []        
         
         # initialize from ROOT file
         if isinstance(source, str):
             if not os.path.exists(source):
                 raise FileNotFoundError(f"workspace file {source} does not exist")
-            self.stdout.info('Opening file "{}"'.format(self.fname))
+            self.stdout.info(f'Opening file "{source}"')
             file = ROOT.TFile(source) 
             if self.is_corrupt(file):
                 raise RuntimeError(f"corrupted file: {source}")
             self._file = file
-            self.fname = source
+            self.filename = source
             if tree_name is not None:
                 self.set_tree(tree_name)
         elif isinstance(source, dict):
             self._rdf = ROOT.RDF.MakeNumpyDataFrame(source)
             self._rdf_map[None] = self._rdf
             self._file = None
-            self.fname = None
+            self.filename = None
         else:
             import pandas as pd
             if isinstance(source, pd.DataFrame):
                 from quickstats.interface.root.data_conversion import dataframe2numpy
                 source = dataframe2numpy(source)
                 self.initialize(source)
             else:
@@ -98,15 +98,15 @@
         self.create_canvas()
         self.canvas.Draw()
     
     def add_tree(self, tree_name:str):
         if tree_name in self._rdf_map:
             self.stdout.info("Tree already added to the rdf collection.")
             return None
-        rdf = ROOT.RDataFrame(tree_name, self.fname)
+        rdf = ROOT.RDataFrame(tree_name, self.filename)
         if not rdf:
             raise RuntimeError(f"failed to load tree \"{tree_name}\"")
         self._rdf_map[tree_name] = rdf
         self.stdout.info(f"Added tree \"{tree_name}\" to the rdf collection")
         
     def set_tree(self, tree_name:str):
         if tree_name not in self._rdf_map:
@@ -149,15 +149,15 @@
     def add_cache(self, robject:ROOT.TObject):
         self.stdout.info(f"Added object \"{robject.GetName()}\" to cache")
         self._cache.append(robject)
         
     def clear_cache(self):
         self._cache = []
     
-    def save_components(self, fname:str, mode:str="RECREATE", components:Optional[List]=None):
+    def save_components(self, filename:str, mode:str="RECREATE", components:Optional[List]=None):
         if components is None:
             components = self.components
-        f = ROOT.TFile(fname, mode)
+        f = ROOT.TFile(filename, mode)
         f.cd()
         for component in components:
             component.Write()
         f.Close()
```

### Comparing `quickstats-0.6.8.6/quickstats/components/likelihood.py` & `quickstats-0.6.8.8/quickstats/components/likelihood.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.6/quickstats/components/modelling/component_source.py` & `quickstats-0.6.8.8/quickstats/components/modelling/component_source.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.6/quickstats/components/modelling/data_modelling.py` & `quickstats-0.6.8.8/quickstats/components/modelling/data_modelling.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.6/quickstats/components/modelling/model_source.py` & `quickstats-0.6.8.8/quickstats/components/modelling/model_source.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.6/quickstats/components/modelling/parameter_templates.py` & `quickstats-0.6.8.8/quickstats/components/modelling/parameter_templates.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.6/quickstats/components/modelling/pdf_fit_tool.py` & `quickstats-0.6.8.8/quickstats/components/modelling/pdf_fit_tool.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.6/quickstats/components/modelling/tree_data_source.py` & `quickstats-0.6.8.8/quickstats/components/modelling/tree_data_source.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.6/quickstats/components/nuisance_parameter_harmonizer.py` & `quickstats-0.6.8.8/quickstats/components/nuisance_parameter_harmonizer.py`

 * *Files 1% similar despite different names*

```diff
@@ -194,15 +194,16 @@
         self.display_mappings(mappings, self.ref_list)
         flattened_mappings = self.flatten_mappings(mappings)
         unknown_nuis = list(set(nuis_names) - set(flattened_mappings))
         if len(unknown_nuis) > 0:
             print('Remained NPs:')
             for unknown in unknown_nuis:
                 NuisanceParameterHarmonizer.display_difference(unknown, '?')
-        flattened_mappings.update({np:None for np in unknown_nuis})
+        # keep name for unknown nuisance parameter
+        flattened_mappings.update({np:np for np in unknown_nuis})
         return flattened_mappings
     
     def harmonize(self, ws_paths, outfile=None):
         if isinstance(ws_paths, str):
             ws_paths = [ws_paths]
         timely_info('Harmonizing collective workspace files', ','.join(ws_paths))
         nuis_names = NuisanceParameterHarmonizer.get_nuiance_parameter_names_collection(ws_paths)
```

### Comparing `quickstats-0.6.8.6/quickstats/components/nuisance_parameter_pull.py` & `quickstats-0.6.8.8/quickstats/components/nuisance_parameter_pull.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,14 +83,16 @@
                    precision:float=0.001, eps:float=1.0, retry:int=0, strategy:int=0, print_level:int=1,
                    num_cpu:int=1, offset:bool=True, optimize:int=2, eigen:bool=False,
                    fix_cache:bool=True, fix_multi:bool=True, max_calls:int=-1, 
                    max_iters:int=-1, batch_mode:bool=False, int_bin_precision:float=-1.,
                    outdir:str='pulls', cache=True, logfile_path=None,
                    minimizer_cls=None, verbosity:str="INFO", **kwargs):
         stdout = VerbosePrint(verbosity)
+        stdout.warning("The NuisanceParameterPull class is deprecated. "
+                       "Please switch to the NuisanceParameterRanking class instead")
         # create output directory if not exists
         if not os.path.exists(outdir):
             os.makedirs(outdir, exist_ok=True)        
         outname_root = os.path.join(outdir, nuis_name + '.root')
         outname_json = os.path.join(outdir, nuis_name + '.json')
         #checkpointing:
         if (os.path.exists(outname_root) and os.path.exists(outname_json)) and cache:
@@ -98,15 +100,15 @@
             return None
         else:
             stdout.info('Evaluating pulls for the NP: {}'.format(nuis_name))
         if logfile_path is not None:
             common_utils.redirect_stdout(logfile_path)
         start_time = time.time()
         # load model
-        model = ExtendedModel(fname=filename, ws_name=ws_name,
+        model = ExtendedModel(filename=filename, ws_name=ws_name,
                               mc_name=mc_name, data_name=data_name, 
                               snapshot_name=snapshot_name, binned_likelihood=binned_likelihood,
                               fix_cache=fix_cache, fix_multi=fix_multi,
                               verbosity=verbosity)
         if fix_param:
             model.fix_parameters(fix_param)
             
@@ -331,12 +333,12 @@
                      repeat(max_calls), repeat(max_iters), repeat(batch_mode),
                      repeat(int_bin_precision), repeat(outdir), repeat(cache), logfile_paths,
                      repeat(minimizer_cls), repeat(verbosity))
         common_utils.execute_multi_tasks(self._run_pulls, *arguments, parallel=parallel)
 
         
     @staticmethod
-    def parse_root_result(fname):
+    def parse_root_result(filename:str):
         import uproot
-        with uproot.open(fname) as file:
+        with uproot.open(filename) as file:
             result = root_utils.uproot_to_dict(file)
         return result
```

### Comparing `quickstats-0.6.8.6/quickstats/components/nuisance_parameter_ranking.py` & `quickstats-0.6.8.8/quickstats/components/nuisance_parameter_ranking.py`

 * *Files 0% similar despite different names*

```diff
@@ -253,12 +253,12 @@
         r_tree = ROOT.TTree(treename, treename)
         root_utils.fill_branch(r_tree, root_data)
         r_file.Write()
         r_file.Close()
         self.stdout(f'INFO: Saved NP pulls and impact output to {outname}')
         
     @staticmethod
-    def parse_root_result(fname):
+    def parse_root_result(filename):
         import uproot
-        with uproot.open(fname) as file:
+        with uproot.open(filename) as file:
             result = root_utils.uproot_to_dict(file)
         return result
```

### Comparing `quickstats-0.6.8.6/quickstats/components/processors/actions/__init__.py` & `quickstats-0.6.8.8/quickstats/components/processors/actions/__init__.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.6/quickstats/components/processors/actions/rooproc_alias.py` & `quickstats-0.6.8.8/quickstats/components/processors/actions/rooproc_alias.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.6/quickstats/components/processors/actions/rooproc_as_numpy.py` & `quickstats-0.6.8.8/quickstats/components/processors/actions/rooproc_as_numpy.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.6/quickstats/components/processors/actions/rooproc_base_action.py` & `quickstats-0.6.8.8/quickstats/components/processors/actions/rooproc_base_action.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,16 +38,16 @@
                 substitute = global_vars[literal]
                 v = v.replace("${" + literal + "}", str(substitute))
             if is_list:
                 v = v.split("__SEPARATOR__")
             formatted_parameters[k] = v
         return formatted_parameters
     
-    def makedirs(self, fname:str):
-        dirname = os.path.dirname(fname)
+    def makedirs(self, filename:str):
+        dirname = os.path.dirname(filename)
         if dirname and (not os.path.exists(dirname)):
             os.makedirs(dirname)
     
     def execute(self, **params):
         raise NotImplementedError
     
     @classmethod
```

### Comparing `quickstats-0.6.8.6/quickstats/components/processors/actions/rooproc_declare.py` & `quickstats-0.6.8.8/quickstats/components/processors/actions/rooproc_declare.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.6/quickstats/components/processors/actions/rooproc_define.py` & `quickstats-0.6.8.8/quickstats/components/processors/actions/rooproc_define.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.6/quickstats/components/processors/actions/rooproc_export.py` & `quickstats-0.6.8.8/quickstats/components/processors/actions/rooproc_export.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.6/quickstats/components/processors/actions/rooproc_filter.py` & `quickstats-0.6.8.8/quickstats/components/processors/actions/rooproc_filter.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.6/quickstats/components/processors/actions/rooproc_global_variables.py` & `quickstats-0.6.8.8/quickstats/components/processors/actions/rooproc_global_variables.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,25 +5,30 @@
 
 class RooProcGlobalVariables(RooProcHelperAction):
     
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
         
     def commarepl(matchobj):
-        return matchobj.group(0).replace(",", "::COMMA::")        
-        
+        return matchobj.group(0).replace(",", "::COMMA::")
+    
     @classmethod
-    def parse(cls, main_text:str, block_text:Optional[str]=None):
+    def _parse(cls, main_text:str, block_text:Optional[str]=None):
         main_text = re.sub(r"\s*", "", main_text)
         main_text = re.sub(r'\[(.*?)\]', cls.commarepl, main_text)
         tokens = [token.replace("::COMMA::", ",") for token in main_text.split(",")]
         global_variables = {}
         for token in tokens:
             result = re.match("^(\w+)=(.*)", token)
             if not result:
                 raise RuntimeError(f"invalid expression {token}")
             global_variables[result[1]] = result[2]
+        return global_variables
+        
+    @classmethod
+    def parse(cls, main_text:str, block_text:Optional[str]=None):
+        global_variables = cls._parse(main_text, block_text)
         return cls(**global_variables)
     
     def _execute(self, processor:"quickstats.RooProcessor", **params):
         processor.global_variables.update(params)
         return processor
```

### Comparing `quickstats-0.6.8.6/quickstats/components/processors/actions/rooproc_hybrid_action.py` & `quickstats-0.6.8.8/quickstats/components/processors/actions/rooproc_hybrid_action.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.6/quickstats/components/processors/actions/rooproc_if_defined.py` & `quickstats-0.6.8.8/quickstats/components/processors/actions/rooproc_if_defined.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.6/quickstats/components/processors/actions/rooproc_if_not_defined.py` & `quickstats-0.6.8.8/quickstats/components/processors/actions/rooproc_if_not_defined.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.6/quickstats/components/processors/actions/rooproc_load_frame.py` & `quickstats-0.6.8.8/quickstats/components/processors/actions/rooproc_load_frame.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.6/quickstats/components/processors/actions/rooproc_load_macro.py` & `quickstats-0.6.8.8/quickstats/components/processors/actions/rooproc_load_macro.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.6/quickstats/components/processors/actions/rooproc_nested_action.py` & `quickstats-0.6.8.8/quickstats/components/processors/actions/rooproc_nested_action.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.6/quickstats/components/processors/actions/rooproc_report.py` & `quickstats-0.6.8.8/quickstats/components/processors/actions/rooproc_report.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.6/quickstats/components/processors/actions/rooproc_safe_alias.py` & `quickstats-0.6.8.8/quickstats/components/processors/actions/rooproc_safe_alias.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.6/quickstats/components/processors/actions/rooproc_save.py` & `quickstats-0.6.8.8/quickstats/components/processors/actions/rooproc_save.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.6/quickstats/components/processors/actions/rooproc_save_frame.py` & `quickstats-0.6.8.8/quickstats/components/processors/actions/rooproc_save_frame.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.6/quickstats/components/processors/actions/rooproc_stat.py` & `quickstats-0.6.8.8/quickstats/components/processors/actions/rooproc_stat.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.6/quickstats/components/processors/actions/rooproc_treename.py` & `quickstats-0.6.8.8/quickstats/components/processors/actions/rooproc_treename.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.6/quickstats/components/processors/builtin_methods.py` & `quickstats-0.6.8.8/quickstats/components/processors/builtin_methods.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.6/quickstats/components/processors/roo_config_parser.py` & `quickstats-0.6.8.8/quickstats/components/processors/roo_config_parser.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.6/quickstats/components/processors/roo_processor.py` & `quickstats-0.6.8.8/quickstats/components/processors/roo_processor.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,25 +82,25 @@
         self.flags = list(flags)        
         
     def cleanup(self):
         close_all_root_files()
         self.rdf_frames = {}
         self.rdf = None
         
-    def _get_all_files(self, filename:Union[List[str], str]):
+    def _get_all_files(self, filenames:Union[List[str], str]):
         all_files = []
         if isinstance(filename, str):
             filename = [filename]
         if not isinstance(filename, list):
             raise ValueError("filename must be either string or list of strings")
-        for fname in filename:
-            if os.path.isdir(fname):
-                all_files += glob.glob(os.path.join(fname, "*.root"))
+        for filename in filenames:
+            if os.path.isdir(filename):
+                all_files += glob.glob(os.path.join(filename, "*.root"))
             else:
-                all_files += glob.glob(fname)
+                all_files += glob.glob(filename)
         if not all_files:
             raise FileNotFoundError(f'file "{filename}" does not exist')
         PathManager.check_files(all_files)
         valid_files = []
         for file in all_files:
             rf = ROOT.TFile(file)
             if TFile.is_corrupt(rf):
@@ -147,17 +147,17 @@
             raise RuntimeError("action tree not initialized")        
         if not self.action_tree.root_node.has_child:
             self.stdout.warning("No actions to be performed.")
             return None
         if self.treename is None:
             raise RuntimeError("tree name is undefined")
     
-    def run(self, filename:Union[List[str], str]):
+    def run(self, filenames:Union[List[str], str]):
         self.sanity_check()
-        all_files = self._get_all_files(filename)
+        all_files = self._get_all_files(filenames)
         if len(all_files) == 0:
             self.stdout.info(f'No files to be processed. Skipped.')
             return None
         elif len(all_files) == 1:
             self.stdout.info(f'Processing file "{all_files[0]}".')
         else:
             self.stdout.info(f"Professing files")
```

### Comparing `quickstats-0.6.8.6/quickstats/components/pvalue_toys.py` & `quickstats-0.6.8.8/quickstats/components/pvalue_toys.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.6/quickstats/components/roo_inspector.py` & `quickstats-0.6.8.8/quickstats/components/roo_inspector.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,35 +11,35 @@
 
 class RooInspector(AbstractObject):
     def __init__(self, tree_name:str, file_expr:Union[str, List[str]], 
                  filter_expr:Optional[str]=None,
                  verbosity:Optional[Union[int, str]]="INFO"):
         super().__init__(verbosity=verbosity)
         self.tree_name = tree_name
-        self.fnames = self._parse_file_expr(file_expr)
+        self.filenames = self._parse_file_expr(file_expr)
         self.initialise(filter_expr=filter_expr)
         
     def _parse_file_expr(self, file_expr:Union[str, List[str]])->List[str]:
-        fnames = []
+        filenames = []
         if isinstance(file_expr, str):
             return self._parse_file_expr([file_expr])
         else:
             for expr in file_expr:
                 if os.path.isdir(expr):
                     file_expr = os.path.join(expr, "*.root")
-                fnames_i = glob.glob(expr)
-                if not fnames_i:
+                filenames_i = glob.glob(expr)
+                if not filenames_i:
                     self.stdout.warning(f"No root files found matching the expression {expr}")
-                fnames += fnames_i
-        if not fnames:
+                filenames.extend(filenames_i)
+        if not filenames:
             raise RuntimeError("no root files found from the given file expression")
-        return fnames
+        return filenames
     
     def initialise(self, filter_expr:Optional[str]=None):
-        self.rdf = ROOT.RDataFrame(self.tree_name, self.fnames)
+        self.rdf = ROOT.RDataFrame(self.tree_name, self.filenames)
         if filter_expr is not None:
             self.rdf = self.rdf.Filter(filter_expr)
         
     def get_column_names(self)->List[str]:
         column_names = sorted([str(i) for i in self.rdf.GetColumnNames()])
         return column_names
```

### Comparing `quickstats-0.6.8.6/quickstats/components/root_object.py` & `quickstats-0.6.8.8/quickstats/components/root_object.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.6/quickstats/components/toy_limit_calculator.py` & `quickstats-0.6.8.8/quickstats/components/toy_limit_calculator.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.6/quickstats/components/workspaces/__init__.py` & `quickstats-0.6.8.8/quickstats/components/workspaces/__init__.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.6/quickstats/components/workspaces/asimov_handler.py` & `quickstats-0.6.8.8/quickstats/components/workspaces/asimov_handler.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.6/quickstats/components/workspaces/core_argument_sets.py` & `quickstats-0.6.8.8/quickstats/components/workspaces/core_argument_sets.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.6/quickstats/components/workspaces/sample.py` & `quickstats-0.6.8.8/quickstats/components/workspaces/sample.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.6/quickstats/components/workspaces/settings.py` & `quickstats-0.6.8.8/quickstats/components/workspaces/settings.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.6/quickstats/components/workspaces/systematic.py` & `quickstats-0.6.8.8/quickstats/components/workspaces/systematic.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.6/quickstats/components/workspaces/systematics_domain.py` & `quickstats-0.6.8.8/quickstats/components/workspaces/systematics_domain.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.6/quickstats/components/workspaces/ws_comparer.py` & `quickstats-0.6.8.8/quickstats/components/workspaces/ws_comparer.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.6/quickstats/components/workspaces/ws_decomposer.py` & `quickstats-0.6.8.8/quickstats/components/workspaces/ws_decomposer.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.6/quickstats/components/workspaces/ws_modifier_config.py` & `quickstats-0.6.8.8/quickstats/components/workspaces/ws_modifier_config.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.6/quickstats/components/workspaces/xml_ws_base.py` & `quickstats-0.6.8.8/quickstats/components/workspaces/xml_ws_base.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.6/quickstats/components/workspaces/xml_ws_builder_v1.py` & `quickstats-0.6.8.8/quickstats/components/workspaces/xml_ws_builder_v1.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.6/quickstats/components/workspaces/xml_ws_builder_v2.py` & `quickstats-0.6.8.8/quickstats/components/workspaces/xml_ws_builder_v2.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.6/quickstats/components/workspaces/xml_ws_combiner.py` & `quickstats-0.6.8.8/quickstats/components/workspaces/xml_ws_combiner.py`

 * *Files 0% similar despite different names*

```diff
@@ -296,15 +296,15 @@
                 
     def validate_channel_input(self, channel:str):
         self._channel_check(channel)
         self.stdout.info(f"Checking input workspace for the channel \"{channel}\".")
         channel_config = self.channel_config[channel]
         model = self._get_channel_model(channel_config)
         strict_mode = self.combination_config["strict"]
-        ws_filename = model.fname
+        ws_filename = model.filename
         renamed_pdfs = list(channel_config["rename_map"]["pdf"])
         renamed_vars = list(channel_config["rename_map"]["var"])
         renamed_pois = list(channel_config["poi_map"].values())
         renamed_constraint = channel_config["renamed_constraint"]
         missing_obj_msg = f'{{obj_type}} "{{obj_name}}" does not exist in the workspace "{ws_filename}"'
         for pdf_name in renamed_pdfs:
             nuis_name = renamed_constraint[pdf_name]["nuis"]
```

### Comparing `quickstats-0.6.8.6/quickstats/components/workspaces/xml_ws_modifier.py` & `quickstats-0.6.8.8/quickstats/components/workspaces/xml_ws_modifier.py`

 * *Files 1% similar despite different names*

```diff
@@ -90,14 +90,15 @@
             "snapshot_globs"     : source.pop("snapshot_globs", []),
             "snapshot_pois"      : source.pop("snapshot_pois", []),
             "snapshot_all"       : source.pop("snapshot_all", []),
             "snapshot_list"      : source.pop("snapshot_list", []),
             "dataset_list"       : source.pop("dataset_list", None),
             "fix_parameters"     : source.pop("fix_parameters", None),
             "profile_parameters" : source.pop("profile_parameters", None),
+            "reset_parameters"   : source.pop("reset_parameters", None),
             "strict"             : source.pop("strict", True)
         }
         if source:
             unknown_attributes = list(source)
             self.stdout.warning(f"The following unrecognized configuration attribute(s) will be ignored: "
                                 f"{', '.join(unknown_attributes)}")
         actions = {
@@ -166,14 +167,15 @@
             'snapshot_globs'   : self._get_node_attrib(root, "SnapshotGO", required=False, default=[], dtype="str_list"),
             'snapshot_pois'    : self._get_node_attrib(root, "SnapshotPOI", required=False, default=[], dtype="str_list"),
             'snapshot_all'     : self._get_node_attrib(root, "SnapshotAll", required=False, default=[], dtype="str_list"),
             'snapshot_list'    : self._get_node_attrib(root, "SnapshotList", required=False, default=[], dtype="str_list"),
             'dataset_list'     : self._get_node_attrib(root, "DatasetList", required=False, default=None, dtype="str_list"),
             "fix_parameters"     : self._get_node_attrib(root, "FixParameters", required=False, default=None),
             "profile_parameters" : self._get_node_attrib(root, "ProfileParameters", required=False, default=None),
+            "reset_parameters" : self._get_node_attrib(root, "ResetParameters", required=False, default=None),
             'strict'           : self._get_node_attrib(root, "Strict", required=False, default="true", dtype="bool")
         }
         # for compatibility with older version of workspaceCombiner
         if config['workspace_name'] == "dummy":
             config['workspace_name'] = None
         if config['model_config_name'] == "dummy":
             config['model_config_name'] = None
@@ -376,14 +378,16 @@
         data_name = self.config['data_name']
         model = ExtendedModel(ws, data_name=data_name, verbosity="WARNING")
         model.stdout.verbosity = self.stdout.verbosity
         if self.config["fix_parameters"] is not None:
             model.fix_parameters(self.config["fix_parameters"])
         if self.config["profile_parameters"] is not None:
             model.profile_parameters(self.config["profile_parameters"])
+        if self.config["reset_parameters"] is not None:
+            model.reset_parameters(self.config["reset_parameters"])
 
     def generate_asimov(self, ws:ROOT.RooWorkspace):
         n_asimov = len(self.actions['asimov'])
         if n_asimov == 0:
             return None
         data_name = self.config['data_name']
         asimov_handler = AsimovHandler(ws, data_name=data_name,
```

### Comparing `quickstats-0.6.8.6/quickstats/concurrent/abstract_runner.py` & `quickstats-0.6.8.8/quickstats/concurrent/abstract_runner.py`

 * *Files 5% similar despite different names*

```diff
@@ -45,22 +45,31 @@
         return outpath
     
     def get_instance_logpath(self, kwargs:Dict):
         outpath = self.get_instance_outpath(kwargs)
         if outpath:
             return os.path.splitext(outpath)[0] + ".log"
         return None
+    
+    def _is_valid_cache(self, cached_result):
+        return True
         
     def run_instance(self, kwargs:Dict[str, Any]):
         self._prerun_instance(**kwargs)
         outpath = self.get_instance_outpath(kwargs)
         
         if outpath and (self.config['cache'] and os.path.exists(outpath) and is_valid_file(outpath)):
-            self.stdout.info(f"Cached output from {outpath}")
-            return self._cached_return(outpath)
+            try:
+                cached_result = self._cached_return(outpath)
+                self.stdout.info(f"Cached output from {outpath}")
+                if self._is_valid_cache(cached_result):
+                    return cached_result
+            except:
+                self.stdout.info(f'Broken output: {outpath}. Retrying')
+                pass
         
         logpath = self.get_instance_logpath(kwargs)
         if logpath and self.config['save_log']:
             with standard_log(logpath) as logger:
                 result = self._run_instance(**kwargs)
         else:
             result = self._run_instance(**kwargs)
```

### Comparing `quickstats-0.6.8.6/quickstats/concurrent/logging.py` & `quickstats-0.6.8.8/quickstats/concurrent/logging.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.6/quickstats/concurrent/nuisance_parameter_ranking_runner.py` & `quickstats-0.6.8.8/quickstats/concurrent/nuisance_parameter_ranking_runner.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.6/quickstats/concurrent/parameterised_asymptotic_cls.py` & `quickstats-0.6.8.8/quickstats/concurrent/parameterised_asymptotic_cls.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.6/quickstats/concurrent/parameterised_likelihood.py` & `quickstats-0.6.8.8/quickstats/concurrent/parameterised_likelihood.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import os
 import sys
 import copy
 import json
+import math
 from typing import Optional, Union, Dict, List, Any
 from itertools import repeat
 
 import ROOT
 from quickstats import semistaticmethod
 from quickstats.parsers import ParamParser
 from quickstats.concurrent import ParameterisedRunner
@@ -15,15 +16,15 @@
 
 class ParameterisedLikelihood(ParameterisedRunner):
     def __init__(self, input_file:str, param_expr:str,
                  filter_expr:Optional[str]=None, exclude_expr:Optional[str]=None,
                  data_name:str="combData", uncond_snapshot:Optional[str]=None,
                  config:Optional[Dict]=None, outdir:str="output", cachedir:str="cache",
                  outname:str="{poi_names}.json", cache:bool=True,
-                 save_log:bool=True, parallel:int=-1,
+                 save_log:bool=True, parallel:int=-1, allow_nan:bool=True,
                  verbosity:Optional[Union[int, str]]="INFO"):
         
         super().__init__(file_expr=None, param_expr=param_expr,
                          filter_expr=filter_expr, exclude_expr=exclude_expr,
                          parallel=parallel, timed=True, save_log=save_log,
                          cache=cache, allow_none=True, verbosity=verbosity)
         
@@ -33,14 +34,16 @@
             'uncond_snapshot': uncond_snapshot,
             'config': config,
             'outdir': outdir,
             'cachedir': cachedir,
             'outname': outname
         }
         
+        self.allow_nan = allow_nan
+        
         self.attributes['poi_names'] = ParamParser._get_param_str_attributes(param_expr)
 
     def _prerun_batch(self):
         self.stdout.tips("When running likelihood scan on an Asimov dataset, remember to restore the global "
                          "observables to their Asimov values by loading the appropriate snapshot.")
         outdir = self.attributes['outdir']
         cache_dir = self.get_cache_dir()
@@ -57,29 +60,37 @@
     @semistaticmethod
     def _cached_return(self, outname:str):
         with open(outname, 'r') as f:
             result = json.load(f)
             processed_result = self._process_result(result)
         return processed_result
     
+    def _is_valid_cache(self, cached_result):
+        if (not self.allow_nan) and math.isnan(cached_result['nll']):
+            self.stdout.info('Found cached result with nan nll. Retrying')
+            return False
+        return True
+    
     @semistaticmethod
     def _process_result(self, result:Dict):
         if 'uncond_fit' in result:
             fit_result = result['uncond_fit']
         elif 'cond_fit' in result:
             fit_result = result['cond_fit']
         else:
             raise RuntimeError("unexpected output (expect only conditional/unconditional fit in each task)")        
-        nll   = fit_result['nll']
-        mu    = fit_result.get("mu", {})
-        muhat = fit_result.get("muhat", {})
+        nll    = fit_result['nll']
+        status = fit_result['status']
+        mu     = fit_result.get("mu", {})
+        muhat  = fit_result.get("muhat", {})
         
         processed_result = {
             'nll': nll,
-            'mu' : mu
+            'mu' : mu,
+            'status': status
         }
         processed_result['mu'].update(muhat)
         return processed_result
         
     @semistaticmethod
     def _run_instance(self, filename:str, mode:int,
                       poi_name:Optional[Union[str, List[str]]]=None,
@@ -188,22 +199,24 @@
                     raise RuntimeError(f'NLL evaluation failed for the conditional fit ({param_str}).'
                                        'Please check the log file for more details.')
             if not isinstance(result, dict):
                 raise RuntimeError("found cache result with deprecated format, a rerun "
                                    "is needed")
         uncond_result = raw_result[0]
         uncond_nll = uncond_result['nll']
-        data = {'nll':[], 'qmu':[]}
+        data = {'nll':[], 'qmu':[], 'status': []}
         poi_names = self.attributes['poi_names']
         for poi_name in poi_names:
             data[poi_name] = []
         for result, poi_values in zip(raw_result, points):
             nll   = result['nll']
+            status = result['status']
             data['nll'].append(nll)
             data['qmu'].append(2*(nll-uncond_nll))
+            data['status'].append(status)
             for poi_name in poi_names:
                 mu_map = result['mu']
                 if poi_name not in mu_map:
                     if poi_values is None:
                         raise RuntimeError(f'unable to extract value for the POI "{poi_name}" '
                                            f'for the unconditional fit. Please check the log '
                                            f'file for more details')
```

### Comparing `quickstats-0.6.8.6/quickstats/concurrent/parameterised_runner.py` & `quickstats-0.6.8.8/quickstats/concurrent/parameterised_runner.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.6/quickstats/core/abstract_object.py` & `quickstats-0.6.8.8/quickstats/core/abstract_object.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.6/quickstats/core/configs.py` & `quickstats-0.6.8.8/quickstats/core/configs.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.6/quickstats/core/configurable_object.py` & `quickstats-0.6.8.8/quickstats/core/configurable_object.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.6/quickstats/core/dataclass_object.py` & `quickstats-0.6.8.8/quickstats/core/dataclass_object.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.6/quickstats/core/decorators.py` & `quickstats-0.6.8.8/quickstats/core/decorators.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.6/quickstats/core/enums.py` & `quickstats-0.6.8.8/quickstats/core/enums.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.6/quickstats/core/methods.py` & `quickstats-0.6.8.8/quickstats/core/methods.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.6/quickstats/core/path_manager.py` & `quickstats-0.6.8.8/quickstats/core/path_manager.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.6/quickstats/core/virtual_trees.py` & `quickstats-0.6.8.8/quickstats/core/virtual_trees.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.6/quickstats/interface/cppyy/core.py` & `quickstats-0.6.8.8/quickstats/interface/cppyy/core.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.6/quickstats/interface/cppyy/macros.py` & `quickstats-0.6.8.8/quickstats/interface/cppyy/macros.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.6/quickstats/interface/cppyy/vectorize.py` & `quickstats-0.6.8.8/quickstats/interface/cppyy/vectorize.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.6/quickstats/interface/root/RooAbsData.py` & `quickstats-0.6.8.8/quickstats/interface/root/RooAbsData.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.6/quickstats/interface/root/RooAbsPdf.py` & `quickstats-0.6.8.8/quickstats/interface/root/RooAbsPdf.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.6/quickstats/interface/root/RooCategory.py` & `quickstats-0.6.8.8/quickstats/interface/root/RooCategory.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.6/quickstats/interface/root/RooDataSet.py` & `quickstats-0.6.8.8/quickstats/interface/root/RooDataSet.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.6/quickstats/interface/root/RooMsgService.py` & `quickstats-0.6.8.8/quickstats/interface/root/RooMsgService.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.6/quickstats/interface/root/RooRealVar.py` & `quickstats-0.6.8.8/quickstats/interface/root/RooRealVar.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.6/quickstats/interface/root/TF1.py` & `quickstats-0.6.8.8/quickstats/interface/root/TF1.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.6/quickstats/interface/root/TFile.py` & `quickstats-0.6.8.8/quickstats/interface/root/TFile.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.6/quickstats/interface/root/TH1.py` & `quickstats-0.6.8.8/quickstats/interface/root/TH1.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.6/quickstats/interface/root/TH2.py` & `quickstats-0.6.8.8/quickstats/interface/root/TH2.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.6/quickstats/interface/root/TObject.py` & `quickstats-0.6.8.8/quickstats/interface/root/TObject.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.6/quickstats/interface/root/__init__.py` & `quickstats-0.6.8.8/quickstats/interface/root/__init__.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.6/quickstats/interface/root/helper.py` & `quickstats-0.6.8.8/quickstats/interface/root/helper.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.6/quickstats/interface/root/inspection.py` & `quickstats-0.6.8.8/quickstats/interface/root/inspection.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.6/quickstats/interface/root/macros.py` & `quickstats-0.6.8.8/quickstats/interface/root/macros.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.6/quickstats/interface/root/roofit_extension.py` & `quickstats-0.6.8.8/quickstats/interface/root/roofit_extension.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.6/quickstats/macros/AsymptoticCLsTool/AsymptoticCLsTool.cxx` & `quickstats-0.6.8.8/quickstats/macros/AsymptoticCLsTool/AsymptoticCLsTool.cxx`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.6/quickstats/macros/AsymptoticCLsTool/AsymptoticCLsTool.h` & `quickstats-0.6.8.8/quickstats/macros/AsymptoticCLsTool/AsymptoticCLsTool.h`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.6/quickstats/macros/FlexibleInterpVarMkII/FlexibleInterpVarMkII.cxx` & `quickstats-0.6.8.8/quickstats/macros/FlexibleInterpVarMkII/FlexibleInterpVarMkII.cxx`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.6/quickstats/macros/FlexibleInterpVarMkII/FlexibleInterpVarMkII.h` & `quickstats-0.6.8.8/quickstats/macros/FlexibleInterpVarMkII/FlexibleInterpVarMkII.h`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.6/quickstats/macros/QuickStatsCore/QuickStatsCore.cxx` & `quickstats-0.6.8.8/quickstats/macros/QuickStatsCore/QuickStatsCore.cxx`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.6/quickstats/macros/QuickStatsCore/RooFitExt.cxx` & `quickstats-0.6.8.8/quickstats/macros/QuickStatsCore/RooFitExt.cxx`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.6/quickstats/macros/QuickStatsCore/RooFitExt.h` & `quickstats-0.6.8.8/quickstats/macros/QuickStatsCore/RooFitExt.h`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.6/quickstats/macros/ResponseFunction/ResponseFunction.cxx` & `quickstats-0.6.8.8/quickstats/macros/ResponseFunction/ResponseFunction.cxx`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.6/quickstats/macros/ResponseFunction/ResponseFunction.h` & `quickstats-0.6.8.8/quickstats/macros/ResponseFunction/ResponseFunction.h`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.6/quickstats/macros/RooTwoSidedCBShape/RooTwoSidedCBShape.cxx` & `quickstats-0.6.8.8/quickstats/macros/RooTwoSidedCBShape/RooTwoSidedCBShape.cxx`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.6/quickstats/macros/RooTwoSidedCBShape/RooTwoSidedCBShape.h` & `quickstats-0.6.8.8/quickstats/macros/RooTwoSidedCBShape/RooTwoSidedCBShape.h`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.6/quickstats/maths/interpolation.py` & `quickstats-0.6.8.8/quickstats/maths/interpolation.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,25 @@
 import numpy as np
 
 def get_intervals(x:np.ndarray, y:np.ndarray, level:float, delta:float=0.0001):
     from scipy.interpolate import interp1d
-    func_interp = interp1d(x, y)
+    sort_idx = np.argsort(x)
+    x = x[sort_idx]
+    y = y[sort_idx]
+    func_interp = interp1d(x, y, fill_value="extrapolate")
     x_interp = np.arange(min(x), max(x), delta)
     y_interp = func_interp(x_interp)
-
+    # remove points that are nan
+    mask = np.argwhere(~np.isnan(y_interp))
+    x_interp = x_interp[mask]
+    y_interp = y_interp[mask]
     asign = np.sign(y_interp - level)
     sign_change   = (np.roll(asign, 1) - asign) != 0
+    # first point can not have a sign change
+    sign_change[0][0] = False
     intersections = x_interp[sign_change]
     sign_slope    = asign[sign_change]
     # no intersections
     if len(intersections) == 0:
         return []
     if len(intersections) == 1:
         if sign_slope[0] == -1:
@@ -29,15 +37,15 @@
         return intersections.reshape((n_pairs, 2))
     
 def get_regular_meshgrid(*xi, n):
     reg_xi = [np.linspace(np.min(x), np.max(x), n) for x in xi]
     return np.meshgrid(*reg_xi)
     
 def get_x_intersections(x1, y1, x2, y2):
-    """Get intersections of two curves
+    """Get x intersections of two curves
     """
     interp_y1 = np.interp(x2, x1, y1) 
 
     diff = interp_y1 - y2 
     # determines what index intersection points are at 
     idx = np.argwhere(np.diff(np.sign(diff))).flatten()
```

### Comparing `quickstats-0.6.8.6/quickstats/maths/numerics.py` & `quickstats-0.6.8.8/quickstats/maths/numerics.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.6/quickstats/maths/statistics.py` & `quickstats-0.6.8.8/quickstats/maths/statistics.py`

 * *Files 3% similar despite different names*

```diff
@@ -192,14 +192,17 @@
     bin_widths = np.round(np.diff(bin_center), 8)
     if len(np.unique(bin_widths)) != 1:
         raise ValueError("can not deduce bin edges from bin centers of irregular bin widths")
     bin_width = bin_widths[0]
     bin_edges = np.concatenate([bin_center - bin_width / 2, [bin_center[-1] + bin_width/2]])
     return bin_edges
 
+def bin_edge_to_bin_width(bin_edge:np.ndarray):
+    return np.diff(bin_edge)
+
 def min_max_to_range(min_val:Optional[float]=None, max_val:Optional[float]=None):
     if (min_val is None) and (max_val is None):
         return None
     if (min_val is not None) and (max_val is not None):
         return (min_val, max_val)
     raise ValueError("min and max values must be all None or all float")
     
@@ -214,14 +217,15 @@
     return np.clip(x, xmin, xmax)
 
 def histogram(x:np.ndarray, weights:Optional[np.ndarray]=None,
               bins:Union[int, Sequence]=10,
               bin_range:Optional[Sequence]=None,
               underflow:bool=False,
               overflow:bool=False,
+              divide_bin_width:bool=False,
               normalize:bool=True,
               clip_weight:bool=False,
               evaluate_error:bool=False,
               error_option:Union[BinErrorOption, str]="auto"):
     """
         Compute the histogram of a data array.
         
@@ -240,14 +244,16 @@
        bin_range: (optional) sequence of the form (float, float)
            The lower and upper range of the bins.  If not provided, range is simply 
            ``(x.min(), x.max())``.  Values outside the range are ignored.
        underflow: bool, default = False
            Include undeflow data in the first bin.
        overflow: bool, default = False
            Include overflow data in the last bin.
+       divide_bin_width: bool, default = False
+           Divide each bin by the bin width.           
        normalize: bool, default = True
            Normalize the sum of weights to one. Weights outside the bin range will
            not be counted if ``clip_weight`` is set to false, so the sum of bin
            content could be less than one.
        clip_weight: bool, default = False
            Ignore data outside given range when evaluating total weight
            used in normalization.
@@ -285,14 +291,18 @@
         else:
             norm_factor = weights.sum()
     else:
         norm_factor = 1
         
     bin_content, bin_edges = np.histogram(x, bins=bins, range=bin_range, weights=weights)
     
+    if divide_bin_width:
+        bin_width = bin_edge_to_bin_width(bin_edges)
+        bin_content /= bin_width
+    
     if evaluate_error:
         error_option = BinErrorOption.parse(error_option)
         if error_option == BinErrorOption.AUTO:
             unit_weight = np.allclose(weights, np.ones(weights.shape))
             error_option = BinErrorOption.POISSON if unit_weight else BinErrorOption.SUMW2
         if error_option == BinErrorOption.POISSON:
             pois_interval = get_poisson_interval(bin_content)
@@ -314,14 +324,15 @@
     return bin_content, bin_edges, bin_errors
         
 def get_hist_data(x:np.ndarray, weights:Optional[np.ndarray]=None,
                   bins:Union[int, Sequence]=10,
                   bin_range:Optional[Sequence]=None,
                   underflow:bool=False,
                   overflow:bool=False,
+                  divide_bin_width:bool=False,
                   normalize:bool=True,
                   clip_weight:bool=False,
                   xerr:bool=True,
                   yerr:bool=True,
                   error_option:Union[BinErrorOption, str]="auto"):
     """
         Extract histogram data from a data array.
@@ -334,51 +345,54 @@
             Array of weights with same shape as input data. If not given, the
             input data is assumed to have unit weights.
         bins: (optional) int or sequence of scalars, default = 10
             If integer, it defines the number of equal-width bins in the
             given range.
             If sequence, it defines a monotonically increasing array of bin edges,
             including the rightmost edge.
-       bin_range: (optional) sequence of the form (float, float)
-           The lower and upper range of the bins.  If not provided, range is simply 
-           ``(x.min(), x.max())``.  Values outside the range are ignored.
-       underflow: bool, default = False
-           Include undeflow data in the first bin.
-       overflow: bool, default = False
-           Include overflow data in the last bin.
-       normalize: bool, default = True
-           Normalize the sum of weights to one. Weights outside the bin range will
-           not be counted if ``clip_weight`` is set to false, so the sum of bin
-           content could be less than one.
-       clip_weight: bool, default = True
-           If True, ignore data outside given range when evaluating total weight
-           used in normalization.
-       xerr: bool, default = True
-           If True, evaluate the error of the bin centers (= bin widths / 2).
-       yerr: bool, default = True
-           If True, evaluate the error of the bin contents using the given error
-           option.
-       error_option: BinErrorOption or str, default = "auto"
-           How to evaluate bin errors. If "sumw2", symmetric errors from the Wald
-           approximation is used (square root of sum of squares of weights). If
-           "poisson", asymmetric errors from Poisson interval at one sigma is
-           used. If "auto", it will use sumw2 error if data has unit weights,
-           else Poisson error will be used.
-           
-       Returns
-       -------------------------------------------------------------------------------
-       hist_data: dict
-           A dictionary with the keys "x", "y", "xerr", "yerr" with the bin centers,
-           bin content, half bin widths and bin errors as values.
+        bin_range: (optional) sequence of the form (float, float)
+            The lower and upper range of the bins.  If not provided, range is simply 
+            ``(x.min(), x.max())``.  Values outside the range are ignored.
+        underflow: bool, default = False
+            Include undeflow data in the first bin.
+        overflow: bool, default = False
+            Include overflow data in the last bin.
+        divide_bin_width: bool, default = False
+            Divide each bin by the bin width.
+        normalize: bool, default = True
+            Normalize the sum of weights to one. Weights outside the bin range will
+            not be counted if ``clip_weight`` is set to false, so the sum of bin
+            content could be less than one.
+        clip_weight: bool, default = True
+            If True, ignore data outside given range when evaluating total weight
+            used in normalization.
+        xerr: bool, default = True
+            If True, evaluate the error of the bin centers (= bin widths / 2).
+        yerr: bool, default = True
+            If True, evaluate the error of the bin contents using the given error
+            option.
+        error_option: BinErrorOption or str, default = "auto"
+            How to evaluate bin errors. If "sumw2", symmetric errors from the Wald
+            approximation is used (square root of sum of squares of weights). If
+            "poisson", asymmetric errors from Poisson interval at one sigma is
+            used. If "auto", it will use sumw2 error if data has unit weights,
+            else Poisson error will be used.
+            
+        Returns
+        -------------------------------------------------------------------------------
+        hist_data: dict
+            A dictionary with the keys "x", "y", "xerr", "yerr" with the bin centers,
+            bin content, half bin widths and bin errors as values.
     """
     y, bin_edges, yerr = histogram(x, weights=weights,
                                    bins=bins, bin_range=bin_range,
                                    underflow=underflow,
                                    overflow=overflow,
                                    normalize=normalize,
+                                   divide_bin_width=divide_bin_width,
                                    clip_weight=clip_weight,
                                    evaluate_error=yerr,
                                    error_option=error_option)
     x = bin_edge_to_bin_center(bin_edges)
     if xerr:
         # todo do not hard-code number of digits to keep
         xerr = np.round(np.diff(bin_edges) / 2, 5)
@@ -394,33 +408,72 @@
 
 def get_stacked_hist_data(x:List[np.ndarray],
                           weights:List[Optional[np.ndarray]]=None,
                           bins:Union[int, Sequence]=10,
                           bin_range:Optional[Sequence]=None,
                           underflow:bool=False,
                           overflow:bool=False,
+                          divide_bin_width:bool=False,
                           normalize:bool=True,
                           clip_weight:bool=False,
                           xerr:bool=True,
                           yerr:bool=True,
+                          merge:bool=True,
                           error_option:Union[BinErrorOption, str]="auto"):
-    x = np.concatenate(x)
-    if weights is not None:
-        weights = np.concatenate(weights)
-        assert x.shape == weights.shape
+    merged_x = np.concatenate(x)
     if bin_range is None:
-        bin_range = (np.min(x), np.max(x))
-    return get_hist_data(x=x, weights=weights,
-                         bins=bins, bin_range=bin_range,
-                         underflow=underflow,
-                         overflow=overflow,
-                         normalize=normalize,
-                         clip_weight=clip_weight,
-                         xerr=xerr, yerr=yerr,
-                         error_option=error_option)
+        bin_range = (np.min(merged_x), np.max(merged_x))
+    if merge:
+        if weights is not None:
+            merged_weights = np.concatenate(weights)
+            assert merged_x.shape == merged_weights.shape
+        else:
+            merged_weights = None
+        hist_data = get_hist_data(x=merged_x, weights=merged_weights,
+                                  bins=bins, bin_range=bin_range,
+                                  underflow=underflow,
+                                  overflow=overflow,
+                                  divide_bin_width=divide_bin_width,
+                                  normalize=normalize,
+                                  clip_weight=clip_weight,
+                                  xerr=xerr, yerr=yerr,
+                                  error_option=error_option)
+        return hist_data
+    else:
+        stacked_hist_data = {
+            "x": [],
+            "y": [],
+            "xerr": [],
+            "yerr": []
+        }
+        if weights is None:
+            weights = len(x) * None
+        for x_i, weights_i in zip(x, weights):
+            hist_data = get_hist_data(x=x_i, weights=weights_i,
+                                      bins=bins, bin_range=bin_range,
+                                      underflow=underflow,
+                                      overflow=overflow,
+                                      divide_bin_width=False,
+                                      normalize=False,
+                                      clip_weight=clip_weight,
+                                      xerr=xerr, yerr=yerr,
+                                      error_option=error_option)
+            stacked_hist_data['x'].append(hist_data['x'])
+            stacked_hist_data['y'].append(hist_data['y'])
+            stacked_hist_data['xerr'].append(hist_data['xerr'])
+            stacked_hist_data['yerr'].append(hist_data['yerr'])
+        if normalize:
+            norm_factor = np.sum(stacked_hist_data['y'])
+            stacked_hist_data['y'] = [y / norm_factor for y in stacked_hist_data['y']]
+        if divide_bin_width:
+            bin_edges = np.histogram_bin_edges([bin_range[0], bin_range[1]],
+                                               bins=bins, range=bin_range)
+            bin_widths = bin_edge_to_bin_width(bin_edges)
+            stacked_hist_data['y'] = [y / bin_widths for y in stacked_hist_data['y']]
+        return stacked_hist_data
 
 def get_sumw2(weights:np.ndarray):
     return np.sqrt(np.sum(weights ** 2))
 
 def get_hist_mean(x:np.ndarray, y:np.ndarray):
     return np.sum(x * y) / np.sum(y)
 
@@ -510,15 +563,14 @@
     from quickstats.interface.root import TH1
     pyh = TH1.from_numpy_histogram(y, bin_edges=bin_edges)
     pyh.rebin(nbins)
     x = pyh.bin_center
     y = pyh.bin_content
     return x, y
 
-
 def get_hist_comparison_data(reference_data, target_data,
                              mode:Union[HistComparisonMode, str]="ratio"):
     mode = HistComparisonMode.parse(mode)
     if not np.allclose(target_data['x'], reference_data['x']):
         raise RuntimeError("cannot compare two distributions with different binnings")
     comparison_data = {}
     comparison_data['x'] = reference_data['x']
```

### Comparing `quickstats-0.6.8.6/quickstats/maths/statistics_jitted.py` & `quickstats-0.6.8.8/quickstats/maths/statistics_jitted.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.6/quickstats/maths/symbolics.py` & `quickstats-0.6.8.8/quickstats/maths/symbolics.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.6/quickstats/parsers/param_parser.py` & `quickstats-0.6.8.8/quickstats/parsers/param_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,29 +47,29 @@
         obj._value_ = value
         obj.description = description
         obj.match_func = match_func
         return obj
 
 class ParamParser:
     
-    DEFAULT_FORMAT_STR = r"[\w-]+"
+    DEFAULT_FORMAT_STR = r"[\.\w-]+"
     
     DEFAULT_FILE_EXT = ".root"
     
     @property
     def format_str(self):
         return self._format_str
     
     @format_str.setter
     def format_str(self, val):
         if val is None:
             self._format_str = self.DEFAULT_FORMAT_STR
         else:
             self._format_str = val
-        self.fname_regex   = self.get_fname_regex(self._format_str, self.file_ext)
+        self.filename_regex   = self.get_filename_regex(self._format_str, self.file_ext)
         self.attribute_parser = self.get_attribute_parser(self._format_str)
         
     @property
     def file_ext(self):
         return self._file_ext
     
     @file_ext.setter
@@ -112,15 +112,15 @@
         signature_map = {}
         for group in attribute_groups:
             attribute, signature = group[0], group[1]
             signature_map[attribute] = signature
         return signature_map
     
     @staticmethod
-    def get_fname_regex(format_str:str, ext:Optional[str]=None):
+    def get_filename_regex(format_str:str, ext:Optional[str]=None):
         if ext is None:
             ext = ParamParser.DEFAULT_FILE_EXT    
         expr = format_str
         signature_map = ParamParser.get_signature_map(format_str)
         for attribute, signature in signature_map.items():
             attribute_expr = signature_regex.get(signature.upper(), None)
             if expr is None:
@@ -250,24 +250,24 @@
             encoded_str_list.append(encoded_str)
         return "_".join(sorted(encoded_str_list))
 
     def get_external_param_points(self, dirname:str="",
                                   filter_expr:Optional[str]=None,
                                   exclude_expr:Optional[str]=None):
         if os.path.isdir(dirname):
-            fnames = glob.glob(os.path.join(dirname, '*'))
+            filenames = glob.glob(os.path.join(dirname, '*'))
         else:
-            fnames = glob.glob(dirname)
+            filenames = glob.glob(dirname)
         param_points = []
-        for fname in fnames:
-            basename = os.path.basename(fname)
-            match = self.fname_regex.match(basename)
+        for filename in filenames:
+            basename = os.path.basename(filename)
+            match = self.filename_regex.match(basename)
             if not match:
                 continue
-            point = {'filename': fname, 'parameters':{}}
+            point = {'filename': filename, 'parameters':{}}
             point['basename'] = basename.split('.')[0]
             for key, value in match.groupdict().items():
                 parser = self.attribute_parser[key]
                 point['parameters'][key] = parser(value)
             param_points.append(point)
         attributes = list(self.attribute_parser)
         param_points = self.sort_param_points(param_points, attributes)
@@ -355,25 +355,25 @@
                 for param_name, param_value in int_point.items():
                     if param_value is None:
                         raise RuntimeError(f"profiled parameter is not allowed ({param_name})")
     
     def get_param_points(self, dirname:str="",
                          filter_expr:Optional[str]=None,
                          exclude_expr:Optional[str]=None):
-        external_param_points = self.get_external_param_points(dirname, filter_expr, exclude_expr)     
+        external_param_points = self.get_external_param_points(dirname, filter_expr, exclude_expr)
         internal_param_points = self.get_internal_param_points(filter_expr, exclude_expr)
         self.sanity_check(internal_param_points, external_param_points)
         if len(internal_param_points) == 0:
             internal_param_points = [{}]
         param_points = []
         for ext_point in external_param_points:
-            fname = ext_point['filename']
+            filename = ext_point['filename']
             basename = ext_point['basename']
             ext_params = ext_point['parameters']
             for int_params in internal_param_points:
                 param_point = {}
-                param_point['filename'] = fname
+                param_point['filename'] = filename
                 param_point['basename'] = basename
                 param_point['external_parameters'] = {**ext_params}
                 param_point['internal_parameters'] = {**int_params}
                 param_points.append(param_point)
         return param_points
```

### Comparing `quickstats-0.6.8.6/quickstats/plots/__init__.py` & `quickstats-0.6.8.8/quickstats/plots/__init__.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.6/quickstats/plots/abstract_plot.py` & `quickstats-0.6.8.8/quickstats/plots/abstract_plot.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,31 +4,37 @@
 import numpy as np
 import matplotlib
 
 from quickstats import AbstractObject, semistaticmethod
 from quickstats.plots import get_color_cycle, get_cmap
 from quickstats.plots.color_schemes import QUICKSTATS_PALETTES
 from quickstats.plots.template import (single_frame, parse_styles, format_axis_ticks,
-                                       parse_analysis_label_options)
+                                       parse_analysis_label_options, centralize_axis)
 from quickstats.utils.common_utils import combine_dict, insert_periodic_substr
 from quickstats.maths.statistics import bin_center_to_bin_edge, get_hist_comparison_data
+from quickstats.maths.statistics import HistComparisonMode
 from .core import PlotFormat, ErrorDisplayFormat
 
 class AbstractPlot(AbstractObject):
     
     STYLES = {}
     
     COLOR_CYCLE = "default"
     
     COLOR_PALLETE = {}
     COLOR_PALLETE_SEC = {}
     
     CONFIG = {
         "xlabellinebreak": 50,
-        "ylabellinebreak": 50
+        "ylabellinebreak": 50,
+        'ratio_line_styles':{
+            'color': 'gray',
+            'linestyle': '--',
+            'zorder': 0
+        },        
     }
     
     def __init__(self,
                  color_pallete:Optional[Dict]=None,
                  color_pallete_sec:Optional[Dict]=None,
                  color_cycle:Optional[Union[List, str, "ListedColorMap"]]=None,
                  styles:Optional[Union[Dict, str]]=None,
@@ -245,14 +251,41 @@
         ax.set_xlim(*xlim)
         ax.set_ylim(*ylim)
     
     @staticmethod
     def close_all_figures():
         matplotlib.pyplot.close()
         
+    def decorate_comparison_axis(self, ax, xlabel:str="", ylabel:str="", 
+                                 mode:Union[HistComparisonMode, str]="ratio",
+                                 ylim:Optional[Sequence]=None,
+                                 ypad:Optional[float]=0.1,
+                                 draw_ratio_line:bool=True):
+        mode = HistComparisonMode.parse(mode)
+        if ylim is not None:
+            ax.set_ylim(ylim)
+        do_centralize_axis = ylim is None
+        if mode == HistComparisonMode.RATIO:
+            if do_centralize_axis:
+                centralize_axis(ax, which="y", ref_value=1, padding=ypad)
+            if draw_ratio_line:
+                ax.axhline(1, **self.config['ratio_line_styles'])
+        elif mode == HistComparisonMode.DIFFERENCE:
+            if do_centralize_axis:
+                centralize_axis(ax, which="y", ref_value=0, padding=ypad)
+            if draw_ratio_line:
+                ax.axhline(0, **self.config['ratio_line_styles'])
+        # set default ylabel if not given
+        if not ylabel:
+            if mode == HistComparisonMode.RATIO:
+                ylabel = "Ratio"
+            elif mode == HistComparisonMode.DIFFERENCE:
+                ylabel = "Difference"
+        self.draw_axis_components(ax, xlabel=xlabel, ylabel=ylabel)
+        
     def draw_binned_data(self, ax, data,
                          draw_data:bool=True,
                          draw_error:bool=True,
                          bin_edges:Optional[np.ndarray]=None,
                          plot_format:Union[PlotFormat, str]='errorbar',
                          error_format:Union[ErrorDisplayFormat, str]='errorbar',
                          styles:Optional[Dict]=None,
```

### Comparing `quickstats-0.6.8.6/quickstats/plots/bidirectional_bar_chart.py` & `quickstats-0.6.8.8/quickstats/plots/bidirectional_bar_chart.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.6/quickstats/plots/collective_data_plot.py` & `quickstats-0.6.8.8/quickstats/plots/collective_data_plot.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.6/quickstats/plots/color_schemes.py` & `quickstats-0.6.8.8/quickstats/plots/color_schemes.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.6/quickstats/plots/core.py` & `quickstats-0.6.8.8/quickstats/plots/core.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.6/quickstats/plots/correlation_plot.py` & `quickstats-0.6.8.8/quickstats/plots/correlation_plot.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.6/quickstats/plots/general_1D_plot.py` & `quickstats-0.6.8.8/quickstats/plots/general_1D_plot.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,14 +66,15 @@
             stat_handles = None
         return handle[0], stat_handles
     
     def draw(self, xattrib:str, yattrib:str, targets:Optional[List[str]]=None,
              xlabel:Optional[str]=None, ylabel:Optional[str]=None,
              ymin:Optional[float]=None, ymax:Optional[float]=None,
              xmin:Optional[float]=None, xmax:Optional[float]=None,
+             ypad:Optional[float]=0.3,
              logx:bool=False, logy:bool=False,
              draw_stats:bool=True):
         
         ax = self.draw_frame(logx=logx, logy=logy)
         
         legend_order = []
         if isinstance(self.data_map, pd.DataFrame):
@@ -127,10 +128,10 @@
             raise ValueError("invalid data format")
             
         self.legend_order = legend_order
         handles, labels = self.get_legend_handles_labels()
         ax.legend(handles, labels, **self.styles['legend'])
         
         self.draw_axis_components(ax, xlabel=xlabel, ylabel=ylabel)
-        self.set_axis_range(ax, xmin=xmin, xmax=xmax, ymin=ymin, ymax=ymax)
+        self.set_axis_range(ax, xmin=xmin, xmax=xmax, ymin=ymin, ymax=ymax, ypad=ypad)
         
         return ax
```

### Comparing `quickstats-0.6.8.6/quickstats/plots/general_distribution_plot.py` & `quickstats-0.6.8.8/quickstats/plots/general_distribution_plot.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.6/quickstats/plots/histo_1D_plot.py` & `quickstats-0.6.8.8/quickstats/plots/histo_1D_plot.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.6/quickstats/plots/hypotest_inverter_plot.py` & `quickstats-0.6.8.8/quickstats/plots/hypotest_inverter_plot.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.6/quickstats/plots/likelihood_1D_plot.py` & `quickstats-0.6.8.8/quickstats/plots/likelihood_1D_plot.py`

 * *Files 4% similar despite different names*

```diff
@@ -72,78 +72,93 @@
                          styles_map=styles_map,
                          color_cycle=color_cycle,
                          styles=styles,
                          analysis_label_options=analysis_label_options,
                          config=config)
         self.intervals = {}
     
-    def get_sigma_levels_values_labels(self, interval_format:str="one_two_sigma"):
-        if interval_format not in self.config['interval_formats']:
-            choices = ','.join([f'"{choice}"' for choice in self.config['interval_formats']])
-            raise ValueError(f'undefined sigma interval format: {interval_format} (choose from {choices})')
-        sigma_levels = self.config['interval_formats'][interval_format]
+    def get_sigma_levels_values_labels(self, interval_format:Union[str, List[str]]="one_two_sigma"):
+        if isinstance(interval_format, (list, tuple)):
+            sigma_levels = list(interval_format)
+        else:
+            if interval_format not in self.config['interval_formats']:
+                choices = ','.join([f'"{choice}"' for choice in self.config['interval_formats']])
+                raise ValueError(f'undefined sigma interval format: {interval_format} (choose from {choices})')
+            sigma_levels = self.config['interval_formats'][interval_format]
         sigma_values = []
         sigma_labels = []
         for sigma_level in sigma_levels:
             if sigma_level not in self.coverage_proba_data:
                 raise RuntimeError(f'undefined sigma level: {sigma_level}')
             sigma_values.append(self.coverage_proba_data[sigma_level]['qmu'])
             sigma_labels.append(self.coverage_proba_data[sigma_level]['label'])
         return sigma_levels, sigma_values, sigma_labels
     
     def get_sigma_intervals(self, x:np.ndarray, y:np.ndarray,
-                            interval_format:str="one_two_sigma"):
+                            interval_format:Union[str, List[str]]="one_two_sigma"):
         from quickstats.maths.interpolation import get_intervals
         sigma_levels, sigma_values, sigma_labels = self.get_sigma_levels_values_labels(interval_format)
         sigma_intervals = {}
         for i, (sigma_level, sigma_value, sigma_label) in enumerate(zip(sigma_levels, sigma_values, sigma_labels)):
             intervals = get_intervals(x, y, sigma_value)
             sigma_intervals[sigma_level] = intervals
         return sigma_intervals
+    
+    def get_bestfit(self, x:np.ndarray, y:np.ndarray):
+        bestfit_idx = np.argmin(y)
+        bestfit_x   = x[bestfit_idx]
+        bestfit_y   = y[bestfit_idx]
+        return bestfit_x, bestfit_y
         
-    def draw_sigma_lines(self, ax, interval_format:str="one_two_sigma"):
+    def draw_sigma_lines(self, ax, interval_format:Union[str, List[str]]="one_two_sigma"):
         sigma_line_styles = self.config['sigma_line_styles']
         sigma_levels, sigma_values, sigma_labels = self.get_sigma_levels_values_labels(interval_format)
         transform = create_transform(transform_x="axis", transform_y="data")
         ax.hlines(sigma_values, xmin=0, xmax=1, zorder=0, transform=transform,
                   **self.config['sigma_line_styles'])
         styles = combine_dict(self.styles['text'], self.config['sigma_text_styles'])
         if 'va' not in styles:
             styles['va'] = 'bottom' if ((styles['x'] > 0) and (styles['x'] < 1)) else 'center'
         for sigma_value, sigma_label in zip(sigma_values, sigma_labels):
             ax.text(y=sigma_value, s=sigma_label, **styles, transform=transform)
     
     def draw_sigma_intervals(self, ax, x:np.ndarray, y:np.ndarray, xlabel:str="",
-                             interval_format:str="one_two_sigma"):
+                             interval_format:Union[str, List[str]]="one_two_sigma"):
         from quickstats.maths.interpolation import get_intervals
         sigma_levels, sigma_values, sigma_labels = self.get_sigma_levels_values_labels(interval_format)
         sigma_intervals = self.get_sigma_intervals(x, y, interval_format=interval_format)
         self.intervals  = sigma_intervals
         styles     = self.config['sigma_interval_styles']
         loc        = styles['loc']
         dp         = styles['decimal_place']
         dy         = styles['dy']
         sigma_text = styles['sigma_text']
+        # do not draw when no intervals available
+        if all(len(intervals) == 0 for intervals in sigma_intervals.values()):
+            return None
         ax.annotate(styles['main_text'], loc, xycoords='axes fraction', **self.styles['annotation'])
         for i, (sigma_level, sigma_label) in enumerate(zip(sigma_levels, sigma_labels)):
             sigma_interval = sigma_intervals[sigma_level]
+            if len(sigma_interval) == 0:
+                continue
             interval_str = r" \cup ".join([f"[{lo:.{dp}f}, {hi:.{dp}f}]" for (lo, hi) in sigma_interval])
+            interval_str = interval_str.replace('-inf', r'N.A.').replace('inf', 'N.A.')
             text = sigma_text.format(sigma_label=sigma_label,
                                      xlabel=xlabel,
                                      intervals=interval_str)
             ax.annotate(text, (loc[0], loc[1] - (i + 1) * dy),
                         xycoords='axes fraction', **self.styles['annotation'])
 
     def draw(self, xattrib:str='mu', yattrib:str='qmu', xlabel:Optional[str]=None, 
              ylabel:Optional[str]="$-2\Delta ln(L)$",
              ymin:float=0, ymax:float=7, xmin:Optional[float]=None, xmax:Optional[float]=None,
              draw_sigma_line:bool=True,
              #draw_sm_line:bool=False,
              draw_sigma_intervals:Union[str, bool]=False,
-             interval_format:str="one_two_sigma"):
+             interval_format:Union[str, List[str]]="one_two_sigma"):
                         
         ax = super().draw(xattrib=xattrib, yattrib=yattrib,
                           xlabel=xlabel, ylabel=ylabel,
                           ymin=ymin, ymax=ymax, xmin=xmin, xmax=xmax)
 
         if draw_sigma_line:
             self.draw_sigma_lines(ax, interval_format=interval_format)
@@ -161,20 +176,20 @@
                 for sm_value, sm_name in zip(sm_values, sm_names):
                     ax.text(sm_value, sm_pos, sm_name, color='gray', ha='right', rotation=90,
                             va='bottom' if (sm_pos > 0 and sm_pos < 1) else 'center', fontsize=20, transform=transform)
         """
         
         if draw_sigma_intervals:
             if isinstance(self.data_map, pd.DataFrame):
-                x = self.data_map[xattrib]
-                y = self.data_map[yattrib]
+                x = self.data_map[xattrib].values
+                y = self.data_map[yattrib].values
             elif isinstance(self.data_map, dict):
                 if not isinstance(draw_sigma_intervals, str):
                     raise RuntimeError("name of the target likelihood curve must be specified "
                                        "when drawing sigma intervals")
                 target = draw_sigma_intervals
-                x = self.data_map[target][xattrib]
-                y = self.data_map[target][yattrib]
+                x = self.data_map[target][xattrib].values
+                y = self.data_map[target][yattrib].values
             else:
                 raise ValueError("invalid data format")
             self.draw_sigma_intervals(ax, x, y, xlabel=xlabel, interval_format=interval_format)
         return ax
```

### Comparing `quickstats-0.6.8.6/quickstats/plots/likelihood_2D_plot.py` & `quickstats-0.6.8.8/quickstats/plots/upper_limit_3D_plot.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,292 +1,297 @@
-from typing import Dict, Optional, Union, List, Sequence
-
-from itertools import repeat
+from typing import Optional, Union, Dict, List
 
 import numpy as np
-import pandas as pd
+import matplotlib.patches as patches
 
 from quickstats.plots import AbstractPlot
 from quickstats.plots.template import create_transform
 from quickstats.utils.common_utils import combine_dict
-from quickstats.maths.interpolation import get_regular_meshgrid
-from matplotlib.lines import Line2D
-
-
-class Likelihood2DPlot(AbstractPlot):
 
-    CONFIG = {
-        # intervals to include in the plot
-        "interval_formats": {
-            "68_95"               : ('0.68', '0.95'),
-            "one_two_sigma"       : ('1sigma', '2sigma'),
-            "68_95_99"            : ('0.68', '0.95', '0.99'),
-            "one_two_three_sigma" : ('1sigma', '2sigma', '3sigma')
-        },
-        'highlight_styles': {
-            'linewidth': 0,
-            'marker': '*',
-            'markersize': 20,
-            'color': '#E9F1DF',
-            'markeredgecolor': 'black'
-        },
-        'bestfit_styles':{
-            'marker': 'P',
-            'linewidth': 0,
-            'markersize': 15
-        },
-        'contour_styles': {
-            'linestyles': 'solid',
-            'linewidths': 3
+class UpperLimit3DPlot(AbstractPlot):
+    
+    STYLES = {
+        'axis':{
+            'tick_bothsides': True
         },
-        'bestfit_label': "Best fit ({x:.2f}, {y:.2f})",
-        'cmap': 'GnBu',
-        'interpolation': 'cubic',
-        'num_grid_points': 500,
+        'errorbar': {
+            "linewidth": 1,
+            "markersize": 5,
+            "marker": 'o',
+        }        
     }
     
-    # qmu from https://pdg.lbl.gov/2018/reviews/rpp2018-rev-statistics.pdf#page=31
-    coverage_proba_data = {
-        '0.68': {
-            'qmu': 2.30,
-            'label': '68% CL',
-            'color': "hh:darkblue"
-        },
-        '1sigma': {  
-            'qmu': 2.30, # 68.2%
-            'label': '1 $\sigma$',
-            'color': "hh:darkblue"
-        },
-        '0.90': {
-            'qmu': 4.61,
-            'label': '90% CL',
-            'color': "#36b1bf"
-        },
-        '0.95': {
-            'qmu': 5.99,
-            'label': '95% CL',
-            'color': "#F2385A"
-        },
-        '2sigma': {
-            'qmu': 6.18, # 95.45%
-            'label': '2 $\sigma$',
-            'color': "#F2385A"
+    COLOR_PALLETE = {
+        '2sigma': '#FDC536',
+        '1sigma': '#4AD9D9',
+        'expected': 'k',
+        'excluded': 'w',
+        'observed': 'k'
+    }
+    
+    COLOR_PALLETE_SEC = {
+        '2sigma': '#FDC536',
+        '1sigma': '#4AD9D9',
+        'expected': 'r',
+        'observed': 'r'
+    }
+    
+    LABELS = {
+        '2sigma': 'Expected limit $\pm 2\sigma$',
+        '1sigma': 'Expected limit $\pm 1\sigma$',
+        'expected': 'Expected limit (95% CL)',
+        'observed': 'Observed limit (95% CL)'
+    }
+    
+    LABELS_SEC = {
+        '2sigma': 'Expected limit $\pm 2\sigma$',
+        '1sigma': 'Expected limit $\pm 1\sigma$',
+        'expected': 'Expected limit (95% CL)',
+        'observed': 'Observed limit (95% CL)'
+    }
+
+    CONFIG = {
+        'primary_hatch'  : '\\\\\\',
+        'secondary_hatch': '///',
+        'primary_alpha'  : 0.9,
+        'secondary_alpha': 0.8,
+        'curve_line_styles': {
+            'color': 'darkred' 
         },
-        '0.99': {
-            'qmu': 9.21,
-            'label': '99% CL',
-            'color': "#FDC536"
+        'curve_fill_styles':{
+            'color': 'hh:darkpink'
         },
-        '3sigma': {
-            'qmu': 11.83, # 99.73%
-            'label': '3 $\sigma$',
-            'color': "#FDC536"
+        'highlight_styles': {
+            'linewidth' : 0,
+            'marker' : '*',
+            'markersize' : 20,
+            'color' : '#E9F1DF',
+            'markeredgecolor' : 'black'
         }
     }
-
-    def __init__(self, data_map: Union[pd.DataFrame, Dict[str, pd.DataFrame]],
-                 label_map: Optional[Dict] = None,
-                 styles_map: Optional[Dict] = None,
-                 config_map: Optional[Dict] = None,
-                 color_cycle=None,
-                 styles: Optional[Union[Dict, str]] = None,
-                 analysis_label_options: Optional[Dict] = None,
-                 config: Optional[Dict] = None):
-
-        self.data_map = data_map
-        self.label_map = label_map
-        self.styles_map = styles_map
-        self.config_map = config_map
-        self.highlight_data = []
-        self.contours = None
-
-        super().__init__(color_cycle=color_cycle,
+    
+    def __init__(self, data, data_sec=None,
+                 num_grid_points=None,
+                 color_pallete:Optional[Dict]=None,
+                 color_pallete_sec:Optional[Dict]=None,
+                 labels:Optional[Dict]=None,
+                 labels_sec:Optional[Dict]=None,
+                 styles:Optional[Union[Dict, str]]=None,
+                 analysis_label_options:Optional[Union[Dict, str]]='default',
+                 config:Optional[Dict]=None):
+        super().__init__(color_pallete=color_pallete,
+                         color_pallete_sec=color_pallete_sec,
                          styles=styles,
                          analysis_label_options=analysis_label_options,
                          config=config)
+        self.data     = data
+        # secondary data
+        self.data_sec = data_sec
         
-    def get_sigma_levels(self, interval_format:str="one_two_three_sigma"):
-        if interval_format not in self.config['interval_formats']:
-            choices = ','.join([f'"{choice}"' for choice in self.config['interval_formats']])
-            raise ValueError(f'undefined sigma interval format: {interval_format} (choose from {choices})')
-        sigma_levels = self.config['interval_formats'][interval_format]
-        return sigma_levels
-
-    def draw_single_data(self, ax, data: pd.DataFrame,
-                         xattrib: str, yattrib: str,
-                         zattrib: str = 'qmu',
-                         styles: Optional[Dict] = None,
-                         clabel_size=None, show_colormesh=False,
-                         interval_format:str="one_two_three_sigma"):
-        config = combine_dict(self.config)
-        sigma_levels = self.get_sigma_levels(interval_format=interval_format)
-        sigma_values = [self.coverage_proba_data[level]['qmu'] for level in sigma_levels]
-        sigma_labels = [self.coverage_proba_data[level]['label'] for level in sigma_levels]
-        sigma_colors = [self.coverage_proba_data[level]['color'] for level in sigma_levels]
-
-        interpolate_method = config.get('interpolation', None)
-        if interpolate_method is not None:
-            from scipy import interpolate
-            x, y, z = data[xattrib], data[yattrib], data[zattrib]
-            n = config.get('num_grid_points', 500)
-            X, Y = get_regular_meshgrid(x, y, n=n)
-            Z = interpolate.griddata(np.stack((x, y), axis=1), z, (X, Y), interpolate_method)
-        else:
-            X_unique = np.sort(data[xattrib].unique())
-            Y_unique = np.sort(data[yattrib].unique())
-            X, Y = np.meshgrid(X_unique, Y_unique)
-            Z = (data.pivot_table(index=xattrib, columns=yattrib, values=zattrib).T.values
-                 - data[zattrib].min())
-            
-        if show_colormesh:
-            cmap = config['cmap']
-            im = ax.pcolormesh(X, Y, Z, cmap=cmap, shading='auto')
-            import matplotlib.pyplot as plt
-            self.cbar = plt.colorbar(im, ax=ax, **config['colorbar'])
-            self.cbar.set_label(**config['colorbar_label'])
-            
-        if sigma_values:
-            cp = ax.contour(X, Y, Z, levels=sigma_values, colors=sigma_colors,
-                            **config['contour_styles'])
-            if clabel_size is not None:
-                ax.clabel(cp, inline=True, fontsize=clabel_size)
-                
-        line_styles = self._get_line_styles(config['contour_styles'])
-        custom_handles = [Line2D([0], [0], color=color, label=label, **styles) \
-                          for color, label, styles in zip(sigma_colors, sigma_labels, line_styles)]
-        self.update_legend_handles(dict(zip(sigma_labels, custom_handles)))
-        self.legend_order.extend(sigma_labels)
-        return custom_handles
+        self.labels = combine_dict(self.LABELS, labels)
+        self.labels_sec = combine_dict(self.LABELS_SEC, labels_sec)
+        
+        self.num_grid_points = num_grid_points
+        self.highlight_data = None
+        
+    def get_default_legend_order(self):
+        return ['observed', 'expected', '1sigma', '2sigma', 'curve', 'highlight']
     
-    def _get_line_styles(self, styles:Dict):
-        style_key_map = {
-            'linestyles': 'linestyle',
-            'linewidths': 'linewidth'
+    def add_highlight(self, x:float, y:float, label:str="SM prediction",
+                      styles:Optional[Dict]=None):
+        highlight_data = {
+            'x'     : x,
+            'y'     : y,
+            'label' : label,
+            'styles': styles
         }
-        new_styles = {new_name: styles[old_name] for old_name, new_name \
-                      in style_key_map.items() if old_name in styles}
-        sizes = []
-        for style in new_styles.values():
-            if (isinstance(style, Sequence)) and (not isinstance(style, str)):
-                sizes.append(len(style))
-            else:
-                sizes.append(1)
-        if not sizes:
-            return repeat({})
-        if not len(np.unique(sizes)) == 1:
-            raise ValueError('contour line styles have inconsistent sizes')
-        size = np.unique(sizes)[0]
-        if size == 1:
-            return repeat(new_styles)
-        list_styles = []
-        for i in range(size):
-            styles_i = {key: value[i] for key, value in new_styles.items()}
-            list_styles.append(styles_i)
-        return list_styles
-
-    def draw(self, xattrib:str, yattrib:str, zattrib:str='qmu', xlabel: Optional[str] = "",
-             ylabel: Optional[str] = "", zlabel: Optional[str] = "$-2\Delta ln(L)$",
-             ymax:Optional[float]=None, ymin:Optional[float]=None,
-             xmin:Optional[float]=None, xmax:Optional[float]=None,
-             clabel_size=None, draw_sm_line: bool = False, draw_bestfit:bool=True,
-             show_colormesh=False, show_legend=True,
-             interval_format:str="one_two_three_sigma"):
-        self.reset_legend_data()
-        ax = self.draw_frame()
-        self.contours = {'keys': [], 'contours': [], 'levels': []}
-        if isinstance(self.data_map, pd.DataFrame):
-            self.draw_single_data(ax, self.data_map, xattrib=xattrib, yattrib=yattrib,
-                                  zattrib=zattrib, styles=self.styles_map,
-                                  clabel_size=clabel_size, show_colormesh=show_colormesh,
-                                  interval_format=interval_format)
-        else:
-            raise ValueError("invalid data format")
-            
-        """
-        elif isinstance(self.data_map, dict):
-            if self.styles_map is None:
-                styles_map = {k: None for k in self.data_map}
-            else:
-                styles_map = self.styles_map
-            if self.label_map is None:
-                label_map = {k: k for k in self.data_map}
-            else:
-                label_map = self.label_map
-            if self.config_map is None:
-                config_map = {k: k for k in self.data_map}
+        self.highlight_data = highlight_data        
+    
+    def draw_highlight(self, ax, data):
+        styles = data['styles']
+        if styles is None:
+            styles = self.config['highlight_styles']
+        handle = ax.plot(data['x'], data['y'], label=data['label'], **styles)
+        self.update_legend_handles({'highlight': handle[0]})
+
+    @staticmethod
+    def get_grid(X_range, Y_range, num_grid_points):
+        X_points = np.linspace(*X_range, num_grid_points)
+        Y_points = np.linspace(*Y_range, num_grid_points)
+        X_grid, Y_grid = np.meshgrid(X_points, Y_points)
+        return X_grid, Y_grid
+
+    def return_points(self, paths):
+        ''' Get x-y coordinates of contour/path in order to fill color for bands '''
+        uout, inn = 0, 1
+        segment1_start = paths[0].vertices[0]
+        segment1_end = paths[0].vertices[-1]
+        try:
+            if len(paths) == 2 and (segment1_start != segment1_end).all():
+                segment2_start = paths[1].vertices[0]
+                segment2_end = paths[1].vertices[-1]
+                if np.square(segment2_start-segment2_end) > np.square(segment1_start-segment1_end):
+                    out, inn = 1, 0
+                return (paths[out].vertices, paths[inn].vertices)
             else:
-                config_map = self.config_map
-                
-            for key in self.data_map:
-                self.contours['keys'].append(key)
-                data = self.data_map[key]
-                styles = styles_map.get(key, None)
-                label = label_map.get(key, "")
-                config = config_map.get(key, None)
-                config = combine_dict(self.CONFIG, config)
-                handle = self.draw_single_data(ax, data,
-                                               xattrib=xattrib,
-                                               yattrib=yattrib,
-                                               zattrib=zattrib,
-                                               styles=styles,
-                                               config=config,
-                                               show_colormesh=show_colormesh)
-                         
-        """
+                return (np.concatenate([i.vertices for i in paths]),)
+        except:
+            return (np.concatenate([i.vertices for i in paths]),)
+
+    def plot_bands(self, ax, cp, labels, cp_obs=None):
+        # loop over contour curves
+        # assumption: 0,4 = 2sigma outer/inner boundaries; 1,3 = 1sigma outer/inner boundaries; 2 = expectation
+        inner2 = self.return_points(cp.collections[0].get_paths())
+        inner1 = self.return_points(cp.collections[1].get_paths())
+        center = self.return_points(cp.collections[2].get_paths())
+        outer1 = self.return_points(cp.collections[3].get_paths())
+        outer2 = self.return_points(cp.collections[4].get_paths())
+        if cp_obs:
+            observ = self.return_points(cp_obs.collections[0].get_paths())
+
+        # fill color from outside to inside
+        handle_2sigma = ax.fill(outer2[0][:,0], outer2[0][:,1], self.color_pallete['2sigma'], label=labels['2sigma'], zorder=1)
+        handle_1sigma = ax.fill(outer1[0][:,0], outer1[0][:,1], self.color_pallete['1sigma'], label=labels['1sigma'], zorder=1)
+        handle_expected = ax.plot(center[0][:,0], center[0][:,1], self.color_pallete['expected'], ls='--', label=labels['expected'], zorder=2)
+        ax.fill(inner1[0][:,0], inner1[0][:,1], self.color_pallete['2sigma'], zorder=1)
+        ax.fill(inner2[0][:,0], inner2[0][:,1], self.color_pallete['excluded'], zorder=1)
+        if len(outer2) > 1:
+            handle_2sigma = ax.fill(outer2[1][:,0], outer2[1][:,1], self.color_pallete['excluded'], zorder=1)
+        if len(outer1) + len(center) + len(inner1) + len(inner2) > 4 :
+            print('WARN', len(outer1) , len(center) , len(inner1) , len(inner2))
+
+        if cp_obs:
+            handle_observed = ax.plot(observ[0][:,0], observ[0][:,1], self.color_pallete['observed'], ls='-', label=labels['observed'], zorder=2)
+
+        self.update_legend_handles({'2sigma': handle_2sigma[0], '1sigma': handle_1sigma[0], 'expected': handle_expected[0]})
+        if cp_obs:
+            self.update_legend_handles({'observed': handle_observed[0]})
+
+    def draw_single_data(self, ax, df, x='klambda', y='k2v', scale_factor=None,
+                         theory_grid=None,
+                         color_pallete:Optional[Dict]=None,
+                         labels:Optional[Dict]=None,
+                         draw_observed:bool=False,
+                         observed_marker:Optional[str]='o', 
+                         alpha:float=1.,
+                         sec:bool=False):
         
-        highlight_index = 0
+        assert(theory_grid.shape == (self.num_grid_points, self.num_grid_points)), '`theory_grid` in draw() fails to have shape of (`self.num_grid_points`, `self.num_grid_points`)'
+        assert(not df.isnull().values.any()), 'input dataframe contains NAN'
+        if color_pallete is None:
+            color_pallete = self.color_pallete
+        if labels is None:
+            labels = self.labels
+        if scale_factor is None:
+            scale_factor = 1.0
+
+        # Create 2D grid of values for a range of two coupling constant variations (e.g. a grid of k2v and kl points) by interpolating to the grid
+        X_range = df[x].min(), df[x].max()
+        Y_range = df[y].min(), df[y].max()
+        X_grid, Y_grid = UpperLimit3DPlot.get_grid(X_range, Y_range, self.num_grid_points)
+
+        expectation_point_list = {}
+        expectation_point_list['points'] = (df[x], df[y])
+        expectation_point_list['exp'] = df['0'] * scale_factor
+        expectation_point_list['1sigma'] = df['1'] * scale_factor
+        expectation_point_list['-1sigma'] = df['-1'] * scale_factor
+        expectation_point_list['2sigma'] = df['2'] * scale_factor
+        expectation_point_list['-2sigma'] = df['-2'] * scale_factor
+        if draw_observed:
+            expectation_point_list['obs'] = df['obs'] * scale_factor
         
-        if draw_bestfit and isinstance(self.data_map, pd.DataFrame):
-            bestfit_idx = np.argmin(self.data_map[zattrib].values)
-            bestfit_x   = self.data_map.iloc[bestfit_idx][xattrib]
-            bestfit_y   = self.data_map.iloc[bestfit_idx][yattrib]
-            highlight_data = {
-                'x': bestfit_x,
-                'y': bestfit_y,
-                'label': self.config["bestfit_label"].format(x=bestfit_x, y=bestfit_y),
-                'styles': self.config["bestfit_styles"]
-            }
-            self.draw_highlight(ax, highlight_data, highlight_index)
-            highlight_index += 1
+        exp_grids = {}
+        for i in expectation_point_list.keys():
+            if i == 'points':
+                continue
+            from scipy import interpolate
+            exp_grids[i] = interpolate.griddata(expectation_point_list['points'], 
+                                                expectation_point_list[i], np.stack((X_grid, Y_grid), axis=2))
         
+        # Create a 2D grid of Z-values for contour plot, arbitarily assign values of:
+        #   0.5 within +1 sigma, 1.5 between +1 and +2 sigma, 2.5 outside of 2 sigma;
+        #   -0.5 within -1 sigma, -1.5 between -1 and -2 sigma, -2.5 outside of -2 sigma
+        Z_grid = np.zeros(theory_grid.shape)
+        Z_grid[theory_grid - exp_grids['exp'] >= 0] = 0.5
+        Z_grid[theory_grid - exp_grids['exp'] < 0] = -0.5
+        Z_grid[theory_grid - exp_grids['1sigma'] > 0] = 1.5
+        Z_grid[theory_grid - exp_grids['2sigma'] > 0] = 2.5
+        Z_grid[theory_grid - exp_grids['-1sigma'] < 0] = -1.5
+        Z_grid[theory_grid - exp_grids['-2sigma'] < 0] = -2.5
+
+        cp = ax.contour(X_grid, Y_grid, Z_grid, levels=[-2, -1, 0, 1, 2], linewidths=2, alpha=0, zorder=0)
+        #ax.contourf(X_grid, Y_grid, Z_grid, levels=[-2, -1, 0, 1, 2], linewidths=2, alpha=1, zorder=0, cmap='GnBu')
+
+        if draw_observed:
+            Z_grid_obs = np.zeros(theory_grid.shape)
+            Z_grid_obs[theory_grid - exp_grids['obs'] >= 0] = 0.5
+            Z_grid_obs[theory_grid - exp_grids['obs'] < 0] = -0.5
+
+            cp_obs = ax.contour(X_grid, Y_grid, Z_grid_obs, levels=[0], linewidths=2, alpha=0, zorder=0)
+
+        # Plot 1 and 2 sigma bands
+        self.plot_bands(ax, cp, labels, cp_obs if draw_observed else None)
+
+
+    def draw(self, x:str="", y:str="", xlabel:str="", ylabel:str="", scale_factor=None, theory_grid=None, ylim=None, xlim=None,
+             draw_observed:bool=True, observed_marker:Optional[str]='o', draw_sm_line:bool=False):
+        
+        ax = self.draw_frame()
+        
+        if self.data_sec is not None:
+            self.draw_single_data(ax, df=self.data_sec, x=x, y=y,
+                                  scale_factor=scale_factor,
+                                  theory_grid=theory_grid,
+                                  draw_observed=draw_observed,
+                                  color_pallete=self.color_pallete_sec,
+                                  labels=self.labels_sec,
+                                  observed_marker=observed_marker, 
+                                  sec=True)
+            alpha = self.config['primary_alpha']
+        else:
+            alpha = 1.
+        self.draw_single_data(ax, df=self.data, x=x, y=y,
+                              scale_factor=scale_factor,
+                              theory_grid=theory_grid,
+                              draw_observed=draw_observed,
+                              color_pallete=self.color_pallete,
+                              labels=self.labels,
+                              observed_marker=observed_marker, 
+                              alpha=alpha)
         if self.highlight_data is not None:
-            for i, h in enumerate(self.highlight_data):
-                self.draw_highlight(ax, h, highlight_index + i)
+            self.draw_highlight(ax, self.highlight_data)
+            
+        self.draw_axis_components(ax, xlabel=xlabel, ylabel=ylabel)
+        
+        if ylim is not None:
+            ax.set_ylim(*ylim)
+        if xlim is not None:
+            ax.set_xlim(*xlim)
 
         if draw_sm_line:
             sm_line_styles = self.config['sm_line_styles']
             sm_values = self.config['sm_values']
-            transform = create_transform(
-                transform_y="axis", transform_x="data")
-            ax.vlines(sm_values[0], ymin=0, ymax=1, zorder=0, transform=transform,
+            transform = create_transform(transform_y="axis", transform_x="data")
+            ax.vlines(sm_values[0], ymin=0, ymax=1, zorder=2, transform=transform,
                       **sm_line_styles)
-            transform = create_transform(
-                transform_x="axis", transform_y="data")
-            ax.hlines(sm_values[1], xmin=0, xmax=1, zorder=0, transform=transform,
+            transform = create_transform(transform_x="axis", transform_y="data")
+            ax.hlines(sm_values[1], xmin=0, xmax=1, zorder=2, transform=transform,
                       **sm_line_styles)
 
-        if show_legend:
-            handles, labels = self.get_legend_handles_labels()
-            ax.legend(handles, labels, **self.styles['legend'])
-
-        self.draw_axis_components(ax, xlabel=xlabel, ylabel=ylabel)
-        self.set_axis_range(ax, xmin=xmin, xmax=xmax, ymin=ymin, ymax=ymax)
+        # border for the legend
+        border_leg = patches.Rectangle((0, 0), 1, 1, facecolor = 'none', edgecolor = 'black', linewidth = 1)
+        self.legend_data['1sigma']['handle'] = (self.legend_data['1sigma']['handle'], border_leg)
+        self.legend_data['2sigma']['handle'] = (self.legend_data['2sigma']['handle'], border_leg)
+        
+        if self.data_sec is not None:
+            self.legend_data_sec['1sigma']['handle'] = (self.legend_data_sec['1sigma']['handle'], border_leg)
+            self.legend_data_sec['2sigma']['handle'] = (self.legend_data_sec['2sigma']['handle'], border_leg)
+            
+        handles, labels = self.get_legend_handles_labels()
+        if self.data_sec is not None:
+            handles_sec, labels_sec = self.get_legend_handles_labels(sec=True)
+            handles = handles + handles_sec
+            labels  = labels + labels_sec
+        ax.legend(handles, labels, **self.styles['legend'])
 
         return ax
 
-    def draw_highlight(self, ax, data, index=0):
-        styles = data['styles']
-        if styles is None:
-            styles = self.config['highlight_styles']
-        handle = ax.plot(data['x'], data['y'], label=data['label'], **styles)
-        self.update_legend_handles({f'highlight_{index}': handle[0]})
-        self.legend_order.append(f'highlight_{index}')
-
-    def add_highlight(self, x: float, y: float, label: str = "SM prediction",
-                      styles: Optional[Dict] = None):
-        highlight_data = {
-            'x': x,
-            'y': y,
-            'label': label,
-            'styles': styles
-        }
-        self.highlight_data.append(highlight_data)
```

### Comparing `quickstats-0.6.8.6/quickstats/plots/np_ranking_plot.py` & `quickstats-0.6.8.8/quickstats/plots/np_ranking_plot.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.6/quickstats/plots/pdf_distribution_plot.py` & `quickstats-0.6.8.8/quickstats/plots/pdf_distribution_plot.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.6/quickstats/plots/sample_purity_plot.py` & `quickstats-0.6.8.8/quickstats/plots/sample_purity_plot.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.6/quickstats/plots/score_distribution_plot.py` & `quickstats-0.6.8.8/quickstats/plots/score_distribution_plot.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.6/quickstats/plots/stat_plot_config.py` & `quickstats-0.6.8.8/quickstats/plots/stat_plot_config.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.6/quickstats/plots/template.py` & `quickstats-0.6.8.8/quickstats/plots/template.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.6/quickstats/plots/test_statistic_distribution_plot.py` & `quickstats-0.6.8.8/quickstats/plots/test_statistic_distribution_plot.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.6/quickstats/plots/upper_limit_1D_plot.py` & `quickstats-0.6.8.8/quickstats/plots/upper_limit_1D_plot.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.6/quickstats/plots/upper_limit_2D_plot.py` & `quickstats-0.6.8.8/quickstats/plots/upper_limit_2D_plot_deprecated.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.6/quickstats/plots/variable_distribution_plot.py` & `quickstats-0.6.8.8/quickstats/plots/variable_distribution_plot.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from matplotlib import colors
 from matplotlib.ticker import MaxNLocator
 from matplotlib.lines import Line2D
 from matplotlib.patches import Polygon
 
 from quickstats.plots import AbstractPlot, get_color_cycle
-from quickstats.plots.template import ratio_frames, suggest_markersize, centralize_axis
+from quickstats.plots.template import ratio_frames, centralize_axis
 from quickstats.utils.common_utils import combine_dict
 from quickstats.maths.numerics import safe_div
 from quickstats.maths.statistics import (HistComparisonMode,
                                          min_max_to_range, get_hist_data,
                                          get_stacked_hist_data,
                                          get_hist_comparison_data,
                                          get_clipped_data)
@@ -246,42 +246,15 @@
                 if target in plot_options:
                     component['error_styles']['color'] = plot_options[target]['error_styles']['color']
                 else:
                     component['error_styles']['color'] = component['styles']['color']
             component['mode'] = comparison_options['mode']
         comparison_options['components'] = components
         return comparison_options
-    
-    def decorate_comparison_axis(self, ax, xlabel:str="", ylabel:str="", 
-                                 mode:Union[HistComparisonMode, str]="ratio",
-                                 ylim:Optional[Sequence]=None,
-                                 ypad:Optional[float]=0.1,
-                                 draw_ratio_line:bool=True):
-        mode = HistComparisonMode.parse(mode)
-        if ylim is not None:
-            ax.set_ylim(ylim)
-        do_centralize_axis = ylim is None
-        if mode == HistComparisonMode.RATIO:
-            if do_centralize_axis:
-                centralize_axis(ax, which="y", ref_value=1, padding=ypad)
-            if draw_ratio_line:
-                ax.axhline(1, **self.config['ratio_line_styles'])
-        elif mode == HistComparisonMode.DIFFERENCE:
-            if do_centralize_axis:
-                centralize_axis(ax, which="y", ref_value=0, padding=ypad)
-            if draw_ratio_line:
-                ax.axhline(0, **self.config['ratio_line_styles'])
-        # set default ylabel if not given
-        if not ylabel:
-            if mode == HistComparisonMode.RATIO:
-                ylabel = "Ratio"
-            elif mode == HistComparisonMode.DIFFERENCE:
-                ylabel = "Difference"
-        self.draw_axis_components(ax, xlabel=xlabel, ylabel=ylabel)
-        
+
     def draw_comparison_data(self, ax, reference_data, target_data,
                              bin_edges:Optional[np.ndarray]=None,
                              mode:Union[HistComparisonMode, str]="ratio",
                              draw_error:bool=True,
                              plot_format:Union[PlotFormat, str]='errorbar',
                              error_format:Union[ErrorDisplayFormat, str]='errorbar',
                              styles:Optional[Dict]=None,
@@ -347,14 +320,15 @@
     
     def draw_stacked(self, ax, plot_options:Dict,
                      column_name:str, weight_name:Optional[str]=None,
                      bins:Union[int, Sequence]=25,
                      bin_range:Optional[Sequence]=None,
                      underflow:bool=False,
                      overflow:bool=False,
+                     divide_bin_width:bool=False,
                      normalize:bool=True,
                      show_error:bool=False,
                      variable_scale:Optional[float]=None):
         stacked_data = {
             'x'       : [],
             'weights' : [],
             'color'   : [],
@@ -372,43 +346,54 @@
                                               weight_name=weight_name)
             x = get_clipped_data(x, bin_range=bin_range, clip_lower=underflow, clip_upper=overflow)
             stacked_data['x'].append(x)
             stacked_data['weights'].append(weights)
             stacked_data['color'].append(color)
             stacked_data['label'].append(label)
             stacked_styles.append(styles)
-        if normalize:
-            norm_factor = np.sum([np.sum(weights) for weights in stacked_data['weights']])
-            stacked_data['weights'] = [weights / norm_factor for weights in stacked_data['weights']]
-        stacked_styles = {k:v for k,v in stacked_styles[0].items() if k not in ['color', 'label']}
-        hist_y, bin_edges, handle = ax.hist(**stacked_data,
-                                            bins=bins,
-                                            range=bin_range,
-                                            stacked=True,
-                                            **stacked_styles)
-        for i, target in enumerate(plot_options):
-            self.update_legend_handles({target:handle[i]})
         bin_edges = np.histogram_bin_edges(np.concatenate(stacked_data['x']).flatten(),
                                            bins=bins, range=bin_range)
         hist_data = get_stacked_hist_data(stacked_data['x'], stacked_data['weights'],
                                           underflow=underflow,
                                           overflow=overflow,
+                                          divide_bin_width=divide_bin_width,
                                           normalize=normalize,
                                           bin_range=bin_range, bins=bins,
                                           clip_weight=False,
                                           xerr=show_error and self.config['show_xerr'],
                                           yerr=show_error,
                                           error_option='auto')
+        stacked_styles = {k:v for k,v in stacked_styles[0].items() if k not in ['color', 'label']}
+        stacked_data_processed = get_stacked_hist_data(stacked_data['x'], stacked_data['weights'],
+                                                       underflow=underflow,
+                                                       overflow=overflow,
+                                                       divide_bin_width=divide_bin_width,
+                                                       normalize=normalize,
+                                                       bin_range=bin_range, bins=bins,
+                                                       clip_weight=False,
+                                                       xerr=False,
+                                                       yerr=False,
+                                                       merge=False,
+                                                       error_option='auto')
+        stacked_data['x'] = stacked_data_processed['x']
+        stacked_data['weights'] = stacked_data_processed['y']
+        hist_y, bin_edges_, handle = ax.hist(**stacked_data,
+                                             bins=bins,
+                                             range=bin_range,
+                                             stacked=True,
+                                             **stacked_styles)
+        for i, target in enumerate(plot_options):
+            self.update_legend_handles({target:handle[i]})
         return bin_edges, hist_data
             
     def draw(self, column_name:str, weight_name:Optional[str]=None,
              targets:Optional[List[str]]=None,
              xlabel:str="", ylabel:str="Fraction of Events / {bin_width:.2f}",
              bins:Union[int, Sequence]=25, bin_range:Optional[Sequence]=None,
-             underflow:bool=False, overflow:bool=False,
+             underflow:bool=False, overflow:bool=False, divide_bin_width:bool=False,
              normalize:bool=True, show_error:bool=False, show_error_legend:bool=False,
              stacked:bool=False, xmin:Optional[float]=None, xmax:Optional[float]=None,
              ymin:Optional[float]=None, ymax:Optional[float]=None, ypad:float=0.3,
              variable_scale:Optional[float]=None, logy:bool=False,
              comparison_options:Optional[Union[Dict, List[Dict]]]=None,
              legend_order:Optional[List[str]]=None):
         """
@@ -434,14 +419,16 @@
                 including the rightmost edge.
             bin_range: (optional) (float, float)
                 Range of histogram bins.
             underflow: bool, default = False
                 Include undeflow data in the first bin.
             overflow: bool, default = False
                 Include overflow data in the last bin.
+            divide_bin_width: bool, default = False
+                Divide each bin by the bin width.
             normalize: bool, default = True
                 Normalize the sum of weights to one. Weights outside the bin range will
                 not be counted if ``clip_weight`` is set to false, so the sum of bin
                 content could be less than one.
             show_error: bool, default = False
                 Whether to display data error.
             show_error_legend: bool, default = False
@@ -478,15 +465,16 @@
             self.legend_order.extend([f"{target}_error" for target in self.legend_order])
                 
         if comparison_options is not None:
             ax, ax_ratio = self.draw_frame(ratio_frames, logy=logy,
                                            **self.styles["ratio_frames"])
         else:
             ax = self.draw_frame(logy=logy)
-        if bin_range is None:
+            
+        if (bin_range is None) and isinstance(bins, (int, float)):
             relevant_samples = [sample for options in plot_options.values() \
                                 for sample in options['samples']]
             bin_range = self.deduce_bin_range(relevant_samples, column_name, variable_scale=variable_scale)
             self.stdout.info(f"Using deduced bin range ({bin_range[0]:.3f}, {bin_range[1]:.3f})")
 
         binned_data   = {}
         target_bin_edges = {}
@@ -507,14 +495,15 @@
                 bin_edges, hist_data = self.draw_stacked(ax, stacked_plot_options_i,
                                                          column_name=column_name,
                                                          weight_name=weight_name,
                                                          bins=bins, bin_range=bin_range,
                                                          underflow=underflow,
                                                          overflow=overflow,
                                                          normalize=normalize,
+                                                         divide_bin_width=divide_bin_width,
                                                          variable_scale=variable_scale)
                 label = self.config['stacked_label'].format(index=stack_index)
                 binned_data[label] = hist_data
                 target_bin_edges[label] = bin_edges
 
         for target, options in plot_options.items():
             samples, styles, error_styles = options['samples'], options['styles'], options['error_styles']
@@ -524,27 +513,28 @@
             x, weights = self.get_sample_data(samples, column_name,
                                               variable_scale=variable_scale,
                                               weight_scale=weight_scale,
                                               weight_name=weight_name)
             bin_edges = np.histogram_bin_edges(x, bins=bins, range=bin_range)
             hist_data = get_hist_data(x, weights, underflow=underflow,
                                       overflow=overflow, normalize=normalize,
+                                      divide_bin_width=divide_bin_width,
                                       bin_range=bin_range, bins=bins,
                                       clip_weight=False,
                                       xerr=show_error and self.config['show_xerr'],
                                       yerr=show_error,
                                       error_option='auto')
             binned_data[target] = hist_data
             target_bin_edges[target] = bin_edges
             if plot_format == PlotFormat.HIST:
-                if normalize:
-                    weights /= weights.sum()
-                x_ = get_clipped_data(x, bin_range=bin_range, clip_lower=underflow, clip_upper=overflow)
-                hist_y, _, handle = ax.hist(x_, bins, range=bin_range,
-                                            weights=weights, **styles)
+                #if normalize:
+                #    weights /= weights.sum()
+                #x_ = get_clipped_data(x, bin_range=bin_range, clip_lower=underflow, clip_upper=overflow)
+                hist_y, _, handle = ax.hist(hist_data['x'], bins, range=bin_range,
+                                            weights=hist_data['y'], **styles)
                 assert np.allclose(hist_data['y'], hist_y)
                 _, error_handle = self.draw_binned_data(ax, hist_data,
                                                         bin_edges=bin_edges,
                                                         draw_data=False,
                                                         draw_error=show_error,
                                                         error_format=error_format,
                                                         error_styles=error_styles)
@@ -554,15 +544,14 @@
                                                              styles=styles,
                                                              draw_error=show_error,
                                                              error_format=error_format,
                                                              error_styles=error_styles)
             self.update_legend_handles({target:handle})
             if error_handle is not None:
                 self.update_legend_handles({f"{target}_error": error_handle})
-                    
         # propagate bin width to ylabel if needed
         if isinstance(bins, int):
             bin_width = (bin_range[1] - bin_range[0]) / bins
             ylabel = ylabel.format(bin_width=bin_width)
         
         self.draw_axis_components(ax, xlabel=xlabel, ylabel=ylabel)
         self.set_axis_range(ax, xmin=xmin, xmax=xmax,
```

### Comparing `quickstats-0.6.8.6/quickstats/root_checker.py` & `quickstats-0.6.8.8/quickstats/root_checker.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.6/quickstats/utils/common_utils.py` & `quickstats-0.6.8.8/quickstats/utils/common_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -178,24 +178,24 @@
         sys.path.remove(scripts_path)
         os.environ["PYTHONPATH"].replace(scripts_path+":","")
         
     if (scripts_path not in sys.path) and (undo==False):
         sys.path.insert(0, scripts_path)
         os.environ["PYTHONPATH"] = scripts_path + ":" + os.environ.get("PYTHONPATH", "")
         
-def is_valid_file(fname:str):
-    if not fname:
+def is_valid_file(filename:str):
+    if not filename:
         return False
-    if not os.path.exists(fname):
+    if not os.path.exists(filename):
         return False
-    ext = os.path.splitext(fname)[-1]
+    ext = os.path.splitext(filename)[-1]
     if ext == ".root":
         from quickstats.utils.root_utils import is_corrupt
-        return not is_corrupt(fname)
-    return (os.path.isfile(fname)) and (os.path.getsize(fname) > 0)
+        return not is_corrupt(filename)
+    return (os.path.isfile(filename)) and (os.path.getsize(filename) > 0)
 
 def remove_list_duplicates(seq:List, keep_order:bool=True):
     if keep_order:
         seen = set()
         seen_add = seen.add
         return [x for x in seq if not (x in seen or seen_add(x))]
     else:
```

### Comparing `quickstats-0.6.8.6/quickstats/utils/data_conversion.py` & `quickstats-0.6.8.8/quickstats/utils/data_conversion.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.6/quickstats/utils/hep_utils.py` & `quickstats-0.6.8.8/quickstats/utils/hep_utils.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.6/quickstats/utils/io.py` & `quickstats-0.6.8.8/quickstats/utils/io.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.6/quickstats/utils/roofit_utils.py` & `quickstats-0.6.8.8/quickstats/utils/roofit_utils.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.6/quickstats/utils/roostats_utils.py` & `quickstats-0.6.8.8/quickstats/utils/roostats_utils.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.6/quickstats/utils/root_utils.py` & `quickstats-0.6.8.8/quickstats/utils/root_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -302,15 +302,15 @@
         column_map = {}
         all_columns = set()
         for rfile in rfiles:
             rdf = ROOT.RDataFrame(treename, rfile)
             columns = set([str(i) for i in rdf.GetColumnNames()])
             all_columns.update(columns)
             column_map[rfile] = columns
-        for fname, columns in column_map.items():
+        for rfile, columns in column_map.items():
             if columns != all_columns:
                 missing_columns = list(all_columns - columns)
                 stdout.warning(f"The root file \"{rfile}\" is missing the following column(s): "
                                f"{','.join(missing_columns)}. The missing column(s) will not be saved.")
         columns_to_keep = list(set.intersection(*column_map.values()))
         rdf = ROOT.RDataFrame(treename, rfiles)
         stdout.info(f"Target path: {target_file}", bare=True)
```

### Comparing `quickstats-0.6.8.6/quickstats/utils/string_utils.py` & `quickstats-0.6.8.8/quickstats/utils/string_utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -32,8 +32,11 @@
         tokens = [cast(s) for s in tokens]
     return tokens
 
 def remove_whitespace(string:str):
     return string.translate(whitespace_trans)
 
 def remove_newline(string:str):
-    return string.translate(newline_trans)
+    return string.translate(newline_trans)
+
+def remove_neg_zero(string:str):
+    return re.sub(r'(?![\w\d])-(0.[0]+)(?![\w\d])', r'\1', string)
```

### Comparing `quickstats-0.6.8.6/quickstats/utils/xml_tools.py` & `quickstats-0.6.8.8/quickstats/utils/xml_tools.py`

 * *Files 2% similar despite different names*

```diff
@@ -127,15 +127,15 @@
         if not isinstance(root, ET.Element):
             raise TypeError('root node must be ElementTree.Element, not %s' % (
                 root.__class__.__name__,))
         if not isinstance(source, ET.Element):
             raise TypeError('souce node must be ElementTree.Element, not %s' % (
                 source.__class__.__name__,))
         element_str = ET.tostring(source, 'unicode')
-        fieldnames = [fname for _, fname, _, _ in Formatter().parse(element_str) if fname]
+        fieldnames = [fieldname for _, fieldname, _, _ in Formatter().parse(element_str) if fieldname]
         argnames = argument_list.keys()
         if set(fieldnames) != set(argnames):
             raise ValueError('mismatch between field names in source node and argument names in argument list')
         
         arg_size = set(map(len, argument_list.values()))
         if len(arg_size) > 1:
             raise ValueError('argument lists must have the same size')
```

### Comparing `quickstats-0.6.8.6/quickstats.egg-info/PKG-INFO` & `quickstats-0.6.8.8/quickstats.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quickstats
-Version: 0.6.8.6
+Version: 0.6.8.8
 Summary: A tool for quick statistical analysis for HEP experiments
 Author: Alkaid Cheng
 Author-email: chi.lung.cheng@cern.ch
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `quickstats-0.6.8.6/quickstats.egg-info/SOURCES.txt` & `quickstats-0.6.8.8/quickstats.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -187,14 +187,15 @@
 quickstats/plots/sample_purity_plot.py
 quickstats/plots/score_distribution_plot.py
 quickstats/plots/stat_plot_config.py
 quickstats/plots/template.py
 quickstats/plots/test_statistic_distribution_plot.py
 quickstats/plots/upper_limit_1D_plot.py
 quickstats/plots/upper_limit_2D_plot.py
+quickstats/plots/upper_limit_2D_plot_deprecated.py
 quickstats/plots/upper_limit_3D_plot.py
 quickstats/plots/upper_limit_benchmark_plot.py
 quickstats/plots/variable_distribution_plot.py
 quickstats/resources/default_workspace_extensions.json
 quickstats/stylesheets/quick_default.mplstyle
 quickstats/utils/__init__.py
 quickstats/utils/common_utils.py
```

### Comparing `quickstats-0.6.8.6/setup.py` & `quickstats-0.6.8.8/setup.py`

 * *Files identical despite different names*

