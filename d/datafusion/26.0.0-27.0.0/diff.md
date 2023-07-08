# Comparing `tmp/datafusion-26.0.0.tar.gz` & `tmp/datafusion-27.0.0.tar.gz`

## Comparing `datafusion-26.0.0.tar` & `datafusion-27.0.0.tar`

### file list

```diff
@@ -1,101 +1,101 @@
--rw-r--r--   0        0        0     2300 1970-01-01 00:00:00.000000 datafusion-26.0.0/Cargo.toml
--rw-rw-r--   0     1000     1000    11358 2023-06-11 16:31:34.000000 datafusion-26.0.0/LICENSE.txt
--rw-rw-r--   0     1000     1000     8888 2023-06-11 16:31:34.000000 datafusion-26.0.0/README.md
--rw-rw-r--   0     1000     1000     4404 2023-06-11 16:31:34.000000 datafusion-26.0.0/datafusion/__init__.py
--rw-rw-r--   0     1000     1000      875 2023-06-11 16:31:34.000000 datafusion-26.0.0/datafusion/common.py
--rw-rw-r--   0     1000     1000     3664 2023-06-11 16:31:34.000000 datafusion-26.0.0/datafusion/context.py
--rw-rw-r--   0     1000     1000     3546 2023-06-11 16:31:34.000000 datafusion-26.0.0/datafusion/cudf.py
--rw-rw-r--   0     1000     1000      871 2023-06-11 16:31:34.000000 datafusion-26.0.0/datafusion/expr.py
--rw-rw-r--   0     1000     1000      881 2023-06-11 16:31:34.000000 datafusion-26.0.0/datafusion/functions.py
--rw-rw-r--   0     1000     1000      887 2023-06-11 16:31:34.000000 datafusion-26.0.0/datafusion/object_store.py
--rw-rw-r--   0     1000     1000     3507 2023-06-11 16:31:34.000000 datafusion-26.0.0/datafusion/pandas.py
--rw-rw-r--   0     1000     1000     4062 2023-06-11 16:31:34.000000 datafusion-26.0.0/datafusion/polars.py
--rw-rw-r--   0     1000     1000      881 2023-06-11 16:31:34.000000 datafusion-26.0.0/datafusion/substrait.py
--rw-rw-r--   0     1000     1000      785 2023-06-11 16:31:34.000000 datafusion-26.0.0/datafusion/tests/__init__.py
--rw-rw-r--   0     1000     1000     1443 2023-06-11 16:31:34.000000 datafusion-26.0.0/datafusion/tests/conftest.py
--rw-rw-r--   0     1000     1000       57 2023-06-11 16:31:34.000000 datafusion-26.0.0/datafusion/tests/data_test_context/data.json
--rw-rw-r--   0     1000     1000     2319 2023-06-11 16:31:34.000000 datafusion-26.0.0/datafusion/tests/generic.py
--rw-rw-r--   0     1000     1000     4339 2023-06-11 16:31:34.000000 datafusion-26.0.0/datafusion/tests/test_aggregation.py
--rw-rw-r--   0     1000     1000     1432 2023-06-11 16:31:34.000000 datafusion-26.0.0/datafusion/tests/test_catalog.py
--rw-rw-r--   0     1000     1000     1365 2023-06-11 16:31:34.000000 datafusion-26.0.0/datafusion/tests/test_config.py
--rw-rw-r--   0     1000     1000     9833 2023-06-11 16:31:34.000000 datafusion-26.0.0/datafusion/tests/test_context.py
--rw-rw-r--   0     1000     1000    17013 2023-06-11 16:31:34.000000 datafusion-26.0.0/datafusion/tests/test_dataframe.py
--rw-rw-r--   0     1000     1000     3179 2023-06-11 16:31:34.000000 datafusion-26.0.0/datafusion/tests/test_expr.py
--rw-rw-r--   0     1000     1000    14842 2023-06-11 16:31:34.000000 datafusion-26.0.0/datafusion/tests/test_functions.py
--rw-rw-r--   0     1000     1000     3984 2023-06-11 16:31:34.000000 datafusion-26.0.0/datafusion/tests/test_imports.py
--rw-rw-r--   0     1000     1000     1631 2023-06-11 16:31:34.000000 datafusion-26.0.0/datafusion/tests/test_indexing.py
--rw-rw-r--   0     1000     1000     9040 2023-06-11 16:31:34.000000 datafusion-26.0.0/datafusion/tests/test_sql.py
--rw-rw-r--   0     1000     1000     1355 2023-06-11 16:31:34.000000 datafusion-26.0.0/datafusion/tests/test_store.py
--rw-rw-r--   0     1000     1000     1949 2023-06-11 16:31:34.000000 datafusion-26.0.0/datafusion/tests/test_substrait.py
--rw-rw-r--   0     1000     1000     3619 2023-06-11 16:31:34.000000 datafusion-26.0.0/datafusion/tests/test_udaf.py
--rw-rw-r--   0     1000     1000     2177 2023-06-11 16:31:34.000000 datafusion-26.0.0/pyproject.toml
--rw-rw-r--   0     1000     1000     3964 2023-06-11 16:31:34.000000 datafusion-26.0.0/src/catalog.rs
--rw-rw-r--   0     1000     1000    22882 2023-06-11 16:31:34.000000 datafusion-26.0.0/src/common/data_type.rs
--rw-rw-r--   0     1000     1000     3557 2023-06-11 16:31:34.000000 datafusion-26.0.0/src/common/df_field.rs
--rw-rw-r--   0     1000     1000     1651 2023-06-11 16:31:34.000000 datafusion-26.0.0/src/common/df_schema.rs
--rw-rw-r--   0     1000     1000     1836 2023-06-11 16:31:34.000000 datafusion-26.0.0/src/common/function.rs
--rw-rw-r--   0     1000     1000     6256 2023-06-11 16:31:34.000000 datafusion-26.0.0/src/common/schema.rs
--rw-rw-r--   0     1000     1000     1613 2023-06-11 16:31:34.000000 datafusion-26.0.0/src/common.rs
--rw-rw-r--   0     1000     1000     3308 2023-06-11 16:31:34.000000 datafusion-26.0.0/src/config.rs
--rw-rw-r--   0     1000     1000    26417 2023-06-11 16:31:34.000000 datafusion-26.0.0/src/context.rs
--rw-rw-r--   0     1000     1000    15231 2023-06-11 16:31:34.000000 datafusion-26.0.0/src/dataframe.rs
--rw-rw-r--   0     1000     1000     4770 2023-06-11 16:31:34.000000 datafusion-26.0.0/src/dataset.rs
--rw-rw-r--   0     1000     1000     9944 2023-06-11 16:31:34.000000 datafusion-26.0.0/src/dataset_exec.rs
--rw-rw-r--   0     1000     1000     3054 2023-06-11 16:31:34.000000 datafusion-26.0.0/src/errors.rs
--rw-rw-r--   0     1000     1000     3243 2023-06-11 16:31:34.000000 datafusion-26.0.0/src/expr/aggregate.rs
--rw-rw-r--   0     1000     1000     2313 2023-06-11 16:31:34.000000 datafusion-26.0.0/src/expr/aggregate_expr.rs
--rw-rw-r--   0     1000     1000     1867 2023-06-11 16:31:34.000000 datafusion-26.0.0/src/expr/alias.rs
--rw-rw-r--   0     1000     1000     2331 2023-06-11 16:31:34.000000 datafusion-26.0.0/src/expr/analyze.rs
--rw-rw-r--   0     1000     1000     2101 2023-06-11 16:31:34.000000 datafusion-26.0.0/src/expr/between.rs
--rw-rw-r--   0     1000     1000     1626 2023-06-11 16:31:34.000000 datafusion-26.0.0/src/expr/binary_expr.rs
--rw-rw-r--   0     1000     1000     6317 2023-06-11 16:31:34.000000 datafusion-26.0.0/src/expr/bool_expr.rs
--rw-rw-r--   0     1000     1000     1662 2023-06-11 16:31:34.000000 datafusion-26.0.0/src/expr/case.rs
--rw-rw-r--   0     1000     1000     2060 2023-06-11 16:31:34.000000 datafusion-26.0.0/src/expr/cast.rs
--rw-rw-r--   0     1000     1000     1688 2023-06-11 16:31:34.000000 datafusion-26.0.0/src/expr/column.rs
--rw-rw-r--   0     1000     1000     2716 2023-06-11 16:31:34.000000 datafusion-26.0.0/src/expr/create_memory_table.rs
--rw-rw-r--   0     1000     1000     2574 2023-06-11 16:31:34.000000 datafusion-26.0.0/src/expr/create_view.rs
--rw-rw-r--   0     1000     1000     2867 2023-06-11 16:31:34.000000 datafusion-26.0.0/src/expr/cross_join.rs
--rw-rw-r--   0     1000     1000     2206 2023-06-11 16:31:34.000000 datafusion-26.0.0/src/expr/distinct.rs
--rw-rw-r--   0     1000     1000     2338 2023-06-11 16:31:34.000000 datafusion-26.0.0/src/expr/drop_table.rs
--rw-rw-r--   0     1000     1000     2522 2023-06-11 16:31:34.000000 datafusion-26.0.0/src/expr/empty_relation.rs
--rw-rw-r--   0     1000     1000     1334 2023-06-11 16:31:34.000000 datafusion-26.0.0/src/expr/exists.rs
--rw-rw-r--   0     1000     1000     3168 2023-06-11 16:31:34.000000 datafusion-26.0.0/src/expr/explain.rs
--rw-rw-r--   0     1000     1000     1535 2023-06-11 16:31:34.000000 datafusion-26.0.0/src/expr/extension.rs
--rw-rw-r--   0     1000     1000     2502 2023-06-11 16:31:34.000000 datafusion-26.0.0/src/expr/filter.rs
--rw-rw-r--   0     1000     1000     1293 2023-06-11 16:31:34.000000 datafusion-26.0.0/src/expr/grouping_set.rs
--rw-rw-r--   0     1000     1000     1495 2023-06-11 16:31:34.000000 datafusion-26.0.0/src/expr/in_list.rs
--rw-rw-r--   0     1000     1000     1531 2023-06-11 16:31:34.000000 datafusion-26.0.0/src/expr/in_subquery.rs
--rw-rw-r--   0     1000     1000     2093 2023-06-11 16:31:34.000000 datafusion-26.0.0/src/expr/indexed_field.rs
--rw-rw-r--   0     1000     1000     5153 2023-06-11 16:31:34.000000 datafusion-26.0.0/src/expr/join.rs
--rw-rw-r--   0     1000     1000     4441 2023-06-11 16:31:34.000000 datafusion-26.0.0/src/expr/like.rs
--rw-rw-r--   0     1000     1000     2584 2023-06-11 16:31:34.000000 datafusion-26.0.0/src/expr/limit.rs
--rw-rw-r--   0     1000     1000     5048 2023-06-11 16:31:34.000000 datafusion-26.0.0/src/expr/literal.rs
--rw-rw-r--   0     1000     1000     1199 2023-06-11 16:31:34.000000 datafusion-26.0.0/src/expr/logical_node.rs
--rw-rw-r--   0     1000     1000     1456 2023-06-11 16:31:34.000000 datafusion-26.0.0/src/expr/placeholder.rs
--rw-rw-r--   0     1000     1000     3557 2023-06-11 16:31:34.000000 datafusion-26.0.0/src/expr/projection.rs
--rw-rw-r--   0     1000     1000     3884 2023-06-11 16:31:34.000000 datafusion-26.0.0/src/expr/repartition.rs
--rw-rw-r--   0     1000     1000     2101 2023-06-11 16:31:34.000000 datafusion-26.0.0/src/expr/scalar_function.rs
--rw-rw-r--   0     1000     1000     1431 2023-06-11 16:31:34.000000 datafusion-26.0.0/src/expr/scalar_subquery.rs
--rw-rw-r--   0     1000     1000     1674 2023-06-11 16:31:34.000000 datafusion-26.0.0/src/expr/scalar_variable.rs
--rw-rw-r--   0     1000     1000     1310 2023-06-11 16:31:34.000000 datafusion-26.0.0/src/expr/signature.rs
--rw-rw-r--   0     1000     1000     2736 2023-06-11 16:31:34.000000 datafusion-26.0.0/src/expr/sort.rs
--rw-rw-r--   0     1000     1000     1233 2023-06-11 16:31:34.000000 datafusion-26.0.0/src/expr/subquery.rs
--rw-rw-r--   0     1000     1000     2754 2023-06-11 16:31:34.000000 datafusion-26.0.0/src/expr/subquery_alias.rs
--rw-rw-r--   0     1000     1000     4489 2023-06-11 16:31:34.000000 datafusion-26.0.0/src/expr/table_scan.rs
--rw-rw-r--   0     1000     1000     2470 2023-06-11 16:31:34.000000 datafusion-26.0.0/src/expr/union.rs
--rw-rw-r--   0     1000     1000    25039 2023-06-11 16:31:34.000000 datafusion-26.0.0/src/expr.rs
--rw-rw-r--   0     1000     1000    17966 2023-06-11 16:31:34.000000 datafusion-26.0.0/src/functions.rs
--rw-rw-r--   0     1000     1000     3778 2023-06-11 16:31:34.000000 datafusion-26.0.0/src/lib.rs
--rw-rw-r--   0     1000     1000     2265 2023-06-11 16:31:34.000000 datafusion-26.0.0/src/physical_plan.rs
--rw-rw-r--   0     1000     1000     8547 2023-06-11 16:31:34.000000 datafusion-26.0.0/src/pyarrow_filter_expression.rs
--rw-rw-r--   0     1000     1000     2055 2023-06-11 16:31:34.000000 datafusion-26.0.0/src/record_batch.rs
--rw-rw-r--   0     1000     1000     1716 2023-06-11 16:31:34.000000 datafusion-26.0.0/src/sql/exceptions.rs
--rw-rw-r--   0     1000     1000     4241 2023-06-11 16:31:34.000000 datafusion-26.0.0/src/sql/logical.rs
--rw-rw-r--   0     1000     1000      839 2023-06-11 16:31:34.000000 datafusion-26.0.0/src/sql.rs
--rw-rw-r--   0     1000     1000     7397 2023-06-11 16:31:34.000000 datafusion-26.0.0/src/store.rs
--rw-rw-r--   0     1000     1000     5211 2023-06-11 16:31:34.000000 datafusion-26.0.0/src/substrait.rs
--rw-rw-r--   0     1000     1000     4766 2023-06-11 16:31:34.000000 datafusion-26.0.0/src/udaf.rs
--rw-rw-r--   0     1000     1000     3535 2023-06-11 16:31:34.000000 datafusion-26.0.0/src/udf.rs
--rw-rw-r--   0     1000     1000     1961 2023-06-11 16:31:34.000000 datafusion-26.0.0/src/utils.rs
--rw-rw-r--   0     1000     1000    78278 2023-06-11 16:31:34.000000 datafusion-26.0.0/Cargo.lock
--rw-r--r--   0        0        0     9574 1970-01-01 00:00:00.000000 datafusion-26.0.0/PKG-INFO
+-rw-r--r--   0        0        0     2298 1970-01-01 00:00:00.000000 datafusion-27.0.0/Cargo.toml
+-rw-rw-r--   0     1000     1000    11358 2023-07-03 17:26:58.000000 datafusion-27.0.0/LICENSE.txt
+-rw-rw-r--   0     1000     1000     8888 2023-07-03 17:26:58.000000 datafusion-27.0.0/README.md
+-rw-rw-r--   0     1000     1000     4404 2023-07-03 17:26:58.000000 datafusion-27.0.0/datafusion/__init__.py
+-rw-rw-r--   0     1000     1000      875 2023-07-03 17:26:58.000000 datafusion-27.0.0/datafusion/common.py
+-rw-rw-r--   0     1000     1000     3664 2023-07-03 17:26:58.000000 datafusion-27.0.0/datafusion/context.py
+-rw-rw-r--   0     1000     1000     3546 2023-07-03 17:26:58.000000 datafusion-27.0.0/datafusion/cudf.py
+-rw-rw-r--   0     1000     1000      871 2023-07-03 17:26:58.000000 datafusion-27.0.0/datafusion/expr.py
+-rw-rw-r--   0     1000     1000      881 2023-07-03 17:26:58.000000 datafusion-27.0.0/datafusion/functions.py
+-rw-rw-r--   0     1000     1000      887 2023-07-03 17:26:58.000000 datafusion-27.0.0/datafusion/object_store.py
+-rw-rw-r--   0     1000     1000     3507 2023-07-03 17:26:58.000000 datafusion-27.0.0/datafusion/pandas.py
+-rw-rw-r--   0     1000     1000     4062 2023-07-03 17:26:58.000000 datafusion-27.0.0/datafusion/polars.py
+-rw-rw-r--   0     1000     1000      881 2023-07-03 17:26:58.000000 datafusion-27.0.0/datafusion/substrait.py
+-rw-rw-r--   0     1000     1000      785 2023-07-03 17:26:58.000000 datafusion-27.0.0/datafusion/tests/__init__.py
+-rw-rw-r--   0     1000     1000     1443 2023-07-03 17:26:58.000000 datafusion-27.0.0/datafusion/tests/conftest.py
+-rw-rw-r--   0     1000     1000       57 2023-07-03 17:26:58.000000 datafusion-27.0.0/datafusion/tests/data_test_context/data.json
+-rw-rw-r--   0     1000     1000     2319 2023-07-03 17:26:58.000000 datafusion-27.0.0/datafusion/tests/generic.py
+-rw-rw-r--   0     1000     1000     4339 2023-07-03 17:26:58.000000 datafusion-27.0.0/datafusion/tests/test_aggregation.py
+-rw-rw-r--   0     1000     1000     1432 2023-07-03 17:26:58.000000 datafusion-27.0.0/datafusion/tests/test_catalog.py
+-rw-rw-r--   0     1000     1000     1365 2023-07-03 17:26:58.000000 datafusion-27.0.0/datafusion/tests/test_config.py
+-rw-rw-r--   0     1000     1000     9833 2023-07-03 17:26:58.000000 datafusion-27.0.0/datafusion/tests/test_context.py
+-rw-rw-r--   0     1000     1000    17013 2023-07-03 17:26:58.000000 datafusion-27.0.0/datafusion/tests/test_dataframe.py
+-rw-rw-r--   0     1000     1000     3179 2023-07-03 17:26:58.000000 datafusion-27.0.0/datafusion/tests/test_expr.py
+-rw-rw-r--   0     1000     1000    14842 2023-07-03 17:26:58.000000 datafusion-27.0.0/datafusion/tests/test_functions.py
+-rw-rw-r--   0     1000     1000     3984 2023-07-03 17:26:58.000000 datafusion-27.0.0/datafusion/tests/test_imports.py
+-rw-rw-r--   0     1000     1000     1631 2023-07-03 17:26:58.000000 datafusion-27.0.0/datafusion/tests/test_indexing.py
+-rw-rw-r--   0     1000     1000     9040 2023-07-03 17:26:58.000000 datafusion-27.0.0/datafusion/tests/test_sql.py
+-rw-rw-r--   0     1000     1000     1370 2023-07-03 17:26:58.000000 datafusion-27.0.0/datafusion/tests/test_store.py
+-rw-rw-r--   0     1000     1000     1949 2023-07-03 17:26:58.000000 datafusion-27.0.0/datafusion/tests/test_substrait.py
+-rw-rw-r--   0     1000     1000     3619 2023-07-03 17:26:58.000000 datafusion-27.0.0/datafusion/tests/test_udaf.py
+-rw-rw-r--   0     1000     1000     2177 2023-07-03 17:26:58.000000 datafusion-27.0.0/pyproject.toml
+-rw-rw-r--   0     1000     1000     3950 2023-07-03 17:26:58.000000 datafusion-27.0.0/src/catalog.rs
+-rw-rw-r--   0     1000     1000    24898 2023-07-03 17:26:58.000000 datafusion-27.0.0/src/common/data_type.rs
+-rw-rw-r--   0     1000     1000     3557 2023-07-03 17:26:58.000000 datafusion-27.0.0/src/common/df_field.rs
+-rw-rw-r--   0     1000     1000     1651 2023-07-03 17:26:58.000000 datafusion-27.0.0/src/common/df_schema.rs
+-rw-rw-r--   0     1000     1000     1836 2023-07-03 17:26:58.000000 datafusion-27.0.0/src/common/function.rs
+-rw-rw-r--   0     1000     1000     6256 2023-07-03 17:26:58.000000 datafusion-27.0.0/src/common/schema.rs
+-rw-rw-r--   0     1000     1000     1613 2023-07-03 17:26:58.000000 datafusion-27.0.0/src/common.rs
+-rw-rw-r--   0     1000     1000     3308 2023-07-03 17:26:58.000000 datafusion-27.0.0/src/config.rs
+-rw-rw-r--   0     1000     1000    26405 2023-07-03 17:26:58.000000 datafusion-27.0.0/src/context.rs
+-rw-rw-r--   0     1000     1000    15226 2023-07-03 17:26:58.000000 datafusion-27.0.0/src/dataframe.rs
+-rw-rw-r--   0     1000     1000     4760 2023-07-03 17:26:58.000000 datafusion-27.0.0/src/dataset.rs
+-rw-rw-r--   0     1000     1000     9973 2023-07-03 17:26:58.000000 datafusion-27.0.0/src/dataset_exec.rs
+-rw-rw-r--   0     1000     1000     3054 2023-07-03 17:26:58.000000 datafusion-27.0.0/src/errors.rs
+-rw-rw-r--   0     1000     1000     3243 2023-07-03 17:26:58.000000 datafusion-27.0.0/src/expr/aggregate.rs
+-rw-rw-r--   0     1000     1000     2313 2023-07-03 17:26:58.000000 datafusion-27.0.0/src/expr/aggregate_expr.rs
+-rw-rw-r--   0     1000     1000     1867 2023-07-03 17:26:58.000000 datafusion-27.0.0/src/expr/alias.rs
+-rw-rw-r--   0     1000     1000     2331 2023-07-03 17:26:58.000000 datafusion-27.0.0/src/expr/analyze.rs
+-rw-rw-r--   0     1000     1000     2101 2023-07-03 17:26:58.000000 datafusion-27.0.0/src/expr/between.rs
+-rw-rw-r--   0     1000     1000     1626 2023-07-03 17:26:58.000000 datafusion-27.0.0/src/expr/binary_expr.rs
+-rw-rw-r--   0     1000     1000     6317 2023-07-03 17:26:58.000000 datafusion-27.0.0/src/expr/bool_expr.rs
+-rw-rw-r--   0     1000     1000     1662 2023-07-03 17:26:58.000000 datafusion-27.0.0/src/expr/case.rs
+-rw-rw-r--   0     1000     1000     2060 2023-07-03 17:26:58.000000 datafusion-27.0.0/src/expr/cast.rs
+-rw-rw-r--   0     1000     1000     1688 2023-07-03 17:26:58.000000 datafusion-27.0.0/src/expr/column.rs
+-rw-rw-r--   0     1000     1000     2716 2023-07-03 17:26:58.000000 datafusion-27.0.0/src/expr/create_memory_table.rs
+-rw-rw-r--   0     1000     1000     2967 2023-07-03 17:26:58.000000 datafusion-27.0.0/src/expr/create_view.rs
+-rw-rw-r--   0     1000     1000     2867 2023-07-03 17:26:58.000000 datafusion-27.0.0/src/expr/cross_join.rs
+-rw-rw-r--   0     1000     1000     2206 2023-07-03 17:26:58.000000 datafusion-27.0.0/src/expr/distinct.rs
+-rw-rw-r--   0     1000     1000     2338 2023-07-03 17:26:58.000000 datafusion-27.0.0/src/expr/drop_table.rs
+-rw-rw-r--   0     1000     1000     2522 2023-07-03 17:26:58.000000 datafusion-27.0.0/src/expr/empty_relation.rs
+-rw-rw-r--   0     1000     1000     1334 2023-07-03 17:26:58.000000 datafusion-27.0.0/src/expr/exists.rs
+-rw-rw-r--   0     1000     1000     3168 2023-07-03 17:26:58.000000 datafusion-27.0.0/src/expr/explain.rs
+-rw-rw-r--   0     1000     1000     1535 2023-07-03 17:26:58.000000 datafusion-27.0.0/src/expr/extension.rs
+-rw-rw-r--   0     1000     1000     2502 2023-07-03 17:26:58.000000 datafusion-27.0.0/src/expr/filter.rs
+-rw-rw-r--   0     1000     1000     1293 2023-07-03 17:26:58.000000 datafusion-27.0.0/src/expr/grouping_set.rs
+-rw-rw-r--   0     1000     1000     1495 2023-07-03 17:26:58.000000 datafusion-27.0.0/src/expr/in_list.rs
+-rw-rw-r--   0     1000     1000     1531 2023-07-03 17:26:58.000000 datafusion-27.0.0/src/expr/in_subquery.rs
+-rw-rw-r--   0     1000     1000     2093 2023-07-03 17:26:58.000000 datafusion-27.0.0/src/expr/indexed_field.rs
+-rw-rw-r--   0     1000     1000     5153 2023-07-03 17:26:58.000000 datafusion-27.0.0/src/expr/join.rs
+-rw-rw-r--   0     1000     1000     4441 2023-07-03 17:26:58.000000 datafusion-27.0.0/src/expr/like.rs
+-rw-rw-r--   0     1000     1000     2584 2023-07-03 17:26:58.000000 datafusion-27.0.0/src/expr/limit.rs
+-rw-rw-r--   0     1000     1000     5048 2023-07-03 17:26:58.000000 datafusion-27.0.0/src/expr/literal.rs
+-rw-rw-r--   0     1000     1000     1199 2023-07-03 17:26:58.000000 datafusion-27.0.0/src/expr/logical_node.rs
+-rw-rw-r--   0     1000     1000     1456 2023-07-03 17:26:58.000000 datafusion-27.0.0/src/expr/placeholder.rs
+-rw-rw-r--   0     1000     1000     3557 2023-07-03 17:26:58.000000 datafusion-27.0.0/src/expr/projection.rs
+-rw-rw-r--   0     1000     1000     3884 2023-07-03 17:26:58.000000 datafusion-27.0.0/src/expr/repartition.rs
+-rw-rw-r--   0     1000     1000     2101 2023-07-03 17:26:58.000000 datafusion-27.0.0/src/expr/scalar_function.rs
+-rw-rw-r--   0     1000     1000     1431 2023-07-03 17:26:58.000000 datafusion-27.0.0/src/expr/scalar_subquery.rs
+-rw-rw-r--   0     1000     1000     1674 2023-07-03 17:26:58.000000 datafusion-27.0.0/src/expr/scalar_variable.rs
+-rw-rw-r--   0     1000     1000     1310 2023-07-03 17:26:58.000000 datafusion-27.0.0/src/expr/signature.rs
+-rw-rw-r--   0     1000     1000     2736 2023-07-03 17:26:58.000000 datafusion-27.0.0/src/expr/sort.rs
+-rw-rw-r--   0     1000     1000     2228 2023-07-03 17:26:58.000000 datafusion-27.0.0/src/expr/subquery.rs
+-rw-rw-r--   0     1000     1000     2754 2023-07-03 17:26:58.000000 datafusion-27.0.0/src/expr/subquery_alias.rs
+-rw-rw-r--   0     1000     1000     4489 2023-07-03 17:26:58.000000 datafusion-27.0.0/src/expr/table_scan.rs
+-rw-rw-r--   0     1000     1000     2470 2023-07-03 17:26:58.000000 datafusion-27.0.0/src/expr/union.rs
+-rw-rw-r--   0     1000     1000    25260 2023-07-03 17:26:58.000000 datafusion-27.0.0/src/expr.rs
+-rw-rw-r--   0     1000     1000    17966 2023-07-03 17:26:58.000000 datafusion-27.0.0/src/functions.rs
+-rw-rw-r--   0     1000     1000     3778 2023-07-03 17:26:58.000000 datafusion-27.0.0/src/lib.rs
+-rw-rw-r--   0     1000     1000     2270 2023-07-03 17:26:58.000000 datafusion-27.0.0/src/physical_plan.rs
+-rw-rw-r--   0     1000     1000     8547 2023-07-03 17:26:58.000000 datafusion-27.0.0/src/pyarrow_filter_expression.rs
+-rw-rw-r--   0     1000     1000     2050 2023-07-03 17:26:58.000000 datafusion-27.0.0/src/record_batch.rs
+-rw-rw-r--   0     1000     1000     1716 2023-07-03 17:26:58.000000 datafusion-27.0.0/src/sql/exceptions.rs
+-rw-rw-r--   0     1000     1000     4524 2023-07-03 17:26:58.000000 datafusion-27.0.0/src/sql/logical.rs
+-rw-rw-r--   0     1000     1000      839 2023-07-03 17:26:58.000000 datafusion-27.0.0/src/sql.rs
+-rw-rw-r--   0     1000     1000     7397 2023-07-03 17:26:58.000000 datafusion-27.0.0/src/store.rs
+-rw-rw-r--   0     1000     1000     5211 2023-07-03 17:26:58.000000 datafusion-27.0.0/src/substrait.rs
+-rw-rw-r--   0     1000     1000     4747 2023-07-03 17:26:58.000000 datafusion-27.0.0/src/udaf.rs
+-rw-rw-r--   0     1000     1000     3543 2023-07-03 17:26:58.000000 datafusion-27.0.0/src/udf.rs
+-rw-rw-r--   0     1000     1000     1961 2023-07-03 17:26:58.000000 datafusion-27.0.0/src/utils.rs
+-rw-rw-r--   0     1000     1000    80851 2023-07-03 17:26:58.000000 datafusion-27.0.0/Cargo.lock
+-rw-r--r--   0        0        0     9574 1970-01-01 00:00:00.000000 datafusion-27.0.0/PKG-INFO
```

### Comparing `datafusion-26.0.0/Cargo.toml` & `datafusion-27.0.0/Cargo.toml`

 * *Files 17% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 [package]
 name = "datafusion-python"
-version = "26.0.0"
+version = "27.0.0"
 homepage = "https://github.com/apache/arrow-datafusion-python"
 repository = "https://github.com/apache/arrow-datafusion-python"
 authors = ["Apache Arrow <dev@arrow.apache.org>"]
 description = "Apache Arrow DataFusion DataFrame and SQL Query Engine"
 readme = "README.md"
 license = "Apache-2.0"
 edition = "2021"
@@ -31,35 +31,35 @@
 [features]
 default = ["mimalloc"]
 protoc = [ "datafusion-substrait/protoc" ]
 
 [dependencies]
 tokio = { version = "1.24", features = ["macros", "rt", "rt-multi-thread", "sync"] }
 rand = "0.8"
-pyo3 = { version = "0.18.1", features = ["extension-module", "abi3", "abi3-py37"] }
-datafusion = { version = "26.0.0" , features = ["pyarrow", "avro"] }
-datafusion-common = { version = "26.0.0", features = ["pyarrow"] }
-datafusion-expr = "26.0.0"
-datafusion-optimizer = "26.0.0"
-datafusion-sql = "26.0.0"
-datafusion-substrait = "26.0.0"
+pyo3 = { version = "0.19", features = ["extension-module", "abi3", "abi3-py38"] }
+datafusion = { version = "27.0.0" , features = ["pyarrow", "avro"] }
+datafusion-common = { version = "27.0.0", features = ["pyarrow"] }
+datafusion-expr = "27.0.0"
+datafusion-optimizer = "27.0.0"
+datafusion-sql = "27.0.0"
+datafusion-substrait = "27.0.0"
 prost = "0.11"
 prost-types = "0.11"
 uuid = { version = "1.3", features = ["v4"] }
 mimalloc = { version = "0.1", optional = true, default-features = false }
 async-trait = "0.1"
 futures = "0.3"
-object_store = { version = "0.5.4", features = ["aws", "gcp", "azure"] }
+object_store = { version = "0.6.1", features = ["aws", "gcp", "azure"] }
 parking_lot = "0.12"
 regex-syntax = "0.7.1"
 syn = "2.0.11"
 url = "2.2"
 
 [build-dependencies]
-pyo3-build-config = "0.18.3"
+pyo3-build-config = "0.19.0"
 
 [lib]
 name = "datafusion_python"
 crate-type = ["cdylib", "rlib"]
 
 [profile.release]
 lto = true
```

### Comparing `datafusion-26.0.0/LICENSE.txt` & `datafusion-27.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `datafusion-26.0.0/README.md` & `datafusion-27.0.0/README.md`

 * *Files identical despite different names*

### Comparing `datafusion-26.0.0/datafusion/__init__.py` & `datafusion-27.0.0/datafusion/__init__.py`

 * *Files identical despite different names*

### Comparing `datafusion-26.0.0/datafusion/common.py` & `datafusion-27.0.0/datafusion/common.py`

 * *Files identical despite different names*

### Comparing `datafusion-26.0.0/datafusion/context.py` & `datafusion-27.0.0/datafusion/context.py`

 * *Files identical despite different names*

### Comparing `datafusion-26.0.0/datafusion/cudf.py` & `datafusion-27.0.0/datafusion/cudf.py`

 * *Files identical despite different names*

### Comparing `datafusion-26.0.0/datafusion/expr.py` & `datafusion-27.0.0/datafusion/expr.py`

 * *Files identical despite different names*

### Comparing `datafusion-26.0.0/datafusion/functions.py` & `datafusion-27.0.0/datafusion/functions.py`

 * *Files identical despite different names*

### Comparing `datafusion-26.0.0/datafusion/object_store.py` & `datafusion-27.0.0/datafusion/object_store.py`

 * *Files identical despite different names*

### Comparing `datafusion-26.0.0/datafusion/pandas.py` & `datafusion-27.0.0/datafusion/pandas.py`

 * *Files identical despite different names*

### Comparing `datafusion-26.0.0/datafusion/polars.py` & `datafusion-27.0.0/datafusion/polars.py`

 * *Files identical despite different names*

### Comparing `datafusion-26.0.0/datafusion/substrait.py` & `datafusion-27.0.0/datafusion/substrait.py`

 * *Files identical despite different names*

### Comparing `datafusion-26.0.0/datafusion/tests/__init__.py` & `datafusion-27.0.0/datafusion/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `datafusion-26.0.0/datafusion/tests/conftest.py` & `datafusion-27.0.0/datafusion/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `datafusion-26.0.0/datafusion/tests/generic.py` & `datafusion-27.0.0/datafusion/tests/generic.py`

 * *Files identical despite different names*

### Comparing `datafusion-26.0.0/datafusion/tests/test_aggregation.py` & `datafusion-27.0.0/datafusion/tests/test_aggregation.py`

 * *Files identical despite different names*

### Comparing `datafusion-26.0.0/datafusion/tests/test_catalog.py` & `datafusion-27.0.0/datafusion/tests/test_catalog.py`

 * *Files identical despite different names*

### Comparing `datafusion-26.0.0/datafusion/tests/test_config.py` & `datafusion-27.0.0/datafusion/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `datafusion-26.0.0/datafusion/tests/test_context.py` & `datafusion-27.0.0/datafusion/tests/test_context.py`

 * *Files identical despite different names*

### Comparing `datafusion-26.0.0/datafusion/tests/test_dataframe.py` & `datafusion-27.0.0/datafusion/tests/test_dataframe.py`

 * *Files identical despite different names*

### Comparing `datafusion-26.0.0/datafusion/tests/test_expr.py` & `datafusion-27.0.0/datafusion/tests/test_expr.py`

 * *Files identical despite different names*

### Comparing `datafusion-26.0.0/datafusion/tests/test_functions.py` & `datafusion-27.0.0/datafusion/tests/test_functions.py`

 * *Files identical despite different names*

### Comparing `datafusion-26.0.0/datafusion/tests/test_imports.py` & `datafusion-27.0.0/datafusion/tests/test_imports.py`

 * *Files identical despite different names*

### Comparing `datafusion-26.0.0/datafusion/tests/test_indexing.py` & `datafusion-27.0.0/datafusion/tests/test_indexing.py`

 * *Files identical despite different names*

### Comparing `datafusion-26.0.0/datafusion/tests/test_sql.py` & `datafusion-27.0.0/datafusion/tests/test_sql.py`

 * *Files identical despite different names*

### Comparing `datafusion-26.0.0/datafusion/tests/test_store.py` & `datafusion-27.0.0/datafusion/tests/test_store.py`

 * *Files 12% similar despite different names*

```diff
@@ -33,14 +33,14 @@
     ctx.register_object_store("file://local", local, None)
     return ctx
 
 
 def test_read_parquet(ctx):
     ctx.register_parquet(
         "test",
-        f"file://{os.getcwd()}/testing/data/parquet",
+        f"file://{os.getcwd()}/parquet/data/alltypes_plain.parquet",
         [],
         True,
         ".parquet",
     )
     df = ctx.sql("SELECT * FROM test")
     assert isinstance(df.collect(), list)
```

### Comparing `datafusion-26.0.0/datafusion/tests/test_substrait.py` & `datafusion-27.0.0/datafusion/tests/test_substrait.py`

 * *Files identical despite different names*

### Comparing `datafusion-26.0.0/datafusion/tests/test_udaf.py` & `datafusion-27.0.0/datafusion/tests/test_udaf.py`

 * *Files identical despite different names*

### Comparing `datafusion-26.0.0/pyproject.toml` & `datafusion-27.0.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `datafusion-26.0.0/src/catalog.rs` & `datafusion-27.0.0/src/catalog.rs`

 * *Files 6% similar despite different names*

```diff
@@ -20,16 +20,16 @@
 
 use pyo3::exceptions::PyKeyError;
 use pyo3::prelude::*;
 
 use crate::errors::DataFusionError;
 use crate::utils::wait_for_future;
 use datafusion::{
-    arrow::pyarrow::PyArrowConvert,
-    catalog::{catalog::CatalogProvider, schema::SchemaProvider},
+    arrow::pyarrow::ToPyArrow,
+    catalog::{schema::SchemaProvider, CatalogProvider},
     datasource::{TableProvider, TableType},
 };
 
 #[pyclass(name = "Catalog", module = "datafusion", subclass)]
 pub(crate) struct PyCatalog {
     catalog: Arc<dyn CatalogProvider>,
 }
```

### Comparing `datafusion-26.0.0/src/common/data_type.rs` & `datafusion-27.0.0/src/common/data_type.rs`

 * *Files 6% similar despite different names*

```diff
@@ -499,14 +499,58 @@
             SqlType::VARCHAR => Ok(DataTypeMap::new(
                 DataType::Utf8,
                 PythonType::Str,
                 SqlType::VARCHAR,
             )),
         }
     }
+
+    /// Unfortunately PyO3 does not allow for us to expose the DataType as an enum since
+    /// we cannot directly annotae the Enum instance of dependency code. Therefore, here
+    /// we provide an enum to mimic it.
+    #[pyo3(name = "friendly_arrow_type_name")]
+    pub fn friendly_arrow_type_name(&self) -> PyResult<&str> {
+        Ok(match &self.arrow_type.data_type {
+            DataType::Null => "Null",
+            DataType::Boolean => "Boolean",
+            DataType::Int8 => "Int8",
+            DataType::Int16 => "Int16",
+            DataType::Int32 => "Int32",
+            DataType::Int64 => "Int64",
+            DataType::UInt8 => "UInt8",
+            DataType::UInt16 => "UInt16",
+            DataType::UInt32 => "UInt32",
+            DataType::UInt64 => "UInt64",
+            DataType::Float16 => "Float16",
+            DataType::Float32 => "Float32",
+            DataType::Float64 => "Float64",
+            DataType::Timestamp(_, _) => "Timestamp",
+            DataType::Date32 => "Date32",
+            DataType::Date64 => "Date64",
+            DataType::Time32(_) => "Time32",
+            DataType::Time64(_) => "Time64",
+            DataType::Duration(_) => "Duration",
+            DataType::Interval(_) => "Interval",
+            DataType::Binary => "Binary",
+            DataType::FixedSizeBinary(_) => "FixedSizeBinary",
+            DataType::LargeBinary => "LargeBinary",
+            DataType::Utf8 => "Utf8",
+            DataType::LargeUtf8 => "LargeUtf8",
+            DataType::List(_) => "List",
+            DataType::FixedSizeList(_, _) => "FixedSizeList",
+            DataType::LargeList(_) => "LargeList",
+            DataType::Struct(_) => "Struct",
+            DataType::Union(_, _) => "Union",
+            DataType::Dictionary(_, _) => "Dictionary",
+            DataType::Decimal128(_, _) => "Decimal128",
+            DataType::Decimal256(_, _) => "Decimal256",
+            DataType::Map(_, _) => "Map",
+            DataType::RunEndEncoded(_, _) => "RunEndEncoded",
+        })
+    }
 }
 
 /// PyO3 requires that objects passed between Rust and Python implement the trait `PyClass`
 /// Since `DataType` exists in another package we cannot make that happen here so we wrap
 /// `DataType` as `PyDataType` This exists solely to satisfy those constraints.
 #[derive(Debug, Clone, PartialEq, Eq, Hash, PartialOrd, Ord)]
 #[pyclass(name = "DataType", module = "datafusion.common")]
```

### Comparing `datafusion-26.0.0/src/common/df_field.rs` & `datafusion-27.0.0/src/common/df_field.rs`

 * *Files identical despite different names*

### Comparing `datafusion-26.0.0/src/common/df_schema.rs` & `datafusion-27.0.0/src/common/df_schema.rs`

 * *Files identical despite different names*

### Comparing `datafusion-26.0.0/src/common/function.rs` & `datafusion-27.0.0/src/common/function.rs`

 * *Files identical despite different names*

### Comparing `datafusion-26.0.0/src/common/schema.rs` & `datafusion-27.0.0/src/common/schema.rs`

 * *Files identical despite different names*

### Comparing `datafusion-26.0.0/src/common.rs` & `datafusion-27.0.0/src/common.rs`

 * *Files identical despite different names*

### Comparing `datafusion-26.0.0/src/config.rs` & `datafusion-27.0.0/src/config.rs`

 * *Files identical despite different names*

### Comparing `datafusion-26.0.0/src/context.rs` & `datafusion-27.0.0/src/context.rs`

 * *Files 1% similar despite different names*

```diff
@@ -36,16 +36,16 @@
 use crate::store::StorageContexts;
 use crate::udaf::PyAggregateUDF;
 use crate::udf::PyScalarUDF;
 use crate::utils::{get_tokio_runtime, wait_for_future};
 use datafusion::arrow::datatypes::{DataType, Schema};
 use datafusion::arrow::pyarrow::PyArrowType;
 use datafusion::arrow::record_batch::RecordBatch;
-use datafusion::datasource::datasource::TableProvider;
 use datafusion::datasource::MemTable;
+use datafusion::datasource::TableProvider;
 use datafusion::execution::context::{SessionConfig, SessionContext, TaskContext};
 use datafusion::execution::disk_manager::DiskManagerConfig;
 use datafusion::execution::memory_pool::{FairSpillPool, GreedyMemoryPool, UnboundedMemoryPool};
 use datafusion::execution::runtime_env::{RuntimeConfig, RuntimeEnv};
 use datafusion::physical_plan::SendableRecordBatchStream;
 use datafusion::prelude::{
     AvroReadOptions, CsvReadOptions, DataFrame, NdJsonReadOptions, ParquetReadOptions,
```

### Comparing `datafusion-26.0.0/src/dataframe.rs` & `datafusion-27.0.0/src/dataframe.rs`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 // under the License.
 
 use crate::physical_plan::PyExecutionPlan;
 use crate::sql::logical::PyLogicalPlan;
 use crate::utils::wait_for_future;
 use crate::{errors::DataFusionError, expr::PyExpr};
 use datafusion::arrow::datatypes::Schema;
-use datafusion::arrow::pyarrow::{PyArrowConvert, PyArrowType};
+use datafusion::arrow::pyarrow::{PyArrowType, ToPyArrow};
 use datafusion::arrow::util::pretty;
 use datafusion::dataframe::DataFrame;
 use datafusion::prelude::*;
 use pyo3::exceptions::PyTypeError;
 use pyo3::prelude::*;
 use pyo3::types::PyTuple;
 use std::sync::Arc;
```

### Comparing `datafusion-26.0.0/src/dataset.rs` & `datafusion-27.0.0/src/dataset.rs`

 * *Files 1% similar despite different names*

```diff
@@ -24,18 +24,18 @@
 use std::any::Any;
 use std::sync::Arc;
 
 use async_trait::async_trait;
 
 use datafusion::arrow::datatypes::SchemaRef;
 use datafusion::arrow::pyarrow::PyArrowType;
-use datafusion::datasource::datasource::TableProviderFilterPushDown;
 use datafusion::datasource::{TableProvider, TableType};
 use datafusion::error::{DataFusionError, Result as DFResult};
 use datafusion::execution::context::SessionState;
+use datafusion::logical_expr::TableProviderFilterPushDown;
 use datafusion::physical_plan::ExecutionPlan;
 use datafusion_expr::Expr;
 
 use crate::dataset_exec::DatasetExec;
 use crate::pyarrow_filter_expression::PyArrowFilterExpression;
 
 // Wraps a pyarrow.dataset.Dataset class and implements a Datafusion TableProvider around it
```

### Comparing `datafusion-26.0.0/src/dataset_exec.rs` & `datafusion-27.0.0/src/dataset_exec.rs`

 * *Files 0% similar despite different names*

```diff
@@ -235,15 +235,15 @@
         })
     }
 
     fn fmt_as(&self, t: DisplayFormatType, f: &mut std::fmt::Formatter) -> std::fmt::Result {
         Python::with_gil(|py| {
             let number_of_fragments = self.fragments.as_ref(py).len();
             match t {
-                DisplayFormatType::Default => {
+                DisplayFormatType::Default | DisplayFormatType::Verbose => {
                     let projected_columns: Vec<String> = self
                         .schema
                         .fields()
                         .iter()
                         .map(|x| x.name().to_owned())
                         .collect();
                     if let Some(filter_expr) = &self.filter_expr {
```

### Comparing `datafusion-26.0.0/src/errors.rs` & `datafusion-27.0.0/src/errors.rs`

 * *Files identical despite different names*

### Comparing `datafusion-26.0.0/src/expr/aggregate.rs` & `datafusion-27.0.0/src/expr/aggregate.rs`

 * *Files identical despite different names*

### Comparing `datafusion-26.0.0/src/expr/aggregate_expr.rs` & `datafusion-27.0.0/src/expr/aggregate_expr.rs`

 * *Files identical despite different names*

### Comparing `datafusion-26.0.0/src/expr/alias.rs` & `datafusion-27.0.0/src/expr/alias.rs`

 * *Files identical despite different names*

### Comparing `datafusion-26.0.0/src/expr/analyze.rs` & `datafusion-27.0.0/src/expr/analyze.rs`

 * *Files identical despite different names*

### Comparing `datafusion-26.0.0/src/expr/between.rs` & `datafusion-27.0.0/src/expr/between.rs`

 * *Files identical despite different names*

### Comparing `datafusion-26.0.0/src/expr/binary_expr.rs` & `datafusion-27.0.0/src/expr/binary_expr.rs`

 * *Files identical despite different names*

### Comparing `datafusion-26.0.0/src/expr/bool_expr.rs` & `datafusion-27.0.0/src/expr/bool_expr.rs`

 * *Files identical despite different names*

### Comparing `datafusion-26.0.0/src/expr/case.rs` & `datafusion-27.0.0/src/expr/case.rs`

 * *Files identical despite different names*

### Comparing `datafusion-26.0.0/src/expr/cast.rs` & `datafusion-27.0.0/src/expr/cast.rs`

 * *Files identical despite different names*

### Comparing `datafusion-26.0.0/src/expr/column.rs` & `datafusion-27.0.0/src/expr/column.rs`

 * *Files identical despite different names*

### Comparing `datafusion-26.0.0/src/expr/create_memory_table.rs` & `datafusion-27.0.0/src/expr/create_memory_table.rs`

 * *Files identical despite different names*

### Comparing `datafusion-26.0.0/src/expr/create_view.rs` & `datafusion-27.0.0/src/expr/create_view.rs`

 * *Files 22% similar despite different names*

```diff
@@ -13,18 +13,18 @@
 // "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 // KIND, either express or implied.  See the License for the
 // specific language governing permissions and limitations
 // under the License.
 
 use std::fmt::{self, Display, Formatter};
 
-use datafusion_expr::CreateView;
+use datafusion_expr::{CreateView, DdlStatement, LogicalPlan};
 use pyo3::prelude::*;
 
-use crate::sql::logical::PyLogicalPlan;
+use crate::{errors::py_type_err, sql::logical::PyLogicalPlan};
 
 use super::logical_node::LogicalNode;
 
 #[pyclass(name = "CreateView", module = "datafusion.expr", subclass)]
 #[derive(Clone)]
 pub struct PyCreateView {
     create: CreateView,
@@ -88,7 +88,18 @@
         vec![PyLogicalPlan::from((*self.create.input).clone())]
     }
 
     fn to_variant(&self, py: Python) -> PyResult<PyObject> {
         Ok(self.clone().into_py(py))
     }
 }
+
+impl TryFrom<LogicalPlan> for PyCreateView {
+    type Error = PyErr;
+
+    fn try_from(logical_plan: LogicalPlan) -> Result<Self, Self::Error> {
+        match logical_plan {
+            LogicalPlan::Ddl(DdlStatement::CreateView(create)) => Ok(PyCreateView { create }),
+            _ => Err(py_type_err("unexpected plan")),
+        }
+    }
+}
```

### Comparing `datafusion-26.0.0/src/expr/cross_join.rs` & `datafusion-27.0.0/src/expr/cross_join.rs`

 * *Files identical despite different names*

### Comparing `datafusion-26.0.0/src/expr/distinct.rs` & `datafusion-27.0.0/src/expr/distinct.rs`

 * *Files identical despite different names*

### Comparing `datafusion-26.0.0/src/expr/drop_table.rs` & `datafusion-27.0.0/src/expr/drop_table.rs`

 * *Files identical despite different names*

### Comparing `datafusion-26.0.0/src/expr/empty_relation.rs` & `datafusion-27.0.0/src/expr/empty_relation.rs`

 * *Files identical despite different names*

### Comparing `datafusion-26.0.0/src/expr/exists.rs` & `datafusion-27.0.0/src/expr/exists.rs`

 * *Files identical despite different names*

### Comparing `datafusion-26.0.0/src/expr/explain.rs` & `datafusion-27.0.0/src/expr/explain.rs`

 * *Files identical despite different names*

### Comparing `datafusion-26.0.0/src/expr/extension.rs` & `datafusion-27.0.0/src/expr/extension.rs`

 * *Files identical despite different names*

### Comparing `datafusion-26.0.0/src/expr/filter.rs` & `datafusion-27.0.0/src/expr/filter.rs`

 * *Files identical despite different names*

### Comparing `datafusion-26.0.0/src/expr/grouping_set.rs` & `datafusion-27.0.0/src/expr/grouping_set.rs`

 * *Files identical despite different names*

### Comparing `datafusion-26.0.0/src/expr/in_list.rs` & `datafusion-27.0.0/src/expr/in_list.rs`

 * *Files identical despite different names*

### Comparing `datafusion-26.0.0/src/expr/in_subquery.rs` & `datafusion-27.0.0/src/expr/in_subquery.rs`

 * *Files identical despite different names*

### Comparing `datafusion-26.0.0/src/expr/indexed_field.rs` & `datafusion-27.0.0/src/expr/indexed_field.rs`

 * *Files identical despite different names*

### Comparing `datafusion-26.0.0/src/expr/join.rs` & `datafusion-27.0.0/src/expr/join.rs`

 * *Files identical despite different names*

### Comparing `datafusion-26.0.0/src/expr/like.rs` & `datafusion-27.0.0/src/expr/like.rs`

 * *Files identical despite different names*

### Comparing `datafusion-26.0.0/src/expr/limit.rs` & `datafusion-27.0.0/src/expr/limit.rs`

 * *Files identical despite different names*

### Comparing `datafusion-26.0.0/src/expr/literal.rs` & `datafusion-27.0.0/src/expr/literal.rs`

 * *Files identical despite different names*

### Comparing `datafusion-26.0.0/src/expr/logical_node.rs` & `datafusion-27.0.0/src/expr/logical_node.rs`

 * *Files identical despite different names*

### Comparing `datafusion-26.0.0/src/expr/placeholder.rs` & `datafusion-27.0.0/src/expr/placeholder.rs`

 * *Files identical despite different names*

### Comparing `datafusion-26.0.0/src/expr/projection.rs` & `datafusion-27.0.0/src/expr/projection.rs`

 * *Files identical despite different names*

### Comparing `datafusion-26.0.0/src/expr/repartition.rs` & `datafusion-27.0.0/src/expr/repartition.rs`

 * *Files identical despite different names*

### Comparing `datafusion-26.0.0/src/expr/scalar_function.rs` & `datafusion-27.0.0/src/expr/scalar_function.rs`

 * *Files identical despite different names*

### Comparing `datafusion-26.0.0/src/expr/scalar_subquery.rs` & `datafusion-27.0.0/src/expr/scalar_subquery.rs`

 * *Files identical despite different names*

### Comparing `datafusion-26.0.0/src/expr/scalar_variable.rs` & `datafusion-27.0.0/src/expr/scalar_variable.rs`

 * *Files identical despite different names*

### Comparing `datafusion-26.0.0/src/expr/signature.rs` & `datafusion-27.0.0/src/expr/signature.rs`

 * *Files identical despite different names*

### Comparing `datafusion-26.0.0/src/expr/sort.rs` & `datafusion-27.0.0/src/expr/sort.rs`

 * *Files identical despite different names*

### Comparing `datafusion-26.0.0/src/expr/subquery_alias.rs` & `datafusion-27.0.0/src/expr/subquery_alias.rs`

 * *Files identical despite different names*

### Comparing `datafusion-26.0.0/src/expr/table_scan.rs` & `datafusion-27.0.0/src/expr/table_scan.rs`

 * *Files identical despite different names*

### Comparing `datafusion-26.0.0/src/expr/union.rs` & `datafusion-27.0.0/src/expr/union.rs`

 * *Files identical despite different names*

### Comparing `datafusion-26.0.0/src/expr.rs` & `datafusion-27.0.0/src/expr.rs`

 * *Files 2% similar despite different names*

```diff
@@ -149,14 +149,20 @@
     }
 
     /// Returns a full and complete string representation of this expression.
     fn canonical_name(&self) -> PyResult<String> {
         Ok(self.expr.canonical_name())
     }
 
+    /// Returns the name of the Expr variant.
+    /// Ex: 'IsNotNull', 'Literal', 'BinaryExpr', etc
+    fn variant_name(&self) -> PyResult<&str> {
+        Ok(self.expr.variant_name())
+    }
+
     fn __richcmp__(&self, other: PyExpr, op: CompareOp) -> PyExpr {
         let expr = match op {
             CompareOp::Lt => self.expr.clone().lt(other.expr),
             CompareOp::Le => self.expr.clone().lt_eq(other.expr),
             CompareOp::Eq => self.expr.clone().eq(other.expr),
             CompareOp::Ne => self.expr.clone().not_eq(other.expr),
             CompareOp::Gt => self.expr.clone().gt(other.expr),
@@ -298,15 +304,15 @@
     pub fn python_value(&self, py: Python) -> PyResult<PyObject> {
         match &self.expr {
             Expr::Literal(scalar_value) => Ok(match scalar_value {
                 ScalarValue::Null => todo!(),
                 ScalarValue::Boolean(v) => v.into_py(py),
                 ScalarValue::Float32(v) => v.into_py(py),
                 ScalarValue::Float64(v) => v.into_py(py),
-                ScalarValue::Decimal128(_, _, _) => todo!(),
+                ScalarValue::Decimal128(v, _, _) => v.into_py(py),
                 ScalarValue::Int8(v) => v.into_py(py),
                 ScalarValue::Int16(v) => v.into_py(py),
                 ScalarValue::Int32(v) => v.into_py(py),
                 ScalarValue::Int64(v) => v.into_py(py),
                 ScalarValue::UInt8(v) => v.into_py(py),
                 ScalarValue::UInt16(v) => v.into_py(py),
                 ScalarValue::UInt32(v) => v.into_py(py),
@@ -319,18 +325,18 @@
                 ScalarValue::List(_, _) => todo!(),
                 ScalarValue::Date32(v) => v.into_py(py),
                 ScalarValue::Date64(v) => v.into_py(py),
                 ScalarValue::Time32Second(v) => v.into_py(py),
                 ScalarValue::Time32Millisecond(v) => v.into_py(py),
                 ScalarValue::Time64Microsecond(v) => v.into_py(py),
                 ScalarValue::Time64Nanosecond(v) => v.into_py(py),
-                ScalarValue::TimestampSecond(_, _) => todo!(),
-                ScalarValue::TimestampMillisecond(_, _) => todo!(),
-                ScalarValue::TimestampMicrosecond(_, _) => todo!(),
-                ScalarValue::TimestampNanosecond(_, _) => todo!(),
+                ScalarValue::TimestampSecond(v, _) => v.into_py(py),
+                ScalarValue::TimestampMillisecond(v, _) => v.into_py(py),
+                ScalarValue::TimestampMicrosecond(v, _) => v.into_py(py),
+                ScalarValue::TimestampNanosecond(v, _) => v.into_py(py),
                 ScalarValue::IntervalYearMonth(v) => v.into_py(py),
                 ScalarValue::IntervalDayTime(v) => v.into_py(py),
                 ScalarValue::IntervalMonthDayNano(v) => v.into_py(py),
                 ScalarValue::Struct(_, _) => todo!(),
                 ScalarValue::Dictionary(_, _) => todo!(),
             }),
             _ => Err(py_type_err(format!(
```

### Comparing `datafusion-26.0.0/src/functions.rs` & `datafusion-27.0.0/src/functions.rs`

 * *Files identical despite different names*

### Comparing `datafusion-26.0.0/src/lib.rs` & `datafusion-27.0.0/src/lib.rs`

 * *Files identical despite different names*

### Comparing `datafusion-26.0.0/src/physical_plan.rs` & `datafusion-27.0.0/src/physical_plan.rs`

 * *Files 1% similar despite different names*

```diff
@@ -47,15 +47,15 @@
     pub fn display(&self) -> String {
         let d = displayable(self.plan.as_ref());
         format!("{}", d.one_line())
     }
 
     pub fn display_indent(&self) -> String {
         let d = displayable(self.plan.as_ref());
-        format!("{}", d.indent())
+        format!("{}", d.indent(false))
     }
 
     fn __repr__(&self) -> String {
         self.display_indent()
     }
 
     #[getter]
```

### Comparing `datafusion-26.0.0/src/pyarrow_filter_expression.rs` & `datafusion-27.0.0/src/pyarrow_filter_expression.rs`

 * *Files identical despite different names*

### Comparing `datafusion-26.0.0/src/record_batch.rs` & `datafusion-27.0.0/src/record_batch.rs`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 // software distributed under the License is distributed on an
 // "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 // KIND, either express or implied.  See the License for the
 // specific language governing permissions and limitations
 // under the License.
 
 use crate::utils::wait_for_future;
-use datafusion::arrow::pyarrow::PyArrowConvert;
+use datafusion::arrow::pyarrow::ToPyArrow;
 use datafusion::arrow::record_batch::RecordBatch;
 use datafusion::physical_plan::SendableRecordBatchStream;
 use futures::StreamExt;
 use pyo3::{pyclass, pymethods, PyObject, PyResult, Python};
 
 #[pyclass(name = "RecordBatch", module = "datafusion", subclass)]
 pub struct PyRecordBatch {
```

### Comparing `datafusion-26.0.0/src/sql/exceptions.rs` & `datafusion-27.0.0/src/sql/exceptions.rs`

 * *Files identical despite different names*

### Comparing `datafusion-26.0.0/src/sql/logical.rs` & `datafusion-27.0.0/src/sql/logical.rs`

 * *Files 4% similar despite different names*

```diff
@@ -24,14 +24,16 @@
 use crate::expr::empty_relation::PyEmptyRelation;
 use crate::expr::explain::PyExplain;
 use crate::expr::extension::PyExtension;
 use crate::expr::filter::PyFilter;
 use crate::expr::limit::PyLimit;
 use crate::expr::projection::PyProjection;
 use crate::expr::sort::PySort;
+use crate::expr::subquery::PySubquery;
+use crate::expr::subquery_alias::PySubqueryAlias;
 use crate::expr::table_scan::PyTableScan;
 use datafusion_expr::LogicalPlan;
 use pyo3::prelude::*;
 
 use crate::expr::logical_node::LogicalNode;
 
 #[pyclass(name = "LogicalPlan", module = "datafusion", subclass)]
@@ -52,27 +54,29 @@
         self.plan.clone()
     }
 }
 
 #[pymethods]
 impl PyLogicalPlan {
     /// Return the specific logical operator
-    fn to_variant(&self, py: Python) -> PyResult<PyObject> {
+    pub fn to_variant(&self, py: Python) -> PyResult<PyObject> {
         Python::with_gil(|_| match self.plan.as_ref() {
             LogicalPlan::Aggregate(plan) => PyAggregate::from(plan.clone()).to_variant(py),
             LogicalPlan::Analyze(plan) => PyAnalyze::from(plan.clone()).to_variant(py),
             LogicalPlan::EmptyRelation(plan) => PyEmptyRelation::from(plan.clone()).to_variant(py),
             LogicalPlan::Explain(plan) => PyExplain::from(plan.clone()).to_variant(py),
             LogicalPlan::Extension(plan) => PyExtension::from(plan.clone()).to_variant(py),
             LogicalPlan::Distinct(plan) => PyDistinct::from(plan.clone()).to_variant(py),
             LogicalPlan::Filter(plan) => PyFilter::from(plan.clone()).to_variant(py),
             LogicalPlan::Limit(plan) => PyLimit::from(plan.clone()).to_variant(py),
             LogicalPlan::Projection(plan) => PyProjection::from(plan.clone()).to_variant(py),
             LogicalPlan::Sort(plan) => PySort::from(plan.clone()).to_variant(py),
             LogicalPlan::TableScan(plan) => PyTableScan::from(plan.clone()).to_variant(py),
+            LogicalPlan::Subquery(plan) => PySubquery::from(plan.clone()).to_variant(py),
+            LogicalPlan::SubqueryAlias(plan) => PySubqueryAlias::from(plan.clone()).to_variant(py),
             other => Err(py_unsupported_variant_err(format!(
                 "Cannot convert this plan to a LogicalNode: {:?}",
                 other
             ))),
         })
     }
```

### Comparing `datafusion-26.0.0/src/sql.rs` & `datafusion-27.0.0/src/sql.rs`

 * *Files identical despite different names*

### Comparing `datafusion-26.0.0/src/store.rs` & `datafusion-27.0.0/src/store.rs`

 * *Files identical despite different names*

### Comparing `datafusion-26.0.0/src/substrait.rs` & `datafusion-27.0.0/src/substrait.rs`

 * *Files identical despite different names*

### Comparing `datafusion-26.0.0/src/udaf.rs` & `datafusion-27.0.0/src/udaf.rs`

 * *Files 6% similar despite different names*

```diff
@@ -17,18 +17,18 @@
 
 use std::sync::Arc;
 
 use pyo3::{prelude::*, types::PyTuple};
 
 use datafusion::arrow::array::{Array, ArrayRef};
 use datafusion::arrow::datatypes::DataType;
-use datafusion::arrow::pyarrow::{PyArrowConvert, PyArrowType};
+use datafusion::arrow::pyarrow::{PyArrowType, ToPyArrow};
 use datafusion::common::ScalarValue;
 use datafusion::error::{DataFusionError, Result};
-use datafusion_expr::{create_udaf, Accumulator, AccumulatorFunctionImplementation, AggregateUDF};
+use datafusion_expr::{create_udaf, Accumulator, AccumulatorFactoryFunction, AggregateUDF};
 
 use crate::expr::PyExpr;
 use crate::utils::parse_volatility;
 
 #[derive(Debug)]
 struct RustAccumulator {
     accum: PyObject,
@@ -91,15 +91,15 @@
     }
 
     fn size(&self) -> usize {
         std::mem::size_of_val(self)
     }
 }
 
-pub fn to_rust_accumulator(accum: PyObject) -> AccumulatorFunctionImplementation {
+pub fn to_rust_accumulator(accum: PyObject) -> AccumulatorFactoryFunction {
     Arc::new(move |_| -> Result<Box<dyn Accumulator>> {
         let accum = Python::with_gil(|py| {
             accum
                 .call0(py)
                 .map_err(|e| DataFusionError::Execution(format!("{e}")))
         })?;
         Ok(Box::new(RustAccumulator::new(accum)))
```

### Comparing `datafusion-26.0.0/src/udf.rs` & `datafusion-27.0.0/src/udf.rs`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 use std::sync::Arc;
 
 use pyo3::{prelude::*, types::PyTuple};
 
 use datafusion::arrow::array::{make_array, Array, ArrayData, ArrayRef};
 use datafusion::arrow::datatypes::DataType;
-use datafusion::arrow::pyarrow::{PyArrowConvert, PyArrowType};
+use datafusion::arrow::pyarrow::{FromPyArrow, PyArrowType, ToPyArrow};
 use datafusion::error::DataFusionError;
 use datafusion::physical_plan::functions::make_scalar_function;
 use datafusion::physical_plan::udf::ScalarUDF;
 use datafusion_expr::create_udf;
 use datafusion_expr::function::ScalarFunctionImplementation;
 
 use crate::expr::PyExpr;
```

### Comparing `datafusion-26.0.0/src/utils.rs` & `datafusion-27.0.0/src/utils.rs`

 * *Files identical despite different names*

### Comparing `datafusion-26.0.0/Cargo.lock` & `datafusion-27.0.0/Cargo.lock`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,21 @@
 # This file is automatically @generated by Cargo.
 # It is not intended for manual editing.
 version = 3
 
 [[package]]
+name = "addr2line"
+version = "0.20.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "f4fa78e18c64fce05e902adecd7a5eed15a5e0a3439f7b0e169f0252214865e3"
+dependencies = [
+ "gimli",
+]
+
+[[package]]
 name = "adler"
 version = "1.0.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f26201604c87b1e01bd3d98f8d5d9a8fcbb815e8cedb41ffccbeb4bf593a35fe"
 
 [[package]]
 name = "adler32"
@@ -48,14 +57,20 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "94fb8275041c72129eb51b7d0322c29b8387a0386127718b096429201a5d6ece"
 dependencies = [
  "alloc-no-stdlib",
 ]
 
 [[package]]
+name = "allocator-api2"
+version = "0.2.15"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "56fc6cf8dc8c4158eed8649f9b8b0ea1518eb62b544fe9490d66fa0b349eafe9"
+
+[[package]]
 name = "android-tzdata"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e999941b234f3131b00bc13c22d06e8c5ff726d1b6318ac7eb276997bbb4fef0"
 
 [[package]]
 name = "android_system_properties"
@@ -87,39 +102,39 @@
  "num-bigint",
  "quad-rand",
  "rand",
  "regex",
  "serde",
  "serde_json",
  "snap",
- "strum",
- "strum_macros",
+ "strum 0.24.1",
+ "strum_macros 0.24.3",
  "thiserror",
  "typed-builder",
  "uuid",
  "zerocopy",
 ]
 
 [[package]]
 name = "arrayref"
 version = "0.3.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6b4930d2cb77ce62f89ee5d5289b4ac049559b1c45539271f5ed4fdc7db34545"
 
 [[package]]
 name = "arrayvec"
-version = "0.7.2"
+version = "0.7.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8da52d66c7071e2e3fa2a1e5c6d088fec47b593032b254f5e980de8ea54454d6"
+checksum = "96d30a06541fbafbc7f82ed10c06164cfbd2c401138f6addd8404629c4b16711"
 
 [[package]]
 name = "arrow"
-version = "40.0.0"
+version = "42.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6619cab21a0cdd8c9b9f1d9e09bfaa9b1974e5ef809a6566aef0b998caf38ace"
+checksum = "773d18d72cd290f3f9e2149a714c8ac404b6c3fd614c684f0015449940fca899"
 dependencies = [
  "ahash",
  "arrow-arith",
  "arrow-array",
  "arrow-buffer",
  "arrow-cast",
  "arrow-csv",
@@ -132,76 +147,77 @@
  "arrow-select",
  "arrow-string",
  "pyo3",
 ]
 
 [[package]]
 name = "arrow-arith"
-version = "40.0.0"
+version = "42.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e0dc95485623a76e00929bda8caa40c1f838190952365c4f43a7b9ae86d03e94"
+checksum = "93bc0da4b22ba63807fa2a74998e21209179c93c67856ae65d9218b81f3ef918"
 dependencies = [
  "arrow-array",
  "arrow-buffer",
  "arrow-data",
  "arrow-schema",
  "chrono",
  "half",
  "num",
 ]
 
 [[package]]
 name = "arrow-array"
-version = "40.0.0"
+version = "42.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3267847f53d3042473cfd2c769afd8d74a6d7d201fc3a34f5cb84c0282ef47a7"
+checksum = "ea9a0fd21121304cad96f307c938d861cb1e7f0c151b93047462cd9817d760fb"
 dependencies = [
  "ahash",
  "arrow-buffer",
  "arrow-data",
  "arrow-schema",
  "chrono",
  "chrono-tz",
  "half",
- "hashbrown 0.13.2",
+ "hashbrown 0.14.0",
  "num",
 ]
 
 [[package]]
 name = "arrow-buffer"
-version = "40.0.0"
+version = "42.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c5f66553e66e120ac4b21570368ee9ebf35ff3f5399f872b0667699e145678f5"
+checksum = "30ce342ecf5971004e23cef8b5fb3bacd2bbc48a381464144925074e1472e9eb"
 dependencies = [
  "half",
  "num",
 ]
 
 [[package]]
 name = "arrow-cast"
-version = "40.0.0"
+version = "42.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "65e6f3579dbf0d97c683d451b2550062b0f0e62a3169bf74238b5f59f44ad6d8"
+checksum = "4b94a0ce7d27abbb02e2ee4db770f593127610f57b32625b0bc6a1a90d65f085"
 dependencies = [
  "arrow-array",
  "arrow-buffer",
  "arrow-data",
  "arrow-schema",
  "arrow-select",
  "chrono",
  "comfy-table",
+ "half",
  "lexical-core",
  "num",
 ]
 
 [[package]]
 name = "arrow-csv"
-version = "40.0.0"
+version = "42.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "373579c4c1a8f5307d3125b7a89c700fcf8caf85821c77eb4baab3855ae0aba5"
+checksum = "0f3be10a00a43c4bf0d243c070754ebdde17c5d576b4928d9c3efbe3005a3853"
 dependencies = [
  "arrow-array",
  "arrow-buffer",
  "arrow-cast",
  "arrow-data",
  "arrow-schema",
  "chrono",
@@ -210,115 +226,115 @@
  "lazy_static",
  "lexical-core",
  "regex",
 ]
 
 [[package]]
 name = "arrow-data"
-version = "40.0.0"
+version = "42.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "61bc8df9912cca6642665fdf989d6fa0de2570f18a7f709bcf59d29de96d2097"
+checksum = "1d9a83dad6a53d6907765106d3bc61d6d9d313cfe1751701b3ef0948e7283dc2"
 dependencies = [
  "arrow-buffer",
  "arrow-schema",
  "half",
  "num",
 ]
 
 [[package]]
 name = "arrow-ipc"
-version = "40.0.0"
+version = "42.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0105dcf5f91daa7182d87b713ee0b32b3bfc88e0c48e7dc3e9d6f1277a07d1ae"
+checksum = "a46da5e438a854e0386b38774da88a98782c0973c6dbc5c949ca4e02faf9b016"
 dependencies = [
  "arrow-array",
  "arrow-buffer",
  "arrow-cast",
  "arrow-data",
  "arrow-schema",
  "flatbuffers",
 ]
 
 [[package]]
 name = "arrow-json"
-version = "40.0.0"
+version = "42.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e73134fb5b5ec8770f8cbb214c2c487b2d350081e403ca4eeeb6f8f5e19846ac"
+checksum = "d5f27a1fbc76553ad92dc1a9583e56b7058d8c418c4089b0b689f5b87e2da5e1"
 dependencies = [
  "arrow-array",
  "arrow-buffer",
  "arrow-cast",
  "arrow-data",
  "arrow-schema",
  "chrono",
  "half",
- "indexmap",
+ "indexmap 1.9.3",
  "lexical-core",
  "num",
  "serde",
  "serde_json",
 ]
 
 [[package]]
 name = "arrow-ord"
-version = "40.0.0"
+version = "42.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "89f25bc66e18d4c2aa1fe2f9bb03e2269da60e636213210385ae41a107f9965a"
+checksum = "f2373661f6c2233e18f6fa69c40999a9440231d1e8899be8bbbe73c7e24aa3b4"
 dependencies = [
  "arrow-array",
  "arrow-buffer",
  "arrow-data",
  "arrow-schema",
  "arrow-select",
  "half",
  "num",
 ]
 
 [[package]]
 name = "arrow-row"
-version = "40.0.0"
+version = "42.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1095ff85ea4f5ff02d17b30b089de31b51a50be01c6b674f0a0509ab771232f1"
+checksum = "377cd5158b7de4034a175e296726c40c3236e65d71d90a5dab2fb4fab526a8f4"
 dependencies = [
  "ahash",
  "arrow-array",
  "arrow-buffer",
  "arrow-data",
  "arrow-schema",
  "half",
- "hashbrown 0.13.2",
+ "hashbrown 0.14.0",
 ]
 
 [[package]]
 name = "arrow-schema"
-version = "40.0.0"
+version = "42.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "25187bbef474151a2e4ddec67b9e34bda5cbfba292dc571392fa3a1f71ff5a82"
+checksum = "ba9ed245bd2d7d97ad1457cb281d4296e8b593588758b8fec6d67b2b2b0f2265"
 dependencies = [
- "bitflags 2.3.1",
+ "bitflags 2.3.3",
 ]
 
 [[package]]
 name = "arrow-select"
-version = "40.0.0"
+version = "42.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fd0d4ee884aec3aa05e41478e3cd312bf609de9babb5d187a43fb45931da4da4"
+checksum = "0dc9bd6aebc565b1d04bae64a0f4dda3abc677190eb7d960471b1b20e1cebed0"
 dependencies = [
  "arrow-array",
  "arrow-buffer",
  "arrow-data",
  "arrow-schema",
  "num",
 ]
 
 [[package]]
 name = "arrow-string"
-version = "40.0.0"
+version = "42.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d6d71c3ffe4c07e66ce8fdc6aed5b00e0e60c5144911879b10546f5b72d8fa1c"
+checksum = "23cf2baea2ef53787332050decf7d71aca836a352e188c8ad062892405955d2b"
 dependencies = [
  "arrow-array",
  "arrow-buffer",
  "arrow-data",
  "arrow-schema",
  "arrow-select",
  "regex",
@@ -347,26 +363,26 @@
 name = "async-recursion"
 version = "1.0.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0e97ce7de6cf12de5d7226c73f5ba9811622f4db3a5b91b55c53e987e5f91cba"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.18",
+ "syn 2.0.22",
 ]
 
 [[package]]
 name = "async-trait"
 version = "0.1.68"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b9ccdd8f2a161be9bd5c023df56f1b2a0bd1d83872ae53b71a84a12c9bf6e842"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.18",
+ "syn 2.0.22",
 ]
 
 [[package]]
 name = "autocfg"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d468802bab17cbc0cc575e9b053f41e72aa36bfa6b7f55e3529ffa43161b97fa"
@@ -377,30 +393,45 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "aef8da1805e028a172334c3b680f93e71126f2327622faef2ec3d893c0a4ad77"
 dependencies = [
  "cc",
 ]
 
 [[package]]
+name = "backtrace"
+version = "0.3.68"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "4319208da049c43661739c5fade2ba182f09d1dc2299b32298d3a31692b17e12"
+dependencies = [
+ "addr2line",
+ "cc",
+ "cfg-if",
+ "libc",
+ "miniz_oxide",
+ "object",
+ "rustc-demangle",
+]
+
+[[package]]
 name = "base64"
 version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "604178f6c5c21f02dc555784810edfb88d34ac2c73b2eae109655649ee73ce3d"
 
 [[package]]
 name = "bitflags"
 version = "1.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bef38d45163c2f1dde094a7dfd33ccf595c92905c8f8f4fdc18d06fb1037718a"
 
 [[package]]
 name = "bitflags"
-version = "2.3.1"
+version = "2.3.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6776fc96284a0bb647b615056fc496d1fe1644a7ab01829818a6d91cae888b84"
+checksum = "630be753d4e58660abd17930c71b647fe46c27ea6b63cc59e1e3851406972e42"
 
 [[package]]
 name = "blake2"
 version = "0.10.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "46502ad458c9a52b69d4d4d32775c788b7a1b85e8bc9d482d92250fc0e3f8efe"
 dependencies = [
@@ -516,42 +547,42 @@
  "num-traits",
  "serde",
  "winapi",
 ]
 
 [[package]]
 name = "chrono-tz"
-version = "0.8.2"
+version = "0.8.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cf9cc2b23599e6d7479755f3594285efb3f74a1bdca7a7374948bc831e23a552"
+checksum = "f1369bc6b9e9a7dfdae2055f6ec151fe9c554a9d23d357c0237cee2e25eaabb7"
 dependencies = [
  "chrono",
  "chrono-tz-build",
  "phf",
 ]
 
 [[package]]
 name = "chrono-tz-build"
-version = "0.1.0"
+version = "0.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d9998fb9f7e9b2111641485bf8beb32f92945f97f92a3d061f744cfef335f751"
+checksum = "e2f5ebdc942f57ed96d560a6d1a459bae5851102a25d5bf89dc04ae453e31ecf"
 dependencies = [
  "parse-zoneinfo",
  "phf",
  "phf_codegen",
 ]
 
 [[package]]
 name = "comfy-table"
-version = "6.2.0"
+version = "7.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7e959d788268e3bf9d35ace83e81b124190378e4c91c9067524675e33394b8ba"
+checksum = "9ab77dbd8adecaf3f0db40581631b995f312a8a5ae3aa9993188bb8f23d83a5b"
 dependencies = [
- "strum",
- "strum_macros",
+ "strum 0.24.1",
+ "strum_macros 0.24.3",
  "unicode-width",
 ]
 
 [[package]]
 name = "const-random"
 version = "0.1.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -583,17 +614,17 @@
 name = "core-foundation-sys"
 version = "0.8.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e496a50fda8aacccc86d7529e2c1e0892dbd0f898a6b5645b5561b89c3210efa"
 
 [[package]]
 name = "cpufeatures"
-version = "0.2.7"
+version = "0.2.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3e4c1eaa2012c47becbbad2ab175484c2a84d1185b566fb2cc5b8707343dfe58"
+checksum = "03e69e28e9f7f77debdedbaafa2866e1de9ba56df55a8bd7cfc724c25a09987c"
 dependencies = [
  "libc",
 ]
 
 [[package]]
 name = "crc32fast"
 version = "1.3.2"
@@ -651,17 +682,17 @@
  "lock_api",
  "once_cell",
  "parking_lot_core",
 ]
 
 [[package]]
 name = "datafusion"
-version = "26.0.0"
+version = "27.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9992c267436551d40b52d65289b144712e7b0ebdc62c8c859fd1574e5f73efbb"
+checksum = "e96f6e4eb10bd3e6b709686858246466983e8c5354a928ff77ee34919aa60d00"
 dependencies = [
  "ahash",
  "apache-avro",
  "arrow",
  "arrow-array",
  "arrow-schema",
  "async-compression",
@@ -676,143 +707,142 @@
  "datafusion-optimizer",
  "datafusion-physical-expr",
  "datafusion-row",
  "datafusion-sql",
  "flate2",
  "futures",
  "glob",
- "hashbrown 0.13.2",
- "indexmap",
- "itertools",
+ "hashbrown 0.14.0",
+ "indexmap 1.9.3",
+ "itertools 0.11.0",
  "lazy_static",
  "log",
  "num-traits",
  "num_cpus",
  "object_store",
  "parking_lot",
  "parquet",
  "percent-encoding",
  "pin-project-lite",
  "rand",
  "smallvec",
  "sqlparser",
  "tempfile",
  "tokio",
- "tokio-stream",
  "tokio-util",
  "url",
  "uuid",
  "xz2",
  "zstd",
 ]
 
 [[package]]
 name = "datafusion-common"
-version = "26.0.0"
+version = "27.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c3be97f7a7c720cdbb71e9eeabf814fa6ad8102b9022390f6cac74d3b4af6392"
+checksum = "00e5fddcc0dd49bbe199e43aa406f39c46c790bb2a43c7b36a478e5f3f971235"
 dependencies = [
  "apache-avro",
  "arrow",
  "arrow-array",
  "chrono",
  "num_cpus",
  "object_store",
  "parquet",
  "pyo3",
  "sqlparser",
 ]
 
 [[package]]
 name = "datafusion-execution"
-version = "26.0.0"
+version = "27.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c77c4b14b809b0e4c5bb101b6834504f06cdbb0d3c643400c61d0d844b33264e"
+checksum = "cfd50b6cb17acc78d2473c0d28014b8fd4e2e0a2c067c07645d6547b33b0aeeb"
 dependencies = [
  "dashmap",
  "datafusion-common",
  "datafusion-expr",
- "hashbrown 0.13.2",
+ "hashbrown 0.14.0",
  "log",
  "object_store",
  "parking_lot",
  "rand",
  "tempfile",
  "url",
 ]
 
 [[package]]
 name = "datafusion-expr"
-version = "26.0.0"
+version = "27.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e6ec7409bd45cf4fae6395d7d1024c8a97e543cadc88363e405d2aad5330e5e7"
+checksum = "e1a35dc2cd9eac18063d636f7ddf4f090fe1f34284d80192ac7ade38cc3c6991"
 dependencies = [
  "ahash",
  "arrow",
  "datafusion-common",
  "lazy_static",
  "sqlparser",
- "strum",
- "strum_macros",
+ "strum 0.25.0",
+ "strum_macros 0.25.0",
 ]
 
 [[package]]
 name = "datafusion-optimizer"
-version = "26.0.0"
+version = "27.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "64b537c93f87989c212db92a448a0f5eb4f0995e27199bb7687ae94f8b64a7a8"
+checksum = "5f5043afeb45ec1c0f45519e1eed6a477f2d30732e8f975d9cf9a75fba0ca716"
 dependencies = [
  "arrow",
  "async-trait",
  "chrono",
  "datafusion-common",
  "datafusion-expr",
  "datafusion-physical-expr",
- "hashbrown 0.13.2",
- "itertools",
+ "hashbrown 0.14.0",
+ "itertools 0.11.0",
  "log",
  "regex-syntax",
 ]
 
 [[package]]
 name = "datafusion-physical-expr"
-version = "26.0.0"
+version = "27.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f60ee3f53340fdef36ee54d9e12d446ae2718b1d0196ac581f791d34808ec876"
+checksum = "6cc892a24f4b829ee7718ad3950884c0346dbdf1517f3df153af4bcf54d8ca4d"
 dependencies = [
  "ahash",
  "arrow",
  "arrow-array",
  "arrow-buffer",
  "arrow-schema",
  "blake2",
  "blake3",
  "chrono",
  "datafusion-common",
  "datafusion-expr",
  "datafusion-row",
  "half",
- "hashbrown 0.13.2",
- "indexmap",
- "itertools",
+ "hashbrown 0.14.0",
+ "indexmap 1.9.3",
+ "itertools 0.11.0",
  "lazy_static",
  "libc",
  "md-5",
  "paste",
  "petgraph",
  "rand",
  "regex",
  "sha2",
  "unicode-segmentation",
  "uuid",
 ]
 
 [[package]]
 name = "datafusion-python"
-version = "26.0.0"
+version = "27.0.0"
 dependencies = [
  "async-trait",
  "datafusion",
  "datafusion-common",
  "datafusion-expr",
  "datafusion-optimizer",
  "datafusion-sql",
@@ -823,56 +853,56 @@
  "parking_lot",
  "prost",
  "prost-types",
  "pyo3",
  "pyo3-build-config",
  "rand",
  "regex-syntax",
- "syn 2.0.18",
+ "syn 2.0.22",
  "tokio",
  "url",
  "uuid",
 ]
 
 [[package]]
 name = "datafusion-row"
-version = "26.0.0"
+version = "27.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d58fc64058aa3bcb00077a0d19474a0d584d31dec8c7ac3406868f485f659af9"
+checksum = "ce75c660bbddfdd254109e668e5b5bd69df31ea26e3768e15cef0c68015e650e"
 dependencies = [
  "arrow",
  "datafusion-common",
  "paste",
  "rand",
 ]
 
 [[package]]
 name = "datafusion-sql"
-version = "26.0.0"
+version = "27.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1531f0314151a34bf6c0a83c7261525688b7c729876f53e7896b8f4ca8f57d07"
+checksum = "49cab87e4933a452e0b7b3f0cbd0e760daf7d33fb54d09d70d3ffba229eaa652"
 dependencies = [
  "arrow",
  "arrow-schema",
  "datafusion-common",
  "datafusion-expr",
  "log",
  "sqlparser",
 ]
 
 [[package]]
 name = "datafusion-substrait"
-version = "26.0.0"
+version = "27.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "079d5be5ec59580777bfa16d79187fea99b6498e3e8e07eb36d504a5fe708f13"
+checksum = "ba77d22232053f6cdd98bd6f5328940850844450253f25b8c50bfc5199c505d4"
 dependencies = [
  "async-recursion",
  "chrono",
  "datafusion",
- "itertools",
+ "itertools 0.11.0",
  "object_store",
  "prost",
  "prost-types",
  "substrait",
  "tokio",
 ]
 
@@ -911,14 +941,20 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "071a31f4ee85403370b58aca746f01041ede6f0da2730960ad001edc2b71b394"
 dependencies = [
  "cfg-if",
 ]
 
 [[package]]
+name = "equivalent"
+version = "1.0.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "88bffebc5d80432c9b140ee17875ff173a8ab62faad5b257da912bd2f6c1c0a1"
+
+[[package]]
 name = "errno"
 version = "0.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4bcfec3a70f97c962c307b2d2c56e358cf1d00b558d74262b5f929ee8cc7e73a"
 dependencies = [
  "errno-dragonfly",
  "libc",
@@ -1037,15 +1073,15 @@
 name = "futures-macro"
 version = "0.3.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "89ca545a94061b6365f2c7355b4b32bd20df3ff95f02da9329b34ccc3bd6ee72"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.18",
+ "syn 2.0.22",
 ]
 
 [[package]]
 name = "futures-sink"
 version = "0.3.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f43be4fe21a13b9781a69afa4985b0f6ee0e1afab2c6f454a8cf30e2b2237b6e"
@@ -1092,14 +1128,20 @@
 dependencies = [
  "cfg-if",
  "libc",
  "wasi",
 ]
 
 [[package]]
+name = "gimli"
+version = "0.27.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b6c80984affa11d98d1b88b66ac8853f143217b399d3c74116778ff8fdb4ed2e"
+
+[[package]]
 name = "git2"
 version = "0.17.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7b989d6a7ca95a362cf2cfc5ad688b3a467be1f87e480b8dad07fee8c79b0044"
 dependencies = [
  "bitflags 1.3.2",
  "libc",
@@ -1112,37 +1154,38 @@
 name = "glob"
 version = "0.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d2fabcfbdc87f4758337ca535fb41a6d701b65693ce38287d856d1674551ec9b"
 
 [[package]]
 name = "h2"
-version = "0.3.19"
+version = "0.3.20"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d357c7ae988e7d2182f7d7871d0b963962420b0678b0997ce7de72001aeab782"
+checksum = "97ec8491ebaf99c8eaa73058b045fe58073cd6be7f596ac993ced0b0a0c01049"
 dependencies = [
  "bytes",
  "fnv",
  "futures-core",
  "futures-sink",
  "futures-util",
  "http",
- "indexmap",
+ "indexmap 1.9.3",
  "slab",
  "tokio",
  "tokio-util",
  "tracing",
 ]
 
 [[package]]
 name = "half"
-version = "2.2.1"
+version = "2.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "02b4af3693f1b705df946e9fe5631932443781d0aabb423b62fcd4d73f6d2fd0"
+checksum = "bc52e53916c08643f1b56ec082790d1e86a32e58dc5268f897f313fbae7b4872"
 dependencies = [
+ "cfg-if",
  "crunchy",
  "num-traits",
 ]
 
 [[package]]
 name = "hashbrown"
 version = "0.12.3"
@@ -1155,27 +1198,28 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "43a3c133739dddd0d2990f9a4bdf8eb4b21ef50e4851ca85ab661199821d510e"
 dependencies = [
  "ahash",
 ]
 
 [[package]]
-name = "heck"
-version = "0.4.1"
+name = "hashbrown"
+version = "0.14.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "95505c38b4572b2d910cecb0281560f54b440a19336cbbcb27bf6ce6adc6f5a8"
+checksum = "2c6201b9ff9fd90a5a3bac2e56a830d0caa509576f0e503818ee82c181b3437a"
+dependencies = [
+ "ahash",
+ "allocator-api2",
+]
 
 [[package]]
-name = "hermit-abi"
-version = "0.2.6"
+name = "heck"
+version = "0.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ee512640fe35acbfb4bb779db6f0d80704c2cacfa2e39b601ef3e3f47d1ae4c7"
-dependencies = [
- "libc",
-]
+checksum = "95505c38b4572b2d910cecb0281560f54b440a19336cbbcb27bf6ce6adc6f5a8"
 
 [[package]]
 name = "hermit-abi"
 version = "0.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fed44880c466736ef9a5c5b5facefb5ed0785676d0c02d612db14e54f0d84286"
 
@@ -1210,18 +1254,24 @@
 [[package]]
 name = "httpdate"
 version = "1.0.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c4a1e36c821dbe04574f602848a19f742f4fb3c98d40449f11bcad18d6b17421"
 
 [[package]]
+name = "humantime"
+version = "2.1.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "9a3a5bfb195931eeb336b2a7b4d761daec841b97f947d34394601737a7bba5e4"
+
+[[package]]
 name = "hyper"
-version = "0.14.26"
+version = "0.14.27"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ab302d72a6f11a3b910431ff93aae7e773078c769f0a3ef15fb9ec692ed147d4"
+checksum = "ffb1cfd654a8219eaef89881fdb3bb3b1cdc5fa75ded05d6933b2b382e395468"
 dependencies = [
  "bytes",
  "futures-channel",
  "futures-core",
  "futures-util",
  "h2",
  "http",
@@ -1290,14 +1340,24 @@
 checksum = "bd070e393353796e801d209ad339e89596eb4c8d430d18ede6a1cced8fafbd99"
 dependencies = [
  "autocfg",
  "hashbrown 0.12.3",
 ]
 
 [[package]]
+name = "indexmap"
+version = "2.0.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "d5477fe2230a79769d8dc68e0eabf5437907c0457a5614a9e8dddb67f65eb65d"
+dependencies = [
+ "equivalent",
+ "hashbrown 0.14.0",
+]
+
+[[package]]
 name = "indoc"
 version = "1.0.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bfa799dd5ed20a7e349f3b4639aa80d74549c81716d9ec4f994c9b5815598306"
 
 [[package]]
 name = "instant"
@@ -1316,35 +1376,44 @@
 
 [[package]]
 name = "io-lifetimes"
 version = "1.0.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "eae7b9aee968036d54dce06cebaefd919e4472e753296daccd6d344e3e2df0c2"
 dependencies = [
- "hermit-abi 0.3.1",
+ "hermit-abi",
  "libc",
  "windows-sys",
 ]
 
 [[package]]
 name = "ipnet"
-version = "2.7.2"
+version = "2.8.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "12b6ee2129af8d4fb011108c73d99a1b83a85977f23b82460c0ae2e25bb4b57f"
+checksum = "28b29a3cd74f0f4598934efe3aeba42bae0eb4680554128851ebbecb02af14e6"
 
 [[package]]
 name = "itertools"
 version = "0.10.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b0fd2260e829bddf4cb6ea802289de2f86d6a7a690192fbe91b3f46e0f2c8473"
 dependencies = [
  "either",
 ]
 
 [[package]]
+name = "itertools"
+version = "0.11.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b1c173a5686ce8bfa551b3563d0c2170bf24ca44da99c7ca4bfdab5418c3fe57"
+dependencies = [
+ "either",
+]
+
+[[package]]
 name = "itoa"
 version = "1.0.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "453ad9f582a441959e5f0d088b02ce04cfe8d51a8eaf077f12ac6d3e94164ca6"
 
 [[package]]
 name = "jobserver"
@@ -1353,17 +1422,17 @@
 checksum = "936cfd212a0155903bcbc060e316fb6cc7cbf2e1907329391ebadc1fe0ce77c2"
 dependencies = [
  "libc",
 ]
 
 [[package]]
 name = "js-sys"
-version = "0.3.63"
+version = "0.3.64"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2f37a4a5928311ac501dee68b3c7613a1037d0edb30c8e5427bd832d55d1b790"
+checksum = "c5f195fe497f702db0f318b07fdd68edb16955aed830df8363d837542f8f935a"
 dependencies = [
  "wasm-bindgen",
 ]
 
 [[package]]
 name = "lazy_static"
 version = "1.4.0"
@@ -1432,17 +1501,17 @@
 dependencies = [
  "lexical-util",
  "static_assertions",
 ]
 
 [[package]]
 name = "libc"
-version = "0.2.146"
+version = "0.2.147"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f92be4933c13fd498862a9e02a3055f8a8d9c039ce33db97306fd5a6caa7f29b"
+checksum = "b4668fb0ea861c1df094127ac5f1da3409a82116a4ba74fca2e58ef927159bb3"
 
 [[package]]
 name = "libflate"
 version = "1.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5ff4ae71b685bbad2f2f391fe74f6b7659a34871c08b210fdc039e43bee07d18"
 dependencies = [
@@ -1566,17 +1635,17 @@
 name = "memchr"
 version = "2.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2dffe52ecf27772e601905b7522cb4ef790d2cc203488bbd0e2fe85fcb74566d"
 
 [[package]]
 name = "memoffset"
-version = "0.8.0"
+version = "0.9.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d61c719bcfbcf5d62b3a09efa6088de8c54bc0bfcd3ea7ae39fcc186108b8de1"
+checksum = "5a634b1c61a95585bd15607c6ab0c4e5b226e695ff2800ba0cdccddf208c406c"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "mimalloc"
 version = "0.1.37"
@@ -1693,34 +1762,45 @@
 dependencies = [
  "autocfg",
  "libm",
 ]
 
 [[package]]
 name = "num_cpus"
-version = "1.15.0"
+version = "1.16.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0fac9e2da13b5eb447a6ce3d392f23a29d8694bff781bf03a16cd9ac8697593b"
+checksum = "4161fcb6d602d4d2081af7c3a45852d875a03dd337a6bfdd6e06407b61342a43"
 dependencies = [
- "hermit-abi 0.2.6",
+ "hermit-abi",
  "libc",
 ]
 
 [[package]]
+name = "object"
+version = "0.31.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "8bda667d9f2b5051b8833f59f3bf748b28ef54f850f4fcb389a252aa383866d1"
+dependencies = [
+ "memchr",
+]
+
+[[package]]
 name = "object_store"
-version = "0.5.6"
+version = "0.6.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ec9cd6ca25e796a49fa242876d1c4de36a24a6da5258e9f0bc062dbf5e81c53b"
+checksum = "27c776db4f332b571958444982ff641d2531417a326ca368995073b639205d58"
 dependencies = [
  "async-trait",
  "base64",
  "bytes",
  "chrono",
  "futures",
- "itertools",
+ "humantime",
+ "hyper",
+ "itertools 0.10.5",
  "parking_lot",
  "percent-encoding",
  "quick-xml",
  "rand",
  "reqwest",
  "ring",
  "rustls-pemfile",
@@ -1769,17 +1849,17 @@
  "redox_syscall",
  "smallvec",
  "windows-targets",
 ]
 
 [[package]]
 name = "parquet"
-version = "40.0.0"
+version = "42.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d6a656fcc17e641657c955742c689732684e096f790ff30865d9f8dcc39f7c4a"
+checksum = "baab9c36b1c8300b81b4d577d306a0a733f9d34021363098d3548e37757ed6c8"
 dependencies = [
  "ahash",
  "arrow-array",
  "arrow-buffer",
  "arrow-cast",
  "arrow-data",
  "arrow-ipc",
@@ -1787,15 +1867,15 @@
  "arrow-select",
  "base64",
  "brotli",
  "bytes",
  "chrono",
  "flate2",
  "futures",
- "hashbrown 0.13.2",
+ "hashbrown 0.14.0",
  "lz4",
  "num",
  "num-bigint",
  "object_store",
  "paste",
  "seq-macro",
  "snap",
@@ -1829,51 +1909,51 @@
 [[package]]
 name = "petgraph"
 version = "0.6.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4dd7d28ee937e54fe3080c91faa1c3a46c06de6252988a7f4592ba2310ef22a4"
 dependencies = [
  "fixedbitset",
- "indexmap",
+ "indexmap 1.9.3",
 ]
 
 [[package]]
 name = "phf"
-version = "0.11.1"
+version = "0.11.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "928c6535de93548188ef63bb7c4036bd415cd8f36ad25af44b9789b2ee72a48c"
+checksum = "ade2d8b8f33c7333b51bcf0428d37e217e9f32192ae4772156f65063b8ce03dc"
 dependencies = [
  "phf_shared",
 ]
 
 [[package]]
 name = "phf_codegen"
-version = "0.11.1"
+version = "0.11.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a56ac890c5e3ca598bbdeaa99964edb5b0258a583a9eb6ef4e89fc85d9224770"
+checksum = "e8d39688d359e6b34654d328e262234662d16cc0f60ec8dcbe5e718709342a5a"
 dependencies = [
  "phf_generator",
  "phf_shared",
 ]
 
 [[package]]
 name = "phf_generator"
-version = "0.11.1"
+version = "0.11.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b1181c94580fa345f50f19d738aaa39c0ed30a600d95cb2d3e23f94266f14fbf"
+checksum = "48e4cc64c2ad9ebe670cb8fd69dd50ae301650392e81c05f9bfcb2d5bdbc24b0"
 dependencies = [
  "phf_shared",
  "rand",
 ]
 
 [[package]]
 name = "phf_shared"
-version = "0.11.1"
+version = "0.11.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e1fb5f6f826b772a8d4c0394209441e7d37cbbb967ae9c7e0e8134365c9ee676"
+checksum = "90fcb95eef784c2ac79119d1dd819e162b5da872ce6f3c3abe1e8ca1c082f72b"
 dependencies = [
  "siphasher",
 ]
 
 [[package]]
 name = "pin-project-lite"
 version = "0.2.9"
@@ -1896,33 +1976,33 @@
 name = "ppv-lite86"
 version = "0.2.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5b40af805b3121feab8a3c29f04d8ad262fa8e0561883e7653e024ae4479e6de"
 
 [[package]]
 name = "prettyplease"
-version = "0.2.6"
+version = "0.2.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3b69d39aab54d069e7f2fe8cb970493e7834601ca2d8c65fd7bbd183578080d1"
+checksum = "9825a04601d60621feed79c4e6b56d65db77cdca55cef43b46b0de1096d1c282"
 dependencies = [
  "proc-macro2",
- "syn 2.0.18",
+ "syn 2.0.22",
 ]
 
 [[package]]
 name = "proc-macro-hack"
 version = "0.5.20+deprecated"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "dc375e1527247fe1a97d8b7156678dfe7c1af2fc075c9a4db3690ecd2a148068"
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.60"
+version = "1.0.63"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dec2b086b7a862cf4de201096214fa870344cf922b2b30c167badb3af3195406"
+checksum = "7b368fba921b0dce7e60f5e04ec15e565b3303972b42bcfde1d0713b881959eb"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "prost"
 version = "0.11.9"
@@ -1937,15 +2017,15 @@
 name = "prost-build"
 version = "0.11.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "119533552c9a7ffacc21e099c24a0ac8bb19c2a2a3f363de84cd9b844feab270"
 dependencies = [
  "bytes",
  "heck",
- "itertools",
+ "itertools 0.10.5",
  "lazy_static",
  "log",
  "multimap",
  "petgraph",
  "prost",
  "prost-types",
  "regex",
@@ -1956,15 +2036,15 @@
 [[package]]
 name = "prost-derive"
 version = "0.11.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e5d2d8d10f3c6ded6da8b05b5fb3b8a5082514344d56c9f871412d29b4e075b4"
 dependencies = [
  "anyhow",
- "itertools",
+ "itertools 0.10.5",
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "prost-types"
@@ -1982,66 +2062,66 @@
 checksum = "c7ac8852baeb3cc6fb83b93646fb93c0ffe5d14bf138c945ceb4b9948ee0e3c1"
 dependencies = [
  "autotools",
 ]
 
 [[package]]
 name = "pyo3"
-version = "0.18.3"
+version = "0.19.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e3b1ac5b3731ba34fdaa9785f8d74d17448cd18f30cf19e0c7e7b1fdb5272109"
+checksum = "cffef52f74ec3b1a1baf295d9b8fcc3070327aefc39a6d00656b13c1d0b8885c"
 dependencies = [
  "cfg-if",
  "indoc",
  "libc",
  "memoffset",
  "parking_lot",
  "pyo3-build-config",
  "pyo3-ffi",
  "pyo3-macros",
  "unindent",
 ]
 
 [[package]]
 name = "pyo3-build-config"
-version = "0.18.3"
+version = "0.19.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9cb946f5ac61bb61a5014924910d936ebd2b23b705f7a4a3c40b05c720b079a3"
+checksum = "713eccf888fb05f1a96eb78c0dbc51907fee42b3377272dc902eb38985f418d5"
 dependencies = [
  "once_cell",
  "target-lexicon",
 ]
 
 [[package]]
 name = "pyo3-ffi"
-version = "0.18.3"
+version = "0.19.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fd4d7c5337821916ea2a1d21d1092e8443cf34879e53a0ac653fbb98f44ff65c"
+checksum = "5b2ecbdcfb01cbbf56e179ce969a048fd7305a66d4cdf3303e0da09d69afe4c3"
 dependencies = [
  "libc",
  "pyo3-build-config",
 ]
 
 [[package]]
 name = "pyo3-macros"
-version = "0.18.3"
+version = "0.19.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a9d39c55dab3fc5a4b25bbd1ac10a2da452c4aca13bb450f22818a002e29648d"
+checksum = "b78fdc0899f2ea781c463679b20cb08af9247febc8d052de941951024cd8aea0"
 dependencies = [
  "proc-macro2",
  "pyo3-macros-backend",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "pyo3-macros-backend"
-version = "0.18.3"
+version = "0.19.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "97daff08a4c48320587b5224cc98d609e3c27b6d437315bd40b605c98eeb5918"
+checksum = "60da7b84f1227c3e2fe7593505de274dcf4c8928b4e0a1c23d551a14e4e80a0f"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
@@ -2058,17 +2138,17 @@
 dependencies = [
  "memchr",
  "serde",
 ]
 
 [[package]]
 name = "quote"
-version = "1.0.28"
+version = "1.0.29"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1b9ab9c7eadfd8df19006f1cf1a4aed13540ed5cbc047010ece5826e10825488"
+checksum = "573015e8ab27661678357f27dc26460738fd2b6c86e46f386fde94cb5d913105"
 dependencies = [
  "proc-macro2",
 ]
 
 [[package]]
 name = "rand"
 version = "0.8.5"
@@ -2194,53 +2274,59 @@
 [[package]]
 name = "rle-decode-fast"
 version = "1.0.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3582f63211428f83597b51b2ddb88e2a91a9d52d12831f9d08f5e624e8977422"
 
 [[package]]
+name = "rustc-demangle"
+version = "0.1.23"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "d626bb9dae77e28219937af045c257c28bfd3f69333c512553507f5f9798cb76"
+
+[[package]]
 name = "rustc_version"
 version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bfa0f585226d2e68097d4f95d113b15b83a82e819ab25717ec0590d9584ef366"
 dependencies = [
  "semver",
 ]
 
 [[package]]
 name = "rustix"
-version = "0.37.20"
+version = "0.37.21"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b96e891d04aa506a6d1f318d2771bcb1c7dfda84e126660ace067c9b474bb2c0"
+checksum = "62f25693a73057a1b4cb56179dd3c7ea21a7c6c5ee7d85781f5749b46f34b79c"
 dependencies = [
  "bitflags 1.3.2",
  "errno",
  "io-lifetimes",
  "libc",
  "linux-raw-sys",
  "windows-sys",
 ]
 
 [[package]]
 name = "rustls"
-version = "0.21.1"
+version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c911ba11bc8433e811ce56fde130ccf32f5127cab0e0194e9c68c5a5b671791e"
+checksum = "e32ca28af694bc1bbf399c33a516dbdf1c90090b8ab23c2bc24f834aa2247f5f"
 dependencies = [
  "log",
  "ring",
  "rustls-webpki",
  "sct",
 ]
 
 [[package]]
 name = "rustls-pemfile"
-version = "1.0.2"
+version = "1.0.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d194b56d58803a43635bdc398cd17e383d6f71f9182b9a192c127ca42494a59b"
+checksum = "2d3987094b1d07b653b7dfdc3f70ce9a1da9c51ac18c1b06b662e4f9a0e9f4b2"
 dependencies = [
  "base64",
 ]
 
 [[package]]
 name = "rustls-webpki"
 version = "0.100.1"
@@ -2337,15 +2423,15 @@
 name = "serde_derive"
 version = "1.0.164"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d9735b638ccc51c28bf6914d90a2e9725b377144fc612c49a611fddd1b631d68"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.18",
+ "syn 2.0.22",
 ]
 
 [[package]]
 name = "serde_derive_internals"
 version = "0.26.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "85bf8229e7920a9f636479437026331ce11aa132b4dde37d121944a44d6e5f3c"
@@ -2353,17 +2439,17 @@
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "serde_json"
-version = "1.0.96"
+version = "1.0.99"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "057d394a50403bcac12672b2b18fb387ab6d289d957dab67dd201875391e52f1"
+checksum = "46266871c240a00b8f503b877622fe33430b3c7d963bdc0f2adc511e54a1eae3"
 dependencies = [
  "itoa",
  "ryu",
  "serde",
 ]
 
 [[package]]
@@ -2371,15 +2457,15 @@
 version = "0.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8a00ffd23fd882d096f09fcaae2a9de8329a328628e86027e049ee051dc1621f"
 dependencies = [
  "proc-macro2",
  "quote",
  "serde",
- "syn 2.0.18",
+ "syn 2.0.22",
 ]
 
 [[package]]
 name = "serde_urlencoded"
 version = "0.7.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d3491c14715ca2294c4d6a88f15e84739788c1d030eed8c110436aafdaa2f3fd"
@@ -2388,30 +2474,30 @@
  "itoa",
  "ryu",
  "serde",
 ]
 
 [[package]]
 name = "serde_yaml"
-version = "0.9.21"
+version = "0.9.22"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d9d684e3ec7de3bf5466b32bd75303ac16f0736426e5a4e0d6e489559ce1249c"
+checksum = "452e67b9c20c37fa79df53201dc03839651086ed9bbe92b3ca585ca9fdaa7d85"
 dependencies = [
- "indexmap",
+ "indexmap 2.0.0",
  "itoa",
  "ryu",
  "serde",
  "unsafe-libyaml",
 ]
 
 [[package]]
 name = "sha2"
-version = "0.10.6"
+version = "0.10.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "82e6b795fe2e3b1e845bafcb27aa35405c4d47cdfc92af5fc8d3002f76cebdc0"
+checksum = "479fb9d862239e610720565ca91403019f2f00410f1864c5aa7479b950a76ed8"
 dependencies = [
  "cfg-if",
  "cpufeatures",
  "digest",
 ]
 
 [[package]]
@@ -2477,17 +2563,17 @@
 name = "spin"
 version = "0.5.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6e63cff320ae2c57904679ba7cb63280a3dc4613885beafb148ee7bf9aa9042d"
 
 [[package]]
 name = "sqlparser"
-version = "0.34.0"
+version = "0.35.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "37d3706eefb17039056234df6b566b0014f303f867f2656108334a55b8096f59"
+checksum = "ca597d77c98894be1f965f2e4e2d2a61575d4998088e655476c73715c54b2b43"
 dependencies = [
  "log",
  "sqlparser_derive",
 ]
 
 [[package]]
 name = "sqlparser_derive"
@@ -2507,16 +2593,22 @@
 checksum = "a2eb9349b6444b326872e140eb1cf5e7c522154d69e7a0ffb0fb81c06b37543f"
 
 [[package]]
 name = "strum"
 version = "0.24.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "063e6045c0e62079840579a7e47a355ae92f60eb74daaf156fb1e84ba164e63f"
+
+[[package]]
+name = "strum"
+version = "0.25.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "290d54ea6f91c969195bdbcd7442c8c2a2ba87da8bf60a7ee86a235d4bc1e125"
 dependencies = [
- "strum_macros",
+ "strum_macros 0.25.0",
 ]
 
 [[package]]
 name = "strum_macros"
 version = "0.24.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1e385be0d24f186b4ce2f9982191e7101bb737312ad61c1f2f984f34bcf85d59"
@@ -2525,32 +2617,45 @@
  "proc-macro2",
  "quote",
  "rustversion",
  "syn 1.0.109",
 ]
 
 [[package]]
+name = "strum_macros"
+version = "0.25.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "fe9f3bd7d2e45dcc5e265fbb88d6513e4747d8ef9444cf01a533119bce28a157"
+dependencies = [
+ "heck",
+ "proc-macro2",
+ "quote",
+ "rustversion",
+ "syn 2.0.22",
+]
+
+[[package]]
 name = "substrait"
-version = "0.10.0"
+version = "0.11.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9df5d9e071804204172dc77e707c363f187e7f6566f9c78e5100c9a8f5ea434e"
+checksum = "7d3b77ddddd080d1bb5ebfe6b62d1c4e2f33c9f6a4586d5eac5306a08f3d4585"
 dependencies = [
  "git2",
  "heck",
  "prettyplease",
  "prost",
  "prost-build",
  "prost-types",
  "protobuf-src",
  "schemars",
  "semver",
  "serde",
  "serde_json",
  "serde_yaml",
- "syn 2.0.18",
+ "syn 2.0.22",
  "typify",
  "walkdir",
 ]
 
 [[package]]
 name = "subtle"
 version = "2.5.0"
@@ -2566,28 +2671,28 @@
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "syn"
-version = "2.0.18"
+version = "2.0.22"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "32d41677bcbe24c20c52e7c70b0d8db04134c5d1066bf98662e2871ad200ea3e"
+checksum = "2efbeae7acf4eabd6bcdcbd11c92f45231ddda7539edc7806bd1a04a03b24616"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "target-lexicon"
-version = "0.12.7"
+version = "0.12.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fd1ba337640d60c3e96bc6f0638a939b9c9a7f2c316a1598c279828b3d1dc8c5"
+checksum = "1b1c7f239eb94671427157bd93b3694320f3668d4e1eff08c7285366fd777fac"
 
 [[package]]
 name = "tempfile"
 version = "3.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "31c0432476357e58790aaa47a8efb0c5138f137343f3b5f23bd36a27e3b0a6d6"
 dependencies = [
@@ -2612,15 +2717,15 @@
 name = "thiserror-impl"
 version = "1.0.40"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f9456a42c5b0d803c8cd86e73dd7cc9edd429499f37a3550d286d5e86720569f"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.18",
+ "syn 2.0.22",
 ]
 
 [[package]]
 name = "thrift"
 version = "0.17.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7e54bc85fc7faa8bc175c4bab5b92ba8d9a3ce893d0e9f42cc455c8ab16a9e09"
@@ -2652,19 +2757,20 @@
 name = "tinyvec_macros"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1f3ccbac311fea05f86f61904b462b55fb3df8837a366dfc601a0161d0532f20"
 
 [[package]]
 name = "tokio"
-version = "1.28.2"
+version = "1.29.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "94d7b1cfd2aa4011f2de74c2c4c63665e27a71006b0a192dcd2710272e73dfa2"
+checksum = "532826ff75199d5833b9d2c5fe410f29235e25704ee5f0ef599fb51c21f4a4da"
 dependencies = [
  "autocfg",
+ "backtrace",
  "bytes",
  "libc",
  "mio",
  "num_cpus",
  "parking_lot",
  "pin-project-lite",
  "socket2",
@@ -2676,39 +2782,28 @@
 name = "tokio-macros"
 version = "2.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "630bdcf245f78637c13ec01ffae6187cca34625e8c63150d424b59e55af2675e"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.18",
+ "syn 2.0.22",
 ]
 
 [[package]]
 name = "tokio-rustls"
 version = "0.24.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c28327cf380ac148141087fbfb9de9d7bd4e84ab5d2c28fbc911d753de8a7081"
 dependencies = [
  "rustls",
  "tokio",
 ]
 
 [[package]]
-name = "tokio-stream"
-version = "0.1.14"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "397c988d37662c7dda6d2208364a706264bf3d6138b11d436cbac0ad38832842"
-dependencies = [
- "futures-core",
- "pin-project-lite",
- "tokio",
-]
-
-[[package]]
 name = "tokio-util"
 version = "0.7.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "806fe8c2c87eccc8b3267cbae29ed3ab2d0bd37fca70ab622e46aaa9375ddb7d"
 dependencies = [
  "bytes",
  "futures-core",
@@ -2734,21 +2829,21 @@
  "pin-project-lite",
  "tracing-attributes",
  "tracing-core",
 ]
 
 [[package]]
 name = "tracing-attributes"
-version = "0.1.24"
+version = "0.1.26"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0f57e3ca2a01450b1a921183a9c9cbfda207fd822cef4ccb00a65402cbba7a74"
+checksum = "5f4f31f56159e98206da9efd823404b79b6ef3143b4a7ab76e67b1751b25a4ab"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.18",
+ "syn 2.0.22",
 ]
 
 [[package]]
 name = "tracing-core"
 version = "0.1.31"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0955b8137a1df6f1a2e9a37d8a6656291ff0297c1a97c24e0d8425fe2312f79a"
@@ -2787,53 +2882,53 @@
 name = "typenum"
 version = "1.16.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "497961ef93d974e23eb6f433eb5fe1b7930b659f06d12dec6fc44a8f554c0bba"
 
 [[package]]
 name = "typify"
-version = "0.0.12"
+version = "0.0.13"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a6658d09e71bfe59e7987dc95ee7f71809fdb5793ab0cdc1503cc0073990484d"
+checksum = "be9bb640c0eece20cac2028ebbc2ca1a3d17e3b1ddd98540309c309ed178d158"
 dependencies = [
  "typify-impl",
  "typify-macro",
 ]
 
 [[package]]
 name = "typify-impl"
-version = "0.0.12"
+version = "0.0.13"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "34d3bb47587b13edf526d6ed02bf360ecefe083ab47a4ef29fc43112828b2bef"
+checksum = "5c8d9ecedde2fd77e975c38eeb9ca40b34ad0247b2259c6e6bbd2a8d6cc2444f"
 dependencies = [
  "heck",
  "log",
  "proc-macro2",
  "quote",
  "regress",
  "schemars",
  "serde_json",
- "syn 2.0.18",
+ "syn 2.0.22",
  "thiserror",
  "unicode-ident",
 ]
 
 [[package]]
 name = "typify-macro"
-version = "0.0.12"
+version = "0.0.13"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d3f7e627c18be12d53bc1f261830b9c2763437b6a86ac57293b9085af2d32ffe"
+checksum = "c08942cd65d458d2da15777a649cb6400cb545f17964f1ca965583f22e9cc3a9"
 dependencies = [
  "proc-macro2",
  "quote",
  "schemars",
  "serde",
  "serde_json",
  "serde_tokenstream",
- "syn 2.0.18",
+ "syn 2.0.22",
  "typify-impl",
 ]
 
 [[package]]
 name = "unicode-bidi"
 version = "0.3.13"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -2893,17 +2988,17 @@
  "form_urlencoded",
  "idna",
  "percent-encoding",
 ]
 
 [[package]]
 name = "uuid"
-version = "1.3.3"
+version = "1.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "345444e32442451b267fc254ae85a209c64be56d2890e601a0c37ff0c3c5ecd2"
+checksum = "d023da39d1fde5a8a3fe1f3e01ca9632ada0a63e9797de55a879d6e2236277be"
 dependencies = [
  "getrandom",
  "serde",
 ]
 
 [[package]]
 name = "vcpkg"
@@ -2925,93 +3020,92 @@
 dependencies = [
  "same-file",
  "winapi-util",
 ]
 
 [[package]]
 name = "want"
-version = "0.3.0"
+version = "0.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1ce8a968cb1cd110d136ff8b819a556d6fb6d919363c61534f6860c7eb172ba0"
+checksum = "bfa7760aed19e106de2c7c0b581b509f2f25d3dacaf737cb82ac61bc6d760b0e"
 dependencies = [
- "log",
  "try-lock",
 ]
 
 [[package]]
 name = "wasi"
 version = "0.11.0+wasi-snapshot-preview1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9c8d87e72b64a3b4db28d11ce29237c246188f4f51057d65a7eab63b7987e423"
 
 [[package]]
 name = "wasm-bindgen"
-version = "0.2.86"
+version = "0.2.87"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5bba0e8cb82ba49ff4e229459ff22a191bbe9a1cb3a341610c9c33efc27ddf73"
+checksum = "7706a72ab36d8cb1f80ffbf0e071533974a60d0a308d01a5d0375bf60499a342"
 dependencies = [
  "cfg-if",
  "wasm-bindgen-macro",
 ]
 
 [[package]]
 name = "wasm-bindgen-backend"
-version = "0.2.86"
+version = "0.2.87"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "19b04bc93f9d6bdee709f6bd2118f57dd6679cf1176a1af464fca3ab0d66d8fb"
+checksum = "5ef2b6d3c510e9625e5fe6f509ab07d66a760f0885d858736483c32ed7809abd"
 dependencies = [
  "bumpalo",
  "log",
  "once_cell",
  "proc-macro2",
  "quote",
- "syn 2.0.18",
+ "syn 2.0.22",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-futures"
-version = "0.4.36"
+version = "0.4.37"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2d1985d03709c53167ce907ff394f5316aa22cb4e12761295c5dc57dacb6297e"
+checksum = "c02dbc21516f9f1f04f187958890d7e6026df8d16540b7ad9492bc34a67cea03"
 dependencies = [
  "cfg-if",
  "js-sys",
  "wasm-bindgen",
  "web-sys",
 ]
 
 [[package]]
 name = "wasm-bindgen-macro"
-version = "0.2.86"
+version = "0.2.87"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "14d6b024f1a526bb0234f52840389927257beb670610081360e5a03c5df9c258"
+checksum = "dee495e55982a3bd48105a7b947fd2a9b4a8ae3010041b9e0faab3f9cd028f1d"
 dependencies = [
  "quote",
  "wasm-bindgen-macro-support",
 ]
 
 [[package]]
 name = "wasm-bindgen-macro-support"
-version = "0.2.86"
+version = "0.2.87"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e128beba882dd1eb6200e1dc92ae6c5dbaa4311aa7bb211ca035779e5efc39f8"
+checksum = "54681b18a46765f095758388f2d0cf16eb8d4169b639ab575a8f5693af210c7b"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.18",
+ "syn 2.0.22",
  "wasm-bindgen-backend",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-shared"
-version = "0.2.86"
+version = "0.2.87"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ed9d5b4305409d1fc9482fee2d7f9bcbf24b3972bf59817ef757e23982242a93"
+checksum = "ca6ad05a4870b2bf5fe995117d3728437bd27d7cd5f06f13c17443ef369775a1"
 
 [[package]]
 name = "wasm-streams"
 version = "0.2.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6bbae3363c08332cadccd13b67db371814cd214c2524020932f0804b8cf7c078"
 dependencies = [
@@ -3020,17 +3114,17 @@
  "wasm-bindgen",
  "wasm-bindgen-futures",
  "web-sys",
 ]
 
 [[package]]
 name = "web-sys"
-version = "0.3.63"
+version = "0.3.64"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3bdd9ef4e984da1187bf8110c5cf5b845fbc87a23602cdf912386a76fcd3a7c2"
+checksum = "9b85cbef8c220a6abc02aefd892dfc0fc23afb1c6a426316ec33253a3877249b"
 dependencies = [
  "js-sys",
  "wasm-bindgen",
 ]
 
 [[package]]
 name = "webpki"
@@ -3109,17 +3203,17 @@
 checksum = "677d2418bec65e3338edb076e806bc1ec15693c5d0104683f2efe857f61056a9"
 dependencies = [
  "windows-targets",
 ]
 
 [[package]]
 name = "windows-targets"
-version = "0.48.0"
+version = "0.48.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7b1eb6f0cd7c80c79759c929114ef071b87354ce476d9d94271031c0497adfd5"
+checksum = "05d4b17490f70499f20b9e791dcf6a299785ce8af4d709018206dc5b4953e95f"
 dependencies = [
  "windows_aarch64_gnullvm",
  "windows_aarch64_msvc",
  "windows_i686_gnu",
  "windows_i686_msvc",
  "windows_x86_64_gnu",
  "windows_x86_64_gnullvm",
```

### Comparing `datafusion-26.0.0/PKG-INFO` & `datafusion-27.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datafusion
-Version: 26.0.0
+Version: 27.0.0
 Requires-Dist: pyarrow >=11.0.0
 License-File: LICENSE.txt
 Summary: Build and run queries against data
 Keywords: datafusion,dataframe,rust,query-engine
 Home-Page: https://github.com/apache/arrow-datafusion-python
 Author: Apache Arrow <dev@arrow.apache.org>
 Author-email: Apache Arrow <dev@arrow.apache.org>
```

