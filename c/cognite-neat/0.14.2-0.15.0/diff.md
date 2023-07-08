# Comparing `tmp/cognite_neat-0.14.2.tar.gz` & `tmp/cognite_neat-0.15.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cognite_neat-0.14.2.tar", max compression
+gzip compressed data, was "cognite_neat-0.15.0.tar", max compression
```

## Comparing `cognite_neat-0.14.2.tar` & `cognite_neat-0.15.0.tar`

### file list

```diff
@@ -1,98 +1,98 @@
--rw-r--r--   0        0        0    11351 2023-07-07 11:11:16.038610 cognite_neat-0.14.2/LICENSE
--rw-r--r--   0        0        0     8765 2023-07-07 11:11:16.038610 cognite_neat-0.14.2/README.md
--rw-r--r--   0        0        0       23 2023-07-07 11:11:16.038610 cognite_neat-0.14.2/cognite/neat/__init__.py
--rw-r--r--   0        0        0     9922 2023-07-07 11:11:16.038610 cognite_neat-0.14.2/cognite/neat/base_workflows/graph2assets_relationships.py
--rw-r--r--   0        0        0     7016 2023-07-07 11:11:16.038610 cognite_neat-0.14.2/cognite/neat/base_workflows/graphs_and_rules.py
--rw-r--r--   0        0        0    14103 2023-07-07 11:11:16.038610 cognite_neat-0.14.2/cognite/neat/base_workflows/sheet2cdf.py
--rw-r--r--   0        0        0    11867 2023-07-07 11:11:16.038610 cognite_neat-0.14.2/cognite/neat/base_workflows/sme_graph_capture.py
--rw-r--r--   0        0        0      761 2023-07-07 11:11:16.038610 cognite_neat-0.14.2/cognite/neat/constants.py
--rw-r--r--   0        0        0        0 2023-07-07 11:11:16.038610 cognite_neat-0.14.2/cognite/neat/core/__init__.py
--rw-r--r--   0        0        0     2792 2023-07-07 11:11:16.038610 cognite_neat-0.14.2/cognite/neat/core/app.py
--rw-r--r--   0        0        0     1400 2023-07-07 11:11:16.038610 cognite_neat-0.14.2/cognite/neat/core/configuration.py
--rw-r--r--   0        0        0      408 2023-07-07 11:11:16.038610 cognite_neat-0.14.2/cognite/neat/core/data_classes/__init__.py
--rw-r--r--   0        0        0     5053 2023-07-07 11:11:16.038610 cognite_neat-0.14.2/cognite/neat/core/data_classes/config.py
--rw-r--r--   0        0        0     8132 2023-07-07 11:11:16.038610 cognite_neat-0.14.2/cognite/neat/core/data_classes/rules.py
--rw-r--r--   0        0        0    37631 2023-07-07 11:11:16.038610 cognite_neat-0.14.2/cognite/neat/core/data_classes/transformation_rules.py
--rw-r--r--   0        0        0        0 2023-07-07 11:11:16.038610 cognite_neat-0.14.2/cognite/neat/core/data_stores/__init__.py
--rw-r--r--   0        0        0     1520 2023-07-07 11:11:16.038610 cognite_neat-0.14.2/cognite/neat/core/data_stores/metrics.py
--rw-r--r--   0        0        0     9436 2023-07-07 11:11:16.038610 cognite_neat-0.14.2/cognite/neat/core/data_stores/oxrdflib.py
--rw-r--r--   0        0        0      646 2023-07-07 11:11:16.038610 cognite_neat-0.14.2/cognite/neat/core/extractors/__init__.py
--rw-r--r--   0        0        0     5449 2023-07-07 11:11:16.038610 cognite_neat-0.14.2/cognite/neat/core/extractors/graph_sheet_to_graph.py
--rw-r--r--   0        0        0     2250 2023-07-07 11:11:16.038610 cognite_neat-0.14.2/cognite/neat/core/extractors/labels.py
--rw-r--r--   0        0        0    39837 2023-07-07 11:11:16.042610 cognite_neat-0.14.2/cognite/neat/core/extractors/rdf_to_assets.py
--rw-r--r--   0        0        0    18682 2023-07-07 11:11:16.042610 cognite_neat-0.14.2/cognite/neat/core/extractors/rdf_to_relationships.py
--rw-r--r--   0        0        0     5400 2023-07-07 11:11:16.042610 cognite_neat-0.14.2/cognite/neat/core/extractors/rules_to_graph_capturing_sheet.py
--rw-r--r--   0        0        0     6698 2023-07-07 11:11:16.042610 cognite_neat-0.14.2/cognite/neat/core/extractors/rules_to_graphql.py
--rw-r--r--   0        0        0      138 2023-07-07 11:11:16.042610 cognite_neat-0.14.2/cognite/neat/core/loader/__init__.py
--rw-r--r--   0        0        0      711 2023-07-07 11:11:16.042610 cognite_neat-0.14.2/cognite/neat/core/loader/config.py
--rw-r--r--   0        0        0     1210 2023-07-07 11:11:16.042610 cognite_neat-0.14.2/cognite/neat/core/loader/graph.py
--rw-r--r--   0        0        0      938 2023-07-07 11:11:16.042610 cognite_neat-0.14.2/cognite/neat/core/loader/graph_capturing_sheet.py
--rw-r--r--   0        0        0    11439 2023-07-07 11:11:16.042610 cognite_neat-0.14.2/cognite/neat/core/loader/graph_store.py
--rw-r--r--   0        0        0     1009 2023-07-07 11:11:16.042610 cognite_neat-0.14.2/cognite/neat/core/loader/rules.py
--rw-r--r--   0        0        0        0 2023-07-07 11:11:16.042610 cognite_neat-0.14.2/cognite/neat/core/mocks/__init__.py
--rw-r--r--   0        0        0    10373 2023-07-07 11:11:16.042610 cognite_neat-0.14.2/cognite/neat/core/mocks/graph.py
--rw-r--r--   0        0        0    15269 2023-07-07 11:11:16.042610 cognite_neat-0.14.2/cognite/neat/core/modeler.py
--rw-r--r--   0        0        0      110 2023-07-07 11:11:16.042610 cognite_neat-0.14.2/cognite/neat/core/parser/__init__.py
--rw-r--r--   0        0        0     1958 2023-07-07 11:11:16.042610 cognite_neat-0.14.2/cognite/neat/core/parser/transformation_rules.py
--rw-r--r--   0        0        0       73 2023-07-07 11:11:16.042610 cognite_neat-0.14.2/cognite/neat/core/query_generator/__init__.py
--rw-r--r--   0        0        0     9595 2023-07-07 11:11:16.042610 cognite_neat-0.14.2/cognite/neat/core/query_generator/sparql.py
--rw-r--r--   0        0        0    11906 2023-07-07 11:11:16.042610 cognite_neat-0.14.2/cognite/neat/core/transformer.py
--rw-r--r--   0        0        0     8743 2023-07-07 11:11:16.042610 cognite_neat-0.14.2/cognite/neat/core/utils.py
--rw-r--r--   0        0        0     2559 2023-07-07 11:11:16.042610 cognite_neat-0.14.2/cognite/neat/core/validator.py
--rw-r--r--   0        0        0      311 2023-07-07 11:11:16.042610 cognite_neat-0.14.2/cognite/neat/core/workflow/__init__.py
--rw-r--r--   0        0        0    20731 2023-07-07 11:11:16.042610 cognite_neat-0.14.2/cognite/neat/core/workflow/base.py
--rw-r--r--   0        0        0    17764 2023-07-07 11:11:16.042610 cognite_neat-0.14.2/cognite/neat/core/workflow/cdf_store.py
--rw-r--r--   0        0        0    11637 2023-07-07 11:11:16.042610 cognite_neat-0.14.2/cognite/neat/core/workflow/manager.py
--rw-r--r--   0        0        0     4361 2023-07-07 11:11:16.042610 cognite_neat-0.14.2/cognite/neat/core/workflow/model.py
--rw-r--r--   0        0        0      775 2023-07-07 11:11:16.042610 cognite_neat-0.14.2/cognite/neat/core/workflow/tasks.py
--rw-r--r--   0        0        0     6977 2023-07-07 11:11:16.042610 cognite_neat-0.14.2/cognite/neat/core/workflow/triggers.py
--rw-r--r--   0        0        0      453 2023-07-07 11:11:16.042610 cognite_neat-0.14.2/cognite/neat/core/workflow/utils.py
--rw-r--r--   0        0        0      286 2023-07-07 11:11:16.042610 cognite_neat-0.14.2/cognite/neat/examples/data-models/power-grid-v0_1_0.graphql
--rw-r--r--   0        0        0    94607 2023-07-07 11:11:16.042610 cognite_neat-0.14.2/cognite/neat/examples/graph-sheets/sheet2cdf-graph-capturing.xlsx
--rw-r--r--   0        0        0    79716 2023-07-07 11:11:16.042610 cognite_neat-0.14.2/cognite/neat/examples/rules/Rules-Nordic44-to-TNT.xlsx
--rw-r--r--   0        0        0    77438 2023-07-07 11:11:16.042610 cognite_neat-0.14.2/cognite/neat/examples/rules/power-grid-example.xlsx
--rw-r--r--   0        0        0    75865 2023-07-07 11:11:16.046610 cognite_neat-0.14.2/cognite/neat/examples/rules/rules-template.xlsx
--rw-r--r--   0        0        0    52178 2023-07-07 11:11:16.046610 cognite_neat-0.14.2/cognite/neat/examples/rules/sheet2cdf-transformation-rules.xlsx
--rw-r--r--   0        0        0    79427 2023-07-07 11:11:16.046610 cognite_neat-0.14.2/cognite/neat/examples/rules/source-to-solution-mapping-rules.xlsx
--rw-r--r--   0        0        0  1437851 2023-07-07 11:11:16.050610 cognite_neat-0.14.2/cognite/neat/examples/source-graphs/Knowledge-Graph-Nordic44.xml
--rw-r--r--   0        0        0     1461 2023-07-07 11:11:16.050610 cognite_neat-0.14.2/cognite/neat/examples/workflows/basic/workflow.py
--rw-r--r--   0        0        0     1782 2023-07-07 11:11:16.050610 cognite_neat-0.14.2/cognite/neat/examples/workflows/basic/workflow.yaml
--rw-r--r--   0        0        0    15613 2023-07-07 11:11:16.050610 cognite_neat-0.14.2/cognite/neat/examples/workflows/default/workflow.py
--rw-r--r--   0        0        0     6774 2023-07-07 11:11:16.050610 cognite_neat-0.14.2/cognite/neat/examples/workflows/default/workflow.yaml
--rw-r--r--   0        0        0     3630 2023-07-07 11:11:16.050610 cognite_neat-0.14.2/cognite/neat/examples/workflows/fdm_schema_generation/workflow.py
--rw-r--r--   0        0        0     2573 2023-07-07 11:11:16.050610 cognite_neat-0.14.2/cognite/neat/examples/workflows/fdm_schema_generation/workflow.yaml
--rw-r--r--   0        0        0    11477 2023-07-07 11:11:16.050610 cognite_neat-0.14.2/cognite/neat/examples/workflows/graph_db_import/workflow.py
--rw-r--r--   0        0        0     4792 2023-07-07 11:11:16.050610 cognite_neat-0.14.2/cognite/neat/examples/workflows/graph_db_import/workflow.yaml
--rw-r--r--   0        0        0      315 2023-07-07 11:11:16.050610 cognite_neat-0.14.2/cognite/neat/examples/workflows/graph_to_asset_hierarchy/workflow.py
--rw-r--r--   0        0        0     8063 2023-07-07 11:11:16.050610 cognite_neat-0.14.2/cognite/neat/examples/workflows/graph_to_asset_hierarchy/workflow.yaml
--rw-r--r--   0        0        0      270 2023-07-07 11:11:16.050610 cognite_neat-0.14.2/cognite/neat/examples/workflows/sheet2cdf/workflow.py
--rw-r--r--   0        0        0     6668 2023-07-07 11:11:16.050610 cognite_neat-0.14.2/cognite/neat/examples/workflows/sheet2cdf/workflow.yaml
--rw-r--r--   0        0        0      291 2023-07-07 11:11:16.050610 cognite_neat-0.14.2/cognite/neat/examples/workflows/sme_graph_capture/workflow.py
--rw-r--r--   0        0        0     6837 2023-07-07 11:11:16.050610 cognite_neat-0.14.2/cognite/neat/examples/workflows/sme_graph_capture/workflow.yaml
--rw-r--r--   0        0        0        0 2023-07-07 11:11:16.098610 cognite_neat-0.14.2/cognite/neat/explorer/__init__.py
--rw-r--r--   0        0        0        0 2023-07-07 11:11:16.098610 cognite_neat-0.14.2/cognite/neat/explorer/data_classes/__init__.py
--rw-r--r--   0        0        0     1040 2023-07-07 11:11:16.098610 cognite_neat-0.14.2/cognite/neat/explorer/data_classes/rest.py
--rw-r--r--   0        0        0    23999 2023-07-07 11:11:16.098610 cognite_neat-0.14.2/cognite/neat/explorer/explorer.py
--rw-r--r--   0        0        0        0 2023-07-07 11:11:16.098610 cognite_neat-0.14.2/cognite/neat/explorer/utils/__init__.py
--rw-r--r--   0        0        0      412 2023-07-07 11:11:16.098610 cognite_neat-0.14.2/cognite/neat/explorer/utils/data_mapping.py
--rw-r--r--   0        0        0     4578 2023-07-07 11:11:16.098610 cognite_neat-0.14.2/cognite/neat/explorer/utils/query_templates.py
--rw-r--r--   0        0        0       16 2023-07-07 11:11:16.050610 cognite_neat-0.14.2/cognite/neat/explorer-ui/index.html
--rw-r--r--   0        0        0      312 2023-07-07 11:11:16.050610 cognite_neat-0.14.2/cognite/neat/explorer-ui/neat-app/.gitignore
--rw-r--r--   0        0        0     3359 2023-07-07 11:11:16.050610 cognite_neat-0.14.2/cognite/neat/explorer-ui/neat-app/README.md
--rw-r--r--   0        0        0      464 2023-07-07 11:11:16.050610 cognite_neat-0.14.2/cognite/neat/explorer-ui/neat-app/build/asset-manifest.json
--rw-r--r--   0        0        0     3870 2023-07-07 11:11:16.050610 cognite_neat-0.14.2/cognite/neat/explorer-ui/neat-app/build/favicon.ico
--rw-r--r--   0        0        0      630 2023-07-07 11:11:16.050610 cognite_neat-0.14.2/cognite/neat/explorer-ui/neat-app/build/index.html
--rw-r--r--   0        0        0     5347 2023-07-07 11:11:16.050610 cognite_neat-0.14.2/cognite/neat/explorer-ui/neat-app/build/logo192.png
--rw-r--r--   0        0        0      492 2023-07-07 11:11:16.050610 cognite_neat-0.14.2/cognite/neat/explorer-ui/neat-app/build/manifest.json
--rw-r--r--   0        0        0       67 2023-07-07 11:11:16.050610 cognite_neat-0.14.2/cognite/neat/explorer-ui/neat-app/build/robots.txt
--rw-r--r--   0        0        0     8524 2023-07-07 11:11:16.050610 cognite_neat-0.14.2/cognite/neat/explorer-ui/neat-app/build/static/css/main.38a62222.css
--rw-r--r--   0        0        0    13319 2023-07-07 11:11:16.050610 cognite_neat-0.14.2/cognite/neat/explorer-ui/neat-app/build/static/css/main.38a62222.css.map
--rw-r--r--   0        0        0  1370103 2023-07-07 11:11:16.058610 cognite_neat-0.14.2/cognite/neat/explorer-ui/neat-app/build/static/js/main.16555d84.js
--rw-r--r--   0        0        0     2667 2023-07-07 11:11:16.062610 cognite_neat-0.14.2/cognite/neat/explorer-ui/neat-app/build/static/js/main.16555d84.js.LICENSE.txt
--rw-r--r--   0        0        0  5883237 2023-07-07 11:11:16.094610 cognite_neat-0.14.2/cognite/neat/explorer-ui/neat-app/build/static/js/main.16555d84.js.map
--rw-r--r--   0        0        0     2633 2023-07-07 11:11:16.094610 cognite_neat-0.14.2/cognite/neat/explorer-ui/neat-app/build/static/media/logo.4bdbcf8396881de06a6723a92fed910b.svg
--rw-r--r--   0        0        0      358 2023-07-07 11:11:16.098610 cognite_neat-0.14.2/cognite/neat/main.py
--rw-r--r--   0        0        0        0 2023-07-07 11:11:16.098610 cognite_neat-0.14.2/cognite/neat/migration/__init__.py
--rw-r--r--   0        0        0     1581 2023-07-07 11:11:16.098610 cognite_neat-0.14.2/cognite/neat/migration/wf_manifests.py
--rw-r--r--   0        0        0     2577 2023-07-07 11:11:16.602612 cognite_neat-0.14.2/pyproject.toml
--rw-r--r--   0        0        0    10431 1970-01-01 00:00:00.000000 cognite_neat-0.14.2/PKG-INFO
+-rw-r--r--   0        0        0    11351 2023-07-08 16:11:35.912624 cognite_neat-0.15.0/LICENSE
+-rw-r--r--   0        0        0     8765 2023-07-08 16:11:35.912624 cognite_neat-0.15.0/README.md
+-rw-r--r--   0        0        0       23 2023-07-08 16:11:35.912624 cognite_neat-0.15.0/cognite/neat/__init__.py
+-rw-r--r--   0        0        0     9922 2023-07-08 16:11:35.912624 cognite_neat-0.15.0/cognite/neat/base_workflows/graph2assets_relationships.py
+-rw-r--r--   0        0        0     7016 2023-07-08 16:11:35.912624 cognite_neat-0.15.0/cognite/neat/base_workflows/graphs_and_rules.py
+-rw-r--r--   0        0        0    14129 2023-07-08 16:11:35.912624 cognite_neat-0.15.0/cognite/neat/base_workflows/sheet2cdf.py
+-rw-r--r--   0        0        0    11867 2023-07-08 16:11:35.912624 cognite_neat-0.15.0/cognite/neat/base_workflows/sme_graph_capture.py
+-rw-r--r--   0        0        0      761 2023-07-08 16:11:35.912624 cognite_neat-0.15.0/cognite/neat/constants.py
+-rw-r--r--   0        0        0        0 2023-07-08 16:11:35.912624 cognite_neat-0.15.0/cognite/neat/core/__init__.py
+-rw-r--r--   0        0        0     2792 2023-07-08 16:11:35.912624 cognite_neat-0.15.0/cognite/neat/core/app.py
+-rw-r--r--   0        0        0     1400 2023-07-08 16:11:35.912624 cognite_neat-0.15.0/cognite/neat/core/configuration.py
+-rw-r--r--   0        0        0      408 2023-07-08 16:11:35.912624 cognite_neat-0.15.0/cognite/neat/core/data_classes/__init__.py
+-rw-r--r--   0        0        0     5073 2023-07-08 16:11:35.912624 cognite_neat-0.15.0/cognite/neat/core/data_classes/config.py
+-rw-r--r--   0        0        0     8228 2023-07-08 16:11:35.912624 cognite_neat-0.15.0/cognite/neat/core/data_classes/rules.py
+-rw-r--r--   0        0        0    38635 2023-07-08 16:11:35.912624 cognite_neat-0.15.0/cognite/neat/core/data_classes/transformation_rules.py
+-rw-r--r--   0        0        0        0 2023-07-08 16:11:35.912624 cognite_neat-0.15.0/cognite/neat/core/data_stores/__init__.py
+-rw-r--r--   0        0        0     1520 2023-07-08 16:11:35.912624 cognite_neat-0.15.0/cognite/neat/core/data_stores/metrics.py
+-rw-r--r--   0        0        0     9436 2023-07-08 16:11:35.912624 cognite_neat-0.15.0/cognite/neat/core/data_stores/oxrdflib.py
+-rw-r--r--   0        0        0      646 2023-07-08 16:11:35.912624 cognite_neat-0.15.0/cognite/neat/core/extractors/__init__.py
+-rw-r--r--   0        0        0     5449 2023-07-08 16:11:35.912624 cognite_neat-0.15.0/cognite/neat/core/extractors/graph_sheet_to_graph.py
+-rw-r--r--   0        0        0     2250 2023-07-08 16:11:35.912624 cognite_neat-0.15.0/cognite/neat/core/extractors/labels.py
+-rw-r--r--   0        0        0    39837 2023-07-08 16:11:35.912624 cognite_neat-0.15.0/cognite/neat/core/extractors/rdf_to_assets.py
+-rw-r--r--   0        0        0    18682 2023-07-08 16:11:35.912624 cognite_neat-0.15.0/cognite/neat/core/extractors/rdf_to_relationships.py
+-rw-r--r--   0        0        0     5400 2023-07-08 16:11:35.912624 cognite_neat-0.15.0/cognite/neat/core/extractors/rules_to_graph_capturing_sheet.py
+-rw-r--r--   0        0        0     6698 2023-07-08 16:11:35.912624 cognite_neat-0.15.0/cognite/neat/core/extractors/rules_to_graphql.py
+-rw-r--r--   0        0        0      138 2023-07-08 16:11:35.912624 cognite_neat-0.15.0/cognite/neat/core/loader/__init__.py
+-rw-r--r--   0        0        0      711 2023-07-08 16:11:35.912624 cognite_neat-0.15.0/cognite/neat/core/loader/config.py
+-rw-r--r--   0        0        0     1210 2023-07-08 16:11:35.912624 cognite_neat-0.15.0/cognite/neat/core/loader/graph.py
+-rw-r--r--   0        0        0      938 2023-07-08 16:11:35.912624 cognite_neat-0.15.0/cognite/neat/core/loader/graph_capturing_sheet.py
+-rw-r--r--   0        0        0    11439 2023-07-08 16:11:35.912624 cognite_neat-0.15.0/cognite/neat/core/loader/graph_store.py
+-rw-r--r--   0        0        0     1009 2023-07-08 16:11:35.912624 cognite_neat-0.15.0/cognite/neat/core/loader/rules.py
+-rw-r--r--   0        0        0        0 2023-07-08 16:11:35.912624 cognite_neat-0.15.0/cognite/neat/core/mocks/__init__.py
+-rw-r--r--   0        0        0    10373 2023-07-08 16:11:35.912624 cognite_neat-0.15.0/cognite/neat/core/mocks/graph.py
+-rw-r--r--   0        0        0    15269 2023-07-08 16:11:35.912624 cognite_neat-0.15.0/cognite/neat/core/modeler.py
+-rw-r--r--   0        0        0      110 2023-07-08 16:11:35.912624 cognite_neat-0.15.0/cognite/neat/core/parser/__init__.py
+-rw-r--r--   0        0        0     1958 2023-07-08 16:11:35.912624 cognite_neat-0.15.0/cognite/neat/core/parser/transformation_rules.py
+-rw-r--r--   0        0        0       73 2023-07-08 16:11:35.912624 cognite_neat-0.15.0/cognite/neat/core/query_generator/__init__.py
+-rw-r--r--   0        0        0     9595 2023-07-08 16:11:35.912624 cognite_neat-0.15.0/cognite/neat/core/query_generator/sparql.py
+-rw-r--r--   0        0        0    11906 2023-07-08 16:11:35.912624 cognite_neat-0.15.0/cognite/neat/core/transformer.py
+-rw-r--r--   0        0        0     8743 2023-07-08 16:11:35.912624 cognite_neat-0.15.0/cognite/neat/core/utils.py
+-rw-r--r--   0        0        0     2559 2023-07-08 16:11:35.912624 cognite_neat-0.15.0/cognite/neat/core/validator.py
+-rw-r--r--   0        0        0      311 2023-07-08 16:11:35.912624 cognite_neat-0.15.0/cognite/neat/core/workflow/__init__.py
+-rw-r--r--   0        0        0    20765 2023-07-08 16:11:35.916624 cognite_neat-0.15.0/cognite/neat/core/workflow/base.py
+-rw-r--r--   0        0        0    17764 2023-07-08 16:11:35.916624 cognite_neat-0.15.0/cognite/neat/core/workflow/cdf_store.py
+-rw-r--r--   0        0        0    11636 2023-07-08 16:11:35.916624 cognite_neat-0.15.0/cognite/neat/core/workflow/manager.py
+-rw-r--r--   0        0        0     4882 2023-07-08 16:11:35.916624 cognite_neat-0.15.0/cognite/neat/core/workflow/model.py
+-rw-r--r--   0        0        0      775 2023-07-08 16:11:35.916624 cognite_neat-0.15.0/cognite/neat/core/workflow/tasks.py
+-rw-r--r--   0        0        0     6977 2023-07-08 16:11:35.916624 cognite_neat-0.15.0/cognite/neat/core/workflow/triggers.py
+-rw-r--r--   0        0        0      453 2023-07-08 16:11:35.916624 cognite_neat-0.15.0/cognite/neat/core/workflow/utils.py
+-rw-r--r--   0        0        0      286 2023-07-08 16:11:35.916624 cognite_neat-0.15.0/cognite/neat/examples/data-models/power-grid-v0_1_0.graphql
+-rw-r--r--   0        0        0    94607 2023-07-08 16:11:35.916624 cognite_neat-0.15.0/cognite/neat/examples/graph-sheets/sheet2cdf-graph-capturing.xlsx
+-rw-r--r--   0        0        0    79716 2023-07-08 16:11:35.916624 cognite_neat-0.15.0/cognite/neat/examples/rules/Rules-Nordic44-to-TNT.xlsx
+-rw-r--r--   0        0        0    77438 2023-07-08 16:11:35.916624 cognite_neat-0.15.0/cognite/neat/examples/rules/power-grid-example.xlsx
+-rw-r--r--   0        0        0    75865 2023-07-08 16:11:35.916624 cognite_neat-0.15.0/cognite/neat/examples/rules/rules-template.xlsx
+-rw-r--r--   0        0        0    52178 2023-07-08 16:11:35.916624 cognite_neat-0.15.0/cognite/neat/examples/rules/sheet2cdf-transformation-rules.xlsx
+-rw-r--r--   0        0        0    79427 2023-07-08 16:11:35.916624 cognite_neat-0.15.0/cognite/neat/examples/rules/source-to-solution-mapping-rules.xlsx
+-rw-r--r--   0        0        0  1437851 2023-07-08 16:11:35.920624 cognite_neat-0.15.0/cognite/neat/examples/source-graphs/Knowledge-Graph-Nordic44.xml
+-rw-r--r--   0        0        0     1461 2023-07-08 16:11:35.920624 cognite_neat-0.15.0/cognite/neat/examples/workflows/basic/workflow.py
+-rw-r--r--   0        0        0     1782 2023-07-08 16:11:35.920624 cognite_neat-0.15.0/cognite/neat/examples/workflows/basic/workflow.yaml
+-rw-r--r--   0        0        0    15613 2023-07-08 16:11:35.920624 cognite_neat-0.15.0/cognite/neat/examples/workflows/default/workflow.py
+-rw-r--r--   0        0        0     6774 2023-07-08 16:11:35.920624 cognite_neat-0.15.0/cognite/neat/examples/workflows/default/workflow.yaml
+-rw-r--r--   0        0        0     3630 2023-07-08 16:11:35.920624 cognite_neat-0.15.0/cognite/neat/examples/workflows/fdm_schema_generation/workflow.py
+-rw-r--r--   0        0        0     2573 2023-07-08 16:11:35.920624 cognite_neat-0.15.0/cognite/neat/examples/workflows/fdm_schema_generation/workflow.yaml
+-rw-r--r--   0        0        0    11477 2023-07-08 16:11:35.920624 cognite_neat-0.15.0/cognite/neat/examples/workflows/graph_db_import/workflow.py
+-rw-r--r--   0        0        0     4792 2023-07-08 16:11:35.920624 cognite_neat-0.15.0/cognite/neat/examples/workflows/graph_db_import/workflow.yaml
+-rw-r--r--   0        0        0      315 2023-07-08 16:11:35.920624 cognite_neat-0.15.0/cognite/neat/examples/workflows/graph_to_asset_hierarchy/workflow.py
+-rw-r--r--   0        0        0     8063 2023-07-08 16:11:35.920624 cognite_neat-0.15.0/cognite/neat/examples/workflows/graph_to_asset_hierarchy/workflow.yaml
+-rw-r--r--   0        0        0      270 2023-07-08 16:11:35.920624 cognite_neat-0.15.0/cognite/neat/examples/workflows/sheet2cdf/workflow.py
+-rw-r--r--   0        0        0     6668 2023-07-08 16:11:35.920624 cognite_neat-0.15.0/cognite/neat/examples/workflows/sheet2cdf/workflow.yaml
+-rw-r--r--   0        0        0      291 2023-07-08 16:11:35.920624 cognite_neat-0.15.0/cognite/neat/examples/workflows/sme_graph_capture/workflow.py
+-rw-r--r--   0        0        0     6837 2023-07-08 16:11:35.920624 cognite_neat-0.15.0/cognite/neat/examples/workflows/sme_graph_capture/workflow.yaml
+-rw-r--r--   0        0        0        0 2023-07-08 16:11:35.964625 cognite_neat-0.15.0/cognite/neat/explorer/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-08 16:11:35.964625 cognite_neat-0.15.0/cognite/neat/explorer/data_classes/__init__.py
+-rw-r--r--   0        0        0     1390 2023-07-08 16:11:35.964625 cognite_neat-0.15.0/cognite/neat/explorer/data_classes/rest.py
+-rw-r--r--   0        0        0    24055 2023-07-08 16:11:35.964625 cognite_neat-0.15.0/cognite/neat/explorer/explorer.py
+-rw-r--r--   0        0        0        0 2023-07-08 16:11:35.964625 cognite_neat-0.15.0/cognite/neat/explorer/utils/__init__.py
+-rw-r--r--   0        0        0      412 2023-07-08 16:11:35.964625 cognite_neat-0.15.0/cognite/neat/explorer/utils/data_mapping.py
+-rw-r--r--   0        0        0     4578 2023-07-08 16:11:35.964625 cognite_neat-0.15.0/cognite/neat/explorer/utils/query_templates.py
+-rw-r--r--   0        0        0       16 2023-07-08 16:11:35.920624 cognite_neat-0.15.0/cognite/neat/explorer-ui/index.html
+-rw-r--r--   0        0        0      312 2023-07-08 16:11:35.920624 cognite_neat-0.15.0/cognite/neat/explorer-ui/neat-app/.gitignore
+-rw-r--r--   0        0        0     3359 2023-07-08 16:11:35.920624 cognite_neat-0.15.0/cognite/neat/explorer-ui/neat-app/README.md
+-rw-r--r--   0        0        0      464 2023-07-08 16:11:35.920624 cognite_neat-0.15.0/cognite/neat/explorer-ui/neat-app/build/asset-manifest.json
+-rw-r--r--   0        0        0     3870 2023-07-08 16:11:35.920624 cognite_neat-0.15.0/cognite/neat/explorer-ui/neat-app/build/favicon.ico
+-rw-r--r--   0        0        0      630 2023-07-08 16:11:35.920624 cognite_neat-0.15.0/cognite/neat/explorer-ui/neat-app/build/index.html
+-rw-r--r--   0        0        0     5347 2023-07-08 16:11:35.920624 cognite_neat-0.15.0/cognite/neat/explorer-ui/neat-app/build/logo192.png
+-rw-r--r--   0        0        0      492 2023-07-08 16:11:35.920624 cognite_neat-0.15.0/cognite/neat/explorer-ui/neat-app/build/manifest.json
+-rw-r--r--   0        0        0       67 2023-07-08 16:11:35.920624 cognite_neat-0.15.0/cognite/neat/explorer-ui/neat-app/build/robots.txt
+-rw-r--r--   0        0        0     8524 2023-07-08 16:11:35.920624 cognite_neat-0.15.0/cognite/neat/explorer-ui/neat-app/build/static/css/main.38a62222.css
+-rw-r--r--   0        0        0    13319 2023-07-08 16:11:35.920624 cognite_neat-0.15.0/cognite/neat/explorer-ui/neat-app/build/static/css/main.38a62222.css.map
+-rw-r--r--   0        0        0  1370103 2023-07-08 16:11:35.928624 cognite_neat-0.15.0/cognite/neat/explorer-ui/neat-app/build/static/js/main.16555d84.js
+-rw-r--r--   0        0        0     2667 2023-07-08 16:11:35.928624 cognite_neat-0.15.0/cognite/neat/explorer-ui/neat-app/build/static/js/main.16555d84.js.LICENSE.txt
+-rw-r--r--   0        0        0  5883237 2023-07-08 16:11:35.960625 cognite_neat-0.15.0/cognite/neat/explorer-ui/neat-app/build/static/js/main.16555d84.js.map
+-rw-r--r--   0        0        0     2633 2023-07-08 16:11:35.960625 cognite_neat-0.15.0/cognite/neat/explorer-ui/neat-app/build/static/media/logo.4bdbcf8396881de06a6723a92fed910b.svg
+-rw-r--r--   0        0        0      358 2023-07-08 16:11:35.964625 cognite_neat-0.15.0/cognite/neat/main.py
+-rw-r--r--   0        0        0        0 2023-07-08 16:11:35.964625 cognite_neat-0.15.0/cognite/neat/migration/__init__.py
+-rw-r--r--   0        0        0     1581 2023-07-08 16:11:35.964625 cognite_neat-0.15.0/cognite/neat/migration/wf_manifests.py
+-rw-r--r--   0        0        0     2579 2023-07-08 16:11:36.428626 cognite_neat-0.15.0/pyproject.toml
+-rw-r--r--   0        0        0    10442 1970-01-01 00:00:00.000000 cognite_neat-0.15.0/PKG-INFO
```

### Comparing `cognite_neat-0.14.2/LICENSE` & `cognite_neat-0.15.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.14.2/README.md` & `cognite_neat-0.15.0/README.md`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.14.2/cognite/neat/base_workflows/graph2assets_relationships.py` & `cognite_neat-0.15.0/cognite/neat/base_workflows/graph2assets_relationships.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.14.2/cognite/neat/base_workflows/graphs_and_rules.py` & `cognite_neat-0.15.0/cognite/neat/base_workflows/graphs_and_rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.14.2/cognite/neat/base_workflows/sheet2cdf.py` & `cognite_neat-0.15.0/cognite/neat/base_workflows/sheet2cdf.py`

 * *Files 0% similar despite different names*

```diff
@@ -77,15 +77,15 @@
         output_text = f"Loaded {len(self.transformation_rules.properties)} rules from {rules_file_path.name!r}."
         logging.info(output_text)
         logging.info(f"Loaded prefixes {str(self.transformation_rules.prefixes)} rules")
 
         self.dataset_id = self.transformation_rules.metadata.data_set_id
         return FlowMessage(output_text=output_text)
 
-    def step_configuring_stores(self, flow_msg: FlowMessage = None):
+    def step_configuring_stores(self, flow_msg: FlowMessage = None, clean_start: bool = True):
         self.source_graph = loader.NeatGraphStore(
             prefixes=self.transformation_rules.prefixes, namespace=self.transformation_rules.metadata.namespace
         )
         self.source_graph.init_graph(base_prefix=self.transformation_rules.metadata.prefix)
 
         # this is fix to be able to display the graph in the UI
         # alex is working on a better solution
```

### Comparing `cognite_neat-0.14.2/cognite/neat/base_workflows/sme_graph_capture.py` & `cognite_neat-0.15.0/cognite/neat/base_workflows/sme_graph_capture.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.14.2/cognite/neat/constants.py` & `cognite_neat-0.15.0/cognite/neat/constants.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.14.2/cognite/neat/core/app.py` & `cognite_neat-0.15.0/cognite/neat/core/app.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.14.2/cognite/neat/core/configuration.py` & `cognite_neat-0.15.0/cognite/neat/core/configuration.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.14.2/cognite/neat/core/data_classes/config.py` & `cognite_neat-0.15.0/cognite/neat/core/data_classes/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import json
 import logging
 import os
 from enum import StrEnum
 from pathlib import Path
-from typing import Literal, Self
+from typing import Literal, Optional, Self
 
 import yaml
 from pydantic import BaseModel, Field, validator
 from yaml import safe_load
 
 LOG_FORMAT = "%(asctime)s.%(msecs)03d %(levelname)-8s %(message)s"
 LOG_DATE_FORMAT = "%Y-%m-%d %H:%M:%S"
@@ -79,15 +79,15 @@
     api_root_url: str = "http://localhost:7200"
 
 
 class Config(BaseModel):
     workflows_store_type: RulesStoreType = WorkflowsStoreType.FILE
     data_store_path: Path = Field(default_factory=lambda: Path.cwd() / "data")
 
-    workflow_downloader_filter: list[str] = Field(
+    workflow_downloader_filter: Optional[list[str]] = Field(
         description="List of workflow names+tags to filter on when downloading workflows from CDF. "
         "Example name:workflow_name=version,tag:tag_name",
         default=None,
     )
 
     cdf_client: InteractiveClient | ServiceClient = ServiceClient()
     cdf_default_dataset_id: int = 0
```

### Comparing `cognite_neat-0.14.2/cognite/neat/core/data_classes/rules.py` & `cognite_neat-0.15.0/cognite/neat/core/data_classes/rules.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 """
 import re
 from collections import Counter
 from dataclasses import dataclass
 from enum import StrEnum
 from typing import Literal, Optional, Self
 
-from pydantic import BaseModel, validator
+from pydantic import BaseModel, field_validator
 
 
 @dataclass
 class Triple:
     subject: str
     predicate: str
     object: str = None
@@ -112,15 +112,15 @@
 
 StepDirection = Literal["source", "target"]
 _direction_by_symbol = {"->": "target", "<-": "source"}
 
 
 class Step(BaseModel):
     class_: Entity
-    property: Optional[Entity]  # only terminal step has property
+    property: Optional[Entity] = None  # only terminal step has property
     direction: StepDirection
 
     @classmethod
     def from_string(cls, raw: str, **kwargs) -> Self:
         if result := _step_class_and_property.match(raw):
             return cls(
                 class_=Entity.from_string(result.group(OWL.class_)),
@@ -142,54 +142,54 @@
     pass
 
 
 class SingleProperty(Traversal):
     class_: Entity
     property: Entity
 
-    @validator("*", pre=True)
+    @field_validator("class_", "property", mode="before")
     def process_if_string(cls, value):
         return Entity.from_string(value) if isinstance(value, str) else value
 
 
 class AllReferences(Traversal):
     class_: Entity
 
-    @validator("class_", pre=True)
+    @field_validator("class_", mode="before")
     def process_if_string(cls, value):
         return Entity.from_string(value) if isinstance(value, str) else value
 
 
 class AllProperties(Traversal):
     class_: Entity
 
-    @validator("class_", pre=True)
+    @field_validator("class_", mode="before")
     def process_if_string(cls, value):
         return Entity.from_string(value) if isinstance(value, str) else value
 
 
 class Origin(BaseModel):
     class_: Entity
 
-    @validator("class_", pre=True)
+    @field_validator("class_", mode="before")
     def process_if_string(cls, value):
         return Entity.from_string(value) if isinstance(value, str) else value
 
 
 class Hop(Traversal):
     """Multi or single hop traversal through graph"""
 
     origin: Origin
     traversal: list[Step]
 
-    @validator("origin", pre=True)
+    @field_validator("origin", mode="before")
     def process_origin_if_string(cls, value):
         return Origin(class_=value) if isinstance(value, str) else value
 
-    @validator("traversal", pre=True)
+    @field_validator("traversal", mode="before")
     def process_path_if_string(cls, value):
         if isinstance(value, str):
             return [Step.from_string(result[0]) for result in _steps.findall(value)]
         return value
 
 
 class TableLookup(BaseModel):
```

### Comparing `cognite_neat-0.14.2/cognite/neat/core/data_classes/transformation_rules.py` & `cognite_neat-0.15.0/cognite/neat/core/data_classes/transformation_rules.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,19 +2,32 @@
 
 import logging
 import math
 import re
 import warnings
 from datetime import datetime
 from pathlib import Path
-from typing import Dict, List, Optional, Self, Union
+from typing import ClassVar, Dict, List, Optional, Self
 
 import pandas as pd
 from graphql import GraphQLBoolean, GraphQLFloat, GraphQLInt, GraphQLString
-from pydantic import BaseModel, Field, HttpUrl, ValidationError, constr, parse_obj_as, root_validator, validator
+from pydantic import (
+    BaseModel,
+    ConfigDict,
+    Field,
+    HttpUrl,
+    ValidationError,
+    constr,
+    field_validator,
+    model_validator,
+    parse_obj_as,
+    root_validator,
+    validator,
+)
+from pydantic.fields import FieldInfo
 from rdflib import XSD, Literal, Namespace, URIRef
 
 from cognite.neat.core.configuration import PREFIXES, Tables
 from cognite.neat.core.data_classes.rules import Entity, RuleType, parse_rule
 
 # mapping of XSD types to Python and GraphQL types
 DATA_TYPE_MAPPING = {
@@ -31,89 +44,98 @@
     "token": {"python": "str", "GraphQL": GraphQLString},
     # Graphql does not have a datetime type this is CDF specific
     "dateTime": {"python": "datetime", "GraphQL": "Timestamp"},
 }
 METADATA_VALUE_MAX_LENGTH = 5120
 
 
+def replace_nan_floats_with_default(values: dict, model_fields: dict[str, FieldInfo]) -> dict:
+    output = {}
+    for field_name, value in values.items():
+        is_nan_float = isinstance(value, float) and math.isnan(value)
+        if not is_nan_float:
+            output[field_name] = value
+            continue
+        if field_name in model_fields:
+            output[field_name] = model_fields[field_name].default
+        else:
+            # field_name may be an alias
+            source_name = next((name for name, field in model_fields.items() if field.alias == field_name), None)
+            if source_name:
+                output[field_name] = model_fields[source_name].default
+            else:
+                # Just pass it through if it is not an alias.
+                output[field_name] = value
+    return output
+
+
+class RuleModel(BaseModel):
+    model_config: ClassVar[ConfigDict] = ConfigDict(
+        populate_by_name=True, str_strip_whitespace=True, arbitrary_types_allowed=True, strict=False
+    )
+
+
 class URL(BaseModel):
     url: HttpUrl
 
 
 Description = constr(min_length=1, max_length=255)
 
 
-class Resource(BaseModel):
+class Resource(RuleModel):
     # Solution model
-    description: Description = Field(alias="Description", default=None)
+    description: Optional[Description] = Field(alias="Description", default=None)
 
     # Solution CDF resource, it is not needed when working with FDM, this is only for
     # Classic CDF data model
-    cdf_resource_type: str = Field(alias="Resource Type", default=None)
+    cdf_resource_type: Optional[str] = Field(alias="Resource Type", default=None)
 
     # Advance data modeling: Keeping track if Resource got deprecated or not
     deprecated: bool = Field(default=False)
     deprecation_date: Optional[datetime] = Field(alias="deprecationDate", default=None)
-    replaced_by: str = Field(alias="replacedBy", default=None)
+    replaced_by: Optional[str] = Field(alias="replacedBy", default=None)
 
     # Advance data modeling: Relation to existing resources for purpose of mapping
-    source: HttpUrl = Field(
+    source: Optional[HttpUrl] = Field(
         alias="Source", description="Source of information for given entity, e.g. CIM", default=None
     )
-    source_entity_name: str = Field(
+    source_entity_name: Optional[str] = Field(
         alias="Source Entity Name", description="Closest entity in source, e.g. Substation", default=None
     )
-    match_type: str = Field(
+    match_type: Optional[str] = Field(
         alias="Match Type", description="Type of match between source entity and one being defined", default=None
     )
-    comment: str = Field(alias="Comment", description="Comment about mapping", default=None)
-    issues: List[str] = Field(default=None, description="Storing list of pydantic validation issues")
-    valid: bool = Field(default=True, description="Indicates whether resource is valid or not")
-
-    @validator(
-        "deprecated",
-        "deprecation_date",
-        "replaced_by",
-        "source",
-        "source_entity_name",
-        "match_type",
-        "comment",
-        pre=True,
-    )
-    def replace_float_nan_with_default(cls, value, field):
-        if isinstance(value, float) and math.isnan(value):
-            return field.default
-        return value
-
-    class Config:
-        allow_population_by_field_name = True
-        anystr_strip_whitespace = True
+    comment: Optional[str] = Field(alias="Comment", description="Comment about mapping", default=None)
+    issues: Optional[List[str]] = Field(default=None, description="Storing list of pydantic validation issues")
+    valid: Optional[bool] = Field(default=True, description="Indicates whether resource is valid or not")
+
+    @model_validator(mode="before")
+    def replace_float_nan_with_default(cls, values: dict) -> dict:
+        return replace_nan_floats_with_default(values, cls.model_fields)
 
 
 class_id_compliance_regex = r"^([a-zA-Z]+[a-zA-Z0-9]+[._-]{0,1}[a-zA-Z0-9]+)+$"
 
 ExternalId = constr(min_length=1, max_length=255)
 
 
 class Class(Resource):
     class_id: ExternalId = Field(
         alias="Class",
     )
-    class_name: ExternalId = Field(alias="Name", default=None)
+    class_name: Optional[ExternalId] = Field(alias="Name", default=None)
     # Solution model
-    parent_class: ExternalId = Field(alias="Parent Class", default=None)
+    parent_class: Optional[ExternalId] = Field(alias="Parent Class", default=None)
 
     # Solution CDF resource
-    parent_asset: ExternalId = Field(alias="Parent Asset", default=None)
+    parent_asset: Optional[ExternalId] = Field(alias="Parent Asset", default=None)
 
-    @validator("parent_class", "parent_asset", pre=True)
-    def replace_float_nan_with_default(cls, value, field):
-        if isinstance(value, float) and math.isnan(value):
-            return field.default
-        return value
+    @model_validator(mode="before")
+    def replace_nan_floats_with_default(cls, values: dict) -> dict:
+        return replace_nan_floats_with_default(values, cls.model_fields)
 
     @validator("class_id", always=True)
     def is_class_id_compliant(cls, value):
         if not re.match(class_id_compliance_regex, value):
             raise ValueError(
                 f"Invalid class_id {value} in Class sheet, it must obey regex {class_id_compliance_regex} !"
             )
@@ -128,60 +150,45 @@
 property_id_compliance_regex = r"^(\*)|(([a-zA-Z]+[a-zA-Z0-9]+[._-]{0,1}[a-zA-Z0-9]+)+)$"
 
 
 class Property(Resource):
     # Solution model
     class_id: ExternalId = Field(alias="Class")
     property_id: ExternalId = Field(alias="Property")
-    property_name: ExternalId = Field(alias="Name", default=None)
+    property_name: Optional[ExternalId] = Field(alias="Name", default=None)
     expected_value_type: ExternalId = Field(alias="Type")
     min_count: Optional[int] = Field(alias="Min Count", default=0)
     max_count: Optional[int] = Field(alias="Max Count", default=None)
 
     # OWL property
     property_type: str = "DatatypeProperty"
 
     # Solution CDF resource
-    resource_type_property: List[str] = Field(alias="Resource Type Property", default=None)
+    resource_type_property: Optional[list[str]] = Field(alias="Resource Type Property", default=None)
     source_type: str = Field(alias="Relationship Source Type", default="Asset")
     target_type: str = Field(alias="Relationship Target Type", default="Asset")
-    label: str = Field(alias="Relationship Label", default=None)
-    relationship_external_id_rule: str = Field(alias="Relationship ExternalID Rule", default=None)
+    label: Optional[str] = Field(alias="Relationship Label", default=None)
+    relationship_external_id_rule: Optional[str] = Field(alias="Relationship ExternalID Rule", default=None)
 
     # Transformation rule (domain to solution)
     rule_type: RuleType = Field(alias="Rule Type", default=None)
-    rule: str = Field(alias="Rule", default=None)
+    rule: Optional[str] = Field(alias="Rule", default=None)
     skip_rule: bool = Field(alias="Skip", default=False)
 
     # Specialization of cdf_resource_type to allow definition of both
     # Asset and Relationship at the same time
     cdf_resource_type: list[str] = Field(alias="Resource Type", default=[])
 
     @property
     def is_raw_lookup(self) -> bool:
         return self.rule_type == RuleType.rawlookup
 
-    @validator(
-        "max_count",
-        "min_count",
-        "target_type",
-        "source_type",
-        "label",
-        "relationship_external_id_rule",
-        "resource_type_property",
-        "skip_rule",
-        "rule",
-        "rule_type",
-        "cdf_resource_type",
-        pre=True,
-    )
-    def replace_float_nan_with_default(cls, value, field):
-        if isinstance(value, float) and math.isnan(value):
-            return field.default
-        return value
+    @model_validator(mode="before")
+    def replace_float_nan_with_default(cls, values: dict) -> dict:
+        return replace_nan_floats_with_default(values, cls.model_fields)
 
     @validator("class_id", always=True)
     def is_class_id_compliant(cls, value):
         if not re.match(class_id_compliance_regex, value):
             raise ValueError(
                 f"Invalid class_id {value} in Property sheet, it must obey regex {class_id_compliance_regex} !"
             )
@@ -233,20 +240,20 @@
 
     @validator("label")
     def set_relationship_label(cls, value, values):
         if "Relationship" in values.get("cdf_resource_type") and not value:
             return values.get("property_id")
         return value
 
-    @validator("cdf_resource_type", pre=True)
-    def to_list_if_comma(cls, value, field):
+    @field_validator("cdf_resource_type", mode="before")
+    def to_list_if_comma(cls, value, info):
         if isinstance(value, str):
             if value:
                 return value.replace(", ", ",").split(",")
-            if field.default is None:
+            if cls.model_fields[info.field_name].default is None:
                 return None
         return value
 
     @validator("property_type", pre=True, always=True)
     def set_property_type(cls, value, values):
         if values["expected_value_type"] in DATA_TYPE_MAPPING.keys():
             return "DatatypeProperty"
@@ -267,31 +274,34 @@
 data_model_name_compliance_regex = r"^([a-zA-Z]+[a-zA-Z0-9]+[_]{0,1}[a-zA-Z0-9])+$"
 version_compliance_regex = r"^([0-9]+[_-]{1}[0-9]+[_-]{1}[0-9]+[_-]{1}[a-zA-Z0-9]+)|([0-9]+[_-]{1}[0-9]+[_-]{1}[0-9]+)|([0-9]+[_-]{1}[0-9])|([0-9]+)$"
 
 Prefix = constr(min_length=1, max_length=43)
 
 
 class Metadata(BaseModel):
+    model_config: ClassVar[ConfigDict] = ConfigDict(
+        populate_by_name=True, str_strip_whitespace=True, arbitrary_types_allowed=True
+    )
     prefix: Prefix = Field(
         alias="shortName",
         description="This is used as prefix for generation of RDF OWL/SHACL data model representation",
     )
     cdf_space_name: Prefix = Field(
         description="This is used as CDF space name to which model is intend to be stored. By default it is set to 'playground'",
         alias="cdfSpaceName",
         default="playground",
     )
 
-    namespace: Namespace = Field(
+    namespace: Optional[Namespace] = Field(
         description="This is used as RDF namespace for generation of RDF OWL/SHACL data model representation and/or for generation of RDF graphs",
         min_length=1,
         max_length=2048,
         default=None,
     )
-    data_model_name: ExternalId = Field(
+    data_model_name: Optional[ExternalId] = Field(
         description="Name that uniquely identifies data model",
         alias="dataModelName",
         default=None,
     )
 
     version: str = Field(
         min_length=1,
@@ -301,38 +311,38 @@
     created: datetime
     updated: datetime = Field(default_factory=lambda: datetime.utcnow())
     title: str = Field(min_length=1, max_length=255)
     description: Description
     creator: str | list[str]
     contributor: Optional[str | list[str]] = None
     rights: Optional[str] = "Restricted for Internal Use of Cognite"
-    externalIdPrefix: str = Field(alias="externalIdPrefix", default=None)
-    data_set_id: int = Field(alias="dataSetId", default=None)
-    imports: list[str] = Field(
+    externalIdPrefix: Optional[str] = Field(alias="externalIdPrefix", default=None)
+    data_set_id: Optional[int] = Field(alias="dataSetId", default=None)
+    imports: Optional[list[str]] = Field(
         description="Placeholder in case when data model is modular, i.e. provided as set of Excel files",
         default=None,
     )
-    source: str | Path = Field(
+    source: Optional[str | Path] = Field(
         description="File path to Excel file which was used to produce Transformation Rules",
         default=None,
     )
-    issues: List[str] = Field(default=None, description="Storing list of pydantic validation issues")
-    valid: bool = Field(default=True, description="Indicates whether resource is valid or not")
+    issues: Optional[List[str]] = Field(default=None, description="Storing list of pydantic validation issues")
+    valid: Optional[bool] = Field(default=True, description="Indicates whether resource is valid or not")
 
-    @validator(
+    @field_validator(
         "externalIdPrefix",
         "contributor",
         "contributor",
         "description",
         "rights",
-        pre=True,
+        mode="before",
     )
-    def replace_float_nan_with_default(cls, value, field):
+    def replace_float_nan_with_default(cls, value, info):
         if isinstance(value, float) and math.isnan(value):
-            return field.default
+            return cls.model_fields[info.field_name].default
         return value
 
     @validator("prefix", always=True)
     def make_prefix_compliant(cls, value):
         repaired_string = re.sub(r"[^-_a-zA-Z0-9]", "", value.replace(" ", "-"))
         if not re.match(prefix_compliance_regex, repaired_string):
             raise ValueError(
@@ -387,40 +397,36 @@
         if not re.match(version_compliance_regex, repaired_string):
             raise ValueError(
                 f"Invalid version {repaired_string} in Metadata sheet, it must obey regex {version_compliance_regex} !"
             )
         else:
             return repaired_string
 
-    @validator("creator", "contributor")
-    def to_list_if_comma(cls, value, field):
+    @field_validator("creator", "contributor", mode="before")
+    def to_list_if_comma(cls, value, info):
         if isinstance(value, str):
             if value:
                 return value.replace(", ", ",").split(",")
-            if field.default is None:
+            if cls.model_fields[info.field_name].default is None:
                 return None
         return value
 
-    class Config:
-        allow_population_by_field_name = True
-        anystr_strip_whitespace = True
-
     @classmethod
     def create_from_dataframe(cls, raw_dfs) -> Self:
         expected_tables = Tables.as_set()
         if missing_tables := (expected_tables - set(raw_dfs)):
             raise ValueError(f"Missing the following tables {', '.join(missing_tables)}")
 
         return Metadata(
             **dict(zip(raw_dfs[Tables.metadata][0], raw_dfs[Tables.metadata][1])),
             source=raw_dfs[Tables.metadata].source if "source" in dir(raw_dfs[Tables.metadata]) else None,
         )
 
 
-class Prefixes(BaseModel):
+class Prefixes(RuleModel):
     prefixes: Dict[str, Namespace] = PREFIXES
 
     @staticmethod
     def create_from_dataframe(raw_dfs: pd.DataFrame) -> dict[str, Namespace]:
         prefixes = {}
         for i, row in raw_dfs.iterrows():
             try:
@@ -430,36 +436,36 @@
                 msg = f"Prefix <{row['Prefix']}> has invalid URL: <{row['URI']}> fix this in Prefixes sheet at the row {i + 2} in the rule file!"
                 logging.error(msg)
                 raise ValueError(msg) from e
 
         return prefixes
 
 
-class Instance(BaseModel):
+class Instance(RuleModel):
     """Class deals with instances of classes in the data model"""
 
-    instance: URIRef = Field(alias="Instance", default=None)
-    property_: URIRef = Field(alias="Property", default=None)
-    value: Union[Literal, URIRef] = Field(alias="Value", default=None)
-    namespace: URIRef
+    instance: Optional[URIRef] = Field(alias="Instance", default=None)
+    property_: Optional[URIRef] = Field(alias="Property", default=None)
+    value: Optional[Literal | URIRef] = Field(alias="Value", default=None)
+    namespace: Namespace
     prefixes: Dict[str, Namespace]
 
     @staticmethod
     def get_value(value, prefixes) -> URIRef | Literal:
         try:
             url = URL(url=value).url
             return URIRef(url)
         except ValidationError:
             try:
                 entity = Entity.from_string(value)
                 return URIRef(prefixes[entity.prefix][entity.name])
             except ValueError:
                 return value
 
-    @root_validator(pre=True)
+    @model_validator(mode="before")
     def convert_values(cls, values: dict):
         # we expect to read Excel sheet which contains naming convention of column
         # 'Instance', 'Property', 'Value', if that's not the case we should raise error
         if not {"Instance", "Property", "Value"}.issubset(set(values.keys())):
             raise TypeError("We only support inputs from the transformation rule Excel sheet!!!")
 
         namespace = values["namespace"]
@@ -515,20 +521,20 @@
             b = int(a)
         except (TypeError, ValueError):
             return False
         else:
             return a == b
 
 
-class TransformationRules(BaseModel):
+class TransformationRules(RuleModel):
     metadata: Metadata
     classes: dict[str, Class]
     properties: dict[str, Property]
     prefixes: dict[str, Namespace]
-    instances: list[tuple] = None
+    instances: Optional[list[tuple]] = None
 
     @property
     def raw_tables(self) -> list[str]:
         return list(
             {
                 parse_rule(rule.rule, RuleType.rawlookup).table.name
                 for rule in self.properties.values()
@@ -836,16 +842,16 @@
             property_names = property_names.union(set(properties.index))
         return class_names.union(property_names)
 
 
 class AssetClassMapping(BaseModel):
     external_id: str
     name: str
-    parent_external_id: Optional[str]
-    description: Optional[str]
+    parent_external_id: Optional[str] = None
+    description: Optional[str] = None
     metadata: Optional[dict] = {}
 
     @root_validator(pre=True)
     def create_metadata(cls, values: dict):
         fields = values.keys()
 
         # adding metadata key in case if it is missing
@@ -859,18 +865,18 @@
 
 class AssetTemplate(BaseModel):
     """This class is used to validate, repair and wrangle rdf asset dictionary according to the
     expected format of cognite sdk Asset dataclass."""
 
     external_id_prefix: Optional[str] = None  # convenience field to add prefix to external_ids
     external_id: str
-    name: Optional[str]
-    parent_external_id: Optional[str]
+    name: Optional[str] = None
+    parent_external_id: Optional[str] = None
     metadata: Optional[dict] = {}
-    description: Optional[str]
+    description: Optional[str] = None
     data_set_id: Optional[int] = None
 
     @root_validator(pre=True)
     def preprocess_fields(cls, values: dict):
         fields = values.keys()
 
         # Adding metadata key in case if it is missing
@@ -946,15 +952,15 @@
 class RelationshipDefinition(BaseModel):
     source_class: str
     target_class: str
     property_: str
     labels: Optional[List[str]] = None
     target_type: str = "Asset"
     source_type: str = "Asset"
-    relationship_external_id_rule: str = None
+    relationship_external_id_rule: Optional[str] = None
 
 
-class RelationshipDefinitions(BaseModel):
+class RelationshipDefinitions(RuleModel):
     data_set_id: int
     prefix: str
     namespace: Namespace
     relationships: dict[str, RelationshipDefinition]
```

### Comparing `cognite_neat-0.14.2/cognite/neat/core/data_stores/metrics.py` & `cognite_neat-0.15.0/cognite/neat/core/data_stores/metrics.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.14.2/cognite/neat/core/data_stores/oxrdflib.py` & `cognite_neat-0.15.0/cognite/neat/core/data_stores/oxrdflib.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.14.2/cognite/neat/core/extractors/__init__.py` & `cognite_neat-0.15.0/cognite/neat/core/extractors/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.14.2/cognite/neat/core/extractors/graph_sheet_to_graph.py` & `cognite_neat-0.15.0/cognite/neat/core/extractors/graph_sheet_to_graph.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.14.2/cognite/neat/core/extractors/labels.py` & `cognite_neat-0.15.0/cognite/neat/core/extractors/labels.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.14.2/cognite/neat/core/extractors/rdf_to_assets.py` & `cognite_neat-0.15.0/cognite/neat/core/extractors/rdf_to_assets.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.14.2/cognite/neat/core/extractors/rdf_to_relationships.py` & `cognite_neat-0.15.0/cognite/neat/core/extractors/rdf_to_relationships.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.14.2/cognite/neat/core/extractors/rules_to_graph_capturing_sheet.py` & `cognite_neat-0.15.0/cognite/neat/core/extractors/rules_to_graph_capturing_sheet.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.14.2/cognite/neat/core/extractors/rules_to_graphql.py` & `cognite_neat-0.15.0/cognite/neat/core/extractors/rules_to_graphql.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.14.2/cognite/neat/core/loader/config.py` & `cognite_neat-0.15.0/cognite/neat/core/loader/config.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.14.2/cognite/neat/core/loader/graph.py` & `cognite_neat-0.15.0/cognite/neat/core/loader/graph.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.14.2/cognite/neat/core/loader/graph_capturing_sheet.py` & `cognite_neat-0.15.0/cognite/neat/core/loader/graph_capturing_sheet.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.14.2/cognite/neat/core/loader/graph_store.py` & `cognite_neat-0.15.0/cognite/neat/core/loader/graph_store.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.14.2/cognite/neat/core/loader/rules.py` & `cognite_neat-0.15.0/cognite/neat/core/loader/rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.14.2/cognite/neat/core/mocks/graph.py` & `cognite_neat-0.15.0/cognite/neat/core/mocks/graph.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.14.2/cognite/neat/core/modeler.py` & `cognite_neat-0.15.0/cognite/neat/core/modeler.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.14.2/cognite/neat/core/parser/transformation_rules.py` & `cognite_neat-0.15.0/cognite/neat/core/parser/transformation_rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.14.2/cognite/neat/core/query_generator/sparql.py` & `cognite_neat-0.15.0/cognite/neat/core/query_generator/sparql.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.14.2/cognite/neat/core/transformer.py` & `cognite_neat-0.15.0/cognite/neat/core/transformer.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.14.2/cognite/neat/core/utils.py` & `cognite_neat-0.15.0/cognite/neat/core/utils.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.14.2/cognite/neat/core/validator.py` & `cognite_neat-0.15.0/cognite/neat/core/validator.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.14.2/cognite/neat/core/workflow/base.py` & `cognite_neat-0.15.0/cognite/neat/core/workflow/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -396,24 +396,24 @@
             name=self.name,
             steps=self.workflow_steps,
             system_components=self.workflow_system_components,
             configs=self.configs,
             implementation_module=custom_implementation_module,
         )
         if output_format == "json":
-            return json.dumps(workflow_definitions.dict(), indent=4)
+            return json.dumps(workflow_definitions.model_dump(), indent=4)
         elif output_format == "yaml":
-            return yaml.dump(workflow_definitions.dict(), indent=4)
+            return yaml.dump(workflow_definitions.model_dump(), indent=4)
 
     @classmethod
     def deserialize_metadata(cls, json_string: str, output_format: str = "json") -> WorkflowDefinition:
         if output_format == "json":
-            workflow_definitions = WorkflowDefinition.parse_raw(json_string)
+            workflow_definitions = WorkflowDefinition.model_validate(json.loads(json_string))
         elif output_format == "yaml":
-            workflow_definitions = WorkflowDefinition.parse_obj(yaml.load(json_string, Loader=yaml.Loader))
+            workflow_definitions = WorkflowDefinition.model_validate(yaml.load(json_string, Loader=yaml.Loader))
         else:
             raise NotImplementedError(f"Output format {output_format} is not supported.")
         return workflow_definitions
 
     def set_metadata(self, metadata: WorkflowDefinition):
         self.workflow_steps = metadata.steps
         self.workflow_system_components = metadata.system_components
```

### Comparing `cognite_neat-0.14.2/cognite/neat/core/workflow/cdf_store.py` & `cognite_neat-0.15.0/cognite/neat/core/workflow/cdf_store.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.14.2/cognite/neat/core/workflow/manager.py` & `cognite_neat-0.15.0/cognite/neat/core/workflow/manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -93,15 +93,15 @@
                 f.write(
                     wf.serialize_workflow(
                         output_format="yaml", custom_implementation_module=custom_implementation_module
                     )
                 )
 
     def load_workflows_from_storage_v2(self, dir_path: str = None):
-        """Loads workflows from disk/storage into memory , initializes and register them in the workflow registry"""
+        """Loads workflows from disk/storage into memory, initializes and register them in the workflow registry"""
         if dir_path:
             dir_path = Path(dir_path)
         else:
             dir_path = self.workflows_storage_path
         sys.path.append(str(dir_path))
         for wf_module_name in os.listdir(dir_path):
             wf_module_full_path = dir_path / wf_module_name
```

### Comparing `cognite_neat-0.14.2/cognite/neat/core/workflow/model.py` & `cognite_neat-0.15.0/cognite/neat/core/workflow/model.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-import typing
 from enum import StrEnum
+from typing import Any, Optional
 
-from pydantic import BaseModel
+from pydantic import BaseModel, field_validator
 
 
 class WorkflowState(StrEnum):
     CREATED = "CREATED"
     RUNNING = "RUNNING"
     RUNNING_WAITING = "RUNNING_WAITING"
     COMPLETED = "COMPLETED"
@@ -30,19 +30,21 @@
 class WorkflowStartException(Exception):
     pass
 
 
 class FlowMessage(BaseModel):
     """A message that can be sent between steps in a workflow.It's the only parameter step takes as input."""
 
-    payload: typing.Any = None  # The payload of the message
-    headers: dict[str, str] = None  # The headers of the message
-    output_text: str = None  # The output text of the step that is captured in the execution log
-    error_text: str = None  # The error text of the step that is captured in the execution log
-    next_step_ids: list[str] = None  # If set, the workflow will skip default route and go to the next step in the list
+    payload: Any = None  # The payload of the message
+    headers: Optional[dict[str, str]] = None  # The headers of the message
+    output_text: Optional[str] = None  # The output text of the step that is captured in the execution log
+    error_text: Optional[str] = None  # The error text of the step that is captured in the execution log
+    next_step_ids: Optional[
+        list[str]
+    ] = None  # If set, the workflow will skip default route and go to the next step in the list
     step_execution_status: StepExecutionStatus = StepExecutionStatus.UNKNOWN  # The status of the step execution
 
 
 class StepType(StrEnum):
     PYSTEP = "pystep"
     START_WORKFLOW_TASK_STEP = "start_workflow_task_step"  # Call a workflow from another workflow
     CONTAINER_TASK_STEP = "container_step"  # TODO: implement
@@ -56,56 +58,56 @@
 class UIConfig(BaseModel):
     pos_x: int = 0
     pos_y: int = 0
 
 
 class WorkflowConfigItem(BaseModel):
     name: str
-    value: str = None
-    label: str = None
-    type: str = None
+    value: Optional[str] = None
+    label: Optional[str] = None
+    type: Optional[str] = None
     required: bool = False
-    options: list[str] = None
-    group: str = None
+    options: Optional[list[str]] = None
+    group: Optional[str] = None
 
 
 class WorkflowStepDefinition(BaseModel):
     id: str
-    label: str = None
+    label: Optional[str] = None
     stype: str = StepType.PYSTEP
-    description: str = None
-    method: str = None
+    description: Optional[str] = None
+    method: Optional[str] = None
     enabled: bool = True
-    system_component_id: str = None
+    system_component_id: Optional[str] = None
     trigger: bool = False
-    transition_to: list[str] = None
+    transition_to: Optional[list[str]] = None
     ui_config: UIConfig = UIConfig()
-    params: dict[str, str] = None
+    params: Optional[dict[str, str]] = None
     max_retries: int = 0
     retry_delay: int = 3
 
 
 class WorkflowSystemComponent(BaseModel):
     # Container for steps
     id: str
     label: str
-    transition_to: list[str] = None
-    description: str = None
+    transition_to: Optional[list[str]] = None
+    description: Optional[str] = None
     ui_config: UIConfig = UIConfig()
 
 
 class WorkflowDefinition(BaseModel):
     """Workflow definition"""
 
     name: str
-    description: str = None
-    implementation_module: str = None
+    description: Optional[str] = None
+    implementation_module: Optional[str] = None
     steps: list[WorkflowStepDefinition]
-    system_components: list[WorkflowSystemComponent] = None
-    configs: list[WorkflowConfigItem] = None
+    system_components: Optional[list[WorkflowSystemComponent]] = None
+    configs: Optional[list[WorkflowConfigItem]] = None
 
     def get_config_item(self, name: str) -> WorkflowConfigItem:
         for config in self.configs:
             if config.name == name:
                 return config
         return None
 
@@ -122,28 +124,34 @@
         self.configs.append(config_item)
 
 
 class WorkflowStepEvent(BaseModel):
     """Workflow step event represent a single step execution"""
 
     id: str
-    system_component_id: str = None
+    system_component_id: Optional[str] = None
     state: StepExecutionStatus
     elapsed_time: float
     timestamp: str
-    error: str = None
-    output_text: str = None
-    data: typing.Any = None
+    error: Optional[str] = None
+    output_text: Optional[str] = None
+    data: Any = None
 
 
 class WorkflowFullStateReport(BaseModel):
     """Workflow state report is complete log of workflow execution"""
 
-    workflow_name: str = None
-    workflow_version: str = None
-    run_id: str = None
+    workflow_name: Optional[str] = None
+    workflow_version: Optional[str] = None
+    run_id: Optional[str] = None
     state: WorkflowState
-    start_time: int = None
-    end_time: int = None
+    start_time: Optional[int] = None
+    end_time: Optional[int] = None
     elapsed_time: float = 0
-    last_error: str = None
+    last_error: Optional[str] = None
     execution_log: list[WorkflowStepEvent]
+
+    @field_validator("start_time", "end_time", mode="before")
+    def float_to_int(cls, value):
+        if isinstance(value, float):
+            return int(value)
+        return value
```

### Comparing `cognite_neat-0.14.2/cognite/neat/core/workflow/tasks.py` & `cognite_neat-0.15.0/cognite/neat/core/workflow/tasks.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.14.2/cognite/neat/core/workflow/triggers.py` & `cognite_neat-0.15.0/cognite/neat/core/workflow/triggers.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.14.2/cognite/neat/examples/graph-sheets/sheet2cdf-graph-capturing.xlsx` & `cognite_neat-0.15.0/cognite/neat/examples/graph-sheets/sheet2cdf-graph-capturing.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.14.2/cognite/neat/examples/rules/Rules-Nordic44-to-TNT.xlsx` & `cognite_neat-0.15.0/cognite/neat/examples/rules/Rules-Nordic44-to-TNT.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.14.2/cognite/neat/examples/rules/power-grid-example.xlsx` & `cognite_neat-0.15.0/cognite/neat/examples/rules/power-grid-example.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.14.2/cognite/neat/examples/rules/rules-template.xlsx` & `cognite_neat-0.15.0/cognite/neat/examples/rules/rules-template.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.14.2/cognite/neat/examples/rules/sheet2cdf-transformation-rules.xlsx` & `cognite_neat-0.15.0/cognite/neat/examples/rules/sheet2cdf-transformation-rules.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.14.2/cognite/neat/examples/rules/source-to-solution-mapping-rules.xlsx` & `cognite_neat-0.15.0/cognite/neat/examples/rules/source-to-solution-mapping-rules.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.14.2/cognite/neat/examples/source-graphs/Knowledge-Graph-Nordic44.xml` & `cognite_neat-0.15.0/cognite/neat/examples/source-graphs/Knowledge-Graph-Nordic44.xml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.14.2/cognite/neat/examples/workflows/basic/workflow.py` & `cognite_neat-0.15.0/cognite/neat/examples/workflows/basic/workflow.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.14.2/cognite/neat/examples/workflows/basic/workflow.yaml` & `cognite_neat-0.15.0/cognite/neat/examples/workflows/basic/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.14.2/cognite/neat/examples/workflows/default/workflow.py` & `cognite_neat-0.15.0/cognite/neat/examples/workflows/default/workflow.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.14.2/cognite/neat/examples/workflows/default/workflow.yaml` & `cognite_neat-0.15.0/cognite/neat/examples/workflows/default/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.14.2/cognite/neat/examples/workflows/fdm_schema_generation/workflow.py` & `cognite_neat-0.15.0/cognite/neat/examples/workflows/fdm_schema_generation/workflow.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.14.2/cognite/neat/examples/workflows/fdm_schema_generation/workflow.yaml` & `cognite_neat-0.15.0/cognite/neat/examples/workflows/fdm_schema_generation/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.14.2/cognite/neat/examples/workflows/graph_db_import/workflow.py` & `cognite_neat-0.15.0/cognite/neat/examples/workflows/graph_db_import/workflow.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.14.2/cognite/neat/examples/workflows/graph_db_import/workflow.yaml` & `cognite_neat-0.15.0/cognite/neat/examples/workflows/graph_db_import/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.14.2/cognite/neat/examples/workflows/graph_to_asset_hierarchy/workflow.yaml` & `cognite_neat-0.15.0/cognite/neat/examples/workflows/graph_to_asset_hierarchy/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.14.2/cognite/neat/examples/workflows/sheet2cdf/workflow.yaml` & `cognite_neat-0.15.0/cognite/neat/examples/workflows/sheet2cdf/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.14.2/cognite/neat/examples/workflows/sme_graph_capture/workflow.yaml` & `cognite_neat-0.15.0/cognite/neat/examples/workflows/sme_graph_capture/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.14.2/cognite/neat/explorer/explorer.py` & `cognite_neat-0.15.0/cognite/neat/explorer/explorer.py`

 * *Files 1% similar despite different names*

```diff
@@ -470,14 +470,15 @@
     return {"result": result}
 
 
 @app.get("/api/workflow/stats/{workflow_name}", response_model=WorkflowFullStateReport)
 def get_workflow_stats(
     workflow_name: str,
 ) -> WorkflowFullStateReport:
+    logging.info("Hit the get_workflow_stats endpoint")
     workflow = neat_app.workflow_manager.get_workflow(workflow_name)
     return workflow.get_state()
 
 
 @app.get("/api/workflow/workflows")
 def get_workflows():
     return {"workflows": neat_app.workflow_manager.get_list_of_workflows()}
```

### Comparing `cognite_neat-0.14.2/cognite/neat/explorer/utils/query_templates.py` & `cognite_neat-0.15.0/cognite/neat/explorer/utils/query_templates.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.14.2/cognite/neat/explorer-ui/neat-app/README.md` & `cognite_neat-0.15.0/cognite/neat/explorer-ui/neat-app/README.md`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.14.2/cognite/neat/explorer-ui/neat-app/build/favicon.ico` & `cognite_neat-0.15.0/cognite/neat/explorer-ui/neat-app/build/favicon.ico`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.14.2/cognite/neat/explorer-ui/neat-app/build/index.html` & `cognite_neat-0.15.0/cognite/neat/explorer-ui/neat-app/build/index.html`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.14.2/cognite/neat/explorer-ui/neat-app/build/logo192.png` & `cognite_neat-0.15.0/cognite/neat/explorer-ui/neat-app/build/logo192.png`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.14.2/cognite/neat/explorer-ui/neat-app/build/static/css/main.38a62222.css` & `cognite_neat-0.15.0/cognite/neat/explorer-ui/neat-app/build/static/css/main.38a62222.css`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.14.2/cognite/neat/explorer-ui/neat-app/build/static/css/main.38a62222.css.map` & `cognite_neat-0.15.0/cognite/neat/explorer-ui/neat-app/build/static/css/main.38a62222.css.map`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.14.2/cognite/neat/explorer-ui/neat-app/build/static/js/main.16555d84.js` & `cognite_neat-0.15.0/cognite/neat/explorer-ui/neat-app/build/static/js/main.16555d84.js`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.14.2/cognite/neat/explorer-ui/neat-app/build/static/js/main.16555d84.js.LICENSE.txt` & `cognite_neat-0.15.0/cognite/neat/explorer-ui/neat-app/build/static/js/main.16555d84.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.14.2/cognite/neat/explorer-ui/neat-app/build/static/js/main.16555d84.js.map` & `cognite_neat-0.15.0/cognite/neat/explorer-ui/neat-app/build/static/js/main.16555d84.js.map`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.14.2/cognite/neat/explorer-ui/neat-app/build/static/media/logo.4bdbcf8396881de06a6723a92fed910b.svg` & `cognite_neat-0.15.0/cognite/neat/explorer-ui/neat-app/build/static/media/logo.4bdbcf8396881de06a6723a92fed910b.svg`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.14.2/cognite/neat/migration/wf_manifests.py` & `cognite_neat-0.15.0/cognite/neat/migration/wf_manifests.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.14.2/pyproject.toml` & `cognite_neat-0.15.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cognite-neat"
-version = "0.14.2"
+version = "0.15.0"
 readme = "README.md"
 description = "Knowledge graph transformation"
 authors = ["Nikola Vasiljevic <nikola.vasiljevic@cognite.com>",
     "Anders Albert <anders.albert@cognite.com>",
     "Aleksandrs Livincovs <aleksandrs.livincovs@cognite.com>"]
 license = "Apache-2.0"
 documentation = "https://cognite-neat.readthedocs-hosted.com/"
@@ -38,26 +38,26 @@
 
 
 [tool.poetry.dependencies]
 python = ">=3.11,<3.12"
 pandas = "*"
 rdflib = "*"
 openpyxl = "*"
-pydantic = "*"
+pydantic = "^2"
 gspread = "*"
 google-api-python-client = "*"
 google-auth-oauthlib = "*"
 PyYAML = "*"
 requests = "*"
 urllib3 = "^1.26"
 uvicorn = {extras = ["standard"], version = "^0.21.0"}
-prometheus-client = "^0.16.0"
+prometheus-client = "^0.17.0"
 cognite-sdk = "^6"
 deepdiff = "*"
-fastapi = "^0.95"
+fastapi = "^0.100"
 schedule = "^1"
 python-multipart = "^0.0.6"
 oxrdflib = {version = "^0.3.3", extras = ["oxigraph"]}
 graphql-core = "^3.2.3"
 
 mkdocs =  {version="*", optional=true}
 mkdocs-jupyter = {version="*", optional=true}
```

### Comparing `cognite_neat-0.14.2/PKG-INFO` & `cognite_neat-0.15.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 Metadata-Version: 2.1
 Name: cognite-neat
-Version: 0.14.2
+Version: 0.15.0
 Summary: Knowledge graph transformation
 Home-page: https://cognite-neat.readthedocs-hosted.com/
 License: Apache-2.0
 Author: Nikola Vasiljevic
 Author-email: nikola.vasiljevic@cognite.com
 Requires-Python: >=3.11,<3.12
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: docs
 Requires-Dist: PyYAML
 Requires-Dist: cognite-sdk (>=6,<7)
 Requires-Dist: deepdiff
-Requires-Dist: fastapi (>=0.95,<0.96)
+Requires-Dist: fastapi (>=0.100,<0.101)
 Requires-Dist: google-api-python-client
 Requires-Dist: google-auth-oauthlib
 Requires-Dist: graphql-core (>=3.2.3,<4.0.0)
 Requires-Dist: gspread
 Requires-Dist: mkdocs ; extra == "docs"
 Requires-Dist: mkdocs-git-authors-plugin ; extra == "docs"
 Requires-Dist: mkdocs-git-revision-date-localized-plugin ; extra == "docs"
 Requires-Dist: mkdocs-gitbook ; extra == "docs"
 Requires-Dist: mkdocs-glightbox ; extra == "docs"
 Requires-Dist: mkdocs-jupyter ; extra == "docs"
 Requires-Dist: mkdocs-material-extensions ; extra == "docs"
 Requires-Dist: openpyxl
 Requires-Dist: oxrdflib[oxigraph] (>=0.3.3,<0.4.0)
 Requires-Dist: pandas
-Requires-Dist: prometheus-client (>=0.16.0,<0.17.0)
-Requires-Dist: pydantic
+Requires-Dist: prometheus-client (>=0.17.0,<0.18.0)
+Requires-Dist: pydantic (>=2,<3)
 Requires-Dist: python-multipart (>=0.0.6,<0.0.7)
 Requires-Dist: rdflib
 Requires-Dist: requests
 Requires-Dist: schedule (>=1,<2)
 Requires-Dist: urllib3 (>=1.26,<2.0)
 Requires-Dist: uvicorn[standard] (>=0.21.0,<0.22.0)
 Project-URL: Documentation, https://cognite-neat.readthedocs-hosted.com/
```

