# Comparing `tmp/otter-grader-4.4.0.tar.gz` & `tmp/otter-grader-4.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "otter-grader-4.4.0.tar", last modified: Thu Jul  6 03:08:29 2023, max compression
+gzip compressed data, was "otter-grader-4.4.1.tar", last modified: Sat Jul  8 20:33:06 2023, max compression
```

## Comparing `otter-grader-4.4.0.tar` & `otter-grader-4.4.1.tar`

### file list

```diff
@@ -1,170 +1,170 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 03:08:29.214744 otter-grader-4.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-07-06 03:07:57.000000 otter-grader-4.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-07-06 03:07:57.000000 otter-grader-4.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2679 2023-07-06 03:08:29.214744 otter-grader-4.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-07-06 03:07:57.000000 otter-grader-4.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 03:08:29.202744 otter-grader-4.4.0/otter/
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-06 03:07:57.000000 otter-grader-4.4.0/otter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-06 03:07:57.000000 otter-grader-4.4.0/otter/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-07-06 03:07:57.000000 otter-grader-4.4.0/otter/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 03:08:29.202744 otter-grader-4.4.0/otter/assign/
--rw-r--r--   0 runner    (1001) docker     (123)     7678 2023-07-06 03:08:27.000000 otter-grader-4.4.0/otter/assign/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11334 2023-07-06 03:07:57.000000 otter-grader-4.4.0/otter/assign/assignment.py
--rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-07-06 03:07:57.000000 otter-grader-4.4.0/otter/assign/blocks.py
--rw-r--r--   0 runner    (1001) docker     (123)     5679 2023-07-06 03:07:57.000000 otter-grader-4.4.0/otter/assign/cell_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-07-06 03:07:57.000000 otter-grader-4.4.0/otter/assign/feature_toggle.py
--rw-r--r--   0 runner    (1001) docker     (123)    16894 2023-07-06 03:07:57.000000 otter-grader-4.4.0/otter/assign/notebook_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4778 2023-07-06 03:07:57.000000 otter-grader-4.4.0/otter/assign/output.py
--rw-r--r--   0 runner    (1001) docker     (123)     2556 2023-07-06 03:07:57.000000 otter-grader-4.4.0/otter/assign/plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-07-06 03:07:57.000000 otter-grader-4.4.0/otter/assign/question_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 03:08:29.202744 otter-grader-4.4.0/otter/assign/r_adapter/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 03:07:57.000000 otter-grader-4.4.0/otter/assign/r_adapter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-07-06 03:07:57.000000 otter-grader-4.4.0/otter/assign/r_adapter/cell_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     4884 2023-07-06 03:07:57.000000 otter-grader-4.4.0/otter/assign/r_adapter/rmarkdown_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-07-06 03:07:57.000000 otter-grader-4.4.0/otter/assign/r_adapter/solutions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-07-06 03:07:57.000000 otter-grader-4.4.0/otter/assign/r_adapter/tests_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     6597 2023-07-06 03:07:57.000000 otter-grader-4.4.0/otter/assign/solutions.py
--rw-r--r--   0 runner    (1001) docker     (123)    13842 2023-07-06 03:08:27.000000 otter-grader-4.4.0/otter/assign/tests_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    11365 2023-07-06 03:07:57.000000 otter-grader-4.4.0/otter/assign/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 03:08:29.202744 otter-grader-4.4.0/otter/assign/v0/
--rw-r--r--   0 runner    (1001) docker     (123)     6010 2023-07-06 03:07:57.000000 otter-grader-4.4.0/otter/assign/v0/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8405 2023-07-06 03:07:57.000000 otter-grader-4.4.0/otter/assign/v0/assignment.py
--rw-r--r--   0 runner    (1001) docker     (123)     5652 2023-07-06 03:07:57.000000 otter-grader-4.4.0/otter/assign/v0/cell_generators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-07-06 03:07:57.000000 otter-grader-4.4.0/otter/assign/v0/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 03:08:29.202744 otter-grader-4.4.0/otter/assign/v0/convert/
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-06 03:07:57.000000 otter-grader-4.4.0/otter/assign/v0/convert/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-06 03:07:57.000000 otter-grader-4.4.0/otter/assign/v0/convert/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6794 2023-07-06 03:07:57.000000 otter-grader-4.4.0/otter/assign/v0/convert/notebook_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     8047 2023-07-06 03:07:57.000000 otter-grader-4.4.0/otter/assign/v0/notebook_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6760 2023-07-06 03:07:57.000000 otter-grader-4.4.0/otter/assign/v0/output.py
--rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-07-06 03:07:57.000000 otter-grader-4.4.0/otter/assign/v0/plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)     2276 2023-07-06 03:07:57.000000 otter-grader-4.4.0/otter/assign/v0/questions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 03:08:29.202744 otter-grader-4.4.0/otter/assign/v0/r_adapter/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 03:07:57.000000 otter-grader-4.4.0/otter/assign/v0/r_adapter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4687 2023-07-06 03:07:57.000000 otter-grader-4.4.0/otter/assign/v0/r_adapter/tests.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 03:08:29.206744 otter-grader-4.4.0/otter/assign/v0/rmarkdown_adapter/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 03:07:57.000000 otter-grader-4.4.0/otter/assign/v0/rmarkdown_adapter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-06 03:07:57.000000 otter-grader-4.4.0/otter/assign/v0/rmarkdown_adapter/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     5262 2023-07-06 03:07:57.000000 otter-grader-4.4.0/otter/assign/v0/rmarkdown_adapter/notebook_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5314 2023-07-06 03:07:57.000000 otter-grader-4.4.0/otter/assign/v0/rmarkdown_adapter/output.py
--rw-r--r--   0 runner    (1001) docker     (123)     3902 2023-07-06 03:07:57.000000 otter-grader-4.4.0/otter/assign/v0/rmarkdown_adapter/solutions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-07-06 03:07:57.000000 otter-grader-4.4.0/otter/assign/v0/rmarkdown_adapter/tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-07-06 03:07:57.000000 otter-grader-4.4.0/otter/assign/v0/rmarkdown_adapter/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4868 2023-07-06 03:07:57.000000 otter-grader-4.4.0/otter/assign/v0/solutions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7883 2023-07-06 03:07:57.000000 otter-grader-4.4.0/otter/assign/v0/tests.py
--rw-r--r--   0 runner    (1001) docker     (123)    11122 2023-07-06 03:07:57.000000 otter-grader-4.4.0/otter/assign/v0/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 03:08:29.206744 otter-grader-4.4.0/otter/check/
--rw-r--r--   0 runner    (1001) docker     (123)     3558 2023-07-06 03:07:57.000000 otter-grader-4.4.0/otter/check/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17923 2023-07-06 03:07:57.000000 otter-grader-4.4.0/otter/check/logs.py
--rw-r--r--   0 runner    (1001) docker     (123)    18909 2023-07-06 03:07:57.000000 otter-grader-4.4.0/otter/check/notebook.py
--rw-r--r--   0 runner    (1001) docker     (123)     8888 2023-07-06 03:07:57.000000 otter-grader-4.4.0/otter/check/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 03:08:29.206744 otter-grader-4.4.0/otter/check/validate_export/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-06 03:07:57.000000 otter-grader-4.4.0/otter/check/validate_export/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-07-06 03:07:57.000000 otter-grader-4.4.0/otter/check/validate_export/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8313 2023-07-06 03:07:57.000000 otter-grader-4.4.0/otter/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 03:08:29.206744 otter-grader-4.4.0/otter/execute/
--rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-07-06 03:07:57.000000 otter-grader-4.4.0/otter/execute/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2480 2023-07-06 03:07:57.000000 otter-grader-4.4.0/otter/execute/checker.py
--rw-r--r--   0 runner    (1001) docker     (123)     3671 2023-07-06 03:07:57.000000 otter-grader-4.4.0/otter/execute/execute_log.py
--rw-r--r--   0 runner    (1001) docker     (123)     5085 2023-07-06 03:07:57.000000 otter-grader-4.4.0/otter/execute/execute_notebook.py
--rw-r--r--   0 runner    (1001) docker     (123)     2246 2023-07-06 03:07:57.000000 otter-grader-4.4.0/otter/execute/transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 03:08:29.206744 otter-grader-4.4.0/otter/export/
--rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-07-06 03:07:57.000000 otter-grader-4.4.0/otter/export/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 03:08:29.206744 otter-grader-4.4.0/otter/export/exporters/
--rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-07-06 03:07:57.000000 otter-grader-4.4.0/otter/export/exporters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5541 2023-07-06 03:07:57.000000 otter-grader-4.4.0/otter/export/exporters/base_exporter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 03:08:29.206744 otter-grader-4.4.0/otter/export/exporters/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 03:08:29.206744 otter-grader-4.4.0/otter/export/exporters/templates/via_html/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-06 03:07:57.000000 otter-grader-4.4.0/otter/export/exporters/templates/via_html/conf.json
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-07-06 03:07:57.000000 otter-grader-4.4.0/otter/export/exporters/templates/via_html/index.html.j2
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-07-06 03:07:57.000000 otter-grader-4.4.0/otter/export/exporters/templates/via_html.tpl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 03:08:29.206744 otter-grader-4.4.0/otter/export/exporters/templates/via_latex/
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-06 03:07:57.000000 otter-grader-4.4.0/otter/export/exporters/templates/via_latex/conf.json
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-07-06 03:07:57.000000 otter-grader-4.4.0/otter/export/exporters/templates/via_latex/index.tex.j2
--rw-r--r--   0 runner    (1001) docker     (123)      894 2023-07-06 03:07:57.000000 otter-grader-4.4.0/otter/export/exporters/templates/via_latex.tpl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 03:08:29.206744 otter-grader-4.4.0/otter/export/exporters/templates/via_latex_xecjk/
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-06 03:07:57.000000 otter-grader-4.4.0/otter/export/exporters/templates/via_latex_xecjk/conf.json
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-07-06 03:07:57.000000 otter-grader-4.4.0/otter/export/exporters/templates/via_latex_xecjk/index.tex.j2
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-07-06 03:07:57.000000 otter-grader-4.4.0/otter/export/exporters/templates/via_latex_xecjk.tpl
--rw-r--r--   0 runner    (1001) docker     (123)     3330 2023-07-06 03:07:57.000000 otter-grader-4.4.0/otter/export/exporters/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2603 2023-07-06 03:07:57.000000 otter-grader-4.4.0/otter/export/exporters/via_html.py
--rw-r--r--   0 runner    (1001) docker     (123)     3475 2023-07-06 03:07:57.000000 otter-grader-4.4.0/otter/export/exporters/via_latex.py
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-07-06 03:07:57.000000 otter-grader-4.4.0/otter/export/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 03:08:29.206744 otter-grader-4.4.0/otter/generate/
--rw-r--r--   0 runner    (1001) docker     (123)     8451 2023-07-06 03:07:57.000000 otter-grader-4.4.0/otter/generate/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 03:08:29.198744 otter-grader-4.4.0/otter/generate/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 03:08:29.206744 otter-grader-4.4.0/otter/generate/templates/python/
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-07-06 03:07:57.000000 otter-grader-4.4.0/otter/generate/templates/python/environment.yml
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-07-06 03:08:27.000000 otter-grader-4.4.0/otter/generate/templates/python/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-07-06 03:07:57.000000 otter-grader-4.4.0/otter/generate/templates/python/run_autograder
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-07-06 03:07:57.000000 otter-grader-4.4.0/otter/generate/templates/python/run_otter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-07-06 03:07:57.000000 otter-grader-4.4.0/otter/generate/templates/python/setup.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 03:08:29.210744 otter-grader-4.4.0/otter/generate/templates/r/
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-07-06 03:07:57.000000 otter-grader-4.4.0/otter/generate/templates/r/environment.yml
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-07-06 03:07:57.000000 otter-grader-4.4.0/otter/generate/templates/r/requirements.r
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-07-06 03:08:27.000000 otter-grader-4.4.0/otter/generate/templates/r/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-07-06 03:07:57.000000 otter-grader-4.4.0/otter/generate/templates/r/run_autograder
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-07-06 03:07:57.000000 otter-grader-4.4.0/otter/generate/templates/r/run_otter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-07-06 03:07:57.000000 otter-grader-4.4.0/otter/generate/templates/r/setup.sh
--rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-07-06 03:07:57.000000 otter-grader-4.4.0/otter/generate/token.py
--rw-r--r--   0 runner    (1001) docker     (123)      997 2023-07-06 03:07:57.000000 otter-grader-4.4.0/otter/generate/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 03:08:29.210744 otter-grader-4.4.0/otter/grade/
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-07-06 03:07:57.000000 otter-grader-4.4.0/otter/grade/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     3601 2023-07-06 03:07:57.000000 otter-grader-4.4.0/otter/grade/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7895 2023-07-06 03:07:57.000000 otter-grader-4.4.0/otter/grade/containers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-07-06 03:07:57.000000 otter-grader-4.4.0/otter/grade/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 03:08:29.210744 otter-grader-4.4.0/otter/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)     7636 2023-07-06 03:07:57.000000 otter-grader-4.4.0/otter/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9124 2023-07-06 03:07:57.000000 otter-grader-4.4.0/otter/plugins/abstract_plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 03:08:29.210744 otter-grader-4.4.0/otter/plugins/builtin/
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-07-06 03:07:57.000000 otter-grader-4.4.0/otter/plugins/builtin/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 03:08:29.210744 otter-grader-4.4.0/otter/plugins/builtin/gmail_notifications/
--rw-r--r--   0 runner    (1001) docker     (123)     6061 2023-07-06 03:07:57.000000 otter-grader-4.4.0/otter/plugins/builtin/gmail_notifications/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 03:08:29.210744 otter-grader-4.4.0/otter/plugins/builtin/gmail_notifications/bin/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 03:07:57.000000 otter-grader-4.4.0/otter/plugins/builtin/gmail_notifications/bin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14192 2023-07-06 03:07:57.000000 otter-grader-4.4.0/otter/plugins/builtin/gmail_notifications/bin/gmail_oauth2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5949 2023-07-06 03:08:27.000000 otter-grader-4.4.0/otter/plugins/builtin/grade_override.py
--rw-r--r--   0 runner    (1001) docker     (123)     4759 2023-07-06 03:07:57.000000 otter-grader-4.4.0/otter/plugins/builtin/rate_limiting.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 03:08:29.210744 otter-grader-4.4.0/otter/run/
--rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-07-06 03:07:57.000000 otter-grader-4.4.0/otter/run/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 03:08:29.210744 otter-grader-4.4.0/otter/run/run_autograder/
--rw-r--r--   0 runner    (1001) docker     (123)     3747 2023-07-06 03:07:57.000000 otter-grader-4.4.0/otter/run/run_autograder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4663 2023-07-06 03:07:57.000000 otter-grader-4.4.0/otter/run/run_autograder/autograder_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 03:08:29.210744 otter-grader-4.4.0/otter/run/run_autograder/runners/
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-07-06 03:07:57.000000 otter-grader-4.4.0/otter/run/run_autograder/runners/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6918 2023-07-06 03:07:57.000000 otter-grader-4.4.0/otter/run/run_autograder/runners/abstract_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     5664 2023-07-06 03:07:57.000000 otter-grader-4.4.0/otter/run/run_autograder/runners/python_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     7029 2023-07-06 03:07:57.000000 otter-grader-4.4.0/otter/run/run_autograder/runners/r_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-07-06 03:07:57.000000 otter-grader-4.4.0/otter/run/run_autograder/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 03:08:29.210744 otter-grader-4.4.0/otter/test_files/
--rw-r--r--   0 runner    (1001) docker     (123)    15243 2023-07-06 03:07:57.000000 otter-grader-4.4.0/otter/test_files/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9442 2023-07-06 03:08:27.000000 otter-grader-4.4.0/otter/test_files/abstract_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     9224 2023-07-06 03:07:57.000000 otter-grader-4.4.0/otter/test_files/exception_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4831 2023-07-06 03:07:57.000000 otter-grader-4.4.0/otter/test_files/metadata_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6103 2023-07-06 03:07:57.000000 otter-grader-4.4.0/otter/test_files/ok_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-07-06 03:07:57.000000 otter-grader-4.4.0/otter/test_files/ottr_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    13040 2023-07-06 03:07:57.000000 otter-grader-4.4.0/otter/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-07-06 03:08:27.000000 otter-grader-4.4.0/otter/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 03:08:29.210744 otter-grader-4.4.0/otter_grader.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2679 2023-07-06 03:08:28.000000 otter-grader-4.4.0/otter_grader.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4525 2023-07-06 03:08:29.000000 otter-grader-4.4.0/otter_grader.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 03:08:28.000000 otter-grader-4.4.0/otter_grader.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-07-06 03:08:28.000000 otter-grader-4.4.0/otter_grader.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-06 03:08:28.000000 otter-grader-4.4.0/otter_grader.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-06 03:08:28.000000 otter-grader-4.4.0/otter_grader.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-06 03:07:57.000000 otter-grader-4.4.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 03:08:29.214744 otter-grader-4.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-07-06 03:07:57.000000 otter-grader-4.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 03:08:29.214744 otter-grader-4.4.0/test/
--rw-r--r--   0 runner    (1001) docker     (123)     8054 2023-07-06 03:08:27.000000 otter-grader-4.4.0/test/test_assign.py
--rw-r--r--   0 runner    (1001) docker     (123)     5013 2023-07-06 03:07:57.000000 otter-grader-4.4.0/test/test_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     3490 2023-07-06 03:07:57.000000 otter-grader-4.4.0/test/test_export.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 03:08:29.214744 otter-grader-4.4.0/test/test_generate/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 03:07:57.000000 otter-grader-4.4.0/test/test_generate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3191 2023-07-06 03:07:57.000000 otter-grader-4.4.0/test/test_generate/test_autograder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2443 2023-07-06 03:07:57.000000 otter-grader-4.4.0/test/test_generate/test_token.py
--rw-r--r--   0 runner    (1001) docker     (123)     9052 2023-07-06 03:07:57.000000 otter-grader-4.4.0/test/test_grade.py
--rw-r--r--   0 runner    (1001) docker     (123)     4049 2023-07-06 03:07:57.000000 otter-grader-4.4.0/test/test_logs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7540 2023-07-06 03:07:57.000000 otter-grader-4.4.0/test/test_notebook.py
--rw-r--r--   0 runner    (1001) docker     (123)    15187 2023-07-06 03:07:57.000000 otter-grader-4.4.0/test/test_run.py
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-06 03:07:57.000000 otter-grader-4.4.0/test/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 20:33:06.289065 otter-grader-4.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-07-08 20:32:38.000000 otter-grader-4.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-07-08 20:32:38.000000 otter-grader-4.4.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2679 2023-07-08 20:33:06.289065 otter-grader-4.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-07-08 20:32:38.000000 otter-grader-4.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 20:33:06.277065 otter-grader-4.4.1/otter/
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-08 20:32:38.000000 otter-grader-4.4.1/otter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-08 20:32:38.000000 otter-grader-4.4.1/otter/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-07-08 20:32:38.000000 otter-grader-4.4.1/otter/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 20:33:06.277065 otter-grader-4.4.1/otter/assign/
+-rw-r--r--   0 runner    (1001) docker     (123)     7678 2023-07-08 20:32:38.000000 otter-grader-4.4.1/otter/assign/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11334 2023-07-08 20:32:38.000000 otter-grader-4.4.1/otter/assign/assignment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-07-08 20:32:38.000000 otter-grader-4.4.1/otter/assign/blocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5679 2023-07-08 20:32:38.000000 otter-grader-4.4.1/otter/assign/cell_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-07-08 20:32:38.000000 otter-grader-4.4.1/otter/assign/feature_toggle.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16894 2023-07-08 20:32:38.000000 otter-grader-4.4.1/otter/assign/notebook_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4778 2023-07-08 20:32:38.000000 otter-grader-4.4.1/otter/assign/output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2556 2023-07-08 20:32:38.000000 otter-grader-4.4.1/otter/assign/plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-07-08 20:32:38.000000 otter-grader-4.4.1/otter/assign/question_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 20:33:06.277065 otter-grader-4.4.1/otter/assign/r_adapter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 20:32:38.000000 otter-grader-4.4.1/otter/assign/r_adapter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-07-08 20:32:38.000000 otter-grader-4.4.1/otter/assign/r_adapter/cell_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4884 2023-07-08 20:32:38.000000 otter-grader-4.4.1/otter/assign/r_adapter/rmarkdown_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-07-08 20:32:38.000000 otter-grader-4.4.1/otter/assign/r_adapter/solutions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-07-08 20:32:38.000000 otter-grader-4.4.1/otter/assign/r_adapter/tests_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6597 2023-07-08 20:32:38.000000 otter-grader-4.4.1/otter/assign/solutions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13842 2023-07-08 20:32:38.000000 otter-grader-4.4.1/otter/assign/tests_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11365 2023-07-08 20:32:38.000000 otter-grader-4.4.1/otter/assign/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 20:33:06.281065 otter-grader-4.4.1/otter/assign/v0/
+-rw-r--r--   0 runner    (1001) docker     (123)     6010 2023-07-08 20:32:38.000000 otter-grader-4.4.1/otter/assign/v0/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8405 2023-07-08 20:32:38.000000 otter-grader-4.4.1/otter/assign/v0/assignment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5652 2023-07-08 20:32:38.000000 otter-grader-4.4.1/otter/assign/v0/cell_generators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-07-08 20:32:38.000000 otter-grader-4.4.1/otter/assign/v0/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 20:33:06.281065 otter-grader-4.4.1/otter/assign/v0/convert/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-08 20:32:38.000000 otter-grader-4.4.1/otter/assign/v0/convert/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-08 20:32:38.000000 otter-grader-4.4.1/otter/assign/v0/convert/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6794 2023-07-08 20:32:38.000000 otter-grader-4.4.1/otter/assign/v0/convert/notebook_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8047 2023-07-08 20:32:38.000000 otter-grader-4.4.1/otter/assign/v0/notebook_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6760 2023-07-08 20:32:38.000000 otter-grader-4.4.1/otter/assign/v0/output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-07-08 20:32:38.000000 otter-grader-4.4.1/otter/assign/v0/plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2276 2023-07-08 20:32:38.000000 otter-grader-4.4.1/otter/assign/v0/questions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 20:33:06.281065 otter-grader-4.4.1/otter/assign/v0/r_adapter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 20:32:38.000000 otter-grader-4.4.1/otter/assign/v0/r_adapter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4687 2023-07-08 20:32:38.000000 otter-grader-4.4.1/otter/assign/v0/r_adapter/tests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 20:33:06.281065 otter-grader-4.4.1/otter/assign/v0/rmarkdown_adapter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 20:32:38.000000 otter-grader-4.4.1/otter/assign/v0/rmarkdown_adapter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-08 20:32:38.000000 otter-grader-4.4.1/otter/assign/v0/rmarkdown_adapter/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5262 2023-07-08 20:32:38.000000 otter-grader-4.4.1/otter/assign/v0/rmarkdown_adapter/notebook_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5314 2023-07-08 20:32:38.000000 otter-grader-4.4.1/otter/assign/v0/rmarkdown_adapter/output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3902 2023-07-08 20:32:38.000000 otter-grader-4.4.1/otter/assign/v0/rmarkdown_adapter/solutions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-07-08 20:32:38.000000 otter-grader-4.4.1/otter/assign/v0/rmarkdown_adapter/tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-07-08 20:32:38.000000 otter-grader-4.4.1/otter/assign/v0/rmarkdown_adapter/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4868 2023-07-08 20:32:38.000000 otter-grader-4.4.1/otter/assign/v0/solutions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7883 2023-07-08 20:32:38.000000 otter-grader-4.4.1/otter/assign/v0/tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11122 2023-07-08 20:32:38.000000 otter-grader-4.4.1/otter/assign/v0/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 20:33:06.281065 otter-grader-4.4.1/otter/check/
+-rw-r--r--   0 runner    (1001) docker     (123)     3558 2023-07-08 20:32:38.000000 otter-grader-4.4.1/otter/check/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17923 2023-07-08 20:32:38.000000 otter-grader-4.4.1/otter/check/logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18909 2023-07-08 20:32:38.000000 otter-grader-4.4.1/otter/check/notebook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8888 2023-07-08 20:32:38.000000 otter-grader-4.4.1/otter/check/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 20:33:06.281065 otter-grader-4.4.1/otter/check/validate_export/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-08 20:32:38.000000 otter-grader-4.4.1/otter/check/validate_export/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-07-08 20:32:38.000000 otter-grader-4.4.1/otter/check/validate_export/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8313 2023-07-08 20:32:38.000000 otter-grader-4.4.1/otter/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 20:33:06.281065 otter-grader-4.4.1/otter/execute/
+-rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-07-08 20:32:38.000000 otter-grader-4.4.1/otter/execute/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2480 2023-07-08 20:32:38.000000 otter-grader-4.4.1/otter/execute/checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3671 2023-07-08 20:32:38.000000 otter-grader-4.4.1/otter/execute/execute_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5085 2023-07-08 20:32:38.000000 otter-grader-4.4.1/otter/execute/execute_notebook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2246 2023-07-08 20:32:38.000000 otter-grader-4.4.1/otter/execute/transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 20:33:06.281065 otter-grader-4.4.1/otter/export/
+-rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-07-08 20:32:38.000000 otter-grader-4.4.1/otter/export/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 20:33:06.281065 otter-grader-4.4.1/otter/export/exporters/
+-rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-07-08 20:32:38.000000 otter-grader-4.4.1/otter/export/exporters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5541 2023-07-08 20:32:38.000000 otter-grader-4.4.1/otter/export/exporters/base_exporter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 20:33:06.281065 otter-grader-4.4.1/otter/export/exporters/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 20:33:06.285065 otter-grader-4.4.1/otter/export/exporters/templates/via_html/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-08 20:32:38.000000 otter-grader-4.4.1/otter/export/exporters/templates/via_html/conf.json
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-07-08 20:32:38.000000 otter-grader-4.4.1/otter/export/exporters/templates/via_html/index.html.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-07-08 20:32:38.000000 otter-grader-4.4.1/otter/export/exporters/templates/via_html.tpl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 20:33:06.285065 otter-grader-4.4.1/otter/export/exporters/templates/via_latex/
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-08 20:32:38.000000 otter-grader-4.4.1/otter/export/exporters/templates/via_latex/conf.json
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-07-08 20:32:38.000000 otter-grader-4.4.1/otter/export/exporters/templates/via_latex/index.tex.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      894 2023-07-08 20:32:38.000000 otter-grader-4.4.1/otter/export/exporters/templates/via_latex.tpl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 20:33:06.285065 otter-grader-4.4.1/otter/export/exporters/templates/via_latex_xecjk/
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-08 20:32:38.000000 otter-grader-4.4.1/otter/export/exporters/templates/via_latex_xecjk/conf.json
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-07-08 20:32:38.000000 otter-grader-4.4.1/otter/export/exporters/templates/via_latex_xecjk/index.tex.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-07-08 20:32:38.000000 otter-grader-4.4.1/otter/export/exporters/templates/via_latex_xecjk.tpl
+-rw-r--r--   0 runner    (1001) docker     (123)     3330 2023-07-08 20:32:38.000000 otter-grader-4.4.1/otter/export/exporters/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2603 2023-07-08 20:32:38.000000 otter-grader-4.4.1/otter/export/exporters/via_html.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3475 2023-07-08 20:32:38.000000 otter-grader-4.4.1/otter/export/exporters/via_latex.py
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-07-08 20:32:38.000000 otter-grader-4.4.1/otter/export/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 20:33:06.285065 otter-grader-4.4.1/otter/generate/
+-rw-r--r--   0 runner    (1001) docker     (123)     8451 2023-07-08 20:32:38.000000 otter-grader-4.4.1/otter/generate/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 20:33:06.269065 otter-grader-4.4.1/otter/generate/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 20:33:06.285065 otter-grader-4.4.1/otter/generate/templates/python/
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-07-08 20:32:38.000000 otter-grader-4.4.1/otter/generate/templates/python/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-07-08 20:33:04.000000 otter-grader-4.4.1/otter/generate/templates/python/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-07-08 20:32:38.000000 otter-grader-4.4.1/otter/generate/templates/python/run_autograder
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-07-08 20:32:38.000000 otter-grader-4.4.1/otter/generate/templates/python/run_otter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-07-08 20:32:38.000000 otter-grader-4.4.1/otter/generate/templates/python/setup.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 20:33:06.285065 otter-grader-4.4.1/otter/generate/templates/r/
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-07-08 20:32:38.000000 otter-grader-4.4.1/otter/generate/templates/r/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-07-08 20:32:38.000000 otter-grader-4.4.1/otter/generate/templates/r/requirements.r
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-07-08 20:33:04.000000 otter-grader-4.4.1/otter/generate/templates/r/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-07-08 20:32:38.000000 otter-grader-4.4.1/otter/generate/templates/r/run_autograder
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-07-08 20:32:38.000000 otter-grader-4.4.1/otter/generate/templates/r/run_otter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-07-08 20:32:38.000000 otter-grader-4.4.1/otter/generate/templates/r/setup.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-07-08 20:32:38.000000 otter-grader-4.4.1/otter/generate/token.py
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-07-08 20:32:38.000000 otter-grader-4.4.1/otter/generate/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 20:33:06.285065 otter-grader-4.4.1/otter/grade/
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-07-08 20:32:38.000000 otter-grader-4.4.1/otter/grade/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     3601 2023-07-08 20:32:38.000000 otter-grader-4.4.1/otter/grade/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8032 2023-07-08 20:33:04.000000 otter-grader-4.4.1/otter/grade/containers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-07-08 20:32:38.000000 otter-grader-4.4.1/otter/grade/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 20:33:06.285065 otter-grader-4.4.1/otter/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)     7636 2023-07-08 20:32:38.000000 otter-grader-4.4.1/otter/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9124 2023-07-08 20:32:38.000000 otter-grader-4.4.1/otter/plugins/abstract_plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 20:33:06.285065 otter-grader-4.4.1/otter/plugins/builtin/
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-07-08 20:32:38.000000 otter-grader-4.4.1/otter/plugins/builtin/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 20:33:06.285065 otter-grader-4.4.1/otter/plugins/builtin/gmail_notifications/
+-rw-r--r--   0 runner    (1001) docker     (123)     6061 2023-07-08 20:32:38.000000 otter-grader-4.4.1/otter/plugins/builtin/gmail_notifications/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 20:33:06.285065 otter-grader-4.4.1/otter/plugins/builtin/gmail_notifications/bin/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 20:32:38.000000 otter-grader-4.4.1/otter/plugins/builtin/gmail_notifications/bin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14192 2023-07-08 20:32:38.000000 otter-grader-4.4.1/otter/plugins/builtin/gmail_notifications/bin/gmail_oauth2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5949 2023-07-08 20:32:38.000000 otter-grader-4.4.1/otter/plugins/builtin/grade_override.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4759 2023-07-08 20:32:38.000000 otter-grader-4.4.1/otter/plugins/builtin/rate_limiting.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 20:33:06.285065 otter-grader-4.4.1/otter/run/
+-rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-07-08 20:32:38.000000 otter-grader-4.4.1/otter/run/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 20:33:06.285065 otter-grader-4.4.1/otter/run/run_autograder/
+-rw-r--r--   0 runner    (1001) docker     (123)     3747 2023-07-08 20:32:38.000000 otter-grader-4.4.1/otter/run/run_autograder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4663 2023-07-08 20:32:38.000000 otter-grader-4.4.1/otter/run/run_autograder/autograder_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 20:33:06.289065 otter-grader-4.4.1/otter/run/run_autograder/runners/
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-07-08 20:32:38.000000 otter-grader-4.4.1/otter/run/run_autograder/runners/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6918 2023-07-08 20:32:38.000000 otter-grader-4.4.1/otter/run/run_autograder/runners/abstract_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5664 2023-07-08 20:32:38.000000 otter-grader-4.4.1/otter/run/run_autograder/runners/python_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7029 2023-07-08 20:32:38.000000 otter-grader-4.4.1/otter/run/run_autograder/runners/r_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-07-08 20:32:38.000000 otter-grader-4.4.1/otter/run/run_autograder/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 20:33:06.289065 otter-grader-4.4.1/otter/test_files/
+-rw-r--r--   0 runner    (1001) docker     (123)    15243 2023-07-08 20:32:38.000000 otter-grader-4.4.1/otter/test_files/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9442 2023-07-08 20:32:38.000000 otter-grader-4.4.1/otter/test_files/abstract_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9224 2023-07-08 20:32:38.000000 otter-grader-4.4.1/otter/test_files/exception_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4831 2023-07-08 20:32:38.000000 otter-grader-4.4.1/otter/test_files/metadata_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6103 2023-07-08 20:32:38.000000 otter-grader-4.4.1/otter/test_files/ok_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-07-08 20:32:38.000000 otter-grader-4.4.1/otter/test_files/ottr_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13040 2023-07-08 20:32:38.000000 otter-grader-4.4.1/otter/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-07-08 20:33:04.000000 otter-grader-4.4.1/otter/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 20:33:06.289065 otter-grader-4.4.1/otter_grader.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2679 2023-07-08 20:33:06.000000 otter-grader-4.4.1/otter_grader.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4525 2023-07-08 20:33:06.000000 otter-grader-4.4.1/otter_grader.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 20:33:06.000000 otter-grader-4.4.1/otter_grader.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-07-08 20:33:06.000000 otter-grader-4.4.1/otter_grader.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-08 20:33:06.000000 otter-grader-4.4.1/otter_grader.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-08 20:33:06.000000 otter-grader-4.4.1/otter_grader.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-08 20:32:38.000000 otter-grader-4.4.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 20:33:06.289065 otter-grader-4.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-07-08 20:32:38.000000 otter-grader-4.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 20:33:06.289065 otter-grader-4.4.1/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     8054 2023-07-08 20:32:38.000000 otter-grader-4.4.1/test/test_assign.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5013 2023-07-08 20:32:38.000000 otter-grader-4.4.1/test/test_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3490 2023-07-08 20:32:38.000000 otter-grader-4.4.1/test/test_export.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 20:33:06.289065 otter-grader-4.4.1/test/test_generate/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 20:32:38.000000 otter-grader-4.4.1/test/test_generate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3191 2023-07-08 20:32:38.000000 otter-grader-4.4.1/test/test_generate/test_autograder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2443 2023-07-08 20:32:38.000000 otter-grader-4.4.1/test/test_generate/test_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9052 2023-07-08 20:32:38.000000 otter-grader-4.4.1/test/test_grade.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4049 2023-07-08 20:32:38.000000 otter-grader-4.4.1/test/test_logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7540 2023-07-08 20:32:38.000000 otter-grader-4.4.1/test/test_notebook.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15187 2023-07-08 20:32:38.000000 otter-grader-4.4.1/test/test_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-08 20:32:38.000000 otter-grader-4.4.1/test/test_utils.py
```

### Comparing `otter-grader-4.4.0/LICENSE` & `otter-grader-4.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `otter-grader-4.4.0/PKG-INFO` & `otter-grader-4.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: otter-grader
-Version: 4.4.0
+Version: 4.4.1
 Summary: Python and Jupyter Notebook autograder
 Home-page: https://github.com/ucbds-infra/otter-grader
 Author: Christopher Pyles
 Author-email: otter-grader@berkeley.edu
 License: BSD-3-Clause
 Description: # Otter-Grader
```

### Comparing `otter-grader-4.4.0/README.md` & `otter-grader-4.4.1/README.md`

 * *Files identical despite different names*

### Comparing `otter-grader-4.4.0/otter/api.py` & `otter-grader-4.4.1/otter/api.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.4.0/otter/assign/__init__.py` & `otter-grader-4.4.1/otter/assign/__init__.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.4.0/otter/assign/assignment.py` & `otter-grader-4.4.1/otter/assign/assignment.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.4.0/otter/assign/blocks.py` & `otter-grader-4.4.1/otter/assign/blocks.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.4.0/otter/assign/cell_factory.py` & `otter-grader-4.4.1/otter/assign/cell_factory.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.4.0/otter/assign/feature_toggle.py` & `otter-grader-4.4.1/otter/assign/feature_toggle.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.4.0/otter/assign/notebook_transformer.py` & `otter-grader-4.4.1/otter/assign/notebook_transformer.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.4.0/otter/assign/output.py` & `otter-grader-4.4.1/otter/assign/output.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.4.0/otter/assign/plugins.py` & `otter-grader-4.4.1/otter/assign/plugins.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.4.0/otter/assign/question_config.py` & `otter-grader-4.4.1/otter/assign/question_config.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.4.0/otter/assign/r_adapter/cell_factory.py` & `otter-grader-4.4.1/otter/assign/r_adapter/cell_factory.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.4.0/otter/assign/r_adapter/rmarkdown_converter.py` & `otter-grader-4.4.1/otter/assign/r_adapter/rmarkdown_converter.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.4.0/otter/assign/r_adapter/solutions.py` & `otter-grader-4.4.1/otter/assign/r_adapter/solutions.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.4.0/otter/assign/r_adapter/tests_manager.py` & `otter-grader-4.4.1/otter/assign/r_adapter/tests_manager.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.4.0/otter/assign/solutions.py` & `otter-grader-4.4.1/otter/assign/solutions.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.4.0/otter/assign/tests_manager.py` & `otter-grader-4.4.1/otter/assign/tests_manager.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.4.0/otter/assign/utils.py` & `otter-grader-4.4.1/otter/assign/utils.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.4.0/otter/assign/v0/__init__.py` & `otter-grader-4.4.1/otter/assign/v0/__init__.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.4.0/otter/assign/v0/assignment.py` & `otter-grader-4.4.1/otter/assign/v0/assignment.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.4.0/otter/assign/v0/cell_generators.py` & `otter-grader-4.4.1/otter/assign/v0/cell_generators.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.4.0/otter/assign/v0/constants.py` & `otter-grader-4.4.1/otter/assign/v0/constants.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.4.0/otter/assign/v0/convert/__main__.py` & `otter-grader-4.4.1/otter/assign/v0/convert/__main__.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.4.0/otter/assign/v0/convert/notebook_transformer.py` & `otter-grader-4.4.1/otter/assign/v0/convert/notebook_transformer.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.4.0/otter/assign/v0/notebook_transformer.py` & `otter-grader-4.4.1/otter/assign/v0/notebook_transformer.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.4.0/otter/assign/v0/output.py` & `otter-grader-4.4.1/otter/assign/v0/output.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.4.0/otter/assign/v0/plugins.py` & `otter-grader-4.4.1/otter/assign/v0/plugins.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.4.0/otter/assign/v0/questions.py` & `otter-grader-4.4.1/otter/assign/v0/questions.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.4.0/otter/assign/v0/r_adapter/tests.py` & `otter-grader-4.4.1/otter/assign/v0/r_adapter/tests.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.4.0/otter/assign/v0/rmarkdown_adapter/notebook_transformer.py` & `otter-grader-4.4.1/otter/assign/v0/rmarkdown_adapter/notebook_transformer.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.4.0/otter/assign/v0/rmarkdown_adapter/output.py` & `otter-grader-4.4.1/otter/assign/v0/rmarkdown_adapter/output.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.4.0/otter/assign/v0/rmarkdown_adapter/solutions.py` & `otter-grader-4.4.1/otter/assign/v0/rmarkdown_adapter/solutions.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.4.0/otter/assign/v0/rmarkdown_adapter/tests.py` & `otter-grader-4.4.1/otter/assign/v0/rmarkdown_adapter/tests.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.4.0/otter/assign/v0/rmarkdown_adapter/utils.py` & `otter-grader-4.4.1/otter/assign/v0/rmarkdown_adapter/utils.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.4.0/otter/assign/v0/solutions.py` & `otter-grader-4.4.1/otter/assign/v0/solutions.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.4.0/otter/assign/v0/tests.py` & `otter-grader-4.4.1/otter/assign/v0/tests.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.4.0/otter/assign/v0/utils.py` & `otter-grader-4.4.1/otter/assign/v0/utils.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.4.0/otter/check/__init__.py` & `otter-grader-4.4.1/otter/check/__init__.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.4.0/otter/check/logs.py` & `otter-grader-4.4.1/otter/check/logs.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.4.0/otter/check/notebook.py` & `otter-grader-4.4.1/otter/check/notebook.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.4.0/otter/check/utils.py` & `otter-grader-4.4.1/otter/check/utils.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.4.0/otter/check/validate_export/__main__.py` & `otter-grader-4.4.1/otter/check/validate_export/__main__.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.4.0/otter/cli.py` & `otter-grader-4.4.1/otter/cli.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.4.0/otter/execute/__init__.py` & `otter-grader-4.4.1/otter/execute/__init__.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.4.0/otter/execute/checker.py` & `otter-grader-4.4.1/otter/execute/checker.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.4.0/otter/execute/execute_log.py` & `otter-grader-4.4.1/otter/execute/execute_log.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.4.0/otter/execute/execute_notebook.py` & `otter-grader-4.4.1/otter/execute/execute_notebook.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.4.0/otter/execute/transforms.py` & `otter-grader-4.4.1/otter/execute/transforms.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.4.0/otter/export/__init__.py` & `otter-grader-4.4.1/otter/export/__init__.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.4.0/otter/export/exporters/__init__.py` & `otter-grader-4.4.1/otter/export/exporters/__init__.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.4.0/otter/export/exporters/base_exporter.py` & `otter-grader-4.4.1/otter/export/exporters/base_exporter.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.4.0/otter/export/exporters/templates/via_html/index.html.j2` & `otter-grader-4.4.1/otter/export/exporters/templates/via_html/index.html.j2`

 * *Files identical despite different names*

### Comparing `otter-grader-4.4.0/otter/export/exporters/templates/via_html.tpl` & `otter-grader-4.4.1/otter/export/exporters/templates/via_html.tpl`

 * *Files identical despite different names*

### Comparing `otter-grader-4.4.0/otter/export/exporters/templates/via_latex/index.tex.j2` & `otter-grader-4.4.1/otter/export/exporters/templates/via_latex/index.tex.j2`

 * *Files identical despite different names*

### Comparing `otter-grader-4.4.0/otter/export/exporters/templates/via_latex.tpl` & `otter-grader-4.4.1/otter/export/exporters/templates/via_latex.tpl`

 * *Files identical despite different names*

### Comparing `otter-grader-4.4.0/otter/export/exporters/templates/via_latex_xecjk/index.tex.j2` & `otter-grader-4.4.1/otter/export/exporters/templates/via_latex_xecjk/index.tex.j2`

 * *Files identical despite different names*

### Comparing `otter-grader-4.4.0/otter/export/exporters/templates/via_latex_xecjk.tpl` & `otter-grader-4.4.1/otter/export/exporters/templates/via_latex_xecjk.tpl`

 * *Files identical despite different names*

### Comparing `otter-grader-4.4.0/otter/export/exporters/utils.py` & `otter-grader-4.4.1/otter/export/exporters/utils.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.4.0/otter/export/exporters/via_html.py` & `otter-grader-4.4.1/otter/export/exporters/via_html.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.4.0/otter/export/exporters/via_latex.py` & `otter-grader-4.4.1/otter/export/exporters/via_latex.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.4.0/otter/generate/__init__.py` & `otter-grader-4.4.1/otter/generate/__init__.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.4.0/otter/generate/templates/python/setup.sh` & `otter-grader-4.4.1/otter/generate/templates/python/setup.sh`

 * *Files identical despite different names*

### Comparing `otter-grader-4.4.0/otter/generate/templates/r/setup.sh` & `otter-grader-4.4.1/otter/generate/templates/r/setup.sh`

 * *Files identical despite different names*

### Comparing `otter-grader-4.4.0/otter/generate/token.py` & `otter-grader-4.4.1/otter/generate/token.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.4.0/otter/generate/utils.py` & `otter-grader-4.4.1/otter/generate/utils.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.4.0/otter/grade/Dockerfile` & `otter-grader-4.4.1/otter/grade/Dockerfile`

 * *Files identical despite different names*

### Comparing `otter-grader-4.4.0/otter/grade/__init__.py` & `otter-grader-4.4.1/otter/grade/__init__.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.4.0/otter/grade/containers.py` & `otter-grader-4.4.1/otter/grade/containers.py`

 * *Files 2% similar despite different names*

```diff
@@ -181,14 +181,21 @@
 
         if timeout:
             timer.cancel()
 
         logs = docker.container.logs(container)
         LOGGER.debug(f"Container {container_id} logs:\n{indent(logs, '    ')}")
 
+        # Close our file handles since docker cp will delete the original file when performing the
+        # copy.
+        os.close(temp_subm_file)
+        os.close(results_file)
+        if pdf_path:
+            os.close(pdf_file)
+
         for local_path, container_path in volumes:
             docker.container.copy((container, container_path), local_path)
 
         if not no_kill:
             container.remove()
 
         if exit != 0:
@@ -207,16 +214,13 @@
         if pdfs:
             os.makedirs(pdf_dir, exist_ok=True)
 
             local_pdf_path = os.path.join(pdf_dir, f"{nb_name}.pdf")
             shutil.copy(pdf_path, local_pdf_path)
 
     finally:
-        os.close(results_file)
         os.remove(results_path)
-        os.close(temp_subm_file)
         os.remove(temp_subm_path)
         if pdfs:
-            os.close(pdf_file)
             os.remove(pdf_path)
 
     return df
```

### Comparing `otter-grader-4.4.0/otter/grade/utils.py` & `otter-grader-4.4.1/otter/grade/utils.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.4.0/otter/plugins/__init__.py` & `otter-grader-4.4.1/otter/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.4.0/otter/plugins/abstract_plugin.py` & `otter-grader-4.4.1/otter/plugins/abstract_plugin.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.4.0/otter/plugins/builtin/gmail_notifications/__init__.py` & `otter-grader-4.4.1/otter/plugins/builtin/gmail_notifications/__init__.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.4.0/otter/plugins/builtin/gmail_notifications/bin/gmail_oauth2.py` & `otter-grader-4.4.1/otter/plugins/builtin/gmail_notifications/bin/gmail_oauth2.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.4.0/otter/plugins/builtin/grade_override.py` & `otter-grader-4.4.1/otter/plugins/builtin/grade_override.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.4.0/otter/plugins/builtin/rate_limiting.py` & `otter-grader-4.4.1/otter/plugins/builtin/rate_limiting.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.4.0/otter/run/__init__.py` & `otter-grader-4.4.1/otter/run/__init__.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.4.0/otter/run/run_autograder/__init__.py` & `otter-grader-4.4.1/otter/run/run_autograder/__init__.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.4.0/otter/run/run_autograder/autograder_config.py` & `otter-grader-4.4.1/otter/run/run_autograder/autograder_config.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.4.0/otter/run/run_autograder/runners/__init__.py` & `otter-grader-4.4.1/otter/run/run_autograder/runners/__init__.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.4.0/otter/run/run_autograder/runners/abstract_runner.py` & `otter-grader-4.4.1/otter/run/run_autograder/runners/abstract_runner.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.4.0/otter/run/run_autograder/runners/python_runner.py` & `otter-grader-4.4.1/otter/run/run_autograder/runners/python_runner.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.4.0/otter/run/run_autograder/runners/r_runner.py` & `otter-grader-4.4.1/otter/run/run_autograder/runners/r_runner.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.4.0/otter/test_files/__init__.py` & `otter-grader-4.4.1/otter/test_files/__init__.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.4.0/otter/test_files/abstract_test.py` & `otter-grader-4.4.1/otter/test_files/abstract_test.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.4.0/otter/test_files/exception_test.py` & `otter-grader-4.4.1/otter/test_files/exception_test.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.4.0/otter/test_files/metadata_test.py` & `otter-grader-4.4.1/otter/test_files/metadata_test.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.4.0/otter/test_files/ok_test.py` & `otter-grader-4.4.1/otter/test_files/ok_test.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.4.0/otter/utils.py` & `otter-grader-4.4.1/otter/utils.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.4.0/otter/version.py` & `otter-grader-4.4.1/otter/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Version and printable logo"""
 
 import sys
 
 from textwrap import dedent
 
 
-__version__ = "4.4.0"
+__version__ = "4.4.1"
 
 
 LOGO_WITH_VERSION = fr"""
   _________        __          __               
  /  _____  \    __|  |__    __|  |__               
 |  /     \  |  |__    __|  |__    __|   _______    _  _____
 | |       | |     |  |        |  |     |  ___  |  | |/ ____|
```

### Comparing `otter-grader-4.4.0/otter_grader.egg-info/PKG-INFO` & `otter-grader-4.4.1/otter_grader.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: otter-grader
-Version: 4.4.0
+Version: 4.4.1
 Summary: Python and Jupyter Notebook autograder
 Home-page: https://github.com/ucbds-infra/otter-grader
 Author: Christopher Pyles
 Author-email: otter-grader@berkeley.edu
 License: BSD-3-Clause
 Description: # Otter-Grader
```

### Comparing `otter-grader-4.4.0/otter_grader.egg-info/SOURCES.txt` & `otter-grader-4.4.1/otter_grader.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `otter-grader-4.4.0/setup.py` & `otter-grader-4.4.1/setup.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.4.0/test/test_assign.py` & `otter-grader-4.4.1/test/test_assign.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.4.0/test/test_check.py` & `otter-grader-4.4.1/test/test_check.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.4.0/test/test_export.py` & `otter-grader-4.4.1/test/test_export.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.4.0/test/test_generate/test_autograder.py` & `otter-grader-4.4.1/test/test_generate/test_autograder.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.4.0/test/test_generate/test_token.py` & `otter-grader-4.4.1/test/test_generate/test_token.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.4.0/test/test_grade.py` & `otter-grader-4.4.1/test/test_grade.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.4.0/test/test_logs.py` & `otter-grader-4.4.1/test/test_logs.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.4.0/test/test_notebook.py` & `otter-grader-4.4.1/test/test_notebook.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.4.0/test/test_run.py` & `otter-grader-4.4.1/test/test_run.py`

 * *Files identical despite different names*

