# Comparing `tmp/pretty-jupyter-2.0.4.tar.gz` & `tmp/pretty-jupyter-2.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pretty-jupyter-2.0.4.tar", last modified: Sun Dec 18 21:55:35 2022, max compression
+gzip compressed data, was "pretty-jupyter-2.0.5.tar", last modified: Sat Jul  8 17:07:30 2023, max compression
```

## Comparing `pretty-jupyter-2.0.4.tar` & `pretty-jupyter-2.0.5.tar`

### file list

```diff
@@ -1,82 +1,81 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-18 21:55:35.914096 pretty-jupyter-2.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)    35151 2022-12-18 21:55:23.000000 pretty-jupyter-2.0.4/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)      144 2022-12-18 21:55:23.000000 pretty-jupyter-2.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3417 2022-12-18 21:55:35.914096 pretty-jupyter-2.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2319 2022-12-18 21:55:23.000000 pretty-jupyter-2.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       99 2022-12-18 21:55:23.000000 pretty-jupyter-2.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     3687 2022-12-18 21:55:35.914096 pretty-jupyter-2.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       37 2022-12-18 21:55:23.000000 pretty-jupyter-2.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-18 21:55:35.894096 pretty-jupyter-2.0.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-18 21:55:35.898096 pretty-jupyter-2.0.4/src/pretty_jupyter/
--rw-r--r--   0 runner    (1001) docker     (123)      499 2022-12-18 21:55:23.000000 pretty-jupyter-2.0.4/src/pretty_jupyter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       76 2022-12-18 21:55:23.000000 pretty-jupyter-2.0.4/src/pretty_jupyter/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-18 21:55:35.894096 pretty-jupyter-2.0.4/src/pretty_jupyter/config/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-18 21:55:35.898096 pretty-jupyter-2.0.4/src/pretty_jupyter/config/metadata/
--rw-r--r--   0 runner    (1001) docker     (123)      167 2022-12-18 21:55:23.000000 pretty-jupyter-2.0.4/src/pretty_jupyter/config/metadata/cell_spec.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      423 2022-12-18 21:55:23.000000 pretty-jupyter-2.0.4/src/pretty_jupyter/config/metadata/nb_defaults.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2022-12-18 21:55:23.000000 pretty-jupyter-2.0.4/src/pretty_jupyter/config/metadata/nb_spec.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2967 2022-12-18 21:55:23.000000 pretty-jupyter-2.0.4/src/pretty_jupyter/console.py
--rw-r--r--   0 runner    (1001) docker     (123)     1829 2022-12-18 21:55:23.000000 pretty-jupyter-2.0.4/src/pretty_jupyter/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-18 21:55:35.898096 pretty-jupyter-2.0.4/src/pretty_jupyter/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)      188 2022-12-18 21:55:23.000000 pretty-jupyter-2.0.4/src/pretty_jupyter/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3198 2022-12-18 21:55:23.000000 pretty-jupyter-2.0.4/src/pretty_jupyter/helpers/matplotlib.py
--rw-r--r--   0 runner    (1001) docker     (123)     2352 2022-12-18 21:55:23.000000 pretty-jupyter-2.0.4/src/pretty_jupyter/magics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-18 21:55:35.898096 pretty-jupyter-2.0.4/src/pretty_jupyter/preprocessors/
--rw-r--r--   0 runner    (1001) docker     (123)      356 2022-12-18 21:55:23.000000 pretty-jupyter-2.0.4/src/pretty_jupyter/preprocessors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10423 2022-12-18 21:55:23.000000 pretty-jupyter-2.0.4/src/pretty_jupyter/preprocessors/_metadata_preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2051 2022-12-18 21:55:23.000000 pretty-jupyter-2.0.4/src/pretty_jupyter/preprocessors/_token_preprocessor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-18 21:55:35.898096 pretty-jupyter-2.0.4/src/pretty_jupyter/quickstart/
--rw-r--r--   0 runner    (1001) docker     (123)      660 2022-12-18 21:55:23.000000 pretty-jupyter-2.0.4/src/pretty_jupyter/quickstart/empty.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-18 21:55:35.894096 pretty-jupyter-2.0.4/src/pretty_jupyter/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-18 21:55:35.902096 pretty-jupyter-2.0.4/src/pretty_jupyter/templates/pj/
--rw-r--r--   0 runner    (1001) docker     (123)     5507 2022-12-18 21:55:23.000000 pretty-jupyter-2.0.4/src/pretty_jupyter/templates/pj/base.html.j2
--rw-r--r--   0 runner    (1001) docker     (123)      464 2022-12-18 21:55:23.000000 pretty-jupyter-2.0.4/src/pretty_jupyter/templates/pj/conf.json
--rw-r--r--   0 runner    (1001) docker     (123)     7411 2022-12-18 21:55:23.000000 pretty-jupyter-2.0.4/src/pretty_jupyter/templates/pj/index.html.j2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-18 21:55:35.902096 pretty-jupyter-2.0.4/src/pretty_jupyter/templates/pj/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-18 21:55:35.906096 pretty-jupyter-2.0.4/src/pretty_jupyter/templates/pj/static/libs/
--rw-r--r--   0 runner    (1001) docker     (123)    36816 2022-12-18 21:55:23.000000 pretty-jupyter-2.0.4/src/pretty_jupyter/templates/pj/static/libs/bootstrap.min.js
--rw-r--r--   0 runner    (1001) docker     (123)   240427 2022-12-18 21:55:23.000000 pretty-jupyter-2.0.4/src/pretty_jupyter/templates/pj/static/libs/jquery-ui.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    89501 2022-12-18 21:55:23.000000 pretty-jupyter-2.0.4/src/pretty_jupyter/templates/pj/static/libs/jquery.min.js
--rw-r--r--   0 runner    (1001) docker     (123)     4564 2022-12-18 21:55:23.000000 pretty-jupyter-2.0.4/src/pretty_jupyter/templates/pj/static/libs/jquery.stickytabs.js
--rw-r--r--   0 runner    (1001) docker     (123)     1451 2022-12-18 21:55:23.000000 pretty-jupyter-2.0.4/src/pretty_jupyter/templates/pj/static/libs/jquery.tocify.css
--rw-r--r--   0 runner    (1001) docker     (123)    31746 2022-12-18 21:55:23.000000 pretty-jupyter-2.0.4/src/pretty_jupyter/templates/pj/static/libs/jquery.tocify.js
--rw-r--r--   0 runner    (1001) docker     (123)  3699622 2022-12-18 21:55:23.000000 pretty-jupyter-2.0.4/src/pretty_jupyter/templates/pj/static/libs/plotly.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    17493 2022-12-18 21:55:23.000000 pretty-jupyter-2.0.4/src/pretty_jupyter/templates/pj/static/libs/require.min.js
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2022-12-18 21:55:23.000000 pretty-jupyter-2.0.4/src/pretty_jupyter/templates/pj/static/pj-tabset.css
--rw-r--r--   0 runner    (1001) docker     (123)      864 2022-12-18 21:55:23.000000 pretty-jupyter-2.0.4/src/pretty_jupyter/templates/pj/static/pj-toc.css
--rw-r--r--   0 runner    (1001) docker     (123)     1592 2022-12-18 21:55:23.000000 pretty-jupyter-2.0.4/src/pretty_jupyter/templates/pj/static/pj.css
--rw-r--r--   0 runner    (1001) docker     (123)     8631 2022-12-18 21:55:23.000000 pretty-jupyter-2.0.4/src/pretty_jupyter/templates/pj/static/pj.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-18 21:55:35.914096 pretty-jupyter-2.0.4/src/pretty_jupyter/templates/pj/static/themes/
--rw-r--r--   0 runner    (1001) docker     (123)   122540 2022-12-18 21:55:23.000000 pretty-jupyter-2.0.4/src/pretty_jupyter/templates/pj/static/themes/bootstrap.css
--rw-r--r--   0 runner    (1001) docker     (123)   120091 2022-12-18 21:55:23.000000 pretty-jupyter-2.0.4/src/pretty_jupyter/templates/pj/static/themes/cerulean.css
--rw-r--r--   0 runner    (1001) docker     (123)   119783 2022-12-18 21:55:23.000000 pretty-jupyter-2.0.4/src/pretty_jupyter/templates/pj/static/themes/cosmo.css
--rw-r--r--   0 runner    (1001) docker     (123)   119814 2022-12-18 21:55:23.000000 pretty-jupyter-2.0.4/src/pretty_jupyter/templates/pj/static/themes/cyborg.css
--rw-r--r--   0 runner    (1001) docker     (123)   121640 2022-12-18 21:55:23.000000 pretty-jupyter-2.0.4/src/pretty_jupyter/templates/pj/static/themes/darkly.css
--rw-r--r--   0 runner    (1001) docker     (123)   121369 2022-12-18 21:55:23.000000 pretty-jupyter-2.0.4/src/pretty_jupyter/templates/pj/static/themes/flatly.css
--rw-r--r--   0 runner    (1001) docker     (123)   118680 2022-12-18 21:55:23.000000 pretty-jupyter-2.0.4/src/pretty_jupyter/templates/pj/static/themes/journal.css
--rw-r--r--   0 runner    (1001) docker     (123)   124446 2022-12-18 21:55:23.000000 pretty-jupyter-2.0.4/src/pretty_jupyter/templates/pj/static/themes/lumen.css
--rw-r--r--   0 runner    (1001) docker     (123)   132332 2022-12-18 21:55:23.000000 pretty-jupyter-2.0.4/src/pretty_jupyter/templates/pj/static/themes/paper.css
--rw-r--r--   0 runner    (1001) docker     (123)   118693 2022-12-18 21:55:23.000000 pretty-jupyter-2.0.4/src/pretty_jupyter/templates/pj/static/themes/readable.css
--rw-r--r--   0 runner    (1001) docker     (123)   118980 2022-12-18 21:55:23.000000 pretty-jupyter-2.0.4/src/pretty_jupyter/templates/pj/static/themes/sandstone.css
--rw-r--r--   0 runner    (1001) docker     (123)   120201 2022-12-18 21:55:23.000000 pretty-jupyter-2.0.4/src/pretty_jupyter/templates/pj/static/themes/simplex.css
--rw-r--r--   0 runner    (1001) docker     (123)   129015 2022-12-18 21:55:23.000000 pretty-jupyter-2.0.4/src/pretty_jupyter/templates/pj/static/themes/slate.css
--rw-r--r--   0 runner    (1001) docker     (123)   121514 2022-12-18 21:55:23.000000 pretty-jupyter-2.0.4/src/pretty_jupyter/templates/pj/static/themes/spacelab.css
--rw-r--r--   0 runner    (1001) docker     (123)   120746 2022-12-18 21:55:23.000000 pretty-jupyter-2.0.4/src/pretty_jupyter/templates/pj/static/themes/superhero.css
--rw-r--r--   0 runner    (1001) docker     (123)   117031 2022-12-18 21:55:23.000000 pretty-jupyter-2.0.4/src/pretty_jupyter/templates/pj/static/themes/united.css
--rw-r--r--   0 runner    (1001) docker     (123)   121880 2022-12-18 21:55:23.000000 pretty-jupyter-2.0.4/src/pretty_jupyter/templates/pj/static/themes/yeti.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-18 21:55:35.902096 pretty-jupyter-2.0.4/src/pretty_jupyter/templates/pj-legacy/
--rw-r--r--   0 runner    (1001) docker     (123)      105 2022-12-18 21:55:23.000000 pretty-jupyter-2.0.4/src/pretty_jupyter/templates/pj-legacy/conf.json
--rw-r--r--   0 runner    (1001) docker     (123)      779 2022-12-18 21:55:23.000000 pretty-jupyter-2.0.4/src/pretty_jupyter/templates/pj-legacy/index.html.j2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-18 21:55:35.902096 pretty-jupyter-2.0.4/src/pretty_jupyter/templates/pj-pdf/
--rw-r--r--   0 runner    (1001) docker     (123)      415 2022-12-18 21:55:23.000000 pretty-jupyter-2.0.4/src/pretty_jupyter/templates/pj-pdf/conf.json
--rw-r--r--   0 runner    (1001) docker     (123)     1331 2022-12-18 21:55:23.000000 pretty-jupyter-2.0.4/src/pretty_jupyter/templates/pj-pdf/index.tex.j2
--rw-r--r--   0 runner    (1001) docker     (123)      504 2022-12-18 21:55:23.000000 pretty-jupyter-2.0.4/src/pretty_jupyter/testing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1898 2022-12-18 21:55:23.000000 pretty-jupyter-2.0.4/src/pretty_jupyter/tokens.py
--rw-r--r--   0 runner    (1001) docker     (123)      645 2022-12-18 21:55:23.000000 pretty-jupyter-2.0.4/src/pretty_jupyter/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-18 21:55:35.898096 pretty-jupyter-2.0.4/src/pretty_jupyter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3417 2022-12-18 21:55:35.000000 pretty-jupyter-2.0.4/src/pretty_jupyter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2981 2022-12-18 21:55:35.000000 pretty-jupyter-2.0.4/src/pretty_jupyter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-18 21:55:35.000000 pretty-jupyter-2.0.4/src/pretty_jupyter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2022-12-18 21:55:35.000000 pretty-jupyter-2.0.4/src/pretty_jupyter.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       92 2022-12-18 21:55:35.000000 pretty-jupyter-2.0.4/src/pretty_jupyter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2022-12-18 21:55:35.000000 pretty-jupyter-2.0.4/src/pretty_jupyter.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 17:07:30.289288 pretty-jupyter-2.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    35151 2023-07-08 17:07:14.000000 pretty-jupyter-2.0.5/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-08 17:07:14.000000 pretty-jupyter-2.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    44075 2023-07-08 17:07:30.289288 pretty-jupyter-2.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-07-08 17:07:14.000000 pretty-jupyter-2.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-07-08 17:07:14.000000 pretty-jupyter-2.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2369 2023-07-08 17:07:30.293288 pretty-jupyter-2.0.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 17:07:30.277287 pretty-jupyter-2.0.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 17:07:30.277287 pretty-jupyter-2.0.5/src/pretty_jupyter/
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-07-08 17:07:14.000000 pretty-jupyter-2.0.5/src/pretty_jupyter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-08 17:07:14.000000 pretty-jupyter-2.0.5/src/pretty_jupyter/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 17:07:30.277287 pretty-jupyter-2.0.5/src/pretty_jupyter/config/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 17:07:30.277287 pretty-jupyter-2.0.5/src/pretty_jupyter/config/metadata/
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-07-08 17:07:14.000000 pretty-jupyter-2.0.5/src/pretty_jupyter/config/metadata/cell_spec.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-07-08 17:07:14.000000 pretty-jupyter-2.0.5/src/pretty_jupyter/config/metadata/nb_defaults.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-07-08 17:07:14.000000 pretty-jupyter-2.0.5/src/pretty_jupyter/config/metadata/nb_spec.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-07-08 17:07:14.000000 pretty-jupyter-2.0.5/src/pretty_jupyter/console.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-07-08 17:07:14.000000 pretty-jupyter-2.0.5/src/pretty_jupyter/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 17:07:30.277287 pretty-jupyter-2.0.5/src/pretty_jupyter/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-07-08 17:07:14.000000 pretty-jupyter-2.0.5/src/pretty_jupyter/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3265 2023-07-08 17:07:14.000000 pretty-jupyter-2.0.5/src/pretty_jupyter/helpers/matplotlib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-07-08 17:07:14.000000 pretty-jupyter-2.0.5/src/pretty_jupyter/magics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 17:07:30.281287 pretty-jupyter-2.0.5/src/pretty_jupyter/preprocessors/
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-07-08 17:07:14.000000 pretty-jupyter-2.0.5/src/pretty_jupyter/preprocessors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10669 2023-07-08 17:07:14.000000 pretty-jupyter-2.0.5/src/pretty_jupyter/preprocessors/_metadata_preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2055 2023-07-08 17:07:14.000000 pretty-jupyter-2.0.5/src/pretty_jupyter/preprocessors/_token_preprocessor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 17:07:30.281287 pretty-jupyter-2.0.5/src/pretty_jupyter/quickstart/
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-07-08 17:07:14.000000 pretty-jupyter-2.0.5/src/pretty_jupyter/quickstart/empty.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 17:07:30.277287 pretty-jupyter-2.0.5/src/pretty_jupyter/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 17:07:30.281287 pretty-jupyter-2.0.5/src/pretty_jupyter/templates/pj/
+-rw-r--r--   0 runner    (1001) docker     (123)     5507 2023-07-08 17:07:14.000000 pretty-jupyter-2.0.5/src/pretty_jupyter/templates/pj/base.html.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-07-08 17:07:14.000000 pretty-jupyter-2.0.5/src/pretty_jupyter/templates/pj/conf.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7517 2023-07-08 17:07:14.000000 pretty-jupyter-2.0.5/src/pretty_jupyter/templates/pj/index.html.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 17:07:30.281287 pretty-jupyter-2.0.5/src/pretty_jupyter/templates/pj/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 17:07:30.285287 pretty-jupyter-2.0.5/src/pretty_jupyter/templates/pj/static/libs/
+-rw-r--r--   0 runner    (1001) docker     (123)    36816 2023-07-08 17:07:14.000000 pretty-jupyter-2.0.5/src/pretty_jupyter/templates/pj/static/libs/bootstrap.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)   240427 2023-07-08 17:07:14.000000 pretty-jupyter-2.0.5/src/pretty_jupyter/templates/pj/static/libs/jquery-ui.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    89501 2023-07-08 17:07:14.000000 pretty-jupyter-2.0.5/src/pretty_jupyter/templates/pj/static/libs/jquery.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4564 2023-07-08 17:07:14.000000 pretty-jupyter-2.0.5/src/pretty_jupyter/templates/pj/static/libs/jquery.stickytabs.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-07-08 17:07:14.000000 pretty-jupyter-2.0.5/src/pretty_jupyter/templates/pj/static/libs/jquery.tocify.css
+-rw-r--r--   0 runner    (1001) docker     (123)    31746 2023-07-08 17:07:14.000000 pretty-jupyter-2.0.5/src/pretty_jupyter/templates/pj/static/libs/jquery.tocify.js
+-rw-r--r--   0 runner    (1001) docker     (123)  3699622 2023-07-08 17:07:15.000000 pretty-jupyter-2.0.5/src/pretty_jupyter/templates/pj/static/libs/plotly.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    17493 2023-07-08 17:07:15.000000 pretty-jupyter-2.0.5/src/pretty_jupyter/templates/pj/static/libs/require.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-07-08 17:07:15.000000 pretty-jupyter-2.0.5/src/pretty_jupyter/templates/pj/static/pj-tabset.css
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-07-08 17:07:15.000000 pretty-jupyter-2.0.5/src/pretty_jupyter/templates/pj/static/pj-toc.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-07-08 17:07:15.000000 pretty-jupyter-2.0.5/src/pretty_jupyter/templates/pj/static/pj.css
+-rw-r--r--   0 runner    (1001) docker     (123)     8677 2023-07-08 17:07:15.000000 pretty-jupyter-2.0.5/src/pretty_jupyter/templates/pj/static/pj.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 17:07:30.289288 pretty-jupyter-2.0.5/src/pretty_jupyter/templates/pj/static/themes/
+-rw-r--r--   0 runner    (1001) docker     (123)   122540 2023-07-08 17:07:15.000000 pretty-jupyter-2.0.5/src/pretty_jupyter/templates/pj/static/themes/bootstrap.css
+-rw-r--r--   0 runner    (1001) docker     (123)   120091 2023-07-08 17:07:15.000000 pretty-jupyter-2.0.5/src/pretty_jupyter/templates/pj/static/themes/cerulean.css
+-rw-r--r--   0 runner    (1001) docker     (123)   119783 2023-07-08 17:07:15.000000 pretty-jupyter-2.0.5/src/pretty_jupyter/templates/pj/static/themes/cosmo.css
+-rw-r--r--   0 runner    (1001) docker     (123)   119814 2023-07-08 17:07:15.000000 pretty-jupyter-2.0.5/src/pretty_jupyter/templates/pj/static/themes/cyborg.css
+-rw-r--r--   0 runner    (1001) docker     (123)   121640 2023-07-08 17:07:15.000000 pretty-jupyter-2.0.5/src/pretty_jupyter/templates/pj/static/themes/darkly.css
+-rw-r--r--   0 runner    (1001) docker     (123)   121369 2023-07-08 17:07:15.000000 pretty-jupyter-2.0.5/src/pretty_jupyter/templates/pj/static/themes/flatly.css
+-rw-r--r--   0 runner    (1001) docker     (123)   118680 2023-07-08 17:07:15.000000 pretty-jupyter-2.0.5/src/pretty_jupyter/templates/pj/static/themes/journal.css
+-rw-r--r--   0 runner    (1001) docker     (123)   124446 2023-07-08 17:07:15.000000 pretty-jupyter-2.0.5/src/pretty_jupyter/templates/pj/static/themes/lumen.css
+-rw-r--r--   0 runner    (1001) docker     (123)   132332 2023-07-08 17:07:15.000000 pretty-jupyter-2.0.5/src/pretty_jupyter/templates/pj/static/themes/paper.css
+-rw-r--r--   0 runner    (1001) docker     (123)   118693 2023-07-08 17:07:15.000000 pretty-jupyter-2.0.5/src/pretty_jupyter/templates/pj/static/themes/readable.css
+-rw-r--r--   0 runner    (1001) docker     (123)   118980 2023-07-08 17:07:15.000000 pretty-jupyter-2.0.5/src/pretty_jupyter/templates/pj/static/themes/sandstone.css
+-rw-r--r--   0 runner    (1001) docker     (123)   120201 2023-07-08 17:07:15.000000 pretty-jupyter-2.0.5/src/pretty_jupyter/templates/pj/static/themes/simplex.css
+-rw-r--r--   0 runner    (1001) docker     (123)   129015 2023-07-08 17:07:15.000000 pretty-jupyter-2.0.5/src/pretty_jupyter/templates/pj/static/themes/slate.css
+-rw-r--r--   0 runner    (1001) docker     (123)   121514 2023-07-08 17:07:15.000000 pretty-jupyter-2.0.5/src/pretty_jupyter/templates/pj/static/themes/spacelab.css
+-rw-r--r--   0 runner    (1001) docker     (123)   120746 2023-07-08 17:07:15.000000 pretty-jupyter-2.0.5/src/pretty_jupyter/templates/pj/static/themes/superhero.css
+-rw-r--r--   0 runner    (1001) docker     (123)   117031 2023-07-08 17:07:15.000000 pretty-jupyter-2.0.5/src/pretty_jupyter/templates/pj/static/themes/united.css
+-rw-r--r--   0 runner    (1001) docker     (123)   121880 2023-07-08 17:07:15.000000 pretty-jupyter-2.0.5/src/pretty_jupyter/templates/pj/static/themes/yeti.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 17:07:30.281287 pretty-jupyter-2.0.5/src/pretty_jupyter/templates/pj-legacy/
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-08 17:07:14.000000 pretty-jupyter-2.0.5/src/pretty_jupyter/templates/pj-legacy/conf.json
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-07-08 17:07:14.000000 pretty-jupyter-2.0.5/src/pretty_jupyter/templates/pj-legacy/index.html.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 17:07:30.281287 pretty-jupyter-2.0.5/src/pretty_jupyter/templates/pj-pdf/
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-07-08 17:07:14.000000 pretty-jupyter-2.0.5/src/pretty_jupyter/templates/pj-pdf/conf.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-07-08 17:07:14.000000 pretty-jupyter-2.0.5/src/pretty_jupyter/templates/pj-pdf/index.tex.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-07-08 17:07:15.000000 pretty-jupyter-2.0.5/src/pretty_jupyter/testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-07-08 17:07:15.000000 pretty-jupyter-2.0.5/src/pretty_jupyter/tokens.py
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-07-08 17:07:15.000000 pretty-jupyter-2.0.5/src/pretty_jupyter/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 17:07:30.277287 pretty-jupyter-2.0.5/src/pretty_jupyter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    44075 2023-07-08 17:07:30.000000 pretty-jupyter-2.0.5/src/pretty_jupyter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2972 2023-07-08 17:07:30.000000 pretty-jupyter-2.0.5/src/pretty_jupyter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 17:07:30.000000 pretty-jupyter-2.0.5/src/pretty_jupyter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-08 17:07:30.000000 pretty-jupyter-2.0.5/src/pretty_jupyter.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-07-08 17:07:30.000000 pretty-jupyter-2.0.5/src/pretty_jupyter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-08 17:07:30.000000 pretty-jupyter-2.0.5/src/pretty_jupyter.egg-info/top_level.txt
```

### Comparing `pretty-jupyter-2.0.4/LICENSE.md` & `pretty-jupyter-2.0.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pretty-jupyter-2.0.4/README.md` & `pretty-jupyter-2.0.5/README.md`

 * *Files identical despite different names*

### Comparing `pretty-jupyter-2.0.4/src/pretty_jupyter/config/metadata/nb_spec.yaml` & `pretty-jupyter-2.0.5/src/pretty_jupyter/config/metadata/nb_spec.yaml`

 * *Files 5% similar despite different names*

```diff
@@ -32,14 +32,16 @@
         toc_depth:
           type: integer
           min: 1
         toc_collapsed:
           type: boolean
         toc_smooth_scroll:
           type: boolean
+        toc_extend_page:
+          type: boolean
         number_sections:
           type: boolean
         code_folding:
           type: string
           allowed:
             - hide
             - show
```

### Comparing `pretty-jupyter-2.0.4/src/pretty_jupyter/console.py` & `pretty-jupyter-2.0.5/src/pretty_jupyter/console.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 import os
 import shutil
 import sys
+from pathlib import Path
+
 import click
-from traitlets.config import Config
-from nbconvert.exporters import HTMLExporter, PDFExporter, LatexExporter
 import pkg_resources
-from pathlib import Path
+from nbconvert.exporters import HTMLExporter, LatexExporter, PDFExporter
+from traitlets.config import Config
 
 
 @click.command()
 @click.argument("out_path", type=click.Path())
 def quickstart(out_path):
-    in_path = pkg_resources.resource_filename("pretty_jupyter", os.path.join("quickstart", "empty.ipynb"))
+    in_path = pkg_resources.resource_filename(
+        "pretty_jupyter", os.path.join("quickstart", "empty.ipynb")
+    )
 
     with open(in_path, "r") as file_r, open(out_path, "w") as file_w:
         in_text = file_r.read()
         file_w.write(in_text)
 
 
 @click.command("nbconvert-dev")
@@ -27,38 +30,36 @@
     """
     Takes the .ipynb notebook from the INPUT and transforms it into HTML.
     Note that after installing you can also use jupyter nbconvert directly.
     """
     if out is None:
         out = os.path.join(os.path.dirname(input), f"{Path(input).stem}.{to}")
 
-    template_map = {
-        "html": "pj",
-        "pdf": "pj-pdf",
-        "latex": "pj-pdf"
-    }
+    template_map = {"html": "pj", "pdf": "pj-pdf", "latex": "pj-pdf"}
 
-    config =  Config()
+    config = Config()
     config.TemplateExporter.template_name = template_map[to]
-    config.TemplateExporter.extra_template_basedirs = [pkg_resources.resource_filename("pretty_jupyter", "templates")]
+    config.TemplateExporter.extra_template_basedirs = [
+        pkg_resources.resource_filename("pretty_jupyter", "templates")
+    ]
     config.TemplateExporter.exclude_input = not include_input
 
     if to == "html":
         exporter = HTMLExporter(config)
     elif to == "pdf":
         exporter = PDFExporter(config)
     elif to == "latex":
         exporter = LatexExporter(config)
     else:
         raise ValueError()
 
     with open(input, "r", encoding="utf-8") as file:
         res = exporter.from_file(file)
     output_data = res[0]
-    
+
     # open file as bytes if the output data are bytes, otherwise opne it as a string
     file = open(out, "wb") if isinstance(output_data, bytes) else open(out, "w", encoding="utf-8")
     try:
         file.write(output_data)
     finally:
         file.close()
 
@@ -67,24 +68,27 @@
 def install_dev():
     """
     Installs this package and makes it callable by `jupyter nbconvert` without the need to specify extra_template_basedirs.
     """
     src_templates = ["pj", "pj-pdf", "pj-legacy"]
 
     for src_template in src_templates:
-        src_folder = os.path.join(pkg_resources.resource_filename("pretty_jupyter", "templates"), src_template)
-        target_folder = os.path.join(sys.prefix, f"share/jupyter/nbconvert/templates/{src_template}")
+        src_folder = os.path.join(
+            pkg_resources.resource_filename("pretty_jupyter", "templates"), src_template
+        )
+        target_folder = os.path.join(
+            sys.prefix, f"share/jupyter/nbconvert/templates/{src_template}"
+        )
 
         # for backward compatibility, otherwise copytree has dirs_exist_ok param
         if os.path.exists(target_folder):
             shutil.rmtree(target_folder)
         shutil.copytree(src_folder, target_folder)
 
 
-
 @click.version_option()
 @click.group()
 def cli():
     pass
 
 
 cli.add_command(quickstart)
```

### Comparing `pretty-jupyter-2.0.4/src/pretty_jupyter/constants.py` & `pretty-jupyter-2.0.5/src/pretty_jupyter/constants.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,15 +58,15 @@
     "readable",
     "sandstone",
     "simplex",
     "slate",
     "spacelab",
     "superhero",
     "united",
-    "yeti"
+    "yeti",
 ]
 """
 List of all available local themes that can be specified in the `theme` html metadata.
 """
 
 DEPRECATED_METADATA_MSG_FORMAT = "Specifying attributes '{attributes}' in this position to notebook metadata is deprecated since {version}. Please consider reading changes in this version.\n"
-METADATA_ERROR_FORMAT = "An error occured when validating cell metadata. Error attributes in the metadata were the following:\n{error}"
+METADATA_ERROR_FORMAT = "An error occured when validating cell metadata. Error attributes in the metadata were the following:\n{error}"
```

### Comparing `pretty-jupyter-2.0.4/src/pretty_jupyter/helpers/matplotlib.py` & `pretty-jupyter-2.0.5/src/pretty_jupyter/helpers/matplotlib.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,200 +1,205 @@
-00000000: 6672 6f6d 2069 6f20 696d 706f 7274 2042  from io import B
-00000010: 7974 6573 494f 0a69 6d70 6f72 7420 6261  ytesIO.import ba
-00000020: 7365 3634 0a0a 5f4d 4152 4b44 4f57 4e5f  se64.._MARKDOWN_
+00000000: 696d 706f 7274 2062 6173 6536 340a 6672  import base64.fr
+00000010: 6f6d 2069 6f20 696d 706f 7274 2042 7974  om io import Byt
+00000020: 6573 494f 0a0a 5f4d 4152 4b44 4f57 4e5f  esIO.._MARKDOWN_
 00000030: 5355 5050 4f52 5445 445f 464d 545f 4d41  SUPPORTED_FMT_MA
-00000040: 5020 3d20 7b0a 2020 2020 2270 6e67 223a  P = {.    "png":
-00000050: 2022 706e 6722 2c0a 2020 2020 226a 7065   "png",.    "jpe
-00000060: 6722 3a20 226a 7065 6722 2c0a 2020 2020  g": "jpeg",.    
-00000070: 226a 7067 223a 2022 6a70 6567 220a 7d0a  "jpg": "jpeg".}.
-00000080: 5f4d 4152 4b44 4f57 4e5f 494d 475f 464f  _MARKDOWN_IMG_FO
-00000090: 524d 4154 203d 2072 2221 5b69 6d61 6765  RMAT = r"![image
-000000a0: 5d28 6461 7461 3a69 6d61 6765 2f7b 666f  ](data:image/{fo
-000000b0: 726d 6174 7d3b 6261 7365 3634 2c7b 656e  rmat};base64,{en
-000000c0: 636f 6465 647d 2922 0a0a 5f48 544d 4c5f  coded})".._HTML_
-000000d0: 5355 5050 4f52 5445 445f 464d 545f 4d41  SUPPORTED_FMT_MA
-000000e0: 5020 3d20 7b0a 2020 2020 2273 7667 223a  P = {.    "svg":
-000000f0: 2022 7376 672b 786d 6c22 2c20 0a20 2020   "svg+xml", .   
-00000100: 2022 706e 6722 3a20 2270 6e67 222c 0a20   "png": "png",. 
-00000110: 2020 2022 6a70 6567 223a 2022 6a70 6567     "jpeg": "jpeg
-00000120: 222c 0a20 2020 2022 6a70 6722 3a20 226a  ",.    "jpg": "j
-00000130: 7065 6722 0a7d 0a5f 4854 4d4c 5f49 4d47  peg".}._HTML_IMG
-00000140: 5f46 4f52 4d41 5420 3d20 7222 3c69 6d67  _FORMAT = r"<img
-00000150: 2073 7263 3d27 6461 7461 3a69 6d61 6765   src='data:image
-00000160: 2f7b 666f 726d 6174 7d3b 6261 7365 3634  /{format};base64
-00000170: 2c7b 656e 636f 6465 647d 2720 2f3e 220a  ,{encoded}' />".
-00000180: 0a0a 6465 6620 6d61 7470 6c6f 746c 6962  ..def matplotlib
-00000190: 5f66 6967 5f74 6f5f 6d61 726b 646f 776e  _fig_to_markdown
-000001a0: 2866 6967 2c20 666d 743d 2270 6e67 222c  (fig, fmt="png",
-000001b0: 2061 7574 6f63 6c6f 7365 3a20 626f 6f6c   autoclose: bool
-000001c0: 203d 2054 7275 652c 2062 626f 785f 696e   = True, bbox_in
-000001d0: 6368 6573 3a20 7374 7220 3d20 2274 6967  ches: str = "tig
-000001e0: 6874 2229 3a0a 2020 2020 2222 220a 2020  ht"):.    """.  
-000001f0: 2020 436f 6e76 6572 7473 206d 6174 706c    Converts matpl
-00000200: 6f74 6c69 6220 6669 6775 7265 2074 6f20  otlib figure to 
-00000210: 656d 6265 6464 6564 206d 6172 6b64 6f77  embedded markdow
-00000220: 6e20 696d 6167 652e 0a0a 2020 2020 4172  n image...    Ar
-00000230: 6773 3a0a 2020 2020 2020 2020 6669 673a  gs:.        fig:
-00000240: 204d 6174 706c 6f74 6c69 6220 6669 6775   Matplotlib figu
-00000250: 7265 2e0a 2020 2020 2020 2020 666d 7420  re..        fmt 
-00000260: 2873 7472 2c20 6f70 7469 6f6e 616c 293a  (str, optional):
-00000270: 2046 6f72 6d61 7420 6f66 2074 6865 206f   Format of the o
-00000280: 7574 7075 7420 696d 6167 652e 2053 7570  utput image. Sup
-00000290: 706f 7274 6564 2076 616c 7565 7320 6172  ported values ar
-000002a0: 653a 2070 6e67 2061 6e64 206a 7067 2e20  e: png and jpg. 
-000002b0: 4465 6661 756c 7473 2074 6f20 2270 6e67  Defaults to "png
-000002c0: 222e 0a20 2020 2020 2020 2061 7574 6f63  "..        autoc
-000002d0: 6c6f 7365 2028 626f 6f6c 293a 2049 6620  lose (bool): If 
-000002e0: 7472 7565 2c20 7468 656e 206d 6174 706c  true, then matpl
-000002f0: 6f74 6c69 6220 676c 6f62 616c 2070 6c6f  otlib global plo
-00000300: 7420 6973 2063 6c6f 7365 642e 2054 6869  t is closed. Thi
-00000310: 7320 7072 6576 656e 7473 2069 7420 6672  s prevents it fr
-00000320: 6f6d 2062 6569 6e67 2066 6c75 7368 6564  om being flushed
-00000330: 2062 7920 4a75 7079 7465 7220 6e6f 7465   by Jupyter note
-00000340: 626f 6f6b 2e20 4465 6661 756c 7473 2074  book. Defaults t
-00000350: 6f20 5472 7565 2e0a 2020 2020 2020 2020  o True..        
-00000360: 6262 6f78 5f69 6e63 6865 7320 2873 7472  bbox_inches (str
-00000370: 293a 2050 6172 616d 6574 6572 2073 656e  ): Parameter sen
-00000380: 7420 746f 2073 6176 6566 6967 2e20 4465  t to savefig. De
-00000390: 6661 756c 7473 2074 6f20 2274 6967 6874  faults to "tight
-000003a0: 222e 0a0a 2020 2020 5265 7475 726e 733a  "...    Returns:
-000003b0: 0a20 2020 2020 2020 2073 7472 3a20 4d61  .        str: Ma
-000003c0: 726b 646f 776e 2073 7472 696e 6720 656d  rkdown string em
-000003d0: 6265 6464 6564 2072 6570 7265 7365 6e74  bedded represent
-000003e0: 6174 696f 6e20 6f66 2074 6865 2066 6967  ation of the fig
-000003f0: 7572 652e 0a20 2020 2022 2222 0a20 2020  ure..    """.   
-00000400: 2072 6574 7572 6e20 636f 6e76 6572 745f   return convert_
-00000410: 6d70 6c28 6669 672c 2066 6d74 3d66 6d74  mpl(fig, fmt=fmt
-00000420: 2c20 6f75 7470 7574 5f66 6d74 5f73 7472  , output_fmt_str
-00000430: 696e 673d 5f4d 4152 4b44 4f57 4e5f 494d  ing=_MARKDOWN_IM
-00000440: 475f 464f 524d 4154 2c20 7375 7070 6f72  G_FORMAT, suppor
+00000040: 5020 3d20 7b22 706e 6722 3a20 2270 6e67  P = {"png": "png
+00000050: 222c 2022 6a70 6567 223a 2022 6a70 6567  ", "jpeg": "jpeg
+00000060: 222c 2022 6a70 6722 3a20 226a 7065 6722  ", "jpg": "jpeg"
+00000070: 7d0a 5f4d 4152 4b44 4f57 4e5f 494d 475f  }._MARKDOWN_IMG_
+00000080: 464f 524d 4154 203d 2072 2221 5b69 6d61  FORMAT = r"![ima
+00000090: 6765 5d28 6461 7461 3a69 6d61 6765 2f7b  ge](data:image/{
+000000a0: 666f 726d 6174 7d3b 6261 7365 3634 2c7b  format};base64,{
+000000b0: 656e 636f 6465 647d 2922 0a0a 5f48 544d  encoded})".._HTM
+000000c0: 4c5f 5355 5050 4f52 5445 445f 464d 545f  L_SUPPORTED_FMT_
+000000d0: 4d41 5020 3d20 7b22 7376 6722 3a20 2273  MAP = {"svg": "s
+000000e0: 7667 2b78 6d6c 222c 2022 706e 6722 3a20  vg+xml", "png": 
+000000f0: 2270 6e67 222c 2022 6a70 6567 223a 2022  "png", "jpeg": "
+00000100: 6a70 6567 222c 2022 6a70 6722 3a20 226a  jpeg", "jpg": "j
+00000110: 7065 6722 7d0a 5f48 544d 4c5f 494d 475f  peg"}._HTML_IMG_
+00000120: 464f 524d 4154 203d 2072 223c 696d 6720  FORMAT = r"<img 
+00000130: 7372 633d 2764 6174 613a 696d 6167 652f  src='data:image/
+00000140: 7b66 6f72 6d61 747d 3b62 6173 6536 342c  {format};base64,
+00000150: 7b65 6e63 6f64 6564 7d27 202f 3e22 0a0a  {encoded}' />"..
+00000160: 0a64 6566 206d 6174 706c 6f74 6c69 625f  .def matplotlib_
+00000170: 6669 675f 746f 5f6d 6172 6b64 6f77 6e28  fig_to_markdown(
+00000180: 6669 672c 2066 6d74 3d22 706e 6722 2c20  fig, fmt="png", 
+00000190: 6175 746f 636c 6f73 653a 2062 6f6f 6c20  autoclose: bool 
+000001a0: 3d20 5472 7565 2c20 6262 6f78 5f69 6e63  = True, bbox_inc
+000001b0: 6865 733a 2073 7472 203d 2022 7469 6768  hes: str = "tigh
+000001c0: 7422 293a 0a20 2020 2022 2222 0a20 2020  t"):.    """.   
+000001d0: 2043 6f6e 7665 7274 7320 6d61 7470 6c6f   Converts matplo
+000001e0: 746c 6962 2066 6967 7572 6520 746f 2065  tlib figure to e
+000001f0: 6d62 6564 6465 6420 6d61 726b 646f 776e  mbedded markdown
+00000200: 2069 6d61 6765 2e0a 0a20 2020 2041 7267   image...    Arg
+00000210: 733a 0a20 2020 2020 2020 2066 6967 3a20  s:.        fig: 
+00000220: 4d61 7470 6c6f 746c 6962 2066 6967 7572  Matplotlib figur
+00000230: 652e 0a20 2020 2020 2020 2066 6d74 2028  e..        fmt (
+00000240: 7374 722c 206f 7074 696f 6e61 6c29 3a20  str, optional): 
+00000250: 466f 726d 6174 206f 6620 7468 6520 6f75  Format of the ou
+00000260: 7470 7574 2069 6d61 6765 2e20 5375 7070  tput image. Supp
+00000270: 6f72 7465 6420 7661 6c75 6573 2061 7265  orted values are
+00000280: 3a20 706e 6720 616e 6420 6a70 672e 2044  : png and jpg. D
+00000290: 6566 6175 6c74 7320 746f 2022 706e 6722  efaults to "png"
+000002a0: 2e0a 2020 2020 2020 2020 6175 746f 636c  ..        autocl
+000002b0: 6f73 6520 2862 6f6f 6c29 3a20 4966 2074  ose (bool): If t
+000002c0: 7275 652c 2074 6865 6e20 6d61 7470 6c6f  rue, then matplo
+000002d0: 746c 6962 2067 6c6f 6261 6c20 706c 6f74  tlib global plot
+000002e0: 2069 7320 636c 6f73 6564 2e20 5468 6973   is closed. This
+000002f0: 2070 7265 7665 6e74 7320 6974 2066 726f   prevents it fro
+00000300: 6d20 6265 696e 6720 666c 7573 6865 6420  m being flushed 
+00000310: 6279 204a 7570 7974 6572 206e 6f74 6562  by Jupyter noteb
+00000320: 6f6f 6b2e 2044 6566 6175 6c74 7320 746f  ook. Defaults to
+00000330: 2054 7275 652e 0a20 2020 2020 2020 2062   True..        b
+00000340: 626f 785f 696e 6368 6573 2028 7374 7229  box_inches (str)
+00000350: 3a20 5061 7261 6d65 7465 7220 7365 6e74  : Parameter sent
+00000360: 2074 6f20 7361 7665 6669 672e 2044 6566   to savefig. Def
+00000370: 6175 6c74 7320 746f 2022 7469 6768 7422  aults to "tight"
+00000380: 2e0a 0a20 2020 2052 6574 7572 6e73 3a0a  ...    Returns:.
+00000390: 2020 2020 2020 2020 7374 723a 204d 6172          str: Mar
+000003a0: 6b64 6f77 6e20 7374 7269 6e67 2065 6d62  kdown string emb
+000003b0: 6564 6465 6420 7265 7072 6573 656e 7461  edded representa
+000003c0: 7469 6f6e 206f 6620 7468 6520 6669 6775  tion of the figu
+000003d0: 7265 2e0a 2020 2020 2222 220a 2020 2020  re..    """.    
+000003e0: 7265 7475 726e 2063 6f6e 7665 7274 5f6d  return convert_m
+000003f0: 706c 280a 2020 2020 2020 2020 6669 672c  pl(.        fig,
+00000400: 0a20 2020 2020 2020 2066 6d74 3d66 6d74  .        fmt=fmt
+00000410: 2c0a 2020 2020 2020 2020 6f75 7470 7574  ,.        output
+00000420: 5f66 6d74 5f73 7472 696e 673d 5f4d 4152  _fmt_string=_MAR
+00000430: 4b44 4f57 4e5f 494d 475f 464f 524d 4154  KDOWN_IMG_FORMAT
+00000440: 2c0a 2020 2020 2020 2020 7375 7070 6f72  ,.        suppor
 00000450: 7465 645f 666d 745f 6d61 703d 5f4d 4152  ted_fmt_map=_MAR
 00000460: 4b44 4f57 4e5f 5355 5050 4f52 5445 445f  KDOWN_SUPPORTED_
-00000470: 464d 545f 4d41 502c 2061 7574 6f63 6c6f  FMT_MAP, autoclo
-00000480: 7365 3d61 7574 6f63 6c6f 7365 2c20 6262  se=autoclose, bb
-00000490: 6f78 5f69 6e63 6865 733d 6262 6f78 5f69  ox_inches=bbox_i
-000004a0: 6e63 6865 7329 0a0a 6465 6620 6d61 7470  nches)..def matp
-000004b0: 6c6f 746c 6962 5f66 6967 5f74 6f5f 6874  lotlib_fig_to_ht
-000004c0: 6d6c 2866 6967 2c20 666d 743d 2270 6e67  ml(fig, fmt="png
-000004d0: 222c 2061 7574 6f63 6c6f 7365 3a20 626f  ", autoclose: bo
-000004e0: 6f6c 203d 2054 7275 652c 2062 626f 785f  ol = True, bbox_
-000004f0: 696e 6368 6573 3a20 7374 7220 3d20 2274  inches: str = "t
-00000500: 6967 6874 2229 3a0a 2020 2020 2222 220a  ight"):.    """.
-00000510: 2020 2020 436f 6e76 6572 7473 206d 6174      Converts mat
-00000520: 706c 6f74 6c69 6220 6669 6775 7265 2074  plotlib figure t
-00000530: 6f20 656d 6265 6464 6564 2068 746d 6c20  o embedded html 
-00000540: 696d 6167 652e 0a0a 2020 2020 4172 6773  image...    Args
-00000550: 3a0a 2020 2020 2020 2020 6669 673a 204d  :.        fig: M
-00000560: 6174 706c 6f74 6c69 6220 6669 6775 7265  atplotlib figure
-00000570: 2e0a 2020 2020 2020 2020 666d 7420 2873  ..        fmt (s
-00000580: 7472 2c20 6f70 7469 6f6e 616c 293a 2046  tr, optional): F
-00000590: 6f72 6d61 7420 6f66 2074 6865 206f 7574  ormat of the out
-000005a0: 7075 7420 696d 6167 652e 2053 7570 706f  put image. Suppo
-000005b0: 7274 6564 2076 616c 7565 7320 6172 653a  rted values are:
-000005c0: 2070 6e67 2c20 6a70 6720 616e 6420 7376   png, jpg and sv
-000005d0: 672e 2044 6566 6175 6c74 7320 746f 2022  g. Defaults to "
-000005e0: 706e 6722 2e0a 2020 2020 2020 2020 6175  png"..        au
-000005f0: 746f 636c 6f73 6520 2862 6f6f 6c29 3a20  toclose (bool): 
-00000600: 4966 2074 7275 652c 2074 6865 6e20 6d61  If true, then ma
-00000610: 7470 6c6f 746c 6962 2067 6c6f 6261 6c20  tplotlib global 
-00000620: 706c 6f74 2069 7320 636c 6f73 6564 2e20  plot is closed. 
-00000630: 5468 6973 2070 7265 7665 6e74 7320 6974  This prevents it
-00000640: 2066 726f 6d20 6265 696e 6720 666c 7573   from being flus
-00000650: 6865 6420 6279 204a 7570 7974 6572 206e  hed by Jupyter n
-00000660: 6f74 6562 6f6f 6b2e 2044 6566 6175 6c74  otebook. Default
-00000670: 7320 746f 2054 7275 652e 0a20 2020 2020  s to True..     
-00000680: 2020 2062 626f 785f 696e 6368 6573 2028     bbox_inches (
-00000690: 7374 7229 3a20 5061 7261 6d65 7465 7220  str): Parameter 
-000006a0: 7365 6e74 2074 6f20 7361 7665 6669 672e  sent to savefig.
-000006b0: 2044 6566 6175 6c74 7320 746f 2022 7469   Defaults to "ti
-000006c0: 6768 7422 2e0a 0a20 2020 2052 6574 7572  ght"...    Retur
-000006d0: 6e73 3a0a 2020 2020 2020 2020 7374 723a  ns:.        str:
-000006e0: 204d 6172 6b64 6f77 6e20 7374 7269 6e67   Markdown string
-000006f0: 2065 6d62 6564 6465 6420 7265 7072 6573   embedded repres
-00000700: 656e 7461 7469 6f6e 206f 6620 7468 6520  entation of the 
-00000710: 6669 6775 7265 2e0a 2020 2020 2222 220a  figure..    """.
-00000720: 2020 2020 7265 7475 726e 2063 6f6e 7665      return conve
-00000730: 7274 5f6d 706c 2866 6967 2c20 666d 742c  rt_mpl(fig, fmt,
-00000740: 205f 4854 4d4c 5f49 4d47 5f46 4f52 4d41   _HTML_IMG_FORMA
-00000750: 542c 205f 4854 4d4c 5f53 5550 504f 5254  T, _HTML_SUPPORT
-00000760: 4544 5f46 4d54 5f4d 4150 2c20 6175 746f  ED_FMT_MAP, auto
-00000770: 636c 6f73 652c 2062 626f 785f 696e 6368  close, bbox_inch
-00000780: 6573 290a 0a64 6566 2063 6f6e 7665 7274  es)..def convert
-00000790: 5f6d 706c 2866 6967 2c20 666d 742c 206f  _mpl(fig, fmt, o
-000007a0: 7574 7075 745f 666d 745f 7374 7269 6e67  utput_fmt_string
-000007b0: 2c20 7375 7070 6f72 7465 645f 666d 745f  , supported_fmt_
-000007c0: 6d61 702c 2061 7574 6f63 6c6f 7365 3a20  map, autoclose: 
-000007d0: 626f 6f6c 203d 2054 7275 652c 2062 626f  bool = True, bbo
-000007e0: 785f 696e 6368 6573 3a20 7374 7220 3d20  x_inches: str = 
-000007f0: 2274 6967 6874 2229 3a0a 2020 2020 2222  "tight"):.    ""
-00000800: 220a 2020 2020 436f 6e76 6572 7473 206d  ".    Converts m
-00000810: 6174 706c 6f74 6c69 6220 6669 6775 7265  atplotlib figure
-00000820: 2069 6e74 6f20 656d 6265 6464 6564 2069   into embedded i
-00000830: 6e6c 696e 6520 7374 7269 6e67 2e0a 0a20  nline string... 
-00000840: 2020 2041 7267 733a 0a20 2020 2020 2020     Args:.       
-00000850: 2066 6967 3a20 4d61 7470 6c6f 746c 6962   fig: Matplotlib
-00000860: 2066 6967 7572 652e 0a20 2020 2020 2020   figure..       
-00000870: 2066 6d74 2028 7374 7229 3a20 466f 726d   fmt (str): Form
-00000880: 6174 206f 6620 7468 6520 6f75 7470 7574  at of the output
-00000890: 2028 706e 672c 206a 7067 2c2e 2e2e 292e   (png, jpg,...).
-000008a0: 0a20 2020 2020 2020 206f 7574 7075 745f  .        output_
-000008b0: 666d 745f 7374 7269 6e67 2028 7374 7229  fmt_string (str)
-000008c0: 3a20 5374 7269 6e67 2066 6f72 6d61 7420  : String format 
-000008d0: 6f66 2074 6865 206f 7574 7075 742e 2049  of the output. I
-000008e0: 7420 6d75 7374 2068 6176 6520 7477 6f20  t must have two 
-000008f0: 656d 7074 7920 666f 726d 6174 2073 7472  empty format str
-00000900: 696e 6773 2074 6f20 7370 6563 6966 792c  ings to specify,
-00000910: 2077 6865 7265 206f 6e65 2069 7320 6e61   where one is na
-00000920: 6d65 6420 666f 726d 6174 2061 6e64 2074  med format and t
-00000930: 6865 2073 6563 6f6e 6420 6973 206e 616d  he second is nam
-00000940: 6564 2065 6e63 6f64 6564 2e0a 2020 2020  ed encoded..    
-00000950: 2020 2020 7375 7070 6f72 7465 645f 666d      supported_fm
-00000960: 745f 6d61 7020 2864 6963 7429 3a20 4d61  t_map (dict): Ma
-00000970: 7073 2073 7570 706f 7274 6564 2066 6f72  ps supported for
-00000980: 6d61 7473 2074 6f20 7468 6520 666f 726d  mats to the form
-00000990: 6174 2075 7365 6420 696e 2074 6865 2e0a  at used in the..
-000009a0: 2020 2020 2020 2020 6175 746f 636c 6f73          autoclos
-000009b0: 6520 2862 6f6f 6c29 3a20 4966 2074 7275  e (bool): If tru
-000009c0: 652c 2074 6865 6e20 6d61 7470 6c6f 746c  e, then matplotl
-000009d0: 6962 2067 6c6f 6261 6c20 706c 6f74 2069  ib global plot i
-000009e0: 7320 636c 6f73 6564 2e20 5468 6973 2070  s closed. This p
-000009f0: 7265 7665 6e74 7320 6974 2066 726f 6d20  revents it from 
-00000a00: 6265 696e 6720 666c 7573 6865 6420 6279  being flushed by
-00000a10: 204a 7570 7974 6572 206e 6f74 6562 6f6f   Jupyter noteboo
-00000a20: 6b2e 2044 6566 6175 6c74 7320 746f 2054  k. Defaults to T
-00000a30: 7275 652e 0a20 2020 2020 2020 2062 626f  rue..        bbo
-00000a40: 785f 696e 6368 6573 2028 7374 7229 3a20  x_inches (str): 
-00000a50: 5061 7261 6d65 7465 7220 7365 6e74 2074  Parameter sent t
-00000a60: 6f20 7361 7665 6669 672e 2044 6566 6175  o savefig. Defau
-00000a70: 6c74 7320 746f 2022 7469 6768 7422 2e0a  lts to "tight"..
-00000a80: 0a20 2020 2052 6574 7572 6e73 3a0a 2020  .    Returns:.  
-00000a90: 2020 2020 2020 7374 723a 2052 6574 7572        str: Retur
-00000aa0: 6e73 2073 7472 696e 6720 7265 7072 6573  ns string repres
-00000ab0: 656e 7461 7469 6f6e 206f 6620 7468 6520  entation of the 
-00000ac0: 6669 6775 7265 2e0a 2020 2020 2222 220a  figure..    """.
-00000ad0: 2020 2020 6966 2066 6d74 206e 6f74 2069      if fmt not i
-00000ae0: 6e20 7375 7070 6f72 7465 645f 666d 745f  n supported_fmt_
-00000af0: 6d61 703a 0a20 2020 2020 2020 2072 6169  map:.        rai
-00000b00: 7365 2056 616c 7565 4572 726f 7228 2246  se ValueError("F
-00000b10: 6f72 6d61 7420 277b 666f 726d 6174 7d27  ormat '{format}'
-00000b20: 2069 7320 6375 7272 656e 746c 7920 6e6f   is currently no
-00000b30: 7420 7375 7070 6f72 7465 642e 2229 0a0a  t supported.")..
-00000b40: 2020 2020 746d 7066 696c 6520 3d20 4279      tmpfile = By
-00000b50: 7465 7349 4f28 290a 2020 2020 6669 672e  tesIO().    fig.
-00000b60: 7361 7665 6669 6728 746d 7066 696c 652c  savefig(tmpfile,
-00000b70: 2066 6f72 6d61 743d 666d 742c 2062 626f   format=fmt, bbo
-00000b80: 785f 696e 6368 6573 3d62 626f 785f 696e  x_inches=bbox_in
-00000b90: 6368 6573 290a 0a20 2020 206d 6172 6b64  ches)..    markd
-00000ba0: 6f77 6e20 3d20 6f75 7470 7574 5f66 6d74  own = output_fmt
-00000bb0: 5f73 7472 696e 672e 666f 726d 6174 2866  _string.format(f
-00000bc0: 6f72 6d61 743d 7375 7070 6f72 7465 645f  ormat=supported_
-00000bd0: 666d 745f 6d61 705b 666d 745d 2c20 656e  fmt_map[fmt], en
-00000be0: 636f 6465 643d 6261 7365 3634 2e62 3634  coded=base64.b64
-00000bf0: 656e 636f 6465 2874 6d70 6669 6c65 2e67  encode(tmpfile.g
-00000c00: 6574 7661 6c75 6528 2929 2e64 6563 6f64  etvalue()).decod
-00000c10: 6528 2775 7466 2d38 2729 290a 0a20 2020  e('utf-8'))..   
-00000c20: 2069 6620 6175 746f 636c 6f73 653a 0a20   if autoclose:. 
-00000c30: 2020 2020 2020 2069 6d70 6f72 7420 6d61         import ma
-00000c40: 7470 6c6f 746c 6962 2e70 7970 6c6f 7420  tplotlib.pyplot 
-00000c50: 6173 2070 6c74 0a20 2020 2020 2020 2070  as plt.        p
-00000c60: 6c74 2e63 6c6f 7365 2829 0a20 2020 2072  lt.close().    r
-00000c70: 6574 7572 6e20 6d61 726b 646f 776e       eturn markdown
+00000470: 464d 545f 4d41 502c 0a20 2020 2020 2020  FMT_MAP,.       
+00000480: 2061 7574 6f63 6c6f 7365 3d61 7574 6f63   autoclose=autoc
+00000490: 6c6f 7365 2c0a 2020 2020 2020 2020 6262  lose,.        bb
+000004a0: 6f78 5f69 6e63 6865 733d 6262 6f78 5f69  ox_inches=bbox_i
+000004b0: 6e63 6865 732c 0a20 2020 2029 0a0a 0a64  nches,.    )...d
+000004c0: 6566 206d 6174 706c 6f74 6c69 625f 6669  ef matplotlib_fi
+000004d0: 675f 746f 5f68 746d 6c28 6669 672c 2066  g_to_html(fig, f
+000004e0: 6d74 3d22 706e 6722 2c20 6175 746f 636c  mt="png", autocl
+000004f0: 6f73 653a 2062 6f6f 6c20 3d20 5472 7565  ose: bool = True
+00000500: 2c20 6262 6f78 5f69 6e63 6865 733a 2073  , bbox_inches: s
+00000510: 7472 203d 2022 7469 6768 7422 293a 0a20  tr = "tight"):. 
+00000520: 2020 2022 2222 0a20 2020 2043 6f6e 7665     """.    Conve
+00000530: 7274 7320 6d61 7470 6c6f 746c 6962 2066  rts matplotlib f
+00000540: 6967 7572 6520 746f 2065 6d62 6564 6465  igure to embedde
+00000550: 6420 6874 6d6c 2069 6d61 6765 2e0a 0a20  d html image... 
+00000560: 2020 2041 7267 733a 0a20 2020 2020 2020     Args:.       
+00000570: 2066 6967 3a20 4d61 7470 6c6f 746c 6962   fig: Matplotlib
+00000580: 2066 6967 7572 652e 0a20 2020 2020 2020   figure..       
+00000590: 2066 6d74 2028 7374 722c 206f 7074 696f   fmt (str, optio
+000005a0: 6e61 6c29 3a20 466f 726d 6174 206f 6620  nal): Format of 
+000005b0: 7468 6520 6f75 7470 7574 2069 6d61 6765  the output image
+000005c0: 2e20 5375 7070 6f72 7465 6420 7661 6c75  . Supported valu
+000005d0: 6573 2061 7265 3a20 706e 672c 206a 7067  es are: png, jpg
+000005e0: 2061 6e64 2073 7667 2e20 4465 6661 756c   and svg. Defaul
+000005f0: 7473 2074 6f20 2270 6e67 222e 0a20 2020  ts to "png"..   
+00000600: 2020 2020 2061 7574 6f63 6c6f 7365 2028       autoclose (
+00000610: 626f 6f6c 293a 2049 6620 7472 7565 2c20  bool): If true, 
+00000620: 7468 656e 206d 6174 706c 6f74 6c69 6220  then matplotlib 
+00000630: 676c 6f62 616c 2070 6c6f 7420 6973 2063  global plot is c
+00000640: 6c6f 7365 642e 2054 6869 7320 7072 6576  losed. This prev
+00000650: 656e 7473 2069 7420 6672 6f6d 2062 6569  ents it from bei
+00000660: 6e67 2066 6c75 7368 6564 2062 7920 4a75  ng flushed by Ju
+00000670: 7079 7465 7220 6e6f 7465 626f 6f6b 2e20  pyter notebook. 
+00000680: 4465 6661 756c 7473 2074 6f20 5472 7565  Defaults to True
+00000690: 2e0a 2020 2020 2020 2020 6262 6f78 5f69  ..        bbox_i
+000006a0: 6e63 6865 7320 2873 7472 293a 2050 6172  nches (str): Par
+000006b0: 616d 6574 6572 2073 656e 7420 746f 2073  ameter sent to s
+000006c0: 6176 6566 6967 2e20 4465 6661 756c 7473  avefig. Defaults
+000006d0: 2074 6f20 2274 6967 6874 222e 0a0a 2020   to "tight"...  
+000006e0: 2020 5265 7475 726e 733a 0a20 2020 2020    Returns:.     
+000006f0: 2020 2073 7472 3a20 4d61 726b 646f 776e     str: Markdown
+00000700: 2073 7472 696e 6720 656d 6265 6464 6564   string embedded
+00000710: 2072 6570 7265 7365 6e74 6174 696f 6e20   representation 
+00000720: 6f66 2074 6865 2066 6967 7572 652e 0a20  of the figure.. 
+00000730: 2020 2022 2222 0a20 2020 2072 6574 7572     """.    retur
+00000740: 6e20 636f 6e76 6572 745f 6d70 6c28 6669  n convert_mpl(fi
+00000750: 672c 2066 6d74 2c20 5f48 544d 4c5f 494d  g, fmt, _HTML_IM
+00000760: 475f 464f 524d 4154 2c20 5f48 544d 4c5f  G_FORMAT, _HTML_
+00000770: 5355 5050 4f52 5445 445f 464d 545f 4d41  SUPPORTED_FMT_MA
+00000780: 502c 2061 7574 6f63 6c6f 7365 2c20 6262  P, autoclose, bb
+00000790: 6f78 5f69 6e63 6865 7329 0a0a 0a64 6566  ox_inches)...def
+000007a0: 2063 6f6e 7665 7274 5f6d 706c 280a 2020   convert_mpl(.  
+000007b0: 2020 6669 672c 0a20 2020 2066 6d74 2c0a    fig,.    fmt,.
+000007c0: 2020 2020 6f75 7470 7574 5f66 6d74 5f73      output_fmt_s
+000007d0: 7472 696e 672c 0a20 2020 2073 7570 706f  tring,.    suppo
+000007e0: 7274 6564 5f66 6d74 5f6d 6170 2c0a 2020  rted_fmt_map,.  
+000007f0: 2020 6175 746f 636c 6f73 653a 2062 6f6f    autoclose: boo
+00000800: 6c20 3d20 5472 7565 2c0a 2020 2020 6262  l = True,.    bb
+00000810: 6f78 5f69 6e63 6865 733a 2073 7472 203d  ox_inches: str =
+00000820: 2022 7469 6768 7422 2c0a 293a 0a20 2020   "tight",.):.   
+00000830: 2022 2222 0a20 2020 2043 6f6e 7665 7274   """.    Convert
+00000840: 7320 6d61 7470 6c6f 746c 6962 2066 6967  s matplotlib fig
+00000850: 7572 6520 696e 746f 2065 6d62 6564 6465  ure into embedde
+00000860: 6420 696e 6c69 6e65 2073 7472 696e 672e  d inline string.
+00000870: 0a0a 2020 2020 4172 6773 3a0a 2020 2020  ..    Args:.    
+00000880: 2020 2020 6669 673a 204d 6174 706c 6f74      fig: Matplot
+00000890: 6c69 6220 6669 6775 7265 2e0a 2020 2020  lib figure..    
+000008a0: 2020 2020 666d 7420 2873 7472 293a 2046      fmt (str): F
+000008b0: 6f72 6d61 7420 6f66 2074 6865 206f 7574  ormat of the out
+000008c0: 7075 7420 2870 6e67 2c20 6a70 672c 2e2e  put (png, jpg,..
+000008d0: 2e29 2e0a 2020 2020 2020 2020 6f75 7470  .)..        outp
+000008e0: 7574 5f66 6d74 5f73 7472 696e 6720 2873  ut_fmt_string (s
+000008f0: 7472 293a 2053 7472 696e 6720 666f 726d  tr): String form
+00000900: 6174 206f 6620 7468 6520 6f75 7470 7574  at of the output
+00000910: 2e20 4974 206d 7573 7420 6861 7665 2074  . It must have t
+00000920: 776f 2065 6d70 7479 2066 6f72 6d61 7420  wo empty format 
+00000930: 7374 7269 6e67 7320 746f 2073 7065 6369  strings to speci
+00000940: 6679 2c20 7768 6572 6520 6f6e 6520 6973  fy, where one is
+00000950: 206e 616d 6564 2066 6f72 6d61 7420 616e   named format an
+00000960: 6420 7468 6520 7365 636f 6e64 2069 7320  d the second is 
+00000970: 6e61 6d65 6420 656e 636f 6465 642e 0a20  named encoded.. 
+00000980: 2020 2020 2020 2073 7570 706f 7274 6564         supported
+00000990: 5f66 6d74 5f6d 6170 2028 6469 6374 293a  _fmt_map (dict):
+000009a0: 204d 6170 7320 7375 7070 6f72 7465 6420   Maps supported 
+000009b0: 666f 726d 6174 7320 746f 2074 6865 2066  formats to the f
+000009c0: 6f72 6d61 7420 7573 6564 2069 6e20 7468  ormat used in th
+000009d0: 652e 0a20 2020 2020 2020 2061 7574 6f63  e..        autoc
+000009e0: 6c6f 7365 2028 626f 6f6c 293a 2049 6620  lose (bool): If 
+000009f0: 7472 7565 2c20 7468 656e 206d 6174 706c  true, then matpl
+00000a00: 6f74 6c69 6220 676c 6f62 616c 2070 6c6f  otlib global plo
+00000a10: 7420 6973 2063 6c6f 7365 642e 2054 6869  t is closed. Thi
+00000a20: 7320 7072 6576 656e 7473 2069 7420 6672  s prevents it fr
+00000a30: 6f6d 2062 6569 6e67 2066 6c75 7368 6564  om being flushed
+00000a40: 2062 7920 4a75 7079 7465 7220 6e6f 7465   by Jupyter note
+00000a50: 626f 6f6b 2e20 4465 6661 756c 7473 2074  book. Defaults t
+00000a60: 6f20 5472 7565 2e0a 2020 2020 2020 2020  o True..        
+00000a70: 6262 6f78 5f69 6e63 6865 7320 2873 7472  bbox_inches (str
+00000a80: 293a 2050 6172 616d 6574 6572 2073 656e  ): Parameter sen
+00000a90: 7420 746f 2073 6176 6566 6967 2e20 4465  t to savefig. De
+00000aa0: 6661 756c 7473 2074 6f20 2274 6967 6874  faults to "tight
+00000ab0: 222e 0a0a 2020 2020 5265 7475 726e 733a  "...    Returns:
+00000ac0: 0a20 2020 2020 2020 2073 7472 3a20 5265  .        str: Re
+00000ad0: 7475 726e 7320 7374 7269 6e67 2072 6570  turns string rep
+00000ae0: 7265 7365 6e74 6174 696f 6e20 6f66 2074  resentation of t
+00000af0: 6865 2066 6967 7572 652e 0a20 2020 2022  he figure..    "
+00000b00: 2222 0a20 2020 2069 6620 666d 7420 6e6f  "".    if fmt no
+00000b10: 7420 696e 2073 7570 706f 7274 6564 5f66  t in supported_f
+00000b20: 6d74 5f6d 6170 3a0a 2020 2020 2020 2020  mt_map:.        
+00000b30: 7261 6973 6520 5661 6c75 6545 7272 6f72  raise ValueError
+00000b40: 2822 466f 726d 6174 2027 7b66 6f72 6d61  ("Format '{forma
+00000b50: 747d 2720 6973 2063 7572 7265 6e74 6c79  t}' is currently
+00000b60: 206e 6f74 2073 7570 706f 7274 6564 2e22   not supported."
+00000b70: 290a 0a20 2020 2074 6d70 6669 6c65 203d  )..    tmpfile =
+00000b80: 2042 7974 6573 494f 2829 0a20 2020 2066   BytesIO().    f
+00000b90: 6967 2e73 6176 6566 6967 2874 6d70 6669  ig.savefig(tmpfi
+00000ba0: 6c65 2c20 666f 726d 6174 3d66 6d74 2c20  le, format=fmt, 
+00000bb0: 6262 6f78 5f69 6e63 6865 733d 6262 6f78  bbox_inches=bbox
+00000bc0: 5f69 6e63 6865 7329 0a0a 2020 2020 6d61  _inches)..    ma
+00000bd0: 726b 646f 776e 203d 206f 7574 7075 745f  rkdown = output_
+00000be0: 666d 745f 7374 7269 6e67 2e66 6f72 6d61  fmt_string.forma
+00000bf0: 7428 0a20 2020 2020 2020 2066 6f72 6d61  t(.        forma
+00000c00: 743d 7375 7070 6f72 7465 645f 666d 745f  t=supported_fmt_
+00000c10: 6d61 705b 666d 745d 2c20 656e 636f 6465  map[fmt], encode
+00000c20: 643d 6261 7365 3634 2e62 3634 656e 636f  d=base64.b64enco
+00000c30: 6465 2874 6d70 6669 6c65 2e67 6574 7661  de(tmpfile.getva
+00000c40: 6c75 6528 2929 2e64 6563 6f64 6528 2275  lue()).decode("u
+00000c50: 7466 2d38 2229 0a20 2020 2029 0a0a 2020  tf-8").    )..  
+00000c60: 2020 6966 2061 7574 6f63 6c6f 7365 3a0a    if autoclose:.
+00000c70: 2020 2020 2020 2020 696d 706f 7274 206d          import m
+00000c80: 6174 706c 6f74 6c69 622e 7079 706c 6f74  atplotlib.pyplot
+00000c90: 2061 7320 706c 740a 0a20 2020 2020 2020   as plt..       
+00000ca0: 2070 6c74 2e63 6c6f 7365 2829 0a20 2020   plt.close().   
+00000cb0: 2072 6574 7572 6e20 6d61 726b 646f 776e   return markdown
+00000cc0: 0a                                       .
```

### Comparing `pretty-jupyter-2.0.4/src/pretty_jupyter/magics.py` & `pretty-jupyter-2.0.5/src/pretty_jupyter/magics.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,57 +1,65 @@
-from IPython import display
-from IPython.core.magic import Magics, magics_class, cell_magic
 import jinja2
+from IPython import display
+from IPython.core.magic import Magics, cell_magic, magics_class
 
 from pretty_jupyter.tokens import convert_markdown_tokens_to_html
 
 
 @magics_class
 class JinjaMagics(Magics):
     def __init__(self, shell):
         super().__init__(shell)
-        
+
         # create a jinja2 environment to use for rendering
         # this can be modified for desired effects (ie: using different variable syntax)
-        self.env = jinja2.Environment(loader=jinja2.FileSystemLoader('.'))
+        self.env = jinja2.Environment(loader=jinja2.FileSystemLoader("."))
 
         # possible output types
-        self.display_functions = dict(html=display.HTML, 
-                                      latex=display.Latex,
-                                      json=display.JSON,
-                                      pretty=display.Pretty,
-                                      display=display.display,
-                                      markdown=display.Markdown)
+        self.display_functions = dict(
+            html=display.HTML,
+            latex=display.Latex,
+            json=display.JSON,
+            pretty=display.Pretty,
+            display=display.display,
+            markdown=display.Markdown,
+        )
 
     @cell_magic
     def jinja(self, line, cell):
         display_fn_name = line.lower().strip()
         if display_fn_name not in self.display_functions:
             raise ValueError(f"Unknown parameter {display_fn_name}.")
 
         display_fn = self.display_functions.get(display_fn_name)
 
         # render the cell with jinja (substitutes variables,...)
         tmp = self.env.from_string(cell)
-        rend = tmp.render(dict((k,v) for (k,v) in self.shell.user_ns.items() 
-                                        if not k.startswith('_') and k not in self.shell.user_ns_hidden))
-        
+        rend = tmp.render(
+            dict(
+                (k, v)
+                for (k, v) in self.shell.user_ns.items()
+                if not k.startswith("_") and k not in self.shell.user_ns_hidden
+            )
+        )
+
         # convert tokens to html
         if display_fn_name == "markdown":
             rend = convert_markdown_tokens_to_html(rend)
 
         # display markdown
         return display_fn(rend)
 
     @cell_magic
     def jmd(self, line, cell):
         if len(line.strip()) > 0:
             raise ValueError(r"%%jmd does not accept any arguments.")
         return self.jinja(line="markdown", cell=cell)
 
+
 def is_jinja_cell(input_str: str) -> bool:
     """
     Checks whether the input is input of a jinja cell.
 
     Args:
         input_str (str): Input.
 
@@ -60,13 +68,10 @@
     """
     lines = input_str.splitlines()
 
     if len(lines) == 0:
         return False
 
     first_line = lines[0]
-    fns = [
-        lambda l: l.startswith("%%jinja"),
-        lambda l: l.startswith("%%jmd")
-    ]
+    fns = [lambda l: l.startswith("%%jinja"), lambda l: l.startswith("%%jmd")]
 
-    return any(fn(first_line) for fn in fns)
+    return any(fn(first_line) for fn in fns)
```

### Comparing `pretty-jupyter-2.0.4/src/pretty_jupyter/preprocessors/_metadata_preprocessor.py` & `pretty-jupyter-2.0.5/src/pretty_jupyter/preprocessors/_metadata_preprocessor.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,30 @@
 import copy
-import os
 import warnings
-from pretty_jupyter.constants import DEPRECATED_METADATA_MSG_FORMAT, CONFIG_DIR, AVAILABLE_THEMES, METADATA_ERROR_FORMAT
 from datetime import date, datetime
-from nbconvert.preprocessors import Preprocessor
-from traitlets import Dict
-from pretty_jupyter.utils import merge_dict
 from pathlib import Path
-from cerberus import Validator
-import yaml
-import nbconvert
-from packaging import version
-import pkg_resources
 
 import jinja2
+import nbconvert
+import pkg_resources
+import yaml
+from cerberus import Validator
+from nbconvert.preprocessors import Preprocessor
+from packaging import version
+from traitlets import Dict
 
-from pretty_jupyter.tokens import read_code_metadata_token, read_markdown_metadata_token
+from pretty_jupyter.constants import (
+    AVAILABLE_THEMES,
+    CONFIG_DIR,
+    DEPRECATED_METADATA_MSG_FORMAT,
+    METADATA_ERROR_FORMAT,
+)
 from pretty_jupyter.magics import is_jinja_cell
+from pretty_jupyter.tokens import read_code_metadata_token, read_markdown_metadata_token
+from pretty_jupyter.utils import merge_dict
 
 _DEPRECATED_ATTRIBUTES = ["title", "theme", "toc", "code_folding"]
 _DEPRECATED_ATTRIBUTES_VERSION = "2.0.0"
 
 
 class NbMetadataPreprocessor(Preprocessor):
     """
@@ -42,15 +46,15 @@
     def __init__(self, **kw):
         if "pj_metadata" in kw and isinstance(kw["pj_metadata"], str):
             # convert to dictionary
             kw["pj_metadata"] = yaml.safe_load(kw["pj_metadata"])
 
         super().__init__(**kw)
 
-        self.env = jinja2.Environment(loader=jinja2.FileSystemLoader('.'))
+        self.env = jinja2.Environment(loader=jinja2.FileSystemLoader("."))
 
         with open(self.nb_spec_path) as file:
             nb_spec = yaml.safe_load(file.read())
         self.nb_validator = Validator(nb_spec, allow_unknown=True)
 
         with open(self.cell_spec_path) as file:
             cell_spec = yaml.safe_load(file.read())
@@ -60,15 +64,20 @@
             nb_defaults = yaml.safe_load(file.read())
         self.defaults = nb_defaults
 
     def preprocess(self, nb, resources):
         # deprecation warnings to help users fix their error
         deprecated_attrs = [a for a in _DEPRECATED_ATTRIBUTES if a in nb.metadata]
         if len(deprecated_attrs) > 0:
-            warnings.warn(DEPRECATED_METADATA_MSG_FORMAT.format(attributes=", ".join(deprecated_attrs), version=_DEPRECATED_ATTRIBUTES_VERSION), category=DeprecationWarning)
+            warnings.warn(
+                DEPRECATED_METADATA_MSG_FORMAT.format(
+                    attributes=", ".join(deprecated_attrs), version=_DEPRECATED_ATTRIBUTES_VERSION
+                ),
+                category=DeprecationWarning,
+            )
 
         # temporarily store nb metadata to resources to be accessible in cell
         resources["__pj_metadata"] = nb.metadata.get("pj_metadata", {})
         return super().preprocess(nb, resources)
 
     def preprocess_cell(self, cell, resources, index):
         """
@@ -83,30 +92,35 @@
             self._synchronize_notebook_metadata(cell, resources)
 
         self._synchronize_cell_metadata(cell)
         if cell.cell_type == "markdown":
             cell, resources = self._preprocess_markdown_cell(cell, resources, index)
         if cell.cell_type == "code":
             cell, resources = self._preprocess_code_cell(cell, resources, index)
-        
+
         return cell, resources
 
     def _synchronize_notebook_metadata(self, cell, resources):
         nb_metadata = resources.get("__pj_metadata", {})
         src_metadata = {}
         if cell.cell_type == "raw":
             try:
                 src_metadata = yaml.safe_load(cell.source)
             except Exception as exc:
-                raise ValueError("An error happend when trying to parse first cell of the notebook with type raw.", exc)
+                raise ValueError(
+                    "An error happend when trying to parse first cell of the notebook with type raw.",
+                    exc,
+                )
 
             remove_cell_input(cell)
 
         if len(nb_metadata) > 0 and len(src_metadata) > 0:
-            warnings.warn("Notebook-level metadata are defined both in the source and in the notebook's metadata. Please remove one of them.")
+            warnings.warn(
+                "Notebook-level metadata are defined both in the source and in the notebook's metadata. Please remove one of them."
+            )
 
         metadata = src_metadata if len(src_metadata) > 0 else nb_metadata
 
         # validate metadata
         is_valid = self.nb_validator.validate(metadata)
         if not is_valid:
             raise ValueError(METADATA_ERROR_FORMAT.format(error=str(self.nb_validator.errors)))
@@ -117,16 +131,20 @@
         # 2. Values specified by user in notebook metadata
         # 3. Default values from NbMetadataProcessor.defaults
         metadata = merge_dict(self.pj_metadata, metadata)
         metadata = merge_dict(metadata, self.defaults)
 
         # run metadata through jinja templating
         metadata_copy = copy.deepcopy(metadata)
-        for m_key, m_val in filter(lambda x: x[1] is not None and isinstance(x[1], str), metadata_copy.items()):
-            metadata[m_key] = self.env.from_string(m_val).render(datetime=datetime, date=date, pj_metadata=metadata_copy)
+        for m_key, m_val in filter(
+            lambda x: x[1] is not None and isinstance(x[1], str), metadata_copy.items()
+        ):
+            metadata[m_key] = self.env.from_string(m_val).render(
+                datetime=datetime, date=date, pj_metadata=metadata_copy
+            )
 
         resources["pj_metadata"] = metadata
 
         del resources["__pj_metadata"]
 
     def _synchronize_cell_metadata(self, cell):
         """
@@ -175,15 +193,15 @@
         # if metadata specify that input shouldnt be enabled => remove it
         if not is_input_enabled(cell, resources):
             remove_cell_input(cell)
 
         for i, output in reversed(list(enumerate(cell.outputs))):
             if not is_output_enabled(cell, resources, output):
                 cell.outputs.pop(i)
-        
+
         return cell, resources
 
 
 class HtmlNbMetadataPreprocessor(NbMetadataPreprocessor):
     def preprocess(self, nb, resources):
         resources["pj_available_themes"] = AVAILABLE_THEMES
         return super().preprocess(nb, resources)
@@ -204,16 +222,19 @@
 
 def is_output_enabled(cell, resources, output):
     cell_metadata = cell.metadata["pj_metadata"]
     nb_metadata = resources["pj_metadata"]["output"]["general"]
 
     def is_stdout(output):
         return output.output_type == "stream" and output.name == "stdout"
+
     def is_error(output):
-        return output.output_type == "error" or (output.output_type == "stream" and output.name == "stderr")
+        return output.output_type == "error" or (
+            output.output_type == "stream" and output.name == "stderr"
+        )
 
     # PRIORITY
     # cell > notebook-level, stdout > output (similarly stderr)
     # we will set a default as the most general setting and then progressively overwrite it by more specific settings
     # least specific: notebook-level output
     # most specific: stdout/stderr cell output
 
@@ -231,14 +252,15 @@
         is_enabled = cell_metadata["output_stdout"]
     # STDERR
     if is_error(output) and "output_error" in cell_metadata:
         is_enabled = cell_metadata["output_error"]
 
     return is_enabled
 
+
 def is_input_enabled(cell, resources):
     cell_metadata = cell.metadata["pj_metadata"]
     nb_metadata = resources["pj_metadata"]["output"]["general"]
 
     is_enabled = nb_metadata["input"]
     if is_jinja_cell(cell.source):
         is_enabled = nb_metadata["input_jinja"]
@@ -254,8 +276,8 @@
     cell_metadata = cell.metadata["pj_metadata"]
     nb_metadata = resources["pj_metadata"]["output"]["html"]
 
     code_folding = nb_metadata["code_folding"]
     if "input_fold" in cell_metadata:
         code_folding = cell_metadata["input_fold"]
     value = f"fold-{code_folding}"
-    return value
+    return value
```

### Comparing `pretty-jupyter-2.0.4/src/pretty_jupyter/preprocessors/_token_preprocessor.py` & `pretty-jupyter-2.0.5/src/pretty_jupyter/preprocessors/_token_preprocessor.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,17 @@
 The main purpose of this package is to provide templates that make the output HTML export from
 ipynb look more pretty.
 
 """
 
 
 import re
+
 from nbconvert.preprocessors import Preprocessor
+
 from pretty_jupyter.constants import HTML_TOKEN_REGEX, TOKEN_SEP
 from pretty_jupyter.tokens import convert_markdown_tokens_to_html
 
 
 class TokenPreprocessor(Preprocessor):
     """
     A preprocessor which tokens from MD comments and transforms them
@@ -29,14 +31,15 @@
 
     Generated HTML:
     ```html
     <h2>Chapter</h2>
     <span class='pj-token token1 token2' style='display: none;'></span>
     ```
     """
+
     def preprocess(self, nb, resources):
         resources["token_sep"] = TOKEN_SEP
 
         return super().preprocess(nb, resources)
 
     def preprocess_cell(self, cell, resources, index):
         if cell.cell_type == "markdown":
@@ -46,14 +49,15 @@
 
 class TokenCleaningPreprocessor(Preprocessor):
     """
     Deletes tokens from cell outputs.
     """
 
     formats = ["text/markdown", "text/html"]
+
     def preprocess_cell(self, cell, resources, index):
         if cell.cell_type == "code":
             for i, output in enumerate(cell.outputs):
                 if not "data" in output:
                     continue
 
                 output_data = output["data"]
```

### Comparing `pretty-jupyter-2.0.4/src/pretty_jupyter/quickstart/empty.ipynb` & `pretty-jupyter-2.0.5/src/pretty_jupyter/quickstart/empty.ipynb`

 * *Files identical despite different names*

### Comparing `pretty-jupyter-2.0.4/src/pretty_jupyter/templates/pj/base.html.j2` & `pretty-jupyter-2.0.5/src/pretty_jupyter/templates/pj/base.html.j2`

 * *Files identical despite different names*

### Comparing `pretty-jupyter-2.0.4/src/pretty_jupyter/templates/pj/index.html.j2` & `pretty-jupyter-2.0.5/src/pretty_jupyter/templates/pj/index.html.j2`

 * *Files 2% similar despite different names*

```diff
@@ -181,15 +181,16 @@
         {% endif %}
 
         {% if html_metadata.toc %}
         // TOC
         let tocDepth = {{ html_metadata["toc_depth"] | tojson }};
         let tocCollapsed = {{ html_metadata['toc_collapsed'] | tojson }};
         let tocSmoothScroll = {{ html_metadata['toc_smooth_scroll'] | tojson }};
-        window.initializeTOC(tocDepth=tocDepth, tocCollapsed=tocCollapsed, tocSmoothScroll=tocSmoothScroll);
+        let tocExtendPage = {{ html_metadata['toc_extend_page'] | tojson }};
+        window.initializeTOC(tocDepth=tocDepth, tocCollapsed=tocCollapsed, tocSmoothScroll=tocSmoothScroll, tocExtendPage=tocExtendPage);
         {% endif %}
 
         {% if html_metadata["code_folding"] in ["show", "hide"] and resources.global_content_filter.include_input %}
         // code folding
         window.initializeCodeFolding({{ html_metadata['code_folding'] | tojson }} === "show");
         {% endif %}
```

### Comparing `pretty-jupyter-2.0.4/src/pretty_jupyter/templates/pj/static/libs/bootstrap.min.js` & `pretty-jupyter-2.0.5/src/pretty_jupyter/templates/pj/static/libs/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `pretty-jupyter-2.0.4/src/pretty_jupyter/templates/pj/static/libs/jquery-ui.min.js` & `pretty-jupyter-2.0.5/src/pretty_jupyter/templates/pj/static/libs/jquery-ui.min.js`

 * *Files identical despite different names*

### Comparing `pretty-jupyter-2.0.4/src/pretty_jupyter/templates/pj/static/libs/jquery.min.js` & `pretty-jupyter-2.0.5/src/pretty_jupyter/templates/pj/static/libs/jquery.min.js`

 * *Files identical despite different names*

### Comparing `pretty-jupyter-2.0.4/src/pretty_jupyter/templates/pj/static/libs/jquery.stickytabs.js` & `pretty-jupyter-2.0.5/src/pretty_jupyter/templates/pj/static/libs/jquery.stickytabs.js`

 * *Files identical despite different names*

### Comparing `pretty-jupyter-2.0.4/src/pretty_jupyter/templates/pj/static/libs/jquery.tocify.css` & `pretty-jupyter-2.0.5/src/pretty_jupyter/templates/pj/static/libs/jquery.tocify.css`

 * *Files identical despite different names*

### Comparing `pretty-jupyter-2.0.4/src/pretty_jupyter/templates/pj/static/libs/jquery.tocify.js` & `pretty-jupyter-2.0.5/src/pretty_jupyter/templates/pj/static/libs/jquery.tocify.js`

 * *Files identical despite different names*

### Comparing `pretty-jupyter-2.0.4/src/pretty_jupyter/templates/pj/static/libs/plotly.min.js` & `pretty-jupyter-2.0.5/src/pretty_jupyter/templates/pj/static/libs/plotly.min.js`

 * *Files identical despite different names*

### Comparing `pretty-jupyter-2.0.4/src/pretty_jupyter/templates/pj/static/libs/require.min.js` & `pretty-jupyter-2.0.5/src/pretty_jupyter/templates/pj/static/libs/require.min.js`

 * *Files identical despite different names*

### Comparing `pretty-jupyter-2.0.4/src/pretty_jupyter/templates/pj/static/pj-tabset.css` & `pretty-jupyter-2.0.5/src/pretty_jupyter/templates/pj/static/pj-tabset.css`

 * *Files identical despite different names*

### Comparing `pretty-jupyter-2.0.4/src/pretty_jupyter/templates/pj/static/pj-toc.css` & `pretty-jupyter-2.0.5/src/pretty_jupyter/templates/pj/static/pj-toc.css`

 * *Files identical despite different names*

### Comparing `pretty-jupyter-2.0.4/src/pretty_jupyter/templates/pj/static/pj.css` & `pretty-jupyter-2.0.5/src/pretty_jupyter/templates/pj/static/pj.css`

 * *Files identical despite different names*

### Comparing `pretty-jupyter-2.0.4/src/pretty_jupyter/templates/pj/static/pj.js` & `pretty-jupyter-2.0.5/src/pretty_jupyter/templates/pj/static/pj.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -231,15 +231,15 @@
         }
 
         numberedText = levels.join(".") + ". " + $(this).text();
         $(this).text(numberedText);
     })
 }
 
-window.initializeTOC = function(tocDepth, tocCollapsed, tocSmoothScroll) {
+window.initializeTOC = function(tocDepth, tocCollapsed, tocSmoothScroll, tocExtendPage) {
     // consistency with pandoc
     $('.unlisted.unnumbered').addClass('toc-ignore')
 
     // get allowed headers str
     let headers = []
     for (let i = 1; i <= MAX_HEADERS; i++) {
         headers.push(`h${i}`)
@@ -262,15 +262,16 @@
         selectors: selectors,
         theme: "bootstrap3",
         context: '.toc-content',
         hashGenerator: function(text) {
             return text.replace(/[.\\/?&!#<>"']/g, '').replace(/\s/g, '_');
         },
         ignoreSelector: ".toc-ignore",
-        scrollTo: 0
+        scrollTo: 0,
+        extendPage: tocExtendPage
     };
 
     options.smoothScroll = tocSmoothScroll;
 
     // tocify
     var toc = $("#TOC").tocify(options).data("toc-tocify");
```

### Comparing `pretty-jupyter-2.0.4/src/pretty_jupyter/templates/pj/static/themes/bootstrap.css` & `pretty-jupyter-2.0.5/src/pretty_jupyter/templates/pj/static/themes/bootstrap.css`

 * *Files identical despite different names*

### Comparing `pretty-jupyter-2.0.4/src/pretty_jupyter/templates/pj/static/themes/cerulean.css` & `pretty-jupyter-2.0.5/src/pretty_jupyter/templates/pj/static/themes/cerulean.css`

 * *Files identical despite different names*

### Comparing `pretty-jupyter-2.0.4/src/pretty_jupyter/templates/pj/static/themes/cosmo.css` & `pretty-jupyter-2.0.5/src/pretty_jupyter/templates/pj/static/themes/cosmo.css`

 * *Files identical despite different names*

### Comparing `pretty-jupyter-2.0.4/src/pretty_jupyter/templates/pj/static/themes/cyborg.css` & `pretty-jupyter-2.0.5/src/pretty_jupyter/templates/pj/static/themes/cyborg.css`

 * *Files identical despite different names*

### Comparing `pretty-jupyter-2.0.4/src/pretty_jupyter/templates/pj/static/themes/darkly.css` & `pretty-jupyter-2.0.5/src/pretty_jupyter/templates/pj/static/themes/darkly.css`

 * *Files identical despite different names*

### Comparing `pretty-jupyter-2.0.4/src/pretty_jupyter/templates/pj/static/themes/flatly.css` & `pretty-jupyter-2.0.5/src/pretty_jupyter/templates/pj/static/themes/flatly.css`

 * *Files identical despite different names*

### Comparing `pretty-jupyter-2.0.4/src/pretty_jupyter/templates/pj/static/themes/journal.css` & `pretty-jupyter-2.0.5/src/pretty_jupyter/templates/pj/static/themes/journal.css`

 * *Files identical despite different names*

### Comparing `pretty-jupyter-2.0.4/src/pretty_jupyter/templates/pj/static/themes/lumen.css` & `pretty-jupyter-2.0.5/src/pretty_jupyter/templates/pj/static/themes/lumen.css`

 * *Files identical despite different names*

### Comparing `pretty-jupyter-2.0.4/src/pretty_jupyter/templates/pj/static/themes/paper.css` & `pretty-jupyter-2.0.5/src/pretty_jupyter/templates/pj/static/themes/paper.css`

 * *Files identical despite different names*

### Comparing `pretty-jupyter-2.0.4/src/pretty_jupyter/templates/pj/static/themes/readable.css` & `pretty-jupyter-2.0.5/src/pretty_jupyter/templates/pj/static/themes/readable.css`

 * *Files identical despite different names*

### Comparing `pretty-jupyter-2.0.4/src/pretty_jupyter/templates/pj/static/themes/sandstone.css` & `pretty-jupyter-2.0.5/src/pretty_jupyter/templates/pj/static/themes/sandstone.css`

 * *Files identical despite different names*

### Comparing `pretty-jupyter-2.0.4/src/pretty_jupyter/templates/pj/static/themes/simplex.css` & `pretty-jupyter-2.0.5/src/pretty_jupyter/templates/pj/static/themes/simplex.css`

 * *Files identical despite different names*

### Comparing `pretty-jupyter-2.0.4/src/pretty_jupyter/templates/pj/static/themes/slate.css` & `pretty-jupyter-2.0.5/src/pretty_jupyter/templates/pj/static/themes/slate.css`

 * *Files identical despite different names*

### Comparing `pretty-jupyter-2.0.4/src/pretty_jupyter/templates/pj/static/themes/spacelab.css` & `pretty-jupyter-2.0.5/src/pretty_jupyter/templates/pj/static/themes/spacelab.css`

 * *Files identical despite different names*

### Comparing `pretty-jupyter-2.0.4/src/pretty_jupyter/templates/pj/static/themes/superhero.css` & `pretty-jupyter-2.0.5/src/pretty_jupyter/templates/pj/static/themes/superhero.css`

 * *Files identical despite different names*

### Comparing `pretty-jupyter-2.0.4/src/pretty_jupyter/templates/pj/static/themes/united.css` & `pretty-jupyter-2.0.5/src/pretty_jupyter/templates/pj/static/themes/united.css`

 * *Files identical despite different names*

### Comparing `pretty-jupyter-2.0.4/src/pretty_jupyter/templates/pj/static/themes/yeti.css` & `pretty-jupyter-2.0.5/src/pretty_jupyter/templates/pj/static/themes/yeti.css`

 * *Files identical despite different names*

### Comparing `pretty-jupyter-2.0.4/src/pretty_jupyter/templates/pj-legacy/index.html.j2` & `pretty-jupyter-2.0.5/src/pretty_jupyter/templates/pj-legacy/index.html.j2`

 * *Files identical despite different names*

### Comparing `pretty-jupyter-2.0.4/src/pretty_jupyter/templates/pj-pdf/index.tex.j2` & `pretty-jupyter-2.0.5/src/pretty_jupyter/templates/pj-pdf/index.tex.j2`

 * *Files identical despite different names*

### Comparing `pretty-jupyter-2.0.4/src/pretty_jupyter/tokens.py` & `pretty-jupyter-2.0.5/src/pretty_jupyter/tokens.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,18 @@
-import yaml
 import re
-from pretty_jupyter.constants import CODE_METADATA_TOKEN_REGEX, MARKDOWN_METADATA_TOKEN_REGEX, MARKDOWN_TOKEN_REGEX, HTML_TOKEN_FORMAT, TOKEN_SEP
+
+import yaml
+
+from pretty_jupyter.constants import (
+    CODE_METADATA_TOKEN_REGEX,
+    HTML_TOKEN_FORMAT,
+    MARKDOWN_METADATA_TOKEN_REGEX,
+    MARKDOWN_TOKEN_REGEX,
+    TOKEN_SEP,
+)
 
 
 def convert_markdown_tokens_to_html(input_str: str) -> str:
     """
     Processes input markdown string, converting all tokens from markdown token format
     to HTML token format.
 
@@ -26,37 +34,39 @@
             tokens = filter(lambda x: len(x) > 0, (m.strip() for m in gr.split()))
 
             # join them together and create html token out of them
             token_str = TOKEN_SEP.join(tokens)
             html = HTML_TOKEN_FORMAT.format(tokens=token_str)
 
             # replace the md tokens by html tokens
-            markdown = line[result.span()[0]:result.span()[1]]
+            markdown = line[result.span()[0] : result.span()[1]]
             line = line.replace(markdown, html)
         all_lines.append(line)
 
     # output is still in md, but token
     output = "\n".join(all_lines)
     return output
 
+
 def read_code_metadata_token(input_line: str) -> dict:
     # parse token
     result = re.search(CODE_METADATA_TOKEN_REGEX, input_line)
 
     if not result:
         return None
 
     if len(result.groups()) == 0:
         return None
 
     return yaml.safe_load(result.groups()[0])
 
+
 def read_markdown_metadata_token(input_line: str):
     result = re.search(MARKDOWN_METADATA_TOKEN_REGEX, input_line)
 
     if not result:
         return None
 
     if len(result.groups()) == 0:
         return None
 
-    return yaml.safe_load(result.groups()[0])
+    return yaml.safe_load(result.groups()[0])
```

### Comparing `pretty-jupyter-2.0.4/src/pretty_jupyter/utils.py` & `pretty-jupyter-2.0.5/src/pretty_jupyter/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,14 +12,15 @@
     main_dict = copy.deepcopy(main_dict)
     other_dict = copy.deepcopy(other_dict)
 
     other_dict = _update_dict(other_dict, main_dict)
 
     return other_dict
 
+
 def _update_dict(dict_, override_dict):
     for key, val in override_dict.items():
         if isinstance(val, dict):
             dict_[key] = _update_dict(dict_.get(key, {}), val)
         else:
             dict_[key] = val
     return dict_
```

### Comparing `pretty-jupyter-2.0.4/src/pretty_jupyter.egg-info/SOURCES.txt` & `pretty-jupyter-2.0.5/src/pretty_jupyter.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 LICENSE.md
 MANIFEST.in
 README.md
 pyproject.toml
 setup.cfg
-setup.py
 src/pretty_jupyter/__init__.py
 src/pretty_jupyter/__main__.py
 src/pretty_jupyter/console.py
 src/pretty_jupyter/constants.py
 src/pretty_jupyter/magics.py
 src/pretty_jupyter/testing.py
 src/pretty_jupyter/tokens.py
```

