# Comparing `tmp/ezhc-0.7.8.tar.gz` & `tmp/ezhc-0.7.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ezhc-0.7.8.tar", last modified: Fri Sep 17 11:18:55 2021, max compression
+gzip compressed data, was "dist/ezhc-0.7.9.tar", last modified: Sun Dec 12 16:05:48 2021, max compression
```

## Comparing `ezhc-0.7.8.tar` & `ezhc-0.7.9.tar`

### file list

```diff
@@ -1,90 +1,96 @@
-drwxrwxr-x   0 olivier   (1000) olivier   (1000)        0 2021-09-17 11:18:55.146475 ezhc-0.7.8/
--rw-rw-r--   0 olivier   (1000) olivier   (1000)     1083 2021-09-17 11:15:08.000000 ezhc-0.7.8/LICENSE
--rw-rw-r--   0 olivier   (1000) olivier   (1000)      332 2021-09-17 11:15:08.000000 ezhc-0.7.8/MANIFEST.in
--rw-rw-r--   0 olivier   (1000) olivier   (1000)      771 2021-09-17 11:18:55.146475 ezhc-0.7.8/PKG-INFO
--rw-rw-r--   0 olivier   (1000) olivier   (1000)     1813 2021-09-17 11:15:08.000000 ezhc-0.7.8/README.md
-drwxrwxr-x   0 olivier   (1000) olivier   (1000)        0 2021-09-17 11:18:55.134475 ezhc-0.7.8/ezhc/
--rw-rw-r--   0 olivier   (1000) olivier   (1000)      463 2021-09-17 11:15:08.000000 ezhc-0.7.8/ezhc/__init__.py
--rw-rw-r--   0 olivier   (1000) olivier   (1000)     1260 2021-09-17 11:17:24.000000 ezhc-0.7.8/ezhc/__meta__.py
--rw-rw-r--   0 olivier   (1000) olivier   (1000)     5074 2021-09-17 11:15:08.000000 ezhc-0.7.8/ezhc/_clock.py
--rw-rw-r--   0 olivier   (1000) olivier   (1000)     2398 2021-09-17 11:15:08.000000 ezhc-0.7.8/ezhc/_config.py
--rw-rw-r--   0 olivier   (1000) olivier   (1000)     3188 2021-09-17 11:15:08.000000 ezhc-0.7.8/ezhc/_global_options.py
--rw-rw-r--   0 olivier   (1000) olivier   (1000)     1107 2021-09-17 11:15:08.000000 ezhc-0.7.8/ezhc/_hc_versions.py
--rw-rw-r--   0 olivier   (1000) olivier   (1000)     2538 2021-09-17 11:15:08.000000 ezhc-0.7.8/ezhc/_highcharts.py
--rw-rw-r--   0 olivier   (1000) olivier   (1000)     4732 2021-09-17 11:15:08.000000 ezhc-0.7.8/ezhc/_highstock.py
--rw-rw-r--   0 olivier   (1000) olivier   (1000)     1111 2021-09-17 11:15:08.000000 ezhc-0.7.8/ezhc/_img.py
--rw-rw-r--   0 olivier   (1000) olivier   (1000)     6555 2021-09-17 11:15:08.000000 ezhc-0.7.8/ezhc/_plot.py
--rw-rw-r--   0 olivier   (1000) olivier   (1000)     1031 2021-09-17 11:15:08.000000 ezhc-0.7.8/ezhc/_proxy.py
--rw-rw-r--   0 olivier   (1000) olivier   (1000)     1178 2021-09-17 11:15:08.000000 ezhc-0.7.8/ezhc/_state.py
--rw-rw-r--   0 olivier   (1000) olivier   (1000)      942 2021-09-17 11:15:08.000000 ezhc-0.7.8/ezhc/_theme.py
--rw-rw-r--   0 olivier   (1000) olivier   (1000)     3903 2021-09-17 11:15:08.000000 ezhc-0.7.8/ezhc/_wrapper.py
-drwxrwxr-x   0 olivier   (1000) olivier   (1000)        0 2021-09-17 11:18:55.138475 ezhc-0.7.8/ezhc/api/
--rw-rw-r--   0 olivier   (1000) olivier   (1000)    69348 2021-09-17 11:15:08.000000 ezhc-0.7.8/ezhc/api/hc_object.json
--rw-rw-r--   0 olivier   (1000) olivier   (1000)  4104951 2021-09-17 11:15:08.000000 ezhc-0.7.8/ezhc/api/hc_option.json
--rw-rw-r--   0 olivier   (1000) olivier   (1000)    58237 2021-09-17 11:15:08.000000 ezhc-0.7.8/ezhc/api/hs_object.json
--rw-rw-r--   0 olivier   (1000) olivier   (1000)  2414273 2021-09-17 11:15:08.000000 ezhc-0.7.8/ezhc/api/hs_option.json
--rw-rw-r--   0 olivier   (1000) olivier   (1000)    14543 2021-09-17 11:15:08.000000 ezhc-0.7.8/ezhc/build.py
--rw-rw-r--   0 olivier   (1000) olivier   (1000)     2469 2021-09-17 11:15:08.000000 ezhc-0.7.8/ezhc/sample.py
-drwxrwxr-x   0 olivier   (1000) olivier   (1000)        0 2021-09-17 11:18:55.142475 ezhc-0.7.8/ezhc/samples/
--rw-rw-r--   0 olivier   (1000) olivier   (1000)      425 2021-09-17 11:15:08.000000 ezhc-0.7.8/ezhc/samples/df_bubble.csv
--rw-rw-r--   0 olivier   (1000) olivier   (1000)      909 2021-09-17 11:15:08.000000 ezhc-0.7.8/ezhc/samples/df_heatmap.csv
--rw-rw-r--   0 olivier   (1000) olivier   (1000)       80 2021-09-17 11:15:08.000000 ezhc-0.7.8/ezhc/samples/df_one_idx_one_col.csv
--rw-rw-r--   0 olivier   (1000) olivier   (1000)       86 2021-09-17 11:15:08.000000 ezhc-0.7.8/ezhc/samples/df_one_idx_several_col.csv
--rw-rw-r--   0 olivier   (1000) olivier   (1000)      275 2021-09-17 11:15:08.000000 ezhc-0.7.8/ezhc/samples/df_one_idx_several_col_2.csv
--rw-rw-r--   0 olivier   (1000) olivier   (1000)      174 2021-09-17 11:15:08.000000 ezhc-0.7.8/ezhc/samples/df_one_idx_two_col.csv
--rw-rw-r--   0 olivier   (1000) olivier   (1000)     8659 2021-09-17 11:15:08.000000 ezhc-0.7.8/ezhc/samples/df_scatter.csv
--rw-rw-r--   0 olivier   (1000) olivier   (1000)    24151 2021-09-17 11:15:08.000000 ezhc-0.7.8/ezhc/samples/df_several_idx_one_col.csv
--rw-rw-r--   0 olivier   (1000) olivier   (1000)    10021 2021-09-17 11:15:08.000000 ezhc-0.7.8/ezhc/samples/df_several_idx_one_col_2.csv
--rw-rw-r--   0 olivier   (1000) olivier   (1000)      694 2021-09-17 11:15:08.000000 ezhc-0.7.8/ezhc/samples/df_two_idx_one_col.csv
--rw-rw-r--   0 olivier   (1000) olivier   (1000)     2634 2021-09-17 11:15:08.000000 ezhc-0.7.8/ezhc/samples/df_two_idx_several_col.csv
-drwxrwxr-x   0 olivier   (1000) olivier   (1000)        0 2021-09-17 11:18:55.142475 ezhc-0.7.8/ezhc/script/
--rw-rw-r--   0 olivier   (1000) olivier   (1000)    24631 2021-09-17 11:15:08.000000 ezhc-0.7.8/ezhc/script/Jupyter_logo.png
--rw-rw-r--   0 olivier   (1000) olivier   (1000)      951 2021-09-17 11:15:08.000000 ezhc-0.7.8/ezhc/script/SG_logo.png
--rw-rw-r--   0 olivier   (1000) olivier   (1000)      197 2021-09-17 11:15:08.000000 ezhc-0.7.8/ezhc/script/financial_time_series_0.js
--rw-rw-r--   0 olivier   (1000) olivier   (1000)     1112 2021-09-17 11:15:08.000000 ezhc-0.7.8/ezhc/script/financial_time_series_table.html
--rw-rw-r--   0 olivier   (1000) olivier   (1000)     6641 2021-09-17 11:15:08.000000 ezhc-0.7.8/ezhc/script/financial_time_series_table_1.js
--rw-rw-r--   0 olivier   (1000) olivier   (1000)     5302 2021-09-17 11:15:08.000000 ezhc-0.7.8/ezhc/script/financial_time_series_table_2.js
--rw-rw-r--   0 olivier   (1000) olivier   (1000)      434 2021-09-17 11:15:08.000000 ezhc-0.7.8/ezhc/script/financial_time_series_table_options_1.js
--rw-rw-r--   0 olivier   (1000) olivier   (1000)      438 2021-09-17 11:15:08.000000 ezhc-0.7.8/ezhc/script/financial_time_series_table_options_2.js
--rw-rw-r--   0 olivier   (1000) olivier   (1000)       66 2021-09-17 11:15:08.000000 ezhc-0.7.8/ezhc/script/formatter_basic.js
--rw-rw-r--   0 olivier   (1000) olivier   (1000)       72 2021-09-17 11:15:08.000000 ezhc-0.7.8/ezhc/script/formatter_percent.js
--rw-rw-r--   0 olivier   (1000) olivier   (1000)      794 2021-09-17 11:15:08.000000 ezhc-0.7.8/ezhc/script/formatter_quantile.js
--rw-rw-r--   0 olivier   (1000) olivier   (1000)      728 2021-09-17 11:15:08.000000 ezhc-0.7.8/ezhc/script/json_parse.js
--rw-rw-r--   0 olivier   (1000) olivier   (1000)      616 2021-09-17 11:15:08.000000 ezhc-0.7.8/ezhc/script/template_disclaimer.html
-drwxrwxr-x   0 olivier   (1000) olivier   (1000)        0 2021-09-17 11:18:55.146475 ezhc-0.7.8/ezhc/script/themes/
--rw-rw-r--   0 olivier   (1000) olivier   (1000)      312 2021-09-17 11:15:08.000000 ezhc-0.7.8/ezhc/script/themes/avocado.js
--rw-rw-r--   0 olivier   (1000) olivier   (1000)      448 2021-09-17 11:15:08.000000 ezhc-0.7.8/ezhc/script/themes/avocado.json
--rw-rw-r--   0 olivier   (1000) olivier   (1000)     2634 2021-09-17 11:15:08.000000 ezhc-0.7.8/ezhc/script/themes/build_theme_json.ipynb
--rw-rw-r--   0 olivier   (1000) olivier   (1000)     4159 2021-09-17 11:15:08.000000 ezhc-0.7.8/ezhc/script/themes/dark-blue.js
--rw-rw-r--   0 olivier   (1000) olivier   (1000)     8477 2021-09-17 11:15:08.000000 ezhc-0.7.8/ezhc/script/themes/dark-blue.json
--rw-rw-r--   0 olivier   (1000) olivier   (1000)     4146 2021-09-17 11:15:08.000000 ezhc-0.7.8/ezhc/script/themes/dark-green.js
--rw-rw-r--   0 olivier   (1000) olivier   (1000)     8457 2021-09-17 11:15:08.000000 ezhc-0.7.8/ezhc/script/themes/dark-green.json
--rw-rw-r--   0 olivier   (1000) olivier   (1000)     3112 2021-09-17 11:15:08.000000 ezhc-0.7.8/ezhc/script/themes/dark-unica.js
--rw-rw-r--   0 olivier   (1000) olivier   (1000)     4917 2021-09-17 11:15:08.000000 ezhc-0.7.8/ezhc/script/themes/dark-unica.json
--rw-rw-r--   0 olivier   (1000) olivier   (1000)     4345 2021-09-17 11:15:08.000000 ezhc-0.7.8/ezhc/script/themes/gray.js
--rw-rw-r--   0 olivier   (1000) olivier   (1000)     8819 2021-09-17 11:15:08.000000 ezhc-0.7.8/ezhc/script/themes/gray.json
--rw-rw-r--   0 olivier   (1000) olivier   (1000)      866 2021-09-17 11:15:08.000000 ezhc-0.7.8/ezhc/script/themes/grid-light.js
--rw-rw-r--   0 olivier   (1000) olivier   (1000)     1321 2021-09-17 11:15:08.000000 ezhc-0.7.8/ezhc/script/themes/grid-light.json
--rw-rw-r--   0 olivier   (1000) olivier   (1000)     1636 2021-09-17 11:15:08.000000 ezhc-0.7.8/ezhc/script/themes/grid.js
--rw-rw-r--   0 olivier   (1000) olivier   (1000)     2669 2021-09-17 11:15:08.000000 ezhc-0.7.8/ezhc/script/themes/grid.json
--rw-rw-r--   0 olivier   (1000) olivier   (1000)     1087 2021-09-17 11:15:08.000000 ezhc-0.7.8/ezhc/script/themes/sand-signika.js
--rw-rw-r--   0 olivier   (1000) olivier   (1000)     1687 2021-09-17 11:15:08.000000 ezhc-0.7.8/ezhc/script/themes/sand-signika.json
--rw-rw-r--   0 olivier   (1000) olivier   (1000)     1643 2021-09-17 11:15:08.000000 ezhc-0.7.8/ezhc/script/themes/skies.js
--rw-rw-r--   0 olivier   (1000) olivier   (1000)     2511 2021-09-17 11:15:08.000000 ezhc-0.7.8/ezhc/script/themes/skies.json
--rw-rw-r--   0 olivier   (1000) olivier   (1000)      272 2021-09-17 11:15:08.000000 ezhc-0.7.8/ezhc/script/themes/sunset.js
--rw-rw-r--   0 olivier   (1000) olivier   (1000)      400 2021-09-17 11:15:08.000000 ezhc-0.7.8/ezhc/script/themes/sunset.json
--rw-rw-r--   0 olivier   (1000) olivier   (1000)      912 2021-09-17 11:15:08.000000 ezhc-0.7.8/ezhc/script/tooltip_positioner_center_top.js
--rw-rw-r--   0 olivier   (1000) olivier   (1000)      792 2021-09-17 11:15:08.000000 ezhc-0.7.8/ezhc/script/tooltip_positioner_left_top.js
--rw-rw-r--   0 olivier   (1000) olivier   (1000)      875 2021-09-17 11:15:08.000000 ezhc-0.7.8/ezhc/script/tooltip_positioner_right_top.js
--rw-rw-r--   0 olivier   (1000) olivier   (1000)     2717 2021-09-17 11:15:08.000000 ezhc-0.7.8/ezhc/scripts.py
--rw-rw-r--   0 olivier   (1000) olivier   (1000)     3823 2021-09-17 11:15:08.000000 ezhc-0.7.8/ezhc/series.py
-drwxrwxr-x   0 olivier   (1000) olivier   (1000)        0 2021-09-17 11:18:55.134475 ezhc-0.7.8/ezhc.egg-info/
--rw-rw-r--   0 olivier   (1000) olivier   (1000)      771 2021-09-17 11:18:55.000000 ezhc-0.7.8/ezhc.egg-info/PKG-INFO
--rw-rw-r--   0 olivier   (1000) olivier   (1000)     2322 2021-09-17 11:18:55.000000 ezhc-0.7.8/ezhc.egg-info/SOURCES.txt
--rw-rw-r--   0 olivier   (1000) olivier   (1000)        1 2021-09-17 11:18:55.000000 ezhc-0.7.8/ezhc.egg-info/dependency_links.txt
--rw-rw-r--   0 olivier   (1000) olivier   (1000)        1 2021-09-17 11:18:01.000000 ezhc-0.7.8/ezhc.egg-info/not-zip-safe
--rw-rw-r--   0 olivier   (1000) olivier   (1000)       52 2021-09-17 11:18:55.000000 ezhc-0.7.8/ezhc.egg-info/requires.txt
--rw-rw-r--   0 olivier   (1000) olivier   (1000)        5 2021-09-17 11:18:55.000000 ezhc-0.7.8/ezhc.egg-info/top_level.txt
--rw-rw-r--   0 olivier   (1000) olivier   (1000)       52 2021-09-17 11:15:08.000000 ezhc-0.7.8/requirements.txt
--rw-rw-r--   0 olivier   (1000) olivier   (1000)       80 2021-09-17 11:18:55.146475 ezhc-0.7.8/setup.cfg
--rw-rw-r--   0 olivier   (1000) olivier   (1000)     1856 2021-09-17 11:15:08.000000 ezhc-0.7.8/setup.py
+drwxrwxr-x   0 olivier   (1000) olivier   (1000)        0 2021-12-12 16:05:48.282328 ezhc-0.7.9/
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)       65 2021-09-17 11:18:29.000000 ezhc-0.7.9/.gitignore
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)     1083 2021-09-17 11:15:08.000000 ezhc-0.7.9/LICENSE
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)      332 2021-09-17 11:15:08.000000 ezhc-0.7.9/MANIFEST.in
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)      771 2021-12-12 16:05:48.282328 ezhc-0.7.9/PKG-INFO
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)     1813 2021-09-17 11:15:08.000000 ezhc-0.7.9/README.md
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)   898249 2021-09-17 11:15:08.000000 ezhc-0.7.9/demo_ezhc.ipynb
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)    27187 2021-09-17 11:15:08.000000 ezhc-0.7.9/demo_ezhc_themes_and_global_options.ipynb
+drwxrwxr-x   0 olivier   (1000) olivier   (1000)        0 2021-12-12 16:05:48.266328 ezhc-0.7.9/ezhc/
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)      463 2021-09-17 11:15:08.000000 ezhc-0.7.9/ezhc/__init__.py
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)     1260 2021-12-12 16:03:09.000000 ezhc-0.7.9/ezhc/__meta__.py
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)     5074 2021-09-17 11:15:08.000000 ezhc-0.7.9/ezhc/_clock.py
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)     2398 2021-09-17 11:15:08.000000 ezhc-0.7.9/ezhc/_config.py
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)     3188 2021-09-17 11:15:08.000000 ezhc-0.7.9/ezhc/_global_options.py
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)     1107 2021-09-17 11:15:08.000000 ezhc-0.7.9/ezhc/_hc_versions.py
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)     2538 2021-09-17 11:15:08.000000 ezhc-0.7.9/ezhc/_highcharts.py
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)     4732 2021-09-17 11:15:08.000000 ezhc-0.7.9/ezhc/_highstock.py
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)     1111 2021-09-17 11:15:08.000000 ezhc-0.7.9/ezhc/_img.py
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)     6555 2021-09-17 11:15:08.000000 ezhc-0.7.9/ezhc/_plot.py
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)     1031 2021-09-17 11:15:08.000000 ezhc-0.7.9/ezhc/_proxy.py
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)     1178 2021-09-17 11:15:08.000000 ezhc-0.7.9/ezhc/_state.py
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)      942 2021-09-17 11:15:08.000000 ezhc-0.7.9/ezhc/_theme.py
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)     3903 2021-09-17 11:15:08.000000 ezhc-0.7.9/ezhc/_wrapper.py
+drwxrwxr-x   0 olivier   (1000) olivier   (1000)        0 2021-12-12 16:05:48.270328 ezhc-0.7.9/ezhc/api/
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)    69348 2021-09-17 11:15:08.000000 ezhc-0.7.9/ezhc/api/hc_object.json
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)  4104951 2021-09-17 11:15:08.000000 ezhc-0.7.9/ezhc/api/hc_option.json
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)    58237 2021-09-17 11:15:08.000000 ezhc-0.7.9/ezhc/api/hs_object.json
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)  2414273 2021-09-17 11:15:08.000000 ezhc-0.7.9/ezhc/api/hs_option.json
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)    14164 2021-12-12 16:02:41.000000 ezhc-0.7.9/ezhc/build.py
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)     2469 2021-09-17 11:15:08.000000 ezhc-0.7.9/ezhc/sample.py
+drwxrwxr-x   0 olivier   (1000) olivier   (1000)        0 2021-12-12 16:05:48.278329 ezhc-0.7.9/ezhc/samples/
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)     1306 2021-09-17 11:15:08.000000 ezhc-0.7.9/ezhc/samples/build_data_world_population.py
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)    50033 2021-09-17 11:15:08.000000 ezhc-0.7.9/ezhc/samples/build_samples.py
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)    23270 2021-09-17 11:15:08.000000 ezhc-0.7.9/ezhc/samples/data_population.py
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)      425 2021-09-17 11:15:08.000000 ezhc-0.7.9/ezhc/samples/df_bubble.csv
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)      909 2021-09-17 11:15:08.000000 ezhc-0.7.9/ezhc/samples/df_heatmap.csv
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)       80 2021-09-17 11:15:08.000000 ezhc-0.7.9/ezhc/samples/df_one_idx_one_col.csv
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)       86 2021-09-17 11:15:08.000000 ezhc-0.7.9/ezhc/samples/df_one_idx_several_col.csv
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)      275 2021-09-17 11:15:08.000000 ezhc-0.7.9/ezhc/samples/df_one_idx_several_col_2.csv
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)      174 2021-09-17 11:15:08.000000 ezhc-0.7.9/ezhc/samples/df_one_idx_two_col.csv
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)     8659 2021-09-17 11:15:08.000000 ezhc-0.7.9/ezhc/samples/df_scatter.csv
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)    24151 2021-09-17 11:15:08.000000 ezhc-0.7.9/ezhc/samples/df_several_idx_one_col.csv
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)    10021 2021-09-17 11:15:08.000000 ezhc-0.7.9/ezhc/samples/df_several_idx_one_col_2.csv
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)      694 2021-09-17 11:15:08.000000 ezhc-0.7.9/ezhc/samples/df_two_idx_one_col.csv
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)     2634 2021-09-17 11:15:08.000000 ezhc-0.7.9/ezhc/samples/df_two_idx_several_col.csv
+drwxrwxr-x   0 olivier   (1000) olivier   (1000)        0 2021-12-12 16:05:48.278329 ezhc-0.7.9/ezhc/script/
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)    24631 2021-09-17 11:15:08.000000 ezhc-0.7.9/ezhc/script/Jupyter_logo.png
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)      951 2021-09-17 11:15:08.000000 ezhc-0.7.9/ezhc/script/SG_logo.png
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)      197 2021-09-17 11:15:08.000000 ezhc-0.7.9/ezhc/script/financial_time_series_0.js
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)     1112 2021-09-17 11:15:08.000000 ezhc-0.7.9/ezhc/script/financial_time_series_table.html
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)     6641 2021-09-17 11:15:08.000000 ezhc-0.7.9/ezhc/script/financial_time_series_table_1.js
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)     5302 2021-09-17 11:15:08.000000 ezhc-0.7.9/ezhc/script/financial_time_series_table_2.js
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)      434 2021-09-17 11:15:08.000000 ezhc-0.7.9/ezhc/script/financial_time_series_table_options_1.js
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)      438 2021-09-17 11:15:08.000000 ezhc-0.7.9/ezhc/script/financial_time_series_table_options_2.js
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)       66 2021-09-17 11:15:08.000000 ezhc-0.7.9/ezhc/script/formatter_basic.js
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)       72 2021-09-17 11:15:08.000000 ezhc-0.7.9/ezhc/script/formatter_percent.js
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)      794 2021-09-17 11:15:08.000000 ezhc-0.7.9/ezhc/script/formatter_quantile.js
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)      728 2021-09-17 11:15:08.000000 ezhc-0.7.9/ezhc/script/json_parse.js
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)      616 2021-09-17 11:15:08.000000 ezhc-0.7.9/ezhc/script/template_disclaimer.html
+drwxrwxr-x   0 olivier   (1000) olivier   (1000)        0 2021-12-12 16:05:48.282328 ezhc-0.7.9/ezhc/script/themes/
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)      312 2021-09-17 11:15:08.000000 ezhc-0.7.9/ezhc/script/themes/avocado.js
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)      448 2021-09-17 11:15:08.000000 ezhc-0.7.9/ezhc/script/themes/avocado.json
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)     2634 2021-09-17 11:15:08.000000 ezhc-0.7.9/ezhc/script/themes/build_theme_json.ipynb
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)     4159 2021-09-17 11:15:08.000000 ezhc-0.7.9/ezhc/script/themes/dark-blue.js
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)     8477 2021-09-17 11:15:08.000000 ezhc-0.7.9/ezhc/script/themes/dark-blue.json
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)     4146 2021-09-17 11:15:08.000000 ezhc-0.7.9/ezhc/script/themes/dark-green.js
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)     8457 2021-09-17 11:15:08.000000 ezhc-0.7.9/ezhc/script/themes/dark-green.json
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)     3112 2021-09-17 11:15:08.000000 ezhc-0.7.9/ezhc/script/themes/dark-unica.js
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)     4917 2021-09-17 11:15:08.000000 ezhc-0.7.9/ezhc/script/themes/dark-unica.json
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)     4345 2021-09-17 11:15:08.000000 ezhc-0.7.9/ezhc/script/themes/gray.js
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)     8819 2021-09-17 11:15:08.000000 ezhc-0.7.9/ezhc/script/themes/gray.json
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)      866 2021-09-17 11:15:08.000000 ezhc-0.7.9/ezhc/script/themes/grid-light.js
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)     1321 2021-09-17 11:15:08.000000 ezhc-0.7.9/ezhc/script/themes/grid-light.json
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)     1636 2021-09-17 11:15:08.000000 ezhc-0.7.9/ezhc/script/themes/grid.js
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)     2669 2021-09-17 11:15:08.000000 ezhc-0.7.9/ezhc/script/themes/grid.json
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)     1087 2021-09-17 11:15:08.000000 ezhc-0.7.9/ezhc/script/themes/sand-signika.js
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)     1687 2021-09-17 11:15:08.000000 ezhc-0.7.9/ezhc/script/themes/sand-signika.json
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)     1643 2021-09-17 11:15:08.000000 ezhc-0.7.9/ezhc/script/themes/skies.js
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)     2511 2021-09-17 11:15:08.000000 ezhc-0.7.9/ezhc/script/themes/skies.json
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)      272 2021-09-17 11:15:08.000000 ezhc-0.7.9/ezhc/script/themes/sunset.js
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)      400 2021-09-17 11:15:08.000000 ezhc-0.7.9/ezhc/script/themes/sunset.json
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)      912 2021-09-17 11:15:08.000000 ezhc-0.7.9/ezhc/script/tooltip_positioner_center_top.js
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)      792 2021-09-17 11:15:08.000000 ezhc-0.7.9/ezhc/script/tooltip_positioner_left_top.js
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)      875 2021-09-17 11:15:08.000000 ezhc-0.7.9/ezhc/script/tooltip_positioner_right_top.js
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)     2717 2021-09-17 11:15:08.000000 ezhc-0.7.9/ezhc/scripts.py
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)     3823 2021-09-17 11:15:08.000000 ezhc-0.7.9/ezhc/series.py
+drwxrwxr-x   0 olivier   (1000) olivier   (1000)        0 2021-12-12 16:05:48.266328 ezhc-0.7.9/ezhc.egg-info/
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)      771 2021-12-12 16:05:48.000000 ezhc-0.7.9/ezhc.egg-info/PKG-INFO
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)     2497 2021-12-12 16:05:48.000000 ezhc-0.7.9/ezhc.egg-info/SOURCES.txt
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)        1 2021-12-12 16:05:48.000000 ezhc-0.7.9/ezhc.egg-info/dependency_links.txt
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)        1 2021-09-17 11:18:01.000000 ezhc-0.7.9/ezhc.egg-info/not-zip-safe
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)       52 2021-12-12 16:05:48.000000 ezhc-0.7.9/ezhc.egg-info/requires.txt
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)        5 2021-12-12 16:05:48.000000 ezhc-0.7.9/ezhc.egg-info/top_level.txt
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)       52 2021-09-17 11:15:08.000000 ezhc-0.7.9/requirements.txt
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)       80 2021-12-12 16:05:48.286329 ezhc-0.7.9/setup.cfg
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)     1864 2021-09-17 11:34:13.000000 ezhc-0.7.9/setup.py
```

### Comparing `ezhc-0.7.8/LICENSE` & `ezhc-0.7.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ezhc-0.7.8/PKG-INFO` & `ezhc-0.7.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 1.1
 Name: ezhc
-Version: 0.7.8
+Version: 0.7.9
 Summary: easy Highcharts & Highstock, dynamic plots from pandas dataframes in the Jupyter notebook
 Home-page: https://github.com/oscar6echo/ezhc
 Author: oscar6echo
 Author-email: olivier.borderies@gmail.com
 License: MIT
-Download-URL: https://github.com/oscar6echo/ezhc/tarball/0.7.8
+Download-URL: https://github.com/oscar6echo/ezhc/tarball/0.7.9
 Description: UNKNOWN
 Keywords: Highcharts,Highstock,pandas,notebook,javascript
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.5
```

### Comparing `ezhc-0.7.8/README.md` & `ezhc-0.7.9/README.md`

 * *Files identical despite different names*

### Comparing `ezhc-0.7.8/ezhc/__meta__.py` & `ezhc-0.7.9/ezhc/__meta__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 
 __name__ = 'ezhc'
 name_url = __name__.replace('_', '-')
 
 __packages__ = [__name__]
-__version__ = '0.7.8'
+__version__ = '0.7.9'
 __description__ = 'easy Highcharts & Highstock, dynamic plots from pandas dataframes in the Jupyter notebook'
 __author__ = 'oscar6echo'
 __author_email__ = 'olivier.borderies@gmail.com'
 __url__ = 'https://github.com/{}/{}'.format(__author__,
                                             name_url)
 __download_url__ = 'https://github.com/{}/{}/tarball/{}'.format(__author__,
                                                                 name_url,
```

### Comparing `ezhc-0.7.8/ezhc/_clock.py` & `ezhc-0.7.9/ezhc/_clock.py`

 * *Files identical despite different names*

### Comparing `ezhc-0.7.8/ezhc/_config.py` & `ezhc-0.7.9/ezhc/_config.py`

 * *Files identical despite different names*

### Comparing `ezhc-0.7.8/ezhc/_global_options.py` & `ezhc-0.7.9/ezhc/_global_options.py`

 * *Files identical despite different names*

### Comparing `ezhc-0.7.8/ezhc/_hc_versions.py` & `ezhc-0.7.9/ezhc/_hc_versions.py`

 * *Files identical despite different names*

### Comparing `ezhc-0.7.8/ezhc/_highcharts.py` & `ezhc-0.7.9/ezhc/_highcharts.py`

 * *Files identical despite different names*

### Comparing `ezhc-0.7.8/ezhc/_highstock.py` & `ezhc-0.7.9/ezhc/_highstock.py`

 * *Files identical despite different names*

### Comparing `ezhc-0.7.8/ezhc/_img.py` & `ezhc-0.7.9/ezhc/_img.py`

 * *Files identical despite different names*

### Comparing `ezhc-0.7.8/ezhc/_plot.py` & `ezhc-0.7.9/ezhc/_plot.py`

 * *Files identical despite different names*

### Comparing `ezhc-0.7.8/ezhc/_proxy.py` & `ezhc-0.7.9/ezhc/_proxy.py`

 * *Files identical despite different names*

### Comparing `ezhc-0.7.8/ezhc/_state.py` & `ezhc-0.7.9/ezhc/_state.py`

 * *Files identical despite different names*

### Comparing `ezhc-0.7.8/ezhc/_theme.py` & `ezhc-0.7.9/ezhc/_theme.py`

 * *Files identical despite different names*

### Comparing `ezhc-0.7.8/ezhc/_wrapper.py` & `ezhc-0.7.9/ezhc/_wrapper.py`

 * *Files identical despite different names*

### Comparing `ezhc-0.7.8/ezhc/api/hc_object.json` & `ezhc-0.7.9/ezhc/api/hc_object.json`

 * *Files identical despite different names*

### Comparing `ezhc-0.7.8/ezhc/api/hc_option.json` & `ezhc-0.7.9/ezhc/api/hc_option.json`

 * *Files identical despite different names*

### Comparing `ezhc-0.7.8/ezhc/api/hs_object.json` & `ezhc-0.7.9/ezhc/api/hs_object.json`

 * *Files identical despite different names*

### Comparing `ezhc-0.7.8/ezhc/api/hs_option.json` & `ezhc-0.7.9/ezhc/api/hs_option.json`

 * *Files identical despite different names*

### Comparing `ezhc-0.7.8/ezhc/build.py` & `ezhc-0.7.9/ezhc/build.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,46 +5,41 @@
                   "#f15c80", "#e4d354", "#2b908f", "#f45b5b", "#91e8e1"]
 
 
 def series(df, *args, **kwargs):
     idx = df.index
     col = df.columns
     data = df.values
-    assert(isinstance(idx, pd.core.index.Index))
+    assert(isinstance(idx, pd.Index))
 
     series = []
     for k, c in enumerate(col):
         if df[c].dtype.kind in 'fib':
             v = data[:, k]
             sec = c in kwargs.get('secondary_y', [])
             d = {
                 'name': c if not sec else c + ' (right)',
                 'yAxis': int(sec),
                 'data': [[idx[q], v[q]] for q in range(len(v))],
             }
-            if c in kwargs.get('color', []):
-                d['color'] = kwargs['color'].get(c)
-            if c in kwargs.get('visible', []):
-                d['visible'] = kwargs['visible'].get(c)
-            if c in kwargs.get('fillColor', []):
-                d['type'] = 'area'
-                d['fillColor'] = kwargs['fillColor'].get(c)
-            if c in kwargs.get('lineColor', []):
-                d['lineColor'] = kwargs['lineColor'].get(c)
-            if kwargs.get('dashStyle', []):
-                d['dashStyle'] = kwargs['dashStyle'].get(c, 'Solid')
+            for key in kwargs.keys():
+                if key == 'fillColor':
+                    d['type'] = 'area'
+                    d['fillColor'] = kwargs['fillColor'].get(c)
+                elif c in kwargs.get(key, []):
+                    d[key] = kwargs[key].get(c)
             series.append(d)
     return series
 
 
 def series_range(df, *args, **kwargs):
     idx = df.index
     col = df.columns
     data = df.values
-    assert(isinstance(idx, pd.core.index.Index))
+    assert(isinstance(idx, pd.Index))
     assert(len(col) == 2)
     assert(df[col[0]].dtype.kind in 'if')
     assert(df[col[1]].dtype.kind in 'if')
 
     series = [{
         'data': [[data[q, 0], data[q, 1]] for q in range(data.shape[0])],
     }]
@@ -54,15 +49,15 @@
 
     return axis_categories, series
 
 
 def series_drilldown_orig(df, colorByPoint=True, pointPlacement='on', *args, **kwargs):
     idx = df.index
     col = df.columns
-    assert(isinstance(idx, pd.core.index.MultiIndex))
+    assert(isinstance(idx, pd.MultiIndex))
     assert(len(idx.levshape) == 2)
     for c in col:
         assert df[c].dtype.kind in 'if'
 
     levone = list(idx.levels[0])
     data = []
     series = []
@@ -109,15 +104,15 @@
                      colors=None,
                      set_precision=False,
                      precision=None,
                      *args,
                      **kwargs):
     idx = df.index
     col = df.columns
-    assert(isinstance(idx, pd.core.index.MultiIndex))
+    assert(isinstance(idx, pd.MultiIndex))
     for c in col:
         assert df[c].dtype.kind in 'if'
 
     class DrillDownBuilder:
         """
         Recursive build of drilldown structure
         """
@@ -226,15 +221,15 @@
 
     return dd.series(), dd.drilldown_series()
 
 
 # def series_drilldown_orig(df, colorByPoint=True, pointPlacement='on', *args, **kwargs):
 #     idx = df.index
 #     col = df.columns
-#     assert(isinstance(idx, pd.core.index.MultiIndex))
+#     assert(isinstance(idx, pd.MultiIndex))
 #     assert(len(idx.levshape) == 2)
 #     for c in col:
 #         assert df[c].dtype.kind in 'if'
 
 #     levone = list(idx.levels[0])
 #     data = []
 #     series = []
@@ -272,15 +267,15 @@
 
 #     return series, drilldownSeries
 
 
 def series_scatter(df, color_column=None, title_column=None, *args, **kwargs):
     idx = df.index
     col = df.columns
-    assert(isinstance(idx, pd.core.index.MultiIndex))
+    assert(isinstance(idx, pd.MultiIndex))
     assert(len(idx.levshape) == 2)
     assert(len(col) <= 2)
     assert(df[color_column].dtype.kind in 'iO')
 
     if color_column == None:
         assert(len(col) == 1)
         color_column = col[0]
@@ -305,15 +300,15 @@
                        })
     return series
 
 
 def series_bubble(df, *args, **kwargs):
     idx = df.index
     col = df.columns
-    assert(isinstance(idx, pd.core.index.MultiIndex))
+    assert(isinstance(idx, pd.MultiIndex))
     assert(len(idx.levshape) == 3)
     assert(len(col) == 1)
     assert(df[col[0]].dtype.kind in 'fib')
 
     names = list(idx.levels[0])
     series = []
     for s in names:
@@ -331,15 +326,15 @@
 
     return series
 
 
 def series_heatmap(df, *args, **kwargs):
     idx = df.index
     col = df.columns
-    assert(isinstance(idx, pd.core.index.Index))
+    assert(isinstance(idx, pd.Index))
     for c in col:
         assert(df[c].dtype.kind in 'if')
 
     dft = df.copy()
     dft.index = range(len(df.index))
     dft.columns = range(len(df.columns))
     res_data = list(dft.stack().swaplevel(0, 1).reset_index().values)
```

### Comparing `ezhc-0.7.8/ezhc/sample.py` & `ezhc-0.7.9/ezhc/sample.py`

 * *Files identical despite different names*

### Comparing `ezhc-0.7.8/ezhc/samples/df_heatmap.csv` & `ezhc-0.7.9/ezhc/samples/df_heatmap.csv`

 * *Files identical despite different names*

### Comparing `ezhc-0.7.8/ezhc/samples/df_scatter.csv` & `ezhc-0.7.9/ezhc/samples/df_scatter.csv`

 * *Files identical despite different names*

### Comparing `ezhc-0.7.8/ezhc/samples/df_several_idx_one_col.csv` & `ezhc-0.7.9/ezhc/samples/df_several_idx_one_col.csv`

 * *Files identical despite different names*

### Comparing `ezhc-0.7.8/ezhc/samples/df_several_idx_one_col_2.csv` & `ezhc-0.7.9/ezhc/samples/df_several_idx_one_col_2.csv`

 * *Files identical despite different names*

### Comparing `ezhc-0.7.8/ezhc/samples/df_two_idx_one_col.csv` & `ezhc-0.7.9/ezhc/samples/df_two_idx_one_col.csv`

 * *Files identical despite different names*

### Comparing `ezhc-0.7.8/ezhc/samples/df_two_idx_several_col.csv` & `ezhc-0.7.9/ezhc/samples/df_two_idx_several_col.csv`

 * *Files identical despite different names*

### Comparing `ezhc-0.7.8/ezhc/script/Jupyter_logo.png` & `ezhc-0.7.9/ezhc/script/Jupyter_logo.png`

 * *Files identical despite different names*

### Comparing `ezhc-0.7.8/ezhc/script/SG_logo.png` & `ezhc-0.7.9/ezhc/script/SG_logo.png`

 * *Files identical despite different names*

### Comparing `ezhc-0.7.8/ezhc/script/financial_time_series_table.html` & `ezhc-0.7.9/ezhc/script/financial_time_series_table.html`

 * *Files identical despite different names*

### Comparing `ezhc-0.7.8/ezhc/script/financial_time_series_table_1.js` & `ezhc-0.7.9/ezhc/script/financial_time_series_table_1.js`

 * *Files identical despite different names*

### Comparing `ezhc-0.7.8/ezhc/script/financial_time_series_table_2.js` & `ezhc-0.7.9/ezhc/script/financial_time_series_table_2.js`

 * *Files identical despite different names*

### Comparing `ezhc-0.7.8/ezhc/script/formatter_quantile.js` & `ezhc-0.7.9/ezhc/script/formatter_quantile.js`

 * *Files identical despite different names*

### Comparing `ezhc-0.7.8/ezhc/script/json_parse.js` & `ezhc-0.7.9/ezhc/script/json_parse.js`

 * *Files identical despite different names*

### Comparing `ezhc-0.7.8/ezhc/script/template_disclaimer.html` & `ezhc-0.7.9/ezhc/script/template_disclaimer.html`

 * *Files identical despite different names*

### Comparing `ezhc-0.7.8/ezhc/script/themes/build_theme_json.ipynb` & `ezhc-0.7.9/ezhc/script/themes/build_theme_json.ipynb`

 * *Files identical despite different names*

### Comparing `ezhc-0.7.8/ezhc/script/themes/dark-blue.js` & `ezhc-0.7.9/ezhc/script/themes/dark-blue.js`

 * *Files identical despite different names*

### Comparing `ezhc-0.7.8/ezhc/script/themes/dark-blue.json` & `ezhc-0.7.9/ezhc/script/themes/dark-blue.json`

 * *Files identical despite different names*

### Comparing `ezhc-0.7.8/ezhc/script/themes/dark-green.js` & `ezhc-0.7.9/ezhc/script/themes/dark-green.js`

 * *Files identical despite different names*

### Comparing `ezhc-0.7.8/ezhc/script/themes/dark-green.json` & `ezhc-0.7.9/ezhc/script/themes/dark-green.json`

 * *Files identical despite different names*

### Comparing `ezhc-0.7.8/ezhc/script/themes/dark-unica.js` & `ezhc-0.7.9/ezhc/script/themes/dark-unica.js`

 * *Files identical despite different names*

### Comparing `ezhc-0.7.8/ezhc/script/themes/dark-unica.json` & `ezhc-0.7.9/ezhc/script/themes/dark-unica.json`

 * *Files identical despite different names*

### Comparing `ezhc-0.7.8/ezhc/script/themes/gray.js` & `ezhc-0.7.9/ezhc/script/themes/gray.js`

 * *Files identical despite different names*

### Comparing `ezhc-0.7.8/ezhc/script/themes/gray.json` & `ezhc-0.7.9/ezhc/script/themes/gray.json`

 * *Files identical despite different names*

### Comparing `ezhc-0.7.8/ezhc/script/themes/grid-light.js` & `ezhc-0.7.9/ezhc/script/themes/grid-light.js`

 * *Files identical despite different names*

### Comparing `ezhc-0.7.8/ezhc/script/themes/grid-light.json` & `ezhc-0.7.9/ezhc/script/themes/grid-light.json`

 * *Files identical despite different names*

### Comparing `ezhc-0.7.8/ezhc/script/themes/grid.js` & `ezhc-0.7.9/ezhc/script/themes/grid.js`

 * *Files identical despite different names*

### Comparing `ezhc-0.7.8/ezhc/script/themes/grid.json` & `ezhc-0.7.9/ezhc/script/themes/grid.json`

 * *Files identical despite different names*

### Comparing `ezhc-0.7.8/ezhc/script/themes/sand-signika.js` & `ezhc-0.7.9/ezhc/script/themes/sand-signika.js`

 * *Files identical despite different names*

### Comparing `ezhc-0.7.8/ezhc/script/themes/sand-signika.json` & `ezhc-0.7.9/ezhc/script/themes/sand-signika.json`

 * *Files identical despite different names*

### Comparing `ezhc-0.7.8/ezhc/script/themes/skies.js` & `ezhc-0.7.9/ezhc/script/themes/skies.js`

 * *Files identical despite different names*

### Comparing `ezhc-0.7.8/ezhc/script/themes/skies.json` & `ezhc-0.7.9/ezhc/script/themes/skies.json`

 * *Files identical despite different names*

### Comparing `ezhc-0.7.8/ezhc/script/tooltip_positioner_center_top.js` & `ezhc-0.7.9/ezhc/script/tooltip_positioner_center_top.js`

 * *Files identical despite different names*

### Comparing `ezhc-0.7.8/ezhc/script/tooltip_positioner_left_top.js` & `ezhc-0.7.9/ezhc/script/tooltip_positioner_left_top.js`

 * *Files identical despite different names*

### Comparing `ezhc-0.7.8/ezhc/script/tooltip_positioner_right_top.js` & `ezhc-0.7.9/ezhc/script/tooltip_positioner_right_top.js`

 * *Files identical despite different names*

### Comparing `ezhc-0.7.8/ezhc/scripts.py` & `ezhc-0.7.9/ezhc/scripts.py`

 * *Files identical despite different names*

### Comparing `ezhc-0.7.8/ezhc/series.py` & `ezhc-0.7.9/ezhc/series.py`

 * *Files identical despite different names*

### Comparing `ezhc-0.7.8/ezhc.egg-info/PKG-INFO` & `ezhc-0.7.9/ezhc.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 1.1
 Name: ezhc
-Version: 0.7.8
+Version: 0.7.9
 Summary: easy Highcharts & Highstock, dynamic plots from pandas dataframes in the Jupyter notebook
 Home-page: https://github.com/oscar6echo/ezhc
 Author: oscar6echo
 Author-email: olivier.borderies@gmail.com
 License: MIT
-Download-URL: https://github.com/oscar6echo/ezhc/tarball/0.7.8
+Download-URL: https://github.com/oscar6echo/ezhc/tarball/0.7.9
 Description: UNKNOWN
 Keywords: Highcharts,Highstock,pandas,notebook,javascript
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.5
```

### Comparing `ezhc-0.7.8/ezhc.egg-info/SOURCES.txt` & `ezhc-0.7.9/ezhc.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,13 @@
+.gitignore
 LICENSE
 MANIFEST.in
 README.md
+demo_ezhc.ipynb
+demo_ezhc_themes_and_global_options.ipynb
 requirements.txt
 setup.cfg
 setup.py
 ezhc/__init__.py
 ezhc/__meta__.py
 ezhc/_clock.py
 ezhc/_config.py
@@ -28,14 +31,17 @@
 ezhc.egg-info/not-zip-safe
 ezhc.egg-info/requires.txt
 ezhc.egg-info/top_level.txt
 ezhc/api/hc_object.json
 ezhc/api/hc_option.json
 ezhc/api/hs_object.json
 ezhc/api/hs_option.json
+ezhc/samples/build_data_world_population.py
+ezhc/samples/build_samples.py
+ezhc/samples/data_population.py
 ezhc/samples/df_bubble.csv
 ezhc/samples/df_heatmap.csv
 ezhc/samples/df_one_idx_one_col.csv
 ezhc/samples/df_one_idx_several_col.csv
 ezhc/samples/df_one_idx_several_col_2.csv
 ezhc/samples/df_one_idx_two_col.csv
 ezhc/samples/df_scatter.csv
```

### Comparing `ezhc-0.7.8/setup.py` & `ezhc-0.7.9/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # cf. https://pythonhosted.org/setuptools/setuptools.html
 
 # commands:
 # one liner
 # python setup.py sdist upload -r pypi
 # 2 steps
 # python setup.py sdist
-# twine upload dist/*
+# twine upload dist/* -r ezhc
 
 
 from setuptools import setup, find_packages
 from distutils.util import convert_path
 
 packages = find_packages()
 module = packages[0]
```

